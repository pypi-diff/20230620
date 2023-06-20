# Comparing `tmp/yellowdog-python-examples-6.0.1.tar.gz` & `tmp/yellowdog-python-examples-6.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yellowdog-python-examples-6.0.1.tar", last modified: Mon Jun 19 07:58:26 2023, max compression
+gzip compressed data, was "yellowdog-python-examples-6.0.2.tar", last modified: Tue Jun 20 15:24:16 2023, max compression
```

## Comparing `yellowdog-python-examples-6.0.1.tar` & `yellowdog-python-examples-6.0.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-06-19 07:58:26.677713 yellowdog-python-examples-6.0.1/
--rw-r--r--   0 pwt        (501) staff       (20)    11357 2022-11-18 20:55:26.000000 yellowdog-python-examples-6.0.1/LICENSE
--rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-06-19 07:58:26.677782 yellowdog-python-examples-6.0.1/PKG-INFO
--rw-r--r--   0 pwt        (501) staff       (20)      676 2022-11-22 08:58:59.000000 yellowdog-python-examples-6.0.1/PYPI_README.md
--rw-r--r--   0 pwt        (501) staff       (20)   109494 2023-06-19 07:57:31.000000 yellowdog-python-examples-6.0.1/README.md
--rw-r--r--   0 pwt        (501) staff       (20)     1806 2023-02-20 09:23:16.000000 yellowdog-python-examples-6.0.1/pyproject.toml
--rw-r--r--   0 pwt        (501) staff       (20)       46 2023-06-19 07:57:31.000000 yellowdog-python-examples-6.0.1/requirements.txt
--rw-r--r--   0 pwt        (501) staff       (20)     1366 2023-06-19 07:58:26.678058 yellowdog-python-examples-6.0.1/setup.cfg
--rw-r--r--   0 pwt        (501) staff       (20)      125 2023-02-14 10:40:48.000000 yellowdog-python-examples-6.0.1/setup.py
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-06-19 07:58:26.676720 yellowdog-python-examples-6.0.1/yd_commands/
--rw-r--r--   0 pwt        (501) staff       (20)       22 2023-06-19 07:57:31.000000 yellowdog-python-examples-6.0.1/yd_commands/__init__.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     3415 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.1/yd_commands/abort.py
--rwxr-xr-x   0 pwt        (501) staff       (20)      982 2023-01-31 15:59:12.000000 yellowdog-python-examples-6.0.1/yd_commands/admin.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    18382 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.1/yd_commands/args.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     5114 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.1/yd_commands/cancel.py
--rw-r--r--   0 pwt        (501) staff       (20)      579 2022-12-12 15:56:41.000000 yellowdog-python-examples-6.0.1/yd_commands/check_imports.py
--rw-r--r--   0 pwt        (501) staff       (20)     3757 2022-11-27 20:53:08.000000 yellowdog-python-examples-6.0.1/yd_commands/compact_json.py
--rw-r--r--   0 pwt        (501) staff       (20)    17400 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.1/yd_commands/config.py
--rw-r--r--   0 pwt        (501) staff       (20)     5019 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.1/yd_commands/config_keys.py
--rw-r--r--   0 pwt        (501) staff       (20)    12135 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.1/yd_commands/csv_data.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     1657 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.1/yd_commands/delete.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     3626 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.1/yd_commands/download.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     9251 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.1/yd_commands/instantiate.py
--rw-r--r--   0 pwt        (501) staff       (20)     3729 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.1/yd_commands/interactive.py
--rwxr-xr-x   0 pwt        (501) staff       (20)      749 2023-03-28 14:27:45.000000 yellowdog-python-examples-6.0.1/yd_commands/jsonnet2json.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     7798 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.1/yd_commands/list.py
--rw-r--r--   0 pwt        (501) staff       (20)     3000 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.1/yd_commands/object_utilities.py
--rw-r--r--   0 pwt        (501) staff       (20)     9525 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.1/yd_commands/printing.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    13218 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.1/yd_commands/provision.py
--rw-r--r--   0 pwt        (501) staff       (20)     1248 2023-05-03 10:27:28.000000 yellowdog-python-examples-6.0.1/yd_commands/provision_utils.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     1479 2023-02-14 10:40:48.000000 yellowdog-python-examples-6.0.1/yd_commands/reformat_json.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     3232 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.1/yd_commands/shutdown.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    40685 2023-06-19 07:57:31.000000 yellowdog-python-examples-6.0.1/yd_commands/submit.py
--rw-r--r--   0 pwt        (501) staff       (20)     6052 2023-05-03 10:27:28.000000 yellowdog-python-examples-6.0.1/yd_commands/submit_utils.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     2916 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.1/yd_commands/terminate.py
--rw-r--r--   0 pwt        (501) staff       (20)     1678 2022-12-07 08:38:57.000000 yellowdog-python-examples-6.0.1/yd_commands/type_check.py
--rw-r--r--   0 pwt        (501) staff       (20)     2237 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.1/yd_commands/upload.py
--rw-r--r--   0 pwt        (501) staff       (20)     3389 2023-06-17 13:30:23.000000 yellowdog-python-examples-6.0.1/yd_commands/upload_utils.py
--rw-r--r--   0 pwt        (501) staff       (20)     2177 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.1/yd_commands/validate_properties.py
--rw-r--r--   0 pwt        (501) staff       (20)    11037 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.1/yd_commands/variables.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     1247 2023-03-24 08:40:30.000000 yellowdog-python-examples-6.0.1/yd_commands/version.py
--rw-r--r--   0 pwt        (501) staff       (20)     2200 2023-04-19 15:22:46.000000 yellowdog-python-examples-6.0.1/yd_commands/wrapper.py
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-06-19 07:58:26.677599 yellowdog-python-examples-6.0.1/yellowdog_python_examples.egg-info/
--rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-06-19 07:58:26.000000 yellowdog-python-examples-6.0.1/yellowdog_python_examples.egg-info/PKG-INFO
--rw-r--r--   0 pwt        (501) staff       (20)     1187 2023-06-19 07:58:26.000000 yellowdog-python-examples-6.0.1/yellowdog_python_examples.egg-info/SOURCES.txt
--rw-r--r--   0 pwt        (501) staff       (20)        1 2023-06-19 07:58:26.000000 yellowdog-python-examples-6.0.1/yellowdog_python_examples.egg-info/dependency_links.txt
--rw-r--r--   0 pwt        (501) staff       (20)      574 2023-06-19 07:58:26.000000 yellowdog-python-examples-6.0.1/yellowdog_python_examples.egg-info/entry_points.txt
--rw-r--r--   0 pwt        (501) staff       (20)       61 2023-06-19 07:58:26.000000 yellowdog-python-examples-6.0.1/yellowdog_python_examples.egg-info/requires.txt
--rw-r--r--   0 pwt        (501) staff       (20)       12 2023-06-19 07:58:26.000000 yellowdog-python-examples-6.0.1/yellowdog_python_examples.egg-info/top_level.txt
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-06-20 15:24:16.870418 yellowdog-python-examples-6.0.2/
+-rw-r--r--   0 pwt        (501) staff       (20)    11357 2022-11-18 20:55:26.000000 yellowdog-python-examples-6.0.2/LICENSE
+-rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-06-20 15:24:16.870472 yellowdog-python-examples-6.0.2/PKG-INFO
+-rw-r--r--   0 pwt        (501) staff       (20)      676 2022-11-22 08:58:59.000000 yellowdog-python-examples-6.0.2/PYPI_README.md
+-rw-r--r--   0 pwt        (501) staff       (20)   110946 2023-06-20 15:23:19.000000 yellowdog-python-examples-6.0.2/README.md
+-rw-r--r--   0 pwt        (501) staff       (20)     1806 2023-02-20 09:23:16.000000 yellowdog-python-examples-6.0.2/pyproject.toml
+-rw-r--r--   0 pwt        (501) staff       (20)       62 2023-06-20 15:23:19.000000 yellowdog-python-examples-6.0.2/requirements.txt
+-rw-r--r--   0 pwt        (501) staff       (20)     1366 2023-06-20 15:24:16.870742 yellowdog-python-examples-6.0.2/setup.cfg
+-rw-r--r--   0 pwt        (501) staff       (20)      125 2023-02-14 10:40:48.000000 yellowdog-python-examples-6.0.2/setup.py
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-06-20 15:24:16.869529 yellowdog-python-examples-6.0.2/yd_commands/
+-rw-r--r--   0 pwt        (501) staff       (20)       22 2023-06-20 15:23:19.000000 yellowdog-python-examples-6.0.2/yd_commands/__init__.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     3415 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.2/yd_commands/abort.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)      982 2023-01-31 15:59:12.000000 yellowdog-python-examples-6.0.2/yd_commands/admin.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    18654 2023-06-20 15:23:19.000000 yellowdog-python-examples-6.0.2/yd_commands/args.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     5114 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.2/yd_commands/cancel.py
+-rw-r--r--   0 pwt        (501) staff       (20)      579 2022-12-12 15:56:41.000000 yellowdog-python-examples-6.0.2/yd_commands/check_imports.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3757 2022-11-27 20:53:08.000000 yellowdog-python-examples-6.0.2/yd_commands/compact_json.py
+-rw-r--r--   0 pwt        (501) staff       (20)    17539 2023-06-20 15:23:19.000000 yellowdog-python-examples-6.0.2/yd_commands/config.py
+-rw-r--r--   0 pwt        (501) staff       (20)     5062 2023-06-20 15:23:19.000000 yellowdog-python-examples-6.0.2/yd_commands/config_keys.py
+-rw-r--r--   0 pwt        (501) staff       (20)    12135 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.2/yd_commands/csv_data.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     1657 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.2/yd_commands/delete.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     3626 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.2/yd_commands/download.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     9251 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.2/yd_commands/instantiate.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3729 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.2/yd_commands/interactive.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)      749 2023-03-28 14:27:45.000000 yellowdog-python-examples-6.0.2/yd_commands/jsonnet2json.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     7798 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.2/yd_commands/list.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3000 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.2/yd_commands/object_utilities.py
+-rw-r--r--   0 pwt        (501) staff       (20)     9525 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.2/yd_commands/printing.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    13218 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.2/yd_commands/provision.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1248 2023-05-03 10:27:28.000000 yellowdog-python-examples-6.0.2/yd_commands/provision_utils.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     1479 2023-02-14 10:40:48.000000 yellowdog-python-examples-6.0.2/yd_commands/reformat_json.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     3232 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.2/yd_commands/shutdown.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    40685 2023-06-19 07:57:31.000000 yellowdog-python-examples-6.0.2/yd_commands/submit.py
+-rw-r--r--   0 pwt        (501) staff       (20)     6052 2023-05-03 10:27:28.000000 yellowdog-python-examples-6.0.2/yd_commands/submit_utils.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     2916 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.2/yd_commands/terminate.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1678 2022-12-07 08:38:57.000000 yellowdog-python-examples-6.0.2/yd_commands/type_check.py
+-rw-r--r--   0 pwt        (501) staff       (20)     2237 2023-06-20 14:36:54.000000 yellowdog-python-examples-6.0.2/yd_commands/upload.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3471 2023-06-20 15:23:19.000000 yellowdog-python-examples-6.0.2/yd_commands/upload_utils.py
+-rw-r--r--   0 pwt        (501) staff       (20)     2177 2023-06-09 10:27:25.000000 yellowdog-python-examples-6.0.2/yd_commands/validate_properties.py
+-rw-r--r--   0 pwt        (501) staff       (20)    11037 2023-05-16 09:40:32.000000 yellowdog-python-examples-6.0.2/yd_commands/variables.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     1247 2023-03-24 08:40:30.000000 yellowdog-python-examples-6.0.2/yd_commands/version.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3002 2023-06-20 15:23:19.000000 yellowdog-python-examples-6.0.2/yd_commands/wrapper.py
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-06-20 15:24:16.870316 yellowdog-python-examples-6.0.2/yellowdog_python_examples.egg-info/
+-rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-06-20 15:24:16.000000 yellowdog-python-examples-6.0.2/yellowdog_python_examples.egg-info/PKG-INFO
+-rw-r--r--   0 pwt        (501) staff       (20)     1187 2023-06-20 15:24:16.000000 yellowdog-python-examples-6.0.2/yellowdog_python_examples.egg-info/SOURCES.txt
+-rw-r--r--   0 pwt        (501) staff       (20)        1 2023-06-20 15:24:16.000000 yellowdog-python-examples-6.0.2/yellowdog_python_examples.egg-info/dependency_links.txt
+-rw-r--r--   0 pwt        (501) staff       (20)      574 2023-06-20 15:24:16.000000 yellowdog-python-examples-6.0.2/yellowdog_python_examples.egg-info/entry_points.txt
+-rw-r--r--   0 pwt        (501) staff       (20)       75 2023-06-20 15:24:16.000000 yellowdog-python-examples-6.0.2/yellowdog_python_examples.egg-info/requires.txt
+-rw-r--r--   0 pwt        (501) staff       (20)       12 2023-06-20 15:24:16.000000 yellowdog-python-examples-6.0.2/yellowdog_python_examples.egg-info/top_level.txt
```

### Comparing `yellowdog-python-examples-6.0.1/LICENSE` & `yellowdog-python-examples-6.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.1/PKG-INFO` & `yellowdog-python-examples-6.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yellowdog-python-examples
-Version: 6.0.1
+Version: 6.0.2
 Summary: Example Python commands using the YellowDog Python SDK
 Home-page: https://github.com/yellowdog/python-examples
 Author: YellowDog Limited
 Author-email: YellowDog Limited <support@yellowdog.co>
 Project-URL: Homepage, https://github.com/yellowdog/python-examples
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yellowdog-python-examples-6.0.1/PYPI_README.md` & `yellowdog-python-examples-6.0.2/PYPI_README.md`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.1/README.md` & `yellowdog-python-examples-6.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -22,6823 +22,6914 @@
 00000150: 2375 7361 6765 290a 2a20 5b43 6f6e 6669  #usage).* [Confi
 00000160: 6775 7261 7469 6f6e 5d28 2363 6f6e 6669  guration](#confi
 00000170: 6775 7261 7469 6f6e 290a 2a20 5b4e 616d  guration).* [Nam
 00000180: 696e 6720 5275 6c65 735d 2823 6e61 6d69  ing Rules](#nami
 00000190: 6e67 2d72 756c 6573 290a 2a20 5b43 6f6d  ng-rules).* [Com
 000001a0: 6d6f 6e20 5072 6f70 6572 7469 6573 5d28  mon Properties](
 000001b0: 2363 6f6d 6d6f 6e2d 7072 6f70 6572 7469  #common-properti
-000001c0: 6573 290a 2020 202a 205b 5370 6563 6966  es).   * [Specif
-000001d0: 7969 6e67 2043 6f6d 6d6f 6e20 5072 6f70  ying Common Prop
-000001e0: 6572 7469 6573 2075 7369 6e67 2074 6865  erties using the
-000001f0: 2043 6f6d 6d61 6e64 204c 696e 6520 6f72   Command Line or
-00000200: 2045 6e76 6972 6f6e 6d65 6e74 2056 6172   Environment Var
-00000210: 6961 626c 6573 5d28 2373 7065 6369 6679  iables](#specify
-00000220: 696e 672d 636f 6d6d 6f6e 2d70 726f 7065  ing-common-prope
-00000230: 7274 6965 732d 7573 696e 672d 7468 652d  rties-using-the-
-00000240: 636f 6d6d 616e 642d 6c69 6e65 2d6f 722d  command-line-or-
-00000250: 656e 7669 726f 6e6d 656e 742d 7661 7269  environment-vari
-00000260: 6162 6c65 7329 0a20 2020 2a20 5b56 6172  ables).   * [Var
-00000270: 6961 626c 6520 5375 6273 7469 7475 7469  iable Substituti
-00000280: 6f6e 7320 696e 2043 6f6d 6d6f 6e20 5072  ons in Common Pr
-00000290: 6f70 6572 7469 6573 5d28 2376 6172 6961  operties](#varia
-000002a0: 626c 652d 7375 6273 7469 7475 7469 6f6e  ble-substitution
-000002b0: 732d 696e 2d63 6f6d 6d6f 6e2d 7072 6f70  s-in-common-prop
-000002c0: 6572 7469 6573 290a 2a20 5b56 6172 6961  erties).* [Varia
-000002d0: 626c 6520 5375 6273 7469 7475 7469 6f6e  ble Substitution
-000002e0: 735d 2823 7661 7269 6162 6c65 2d73 7562  s](#variable-sub
-000002f0: 7374 6974 7574 696f 6e73 290a 2020 202a  stitutions).   *
-00000300: 205b 4465 6661 756c 7420 5661 7269 6162   [Default Variab
-00000310: 6c65 735d 2823 6465 6661 756c 742d 7661  les](#default-va
-00000320: 7269 6162 6c65 7329 0a20 2020 2a20 5b55  riables).   * [U
-00000330: 7365 722d 4465 6669 6e65 6420 5661 7269  ser-Defined Vari
-00000340: 6162 6c65 735d 2823 7573 6572 2d64 6566  ables](#user-def
-00000350: 696e 6564 2d76 6172 6961 626c 6573 290a  ined-variables).
-00000360: 2020 202a 205b 4e65 7374 6564 2056 6172     * [Nested Var
-00000370: 6961 626c 6573 5d28 236e 6573 7465 642d  iables](#nested-
-00000380: 7661 7269 6162 6c65 7329 0a2a 205b 576f  variables).* [Wo
-00000390: 726b 2052 6571 7569 7265 6d65 6e74 2050  rk Requirement P
-000003a0: 726f 7065 7274 6965 735d 2823 776f 726b  roperties](#work
-000003b0: 2d72 6571 7569 7265 6d65 6e74 2d70 726f  -requirement-pro
-000003c0: 7065 7274 6965 7329 0a20 2020 2a20 5b57  perties).   * [W
-000003d0: 6f72 6b20 5265 7175 6972 656d 656e 7420  ork Requirement 
-000003e0: 4a53 4f4e 2046 696c 6520 5374 7275 6374  JSON File Struct
-000003f0: 7572 655d 2823 776f 726b 2d72 6571 7569  ure](#work-requi
-00000400: 7265 6d65 6e74 2d6a 736f 6e2d 6669 6c65  rement-json-file
-00000410: 2d73 7472 7563 7475 7265 290a 2020 202a  -structure).   *
-00000420: 205b 5072 6f70 6572 7479 2049 6e68 6572   [Property Inher
-00000430: 6974 616e 6365 5d28 2370 726f 7065 7274  itance](#propert
-00000440: 792d 696e 6865 7269 7461 6e63 6529 0a20  y-inheritance). 
-00000450: 2020 2a20 5b57 6f72 6b20 5265 7175 6972    * [Work Requir
-00000460: 656d 656e 7420 5072 6f70 6572 7479 2044  ement Property D
-00000470: 6963 7469 6f6e 6172 795d 2823 776f 726b  ictionary](#work
-00000480: 2d72 6571 7569 7265 6d65 6e74 2d70 726f  -requirement-pro
-00000490: 7065 7274 792d 6469 6374 696f 6e61 7279  perty-dictionary
-000004a0: 290a 2020 202a 205b 4175 746f 6d61 7469  ).   * [Automati
-000004b0: 6320 5072 6f70 6572 7469 6573 5d28 2361  c Properties](#a
-000004c0: 7574 6f6d 6174 6963 2d70 726f 7065 7274  utomatic-propert
-000004d0: 6965 7329 0a20 2020 2020 202a 205b 576f  ies).      * [Wo
-000004e0: 726b 2052 6571 7569 7265 6d65 6e74 2c20  rk Requirement, 
-000004f0: 5461 736b 2047 726f 7570 2061 6e64 2054  Task Group and T
-00000500: 6173 6b20 4e61 6d69 6e67 5d28 2377 6f72  ask Naming](#wor
-00000510: 6b2d 7265 7175 6972 656d 656e 742d 7461  k-requirement-ta
-00000520: 736b 2d67 726f 7570 2d61 6e64 2d74 6173  sk-group-and-tas
-00000530: 6b2d 6e61 6d69 6e67 290a 2020 2020 2020  k-naming).      
-00000540: 2a20 5b54 6173 6b20 5479 7065 735d 2823  * [Task Types](#
-00000550: 7461 736b 2d74 7970 6573 290a 2020 2020  task-types).    
-00000560: 2020 2020 202a 205b 4261 7368 2c20 5079       * [Bash, Py
-00000570: 7468 6f6e 2c20 506f 7765 7253 6865 6c6c  thon, PowerShell
-00000580: 2061 6e64 2063 6d64 2f62 6174 2054 6173   and cmd/bat Tas
-00000590: 6b73 5d28 2362 6173 682d 7079 7468 6f6e  ks](#bash-python
-000005a0: 2d70 6f77 6572 7368 656c 6c2d 616e 642d  -powershell-and-
-000005b0: 636d 6462 6174 2d74 6173 6b73 290a 2020  cmdbat-tasks).  
-000005c0: 2020 2020 2020 202a 205b 446f 636b 6572         * [Docker
-000005d0: 2054 6173 6b73 5d28 2364 6f63 6b65 722d   Tasks](#docker-
-000005e0: 7461 736b 7329 0a20 2020 2020 2020 2020  tasks).         
-000005f0: 2a20 5b42 6173 682c 2050 7974 686f 6e2c  * [Bash, Python,
-00000600: 2050 6f77 6572 5368 656c 6c2c 2063 6d64   PowerShell, cmd
-00000610: 2f62 6174 2061 6e64 2044 6f63 6b65 7220  /bat and Docker 
-00000620: 7769 7468 6f75 7420 4175 746f 6d61 7469  without Automati
-00000630: 6320 5072 6f63 6573 7369 6e67 5d28 2362  c Processing](#b
-00000640: 6173 682d 7079 7468 6f6e 2d70 6f77 6572  ash-python-power
-00000650: 7368 656c 6c2d 636d 6462 6174 2d61 6e64  shell-cmdbat-and
-00000660: 2d64 6f63 6b65 722d 7769 7468 6f75 742d  -docker-without-
-00000670: 6175 746f 6d61 7469 632d 7072 6f63 6573  automatic-proces
-00000680: 7369 6e67 290a 2020 2020 2020 2a20 5b54  sing).      * [T
-00000690: 6173 6b20 436f 756e 7473 5d28 2374 6173  ask Counts](#tas
-000006a0: 6b2d 636f 756e 7473 290a 2020 202a 205b  k-counts).   * [
-000006b0: 4578 616d 706c 6573 5d28 2365 7861 6d70  Examples](#examp
-000006c0: 6c65 7329 0a20 2020 2020 202a 205b 544f  les).      * [TO
-000006d0: 4d4c 2050 726f 7065 7274 6965 7320 696e  ML Properties in
-000006e0: 2074 6865 2077 6f72 6b52 6571 7569 7265   the workRequire
-000006f0: 6d65 6e74 2053 6563 7469 6f6e 5d28 2374  ment Section](#t
-00000700: 6f6d 6c2d 7072 6f70 6572 7469 6573 2d69  oml-properties-i
-00000710: 6e2d 7468 652d 776f 726b 7265 7175 6972  n-the-workrequir
-00000720: 656d 656e 742d 7365 6374 696f 6e29 0a20  ement-section). 
-00000730: 2020 2020 202a 205b 4a53 4f4e 2050 726f       * [JSON Pro
-00000740: 7065 7274 6965 7320 6174 2074 6865 2057  perties at the W
-00000750: 6f72 6b20 5265 7175 6972 656d 656e 7420  ork Requirement 
-00000760: 4c65 7665 6c5d 2823 6a73 6f6e 2d70 726f  Level](#json-pro
-00000770: 7065 7274 6965 732d 6174 2d74 6865 2d77  perties-at-the-w
-00000780: 6f72 6b2d 7265 7175 6972 656d 656e 742d  ork-requirement-
-00000790: 6c65 7665 6c29 0a20 2020 2020 202a 205b  level).      * [
-000007a0: 4a53 4f4e 2050 726f 7065 7274 6965 7320  JSON Properties 
-000007b0: 6174 2074 6865 2054 6173 6b20 4772 6f75  at the Task Grou
-000007c0: 7020 4c65 7665 6c5d 2823 6a73 6f6e 2d70  p Level](#json-p
-000007d0: 726f 7065 7274 6965 732d 6174 2d74 6865  roperties-at-the
-000007e0: 2d74 6173 6b2d 6772 6f75 702d 6c65 7665  -task-group-leve
-000007f0: 6c29 0a20 2020 2020 202a 205b 4a53 4f4e  l).      * [JSON
-00000800: 2050 726f 7065 7274 6965 7320 6174 2074   Properties at t
-00000810: 6865 2054 6173 6b20 4c65 7665 6c5d 2823  he Task Level](#
-00000820: 6a73 6f6e 2d70 726f 7065 7274 6965 732d  json-properties-
-00000830: 6174 2d74 6865 2d74 6173 6b2d 6c65 7665  at-the-task-leve
-00000840: 6c29 0a20 2020 2a20 5b56 6172 6961 626c  l).   * [Variabl
-00000850: 6520 5375 6273 7469 7475 7469 6f6e 7320  e Substitutions 
-00000860: 696e 2057 6f72 6b20 5265 7175 6972 656d  in Work Requirem
-00000870: 656e 7420 5072 6f70 6572 7469 6573 5d28  ent Properties](
-00000880: 2376 6172 6961 626c 652d 7375 6273 7469  #variable-substi
-00000890: 7475 7469 6f6e 732d 696e 2d77 6f72 6b2d  tutions-in-work-
-000008a0: 7265 7175 6972 656d 656e 742d 7072 6f70  requirement-prop
-000008b0: 6572 7469 6573 290a 2020 2020 2020 2a20  erties).      * 
-000008c0: 5b54 6173 6b20 616e 6420 5461 736b 2047  [Task and Task G
-000008d0: 726f 7570 204e 616d 6520 5375 6273 7469  roup Name Substi
-000008e0: 7475 7469 6f6e 5d28 2374 6173 6b2d 616e  tution](#task-an
-000008f0: 642d 7461 736b 2d67 726f 7570 2d6e 616d  d-task-group-nam
-00000900: 652d 7375 6273 7469 7475 7469 6f6e 290a  e-substitution).
-00000910: 2020 2020 2020 2a20 5b57 6f72 6b20 5265        * [Work Re
-00000920: 7175 6972 656d 656e 7420 4e61 6d65 2053  quirement Name S
-00000930: 7562 7374 6974 7574 696f 6e5d 2823 776f  ubstitution](#wo
-00000940: 726b 2d72 6571 7569 7265 6d65 6e74 2d6e  rk-requirement-n
-00000950: 616d 652d 7375 6273 7469 7475 7469 6f6e  ame-substitution
-00000960: 290a 2020 202a 205b 4472 792d 5275 6e6e  ).   * [Dry-Runn
-00000970: 696e 6720 576f 726b 2052 6571 7569 7265  ing Work Require
-00000980: 6d65 6e74 2053 7562 6d69 7373 696f 6e73  ment Submissions
-00000990: 5d28 2364 7279 2d72 756e 6e69 6e67 2d77  ](#dry-running-w
-000009a0: 6f72 6b2d 7265 7175 6972 656d 656e 742d  ork-requirement-
-000009b0: 7375 626d 6973 7369 6f6e 7329 0a20 2020  submissions).   
-000009c0: 2020 202a 205b 5375 626d 6974 7469 6e67     * [Submitting
-000009d0: 2027 5261 7727 204a 534f 4e20 576f 726b   'Raw' JSON Work
-000009e0: 2052 6571 7569 7265 6d65 6e74 2053 7065   Requirement Spe
-000009f0: 6369 6669 6361 7469 6f6e 735d 2823 7375  cifications](#su
-00000a00: 626d 6974 7469 6e67 2d72 6177 2d6a 736f  bmitting-raw-jso
-00000a10: 6e2d 776f 726b 2d72 6571 7569 7265 6d65  n-work-requireme
-00000a20: 6e74 2d73 7065 6369 6669 6361 7469 6f6e  nt-specification
-00000a30: 7329 0a20 2020 2a20 5b46 696c 6520 5374  s).   * [File St
-00000a40: 6f72 6167 6520 4c6f 6361 7469 6f6e 7320  orage Locations 
-00000a50: 616e 6420 4669 6c65 2055 7361 6765 5d28  and File Usage](
-00000a60: 2366 696c 652d 7374 6f72 6167 652d 6c6f  #file-storage-lo
-00000a70: 6361 7469 6f6e 732d 616e 642d 6669 6c65  cations-and-file
-00000a80: 2d75 7361 6765 290a 2020 2020 2020 2a20  -usage).      * 
-00000a90: 5b46 696c 6573 2055 706c 6f61 6465 6420  [Files Uploaded 
-00000aa0: 746f 2074 6865 204f 626a 6563 7420 5374  to the Object St
-00000ab0: 6f72 6520 6672 6f6d 204c 6f63 616c 2053  ore from Local S
-00000ac0: 746f 7261 6765 5d28 2366 696c 6573 2d75  torage](#files-u
-00000ad0: 706c 6f61 6465 642d 746f 2d74 6865 2d6f  ploaded-to-the-o
-00000ae0: 626a 6563 742d 7374 6f72 652d 6672 6f6d  bject-store-from
-00000af0: 2d6c 6f63 616c 2d73 746f 7261 6765 290a  -local-storage).
-00000b00: 2020 2020 2020 2020 202a 205b 4669 6c65           * [File
-00000b10: 7320 696e 2074 6865 2069 6e70 7574 7320  s in the inputs 
-00000b20: 4c69 7374 5d28 2366 696c 6573 2d69 6e2d  List](#files-in-
-00000b30: 7468 652d 696e 7075 7473 2d6c 6973 7429  the-inputs-list)
-00000b40: 0a20 2020 2020 2020 2020 2a20 5b46 696c  .         * [Fil
-00000b50: 6573 2069 6e20 7468 6520 7570 6c6f 6164  es in the upload
-00000b60: 4669 6c65 7320 4c69 7374 5d28 2366 696c  Files List](#fil
-00000b70: 6573 2d69 6e2d 7468 652d 7570 6c6f 6164  es-in-the-upload
-00000b80: 6669 6c65 732d 6c69 7374 290a 2020 2020  files-list).    
-00000b90: 2020 2a20 5b46 696c 6520 4465 7065 6e64    * [File Depend
-00000ba0: 656e 6369 6573 2055 7369 6e67 2076 6572  encies Using ver
-00000bb0: 6966 7941 7453 7461 7274 2061 6e64 2076  ifyAtStart and v
-00000bc0: 6572 6966 7957 6169 745d 2823 6669 6c65  erifyWait](#file
-00000bd0: 2d64 6570 656e 6465 6e63 6965 732d 7573  -dependencies-us
-00000be0: 696e 672d 7665 7269 6679 6174 7374 6172  ing-verifyatstar
-00000bf0: 742d 616e 642d 7665 7269 6679 7761 6974  t-and-verifywait
-00000c00: 290a 2020 2020 2020 2a20 5b46 696c 6573  ).      * [Files
-00000c10: 2044 6f77 6e6c 6f61 6465 6420 5573 696e   Downloaded Usin
-00000c20: 6720 696e 7075 7473 4f70 7469 6f6e 616c  g inputsOptional
-00000c30: 5d28 2366 696c 6573 2d64 6f77 6e6c 6f61  ](#files-downloa
-00000c40: 6465 642d 7573 696e 672d 696e 7075 7473  ded-using-inputs
-00000c50: 6f70 7469 6f6e 616c 290a 2020 2020 2020  optional).      
-00000c60: 2a20 5b46 696c 6573 2044 6f77 6e6c 6f61  * [Files Downloa
-00000c70: 6465 6420 746f 2061 204e 6f64 6520 666f  ded to a Node fo
-00000c80: 7220 7573 6520 696e 2054 6173 6b20 4578  r use in Task Ex
-00000c90: 6563 7574 696f 6e5d 2823 6669 6c65 732d  ecution](#files-
-00000ca0: 646f 776e 6c6f 6164 6564 2d74 6f2d 612d  downloaded-to-a-
-00000cb0: 6e6f 6465 2d66 6f72 2d75 7365 2d69 6e2d  node-for-use-in-
-00000cc0: 7461 736b 2d65 7865 6375 7469 6f6e 290a  task-execution).
-00000cd0: 2020 2020 2020 2a20 5b46 696c 6573 2055        * [Files U
-00000ce0: 706c 6f61 6465 6420 6672 6f6d 2061 204e  ploaded from a N
-00000cf0: 6f64 6520 746f 2074 6865 204f 626a 6563  ode to the Objec
-00000d00: 7420 5374 6f72 6520 6166 7465 7220 5461  t Store after Ta
-00000d10: 736b 2045 7865 6375 7469 6f6e 5d28 2366  sk Execution](#f
-00000d20: 696c 6573 2d75 706c 6f61 6465 642d 6672  iles-uploaded-fr
-00000d30: 6f6d 2d61 2d6e 6f64 652d 746f 2d74 6865  om-a-node-to-the
-00000d40: 2d6f 626a 6563 742d 7374 6f72 652d 6166  -object-store-af
-00000d50: 7465 722d 7461 736b 2d65 7865 6375 7469  ter-task-executi
-00000d60: 6f6e 290a 2020 2020 2020 2a20 5b46 696c  on).      * [Fil
-00000d70: 6573 2044 6f77 6e6c 6f61 6465 6420 6672  es Downloaded fr
-00000d80: 6f6d 2074 6865 204f 626a 6563 7420 5374  om the Object St
-00000d90: 6f72 6520 746f 204c 6f63 616c 2053 746f  ore to Local Sto
-00000da0: 7261 6765 5d28 2366 696c 6573 2d64 6f77  rage](#files-dow
-00000db0: 6e6c 6f61 6465 642d 6672 6f6d 2d74 6865  nloaded-from-the
-00000dc0: 2d6f 626a 6563 742d 7374 6f72 652d 746f  -object-store-to
-00000dd0: 2d6c 6f63 616c 2d73 746f 7261 6765 290a  -local-storage).
-00000de0: 2020 202a 205b 5461 736b 2045 7865 6375     * [Task Execu
-00000df0: 7469 6f6e 2043 6f6e 7465 7874 5d28 2374  tion Context](#t
-00000e00: 6173 6b2d 6578 6563 7574 696f 6e2d 636f  ask-execution-co
-00000e10: 6e74 6578 7429 0a20 2020 2020 202a 205b  ntext).      * [
-00000e20: 5461 736b 2045 7865 6375 7469 6f6e 2053  Task Execution S
-00000e30: 7465 7073 5d28 2374 6173 6b2d 6578 6563  teps](#task-exec
-00000e40: 7574 696f 6e2d 7374 6570 7329 0a20 2020  ution-steps).   
-00000e50: 2020 202a 205b 5468 6520 5573 6572 2061     * [The User a
-00000e60: 6e64 2047 726f 7570 2075 7365 6420 666f  nd Group used fo
-00000e70: 7220 5461 736b 735d 2823 7468 652d 7573  r Tasks](#the-us
-00000e80: 6572 2d61 6e64 2d67 726f 7570 2d75 7365  er-and-group-use
-00000e90: 642d 666f 722d 7461 736b 7329 0a20 2020  d-for-tasks).   
-00000ea0: 2020 202a 205b 486f 6d65 2044 6972 6563     * [Home Direc
-00000eb0: 746f 7279 2066 6f72 2079 642d 6167 656e  tory for yd-agen
-00000ec0: 745d 2823 686f 6d65 2d64 6972 6563 746f  t](#home-directo
-00000ed0: 7279 2d66 6f72 2d79 642d 6167 656e 7429  ry-for-yd-agent)
-00000ee0: 0a20 2020 2020 202a 205b 5461 736b 2045  .      * [Task E
-00000ef0: 7865 6375 7469 6f6e 2044 6972 6563 746f  xecution Directo
-00000f00: 7279 5d28 2374 6173 6b2d 6578 6563 7574  ry](#task-execut
-00000f10: 696f 6e2d 6469 7265 6374 6f72 7929 0a20  ion-directory). 
-00000f20: 2020 2a20 5b53 7065 6369 6679 696e 6720    * [Specifying 
-00000f30: 576f 726b 2052 6571 7569 7265 6d65 6e74  Work Requirement
-00000f40: 7320 7573 696e 6720 4353 5620 4461 7461  s using CSV Data
-00000f50: 5d28 2373 7065 6369 6679 696e 672d 776f  ](#specifying-wo
-00000f60: 726b 2d72 6571 7569 7265 6d65 6e74 732d  rk-requirements-
-00000f70: 7573 696e 672d 6373 762d 6461 7461 290a  using-csv-data).
-00000f80: 2020 2020 2020 2a20 5b57 6f72 6b20 5265        * [Work Re
-00000f90: 7175 6972 656d 656e 7420 4353 5620 4461  quirement CSV Da
-00000fa0: 7461 2045 7861 6d70 6c65 5d28 2377 6f72  ta Example](#wor
-00000fb0: 6b2d 7265 7175 6972 656d 656e 742d 6373  k-requirement-cs
-00000fc0: 762d 6461 7461 2d65 7861 6d70 6c65 290a  v-data-example).
-00000fd0: 2020 2020 2020 2a20 5b43 5356 2056 6172        * [CSV Var
-00000fe0: 6961 626c 6520 5375 6273 7469 7475 7469  iable Substituti
-00000ff0: 6f6e 735d 2823 6373 762d 7661 7269 6162  ons](#csv-variab
-00001000: 6c65 2d73 7562 7374 6974 7574 696f 6e73  le-substitutions
-00001010: 290a 2020 2020 2020 2a20 5b50 726f 7065  ).      * [Prope
-00001020: 7274 7920 496e 6865 7269 7461 6e63 655d  rty Inheritance]
-00001030: 2823 7072 6f70 6572 7479 2d69 6e68 6572  (#property-inher
-00001040: 6974 616e 6365 2d31 290a 2020 2020 2020  itance-1).      
-00001050: 2a20 5b4d 756c 7469 706c 6520 5461 736b  * [Multiple Task
-00001060: 2047 726f 7570 7320 7573 696e 6720 4d75   Groups using Mu
-00001070: 6c74 6970 6c65 2043 5356 2046 696c 6573  ltiple CSV Files
-00001080: 5d28 236d 756c 7469 706c 652d 7461 736b  ](#multiple-task
-00001090: 2d67 726f 7570 732d 7573 696e 672d 6d75  -groups-using-mu
-000010a0: 6c74 6970 6c65 2d63 7376 2d66 696c 6573  ltiple-csv-files
-000010b0: 290a 2020 2020 2020 2a20 5b55 7369 6e67  ).      * [Using
-000010c0: 2043 5356 2044 6174 6120 7769 7468 2053   CSV Data with S
-000010d0: 696d 706c 652c 2054 4f4d 4c2d 4f6e 6c79  imple, TOML-Only
-000010e0: 2057 6f72 6b20 5265 7175 6972 656d 656e   Work Requiremen
-000010f0: 7420 5370 6563 6966 6963 6174 696f 6e73  t Specifications
-00001100: 5d28 2375 7369 6e67 2d63 7376 2d64 6174  ](#using-csv-dat
-00001110: 612d 7769 7468 2d73 696d 706c 652d 746f  a-with-simple-to
-00001120: 6d6c 2d6f 6e6c 792d 776f 726b 2d72 6571  ml-only-work-req
-00001130: 7569 7265 6d65 6e74 2d73 7065 6369 6669  uirement-specifi
-00001140: 6361 7469 6f6e 7329 0a20 2020 2020 202a  cations).      *
-00001150: 205b 496e 7370 6563 7469 6e67 2074 6865   [Inspecting the
-00001160: 2052 6573 756c 7473 206f 6620 4353 5620   Results of CSV 
-00001170: 5661 7269 6162 6c65 2053 7562 7374 6974  Variable Substit
-00001180: 7574 696f 6e5d 2823 696e 7370 6563 7469  ution](#inspecti
-00001190: 6e67 2d74 6865 2d72 6573 756c 7473 2d6f  ng-the-results-o
-000011a0: 662d 6373 762d 7661 7269 6162 6c65 2d73  f-csv-variable-s
-000011b0: 7562 7374 6974 7574 696f 6e29 0a2a 205b  ubstitution).* [
-000011c0: 576f 726b 6572 2050 6f6f 6c20 5072 6f70  Worker Pool Prop
-000011d0: 6572 7469 6573 5d28 2377 6f72 6b65 722d  erties](#worker-
-000011e0: 706f 6f6c 2d70 726f 7065 7274 6965 7329  pool-properties)
-000011f0: 0a20 2020 2a20 5b41 7574 6f6d 6174 6963  .   * [Automatic
-00001200: 2050 726f 7065 7274 6965 735d 2823 6175   Properties](#au
-00001210: 746f 6d61 7469 632d 7072 6f70 6572 7469  tomatic-properti
-00001220: 6573 2d31 290a 2020 202a 205b 544f 4d4c  es-1).   * [TOML
-00001230: 2050 726f 7065 7274 6965 7320 696e 2074   Properties in t
-00001240: 6865 2077 6f72 6b65 7250 6f6f 6c20 5365  he workerPool Se
-00001250: 6374 696f 6e5d 2823 746f 6d6c 2d70 726f  ction](#toml-pro
-00001260: 7065 7274 6965 732d 696e 2d74 6865 2d77  perties-in-the-w
-00001270: 6f72 6b65 7270 6f6f 6c2d 7365 6374 696f  orkerpool-sectio
-00001280: 6e29 0a20 2020 2a20 5b57 6f72 6b65 7220  n).   * [Worker 
-00001290: 506f 6f6c 2053 7065 6369 6669 6361 7469  Pool Specificati
-000012a0: 6f6e 2055 7369 6e67 204a 534f 4e20 446f  on Using JSON Do
-000012b0: 6375 6d65 6e74 735d 2823 776f 726b 6572  cuments](#worker
-000012c0: 2d70 6f6f 6c2d 7370 6563 6966 6963 6174  -pool-specificat
-000012d0: 696f 6e2d 7573 696e 672d 6a73 6f6e 2d64  ion-using-json-d
-000012e0: 6f63 756d 656e 7473 290a 2020 2020 2020  ocuments).      
-000012f0: 2a20 5b57 6f72 6b65 7220 506f 6f6c 204a  * [Worker Pool J
-00001300: 534f 4e20 4578 616d 706c 6573 5d28 2377  SON Examples](#w
-00001310: 6f72 6b65 722d 706f 6f6c 2d6a 736f 6e2d  orker-pool-json-
-00001320: 6578 616d 706c 6573 290a 2020 2020 2020  examples).      
-00001330: 2a20 5b54 4f4d 4c20 5072 6f70 6572 7469  * [TOML Properti
-00001340: 6573 2049 6e68 6572 6974 6564 2062 7920  es Inherited by 
-00001350: 576f 726b 6572 2050 6f6f 6c20 4a53 4f4e  Worker Pool JSON
-00001360: 2053 7065 6369 6669 6361 7469 6f6e 735d   Specifications]
-00001370: 2823 746f 6d6c 2d70 726f 7065 7274 6965  (#toml-propertie
-00001380: 732d 696e 6865 7269 7465 642d 6279 2d77  s-inherited-by-w
-00001390: 6f72 6b65 722d 706f 6f6c 2d6a 736f 6e2d  orker-pool-json-
-000013a0: 7370 6563 6966 6963 6174 696f 6e73 290a  specifications).
-000013b0: 2020 202a 205b 5661 7269 6162 6c65 2053     * [Variable S
-000013c0: 7562 7374 6974 7574 696f 6e73 2069 6e20  ubstitutions in 
-000013d0: 576f 726b 6572 2050 6f6f 6c20 5072 6f70  Worker Pool Prop
-000013e0: 6572 7469 6573 5d28 2376 6172 6961 626c  erties](#variabl
-000013f0: 652d 7375 6273 7469 7475 7469 6f6e 732d  e-substitutions-
-00001400: 696e 2d77 6f72 6b65 722d 706f 6f6c 2d70  in-worker-pool-p
-00001410: 726f 7065 7274 6965 7329 0a20 2020 2a20  roperties).   * 
-00001420: 5b44 7279 2d52 756e 6e69 6e67 2057 6f72  [Dry-Running Wor
-00001430: 6b65 7220 506f 6f6c 2050 726f 7669 7369  ker Pool Provisi
-00001440: 6f6e 696e 675d 2823 6472 792d 7275 6e6e  oning](#dry-runn
-00001450: 696e 672d 776f 726b 6572 2d70 6f6f 6c2d  ing-worker-pool-
-00001460: 7072 6f76 6973 696f 6e69 6e67 290a 2a20  provisioning).* 
-00001470: 5b4a 736f 6e6e 6574 2053 7570 706f 7274  [Jsonnet Support
-00001480: 5d28 236a 736f 6e6e 6574 2d73 7570 706f  ](#jsonnet-suppo
-00001490: 7274 290a 2020 202a 205b 4a73 6f6e 6e65  rt).   * [Jsonne
-000014a0: 7420 496e 7374 616c 6c61 7469 6f6e 5d28  t Installation](
-000014b0: 236a 736f 6e6e 6574 2d69 6e73 7461 6c6c  #jsonnet-install
-000014c0: 6174 696f 6e29 0a20 2020 2a20 5b56 6172  ation).   * [Var
-000014d0: 6961 626c 6520 5375 6273 7469 7475 7469  iable Substituti
-000014e0: 6f6e 7320 696e 204a 736f 6e6e 6574 2046  ons in Jsonnet F
-000014f0: 696c 6573 5d28 2376 6172 6961 626c 652d  iles](#variable-
-00001500: 7375 6273 7469 7475 7469 6f6e 732d 696e  substitutions-in
-00001510: 2d6a 736f 6e6e 6574 2d66 696c 6573 290a  -jsonnet-files).
-00001520: 2020 202a 205b 4368 6563 6b69 6e67 204a     * [Checking J
-00001530: 736f 6e6e 6574 2050 726f 6365 7373 696e  sonnet Processin
-00001540: 675d 2823 6368 6563 6b69 6e67 2d6a 736f  g](#checking-jso
-00001550: 6e6e 6574 2d70 726f 6365 7373 696e 6729  nnet-processing)
-00001560: 0a20 2020 2a20 5b4a 736f 6e6e 6574 2045  .   * [Jsonnet E
-00001570: 7861 6d70 6c65 5d28 236a 736f 6e6e 6574  xample](#jsonnet
-00001580: 2d65 7861 6d70 6c65 290a 2a20 5b43 6f6d  -example).* [Com
-00001590: 6d61 6e64 204c 6973 745d 2823 636f 6d6d  mand List](#comm
-000015a0: 616e 642d 6c69 7374 290a 2020 202a 205b  and-list).   * [
-000015b0: 7964 2d73 7562 6d69 745d 2823 7964 2d73  yd-submit](#yd-s
-000015c0: 7562 6d69 7429 0a20 2020 2a20 5b79 642d  ubmit).   * [yd-
-000015d0: 7072 6f76 6973 696f 6e5d 2823 7964 2d70  provision](#yd-p
-000015e0: 726f 7669 7369 6f6e 290a 2020 202a 205b  rovision).   * [
-000015f0: 7964 2d63 616e 6365 6c5d 2823 7964 2d63  yd-cancel](#yd-c
-00001600: 616e 6365 6c29 0a20 2020 2a20 5b79 642d  ancel).   * [yd-
-00001610: 6162 6f72 745d 2823 7964 2d61 626f 7274  abort](#yd-abort
-00001620: 290a 2020 202a 205b 7964 2d64 6f77 6e6c  ).   * [yd-downl
-00001630: 6f61 645d 2823 7964 2d64 6f77 6e6c 6f61  oad](#yd-downloa
-00001640: 6429 0a20 2020 2a20 5b79 642d 6465 6c65  d).   * [yd-dele
-00001650: 7465 5d28 2379 642d 6465 6c65 7465 290a  te](#yd-delete).
-00001660: 2020 202a 205b 7964 2d75 706c 6f61 645d     * [yd-upload]
-00001670: 2823 7964 2d75 706c 6f61 6429 0a20 2020  (#yd-upload).   
-00001680: 2a20 5b79 642d 7368 7574 646f 776e 5d28  * [yd-shutdown](
-00001690: 2379 642d 7368 7574 646f 776e 290a 2020  #yd-shutdown).  
-000016a0: 202a 205b 7964 2d69 6e73 7461 6e74 6961   * [yd-instantia
-000016b0: 7465 5d28 2379 642d 696e 7374 616e 7469  te](#yd-instanti
-000016c0: 6174 6529 0a20 2020 2020 202a 205b 5465  ate).      * [Te
-000016d0: 7374 2d52 756e 6e69 6e67 2061 2044 796e  st-Running a Dyn
-000016e0: 616d 6963 2054 656d 706c 6174 655d 2823  amic Template](#
-000016f0: 7465 7374 2d72 756e 6e69 6e67 2d61 2d64  test-running-a-d
-00001700: 796e 616d 6963 2d74 656d 706c 6174 6529  ynamic-template)
-00001710: 0a20 2020 2a20 5b79 642d 7465 726d 696e  .   * [yd-termin
-00001720: 6174 655d 2823 7964 2d74 6572 6d69 6e61  ate](#yd-termina
-00001730: 7465 290a 0a3c 212d 2d20 4164 6465 6420  te)..<!-- Added 
-00001740: 6279 3a20 7077 742c 2061 743a 2053 6174  by: pwt, at: Sat
-00001750: 204a 756e 2031 3720 3134 3a33 373a 3439   Jun 17 14:37:49
-00001760: 2042 5354 2032 3032 3320 2d2d 3e0a 0a3c   BST 2023 -->..<
-00001770: 212d 2d74 652d 2d3e 0a0a 2320 4f76 6572  !--te-->..# Over
-00001780: 7669 6577 0a0a 5468 6973 2072 6570 6f73  view..This repos
-00001790: 6974 6f72 7920 636f 6e74 6169 6e73 2061  itory contains a
-000017a0: 2073 6574 206f 6620 6578 616d 706c 6520   set of example 
-000017b0: 5079 7468 6f6e 2073 6372 6970 7473 2066  Python scripts f
-000017c0: 6f72 2069 6e74 6572 6163 7469 6e67 2077  or interacting w
-000017d0: 6974 6820 7468 6520 5965 6c6c 6f77 446f  ith the YellowDo
-000017e0: 6720 506c 6174 666f 726d 2e20 5468 6520  g Platform. The 
-000017f0: 7363 7269 7074 7320 7573 6520 7468 6520  scripts use the 
-00001800: 2a2a 5b59 656c 6c6f 7744 6f67 2050 7974  **[YellowDog Pyt
-00001810: 686f 6e20 5344 4b5d 2868 7474 7073 3a2f  hon SDK](https:/
-00001820: 2f64 6f63 732e 7965 6c6c 6f77 646f 672e  /docs.yellowdog.
-00001830: 636f 2f61 7069 2f70 7974 686f 6e2f 696e  co/api/python/in
-00001840: 6465 782e 6874 6d6c 292a 2a2c 2074 6865  dex.html)**, the
-00001850: 2063 6f64 6520 666f 7220 7768 6963 6820   code for which 
-00001860: 6361 6e20 6265 2066 6f75 6e64 205b 6f6e  can be found [on
-00001870: 2047 6974 4875 625d 2868 7474 7073 3a2f   GitHub](https:/
-00001880: 2f67 6974 6875 622e 636f 6d2f 7965 6c6c  /github.com/yell
-00001890: 6f77 646f 672f 7965 6c6c 6f77 646f 672d  owdog/yellowdog-
-000018a0: 7364 6b2d 7079 7468 6f6e 2d70 7562 6c69  sdk-python-publi
-000018b0: 6329 2e0a 0a0a 2a28 4e6f 7465 3a20 7468  c)....*(Note: th
-000018c0: 6573 6520 7363 7269 7074 7320 6172 6520  ese scripts are 
-000018d0: 696e 7465 6e64 6564 2074 6f20 6265 2061  intended to be a
-000018e0: 2068 656c 7066 756c 2073 7461 7274 696e   helpful startin
-000018f0: 6720 706f 696e 7420 666f 7220 6578 7065  g point for expe
-00001900: 7269 6d65 6e74 696e 6720 7769 7468 2074  rimenting with t
-00001910: 6865 2059 656c 6c6f 7744 6f67 2050 6c61  he YellowDog Pla
-00001920: 7466 6f72 6d2e 2054 6865 7920 6172 6520  tform. They are 
-00001930: 6e6f 7420 6173 7375 7265 6420 746f 2062  not assured to b
-00001940: 6520 6f66 2070 726f 6475 6374 696f 6e20  e of production 
-00001950: 7175 616c 6974 7920 6e6f 7220 646f 2074  quality nor do t
-00001960: 6865 7920 7265 7072 6573 656e 7420 6120  hey represent a 
-00001970: 7374 616e 6461 7264 206f 7220 7265 636f  standard or reco
-00001980: 6d6d 656e 6465 6420 6d65 7468 6f64 2066  mmended method f
-00001990: 6f72 2075 7369 6e67 2059 656c 6c6f 7744  or using YellowD
-000019a0: 6f67 2e29 2a0a 0a54 6869 7320 646f 6375  og.)*..This docu
-000019b0: 6d65 6e74 6174 696f 6e20 7368 6f75 6c64  mentation should
-000019c0: 2062 6520 7265 6164 2069 6e20 636f 6e6a   be read in conj
-000019d0: 756e 6374 696f 6e20 7769 7468 2074 6865  unction with the
-000019e0: 206d 6169 6e20 2a2a 5b59 656c 6c6f 7744   main **[YellowD
-000019f0: 6f67 2044 6f63 756d 656e 7461 7469 6f6e  og Documentation
-00001a00: 5d28 6874 7470 733a 2f2f 646f 6373 2e79  ](https://docs.y
-00001a10: 656c 6c6f 7764 6f67 2e63 6f29 2a2a 2c20  ellowdog.co)**, 
-00001a20: 7768 6963 6820 7072 6f76 6964 6573 2061  which provides a
-00001a30: 2063 6f6d 7072 6568 656e 7369 7665 2064   comprehensive d
-00001a40: 6573 6372 6970 7469 6f6e 206f 6620 7468  escription of th
-00001a50: 6520 636f 6e63 6570 7473 2061 6e64 206f  e concepts and o
-00001a60: 7065 7261 7469 6f6e 206f 6620 7468 6520  peration of the 
-00001a70: 5965 6c6c 6f77 446f 6720 506c 6174 666f  YellowDog Platfo
-00001a80: 726d 2e0a 0a54 656d 706c 6174 6520 736f  rm...Template so
-00001a90: 6c75 7469 6f6e 7320 666f 7220 6578 7065  lutions for expe
-00001aa0: 7269 6d65 6e74 696e 6720 7769 7468 2074  rimenting with t
-00001ab0: 6865 7365 2073 6372 6970 7473 2063 616e  hese scripts can
-00001ac0: 2062 6520 666f 756e 6420 696e 2074 6865   be found in the
-00001ad0: 202a 2a5b 7079 7468 6f6e 2d65 7861 6d70   **[python-examp
-00001ae0: 6c65 732d 7465 6d70 6c61 7465 735d 2868  les-templates](h
-00001af0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001b00: 6d2f 7965 6c6c 6f77 646f 672f 7079 7468  m/yellowdog/pyth
-00001b10: 6f6e 2d65 7861 6d70 6c65 732d 7465 6d70  on-examples-temp
-00001b20: 6c61 7465 7329 2a2a 2072 6570 6f73 6974  lates)** reposit
-00001b30: 6f72 792e 0a0a 5468 6520 7363 7269 7074  ory...The script
-00001b40: 7320 7072 6f76 6964 6520 7468 6520 666f  s provide the fo
-00001b50: 6c6c 6f77 696e 6720 6361 7061 6269 6c69  llowing capabili
-00001b60: 7469 6573 3a0a 0a2d 202a 2a50 726f 7669  ties:..- **Provi
-00001b70: 7369 6f6e 696e 672a 2a20 576f 726b 6572  sioning** Worker
-00001b80: 2050 6f6f 6c73 2077 6974 6820 7468 6520   Pools with the 
-00001b90: 2a2a 6079 642d 7072 6f76 6973 696f 6e60  **`yd-provision`
-00001ba0: 2a2a 2063 6f6d 6d61 6e64 0a2d 202a 2a53  ** command.- **S
-00001bb0: 7562 6d69 7474 696e 672a 2a20 576f 726b  ubmitting** Work
-00001bc0: 2052 6571 7569 7265 6d65 6e74 7320 7769   Requirements wi
-00001bd0: 7468 2074 6865 202a 2a60 7964 2d73 7562  th the **`yd-sub
-00001be0: 6d69 7460 2a2a 2063 6f6d 6d61 6e64 0a2d  mit`** command.-
-00001bf0: 202a 2a55 706c 6f61 6469 6e67 2a2a 2066   **Uploading** f
-00001c00: 696c 6573 2074 6f20 7468 6520 5965 6c6c  iles to the Yell
-00001c10: 6f77 446f 6720 4f62 6a65 6374 2053 746f  owDog Object Sto
-00001c20: 7265 2077 6974 6820 7468 6520 2a2a 6079  re with the **`y
-00001c30: 642d 7570 6c6f 6164 602a 2a20 636f 6d6d  d-upload`** comm
-00001c40: 616e 640a 2d20 2a2a 496e 7374 616e 7469  and.- **Instanti
-00001c50: 6174 696e 672a 2a20 436f 6d70 7574 6520  ating** Compute 
-00001c60: 5265 7175 6972 656d 656e 7473 2077 6974  Requirements wit
-00001c70: 6820 7468 6520 2a2a 6079 642d 696e 7374  h the **`yd-inst
-00001c80: 616e 7469 6174 6560 2a2a 2063 6f6d 6d61  antiate`** comma
-00001c90: 6e64 0a2d 202a 2a44 6f77 6e6c 6f61 6469  nd.- **Downloadi
-00001ca0: 6e67 2a2a 2052 6573 756c 7473 2066 726f  ng** Results fro
-00001cb0: 6d20 7468 6520 5965 6c6c 6f77 446f 6720  m the YellowDog 
-00001cc0: 4f62 6a65 6374 2053 746f 7265 2077 6974  Object Store wit
-00001cd0: 6820 7468 6520 2a2a 6079 642d 646f 776e  h the **`yd-down
-00001ce0: 6c6f 6164 602a 2a20 636f 6d6d 616e 640a  load`** command.
-00001cf0: 2d20 2a2a 4162 6f72 7469 6e67 2a2a 2072  - **Aborting** r
-00001d00: 756e 6e69 6e67 2054 6173 6b73 2077 6974  unning Tasks wit
-00001d10: 6820 7468 6520 2a2a 6079 642d 6162 6f72  h the **`yd-abor
-00001d20: 7460 2a2a 2063 6f6d 6d61 6e64 0a2d 202a  t`** command.- *
-00001d30: 2a43 616e 6365 6c6c 696e 672a 2a20 576f  *Cancelling** Wo
-00001d40: 726b 2052 6571 7569 7265 6d65 6e74 7320  rk Requirements 
-00001d50: 7769 7468 2074 6865 202a 2a60 7964 2d63  with the **`yd-c
-00001d60: 616e 6365 6c60 2a2a 2063 6f6d 6d61 6e64  ancel`** command
-00001d70: 0a2d 202a 2a53 6875 7474 696e 6720 446f  .- **Shutting Do
-00001d80: 776e 2a2a 2057 6f72 6b65 7220 506f 6f6c  wn** Worker Pool
-00001d90: 7320 7769 7468 2074 6865 202a 2a60 7964  s with the **`yd
-00001da0: 2d73 6875 7464 6f77 6e60 2a2a 2063 6f6d  -shutdown`** com
-00001db0: 6d61 6e64 0a2d 202a 2a54 6572 6d69 6e61  mand.- **Termina
-00001dc0: 7469 6e67 2a2a 2043 6f6d 7075 7465 2052  ting** Compute R
-00001dd0: 6571 7569 7265 6d65 6e74 7320 7769 7468  equirements with
-00001de0: 2074 6865 202a 2a60 7964 2d74 6572 6d69   the **`yd-termi
-00001df0: 6e61 7465 602a 2a20 636f 6d6d 616e 640a  nate`** command.
-00001e00: 2d20 2a2a 4465 6c65 7469 6e67 2a2a 206f  - **Deleting** o
-00001e10: 626a 6563 7473 2069 6e20 7468 6520 5965  bjects in the Ye
-00001e20: 6c6c 6f77 446f 6720 4f62 6a65 6374 2053  llowDog Object S
-00001e30: 746f 7265 2077 6974 6820 7468 6520 2a2a  tore with the **
-00001e40: 6079 642d 6465 6c65 7465 602a 2a20 636f  `yd-delete`** co
-00001e50: 6d6d 616e 640a 0a54 6865 206f 7065 7261  mmand..The opera
-00001e60: 7469 6f6e 206f 6620 7468 6520 636f 6d6d  tion of the comm
-00001e70: 616e 6473 2069 7320 636f 6e74 726f 6c6c  ands is controll
-00001e80: 6564 2075 7369 6e67 2054 4f4d 4c20 636f  ed using TOML co
-00001e90: 6e66 6967 7572 6174 696f 6e20 6669 6c65  nfiguration file
-00001ea0: 732e 2049 6e20 6164 6469 7469 6f6e 2c20  s. In addition, 
-00001eb0: 576f 726b 2052 6571 7569 7265 6d65 6e74  Work Requirement
-00001ec0: 7320 616e 6420 576f 726b 6572 2050 6f6f  s and Worker Poo
-00001ed0: 6c73 2063 616e 2062 6520 6465 6669 6e65  ls can be define
-00001ee0: 6420 7573 696e 6720 4a53 4f4e 2066 696c  d using JSON fil
-00001ef0: 6573 2070 726f 7669 6469 6e67 2065 7874  es providing ext
-00001f00: 656e 7369 7665 2063 6f6e 6669 6775 7261  ensive configura
-00001f10: 6269 6c69 7479 2e0a 0a23 2059 656c 6c6f  bility...# Yello
-00001f20: 7744 6f67 2050 7265 7265 7175 6973 6974  wDog Prerequisit
-00001f30: 6573 0a0a 546f 2073 7562 6d69 7420 2a2a  es..To submit **
-00001f40: 576f 726b 2052 6571 7569 7265 6d65 6e74  Work Requirement
-00001f50: 732a 2a20 746f 2059 656c 6c6f 7744 6f67  s** to YellowDog
-00001f60: 2066 6f72 2070 726f 6365 7373 696e 6720   for processing 
-00001f70: 6279 2043 6f6e 6669 6775 7265 6420 576f  by Configured Wo
-00001f80: 726b 6572 2050 6f6f 6c73 2028 6f6e 2d70  rker Pools (on-p
-00001f90: 7265 6d69 7365 2920 616e 642f 6f72 2050  remise) and/or P
-00001fa0: 726f 7669 7369 6f6e 6564 2057 6f72 6b65  rovisioned Worke
-00001fb0: 7220 506f 6f6c 7320 2863 6c6f 7564 2d70  r Pools (cloud-p
-00001fc0: 726f 7669 7369 6f6e 6564 2072 6573 6f75  rovisioned resou
-00001fd0: 7263 6573 292c 2079 6f75 276c 6c20 6e65  rces), you'll ne
-00001fe0: 6564 3a0a 0a31 2e20 4120 5965 6c6c 6f77  ed:..1. A Yellow
-00001ff0: 446f 6720 506c 6174 666f 726d 2041 6363  Dog Platform Acc
-00002000: 6f75 6e74 2e0a 0a0a 322e 2041 6e20 4170  ount....2. An Ap
-00002010: 706c 6963 6174 696f 6e20 4b65 7920 2620  plication Key & 
-00002020: 5365 6372 6574 3a20 696e 2074 6865 202a  Secret: in the *
-00002030: 2a41 6363 6f75 6e74 732a 2a20 7365 6374  *Accounts** sect
-00002040: 696f 6e20 756e 6465 7220 7468 6520 2a2a  ion under the **
-00002050: 4170 706c 6963 6174 696f 6e73 2a2a 2074  Applications** t
-00002060: 6162 2069 6e20 7468 6520 5b59 656c 6c6f  ab in the [Yello
-00002070: 7744 6f67 2050 6f72 7461 6c5d 2868 7474  wDog Portal](htt
-00002080: 7073 3a2f 2f70 6f72 7461 6c2e 7965 6c6c  ps://portal.yell
-00002090: 6f77 646f 672e 636f 2f23 2f61 6363 6f75  owdog.co/#/accou
-000020a0: 6e74 2f61 7070 6c69 6361 7469 6f6e 7329  nt/applications)
-000020b0: 2c20 7573 6520 7468 6520 2a2a 4164 6420  , use the **Add 
-000020c0: 4170 706c 6963 6174 696f 6e2a 2a20 6275  Application** bu
-000020d0: 7474 6f6e 2074 6f20 6372 6561 7465 2061  tton to create a
-000020e0: 206e 6577 2041 7070 6c69 6361 7469 6f6e   new Application
-000020f0: 2c20 616e 6420 6d61 6b65 2061 206e 6f74  , and make a not
-00002100: 6520 6f66 2069 7473 202a 2a4b 6579 2a2a  e of its **Key**
-00002110: 2061 6e64 202a 2a53 6563 7265 742a 2a20   and **Secret** 
-00002120: 2874 6865 7365 2077 696c 6c20 6f6e 6c79  (these will only
-00002130: 2062 6520 6469 7370 6c61 7965 6420 6f6e   be displayed on
-00002140: 6365 292e 0a0a 0a54 6f20 6372 6561 7465  ce)....To create
-00002150: 202a 2a50 726f 7669 7369 6f6e 6564 2057   **Provisioned W
-00002160: 6f72 6b65 7220 506f 6f6c 732a 2a2c 2079  orker Pools**, y
-00002170: 6f75 276c 6c20 6e65 6564 3a0a 0a33 2e20  ou'll need:..3. 
-00002180: 4120 2a2a 4b65 7972 696e 672a 2a20 6372  A **Keyring** cr
-00002190: 6561 7465 6420 7669 6120 7468 6520 5965  eated via the Ye
-000021a0: 6c6c 6f77 446f 6720 506f 7274 616c 2c20  llowDog Portal, 
-000021b0: 7769 7468 2061 6363 6573 7320 746f 2043  with access to C
-000021c0: 6c6f 7564 2050 726f 7669 6465 7220 6372  loud Provider cr
-000021d0: 6564 656e 7469 616c 7320 6173 2072 6571  edentials as req
-000021e0: 7569 7265 642e 2054 6865 2041 7070 6c69  uired. The Appli
-000021f0: 6361 7469 6f6e 206d 7573 7420 6265 2067  cation must be g
-00002200: 7261 6e74 6564 2061 6363 6573 7320 746f  ranted access to
-00002210: 2074 6865 204b 6579 7269 6e67 2e0a 0a0a   the Keyring....
-00002220: 342e 204f 6e65 206f 7220 6d6f 7265 202a  4. One or more *
-00002230: 2a43 6f6d 7075 7465 2053 6f75 7263 6573  *Compute Sources
-00002240: 2a2a 2064 6566 696e 6564 2c20 616e 6420  ** defined, and 
-00002250: 6120 2a2a 436f 6d70 7574 6520 5265 7175  a **Compute Requ
-00002260: 6972 656d 656e 7420 5465 6d70 6c61 7465  irement Template
-00002270: 2a2a 2063 7265 6174 6564 2e20 5468 6520  ** created. The 
-00002280: 696d 6167 6573 2075 7365 6420 6279 2069  images used by i
-00002290: 6e73 7461 6e63 6573 206d 7573 7420 696e  nstances must in
-000022a0: 636c 7564 6520 7468 6520 5965 6c6c 6f77  clude the Yellow
-000022b0: 446f 6720 6167 656e 742c 2063 6f6e 6669  Dog agent, confi
-000022c0: 6775 7265 6420 7769 7468 2074 6865 2054  gured with the T
-000022d0: 6173 6b20 5479 7065 2873 2920 746f 206d  ask Type(s) to m
-000022e0: 6174 6368 2074 6865 2057 6f72 6b20 5265  atch the Work Re
-000022f0: 7175 6972 656d 656e 7473 2074 6f20 6265  quirements to be
-00002300: 2073 7562 6d69 7474 6564 2e0a 0a54 6f20   submitted...To 
-00002310: 7365 7420 7570 202a 2a43 6f6e 6669 6775  set up **Configu
-00002320: 7265 6420 576f 726b 6572 2050 6f6f 6c73  red Worker Pools
-00002330: 2a2a 2c20 796f 7527 6c6c 206e 6565 643a  **, you'll need:
-00002340: 0a0a 352e 2041 2043 6f6e 6669 6775 7265  ..5. A Configure
-00002350: 6420 576f 726b 6572 2050 6f6f 6c20 546f  d Worker Pool To
-00002360: 6b65 6e3a 2066 726f 6d20 7468 6520 2a2a  ken: from the **
-00002370: 576f 726b 6572 732a 2a20 7461 6220 696e  Workers** tab in
-00002380: 2074 6865 205b 5965 6c6c 6f77 446f 6720   the [YellowDog 
-00002390: 506f 7274 616c 5d28 6874 7470 733a 2f2f  Portal](https://
-000023a0: 706f 7274 616c 2e79 656c 6c6f 7764 6f67  portal.yellowdog
-000023b0: 2e63 6f2f 232f 776f 726b 6572 7329 2c20  .co/#/workers), 
-000023c0: 7573 6520 7468 6520 2a2a 2b41 6464 2043  use the **+Add C
-000023d0: 6f6e 6669 6775 7265 6420 576f 726b 6572  onfigured Worker
-000023e0: 2050 6f6f 6c2a 2a20 6275 7474 6f6e 2074   Pool** button t
-000023f0: 6f20 6372 6561 7465 2061 206e 6577 2057  o create a new W
-00002400: 6f72 6b65 7220 506f 6f6c 2061 6e64 2067  orker Pool and g
-00002410: 656e 6572 6174 6520 6120 746f 6b65 6e2e  enerate a token.
-00002420: 0a0a 0a36 2e20 4f62 7461 696e 2074 6865  ...6. Obtain the
-00002430: 2059 656c 6c6f 7744 6f67 2041 6765 6e74   YellowDog Agent
-00002440: 2061 6e64 2069 6e73 7461 6c6c 2f63 6f6e   and install/con
-00002450: 6669 6775 7265 2069 7420 6f6e 2079 6f75  figure it on you
-00002460: 7220 6f6e 2d70 7265 6d69 7365 2073 7973  r on-premise sys
-00002470: 7465 6d73 2075 7369 6e67 2074 6865 2054  tems using the T
-00002480: 6f6b 656e 2061 626f 7665 2e0a 0a23 2053  oken above...# S
-00002490: 6372 6970 7420 496e 7374 616c 6c61 7469  cript Installati
-000024a0: 6f6e 2077 6974 6820 5069 700a 0a50 7974  on with Pip..Pyt
-000024b0: 686f 6e20 7665 7273 696f 6e20 332e 3720  hon version 3.7 
-000024c0: 6f72 206c 6174 6572 2069 7320 7265 7175  or later is requ
-000024d0: 6972 6564 2e20 4974 2773 2072 6563 6f6d  ired. It's recom
-000024e0: 6d65 6e64 6564 2074 6861 7420 696e 7374  mended that inst
-000024f0: 616c 6c61 7469 6f6e 2069 7320 7065 7266  allation is perf
-00002500: 6f72 6d65 6420 696e 2061 2050 7974 686f  ormed in a Pytho
-00002510: 6e20 7669 7274 7561 6c20 656e 7669 726f  n virtual enviro
-00002520: 6e6d 656e 7420 286f 7220 7369 6d69 6c61  nment (or simila
-00002530: 7229 2074 6f20 6973 6f6c 6174 6520 7468  r) to isolate th
-00002540: 6520 696e 7374 616c 6c61 7469 6f6e 2066  e installation f
-00002550: 726f 6d20 6f74 6865 7220 5079 7468 6f6e  rom other Python
-00002560: 2065 6e76 6972 6f6e 6d65 6e74 7320 6f6e   environments on
-00002570: 2079 6f75 7220 7379 7374 656d 2e0a 0a49   your system...I
-00002580: 6e73 7461 6c6c 6174 696f 6e20 616e 6420  nstallation and 
-00002590: 7375 6273 6571 7565 6e74 2075 7064 6174  subsequent updat
-000025a0: 6520 6172 6520 7669 6120 6070 6970 6020  e are via `pip` 
-000025b0: 616e 6420 5079 5049 2075 7369 6e67 3a20  and PyPI using: 
-000025c0: 0a0a 6060 6073 6865 6c6c 0a70 6970 2069  ..```shell.pip i
-000025d0: 6e73 7461 6c6c 202d 5520 7965 6c6c 6f77  nstall -U yellow
-000025e0: 646f 672d 7079 7468 6f6e 2d65 7861 6d70  dog-python-examp
-000025f0: 6c65 730a 6060 600a 0a49 6620 796f 7527  les.```..If you'
-00002600: 7265 2069 6e74 6572 6573 7465 6420 696e  re interested in
-00002610: 2069 6e63 6c75 6469 6e67 202a 2a4a 736f   including **Jso
-00002620: 6e6e 6574 2a2a 2073 7570 706f 7274 2c20  nnet** support, 
-00002630: 706c 6561 7365 2073 6565 2074 6865 205b  please see the [
-00002640: 4a73 6f6e 6e65 7420 5375 7070 6f72 745d  Jsonnet Support]
-00002650: 2823 6a73 6f6e 6e65 742d 7375 7070 6f72  (#jsonnet-suppor
-00002660: 7429 2073 6563 7469 6f6e 2062 656c 6f77  t) section below
-00002670: 2e0a 0a23 2053 6372 6970 7420 496e 7374  ...# Script Inst
-00002680: 616c 6c61 7469 6f6e 2077 6974 6820 5069  allation with Pi
-00002690: 7078 0a0a 5468 6520 636f 6d6d 616e 6473  px..The commands
-000026a0: 2063 616e 2061 6c73 6f20 6265 2069 6e73   can also be ins
-000026b0: 7461 6c6c 6564 2075 7369 6e67 202a 2a5b  talled using **[
-000026c0: 7069 7078 5d28 6874 7470 733a 2f2f 7079  pipx](https://py
-000026d0: 7061 2e67 6974 6875 622e 696f 2f70 6970  pa.github.io/pip
-000026e0: 782f 292a 2a2e 0a0a 5468 6973 206d 6574  x/)**...This met
-000026f0: 686f 6420 7265 7175 6972 6573 2050 7974  hod requires Pyt
-00002700: 686f 6e20 332e 372b 2061 6e64 2070 6970  hon 3.7+ and pip
-00002710: 7820 746f 2062 6520 696e 7374 616c 6c65  x to be installe
-00002720: 642e 2054 6f20 696e 7374 616c 6c3a 0a60  d. To install:.`
-00002730: 6060 7368 656c 6c0a 7069 7078 2069 6e73  ``shell.pipx ins
-00002740: 7461 6c6c 2079 656c 6c6f 7764 6f67 2d70  tall yellowdog-p
-00002750: 7974 686f 6e2d 6578 616d 706c 6573 0a60  ython-examples.`
-00002760: 6060 0a0a 546f 2075 7064 6174 653a 0a60  ``..To update:.`
-00002770: 6060 7368 656c 6c0a 7069 7078 2075 7067  ``shell.pipx upg
-00002780: 7261 6465 2079 656c 6c6f 7764 6f67 2d70  rade yellowdog-p
-00002790: 7974 686f 6e2d 6578 616d 706c 6573 0a60  ython-examples.`
-000027a0: 6060 0a0a 2320 5573 6167 650a 0a42 6f74  ``..# Usage..Bot
-000027b0: 6820 6f66 2074 6865 2069 6e73 7461 6c6c  h of the install
-000027c0: 6174 696f 6e20 6d65 7468 6f64 7320 6162  ation methods ab
-000027d0: 6f76 6520 7769 6c6c 2069 6e73 7461 6c6c  ove will install
-000027e0: 2061 206e 756d 6265 7220 6f66 202a 2a60   a number of **`
-000027f0: 7964 2d60 2a2a 2063 6f6d 6d61 6e64 7320  yd-`** commands 
-00002800: 6f6e 2079 6f75 7220 5041 5448 2e0a 0a43  on your PATH...C
-00002810: 6f6d 6d61 6e64 7320 6172 6520 7275 6e20  ommands are run 
-00002820: 6672 6f6d 2074 6865 2063 6f6d 6d61 6e64  from the command
-00002830: 206c 696e 652e 2049 6e76 6f6b 696e 6720   line. Invoking 
-00002840: 7468 6520 636f 6d6d 616e 6420 7769 7468  the command with
-00002850: 2074 6865 2060 2d2d 6865 6c70 6020 6f72   the `--help` or
-00002860: 2060 2d68 6020 6f70 7469 6f6e 2077 696c   `-h` option wil
-00002870: 6c20 6469 7370 6c61 7920 7468 6520 636f  l display the co
-00002880: 6d6d 616e 6420 6c69 6e65 206f 7074 696f  mmand line optio
-00002890: 6e73 2061 7070 6c69 6361 626c 6520 746f  ns applicable to
-000028a0: 2061 2067 6976 656e 2063 6f6d 6d61 6e64   a given command
-000028b0: 2c20 652e 672e 3a0a 0a60 6060 7465 7874  , e.g.:..```text
-000028c0: 0a25 2079 642d 6361 6e63 656c 202d 2d68  .% yd-cancel --h
-000028d0: 656c 700a 7573 6167 653a 2079 642d 6361  elp.usage: yd-ca
-000028e0: 6e63 656c 205b 2d68 5d20 5b2d 2d64 6f63  ncel [-h] [--doc
-000028f0: 735d 205b 2d2d 636f 6e66 6967 203c 636f  s] [--config <co
-00002900: 6e66 6967 5f66 696c 652e 746f 6d6c 3e5d  nfig_file.toml>]
-00002910: 205b 2d2d 6b65 7920 3c61 7070 2d6b 6579   [--key <app-key
-00002920: 3e5d 205b 2d2d 7365 6372 6574 203c 6170  >] [--secret <ap
-00002930: 702d 7365 6372 6574 3e5d 0a20 2020 2020  p-secret>].     
-00002940: 2020 2020 2020 2020 2020 2020 5b2d 2d6e              [--n
-00002950: 616d 6573 7061 6365 203c 6e61 6d65 7370  amespace <namesp
-00002960: 6163 653e 5d20 5b2d 2d74 6167 203c 7461  ace>] [--tag <ta
-00002970: 673e 5d20 5b2d 2d75 726c 203c 7572 6c3e  g>] [--url <url>
-00002980: 5d20 5b2d 2d76 6172 6961 626c 6520 3c76  ] [--variable <v
-00002990: 6172 313d 7631 3e5d 205b 2d2d 7175 6965  ar1=v1>] [--quie
-000029a0: 745d 205b 2d2d 6465 6275 675d 0a20 2020  t] [--debug].   
-000029b0: 2020 2020 2020 2020 2020 2020 2020 5b2d                [-
-000029c0: 2d61 626f 7274 5d20 5b2d 2d66 6f6c 6c6f  -abort] [--follo
-000029d0: 775d 205b 2d2d 696e 7465 7261 6374 6976  w] [--interactiv
-000029e0: 655d 205b 2d2d 7965 735d 0a0a 5965 6c6c  e] [--yes]..Yell
-000029f0: 6f77 446f 6720 6578 616d 706c 6520 7574  owDog example ut
-00002a00: 696c 6974 7920 666f 7220 6361 6e63 656c  ility for cancel
-00002a10: 6c69 6e67 2057 6f72 6b20 5265 7175 6972  ling Work Requir
-00002a20: 656d 656e 7473 0a0a 6f70 7469 6f6e 616c  ements..optional
-00002a30: 2061 7267 756d 656e 7473 3a0a 2020 2d68   arguments:.  -h
-00002a40: 2c20 2d2d 6865 6c70 2020 2020 2020 2020  , --help        
-00002a50: 2020 2020 7368 6f77 2074 6869 7320 6865      show this he
-00002a60: 6c70 206d 6573 7361 6765 2061 6e64 2065  lp message and e
-00002a70: 7869 740a 2020 2d2d 646f 6373 2020 2020  xit.  --docs    
-00002a80: 2020 2020 2020 2020 2020 2020 7072 6f76              prov
-00002a90: 6964 6520 6120 6c69 6e6b 2074 6f20 7468  ide a link to th
-00002aa0: 6520 646f 6375 6d65 6e74 6174 696f 6e20  e documentation 
-00002ab0: 666f 7220 7468 6973 2076 6572 7369 6f6e  for this version
-00002ac0: 0a20 202d 2d63 6f6e 6669 6720 3c63 6f6e  .  --config <con
-00002ad0: 6669 675f 6669 6c65 2e74 6f6d 6c3e 2c20  fig_file.toml>, 
-00002ae0: 2d63 203c 636f 6e66 6967 5f66 696c 652e  -c <config_file.
-00002af0: 746f 6d6c 3e0a 2020 2020 2020 2020 2020  toml>.          
-00002b00: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00002b10: 6e66 6967 7572 6174 696f 6e20 6669 6c65  nfiguration file
-00002b20: 2069 6e20 544f 4d4c 2066 6f72 6d61 743b   in TOML format;
-00002b30: 2064 6566 6175 6c74 2069 7320 2763 6f6e   default is 'con
-00002b40: 6669 672e 746f 6d6c 2720 696e 2074 6865  fig.toml' in the
-00002b50: 2063 7572 7265 6e74 2064 6972 6563 746f   current directo
-00002b60: 7279 0a20 202d 2d6b 6579 203c 6170 702d  ry.  --key <app-
-00002b70: 6b65 793e 2c20 2d6b 203c 6170 702d 6b65  key>, -k <app-ke
-00002b80: 793e 0a20 2020 2020 2020 2020 2020 2020  y>.             
-00002b90: 2020 2020 2020 2020 2020 2074 6865 2059             the Y
-00002ba0: 656c 6c6f 7744 6f67 2041 7070 6c69 6361  ellowDog Applica
-00002bb0: 7469 6f6e 206b 6579 0a20 202d 2d73 6563  tion key.  --sec
-00002bc0: 7265 7420 3c61 7070 2d73 6563 7265 743e  ret <app-secret>
-00002bd0: 2c20 2d73 203c 6170 702d 7365 6372 6574  , -s <app-secret
-00002be0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00002bf0: 2020 2020 2020 2020 2020 7468 6520 5965            the Ye
-00002c00: 6c6c 6f77 446f 6720 4170 706c 6963 6174  llowDog Applicat
-00002c10: 696f 6e20 7365 6372 6574 0a20 202d 2d6e  ion secret.  --n
-00002c20: 616d 6573 7061 6365 203c 6e61 6d65 7370  amespace <namesp
-00002c30: 6163 653e 2c20 2d6e 203c 6e61 6d65 7370  ace>, -n <namesp
-00002c40: 6163 653e 0a20 2020 2020 2020 2020 2020  ace>.           
-00002c50: 2020 2020 2020 2020 2020 2020 2074 6865               the
-00002c60: 206e 616d 6573 7061 6365 2074 6f20 7573   namespace to us
-00002c70: 6520 7768 656e 2063 7265 6174 696e 6720  e when creating 
-00002c80: 616e 6420 6964 656e 7469 6679 696e 6720  and identifying 
-00002c90: 656e 7469 7469 6573 0a20 202d 2d74 6167  entities.  --tag
-00002ca0: 203c 7461 673e 2c20 2d74 203c 7461 673e   <tag>, -t <tag>
-00002cb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002cc0: 2020 2020 2020 2020 2074 6865 2074 6167           the tag
-00002cd0: 2074 6f20 7573 6520 666f 7220 7461 6767   to use for tagg
-00002ce0: 696e 6720 616e 6420 6e61 6d69 6e67 2065  ing and naming e
-00002cf0: 6e74 6974 6965 730a 2020 2d2d 7572 6c20  ntities.  --url 
-00002d00: 3c75 726c 3e2c 202d 7520 3c75 726c 3e0a  <url>, -u <url>.
-00002d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d20: 2020 2020 2020 2020 7468 6520 5552 4c20          the URL 
-00002d30: 6f66 2074 6865 2059 656c 6c6f 7744 6f67  of the YellowDog
-00002d40: 2050 6c61 7466 6f72 6d20 4150 490a 2020   Platform API.  
-00002d50: 2d2d 7661 7269 6162 6c65 203c 7661 7231  --variable <var1
-00002d60: 3d76 313e 2c20 2d76 203c 7661 7231 3d76  =v1>, -v <var1=v
-00002d70: 313e 0a20 2020 2020 2020 2020 2020 2020  1>.             
-00002d80: 2020 2020 2020 2020 2020 2075 7365 722d             user-
-00002d90: 6465 6669 6e65 6420 7661 7269 6162 6c65  defined variable
-00002da0: 2073 7562 7374 6974 7574 696f 6e73 3b20   substitutions; 
-00002db0: 6361 6e20 6265 2073 7570 706c 6965 6420  can be supplied 
-00002dc0: 6d75 6c74 6970 6c65 2074 696d 6573 0a20  multiple times. 
-00002dd0: 202d 2d71 7569 6574 2c20 2d71 2020 2020   --quiet, -q    
-00002de0: 2020 2020 2020 2073 7570 7072 6573 7320         suppress 
-00002df0: 286e 6f6e 2d65 7272 6f72 2c20 6e6f 6e2d  (non-error, non-
-00002e00: 696e 7465 7261 6374 6976 6529 2073 7461  interactive) sta
-00002e10: 7475 7320 616e 6420 7072 6f67 7265 7373  tus and progress
-00002e20: 206d 6573 7361 6765 730a 2020 2d2d 6465   messages.  --de
-00002e30: 6275 6720 2020 2020 2020 2020 2020 2020  bug             
-00002e40: 2020 7072 696e 7420 6120 7374 6163 6b20    print a stack 
-00002e50: 7472 6163 6520 2865 7463 2e29 206f 6e20  trace (etc.) on 
-00002e60: 6572 726f 720a 2020 2d2d 6162 6f72 742c  error.  --abort,
-00002e70: 202d 6120 2020 2020 2020 2020 2020 6162   -a           ab
-00002e80: 6f72 7420 616c 6c20 7275 6e6e 696e 6720  ort all running 
-00002e90: 7461 736b 7320 7769 7468 2069 6d6d 6564  tasks with immed
-00002ea0: 6961 7465 2065 6666 6563 740a 2020 2d2d  iate effect.  --
-00002eb0: 666f 6c6c 6f77 2c20 2d66 2020 2020 2020  follow, -f      
-00002ec0: 2020 2020 7768 656e 2075 7369 6e67 202d      when using -
-00002ed0: 2d61 626f 7274 2c20 706f 6c6c 2075 6e74  -abort, poll unt
-00002ee0: 696c 2061 6c6c 2054 6173 6b73 2068 6176  il all Tasks hav
-00002ef0: 6520 6265 656e 2061 626f 7274 6564 0a20  e been aborted. 
-00002f00: 202d 2d69 6e74 6572 6163 7469 7665 2c20   --interactive, 
-00002f10: 2d69 2020 2020 206c 6973 742c 2061 6e64  -i     list, and
-00002f20: 2069 6e74 6572 6163 7469 7665 6c79 2073   interactively s
-00002f30: 656c 6563 742c 2069 7465 6d73 2074 6f20  elect, items to 
-00002f40: 6163 7420 6f6e 0a20 202d 2d79 6573 2c20  act on.  --yes, 
-00002f50: 2d79 2020 2020 2020 2020 2020 2020 2070  -y             p
-00002f60: 6572 666f 726d 2064 6573 7472 7563 7469  erform destructi
-00002f70: 7665 2061 6374 696f 6e73 2077 6974 686f  ve actions witho
-00002f80: 7574 2072 6571 7569 7269 6e67 2075 7365  ut requiring use
-00002f90: 7220 636f 6e66 6972 6d61 7469 6f6e 0a60  r confirmation.`
-00002fa0: 6060 0a0a 2320 436f 6e66 6967 7572 6174  ``..# Configurat
-00002fb0: 696f 6e0a 0a42 7920 6465 6661 756c 742c  ion..By default,
-00002fc0: 2074 6865 206f 7065 7261 7469 6f6e 206f   the operation o
-00002fd0: 6620 616c 6c20 636f 6d6d 616e 6473 2069  f all commands i
-00002fe0: 7320 636f 6e66 6967 7572 6564 2075 7369  s configured usi
-00002ff0: 6e67 2061 2054 4f4d 4c20 636f 6e66 6967  ng a TOML config
-00003000: 7572 6174 696f 6e20 6669 6c65 2e0a 0a54  uration file...T
-00003010: 6865 2063 6f6e 6669 6775 7261 7469 6f6e  he configuration
-00003020: 2066 696c 6520 6861 7320 7468 7265 6520   file has three 
-00003030: 706f 7373 6962 6c65 2073 6563 7469 6f6e  possible section
-00003040: 733a 0a0a 312e 2041 2060 636f 6d6d 6f6e  s:..1. A `common
-00003050: 6020 7365 6374 696f 6e20 7468 6174 2063  ` section that c
-00003060: 6f6e 7461 696e 7320 7265 7175 6972 6564  ontains required
-00003070: 2073 6563 7572 6974 7920 7072 6f70 6572   security proper
-00003080: 7469 6573 2066 6f72 2069 6e74 6572 6163  ties for interac
-00003090: 7469 6e67 2077 6974 6820 7468 6520 5965  ting with the Ye
-000030a0: 6c6c 6f77 446f 6720 706c 6174 666f 726d  llowDog platform
-000030b0: 2c20 7365 7473 2074 6865 204e 616d 6573  , sets the Names
-000030c0: 7061 6365 2069 6e20 7768 6963 6820 5965  pace in which Ye
-000030d0: 6c6c 6f77 446f 6720 6173 7365 7473 2061  llowDog assets a
-000030e0: 6e64 206f 626a 6563 7473 2061 7265 2063  nd objects are c
-000030f0: 7265 6174 6564 2c20 616e 6420 6120 5461  reated, and a Ta
-00003100: 6720 7468 6174 2069 7320 7573 6564 2066  g that is used f
-00003110: 6f72 2074 6167 6769 6e67 2061 6e64 206e  or tagging and n
-00003120: 616d 696e 6720 6173 7365 7473 2061 6e64  aming assets and
-00003130: 206f 626a 6563 7473 2e0a 322e 2041 2060   objects..2. A `
-00003140: 776f 726b 5265 7175 6972 656d 656e 7460  workRequirement`
-00003150: 2073 6563 7469 6f6e 2074 6861 7420 6465   section that de
-00003160: 6669 6e65 7320 7468 6520 7072 6f70 6572  fines the proper
-00003170: 7469 6573 206f 6620 576f 726b 2052 6571  ties of Work Req
-00003180: 7569 7265 6d65 6e74 7320 746f 2062 6520  uirements to be 
-00003190: 7375 626d 6974 7465 6420 746f 2074 6865  submitted to the
-000031a0: 2059 656c 6c6f 7744 6f67 2070 6c61 7466   YellowDog platf
-000031b0: 6f72 6d2e 0a33 2e20 4120 6077 6f72 6b65  orm..3. A `worke
-000031c0: 7250 6f6f 6c60 2073 6563 7469 6f6e 2074  rPool` section t
-000031d0: 6861 7420 6465 6669 6e65 7320 7468 6520  hat defines the 
-000031e0: 7072 6f70 6572 7469 6573 206f 6620 5072  properties of Pr
-000031f0: 6f76 6973 6f6e 6564 2057 6f72 6b65 7220  ovisoned Worker 
-00003200: 506f 6f6c 7320 746f 2062 6520 6372 6561  Pools to be crea
-00003210: 7465 6420 7573 696e 6720 7468 6520 5965  ted using the Ye
-00003220: 6c6c 6f77 446f 6720 706c 6174 666f 726d  llowDog platform
-00003230: 2e20 0a0a 5468 6572 6520 6973 2061 2064  . ..There is a d
-00003240: 6f63 756d 656e 7465 6420 7465 6d70 6c61  ocumented templa
-00003250: 7465 2054 4f4d 4c20 6669 6c65 2070 726f  te TOML file pro
-00003260: 7669 6465 6420 696e 205b 636f 6e66 6967  vided in [config
-00003270: 2e74 6f6d 6c2e 7465 6d70 6c61 7465 5d28  .toml.template](
-00003280: 636f 6e66 6967 2e74 6f6d 6c2e 7465 6d70  config.toml.temp
-00003290: 6c61 7465 292c 2063 6f6e 7461 696e 696e  late), containin
-000032a0: 6720 7468 6520 6d61 696e 2070 726f 7065  g the main prope
-000032b0: 7274 6965 7320 7468 6174 2063 616e 2062  rties that can b
-000032c0: 6520 636f 6e66 6967 7572 6564 2e0a 0a54  e configured...T
-000032d0: 6865 2063 6f6e 6669 6775 7261 7469 6f6e  he configuration
-000032e0: 2066 696c 656e 616d 6520 6361 6e20 6265   filename can be
-000032f0: 2073 7570 706c 6965 6420 696e 2074 6872   supplied in thr
-00003300: 6565 2064 6966 6665 7265 6e74 2077 6179  ee different way
-00003310: 733a 0a0a 312e 204f 6e20 7468 6520 636f  s:..1. On the co
-00003320: 6d6d 616e 6420 6c69 6e65 2c20 7573 696e  mmand line, usin
-00003330: 6720 7468 6520 602d 2d63 6f6e 6669 6760  g the `--config`
-00003340: 206f 7220 602d 6360 206f 7074 696f 6e73   or `-c` options
-00003350: 2c20 652e 672e 3a3c 6272 3e60 7964 2d73  , e.g.:<br>`yd-s
-00003360: 7562 6d69 7420 2d63 206a 6f62 732f 636f  ubmit -c jobs/co
-00003370: 6e66 6967 5f31 2e74 6f6d 6c60 0a32 2e20  nfig_1.toml`.2. 
-00003380: 5573 696e 6720 7468 6520 6059 445f 434f  Using the `YD_CO
-00003390: 4e46 6020 656e 7669 726f 6e6d 656e 7420  NF` environment 
-000033a0: 7661 7269 6162 6c65 2c20 652e 672e 3a20  variable, e.g.: 
-000033b0: 3c62 723e 6065 7870 6f72 7420 5944 5f43  <br>`export YD_C
-000033c0: 4f4e 463d 226a 6f62 732f 636f 6e66 6967  ONF="jobs/config
-000033d0: 5f31 2e74 6f6d 6c22 600a 332e 2049 6620  _1.toml"`.3. If 
-000033e0: 6e65 6974 6865 7220 6f66 2074 6865 2061  neither of the a
-000033f0: 626f 7665 2069 7320 7375 7070 6c69 6564  bove is supplied
-00003400: 2c20 7468 6520 636f 6d6d 616e 6473 206c  , the commands l
-00003410: 6f6f 6b20 666f 7220 6120 6063 6f6e 6669  ook for a `confi
-00003420: 672e 746f 6d6c 6020 6669 6c65 2069 6e20  g.toml` file in 
-00003430: 7468 6520 6375 7272 656e 7420 6469 7265  the current dire
-00003440: 6374 6f72 790a 0a54 6865 206f 7074 696f  ctory..The optio
-00003450: 6e73 2061 626f 7665 2061 7265 2073 686f  ns above are sho
-00003460: 776e 2069 6e20 6f72 6465 7220 6f66 2070  wn in order of p
-00003470: 7265 6365 6465 6e63 652c 2069 2e65 2e2c  recedence, i.e.,
-00003480: 2061 2066 696c 656e 616d 6520 7375 7070   a filename supp
-00003490: 6c69 6564 206f 6e20 7468 6520 636f 6d6d  lied on the comm
-000034a0: 616e 6420 6c69 6e65 2073 7570 6572 7365  and line superse
-000034b0: 6465 7320 6f6e 6520 7365 7420 696e 2060  des one set in `
-000034c0: 5944 5f43 4f4e 4660 2c20 7768 6963 6820  YD_CONF`, which 
-000034d0: 7375 7065 7273 6564 6573 2074 6865 2064  supersedes the d
-000034e0: 6566 6175 6c74 2e0a 0a23 204e 616d 696e  efault...# Namin
-000034f0: 6720 5275 6c65 730a 0a41 6c6c 2065 6e74  g Rules..All ent
-00003500: 6974 7920 6e61 6d65 7320 7573 6564 2077  ity names used w
-00003510: 6974 6869 6e20 7468 6520 5965 6c6c 6f77  ithin the Yellow
-00003520: 446f 6720 506c 6174 666f 726d 206d 7573  Dog Platform mus
-00003530: 7420 636f 6d70 6c79 2077 6974 6820 7468  t comply with th
-00003540: 6520 666f 6c6c 6f77 696e 6720 7265 7374  e following rest
-00003550: 7269 6374 696f 6e73 3a0a 0a2d 204e 616d  rictions:..- Nam
-00003560: 6573 2063 616e 206f 6e6c 7920 636f 6e74  es can only cont
-00003570: 6169 6e20 7468 6520 666f 6c6c 6f77 696e  ain the followin
-00003580: 673a 206c 6f77 6572 6361 7365 206c 6574  g: lowercase let
-00003590: 7465 7273 2c20 6469 6769 7473 2c20 6879  ters, digits, hy
-000035a0: 7068 656e 7320 616e 6420 756e 6465 7273  phens and unders
-000035b0: 636f 7265 7320 286e 6f74 6520 7468 6174  cores (note that
-000035c0: 2073 7061 6365 7320 6172 6520 6e6f 7420   spaces are not 
-000035d0: 7065 726d 6974 7465 6429 0a2d 204e 616d  permitted).- Nam
-000035e0: 6573 206d 7573 7420 7374 6172 7420 7769  es must start wi
-000035f0: 7468 2061 206c 6574 7465 720a 2d20 4e61  th a letter.- Na
-00003600: 6d65 7320 6d75 7374 2065 6e64 2077 6974  mes must end wit
-00003610: 6820 6120 6c65 7474 6572 206f 7220 6469  h a letter or di
-00003620: 6769 740a 2d20 4e61 6d65 206c 656e 6774  git.- Name lengt
-00003630: 6820 6d75 7374 2062 6520 3c3d 2036 3020  h must be <= 60 
-00003640: 6368 6172 6163 7465 7273 0a0a 5468 6573  characters..Thes
-00003650: 6520 7265 7374 7269 6374 696f 6e73 2061  e restrictions a
-00003660: 7070 6c79 2074 6f20 656e 7469 7469 6573  pply to entities
-00003670: 2069 6e63 6c75 6469 6e67 204e 616d 6573   including Names
-00003680: 7061 6365 732c 2054 6167 732c 2057 6f72  paces, Tags, Wor
-00003690: 6b20 5265 7175 6972 656d 656e 7473 2c20  k Requirements, 
-000036a0: 5461 736b 2047 726f 7570 732c 2054 6173  Task Groups, Tas
-000036b0: 6b73 2c20 576f 726b 6572 2050 6f6f 6c73  ks, Worker Pools
-000036c0: 2c20 616e 6420 436f 6d70 7574 6520 5265  , and Compute Re
-000036d0: 7175 6972 656d 656e 7473 2c20 616e 6420  quirements, and 
-000036e0: 616c 736f 2061 7070 6c79 2074 6f20 656e  also apply to en
-000036f0: 7469 7469 6573 2074 6861 7420 6172 6520  tities that are 
-00003700: 6375 7272 656e 746c 7920 7573 6564 2069  currently used i
-00003710: 6e64 6972 6563 746c 7920 6279 2074 6865  ndirectly by the
-00003720: 7365 2073 6372 6970 7473 2c20 696e 636c  se scripts, incl
-00003730: 7564 696e 6720 5573 6572 6e61 6d65 732c  uding Usernames,
-00003740: 2043 7265 6465 6e74 6961 6c73 2c20 4b65   Credentials, Ke
-00003750: 7972 696e 6773 2c20 436f 6d70 7574 6520  yrings, Compute 
-00003760: 536f 7572 6365 7320 616e 6420 436f 6d70  Sources and Comp
-00003770: 7574 6520 5465 6d70 6c61 7465 732e 0a0a  ute Templates...
-00003780: 2320 436f 6d6d 6f6e 2050 726f 7065 7274  # Common Propert
-00003790: 6965 730a 0a54 6865 2060 5b63 6f6d 6d6f  ies..The `[commo
-000037a0: 6e5d 6020 7365 6374 696f 6e20 6f66 2074  n]` section of t
-000037b0: 6865 2063 6f6e 6669 6775 7261 7469 6f6e  he configuration
-000037c0: 2066 696c 6520 6361 6e20 636f 6e74 6169   file can contai
-000037d0: 6e20 7468 6520 666f 6c6c 6f77 696e 6720  n the following 
-000037e0: 7072 6f70 6572 7469 6573 3a0a 0a7c 2050  properties:..| P
-000037f0: 726f 7065 7274 7920 2020 207c 2044 6573  roperty    | Des
-00003800: 6372 6970 7469 6f6e 2020 2020 2020 2020  cription        
-00003810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003850: 207c 0a7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d   |.|:-----------
-00003860: 2d7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -|:-------------
-00003870: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003880: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003890: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000038a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000038b0: 2d2d 2d2d 2d2d 2d7c 0a7c 2060 6b65 7960  -------|.| `key`
-000038c0: 2020 2020 2020 207c 2054 6865 202a 2a6b         | The **k
-000038d0: 6579 2a2a 206f 6620 7468 6520 5965 6c6c  ey** of the Yell
-000038e0: 6f77 446f 6720 4170 706c 6963 6174 696f  owDog Applicatio
-000038f0: 6e20 756e 6465 7220 7768 6963 6820 7468  n under which th
-00003900: 6520 636f 6d6d 616e 6473 2077 696c 6c20  e commands will 
-00003910: 7275 6e20 2020 2020 2020 2020 207c 0a7c  run          |.|
-00003920: 2060 7365 6372 6574 6020 2020 207c 2054   `secret`    | T
-00003930: 6865 202a 2a73 6563 7265 742a 2a20 6f66  he **secret** of
-00003940: 2074 6865 2059 656c 6c6f 7744 6f67 2041   the YellowDog A
-00003950: 7070 6c69 6361 7469 6f6e 2075 6e64 6572  pplication under
-00003960: 2077 6869 6368 2074 6865 2063 6f6d 6d61   which the comma
-00003970: 6e64 7320 7769 6c6c 2072 756e 2020 2020  nds will run    
-00003980: 2020 207c 0a7c 2060 6e61 6d65 7370 6163     |.| `namespac
-00003990: 6560 207c 2054 6865 202a 2a6e 616d 6573  e` | The **names
-000039a0: 7061 6365 2a2a 2074 6f20 6265 2075 7365  pace** to be use
-000039b0: 6420 666f 7220 6772 6f75 7069 6e67 2072  d for grouping r
-000039c0: 6573 6f75 7263 6573 2020 2020 2020 2020  esources        
-000039d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000039e0: 2020 2020 2020 2020 207c 0a7c 2060 7461           |.| `ta
-000039f0: 6760 2020 2020 2020 207c 2054 6865 202a  g`       | The *
-00003a00: 2a74 6167 2a2a 2074 6f20 6265 2075 7365  *tag** to be use
-00003a10: 6420 666f 7220 7461 6767 696e 6720 7265  d for tagging re
-00003a20: 736f 7572 6365 7320 616e 6420 6e61 6d69  sources and nami
-00003a30: 6e67 206f 626a 6563 7473 2020 2020 2020  ng objects      
-00003a40: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00003a50: 0a7c 2060 7572 6c60 2020 2020 2020 207c  .| `url`       |
-00003a60: 2054 6865 202a 2a55 524c 2a2a 206f 6620   The **URL** of 
-00003a70: 7468 6520 5965 6c6c 6f77 446f 6720 506c  the YellowDog Pl
-00003a80: 6174 666f 726d 2041 5049 2065 6e64 706f  atform API endpo
-00003a90: 696e 742c 2069 6620 7468 6520 6465 6661  int, if the defa
-00003aa0: 756c 7420 6973 6e27 7420 746f 2062 6520  ult isn't to be 
-00003ab0: 7573 6564 207c 0a7c 2060 7661 7269 6162  used |.| `variab
-00003ac0: 6c65 7360 207c 2041 2074 6162 6c65 2063  les` | A table c
-00003ad0: 6f6e 7461 696e 696e 6720 2a2a 7661 7269  ontaining **vari
-00003ae0: 6162 6c65 2073 7562 7374 6974 7574 696f  able substitutio
-00003af0: 6e73 2a2a 2028 7365 6520 7468 6520 5661  ns** (see the Va
-00003b00: 7269 6162 6c65 7320 7365 6374 696f 6e20  riables section 
-00003b10: 6265 6c6f 7729 2020 2020 207c 0a0a 416e  below)     |..An
-00003b20: 2065 7861 6d70 6c65 2060 636f 6d6d 6f6e   example `common
-00003b30: 6020 7365 6374 696f 6e20 6973 2073 686f  ` section is sho
-00003b40: 776e 2062 656c 6f77 3a0a 0a60 6060 746f  wn below:..```to
-00003b50: 6d6c 0a5b 636f 6d6d 6f6e 5d0a 2020 2020  ml.[common].    
-00003b60: 6b65 7920 3d20 2261 7364 6667 686a 6b6c  key = "asdfghjkl
-00003b70: 7a78 6376 622d 3132 3334 3536 3722 0a20  zxcvb-1234567". 
-00003b80: 2020 2073 6563 7265 7420 3d20 2271 7765     secret = "qwe
-00003b90: 7274 7975 696f 7061 7364 6667 686a 6b6c  rtyuiopasdfghjkl
-00003ba0: 7a78 6376 626e 6d31 3233 3435 3637 3839  zxcvbnm123456789
-00003bb0: 3071 7765 7274 7975 220a 2020 2020 6e61  0qwertyu".    na
-00003bc0: 6d65 7370 6163 6520 3d20 2270 726f 6a65  mespace = "proje
-00003bd0: 6374 2d78 220a 2020 2020 7461 6720 3d20  ct-x".    tag = 
-00003be0: 2274 6573 7469 6e67 2d7b 7b75 7365 726e  "testing-{{usern
-00003bf0: 616d 657d 7d22 0a60 6060 0a0a 496e 6465  ame}}".```..Inde
-00003c00: 6e74 6174 696f 6e20 6973 206f 7074 696f  ntation is optio
-00003c10: 6e61 6c20 696e 2054 4f4d 4c20 6669 6c65  nal in TOML file
-00003c20: 7320 616e 6420 6973 2066 6f72 2072 6561  s and is for rea
-00003c30: 6461 6269 6c69 7479 206f 6e6c 792e 0a0a  dability only...
-00003c40: 2323 2053 7065 6369 6679 696e 6720 436f  ## Specifying Co
-00003c50: 6d6d 6f6e 2050 726f 7065 7274 6965 7320  mmon Properties 
-00003c60: 7573 696e 6720 7468 6520 436f 6d6d 616e  using the Comman
-00003c70: 6420 4c69 6e65 206f 7220 456e 7669 726f  d Line or Enviro
-00003c80: 6e6d 656e 7420 5661 7269 6162 6c65 730a  nment Variables.
-00003c90: 0a41 6c6c 2074 6865 2063 6f6d 6d6f 6e20  .All the common 
-00003ca0: 7072 6f70 6572 7469 6573 2063 616e 2062  properties can b
-00003cb0: 6520 7365 7420 7573 696e 6720 636f 6d6d  e set using comm
-00003cc0: 616e 6420 6c69 6e65 206f 7074 696f 6e73  and line options
-00003cd0: 2c20 6f72 2069 6e20 656e 7669 726f 6e6d  , or in environm
-00003ce0: 656e 7420 7661 7269 6162 6c65 732e 0a0a  ent variables...
-00003cf0: 5468 6520 2a2a 636f 6d6d 616e 6420 6c69  The **command li
-00003d00: 6e65 206f 7074 696f 6e73 2a2a 2061 7265  ne options** are
-00003d10: 2061 7320 666f 6c6c 6f77 733a 0a0a 2d20   as follows:..- 
-00003d20: 602d 2d6b 6579 6020 6f72 2060 2d6b 600a  `--key` or `-k`.
-00003d30: 2d20 602d 2d73 6563 7265 7460 206f 7220  - `--secret` or 
-00003d40: 602d 7360 0a2d 2060 2d2d 6e61 6d65 7370  `-s`.- `--namesp
-00003d50: 6163 6560 206f 7220 602d 6e60 0a2d 2060  ace` or `-n`.- `
-00003d60: 2d2d 7461 6760 206f 7220 602d 7460 0a2d  --tag` or `-t`.-
-00003d70: 2060 2d2d 7572 6c60 206f 7220 602d 7560   `--url` or `-u`
-00003d80: 0a0a 5468 6573 6520 6f70 7469 6f6e 7320  ..These options 
-00003d90: 6361 6e20 616c 736f 2062 6520 6c69 7374  can also be list
-00003da0: 6564 2062 7920 7275 6e6e 696e 6720 6120  ed by running a 
-00003db0: 636f 6d6d 616e 6420 7769 7468 2074 6865  command with the
-00003dc0: 2060 2d2d 6865 6c70 6020 6f72 2060 2d68   `--help` or `-h
-00003dd0: 6020 6f70 7469 6f6e 2e0a 0a54 6865 202a  ` option...The *
-00003de0: 2a65 6e76 6972 6f6e 6d65 6e74 2076 6172  *environment var
-00003df0: 6961 626c 6573 2a2a 2061 7265 2061 7320  iables** are as 
-00003e00: 666f 6c6c 6f77 733a 0a0a 2d20 6059 445f  follows:..- `YD_
-00003e10: 4b45 5960 0a2d 2060 5944 5f53 4543 5245  KEY`.- `YD_SECRE
-00003e20: 5460 0a2d 2060 5944 5f4e 414d 4553 5041  T`.- `YD_NAMESPA
-00003e30: 4345 600a 2d20 6059 445f 5441 4760 0a2d  CE`.- `YD_TAG`.-
-00003e40: 2060 5944 5f55 524c 600a 0a57 6865 6e20   `YD_URL`..When 
-00003e50: 7365 7474 696e 6720 7468 6520 7661 6c75  setting the valu
-00003e60: 6520 6f66 2074 6865 2061 626f 7665 2070  e of the above p
-00003e70: 726f 7065 7274 6965 732c 2061 2070 726f  roperties, a pro
-00003e80: 7065 7274 7920 7365 7420 6f6e 2074 6865  perty set on the
-00003e90: 2063 6f6d 6d61 6e64 206c 696e 6520 7461   command line ta
-00003ea0: 6b65 7320 7072 6563 6564 656e 6365 206f  kes precedence o
-00003eb0: 7665 7220 6f6e 6520 7365 7420 7669 6120  ver one set via 
-00003ec0: 616e 2065 6e76 6972 6f6e 6d65 6e74 2076  an environment v
-00003ed0: 6172 6961 626c 652c 2061 6e64 2062 6f74  ariable, and bot
-00003ee0: 6820 7461 6b65 2070 7265 6365 6465 6e63  h take precedenc
-00003ef0: 6520 6f76 6572 2061 2076 616c 7565 2073  e over a value s
-00003f00: 6574 2069 6e20 6120 636f 6e66 6967 7572  et in a configur
-00003f10: 6174 696f 6e20 6669 6c65 2e0a 0a49 6620  ation file...If 
-00003f20: 616c 6c20 7468 6520 7265 7175 6972 6564  all the required
-00003f30: 2063 6f6d 6d6f 6e20 7072 6f70 6572 7469   common properti
-00003f40: 6573 2061 7265 2073 6574 2075 7369 6e67  es are set using
-00003f50: 2074 6865 2063 6f6d 6d61 6e64 206c 696e   the command lin
-00003f60: 6520 6f72 2065 6e76 6972 6f6e 6d65 6e74  e or environment
-00003f70: 2076 6172 6961 626c 6573 2c20 7468 656e   variables, then
-00003f80: 2074 6865 2065 6e74 6972 6520 6063 6f6d   the entire `com
-00003f90: 6d6f 6e60 2073 6563 7469 6f6e 206f 6620  mon` section of 
-00003fa0: 7468 6520 544f 4d4c 2066 696c 6520 6361  the TOML file ca
-00003fb0: 6e20 6265 206f 6d69 7474 6564 2e0a 0a23  n be omitted...#
-00003fc0: 2320 5661 7269 6162 6c65 2053 7562 7374  # Variable Subst
-00003fd0: 6974 7574 696f 6e73 2069 6e20 436f 6d6d  itutions in Comm
-00003fe0: 6f6e 2050 726f 7065 7274 6965 730a 0a4e  on Properties..N
-00003ff0: 6f74 6520 7468 6520 7573 6520 6f66 2060  ote the use of `
-00004000: 7b7b 7573 6572 6e61 6d65 7d7d 6020 696e  {{username}}` in
-00004010: 2074 6865 2076 616c 7565 206f 6620 7468   the value of th
-00004020: 6520 6074 6167 6020 7072 6f70 6572 7479  e `tag` property
-00004030: 3a20 7468 6973 2069 7320 6120 2a2a 7661  : this is a **va
-00004040: 7269 6162 6c65 2073 7562 7374 6974 7574  riable substitut
-00004050: 696f 6e2a 2a20 7468 6174 2063 616e 206f  ion** that can o
-00004060: 7074 696f 6e61 6c6c 7920 6265 2075 7365  ptionally be use
-00004070: 6420 746f 2069 6e73 6572 7420 7468 6520  d to insert the 
-00004080: 6c6f 6769 6e20 7573 6572 6e61 6d65 206f  login username o
-00004090: 6620 7468 6520 7573 6572 2072 756e 6e69  f the user runni
-000040a0: 6e67 2074 6865 2063 6f6d 6d61 6e64 732e  ng the commands.
-000040b0: 2053 6f2c 2066 6f72 2075 7365 726e 616d   So, for usernam
-000040c0: 6520 6061 6263 602c 2074 6865 2060 7461  e `abc`, the `ta
-000040d0: 6760 2077 6f75 6c64 2062 6520 7365 7420  g` would be set 
-000040e0: 746f 2060 7465 7374 696e 672d 6162 6360  to `testing-abc`
-000040f0: 2e20 5468 6973 2063 616e 2062 6520 6865  . This can be he
-00004100: 6c70 6675 6c20 746f 2064 6973 616d 6269  lpful to disambi
-00004110: 6775 6174 6520 6d75 6c74 6970 6c65 2075  guate multiple u
-00004120: 7365 7273 2072 756e 6e69 6e67 2077 6974  sers running wit
-00004130: 6820 7468 6520 7361 6d65 2063 6f6e 6669  h the same confi
-00004140: 6775 7261 7469 6f6e 2064 6174 612e 0a0a  guration data...
-00004150: 5661 7269 6162 6c65 2073 7562 7374 6974  Variable substit
-00004160: 7574 696f 6e73 2061 7265 2064 6973 6375  utions are discu
-00004170: 7373 6564 2062 656c 6f77 2e0a 0a23 2056  ssed below...# V
-00004180: 6172 6961 626c 6520 5375 6273 7469 7475  ariable Substitu
-00004190: 7469 6f6e 730a 0a56 6172 6961 626c 6520  tions..Variable 
-000041a0: 7375 6273 7469 7475 7469 6f6e 7320 7072  substitutions pr
-000041b0: 6f76 6964 6520 6120 706f 7765 7266 756c  ovide a powerful
-000041c0: 2077 6179 206f 6620 696e 7472 6f64 7563   way of introduc
-000041d0: 696e 6720 7661 7269 6162 6c65 2076 616c  ing variable val
-000041e0: 7565 7320 696e 746f 2054 4f4d 4c20 636f  ues into TOML co
-000041f0: 6e66 6967 7572 6174 696f 6e20 6669 6c65  nfiguration file
-00004200: 732c 2057 6f72 6b20 5265 7175 6972 656d  s, Work Requirem
-00004210: 656e 7420 4a53 4f4e 2064 6566 696e 6974  ent JSON definit
-00004220: 696f 6e73 2c20 616e 6420 576f 726b 6572  ions, and Worker
-00004230: 2050 6f6f 6c20 4a53 4f4e 2064 6566 696e   Pool JSON defin
-00004240: 6974 696f 6e73 2e20 5468 6579 2063 616e  itions. They can
-00004250: 2062 6520 696e 636c 7564 6564 2069 6e20   be included in 
-00004260: 7468 6520 7661 6c75 6520 6f66 2061 6e79  the value of any
-00004270: 2070 726f 7065 7274 7920 696e 2065 6163   property in eac
-00004280: 6820 6f66 2074 6865 7365 206f 626a 6563  h of these objec
-00004290: 7473 2c20 696e 636c 7564 696e 6720 696e  ts, including in
-000042a0: 2076 616c 7565 7320 7769 7468 696e 206c   values within l
-000042b0: 6973 7473 2028 652e 672e 2c20 666f 7220  ists (e.g., for 
-000042c0: 7468 6520 6061 7267 756d 656e 7473 6020  the `arguments` 
-000042d0: 7072 6f70 6572 7479 2920 616e 6420 6172  property) and ar
-000042e0: 7261 7973 2028 652e 672e 2c20 7468 6520  rays (e.g., the 
-000042f0: 6065 6e76 6972 6f6e 6d65 6e74 6020 7072  `environment` pr
-00004300: 6f70 6572 7479 292e 0a0a 5661 7269 6162  operty)...Variab
-00004310: 6c65 2073 7562 7374 6974 7574 696f 6e73  le substitutions
-00004320: 2061 7265 2065 7870 7265 7373 6564 2075   are expressed u
-00004330: 7369 6e67 2060 7b7b 7661 7269 6162 6c65  sing `{{variable
-00004340: 7d7d 6020 6e6f 7461 7469 6f6e 2c20 7768  }}` notation, wh
-00004350: 6572 6520 7468 6520 6578 7072 6573 7369  ere the expressi
-00004360: 6f6e 2069 7320 7265 706c 6163 6564 2062  on is replaced b
-00004370: 7920 7468 6520 7661 6c75 6520 6f66 2060  y the value of `
-00004380: 7661 7269 6162 6c65 602e 0a0a 5375 6273  variable`...Subs
-00004390: 7469 7475 7469 6f6e 7320 6361 6e20 616c  titutions can al
-000043a0: 736f 2062 6520 7065 7266 6f72 6d65 6420  so be performed 
-000043b0: 666f 7220 6e6f 6e2d 7374 7269 6e67 2028  for non-string (
-000043c0: 6e75 6d62 6572 2061 6e64 2062 6f6f 6c65  number and boole
-000043d0: 616e 2920 7661 6c75 6573 2075 7369 6e67  an) values using
-000043e0: 2074 6865 2060 6e75 6d3a 6020 616e 6420   the `num:` and 
-000043f0: 6062 6f6f 6c3a 6020 7072 6566 6978 6573  `bool:` prefixes
-00004400: 2077 6974 6869 6e20 7468 6520 7661 7269   within the vari
-00004410: 6162 6c65 2073 7562 7374 6974 7574 696f  able substitutio
-00004420: 6e3a 0a0a 2d20 4465 6669 6e65 2074 6865  n:..- Define the
-00004430: 2076 6172 6961 626c 6520 7375 6273 7469   variable substi
-00004440: 7475 7469 6f6e 2075 7369 6e67 206f 6e65  tution using one
-00004450: 206f 6620 7468 6520 666f 6c6c 6f77 696e   of the followin
-00004460: 6720 7061 7474 6572 6e73 3a20 6022 7b7b  g patterns: `"{{
-00004470: 6e75 6d3a 6d79 5f69 6e74 7d7d 2260 2c20  num:my_int}}"`, 
-00004480: 6022 7b7b 6e75 6d3a 6d79 5f66 6c6f 6174  `"{{num:my_float
-00004490: 7d7d 2260 2c20 6022 7b7b 626f 6f6c 3a6d  }}"`, `"{{bool:m
-000044a0: 795f 626f 6f6c 7d7d 2260 0a2d 2056 6172  y_bool}}"`.- Var
-000044b0: 6961 626c 6520 6465 6669 6e69 7469 6f6e  iable definition
-000044c0: 7320 7375 7070 6c69 6564 206f 6e20 7468  s supplied on th
-000044d0: 6520 636f 6d6d 616e 6420 6c69 6e65 2077  e command line w
-000044e0: 6f75 6c64 2074 6865 6e20 6265 206f 6620  ould then be of 
-000044f0: 7468 6520 666f 726d 3a20 602d 6d20 6d79  the form: `-m my
-00004500: 5f69 6e74 3d35 202d 6d20 6d79 5f66 6c6f  _int=5 -m my_flo
-00004510: 6174 3d32 2e35 202d 6d20 6d79 5f62 6f6f  at=2.5 -m my_boo
-00004520: 6c3d 7472 7565 600a 2d20 496e 2074 6865  l=true`.- In the
-00004530: 2070 726f 6365 7373 6564 204a 534f 4e20   processed JSON 
-00004540: 6f72 2054 4f4d 4c2c 2074 6865 7365 2076  or TOML, these v
-00004550: 616c 7565 7320 776f 756c 6420 6265 636f  alues would beco
-00004560: 6d65 2060 3560 2c20 6032 2e35 6020 616e  me `5`, `2.5` an
-00004570: 6420 6074 7275 6560 2c20 7265 7370 6563  d `true`, respec
-00004580: 7469 7665 6c79 2c20 636f 6e76 6572 7465  tively, converte
-00004590: 6420 6672 6f6d 2073 7472 696e 6773 2074  d from strings t
-000045a0: 6f20 7468 6569 7220 636f 7272 6563 7420  o their correct 
-000045b0: 4a53 4f4e 2074 7970 6573 0a0a 2323 2044  JSON types..## D
-000045c0: 6566 6175 6c74 2056 6172 6961 626c 6573  efault Variables
-000045d0: 0a0a 5468 6520 666f 6c6c 6f77 696e 6720  ..The following 
-000045e0: 7375 6273 7469 7475 7469 6f6e 7320 6172  substitutions ar
-000045f0: 6520 6175 746f 6d61 7469 6361 6c6c 7920  e automatically 
-00004600: 6372 6561 7465 6420 616e 6420 6361 6e20  created and can 
-00004610: 6265 2075 7365 6420 696e 2061 6e79 2073  be used in any s
-00004620: 6563 7469 6f6e 206f 6620 7468 6520 636f  ection of the co
-00004630: 6e66 6967 7572 6174 696f 6e20 6669 6c65  nfiguration file
-00004640: 2c20 6f72 2069 6e20 616e 7920 4a53 4f4e  , or in any JSON
-00004650: 2073 7065 6369 6669 6361 7469 6f6e 3a0a   specification:.
-00004660: 0a7c 2044 6972 6563 7469 7665 2020 2020  .| Directive    
-00004670: 2020 207c 2044 6573 6372 6970 7469 6f6e     | Description
-00004680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000046a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000046b0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-000046c0: 4578 616d 706c 6520 6f66 2053 7562 7374  Example of Subst
-000046d0: 6974 7574 696f 6e20 7c0a 7c3a 2d2d 2d2d  itution |.|:----
-000046e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c3a 2d2d  ------------|:--
-000046f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004700: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004710: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004720: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004730: 2d2d 2d2d 2d2d 2d7c 3a2d 2d2d 2d2d 2d2d  -------|:-------
-00004740: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004750: 2d7c 0a7c 2060 7b7b 7573 6572 6e61 6d65  -|.| `{{username
-00004760: 7d7d 6020 207c 2054 6865 2063 7572 7265  }}`  | The curre
-00004770: 6e74 2075 7365 7227 7320 6c6f 6769 6e20  nt user's login 
-00004780: 7573 6572 6e61 6d65 2c20 6c6f 7765 7220  username, lower 
-00004790: 6361 7365 2c20 7370 6163 6573 2072 6570  case, spaces rep
-000047a0: 6c61 6365 6420 2020 2020 2020 2020 2020  laced           
-000047b0: 7c20 6a61 6e65 5f73 6d69 7468 2020 2020  | jane_smith    
-000047c0: 2020 2020 2020 2020 2020 7c0a 7c20 607b            |.| `{
-000047d0: 7b64 6174 657d 7d60 2020 2020 2020 7c20  {date}}`      | 
-000047e0: 5468 6520 6375 7272 656e 7420 6461 7465  The current date
-000047f0: 2028 5554 4329 3a20 5959 5959 4d4d 4444   (UTC): YYYYMMDD
-00004800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004820: 2020 2020 2020 2020 207c 2032 3032 3231           | 20221
-00004830: 3032 3720 2020 2020 2020 2020 2020 2020  027             
-00004840: 2020 207c 0a7c 2060 7b7b 7469 6d65 7d7d     |.| `{{time}}
-00004850: 6020 2020 2020 207c 2054 6865 2063 7572  `      | The cur
-00004860: 7265 6e74 2074 696d 6520 2855 5443 293a  rent time (UTC):
-00004870: 2048 484d 4d53 5320 2020 2020 2020 2020   HHMMSS         
-00004880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000048a0: 2020 7c20 3136 3330 3236 2020 2020 2020    | 163026      
-000048b0: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
-000048c0: 607b 7b64 6174 6574 696d 657d 7d60 2020  `{{datetime}}`  
-000048d0: 7c20 436f 6e63 6174 656e 6174 696f 6e20  | Concatenation 
-000048e0: 6f66 2074 6865 2064 6174 6520 616e 6420  of the date and 
-000048f0: 7469 6d65 2061 626f 7665 2c20 7769 7468  time above, with
-00004900: 2061 2027 2d27 2073 6570 6172 6174 6f72   a '-' separator
-00004910: 2020 2020 2020 2020 2020 207c 2032 3032             | 202
-00004920: 3231 3032 372d 3136 3330 3236 2020 2020  21027-163026    
-00004930: 2020 2020 207c 0a7c 2060 7b7b 7261 6e64       |.| `{{rand
-00004940: 6f6d 7d7d 6020 2020 207c 2041 2072 616e  om}}`    | A ran
-00004950: 646f 6d2c 2074 6872 6565 2064 6967 6974  dom, three digit
-00004960: 2068 6578 6164 6563 696d 616c 206e 756d   hexadecimal num
-00004970: 6265 7220 286c 6f77 6572 2063 6173 6529  ber (lower case)
-00004980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004990: 2020 2020 7c20 6131 6320 2020 2020 2020      | a1c       
-000049a0: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-000049b0: 7c20 607b 7b6e 616d 6573 7061 6365 7d7d  | `{{namespace}}
-000049c0: 6020 7c20 5468 6520 606e 616d 6573 7061  ` | The `namespa
-000049d0: 6365 6020 7072 6f70 6572 7479 2e20 4e6f  ce` property. No
-000049e0: 7465 2074 6861 7420 606e 616d 6573 7061  te that `namespa
-000049f0: 6365 6020 6d75 7374 2c20 6f66 2063 6f75  ce` must, of cou
-00004a00: 7273 652c 2062 6520 7365 742e 207c 206d  rse, be set. | m
-00004a10: 795f 6e61 6d65 7370 6163 6520 2020 2020  y_namespace     
-00004a20: 2020 2020 2020 207c 0a7c 2060 7b7b 7461         |.| `{{ta
-00004a30: 677d 7d60 2020 2020 2020 207c 2054 6865  g}}`       | The
-00004a40: 2060 7461 6760 2070 726f 7065 7274 792e   `tag` property.
-00004a50: 204e 6f74 6520 7468 6174 2060 7461 6760   Note that `tag`
-00004a60: 206d 7573 7420 6265 2073 6574 2e20 2020   must be set.   
-00004a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a80: 2020 2020 2020 7c20 6d79 5f74 6167 2020        | my_tag  
+000001c0: 6573 290a 2020 202a 205b 4854 5450 5320  es).   * [HTTPS 
+000001d0: 5072 6f78 7920 5375 7070 6f72 745d 2823  Proxy Support](#
+000001e0: 6874 7470 732d 7072 6f78 792d 7375 7070  https-proxy-supp
+000001f0: 6f72 7429 0a20 2020 2a20 5b53 7065 6369  ort).   * [Speci
+00000200: 6679 696e 6720 436f 6d6d 6f6e 2050 726f  fying Common Pro
+00000210: 7065 7274 6965 7320 7573 696e 6720 7468  perties using th
+00000220: 6520 436f 6d6d 616e 6420 4c69 6e65 206f  e Command Line o
+00000230: 7220 456e 7669 726f 6e6d 656e 7420 5661  r Environment Va
+00000240: 7269 6162 6c65 735d 2823 7370 6563 6966  riables](#specif
+00000250: 7969 6e67 2d63 6f6d 6d6f 6e2d 7072 6f70  ying-common-prop
+00000260: 6572 7469 6573 2d75 7369 6e67 2d74 6865  erties-using-the
+00000270: 2d63 6f6d 6d61 6e64 2d6c 696e 652d 6f72  -command-line-or
+00000280: 2d65 6e76 6972 6f6e 6d65 6e74 2d76 6172  -environment-var
+00000290: 6961 626c 6573 290a 2020 202a 205b 5661  iables).   * [Va
+000002a0: 7269 6162 6c65 2053 7562 7374 6974 7574  riable Substitut
+000002b0: 696f 6e73 2069 6e20 436f 6d6d 6f6e 2050  ions in Common P
+000002c0: 726f 7065 7274 6965 735d 2823 7661 7269  roperties](#vari
+000002d0: 6162 6c65 2d73 7562 7374 6974 7574 696f  able-substitutio
+000002e0: 6e73 2d69 6e2d 636f 6d6d 6f6e 2d70 726f  ns-in-common-pro
+000002f0: 7065 7274 6965 7329 0a2a 205b 5661 7269  perties).* [Vari
+00000300: 6162 6c65 2053 7562 7374 6974 7574 696f  able Substitutio
+00000310: 6e73 5d28 2376 6172 6961 626c 652d 7375  ns](#variable-su
+00000320: 6273 7469 7475 7469 6f6e 7329 0a20 2020  bstitutions).   
+00000330: 2a20 5b44 6566 6175 6c74 2056 6172 6961  * [Default Varia
+00000340: 626c 6573 5d28 2364 6566 6175 6c74 2d76  bles](#default-v
+00000350: 6172 6961 626c 6573 290a 2020 202a 205b  ariables).   * [
+00000360: 5573 6572 2d44 6566 696e 6564 2056 6172  User-Defined Var
+00000370: 6961 626c 6573 5d28 2375 7365 722d 6465  iables](#user-de
+00000380: 6669 6e65 642d 7661 7269 6162 6c65 7329  fined-variables)
+00000390: 0a20 2020 2a20 5b4e 6573 7465 6420 5661  .   * [Nested Va
+000003a0: 7269 6162 6c65 735d 2823 6e65 7374 6564  riables](#nested
+000003b0: 2d76 6172 6961 626c 6573 290a 2a20 5b57  -variables).* [W
+000003c0: 6f72 6b20 5265 7175 6972 656d 656e 7420  ork Requirement 
+000003d0: 5072 6f70 6572 7469 6573 5d28 2377 6f72  Properties](#wor
+000003e0: 6b2d 7265 7175 6972 656d 656e 742d 7072  k-requirement-pr
+000003f0: 6f70 6572 7469 6573 290a 2020 202a 205b  operties).   * [
+00000400: 576f 726b 2052 6571 7569 7265 6d65 6e74  Work Requirement
+00000410: 204a 534f 4e20 4669 6c65 2053 7472 7563   JSON File Struc
+00000420: 7475 7265 5d28 2377 6f72 6b2d 7265 7175  ture](#work-requ
+00000430: 6972 656d 656e 742d 6a73 6f6e 2d66 696c  irement-json-fil
+00000440: 652d 7374 7275 6374 7572 6529 0a20 2020  e-structure).   
+00000450: 2a20 5b50 726f 7065 7274 7920 496e 6865  * [Property Inhe
+00000460: 7269 7461 6e63 655d 2823 7072 6f70 6572  ritance](#proper
+00000470: 7479 2d69 6e68 6572 6974 616e 6365 290a  ty-inheritance).
+00000480: 2020 202a 205b 576f 726b 2052 6571 7569     * [Work Requi
+00000490: 7265 6d65 6e74 2050 726f 7065 7274 7920  rement Property 
+000004a0: 4469 6374 696f 6e61 7279 5d28 2377 6f72  Dictionary](#wor
+000004b0: 6b2d 7265 7175 6972 656d 656e 742d 7072  k-requirement-pr
+000004c0: 6f70 6572 7479 2d64 6963 7469 6f6e 6172  operty-dictionar
+000004d0: 7929 0a20 2020 2a20 5b41 7574 6f6d 6174  y).   * [Automat
+000004e0: 6963 2050 726f 7065 7274 6965 735d 2823  ic Properties](#
+000004f0: 6175 746f 6d61 7469 632d 7072 6f70 6572  automatic-proper
+00000500: 7469 6573 290a 2020 2020 2020 2a20 5b57  ties).      * [W
+00000510: 6f72 6b20 5265 7175 6972 656d 656e 742c  ork Requirement,
+00000520: 2054 6173 6b20 4772 6f75 7020 616e 6420   Task Group and 
+00000530: 5461 736b 204e 616d 696e 675d 2823 776f  Task Naming](#wo
+00000540: 726b 2d72 6571 7569 7265 6d65 6e74 2d74  rk-requirement-t
+00000550: 6173 6b2d 6772 6f75 702d 616e 642d 7461  ask-group-and-ta
+00000560: 736b 2d6e 616d 696e 6729 0a20 2020 2020  sk-naming).     
+00000570: 202a 205b 5461 736b 2054 7970 6573 5d28   * [Task Types](
+00000580: 2374 6173 6b2d 7479 7065 7329 0a20 2020  #task-types).   
+00000590: 2020 2020 2020 2a20 5b42 6173 682c 2050        * [Bash, P
+000005a0: 7974 686f 6e2c 2050 6f77 6572 5368 656c  ython, PowerShel
+000005b0: 6c20 616e 6420 636d 642f 6261 7420 5461  l and cmd/bat Ta
+000005c0: 736b 735d 2823 6261 7368 2d70 7974 686f  sks](#bash-pytho
+000005d0: 6e2d 706f 7765 7273 6865 6c6c 2d61 6e64  n-powershell-and
+000005e0: 2d63 6d64 6261 742d 7461 736b 7329 0a20  -cmdbat-tasks). 
+000005f0: 2020 2020 2020 2020 2a20 5b44 6f63 6b65          * [Docke
+00000600: 7220 5461 736b 735d 2823 646f 636b 6572  r Tasks](#docker
+00000610: 2d74 6173 6b73 290a 2020 2020 2020 2020  -tasks).        
+00000620: 202a 205b 4261 7368 2c20 5079 7468 6f6e   * [Bash, Python
+00000630: 2c20 506f 7765 7253 6865 6c6c 2c20 636d  , PowerShell, cm
+00000640: 642e 6578 652f 6261 7463 682c 2061 6e64  d.exe/batch, and
+00000650: 2044 6f63 6b65 7220 7769 7468 6f75 7420   Docker without 
+00000660: 4175 746f 6d61 7469 6320 5072 6f63 6573  Automatic Proces
+00000670: 7369 6e67 5d28 2362 6173 682d 7079 7468  sing](#bash-pyth
+00000680: 6f6e 2d70 6f77 6572 7368 656c 6c2d 636d  on-powershell-cm
+00000690: 6465 7865 6261 7463 682d 616e 642d 646f  dexebatch-and-do
+000006a0: 636b 6572 2d77 6974 686f 7574 2d61 7574  cker-without-aut
+000006b0: 6f6d 6174 6963 2d70 726f 6365 7373 696e  omatic-processin
+000006c0: 6729 0a20 2020 2020 202a 205b 5461 736b  g).      * [Task
+000006d0: 2043 6f75 6e74 735d 2823 7461 736b 2d63   Counts](#task-c
+000006e0: 6f75 6e74 7329 0a20 2020 2a20 5b45 7861  ounts).   * [Exa
+000006f0: 6d70 6c65 735d 2823 6578 616d 706c 6573  mples](#examples
+00000700: 290a 2020 2020 2020 2a20 5b54 4f4d 4c20  ).      * [TOML 
+00000710: 5072 6f70 6572 7469 6573 2069 6e20 7468  Properties in th
+00000720: 6520 776f 726b 5265 7175 6972 656d 656e  e workRequiremen
+00000730: 7420 5365 6374 696f 6e5d 2823 746f 6d6c  t Section](#toml
+00000740: 2d70 726f 7065 7274 6965 732d 696e 2d74  -properties-in-t
+00000750: 6865 2d77 6f72 6b72 6571 7569 7265 6d65  he-workrequireme
+00000760: 6e74 2d73 6563 7469 6f6e 290a 2020 2020  nt-section).    
+00000770: 2020 2a20 5b4a 534f 4e20 5072 6f70 6572    * [JSON Proper
+00000780: 7469 6573 2061 7420 7468 6520 576f 726b  ties at the Work
+00000790: 2052 6571 7569 7265 6d65 6e74 204c 6576   Requirement Lev
+000007a0: 656c 5d28 236a 736f 6e2d 7072 6f70 6572  el](#json-proper
+000007b0: 7469 6573 2d61 742d 7468 652d 776f 726b  ties-at-the-work
+000007c0: 2d72 6571 7569 7265 6d65 6e74 2d6c 6576  -requirement-lev
+000007d0: 656c 290a 2020 2020 2020 2a20 5b4a 534f  el).      * [JSO
+000007e0: 4e20 5072 6f70 6572 7469 6573 2061 7420  N Properties at 
+000007f0: 7468 6520 5461 736b 2047 726f 7570 204c  the Task Group L
+00000800: 6576 656c 5d28 236a 736f 6e2d 7072 6f70  evel](#json-prop
+00000810: 6572 7469 6573 2d61 742d 7468 652d 7461  erties-at-the-ta
+00000820: 736b 2d67 726f 7570 2d6c 6576 656c 290a  sk-group-level).
+00000830: 2020 2020 2020 2a20 5b4a 534f 4e20 5072        * [JSON Pr
+00000840: 6f70 6572 7469 6573 2061 7420 7468 6520  operties at the 
+00000850: 5461 736b 204c 6576 656c 5d28 236a 736f  Task Level](#jso
+00000860: 6e2d 7072 6f70 6572 7469 6573 2d61 742d  n-properties-at-
+00000870: 7468 652d 7461 736b 2d6c 6576 656c 290a  the-task-level).
+00000880: 2020 202a 205b 5661 7269 6162 6c65 2053     * [Variable S
+00000890: 7562 7374 6974 7574 696f 6e73 2069 6e20  ubstitutions in 
+000008a0: 576f 726b 2052 6571 7569 7265 6d65 6e74  Work Requirement
+000008b0: 2050 726f 7065 7274 6965 735d 2823 7661   Properties](#va
+000008c0: 7269 6162 6c65 2d73 7562 7374 6974 7574  riable-substitut
+000008d0: 696f 6e73 2d69 6e2d 776f 726b 2d72 6571  ions-in-work-req
+000008e0: 7569 7265 6d65 6e74 2d70 726f 7065 7274  uirement-propert
+000008f0: 6965 7329 0a20 2020 2020 202a 205b 5461  ies).      * [Ta
+00000900: 736b 2061 6e64 2054 6173 6b20 4772 6f75  sk and Task Grou
+00000910: 7020 4e61 6d65 2053 7562 7374 6974 7574  p Name Substitut
+00000920: 696f 6e5d 2823 7461 736b 2d61 6e64 2d74  ion](#task-and-t
+00000930: 6173 6b2d 6772 6f75 702d 6e61 6d65 2d73  ask-group-name-s
+00000940: 7562 7374 6974 7574 696f 6e29 0a20 2020  ubstitution).   
+00000950: 2020 202a 205b 576f 726b 2052 6571 7569     * [Work Requi
+00000960: 7265 6d65 6e74 204e 616d 6520 5375 6273  rement Name Subs
+00000970: 7469 7475 7469 6f6e 5d28 2377 6f72 6b2d  titution](#work-
+00000980: 7265 7175 6972 656d 656e 742d 6e61 6d65  requirement-name
+00000990: 2d73 7562 7374 6974 7574 696f 6e29 0a20  -substitution). 
+000009a0: 2020 2a20 5b44 7279 2d52 756e 6e69 6e67    * [Dry-Running
+000009b0: 2057 6f72 6b20 5265 7175 6972 656d 656e   Work Requiremen
+000009c0: 7420 5375 626d 6973 7369 6f6e 735d 2823  t Submissions](#
+000009d0: 6472 792d 7275 6e6e 696e 672d 776f 726b  dry-running-work
+000009e0: 2d72 6571 7569 7265 6d65 6e74 2d73 7562  -requirement-sub
+000009f0: 6d69 7373 696f 6e73 290a 2020 2020 2020  missions).      
+00000a00: 2a20 5b53 7562 6d69 7474 696e 6720 2752  * [Submitting 'R
+00000a10: 6177 2720 4a53 4f4e 2057 6f72 6b20 5265  aw' JSON Work Re
+00000a20: 7175 6972 656d 656e 7420 5370 6563 6966  quirement Specif
+00000a30: 6963 6174 696f 6e73 5d28 2373 7562 6d69  ications](#submi
+00000a40: 7474 696e 672d 7261 772d 6a73 6f6e 2d77  tting-raw-json-w
+00000a50: 6f72 6b2d 7265 7175 6972 656d 656e 742d  ork-requirement-
+00000a60: 7370 6563 6966 6963 6174 696f 6e73 290a  specifications).
+00000a70: 2020 202a 205b 4669 6c65 2053 746f 7261     * [File Stora
+00000a80: 6765 204c 6f63 6174 696f 6e73 2061 6e64  ge Locations and
+00000a90: 2046 696c 6520 5573 6167 655d 2823 6669   File Usage](#fi
+00000aa0: 6c65 2d73 746f 7261 6765 2d6c 6f63 6174  le-storage-locat
+00000ab0: 696f 6e73 2d61 6e64 2d66 696c 652d 7573  ions-and-file-us
+00000ac0: 6167 6529 0a20 2020 2020 202a 205b 4669  age).      * [Fi
+00000ad0: 6c65 7320 5570 6c6f 6164 6564 2074 6f20  les Uploaded to 
+00000ae0: 7468 6520 4f62 6a65 6374 2053 746f 7265  the Object Store
+00000af0: 2066 726f 6d20 4c6f 6361 6c20 5374 6f72   from Local Stor
+00000b00: 6167 655d 2823 6669 6c65 732d 7570 6c6f  age](#files-uplo
+00000b10: 6164 6564 2d74 6f2d 7468 652d 6f62 6a65  aded-to-the-obje
+00000b20: 6374 2d73 746f 7265 2d66 726f 6d2d 6c6f  ct-store-from-lo
+00000b30: 6361 6c2d 7374 6f72 6167 6529 0a20 2020  cal-storage).   
+00000b40: 2020 2020 2020 2a20 5b46 696c 6573 2069        * [Files i
+00000b50: 6e20 7468 6520 696e 7075 7473 204c 6973  n the inputs Lis
+00000b60: 745d 2823 6669 6c65 732d 696e 2d74 6865  t](#files-in-the
+00000b70: 2d69 6e70 7574 732d 6c69 7374 290a 2020  -inputs-list).  
+00000b80: 2020 2020 2020 202a 205b 4669 6c65 7320         * [Files 
+00000b90: 696e 2074 6865 2075 706c 6f61 6446 696c  in the uploadFil
+00000ba0: 6573 204c 6973 745d 2823 6669 6c65 732d  es List](#files-
+00000bb0: 696e 2d74 6865 2d75 706c 6f61 6466 696c  in-the-uploadfil
+00000bc0: 6573 2d6c 6973 7429 0a20 2020 2020 202a  es-list).      *
+00000bd0: 205b 4669 6c65 2044 6570 656e 6465 6e63   [File Dependenc
+00000be0: 6965 7320 5573 696e 6720 7665 7269 6679  ies Using verify
+00000bf0: 4174 5374 6172 7420 616e 6420 7665 7269  AtStart and veri
+00000c00: 6679 5761 6974 5d28 2366 696c 652d 6465  fyWait](#file-de
+00000c10: 7065 6e64 656e 6369 6573 2d75 7369 6e67  pendencies-using
+00000c20: 2d76 6572 6966 7961 7473 7461 7274 2d61  -verifyatstart-a
+00000c30: 6e64 2d76 6572 6966 7977 6169 7429 0a20  nd-verifywait). 
+00000c40: 2020 2020 202a 205b 4669 6c65 7320 446f       * [Files Do
+00000c50: 776e 6c6f 6164 6564 2055 7369 6e67 2069  wnloaded Using i
+00000c60: 6e70 7574 734f 7074 696f 6e61 6c5d 2823  nputsOptional](#
+00000c70: 6669 6c65 732d 646f 776e 6c6f 6164 6564  files-downloaded
+00000c80: 2d75 7369 6e67 2d69 6e70 7574 736f 7074  -using-inputsopt
+00000c90: 696f 6e61 6c29 0a20 2020 2020 202a 205b  ional).      * [
+00000ca0: 4669 6c65 7320 446f 776e 6c6f 6164 6564  Files Downloaded
+00000cb0: 2074 6f20 6120 4e6f 6465 2066 6f72 2075   to a Node for u
+00000cc0: 7365 2069 6e20 5461 736b 2045 7865 6375  se in Task Execu
+00000cd0: 7469 6f6e 5d28 2366 696c 6573 2d64 6f77  tion](#files-dow
+00000ce0: 6e6c 6f61 6465 642d 746f 2d61 2d6e 6f64  nloaded-to-a-nod
+00000cf0: 652d 666f 722d 7573 652d 696e 2d74 6173  e-for-use-in-tas
+00000d00: 6b2d 6578 6563 7574 696f 6e29 0a20 2020  k-execution).   
+00000d10: 2020 202a 205b 4669 6c65 7320 5570 6c6f     * [Files Uplo
+00000d20: 6164 6564 2066 726f 6d20 6120 4e6f 6465  aded from a Node
+00000d30: 2074 6f20 7468 6520 4f62 6a65 6374 2053   to the Object S
+00000d40: 746f 7265 2061 6674 6572 2054 6173 6b20  tore after Task 
+00000d50: 4578 6563 7574 696f 6e5d 2823 6669 6c65  Execution](#file
+00000d60: 732d 7570 6c6f 6164 6564 2d66 726f 6d2d  s-uploaded-from-
+00000d70: 612d 6e6f 6465 2d74 6f2d 7468 652d 6f62  a-node-to-the-ob
+00000d80: 6a65 6374 2d73 746f 7265 2d61 6674 6572  ject-store-after
+00000d90: 2d74 6173 6b2d 6578 6563 7574 696f 6e29  -task-execution)
+00000da0: 0a20 2020 2020 202a 205b 4669 6c65 7320  .      * [Files 
+00000db0: 446f 776e 6c6f 6164 6564 2066 726f 6d20  Downloaded from 
+00000dc0: 7468 6520 4f62 6a65 6374 2053 746f 7265  the Object Store
+00000dd0: 2074 6f20 4c6f 6361 6c20 5374 6f72 6167   to Local Storag
+00000de0: 655d 2823 6669 6c65 732d 646f 776e 6c6f  e](#files-downlo
+00000df0: 6164 6564 2d66 726f 6d2d 7468 652d 6f62  aded-from-the-ob
+00000e00: 6a65 6374 2d73 746f 7265 2d74 6f2d 6c6f  ject-store-to-lo
+00000e10: 6361 6c2d 7374 6f72 6167 6529 0a20 2020  cal-storage).   
+00000e20: 2a20 5b54 6173 6b20 4578 6563 7574 696f  * [Task Executio
+00000e30: 6e20 436f 6e74 6578 745d 2823 7461 736b  n Context](#task
+00000e40: 2d65 7865 6375 7469 6f6e 2d63 6f6e 7465  -execution-conte
+00000e50: 7874 290a 2020 2020 2020 2a20 5b54 6173  xt).      * [Tas
+00000e60: 6b20 4578 6563 7574 696f 6e20 5374 6570  k Execution Step
+00000e70: 735d 2823 7461 736b 2d65 7865 6375 7469  s](#task-executi
+00000e80: 6f6e 2d73 7465 7073 290a 2020 2020 2020  on-steps).      
+00000e90: 2a20 5b54 6865 2055 7365 7220 616e 6420  * [The User and 
+00000ea0: 4772 6f75 7020 7573 6564 2066 6f72 2054  Group used for T
+00000eb0: 6173 6b73 5d28 2374 6865 2d75 7365 722d  asks](#the-user-
+00000ec0: 616e 642d 6772 6f75 702d 7573 6564 2d66  and-group-used-f
+00000ed0: 6f72 2d74 6173 6b73 290a 2020 2020 2020  or-tasks).      
+00000ee0: 2a20 5b48 6f6d 6520 4469 7265 6374 6f72  * [Home Director
+00000ef0: 7920 666f 7220 7964 2d61 6765 6e74 5d28  y for yd-agent](
+00000f00: 2368 6f6d 652d 6469 7265 6374 6f72 792d  #home-directory-
+00000f10: 666f 722d 7964 2d61 6765 6e74 290a 2020  for-yd-agent).  
+00000f20: 2020 2020 2a20 5b54 6173 6b20 4578 6563      * [Task Exec
+00000f30: 7574 696f 6e20 4469 7265 6374 6f72 795d  ution Directory]
+00000f40: 2823 7461 736b 2d65 7865 6375 7469 6f6e  (#task-execution
+00000f50: 2d64 6972 6563 746f 7279 290a 2020 202a  -directory).   *
+00000f60: 205b 5370 6563 6966 7969 6e67 2057 6f72   [Specifying Wor
+00000f70: 6b20 5265 7175 6972 656d 656e 7473 2075  k Requirements u
+00000f80: 7369 6e67 2043 5356 2044 6174 615d 2823  sing CSV Data](#
+00000f90: 7370 6563 6966 7969 6e67 2d77 6f72 6b2d  specifying-work-
+00000fa0: 7265 7175 6972 656d 656e 7473 2d75 7369  requirements-usi
+00000fb0: 6e67 2d63 7376 2d64 6174 6129 0a20 2020  ng-csv-data).   
+00000fc0: 2020 202a 205b 576f 726b 2052 6571 7569     * [Work Requi
+00000fd0: 7265 6d65 6e74 2043 5356 2044 6174 6120  rement CSV Data 
+00000fe0: 4578 616d 706c 655d 2823 776f 726b 2d72  Example](#work-r
+00000ff0: 6571 7569 7265 6d65 6e74 2d63 7376 2d64  equirement-csv-d
+00001000: 6174 612d 6578 616d 706c 6529 0a20 2020  ata-example).   
+00001010: 2020 202a 205b 4353 5620 5661 7269 6162     * [CSV Variab
+00001020: 6c65 2053 7562 7374 6974 7574 696f 6e73  le Substitutions
+00001030: 5d28 2363 7376 2d76 6172 6961 626c 652d  ](#csv-variable-
+00001040: 7375 6273 7469 7475 7469 6f6e 7329 0a20  substitutions). 
+00001050: 2020 2020 202a 205b 5072 6f70 6572 7479       * [Property
+00001060: 2049 6e68 6572 6974 616e 6365 5d28 2370   Inheritance](#p
+00001070: 726f 7065 7274 792d 696e 6865 7269 7461  roperty-inherita
+00001080: 6e63 652d 3129 0a20 2020 2020 202a 205b  nce-1).      * [
+00001090: 4d75 6c74 6970 6c65 2054 6173 6b20 4772  Multiple Task Gr
+000010a0: 6f75 7073 2075 7369 6e67 204d 756c 7469  oups using Multi
+000010b0: 706c 6520 4353 5620 4669 6c65 735d 2823  ple CSV Files](#
+000010c0: 6d75 6c74 6970 6c65 2d74 6173 6b2d 6772  multiple-task-gr
+000010d0: 6f75 7073 2d75 7369 6e67 2d6d 756c 7469  oups-using-multi
+000010e0: 706c 652d 6373 762d 6669 6c65 7329 0a20  ple-csv-files). 
+000010f0: 2020 2020 202a 205b 5573 696e 6720 4353       * [Using CS
+00001100: 5620 4461 7461 2077 6974 6820 5369 6d70  V Data with Simp
+00001110: 6c65 2c20 544f 4d4c 2d4f 6e6c 7920 576f  le, TOML-Only Wo
+00001120: 726b 2052 6571 7569 7265 6d65 6e74 2053  rk Requirement S
+00001130: 7065 6369 6669 6361 7469 6f6e 735d 2823  pecifications](#
+00001140: 7573 696e 672d 6373 762d 6461 7461 2d77  using-csv-data-w
+00001150: 6974 682d 7369 6d70 6c65 2d74 6f6d 6c2d  ith-simple-toml-
+00001160: 6f6e 6c79 2d77 6f72 6b2d 7265 7175 6972  only-work-requir
+00001170: 656d 656e 742d 7370 6563 6966 6963 6174  ement-specificat
+00001180: 696f 6e73 290a 2020 2020 2020 2a20 5b49  ions).      * [I
+00001190: 6e73 7065 6374 696e 6720 7468 6520 5265  nspecting the Re
+000011a0: 7375 6c74 7320 6f66 2043 5356 2056 6172  sults of CSV Var
+000011b0: 6961 626c 6520 5375 6273 7469 7475 7469  iable Substituti
+000011c0: 6f6e 5d28 2369 6e73 7065 6374 696e 672d  on](#inspecting-
+000011d0: 7468 652d 7265 7375 6c74 732d 6f66 2d63  the-results-of-c
+000011e0: 7376 2d76 6172 6961 626c 652d 7375 6273  sv-variable-subs
+000011f0: 7469 7475 7469 6f6e 290a 2a20 5b57 6f72  titution).* [Wor
+00001200: 6b65 7220 506f 6f6c 2050 726f 7065 7274  ker Pool Propert
+00001210: 6965 735d 2823 776f 726b 6572 2d70 6f6f  ies](#worker-poo
+00001220: 6c2d 7072 6f70 6572 7469 6573 290a 2020  l-properties).  
+00001230: 202a 205b 4175 746f 6d61 7469 6320 5072   * [Automatic Pr
+00001240: 6f70 6572 7469 6573 5d28 2361 7574 6f6d  operties](#autom
+00001250: 6174 6963 2d70 726f 7065 7274 6965 732d  atic-properties-
+00001260: 3129 0a20 2020 2a20 5b54 4f4d 4c20 5072  1).   * [TOML Pr
+00001270: 6f70 6572 7469 6573 2069 6e20 7468 6520  operties in the 
+00001280: 776f 726b 6572 506f 6f6c 2053 6563 7469  workerPool Secti
+00001290: 6f6e 5d28 2374 6f6d 6c2d 7072 6f70 6572  on](#toml-proper
+000012a0: 7469 6573 2d69 6e2d 7468 652d 776f 726b  ties-in-the-work
+000012b0: 6572 706f 6f6c 2d73 6563 7469 6f6e 290a  erpool-section).
+000012c0: 2020 202a 205b 576f 726b 6572 2050 6f6f     * [Worker Poo
+000012d0: 6c20 5370 6563 6966 6963 6174 696f 6e20  l Specification 
+000012e0: 5573 696e 6720 4a53 4f4e 2044 6f63 756d  Using JSON Docum
+000012f0: 656e 7473 5d28 2377 6f72 6b65 722d 706f  ents](#worker-po
+00001300: 6f6c 2d73 7065 6369 6669 6361 7469 6f6e  ol-specification
+00001310: 2d75 7369 6e67 2d6a 736f 6e2d 646f 6375  -using-json-docu
+00001320: 6d65 6e74 7329 0a20 2020 2020 202a 205b  ments).      * [
+00001330: 576f 726b 6572 2050 6f6f 6c20 4a53 4f4e  Worker Pool JSON
+00001340: 2045 7861 6d70 6c65 735d 2823 776f 726b   Examples](#work
+00001350: 6572 2d70 6f6f 6c2d 6a73 6f6e 2d65 7861  er-pool-json-exa
+00001360: 6d70 6c65 7329 0a20 2020 2020 202a 205b  mples).      * [
+00001370: 544f 4d4c 2050 726f 7065 7274 6965 7320  TOML Properties 
+00001380: 496e 6865 7269 7465 6420 6279 2057 6f72  Inherited by Wor
+00001390: 6b65 7220 506f 6f6c 204a 534f 4e20 5370  ker Pool JSON Sp
+000013a0: 6563 6966 6963 6174 696f 6e73 5d28 2374  ecifications](#t
+000013b0: 6f6d 6c2d 7072 6f70 6572 7469 6573 2d69  oml-properties-i
+000013c0: 6e68 6572 6974 6564 2d62 792d 776f 726b  nherited-by-work
+000013d0: 6572 2d70 6f6f 6c2d 6a73 6f6e 2d73 7065  er-pool-json-spe
+000013e0: 6369 6669 6361 7469 6f6e 7329 0a20 2020  cifications).   
+000013f0: 2a20 5b56 6172 6961 626c 6520 5375 6273  * [Variable Subs
+00001400: 7469 7475 7469 6f6e 7320 696e 2057 6f72  titutions in Wor
+00001410: 6b65 7220 506f 6f6c 2050 726f 7065 7274  ker Pool Propert
+00001420: 6965 735d 2823 7661 7269 6162 6c65 2d73  ies](#variable-s
+00001430: 7562 7374 6974 7574 696f 6e73 2d69 6e2d  ubstitutions-in-
+00001440: 776f 726b 6572 2d70 6f6f 6c2d 7072 6f70  worker-pool-prop
+00001450: 6572 7469 6573 290a 2020 202a 205b 4472  erties).   * [Dr
+00001460: 792d 5275 6e6e 696e 6720 576f 726b 6572  y-Running Worker
+00001470: 2050 6f6f 6c20 5072 6f76 6973 696f 6e69   Pool Provisioni
+00001480: 6e67 5d28 2364 7279 2d72 756e 6e69 6e67  ng](#dry-running
+00001490: 2d77 6f72 6b65 722d 706f 6f6c 2d70 726f  -worker-pool-pro
+000014a0: 7669 7369 6f6e 696e 6729 0a2a 205b 4a73  visioning).* [Js
+000014b0: 6f6e 6e65 7420 5375 7070 6f72 745d 2823  onnet Support](#
+000014c0: 6a73 6f6e 6e65 742d 7375 7070 6f72 7429  jsonnet-support)
+000014d0: 0a20 2020 2a20 5b4a 736f 6e6e 6574 2049  .   * [Jsonnet I
+000014e0: 6e73 7461 6c6c 6174 696f 6e5d 2823 6a73  nstallation](#js
+000014f0: 6f6e 6e65 742d 696e 7374 616c 6c61 7469  onnet-installati
+00001500: 6f6e 290a 2020 202a 205b 5661 7269 6162  on).   * [Variab
+00001510: 6c65 2053 7562 7374 6974 7574 696f 6e73  le Substitutions
+00001520: 2069 6e20 4a73 6f6e 6e65 7420 4669 6c65   in Jsonnet File
+00001530: 735d 2823 7661 7269 6162 6c65 2d73 7562  s](#variable-sub
+00001540: 7374 6974 7574 696f 6e73 2d69 6e2d 6a73  stitutions-in-js
+00001550: 6f6e 6e65 742d 6669 6c65 7329 0a20 2020  onnet-files).   
+00001560: 2a20 5b43 6865 636b 696e 6720 4a73 6f6e  * [Checking Json
+00001570: 6e65 7420 5072 6f63 6573 7369 6e67 5d28  net Processing](
+00001580: 2363 6865 636b 696e 672d 6a73 6f6e 6e65  #checking-jsonne
+00001590: 742d 7072 6f63 6573 7369 6e67 290a 2020  t-processing).  
+000015a0: 202a 205b 4a73 6f6e 6e65 7420 4578 616d   * [Jsonnet Exam
+000015b0: 706c 655d 2823 6a73 6f6e 6e65 742d 6578  ple](#jsonnet-ex
+000015c0: 616d 706c 6529 0a2a 205b 436f 6d6d 616e  ample).* [Comman
+000015d0: 6420 4c69 7374 5d28 2363 6f6d 6d61 6e64  d List](#command
+000015e0: 2d6c 6973 7429 0a20 2020 2a20 5b79 642d  -list).   * [yd-
+000015f0: 7375 626d 6974 5d28 2379 642d 7375 626d  submit](#yd-subm
+00001600: 6974 290a 2020 202a 205b 7964 2d70 726f  it).   * [yd-pro
+00001610: 7669 7369 6f6e 5d28 2379 642d 7072 6f76  vision](#yd-prov
+00001620: 6973 696f 6e29 0a20 2020 2a20 5b79 642d  ision).   * [yd-
+00001630: 6361 6e63 656c 5d28 2379 642d 6361 6e63  cancel](#yd-canc
+00001640: 656c 290a 2020 202a 205b 7964 2d61 626f  el).   * [yd-abo
+00001650: 7274 5d28 2379 642d 6162 6f72 7429 0a20  rt](#yd-abort). 
+00001660: 2020 2a20 5b79 642d 646f 776e 6c6f 6164    * [yd-download
+00001670: 5d28 2379 642d 646f 776e 6c6f 6164 290a  ](#yd-download).
+00001680: 2020 202a 205b 7964 2d64 656c 6574 655d     * [yd-delete]
+00001690: 2823 7964 2d64 656c 6574 6529 0a20 2020  (#yd-delete).   
+000016a0: 2a20 5b79 642d 7570 6c6f 6164 5d28 2379  * [yd-upload](#y
+000016b0: 642d 7570 6c6f 6164 290a 2020 202a 205b  d-upload).   * [
+000016c0: 7964 2d73 6875 7464 6f77 6e5d 2823 7964  yd-shutdown](#yd
+000016d0: 2d73 6875 7464 6f77 6e29 0a20 2020 2a20  -shutdown).   * 
+000016e0: 5b79 642d 696e 7374 616e 7469 6174 655d  [yd-instantiate]
+000016f0: 2823 7964 2d69 6e73 7461 6e74 6961 7465  (#yd-instantiate
+00001700: 290a 2020 2020 2020 2a20 5b54 6573 742d  ).      * [Test-
+00001710: 5275 6e6e 696e 6720 6120 4479 6e61 6d69  Running a Dynami
+00001720: 6320 5465 6d70 6c61 7465 5d28 2374 6573  c Template](#tes
+00001730: 742d 7275 6e6e 696e 672d 612d 6479 6e61  t-running-a-dyna
+00001740: 6d69 632d 7465 6d70 6c61 7465 290a 2020  mic-template).  
+00001750: 202a 205b 7964 2d74 6572 6d69 6e61 7465   * [yd-terminate
+00001760: 5d28 2379 642d 7465 726d 696e 6174 6529  ](#yd-terminate)
+00001770: 0a0a 3c21 2d2d 2041 6464 6564 2062 793a  ..<!-- Added by:
+00001780: 2070 7774 2c20 6174 3a20 5475 6520 4a75   pwt, at: Tue Ju
+00001790: 6e20 3230 2031 363a 3139 3a35 3120 4253  n 20 16:19:51 BS
+000017a0: 5420 3230 3233 202d 2d3e 0a0a 3c21 2d2d  T 2023 -->..<!--
+000017b0: 7465 2d2d 3e0a 0a23 204f 7665 7276 6965  te-->..# Overvie
+000017c0: 770a 0a54 6869 7320 7265 706f 7369 746f  w..This reposito
+000017d0: 7279 2063 6f6e 7461 696e 7320 6120 7365  ry contains a se
+000017e0: 7420 6f66 2065 7861 6d70 6c65 2050 7974  t of example Pyt
+000017f0: 686f 6e20 7363 7269 7074 7320 666f 7220  hon scripts for 
+00001800: 696e 7465 7261 6374 696e 6720 7769 7468  interacting with
+00001810: 2074 6865 2059 656c 6c6f 7744 6f67 2050   the YellowDog P
+00001820: 6c61 7466 6f72 6d2e 2054 6865 2073 6372  latform. The scr
+00001830: 6970 7473 2075 7365 2074 6865 202a 2a5b  ipts use the **[
+00001840: 5965 6c6c 6f77 446f 6720 5079 7468 6f6e  YellowDog Python
+00001850: 2053 444b 5d28 6874 7470 733a 2f2f 646f   SDK](https://do
+00001860: 6373 2e79 656c 6c6f 7764 6f67 2e63 6f2f  cs.yellowdog.co/
+00001870: 6170 692f 7079 7468 6f6e 2f69 6e64 6578  api/python/index
+00001880: 2e68 746d 6c29 2a2a 2c20 7468 6520 636f  .html)**, the co
+00001890: 6465 2066 6f72 2077 6869 6368 2063 616e  de for which can
+000018a0: 2062 6520 666f 756e 6420 5b6f 6e20 4769   be found [on Gi
+000018b0: 7448 7562 5d28 6874 7470 733a 2f2f 6769  tHub](https://gi
+000018c0: 7468 7562 2e63 6f6d 2f79 656c 6c6f 7764  thub.com/yellowd
+000018d0: 6f67 2f79 656c 6c6f 7764 6f67 2d73 646b  og/yellowdog-sdk
+000018e0: 2d70 7974 686f 6e2d 7075 626c 6963 292e  -python-public).
+000018f0: 0a0a 0a2a 284e 6f74 653a 2074 6865 7365  ...*(Note: these
+00001900: 2073 6372 6970 7473 2061 7265 2069 6e74   scripts are int
+00001910: 656e 6465 6420 746f 2062 6520 6120 6865  ended to be a he
+00001920: 6c70 6675 6c20 7374 6172 7469 6e67 2070  lpful starting p
+00001930: 6f69 6e74 2066 6f72 2065 7870 6572 696d  oint for experim
+00001940: 656e 7469 6e67 2077 6974 6820 7468 6520  enting with the 
+00001950: 5965 6c6c 6f77 446f 6720 506c 6174 666f  YellowDog Platfo
+00001960: 726d 2e20 5468 6579 2061 7265 206e 6f74  rm. They are not
+00001970: 2061 7373 7572 6564 2074 6f20 6265 206f   assured to be o
+00001980: 6620 7072 6f64 7563 7469 6f6e 2071 7561  f production qua
+00001990: 6c69 7479 206e 6f72 2064 6f20 7468 6579  lity nor do they
+000019a0: 2072 6570 7265 7365 6e74 2061 2073 7461   represent a sta
+000019b0: 6e64 6172 6420 6f72 2072 6563 6f6d 6d65  ndard or recomme
+000019c0: 6e64 6564 206d 6574 686f 6420 666f 7220  nded method for 
+000019d0: 7573 696e 6720 5965 6c6c 6f77 446f 672e  using YellowDog.
+000019e0: 292a 0a0a 5468 6973 2064 6f63 756d 656e  )*..This documen
+000019f0: 7461 7469 6f6e 2073 686f 756c 6420 6265  tation should be
+00001a00: 2072 6561 6420 696e 2063 6f6e 6a75 6e63   read in conjunc
+00001a10: 7469 6f6e 2077 6974 6820 7468 6520 6d61  tion with the ma
+00001a20: 696e 202a 2a5b 5965 6c6c 6f77 446f 6720  in **[YellowDog 
+00001a30: 446f 6375 6d65 6e74 6174 696f 6e5d 2868  Documentation](h
+00001a40: 7474 7073 3a2f 2f64 6f63 732e 7965 6c6c  ttps://docs.yell
+00001a50: 6f77 646f 672e 636f 292a 2a2c 2077 6869  owdog.co)**, whi
+00001a60: 6368 2070 726f 7669 6465 7320 6120 636f  ch provides a co
+00001a70: 6d70 7265 6865 6e73 6976 6520 6465 7363  mprehensive desc
+00001a80: 7269 7074 696f 6e20 6f66 2074 6865 2063  ription of the c
+00001a90: 6f6e 6365 7074 7320 616e 6420 6f70 6572  oncepts and oper
+00001aa0: 6174 696f 6e20 6f66 2074 6865 2059 656c  ation of the Yel
+00001ab0: 6c6f 7744 6f67 2050 6c61 7466 6f72 6d2e  lowDog Platform.
+00001ac0: 0a0a 5465 6d70 6c61 7465 2073 6f6c 7574  ..Template solut
+00001ad0: 696f 6e73 2066 6f72 2065 7870 6572 696d  ions for experim
+00001ae0: 656e 7469 6e67 2077 6974 6820 7468 6573  enting with thes
+00001af0: 6520 7363 7269 7074 7320 6361 6e20 6265  e scripts can be
+00001b00: 2066 6f75 6e64 2069 6e20 7468 6520 2a2a   found in the **
+00001b10: 5b70 7974 686f 6e2d 6578 616d 706c 6573  [python-examples
+00001b20: 2d74 656d 706c 6174 6573 5d28 6874 7470  -templates](http
+00001b30: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f79  s://github.com/y
+00001b40: 656c 6c6f 7764 6f67 2f70 7974 686f 6e2d  ellowdog/python-
+00001b50: 6578 616d 706c 6573 2d74 656d 706c 6174  examples-templat
+00001b60: 6573 292a 2a20 7265 706f 7369 746f 7279  es)** repository
+00001b70: 2e0a 0a54 6865 2073 6372 6970 7473 2070  ...The scripts p
+00001b80: 726f 7669 6465 2074 6865 2066 6f6c 6c6f  rovide the follo
+00001b90: 7769 6e67 2063 6170 6162 696c 6974 6965  wing capabilitie
+00001ba0: 733a 0a0a 2d20 2a2a 5072 6f76 6973 696f  s:..- **Provisio
+00001bb0: 6e69 6e67 2a2a 2057 6f72 6b65 7220 506f  ning** Worker Po
+00001bc0: 6f6c 7320 7769 7468 2074 6865 202a 2a60  ols with the **`
+00001bd0: 7964 2d70 726f 7669 7369 6f6e 602a 2a20  yd-provision`** 
+00001be0: 636f 6d6d 616e 640a 2d20 2a2a 5375 626d  command.- **Subm
+00001bf0: 6974 7469 6e67 2a2a 2057 6f72 6b20 5265  itting** Work Re
+00001c00: 7175 6972 656d 656e 7473 2077 6974 6820  quirements with 
+00001c10: 7468 6520 2a2a 6079 642d 7375 626d 6974  the **`yd-submit
+00001c20: 602a 2a20 636f 6d6d 616e 640a 2d20 2a2a  `** command.- **
+00001c30: 5570 6c6f 6164 696e 672a 2a20 6669 6c65  Uploading** file
+00001c40: 7320 746f 2074 6865 2059 656c 6c6f 7744  s to the YellowD
+00001c50: 6f67 204f 626a 6563 7420 5374 6f72 6520  og Object Store 
+00001c60: 7769 7468 2074 6865 202a 2a60 7964 2d75  with the **`yd-u
+00001c70: 706c 6f61 6460 2a2a 2063 6f6d 6d61 6e64  pload`** command
+00001c80: 0a2d 202a 2a49 6e73 7461 6e74 6961 7469  .- **Instantiati
+00001c90: 6e67 2a2a 2043 6f6d 7075 7465 2052 6571  ng** Compute Req
+00001ca0: 7569 7265 6d65 6e74 7320 7769 7468 2074  uirements with t
+00001cb0: 6865 202a 2a60 7964 2d69 6e73 7461 6e74  he **`yd-instant
+00001cc0: 6961 7465 602a 2a20 636f 6d6d 616e 640a  iate`** command.
+00001cd0: 2d20 2a2a 446f 776e 6c6f 6164 696e 672a  - **Downloading*
+00001ce0: 2a20 5265 7375 6c74 7320 6672 6f6d 2074  * Results from t
+00001cf0: 6865 2059 656c 6c6f 7744 6f67 204f 626a  he YellowDog Obj
+00001d00: 6563 7420 5374 6f72 6520 7769 7468 2074  ect Store with t
+00001d10: 6865 202a 2a60 7964 2d64 6f77 6e6c 6f61  he **`yd-downloa
+00001d20: 6460 2a2a 2063 6f6d 6d61 6e64 0a2d 202a  d`** command.- *
+00001d30: 2a41 626f 7274 696e 672a 2a20 7275 6e6e  *Aborting** runn
+00001d40: 696e 6720 5461 736b 7320 7769 7468 2074  ing Tasks with t
+00001d50: 6865 202a 2a60 7964 2d61 626f 7274 602a  he **`yd-abort`*
+00001d60: 2a20 636f 6d6d 616e 640a 2d20 2a2a 4361  * command.- **Ca
+00001d70: 6e63 656c 6c69 6e67 2a2a 2057 6f72 6b20  ncelling** Work 
+00001d80: 5265 7175 6972 656d 656e 7473 2077 6974  Requirements wit
+00001d90: 6820 7468 6520 2a2a 6079 642d 6361 6e63  h the **`yd-canc
+00001da0: 656c 602a 2a20 636f 6d6d 616e 640a 2d20  el`** command.- 
+00001db0: 2a2a 5368 7574 7469 6e67 2044 6f77 6e2a  **Shutting Down*
+00001dc0: 2a20 576f 726b 6572 2050 6f6f 6c73 2077  * Worker Pools w
+00001dd0: 6974 6820 7468 6520 2a2a 6079 642d 7368  ith the **`yd-sh
+00001de0: 7574 646f 776e 602a 2a20 636f 6d6d 616e  utdown`** comman
+00001df0: 640a 2d20 2a2a 5465 726d 696e 6174 696e  d.- **Terminatin
+00001e00: 672a 2a20 436f 6d70 7574 6520 5265 7175  g** Compute Requ
+00001e10: 6972 656d 656e 7473 2077 6974 6820 7468  irements with th
+00001e20: 6520 2a2a 6079 642d 7465 726d 696e 6174  e **`yd-terminat
+00001e30: 6560 2a2a 2063 6f6d 6d61 6e64 0a2d 202a  e`** command.- *
+00001e40: 2a44 656c 6574 696e 672a 2a20 6f62 6a65  *Deleting** obje
+00001e50: 6374 7320 696e 2074 6865 2059 656c 6c6f  cts in the Yello
+00001e60: 7744 6f67 204f 626a 6563 7420 5374 6f72  wDog Object Stor
+00001e70: 6520 7769 7468 2074 6865 202a 2a60 7964  e with the **`yd
+00001e80: 2d64 656c 6574 6560 2a2a 2063 6f6d 6d61  -delete`** comma
+00001e90: 6e64 0a0a 5468 6520 6f70 6572 6174 696f  nd..The operatio
+00001ea0: 6e20 6f66 2074 6865 2063 6f6d 6d61 6e64  n of the command
+00001eb0: 7320 6973 2063 6f6e 7472 6f6c 6c65 6420  s is controlled 
+00001ec0: 7573 696e 6720 544f 4d4c 2063 6f6e 6669  using TOML confi
+00001ed0: 6775 7261 7469 6f6e 2066 696c 6573 2e20  guration files. 
+00001ee0: 496e 2061 6464 6974 696f 6e2c 2057 6f72  In addition, Wor
+00001ef0: 6b20 5265 7175 6972 656d 656e 7473 2061  k Requirements a
+00001f00: 6e64 2057 6f72 6b65 7220 506f 6f6c 7320  nd Worker Pools 
+00001f10: 6361 6e20 6265 2064 6566 696e 6564 2075  can be defined u
+00001f20: 7369 6e67 204a 534f 4e20 6669 6c65 7320  sing JSON files 
+00001f30: 7072 6f76 6964 696e 6720 6578 7465 6e73  providing extens
+00001f40: 6976 6520 636f 6e66 6967 7572 6162 696c  ive configurabil
+00001f50: 6974 792e 0a0a 2320 5965 6c6c 6f77 446f  ity...# YellowDo
+00001f60: 6720 5072 6572 6571 7569 7369 7465 730a  g Prerequisites.
+00001f70: 0a54 6f20 7375 626d 6974 202a 2a57 6f72  .To submit **Wor
+00001f80: 6b20 5265 7175 6972 656d 656e 7473 2a2a  k Requirements**
+00001f90: 2074 6f20 5965 6c6c 6f77 446f 6720 666f   to YellowDog fo
+00001fa0: 7220 7072 6f63 6573 7369 6e67 2062 7920  r processing by 
+00001fb0: 436f 6e66 6967 7572 6564 2057 6f72 6b65  Configured Worke
+00001fc0: 7220 506f 6f6c 7320 286f 6e2d 7072 656d  r Pools (on-prem
+00001fd0: 6973 6529 2061 6e64 2f6f 7220 5072 6f76  ise) and/or Prov
+00001fe0: 6973 696f 6e65 6420 576f 726b 6572 2050  isioned Worker P
+00001ff0: 6f6f 6c73 2028 636c 6f75 642d 7072 6f76  ools (cloud-prov
+00002000: 6973 696f 6e65 6420 7265 736f 7572 6365  isioned resource
+00002010: 7329 2c20 796f 7527 6c6c 206e 6565 643a  s), you'll need:
+00002020: 0a0a 312e 2041 2059 656c 6c6f 7744 6f67  ..1. A YellowDog
+00002030: 2050 6c61 7466 6f72 6d20 4163 636f 756e   Platform Accoun
+00002040: 742e 0a0a 0a32 2e20 416e 2041 7070 6c69  t....2. An Appli
+00002050: 6361 7469 6f6e 204b 6579 2026 2053 6563  cation Key & Sec
+00002060: 7265 743a 2069 6e20 7468 6520 2a2a 4163  ret: in the **Ac
+00002070: 636f 756e 7473 2a2a 2073 6563 7469 6f6e  counts** section
+00002080: 2075 6e64 6572 2074 6865 202a 2a41 7070   under the **App
+00002090: 6c69 6361 7469 6f6e 732a 2a20 7461 6220  lications** tab 
+000020a0: 696e 2074 6865 205b 5965 6c6c 6f77 446f  in the [YellowDo
+000020b0: 6720 506f 7274 616c 5d28 6874 7470 733a  g Portal](https:
+000020c0: 2f2f 706f 7274 616c 2e79 656c 6c6f 7764  //portal.yellowd
+000020d0: 6f67 2e63 6f2f 232f 6163 636f 756e 742f  og.co/#/account/
+000020e0: 6170 706c 6963 6174 696f 6e73 292c 2075  applications), u
+000020f0: 7365 2074 6865 202a 2a41 6464 2041 7070  se the **Add App
+00002100: 6c69 6361 7469 6f6e 2a2a 2062 7574 746f  lication** butto
+00002110: 6e20 746f 2063 7265 6174 6520 6120 6e65  n to create a ne
+00002120: 7720 4170 706c 6963 6174 696f 6e2c 2061  w Application, a
+00002130: 6e64 206d 616b 6520 6120 6e6f 7465 206f  nd make a note o
+00002140: 6620 6974 7320 2a2a 4b65 792a 2a20 616e  f its **Key** an
+00002150: 6420 2a2a 5365 6372 6574 2a2a 2028 7468  d **Secret** (th
+00002160: 6573 6520 7769 6c6c 206f 6e6c 7920 6265  ese will only be
+00002170: 2064 6973 706c 6179 6564 206f 6e63 6529   displayed once)
+00002180: 2e0a 0a0a 546f 2063 7265 6174 6520 2a2a  ....To create **
+00002190: 5072 6f76 6973 696f 6e65 6420 576f 726b  Provisioned Work
+000021a0: 6572 2050 6f6f 6c73 2a2a 2c20 796f 7527  er Pools**, you'
+000021b0: 6c6c 206e 6565 643a 0a0a 332e 2041 202a  ll need:..3. A *
+000021c0: 2a4b 6579 7269 6e67 2a2a 2063 7265 6174  *Keyring** creat
+000021d0: 6564 2076 6961 2074 6865 2059 656c 6c6f  ed via the Yello
+000021e0: 7744 6f67 2050 6f72 7461 6c2c 2077 6974  wDog Portal, wit
+000021f0: 6820 6163 6365 7373 2074 6f20 436c 6f75  h access to Clou
+00002200: 6420 5072 6f76 6964 6572 2063 7265 6465  d Provider crede
+00002210: 6e74 6961 6c73 2061 7320 7265 7175 6972  ntials as requir
+00002220: 6564 2e20 5468 6520 4170 706c 6963 6174  ed. The Applicat
+00002230: 696f 6e20 6d75 7374 2062 6520 6772 616e  ion must be gran
+00002240: 7465 6420 6163 6365 7373 2074 6f20 7468  ted access to th
+00002250: 6520 4b65 7972 696e 672e 0a0a 0a34 2e20  e Keyring....4. 
+00002260: 4f6e 6520 6f72 206d 6f72 6520 2a2a 436f  One or more **Co
+00002270: 6d70 7574 6520 536f 7572 6365 732a 2a20  mpute Sources** 
+00002280: 6465 6669 6e65 642c 2061 6e64 2061 202a  defined, and a *
+00002290: 2a43 6f6d 7075 7465 2052 6571 7569 7265  *Compute Require
+000022a0: 6d65 6e74 2054 656d 706c 6174 652a 2a20  ment Template** 
+000022b0: 6372 6561 7465 642e 2054 6865 2069 6d61  created. The ima
+000022c0: 6765 7320 7573 6564 2062 7920 696e 7374  ges used by inst
+000022d0: 616e 6365 7320 6d75 7374 2069 6e63 6c75  ances must inclu
+000022e0: 6465 2074 6865 2059 656c 6c6f 7744 6f67  de the YellowDog
+000022f0: 2061 6765 6e74 2c20 636f 6e66 6967 7572   agent, configur
+00002300: 6564 2077 6974 6820 7468 6520 5461 736b  ed with the Task
+00002310: 2054 7970 6528 7329 2074 6f20 6d61 7463   Type(s) to matc
+00002320: 6820 7468 6520 576f 726b 2052 6571 7569  h the Work Requi
+00002330: 7265 6d65 6e74 7320 746f 2062 6520 7375  rements to be su
+00002340: 626d 6974 7465 642e 0a0a 546f 2073 6574  bmitted...To set
+00002350: 2075 7020 2a2a 436f 6e66 6967 7572 6564   up **Configured
+00002360: 2057 6f72 6b65 7220 506f 6f6c 732a 2a2c   Worker Pools**,
+00002370: 2079 6f75 276c 6c20 6e65 6564 3a0a 0a35   you'll need:..5
+00002380: 2e20 4120 436f 6e66 6967 7572 6564 2057  . A Configured W
+00002390: 6f72 6b65 7220 506f 6f6c 2054 6f6b 656e  orker Pool Token
+000023a0: 3a20 6672 6f6d 2074 6865 202a 2a57 6f72  : from the **Wor
+000023b0: 6b65 7273 2a2a 2074 6162 2069 6e20 7468  kers** tab in th
+000023c0: 6520 5b59 656c 6c6f 7744 6f67 2050 6f72  e [YellowDog Por
+000023d0: 7461 6c5d 2868 7474 7073 3a2f 2f70 6f72  tal](https://por
+000023e0: 7461 6c2e 7965 6c6c 6f77 646f 672e 636f  tal.yellowdog.co
+000023f0: 2f23 2f77 6f72 6b65 7273 292c 2075 7365  /#/workers), use
+00002400: 2074 6865 202a 2a2b 4164 6420 436f 6e66   the **+Add Conf
+00002410: 6967 7572 6564 2057 6f72 6b65 7220 506f  igured Worker Po
+00002420: 6f6c 2a2a 2062 7574 746f 6e20 746f 2063  ol** button to c
+00002430: 7265 6174 6520 6120 6e65 7720 576f 726b  reate a new Work
+00002440: 6572 2050 6f6f 6c20 616e 6420 6765 6e65  er Pool and gene
+00002450: 7261 7465 2061 2074 6f6b 656e 2e0a 0a0a  rate a token....
+00002460: 362e 204f 6274 6169 6e20 7468 6520 5965  6. Obtain the Ye
+00002470: 6c6c 6f77 446f 6720 4167 656e 7420 616e  llowDog Agent an
+00002480: 6420 696e 7374 616c 6c2f 636f 6e66 6967  d install/config
+00002490: 7572 6520 6974 206f 6e20 796f 7572 206f  ure it on your o
+000024a0: 6e2d 7072 656d 6973 6520 7379 7374 656d  n-premise system
+000024b0: 7320 7573 696e 6720 7468 6520 546f 6b65  s using the Toke
+000024c0: 6e20 6162 6f76 652e 0a0a 2320 5363 7269  n above...# Scri
+000024d0: 7074 2049 6e73 7461 6c6c 6174 696f 6e20  pt Installation 
+000024e0: 7769 7468 2050 6970 0a0a 5079 7468 6f6e  with Pip..Python
+000024f0: 2076 6572 7369 6f6e 2033 2e37 206f 7220   version 3.7 or 
+00002500: 6c61 7465 7220 6973 2072 6571 7569 7265  later is require
+00002510: 642e 2049 7427 7320 7265 636f 6d6d 656e  d. It's recommen
+00002520: 6465 6420 7468 6174 2069 6e73 7461 6c6c  ded that install
+00002530: 6174 696f 6e20 6973 2070 6572 666f 726d  ation is perform
+00002540: 6564 2069 6e20 6120 5079 7468 6f6e 2076  ed in a Python v
+00002550: 6972 7475 616c 2065 6e76 6972 6f6e 6d65  irtual environme
+00002560: 6e74 2028 6f72 2073 696d 696c 6172 2920  nt (or similar) 
+00002570: 746f 2069 736f 6c61 7465 2074 6865 2069  to isolate the i
+00002580: 6e73 7461 6c6c 6174 696f 6e20 6672 6f6d  nstallation from
+00002590: 206f 7468 6572 2050 7974 686f 6e20 656e   other Python en
+000025a0: 7669 726f 6e6d 656e 7473 206f 6e20 796f  vironments on yo
+000025b0: 7572 2073 7973 7465 6d2e 0a0a 496e 7374  ur system...Inst
+000025c0: 616c 6c61 7469 6f6e 2061 6e64 2073 7562  allation and sub
+000025d0: 7365 7175 656e 7420 7570 6461 7465 2061  sequent update a
+000025e0: 7265 2076 6961 2060 7069 7060 2061 6e64  re via `pip` and
+000025f0: 2050 7950 4920 7573 696e 673a 200a 0a60   PyPI using: ..`
+00002600: 6060 7368 656c 6c0a 7069 7020 696e 7374  ``shell.pip inst
+00002610: 616c 6c20 2d55 2079 656c 6c6f 7764 6f67  all -U yellowdog
+00002620: 2d70 7974 686f 6e2d 6578 616d 706c 6573  -python-examples
+00002630: 0a60 6060 0a0a 4966 2079 6f75 2772 6520  .```..If you're 
+00002640: 696e 7465 7265 7374 6564 2069 6e20 696e  interested in in
+00002650: 636c 7564 696e 6720 2a2a 4a73 6f6e 6e65  cluding **Jsonne
+00002660: 742a 2a20 7375 7070 6f72 742c 2070 6c65  t** support, ple
+00002670: 6173 6520 7365 6520 7468 6520 5b4a 736f  ase see the [Jso
+00002680: 6e6e 6574 2053 7570 706f 7274 5d28 236a  nnet Support](#j
+00002690: 736f 6e6e 6574 2d73 7570 706f 7274 2920  sonnet-support) 
+000026a0: 7365 6374 696f 6e20 6265 6c6f 772e 0a0a  section below...
+000026b0: 2320 5363 7269 7074 2049 6e73 7461 6c6c  # Script Install
+000026c0: 6174 696f 6e20 7769 7468 2050 6970 780a  ation with Pipx.
+000026d0: 0a54 6865 2063 6f6d 6d61 6e64 7320 6361  .The commands ca
+000026e0: 6e20 616c 736f 2062 6520 696e 7374 616c  n also be instal
+000026f0: 6c65 6420 7573 696e 6720 2a2a 5b70 6970  led using **[pip
+00002700: 785d 2868 7474 7073 3a2f 2f70 7970 612e  x](https://pypa.
+00002710: 6769 7468 7562 2e69 6f2f 7069 7078 2f29  github.io/pipx/)
+00002720: 2a2a 2e0a 0a54 6869 7320 6d65 7468 6f64  **...This method
+00002730: 2072 6571 7569 7265 7320 5079 7468 6f6e   requires Python
+00002740: 2033 2e37 2b20 616e 6420 7069 7078 2074   3.7+ and pipx t
+00002750: 6f20 6265 2069 6e73 7461 6c6c 6564 2e20  o be installed. 
+00002760: 546f 2069 6e73 7461 6c6c 3a0a 6060 6073  To install:.```s
+00002770: 6865 6c6c 0a70 6970 7820 696e 7374 616c  hell.pipx instal
+00002780: 6c20 7965 6c6c 6f77 646f 672d 7079 7468  l yellowdog-pyth
+00002790: 6f6e 2d65 7861 6d70 6c65 730a 6060 600a  on-examples.```.
+000027a0: 0a54 6f20 7570 6461 7465 3a0a 6060 6073  .To update:.```s
+000027b0: 6865 6c6c 0a70 6970 7820 7570 6772 6164  hell.pipx upgrad
+000027c0: 6520 7965 6c6c 6f77 646f 672d 7079 7468  e yellowdog-pyth
+000027d0: 6f6e 2d65 7861 6d70 6c65 730a 6060 600a  on-examples.```.
+000027e0: 0a23 2055 7361 6765 0a0a 426f 7468 206f  .# Usage..Both o
+000027f0: 6620 7468 6520 696e 7374 616c 6c61 7469  f the installati
+00002800: 6f6e 206d 6574 686f 6473 2061 626f 7665  on methods above
+00002810: 2077 696c 6c20 696e 7374 616c 6c20 6120   will install a 
+00002820: 6e75 6d62 6572 206f 6620 2a2a 6079 642d  number of **`yd-
+00002830: 602a 2a20 636f 6d6d 616e 6473 206f 6e20  `** commands on 
+00002840: 796f 7572 2050 4154 482e 0a0a 436f 6d6d  your PATH...Comm
+00002850: 616e 6473 2061 7265 2072 756e 2066 726f  ands are run fro
+00002860: 6d20 7468 6520 636f 6d6d 616e 6420 6c69  m the command li
+00002870: 6e65 2e20 496e 766f 6b69 6e67 2074 6865  ne. Invoking the
+00002880: 2063 6f6d 6d61 6e64 2077 6974 6820 7468   command with th
+00002890: 6520 602d 2d68 656c 7060 206f 7220 602d  e `--help` or `-
+000028a0: 6860 206f 7074 696f 6e20 7769 6c6c 2064  h` option will d
+000028b0: 6973 706c 6179 2074 6865 2063 6f6d 6d61  isplay the comma
+000028c0: 6e64 206c 696e 6520 6f70 7469 6f6e 7320  nd line options 
+000028d0: 6170 706c 6963 6162 6c65 2074 6f20 6120  applicable to a 
+000028e0: 6769 7665 6e20 636f 6d6d 616e 642c 2065  given command, e
+000028f0: 2e67 2e3a 0a0a 6060 6074 6578 740a 2025  .g.:..```text. %
+00002900: 2079 642d 6361 6e63 656c 202d 2d68 656c   yd-cancel --hel
+00002910: 700a 7573 6167 653a 2079 642d 6361 6e63  p.usage: yd-canc
+00002920: 656c 205b 2d68 5d20 5b2d 2d64 6f63 735d  el [-h] [--docs]
+00002930: 205b 2d2d 636f 6e66 6967 203c 636f 6e66   [--config <conf
+00002940: 6967 5f66 696c 652e 746f 6d6c 3e5d 205b  ig_file.toml>] [
+00002950: 2d2d 6b65 7920 3c61 7070 2d6b 6579 3e5d  --key <app-key>]
+00002960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002970: 2020 5b2d 2d73 6563 7265 7420 3c61 7070    [--secret <app
+00002980: 2d73 6563 7265 743e 5d20 5b2d 2d6e 616d  -secret>] [--nam
+00002990: 6573 7061 6365 203c 6e61 6d65 7370 6163  espace <namespac
+000029a0: 653e 5d20 5b2d 2d74 6167 203c 7461 673e  e>] [--tag <tag>
+000029b0: 5d20 5b2d 2d75 726c 203c 7572 6c3e 5d0a  ] [--url <url>].
+000029c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029d0: 205b 2d2d 7661 7269 6162 6c65 203c 7661   [--variable <va
+000029e0: 7231 3d76 313e 5d20 5b2d 2d71 7569 6574  r1=v1>] [--quiet
+000029f0: 5d20 5b2d 2d64 6562 7567 5d20 5b2d 2d70  ] [--debug] [--p
+00002a00: 6163 5d20 5b2d 2d61 626f 7274 5d20 5b2d  ac] [--abort] [-
+00002a10: 2d66 6f6c 6c6f 775d 0a20 2020 2020 2020  -follow].       
+00002a20: 2020 2020 2020 2020 2020 5b2d 2d69 6e74            [--int
+00002a30: 6572 6163 7469 7665 5d20 5b2d 2d79 6573  eractive] [--yes
+00002a40: 5d0a 0a59 656c 6c6f 7744 6f67 2065 7861  ]..YellowDog exa
+00002a50: 6d70 6c65 2075 7469 6c69 7479 2066 6f72  mple utility for
+00002a60: 2063 616e 6365 6c6c 696e 6720 576f 726b   cancelling Work
+00002a70: 2052 6571 7569 7265 6d65 6e74 730a 0a6f   Requirements..o
+00002a80: 7074 696f 6e61 6c20 6172 6775 6d65 6e74  ptional argument
+00002a90: 733a 0a20 202d 682c 202d 2d68 656c 7020  s:.  -h, --help 
+00002aa0: 2020 2020 2020 2020 2020 2073 686f 7720             show 
+00002ab0: 7468 6973 2068 656c 7020 6d65 7373 6167  this help messag
+00002ac0: 6520 616e 6420 6578 6974 0a20 202d 2d64  e and exit.  --d
+00002ad0: 6f63 7320 2020 2020 2020 2020 2020 2020  ocs             
+00002ae0: 2020 2070 726f 7669 6465 2061 206c 696e     provide a lin
+00002af0: 6b20 746f 2074 6865 2064 6f63 756d 656e  k to the documen
+00002b00: 7461 7469 6f6e 2066 6f72 2074 6869 7320  tation for this 
+00002b10: 7665 7273 696f 6e0a 2020 2d2d 636f 6e66  version.  --conf
+00002b20: 6967 203c 636f 6e66 6967 5f66 696c 652e  ig <config_file.
+00002b30: 746f 6d6c 3e2c 202d 6320 3c63 6f6e 6669  toml>, -c <confi
+00002b40: 675f 6669 6c65 2e74 6f6d 6c3e 0a20 2020  g_file.toml>.   
+00002b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b60: 2020 2020 2063 6f6e 6669 6775 7261 7469       configurati
+00002b70: 6f6e 2066 696c 6520 696e 2054 4f4d 4c20  on file in TOML 
+00002b80: 666f 726d 6174 3b20 6465 6661 756c 7420  format; default 
+00002b90: 6973 2027 636f 6e66 6967 2e74 6f6d 6c27  is 'config.toml'
+00002ba0: 2069 6e20 7468 6520 6375 7272 656e 740a   in the current.
+00002bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002bc0: 2020 2020 2020 2020 6469 7265 6374 6f72          director
+00002bd0: 790a 2020 2d2d 6b65 7920 3c61 7070 2d6b  y.  --key <app-k
+00002be0: 6579 3e2c 202d 6b20 3c61 7070 2d6b 6579  ey>, -k <app-key
+00002bf0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00002c00: 2020 2020 2020 2020 2020 7468 6520 5965            the Ye
+00002c10: 6c6c 6f77 446f 6720 4170 706c 6963 6174  llowDog Applicat
+00002c20: 696f 6e20 6b65 790a 2020 2d2d 7365 6372  ion key.  --secr
+00002c30: 6574 203c 6170 702d 7365 6372 6574 3e2c  et <app-secret>,
+00002c40: 202d 7320 3c61 7070 2d73 6563 7265 743e   -s <app-secret>
+00002c50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002c60: 2020 2020 2020 2020 2074 6865 2059 656c           the Yel
+00002c70: 6c6f 7744 6f67 2041 7070 6c69 6361 7469  lowDog Applicati
+00002c80: 6f6e 2073 6563 7265 740a 2020 2d2d 6e61  on secret.  --na
+00002c90: 6d65 7370 6163 6520 3c6e 616d 6573 7061  mespace <namespa
+00002ca0: 6365 3e2c 202d 6e20 3c6e 616d 6573 7061  ce>, -n <namespa
+00002cb0: 6365 3e0a 2020 2020 2020 2020 2020 2020  ce>.            
+00002cc0: 2020 2020 2020 2020 2020 2020 7468 6520              the 
+00002cd0: 6e61 6d65 7370 6163 6520 746f 2075 7365  namespace to use
+00002ce0: 2077 6865 6e20 6372 6561 7469 6e67 2061   when creating a
+00002cf0: 6e64 2069 6465 6e74 6966 7969 6e67 2065  nd identifying e
+00002d00: 6e74 6974 6965 730a 2020 2d2d 7461 6720  ntities.  --tag 
+00002d10: 3c74 6167 3e2c 202d 7420 3c74 6167 3e0a  <tag>, -t <tag>.
+00002d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d30: 2020 2020 2020 2020 7468 6520 7461 6720          the tag 
+00002d40: 746f 2075 7365 2066 6f72 2074 6167 6769  to use for taggi
+00002d50: 6e67 2061 6e64 206e 616d 696e 6720 656e  ng and naming en
+00002d60: 7469 7469 6573 0a20 202d 2d75 726c 203c  tities.  --url <
+00002d70: 7572 6c3e 2c20 2d75 203c 7572 6c3e 0a20  url>, -u <url>. 
+00002d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d90: 2020 2020 2020 2074 6865 2055 524c 206f         the URL o
+00002da0: 6620 7468 6520 5965 6c6c 6f77 446f 6720  f the YellowDog 
+00002db0: 506c 6174 666f 726d 2041 5049 0a20 202d  Platform API.  -
+00002dc0: 2d76 6172 6961 626c 6520 3c76 6172 313d  -variable <var1=
+00002dd0: 7631 3e2c 202d 7620 3c76 6172 313d 7631  v1>, -v <var1=v1
+00002de0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00002df0: 2020 2020 2020 2020 2020 7573 6572 2d64            user-d
+00002e00: 6566 696e 6564 2076 6172 6961 626c 6520  efined variable 
+00002e10: 7375 6273 7469 7475 7469 6f6e 733b 2063  substitutions; c
+00002e20: 616e 2062 6520 7375 7070 6c69 6564 206d  an be supplied m
+00002e30: 756c 7469 706c 6520 7469 6d65 730a 2020  ultiple times.  
+00002e40: 2d2d 7175 6965 742c 202d 7120 2020 2020  --quiet, -q     
+00002e50: 2020 2020 2020 7375 7070 7265 7373 2028        suppress (
+00002e60: 6e6f 6e2d 6572 726f 722c 206e 6f6e 2d69  non-error, non-i
+00002e70: 6e74 6572 6163 7469 7665 2920 7374 6174  nteractive) stat
+00002e80: 7573 2061 6e64 2070 726f 6772 6573 7320  us and progress 
+00002e90: 6d65 7373 6167 6573 0a20 202d 2d64 6562  messages.  --deb
+00002ea0: 7567 2020 2020 2020 2020 2020 2020 2020  ug              
+00002eb0: 2070 7269 6e74 2061 2073 7461 636b 2074   print a stack t
+00002ec0: 7261 6365 2028 6574 632e 2920 6f6e 2065  race (etc.) on e
+00002ed0: 7272 6f72 0a20 202d 2d70 6163 2020 2020  rror.  --pac    
+00002ee0: 2020 2020 2020 2020 2020 2020 2065 6e61               ena
+00002ef0: 626c 6520 5041 4320 2870 726f 7879 2061  ble PAC (proxy a
+00002f00: 7574 6f2d 636f 6e66 6967 7572 6174 696f  uto-configuratio
+00002f10: 6e29 2073 7570 706f 7274 0a20 202d 2d61  n) support.  --a
+00002f20: 626f 7274 2c20 2d61 2020 2020 2020 2020  bort, -a        
+00002f30: 2020 2061 626f 7274 2061 6c6c 2072 756e     abort all run
+00002f40: 6e69 6e67 2074 6173 6b73 2077 6974 6820  ning tasks with 
+00002f50: 696d 6d65 6469 6174 6520 6566 6665 6374  immediate effect
+00002f60: 0a20 202d 2d66 6f6c 6c6f 772c 202d 6620  .  --follow, -f 
+00002f70: 2020 2020 2020 2020 2077 6865 6e20 7573           when us
+00002f80: 696e 6720 2d2d 6162 6f72 742c 2070 6f6c  ing --abort, pol
+00002f90: 6c20 756e 7469 6c20 616c 6c20 5461 736b  l until all Task
+00002fa0: 7320 6861 7665 2062 6565 6e20 6162 6f72  s have been abor
+00002fb0: 7465 640a 2020 2d2d 696e 7465 7261 6374  ted.  --interact
+00002fc0: 6976 652c 202d 6920 2020 2020 6c69 7374  ive, -i     list
+00002fd0: 2c20 616e 6420 696e 7465 7261 6374 6976  , and interactiv
+00002fe0: 656c 7920 7365 6c65 6374 2c20 6974 656d  ely select, item
+00002ff0: 7320 746f 2061 6374 206f 6e0a 2020 2d2d  s to act on.  --
+00003000: 7965 732c 202d 7920 2020 2020 2020 2020  yes, -y         
+00003010: 2020 2020 7065 7266 6f72 6d20 6465 7374      perform dest
+00003020: 7275 6374 6976 6520 6163 7469 6f6e 7320  ructive actions 
+00003030: 7769 7468 6f75 7420 7265 7175 6972 696e  without requirin
+00003040: 6720 7573 6572 2063 6f6e 6669 726d 6174  g user confirmat
+00003050: 696f 6e0a 6060 600a 0a23 2043 6f6e 6669  ion.```..# Confi
+00003060: 6775 7261 7469 6f6e 0a0a 4279 2064 6566  guration..By def
+00003070: 6175 6c74 2c20 7468 6520 6f70 6572 6174  ault, the operat
+00003080: 696f 6e20 6f66 2061 6c6c 2063 6f6d 6d61  ion of all comma
+00003090: 6e64 7320 6973 2063 6f6e 6669 6775 7265  nds is configure
+000030a0: 6420 7573 696e 6720 6120 544f 4d4c 2063  d using a TOML c
+000030b0: 6f6e 6669 6775 7261 7469 6f6e 2066 696c  onfiguration fil
+000030c0: 652e 0a0a 5468 6520 636f 6e66 6967 7572  e...The configur
+000030d0: 6174 696f 6e20 6669 6c65 2068 6173 2074  ation file has t
+000030e0: 6872 6565 2070 6f73 7369 626c 6520 7365  hree possible se
+000030f0: 6374 696f 6e73 3a0a 0a31 2e20 4120 6063  ctions:..1. A `c
+00003100: 6f6d 6d6f 6e60 2073 6563 7469 6f6e 2074  ommon` section t
+00003110: 6861 7420 636f 6e74 6169 6e73 2072 6571  hat contains req
+00003120: 7569 7265 6420 7365 6375 7269 7479 2070  uired security p
+00003130: 726f 7065 7274 6965 7320 666f 7220 696e  roperties for in
+00003140: 7465 7261 6374 696e 6720 7769 7468 2074  teracting with t
+00003150: 6865 2059 656c 6c6f 7744 6f67 2070 6c61  he YellowDog pla
+00003160: 7466 6f72 6d2c 2073 6574 7320 7468 6520  tform, sets the 
+00003170: 4e61 6d65 7370 6163 6520 696e 2077 6869  Namespace in whi
+00003180: 6368 2059 656c 6c6f 7744 6f67 2061 7373  ch YellowDog ass
+00003190: 6574 7320 616e 6420 6f62 6a65 6374 7320  ets and objects 
+000031a0: 6172 6520 6372 6561 7465 642c 2061 6e64  are created, and
+000031b0: 2061 2054 6167 2074 6861 7420 6973 2075   a Tag that is u
+000031c0: 7365 6420 666f 7220 7461 6767 696e 6720  sed for tagging 
+000031d0: 616e 6420 6e61 6d69 6e67 2061 7373 6574  and naming asset
+000031e0: 7320 616e 6420 6f62 6a65 6374 732e 0a32  s and objects..2
+000031f0: 2e20 4120 6077 6f72 6b52 6571 7569 7265  . A `workRequire
+00003200: 6d65 6e74 6020 7365 6374 696f 6e20 7468  ment` section th
+00003210: 6174 2064 6566 696e 6573 2074 6865 2070  at defines the p
+00003220: 726f 7065 7274 6965 7320 6f66 2057 6f72  roperties of Wor
+00003230: 6b20 5265 7175 6972 656d 656e 7473 2074  k Requirements t
+00003240: 6f20 6265 2073 7562 6d69 7474 6564 2074  o be submitted t
+00003250: 6f20 7468 6520 5965 6c6c 6f77 446f 6720  o the YellowDog 
+00003260: 706c 6174 666f 726d 2e0a 332e 2041 2060  platform..3. A `
+00003270: 776f 726b 6572 506f 6f6c 6020 7365 6374  workerPool` sect
+00003280: 696f 6e20 7468 6174 2064 6566 696e 6573  ion that defines
+00003290: 2074 6865 2070 726f 7065 7274 6965 7320   the properties 
+000032a0: 6f66 2050 726f 7669 736f 6e65 6420 576f  of Provisoned Wo
+000032b0: 726b 6572 2050 6f6f 6c73 2074 6f20 6265  rker Pools to be
+000032c0: 2063 7265 6174 6564 2075 7369 6e67 2074   created using t
+000032d0: 6865 2059 656c 6c6f 7744 6f67 2070 6c61  he YellowDog pla
+000032e0: 7466 6f72 6d2e 200a 0a54 6865 7265 2069  tform. ..There i
+000032f0: 7320 6120 646f 6375 6d65 6e74 6564 2074  s a documented t
+00003300: 656d 706c 6174 6520 544f 4d4c 2066 696c  emplate TOML fil
+00003310: 6520 7072 6f76 6964 6564 2069 6e20 5b63  e provided in [c
+00003320: 6f6e 6669 672e 746f 6d6c 2e74 656d 706c  onfig.toml.templ
+00003330: 6174 655d 2863 6f6e 6669 672e 746f 6d6c  ate](config.toml
+00003340: 2e74 656d 706c 6174 6529 2c20 636f 6e74  .template), cont
+00003350: 6169 6e69 6e67 2074 6865 206d 6169 6e20  aining the main 
+00003360: 7072 6f70 6572 7469 6573 2074 6861 7420  properties that 
+00003370: 6361 6e20 6265 2063 6f6e 6669 6775 7265  can be configure
+00003380: 642e 0a0a 5468 6520 636f 6e66 6967 7572  d...The configur
+00003390: 6174 696f 6e20 6669 6c65 6e61 6d65 2063  ation filename c
+000033a0: 616e 2062 6520 7375 7070 6c69 6564 2069  an be supplied i
+000033b0: 6e20 7468 7265 6520 6469 6666 6572 656e  n three differen
+000033c0: 7420 7761 7973 3a0a 0a31 2e20 4f6e 2074  t ways:..1. On t
+000033d0: 6865 2063 6f6d 6d61 6e64 206c 696e 652c  he command line,
+000033e0: 2075 7369 6e67 2074 6865 2060 2d2d 636f   using the `--co
+000033f0: 6e66 6967 6020 6f72 2060 2d63 6020 6f70  nfig` or `-c` op
+00003400: 7469 6f6e 732c 2065 2e67 2e3a 3c62 723e  tions, e.g.:<br>
+00003410: 6079 642d 7375 626d 6974 202d 6320 6a6f  `yd-submit -c jo
+00003420: 6273 2f63 6f6e 6669 675f 312e 746f 6d6c  bs/config_1.toml
+00003430: 600a 322e 2055 7369 6e67 2074 6865 2060  `.2. Using the `
+00003440: 5944 5f43 4f4e 4660 2065 6e76 6972 6f6e  YD_CONF` environ
+00003450: 6d65 6e74 2076 6172 6961 626c 652c 2065  ment variable, e
+00003460: 2e67 2e3a 203c 6272 3e60 6578 706f 7274  .g.: <br>`export
+00003470: 2059 445f 434f 4e46 3d22 6a6f 6273 2f63   YD_CONF="jobs/c
+00003480: 6f6e 6669 675f 312e 746f 6d6c 2260 0a33  onfig_1.toml"`.3
+00003490: 2e20 4966 206e 6569 7468 6572 206f 6620  . If neither of 
+000034a0: 7468 6520 6162 6f76 6520 6973 2073 7570  the above is sup
+000034b0: 706c 6965 642c 2074 6865 2063 6f6d 6d61  plied, the comma
+000034c0: 6e64 7320 6c6f 6f6b 2066 6f72 2061 2060  nds look for a `
+000034d0: 636f 6e66 6967 2e74 6f6d 6c60 2066 696c  config.toml` fil
+000034e0: 6520 696e 2074 6865 2063 7572 7265 6e74  e in the current
+000034f0: 2064 6972 6563 746f 7279 0a0a 5468 6520   directory..The 
+00003500: 6f70 7469 6f6e 7320 6162 6f76 6520 6172  options above ar
+00003510: 6520 7368 6f77 6e20 696e 206f 7264 6572  e shown in order
+00003520: 206f 6620 7072 6563 6564 656e 6365 2c20   of precedence, 
+00003530: 692e 652e 2c20 6120 6669 6c65 6e61 6d65  i.e., a filename
+00003540: 2073 7570 706c 6965 6420 6f6e 2074 6865   supplied on the
+00003550: 2063 6f6d 6d61 6e64 206c 696e 6520 7375   command line su
+00003560: 7065 7273 6564 6573 206f 6e65 2073 6574  persedes one set
+00003570: 2069 6e20 6059 445f 434f 4e46 602c 2077   in `YD_CONF`, w
+00003580: 6869 6368 2073 7570 6572 7365 6465 7320  hich supersedes 
+00003590: 7468 6520 6465 6661 756c 742e 0a0a 2320  the default...# 
+000035a0: 4e61 6d69 6e67 2052 756c 6573 0a0a 416c  Naming Rules..Al
+000035b0: 6c20 656e 7469 7479 206e 616d 6573 2075  l entity names u
+000035c0: 7365 6420 7769 7468 696e 2074 6865 2059  sed within the Y
+000035d0: 656c 6c6f 7744 6f67 2050 6c61 7466 6f72  ellowDog Platfor
+000035e0: 6d20 6d75 7374 2063 6f6d 706c 7920 7769  m must comply wi
+000035f0: 7468 2074 6865 2066 6f6c 6c6f 7769 6e67  th the following
+00003600: 2072 6573 7472 6963 7469 6f6e 733a 0a0a   restrictions:..
+00003610: 2d20 4e61 6d65 7320 6361 6e20 6f6e 6c79  - Names can only
+00003620: 2063 6f6e 7461 696e 2074 6865 2066 6f6c   contain the fol
+00003630: 6c6f 7769 6e67 3a20 6c6f 7765 7263 6173  lowing: lowercas
+00003640: 6520 6c65 7474 6572 732c 2064 6967 6974  e letters, digit
+00003650: 732c 2068 7970 6865 6e73 2061 6e64 2075  s, hyphens and u
+00003660: 6e64 6572 7363 6f72 6573 2028 6e6f 7465  nderscores (note
+00003670: 2074 6861 7420 7370 6163 6573 2061 7265   that spaces are
+00003680: 206e 6f74 2070 6572 6d69 7474 6564 290a   not permitted).
+00003690: 2d20 4e61 6d65 7320 6d75 7374 2073 7461  - Names must sta
+000036a0: 7274 2077 6974 6820 6120 6c65 7474 6572  rt with a letter
+000036b0: 0a2d 204e 616d 6573 206d 7573 7420 656e  .- Names must en
+000036c0: 6420 7769 7468 2061 206c 6574 7465 7220  d with a letter 
+000036d0: 6f72 2064 6967 6974 0a2d 204e 616d 6520  or digit.- Name 
+000036e0: 6c65 6e67 7468 206d 7573 7420 6265 203c  length must be <
+000036f0: 3d20 3630 2063 6861 7261 6374 6572 730a  = 60 characters.
+00003700: 0a54 6865 7365 2072 6573 7472 6963 7469  .These restricti
+00003710: 6f6e 7320 6170 706c 7920 746f 2065 6e74  ons apply to ent
+00003720: 6974 6965 7320 696e 636c 7564 696e 6720  ities including 
+00003730: 4e61 6d65 7370 6163 6573 2c20 5461 6773  Namespaces, Tags
+00003740: 2c20 576f 726b 2052 6571 7569 7265 6d65  , Work Requireme
+00003750: 6e74 732c 2054 6173 6b20 4772 6f75 7073  nts, Task Groups
+00003760: 2c20 5461 736b 732c 2057 6f72 6b65 7220  , Tasks, Worker 
+00003770: 506f 6f6c 732c 2061 6e64 2043 6f6d 7075  Pools, and Compu
+00003780: 7465 2052 6571 7569 7265 6d65 6e74 732c  te Requirements,
+00003790: 2061 6e64 2061 6c73 6f20 6170 706c 7920   and also apply 
+000037a0: 746f 2065 6e74 6974 6965 7320 7468 6174  to entities that
+000037b0: 2061 7265 2063 7572 7265 6e74 6c79 2075   are currently u
+000037c0: 7365 6420 696e 6469 7265 6374 6c79 2062  sed indirectly b
+000037d0: 7920 7468 6573 6520 7363 7269 7074 732c  y these scripts,
+000037e0: 2069 6e63 6c75 6469 6e67 2055 7365 726e   including Usern
+000037f0: 616d 6573 2c20 4372 6564 656e 7469 616c  ames, Credential
+00003800: 732c 204b 6579 7269 6e67 732c 2043 6f6d  s, Keyrings, Com
+00003810: 7075 7465 2053 6f75 7263 6573 2061 6e64  pute Sources and
+00003820: 2043 6f6d 7075 7465 2054 656d 706c 6174   Compute Templat
+00003830: 6573 2e0a 0a23 2043 6f6d 6d6f 6e20 5072  es...# Common Pr
+00003840: 6f70 6572 7469 6573 0a0a 5468 6520 605b  operties..The `[
+00003850: 636f 6d6d 6f6e 5d60 2073 6563 7469 6f6e  common]` section
+00003860: 206f 6620 7468 6520 636f 6e66 6967 7572   of the configur
+00003870: 6174 696f 6e20 6669 6c65 2063 616e 2063  ation file can c
+00003880: 6f6e 7461 696e 2074 6865 2066 6f6c 6c6f  ontain the follo
+00003890: 7769 6e67 2070 726f 7065 7274 6965 733a  wing properties:
+000038a0: 0a0a 7c20 5072 6f70 6572 7479 2020 2020  ..| Property    
+000038b0: 7c20 4465 7363 7269 7074 696f 6e20 2020  | Description   
+000038c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000038d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000038e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000038f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003900: 2020 2020 2020 7c0a 7c3a 2d2d 2d2d 2d2d        |.|:------
+00003910: 2d2d 2d2d 2d2d 7c3a 2d2d 2d2d 2d2d 2d2d  ------|:--------
+00003920: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003930: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003940: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003950: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003960: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a 7c20  ------------|.| 
+00003970: 606b 6579 6020 2020 2020 2020 7c20 5468  `key`       | Th
+00003980: 6520 2a2a 6b65 792a 2a20 6f66 2074 6865  e **key** of the
+00003990: 2059 656c 6c6f 7744 6f67 2041 7070 6c69   YellowDog Appli
+000039a0: 6361 7469 6f6e 2075 6e64 6572 2077 6869  cation under whi
+000039b0: 6368 2074 6865 2063 6f6d 6d61 6e64 7320  ch the commands 
+000039c0: 7769 6c6c 2072 756e 2020 2020 2020 2020  will run        
+000039d0: 2020 7c0a 7c20 6073 6563 7265 7460 2020    |.| `secret`  
+000039e0: 2020 7c20 5468 6520 2a2a 7365 6372 6574    | The **secret
+000039f0: 2a2a 206f 6620 7468 6520 5965 6c6c 6f77  ** of the Yellow
+00003a00: 446f 6720 4170 706c 6963 6174 696f 6e20  Dog Application 
+00003a10: 756e 6465 7220 7768 6963 6820 7468 6520  under which the 
+00003a20: 636f 6d6d 616e 6473 2077 696c 6c20 7275  commands will ru
+00003a30: 6e20 2020 2020 2020 7c0a 7c20 606e 616d  n       |.| `nam
+00003a40: 6573 7061 6365 6020 7c20 5468 6520 2a2a  espace` | The **
+00003a50: 6e61 6d65 7370 6163 652a 2a20 746f 2062  namespace** to b
+00003a60: 6520 7573 6564 2066 6f72 2067 726f 7570  e used for group
+00003a70: 696e 6720 7265 736f 7572 6365 7320 2020  ing resources   
+00003a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a90: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+00003aa0: 7c20 6074 6167 6020 2020 2020 2020 7c20  | `tag`       | 
+00003ab0: 5468 6520 2a2a 7461 672a 2a20 746f 2062  The **tag** to b
+00003ac0: 6520 7573 6564 2066 6f72 2074 6167 6769  e used for taggi
+00003ad0: 6e67 2072 6573 6f75 7263 6573 2061 6e64  ng resources and
+00003ae0: 206e 616d 696e 6720 6f62 6a65 6374 7320   naming objects 
+00003af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b00: 2020 2020 7c0a 7c20 6075 726c 6020 2020      |.| `url`   
+00003b10: 2020 2020 7c20 5468 6520 2a2a 5552 4c2a      | The **URL*
+00003b20: 2a20 6f66 2074 6865 2059 656c 6c6f 7744  * of the YellowD
+00003b30: 6f67 2050 6c61 7466 6f72 6d20 4150 4920  og Platform API 
+00003b40: 656e 6470 6f69 6e74 2c20 6966 2074 6865  endpoint, if the
+00003b50: 2064 6566 6175 6c74 2069 736e 2774 2074   default isn't t
+00003b60: 6f20 6265 2075 7365 6420 7c0a 7c20 6075  o be used |.| `u
+00003b70: 7365 5041 4360 2020 2020 7c20 5573 6520  sePAC`    | Use 
+00003b80: 5041 4320 2870 726f 7879 2061 7574 6f63  PAC (proxy autoc
+00003b90: 6f6e 6669 6775 7261 7469 6f6e 2920 6966  onfiguration) if
+00003ba0: 2073 6574 2074 6f20 6074 7275 6560 2020   set to `true`  
+00003bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003bd0: 7c0a 7c20 6076 6172 6961 626c 6573 6020  |.| `variables` 
+00003be0: 7c20 4120 7461 626c 6520 636f 6e74 6169  | A table contai
+00003bf0: 6e69 6e67 202a 2a76 6172 6961 626c 6520  ning **variable 
+00003c00: 7375 6273 7469 7475 7469 6f6e 732a 2a20  substitutions** 
+00003c10: 2873 6565 2074 6865 2056 6172 6961 626c  (see the Variabl
+00003c20: 6573 2073 6563 7469 6f6e 2062 656c 6f77  es section below
+00003c30: 2920 2020 2020 7c0a 0a41 6e20 6578 616d  )     |..An exam
+00003c40: 706c 6520 6063 6f6d 6d6f 6e60 2073 6563  ple `common` sec
+00003c50: 7469 6f6e 2069 7320 7368 6f77 6e20 6265  tion is shown be
+00003c60: 6c6f 773a 0a0a 6060 6074 6f6d 6c0a 5b63  low:..```toml.[c
+00003c70: 6f6d 6d6f 6e5d 0a20 2020 206b 6579 203d  ommon].    key =
+00003c80: 2022 6173 6466 6768 6a6b 6c7a 7863 7662   "asdfghjklzxcvb
+00003c90: 2d31 3233 3435 3637 220a 2020 2020 7365  -1234567".    se
+00003ca0: 6372 6574 203d 2022 7177 6572 7479 7569  cret = "qwertyui
+00003cb0: 6f70 6173 6466 6768 6a6b 6c7a 7863 7662  opasdfghjklzxcvb
+00003cc0: 6e6d 3132 3334 3536 3738 3930 7177 6572  nm1234567890qwer
+00003cd0: 7479 7522 0a20 2020 206e 616d 6573 7061  tyu".    namespa
+00003ce0: 6365 203d 2022 7072 6f6a 6563 742d 7822  ce = "project-x"
+00003cf0: 0a20 2020 2074 6167 203d 2022 7465 7374  .    tag = "test
+00003d00: 696e 672d 7b7b 7573 6572 6e61 6d65 7d7d  ing-{{username}}
+00003d10: 220a 6060 600a 0a49 6e64 656e 7461 7469  ".```..Indentati
+00003d20: 6f6e 2069 7320 6f70 7469 6f6e 616c 2069  on is optional i
+00003d30: 6e20 544f 4d4c 2066 696c 6573 2061 6e64  n TOML files and
+00003d40: 2069 7320 666f 7220 7265 6164 6162 696c   is for readabil
+00003d50: 6974 7920 6f6e 6c79 2e0a 0a23 2320 4854  ity only...## HT
+00003d60: 5450 5320 5072 6f78 7920 5375 7070 6f72  TPS Proxy Suppor
+00003d70: 740a 0a54 6865 2063 6f6d 6d61 6e64 7320  t..The commands 
+00003d80: 7769 6c6c 2075 7365 2074 6865 2076 616c  will use the val
+00003d90: 7565 206f 6620 7468 6520 656e 7669 726f  ue of the enviro
+00003da0: 6e6d 656e 7420 7661 7269 6162 6c65 2060  nment variable `
+00003db0: 4854 5450 535f 5052 4f58 5960 2069 6620  HTTPS_PROXY` if 
+00003dc0: 726f 7574 696e 6720 7468 726f 7567 6820  routing through 
+00003dd0: 6120 7072 6f78 7920 6973 2072 6571 7569  a proxy is requi
+00003de0: 7265 642e 0a0a 496e 2061 6464 6974 696f  red...In additio
+00003df0: 6e2c 2074 6865 2063 6f6d 6d61 6e64 7320  n, the commands 
+00003e00: 6361 6e20 7573 6520 5072 6f78 7920 4175  can use Proxy Au
+00003e10: 746f 2d43 6f6e 6669 6775 7261 7469 6f6e  to-Configuration
+00003e20: 2028 5041 4329 2069 6620 7468 6520 602d   (PAC) if the `-
+00003e30: 2d70 6163 6020 636f 6d6d 616e 6420 6c69  -pac` command li
+00003e40: 6e65 206f 7074 696f 6e20 6973 2073 7065  ne option is spe
+00003e50: 6369 6669 6564 2c20 6f72 2069 6620 7468  cified, or if th
+00003e60: 6520 6075 7365 5041 4360 2070 726f 7065  e `usePAC` prope
+00003e70: 7274 7920 6973 2073 6574 2074 6f20 6074  rty is set to `t
+00003e80: 7275 6560 2069 6e20 7468 6520 605b 636f  rue` in the `[co
+00003e90: 6d6d 6f6e 5d60 2073 6563 7469 6f6e 206f  mmon]` section o
+00003ea0: 6620 7468 6520 6063 6f6e 6669 672e 746f  f the `config.to
+00003eb0: 6d6c 6020 6669 6c65 2e0a 0a23 2320 5370  ml` file...## Sp
+00003ec0: 6563 6966 7969 6e67 2043 6f6d 6d6f 6e20  ecifying Common 
+00003ed0: 5072 6f70 6572 7469 6573 2075 7369 6e67  Properties using
+00003ee0: 2074 6865 2043 6f6d 6d61 6e64 204c 696e   the Command Lin
+00003ef0: 6520 6f72 2045 6e76 6972 6f6e 6d65 6e74  e or Environment
+00003f00: 2056 6172 6961 626c 6573 0a0a 416c 6c20   Variables..All 
+00003f10: 7468 6520 636f 6d6d 6f6e 2070 726f 7065  the common prope
+00003f20: 7274 6965 7320 6361 6e20 6265 2073 6574  rties can be set
+00003f30: 2075 7369 6e67 2063 6f6d 6d61 6e64 206c   using command l
+00003f40: 696e 6520 6f70 7469 6f6e 732c 206f 7220  ine options, or 
+00003f50: 696e 2065 6e76 6972 6f6e 6d65 6e74 2076  in environment v
+00003f60: 6172 6961 626c 6573 2e0a 0a54 6865 202a  ariables...The *
+00003f70: 2a63 6f6d 6d61 6e64 206c 696e 6520 6f70  *command line op
+00003f80: 7469 6f6e 732a 2a20 6172 6520 6173 2066  tions** are as f
+00003f90: 6f6c 6c6f 7773 3a0a 0a2d 2060 2d2d 6b65  ollows:..- `--ke
+00003fa0: 7960 206f 7220 602d 6b60 0a2d 2060 2d2d  y` or `-k`.- `--
+00003fb0: 7365 6372 6574 6020 6f72 2060 2d73 600a  secret` or `-s`.
+00003fc0: 2d20 602d 2d6e 616d 6573 7061 6365 6020  - `--namespace` 
+00003fd0: 6f72 2060 2d6e 600a 2d20 602d 2d74 6167  or `-n`.- `--tag
+00003fe0: 6020 6f72 2060 2d74 600a 2d20 602d 2d75  ` or `-t`.- `--u
+00003ff0: 726c 6020 6f72 2060 2d75 600a 2d20 602d  rl` or `-u`.- `-
+00004000: 2d70 6163 600a 0a54 6865 7365 206f 7074  -pac`..These opt
+00004010: 696f 6e73 2063 616e 2061 6c73 6f20 6265  ions can also be
+00004020: 206c 6973 7465 6420 6279 2072 756e 6e69   listed by runni
+00004030: 6e67 2061 2063 6f6d 6d61 6e64 2077 6974  ng a command wit
+00004040: 6820 7468 6520 602d 2d68 656c 7060 206f  h the `--help` o
+00004050: 7220 602d 6860 206f 7074 696f 6e2e 0a0a  r `-h` option...
+00004060: 5468 6520 2a2a 656e 7669 726f 6e6d 656e  The **environmen
+00004070: 7420 7661 7269 6162 6c65 732a 2a20 6172  t variables** ar
+00004080: 6520 6173 2066 6f6c 6c6f 7773 3a0a 0a2d  e as follows:..-
+00004090: 2060 5944 5f4b 4559 600a 2d20 6059 445f   `YD_KEY`.- `YD_
+000040a0: 5345 4352 4554 600a 2d20 6059 445f 4e41  SECRET`.- `YD_NA
+000040b0: 4d45 5350 4143 4560 0a2d 2060 5944 5f54  MESPACE`.- `YD_T
+000040c0: 4147 600a 2d20 6059 445f 5552 4c60 0a0a  AG`.- `YD_URL`..
+000040d0: 5768 656e 2073 6574 7469 6e67 2074 6865  When setting the
+000040e0: 2076 616c 7565 206f 6620 7468 6520 6162   value of the ab
+000040f0: 6f76 6520 7072 6f70 6572 7469 6573 2c20  ove properties, 
+00004100: 6120 7072 6f70 6572 7479 2073 6574 206f  a property set o
+00004110: 6e20 7468 6520 636f 6d6d 616e 6420 6c69  n the command li
+00004120: 6e65 2074 616b 6573 2070 7265 6365 6465  ne takes precede
+00004130: 6e63 6520 6f76 6572 206f 6e65 2073 6574  nce over one set
+00004140: 2076 6961 2061 6e20 656e 7669 726f 6e6d   via an environm
+00004150: 656e 7420 7661 7269 6162 6c65 2c20 616e  ent variable, an
+00004160: 6420 626f 7468 2074 616b 6520 7072 6563  d both take prec
+00004170: 6564 656e 6365 206f 7665 7220 6120 7661  edence over a va
+00004180: 6c75 6520 7365 7420 696e 2061 2063 6f6e  lue set in a con
+00004190: 6669 6775 7261 7469 6f6e 2066 696c 652e  figuration file.
+000041a0: 0a0a 4966 2061 6c6c 2074 6865 2072 6571  ..If all the req
+000041b0: 7569 7265 6420 636f 6d6d 6f6e 2070 726f  uired common pro
+000041c0: 7065 7274 6965 7320 6172 6520 7365 7420  perties are set 
+000041d0: 7573 696e 6720 7468 6520 636f 6d6d 616e  using the comman
+000041e0: 6420 6c69 6e65 206f 7220 656e 7669 726f  d line or enviro
+000041f0: 6e6d 656e 7420 7661 7269 6162 6c65 732c  nment variables,
+00004200: 2074 6865 6e20 7468 6520 656e 7469 7265   then the entire
+00004210: 2060 636f 6d6d 6f6e 6020 7365 6374 696f   `common` sectio
+00004220: 6e20 6f66 2074 6865 2054 4f4d 4c20 6669  n of the TOML fi
+00004230: 6c65 2063 616e 2062 6520 6f6d 6974 7465  le can be omitte
+00004240: 642e 0a0a 2323 2056 6172 6961 626c 6520  d...## Variable 
+00004250: 5375 6273 7469 7475 7469 6f6e 7320 696e  Substitutions in
+00004260: 2043 6f6d 6d6f 6e20 5072 6f70 6572 7469   Common Properti
+00004270: 6573 0a0a 4e6f 7465 2074 6865 2075 7365  es..Note the use
+00004280: 206f 6620 607b 7b75 7365 726e 616d 657d   of `{{username}
+00004290: 7d60 2069 6e20 7468 6520 7661 6c75 6520  }` in the value 
+000042a0: 6f66 2074 6865 2060 7461 6760 2070 726f  of the `tag` pro
+000042b0: 7065 7274 793a 2074 6869 7320 6973 2061  perty: this is a
+000042c0: 202a 2a76 6172 6961 626c 6520 7375 6273   **variable subs
+000042d0: 7469 7475 7469 6f6e 2a2a 2074 6861 7420  titution** that 
+000042e0: 6361 6e20 6f70 7469 6f6e 616c 6c79 2062  can optionally b
+000042f0: 6520 7573 6564 2074 6f20 696e 7365 7274  e used to insert
+00004300: 2074 6865 206c 6f67 696e 2075 7365 726e   the login usern
+00004310: 616d 6520 6f66 2074 6865 2075 7365 7220  ame of the user 
+00004320: 7275 6e6e 696e 6720 7468 6520 636f 6d6d  running the comm
+00004330: 616e 6473 2e20 536f 2c20 666f 7220 7573  ands. So, for us
+00004340: 6572 6e61 6d65 2060 6162 6360 2c20 7468  ername `abc`, th
+00004350: 6520 6074 6167 6020 776f 756c 6420 6265  e `tag` would be
+00004360: 2073 6574 2074 6f20 6074 6573 7469 6e67   set to `testing
+00004370: 2d61 6263 602e 2054 6869 7320 6361 6e20  -abc`. This can 
+00004380: 6265 2068 656c 7066 756c 2074 6f20 6469  be helpful to di
+00004390: 7361 6d62 6967 7561 7465 206d 756c 7469  sambiguate multi
+000043a0: 706c 6520 7573 6572 7320 7275 6e6e 696e  ple users runnin
+000043b0: 6720 7769 7468 2074 6865 2073 616d 6520  g with the same 
+000043c0: 636f 6e66 6967 7572 6174 696f 6e20 6461  configuration da
+000043d0: 7461 2e0a 0a56 6172 6961 626c 6520 7375  ta...Variable su
+000043e0: 6273 7469 7475 7469 6f6e 7320 6172 6520  bstitutions are 
+000043f0: 6469 7363 7573 7365 6420 6265 6c6f 772e  discussed below.
+00004400: 0a0a 2320 5661 7269 6162 6c65 2053 7562  ..# Variable Sub
+00004410: 7374 6974 7574 696f 6e73 0a0a 5661 7269  stitutions..Vari
+00004420: 6162 6c65 2073 7562 7374 6974 7574 696f  able substitutio
+00004430: 6e73 2070 726f 7669 6465 2061 2070 6f77  ns provide a pow
+00004440: 6572 6675 6c20 7761 7920 6f66 2069 6e74  erful way of int
+00004450: 726f 6475 6369 6e67 2076 6172 6961 626c  roducing variabl
+00004460: 6520 7661 6c75 6573 2069 6e74 6f20 544f  e values into TO
+00004470: 4d4c 2063 6f6e 6669 6775 7261 7469 6f6e  ML configuration
+00004480: 2066 696c 6573 2c20 576f 726b 2052 6571   files, Work Req
+00004490: 7569 7265 6d65 6e74 204a 534f 4e20 6465  uirement JSON de
+000044a0: 6669 6e69 7469 6f6e 732c 2061 6e64 2057  finitions, and W
+000044b0: 6f72 6b65 7220 506f 6f6c 204a 534f 4e20  orker Pool JSON 
+000044c0: 6465 6669 6e69 7469 6f6e 732e 2054 6865  definitions. The
+000044d0: 7920 6361 6e20 6265 2069 6e63 6c75 6465  y can be include
+000044e0: 6420 696e 2074 6865 2076 616c 7565 206f  d in the value o
+000044f0: 6620 616e 7920 7072 6f70 6572 7479 2069  f any property i
+00004500: 6e20 6561 6368 206f 6620 7468 6573 6520  n each of these 
+00004510: 6f62 6a65 6374 732c 2069 6e63 6c75 6469  objects, includi
+00004520: 6e67 2069 6e20 7661 6c75 6573 2077 6974  ng in values wit
+00004530: 6869 6e20 6c69 7374 7320 2865 2e67 2e2c  hin lists (e.g.,
+00004540: 2066 6f72 2074 6865 2060 6172 6775 6d65   for the `argume
+00004550: 6e74 7360 2070 726f 7065 7274 7929 2061  nts` property) a
+00004560: 6e64 2061 7272 6179 7320 2865 2e67 2e2c  nd arrays (e.g.,
+00004570: 2074 6865 2060 656e 7669 726f 6e6d 656e   the `environmen
+00004580: 7460 2070 726f 7065 7274 7929 2e0a 0a56  t` property)...V
+00004590: 6172 6961 626c 6520 7375 6273 7469 7475  ariable substitu
+000045a0: 7469 6f6e 7320 6172 6520 6578 7072 6573  tions are expres
+000045b0: 7365 6420 7573 696e 6720 607b 7b76 6172  sed using `{{var
+000045c0: 6961 626c 657d 7d60 206e 6f74 6174 696f  iable}}` notatio
+000045d0: 6e2c 2077 6865 7265 2074 6865 2065 7870  n, where the exp
+000045e0: 7265 7373 696f 6e20 6973 2072 6570 6c61  ression is repla
+000045f0: 6365 6420 6279 2074 6865 2076 616c 7565  ced by the value
+00004600: 206f 6620 6076 6172 6961 626c 6560 2e0a   of `variable`..
+00004610: 0a53 7562 7374 6974 7574 696f 6e73 2063  .Substitutions c
+00004620: 616e 2061 6c73 6f20 6265 2070 6572 666f  an also be perfo
+00004630: 726d 6564 2066 6f72 206e 6f6e 2d73 7472  rmed for non-str
+00004640: 696e 6720 286e 756d 6265 7220 616e 6420  ing (number and 
+00004650: 626f 6f6c 6561 6e29 2076 616c 7565 7320  boolean) values 
+00004660: 7573 696e 6720 7468 6520 606e 756d 3a60  using the `num:`
+00004670: 2061 6e64 2060 626f 6f6c 3a60 2070 7265   and `bool:` pre
+00004680: 6669 7865 7320 7769 7468 696e 2074 6865  fixes within the
+00004690: 2076 6172 6961 626c 6520 7375 6273 7469   variable substi
+000046a0: 7475 7469 6f6e 3a0a 0a2d 2044 6566 696e  tution:..- Defin
+000046b0: 6520 7468 6520 7661 7269 6162 6c65 2073  e the variable s
+000046c0: 7562 7374 6974 7574 696f 6e20 7573 696e  ubstitution usin
+000046d0: 6720 6f6e 6520 6f66 2074 6865 2066 6f6c  g one of the fol
+000046e0: 6c6f 7769 6e67 2070 6174 7465 726e 733a  lowing patterns:
+000046f0: 2060 227b 7b6e 756d 3a6d 795f 696e 747d   `"{{num:my_int}
+00004700: 7d22 602c 2060 227b 7b6e 756d 3a6d 795f  }"`, `"{{num:my_
+00004710: 666c 6f61 747d 7d22 602c 2060 227b 7b62  float}}"`, `"{{b
+00004720: 6f6f 6c3a 6d79 5f62 6f6f 6c7d 7d22 600a  ool:my_bool}}"`.
+00004730: 2d20 5661 7269 6162 6c65 2064 6566 696e  - Variable defin
+00004740: 6974 696f 6e73 2073 7570 706c 6965 6420  itions supplied 
+00004750: 6f6e 2074 6865 2063 6f6d 6d61 6e64 206c  on the command l
+00004760: 696e 6520 776f 756c 6420 7468 656e 2062  ine would then b
+00004770: 6520 6f66 2074 6865 2066 6f72 6d3a 2060  e of the form: `
+00004780: 2d6d 206d 795f 696e 743d 3520 2d6d 206d  -m my_int=5 -m m
+00004790: 795f 666c 6f61 743d 322e 3520 2d6d 206d  y_float=2.5 -m m
+000047a0: 795f 626f 6f6c 3d74 7275 6560 0a2d 2049  y_bool=true`.- I
+000047b0: 6e20 7468 6520 7072 6f63 6573 7365 6420  n the processed 
+000047c0: 4a53 4f4e 206f 7220 544f 4d4c 2c20 7468  JSON or TOML, th
+000047d0: 6573 6520 7661 6c75 6573 2077 6f75 6c64  ese values would
+000047e0: 2062 6563 6f6d 6520 6035 602c 2060 322e   become `5`, `2.
+000047f0: 3560 2061 6e64 2060 7472 7565 602c 2072  5` and `true`, r
+00004800: 6573 7065 6374 6976 656c 792c 2063 6f6e  espectively, con
+00004810: 7665 7274 6564 2066 726f 6d20 7374 7269  verted from stri
+00004820: 6e67 7320 746f 2074 6865 6972 2063 6f72  ngs to their cor
+00004830: 7265 6374 204a 534f 4e20 7479 7065 730a  rect JSON types.
+00004840: 0a23 2320 4465 6661 756c 7420 5661 7269  .## Default Vari
+00004850: 6162 6c65 730a 0a54 6865 2066 6f6c 6c6f  ables..The follo
+00004860: 7769 6e67 2073 7562 7374 6974 7574 696f  wing substitutio
+00004870: 6e73 2061 7265 2061 7574 6f6d 6174 6963  ns are automatic
+00004880: 616c 6c79 2063 7265 6174 6564 2061 6e64  ally created and
+00004890: 2063 616e 2062 6520 7573 6564 2069 6e20   can be used in 
+000048a0: 616e 7920 7365 6374 696f 6e20 6f66 2074  any section of t
+000048b0: 6865 2063 6f6e 6669 6775 7261 7469 6f6e  he configuration
+000048c0: 2066 696c 652c 206f 7220 696e 2061 6e79   file, or in any
+000048d0: 204a 534f 4e20 7370 6563 6966 6963 6174   JSON specificat
+000048e0: 696f 6e3a 0a0a 7c20 4469 7265 6374 6976  ion:..| Directiv
+000048f0: 6520 2020 2020 2020 7c20 4465 7363 7269  e       | Descri
+00004900: 7074 696f 6e20 2020 2020 2020 2020 2020  ption           
+00004910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004940: 2020 207c 2045 7861 6d70 6c65 206f 6620     | Example of 
+00004950: 5375 6273 7469 7475 7469 6f6e 207c 0a7c  Substitution |.|
+00004960: 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  :---------------
+00004970: 2d7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -|:-------------
+00004980: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004990: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000049a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000049b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c3a 2d2d  ------------|:--
+000049c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000049d0: 2d2d 2d2d 2d2d 7c0a 7c20 607b 7b75 7365  ------|.| `{{use
+000049e0: 726e 616d 657d 7d60 2020 7c20 5468 6520  rname}}`  | The 
+000049f0: 6375 7272 656e 7420 7573 6572 2773 206c  current user's l
+00004a00: 6f67 696e 2075 7365 726e 616d 652c 206c  ogin username, l
+00004a10: 6f77 6572 2063 6173 652c 2073 7061 6365  ower case, space
+00004a20: 7320 7265 706c 6163 6564 2020 2020 2020  s replaced      
+00004a30: 2020 2020 207c 206a 616e 655f 736d 6974       | jane_smit
+00004a40: 6820 2020 2020 2020 2020 2020 2020 207c  h              |
+00004a50: 0a7c 2060 7b7b 6461 7465 7d7d 6020 2020  .| `{{date}}`   
+00004a60: 2020 207c 2054 6865 2063 7572 7265 6e74     | The current
+00004a70: 2064 6174 6520 2855 5443 293a 2059 5959   date (UTC): YYY
+00004a80: 594d 4d44 4420 2020 2020 2020 2020 2020  YMMDD           
 00004a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004aa0: 7c0a 7c20 607b 7b6b 6579 7d7d 6020 2020  |.| `{{key}}`   
-00004ab0: 2020 2020 7c20 5468 6520 6170 706c 6963      | The applic
-00004ac0: 6174 696f 6e20 606b 6579 6020 7072 6f70  ation `key` prop
-00004ad0: 6572 7479 2e20 2020 2020 2020 2020 2020  erty.           
-00004ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004af0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00004aa0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00004ab0: 3230 3232 3130 3237 2020 2020 2020 2020  20221027        
+00004ac0: 2020 2020 2020 2020 7c0a 7c20 607b 7b74          |.| `{{t
+00004ad0: 696d 657d 7d60 2020 2020 2020 7c20 5468  ime}}`      | Th
+00004ae0: 6520 6375 7272 656e 7420 7469 6d65 2028  e current time (
+00004af0: 5554 4329 3a20 4848 4d4d 5353 2020 2020  UTC): HHMMSS    
 00004b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b10: 2020 2020 2020 2020 207c 0a7c 2060 7b7b           |.| `{{
-00004b20: 7365 6372 6574 7d7d 6020 2020 207c 2054  secret}}`    | T
-00004b30: 6865 2061 7070 6c69 6361 7469 6f6e 2060  he application `
-00004b40: 7365 6372 6574 6020 7072 6f70 6572 7479  secret` property
-00004b50: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
-00004b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b70: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-00004b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b90: 2020 7c0a 7c20 607b 7b75 726c 7d7d 6020    |.| `{{url}}` 
-00004ba0: 2020 2020 2020 7c20 5468 6520 506c 6174        | The Plat
-00004bb0: 666f 726d 2060 7572 6c60 2070 726f 7065  form `url` prope
-00004bc0: 7274 792e 2020 2020 2020 2020 2020 2020  rty.            
-00004bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004bf0: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-00004c00: 2020 2020 2020 2020 2020 207c 0a0a 466f             |..Fo
-00004c10: 7220 7468 6520 6064 6174 6560 2c20 6074  r the `date`, `t
-00004c20: 696d 6560 2c20 6064 6174 6574 696d 6560  ime`, `datetime`
-00004c30: 2061 6e64 2060 7261 6e64 6f6d 6020 6469   and `random` di
-00004c40: 7265 6374 6976 6573 2c20 7468 6520 7361  rectives, the sa
-00004c50: 6d65 2076 616c 7565 7320 7769 6c6c 2062  me values will b
-00004c60: 6520 7573 6564 2066 6f72 2074 6865 2064  e used for the d
-00004c70: 7572 6174 696f 6e20 6f66 2061 2063 6f6d  uration of a com
-00004c80: 6d61 6e64 202d 2d20 692e 652e 2c20 6966  mand -- i.e., if
-00004c90: 2060 7b7b 7469 6d65 7d7d 6020 6973 2075   `{{time}}` is u
-00004ca0: 7365 6420 7769 7468 696e 206d 756c 7469  sed within multi
-00004cb0: 706c 6520 7072 6f70 6572 7469 6573 2c20  ple properties, 
-00004cc0: 7468 6520 7361 6d65 2076 616c 7565 2077  the same value w
-00004cd0: 696c 6c20 6265 2075 7365 6420 666f 7220  ill be used for 
-00004ce0: 6561 6368 2073 7562 7374 6974 7574 696f  each substitutio
-00004cf0: 6e2e 0a0a 2323 2055 7365 722d 4465 6669  n...## User-Defi
-00004d00: 6e65 6420 5661 7269 6162 6c65 730a 0a41  ned Variables..A
-00004d10: 7262 6974 7261 7279 2076 6172 6961 626c  rbitrary variabl
-00004d20: 6573 2063 616e 2062 6520 7375 7070 6c69  es can be suppli
-00004d30: 6564 2075 7369 6e67 2063 6f6d 6d61 6e64  ed using command
-00004d40: 206c 696e 6520 6f70 7469 6f6e 732c 2062   line options, b
-00004d50: 7920 7365 7474 696e 6720 656e 7669 726f  y setting enviro
-00004d60: 6e6d 656e 7420 7661 7269 6162 6c65 7320  nment variables 
-00004d70: 7072 6566 6978 6564 2077 6974 6820 6059  prefixed with `Y
-00004d80: 445f 5641 525f 602c 206f 7220 6279 2069  D_VAR_`, or by i
-00004d90: 6e63 6c75 6469 6e67 2074 6865 2064 6972  ncluding the dir
-00004da0: 6563 7469 7665 7320 696e 2074 6865 2060  ectives in the `
-00004db0: 5b63 6f6d 6d6f 6e5d 6020 7365 6374 696f  [common]` sectio
-00004dc0: 6e20 6f66 2074 6865 2054 4f4d 4c20 636f  n of the TOML co
-00004dd0: 6e66 6967 7572 6174 696f 6e20 6669 6c65  nfiguration file
-00004de0: 2e0a 0a31 2e20 5468 6520 2a2a 636f 6d6d  ...1. The **comm
-00004df0: 616e 6420 6c69 6e65 2a2a 206f 7074 696f  and line** optio
-00004e00: 6e20 6973 2060 2d2d 7661 7269 6162 6c65  n is `--variable
-00004e10: 6020 286f 7220 602d 7660 292e 2046 6f72  ` (or `-v`). For
-00004e20: 2065 7861 6d70 6c65 2c20 6079 642d 7375   example, `yd-su
-00004e30: 626d 6974 202d 7620 7072 6f6a 6563 745f  bmit -v project_
-00004e40: 636f 6465 3d70 722d 3231 332d 6120 2d76  code=pr-213-a -v
-00004e50: 2072 756e 5f69 643d 3132 3334 6020 7769   run_id=1234` wi
-00004e60: 6c6c 2065 7374 6162 6c69 7368 2074 776f  ll establish two
-00004e70: 206e 6577 2076 6172 6961 626c 6573 2074   new variables t
-00004e80: 6861 7420 6361 6e20 6265 2075 7365 6420  hat can be used 
-00004e90: 6173 2060 7b7b 7072 6f6a 6563 745f 636f  as `{{project_co
-00004ea0: 6465 7d7d 6020 616e 6420 607b 7b72 756e  de}}` and `{{run
-00004eb0: 5f69 647d 7d60 2c20 7768 6963 6820 7769  _id}}`, which wi
-00004ec0: 6c6c 2062 6520 7375 6273 7469 7475 7465  ll be substitute
-00004ed0: 6420 6279 2060 7072 2d32 3133 2d61 6020  d by `pr-213-a` 
-00004ee0: 616e 6420 6031 3233 3460 2072 6573 7065  and `1234` respe
-00004ef0: 6374 6976 656c 792e 0a0a 0a32 2e20 466f  ctively....2. Fo
-00004f00: 7220 2a2a 656e 7669 726f 6e6d 656e 7420  r **environment 
-00004f10: 7661 7269 6162 6c65 732a 2a2c 2073 6574  variables**, set
-00004f20: 7469 6e67 2074 6865 2076 6172 6961 626c  ting the variabl
-00004f30: 6520 6059 445f 5641 525f 7072 6f6a 6563  e `YD_VAR_projec
-00004f40: 745f 636f 6465 3d22 7072 2d32 3133 2d61  t_code="pr-213-a
-00004f50: 2260 2077 696c 6c20 6372 6561 7465 2061  "` will create a
-00004f60: 206e 6577 2076 6172 6961 626c 6520 7468   new variable th
-00004f70: 6174 2063 616e 2062 6520 7573 6564 2061  at can be used a
-00004f80: 7320 607b 7b70 726f 6a65 6374 5f63 6f64  s `{{project_cod
-00004f90: 657d 7d60 2c20 7768 6963 6820 7769 6c6c  e}}`, which will
-00004fa0: 2062 6520 7375 6273 7469 7475 7465 6420   be substituted 
-00004fb0: 6279 2060 7072 2d32 3133 2d61 602e 0a0a  by `pr-213-a`...
-00004fc0: 0a33 2e20 466f 7220 2a2a 7365 7474 696e  .3. For **settin
-00004fd0: 6720 7769 7468 696e 2074 6865 2054 4f4d  g within the TOM
-00004fe0: 4c20 6669 6c65 2a2a 2c20 696e 636c 7564  L file**, includ
-00004ff0: 6520 6120 2a2a 6076 6172 6961 626c 6573  e a **`variables
-00005000: 602a 2a20 7461 626c 6520 696e 2074 6865  `** table in the
-00005010: 2060 5b63 6f6d 6d6f 6e5d 6020 7365 6374   `[common]` sect
-00005020: 696f 6e20 6f66 2074 6865 2066 696c 652e  ion of the file.
-00005030: 2045 2e67 2e2c 2060 7661 7269 6162 6c65   E.g., `variable
-00005040: 7320 3d20 7b70 726f 6a65 6374 5f63 6f64  s = {project_cod
-00005050: 6520 3d20 2270 722d 3231 3361 222c 2072  e = "pr-213a", r
-00005060: 756e 5f69 6420 3d20 2231 3233 3422 7d60  un_id = "1234"}`
-00005070: 2e20 4e6f 7465 2074 6861 7420 7468 6973  . Note that this
-00005080: 2063 616e 2061 6c73 6f20 7573 6520 7468   can also use th
-00005090: 6520 666f 726d 3a0a 0a60 6060 746f 6d6c  e form:..```toml
-000050a0: 0a5b 636f 6d6d 6f6e 2e76 6172 6961 626c  .[common.variabl
-000050b0: 6573 5d0a 7072 6f6a 6563 745f 636f 6465  es].project_code
-000050c0: 203d 2022 7072 2d32 3133 6122 0a72 756e   = "pr-213a".run
-000050d0: 5f69 6420 3d20 2231 3233 3422 0a60 6060  _id = "1234".```
-000050e0: 0a0a 4469 7265 6374 6976 6573 2073 6574  ..Directives set
-000050f0: 206f 6e20 7468 6520 636f 6d6d 616e 6420   on the command 
-00005100: 6c69 6e65 2074 616b 6520 7072 6563 6564  line take preced
-00005110: 656e 6365 206f 7665 7220 6469 7265 6374  ence over direct
-00005120: 6976 6573 2073 6574 2069 6e20 656e 7669  ives set in envi
-00005130: 726f 6e6d 656e 7420 7661 7269 6162 6c65  ronment variable
-00005140: 732c 2061 6e64 2062 6f74 6820 6f66 2074  s, and both of t
-00005150: 6865 6d20 7461 6b65 2070 7265 6365 6465  hem take precede
-00005160: 6e63 6520 6f76 6572 2064 6972 6563 7469  nce over directi
-00005170: 7665 7320 7365 7420 696e 2061 2054 4f4d  ves set in a TOM
-00005180: 4c20 6669 6c65 2e0a 0a54 6869 7320 6d65  L file...This me
-00005190: 7468 6f64 2063 616e 2062 6520 7573 6564  thod can be used
-000051a0: 2074 6f20 6f76 6572 7269 6465 2074 6865   to override the
-000051b0: 2064 6566 6175 6c74 2064 6972 6563 7469   default directi
-000051c0: 7665 732c 2065 2e67 2e2c 2073 6574 7469  ves, e.g., setti
-000051d0: 6e67 2060 2d76 2075 7365 726e 616d 653d  ng `-v username=
-000051e0: 226f 7468 6572 2d75 7365 7222 6020 7769  "other-user"` wi
-000051f0: 6c6c 206f 7665 7272 6964 6520 7468 6520  ll override the 
-00005200: 6465 6661 756c 7420 607b 7b75 7365 726e  default `{{usern
-00005210: 616d 657d 7d60 2064 6972 6563 7469 7665  ame}}` directive
-00005220: 2e0a 0a23 2320 4e65 7374 6564 2056 6172  ...## Nested Var
-00005230: 6961 626c 6573 0a0a 496e 2074 6865 2063  iables..In the c
-00005240: 6173 6520 6f66 202a 2a54 4f4d 4c20 7072  ase of **TOML pr
-00005250: 6f70 6572 7469 6573 206f 6e6c 792a 2a2c  operties only**,
-00005260: 2076 6172 6961 626c 6520 7375 6273 7469   variable substi
-00005270: 7475 7469 6f6e 7320 6361 6e20 6265 206e  tutions can be n
-00005280: 6573 7465 642e 0a0a 466f 7220 6578 616d  ested...For exam
-00005290: 706c 652c 2069 6620 6f6e 6520 7761 6e74  ple, if one want
-000052a0: 6564 2074 6f20 7365 6c65 6374 2061 2064  ed to select a d
-000052b0: 6966 6665 7265 6e74 2060 7465 6d70 6c61  ifferent `templa
-000052c0: 7465 4964 6020 666f 7220 6120 576f 726b  teId` for a Work
-000052d0: 6572 2050 6f6f 6c20 6465 7065 6e64 696e  er Pool dependin
-000052e0: 6720 6f6e 2074 6865 2076 616c 7565 206f  g on the value o
-000052f0: 6620 6120 6072 6567 696f 6e60 2076 6172  f a `region` var
-00005300: 6961 626c 652c 206f 6e65 2063 6f75 6c64  iable, one could
-00005310: 2075 7365 2074 6865 2066 6f6c 6c6f 7769   use the followi
-00005320: 6e67 3a0a 0a60 6060 746f 6d6c 0a5b 636f  ng:..```toml.[co
-00005330: 6d6d 6f6e 2e76 6172 6961 626c 6573 5d0a  mmon.variables].
-00005340: 2020 2020 7465 6d70 6c61 7465 5f6c 6f6e      template_lon
-00005350: 646f 6e20 3d20 2279 6469 643a 6372 743a  don = "ydid:crt:
-00005360: 3635 4546 3446 3a61 3464 3735 3763 662d  65EF4F:a4d757cf-
-00005370: 6236 3761 2d34 6562 362d 6264 3339 2d38  b67a-4eb6-bd39-8
-00005380: 6136 6666 6434 3663 3866 3422 0a20 2020  a6ffd46c8f4".   
-00005390: 2074 656d 706c 6174 655f 7068 6f65 6e69   template_phoeni
-000053a0: 7820 3d20 2279 6469 643a 6372 743a 3635  x = "ydid:crt:65
-000053b0: 4546 3446 3a65 3432 3339 6465 632d 3738  EF4F:e4239dec-78
-000053c0: 6332 2d34 3231 632d 6137 6633 2d37 3165  c2-421c-a7f3-71e
-000053d0: 3631 6237 3239 3436 6622 0a20 2020 2074  61b72946f".    t
-000053e0: 656d 706c 6174 655f 6672 616e 6b66 7572  emplate_frankfur
-000053f0: 7420 3d20 2279 6469 643a 6372 743a 3635  t = "ydid:crt:65
-00005400: 4546 3446 3a33 3239 3630 3263 662d 3539  EF4F:329602cf-59
-00005410: 3435 2d34 6161 642d 6132 3838 2d65 6134  45-4aad-a288-ea4
-00005420: 3234 6436 3464 3535 6522 0a0a 5b63 6f6d  24d64d55e"..[com
-00005430: 6d6f 6e2e 776f 726b 6572 506f 6f6c 5d0a  mon.workerPool].
-00005440: 2020 2020 7465 6d70 6c61 7465 4964 203d      templateId =
-00005450: 2022 7b7b 7465 6d70 6c61 7465 5f7b 7b72   "{{template_{{r
-00005460: 6567 696f 6e7d 7d7d 7d22 0a60 6060 0a0a  egion}}}}".```..
-00005470: 5468 656e 2c20 6966 206f 6e65 2075 7365  Then, if one use
-00005480: 6420 6079 642d 7072 6f76 6973 696f 6e20  d `yd-provision 
-00005490: 2d76 2072 6567 696f 6e3d 7068 6f65 6e69  -v region=phoeni
-000054a0: 7860 2c20 7468 6520 6074 656d 706c 6174  x`, the `templat
-000054b0: 6549 6460 2070 726f 7065 7274 7920 776f  eId` property wo
-000054c0: 756c 6420 6669 7273 7420 7265 736f 6c76  uld first resolv
-000054d0: 6520 746f 2060 227b 7b74 656d 706c 6174  e to `"{{templat
-000054e0: 655f 7068 656f 6e69 787d 7d22 602c 2061  e_pheonix}}"`, a
-000054f0: 6e64 2074 6865 6e20 746f 2060 2279 6469  nd then to `"ydi
-00005500: 643a 6372 743a 3635 4546 3446 3a65 3432  d:crt:65EF4F:e42
-00005510: 3339 6465 632d 3738 6332 2d34 3231 632d  39dec-78c2-421c-
-00005520: 6137 6633 2d37 3165 3631 6237 3239 3436  a7f3-71e61b72946
-00005530: 6622 602e 0a0a 4e65 7374 696e 6720 6361  f"`...Nesting ca
-00005540: 6e20 6265 2075 7020 746f 2074 6872 6565  n be up to three
-00005550: 206c 6576 656c 7320 6465 6570 2069 6e63   levels deep inc
-00005560: 6c75 6469 6e67 2074 6865 2074 6f70 206c  luding the top l
-00005570: 6576 656c 2e0a 0a23 2057 6f72 6b20 5265  evel...# Work Re
-00005580: 7175 6972 656d 656e 7420 5072 6f70 6572  quirement Proper
-00005590: 7469 6573 0a0a 5468 6520 6077 6f72 6b52  ties..The `workR
-000055a0: 6571 7569 7265 6d65 6e74 6020 7365 6374  equirement` sect
-000055b0: 696f 6e20 6f66 2074 6865 2063 6f6e 6669  ion of the confi
-000055c0: 6775 7261 7469 6f6e 2066 696c 6520 6973  guration file is
-000055d0: 206f 7074 696f 6e61 6c2e 2049 7427 7320   optional. It's 
-000055e0: 7573 6564 206f 6e6c 7920 6279 2074 6865  used only by the
-000055f0: 2060 7964 2d73 7562 6d69 7460 2063 6f6d   `yd-submit` com
-00005600: 6d61 6e64 2c20 616e 6420 636f 6e74 726f  mand, and contro
-00005610: 6c73 2074 6865 2057 6f72 6b20 5265 7175  ls the Work Requ
-00005620: 6972 656d 656e 7420 7468 6174 2069 7320  irement that is 
-00005630: 7375 626d 6974 7465 6420 746f 2074 6865  submitted to the
-00005640: 2050 6c61 7466 6f72 6d2e 0a0a 5468 6520   Platform...The 
-00005650: 6465 7461 696c 7320 6f66 2061 2057 6f72  details of a Wor
-00005660: 6b20 5265 7175 6972 656d 656e 7420 746f  k Requirement to
-00005670: 2062 6520 7375 626d 6974 7465 6420 6361   be submitted ca
-00005680: 6e20 6265 2063 6170 7475 7265 6420 656e  n be captured en
-00005690: 7469 7265 6c79 2077 6974 6869 6e20 7468  tirely within th
-000056a0: 6520 544f 4d4c 2063 6f6e 6669 6775 7261  e TOML configura
-000056b0: 7469 6f6e 2066 696c 6520 666f 7220 7369  tion file for si
-000056c0: 6d70 6c65 2065 7861 6d70 6c65 732e 204d  mple examples. M
-000056d0: 6f72 6520 636f 6d70 6c65 7820 6578 616d  ore complex exam
-000056e0: 706c 6573 2063 6170 7475 7265 2074 6865  ples capture the
-000056f0: 2057 6f72 6b20 5265 7175 6972 656d 656e   Work Requiremen
-00005700: 7420 696e 2061 2063 6f6d 6269 6e61 7469  t in a combinati
-00005710: 6f6e 206f 6620 7468 6520 544f 4d4c 2066  on of the TOML f
-00005720: 696c 6520 706c 7573 2061 204a 534f 4e20  ile plus a JSON 
-00005730: 646f 6375 6d65 6e74 2c20 6f72 2069 6e20  document, or in 
-00005740: 6120 4a53 4f4e 2064 6f63 756d 656e 7420  a JSON document 
-00005750: 6f6e 6c79 2e0a 0a23 2320 576f 726b 2052  only...## Work R
-00005760: 6571 7569 7265 6d65 6e74 204a 534f 4e20  equirement JSON 
-00005770: 4669 6c65 2053 7472 7563 7475 7265 0a0a  File Structure..
-00005780: 576f 726b 2052 6571 7569 7265 6d65 6e74  Work Requirement
-00005790: 7320 6172 6520 7265 7072 6573 656e 7465  s are represente
-000057a0: 6420 696e 204a 534f 4e20 646f 6375 6d65  d in JSON docume
-000057b0: 6e74 7320 7573 696e 6720 6120 636f 6e74  nts using a cont
-000057c0: 6169 6e6d 656e 7420 6869 6572 6172 6368  ainment hierarch
-000057d0: 7920 6f66 2061 202a 2a57 6f72 6b20 5265  y of a **Work Re
-000057e0: 7175 6972 656d 656e 742a 2a20 636f 6e74  quirement** cont
-000057f0: 6169 6e69 6e67 2061 202a 2a6c 6973 7420  aining a **list 
-00005800: 6f66 2054 6173 6b20 4772 6f75 7073 2a2a  of Task Groups**
-00005810: 2c20 636f 6e74 6169 6e69 6e67 2061 202a  , containing a *
-00005820: 2a6c 6973 7420 6f66 2054 6173 6b73 2a2a  *list of Tasks**
-00005830: 2e0a 0a41 2076 6572 7920 7369 6d70 6c65  ...A very simple
-00005840: 2065 7861 6d70 6c65 2064 6f63 756d 656e   example documen
-00005850: 7420 6973 2073 686f 776e 2062 656c 6f77  t is shown below
-00005860: 2077 6974 6820 6120 746f 702d 6c65 7665   with a top-leve
-00005870: 6c20 576f 726b 2052 6571 7569 7265 6d65  l Work Requireme
-00005880: 6e74 2063 6f6e 7461 696e 696e 6720 7477  nt containing tw
-00005890: 6f20 5461 736b 2047 726f 7570 7320 6561  o Task Groups ea
-000058a0: 6368 2063 6f6e 7461 696e 696e 6720 7477  ch containing tw
-000058b0: 6f20 5461 736b 732c 2065 6163 6820 7769  o Tasks, each wi
-000058c0: 7468 2061 2064 6966 6665 7265 6e74 2073  th a different s
-000058d0: 6574 206f 6620 6172 6775 6d65 6e74 7320  et of arguments 
-000058e0: 746f 2062 6520 7061 7373 6564 2074 6f20  to be passed to 
-000058f0: 7468 6520 5461 736b 2e0a 0a60 6060 6a73  the Task...```js
-00005900: 6f6e 0a7b 0a20 2022 7461 736b 4772 6f75  on.{.  "taskGrou
-00005910: 7073 223a 205b 0a20 2020 207b 0a20 2020  ps": [.    {.   
-00005920: 2020 2022 7461 736b 7322 3a20 5b0a 2020     "tasks": [.  
-00005930: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-00005940: 2020 2261 7267 756d 656e 7473 223a 205b    "arguments": [
-00005950: 312c 2032 2c20 335d 0a20 2020 2020 2020  1, 2, 3].       
-00005960: 207d 2c0a 2020 2020 2020 2020 7b0a 2020   },.        {.  
-00005970: 2020 2020 2020 2020 2261 7267 756d 656e          "argumen
-00005980: 7473 223a 205b 342c 2035 2c20 365d 0a20  ts": [4, 5, 6]. 
-00005990: 2020 2020 2020 207d 0a20 2020 2020 205d         }.      ]
-000059a0: 0a20 2020 207d 2c0a 2020 2020 7b0a 2020  .    },.    {.  
-000059b0: 2020 2020 2274 6173 6b73 223a 205b 0a20      "tasks": [. 
-000059c0: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
-000059d0: 2020 2022 6172 6775 6d65 6e74 7322 3a20     "arguments": 
-000059e0: 5b37 2c20 382c 2039 5d0a 2020 2020 2020  [7, 8, 9].      
-000059f0: 2020 7d2c 0a20 2020 2020 2020 207b 0a20    },.        {. 
-00005a00: 2020 2020 2020 2020 2022 6172 6775 6d65           "argume
-00005a10: 6e74 7322 3a20 5b31 302c 2031 312c 2031  nts": [10, 11, 1
-00005a20: 325d 0a20 2020 2020 2020 207d 0a20 2020  2].        }.   
-00005a30: 2020 205d 0a20 2020 207d 0a20 205d 0a7d     ].    }.  ].}
-00005a40: 0a0a 6060 600a 0a54 6f20 7370 6563 6966  ..```..To specif
-00005a50: 7920 7468 6520 6669 6c65 2063 6f6e 7461  y the file conta
-00005a60: 696e 696e 6720 7468 6520 4a53 4f4e 2064  ining the JSON d
-00005a70: 6f63 756d 656e 742c 2065 6974 6865 7220  ocument, either 
-00005a80: 706f 7075 6c61 7465 2074 6865 2060 776f  populate the `wo
-00005a90: 726b 5265 7175 6972 656d 656e 7444 6174  rkRequirementDat
-00005aa0: 6160 2070 726f 7065 7274 7920 696e 2074  a` property in t
-00005ab0: 6865 2060 776f 726b 5265 7175 6972 656d  he `workRequirem
-00005ac0: 656e 7460 2073 6563 7469 6f6e 206f 6620  ent` section of 
-00005ad0: 7468 6520 544f 4d4c 2063 6f6e 6669 6775  the TOML configu
-00005ae0: 7261 7469 6f6e 2066 696c 6520 7769 7468  ration file with
-00005af0: 2074 6865 204a 534f 4e20 6669 6c65 6e61   the JSON filena
-00005b00: 6d65 2c20 6f72 2073 7065 6369 6679 2069  me, or specify i
-00005b10: 7420 6f6e 2074 6865 2063 6f6d 6d61 6e64  t on the command
-00005b20: 206c 696e 6520 7573 696e 6720 7468 6520   line using the 
-00005b30: 602d 2d77 6f72 6b2d 7265 7175 6972 656d  `--work-requirem
-00005b40: 656e 7460 206f 7220 602d 7260 206f 7074  ent` or `-r` opt
-00005b50: 696f 6e73 2028 7768 6963 6820 7769 6c6c  ions (which will
-00005b60: 206f 7665 7272 6964 6520 7468 6520 7072   override the pr
-00005b70: 6f70 6572 7479 2069 6e20 7468 6520 544f  operty in the TO
-00005b80: 4d4c 2066 696c 6529 2c20 652e 672e 0a0a  ML file), e.g...
-00005b90: 6079 642d 7375 626d 6974 202d 2d63 6f6e  `yd-submit --con
-00005ba0: 6669 6720 6d79 636f 6e66 6967 2e74 6f6d  fig myconfig.tom
-00005bb0: 6c20 2d2d 776f 726b 2d72 6571 7569 7265  l --work-require
-00005bc0: 6d65 6e74 206d 795f 776f 726b 7265 712e  ment my_workreq.
-00005bd0: 6a73 6f6e 600a 0a23 2320 5072 6f70 6572  json`..## Proper
-00005be0: 7479 2049 6e68 6572 6974 616e 6365 0a0a  ty Inheritance..
-00005bf0: 546f 2073 696d 706c 6966 7920 7468 6520  To simplify the 
-00005c00: 6465 6669 6e69 7469 6f6e 206f 6620 576f  definition of Wo
-00005c10: 726b 2052 6571 7569 7265 6d65 6e74 732c  rk Requirements,
-00005c20: 2074 6865 7265 2069 7320 6120 7072 6f70   there is a prop
-00005c30: 6572 7479 2069 6e68 6572 6974 616e 6365  erty inheritance
-00005c40: 206d 6563 6861 6e69 736d 2e20 5072 6f70   mechanism. Prop
-00005c50: 6572 7469 6573 2074 6861 7420 6172 6520  erties that are 
-00005c60: 7365 7420 6174 2061 2068 6967 6865 7220  set at a higher 
-00005c70: 6c65 7665 6c20 696e 2074 6865 2068 6965  level in the hie
-00005c80: 7261 7263 6879 2061 7265 2069 6e68 6572  rarchy are inher
-00005c90: 6974 6564 2061 7420 6c6f 7765 7220 6c65  ited at lower le
-00005ca0: 7665 6c73 2c20 756e 6c65 7373 2065 7870  vels, unless exp
-00005cb0: 6c69 6369 746c 7920 6f76 6572 7269 6464  licitly overridd
-00005cc0: 656e 2e0a 0a54 6869 7320 6d65 616e 7320  en...This means 
-00005cd0: 7468 6174 2061 2070 726f 7065 7274 7920  that a property 
-00005ce0: 7365 7420 696e 2074 6865 2060 776f 726b  set in the `work
-00005cf0: 5265 7175 6972 656d 656e 7460 2073 6563  Requirement` sec
-00005d00: 7469 6f6e 206f 6620 7468 6520 544f 4d4c  tion of the TOML
-00005d10: 2066 696c 6520 6361 6e20 6265 2069 6e68   file can be inh
-00005d20: 6572 6974 6564 2073 7563 6365 7373 6976  erited successiv
-00005d30: 656c 7920 6279 2074 6865 2057 6f72 6b20  ely by the Work 
-00005d40: 5265 7175 6972 656d 656e 742c 2054 6173  Requirement, Tas
-00005d50: 6b20 4772 6f75 7073 2061 6e64 2054 6173  k Groups and Tas
-00005d60: 6b73 2069 6e20 7468 6520 4a53 4f4e 2064  ks in the JSON d
-00005d70: 6f63 756d 656e 7420 2861 7373 756d 696e  ocument (assumin
-00005d80: 6720 7468 6520 7072 6f70 6572 7479 2069  g the property i
-00005d90: 7320 7661 6c69 6420 6174 2065 6163 6820  s valid at each 
-00005da0: 6c65 7665 6c29 2e20 2048 656e 6365 2c20  level).  Hence, 
-00005db0: 5461 736b 7320 696e 6865 7269 7420 6672  Tasks inherit fr
-00005dc0: 6f6d 2054 6173 6b20 4772 6f75 7073 2c20  om Task Groups, 
-00005dd0: 7768 6963 6820 696e 6865 7269 7420 6672  which inherit fr
-00005de0: 6f6d 2074 6865 2057 6f72 6b20 5265 7175  om the Work Requ
-00005df0: 6972 656d 656e 7420 696e 2074 6865 204a  irement in the J
-00005e00: 534f 4e20 646f 6375 6d65 6e74 2c20 7768  SON document, wh
-00005e10: 6963 6820 696e 6865 7269 7473 2066 726f  ich inherits fro
-00005e20: 6d20 7468 6520 6077 6f72 6b52 6571 7569  m the `workRequi
-00005e30: 7265 6d65 6e74 6020 7072 6f70 6572 7469  rement` properti
-00005e40: 6573 2069 6e20 7468 6520 544f 4d4c 2066  es in the TOML f
-00005e50: 696c 652e 0a0a 4f76 6572 7269 6464 656e  ile...Overridden
-00005e60: 2070 726f 7065 7274 6965 7320 6172 6520   properties are 
-00005e70: 616c 736f 2069 6e68 6572 6974 6564 2e20  also inherited. 
-00005e80: 452e 672e 2c20 6966 2061 2070 726f 7065  E.g., if a prope
-00005e90: 7274 7920 6973 2073 6574 2061 7420 7468  rty is set at th
-00005ea0: 6520 5461 736b 2047 726f 7570 206c 6576  e Task Group lev
-00005eb0: 656c 2c20 6974 2077 696c 6c20 6265 2069  el, it will be i
-00005ec0: 6e68 6572 6974 6564 2062 7920 7468 6520  nherited by the 
-00005ed0: 5461 736b 7320 696e 2074 6861 7420 5461  Tasks in that Ta
-00005ee0: 736b 2047 726f 7570 2075 6e6c 6573 7320  sk Group unless 
-00005ef0: 6578 706c 6963 6974 6c79 206f 7665 7272  explicitly overr
-00005f00: 6964 6465 6e2e 0a0a 2323 2057 6f72 6b20  idden...## Work 
-00005f10: 5265 7175 6972 656d 656e 7420 5072 6f70  Requirement Prop
-00005f20: 6572 7479 2044 6963 7469 6f6e 6172 790a  erty Dictionary.
-00005f30: 0a54 6865 2066 6f6c 6c6f 7769 6e67 2074  .The following t
-00005f40: 6162 6c65 206f 7574 6c69 6e65 7320 616c  able outlines al
-00005f50: 6c20 7468 6520 7072 6f70 6572 7469 6573  l the properties
-00005f60: 2061 7661 696c 6162 6c65 2066 6f72 2064   available for d
-00005f70: 6566 696e 696e 6720 576f 726b 2052 6571  efining Work Req
-00005f80: 7569 7265 6d65 6e74 732c 2061 6e64 2074  uirements, and t
-00005f90: 6865 206c 6576 656c 7320 6174 2077 6869  he levels at whi
-00005fa0: 6368 2074 6865 7920 6172 6520 616c 6c6f  ch they are allo
-00005fb0: 7765 6420 746f 2062 6520 7573 6564 2e20  wed to be used. 
-00005fc0: 536f 2c20 666f 7220 6578 616d 706c 652c  So, for example,
-00005fd0: 2074 6865 2060 7072 6f76 6964 6572 6020   the `provider` 
-00005fe0: 7072 6f70 6572 7479 2063 616e 2062 6520  property can be 
-00005ff0: 7365 7420 696e 2074 6865 2054 4f4d 4c20  set in the TOML 
-00006000: 6669 6c65 2c20 6174 2074 6865 2057 6f72  file, at the Wor
-00006010: 6b20 5265 7175 6972 656d 656e 7420 4c65  k Requirement Le
-00006020: 7665 6c20 6f72 2061 7420 7468 6520 5461  vel or at the Ta
-00006030: 736b 2047 726f 7570 204c 6576 656c 2c20  sk Group Level, 
-00006040: 6275 7420 6e6f 7420 6174 2074 6865 2054  but not at the T
-00006050: 6173 6b20 6c65 7665 6c2c 2061 6e64 2070  ask level, and p
-00006060: 726f 7065 7274 7920 6064 6570 656e 6465  roperty `depende
-00006070: 6e74 4f6e 6020 6361 6e20 6f6e 6c79 2062  ntOn` can only b
-00006080: 6520 7365 7420 6174 2074 6865 2054 6173  e set at the Tas
-00006090: 6b20 4772 6f75 7020 6c65 7665 6c2e 0a0a  k Group level...
-000060a0: 416c 6c20 7072 6f70 6572 7469 6573 2061  All properties a
-000060b0: 7265 206f 7074 696f 6e61 6c20 6578 6365  re optional exce
-000060c0: 7074 2066 6f72 202a 2a60 7461 736b 5479  pt for **`taskTy
-000060d0: 7065 602a 2a20 286f 7220 2a2a 6074 6173  pe`** (or **`tas
-000060e0: 6b54 7970 6573 602a 2a29 2e0a 0a7c 2050  kTypes`**)...| P
-000060f0: 726f 7065 7274 7920 4e61 6d65 2020 2020  roperty Name    
-00006100: 2020 2020 2020 2020 2020 7c20 4465 7363            | Desc
-00006110: 7269 7074 696f 6e20 2020 2020 2020 2020  ription         
-00006120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061b0: 2020 2020 207c 2054 4f4d 4c20 7c20 5752       | TOML | WR
-000061c0: 2020 7c20 5447 7270 207c 2054 6173 6b20    | TGrp | Task 
-000061d0: 7c0a 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |.|:------------
-000061e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  ---------------|
-000061f0: 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  :---------------
-00006200: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006210: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006220: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006230: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006240: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006250: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006260: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006270: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006280: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00006290: 2d2d 2d2d 2d2d 2d2d 2d2d 7c3a 2d2d 2d2d  ----------|:----
-000062a0: 2d7c 3a2d 2d2d 2d7c 3a2d 2d2d 2d2d 7c3a  -|:----|:-----|:
-000062b0: 2d2d 2d2d 2d7c 0a7c 2060 6172 6775 6d65  -----|.| `argume
-000062c0: 6e74 7360 2020 2020 2020 2020 2020 2020  nts`            
-000062d0: 2020 2020 7c20 5468 6520 6c69 7374 206f      | The list o
-000062e0: 6620 6172 6775 6d65 6e74 7320 746f 2062  f arguments to b
-000062f0: 6520 7061 7373 6564 2074 6f20 7468 6520  e passed to the 
-00006300: 5461 736b 2077 6865 6e20 6974 2069 7320  Task when it is 
-00006310: 6578 6563 7574 6564 2e20 452e 672e 3a20  executed. E.g.: 
-00006320: 605b 312c 2022 5477 6f22 5d60 2e20 2020  `[1, "Two"]`.   
-00006330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006370: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00006380: 2059 6573 2020 7c20 5965 7320 7c20 5965   Yes  | Yes | Ye
-00006390: 7320 207c 2059 6573 2020 7c0a 7c20 6063  s  | Yes  |.| `c
-000063a0: 6170 7475 7265 5461 736b 4f75 7470 7574  aptureTaskOutput
-000063b0: 6020 2020 2020 2020 207c 2057 6865 7468  `        | Wheth
-000063c0: 6572 2074 6865 2063 6f6e 736f 6c65 206f  er the console o
-000063d0: 7574 7075 7420 6f66 2061 2054 6173 6b27  utput of a Task'
-000063e0: 7320 7072 6f63 6573 7320 7368 6f75 6c64  s process should
-000063f0: 2062 6520 7570 6c6f 6164 6564 2074 6f20   be uploaded to 
-00006400: 7468 6520 5965 6c6c 6f77 446f 6720 4f62  the YellowDog Ob
-00006410: 6a65 6374 2053 746f 7265 206f 6e20 5461  ject Store on Ta
-00006420: 736b 2063 6f6d 706c 6574 696f 6e2e 2044  sk completion. D
-00006430: 6566 6175 6c74 3a20 6074 7275 6560 2e20  efault: `true`. 
-00006440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006460: 2020 2020 7c20 5965 7320 207c 2059 6573      | Yes  | Yes
-00006470: 207c 2059 6573 2020 7c20 5965 7320 207c   | Yes  | Yes  |
-00006480: 0a7c 2060 636f 6d70 6c65 7465 6454 6173  .| `completedTas
-00006490: 6b54 746c 6020 2020 2020 2020 2020 7c20  kTtl`         | 
-000064a0: 5468 6520 7469 6d65 2028 696e 206d 696e  The time (in min
-000064b0: 7574 6573 2920 746f 206c 6976 6520 666f  utes) to live fo
-000064c0: 7220 636f 6d70 6c65 7465 6420 5461 736b  r completed Task
-000064d0: 732e 2049 6620 7365 742c 2054 6173 6b73  s. If set, Tasks
-000064e0: 2074 6861 7420 6861 7665 2062 6565 6e20   that have been 
-000064f0: 636f 6d70 6c65 7465 6420 666f 7220 6c6f  completed for lo
-00006500: 6e67 6572 2074 6861 6e20 7468 6973 2070  nger than this p
-00006510: 6572 696f 6420 7769 6c6c 2062 6520 6465  eriod will be de
-00006520: 6c65 7465 642e 2045 2e67 2e3a 2060 3130  leted. E.g.: `10
-00006530: 2e30 602e 2020 2020 2020 2020 2020 2020  .0`.            
-00006540: 2020 2020 2020 2020 207c 2059 6573 2020           | Yes  
-00006550: 7c20 5965 7320 7c20 5965 7320 207c 2020  | Yes | Yes  |  
-00006560: 2020 2020 7c0a 7c20 6063 7376 4669 6c65      |.| `csvFile
-00006570: 6020 2020 2020 2020 2020 2020 2020 2020  `               
-00006580: 2020 207c 2054 6865 206e 616d 6520 6f66     | The name of
-00006590: 2074 6865 2043 5356 2066 696c 6520 7573   the CSV file us
-000065a0: 6564 2074 6f20 6465 7269 7665 2054 6173  ed to derive Tas
-000065b0: 6b20 6461 7461 2e20 416e 2061 6c74 6572  k data. An alter
-000065c0: 6e61 7469 7665 2074 6f20 6063 7376 4669  native to `csvFi
-000065d0: 6c65 7360 2074 6861 7420 6361 6e20 6265  les` that can be
-000065e0: 2075 7365 6420 7768 656e 2074 6865 7265   used when there
-000065f0: 2773 206f 6e6c 7920 6120 7369 6e67 6c65  's only a single
-00006600: 2043 5356 2066 696c 652e 2045 2e67 2e20   CSV file. E.g. 
-00006610: 6022 6669 6c65 2e63 7376 2260 2e20 2020  `"file.csv"`.   
-00006620: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00006630: 5965 7320 207c 2020 2020 207c 2020 2020  Yes  |     |    
-00006640: 2020 7c20 2020 2020 207c 0a7c 2060 6373    |      |.| `cs
-00006650: 7646 696c 6573 6020 2020 2020 2020 2020  vFiles`         
-00006660: 2020 2020 2020 2020 7c20 4120 6c69 7374          | A list
-00006670: 206f 6620 4353 5620 6669 6c65 7320 7573   of CSV files us
-00006680: 6564 2074 6f20 6465 7269 7665 2054 6173  ed to derive Tas
-00006690: 6b20 6461 7461 2e20 452e 672e 2060 5b22  k data. E.g. `["
-000066a0: 6669 6c65 2e63 7376 222c 2022 6669 6c65  file.csv", "file
-000066b0: 5f32 2e63 7376 3a32 5d60 2e20 2020 2020  _2.csv:2]`.     
-000066c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b20: 2020 2020 2020 207c 2031 3633 3032 3620         | 163026 
+00004b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b40: 207c 0a7c 2060 7b7b 6461 7465 7469 6d65   |.| `{{datetime
+00004b50: 7d7d 6020 207c 2043 6f6e 6361 7465 6e61  }}`  | Concatena
+00004b60: 7469 6f6e 206f 6620 7468 6520 6461 7465  tion of the date
+00004b70: 2061 6e64 2074 696d 6520 6162 6f76 652c   and time above,
+00004b80: 2077 6974 6820 6120 272d 2720 7365 7061   with a '-' sepa
+00004b90: 7261 746f 7220 2020 2020 2020 2020 2020  rator           
+00004ba0: 7c20 3230 3232 3130 3237 2d31 3633 3032  | 20221027-16302
+00004bb0: 3620 2020 2020 2020 2020 7c0a 7c20 607b  6         |.| `{
+00004bc0: 7b72 616e 646f 6d7d 7d60 2020 2020 7c20  {random}}`    | 
+00004bd0: 4120 7261 6e64 6f6d 2c20 7468 7265 6520  A random, three 
+00004be0: 6469 6769 7420 6865 7861 6465 6369 6d61  digit hexadecima
+00004bf0: 6c20 6e75 6d62 6572 2028 6c6f 7765 7220  l number (lower 
+00004c00: 6361 7365 2920 2020 2020 2020 2020 2020  case)           
+00004c10: 2020 2020 2020 2020 207c 2061 3163 2020           | a1c  
+00004c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c30: 2020 207c 0a7c 2060 7b7b 6e61 6d65 7370     |.| `{{namesp
+00004c40: 6163 657d 7d60 207c 2054 6865 2060 6e61  ace}}` | The `na
+00004c50: 6d65 7370 6163 6560 2070 726f 7065 7274  mespace` propert
+00004c60: 792e 204e 6f74 6520 7468 6174 2060 6e61  y. Note that `na
+00004c70: 6d65 7370 6163 6560 206d 7573 742c 206f  mespace` must, o
+00004c80: 6620 636f 7572 7365 2c20 6265 2073 6574  f course, be set
+00004c90: 2e20 7c20 6d79 5f6e 616d 6573 7061 6365  . | my_namespace
+00004ca0: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
+00004cb0: 607b 7b74 6167 7d7d 6020 2020 2020 2020  `{{tag}}`       
+00004cc0: 7c20 5468 6520 6074 6167 6020 7072 6f70  | The `tag` prop
+00004cd0: 6572 7479 2e20 4e6f 7465 2074 6861 7420  erty. Note that 
+00004ce0: 6074 6167 6020 6d75 7374 2062 6520 7365  `tag` must be se
+00004cf0: 742e 2020 2020 2020 2020 2020 2020 2020  t.              
+00004d00: 2020 2020 2020 2020 2020 207c 206d 795f             | my_
+00004d10: 7461 6720 2020 2020 2020 2020 2020 2020  tag             
+00004d20: 2020 2020 207c 0a7c 2060 7b7b 6b65 797d       |.| `{{key}
+00004d30: 7d60 2020 2020 2020 207c 2054 6865 2061  }`       | The a
+00004d40: 7070 6c69 6361 7469 6f6e 2060 6b65 7960  pplication `key`
+00004d50: 2070 726f 7065 7274 792e 2020 2020 2020   property.      
+00004d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d80: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+00004d90: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+00004da0: 7c20 607b 7b73 6563 7265 747d 7d60 2020  | `{{secret}}`  
+00004db0: 2020 7c20 5468 6520 6170 706c 6963 6174    | The applicat
+00004dc0: 696f 6e20 6073 6563 7265 7460 2070 726f  ion `secret` pro
+00004dd0: 7065 7274 792e 2020 2020 2020 2020 2020  perty.          
+00004de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004df0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+00004e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e10: 2020 2020 2020 207c 0a7c 2060 7b7b 7572         |.| `{{ur
+00004e20: 6c7d 7d60 2020 2020 2020 207c 2054 6865  l}}`       | The
+00004e30: 2050 6c61 7466 6f72 6d20 6075 726c 6020   Platform `url` 
+00004e40: 7072 6f70 6572 7479 2e20 2020 2020 2020  property.       
+00004e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e70: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
+00004e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e90: 7c0a 0a46 6f72 2074 6865 2060 6461 7465  |..For the `date
+00004ea0: 602c 2060 7469 6d65 602c 2060 6461 7465  `, `time`, `date
+00004eb0: 7469 6d65 6020 616e 6420 6072 616e 646f  time` and `rando
+00004ec0: 6d60 2064 6972 6563 7469 7665 732c 2074  m` directives, t
+00004ed0: 6865 2073 616d 6520 7661 6c75 6573 2077  he same values w
+00004ee0: 696c 6c20 6265 2075 7365 6420 666f 7220  ill be used for 
+00004ef0: 7468 6520 6475 7261 7469 6f6e 206f 6620  the duration of 
+00004f00: 6120 636f 6d6d 616e 6420 2d2d 2069 2e65  a command -- i.e
+00004f10: 2e2c 2069 6620 607b 7b74 696d 657d 7d60  ., if `{{time}}`
+00004f20: 2069 7320 7573 6564 2077 6974 6869 6e20   is used within 
+00004f30: 6d75 6c74 6970 6c65 2070 726f 7065 7274  multiple propert
+00004f40: 6965 732c 2074 6865 2073 616d 6520 7661  ies, the same va
+00004f50: 6c75 6520 7769 6c6c 2062 6520 7573 6564  lue will be used
+00004f60: 2066 6f72 2065 6163 6820 7375 6273 7469   for each substi
+00004f70: 7475 7469 6f6e 2e0a 0a23 2320 5573 6572  tution...## User
+00004f80: 2d44 6566 696e 6564 2056 6172 6961 626c  -Defined Variabl
+00004f90: 6573 0a0a 4172 6269 7472 6172 7920 7661  es..Arbitrary va
+00004fa0: 7269 6162 6c65 7320 6361 6e20 6265 2073  riables can be s
+00004fb0: 7570 706c 6965 6420 7573 696e 6720 636f  upplied using co
+00004fc0: 6d6d 616e 6420 6c69 6e65 206f 7074 696f  mmand line optio
+00004fd0: 6e73 2c20 6279 2073 6574 7469 6e67 2065  ns, by setting e
+00004fe0: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
+00004ff0: 626c 6573 2070 7265 6669 7865 6420 7769  bles prefixed wi
+00005000: 7468 2060 5944 5f56 4152 5f60 2c20 6f72  th `YD_VAR_`, or
+00005010: 2062 7920 696e 636c 7564 696e 6720 7468   by including th
+00005020: 6520 6469 7265 6374 6976 6573 2069 6e20  e directives in 
+00005030: 7468 6520 605b 636f 6d6d 6f6e 5d60 2073  the `[common]` s
+00005040: 6563 7469 6f6e 206f 6620 7468 6520 544f  ection of the TO
+00005050: 4d4c 2063 6f6e 6669 6775 7261 7469 6f6e  ML configuration
+00005060: 2066 696c 652e 0a0a 312e 2054 6865 202a   file...1. The *
+00005070: 2a63 6f6d 6d61 6e64 206c 696e 652a 2a20  *command line** 
+00005080: 6f70 7469 6f6e 2069 7320 602d 2d76 6172  option is `--var
+00005090: 6961 626c 6560 2028 6f72 2060 2d76 6029  iable` (or `-v`)
+000050a0: 2e20 466f 7220 6578 616d 706c 652c 2060  . For example, `
+000050b0: 7964 2d73 7562 6d69 7420 2d76 2070 726f  yd-submit -v pro
+000050c0: 6a65 6374 5f63 6f64 653d 7072 2d32 3133  ject_code=pr-213
+000050d0: 2d61 202d 7620 7275 6e5f 6964 3d31 3233  -a -v run_id=123
+000050e0: 3460 2077 696c 6c20 6573 7461 626c 6973  4` will establis
+000050f0: 6820 7477 6f20 6e65 7720 7661 7269 6162  h two new variab
+00005100: 6c65 7320 7468 6174 2063 616e 2062 6520  les that can be 
+00005110: 7573 6564 2061 7320 607b 7b70 726f 6a65  used as `{{proje
+00005120: 6374 5f63 6f64 657d 7d60 2061 6e64 2060  ct_code}}` and `
+00005130: 7b7b 7275 6e5f 6964 7d7d 602c 2077 6869  {{run_id}}`, whi
+00005140: 6368 2077 696c 6c20 6265 2073 7562 7374  ch will be subst
+00005150: 6974 7574 6564 2062 7920 6070 722d 3231  ituted by `pr-21
+00005160: 332d 6160 2061 6e64 2060 3132 3334 6020  3-a` and `1234` 
+00005170: 7265 7370 6563 7469 7665 6c79 2e0a 0a0a  respectively....
+00005180: 322e 2046 6f72 202a 2a65 6e76 6972 6f6e  2. For **environ
+00005190: 6d65 6e74 2076 6172 6961 626c 6573 2a2a  ment variables**
+000051a0: 2c20 7365 7474 696e 6720 7468 6520 7661  , setting the va
+000051b0: 7269 6162 6c65 2060 5944 5f56 4152 5f70  riable `YD_VAR_p
+000051c0: 726f 6a65 6374 5f63 6f64 653d 2270 722d  roject_code="pr-
+000051d0: 3231 332d 6122 6020 7769 6c6c 2063 7265  213-a"` will cre
+000051e0: 6174 6520 6120 6e65 7720 7661 7269 6162  ate a new variab
+000051f0: 6c65 2074 6861 7420 6361 6e20 6265 2075  le that can be u
+00005200: 7365 6420 6173 2060 7b7b 7072 6f6a 6563  sed as `{{projec
+00005210: 745f 636f 6465 7d7d 602c 2077 6869 6368  t_code}}`, which
+00005220: 2077 696c 6c20 6265 2073 7562 7374 6974   will be substit
+00005230: 7574 6564 2062 7920 6070 722d 3231 332d  uted by `pr-213-
+00005240: 6160 2e0a 0a0a 332e 2046 6f72 202a 2a73  a`....3. For **s
+00005250: 6574 7469 6e67 2077 6974 6869 6e20 7468  etting within th
+00005260: 6520 544f 4d4c 2066 696c 652a 2a2c 2069  e TOML file**, i
+00005270: 6e63 6c75 6465 2061 202a 2a60 7661 7269  nclude a **`vari
+00005280: 6162 6c65 7360 2a2a 2074 6162 6c65 2069  ables`** table i
+00005290: 6e20 7468 6520 605b 636f 6d6d 6f6e 5d60  n the `[common]`
+000052a0: 2073 6563 7469 6f6e 206f 6620 7468 6520   section of the 
+000052b0: 6669 6c65 2e20 452e 672e 2c20 6076 6172  file. E.g., `var
+000052c0: 6961 626c 6573 203d 207b 7072 6f6a 6563  iables = {projec
+000052d0: 745f 636f 6465 203d 2022 7072 2d32 3133  t_code = "pr-213
+000052e0: 6122 2c20 7275 6e5f 6964 203d 2022 3132  a", run_id = "12
+000052f0: 3334 227d 602e 204e 6f74 6520 7468 6174  34"}`. Note that
+00005300: 2074 6869 7320 6361 6e20 616c 736f 2075   this can also u
+00005310: 7365 2074 6865 2066 6f72 6d3a 0a0a 6060  se the form:..``
+00005320: 6074 6f6d 6c0a 5b63 6f6d 6d6f 6e2e 7661  `toml.[common.va
+00005330: 7269 6162 6c65 735d 0a70 726f 6a65 6374  riables].project
+00005340: 5f63 6f64 6520 3d20 2270 722d 3231 3361  _code = "pr-213a
+00005350: 220a 7275 6e5f 6964 203d 2022 3132 3334  ".run_id = "1234
+00005360: 220a 6060 600a 0a44 6972 6563 7469 7665  ".```..Directive
+00005370: 7320 7365 7420 6f6e 2074 6865 2063 6f6d  s set on the com
+00005380: 6d61 6e64 206c 696e 6520 7461 6b65 2070  mand line take p
+00005390: 7265 6365 6465 6e63 6520 6f76 6572 2064  recedence over d
+000053a0: 6972 6563 7469 7665 7320 7365 7420 696e  irectives set in
+000053b0: 2065 6e76 6972 6f6e 6d65 6e74 2076 6172   environment var
+000053c0: 6961 626c 6573 2c20 616e 6420 626f 7468  iables, and both
+000053d0: 206f 6620 7468 656d 2074 616b 6520 7072   of them take pr
+000053e0: 6563 6564 656e 6365 206f 7665 7220 6469  ecedence over di
+000053f0: 7265 6374 6976 6573 2073 6574 2069 6e20  rectives set in 
+00005400: 6120 544f 4d4c 2066 696c 652e 0a0a 5468  a TOML file...Th
+00005410: 6973 206d 6574 686f 6420 6361 6e20 6265  is method can be
+00005420: 2075 7365 6420 746f 206f 7665 7272 6964   used to overrid
+00005430: 6520 7468 6520 6465 6661 756c 7420 6469  e the default di
+00005440: 7265 6374 6976 6573 2c20 652e 672e 2c20  rectives, e.g., 
+00005450: 7365 7474 696e 6720 602d 7620 7573 6572  setting `-v user
+00005460: 6e61 6d65 3d22 6f74 6865 722d 7573 6572  name="other-user
+00005470: 2260 2077 696c 6c20 6f76 6572 7269 6465  "` will override
+00005480: 2074 6865 2064 6566 6175 6c74 2060 7b7b   the default `{{
+00005490: 7573 6572 6e61 6d65 7d7d 6020 6469 7265  username}}` dire
+000054a0: 6374 6976 652e 0a0a 2323 204e 6573 7465  ctive...## Neste
+000054b0: 6420 5661 7269 6162 6c65 730a 0a49 6e20  d Variables..In 
+000054c0: 7468 6520 6361 7365 206f 6620 2a2a 544f  the case of **TO
+000054d0: 4d4c 2070 726f 7065 7274 6965 7320 6f6e  ML properties on
+000054e0: 6c79 2a2a 2c20 7661 7269 6162 6c65 2073  ly**, variable s
+000054f0: 7562 7374 6974 7574 696f 6e73 2063 616e  ubstitutions can
+00005500: 2062 6520 6e65 7374 6564 2e0a 0a46 6f72   be nested...For
+00005510: 2065 7861 6d70 6c65 2c20 6966 206f 6e65   example, if one
+00005520: 2077 616e 7465 6420 746f 2073 656c 6563   wanted to selec
+00005530: 7420 6120 6469 6666 6572 656e 7420 6074  t a different `t
+00005540: 656d 706c 6174 6549 6460 2066 6f72 2061  emplateId` for a
+00005550: 2057 6f72 6b65 7220 506f 6f6c 2064 6570   Worker Pool dep
+00005560: 656e 6469 6e67 206f 6e20 7468 6520 7661  ending on the va
+00005570: 6c75 6520 6f66 2061 2060 7265 6769 6f6e  lue of a `region
+00005580: 6020 7661 7269 6162 6c65 2c20 6f6e 6520  ` variable, one 
+00005590: 636f 756c 6420 7573 6520 7468 6520 666f  could use the fo
+000055a0: 6c6c 6f77 696e 673a 0a0a 6060 6074 6f6d  llowing:..```tom
+000055b0: 6c0a 5b63 6f6d 6d6f 6e2e 7661 7269 6162  l.[common.variab
+000055c0: 6c65 735d 0a20 2020 2074 656d 706c 6174  les].    templat
+000055d0: 655f 6c6f 6e64 6f6e 203d 2022 7964 6964  e_london = "ydid
+000055e0: 3a63 7274 3a36 3545 4634 463a 6134 6437  :crt:65EF4F:a4d7
+000055f0: 3537 6366 2d62 3637 612d 3465 6236 2d62  57cf-b67a-4eb6-b
+00005600: 6433 392d 3861 3666 6664 3436 6338 6634  d39-8a6ffd46c8f4
+00005610: 220a 2020 2020 7465 6d70 6c61 7465 5f70  ".    template_p
+00005620: 686f 656e 6978 203d 2022 7964 6964 3a63  hoenix = "ydid:c
+00005630: 7274 3a36 3545 4634 463a 6534 3233 3964  rt:65EF4F:e4239d
+00005640: 6563 2d37 3863 322d 3432 3163 2d61 3766  ec-78c2-421c-a7f
+00005650: 332d 3731 6536 3162 3732 3934 3666 220a  3-71e61b72946f".
+00005660: 2020 2020 7465 6d70 6c61 7465 5f66 7261      template_fra
+00005670: 6e6b 6675 7274 203d 2022 7964 6964 3a63  nkfurt = "ydid:c
+00005680: 7274 3a36 3545 4634 463a 3332 3936 3032  rt:65EF4F:329602
+00005690: 6366 2d35 3934 352d 3461 6164 2d61 3238  cf-5945-4aad-a28
+000056a0: 382d 6561 3432 3464 3634 6435 3565 220a  8-ea424d64d55e".
+000056b0: 0a5b 636f 6d6d 6f6e 2e77 6f72 6b65 7250  .[common.workerP
+000056c0: 6f6f 6c5d 0a20 2020 2074 656d 706c 6174  ool].    templat
+000056d0: 6549 6420 3d20 227b 7b74 656d 706c 6174  eId = "{{templat
+000056e0: 655f 7b7b 7265 6769 6f6e 7d7d 7d7d 220a  e_{{region}}}}".
+000056f0: 6060 600a 0a54 6865 6e2c 2069 6620 6f6e  ```..Then, if on
+00005700: 6520 7573 6564 2060 7964 2d70 726f 7669  e used `yd-provi
+00005710: 7369 6f6e 202d 7620 7265 6769 6f6e 3d70  sion -v region=p
+00005720: 686f 656e 6978 602c 2074 6865 2060 7465  hoenix`, the `te
+00005730: 6d70 6c61 7465 4964 6020 7072 6f70 6572  mplateId` proper
+00005740: 7479 2077 6f75 6c64 2066 6972 7374 2072  ty would first r
+00005750: 6573 6f6c 7665 2074 6f20 6022 7b7b 7465  esolve to `"{{te
+00005760: 6d70 6c61 7465 5f70 6865 6f6e 6978 7d7d  mplate_pheonix}}
+00005770: 2260 2c20 616e 6420 7468 656e 2074 6f20  "`, and then to 
+00005780: 6022 7964 6964 3a63 7274 3a36 3545 4634  `"ydid:crt:65EF4
+00005790: 463a 6534 3233 3964 6563 2d37 3863 322d  F:e4239dec-78c2-
+000057a0: 3432 3163 2d61 3766 332d 3731 6536 3162  421c-a7f3-71e61b
+000057b0: 3732 3934 3666 2260 2e0a 0a4e 6573 7469  72946f"`...Nesti
+000057c0: 6e67 2063 616e 2062 6520 7570 2074 6f20  ng can be up to 
+000057d0: 7468 7265 6520 6c65 7665 6c73 2064 6565  three levels dee
+000057e0: 7020 696e 636c 7564 696e 6720 7468 6520  p including the 
+000057f0: 746f 7020 6c65 7665 6c2e 0a0a 2320 576f  top level...# Wo
+00005800: 726b 2052 6571 7569 7265 6d65 6e74 2050  rk Requirement P
+00005810: 726f 7065 7274 6965 730a 0a54 6865 2060  roperties..The `
+00005820: 776f 726b 5265 7175 6972 656d 656e 7460  workRequirement`
+00005830: 2073 6563 7469 6f6e 206f 6620 7468 6520   section of the 
+00005840: 636f 6e66 6967 7572 6174 696f 6e20 6669  configuration fi
+00005850: 6c65 2069 7320 6f70 7469 6f6e 616c 2e20  le is optional. 
+00005860: 4974 2773 2075 7365 6420 6f6e 6c79 2062  It's used only b
+00005870: 7920 7468 6520 6079 642d 7375 626d 6974  y the `yd-submit
+00005880: 6020 636f 6d6d 616e 642c 2061 6e64 2063  ` command, and c
+00005890: 6f6e 7472 6f6c 7320 7468 6520 576f 726b  ontrols the Work
+000058a0: 2052 6571 7569 7265 6d65 6e74 2074 6861   Requirement tha
+000058b0: 7420 6973 2073 7562 6d69 7474 6564 2074  t is submitted t
+000058c0: 6f20 7468 6520 506c 6174 666f 726d 2e0a  o the Platform..
+000058d0: 0a54 6865 2064 6574 6169 6c73 206f 6620  .The details of 
+000058e0: 6120 576f 726b 2052 6571 7569 7265 6d65  a Work Requireme
+000058f0: 6e74 2074 6f20 6265 2073 7562 6d69 7474  nt to be submitt
+00005900: 6564 2063 616e 2062 6520 6361 7074 7572  ed can be captur
+00005910: 6564 2065 6e74 6972 656c 7920 7769 7468  ed entirely with
+00005920: 696e 2074 6865 2054 4f4d 4c20 636f 6e66  in the TOML conf
+00005930: 6967 7572 6174 696f 6e20 6669 6c65 2066  iguration file f
+00005940: 6f72 2073 696d 706c 6520 6578 616d 706c  or simple exampl
+00005950: 6573 2e20 4d6f 7265 2063 6f6d 706c 6578  es. More complex
+00005960: 2065 7861 6d70 6c65 7320 6361 7074 7572   examples captur
+00005970: 6520 7468 6520 576f 726b 2052 6571 7569  e the Work Requi
+00005980: 7265 6d65 6e74 2069 6e20 6120 636f 6d62  rement in a comb
+00005990: 696e 6174 696f 6e20 6f66 2074 6865 2054  ination of the T
+000059a0: 4f4d 4c20 6669 6c65 2070 6c75 7320 6120  OML file plus a 
+000059b0: 4a53 4f4e 2064 6f63 756d 656e 742c 206f  JSON document, o
+000059c0: 7220 696e 2061 204a 534f 4e20 646f 6375  r in a JSON docu
+000059d0: 6d65 6e74 206f 6e6c 792e 0a0a 2323 2057  ment only...## W
+000059e0: 6f72 6b20 5265 7175 6972 656d 656e 7420  ork Requirement 
+000059f0: 4a53 4f4e 2046 696c 6520 5374 7275 6374  JSON File Struct
+00005a00: 7572 650a 0a57 6f72 6b20 5265 7175 6972  ure..Work Requir
+00005a10: 656d 656e 7473 2061 7265 2072 6570 7265  ements are repre
+00005a20: 7365 6e74 6564 2069 6e20 4a53 4f4e 2064  sented in JSON d
+00005a30: 6f63 756d 656e 7473 2075 7369 6e67 2061  ocuments using a
+00005a40: 2063 6f6e 7461 696e 6d65 6e74 2068 6965   containment hie
+00005a50: 7261 7263 6879 206f 6620 6120 2a2a 576f  rarchy of a **Wo
+00005a60: 726b 2052 6571 7569 7265 6d65 6e74 2a2a  rk Requirement**
+00005a70: 2063 6f6e 7461 696e 696e 6720 6120 2a2a   containing a **
+00005a80: 6c69 7374 206f 6620 5461 736b 2047 726f  list of Task Gro
+00005a90: 7570 732a 2a2c 2063 6f6e 7461 696e 696e  ups**, containin
+00005aa0: 6720 6120 2a2a 6c69 7374 206f 6620 5461  g a **list of Ta
+00005ab0: 736b 732a 2a2e 0a0a 4120 7665 7279 2073  sks**...A very s
+00005ac0: 696d 706c 6520 6578 616d 706c 6520 646f  imple example do
+00005ad0: 6375 6d65 6e74 2069 7320 7368 6f77 6e20  cument is shown 
+00005ae0: 6265 6c6f 7720 7769 7468 2061 2074 6f70  below with a top
+00005af0: 2d6c 6576 656c 2057 6f72 6b20 5265 7175  -level Work Requ
+00005b00: 6972 656d 656e 7420 636f 6e74 6169 6e69  irement containi
+00005b10: 6e67 2074 776f 2054 6173 6b20 4772 6f75  ng two Task Grou
+00005b20: 7073 2065 6163 6820 636f 6e74 6169 6e69  ps each containi
+00005b30: 6e67 2074 776f 2054 6173 6b73 2c20 6561  ng two Tasks, ea
+00005b40: 6368 2077 6974 6820 6120 6469 6666 6572  ch with a differ
+00005b50: 656e 7420 7365 7420 6f66 2061 7267 756d  ent set of argum
+00005b60: 656e 7473 2074 6f20 6265 2070 6173 7365  ents to be passe
+00005b70: 6420 746f 2074 6865 2054 6173 6b2e 0a0a  d to the Task...
+00005b80: 6060 606a 736f 6e0a 7b0a 2020 2274 6173  ```json.{.  "tas
+00005b90: 6b47 726f 7570 7322 3a20 5b0a 2020 2020  kGroups": [.    
+00005ba0: 7b0a 2020 2020 2020 2274 6173 6b73 223a  {.      "tasks":
+00005bb0: 205b 0a20 2020 2020 2020 207b 0a20 2020   [.        {.   
+00005bc0: 2020 2020 2020 2022 6172 6775 6d65 6e74         "argument
+00005bd0: 7322 3a20 5b31 2c20 322c 2033 5d0a 2020  s": [1, 2, 3].  
+00005be0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00005bf0: 207b 0a20 2020 2020 2020 2020 2022 6172   {.          "ar
+00005c00: 6775 6d65 6e74 7322 3a20 5b34 2c20 352c  guments": [4, 5,
+00005c10: 2036 5d0a 2020 2020 2020 2020 7d0a 2020   6].        }.  
+00005c20: 2020 2020 5d0a 2020 2020 7d2c 0a20 2020      ].    },.   
+00005c30: 207b 0a20 2020 2020 2022 7461 736b 7322   {.      "tasks"
+00005c40: 3a20 5b0a 2020 2020 2020 2020 7b0a 2020  : [.        {.  
+00005c50: 2020 2020 2020 2020 2261 7267 756d 656e          "argumen
+00005c60: 7473 223a 205b 372c 2038 2c20 395d 0a20  ts": [7, 8, 9]. 
+00005c70: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00005c80: 2020 7b0a 2020 2020 2020 2020 2020 2261    {.          "a
+00005c90: 7267 756d 656e 7473 223a 205b 3130 2c20  rguments": [10, 
+00005ca0: 3131 2c20 3132 5d0a 2020 2020 2020 2020  11, 12].        
+00005cb0: 7d0a 2020 2020 2020 5d0a 2020 2020 7d0a  }.      ].    }.
+00005cc0: 2020 5d0a 7d0a 0a60 6060 0a0a 546f 2073    ].}..```..To s
+00005cd0: 7065 6369 6679 2074 6865 2066 696c 6520  pecify the file 
+00005ce0: 636f 6e74 6169 6e69 6e67 2074 6865 204a  containing the J
+00005cf0: 534f 4e20 646f 6375 6d65 6e74 2c20 6569  SON document, ei
+00005d00: 7468 6572 2070 6f70 756c 6174 6520 7468  ther populate th
+00005d10: 6520 6077 6f72 6b52 6571 7569 7265 6d65  e `workRequireme
+00005d20: 6e74 4461 7461 6020 7072 6f70 6572 7479  ntData` property
+00005d30: 2069 6e20 7468 6520 6077 6f72 6b52 6571   in the `workReq
+00005d40: 7569 7265 6d65 6e74 6020 7365 6374 696f  uirement` sectio
+00005d50: 6e20 6f66 2074 6865 2054 4f4d 4c20 636f  n of the TOML co
+00005d60: 6e66 6967 7572 6174 696f 6e20 6669 6c65  nfiguration file
+00005d70: 2077 6974 6820 7468 6520 4a53 4f4e 2066   with the JSON f
+00005d80: 696c 656e 616d 652c 206f 7220 7370 6563  ilename, or spec
+00005d90: 6966 7920 6974 206f 6e20 7468 6520 636f  ify it on the co
+00005da0: 6d6d 616e 6420 6c69 6e65 2075 7369 6e67  mmand line using
+00005db0: 2074 6865 2060 2d2d 776f 726b 2d72 6571   the `--work-req
+00005dc0: 7569 7265 6d65 6e74 6020 6f72 2060 2d72  uirement` or `-r
+00005dd0: 6020 6f70 7469 6f6e 7320 2877 6869 6368  ` options (which
+00005de0: 2077 696c 6c20 6f76 6572 7269 6465 2074   will override t
+00005df0: 6865 2070 726f 7065 7274 7920 696e 2074  he property in t
+00005e00: 6865 2054 4f4d 4c20 6669 6c65 292c 2065  he TOML file), e
+00005e10: 2e67 2e0a 0a60 7964 2d73 7562 6d69 7420  .g...`yd-submit 
+00005e20: 2d2d 636f 6e66 6967 206d 7963 6f6e 6669  --config myconfi
+00005e30: 672e 746f 6d6c 202d 2d77 6f72 6b2d 7265  g.toml --work-re
+00005e40: 7175 6972 656d 656e 7420 6d79 5f77 6f72  quirement my_wor
+00005e50: 6b72 6571 2e6a 736f 6e60 0a0a 2323 2050  kreq.json`..## P
+00005e60: 726f 7065 7274 7920 496e 6865 7269 7461  roperty Inherita
+00005e70: 6e63 650a 0a54 6f20 7369 6d70 6c69 6679  nce..To simplify
+00005e80: 2074 6865 2064 6566 696e 6974 696f 6e20   the definition 
+00005e90: 6f66 2057 6f72 6b20 5265 7175 6972 656d  of Work Requirem
+00005ea0: 656e 7473 2c20 7468 6572 6520 6973 2061  ents, there is a
+00005eb0: 2070 726f 7065 7274 7920 696e 6865 7269   property inheri
+00005ec0: 7461 6e63 6520 6d65 6368 616e 6973 6d2e  tance mechanism.
+00005ed0: 2050 726f 7065 7274 6965 7320 7468 6174   Properties that
+00005ee0: 2061 7265 2073 6574 2061 7420 6120 6869   are set at a hi
+00005ef0: 6768 6572 206c 6576 656c 2069 6e20 7468  gher level in th
+00005f00: 6520 6869 6572 6172 6368 7920 6172 6520  e hierarchy are 
+00005f10: 696e 6865 7269 7465 6420 6174 206c 6f77  inherited at low
+00005f20: 6572 206c 6576 656c 732c 2075 6e6c 6573  er levels, unles
+00005f30: 7320 6578 706c 6963 6974 6c79 206f 7665  s explicitly ove
+00005f40: 7272 6964 6465 6e2e 0a0a 5468 6973 206d  rridden...This m
+00005f50: 6561 6e73 2074 6861 7420 6120 7072 6f70  eans that a prop
+00005f60: 6572 7479 2073 6574 2069 6e20 7468 6520  erty set in the 
+00005f70: 6077 6f72 6b52 6571 7569 7265 6d65 6e74  `workRequirement
+00005f80: 6020 7365 6374 696f 6e20 6f66 2074 6865  ` section of the
+00005f90: 2054 4f4d 4c20 6669 6c65 2063 616e 2062   TOML file can b
+00005fa0: 6520 696e 6865 7269 7465 6420 7375 6363  e inherited succ
+00005fb0: 6573 7369 7665 6c79 2062 7920 7468 6520  essively by the 
+00005fc0: 576f 726b 2052 6571 7569 7265 6d65 6e74  Work Requirement
+00005fd0: 2c20 5461 736b 2047 726f 7570 7320 616e  , Task Groups an
+00005fe0: 6420 5461 736b 7320 696e 2074 6865 204a  d Tasks in the J
+00005ff0: 534f 4e20 646f 6375 6d65 6e74 2028 6173  SON document (as
+00006000: 7375 6d69 6e67 2074 6865 2070 726f 7065  suming the prope
+00006010: 7274 7920 6973 2076 616c 6964 2061 7420  rty is valid at 
+00006020: 6561 6368 206c 6576 656c 292e 2020 4865  each level).  He
+00006030: 6e63 652c 2054 6173 6b73 2069 6e68 6572  nce, Tasks inher
+00006040: 6974 2066 726f 6d20 5461 736b 2047 726f  it from Task Gro
+00006050: 7570 732c 2077 6869 6368 2069 6e68 6572  ups, which inher
+00006060: 6974 2066 726f 6d20 7468 6520 576f 726b  it from the Work
+00006070: 2052 6571 7569 7265 6d65 6e74 2069 6e20   Requirement in 
+00006080: 7468 6520 4a53 4f4e 2064 6f63 756d 656e  the JSON documen
+00006090: 742c 2077 6869 6368 2069 6e68 6572 6974  t, which inherit
+000060a0: 7320 6672 6f6d 2074 6865 2060 776f 726b  s from the `work
+000060b0: 5265 7175 6972 656d 656e 7460 2070 726f  Requirement` pro
+000060c0: 7065 7274 6965 7320 696e 2074 6865 2054  perties in the T
+000060d0: 4f4d 4c20 6669 6c65 2e0a 0a4f 7665 7272  OML file...Overr
+000060e0: 6964 6465 6e20 7072 6f70 6572 7469 6573  idden properties
+000060f0: 2061 7265 2061 6c73 6f20 696e 6865 7269   are also inheri
+00006100: 7465 642e 2045 2e67 2e2c 2069 6620 6120  ted. E.g., if a 
+00006110: 7072 6f70 6572 7479 2069 7320 7365 7420  property is set 
+00006120: 6174 2074 6865 2054 6173 6b20 4772 6f75  at the Task Grou
+00006130: 7020 6c65 7665 6c2c 2069 7420 7769 6c6c  p level, it will
+00006140: 2062 6520 696e 6865 7269 7465 6420 6279   be inherited by
+00006150: 2074 6865 2054 6173 6b73 2069 6e20 7468   the Tasks in th
+00006160: 6174 2054 6173 6b20 4772 6f75 7020 756e  at Task Group un
+00006170: 6c65 7373 2065 7870 6c69 6369 746c 7920  less explicitly 
+00006180: 6f76 6572 7269 6464 656e 2e0a 0a23 2320  overridden...## 
+00006190: 576f 726b 2052 6571 7569 7265 6d65 6e74  Work Requirement
+000061a0: 2050 726f 7065 7274 7920 4469 6374 696f   Property Dictio
+000061b0: 6e61 7279 0a0a 5468 6520 666f 6c6c 6f77  nary..The follow
+000061c0: 696e 6720 7461 626c 6520 6f75 746c 696e  ing table outlin
+000061d0: 6573 2061 6c6c 2074 6865 2070 726f 7065  es all the prope
+000061e0: 7274 6965 7320 6176 6169 6c61 626c 6520  rties available 
+000061f0: 666f 7220 6465 6669 6e69 6e67 2057 6f72  for defining Wor
+00006200: 6b20 5265 7175 6972 656d 656e 7473 2c20  k Requirements, 
+00006210: 616e 6420 7468 6520 6c65 7665 6c73 2061  and the levels a
+00006220: 7420 7768 6963 6820 7468 6579 2061 7265  t which they are
+00006230: 2061 6c6c 6f77 6564 2074 6f20 6265 2075   allowed to be u
+00006240: 7365 642e 2053 6f2c 2066 6f72 2065 7861  sed. So, for exa
+00006250: 6d70 6c65 2c20 7468 6520 6070 726f 7669  mple, the `provi
+00006260: 6465 7260 2070 726f 7065 7274 7920 6361  der` property ca
+00006270: 6e20 6265 2073 6574 2069 6e20 7468 6520  n be set in the 
+00006280: 544f 4d4c 2066 696c 652c 2061 7420 7468  TOML file, at th
+00006290: 6520 576f 726b 2052 6571 7569 7265 6d65  e Work Requireme
+000062a0: 6e74 204c 6576 656c 206f 7220 6174 2074  nt Level or at t
+000062b0: 6865 2054 6173 6b20 4772 6f75 7020 4c65  he Task Group Le
+000062c0: 7665 6c2c 2062 7574 206e 6f74 2061 7420  vel, but not at 
+000062d0: 7468 6520 5461 736b 206c 6576 656c 2c20  the Task level, 
+000062e0: 616e 6420 7072 6f70 6572 7479 2060 6465  and property `de
+000062f0: 7065 6e64 656e 744f 6e60 2063 616e 206f  pendentOn` can o
+00006300: 6e6c 7920 6265 2073 6574 2061 7420 7468  nly be set at th
+00006310: 6520 5461 736b 2047 726f 7570 206c 6576  e Task Group lev
+00006320: 656c 2e0a 0a41 6c6c 2070 726f 7065 7274  el...All propert
+00006330: 6965 7320 6172 6520 6f70 7469 6f6e 616c  ies are optional
+00006340: 2065 7863 6570 7420 666f 7220 2a2a 6074   except for **`t
+00006350: 6173 6b54 7970 6560 2a2a 2028 6f72 202a  askType`** (or *
+00006360: 2a60 7461 736b 5479 7065 7360 2a2a 292e  *`taskTypes`**).
+00006370: 0a0a 7c20 5072 6f70 6572 7479 204e 616d  ..| Property Nam
+00006380: 6520 2020 2020 2020 2020 2020 2020 207c  e              |
+00006390: 2044 6573 6372 6970 7469 6f6e 2020 2020   Description    
+000063a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006430: 2020 2020 2020 2020 2020 7c20 544f 4d4c            | TOML
+00006440: 207c 2057 5220 207c 2054 4772 7020 7c20   | WR  | TGrp | 
+00006450: 5461 736b 207c 0a7c 3a2d 2d2d 2d2d 2d2d  Task |.|:-------
+00006460: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006470: 2d2d 2d2d 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d  ----|:----------
+00006480: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006490: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000064a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000064b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000064c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000064d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000064e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000064f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006500: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006510: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  ---------------|
+00006520: 3a2d 2d2d 2d2d 7c3a 2d2d 2d2d 7c3a 2d2d  :-----|:----|:--
+00006530: 2d2d 2d7c 3a2d 2d2d 2d2d 7c0a 7c20 6061  ---|:-----|.| `a
+00006540: 7267 756d 656e 7473 6020 2020 2020 2020  rguments`       
+00006550: 2020 2020 2020 2020 207c 2054 6865 206c           | The l
+00006560: 6973 7420 6f66 2061 7267 756d 656e 7473  ist of arguments
+00006570: 2074 6f20 6265 2070 6173 7365 6420 746f   to be passed to
+00006580: 2074 6865 2054 6173 6b20 7768 656e 2069   the Task when i
+00006590: 7420 6973 2065 7865 6375 7465 642e 2045  t is executed. E
+000065a0: 2e67 2e3a 2060 5b31 2c20 2254 776f 225d  .g.: `[1, "Two"]
+000065b0: 602e 2020 2020 2020 2020 2020 2020 2020  `.              
+000065c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000065d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000065e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000065f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006600: 2020 2020 7c20 5965 7320 207c 2059 6573      | Yes  | Yes
+00006610: 207c 2059 6573 2020 7c20 5965 7320 207c   | Yes  | Yes  |
+00006620: 0a7c 2060 6361 7074 7572 6554 6173 6b4f  .| `captureTaskO
+00006630: 7574 7075 7460 2020 2020 2020 2020 7c20  utput`        | 
+00006640: 5768 6574 6865 7220 7468 6520 636f 6e73  Whether the cons
+00006650: 6f6c 6520 6f75 7470 7574 206f 6620 6120  ole output of a 
+00006660: 5461 736b 2773 2070 726f 6365 7373 2073  Task's process s
+00006670: 686f 756c 6420 6265 2075 706c 6f61 6465  hould be uploade
+00006680: 6420 746f 2074 6865 2059 656c 6c6f 7744  d to the YellowD
+00006690: 6f67 204f 626a 6563 7420 5374 6f72 6520  og Object Store 
+000066a0: 6f6e 2054 6173 6b20 636f 6d70 6c65 7469  on Task completi
+000066b0: 6f6e 2e20 4465 6661 756c 743a 2060 7472  on. Default: `tr
+000066c0: 7565 602e 2020 2020 2020 2020 2020 2020  ue`.            
 000066d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000066e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000066f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006710: 2020 207c 2059 6573 2020 7c20 2020 2020     | Yes  |     
-00006720: 7c20 2020 2020 207c 2020 2020 2020 7c0a  |      |      |.
-00006730: 7c20 6064 6570 656e 6465 6e74 4f6e 6020  | `dependentOn` 
-00006740: 2020 2020 2020 2020 2020 2020 207c 2054               | T
-00006750: 6865 206e 616d 6520 6f66 2061 6e6f 7468  he name of anoth
-00006760: 6572 2054 6173 6b20 4772 6f75 7020 7769  er Task Group wi
-00006770: 7468 696e 2074 6865 2073 616d 6520 576f  thin the same Wo
-00006780: 726b 2052 6571 7569 7265 6d65 6e74 2074  rk Requirement t
-00006790: 6861 7420 6d75 7374 2062 6520 7375 6363  hat must be succ
-000067a0: 6573 7366 756c 6c79 2063 6f6d 706c 6574  essfully complet
-000067b0: 6564 2062 6566 6f72 6520 7468 6520 5461  ed before the Ta
-000067c0: 736b 2047 726f 7570 2069 7320 7374 6172  sk Group is star
-000067d0: 7465 642e 2045 2e67 2e20 6022 7461 736b  ted. E.g. `"task
-000067e0: 5f67 726f 7570 5f31 2260 2e20 2020 2020  _group_1"`.     
-000067f0: 2020 2020 2020 2020 7c20 2020 2020 207c          |      |
-00006800: 2020 2020 207c 2059 6573 2020 7c20 2020       | Yes  |   
-00006810: 2020 207c 0a7c 2060 646f 636b 6572 456e     |.| `dockerEn
-00006820: 7669 726f 6e6d 656e 7460 2020 2020 2020  vironment`      
-00006830: 2020 7c20 5468 6520 656e 7669 726f 6e6d    | The environm
-00006840: 656e 7420 746f 2062 6520 7061 7373 6564  ent to be passed
-00006850: 2074 6f20 6120 446f 636b 6572 2063 6f6e   to a Docker con
-00006860: 7461 696e 6572 2e20 4f6e 6c79 2075 7365  tainer. Only use
-00006870: 6420 6279 2074 6865 2060 646f 636b 6572  d by the `docker
-00006880: 6020 5461 736b 2054 7970 652e 2045 2e67  ` Task Type. E.g
-00006890: 2e2c 204a 534f 4e3a 2060 7b22 5641 525f  ., JSON: `{"VAR_
-000068a0: 3122 3a20 2261 6263 227d 602c 2054 4f4d  1": "abc"}`, TOM
-000068b0: 4c3a 2060 7b56 4152 5f31 203d 2022 6162  L: `{VAR_1 = "ab
-000068c0: 6322 2c20 5641 525f 3220 3d20 2264 6566  c", VAR_2 = "def
-000068d0: 227d 602e 2020 2020 2020 2020 207c 2059  "}`.         | Y
-000068e0: 6573 2020 7c20 5965 7320 7c20 5965 7320  es  | Yes | Yes 
-000068f0: 207c 2059 6573 2020 7c0a 7c20 6064 6f63   | Yes  |.| `doc
-00006900: 6b65 7250 6173 7377 6f72 6460 2020 2020  kerPassword`    
-00006910: 2020 2020 2020 207c 2054 6865 2070 6173         | The pas
-00006920: 7377 6f72 6420 666f 7220 446f 636b 6572  sword for Docker
-00006930: 4875 622c 206f 6e6c 7920 7573 6564 2062  Hub, only used b
-00006940: 7920 7468 6520 6064 6f63 6b65 7260 2054  y the `docker` T
-00006950: 6173 6b20 5479 7065 2e20 452c 672e 2c20  ask Type. E,g., 
-00006960: 6022 6d79 5f70 6173 7377 6f72 6422 602e  `"my_password"`.
+000066e0: 2020 2020 2020 2020 207c 2059 6573 2020           | Yes  
+000066f0: 7c20 5965 7320 7c20 5965 7320 207c 2059  | Yes | Yes  | Y
+00006700: 6573 2020 7c0a 7c20 6063 6f6d 706c 6574  es  |.| `complet
+00006710: 6564 5461 736b 5474 6c60 2020 2020 2020  edTaskTtl`      
+00006720: 2020 207c 2054 6865 2074 696d 6520 2869     | The time (i
+00006730: 6e20 6d69 6e75 7465 7329 2074 6f20 6c69  n minutes) to li
+00006740: 7665 2066 6f72 2063 6f6d 706c 6574 6564  ve for completed
+00006750: 2054 6173 6b73 2e20 4966 2073 6574 2c20   Tasks. If set, 
+00006760: 5461 736b 7320 7468 6174 2068 6176 6520  Tasks that have 
+00006770: 6265 656e 2063 6f6d 706c 6574 6564 2066  been completed f
+00006780: 6f72 206c 6f6e 6765 7220 7468 616e 2074  or longer than t
+00006790: 6869 7320 7065 7269 6f64 2077 696c 6c20  his period will 
+000067a0: 6265 2064 656c 6574 6564 2e20 452e 672e  be deleted. E.g.
+000067b0: 3a20 6031 302e 3060 2e20 2020 2020 2020  : `10.0`.       
+000067c0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+000067d0: 5965 7320 207c 2059 6573 207c 2059 6573  Yes  | Yes | Yes
+000067e0: 2020 7c20 2020 2020 207c 0a7c 2060 6373    |      |.| `cs
+000067f0: 7646 696c 6560 2020 2020 2020 2020 2020  vFile`          
+00006800: 2020 2020 2020 2020 7c20 5468 6520 6e61          | The na
+00006810: 6d65 206f 6620 7468 6520 4353 5620 6669  me of the CSV fi
+00006820: 6c65 2075 7365 6420 746f 2064 6572 6976  le used to deriv
+00006830: 6520 5461 736b 2064 6174 612e 2041 6e20  e Task data. An 
+00006840: 616c 7465 726e 6174 6976 6520 746f 2060  alternative to `
+00006850: 6373 7646 696c 6573 6020 7468 6174 2063  csvFiles` that c
+00006860: 616e 2062 6520 7573 6564 2077 6865 6e20  an be used when 
+00006870: 7468 6572 6527 7320 6f6e 6c79 2061 2073  there's only a s
+00006880: 696e 676c 6520 4353 5620 6669 6c65 2e20  ingle CSV file. 
+00006890: 452e 672e 2060 2266 696c 652e 6373 7622  E.g. `"file.csv"
+000068a0: 602e 2020 2020 2020 2020 2020 2020 2020  `.              
+000068b0: 2020 207c 2059 6573 2020 7c20 2020 2020     | Yes  |     
+000068c0: 7c20 2020 2020 207c 2020 2020 2020 7c0a  |      |      |.
+000068d0: 7c20 6063 7376 4669 6c65 7360 2020 2020  | `csvFiles`    
+000068e0: 2020 2020 2020 2020 2020 2020 207c 2041               | A
+000068f0: 206c 6973 7420 6f66 2043 5356 2066 696c   list of CSV fil
+00006900: 6573 2075 7365 6420 746f 2064 6572 6976  es used to deriv
+00006910: 6520 5461 736b 2064 6174 612e 2045 2e67  e Task data. E.g
+00006920: 2e20 605b 2266 696c 652e 6373 7622 2c20  . `["file.csv", 
+00006930: 2266 696c 655f 322e 6373 763a 325d 602e  "file_2.csv:2]`.
+00006940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006960: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006970: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069c0: 2020 7c20 5965 7320 207c 2059 6573 207c    | Yes  | Yes |
-000069d0: 2059 6573 2020 7c20 5965 7320 207c 0a7c   Yes  | Yes  |.|
-000069e0: 2060 646f 636b 6572 5573 6572 6e61 6d65   `dockerUsername
-000069f0: 6020 2020 2020 2020 2020 2020 7c20 5468  `           | Th
-00006a00: 6520 7573 6572 6e61 6d65 2066 6f72 2044  e username for D
-00006a10: 6f63 6b65 7248 7562 2c20 6f6e 6c79 2075  ockerHub, only u
-00006a20: 7365 6420 6279 2074 6865 2060 646f 636b  sed by the `dock
-00006a30: 6572 6020 5461 736b 2054 7970 652e 2045  er` Task Type. E
-00006a40: 2c67 2e2c 2060 226d 795f 7573 6572 6e61  ,g., `"my_userna
-00006a50: 6d65 2260 2e20 2020 2020 2020 2020 2020  me"`.           
-00006a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006aa0: 2020 2020 2020 207c 2059 6573 2020 7c20         | Yes  | 
-00006ab0: 5965 7320 7c20 5965 7320 207c 2059 6573  Yes | Yes  | Yes
-00006ac0: 2020 7c0a 7c20 6065 6e76 6972 6f6e 6d65    |.| `environme
-00006ad0: 6e74 6020 2020 2020 2020 2020 2020 2020  nt`             
-00006ae0: 207c 2054 6865 2065 6e76 6972 6f6e 6d65   | The environme
-00006af0: 6e74 2076 6172 6961 626c 6573 2074 6f20  nt variables to 
-00006b00: 7365 7420 666f 7220 6120 5461 736b 2077  set for a Task w
-00006b10: 6865 6e20 6974 2773 2065 7865 6375 7465  hen it's execute
-00006b20: 642e 2045 2e67 2e2c 204a 534f 4e3a 2060  d. E.g., JSON: `
-00006b30: 7b22 5641 525f 3122 3a20 2261 6263 222c  {"VAR_1": "abc",
-00006b40: 2022 5641 525f 3222 3a20 2264 6566 227d   "VAR_2": "def"}
-00006b50: 602c 2054 4f4d 4c3a 2060 7b56 4152 5f31  `, TOML: `{VAR_1
-00006b60: 203d 2022 6162 6322 2c20 5641 525f 3220   = "abc", VAR_2 
-00006b70: 3d20 2264 6566 227d 602e 2020 2020 2020  = "def"}`.      
-00006b80: 2020 2020 2020 2020 2020 2020 7c20 5965              | Ye
-00006b90: 7320 207c 2059 6573 207c 2059 6573 2020  s  | Yes | Yes  
-00006ba0: 7c20 5965 7320 207c 0a7c 2060 6578 636c  | Yes  |.| `excl
-00006bb0: 7573 6976 6557 6f72 6b65 7273 6020 2020  usiveWorkers`   
-00006bc0: 2020 2020 2020 7c20 4966 2074 7275 652c        | If true,
-00006bd0: 2074 6865 6e20 646f 206e 6f74 2061 6c6c   then do not all
-00006be0: 6f77 2063 6c61 696d 6564 2057 6f72 6b65  ow claimed Worke
-00006bf0: 7273 2074 6f20 6265 2073 6861 7265 6420  rs to be shared 
-00006c00: 7769 7468 206f 7468 6572 2054 6173 6b20  with other Task 
-00006c10: 4772 6f75 7073 3b20 6f74 6865 7277 6973  Groups; otherwis
-00006c20: 652c 2057 6f72 6b65 7273 2063 616e 2062  e, Workers can b
-00006c30: 6520 7368 6172 6564 2e20 4465 6661 756c  e shared. Defaul
-00006c40: 743a 6066 616c 7365 602e 2020 2020 2020  t:`false`.      
-00006c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c70: 207c 2059 6573 2020 7c20 5965 7320 7c20   | Yes  | Yes | 
-00006c80: 5965 7320 207c 2020 2020 2020 7c0a 7c20  Yes  |      |.| 
-00006c90: 6065 7865 6375 7461 626c 6560 2020 2020  `executable`    
-00006ca0: 2020 2020 2020 2020 2020 207c 2054 6865             | The
-00006cb0: 2027 6578 6563 7574 6162 6c65 2720 746f   'executable' to
-00006cc0: 2072 756e 2077 6865 6e20 6120 4261 7368   run when a Bash
-00006cd0: 206f 7220 446f 636b 6572 2054 6173 6b20   or Docker Task 
-00006ce0: 6973 2065 7865 6375 7465 642e 2042 6173  is executed. Bas
-00006cf0: 6820 7363 7269 7074 2066 6f72 2042 6173  h script for Bas
-00006d00: 682c 2063 6f6e 7461 696e 6572 2069 6d61  h, container ima
-00006d10: 6765 2066 6f72 2044 6f63 6b65 722e 204f  ge for Docker. O
-00006d20: 7074 696f 6e61 6c3a 206f 6d69 7420 746f  ptional: omit to
-00006d30: 2073 7570 7072 6573 7320 6175 746f 6d61   suppress automa
-00006d40: 7469 6320 7072 6f63 6573 7369 6e67 2e20  tic processing. 
-00006d50: 2020 2020 2020 7c20 5965 7320 207c 2059        | Yes  | Y
-00006d60: 6573 207c 2059 6573 2020 7c20 5965 7320  es | Yes  | Yes 
-00006d70: 207c 0a7c 2060 6669 6e69 7368 4966 416c   |.| `finishIfAl
-00006d80: 6c54 6173 6b73 4669 6e69 7368 6564 6020  lTasksFinished` 
-00006d90: 7c20 4966 2074 7275 652c 2074 6865 2054  | If true, the T
-00006da0: 6173 6b20 4772 6f75 7020 7769 6c6c 2066  ask Group will f
-00006db0: 696e 6973 6820 6175 746f 6d61 7469 6361  inish automatica
-00006dc0: 6c6c 7920 6966 2061 6c6c 2063 6f6e 7461  lly if all conta
-00006dd0: 696e 6564 2074 6173 6b73 2066 696e 6973  ined tasks finis
-00006de0: 682e 2044 6566 6175 6c74 3a60 7472 7565  h. Default:`true
-00006df0: 602e 2020 2020 2020 2020 2020 2020 2020  `.              
+00006990: 2020 2020 2020 2020 7c20 5965 7320 207c          | Yes  |
+000069a0: 2020 2020 207c 2020 2020 2020 7c20 2020       |      |   
+000069b0: 2020 207c 0a7c 2060 6465 7065 6e64 656e     |.| `dependen
+000069c0: 744f 6e60 2020 2020 2020 2020 2020 2020  tOn`            
+000069d0: 2020 7c20 5468 6520 6e61 6d65 206f 6620    | The name of 
+000069e0: 616e 6f74 6865 7220 5461 736b 2047 726f  another Task Gro
+000069f0: 7570 2077 6974 6869 6e20 7468 6520 7361  up within the sa
+00006a00: 6d65 2057 6f72 6b20 5265 7175 6972 656d  me Work Requirem
+00006a10: 656e 7420 7468 6174 206d 7573 7420 6265  ent that must be
+00006a20: 2073 7563 6365 7373 6675 6c6c 7920 636f   successfully co
+00006a30: 6d70 6c65 7465 6420 6265 666f 7265 2074  mpleted before t
+00006a40: 6865 2054 6173 6b20 4772 6f75 7020 6973  he Task Group is
+00006a50: 2073 7461 7274 6564 2e20 452e 672e 2060   started. E.g. `
+00006a60: 2274 6173 6b5f 6772 6f75 705f 3122 602e  "task_group_1"`.
+00006a70: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+00006a80: 2020 2020 7c20 2020 2020 7c20 5965 7320      |     | Yes 
+00006a90: 207c 2020 2020 2020 7c0a 7c20 6064 6f63   |      |.| `doc
+00006aa0: 6b65 7245 6e76 6972 6f6e 6d65 6e74 6020  kerEnvironment` 
+00006ab0: 2020 2020 2020 207c 2054 6865 2065 6e76         | The env
+00006ac0: 6972 6f6e 6d65 6e74 2074 6f20 6265 2070  ironment to be p
+00006ad0: 6173 7365 6420 746f 2061 2044 6f63 6b65  assed to a Docke
+00006ae0: 7220 636f 6e74 6169 6e65 722e 204f 6e6c  r container. Onl
+00006af0: 7920 7573 6564 2062 7920 7468 6520 6064  y used by the `d
+00006b00: 6f63 6b65 7260 2054 6173 6b20 5479 7065  ocker` Task Type
+00006b10: 2e20 452e 672e 2c20 4a53 4f4e 3a20 607b  . E.g., JSON: `{
+00006b20: 2256 4152 5f31 223a 2022 6162 6322 7d60  "VAR_1": "abc"}`
+00006b30: 2c20 544f 4d4c 3a20 607b 5641 525f 3120  , TOML: `{VAR_1 
+00006b40: 3d20 2261 6263 222c 2056 4152 5f32 203d  = "abc", VAR_2 =
+00006b50: 2022 6465 6622 7d60 2e20 2020 2020 2020   "def"}`.       
+00006b60: 2020 7c20 5965 7320 207c 2059 6573 207c    | Yes  | Yes |
+00006b70: 2059 6573 2020 7c20 5965 7320 207c 0a7c   Yes  | Yes  |.|
+00006b80: 2060 646f 636b 6572 5061 7373 776f 7264   `dockerPassword
+00006b90: 6020 2020 2020 2020 2020 2020 7c20 5468  `           | Th
+00006ba0: 6520 7061 7373 776f 7264 2066 6f72 2044  e password for D
+00006bb0: 6f63 6b65 7248 7562 2c20 6f6e 6c79 2075  ockerHub, only u
+00006bc0: 7365 6420 6279 2074 6865 2060 646f 636b  sed by the `dock
+00006bd0: 6572 6020 5461 736b 2054 7970 652e 2045  er` Task Type. E
+00006be0: 2c67 2e2c 2060 226d 795f 7061 7373 776f  ,g., `"my_passwo
+00006bf0: 7264 2260 2e20 2020 2020 2020 2020 2020  rd"`.           
+00006c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c40: 2020 2020 2020 207c 2059 6573 2020 7c20         | Yes  | 
+00006c50: 5965 7320 7c20 5965 7320 207c 2059 6573  Yes | Yes  | Yes
+00006c60: 2020 7c0a 7c20 6064 6f63 6b65 7255 7365    |.| `dockerUse
+00006c70: 726e 616d 6560 2020 2020 2020 2020 2020  rname`          
+00006c80: 207c 2054 6865 2075 7365 726e 616d 6520   | The username 
+00006c90: 666f 7220 446f 636b 6572 4875 622c 206f  for DockerHub, o
+00006ca0: 6e6c 7920 7573 6564 2062 7920 7468 6520  nly used by the 
+00006cb0: 6064 6f63 6b65 7260 2054 6173 6b20 5479  `docker` Task Ty
+00006cc0: 7065 2e20 452c 672e 2c20 6022 6d79 5f75  pe. E,g., `"my_u
+00006cd0: 7365 726e 616d 6522 602e 2020 2020 2020  sername"`.      
+00006ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d20: 2020 2020 2020 2020 2020 2020 7c20 5965              | Ye
+00006d30: 7320 207c 2059 6573 207c 2059 6573 2020  s  | Yes | Yes  
+00006d40: 7c20 5965 7320 207c 0a7c 2060 656e 7669  | Yes  |.| `envi
+00006d50: 726f 6e6d 656e 7460 2020 2020 2020 2020  ronment`        
+00006d60: 2020 2020 2020 7c20 5468 6520 656e 7669        | The envi
+00006d70: 726f 6e6d 656e 7420 7661 7269 6162 6c65  ronment variable
+00006d80: 7320 746f 2073 6574 2066 6f72 2061 2054  s to set for a T
+00006d90: 6173 6b20 7768 656e 2069 7427 7320 6578  ask when it's ex
+00006da0: 6563 7574 6564 2e20 452e 672e 2c20 4a53  ecuted. E.g., JS
+00006db0: 4f4e 3a20 607b 2256 4152 5f31 223a 2022  ON: `{"VAR_1": "
+00006dc0: 6162 6322 2c20 2256 4152 5f32 223a 2022  abc", "VAR_2": "
+00006dd0: 6465 6622 7d60 2c20 544f 4d4c 3a20 607b  def"}`, TOML: `{
+00006de0: 5641 525f 3120 3d20 2261 6263 222c 2056  VAR_1 = "abc", V
+00006df0: 4152 5f32 203d 2022 6465 6622 7d60 2e20  AR_2 = "def"}`. 
 00006e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e30: 2020 2020 2020 2020 2020 207c 2059 6573             | Yes
-00006e40: 2020 7c20 5965 7320 7c20 5965 7320 207c    | Yes | Yes  |
-00006e50: 2020 2020 2020 7c0a 7c20 6066 696e 6973        |.| `finis
-00006e60: 6849 6641 6e79 5461 736b 4661 696c 6564  hIfAnyTaskFailed
-00006e70: 6020 2020 207c 2049 6620 7472 7565 2c20  `    | If true, 
-00006e80: 7468 6520 5461 736b 2047 726f 7570 2077  the Task Group w
-00006e90: 696c 6c20 6265 2066 6169 6c65 6420 6175  ill be failed au
-00006ea0: 746f 6d61 7469 6361 6c6c 7920 6966 2061  tomatically if a
-00006eb0: 6e79 2063 6f6e 7461 696e 6564 2074 6173  ny contained tas
-00006ec0: 6b73 2066 6169 6c2e 2044 6566 6175 6c74  ks fail. Default
-00006ed0: 3a60 6661 6c73 6560 2e20 2020 2020 2020  :`false`.       
+00006e10: 207c 2059 6573 2020 7c20 5965 7320 7c20   | Yes  | Yes | 
+00006e20: 5965 7320 207c 2059 6573 2020 7c0a 7c20  Yes  | Yes  |.| 
+00006e30: 6065 7863 6c75 7369 7665 576f 726b 6572  `exclusiveWorker
+00006e40: 7360 2020 2020 2020 2020 207c 2049 6620  s`         | If 
+00006e50: 7472 7565 2c20 7468 656e 2064 6f20 6e6f  true, then do no
+00006e60: 7420 616c 6c6f 7720 636c 6169 6d65 6420  t allow claimed 
+00006e70: 576f 726b 6572 7320 746f 2062 6520 7368  Workers to be sh
+00006e80: 6172 6564 2077 6974 6820 6f74 6865 7220  ared with other 
+00006e90: 5461 736b 2047 726f 7570 733b 206f 7468  Task Groups; oth
+00006ea0: 6572 7769 7365 2c20 576f 726b 6572 7320  erwise, Workers 
+00006eb0: 6361 6e20 6265 2073 6861 7265 642e 2044  can be shared. D
+00006ec0: 6566 6175 6c74 3a60 6661 6c73 6560 2e20  efault:`false`. 
+00006ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f20: 7c20 5965 7320 207c 2059 6573 207c 2059  | Yes  | Yes | Y
-00006f30: 6573 2020 7c20 2020 2020 207c 0a7c 2060  es  |      |.| `
-00006f40: 666c 6174 7465 6e49 6e70 7574 5061 7468  flattenInputPath
-00006f50: 7360 2020 2020 2020 2020 7c20 4465 7465  s`        | Dete
-00006f60: 726d 696e 6573 2077 6865 7468 6572 2069  rmines whether i
-00006f70: 6e70 7574 206f 626a 6563 7420 7061 7468  nput object path
-00006f80: 7320 7368 6f75 6c64 2062 6520 666c 6174  s should be flat
-00006f90: 7465 6e65 6420 2869 2e65 2e2c 2064 6972  tened (i.e., dir
-00006fa0: 6563 746f 7279 2073 7472 7563 7475 7265  ectory structure
-00006fb0: 2072 656d 6f76 6564 2920 7768 656e 2064   removed) when d
-00006fc0: 6f77 6e6c 6f61 6465 6420 746f 2061 206e  ownloaded to a n
-00006fd0: 6f64 652e 2044 6566 6175 6c74 3a20 6066  ode. Default: `f
-00006fe0: 616c 7365 602e 2020 2020 2020 2020 2020  alse`.          
-00006ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007000: 2020 2020 207c 2059 6573 2020 7c20 5965       | Yes  | Ye
-00007010: 7320 7c20 5965 7320 207c 2059 6573 2020  s | Yes  | Yes  
-00007020: 7c0a 7c20 6066 6c61 7474 656e 5570 6c6f  |.| `flattenUplo
-00007030: 6164 5061 7468 7360 2020 2020 2020 207c  adPaths`       |
-00007040: 2049 676e 6f72 6520 6c6f 6361 6c20 6469   Ignore local di
-00007050: 7265 6374 6f72 7920 7061 7468 7320 7768  rectory paths wh
-00007060: 656e 2075 706c 6f61 6469 6e67 2066 696c  en uploading fil
-00007070: 6573 2074 6f20 7468 6520 4f62 6a65 6374  es to the Object
-00007080: 2053 746f 7265 3b20 706c 6163 6520 696e   Store; place in
-00007090: 2060 3c6e 616d 6573 7061 6365 3e3a 3c77   `<namespace>:<w
-000070a0: 6f72 6b2d 7265 712d 6e61 6d65 3e2f 602e  ork-req-name>/`.
-000070b0: 2044 6566 6175 6c74 3a20 6066 616c 7365   Default: `false
-000070c0: 602e 2020 2020 2020 2020 2020 2020 2020  `.              
-000070d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070e0: 2020 2020 2020 2020 2020 7c20 5965 7320            | Yes 
-000070f0: 207c 2059 6573 207c 2020 2020 2020 7c20   | Yes |      | 
-00007100: 2020 2020 207c 0a7c 2060 6675 6c66 696c       |.| `fulfil
-00007110: 4f6e 5375 626d 6974 6020 2020 2020 2020  OnSubmit`       
-00007120: 2020 2020 7c20 496e 6469 6361 7465 7320      | Indicates 
-00007130: 6966 2074 6865 2057 6f72 6b20 5265 7175  if the Work Requ
-00007140: 6972 656d 656e 7420 7368 6f75 6c64 2062  irement should b
-00007150: 6520 6675 6c66 696c 6c65 6420 7768 656e  e fulfilled when
-00007160: 2069 7420 6973 2073 7562 6d69 7474 6564   it is submitted
-00007170: 2c20 7261 7468 6572 2074 6861 6e20 6265  , rather than be
-00007180: 696e 6720 616c 6c6f 7765 6420 746f 2077  ing allowed to w
-00007190: 6169 7420 696e 2050 454e 4449 4e47 2073  ait in PENDING s
-000071a0: 7461 7475 732e 2044 6566 6175 6c74 3a60  tatus. Default:`
-000071b0: 6661 6c73 6560 2e20 2020 2020 2020 2020  false`.         
-000071c0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-000071d0: 2059 6573 2020 7c20 5965 7320 7c20 2020   Yes  | Yes |   
-000071e0: 2020 207c 2020 2020 2020 7c0a 7c20 6069     |      |.| `i
-000071f0: 6e70 7574 7360 2020 2020 2020 2020 2020  nputs`          
-00007200: 2020 2020 2020 2020 207c 2054 6865 206c           | The l
-00007210: 6973 7420 6f66 2069 6e70 7574 2066 696c  ist of input fil
-00007220: 6573 2074 6f20 6265 2075 706c 6f61 6465  es to be uploade
-00007230: 6420 746f 2074 6865 2059 656c 6c6f 7744  d to the YellowD
-00007240: 6f67 204f 626a 6563 7420 5374 6f72 652c  og Object Store,
-00007250: 2061 6e64 2072 6571 7569 7265 6420 6279   and required by
-00007260: 2074 6865 2054 6173 6b20 2869 6d70 6c69   the Task (impli
-00007270: 6573 2060 7665 7269 6679 4174 5374 6172  es `verifyAtStar
-00007280: 7460 292e 2045 2e67 2e20 605b 2261 2e73  t`). E.g. `["a.s
-00007290: 6822 2c20 2262 2e73 6822 5d60 2e20 2020  h", "b.sh"]`.   
-000072a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000072b0: 2020 2020 7c20 5965 7320 207c 2059 6573      | Yes  | Yes
-000072c0: 207c 2059 6573 2020 7c20 5965 7320 207c   | Yes  | Yes  |
-000072d0: 0a7c 2060 696e 7075 7473 4f70 7469 6f6e  .| `inputsOption
-000072e0: 616c 6020 2020 2020 2020 2020 2020 7c20  al`           | 
-000072f0: 4120 6c69 7374 206f 6620 696e 7075 7420  A list of input 
-00007300: 6669 6c65 7320 7265 7175 6972 6564 2062  files required b
-00007310: 7920 6120 5461 736b 2c20 6275 7420 7768  y a Task, but wh
-00007320: 6963 6820 6172 6520 6e6f 7420 7375 626a  ich are not subj
-00007330: 6563 7420 746f 2076 6572 6966 6963 6174  ect to verificat
-00007340: 696f 6e2e 2043 616e 2063 6f6e 7461 696e  ion. Can contain
-00007350: 2077 696c 6463 6172 6473 2e20 452e 672e   wildcards. E.g.
-00007360: 3a20 605b 2274 6173 6b5f 6772 6f75 705f  : `["task_group_
-00007370: 312f 2a2a 2f72 6573 756c 7473 2e74 7874  1/**/results.txt
-00007380: 225d 602e 2020 2020 2020 2020 2020 2020  "]`.            
-00007390: 2020 2020 2020 2020 207c 2059 6573 2020           | Yes  
-000073a0: 7c20 5965 7320 7c20 5965 7320 207c 2059  | Yes | Yes  | Y
-000073b0: 6573 2020 7c0a 7c20 6069 6e73 7461 6e63  es  |.| `instanc
-000073c0: 6554 7970 6573 6020 2020 2020 2020 2020  eTypes`         
-000073d0: 2020 207c 2054 6865 206d 6163 6869 6e65     | The machine
-000073e0: 2069 6e73 7461 6e63 6520 7479 7065 7320   instance types 
-000073f0: 7468 6174 2063 616e 2062 6520 7573 6564  that can be used
-00007400: 2074 6f20 6578 6563 7574 6520 5461 736b   to execute Task
-00007410: 732e 2045 2e67 2e2c 2060 5b22 7433 2e6d  s. E.g., `["t3.m
-00007420: 6963 726f 222c 2022 7433 612e 6d69 6372  icro", "t3a.micr
-00007430: 6f22 5d60 2e20 2020 2020 2020 2020 2020  o"]`.           
+00006ef0: 2020 2020 2020 7c20 5965 7320 207c 2059        | Yes  | Y
+00006f00: 6573 207c 2059 6573 2020 7c20 2020 2020  es | Yes  |     
+00006f10: 207c 0a7c 2060 6578 6563 7574 6162 6c65   |.| `executable
+00006f20: 6020 2020 2020 2020 2020 2020 2020 2020  `               
+00006f30: 7c20 5468 6520 2765 7865 6375 7461 626c  | The 'executabl
+00006f40: 6527 2074 6f20 7275 6e20 7768 656e 2061  e' to run when a
+00006f50: 2042 6173 6820 6f72 2044 6f63 6b65 7220   Bash or Docker 
+00006f60: 5461 736b 2069 7320 6578 6563 7574 6564  Task is executed
+00006f70: 2e20 4261 7368 2073 6372 6970 7420 666f  . Bash script fo
+00006f80: 7220 4261 7368 2c20 636f 6e74 6169 6e65  r Bash, containe
+00006f90: 7220 696d 6167 6520 666f 7220 446f 636b  r image for Dock
+00006fa0: 6572 2e20 4f70 7469 6f6e 616c 3a20 6f6d  er. Optional: om
+00006fb0: 6974 2074 6f20 7375 7070 7265 7373 2061  it to suppress a
+00006fc0: 7574 6f6d 6174 6963 2070 726f 6365 7373  utomatic process
+00006fd0: 696e 672e 2020 2020 2020 207c 2059 6573  ing.       | Yes
+00006fe0: 2020 7c20 5965 7320 7c20 5965 7320 207c    | Yes | Yes  |
+00006ff0: 2059 6573 2020 7c0a 7c20 6066 696e 6973   Yes  |.| `finis
+00007000: 6849 6641 6c6c 5461 736b 7346 696e 6973  hIfAllTasksFinis
+00007010: 6865 6460 207c 2049 6620 7472 7565 2c20  hed` | If true, 
+00007020: 7468 6520 5461 736b 2047 726f 7570 2077  the Task Group w
+00007030: 696c 6c20 6669 6e69 7368 2061 7574 6f6d  ill finish autom
+00007040: 6174 6963 616c 6c79 2069 6620 616c 6c20  atically if all 
+00007050: 636f 6e74 6169 6e65 6420 7461 736b 7320  contained tasks 
+00007060: 6669 6e69 7368 2e20 4465 6661 756c 743a  finish. Default:
+00007070: 6074 7275 6560 2e20 2020 2020 2020 2020  `true`.         
+00007080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000070a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000070b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000070c0: 7c20 5965 7320 207c 2059 6573 207c 2059  | Yes  | Yes | Y
+000070d0: 6573 2020 7c20 2020 2020 207c 0a7c 2060  es  |      |.| `
+000070e0: 6669 6e69 7368 4966 416e 7954 6173 6b46  finishIfAnyTaskF
+000070f0: 6169 6c65 6460 2020 2020 7c20 4966 2074  ailed`    | If t
+00007100: 7275 652c 2074 6865 2054 6173 6b20 4772  rue, the Task Gr
+00007110: 6f75 7020 7769 6c6c 2062 6520 6661 696c  oup will be fail
+00007120: 6564 2061 7574 6f6d 6174 6963 616c 6c79  ed automatically
+00007130: 2069 6620 616e 7920 636f 6e74 6169 6e65   if any containe
+00007140: 6420 7461 736b 7320 6661 696c 2e20 4465  d tasks fail. De
+00007150: 6661 756c 743a 6066 616c 7365 602e 2020  fault:`false`.  
+00007160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000071a0: 2020 2020 207c 2059 6573 2020 7c20 5965       | Yes  | Ye
+000071b0: 7320 7c20 5965 7320 207c 2020 2020 2020  s | Yes  |      
+000071c0: 7c0a 7c20 6066 6c61 7474 656e 496e 7075  |.| `flattenInpu
+000071d0: 7450 6174 6873 6020 2020 2020 2020 207c  tPaths`        |
+000071e0: 2044 6574 6572 6d69 6e65 7320 7768 6574   Determines whet
+000071f0: 6865 7220 696e 7075 7420 6f62 6a65 6374  her input object
+00007200: 2070 6174 6873 2073 686f 756c 6420 6265   paths should be
+00007210: 2066 6c61 7474 656e 6564 2028 692e 652e   flattened (i.e.
+00007220: 2c20 6469 7265 6374 6f72 7920 7374 7275  , directory stru
+00007230: 6374 7572 6520 7265 6d6f 7665 6429 2077  cture removed) w
+00007240: 6865 6e20 646f 776e 6c6f 6164 6564 2074  hen downloaded t
+00007250: 6f20 6120 6e6f 6465 2e20 4465 6661 756c  o a node. Defaul
+00007260: 743a 2060 6661 6c73 6560 2e20 2020 2020  t: `false`.     
+00007270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007280: 2020 2020 2020 2020 2020 7c20 5965 7320            | Yes 
+00007290: 207c 2059 6573 207c 2059 6573 2020 7c20   | Yes | Yes  | 
+000072a0: 5965 7320 207c 0a7c 2060 666c 6174 7465  Yes  |.| `flatte
+000072b0: 6e55 706c 6f61 6450 6174 6873 6020 2020  nUploadPaths`   
+000072c0: 2020 2020 7c20 4967 6e6f 7265 206c 6f63      | Ignore loc
+000072d0: 616c 2064 6972 6563 746f 7279 2070 6174  al directory pat
+000072e0: 6873 2077 6865 6e20 7570 6c6f 6164 696e  hs when uploadin
+000072f0: 6720 6669 6c65 7320 746f 2074 6865 204f  g files to the O
+00007300: 626a 6563 7420 5374 6f72 653b 2070 6c61  bject Store; pla
+00007310: 6365 2069 6e20 603c 6e61 6d65 7370 6163  ce in `<namespac
+00007320: 653e 3a3c 776f 726b 2d72 6571 2d6e 616d  e>:<work-req-nam
+00007330: 653e 2f60 2e20 4465 6661 756c 743a 2060  e>/`. Default: `
+00007340: 6661 6c73 6560 2e20 2020 2020 2020 2020  false`.         
+00007350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007360: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00007370: 2059 6573 2020 7c20 5965 7320 7c20 2020   Yes  | Yes |   
+00007380: 2020 207c 2020 2020 2020 7c0a 7c20 6066     |      |.| `f
+00007390: 756c 6669 6c4f 6e53 7562 6d69 7460 2020  ulfilOnSubmit`  
+000073a0: 2020 2020 2020 2020 207c 2049 6e64 6963           | Indic
+000073b0: 6174 6573 2069 6620 7468 6520 576f 726b  ates if the Work
+000073c0: 2052 6571 7569 7265 6d65 6e74 2073 686f   Requirement sho
+000073d0: 756c 6420 6265 2066 756c 6669 6c6c 6564  uld be fulfilled
+000073e0: 2077 6865 6e20 6974 2069 7320 7375 626d   when it is subm
+000073f0: 6974 7465 642c 2072 6174 6865 7220 7468  itted, rather th
+00007400: 616e 2062 6569 6e67 2061 6c6c 6f77 6564  an being allowed
+00007410: 2074 6f20 7761 6974 2069 6e20 5045 4e44   to wait in PEND
+00007420: 494e 4720 7374 6174 7573 2e20 4465 6661  ING status. Defa
+00007430: 756c 743a 6066 616c 7365 602e 2020 2020  ult:`false`.    
 00007440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007470: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00007480: 5965 7320 207c 2059 6573 207c 2059 6573  Yes  | Yes | Yes
-00007490: 2020 7c20 2020 2020 207c 0a7c 2060 6d61    |      |.| `ma
-000074a0: 7869 6d75 6d54 6173 6b52 6574 7269 6573  ximumTaskRetries
-000074b0: 6020 2020 2020 2020 7c20 5468 6520 6d61  `       | The ma
-000074c0: 7869 6d75 6d20 6e75 6d62 6572 206f 6620  ximum number of 
-000074d0: 7469 6d65 7320 6120 5461 736b 2063 616e  times a Task can
-000074e0: 2062 6520 7265 7472 6965 6420 6166 7465   be retried afte
-000074f0: 7220 6974 2068 6173 2066 6169 6c65 642e  r it has failed.
-00007500: 2045 2e67 2e3a 2060 3560 2e20 2020 2020   E.g.: `5`.     
-00007510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007560: 2020 207c 2059 6573 2020 7c20 5965 7320     | Yes  | Yes 
-00007570: 7c20 5965 7320 207c 2020 2020 2020 7c0a  | Yes  |      |.
-00007580: 7c20 606d 6178 576f 726b 6572 7360 2020  | `maxWorkers`  
-00007590: 2020 2020 2020 2020 2020 2020 207c 2054               | T
-000075a0: 6865 206d 6178 696d 756d 206e 756d 6265  he maximum numbe
-000075b0: 7220 6f66 2057 6f72 6b65 7273 2074 6861  r of Workers tha
-000075c0: 7420 6361 6e20 6265 2063 6c61 696d 6564  t can be claimed
-000075d0: 2066 6f72 2074 6865 2061 7373 6f63 6961   for the associa
-000075e0: 7465 6420 5461 736b 2047 726f 7570 2e20  ted Task Group. 
-000075f0: 452e 672e 2c20 6031 3060 2e20 2020 2020  E.g., `10`.     
-00007600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007640: 2020 2020 2020 2020 7c20 5965 7320 207c          | Yes  |
-00007650: 2059 6573 207c 2059 6573 2020 7c20 2020   Yes | Yes  |   
-00007660: 2020 207c 0a7c 2060 6d69 6e57 6f72 6b65     |.| `minWorke
-00007670: 7273 6020 2020 2020 2020 2020 2020 2020  rs`             
-00007680: 2020 7c20 5468 6520 6d69 6e69 6d75 6d20    | The minimum 
-00007690: 6e75 6d62 6572 206f 6620 576f 726b 6572  number of Worker
-000076a0: 7320 7468 6174 2074 6865 2061 7373 6f63  s that the assoc
-000076b0: 6961 7465 6420 5461 736b 2047 726f 7570  iated Task Group
-000076c0: 2072 6571 7569 7265 732e 2054 6869 7320   requires. This 
-000076d0: 6d61 6e79 2077 6f72 6b65 7273 206d 7573  many workers mus
-000076e0: 7420 6265 2063 6c61 696d 6564 2062 6566  t be claimed bef
-000076f0: 6f72 6520 7468 6520 6173 736f 6369 6174  ore the associat
-00007700: 6564 2054 6173 6b20 4772 6f75 7020 7769  ed Task Group wi
-00007710: 6c6c 2073 7461 7274 2077 6f72 6b69 6e67  ll start working
-00007720: 2e20 452e 672e 2c20 6031 602e 207c 2059  . E.g., `1`. | Y
-00007730: 6573 2020 7c20 5965 7320 7c20 5965 7320  es  | Yes | Yes 
-00007740: 207c 2020 2020 2020 7c0a 7c20 606e 616d   |      |.| `nam
-00007750: 6560 2020 2020 2020 2020 2020 2020 2020  e`              
-00007760: 2020 2020 2020 207c 2054 6865 206e 616d         | The nam
-00007770: 6520 6f66 2074 6865 2057 6f72 6b20 5265  e of the Work Re
-00007780: 7175 6972 656d 656e 742c 2054 6173 6b20  quirement, Task 
-00007790: 4772 6f75 7020 6f72 2054 6173 6b2e 2045  Group or Task. E
-000077a0: 2e67 2e2c 2060 2277 725f 6e61 6d65 2260  .g., `"wr_name"`
-000077b0: 2e20 4e6f 7465 2074 6861 7420 7468 6520  . Note that the 
-000077c0: 606e 616d 6560 2070 726f 7065 7274 7920  `name` property 
-000077d0: 6973 206e 6f74 2069 6e68 6572 6974 6564  is not inherited
-000077e0: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
-000077f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007810: 2020 7c20 5965 7320 207c 2059 6573 207c    | Yes  | Yes |
-00007820: 2059 6573 2020 7c20 5965 7320 207c 0a7c   Yes  | Yes  |.|
-00007830: 2060 6f75 7470 7574 7360 2020 2020 2020   `outputs`      
-00007840: 2020 2020 2020 2020 2020 2020 7c20 5468              | Th
-00007850: 6520 6669 6c65 7320 746f 2062 6520 7570  e files to be up
-00007860: 6c6f 6164 6564 2074 6f20 7468 6520 5965  loaded to the Ye
-00007870: 6c6c 6f77 446f 6720 4f62 6a65 6374 2053  llowDog Object S
-00007880: 746f 7265 2062 7920 6120 576f 726b 6572  tore by a Worker
-00007890: 206e 6f64 6520 6f6e 2063 6f6d 706c 6574   node on complet
-000078a0: 696f 6e20 6f66 2074 6865 2054 6173 6b2e  ion of the Task.
-000078b0: 2045 2e67 2e2c 2060 5b22 7265 7375 6c74   E.g., `["result
-000078c0: 735f 312e 7478 7422 2c20 2272 6573 756c  s_1.txt", "resul
-000078d0: 7473 5f32 2e74 7874 225d 602e 2020 2020  ts_2.txt"]`.    
-000078e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078f0: 2020 2020 2020 207c 2059 6573 2020 7c20         | Yes  | 
-00007900: 5965 7320 7c20 5965 7320 207c 2059 6573  Yes | Yes  | Yes
-00007910: 2020 7c0a 7c20 606f 7574 7075 7473 5265    |.| `outputsRe
-00007920: 7175 6972 6564 6020 2020 2020 2020 2020  quired`         
-00007930: 207c 2054 6865 2066 696c 6573 2074 6861   | The files tha
-00007940: 7420 2a6d 7573 742a 2062 6520 7570 6c6f  t *must* be uplo
-00007950: 6164 6564 2074 6f20 7468 6520 5965 6c6c  aded to the Yell
-00007960: 6f77 446f 6720 4f62 6a65 6374 2053 746f  owDog Object Sto
-00007970: 7265 2062 7920 6120 576f 726b 6572 206e  re by a Worker n
-00007980: 6f64 6520 6f6e 2063 6f6d 706c 6574 696f  ode on completio
-00007990: 6e20 6f66 2074 6865 2054 6173 6b2e 2054  n of the Task. T
-000079a0: 6865 2054 6173 6b20 7769 6c6c 2066 6169  he Task will fai
-000079b0: 6c20 6966 2061 6e79 206f 7574 7075 7473  l if any outputs
-000079c0: 2061 7265 2075 6e61 7661 696c 6162 6c65   are unavailable
-000079d0: 2e20 2020 2020 2020 2020 2020 7c20 5965  .           | Ye
-000079e0: 7320 207c 2059 6573 207c 2059 6573 2020  s  | Yes | Yes  
-000079f0: 7c20 5965 7320 207c 0a7c 2060 7072 696f  | Yes  |.| `prio
-00007a00: 7269 7479 6020 2020 2020 2020 2020 2020  rity`           
-00007a10: 2020 2020 2020 7c20 5468 6520 7072 696f        | The prio
-00007a20: 7269 7479 206f 6620 576f 726b 2052 6571  rity of Work Req
-00007a30: 7569 7265 6d65 6e74 7320 616e 6420 5461  uirements and Ta
-00007a40: 736b 2047 726f 7570 732e 2048 6967 6865  sk Groups. Highe
-00007a50: 7220 7072 696f 7269 7479 2061 6371 7569  r priority acqui
-00007a60: 7265 7320 576f 726b 6572 7320 6168 6561  res Workers ahea
-00007a70: 6420 6f66 206c 6f77 6572 2070 7269 6f72  d of lower prior
-00007a80: 6974 792e 2045 2e67 2e2c 2060 302e 3060  ity. E.g., `0.0`
-00007a90: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
-00007aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ac0: 207c 2059 6573 2020 7c20 5965 7320 7c20   | Yes  | Yes | 
-00007ad0: 5965 7320 207c 2020 2020 2020 7c0a 7c20  Yes  |      |.| 
-00007ae0: 6070 726f 7669 6465 7273 6020 2020 2020  `providers`     
-00007af0: 2020 2020 2020 2020 2020 207c 2043 6f6e             | Con
-00007b00: 7374 7261 696e 7320 7468 6520 5965 6c6c  strains the Yell
-00007b10: 6f77 446f 6720 5363 6865 6475 6c65 7220  owDog Scheduler 
-00007b20: 6f6e 6c79 2074 6f20 6578 6563 7574 6520  only to execute 
-00007b30: 7461 736b 7320 6672 6f6d 2074 6865 2061  tasks from the a
-00007b40: 7373 6f63 6961 7465 6420 5461 736b 2047  ssociated Task G
-00007b50: 726f 7570 206f 6e20 7468 6520 7370 6563  roup on the spec
-00007b60: 6966 6965 6420 7072 6f76 6964 6572 732e  ified providers.
-00007b70: 2045 2e67 2e2c 2060 5b22 4157 5322 2c20   E.g., `["AWS", 
-00007b80: 2247 4f4f 474c 4522 5d60 2e20 2020 2020  "GOOGLE"]`.     
-00007b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ba0: 2020 2020 2020 7c20 5965 7320 207c 2059        | Yes  | Y
-00007bb0: 6573 207c 2059 6573 2020 7c20 2020 2020  es | Yes  |     
-00007bc0: 207c 0a7c 2060 7261 6d60 2020 2020 2020   |.| `ram`      
-00007bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007be0: 7c20 5261 6e67 6520 636f 6e73 7472 6169  | Range constrai
-00007bf0: 6e74 206f 6e20 4742 206f 6620 5241 4d20  nt on GB of RAM 
-00007c00: 7468 6174 2061 7265 2072 6571 7569 7265  that are require
-00007c10: 6420 746f 2065 7865 6375 7465 2054 6173  d to execute Tas
-00007c20: 6b73 2e20 452e 672e 2c20 605b 322e 352c  ks. E.g., `[2.5,
-00007c30: 2034 2e30 5d60 2e20 2020 2020 2020 2020   4.0]`.         
-00007c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c80: 2020 2020 2020 2020 2020 207c 2059 6573             | Yes
-00007c90: 2020 7c20 5965 7320 7c20 5965 7320 207c    | Yes | Yes  |
-00007ca0: 2020 2020 2020 7c0a 7c20 6072 6567 696f        |.| `regio
-00007cb0: 6e73 6020 2020 2020 2020 2020 2020 2020  ns`             
-00007cc0: 2020 2020 207c 2043 6f6e 7374 7261 696e       | Constrain
-00007cd0: 7320 7468 6520 5965 6c6c 6f77 446f 6720  s the YellowDog 
-00007ce0: 5363 6865 6475 6c65 7220 6f6e 6c79 2074  Scheduler only t
-00007cf0: 6f20 6578 6563 7574 6520 5461 736b 7320  o execute Tasks 
-00007d00: 6672 6f6d 2074 6865 2061 7373 6f63 6961  from the associa
-00007d10: 7465 6420 5461 736b 2047 726f 7570 2069  ted Task Group i
-00007d20: 6e20 7468 6520 7370 6563 6966 6965 6420  n the specified 
-00007d30: 7265 6769 6f6e 732e 2045 2e67 2e2c 2060  regions. E.g., `
-00007d40: 5b22 6575 2d77 6573 742d 325d 602e 2020  ["eu-west-2]`.  
-00007d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d70: 7c20 5965 7320 207c 2059 6573 207c 2059  | Yes  | Yes | Y
-00007d80: 6573 2020 7c20 2020 2020 207c 0a7c 2060  es  |      |.| `
-00007d90: 7461 736b 4261 7463 6853 697a 6560 2020  taskBatchSize`  
-00007da0: 2020 2020 2020 2020 2020 7c20 4465 7465            | Dete
-00007db0: 726d 696e 6573 2074 6865 2062 6174 6368  rmines the batch
-00007dc0: 2073 697a 6520 7573 6564 2074 6f20 6164   size used to ad
-00007dd0: 6420 5461 736b 7320 746f 2054 6173 6b20  d Tasks to Task 
-00007de0: 4772 6f75 7073 2e20 4465 6661 756c 7420  Groups. Default 
-00007df0: 6973 2032 2c30 3030 2e20 2020 2020 2020  is 2,000.       
-00007e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007450: 2020 2020 7c20 5965 7320 207c 2059 6573      | Yes  | Yes
+00007460: 207c 2020 2020 2020 7c20 2020 2020 207c   |      |      |
+00007470: 0a7c 2060 696e 7075 7473 6020 2020 2020  .| `inputs`     
+00007480: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00007490: 5468 6520 6c69 7374 206f 6620 696e 7075  The list of inpu
+000074a0: 7420 6669 6c65 7320 746f 2062 6520 7570  t files to be up
+000074b0: 6c6f 6164 6564 2074 6f20 7468 6520 5965  loaded to the Ye
+000074c0: 6c6c 6f77 446f 6720 4f62 6a65 6374 2053  llowDog Object S
+000074d0: 746f 7265 2c20 616e 6420 7265 7175 6972  tore, and requir
+000074e0: 6564 2062 7920 7468 6520 5461 736b 2028  ed by the Task (
+000074f0: 696d 706c 6965 7320 6076 6572 6966 7941  implies `verifyA
+00007500: 7453 7461 7274 6029 2e20 452e 672e 2060  tStart`). E.g. `
+00007510: 5b22 612e 7368 222c 2022 622e 7368 225d  ["a.sh", "b.sh"]
+00007520: 602e 2020 2020 2020 2020 2020 2020 2020  `.              
+00007530: 2020 2020 2020 2020 207c 2059 6573 2020           | Yes  
+00007540: 7c20 5965 7320 7c20 5965 7320 207c 2059  | Yes | Yes  | Y
+00007550: 6573 2020 7c0a 7c20 6069 6e70 7574 734f  es  |.| `inputsO
+00007560: 7074 696f 6e61 6c60 2020 2020 2020 2020  ptional`        
+00007570: 2020 207c 2041 206c 6973 7420 6f66 2069     | A list of i
+00007580: 6e70 7574 2066 696c 6573 2072 6571 7569  nput files requi
+00007590: 7265 6420 6279 2061 2054 6173 6b2c 2062  red by a Task, b
+000075a0: 7574 2077 6869 6368 2061 7265 206e 6f74  ut which are not
+000075b0: 2073 7562 6a65 6374 2074 6f20 7665 7269   subject to veri
+000075c0: 6669 6361 7469 6f6e 2e20 4361 6e20 636f  fication. Can co
+000075d0: 6e74 6169 6e20 7769 6c64 6361 7264 732e  ntain wildcards.
+000075e0: 2045 2e67 2e3a 2060 5b22 7461 736b 5f67   E.g.: `["task_g
+000075f0: 726f 7570 5f31 2f2a 2a2f 7265 7375 6c74  roup_1/**/result
+00007600: 732e 7478 7422 5d60 2e20 2020 2020 2020  s.txt"]`.       
+00007610: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00007620: 5965 7320 207c 2059 6573 207c 2059 6573  Yes  | Yes | Yes
+00007630: 2020 7c20 5965 7320 207c 0a7c 2060 696e    | Yes  |.| `in
+00007640: 7374 616e 6365 5479 7065 7360 2020 2020  stanceTypes`    
+00007650: 2020 2020 2020 2020 7c20 5468 6520 6d61          | The ma
+00007660: 6368 696e 6520 696e 7374 616e 6365 2074  chine instance t
+00007670: 7970 6573 2074 6861 7420 6361 6e20 6265  ypes that can be
+00007680: 2075 7365 6420 746f 2065 7865 6375 7465   used to execute
+00007690: 2054 6173 6b73 2e20 452e 672e 2c20 605b   Tasks. E.g., `[
+000076a0: 2274 332e 6d69 6372 6f22 2c20 2274 3361  "t3.micro", "t3a
+000076b0: 2e6d 6963 726f 225d 602e 2020 2020 2020  .micro"]`.      
+000076c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000076d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000076e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000076f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007700: 2020 207c 2059 6573 2020 7c20 5965 7320     | Yes  | Yes 
+00007710: 7c20 5965 7320 207c 2020 2020 2020 7c0a  | Yes  |      |.
+00007720: 7c20 606d 6178 696d 756d 5461 736b 5265  | `maximumTaskRe
+00007730: 7472 6965 7360 2020 2020 2020 207c 2054  tries`       | T
+00007740: 6865 206d 6178 696d 756d 206e 756d 6265  he maximum numbe
+00007750: 7220 6f66 2074 696d 6573 2061 2054 6173  r of times a Tas
+00007760: 6b20 6361 6e20 6265 2072 6574 7269 6564  k can be retried
+00007770: 2061 6674 6572 2069 7420 6861 7320 6661   after it has fa
+00007780: 696c 6564 2e20 452e 672e 3a20 6035 602e  iled. E.g.: `5`.
+00007790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000077a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000077b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000077c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000077d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000077e0: 2020 2020 2020 2020 7c20 5965 7320 207c          | Yes  |
+000077f0: 2059 6573 207c 2059 6573 2020 7c20 2020   Yes | Yes  |   
+00007800: 2020 207c 0a7c 2060 6d61 7857 6f72 6b65     |.| `maxWorke
+00007810: 7273 6020 2020 2020 2020 2020 2020 2020  rs`             
+00007820: 2020 7c20 5468 6520 6d61 7869 6d75 6d20    | The maximum 
+00007830: 6e75 6d62 6572 206f 6620 576f 726b 6572  number of Worker
+00007840: 7320 7468 6174 2063 616e 2062 6520 636c  s that can be cl
+00007850: 6169 6d65 6420 666f 7220 7468 6520 6173  aimed for the as
+00007860: 736f 6369 6174 6564 2054 6173 6b20 4772  sociated Task Gr
+00007870: 6f75 702e 2045 2e67 2e2c 2060 3130 602e  oup. E.g., `10`.
+00007880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000078a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000078b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000078c0: 2020 2020 2020 2020 2020 2020 207c 2059               | Y
+000078d0: 6573 2020 7c20 5965 7320 7c20 5965 7320  es  | Yes | Yes 
+000078e0: 207c 2020 2020 2020 7c0a 7c20 606d 696e   |      |.| `min
+000078f0: 576f 726b 6572 7360 2020 2020 2020 2020  Workers`        
+00007900: 2020 2020 2020 207c 2054 6865 206d 696e         | The min
+00007910: 696d 756d 206e 756d 6265 7220 6f66 2057  imum number of W
+00007920: 6f72 6b65 7273 2074 6861 7420 7468 6520  orkers that the 
+00007930: 6173 736f 6369 6174 6564 2054 6173 6b20  associated Task 
+00007940: 4772 6f75 7020 7265 7175 6972 6573 2e20  Group requires. 
+00007950: 5468 6973 206d 616e 7920 776f 726b 6572  This many worker
+00007960: 7320 6d75 7374 2062 6520 636c 6169 6d65  s must be claime
+00007970: 6420 6265 666f 7265 2074 6865 2061 7373  d before the ass
+00007980: 6f63 6961 7465 6420 5461 736b 2047 726f  ociated Task Gro
+00007990: 7570 2077 696c 6c20 7374 6172 7420 776f  up will start wo
+000079a0: 726b 696e 672e 2045 2e67 2e2c 2060 3160  rking. E.g., `1`
+000079b0: 2e20 7c20 5965 7320 207c 2059 6573 207c  . | Yes  | Yes |
+000079c0: 2059 6573 2020 7c20 2020 2020 207c 0a7c   Yes  |      |.|
+000079d0: 2060 6e61 6d65 6020 2020 2020 2020 2020   `name`         
+000079e0: 2020 2020 2020 2020 2020 2020 7c20 5468              | Th
+000079f0: 6520 6e61 6d65 206f 6620 7468 6520 576f  e name of the Wo
+00007a00: 726b 2052 6571 7569 7265 6d65 6e74 2c20  rk Requirement, 
+00007a10: 5461 736b 2047 726f 7570 206f 7220 5461  Task Group or Ta
+00007a20: 736b 2e20 452e 672e 2c20 6022 7772 5f6e  sk. E.g., `"wr_n
+00007a30: 616d 6522 602e 204e 6f74 6520 7468 6174  ame"`. Note that
+00007a40: 2074 6865 2060 6e61 6d65 6020 7072 6f70   the `name` prop
+00007a50: 6572 7479 2069 7320 6e6f 7420 696e 6865  erty is not inhe
+00007a60: 7269 7465 642e 2020 2020 2020 2020 2020  rited.          
+00007a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a90: 2020 2020 2020 207c 2059 6573 2020 7c20         | Yes  | 
+00007aa0: 5965 7320 7c20 5965 7320 207c 2059 6573  Yes | Yes  | Yes
+00007ab0: 2020 7c0a 7c20 606f 7574 7075 7473 6020    |.| `outputs` 
+00007ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ad0: 207c 2054 6865 2066 696c 6573 2074 6f20   | The files to 
+00007ae0: 6265 2075 706c 6f61 6465 6420 746f 2074  be uploaded to t
+00007af0: 6865 2059 656c 6c6f 7744 6f67 204f 626a  he YellowDog Obj
+00007b00: 6563 7420 5374 6f72 6520 6279 2061 2057  ect Store by a W
+00007b10: 6f72 6b65 7220 6e6f 6465 206f 6e20 636f  orker node on co
+00007b20: 6d70 6c65 7469 6f6e 206f 6620 7468 6520  mpletion of the 
+00007b30: 5461 736b 2e20 452e 672e 2c20 605b 2272  Task. E.g., `["r
+00007b40: 6573 756c 7473 5f31 2e74 7874 222c 2022  esults_1.txt", "
+00007b50: 7265 7375 6c74 735f 322e 7478 7422 5d60  results_2.txt"]`
+00007b60: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
+00007b70: 2020 2020 2020 2020 2020 2020 7c20 5965              | Ye
+00007b80: 7320 207c 2059 6573 207c 2059 6573 2020  s  | Yes | Yes  
+00007b90: 7c20 5965 7320 207c 0a7c 2060 6f75 7470  | Yes  |.| `outp
+00007ba0: 7574 7352 6571 7569 7265 6460 2020 2020  utsRequired`    
+00007bb0: 2020 2020 2020 7c20 5468 6520 6669 6c65        | The file
+00007bc0: 7320 7468 6174 202a 6d75 7374 2a20 6265  s that *must* be
+00007bd0: 2075 706c 6f61 6465 6420 746f 2074 6865   uploaded to the
+00007be0: 2059 656c 6c6f 7744 6f67 204f 626a 6563   YellowDog Objec
+00007bf0: 7420 5374 6f72 6520 6279 2061 2057 6f72  t Store by a Wor
+00007c00: 6b65 7220 6e6f 6465 206f 6e20 636f 6d70  ker node on comp
+00007c10: 6c65 7469 6f6e 206f 6620 7468 6520 5461  letion of the Ta
+00007c20: 736b 2e20 5468 6520 5461 736b 2077 696c  sk. The Task wil
+00007c30: 6c20 6661 696c 2069 6620 616e 7920 6f75  l fail if any ou
+00007c40: 7470 7574 7320 6172 6520 756e 6176 6169  tputs are unavai
+00007c50: 6c61 626c 652e 2020 2020 2020 2020 2020  lable.          
+00007c60: 207c 2059 6573 2020 7c20 5965 7320 7c20   | Yes  | Yes | 
+00007c70: 5965 7320 207c 2059 6573 2020 7c0a 7c20  Yes  | Yes  |.| 
+00007c80: 6070 7269 6f72 6974 7960 2020 2020 2020  `priority`      
+00007c90: 2020 2020 2020 2020 2020 207c 2054 6865             | The
+00007ca0: 2070 7269 6f72 6974 7920 6f66 2057 6f72   priority of Wor
+00007cb0: 6b20 5265 7175 6972 656d 656e 7473 2061  k Requirements a
+00007cc0: 6e64 2054 6173 6b20 4772 6f75 7073 2e20  nd Task Groups. 
+00007cd0: 4869 6768 6572 2070 7269 6f72 6974 7920  Higher priority 
+00007ce0: 6163 7175 6972 6573 2057 6f72 6b65 7273  acquires Workers
+00007cf0: 2061 6865 6164 206f 6620 6c6f 7765 7220   ahead of lower 
+00007d00: 7072 696f 7269 7479 2e20 452e 672e 2c20  priority. E.g., 
+00007d10: 6030 2e30 602e 2020 2020 2020 2020 2020  `0.0`.          
+00007d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d40: 2020 2020 2020 7c20 5965 7320 207c 2059        | Yes  | Y
+00007d50: 6573 207c 2059 6573 2020 7c20 2020 2020  es | Yes  |     
+00007d60: 207c 0a7c 2060 7072 6f76 6964 6572 7360   |.| `providers`
+00007d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d80: 7c20 436f 6e73 7472 6169 6e73 2074 6865  | Constrains the
+00007d90: 2059 656c 6c6f 7744 6f67 2053 6368 6564   YellowDog Sched
+00007da0: 756c 6572 206f 6e6c 7920 746f 2065 7865  uler only to exe
+00007db0: 6375 7465 2074 6173 6b73 2066 726f 6d20  cute tasks from 
+00007dc0: 7468 6520 6173 736f 6369 6174 6564 2054  the associated T
+00007dd0: 6173 6b20 4772 6f75 7020 6f6e 2074 6865  ask Group on the
+00007de0: 2073 7065 6369 6669 6564 2070 726f 7669   specified provi
+00007df0: 6465 7273 2e20 452e 672e 2c20 605b 2241  ders. E.g., `["A
+00007e00: 5753 222c 2022 474f 4f47 4c45 225d 602e  WS", "GOOGLE"]`.
 00007e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e50: 2020 2020 207c 2059 6573 2020 7c20 2020       | Yes  |   
-00007e60: 2020 7c20 2020 2020 207c 2020 2020 2020    |      |      
-00007e70: 7c0a 7c20 6074 6173 6b43 6f75 6e74 6020  |.| `taskCount` 
-00007e80: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00007e90: 2054 6865 206e 756d 6265 7220 6f66 2074   The number of t
-00007ea0: 696d 6573 2074 6f20 6578 6563 7574 6520  imes to execute 
-00007eb0: 7468 6520 5461 736b 2e20 4361 6e20 6265  the Task. Can be
-00007ec0: 2073 6574 2069 6e20 7468 6520 544f 4d4c   set in the TOML
-00007ed0: 2066 696c 6520 6f72 2069 6e20 616e 7920   file or in any 
-00007ee0: 4a53 4f4e 2054 6173 6b20 4772 6f75 7020  JSON Task Group 
-00007ef0: 6465 6669 6e69 7469 6f6e 2e20 4e6f 7465  definition. Note
-00007f00: 3a20 6e6f 2069 6e68 6572 6974 616e 6365  : no inheritance
-00007f10: 2066 726f 6d20 544f 4d4c 2074 6f20 4a53   from TOML to JS
-00007f20: 4f4e 2e20 2020 2020 2020 2020 2020 2020  ON.             
-00007f30: 2020 2020 2020 2020 2020 7c20 5965 7320            | Yes 
-00007f40: 207c 2020 2020 207c 2059 6573 2020 7c20   |     | Yes  | 
-00007f50: 2020 2020 207c 0a7c 2060 7461 736b 4461       |.| `taskDa
-00007f60: 7461 6020 2020 2020 2020 2020 2020 2020  ta`             
-00007f70: 2020 2020 7c20 5468 6520 6461 7461 2074      | The data t
-00007f80: 6f20 6265 2070 6173 7365 6420 746f 2074  o be passed to t
-00007f90: 6865 2057 6f72 6b65 7220 7768 656e 2074  he Worker when t
-00007fa0: 6865 2054 6173 6b20 6973 2073 7461 7274  he Task is start
-00007fb0: 6564 2e20 452e 672e 2c20 6022 6d79 6461  ed. E.g., `"myda
-00007fc0: 7461 2260 2e20 4265 636f 6d65 7320 6669  ta"`. Becomes fi
-00007fd0: 6c65 2060 7461 736b 6461 7461 2e74 7874  le `taskdata.txt
-00007fe0: 6020 696e 2074 6865 2054 6173 6b27 7320  ` in the Task's 
-00007ff0: 776f 726b 696e 6720 6469 7265 6374 6f72  working director
-00008000: 7920 7768 656e 2054 6865 2054 6173 6b20  y when The Task 
-00008010: 6578 6563 7574 6573 2e20 2020 2020 207c  executes.      |
-00008020: 2059 6573 2020 7c20 5965 7320 7c20 5965   Yes  | Yes | Ye
-00008030: 7320 207c 2059 6573 2020 7c0a 7c20 6074  s  | Yes  |.| `t
-00008040: 6173 6b44 6174 6146 696c 6560 2020 2020  askDataFile`    
-00008050: 2020 2020 2020 2020 207c 2050 6f70 756c           | Popul
-00008060: 6174 6520 7468 6520 6074 6173 6b44 6174  ate the `taskDat
-00008070: 6160 2070 726f 7065 7274 7920 6162 6f76  a` property abov
-00008080: 6520 7769 7468 2074 6865 2063 6f6e 7465  e with the conte
-00008090: 6e74 7320 6f66 2074 6865 2073 7065 6369  nts of the speci
-000080a0: 6669 6564 2066 696c 652e 2045 2e67 2e2c  fied file. E.g.,
-000080b0: 2060 226d 795f 7461 736b 5f64 6174 615f   `"my_task_data_
-000080c0: 6669 6c65 2e74 7874 2260 2e20 2020 2020  file.txt"`.     
-000080d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000080e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000080f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008100: 2020 2020 7c20 5965 7320 207c 2059 6573      | Yes  | Yes
-00008110: 207c 2059 6573 2020 7c20 5965 7320 207c   | Yes  | Yes  |
-00008120: 0a7c 2060 7461 736b 4e61 6d65 6020 2020  .| `taskName`   
-00008130: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00008140: 5468 6520 6e61 6d65 2074 6f20 7573 6520  The name to use 
-00008150: 666f 7220 7468 6520 5461 736b 2e20 4f6e  for the Task. On
-00008160: 6c79 2075 7361 626c 6520 696e 2074 6865  ly usable in the
-00008170: 2054 4f4d 4c20 6669 6c65 2e20 4d6f 7374   TOML file. Most
-00008180: 6c79 2075 7365 6675 6c20 696e 2063 6f6e  ly useful in con
-00008190: 6a75 6e63 7469 6f6e 2077 6974 6820 4353  junction with CS
-000081a0: 5620 5461 736b 2064 6174 612e 2045 2e67  V Task data. E.g
-000081b0: 2e2c 2060 226d 795f 7461 736b 5f6e 756d  ., `"my_task_num
-000081c0: 6265 725f 7b7b 7461 736b 5f6e 756d 6265  ber_{{task_numbe
-000081d0: 727d 7d22 602e 2020 2020 2020 2020 2020  r}}"`.          
-000081e0: 2020 2020 2020 2020 207c 2059 6573 2020           | Yes  
-000081f0: 7c20 2020 2020 7c20 2020 2020 207c 2020  |     |      |  
-00008200: 2020 2020 7c0a 7c20 6074 6173 6b47 726f      |.| `taskGro
-00008210: 7570 4e61 6d65 6020 2020 2020 2020 2020  upName`         
-00008220: 2020 207c 2054 6865 206e 616d 6520 746f     | The name to
-00008230: 2075 7365 2066 6f72 2074 6865 2054 6173   use for the Tas
-00008240: 6b20 4772 6f75 702e 204f 6e6c 7920 7573  k Group. Only us
-00008250: 6162 6c65 2069 6e20 7468 6520 544f 4d4c  able in the TOML
-00008260: 2066 696c 652e 2045 2e67 2e2c 2060 226d   file. E.g., `"m
-00008270: 795f 7467 5f6e 756d 6265 725f 7b7b 7461  y_tg_number_{{ta
-00008280: 736b 5f67 726f 7570 5f6e 756d 6265 727d  sk_group_number}
-00008290: 7d22 602e 2020 2020 2020 2020 2020 2020  }"`.            
-000082a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000082b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000082c0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-000082d0: 5965 7320 207c 2020 2020 207c 2020 2020  Yes  |     |    
-000082e0: 2020 7c20 2020 2020 207c 0a7c 2060 7461    |      |.| `ta
-000082f0: 736b 5479 7065 6020 2020 2020 2020 2020  skType`         
-00008300: 2020 2020 2020 2020 7c20 5468 6520 5461          | The Ta
-00008310: 736b 2054 7970 6520 6f66 2061 2054 6173  sk Type of a Tas
-00008320: 6b2e 2045 2e67 2e2c 2060 2264 6f63 6b65  k. E.g., `"docke
-00008330: 7222 602e 2020 2020 2020 2020 2020 2020  r"`.            
-00008340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007e20: 2020 2020 2020 2020 2020 207c 2059 6573             | Yes
+00007e30: 2020 7c20 5965 7320 7c20 5965 7320 207c    | Yes | Yes  |
+00007e40: 2020 2020 2020 7c0a 7c20 6072 616d 6020        |.| `ram` 
+00007e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007e60: 2020 2020 207c 2052 616e 6765 2063 6f6e       | Range con
+00007e70: 7374 7261 696e 7420 6f6e 2047 4220 6f66  straint on GB of
+00007e80: 2052 414d 2074 6861 7420 6172 6520 7265   RAM that are re
+00007e90: 7175 6972 6564 2074 6f20 6578 6563 7574  quired to execut
+00007ea0: 6520 5461 736b 732e 2045 2e67 2e2c 2060  e Tasks. E.g., `
+00007eb0: 5b32 2e35 2c20 342e 305d 602e 2020 2020  [2.5, 4.0]`.    
+00007ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f10: 7c20 5965 7320 207c 2059 6573 207c 2059  | Yes  | Yes | Y
+00007f20: 6573 2020 7c20 2020 2020 207c 0a7c 2060  es  |      |.| `
+00007f30: 7265 6769 6f6e 7360 2020 2020 2020 2020  regions`        
+00007f40: 2020 2020 2020 2020 2020 7c20 436f 6e73            | Cons
+00007f50: 7472 6169 6e73 2074 6865 2059 656c 6c6f  trains the Yello
+00007f60: 7744 6f67 2053 6368 6564 756c 6572 206f  wDog Scheduler o
+00007f70: 6e6c 7920 746f 2065 7865 6375 7465 2054  nly to execute T
+00007f80: 6173 6b73 2066 726f 6d20 7468 6520 6173  asks from the as
+00007f90: 736f 6369 6174 6564 2054 6173 6b20 4772  sociated Task Gr
+00007fa0: 6f75 7020 696e 2074 6865 2073 7065 6369  oup in the speci
+00007fb0: 6669 6564 2072 6567 696f 6e73 2e20 452e  fied regions. E.
+00007fc0: 672e 2c20 605b 2265 752d 7765 7374 2d32  g., `["eu-west-2
+00007fd0: 5d60 2e20 2020 2020 2020 2020 2020 2020  ]`.             
+00007fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ff0: 2020 2020 207c 2059 6573 2020 7c20 5965       | Yes  | Ye
+00008000: 7320 7c20 5965 7320 207c 2020 2020 2020  s | Yes  |      
+00008010: 7c0a 7c20 6074 6173 6b42 6174 6368 5369  |.| `taskBatchSi
+00008020: 7a65 6020 2020 2020 2020 2020 2020 207c  ze`            |
+00008030: 2044 6574 6572 6d69 6e65 7320 7468 6520   Determines the 
+00008040: 6261 7463 6820 7369 7a65 2075 7365 6420  batch size used 
+00008050: 746f 2061 6464 2054 6173 6b73 2074 6f20  to add Tasks to 
+00008060: 5461 736b 2047 726f 7570 732e 2044 6566  Task Groups. Def
+00008070: 6175 6c74 2069 7320 322c 3030 302e 2020  ault is 2,000.  
+00008080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000080a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000080b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000080c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000080d0: 2020 2020 2020 2020 2020 7c20 5965 7320            | Yes 
+000080e0: 207c 2020 2020 207c 2020 2020 2020 7c20   |     |      | 
+000080f0: 2020 2020 207c 0a7c 2060 7461 736b 436f       |.| `taskCo
+00008100: 756e 7460 2020 2020 2020 2020 2020 2020  unt`            
+00008110: 2020 2020 7c20 5468 6520 6e75 6d62 6572      | The number
+00008120: 206f 6620 7469 6d65 7320 746f 2065 7865   of times to exe
+00008130: 6375 7465 2074 6865 2054 6173 6b2e 2043  cute the Task. C
+00008140: 616e 2062 6520 7365 7420 696e 2074 6865  an be set in the
+00008150: 2054 4f4d 4c20 6669 6c65 206f 7220 696e   TOML file or in
+00008160: 2061 6e79 204a 534f 4e20 5461 736b 2047   any JSON Task G
+00008170: 726f 7570 2064 6566 696e 6974 696f 6e2e  roup definition.
+00008180: 204e 6f74 653a 206e 6f20 696e 6865 7269   Note: no inheri
+00008190: 7461 6e63 6520 6672 6f6d 2054 4f4d 4c20  tance from TOML 
+000081a0: 746f 204a 534f 4e2e 2020 2020 2020 2020  to JSON.        
+000081b0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+000081c0: 2059 6573 2020 7c20 2020 2020 7c20 5965   Yes  |     | Ye
+000081d0: 7320 207c 2020 2020 2020 7c0a 7c20 6074  s  |      |.| `t
+000081e0: 6173 6b44 6174 6160 2020 2020 2020 2020  askData`        
+000081f0: 2020 2020 2020 2020 207c 2054 6865 2064           | The d
+00008200: 6174 6120 746f 2062 6520 7061 7373 6564  ata to be passed
+00008210: 2074 6f20 7468 6520 576f 726b 6572 2077   to the Worker w
+00008220: 6865 6e20 7468 6520 5461 736b 2069 7320  hen the Task is 
+00008230: 7374 6172 7465 642e 2045 2e67 2e2c 2060  started. E.g., `
+00008240: 226d 7964 6174 6122 602e 2042 6563 6f6d  "mydata"`. Becom
+00008250: 6573 2066 696c 6520 6074 6173 6b64 6174  es file `taskdat
+00008260: 612e 7478 7460 2069 6e20 7468 6520 5461  a.txt` in the Ta
+00008270: 736b 2773 2077 6f72 6b69 6e67 2064 6972  sk's working dir
+00008280: 6563 746f 7279 2077 6865 6e20 5468 6520  ectory when The 
+00008290: 5461 736b 2065 7865 6375 7465 732e 2020  Task executes.  
+000082a0: 2020 2020 7c20 5965 7320 207c 2059 6573      | Yes  | Yes
+000082b0: 207c 2059 6573 2020 7c20 5965 7320 207c   | Yes  | Yes  |
+000082c0: 0a7c 2060 7461 736b 4461 7461 4669 6c65  .| `taskDataFile
+000082d0: 6020 2020 2020 2020 2020 2020 2020 7c20  `             | 
+000082e0: 506f 7075 6c61 7465 2074 6865 2060 7461  Populate the `ta
+000082f0: 736b 4461 7461 6020 7072 6f70 6572 7479  skData` property
+00008300: 2061 626f 7665 2077 6974 6820 7468 6520   above with the 
+00008310: 636f 6e74 656e 7473 206f 6620 7468 6520  contents of the 
+00008320: 7370 6563 6966 6965 6420 6669 6c65 2e20  specified file. 
+00008330: 452e 672e 2c20 6022 6d79 5f74 6173 6b5f  E.g., `"my_task_
+00008340: 6461 7461 5f66 696c 652e 7478 7422 602e  data_file.txt"`.
 00008350: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008360: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000083a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000083b0: 2020 207c 2059 6573 2020 7c20 2020 2020     | Yes  |     
-000083c0: 7c20 2020 2020 207c 2059 6573 2020 7c0a  |      | Yes  |.
-000083d0: 7c20 6074 6173 6b54 7970 6573 6020 2020  | `taskTypes`   
-000083e0: 2020 2020 2020 2020 2020 2020 207c 2054               | T
-000083f0: 6865 206c 6973 7420 6f66 2054 6173 6b20  he list of Task 
-00008400: 5479 7065 7320 7265 7175 6972 6564 2062  Types required b
-00008410: 7920 7468 6520 7261 6e67 6520 6f66 2054  y the range of T
-00008420: 6173 6b73 2069 6e20 6120 5461 736b 2047  asks in a Task G
-00008430: 726f 7570 2e20 452e 672e 2c20 605b 2264  roup. E.g., `["d
-00008440: 6f63 6b65 7222 2c20 6261 7368 225d 602e  ocker", bash"]`.
-00008450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008490: 2020 2020 2020 2020 7c20 2020 2020 207c          |      |
-000084a0: 2059 6573 207c 2059 6573 2020 7c20 2020   Yes | Yes  |   
-000084b0: 2020 207c 0a7c 2060 7461 736b 7350 6572     |.| `tasksPer
-000084c0: 576f 726b 6572 6020 2020 2020 2020 2020  Worker`         
-000084d0: 2020 7c20 4465 7465 726d 696e 6573 2074    | Determines t
-000084e0: 6865 206e 756d 6265 7220 6f66 2057 6f72  he number of Wor
-000084f0: 6b65 7220 636c 6169 6d73 2062 6173 6564  ker claims based
-00008500: 206f 6e20 7370 6c69 7474 696e 6720 7468   on splitting th
-00008510: 6520 6e75 6d62 6572 206f 6620 756e 6669  e number of unfi
-00008520: 6e69 7368 6564 2054 6173 6b73 2061 6372  nished Tasks acr
-00008530: 6f73 7320 576f 726b 6572 732e 2045 2e67  oss Workers. E.g
-00008540: 2e2c 2060 3160 2e20 2020 2020 2020 2020  ., `1`.         
-00008550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008570: 2020 2020 2020 2020 2020 2020 207c 2059               | Y
-00008580: 6573 2020 7c20 5965 7320 7c20 5965 7320  es  | Yes | Yes 
-00008590: 207c 2020 2020 2020 7c0a 7c20 6075 706c   |      |.| `upl
-000085a0: 6f61 6446 696c 6573 6020 2020 2020 2020  oadFiles`       
-000085b0: 2020 2020 2020 207c 2054 6865 206c 6973         | The lis
-000085c0: 7420 6f66 2066 696c 6573 2074 6f20 6265  t of files to be
-000085d0: 2075 706c 6f61 6465 6420 746f 2074 6865   uploaded to the
-000085e0: 2059 656c 6c6f 7744 6f67 204f 626a 6563   YellowDog Objec
-000085f0: 7420 5374 6f72 652e 2045 2e67 2e2c 2028  t Store. E.g., (
-00008600: 4a53 4f4e 293a 2060 5b7b 226c 6f63 616c  JSON): `[{"local
-00008610: 5061 7468 223a 2066 696c 655f 312e 7478  Path": file_1.tx
-00008620: 7422 2c20 2275 706c 6f61 6450 6174 6822  t", "uploadPath"
-00008630: 3a20 2266 696c 655f 312e 7478 7422 7d5d  : "file_1.txt"}]
-00008640: 602e 2020 2020 2020 2020 2020 2020 2020  `.              
-00008650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008660: 2020 7c20 5965 7320 207c 2059 6573 207c    | Yes  | Yes |
-00008670: 2059 6573 2020 7c20 5965 7320 207c 0a7c   Yes  | Yes  |.|
-00008680: 2060 7663 7075 7360 2020 2020 2020 2020   `vcpus`        
-00008690: 2020 2020 2020 2020 2020 2020 7c20 5261              | Ra
-000086a0: 6e67 6520 636f 6e73 7472 6169 6e74 206f  nge constraint o
-000086b0: 6e20 6e75 6d62 6572 206f 6620 7643 5055  n number of vCPU
-000086c0: 7320 7468 6174 2061 7265 2072 6571 7569  s that are requi
-000086d0: 7265 6420 746f 2065 7865 6375 7465 2054  red to execute T
-000086e0: 6173 6b73 2045 2e67 2e2c 2060 5b32 2e30  asks E.g., `[2.0
-000086f0: 2c20 342e 305d 602e 2020 2020 2020 2020  , 4.0]`.        
+00008380: 2020 2020 2020 2020 207c 2059 6573 2020           | Yes  
+00008390: 7c20 5965 7320 7c20 5965 7320 207c 2059  | Yes | Yes  | Y
+000083a0: 6573 2020 7c0a 7c20 6074 6173 6b4e 616d  es  |.| `taskNam
+000083b0: 6560 2020 2020 2020 2020 2020 2020 2020  e`              
+000083c0: 2020 207c 2054 6865 206e 616d 6520 746f     | The name to
+000083d0: 2075 7365 2066 6f72 2074 6865 2054 6173   use for the Tas
+000083e0: 6b2e 204f 6e6c 7920 7573 6162 6c65 2069  k. Only usable i
+000083f0: 6e20 7468 6520 544f 4d4c 2066 696c 652e  n the TOML file.
+00008400: 204d 6f73 746c 7920 7573 6566 756c 2069   Mostly useful i
+00008410: 6e20 636f 6e6a 756e 6374 696f 6e20 7769  n conjunction wi
+00008420: 7468 2043 5356 2054 6173 6b20 6461 7461  th CSV Task data
+00008430: 2e20 452e 672e 2c20 6022 6d79 5f74 6173  . E.g., `"my_tas
+00008440: 6b5f 6e75 6d62 6572 5f7b 7b74 6173 6b5f  k_number_{{task_
+00008450: 6e75 6d62 6572 7d7d 2260 2e20 2020 2020  number}}"`.     
+00008460: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00008470: 5965 7320 207c 2020 2020 207c 2020 2020  Yes  |     |    
+00008480: 2020 7c20 2020 2020 207c 0a7c 2060 7461    |      |.| `ta
+00008490: 736b 4772 6f75 704e 616d 6560 2020 2020  skGroupName`    
+000084a0: 2020 2020 2020 2020 7c20 5468 6520 6e61          | The na
+000084b0: 6d65 2074 6f20 7573 6520 666f 7220 7468  me to use for th
+000084c0: 6520 5461 736b 2047 726f 7570 2e20 4f6e  e Task Group. On
+000084d0: 6c79 2075 7361 626c 6520 696e 2074 6865  ly usable in the
+000084e0: 2054 4f4d 4c20 6669 6c65 2e20 452e 672e   TOML file. E.g.
+000084f0: 2c20 6022 6d79 5f74 675f 6e75 6d62 6572  , `"my_tg_number
+00008500: 5f7b 7b74 6173 6b5f 6772 6f75 705f 6e75  _{{task_group_nu
+00008510: 6d62 6572 7d7d 2260 2e20 2020 2020 2020  mber}}"`.       
+00008520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008550: 2020 207c 2059 6573 2020 7c20 2020 2020     | Yes  |     
+00008560: 7c20 2020 2020 207c 2020 2020 2020 7c0a  |      |      |.
+00008570: 7c20 6074 6173 6b54 7970 6560 2020 2020  | `taskType`    
+00008580: 2020 2020 2020 2020 2020 2020 207c 2054               | T
+00008590: 6865 2054 6173 6b20 5479 7065 206f 6620  he Task Type of 
+000085a0: 6120 5461 736b 2e20 452e 672e 2c20 6022  a Task. E.g., `"
+000085b0: 646f 636b 6572 2260 2e20 2020 2020 2020  docker"`.       
+000085c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000085d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000085e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000085f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008630: 2020 2020 2020 2020 7c20 5965 7320 207c          | Yes  |
+00008640: 2020 2020 207c 2020 2020 2020 7c20 5965       |      | Ye
+00008650: 7320 207c 0a7c 2060 7461 736b 5479 7065  s  |.| `taskType
+00008660: 7360 2020 2020 2020 2020 2020 2020 2020  s`              
+00008670: 2020 7c20 5468 6520 6c69 7374 206f 6620    | The list of 
+00008680: 5461 736b 2054 7970 6573 2072 6571 7569  Task Types requi
+00008690: 7265 6420 6279 2074 6865 2072 616e 6765  red by the range
+000086a0: 206f 6620 5461 736b 7320 696e 2061 2054   of Tasks in a T
+000086b0: 6173 6b20 4772 6f75 702e 2045 2e67 2e2c  ask Group. E.g.,
+000086c0: 2060 5b22 646f 636b 6572 222c 2062 6173   `["docker", bas
+000086d0: 6822 5d60 2e20 2020 2020 2020 2020 2020  h"]`.           
+000086e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000086f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008740: 2020 2020 2020 207c 2059 6573 2020 7c20         | Yes  | 
-00008750: 5965 7320 7c20 5965 7320 207c 2020 2020  Yes | Yes  |    
-00008760: 2020 7c0a 7c20 6076 6572 6966 7941 7453    |.| `verifyAtS
-00008770: 7461 7274 6020 2020 2020 2020 2020 2020  tart`           
-00008780: 207c 2041 206c 6973 7420 6f66 2066 696c   | A list of fil
-00008790: 6573 2072 6571 7569 7265 6420 6279 2061  es required by a
-000087a0: 2054 6173 6b2e 204d 7573 7420 6265 2070   Task. Must be p
-000087b0: 7265 7365 6e74 2077 6865 6e20 7468 6520  resent when the 
-000087c0: 5461 736b 2069 7320 7265 6164 7920 746f  Task is ready to
-000087d0: 2073 7461 7274 206f 7220 7468 6520 5461   start or the Ta
-000087e0: 736b 2077 696c 6c20 6661 696c 2e20 452e  sk will fail. E.
-000087f0: 672e 3a20 605b 2274 6173 6b5f 6772 6f75  g.: `["task_grou
-00008800: 705f 312f 7461 736b 5f31 2f72 6573 756c  p_1/task_1/resul
-00008810: 7473 2e74 7874 225d 602e 2020 2020 2020  ts.txt"]`.      
-00008820: 2020 2020 2020 2020 2020 2020 7c20 5965              | Ye
-00008830: 7320 207c 2059 6573 207c 2059 6573 2020  s  | Yes | Yes  
-00008840: 7c20 5965 7320 207c 0a7c 2060 7665 7269  | Yes  |.| `veri
-00008850: 6679 5761 6974 6020 2020 2020 2020 2020  fyWait`         
-00008860: 2020 2020 2020 7c20 4120 6c69 7374 206f        | A list o
-00008870: 6620 6669 6c65 7320 7265 7175 6972 6564  f files required
-00008880: 2062 7920 6120 5461 736b 2e20 5468 6520   by a Task. The 
-00008890: 5461 736b 2077 696c 6c20 7761 6974 2075  Task will wait u
-000088a0: 6e74 696c 2074 6865 2066 696c 6573 2061  ntil the files a
-000088b0: 7265 2061 7661 696c 6162 6c65 2062 6566  re available bef
-000088c0: 6f72 6520 7374 6172 7469 6e67 2e20 452e  ore starting. E.
-000088d0: 672e 3a20 605b 2274 6173 6b5f 6772 6f75  g.: `["task_grou
-000088e0: 705f 312f 7461 736b 5f31 2f72 6573 756c  p_1/task_1/resul
-000088f0: 7473 2e74 7874 225d 602e 2020 2020 2020  ts.txt"]`.      
-00008900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008910: 207c 2059 6573 2020 7c20 5965 7320 7c20   | Yes  | Yes | 
-00008920: 5965 7320 207c 2059 6573 2020 7c0a 7c20  Yes  | Yes  |.| 
-00008930: 6077 6f72 6b65 7254 6167 7360 2020 2020  `workerTags`    
-00008940: 2020 2020 2020 2020 2020 207c 2054 6865             | The
-00008950: 206c 6973 7420 6f66 2057 6f72 6b65 7220   list of Worker 
-00008960: 5461 6773 2074 6861 7420 7769 6c6c 2062  Tags that will b
-00008970: 6520 7573 6564 2074 6f20 6d61 7463 6820  e used to match 
-00008980: 6167 6169 6e73 7420 7468 6520 576f 726b  against the Work
-00008990: 6572 2054 6167 206f 6620 6120 6361 6e64  er Tag of a cand
-000089a0: 6964 6174 6520 576f 726b 6572 2e20 452e  idate Worker. E.
-000089b0: 672e 2c20 605b 2274 6167 5f78 222c 2022  g., `["tag_x", "
-000089c0: 7461 675f 7922 5d60 2e20 2020 2020 2020  tag_y"]`.       
-000089d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089f0: 2020 2020 2020 7c20 5965 7320 207c 2059        | Yes  | Y
-00008a00: 6573 207c 2059 6573 2020 7c20 2020 2020  es | Yes  |     
-00008a10: 207c 0a7c 2060 776f 726b 5265 7175 6972   |.| `workRequir
-00008a20: 656d 656e 7444 6174 6160 2020 2020 2020  ementData`      
-00008a30: 7c20 5468 6520 6e61 6d65 206f 6620 7468  | The name of th
-00008a40: 6520 6669 6c65 2063 6f6e 7461 696e 696e  e file containin
-00008a50: 6720 7468 6520 4a53 4f4e 2064 6f63 756d  g the JSON docum
-00008a60: 656e 7420 696e 2077 6869 6368 2074 6865  ent in which the
-00008a70: 2057 6f72 6b20 5265 7175 6972 656d 656e   Work Requiremen
-00008a80: 7420 6973 2064 6566 696e 6564 2e20 452e  t is defined. E.
-00008a90: 672e 2c20 6022 7465 7374 5f77 6f72 6b72  g., `"test_workr
-00008aa0: 6571 2e6a 736f 6e22 602e 2020 2020 2020  eq.json"`.      
-00008ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ad0: 2020 2020 2020 2020 2020 207c 2059 6573             | Yes
-00008ae0: 2020 7c20 2020 2020 7c20 2020 2020 207c    |     |      |
-00008af0: 2020 2020 2020 7c0a 0a23 2320 4175 746f        |..## Auto
-00008b00: 6d61 7469 6320 5072 6f70 6572 7469 6573  matic Properties
-00008b10: 0a0a 496e 2061 6464 6974 696f 6e20 746f  ..In addition to
-00008b20: 2074 6865 2069 6e68 6572 6974 616e 6365   the inheritance
-00008b30: 206d 6563 6861 6e69 736d 2c20 736f 6d65   mechanism, some
-00008b40: 2070 726f 7065 7274 6965 7320 6172 6520   properties are 
-00008b50: 7365 7420 6175 746f 6d61 7469 6361 6c6c  set automaticall
-00008b60: 7920 6279 2074 6865 2060 7964 2d73 7562  y by the `yd-sub
-00008b70: 6d69 7460 2063 6f6d 6d61 6e64 2c20 6173  mit` command, as
-00008b80: 2061 2075 7361 6765 2063 6f6e 7665 6e69   a usage conveni
-00008b90: 656e 6365 2069 6620 7468 6579 2772 6520  ence if they're 
-00008ba0: 6e6f 7420 6578 706c 6963 6974 6c79 2070  not explicitly p
-00008bb0: 726f 7669 6465 642e 0a0a 2323 2320 576f  rovided...### Wo
-00008bc0: 726b 2052 6571 7569 7265 6d65 6e74 2c20  rk Requirement, 
-00008bd0: 5461 736b 2047 726f 7570 2061 6e64 2054  Task Group and T
-00008be0: 6173 6b20 4e61 6d69 6e67 0a0a 2d20 5468  ask Naming..- Th
-00008bf0: 6520 2a2a 576f 726b 2052 6571 7569 7265  e **Work Require
-00008c00: 6d65 6e74 2a2a 206e 616d 6520 6973 2061  ment** name is a
-00008c10: 7574 6f6d 6174 6963 616c 6c79 2073 6574  utomatically set
-00008c20: 2075 7369 6e67 2061 2063 6f6e 6361 7465   using a concate
-00008c30: 6e61 7469 6f6e 206f 6620 7468 6520 6074  nation of the `t
-00008c40: 6167 6020 7072 6f70 6572 7479 2c20 6120  ag` property, a 
-00008c50: 5554 4320 7469 6d65 7374 616d 702c 2061  UTC timestamp, a
-00008c60: 6e64 2074 6872 6565 2072 616e 646f 6d20  nd three random 
-00008c70: 6865 7820 6368 6172 6163 7465 7273 3a20  hex characters: 
-00008c80: 652c 672c 2e20 606d 7974 6167 5f32 3231  e,g,. `mytag_221
-00008c90: 3032 342d 3135 3535 3234 2d34 3061 602e  024-155524-40a`.
-00008ca0: 0a2d 202a 2a54 6173 6b20 4772 6f75 702a  .- **Task Group*
-00008cb0: 2a20 6e61 6d65 7320 6172 6520 6175 746f  * names are auto
-00008cc0: 6d61 7469 6361 6c6c 7920 6372 6561 7465  matically create
-00008cd0: 6420 666f 7220 616e 7920 5461 736b 2047  d for any Task G
-00008ce0: 726f 7570 2074 6861 7420 6973 206e 6f74  roup that is not
-00008cf0: 2065 7870 6c69 6369 746c 7920 6e61 6d65   explicitly name
-00008d00: 642c 2075 7369 6e67 206e 616d 6573 206f  d, using names o
-00008d10: 6620 7468 6520 666f 726d 2060 7461 736b  f the form `task
-00008d20: 5f67 726f 7570 5f31 6020 286f 7220 6074  _group_1` (or `t
-00008d30: 6173 6b5f 6772 6f75 705f 3031 602c 2065  ask_group_01`, e
-00008d40: 7463 2e2c 2066 6f72 206c 6172 6765 7220  tc., for larger 
-00008d50: 6e75 6d62 6572 7320 6f66 2054 6173 6b20  numbers of Task 
-00008d60: 4772 6f75 7073 292e 2054 6173 6b20 4772  Groups). Task Gr
-00008d70: 6f75 7020 6e75 6d62 6572 7320 6361 6e20  oup numbers can 
-00008d80: 616c 736f 2062 6520 696e 636c 7564 6564  also be included
-00008d90: 2069 6e20 7573 6572 2d64 6566 696e 6564   in user-defined
-00008da0: 2054 6173 6b20 4772 6f75 7020 6e61 6d65   Task Group name
-00008db0: 7320 7573 696e 6720 7468 6520 607b 7b74  s using the `{{t
-00008dc0: 6173 6b5f 6772 6f75 705f 6e75 6d62 6572  ask_group_number
-00008dd0: 7d7d 6020 7661 7269 6162 6c65 2073 7562  }}` variable sub
-00008de0: 7374 6974 7574 696f 6e20 6469 7363 7573  stitution discus
-00008df0: 7365 6420 6265 6c6f 772e 0a2d 202a 2a54  sed below..- **T
-00008e00: 6173 6b2a 2a20 6e61 6d65 7320 6172 6520  ask** names are 
-00008e10: 6175 746f 6d61 7469 6361 6c6c 7920 6372  automatically cr
-00008e20: 6561 7465 6420 666f 7220 616e 7920 5461  eated for any Ta
-00008e30: 736b 2074 6861 7420 6973 206e 6f74 2065  sk that is not e
-00008e40: 7870 6c69 6369 746c 7920 6e61 6d65 642c  xplicitly named,
-00008e50: 2075 7369 6e67 206e 616d 6573 206f 6620   using names of 
-00008e60: 7468 6520 666f 726d 2060 7461 736b 5f31  the form `task_1
-00008e70: 6020 286f 7220 6074 6173 6b5f 3031 602c  ` (or `task_01`,
-00008e80: 2065 7463 2e2c 2066 6f72 206c 6172 6765   etc., for large
-00008e90: 7220 6e75 6d62 6572 7320 6f66 2054 6173  r numbers of Tas
-00008ea0: 6b73 292e 2054 6865 2054 6173 6b20 636f  ks). The Task co
-00008eb0: 756e 7465 7220 7265 7365 7473 2066 6f72  unter resets for
-00008ec0: 2065 6163 6820 6469 6666 6572 656e 7420   each different 
-00008ed0: 5461 736b 2047 726f 7570 2e20 5461 736b  Task Group. Task
-00008ee0: 206e 756d 6265 7273 2063 616e 2061 6c73   numbers can als
-00008ef0: 6f20 6265 2069 6e63 6c75 6465 6420 696e  o be included in
-00008f00: 2075 7365 722d 6465 6669 6e65 6420 5461   user-defined Ta
-00008f10: 736b 206e 616d 6573 2075 7369 6e67 2074  sk names using t
-00008f20: 6865 2060 7b7b 7461 736b 5f6e 756d 6265  he `{{task_numbe
-00008f30: 727d 7d60 2076 6172 6961 626c 6520 7375  r}}` variable su
-00008f40: 6273 7469 7475 7469 6f6e 2064 6973 6375  bstitution discu
-00008f50: 7373 6564 2062 656c 6f77 2e0a 0a23 2323  ssed below...###
-00008f60: 2054 6173 6b20 5479 7065 730a 0a2d 2049   Task Types..- I
-00008f70: 6620 6074 6173 6b54 7970 6560 2069 7320  f `taskType` is 
-00008f80: 7365 7420 6f6e 6c79 2061 7420 7468 6520  set only at the 
-00008f90: 544f 4d4c 2066 696c 6520 6c65 7665 6c2c  TOML file level,
-00008fa0: 2074 6865 6e20 6074 6173 6b54 7970 6573   then `taskTypes
-00008fb0: 6020 6973 2061 7574 6f6d 6174 6963 616c  ` is automatical
-00008fc0: 6c79 2070 6f70 756c 6174 6564 2066 6f72  ly populated for
-00008fd0: 2054 6173 6b20 4772 6f75 7073 2c20 756e   Task Groups, un
-00008fe0: 6c65 7373 206f 7665 7272 6964 6465 6e2e  less overridden.
-00008ff0: 0a2d 2049 6620 6074 6173 6b54 7970 6560  .- If `taskType`
-00009000: 2069 7320 7365 7420 6174 2074 6865 2054   is set at the T
-00009010: 6173 6b20 6c65 7665 6c2c 2074 6865 6e20  ask level, then 
-00009020: 6074 6173 6b54 7970 6573 6020 6973 2061  `taskTypes` is a
-00009030: 7574 6f6d 6174 6963 616c 6c79 2070 6f70  utomatically pop
-00009040: 756c 6174 6564 2066 6f72 2074 6865 2054  ulated for the T
-00009050: 6173 6b20 4772 6f75 7073 206c 6576 656c  ask Groups level
-00009060: 2075 7369 6e67 2074 6865 2061 6363 756d   using the accum
-00009070: 756c 6174 6564 2054 6173 6b20 5479 7065  ulated Task Type
-00009080: 7320 6672 6f6d 2074 6865 2054 6173 6b73  s from the Tasks
-00009090: 2069 6e63 6c75 6465 6420 696e 2065 6163   included in eac
-000090a0: 6820 5461 736b 2047 726f 7570 2c20 756e  h Task Group, un
-000090b0: 6c65 7373 206f 7665 7272 6964 6465 6e2e  less overridden.
-000090c0: 0a2d 2049 6620 6074 6173 6b54 7970 6573  .- If `taskTypes
-000090d0: 6020 6973 2073 6574 2061 7420 7468 6520  ` is set at the 
-000090e0: 5461 736b 2047 726f 7570 204c 6576 656c  Task Group Level
-000090f0: 2c20 616e 6420 6861 7320 6f6e 6c79 206f  , and has only o
-00009100: 6e65 2054 6173 6b20 5479 7065 2065 6e74  ne Task Type ent
-00009110: 7279 2c20 7468 656e 2060 7461 736b 5479  ry, then `taskTy
-00009120: 7065 6020 6973 2061 7574 6f6d 6174 6963  pe` is automatic
-00009130: 616c 6c79 2073 6574 2061 7420 7468 6520  ally set at the 
-00009140: 5461 736b 204c 6576 656c 2075 7369 6e67  Task Level using
-00009150: 2074 6865 2073 696e 676c 6520 5461 736b   the single Task
-00009160: 2054 7970 652c 2075 6e6c 6573 7320 6f76   Type, unless ov
-00009170: 6572 7269 6464 656e 2e0a 0a46 6f72 2074  erridden...For t
-00009180: 6865 202a 2a60 6261 7368 602a 2a2c 202a  he **`bash`**, *
-00009190: 2a60 706f 7765 7273 6865 6c6c 602a 2a2c  *`powershell`**,
-000091a0: 202a 2a60 636d 6460 2a2a 2f2a 2a60 6261   **`cmd`**/**`ba
-000091b0: 7460 2a2a 2061 6e64 202a 2a60 646f 636b  t`** and **`dock
-000091c0: 6572 602a 2a20 7461 736b 2074 7970 6573  er`** task types
-000091d0: 2c20 736f 6d65 2061 7574 6f6d 6174 6963  , some automatic
-000091e0: 2070 726f 6365 7373 696e 6720 7769 6c6c   processing will
-000091f0: 2062 6520 7065 7266 6f72 6d65 6420 6966   be performed if
-00009200: 2074 6865 202a 2a60 6578 6563 7574 6162   the **`executab
-00009210: 6c65 602a 2a20 7072 6f70 6572 7479 2069  le`** property i
-00009220: 7320 7365 742e 0a0a 2323 2323 2042 6173  s set...#### Bas
-00009230: 682c 2050 7974 686f 6e2c 2050 6f77 6572  h, Python, Power
-00009240: 5368 656c 6c20 616e 6420 636d 642f 6261  Shell and cmd/ba
-00009250: 7420 5461 736b 730a 0a41 7320 6120 636f  t Tasks..As a co
-00009260: 6e76 656e 6965 6e63 652c 2066 6f72 2074  nvenience, for t
-00009270: 6865 202a 2a60 6261 7368 602a 2a2c 202a  he **`bash`**, *
-00009280: 2a60 7079 7468 6f6e 602a 2a2c 202a 2a60  *`python`**, **`
-00009290: 706f 7765 7273 6865 6c6c 602a 2a2c 2061  powershell`**, a
-000092a0: 6e64 202a 2a60 636d 6460 2a2a 2028 6f72  nd **`cmd`** (or
-000092b0: 202a 2a60 6261 7460 2a2a 2920 5461 736b   **`bat`**) Task
-000092c0: 2054 7970 6573 2c20 7468 6520 7363 7269   Types, the scri
-000092d0: 7074 206e 6f6d 696e 6174 6564 2069 6e20  pt nominated in 
-000092e0: 7468 6520 2a2a 6065 7865 6375 7461 626c  the **`executabl
-000092f0: 6560 2a2a 2070 726f 7065 7274 7920 6973  e`** property is
-00009300: 2061 7574 6f6d 6174 6963 616c 6c79 2061   automatically a
-00009310: 6464 6564 2074 6f20 7468 6520 6069 6e70  dded to the `inp
-00009320: 7574 7360 206c 6973 7420 2869 6620 6e6f  uts` list (if no
-00009330: 7420 616c 7265 6164 7920 7072 6573 656e  t already presen
-00009340: 7429 2e20 5468 6973 206d 6561 6e73 2074  t). This means t
-00009350: 6865 2073 6372 6970 7420 6669 6c65 2077  he script file w
-00009360: 696c 6c20 6265 2075 706c 6f61 6465 6420  ill be uploaded 
-00009370: 746f 2074 6865 204f 626a 6563 7420 5374  to the Object St
-00009380: 6f72 652c 2061 6e64 206d 6164 6520 6120  ore, and made a 
-00009390: 7265 7175 6972 656d 656e 7420 6f66 2074  requirement of t
-000093a0: 6865 2054 6173 6b20 7768 656e 2069 7420  he Task when it 
-000093b0: 7275 6e73 2e0a 0a55 7369 6e67 2061 2042  runs...Using a B
-000093c0: 6173 6820 5461 736b 2061 7320 616e 2065  ash Task as an e
-000093d0: 7861 6d70 6c65 2028 696e 2054 4f4d 4c20  xample (in TOML 
-000093e0: 666f 726d 293a 0a0a 6060 6074 6f6d 6c0a  form):..```toml.
-000093f0: 7461 736b 5479 7065 203d 2022 6261 7368  taskType = "bash
-00009400: 220a 6578 6563 7574 6162 6c65 203d 2022  ".executable = "
-00009410: 6d79 5f62 6173 685f 7363 7269 7074 2e73  my_bash_script.s
-00009420: 6822 0a61 7267 756d 656e 7473 203d 205b  h".arguments = [
-00009430: 2231 222c 2022 3222 2c20 2233 225d 0a60  "1", "2", "3"].`
-00009440: 6060 0a69 7320 6571 7569 7661 6c65 6e74  ``.is equivalent
-00009450: 2074 6f3a 0a0a 6060 6074 6f6d 6c0a 7461   to:..```toml.ta
-00009460: 736b 5479 7065 203d 2022 6261 7368 220a  skType = "bash".
-00009470: 696e 7075 7473 203d 205b 226d 795f 6261  inputs = ["my_ba
-00009480: 7368 5f73 6372 6970 742e 7368 225d 0a61  sh_script.sh"].a
-00009490: 7267 756d 656e 7473 203d 205b 227b 7b77  rguments = ["{{w
-000094a0: 725f 6e61 6d65 7d7d 2f6d 795f 6261 7368  r_name}}/my_bash
-000094b0: 5f73 6372 6970 742e 7368 222c 2022 3122  _script.sh", "1"
-000094c0: 2c20 2232 222c 2022 3322 5d0a 6060 600a  , "2", "3"].```.
-000094d0: 0a49 6e20 7468 6520 6361 7365 206f 6620  .In the case of 
-000094e0: 5769 6e64 6f77 7320 6261 7463 6820 2860  Windows batch (`
-000094f0: 2e62 6174 6029 2066 696c 6573 2c20 6120  .bat`) files, a 
-00009500: 602f 6360 2066 6c61 6720 6973 2070 7265  `/c` flag is pre
-00009510: 7065 6e64 6564 2074 6f20 7468 6520 6063  pended to the `c
-00009520: 6d64 2e65 7865 6020 6172 6775 6d65 6e74  md.exe` argument
-00009530: 206c 6973 7420 746f 2065 6e73 7572 6520   list to ensure 
-00009540: 636f 7272 6563 7420 6578 6563 7574 696f  correct executio
-00009550: 6e20 6261 6861 7669 6f75 722e 2046 6f72  n bahaviour. For
-00009560: 2065 7861 6d70 6c65 3a0a 0a60 6060 746f   example:..```to
-00009570: 6d6c 0a74 6173 6b54 7970 6520 3d20 2263  ml.taskType = "c
-00009580: 6d64 2220 2023 206f 7220 2262 6174 220a  md"  # or "bat".
-00009590: 6578 6563 7574 6162 6c65 203d 2022 6d79  executable = "my
-000095a0: 5f73 6372 6970 742e 6261 7422 0a61 7267  _script.bat".arg
-000095b0: 756d 656e 7473 203d 205b 2231 222c 2022  uments = ["1", "
-000095c0: 3222 2c20 2233 225d 0a60 6060 0a0a 6973  2", "3"].```..is
-000095d0: 2065 7175 6976 616c 656e 7420 746f 3a0a   equivalent to:.
-000095e0: 0a60 6060 746f 6d6c 0a74 6173 6b54 7970  .```toml.taskTyp
-000095f0: 6520 3d20 2263 6d64 2220 2023 206f 7220  e = "cmd"  # or 
-00009600: 2262 6174 220a 696e 7075 7473 203d 205b  "bat".inputs = [
-00009610: 226d 795f 7363 7269 7074 2e62 6174 225d  "my_script.bat"]
-00009620: 0a61 7267 756d 656e 7473 203d 205b 222f  .arguments = ["/
-00009630: 6322 2c20 227b 7b77 725f 6e61 6d65 7d7d  c", "{{wr_name}}
-00009640: 5c5c 6d79 5f62 6173 685f 7363 7269 7074  \\my_bash_script
-00009650: 2e73 6822 2c20 2231 222c 2022 3222 2c20  .sh", "1", "2", 
-00009660: 2233 225d 0a60 6060 0a0a 2323 2323 2044  "3"].```..#### D
-00009670: 6f63 6b65 7220 5461 736b 730a 0a46 6f72  ocker Tasks..For
-00009680: 2074 6865 202a 2a60 646f 636b 6572 602a   the **`docker`*
-00009690: 2a20 5461 736b 2054 7970 652c 2074 6865  * Task Type, the
-000096a0: 2076 6172 6961 626c 6573 2073 7570 706c   variables suppl
-000096b0: 6965 6420 696e 2074 6865 2060 646f 636b  ied in the `dock
-000096c0: 6572 456e 7669 726f 6e6d 656e 7460 2070  erEnvironment` p
-000096d0: 726f 7065 7274 7920 6172 6520 756e 7061  roperty are unpa
-000096e0: 636b 6564 2069 6e74 6f20 7468 6520 6172  cked into the ar
-000096f0: 6775 6d65 6e74 206c 6973 7420 6173 2060  gument list as `
-00009700: 2d2d 656e 7660 2065 6e74 7269 6573 2c20  --env` entries, 
-00009710: 7468 6520 446f 636b 6572 2063 6f6e 7461  the Docker conta
-00009720: 696e 6572 206e 616d 6520 7375 7070 6c69  iner name suppli
-00009730: 6564 2069 6e20 7468 6520 6065 7865 6375  ed in the `execu
-00009740: 7461 626c 6560 2070 726f 7065 7274 7920  table` property 
-00009750: 6973 2074 6865 6e20 6164 6465 6420 746f  is then added to
-00009760: 2074 6865 2061 7267 756d 656e 7473 206c   the arguments l
-00009770: 6973 742c 2066 6f6c 6c6f 7765 6420 6279  ist, followed by
-00009780: 2074 6865 2061 7267 756d 656e 7473 2073   the arguments s
-00009790: 7570 706c 6965 6420 696e 2074 6865 2060  upplied in the `
-000097a0: 6172 6775 6d65 6e74 7360 2070 726f 7065  arguments` prope
-000097b0: 7274 792e 2054 6865 2060 646f 636b 6572  rty. The `docker
-000097c0: 5573 6572 6e61 6d65 6020 616e 6420 6064  Username` and `d
-000097d0: 6f63 6b65 7250 6173 7377 6f72 6460 2070  ockerPassword` p
-000097e0: 726f 7065 7274 6965 732c 2069 6620 7375  roperties, if su
-000097f0: 7070 6c69 6564 2c20 6172 6520 6164 6465  pplied, are adde
-00009800: 6420 746f 2074 6865 2060 656e 7669 726f  d to the `enviro
-00009810: 6e6d 656e 7460 2070 726f 7065 7274 792e  nment` property.
-00009820: 0a0a 466f 7220 6578 616d 706c 653a 0a60  ..For example:.`
-00009830: 6060 746f 6d6c 0a74 6173 6b54 7970 6520  ``toml.taskType 
-00009840: 3d20 2264 6f63 6b65 7222 0a65 7865 6375  = "docker".execu
-00009850: 7461 626c 6520 3d20 226d 795f 646f 636b  table = "my_dock
-00009860: 6572 6875 625f 7265 706f 2f6d 795f 636f  erhub_repo/my_co
-00009870: 6e74 6169 6e65 725f 696d 6167 6522 0a64  ntainer_image".d
-00009880: 6f63 6b65 7245 6e76 6972 6f6e 6d65 6e74  ockerEnvironment
-00009890: 203d 207b 4531 203d 2022 4565 654f 6e65   = {E1 = "EeeOne
-000098a0: 227d 0a64 6f63 6b65 7255 7365 726e 616d  "}.dockerUsernam
-000098b0: 6520 3d20 226d 795f 7573 6572 220a 646f  e = "my_user".do
-000098c0: 636b 6572 5061 7373 776f 7264 203d 2022  ckerPassword = "
-000098d0: 6d79 5f70 6173 7377 6f72 6422 0a61 7267  my_password".arg
-000098e0: 756d 656e 7473 203d 205b 2231 222c 2022  uments = ["1", "
-000098f0: 3222 2c20 2233 225d 0a60 6060 0a0a 6973  2", "3"].```..is
-00009900: 2065 7175 6976 616c 656e 7420 746f 2074   equivalent to t
-00009910: 6865 2066 6f6c 6c6f 7769 6e67 2062 6569  he following bei
-00009920: 6e67 2073 656e 7420 666f 7220 7072 6f63  ng sent for proc
-00009930: 6573 7369 6e67 2062 7920 7468 6520 6064  essing by the `d
-00009940: 6f63 6b65 7260 2054 6173 6b20 5479 7065  ocker` Task Type
-00009950: 2c20 7468 6520 5965 6c6c 6f77 446f 6720  , the YellowDog 
-00009960: 7665 7273 696f 6e20 6f66 2077 6869 6368  version of which
-00009970: 2077 696c 6c20 6c6f 6720 696e 2074 6f20   will log in to 
-00009980: 7468 6520 446f 636b 6572 2072 6570 6f20  the Docker repo 
-00009990: 2869 6620 7265 7175 6972 6564 2920 7468  (if required) th
-000099a0: 656e 2069 7373 7565 2061 2060 646f 636b  en issue a `dock
-000099b0: 6572 2072 756e 6020 636f 6d6d 616e 6420  er run` command 
-000099c0: 7769 7468 2074 6865 2061 7267 756d 656e  with the argumen
-000099d0: 7473 2073 7570 706c 6965 643a 0a0a 6060  ts supplied:..``
-000099e0: 6074 6f6d 6c0a 7461 736b 5479 7065 203d  `toml.taskType =
-000099f0: 2022 646f 636b 6572 220a 6172 6775 6d65   "docker".argume
-00009a00: 6e74 7320 3d20 5b22 2d2d 656e 7620 4531  nts = ["--env E1
-00009a10: 3d45 6565 4f6e 6522 2c20 226d 795f 646f  =EeeOne", "my_do
-00009a20: 636b 6572 6875 6272 6570 6f2f 6d79 5f63  ckerhubrepo/my_c
-00009a30: 6f6e 7461 696e 6572 5f69 6d61 6765 222c  ontainer_image",
-00009a40: 2022 3122 2c20 2232 222c 2022 3322 5d0a   "1", "2", "3"].
-00009a50: 656e 7669 726f 6e6d 656e 7420 3d20 7b44  environment = {D
-00009a60: 4f43 4b45 525f 5553 4552 4e41 4d45 203d  OCKER_USERNAME =
-00009a70: 2022 6d79 5f75 7365 7222 2c20 444f 434b   "my_user", DOCK
-00009a80: 4552 5f50 4153 5357 4f52 4420 3d20 226d  ER_PASSWORD = "m
-00009a90: 795f 7061 7373 776f 7264 227d 0a60 6060  y_password"}.```
-00009aa0: 0a0a 2323 2323 2042 6173 682c 2050 7974  ..#### Bash, Pyt
-00009ab0: 686f 6e2c 2050 6f77 6572 5368 656c 6c2c  hon, PowerShell,
-00009ac0: 2063 6d64 2f62 6174 2061 6e64 2044 6f63   cmd/bat and Doc
-00009ad0: 6b65 7220 7769 7468 6f75 7420 4175 746f  ker without Auto
-00009ae0: 6d61 7469 6320 5072 6f63 6573 7369 6e67  matic Processing
-00009af0: 0a0a 4966 2074 6865 2060 6578 6563 7574  ..If the `execut
-00009b00: 6162 6c65 6020 7072 6f70 6572 7479 2069  able` property i
-00009b10: 7320 6e6f 7420 7375 7070 6c69 6564 2c20  s not supplied, 
-00009b20: 7468 6520 6175 746f 6d61 7469 6320 7072  the automatic pr
-00009b30: 6f63 6573 7369 6e67 2064 6573 6372 6962  ocessing describ
-00009b40: 6564 2061 626f 7665 2066 6f72 2060 6261  ed above for `ba
-00009b50: 7368 602c 2060 7079 7468 6f6e 602c 2060  sh`, `python`, `
-00009b60: 706f 7765 7273 6865 6c6c 602c 2060 636d  powershell`, `cm
-00009b70: 6460 2028 6f72 2060 6261 7460 2920 616e  d` (or `bat`) an
-00009b80: 6420 6064 6f63 6b65 7260 2074 6173 6b20  d `docker` task 
-00009b90: 7479 7065 7320 6973 206e 6f74 2061 7070  types is not app
-00009ba0: 6c69 6564 2e0a 0a23 2323 2054 6173 6b20  lied...### Task 
-00009bb0: 436f 756e 7473 0a0a 5468 6973 2070 726f  Counts..This pro
-00009bc0: 7065 7274 7920 7769 6c6c 2065 7870 616e  perty will expan
-00009bd0: 6420 7468 6520 6e75 6d62 6572 206f 6620  d the number of 
-00009be0: 5461 736b 7320 746f 206d 6174 6368 2060  Tasks to match `
-00009bf0: 7461 736b 436f 756e 7460 2e0a 0a54 6865  taskCount`...The
-00009c00: 2060 7461 736b 436f 756e 7460 2070 726f   `taskCount` pro
-00009c10: 7065 7274 7920 6361 6e20 6265 2073 6574  perty can be set
-00009c20: 206f 6e6c 7920 696e 2074 6865 2060 776f   only in the `wo
-00009c30: 726b 5265 7175 6972 656d 656e 7460 2073  rkRequirement` s
-00009c40: 6563 7469 6f6e 206f 6620 7468 6520 6063  ection of the `c
-00009c50: 6f6e 6669 672e 746f 6d6c 6020 6669 6c65  onfig.toml` file
-00009c60: 2c20 6f72 2069 6e20 7468 6520 6074 6173  , or in the `tas
-00009c70: 6b47 726f 7570 6020 7365 6374 696f 6e28  kGroup` section(
-00009c80: 7329 206f 6620 6120 4a53 4f4e 2057 6f72  s) of a JSON Wor
-00009c90: 6b20 5265 7175 6972 656d 656e 7420 6465  k Requirement de
-00009ca0: 6669 6e69 7469 6f6e 2e0a 0a49 6e20 7468  finition...In th
-00009cb0: 6520 666f 726d 6572 2063 6173 652c 2074  e former case, t
-00009cc0: 6865 2060 7461 736b 436f 756e 7460 2061  he `taskCount` a
-00009cd0: 7070 6c69 6573 206f 6e6c 7920 746f 2074  pplies only to t
-00009ce0: 6865 2054 6173 6b20 7370 6563 6966 6965  he Task specifie
-00009cf0: 6420 7769 7468 696e 2074 6865 2060 636f  d within the `co
-00009d00: 6e66 6967 2e74 6f6d 6c60 2066 696c 6520  nfig.toml` file 
-00009d10: 616e 6420 6973 206e 6f74 2069 6e68 6572  and is not inher
-00009d20: 6974 6564 2062 7920 4a53 4f4e 2057 6f72  ited by JSON Wor
-00009d30: 6b20 5265 7175 6972 656d 656e 7420 7370  k Requirement sp
-00009d40: 6563 6966 6963 6174 696f 6e73 2e0a 0a49  ecifications...I
-00009d50: 6e20 7468 6520 6c61 7474 6572 2063 6173  n the latter cas
-00009d60: 652c 2074 6865 2060 7461 736b 436f 756e  e, the `taskCoun
-00009d70: 7460 2061 7070 6c69 6573 2074 6f20 7468  t` applies to th
-00009d80: 6520 5461 736b 2073 7065 6369 6669 6564  e Task specified
-00009d90: 2077 6974 6869 6e20 7468 6520 5461 736b   within the Task
-00009da0: 2047 726f 7570 2c20 616e 6420 7468 6572   Group, and ther
-00009db0: 6520 6d75 7374 2062 6520 7a65 726f 206f  e must be zero o
-00009dc0: 7220 6f6e 6520 5461 736b 2873 2920 6c69  r one Task(s) li
-00009dd0: 7374 6564 2077 6974 6869 6e20 7468 6520  sted within the 
-00009de0: 6772 6f75 7020 6f72 2060 7461 736b 436f  group or `taskCo
-00009df0: 756e 7460 2069 7320 6967 6e6f 7265 642e  unt` is ignored.
-00009e00: 0a0a 2323 2045 7861 6d70 6c65 730a 0a23  ..## Examples..#
-00009e10: 2323 2054 4f4d 4c20 5072 6f70 6572 7469  ## TOML Properti
-00009e20: 6573 2069 6e20 7468 6520 6077 6f72 6b52  es in the `workR
-00009e30: 6571 7569 7265 6d65 6e74 6020 5365 6374  equirement` Sect
-00009e40: 696f 6e0a 0a48 6572 6527 7320 616e 2065  ion..Here's an e
-00009e50: 7861 6d70 6c65 206f 6620 7468 6520 6077  xample of the `w
-00009e60: 6f72 6b52 6571 7569 7265 6d65 6e74 6020  orkRequirement` 
-00009e70: 7365 6374 696f 6e20 6f66 2061 2054 4f4d  section of a TOM
-00009e80: 4c20 636f 6e66 6967 7572 6174 696f 6e20  L configuration 
-00009e90: 6669 6c65 2c20 7368 6f77 696e 6720 616c  file, showing al
-00009ea0: 6c20 7468 6520 706f 7373 6962 6c65 2070  l the possible p
-00009eb0: 726f 7065 7274 6965 7320 7468 6174 2063  roperties that c
-00009ec0: 616e 2062 6520 7365 743a 0a0a 6060 6074  an be set:..```t
-00009ed0: 6f6d 6c0a 5b77 6f72 6b52 6571 7569 7265  oml.[workRequire
-00009ee0: 6d65 6e74 5d0a 2020 2020 6172 6775 6d65  ment].    argume
-00009ef0: 6e74 7320 3d20 5b22 3122 2c20 2254 574f  nts = ["1", "TWO
-00009f00: 225d 0a20 2020 2063 6170 7475 7265 5461  "].    captureTa
-00009f10: 736b 4f75 7470 7574 203d 2074 7275 650a  skOutput = true.
-00009f20: 2020 2020 636f 6d70 6c65 7465 6454 6173      completedTas
-00009f30: 6b54 746c 203d 2031 300a 2020 2020 6373  kTtl = 10.    cs
-00009f40: 7646 696c 6520 3d20 2266 696c 6531 2e63  vFile = "file1.c
-00009f50: 7376 220a 2020 2020 6373 7646 696c 6573  sv".    csvFiles
-00009f60: 203d 205b 2266 696c 6531 2e63 7376 222c   = ["file1.csv",
-00009f70: 2022 6669 6c65 332e 6373 763a 3322 5d0a   "file3.csv:3"].
-00009f80: 2020 2020 646f 636b 6572 456e 7669 726f      dockerEnviro
-00009f90: 6e6d 656e 7420 3d20 7b4d 595f 444f 434b  nment = {MY_DOCK
-00009fa0: 4552 5f56 4152 203d 2031 3030 7d0a 2020  ER_VAR = 100}.  
-00009fb0: 2020 646f 636b 6572 5061 7373 776f 7264    dockerPassword
-00009fc0: 203d 2022 6d79 5061 7373 776f 7264 220a   = "myPassword".
-00009fd0: 2020 2020 646f 636b 6572 5573 6572 6e61      dockerUserna
-00009fe0: 6d65 203d 2022 6d79 5573 6572 6e61 6d65  me = "myUsername
-00009ff0: 220a 2020 2020 656e 7669 726f 6e6d 656e  ".    environmen
-0000a000: 7420 3d20 7b4d 595f 5641 5220 3d20 3130  t = {MY_VAR = 10
-0000a010: 307d 0a20 2020 2065 7863 6c75 7369 7665  0}.    exclusive
-0000a020: 576f 726b 6572 7320 3d20 6661 6c73 650a  Workers = false.
-0000a030: 2020 2020 6578 6563 7574 6162 6c65 203d      executable =
-0000a040: 2022 6d79 2d63 6f6e 7461 696e 6572 220a   "my-container".
-0000a050: 2020 2020 6669 6e69 7368 4966 416c 6c54      finishIfAllT
-0000a060: 6173 6b73 4669 6e69 7368 6564 203d 2074  asksFinished = t
-0000a070: 7275 650a 2020 2020 6669 6e69 7368 4966  rue.    finishIf
-0000a080: 416e 7954 6173 6b46 6169 6c65 6420 3d20  AnyTaskFailed = 
-0000a090: 6661 6c73 650a 2020 2020 666c 6174 7465  false.    flatte
-0000a0a0: 6e49 6e70 7574 5061 7468 7320 3d20 6661  nInputPaths = fa
-0000a0b0: 6c73 650a 2020 2020 666c 6174 7465 6e55  lse.    flattenU
-0000a0c0: 706c 6f61 6450 6174 6873 203d 2066 616c  ploadPaths = fal
-0000a0d0: 7365 0a20 2020 2066 756c 6669 6c4f 6e53  se.    fulfilOnS
-0000a0e0: 7562 6d69 7420 3d20 6661 6c73 650a 2020  ubmit = false.  
-0000a0f0: 2020 696e 7075 7473 203d 205b 0a20 2020    inputs = [.   
-0000a100: 2020 2020 2022 2e2e 2f61 7070 2f6d 6169       "../app/mai
-0000a110: 6e2e 7079 222c 0a20 2020 2020 2020 2022  n.py",.        "
-0000a120: 2e2e 2f61 7070 2f72 6571 7569 7265 6d65  ../app/requireme
-0000a130: 6e74 732e 7478 7422 0a20 2020 205d 0a20  nts.txt".    ]. 
-0000a140: 2020 2069 6e70 7574 734f 7074 696f 6e61     inputsOptiona
-0000a150: 6c20 3d20 5b22 6f70 7469 6f6e 616c 2e74  l = ["optional.t
-0000a160: 7874 225d 0a20 2020 2069 6e73 7461 6e63  xt"].    instanc
-0000a170: 6554 7970 6573 203d 205b 2274 3361 2e6d  eTypes = ["t3a.m
-0000a180: 6963 726f 222c 2022 7433 2e6d 6963 726f  icro", "t3.micro
-0000a190: 225d 0a20 2020 206d 6178 576f 726b 6572  "].    maxWorker
-0000a1a0: 7320 3d20 310a 2020 2020 6d61 7869 6d75  s = 1.    maximu
-0000a1b0: 6d54 6173 6b52 6574 7269 6573 203d 2030  mTaskRetries = 0
-0000a1c0: 0a20 2020 206d 696e 576f 726b 6572 7320  .    minWorkers 
-0000a1d0: 3d20 310a 2020 2020 6e61 6d65 203d 2022  = 1.    name = "
-0000a1e0: 6d79 2d77 6f72 6b2d 7265 7175 6972 656d  my-work-requirem
-0000a1f0: 656e 7422 0a20 2020 206f 7574 7075 7473  ent".    outputs
-0000a200: 203d 205b 2272 6573 756c 7473 2e74 7874   = ["results.txt
-0000a210: 225d 0a20 2020 206f 7574 7075 7473 5265  "].    outputsRe
-0000a220: 7175 6972 6564 203d 205b 2272 6573 756c  quired = ["resul
-0000a230: 7473 5f72 6571 7569 7265 642e 7478 7422  ts_required.txt"
-0000a240: 5d0a 2020 2020 7072 696f 7269 7479 203d  ].    priority =
-0000a250: 2030 2e30 0a20 2020 2070 726f 7669 6465   0.0.    provide
-0000a260: 7273 203d 205b 2241 5753 225d 0a20 2020  rs = ["AWS"].   
-0000a270: 2072 616d 203d 205b 302e 352c 2032 2e30   ram = [0.5, 2.0
-0000a280: 5d0a 2020 2020 7265 6769 6f6e 7320 3d20  ].    regions = 
-0000a290: 5b22 6575 2d77 6573 742d 3222 5d0a 2020  ["eu-west-2"].  
-0000a2a0: 2020 7461 736b 4261 7463 6853 697a 6520    taskBatchSize 
-0000a2b0: 3d20 3130 3030 0a20 2020 2074 6173 6b43  = 1000.    taskC
-0000a2c0: 6f75 6e74 203d 2031 3030 0a20 2020 2074  ount = 100.    t
-0000a2d0: 6173 6b44 6174 6120 3d20 226d 795f 6461  askData = "my_da
-0000a2e0: 7461 5f73 7472 696e 6722 0a20 2020 2074  ta_string".    t
-0000a2f0: 6173 6b44 6174 6146 696c 6520 3d20 226d  askDataFile = "m
-0000a300: 795f 6461 7461 5f66 696c 652e 7478 7422  y_data_file.txt"
-0000a310: 0a20 2020 2074 6173 6b4e 616d 6520 3d20  .    taskName = 
-0000a320: 226d 795f 7461 736b 5f6e 756d 6265 725f  "my_task_number_
-0000a330: 7b7b 7461 736b 5f6e 756d 6265 727d 7d22  {{task_number}}"
-0000a340: 0a20 2020 2074 6173 6b47 726f 7570 4e61  .    taskGroupNa
-0000a350: 6d65 203d 2022 6d79 5f74 6173 6b5f 6772  me = "my_task_gr
-0000a360: 6f75 705f 6e75 6d62 6572 5f7b 7b74 6173  oup_number_{{tas
-0000a370: 6b5f 6772 6f75 705f 6e75 6d62 6572 7d7d  k_group_number}}
-0000a380: 220a 2020 2020 7461 736b 5479 7065 203d  ".    taskType =
-0000a390: 2022 646f 636b 6572 220a 2020 2020 7461   "docker".    ta
-0000a3a0: 736b 7350 6572 576f 726b 6572 203d 2031  sksPerWorker = 1
-0000a3b0: 0a20 2020 2075 706c 6f61 6446 696c 6573  .    uploadFiles
-0000a3c0: 203d 205b 7b6c 6f63 616c 5061 7468 203d   = [{localPath =
-0000a3d0: 2022 6669 6c65 5f31 2e74 7874 222c 2075   "file_1.txt", u
-0000a3e0: 706c 6f61 6450 6174 6820 3d20 2266 696c  ploadPath = "fil
-0000a3f0: 655f 312e 7478 7422 7d5d 0a20 2020 2076  e_1.txt"}].    v
-0000a400: 6370 7573 203d 205b 312c 2034 5d0a 2020  cpus = [1, 4].  
-0000a410: 2020 7665 7269 6679 4174 5374 6172 7420    verifyAtStart 
-0000a420: 3d20 5b22 7265 6164 795f 7265 7375 6c74  = ["ready_result
-0000a430: 732e 7478 7422 5d0a 2020 2020 7665 7269  s.txt"].    veri
-0000a440: 6679 5761 6974 203d 205b 2277 6169 745f  fyWait = ["wait_
-0000a450: 666f 725f 7265 7375 6c74 732e 7478 7422  for_results.txt"
-0000a460: 5d0a 2020 2020 776f 726b 6572 5461 6773  ].    workerTags
-0000a470: 203d 205b 2274 6167 2d7b 7b75 7365 726e   = ["tag-{{usern
-0000a480: 616d 657d 7d22 5d0a 2020 2020 776f 726b  ame}}"].    work
-0000a490: 5265 7175 6972 656d 656e 7444 6174 6120  RequirementData 
-0000a4a0: 3d20 2277 6f72 6b5f 7265 7175 6972 656d  = "work_requirem
-0000a4b0: 656e 742e 6a73 6f6e 220a 6060 600a 0a23  ent.json".```..#
-0000a4c0: 2323 204a 534f 4e20 5072 6f70 6572 7469  ## JSON Properti
-0000a4d0: 6573 2061 7420 7468 6520 576f 726b 2052  es at the Work R
-0000a4e0: 6571 7569 7265 6d65 6e74 204c 6576 656c  equirement Level
-0000a4f0: 0a0a 5368 6f77 696e 6720 616c 6c20 706f  ..Showing all po
-0000a500: 7373 6962 6c65 2070 726f 7065 7274 6965  ssible propertie
-0000a510: 7320 6174 2074 6865 2057 6f72 6b20 5265  s at the Work Re
-0000a520: 7175 6972 656d 656e 7420 6c65 7665 6c3a  quirement level:
-0000a530: 0a0a 6060 606a 736f 6e0a 7b0a 2020 2261  ..```json.{.  "a
-0000a540: 7267 756d 656e 7473 223a 205b 312c 2022  rguments": [1, "
-0000a550: 5457 4f22 5d2c 0a20 2022 6361 7074 7572  TWO"],.  "captur
-0000a560: 6554 6173 6b4f 7574 7075 7422 3a20 7472  eTaskOutput": tr
-0000a570: 7565 2c0a 2020 2263 6f6d 706c 6574 6564  ue,.  "completed
-0000a580: 5461 736b 5474 6c22 3a20 3130 2c0a 2020  TaskTtl": 10,.  
-0000a590: 2264 6f63 6b65 7245 6e76 6972 6f6e 6d65  "dockerEnvironme
-0000a5a0: 6e74 223a 207b 224d 595f 444f 434b 4552  nt": {"MY_DOCKER
-0000a5b0: 5f56 4152 223a 2031 3030 7d2c 0a20 2022  _VAR": 100},.  "
-0000a5c0: 646f 636b 6572 5061 7373 776f 7264 223a  dockerPassword":
-0000a5d0: 2022 6d79 5061 7373 776f 7264 222c 0a20   "myPassword",. 
-0000a5e0: 2022 646f 636b 6572 5573 6572 6e61 6d65   "dockerUsername
-0000a5f0: 223a 2022 6d79 5573 6572 6e61 6d65 222c  ": "myUsername",
-0000a600: 0a20 2022 656e 7669 726f 6e6d 656e 7422  .  "environment"
-0000a610: 3a20 7b22 4d59 5f56 4152 223a 2031 3030  : {"MY_VAR": 100
-0000a620: 7d2c 0a20 2022 6578 636c 7573 6976 6557  },.  "exclusiveW
-0000a630: 6f72 6b65 7273 223a 2066 616c 7365 2c0a  orkers": false,.
-0000a640: 2020 2265 7865 6375 7461 626c 6522 3a20    "executable": 
-0000a650: 226d 792d 636f 6e74 6169 6e65 7222 2c0a  "my-container",.
-0000a660: 2020 2266 696e 6973 6849 6641 6c6c 5461    "finishIfAllTa
-0000a670: 736b 7346 696e 6973 6865 6422 3a20 7472  sksFinished": tr
-0000a680: 7565 2c0a 2020 2266 696e 6973 6849 6641  ue,.  "finishIfA
-0000a690: 6e79 5461 736b 4661 696c 6564 223a 2066  nyTaskFailed": f
-0000a6a0: 616c 7365 2c0a 2020 2266 6c61 7474 656e  alse,.  "flatten
-0000a6b0: 496e 7075 7450 6174 6873 223a 2066 616c  InputPaths": fal
-0000a6c0: 7365 2c0a 2020 2266 6c61 7474 656e 5570  se,.  "flattenUp
-0000a6d0: 6c6f 6164 5061 7468 7322 3a20 6661 6c73  loadPaths": fals
-0000a6e0: 652c 0a20 2022 6675 6c66 696c 4f6e 5375  e,.  "fulfilOnSu
-0000a6f0: 626d 6974 223a 2066 616c 7365 2c0a 2020  bmit": false,.  
-0000a700: 2269 6e70 7574 7322 3a20 5b22 6170 702f  "inputs": ["app/
-0000a710: 6d61 696e 2e70 7922 2c20 2261 7070 2f72  main.py", "app/r
-0000a720: 6571 7569 7265 6d65 6e74 732e 7478 7422  equirements.txt"
-0000a730: 5d2c 0a20 2022 696e 7075 7473 4f70 7469  ],.  "inputsOpti
-0000a740: 6f6e 616c 223a 205b 226f 7074 696f 6e61  onal": ["optiona
-0000a750: 6c2e 7478 7422 5d2c 0a20 2022 696e 7374  l.txt"],.  "inst
-0000a760: 616e 6365 5479 7065 7322 3a20 5b22 7433  anceTypes": ["t3
-0000a770: 612e 6d69 6372 6f22 2c20 2274 332e 6d69  a.micro", "t3.mi
-0000a780: 6372 6f22 5d2c 0a20 2022 6d61 7857 6f72  cro"],.  "maxWor
-0000a790: 6b65 7273 223a 2031 2c0a 2020 226d 6178  kers": 1,.  "max
-0000a7a0: 696d 756d 5461 736b 5265 7472 6965 7322  imumTaskRetries"
-0000a7b0: 3a20 302c 0a20 2022 6d69 6e57 6f72 6b65  : 0,.  "minWorke
-0000a7c0: 7273 223a 2031 2c0a 2020 226e 616d 6522  rs": 1,.  "name"
-0000a7d0: 3a20 226d 792d 776f 726b 2d72 6571 7569  : "my-work-requi
-0000a7e0: 7265 6d65 6e74 222c 0a20 2022 6f75 7470  rement",.  "outp
-0000a7f0: 7574 7322 3a20 5b22 7265 7375 6c74 732e  uts": ["results.
-0000a800: 7478 7422 5d2c 0a20 2022 6f75 7470 7574  txt"],.  "output
-0000a810: 7352 6571 7569 7265 6422 3a20 5b22 7265  sRequired": ["re
-0000a820: 7375 6c74 735f 7265 7175 6972 6564 2e74  sults_required.t
-0000a830: 7874 225d 2c0a 2020 2270 7269 6f72 6974  xt"],.  "priorit
-0000a840: 7922 3a20 302e 302c 0a20 2022 7072 6f76  y": 0.0,.  "prov
-0000a850: 6964 6572 7322 3a20 5b22 4157 5322 5d2c  iders": ["AWS"],
-0000a860: 0a20 2022 7261 6d22 3a20 5b30 2e35 2c20  .  "ram": [0.5, 
-0000a870: 325d 2c0a 2020 2272 6567 696f 6e73 223a  2],.  "regions":
-0000a880: 205b 2265 752d 7765 7374 2d32 225d 2c0a   ["eu-west-2"],.
-0000a890: 2020 2274 6173 6b44 6174 6122 3a20 226d    "taskData": "m
-0000a8a0: 795f 7461 736b 5f64 6174 615f 7374 7269  y_task_data_stri
-0000a8b0: 6e67 222c 0a20 2022 7461 736b 4461 7461  ng",.  "taskData
-0000a8c0: 4669 6c65 223a 2022 6d79 5f64 6174 615f  File": "my_data_
-0000a8d0: 6669 6c65 2e74 7874 222c 0a20 2022 7461  file.txt",.  "ta
-0000a8e0: 736b 5479 7065 7322 3a20 5b22 646f 636b  skTypes": ["dock
-0000a8f0: 6572 225d 2c0a 2020 2274 6173 6b73 5065  er"],.  "tasksPe
-0000a900: 7257 6f72 6b65 7222 3a20 312c 0a20 2022  rWorker": 1,.  "
-0000a910: 7570 6c6f 6164 4669 6c65 7322 3a20 5b7b  uploadFiles": [{
-0000a920: 226c 6f63 616c 5061 7468 223a 2022 6669  "localPath": "fi
-0000a930: 6c65 5f31 2e74 7874 222c 2022 7570 6c6f  le_1.txt", "uplo
-0000a940: 6164 5061 7468 223a 2022 6669 6c65 5f31  adPath": "file_1
-0000a950: 2e74 7874 227d 5d2c 0a20 2022 7663 7075  .txt"}],.  "vcpu
-0000a960: 7322 3a20 5b31 2c20 345d 2c0a 2020 2276  s": [1, 4],.  "v
-0000a970: 6572 6966 7941 7453 7461 7274 223a 205b  erifyAtStart": [
-0000a980: 2272 6561 6479 5f72 6573 756c 7473 2e74  "ready_results.t
-0000a990: 7874 225d 2c0a 2020 2276 6572 6966 7957  xt"],.  "verifyW
-0000a9a0: 6169 7422 3a20 5b22 7761 6974 5f66 6f72  ait": ["wait_for
-0000a9b0: 5f72 6573 756c 7473 2e74 7874 225d 2c0a  _results.txt"],.
-0000a9c0: 2020 2277 6f72 6b65 7254 6167 7322 3a20    "workerTags": 
-0000a9d0: 5b5d 2c0a 2020 2274 6173 6b47 726f 7570  [],.  "taskGroup
-0000a9e0: 7322 3a20 5b0a 2020 2020 7b0a 2020 2020  s": [.    {.    
-0000a9f0: 2020 2274 6173 6b73 223a 205b 0a20 2020    "tasks": [.   
-0000aa00: 2020 2020 207b 7d0a 2020 2020 2020 5d0a       {}.      ].
-0000aa10: 2020 2020 7d0a 2020 5d0a 7d0a 0a60 6060      }.  ].}..```
-0000aa20: 0a0a 2323 2320 4a53 4f4e 2050 726f 7065  ..### JSON Prope
-0000aa30: 7274 6965 7320 6174 2074 6865 2054 6173  rties at the Tas
-0000aa40: 6b20 4772 6f75 7020 4c65 7665 6c0a 0a53  k Group Level..S
-0000aa50: 686f 7769 6e67 2061 6c6c 2070 6f73 7369  howing all possi
-0000aa60: 626c 6520 7072 6f70 6572 7469 6573 2061  ble properties a
-0000aa70: 7420 7468 6520 5461 736b 2047 726f 7570  t the Task Group
-0000aa80: 206c 6576 656c 3a0a 0a60 6060 6a73 6f6e   level:..```json
-0000aa90: 0a7b 0a20 2022 7461 736b 4772 6f75 7073  .{.  "taskGroups
-0000aaa0: 223a 205b 0a20 2020 207b 0a20 2020 2020  ": [.    {.     
-0000aab0: 2022 6172 6775 6d65 6e74 7322 3a20 5b31   "arguments": [1
-0000aac0: 2c20 2254 574f 225d 2c0a 2020 2020 2020  , "TWO"],.      
-0000aad0: 2263 6170 7475 7265 5461 736b 4f75 7470  "captureTaskOutp
-0000aae0: 7574 223a 2074 7275 652c 0a20 2020 2020  ut": true,.     
-0000aaf0: 2022 636f 6d70 6c65 7465 6454 6173 6b54   "completedTaskT
-0000ab00: 746c 223a 2031 302c 0a20 2020 2020 2022  tl": 10,.      "
-0000ab10: 646f 636b 6572 456e 7669 726f 6e6d 656e  dockerEnvironmen
-0000ab20: 7422 3a20 7b22 4d59 5f44 4f43 4b45 525f  t": {"MY_DOCKER_
-0000ab30: 5641 5222 3a20 3130 307d 2c0a 2020 2020  VAR": 100},.    
-0000ab40: 2020 2264 6f63 6b65 7250 6173 7377 6f72    "dockerPasswor
-0000ab50: 6422 3a20 226d 7950 6173 7377 6f72 6422  d": "myPassword"
-0000ab60: 2c0a 2020 2020 2020 2264 6f63 6b65 7255  ,.      "dockerU
-0000ab70: 7365 726e 616d 6522 3a20 226d 7955 7365  sername": "myUse
-0000ab80: 726e 616d 6522 2c0a 2020 2020 2020 2265  rname",.      "e
-0000ab90: 6e76 6972 6f6e 6d65 6e74 223a 207b 224d  nvironment": {"M
-0000aba0: 595f 5641 5222 3a20 3130 307d 2c0a 2020  Y_VAR": 100},.  
-0000abb0: 2020 2020 2265 7863 6c75 7369 7665 576f      "exclusiveWo
-0000abc0: 726b 6572 7322 3a20 6661 6c73 652c 0a20  rkers": false,. 
-0000abd0: 2020 2020 2022 6578 6563 7574 6162 6c65       "executable
-0000abe0: 223a 2022 6d79 2d63 6f6e 7461 696e 6572  ": "my-container
-0000abf0: 222c 0a20 2020 2020 2022 6669 6e69 7368  ",.      "finish
-0000ac00: 4966 416c 6c54 6173 6b73 4669 6e69 7368  IfAllTasksFinish
-0000ac10: 6564 223a 2074 7275 652c 0a20 2020 2020  ed": true,.     
-0000ac20: 2022 6669 6e69 7368 4966 416e 7954 6173   "finishIfAnyTas
-0000ac30: 6b46 6169 6c65 6422 3a20 6661 6c73 652c  kFailed": false,
-0000ac40: 0a20 2020 2020 2022 666c 6174 7465 6e49  .      "flattenI
-0000ac50: 6e70 7574 5061 7468 7322 3a20 6661 6c73  nputPaths": fals
-0000ac60: 652c 0a20 2020 2020 2022 696e 7075 7473  e,.      "inputs
-0000ac70: 223a 205b 2261 7070 2f6d 6169 6e2e 7079  ": ["app/main.py
-0000ac80: 222c 2022 6170 702f 7265 7175 6972 656d  ", "app/requirem
-0000ac90: 656e 7473 2e74 7874 225d 2c0a 2020 2020  ents.txt"],.    
-0000aca0: 2020 2269 6e70 7574 734f 7074 696f 6e61    "inputsOptiona
-0000acb0: 6c22 3a20 5b22 6f70 7469 6f6e 616c 2e74  l": ["optional.t
-0000acc0: 7874 225d 2c0a 2020 2020 2020 2269 6e73  xt"],.      "ins
-0000acd0: 7461 6e63 6554 7970 6573 223a 205b 2274  tanceTypes": ["t
-0000ace0: 3361 2e6d 6963 726f 222c 2022 7433 2e6d  3a.micro", "t3.m
-0000acf0: 6963 726f 225d 2c0a 2020 2020 2020 226d  icro"],.      "m
-0000ad00: 6178 696d 756d 5461 736b 5265 7472 6965  aximumTaskRetrie
-0000ad10: 7322 3a20 302c 0a20 2020 2020 2022 6d61  s": 0,.      "ma
-0000ad20: 7857 6f72 6b65 7273 223a 2031 2c0a 2020  xWorkers": 1,.  
-0000ad30: 2020 2020 226d 696e 576f 726b 6572 7322      "minWorkers"
-0000ad40: 3a20 312c 0a20 2020 2020 2022 6e61 6d65  : 1,.      "name
-0000ad50: 223a 2022 6669 7273 742d 7461 736b 2d67  ": "first-task-g
-0000ad60: 726f 7570 222c 0a20 2020 2020 2022 6f75  roup",.      "ou
-0000ad70: 7470 7574 7322 3a20 5b22 7265 7375 6c74  tputs": ["result
-0000ad80: 732e 7478 7422 5d2c 0a20 2020 2020 2022  s.txt"],.      "
-0000ad90: 6f75 7470 7574 7352 6571 7569 7265 6422  outputsRequired"
-0000ada0: 3a20 5b22 7265 7375 6c74 735f 7265 7175  : ["results_requ
-0000adb0: 6972 6564 2e74 7874 225d 2c0a 2020 2020  ired.txt"],.    
-0000adc0: 2020 2270 7269 6f72 6974 7922 3a20 302e    "priority": 0.
-0000add0: 302c 0a20 2020 2020 2022 7072 6f76 6964  0,.      "provid
-0000ade0: 6572 7322 3a20 5b22 4157 5322 5d2c 0a20  ers": ["AWS"],. 
-0000adf0: 2020 2020 2022 7261 6d22 3a20 5b30 2e35       "ram": [0.5
-0000ae00: 2c20 325d 2c0a 2020 2020 2020 2272 6567  , 2],.      "reg
-0000ae10: 696f 6e73 223a 205b 2265 752d 7765 7374  ions": ["eu-west
-0000ae20: 2d32 225d 2c0a 2020 2020 2020 2274 6173  -2"],.      "tas
-0000ae30: 6b43 6f75 6e74 223a 2035 2c0a 2020 2020  kCount": 5,.    
-0000ae40: 2020 2274 6173 6b44 6174 6122 3a20 226d    "taskData": "m
-0000ae50: 795f 7461 736b 5f64 6174 615f 7374 7269  y_task_data_stri
-0000ae60: 6e67 222c 0a20 2020 2020 2022 7461 736b  ng",.      "task
-0000ae70: 4461 7461 4669 6c65 223a 2022 6d79 5f64  DataFile": "my_d
-0000ae80: 6174 615f 6669 6c65 2e74 7874 222c 0a20  ata_file.txt",. 
-0000ae90: 2020 2020 2022 7461 736b 5479 7065 7322       "taskTypes"
-0000aea0: 3a20 5b22 646f 636b 6572 225d 2c0a 2020  : ["docker"],.  
-0000aeb0: 2020 2020 2274 6173 6b73 5065 7257 6f72      "tasksPerWor
-0000aec0: 6b65 7222 3a20 312c 0a20 2020 2020 2022  ker": 1,.      "
-0000aed0: 7570 6c6f 6164 4669 6c65 7322 3a20 5b7b  uploadFiles": [{
-0000aee0: 226c 6f63 616c 5061 7468 223a 2022 6669  "localPath": "fi
-0000aef0: 6c65 5f31 2e74 7874 222c 2022 7570 6c6f  le_1.txt", "uplo
-0000af00: 6164 5061 7468 223a 2022 6669 6c65 5f31  adPath": "file_1
-0000af10: 2e74 7874 227d 5d2c 0a20 2020 2020 2022  .txt"}],.      "
-0000af20: 7663 7075 7322 3a20 5b31 2c20 345d 2c0a  vcpus": [1, 4],.
-0000af30: 2020 2020 2020 2276 6572 6966 7941 7453        "verifyAtS
-0000af40: 7461 7274 223a 205b 2272 6561 6479 5f72  tart": ["ready_r
-0000af50: 6573 756c 7473 2e74 7874 225d 2c0a 2020  esults.txt"],.  
-0000af60: 2020 2020 2276 6572 6966 7957 6169 7422      "verifyWait"
-0000af70: 3a20 5b22 7761 6974 5f66 6f72 5f72 6573  : ["wait_for_res
-0000af80: 756c 7473 2e74 7874 225d 2c0a 2020 2020  ults.txt"],.    
-0000af90: 2020 2277 6f72 6b65 7254 6167 7322 3a20    "workerTags": 
-0000afa0: 5b5d 2c0a 2020 2020 2020 2274 6173 6b73  [],.      "tasks
-0000afb0: 223a 205b 0a20 2020 2020 2020 207b 7d0a  ": [.        {}.
-0000afc0: 2020 2020 2020 5d0a 2020 2020 7d2c 0a20        ].    },. 
-0000afd0: 2020 207b 0a20 2020 2020 2022 6e61 6d65     {.      "name
-0000afe0: 223a 2022 7365 636f 6e64 2d74 6173 6b2d  ": "second-task-
-0000aff0: 6772 6f75 7022 2c0a 2020 2020 2020 2264  group",.      "d
-0000b000: 6570 656e 6465 6e74 4f6e 223a 2022 6669  ependentOn": "fi
-0000b010: 7273 742d 7461 736b 2d67 726f 7570 222c  rst-task-group",
-0000b020: 0a20 2020 2020 2022 7461 736b 7322 3a20  .      "tasks": 
-0000b030: 5b0a 2020 2020 2020 2020 7b7d 0a20 2020  [.        {}.   
-0000b040: 2020 205d 0a20 2020 207d 0a20 205d 0a7d     ].    }.  ].}
-0000b050: 0a60 6060 0a0a 2323 2320 4a53 4f4e 2050  .```..### JSON P
-0000b060: 726f 7065 7274 6965 7320 6174 2074 6865  roperties at the
-0000b070: 2054 6173 6b20 4c65 7665 6c0a 0a53 686f   Task Level..Sho
-0000b080: 7769 6e67 2061 6c6c 2070 6f73 7369 626c  wing all possibl
-0000b090: 6520 7072 6f70 6572 7469 6573 2061 7420  e properties at 
-0000b0a0: 7468 6520 5461 736b 206c 6576 656c 3a0a  the Task level:.
-0000b0b0: 0a60 6060 6a73 6f6e 0a7b 0a20 2022 7461  .```json.{.  "ta
-0000b0c0: 736b 4772 6f75 7073 223a 205b 0a20 2020  skGroups": [.   
-0000b0d0: 207b 0a20 2020 2020 2022 7461 736b 7322   {.      "tasks"
-0000b0e0: 3a20 5b0a 2020 2020 2020 2020 7b0a 2020  : [.        {.  
-0000b0f0: 2020 2020 2020 2020 2261 7267 756d 656e          "argumen
-0000b100: 7473 223a 205b 312c 2032 5d2c 0a20 2020  ts": [1, 2],.   
-0000b110: 2020 2020 2020 2022 6361 7074 7572 6554         "captureT
-0000b120: 6173 6b4f 7574 7075 7422 3a20 7472 7565  askOutput": true
-0000b130: 2c0a 2020 2020 2020 2020 2020 2264 6f63  ,.          "doc
-0000b140: 6b65 7245 6e76 6972 6f6e 6d65 6e74 223a  kerEnvironment":
-0000b150: 207b 224d 595f 444f 434b 4552 5f56 4152   {"MY_DOCKER_VAR
-0000b160: 223a 2031 3030 7d2c 0a20 2020 2020 2020  ": 100},.       
-0000b170: 2020 2022 646f 636b 6572 5061 7373 776f     "dockerPasswo
-0000b180: 7264 223a 2022 6d79 5061 7373 776f 7264  rd": "myPassword
-0000b190: 222c 0a20 2020 2020 2020 2020 2022 646f  ",.          "do
-0000b1a0: 636b 6572 5573 6572 6e61 6d65 223a 2022  ckerUsername": "
-0000b1b0: 6d79 5573 6572 6e61 6d65 222c 0a20 2020  myUsername",.   
-0000b1c0: 2020 2020 2020 2022 656e 7669 726f 6e6d         "environm
-0000b1d0: 656e 7422 3a20 7b22 4d59 5f56 4152 223a  ent": {"MY_VAR":
-0000b1e0: 2031 3030 7d2c 0a20 2020 2020 2020 2020   100},.         
-0000b1f0: 2022 6578 6563 7574 6162 6c65 223a 2022   "executable": "
-0000b200: 6d79 2d63 6f6e 7461 696e 6572 222c 0a20  my-container",. 
-0000b210: 2020 2020 2020 2020 2022 666c 6174 7465           "flatte
-0000b220: 6e49 6e70 7574 5061 7468 7322 3a20 6661  nInputPaths": fa
-0000b230: 6c73 652c 0a20 2020 2020 2020 2020 2022  lse,.          "
-0000b240: 696e 7075 7473 223a 205b 2261 7070 2f6d  inputs": ["app/m
-0000b250: 6169 6e2e 7079 222c 2022 6170 702f 7265  ain.py", "app/re
-0000b260: 7175 6972 656d 656e 7473 2e74 7874 225d  quirements.txt"]
-0000b270: 2c0a 2020 2020 2020 2020 2020 2269 6e70  ,.          "inp
-0000b280: 7574 734f 7074 696f 6e61 6c22 3a20 5b22  utsOptional": ["
-0000b290: 6f70 7469 6f6e 616c 2e74 7874 225d 2c0a  optional.txt"],.
-0000b2a0: 2020 2020 2020 2020 2020 226e 616d 6522            "name"
-0000b2b0: 3a20 226d 792d 7461 736b 222c 0a20 2020  : "my-task",.   
-0000b2c0: 2020 2020 2020 2022 6f75 7470 7574 7322         "outputs"
-0000b2d0: 3a20 5b22 7265 7375 6c74 732e 7478 7422  : ["results.txt"
-0000b2e0: 5d2c 0a20 2020 2020 2020 2020 2022 6f75  ],.          "ou
-0000b2f0: 7470 7574 7352 6571 7569 7265 6422 3a20  tputsRequired": 
-0000b300: 5b22 7265 7375 6c74 735f 7265 7175 6972  ["results_requir
-0000b310: 6564 2e74 7874 225d 2c0a 2020 2020 2020  ed.txt"],.      
-0000b320: 2020 2020 2274 6173 6b44 6174 6122 3a20      "taskData": 
-0000b330: 226d 795f 7461 736b 5f64 6174 615f 7374  "my_task_data_st
-0000b340: 7269 6e67 222c 0a20 2020 2020 2020 2020  ring",.         
-0000b350: 2022 7461 736b 4461 7461 4669 6c65 223a   "taskDataFile":
-0000b360: 2022 6d79 5f64 6174 615f 6669 6c65 2e74   "my_data_file.t
-0000b370: 7874 222c 0a20 2020 2020 2020 2020 2022  xt",.          "
-0000b380: 7461 736b 5479 7065 223a 2022 646f 636b  taskType": "dock
-0000b390: 6572 222c 0a20 2020 2020 2020 2020 2022  er",.          "
-0000b3a0: 7570 6c6f 6164 4669 6c65 7322 3a20 5b7b  uploadFiles": [{
-0000b3b0: 226c 6f63 616c 5061 7468 223a 2022 6669  "localPath": "fi
-0000b3c0: 6c65 5f31 2e74 7874 222c 2022 7570 6c6f  le_1.txt", "uplo
-0000b3d0: 6164 5061 7468 223a 2022 6669 6c65 5f31  adPath": "file_1
-0000b3e0: 2e74 7874 227d 5d2c 0a20 2020 2020 2020  .txt"}],.       
-0000b3f0: 2020 2022 7665 7269 6679 4174 5374 6172     "verifyAtStar
-0000b400: 7422 3a20 5b22 7265 6164 795f 7265 7375  t": ["ready_resu
-0000b410: 6c74 732e 7478 7422 5d2c 0a20 2020 2020  lts.txt"],.     
-0000b420: 2020 2020 2022 7665 7269 6679 5761 6974       "verifyWait
-0000b430: 223a 205b 2277 6169 745f 666f 725f 7265  ": ["wait_for_re
-0000b440: 7375 6c74 732e 7478 7422 5d0a 2020 2020  sults.txt"].    
-0000b450: 2020 2020 7d0a 2020 2020 2020 5d0a 2020      }.      ].  
-0000b460: 2020 7d0a 2020 5d0a 7d0a 6060 600a 0a23    }.  ].}.```..#
-0000b470: 2320 5661 7269 6162 6c65 2053 7562 7374  # Variable Subst
-0000b480: 6974 7574 696f 6e73 2069 6e20 576f 726b  itutions in Work
-0000b490: 2052 6571 7569 7265 6d65 6e74 2050 726f   Requirement Pro
-0000b4a0: 7065 7274 6965 730a 0a56 6172 6961 626c  perties..Variabl
-0000b4b0: 6520 7375 6273 7469 7475 7469 6f6e 7320  e substitutions 
-0000b4c0: 6361 6e20 6265 2075 7365 6420 7769 7468  can be used with
-0000b4d0: 696e 2061 6e79 2070 726f 7065 7274 7920  in any property 
-0000b4e0: 7661 6c75 6520 696e 2054 4f4d 4c20 636f  value in TOML co
-0000b4f0: 6e66 6967 7572 6174 696f 6e20 6669 6c65  nfiguration file
-0000b500: 7320 6f72 2057 6f72 6b20 5265 7175 6972  s or Work Requir
-0000b510: 656d 656e 7420 4a53 4f4e 2066 696c 6573  ement JSON files
-0000b520: 2e20 5365 6520 7468 6520 6465 7363 7269  . See the descri
-0000b530: 7074 696f 6e20 5b61 626f 7665 5d28 2376  ption [above](#v
-0000b540: 6172 6961 626c 652d 7375 6273 7469 7475  ariable-substitu
-0000b550: 7469 6f6e 7329 2066 6f72 206d 6f72 6520  tions) for more 
-0000b560: 6465 7461 696c 7320 6f6e 2076 6172 6961  details on varia
-0000b570: 626c 6520 7375 6273 7469 7475 7469 6f6e  ble substitution
-0000b580: 732e 2054 6869 7320 6973 2061 2070 6f77  s. This is a pow
-0000b590: 6572 6675 6c20 6665 6174 7572 6520 7468  erful feature th
-0000b5a0: 6174 2061 6c6c 6f77 7320 576f 726b 2052  at allows Work R
-0000b5b0: 6571 7569 7265 6d65 6e74 7320 746f 2062  equirements to b
-0000b5c0: 6520 7061 7261 6d65 7465 7269 7365 6420  e parameterised 
-0000b5d0: 6279 2073 7570 706c 7969 6e67 2076 616c  by supplying val
-0000b5e0: 7565 7320 6f6e 2074 6865 2063 6f6d 6d61  ues on the comma
-0000b5f0: 6e64 206c 696e 652c 2076 6961 2065 6e76  nd line, via env
-0000b600: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
-0000b610: 6573 206f 7220 7669 6120 7468 6520 544f  es or via the TO
-0000b620: 4d4c 2066 696c 652e 0a0a 2323 2320 5461  ML file...### Ta
-0000b630: 736b 2061 6e64 2054 6173 6b20 4772 6f75  sk and Task Grou
-0000b640: 7020 4e61 6d65 2053 7562 7374 6974 7574  p Name Substitut
-0000b650: 696f 6e0a 0a54 6865 2066 6f6c 6c6f 7769  ion..The followi
-0000b660: 6e67 206e 756d 6265 7269 6e67 2061 6e64  ng numbering and
-0000b670: 206e 616d 696e 6720 7375 6273 7469 7475   naming substitu
-0000b680: 7469 6f6e 7320 6172 6520 6176 6169 6c61  tions are availa
-0000b690: 626c 6520 666f 7220 7573 6520 696e 2054  ble for use in T
-0000b6a0: 6173 6b20 616e 6420 5461 736b 2047 726f  ask and Task Gro
-0000b6b0: 7570 206e 616d 696e 672c 206f 6e6c 7920  up naming, only 
-0000b6c0: 7768 656e 2074 6865 2057 6f72 6b20 5265  when the Work Re
-0000b6d0: 7175 6972 656d 656e 7420 6973 2073 7065  quirement is spe
-0000b6e0: 6369 6669 6564 2061 7320 204a 534f 4e20  cified as  JSON 
-0000b6f0: 646f 6375 6d65 6e74 2c20 692e 652e 2c20  document, i.e., 
-0000b700: 7468 6579 2063 616e 2062 6520 7573 6564  they can be used
-0000b710: 2069 6e20 7468 6520 606e 616d 6560 2070   in the `name` p
-0000b720: 726f 7065 7274 6965 7320 666f 7220 5461  roperties for Ta
-0000b730: 736b 7320 616e 6420 5461 736b 2047 726f  sks and Task Gro
-0000b740: 7570 7320 696e 204a 534f 4e20 7370 6563  ups in JSON spec
-0000b750: 6966 6963 6174 696f 6e73 2e0a 0a54 6865  ifications...The
-0000b760: 2066 6f6c 6c6f 7769 6e67 2074 6162 6c65   following table
-0000b770: 2064 6566 696e 6573 2074 6865 2063 6f6e   defines the con
-0000b780: 7465 7874 2873 2920 696e 2077 6869 6368  text(s) in which
-0000b790: 2065 6163 6820 7661 7269 6162 6c65 2063   each variable c
-0000b7a0: 616e 2062 6520 7573 6564 3a0a 0a7c 2044  an be used:..| D
-0000b7b0: 6972 6563 7469 7665 2020 2020 2020 2020  irective        
-0000b7c0: 2020 2020 2020 207c 2044 6573 6372 6970         | Descrip
-0000b7d0: 7469 6f6e 2020 2020 2020 2020 2020 2020  tion            
-0000b7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b7f0: 2020 2020 2020 2020 2020 207c 2054 6173             | Tas
-0000b800: 6b20 7c20 5461 736b 2047 726f 7570 207c  k | Task Group |
-0000b810: 0a7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .|:-------------
-0000b820: 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 3a2d 2d2d  -----------|:---
-0000b830: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000b840: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000b850: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  ---------------|
-0000b860: 3a2d 2d2d 2d2d 7c3a 2d2d 2d2d 2d2d 2d2d  :-----|:--------
-0000b870: 2d2d 2d7c 0a7c 2060 7b7b 7461 736b 5f6e  ---|.| `{{task_n
-0000b880: 756d 6265 727d 7d60 2020 2020 2020 207c  umber}}`       |
-0000b890: 2054 6865 2063 7572 7265 6e74 2054 6173   The current Tas
-0000b8a0: 6b20 6e75 6d62 6572 2020 2020 2020 2020  k number        
-0000b8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b8c0: 2020 207c 2059 6573 2020 7c20 2020 2020     | Yes  |     
-0000b8d0: 2020 2020 2020 207c 0a7c 2060 7b7b 7461         |.| `{{ta
-0000b8e0: 736b 5f6e 616d 657d 7d60 2020 2020 2020  sk_name}}`      
-0000b8f0: 2020 207c 2054 6865 2063 7572 7265 6e74     | The current
-0000b900: 2054 6173 6b20 6e61 6d65 2020 2020 2020   Task name      
-0000b910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b920: 2020 2020 2020 207c 2059 6573 2020 7c20         | Yes  | 
-0000b930: 2020 2020 2020 2020 2020 207c 0a7c 2060             |.| `
-0000b940: 7b7b 7461 736b 5f67 726f 7570 5f6e 616d  {{task_group_nam
-0000b950: 657d 7d60 2020 207c 2054 6865 2063 7572  e}}`   | The cur
-0000b960: 7265 6e74 2054 6173 6b20 4772 6f75 7020  rent Task Group 
-0000b970: 6e61 6d65 2020 2020 2020 2020 2020 2020  name            
-0000b980: 2020 2020 2020 2020 2020 207c 2059 6573             | Yes
-0000b990: 2020 7c20 2020 2020 2020 2020 2020 207c    |            |
-0000b9a0: 0a7c 2060 7b7b 7461 736b 5f63 6f75 6e74  .| `{{task_count
-0000b9b0: 7d7d 6020 2020 2020 2020 207c 2054 6865  }}`        | The
-0000b9c0: 206e 756d 6265 7220 6f66 2054 6173 6b73   number of Tasks
-0000b9d0: 2069 6e20 7468 6520 6375 7272 656e 7420   in the current 
-0000b9e0: 5461 736b 2047 726f 7570 2020 2020 207c  Task Group     |
-0000b9f0: 2059 6573 2020 7c20 5965 7320 2020 2020   Yes  | Yes     
-0000ba00: 2020 207c 0a7c 2060 7b7b 7461 736b 5f67     |.| `{{task_g
-0000ba10: 726f 7570 5f6e 756d 6265 727d 7d60 207c  roup_number}}` |
-0000ba20: 2054 6865 2063 7572 7265 6e74 2054 6173   The current Tas
-0000ba30: 6b20 4772 6f75 7020 6e75 6d62 6572 2020  k Group number  
-0000ba40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba50: 2020 207c 2059 6573 2020 7c20 5965 7320     | Yes  | Yes 
-0000ba60: 2020 2020 2020 207c 0a7c 2060 7b7b 7461         |.| `{{ta
-0000ba70: 736b 5f67 726f 7570 5f63 6f75 6e74 7d7d  sk_group_count}}
-0000ba80: 6020 207c 2054 6865 206e 756d 6265 7220  `  | The number 
-0000ba90: 6f66 2054 6173 6b20 4772 6f75 7073 2069  of Task Groups i
-0000baa0: 6e20 7468 6520 576f 726b 2052 6571 7569  n the Work Requi
-0000bab0: 7265 6d65 6e74 207c 2059 6573 2020 7c20  rement | Yes  | 
-0000bac0: 5965 7320 2020 2020 2020 207c 0a0a 496e  Yes        |..In
-0000bad0: 2061 6464 6974 696f 6e2c 202a 2a54 6173   addition, **Tas
-0000bae0: 6b73 2a2a 2064 6566 696e 6564 2069 6e20  ks** defined in 
-0000baf0: 4a53 4f4e 2064 6f63 756d 656e 7473 2063  JSON documents c
-0000bb00: 616e 2075 7365 2061 6e79 206f 6620 7468  an use any of th
-0000bb10: 6520 7375 6273 7469 7475 7469 6f6e 7320  e substitutions 
-0000bb20: 6162 6f76 6520 696e 2061 6e79 206f 6620  above in any of 
-0000bb30: 7468 6569 7220 7072 6f70 6572 7469 6573  their properties
-0000bb40: 2c20 6e6f 7420 6a75 7374 2060 6e61 6d65  , not just `name
-0000bb50: 602e 0a0a 4e75 6d62 6572 7320 6172 6520  `...Numbers are 
-0000bb60: 7a65 726f 2d70 6164 6465 6420 666f 7220  zero-padded for 
-0000bb70: 6e65 6174 2066 6f72 6d61 7474 696e 6720  neat formatting 
-0000bb80: 616e 6420 736f 7274 696e 672c 2065 2e67  and sorting, e.g
-0000bb90: 2e2c 2054 6173 6b20 6e75 6d62 6572 2060  ., Task number `
-0000bba0: 3337 6020 6f66 2060 3130 3030 6020 5461  37` of `1000` Ta
-0000bbb0: 736b 7320 776f 756c 6420 6265 2073 7562  sks would be sub
-0000bbc0: 7374 6974 7574 6564 2061 7320 6030 3033  stituted as `003
-0000bbd0: 3760 2e0a 0a41 7320 616e 2065 7861 6d70  7`...As an examp
-0000bbe0: 6c65 2c20 7468 6520 666f 6c6c 6f77 696e  le, the followin
-0000bbf0: 6720 4a53 4f4e 2057 6f72 6b20 5265 7175  g JSON Work Requ
-0000bc00: 6972 656d 656e 743a 0a0a 6060 606a 736f  irement:..```jso
-0000bc10: 6e0a 7b0a 2020 2274 6173 6b47 726f 7570  n.{.  "taskGroup
-0000bc20: 7322 3a20 5b0a 2020 2020 7b0a 2020 2020  s": [.    {.    
-0000bc30: 2020 226e 616d 6522 3a20 226d 795f 7461    "name": "my_ta
-0000bc40: 736b 5f67 726f 7570 5f7b 7b74 6173 6b5f  sk_group_{{task_
-0000bc50: 6772 6f75 705f 6e75 6d62 6572 7d7d 5f61  group_number}}_a
-0000bc60: 3122 2c0a 2020 2020 2020 2265 7865 6375  1",.      "execu
-0000bc70: 7461 626c 6522 3a20 2265 7831 2e73 6822  table": "ex1.sh"
-0000bc80: 2c0a 2020 2020 2020 2274 6173 6b43 6f75  ,.      "taskCou
-0000bc90: 6e74 223a 2032 2c0a 2020 2020 2020 2274  nt": 2,.      "t
-0000bca0: 6173 6b73 223a 205b 0a20 2020 2020 2020  asks": [.       
-0000bcb0: 207b 0a20 2020 2020 2020 2020 2022 6e61   {.          "na
-0000bcc0: 6d65 223a 2022 6d79 5f74 6173 6b5f 7b7b  me": "my_task_{{
-0000bcd0: 7461 736b 5f6e 756d 6265 727d 7d2d 6f66  task_number}}-of
-0000bce0: 2d7b 7b74 6173 6b5f 636f 756e 747d 7d22  -{{task_count}}"
-0000bcf0: 2c0a 2020 2020 2020 2020 2020 2265 6e76  ,.          "env
-0000bd00: 6972 6f6e 6d65 6e74 223a 207b 2254 4153  ironment": {"TAS
-0000bd10: 4b5f 4e55 4d42 4552 223a 2022 7b7b 7461  K_NUMBER": "{{ta
-0000bd20: 736b 5f6e 756d 6265 727d 7d22 7d0a 2020  sk_number}}"}.  
-0000bd30: 2020 2020 2020 7d0a 2020 2020 2020 5d0a        }.      ].
-0000bd40: 2020 2020 7d2c 0a20 2020 207b 0a20 2020      },.    {.   
-0000bd50: 2020 2022 6e61 6d65 223a 2022 6d79 5f74     "name": "my_t
-0000bd60: 6173 6b5f 6772 6f75 705f 7b7b 7461 736b  ask_group_{{task
-0000bd70: 5f67 726f 7570 5f6e 756d 6265 727d 7d5f  _group_number}}_
-0000bd80: 6231 222c 0a20 2020 2020 2022 6578 6563  b1",.      "exec
-0000bd90: 7574 6162 6c65 223a 2022 6578 322e 7368  utable": "ex2.sh
-0000bda0: 222c 0a20 2020 2020 2022 7461 736b 436f  ",.      "taskCo
-0000bdb0: 756e 7422 3a20 322c 0a20 2020 2020 2022  unt": 2,.      "
-0000bdc0: 7461 736b 7322 3a20 5b0a 2020 2020 2020  tasks": [.      
-0000bdd0: 2020 7b0a 2020 2020 2020 2020 2020 226e    {.          "n
-0000bde0: 616d 6522 3a20 226d 795f 7461 736b 5f7b  ame": "my_task_{
-0000bdf0: 7b74 6173 6b5f 6e75 6d62 6572 7d7d 2d6f  {task_number}}-o
-0000be00: 662d 7b7b 7461 736b 5f63 6f75 6e74 7d7d  f-{{task_count}}
-0000be10: 220a 2020 2020 2020 2020 7d0a 2020 2020  ".        }.    
-0000be20: 2020 5d0a 2020 2020 7d0a 2020 5d0a 7d0a    ].    }.  ].}.
-0000be30: 6060 600a 0a2e 2e2e 2077 6f75 6c64 2063  ```..... would c
-0000be40: 7265 6174 6520 5461 736b 2047 726f 7570  reate Task Group
-0000be50: 7320 6e61 6d65 6420 606d 795f 7461 736b  s named `my_task
-0000be60: 5f67 726f 7570 5f31 5f61 3160 2061 6e64  _group_1_a1` and
-0000be70: 2060 6d79 5f74 6173 6b5f 6772 6f75 705f   `my_task_group_
-0000be80: 325f 6231 602c 2065 6163 6820 636f 6e74  2_b1`, each cont
-0000be90: 6169 6e69 6e67 2054 6173 6b73 206e 616d  aining Tasks nam
-0000bea0: 6564 2060 6d79 5f74 6173 6b5f 312d 6f66  ed `my_task_1-of
-0000beb0: 2d32 602c 2060 6d79 5f74 6173 6b5f 322d  -2`, `my_task_2-
-0000bec0: 6f66 2d32 602e 0a0a 2323 2320 576f 726b  of-2`...### Work
-0000bed0: 2052 6571 7569 7265 6d65 6e74 204e 616d   Requirement Nam
-0000bee0: 6520 5375 6273 7469 7475 7469 6f6e 0a0a  e Substitution..
-0000bef0: 5468 6520 6e61 6d65 206f 6620 7468 6520  The name of the 
-0000bf00: 576f 726b 2052 6571 7569 7265 6d65 6e74  Work Requirement
-0000bf10: 2069 7473 656c 6620 6361 6e20 6265 2075   itself can be u
-0000bf20: 7365 6420 7669 6120 7468 6520 7661 7269  sed via the vari
-0000bf30: 6162 6c65 2073 7562 7374 6974 7574 696f  able substitutio
-0000bf40: 6e20 607b 7b77 725f 6e61 6d65 7d7d 602e  n `{{wr_name}}`.
-0000bf50: 2054 6869 7320 6361 6e20 6265 2075 7365   This can be use
-0000bf60: 6420 616e 7977 6865 7265 2069 6e20 6120  d anywhere in a 
-0000bf70: 544f 4d4c 2063 6f6e 6669 6775 7261 7469  TOML configurati
-0000bf80: 6f6e 2066 696c 6520 6f72 2069 6e20 6120  on file or in a 
-0000bf90: 4a53 4f4e 2057 6f72 6b20 5265 7175 6972  JSON Work Requir
-0000bfa0: 656d 656e 742e 0a0a 2323 2044 7279 2d52  ement...## Dry-R
-0000bfb0: 756e 6e69 6e67 2057 6f72 6b20 5265 7175  unning Work Requ
-0000bfc0: 6972 656d 656e 7420 5375 626d 6973 7369  irement Submissi
-0000bfd0: 6f6e 730a 0a54 6f20 6578 616d 696e 6520  ons..To examine 
-0000bfe0: 7468 6520 4a53 4f4e 2074 6861 7420 7769  the JSON that wi
-0000bff0: 6c6c 2061 6374 7561 6c6c 7920 6265 2073  ll actually be s
-0000c000: 656e 7420 746f 2074 6865 2059 656c 6c6f  ent to the Yello
-0000c010: 7744 6f67 2041 5049 2061 6674 6572 2061  wDog API after a
-0000c020: 6c6c 2070 726f 6365 7373 696e 672c 2075  ll processing, u
-0000c030: 7365 2074 6865 2060 2d2d 6472 792d 7275  se the `--dry-ru
-0000c040: 6e60 2063 6f6d 6d61 6e64 206c 696e 6520  n` command line 
-0000c050: 6f70 7469 6f6e 2077 6865 6e20 7275 6e6e  option when runn
-0000c060: 696e 6720 6079 642d 7375 626d 6974 602e  ing `yd-submit`.
-0000c070: 2054 6869 7320 7769 6c6c 2070 7269 6e74   This will print
-0000c080: 2074 6865 2066 756c 6c79 2070 726f 6365   the fully proce
-0000c090: 7373 6564 204a 534f 4e20 666f 7220 7468  ssed JSON for th
-0000c0a0: 6520 576f 726b 2052 6571 7569 7265 6d65  e Work Requireme
-0000c0b0: 6e74 2e20 4e6f 7468 696e 6720 7769 6c6c  nt. Nothing will
-0000c0c0: 2062 6520 7375 626d 6974 7465 6420 746f   be submitted to
-0000c0d0: 2074 6865 2050 6c61 7466 6f72 6d2e 0a0a   the Platform...
-0000c0e0: 5468 6520 6472 792d 7275 6e20 6973 2075  The dry-run is u
-0000c0f0: 7365 6675 6c20 666f 7220 696e 7370 6563  seful for inspec
-0000c100: 7469 6e67 2074 6865 2072 6573 756c 7473  ting the results
-0000c110: 206f 6620 616c 6c20 7468 6520 7072 6f63   of all the proc
-0000c120: 6573 7369 6e67 2074 6861 7427 7320 6265  essing that's be
-0000c130: 656e 2070 6572 666f 726d 6564 2e20 546f  en performed. To
-0000c140: 2073 7570 7072 6573 7320 616c 6c20 6f75   suppress all ou
-0000c150: 7470 7574 2065 7863 6570 7420 666f 7220  tput except for 
-0000c160: 7468 6520 4a53 4f4e 2069 7473 656c 662c  the JSON itself,
-0000c170: 2075 7365 2074 6865 2060 2d2d 7175 6965   use the `--quie
-0000c180: 7460 2028 602d 7160 2920 636f 6d6d 616e  t` (`-q`) comman
-0000c190: 6420 6c69 6e65 206f 7074 696f 6e2e 0a0a  d line option...
-0000c1a0: 4e6f 7465 2074 6861 7420 7468 6520 6765  Note that the ge
-0000c1b0: 6e65 7261 7465 6420 4a53 4f4e 2069 7320  nerated JSON is 
-0000c1c0: 6120 636f 6e73 6f6c 6964 6174 6564 2066  a consolidated f
-0000c1d0: 6f72 6d20 6f66 2077 6861 7420 776f 756c  orm of what woul
-0000c1e0: 6420 6265 2073 7562 6d69 7474 6564 2074  d be submitted t
-0000c1f0: 6f20 7468 6520 5965 6c6c 6f77 446f 6720  o the YellowDog 
-0000c200: 4150 492c 2061 6e64 2054 6173 6b73 2061  API, and Tasks a
-0000c210: 7265 2064 6566 696e 6564 2064 6972 6563  re defined direc
-0000c220: 746c 7920 7769 7468 696e 2074 6865 6972  tly within their
-0000c230: 2054 6173 6b20 4772 6f75 7073 2066 6f72   Task Groups for
-0000c240: 2065 6173 6520 6f66 2063 6f6d 7072 6568   ease of compreh
-0000c250: 656e 7369 6f6e 2e20 496e 2061 6374 7561  ension. In actua
-0000c260: 6c20 4150 4920 7375 626d 6973 7369 6f6e  l API submission
-0000c270: 732c 2074 6865 2057 6f72 6b20 5265 7175  s, the Work Requ
-0000c280: 6972 656d 656e 7420 7769 7468 2069 7473  irement with its
-0000c290: 2054 6173 6b20 4772 6f75 7073 2069 7320   Task Groups is 
-0000c2a0: 7375 626d 6974 7465 6420 6669 7273 742c  submitted first,
-0000c2b0: 2061 6e64 2054 6173 6b73 2061 7265 2074   and Tasks are t
-0000c2c0: 6865 6e20 6164 6465 6420 746f 2054 6173  hen added to Tas
-0000c2d0: 6b20 4772 6f75 7073 2073 6570 6172 6174  k Groups separat
-0000c2e0: 656c 7920 696e 2073 7562 7365 7175 656e  ely in subsequen
-0000c2f0: 7420 4150 4920 6361 6c6c 732e 0a0a 4120  t API calls...A 
-0000c300: 7369 6d70 6c65 2065 7861 6d70 6c65 206f  simple example o
-0000c310: 6620 7468 6520 4a53 4f4e 206f 7574 7075  f the JSON outpu
-0000c320: 7420 6973 2073 686f 776e 2062 656c 6f77  t is shown below
-0000c330: 2c20 7368 6f77 696e 6720 6120 576f 726b  , showing a Work
-0000c340: 2052 6571 7569 7265 6d65 6e74 2077 6974   Requirement wit
-0000c350: 6820 6120 7369 6e67 6c65 2054 6173 6b20  h a single Task 
-0000c360: 4772 6f75 702c 2063 6f6e 7461 696e 696e  Group, containin
-0000c370: 6720 6120 7369 6e67 6c65 2054 6173 6b2e  g a single Task.
-0000c380: 0a0a 6025 2079 642d 7375 626d 6974 202d  ..`% yd-submit -
-0000c390: 2d64 7279 2d72 756e 202d 2d71 7569 6574  -dry-run --quiet
-0000c3a0: 600a 6060 606a 736f 6e0a 7b0a 2020 2266  `.```json.{.  "f
-0000c3b0: 756c 6669 6c4f 6e53 7562 6d69 7422 3a20  ulfilOnSubmit": 
-0000c3c0: 6661 6c73 652c 0a20 2022 6e61 6d65 223a  false,.  "name":
-0000c3d0: 2022 7079 6578 2d62 6173 685f 3233 3031   "pyex-bash_2301
-0000c3e0: 3134 2d30 3935 3530 342d 3533 6122 2c0a  14-095504-53a",.
-0000c3f0: 2020 226e 616d 6573 7061 6365 223a 2022    "namespace": "
-0000c400: 7079 6578 616d 706c 6573 222c 0a20 2022  pyexamples",.  "
-0000c410: 7072 696f 7269 7479 223a 2030 2c0a 2020  priority": 0,.  
-0000c420: 2274 6167 223a 2022 7079 6578 2d62 6173  "tag": "pyex-bas
-0000c430: 6822 2c0a 2020 2274 6173 6b47 726f 7570  h",.  "taskGroup
-0000c440: 7322 3a20 5b0a 2020 2020 7b0a 2020 2020  s": [.    {.    
-0000c450: 2020 2266 696e 6973 6849 6641 6c6c 5461    "finishIfAllTa
-0000c460: 736b 7346 696e 6973 6865 6422 3a20 7472  sksFinished": tr
-0000c470: 7565 2c0a 2020 2020 2020 2266 696e 6973  ue,.      "finis
-0000c480: 6849 6641 6e79 5461 736b 4661 696c 6564  hIfAnyTaskFailed
-0000c490: 223a 2066 616c 7365 2c0a 2020 2020 2020  ": false,.      
-0000c4a0: 226e 616d 6522 3a20 2274 6173 6b5f 6772  "name": "task_gr
-0000c4b0: 6f75 705f 3122 2c0a 2020 2020 2020 2270  oup_1",.      "p
-0000c4c0: 7269 6f72 6974 7922 3a20 302c 0a20 2020  riority": 0,.   
-0000c4d0: 2020 2022 7275 6e53 7065 6369 6669 6361     "runSpecifica
-0000c4e0: 7469 6f6e 223a 207b 0a20 2020 2020 2020  tion": {.       
-0000c4f0: 2022 6d61 7869 6d75 6d54 6173 6b52 6574   "maximumTaskRet
-0000c500: 7269 6573 223a 2030 2c0a 2020 2020 2020  ries": 0,.      
-0000c510: 2020 2274 6173 6b54 7970 6573 223a 205b    "taskTypes": [
-0000c520: 2262 6173 6822 5d2c 0a20 2020 2020 2020  "bash"],.       
-0000c530: 2022 776f 726b 6572 5461 6773 223a 205b   "workerTags": [
-0000c540: 2270 7965 782d 6261 7368 225d 0a20 2020  "pyex-bash"].   
-0000c550: 2020 207d 2c0a 2020 2020 2020 2274 6173     },.      "tas
-0000c560: 6b73 223a 205b 0a20 2020 2020 2020 207b  ks": [.        {
-0000c570: 0a20 2020 2020 2020 2020 2022 6172 6775  .          "argu
-0000c580: 6d65 6e74 7322 3a20 5b22 7079 6578 2d62  ments": ["pyex-b
-0000c590: 6173 685f 3233 3031 3134 2d30 3935 3530  ash_230114-09550
-0000c5a0: 342d 3533 612f 736c 6565 705f 7363 7269  4-53a/sleep_scri
-0000c5b0: 7074 2e73 6822 5d2c 0a20 2020 2020 2020  pt.sh"],.       
-0000c5c0: 2020 2022 656e 7669 726f 6e6d 656e 7422     "environment"
-0000c5d0: 3a20 7b7d 2c0a 2020 2020 2020 2020 2020  : {},.          
-0000c5e0: 2269 6e70 7574 7322 3a20 5b0a 2020 2020  "inputs": [.    
-0000c5f0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
-0000c600: 2020 2020 2020 2020 226f 626a 6563 744e          "objectN
-0000c610: 616d 6550 6174 7465 726e 223a 2022 7079  amePattern": "py
-0000c620: 6578 2d62 6173 685f 3233 3031 3134 2d30  ex-bash_230114-0
-0000c630: 3935 3530 342d 3533 612f 736c 6565 705f  95504-53a/sleep_
-0000c640: 7363 7269 7074 2e73 6822 2c0a 2020 2020  script.sh",.    
-0000c650: 2020 2020 2020 2020 2020 2273 6f75 7263            "sourc
-0000c660: 6522 3a20 2254 4153 4b5f 4e41 4d45 5350  e": "TASK_NAMESP
-0000c670: 4143 4522 2c0a 2020 2020 2020 2020 2020  ACE",.          
-0000c680: 2020 2020 2276 6572 6966 6963 6174 696f      "verificatio
-0000c690: 6e22 3a20 2256 4552 4946 595f 5741 4954  n": "VERIFY_WAIT
-0000c6a0: 220a 2020 2020 2020 2020 2020 2020 7d0a  ".            }.
-0000c6b0: 2020 2020 2020 2020 2020 5d2c 0a20 2020            ],.   
-0000c6c0: 2020 2020 2020 2022 6e61 6d65 223a 2022         "name": "
-0000c6d0: 7461 736b 5f30 3122 2c0a 2020 2020 2020  task_01",.      
-0000c6e0: 2020 2020 226f 7574 7075 7473 223a 205b      "outputs": [
-0000c6f0: 0a20 2020 2020 2020 2020 2020 207b 2261  .            {"a
-0000c700: 6c77 6179 7355 706c 6f61 6422 3a20 7472  lwaysUpload": tr
-0000c710: 7565 2c20 2272 6571 7569 7265 6422 3a20  ue, "required": 
-0000c720: 6661 6c73 652c 2022 736f 7572 6365 223a  false, "source":
-0000c730: 2022 5052 4f43 4553 535f 4f55 5450 5554   "PROCESS_OUTPUT
-0000c740: 227d 0a20 2020 2020 2020 2020 205d 2c0a  "}.          ],.
-0000c750: 2020 2020 2020 2020 2020 2274 6173 6b54            "taskT
-0000c760: 7970 6522 3a20 2262 6173 6822 0a20 2020  ype": "bash".   
-0000c770: 2020 2020 207d 0a20 2020 2020 205d 0a20       }.      ]. 
-0000c780: 2020 207d 0a20 205d 0a7d 0a60 6060 0a0a     }.  ].}.```..
-0000c790: 2323 2320 5375 626d 6974 7469 6e67 2027  ### Submitting '
-0000c7a0: 5261 7727 204a 534f 4e20 576f 726b 2052  Raw' JSON Work R
-0000c7b0: 6571 7569 7265 6d65 6e74 2053 7065 6369  equirement Speci
-0000c7c0: 6669 6361 7469 6f6e 730a 0a49 7427 7320  fications..It's 
-0000c7d0: 706f 7373 6962 6c65 2074 6f20 7573 6520  possible to use 
-0000c7e0: 7468 6520 4a53 4f4e 206f 7574 7075 7420  the JSON output 
-0000c7f0: 6f66 2060 7964 2d73 7562 6d69 7420 2d2d  of `yd-submit --
-0000c800: 6472 792d 7275 6e60 2028 7375 6368 2061  dry-run` (such a
-0000c810: 7320 7468 6520 6578 616d 706c 6520 6162  s the example ab
-0000c820: 6f76 6529 2061 7320 6120 7365 6c66 2d63  ove) as a self-c
-0000c830: 6f6e 7461 696e 6564 2c20 6675 6c6c 792d  ontained, fully-
-0000c840: 7370 6563 6966 6965 6420 576f 726b 2052  specified Work R
-0000c850: 6571 7569 7265 6d65 6e74 2073 7065 6369  equirement speci
-0000c860: 6669 6361 7469 6f6e 2c20 7573 696e 6720  fication, using 
-0000c870: 7468 6520 602d 2d6a 736f 6e2d 7261 7760  the `--json-raw`
-0000c880: 2028 6f72 2060 2d6a 6029 2063 6f6d 6d61   (or `-j`) comma
-0000c890: 6e64 206c 696e 6520 6f70 7469 6f6e 2c20  nd line option, 
-0000c8a0: 692e 652e 3a20 6079 642d 7375 626d 6974  i.e.: `yd-submit
-0000c8b0: 202d 2d6a 736f 6e2d 7261 7720 3c66 696c   --json-raw <fil
-0000c8c0: 656e 616d 652e 6a73 6f6e 3e60 2e0a 0a54  ename.json>`...T
-0000c8d0: 6869 7320 7769 6c6c 2073 7562 6d69 7420  his will submit 
-0000c8e0: 7468 6520 576f 726b 2052 6571 7569 7265  the Work Require
-0000c8f0: 6d65 6e74 2c20 7468 656e 2061 6464 2061  ment, then add a
-0000c900: 6c6c 2074 6865 2073 7065 6369 6669 6564  ll the specified
-0000c910: 2054 6173 6b73 2e0a 0a4e 6f74 6520 7468   Tasks...Note th
-0000c920: 6174 2076 6172 6961 626c 6520 7375 6273  at variable subs
-0000c930: 7469 7475 7469 6f6e 7320 2a2a 6361 6e2a  titutions **can*
-0000c940: 2a20 6265 2075 7365 6420 696e 2074 6865  * be used in the
-0000c950: 2072 6177 204a 534f 4e20 6669 6c65 2c20   raw JSON file, 
-0000c960: 6a75 7374 2061 7320 696e 2074 6865 206f  just as in the o
-0000c970: 7468 6572 2057 6f72 6b20 5265 7175 6972  ther Work Requir
-0000c980: 656d 656e 7420 4a53 4f4e 2065 7861 6d70  ement JSON examp
-0000c990: 6c65 732c 2062 7574 2074 6865 7265 2069  les, but there i
-0000c9a0: 7320 6e6f 2070 726f 7065 7274 7920 696e  s no property in
-0000c9b0: 6865 7269 7461 6e63 652c 2069 6e63 6c75  heritance, inclu
-0000c9c0: 6469 6e67 2066 726f 6d20 7468 6520 605b  ding from the `[
-0000c9d0: 776f 726b 5265 7175 6972 656d 656e 745d  workRequirement]
-0000c9e0: 6020 7365 6374 696f 6e20 6f66 2074 6865  ` section of the
-0000c9f0: 2054 4f4d 4c20 636f 6e66 6967 7572 6174   TOML configurat
-0000ca00: 696f 6e20 6f72 2066 726f 6d20 576f 726b  ion or from Work
-0000ca10: 2052 6571 7569 7265 6d65 6e74 2070 726f   Requirement pro
-0000ca20: 7065 7274 6965 7320 7375 7070 6c69 6564  perties supplied
-0000ca30: 206f 6e20 7468 6520 636f 6d6d 616e 6420   on the command 
-0000ca40: 6c69 6e65 2e0a 0a4e 6f74 6520 7468 6174  line...Note that
-0000ca50: 2074 6865 7265 2069 7320 6e6f 2061 7574   there is no aut
-0000ca60: 6f6d 6174 6963 2066 696c 6520 7570 6c6f  omatic file uplo
-0000ca70: 6164 2077 6865 6e20 7573 696e 6720 7468  ad when using th
-0000ca80: 6973 206f 7074 696f 6e2c 2073 6f20 616e  is option, so an
-0000ca90: 7920 6669 6c65 7320 7265 7175 6972 6564  y files required
-0000caa0: 2061 7420 7468 6520 7374 6172 7420 6f66   at the start of
-0000cab0: 2074 6865 2074 6173 6b20 2873 7065 6369   the task (speci
-0000cac0: 6669 6564 2075 7369 6e67 2060 5645 5249  fied using `VERI
-0000cad0: 4659 5f41 545f 5354 4152 5460 2920 6d75  FY_AT_START`) mu
-0000cae0: 7374 2062 6520 7072 6573 656e 7420 6265  st be present be
-0000caf0: 666f 7265 2074 6865 2054 6173 6b73 2061  fore the Tasks a
-0000cb00: 7265 2075 706c 6f61 6465 642c 206f 7220  re uploaded, or 
-0000cb10: 7468 6520 5461 736b 7320 7769 6c6c 2066  the Tasks will f
-0000cb20: 6169 6c20 696d 6d65 6469 6174 656c 792e  ail immediately.
-0000cb30: 2054 6865 2060 7964 2d75 706c 6f61 6460   The `yd-upload`
-0000cb40: 2063 6f6d 6d61 6e64 2063 616e 2062 6520   command can be 
-0000cb50: 7573 6564 2074 6f20 7570 6c6f 6164 2074  used to upload t
-0000cb60: 6865 7365 2066 696c 6573 2c20 616e 6420  hese files, and 
-0000cb70: 6079 642d 7375 626d 6974 6020 7769 6c6c  `yd-submit` will
-0000cb80: 2070 6175 7365 2074 6f20 616c 6c6f 7720   pause to allow 
-0000cb90: 7468 6973 2074 6f20 6861 7070 656e 2e0a  this to happen..
-0000cba0: 0a23 2320 4669 6c65 2053 746f 7261 6765  .## File Storage
-0000cbb0: 204c 6f63 6174 696f 6e73 2061 6e64 2046   Locations and F
-0000cbc0: 696c 6520 5573 6167 650a 0a54 6869 7320  ile Usage..This 
-0000cbd0: 7365 6374 696f 6e20 6469 7363 7573 7365  section discusse
-0000cbe0: 7320 686f 7720 746f 2075 706c 6f61 6420  s how to upload 
-0000cbf0: 6669 6c65 7320 6672 6f6d 206c 6f63 616c  files from local
-0000cc00: 2073 746f 7261 6765 2074 6f20 7468 6520   storage to the 
-0000cc10: 5965 6c6c 6f77 446f 6720 4f62 6a65 6374  YellowDog Object
-0000cc20: 2053 746f 7265 2c20 686f 7720 7468 6f73   Store, how thos
-0000cc30: 6520 6669 6c65 7320 6172 6520 7472 616e  e files are tran
-0000cc40: 7366 6572 7265 6420 746f 2057 6f72 6b65  sferred to Worke
-0000cc50: 7220 4e6f 6465 7320 666f 7220 5461 736b  r Nodes for Task
-0000cc60: 2070 726f 6365 7373 696e 672c 2068 6f77   processing, how
-0000cc70: 2074 6865 2072 6573 756c 7473 206f 6620   the results of 
-0000cc80: 5461 736b 2070 726f 6365 7373 696e 6720  Task processing 
-0000cc90: 6172 6520 7265 7475 726e 6564 2062 7920  are returned by 
-0000cca0: 576f 726b 6572 204e 6f64 6573 2c20 616e  Worker Nodes, an
-0000ccb0: 6420 686f 7720 6669 6c65 7320 6172 6520  d how files are 
-0000ccc0: 7472 616e 7366 6572 7265 6420 6261 636b  transferred back
-0000ccd0: 2066 726f 6d20 7468 6520 5965 6c6c 6f77   from the Yellow
-0000cce0: 446f 6720 4f62 6a65 6374 2053 746f 7265  Dog Object Store
-0000ccf0: 2074 6f20 6c6f 6361 6c20 7374 6f72 6167   to local storag
-0000cd00: 652e 0a0a 2323 2320 4669 6c65 7320 5570  e...### Files Up
-0000cd10: 6c6f 6164 6564 2074 6f20 7468 6520 4f62  loaded to the Ob
-0000cd20: 6a65 6374 2053 746f 7265 2066 726f 6d20  ject Store from 
-0000cd30: 4c6f 6361 6c20 5374 6f72 6167 650a 0a23  Local Storage..#
-0000cd40: 2323 2320 4669 6c65 7320 696e 2074 6865  ### Files in the
-0000cd50: 2060 696e 7075 7473 6020 4c69 7374 0a0a   `inputs` List..
-0000cd60: 5768 656e 2061 2057 6f72 6b20 5265 7175  When a Work Requ
-0000cd70: 6972 656d 656e 7420 6973 2073 7562 6d69  irement is submi
-0000cd80: 7474 6564 2075 7369 6e67 2060 7964 2d73  tted using `yd-s
-0000cd90: 7562 6d69 7460 2c20 6669 6c65 7320 6172  ubmit`, files ar
-0000cda0: 6520 7570 6c6f 6164 6564 2074 6f20 7468  e uploaded to th
-0000cdb0: 6520 5965 6c6c 6f77 446f 6720 4f62 6a65  e YellowDog Obje
-0000cdc0: 6374 2053 746f 7265 2069 6620 7468 6579  ct Store if they
-0000cdd0: 2772 6520 696e 636c 7564 6564 2069 6e20  're included in 
-0000cde0: 7468 6520 6c69 7374 206f 6620 6669 6c65  the list of file
-0000cdf0: 7320 696e 2074 6865 2060 696e 7075 7473  s in the `inputs
-0000ce00: 6020 7072 6f70 6572 7479 2e20 2846 6f72  ` property. (For
-0000ce10: 2074 6865 2063 6173 6520 6f66 2074 6865   the case of the
-0000ce20: 2060 6261 7368 6020 5461 736b 2054 7970   `bash` Task Typ
-0000ce30: 652c 2074 6865 2073 6372 6970 7420 7370  e, the script sp
-0000ce40: 6563 6966 6965 6420 696e 2074 6865 2060  ecified in the `
-0000ce50: 6578 6563 7574 6162 6c65 6020 7072 6f70  executable` prop
-0000ce60: 6572 7479 2069 7320 616c 736f 2061 7574  erty is also aut
-0000ce70: 6f6d 6174 6963 616c 6c79 2075 706c 6f61  omatically uploa
-0000ce80: 6465 6420 6173 2061 2063 6f6e 7665 6e69  ded as a conveni
-0000ce90: 656e 6365 2c20 6576 656e 2069 6620 6e6f  ence, even if no
-0000cea0: 7420 696e 636c 7564 6564 2069 6e20 7468  t included in th
-0000ceb0: 6520 6069 6e70 7574 7360 206c 6973 742e  e `inputs` list.
-0000cec0: 290a 0a46 696c 6573 2061 7265 2075 706c  )..Files are upl
-0000ced0: 6f61 6465 6420 746f 2074 6865 204e 616d  oaded to the Nam
-0000cee0: 6573 7061 6365 2073 7065 6369 6669 6564  espace specified
-0000cef0: 2069 6e20 7468 6520 636f 6e66 6967 7572   in the configur
-0000cf00: 6174 696f 6e2e 2057 6974 6869 6e20 7468  ation. Within th
-0000cf10: 6520 4e61 6d65 7370 6163 652c 2065 6163  e Namespace, eac
-0000cf20: 6820 576f 726b 2052 6571 7569 7265 6d65  h Work Requireme
-0000cf30: 6e74 2068 6173 2061 2073 6570 6172 6174  nt has a separat
-0000cf40: 6520 666f 6c64 6572 2074 6861 7420 7368  e folder that sh
-0000cf50: 6172 6573 2074 6865 206e 616d 6520 6f66  ares the name of
-0000cf60: 2074 6865 2057 6f72 6b20 5265 7175 6972   the Work Requir
-0000cf70: 656d 656e 742c 2061 6e64 2069 6e20 7768  ement, and in wh
-0000cf80: 6963 6820 616c 6c20 6669 6c65 7320 7265  ich all files re
-0000cf90: 6c61 7465 6420 746f 2074 6865 2057 6f72  lated to the Wor
-0000cfa0: 6b20 5265 7175 6972 656d 656e 7420 6172  k Requirement ar
-0000cfb0: 6520 7374 6f72 6564 2e0a 0a31 2e20 4669  e stored...1. Fi
-0000cfc0: 6c65 7320 746f 2062 6520 7570 6c6f 6164  les to be upload
-0000cfd0: 6564 2074 6861 7420 6172 6520 696e 2074  ed that are in t
-0000cfe0: 6865 202a 2a73 616d 6520 6469 7265 6374  he **same direct
-0000cff0: 6f72 7920 6173 2074 6865 2057 6f72 6b20  ory as the Work 
-0000d000: 5265 7175 6972 656d 656e 7420 7370 6563  Requirement spec
-0000d010: 6966 6963 6174 696f 6e2a 2a20 2874 6865  ification** (the
-0000d020: 2054 4f4d 4c20 6f72 204a 534f 4e20 6669   TOML or JSON fi
-0000d030: 6c65 2920 6172 6520 7570 6c6f 6164 6564  le) are uploaded
-0000d040: 2074 6f20 7468 6520 726f 6f74 206f 6620   to the root of 
-0000d050: 7468 6520 576f 726b 2052 6571 7569 7265  the Work Require
-0000d060: 6d65 6e74 2066 6f6c 6465 722e 0a0a 0a32  ment folder....2
-0000d070: 2e20 4669 6c65 7320 746f 2062 6520 7570  . Files to be up
-0000d080: 6c6f 6164 6564 2074 6861 7420 6172 6520  loaded that are 
-0000d090: 696e 202a 2a73 7562 6469 7265 6374 6f72  in **subdirector
-0000d0a0: 6965 7320 6265 6c6f 7720 7468 6520 576f  ies below the Wo
-0000d0b0: 726b 2052 6571 7569 7265 6d65 6e74 2073  rk Requirement s
-0000d0c0: 7065 6369 6669 6361 7469 6f6e 2c20 6f72  pecification, or
-0000d0d0: 2077 6865 7265 2061 6273 6f6c 7574 6520   where absolute 
-0000d0e0: 7061 7468 6e61 6d65 7320 6172 6520 7375  pathnames are su
-0000d0f0: 7070 6c69 6564 2a2a 2061 7265 2070 6c61  pplied** are pla
-0000d100: 6365 6420 696e 2074 6865 204f 626a 6563  ced in the Objec
-0000d110: 7420 5374 6f72 6520 696e 2064 6972 6563  t Store in direc
-0000d120: 746f 7269 6573 2074 6861 7420 6d69 7272  tories that mirr
-0000d130: 6f72 2074 6865 6972 206c 6f63 616c 2073  or their local s
-0000d140: 746f 7261 6765 206c 6f63 6174 696f 6e73  torage locations
-0000d150: 2e0a 0a0a 332e 2046 696c 6573 2074 6f20  ....3. Files to 
-0000d160: 6265 2075 706c 6f61 6465 6420 7468 6174  be uploaded that
-0000d170: 2061 7265 2069 6e20 2a2a 6469 7265 6374   are in **direct
-0000d180: 6f72 6965 7320 7265 6c61 7469 7665 2074  ories relative t
-0000d190: 6f20 7468 6520 576f 726b 2052 6571 7569  o the Work Requi
-0000d1a0: 7265 6d65 6e74 2073 7065 6369 6669 6361  rement specifica
-0000d1b0: 7469 6f6e 2c20 7573 696e 6720 602e 2e60  tion, using `..`
-0000d1c0: 2072 656c 6174 6976 6520 7061 7468 732a   relative paths*
-0000d1d0: 2a20 6172 6520 706c 6163 6564 2069 6e20  * are placed in 
-0000d1e0: 4f62 6a65 6374 2053 746f 7265 2064 6972  Object Store dir
-0000d1f0: 6563 746f 7269 6573 2069 6e20 7768 6963  ectories in whic
-0000d200: 6820 7468 6520 602e 2e60 2070 6172 7473  h the `..` parts
-0000d210: 206f 6620 7468 6520 7061 7468 6e61 6d65   of the pathname
-0000d220: 2061 7265 2072 6570 6c61 6365 6420 7769   are replaced wi
-0000d230: 7468 2061 6e20 696e 7465 6765 7220 636f  th an integer co
-0000d240: 756e 7420 6f66 2074 6865 206e 756d 6265  unt of the numbe
-0000d250: 7220 6f66 2060 2e2e 6020 656e 7472 6965  r of `..` entrie
-0000d260: 7320 2862 6563 6175 7365 2077 6520 6361  s (because we ca
-0000d270: 6e27 7420 7573 6520 7468 6520 602e 2e60  n't use the `..`
-0000d280: 2072 656c 6174 6976 6520 666f 726d 2069   relative form i
-0000d290: 6e20 7468 6520 4f62 6a65 6374 2053 746f  n the Object Sto
-0000d2a0: 7265 292e 0a0a 4173 7375 6d69 6e67 2061  re)...Assuming a
-0000d2b0: 204e 616d 6573 7061 6365 2063 616c 6c65   Namespace calle
-0000d2c0: 6420 6064 6576 656c 6f70 6d65 6e74 6020  d `development` 
-0000d2d0: 616e 6420 6120 576f 726b 2052 6571 7569  and a Work Requi
-0000d2e0: 7265 6d65 6e74 206e 616d 6564 2060 7465  rement named `te
-0000d2f0: 7374 7275 6e5f 3232 3131 3038 2d31 3230  strun_221108-120
-0000d300: 3430 342d 3764 3260 2c20 7468 6520 666f  404-7d2`, the fo
-0000d310: 6c6c 6f77 696e 6720 6c6f 6361 7469 6f6e  llowing location
-0000d320: 7320 6172 6520 7573 6564 2077 6865 6e20  s are used when 
-0000d330: 7570 6c6f 6164 696e 6720 6669 6c65 7320  uploading files 
-0000d340: 666f 6c6c 6f77 696e 6720 7468 6520 7061  following the pa
-0000d350: 7474 6572 6e73 2061 626f 7665 3a0a 0a60  tterns above:..`
-0000d360: 6060 7368 656c 6c0a 2269 6e70 7574 7322  ``shell."inputs"
-0000d370: 203a 205b 2266 696c 655f 312e 7478 7422   : ["file_1.txt"
-0000d380: 5d20 2d3e 2064 6576 656c 6f70 6d65 6e74  ] -> development
-0000d390: 3a3a 7465 7374 7275 6e5f 3232 3131 3038  ::testrun_221108
-0000d3a0: 2d31 3230 3430 342d 3764 322f 6669 6c65  -120404-7d2/file
-0000d3b0: 5f31 2e74 7874 0a22 696e 7075 7473 2220  _1.txt."inputs" 
-0000d3c0: 3a20 5b22 6465 762f 6669 6c65 5f31 2e74  : ["dev/file_1.t
-0000d3d0: 7874 225d 202d 3e20 6465 7665 6c6f 706d  xt"] -> developm
-0000d3e0: 656e 743a 3a74 6573 7472 756e 5f32 3231  ent::testrun_221
-0000d3f0: 3130 382d 3132 3034 3034 2d37 6432 2f64  108-120404-7d2/d
-0000d400: 6576 2f66 696c 655f 312e 7478 740a 2269  ev/file_1.txt."i
-0000d410: 6e70 7574 7322 203a 205b 222f 686f 6d65  nputs" : ["/home
-0000d420: 2f64 6576 2f66 696c 655f 312e 7478 7422  /dev/file_1.txt"
-0000d430: 5d20 2d3e 2064 6576 656c 6f70 6d65 6e74  ] -> development
-0000d440: 3a3a 7465 7374 7275 6e5f 3232 3131 3038  ::testrun_221108
-0000d450: 2d31 3230 3430 342d 3764 322f 686f 6d65  -120404-7d2/home
-0000d460: 2f64 6576 2f66 696c 655f 312e 7478 740a  /dev/file_1.txt.
-0000d470: 2269 6e70 7574 7322 203a 205b 222e 2e2f  "inputs" : ["../
-0000d480: 6465 762f 6669 6c65 5f31 2e74 7874 225d  dev/file_1.txt"]
-0000d490: 202d 3e20 6465 7665 6c6f 706d 656e 743a   -> development:
-0000d4a0: 3a74 6573 7472 756e 5f32 3231 3130 382d  :testrun_221108-
-0000d4b0: 3132 3034 3034 2d37 6432 2f31 2f64 6576  120404-7d2/1/dev
-0000d4c0: 2f66 696c 655f 312e 7478 740a 2269 6e70  /file_1.txt."inp
-0000d4d0: 7574 7322 203a 205b 222e 2e2f 2e2e 2f64  uts" : ["../../d
-0000d4e0: 6576 2f66 696c 655f 312e 7478 7422 5d20  ev/file_1.txt"] 
-0000d4f0: 2d3e 2064 6576 656c 6f70 6d65 6e74 3a3a  -> development::
-0000d500: 7465 7374 7275 6e5f 3232 3131 3038 2d31  testrun_221108-1
-0000d510: 3230 3430 342d 3764 322f 322f 6465 762f  20404-7d2/2/dev/
-0000d520: 6669 6c65 5f31 2e74 7874 0a60 6060 0a0a  file_1.txt.```..
-0000d530: 2a2a 5573 696e 6720 6066 6c61 7474 656e  **Using `flatten
-0000d540: 5570 6c6f 6164 5061 7468 7360 2a2a 0a0a  UploadPaths`**..
-0000d550: 5468 6520 6066 6c61 7474 656e 5570 6c6f  The `flattenUplo
-0000d560: 6164 5061 7468 7360 2070 726f 7065 7274  adPaths` propert
-0000d570: 7920 6361 6e20 6265 2075 7365 6420 746f  y can be used to
-0000d580: 2073 7570 7072 6573 7320 7468 6520 6d69   suppress the mi
-0000d590: 7272 6f72 696e 6720 6f66 2061 6e79 206c  rroring of any l
-0000d5a0: 6f63 616c 2064 6972 6563 746f 7279 2073  ocal directory s
-0000d5b0: 7472 7563 7475 7265 2077 6865 6e20 7570  tructure when up
-0000d5c0: 6c6f 6164 696e 6720 6669 6c65 7320 746f  loading files to
-0000d5d0: 2074 6865 204f 626a 6563 7420 5374 6f72   the Object Stor
-0000d5e0: 652e 2049 6620 7365 7420 746f 2060 7472  e. If set to `tr
-0000d5f0: 7565 602c 2061 6c6c 2066 696c 6573 2077  ue`, all files w
-0000d600: 696c 6c20 6265 2075 706c 6f61 6465 6420  ill be uploaded 
-0000d610: 746f 2074 6865 2072 6f6f 7420 6f66 2074  to the root of t
-0000d620: 6865 2057 6f72 6b20 5265 7175 6972 656d  he Work Requirem
-0000d630: 656e 7420 666f 6c64 6572 2e20 466f 7220  ent folder. For 
-0000d640: 6578 616d 706c 653a 0a0a 6060 6073 6865  example:..```she
-0000d650: 6c6c 0a22 696e 7075 7473 2220 3a20 5b22  ll."inputs" : ["
-0000d660: 6669 6c65 5f31 2e74 7874 225d 202d 3e20  file_1.txt"] -> 
-0000d670: 6465 7665 6c6f 706d 656e 743a 3a74 6573  development::tes
-0000d680: 7472 756e 5f32 3231 3130 382d 3132 3034  trun_221108-1204
-0000d690: 3034 2d37 6432 2f66 696c 655f 312e 7478  04-7d2/file_1.tx
-0000d6a0: 740a 2269 6e70 7574 7322 203a 205b 2264  t."inputs" : ["d
-0000d6b0: 6576 2f66 696c 655f 312e 7478 7422 5d20  ev/file_1.txt"] 
-0000d6c0: 2d3e 2064 6576 656c 6f70 6d65 6e74 3a3a  -> development::
-0000d6d0: 7465 7374 7275 6e5f 3232 3131 3038 2d31  testrun_221108-1
-0000d6e0: 3230 3430 342d 3764 322f 6669 6c65 5f31  20404-7d2/file_1
-0000d6f0: 2e74 7874 0a22 696e 7075 7473 2220 3a20  .txt."inputs" : 
-0000d700: 5b22 2f68 6f6d 652f 6465 762f 6669 6c65  ["/home/dev/file
-0000d710: 5f31 2e74 7874 225d 202d 3e20 6465 7665  _1.txt"] -> deve
-0000d720: 6c6f 706d 656e 743a 3a74 6573 7472 756e  lopment::testrun
-0000d730: 5f32 3231 3130 382d 3132 3034 3034 2d37  _221108-120404-7
-0000d740: 6432 2f66 696c 655f 312e 7478 740a 2269  d2/file_1.txt."i
-0000d750: 6e70 7574 7322 203a 205b 222e 2e2f 6465  nputs" : ["../de
-0000d760: 762f 6669 6c65 5f31 2e74 7874 225d 202d  v/file_1.txt"] -
-0000d770: 3e20 6465 7665 6c6f 706d 656e 743a 3a74  > development::t
-0000d780: 6573 7472 756e 5f32 3231 3130 382d 3132  estrun_221108-12
-0000d790: 3034 3034 2d37 6432 2f66 696c 655f 312e  0404-7d2/file_1.
-0000d7a0: 7478 740a 2269 6e70 7574 7322 203a 205b  txt."inputs" : [
-0000d7b0: 222e 2e2f 2e2e 2f64 6576 2f66 696c 655f  "../../dev/file_
-0000d7c0: 312e 7478 7422 5d20 2d3e 2064 6576 656c  1.txt"] -> devel
-0000d7d0: 6f70 6d65 6e74 3a3a 7465 7374 7275 6e5f  opment::testrun_
-0000d7e0: 3232 3131 3038 2d31 3230 3430 342d 3764  221108-120404-7d
-0000d7f0: 322f 6669 6c65 5f31 2e74 7874 0a60 6060  2/file_1.txt.```
-0000d800: 0a0a 5468 6520 7072 6f70 6572 7479 2064  ..The property d
-0000d810: 6566 6175 6c74 2069 7320 6066 616c 7365  efault is `false
-0000d820: 602e 2054 6869 7320 7072 6f70 6572 7479  `. This property
-0000d830: 202a 2a63 616e 206f 6e6c 7920 6265 2073   **can only be s
-0000d840: 6574 2061 7420 7468 6520 576f 726b 2052  et at the Work R
-0000d850: 6571 7569 7265 6d65 6e74 206c 6576 656c  equirement level
-0000d860: 2a2a 2061 6e64 2077 696c 6c20 7468 6572  ** and will ther
-0000d870: 6566 6f72 6520 6170 706c 7920 746f 2061  efore apply to a
-0000d880: 6c6c 2054 6173 6b20 4772 6f75 7073 2061  ll Task Groups a
-0000d890: 6e64 2054 6173 6b73 2077 6974 6869 6e20  nd Tasks within 
-0000d8a0: 6120 576f 726b 2052 6571 7569 7265 6d65  a Work Requireme
-0000d8b0: 6e74 2e0a 0a57 6865 6e20 6669 6c65 7320  nt...When files 
-0000d8c0: 6170 7065 6172 2069 6e20 7468 6520 6069  appear in the `i
-0000d8d0: 6e70 7574 7360 206c 6973 742c 2074 6865  nputs` list, the
-0000d8e0: 7920 6172 6520 616c 736f 2061 7574 6f6d  y are also autom
-0000d8f0: 6174 6963 616c 6c79 2061 6464 6564 2074  atically added t
-0000d900: 6f20 7468 6520 6c69 7374 206f 6620 6669  o the list of fi
-0000d910: 6c65 7320 7265 7175 6972 6564 2062 7920  les required by 
-0000d920: 7468 6520 7265 6c65 7661 6e74 2054 6173  the relevant Tas
-0000d930: 6b28 7329 2061 7320 6056 6572 6966 7941  k(s) as `VerifyA
-0000d940: 7453 7461 7274 6020 6465 7065 6e64 656e  tStart` dependen
-0000d950: 6369 6573 2e0a 0a23 2323 2320 4669 6c65  cies...#### File
-0000d960: 7320 696e 2074 6865 2060 7570 6c6f 6164  s in the `upload
-0000d970: 4669 6c65 7360 204c 6973 740a 0a54 6865  Files` List..The
-0000d980: 2060 7570 6c6f 6164 4669 6c65 7360 2070   `uploadFiles` p
-0000d990: 726f 7065 7274 7920 616c 6c6f 7773 206d  roperty allows m
-0000d9a0: 6f72 6520 666c 6578 6962 6c65 2063 6f6e  ore flexible con
-0000d9b0: 7472 6f6c 206f 7665 7220 7468 6520 6669  trol over the fi
-0000d9c0: 6c65 7320 746f 2062 6520 7570 6c6f 6164  les to be upload
-0000d9d0: 6564 2066 726f 6d20 6c6f 6361 6c20 7374  ed from local st
-0000d9e0: 6f72 6167 6520 746f 2074 6865 204f 626a  orage to the Obj
-0000d9f0: 6563 7420 5374 6f72 6520 7768 656e 2060  ect Store when `
-0000da00: 7964 2d73 7562 6d69 7460 2069 7320 7275  yd-submit` is ru
-0000da10: 6e2e 2054 6865 2070 726f 7065 7274 7920  n. The property 
-0000da20: 6361 6e20 6265 2075 7365 6420 6174 2061  can be used at a
-0000da30: 6c6c 2057 6f72 6b20 5265 7175 6972 656d  ll Work Requirem
-0000da40: 656e 7420 6c65 7665 6c73 2c20 6672 6f6d  ent levels, from
-0000da50: 2074 6865 2054 4f4d 4c20 6669 6c65 2074   the TOML file t
-0000da60: 6872 6f75 6768 2074 6f20 696e 6469 7669  hrough to indivi
-0000da70: 6475 616c 2054 6173 6b20 7370 6563 6966  dual Task specif
-0000da80: 6963 6174 696f 6e73 2e0a 0a54 6865 2070  ications...The p
-0000da90: 726f 7065 7274 7920 6973 2073 7570 706c  roperty is suppl
-0000daa0: 6965 6420 6173 2061 206c 6973 7420 6f66  ied as a list of
-0000dab0: 2064 6963 7469 6f6e 6172 7920 6974 656d   dictionary item
-0000dac0: 732c 2065 6163 6820 6f66 2077 6869 6368  s, each of which
-0000dad0: 206d 7573 7420 696e 636c 7564 6520 7468   must include th
-0000dae0: 6520 7072 6f70 6572 7469 6573 2060 6c6f  e properties `lo
-0000daf0: 6361 6c50 6174 6860 2061 6e64 2060 7570  calPath` and `up
-0000db00: 6c6f 6164 5061 7468 602e 200a 0a2d 2060  loadPath`. ..- `
-0000db10: 6c6f 6361 6c50 6174 6860 2073 7065 6369  localPath` speci
-0000db20: 6669 6573 2074 6865 2070 6174 686e 616d  fies the pathnam
-0000db30: 6520 6f66 2074 6865 2066 696c 6520 6f6e  e of the file on
-0000db40: 206c 6f63 616c 2073 746f 7261 6765 0a2d   local storage.-
-0000db50: 2060 7570 6c6f 6164 5061 7468 6020 7370   `uploadPath` sp
-0000db60: 6563 6966 6965 7320 7468 6520 6e61 6d65  ecifies the name
-0000db70: 2061 6e64 206c 6f63 6174 696f 6e20 6f66   and location of
-0000db80: 2074 6865 2066 696c 6527 7320 6465 7374   the file's dest
-0000db90: 696e 6174 696f 6e20 696e 2074 6865 204f  ination in the O
-0000dba0: 626a 6563 7420 5374 6f72 650a 0a46 6f72  bject Store..For
-0000dbb0: 2065 7861 6d70 6c65 2c20 696e 2054 4f4d   example, in TOM
-0000dbc0: 4c3a 0a60 6060 746f 6d6c 0a75 706c 6f61  L:.```toml.uploa
-0000dbd0: 6446 696c 6573 203d 205b 0a20 2020 207b  dFiles = [.    {
-0000dbe0: 6c6f 6361 6c50 6174 6820 3d20 2266 696c  localPath = "fil
-0000dbf0: 655f 312e 7478 7422 2c20 7570 6c6f 6164  e_1.txt", upload
-0000dc00: 5061 7468 203d 2022 6669 6c65 5f31 2e74  Path = "file_1.t
-0000dc10: 7874 227d 2c0a 2020 2020 7b6c 6f63 616c  xt"},.    {local
-0000dc20: 5061 7468 203d 2022 6469 725f 322f 6669  Path = "dir_2/fi
-0000dc30: 6c65 5f32 2e74 7874 222c 2075 706c 6f61  le_2.txt", uploa
-0000dc40: 6450 6174 6820 3d20 223a 3a66 696c 655f  dPath = "::file_
-0000dc50: 322e 7478 7422 7d2c 0a20 2020 207b 6c6f  2.txt"},.    {lo
-0000dc60: 6361 6c50 6174 6820 3d20 2266 696c 655f  calPath = "file_
-0000dc70: 332e 7478 7422 2c20 7570 6c6f 6164 5061  3.txt", uploadPa
-0000dc80: 7468 203d 2022 6f74 6865 725f 6e61 6d65  th = "other_name
-0000dc90: 7370 6163 653a 3a66 696c 655f 332e 7478  space::file_3.tx
-0000dca0: 7422 7d0a 5d0a 6060 600a 416e 6420 696e  t"}.].```.And in
-0000dcb0: 204a 534f 4e2c 2077 6974 6820 7468 6520   JSON, with the 
-0000dcc0: 7072 6f70 6572 7479 2073 6574 2061 7420  property set at 
-0000dcd0: 7468 6520 5461 736b 206c 6576 656c 2c20  the Task level, 
-0000dce0: 7468 6520 7361 6d65 2073 7065 6369 6669  the same specifi
-0000dcf0: 6361 7469 6f6e 2077 6f75 6c64 2062 653a  cation would be:
-0000dd00: 0a60 6060 6a73 6f6e 0a7b 0a20 2022 7461  .```json.{.  "ta
-0000dd10: 736b 4772 6f75 7073 223a 205b 0a20 2020  skGroups": [.   
-0000dd20: 207b 0a20 2020 2020 2022 7461 736b 7322   {.      "tasks"
-0000dd30: 3a20 5b0a 2020 2020 2020 2020 7b0a 2020  : [.        {.  
-0000dd40: 2020 2020 2020 2020 2275 706c 6f61 6446          "uploadF
-0000dd50: 696c 6573 223a 205b 0a20 2020 2020 2020  iles": [.       
-0000dd60: 2020 2020 207b 226c 6f63 616c 5061 7468       {"localPath
-0000dd70: 223a 2022 6669 6c65 5f31 2e74 7874 222c  ": "file_1.txt",
-0000dd80: 2022 7570 6c6f 6164 5061 7468 223a 2022   "uploadPath": "
-0000dd90: 6669 6c65 5f31 2e74 7874 227d 2c0a 2020  file_1.txt"},.  
-0000dda0: 2020 2020 2020 2020 2020 7b22 6c6f 6361            {"loca
-0000ddb0: 6c50 6174 6822 3a20 2264 6972 5f32 2f66  lPath": "dir_2/f
-0000ddc0: 696c 655f 322e 7478 7422 2c20 2275 706c  ile_2.txt", "upl
-0000ddd0: 6f61 6450 6174 6822 3a20 223a 3a66 696c  oadPath": "::fil
-0000dde0: 655f 322e 7478 7422 7d2c 0a20 2020 2020  e_2.txt"},.     
-0000ddf0: 2020 2020 2020 207b 226c 6f63 616c 5061         {"localPa
-0000de00: 7468 223a 2022 6669 6c65 5f33 2e74 7874  th": "file_3.txt
-0000de10: 222c 2022 7570 6c6f 6164 5061 7468 223a  ", "uploadPath":
-0000de20: 2022 6f74 6865 725f 6e61 6d65 7370 6163   "other_namespac
-0000de30: 653a 3a66 696c 655f 332e 7478 7422 7d0a  e::file_3.txt"}.
-0000de40: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
-0000de50: 2020 2020 7d0a 2020 2020 2020 5d0a 2020      }.      ].  
-0000de60: 2020 7d0a 2020 5d0a 7d0a 6060 600a 5468    }.  ].}.```.Th
-0000de70: 6520 6075 706c 6f61 6446 696c 6573 6020  e `uploadFiles` 
-0000de80: 7072 6f70 6572 7479 2063 616e 2061 6c73  property can als
-0000de90: 6f20 6265 2073 6574 2061 7420 7468 6520  o be set at the 
-0000dea0: 576f 726b 2052 6571 7569 7265 6d65 6e74  Work Requirement
-0000deb0: 2061 6e64 2054 6173 6b20 4772 6f75 7020   and Task Group 
-0000dec0: 6c65 7665 6c73 2c20 616e 6420 7072 6f70  levels, and prop
-0000ded0: 6572 7479 2069 6e68 6572 6974 616e 6365  erty inheritance
-0000dee0: 206f 7065 7261 7465 7320 6173 206e 6f72   operates as nor
-0000def0: 6d61 6c2e 0a0a 466f 7220 6075 706c 6f61  mal...For `uploa
-0000df00: 6450 6174 6860 2c20 7468 6520 7361 6d65  dPath`, the same
-0000df10: 2060 3a3a 6020 6e61 6d69 6e67 2063 6f6e   `::` naming con
-0000df20: 7665 6e74 696f 6e20 6973 2061 7661 696c  vention is avail
-0000df30: 6162 6c65 2061 7320 6973 2075 7365 6420  able as is used 
-0000df40: 696e 2074 6865 2060 7665 7269 6679 4174  in the `verifyAt
-0000df50: 5374 6172 7460 2c20 6076 6572 6966 7957  Start`, `verifyW
-0000df60: 6169 7460 2061 6e64 2060 696e 7075 7473  ait` and `inputs
-0000df70: 4f70 7469 6f6e 616c 6020 7072 6f70 6572  Optional` proper
-0000df80: 7469 6573 2064 6973 6375 7373 6564 2062  ties discussed b
-0000df90: 656c 6f77 3a0a 0a2d 2049 6620 603a 3a60  elow:..- If `::`
-0000dfa0: 2069 7320 6e6f 7420 7573 6564 2c20 7468   is not used, th
-0000dfb0: 656e 2074 6865 2066 696c 6520 6973 2075  en the file is u
-0000dfc0: 706c 6f61 6465 6420 7265 6c61 7469 7665  ploaded relative
-0000dfd0: 2074 6f20 7468 6520 6375 7272 656e 7420   to the current 
-0000dfe0: 6e61 6d65 7370 6163 6520 696e 2061 2064  namespace in a d
-0000dff0: 6972 6563 746f 7279 206e 616d 6564 2061  irectory named a
-0000e000: 6674 6572 2074 6865 206e 616d 6520 6f66  fter the name of
-0000e010: 2074 6865 2057 6f72 6b20 5265 7175 6972   the Work Requir
-0000e020: 656d 656e 740a 2d20 4966 2060 3a3a 6020  ement.- If `::` 
-0000e030: 6973 2075 7365 6420 6174 2074 6865 2073  is used at the s
-0000e040: 7461 7274 206f 6620 7468 6520 6075 706c  tart of the `upl
-0000e050: 6f61 6450 6174 6860 2c20 7468 6520 6669  oadPath`, the fi
-0000e060: 6c65 2069 7320 7570 6c6f 6164 6564 2072  le is uploaded r
-0000e070: 656c 6174 6976 6520 746f 2074 6865 2072  elative to the r
-0000e080: 6f6f 7420 6f66 2074 6865 2063 7572 7265  oot of the curre
-0000e090: 6e74 206e 616d 6573 7061 6365 0a2d 2049  nt namespace.- I
-0000e0a0: 6620 603c 6e61 6d65 7370 6163 653e 3a3a  f `<namespace>::
-0000e0b0: 6020 6973 2075 7365 6420 6174 2074 6865  ` is used at the
-0000e0c0: 2073 7461 7274 206f 6620 6075 706c 6f61   start of `uploa
-0000e0d0: 6450 6174 6860 2c20 7468 6520 6669 6c65  dPath`, the file
-0000e0e0: 2069 7320 7570 6c6f 6164 6564 2072 656c   is uploaded rel
-0000e0f0: 6174 6976 6520 746f 2074 6865 2072 6f6f  ative to the roo
-0000e100: 7420 6f66 2060 3c6e 616d 6573 7061 6365  t of `<namespace
-0000e110: 3e60 0a0a 4561 6368 2066 696c 6520 7370  >`..Each file sp
-0000e120: 6563 6966 6965 6420 696e 2074 6865 2060  ecified in the `
-0000e130: 7570 6c6f 6164 4669 6c65 7360 206c 6973  uploadFiles` lis
-0000e140: 7473 2077 696c 6c20 6f6e 6c79 2062 6520  ts will only be 
-0000e150: 7570 6c6f 6164 6564 206f 6e63 6520 746f  uploaded once to
-0000e160: 2065 6163 6820 756e 6971 7565 2075 706c   each unique upl
-0000e170: 6f61 6420 6c6f 6361 7469 6f6e 2066 6f72  oad location for
-0000e180: 2061 6e79 2067 6976 656e 2069 6e76 6f63   any given invoc
-0000e190: 6174 696f 6e20 6f66 2060 7964 2d73 7562  ation of `yd-sub
-0000e1a0: 6d69 7460 2e0a 0a49 6620 6120 6669 6c65  mit`...If a file
-0000e1b0: 2069 6e20 7468 6520 6075 706c 6f61 6446   in the `uploadF
-0000e1c0: 696c 6573 6020 6c69 7374 2069 7320 7265  iles` list is re
-0000e1d0: 7175 6972 6564 2062 7920 6120 5461 736b  quired by a Task
-0000e1e0: 2c20 6974 206d 7573 7420 7365 7061 7261  , it must separa
-0000e1f0: 7465 6c79 2062 6520 6164 6465 6420 746f  tely be added to
-0000e200: 2074 6865 2060 7665 7269 6679 4174 5374   the `verifyAtSt
-0000e210: 6172 7460 206f 7220 6076 6572 6966 7957  art` or `verifyW
-0000e220: 6169 7460 206c 6973 7473 2064 6973 6375  ait` lists discu
-0000e230: 7373 6564 2062 656c 6f77 2e20 5468 6973  ssed below. This
-0000e240: 2069 7320 6e6f 7420 646f 6e65 2061 7574   is not done aut
-0000e250: 6f6d 6174 6963 616c 6c79 2e20 4e6f 7465  omatically. Note
-0000e260: 2061 6c73 6f20 7468 6174 2074 6865 2060   also that the `
-0000e270: 666c 6174 7465 6e55 706c 6f61 6450 6174  flattenUploadPat
-0000e280: 6873 6020 7072 6f70 6572 7479 2069 7320  hs` property is 
-0000e290: 6967 6e6f 7265 6420 666f 7220 6669 6c65  ignored for file
-0000e2a0: 7320 696e 2074 6865 2060 7570 6c6f 6164  s in the `upload
-0000e2b0: 4669 6c65 7360 206c 6973 742e 0a0a 2323  Files` list...##
-0000e2c0: 2320 4669 6c65 2044 6570 656e 6465 6e63  # File Dependenc
-0000e2d0: 6965 7320 5573 696e 6720 6076 6572 6966  ies Using `verif
-0000e2e0: 7941 7453 7461 7274 6020 616e 6420 6076  yAtStart` and `v
-0000e2f0: 6572 6966 7957 6169 7460 0a0a 4974 2773  erifyWait`..It's
-0000e300: 2070 6f73 7369 626c 6520 746f 206d 616b   possible to mak
-0000e310: 6520 5461 736b 7320 6465 7065 6e64 656e  e Tasks dependen
-0000e320: 7420 6f6e 2074 6865 2070 7265 7365 6e63  t on the presenc
-0000e330: 6520 6f66 2066 696c 6573 2069 6e20 7468  e of files in th
-0000e340: 6520 4f62 6a65 6374 2053 746f 7265 2062  e Object Store b
-0000e350: 7920 7573 696e 6720 7468 6520 6076 6572  y using the `ver
-0000e360: 6966 7941 7453 7461 7274 6020 616e 6420  ifyAtStart` and 
-0000e370: 6076 6572 6966 7957 6169 7460 206c 6973  `verifyWait` lis
-0000e380: 7473 2e20 5468 6573 6520 6669 6c65 7320  ts. These files 
-0000e390: 6172 6520 6e6f 7420 6175 746f 6d61 7469  are not automati
-0000e3a0: 6361 6c6c 7920 7570 6c6f 6164 6564 2077  cally uploaded w
-0000e3b0: 6865 6e20 7573 696e 6720 6079 642d 7375  hen using `yd-su
-0000e3c0: 626d 6974 6020 736f 2061 7265 2065 6974  bmit` so are eit
-0000e3d0: 6865 7220 7570 6c6f 6164 6564 206d 616e  her uploaded man
-0000e3e0: 7561 6c6c 7920 2865 2e67 2e2c 2062 7920  ually (e.g., by 
-0000e3f0: 7573 696e 6720 6079 642d 7570 6c6f 6164  using `yd-upload
-0000e400: 6029 2c20 6f72 2061 7265 2063 7265 6174  `), or are creat
-0000e410: 6564 2061 7320 6120 7265 7375 6c74 206f  ed as a result o
-0000e420: 6620 7468 6520 6578 6563 7574 696f 6e20  f the execution 
-0000e430: 6f66 206f 7468 6572 2054 6173 6b73 2e0a  of other Tasks..
-0000e440: 0a4e 6f74 6520 7468 6174 2061 2067 6976  .Note that a giv
-0000e450: 656e 2066 696c 6520 6361 6e20 6f6e 6c79  en file can only
-0000e460: 2061 7070 6561 7220 696e 202a 6f6e 652a   appear in *one*
-0000e470: 206f 6620 7468 6520 6069 6e70 7574 7360   of the `inputs`
-0000e480: 2c20 6076 6572 6966 7941 7453 7461 7274  , `verifyAtStart
-0000e490: 6020 6f72 2060 7665 7269 6679 5761 6974  ` or `verifyWait
-0000e4a0: 6020 6c69 7374 732e 0a0a 5461 736b 7320  ` lists...Tasks 
-0000e4b0: 7769 7468 2060 7665 7269 6679 4174 5374  with `verifyAtSt
-0000e4c0: 6172 7460 2064 6570 656e 6465 6e63 6965  art` dependencie
-0000e4d0: 7320 7769 6c6c 2066 6169 6c20 696d 6d65  s will fail imme
-0000e4e0: 6469 6174 656c 7920 6966 2074 6865 2072  diately if the r
-0000e4f0: 6571 7569 7265 6420 6669 6c65 7320 6172  equired files ar
-0000e500: 6520 6e6f 7420 7072 6573 656e 7420 7768  e not present wh
-0000e510: 656e 2074 6865 2054 6173 6b20 6973 2073  en the Task is s
-0000e520: 7562 6d69 7474 6564 2e20 5461 736b 7320  ubmitted. Tasks 
-0000e530: 7769 7468 2060 7665 7269 6679 5761 6974  with `verifyWait
-0000e540: 6020 6465 7065 6e64 656e 6369 6573 2077  ` dependencies w
-0000e550: 696c 6c20 6e6f 7420 6265 636f 6d65 2060  ill not become `
-0000e560: 5245 4144 5960 2074 6f20 6265 2073 6368  READY` to be sch
-0000e570: 6564 756c 6564 2074 6f20 576f 726b 6572  eduled to Worker
-0000e580: 7320 756e 7469 6c20 7468 6520 6465 7065  s until the depe
-0000e590: 6e64 656e 6369 6573 2061 7265 2073 6174  ndencies are sat
-0000e5a0: 6973 6669 6564 2e0a 0a57 6865 6e20 7370  isfied...When sp
-0000e5b0: 6563 6966 7969 6e67 2066 696c 6573 2069  ecifying files i
-0000e5c0: 6e20 7468 6520 6076 6572 6966 7941 7453  n the `verifyAtS
-0000e5d0: 7461 7274 6020 616e 6420 6076 6572 6966  tart` and `verif
-0000e5e0: 7957 6169 7460 206c 6973 7473 2c20 6173  yWait` lists, as
-0000e5f0: 2077 6974 6820 7468 6520 6075 706c 6f61   with the `uploa
-0000e600: 6450 6174 6860 2070 726f 7065 7274 7920  dPath` property 
-0000e610: 6469 7363 7573 7365 6420 6162 6f76 652c  discussed above,
-0000e620: 2074 6865 2066 696c 6520 6c6f 6361 7469   the file locati
-0000e630: 6f6e 7320 6361 6e20 6265 2028 3129 2072  ons can be (1) r
-0000e640: 656c 6174 6976 6520 746f 2074 6865 2057  elative to the W
-0000e650: 6f72 6b20 5265 7175 6972 656d 656e 7420  ork Requirement 
-0000e660: 6e61 6d65 2069 6e20 7468 6520 6375 7272  name in the curr
-0000e670: 656e 7420 6e61 6d65 7370 6163 6520 2874  ent namespace (t
-0000e680: 6865 2064 6566 6175 6c74 292c 2028 3229  he default), (2)
-0000e690: 2072 656c 6174 6976 6520 746f 2074 6865   relative to the
-0000e6a0: 2072 6f6f 7420 6f66 2074 6865 2063 7572   root of the cur
-0000e6b0: 7265 6e74 206e 616d 6573 7061 6365 2c20  rent namespace, 
-0000e6c0: 6f72 2028 3329 2072 656c 6174 6976 6520  or (3) relative 
-0000e6d0: 746f 2074 6865 2072 6f6f 7420 6f66 2061  to the root of a
-0000e6e0: 2064 6966 6665 7265 6e74 206e 616d 6573   different names
-0000e6f0: 7061 6365 2069 6e20 7468 6520 7573 6572  pace in the user
-0000e700: 2773 2041 6363 6f75 6e74 2e0a 0a31 2e20  's Account...1. 
-0000e710: 466f 7220 6669 6c65 7320 7265 6c61 7469  For files relati
-0000e720: 7665 2074 6f20 7468 6520 576f 726b 2052  ve to the Work R
-0000e730: 6571 7569 7265 6d65 6e74 206e 616d 6520  equirement name 
-0000e740: 696e 2074 6865 2063 7572 7265 6e74 206e  in the current n
-0000e750: 616d 6573 7061 6365 2c20 6a75 7374 2075  amespace, just u
-0000e760: 7365 2074 6865 2066 696c 6520 7061 7468  se the file path
-0000e770: 2c20 652e 672e 0a60 6060 7368 656c 6c0a  , e.g..```shell.
-0000e780: 2276 6572 6966 7957 6169 7422 3a20 5b22  "verifyWait": ["
-0000e790: 6669 6c65 5f31 2e74 7874 225d 202d 3e20  file_1.txt"] -> 
-0000e7a0: 6465 7665 6c6f 706d 656e 743a 7465 7374  development:test
-0000e7b0: 7275 6e5f 3232 3131 3038 2d31 3230 3430  run_221108-12040
-0000e7c0: 342d 3764 322f 6669 6c65 5f31 2e74 7874  4-7d2/file_1.txt
-0000e7d0: 0a60 6060 0a0a 322e 2046 6f72 2066 696c  .```..2. For fil
-0000e7e0: 6573 2072 656c 6174 6976 6520 746f 2074  es relative to t
-0000e7f0: 6865 2072 6f6f 7420 6f66 2074 6865 2063  he root of the c
-0000e800: 7572 7265 6e74 206e 616d 6573 7061 6365  urrent namespace
-0000e810: 2c20 7072 6566 6978 2074 6865 2066 696c  , prefix the fil
-0000e820: 6520 7061 7468 2077 6974 6820 603a 3a60  e path with `::`
-0000e830: 2c20 652e 672e 0a60 6060 7368 656c 6c0a  , e.g..```shell.
-0000e840: 2276 6572 6966 7957 6169 7422 3a20 5b22  "verifyWait": ["
-0000e850: 3a3a 6669 6c65 5f31 2e74 7874 225d 202d  ::file_1.txt"] -
-0000e860: 3e20 6465 7665 6c6f 706d 656e 743a 6669  > development:fi
-0000e870: 6c65 5f31 2e74 7874 0a60 6060 0a0a 332e  le_1.txt.```..3.
-0000e880: 2046 6f72 2066 696c 6573 2072 656c 6174   For files relat
-0000e890: 6976 6520 746f 2074 6865 2072 6f6f 7420  ive to the root 
-0000e8a0: 6f66 2061 2064 6966 6665 7265 6e74 206e  of a different n
-0000e8b0: 616d 6573 7061 6365 2c20 7072 6566 6978  amespace, prefix
-0000e8c0: 2074 6865 2066 696c 6520 7061 7468 2077   the file path w
-0000e8d0: 6974 6820 7468 6520 6e61 6d65 7370 6163  ith the namespac
-0000e8e0: 6520 6e61 6d65 2061 6e64 2060 3a3a 602c  e name and `::`,
-0000e8f0: 2065 2e67 2e0a 6060 6073 6865 6c6c 0a22   e.g..```shell."
-0000e900: 7665 7269 6679 5761 6974 223a 205b 226f  verifyWait": ["o
-0000e910: 7468 6572 5f6e 616d 6573 7061 6365 3a3a  ther_namespace::
-0000e920: 6669 6c65 5f31 2e74 7874 225d 202d 3e20  file_1.txt"] -> 
-0000e930: 6f74 6865 725f 6e61 6d65 7370 6163 653a  other_namespace:
-0000e940: 6669 6c65 5f31 2e74 7874 0a60 6060 0a0a  file_1.txt.```..
-0000e950: 5468 6520 7573 6520 6f66 2074 6865 2074  The use of the t
-0000e960: 6872 6565 2064 6966 6665 7265 6e74 2066  hree different f
-0000e970: 6f72 6d73 2063 616e 2062 6520 6d69 7865  orms can be mixe
-0000e980: 6420 7769 7468 696e 2061 2073 696e 676c  d within a singl
-0000e990: 6520 6c69 7374 2c20 652e 672e 3a0a 6060  e list, e.g.:.``
-0000e9a0: 6073 6865 6c6c 0a22 7665 7269 6679 4174  `shell."verifyAt
-0000e9b0: 5374 6172 7422 3a20 5b22 6669 6c65 5f31  Start": ["file_1
-0000e9c0: 2e74 7874 222c 2022 3a3a 6469 725f 322f  .txt", "::dir_2/
-0000e9d0: 6669 6c65 5f32 2e74 7874 222c 2022 6f74  file_2.txt", "ot
-0000e9e0: 6865 725f 6e61 6d65 7370 6163 653a 3a64  her_namespace::d
-0000e9f0: 6972 5f33 2f66 696c 655f 332e 7478 7422  ir_3/file_3.txt"
-0000ea00: 5d0a 6060 600a 0a23 2323 2046 696c 6573  ].```..### Files
-0000ea10: 2044 6f77 6e6c 6f61 6465 6420 5573 696e   Downloaded Usin
-0000ea20: 6720 6069 6e70 7574 734f 7074 696f 6e61  g `inputsOptiona
-0000ea30: 6c60 0a0a 5468 6520 6069 6e70 7574 734f  l`..The `inputsO
-0000ea40: 7074 696f 6e61 6c60 2070 726f 7065 7274  ptional` propert
-0000ea50: 7920 776f 726b 7320 696e 2061 2073 696d  y works in a sim
-0000ea60: 696c 6172 2066 6173 6869 6f6e 2074 6f20  ilar fashion to 
-0000ea70: 7468 6520 6076 6572 6966 792a 6020 7072  the `verify*` pr
-0000ea80: 6f70 6572 7469 6573 2061 626f 7665 2c20  operties above, 
-0000ea90: 6275 7420 7468 6520 6669 6c65 7320 7370  but the files sp
-0000eaa0: 6563 6966 6965 6420 696e 2074 6869 7320  ecified in this 
-0000eab0: 6c69 7374 2061 7265 206f 7074 696f 6e61  list are optiona
-0000eac0: 6c2e 2054 6869 7320 7072 6f70 6572 7479  l. This property
-0000ead0: 2061 6c73 6f20 616c 6c6f 7773 2066 6f72   also allows for
-0000eae0: 2074 6865 2075 7365 206f 6620 7769 6c64   the use of wild
-0000eaf0: 6361 7264 7320 602a 6020 616e 6420 602a  cards `*` and `*
-0000eb00: 2a60 2074 6f20 636f 6c6c 6563 7420 6669  *` to collect fi
-0000eb10: 6c65 7320 7573 696e 6720 7769 6c64 6361  les using wildca
-0000eb20: 7264 2070 6174 6873 2e0a 0a23 2323 2046  rd paths...### F
-0000eb30: 696c 6573 2044 6f77 6e6c 6f61 6465 6420  iles Downloaded 
-0000eb40: 746f 2061 204e 6f64 6520 666f 7220 7573  to a Node for us
-0000eb50: 6520 696e 2054 6173 6b20 4578 6563 7574  e in Task Execut
-0000eb60: 696f 6e0a 0a57 6865 6e20 6120 5461 736b  ion..When a Task
-0000eb70: 2069 7320 6578 6563 7574 6564 2062 7920   is executed by 
-0000eb80: 6120 576f 726b 6572 206f 6e20 6120 4e6f  a Worker on a No
-0000eb90: 6465 2c20 6974 7320 7265 7175 6972 6564  de, its required
-0000eba0: 2066 696c 6573 2061 7265 2064 6f77 6e6c   files are downl
-0000ebb0: 6f61 6465 6420 6672 6f6d 2074 6865 204f  oaded from the O
-0000ebc0: 626a 6563 7420 5374 6f72 6520 7072 696f  bject Store prio
-0000ebd0: 7220 746f 2054 6173 6b20 6578 6563 7574  r to Task execut
-0000ebe0: 696f 6e2e 2041 6e79 2066 696c 6520 6c69  ion. Any file li
-0000ebf0: 7374 6564 2069 6e20 7468 6520 6069 6e70  sted in the `inp
-0000ec00: 7574 7360 2066 6f72 2061 2054 6173 6b20  uts` for a Task 
-0000ec10: 6973 2061 7373 756d 6564 2074 6f20 6265  is assumed to be
-0000ec20: 2072 6571 7569 7265 642c 2061 6c6f 6e67   required, along
-0000ec30: 2077 6974 6820 616e 7920 6164 6469 7469   with any additi
-0000ec40: 6f6e 616c 2066 696c 6573 2073 7065 6369  onal files speci
-0000ec50: 6669 6564 2069 6e20 7468 6520 6076 6572  fied in the `ver
-0000ec60: 6966 7941 7453 7461 7274 6020 616e 6420  ifyAtStart` and 
-0000ec70: 6076 6572 6966 7957 6169 7460 206c 6973  `verifyWait` lis
-0000ec80: 7473 2e20 4669 6c65 7320 7370 6563 6966  ts. Files specif
-0000ec90: 6965 6420 7573 696e 6720 7468 6520 6069  ied using the `i
-0000eca0: 6e70 7574 734f 7074 696f 6e61 6c60 2070  nputsOptional` p
-0000ecb0: 726f 7065 7274 7920 6172 6520 6f70 7469  roperty are opti
-0000ecc0: 6f6e 616c 6c79 2064 6f77 6e6c 6f61 6465  onally downloade
-0000ecd0: 6420 6672 6f6d 2074 6865 204f 626a 6563  d from the Objec
-0000ece0: 7420 5374 6f72 652e 2028 4e6f 7465 2074  t Store. (Note t
-0000ecf0: 6861 7420 6120 6669 6c65 2073 686f 756c  hat a file shoul
-0000ed00: 6420 6f6e 6c79 2061 7070 6561 7220 696e  d only appear in
-0000ed10: 206f 6e65 206f 6620 7468 6573 6520 666f   one of these fo
-0000ed20: 7572 206c 6973 7473 2c20 6f74 6865 7277  ur lists, otherw
-0000ed30: 6973 6520 6079 642d 7375 626d 6974 6020  ise `yd-submit` 
-0000ed40: 7769 6c6c 2072 6574 7572 6e20 616e 2065  will return an e
-0000ed50: 7272 6f72 2e29 0a0a 5768 656e 2061 2054  rror.)..When a T
-0000ed60: 6173 6b20 6973 2073 7461 7274 6564 2062  ask is started b
-0000ed70: 7920 7468 6520 4167 656e 742c 2069 7473  y the Agent, its
-0000ed80: 2077 6f72 6b69 6e67 2064 6972 6563 746f   working directo
-0000ed90: 7279 2068 6173 2061 2070 6174 7465 726e  ry has a pattern
-0000eda0: 2073 6f6d 6574 6869 6e67 206c 696b 653a   something like:
-0000edb0: 0a0a 602f 7661 722f 6f70 742f 7965 6c6c  ..`/var/opt/yell
-0000edc0: 6f77 646f 672f 7964 2d61 6765 6e74 2d34  owdog/yd-agent-4
-0000edd0: 2f64 6174 612f 776f 726b 6572 732f 312f  /data/workers/1/
-0000ede0: 7964 6964 5f74 6173 6b5f 4430 4430 4430  ydid_task_D0D0D0
-0000edf0: 5f36 3866 3565 3562 652d 6463 3933 2d34  _68f5e5be-dc93-4
-0000ee00: 3965 622d 6138 3234 2d31 6663 6462 3532  9eb-a824-1fcdb52
-0000ee10: 6639 3139 355f 315f 3160 0a0a 2860 7964  f9195_1_1`..(`yd
-0000ee20: 6964 5f74 6173 6b5f 4430 4430 4430 5f36  id_task_D0D0D0_6
-0000ee30: 3866 3565 3562 652d 6463 3933 2d34 3965  8f5e5be-dc93-49e
-0000ee40: 622d 6138 3234 2d31 6663 6462 3532 6639  b-a824-1fcdb52f9
-0000ee50: 3139 355f 315f 3160 2069 7320 616e 2065  195_1_1` is an e
-0000ee60: 7068 656d 6572 616c 2064 6972 6563 746f  phemeral directo
-0000ee70: 7279 2074 6861 7420 6973 2072 656d 6f76  ry that is remov
-0000ee80: 6564 2061 6674 6572 2074 6865 2054 6173  ed after the Tas
-0000ee90: 6b20 6669 6e69 7368 6573 2061 6e64 2061  k finishes and a
-0000eea0: 6e79 206f 7574 7075 7473 2068 6176 6520  ny outputs have 
-0000eeb0: 6265 656e 2075 706c 6f61 6465 642e 290a  been uploaded.).
-0000eec0: 0a46 696c 6573 2074 6861 7420 6172 6520  .Files that are 
-0000eed0: 646f 776e 6c6f 6164 6564 2062 7920 7468  downloaded by th
-0000eee0: 6520 4167 656e 7420 7072 696f 7220 746f  e Agent prior to
-0000eef0: 2054 6173 6b20 6578 6563 7574 696f 6e20   Task execution 
-0000ef00: 6172 6520 6c6f 6361 7465 6420 6173 2066  are located as f
-0000ef10: 6f6c 6c6f 7773 3a0a 0a31 2e20 4966 2074  ollows:..1. If t
-0000ef20: 6865 2060 666c 6174 7465 6e49 6e70 7574  he `flattenInput
-0000ef30: 5061 7468 7360 2070 726f 7065 7274 7920  Paths` property 
-0000ef40: 6973 2073 6574 2074 6f20 7468 6520 6465  is set to the de
-0000ef50: 6661 756c 7420 6f66 2060 6661 6c73 6560  fault of `false`
-0000ef60: 2066 6f72 2074 6865 2054 6173 6b2c 2074   for the Task, t
-0000ef70: 6865 2064 6f77 6e6c 6f61 6465 6420 6f62  he downloaded ob
-0000ef80: 6a65 6374 7320 6172 6520 706c 6163 6564  jects are placed
-0000ef90: 2069 6e20 7375 6264 6972 6563 746f 7269   in subdirectori
-0000efa0: 6573 2074 6861 7420 6d69 7272 6f72 2074  es that mirror t
-0000efb0: 686f 7365 2069 6e20 7468 6520 4f62 6a65  hose in the Obje
-0000efc0: 6374 2053 746f 7265 2c20 696e 636c 7564  ct Store, includ
-0000efd0: 696e 6720 7468 6520 576f 726b 2052 6571  ing the Work Req
-0000efe0: 7569 7265 6d65 6e74 206e 616d 652c 2073  uirement name, s
-0000eff0: 6974 7561 7465 6420 6265 6e65 6174 6820  ituated beneath 
-0000f000: 7468 6520 776f 726b 696e 6720 6469 7265  the working dire
-0000f010: 6374 6f72 792e 0a0a 0a32 2e20 4966 2074  ctory....2. If t
-0000f020: 6865 2060 666c 6174 7465 6e49 6e70 7574  he `flattenInput
-0000f030: 5061 7468 7360 2070 726f 7065 7274 7920  Paths` property 
-0000f040: 6973 2073 6574 2074 6f20 6074 7275 6560  is set to `true`
-0000f050: 2066 6f72 2074 6865 2054 6173 6b2c 2074   for the Task, t
-0000f060: 6865 2064 6f77 6e6c 6f61 6465 6420 6f62  he downloaded ob
-0000f070: 6a65 6374 7320 6172 6520 616c 6c20 706c  jects are all pl
-0000f080: 6163 6564 2064 6972 6563 746c 7920 696e  aced directly in
-0000f090: 2072 6f6f 7420 6f66 2074 6865 2054 6173   root of the Tas
-0000f0a0: 6b27 7320 776f 726b 696e 6720 6469 7265  k's working dire
-0000f0b0: 6374 6f72 792e 0a0a 466f 7220 6578 616d  ctory...For exam
-0000f0c0: 706c 653a 0a0a 6060 6073 6865 6c6c 0a49  ple:..```shell.I
-0000f0d0: 6620 7468 6520 7265 7175 6972 6564 206f  f the required o
-0000f0e0: 626a 6563 7420 6973 3a20 6465 7665 6c6f  bject is: develo
-0000f0f0: 706d 656e 743a 3a74 6573 7472 756e 5f32  pment::testrun_2
-0000f100: 3231 3130 382d 3132 3034 3034 2d37 6432  21108-120404-7d2
-0000f110: 2f64 6576 2f66 696c 655f 312e 7478 740a  /dev/file_1.txt.
-0000f120: 0a74 6865 6e2c 2069 6620 666c 6174 7465  .then, if flatte
-0000f130: 6e49 6e70 7574 5061 7468 7320 6973 2066  nInputPaths is f
-0000f140: 616c 7365 2c20 7468 6520 6669 6c65 2077  alse, the file w
-0000f150: 696c 6c20 6265 2066 6f75 6e64 2061 743a  ill be found at:
-0000f160: 0a20 2d3e 203c 776f 726b 696e 675f 6469  . -> <working_di
-0000f170: 7265 6374 6f72 793e 2f74 6573 7472 756e  rectory>/testrun
-0000f180: 5f32 3231 3130 382d 3132 3034 3034 2d37  _221108-120404-7
-0000f190: 6432 2f64 6576 2f66 696c 655f 312e 7478  d2/dev/file_1.tx
-0000f1a0: 740a 200a 656c 7365 2c20 6966 2066 6c61  t. .else, if fla
-0000f1b0: 7474 656e 496e 7075 7450 6174 6873 2069  ttenInputPaths i
-0000f1c0: 7320 7472 7565 2c20 7468 6520 6669 6c65  s true, the file
-0000f1d0: 2077 696c 6c20 6265 2066 6f75 6e64 2061   will be found a
-0000f1e0: 743a 0a20 2d3e 203c 776f 726b 696e 675f  t:. -> <working_
-0000f1f0: 6469 7265 6374 6f72 793e 2f66 696c 655f  directory>/file_
-0000f200: 312e 7478 7420 0a20 0a77 6865 7265 203c  1.txt . .where <
-0000f210: 776f 726b 696e 675f 6469 7265 6374 6f72  working_director
-0000f220: 793e 2069 733a 0a20 202f 7661 722f 6f70  y> is:.  /var/op
-0000f230: 742f 7965 6c6c 6f77 646f 672f 7964 2d61  t/yellowdog/yd-a
-0000f240: 6765 6e74 2d34 2f64 6174 612f 776f 726b  gent-4/data/work
-0000f250: 6572 732f 312f 7964 6964 5f74 6173 6b5f  ers/1/ydid_task_
-0000f260: 4430 4430 4430 5f36 3866 3565 3562 652d  D0D0D0_68f5e5be-
-0000f270: 6463 3933 2d34 3965 622d 6138 3234 2d31  dc93-49eb-a824-1
-0000f280: 6663 6462 3532 6639 3139 355f 315f 312f  fcdb52f9195_1_1/
-0000f290: 0a60 6060 0a0a 4e6f 7465 2074 6861 7420  .```..Note that 
-0000f2a0: 576f 726b 2052 6571 7569 7265 6d65 6e74  Work Requirement
-0000f2b0: 206e 616d 6520 2865 2e67 2e2c 2060 7465   name (e.g., `te
-0000f2c0: 7374 7275 6e5f 3232 3131 3038 2d31 3230  strun_221108-120
-0000f2d0: 3430 342d 3764 3260 2920 6973 2061 7661  404-7d2`) is ava
-0000f2e0: 696c 6162 6c65 2076 6961 2074 6865 2076  ilable via the v
-0000f2f0: 6172 6961 626c 6520 7375 6273 7469 7475  ariable substitu
-0000f300: 7469 6f6e 2060 7772 5f6e 616d 6560 2c20  tion `wr_name`, 
-0000f310: 736f 2074 6869 7320 636f 756c 6420 6265  so this could be
-0000f320: 2073 7570 706c 6965 6420 746f 2074 6865   supplied to the
-0000f330: 2054 6173 6b20 746f 2068 656c 7020 6974   Task to help it
-0000f340: 206c 6f63 6174 6520 6974 7320 646f 776e   locate its down
-0000f350: 6c6f 6164 6564 2066 696c 6573 2e20 466f  loaded files. Fo
-0000f360: 7220 6578 616d 706c 652c 2069 6e20 7468  r example, in th
-0000f370: 6520 6077 6f72 6b52 6571 7569 7265 6d65  e `workRequireme
-0000f380: 6e74 6020 7365 6374 696f 6e20 6f66 2074  nt` section of t
-0000f390: 6865 2060 636f 6e66 6967 2e74 6f6d 6c60  he `config.toml`
-0000f3a0: 2066 696c 652c 2049 2063 6f75 6c64 2073   file, I could s
-0000f3b0: 7065 6369 6679 3a0a 0a60 6060 746f 6d6c  pecify:..```toml
-0000f3c0: 0a65 6e76 6972 6f6e 6d65 6e74 203d 207b  .environment = {
-0000f3d0: 5752 5f44 4952 4543 544f 5259 203d 2022  WR_DIRECTORY = "
-0000f3e0: 7b7b 7772 5f6e 616d 657d 7d22 7d0a 6060  {{wr_name}}"}.``
-0000f3f0: 600a 0a54 6865 2057 6f72 6b20 5265 7175  `..The Work Requ
-0000f400: 6972 656d 656e 7420 6e61 6d65 2077 6f75  irement name wou
-0000f410: 6c64 2074 6865 6e20 6265 2061 7661 696c  ld then be avail
-0000f420: 6162 6c65 2074 6f20 7468 6520 5461 736b  able to the Task
-0000f430: 2069 6e20 7468 6520 656e 7669 726f 6e6d   in the environm
-0000f440: 656e 7420 7661 7269 6162 6c65 2060 2457  ent variable `$W
-0000f450: 525f 4449 5245 4354 4f52 5960 2e0a 0a23  R_DIRECTORY`...#
-0000f460: 2323 2046 696c 6573 2055 706c 6f61 6465  ## Files Uploade
-0000f470: 6420 6672 6f6d 2061 204e 6f64 6520 746f  d from a Node to
-0000f480: 2074 6865 204f 626a 6563 7420 5374 6f72   the Object Stor
-0000f490: 6520 6166 7465 7220 5461 736b 2045 7865  e after Task Exe
-0000f4a0: 6375 7469 6f6e 0a0a 4166 7465 7220 5461  cution..After Ta
-0000f4b0: 736b 2063 6f6d 706c 6574 696f 6e2c 2074  sk completion, t
-0000f4c0: 6865 2041 6765 6e74 2077 696c 6c20 7570  he Agent will up
-0000f4d0: 6c6f 6164 2073 7065 6369 6669 6564 206f  load specified o
-0000f4e0: 7574 7075 7420 6669 6c65 7320 746f 2074  utput files to t
-0000f4f0: 6865 204f 626a 6563 7420 5374 6f72 652e  he Object Store.
-0000f500: 2054 6865 2066 696c 6573 2074 6f20 6265   The files to be
-0000f510: 2075 706c 6f61 6465 6420 6172 6520 7468   uploaded are th
-0000f520: 6f73 6520 6c69 7374 6564 2069 6e20 7468  ose listed in th
-0000f530: 6520 606f 7574 7075 7473 6020 616e 6420  e `outputs` and 
-0000f540: 606f 7574 7075 7473 5265 7175 6972 6564  `outputsRequired
-0000f550: 6020 7072 6f70 6572 7469 6573 2066 6f72  ` properties for
-0000f560: 2074 6865 2054 6173 6b2e 0a0a 496e 2061   the Task...In a
-0000f570: 6464 6974 696f 6e2c 2074 6865 2063 6f6e  ddition, the con
-0000f580: 736f 6c65 206f 7574 7075 7420 6f66 2074  sole output of t
-0000f590: 6865 2054 6173 6b20 6973 2063 6170 7475  he Task is captu
-0000f5a0: 7265 6420 696e 2061 2066 696c 6520 6361  red in a file ca
-0000f5b0: 6c6c 6564 2060 7461 736b 6f75 7470 7574  lled `taskoutput
-0000f5c0: 2e74 7874 6020 696e 2074 6865 2072 6f6f  .txt` in the roo
-0000f5d0: 7420 6f66 2074 6865 2054 6173 6b27 7320  t of the Task's 
-0000f5e0: 776f 726b 696e 6720 6469 7265 6374 6f72  working director
-0000f5f0: 792e 2057 6865 7468 6572 2074 6865 2060  y. Whether the `
-0000f600: 7461 736b 6f75 7470 7574 2e74 7874 6020  taskoutput.txt` 
-0000f610: 6669 6c65 2069 7320 7570 6c6f 6164 6564  file is uploaded
-0000f620: 2074 6f20 7468 6520 4f62 6a65 6374 2053   to the Object S
-0000f630: 746f 7265 2069 7320 6465 7465 726d 696e  tore is determin
-0000f640: 6564 2062 7920 7468 6520 6063 6170 7475  ed by the `captu
-0000f650: 7265 5461 736b 4f75 7470 7574 6020 7072  reTaskOutput` pr
-0000f660: 6f70 6572 7479 2066 6f72 2074 6865 2054  operty for the T
-0000f670: 6173 6b2c 2061 6e64 2074 6869 7320 6973  ask, and this is
-0000f680: 2073 6574 2074 6f20 2774 7275 6527 2062   set to 'true' b
-0000f690: 7920 6465 6661 756c 742e 0a0a 4966 2054  y default...If T
-0000f6a0: 6173 6b20 6f75 7470 7574 7320 6172 6520  ask outputs are 
-0000f6b0: 6372 6561 7465 6420 696e 2073 7562 6469  created in subdi
-0000f6c0: 7265 6374 6f72 6965 7320 6265 6c6f 7720  rectories below 
-0000f6d0: 7468 6520 5461 736b 2773 2077 6f72 6b69  the Task's worki
-0000f6e0: 6e67 2064 6972 6563 746f 7279 2c20 696e  ng directory, in
-0000f6f0: 636c 7564 6520 7468 6520 6469 7265 6374  clude the direct
-0000f700: 6f72 6965 7320 666f 7220 6669 6c65 7320  ories for files 
-0000f710: 696e 2074 6865 2060 6f75 7470 7574 7360  in the `outputs`
-0000f720: 2070 726f 7065 7274 792e 2045 2e67 2e2c   property. E.g.,
-0000f730: 2069 6620 6120 5461 736b 2063 7265 6174   if a Task creat
-0000f740: 6573 2066 696c 6573 2060 7265 7375 6c74  es files `result
-0000f750: 732f 6f70 656e 666f 616d 2e74 6172 2e67  s/openfoam.tar.g
-0000f760: 7a60 2061 6e64 2060 7265 7375 6c74 732f  z` and `results/
-0000f770: 6f70 656e 666f 616d 2e6c 6f67 602c 2074  openfoam.log`, t
-0000f780: 6865 6e20 7370 6563 6966 7920 7468 6573  hen specify thes
-0000f790: 6520 666f 7220 7570 6c6f 6164 2069 6e20  e for upload in 
-0000f7a0: 7468 6520 606f 7574 7075 7473 6020 7072  the `outputs` pr
-0000f7b0: 6f70 6572 7479 2061 7320 666f 6c6c 6f77  operty as follow
-0000f7c0: 733a 0a0a 6022 6f75 7470 7574 7322 3a20  s:..`"outputs": 
-0000f7d0: 5b22 7265 7375 6c74 732f 6f70 656e 666f  ["results/openfo
-0000f7e0: 616d 2e74 6172 2e67 7a22 2c20 2272 6573  am.tar.gz", "res
-0000f7f0: 756c 7473 2f6f 7065 6e66 6f61 6d2e 6c6f  ults/openfoam.lo
-0000f800: 6722 5d60 0a0a 5768 656e 206f 7574 7075  g"]`..When outpu
-0000f810: 7420 6669 6c65 7320 6172 6520 7570 6c6f  t files are uplo
-0000f820: 6164 6564 2074 6f20 7468 6520 4f62 6a65  aded to the Obje
-0000f830: 6374 2053 746f 7265 2c20 7468 6579 2061  ct Store, they a
-0000f840: 7265 2070 6c61 6365 6420 696e 2061 2054  re placed in a T
-0000f850: 6173 6b20 4772 6f75 7020 616e 6420 5461  ask Group and Ta
-0000f860: 736b 2073 7065 6369 6669 6320 6469 7265  sk specific dire
-0000f870: 6374 6f72 792e 2053 6f2c 2069 6620 7468  ctory. So, if th
-0000f880: 6520 4e61 6d65 7370 6163 6520 6973 2060  e Namespace is `
-0000f890: 6465 7665 6c6f 706d 656e 7460 2c20 7468  development`, th
-0000f8a0: 6520 576f 726b 2052 6571 7569 7265 6d65  e Work Requireme
-0000f8b0: 6e74 2069 7320 6074 6573 7472 756e 5f32  nt is `testrun_2
-0000f8c0: 3231 3130 382d 3132 3034 3034 2d37 6432  21108-120404-7d2
-0000f8d0: 602c 2074 6865 2054 6173 6b20 4772 6f75  `, the Task Grou
-0000f8e0: 7020 6973 2060 7461 736b 5f67 726f 7570  p is `task_group
-0000f8f0: 5f31 6020 616e 6420 7468 6520 5461 736b  _1` and the Task
-0000f900: 2069 7320 6074 6173 6b5f 3160 2c20 7468   is `task_1`, th
-0000f910: 656e 2074 6865 2066 696c 6573 2061 626f  en the files abo
-0000f920: 7665 2077 6f75 6c64 2062 6520 7570 6c6f  ve would be uplo
-0000f930: 6164 6564 2074 6f20 7468 6520 4f62 6a65  aded to the Obje
-0000f940: 6374 2053 746f 7265 2061 7320 666f 6c6c  ct Store as foll
-0000f950: 6f77 733a 0a0a 6060 6073 6865 6c6c 0a64  ows:..```shell.d
-0000f960: 6576 656c 6f70 6d65 6e74 3a3a 7465 7374  evelopment::test
-0000f970: 7275 6e5f 3232 3131 3038 2d31 3230 3430  run_221108-12040
-0000f980: 342d 3764 322f 7461 736b 5f67 726f 7570  4-7d2/task_group
-0000f990: 5f31 2f74 6173 6b5f 312f 7265 7375 6c74  _1/task_1/result
-0000f9a0: 732f 6f70 656e 666f 616d 2e74 6172 2e67  s/openfoam.tar.g
-0000f9b0: 7a0a 6465 7665 6c6f 706d 656e 743a 3a74  z.development::t
-0000f9c0: 6573 7472 756e 5f32 3231 3130 382d 3132  estrun_221108-12
-0000f9d0: 3034 3034 2d37 6432 2f74 6173 6b5f 6772  0404-7d2/task_gr
-0000f9e0: 6f75 705f 312f 7461 736b 5f31 2f72 6573  oup_1/task_1/res
-0000f9f0: 756c 7473 2f6f 7065 6e66 6f61 6d2e 6c6f  ults/openfoam.lo
-0000fa00: 670a 6465 7665 6c6f 706d 656e 743a 3a74  g.development::t
-0000fa10: 6573 7472 756e 5f32 3231 3130 382d 3132  estrun_221108-12
-0000fa20: 3034 3034 2d37 6432 2f74 6173 6b5f 6772  0404-7d2/task_gr
-0000fa30: 6f75 705f 312f 7461 736b 5f31 2f74 6173  oup_1/task_1/tas
-0000fa40: 6b6f 7574 7075 742e 7478 740a 6060 600a  koutput.txt.```.
-0000fa50: 0a54 6865 202a 2a60 6f75 7470 7574 7352  .The **`outputsR
-0000fa60: 6571 7569 7265 6460 2a2a 2070 726f 7065  equired`** prope
-0000fa70: 7274 7920 6361 6e20 6265 2075 7365 6420  rty can be used 
-0000fa80: 696e 7374 6561 6420 6f66 2028 6f72 2069  instead of (or i
-0000fa90: 6e20 6164 6469 7469 6f6e 2074 6f29 2074  n addition to) t
-0000faa0: 6865 2060 6f75 7470 7574 7360 2070 726f  he `outputs` pro
-0000fab0: 7065 7274 792c 2069 6620 7468 6520 6f75  perty, if the ou
-0000fac0: 7470 7574 2066 696c 6528 7329 202a 2a6d  tput file(s) **m
-0000fad0: 7573 742a 2a20 6265 2061 7661 696c 6162  ust** be availab
-0000fae0: 6c65 2066 6f72 2075 706c 6f61 6420 746f  le for upload to
-0000faf0: 2074 6865 204f 626a 6563 7420 5374 6f72   the Object Stor
-0000fb00: 6520 6174 2074 6865 2063 6f6e 636c 7573  e at the conclus
-0000fb10: 696f 6e20 6f66 2074 6865 2054 6173 6b20  ion of the Task 
-0000fb20: 6f72 2074 6865 2054 6173 6b20 7769 6c6c  or the Task will
-0000fb30: 2062 6520 6d61 726b 6564 2061 7320 6046   be marked as `F
-0000fb40: 6169 6c65 6460 2c20 652e 672e 3a0a 0a60  ailed`, e.g.:..`
-0000fb50: 226f 7574 7075 7473 5265 7175 6972 6564  "outputsRequired
-0000fb60: 223a 205b 2272 6573 756c 7473 2f70 726f  ": ["results/pro
-0000fb70: 6365 7373 5f6f 7574 7075 742e 7478 7422  cess_output.txt"
-0000fb80: 5d60 0a0a 2323 2320 4669 6c65 7320 446f  ]`..### Files Do
-0000fb90: 776e 6c6f 6164 6564 2066 726f 6d20 7468  wnloaded from th
-0000fba0: 6520 4f62 6a65 6374 2053 746f 7265 2074  e Object Store t
-0000fbb0: 6f20 4c6f 6361 6c20 5374 6f72 6167 650a  o Local Storage.
-0000fbc0: 0a54 6865 2060 7964 2d64 6f77 6e6c 6f61  .The `yd-downloa
-0000fbd0: 6460 2063 6f6d 6d61 6e64 2077 696c 6c20  d` command will 
-0000fbe0: 646f 776e 6c6f 6164 2061 6c6c 206f 626a  download all obj
-0000fbf0: 6563 7473 2066 726f 6d20 7468 6520 4f62  ects from the Ob
-0000fc00: 6a65 6374 2053 746f 7265 2074 6f20 6120  ject Store to a 
-0000fc10: 6c6f 6361 6c20 6469 7265 6374 6f72 792c  local directory,
-0000fc20: 206f 6e20 6120 7065 7220 576f 726b 2052   on a per Work R
-0000fc30: 6571 7569 7265 6d65 6e74 2062 6173 6973  equirement basis
-0000fc40: 2028 696e 636c 7564 696e 6720 616e 7920   (including any 
-0000fc50: 6669 6c65 7320 7468 6174 2068 6176 6520  files that have 
-0000fc60: 6265 656e 2075 706c 6f61 6465 6429 2e20  been uploaded). 
-0000fc70: 4120 6c6f 6361 6c20 6469 7265 6374 6f72  A local director
-0000fc80: 7920 6973 2063 7265 6174 6564 2077 6974  y is created wit
-0000fc90: 6820 7468 6520 7361 6d65 206e 616d 6520  h the same name 
-0000fca0: 6173 2074 6865 204e 616d 6573 7061 6365  as the Namespace
-0000fcb0: 2061 6e64 2063 6f6e 7461 696e 696e 6720   and containing 
-0000fcc0: 7468 6520 576f 726b 2052 6571 7569 7265  the Work Require
-0000fcd0: 6d65 6e74 2064 6972 6563 746f 7269 6573  ment directories
-0000fce0: 2e0a 0a55 7365 2074 6865 2060 2d2d 696e  ...Use the `--in
-0000fcf0: 7465 7261 6374 6976 6560 206f 7074 696f  teractive` optio
-0000fd00: 6e20 7769 7468 2060 7964 2d64 6f77 6e6c  n with `yd-downl
-0000fd10: 6f61 6460 2074 6f20 7365 6c65 6374 2077  oad` to select w
-0000fd20: 6869 6368 2057 6f72 6b20 5265 7175 6972  hich Work Requir
-0000fd30: 656d 656e 7428 7329 2074 6f20 646f 776e  ement(s) to down
-0000fd40: 6c6f 6164 2e0a 0a46 6f72 2074 6865 2065  load...For the e
-0000fd50: 7861 6d70 6c65 2061 626f 7665 2c20 6079  xample above, `y
-0000fd60: 642d 646f 776e 6c6f 6164 6020 776f 756c  d-download` woul
-0000fd70: 6420 6372 6561 7465 2061 2064 6972 6563  d create a direc
-0000fd80: 746f 7279 2063 616c 6c65 6420 6064 6576  tory called `dev
-0000fd90: 656c 6f70 6d65 6e74 6020 696e 2074 6865  elopment` in the
-0000fda0: 2063 7572 7265 6e74 2077 6f72 6b69 6e67   current working
-0000fdb0: 2064 6972 6563 746f 7279 2c20 636f 6e74   directory, cont
-0000fdc0: 6169 6e69 6e67 2073 6f6d 6574 6869 6e67  aining something
-0000fdd0: 206c 696b 653a 0a0a 6060 6073 6865 6c6c   like:..```shell
-0000fde0: 0a64 6576 656c 6f70 6d65 6e74 0ae2 9494  .development....
-0000fdf0: e294 80e2 9480 2074 6573 7472 756e 5f32  ...... testrun_2
-0000fe00: 3231 3130 382d 3132 3034 3034 2d37 6432  21108-120404-7d2
-0000fe10: 0a20 2020 20e2 949c e294 80e2 9480 2062  .    ......... b
-0000fe20: 6173 685f 7363 7269 7074 2e73 680a 2020  ash_script.sh.  
-0000fe30: 2020 e294 9ce2 9480 e294 8020 6669 6c65    ......... file
-0000fe40: 5f31 2e74 7874 0a20 2020 20e2 9494 e294  _1.txt.    .....
-0000fe50: 80e2 9480 2074 6173 6b5f 6772 6f75 705f  .... task_group_
-0000fe60: 310a 2020 2020 2020 2020 e294 94e2 9480  1.        ......
-0000fe70: e294 8020 7461 736b 5f31 0a20 2020 2020  ... task_1.     
-0000fe80: 2020 2020 2020 20e2 949c e294 80e2 9480         .........
-0000fe90: 2072 6573 756c 7473 0a20 2020 2020 2020   results.       
-0000fea0: 2020 2020 20e2 9482 c2a0 c2a0 20e2 949c       ....... ...
-0000feb0: e294 80e2 9480 206f 7065 6e66 6f61 6d2e  ...... openfoam.
-0000fec0: 6c6f 670a 2020 2020 2020 2020 2020 2020  log.            
-0000fed0: e294 82c2 a0c2 a020 e294 94e2 9480 e294  ....... ........
-0000fee0: 8020 6f70 656e 666f 616d 2e74 6172 2e67  . openfoam.tar.g
-0000fef0: 7a0a 2020 2020 2020 2020 2020 2020 e294  z.            ..
-0000ff00: 94e2 9480 e294 8020 7461 736b 6f75 7470  ....... taskoutp
-0000ff10: 7574 2e74 7874 0a60 6060 0a0a 4e6f 7465  ut.txt.```..Note
-0000ff20: 2074 6861 7420 6576 6572 7974 6869 6e67   that everything
-0000ff30: 2077 6974 6869 6e20 7468 6520 606e 616d   within the `nam
-0000ff40: 6573 7061 6365 3a3a 776f 726b 2d72 6571  espace::work-req
-0000ff50: 7569 7265 6d65 6e74 6020 6469 7265 6374  uirement` direct
-0000ff60: 6f72 7920 696e 2074 6865 204f 626a 6563  ory in the Objec
-0000ff70: 7420 5374 6f72 6520 6973 2064 6f77 6e6c  t Store is downl
-0000ff80: 6f61 6465 642c 2069 6e63 6c75 6469 6e67  oaded, including
-0000ff90: 2061 6e79 2066 696c 6573 2074 6861 7420   any files that 
-0000ffa0: 7765 7265 2073 7065 6369 6669 6564 2069  were specified i
-0000ffb0: 6e20 6069 6e70 7574 7360 2061 6e64 2075  n `inputs` and u
-0000ffc0: 706c 6f61 6465 6420 6173 2070 6172 7420  ploaded as part 
-0000ffd0: 6f66 2074 6865 2057 6f72 6b20 5265 7175  of the Work Requ
-0000ffe0: 6972 656d 656e 7420 7375 626d 6973 7369  irement submissi
-0000fff0: 6f6e 2e20 4d75 6c74 6970 6c65 2054 6173  on. Multiple Tas
-00010000: 6b20 4772 6f75 7073 2c20 616e 6420 6d75  k Groups, and mu
-00010010: 6c74 6970 6c65 2054 6173 6b73 2077 696c  ltiple Tasks wil
-00010020: 6c20 616c 6c20 6170 7065 6172 2069 6e20  l all appear in 
-00010030: 7468 6520 6469 7265 6374 6f72 7920 7374  the directory st
-00010040: 7275 6374 7572 652e 0a0a 4966 2074 6865  ructure...If the
-00010050: 2060 6465 7665 6c6f 706d 656e 7460 2064   `development` d
-00010060: 6972 6563 746f 7279 2061 6c72 6561 6479  irectory already
-00010070: 2065 7869 7374 732c 2060 7964 2d64 6f77   exists, `yd-dow
-00010080: 6e6c 6f61 6460 2077 696c 6c20 7472 7920  nload` will try 
-00010090: 6064 6576 656c 6f70 6d65 6e74 2e30 3160  `development.01`
-000100a0: 2c20 6574 632e 2c20 746f 2061 766f 6964  , etc., to avoid
-000100b0: 206f 7665 7277 7269 7469 6e67 2070 7265   overwriting pre
-000100c0: 7669 6f75 7320 646f 776e 6c6f 6164 732e  vious downloads.
-000100d0: 0a0a 2323 2054 6173 6b20 4578 6563 7574  ..## Task Execut
-000100e0: 696f 6e20 436f 6e74 6578 740a 0a54 6869  ion Context..Thi
-000100f0: 7320 7365 6374 696f 6e20 6469 7363 7573  s section discus
-00010100: 7365 7320 7468 6520 636f 6e74 6578 7420  ses the context 
-00010110: 7769 7468 696e 2077 6869 6368 2061 2054  within which a T
-00010120: 6173 6b20 6f70 6572 6174 6573 2077 6865  ask operates whe
-00010130: 6e20 6974 2773 2065 7865 6375 7465 6420  n it's executed 
-00010140: 6279 2061 2057 6f72 6b65 7220 6f6e 2061  by a Worker on a
-00010150: 206e 6f64 652e 2049 7420 6170 706c 6965   node. It applie
-00010160: 7320 7370 6563 6966 6963 616c 6c79 2074  s specifically t
-00010170: 6f20 7468 6520 5965 6c6c 6f77 446f 6720  o the YellowDog 
-00010180: 4167 656e 7420 7275 6e6e 696e 6720 6f6e  Agent running on
-00010190: 2061 204c 696e 7578 206e 6f64 652c 2061   a Linux node, a
-000101a0: 6e64 2063 6f6e 6669 6775 7265 6420 7573  nd configured us
-000101b0: 696e 6720 7468 6520 6465 6661 756c 7420  ing the default 
-000101c0: 7573 6572 6e61 6d65 2c20 6469 7265 6374  username, direct
-000101d0: 6f72 6965 732c 2065 7463 2e20 436f 6e66  ories, etc. Conf
-000101e0: 6967 7572 6174 696f 6e73 2063 616e 2076  igurations can v
-000101f0: 6172 792e 0a0a 2323 2320 5461 736b 2045  ary...### Task E
-00010200: 7865 6375 7469 6f6e 2053 7465 7073 0a0a  xecution Steps..
-00010210: 5768 656e 2061 2054 6173 6b20 6973 2061  When a Task is a
-00010220: 6c6c 6f63 6174 6564 2074 6f20 6120 576f  llocated to a Wo
-00010230: 726b 6572 206f 6e20 6120 6e6f 6465 2062  rker on a node b
-00010240: 7920 7468 6520 5965 6c6c 6f77 446f 6720  y the YellowDog 
-00010250: 5363 6865 6475 6c65 722c 2074 6865 2066  Scheduler, the f
-00010260: 6f6c 6c6f 7769 6e67 2073 7465 7073 2061  ollowing steps a
-00010270: 7265 2066 6f6c 6c6f 7765 643a 0a0a 312e  re followed:..1.
-00010280: 2054 6865 2041 6765 6e74 2072 756e 6e69   The Agent runni
-00010290: 6e67 206f 6e20 7468 6520 6e6f 6465 2064  ng on the node d
-000102a0: 6f77 6e6c 6f61 6473 2074 6865 2054 6173  ownloads the Tas
-000102b0: 6b27 7320 7072 6f70 6572 7469 6573 3a20  k's properties: 
-000102c0: 6974 7320 6074 6173 6b54 7970 6560 2c20  its `taskType`, 
-000102d0: 2060 6172 6775 6d65 6e74 7360 2c20 6065   `arguments`, `e
-000102e0: 6e76 6972 6f6e 6d65 6e74 602c 2060 7461  nvironment`, `ta
-000102f0: 736b 6461 7461 602c 2061 6e64 2028 6672  skdata`, and (fr
-00010300: 6f6d 2074 6865 204f 626a 6563 7420 5374  om the Object St
-00010310: 6f72 6529 2061 6e79 2066 696c 6573 2069  ore) any files i
-00010320: 6e20 7468 6520 6069 6e70 7574 7360 206c  n the `inputs` l
-00010330: 6973 7420 616e 6420 616e 7920 6176 6169  ist and any avai
-00010340: 6c61 626c 6520 6669 6c65 7320 696e 2074  lable files in t
-00010350: 6865 2060 696e 7075 7473 4f70 7469 6f6e  he `inputsOption
-00010360: 616c 6020 6c69 7374 2e0a 322e 2054 6865  al` list..2. The
-00010370: 7365 2066 696c 6573 2061 7265 2070 6c61  se files are pla
-00010380: 6365 6420 696e 2061 6e20 6570 6865 6d65  ced in an epheme
-00010390: 7261 6c20 6469 7265 6374 6f72 7920 6372  ral directory cr
-000103a0: 6561 7465 6420 666f 7220 7468 6973 2054  eated for this T
-000103b0: 6173 6b27 7320 6578 6563 7574 696f 6e2c  ask's execution,
-000103c0: 2061 6e64 2069 6e74 6f20 7768 6963 6820   and into which 
-000103d0: 616e 7920 6f75 7470 7574 2066 696c 6573  any output files
-000103e0: 2061 7265 2061 6c73 6f20 706c 6163 6564   are also placed
-000103f0: 2062 7920 6465 6661 756c 742e 0a32 2e20   by default..2. 
-00010400: 5468 6520 4167 656e 7420 7275 6e73 2074  The Agent runs t
-00010410: 6865 2063 6f6d 6d61 6e64 2073 7065 6369  he command speci
-00010420: 6669 6564 2066 6f72 2074 6865 2060 7461  fied for the `ta
-00010430: 736b 5479 7065 6020 696e 2074 6865 2041  skType` in the A
-00010440: 6765 6e74 2773 2060 6170 706c 6963 6174  gent's `applicat
-00010450: 696f 6e2e 7961 6d6c 6020 636f 6e66 6967  ion.yaml` config
-00010460: 7572 6174 696f 6e20 6669 6c65 2e20 5468  uration file. Th
-00010470: 6973 2064 6f6e 6520 6173 2061 2073 696d  is done as a sim
-00010480: 706c 6520 6065 7865 6360 206f 6620 6120  ple `exec` of a 
-00010490: 7375 6270 726f 6365 7373 2e0a 332e 2057  subprocess..3. W
-000104a0: 6865 6e20 7468 6520 5461 736b 2063 6f6e  hen the Task con
-000104b0: 636c 7564 6573 2c20 7468 6520 4167 656e  cludes, the Agen
-000104c0: 7420 7573 6573 2074 6865 2065 7869 7420  t uses the exit 
-000104d0: 636f 6465 206f 6620 7468 6520 7375 6270  code of the subp
-000104e0: 726f 6365 7373 2074 6f20 7265 706f 7274  rocess to report
-000104f0: 2073 7563 6365 7373 2028 7a65 726f 2920   success (zero) 
-00010500: 6f72 2066 6169 6c75 7265 2028 6e6f 6e2d  or failure (non-
-00010510: 7a65 726f 292e 0a34 2e20 5468 6520 4167  zero)..4. The Ag
-00010520: 656e 7420 7468 656e 2067 6174 6865 7273  ent then gathers
-00010530: 2061 6e79 2066 696c 6573 2069 6e20 7468   any files in th
-00010540: 6520 606f 7574 7075 7473 6020 616e 6420  e `outputs` and 
-00010550: 606f 7574 7075 7473 5265 7175 6972 6564  `outputsRequired
-00010560: 6020 6c69 7374 7320 616e 6420 7570 6c6f  ` lists and uplo
-00010570: 6164 7320 7468 656d 2074 6f20 7468 6520  ads them to the 
-00010580: 4f62 6a65 6374 2053 746f 7265 2e20 4966  Object Store. If
-00010590: 2061 2066 696c 6520 696e 2074 6865 2060   a file in the `
-000105a0: 6f75 7470 7574 7352 6571 7569 7265 6460  outputsRequired`
-000105b0: 206c 6973 7420 6973 206e 6f74 2066 6f75   list is not fou
-000105c0: 6e64 2c20 7468 6520 5461 736b 2077 696c  nd, the Task wil
-000105d0: 6c20 6265 2072 6570 6f72 7465 6420 6173  l be reported as
-000105e0: 2066 6169 6c65 642e 2054 6865 2041 6765   failed. The Age
-000105f0: 6e74 2077 696c 6c20 616c 736f 206f 7074  nt will also opt
-00010600: 696f 6e61 6c6c 7920 7570 6c6f 6164 2074  ionally upload t
-00010610: 6865 2063 6f6e 736f 6c65 206f 7574 7075  he console outpu
-00010620: 7420 2869 6e63 6c75 6469 6e67 2062 6f74  t (including bot
-00010630: 6820 6073 7464 6f75 7460 2061 6e64 2060  h `stdout` and `
-00010640: 7374 6465 7272 6029 206f 6620 7468 6520  stderr`) of the 
-00010650: 5461 736b 2c20 636f 6e74 6169 6e65 6420  Task, contained 
-00010660: 696e 2074 6865 2060 7461 736b 6f75 7470  in the `taskoutp
-00010670: 7574 2e74 7874 6020 6669 6c65 2e0a 352e  ut.txt` file..5.
-00010680: 2054 6865 2065 7068 656d 6572 616c 2054   The ephemeral T
-00010690: 6173 6b20 6469 7265 6374 6f72 7920 6973  ask directory is
-000106a0: 2074 6865 6e20 6465 6c65 7465 642e 0a0a   then deleted...
-000106b0: 4e6f 7465 2074 6861 7420 6966 2061 2054  Note that if a T
-000106c0: 6173 6b20 6973 2061 626f 7274 6564 2064  ask is aborted d
-000106d0: 7572 696e 6720 6578 6563 7574 696f 6e2c  uring execution,
-000106e0: 2074 6865 2054 6173 6b27 7320 7375 6270   the Task's subp
-000106f0: 726f 6365 7373 2069 7320 7365 6e74 2061  rocess is sent a
-00010700: 2060 5349 4749 4e54 602c 2061 6c6c 6f77   `SIGINT`, allow
-00010710: 696e 6720 7468 6520 5461 736b 2061 6e20  ing the Task an 
-00010720: 6f70 706f 7274 756e 6974 7920 746f 2074  opportunity to t
-00010730: 6572 6d69 6e61 7465 2061 6e79 2063 6869  erminate any chi
-00010740: 6c64 2070 726f 6365 7373 6573 206f 7220  ld processes or 
-00010750: 6f74 6865 7220 7265 736f 7572 6365 7320  other resources 
-00010760: 2865 2e67 2e2c 2063 6f6e 7461 696e 6572  (e.g., container
-00010770: 7329 2074 6861 7420 6d61 7920 6861 7665  s) that may have
-00010780: 2062 6565 6e20 7374 6172 7465 6420 6173   been started as
-00010790: 2070 6172 7420 6f66 2054 6173 6b20 6578   part of Task ex
-000107a0: 6563 7574 696f 6e2e 0a0a 4f6e 6365 2074  ecution...Once t
-000107b0: 6865 2073 7465 7073 2061 626f 7665 2068  he steps above h
-000107c0: 6176 6520 6265 656e 2063 6f6d 706c 6574  ave been complet
-000107d0: 6564 2c20 7468 6520 576f 726b 6572 2069  ed, the Worker i
-000107e0: 7320 7265 6164 7920 746f 2061 6363 6570  s ready to accep
-000107f0: 7420 6974 7320 6e65 7874 2054 6173 6b20  t its next Task 
-00010800: 6672 6f6d 2074 6865 2059 656c 6c6f 7744  from the YellowD
-00010810: 6f67 2073 6368 6564 756c 6572 2e0a 0a4e  og scheduler...N
-00010820: 6f74 6520 7468 6174 2069 6620 7468 6520  ote that if the 
-00010830: 4167 656e 7420 6f6e 2061 206e 6f64 6520  Agent on a node 
-00010840: 6861 7320 6d75 6c74 6970 6c65 2057 6f72  has multiple Wor
-00010850: 6b65 7273 2c20 7468 656e 2054 6173 6b73  kers, then Tasks
-00010860: 2061 7265 2065 7865 6375 7465 6420 696e   are executed in
-00010870: 2070 6172 616c 6c65 6c20 6f6e 2074 6865   parallel on the
-00010880: 206e 6f64 6520 616e 6420 6361 6e20 7374   node and can st
-00010890: 6172 7420 616e 6420 7374 6f70 2069 6e64  art and stop ind
-000108a0: 6570 656e 6465 6e74 6c79 2e0a 0a23 2323  ependently...###
-000108b0: 2054 6865 2055 7365 7220 616e 6420 4772   The User and Gr
-000108c0: 6f75 7020 7573 6564 2066 6f72 2054 6173  oup used for Tas
-000108d0: 6b73 0a0a 4279 2064 6566 6175 6c74 2c20  ks..By default, 
-000108e0: 7468 6520 4167 656e 7420 7275 6e73 2061  the Agent runs a
-000108f0: 7320 7573 6572 2061 6e64 2067 726f 7570  s user and group
-00010900: 2060 7964 2d61 6765 6e74 602c 2061 6e64   `yd-agent`, and
-00010910: 2068 656e 6365 2054 6173 6b73 2061 6c73   hence Tasks als
-00010920: 6f20 6578 6563 7574 6520 756e 6465 7220  o execute under 
-00010930: 7468 6973 2075 7365 722e 0a0a 6079 642d  this user...`yd-
-00010940: 6167 656e 7460 2064 6f65 7320 6e6f 7420  agent` does not 
-00010950: 6861 7665 2060 7375 646f 6020 7072 6976  have `sudo` priv
-00010960: 696c 6567 6573 2061 7320 7374 616e 6461  ileges as standa
-00010970: 7264 2c20 6275 7420 7468 6973 2063 616e  rd, but this can
-00010980: 2062 6520 6164 6465 6420 6966 2072 6571   be added if req
-00010990: 7569 7265 6420 6174 2069 6e73 7461 6e63  uired at instanc
-000109a0: 6520 626f 6f74 2074 696d 6520 7669 6120  e boot time via 
-000109b0: 7468 6520 6075 7365 7244 6174 6160 2070  the `userData` p
-000109c0: 726f 7065 7274 7920 6f66 2061 2070 726f  roperty of a pro
-000109d0: 7669 7369 6f6e 696e 6720 7265 7175 6573  visioning reques
-000109e0: 742e 2045 2e67 2e20 2866 6f72 2055 6275  t. E.g. (for Ubu
-000109f0: 6e74 7529 3a0a 0a60 6060 7368 656c 6c0a  ntu):..```shell.
-00010a00: 7573 6572 6d6f 6420 2d61 4720 7768 6565  usermod -aG whee
-00010a10: 6c20 7964 2d61 6765 6e74 0a65 6368 6f20  l yd-agent.echo 
-00010a20: 2d65 2022 7964 2d61 6765 6e74 5c74 414c  -e "yd-agent\tAL
-00010a30: 4c3d 2841 4c4c 295c 744e 4f50 4153 5357  L=(ALL)\tNOPASSW
-00010a40: 443a 2041 4c4c 2220 3e20 2f65 7463 2f73  D: ALL" > /etc/s
-00010a50: 7564 6f65 7273 2e64 2f30 3230 2d79 642d  udoers.d/020-yd-
-00010a60: 6167 656e 740a 6060 600a 0a23 2323 2048  agent.```..### H
-00010a70: 6f6d 6520 4469 7265 6374 6f72 7920 666f  ome Directory fo
-00010a80: 7220 6079 642d 6167 656e 7460 0a0a 4279  r `yd-agent`..By
-00010a90: 2064 6566 6175 6c74 2c20 7468 6520 686f   default, the ho
-00010aa0: 6d65 2064 6972 6563 746f 7279 206f 6620  me directory of 
-00010ab0: 7468 6520 6079 642d 6167 656e 7460 2075  the `yd-agent` u
-00010ac0: 7365 7220 6973 2060 2f6f 7074 2f79 656c  ser is `/opt/yel
-00010ad0: 6c6f 7764 6f67 2f61 6765 6e74 602e 2054  lowdog/agent`. T
-00010ae0: 6869 7320 6469 7265 6374 6f72 7920 7479  his directory ty
-00010af0: 7069 6361 6c6c 7920 636f 6e74 6169 6e73  pically contains
-00010b00: 2074 6865 2060 6170 706c 6963 6174 696f   the `applicatio
-00010b10: 6e2e 7961 6d6c 6020 6669 6c65 2075 7365  n.yaml` file use
-00010b20: 6420 746f 2063 6f6e 6669 6775 7265 2074  d to configure t
-00010b30: 6865 2041 6765 6e74 2c20 6173 2077 656c  he Agent, as wel
-00010b40: 6c20 6173 2061 6e79 2073 6372 6970 7473  l as any scripts
-00010b50: 2074 6861 7420 6172 6520 7573 6564 2074   that are used t
-00010b60: 6f20 6578 6563 7574 6520 7468 6520 5461  o execute the Ta
-00010b70: 736b 2054 7970 6573 2074 6861 7420 7468  sk Types that th
-00010b80: 6520 6e6f 6465 2073 7570 706f 7274 732e  e node supports.
-00010b90: 0a0a 4966 206f 6e65 2077 616e 7473 2074  ..If one wants t
-00010ba0: 6f20 5353 4820 746f 2061 6e20 696e 7374  o SSH to an inst
-00010bb0: 616e 6365 2061 7320 7573 6572 2060 7964  ance as user `yd
-00010bc0: 2d61 6765 6e74 602c 2070 6572 6861 7073  -agent`, perhaps
-00010bd0: 2066 6f72 2064 6562 7567 6769 6e67 2070   for debugging p
-00010be0: 7572 706f 7365 732c 2053 5348 206b 6579  urposes, SSH key
-00010bf0: 7320 6361 6e20 6265 2069 6e73 6572 7465  s can be inserte
-00010c00: 6420 7669 6120 696e 7374 616e 6365 2060  d via instance `
-00010c10: 7573 6572 4461 7461 602c 2065 2e67 2e3a  userData`, e.g.:
-00010c20: 0a0a 6060 6073 6865 6c6c 0a59 4441 5f48  ..```shell.YDA_H
-00010c30: 4f4d 453d 2f6f 7074 2f79 656c 6c6f 7764  OME=/opt/yellowd
-00010c40: 6f67 2f61 6765 6e74 0a6d 6b64 6972 202d  og/agent.mkdir -
-00010c50: 7020 2459 4441 5f48 4f4d 452f 2e73 7368  p $YDA_HOME/.ssh
-00010c60: 0a63 686d 6f64 206f 672d 7277 7820 2459  .chmod og-rwx $Y
-00010c70: 4441 5f48 4f4d 452f 2e73 7368 0a63 6174  DA_HOME/.ssh.cat
-00010c80: 203e 3e20 2459 4441 5f48 4f4d 452f 2e73   >> $YDA_HOME/.s
-00010c90: 7368 2f61 7574 686f 7269 7a65 645f 6b65  sh/authorized_ke
-00010ca0: 7973 203c 3c20 454f 460a 3c3c 496e 7365  ys << EOF.<<Inse
-00010cb0: 7274 5f50 7562 6c69 635f 6b65 795f 4865  rt_Public_key_He
-00010cc0: 7265 3e3e 0a45 4f46 0a63 686d 6f64 206f  re>>.EOF.chmod o
-00010cd0: 672d 7277 2024 5944 415f 484f 4d45 2f2e  g-rw $YDA_HOME/.
-00010ce0: 7373 682f 6175 7468 6f72 697a 6564 5f6b  ssh/authorized_k
-00010cf0: 6579 730a 6368 6f77 6e20 2d52 2079 642d  eys.chown -R yd-
-00010d00: 6167 656e 743a 7964 2d61 6765 6e74 2024  agent:yd-agent $
-00010d10: 5944 415f 484f 4d45 2f2e 7373 680a 6060  YDA_HOME/.ssh.``
-00010d20: 600a 0a23 2323 2054 6173 6b20 4578 6563  `..### Task Exec
-00010d30: 7574 696f 6e20 4469 7265 6374 6f72 790a  ution Directory.
-00010d40: 0a45 7068 656d 6572 616c 2054 6173 6b20  .Ephemeral Task 
-00010d50: 6469 7265 6374 6f72 6965 7320 6172 6520  directories are 
-00010d60: 6372 6561 7465 6420 756e 6465 7220 602f  created under `/
-00010d70: 7661 722f 6f70 742f 7965 6c6c 6f77 646f  var/opt/yellowdo
-00010d80: 672f 6167 656e 742f 6461 7461 2f77 6f72  g/agent/data/wor
-00010d90: 6b65 7273 602e 2054 6869 7320 6469 7265  kers`. This dire
-00010da0: 6374 6f72 7920 636f 6e74 6169 6e73 206f  ctory contains o
-00010db0: 6e65 206f 7220 6d6f 7265 206e 756d 6265  ne or more numbe
-00010dc0: 7265 6420 7375 6264 6972 6563 746f 7269  red subdirectori
-00010dd0: 6573 2077 6865 7265 2065 6163 6820 6e75  es where each nu
-00010de0: 6d62 6572 6564 2064 6972 6563 746f 7279  mbered directory
-00010df0: 2063 6f72 7265 7370 6f6e 6473 2074 6f20   corresponds to 
-00010e00: 6120 576f 726b 6572 206f 6e20 7468 6520  a Worker on the 
-00010e10: 6e6f 6465 2e0a 0a57 6865 6e20 6120 5461  node...When a Ta
-00010e20: 736b 2069 7320 616c 6c6f 6361 7465 6420  sk is allocated 
-00010e30: 746f 2061 206e 6f64 652c 2061 6e20 6570  to a node, an ep
-00010e40: 6865 6d65 7261 6c20 6469 7265 6374 6f72  hemeral director
-00010e50: 7920 6973 2063 7265 6174 6564 2075 6e64  y is created und
-00010e60: 6572 2074 6865 2061 7070 6c69 6361 626c  er the applicabl
-00010e70: 6520 576f 726b 6572 2064 6972 6563 746f  e Worker directo
-00010e80: 7279 2c20 7769 7468 2061 206e 616d 6520  ry, with a name 
-00010e90: 636f 7272 6573 706f 6e64 696e 6720 7468  corresponding th
-00010ea0: 6520 5965 6c6c 6f77 446f 6720 4944 2066  e YellowDog ID f
-00010eb0: 6f72 2074 6865 2054 6173 6b2e 2046 6f72  or the Task. For
-00010ec0: 2065 7861 6d70 6c65 2c20 7468 6973 2069   example, this i
-00010ed0: 7320 616e 2065 7068 656d 6572 616c 2064  s an ephemeral d
-00010ee0: 6972 6563 746f 7279 2062 6569 6e67 2075  irectory being u
-00010ef0: 7365 6420 6279 2057 6f72 6b65 7220 6e75  sed by Worker nu
-00010f00: 6d62 6572 2060 3160 3a0a 0a60 2f76 6172  mber `1`:..`/var
-00010f10: 2f6f 7074 2f79 656c 6c6f 7764 6f67 2f61  /opt/yellowdog/a
-00010f20: 6765 6e74 2f64 6174 612f 776f 726b 6572  gent/data/worker
-00010f30: 732f 312f 7964 6964 5f74 6173 6b5f 3535  s/1/ydid_task_55
-00010f40: 3945 4245 5f37 3439 3439 3333 362d 6163  9EBE_74949336-ac
-00010f50: 3262 2d34 3831 312d 6137 6435 2d66 3365  2b-4811-a7d5-f3e
-00010f60: 6364 3937 3339 3930 385f 315f 3160 0a0a  cd9739908_1_1`..
-00010f70: 5468 6973 2069 7320 7468 6520 6469 7265  This is the dire
-00010f80: 6374 6f72 7920 696e 746f 2077 6869 6368  ctory into which
-00010f90: 2064 6f77 6e6c 6f61 6465 6420 6f62 6a65   downloaded obje
-00010fa0: 6374 7320 6172 6520 706c 6163 6564 2c20  cts are placed, 
-00010fb0: 616e 6420 696e 2077 6869 6368 206f 7574  and in which out
-00010fc0: 7075 7420 6669 6c65 7320 6172 6520 6372  put files are cr
-00010fd0: 6561 7465 6420 6279 2064 6566 6175 6c74  eated by default
-00010fe0: 2e20 5468 6520 636f 6e73 6f6c 6520 6f75  . The console ou
-00010ff0: 7470 7574 2060 7461 736b 6f75 7470 7574  tput `taskoutput
-00011000: 2e74 7874 6020 6669 6c65 2077 696c 6c20  .txt` file will 
-00011010: 616c 736f 2062 6520 6372 6561 7465 6420  also be created 
-00011020: 696e 2074 6869 7320 6469 7265 6374 6f72  in this director
-00011030: 792e 0a0a 5365 6520 7468 6520 5b46 696c  y...See the [Fil
-00011040: 6573 2044 6f77 6e6c 6f61 6465 6420 746f  es Downloaded to
-00011050: 2061 204e 6f64 655d 2823 6669 6c65 732d   a Node](#files-
-00011060: 646f 776e 6c6f 6164 6564 2d74 6f2d 612d  downloaded-to-a-
-00011070: 6e6f 6465 2d66 6f72 2d75 7365 2d69 6e2d  node-for-use-in-
-00011080: 7461 736b 2d65 7865 6375 7469 6f6e 2920  task-execution) 
-00011090: 7365 6374 696f 6e20 6162 6f76 6520 666f  section above fo
-000110a0: 7220 6d6f 7265 2064 6574 6169 6c73 206f  r more details o
-000110b0: 6e20 686f 7720 6669 6c65 7320 696e 2074  n how files in t
-000110c0: 6869 7320 6469 7265 6374 6f72 7920 6172  his directory ar
-000110d0: 6520 6861 6e64 6c65 642e 0a0a 4174 2074  e handled...At t
-000110e0: 6865 2063 6f6e 636c 7573 696f 6e20 6f66  he conclusion of
-000110f0: 2074 6865 2054 6173 6b2c 2061 6674 6572   the Task, after
-00011100: 2061 6e79 2066 696c 6573 2072 6571 7565   any files reque
-00011110: 7374 6564 2066 6f72 2075 706c 6f61 6420  sted for upload 
-00011120: 6861 7665 2062 6565 6e20 7570 6c6f 6164  have been upload
-00011130: 6564 2074 6f20 7468 6520 4f62 6a65 6374  ed to the Object
-00011140: 2053 746f 7265 2028 7365 6520 7468 6520   Store (see the 
-00011150: 5b46 696c 6573 2055 706c 6f61 6465 6420  [Files Uploaded 
-00011160: 6672 6f6d 2061 204e 6f64 655d 2823 6669  from a Node](#fi
-00011170: 6c65 732d 7570 6c6f 6164 6564 2d66 726f  les-uploaded-fro
-00011180: 6d2d 612d 6e6f 6465 2d74 6f2d 7468 652d  m-a-node-to-the-
-00011190: 6f62 6a65 6374 2d73 746f 7265 2d61 6674  object-store-aft
-000111a0: 6572 2d74 6173 6b2d 6578 6563 7574 696f  er-task-executio
-000111b0: 6e29 2073 6563 7469 6f6e 2066 6f72 206d  n) section for m
-000111c0: 6f72 6520 696e 666f 726d 6174 696f 6e29  ore information)
-000111d0: 2c20 7468 6520 6079 6469 645f 7461 736b  , the `ydid_task
-000111e0: 5f35 3539 4542 455f 3734 3934 3933 3336  _559EBE_74949336
-000111f0: 2d61 6332 622d 3438 3131 2d61 3764 352d  -ac2b-4811-a7d5-
-00011200: 6633 6563 6439 3733 3939 3038 5f31 5f31  f3ecd9739908_1_1
-00011210: 6020 7769 6c6c 2062 6520 7265 6d6f 7665  ` will be remove
-00011220: 642e 0a0a 2323 2053 7065 6369 6679 696e  d...## Specifyin
-00011230: 6720 576f 726b 2052 6571 7569 7265 6d65  g Work Requireme
-00011240: 6e74 7320 7573 696e 6720 4353 5620 4461  nts using CSV Da
-00011250: 7461 0a0a 4353 5620 6461 7461 2066 696c  ta..CSV data fil
-00011260: 6573 2063 616e 2062 6520 7573 6564 2074  es can be used t
-00011270: 6f20 6472 6976 6520 7468 6520 6765 6e65  o drive the gene
-00011280: 7261 7469 6f6e 206f 6620 6c69 7374 7320  ration of lists 
-00011290: 6f66 2054 6173 6b73 2c20 6173 2066 6f6c  of Tasks, as fol
-000112a0: 6c6f 7773 3a0a 0a2d 2041 202a 2a70 726f  lows:..- A **pro
-000112b0: 746f 7479 7065 2a2a 2054 6173 6b20 7370  totype** Task sp
-000112c0: 6563 6966 6963 6174 696f 6e20 6973 2063  ecification is c
-000112d0: 7265 6174 6564 2077 6974 6869 6e20 6120  reated within a 
-000112e0: 4a53 4f4e 2057 6f72 6b20 5265 7175 6972  JSON Work Requir
-000112f0: 656d 656e 7420 7370 6563 6966 6963 6174  ement specificat
-00011300: 696f 6e20 6f72 2069 6e20 7468 6520 6077  ion or in the `w
-00011310: 6f72 6b52 6571 7569 7265 6d65 6e74 6020  orkRequirement` 
-00011320: 7365 6374 696f 6e20 6f66 2074 6865 2054  section of the T
-00011330: 4f4d 4c20 636f 6e66 6967 7572 6174 696f  OML configuratio
-00011340: 6e20 6669 6c65 0a2d 2054 6865 2070 726f  n file.- The pro
-00011350: 746f 7479 7065 2074 6173 6b20 696e 636c  totype task incl
-00011360: 7564 6573 206f 6e65 206f 7220 6d6f 7265  udes one or more
-00011370: 2076 6172 6961 626c 6520 7375 6273 7469   variable substi
-00011380: 7475 7469 6f6e 730a 2d20 4120 4353 5620  tutions.- A CSV 
-00011390: 6669 6c65 2069 7320 6372 6561 7465 642c  file is created,
-000113a0: 2077 6974 6820 7468 6520 2a2a 6865 6164   with the **head
-000113b0: 6572 732a 2a20 2866 6972 7374 2072 6f77  ers** (first row
-000113c0: 2920 6d61 7463 6869 6e67 2074 6865 206e  ) matching the n
-000113d0: 616d 6573 206f 6620 7468 6520 7661 7269  ames of the vari
-000113e0: 6162 6c65 2073 7562 7374 6974 7574 696f  able substitutio
-000113f0: 6e73 2069 6e20 7468 6520 5461 736b 2070  ns in the Task p
-00011400: 726f 746f 7479 7065 0a2d 2045 6163 6820  rototype.- Each 
-00011410: 7375 6273 6571 7565 6e74 2072 6f77 206f  subsequent row o
-00011420: 6620 7468 6520 4353 5620 6669 6c65 2072  f the CSV file r
-00011430: 6570 7265 7365 6e74 7320 6120 6e65 7720  epresents a new 
-00011440: 5461 736b 2062 7569 6c74 2075 7369 6e67  Task built using
-00011450: 2074 6865 2070 726f 746f 7479 7065 2c20   the prototype, 
-00011460: 7769 7468 2074 6865 2076 6172 6961 626c  with the variabl
-00011470: 6573 2073 7562 7374 6974 7574 6564 2062  es substituted b
-00011480: 7920 7468 6520 7661 6c75 6573 2069 6e20  y the values in 
-00011490: 7468 6520 726f 770a 2d20 4120 5461 736b  the row.- A Task
-000114a0: 2077 696c 6c20 6265 2063 7265 6174 6564   will be created
-000114b0: 2066 6f72 2065 6163 6820 6461 7461 2072   for each data r
-000114c0: 6f77 0a0a 2323 2320 576f 726b 2052 6571  ow..### Work Req
-000114d0: 7569 7265 6d65 6e74 2043 5356 2044 6174  uirement CSV Dat
-000114e0: 6120 4578 616d 706c 650a 0a41 7320 616e  a Example..As an
-000114f0: 2065 7861 6d70 6c65 2c20 636f 6e73 6964   example, consid
-00011500: 6572 2074 6865 2066 6f6c 6c6f 7769 6e67  er the following
-00011510: 204a 534f 4e20 576f 726b 2052 6571 7569   JSON Work Requi
-00011520: 7265 6d65 6e74 2060 7772 2e6a 736f 6e60  rement `wr.json`
-00011530: 3a0a 0a60 6060 6a73 6f6e 0a7b 0a20 2022  :..```json.{.  "
-00011540: 7461 736b 4772 6f75 7073 223a 205b 0a20  taskGroups": [. 
-00011550: 2020 207b 0a20 2020 2020 2022 7461 736b     {.      "task
-00011560: 7322 3a20 5b0a 2020 2020 2020 2020 7b0a  s": [.        {.
-00011570: 2020 2020 2020 2020 2020 2261 7267 756d            "argum
-00011580: 656e 7473 223a 205b 227b 7b61 7267 5f31  ents": ["{{arg_1
-00011590: 7d7d 222c 2022 7b7b 6172 675f 327d 7d22  }}", "{{arg_2}}"
-000115a0: 2c20 227b 7b61 7267 5f33 7d7d 225d 2c0a  , "{{arg_3}}"],.
-000115b0: 2020 2020 2020 2020 2020 2265 6e76 6972            "envir
-000115c0: 6f6e 6d65 6e74 223a 207b 2245 4e56 5f56  onment": {"ENV_V
-000115d0: 4152 5f31 223a 2022 7b7b 656e 765f 317d  AR_1": "{{env_1}
-000115e0: 7d22 7d0a 2020 2020 2020 2020 7d0a 2020  }"}.        }.  
-000115f0: 2020 2020 5d0a 2020 2020 7d0a 2020 5d0a      ].    }.  ].
-00011600: 7d0a 6060 600a 0a4e 6f74 6520 7468 6174  }.```..Note that
-00011610: 2074 6865 2054 6173 6b20 4772 6f75 7020   the Task Group 
-00011620: 6d75 7374 2063 6f6e 7461 696e 206f 6e6c  must contain onl
-00011630: 7920 6120 7369 6e67 6c65 2054 6173 6b2c  y a single Task,
-00011640: 2061 6374 696e 6720 6173 2074 6865 2070   acting as the p
-00011650: 726f 746f 7479 7065 2e0a 0a4e 6f77 2063  rototype...Now c
-00011660: 6f6e 7369 6465 7220 6120 4353 5620 6669  onsider a CSV fi
-00011670: 6c65 2060 7772 5f64 6174 612e 6373 7660  le `wr_data.csv`
-00011680: 2077 6974 6820 7468 6520 666f 6c6c 6f77   with the follow
-00011690: 696e 6720 636f 6e74 656e 7473 3a0a 0a60  ing contents:..`
-000116a0: 6060 7465 7874 0a61 7267 5f31 2c20 6172  ``text.arg_1, ar
-000116b0: 675f 322c 2061 7267 5f33 2c20 656e 765f  g_2, arg_3, env_
-000116c0: 310a 412c 2020 2020 2042 2c20 2020 2020  1.A,     B,     
-000116d0: 432c 2020 2020 2045 2d31 0a44 2c20 2020  C,     E-1.D,   
-000116e0: 2020 452c 2020 2020 2046 2c20 2020 2020    E,     F,     
-000116f0: 452d 320a 472c 2020 2020 2048 2c20 2020  E-2.G,     H,   
-00011700: 2020 492c 2020 2020 2045 2d33 0a60 6060    I,     E-3.```
-00011710: 0a0a 4e6f 7465 2074 6861 7420 7468 6520  ..Note that the 
-00011720: 286f 7074 696f 6e61 6c29 206c 6561 6469  (optional) leadi
-00011730: 6e67 2073 7061 6365 7320 6166 7465 7220  ng spaces after 
-00011740: 6561 6368 2063 6f6d 6d61 2061 7265 2069  each comma are i
-00011750: 676e 6f72 6564 2c20 6275 7420 7472 6169  gnored, but trai
-00011760: 6c69 6e67 2073 7061 6365 7320 6172 6520  ling spaces are 
-00011770: 6e6f 7420 616e 6420 7769 6c6c 2066 6f72  not and will for
-00011780: 6d20 7061 7274 206f 6620 7468 6520 696d  m part of the im
-00011790: 706f 7274 6564 2064 6174 612e 0a0a 4966  ported data...If
-000117a0: 2074 6865 7365 2066 696c 6573 2061 7265   these files are
-000117b0: 2070 726f 6365 7373 6564 2075 7369 6e67   processed using
-000117c0: 2060 7964 2d73 7562 6d69 7420 2d72 2077   `yd-submit -r w
-000117d0: 722e 6a73 6f6e 202d 5620 7772 5f64 6174  r.json -V wr_dat
-000117e0: 612e 6373 7660 2c20 7468 6520 666f 6c6c  a.csv`, the foll
-000117f0: 6f77 696e 6720 6578 7061 6e64 6564 206c  owing expanded l
-00011800: 6973 7420 6f66 2074 6872 6565 2054 6173  ist of three Tas
-00011810: 6b73 2077 696c 6c20 6265 2063 7265 6174  ks will be creat
-00011820: 6564 2070 7269 6f72 2074 6f20 6675 7274  ed prior to furt
-00011830: 6865 7220 7072 6f63 6573 7369 6e67 2062  her processing b
-00011840: 7920 7468 6520 6079 642d 7375 626d 6974  y the `yd-submit
-00011850: 6020 7363 7269 7074 3a0a 0a60 6060 6a73  ` script:..```js
-00011860: 6f6e 0a7b 0a20 2022 7461 736b 4772 6f75  on.{.  "taskGrou
-00011870: 7073 223a 205b 0a20 2020 207b 0a20 2020  ps": [.    {.   
-00011880: 2020 2022 7461 736b 7322 3a20 5b0a 2020     "tasks": [.  
-00011890: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-000118a0: 2020 2261 7267 756d 656e 7473 223a 205b    "arguments": [
-000118b0: 2241 222c 2022 4222 2c20 2243 225d 2c0a  "A", "B", "C"],.
-000118c0: 2020 2020 2020 2020 2020 2265 6e76 6972            "envir
-000118d0: 6f6e 6d65 6e74 223a 207b 2245 4e56 5f56  onment": {"ENV_V
-000118e0: 4152 5f31 223a 2022 452d 3122 7d0a 2020  AR_1": "E-1"}.  
-000118f0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00011900: 207b 0a20 2020 2020 2020 2020 2022 6172   {.          "ar
-00011910: 6775 6d65 6e74 7322 3a20 5b22 4422 2c20  guments": ["D", 
-00011920: 2245 222c 2022 4622 5d2c 0a20 2020 2020  "E", "F"],.     
-00011930: 2020 2020 2022 656e 7669 726f 6e6d 656e       "environmen
-00011940: 7422 3a20 7b22 454e 565f 5641 525f 3122  t": {"ENV_VAR_1"
-00011950: 3a20 2245 2d32 227d 0a20 2020 2020 2020  : "E-2"}.       
-00011960: 207d 2c0a 2020 2020 2020 2020 7b0a 2020   },.        {.  
-00011970: 2020 2020 2020 2020 2261 7267 756d 656e          "argumen
-00011980: 7473 223a 205b 2247 222c 2022 4822 2c20  ts": ["G", "H", 
-00011990: 2249 225d 2c0a 2020 2020 2020 2020 2020  "I"],.          
-000119a0: 2265 6e76 6972 6f6e 6d65 6e74 223a 207b  "environment": {
-000119b0: 2245 4e56 5f56 4152 5f31 223a 2022 452d  "ENV_VAR_1": "E-
-000119c0: 3322 7d0a 2020 2020 2020 2020 7d0a 2020  3"}.        }.  
-000119d0: 2020 2020 5d0a 2020 2020 7d0a 2020 5d0a      ].    }.  ].
-000119e0: 7d0a 6060 600a 0a23 2323 2043 5356 2056  }.```..### CSV V
-000119f0: 6172 6961 626c 6520 5375 6273 7469 7475  ariable Substitu
-00011a00: 7469 6f6e 730a 0a57 6865 6e20 7468 6520  tions..When the 
-00011a10: 4353 5620 6669 6c65 2064 6174 6120 6973  CSV file data is
-00011a20: 2070 726f 6365 7373 6564 2c20 7468 6520   processed, the 
-00011a30: 6f6e 6c79 2073 7562 7374 6974 7574 696f  only substitutio
-00011a40: 6e73 206d 6164 6520 6172 6520 7468 6f73  ns made are thos
-00011a50: 6520 7768 6963 6820 6d61 7463 6820 7468  e which match th
-00011a60: 6520 7661 7269 6162 6c65 2073 7562 7374  e variable subst
-00011a70: 6974 7574 696f 6e73 2069 6e20 7468 6520  itutions in the 
-00011a80: 7072 6f74 6f74 7970 6520 5461 736b 2e20  prototype Task. 
-00011a90: 5468 6520 4353 5620 6669 6c65 2069 7320  The CSV file is 
-00011aa0: 7468 6520 2a2a 6f6e 6c79 2a2a 2073 6f75  the **only** sou
-00011ab0: 7263 6520 6f66 2073 7562 7374 6974 7574  rce of substitut
-00011ac0: 696f 6e73 2075 7365 6420 666f 7220 7468  ions used for th
-00011ad0: 6973 2070 726f 6365 7373 696e 6720 7068  is processing ph
-00011ae0: 6173 653b 2061 6c6c 206f 7468 6572 2076  ase; all other v
-00011af0: 6172 6961 626c 6520 7375 6273 7469 7475  ariable substitu
-00011b00: 7469 6f6e 7320 2873 7570 706c 6965 6420  tions (supplied 
-00011b10: 6f6e 2074 6865 2063 6f6d 6d61 6e64 206c  on the command l
-00011b20: 696e 652c 2069 6e20 7468 6520 544f 4d4c  ine, in the TOML
-00011b30: 2063 6f6e 6669 6775 7261 7469 6f6e 2066   configuration f
-00011b40: 696c 652c 206f 7220 6672 6f6d 2065 6e76  ile, or from env
-00011b50: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
-00011b60: 6573 2920 6172 6520 6967 6e6f 7265 6420  es) are ignored 
-00011b70: 2d2d 2069 2e65 2e2c 2074 6865 7920 646f  -- i.e., they do
-00011b80: 206e 6f74 206f 7665 7272 6964 6520 7468   not override th
-00011b90: 6520 636f 6e74 656e 7473 206f 6620 7468  e contents of th
-00011ba0: 6520 4353 5620 6669 6c65 2e0a 0a41 6c6c  e CSV file...All
-00011bb0: 2076 6172 6961 626c 6520 7375 6273 7469   variable substi
-00011bc0: 7475 7469 6f6e 7320 756e 7265 6c61 7465  tutions unrelate
-00011bd0: 6420 746f 2074 6865 2043 5356 2066 696c  d to the CSV fil
-00011be0: 6520 6461 7461 2061 7265 206c 6566 7420  e data are left 
-00011bf0: 756e 6368 616e 6765 642c 2066 6f72 2073  unchanged, for s
-00011c00: 7562 7365 7175 656e 7420 7072 6f63 6573  ubsequent proces
-00011c10: 7369 6e67 2062 7920 6079 642d 7375 626d  sing by `yd-subm
-00011c20: 6974 602e 0a0a 4966 2074 6865 2076 616c  it`...If the val
-00011c30: 7565 2074 6f20 6265 2069 6e73 6572 7465  ue to be inserte
-00011c40: 6420 6973 2061 206e 756d 6265 7220 2861  d is a number (a
-00011c50: 6e20 696e 7465 6765 7220 6f72 2066 6c6f  n integer or flo
-00011c60: 6174 696e 6720 706f 696e 7420 7661 6c75  ating point valu
-00011c70: 6529 206f 7220 426f 6f6c 6561 6e2c 2074  e) or Boolean, t
-00011c80: 6865 2060 7b7b 6e75 6d3a 6d79 5f6e 756d  he `{{num:my_num
-00011c90: 6265 725f 7661 727d 7d60 2061 6e64 2060  ber_var}}` and `
-00011ca0: 7b7b 626f 6f6c 3a6d 795f 626f 6f6c 6561  {{bool:my_boolea
-00011cb0: 6e5f 7661 727d 7d60 2066 6f72 6d73 2063  n_var}}` forms c
-00011cc0: 616e 2062 6520 7573 6564 2069 6e20 7468  an be used in th
-00011cd0: 6520 4a53 4f4e 2066 696c 652c 2061 7320  e JSON file, as 
-00011ce0: 7769 7468 2074 6865 6972 2075 7365 2069  with their use i
-00011cf0: 6e20 6f74 6865 7220 7061 7274 7320 6f66  n other parts of
-00011d00: 2074 6865 204a 534f 4e20 576f 726b 2052   the JSON Work R
-00011d10: 6571 7569 7265 6d65 6e74 2073 7065 6369  equirement speci
-00011d20: 6669 6361 7469 6f6e 2e20 5468 6520 7375  fication. The su
-00011d30: 6273 7469 7475 7465 6420 7661 6c75 6520  bstituted value 
-00011d40: 7769 6c6c 2061 7373 756d 6520 7468 6520  will assume the 
-00011d50: 6e6f 6d69 6e61 7465 6420 7479 7065 2072  nominated type r
-00011d60: 6174 6865 7220 7468 616e 2062 6569 6e67  ather than being
-00011d70: 2061 2073 7472 696e 672e 0a0a 2323 2320   a string...### 
-00011d80: 5072 6f70 6572 7479 2049 6e68 6572 6974  Property Inherit
-00011d90: 616e 6365 0a0a 416c 6c20 7468 6520 7573  ance..All the us
-00011da0: 7561 6c20 7072 6f70 6572 7479 2069 6e68  ual property inh
-00011db0: 6572 6974 616e 6365 2066 6561 7475 7265  eritance feature
-00011dc0: 7320 6f70 6572 6174 6520 6173 206e 6f72  s operate as nor
-00011dd0: 6d61 6c2e 2050 726f 7065 7274 6965 7320  mal. Properties 
-00011de0: 6172 6520 696e 6865 7269 7465 6420 6672  are inherited fr
-00011df0: 6f6d 2074 6865 2060 636f 6e66 6967 2e74  om the `config.t
-00011e00: 6f6d 6c60 2066 696c 652c 2061 6e64 2066  oml` file, and f
-00011e10: 726f 6d20 7468 6520 7265 6c65 7661 6e74  rom the relevant
-00011e20: 2073 6563 7469 6f6e 7320 6f66 2074 6865   sections of the
-00011e30: 204a 534f 4e20 576f 726b 2052 6571 7569   JSON Work Requi
-00011e40: 7265 6d65 6e74 2066 696c 652e 2041 6e79  rement file. Any
-00011e50: 2070 726f 7065 7274 6965 7320 7365 7420   properties set 
-00011e60: 7769 7468 696e 2061 2054 6173 6b20 7072  within a Task pr
-00011e70: 6f74 6f74 7970 6520 6172 6520 636f 7069  ototype are copi
-00011e80: 6564 2074 6f20 616c 6c20 7468 6520 6765  ed to all the ge
-00011e90: 6e65 7261 7465 6420 5461 736b 732e 0a0a  nerated Tasks...
-00011ea0: 2323 2320 4d75 6c74 6970 6c65 2054 6173  ### Multiple Tas
-00011eb0: 6b20 4772 6f75 7073 2075 7369 6e67 204d  k Groups using M
-00011ec0: 756c 7469 706c 6520 4353 5620 4669 6c65  ultiple CSV File
-00011ed0: 730a 0a54 6865 2075 7365 206f 6620 6d75  s..The use of mu
-00011ee0: 6c74 6970 6c65 2054 6173 6b20 4772 6f75  ltiple Task Grou
-00011ef0: 7073 2069 7320 616c 736f 2073 7570 706f  ps is also suppo
-00011f00: 7274 6564 2c20 6279 2075 7369 6e67 206f  rted, by using o
-00011f10: 6e65 2043 5356 2066 696c 6520 7065 7220  ne CSV file per 
-00011f20: 5461 736b 2047 726f 7570 2e20 4561 6368  Task Group. Each
-00011f30: 2054 6173 6b20 4772 6f75 7020 6d75 7374   Task Group must
-00011f40: 2063 6f6e 7461 696e 206f 6e6c 7920 6120   contain only a 
-00011f50: 7369 6e67 6c65 2070 726f 746f 7479 7065  single prototype
-00011f60: 2054 6173 6b2e 0a0a 5468 6520 4353 5620   Task...The CSV 
-00011f70: 6669 6c65 7320 6172 6520 7375 7070 6c69  files are suppli
-00011f80: 6564 206f 6e20 7468 6520 636f 6d6d 616e  ed on the comman
-00011f90: 6420 6c69 6e65 2069 6e20 7468 6520 6f72  d line in the or
-00011fa0: 6465 7220 6f66 2074 6865 2054 6173 6b20  der of the Task 
-00011fb0: 4772 6f75 7073 2074 6f20 7768 6963 6820  Groups to which 
-00011fc0: 7468 6579 2061 7070 6c79 2e20 466f 7220  they apply. For 
-00011fd0: 6578 616d 706c 652c 2069 6620 6077 725f  example, if `wr_
-00011fe0: 6a73 6f6e 6020 636f 6e74 6169 6e73 2074  json` contains t
-00011ff0: 776f 2054 6173 6b20 4772 6f75 7073 2c20  wo Task Groups, 
-00012000: 6173 2066 6f6c 6c6f 7773 3a0a 0a60 6060  as follows:..```
-00012010: 6a73 6f6e 0a7b 0a20 2022 7461 736b 4772  json.{.  "taskGr
-00012020: 6f75 7073 223a 205b 0a20 2020 207b 0a20  oups": [.    {. 
-00012030: 2020 2020 2022 7461 736b 7322 3a20 5b0a       "tasks": [.
-00012040: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
-00012050: 2020 2020 2261 7267 756d 656e 7473 223a      "arguments":
-00012060: 205b 227b 7b61 7267 5f31 7d7d 222c 2022   ["{{arg_1}}", "
-00012070: 7b7b 6172 675f 327d 7d22 2c20 227b 7b61  {{arg_2}}", "{{a
-00012080: 7267 5f33 7d7d 225d 2c0a 2020 2020 2020  rg_3}}"],.      
-00012090: 2020 2020 2265 6e76 6972 6f6e 6d65 6e74      "environment
-000120a0: 223a 207b 2245 4e56 5f56 4152 5f31 223a  ": {"ENV_VAR_1":
-000120b0: 2022 7b7b 656e 765f 317d 7d22 7d0a 2020   "{{env_1}}"}.  
-000120c0: 2020 2020 2020 7d0a 2020 2020 2020 5d0a        }.      ].
-000120d0: 2020 2020 7d2c 0a20 2020 207b 0a20 2020      },.    {.   
-000120e0: 2020 2022 7461 736b 7322 3a20 5b0a 2020     "tasks": [.  
-000120f0: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-00012100: 2020 2261 7267 756d 656e 7473 223a 205b    "arguments": [
-00012110: 227b 7b61 7267 5f31 7d7d 222c 2022 7b7b  "{{arg_1}}", "{{
-00012120: 6172 675f 327d 7d22 5d2c 0a20 2020 2020  arg_2}}"],.     
-00012130: 2020 2020 2022 656e 7669 726f 6e6d 656e       "environmen
-00012140: 7422 3a20 7b22 454e 565f 5641 525f 3122  t": {"ENV_VAR_1"
-00012150: 3a20 227b 7b65 6e76 5f31 7d7d 222c 2022  : "{{env_1}}", "
-00012160: 454e 565f 5641 525f 3222 3a20 227b 7b65  ENV_VAR_2": "{{e
-00012170: 6e76 5f32 7d7d 227d 0a20 2020 2020 2020  nv_2}}"}.       
-00012180: 207d 0a20 2020 2020 205d 0a20 2020 207d   }.      ].    }
-00012190: 0a20 205d 0a7d 0a60 6060 0a0a 5468 6520  .  ].}.```..The 
-000121a0: 6079 642d 7375 626d 6974 6020 636f 6d6d  `yd-submit` comm
-000121b0: 616e 6420 776f 756c 6420 7468 656e 2062  and would then b
-000121c0: 6520 696e 766f 6b65 6420 7769 7468 2061  e invoked with a
-000121d0: 2073 6570 6172 6174 6520 4353 5620 6669   separate CSV fi
-000121e0: 6c65 2066 6f72 2065 6163 6820 5461 736b  le for each Task
-000121f0: 2047 726f 7570 2c20 652e 672e 3a0a 0a60   Group, e.g.:..`
-00012200: 6060 7368 656c 6c0a 7964 2d73 7562 6d69  ``shell.yd-submi
-00012210: 7420 2d72 2077 722e 6a73 6f6e 202d 5620  t -r wr.json -V 
-00012220: 7772 5f64 6174 615f 7461 736b 5f67 726f  wr_data_task_gro
-00012230: 7570 5f31 2e63 7376 202d 5620 7772 5f64  up_1.csv -V wr_d
-00012240: 6174 615f 7461 736b 5f67 726f 7570 5f32  ata_task_group_2
-00012250: 2e63 7376 0a60 6060 0a0a 4966 2074 6865  .csv.```..If the
-00012260: 7265 2061 7265 202a 2a66 6577 6572 2a2a  re are **fewer**
-00012270: 2043 5356 2066 696c 6573 2074 6861 6e20   CSV files than 
-00012280: 5461 736b 2047 726f 7570 7320 6120 7761  Task Groups a wa
-00012290: 726e 696e 6720 7769 6c6c 2062 6520 7072  rning will be pr
-000122a0: 696e 7465 6420 616e 642c 2069 6620 7468  inted and, if th
-000122b0: 6572 6520 6172 6520 276e 2720 4353 5620  ere are 'n' CSV 
-000122c0: 6669 6c65 732c 2043 5356 2064 6174 6120  files, CSV data 
-000122d0: 7072 6f63 6573 7369 6e67 2077 696c 6c20  processing will 
-000122e0: 6265 2061 7070 6c69 6564 2074 6f20 7468  be applied to th
-000122f0: 6520 6669 7273 7420 276e 2720 5461 736b  e first 'n' Task
-00012300: 2047 726f 7570 7320 696e 2074 6865 2057   Groups in the W
-00012310: 6f72 6b20 5265 7175 6972 656d 656e 7420  ork Requirement 
-00012320: 6279 2064 6566 6175 6c74 2c20 696e 2074  by default, in t
-00012330: 6865 206f 7264 6572 2069 6e20 7768 6963  he order in whic
-00012340: 6820 7468 6520 4353 5620 6669 6c65 7320  h the CSV files 
-00012350: 7765 7265 2073 7570 706c 6965 642e 2049  were supplied. I
-00012360: 6620 7468 6572 6520 6172 6520 2a2a 6d6f  f there are **mo
-00012370: 7265 2a2a 2043 5356 2066 696c 6573 2074  re** CSV files t
-00012380: 6861 6e20 5461 736b 2047 726f 7570 732c  han Task Groups,
-00012390: 2061 6e20 6572 726f 7220 7769 6c6c 2062   an error will b
-000123a0: 6520 7261 6973 6564 2061 6e64 2070 726f  e raised and pro
-000123b0: 6365 7373 696e 6720 7769 6c6c 2073 746f  cessing will sto
-000123c0: 702e 0a0a 4974 2069 7320 706f 7373 6962  p...It is possib
-000123d0: 6c65 2074 6f20 6170 706c 7920 4353 5620  le to apply CSV 
-000123e0: 6669 6c65 7320 6578 706c 6963 6974 6c79  files explicitly
-000123f0: 2074 6f20 7370 6563 6966 6963 2054 6173   to specific Tas
-00012400: 6b20 4772 6f75 7073 2c20 6279 2075 7369  k Groups, by usi
-00012410: 6e67 2061 6e20 6f70 7469 6f6e 616c 202a  ng an optional *
-00012420: 2a69 6e64 6578 2070 6f73 7466 6978 2a2a  *index postfix**
-00012430: 2028 652e 672e 2c20 603a 3260 2920 6174   (e.g., `:2`) at
-00012440: 2074 6865 2065 6e64 206f 6620 6561 6368   the end of each
-00012450: 2043 5356 2066 696c 656e 616d 652e 2046   CSV filename. F
-00012460: 6f72 2065 7861 6d70 6c65 2c20 6966 2074  or example, if t
-00012470: 6865 7265 2061 7265 2074 776f 2043 5356  here are two CSV
-00012480: 2066 696c 6573 2074 6f20 6265 2061 7070   files to be app
-00012490: 6c69 6564 2074 6f20 7468 6520 7365 636f  lied to the seco
-000124a0: 6e64 2061 6e64 2066 6f75 7274 6820 5461  nd and fourth Ta
-000124b0: 736b 2047 726f 7570 7320 696e 2061 204a  sk Groups in a J
-000124c0: 534f 4e20 576f 726b 2052 6571 7569 7265  SON Work Require
-000124d0: 6d65 6e74 2c20 7573 6520 7468 6520 666f  ment, use the fo
-000124e0: 6c6c 6f77 696e 6720 7379 6e74 6178 3a0a  llowing syntax:.
-000124f0: 0a60 6060 7368 656c 6c0a 7964 2d73 7562  .```shell.yd-sub
-00012500: 6d69 7420 2d72 2077 722e 6a73 6f6e 202d  mit -r wr.json -
-00012510: 5620 7772 5f64 6174 615f 7461 736b 5f67  V wr_data_task_g
-00012520: 726f 7570 5f32 2e63 7376 3a32 202d 5620  roup_2.csv:2 -V 
-00012530: 7772 5f64 6174 615f 7461 736b 5f67 726f  wr_data_task_gro
-00012540: 7570 5f34 2e63 7376 3a34 0a60 6060 0a0a  up_4.csv:4.```..
-00012550: 416c 7465 726e 6174 6976 656c 792c 2074  Alternatively, t
-00012560: 6865 202a 2a54 6173 6b20 4772 6f75 7020  he **Task Group 
-00012570: 6e61 6d65 2a2a 2028 6966 2073 7570 706c  name** (if suppl
-00012580: 6965 6420 696e 2074 6865 204a 534f 4e20  ied in the JSON 
-00012590: 6669 6c65 2920 6361 6e20 6265 2075 7365  file) can be use
-000125a0: 6420 6173 2074 6865 2070 6f73 7466 6978  d as the postfix
-000125b0: 2e20 466f 7220 6578 616d 706c 652c 2069  . For example, i
-000125c0: 6620 7468 6520 5461 736b 2047 726f 7570  f the Task Group
-000125d0: 7320 6162 6f76 6520 6172 6520 6e61 6d65  s above are name
-000125e0: 6420 6074 675f 7477 6f60 2061 6e64 2060  d `tg_two` and `
-000125f0: 7467 5f66 6f75 7260 2c20 7468 6520 6079  tg_four`, the `y
-00012600: 642d 7375 626d 6974 6020 636f 6d6d 616e  d-submit` comman
-00012610: 6420 776f 756c 6420 6265 636f 6d65 3a0a  d would become:.
-00012620: 0a60 6060 7368 656c 6c0a 7964 2d73 7562  .```shell.yd-sub
-00012630: 6d69 7420 2d72 2077 722e 6a73 6f6e 202d  mit -r wr.json -
-00012640: 5620 7772 5f64 6174 615f 7461 736b 5f67  V wr_data_task_g
-00012650: 726f 7570 5f32 2e63 7376 3a74 675f 7477  roup_2.csv:tg_tw
-00012660: 6f20 2d56 2077 725f 6461 7461 5f74 6173  o -V wr_data_tas
-00012670: 6b5f 6772 6f75 705f 342e 6373 763a 7467  k_group_4.csv:tg
-00012680: 5f66 6f75 720a 6060 600a 0a4e 6f74 6520  _four.```..Note 
-00012690: 7468 6174 206f 6e6c 7920 6f6e 6520 4353  that only one CS
-000126a0: 5620 6669 6c65 2063 616e 2062 6520 6170  V file can be ap
-000126b0: 706c 6965 6420 746f 2061 6e79 2067 6976  plied to any giv
-000126c0: 656e 2054 6173 6b20 4772 6f75 702e 2041  en Task Group. A
-000126d0: 2073 696e 676c 6520 4353 5620 6669 6c65   single CSV file
-000126e0: 2063 616e 2c20 686f 7765 7665 722c 2062   can, however, b
-000126f0: 6520 7265 7573 6564 2066 6f72 206d 756c  e reused for mul
-00012700: 7469 706c 6520 5461 736b 2047 726f 7570  tiple Task Group
-00012710: 732e 0a0a 2323 2320 5573 696e 6720 4353  s...### Using CS
-00012720: 5620 4461 7461 2077 6974 6820 5369 6d70  V Data with Simp
-00012730: 6c65 2c20 544f 4d4c 2d4f 6e6c 7920 576f  le, TOML-Only Wo
-00012740: 726b 2052 6571 7569 7265 6d65 6e74 2053  rk Requirement S
-00012750: 7065 6369 6669 6361 7469 6f6e 730a 0a49  pecifications..I
-00012760: 7427 7320 706f 7373 6962 6c65 2074 6f20  t's possible to 
-00012770: 7573 6520 544f 4d4c 2065 7863 6c75 7369  use TOML exclusi
-00012780: 7665 6c79 2074 6f20 6465 7269 7665 2061  vely to derive a
-00012790: 206c 6973 7420 6f66 2054 6173 6b73 2066   list of Tasks f
-000127a0: 726f 6d20 4353 5620 6461 7461 202d 2d20  rom CSV data -- 
-000127b0: 692e 652e 2c20 6120 4a53 4f4e 2057 6f72  i.e., a JSON Wor
-000127c0: 6b20 5265 7175 6972 656d 656e 7420 7370  k Requirement sp
-000127d0: 6563 6966 6963 6174 696f 6e20 6973 206e  ecification is n
-000127e0: 6f74 2072 6571 7569 7265 642e 0a0a 546f  ot required...To
-000127f0: 206d 616b 6520 7573 6520 6f66 2074 6869   make use of thi
-00012800: 733a 0a0a 312e 2045 6e73 7572 6520 7468  s:..1. Ensure th
-00012810: 6174 206e 6f20 4a53 4f4e 2057 6f72 6b20  at no JSON Work 
-00012820: 5265 7175 6972 656d 656e 7420 646f 6375  Requirement docu
-00012830: 6d65 6e74 2069 7320 7370 6563 6966 6965  ment is specifie
-00012840: 6420 286e 6f20 6077 6f72 6b52 6571 7569  d (no `workRequi
-00012850: 7265 6d65 6e74 4461 7461 6020 696e 2074  rementData` in t
-00012860: 6865 2054 4f4d 4c20 6669 6c65 2c20 6f72  he TOML file, or
-00012870: 2060 2d2d 776f 726b 2d72 6571 7569 7265   `--work-require
-00012880: 6d65 6e74 6020 6f6e 2074 6865 2063 6f6d  ment` on the com
-00012890: 6d61 6e64 206c 696e 6529 0a32 2e20 496e  mand line).2. In
-000128a0: 7365 7274 2074 6865 2072 6571 7569 7265  sert the require
-000128b0: 6420 4353 562d 7375 7070 6c69 6564 2076  d CSV-supplied v
-000128c0: 6172 6961 626c 6520 7375 6273 7469 7475  ariable substitu
-000128d0: 7469 6f6e 7320 6469 7265 6374 6c79 2069  tions directly i
-000128e0: 6e74 6f20 7468 6520 544f 4d4c 2070 726f  nto the TOML pro
-000128f0: 7065 7274 6965 732c 2065 2e67 2e20 6061  perties, e.g. `a
-00012900: 7267 756d 656e 7473 203d 205b 227b 7b61  rguments = ["{{a
-00012910: 7267 5f31 7d7d 222c 2022 7b7b 6172 675f  rg_1}}", "{{arg_
-00012920: 327d 7d22 5d60 0a33 2e20 5370 6563 6966  2}}"]`.3. Specif
-00012930: 7920 6120 7369 6e67 6c65 2043 5356 2066  y a single CSV f
-00012940: 696c 6520 696e 2074 6865 2060 6373 7646  ile in the `csvF
-00012950: 696c 6573 6020 544f 4d4c 2070 726f 7065  iles` TOML prope
-00012960: 7274 792c 2065 2e67 2e20 6063 7376 4669  rty, e.g. `csvFi
-00012970: 6c65 7320 3d20 5b22 7772 5f64 6174 612e  les = ["wr_data.
-00012980: 6373 7622 5d60 2c20 6f72 2070 726f 7669  csv"]`, or provi
-00012990: 6465 2074 6865 2043 5356 2066 696c 6520  de the CSV file 
-000129a0: 6f6e 2074 6865 2063 6f6d 6d61 6e64 206c  on the command l
-000129b0: 696e 6520 602d 5620 7772 5f64 6174 612e  ine `-V wr_data.
-000129c0: 6373 7660 0a0a 5768 656e 2060 7964 2d73  csv`..When `yd-s
-000129d0: 7562 6d69 7460 2069 7320 7275 6e2c 2069  ubmit` is run, i
-000129e0: 7420 7769 6c6c 2065 7870 616e 6420 7468  t will expand th
-000129f0: 6520 5461 736b 206c 6973 7420 746f 206d  e Task list to m
-00012a00: 6174 6368 2074 6865 206e 756d 6265 7220  atch the number 
-00012a10: 6f66 2064 6174 6120 726f 7773 2069 6e20  of data rows in 
-00012a20: 7468 6520 4353 5620 6669 6c65 2e0a 0a23  the CSV file...#
-00012a30: 2323 2049 6e73 7065 6374 696e 6720 7468  ## Inspecting th
-00012a40: 6520 5265 7375 6c74 7320 6f66 2043 5356  e Results of CSV
-00012a50: 2056 6172 6961 626c 6520 5375 6273 7469   Variable Substi
-00012a60: 7475 7469 6f6e 0a0a 5468 6520 602d 2d70  tution..The `--p
-00012a70: 726f 6365 7373 2d63 7376 2d6f 6e6c 7960  rocess-csv-only`
-00012a80: 2028 6f72 2060 2d70 6029 206f 7074 696f   (or `-p`) optio
-00012a90: 6e20 6361 6e20 6265 2075 7365 6420 7769  n can be used wi
-00012aa0: 7468 2060 7964 2d73 7562 6d69 7460 2074  th `yd-submit` t
-00012ab0: 6f20 6f75 7470 7574 2074 6865 204a 534f  o output the JSO
-00012ac0: 4e20 576f 726b 2052 6571 7569 7265 6d65  N Work Requireme
-00012ad0: 6e74 2061 6674 6572 2043 5356 2076 6172  nt after CSV var
-00012ae0: 6961 626c 6520 7375 6273 7469 7475 7469  iable substituti
-00012af0: 6f6e 7320 6f6e 6c79 2c20 7072 696f 7220  ons only, prior 
-00012b00: 746f 2061 6c6c 206f 7468 6572 2073 7562  to all other sub
-00012b10: 7374 6974 7574 696f 6e73 2061 6e64 2070  stitutions and p
-00012b20: 726f 7065 7274 7920 696e 6865 7269 7461  roperty inherita
-00012b30: 6e63 6520 6170 706c 6965 6420 6279 2060  nce applied by `
-00012b40: 7964 2d73 7562 6d69 7460 2e0a 0a23 2057  yd-submit`...# W
-00012b50: 6f72 6b65 7220 506f 6f6c 2050 726f 7065  orker Pool Prope
-00012b60: 7274 6965 730a 0a54 6865 2060 776f 726b  rties..The `work
-00012b70: 6572 506f 6f6c 6020 7365 6374 696f 6e20  erPool` section 
-00012b80: 6f66 2074 6865 2054 4f4d 4c20 6669 6c65  of the TOML file
-00012b90: 2064 6566 696e 6573 2074 6865 2070 726f   defines the pro
-00012ba0: 7065 7274 6965 7320 6f66 2074 6865 2057  perties of the W
-00012bb0: 6f72 6b65 7220 506f 6f6c 2074 6f20 6265  orker Pool to be
-00012bc0: 2063 7265 6174 6564 2c20 616e 6420 6973   created, and is
-00012bd0: 2075 7365 6420 6279 2074 6865 2060 7964   used by the `yd
-00012be0: 2d70 726f 7669 7369 6f6e 6020 636f 6d6d  -provision` comm
-00012bf0: 616e 642e 2041 2073 7562 7365 7420 6f66  and. A subset of
-00012c00: 2074 6865 2070 726f 7065 7274 6965 7320   the properties 
-00012c10: 6973 2061 6c73 6f20 7573 6564 2062 7920  is also used by 
-00012c20: 7468 6520 6079 642d 696e 7374 616e 7469  the `yd-instanti
-00012c30: 6174 6560 2063 6f6d 6d61 6e64 2c20 666f  ate` command, fo
-00012c40: 7220 6372 6561 7469 6e67 2073 7461 6e64  r creating stand
-00012c50: 616c 6f6e 6520 436f 6d70 7574 6520 5265  alone Compute Re
-00012c60: 7175 6972 656d 656e 7473 2074 6861 7420  quirements that 
-00012c70: 6172 6520 6e6f 7420 6173 736f 6369 6174  are not associat
-00012c80: 6564 2077 6974 6820 576f 726b 6572 2050  ed with Worker P
-00012c90: 6f6f 6c73 2e0a 0a54 6865 206f 6e6c 7920  ools...The only 
-00012ca0: 6d61 6e64 6174 6f72 7920 7072 6f70 6572  mandatory proper
-00012cb0: 7479 2069 7320 6074 656d 706c 6174 6549  ty is `templateI
-00012cc0: 6460 2e20 416c 6c20 6f74 6865 7220 7072  d`. All other pr
-00012cd0: 6f70 6572 7469 6573 2068 6176 6520 6465  operties have de
-00012ce0: 6661 756c 7473 2028 6f72 2061 7265 206e  faults (or are n
-00012cf0: 6f74 2072 6571 7569 7265 6429 2e0a 0a54  ot required)...T
-00012d00: 6865 2066 6f6c 6c6f 7769 6e67 2070 726f  he following pro
-00012d10: 7065 7274 6965 7320 6172 6520 6176 6169  perties are avai
-00012d20: 6c61 626c 653a 0a0a 7c20 5072 6f70 6572  lable:..| Proper
-00012d30: 7479 2020 2020 2020 2020 2020 2020 2020  ty              
-00012d40: 2020 2020 7c20 4465 7363 7269 7074 696f      | Descriptio
-00012d50: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-00012d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012db0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00012dc0: 4465 6661 756c 7420 2020 2020 2020 2020  Default         
-00012dd0: 2020 2020 2020 2020 7c0a 7c3a 2d2d 2d2d          |.|:----
-00012de0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00012df0: 2d2d 2d2d 2d2d 7c3a 2d2d 2d2d 2d2d 2d2d  ------|:--------
-00012e00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00012e10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00012e20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00012e30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00012e40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00012e50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00012e60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00012e70: 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |:--------------
-00012e80: 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a 7c20 6069  ----------|.| `i
-00012e90: 646c 654e 6f64 6553 6875 7464 6f77 6e45  dleNodeShutdownE
-00012ea0: 6e61 626c 6564 6020 7c20 5768 6574 6865  nabled` | Whethe
-00012eb0: 7220 746f 2073 6875 7420 646f 776e 206e  r to shut down n
-00012ec0: 6f64 6573 2074 6861 7420 6861 7665 2062  odes that have b
-00012ed0: 6565 6e20 6964 6c65 2066 6f72 2060 6964  een idle for `id
-00012ee0: 6c65 4e6f 6465 5368 7574 646f 776e 5469  leNodeShutdownTi
-00012ef0: 6d65 6f75 7460 206d 696e 7574 6573 2e20  meout` minutes. 
-00012f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f20: 2020 7c20 6054 7275 6560 2020 2020 2020    | `True`      
-00012f30: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
-00012f40: 6069 646c 654e 6f64 6553 6875 7464 6f77  `idleNodeShutdow
-00012f50: 6e54 696d 656f 7574 6020 7c20 5468 6520  nTimeout` | The 
-00012f60: 7469 6d65 6f75 7420 696e 206d 696e 7574  timeout in minut
-00012f70: 6573 2061 6674 6572 2077 6869 6368 2061  es after which a
-00012f80: 6e20 6964 6c65 206e 6f64 6520 7769 6c6c  n idle node will
-00012f90: 2062 6520 7368 7574 2064 6f77 6e20 6966   be shut down if
-00012fa0: 2060 6964 6c65 4e6f 6465 5368 7574 646f   `idleNodeShutdo
-00012fb0: 776e 456e 6162 6c65 6460 2069 7320 7365  wnEnabled` is se
-00012fc0: 7420 746f 2060 5472 7565 602e 2020 2020  t to `True`.    
-00012fd0: 2020 2020 7c20 6035 2e30 6020 2020 2020      | `5.0`     
-00012fe0: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-00012ff0: 7c20 6069 646c 6550 6f6f 6c53 6875 7464  | `idlePoolShutd
-00013000: 6f77 6e45 6e61 626c 6564 6020 7c20 5768  ownEnabled` | Wh
-00013010: 6574 6865 7220 746f 2073 6875 7420 646f  ether to shut do
-00013020: 776e 2074 6865 2057 6f72 6b65 7220 506f  wn the Worker Po
-00013030: 6f6c 2077 6865 6e20 6974 2068 6173 2062  ol when it has b
-00013040: 6565 6e20 6964 6c65 2066 6f72 2060 6964  een idle for `id
-00013050: 6c65 506f 6f6c 5368 7574 646f 776e 5469  lePoolShutdownTi
-00013060: 6d65 6f75 7460 206d 696e 7574 6573 2e20  meout` minutes. 
-00013070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013080: 2020 2020 2020 7c20 6054 7275 6560 2020        | `True`  
-00013090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000130a0: 7c0a 7c20 6069 646c 6550 6f6f 6c53 6875  |.| `idlePoolShu
-000130b0: 7464 6f77 6e54 696d 656f 7574 6020 7c20  tdownTimeout` | 
-000130c0: 5468 6520 7469 6d65 6f75 7420 696e 206d  The timeout in m
-000130d0: 696e 7574 6573 2061 6674 6572 2077 6869  inutes after whi
-000130e0: 6368 2061 6e20 6964 6c65 2057 6f72 6b65  ch an idle Worke
-000130f0: 7220 506f 6f6c 2077 696c 6c20 6265 2073  r Pool will be s
-00013100: 6875 7420 646f 776e 2069 6620 6069 646c  hut down if `idl
-00013110: 6550 6f6f 6c53 6875 7464 6f77 6e45 6e61  ePoolShutdownEna
-00013120: 626c 6564 6020 6973 2073 6574 2074 6f20  bled` is set to 
-00013130: 6054 7275 6560 2e20 7c20 6033 302e 3060  `True`. | `30.0`
-00013140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013150: 2020 7c0a 7c20 6069 6d61 6765 7349 6460    |.| `imagesId`
-00013160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013170: 7c20 5468 6520 696d 6167 6573 2049 4420  | The images ID 
-00013180: 746f 2075 7365 2077 6865 6e20 626f 6f74  to use when boot
-00013190: 696e 6720 696e 7374 616e 6365 732e 2020  ing instances.  
-000131a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000131b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000131c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000131d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000131e0: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-000131f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013200: 2020 2020 7c0a 7c20 6069 6e73 7461 6e63      |.| `instanc
-00013210: 6554 6167 7360 2020 2020 2020 2020 2020  eTags`          
-00013220: 2020 7c20 5468 6520 6469 6374 696f 6e61    | The dictiona
-00013230: 7279 206f 6620 696e 7374 616e 6365 2074  ry of instance t
-00013240: 6167 7320 746f 2061 7070 6c79 2074 6f20  ags to apply to 
-00013250: 7468 6520 696e 7374 616e 6365 732e 2020  the instances.  
-00013260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013290: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-000132a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000132b0: 2020 2020 2020 7c0a 7c20 606d 696e 4e6f        |.| `minNo
-000132c0: 6465 7360 2020 2020 2020 2020 2020 2020  des`            
-000132d0: 2020 2020 7c20 5468 6520 6d69 6e69 6d75      | The minimu
-000132e0: 6d20 6e75 6d62 6572 206f 6620 6e6f 6465  m number of node
-000132f0: 7320 746f 2077 6869 6368 2074 6865 2057  s to which the W
-00013300: 6f72 6b65 7220 506f 6f6c 2063 616e 2062  orker Pool can b
-00013310: 6520 7363 616c 6564 2064 6f77 6e2e 2020  e scaled down.  
+00008710: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+00008720: 2020 2020 7c20 5965 7320 7c20 5965 7320      | Yes | Yes 
+00008730: 207c 2020 2020 2020 7c0a 7c20 6074 6173   |      |.| `tas
+00008740: 6b73 5065 7257 6f72 6b65 7260 2020 2020  ksPerWorker`    
+00008750: 2020 2020 2020 207c 2044 6574 6572 6d69         | Determi
+00008760: 6e65 7320 7468 6520 6e75 6d62 6572 206f  nes the number o
+00008770: 6620 576f 726b 6572 2063 6c61 696d 7320  f Worker claims 
+00008780: 6261 7365 6420 6f6e 2073 706c 6974 7469  based on splitti
+00008790: 6e67 2074 6865 206e 756d 6265 7220 6f66  ng the number of
+000087a0: 2075 6e66 696e 6973 6865 6420 5461 736b   unfinished Task
+000087b0: 7320 6163 726f 7373 2057 6f72 6b65 7273  s across Workers
+000087c0: 2e20 452e 672e 2c20 6031 602e 2020 2020  . E.g., `1`.    
+000087d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000087e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000087f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008800: 2020 7c20 5965 7320 207c 2059 6573 207c    | Yes  | Yes |
+00008810: 2059 6573 2020 7c20 2020 2020 207c 0a7c   Yes  |      |.|
+00008820: 2060 7570 6c6f 6164 4669 6c65 7360 2020   `uploadFiles`  
+00008830: 2020 2020 2020 2020 2020 2020 7c20 5468              | Th
+00008840: 6520 6c69 7374 206f 6620 6669 6c65 7320  e list of files 
+00008850: 746f 2062 6520 7570 6c6f 6164 6564 2074  to be uploaded t
+00008860: 6f20 7468 6520 5965 6c6c 6f77 446f 6720  o the YellowDog 
+00008870: 4f62 6a65 6374 2053 746f 7265 2e20 452e  Object Store. E.
+00008880: 672e 2c20 284a 534f 4e29 3a20 605b 7b22  g., (JSON): `[{"
+00008890: 6c6f 6361 6c50 6174 6822 3a20 6669 6c65  localPath": file
+000088a0: 5f31 2e74 7874 222c 2022 7570 6c6f 6164  _1.txt", "upload
+000088b0: 5061 7468 223a 2022 6669 6c65 5f31 2e74  Path": "file_1.t
+000088c0: 7874 227d 5d60 2e20 2020 2020 2020 2020  xt"}]`.         
+000088d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000088e0: 2020 2020 2020 207c 2059 6573 2020 7c20         | Yes  | 
+000088f0: 5965 7320 7c20 5965 7320 207c 2059 6573  Yes | Yes  | Yes
+00008900: 2020 7c0a 7c20 6076 6370 7573 6020 2020    |.| `vcpus`   
+00008910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008920: 207c 2052 616e 6765 2063 6f6e 7374 7261   | Range constra
+00008930: 696e 7420 6f6e 206e 756d 6265 7220 6f66  int on number of
+00008940: 2076 4350 5573 2074 6861 7420 6172 6520   vCPUs that are 
+00008950: 7265 7175 6972 6564 2074 6f20 6578 6563  required to exec
+00008960: 7574 6520 5461 736b 7320 452e 672e 2c20  ute Tasks E.g., 
+00008970: 605b 322e 302c 2034 2e30 5d60 2e20 2020  `[2.0, 4.0]`.   
+00008980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000089a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000089b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000089c0: 2020 2020 2020 2020 2020 2020 7c20 5965              | Ye
+000089d0: 7320 207c 2059 6573 207c 2059 6573 2020  s  | Yes | Yes  
+000089e0: 7c20 2020 2020 207c 0a7c 2060 7665 7269  |      |.| `veri
+000089f0: 6679 4174 5374 6172 7460 2020 2020 2020  fyAtStart`      
+00008a00: 2020 2020 2020 7c20 4120 6c69 7374 206f        | A list o
+00008a10: 6620 6669 6c65 7320 7265 7175 6972 6564  f files required
+00008a20: 2062 7920 6120 5461 736b 2e20 4d75 7374   by a Task. Must
+00008a30: 2062 6520 7072 6573 656e 7420 7768 656e   be present when
+00008a40: 2074 6865 2054 6173 6b20 6973 2072 6561   the Task is rea
+00008a50: 6479 2074 6f20 7374 6172 7420 6f72 2074  dy to start or t
+00008a60: 6865 2054 6173 6b20 7769 6c6c 2066 6169  he Task will fai
+00008a70: 6c2e 2045 2e67 2e3a 2060 5b22 7461 736b  l. E.g.: `["task
+00008a80: 5f67 726f 7570 5f31 2f74 6173 6b5f 312f  _group_1/task_1/
+00008a90: 7265 7375 6c74 732e 7478 7422 5d60 2e20  results.txt"]`. 
+00008aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ab0: 207c 2059 6573 2020 7c20 5965 7320 7c20   | Yes  | Yes | 
+00008ac0: 5965 7320 207c 2059 6573 2020 7c0a 7c20  Yes  | Yes  |.| 
+00008ad0: 6076 6572 6966 7957 6169 7460 2020 2020  `verifyWait`    
+00008ae0: 2020 2020 2020 2020 2020 207c 2041 206c             | A l
+00008af0: 6973 7420 6f66 2066 696c 6573 2072 6571  ist of files req
+00008b00: 7569 7265 6420 6279 2061 2054 6173 6b2e  uired by a Task.
+00008b10: 2054 6865 2054 6173 6b20 7769 6c6c 2077   The Task will w
+00008b20: 6169 7420 756e 7469 6c20 7468 6520 6669  ait until the fi
+00008b30: 6c65 7320 6172 6520 6176 6169 6c61 626c  les are availabl
+00008b40: 6520 6265 666f 7265 2073 7461 7274 696e  e before startin
+00008b50: 672e 2045 2e67 2e3a 2060 5b22 7461 736b  g. E.g.: `["task
+00008b60: 5f67 726f 7570 5f31 2f74 6173 6b5f 312f  _group_1/task_1/
+00008b70: 7265 7375 6c74 732e 7478 7422 5d60 2e20  results.txt"]`. 
+00008b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b90: 2020 2020 2020 7c20 5965 7320 207c 2059        | Yes  | Y
+00008ba0: 6573 207c 2059 6573 2020 7c20 5965 7320  es | Yes  | Yes 
+00008bb0: 207c 0a7c 2060 776f 726b 6572 5461 6773   |.| `workerTags
+00008bc0: 6020 2020 2020 2020 2020 2020 2020 2020  `               
+00008bd0: 7c20 5468 6520 6c69 7374 206f 6620 576f  | The list of Wo
+00008be0: 726b 6572 2054 6167 7320 7468 6174 2077  rker Tags that w
+00008bf0: 696c 6c20 6265 2075 7365 6420 746f 206d  ill be used to m
+00008c00: 6174 6368 2061 6761 696e 7374 2074 6865  atch against the
+00008c10: 2057 6f72 6b65 7220 5461 6720 6f66 2061   Worker Tag of a
+00008c20: 2063 616e 6469 6461 7465 2057 6f72 6b65   candidate Worke
+00008c30: 722e 2045 2e67 2e2c 2060 5b22 7461 675f  r. E.g., `["tag_
+00008c40: 7822 2c20 2274 6167 5f79 225d 602e 2020  x", "tag_y"]`.  
+00008c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008c70: 2020 2020 2020 2020 2020 207c 2059 6573             | Yes
+00008c80: 2020 7c20 5965 7320 7c20 5965 7320 207c    | Yes | Yes  |
+00008c90: 2020 2020 2020 7c0a 7c20 6077 6f72 6b52        |.| `workR
+00008ca0: 6571 7569 7265 6d65 6e74 4461 7461 6020  equirementData` 
+00008cb0: 2020 2020 207c 2054 6865 206e 616d 6520       | The name 
+00008cc0: 6f66 2074 6865 2066 696c 6520 636f 6e74  of the file cont
+00008cd0: 6169 6e69 6e67 2074 6865 204a 534f 4e20  aining the JSON 
+00008ce0: 646f 6375 6d65 6e74 2069 6e20 7768 6963  document in whic
+00008cf0: 6820 7468 6520 576f 726b 2052 6571 7569  h the Work Requi
+00008d00: 7265 6d65 6e74 2069 7320 6465 6669 6e65  rement is define
+00008d10: 642e 2045 2e67 2e2c 2060 2274 6573 745f  d. E.g., `"test_
+00008d20: 776f 726b 7265 712e 6a73 6f6e 2260 2e20  workreq.json"`. 
+00008d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008d60: 7c20 5965 7320 207c 2020 2020 207c 2020  | Yes  |     |  
+00008d70: 2020 2020 7c20 2020 2020 207c 0a0a 2323      |      |..##
+00008d80: 2041 7574 6f6d 6174 6963 2050 726f 7065   Automatic Prope
+00008d90: 7274 6965 730a 0a49 6e20 6164 6469 7469  rties..In additi
+00008da0: 6f6e 2074 6f20 7468 6520 696e 6865 7269  on to the inheri
+00008db0: 7461 6e63 6520 6d65 6368 616e 6973 6d2c  tance mechanism,
+00008dc0: 2073 6f6d 6520 7072 6f70 6572 7469 6573   some properties
+00008dd0: 2061 7265 2073 6574 2061 7574 6f6d 6174   are set automat
+00008de0: 6963 616c 6c79 2062 7920 7468 6520 6079  ically by the `y
+00008df0: 642d 7375 626d 6974 6020 636f 6d6d 616e  d-submit` comman
+00008e00: 642c 2061 7320 6120 7573 6167 6520 636f  d, as a usage co
+00008e10: 6e76 656e 6965 6e63 6520 6966 2074 6865  nvenience if the
+00008e20: 7927 7265 206e 6f74 2065 7870 6c69 6369  y're not explici
+00008e30: 746c 7920 7072 6f76 6964 6564 2e0a 0a23  tly provided...#
+00008e40: 2323 2057 6f72 6b20 5265 7175 6972 656d  ## Work Requirem
+00008e50: 656e 742c 2054 6173 6b20 4772 6f75 7020  ent, Task Group 
+00008e60: 616e 6420 5461 736b 204e 616d 696e 670a  and Task Naming.
+00008e70: 0a2d 2054 6865 202a 2a57 6f72 6b20 5265  .- The **Work Re
+00008e80: 7175 6972 656d 656e 742a 2a20 6e61 6d65  quirement** name
+00008e90: 2069 7320 6175 746f 6d61 7469 6361 6c6c   is automaticall
+00008ea0: 7920 7365 7420 7573 696e 6720 6120 636f  y set using a co
+00008eb0: 6e63 6174 656e 6174 696f 6e20 6f66 2074  ncatenation of t
+00008ec0: 6865 2060 7461 6760 2070 726f 7065 7274  he `tag` propert
+00008ed0: 792c 2061 2055 5443 2074 696d 6573 7461  y, a UTC timesta
+00008ee0: 6d70 2c20 616e 6420 7468 7265 6520 7261  mp, and three ra
+00008ef0: 6e64 6f6d 2068 6578 2063 6861 7261 6374  ndom hex charact
+00008f00: 6572 733a 2065 2c67 2c2e 2060 6d79 7461  ers: e,g,. `myta
+00008f10: 675f 3232 3130 3234 2d31 3535 3532 342d  g_221024-155524-
+00008f20: 3430 6160 2e0a 2d20 2a2a 5461 736b 2047  40a`..- **Task G
+00008f30: 726f 7570 2a2a 206e 616d 6573 2061 7265  roup** names are
+00008f40: 2061 7574 6f6d 6174 6963 616c 6c79 2063   automatically c
+00008f50: 7265 6174 6564 2066 6f72 2061 6e79 2054  reated for any T
+00008f60: 6173 6b20 4772 6f75 7020 7468 6174 2069  ask Group that i
+00008f70: 7320 6e6f 7420 6578 706c 6963 6974 6c79  s not explicitly
+00008f80: 206e 616d 6564 2c20 7573 696e 6720 6e61   named, using na
+00008f90: 6d65 7320 6f66 2074 6865 2066 6f72 6d20  mes of the form 
+00008fa0: 6074 6173 6b5f 6772 6f75 705f 3160 2028  `task_group_1` (
+00008fb0: 6f72 2060 7461 736b 5f67 726f 7570 5f30  or `task_group_0
+00008fc0: 3160 2c20 6574 632e 2c20 666f 7220 6c61  1`, etc., for la
+00008fd0: 7267 6572 206e 756d 6265 7273 206f 6620  rger numbers of 
+00008fe0: 5461 736b 2047 726f 7570 7329 2e20 5461  Task Groups). Ta
+00008ff0: 736b 2047 726f 7570 206e 756d 6265 7273  sk Group numbers
+00009000: 2063 616e 2061 6c73 6f20 6265 2069 6e63   can also be inc
+00009010: 6c75 6465 6420 696e 2075 7365 722d 6465  luded in user-de
+00009020: 6669 6e65 6420 5461 736b 2047 726f 7570  fined Task Group
+00009030: 206e 616d 6573 2075 7369 6e67 2074 6865   names using the
+00009040: 2060 7b7b 7461 736b 5f67 726f 7570 5f6e   `{{task_group_n
+00009050: 756d 6265 727d 7d60 2076 6172 6961 626c  umber}}` variabl
+00009060: 6520 7375 6273 7469 7475 7469 6f6e 2064  e substitution d
+00009070: 6973 6375 7373 6564 2062 656c 6f77 2e0a  iscussed below..
+00009080: 2d20 2a2a 5461 736b 2a2a 206e 616d 6573  - **Task** names
+00009090: 2061 7265 2061 7574 6f6d 6174 6963 616c   are automatical
+000090a0: 6c79 2063 7265 6174 6564 2066 6f72 2061  ly created for a
+000090b0: 6e79 2054 6173 6b20 7468 6174 2069 7320  ny Task that is 
+000090c0: 6e6f 7420 6578 706c 6963 6974 6c79 206e  not explicitly n
+000090d0: 616d 6564 2c20 7573 696e 6720 6e61 6d65  amed, using name
+000090e0: 7320 6f66 2074 6865 2066 6f72 6d20 6074  s of the form `t
+000090f0: 6173 6b5f 3160 2028 6f72 2060 7461 736b  ask_1` (or `task
+00009100: 5f30 3160 2c20 6574 632e 2c20 666f 7220  _01`, etc., for 
+00009110: 6c61 7267 6572 206e 756d 6265 7273 206f  larger numbers o
+00009120: 6620 5461 736b 7329 2e20 5468 6520 5461  f Tasks). The Ta
+00009130: 736b 2063 6f75 6e74 6572 2072 6573 6574  sk counter reset
+00009140: 7320 666f 7220 6561 6368 2064 6966 6665  s for each diffe
+00009150: 7265 6e74 2054 6173 6b20 4772 6f75 702e  rent Task Group.
+00009160: 2054 6173 6b20 6e75 6d62 6572 7320 6361   Task numbers ca
+00009170: 6e20 616c 736f 2062 6520 696e 636c 7564  n also be includ
+00009180: 6564 2069 6e20 7573 6572 2d64 6566 696e  ed in user-defin
+00009190: 6564 2054 6173 6b20 6e61 6d65 7320 7573  ed Task names us
+000091a0: 696e 6720 7468 6520 607b 7b74 6173 6b5f  ing the `{{task_
+000091b0: 6e75 6d62 6572 7d7d 6020 7661 7269 6162  number}}` variab
+000091c0: 6c65 2073 7562 7374 6974 7574 696f 6e20  le substitution 
+000091d0: 6469 7363 7573 7365 6420 6265 6c6f 772e  discussed below.
+000091e0: 0a0a 2323 2320 5461 736b 2054 7970 6573  ..### Task Types
+000091f0: 0a0a 2d20 4966 2060 7461 736b 5479 7065  ..- If `taskType
+00009200: 6020 6973 2073 6574 206f 6e6c 7920 6174  ` is set only at
+00009210: 2074 6865 2054 4f4d 4c20 6669 6c65 206c   the TOML file l
+00009220: 6576 656c 2c20 7468 656e 2060 7461 736b  evel, then `task
+00009230: 5479 7065 7360 2069 7320 6175 746f 6d61  Types` is automa
+00009240: 7469 6361 6c6c 7920 706f 7075 6c61 7465  tically populate
+00009250: 6420 666f 7220 5461 736b 2047 726f 7570  d for Task Group
+00009260: 732c 2075 6e6c 6573 7320 6f76 6572 7269  s, unless overri
+00009270: 6464 656e 2e0a 2d20 4966 2060 7461 736b  dden..- If `task
+00009280: 5479 7065 6020 6973 2073 6574 2061 7420  Type` is set at 
+00009290: 7468 6520 5461 736b 206c 6576 656c 2c20  the Task level, 
+000092a0: 7468 656e 2060 7461 736b 5479 7065 7360  then `taskTypes`
+000092b0: 2069 7320 6175 746f 6d61 7469 6361 6c6c   is automaticall
+000092c0: 7920 706f 7075 6c61 7465 6420 666f 7220  y populated for 
+000092d0: 7468 6520 5461 736b 2047 726f 7570 7320  the Task Groups 
+000092e0: 6c65 7665 6c20 7573 696e 6720 7468 6520  level using the 
+000092f0: 6163 6375 6d75 6c61 7465 6420 5461 736b  accumulated Task
+00009300: 2054 7970 6573 2066 726f 6d20 7468 6520   Types from the 
+00009310: 5461 736b 7320 696e 636c 7564 6564 2069  Tasks included i
+00009320: 6e20 6561 6368 2054 6173 6b20 4772 6f75  n each Task Grou
+00009330: 702c 2075 6e6c 6573 7320 6f76 6572 7269  p, unless overri
+00009340: 6464 656e 2e0a 2d20 4966 2060 7461 736b  dden..- If `task
+00009350: 5479 7065 7360 2069 7320 7365 7420 6174  Types` is set at
+00009360: 2074 6865 2054 6173 6b20 4772 6f75 7020   the Task Group 
+00009370: 4c65 7665 6c2c 2061 6e64 2068 6173 206f  Level, and has o
+00009380: 6e6c 7920 6f6e 6520 5461 736b 2054 7970  nly one Task Typ
+00009390: 6520 656e 7472 792c 2074 6865 6e20 6074  e entry, then `t
+000093a0: 6173 6b54 7970 6560 2069 7320 6175 746f  askType` is auto
+000093b0: 6d61 7469 6361 6c6c 7920 7365 7420 6174  matically set at
+000093c0: 2074 6865 2054 6173 6b20 4c65 7665 6c20   the Task Level 
+000093d0: 7573 696e 6720 7468 6520 7369 6e67 6c65  using the single
+000093e0: 2054 6173 6b20 5479 7065 2c20 756e 6c65   Task Type, unle
+000093f0: 7373 206f 7665 7272 6964 6465 6e2e 0a0a  ss overridden...
+00009400: 466f 7220 7468 6520 2a2a 6062 6173 6860  For the **`bash`
+00009410: 2a2a 2c20 2a2a 6070 6f77 6572 7368 656c  **, **`powershel
+00009420: 6c60 2a2a 2c20 2a2a 6063 6d64 602a 2a2f  l`**, **`cmd`**/
+00009430: 2a2a 6062 6174 602a 2a20 616e 6420 2a2a  **`bat`** and **
+00009440: 6064 6f63 6b65 7260 2a2a 2074 6173 6b20  `docker`** task 
+00009450: 7479 7065 732c 2073 6f6d 6520 6175 746f  types, some auto
+00009460: 6d61 7469 6320 7072 6f63 6573 7369 6e67  matic processing
+00009470: 2077 696c 6c20 6265 2070 6572 666f 726d   will be perform
+00009480: 6564 2069 6620 7468 6520 2a2a 6065 7865  ed if the **`exe
+00009490: 6375 7461 626c 6560 2a2a 2070 726f 7065  cutable`** prope
+000094a0: 7274 7920 6973 2073 6574 2e0a 0a23 2323  rty is set...###
+000094b0: 2320 4261 7368 2c20 5079 7468 6f6e 2c20  # Bash, Python, 
+000094c0: 506f 7765 7253 6865 6c6c 2061 6e64 2063  PowerShell and c
+000094d0: 6d64 2f62 6174 2054 6173 6b73 0a0a 4173  md/bat Tasks..As
+000094e0: 2061 2063 6f6e 7665 6e69 656e 6365 2c20   a convenience, 
+000094f0: 666f 7220 7468 6520 2a2a 6062 6173 6860  for the **`bash`
+00009500: 2a2a 2c20 2a2a 6070 7974 686f 6e60 2a2a  **, **`python`**
+00009510: 2c20 2a2a 6070 6f77 6572 7368 656c 6c60  , **`powershell`
+00009520: 2a2a 2c20 616e 6420 2a2a 6063 6d64 602a  **, and **`cmd`*
+00009530: 2a20 286f 7220 2a2a 6062 6174 602a 2a29  * (or **`bat`**)
+00009540: 2054 6173 6b20 5479 7065 732c 2074 6865   Task Types, the
+00009550: 2073 6372 6970 7420 6e6f 6d69 6e61 7465   script nominate
+00009560: 6420 696e 2074 6865 202a 2a60 6578 6563  d in the **`exec
+00009570: 7574 6162 6c65 602a 2a20 7072 6f70 6572  utable`** proper
+00009580: 7479 2069 7320 6175 746f 6d61 7469 6361  ty is automatica
+00009590: 6c6c 7920 6164 6465 6420 746f 2074 6865  lly added to the
+000095a0: 2060 696e 7075 7473 6020 6c69 7374 2028   `inputs` list (
+000095b0: 6966 206e 6f74 2061 6c72 6561 6479 2070  if not already p
+000095c0: 7265 7365 6e74 292e 2054 6869 7320 6d65  resent). This me
+000095d0: 616e 7320 7468 6520 7363 7269 7074 2066  ans the script f
+000095e0: 696c 6520 7769 6c6c 2062 6520 7570 6c6f  ile will be uplo
+000095f0: 6164 6564 2074 6f20 7468 6520 4f62 6a65  aded to the Obje
+00009600: 6374 2053 746f 7265 2c20 616e 6420 6d61  ct Store, and ma
+00009610: 6465 2061 2072 6571 7569 7265 6d65 6e74  de a requirement
+00009620: 206f 6620 7468 6520 5461 736b 2077 6865   of the Task whe
+00009630: 6e20 6974 2072 756e 732e 0a0a 5573 696e  n it runs...Usin
+00009640: 6720 6120 4261 7368 2054 6173 6b20 6173  g a Bash Task as
+00009650: 2061 6e20 6578 616d 706c 6520 2869 6e20   an example (in 
+00009660: 544f 4d4c 2066 6f72 6d29 3a0a 0a60 6060  TOML form):..```
+00009670: 746f 6d6c 0a74 6173 6b54 7970 6520 3d20  toml.taskType = 
+00009680: 2262 6173 6822 0a65 7865 6375 7461 626c  "bash".executabl
+00009690: 6520 3d20 226d 795f 6261 7368 5f73 6372  e = "my_bash_scr
+000096a0: 6970 742e 7368 220a 6172 6775 6d65 6e74  ipt.sh".argument
+000096b0: 7320 3d20 5b22 3122 2c20 2232 222c 2022  s = ["1", "2", "
+000096c0: 3322 5d0a 6060 600a 6973 2065 7175 6976  3"].```.is equiv
+000096d0: 616c 656e 7420 746f 3a0a 0a60 6060 746f  alent to:..```to
+000096e0: 6d6c 0a74 6173 6b54 7970 6520 3d20 2262  ml.taskType = "b
+000096f0: 6173 6822 0a69 6e70 7574 7320 3d20 5b22  ash".inputs = ["
+00009700: 6d79 5f62 6173 685f 7363 7269 7074 2e73  my_bash_script.s
+00009710: 6822 5d0a 6172 6775 6d65 6e74 7320 3d20  h"].arguments = 
+00009720: 5b22 7b7b 7772 5f6e 616d 657d 7d2f 6d79  ["{{wr_name}}/my
+00009730: 5f62 6173 685f 7363 7269 7074 2e73 6822  _bash_script.sh"
+00009740: 2c20 2231 222c 2022 3222 2c20 2233 225d  , "1", "2", "3"]
+00009750: 0a60 6060 0a0a 496e 2074 6865 2063 6173  .```..In the cas
+00009760: 6520 6f66 2057 696e 646f 7773 2062 6174  e of Windows bat
+00009770: 6368 2028 602e 6261 7460 2920 6669 6c65  ch (`.bat`) file
+00009780: 732c 2061 2060 2f63 6020 666c 6167 2069  s, a `/c` flag i
+00009790: 7320 7072 6570 656e 6465 6420 746f 2074  s prepended to t
+000097a0: 6865 2060 636d 642e 6578 6560 2061 7267  he `cmd.exe` arg
+000097b0: 756d 656e 7420 6c69 7374 2074 6f20 656e  ument list to en
+000097c0: 7375 7265 2063 6f72 7265 6374 2065 7865  sure correct exe
+000097d0: 6375 7469 6f6e 2062 6168 6176 696f 7572  cution bahaviour
+000097e0: 2e20 466f 7220 6578 616d 706c 653a 0a0a  . For example:..
+000097f0: 6060 6074 6f6d 6c0a 7461 736b 5479 7065  ```toml.taskType
+00009800: 203d 2022 636d 6422 2020 2320 6f72 2022   = "cmd"  # or "
+00009810: 6261 7422 0a65 7865 6375 7461 626c 6520  bat".executable 
+00009820: 3d20 226d 795f 7363 7269 7074 2e62 6174  = "my_script.bat
+00009830: 220a 6172 6775 6d65 6e74 7320 3d20 5b22  ".arguments = ["
+00009840: 3122 2c20 2232 222c 2022 3322 5d0a 6060  1", "2", "3"].``
+00009850: 600a 0a69 7320 6571 7569 7661 6c65 6e74  `..is equivalent
+00009860: 2074 6f3a 0a0a 6060 6074 6f6d 6c0a 7461   to:..```toml.ta
+00009870: 736b 5479 7065 203d 2022 636d 6422 2020  skType = "cmd"  
+00009880: 2320 6f72 2022 6261 7422 0a69 6e70 7574  # or "bat".input
+00009890: 7320 3d20 5b22 6d79 5f73 6372 6970 742e  s = ["my_script.
+000098a0: 6261 7422 5d0a 6172 6775 6d65 6e74 7320  bat"].arguments 
+000098b0: 3d20 5b22 2f63 222c 2022 7b7b 7772 5f6e  = ["/c", "{{wr_n
+000098c0: 616d 657d 7d5c 5c6d 795f 7363 7269 7074  ame}}\\my_script
+000098d0: 2e62 6174 222c 2022 3122 2c20 2232 222c  .bat", "1", "2",
+000098e0: 2022 3322 5d0a 6060 600a 0a4e 6f74 6520   "3"].```..Note 
+000098f0: 7468 6520 605c 5c60 2072 6571 7569 7265  the `\\` require
+00009900: 6d65 6e74 2066 6f72 2064 6972 6563 746f  ment for directo
+00009910: 7279 2073 6570 6172 6174 6f72 7320 7768  ry separators wh
+00009920: 656e 2064 6566 696e 696e 6720 5461 736b  en defining Task
+00009930: 7320 6f6e 2057 696e 646f 7773 2068 6f73  s on Windows hos
+00009940: 7473 2e20 4e6f 7465 2061 6c73 6f20 7468  ts. Note also th
+00009950: 6174 2074 6865 2060 2f63 6020 6973 2072  at the `/c` is r
+00009960: 6571 7569 7265 6420 7768 656e 2072 756e  equired when run
+00009970: 6e69 6e67 2063 6f6d 6d61 6e64 7320 6f72  ning commands or
+00009980: 2062 6174 6368 2073 6372 6970 7473 2075   batch scripts u
+00009990: 7369 6e67 2060 636d 642e 6578 6560 2c20  sing `cmd.exe`, 
+000099a0: 6f74 6865 7277 6973 6520 7468 6520 6063  otherwise the `c
+000099b0: 6d64 2e65 7865 6020 7072 6f63 6573 7320  md.exe` process 
+000099c0: 6372 6561 7465 6420 746f 2065 7865 6375  created to execu
+000099d0: 7465 2074 6865 2054 6173 6b20 7769 6c6c  te the Task will
+000099e0: 206e 6f74 2074 6572 6d69 6e61 7465 2e0a   not terminate..
+000099f0: 0a23 2323 2320 446f 636b 6572 2054 6173  .#### Docker Tas
+00009a00: 6b73 0a0a 466f 7220 7468 6520 2a2a 6064  ks..For the **`d
+00009a10: 6f63 6b65 7260 2a2a 2054 6173 6b20 5479  ocker`** Task Ty
+00009a20: 7065 2c20 7468 6520 7661 7269 6162 6c65  pe, the variable
+00009a30: 7320 7375 7070 6c69 6564 2069 6e20 7468  s supplied in th
+00009a40: 6520 6064 6f63 6b65 7245 6e76 6972 6f6e  e `dockerEnviron
+00009a50: 6d65 6e74 6020 7072 6f70 6572 7479 2061  ment` property a
+00009a60: 7265 2075 6e70 6163 6b65 6420 696e 746f  re unpacked into
+00009a70: 2074 6865 2061 7267 756d 656e 7420 6c69   the argument li
+00009a80: 7374 2061 7320 602d 2d65 6e76 6020 656e  st as `--env` en
+00009a90: 7472 6965 732c 2074 6865 2044 6f63 6b65  tries, the Docke
+00009aa0: 7220 636f 6e74 6169 6e65 7220 6e61 6d65  r container name
+00009ab0: 2073 7570 706c 6965 6420 696e 2074 6865   supplied in the
+00009ac0: 2060 6578 6563 7574 6162 6c65 6020 7072   `executable` pr
+00009ad0: 6f70 6572 7479 2069 7320 7468 656e 2061  operty is then a
+00009ae0: 6464 6564 2074 6f20 7468 6520 6172 6775  dded to the argu
+00009af0: 6d65 6e74 7320 6c69 7374 2c20 666f 6c6c  ments list, foll
+00009b00: 6f77 6564 2062 7920 7468 6520 6172 6775  owed by the argu
+00009b10: 6d65 6e74 7320 7375 7070 6c69 6564 2069  ments supplied i
+00009b20: 6e20 7468 6520 6061 7267 756d 656e 7473  n the `arguments
+00009b30: 6020 7072 6f70 6572 7479 2e20 5468 6520  ` property. The 
+00009b40: 6064 6f63 6b65 7255 7365 726e 616d 6560  `dockerUsername`
+00009b50: 2061 6e64 2060 646f 636b 6572 5061 7373   and `dockerPass
+00009b60: 776f 7264 6020 7072 6f70 6572 7469 6573  word` properties
+00009b70: 2c20 6966 2073 7570 706c 6965 642c 2061  , if supplied, a
+00009b80: 7265 2061 6464 6564 2074 6f20 7468 6520  re added to the 
+00009b90: 6065 6e76 6972 6f6e 6d65 6e74 6020 7072  `environment` pr
+00009ba0: 6f70 6572 7479 2e0a 0a46 6f72 2065 7861  operty...For exa
+00009bb0: 6d70 6c65 3a0a 6060 6074 6f6d 6c0a 7461  mple:.```toml.ta
+00009bc0: 736b 5479 7065 203d 2022 646f 636b 6572  skType = "docker
+00009bd0: 220a 6578 6563 7574 6162 6c65 203d 2022  ".executable = "
+00009be0: 6d79 5f64 6f63 6b65 7268 7562 5f72 6570  my_dockerhub_rep
+00009bf0: 6f2f 6d79 5f63 6f6e 7461 696e 6572 5f69  o/my_container_i
+00009c00: 6d61 6765 220a 646f 636b 6572 456e 7669  mage".dockerEnvi
+00009c10: 726f 6e6d 656e 7420 3d20 7b45 3120 3d20  ronment = {E1 = 
+00009c20: 2245 6565 4f6e 6522 7d0a 646f 636b 6572  "EeeOne"}.docker
+00009c30: 5573 6572 6e61 6d65 203d 2022 6d79 5f75  Username = "my_u
+00009c40: 7365 7222 0a64 6f63 6b65 7250 6173 7377  ser".dockerPassw
+00009c50: 6f72 6420 3d20 226d 795f 7061 7373 776f  ord = "my_passwo
+00009c60: 7264 220a 6172 6775 6d65 6e74 7320 3d20  rd".arguments = 
+00009c70: 5b22 3122 2c20 2232 222c 2022 3322 5d0a  ["1", "2", "3"].
+00009c80: 6060 600a 0a69 7320 6571 7569 7661 6c65  ```..is equivale
+00009c90: 6e74 2074 6f20 7468 6520 666f 6c6c 6f77  nt to the follow
+00009ca0: 696e 6720 6265 696e 6720 7365 6e74 2066  ing being sent f
+00009cb0: 6f72 2070 726f 6365 7373 696e 6720 6279  or processing by
+00009cc0: 2074 6865 2060 646f 636b 6572 6020 5461   the `docker` Ta
+00009cd0: 736b 2054 7970 652c 2074 6865 2059 656c  sk Type, the Yel
+00009ce0: 6c6f 7744 6f67 2076 6572 7369 6f6e 206f  lowDog version o
+00009cf0: 6620 7768 6963 6820 7769 6c6c 206c 6f67  f which will log
+00009d00: 2069 6e20 746f 2074 6865 2044 6f63 6b65   in to the Docke
+00009d10: 7220 7265 706f 2028 6966 2072 6571 7569  r repo (if requi
+00009d20: 7265 6429 2074 6865 6e20 6973 7375 6520  red) then issue 
+00009d30: 6120 6064 6f63 6b65 7220 7275 6e60 2063  a `docker run` c
+00009d40: 6f6d 6d61 6e64 2077 6974 6820 7468 6520  ommand with the 
+00009d50: 6172 6775 6d65 6e74 7320 7375 7070 6c69  arguments suppli
+00009d60: 6564 3a0a 0a60 6060 746f 6d6c 0a74 6173  ed:..```toml.tas
+00009d70: 6b54 7970 6520 3d20 2264 6f63 6b65 7222  kType = "docker"
+00009d80: 0a61 7267 756d 656e 7473 203d 205b 222d  .arguments = ["-
+00009d90: 2d65 6e76 2045 313d 4565 654f 6e65 222c  -env E1=EeeOne",
+00009da0: 2022 6d79 5f64 6f63 6b65 7268 7562 7265   "my_dockerhubre
+00009db0: 706f 2f6d 795f 636f 6e74 6169 6e65 725f  po/my_container_
+00009dc0: 696d 6167 6522 2c20 2231 222c 2022 3222  image", "1", "2"
+00009dd0: 2c20 2233 225d 0a65 6e76 6972 6f6e 6d65  , "3"].environme
+00009de0: 6e74 203d 207b 444f 434b 4552 5f55 5345  nt = {DOCKER_USE
+00009df0: 524e 414d 4520 3d20 226d 795f 7573 6572  RNAME = "my_user
+00009e00: 222c 2044 4f43 4b45 525f 5041 5353 574f  ", DOCKER_PASSWO
+00009e10: 5244 203d 2022 6d79 5f70 6173 7377 6f72  RD = "my_passwor
+00009e20: 6422 7d0a 6060 600a 0a23 2323 2320 4261  d"}.```..#### Ba
+00009e30: 7368 2c20 5079 7468 6f6e 2c20 506f 7765  sh, Python, Powe
+00009e40: 7253 6865 6c6c 2c20 636d 642e 6578 652f  rShell, cmd.exe/
+00009e50: 6261 7463 682c 2061 6e64 2044 6f63 6b65  batch, and Docke
+00009e60: 7220 7769 7468 6f75 7420 4175 746f 6d61  r without Automa
+00009e70: 7469 6320 5072 6f63 6573 7369 6e67 0a0a  tic Processing..
+00009e80: 4966 2074 6865 2060 6578 6563 7574 6162  If the `executab
+00009e90: 6c65 6020 7072 6f70 6572 7479 2069 7320  le` property is 
+00009ea0: 6e6f 7420 7375 7070 6c69 6564 2c20 7468  not supplied, th
+00009eb0: 6520 6175 746f 6d61 7469 6320 7072 6f63  e automatic proc
+00009ec0: 6573 7369 6e67 2064 6573 6372 6962 6564  essing described
+00009ed0: 2061 626f 7665 2066 6f72 2060 6261 7368   above for `bash
+00009ee0: 602c 2060 7079 7468 6f6e 602c 2060 706f  `, `python`, `po
+00009ef0: 7765 7273 6865 6c6c 602c 2060 636d 6460  wershell`, `cmd`
+00009f00: 2028 6f72 2060 6261 7460 2920 616e 6420   (or `bat`) and 
+00009f10: 6064 6f63 6b65 7260 2074 6173 6b20 7479  `docker` task ty
+00009f20: 7065 7320 6973 206e 6f74 2061 7070 6c69  pes is not appli
+00009f30: 6564 2e0a 0a23 2323 2054 6173 6b20 436f  ed...### Task Co
+00009f40: 756e 7473 0a0a 5468 6973 2070 726f 7065  unts..This prope
+00009f50: 7274 7920 7769 6c6c 2065 7870 616e 6420  rty will expand 
+00009f60: 7468 6520 6e75 6d62 6572 206f 6620 5461  the number of Ta
+00009f70: 736b 7320 746f 206d 6174 6368 2060 7461  sks to match `ta
+00009f80: 736b 436f 756e 7460 2e0a 0a54 6865 2060  skCount`...The `
+00009f90: 7461 736b 436f 756e 7460 2070 726f 7065  taskCount` prope
+00009fa0: 7274 7920 6361 6e20 6265 2073 6574 206f  rty can be set o
+00009fb0: 6e6c 7920 696e 2074 6865 2060 776f 726b  nly in the `work
+00009fc0: 5265 7175 6972 656d 656e 7460 2073 6563  Requirement` sec
+00009fd0: 7469 6f6e 206f 6620 7468 6520 6063 6f6e  tion of the `con
+00009fe0: 6669 672e 746f 6d6c 6020 6669 6c65 2c20  fig.toml` file, 
+00009ff0: 6f72 2069 6e20 7468 6520 6074 6173 6b47  or in the `taskG
+0000a000: 726f 7570 6020 7365 6374 696f 6e28 7329  roup` section(s)
+0000a010: 206f 6620 6120 4a53 4f4e 2057 6f72 6b20   of a JSON Work 
+0000a020: 5265 7175 6972 656d 656e 7420 6465 6669  Requirement defi
+0000a030: 6e69 7469 6f6e 2e0a 0a49 6e20 7468 6520  nition...In the 
+0000a040: 666f 726d 6572 2063 6173 652c 2074 6865  former case, the
+0000a050: 2060 7461 736b 436f 756e 7460 2061 7070   `taskCount` app
+0000a060: 6c69 6573 206f 6e6c 7920 746f 2074 6865  lies only to the
+0000a070: 2054 6173 6b20 7370 6563 6966 6965 6420   Task specified 
+0000a080: 7769 7468 696e 2074 6865 2060 636f 6e66  within the `conf
+0000a090: 6967 2e74 6f6d 6c60 2066 696c 6520 616e  ig.toml` file an
+0000a0a0: 6420 6973 206e 6f74 2069 6e68 6572 6974  d is not inherit
+0000a0b0: 6564 2062 7920 4a53 4f4e 2057 6f72 6b20  ed by JSON Work 
+0000a0c0: 5265 7175 6972 656d 656e 7420 7370 6563  Requirement spec
+0000a0d0: 6966 6963 6174 696f 6e73 2e0a 0a49 6e20  ifications...In 
+0000a0e0: 7468 6520 6c61 7474 6572 2063 6173 652c  the latter case,
+0000a0f0: 2074 6865 2060 7461 736b 436f 756e 7460   the `taskCount`
+0000a100: 2061 7070 6c69 6573 2074 6f20 7468 6520   applies to the 
+0000a110: 5461 736b 2073 7065 6369 6669 6564 2077  Task specified w
+0000a120: 6974 6869 6e20 7468 6520 5461 736b 2047  ithin the Task G
+0000a130: 726f 7570 2c20 616e 6420 7468 6572 6520  roup, and there 
+0000a140: 6d75 7374 2062 6520 7a65 726f 206f 7220  must be zero or 
+0000a150: 6f6e 6520 5461 736b 2873 2920 6c69 7374  one Task(s) list
+0000a160: 6564 2077 6974 6869 6e20 7468 6520 6772  ed within the gr
+0000a170: 6f75 7020 6f72 2060 7461 736b 436f 756e  oup or `taskCoun
+0000a180: 7460 2069 7320 6967 6e6f 7265 642e 0a0a  t` is ignored...
+0000a190: 2323 2045 7861 6d70 6c65 730a 0a23 2323  ## Examples..###
+0000a1a0: 2054 4f4d 4c20 5072 6f70 6572 7469 6573   TOML Properties
+0000a1b0: 2069 6e20 7468 6520 6077 6f72 6b52 6571   in the `workReq
+0000a1c0: 7569 7265 6d65 6e74 6020 5365 6374 696f  uirement` Sectio
+0000a1d0: 6e0a 0a48 6572 6527 7320 616e 2065 7861  n..Here's an exa
+0000a1e0: 6d70 6c65 206f 6620 7468 6520 6077 6f72  mple of the `wor
+0000a1f0: 6b52 6571 7569 7265 6d65 6e74 6020 7365  kRequirement` se
+0000a200: 6374 696f 6e20 6f66 2061 2054 4f4d 4c20  ction of a TOML 
+0000a210: 636f 6e66 6967 7572 6174 696f 6e20 6669  configuration fi
+0000a220: 6c65 2c20 7368 6f77 696e 6720 616c 6c20  le, showing all 
+0000a230: 7468 6520 706f 7373 6962 6c65 2070 726f  the possible pro
+0000a240: 7065 7274 6965 7320 7468 6174 2063 616e  perties that can
+0000a250: 2062 6520 7365 743a 0a0a 6060 6074 6f6d   be set:..```tom
+0000a260: 6c0a 5b77 6f72 6b52 6571 7569 7265 6d65  l.[workRequireme
+0000a270: 6e74 5d0a 2020 2020 6172 6775 6d65 6e74  nt].    argument
+0000a280: 7320 3d20 5b22 3122 2c20 2254 574f 225d  s = ["1", "TWO"]
+0000a290: 0a20 2020 2063 6170 7475 7265 5461 736b  .    captureTask
+0000a2a0: 4f75 7470 7574 203d 2074 7275 650a 2020  Output = true.  
+0000a2b0: 2020 636f 6d70 6c65 7465 6454 6173 6b54    completedTaskT
+0000a2c0: 746c 203d 2031 300a 2020 2020 6373 7646  tl = 10.    csvF
+0000a2d0: 696c 6520 3d20 2266 696c 6531 2e63 7376  ile = "file1.csv
+0000a2e0: 220a 2020 2020 6373 7646 696c 6573 203d  ".    csvFiles =
+0000a2f0: 205b 2266 696c 6531 2e63 7376 222c 2022   ["file1.csv", "
+0000a300: 6669 6c65 332e 6373 763a 3322 5d0a 2020  file3.csv:3"].  
+0000a310: 2020 646f 636b 6572 456e 7669 726f 6e6d    dockerEnvironm
+0000a320: 656e 7420 3d20 7b4d 595f 444f 434b 4552  ent = {MY_DOCKER
+0000a330: 5f56 4152 203d 2031 3030 7d0a 2020 2020  _VAR = 100}.    
+0000a340: 646f 636b 6572 5061 7373 776f 7264 203d  dockerPassword =
+0000a350: 2022 6d79 5061 7373 776f 7264 220a 2020   "myPassword".  
+0000a360: 2020 646f 636b 6572 5573 6572 6e61 6d65    dockerUsername
+0000a370: 203d 2022 6d79 5573 6572 6e61 6d65 220a   = "myUsername".
+0000a380: 2020 2020 656e 7669 726f 6e6d 656e 7420      environment 
+0000a390: 3d20 7b4d 595f 5641 5220 3d20 3130 307d  = {MY_VAR = 100}
+0000a3a0: 0a20 2020 2065 7863 6c75 7369 7665 576f  .    exclusiveWo
+0000a3b0: 726b 6572 7320 3d20 6661 6c73 650a 2020  rkers = false.  
+0000a3c0: 2020 6578 6563 7574 6162 6c65 203d 2022    executable = "
+0000a3d0: 6d79 2d63 6f6e 7461 696e 6572 220a 2020  my-container".  
+0000a3e0: 2020 6669 6e69 7368 4966 416c 6c54 6173    finishIfAllTas
+0000a3f0: 6b73 4669 6e69 7368 6564 203d 2074 7275  ksFinished = tru
+0000a400: 650a 2020 2020 6669 6e69 7368 4966 416e  e.    finishIfAn
+0000a410: 7954 6173 6b46 6169 6c65 6420 3d20 6661  yTaskFailed = fa
+0000a420: 6c73 650a 2020 2020 666c 6174 7465 6e49  lse.    flattenI
+0000a430: 6e70 7574 5061 7468 7320 3d20 6661 6c73  nputPaths = fals
+0000a440: 650a 2020 2020 666c 6174 7465 6e55 706c  e.    flattenUpl
+0000a450: 6f61 6450 6174 6873 203d 2066 616c 7365  oadPaths = false
+0000a460: 0a20 2020 2066 756c 6669 6c4f 6e53 7562  .    fulfilOnSub
+0000a470: 6d69 7420 3d20 6661 6c73 650a 2020 2020  mit = false.    
+0000a480: 696e 7075 7473 203d 205b 0a20 2020 2020  inputs = [.     
+0000a490: 2020 2022 2e2e 2f61 7070 2f6d 6169 6e2e     "../app/main.
+0000a4a0: 7079 222c 0a20 2020 2020 2020 2022 2e2e  py",.        "..
+0000a4b0: 2f61 7070 2f72 6571 7569 7265 6d65 6e74  /app/requirement
+0000a4c0: 732e 7478 7422 0a20 2020 205d 0a20 2020  s.txt".    ].   
+0000a4d0: 2069 6e70 7574 734f 7074 696f 6e61 6c20   inputsOptional 
+0000a4e0: 3d20 5b22 6f70 7469 6f6e 616c 2e74 7874  = ["optional.txt
+0000a4f0: 225d 0a20 2020 2069 6e73 7461 6e63 6554  "].    instanceT
+0000a500: 7970 6573 203d 205b 2274 3361 2e6d 6963  ypes = ["t3a.mic
+0000a510: 726f 222c 2022 7433 2e6d 6963 726f 225d  ro", "t3.micro"]
+0000a520: 0a20 2020 206d 6178 576f 726b 6572 7320  .    maxWorkers 
+0000a530: 3d20 310a 2020 2020 6d61 7869 6d75 6d54  = 1.    maximumT
+0000a540: 6173 6b52 6574 7269 6573 203d 2030 0a20  askRetries = 0. 
+0000a550: 2020 206d 696e 576f 726b 6572 7320 3d20     minWorkers = 
+0000a560: 310a 2020 2020 6e61 6d65 203d 2022 6d79  1.    name = "my
+0000a570: 2d77 6f72 6b2d 7265 7175 6972 656d 656e  -work-requiremen
+0000a580: 7422 0a20 2020 206f 7574 7075 7473 203d  t".    outputs =
+0000a590: 205b 2272 6573 756c 7473 2e74 7874 225d   ["results.txt"]
+0000a5a0: 0a20 2020 206f 7574 7075 7473 5265 7175  .    outputsRequ
+0000a5b0: 6972 6564 203d 205b 2272 6573 756c 7473  ired = ["results
+0000a5c0: 5f72 6571 7569 7265 642e 7478 7422 5d0a  _required.txt"].
+0000a5d0: 2020 2020 7072 696f 7269 7479 203d 2030      priority = 0
+0000a5e0: 2e30 0a20 2020 2070 726f 7669 6465 7273  .0.    providers
+0000a5f0: 203d 205b 2241 5753 225d 0a20 2020 2072   = ["AWS"].    r
+0000a600: 616d 203d 205b 302e 352c 2032 2e30 5d0a  am = [0.5, 2.0].
+0000a610: 2020 2020 7265 6769 6f6e 7320 3d20 5b22      regions = ["
+0000a620: 6575 2d77 6573 742d 3222 5d0a 2020 2020  eu-west-2"].    
+0000a630: 7461 736b 4261 7463 6853 697a 6520 3d20  taskBatchSize = 
+0000a640: 3130 3030 0a20 2020 2074 6173 6b43 6f75  1000.    taskCou
+0000a650: 6e74 203d 2031 3030 0a20 2020 2074 6173  nt = 100.    tas
+0000a660: 6b44 6174 6120 3d20 226d 795f 6461 7461  kData = "my_data
+0000a670: 5f73 7472 696e 6722 0a20 2020 2074 6173  _string".    tas
+0000a680: 6b44 6174 6146 696c 6520 3d20 226d 795f  kDataFile = "my_
+0000a690: 6461 7461 5f66 696c 652e 7478 7422 0a20  data_file.txt". 
+0000a6a0: 2020 2074 6173 6b4e 616d 6520 3d20 226d     taskName = "m
+0000a6b0: 795f 7461 736b 5f6e 756d 6265 725f 7b7b  y_task_number_{{
+0000a6c0: 7461 736b 5f6e 756d 6265 727d 7d22 0a20  task_number}}". 
+0000a6d0: 2020 2074 6173 6b47 726f 7570 4e61 6d65     taskGroupName
+0000a6e0: 203d 2022 6d79 5f74 6173 6b5f 6772 6f75   = "my_task_grou
+0000a6f0: 705f 6e75 6d62 6572 5f7b 7b74 6173 6b5f  p_number_{{task_
+0000a700: 6772 6f75 705f 6e75 6d62 6572 7d7d 220a  group_number}}".
+0000a710: 2020 2020 7461 736b 5479 7065 203d 2022      taskType = "
+0000a720: 646f 636b 6572 220a 2020 2020 7461 736b  docker".    task
+0000a730: 7350 6572 576f 726b 6572 203d 2031 0a20  sPerWorker = 1. 
+0000a740: 2020 2075 706c 6f61 6446 696c 6573 203d     uploadFiles =
+0000a750: 205b 7b6c 6f63 616c 5061 7468 203d 2022   [{localPath = "
+0000a760: 6669 6c65 5f31 2e74 7874 222c 2075 706c  file_1.txt", upl
+0000a770: 6f61 6450 6174 6820 3d20 2266 696c 655f  oadPath = "file_
+0000a780: 312e 7478 7422 7d5d 0a20 2020 2076 6370  1.txt"}].    vcp
+0000a790: 7573 203d 205b 312c 2034 5d0a 2020 2020  us = [1, 4].    
+0000a7a0: 7665 7269 6679 4174 5374 6172 7420 3d20  verifyAtStart = 
+0000a7b0: 5b22 7265 6164 795f 7265 7375 6c74 732e  ["ready_results.
+0000a7c0: 7478 7422 5d0a 2020 2020 7665 7269 6679  txt"].    verify
+0000a7d0: 5761 6974 203d 205b 2277 6169 745f 666f  Wait = ["wait_fo
+0000a7e0: 725f 7265 7375 6c74 732e 7478 7422 5d0a  r_results.txt"].
+0000a7f0: 2020 2020 776f 726b 6572 5461 6773 203d      workerTags =
+0000a800: 205b 2274 6167 2d7b 7b75 7365 726e 616d   ["tag-{{usernam
+0000a810: 657d 7d22 5d0a 2020 2020 776f 726b 5265  e}}"].    workRe
+0000a820: 7175 6972 656d 656e 7444 6174 6120 3d20  quirementData = 
+0000a830: 2277 6f72 6b5f 7265 7175 6972 656d 656e  "work_requiremen
+0000a840: 742e 6a73 6f6e 220a 6060 600a 0a23 2323  t.json".```..###
+0000a850: 204a 534f 4e20 5072 6f70 6572 7469 6573   JSON Properties
+0000a860: 2061 7420 7468 6520 576f 726b 2052 6571   at the Work Req
+0000a870: 7569 7265 6d65 6e74 204c 6576 656c 0a0a  uirement Level..
+0000a880: 5368 6f77 696e 6720 616c 6c20 706f 7373  Showing all poss
+0000a890: 6962 6c65 2070 726f 7065 7274 6965 7320  ible properties 
+0000a8a0: 6174 2074 6865 2057 6f72 6b20 5265 7175  at the Work Requ
+0000a8b0: 6972 656d 656e 7420 6c65 7665 6c3a 0a0a  irement level:..
+0000a8c0: 6060 606a 736f 6e0a 7b0a 2020 2261 7267  ```json.{.  "arg
+0000a8d0: 756d 656e 7473 223a 205b 312c 2022 5457  uments": [1, "TW
+0000a8e0: 4f22 5d2c 0a20 2022 6361 7074 7572 6554  O"],.  "captureT
+0000a8f0: 6173 6b4f 7574 7075 7422 3a20 7472 7565  askOutput": true
+0000a900: 2c0a 2020 2263 6f6d 706c 6574 6564 5461  ,.  "completedTa
+0000a910: 736b 5474 6c22 3a20 3130 2c0a 2020 2264  skTtl": 10,.  "d
+0000a920: 6f63 6b65 7245 6e76 6972 6f6e 6d65 6e74  ockerEnvironment
+0000a930: 223a 207b 224d 595f 444f 434b 4552 5f56  ": {"MY_DOCKER_V
+0000a940: 4152 223a 2031 3030 7d2c 0a20 2022 646f  AR": 100},.  "do
+0000a950: 636b 6572 5061 7373 776f 7264 223a 2022  ckerPassword": "
+0000a960: 6d79 5061 7373 776f 7264 222c 0a20 2022  myPassword",.  "
+0000a970: 646f 636b 6572 5573 6572 6e61 6d65 223a  dockerUsername":
+0000a980: 2022 6d79 5573 6572 6e61 6d65 222c 0a20   "myUsername",. 
+0000a990: 2022 656e 7669 726f 6e6d 656e 7422 3a20   "environment": 
+0000a9a0: 7b22 4d59 5f56 4152 223a 2031 3030 7d2c  {"MY_VAR": 100},
+0000a9b0: 0a20 2022 6578 636c 7573 6976 6557 6f72  .  "exclusiveWor
+0000a9c0: 6b65 7273 223a 2066 616c 7365 2c0a 2020  kers": false,.  
+0000a9d0: 2265 7865 6375 7461 626c 6522 3a20 226d  "executable": "m
+0000a9e0: 792d 636f 6e74 6169 6e65 7222 2c0a 2020  y-container",.  
+0000a9f0: 2266 696e 6973 6849 6641 6c6c 5461 736b  "finishIfAllTask
+0000aa00: 7346 696e 6973 6865 6422 3a20 7472 7565  sFinished": true
+0000aa10: 2c0a 2020 2266 696e 6973 6849 6641 6e79  ,.  "finishIfAny
+0000aa20: 5461 736b 4661 696c 6564 223a 2066 616c  TaskFailed": fal
+0000aa30: 7365 2c0a 2020 2266 6c61 7474 656e 496e  se,.  "flattenIn
+0000aa40: 7075 7450 6174 6873 223a 2066 616c 7365  putPaths": false
+0000aa50: 2c0a 2020 2266 6c61 7474 656e 5570 6c6f  ,.  "flattenUplo
+0000aa60: 6164 5061 7468 7322 3a20 6661 6c73 652c  adPaths": false,
+0000aa70: 0a20 2022 6675 6c66 696c 4f6e 5375 626d  .  "fulfilOnSubm
+0000aa80: 6974 223a 2066 616c 7365 2c0a 2020 2269  it": false,.  "i
+0000aa90: 6e70 7574 7322 3a20 5b22 6170 702f 6d61  nputs": ["app/ma
+0000aaa0: 696e 2e70 7922 2c20 2261 7070 2f72 6571  in.py", "app/req
+0000aab0: 7569 7265 6d65 6e74 732e 7478 7422 5d2c  uirements.txt"],
+0000aac0: 0a20 2022 696e 7075 7473 4f70 7469 6f6e  .  "inputsOption
+0000aad0: 616c 223a 205b 226f 7074 696f 6e61 6c2e  al": ["optional.
+0000aae0: 7478 7422 5d2c 0a20 2022 696e 7374 616e  txt"],.  "instan
+0000aaf0: 6365 5479 7065 7322 3a20 5b22 7433 612e  ceTypes": ["t3a.
+0000ab00: 6d69 6372 6f22 2c20 2274 332e 6d69 6372  micro", "t3.micr
+0000ab10: 6f22 5d2c 0a20 2022 6d61 7857 6f72 6b65  o"],.  "maxWorke
+0000ab20: 7273 223a 2031 2c0a 2020 226d 6178 696d  rs": 1,.  "maxim
+0000ab30: 756d 5461 736b 5265 7472 6965 7322 3a20  umTaskRetries": 
+0000ab40: 302c 0a20 2022 6d69 6e57 6f72 6b65 7273  0,.  "minWorkers
+0000ab50: 223a 2031 2c0a 2020 226e 616d 6522 3a20  ": 1,.  "name": 
+0000ab60: 226d 792d 776f 726b 2d72 6571 7569 7265  "my-work-require
+0000ab70: 6d65 6e74 222c 0a20 2022 6f75 7470 7574  ment",.  "output
+0000ab80: 7322 3a20 5b22 7265 7375 6c74 732e 7478  s": ["results.tx
+0000ab90: 7422 5d2c 0a20 2022 6f75 7470 7574 7352  t"],.  "outputsR
+0000aba0: 6571 7569 7265 6422 3a20 5b22 7265 7375  equired": ["resu
+0000abb0: 6c74 735f 7265 7175 6972 6564 2e74 7874  lts_required.txt
+0000abc0: 225d 2c0a 2020 2270 7269 6f72 6974 7922  "],.  "priority"
+0000abd0: 3a20 302e 302c 0a20 2022 7072 6f76 6964  : 0.0,.  "provid
+0000abe0: 6572 7322 3a20 5b22 4157 5322 5d2c 0a20  ers": ["AWS"],. 
+0000abf0: 2022 7261 6d22 3a20 5b30 2e35 2c20 325d   "ram": [0.5, 2]
+0000ac00: 2c0a 2020 2272 6567 696f 6e73 223a 205b  ,.  "regions": [
+0000ac10: 2265 752d 7765 7374 2d32 225d 2c0a 2020  "eu-west-2"],.  
+0000ac20: 2274 6173 6b44 6174 6122 3a20 226d 795f  "taskData": "my_
+0000ac30: 7461 736b 5f64 6174 615f 7374 7269 6e67  task_data_string
+0000ac40: 222c 0a20 2022 7461 736b 4461 7461 4669  ",.  "taskDataFi
+0000ac50: 6c65 223a 2022 6d79 5f64 6174 615f 6669  le": "my_data_fi
+0000ac60: 6c65 2e74 7874 222c 0a20 2022 7461 736b  le.txt",.  "task
+0000ac70: 5479 7065 7322 3a20 5b22 646f 636b 6572  Types": ["docker
+0000ac80: 225d 2c0a 2020 2274 6173 6b73 5065 7257  "],.  "tasksPerW
+0000ac90: 6f72 6b65 7222 3a20 312c 0a20 2022 7570  orker": 1,.  "up
+0000aca0: 6c6f 6164 4669 6c65 7322 3a20 5b7b 226c  loadFiles": [{"l
+0000acb0: 6f63 616c 5061 7468 223a 2022 6669 6c65  ocalPath": "file
+0000acc0: 5f31 2e74 7874 222c 2022 7570 6c6f 6164  _1.txt", "upload
+0000acd0: 5061 7468 223a 2022 6669 6c65 5f31 2e74  Path": "file_1.t
+0000ace0: 7874 227d 5d2c 0a20 2022 7663 7075 7322  xt"}],.  "vcpus"
+0000acf0: 3a20 5b31 2c20 345d 2c0a 2020 2276 6572  : [1, 4],.  "ver
+0000ad00: 6966 7941 7453 7461 7274 223a 205b 2272  ifyAtStart": ["r
+0000ad10: 6561 6479 5f72 6573 756c 7473 2e74 7874  eady_results.txt
+0000ad20: 225d 2c0a 2020 2276 6572 6966 7957 6169  "],.  "verifyWai
+0000ad30: 7422 3a20 5b22 7761 6974 5f66 6f72 5f72  t": ["wait_for_r
+0000ad40: 6573 756c 7473 2e74 7874 225d 2c0a 2020  esults.txt"],.  
+0000ad50: 2277 6f72 6b65 7254 6167 7322 3a20 5b5d  "workerTags": []
+0000ad60: 2c0a 2020 2274 6173 6b47 726f 7570 7322  ,.  "taskGroups"
+0000ad70: 3a20 5b0a 2020 2020 7b0a 2020 2020 2020  : [.    {.      
+0000ad80: 2274 6173 6b73 223a 205b 0a20 2020 2020  "tasks": [.     
+0000ad90: 2020 207b 7d0a 2020 2020 2020 5d0a 2020     {}.      ].  
+0000ada0: 2020 7d0a 2020 5d0a 7d0a 0a60 6060 0a0a    }.  ].}..```..
+0000adb0: 2323 2320 4a53 4f4e 2050 726f 7065 7274  ### JSON Propert
+0000adc0: 6965 7320 6174 2074 6865 2054 6173 6b20  ies at the Task 
+0000add0: 4772 6f75 7020 4c65 7665 6c0a 0a53 686f  Group Level..Sho
+0000ade0: 7769 6e67 2061 6c6c 2070 6f73 7369 626c  wing all possibl
+0000adf0: 6520 7072 6f70 6572 7469 6573 2061 7420  e properties at 
+0000ae00: 7468 6520 5461 736b 2047 726f 7570 206c  the Task Group l
+0000ae10: 6576 656c 3a0a 0a60 6060 6a73 6f6e 0a7b  evel:..```json.{
+0000ae20: 0a20 2022 7461 736b 4772 6f75 7073 223a  .  "taskGroups":
+0000ae30: 205b 0a20 2020 207b 0a20 2020 2020 2022   [.    {.      "
+0000ae40: 6172 6775 6d65 6e74 7322 3a20 5b31 2c20  arguments": [1, 
+0000ae50: 2254 574f 225d 2c0a 2020 2020 2020 2263  "TWO"],.      "c
+0000ae60: 6170 7475 7265 5461 736b 4f75 7470 7574  aptureTaskOutput
+0000ae70: 223a 2074 7275 652c 0a20 2020 2020 2022  ": true,.      "
+0000ae80: 636f 6d70 6c65 7465 6454 6173 6b54 746c  completedTaskTtl
+0000ae90: 223a 2031 302c 0a20 2020 2020 2022 646f  ": 10,.      "do
+0000aea0: 636b 6572 456e 7669 726f 6e6d 656e 7422  ckerEnvironment"
+0000aeb0: 3a20 7b22 4d59 5f44 4f43 4b45 525f 5641  : {"MY_DOCKER_VA
+0000aec0: 5222 3a20 3130 307d 2c0a 2020 2020 2020  R": 100},.      
+0000aed0: 2264 6f63 6b65 7250 6173 7377 6f72 6422  "dockerPassword"
+0000aee0: 3a20 226d 7950 6173 7377 6f72 6422 2c0a  : "myPassword",.
+0000aef0: 2020 2020 2020 2264 6f63 6b65 7255 7365        "dockerUse
+0000af00: 726e 616d 6522 3a20 226d 7955 7365 726e  rname": "myUsern
+0000af10: 616d 6522 2c0a 2020 2020 2020 2265 6e76  ame",.      "env
+0000af20: 6972 6f6e 6d65 6e74 223a 207b 224d 595f  ironment": {"MY_
+0000af30: 5641 5222 3a20 3130 307d 2c0a 2020 2020  VAR": 100},.    
+0000af40: 2020 2265 7863 6c75 7369 7665 576f 726b    "exclusiveWork
+0000af50: 6572 7322 3a20 6661 6c73 652c 0a20 2020  ers": false,.   
+0000af60: 2020 2022 6578 6563 7574 6162 6c65 223a     "executable":
+0000af70: 2022 6d79 2d63 6f6e 7461 696e 6572 222c   "my-container",
+0000af80: 0a20 2020 2020 2022 6669 6e69 7368 4966  .      "finishIf
+0000af90: 416c 6c54 6173 6b73 4669 6e69 7368 6564  AllTasksFinished
+0000afa0: 223a 2074 7275 652c 0a20 2020 2020 2022  ": true,.      "
+0000afb0: 6669 6e69 7368 4966 416e 7954 6173 6b46  finishIfAnyTaskF
+0000afc0: 6169 6c65 6422 3a20 6661 6c73 652c 0a20  ailed": false,. 
+0000afd0: 2020 2020 2022 666c 6174 7465 6e49 6e70       "flattenInp
+0000afe0: 7574 5061 7468 7322 3a20 6661 6c73 652c  utPaths": false,
+0000aff0: 0a20 2020 2020 2022 696e 7075 7473 223a  .      "inputs":
+0000b000: 205b 2261 7070 2f6d 6169 6e2e 7079 222c   ["app/main.py",
+0000b010: 2022 6170 702f 7265 7175 6972 656d 656e   "app/requiremen
+0000b020: 7473 2e74 7874 225d 2c0a 2020 2020 2020  ts.txt"],.      
+0000b030: 2269 6e70 7574 734f 7074 696f 6e61 6c22  "inputsOptional"
+0000b040: 3a20 5b22 6f70 7469 6f6e 616c 2e74 7874  : ["optional.txt
+0000b050: 225d 2c0a 2020 2020 2020 2269 6e73 7461  "],.      "insta
+0000b060: 6e63 6554 7970 6573 223a 205b 2274 3361  nceTypes": ["t3a
+0000b070: 2e6d 6963 726f 222c 2022 7433 2e6d 6963  .micro", "t3.mic
+0000b080: 726f 225d 2c0a 2020 2020 2020 226d 6178  ro"],.      "max
+0000b090: 696d 756d 5461 736b 5265 7472 6965 7322  imumTaskRetries"
+0000b0a0: 3a20 302c 0a20 2020 2020 2022 6d61 7857  : 0,.      "maxW
+0000b0b0: 6f72 6b65 7273 223a 2031 2c0a 2020 2020  orkers": 1,.    
+0000b0c0: 2020 226d 696e 576f 726b 6572 7322 3a20    "minWorkers": 
+0000b0d0: 312c 0a20 2020 2020 2022 6e61 6d65 223a  1,.      "name":
+0000b0e0: 2022 6669 7273 742d 7461 736b 2d67 726f   "first-task-gro
+0000b0f0: 7570 222c 0a20 2020 2020 2022 6f75 7470  up",.      "outp
+0000b100: 7574 7322 3a20 5b22 7265 7375 6c74 732e  uts": ["results.
+0000b110: 7478 7422 5d2c 0a20 2020 2020 2022 6f75  txt"],.      "ou
+0000b120: 7470 7574 7352 6571 7569 7265 6422 3a20  tputsRequired": 
+0000b130: 5b22 7265 7375 6c74 735f 7265 7175 6972  ["results_requir
+0000b140: 6564 2e74 7874 225d 2c0a 2020 2020 2020  ed.txt"],.      
+0000b150: 2270 7269 6f72 6974 7922 3a20 302e 302c  "priority": 0.0,
+0000b160: 0a20 2020 2020 2022 7072 6f76 6964 6572  .      "provider
+0000b170: 7322 3a20 5b22 4157 5322 5d2c 0a20 2020  s": ["AWS"],.   
+0000b180: 2020 2022 7261 6d22 3a20 5b30 2e35 2c20     "ram": [0.5, 
+0000b190: 325d 2c0a 2020 2020 2020 2272 6567 696f  2],.      "regio
+0000b1a0: 6e73 223a 205b 2265 752d 7765 7374 2d32  ns": ["eu-west-2
+0000b1b0: 225d 2c0a 2020 2020 2020 2274 6173 6b43  "],.      "taskC
+0000b1c0: 6f75 6e74 223a 2035 2c0a 2020 2020 2020  ount": 5,.      
+0000b1d0: 2274 6173 6b44 6174 6122 3a20 226d 795f  "taskData": "my_
+0000b1e0: 7461 736b 5f64 6174 615f 7374 7269 6e67  task_data_string
+0000b1f0: 222c 0a20 2020 2020 2022 7461 736b 4461  ",.      "taskDa
+0000b200: 7461 4669 6c65 223a 2022 6d79 5f64 6174  taFile": "my_dat
+0000b210: 615f 6669 6c65 2e74 7874 222c 0a20 2020  a_file.txt",.   
+0000b220: 2020 2022 7461 736b 5479 7065 7322 3a20     "taskTypes": 
+0000b230: 5b22 646f 636b 6572 225d 2c0a 2020 2020  ["docker"],.    
+0000b240: 2020 2274 6173 6b73 5065 7257 6f72 6b65    "tasksPerWorke
+0000b250: 7222 3a20 312c 0a20 2020 2020 2022 7570  r": 1,.      "up
+0000b260: 6c6f 6164 4669 6c65 7322 3a20 5b7b 226c  loadFiles": [{"l
+0000b270: 6f63 616c 5061 7468 223a 2022 6669 6c65  ocalPath": "file
+0000b280: 5f31 2e74 7874 222c 2022 7570 6c6f 6164  _1.txt", "upload
+0000b290: 5061 7468 223a 2022 6669 6c65 5f31 2e74  Path": "file_1.t
+0000b2a0: 7874 227d 5d2c 0a20 2020 2020 2022 7663  xt"}],.      "vc
+0000b2b0: 7075 7322 3a20 5b31 2c20 345d 2c0a 2020  pus": [1, 4],.  
+0000b2c0: 2020 2020 2276 6572 6966 7941 7453 7461      "verifyAtSta
+0000b2d0: 7274 223a 205b 2272 6561 6479 5f72 6573  rt": ["ready_res
+0000b2e0: 756c 7473 2e74 7874 225d 2c0a 2020 2020  ults.txt"],.    
+0000b2f0: 2020 2276 6572 6966 7957 6169 7422 3a20    "verifyWait": 
+0000b300: 5b22 7761 6974 5f66 6f72 5f72 6573 756c  ["wait_for_resul
+0000b310: 7473 2e74 7874 225d 2c0a 2020 2020 2020  ts.txt"],.      
+0000b320: 2277 6f72 6b65 7254 6167 7322 3a20 5b5d  "workerTags": []
+0000b330: 2c0a 2020 2020 2020 2274 6173 6b73 223a  ,.      "tasks":
+0000b340: 205b 0a20 2020 2020 2020 207b 7d0a 2020   [.        {}.  
+0000b350: 2020 2020 5d0a 2020 2020 7d2c 0a20 2020      ].    },.   
+0000b360: 207b 0a20 2020 2020 2022 6e61 6d65 223a   {.      "name":
+0000b370: 2022 7365 636f 6e64 2d74 6173 6b2d 6772   "second-task-gr
+0000b380: 6f75 7022 2c0a 2020 2020 2020 2264 6570  oup",.      "dep
+0000b390: 656e 6465 6e74 4f6e 223a 2022 6669 7273  endentOn": "firs
+0000b3a0: 742d 7461 736b 2d67 726f 7570 222c 0a20  t-task-group",. 
+0000b3b0: 2020 2020 2022 7461 736b 7322 3a20 5b0a       "tasks": [.
+0000b3c0: 2020 2020 2020 2020 7b7d 0a20 2020 2020          {}.     
+0000b3d0: 205d 0a20 2020 207d 0a20 205d 0a7d 0a60   ].    }.  ].}.`
+0000b3e0: 6060 0a0a 2323 2320 4a53 4f4e 2050 726f  ``..### JSON Pro
+0000b3f0: 7065 7274 6965 7320 6174 2074 6865 2054  perties at the T
+0000b400: 6173 6b20 4c65 7665 6c0a 0a53 686f 7769  ask Level..Showi
+0000b410: 6e67 2061 6c6c 2070 6f73 7369 626c 6520  ng all possible 
+0000b420: 7072 6f70 6572 7469 6573 2061 7420 7468  properties at th
+0000b430: 6520 5461 736b 206c 6576 656c 3a0a 0a60  e Task level:..`
+0000b440: 6060 6a73 6f6e 0a7b 0a20 2022 7461 736b  ``json.{.  "task
+0000b450: 4772 6f75 7073 223a 205b 0a20 2020 207b  Groups": [.    {
+0000b460: 0a20 2020 2020 2022 7461 736b 7322 3a20  .      "tasks": 
+0000b470: 5b0a 2020 2020 2020 2020 7b0a 2020 2020  [.        {.    
+0000b480: 2020 2020 2020 2261 7267 756d 656e 7473        "arguments
+0000b490: 223a 205b 312c 2032 5d2c 0a20 2020 2020  ": [1, 2],.     
+0000b4a0: 2020 2020 2022 6361 7074 7572 6554 6173       "captureTas
+0000b4b0: 6b4f 7574 7075 7422 3a20 7472 7565 2c0a  kOutput": true,.
+0000b4c0: 2020 2020 2020 2020 2020 2264 6f63 6b65            "docke
+0000b4d0: 7245 6e76 6972 6f6e 6d65 6e74 223a 207b  rEnvironment": {
+0000b4e0: 224d 595f 444f 434b 4552 5f56 4152 223a  "MY_DOCKER_VAR":
+0000b4f0: 2031 3030 7d2c 0a20 2020 2020 2020 2020   100},.         
+0000b500: 2022 646f 636b 6572 5061 7373 776f 7264   "dockerPassword
+0000b510: 223a 2022 6d79 5061 7373 776f 7264 222c  ": "myPassword",
+0000b520: 0a20 2020 2020 2020 2020 2022 646f 636b  .          "dock
+0000b530: 6572 5573 6572 6e61 6d65 223a 2022 6d79  erUsername": "my
+0000b540: 5573 6572 6e61 6d65 222c 0a20 2020 2020  Username",.     
+0000b550: 2020 2020 2022 656e 7669 726f 6e6d 656e       "environmen
+0000b560: 7422 3a20 7b22 4d59 5f56 4152 223a 2031  t": {"MY_VAR": 1
+0000b570: 3030 7d2c 0a20 2020 2020 2020 2020 2022  00},.          "
+0000b580: 6578 6563 7574 6162 6c65 223a 2022 6d79  executable": "my
+0000b590: 2d63 6f6e 7461 696e 6572 222c 0a20 2020  -container",.   
+0000b5a0: 2020 2020 2020 2022 666c 6174 7465 6e49         "flattenI
+0000b5b0: 6e70 7574 5061 7468 7322 3a20 6661 6c73  nputPaths": fals
+0000b5c0: 652c 0a20 2020 2020 2020 2020 2022 696e  e,.          "in
+0000b5d0: 7075 7473 223a 205b 2261 7070 2f6d 6169  puts": ["app/mai
+0000b5e0: 6e2e 7079 222c 2022 6170 702f 7265 7175  n.py", "app/requ
+0000b5f0: 6972 656d 656e 7473 2e74 7874 225d 2c0a  irements.txt"],.
+0000b600: 2020 2020 2020 2020 2020 2269 6e70 7574            "input
+0000b610: 734f 7074 696f 6e61 6c22 3a20 5b22 6f70  sOptional": ["op
+0000b620: 7469 6f6e 616c 2e74 7874 225d 2c0a 2020  tional.txt"],.  
+0000b630: 2020 2020 2020 2020 226e 616d 6522 3a20          "name": 
+0000b640: 226d 792d 7461 736b 222c 0a20 2020 2020  "my-task",.     
+0000b650: 2020 2020 2022 6f75 7470 7574 7322 3a20       "outputs": 
+0000b660: 5b22 7265 7375 6c74 732e 7478 7422 5d2c  ["results.txt"],
+0000b670: 0a20 2020 2020 2020 2020 2022 6f75 7470  .          "outp
+0000b680: 7574 7352 6571 7569 7265 6422 3a20 5b22  utsRequired": ["
+0000b690: 7265 7375 6c74 735f 7265 7175 6972 6564  results_required
+0000b6a0: 2e74 7874 225d 2c0a 2020 2020 2020 2020  .txt"],.        
+0000b6b0: 2020 2274 6173 6b44 6174 6122 3a20 226d    "taskData": "m
+0000b6c0: 795f 7461 736b 5f64 6174 615f 7374 7269  y_task_data_stri
+0000b6d0: 6e67 222c 0a20 2020 2020 2020 2020 2022  ng",.          "
+0000b6e0: 7461 736b 4461 7461 4669 6c65 223a 2022  taskDataFile": "
+0000b6f0: 6d79 5f64 6174 615f 6669 6c65 2e74 7874  my_data_file.txt
+0000b700: 222c 0a20 2020 2020 2020 2020 2022 7461  ",.          "ta
+0000b710: 736b 5479 7065 223a 2022 646f 636b 6572  skType": "docker
+0000b720: 222c 0a20 2020 2020 2020 2020 2022 7570  ",.          "up
+0000b730: 6c6f 6164 4669 6c65 7322 3a20 5b7b 226c  loadFiles": [{"l
+0000b740: 6f63 616c 5061 7468 223a 2022 6669 6c65  ocalPath": "file
+0000b750: 5f31 2e74 7874 222c 2022 7570 6c6f 6164  _1.txt", "upload
+0000b760: 5061 7468 223a 2022 6669 6c65 5f31 2e74  Path": "file_1.t
+0000b770: 7874 227d 5d2c 0a20 2020 2020 2020 2020  xt"}],.         
+0000b780: 2022 7665 7269 6679 4174 5374 6172 7422   "verifyAtStart"
+0000b790: 3a20 5b22 7265 6164 795f 7265 7375 6c74  : ["ready_result
+0000b7a0: 732e 7478 7422 5d2c 0a20 2020 2020 2020  s.txt"],.       
+0000b7b0: 2020 2022 7665 7269 6679 5761 6974 223a     "verifyWait":
+0000b7c0: 205b 2277 6169 745f 666f 725f 7265 7375   ["wait_for_resu
+0000b7d0: 6c74 732e 7478 7422 5d0a 2020 2020 2020  lts.txt"].      
+0000b7e0: 2020 7d0a 2020 2020 2020 5d0a 2020 2020    }.      ].    
+0000b7f0: 7d0a 2020 5d0a 7d0a 6060 600a 0a23 2320  }.  ].}.```..## 
+0000b800: 5661 7269 6162 6c65 2053 7562 7374 6974  Variable Substit
+0000b810: 7574 696f 6e73 2069 6e20 576f 726b 2052  utions in Work R
+0000b820: 6571 7569 7265 6d65 6e74 2050 726f 7065  equirement Prope
+0000b830: 7274 6965 730a 0a56 6172 6961 626c 6520  rties..Variable 
+0000b840: 7375 6273 7469 7475 7469 6f6e 7320 6361  substitutions ca
+0000b850: 6e20 6265 2075 7365 6420 7769 7468 696e  n be used within
+0000b860: 2061 6e79 2070 726f 7065 7274 7920 7661   any property va
+0000b870: 6c75 6520 696e 2054 4f4d 4c20 636f 6e66  lue in TOML conf
+0000b880: 6967 7572 6174 696f 6e20 6669 6c65 7320  iguration files 
+0000b890: 6f72 2057 6f72 6b20 5265 7175 6972 656d  or Work Requirem
+0000b8a0: 656e 7420 4a53 4f4e 2066 696c 6573 2e20  ent JSON files. 
+0000b8b0: 5365 6520 7468 6520 6465 7363 7269 7074  See the descript
+0000b8c0: 696f 6e20 5b61 626f 7665 5d28 2376 6172  ion [above](#var
+0000b8d0: 6961 626c 652d 7375 6273 7469 7475 7469  iable-substituti
+0000b8e0: 6f6e 7329 2066 6f72 206d 6f72 6520 6465  ons) for more de
+0000b8f0: 7461 696c 7320 6f6e 2076 6172 6961 626c  tails on variabl
+0000b900: 6520 7375 6273 7469 7475 7469 6f6e 732e  e substitutions.
+0000b910: 2054 6869 7320 6973 2061 2070 6f77 6572   This is a power
+0000b920: 6675 6c20 6665 6174 7572 6520 7468 6174  ful feature that
+0000b930: 2061 6c6c 6f77 7320 576f 726b 2052 6571   allows Work Req
+0000b940: 7569 7265 6d65 6e74 7320 746f 2062 6520  uirements to be 
+0000b950: 7061 7261 6d65 7465 7269 7365 6420 6279  parameterised by
+0000b960: 2073 7570 706c 7969 6e67 2076 616c 7565   supplying value
+0000b970: 7320 6f6e 2074 6865 2063 6f6d 6d61 6e64  s on the command
+0000b980: 206c 696e 652c 2076 6961 2065 6e76 6972   line, via envir
+0000b990: 6f6e 6d65 6e74 2076 6172 6961 626c 6573  onment variables
+0000b9a0: 206f 7220 7669 6120 7468 6520 544f 4d4c   or via the TOML
+0000b9b0: 2066 696c 652e 0a0a 2323 2320 5461 736b   file...### Task
+0000b9c0: 2061 6e64 2054 6173 6b20 4772 6f75 7020   and Task Group 
+0000b9d0: 4e61 6d65 2053 7562 7374 6974 7574 696f  Name Substitutio
+0000b9e0: 6e0a 0a54 6865 2066 6f6c 6c6f 7769 6e67  n..The following
+0000b9f0: 206e 756d 6265 7269 6e67 2061 6e64 206e   numbering and n
+0000ba00: 616d 696e 6720 7375 6273 7469 7475 7469  aming substituti
+0000ba10: 6f6e 7320 6172 6520 6176 6169 6c61 626c  ons are availabl
+0000ba20: 6520 666f 7220 7573 6520 696e 2054 6173  e for use in Tas
+0000ba30: 6b20 616e 6420 5461 736b 2047 726f 7570  k and Task Group
+0000ba40: 206e 616d 696e 672c 206f 6e6c 7920 7768   naming, only wh
+0000ba50: 656e 2074 6865 2057 6f72 6b20 5265 7175  en the Work Requ
+0000ba60: 6972 656d 656e 7420 6973 2073 7065 6369  irement is speci
+0000ba70: 6669 6564 2061 7320 204a 534f 4e20 646f  fied as  JSON do
+0000ba80: 6375 6d65 6e74 2c20 692e 652e 2c20 7468  cument, i.e., th
+0000ba90: 6579 2063 616e 2062 6520 7573 6564 2069  ey can be used i
+0000baa0: 6e20 7468 6520 606e 616d 6560 2070 726f  n the `name` pro
+0000bab0: 7065 7274 6965 7320 666f 7220 5461 736b  perties for Task
+0000bac0: 7320 616e 6420 5461 736b 2047 726f 7570  s and Task Group
+0000bad0: 7320 696e 204a 534f 4e20 7370 6563 6966  s in JSON specif
+0000bae0: 6963 6174 696f 6e73 2e0a 0a54 6865 2066  ications...The f
+0000baf0: 6f6c 6c6f 7769 6e67 2074 6162 6c65 2064  ollowing table d
+0000bb00: 6566 696e 6573 2074 6865 2063 6f6e 7465  efines the conte
+0000bb10: 7874 2873 2920 696e 2077 6869 6368 2065  xt(s) in which e
+0000bb20: 6163 6820 7661 7269 6162 6c65 2063 616e  ach variable can
+0000bb30: 2062 6520 7573 6564 3a0a 0a7c 2044 6972   be used:..| Dir
+0000bb40: 6563 7469 7665 2020 2020 2020 2020 2020  ective          
+0000bb50: 2020 2020 207c 2044 6573 6372 6970 7469       | Descripti
+0000bb60: 6f6e 2020 2020 2020 2020 2020 2020 2020  on              
+0000bb70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb80: 2020 2020 2020 2020 207c 2054 6173 6b20           | Task 
+0000bb90: 7c20 5461 736b 2047 726f 7570 207c 0a7c  | Task Group |.|
+0000bba0: 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  :---------------
+0000bbb0: 2d2d 2d2d 2d2d 2d2d 2d7c 3a2d 2d2d 2d2d  ---------|:-----
+0000bbc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000bbd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000bbe0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 3a2d  -------------|:-
+0000bbf0: 2d2d 2d2d 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d  ----|:----------
+0000bc00: 2d7c 0a7c 2060 7b7b 7461 736b 5f6e 756d  -|.| `{{task_num
+0000bc10: 6265 727d 7d60 2020 2020 2020 207c 2054  ber}}`       | T
+0000bc20: 6865 2063 7572 7265 6e74 2054 6173 6b20  he current Task 
+0000bc30: 6e75 6d62 6572 2020 2020 2020 2020 2020  number          
+0000bc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc50: 207c 2059 6573 2020 7c20 2020 2020 2020   | Yes  |       
+0000bc60: 2020 2020 207c 0a7c 2060 7b7b 7461 736b       |.| `{{task
+0000bc70: 5f6e 616d 657d 7d60 2020 2020 2020 2020  _name}}`        
+0000bc80: 207c 2054 6865 2063 7572 7265 6e74 2054   | The current T
+0000bc90: 6173 6b20 6e61 6d65 2020 2020 2020 2020  ask name        
+0000bca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bcb0: 2020 2020 207c 2059 6573 2020 7c20 2020       | Yes  |   
+0000bcc0: 2020 2020 2020 2020 207c 0a7c 2060 7b7b           |.| `{{
+0000bcd0: 7461 736b 5f67 726f 7570 5f6e 616d 657d  task_group_name}
+0000bce0: 7d60 2020 207c 2054 6865 2063 7572 7265  }`   | The curre
+0000bcf0: 6e74 2054 6173 6b20 4772 6f75 7020 6e61  nt Task Group na
+0000bd00: 6d65 2020 2020 2020 2020 2020 2020 2020  me              
+0000bd10: 2020 2020 2020 2020 207c 2059 6573 2020           | Yes  
+0000bd20: 7c20 2020 2020 2020 2020 2020 207c 0a7c  |            |.|
+0000bd30: 2060 7b7b 7461 736b 5f63 6f75 6e74 7d7d   `{{task_count}}
+0000bd40: 6020 2020 2020 2020 207c 2054 6865 206e  `        | The n
+0000bd50: 756d 6265 7220 6f66 2054 6173 6b73 2069  umber of Tasks i
+0000bd60: 6e20 7468 6520 6375 7272 656e 7420 5461  n the current Ta
+0000bd70: 736b 2047 726f 7570 2020 2020 207c 2059  sk Group     | Y
+0000bd80: 6573 2020 7c20 5965 7320 2020 2020 2020  es  | Yes       
+0000bd90: 207c 0a7c 2060 7b7b 7461 736b 5f67 726f   |.| `{{task_gro
+0000bda0: 7570 5f6e 756d 6265 727d 7d60 207c 2054  up_number}}` | T
+0000bdb0: 6865 2063 7572 7265 6e74 2054 6173 6b20  he current Task 
+0000bdc0: 4772 6f75 7020 6e75 6d62 6572 2020 2020  Group number    
+0000bdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bde0: 207c 2059 6573 2020 7c20 5965 7320 2020   | Yes  | Yes   
+0000bdf0: 2020 2020 207c 0a7c 2060 7b7b 7461 736b       |.| `{{task
+0000be00: 5f67 726f 7570 5f63 6f75 6e74 7d7d 6020  _group_count}}` 
+0000be10: 207c 2054 6865 206e 756d 6265 7220 6f66   | The number of
+0000be20: 2054 6173 6b20 4772 6f75 7073 2069 6e20   Task Groups in 
+0000be30: 7468 6520 576f 726b 2052 6571 7569 7265  the Work Require
+0000be40: 6d65 6e74 207c 2059 6573 2020 7c20 5965  ment | Yes  | Ye
+0000be50: 7320 2020 2020 2020 207c 0a0a 496e 2061  s        |..In a
+0000be60: 6464 6974 696f 6e2c 202a 2a54 6173 6b73  ddition, **Tasks
+0000be70: 2a2a 2064 6566 696e 6564 2069 6e20 4a53  ** defined in JS
+0000be80: 4f4e 2064 6f63 756d 656e 7473 2063 616e  ON documents can
+0000be90: 2075 7365 2061 6e79 206f 6620 7468 6520   use any of the 
+0000bea0: 7375 6273 7469 7475 7469 6f6e 7320 6162  substitutions ab
+0000beb0: 6f76 6520 696e 2061 6e79 206f 6620 7468  ove in any of th
+0000bec0: 6569 7220 7072 6f70 6572 7469 6573 2c20  eir properties, 
+0000bed0: 6e6f 7420 6a75 7374 2060 6e61 6d65 602e  not just `name`.
+0000bee0: 0a0a 4e75 6d62 6572 7320 6172 6520 7a65  ..Numbers are ze
+0000bef0: 726f 2d70 6164 6465 6420 666f 7220 6e65  ro-padded for ne
+0000bf00: 6174 2066 6f72 6d61 7474 696e 6720 616e  at formatting an
+0000bf10: 6420 736f 7274 696e 672c 2065 2e67 2e2c  d sorting, e.g.,
+0000bf20: 2054 6173 6b20 6e75 6d62 6572 2060 3337   Task number `37
+0000bf30: 6020 6f66 2060 3130 3030 6020 5461 736b  ` of `1000` Task
+0000bf40: 7320 776f 756c 6420 6265 2073 7562 7374  s would be subst
+0000bf50: 6974 7574 6564 2061 7320 6030 3033 3760  ituted as `0037`
+0000bf60: 2e0a 0a41 7320 616e 2065 7861 6d70 6c65  ...As an example
+0000bf70: 2c20 7468 6520 666f 6c6c 6f77 696e 6720  , the following 
+0000bf80: 4a53 4f4e 2057 6f72 6b20 5265 7175 6972  JSON Work Requir
+0000bf90: 656d 656e 743a 0a0a 6060 606a 736f 6e0a  ement:..```json.
+0000bfa0: 7b0a 2020 2274 6173 6b47 726f 7570 7322  {.  "taskGroups"
+0000bfb0: 3a20 5b0a 2020 2020 7b0a 2020 2020 2020  : [.    {.      
+0000bfc0: 226e 616d 6522 3a20 226d 795f 7461 736b  "name": "my_task
+0000bfd0: 5f67 726f 7570 5f7b 7b74 6173 6b5f 6772  _group_{{task_gr
+0000bfe0: 6f75 705f 6e75 6d62 6572 7d7d 5f61 3122  oup_number}}_a1"
+0000bff0: 2c0a 2020 2020 2020 2265 7865 6375 7461  ,.      "executa
+0000c000: 626c 6522 3a20 2265 7831 2e73 6822 2c0a  ble": "ex1.sh",.
+0000c010: 2020 2020 2020 2274 6173 6b43 6f75 6e74        "taskCount
+0000c020: 223a 2032 2c0a 2020 2020 2020 2274 6173  ": 2,.      "tas
+0000c030: 6b73 223a 205b 0a20 2020 2020 2020 207b  ks": [.        {
+0000c040: 0a20 2020 2020 2020 2020 2022 6e61 6d65  .          "name
+0000c050: 223a 2022 6d79 5f74 6173 6b5f 7b7b 7461  ": "my_task_{{ta
+0000c060: 736b 5f6e 756d 6265 727d 7d2d 6f66 2d7b  sk_number}}-of-{
+0000c070: 7b74 6173 6b5f 636f 756e 747d 7d22 2c0a  {task_count}}",.
+0000c080: 2020 2020 2020 2020 2020 2265 6e76 6972            "envir
+0000c090: 6f6e 6d65 6e74 223a 207b 2254 4153 4b5f  onment": {"TASK_
+0000c0a0: 4e55 4d42 4552 223a 2022 7b7b 7461 736b  NUMBER": "{{task
+0000c0b0: 5f6e 756d 6265 727d 7d22 7d0a 2020 2020  _number}}"}.    
+0000c0c0: 2020 2020 7d0a 2020 2020 2020 5d0a 2020      }.      ].  
+0000c0d0: 2020 7d2c 0a20 2020 207b 0a20 2020 2020    },.    {.     
+0000c0e0: 2022 6e61 6d65 223a 2022 6d79 5f74 6173   "name": "my_tas
+0000c0f0: 6b5f 6772 6f75 705f 7b7b 7461 736b 5f67  k_group_{{task_g
+0000c100: 726f 7570 5f6e 756d 6265 727d 7d5f 6231  roup_number}}_b1
+0000c110: 222c 0a20 2020 2020 2022 6578 6563 7574  ",.      "execut
+0000c120: 6162 6c65 223a 2022 6578 322e 7368 222c  able": "ex2.sh",
+0000c130: 0a20 2020 2020 2022 7461 736b 436f 756e  .      "taskCoun
+0000c140: 7422 3a20 322c 0a20 2020 2020 2022 7461  t": 2,.      "ta
+0000c150: 736b 7322 3a20 5b0a 2020 2020 2020 2020  sks": [.        
+0000c160: 7b0a 2020 2020 2020 2020 2020 226e 616d  {.          "nam
+0000c170: 6522 3a20 226d 795f 7461 736b 5f7b 7b74  e": "my_task_{{t
+0000c180: 6173 6b5f 6e75 6d62 6572 7d7d 2d6f 662d  ask_number}}-of-
+0000c190: 7b7b 7461 736b 5f63 6f75 6e74 7d7d 220a  {{task_count}}".
+0000c1a0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+0000c1b0: 5d0a 2020 2020 7d0a 2020 5d0a 7d0a 6060  ].    }.  ].}.``
+0000c1c0: 600a 0a2e 2e2e 2077 6f75 6c64 2063 7265  `..... would cre
+0000c1d0: 6174 6520 5461 736b 2047 726f 7570 7320  ate Task Groups 
+0000c1e0: 6e61 6d65 6420 606d 795f 7461 736b 5f67  named `my_task_g
+0000c1f0: 726f 7570 5f31 5f61 3160 2061 6e64 2060  roup_1_a1` and `
+0000c200: 6d79 5f74 6173 6b5f 6772 6f75 705f 325f  my_task_group_2_
+0000c210: 6231 602c 2065 6163 6820 636f 6e74 6169  b1`, each contai
+0000c220: 6e69 6e67 2054 6173 6b73 206e 616d 6564  ning Tasks named
+0000c230: 2060 6d79 5f74 6173 6b5f 312d 6f66 2d32   `my_task_1-of-2
+0000c240: 602c 2060 6d79 5f74 6173 6b5f 322d 6f66  `, `my_task_2-of
+0000c250: 2d32 602e 0a0a 2323 2320 576f 726b 2052  -2`...### Work R
+0000c260: 6571 7569 7265 6d65 6e74 204e 616d 6520  equirement Name 
+0000c270: 5375 6273 7469 7475 7469 6f6e 0a0a 5468  Substitution..Th
+0000c280: 6520 6e61 6d65 206f 6620 7468 6520 576f  e name of the Wo
+0000c290: 726b 2052 6571 7569 7265 6d65 6e74 2069  rk Requirement i
+0000c2a0: 7473 656c 6620 6361 6e20 6265 2075 7365  tself can be use
+0000c2b0: 6420 7669 6120 7468 6520 7661 7269 6162  d via the variab
+0000c2c0: 6c65 2073 7562 7374 6974 7574 696f 6e20  le substitution 
+0000c2d0: 607b 7b77 725f 6e61 6d65 7d7d 602e 2054  `{{wr_name}}`. T
+0000c2e0: 6869 7320 6361 6e20 6265 2075 7365 6420  his can be used 
+0000c2f0: 616e 7977 6865 7265 2069 6e20 6120 544f  anywhere in a TO
+0000c300: 4d4c 2063 6f6e 6669 6775 7261 7469 6f6e  ML configuration
+0000c310: 2066 696c 6520 6f72 2069 6e20 6120 4a53   file or in a JS
+0000c320: 4f4e 2057 6f72 6b20 5265 7175 6972 656d  ON Work Requirem
+0000c330: 656e 742e 0a0a 2323 2044 7279 2d52 756e  ent...## Dry-Run
+0000c340: 6e69 6e67 2057 6f72 6b20 5265 7175 6972  ning Work Requir
+0000c350: 656d 656e 7420 5375 626d 6973 7369 6f6e  ement Submission
+0000c360: 730a 0a54 6f20 6578 616d 696e 6520 7468  s..To examine th
+0000c370: 6520 4a53 4f4e 2074 6861 7420 7769 6c6c  e JSON that will
+0000c380: 2061 6374 7561 6c6c 7920 6265 2073 656e   actually be sen
+0000c390: 7420 746f 2074 6865 2059 656c 6c6f 7744  t to the YellowD
+0000c3a0: 6f67 2041 5049 2061 6674 6572 2061 6c6c  og API after all
+0000c3b0: 2070 726f 6365 7373 696e 672c 2075 7365   processing, use
+0000c3c0: 2074 6865 2060 2d2d 6472 792d 7275 6e60   the `--dry-run`
+0000c3d0: 2063 6f6d 6d61 6e64 206c 696e 6520 6f70   command line op
+0000c3e0: 7469 6f6e 2077 6865 6e20 7275 6e6e 696e  tion when runnin
+0000c3f0: 6720 6079 642d 7375 626d 6974 602e 2054  g `yd-submit`. T
+0000c400: 6869 7320 7769 6c6c 2070 7269 6e74 2074  his will print t
+0000c410: 6865 2066 756c 6c79 2070 726f 6365 7373  he fully process
+0000c420: 6564 204a 534f 4e20 666f 7220 7468 6520  ed JSON for the 
+0000c430: 576f 726b 2052 6571 7569 7265 6d65 6e74  Work Requirement
+0000c440: 2e20 4e6f 7468 696e 6720 7769 6c6c 2062  . Nothing will b
+0000c450: 6520 7375 626d 6974 7465 6420 746f 2074  e submitted to t
+0000c460: 6865 2050 6c61 7466 6f72 6d2e 0a0a 5468  he Platform...Th
+0000c470: 6520 6472 792d 7275 6e20 6973 2075 7365  e dry-run is use
+0000c480: 6675 6c20 666f 7220 696e 7370 6563 7469  ful for inspecti
+0000c490: 6e67 2074 6865 2072 6573 756c 7473 206f  ng the results o
+0000c4a0: 6620 616c 6c20 7468 6520 7072 6f63 6573  f all the proces
+0000c4b0: 7369 6e67 2074 6861 7427 7320 6265 656e  sing that's been
+0000c4c0: 2070 6572 666f 726d 6564 2e20 546f 2073   performed. To s
+0000c4d0: 7570 7072 6573 7320 616c 6c20 6f75 7470  uppress all outp
+0000c4e0: 7574 2065 7863 6570 7420 666f 7220 7468  ut except for th
+0000c4f0: 6520 4a53 4f4e 2069 7473 656c 662c 2075  e JSON itself, u
+0000c500: 7365 2074 6865 2060 2d2d 7175 6965 7460  se the `--quiet`
+0000c510: 2028 602d 7160 2920 636f 6d6d 616e 6420   (`-q`) command 
+0000c520: 6c69 6e65 206f 7074 696f 6e2e 0a0a 4e6f  line option...No
+0000c530: 7465 2074 6861 7420 7468 6520 6765 6e65  te that the gene
+0000c540: 7261 7465 6420 4a53 4f4e 2069 7320 6120  rated JSON is a 
+0000c550: 636f 6e73 6f6c 6964 6174 6564 2066 6f72  consolidated for
+0000c560: 6d20 6f66 2077 6861 7420 776f 756c 6420  m of what would 
+0000c570: 6265 2073 7562 6d69 7474 6564 2074 6f20  be submitted to 
+0000c580: 7468 6520 5965 6c6c 6f77 446f 6720 4150  the YellowDog AP
+0000c590: 492c 2061 6e64 2054 6173 6b73 2061 7265  I, and Tasks are
+0000c5a0: 2064 6566 696e 6564 2064 6972 6563 746c   defined directl
+0000c5b0: 7920 7769 7468 696e 2074 6865 6972 2054  y within their T
+0000c5c0: 6173 6b20 4772 6f75 7073 2066 6f72 2065  ask Groups for e
+0000c5d0: 6173 6520 6f66 2063 6f6d 7072 6568 656e  ase of comprehen
+0000c5e0: 7369 6f6e 2e20 496e 2061 6374 7561 6c20  sion. In actual 
+0000c5f0: 4150 4920 7375 626d 6973 7369 6f6e 732c  API submissions,
+0000c600: 2074 6865 2057 6f72 6b20 5265 7175 6972   the Work Requir
+0000c610: 656d 656e 7420 7769 7468 2069 7473 2054  ement with its T
+0000c620: 6173 6b20 4772 6f75 7073 2069 7320 7375  ask Groups is su
+0000c630: 626d 6974 7465 6420 6669 7273 742c 2061  bmitted first, a
+0000c640: 6e64 2054 6173 6b73 2061 7265 2074 6865  nd Tasks are the
+0000c650: 6e20 6164 6465 6420 746f 2054 6173 6b20  n added to Task 
+0000c660: 4772 6f75 7073 2073 6570 6172 6174 656c  Groups separatel
+0000c670: 7920 696e 2073 7562 7365 7175 656e 7420  y in subsequent 
+0000c680: 4150 4920 6361 6c6c 732e 0a0a 4120 7369  API calls...A si
+0000c690: 6d70 6c65 2065 7861 6d70 6c65 206f 6620  mple example of 
+0000c6a0: 7468 6520 4a53 4f4e 206f 7574 7075 7420  the JSON output 
+0000c6b0: 6973 2073 686f 776e 2062 656c 6f77 2c20  is shown below, 
+0000c6c0: 7368 6f77 696e 6720 6120 576f 726b 2052  showing a Work R
+0000c6d0: 6571 7569 7265 6d65 6e74 2077 6974 6820  equirement with 
+0000c6e0: 6120 7369 6e67 6c65 2054 6173 6b20 4772  a single Task Gr
+0000c6f0: 6f75 702c 2063 6f6e 7461 696e 696e 6720  oup, containing 
+0000c700: 6120 7369 6e67 6c65 2054 6173 6b2e 0a0a  a single Task...
+0000c710: 6025 2079 642d 7375 626d 6974 202d 2d64  `% yd-submit --d
+0000c720: 7279 2d72 756e 202d 2d71 7569 6574 600a  ry-run --quiet`.
+0000c730: 6060 606a 736f 6e0a 7b0a 2020 2266 756c  ```json.{.  "ful
+0000c740: 6669 6c4f 6e53 7562 6d69 7422 3a20 6661  filOnSubmit": fa
+0000c750: 6c73 652c 0a20 2022 6e61 6d65 223a 2022  lse,.  "name": "
+0000c760: 7079 6578 2d62 6173 685f 3233 3031 3134  pyex-bash_230114
+0000c770: 2d30 3935 3530 342d 3533 6122 2c0a 2020  -095504-53a",.  
+0000c780: 226e 616d 6573 7061 6365 223a 2022 7079  "namespace": "py
+0000c790: 6578 616d 706c 6573 222c 0a20 2022 7072  examples",.  "pr
+0000c7a0: 696f 7269 7479 223a 2030 2c0a 2020 2274  iority": 0,.  "t
+0000c7b0: 6167 223a 2022 7079 6578 2d62 6173 6822  ag": "pyex-bash"
+0000c7c0: 2c0a 2020 2274 6173 6b47 726f 7570 7322  ,.  "taskGroups"
+0000c7d0: 3a20 5b0a 2020 2020 7b0a 2020 2020 2020  : [.    {.      
+0000c7e0: 2266 696e 6973 6849 6641 6c6c 5461 736b  "finishIfAllTask
+0000c7f0: 7346 696e 6973 6865 6422 3a20 7472 7565  sFinished": true
+0000c800: 2c0a 2020 2020 2020 2266 696e 6973 6849  ,.      "finishI
+0000c810: 6641 6e79 5461 736b 4661 696c 6564 223a  fAnyTaskFailed":
+0000c820: 2066 616c 7365 2c0a 2020 2020 2020 226e   false,.      "n
+0000c830: 616d 6522 3a20 2274 6173 6b5f 6772 6f75  ame": "task_grou
+0000c840: 705f 3122 2c0a 2020 2020 2020 2270 7269  p_1",.      "pri
+0000c850: 6f72 6974 7922 3a20 302c 0a20 2020 2020  ority": 0,.     
+0000c860: 2022 7275 6e53 7065 6369 6669 6361 7469   "runSpecificati
+0000c870: 6f6e 223a 207b 0a20 2020 2020 2020 2022  on": {.        "
+0000c880: 6d61 7869 6d75 6d54 6173 6b52 6574 7269  maximumTaskRetri
+0000c890: 6573 223a 2030 2c0a 2020 2020 2020 2020  es": 0,.        
+0000c8a0: 2274 6173 6b54 7970 6573 223a 205b 2262  "taskTypes": ["b
+0000c8b0: 6173 6822 5d2c 0a20 2020 2020 2020 2022  ash"],.        "
+0000c8c0: 776f 726b 6572 5461 6773 223a 205b 2270  workerTags": ["p
+0000c8d0: 7965 782d 6261 7368 225d 0a20 2020 2020  yex-bash"].     
+0000c8e0: 207d 2c0a 2020 2020 2020 2274 6173 6b73   },.      "tasks
+0000c8f0: 223a 205b 0a20 2020 2020 2020 207b 0a20  ": [.        {. 
+0000c900: 2020 2020 2020 2020 2022 6172 6775 6d65           "argume
+0000c910: 6e74 7322 3a20 5b22 7079 6578 2d62 6173  nts": ["pyex-bas
+0000c920: 685f 3233 3031 3134 2d30 3935 3530 342d  h_230114-095504-
+0000c930: 3533 612f 736c 6565 705f 7363 7269 7074  53a/sleep_script
+0000c940: 2e73 6822 5d2c 0a20 2020 2020 2020 2020  .sh"],.         
+0000c950: 2022 656e 7669 726f 6e6d 656e 7422 3a20   "environment": 
+0000c960: 7b7d 2c0a 2020 2020 2020 2020 2020 2269  {},.          "i
+0000c970: 6e70 7574 7322 3a20 5b0a 2020 2020 2020  nputs": [.      
+0000c980: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+0000c990: 2020 2020 2020 226f 626a 6563 744e 616d        "objectNam
+0000c9a0: 6550 6174 7465 726e 223a 2022 7079 6578  ePattern": "pyex
+0000c9b0: 2d62 6173 685f 3233 3031 3134 2d30 3935  -bash_230114-095
+0000c9c0: 3530 342d 3533 612f 736c 6565 705f 7363  504-53a/sleep_sc
+0000c9d0: 7269 7074 2e73 6822 2c0a 2020 2020 2020  ript.sh",.      
+0000c9e0: 2020 2020 2020 2020 2273 6f75 7263 6522          "source"
+0000c9f0: 3a20 2254 4153 4b5f 4e41 4d45 5350 4143  : "TASK_NAMESPAC
+0000ca00: 4522 2c0a 2020 2020 2020 2020 2020 2020  E",.            
+0000ca10: 2020 2276 6572 6966 6963 6174 696f 6e22    "verification"
+0000ca20: 3a20 2256 4552 4946 595f 5741 4954 220a  : "VERIFY_WAIT".
+0000ca30: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+0000ca40: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
+0000ca50: 2020 2020 2022 6e61 6d65 223a 2022 7461       "name": "ta
+0000ca60: 736b 5f30 3122 2c0a 2020 2020 2020 2020  sk_01",.        
+0000ca70: 2020 226f 7574 7075 7473 223a 205b 0a20    "outputs": [. 
+0000ca80: 2020 2020 2020 2020 2020 207b 2261 6c77             {"alw
+0000ca90: 6179 7355 706c 6f61 6422 3a20 7472 7565  aysUpload": true
+0000caa0: 2c20 2272 6571 7569 7265 6422 3a20 6661  , "required": fa
+0000cab0: 6c73 652c 2022 736f 7572 6365 223a 2022  lse, "source": "
+0000cac0: 5052 4f43 4553 535f 4f55 5450 5554 227d  PROCESS_OUTPUT"}
+0000cad0: 0a20 2020 2020 2020 2020 205d 2c0a 2020  .          ],.  
+0000cae0: 2020 2020 2020 2020 2274 6173 6b54 7970          "taskTyp
+0000caf0: 6522 3a20 2262 6173 6822 0a20 2020 2020  e": "bash".     
+0000cb00: 2020 207d 0a20 2020 2020 205d 0a20 2020     }.      ].   
+0000cb10: 207d 0a20 205d 0a7d 0a60 6060 0a0a 2323   }.  ].}.```..##
+0000cb20: 2320 5375 626d 6974 7469 6e67 2027 5261  # Submitting 'Ra
+0000cb30: 7727 204a 534f 4e20 576f 726b 2052 6571  w' JSON Work Req
+0000cb40: 7569 7265 6d65 6e74 2053 7065 6369 6669  uirement Specifi
+0000cb50: 6361 7469 6f6e 730a 0a49 7427 7320 706f  cations..It's po
+0000cb60: 7373 6962 6c65 2074 6f20 7573 6520 7468  ssible to use th
+0000cb70: 6520 4a53 4f4e 206f 7574 7075 7420 6f66  e JSON output of
+0000cb80: 2060 7964 2d73 7562 6d69 7420 2d2d 6472   `yd-submit --dr
+0000cb90: 792d 7275 6e60 2028 7375 6368 2061 7320  y-run` (such as 
+0000cba0: 7468 6520 6578 616d 706c 6520 6162 6f76  the example abov
+0000cbb0: 6529 2061 7320 6120 7365 6c66 2d63 6f6e  e) as a self-con
+0000cbc0: 7461 696e 6564 2c20 6675 6c6c 792d 7370  tained, fully-sp
+0000cbd0: 6563 6966 6965 6420 576f 726b 2052 6571  ecified Work Req
+0000cbe0: 7569 7265 6d65 6e74 2073 7065 6369 6669  uirement specifi
+0000cbf0: 6361 7469 6f6e 2c20 7573 696e 6720 7468  cation, using th
+0000cc00: 6520 602d 2d6a 736f 6e2d 7261 7760 2028  e `--json-raw` (
+0000cc10: 6f72 2060 2d6a 6029 2063 6f6d 6d61 6e64  or `-j`) command
+0000cc20: 206c 696e 6520 6f70 7469 6f6e 2c20 692e   line option, i.
+0000cc30: 652e 3a20 6079 642d 7375 626d 6974 202d  e.: `yd-submit -
+0000cc40: 2d6a 736f 6e2d 7261 7720 3c66 696c 656e  -json-raw <filen
+0000cc50: 616d 652e 6a73 6f6e 3e60 2e0a 0a54 6869  ame.json>`...Thi
+0000cc60: 7320 7769 6c6c 2073 7562 6d69 7420 7468  s will submit th
+0000cc70: 6520 576f 726b 2052 6571 7569 7265 6d65  e Work Requireme
+0000cc80: 6e74 2c20 7468 656e 2061 6464 2061 6c6c  nt, then add all
+0000cc90: 2074 6865 2073 7065 6369 6669 6564 2054   the specified T
+0000cca0: 6173 6b73 2e0a 0a4e 6f74 6520 7468 6174  asks...Note that
+0000ccb0: 2076 6172 6961 626c 6520 7375 6273 7469   variable substi
+0000ccc0: 7475 7469 6f6e 7320 2a2a 6361 6e2a 2a20  tutions **can** 
+0000ccd0: 6265 2075 7365 6420 696e 2074 6865 2072  be used in the r
+0000cce0: 6177 204a 534f 4e20 6669 6c65 2c20 6a75  aw JSON file, ju
+0000ccf0: 7374 2061 7320 696e 2074 6865 206f 7468  st as in the oth
+0000cd00: 6572 2057 6f72 6b20 5265 7175 6972 656d  er Work Requirem
+0000cd10: 656e 7420 4a53 4f4e 2065 7861 6d70 6c65  ent JSON example
+0000cd20: 732c 2062 7574 2074 6865 7265 2069 7320  s, but there is 
+0000cd30: 6e6f 2070 726f 7065 7274 7920 696e 6865  no property inhe
+0000cd40: 7269 7461 6e63 652c 2069 6e63 6c75 6469  ritance, includi
+0000cd50: 6e67 2066 726f 6d20 7468 6520 605b 776f  ng from the `[wo
+0000cd60: 726b 5265 7175 6972 656d 656e 745d 6020  rkRequirement]` 
+0000cd70: 7365 6374 696f 6e20 6f66 2074 6865 2054  section of the T
+0000cd80: 4f4d 4c20 636f 6e66 6967 7572 6174 696f  OML configuratio
+0000cd90: 6e20 6f72 2066 726f 6d20 576f 726b 2052  n or from Work R
+0000cda0: 6571 7569 7265 6d65 6e74 2070 726f 7065  equirement prope
+0000cdb0: 7274 6965 7320 7375 7070 6c69 6564 206f  rties supplied o
+0000cdc0: 6e20 7468 6520 636f 6d6d 616e 6420 6c69  n the command li
+0000cdd0: 6e65 2e0a 0a4e 6f74 6520 7468 6174 2074  ne...Note that t
+0000cde0: 6865 7265 2069 7320 6e6f 2061 7574 6f6d  here is no autom
+0000cdf0: 6174 6963 2066 696c 6520 7570 6c6f 6164  atic file upload
+0000ce00: 2077 6865 6e20 7573 696e 6720 7468 6973   when using this
+0000ce10: 206f 7074 696f 6e2c 2073 6f20 616e 7920   option, so any 
+0000ce20: 6669 6c65 7320 7265 7175 6972 6564 2061  files required a
+0000ce30: 7420 7468 6520 7374 6172 7420 6f66 2074  t the start of t
+0000ce40: 6865 2074 6173 6b20 2873 7065 6369 6669  he task (specifi
+0000ce50: 6564 2075 7369 6e67 2060 5645 5249 4659  ed using `VERIFY
+0000ce60: 5f41 545f 5354 4152 5460 2920 6d75 7374  _AT_START`) must
+0000ce70: 2062 6520 7072 6573 656e 7420 6265 666f   be present befo
+0000ce80: 7265 2074 6865 2054 6173 6b73 2061 7265  re the Tasks are
+0000ce90: 2075 706c 6f61 6465 642c 206f 7220 7468   uploaded, or th
+0000cea0: 6520 5461 736b 7320 7769 6c6c 2066 6169  e Tasks will fai
+0000ceb0: 6c20 696d 6d65 6469 6174 656c 792e 2054  l immediately. T
+0000cec0: 6865 2060 7964 2d75 706c 6f61 6460 2063  he `yd-upload` c
+0000ced0: 6f6d 6d61 6e64 2063 616e 2062 6520 7573  ommand can be us
+0000cee0: 6564 2074 6f20 7570 6c6f 6164 2074 6865  ed to upload the
+0000cef0: 7365 2066 696c 6573 2c20 616e 6420 6079  se files, and `y
+0000cf00: 642d 7375 626d 6974 6020 7769 6c6c 2070  d-submit` will p
+0000cf10: 6175 7365 2074 6f20 616c 6c6f 7720 7468  ause to allow th
+0000cf20: 6973 2074 6f20 6861 7070 656e 2e0a 0a23  is to happen...#
+0000cf30: 2320 4669 6c65 2053 746f 7261 6765 204c  # File Storage L
+0000cf40: 6f63 6174 696f 6e73 2061 6e64 2046 696c  ocations and Fil
+0000cf50: 6520 5573 6167 650a 0a54 6869 7320 7365  e Usage..This se
+0000cf60: 6374 696f 6e20 6469 7363 7573 7365 7320  ction discusses 
+0000cf70: 686f 7720 746f 2075 706c 6f61 6420 6669  how to upload fi
+0000cf80: 6c65 7320 6672 6f6d 206c 6f63 616c 2073  les from local s
+0000cf90: 746f 7261 6765 2074 6f20 7468 6520 5965  torage to the Ye
+0000cfa0: 6c6c 6f77 446f 6720 4f62 6a65 6374 2053  llowDog Object S
+0000cfb0: 746f 7265 2c20 686f 7720 7468 6f73 6520  tore, how those 
+0000cfc0: 6669 6c65 7320 6172 6520 7472 616e 7366  files are transf
+0000cfd0: 6572 7265 6420 746f 2057 6f72 6b65 7220  erred to Worker 
+0000cfe0: 4e6f 6465 7320 666f 7220 5461 736b 2070  Nodes for Task p
+0000cff0: 726f 6365 7373 696e 672c 2068 6f77 2074  rocessing, how t
+0000d000: 6865 2072 6573 756c 7473 206f 6620 5461  he results of Ta
+0000d010: 736b 2070 726f 6365 7373 696e 6720 6172  sk processing ar
+0000d020: 6520 7265 7475 726e 6564 2062 7920 576f  e returned by Wo
+0000d030: 726b 6572 204e 6f64 6573 2c20 616e 6420  rker Nodes, and 
+0000d040: 686f 7720 6669 6c65 7320 6172 6520 7472  how files are tr
+0000d050: 616e 7366 6572 7265 6420 6261 636b 2066  ansferred back f
+0000d060: 726f 6d20 7468 6520 5965 6c6c 6f77 446f  rom the YellowDo
+0000d070: 6720 4f62 6a65 6374 2053 746f 7265 2074  g Object Store t
+0000d080: 6f20 6c6f 6361 6c20 7374 6f72 6167 652e  o local storage.
+0000d090: 0a0a 2323 2320 4669 6c65 7320 5570 6c6f  ..### Files Uplo
+0000d0a0: 6164 6564 2074 6f20 7468 6520 4f62 6a65  aded to the Obje
+0000d0b0: 6374 2053 746f 7265 2066 726f 6d20 4c6f  ct Store from Lo
+0000d0c0: 6361 6c20 5374 6f72 6167 650a 0a23 2323  cal Storage..###
+0000d0d0: 2320 4669 6c65 7320 696e 2074 6865 2060  # Files in the `
+0000d0e0: 696e 7075 7473 6020 4c69 7374 0a0a 5768  inputs` List..Wh
+0000d0f0: 656e 2061 2057 6f72 6b20 5265 7175 6972  en a Work Requir
+0000d100: 656d 656e 7420 6973 2073 7562 6d69 7474  ement is submitt
+0000d110: 6564 2075 7369 6e67 2060 7964 2d73 7562  ed using `yd-sub
+0000d120: 6d69 7460 2c20 6669 6c65 7320 6172 6520  mit`, files are 
+0000d130: 7570 6c6f 6164 6564 2074 6f20 7468 6520  uploaded to the 
+0000d140: 5965 6c6c 6f77 446f 6720 4f62 6a65 6374  YellowDog Object
+0000d150: 2053 746f 7265 2069 6620 7468 6579 2772   Store if they'r
+0000d160: 6520 696e 636c 7564 6564 2069 6e20 7468  e included in th
+0000d170: 6520 6c69 7374 206f 6620 6669 6c65 7320  e list of files 
+0000d180: 696e 2074 6865 2060 696e 7075 7473 6020  in the `inputs` 
+0000d190: 7072 6f70 6572 7479 2e20 2846 6f72 2074  property. (For t
+0000d1a0: 6865 2063 6173 6520 6f66 2074 6865 2060  he case of the `
+0000d1b0: 6261 7368 6020 5461 736b 2054 7970 652c  bash` Task Type,
+0000d1c0: 2074 6865 2073 6372 6970 7420 7370 6563   the script spec
+0000d1d0: 6966 6965 6420 696e 2074 6865 2060 6578  ified in the `ex
+0000d1e0: 6563 7574 6162 6c65 6020 7072 6f70 6572  ecutable` proper
+0000d1f0: 7479 2069 7320 616c 736f 2061 7574 6f6d  ty is also autom
+0000d200: 6174 6963 616c 6c79 2075 706c 6f61 6465  atically uploade
+0000d210: 6420 6173 2061 2063 6f6e 7665 6e69 656e  d as a convenien
+0000d220: 6365 2c20 6576 656e 2069 6620 6e6f 7420  ce, even if not 
+0000d230: 696e 636c 7564 6564 2069 6e20 7468 6520  included in the 
+0000d240: 6069 6e70 7574 7360 206c 6973 742e 290a  `inputs` list.).
+0000d250: 0a46 696c 6573 2061 7265 2075 706c 6f61  .Files are uploa
+0000d260: 6465 6420 746f 2074 6865 204e 616d 6573  ded to the Names
+0000d270: 7061 6365 2073 7065 6369 6669 6564 2069  pace specified i
+0000d280: 6e20 7468 6520 636f 6e66 6967 7572 6174  n the configurat
+0000d290: 696f 6e2e 2057 6974 6869 6e20 7468 6520  ion. Within the 
+0000d2a0: 4e61 6d65 7370 6163 652c 2065 6163 6820  Namespace, each 
+0000d2b0: 576f 726b 2052 6571 7569 7265 6d65 6e74  Work Requirement
+0000d2c0: 2068 6173 2061 2073 6570 6172 6174 6520   has a separate 
+0000d2d0: 666f 6c64 6572 2074 6861 7420 7368 6172  folder that shar
+0000d2e0: 6573 2074 6865 206e 616d 6520 6f66 2074  es the name of t
+0000d2f0: 6865 2057 6f72 6b20 5265 7175 6972 656d  he Work Requirem
+0000d300: 656e 742c 2061 6e64 2069 6e20 7768 6963  ent, and in whic
+0000d310: 6820 616c 6c20 6669 6c65 7320 7265 6c61  h all files rela
+0000d320: 7465 6420 746f 2074 6865 2057 6f72 6b20  ted to the Work 
+0000d330: 5265 7175 6972 656d 656e 7420 6172 6520  Requirement are 
+0000d340: 7374 6f72 6564 2e0a 0a31 2e20 4669 6c65  stored...1. File
+0000d350: 7320 746f 2062 6520 7570 6c6f 6164 6564  s to be uploaded
+0000d360: 2074 6861 7420 6172 6520 696e 2074 6865   that are in the
+0000d370: 202a 2a73 616d 6520 6469 7265 6374 6f72   **same director
+0000d380: 7920 6173 2074 6865 2057 6f72 6b20 5265  y as the Work Re
+0000d390: 7175 6972 656d 656e 7420 7370 6563 6966  quirement specif
+0000d3a0: 6963 6174 696f 6e2a 2a20 2874 6865 2054  ication** (the T
+0000d3b0: 4f4d 4c20 6f72 204a 534f 4e20 6669 6c65  OML or JSON file
+0000d3c0: 2920 6172 6520 7570 6c6f 6164 6564 2074  ) are uploaded t
+0000d3d0: 6f20 7468 6520 726f 6f74 206f 6620 7468  o the root of th
+0000d3e0: 6520 576f 726b 2052 6571 7569 7265 6d65  e Work Requireme
+0000d3f0: 6e74 2066 6f6c 6465 722e 0a0a 0a32 2e20  nt folder....2. 
+0000d400: 4669 6c65 7320 746f 2062 6520 7570 6c6f  Files to be uplo
+0000d410: 6164 6564 2074 6861 7420 6172 6520 696e  aded that are in
+0000d420: 202a 2a73 7562 6469 7265 6374 6f72 6965   **subdirectorie
+0000d430: 7320 6265 6c6f 7720 7468 6520 576f 726b  s below the Work
+0000d440: 2052 6571 7569 7265 6d65 6e74 2073 7065   Requirement spe
+0000d450: 6369 6669 6361 7469 6f6e 2c20 6f72 2077  cification, or w
+0000d460: 6865 7265 2061 6273 6f6c 7574 6520 7061  here absolute pa
+0000d470: 7468 6e61 6d65 7320 6172 6520 7375 7070  thnames are supp
+0000d480: 6c69 6564 2a2a 2061 7265 2070 6c61 6365  lied** are place
+0000d490: 6420 696e 2074 6865 204f 626a 6563 7420  d in the Object 
+0000d4a0: 5374 6f72 6520 696e 2064 6972 6563 746f  Store in directo
+0000d4b0: 7269 6573 2074 6861 7420 6d69 7272 6f72  ries that mirror
+0000d4c0: 2074 6865 6972 206c 6f63 616c 2073 746f   their local sto
+0000d4d0: 7261 6765 206c 6f63 6174 696f 6e73 2e0a  rage locations..
+0000d4e0: 0a0a 332e 2046 696c 6573 2074 6f20 6265  ..3. Files to be
+0000d4f0: 2075 706c 6f61 6465 6420 7468 6174 2061   uploaded that a
+0000d500: 7265 2069 6e20 2a2a 6469 7265 6374 6f72  re in **director
+0000d510: 6965 7320 7265 6c61 7469 7665 2074 6f20  ies relative to 
+0000d520: 7468 6520 576f 726b 2052 6571 7569 7265  the Work Require
+0000d530: 6d65 6e74 2073 7065 6369 6669 6361 7469  ment specificati
+0000d540: 6f6e 2c20 7573 696e 6720 602e 2e60 2072  on, using `..` r
+0000d550: 656c 6174 6976 6520 7061 7468 732a 2a20  elative paths** 
+0000d560: 6172 6520 706c 6163 6564 2069 6e20 4f62  are placed in Ob
+0000d570: 6a65 6374 2053 746f 7265 2064 6972 6563  ject Store direc
+0000d580: 746f 7269 6573 2069 6e20 7768 6963 6820  tories in which 
+0000d590: 7468 6520 602e 2e60 2070 6172 7473 206f  the `..` parts o
+0000d5a0: 6620 7468 6520 7061 7468 6e61 6d65 2061  f the pathname a
+0000d5b0: 7265 2072 6570 6c61 6365 6420 7769 7468  re replaced with
+0000d5c0: 2061 6e20 696e 7465 6765 7220 636f 756e   an integer coun
+0000d5d0: 7420 6f66 2074 6865 206e 756d 6265 7220  t of the number 
+0000d5e0: 6f66 2060 2e2e 6020 656e 7472 6965 7320  of `..` entries 
+0000d5f0: 2862 6563 6175 7365 2077 6520 6361 6e27  (because we can'
+0000d600: 7420 7573 6520 7468 6520 602e 2e60 2072  t use the `..` r
+0000d610: 656c 6174 6976 6520 666f 726d 2069 6e20  elative form in 
+0000d620: 7468 6520 4f62 6a65 6374 2053 746f 7265  the Object Store
+0000d630: 292e 0a0a 4173 7375 6d69 6e67 2061 204e  )...Assuming a N
+0000d640: 616d 6573 7061 6365 2063 616c 6c65 6420  amespace called 
+0000d650: 6064 6576 656c 6f70 6d65 6e74 6020 616e  `development` an
+0000d660: 6420 6120 576f 726b 2052 6571 7569 7265  d a Work Require
+0000d670: 6d65 6e74 206e 616d 6564 2060 7465 7374  ment named `test
+0000d680: 7275 6e5f 3232 3131 3038 2d31 3230 3430  run_221108-12040
+0000d690: 342d 3764 3260 2c20 7468 6520 666f 6c6c  4-7d2`, the foll
+0000d6a0: 6f77 696e 6720 6c6f 6361 7469 6f6e 7320  owing locations 
+0000d6b0: 6172 6520 7573 6564 2077 6865 6e20 7570  are used when up
+0000d6c0: 6c6f 6164 696e 6720 6669 6c65 7320 666f  loading files fo
+0000d6d0: 6c6c 6f77 696e 6720 7468 6520 7061 7474  llowing the patt
+0000d6e0: 6572 6e73 2061 626f 7665 3a0a 0a60 6060  erns above:..```
+0000d6f0: 7368 656c 6c0a 2269 6e70 7574 7322 203a  shell."inputs" :
+0000d700: 205b 2266 696c 655f 312e 7478 7422 5d20   ["file_1.txt"] 
+0000d710: 2d3e 2064 6576 656c 6f70 6d65 6e74 3a3a  -> development::
+0000d720: 7465 7374 7275 6e5f 3232 3131 3038 2d31  testrun_221108-1
+0000d730: 3230 3430 342d 3764 322f 6669 6c65 5f31  20404-7d2/file_1
+0000d740: 2e74 7874 0a22 696e 7075 7473 2220 3a20  .txt."inputs" : 
+0000d750: 5b22 6465 762f 6669 6c65 5f31 2e74 7874  ["dev/file_1.txt
+0000d760: 225d 202d 3e20 6465 7665 6c6f 706d 656e  "] -> developmen
+0000d770: 743a 3a74 6573 7472 756e 5f32 3231 3130  t::testrun_22110
+0000d780: 382d 3132 3034 3034 2d37 6432 2f64 6576  8-120404-7d2/dev
+0000d790: 2f66 696c 655f 312e 7478 740a 2269 6e70  /file_1.txt."inp
+0000d7a0: 7574 7322 203a 205b 222f 686f 6d65 2f64  uts" : ["/home/d
+0000d7b0: 6576 2f66 696c 655f 312e 7478 7422 5d20  ev/file_1.txt"] 
+0000d7c0: 2d3e 2064 6576 656c 6f70 6d65 6e74 3a3a  -> development::
+0000d7d0: 7465 7374 7275 6e5f 3232 3131 3038 2d31  testrun_221108-1
+0000d7e0: 3230 3430 342d 3764 322f 686f 6d65 2f64  20404-7d2/home/d
+0000d7f0: 6576 2f66 696c 655f 312e 7478 740a 2269  ev/file_1.txt."i
+0000d800: 6e70 7574 7322 203a 205b 222e 2e2f 6465  nputs" : ["../de
+0000d810: 762f 6669 6c65 5f31 2e74 7874 225d 202d  v/file_1.txt"] -
+0000d820: 3e20 6465 7665 6c6f 706d 656e 743a 3a74  > development::t
+0000d830: 6573 7472 756e 5f32 3231 3130 382d 3132  estrun_221108-12
+0000d840: 3034 3034 2d37 6432 2f31 2f64 6576 2f66  0404-7d2/1/dev/f
+0000d850: 696c 655f 312e 7478 740a 2269 6e70 7574  ile_1.txt."input
+0000d860: 7322 203a 205b 222e 2e2f 2e2e 2f64 6576  s" : ["../../dev
+0000d870: 2f66 696c 655f 312e 7478 7422 5d20 2d3e  /file_1.txt"] ->
+0000d880: 2064 6576 656c 6f70 6d65 6e74 3a3a 7465   development::te
+0000d890: 7374 7275 6e5f 3232 3131 3038 2d31 3230  strun_221108-120
+0000d8a0: 3430 342d 3764 322f 322f 6465 762f 6669  404-7d2/2/dev/fi
+0000d8b0: 6c65 5f31 2e74 7874 0a60 6060 0a0a 2a2a  le_1.txt.```..**
+0000d8c0: 5573 696e 6720 6066 6c61 7474 656e 5570  Using `flattenUp
+0000d8d0: 6c6f 6164 5061 7468 7360 2a2a 0a0a 5468  loadPaths`**..Th
+0000d8e0: 6520 6066 6c61 7474 656e 5570 6c6f 6164  e `flattenUpload
+0000d8f0: 5061 7468 7360 2070 726f 7065 7274 7920  Paths` property 
+0000d900: 6361 6e20 6265 2075 7365 6420 746f 2073  can be used to s
+0000d910: 7570 7072 6573 7320 7468 6520 6d69 7272  uppress the mirr
+0000d920: 6f72 696e 6720 6f66 2061 6e79 206c 6f63  oring of any loc
+0000d930: 616c 2064 6972 6563 746f 7279 2073 7472  al directory str
+0000d940: 7563 7475 7265 2077 6865 6e20 7570 6c6f  ucture when uplo
+0000d950: 6164 696e 6720 6669 6c65 7320 746f 2074  ading files to t
+0000d960: 6865 204f 626a 6563 7420 5374 6f72 652e  he Object Store.
+0000d970: 2049 6620 7365 7420 746f 2060 7472 7565   If set to `true
+0000d980: 602c 2061 6c6c 2066 696c 6573 2077 696c  `, all files wil
+0000d990: 6c20 6265 2075 706c 6f61 6465 6420 746f  l be uploaded to
+0000d9a0: 2074 6865 2072 6f6f 7420 6f66 2074 6865   the root of the
+0000d9b0: 2057 6f72 6b20 5265 7175 6972 656d 656e   Work Requiremen
+0000d9c0: 7420 666f 6c64 6572 2e20 466f 7220 6578  t folder. For ex
+0000d9d0: 616d 706c 653a 0a0a 6060 6073 6865 6c6c  ample:..```shell
+0000d9e0: 0a22 696e 7075 7473 2220 3a20 5b22 6669  ."inputs" : ["fi
+0000d9f0: 6c65 5f31 2e74 7874 225d 202d 3e20 6465  le_1.txt"] -> de
+0000da00: 7665 6c6f 706d 656e 743a 3a74 6573 7472  velopment::testr
+0000da10: 756e 5f32 3231 3130 382d 3132 3034 3034  un_221108-120404
+0000da20: 2d37 6432 2f66 696c 655f 312e 7478 740a  -7d2/file_1.txt.
+0000da30: 2269 6e70 7574 7322 203a 205b 2264 6576  "inputs" : ["dev
+0000da40: 2f66 696c 655f 312e 7478 7422 5d20 2d3e  /file_1.txt"] ->
+0000da50: 2064 6576 656c 6f70 6d65 6e74 3a3a 7465   development::te
+0000da60: 7374 7275 6e5f 3232 3131 3038 2d31 3230  strun_221108-120
+0000da70: 3430 342d 3764 322f 6669 6c65 5f31 2e74  404-7d2/file_1.t
+0000da80: 7874 0a22 696e 7075 7473 2220 3a20 5b22  xt."inputs" : ["
+0000da90: 2f68 6f6d 652f 6465 762f 6669 6c65 5f31  /home/dev/file_1
+0000daa0: 2e74 7874 225d 202d 3e20 6465 7665 6c6f  .txt"] -> develo
+0000dab0: 706d 656e 743a 3a74 6573 7472 756e 5f32  pment::testrun_2
+0000dac0: 3231 3130 382d 3132 3034 3034 2d37 6432  21108-120404-7d2
+0000dad0: 2f66 696c 655f 312e 7478 740a 2269 6e70  /file_1.txt."inp
+0000dae0: 7574 7322 203a 205b 222e 2e2f 6465 762f  uts" : ["../dev/
+0000daf0: 6669 6c65 5f31 2e74 7874 225d 202d 3e20  file_1.txt"] -> 
+0000db00: 6465 7665 6c6f 706d 656e 743a 3a74 6573  development::tes
+0000db10: 7472 756e 5f32 3231 3130 382d 3132 3034  trun_221108-1204
+0000db20: 3034 2d37 6432 2f66 696c 655f 312e 7478  04-7d2/file_1.tx
+0000db30: 740a 2269 6e70 7574 7322 203a 205b 222e  t."inputs" : [".
+0000db40: 2e2f 2e2e 2f64 6576 2f66 696c 655f 312e  ./../dev/file_1.
+0000db50: 7478 7422 5d20 2d3e 2064 6576 656c 6f70  txt"] -> develop
+0000db60: 6d65 6e74 3a3a 7465 7374 7275 6e5f 3232  ment::testrun_22
+0000db70: 3131 3038 2d31 3230 3430 342d 3764 322f  1108-120404-7d2/
+0000db80: 6669 6c65 5f31 2e74 7874 0a60 6060 0a0a  file_1.txt.```..
+0000db90: 5468 6520 7072 6f70 6572 7479 2064 6566  The property def
+0000dba0: 6175 6c74 2069 7320 6066 616c 7365 602e  ault is `false`.
+0000dbb0: 2054 6869 7320 7072 6f70 6572 7479 202a   This property *
+0000dbc0: 2a63 616e 206f 6e6c 7920 6265 2073 6574  *can only be set
+0000dbd0: 2061 7420 7468 6520 576f 726b 2052 6571   at the Work Req
+0000dbe0: 7569 7265 6d65 6e74 206c 6576 656c 2a2a  uirement level**
+0000dbf0: 2061 6e64 2077 696c 6c20 7468 6572 6566   and will theref
+0000dc00: 6f72 6520 6170 706c 7920 746f 2061 6c6c  ore apply to all
+0000dc10: 2054 6173 6b20 4772 6f75 7073 2061 6e64   Task Groups and
+0000dc20: 2054 6173 6b73 2077 6974 6869 6e20 6120   Tasks within a 
+0000dc30: 576f 726b 2052 6571 7569 7265 6d65 6e74  Work Requirement
+0000dc40: 2e0a 0a57 6865 6e20 6669 6c65 7320 6170  ...When files ap
+0000dc50: 7065 6172 2069 6e20 7468 6520 6069 6e70  pear in the `inp
+0000dc60: 7574 7360 206c 6973 742c 2074 6865 7920  uts` list, they 
+0000dc70: 6172 6520 616c 736f 2061 7574 6f6d 6174  are also automat
+0000dc80: 6963 616c 6c79 2061 6464 6564 2074 6f20  ically added to 
+0000dc90: 7468 6520 6c69 7374 206f 6620 6669 6c65  the list of file
+0000dca0: 7320 7265 7175 6972 6564 2062 7920 7468  s required by th
+0000dcb0: 6520 7265 6c65 7661 6e74 2054 6173 6b28  e relevant Task(
+0000dcc0: 7329 2061 7320 6056 6572 6966 7941 7453  s) as `VerifyAtS
+0000dcd0: 7461 7274 6020 6465 7065 6e64 656e 6369  tart` dependenci
+0000dce0: 6573 2e0a 0a23 2323 2320 4669 6c65 7320  es...#### Files 
+0000dcf0: 696e 2074 6865 2060 7570 6c6f 6164 4669  in the `uploadFi
+0000dd00: 6c65 7360 204c 6973 740a 0a54 6865 2060  les` List..The `
+0000dd10: 7570 6c6f 6164 4669 6c65 7360 2070 726f  uploadFiles` pro
+0000dd20: 7065 7274 7920 616c 6c6f 7773 206d 6f72  perty allows mor
+0000dd30: 6520 666c 6578 6962 6c65 2063 6f6e 7472  e flexible contr
+0000dd40: 6f6c 206f 7665 7220 7468 6520 6669 6c65  ol over the file
+0000dd50: 7320 746f 2062 6520 7570 6c6f 6164 6564  s to be uploaded
+0000dd60: 2066 726f 6d20 6c6f 6361 6c20 7374 6f72   from local stor
+0000dd70: 6167 6520 746f 2074 6865 204f 626a 6563  age to the Objec
+0000dd80: 7420 5374 6f72 6520 7768 656e 2060 7964  t Store when `yd
+0000dd90: 2d73 7562 6d69 7460 2069 7320 7275 6e2e  -submit` is run.
+0000dda0: 2054 6865 2070 726f 7065 7274 7920 6361   The property ca
+0000ddb0: 6e20 6265 2075 7365 6420 6174 2061 6c6c  n be used at all
+0000ddc0: 2057 6f72 6b20 5265 7175 6972 656d 656e   Work Requiremen
+0000ddd0: 7420 6c65 7665 6c73 2c20 6672 6f6d 2074  t levels, from t
+0000dde0: 6865 2054 4f4d 4c20 6669 6c65 2074 6872  he TOML file thr
+0000ddf0: 6f75 6768 2074 6f20 696e 6469 7669 6475  ough to individu
+0000de00: 616c 2054 6173 6b20 7370 6563 6966 6963  al Task specific
+0000de10: 6174 696f 6e73 2e0a 0a54 6865 2070 726f  ations...The pro
+0000de20: 7065 7274 7920 6973 2073 7570 706c 6965  perty is supplie
+0000de30: 6420 6173 2061 206c 6973 7420 6f66 2064  d as a list of d
+0000de40: 6963 7469 6f6e 6172 7920 6974 656d 732c  ictionary items,
+0000de50: 2065 6163 6820 6f66 2077 6869 6368 206d   each of which m
+0000de60: 7573 7420 696e 636c 7564 6520 7468 6520  ust include the 
+0000de70: 7072 6f70 6572 7469 6573 2060 6c6f 6361  properties `loca
+0000de80: 6c50 6174 6860 2061 6e64 2060 7570 6c6f  lPath` and `uplo
+0000de90: 6164 5061 7468 602e 200a 0a2d 2060 6c6f  adPath`. ..- `lo
+0000dea0: 6361 6c50 6174 6860 2073 7065 6369 6669  calPath` specifi
+0000deb0: 6573 2074 6865 2070 6174 686e 616d 6520  es the pathname 
+0000dec0: 6f66 2074 6865 2066 696c 6520 6f6e 206c  of the file on l
+0000ded0: 6f63 616c 2073 746f 7261 6765 0a2d 2060  ocal storage.- `
+0000dee0: 7570 6c6f 6164 5061 7468 6020 7370 6563  uploadPath` spec
+0000def0: 6966 6965 7320 7468 6520 6e61 6d65 2061  ifies the name a
+0000df00: 6e64 206c 6f63 6174 696f 6e20 6f66 2074  nd location of t
+0000df10: 6865 2066 696c 6527 7320 6465 7374 696e  he file's destin
+0000df20: 6174 696f 6e20 696e 2074 6865 204f 626a  ation in the Obj
+0000df30: 6563 7420 5374 6f72 650a 0a46 6f72 2065  ect Store..For e
+0000df40: 7861 6d70 6c65 2c20 696e 2054 4f4d 4c3a  xample, in TOML:
+0000df50: 0a60 6060 746f 6d6c 0a75 706c 6f61 6446  .```toml.uploadF
+0000df60: 696c 6573 203d 205b 0a20 2020 207b 6c6f  iles = [.    {lo
+0000df70: 6361 6c50 6174 6820 3d20 2266 696c 655f  calPath = "file_
+0000df80: 312e 7478 7422 2c20 7570 6c6f 6164 5061  1.txt", uploadPa
+0000df90: 7468 203d 2022 6669 6c65 5f31 2e74 7874  th = "file_1.txt
+0000dfa0: 227d 2c0a 2020 2020 7b6c 6f63 616c 5061  "},.    {localPa
+0000dfb0: 7468 203d 2022 6469 725f 322f 6669 6c65  th = "dir_2/file
+0000dfc0: 5f32 2e74 7874 222c 2075 706c 6f61 6450  _2.txt", uploadP
+0000dfd0: 6174 6820 3d20 223a 3a66 696c 655f 322e  ath = "::file_2.
+0000dfe0: 7478 7422 7d2c 0a20 2020 207b 6c6f 6361  txt"},.    {loca
+0000dff0: 6c50 6174 6820 3d20 2266 696c 655f 332e  lPath = "file_3.
+0000e000: 7478 7422 2c20 7570 6c6f 6164 5061 7468  txt", uploadPath
+0000e010: 203d 2022 6f74 6865 725f 6e61 6d65 7370   = "other_namesp
+0000e020: 6163 653a 3a66 696c 655f 332e 7478 7422  ace::file_3.txt"
+0000e030: 7d0a 5d0a 6060 600a 416e 6420 696e 204a  }.].```.And in J
+0000e040: 534f 4e2c 2077 6974 6820 7468 6520 7072  SON, with the pr
+0000e050: 6f70 6572 7479 2073 6574 2061 7420 7468  operty set at th
+0000e060: 6520 5461 736b 206c 6576 656c 2c20 7468  e Task level, th
+0000e070: 6520 7361 6d65 2073 7065 6369 6669 6361  e same specifica
+0000e080: 7469 6f6e 2077 6f75 6c64 2062 653a 0a60  tion would be:.`
+0000e090: 6060 6a73 6f6e 0a7b 0a20 2022 7461 736b  ``json.{.  "task
+0000e0a0: 4772 6f75 7073 223a 205b 0a20 2020 207b  Groups": [.    {
+0000e0b0: 0a20 2020 2020 2022 7461 736b 7322 3a20  .      "tasks": 
+0000e0c0: 5b0a 2020 2020 2020 2020 7b0a 2020 2020  [.        {.    
+0000e0d0: 2020 2020 2020 2275 706c 6f61 6446 696c        "uploadFil
+0000e0e0: 6573 223a 205b 0a20 2020 2020 2020 2020  es": [.         
+0000e0f0: 2020 207b 226c 6f63 616c 5061 7468 223a     {"localPath":
+0000e100: 2022 6669 6c65 5f31 2e74 7874 222c 2022   "file_1.txt", "
+0000e110: 7570 6c6f 6164 5061 7468 223a 2022 6669  uploadPath": "fi
+0000e120: 6c65 5f31 2e74 7874 227d 2c0a 2020 2020  le_1.txt"},.    
+0000e130: 2020 2020 2020 2020 7b22 6c6f 6361 6c50          {"localP
+0000e140: 6174 6822 3a20 2264 6972 5f32 2f66 696c  ath": "dir_2/fil
+0000e150: 655f 322e 7478 7422 2c20 2275 706c 6f61  e_2.txt", "uploa
+0000e160: 6450 6174 6822 3a20 223a 3a66 696c 655f  dPath": "::file_
+0000e170: 322e 7478 7422 7d2c 0a20 2020 2020 2020  2.txt"},.       
+0000e180: 2020 2020 207b 226c 6f63 616c 5061 7468       {"localPath
+0000e190: 223a 2022 6669 6c65 5f33 2e74 7874 222c  ": "file_3.txt",
+0000e1a0: 2022 7570 6c6f 6164 5061 7468 223a 2022   "uploadPath": "
+0000e1b0: 6f74 6865 725f 6e61 6d65 7370 6163 653a  other_namespace:
+0000e1c0: 3a66 696c 655f 332e 7478 7422 7d0a 2020  :file_3.txt"}.  
+0000e1d0: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
+0000e1e0: 2020 7d0a 2020 2020 2020 5d0a 2020 2020    }.      ].    
+0000e1f0: 7d0a 2020 5d0a 7d0a 6060 600a 0a57 6865  }.  ].}.```..Whe
+0000e200: 6e20 7275 6e6e 696e 6720 7468 6520 5079  n running the Py
+0000e210: 7468 6f6e 2045 7861 6d70 6c65 7320 636f  thon Examples co
+0000e220: 6d6d 616e 6473 206f 6e20 2a2a 5769 6e64  mmands on **Wind
+0000e230: 6f77 732a 2a20 686f 7374 732c 206e 6f74  ows** hosts, not
+0000e240: 6520 7468 6174 2065 6974 6865 7220 5769  e that either Wi
+0000e250: 6e64 6f77 7320 6f72 2055 6e69 7820 6469  ndows or Unix di
+0000e260: 7265 6374 6f72 7920 7365 7061 7261 746f  rectory separato
+0000e270: 7273 2063 616e 2062 6520 7573 6564 2066  rs can be used f
+0000e280: 6f72 2074 6865 2060 6c6f 6361 6c50 6174  or the `localPat
+0000e290: 6860 2070 6174 686e 616d 6573 2028 6f72  h` pathnames (or
+0000e2a0: 2074 6865 2070 6174 686e 616d 6573 2069   the pathnames i
+0000e2b0: 6e20 6069 6e70 7574 7360 292c 2062 7574  n `inputs`), but
+0000e2c0: 2074 6865 2055 6e69 7820 636f 6e76 656e   the Unix conven
+0000e2d0: 7469 6f6e 206d 7573 7420 6265 2075 7365  tion must be use
+0000e2e0: 6420 666f 7220 7468 6520 6075 706c 6f61  d for the `uploa
+0000e2f0: 6450 6174 6860 206e 616d 6573 2c20 652e  dPath` names, e.
+0000e300: 672e 3a0a 0a60 6060 746f 6d6c 0a75 706c  g.:..```toml.upl
+0000e310: 6f61 6446 696c 6573 203d 205b 0a20 2020  oadFiles = [.   
+0000e320: 207b 6c6f 6361 6c50 6174 6820 3d20 2264   {localPath = "d
+0000e330: 6972 5f32 5c5c 6669 6c65 5f32 2e74 7874  ir_2\\file_2.txt
+0000e340: 222c 2075 706c 6f61 6450 6174 6820 3d20  ", uploadPath = 
+0000e350: 223a 3a6d 795f 6469 7265 6374 6f72 792f  "::my_directory/
+0000e360: 6669 6c65 5f32 2e74 7874 227d 2c0a 5d0a  file_2.txt"},.].
+0000e370: 6060 600a 0a54 6865 2060 7570 6c6f 6164  ```..The `upload
+0000e380: 4669 6c65 7360 2070 726f 7065 7274 7920  Files` property 
+0000e390: 6361 6e20 616c 736f 2062 6520 7365 7420  can also be set 
+0000e3a0: 6174 2074 6865 2057 6f72 6b20 5265 7175  at the Work Requ
+0000e3b0: 6972 656d 656e 7420 616e 6420 5461 736b  irement and Task
+0000e3c0: 2047 726f 7570 206c 6576 656c 732c 2061   Group levels, a
+0000e3d0: 6e64 2070 726f 7065 7274 7920 696e 6865  nd property inhe
+0000e3e0: 7269 7461 6e63 6520 6f70 6572 6174 6573  ritance operates
+0000e3f0: 2061 7320 6e6f 726d 616c 2e0a 0a46 6f72   as normal...For
+0000e400: 2060 7570 6c6f 6164 5061 7468 602c 2074   `uploadPath`, t
+0000e410: 6865 2073 616d 6520 603a 3a60 206e 616d  he same `::` nam
+0000e420: 696e 6720 636f 6e76 656e 7469 6f6e 2069  ing convention i
+0000e430: 7320 6176 6169 6c61 626c 6520 6173 2069  s available as i
+0000e440: 7320 7573 6564 2069 6e20 7468 6520 6076  s used in the `v
+0000e450: 6572 6966 7941 7453 7461 7274 602c 2060  erifyAtStart`, `
+0000e460: 7665 7269 6679 5761 6974 6020 616e 6420  verifyWait` and 
+0000e470: 6069 6e70 7574 734f 7074 696f 6e61 6c60  `inputsOptional`
+0000e480: 2070 726f 7065 7274 6965 7320 6469 7363   properties disc
+0000e490: 7573 7365 6420 6265 6c6f 773a 0a0a 2d20  ussed below:..- 
+0000e4a0: 4966 2060 3a3a 6020 6973 206e 6f74 2075  If `::` is not u
+0000e4b0: 7365 642c 2074 6865 6e20 7468 6520 6669  sed, then the fi
+0000e4c0: 6c65 2069 7320 7570 6c6f 6164 6564 2072  le is uploaded r
+0000e4d0: 656c 6174 6976 6520 746f 2074 6865 2063  elative to the c
+0000e4e0: 7572 7265 6e74 206e 616d 6573 7061 6365  urrent namespace
+0000e4f0: 2069 6e20 6120 6469 7265 6374 6f72 7920   in a directory 
+0000e500: 6e61 6d65 6420 6166 7465 7220 7468 6520  named after the 
+0000e510: 6e61 6d65 206f 6620 7468 6520 576f 726b  name of the Work
+0000e520: 2052 6571 7569 7265 6d65 6e74 0a2d 2049   Requirement.- I
+0000e530: 6620 603a 3a60 2069 7320 7573 6564 2061  f `::` is used a
+0000e540: 7420 7468 6520 7374 6172 7420 6f66 2074  t the start of t
+0000e550: 6865 2060 7570 6c6f 6164 5061 7468 602c  he `uploadPath`,
+0000e560: 2074 6865 2066 696c 6520 6973 2075 706c   the file is upl
+0000e570: 6f61 6465 6420 7265 6c61 7469 7665 2074  oaded relative t
+0000e580: 6f20 7468 6520 726f 6f74 206f 6620 7468  o the root of th
+0000e590: 6520 6375 7272 656e 7420 6e61 6d65 7370  e current namesp
+0000e5a0: 6163 650a 2d20 4966 2060 3c6e 616d 6573  ace.- If `<names
+0000e5b0: 7061 6365 3e3a 3a60 2069 7320 7573 6564  pace>::` is used
+0000e5c0: 2061 7420 7468 6520 7374 6172 7420 6f66   at the start of
+0000e5d0: 2060 7570 6c6f 6164 5061 7468 602c 2074   `uploadPath`, t
+0000e5e0: 6865 2066 696c 6520 6973 2075 706c 6f61  he file is uploa
+0000e5f0: 6465 6420 7265 6c61 7469 7665 2074 6f20  ded relative to 
+0000e600: 7468 6520 726f 6f74 206f 6620 603c 6e61  the root of `<na
+0000e610: 6d65 7370 6163 653e 600a 0a45 6163 6820  mespace>`..Each 
+0000e620: 6669 6c65 2073 7065 6369 6669 6564 2069  file specified i
+0000e630: 6e20 7468 6520 6075 706c 6f61 6446 696c  n the `uploadFil
+0000e640: 6573 6020 6c69 7374 7320 7769 6c6c 206f  es` lists will o
+0000e650: 6e6c 7920 6265 2075 706c 6f61 6465 6420  nly be uploaded 
+0000e660: 6f6e 6365 2074 6f20 6561 6368 2075 6e69  once to each uni
+0000e670: 7175 6520 7570 6c6f 6164 206c 6f63 6174  que upload locat
+0000e680: 696f 6e20 666f 7220 616e 7920 6769 7665  ion for any give
+0000e690: 6e20 696e 766f 6361 7469 6f6e 206f 6620  n invocation of 
+0000e6a0: 6079 642d 7375 626d 6974 602e 0a0a 4966  `yd-submit`...If
+0000e6b0: 2061 2066 696c 6520 696e 2074 6865 2060   a file in the `
+0000e6c0: 7570 6c6f 6164 4669 6c65 7360 206c 6973  uploadFiles` lis
+0000e6d0: 7420 6973 2072 6571 7569 7265 6420 6279  t is required by
+0000e6e0: 2061 2054 6173 6b2c 2069 7420 6d75 7374   a Task, it must
+0000e6f0: 2073 6570 6172 6174 656c 7920 6265 2061   separately be a
+0000e700: 6464 6564 2074 6f20 7468 6520 6076 6572  dded to the `ver
+0000e710: 6966 7941 7453 7461 7274 6020 6f72 2060  ifyAtStart` or `
+0000e720: 7665 7269 6679 5761 6974 6020 6c69 7374  verifyWait` list
+0000e730: 7320 6469 7363 7573 7365 6420 6265 6c6f  s discussed belo
+0000e740: 772e 2054 6869 7320 6973 206e 6f74 2064  w. This is not d
+0000e750: 6f6e 6520 6175 746f 6d61 7469 6361 6c6c  one automaticall
+0000e760: 792e 204e 6f74 6520 616c 736f 2074 6861  y. Note also tha
+0000e770: 7420 7468 6520 6066 6c61 7474 656e 5570  t the `flattenUp
+0000e780: 6c6f 6164 5061 7468 7360 2070 726f 7065  loadPaths` prope
+0000e790: 7274 7920 6973 2069 676e 6f72 6564 2066  rty is ignored f
+0000e7a0: 6f72 2066 696c 6573 2069 6e20 7468 6520  or files in the 
+0000e7b0: 6075 706c 6f61 6446 696c 6573 6020 6c69  `uploadFiles` li
+0000e7c0: 7374 2e0a 0a23 2323 2046 696c 6520 4465  st...### File De
+0000e7d0: 7065 6e64 656e 6369 6573 2055 7369 6e67  pendencies Using
+0000e7e0: 2060 7665 7269 6679 4174 5374 6172 7460   `verifyAtStart`
+0000e7f0: 2061 6e64 2060 7665 7269 6679 5761 6974   and `verifyWait
+0000e800: 600a 0a49 7427 7320 706f 7373 6962 6c65  `..It's possible
+0000e810: 2074 6f20 6d61 6b65 2054 6173 6b73 2064   to make Tasks d
+0000e820: 6570 656e 6465 6e74 206f 6e20 7468 6520  ependent on the 
+0000e830: 7072 6573 656e 6365 206f 6620 6669 6c65  presence of file
+0000e840: 7320 696e 2074 6865 204f 626a 6563 7420  s in the Object 
+0000e850: 5374 6f72 6520 6279 2075 7369 6e67 2074  Store by using t
+0000e860: 6865 2060 7665 7269 6679 4174 5374 6172  he `verifyAtStar
+0000e870: 7460 2061 6e64 2060 7665 7269 6679 5761  t` and `verifyWa
+0000e880: 6974 6020 6c69 7374 732e 2054 6865 7365  it` lists. These
+0000e890: 2066 696c 6573 2061 7265 206e 6f74 2061   files are not a
+0000e8a0: 7574 6f6d 6174 6963 616c 6c79 2075 706c  utomatically upl
+0000e8b0: 6f61 6465 6420 7768 656e 2075 7369 6e67  oaded when using
+0000e8c0: 2060 7964 2d73 7562 6d69 7460 2073 6f20   `yd-submit` so 
+0000e8d0: 6172 6520 6569 7468 6572 2075 706c 6f61  are either uploa
+0000e8e0: 6465 6420 6d61 6e75 616c 6c79 2028 652e  ded manually (e.
+0000e8f0: 672e 2c20 6279 2075 7369 6e67 2060 7964  g., by using `yd
+0000e900: 2d75 706c 6f61 6460 292c 206f 7220 6172  -upload`), or ar
+0000e910: 6520 6372 6561 7465 6420 6173 2061 2072  e created as a r
+0000e920: 6573 756c 7420 6f66 2074 6865 2065 7865  esult of the exe
+0000e930: 6375 7469 6f6e 206f 6620 6f74 6865 7220  cution of other 
+0000e940: 5461 736b 732e 0a0a 4e6f 7465 2074 6861  Tasks...Note tha
+0000e950: 7420 6120 6769 7665 6e20 6669 6c65 2063  t a given file c
+0000e960: 616e 206f 6e6c 7920 6170 7065 6172 2069  an only appear i
+0000e970: 6e20 2a6f 6e65 2a20 6f66 2074 6865 2060  n *one* of the `
+0000e980: 696e 7075 7473 602c 2060 7665 7269 6679  inputs`, `verify
+0000e990: 4174 5374 6172 7460 206f 7220 6076 6572  AtStart` or `ver
+0000e9a0: 6966 7957 6169 7460 206c 6973 7473 2e0a  ifyWait` lists..
+0000e9b0: 0a54 6173 6b73 2077 6974 6820 6076 6572  .Tasks with `ver
+0000e9c0: 6966 7941 7453 7461 7274 6020 6465 7065  ifyAtStart` depe
+0000e9d0: 6e64 656e 6369 6573 2077 696c 6c20 6661  ndencies will fa
+0000e9e0: 696c 2069 6d6d 6564 6961 7465 6c79 2069  il immediately i
+0000e9f0: 6620 7468 6520 7265 7175 6972 6564 2066  f the required f
+0000ea00: 696c 6573 2061 7265 206e 6f74 2070 7265  iles are not pre
+0000ea10: 7365 6e74 2077 6865 6e20 7468 6520 5461  sent when the Ta
+0000ea20: 736b 2069 7320 7375 626d 6974 7465 642e  sk is submitted.
+0000ea30: 2054 6173 6b73 2077 6974 6820 6076 6572   Tasks with `ver
+0000ea40: 6966 7957 6169 7460 2064 6570 656e 6465  ifyWait` depende
+0000ea50: 6e63 6965 7320 7769 6c6c 206e 6f74 2062  ncies will not b
+0000ea60: 6563 6f6d 6520 6052 4541 4459 6020 746f  ecome `READY` to
+0000ea70: 2062 6520 7363 6865 6475 6c65 6420 746f   be scheduled to
+0000ea80: 2057 6f72 6b65 7273 2075 6e74 696c 2074   Workers until t
+0000ea90: 6865 2064 6570 656e 6465 6e63 6965 7320  he dependencies 
+0000eaa0: 6172 6520 7361 7469 7366 6965 642e 0a0a  are satisfied...
+0000eab0: 5768 656e 2073 7065 6369 6679 696e 6720  When specifying 
+0000eac0: 6669 6c65 7320 696e 2074 6865 2060 7665  files in the `ve
+0000ead0: 7269 6679 4174 5374 6172 7460 2061 6e64  rifyAtStart` and
+0000eae0: 2060 7665 7269 6679 5761 6974 6020 6c69   `verifyWait` li
+0000eaf0: 7374 732c 2061 7320 7769 7468 2074 6865  sts, as with the
+0000eb00: 2060 7570 6c6f 6164 5061 7468 6020 7072   `uploadPath` pr
+0000eb10: 6f70 6572 7479 2064 6973 6375 7373 6564  operty discussed
+0000eb20: 2061 626f 7665 2c20 7468 6520 6669 6c65   above, the file
+0000eb30: 206c 6f63 6174 696f 6e73 2063 616e 2062   locations can b
+0000eb40: 6520 2831 2920 7265 6c61 7469 7665 2074  e (1) relative t
+0000eb50: 6f20 7468 6520 576f 726b 2052 6571 7569  o the Work Requi
+0000eb60: 7265 6d65 6e74 206e 616d 6520 696e 2074  rement name in t
+0000eb70: 6865 2063 7572 7265 6e74 206e 616d 6573  he current names
+0000eb80: 7061 6365 2028 7468 6520 6465 6661 756c  pace (the defaul
+0000eb90: 7429 2c20 2832 2920 7265 6c61 7469 7665  t), (2) relative
+0000eba0: 2074 6f20 7468 6520 726f 6f74 206f 6620   to the root of 
+0000ebb0: 7468 6520 6375 7272 656e 7420 6e61 6d65  the current name
+0000ebc0: 7370 6163 652c 206f 7220 2833 2920 7265  space, or (3) re
+0000ebd0: 6c61 7469 7665 2074 6f20 7468 6520 726f  lative to the ro
+0000ebe0: 6f74 206f 6620 6120 6469 6666 6572 656e  ot of a differen
+0000ebf0: 7420 6e61 6d65 7370 6163 6520 696e 2074  t namespace in t
+0000ec00: 6865 2075 7365 7227 7320 4163 636f 756e  he user's Accoun
+0000ec10: 742e 0a0a 312e 2046 6f72 2066 696c 6573  t...1. For files
+0000ec20: 2072 656c 6174 6976 6520 746f 2074 6865   relative to the
+0000ec30: 2057 6f72 6b20 5265 7175 6972 656d 656e   Work Requiremen
+0000ec40: 7420 6e61 6d65 2069 6e20 7468 6520 6375  t name in the cu
+0000ec50: 7272 656e 7420 6e61 6d65 7370 6163 652c  rrent namespace,
+0000ec60: 206a 7573 7420 7573 6520 7468 6520 6669   just use the fi
+0000ec70: 6c65 2070 6174 682c 2065 2e67 2e0a 6060  le path, e.g..``
+0000ec80: 6073 6865 6c6c 0a22 7665 7269 6679 5761  `shell."verifyWa
+0000ec90: 6974 223a 205b 2266 696c 655f 312e 7478  it": ["file_1.tx
+0000eca0: 7422 5d20 2d3e 2064 6576 656c 6f70 6d65  t"] -> developme
+0000ecb0: 6e74 3a74 6573 7472 756e 5f32 3231 3130  nt:testrun_22110
+0000ecc0: 382d 3132 3034 3034 2d37 6432 2f66 696c  8-120404-7d2/fil
+0000ecd0: 655f 312e 7478 740a 6060 600a 0a32 2e20  e_1.txt.```..2. 
+0000ece0: 466f 7220 6669 6c65 7320 7265 6c61 7469  For files relati
+0000ecf0: 7665 2074 6f20 7468 6520 726f 6f74 206f  ve to the root o
+0000ed00: 6620 7468 6520 6375 7272 656e 7420 6e61  f the current na
+0000ed10: 6d65 7370 6163 652c 2070 7265 6669 7820  mespace, prefix 
+0000ed20: 7468 6520 6669 6c65 2070 6174 6820 7769  the file path wi
+0000ed30: 7468 2060 3a3a 602c 2065 2e67 2e0a 6060  th `::`, e.g..``
+0000ed40: 6073 6865 6c6c 0a22 7665 7269 6679 5761  `shell."verifyWa
+0000ed50: 6974 223a 205b 223a 3a66 696c 655f 312e  it": ["::file_1.
+0000ed60: 7478 7422 5d20 2d3e 2064 6576 656c 6f70  txt"] -> develop
+0000ed70: 6d65 6e74 3a66 696c 655f 312e 7478 740a  ment:file_1.txt.
+0000ed80: 6060 600a 0a33 2e20 466f 7220 6669 6c65  ```..3. For file
+0000ed90: 7320 7265 6c61 7469 7665 2074 6f20 7468  s relative to th
+0000eda0: 6520 726f 6f74 206f 6620 6120 6469 6666  e root of a diff
+0000edb0: 6572 656e 7420 6e61 6d65 7370 6163 652c  erent namespace,
+0000edc0: 2070 7265 6669 7820 7468 6520 6669 6c65   prefix the file
+0000edd0: 2070 6174 6820 7769 7468 2074 6865 206e   path with the n
+0000ede0: 616d 6573 7061 6365 206e 616d 6520 616e  amespace name an
+0000edf0: 6420 603a 3a60 2c20 652e 672e 0a60 6060  d `::`, e.g..```
+0000ee00: 7368 656c 6c0a 2276 6572 6966 7957 6169  shell."verifyWai
+0000ee10: 7422 3a20 5b22 6f74 6865 725f 6e61 6d65  t": ["other_name
+0000ee20: 7370 6163 653a 3a66 696c 655f 312e 7478  space::file_1.tx
+0000ee30: 7422 5d20 2d3e 206f 7468 6572 5f6e 616d  t"] -> other_nam
+0000ee40: 6573 7061 6365 3a66 696c 655f 312e 7478  espace:file_1.tx
+0000ee50: 740a 6060 600a 0a54 6865 2075 7365 206f  t.```..The use o
+0000ee60: 6620 7468 6520 7468 7265 6520 6469 6666  f the three diff
+0000ee70: 6572 656e 7420 666f 726d 7320 6361 6e20  erent forms can 
+0000ee80: 6265 206d 6978 6564 2077 6974 6869 6e20  be mixed within 
+0000ee90: 6120 7369 6e67 6c65 206c 6973 742c 2065  a single list, e
+0000eea0: 2e67 2e3a 0a60 6060 7368 656c 6c0a 2276  .g.:.```shell."v
+0000eeb0: 6572 6966 7941 7453 7461 7274 223a 205b  erifyAtStart": [
+0000eec0: 2266 696c 655f 312e 7478 7422 2c20 223a  "file_1.txt", ":
+0000eed0: 3a64 6972 5f32 2f66 696c 655f 322e 7478  :dir_2/file_2.tx
+0000eee0: 7422 2c20 226f 7468 6572 5f6e 616d 6573  t", "other_names
+0000eef0: 7061 6365 3a3a 6469 725f 332f 6669 6c65  pace::dir_3/file
+0000ef00: 5f33 2e74 7874 225d 0a60 6060 0a0a 2323  _3.txt"].```..##
+0000ef10: 2320 4669 6c65 7320 446f 776e 6c6f 6164  # Files Download
+0000ef20: 6564 2055 7369 6e67 2060 696e 7075 7473  ed Using `inputs
+0000ef30: 4f70 7469 6f6e 616c 600a 0a54 6865 2060  Optional`..The `
+0000ef40: 696e 7075 7473 4f70 7469 6f6e 616c 6020  inputsOptional` 
+0000ef50: 7072 6f70 6572 7479 2077 6f72 6b73 2069  property works i
+0000ef60: 6e20 6120 7369 6d69 6c61 7220 6661 7368  n a similar fash
+0000ef70: 696f 6e20 746f 2074 6865 2060 7665 7269  ion to the `veri
+0000ef80: 6679 2a60 2070 726f 7065 7274 6965 7320  fy*` properties 
+0000ef90: 6162 6f76 652c 2062 7574 2074 6865 2066  above, but the f
+0000efa0: 696c 6573 2073 7065 6369 6669 6564 2069  iles specified i
+0000efb0: 6e20 7468 6973 206c 6973 7420 6172 6520  n this list are 
+0000efc0: 6f70 7469 6f6e 616c 2e20 5468 6973 2070  optional. This p
+0000efd0: 726f 7065 7274 7920 616c 736f 2061 6c6c  roperty also all
+0000efe0: 6f77 7320 666f 7220 7468 6520 7573 6520  ows for the use 
+0000eff0: 6f66 2077 696c 6463 6172 6473 2060 2a60  of wildcards `*`
+0000f000: 2061 6e64 2060 2a2a 6020 746f 2063 6f6c   and `**` to col
+0000f010: 6c65 6374 2066 696c 6573 2075 7369 6e67  lect files using
+0000f020: 2077 696c 6463 6172 6420 7061 7468 732e   wildcard paths.
+0000f030: 2054 6865 202a 2a61 6e74 2a2a 2063 6f6e   The **ant** con
+0000f040: 7665 6e74 696f 6e73 2061 7265 2075 7365  ventions are use
+0000f050: 6420 666f 7220 7468 6573 6520 7769 6c64  d for these wild
+0000f060: 6361 7264 732e 0a0a 2323 2320 4669 6c65  cards...### File
+0000f070: 7320 446f 776e 6c6f 6164 6564 2074 6f20  s Downloaded to 
+0000f080: 6120 4e6f 6465 2066 6f72 2075 7365 2069  a Node for use i
+0000f090: 6e20 5461 736b 2045 7865 6375 7469 6f6e  n Task Execution
+0000f0a0: 0a0a 5768 656e 2061 2054 6173 6b20 6973  ..When a Task is
+0000f0b0: 2065 7865 6375 7465 6420 6279 2061 2057   executed by a W
+0000f0c0: 6f72 6b65 7220 6f6e 2061 204e 6f64 652c  orker on a Node,
+0000f0d0: 2069 7473 2072 6571 7569 7265 6420 6669   its required fi
+0000f0e0: 6c65 7320 6172 6520 646f 776e 6c6f 6164  les are download
+0000f0f0: 6564 2066 726f 6d20 7468 6520 4f62 6a65  ed from the Obje
+0000f100: 6374 2053 746f 7265 2070 7269 6f72 2074  ct Store prior t
+0000f110: 6f20 5461 736b 2065 7865 6375 7469 6f6e  o Task execution
+0000f120: 2e20 416e 7920 6669 6c65 206c 6973 7465  . Any file liste
+0000f130: 6420 696e 2074 6865 2060 696e 7075 7473  d in the `inputs
+0000f140: 6020 666f 7220 6120 5461 736b 2069 7320  ` for a Task is 
+0000f150: 6173 7375 6d65 6420 746f 2062 6520 7265  assumed to be re
+0000f160: 7175 6972 6564 2c20 616c 6f6e 6720 7769  quired, along wi
+0000f170: 7468 2061 6e79 2061 6464 6974 696f 6e61  th any additiona
+0000f180: 6c20 6669 6c65 7320 7370 6563 6966 6965  l files specifie
+0000f190: 6420 696e 2074 6865 2060 7665 7269 6679  d in the `verify
+0000f1a0: 4174 5374 6172 7460 2061 6e64 2060 7665  AtStart` and `ve
+0000f1b0: 7269 6679 5761 6974 6020 6c69 7374 732e  rifyWait` lists.
+0000f1c0: 2046 696c 6573 2073 7065 6369 6669 6564   Files specified
+0000f1d0: 2075 7369 6e67 2074 6865 2060 696e 7075   using the `inpu
+0000f1e0: 7473 4f70 7469 6f6e 616c 6020 7072 6f70  tsOptional` prop
+0000f1f0: 6572 7479 2061 7265 206f 7074 696f 6e61  erty are optiona
+0000f200: 6c6c 7920 646f 776e 6c6f 6164 6564 2066  lly downloaded f
+0000f210: 726f 6d20 7468 6520 4f62 6a65 6374 2053  rom the Object S
+0000f220: 746f 7265 2e20 284e 6f74 6520 7468 6174  tore. (Note that
+0000f230: 2061 2066 696c 6520 7368 6f75 6c64 206f   a file should o
+0000f240: 6e6c 7920 6170 7065 6172 2069 6e20 6f6e  nly appear in on
+0000f250: 6520 6f66 2074 6865 7365 2066 6f75 7220  e of these four 
+0000f260: 6c69 7374 732c 206f 7468 6572 7769 7365  lists, otherwise
+0000f270: 2060 7964 2d73 7562 6d69 7460 2077 696c   `yd-submit` wil
+0000f280: 6c20 7265 7475 726e 2061 6e20 6572 726f  l return an erro
+0000f290: 722e 290a 0a57 6865 6e20 6120 5461 736b  r.)..When a Task
+0000f2a0: 2069 7320 7374 6172 7465 6420 6279 2074   is started by t
+0000f2b0: 6865 2041 6765 6e74 2c20 6974 7320 776f  he Agent, its wo
+0000f2c0: 726b 696e 6720 6469 7265 6374 6f72 7920  rking directory 
+0000f2d0: 6861 7320 6120 7061 7474 6572 6e20 736f  has a pattern so
+0000f2e0: 6d65 7468 696e 6720 6c69 6b65 3a0a 0a60  mething like:..`
+0000f2f0: 2f76 6172 2f6f 7074 2f79 656c 6c6f 7764  /var/opt/yellowd
+0000f300: 6f67 2f79 642d 6167 656e 742d 342f 6461  og/yd-agent-4/da
+0000f310: 7461 2f77 6f72 6b65 7273 2f31 2f79 6469  ta/workers/1/ydi
+0000f320: 645f 7461 736b 5f44 3044 3044 305f 3638  d_task_D0D0D0_68
+0000f330: 6635 6535 6265 2d64 6339 332d 3439 6562  f5e5be-dc93-49eb
+0000f340: 2d61 3832 342d 3166 6364 6235 3266 3931  -a824-1fcdb52f91
+0000f350: 3935 5f31 5f31 600a 0a28 6079 6469 645f  95_1_1`..(`ydid_
+0000f360: 7461 736b 5f44 3044 3044 305f 3638 6635  task_D0D0D0_68f5
+0000f370: 6535 6265 2d64 6339 332d 3439 6562 2d61  e5be-dc93-49eb-a
+0000f380: 3832 342d 3166 6364 6235 3266 3931 3935  824-1fcdb52f9195
+0000f390: 5f31 5f31 6020 6973 2061 6e20 6570 6865  _1_1` is an ephe
+0000f3a0: 6d65 7261 6c20 6469 7265 6374 6f72 7920  meral directory 
+0000f3b0: 7468 6174 2069 7320 7265 6d6f 7665 6420  that is removed 
+0000f3c0: 6166 7465 7220 7468 6520 5461 736b 2066  after the Task f
+0000f3d0: 696e 6973 6865 7320 616e 6420 616e 7920  inishes and any 
+0000f3e0: 6f75 7470 7574 7320 6861 7665 2062 6565  outputs have bee
+0000f3f0: 6e20 7570 6c6f 6164 6564 2e29 0a0a 4669  n uploaded.)..Fi
+0000f400: 6c65 7320 7468 6174 2061 7265 2064 6f77  les that are dow
+0000f410: 6e6c 6f61 6465 6420 6279 2074 6865 2041  nloaded by the A
+0000f420: 6765 6e74 2070 7269 6f72 2074 6f20 5461  gent prior to Ta
+0000f430: 736b 2065 7865 6375 7469 6f6e 2061 7265  sk execution are
+0000f440: 206c 6f63 6174 6564 2061 7320 666f 6c6c   located as foll
+0000f450: 6f77 733a 0a0a 312e 2049 6620 7468 6520  ows:..1. If the 
+0000f460: 6066 6c61 7474 656e 496e 7075 7450 6174  `flattenInputPat
+0000f470: 6873 6020 7072 6f70 6572 7479 2069 7320  hs` property is 
+0000f480: 7365 7420 746f 2074 6865 2064 6566 6175  set to the defau
+0000f490: 6c74 206f 6620 6066 616c 7365 6020 666f  lt of `false` fo
+0000f4a0: 7220 7468 6520 5461 736b 2c20 7468 6520  r the Task, the 
+0000f4b0: 646f 776e 6c6f 6164 6564 206f 626a 6563  downloaded objec
+0000f4c0: 7473 2061 7265 2070 6c61 6365 6420 696e  ts are placed in
+0000f4d0: 2073 7562 6469 7265 6374 6f72 6965 7320   subdirectories 
+0000f4e0: 7468 6174 206d 6972 726f 7220 7468 6f73  that mirror thos
+0000f4f0: 6520 696e 2074 6865 204f 626a 6563 7420  e in the Object 
+0000f500: 5374 6f72 652c 2069 6e63 6c75 6469 6e67  Store, including
+0000f510: 2074 6865 2057 6f72 6b20 5265 7175 6972   the Work Requir
+0000f520: 656d 656e 7420 6e61 6d65 2c20 7369 7475  ement name, situ
+0000f530: 6174 6564 2062 656e 6561 7468 2074 6865  ated beneath the
+0000f540: 2077 6f72 6b69 6e67 2064 6972 6563 746f   working directo
+0000f550: 7279 2e0a 0a0a 322e 2049 6620 7468 6520  ry....2. If the 
+0000f560: 6066 6c61 7474 656e 496e 7075 7450 6174  `flattenInputPat
+0000f570: 6873 6020 7072 6f70 6572 7479 2069 7320  hs` property is 
+0000f580: 7365 7420 746f 2060 7472 7565 6020 666f  set to `true` fo
+0000f590: 7220 7468 6520 5461 736b 2c20 7468 6520  r the Task, the 
+0000f5a0: 646f 776e 6c6f 6164 6564 206f 626a 6563  downloaded objec
+0000f5b0: 7473 2061 7265 2061 6c6c 2070 6c61 6365  ts are all place
+0000f5c0: 6420 6469 7265 6374 6c79 2069 6e20 726f  d directly in ro
+0000f5d0: 6f74 206f 6620 7468 6520 5461 736b 2773  ot of the Task's
+0000f5e0: 2077 6f72 6b69 6e67 2064 6972 6563 746f   working directo
+0000f5f0: 7279 2e0a 0a46 6f72 2065 7861 6d70 6c65  ry...For example
+0000f600: 3a0a 0a60 6060 7368 656c 6c0a 4966 2074  :..```shell.If t
+0000f610: 6865 2072 6571 7569 7265 6420 6f62 6a65  he required obje
+0000f620: 6374 2069 733a 2064 6576 656c 6f70 6d65  ct is: developme
+0000f630: 6e74 3a3a 7465 7374 7275 6e5f 3232 3131  nt::testrun_2211
+0000f640: 3038 2d31 3230 3430 342d 3764 322f 6465  08-120404-7d2/de
+0000f650: 762f 6669 6c65 5f31 2e74 7874 0a0a 7468  v/file_1.txt..th
+0000f660: 656e 2c20 6966 2066 6c61 7474 656e 496e  en, if flattenIn
+0000f670: 7075 7450 6174 6873 2069 7320 6661 6c73  putPaths is fals
+0000f680: 652c 2074 6865 2066 696c 6520 7769 6c6c  e, the file will
+0000f690: 2062 6520 666f 756e 6420 6174 3a0a 202d   be found at:. -
+0000f6a0: 3e20 3c77 6f72 6b69 6e67 5f64 6972 6563  > <working_direc
+0000f6b0: 746f 7279 3e2f 7465 7374 7275 6e5f 3232  tory>/testrun_22
+0000f6c0: 3131 3038 2d31 3230 3430 342d 3764 322f  1108-120404-7d2/
+0000f6d0: 6465 762f 6669 6c65 5f31 2e74 7874 0a20  dev/file_1.txt. 
+0000f6e0: 0a65 6c73 652c 2069 6620 666c 6174 7465  .else, if flatte
+0000f6f0: 6e49 6e70 7574 5061 7468 7320 6973 2074  nInputPaths is t
+0000f700: 7275 652c 2074 6865 2066 696c 6520 7769  rue, the file wi
+0000f710: 6c6c 2062 6520 666f 756e 6420 6174 3a0a  ll be found at:.
+0000f720: 202d 3e20 3c77 6f72 6b69 6e67 5f64 6972   -> <working_dir
+0000f730: 6563 746f 7279 3e2f 6669 6c65 5f31 2e74  ectory>/file_1.t
+0000f740: 7874 200a 200a 7768 6572 6520 3c77 6f72  xt . .where <wor
+0000f750: 6b69 6e67 5f64 6972 6563 746f 7279 3e20  king_directory> 
+0000f760: 6973 3a0a 2020 2f76 6172 2f6f 7074 2f79  is:.  /var/opt/y
+0000f770: 656c 6c6f 7764 6f67 2f79 642d 6167 656e  ellowdog/yd-agen
+0000f780: 742d 342f 6461 7461 2f77 6f72 6b65 7273  t-4/data/workers
+0000f790: 2f31 2f79 6469 645f 7461 736b 5f44 3044  /1/ydid_task_D0D
+0000f7a0: 3044 305f 3638 6635 6535 6265 2d64 6339  0D0_68f5e5be-dc9
+0000f7b0: 332d 3439 6562 2d61 3832 342d 3166 6364  3-49eb-a824-1fcd
+0000f7c0: 6235 3266 3931 3935 5f31 5f31 2f0a 6060  b52f9195_1_1/.``
+0000f7d0: 600a 0a4e 6f74 6520 7468 6174 2057 6f72  `..Note that Wor
+0000f7e0: 6b20 5265 7175 6972 656d 656e 7420 6e61  k Requirement na
+0000f7f0: 6d65 2028 652e 672e 2c20 6074 6573 7472  me (e.g., `testr
+0000f800: 756e 5f32 3231 3130 382d 3132 3034 3034  un_221108-120404
+0000f810: 2d37 6432 6029 2069 7320 6176 6169 6c61  -7d2`) is availa
+0000f820: 626c 6520 7669 6120 7468 6520 7661 7269  ble via the vari
+0000f830: 6162 6c65 2073 7562 7374 6974 7574 696f  able substitutio
+0000f840: 6e20 6077 725f 6e61 6d65 602c 2073 6f20  n `wr_name`, so 
+0000f850: 7468 6973 2063 6f75 6c64 2062 6520 7375  this could be su
+0000f860: 7070 6c69 6564 2074 6f20 7468 6520 5461  pplied to the Ta
+0000f870: 736b 2074 6f20 6865 6c70 2069 7420 6c6f  sk to help it lo
+0000f880: 6361 7465 2069 7473 2064 6f77 6e6c 6f61  cate its downloa
+0000f890: 6465 6420 6669 6c65 732e 2046 6f72 2065  ded files. For e
+0000f8a0: 7861 6d70 6c65 2c20 696e 2074 6865 2060  xample, in the `
+0000f8b0: 776f 726b 5265 7175 6972 656d 656e 7460  workRequirement`
+0000f8c0: 2073 6563 7469 6f6e 206f 6620 7468 6520   section of the 
+0000f8d0: 6063 6f6e 6669 672e 746f 6d6c 6020 6669  `config.toml` fi
+0000f8e0: 6c65 2c20 4920 636f 756c 6420 7370 6563  le, I could spec
+0000f8f0: 6966 793a 0a0a 6060 6074 6f6d 6c0a 656e  ify:..```toml.en
+0000f900: 7669 726f 6e6d 656e 7420 3d20 7b57 525f  vironment = {WR_
+0000f910: 4449 5245 4354 4f52 5920 3d20 227b 7b77  DIRECTORY = "{{w
+0000f920: 725f 6e61 6d65 7d7d 227d 0a60 6060 0a0a  r_name}}"}.```..
+0000f930: 5468 6520 576f 726b 2052 6571 7569 7265  The Work Require
+0000f940: 6d65 6e74 206e 616d 6520 776f 756c 6420  ment name would 
+0000f950: 7468 656e 2062 6520 6176 6169 6c61 626c  then be availabl
+0000f960: 6520 746f 2074 6865 2054 6173 6b20 696e  e to the Task in
+0000f970: 2074 6865 2065 6e76 6972 6f6e 6d65 6e74   the environment
+0000f980: 2076 6172 6961 626c 6520 6024 5752 5f44   variable `$WR_D
+0000f990: 4952 4543 544f 5259 602e 0a0a 2323 2320  IRECTORY`...### 
+0000f9a0: 4669 6c65 7320 5570 6c6f 6164 6564 2066  Files Uploaded f
+0000f9b0: 726f 6d20 6120 4e6f 6465 2074 6f20 7468  rom a Node to th
+0000f9c0: 6520 4f62 6a65 6374 2053 746f 7265 2061  e Object Store a
+0000f9d0: 6674 6572 2054 6173 6b20 4578 6563 7574  fter Task Execut
+0000f9e0: 696f 6e0a 0a41 6674 6572 2054 6173 6b20  ion..After Task 
+0000f9f0: 636f 6d70 6c65 7469 6f6e 2c20 7468 6520  completion, the 
+0000fa00: 4167 656e 7420 7769 6c6c 2075 706c 6f61  Agent will uploa
+0000fa10: 6420 7370 6563 6966 6965 6420 6f75 7470  d specified outp
+0000fa20: 7574 2066 696c 6573 2074 6f20 7468 6520  ut files to the 
+0000fa30: 4f62 6a65 6374 2053 746f 7265 2e20 5468  Object Store. Th
+0000fa40: 6520 6669 6c65 7320 746f 2062 6520 7570  e files to be up
+0000fa50: 6c6f 6164 6564 2061 7265 2074 686f 7365  loaded are those
+0000fa60: 206c 6973 7465 6420 696e 2074 6865 2060   listed in the `
+0000fa70: 6f75 7470 7574 7360 2061 6e64 2060 6f75  outputs` and `ou
+0000fa80: 7470 7574 7352 6571 7569 7265 6460 2070  tputsRequired` p
+0000fa90: 726f 7065 7274 6965 7320 666f 7220 7468  roperties for th
+0000faa0: 6520 5461 736b 2e0a 0a49 6e20 6164 6469  e Task...In addi
+0000fab0: 7469 6f6e 2c20 7468 6520 636f 6e73 6f6c  tion, the consol
+0000fac0: 6520 6f75 7470 7574 206f 6620 7468 6520  e output of the 
+0000fad0: 5461 736b 2069 7320 6361 7074 7572 6564  Task is captured
+0000fae0: 2069 6e20 6120 6669 6c65 2063 616c 6c65   in a file calle
+0000faf0: 6420 6074 6173 6b6f 7574 7075 742e 7478  d `taskoutput.tx
+0000fb00: 7460 2069 6e20 7468 6520 726f 6f74 206f  t` in the root o
+0000fb10: 6620 7468 6520 5461 736b 2773 2077 6f72  f the Task's wor
+0000fb20: 6b69 6e67 2064 6972 6563 746f 7279 2e20  king directory. 
+0000fb30: 5768 6574 6865 7220 7468 6520 6074 6173  Whether the `tas
+0000fb40: 6b6f 7574 7075 742e 7478 7460 2066 696c  koutput.txt` fil
+0000fb50: 6520 6973 2075 706c 6f61 6465 6420 746f  e is uploaded to
+0000fb60: 2074 6865 204f 626a 6563 7420 5374 6f72   the Object Stor
+0000fb70: 6520 6973 2064 6574 6572 6d69 6e65 6420  e is determined 
+0000fb80: 6279 2074 6865 2060 6361 7074 7572 6554  by the `captureT
+0000fb90: 6173 6b4f 7574 7075 7460 2070 726f 7065  askOutput` prope
+0000fba0: 7274 7920 666f 7220 7468 6520 5461 736b  rty for the Task
+0000fbb0: 2c20 616e 6420 7468 6973 2069 7320 7365  , and this is se
+0000fbc0: 7420 746f 2027 7472 7565 2720 6279 2064  t to 'true' by d
+0000fbd0: 6566 6175 6c74 2e0a 0a49 6620 5461 736b  efault...If Task
+0000fbe0: 206f 7574 7075 7473 2061 7265 2063 7265   outputs are cre
+0000fbf0: 6174 6564 2069 6e20 7375 6264 6972 6563  ated in subdirec
+0000fc00: 746f 7269 6573 2062 656c 6f77 2074 6865  tories below the
+0000fc10: 2054 6173 6b27 7320 776f 726b 696e 6720   Task's working 
+0000fc20: 6469 7265 6374 6f72 792c 2069 6e63 6c75  directory, inclu
+0000fc30: 6465 2074 6865 2064 6972 6563 746f 7269  de the directori
+0000fc40: 6573 2066 6f72 2066 696c 6573 2069 6e20  es for files in 
+0000fc50: 7468 6520 606f 7574 7075 7473 6020 7072  the `outputs` pr
+0000fc60: 6f70 6572 7479 2e20 452e 672e 2c20 6966  operty. E.g., if
+0000fc70: 2061 2054 6173 6b20 6372 6561 7465 7320   a Task creates 
+0000fc80: 6669 6c65 7320 6072 6573 756c 7473 2f6f  files `results/o
+0000fc90: 7065 6e66 6f61 6d2e 7461 722e 677a 6020  penfoam.tar.gz` 
+0000fca0: 616e 6420 6072 6573 756c 7473 2f6f 7065  and `results/ope
+0000fcb0: 6e66 6f61 6d2e 6c6f 6760 2c20 7468 656e  nfoam.log`, then
+0000fcc0: 2073 7065 6369 6679 2074 6865 7365 2066   specify these f
+0000fcd0: 6f72 2075 706c 6f61 6420 696e 2074 6865  or upload in the
+0000fce0: 2060 6f75 7470 7574 7360 2070 726f 7065   `outputs` prope
+0000fcf0: 7274 7920 6173 2066 6f6c 6c6f 7773 3a0a  rty as follows:.
+0000fd00: 0a60 226f 7574 7075 7473 223a 205b 2272  .`"outputs": ["r
+0000fd10: 6573 756c 7473 2f6f 7065 6e66 6f61 6d2e  esults/openfoam.
+0000fd20: 7461 722e 677a 222c 2022 7265 7375 6c74  tar.gz", "result
+0000fd30: 732f 6f70 656e 666f 616d 2e6c 6f67 225d  s/openfoam.log"]
+0000fd40: 600a 0a57 6865 6e20 6f75 7470 7574 2066  `..When output f
+0000fd50: 696c 6573 2061 7265 2075 706c 6f61 6465  iles are uploade
+0000fd60: 6420 746f 2074 6865 204f 626a 6563 7420  d to the Object 
+0000fd70: 5374 6f72 652c 2074 6865 7920 6172 6520  Store, they are 
+0000fd80: 706c 6163 6564 2069 6e20 6120 5461 736b  placed in a Task
+0000fd90: 2047 726f 7570 2061 6e64 2054 6173 6b20   Group and Task 
+0000fda0: 7370 6563 6966 6963 2064 6972 6563 746f  specific directo
+0000fdb0: 7279 2e20 536f 2c20 6966 2074 6865 204e  ry. So, if the N
+0000fdc0: 616d 6573 7061 6365 2069 7320 6064 6576  amespace is `dev
+0000fdd0: 656c 6f70 6d65 6e74 602c 2074 6865 2057  elopment`, the W
+0000fde0: 6f72 6b20 5265 7175 6972 656d 656e 7420  ork Requirement 
+0000fdf0: 6973 2060 7465 7374 7275 6e5f 3232 3131  is `testrun_2211
+0000fe00: 3038 2d31 3230 3430 342d 3764 3260 2c20  08-120404-7d2`, 
+0000fe10: 7468 6520 5461 736b 2047 726f 7570 2069  the Task Group i
+0000fe20: 7320 6074 6173 6b5f 6772 6f75 705f 3160  s `task_group_1`
+0000fe30: 2061 6e64 2074 6865 2054 6173 6b20 6973   and the Task is
+0000fe40: 2060 7461 736b 5f31 602c 2074 6865 6e20   `task_1`, then 
+0000fe50: 7468 6520 6669 6c65 7320 6162 6f76 6520  the files above 
+0000fe60: 776f 756c 6420 6265 2075 706c 6f61 6465  would be uploade
+0000fe70: 6420 746f 2074 6865 204f 626a 6563 7420  d to the Object 
+0000fe80: 5374 6f72 6520 6173 2066 6f6c 6c6f 7773  Store as follows
+0000fe90: 3a0a 0a60 6060 7368 656c 6c0a 6465 7665  :..```shell.deve
+0000fea0: 6c6f 706d 656e 743a 3a74 6573 7472 756e  lopment::testrun
+0000feb0: 5f32 3231 3130 382d 3132 3034 3034 2d37  _221108-120404-7
+0000fec0: 6432 2f74 6173 6b5f 6772 6f75 705f 312f  d2/task_group_1/
+0000fed0: 7461 736b 5f31 2f72 6573 756c 7473 2f6f  task_1/results/o
+0000fee0: 7065 6e66 6f61 6d2e 7461 722e 677a 0a64  penfoam.tar.gz.d
+0000fef0: 6576 656c 6f70 6d65 6e74 3a3a 7465 7374  evelopment::test
+0000ff00: 7275 6e5f 3232 3131 3038 2d31 3230 3430  run_221108-12040
+0000ff10: 342d 3764 322f 7461 736b 5f67 726f 7570  4-7d2/task_group
+0000ff20: 5f31 2f74 6173 6b5f 312f 7265 7375 6c74  _1/task_1/result
+0000ff30: 732f 6f70 656e 666f 616d 2e6c 6f67 0a64  s/openfoam.log.d
+0000ff40: 6576 656c 6f70 6d65 6e74 3a3a 7465 7374  evelopment::test
+0000ff50: 7275 6e5f 3232 3131 3038 2d31 3230 3430  run_221108-12040
+0000ff60: 342d 3764 322f 7461 736b 5f67 726f 7570  4-7d2/task_group
+0000ff70: 5f31 2f74 6173 6b5f 312f 7461 736b 6f75  _1/task_1/taskou
+0000ff80: 7470 7574 2e74 7874 0a60 6060 0a0a 5468  tput.txt.```..Th
+0000ff90: 6520 2a2a 606f 7574 7075 7473 5265 7175  e **`outputsRequ
+0000ffa0: 6972 6564 602a 2a20 7072 6f70 6572 7479  ired`** property
+0000ffb0: 2063 616e 2062 6520 7573 6564 2069 6e73   can be used ins
+0000ffc0: 7465 6164 206f 6620 286f 7220 696e 2061  tead of (or in a
+0000ffd0: 6464 6974 696f 6e20 746f 2920 7468 6520  ddition to) the 
+0000ffe0: 606f 7574 7075 7473 6020 7072 6f70 6572  `outputs` proper
+0000fff0: 7479 2c20 6966 2074 6865 206f 7574 7075  ty, if the outpu
+00010000: 7420 6669 6c65 2873 2920 2a2a 6d75 7374  t file(s) **must
+00010010: 2a2a 2062 6520 6176 6169 6c61 626c 6520  ** be available 
+00010020: 666f 7220 7570 6c6f 6164 2074 6f20 7468  for upload to th
+00010030: 6520 4f62 6a65 6374 2053 746f 7265 2061  e Object Store a
+00010040: 7420 7468 6520 636f 6e63 6c75 7369 6f6e  t the conclusion
+00010050: 206f 6620 7468 6520 5461 736b 206f 7220   of the Task or 
+00010060: 7468 6520 5461 736b 2077 696c 6c20 6265  the Task will be
+00010070: 206d 6172 6b65 6420 6173 2060 4661 696c   marked as `Fail
+00010080: 6564 602c 2065 2e67 2e3a 0a0a 6022 6f75  ed`, e.g.:..`"ou
+00010090: 7470 7574 7352 6571 7569 7265 6422 3a20  tputsRequired": 
+000100a0: 5b22 7265 7375 6c74 732f 7072 6f63 6573  ["results/proces
+000100b0: 735f 6f75 7470 7574 2e74 7874 225d 600a  s_output.txt"]`.
+000100c0: 0a23 2323 2046 696c 6573 2044 6f77 6e6c  .### Files Downl
+000100d0: 6f61 6465 6420 6672 6f6d 2074 6865 204f  oaded from the O
+000100e0: 626a 6563 7420 5374 6f72 6520 746f 204c  bject Store to L
+000100f0: 6f63 616c 2053 746f 7261 6765 0a0a 5468  ocal Storage..Th
+00010100: 6520 6079 642d 646f 776e 6c6f 6164 6020  e `yd-download` 
+00010110: 636f 6d6d 616e 6420 7769 6c6c 2064 6f77  command will dow
+00010120: 6e6c 6f61 6420 616c 6c20 6f62 6a65 6374  nload all object
+00010130: 7320 6672 6f6d 2074 6865 204f 626a 6563  s from the Objec
+00010140: 7420 5374 6f72 6520 746f 2061 206c 6f63  t Store to a loc
+00010150: 616c 2064 6972 6563 746f 7279 2c20 6f6e  al directory, on
+00010160: 2061 2070 6572 2057 6f72 6b20 5265 7175   a per Work Requ
+00010170: 6972 656d 656e 7420 6261 7369 7320 2869  irement basis (i
+00010180: 6e63 6c75 6469 6e67 2061 6e79 2066 696c  ncluding any fil
+00010190: 6573 2074 6861 7420 6861 7665 2062 6565  es that have bee
+000101a0: 6e20 7570 6c6f 6164 6564 292e 2041 206c  n uploaded). A l
+000101b0: 6f63 616c 2064 6972 6563 746f 7279 2069  ocal directory i
+000101c0: 7320 6372 6561 7465 6420 7769 7468 2074  s created with t
+000101d0: 6865 2073 616d 6520 6e61 6d65 2061 7320  he same name as 
+000101e0: 7468 6520 4e61 6d65 7370 6163 6520 616e  the Namespace an
+000101f0: 6420 636f 6e74 6169 6e69 6e67 2074 6865  d containing the
+00010200: 2057 6f72 6b20 5265 7175 6972 656d 656e   Work Requiremen
+00010210: 7420 6469 7265 6374 6f72 6965 732e 0a0a  t directories...
+00010220: 5573 6520 7468 6520 602d 2d69 6e74 6572  Use the `--inter
+00010230: 6163 7469 7665 6020 6f70 7469 6f6e 2077  active` option w
+00010240: 6974 6820 6079 642d 646f 776e 6c6f 6164  ith `yd-download
+00010250: 6020 746f 2073 656c 6563 7420 7768 6963  ` to select whic
+00010260: 6820 576f 726b 2052 6571 7569 7265 6d65  h Work Requireme
+00010270: 6e74 2873 2920 746f 2064 6f77 6e6c 6f61  nt(s) to downloa
+00010280: 642e 0a0a 466f 7220 7468 6520 6578 616d  d...For the exam
+00010290: 706c 6520 6162 6f76 652c 2060 7964 2d64  ple above, `yd-d
+000102a0: 6f77 6e6c 6f61 6460 2077 6f75 6c64 2063  ownload` would c
+000102b0: 7265 6174 6520 6120 6469 7265 6374 6f72  reate a director
+000102c0: 7920 6361 6c6c 6564 2060 6465 7665 6c6f  y called `develo
+000102d0: 706d 656e 7460 2069 6e20 7468 6520 6375  pment` in the cu
+000102e0: 7272 656e 7420 776f 726b 696e 6720 6469  rrent working di
+000102f0: 7265 6374 6f72 792c 2063 6f6e 7461 696e  rectory, contain
+00010300: 696e 6720 736f 6d65 7468 696e 6720 6c69  ing something li
+00010310: 6b65 3a0a 0a60 6060 7368 656c 6c0a 6465  ke:..```shell.de
+00010320: 7665 6c6f 706d 656e 740a e294 94e2 9480  velopment.......
+00010330: e294 8020 7465 7374 7275 6e5f 3232 3131  ... testrun_2211
+00010340: 3038 2d31 3230 3430 342d 3764 320a 2020  08-120404-7d2.  
+00010350: 2020 e294 9ce2 9480 e294 8020 6261 7368    ......... bash
+00010360: 5f73 6372 6970 742e 7368 0a20 2020 20e2  _script.sh.    .
+00010370: 949c e294 80e2 9480 2066 696c 655f 312e  ........ file_1.
+00010380: 7478 740a 2020 2020 e294 94e2 9480 e294  txt.    ........
+00010390: 8020 7461 736b 5f67 726f 7570 5f31 0a20  . task_group_1. 
+000103a0: 2020 2020 2020 20e2 9494 e294 80e2 9480         .........
+000103b0: 2074 6173 6b5f 310a 2020 2020 2020 2020   task_1.        
+000103c0: 2020 2020 e294 9ce2 9480 e294 8020 7265      ......... re
+000103d0: 7375 6c74 730a 2020 2020 2020 2020 2020  sults.          
+000103e0: 2020 e294 82c2 a0c2 a020 e294 9ce2 9480    ....... ......
+000103f0: e294 8020 6f70 656e 666f 616d 2e6c 6f67  ... openfoam.log
+00010400: 0a20 2020 2020 2020 2020 2020 20e2 9482  .            ...
+00010410: c2a0 c2a0 20e2 9494 e294 80e2 9480 206f  .... ......... o
+00010420: 7065 6e66 6f61 6d2e 7461 722e 677a 0a20  penfoam.tar.gz. 
+00010430: 2020 2020 2020 2020 2020 20e2 9494 e294             .....
+00010440: 80e2 9480 2074 6173 6b6f 7574 7075 742e  .... taskoutput.
+00010450: 7478 740a 6060 600a 0a4e 6f74 6520 7468  txt.```..Note th
+00010460: 6174 2065 7665 7279 7468 696e 6720 7769  at everything wi
+00010470: 7468 696e 2074 6865 2060 6e61 6d65 7370  thin the `namesp
+00010480: 6163 653a 3a77 6f72 6b2d 7265 7175 6972  ace::work-requir
+00010490: 656d 656e 7460 2064 6972 6563 746f 7279  ement` directory
+000104a0: 2069 6e20 7468 6520 4f62 6a65 6374 2053   in the Object S
+000104b0: 746f 7265 2069 7320 646f 776e 6c6f 6164  tore is download
+000104c0: 6564 2c20 696e 636c 7564 696e 6720 616e  ed, including an
+000104d0: 7920 6669 6c65 7320 7468 6174 2077 6572  y files that wer
+000104e0: 6520 7370 6563 6966 6965 6420 696e 2060  e specified in `
+000104f0: 696e 7075 7473 6020 616e 6420 7570 6c6f  inputs` and uplo
+00010500: 6164 6564 2061 7320 7061 7274 206f 6620  aded as part of 
+00010510: 7468 6520 576f 726b 2052 6571 7569 7265  the Work Require
+00010520: 6d65 6e74 2073 7562 6d69 7373 696f 6e2e  ment submission.
+00010530: 204d 756c 7469 706c 6520 5461 736b 2047   Multiple Task G
+00010540: 726f 7570 732c 2061 6e64 206d 756c 7469  roups, and multi
+00010550: 706c 6520 5461 736b 7320 7769 6c6c 2061  ple Tasks will a
+00010560: 6c6c 2061 7070 6561 7220 696e 2074 6865  ll appear in the
+00010570: 2064 6972 6563 746f 7279 2073 7472 7563   directory struc
+00010580: 7475 7265 2e0a 0a49 6620 7468 6520 6064  ture...If the `d
+00010590: 6576 656c 6f70 6d65 6e74 6020 6469 7265  evelopment` dire
+000105a0: 6374 6f72 7920 616c 7265 6164 7920 6578  ctory already ex
+000105b0: 6973 7473 2c20 6079 642d 646f 776e 6c6f  ists, `yd-downlo
+000105c0: 6164 6020 7769 6c6c 2074 7279 2060 6465  ad` will try `de
+000105d0: 7665 6c6f 706d 656e 742e 3031 602c 2065  velopment.01`, e
+000105e0: 7463 2e2c 2074 6f20 6176 6f69 6420 6f76  tc., to avoid ov
+000105f0: 6572 7772 6974 696e 6720 7072 6576 696f  erwriting previo
+00010600: 7573 2064 6f77 6e6c 6f61 6473 2e0a 0a23  us downloads...#
+00010610: 2320 5461 736b 2045 7865 6375 7469 6f6e  # Task Execution
+00010620: 2043 6f6e 7465 7874 0a0a 5468 6973 2073   Context..This s
+00010630: 6563 7469 6f6e 2064 6973 6375 7373 6573  ection discusses
+00010640: 2074 6865 2063 6f6e 7465 7874 2077 6974   the context wit
+00010650: 6869 6e20 7768 6963 6820 6120 5461 736b  hin which a Task
+00010660: 206f 7065 7261 7465 7320 7768 656e 2069   operates when i
+00010670: 7427 7320 6578 6563 7574 6564 2062 7920  t's executed by 
+00010680: 6120 576f 726b 6572 206f 6e20 6120 6e6f  a Worker on a no
+00010690: 6465 2e20 4974 2061 7070 6c69 6573 2073  de. It applies s
+000106a0: 7065 6369 6669 6361 6c6c 7920 746f 2074  pecifically to t
+000106b0: 6865 2059 656c 6c6f 7744 6f67 2041 6765  he YellowDog Age
+000106c0: 6e74 2072 756e 6e69 6e67 206f 6e20 6120  nt running on a 
+000106d0: 4c69 6e75 7820 6e6f 6465 2c20 616e 6420  Linux node, and 
+000106e0: 636f 6e66 6967 7572 6564 2075 7369 6e67  configured using
+000106f0: 2074 6865 2064 6566 6175 6c74 2075 7365   the default use
+00010700: 726e 616d 652c 2064 6972 6563 746f 7269  rname, directori
+00010710: 6573 2c20 6574 632e 2043 6f6e 6669 6775  es, etc. Configu
+00010720: 7261 7469 6f6e 7320 6361 6e20 7661 7279  rations can vary
+00010730: 2e0a 0a23 2323 2054 6173 6b20 4578 6563  ...### Task Exec
+00010740: 7574 696f 6e20 5374 6570 730a 0a57 6865  ution Steps..Whe
+00010750: 6e20 6120 5461 736b 2069 7320 616c 6c6f  n a Task is allo
+00010760: 6361 7465 6420 746f 2061 2057 6f72 6b65  cated to a Worke
+00010770: 7220 6f6e 2061 206e 6f64 6520 6279 2074  r on a node by t
+00010780: 6865 2059 656c 6c6f 7744 6f67 2053 6368  he YellowDog Sch
+00010790: 6564 756c 6572 2c20 7468 6520 666f 6c6c  eduler, the foll
+000107a0: 6f77 696e 6720 7374 6570 7320 6172 6520  owing steps are 
+000107b0: 666f 6c6c 6f77 6564 3a0a 0a31 2e20 5468  followed:..1. Th
+000107c0: 6520 4167 656e 7420 7275 6e6e 696e 6720  e Agent running 
+000107d0: 6f6e 2074 6865 206e 6f64 6520 646f 776e  on the node down
+000107e0: 6c6f 6164 7320 7468 6520 5461 736b 2773  loads the Task's
+000107f0: 2070 726f 7065 7274 6965 733a 2069 7473   properties: its
+00010800: 2060 7461 736b 5479 7065 602c 2020 6061   `taskType`,  `a
+00010810: 7267 756d 656e 7473 602c 2060 656e 7669  rguments`, `envi
+00010820: 726f 6e6d 656e 7460 2c20 6074 6173 6b64  ronment`, `taskd
+00010830: 6174 6160 2c20 616e 6420 2866 726f 6d20  ata`, and (from 
+00010840: 7468 6520 4f62 6a65 6374 2053 746f 7265  the Object Store
+00010850: 2920 616e 7920 6669 6c65 7320 696e 2074  ) any files in t
+00010860: 6865 2060 696e 7075 7473 6020 6c69 7374  he `inputs` list
+00010870: 2061 6e64 2061 6e79 2061 7661 696c 6162   and any availab
+00010880: 6c65 2066 696c 6573 2069 6e20 7468 6520  le files in the 
+00010890: 6069 6e70 7574 734f 7074 696f 6e61 6c60  `inputsOptional`
+000108a0: 206c 6973 742e 0a32 2e20 5468 6573 6520   list..2. These 
+000108b0: 6669 6c65 7320 6172 6520 706c 6163 6564  files are placed
+000108c0: 2069 6e20 616e 2065 7068 656d 6572 616c   in an ephemeral
+000108d0: 2064 6972 6563 746f 7279 2063 7265 6174   directory creat
+000108e0: 6564 2066 6f72 2074 6869 7320 5461 736b  ed for this Task
+000108f0: 2773 2065 7865 6375 7469 6f6e 2c20 616e  's execution, an
+00010900: 6420 696e 746f 2077 6869 6368 2061 6e79  d into which any
+00010910: 206f 7574 7075 7420 6669 6c65 7320 6172   output files ar
+00010920: 6520 616c 736f 2070 6c61 6365 6420 6279  e also placed by
+00010930: 2064 6566 6175 6c74 2e0a 322e 2054 6865   default..2. The
+00010940: 2041 6765 6e74 2072 756e 7320 7468 6520   Agent runs the 
+00010950: 636f 6d6d 616e 6420 7370 6563 6966 6965  command specifie
+00010960: 6420 666f 7220 7468 6520 6074 6173 6b54  d for the `taskT
+00010970: 7970 6560 2069 6e20 7468 6520 4167 656e  ype` in the Agen
+00010980: 7427 7320 6061 7070 6c69 6361 7469 6f6e  t's `application
+00010990: 2e79 616d 6c60 2063 6f6e 6669 6775 7261  .yaml` configura
+000109a0: 7469 6f6e 2066 696c 652e 2054 6869 7320  tion file. This 
+000109b0: 646f 6e65 2061 7320 6120 7369 6d70 6c65  done as a simple
+000109c0: 2060 6578 6563 6020 6f66 2061 2073 7562   `exec` of a sub
+000109d0: 7072 6f63 6573 732e 0a33 2e20 5768 656e  process..3. When
+000109e0: 2074 6865 2054 6173 6b20 636f 6e63 6c75   the Task conclu
+000109f0: 6465 732c 2074 6865 2041 6765 6e74 2075  des, the Agent u
+00010a00: 7365 7320 7468 6520 6578 6974 2063 6f64  ses the exit cod
+00010a10: 6520 6f66 2074 6865 2073 7562 7072 6f63  e of the subproc
+00010a20: 6573 7320 746f 2072 6570 6f72 7420 7375  ess to report su
+00010a30: 6363 6573 7320 287a 6572 6f29 206f 7220  ccess (zero) or 
+00010a40: 6661 696c 7572 6520 286e 6f6e 2d7a 6572  failure (non-zer
+00010a50: 6f29 2e0a 342e 2054 6865 2041 6765 6e74  o)..4. The Agent
+00010a60: 2074 6865 6e20 6761 7468 6572 7320 616e   then gathers an
+00010a70: 7920 6669 6c65 7320 696e 2074 6865 2060  y files in the `
+00010a80: 6f75 7470 7574 7360 2061 6e64 2060 6f75  outputs` and `ou
+00010a90: 7470 7574 7352 6571 7569 7265 6460 206c  tputsRequired` l
+00010aa0: 6973 7473 2061 6e64 2075 706c 6f61 6473  ists and uploads
+00010ab0: 2074 6865 6d20 746f 2074 6865 204f 626a   them to the Obj
+00010ac0: 6563 7420 5374 6f72 652e 2049 6620 6120  ect Store. If a 
+00010ad0: 6669 6c65 2069 6e20 7468 6520 606f 7574  file in the `out
+00010ae0: 7075 7473 5265 7175 6972 6564 6020 6c69  putsRequired` li
+00010af0: 7374 2069 7320 6e6f 7420 666f 756e 642c  st is not found,
+00010b00: 2074 6865 2054 6173 6b20 7769 6c6c 2062   the Task will b
+00010b10: 6520 7265 706f 7274 6564 2061 7320 6661  e reported as fa
+00010b20: 696c 6564 2e20 5468 6520 4167 656e 7420  iled. The Agent 
+00010b30: 7769 6c6c 2061 6c73 6f20 6f70 7469 6f6e  will also option
+00010b40: 616c 6c79 2075 706c 6f61 6420 7468 6520  ally upload the 
+00010b50: 636f 6e73 6f6c 6520 6f75 7470 7574 2028  console output (
+00010b60: 696e 636c 7564 696e 6720 626f 7468 2060  including both `
+00010b70: 7374 646f 7574 6020 616e 6420 6073 7464  stdout` and `std
+00010b80: 6572 7260 2920 6f66 2074 6865 2054 6173  err`) of the Tas
+00010b90: 6b2c 2063 6f6e 7461 696e 6564 2069 6e20  k, contained in 
+00010ba0: 7468 6520 6074 6173 6b6f 7574 7075 742e  the `taskoutput.
+00010bb0: 7478 7460 2066 696c 652e 0a35 2e20 5468  txt` file..5. Th
+00010bc0: 6520 6570 6865 6d65 7261 6c20 5461 736b  e ephemeral Task
+00010bd0: 2064 6972 6563 746f 7279 2069 7320 7468   directory is th
+00010be0: 656e 2064 656c 6574 6564 2e0a 0a4e 6f74  en deleted...Not
+00010bf0: 6520 7468 6174 2069 6620 6120 5461 736b  e that if a Task
+00010c00: 2069 7320 6162 6f72 7465 6420 6475 7269   is aborted duri
+00010c10: 6e67 2065 7865 6375 7469 6f6e 2c20 7468  ng execution, th
+00010c20: 6520 5461 736b 2773 2073 7562 7072 6f63  e Task's subproc
+00010c30: 6573 7320 6973 2073 656e 7420 6120 6053  ess is sent a `S
+00010c40: 4947 494e 5460 2c20 616c 6c6f 7769 6e67  IGINT`, allowing
+00010c50: 2074 6865 2054 6173 6b20 616e 206f 7070   the Task an opp
+00010c60: 6f72 7475 6e69 7479 2074 6f20 7465 726d  ortunity to term
+00010c70: 696e 6174 6520 616e 7920 6368 696c 6420  inate any child 
+00010c80: 7072 6f63 6573 7365 7320 6f72 206f 7468  processes or oth
+00010c90: 6572 2072 6573 6f75 7263 6573 2028 652e  er resources (e.
+00010ca0: 672e 2c20 636f 6e74 6169 6e65 7273 2920  g., containers) 
+00010cb0: 7468 6174 206d 6179 2068 6176 6520 6265  that may have be
+00010cc0: 656e 2073 7461 7274 6564 2061 7320 7061  en started as pa
+00010cd0: 7274 206f 6620 5461 736b 2065 7865 6375  rt of Task execu
+00010ce0: 7469 6f6e 2e0a 0a4f 6e63 6520 7468 6520  tion...Once the 
+00010cf0: 7374 6570 7320 6162 6f76 6520 6861 7665  steps above have
+00010d00: 2062 6565 6e20 636f 6d70 6c65 7465 642c   been completed,
+00010d10: 2074 6865 2057 6f72 6b65 7220 6973 2072   the Worker is r
+00010d20: 6561 6479 2074 6f20 6163 6365 7074 2069  eady to accept i
+00010d30: 7473 206e 6578 7420 5461 736b 2066 726f  ts next Task fro
+00010d40: 6d20 7468 6520 5965 6c6c 6f77 446f 6720  m the YellowDog 
+00010d50: 7363 6865 6475 6c65 722e 0a0a 4e6f 7465  scheduler...Note
+00010d60: 2074 6861 7420 6966 2074 6865 2041 6765   that if the Age
+00010d70: 6e74 206f 6e20 6120 6e6f 6465 2068 6173  nt on a node has
+00010d80: 206d 756c 7469 706c 6520 576f 726b 6572   multiple Worker
+00010d90: 732c 2074 6865 6e20 5461 736b 7320 6172  s, then Tasks ar
+00010da0: 6520 6578 6563 7574 6564 2069 6e20 7061  e executed in pa
+00010db0: 7261 6c6c 656c 206f 6e20 7468 6520 6e6f  rallel on the no
+00010dc0: 6465 2061 6e64 2063 616e 2073 7461 7274  de and can start
+00010dd0: 2061 6e64 2073 746f 7020 696e 6465 7065   and stop indepe
+00010de0: 6e64 656e 746c 792e 0a0a 2323 2320 5468  ndently...### Th
+00010df0: 6520 5573 6572 2061 6e64 2047 726f 7570  e User and Group
+00010e00: 2075 7365 6420 666f 7220 5461 736b 730a   used for Tasks.
+00010e10: 0a42 7920 6465 6661 756c 742c 2074 6865  .By default, the
+00010e20: 2041 6765 6e74 2072 756e 7320 6173 2075   Agent runs as u
+00010e30: 7365 7220 616e 6420 6772 6f75 7020 6079  ser and group `y
+00010e40: 642d 6167 656e 7460 2c20 616e 6420 6865  d-agent`, and he
+00010e50: 6e63 6520 5461 736b 7320 616c 736f 2065  nce Tasks also e
+00010e60: 7865 6375 7465 2075 6e64 6572 2074 6869  xecute under thi
+00010e70: 7320 7573 6572 2e0a 0a60 7964 2d61 6765  s user...`yd-age
+00010e80: 6e74 6020 646f 6573 206e 6f74 2068 6176  nt` does not hav
+00010e90: 6520 6073 7564 6f60 2070 7269 7669 6c65  e `sudo` privile
+00010ea0: 6765 7320 6173 2073 7461 6e64 6172 642c  ges as standard,
+00010eb0: 2062 7574 2074 6869 7320 6361 6e20 6265   but this can be
+00010ec0: 2061 6464 6564 2069 6620 7265 7175 6972   added if requir
+00010ed0: 6564 2061 7420 696e 7374 616e 6365 2062  ed at instance b
+00010ee0: 6f6f 7420 7469 6d65 2076 6961 2074 6865  oot time via the
+00010ef0: 2060 7573 6572 4461 7461 6020 7072 6f70   `userData` prop
+00010f00: 6572 7479 206f 6620 6120 7072 6f76 6973  erty of a provis
+00010f10: 696f 6e69 6e67 2072 6571 7565 7374 2e20  ioning request. 
+00010f20: 452e 672e 2028 666f 7220 5562 756e 7475  E.g. (for Ubuntu
+00010f30: 293a 0a0a 6060 6073 6865 6c6c 0a75 7365  ):..```shell.use
+00010f40: 726d 6f64 202d 6147 2077 6865 656c 2079  rmod -aG wheel y
+00010f50: 642d 6167 656e 740a 6563 686f 202d 6520  d-agent.echo -e 
+00010f60: 2279 642d 6167 656e 745c 7441 4c4c 3d28  "yd-agent\tALL=(
+00010f70: 414c 4c29 5c74 4e4f 5041 5353 5744 3a20  ALL)\tNOPASSWD: 
+00010f80: 414c 4c22 203e 202f 6574 632f 7375 646f  ALL" > /etc/sudo
+00010f90: 6572 732e 642f 3032 302d 7964 2d61 6765  ers.d/020-yd-age
+00010fa0: 6e74 0a60 6060 0a0a 2323 2320 486f 6d65  nt.```..### Home
+00010fb0: 2044 6972 6563 746f 7279 2066 6f72 2060   Directory for `
+00010fc0: 7964 2d61 6765 6e74 600a 0a42 7920 6465  yd-agent`..By de
+00010fd0: 6661 756c 742c 2074 6865 2068 6f6d 6520  fault, the home 
+00010fe0: 6469 7265 6374 6f72 7920 6f66 2074 6865  directory of the
+00010ff0: 2060 7964 2d61 6765 6e74 6020 7573 6572   `yd-agent` user
+00011000: 2069 7320 602f 6f70 742f 7965 6c6c 6f77   is `/opt/yellow
+00011010: 646f 672f 6167 656e 7460 2e20 5468 6973  dog/agent`. This
+00011020: 2064 6972 6563 746f 7279 2074 7970 6963   directory typic
+00011030: 616c 6c79 2063 6f6e 7461 696e 7320 7468  ally contains th
+00011040: 6520 6061 7070 6c69 6361 7469 6f6e 2e79  e `application.y
+00011050: 616d 6c60 2066 696c 6520 7573 6564 2074  aml` file used t
+00011060: 6f20 636f 6e66 6967 7572 6520 7468 6520  o configure the 
+00011070: 4167 656e 742c 2061 7320 7765 6c6c 2061  Agent, as well a
+00011080: 7320 616e 7920 7363 7269 7074 7320 7468  s any scripts th
+00011090: 6174 2061 7265 2075 7365 6420 746f 2065  at are used to e
+000110a0: 7865 6375 7465 2074 6865 2054 6173 6b20  xecute the Task 
+000110b0: 5479 7065 7320 7468 6174 2074 6865 206e  Types that the n
+000110c0: 6f64 6520 7375 7070 6f72 7473 2e0a 0a49  ode supports...I
+000110d0: 6620 6f6e 6520 7761 6e74 7320 746f 2053  f one wants to S
+000110e0: 5348 2074 6f20 616e 2069 6e73 7461 6e63  SH to an instanc
+000110f0: 6520 6173 2075 7365 7220 6079 642d 6167  e as user `yd-ag
+00011100: 656e 7460 2c20 7065 7268 6170 7320 666f  ent`, perhaps fo
+00011110: 7220 6465 6275 6767 696e 6720 7075 7270  r debugging purp
+00011120: 6f73 6573 2c20 5353 4820 6b65 7973 2063  oses, SSH keys c
+00011130: 616e 2062 6520 696e 7365 7274 6564 2076  an be inserted v
+00011140: 6961 2069 6e73 7461 6e63 6520 6075 7365  ia instance `use
+00011150: 7244 6174 6160 2c20 652e 672e 3a0a 0a60  rData`, e.g.:..`
+00011160: 6060 7368 656c 6c0a 5944 415f 484f 4d45  ``shell.YDA_HOME
+00011170: 3d2f 6f70 742f 7965 6c6c 6f77 646f 672f  =/opt/yellowdog/
+00011180: 6167 656e 740a 6d6b 6469 7220 2d70 2024  agent.mkdir -p $
+00011190: 5944 415f 484f 4d45 2f2e 7373 680a 6368  YDA_HOME/.ssh.ch
+000111a0: 6d6f 6420 6f67 2d72 7778 2024 5944 415f  mod og-rwx $YDA_
+000111b0: 484f 4d45 2f2e 7373 680a 6361 7420 3e3e  HOME/.ssh.cat >>
+000111c0: 2024 5944 415f 484f 4d45 2f2e 7373 682f   $YDA_HOME/.ssh/
+000111d0: 6175 7468 6f72 697a 6564 5f6b 6579 7320  authorized_keys 
+000111e0: 3c3c 2045 4f46 0a3c 3c49 6e73 6572 745f  << EOF.<<Insert_
+000111f0: 5075 626c 6963 5f6b 6579 5f48 6572 653e  Public_key_Here>
+00011200: 3e0a 454f 460a 6368 6d6f 6420 6f67 2d72  >.EOF.chmod og-r
+00011210: 7720 2459 4441 5f48 4f4d 452f 2e73 7368  w $YDA_HOME/.ssh
+00011220: 2f61 7574 686f 7269 7a65 645f 6b65 7973  /authorized_keys
+00011230: 0a63 686f 776e 202d 5220 7964 2d61 6765  .chown -R yd-age
+00011240: 6e74 3a79 642d 6167 656e 7420 2459 4441  nt:yd-agent $YDA
+00011250: 5f48 4f4d 452f 2e73 7368 0a60 6060 0a0a  _HOME/.ssh.```..
+00011260: 2323 2320 5461 736b 2045 7865 6375 7469  ### Task Executi
+00011270: 6f6e 2044 6972 6563 746f 7279 0a0a 4570  on Directory..Ep
+00011280: 6865 6d65 7261 6c20 5461 736b 2064 6972  hemeral Task dir
+00011290: 6563 746f 7269 6573 2061 7265 2062 7920  ectories are by 
+000112a0: 6465 6661 756c 7420 6372 6561 7465 6420  default created 
+000112b0: 756e 6465 7220 602f 7661 722f 6f70 742f  under `/var/opt/
+000112c0: 7965 6c6c 6f77 646f 672f 6167 656e 742f  yellowdog/agent/
+000112d0: 6461 7461 2f77 6f72 6b65 7273 602e 2054  data/workers`. T
+000112e0: 6869 7320 6469 7265 6374 6f72 7920 636f  his directory co
+000112f0: 6e74 6169 6e73 206f 6e65 206f 7220 6d6f  ntains one or mo
+00011300: 7265 206e 756d 6265 7265 6420 7375 6264  re numbered subd
+00011310: 6972 6563 746f 7269 6573 2077 6865 7265  irectories where
+00011320: 2065 6163 6820 6e75 6d62 6572 6564 2064   each numbered d
+00011330: 6972 6563 746f 7279 2063 6f72 7265 7370  irectory corresp
+00011340: 6f6e 6473 2074 6f20 6120 576f 726b 6572  onds to a Worker
+00011350: 206f 6e20 7468 6520 6e6f 6465 2e0a 0a28   on the node...(
+00011360: 4f6e 2057 696e 646f 7773 2068 6f73 7473  On Windows hosts
+00011370: 2c20 7468 6520 5461 736b 2064 6972 6563  , the Task direc
+00011380: 746f 7269 6573 2061 7265 2066 6f75 6e64  tories are found
+00011390: 2075 6e64 6572 2060 2541 7070 4461 7461   under `%AppData
+000113a0: 255c 7965 6c6c 6f77 646f 675c 6167 656e  %\yellowdog\agen
+000113b0: 745c 6461 7461 5c77 6f72 6b65 7273 602e  t\data\workers`.
+000113c0: 290a 0a57 6865 6e20 6120 5461 736b 2069  )..When a Task i
+000113d0: 7320 616c 6c6f 6361 7465 6420 746f 2061  s allocated to a
+000113e0: 206e 6f64 652c 2061 6e20 6570 6865 6d65   node, an epheme
+000113f0: 7261 6c20 6469 7265 6374 6f72 7920 6973  ral directory is
+00011400: 2063 7265 6174 6564 2075 6e64 6572 2074   created under t
+00011410: 6865 2061 7070 6c69 6361 626c 6520 576f  he applicable Wo
+00011420: 726b 6572 2064 6972 6563 746f 7279 2c20  rker directory, 
+00011430: 7769 7468 2061 206e 616d 6520 636f 7272  with a name corr
+00011440: 6573 706f 6e64 696e 6720 7468 6520 5965  esponding the Ye
+00011450: 6c6c 6f77 446f 6720 4944 2066 6f72 2074  llowDog ID for t
+00011460: 6865 2054 6173 6b2e 2046 6f72 2065 7861  he Task. For exa
+00011470: 6d70 6c65 2c20 7468 6973 2069 7320 616e  mple, this is an
+00011480: 2065 7068 656d 6572 616c 2064 6972 6563   ephemeral direc
+00011490: 746f 7279 2062 6569 6e67 2075 7365 6420  tory being used 
+000114a0: 6279 2057 6f72 6b65 7220 6e75 6d62 6572  by Worker number
+000114b0: 2060 3160 3a0a 0a60 2f76 6172 2f6f 7074   `1`:..`/var/opt
+000114c0: 2f79 656c 6c6f 7764 6f67 2f61 6765 6e74  /yellowdog/agent
+000114d0: 2f64 6174 612f 776f 726b 6572 732f 312f  /data/workers/1/
+000114e0: 7964 6964 5f74 6173 6b5f 3535 3945 4245  ydid_task_559EBE
+000114f0: 5f37 3439 3439 3333 362d 6163 3262 2d34  _74949336-ac2b-4
+00011500: 3831 312d 6137 6435 2d66 3365 6364 3937  811-a7d5-f3ecd97
+00011510: 3339 3930 385f 315f 3160 0a0a 5468 6973  39908_1_1`..This
+00011520: 2069 7320 7468 6520 6469 7265 6374 6f72   is the director
+00011530: 7920 696e 746f 2077 6869 6368 2064 6f77  y into which dow
+00011540: 6e6c 6f61 6465 6420 6f62 6a65 6374 7320  nloaded objects 
+00011550: 6172 6520 706c 6163 6564 2c20 616e 6420  are placed, and 
+00011560: 696e 2077 6869 6368 206f 7574 7075 7420  in which output 
+00011570: 6669 6c65 7320 6172 6520 6372 6561 7465  files are create
+00011580: 6420 6279 2064 6566 6175 6c74 2e20 5468  d by default. Th
+00011590: 6520 636f 6e73 6f6c 6520 6f75 7470 7574  e console output
+000115a0: 2060 7461 736b 6f75 7470 7574 2e74 7874   `taskoutput.txt
+000115b0: 6020 6669 6c65 2077 696c 6c20 616c 736f  ` file will also
+000115c0: 2062 6520 6372 6561 7465 6420 696e 2074   be created in t
+000115d0: 6869 7320 6469 7265 6374 6f72 792e 0a0a  his directory...
+000115e0: 5365 6520 7468 6520 5b46 696c 6573 2044  See the [Files D
+000115f0: 6f77 6e6c 6f61 6465 6420 746f 2061 204e  ownloaded to a N
+00011600: 6f64 655d 2823 6669 6c65 732d 646f 776e  ode](#files-down
+00011610: 6c6f 6164 6564 2d74 6f2d 612d 6e6f 6465  loaded-to-a-node
+00011620: 2d66 6f72 2d75 7365 2d69 6e2d 7461 736b  -for-use-in-task
+00011630: 2d65 7865 6375 7469 6f6e 2920 7365 6374  -execution) sect
+00011640: 696f 6e20 6162 6f76 6520 666f 7220 6d6f  ion above for mo
+00011650: 7265 2064 6574 6169 6c73 206f 6e20 686f  re details on ho
+00011660: 7720 6669 6c65 7320 696e 2074 6869 7320  w files in this 
+00011670: 6469 7265 6374 6f72 7920 6172 6520 6861  directory are ha
+00011680: 6e64 6c65 642e 0a0a 4174 2074 6865 2063  ndled...At the c
+00011690: 6f6e 636c 7573 696f 6e20 6f66 2074 6865  onclusion of the
+000116a0: 2054 6173 6b2c 2061 6674 6572 2061 6e79   Task, after any
+000116b0: 2066 696c 6573 2072 6571 7565 7374 6564   files requested
+000116c0: 2066 6f72 2075 706c 6f61 6420 6861 7665   for upload have
+000116d0: 2062 6565 6e20 7570 6c6f 6164 6564 2074   been uploaded t
+000116e0: 6f20 7468 6520 4f62 6a65 6374 2053 746f  o the Object Sto
+000116f0: 7265 2028 7365 6520 7468 6520 5b46 696c  re (see the [Fil
+00011700: 6573 2055 706c 6f61 6465 6420 6672 6f6d  es Uploaded from
+00011710: 2061 204e 6f64 655d 2823 6669 6c65 732d   a Node](#files-
+00011720: 7570 6c6f 6164 6564 2d66 726f 6d2d 612d  uploaded-from-a-
+00011730: 6e6f 6465 2d74 6f2d 7468 652d 6f62 6a65  node-to-the-obje
+00011740: 6374 2d73 746f 7265 2d61 6674 6572 2d74  ct-store-after-t
+00011750: 6173 6b2d 6578 6563 7574 696f 6e29 2073  ask-execution) s
+00011760: 6563 7469 6f6e 2066 6f72 206d 6f72 6520  ection for more 
+00011770: 696e 666f 726d 6174 696f 6e29 2c20 7468  information), th
+00011780: 6520 6079 6469 645f 7461 736b 5f35 3539  e `ydid_task_559
+00011790: 4542 455f 3734 3934 3933 3336 2d61 6332  EBE_74949336-ac2
+000117a0: 622d 3438 3131 2d61 3764 352d 6633 6563  b-4811-a7d5-f3ec
+000117b0: 6439 3733 3939 3038 5f31 5f31 6020 7769  d9739908_1_1` wi
+000117c0: 6c6c 2062 6520 7265 6d6f 7665 642e 0a0a  ll be removed...
+000117d0: 2323 2053 7065 6369 6679 696e 6720 576f  ## Specifying Wo
+000117e0: 726b 2052 6571 7569 7265 6d65 6e74 7320  rk Requirements 
+000117f0: 7573 696e 6720 4353 5620 4461 7461 0a0a  using CSV Data..
+00011800: 4353 5620 6461 7461 2066 696c 6573 2063  CSV data files c
+00011810: 616e 2062 6520 7573 6564 2074 6f20 6472  an be used to dr
+00011820: 6976 6520 7468 6520 6765 6e65 7261 7469  ive the generati
+00011830: 6f6e 206f 6620 6c69 7374 7320 6f66 2054  on of lists of T
+00011840: 6173 6b73 2c20 6173 2066 6f6c 6c6f 7773  asks, as follows
+00011850: 3a0a 0a2d 2041 202a 2a70 726f 746f 7479  :..- A **prototy
+00011860: 7065 2a2a 2054 6173 6b20 7370 6563 6966  pe** Task specif
+00011870: 6963 6174 696f 6e20 6973 2063 7265 6174  ication is creat
+00011880: 6564 2077 6974 6869 6e20 6120 4a53 4f4e  ed within a JSON
+00011890: 2057 6f72 6b20 5265 7175 6972 656d 656e   Work Requiremen
+000118a0: 7420 7370 6563 6966 6963 6174 696f 6e20  t specification 
+000118b0: 6f72 2069 6e20 7468 6520 6077 6f72 6b52  or in the `workR
+000118c0: 6571 7569 7265 6d65 6e74 6020 7365 6374  equirement` sect
+000118d0: 696f 6e20 6f66 2074 6865 2054 4f4d 4c20  ion of the TOML 
+000118e0: 636f 6e66 6967 7572 6174 696f 6e20 6669  configuration fi
+000118f0: 6c65 0a2d 2054 6865 2070 726f 746f 7479  le.- The prototy
+00011900: 7065 2074 6173 6b20 696e 636c 7564 6573  pe task includes
+00011910: 206f 6e65 206f 7220 6d6f 7265 2076 6172   one or more var
+00011920: 6961 626c 6520 7375 6273 7469 7475 7469  iable substituti
+00011930: 6f6e 730a 2d20 4120 4353 5620 6669 6c65  ons.- A CSV file
+00011940: 2069 7320 6372 6561 7465 642c 2077 6974   is created, wit
+00011950: 6820 7468 6520 2a2a 6865 6164 6572 732a  h the **headers*
+00011960: 2a20 2866 6972 7374 2072 6f77 2920 6d61  * (first row) ma
+00011970: 7463 6869 6e67 2074 6865 206e 616d 6573  tching the names
+00011980: 206f 6620 7468 6520 7661 7269 6162 6c65   of the variable
+00011990: 2073 7562 7374 6974 7574 696f 6e73 2069   substitutions i
+000119a0: 6e20 7468 6520 5461 736b 2070 726f 746f  n the Task proto
+000119b0: 7479 7065 0a2d 2045 6163 6820 7375 6273  type.- Each subs
+000119c0: 6571 7565 6e74 2072 6f77 206f 6620 7468  equent row of th
+000119d0: 6520 4353 5620 6669 6c65 2072 6570 7265  e CSV file repre
+000119e0: 7365 6e74 7320 6120 6e65 7720 5461 736b  sents a new Task
+000119f0: 2062 7569 6c74 2075 7369 6e67 2074 6865   built using the
+00011a00: 2070 726f 746f 7479 7065 2c20 7769 7468   prototype, with
+00011a10: 2074 6865 2076 6172 6961 626c 6573 2073   the variables s
+00011a20: 7562 7374 6974 7574 6564 2062 7920 7468  ubstituted by th
+00011a30: 6520 7661 6c75 6573 2069 6e20 7468 6520  e values in the 
+00011a40: 726f 770a 2d20 4120 5461 736b 2077 696c  row.- A Task wil
+00011a50: 6c20 6265 2063 7265 6174 6564 2066 6f72  l be created for
+00011a60: 2065 6163 6820 6461 7461 2072 6f77 0a0a   each data row..
+00011a70: 2323 2320 576f 726b 2052 6571 7569 7265  ### Work Require
+00011a80: 6d65 6e74 2043 5356 2044 6174 6120 4578  ment CSV Data Ex
+00011a90: 616d 706c 650a 0a41 7320 616e 2065 7861  ample..As an exa
+00011aa0: 6d70 6c65 2c20 636f 6e73 6964 6572 2074  mple, consider t
+00011ab0: 6865 2066 6f6c 6c6f 7769 6e67 204a 534f  he following JSO
+00011ac0: 4e20 576f 726b 2052 6571 7569 7265 6d65  N Work Requireme
+00011ad0: 6e74 2060 7772 2e6a 736f 6e60 3a0a 0a60  nt `wr.json`:..`
+00011ae0: 6060 6a73 6f6e 0a7b 0a20 2022 7461 736b  ``json.{.  "task
+00011af0: 4772 6f75 7073 223a 205b 0a20 2020 207b  Groups": [.    {
+00011b00: 0a20 2020 2020 2022 7461 736b 7322 3a20  .      "tasks": 
+00011b10: 5b0a 2020 2020 2020 2020 7b0a 2020 2020  [.        {.    
+00011b20: 2020 2020 2020 2261 7267 756d 656e 7473        "arguments
+00011b30: 223a 205b 227b 7b61 7267 5f31 7d7d 222c  ": ["{{arg_1}}",
+00011b40: 2022 7b7b 6172 675f 327d 7d22 2c20 227b   "{{arg_2}}", "{
+00011b50: 7b61 7267 5f33 7d7d 225d 2c0a 2020 2020  {arg_3}}"],.    
+00011b60: 2020 2020 2020 2265 6e76 6972 6f6e 6d65        "environme
+00011b70: 6e74 223a 207b 2245 4e56 5f56 4152 5f31  nt": {"ENV_VAR_1
+00011b80: 223a 2022 7b7b 656e 765f 317d 7d22 7d0a  ": "{{env_1}}"}.
+00011b90: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00011ba0: 5d0a 2020 2020 7d0a 2020 5d0a 7d0a 6060  ].    }.  ].}.``
+00011bb0: 600a 0a4e 6f74 6520 7468 6174 2074 6865  `..Note that the
+00011bc0: 2054 6173 6b20 4772 6f75 7020 6d75 7374   Task Group must
+00011bd0: 2063 6f6e 7461 696e 206f 6e6c 7920 6120   contain only a 
+00011be0: 7369 6e67 6c65 2054 6173 6b2c 2061 6374  single Task, act
+00011bf0: 696e 6720 6173 2074 6865 2070 726f 746f  ing as the proto
+00011c00: 7479 7065 2e0a 0a4e 6f77 2063 6f6e 7369  type...Now consi
+00011c10: 6465 7220 6120 4353 5620 6669 6c65 2060  der a CSV file `
+00011c20: 7772 5f64 6174 612e 6373 7660 2077 6974  wr_data.csv` wit
+00011c30: 6820 7468 6520 666f 6c6c 6f77 696e 6720  h the following 
+00011c40: 636f 6e74 656e 7473 3a0a 0a60 6060 7465  contents:..```te
+00011c50: 7874 0a61 7267 5f31 2c20 6172 675f 322c  xt.arg_1, arg_2,
+00011c60: 2061 7267 5f33 2c20 656e 765f 310a 412c   arg_3, env_1.A,
+00011c70: 2020 2020 2042 2c20 2020 2020 432c 2020       B,     C,  
+00011c80: 2020 2045 2d31 0a44 2c20 2020 2020 452c     E-1.D,     E,
+00011c90: 2020 2020 2046 2c20 2020 2020 452d 320a       F,     E-2.
+00011ca0: 472c 2020 2020 2048 2c20 2020 2020 492c  G,     H,     I,
+00011cb0: 2020 2020 2045 2d33 0a60 6060 0a0a 4e6f       E-3.```..No
+00011cc0: 7465 2074 6861 7420 7468 6520 286f 7074  te that the (opt
+00011cd0: 696f 6e61 6c29 206c 6561 6469 6e67 2073  ional) leading s
+00011ce0: 7061 6365 7320 6166 7465 7220 6561 6368  paces after each
+00011cf0: 2063 6f6d 6d61 2061 7265 2069 676e 6f72   comma are ignor
+00011d00: 6564 2c20 6275 7420 7472 6169 6c69 6e67  ed, but trailing
+00011d10: 2073 7061 6365 7320 6172 6520 6e6f 7420   spaces are not 
+00011d20: 616e 6420 7769 6c6c 2066 6f72 6d20 7061  and will form pa
+00011d30: 7274 206f 6620 7468 6520 696d 706f 7274  rt of the import
+00011d40: 6564 2064 6174 612e 0a0a 4966 2074 6865  ed data...If the
+00011d50: 7365 2066 696c 6573 2061 7265 2070 726f  se files are pro
+00011d60: 6365 7373 6564 2075 7369 6e67 2060 7964  cessed using `yd
+00011d70: 2d73 7562 6d69 7420 2d72 2077 722e 6a73  -submit -r wr.js
+00011d80: 6f6e 202d 5620 7772 5f64 6174 612e 6373  on -V wr_data.cs
+00011d90: 7660 2c20 7468 6520 666f 6c6c 6f77 696e  v`, the followin
+00011da0: 6720 6578 7061 6e64 6564 206c 6973 7420  g expanded list 
+00011db0: 6f66 2074 6872 6565 2054 6173 6b73 2077  of three Tasks w
+00011dc0: 696c 6c20 6265 2063 7265 6174 6564 2070  ill be created p
+00011dd0: 7269 6f72 2074 6f20 6675 7274 6865 7220  rior to further 
+00011de0: 7072 6f63 6573 7369 6e67 2062 7920 7468  processing by th
+00011df0: 6520 6079 642d 7375 626d 6974 6020 7363  e `yd-submit` sc
+00011e00: 7269 7074 3a0a 0a60 6060 6a73 6f6e 0a7b  ript:..```json.{
+00011e10: 0a20 2022 7461 736b 4772 6f75 7073 223a  .  "taskGroups":
+00011e20: 205b 0a20 2020 207b 0a20 2020 2020 2022   [.    {.      "
+00011e30: 7461 736b 7322 3a20 5b0a 2020 2020 2020  tasks": [.      
+00011e40: 2020 7b0a 2020 2020 2020 2020 2020 2261    {.          "a
+00011e50: 7267 756d 656e 7473 223a 205b 2241 222c  rguments": ["A",
+00011e60: 2022 4222 2c20 2243 225d 2c0a 2020 2020   "B", "C"],.    
+00011e70: 2020 2020 2020 2265 6e76 6972 6f6e 6d65        "environme
+00011e80: 6e74 223a 207b 2245 4e56 5f56 4152 5f31  nt": {"ENV_VAR_1
+00011e90: 223a 2022 452d 3122 7d0a 2020 2020 2020  ": "E-1"}.      
+00011ea0: 2020 7d2c 0a20 2020 2020 2020 207b 0a20    },.        {. 
+00011eb0: 2020 2020 2020 2020 2022 6172 6775 6d65           "argume
+00011ec0: 6e74 7322 3a20 5b22 4422 2c20 2245 222c  nts": ["D", "E",
+00011ed0: 2022 4622 5d2c 0a20 2020 2020 2020 2020   "F"],.         
+00011ee0: 2022 656e 7669 726f 6e6d 656e 7422 3a20   "environment": 
+00011ef0: 7b22 454e 565f 5641 525f 3122 3a20 2245  {"ENV_VAR_1": "E
+00011f00: 2d32 227d 0a20 2020 2020 2020 207d 2c0a  -2"}.        },.
+00011f10: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+00011f20: 2020 2020 2261 7267 756d 656e 7473 223a      "arguments":
+00011f30: 205b 2247 222c 2022 4822 2c20 2249 225d   ["G", "H", "I"]
+00011f40: 2c0a 2020 2020 2020 2020 2020 2265 6e76  ,.          "env
+00011f50: 6972 6f6e 6d65 6e74 223a 207b 2245 4e56  ironment": {"ENV
+00011f60: 5f56 4152 5f31 223a 2022 452d 3322 7d0a  _VAR_1": "E-3"}.
+00011f70: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00011f80: 5d0a 2020 2020 7d0a 2020 5d0a 7d0a 6060  ].    }.  ].}.``
+00011f90: 600a 0a23 2323 2043 5356 2056 6172 6961  `..### CSV Varia
+00011fa0: 626c 6520 5375 6273 7469 7475 7469 6f6e  ble Substitution
+00011fb0: 730a 0a57 6865 6e20 7468 6520 4353 5620  s..When the CSV 
+00011fc0: 6669 6c65 2064 6174 6120 6973 2070 726f  file data is pro
+00011fd0: 6365 7373 6564 2c20 7468 6520 6f6e 6c79  cessed, the only
+00011fe0: 2073 7562 7374 6974 7574 696f 6e73 206d   substitutions m
+00011ff0: 6164 6520 6172 6520 7468 6f73 6520 7768  ade are those wh
+00012000: 6963 6820 6d61 7463 6820 7468 6520 7661  ich match the va
+00012010: 7269 6162 6c65 2073 7562 7374 6974 7574  riable substitut
+00012020: 696f 6e73 2069 6e20 7468 6520 7072 6f74  ions in the prot
+00012030: 6f74 7970 6520 5461 736b 2e20 5468 6520  otype Task. The 
+00012040: 4353 5620 6669 6c65 2069 7320 7468 6520  CSV file is the 
+00012050: 2a2a 6f6e 6c79 2a2a 2073 6f75 7263 6520  **only** source 
+00012060: 6f66 2073 7562 7374 6974 7574 696f 6e73  of substitutions
+00012070: 2075 7365 6420 666f 7220 7468 6973 2070   used for this p
+00012080: 726f 6365 7373 696e 6720 7068 6173 653b  rocessing phase;
+00012090: 2061 6c6c 206f 7468 6572 2076 6172 6961   all other varia
+000120a0: 626c 6520 7375 6273 7469 7475 7469 6f6e  ble substitution
+000120b0: 7320 2873 7570 706c 6965 6420 6f6e 2074  s (supplied on t
+000120c0: 6865 2063 6f6d 6d61 6e64 206c 696e 652c  he command line,
+000120d0: 2069 6e20 7468 6520 544f 4d4c 2063 6f6e   in the TOML con
+000120e0: 6669 6775 7261 7469 6f6e 2066 696c 652c  figuration file,
+000120f0: 206f 7220 6672 6f6d 2065 6e76 6972 6f6e   or from environ
+00012100: 6d65 6e74 2076 6172 6961 626c 6573 2920  ment variables) 
+00012110: 6172 6520 6967 6e6f 7265 6420 2d2d 2069  are ignored -- i
+00012120: 2e65 2e2c 2074 6865 7920 646f 206e 6f74  .e., they do not
+00012130: 206f 7665 7272 6964 6520 7468 6520 636f   override the co
+00012140: 6e74 656e 7473 206f 6620 7468 6520 4353  ntents of the CS
+00012150: 5620 6669 6c65 2e0a 0a41 6c6c 2076 6172  V file...All var
+00012160: 6961 626c 6520 7375 6273 7469 7475 7469  iable substituti
+00012170: 6f6e 7320 756e 7265 6c61 7465 6420 746f  ons unrelated to
+00012180: 2074 6865 2043 5356 2066 696c 6520 6461   the CSV file da
+00012190: 7461 2061 7265 206c 6566 7420 756e 6368  ta are left unch
+000121a0: 616e 6765 642c 2066 6f72 2073 7562 7365  anged, for subse
+000121b0: 7175 656e 7420 7072 6f63 6573 7369 6e67  quent processing
+000121c0: 2062 7920 6079 642d 7375 626d 6974 602e   by `yd-submit`.
+000121d0: 0a0a 4966 2074 6865 2076 616c 7565 2074  ..If the value t
+000121e0: 6f20 6265 2069 6e73 6572 7465 6420 6973  o be inserted is
+000121f0: 2061 206e 756d 6265 7220 2861 6e20 696e   a number (an in
+00012200: 7465 6765 7220 6f72 2066 6c6f 6174 696e  teger or floatin
+00012210: 6720 706f 696e 7420 7661 6c75 6529 206f  g point value) o
+00012220: 7220 426f 6f6c 6561 6e2c 2074 6865 2060  r Boolean, the `
+00012230: 7b7b 6e75 6d3a 6d79 5f6e 756d 6265 725f  {{num:my_number_
+00012240: 7661 727d 7d60 2061 6e64 2060 7b7b 626f  var}}` and `{{bo
+00012250: 6f6c 3a6d 795f 626f 6f6c 6561 6e5f 7661  ol:my_boolean_va
+00012260: 727d 7d60 2066 6f72 6d73 2063 616e 2062  r}}` forms can b
+00012270: 6520 7573 6564 2069 6e20 7468 6520 4a53  e used in the JS
+00012280: 4f4e 2066 696c 652c 2061 7320 7769 7468  ON file, as with
+00012290: 2074 6865 6972 2075 7365 2069 6e20 6f74   their use in ot
+000122a0: 6865 7220 7061 7274 7320 6f66 2074 6865  her parts of the
+000122b0: 204a 534f 4e20 576f 726b 2052 6571 7569   JSON Work Requi
+000122c0: 7265 6d65 6e74 2073 7065 6369 6669 6361  rement specifica
+000122d0: 7469 6f6e 2e20 5468 6520 7375 6273 7469  tion. The substi
+000122e0: 7475 7465 6420 7661 6c75 6520 7769 6c6c  tuted value will
+000122f0: 2061 7373 756d 6520 7468 6520 6e6f 6d69   assume the nomi
+00012300: 6e61 7465 6420 7479 7065 2072 6174 6865  nated type rathe
+00012310: 7220 7468 616e 2062 6569 6e67 2061 2073  r than being a s
+00012320: 7472 696e 672e 0a0a 2323 2320 5072 6f70  tring...### Prop
+00012330: 6572 7479 2049 6e68 6572 6974 616e 6365  erty Inheritance
+00012340: 0a0a 416c 6c20 7468 6520 7573 7561 6c20  ..All the usual 
+00012350: 7072 6f70 6572 7479 2069 6e68 6572 6974  property inherit
+00012360: 616e 6365 2066 6561 7475 7265 7320 6f70  ance features op
+00012370: 6572 6174 6520 6173 206e 6f72 6d61 6c2e  erate as normal.
+00012380: 2050 726f 7065 7274 6965 7320 6172 6520   Properties are 
+00012390: 696e 6865 7269 7465 6420 6672 6f6d 2074  inherited from t
+000123a0: 6865 2060 636f 6e66 6967 2e74 6f6d 6c60  he `config.toml`
+000123b0: 2066 696c 652c 2061 6e64 2066 726f 6d20   file, and from 
+000123c0: 7468 6520 7265 6c65 7661 6e74 2073 6563  the relevant sec
+000123d0: 7469 6f6e 7320 6f66 2074 6865 204a 534f  tions of the JSO
+000123e0: 4e20 576f 726b 2052 6571 7569 7265 6d65  N Work Requireme
+000123f0: 6e74 2066 696c 652e 2041 6e79 2070 726f  nt file. Any pro
+00012400: 7065 7274 6965 7320 7365 7420 7769 7468  perties set with
+00012410: 696e 2061 2054 6173 6b20 7072 6f74 6f74  in a Task protot
+00012420: 7970 6520 6172 6520 636f 7069 6564 2074  ype are copied t
+00012430: 6f20 616c 6c20 7468 6520 6765 6e65 7261  o all the genera
+00012440: 7465 6420 5461 736b 732e 0a0a 2323 2320  ted Tasks...### 
+00012450: 4d75 6c74 6970 6c65 2054 6173 6b20 4772  Multiple Task Gr
+00012460: 6f75 7073 2075 7369 6e67 204d 756c 7469  oups using Multi
+00012470: 706c 6520 4353 5620 4669 6c65 730a 0a54  ple CSV Files..T
+00012480: 6865 2075 7365 206f 6620 6d75 6c74 6970  he use of multip
+00012490: 6c65 2054 6173 6b20 4772 6f75 7073 2069  le Task Groups i
+000124a0: 7320 616c 736f 2073 7570 706f 7274 6564  s also supported
+000124b0: 2c20 6279 2075 7369 6e67 206f 6e65 2043  , by using one C
+000124c0: 5356 2066 696c 6520 7065 7220 5461 736b  SV file per Task
+000124d0: 2047 726f 7570 2e20 4561 6368 2054 6173   Group. Each Tas
+000124e0: 6b20 4772 6f75 7020 6d75 7374 2063 6f6e  k Group must con
+000124f0: 7461 696e 206f 6e6c 7920 6120 7369 6e67  tain only a sing
+00012500: 6c65 2070 726f 746f 7479 7065 2054 6173  le prototype Tas
+00012510: 6b2e 0a0a 5468 6520 4353 5620 6669 6c65  k...The CSV file
+00012520: 7320 6172 6520 7375 7070 6c69 6564 206f  s are supplied o
+00012530: 6e20 7468 6520 636f 6d6d 616e 6420 6c69  n the command li
+00012540: 6e65 2069 6e20 7468 6520 6f72 6465 7220  ne in the order 
+00012550: 6f66 2074 6865 2054 6173 6b20 4772 6f75  of the Task Grou
+00012560: 7073 2074 6f20 7768 6963 6820 7468 6579  ps to which they
+00012570: 2061 7070 6c79 2e20 466f 7220 6578 616d   apply. For exam
+00012580: 706c 652c 2069 6620 6077 725f 6a73 6f6e  ple, if `wr_json
+00012590: 6020 636f 6e74 6169 6e73 2074 776f 2054  ` contains two T
+000125a0: 6173 6b20 4772 6f75 7073 2c20 6173 2066  ask Groups, as f
+000125b0: 6f6c 6c6f 7773 3a0a 0a60 6060 6a73 6f6e  ollows:..```json
+000125c0: 0a7b 0a20 2022 7461 736b 4772 6f75 7073  .{.  "taskGroups
+000125d0: 223a 205b 0a20 2020 207b 0a20 2020 2020  ": [.    {.     
+000125e0: 2022 7461 736b 7322 3a20 5b0a 2020 2020   "tasks": [.    
+000125f0: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+00012600: 2261 7267 756d 656e 7473 223a 205b 227b  "arguments": ["{
+00012610: 7b61 7267 5f31 7d7d 222c 2022 7b7b 6172  {arg_1}}", "{{ar
+00012620: 675f 327d 7d22 2c20 227b 7b61 7267 5f33  g_2}}", "{{arg_3
+00012630: 7d7d 225d 2c0a 2020 2020 2020 2020 2020  }}"],.          
+00012640: 2265 6e76 6972 6f6e 6d65 6e74 223a 207b  "environment": {
+00012650: 2245 4e56 5f56 4152 5f31 223a 2022 7b7b  "ENV_VAR_1": "{{
+00012660: 656e 765f 317d 7d22 7d0a 2020 2020 2020  env_1}}"}.      
+00012670: 2020 7d0a 2020 2020 2020 5d0a 2020 2020    }.      ].    
+00012680: 7d2c 0a20 2020 207b 0a20 2020 2020 2022  },.    {.      "
+00012690: 7461 736b 7322 3a20 5b0a 2020 2020 2020  tasks": [.      
+000126a0: 2020 7b0a 2020 2020 2020 2020 2020 2261    {.          "a
+000126b0: 7267 756d 656e 7473 223a 205b 227b 7b61  rguments": ["{{a
+000126c0: 7267 5f31 7d7d 222c 2022 7b7b 6172 675f  rg_1}}", "{{arg_
+000126d0: 327d 7d22 5d2c 0a20 2020 2020 2020 2020  2}}"],.         
+000126e0: 2022 656e 7669 726f 6e6d 656e 7422 3a20   "environment": 
+000126f0: 7b22 454e 565f 5641 525f 3122 3a20 227b  {"ENV_VAR_1": "{
+00012700: 7b65 6e76 5f31 7d7d 222c 2022 454e 565f  {env_1}}", "ENV_
+00012710: 5641 525f 3222 3a20 227b 7b65 6e76 5f32  VAR_2": "{{env_2
+00012720: 7d7d 227d 0a20 2020 2020 2020 207d 0a20  }}"}.        }. 
+00012730: 2020 2020 205d 0a20 2020 207d 0a20 205d       ].    }.  ]
+00012740: 0a7d 0a60 6060 0a0a 5468 6520 6079 642d  .}.```..The `yd-
+00012750: 7375 626d 6974 6020 636f 6d6d 616e 6420  submit` command 
+00012760: 776f 756c 6420 7468 656e 2062 6520 696e  would then be in
+00012770: 766f 6b65 6420 7769 7468 2061 2073 6570  voked with a sep
+00012780: 6172 6174 6520 4353 5620 6669 6c65 2066  arate CSV file f
+00012790: 6f72 2065 6163 6820 5461 736b 2047 726f  or each Task Gro
+000127a0: 7570 2c20 652e 672e 3a0a 0a60 6060 7368  up, e.g.:..```sh
+000127b0: 656c 6c0a 7964 2d73 7562 6d69 7420 2d72  ell.yd-submit -r
+000127c0: 2077 722e 6a73 6f6e 202d 5620 7772 5f64   wr.json -V wr_d
+000127d0: 6174 615f 7461 736b 5f67 726f 7570 5f31  ata_task_group_1
+000127e0: 2e63 7376 202d 5620 7772 5f64 6174 615f  .csv -V wr_data_
+000127f0: 7461 736b 5f67 726f 7570 5f32 2e63 7376  task_group_2.csv
+00012800: 0a60 6060 0a0a 4966 2074 6865 7265 2061  .```..If there a
+00012810: 7265 202a 2a66 6577 6572 2a2a 2043 5356  re **fewer** CSV
+00012820: 2066 696c 6573 2074 6861 6e20 5461 736b   files than Task
+00012830: 2047 726f 7570 7320 6120 7761 726e 696e   Groups a warnin
+00012840: 6720 7769 6c6c 2062 6520 7072 696e 7465  g will be printe
+00012850: 6420 616e 642c 2069 6620 7468 6572 6520  d and, if there 
+00012860: 6172 6520 276e 2720 4353 5620 6669 6c65  are 'n' CSV file
+00012870: 732c 2043 5356 2064 6174 6120 7072 6f63  s, CSV data proc
+00012880: 6573 7369 6e67 2077 696c 6c20 6265 2061  essing will be a
+00012890: 7070 6c69 6564 2074 6f20 7468 6520 6669  pplied to the fi
+000128a0: 7273 7420 276e 2720 5461 736b 2047 726f  rst 'n' Task Gro
+000128b0: 7570 7320 696e 2074 6865 2057 6f72 6b20  ups in the Work 
+000128c0: 5265 7175 6972 656d 656e 7420 6279 2064  Requirement by d
+000128d0: 6566 6175 6c74 2c20 696e 2074 6865 206f  efault, in the o
+000128e0: 7264 6572 2069 6e20 7768 6963 6820 7468  rder in which th
+000128f0: 6520 4353 5620 6669 6c65 7320 7765 7265  e CSV files were
+00012900: 2073 7570 706c 6965 642e 2049 6620 7468   supplied. If th
+00012910: 6572 6520 6172 6520 2a2a 6d6f 7265 2a2a  ere are **more**
+00012920: 2043 5356 2066 696c 6573 2074 6861 6e20   CSV files than 
+00012930: 5461 736b 2047 726f 7570 732c 2061 6e20  Task Groups, an 
+00012940: 6572 726f 7220 7769 6c6c 2062 6520 7261  error will be ra
+00012950: 6973 6564 2061 6e64 2070 726f 6365 7373  ised and process
+00012960: 696e 6720 7769 6c6c 2073 746f 702e 0a0a  ing will stop...
+00012970: 4974 2069 7320 706f 7373 6962 6c65 2074  It is possible t
+00012980: 6f20 6170 706c 7920 4353 5620 6669 6c65  o apply CSV file
+00012990: 7320 6578 706c 6963 6974 6c79 2074 6f20  s explicitly to 
+000129a0: 7370 6563 6966 6963 2054 6173 6b20 4772  specific Task Gr
+000129b0: 6f75 7073 2c20 6279 2075 7369 6e67 2061  oups, by using a
+000129c0: 6e20 6f70 7469 6f6e 616c 202a 2a69 6e64  n optional **ind
+000129d0: 6578 2070 6f73 7466 6978 2a2a 2028 652e  ex postfix** (e.
+000129e0: 672e 2c20 603a 3260 2920 6174 2074 6865  g., `:2`) at the
+000129f0: 2065 6e64 206f 6620 6561 6368 2043 5356   end of each CSV
+00012a00: 2066 696c 656e 616d 652e 2046 6f72 2065   filename. For e
+00012a10: 7861 6d70 6c65 2c20 6966 2074 6865 7265  xample, if there
+00012a20: 2061 7265 2074 776f 2043 5356 2066 696c   are two CSV fil
+00012a30: 6573 2074 6f20 6265 2061 7070 6c69 6564  es to be applied
+00012a40: 2074 6f20 7468 6520 7365 636f 6e64 2061   to the second a
+00012a50: 6e64 2066 6f75 7274 6820 5461 736b 2047  nd fourth Task G
+00012a60: 726f 7570 7320 696e 2061 204a 534f 4e20  roups in a JSON 
+00012a70: 576f 726b 2052 6571 7569 7265 6d65 6e74  Work Requirement
+00012a80: 2c20 7573 6520 7468 6520 666f 6c6c 6f77  , use the follow
+00012a90: 696e 6720 7379 6e74 6178 3a0a 0a60 6060  ing syntax:..```
+00012aa0: 7368 656c 6c0a 7964 2d73 7562 6d69 7420  shell.yd-submit 
+00012ab0: 2d72 2077 722e 6a73 6f6e 202d 5620 7772  -r wr.json -V wr
+00012ac0: 5f64 6174 615f 7461 736b 5f67 726f 7570  _data_task_group
+00012ad0: 5f32 2e63 7376 3a32 202d 5620 7772 5f64  _2.csv:2 -V wr_d
+00012ae0: 6174 615f 7461 736b 5f67 726f 7570 5f34  ata_task_group_4
+00012af0: 2e63 7376 3a34 0a60 6060 0a0a 416c 7465  .csv:4.```..Alte
+00012b00: 726e 6174 6976 656c 792c 2074 6865 202a  rnatively, the *
+00012b10: 2a54 6173 6b20 4772 6f75 7020 6e61 6d65  *Task Group name
+00012b20: 2a2a 2028 6966 2073 7570 706c 6965 6420  ** (if supplied 
+00012b30: 696e 2074 6865 204a 534f 4e20 6669 6c65  in the JSON file
+00012b40: 2920 6361 6e20 6265 2075 7365 6420 6173  ) can be used as
+00012b50: 2074 6865 2070 6f73 7466 6978 2e20 466f   the postfix. Fo
+00012b60: 7220 6578 616d 706c 652c 2069 6620 7468  r example, if th
+00012b70: 6520 5461 736b 2047 726f 7570 7320 6162  e Task Groups ab
+00012b80: 6f76 6520 6172 6520 6e61 6d65 6420 6074  ove are named `t
+00012b90: 675f 7477 6f60 2061 6e64 2060 7467 5f66  g_two` and `tg_f
+00012ba0: 6f75 7260 2c20 7468 6520 6079 642d 7375  our`, the `yd-su
+00012bb0: 626d 6974 6020 636f 6d6d 616e 6420 776f  bmit` command wo
+00012bc0: 756c 6420 6265 636f 6d65 3a0a 0a60 6060  uld become:..```
+00012bd0: 7368 656c 6c0a 7964 2d73 7562 6d69 7420  shell.yd-submit 
+00012be0: 2d72 2077 722e 6a73 6f6e 202d 5620 7772  -r wr.json -V wr
+00012bf0: 5f64 6174 615f 7461 736b 5f67 726f 7570  _data_task_group
+00012c00: 5f32 2e63 7376 3a74 675f 7477 6f20 2d56  _2.csv:tg_two -V
+00012c10: 2077 725f 6461 7461 5f74 6173 6b5f 6772   wr_data_task_gr
+00012c20: 6f75 705f 342e 6373 763a 7467 5f66 6f75  oup_4.csv:tg_fou
+00012c30: 720a 6060 600a 0a4e 6f74 6520 7468 6174  r.```..Note that
+00012c40: 206f 6e6c 7920 6f6e 6520 4353 5620 6669   only one CSV fi
+00012c50: 6c65 2063 616e 2062 6520 6170 706c 6965  le can be applie
+00012c60: 6420 746f 2061 6e79 2067 6976 656e 2054  d to any given T
+00012c70: 6173 6b20 4772 6f75 702e 2041 2073 696e  ask Group. A sin
+00012c80: 676c 6520 4353 5620 6669 6c65 2063 616e  gle CSV file can
+00012c90: 2c20 686f 7765 7665 722c 2062 6520 7265  , however, be re
+00012ca0: 7573 6564 2066 6f72 206d 756c 7469 706c  used for multipl
+00012cb0: 6520 5461 736b 2047 726f 7570 732e 0a0a  e Task Groups...
+00012cc0: 2323 2320 5573 696e 6720 4353 5620 4461  ### Using CSV Da
+00012cd0: 7461 2077 6974 6820 5369 6d70 6c65 2c20  ta with Simple, 
+00012ce0: 544f 4d4c 2d4f 6e6c 7920 576f 726b 2052  TOML-Only Work R
+00012cf0: 6571 7569 7265 6d65 6e74 2053 7065 6369  equirement Speci
+00012d00: 6669 6361 7469 6f6e 730a 0a49 7427 7320  fications..It's 
+00012d10: 706f 7373 6962 6c65 2074 6f20 7573 6520  possible to use 
+00012d20: 544f 4d4c 2065 7863 6c75 7369 7665 6c79  TOML exclusively
+00012d30: 2074 6f20 6465 7269 7665 2061 206c 6973   to derive a lis
+00012d40: 7420 6f66 2054 6173 6b73 2066 726f 6d20  t of Tasks from 
+00012d50: 4353 5620 6461 7461 202d 2d20 692e 652e  CSV data -- i.e.
+00012d60: 2c20 6120 4a53 4f4e 2057 6f72 6b20 5265  , a JSON Work Re
+00012d70: 7175 6972 656d 656e 7420 7370 6563 6966  quirement specif
+00012d80: 6963 6174 696f 6e20 6973 206e 6f74 2072  ication is not r
+00012d90: 6571 7569 7265 642e 0a0a 546f 206d 616b  equired...To mak
+00012da0: 6520 7573 6520 6f66 2074 6869 733a 0a0a  e use of this:..
+00012db0: 312e 2045 6e73 7572 6520 7468 6174 206e  1. Ensure that n
+00012dc0: 6f20 4a53 4f4e 2057 6f72 6b20 5265 7175  o JSON Work Requ
+00012dd0: 6972 656d 656e 7420 646f 6375 6d65 6e74  irement document
+00012de0: 2069 7320 7370 6563 6966 6965 6420 286e   is specified (n
+00012df0: 6f20 6077 6f72 6b52 6571 7569 7265 6d65  o `workRequireme
+00012e00: 6e74 4461 7461 6020 696e 2074 6865 2054  ntData` in the T
+00012e10: 4f4d 4c20 6669 6c65 2c20 6f72 2060 2d2d  OML file, or `--
+00012e20: 776f 726b 2d72 6571 7569 7265 6d65 6e74  work-requirement
+00012e30: 6020 6f6e 2074 6865 2063 6f6d 6d61 6e64  ` on the command
+00012e40: 206c 696e 6529 0a32 2e20 496e 7365 7274   line).2. Insert
+00012e50: 2074 6865 2072 6571 7569 7265 6420 4353   the required CS
+00012e60: 562d 7375 7070 6c69 6564 2076 6172 6961  V-supplied varia
+00012e70: 626c 6520 7375 6273 7469 7475 7469 6f6e  ble substitution
+00012e80: 7320 6469 7265 6374 6c79 2069 6e74 6f20  s directly into 
+00012e90: 7468 6520 544f 4d4c 2070 726f 7065 7274  the TOML propert
+00012ea0: 6965 732c 2065 2e67 2e20 6061 7267 756d  ies, e.g. `argum
+00012eb0: 656e 7473 203d 205b 227b 7b61 7267 5f31  ents = ["{{arg_1
+00012ec0: 7d7d 222c 2022 7b7b 6172 675f 327d 7d22  }}", "{{arg_2}}"
+00012ed0: 5d60 0a33 2e20 5370 6563 6966 7920 6120  ]`.3. Specify a 
+00012ee0: 7369 6e67 6c65 2043 5356 2066 696c 6520  single CSV file 
+00012ef0: 696e 2074 6865 2060 6373 7646 696c 6573  in the `csvFiles
+00012f00: 6020 544f 4d4c 2070 726f 7065 7274 792c  ` TOML property,
+00012f10: 2065 2e67 2e20 6063 7376 4669 6c65 7320   e.g. `csvFiles 
+00012f20: 3d20 5b22 7772 5f64 6174 612e 6373 7622  = ["wr_data.csv"
+00012f30: 5d60 2c20 6f72 2070 726f 7669 6465 2074  ]`, or provide t
+00012f40: 6865 2043 5356 2066 696c 6520 6f6e 2074  he CSV file on t
+00012f50: 6865 2063 6f6d 6d61 6e64 206c 696e 6520  he command line 
+00012f60: 602d 5620 7772 5f64 6174 612e 6373 7660  `-V wr_data.csv`
+00012f70: 0a0a 5768 656e 2060 7964 2d73 7562 6d69  ..When `yd-submi
+00012f80: 7460 2069 7320 7275 6e2c 2069 7420 7769  t` is run, it wi
+00012f90: 6c6c 2065 7870 616e 6420 7468 6520 5461  ll expand the Ta
+00012fa0: 736b 206c 6973 7420 746f 206d 6174 6368  sk list to match
+00012fb0: 2074 6865 206e 756d 6265 7220 6f66 2064   the number of d
+00012fc0: 6174 6120 726f 7773 2069 6e20 7468 6520  ata rows in the 
+00012fd0: 4353 5620 6669 6c65 2e0a 0a23 2323 2049  CSV file...### I
+00012fe0: 6e73 7065 6374 696e 6720 7468 6520 5265  nspecting the Re
+00012ff0: 7375 6c74 7320 6f66 2043 5356 2056 6172  sults of CSV Var
+00013000: 6961 626c 6520 5375 6273 7469 7475 7469  iable Substituti
+00013010: 6f6e 0a0a 5468 6520 602d 2d70 726f 6365  on..The `--proce
+00013020: 7373 2d63 7376 2d6f 6e6c 7960 2028 6f72  ss-csv-only` (or
+00013030: 2060 2d70 6029 206f 7074 696f 6e20 6361   `-p`) option ca
+00013040: 6e20 6265 2075 7365 6420 7769 7468 2060  n be used with `
+00013050: 7964 2d73 7562 6d69 7460 2074 6f20 6f75  yd-submit` to ou
+00013060: 7470 7574 2074 6865 204a 534f 4e20 576f  tput the JSON Wo
+00013070: 726b 2052 6571 7569 7265 6d65 6e74 2061  rk Requirement a
+00013080: 6674 6572 2043 5356 2076 6172 6961 626c  fter CSV variabl
+00013090: 6520 7375 6273 7469 7475 7469 6f6e 7320  e substitutions 
+000130a0: 6f6e 6c79 2c20 7072 696f 7220 746f 2061  only, prior to a
+000130b0: 6c6c 206f 7468 6572 2073 7562 7374 6974  ll other substit
+000130c0: 7574 696f 6e73 2061 6e64 2070 726f 7065  utions and prope
+000130d0: 7274 7920 696e 6865 7269 7461 6e63 6520  rty inheritance 
+000130e0: 6170 706c 6965 6420 6279 2060 7964 2d73  applied by `yd-s
+000130f0: 7562 6d69 7460 2e0a 0a23 2057 6f72 6b65  ubmit`...# Worke
+00013100: 7220 506f 6f6c 2050 726f 7065 7274 6965  r Pool Propertie
+00013110: 730a 0a54 6865 2060 776f 726b 6572 506f  s..The `workerPo
+00013120: 6f6c 6020 7365 6374 696f 6e20 6f66 2074  ol` section of t
+00013130: 6865 2054 4f4d 4c20 6669 6c65 2064 6566  he TOML file def
+00013140: 696e 6573 2074 6865 2070 726f 7065 7274  ines the propert
+00013150: 6965 7320 6f66 2074 6865 2057 6f72 6b65  ies of the Worke
+00013160: 7220 506f 6f6c 2074 6f20 6265 2063 7265  r Pool to be cre
+00013170: 6174 6564 2c20 616e 6420 6973 2075 7365  ated, and is use
+00013180: 6420 6279 2074 6865 2060 7964 2d70 726f  d by the `yd-pro
+00013190: 7669 7369 6f6e 6020 636f 6d6d 616e 642e  vision` command.
+000131a0: 2041 2073 7562 7365 7420 6f66 2074 6865   A subset of the
+000131b0: 2070 726f 7065 7274 6965 7320 6973 2061   properties is a
+000131c0: 6c73 6f20 7573 6564 2062 7920 7468 6520  lso used by the 
+000131d0: 6079 642d 696e 7374 616e 7469 6174 6560  `yd-instantiate`
+000131e0: 2063 6f6d 6d61 6e64 2c20 666f 7220 6372   command, for cr
+000131f0: 6561 7469 6e67 2073 7461 6e64 616c 6f6e  eating standalon
+00013200: 6520 436f 6d70 7574 6520 5265 7175 6972  e Compute Requir
+00013210: 656d 656e 7473 2074 6861 7420 6172 6520  ements that are 
+00013220: 6e6f 7420 6173 736f 6369 6174 6564 2077  not associated w
+00013230: 6974 6820 576f 726b 6572 2050 6f6f 6c73  ith Worker Pools
+00013240: 2e0a 0a54 6865 206f 6e6c 7920 6d61 6e64  ...The only mand
+00013250: 6174 6f72 7920 7072 6f70 6572 7479 2069  atory property i
+00013260: 7320 6074 656d 706c 6174 6549 6460 2e20  s `templateId`. 
+00013270: 416c 6c20 6f74 6865 7220 7072 6f70 6572  All other proper
+00013280: 7469 6573 2068 6176 6520 6465 6661 756c  ties have defaul
+00013290: 7473 2028 6f72 2061 7265 206e 6f74 2072  ts (or are not r
+000132a0: 6571 7569 7265 6429 2e0a 0a54 6865 2066  equired)...The f
+000132b0: 6f6c 6c6f 7769 6e67 2070 726f 7065 7274  ollowing propert
+000132c0: 6965 7320 6172 6520 6176 6169 6c61 626c  ies are availabl
+000132d0: 653a 0a0a 7c20 5072 6f70 6572 7479 2020  e:..| Property  
+000132e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000132f0: 7c20 4465 7363 7269 7074 696f 6e20 2020  | Description   
+00013300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013310: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013320: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013340: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00013350: 6030 6020 2020 2020 2020 2020 2020 2020  `0`             
-00013360: 2020 2020 2020 2020 7c0a 7c20 606d 6178          |.| `max
-00013370: 4e6f 6465 7360 2020 2020 2020 2020 2020  Nodes`          
-00013380: 2020 2020 2020 7c20 5468 6520 6d61 7869        | The maxi
-00013390: 6d75 6d20 6e75 6d62 6572 206f 6620 6e6f  mum number of no
-000133a0: 6465 7320 746f 2077 6869 6368 2074 6865  des to which the
-000133b0: 2057 6f72 6b65 7220 506f 6f6c 2063 616e   Worker Pool can
-000133c0: 2062 6520 7363 616c 6564 2075 702e 2020   be scaled up.  
-000133d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000133e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000133f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013400: 7c20 6031 6020 2020 2020 2020 2020 2020  | `1`           
-00013410: 2020 2020 2020 2020 2020 7c0a 7c20 606e            |.| `n
-00013420: 616d 6560 2020 2020 2020 2020 2020 2020  ame`            
-00013430: 2020 2020 2020 2020 7c20 5468 6520 6e61          | The na
-00013440: 6d65 206f 6620 7468 6520 576f 726b 6572  me of the Worker
-00013450: 2050 6f6f 6c2e 2020 2020 2020 2020 2020   Pool.          
-00013460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000134a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000134b0: 2020 7c20 4175 746f 6d61 7469 6361 6c6c    | Automaticall
-000134c0: 7920 4765 6e65 7261 7465 6420 7c0a 7c20  y Generated |.| 
-000134d0: 606e 6f64 6542 6f6f 7454 696d 656f 7574  `nodeBootTimeout
-000134e0: 6020 2020 2020 2020 2020 7c20 5468 6520  `         | The 
-000134f0: 7469 6d65 2069 6e20 6d69 6e75 7465 7320  time in minutes 
-00013500: 616c 6c6f 7765 6420 666f 7220 6120 6e6f  allowed for a no
-00013510: 6465 2074 6f20 626f 6f74 2061 6e64 2072  de to boot and r
-00013520: 6567 6973 7465 7220 7769 7468 2074 6865  egister with the
-00013530: 2070 6c61 7466 6f72 6d2c 206f 7468 6572   platform, other
-00013540: 7769 7365 2069 7420 7769 6c6c 2062 6520  wise it will be 
-00013550: 7465 726d 696e 6174 6564 2e20 2020 2020  terminated.     
-00013560: 2020 2020 7c20 6031 302e 3060 2020 2020      | `10.0`    
-00013570: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-00013580: 7c20 6074 6172 6765 7449 6e73 7461 6e63  | `targetInstanc
-00013590: 6543 6f75 6e74 6020 2020 2020 7c20 5468  eCount`     | Th
-000135a0: 6520 696e 6974 6961 6c20 6e75 6d62 6572  e initial number
-000135b0: 206f 6620 6e6f 6465 7320 746f 2063 7265   of nodes to cre
-000135c0: 6174 6520 666f 7220 7468 6520 576f 726b  ate for the Work
-000135d0: 6572 2050 6f6f 6c2e 2020 2020 2020 2020  er Pool.        
-000135e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000135f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013610: 2020 2020 2020 7c20 6031 6020 2020 2020        | `1`     
+00013340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013360: 2020 2020 2020 2020 2020 7c20 4465 6661            | Defa
+00013370: 756c 7420 2020 2020 2020 2020 2020 2020  ult             
+00013380: 2020 2020 7c0a 7c3a 2d2d 2d2d 2d2d 2d2d      |.|:--------
+00013390: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000133a0: 2d2d 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --|:------------
+000133b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000133c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000133d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000133e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000133f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00013400: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00013410: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c3a 2d2d  ------------|:--
+00013420: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00013430: 2d2d 2d2d 2d2d 7c0a 7c20 6069 646c 654e  ------|.| `idleN
+00013440: 6f64 6553 6875 7464 6f77 6e45 6e61 626c  odeShutdownEnabl
+00013450: 6564 6020 7c20 5768 6574 6865 7220 746f  ed` | Whether to
+00013460: 2073 6875 7420 646f 776e 206e 6f64 6573   shut down nodes
+00013470: 2074 6861 7420 6861 7665 2062 6565 6e20   that have been 
+00013480: 6964 6c65 2066 6f72 2060 6964 6c65 4e6f  idle for `idleNo
+00013490: 6465 5368 7574 646f 776e 5469 6d65 6f75  deShutdownTimeou
+000134a0: 7460 206d 696e 7574 6573 2e20 2020 2020  t` minutes.     
+000134b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000134c0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+000134d0: 6054 7275 6560 2020 2020 2020 2020 2020  `True`          
+000134e0: 2020 2020 2020 2020 7c0a 7c20 6069 646c          |.| `idl
+000134f0: 654e 6f64 6553 6875 7464 6f77 6e54 696d  eNodeShutdownTim
+00013500: 656f 7574 6020 7c20 5468 6520 7469 6d65  eout` | The time
+00013510: 6f75 7420 696e 206d 696e 7574 6573 2061  out in minutes a
+00013520: 6674 6572 2077 6869 6368 2061 6e20 6964  fter which an id
+00013530: 6c65 206e 6f64 6520 7769 6c6c 2062 6520  le node will be 
+00013540: 7368 7574 2064 6f77 6e20 6966 2060 6964  shut down if `id
+00013550: 6c65 4e6f 6465 5368 7574 646f 776e 456e  leNodeShutdownEn
+00013560: 6162 6c65 6460 2069 7320 7365 7420 746f  abled` is set to
+00013570: 2060 5472 7565 602e 2020 2020 2020 2020   `True`.        
+00013580: 7c20 6035 2e30 6020 2020 2020 2020 2020  | `5.0`         
+00013590: 2020 2020 2020 2020 2020 7c0a 7c20 6069            |.| `i
+000135a0: 646c 6550 6f6f 6c53 6875 7464 6f77 6e45  dlePoolShutdownE
+000135b0: 6e61 626c 6564 6020 7c20 5768 6574 6865  nabled` | Whethe
+000135c0: 7220 746f 2073 6875 7420 646f 776e 2074  r to shut down t
+000135d0: 6865 2057 6f72 6b65 7220 506f 6f6c 2077  he Worker Pool w
+000135e0: 6865 6e20 6974 2068 6173 2062 6565 6e20  hen it has been 
+000135f0: 6964 6c65 2066 6f72 2060 6964 6c65 506f  idle for `idlePo
+00013600: 6f6c 5368 7574 646f 776e 5469 6d65 6f75  olShutdownTimeou
+00013610: 7460 206d 696e 7574 6573 2e20 2020 2020  t` minutes.     
 00013620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013630: 7c0a 7c20 6074 656d 706c 6174 6549 6460  |.| `templateId`
-00013640: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00013650: 5468 6520 5965 6c6c 6f77 446f 6720 436f  The YellowDog Co
-00013660: 6d70 7574 6520 5465 6d70 6c61 7465 2049  mpute Template I
-00013670: 4420 746f 2075 7365 2066 6f72 2070 726f  D to use for pro
-00013680: 7669 7369 6f6e 696e 672e 2028 2a2a 5265  visioning. (**Re
-00013690: 7175 6972 6564 2a2a 2c20 6e6f 2064 6566  quired**, no def
-000136a0: 6175 6c74 2070 726f 7669 6465 642e 2920  ault provided.) 
-000136b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000136c0: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-000136d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000136e0: 2020 7c0a 7c20 6075 7365 7244 6174 6160    |.| `userData`
-000136f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013700: 7c20 5573 6572 2044 6174 6120 746f 2062  | User Data to b
-00013710: 6520 7375 7070 6c69 6564 2074 6f20 696e  e supplied to in
-00013720: 7374 616e 6365 7320 6f6e 2062 6f6f 742e  stances on boot.
-00013730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013630: 2020 7c20 6054 7275 6560 2020 2020 2020    | `True`      
+00013640: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
+00013650: 6069 646c 6550 6f6f 6c53 6875 7464 6f77  `idlePoolShutdow
+00013660: 6e54 696d 656f 7574 6020 7c20 5468 6520  nTimeout` | The 
+00013670: 7469 6d65 6f75 7420 696e 206d 696e 7574  timeout in minut
+00013680: 6573 2061 6674 6572 2077 6869 6368 2061  es after which a
+00013690: 6e20 6964 6c65 2057 6f72 6b65 7220 506f  n idle Worker Po
+000136a0: 6f6c 2077 696c 6c20 6265 2073 6875 7420  ol will be shut 
+000136b0: 646f 776e 2069 6620 6069 646c 6550 6f6f  down if `idlePoo
+000136c0: 6c53 6875 7464 6f77 6e45 6e61 626c 6564  lShutdownEnabled
+000136d0: 6020 6973 2073 6574 2074 6f20 6054 7275  ` is set to `Tru
+000136e0: 6560 2e20 7c20 6033 302e 3060 2020 2020  e`. | `30.0`    
+000136f0: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+00013700: 7c20 6069 6d61 6765 7349 6460 2020 2020  | `imagesId`    
+00013710: 2020 2020 2020 2020 2020 2020 7c20 5468              | Th
+00013720: 6520 696d 6167 6573 2049 4420 746f 2075  e images ID to u
+00013730: 7365 2077 6865 6e20 626f 6f74 696e 6720  se when booting 
+00013740: 696e 7374 616e 6365 732e 2020 2020 2020  instances.      
 00013750: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013770: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
+00013770: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013790: 2020 2020 7c0a 7c20 6075 7365 7244 6174      |.| `userDat
-000137a0: 6146 696c 6560 2020 2020 2020 2020 2020  aFile`          
-000137b0: 2020 7c20 4173 2061 626f 7665 2c20 6275    | As above, bu
-000137c0: 7420 7265 6164 2074 6865 2055 7365 7220  t read the User 
-000137d0: 4461 7461 2066 726f 6d20 7468 6520 6669  Data from the fi
-000137e0: 6c65 6e61 6d65 2073 7570 706c 6965 6420  lename supplied 
-000137f0: 696e 2074 6869 7320 7072 6f70 6572 7479  in this property
-00013800: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
+00013790: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
+000137a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000137b0: 7c0a 7c20 6069 6e73 7461 6e63 6554 6167  |.| `instanceTag
+000137c0: 7360 2020 2020 2020 2020 2020 2020 7c20  s`            | 
+000137d0: 5468 6520 6469 6374 696f 6e61 7279 206f  The dictionary o
+000137e0: 6620 696e 7374 616e 6365 2074 6167 7320  f instance tags 
+000137f0: 746f 2061 7070 6c79 2074 6f20 7468 6520  to apply to the 
+00013800: 696e 7374 616e 6365 732e 2020 2020 2020  instances.      
 00013810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013820: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
+00013820: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013840: 2020 2020 2020 7c0a 7c20 6075 7365 7244        |.| `userD
-00013850: 6174 6146 696c 6573 6020 2020 2020 2020  ataFiles`       
-00013860: 2020 2020 7c20 4173 2061 626f 7665 2c20      | As above, 
-00013870: 6275 7420 6372 6561 7465 2074 6865 2055  but create the U
-00013880: 7365 7220 4461 7461 2062 7920 636f 6e63  ser Data by conc
-00013890: 6174 656e 6174 696e 6720 7468 6520 636f  atenating the co
-000138a0: 6e74 656e 7473 206f 6620 7468 6520 6c69  ntents of the li
-000138b0: 7374 206f 6620 6669 6c65 6e61 6d65 7320  st of filenames 
-000138c0: 7375 7070 6c69 6564 2069 6e20 7468 6973  supplied in this
-000138d0: 2070 726f 7065 7274 792e 2020 2020 7c20   property.    | 
+00013840: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+00013850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013860: 2020 7c0a 7c20 606d 696e 4e6f 6465 7360    |.| `minNodes`
+00013870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013880: 7c20 5468 6520 6d69 6e69 6d75 6d20 6e75  | The minimum nu
+00013890: 6d62 6572 206f 6620 6e6f 6465 7320 746f  mber of nodes to
+000138a0: 2077 6869 6368 2074 6865 2057 6f72 6b65   which the Worke
+000138b0: 7220 506f 6f6c 2063 616e 2062 6520 7363  r Pool can be sc
+000138c0: 616c 6564 2064 6f77 6e2e 2020 2020 2020  aled down.      
+000138d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000138e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000138f0: 2020 2020 2020 2020 7c0a 7c20 6077 6f72          |.| `wor
-00013900: 6b65 7273 5065 7256 4350 5560 2020 2020  kersPerVCPU`    
-00013910: 2020 2020 2020 7c20 5468 6520 6e75 6d62        | The numb
-00013920: 6572 206f 6620 576f 726b 6572 7320 746f  er of Workers to
-00013930: 2065 7374 6162 6c69 7368 2070 6572 2076   establish per v
-00013940: 4350 5520 6f6e 2065 6163 6820 6e6f 6465  CPU on each node
-00013950: 2069 6e20 7468 6520 576f 726b 6572 2050   in the Worker P
-00013960: 6f6f 6c2e 2028 4f76 6572 7269 6465 7320  ool. (Overrides 
-00013970: 6077 6f72 6b65 7273 5065 724e 6f64 6560  `workersPerNode`
-00013980: 2e29 2020 2020 2020 2020 2020 2020 2020  .)              
-00013990: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-000139a0: 2020 2020 2020 2020 2020 7c0a 7c20 6077            |.| `w
-000139b0: 6f72 6b65 7273 5065 724e 6f64 6560 2020  orkersPerNode`  
-000139c0: 2020 2020 2020 2020 7c20 5468 6520 6e75          | The nu
-000139d0: 6d62 6572 206f 6620 576f 726b 6572 7320  mber of Workers 
-000139e0: 746f 2065 7374 6162 6c69 7368 206f 6e20  to establish on 
-000139f0: 6561 6368 206e 6f64 6520 696e 2074 6865  each node in the
-00013a00: 2057 6f72 6b65 7220 506f 6f6c 2e20 2020   Worker Pool.   
+000138f0: 2020 2020 2020 2020 2020 7c20 6030 6020            | `0` 
+00013900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013910: 2020 2020 7c0a 7c20 606d 6178 4e6f 6465      |.| `maxNode
+00013920: 7360 2020 2020 2020 2020 2020 2020 2020  s`              
+00013930: 2020 7c20 5468 6520 6d61 7869 6d75 6d20    | The maximum 
+00013940: 6e75 6d62 6572 206f 6620 6e6f 6465 7320  number of nodes 
+00013950: 746f 2077 6869 6368 2074 6865 2057 6f72  to which the Wor
+00013960: 6b65 7220 506f 6f6c 2063 616e 2062 6520  ker Pool can be 
+00013970: 7363 616c 6564 2075 702e 2020 2020 2020  scaled up.      
+00013980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000139a0: 2020 2020 2020 2020 2020 2020 7c20 6031              | `1
+000139b0: 6020 2020 2020 2020 2020 2020 2020 2020  `               
+000139c0: 2020 2020 2020 7c0a 7c20 606e 616d 6560        |.| `name`
+000139d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000139e0: 2020 2020 7c20 5468 6520 6e61 6d65 206f      | The name o
+000139f0: 6620 7468 6520 576f 726b 6572 2050 6f6f  f the Worker Poo
+00013a00: 6c2e 2020 2020 2020 2020 2020 2020 2020  l.              
 00013a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013a40: 2020 7c20 6031 6020 2020 2020 2020 2020    | `1`         
-00013a50: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
-00013a60: 6077 6f72 6b65 7250 6f6f 6c44 6174 6160  `workerPoolData`
-00013a70: 2020 2020 2020 2020 2020 7c20 5468 6520            | The 
-00013a80: 6e61 6d65 206f 6620 6120 6669 6c65 2063  name of a file c
-00013a90: 6f6e 7461 696e 696e 6720 6120 4a53 4f4e  ontaining a JSON
-00013aa0: 2064 6f63 756d 656e 7420 6465 6669 6e69   document defini
-00013ab0: 6e67 2061 2057 6f72 6b65 7220 506f 6f6c  ng a Worker Pool
-00013ac0: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
-00013ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013af0: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
-00013b00: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-00013b10: 7c20 6077 6f72 6b65 7254 6167 6020 2020  | `workerTag`   
-00013b20: 2020 2020 2020 2020 2020 2020 7c20 5468              | Th
-00013b30: 6520 576f 726b 6572 2054 6167 2074 6f20  e Worker Tag to 
-00013b40: 7075 626c 6973 6820 666f 7220 7468 6520  publish for the 
-00013b50: 616c 6c20 6f66 2074 6865 2057 6f72 6b65  all of the Worke
-00013b60: 7273 206f 6e20 7468 6520 6e6f 6465 2e20  rs on the node. 
-00013b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013a50: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00013a60: 4175 746f 6d61 7469 6361 6c6c 7920 4765  Automatically Ge
+00013a70: 6e65 7261 7465 6420 7c0a 7c20 606e 6f64  nerated |.| `nod
+00013a80: 6542 6f6f 7454 696d 656f 7574 6020 2020  eBootTimeout`   
+00013a90: 2020 2020 2020 7c20 5468 6520 7469 6d65        | The time
+00013aa0: 2069 6e20 6d69 6e75 7465 7320 616c 6c6f   in minutes allo
+00013ab0: 7765 6420 666f 7220 6120 6e6f 6465 2074  wed for a node t
+00013ac0: 6f20 626f 6f74 2061 6e64 2072 6567 6973  o boot and regis
+00013ad0: 7465 7220 7769 7468 2074 6865 2070 6c61  ter with the pla
+00013ae0: 7466 6f72 6d2c 206f 7468 6572 7769 7365  tform, otherwise
+00013af0: 2069 7420 7769 6c6c 2062 6520 7465 726d   it will be term
+00013b00: 696e 6174 6564 2e20 2020 2020 2020 2020  inated.         
+00013b10: 7c20 6031 302e 3060 2020 2020 2020 2020  | `10.0`        
+00013b20: 2020 2020 2020 2020 2020 7c0a 7c20 6074            |.| `t
+00013b30: 6172 6765 7449 6e73 7461 6e63 6543 6f75  argetInstanceCou
+00013b40: 6e74 6020 2020 2020 7c20 5468 6520 696e  nt`     | The in
+00013b50: 6974 6961 6c20 6e75 6d62 6572 206f 6620  itial number of 
+00013b60: 6e6f 6465 7320 746f 2063 7265 6174 6520  nodes to create 
+00013b70: 666f 7220 7468 6520 576f 726b 6572 2050  for the Worker P
+00013b80: 6f6f 6c2e 2020 2020 2020 2020 2020 2020  ool.            
 00013b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013ba0: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
+00013ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013bc0: 7c0a 0a23 2320 4175 746f 6d61 7469 6320  |..## Automatic 
-00013bd0: 5072 6f70 6572 7469 6573 0a0a 5468 6520  Properties..The 
-00013be0: 6e61 6d65 206f 6620 7468 6520 576f 726b  name of the Work
-00013bf0: 6572 2050 6f6f 6c2c 2069 6620 6e6f 7420  er Pool, if not 
-00013c00: 7375 7070 6c69 6564 2c20 6973 2061 7574  supplied, is aut
-00013c10: 6f6d 6174 6963 616c 6c79 2067 656e 6572  omatically gener
-00013c20: 6174 6564 2075 7369 6e67 2061 2063 6f6e  ated using a con
-00013c30: 6361 7465 6e61 7469 6f6e 206f 6620 6077  catenation of `w
-00013c40: 705f 602c 2074 6865 2060 7461 6760 2070  p_`, the `tag` p
-00013c50: 726f 7065 7274 792c 2061 2055 5443 2074  roperty, a UTC t
-00013c60: 696d 6573 7461 6d70 2c20 616e 6420 7468  imestamp, and th
-00013c70: 7265 6520 7261 6e64 6f6d 2068 6578 2063  ree random hex c
-00013c80: 6861 7261 6374 6572 733a 2065 2c67 2c2e  haracters: e,g,.
-00013c90: 2060 7770 5f6d 7974 6167 5f32 3231 3032   `wp_mytag_22102
-00013ca0: 342d 3135 3535 3234 2d62 3061 602e 0a0a  4-155524-b0a`...
-00013cb0: 2323 2054 4f4d 4c20 5072 6f70 6572 7469  ## TOML Properti
-00013cc0: 6573 2069 6e20 7468 6520 6077 6f72 6b65  es in the `worke
-00013cd0: 7250 6f6f 6c60 2053 6563 7469 6f6e 0a0a  rPool` Section..
-00013ce0: 4865 7265 2773 2061 6e20 6578 616d 706c  Here's an exampl
-00013cf0: 6520 6f66 2074 6865 2060 776f 726b 6572  e of the `worker
-00013d00: 506f 6f6c 6020 7365 6374 696f 6e20 6f66  Pool` section of
-00013d10: 2061 2054 4f4d 4c20 636f 6e66 6967 7572   a TOML configur
-00013d20: 6174 696f 6e20 6669 6c65 2c20 7368 6f77  ation file, show
-00013d30: 696e 6720 616c 6c20 7468 6520 706f 7373  ing all the poss
-00013d40: 6962 6c65 2070 726f 7065 7274 6965 7320  ible properties 
-00013d50: 7468 6174 2063 616e 2062 6520 7365 743a  that can be set:
-00013d60: 0a0a 6060 6074 6f6d 6c0a 5b77 6f72 6b65  ..```toml.[worke
-00013d70: 7250 6f6f 6c5d 0a20 2020 2069 646c 654e  rPool].    idleN
-00013d80: 6f64 6553 6875 7464 6f77 6e45 6e61 626c  odeShutdownEnabl
-00013d90: 6564 203d 2074 7275 650a 2020 2020 6964  ed = true.    id
-00013da0: 6c65 4e6f 6465 5368 7574 646f 776e 5469  leNodeShutdownTi
-00013db0: 6d65 6f75 7420 3d20 3130 2e30 0a20 2020  meout = 10.0.   
-00013dc0: 2069 646c 6550 6f6f 6c53 6875 7464 6f77   idlePoolShutdow
-00013dd0: 6e45 6e61 626c 6564 203d 2074 7275 650a  nEnabled = true.
-00013de0: 2020 2020 6964 6c65 506f 6f6c 5368 7574      idlePoolShut
-00013df0: 646f 776e 5469 6d65 6f75 7420 3d20 3630  downTimeout = 60
-00013e00: 2e30 0a20 2020 2069 6d61 6765 7349 6420  .0.    imagesId 
-00013e10: 3d20 2279 6469 643a 696d 6766 616d 3a30  = "ydid:imgfam:0
-00013e20: 3030 3030 303a 3431 3936 3235 3932 2d35  00000:41962592-5
-00013e30: 3737 632d 3466 6465 2d61 6230 332d 6438  77c-4fde-ab03-d8
-00013e40: 3532 3436 3565 3766 3862 220a 2020 2020  52465e7f8b".    
-00013e50: 696e 7374 616e 6365 5461 6773 203d 207b  instanceTags = {
-00013e60: 7d0a 2020 2020 6d61 784e 6f64 6573 203d  }.    maxNodes =
-00013e70: 2031 0a20 2020 206d 696e 4e6f 6465 7320   1.    minNodes 
-00013e80: 3d20 310a 2020 2020 6e61 6d65 203d 2022  = 1.    name = "
-00013e90: 6d79 2d77 6f72 6b65 722d 706f 6f6c 220a  my-worker-pool".
-00013ea0: 2020 2020 6e6f 6465 426f 6f74 5469 6d65      nodeBootTime
-00013eb0: 6f75 7420 3d20 350a 2020 2020 7461 7267  out = 5.    targ
-00013ec0: 6574 496e 7374 616e 6365 436f 756e 7420  etInstanceCount 
-00013ed0: 3d20 310a 2020 2020 7465 6d70 6c61 7465  = 1.    template
-00013ee0: 4964 203d 2022 7964 6964 3a63 7274 3a44  Id = "ydid:crt:D
-00013ef0: 3943 3534 383a 3436 3561 3130 3763 2d37  9C548:465a107c-7
-00013f00: 6365 612d 3436 6533 2d39 6664 642d 3135  cea-46e3-9fdd-15
-00013f10: 3131 3663 6239 3263 3430 220a 2020 2020  116cb92c40".    
-00013f20: 2320 4e6f 7465 3a20 6f6e 6c79 206f 6e65  # Note: only one
-00013f30: 206f 6620 2775 7365 7244 6174 6127 2f27   of 'userData'/'
-00013f40: 7573 6572 4461 7461 4669 6c65 272f 2775  userDataFile'/'u
-00013f50: 7365 7244 6174 6146 696c 6573 2720 7368  serDataFiles' sh
-00013f60: 6f75 6c64 2062 6520 7365 740a 2020 2020  ould be set.    
-00013f70: 7573 6572 4461 7461 203d 2022 220a 2020  userData = "".  
-00013f80: 2020 7573 6572 4461 7461 4669 6c65 203d    userDataFile =
-00013f90: 2022 6d79 7573 6572 6461 7461 2e74 7874   "myuserdata.txt
-00013fa0: 220a 2020 2020 7573 6572 4461 7461 4669  ".    userDataFi
-00013fb0: 6c65 7320 3d20 5b22 6d79 7573 6572 6461  les = ["myuserda
-00013fc0: 7461 312e 7478 7422 2c20 226d 7975 7365  ta1.txt", "myuse
-00013fd0: 7264 6174 6132 2e74 7874 225d 0a20 2020  rdata2.txt"].   
-00013fe0: 2077 6f72 6b65 7254 6167 203d 2022 7461   workerTag = "ta
-00013ff0: 672d 7b7b 7573 6572 6e61 6d65 7d7d 220a  g-{{username}}".
-00014000: 2020 2020 2320 5370 6563 6966 7920 6569      # Specify ei
-00014010: 7468 6572 2077 6f72 6b65 7273 5065 724e  ther workersPerN
-00014020: 6f64 6520 6f72 2077 6f72 6b65 7273 5065  ode or workersPe
-00014030: 7256 4350 550a 2020 2020 776f 726b 6572  rVCPU.    worker
-00014040: 7350 6572 4e6f 6465 203d 2031 0a20 2020  sPerNode = 1.   
-00014050: 2077 6f72 6b65 7273 5065 7256 4350 5520   workersPerVCPU 
-00014060: 3d20 310a 2320 2020 776f 726b 6572 506f  = 1.#   workerPo
-00014070: 6f6c 4461 7461 203d 2022 776f 726b 6572  olData = "worker
-00014080: 5f70 6f6f 6c2e 6a73 6f6e 220a 6060 600a  _pool.json".```.
-00014090: 0a23 2320 576f 726b 6572 2050 6f6f 6c20  .## Worker Pool 
-000140a0: 5370 6563 6966 6963 6174 696f 6e20 5573  Specification Us
-000140b0: 696e 6720 4a53 4f4e 2044 6f63 756d 656e  ing JSON Documen
-000140c0: 7473 0a0a 4974 2773 2061 6c73 6f20 706f  ts..It's also po
-000140d0: 7373 6962 6c65 2074 6f20 6361 7074 7572  ssible to captur
-000140e0: 6520 6120 576f 726b 6572 2050 6f6f 6c20  e a Worker Pool 
-000140f0: 6465 6669 6e69 7469 6f6e 2061 7320 6120  definition as a 
-00014100: 4a53 4f4e 2064 6f63 756d 656e 742e 2054  JSON document. T
-00014110: 6865 204a 534f 4e20 6669 6c65 6e61 6d65  he JSON filename
-00014120: 2063 616e 2062 6520 7375 7070 6c69 6564   can be supplied
-00014130: 2065 6974 6865 7220 7573 696e 6720 7468   either using th
-00014140: 6520 636f 6d6d 616e 6420 6c69 6e65 2077  e command line w
-00014150: 6974 6820 7468 6520 602d 2d77 6f72 6b65  ith the `--worke
-00014160: 722d 706f 6f6c 6020 6f72 2060 2d70 6020  r-pool` or `-p` 
-00014170: 7061 7261 6d65 7465 7220 7769 7468 2060  parameter with `
-00014180: 7964 2d70 726f 7669 7369 6f6e 602c 206f  yd-provision`, o
-00014190: 7220 6279 2070 6f70 756c 6174 696e 6720  r by populating 
-000141a0: 7468 6520 6077 6f72 6b65 7250 6f6f 6c44  the `workerPoolD
-000141b0: 6174 6160 2070 726f 7065 7274 7920 696e  ata` property in
-000141c0: 2074 6865 2054 4f4d 4c20 636f 6e66 6967   the TOML config
-000141d0: 7572 6174 696f 6e20 6669 6c65 2077 6974  uration file wit
-000141e0: 6820 7468 6520 4a53 4f4e 2066 696c 656e  h the JSON filen
-000141f0: 616d 652e 2043 6f6d 6d61 6e64 206c 696e  ame. Command lin
-00014200: 6520 7370 6563 6966 6963 6174 696f 6e20  e specification 
-00014210: 7461 6b65 7320 7072 696f 7269 7479 206f  takes priority o
-00014220: 7665 7220 544f 4d4c 2073 7065 6369 6669  ver TOML specifi
-00014230: 6361 7469 6f6e 2e0a 0a54 6865 204a 534f  cation...The JSO
-00014240: 4e20 7370 6563 6966 6963 6174 696f 6e20  N specification 
-00014250: 616c 6c6f 7773 2074 6865 2063 7265 6174  allows the creat
-00014260: 696f 6e20 6f66 202a 2a41 6476 616e 6365  ion of **Advance
-00014270: 6420 576f 726b 6572 2050 6f6f 6c73 2a2a  d Worker Pools**
-00014280: 2c20 7769 7468 2064 6966 6665 7265 6e74  , with different
-00014290: 206e 6f64 6520 7479 7065 7320 616e 6420   node types and 
-000142a0: 7468 6520 6162 696c 6974 7920 746f 2073  the ability to s
-000142b0: 7065 6369 6679 204e 6f64 6520 4163 7469  pecify Node Acti
-000142c0: 6f6e 732e 0a0a 5768 656e 2075 7369 6e67  ons...When using
-000142d0: 2061 204a 534f 4e20 646f 6375 6d65 6e74   a JSON document
-000142e0: 2074 6f20 7370 6563 6966 7920 7468 6520   to specify the 
-000142f0: 576f 726b 6572 2050 6f6f 6c2c 2074 6865  Worker Pool, the
-00014300: 2073 6368 656d 6120 6f66 2074 6865 2064   schema of the d
-00014310: 6f63 756d 656e 7420 6973 2069 6465 6e74  ocument is ident
-00014320: 6963 616c 2074 6f20 7468 6174 2065 7870  ical to that exp
-00014330: 6563 7465 6420 6279 2074 6865 2059 656c  ected by the Yel
-00014340: 6c6f 7744 6f67 2052 4553 5420 4150 4920  lowDog REST API 
-00014350: 666f 7220 576f 726b 6572 2050 6f6f 6c20  for Worker Pool 
-00014360: 5072 6f76 6973 696f 6e69 6e67 2e0a 0a23  Provisioning...#
-00014370: 2323 2057 6f72 6b65 7220 506f 6f6c 204a  ## Worker Pool J
-00014380: 534f 4e20 4578 616d 706c 6573 0a0a 5468  SON Examples..Th
-00014390: 6520 6578 616d 706c 6520 6265 6c6f 7720  e example below 
-000143a0: 6973 206f 6620 6120 7369 6d70 6c65 204a  is of a simple J
-000143b0: 534f 4e20 7370 6563 6966 6963 6174 696f  SON specificatio
-000143c0: 6e20 6f66 2061 2057 6f72 6b65 7220 506f  n of a Worker Po
-000143d0: 6f6c 2077 6974 6820 6f6e 6520 696e 6974  ol with one init
-000143e0: 6961 6c20 6e6f 6465 2c20 576f 726b 6572  ial node, Worker
-000143f0: 2050 6f6f 6c20 7368 7574 646f 776e 2c20   Pool shutdown, 
-00014400: 6574 632e 0a0a 6060 606a 736f 6e0a 7b0a  etc...```json.{.
-00014410: 2020 2272 6571 7569 7265 6d65 6e74 5465    "requirementTe
-00014420: 6d70 6c61 7465 5573 6167 6522 3a20 7b0a  mplateUsage": {.
-00014430: 2020 2020 226d 6169 6e74 6169 6e49 6e73      "maintainIns
-00014440: 7461 6e63 6543 6f75 6e74 223a 2066 616c  tanceCount": fal
-00014450: 7365 2c0a 2020 2020 2272 6571 7569 7265  se,.    "require
-00014460: 6d65 6e74 4e61 6d65 223a 2022 7770 5f70  mentName": "wp_p
-00014470: 7965 782d 7072 696d 6573 5f32 3330 3131  yex-primes_23011
-00014480: 332d 3136 3135 3238 2d64 6130 222c 0a20  3-161528-da0",. 
-00014490: 2020 2022 7265 7175 6972 656d 656e 744e     "requirementN
-000144a0: 616d 6573 7061 6365 223a 2022 7079 6578  amespace": "pyex
-000144b0: 616d 706c 6573 222c 0a20 2020 2022 7265  amples",.    "re
-000144c0: 7175 6972 656d 656e 7454 6167 223a 2022  quirementTag": "
-000144d0: 7079 6578 2d70 7269 6d65 7322 2c0a 2020  pyex-primes",.  
-000144e0: 2020 2274 6172 6765 7449 6e73 7461 6e63    "targetInstanc
-000144f0: 6543 6f75 6e74 223a 2031 2c0a 2020 2020  eCount": 1,.    
-00014500: 2274 656d 706c 6174 6549 6422 3a20 2279  "templateId": "y
-00014510: 6469 643a 6372 743a 4439 4335 3438 3a34  did:crt:D9C548:4
-00014520: 3635 6131 3037 632d 3763 6561 2d34 3665  65a107c-7cea-46e
-00014530: 332d 3966 6464 2d31 3531 3136 6362 3932  3-9fdd-15116cb92
-00014540: 6334 3022 0a20 207d 2c0a 2020 2270 726f  c40".  },.  "pro
-00014550: 7669 7369 6f6e 6564 5072 6f70 6572 7469  visionedProperti
-00014560: 6573 223a 207b 0a20 2020 2022 6964 6c65  es": {.    "idle
-00014570: 4e6f 6465 5368 7574 646f 776e 223a 207b  NodeShutdown": {
-00014580: 2265 6e61 626c 6564 223a 2074 7275 652c  "enabled": true,
-00014590: 2022 7469 6d65 6f75 7422 3a20 2250 5431   "timeout": "PT1
-000145a0: 304d 227d 2c0a 2020 2020 2269 646c 6550  0M"},.    "idleP
-000145b0: 6f6f 6c53 6875 7464 6f77 6e22 3a20 7b22  oolShutdown": {"
-000145c0: 656e 6162 6c65 6422 3a20 7472 7565 2c20  enabled": true, 
-000145d0: 2274 696d 656f 7574 223a 2022 5054 3148  "timeout": "PT1H
-000145e0: 227d 2c0a 2020 2020 2263 7265 6174 654e  "},.    "createN
-000145f0: 6f64 6557 6f72 6b65 7273 223a 207b 2274  odeWorkers": {"t
-00014600: 6172 6765 7443 6f75 6e74 223a 2031 2c20  argetCount": 1, 
-00014610: 2274 6172 6765 7454 7970 6522 3a20 2250  "targetType": "P
-00014620: 4552 5f56 4350 5522 7d2c 0a20 2020 2022  ER_VCPU"},.    "
-00014630: 6d61 784e 6f64 6573 223a 2035 2c0a 2020  maxNodes": 5,.  
-00014640: 2020 226d 696e 4e6f 6465 7322 3a20 302c    "minNodes": 0,
-00014650: 0a20 2020 2022 6e6f 6465 426f 6f74 5469  .    "nodeBootTi
-00014660: 6d65 6f75 7422 3a20 2250 5435 4d22 2c0a  meout": "PT5M",.
-00014670: 2020 2020 226e 6f64 6549 646c 6547 7261      "nodeIdleGra
-00014680: 6365 5065 7269 6f64 223a 2022 5054 334d  cePeriod": "PT3M
-00014690: 222c 0a20 2020 2022 6e6f 6465 4964 6c65  ",.    "nodeIdle
-000146a0: 5469 6d65 4c69 6d69 7422 3a20 2250 5433  TimeLimit": "PT3
-000146b0: 4d22 2c0a 2020 2020 2277 6f72 6b65 7254  M",.    "workerT
-000146c0: 6167 223a 2022 7079 6578 2d62 6173 682d  ag": "pyex-bash-
-000146d0: 646f 636b 6572 220a 2020 7d0a 7d0a 6060  docker".  }.}.``
-000146e0: 600a 0a54 6865 206e 6578 7420 6578 616d  `..The next exam
-000146f0: 706c 6520 6973 206f 6620 6120 7265 6c61  ple is of a rela
-00014700: 7469 7665 6c79 2072 6963 6820 4a53 4f4e  tively rich JSON
-00014710: 2073 7065 6369 6669 6361 7469 6f6e 206f   specification o
-00014720: 6620 616e 2041 6476 616e 6365 6420 576f  f an Advanced Wo
-00014730: 726b 6572 2050 6f6f 6c2c 2066 726f 6d20  rker Pool, from 
-00014740: 6f6e 6520 6f66 2074 6865 2059 656c 6c6f  one of the Yello
-00014750: 7744 6f67 2064 656d 6f73 2e20 4974 2069  wDog demos. It i
-00014760: 6e63 6c75 6465 7320 6e6f 6465 2073 7065  ncludes node spe
-00014770: 6369 616c 6973 6174 696f 6e2c 2061 6e64  cialisation, and
-00014780: 2061 6374 696f 6e20 6772 6f75 7073 2074   action groups t
-00014790: 6861 7420 7265 7370 6f6e 6420 746f 2074  hat respond to t
-000147a0: 6865 2060 5354 4152 5455 505f 4e4f 4445  he `STARTUP_NODE
-000147b0: 535f 4144 4445 4460 2061 6e64 2060 4e4f  S_ADDED` and `NO
-000147c0: 4445 535f 4144 4445 4460 2065 7665 6e74  DES_ADDED` event
-000147d0: 7320 746f 2064 7269 7665 202a 2a4e 6f64  s to drive **Nod
-000147e0: 6520 4163 7469 6f6e 732a 2a2e 0a0a 6060  e Actions**...``
-000147f0: 606a 736f 6e0a 7b0a 2020 2272 6571 7569  `json.{.  "requi
-00014800: 7265 6d65 6e74 5465 6d70 6c61 7465 5573  rementTemplateUs
-00014810: 6167 6522 3a20 7b0a 2020 2020 226d 6169  age": {.    "mai
-00014820: 6e74 6169 6e49 6e73 7461 6e63 6543 6f75  ntainInstanceCou
-00014830: 6e74 223a 2066 616c 7365 2c0a 2020 2020  nt": false,.    
-00014840: 2274 6172 6765 7449 6e73 7461 6e63 6543  "targetInstanceC
-00014850: 6f75 6e74 223a 2036 2c0a 2020 2020 2274  ount": 6,.    "t
-00014860: 656d 706c 6174 6549 6422 3a20 2279 6469  emplateId": "ydi
-00014870: 643a 6372 743a 4439 4335 3438 3a61 3765  d:crt:D9C548:a7e
-00014880: 6461 3238 372d 6639 6436 2d34 6263 382d  da287-f9d6-4bc8-
-00014890: 6232 6463 2d34 3535 3334 3430 3537 3235  b2dc-45534405725
-000148a0: 3722 2c0a 2020 2020 2272 6571 7569 7265  7",.    "require
-000148b0: 6d65 6e74 4e61 6d65 223a 2022 7770 5f70  mentName": "wp_p
-000148c0: 7965 782d 736c 7572 6d5f 3233 3031 3133  yex-slurm_230113
-000148d0: 2d31 3635 3631 352d 3262 3722 2c0a 2020  -165615-2b7",.  
-000148e0: 2020 2272 6571 7569 7265 6d65 6e74 4e61    "requirementNa
-000148f0: 6d65 7370 6163 6522 3a20 2270 7965 7861  mespace": "pyexa
-00014900: 6d70 6c65 7322 2c0a 2020 2020 2272 6571  mples",.    "req
-00014910: 7569 7265 6d65 6e74 5461 6722 3a20 2270  uirementTag": "p
-00014920: 7965 782d 736c 7572 6d22 0a20 207d 2c0a  yex-slurm".  },.
-00014930: 2020 2270 726f 7669 7369 6f6e 6564 5072    "provisionedPr
-00014940: 6f70 6572 7469 6573 223a 207b 0a20 2020  operties": {.   
-00014950: 2022 6372 6561 7465 4e6f 6465 576f 726b   "createNodeWork
-00014960: 6572 7322 3a20 7b22 7461 7267 6574 436f  ers": {"targetCo
-00014970: 756e 7422 3a20 302c 2022 7461 7267 6574  unt": 0, "target
-00014980: 5479 7065 223a 2022 5045 525f 4e4f 4445  Type": "PER_NODE
-00014990: 227d 2c0a 2020 2020 226e 6f64 6543 6f6e  "},.    "nodeCon
-000149a0: 6669 6775 7261 7469 6f6e 223a 207b 0a20  figuration": {. 
-000149b0: 2020 2020 2022 6e6f 6465 5479 7065 7322       "nodeTypes"
-000149c0: 3a20 5b0a 2020 2020 2020 2020 7b22 6e61  : [.        {"na
-000149d0: 6d65 223a 2022 736c 7572 6d63 746c 6422  me": "slurmctld"
-000149e0: 2c20 2263 6f75 6e74 223a 2031 7d2c 0a20  , "count": 1},. 
-000149f0: 2020 2020 2020 207b 226e 616d 6522 3a20         {"name": 
-00014a00: 2273 6c75 726d 6422 2c20 226d 696e 223a  "slurmd", "min":
-00014a10: 2035 2c20 2273 6c6f 744e 756d 6265 7269   5, "slotNumberi
-00014a20: 6e67 223a 2022 5245 5553 4142 4c45 227d  ng": "REUSABLE"}
-00014a30: 0a20 2020 2020 205d 2c0a 2020 2020 2020  .      ],.      
-00014a40: 226e 6f64 6545 7665 6e74 7322 3a20 7b0a  "nodeEvents": {.
-00014a50: 2020 2020 2020 2020 2253 5441 5254 5550          "STARTUP
-00014a60: 5f4e 4f44 4553 5f41 4444 4544 223a 205b  _NODES_ADDED": [
-00014a70: 0a20 2020 2020 2020 2020 207b 0a20 2020  .          {.   
-00014a80: 2020 2020 2020 2020 2022 6163 7469 6f6e           "action
-00014a90: 7322 3a20 5b0a 2020 2020 2020 2020 2020  s": [.          
-00014aa0: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
-00014ab0: 2020 2020 2020 2261 6374 696f 6e22 3a20        "action": 
-00014ac0: 2257 5249 5445 5f46 494c 4522 2c0a 2020  "WRITE_FILE",.  
-00014ad0: 2020 2020 2020 2020 2020 2020 2020 2270                "p
-00014ae0: 6174 6822 3a20 226e 6f64 6573 2e6a 736f  ath": "nodes.jso
-00014af0: 6e22 2c0a 2020 2020 2020 2020 2020 2020  n",.            
-00014b00: 2020 2020 2263 6f6e 7465 6e74 223a 2022      "content": "
-00014b10: 7b5c 6e20 205c 226e 6f64 6573 5c22 3a20  {\n  \"nodes\": 
-00014b20: 5b5c 6e7b 7b23 6f74 6865 724e 6f64 6573  [\n{{#otherNodes
-00014b30: 7d7d 5c6e 2020 2020 7b5c 6e20 2020 2020  }}\n    {\n     
-00014b40: 205c 226e 616d 655c 223a 205c 2273 6c75   \"name\": \"slu
-00014b50: 726d 647b 7b64 6574 6169 6c73 2e6e 6f64  rmd{{details.nod
-00014b60: 6553 6c6f 747d 7d5c 222c 5c6e 2020 2020  eSlot}}\",\n    
-00014b70: 2020 5c22 6970 5c22 3a20 5c22 7b7b 6465    \"ip\": \"{{de
-00014b80: 7461 696c 732e 7072 6976 6174 6549 7041  tails.privateIpA
-00014b90: 6464 7265 7373 7d7d 5c22 5c6e 2020 2020  ddress}}\"\n    
-00014ba0: 7d7b 7b5e 2d6c 6173 747d 7d2c 7b7b 2f2d  }{{^-last}},{{/-
-00014bb0: 6c61 7374 7d7d 5c6e 7b7b 2f6f 7468 6572  last}}\n{{/other
-00014bc0: 4e6f 6465 737d 7d5c 6e20 205d 5c6e 7d22  Nodes}}\n  ]\n}"
-00014bd0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00014be0: 2020 226e 6f64 6554 7970 6573 223a 205b    "nodeTypes": [
-00014bf0: 2273 6c75 726d 6374 6c64 225d 0a20 2020  "slurmctld"].   
-00014c00: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
-00014c10: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
-00014c20: 2020 2020 2020 2020 2020 2020 2020 2261                "a
-00014c30: 6374 696f 6e22 3a20 2252 554e 5f43 4f4d  ction": "RUN_COM
-00014c40: 4d41 4e44 222c 0a20 2020 2020 2020 2020  MAND",.         
-00014c50: 2020 2020 2020 2022 7061 7468 223a 2022         "path": "
-00014c60: 7374 6172 745f 7369 6d70 6c65 5f73 6c75  start_simple_slu
-00014c70: 726d 6374 6c64 222c 0a20 2020 2020 2020  rmctld",.       
-00014c80: 2020 2020 2020 2020 2022 6172 6775 6d65           "argume
-00014c90: 6e74 7322 3a20 5b22 6e6f 6465 732e 6a73  nts": ["nodes.js
-00014ca0: 6f6e 225d 2c0a 2020 2020 2020 2020 2020  on"],.          
-00014cb0: 2020 2020 2020 2265 6e76 6972 6f6e 6d65        "environme
-00014cc0: 6e74 223a 207b 2245 5841 4d50 4c45 223a  nt": {"EXAMPLE":
-00014cd0: 2022 464f 4f22 7d2c 0a20 2020 2020 2020   "FOO"},.       
-00014ce0: 2020 2020 2020 2020 2022 6e6f 6465 5479           "nodeTy
-00014cf0: 7065 7322 3a20 5b22 736c 7572 6d63 746c  pes": ["slurmctl
-00014d00: 6422 5d0a 2020 2020 2020 2020 2020 2020  d"].            
-00014d10: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
-00014d20: 5d0a 2020 2020 2020 2020 2020 7d2c 0a20  ].          },. 
-00014d30: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
-00014d40: 2020 2020 2020 2022 6163 7469 6f6e 7322         "actions"
-00014d50: 3a20 5b0a 2020 2020 2020 2020 2020 2020  : [.            
-00014d60: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
-00014d70: 2020 2020 2261 6374 696f 6e22 3a20 2252      "action": "R
-00014d80: 554e 5f43 4f4d 4d41 4e44 222c 0a20 2020  UN_COMMAND",.   
-00014d90: 2020 2020 2020 2020 2020 2020 2022 7061               "pa
-00014da0: 7468 223a 2022 7374 6172 745f 7369 6d70  th": "start_simp
-00014db0: 6c65 5f73 6c75 726d 6422 2c0a 2020 2020  le_slurmd",.    
-00014dc0: 2020 2020 2020 2020 2020 2020 2261 7267              "arg
-00014dd0: 756d 656e 7473 223a 205b 227b 7b6e 6f64  uments": ["{{nod
-00014de0: 6573 4279 5479 7065 2e73 6c75 726d 6374  esByType.slurmct
-00014df0: 6c64 2e30 2e64 6574 6169 6c73 2e70 7269  ld.0.details.pri
-00014e00: 7661 7465 4970 4164 6472 6573 737d 7d22  vateIpAddress}}"
-00014e10: 2c20 227b 7b6e 6f64 652e 6465 7461 696c  , "{{node.detail
-00014e20: 732e 6e6f 6465 536c 6f74 7d7d 225d 2c0a  s.nodeSlot}}"],.
-00014e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014e40: 226e 6f64 6554 7970 6573 223a 205b 2273  "nodeTypes": ["s
-00014e50: 6c75 726d 6422 5d0a 2020 2020 2020 2020  lurmd"].        
-00014e60: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00014e70: 2020 2020 5d0a 2020 2020 2020 2020 2020      ].          
-00014e80: 7d2c 0a20 2020 2020 2020 2020 207b 0a20  },.          {. 
-00014e90: 2020 2020 2020 2020 2020 2022 6163 7469             "acti
-00014ea0: 6f6e 7322 3a20 5b0a 2020 2020 2020 2020  ons": [.        
-00014eb0: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-00014ec0: 2020 2020 2020 2020 2261 6374 696f 6e22          "action"
-00014ed0: 3a20 2243 5245 4154 455f 574f 524b 4552  : "CREATE_WORKER
-00014ee0: 5322 2c0a 2020 2020 2020 2020 2020 2020  S",.            
-00014ef0: 2020 2020 2274 6f74 616c 576f 726b 6572      "totalWorker
-00014f00: 7322 3a20 312c 0a20 2020 2020 2020 2020  s": 1,.         
-00014f10: 2020 2020 2020 2022 6e6f 6465 5479 7065         "nodeType
-00014f20: 7322 3a20 5b22 736c 7572 6d63 746c 6422  s": ["slurmctld"
-00014f30: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-00014f40: 7d0a 2020 2020 2020 2020 2020 2020 5d0a  }.            ].
-00014f50: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-00014f60: 2020 2020 5d2c 0a20 2020 2020 2020 2022      ],.        "
-00014f70: 4e4f 4445 535f 4144 4445 4422 3a20 5b0a  NODES_ADDED": [.
-00014f80: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
-00014f90: 2020 2020 2020 2020 2261 6374 696f 6e73          "actions
-00014fa0: 223a 205b 0a20 2020 2020 2020 2020 2020  ": [.           
-00014fb0: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
-00014fc0: 2020 2020 2022 6163 7469 6f6e 223a 2022       "action": "
-00014fd0: 5752 4954 455f 4649 4c45 222c 0a20 2020  WRITE_FILE",.   
-00014fe0: 2020 2020 2020 2020 2020 2020 2022 7061               "pa
-00014ff0: 7468 223a 2022 6e6f 6465 732e 6a73 6f6e  th": "nodes.json
-00015000: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00015010: 2020 2022 636f 6e74 656e 7422 3a20 227b     "content": "{
-00015020: 5c6e 2020 5c22 6e6f 6465 735c 223a 205b  \n  \"nodes\": [
-00015030: 5c6e 7b7b 2366 696c 7465 7265 644e 6f64  \n{{#filteredNod
-00015040: 6573 7d7d 5c6e 2020 2020 7b5c 6e20 2020  es}}\n    {\n   
-00015050: 2020 205c 226e 616d 655c 223a 205c 2273     \"name\": \"s
-00015060: 6c75 726d 647b 7b64 6574 6169 6c73 2e6e  lurmd{{details.n
-00015070: 6f64 6553 6c6f 747d 7d5c 222c 5c6e 2020  odeSlot}}\",\n  
-00015080: 2020 2020 5c22 6970 5c22 3a20 5c22 7b7b      \"ip\": \"{{
-00015090: 6465 7461 696c 732e 7072 6976 6174 6549  details.privateI
-000150a0: 7041 6464 7265 7373 7d7d 5c22 5c6e 2020  pAddress}}\"\n  
-000150b0: 2020 7d7b 7b5e 2d6c 6173 747d 7d2c 7b7b    }{{^-last}},{{
-000150c0: 2f2d 6c61 7374 7d7d 5c6e 7b7b 2f66 696c  /-last}}\n{{/fil
-000150d0: 7465 7265 644e 6f64 6573 7d7d 5c6e 2020  teredNodes}}\n  
-000150e0: 5d5c 6e7d 222c 0a20 2020 2020 2020 2020  ]\n}",.         
-000150f0: 2020 2020 2020 2022 6e6f 6465 5479 7065         "nodeType
-00015100: 7322 3a20 5b22 736c 7572 6d63 746c 6422  s": ["slurmctld"
-00015110: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-00015120: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
-00015130: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00015140: 2020 2022 6163 7469 6f6e 223a 2022 5255     "action": "RU
-00015150: 4e5f 434f 4d4d 414e 4422 2c0a 2020 2020  N_COMMAND",.    
-00015160: 2020 2020 2020 2020 2020 2020 2270 6174              "pat
-00015170: 6822 3a20 2261 6464 5f6e 6f64 6573 222c  h": "add_nodes",
-00015180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015190: 2022 6172 6775 6d65 6e74 7322 3a20 5b22   "arguments": ["
-000151a0: 6e6f 6465 732e 6a73 6f6e 225d 2c0a 2020  nodes.json"],.  
-000151b0: 2020 2020 2020 2020 2020 2020 2020 226e                "n
-000151c0: 6f64 6554 7970 6573 223a 205b 2273 6c75  odeTypes": ["slu
-000151d0: 726d 6374 6c64 225d 0a20 2020 2020 2020  rmctld"].       
-000151e0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-000151f0: 2020 2020 205d 0a20 2020 2020 2020 2020       ].         
-00015200: 207d 2c0a 2020 2020 2020 2020 2020 7b0a   },.          {.
-00015210: 2020 2020 2020 2020 2020 2020 2261 6374              "act
-00015220: 696f 6e73 223a 205b 0a20 2020 2020 2020  ions": [.       
-00015230: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
-00015240: 2020 2020 2020 2020 2022 6163 7469 6f6e           "action
-00015250: 223a 2022 5255 4e5f 434f 4d4d 414e 4422  ": "RUN_COMMAND"
-00015260: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00015270: 2020 2270 6174 6822 3a20 2273 7461 7274    "path": "start
-00015280: 5f73 696d 706c 655f 736c 7572 6d64 222c  _simple_slurmd",
-00015290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000152a0: 2022 6172 6775 6d65 6e74 7322 3a20 5b22   "arguments": ["
-000152b0: 7b7b 6e6f 6465 7342 7954 7970 652e 736c  {{nodesByType.sl
-000152c0: 7572 6d63 746c 642e 302e 6465 7461 696c  urmctld.0.detail
-000152d0: 732e 7072 6976 6174 6549 7041 6464 7265  s.privateIpAddre
-000152e0: 7373 7d7d 222c 2022 7b7b 6e6f 6465 2e64  ss}}", "{{node.d
-000152f0: 6574 6169 6c73 2e6e 6f64 6553 6c6f 747d  etails.nodeSlot}
-00015300: 7d22 5d2c 0a20 2020 2020 2020 2020 2020  }"],.           
-00015310: 2020 2020 2022 6e6f 6465 4964 4669 6c74       "nodeIdFilt
-00015320: 6572 223a 2022 4556 454e 5422 2c0a 2020  er": "EVENT",.  
-00015330: 2020 2020 2020 2020 2020 2020 2020 226e                "n
-00015340: 6f64 6554 7970 6573 223a 205b 2273 6c75  odeTypes": ["slu
-00015350: 726d 6422 5d0a 2020 2020 2020 2020 2020  rmd"].          
-00015360: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
-00015370: 2020 5d0a 2020 2020 2020 2020 2020 7d0a    ].          }.
-00015380: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
-00015390: 7d0a 2020 2020 7d2c 0a20 2020 2022 776f  }.    },.    "wo
-000153a0: 726b 6572 5461 6722 3a20 2270 7965 782d  rkerTag": "pyex-
-000153b0: 736c 7572 6d2d 636c 7573 7465 7222 0a20  slurm-cluster". 
-000153c0: 207d 0a7d 0a60 6060 0a0a 2323 2320 544f   }.}.```..### TO
-000153d0: 4d4c 2050 726f 7065 7274 6965 7320 496e  ML Properties In
-000153e0: 6865 7269 7465 6420 6279 2057 6f72 6b65  herited by Worke
-000153f0: 7220 506f 6f6c 204a 534f 4e20 5370 6563  r Pool JSON Spec
-00015400: 6966 6963 6174 696f 6e73 0a0a 5768 656e  ifications..When
-00015410: 2061 204a 534f 4e20 576f 726b 6572 2050   a JSON Worker P
-00015420: 6f6f 6c20 7370 6563 6966 6963 6174 696f  ool specificatio
-00015430: 6e20 6973 2075 7365 642c 2074 6865 2066  n is used, the f
-00015440: 6f6c 6c6f 7769 6e67 2070 726f 7065 7274  ollowing propert
-00015450: 6965 7320 6672 6f6d 2074 6865 2060 636f  ies from the `co
-00015460: 6e66 6967 2e74 6f6d 6c60 2066 696c 6520  nfig.toml` file 
-00015470: 7769 6c6c 2062 6520 696e 6865 7269 7465  will be inherite
-00015480: 6420 6966 2074 6865 2076 616c 7565 2069  d if the value i
-00015490: 7320 6162 7365 6e74 2069 6e20 7468 6520  s absent in the 
-000154a0: 4a53 4f4e 2066 696c 653a 0a0a 2a2a 5072  JSON file:..**Pr
-000154b0: 6f70 6572 7469 6573 2049 6e68 6572 6974  operties Inherit
-000154c0: 6564 2077 6974 6869 6e20 7468 6520 6072  ed within the `r
-000154d0: 6571 7569 7265 6d65 6e74 5465 6d70 6c61  equirementTempla
-000154e0: 7465 5573 6167 6560 2070 726f 7065 7274  teUsage` propert
-000154f0: 792a 2a0a 0a2d 2060 696d 6167 6573 4964  y**..- `imagesId
-00015500: 600a 2d20 6069 6e73 7461 6e63 6554 6167  `.- `instanceTag
-00015510: 7360 0a2d 2060 7265 7175 6972 656d 656e  s`.- `requiremen
-00015520: 744e 616d 6560 3a20 6465 7269 7665 6420  tName`: derived 
-00015530: 6672 6f6d 2074 6865 2060 6e61 6d65 6020  from the `name` 
-00015540: 7072 6f70 6572 7479 2069 6e20 7468 6520  property in the 
-00015550: 6054 4f4d 4c60 2063 6f6e 6669 6775 7261  `TOML` configura
-00015560: 7469 6f6e 2e20 2854 6865 206e 616d 6520  tion. (The name 
-00015570: 7769 6c6c 2062 6520 6765 6e65 7261 7465  will be generate
-00015580: 6420 6175 746f 6d61 7469 6361 6c6c 7920  d automatically 
-00015590: 6966 206e 6f74 2073 7570 706c 6965 6420  if not supplied 
-000155a0: 696e 2065 6974 6865 7220 7468 6520 544f  in either the TO
-000155b0: 4d4c 2066 696c 6520 6f72 2074 6865 204a  ML file or the J
-000155c0: 534f 4e20 7370 6563 6966 6963 6174 696f  SON specificatio
-000155d0: 6e2e 290a 2d20 6072 6571 7569 7265 6d65  n.).- `requireme
-000155e0: 6e74 4e61 6d65 7370 6163 6560 3a20 6465  ntNamespace`: de
-000155f0: 7269 7665 6420 6672 6f6d 2074 6865 2060  rived from the `
-00015600: 6e61 6d65 7370 6163 6560 2070 726f 7065  namespace` prope
-00015610: 7274 7920 696e 2074 6865 2060 544f 4d4c  rty in the `TOML
-00015620: 6020 636f 6e66 6967 7572 6174 696f 6e0a  ` configuration.
-00015630: 2d20 6072 6571 7569 7265 6d65 6e74 5461  - `requirementTa
-00015640: 6760 3a20 3a20 6465 7269 7665 6420 6672  g`: : derived fr
-00015650: 6f6d 2074 6865 2060 7461 6760 2070 726f  om the `tag` pro
-00015660: 7065 7274 7920 696e 2074 6865 2060 544f  perty in the `TO
-00015670: 4d4c 6020 636f 6e66 6967 7572 6174 696f  ML` configuratio
-00015680: 6e0a 2d20 6074 6172 6765 7449 6e73 7461  n.- `targetInsta
-00015690: 6e63 6543 6f75 6e74 600a 2d20 6074 656d  nceCount`.- `tem
-000156a0: 706c 6174 6549 6460 0a2d 2060 7573 6572  plateId`.- `user
-000156b0: 4461 7461 600a 2d20 6075 7365 7244 6174  Data`.- `userDat
-000156c0: 6146 696c 6560 0a2d 2060 7573 6572 4461  aFile`.- `userDa
-000156d0: 7461 4669 6c65 7360 0a0a 2a2a 5072 6f70  taFiles`..**Prop
-000156e0: 6572 7469 6573 2049 6e68 6572 6974 6564  erties Inherited
-000156f0: 2077 6974 6869 6e20 7468 6520 6070 726f   within the `pro
-00015700: 7669 7369 6f6e 6564 5072 6f70 6572 7469  visionedProperti
-00015710: 6573 6020 5072 6f70 6572 7479 2a2a 0a0a  es` Property**..
-00015720: 2d20 6069 646c 654e 6f64 6553 6875 7464  - `idleNodeShutd
-00015730: 6f77 6e45 6e61 626c 6564 600a 2d20 6069  ownEnabled`.- `i
-00015740: 646c 654e 6f64 6553 6875 7464 6f77 6e54  dleNodeShutdownT
-00015750: 696d 656f 7574 600a 2d20 6069 646c 6550  imeout`.- `idleP
-00015760: 6f6f 6c53 6875 7464 6f77 6e45 6e61 626c  oolShutdownEnabl
-00015770: 6564 600a 2d20 6069 646c 6550 6f6f 6c53  ed`.- `idlePoolS
-00015780: 6875 7464 6f77 6e54 696d 656f 7574 600a  hutdownTimeout`.
-00015790: 2d20 606e 6f64 6542 6f6f 7454 696d 656f  - `nodeBootTimeo
-000157a0: 7574 600a 2d20 6077 6f72 6b65 7254 6167  ut`.- `workerTag
-000157b0: 600a 0a23 2320 5661 7269 6162 6c65 2053  `..## Variable S
-000157c0: 7562 7374 6974 7574 696f 6e73 2069 6e20  ubstitutions in 
-000157d0: 576f 726b 6572 2050 6f6f 6c20 5072 6f70  Worker Pool Prop
-000157e0: 6572 7469 6573 0a0a 5661 7269 6162 6c65  erties..Variable
-000157f0: 2073 7562 7374 6974 7574 696f 6e73 2063   substitutions c
-00015800: 616e 2062 6520 7573 6564 2077 6974 6869  an be used withi
-00015810: 6e20 616e 7920 7072 6f70 6572 7479 2076  n any property v
-00015820: 616c 7565 2069 6e20 544f 4d4c 2063 6f6e  alue in TOML con
-00015830: 6669 6775 7261 7469 6f6e 2066 696c 6573  figuration files
-00015840: 206f 7220 576f 726b 6572 2050 6f6f 6c20   or Worker Pool 
-00015850: 4a53 4f4e 2066 696c 6573 2e20 5365 6520  JSON files. See 
-00015860: 7468 6520 6465 7363 7269 7074 696f 6e20  the description 
-00015870: 5b61 626f 7665 5d28 2376 6172 6961 626c  [above](#variabl
-00015880: 652d 7375 6273 7469 7475 7469 6f6e 7329  e-substitutions)
-00015890: 2066 6f72 206d 6f72 6520 6465 7461 696c   for more detail
-000158a0: 7320 6f6e 2076 6172 6961 626c 6520 7375  s on variable su
-000158b0: 6273 7469 7475 7469 6f6e 732e 2054 6869  bstitutions. Thi
-000158c0: 7320 6973 2061 2070 6f77 6572 6675 6c20  s is a powerful 
-000158d0: 6665 6174 7572 6520 7468 6174 2061 6c6c  feature that all
-000158e0: 6f77 7320 576f 726b 6572 2050 6f6f 6c73  ows Worker Pools
-000158f0: 2074 6f20 6265 2070 6172 616d 6574 6572   to be parameter
-00015900: 6973 6564 2062 7920 7375 7070 6c79 696e  ised by supplyin
-00015910: 6720 7661 6c75 6573 206f 6e20 7468 6520  g values on the 
-00015920: 636f 6d6d 616e 6420 6c69 6e65 2c20 7669  command line, vi
-00015930: 6120 656e 7669 726f 6e6d 656e 7420 7661  a environment va
-00015940: 7269 6162 6c65 732c 206f 7220 7669 6120  riables, or via 
-00015950: 7468 6520 544f 4d4c 2066 696c 652e 0a0a  the TOML file...
-00015960: 416e 2069 6d70 6f72 7461 6e74 2064 6973  An important dis
-00015970: 7469 6e63 7469 6f6e 202a 2a6f 6e6c 792a  tinction **only*
-00015980: 2a20 7768 656e 2075 7369 6e67 2076 6172  * when using var
-00015990: 6961 626c 6520 7375 6273 7469 7475 7469  iable substituti
-000159a0: 6f6e 7320 7769 7468 696e 2057 6f72 6b65  ons within Worke
-000159b0: 7220 506f 6f6c 204a 534f 4e20 646f 6375  r Pool JSON docu
-000159c0: 6d65 6e74 7320 6973 2074 6861 7420 6561  ments is that ea
-000159d0: 6368 2064 6972 6563 7469 7665 202a 2a6d  ch directive **m
-000159e0: 7573 7420 6265 2070 7265 6365 6465 6420  ust be preceded 
-000159f0: 6279 2061 2060 5f5f 6020 2864 6f75 626c  by a `__` (doubl
-00015a00: 6520 756e 6465 7273 636f 7265 292a 2a20  e underscore)** 
-00015a10: 746f 2064 6973 616d 6269 6775 6174 6520  to disambiguate 
-00015a20: 6974 2066 726f 6d20 7661 7269 6162 6c65  it from variable
-00015a30: 2073 7562 7374 6974 7574 696f 6e73 2074   substitutions t
-00015a40: 6861 7420 6172 6520 746f 2062 6520 7061  hat are to be pa
-00015a50: 7373 6564 2064 6972 6563 746c 7920 746f  ssed directly to
-00015a60: 2074 6865 2041 5049 2e20 466f 7220 6578   the API. For ex
-00015a70: 616d 706c 652c 2075 7365 3a20 605f 5f7b  ample, use: `__{
-00015a80: 7b75 7365 726e 616d 657d 7d60 2074 6f20  {username}}` to 
-00015a90: 6170 706c 7920 6120 7375 6273 7469 7475  apply a substitu
-00015aa0: 7469 6f6e 2066 6f72 2074 6865 2060 7573  tion for the `us
-00015ab0: 6572 6e61 6d65 6020 6465 6661 756c 7420  ername` default 
-00015ac0: 7375 6273 7469 7475 7469 6f6e 2e0a 0a23  substitution...#
-00015ad0: 2320 4472 792d 5275 6e6e 696e 6720 576f  # Dry-Running Wo
-00015ae0: 726b 6572 2050 6f6f 6c20 5072 6f76 6973  rker Pool Provis
-00015af0: 696f 6e69 6e67 0a0a 546f 2065 7861 6d69  ioning..To exami
-00015b00: 6e65 2074 6865 204a 534f 4e20 7468 6174  ne the JSON that
-00015b10: 2077 696c 6c20 6163 7475 616c 6c79 2062   will actually b
-00015b20: 6520 7365 6e74 2074 6f20 7468 6520 5965  e sent to the Ye
-00015b30: 6c6c 6f77 446f 6720 4150 4920 6166 7465  llowDog API afte
-00015b40: 7220 616c 6c20 7072 6f63 6573 7369 6e67  r all processing
-00015b50: 2c20 7573 6520 7468 6520 602d 2d64 7279  , use the `--dry
-00015b60: 2d72 756e 6020 636f 6d6d 616e 6420 6c69  -run` command li
-00015b70: 6e65 206f 7074 696f 6e20 7768 656e 2072  ne option when r
-00015b80: 756e 6e69 6e67 2060 7964 2d70 726f 7669  unning `yd-provi
-00015b90: 7369 6f6e 602e 2054 6869 7320 7769 6c6c  sion`. This will
-00015ba0: 2070 7269 6e74 2074 6865 204a 534f 4e20   print the JSON 
-00015bb0: 7370 6563 6966 6963 6174 696f 6e20 666f  specification fo
-00015bc0: 7220 7468 6520 576f 726b 6572 2050 6f6f  r the Worker Poo
-00015bd0: 6c2e 204e 6f74 6869 6e67 2077 696c 6c20  l. Nothing will 
-00015be0: 6265 2073 7562 6d69 7474 6564 2074 6f20  be submitted to 
-00015bf0: 7468 6520 706c 6174 666f 726d 2e0a 0a54  the platform...T
-00015c00: 6865 2067 656e 6572 6174 6564 204a 534f  he generated JSO
-00015c10: 4e20 6973 2070 726f 6475 6365 6420 6166  N is produced af
-00015c20: 7465 7220 616c 6c20 7072 6f63 6573 7369  ter all processi
-00015c30: 6e67 2028 696e 636f 7270 6f72 6174 696e  ng (incorporatin
-00015c40: 6720 6063 6f6e 6669 672e 746f 6d6c 6020  g `config.toml` 
-00015c50: 7072 6f70 6572 7469 6573 2c20 7661 7269  properties, vari
-00015c60: 6162 6c65 2073 7562 7374 6974 7574 696f  able substitutio
-00015c70: 6e73 2c20 6574 632e 2920 6861 7320 6265  ns, etc.) has be
-00015c80: 656e 2063 6f6e 636c 7564 6564 2c20 736f  en concluded, so
-00015c90: 2074 6865 2064 7279 2d72 756e 2069 7320   the dry-run is 
-00015ca0: 7573 6566 756c 2066 6f72 2069 6e73 7065  useful for inspe
-00015cb0: 6374 696e 6720 7468 6520 7265 7375 6c74  cting the result
-00015cc0: 7320 6f66 2061 6c6c 2074 6865 2070 726f  s of all the pro
-00015cd0: 6365 7373 696e 6720 7468 6174 2773 2062  cessing that's b
-00015ce0: 6565 6e20 7065 7266 6f72 6d65 642e 0a0a  een performed...
-00015cf0: 546f 2073 7570 7072 6573 7320 616c 6c20  To suppress all 
-00015d00: 6f75 7470 7574 2065 7863 6570 7420 666f  output except fo
-00015d10: 7220 7468 6520 4a53 4f4e 2069 7473 656c  r the JSON itsel
-00015d20: 662c 2075 7365 2074 6865 2060 2d2d 7175  f, use the `--qu
-00015d30: 6965 7460 2028 602d 7160 2920 636f 6d6d  iet` (`-q`) comm
-00015d40: 616e 6420 6c69 6e65 206f 7074 696f 6e2e  and line option.
-00015d50: 0a0a 5468 6520 4a53 4f4e 2064 7279 2d72  ..The JSON dry-r
-00015d60: 756e 206f 7574 7075 7420 636f 756c 6420  un output could 
-00015d70: 6974 7365 6c66 2062 6520 7573 6564 2062  itself be used b
-00015d80: 7920 6079 642d 7072 6f76 6973 696f 6e60  y `yd-provision`
-00015d90: 2c20 6966 2063 6170 7475 7265 6420 696e  , if captured in
-00015da0: 2061 2066 696c 652c 2065 2e67 2e3a 0a0a   a file, e.g.:..
-00015db0: 6060 6073 6865 6c6c 0a79 642d 7072 6f76  ```shell.yd-prov
-00015dc0: 6973 696f 6e20 2d2d 6472 792d 7275 6e20  ision --dry-run 
-00015dd0: 2d71 203e 206d 795f 776f 726b 6572 5f70  -q > my_worker_p
-00015de0: 6f6f 6c2e 6a73 6f6e 0a79 642d 7072 6f76  ool.json.yd-prov
-00015df0: 6973 696f 6e20 2d70 206d 795f 776f 726b  ision -p my_work
-00015e00: 6572 5f70 6f6f 6c2e 6a73 6f6e 0a60 6060  er_pool.json.```
-00015e10: 0a0a 2320 4a73 6f6e 6e65 7420 5375 7070  ..# Jsonnet Supp
-00015e20: 6f72 740a 0a49 6e20 616c 6c20 6369 7263  ort..In all circ
-00015e30: 756d 7374 616e 6365 7320 7768 6572 6520  umstances where 
-00015e40: 4a53 4f4e 2066 696c 6573 2061 7265 2075  JSON files are u
-00015e50: 7365 6420 6279 2074 6865 2050 7974 686f  sed by the Pytho
-00015e60: 6e20 4578 616d 706c 6573 2073 6372 6970  n Examples scrip
-00015e70: 7473 2c20 202a 2a5b 4a73 6f6e 6e65 745d  ts,  **[Jsonnet]
-00015e80: 2868 7474 7073 3a2f 2f6a 736f 6e6e 6574  (https://jsonnet
-00015e90: 2e6f 7267 292a 2a20 6669 6c65 7320 6361  .org)** files ca
-00015ea0: 6e20 6265 2075 7365 6420 696e 7374 6561  n be used instea
-00015eb0: 642e 2054 6869 7320 616c 6c6f 7773 2074  d. This allows t
-00015ec0: 6865 2075 7365 206f 6620 4a73 6f6e 6e65  he use of Jsonne
-00015ed0: 7427 7320 706f 7765 7266 756c 204a 534f  t's powerful JSO
-00015ee0: 4e20 6578 7465 6e73 696f 6e73 2c20 696e  N extensions, in
-00015ef0: 636c 7564 696e 6720 636f 6d6d 656e 7473  cluding comments
-00015f00: 2c20 7661 7269 6162 6c65 732c 2066 756e  , variables, fun
-00015f10: 6374 696f 6e73 2c20 6574 632e 0a0a 4120  ctions, etc...A 
-00015f20: 7369 6d70 6c65 2075 7361 6765 2065 7861  simple usage exa
-00015f30: 6d70 6c65 206d 6967 6874 2062 653a 0a0a  mple might be:..
-00015f40: 6060 6073 6865 6c6c 0a79 642d 7375 626d  ```shell.yd-subm
-00015f50: 6974 202d 2d77 6f72 6b2d 7265 7175 6972  it --work-requir
-00015f60: 656d 656e 7420 6d79 5f77 6f72 6b5f 7265  ement my_work_re
-00015f70: 712e 6a73 6f6e 6e65 740a 6060 600a 0a54  q.jsonnet.```..T
-00015f80: 6865 2075 7365 206f 6620 7468 6520 6669  he use of the fi
-00015f90: 6c65 6e61 6d65 2065 7874 656e 7369 6f6e  lename extension
-00015fa0: 2060 2e6a 736f 6e6e 6574 6020 7769 6c6c   `.jsonnet` will
-00015fb0: 2069 6e76 6f6b 6520 4a73 6f6e 6e65 7420   invoke Jsonnet 
-00015fc0: 6576 616c 7561 7469 6f6e 2e20 284e 6f74  evaluation. (Not
-00015fd0: 6520 7468 6174 2061 2074 656d 706f 7261  e that a tempora
-00015fe0: 7279 204a 534f 4e20 6669 6c65 2069 7320  ry JSON file is 
-00015ff0: 6372 6561 7465 6420 6173 2070 6172 7420  created as part 
-00016000: 6f66 204a 736f 6e6e 6574 2070 726f 6365  of Jsonnet proce
-00016010: 7373 696e 672c 2077 6869 6368 2079 6f75  ssing, which you
-00016020: 206d 6179 2073 6565 2072 6566 6572 7265   may see referre
-00016030: 6420 746f 2069 6e20 6572 726f 7220 6d65  d to in error me
-00016040: 7373 6167 6573 3a20 7468 6973 2066 696c  ssages: this fil
-00016050: 6520 7769 6c6c 2068 6176 6520 6265 656e  e will have been
-00016060: 2064 656c 6574 6564 2062 6566 6f72 6520   deleted before 
-00016070: 7468 6520 7363 7269 7074 2073 746f 7073  the script stops
-00016080: 2e29 0a0a 2323 204a 736f 6e6e 6574 2049  .)..## Jsonnet I
-00016090: 6e73 7461 6c6c 6174 696f 6e0a 0a4a 736f  nstallation..Jso
-000160a0: 6e6e 6574 2069 7320 2a2a 6e6f 742a 2a20  nnet is **not** 
-000160b0: 696e 7374 616c 6c65 6420 6279 2064 6566  installed by def
-000160c0: 6175 6c74 2077 6865 6e20 6079 656c 6c6f  ault when `yello
-000160d0: 7764 6f67 2d70 7974 686f 6e2d 6578 616d  wdog-python-exam
-000160e0: 706c 6573 6020 6973 2069 6e73 7461 6c6c  ples` is install
-000160f0: 6564 2c20 6265 6361 7573 6520 7468 6520  ed, because the 
-00016100: 7061 636b 6167 6520 6861 7320 6269 6e61  package has bina
-00016110: 7279 2063 6f6d 706f 6e65 6e74 7320 7768  ry components wh
-00016120: 6963 6820 6172 6520 6e6f 7420 6176 6169  ich are not avai
-00016130: 6c61 626c 6520 6f6e 2050 7950 4920 666f  lable on PyPI fo
-00016140: 7220 616c 6c20 706c 6174 666f 726d 732e  r all platforms.
-00016150: 2049 6620 796f 7520 7472 7920 746f 2075   If you try to u
-00016160: 7365 2061 204a 736f 6e6e 6574 2066 696c  se a Jsonnet fil
-00016170: 6520 696e 2074 6865 2061 6273 656e 6365  e in the absence
-00016180: 206f 6620 4a73 6f6e 6e65 742c 2074 6865   of Jsonnet, the
-00016190: 2073 6372 6970 7473 2077 696c 6c20 7072   scripts will pr
-000161a0: 696e 7420 616e 2065 7272 6f72 206d 6573  int an error mes
-000161b0: 7361 6765 2c20 616e 6420 7375 6767 6573  sage, and sugges
-000161c0: 7420 616e 2069 6e73 7461 6c6c 6174 696f  t an installatio
-000161d0: 6e20 6d65 6368 616e 6973 6d2e 0a0a 546f  n mechanism...To
-000161e0: 2069 6e73 7461 6c6c 204a 736f 6e6e 6574   install Jsonnet
-000161f0: 2061 7420 7468 6520 7361 6d65 2074 696d   at the same tim
-00016200: 6520 6173 2069 6e73 7461 6c6c 696e 6720  e as installing 
-00016210: 6f72 2075 7064 6174 696e 6720 7468 6520  or updating the 
-00016220: 5079 7468 6f6e 2045 7861 6d70 6c65 7320  Python Examples 
-00016230: 7363 7269 7074 732c 206d 6f64 6966 7920  scripts, modify 
-00016240: 7468 6520 696e 7374 616c 6c61 7469 6f6e  the installation
-00016250: 2061 7320 666f 6c6c 6f77 7320 746f 2069   as follows to i
-00016260: 6e63 6c75 6465 2074 6865 2060 6a73 6f6e  nclude the `json
-00016270: 6e65 7460 206f 7074 696f 6e3a 0a0a 6060  net` option:..``
-00016280: 600a 7069 7020 696e 7374 616c 6c20 2d55  `.pip install -U
-00016290: 2022 7965 6c6c 6f77 646f 672d 7079 7468   "yellowdog-pyth
-000162a0: 6f6e 2d65 7861 6d70 6c65 735b 6a73 6f6e  on-examples[json
-000162b0: 6e65 745d 220a 6060 600a 0a54 6f20 696e  net]".```..To in
-000162c0: 7374 616c 6c20 4a73 6f6e 6e65 7420 7365  stall Jsonnet se
-000162d0: 7061 7261 7465 6c79 2066 726f 6d20 6079  parately from `y
-000162e0: 656c 6c6f 7764 6f67 2d70 7974 686f 6e2d  ellowdog-python-
-000162f0: 6578 616d 706c 6573 602c 2074 7279 3a0a  examples`, try:.
-00016300: 0a60 6060 7368 656c 6c0a 7069 7020 696e  .```shell.pip in
-00016310: 7374 616c 6c20 2d55 206a 736f 6e6e 6574  stall -U jsonnet
-00016320: 0a60 6060 0a0a 4966 2074 6869 7320 6661  .```..If this fa
-00016330: 696c 732c 2074 7279 3a0a 0a60 6060 7368  ils, try:..```sh
-00016340: 656c 6c0a 7069 7020 696e 7374 616c 6c20  ell.pip install 
-00016350: 2d55 206a 736f 6e6e 6574 2d62 696e 6172  -U jsonnet-binar
-00016360: 790a 6060 600a 0a49 6620 626f 7468 206f  y.```..If both o
-00016370: 6620 7468 6573 6520 6d65 7468 6f64 7320  f these methods 
-00016380: 6661 696c 2c20 796f 7527 6c6c 206e 6565  fail, you'll nee
-00016390: 6420 746f 2065 6e73 7572 6520 7468 6174  d to ensure that
-000163a0: 2074 6865 2070 6c61 7466 6f72 6d20 6f6e   the platform on
-000163b0: 2077 6869 6368 2079 6f75 2772 6520 7275   which you're ru
-000163c0: 6e6e 696e 6720 6861 7320 7468 6520 7265  nning has the re
-000163d0: 7175 6972 6564 2062 7569 6c64 2074 6f6f  quired build too
-000163e0: 6c73 2061 7661 696c 6162 6c65 2c20 736f  ls available, so
-000163f0: 2074 6861 7420 7468 6520 4a73 6f6e 6e65   that the Jsonne
-00016400: 7420 6269 6e61 7279 2063 6f6d 706f 6e65  t binary compone
-00016410: 6e74 7320 6361 6e20 6265 2062 7569 6c74  nts can be built
-00016420: 206c 6f63 616c 6c79 2e20 5468 6520 7265   locally. The re
-00016430: 7175 6972 6564 2062 7569 6c64 2070 6163  quired build pac
-00016440: 6b61 6765 7320 7661 7279 2062 7920 706c  kages vary by pl
-00016450: 6174 666f 726d 2062 7574 2075 7375 616c  atform but usual
-00016460: 6c79 2069 6e63 6c75 6465 2067 656e 6572  ly include gener
-00016470: 616c 2064 6576 656c 6f70 6d65 6e74 2074  al development t
-00016480: 6f6f 6c73 2069 6e63 6c75 6469 6e67 2061  ools including a
-00016490: 2043 2b2b 2063 6f6d 7069 6c65 722c 2061   C++ compiler, a
-000164a0: 6e64 2050 7974 686f 6e20 6465 7665 6c6f  nd Python develo
-000164b0: 706d 656e 7420 746f 6f6c 7320 696e 636c  pment tools incl
-000164c0: 7564 696e 6720 7468 6520 5079 7468 6f6e  uding the Python
-000164d0: 2068 6561 6465 7273 2e0a 0a50 6c65 6173   headers...Pleas
-000164e0: 6520 6765 7420 696e 2074 6f75 6368 2077  e get in touch w
-000164f0: 6974 6820 5965 6c6c 6f77 446f 6720 6966  ith YellowDog if
-00016500: 2079 6f75 2067 6574 2073 7475 636b 2e0a   you get stuck..
-00016510: 0a23 2320 5661 7269 6162 6c65 2053 7562  .## Variable Sub
-00016520: 7374 6974 7574 696f 6e73 2069 6e20 4a73  stitutions in Js
-00016530: 6f6e 6e65 7420 4669 6c65 730a 0a54 6865  onnet Files..The
-00016540: 2073 6372 6970 7473 2070 726f 7669 6465   scripts provide
-00016550: 2066 756c 6c20 7375 7070 6f72 7420 666f   full support fo
-00016560: 7220 7661 7269 6162 6c65 2073 7562 7374  r variable subst
-00016570: 6974 7574 696f 6e73 2069 6e20 4a73 6f6e  itutions in Json
-00016580: 6e65 7420 6669 6c65 732c 2075 7369 6e67  net files, using
-00016590: 2074 6865 2073 616d 6520 7275 6c65 7320   the same rules 
-000165a0: 6173 2066 6f72 2074 6865 204a 534f 4e20  as for the JSON 
-000165b0: 7370 6563 6966 6963 6174 696f 6e73 2e20  specifications. 
-000165c0: 5265 6d65 6d62 6572 2074 6861 7420 666f  Remember that fo
-000165d0: 7220 2a2a 576f 726b 6572 2050 6f6f 6c2a  r **Worker Pool*
-000165e0: 2a20 7370 6563 6966 6963 6174 696f 6e73  * specifications
-000165f0: 2c20 7661 7269 6162 6c65 2073 7562 7374  , variable subst
-00016600: 6974 7574 696f 6e73 206d 7573 7420 6265  itutions must be
-00016610: 2070 7265 6669 7865 6420 6279 2060 5f5f   prefixed by `__
-00016620: 602c 2065 2e67 2e20 6022 5f5f 7b7b 7573  `, e.g. `"__{{us
-00016630: 6572 6e61 6d65 7d7d 7d22 602e 0a0a 5661  ername}}}"`...Va
-00016640: 7269 6162 6c65 2073 7562 7374 6974 7574  riable substitut
-00016650: 696f 6e20 6973 2070 6572 666f 726d 6564  ion is performed
-00016660: 2062 6566 6f72 6520 4a73 6f6e 6e65 7420   before Jsonnet 
-00016670: 6578 7061 6e73 696f 6e20 696e 746f 204a  expansion into J
-00016680: 534f 4e2c 2061 6e64 2061 6761 696e 2061  SON, and again a
-00016690: 6674 6572 2074 6865 2065 7870 616e 7369  fter the expansi
-000166a0: 6f6e 2e0a 0a23 2320 4368 6563 6b69 6e67  on...## Checking
-000166b0: 204a 736f 6e6e 6574 2050 726f 6365 7373   Jsonnet Process
-000166c0: 696e 670a 0a54 6865 7265 2061 7265 2074  ing..There are t
-000166d0: 6872 6565 2070 6f73 7369 6269 6c69 7469  hree possibiliti
-000166e0: 6573 2066 6f72 2076 6572 6966 7969 6e67  es for verifying
-000166f0: 2074 6861 7420 6120 4a73 6f6e 6e65 7420   that a Jsonnet 
-00016700: 7370 6563 6966 6963 6174 696f 6e20 6973  specification is
-00016710: 2064 6f69 6e67 2077 6861 7420 6973 2069   doing what is i
-00016720: 6e74 656e 6465 643a 0a0a 312e 2054 6f20  ntended:..1. To 
-00016730: 696e 7370 6563 7420 7468 6520 6261 7369  inspect the basi
-00016740: 6320 636f 6e76 6572 7369 6f6e 206f 6620  c conversion of 
-00016750: 4a73 6f6e 6e65 7420 696e 746f 204a 534f  Jsonnet into JSO
-00016760: 4e2c 2077 6974 686f 7574 2061 6e79 2061  N, without any a
-00016770: 6464 6974 696f 6e61 6c20 7072 6f63 6573  dditional proces
-00016780: 7369 6e67 2062 7920 7468 6520 5079 7468  sing by the Pyth
-00016790: 6f6e 2045 7861 6d70 6c65 7320 7363 7269  on Examples scri
-000167a0: 7074 732c 2074 6865 2060 7964 2d6a 736f  pts, the `yd-jso
-000167b0: 6e6e 6574 326a 736f 6e60 2063 6f6d 6d61  nnet2json` comma
-000167c0: 6e64 2063 616e 2062 6520 7573 6564 2e20  nd can be used. 
-000167d0: 5468 6973 2074 616b 6573 2061 2073 696e  This takes a sin
-000167e0: 676c 6520 636f 6d6d 616e 6420 6c69 6e65  gle command line
-000167f0: 2061 7267 756d 656e 7420 7768 6963 6820   argument which 
-00016800: 6973 2074 6865 206e 616d 6520 6f66 2074  is the name of t
-00016810: 6865 206a 736f 6e6e 6574 2066 696c 6520  he jsonnet file 
-00016820: 746f 2062 6520 7072 6f63 6573 7365 643a  to be processed:
-00016830: 0a0a 6060 6073 6865 6c6c 0a79 642d 6a73  ..```shell.yd-js
-00016840: 6f6e 6e65 7432 6a73 6f6e 206d 795f 6669  onnet2json my_fi
-00016850: 6c65 2e6a 736f 6e6e 6574 0a60 6060 0a0a  le.jsonnet.```..
-00016860: 0a32 2e20 5468 6520 606a 736f 6e6e 6574  .2. The `jsonnet
-00016870: 2d64 7279 2d72 756e 6020 2860 2d4a 6029  -dry-run` (`-J`)
-00016880: 206f 7074 696f 6e20 6f66 2074 6865 2060   option of the `
-00016890: 7964 2d73 7562 6d69 7460 2c20 6079 642d  yd-submit`, `yd-
-000168a0: 7072 6f76 6973 696f 6e60 2061 6e64 2060  provision` and `
-000168b0: 7964 2d69 6e73 7461 6e74 6961 7465 6020  yd-instantiate` 
-000168c0: 636f 6d6d 616e 6473 2077 696c 6c20 6765  commands will ge
-000168d0: 6e65 7261 7465 204a 534f 4e20 6f75 7470  nerate JSON outp
-000168e0: 7574 2072 6570 7265 7365 6e74 696e 6720  ut representing 
-000168f0: 7468 6520 4a73 6f6e 6e65 7420 746f 204a  the Jsonnet to J
-00016900: 534f 4e20 7072 6f63 6573 7369 6e67 206f  SON processing o
-00016910: 6e6c 792c 2069 6e63 6c75 6469 6e67 2061  nly, including a
-00016920: 7070 6c69 6361 626c 6520 7661 7269 6162  pplicable variab
-00016930: 6c65 2073 7562 7374 6974 7574 696f 6e73  le substitutions
-00016940: 2c20 6275 7420 6265 666f 7265 2066 756c  , but before ful
-00016950: 6c20 7072 6f70 6572 7479 2065 7870 616e  l property expan
-00016960: 7369 6f6e 2069 6e74 6f20 7468 6520 4a53  sion into the JS
-00016970: 4f4e 2074 6861 7420 7769 6c6c 2062 6520  ON that will be 
-00016980: 7375 626d 6974 7465 6420 746f 2074 6865  submitted to the
-00016990: 2050 6c61 7466 6f72 6d2e 0a0a 0a33 2e20   Platform....3. 
-000169a0: 5468 6520 6064 7279 2d72 756e 6020 2860  The `dry-run` (`
-000169b0: 2d44 6029 206f 7074 696f 6e20 7769 6c6c  -D`) option will
-000169c0: 2067 656e 6572 6174 6520 4a53 4f4e 206f   generate JSON o
-000169d0: 7574 7075 7420 7265 7072 6573 656e 7469  utput representi
-000169e0: 6e67 2074 6865 2066 756c 6c20 7072 6f63  ng the full proc
-000169f0: 6573 7369 6e67 206f 6620 7468 6520 4a73  essing of the Js
-00016a00: 6f6e 6e65 7420 6669 6c65 2069 6e74 6f20  onnet file into 
-00016a10: 7768 6174 2077 696c 6c20 6265 2073 7562  what will be sub
-00016a20: 6d69 7474 6564 2074 6f20 7468 6520 4150  mitted to the AP
-00016a30: 492e 2054 6869 7320 616c 6c6f 7773 2069  I. This allows i
-00016a40: 6e73 7065 6374 696f 6e20 746f 2063 6865  nspection to che
-00016a50: 636b 2074 6861 7420 7468 6520 6f75 7470  ck that the outp
-00016a60: 7574 206d 6174 6368 6573 2065 7870 6563  ut matches expec
-00016a70: 7461 7469 6f6e 732c 2070 7269 6f72 2074  tations, prior t
-00016a80: 6f20 7375 626d 6974 7469 6e67 2074 6f20  o submitting to 
-00016a90: 7468 6520 506c 6174 666f 726d 2e0a 0a23  the Platform...#
-00016aa0: 2320 4a73 6f6e 6e65 7420 4578 616d 706c  # Jsonnet Exampl
-00016ab0: 650a 0a48 6572 6527 7320 616e 2065 7861  e..Here's an exa
-00016ac0: 6d70 6c65 206f 6620 6120 4a73 6f6e 6e65  mple of a Jsonne
-00016ad0: 7420 6669 6c65 2074 6861 7420 6765 6e65  t file that gene
-00016ae0: 7261 7465 7320 6120 576f 726b 2052 6571  rates a Work Req
-00016af0: 7569 7265 6d65 6e74 2077 6974 6820 666f  uirement with fo
-00016b00: 7572 2054 6173 6b73 3a0a 0a60 6060 6a73  ur Tasks:..```js
-00016b10: 6f6e 6e65 740a 2320 4675 6e63 7469 6f6e  onnet.# Function
-00016b20: 2066 6f72 2073 796e 7468 6573 6973 696e   for synthesisin
-00016b30: 6720 5461 736b 730a 6c6f 6361 6c20 5461  g Tasks.local Ta
-00016b40: 736b 2861 7267 756d 656e 7473 3d5b 5d2c  sk(arguments=[],
-00016b50: 2065 6e76 6972 6f6e 6d65 6e74 3d7b 7d29   environment={})
-00016b60: 203d 207b 0a20 2020 2061 7267 756d 656e   = {.    argumen
-00016b70: 7473 3a20 6172 6775 6d65 6e74 732c 0a20  ts: arguments,. 
-00016b80: 2020 2065 6e76 6972 6f6e 6d65 6e74 3a20     environment: 
-00016b90: 656e 7669 726f 6e6d 656e 742c 0a20 2020  environment,.   
-00016ba0: 206e 616d 653a 2022 6d79 5f74 6173 6b5f   name: "my_task_
-00016bb0: 7b7b 7461 736b 5f6e 756d 6265 727d 7d22  {{task_number}}"
-00016bc0: 0a7d 3b0a 0a23 2057 6f72 6b20 5265 7175  .};..# Work Requ
-00016bd0: 6972 656d 656e 740a 7b0a 2020 226e 616d  irement.{.  "nam
-00016be0: 6522 3a20 2277 6f72 6b72 6571 5f7b 7b64  e": "workreq_{{d
-00016bf0: 6174 6574 696d 657d 7d22 2c0a 2020 2274  atetime}}",.  "t
-00016c00: 6173 6b47 726f 7570 7322 3a20 5b0a 2020  askGroups": [.  
-00016c10: 2020 7b0a 2020 2020 2020 2274 6173 6b73    {.      "tasks
-00016c20: 223a 205b 0a20 2020 2020 2020 2054 6173  ": [.        Tas
-00016c30: 6b28 5b22 3122 5d2c 207b 413a 2022 415f  k(["1"], {A: "A_
-00016c40: 3122 7d29 2c20 2023 2061 7267 756d 656e  1"}),  # argumen
-00016c50: 7473 2061 6e64 2065 6e76 6972 6f6e 6d65  ts and environme
-00016c60: 6e74 0a20 2020 2020 2020 2054 6173 6b28  nt.        Task(
-00016c70: 5b22 3222 2c20 2233 225d 2c20 7b7d 292c  ["2", "3"], {}),
-00016c80: 2020 2020 2023 2061 7267 756d 656e 7473       # arguments
-00016c90: 2061 6e64 2065 6d70 7479 2065 6e76 6972   and empty envir
-00016ca0: 6f6e 6d65 6e74 0a20 2020 2020 2020 2054  onment.        T
-00016cb0: 6173 6b28 5b22 3422 5d29 2c20 2020 2020  ask(["4"]),     
-00016cc0: 2020 2020 2020 2020 2023 2061 7267 756d           # argum
-00016cd0: 656e 7473 2061 6e64 2064 6566 6175 6c74  ents and default
-00016ce0: 2065 6e76 6972 6f6e 6d65 6e74 0a20 2020   environment.   
-00016cf0: 2020 2020 2054 6173 6b28 2920 2020 2020       Task()     
-00016d00: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00016d10: 2064 6566 6175 6c74 2061 7267 756d 656e   default argumen
-00016d20: 7473 2061 6e64 2065 6e76 6972 6f6e 6d65  ts and environme
-00016d30: 6e74 0a20 2020 2020 205d 0a20 2020 207d  nt.      ].    }
-00016d40: 0a20 205d 0a7d 0a60 6060 0a0a 5768 656e  .  ].}.```..When
-00016d50: 2074 6869 7320 6973 2069 6e73 7065 6374   this is inspect
-00016d60: 6564 2075 7369 6e67 2074 6865 2060 6a73  ed using the `js
-00016d70: 6f6e 6e65 742d 6472 792d 7275 6e60 206f  onnet-dry-run` o
-00016d80: 7074 696f 6e20 2860 7964 2d73 7562 6d69  ption (`yd-submi
-00016d90: 7420 2d4a 7120 2d72 206d 795f 776f 726b  t -Jq -r my_work
-00016da0: 5f72 6571 2e6a 736f 6e6e 6574 6029 2c20  _req.jsonnet`), 
-00016db0: 7468 6973 2069 7320 7468 6520 7072 6f63  this is the proc
-00016dc0: 6573 7365 6420 6f75 7470 7574 3a0a 0a60  essed output:..`
-00016dd0: 6060 6a73 6f6e 0a7b 0a20 2022 6e61 6d65  ``json.{.  "name
-00016de0: 223a 2022 776f 726b 7265 715f 3233 3031  ": "workreq_2301
-00016df0: 3134 2d31 3430 3634 3522 2c0a 2020 2274  14-140645",.  "t
-00016e00: 6173 6b47 726f 7570 7322 3a20 5b0a 2020  askGroups": [.  
-00016e10: 2020 7b0a 2020 2020 2020 2274 6173 6b73    {.      "tasks
-00016e20: 223a 205b 0a20 2020 2020 2020 207b 0a20  ": [.        {. 
-00016e30: 2020 2020 2020 2020 2022 6172 6775 6d65           "argume
-00016e40: 6e74 7322 3a20 5b22 3122 5d2c 0a20 2020  nts": ["1"],.   
-00016e50: 2020 2020 2020 2022 656e 7669 726f 6e6d         "environm
-00016e60: 656e 7422 3a20 7b22 4122 3a20 2241 5f31  ent": {"A": "A_1
-00016e70: 227d 2c0a 2020 2020 2020 2020 2020 226e  "},.          "n
-00016e80: 616d 6522 3a20 226d 795f 7461 736b 5f7b  ame": "my_task_{
-00016e90: 7b74 6173 6b5f 6e75 6d62 6572 7d7d 220a  {task_number}}".
-00016ea0: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00016eb0: 2020 207b 0a20 2020 2020 2020 2020 2022     {.          "
-00016ec0: 6172 6775 6d65 6e74 7322 3a20 5b22 3222  arguments": ["2"
-00016ed0: 2c20 2233 225d 2c0a 2020 2020 2020 2020  , "3"],.        
-00016ee0: 2020 2265 6e76 6972 6f6e 6d65 6e74 223a    "environment":
-00016ef0: 207b 7d2c 0a20 2020 2020 2020 2020 2022   {},.          "
-00016f00: 6e61 6d65 223a 2022 6d79 5f74 6173 6b5f  name": "my_task_
-00016f10: 7b7b 7461 736b 5f6e 756d 6265 727d 7d22  {{task_number}}"
-00016f20: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
-00016f30: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
-00016f40: 2261 7267 756d 656e 7473 223a 205b 2234  "arguments": ["4
-00016f50: 225d 2c0a 2020 2020 2020 2020 2020 2265  "],.          "e
-00016f60: 6e76 6972 6f6e 6d65 6e74 223a 207b 7d2c  nvironment": {},
-00016f70: 0a20 2020 2020 2020 2020 2022 6e61 6d65  .          "name
-00016f80: 223a 2022 6d79 5f74 6173 6b5f 7b7b 7461  ": "my_task_{{ta
-00016f90: 736b 5f6e 756d 6265 727d 7d22 0a20 2020  sk_number}}".   
-00016fa0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-00016fb0: 7b0a 2020 2020 2020 2020 2020 2261 7267  {.          "arg
-00016fc0: 756d 656e 7473 223a 205b 5d2c 0a20 2020  uments": [],.   
-00016fd0: 2020 2020 2020 2022 656e 7669 726f 6e6d         "environm
-00016fe0: 656e 7422 3a20 7b7d 2c0a 2020 2020 2020  ent": {},.      
-00016ff0: 2020 2020 226e 616d 6522 3a20 226d 795f      "name": "my_
-00017000: 7461 736b 5f7b 7b74 6173 6b5f 6e75 6d62  task_{{task_numb
-00017010: 6572 7d7d 220a 2020 2020 2020 2020 7d0a  er}}".        }.
-00017020: 2020 2020 2020 5d0a 2020 2020 7d0a 2020        ].    }.  
-00017030: 5d0a 7d0a 6060 600a 0a57 6865 6e20 7468  ].}.```..When th
-00017040: 6973 2069 7320 696e 7370 6563 7465 6420  is is inspected 
-00017050: 7573 696e 6720 7468 6520 6064 7279 2d72  using the `dry-r
-00017060: 756e 6020 6f70 7469 6f6e 2028 6079 642d  un` option (`yd-
-00017070: 7375 626d 6974 202d 4471 202d 7220 6d79  submit -Dq -r my
-00017080: 5f77 6f72 6b5f 7265 712e 6a73 6f6e 6e65  _work_req.jsonne
-00017090: 7460 292c 2074 6869 7320 6973 2074 6865  t`), this is the
-000170a0: 2070 726f 6365 7373 6564 206f 7574 7075   processed outpu
-000170b0: 743a 0a0a 6060 606a 736f 6e0a 7b0a 2020  t:..```json.{.  
-000170c0: 2266 756c 6669 6c4f 6e53 7562 6d69 7422  "fulfilOnSubmit"
-000170d0: 3a20 6661 6c73 652c 0a20 2022 6e61 6d65  : false,.  "name
-000170e0: 223a 2022 776f 726b 7265 715f 3233 3031  ": "workreq_2301
-000170f0: 3134 2d31 3430 3634 3522 2c0a 2020 226e  14-140645",.  "n
-00017100: 616d 6573 7061 6365 223a 2022 7079 6578  amespace": "pyex
-00017110: 616d 706c 6573 222c 0a20 2022 7072 696f  amples",.  "prio
-00017120: 7269 7479 223a 2030 2c0a 2020 2274 6167  rity": 0,.  "tag
-00017130: 223a 2022 7079 6578 2d62 6173 6822 2c0a  ": "pyex-bash",.
-00017140: 2020 2274 6173 6b47 726f 7570 7322 3a20    "taskGroups": 
-00017150: 5b0a 2020 2020 7b0a 2020 2020 2020 2266  [.    {.      "f
-00017160: 696e 6973 6849 6641 6c6c 5461 736b 7346  inishIfAllTasksF
-00017170: 696e 6973 6865 6422 3a20 7472 7565 2c0a  inished": true,.
-00017180: 2020 2020 2020 2266 696e 6973 6849 6641        "finishIfA
-00017190: 6e79 5461 736b 4661 696c 6564 223a 2066  nyTaskFailed": f
-000171a0: 616c 7365 2c0a 2020 2020 2020 226e 616d  alse,.      "nam
-000171b0: 6522 3a20 2274 6173 6b5f 6772 6f75 705f  e": "task_group_
-000171c0: 3122 2c0a 2020 2020 2020 2270 7269 6f72  1",.      "prior
-000171d0: 6974 7922 3a20 302c 0a20 2020 2020 2022  ity": 0,.      "
-000171e0: 7275 6e53 7065 6369 6669 6361 7469 6f6e  runSpecification
-000171f0: 223a 207b 0a20 2020 2020 2020 2022 6d61  ": {.        "ma
-00017200: 7869 6d75 6d54 6173 6b52 6574 7269 6573  ximumTaskRetries
-00017210: 223a 2030 2c0a 2020 2020 2020 2020 2274  ": 0,.        "t
-00017220: 6173 6b54 7970 6573 223a 205b 2262 6173  askTypes": ["bas
-00017230: 6822 5d2c 0a20 2020 2020 2020 2022 776f  h"],.        "wo
-00017240: 726b 6572 5461 6773 223a 205b 2270 7965  rkerTags": ["pye
-00017250: 782d 6261 7368 2d64 6f63 6b65 7222 5d0a  x-bash-docker"].
-00017260: 2020 2020 2020 7d2c 0a20 2020 2020 2022        },.      "
-00017270: 7461 736b 7322 3a20 5b0a 2020 2020 2020  tasks": [.      
-00017280: 2020 7b0a 2020 2020 2020 2020 2020 2261    {.          "a
-00017290: 7267 756d 656e 7473 223a 205b 2277 6f72  rguments": ["wor
-000172a0: 6b72 6571 5f32 3330 3131 342d 3134 3036  kreq_230114-1406
-000172b0: 3435 2f73 6c65 6570 5f73 6372 6970 742e  45/sleep_script.
-000172c0: 7368 222c 2022 3122 5d2c 0a20 2020 2020  sh", "1"],.     
-000172d0: 2020 2020 2022 656e 7669 726f 6e6d 656e       "environmen
-000172e0: 7422 3a20 7b22 4122 3a20 2241 5f31 227d  t": {"A": "A_1"}
-000172f0: 2c0a 2020 2020 2020 2020 2020 2269 6e70  ,.          "inp
-00017300: 7574 7322 3a20 5b0a 2020 2020 2020 2020  uts": [.        
-00017310: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
-00017320: 2020 2020 226f 626a 6563 744e 616d 6550      "objectNameP
-00017330: 6174 7465 726e 223a 2022 776f 726b 7265  attern": "workre
-00017340: 715f 3233 3031 3134 2d31 3430 3634 352f  q_230114-140645/
-00017350: 736c 6565 705f 7363 7269 7074 2e73 6822  sleep_script.sh"
-00017360: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00017370: 2273 6f75 7263 6522 3a20 2254 4153 4b5f  "source": "TASK_
-00017380: 4e41 4d45 5350 4143 4522 2c0a 2020 2020  NAMESPACE",.    
-00017390: 2020 2020 2020 2020 2020 2276 6572 6966            "verif
-000173a0: 6963 6174 696f 6e22 3a20 2256 4552 4946  ication": "VERIF
-000173b0: 595f 4154 5f53 5441 5254 220a 2020 2020  Y_AT_START".    
-000173c0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-000173d0: 2020 2020 5d2c 0a20 2020 2020 2020 2020      ],.         
-000173e0: 2022 6e61 6d65 223a 2022 6d79 5f74 6173   "name": "my_tas
-000173f0: 6b5f 3122 2c0a 2020 2020 2020 2020 2020  k_1",.          
-00017400: 226f 7574 7075 7473 223a 205b 0a20 2020  "outputs": [.   
-00017410: 2020 2020 2020 2020 207b 2261 6c77 6179           {"alway
-00017420: 7355 706c 6f61 6422 3a20 7472 7565 2c20  sUpload": true, 
-00017430: 2272 6571 7569 7265 6422 3a20 6661 6c73  "required": fals
-00017440: 652c 2022 736f 7572 6365 223a 2022 5052  e, "source": "PR
-00017450: 4f43 4553 535f 4f55 5450 5554 227d 0a20  OCESS_OUTPUT"}. 
-00017460: 2020 2020 2020 2020 205d 2c0a 2020 2020           ],.    
-00017470: 2020 2020 2020 2274 6173 6b54 7970 6522        "taskType"
-00017480: 3a20 2262 6173 6822 0a20 2020 2020 2020  : "bash".       
-00017490: 207d 2c0a 2020 2020 2020 2020 7b0a 2020   },.        {.  
-000174a0: 2020 2020 2020 2020 2261 7267 756d 656e          "argumen
-000174b0: 7473 223a 205b 2277 6f72 6b72 6571 5f32  ts": ["workreq_2
-000174c0: 3330 3131 342d 3134 3036 3435 2f73 6c65  30114-140645/sle
-000174d0: 6570 5f73 6372 6970 742e 7368 222c 2022  ep_script.sh", "
-000174e0: 3222 2c20 2233 225d 2c0a 2020 2020 2020  2", "3"],.      
-000174f0: 2020 2020 2265 6e76 6972 6f6e 6d65 6e74      "environment
-00017500: 223a 207b 7d2c 0a20 2020 2020 2020 2020  ": {},.         
-00017510: 2022 696e 7075 7473 223a 205b 0a20 2020   "inputs": [.   
-00017520: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
-00017530: 2020 2020 2020 2020 2022 6f62 6a65 6374           "object
-00017540: 4e61 6d65 5061 7474 6572 6e22 3a20 2277  NamePattern": "w
-00017550: 6f72 6b72 6571 5f32 3330 3131 342d 3134  orkreq_230114-14
-00017560: 3036 3435 2f73 6c65 6570 5f73 6372 6970  0645/sleep_scrip
-00017570: 742e 7368 222c 0a20 2020 2020 2020 2020  t.sh",.         
-00017580: 2020 2020 2022 736f 7572 6365 223a 2022       "source": "
-00017590: 5441 534b 5f4e 414d 4553 5041 4345 222c  TASK_NAMESPACE",
-000175a0: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-000175b0: 7665 7269 6669 6361 7469 6f6e 223a 2022  verification": "
-000175c0: 5645 5249 4659 5f41 545f 5354 4152 5422  VERIFY_AT_START"
-000175d0: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
-000175e0: 2020 2020 2020 2020 205d 2c0a 2020 2020           ],.    
-000175f0: 2020 2020 2020 226e 616d 6522 3a20 226d        "name": "m
-00017600: 795f 7461 736b 5f32 222c 0a20 2020 2020  y_task_2",.     
-00017610: 2020 2020 2022 6f75 7470 7574 7322 3a20       "outputs": 
-00017620: 5b0a 2020 2020 2020 2020 2020 2020 7b22  [.            {"
-00017630: 616c 7761 7973 5570 6c6f 6164 223a 2074  alwaysUpload": t
-00017640: 7275 652c 2022 7265 7175 6972 6564 223a  rue, "required":
-00017650: 2066 616c 7365 2c20 2273 6f75 7263 6522   false, "source"
-00017660: 3a20 2250 524f 4345 5353 5f4f 5554 5055  : "PROCESS_OUTPU
-00017670: 5422 7d0a 2020 2020 2020 2020 2020 5d2c  T"}.          ],
-00017680: 0a20 2020 2020 2020 2020 2022 7461 736b  .          "task
-00017690: 5479 7065 223a 2022 6261 7368 220a 2020  Type": "bash".  
-000176a0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-000176b0: 207b 0a20 2020 2020 2020 2020 2022 6172   {.          "ar
-000176c0: 6775 6d65 6e74 7322 3a20 5b22 776f 726b  guments": ["work
-000176d0: 7265 715f 3233 3031 3134 2d31 3430 3634  req_230114-14064
-000176e0: 352f 736c 6565 705f 7363 7269 7074 2e73  5/sleep_script.s
-000176f0: 6822 2c20 2234 225d 2c0a 2020 2020 2020  h", "4"],.      
-00017700: 2020 2020 2265 6e76 6972 6f6e 6d65 6e74      "environment
-00017710: 223a 207b 7d2c 0a20 2020 2020 2020 2020  ": {},.         
-00017720: 2022 696e 7075 7473 223a 205b 0a20 2020   "inputs": [.   
-00017730: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
-00017740: 2020 2020 2020 2020 2022 6f62 6a65 6374           "object
-00017750: 4e61 6d65 5061 7474 6572 6e22 3a20 2277  NamePattern": "w
-00017760: 6f72 6b72 6571 5f32 3330 3131 342d 3134  orkreq_230114-14
-00017770: 3036 3435 2f73 6c65 6570 5f73 6372 6970  0645/sleep_scrip
-00017780: 742e 7368 222c 0a20 2020 2020 2020 2020  t.sh",.         
-00017790: 2020 2020 2022 736f 7572 6365 223a 2022       "source": "
-000177a0: 5441 534b 5f4e 414d 4553 5041 4345 222c  TASK_NAMESPACE",
-000177b0: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-000177c0: 7665 7269 6669 6361 7469 6f6e 223a 2022  verification": "
-000177d0: 5645 5249 4659 5f41 545f 5354 4152 5422  VERIFY_AT_START"
-000177e0: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
-000177f0: 2020 2020 2020 2020 205d 2c0a 2020 2020           ],.    
-00017800: 2020 2020 2020 226e 616d 6522 3a20 226d        "name": "m
-00017810: 795f 7461 736b 5f33 222c 0a20 2020 2020  y_task_3",.     
-00017820: 2020 2020 2022 6f75 7470 7574 7322 3a20       "outputs": 
-00017830: 5b0a 2020 2020 2020 2020 2020 2020 7b22  [.            {"
-00017840: 616c 7761 7973 5570 6c6f 6164 223a 2074  alwaysUpload": t
-00017850: 7275 652c 2022 7265 7175 6972 6564 223a  rue, "required":
-00017860: 2066 616c 7365 2c20 2273 6f75 7263 6522   false, "source"
-00017870: 3a20 2250 524f 4345 5353 5f4f 5554 5055  : "PROCESS_OUTPU
-00017880: 5422 7d0a 2020 2020 2020 2020 2020 5d2c  T"}.          ],
-00017890: 0a20 2020 2020 2020 2020 2022 7461 736b  .          "task
-000178a0: 5479 7065 223a 2022 6261 7368 220a 2020  Type": "bash".  
-000178b0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-000178c0: 207b 0a20 2020 2020 2020 2020 2022 6172   {.          "ar
-000178d0: 6775 6d65 6e74 7322 3a20 5b22 776f 726b  guments": ["work
-000178e0: 7265 715f 3233 3031 3134 2d31 3430 3634  req_230114-14064
-000178f0: 352f 736c 6565 705f 7363 7269 7074 2e73  5/sleep_script.s
-00017900: 6822 5d2c 0a20 2020 2020 2020 2020 2022  h"],.          "
-00017910: 656e 7669 726f 6e6d 656e 7422 3a20 7b7d  environment": {}
-00017920: 2c0a 2020 2020 2020 2020 2020 2269 6e70  ,.          "inp
-00017930: 7574 7322 3a20 5b0a 2020 2020 2020 2020  uts": [.        
-00017940: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
-00017950: 2020 2020 226f 626a 6563 744e 616d 6550      "objectNameP
-00017960: 6174 7465 726e 223a 2022 776f 726b 7265  attern": "workre
-00017970: 715f 3233 3031 3134 2d31 3430 3634 352f  q_230114-140645/
-00017980: 736c 6565 705f 7363 7269 7074 2e73 6822  sleep_script.sh"
-00017990: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000179a0: 2273 6f75 7263 6522 3a20 2254 4153 4b5f  "source": "TASK_
-000179b0: 4e41 4d45 5350 4143 4522 2c0a 2020 2020  NAMESPACE",.    
-000179c0: 2020 2020 2020 2020 2020 2276 6572 6966            "verif
-000179d0: 6963 6174 696f 6e22 3a20 2256 4552 4946  ication": "VERIF
-000179e0: 595f 4154 5f53 5441 5254 220a 2020 2020  Y_AT_START".    
-000179f0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00017a00: 2020 2020 5d2c 0a20 2020 2020 2020 2020      ],.         
-00017a10: 2022 6e61 6d65 223a 2022 6d79 5f74 6173   "name": "my_tas
-00017a20: 6b5f 3422 2c0a 2020 2020 2020 2020 2020  k_4",.          
-00017a30: 226f 7574 7075 7473 223a 205b 0a20 2020  "outputs": [.   
-00017a40: 2020 2020 2020 2020 207b 2261 6c77 6179           {"alway
-00017a50: 7355 706c 6f61 6422 3a20 7472 7565 2c20  sUpload": true, 
-00017a60: 2272 6571 7569 7265 6422 3a20 6661 6c73  "required": fals
-00017a70: 652c 2022 736f 7572 6365 223a 2022 5052  e, "source": "PR
-00017a80: 4f43 4553 535f 4f55 5450 5554 227d 0a20  OCESS_OUTPUT"}. 
-00017a90: 2020 2020 2020 2020 205d 2c0a 2020 2020           ],.    
-00017aa0: 2020 2020 2020 2274 6173 6b54 7970 6522        "taskType"
-00017ab0: 3a20 2262 6173 6822 0a20 2020 2020 2020  : "bash".       
-00017ac0: 207d 0a20 2020 2020 205d 0a20 2020 207d   }.      ].    }
-00017ad0: 0a20 205d 0a7d 0a60 6060 0a0a 2320 436f  .  ].}.```..# Co
-00017ae0: 6d6d 616e 6420 4c69 7374 0a0a 4865 6c70  mmand List..Help
-00017af0: 2069 7320 6176 6169 6c61 626c 6520 666f   is available fo
-00017b00: 7220 616c 6c20 636f 6d6d 616e 6473 2062  r all commands b
-00017b10: 7920 696e 766f 6b69 6e67 2061 2063 6f6d  y invoking a com
-00017b20: 6d61 6e64 2077 6974 6820 7468 6520 602d  mand with the `-
-00017b30: 2d68 656c 7060 206f 7220 602d 6860 206f  -help` or `-h` o
-00017b40: 7074 696f 6e2e 2053 6f6d 6520 636f 6d6d  ption. Some comm
-00017b50: 616e 6420 6c69 6e65 2070 6172 616d 6574  and line paramet
-00017b60: 6572 7320 6172 6520 636f 6d6d 6f6e 2074  ers are common t
-00017b70: 6f20 616c 6c20 636f 6d6d 616e 6473 2c20  o all commands, 
-00017b80: 7768 696c 6520 6f74 6865 7273 2061 7265  while others are
-00017b90: 2063 6f6d 6d61 6e64 2d73 7065 6369 6669   command-specifi
-00017ba0: 632e 0a0a 416c 6c20 6465 7374 7275 6374  c...All destruct
-00017bb0: 6976 6520 636f 6d6d 616e 6473 2072 6571  ive commands req
-00017bc0: 7569 7265 2075 7365 7220 636f 6e66 6972  uire user confir
-00017bd0: 6d61 7469 6f6e 2062 6566 6f72 6520 7461  mation before ta
-00017be0: 6b69 6e67 2065 6666 6563 742e 2054 6869  king effect. Thi
-00017bf0: 7320 6361 6e20 6265 2073 7570 7072 6573  s can be suppres
-00017c00: 7365 6420 7573 696e 6720 7468 6520 602d  sed using the `-
-00017c10: 2d79 6573 6020 6f72 2060 2d79 6020 6f70  -yes` or `-y` op
-00017c20: 7469 6f6e 2c20 696e 2077 6869 6368 2063  tion, in which c
-00017c30: 6173 6520 7468 6520 636f 6d6d 616e 6420  ase the command 
-00017c40: 7769 6c6c 2070 726f 6365 6564 2077 6974  will proceed wit
-00017c50: 686f 7574 2063 6f6e 6669 726d 6174 696f  hout confirmatio
-00017c60: 6e2e 0a0a 536f 6d65 2063 6f6d 6d61 6e64  n...Some command
-00017c70: 7320 7375 7070 6f72 7420 7468 6520 602d  s support the `-
-00017c80: 2d69 6e74 6572 6163 7469 7665 6020 6f72  -interactive` or
-00017c90: 2060 2d69 6020 6f70 7469 6f6e 2c20 616c   `-i` option, al
-00017ca0: 6c6f 7769 6e67 2075 7365 7220 7365 6c65  lowing user sele
-00017cb0: 6374 696f 6e73 2074 6f20 6265 206d 6164  ctions to be mad
-00017cc0: 652e 2045 2e67 2e2c 2074 6869 7320 6361  e. E.g., this ca
-00017cd0: 6e20 6265 2075 7365 6420 746f 2073 656c  n be used to sel
-00017ce0: 6563 7420 7768 6963 6820 6f62 6a65 6374  ect which object
-00017cf0: 2070 6174 6873 2074 6f20 6465 6c65 7465   paths to delete
-00017d00: 2e0a 0a54 6865 2060 2d2d 7175 6965 7460  ...The `--quiet`
-00017d10: 206f 7220 602d 7160 206f 7074 696f 6e20   or `-q` option 
-00017d20: 7265 6475 6365 7320 7468 6520 636f 6d6d  reduces the comm
-00017d30: 616e 6420 6f75 7470 7574 2064 6f77 6e20  and output down 
-00017d40: 746f 2065 7373 656e 7469 616c 206d 6573  to essential mes
-00017d50: 7361 6765 7320 6f6e 6c79 2e20 536f 2c20  sages only. So, 
-00017d60: 666f 7220 6578 616d 706c 652c 2060 7964  for example, `yd
-00017d70: 2d64 656c 6574 6520 2d79 7160 2077 6f75  -delete -yq` wou
-00017d80: 6c64 2064 656c 6574 6520 616c 6c20 6d61  ld delete all ma
-00017d90: 7463 6869 6e67 206f 626a 6563 7420 7061  tching object pa
-00017da0: 7468 7320 7369 6c65 6e74 6c79 2e0a 0a49  ths silently...I
-00017db0: 6620 796f 7520 656e 636f 756e 7465 7220  f you encounter 
-00017dc0: 616e 2065 7272 6f72 2069 7420 6361 6e20  an error it can 
-00017dd0: 6265 2075 7365 6675 6c20 666f 7220 7375  be useful for su
-00017de0: 7070 6f72 7420 7075 7270 6f73 6573 2074  pport purposes t
-00017df0: 6f20 7365 6520 7468 6520 6675 6c6c 2050  o see the full P
-00017e00: 7974 686f 6e20 7374 6163 6b20 7472 6163  ython stack trac
-00017e10: 652e 2054 6869 7320 6361 6e20 6265 2065  e. This can be e
-00017e20: 6e61 626c 6564 2062 7920 7275 6e6e 696e  nabled by runnin
-00017e30: 6720 7468 6520 636f 6d6d 616e 6420 7573  g the command us
-00017e40: 696e 6720 7468 6520 602d 2d64 6562 7567  ing the `--debug
-00017e50: 6020 6f70 7469 6f6e 2e0a 0a23 2320 7964  ` option...## yd
-00017e60: 2d73 7562 6d69 740a 0a54 6865 2060 7964  -submit..The `yd
-00017e70: 2d73 7562 6d69 7460 2063 6f6d 6d61 6e64  -submit` command
-00017e80: 2073 7562 6d69 7473 2061 206e 6577 2057   submits a new W
-00017e90: 6f72 6b20 5265 7175 6972 656d 656e 742c  ork Requirement,
-00017ea0: 2061 6363 6f72 6469 6e67 2074 6f20 7468   according to th
-00017eb0: 6520 576f 726b 2052 6571 7569 7265 6d65  e Work Requireme
-00017ec0: 6e74 2064 6566 696e 6974 696f 6e20 666f  nt definition fo
-00017ed0: 756e 6420 696e 2074 6865 2060 776f 726b  und in the `work
-00017ee0: 5265 7175 6972 656d 656e 7460 2073 6563  Requirement` sec
-00017ef0: 7469 6f6e 206f 6620 7468 6520 544f 4d4c  tion of the TOML
-00017f00: 2063 6f6e 6669 6775 7261 7469 6f6e 2066   configuration f
-00017f10: 696c 6520 616e 642f 6f72 2074 6865 2073  ile and/or the s
-00017f20: 7065 6369 6669 6361 7469 6f6e 2066 6f75  pecification fou
-00017f30: 6e64 2069 6e20 6120 576f 726b 2052 6571  nd in a Work Req
-00017f40: 7569 7265 6d65 6e74 204a 534f 4e20 646f  uirement JSON do
-00017f50: 6375 6d65 6e74 2073 7570 706c 6965 6420  cument supplied 
-00017f60: 7573 696e 6720 7468 6520 602d 2d77 6f72  using the `--wor
-00017f70: 6b2d 7265 7175 6972 656d 656e 7460 206f  k-requirement` o
-00017f80: 7074 696f 6e2e 0a0a 5573 6520 7468 6520  ption...Use the 
-00017f90: 602d 2d64 7279 2d72 756e 6020 6f70 7469  `--dry-run` opti
-00017fa0: 6f6e 2074 6f20 696e 7370 6563 7420 7468  on to inspect th
-00017fb0: 6520 6465 7461 696c 7320 6f66 2074 6865  e details of the
-00017fc0: 2057 6f72 6b20 5265 7175 6972 656d 656e   Work Requiremen
-00017fd0: 742c 2054 6173 6b20 4772 6f75 7073 2c20  t, Task Groups, 
-00017fe0: 616e 6420 5461 736b 7320 7468 6174 2077  and Tasks that w
-00017ff0: 696c 6c20 6265 2073 7562 6d69 7474 6564  ill be submitted
-00018000: 2c20 696e 204a 534f 4e20 666f 726d 6174  , in JSON format
-00018010: 2e0a 0a4f 6e63 6520 7375 626d 6974 7465  ...Once submitte
-00018020: 642c 2074 6865 2057 6f72 6b20 5265 7175  d, the Work Requ
-00018030: 6972 656d 656e 7420 7769 6c6c 2061 7070  irement will app
-00018040: 6561 7220 696e 2074 6865 202a 2a57 6f72  ear in the **Wor
-00018050: 6b2a 2a20 7461 6220 696e 2074 6865 2059  k** tab in the Y
-00018060: 656c 6c6f 7744 6f67 2050 6f72 7461 6c2e  ellowDog Portal.
-00018070: 0a0a 5468 6520 576f 726b 2052 6571 7569  ..The Work Requi
-00018080: 7265 6d65 6e74 2773 2070 726f 6772 6573  rement's progres
-00018090: 7320 6361 6e20 6265 2074 7261 636b 6564  s can be tracked
-000180a0: 2074 6f20 636f 6d70 6c65 7469 6f6e 2062   to completion b
-000180b0: 7920 7573 696e 6720 7468 6520 602d 2d66  y using the `--f
-000180c0: 6f6c 6c6f 7760 2028 6f72 2060 2d66 6029  ollow` (or `-f`)
-000180d0: 206f 7074 696f 6e20 7768 656e 2069 6e76   option when inv
-000180e0: 6f6b 696e 6720 6079 642d 7375 626d 6974  oking `yd-submit
-000180f0: 603a 2074 6865 2063 6f6d 6d61 6e64 2077  `: the command w
-00018100: 696c 6c20 7265 706f 7274 206f 6e20 5461  ill report on Ta
-00018110: 736b 7320 6173 2074 6865 7920 636f 6e63  sks as they conc
-00018120: 6c75 6465 2061 6e64 2077 6f6e 2774 2072  lude and won't r
-00018130: 6574 7572 6e20 756e 7469 6c20 7468 6520  eturn until the 
-00018140: 576f 726b 2052 6571 7569 7265 6d65 6e74  Work Requirement
-00018150: 2068 6173 2066 696e 6973 6865 642e 0a0a   has finished...
-00018160: 2323 2079 642d 7072 6f76 6973 696f 6e0a  ## yd-provision.
-00018170: 0a54 6865 2060 7964 2d70 726f 7669 7369  .The `yd-provisi
-00018180: 6f6e 6020 636f 6d6d 616e 6420 7072 6f76  on` command prov
-00018190: 6973 696f 6e73 2061 206e 6577 2057 6f72  isions a new Wor
-000181a0: 6b65 7220 506f 6f6c 2061 6363 6f72 6469  ker Pool accordi
-000181b0: 6e67 2074 6f20 7468 6520 7370 6563 6966  ng to the specif
-000181c0: 6963 6174 696f 6e73 2069 6e20 7468 6520  ications in the 
-000181d0: 6077 6f72 6b65 7250 6f6f 6c60 2073 6563  `workerPool` sec
-000181e0: 7469 6f6e 206f 6620 7468 6520 544f 4d4c  tion of the TOML
-000181f0: 2063 6f6e 6669 6775 7261 7469 6f6e 2066   configuration f
-00018200: 696c 6520 616e 642f 6f72 2069 6e20 7468  ile and/or in th
-00018210: 6520 7370 6563 6966 6963 6174 696f 6e20  e specification 
-00018220: 666f 756e 6420 696e 2061 2057 6f72 6b65  found in a Worke
-00018230: 7220 506f 6f6c 204a 534f 4e20 646f 6375  r Pool JSON docu
-00018240: 6d65 6e74 2073 7570 706c 6965 6420 7573  ment supplied us
-00018250: 696e 6720 7468 6520 602d 2d77 6f72 6b65  ing the `--worke
-00018260: 722d 706f 6f6c 6020 6f70 7469 6f6e 2e0a  r-pool` option..
-00018270: 0a55 7365 2074 6865 2060 2d2d 6472 792d  .Use the `--dry-
-00018280: 7275 6e60 206f 7074 696f 6e20 746f 2069  run` option to i
-00018290: 6e73 7065 6374 2074 6865 2064 6574 6169  nspect the detai
-000182a0: 6c73 206f 6620 7468 6520 576f 726b 6572  ls of the Worker
-000182b0: 2050 6f6f 6c20 7370 6563 6966 6963 6174   Pool specificat
-000182c0: 696f 6e20 7468 6174 2077 696c 6c20 6265  ion that will be
-000182d0: 2073 7562 6d69 7474 6564 2c20 696e 204a   submitted, in J
-000182e0: 534f 4e20 666f 726d 6174 2e0a 0a4f 6e63  SON format...Onc
-000182f0: 6520 7072 6f76 6973 696f 6e65 642c 2074  e provisioned, t
-00018300: 6865 2057 6f72 6b65 7220 506f 6f6c 2077  he Worker Pool w
-00018310: 696c 6c20 6170 7065 6172 2069 6e20 7468  ill appear in th
-00018320: 6520 2a2a 576f 726b 6572 732a 2a20 7461  e **Workers** ta
-00018330: 6220 696e 2074 6865 2059 656c 6c6f 7744  b in the YellowD
-00018340: 6f67 2050 6f72 7461 6c2c 2061 6e64 2069  og Portal, and i
-00018350: 7473 2061 7373 6f63 6961 7465 6420 436f  ts associated Co
-00018360: 6d70 7574 6520 5265 7175 6972 656d 656e  mpute Requiremen
-00018370: 7420 7769 6c6c 2061 7070 6561 7220 696e  t will appear in
-00018380: 2074 6865 202a 2a43 6f6d 7075 7465 2a2a   the **Compute**
-00018390: 2074 6162 2e0a 0a23 2320 7964 2d63 616e   tab...## yd-can
-000183a0: 6365 6c0a 0a54 6865 2060 7964 2d63 616e  cel..The `yd-can
-000183b0: 6365 6c60 2063 6f6d 6d61 6e64 2063 616e  cel` command can
-000183c0: 6365 6c73 2061 6e79 2061 6374 6976 6520  cels any active 
-000183d0: 576f 726b 2052 6571 7569 7265 6d65 6e74  Work Requirement
-000183e0: 732c 2069 6e63 6c75 6469 6e67 2061 6e79  s, including any
-000183f0: 2070 656e 6469 6e67 2054 6173 6b20 4772   pending Task Gr
-00018400: 6f75 7073 2061 6e64 2074 6865 2054 6173  oups and the Tas
-00018410: 6b73 2074 6865 7920 636f 6e74 6169 6e2e  ks they contain.
-00018420: 200a 0a54 6865 2060 6e61 6d65 7370 6163   ..The `namespac
-00018430: 6560 2061 6e64 2060 7461 6760 2076 616c  e` and `tag` val
-00018440: 7565 7320 696e 2074 6865 2060 636f 6e66  ues in the `conf
-00018450: 6967 2e74 6f6d 6c60 2066 696c 6520 6172  ig.toml` file ar
-00018460: 6520 7573 6564 2074 6f20 6964 656e 7469  e used to identi
-00018470: 6679 2077 6869 6368 2057 6f72 6b20 5265  fy which Work Re
-00018480: 7175 6972 656d 656e 7473 2074 6f20 6361  quirements to ca
-00018490: 6e63 656c 2e0a 0a42 7920 6465 6661 756c  ncel...By defaul
-000184a0: 742c 2061 6e79 2054 6173 6b73 2074 6861  t, any Tasks tha
-000184b0: 7420 6172 6520 6375 7272 656e 746c 7920  t are currently 
-000184c0: 7275 6e6e 696e 6720 6f6e 2057 6f72 6b65  running on Worke
-000184d0: 7273 2077 696c 6c20 636f 6e74 696e 7565  rs will continue
-000184e0: 2074 6f20 7275 6e20 746f 2063 6f6d 706c   to run to compl
-000184f0: 6574 696f 6e20 6f72 2075 6e74 696c 2074  etion or until t
-00018500: 6865 7920 6661 696c 2e20 5461 736b 7320  hey fail. Tasks 
-00018510: 6361 6e20 6265 2069 6e73 7472 7563 7465  can be instructe
-00018520: 6420 746f 2061 626f 7274 2069 6d6d 6564  d to abort immed
-00018530: 6961 7465 6c79 2062 7920 7375 7070 6c79  iately by supply
-00018540: 696e 6720 7468 6520 602d 2d61 626f 7274  ing the `--abort
-00018550: 6020 6f72 2060 2d61 6020 6f70 7469 6f6e  ` or `-a` option
-00018560: 2074 6f20 6079 642d 6361 6e63 656c 602e   to `yd-cancel`.
-00018570: 0a0a 2323 2079 642d 6162 6f72 740a 0a54  ..## yd-abort..T
-00018580: 6865 2060 7964 2d61 626f 7274 6020 636f  he `yd-abort` co
-00018590: 6d6d 616e 6420 6973 2075 7365 6420 746f  mmand is used to
-000185a0: 2061 626f 7274 2054 6173 6b73 2074 6861   abort Tasks tha
-000185b0: 7420 6172 6520 6375 7272 656e 746c 7920  t are currently 
-000185c0: 7275 6e6e 696e 672e 2054 6865 2075 7365  running. The use
-000185d0: 7220 696e 7465 7261 6374 6976 656c 7920  r interactively 
-000185e0: 7365 6c65 6374 7320 7468 6520 576f 726b  selects the Work
-000185f0: 2052 6571 7569 7265 6d65 6e74 7320 746f   Requirements to
-00018600: 2074 6172 6765 742c 2061 6e64 2074 6865   target, and the
-00018610: 6e20 7768 6963 6820 5461 736b 7320 7769  n which Tasks wi
-00018620: 7468 696e 2074 686f 7365 2057 6f72 6b20  thin those Work 
-00018630: 5265 7175 6972 656d 656e 7473 2074 6f20  Requirements to 
-00018640: 6162 6f72 742e 2054 6865 2057 6f72 6b20  abort. The Work 
-00018650: 5265 7175 6972 656d 656e 7473 2061 7265  Requirements are
-00018660: 206e 6f74 2063 616e 6365 6c6c 6564 2061   not cancelled a
-00018670: 7320 7061 7274 206f 6620 7468 6973 2070  s part of this p
-00018680: 726f 6365 7373 2e0a 0a54 6865 2060 6e61  rocess...The `na
-00018690: 6d65 7370 6163 6560 2061 6e64 2060 7461  mespace` and `ta
-000186a0: 6760 2076 616c 7565 7320 696e 2074 6865  g` values in the
-000186b0: 2060 636f 6e66 6967 2e74 6f6d 6c60 2066   `config.toml` f
-000186c0: 696c 6520 6172 6520 7573 6564 2074 6f20  ile are used to 
-000186d0: 6964 656e 7469 6679 2077 6869 6368 2057  identify which W
-000186e0: 6f72 6b20 5265 7175 6972 656d 656e 7473  ork Requirements
-000186f0: 2074 6f20 6c69 7374 2066 6f72 2073 656c   to list for sel
-00018700: 6563 7469 6f6e 2e0a 0a23 2320 7964 2d64  ection...## yd-d
-00018710: 6f77 6e6c 6f61 640a 0a54 6865 2060 7964  ownload..The `yd
-00018720: 2d64 6f77 6e6c 6f61 6460 2063 6f6d 6d61  -download` comma
-00018730: 6e64 2064 6f77 6e6c 6f61 6473 2061 6e79  nd downloads any
-00018740: 206f 626a 6563 7473 2063 7265 6174 6564   objects created
-00018750: 2069 6e20 7468 6520 5965 6c6c 6f77 446f   in the YellowDo
-00018760: 6720 4f62 6a65 6374 2053 746f 7265 2e0a  g Object Store..
-00018770: 0a54 6865 2060 6e61 6d65 7370 6163 6560  .The `namespace`
-00018780: 2061 6e64 2060 7461 6760 2076 616c 7565   and `tag` value
-00018790: 7320 6172 6520 7573 6564 2074 6f20 6465  s are used to de
-000187a0: 7465 726d 696e 6520 7768 6963 6820 6f62  termine which ob
-000187b0: 6a65 6374 7320 746f 2064 6f77 6e6c 6f61  jects to downloa
-000187c0: 642e 204f 626a 6563 7473 2077 696c 6c20  d. Objects will 
-000187d0: 6265 2064 6f77 6e6c 6f61 6465 6420 746f  be downloaded to
-000187e0: 2061 2064 6972 6563 746f 7279 2077 6974   a directory wit
-000187f0: 6820 7468 6520 7361 6d65 206e 616d 6520  h the same name 
-00018800: 6173 2060 6e61 6d65 7370 6163 6560 2e20  as `namespace`. 
-00018810: 4966 2061 2064 6972 6563 746f 7279 2061  If a directory a
-00018820: 6c72 6561 6479 2065 7869 7374 732c 2061  lready exists, a
-00018830: 206e 6577 2064 6972 6563 746f 7279 2077   new directory w
-00018840: 6974 6820 6e61 6d65 2060 3c6e 616d 6573  ith name `<names
-00018850: 7061 6365 3e2e 3031 6020 2865 7463 2e29  pace>.01` (etc.)
-00018860: 2077 696c 6c20 6265 2063 7265 6174 6564   will be created
-00018870: 2e0a 0a23 2320 7964 2d64 656c 6574 650a  ...## yd-delete.
-00018880: 0a54 6865 2060 7964 2d64 656c 6574 6560  .The `yd-delete`
-00018890: 2063 6f6d 6d61 6e64 2064 656c 6574 6573   command deletes
-000188a0: 2061 6e79 206f 626a 6563 7473 2063 7265   any objects cre
-000188b0: 6174 6564 2069 6e20 7468 6520 5965 6c6c  ated in the Yell
-000188c0: 6f77 446f 6720 4f62 6a65 6374 2053 746f  owDog Object Sto
-000188d0: 7265 2e0a 0a54 6865 2060 6e61 6d65 7370  re...The `namesp
-000188e0: 6163 6560 2061 6e64 2060 7461 6760 2076  ace` and `tag` v
-000188f0: 616c 7565 7320 696e 2074 6865 2060 636f  alues in the `co
-00018900: 6e66 6967 2e74 6f6d 6c60 2066 696c 6520  nfig.toml` file 
-00018910: 6172 6520 7573 6564 2074 6f20 6964 656e  are used to iden
-00018920: 7469 6679 2077 6869 6368 206f 626a 6563  tify which objec
-00018930: 7473 2074 6f20 6465 6c65 7465 2e20 4e6f  ts to delete. No
-00018940: 7465 2074 6861 7420 6974 2773 2065 6173  te that it's eas
-00018950: 7920 746f 2075 7365 2060 7964 2d64 656c  y to use `yd-del
-00018960: 6574 6560 2074 6f20 636c 6561 7220 7468  ete` to clear th
-00018970: 6520 636f 6e74 656e 7473 206f 6620 6120  e contents of a 
-00018980: 6e61 6d65 7370 6163 6520 6279 2075 7369  namespace by usi
-00018990: 6e67 2061 6e20 656d 7074 7920 6074 6167  ng an empty `tag
-000189a0: 602c 2061 7320 666f 6c6c 6f77 733a 0a0a  `, as follows:..
-000189b0: 6060 6073 6865 6c6c 0a79 642d 6465 6c65  ```shell.yd-dele
-000189c0: 7465 202d 7420 2222 0a60 6060 0a0a 5468  te -t "".```..Th
-000189d0: 6973 2063 616e 2062 6520 6578 7465 6e64  is can be extend
-000189e0: 6564 2074 6f20 616e 7920 6f74 6865 7220  ed to any other 
-000189f0: 6e61 6d65 7370 6163 6520 6279 2075 7369  namespace by usi
-00018a00: 6e67 2074 6865 2060 2d2d 6e61 6d65 7370  ng the `--namesp
-00018a10: 6163 6560 2f60 2d6e 6020 6f70 7469 6f6e  ace`/`-n` option
-00018a20: 2e0a 0a23 2320 7964 2d75 706c 6f61 640a  ...## yd-upload.
-00018a30: 0a54 6865 2060 7964 2d75 706c 6f61 6460  .The `yd-upload`
-00018a40: 2063 6f6d 6d61 6e64 2075 706c 6f61 6473   command uploads
-00018a50: 2066 696c 6573 2066 726f 6d20 7468 6520   files from the 
-00018a60: 6c6f 6361 6c20 6669 6c65 7379 7374 656d  local filesystem
-00018a70: 2074 6f20 7468 6520 5965 6c6c 6f77 446f   to the YellowDo
-00018a80: 6720 4f62 6a65 6374 2073 746f 7265 2e20  g Object store. 
-00018a90: 4669 6c65 7320 6172 6520 706c 6163 6564  Files are placed
-00018aa0: 2069 6e20 7468 6520 636f 6e66 6967 7572   in the configur
-00018ab0: 6564 2060 6e61 6d65 7370 6163 6560 2077  ed `namespace` w
-00018ac0: 6974 6869 6e20 6120 6469 7265 6374 6f72  ithin a director
-00018ad0: 7920 7375 7070 6c69 6564 2075 7369 6e67  y supplied using
-00018ae0: 2074 6865 2028 7265 7175 6972 6564 2920   the (required) 
-00018af0: 602d 2d64 6972 6563 746f 7279 6020 6f70  `--directory` op
-00018b00: 7469 6f6e 2c20 652e 672e 3a0a 0a60 6060  tion, e.g.:..```
-00018b10: 7368 656c 6c0a 7964 2d75 706c 6f61 6420  shell.yd-upload 
-00018b20: 2d2d 6469 7265 6374 6f72 7920 6d79 5f77  --directory my_w
-00018b30: 6f72 6b5f 7265 7175 6972 656d 656e 7420  ork_requirement 
-00018b40: 6669 6c65 5f31 2066 696c 655f 3220 6d6f  file_1 file_2 mo
-00018b50: 7265 6669 6c65 732f 6669 6c65 330a 6060  refiles/file3.``
-00018b60: 600a 546f 2073 7570 7072 6573 7320 7468  `.To suppress th
-00018b70: 6520 6d69 7272 6f72 696e 6720 6f66 2074  e mirroring of t
-00018b80: 6865 206c 6f63 616c 2064 6972 6563 746f  he local directo
-00018b90: 7279 2073 7472 7563 7475 7265 2077 6974  ry structure wit
-00018ba0: 6869 6e20 7468 6520 6f62 6a65 6374 2073  hin the object s
-00018bb0: 746f 7265 2c20 7573 6520 7468 6520 602d  tore, use the `-
-00018bc0: 2d66 6c61 7474 656e 2d75 706c 6f61 642d  -flatten-upload-
-00018bd0: 7061 7468 7360 206f 7220 602d 6660 206f  paths` or `-f` o
-00018be0: 7074 696f 6e2e 204e 6f74 6520 7468 6174  ption. Note that
-00018bf0: 2069 6620 7468 6973 2063 7265 6174 6573   if this creates
-00018c00: 206d 756c 7469 706c 6520 7570 6c6f 6164   multiple upload
-00018c10: 6564 2066 696c 6573 2077 6974 6820 7468  ed files with th
-00018c20: 6520 7361 6d65 2070 6174 6820 696e 2074  e same path in t
-00018c30: 6865 204f 626a 6563 7420 5374 6f72 6520  he Object Store 
-00018c40: 666f 6c64 6572 2c20 6669 6c65 7320 7769  folder, files wi
-00018c50: 6c6c 2062 6520 6f76 6572 7772 6974 7465  ll be overwritte
-00018c60: 6e2e 0a0a 4669 6c65 7320 696e 2064 6972  n...Files in dir
-00018c70: 6563 746f 7269 6573 206d 6179 2062 6520  ectories may be 
-00018c80: 7265 6375 7273 6976 656c 7920 7570 6c6f  recursively uplo
-00018c90: 6164 6564 2075 7369 6e67 2074 6865 2060  aded using the `
-00018ca0: 2d2d 7265 6375 7273 6976 6560 206f 7220  --recursive` or 
-00018cb0: 602d 7260 206f 7074 696f 6e2c 2065 2e67  `-r` option, e.g
-00018cc0: 2e3a 0a0a 6060 6073 6865 6c6c 0a79 642d  .:..```shell.yd-
-00018cd0: 7570 6c6f 6164 202d 2d64 6972 6563 746f  upload --directo
-00018ce0: 7279 206d 795f 776f 726b 5f72 6571 7569  ry my_work_requi
-00018cf0: 7265 6d65 6e74 202d 7220 6d79 6469 7220  rement -r mydir 
-00018d00: 6d79 6f74 6865 7264 6972 0a60 6060 0a0a  myotherdir.```..
-00018d10: 546f 2075 706c 6f61 6420 746f 206f 7468  To upload to oth
-00018d20: 6572 206e 616d 6573 7061 6365 732c 2075  er namespaces, u
-00018d30: 7365 2074 6865 2060 2d2d 6e61 6d65 7370  se the `--namesp
-00018d40: 6163 6560 2f60 2d6e 6020 6f70 7469 6f6e  ace`/`-n` option
-00018d50: 2e0a 0a23 2320 7964 2d73 6875 7464 6f77  ...## yd-shutdow
-00018d60: 6e0a 0a54 6865 2060 7964 2d73 6875 7464  n..The `yd-shutd
-00018d70: 6f77 6e60 2063 6f6d 6d61 6e64 2073 6875  own` command shu
-00018d80: 7473 2064 6f77 6e20 576f 726b 6572 2050  ts down Worker P
-00018d90: 6f6f 6c73 2074 6861 7420 6d61 7463 6820  ools that match 
-00018da0: 7468 6520 606e 616d 6573 7061 6365 6020  the `namespace` 
-00018db0: 616e 6420 6074 6167 6020 666f 756e 6420  and `tag` found 
-00018dc0: 696e 2074 6865 2063 6f6e 6669 6775 7261  in the configura
-00018dd0: 7469 6f6e 2066 696c 652e 2041 6c6c 2072  tion file. All r
-00018de0: 656d 6169 6e69 6e67 2077 6f72 6b20 7769  emaining work wi
-00018df0: 6c6c 2062 6520 6361 6e63 656c 6c65 642c  ll be cancelled,
-00018e00: 2062 7574 2063 7572 7265 6e74 6c79 2065   but currently e
-00018e10: 7865 6375 7469 6e67 2054 6173 6b73 2077  xecuting Tasks w
-00018e20: 696c 6c20 6265 2061 6c6c 6f77 6564 2074  ill be allowed t
-00018e30: 6f20 636f 6d70 6c65 7465 2c20 6166 7465  o complete, afte
-00018e40: 7220 7768 6963 6820 7468 6520 436f 6d70  r which the Comp
-00018e50: 7574 6520 5265 7175 6972 656d 656e 7420  ute Requirement 
-00018e60: 7769 6c6c 2062 6520 7465 726d 696e 6174  will be terminat
-00018e70: 6564 2e0a 0a23 2320 7964 2d69 6e73 7461  ed...## yd-insta
-00018e80: 6e74 6961 7465 0a0a 5468 6520 6079 642d  ntiate..The `yd-
-00018e90: 696e 7374 616e 7469 6174 6560 2063 6f6d  instantiate` com
-00018ea0: 6d61 6e64 2069 6e73 7461 6e74 6961 7465  mand instantiate
-00018eb0: 7320 6120 436f 6d70 7574 6520 5265 7175  s a Compute Requ
-00018ec0: 6972 656d 656e 7420 2869 2e65 2e2c 2061  irement (i.e., a
-00018ed0: 2073 6574 206f 6620 696e 7374 616e 6365   set of instance
-00018ee0: 7320 7468 6174 2061 7265 206d 616e 6167  s that are manag
-00018ef0: 6564 2062 7920 7468 6569 7220 6372 6561  ed by their crea
-00018f00: 746f 7220 616e 6420 646f 206e 6f74 2061  tor and do not a
-00018f10: 7574 6f6d 6174 6963 616c 6c79 2062 6563  utomatically bec
-00018f20: 6f6d 6520 7061 7274 206f 6620 6120 5965  ome part of a Ye
-00018f30: 6c6c 6f77 446f 6720 576f 726b 6572 2050  llowDog Worker P
-00018f40: 6f6f 6c29 2e0a 0a54 6869 7320 636f 6d6d  ool)...This comm
-00018f50: 616e 6420 7573 6573 2074 6865 2064 6174  and uses the dat
-00018f60: 6120 6672 6f6d 2074 6865 2060 776f 726b  a from the `work
-00018f70: 6572 506f 6f6c 6020 636f 6e66 6967 7572  erPool` configur
-00018f80: 6174 696f 6e20 7365 6374 696f 6e2c 2062  ation section, b
-00018f90: 7574 206f 6e6c 7920 7573 6573 2074 6865  ut only uses the
-00018fa0: 2060 6e61 6d65 602c 2060 7465 6d70 6c61   `name`, `templa
-00018fb0: 7465 4964 602c 2060 7461 7267 6574 496e  teId`, `targetIn
-00018fc0: 7374 616e 6365 436f 756e 7460 2c20 6069  stanceCount`, `i
-00018fd0: 6e73 7461 6e63 6554 6167 7360 2c20 6075  nstanceTags`, `u
-00018fe0: 7365 7244 6174 6160 2c20 616e 6420 6069  serData`, and `i
-00018ff0: 6d61 6765 7349 6460 2070 726f 7065 7274  magesId` propert
-00019000: 6965 732e 2049 6e20 6164 6469 7469 6f6e  ies. In addition
-00019010: 2c20 7468 6520 426f 6f6c 6561 6e20 7072  , the Boolean pr
-00019020: 6f70 6572 7479 2060 6d61 696e 7461 696e  operty `maintain
-00019030: 496e 7374 616e 6365 436f 756e 7460 2028  InstanceCount` (
-00019040: 6465 6661 756c 7420 3d20 6066 616c 7365  default = `false
-00019050: 6029 2069 7320 6176 6169 6c61 626c 6520  `) is available 
-00019060: 666f 7220 7573 6520 7769 7468 2060 7964  for use with `yd
-00019070: 2d69 6e73 7461 6e74 6961 7465 602e 0a0a  -instantiate`...
-00019080: 436f 6d70 7574 6520 5265 7175 6972 656d  Compute Requirem
-00019090: 656e 7473 2063 616e 2062 6520 696e 7374  ents can be inst
-000190a0: 616e 7469 6174 6564 2064 6972 6563 746c  antiated directl
-000190b0: 7920 6672 6f6d 204a 534f 4e20 286f 7220  y from JSON (or 
-000190c0: 4a73 6f6e 6e65 7429 2073 7065 6369 6669  Jsonnet) specifi
-000190d0: 6361 7469 6f6e 732c 2075 7369 6e67 2074  cations, using t
-000190e0: 6865 2060 2d2d 636f 6d70 7574 652d 7265  he `--compute-re
-000190f0: 7175 6972 656d 656e 7460 2028 6f72 2060  quirement` (or `
-00019100: 2d43 6029 2063 6f6d 6d61 6e64 206c 696e  -C`) command lin
-00019110: 6520 6f70 7469 6f6e 2c20 666f 6c6c 6f77  e option, follow
-00019120: 6564 2062 7920 7468 6520 6669 6c65 6e61  ed by the filena
-00019130: 6d65 2e20 5468 6520 7072 6f70 6572 7469  me. The properti
-00019140: 6573 206c 6973 7465 6420 6162 6f76 6520  es listed above 
-00019150: 7769 6c6c 2062 6520 696e 6865 7269 7465  will be inherite
-00019160: 6420 6672 6f6d 2074 6865 2063 6f6e 6669  d from the confi
-00019170: 672e 746f 6d6c 2060 776f 726b 6572 506f  g.toml `workerPo
-00019180: 6f6c 6020 7370 6563 6966 6963 6174 696f  ol` specificatio
-00019190: 6e20 6966 2074 6865 7920 6172 6520 6e6f  n if they are no
-000191a0: 7420 7072 6573 656e 7420 696e 2074 6865  t present in the
-000191b0: 204a 534f 4e20 6669 6c65 2e20 416e 2065   JSON file. An e
-000191c0: 7861 6d70 6c65 204a 534f 4e20 7370 6563  xample JSON spec
-000191d0: 6966 6963 6174 696f 6e20 6973 2073 686f  ification is sho
-000191e0: 776e 2062 656c 6f77 3a0a 0a60 6060 6a73  wn below:..```js
-000191f0: 6f6e 0a7b 0a20 2022 696d 6167 6573 4964  on.{.  "imagesId
-00019200: 223a 2022 7964 6964 3a69 6d67 6661 6d3a  ": "ydid:imgfam:
-00019210: 3030 3030 3030 3a34 3139 3632 3539 322d  000000:41962592-
-00019220: 3537 3763 2d34 6664 652d 6162 3033 2d64  577c-4fde-ab03-d
-00019230: 3835 3234 3635 6537 6638 6222 2c0a 2020  852465e7f8b",.  
-00019240: 2269 6e73 7461 6e63 6554 6167 7322 3a20  "instanceTags": 
-00019250: 7b22 6131 223a 2022 6f6e 6522 2c20 2261  {"a1": "one", "a
-00019260: 3222 3a20 2274 776f 227d 2c0a 2020 2272  2": "two"},.  "r
-00019270: 6571 7569 7265 6d65 6e74 4e61 6d65 223a  equirementName":
-00019280: 2022 6372 5f74 6573 745f 7b7b 6461 7465   "cr_test_{{date
-00019290: 7469 6d65 7d7d 222c 0a20 2022 7265 7175  time}}",.  "requ
-000192a0: 6972 656d 656e 744e 616d 6573 7061 6365  irementNamespace
-000192b0: 223a 2022 7079 6578 616d 706c 6573 222c  ": "pyexamples",
-000192c0: 0a20 2022 7265 7175 6972 656d 656e 7454  .  "requirementT
-000192d0: 6167 223a 2022 7079 6578 616d 706c 6573  ag": "pyexamples
-000192e0: 2d74 6573 7422 2c0a 2020 2274 656d 706c  -test",.  "templ
-000192f0: 6174 6549 6422 3a20 2279 6469 643a 6372  ateId": "ydid:cr
-00019300: 743a 3030 3030 3030 3a32 3330 6539 6134  t:000000:230e9a4
-00019310: 322d 3937 6462 2d34 6436 392d 6161 3931  2-97db-4d69-aa91
-00019320: 2d32 3966 6633 3039 3935 3162 3422 2c0a  -29ff309951b4",.
-00019330: 2020 2275 7365 7244 6174 6122 3a20 2223    "userData": "#
-00019340: 2f62 696e 2f62 6173 685c 6e23 4f74 6865  /bin/bash\n#Othe
-00019350: 7220 7374 7566 662e 2e2e 222c 0a20 2022  r stuff...",.  "
-00019360: 7461 7267 6574 496e 7374 616e 6365 436f  targetInstanceCo
-00019370: 756e 7422 3a20 312c 0a20 2022 6d61 696e  unt": 1,.  "main
-00019380: 7461 696e 496e 7374 616e 6365 436f 756e  tainInstanceCoun
-00019390: 7422 3a20 7472 7565 0a7d 0a60 6060 0a0a  t": true.}.```..
-000193a0: 4966 2061 2057 6f72 6b65 7220 506f 6f6c  If a Worker Pool
-000193b0: 2069 7320 6465 6669 6e65 642c 2075 7369   is defined, usi
-000193c0: 6e67 2060 776f 726b 6572 506f 6f6c 4461  ng `workerPoolDa
-000193d0: 7461 6020 696e 2074 6865 2063 6f6e 6669  ta` in the confi
-000193e0: 6775 7261 7469 6f6e 2066 696c 6520 6f72  guration file or
-000193f0: 2062 7920 7573 696e 6720 7468 6520 602d   by using the `-
-00019400: 2d77 6f72 6b65 722d 706f 6f6c 6020 286f  -worker-pool` (o
-00019410: 7220 602d 7060 2920 6f70 7469 6f6e 2c20  r `-p`) option, 
-00019420: 6079 642d 696e 7374 616e 7469 6174 6560  `yd-instantiate`
-00019430: 2077 696c 6c20 6578 7472 6163 7420 7468   will extract th
-00019440: 6520 436f 6d70 7574 6520 5265 7175 6972  e Compute Requir
-00019450: 656d 656e 7420 6672 6f6d 2074 6865 2057  ement from the W
-00019460: 6f72 6b65 7220 506f 6f6c 2073 7065 6369  orker Pool speci
-00019470: 6669 6361 7469 6f6e 2028 6967 6e6f 7269  fication (ignori
-00019480: 6e67 2057 6f72 6b65 722d 506f 6f6c 2d73  ng Worker-Pool-s
-00019490: 7065 6369 6669 6320 6461 7461 292c 2061  pecific data), a
-000194a0: 6e64 2075 7365 2074 6861 7420 666f 7220  nd use that for 
-000194b0: 696e 7374 616e 7469 6174 696e 6720 7468  instantiating th
-000194c0: 6520 436f 6d70 7574 6520 5265 7175 6972  e Compute Requir
-000194d0: 656d 656e 742e 0a0a 5573 6520 7468 6520  ement...Use the 
-000194e0: 602d 2d64 7279 2d72 756e 6020 6f70 7469  `--dry-run` opti
-000194f0: 6f6e 2074 6f20 696e 7370 6563 7420 7468  on to inspect th
-00019500: 6520 6465 7461 696c 7320 6f66 2074 6865  e details of the
-00019510: 2043 6f6d 7075 7465 2052 6571 7569 7265   Compute Require
-00019520: 6d65 6e74 2073 7065 6369 6669 6361 7469  ment specificati
-00019530: 6f6e 2074 6861 7420 7769 6c6c 2062 6520  on that will be 
-00019540: 7375 626d 6974 7465 642c 2069 6e20 4a53  submitted, in JS
-00019550: 4f4e 2066 6f72 6d61 742e 2054 6865 204a  ON format. The J
-00019560: 534f 4e20 6f75 7470 7574 206f 6620 7468  SON output of th
-00019570: 6973 2063 6f6d 6d61 6e64 2063 616e 2062  is command can b
-00019580: 6520 7573 6564 2077 6974 6820 7468 6520  e used with the 
-00019590: 602d 4360 206f 7074 696f 6e20 6162 6f76  `-C` option abov
-000195a0: 6520 286f 7220 7769 7468 2060 2d70 6020  e (or with `-p` 
-000195b0: 666f 7220 576f 726b 6572 2050 6f6f 6c20  for Worker Pool 
-000195c0: 7370 6563 6966 6963 6174 696f 6e73 292e  specifications).
-000195d0: 0a0a 2323 2320 5465 7374 2d52 756e 6e69  ..### Test-Runni
-000195e0: 6e67 2061 2044 796e 616d 6963 2054 656d  ng a Dynamic Tem
-000195f0: 706c 6174 650a 0a57 6865 6e20 6120 7468  plate..When a th
-00019600: 6520 6074 656d 706c 6174 6549 6460 206f  e `templateId` o
-00019610: 6620 6120 4479 6e61 6d69 6320 5265 7175  f a Dynamic Requ
-00019620: 6972 656d 656e 7420 6973 2075 7365 642c  irement is used,
-00019630: 2074 6865 2060 7964 2d69 6e73 7461 6e74   the `yd-instant
-00019640: 6961 7465 6020 636f 6d6d 616e 6420 6361  iate` command ca
-00019650: 6e20 6265 2075 7365 6420 746f 2072 6570  n be used to rep
-00019660: 6f72 7420 6f6e 2061 2074 6573 7420 7275  ort on a test ru
-00019670: 6e20 6f66 2074 6865 2054 656d 706c 6174  n of the Templat
-00019680: 652c 2075 7369 6e67 2074 6865 2060 2d2d  e, using the `--
-00019690: 7265 706f 7274 6020 286f 7220 602d 7260  report` (or `-r`
-000196a0: 2920 636f 6d6d 616e 6420 6c69 6e65 206f  ) command line o
-000196b0: 7074 696f 6e2e 2054 6869 7320 6361 6e20  ption. This can 
-000196c0: 6265 2075 7365 6420 7769 7468 2054 4f4d  be used with TOM
-000196d0: 4c2d 6465 6669 6e65 6420 436f 6d70 7574  L-defined Comput
-000196e0: 6520 5265 7175 6972 656d 656e 7420 7370  e Requirement sp
-000196f0: 6563 6966 6963 6174 696f 6e73 2c20 6275  ecifications, bu
-00019700: 7420 6e6f 7420 7468 6f73 6520 7468 6174  t not those that
-00019710: 2061 7265 204a 534f 4e2d 6465 6669 6e65   are JSON-define
-00019720: 642e 0a0a 4e6f 2069 6e73 7461 6e63 6573  d...No instances
-00019730: 2077 696c 6c20 6265 2070 726f 7669 7369   will be provisi
-00019740: 6f6e 6564 2064 7572 696e 6720 7468 6520  oned during the 
-00019750: 7465 7374 2072 756e 2e0a 0a46 6f72 2065  test run...For e
-00019760: 7861 6d70 6c65 3a0a 0a60 6060 7368 656c  xample:..```shel
-00019770: 6c0a 2520 7964 2d69 6e73 7461 6e74 6961  l.% yd-instantia
-00019780: 7465 202d 2d72 6570 6f72 7420 2d2d 7175  te --report --qu
-00019790: 6965 740a 0ae2 948c e294 80e2 9480 e294  iet.............
-000197a0: 80e2 9480 e294 ace2 9480 e294 80e2 9480  ................
-000197b0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000197c0: 94ac e294 80e2 9480 e294 80e2 9480 e294  ................
-000197d0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000197e0: e294 80e2 9480 e294 ace2 9480 e294 80e2  ................
-000197f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00019800: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00019810: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00019820: 9480 e294 80e2 9480 e294 80e2 94ac e294  ................
-00019830: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00019840: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00019850: 94ac e294 80e2 9480 e294 80e2 9480 e294  ................
-00019860: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00019870: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00019880: 9480 e294 ace2 9480 e294 80e2 9480 e294  ................
-00019890: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000198a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000198b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000198c0: 900a e294 8220 2020 20e2 9482 2020 2052  .....    ...   R
-000198d0: 616e 6b20 e294 8220 5072 6f76 6964 6572  ank ... Provider
-000198e0: 2020 20e2 9482 2054 7970 6520 2020 2020     ... Type     
-000198f0: 2020 2020 2020 2020 2020 2020 e294 8220              ... 
-00019900: 5265 6769 6f6e 2020 2020 e294 8220 496e  Region    ... In
-00019910: 7374 616e 6365 5479 7065 2020 20e2 9482  stanceType   ...
-00019920: 2053 6f75 7263 6520 4e61 6d65 2020 2020   Source Name    
-00019930: 2020 20e2 9482 0ae2 949c e294 80e2 9480     .............
-00019940: e294 80e2 9480 e294 bce2 9480 e294 80e2  ................
-00019950: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00019960: 80e2 94bc e294 80e2 9480 e294 80e2 9480  ................
-00019970: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00019980: 9480 e294 80e2 9480 e294 bce2 9480 e294  ................
-00019990: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000199a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000199b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000199c0: 80e2 9480 e294 80e2 9480 e294 80e2 94bc  ................
-000199d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000199e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000199f0: 80e2 94bc e294 80e2 9480 e294 80e2 9480  ................
-00019a00: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00019a10: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00019a20: 80e2 9480 e294 bce2 9480 e294 80e2 9480  ................
-00019a30: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00019a40: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00019a50: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00019a60: e294 a40a e294 8220 2031 20e2 9482 2020  .......  1 ...  
-00019a70: 2020 2020 3120 e294 8220 4157 5320 2020      1 ... AWS   
-00019a80: 2020 2020 20e2 9482 2041 7773 5370 6f74       ... AwsSpot
-00019a90: 436f 6d70 7574 6553 6f75 7263 6520 e294  ComputeSource ..
-00019aa0: 8220 6575 2d77 6573 742d 3220 e294 8220  . eu-west-2 ... 
-00019ab0: 7433 612e 6e61 6e6f 2020 2020 2020 20e2  t3a.nano       .
-00019ac0: 9482 2061 7773 7370 6f74 2d65 752d 7765  .. awsspot-eu-we
-00019ad0: 7374 2d32 20e2 9482 0ae2 949c e294 80e2  st-2 ...........
-00019ae0: 9480 e294 80e2 9480 e294 bce2 9480 e294  ................
-00019af0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00019b00: e294 80e2 94bc e294 80e2 9480 e294 80e2  ................
-00019b10: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00019b20: 80e2 9480 e294 80e2 9480 e294 bce2 9480  ................
-00019b30: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00019b40: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00019b50: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00019b60: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00019b70: 94bc e294 80e2 9480 e294 80e2 9480 e294  ................
-00019b80: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00019b90: e294 80e2 94bc e294 80e2 9480 e294 80e2  ................
-00019ba0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00019bb0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00019bc0: e294 80e2 9480 e294 bce2 9480 e294 80e2  ................
-00019bd0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00019be0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00019bf0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00019c00: 9480 e294 a40a e294 8220 2032 20e2 9482  .........  2 ...
-00019c10: 2020 2020 2020 3220 e294 8220 4157 5320        2 ... AWS 
-00019c20: 2020 2020 2020 20e2 9482 2041 7773 5370         ... AwsSp
-00019c30: 6f74 436f 6d70 7574 6553 6f75 7263 6520  otComputeSource 
-00019c40: e294 8220 6575 2d77 6573 742d 3220 e294  ... eu-west-2 ..
-00019c50: 8220 7433 612e 6d69 6372 6f20 2020 2020  . t3a.micro     
-00019c60: 20e2 9482 2061 7773 7370 6f74 2d65 752d   ... awsspot-eu-
-00019c70: 7765 7374 2d32 20e2 9482 0ae2 949c e294  west-2 .........
-00019c80: 80e2 9480 e294 80e2 9480 e294 bce2 9480  ................
-00019c90: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00019ca0: 9480 e294 80e2 94bc e294 80e2 9480 e294  ................
-00019cb0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00019cc0: e294 80e2 9480 e294 80e2 9480 e294 bce2  ................
-00019cd0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00019ce0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00019cf0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00019d00: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00019d10: 80e2 94bc e294 80e2 9480 e294 80e2 9480  ................
-00019d20: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00019d30: 9480 e294 80e2 94bc e294 80e2 9480 e294  ................
-00019d40: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00019d50: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00019d60: 9480 e294 80e2 9480 e294 bce2 9480 e294  ................
+00013bc0: 2020 7c20 6031 6020 2020 2020 2020 2020    | `1`         
+00013bd0: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
+00013be0: 6074 656d 706c 6174 6549 6460 2020 2020  `templateId`    
+00013bf0: 2020 2020 2020 2020 2020 7c20 5468 6520            | The 
+00013c00: 5965 6c6c 6f77 446f 6720 436f 6d70 7574  YellowDog Comput
+00013c10: 6520 5465 6d70 6c61 7465 2049 4420 746f  e Template ID to
+00013c20: 2075 7365 2066 6f72 2070 726f 7669 7369   use for provisi
+00013c30: 6f6e 696e 672e 2028 2a2a 5265 7175 6972  oning. (**Requir
+00013c40: 6564 2a2a 2c20 6e6f 2064 6566 6175 6c74  ed**, no default
+00013c50: 2070 726f 7669 6465 642e 2920 2020 2020   provided.)     
+00013c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c70: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+00013c80: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+00013c90: 7c20 6075 7365 7244 6174 6160 2020 2020  | `userData`    
+00013ca0: 2020 2020 2020 2020 2020 2020 7c20 5573              | Us
+00013cb0: 6572 2044 6174 6120 746f 2062 6520 7375  er Data to be su
+00013cc0: 7070 6c69 6564 2074 6f20 696e 7374 616e  pplied to instan
+00013cd0: 6365 7320 6f6e 2062 6f6f 742e 2020 2020  ces on boot.    
+00013ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d20: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
+00013d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d40: 7c0a 7c20 6075 7365 7244 6174 6146 696c  |.| `userDataFil
+00013d50: 6560 2020 2020 2020 2020 2020 2020 7c20  e`            | 
+00013d60: 4173 2061 626f 7665 2c20 6275 7420 7265  As above, but re
+00013d70: 6164 2074 6865 2055 7365 7220 4461 7461  ad the User Data
+00013d80: 2066 726f 6d20 7468 6520 6669 6c65 6e61   from the filena
+00013d90: 6d65 2073 7570 706c 6965 6420 696e 2074  me supplied in t
+00013da0: 6869 7320 7072 6f70 6572 7479 2e20 2020  his property.   
+00013db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013dd0: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+00013de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013df0: 2020 7c0a 7c20 6075 7365 7244 6174 6146    |.| `userDataF
+00013e00: 696c 6573 6020 2020 2020 2020 2020 2020  iles`           
+00013e10: 7c20 4173 2061 626f 7665 2c20 6275 7420  | As above, but 
+00013e20: 6372 6561 7465 2074 6865 2055 7365 7220  create the User 
+00013e30: 4461 7461 2062 7920 636f 6e63 6174 656e  Data by concaten
+00013e40: 6174 696e 6720 7468 6520 636f 6e74 656e  ating the conten
+00013e50: 7473 206f 6620 7468 6520 6c69 7374 206f  ts of the list o
+00013e60: 6620 6669 6c65 6e61 6d65 7320 7375 7070  f filenames supp
+00013e70: 6c69 6564 2069 6e20 7468 6973 2070 726f  lied in this pro
+00013e80: 7065 7274 792e 2020 2020 7c20 2020 2020  perty.    |     
+00013e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ea0: 2020 2020 7c0a 7c20 6077 6f72 6b65 7273      |.| `workers
+00013eb0: 5065 7256 4350 5560 2020 2020 2020 2020  PerVCPU`        
+00013ec0: 2020 7c20 5468 6520 6e75 6d62 6572 206f    | The number o
+00013ed0: 6620 576f 726b 6572 7320 746f 2065 7374  f Workers to est
+00013ee0: 6162 6c69 7368 2070 6572 2076 4350 5520  ablish per vCPU 
+00013ef0: 6f6e 2065 6163 6820 6e6f 6465 2069 6e20  on each node in 
+00013f00: 7468 6520 576f 726b 6572 2050 6f6f 6c2e  the Worker Pool.
+00013f10: 2028 4f76 6572 7269 6465 7320 6077 6f72   (Overrides `wor
+00013f20: 6b65 7273 5065 724e 6f64 6560 2e29 2020  kersPerNode`.)  
+00013f30: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
+00013f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013f50: 2020 2020 2020 7c0a 7c20 6077 6f72 6b65        |.| `worke
+00013f60: 7273 5065 724e 6f64 6560 2020 2020 2020  rsPerNode`      
+00013f70: 2020 2020 7c20 5468 6520 6e75 6d62 6572      | The number
+00013f80: 206f 6620 576f 726b 6572 7320 746f 2065   of Workers to e
+00013f90: 7374 6162 6c69 7368 206f 6e20 6561 6368  stablish on each
+00013fa0: 206e 6f64 6520 696e 2074 6865 2057 6f72   node in the Wor
+00013fb0: 6b65 7220 506f 6f6c 2e20 2020 2020 2020  ker Pool.       
+00013fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013fe0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00013ff0: 6031 6020 2020 2020 2020 2020 2020 2020  `1`             
+00014000: 2020 2020 2020 2020 7c0a 7c20 6077 6f72          |.| `wor
+00014010: 6b65 7250 6f6f 6c44 6174 6160 2020 2020  kerPoolData`    
+00014020: 2020 2020 2020 7c20 5468 6520 6e61 6d65        | The name
+00014030: 206f 6620 6120 6669 6c65 2063 6f6e 7461   of a file conta
+00014040: 696e 696e 6720 6120 4a53 4f4e 2064 6f63  ining a JSON doc
+00014050: 756d 656e 7420 6465 6669 6e69 6e67 2061  ument defining a
+00014060: 2057 6f72 6b65 7220 506f 6f6c 2e20 2020   Worker Pool.   
+00014070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000140a0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+000140b0: 2020 2020 2020 2020 2020 7c0a 7c20 6077            |.| `w
+000140c0: 6f72 6b65 7254 6167 6020 2020 2020 2020  orkerTag`       
+000140d0: 2020 2020 2020 2020 7c20 5468 6520 576f          | The Wo
+000140e0: 726b 6572 2054 6167 2074 6f20 7075 626c  rker Tag to publ
+000140f0: 6973 6820 666f 7220 7468 6520 616c 6c20  ish for the all 
+00014100: 6f66 2074 6865 2057 6f72 6b65 7273 206f  of the Workers o
+00014110: 6e20 7468 6520 6e6f 6465 2e20 2020 2020  n the node.     
+00014120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014150: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
+00014160: 2020 2020 2020 2020 2020 2020 7c0a 0a23              |..#
+00014170: 2320 4175 746f 6d61 7469 6320 5072 6f70  # Automatic Prop
+00014180: 6572 7469 6573 0a0a 5468 6520 6e61 6d65  erties..The name
+00014190: 206f 6620 7468 6520 576f 726b 6572 2050   of the Worker P
+000141a0: 6f6f 6c2c 2069 6620 6e6f 7420 7375 7070  ool, if not supp
+000141b0: 6c69 6564 2c20 6973 2061 7574 6f6d 6174  lied, is automat
+000141c0: 6963 616c 6c79 2067 656e 6572 6174 6564  ically generated
+000141d0: 2075 7369 6e67 2061 2063 6f6e 6361 7465   using a concate
+000141e0: 6e61 7469 6f6e 206f 6620 6077 705f 602c  nation of `wp_`,
+000141f0: 2074 6865 2060 7461 6760 2070 726f 7065   the `tag` prope
+00014200: 7274 792c 2061 2055 5443 2074 696d 6573  rty, a UTC times
+00014210: 7461 6d70 2c20 616e 6420 7468 7265 6520  tamp, and three 
+00014220: 7261 6e64 6f6d 2068 6578 2063 6861 7261  random hex chara
+00014230: 6374 6572 733a 2065 2c67 2c2e 2060 7770  cters: e,g,. `wp
+00014240: 5f6d 7974 6167 5f32 3231 3032 342d 3135  _mytag_221024-15
+00014250: 3535 3234 2d62 3061 602e 0a0a 2323 2054  5524-b0a`...## T
+00014260: 4f4d 4c20 5072 6f70 6572 7469 6573 2069  OML Properties i
+00014270: 6e20 7468 6520 6077 6f72 6b65 7250 6f6f  n the `workerPoo
+00014280: 6c60 2053 6563 7469 6f6e 0a0a 4865 7265  l` Section..Here
+00014290: 2773 2061 6e20 6578 616d 706c 6520 6f66  's an example of
+000142a0: 2074 6865 2060 776f 726b 6572 506f 6f6c   the `workerPool
+000142b0: 6020 7365 6374 696f 6e20 6f66 2061 2054  ` section of a T
+000142c0: 4f4d 4c20 636f 6e66 6967 7572 6174 696f  OML configuratio
+000142d0: 6e20 6669 6c65 2c20 7368 6f77 696e 6720  n file, showing 
+000142e0: 616c 6c20 7468 6520 706f 7373 6962 6c65  all the possible
+000142f0: 2070 726f 7065 7274 6965 7320 7468 6174   properties that
+00014300: 2063 616e 2062 6520 7365 743a 0a0a 6060   can be set:..``
+00014310: 6074 6f6d 6c0a 5b77 6f72 6b65 7250 6f6f  `toml.[workerPoo
+00014320: 6c5d 0a20 2020 2069 646c 654e 6f64 6553  l].    idleNodeS
+00014330: 6875 7464 6f77 6e45 6e61 626c 6564 203d  hutdownEnabled =
+00014340: 2074 7275 650a 2020 2020 6964 6c65 4e6f   true.    idleNo
+00014350: 6465 5368 7574 646f 776e 5469 6d65 6f75  deShutdownTimeou
+00014360: 7420 3d20 3130 2e30 0a20 2020 2069 646c  t = 10.0.    idl
+00014370: 6550 6f6f 6c53 6875 7464 6f77 6e45 6e61  ePoolShutdownEna
+00014380: 626c 6564 203d 2074 7275 650a 2020 2020  bled = true.    
+00014390: 6964 6c65 506f 6f6c 5368 7574 646f 776e  idlePoolShutdown
+000143a0: 5469 6d65 6f75 7420 3d20 3630 2e30 0a20  Timeout = 60.0. 
+000143b0: 2020 2069 6d61 6765 7349 6420 3d20 2279     imagesId = "y
+000143c0: 6469 643a 696d 6766 616d 3a30 3030 3030  did:imgfam:00000
+000143d0: 303a 3431 3936 3235 3932 2d35 3737 632d  0:41962592-577c-
+000143e0: 3466 6465 2d61 6230 332d 6438 3532 3436  4fde-ab03-d85246
+000143f0: 3565 3766 3862 220a 2020 2020 696e 7374  5e7f8b".    inst
+00014400: 616e 6365 5461 6773 203d 207b 7d0a 2020  anceTags = {}.  
+00014410: 2020 6d61 784e 6f64 6573 203d 2031 0a20    maxNodes = 1. 
+00014420: 2020 206d 696e 4e6f 6465 7320 3d20 310a     minNodes = 1.
+00014430: 2020 2020 6e61 6d65 203d 2022 6d79 2d77      name = "my-w
+00014440: 6f72 6b65 722d 706f 6f6c 220a 2020 2020  orker-pool".    
+00014450: 6e6f 6465 426f 6f74 5469 6d65 6f75 7420  nodeBootTimeout 
+00014460: 3d20 350a 2020 2020 7461 7267 6574 496e  = 5.    targetIn
+00014470: 7374 616e 6365 436f 756e 7420 3d20 310a  stanceCount = 1.
+00014480: 2020 2020 7465 6d70 6c61 7465 4964 203d      templateId =
+00014490: 2022 7964 6964 3a63 7274 3a44 3943 3534   "ydid:crt:D9C54
+000144a0: 383a 3436 3561 3130 3763 2d37 6365 612d  8:465a107c-7cea-
+000144b0: 3436 6533 2d39 6664 642d 3135 3131 3663  46e3-9fdd-15116c
+000144c0: 6239 3263 3430 220a 2020 2020 2320 4e6f  b92c40".    # No
+000144d0: 7465 3a20 6f6e 6c79 206f 6e65 206f 6620  te: only one of 
+000144e0: 2775 7365 7244 6174 6127 2f27 7573 6572  'userData'/'user
+000144f0: 4461 7461 4669 6c65 272f 2775 7365 7244  DataFile'/'userD
+00014500: 6174 6146 696c 6573 2720 7368 6f75 6c64  ataFiles' should
+00014510: 2062 6520 7365 740a 2020 2020 7573 6572   be set.    user
+00014520: 4461 7461 203d 2022 220a 2020 2020 7573  Data = "".    us
+00014530: 6572 4461 7461 4669 6c65 203d 2022 6d79  erDataFile = "my
+00014540: 7573 6572 6461 7461 2e74 7874 220a 2020  userdata.txt".  
+00014550: 2020 7573 6572 4461 7461 4669 6c65 7320    userDataFiles 
+00014560: 3d20 5b22 6d79 7573 6572 6461 7461 312e  = ["myuserdata1.
+00014570: 7478 7422 2c20 226d 7975 7365 7264 6174  txt", "myuserdat
+00014580: 6132 2e74 7874 225d 0a20 2020 2077 6f72  a2.txt"].    wor
+00014590: 6b65 7254 6167 203d 2022 7461 672d 7b7b  kerTag = "tag-{{
+000145a0: 7573 6572 6e61 6d65 7d7d 220a 2020 2020  username}}".    
+000145b0: 2320 5370 6563 6966 7920 6569 7468 6572  # Specify either
+000145c0: 2077 6f72 6b65 7273 5065 724e 6f64 6520   workersPerNode 
+000145d0: 6f72 2077 6f72 6b65 7273 5065 7256 4350  or workersPerVCP
+000145e0: 550a 2020 2020 776f 726b 6572 7350 6572  U.    workersPer
+000145f0: 4e6f 6465 203d 2031 0a20 2020 2077 6f72  Node = 1.    wor
+00014600: 6b65 7273 5065 7256 4350 5520 3d20 310a  kersPerVCPU = 1.
+00014610: 2320 2020 776f 726b 6572 506f 6f6c 4461  #   workerPoolDa
+00014620: 7461 203d 2022 776f 726b 6572 5f70 6f6f  ta = "worker_poo
+00014630: 6c2e 6a73 6f6e 220a 6060 600a 0a23 2320  l.json".```..## 
+00014640: 576f 726b 6572 2050 6f6f 6c20 5370 6563  Worker Pool Spec
+00014650: 6966 6963 6174 696f 6e20 5573 696e 6720  ification Using 
+00014660: 4a53 4f4e 2044 6f63 756d 656e 7473 0a0a  JSON Documents..
+00014670: 4974 2773 2061 6c73 6f20 706f 7373 6962  It's also possib
+00014680: 6c65 2074 6f20 6361 7074 7572 6520 6120  le to capture a 
+00014690: 576f 726b 6572 2050 6f6f 6c20 6465 6669  Worker Pool defi
+000146a0: 6e69 7469 6f6e 2061 7320 6120 4a53 4f4e  nition as a JSON
+000146b0: 2064 6f63 756d 656e 742e 2054 6865 204a   document. The J
+000146c0: 534f 4e20 6669 6c65 6e61 6d65 2063 616e  SON filename can
+000146d0: 2062 6520 7375 7070 6c69 6564 2065 6974   be supplied eit
+000146e0: 6865 7220 7573 696e 6720 7468 6520 636f  her using the co
+000146f0: 6d6d 616e 6420 6c69 6e65 2077 6974 6820  mmand line with 
+00014700: 7468 6520 602d 2d77 6f72 6b65 722d 706f  the `--worker-po
+00014710: 6f6c 6020 6f72 2060 2d70 6020 7061 7261  ol` or `-p` para
+00014720: 6d65 7465 7220 7769 7468 2060 7964 2d70  meter with `yd-p
+00014730: 726f 7669 7369 6f6e 602c 206f 7220 6279  rovision`, or by
+00014740: 2070 6f70 756c 6174 696e 6720 7468 6520   populating the 
+00014750: 6077 6f72 6b65 7250 6f6f 6c44 6174 6160  `workerPoolData`
+00014760: 2070 726f 7065 7274 7920 696e 2074 6865   property in the
+00014770: 2054 4f4d 4c20 636f 6e66 6967 7572 6174   TOML configurat
+00014780: 696f 6e20 6669 6c65 2077 6974 6820 7468  ion file with th
+00014790: 6520 4a53 4f4e 2066 696c 656e 616d 652e  e JSON filename.
+000147a0: 2043 6f6d 6d61 6e64 206c 696e 6520 7370   Command line sp
+000147b0: 6563 6966 6963 6174 696f 6e20 7461 6b65  ecification take
+000147c0: 7320 7072 696f 7269 7479 206f 7665 7220  s priority over 
+000147d0: 544f 4d4c 2073 7065 6369 6669 6361 7469  TOML specificati
+000147e0: 6f6e 2e0a 0a54 6865 204a 534f 4e20 7370  on...The JSON sp
+000147f0: 6563 6966 6963 6174 696f 6e20 616c 6c6f  ecification allo
+00014800: 7773 2074 6865 2063 7265 6174 696f 6e20  ws the creation 
+00014810: 6f66 202a 2a41 6476 616e 6365 6420 576f  of **Advanced Wo
+00014820: 726b 6572 2050 6f6f 6c73 2a2a 2c20 7769  rker Pools**, wi
+00014830: 7468 2064 6966 6665 7265 6e74 206e 6f64  th different nod
+00014840: 6520 7479 7065 7320 616e 6420 7468 6520  e types and the 
+00014850: 6162 696c 6974 7920 746f 2073 7065 6369  ability to speci
+00014860: 6679 204e 6f64 6520 4163 7469 6f6e 732e  fy Node Actions.
+00014870: 0a0a 5768 656e 2075 7369 6e67 2061 204a  ..When using a J
+00014880: 534f 4e20 646f 6375 6d65 6e74 2074 6f20  SON document to 
+00014890: 7370 6563 6966 7920 7468 6520 576f 726b  specify the Work
+000148a0: 6572 2050 6f6f 6c2c 2074 6865 2073 6368  er Pool, the sch
+000148b0: 656d 6120 6f66 2074 6865 2064 6f63 756d  ema of the docum
+000148c0: 656e 7420 6973 2069 6465 6e74 6963 616c  ent is identical
+000148d0: 2074 6f20 7468 6174 2065 7870 6563 7465   to that expecte
+000148e0: 6420 6279 2074 6865 2059 656c 6c6f 7744  d by the YellowD
+000148f0: 6f67 2052 4553 5420 4150 4920 666f 7220  og REST API for 
+00014900: 576f 726b 6572 2050 6f6f 6c20 5072 6f76  Worker Pool Prov
+00014910: 6973 696f 6e69 6e67 2e0a 0a23 2323 2057  isioning...### W
+00014920: 6f72 6b65 7220 506f 6f6c 204a 534f 4e20  orker Pool JSON 
+00014930: 4578 616d 706c 6573 0a0a 5468 6520 6578  Examples..The ex
+00014940: 616d 706c 6520 6265 6c6f 7720 6973 206f  ample below is o
+00014950: 6620 6120 7369 6d70 6c65 204a 534f 4e20  f a simple JSON 
+00014960: 7370 6563 6966 6963 6174 696f 6e20 6f66  specification of
+00014970: 2061 2057 6f72 6b65 7220 506f 6f6c 2077   a Worker Pool w
+00014980: 6974 6820 6f6e 6520 696e 6974 6961 6c20  ith one initial 
+00014990: 6e6f 6465 2c20 576f 726b 6572 2050 6f6f  node, Worker Poo
+000149a0: 6c20 7368 7574 646f 776e 2c20 6574 632e  l shutdown, etc.
+000149b0: 0a0a 6060 606a 736f 6e0a 7b0a 2020 2272  ..```json.{.  "r
+000149c0: 6571 7569 7265 6d65 6e74 5465 6d70 6c61  equirementTempla
+000149d0: 7465 5573 6167 6522 3a20 7b0a 2020 2020  teUsage": {.    
+000149e0: 226d 6169 6e74 6169 6e49 6e73 7461 6e63  "maintainInstanc
+000149f0: 6543 6f75 6e74 223a 2066 616c 7365 2c0a  eCount": false,.
+00014a00: 2020 2020 2272 6571 7569 7265 6d65 6e74      "requirement
+00014a10: 4e61 6d65 223a 2022 7770 5f70 7965 782d  Name": "wp_pyex-
+00014a20: 7072 696d 6573 5f32 3330 3131 332d 3136  primes_230113-16
+00014a30: 3135 3238 2d64 6130 222c 0a20 2020 2022  1528-da0",.    "
+00014a40: 7265 7175 6972 656d 656e 744e 616d 6573  requirementNames
+00014a50: 7061 6365 223a 2022 7079 6578 616d 706c  pace": "pyexampl
+00014a60: 6573 222c 0a20 2020 2022 7265 7175 6972  es",.    "requir
+00014a70: 656d 656e 7454 6167 223a 2022 7079 6578  ementTag": "pyex
+00014a80: 2d70 7269 6d65 7322 2c0a 2020 2020 2274  -primes",.    "t
+00014a90: 6172 6765 7449 6e73 7461 6e63 6543 6f75  argetInstanceCou
+00014aa0: 6e74 223a 2031 2c0a 2020 2020 2274 656d  nt": 1,.    "tem
+00014ab0: 706c 6174 6549 6422 3a20 2279 6469 643a  plateId": "ydid:
+00014ac0: 6372 743a 4439 4335 3438 3a34 3635 6131  crt:D9C548:465a1
+00014ad0: 3037 632d 3763 6561 2d34 3665 332d 3966  07c-7cea-46e3-9f
+00014ae0: 6464 2d31 3531 3136 6362 3932 6334 3022  dd-15116cb92c40"
+00014af0: 0a20 207d 2c0a 2020 2270 726f 7669 7369  .  },.  "provisi
+00014b00: 6f6e 6564 5072 6f70 6572 7469 6573 223a  onedProperties":
+00014b10: 207b 0a20 2020 2022 6964 6c65 4e6f 6465   {.    "idleNode
+00014b20: 5368 7574 646f 776e 223a 207b 2265 6e61  Shutdown": {"ena
+00014b30: 626c 6564 223a 2074 7275 652c 2022 7469  bled": true, "ti
+00014b40: 6d65 6f75 7422 3a20 2250 5431 304d 227d  meout": "PT10M"}
+00014b50: 2c0a 2020 2020 2269 646c 6550 6f6f 6c53  ,.    "idlePoolS
+00014b60: 6875 7464 6f77 6e22 3a20 7b22 656e 6162  hutdown": {"enab
+00014b70: 6c65 6422 3a20 7472 7565 2c20 2274 696d  led": true, "tim
+00014b80: 656f 7574 223a 2022 5054 3148 227d 2c0a  eout": "PT1H"},.
+00014b90: 2020 2020 2263 7265 6174 654e 6f64 6557      "createNodeW
+00014ba0: 6f72 6b65 7273 223a 207b 2274 6172 6765  orkers": {"targe
+00014bb0: 7443 6f75 6e74 223a 2031 2c20 2274 6172  tCount": 1, "tar
+00014bc0: 6765 7454 7970 6522 3a20 2250 4552 5f56  getType": "PER_V
+00014bd0: 4350 5522 7d2c 0a20 2020 2022 6d61 784e  CPU"},.    "maxN
+00014be0: 6f64 6573 223a 2035 2c0a 2020 2020 226d  odes": 5,.    "m
+00014bf0: 696e 4e6f 6465 7322 3a20 302c 0a20 2020  inNodes": 0,.   
+00014c00: 2022 6e6f 6465 426f 6f74 5469 6d65 6f75   "nodeBootTimeou
+00014c10: 7422 3a20 2250 5435 4d22 2c0a 2020 2020  t": "PT5M",.    
+00014c20: 226e 6f64 6549 646c 6547 7261 6365 5065  "nodeIdleGracePe
+00014c30: 7269 6f64 223a 2022 5054 334d 222c 0a20  riod": "PT3M",. 
+00014c40: 2020 2022 6e6f 6465 4964 6c65 5469 6d65     "nodeIdleTime
+00014c50: 4c69 6d69 7422 3a20 2250 5433 4d22 2c0a  Limit": "PT3M",.
+00014c60: 2020 2020 2277 6f72 6b65 7254 6167 223a      "workerTag":
+00014c70: 2022 7079 6578 2d62 6173 682d 646f 636b   "pyex-bash-dock
+00014c80: 6572 220a 2020 7d0a 7d0a 6060 600a 0a54  er".  }.}.```..T
+00014c90: 6865 206e 6578 7420 6578 616d 706c 6520  he next example 
+00014ca0: 6973 206f 6620 6120 7265 6c61 7469 7665  is of a relative
+00014cb0: 6c79 2072 6963 6820 4a53 4f4e 2073 7065  ly rich JSON spe
+00014cc0: 6369 6669 6361 7469 6f6e 206f 6620 616e  cification of an
+00014cd0: 2041 6476 616e 6365 6420 576f 726b 6572   Advanced Worker
+00014ce0: 2050 6f6f 6c2c 2066 726f 6d20 6f6e 6520   Pool, from one 
+00014cf0: 6f66 2074 6865 2059 656c 6c6f 7744 6f67  of the YellowDog
+00014d00: 2064 656d 6f73 2e20 4974 2069 6e63 6c75   demos. It inclu
+00014d10: 6465 7320 6e6f 6465 2073 7065 6369 616c  des node special
+00014d20: 6973 6174 696f 6e2c 2061 6e64 2061 6374  isation, and act
+00014d30: 696f 6e20 6772 6f75 7073 2074 6861 7420  ion groups that 
+00014d40: 7265 7370 6f6e 6420 746f 2074 6865 2060  respond to the `
+00014d50: 5354 4152 5455 505f 4e4f 4445 535f 4144  STARTUP_NODES_AD
+00014d60: 4445 4460 2061 6e64 2060 4e4f 4445 535f  DED` and `NODES_
+00014d70: 4144 4445 4460 2065 7665 6e74 7320 746f  ADDED` events to
+00014d80: 2064 7269 7665 202a 2a4e 6f64 6520 4163   drive **Node Ac
+00014d90: 7469 6f6e 732a 2a2e 0a0a 6060 606a 736f  tions**...```jso
+00014da0: 6e0a 7b0a 2020 2272 6571 7569 7265 6d65  n.{.  "requireme
+00014db0: 6e74 5465 6d70 6c61 7465 5573 6167 6522  ntTemplateUsage"
+00014dc0: 3a20 7b0a 2020 2020 226d 6169 6e74 6169  : {.    "maintai
+00014dd0: 6e49 6e73 7461 6e63 6543 6f75 6e74 223a  nInstanceCount":
+00014de0: 2066 616c 7365 2c0a 2020 2020 2274 6172   false,.    "tar
+00014df0: 6765 7449 6e73 7461 6e63 6543 6f75 6e74  getInstanceCount
+00014e00: 223a 2036 2c0a 2020 2020 2274 656d 706c  ": 6,.    "templ
+00014e10: 6174 6549 6422 3a20 2279 6469 643a 6372  ateId": "ydid:cr
+00014e20: 743a 4439 4335 3438 3a61 3765 6461 3238  t:D9C548:a7eda28
+00014e30: 372d 6639 6436 2d34 6263 382d 6232 6463  7-f9d6-4bc8-b2dc
+00014e40: 2d34 3535 3334 3430 3537 3235 3722 2c0a  -455344057257",.
+00014e50: 2020 2020 2272 6571 7569 7265 6d65 6e74      "requirement
+00014e60: 4e61 6d65 223a 2022 7770 5f70 7965 782d  Name": "wp_pyex-
+00014e70: 736c 7572 6d5f 3233 3031 3133 2d31 3635  slurm_230113-165
+00014e80: 3631 352d 3262 3722 2c0a 2020 2020 2272  615-2b7",.    "r
+00014e90: 6571 7569 7265 6d65 6e74 4e61 6d65 7370  equirementNamesp
+00014ea0: 6163 6522 3a20 2270 7965 7861 6d70 6c65  ace": "pyexample
+00014eb0: 7322 2c0a 2020 2020 2272 6571 7569 7265  s",.    "require
+00014ec0: 6d65 6e74 5461 6722 3a20 2270 7965 782d  mentTag": "pyex-
+00014ed0: 736c 7572 6d22 0a20 207d 2c0a 2020 2270  slurm".  },.  "p
+00014ee0: 726f 7669 7369 6f6e 6564 5072 6f70 6572  rovisionedProper
+00014ef0: 7469 6573 223a 207b 0a20 2020 2022 6372  ties": {.    "cr
+00014f00: 6561 7465 4e6f 6465 576f 726b 6572 7322  eateNodeWorkers"
+00014f10: 3a20 7b22 7461 7267 6574 436f 756e 7422  : {"targetCount"
+00014f20: 3a20 302c 2022 7461 7267 6574 5479 7065  : 0, "targetType
+00014f30: 223a 2022 5045 525f 4e4f 4445 227d 2c0a  ": "PER_NODE"},.
+00014f40: 2020 2020 226e 6f64 6543 6f6e 6669 6775      "nodeConfigu
+00014f50: 7261 7469 6f6e 223a 207b 0a20 2020 2020  ration": {.     
+00014f60: 2022 6e6f 6465 5479 7065 7322 3a20 5b0a   "nodeTypes": [.
+00014f70: 2020 2020 2020 2020 7b22 6e61 6d65 223a          {"name":
+00014f80: 2022 736c 7572 6d63 746c 6422 2c20 2263   "slurmctld", "c
+00014f90: 6f75 6e74 223a 2031 7d2c 0a20 2020 2020  ount": 1},.     
+00014fa0: 2020 207b 226e 616d 6522 3a20 2273 6c75     {"name": "slu
+00014fb0: 726d 6422 2c20 226d 696e 223a 2035 2c20  rmd", "min": 5, 
+00014fc0: 2273 6c6f 744e 756d 6265 7269 6e67 223a  "slotNumbering":
+00014fd0: 2022 5245 5553 4142 4c45 227d 0a20 2020   "REUSABLE"}.   
+00014fe0: 2020 205d 2c0a 2020 2020 2020 226e 6f64     ],.      "nod
+00014ff0: 6545 7665 6e74 7322 3a20 7b0a 2020 2020  eEvents": {.    
+00015000: 2020 2020 2253 5441 5254 5550 5f4e 4f44      "STARTUP_NOD
+00015010: 4553 5f41 4444 4544 223a 205b 0a20 2020  ES_ADDED": [.   
+00015020: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+00015030: 2020 2020 2022 6163 7469 6f6e 7322 3a20       "actions": 
+00015040: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
+00015050: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00015060: 2020 2261 6374 696f 6e22 3a20 2257 5249    "action": "WRI
+00015070: 5445 5f46 494c 4522 2c0a 2020 2020 2020  TE_FILE",.      
+00015080: 2020 2020 2020 2020 2020 2270 6174 6822            "path"
+00015090: 3a20 226e 6f64 6573 2e6a 736f 6e22 2c0a  : "nodes.json",.
+000150a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000150b0: 2263 6f6e 7465 6e74 223a 2022 7b5c 6e20  "content": "{\n 
+000150c0: 205c 226e 6f64 6573 5c22 3a20 5b5c 6e7b   \"nodes\": [\n{
+000150d0: 7b23 6f74 6865 724e 6f64 6573 7d7d 5c6e  {#otherNodes}}\n
+000150e0: 2020 2020 7b5c 6e20 2020 2020 205c 226e      {\n      \"n
+000150f0: 616d 655c 223a 205c 2273 6c75 726d 647b  ame\": \"slurmd{
+00015100: 7b64 6574 6169 6c73 2e6e 6f64 6553 6c6f  {details.nodeSlo
+00015110: 747d 7d5c 222c 5c6e 2020 2020 2020 5c22  t}}\",\n      \"
+00015120: 6970 5c22 3a20 5c22 7b7b 6465 7461 696c  ip\": \"{{detail
+00015130: 732e 7072 6976 6174 6549 7041 6464 7265  s.privateIpAddre
+00015140: 7373 7d7d 5c22 5c6e 2020 2020 7d7b 7b5e  ss}}\"\n    }{{^
+00015150: 2d6c 6173 747d 7d2c 7b7b 2f2d 6c61 7374  -last}},{{/-last
+00015160: 7d7d 5c6e 7b7b 2f6f 7468 6572 4e6f 6465  }}\n{{/otherNode
+00015170: 737d 7d5c 6e20 205d 5c6e 7d22 2c0a 2020  s}}\n  ]\n}",.  
+00015180: 2020 2020 2020 2020 2020 2020 2020 226e                "n
+00015190: 6f64 6554 7970 6573 223a 205b 2273 6c75  odeTypes": ["slu
+000151a0: 726d 6374 6c64 225d 0a20 2020 2020 2020  rmctld"].       
+000151b0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+000151c0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+000151d0: 2020 2020 2020 2020 2020 2261 6374 696f            "actio
+000151e0: 6e22 3a20 2252 554e 5f43 4f4d 4d41 4e44  n": "RUN_COMMAND
+000151f0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00015200: 2020 2022 7061 7468 223a 2022 7374 6172     "path": "star
+00015210: 745f 7369 6d70 6c65 5f73 6c75 726d 6374  t_simple_slurmct
+00015220: 6c64 222c 0a20 2020 2020 2020 2020 2020  ld",.           
+00015230: 2020 2020 2022 6172 6775 6d65 6e74 7322       "arguments"
+00015240: 3a20 5b22 6e6f 6465 732e 6a73 6f6e 225d  : ["nodes.json"]
+00015250: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00015260: 2020 2265 6e76 6972 6f6e 6d65 6e74 223a    "environment":
+00015270: 207b 2245 5841 4d50 4c45 223a 2022 464f   {"EXAMPLE": "FO
+00015280: 4f22 7d2c 0a20 2020 2020 2020 2020 2020  O"},.           
+00015290: 2020 2020 2022 6e6f 6465 5479 7065 7322       "nodeTypes"
+000152a0: 3a20 5b22 736c 7572 6d63 746c 6422 5d0a  : ["slurmctld"].
+000152b0: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
+000152c0: 2020 2020 2020 2020 2020 2020 5d0a 2020              ].  
+000152d0: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+000152e0: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+000152f0: 2020 2022 6163 7469 6f6e 7322 3a20 5b0a     "actions": [.
+00015300: 2020 2020 2020 2020 2020 2020 2020 7b0a                {.
+00015310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015320: 2261 6374 696f 6e22 3a20 2252 554e 5f43  "action": "RUN_C
+00015330: 4f4d 4d41 4e44 222c 0a20 2020 2020 2020  OMMAND",.       
+00015340: 2020 2020 2020 2020 2022 7061 7468 223a           "path":
+00015350: 2022 7374 6172 745f 7369 6d70 6c65 5f73   "start_simple_s
+00015360: 6c75 726d 6422 2c0a 2020 2020 2020 2020  lurmd",.        
+00015370: 2020 2020 2020 2020 2261 7267 756d 656e          "argumen
+00015380: 7473 223a 205b 227b 7b6e 6f64 6573 4279  ts": ["{{nodesBy
+00015390: 5479 7065 2e73 6c75 726d 6374 6c64 2e30  Type.slurmctld.0
+000153a0: 2e64 6574 6169 6c73 2e70 7269 7661 7465  .details.private
+000153b0: 4970 4164 6472 6573 737d 7d22 2c20 227b  IpAddress}}", "{
+000153c0: 7b6e 6f64 652e 6465 7461 696c 732e 6e6f  {node.details.no
+000153d0: 6465 536c 6f74 7d7d 225d 2c0a 2020 2020  deSlot}}"],.    
+000153e0: 2020 2020 2020 2020 2020 2020 226e 6f64              "nod
+000153f0: 6554 7970 6573 223a 205b 2273 6c75 726d  eTypes": ["slurm
+00015400: 6422 5d0a 2020 2020 2020 2020 2020 2020  d"].            
+00015410: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
+00015420: 5d0a 2020 2020 2020 2020 2020 7d2c 0a20  ].          },. 
+00015430: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
+00015440: 2020 2020 2020 2022 6163 7469 6f6e 7322         "actions"
+00015450: 3a20 5b0a 2020 2020 2020 2020 2020 2020  : [.            
+00015460: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
+00015470: 2020 2020 2261 6374 696f 6e22 3a20 2243      "action": "C
+00015480: 5245 4154 455f 574f 524b 4552 5322 2c0a  REATE_WORKERS",.
+00015490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000154a0: 2274 6f74 616c 576f 726b 6572 7322 3a20  "totalWorkers": 
+000154b0: 312c 0a20 2020 2020 2020 2020 2020 2020  1,.             
+000154c0: 2020 2022 6e6f 6465 5479 7065 7322 3a20     "nodeTypes": 
+000154d0: 5b22 736c 7572 6d63 746c 6422 5d0a 2020  ["slurmctld"].  
+000154e0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+000154f0: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
+00015500: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00015510: 5d2c 0a20 2020 2020 2020 2022 4e4f 4445  ],.        "NODE
+00015520: 535f 4144 4445 4422 3a20 5b0a 2020 2020  S_ADDED": [.    
+00015530: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+00015540: 2020 2020 2261 6374 696f 6e73 223a 205b      "actions": [
+00015550: 0a20 2020 2020 2020 2020 2020 2020 207b  .              {
+00015560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015570: 2022 6163 7469 6f6e 223a 2022 5752 4954   "action": "WRIT
+00015580: 455f 4649 4c45 222c 0a20 2020 2020 2020  E_FILE",.       
+00015590: 2020 2020 2020 2020 2022 7061 7468 223a           "path":
+000155a0: 2022 6e6f 6465 732e 6a73 6f6e 222c 0a20   "nodes.json",. 
+000155b0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000155c0: 636f 6e74 656e 7422 3a20 227b 5c6e 2020  content": "{\n  
+000155d0: 5c22 6e6f 6465 735c 223a 205b 5c6e 7b7b  \"nodes\": [\n{{
+000155e0: 2366 696c 7465 7265 644e 6f64 6573 7d7d  #filteredNodes}}
+000155f0: 5c6e 2020 2020 7b5c 6e20 2020 2020 205c  \n    {\n      \
+00015600: 226e 616d 655c 223a 205c 2273 6c75 726d  "name\": \"slurm
+00015610: 647b 7b64 6574 6169 6c73 2e6e 6f64 6553  d{{details.nodeS
+00015620: 6c6f 747d 7d5c 222c 5c6e 2020 2020 2020  lot}}\",\n      
+00015630: 5c22 6970 5c22 3a20 5c22 7b7b 6465 7461  \"ip\": \"{{deta
+00015640: 696c 732e 7072 6976 6174 6549 7041 6464  ils.privateIpAdd
+00015650: 7265 7373 7d7d 5c22 5c6e 2020 2020 7d7b  ress}}\"\n    }{
+00015660: 7b5e 2d6c 6173 747d 7d2c 7b7b 2f2d 6c61  {^-last}},{{/-la
+00015670: 7374 7d7d 5c6e 7b7b 2f66 696c 7465 7265  st}}\n{{/filtere
+00015680: 644e 6f64 6573 7d7d 5c6e 2020 5d5c 6e7d  dNodes}}\n  ]\n}
+00015690: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+000156a0: 2020 2022 6e6f 6465 5479 7065 7322 3a20     "nodeTypes": 
+000156b0: 5b22 736c 7572 6d63 746c 6422 5d0a 2020  ["slurmctld"].  
+000156c0: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+000156d0: 2020 2020 2020 2020 2020 2020 207b 0a20               {. 
+000156e0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000156f0: 6163 7469 6f6e 223a 2022 5255 4e5f 434f  action": "RUN_CO
+00015700: 4d4d 414e 4422 2c0a 2020 2020 2020 2020  MMAND",.        
+00015710: 2020 2020 2020 2020 2270 6174 6822 3a20          "path": 
+00015720: 2261 6464 5f6e 6f64 6573 222c 0a20 2020  "add_nodes",.   
+00015730: 2020 2020 2020 2020 2020 2020 2022 6172               "ar
+00015740: 6775 6d65 6e74 7322 3a20 5b22 6e6f 6465  guments": ["node
+00015750: 732e 6a73 6f6e 225d 2c0a 2020 2020 2020  s.json"],.      
+00015760: 2020 2020 2020 2020 2020 226e 6f64 6554            "nodeT
+00015770: 7970 6573 223a 205b 2273 6c75 726d 6374  ypes": ["slurmct
+00015780: 6c64 225d 0a20 2020 2020 2020 2020 2020  ld"].           
+00015790: 2020 207d 0a20 2020 2020 2020 2020 2020     }.           
+000157a0: 205d 0a20 2020 2020 2020 2020 207d 2c0a   ].          },.
+000157b0: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
+000157c0: 2020 2020 2020 2020 2261 6374 696f 6e73          "actions
+000157d0: 223a 205b 0a20 2020 2020 2020 2020 2020  ": [.           
+000157e0: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
+000157f0: 2020 2020 2022 6163 7469 6f6e 223a 2022       "action": "
+00015800: 5255 4e5f 434f 4d4d 414e 4422 2c0a 2020  RUN_COMMAND",.  
+00015810: 2020 2020 2020 2020 2020 2020 2020 2270                "p
+00015820: 6174 6822 3a20 2273 7461 7274 5f73 696d  ath": "start_sim
+00015830: 706c 655f 736c 7572 6d64 222c 0a20 2020  ple_slurmd",.   
+00015840: 2020 2020 2020 2020 2020 2020 2022 6172               "ar
+00015850: 6775 6d65 6e74 7322 3a20 5b22 7b7b 6e6f  guments": ["{{no
+00015860: 6465 7342 7954 7970 652e 736c 7572 6d63  desByType.slurmc
+00015870: 746c 642e 302e 6465 7461 696c 732e 7072  tld.0.details.pr
+00015880: 6976 6174 6549 7041 6464 7265 7373 7d7d  ivateIpAddress}}
+00015890: 222c 2022 7b7b 6e6f 6465 2e64 6574 6169  ", "{{node.detai
+000158a0: 6c73 2e6e 6f64 6553 6c6f 747d 7d22 5d2c  ls.nodeSlot}}"],
+000158b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000158c0: 2022 6e6f 6465 4964 4669 6c74 6572 223a   "nodeIdFilter":
+000158d0: 2022 4556 454e 5422 2c0a 2020 2020 2020   "EVENT",.      
+000158e0: 2020 2020 2020 2020 2020 226e 6f64 6554            "nodeT
+000158f0: 7970 6573 223a 205b 2273 6c75 726d 6422  ypes": ["slurmd"
+00015900: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00015910: 7d0a 2020 2020 2020 2020 2020 2020 5d0a  }.            ].
+00015920: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+00015930: 2020 2020 5d0a 2020 2020 2020 7d0a 2020      ].      }.  
+00015940: 2020 7d2c 0a20 2020 2022 776f 726b 6572    },.    "worker
+00015950: 5461 6722 3a20 2270 7965 782d 736c 7572  Tag": "pyex-slur
+00015960: 6d2d 636c 7573 7465 7222 0a20 207d 0a7d  m-cluster".  }.}
+00015970: 0a60 6060 0a0a 2323 2320 544f 4d4c 2050  .```..### TOML P
+00015980: 726f 7065 7274 6965 7320 496e 6865 7269  roperties Inheri
+00015990: 7465 6420 6279 2057 6f72 6b65 7220 506f  ted by Worker Po
+000159a0: 6f6c 204a 534f 4e20 5370 6563 6966 6963  ol JSON Specific
+000159b0: 6174 696f 6e73 0a0a 5768 656e 2061 204a  ations..When a J
+000159c0: 534f 4e20 576f 726b 6572 2050 6f6f 6c20  SON Worker Pool 
+000159d0: 7370 6563 6966 6963 6174 696f 6e20 6973  specification is
+000159e0: 2075 7365 642c 2074 6865 2066 6f6c 6c6f   used, the follo
+000159f0: 7769 6e67 2070 726f 7065 7274 6965 7320  wing properties 
+00015a00: 6672 6f6d 2074 6865 2060 636f 6e66 6967  from the `config
+00015a10: 2e74 6f6d 6c60 2066 696c 6520 7769 6c6c  .toml` file will
+00015a20: 2062 6520 696e 6865 7269 7465 6420 6966   be inherited if
+00015a30: 2074 6865 2076 616c 7565 2069 7320 6162   the value is ab
+00015a40: 7365 6e74 2069 6e20 7468 6520 4a53 4f4e  sent in the JSON
+00015a50: 2066 696c 653a 0a0a 2a2a 5072 6f70 6572   file:..**Proper
+00015a60: 7469 6573 2049 6e68 6572 6974 6564 2077  ties Inherited w
+00015a70: 6974 6869 6e20 7468 6520 6072 6571 7569  ithin the `requi
+00015a80: 7265 6d65 6e74 5465 6d70 6c61 7465 5573  rementTemplateUs
+00015a90: 6167 6560 2070 726f 7065 7274 792a 2a0a  age` property**.
+00015aa0: 0a2d 2060 696d 6167 6573 4964 600a 2d20  .- `imagesId`.- 
+00015ab0: 6069 6e73 7461 6e63 6554 6167 7360 0a2d  `instanceTags`.-
+00015ac0: 2060 7265 7175 6972 656d 656e 744e 616d   `requirementNam
+00015ad0: 6560 3a20 6465 7269 7665 6420 6672 6f6d  e`: derived from
+00015ae0: 2074 6865 2060 6e61 6d65 6020 7072 6f70   the `name` prop
+00015af0: 6572 7479 2069 6e20 7468 6520 6054 4f4d  erty in the `TOM
+00015b00: 4c60 2063 6f6e 6669 6775 7261 7469 6f6e  L` configuration
+00015b10: 2e20 2854 6865 206e 616d 6520 7769 6c6c  . (The name will
+00015b20: 2062 6520 6765 6e65 7261 7465 6420 6175   be generated au
+00015b30: 746f 6d61 7469 6361 6c6c 7920 6966 206e  tomatically if n
+00015b40: 6f74 2073 7570 706c 6965 6420 696e 2065  ot supplied in e
+00015b50: 6974 6865 7220 7468 6520 544f 4d4c 2066  ither the TOML f
+00015b60: 696c 6520 6f72 2074 6865 204a 534f 4e20  ile or the JSON 
+00015b70: 7370 6563 6966 6963 6174 696f 6e2e 290a  specification.).
+00015b80: 2d20 6072 6571 7569 7265 6d65 6e74 4e61  - `requirementNa
+00015b90: 6d65 7370 6163 6560 3a20 6465 7269 7665  mespace`: derive
+00015ba0: 6420 6672 6f6d 2074 6865 2060 6e61 6d65  d from the `name
+00015bb0: 7370 6163 6560 2070 726f 7065 7274 7920  space` property 
+00015bc0: 696e 2074 6865 2060 544f 4d4c 6020 636f  in the `TOML` co
+00015bd0: 6e66 6967 7572 6174 696f 6e0a 2d20 6072  nfiguration.- `r
+00015be0: 6571 7569 7265 6d65 6e74 5461 6760 3a20  equirementTag`: 
+00015bf0: 3a20 6465 7269 7665 6420 6672 6f6d 2074  : derived from t
+00015c00: 6865 2060 7461 6760 2070 726f 7065 7274  he `tag` propert
+00015c10: 7920 696e 2074 6865 2060 544f 4d4c 6020  y in the `TOML` 
+00015c20: 636f 6e66 6967 7572 6174 696f 6e0a 2d20  configuration.- 
+00015c30: 6074 6172 6765 7449 6e73 7461 6e63 6543  `targetInstanceC
+00015c40: 6f75 6e74 600a 2d20 6074 656d 706c 6174  ount`.- `templat
+00015c50: 6549 6460 0a2d 2060 7573 6572 4461 7461  eId`.- `userData
+00015c60: 600a 2d20 6075 7365 7244 6174 6146 696c  `.- `userDataFil
+00015c70: 6560 0a2d 2060 7573 6572 4461 7461 4669  e`.- `userDataFi
+00015c80: 6c65 7360 0a0a 2a2a 5072 6f70 6572 7469  les`..**Properti
+00015c90: 6573 2049 6e68 6572 6974 6564 2077 6974  es Inherited wit
+00015ca0: 6869 6e20 7468 6520 6070 726f 7669 7369  hin the `provisi
+00015cb0: 6f6e 6564 5072 6f70 6572 7469 6573 6020  onedProperties` 
+00015cc0: 5072 6f70 6572 7479 2a2a 0a0a 2d20 6069  Property**..- `i
+00015cd0: 646c 654e 6f64 6553 6875 7464 6f77 6e45  dleNodeShutdownE
+00015ce0: 6e61 626c 6564 600a 2d20 6069 646c 654e  nabled`.- `idleN
+00015cf0: 6f64 6553 6875 7464 6f77 6e54 696d 656f  odeShutdownTimeo
+00015d00: 7574 600a 2d20 6069 646c 6550 6f6f 6c53  ut`.- `idlePoolS
+00015d10: 6875 7464 6f77 6e45 6e61 626c 6564 600a  hutdownEnabled`.
+00015d20: 2d20 6069 646c 6550 6f6f 6c53 6875 7464  - `idlePoolShutd
+00015d30: 6f77 6e54 696d 656f 7574 600a 2d20 606e  ownTimeout`.- `n
+00015d40: 6f64 6542 6f6f 7454 696d 656f 7574 600a  odeBootTimeout`.
+00015d50: 2d20 6077 6f72 6b65 7254 6167 600a 0a23  - `workerTag`..#
+00015d60: 2320 5661 7269 6162 6c65 2053 7562 7374  # Variable Subst
+00015d70: 6974 7574 696f 6e73 2069 6e20 576f 726b  itutions in Work
+00015d80: 6572 2050 6f6f 6c20 5072 6f70 6572 7469  er Pool Properti
+00015d90: 6573 0a0a 5661 7269 6162 6c65 2073 7562  es..Variable sub
+00015da0: 7374 6974 7574 696f 6e73 2063 616e 2062  stitutions can b
+00015db0: 6520 7573 6564 2077 6974 6869 6e20 616e  e used within an
+00015dc0: 7920 7072 6f70 6572 7479 2076 616c 7565  y property value
+00015dd0: 2069 6e20 544f 4d4c 2063 6f6e 6669 6775   in TOML configu
+00015de0: 7261 7469 6f6e 2066 696c 6573 206f 7220  ration files or 
+00015df0: 576f 726b 6572 2050 6f6f 6c20 4a53 4f4e  Worker Pool JSON
+00015e00: 2066 696c 6573 2e20 5365 6520 7468 6520   files. See the 
+00015e10: 6465 7363 7269 7074 696f 6e20 5b61 626f  description [abo
+00015e20: 7665 5d28 2376 6172 6961 626c 652d 7375  ve](#variable-su
+00015e30: 6273 7469 7475 7469 6f6e 7329 2066 6f72  bstitutions) for
+00015e40: 206d 6f72 6520 6465 7461 696c 7320 6f6e   more details on
+00015e50: 2076 6172 6961 626c 6520 7375 6273 7469   variable substi
+00015e60: 7475 7469 6f6e 732e 2054 6869 7320 6973  tutions. This is
+00015e70: 2061 2070 6f77 6572 6675 6c20 6665 6174   a powerful feat
+00015e80: 7572 6520 7468 6174 2061 6c6c 6f77 7320  ure that allows 
+00015e90: 576f 726b 6572 2050 6f6f 6c73 2074 6f20  Worker Pools to 
+00015ea0: 6265 2070 6172 616d 6574 6572 6973 6564  be parameterised
+00015eb0: 2062 7920 7375 7070 6c79 696e 6720 7661   by supplying va
+00015ec0: 6c75 6573 206f 6e20 7468 6520 636f 6d6d  lues on the comm
+00015ed0: 616e 6420 6c69 6e65 2c20 7669 6120 656e  and line, via en
+00015ee0: 7669 726f 6e6d 656e 7420 7661 7269 6162  vironment variab
+00015ef0: 6c65 732c 206f 7220 7669 6120 7468 6520  les, or via the 
+00015f00: 544f 4d4c 2066 696c 652e 0a0a 416e 2069  TOML file...An i
+00015f10: 6d70 6f72 7461 6e74 2064 6973 7469 6e63  mportant distinc
+00015f20: 7469 6f6e 202a 2a6f 6e6c 792a 2a20 7768  tion **only** wh
+00015f30: 656e 2075 7369 6e67 2076 6172 6961 626c  en using variabl
+00015f40: 6520 7375 6273 7469 7475 7469 6f6e 7320  e substitutions 
+00015f50: 7769 7468 696e 2057 6f72 6b65 7220 506f  within Worker Po
+00015f60: 6f6c 204a 534f 4e20 646f 6375 6d65 6e74  ol JSON document
+00015f70: 7320 6973 2074 6861 7420 6561 6368 2064  s is that each d
+00015f80: 6972 6563 7469 7665 202a 2a6d 7573 7420  irective **must 
+00015f90: 6265 2070 7265 6365 6465 6420 6279 2061  be preceded by a
+00015fa0: 2060 5f5f 6020 2864 6f75 626c 6520 756e   `__` (double un
+00015fb0: 6465 7273 636f 7265 292a 2a20 746f 2064  derscore)** to d
+00015fc0: 6973 616d 6269 6775 6174 6520 6974 2066  isambiguate it f
+00015fd0: 726f 6d20 7661 7269 6162 6c65 2073 7562  rom variable sub
+00015fe0: 7374 6974 7574 696f 6e73 2074 6861 7420  stitutions that 
+00015ff0: 6172 6520 746f 2062 6520 7061 7373 6564  are to be passed
+00016000: 2064 6972 6563 746c 7920 746f 2074 6865   directly to the
+00016010: 2041 5049 2e20 466f 7220 6578 616d 706c   API. For exampl
+00016020: 652c 2075 7365 3a20 605f 5f7b 7b75 7365  e, use: `__{{use
+00016030: 726e 616d 657d 7d60 2074 6f20 6170 706c  rname}}` to appl
+00016040: 7920 6120 7375 6273 7469 7475 7469 6f6e  y a substitution
+00016050: 2066 6f72 2074 6865 2060 7573 6572 6e61   for the `userna
+00016060: 6d65 6020 6465 6661 756c 7420 7375 6273  me` default subs
+00016070: 7469 7475 7469 6f6e 2e0a 0a23 2320 4472  titution...## Dr
+00016080: 792d 5275 6e6e 696e 6720 576f 726b 6572  y-Running Worker
+00016090: 2050 6f6f 6c20 5072 6f76 6973 696f 6e69   Pool Provisioni
+000160a0: 6e67 0a0a 546f 2065 7861 6d69 6e65 2074  ng..To examine t
+000160b0: 6865 204a 534f 4e20 7468 6174 2077 696c  he JSON that wil
+000160c0: 6c20 6163 7475 616c 6c79 2062 6520 7365  l actually be se
+000160d0: 6e74 2074 6f20 7468 6520 5965 6c6c 6f77  nt to the Yellow
+000160e0: 446f 6720 4150 4920 6166 7465 7220 616c  Dog API after al
+000160f0: 6c20 7072 6f63 6573 7369 6e67 2c20 7573  l processing, us
+00016100: 6520 7468 6520 602d 2d64 7279 2d72 756e  e the `--dry-run
+00016110: 6020 636f 6d6d 616e 6420 6c69 6e65 206f  ` command line o
+00016120: 7074 696f 6e20 7768 656e 2072 756e 6e69  ption when runni
+00016130: 6e67 2060 7964 2d70 726f 7669 7369 6f6e  ng `yd-provision
+00016140: 602e 2054 6869 7320 7769 6c6c 2070 7269  `. This will pri
+00016150: 6e74 2074 6865 204a 534f 4e20 7370 6563  nt the JSON spec
+00016160: 6966 6963 6174 696f 6e20 666f 7220 7468  ification for th
+00016170: 6520 576f 726b 6572 2050 6f6f 6c2e 204e  e Worker Pool. N
+00016180: 6f74 6869 6e67 2077 696c 6c20 6265 2073  othing will be s
+00016190: 7562 6d69 7474 6564 2074 6f20 7468 6520  ubmitted to the 
+000161a0: 706c 6174 666f 726d 2e0a 0a54 6865 2067  platform...The g
+000161b0: 656e 6572 6174 6564 204a 534f 4e20 6973  enerated JSON is
+000161c0: 2070 726f 6475 6365 6420 6166 7465 7220   produced after 
+000161d0: 616c 6c20 7072 6f63 6573 7369 6e67 2028  all processing (
+000161e0: 696e 636f 7270 6f72 6174 696e 6720 6063  incorporating `c
+000161f0: 6f6e 6669 672e 746f 6d6c 6020 7072 6f70  onfig.toml` prop
+00016200: 6572 7469 6573 2c20 7661 7269 6162 6c65  erties, variable
+00016210: 2073 7562 7374 6974 7574 696f 6e73 2c20   substitutions, 
+00016220: 6574 632e 2920 6861 7320 6265 656e 2063  etc.) has been c
+00016230: 6f6e 636c 7564 6564 2c20 736f 2074 6865  oncluded, so the
+00016240: 2064 7279 2d72 756e 2069 7320 7573 6566   dry-run is usef
+00016250: 756c 2066 6f72 2069 6e73 7065 6374 696e  ul for inspectin
+00016260: 6720 7468 6520 7265 7375 6c74 7320 6f66  g the results of
+00016270: 2061 6c6c 2074 6865 2070 726f 6365 7373   all the process
+00016280: 696e 6720 7468 6174 2773 2062 6565 6e20  ing that's been 
+00016290: 7065 7266 6f72 6d65 642e 0a0a 546f 2073  performed...To s
+000162a0: 7570 7072 6573 7320 616c 6c20 6f75 7470  uppress all outp
+000162b0: 7574 2065 7863 6570 7420 666f 7220 7468  ut except for th
+000162c0: 6520 4a53 4f4e 2069 7473 656c 662c 2075  e JSON itself, u
+000162d0: 7365 2074 6865 2060 2d2d 7175 6965 7460  se the `--quiet`
+000162e0: 2028 602d 7160 2920 636f 6d6d 616e 6420   (`-q`) command 
+000162f0: 6c69 6e65 206f 7074 696f 6e2e 0a0a 5468  line option...Th
+00016300: 6520 4a53 4f4e 2064 7279 2d72 756e 206f  e JSON dry-run o
+00016310: 7574 7075 7420 636f 756c 6420 6974 7365  utput could itse
+00016320: 6c66 2062 6520 7573 6564 2062 7920 6079  lf be used by `y
+00016330: 642d 7072 6f76 6973 696f 6e60 2c20 6966  d-provision`, if
+00016340: 2063 6170 7475 7265 6420 696e 2061 2066   captured in a f
+00016350: 696c 652c 2065 2e67 2e3a 0a0a 6060 6073  ile, e.g.:..```s
+00016360: 6865 6c6c 0a79 642d 7072 6f76 6973 696f  hell.yd-provisio
+00016370: 6e20 2d2d 6472 792d 7275 6e20 2d71 203e  n --dry-run -q >
+00016380: 206d 795f 776f 726b 6572 5f70 6f6f 6c2e   my_worker_pool.
+00016390: 6a73 6f6e 0a79 642d 7072 6f76 6973 696f  json.yd-provisio
+000163a0: 6e20 2d70 206d 795f 776f 726b 6572 5f70  n -p my_worker_p
+000163b0: 6f6f 6c2e 6a73 6f6e 0a60 6060 0a0a 2320  ool.json.```..# 
+000163c0: 4a73 6f6e 6e65 7420 5375 7070 6f72 740a  Jsonnet Support.
+000163d0: 0a49 6e20 616c 6c20 6369 7263 756d 7374  .In all circumst
+000163e0: 616e 6365 7320 7768 6572 6520 4a53 4f4e  ances where JSON
+000163f0: 2066 696c 6573 2061 7265 2075 7365 6420   files are used 
+00016400: 6279 2074 6865 2050 7974 686f 6e20 4578  by the Python Ex
+00016410: 616d 706c 6573 2073 6372 6970 7473 2c20  amples scripts, 
+00016420: 202a 2a5b 4a73 6f6e 6e65 745d 2868 7474   **[Jsonnet](htt
+00016430: 7073 3a2f 2f6a 736f 6e6e 6574 2e6f 7267  ps://jsonnet.org
+00016440: 292a 2a20 6669 6c65 7320 6361 6e20 6265  )** files can be
+00016450: 2075 7365 6420 696e 7374 6561 642e 2054   used instead. T
+00016460: 6869 7320 616c 6c6f 7773 2074 6865 2075  his allows the u
+00016470: 7365 206f 6620 4a73 6f6e 6e65 7427 7320  se of Jsonnet's 
+00016480: 706f 7765 7266 756c 204a 534f 4e20 6578  powerful JSON ex
+00016490: 7465 6e73 696f 6e73 2c20 696e 636c 7564  tensions, includ
+000164a0: 696e 6720 636f 6d6d 656e 7473 2c20 7661  ing comments, va
+000164b0: 7269 6162 6c65 732c 2066 756e 6374 696f  riables, functio
+000164c0: 6e73 2c20 6574 632e 0a0a 4120 7369 6d70  ns, etc...A simp
+000164d0: 6c65 2075 7361 6765 2065 7861 6d70 6c65  le usage example
+000164e0: 206d 6967 6874 2062 653a 0a0a 6060 6073   might be:..```s
+000164f0: 6865 6c6c 0a79 642d 7375 626d 6974 202d  hell.yd-submit -
+00016500: 2d77 6f72 6b2d 7265 7175 6972 656d 656e  -work-requiremen
+00016510: 7420 6d79 5f77 6f72 6b5f 7265 712e 6a73  t my_work_req.js
+00016520: 6f6e 6e65 740a 6060 600a 0a54 6865 2075  onnet.```..The u
+00016530: 7365 206f 6620 7468 6520 6669 6c65 6e61  se of the filena
+00016540: 6d65 2065 7874 656e 7369 6f6e 2060 2e6a  me extension `.j
+00016550: 736f 6e6e 6574 6020 7769 6c6c 2069 6e76  sonnet` will inv
+00016560: 6f6b 6520 4a73 6f6e 6e65 7420 6576 616c  oke Jsonnet eval
+00016570: 7561 7469 6f6e 2e20 284e 6f74 6520 7468  uation. (Note th
+00016580: 6174 2061 2074 656d 706f 7261 7279 204a  at a temporary J
+00016590: 534f 4e20 6669 6c65 2069 7320 6372 6561  SON file is crea
+000165a0: 7465 6420 6173 2070 6172 7420 6f66 204a  ted as part of J
+000165b0: 736f 6e6e 6574 2070 726f 6365 7373 696e  sonnet processin
+000165c0: 672c 2077 6869 6368 2079 6f75 206d 6179  g, which you may
+000165d0: 2073 6565 2072 6566 6572 7265 6420 746f   see referred to
+000165e0: 2069 6e20 6572 726f 7220 6d65 7373 6167   in error messag
+000165f0: 6573 3a20 7468 6973 2066 696c 6520 7769  es: this file wi
+00016600: 6c6c 2068 6176 6520 6265 656e 2064 656c  ll have been del
+00016610: 6574 6564 2062 6566 6f72 6520 7468 6520  eted before the 
+00016620: 7363 7269 7074 2073 746f 7073 2e29 0a0a  script stops.)..
+00016630: 2323 204a 736f 6e6e 6574 2049 6e73 7461  ## Jsonnet Insta
+00016640: 6c6c 6174 696f 6e0a 0a4a 736f 6e6e 6574  llation..Jsonnet
+00016650: 2069 7320 2a2a 6e6f 742a 2a20 696e 7374   is **not** inst
+00016660: 616c 6c65 6420 6279 2064 6566 6175 6c74  alled by default
+00016670: 2077 6865 6e20 6079 656c 6c6f 7764 6f67   when `yellowdog
+00016680: 2d70 7974 686f 6e2d 6578 616d 706c 6573  -python-examples
+00016690: 6020 6973 2069 6e73 7461 6c6c 6564 2c20  ` is installed, 
+000166a0: 6265 6361 7573 6520 7468 6520 7061 636b  because the pack
+000166b0: 6167 6520 6861 7320 6269 6e61 7279 2063  age has binary c
+000166c0: 6f6d 706f 6e65 6e74 7320 7768 6963 6820  omponents which 
+000166d0: 6172 6520 6e6f 7420 6176 6169 6c61 626c  are not availabl
+000166e0: 6520 6f6e 2050 7950 4920 666f 7220 616c  e on PyPI for al
+000166f0: 6c20 706c 6174 666f 726d 732e 2049 6620  l platforms. If 
+00016700: 796f 7520 7472 7920 746f 2075 7365 2061  you try to use a
+00016710: 204a 736f 6e6e 6574 2066 696c 6520 696e   Jsonnet file in
+00016720: 2074 6865 2061 6273 656e 6365 206f 6620   the absence of 
+00016730: 4a73 6f6e 6e65 742c 2074 6865 2073 6372  Jsonnet, the scr
+00016740: 6970 7473 2077 696c 6c20 7072 696e 7420  ipts will print 
+00016750: 616e 2065 7272 6f72 206d 6573 7361 6765  an error message
+00016760: 2c20 616e 6420 7375 6767 6573 7420 616e  , and suggest an
+00016770: 2069 6e73 7461 6c6c 6174 696f 6e20 6d65   installation me
+00016780: 6368 616e 6973 6d2e 0a0a 546f 2069 6e73  chanism...To ins
+00016790: 7461 6c6c 204a 736f 6e6e 6574 2061 7420  tall Jsonnet at 
+000167a0: 7468 6520 7361 6d65 2074 696d 6520 6173  the same time as
+000167b0: 2069 6e73 7461 6c6c 696e 6720 6f72 2075   installing or u
+000167c0: 7064 6174 696e 6720 7468 6520 5079 7468  pdating the Pyth
+000167d0: 6f6e 2045 7861 6d70 6c65 7320 7363 7269  on Examples scri
+000167e0: 7074 732c 206d 6f64 6966 7920 7468 6520  pts, modify the 
+000167f0: 696e 7374 616c 6c61 7469 6f6e 2061 7320  installation as 
+00016800: 666f 6c6c 6f77 7320 746f 2069 6e63 6c75  follows to inclu
+00016810: 6465 2074 6865 2060 6a73 6f6e 6e65 7460  de the `jsonnet`
+00016820: 206f 7074 696f 6e3a 0a0a 6060 600a 7069   option:..```.pi
+00016830: 7020 696e 7374 616c 6c20 2d55 2022 7965  p install -U "ye
+00016840: 6c6c 6f77 646f 672d 7079 7468 6f6e 2d65  llowdog-python-e
+00016850: 7861 6d70 6c65 735b 6a73 6f6e 6e65 745d  xamples[jsonnet]
+00016860: 220a 6060 600a 0a54 6f20 696e 7374 616c  ".```..To instal
+00016870: 6c20 4a73 6f6e 6e65 7420 7365 7061 7261  l Jsonnet separa
+00016880: 7465 6c79 2066 726f 6d20 6079 656c 6c6f  tely from `yello
+00016890: 7764 6f67 2d70 7974 686f 6e2d 6578 616d  wdog-python-exam
+000168a0: 706c 6573 602c 2074 7279 3a0a 0a60 6060  ples`, try:..```
+000168b0: 7368 656c 6c0a 7069 7020 696e 7374 616c  shell.pip instal
+000168c0: 6c20 2d55 206a 736f 6e6e 6574 0a60 6060  l -U jsonnet.```
+000168d0: 0a0a 4966 2074 6869 7320 6661 696c 732c  ..If this fails,
+000168e0: 2074 7279 3a0a 0a60 6060 7368 656c 6c0a   try:..```shell.
+000168f0: 7069 7020 696e 7374 616c 6c20 2d55 206a  pip install -U j
+00016900: 736f 6e6e 6574 2d62 696e 6172 790a 6060  sonnet-binary.``
+00016910: 600a 0a49 6620 626f 7468 206f 6620 7468  `..If both of th
+00016920: 6573 6520 6d65 7468 6f64 7320 6661 696c  ese methods fail
+00016930: 2c20 796f 7527 6c6c 206e 6565 6420 746f  , you'll need to
+00016940: 2065 6e73 7572 6520 7468 6174 2074 6865   ensure that the
+00016950: 2070 6c61 7466 6f72 6d20 6f6e 2077 6869   platform on whi
+00016960: 6368 2079 6f75 2772 6520 7275 6e6e 696e  ch you're runnin
+00016970: 6720 6861 7320 7468 6520 7265 7175 6972  g has the requir
+00016980: 6564 2062 7569 6c64 2074 6f6f 6c73 2061  ed build tools a
+00016990: 7661 696c 6162 6c65 2c20 736f 2074 6861  vailable, so tha
+000169a0: 7420 7468 6520 4a73 6f6e 6e65 7420 6269  t the Jsonnet bi
+000169b0: 6e61 7279 2063 6f6d 706f 6e65 6e74 7320  nary components 
+000169c0: 6361 6e20 6265 2062 7569 6c74 206c 6f63  can be built loc
+000169d0: 616c 6c79 2e20 5468 6520 7265 7175 6972  ally. The requir
+000169e0: 6564 2062 7569 6c64 2070 6163 6b61 6765  ed build package
+000169f0: 7320 7661 7279 2062 7920 706c 6174 666f  s vary by platfo
+00016a00: 726d 2062 7574 2075 7375 616c 6c79 2069  rm but usually i
+00016a10: 6e63 6c75 6465 2067 656e 6572 616c 2064  nclude general d
+00016a20: 6576 656c 6f70 6d65 6e74 2074 6f6f 6c73  evelopment tools
+00016a30: 2069 6e63 6c75 6469 6e67 2061 2043 2b2b   including a C++
+00016a40: 2063 6f6d 7069 6c65 722c 2061 6e64 2050   compiler, and P
+00016a50: 7974 686f 6e20 6465 7665 6c6f 706d 656e  ython developmen
+00016a60: 7420 746f 6f6c 7320 696e 636c 7564 696e  t tools includin
+00016a70: 6720 7468 6520 5079 7468 6f6e 2068 6561  g the Python hea
+00016a80: 6465 7273 2e0a 0a50 6c65 6173 6520 6765  ders...Please ge
+00016a90: 7420 696e 2074 6f75 6368 2077 6974 6820  t in touch with 
+00016aa0: 5965 6c6c 6f77 446f 6720 6966 2079 6f75  YellowDog if you
+00016ab0: 2067 6574 2073 7475 636b 2e0a 0a23 2320   get stuck...## 
+00016ac0: 5661 7269 6162 6c65 2053 7562 7374 6974  Variable Substit
+00016ad0: 7574 696f 6e73 2069 6e20 4a73 6f6e 6e65  utions in Jsonne
+00016ae0: 7420 4669 6c65 730a 0a54 6865 2073 6372  t Files..The scr
+00016af0: 6970 7473 2070 726f 7669 6465 2066 756c  ipts provide ful
+00016b00: 6c20 7375 7070 6f72 7420 666f 7220 7661  l support for va
+00016b10: 7269 6162 6c65 2073 7562 7374 6974 7574  riable substitut
+00016b20: 696f 6e73 2069 6e20 4a73 6f6e 6e65 7420  ions in Jsonnet 
+00016b30: 6669 6c65 732c 2075 7369 6e67 2074 6865  files, using the
+00016b40: 2073 616d 6520 7275 6c65 7320 6173 2066   same rules as f
+00016b50: 6f72 2074 6865 204a 534f 4e20 7370 6563  or the JSON spec
+00016b60: 6966 6963 6174 696f 6e73 2e20 5265 6d65  ifications. Reme
+00016b70: 6d62 6572 2074 6861 7420 666f 7220 2a2a  mber that for **
+00016b80: 576f 726b 6572 2050 6f6f 6c2a 2a20 7370  Worker Pool** sp
+00016b90: 6563 6966 6963 6174 696f 6e73 2c20 7661  ecifications, va
+00016ba0: 7269 6162 6c65 2073 7562 7374 6974 7574  riable substitut
+00016bb0: 696f 6e73 206d 7573 7420 6265 2070 7265  ions must be pre
+00016bc0: 6669 7865 6420 6279 2060 5f5f 602c 2065  fixed by `__`, e
+00016bd0: 2e67 2e20 6022 5f5f 7b7b 7573 6572 6e61  .g. `"__{{userna
+00016be0: 6d65 7d7d 7d22 602e 0a0a 5661 7269 6162  me}}}"`...Variab
+00016bf0: 6c65 2073 7562 7374 6974 7574 696f 6e20  le substitution 
+00016c00: 6973 2070 6572 666f 726d 6564 2062 6566  is performed bef
+00016c10: 6f72 6520 4a73 6f6e 6e65 7420 6578 7061  ore Jsonnet expa
+00016c20: 6e73 696f 6e20 696e 746f 204a 534f 4e2c  nsion into JSON,
+00016c30: 2061 6e64 2061 6761 696e 2061 6674 6572   and again after
+00016c40: 2074 6865 2065 7870 616e 7369 6f6e 2e0a   the expansion..
+00016c50: 0a23 2320 4368 6563 6b69 6e67 204a 736f  .## Checking Jso
+00016c60: 6e6e 6574 2050 726f 6365 7373 696e 670a  nnet Processing.
+00016c70: 0a54 6865 7265 2061 7265 2074 6872 6565  .There are three
+00016c80: 2070 6f73 7369 6269 6c69 7469 6573 2066   possibilities f
+00016c90: 6f72 2076 6572 6966 7969 6e67 2074 6861  or verifying tha
+00016ca0: 7420 6120 4a73 6f6e 6e65 7420 7370 6563  t a Jsonnet spec
+00016cb0: 6966 6963 6174 696f 6e20 6973 2064 6f69  ification is doi
+00016cc0: 6e67 2077 6861 7420 6973 2069 6e74 656e  ng what is inten
+00016cd0: 6465 643a 0a0a 312e 2054 6f20 696e 7370  ded:..1. To insp
+00016ce0: 6563 7420 7468 6520 6261 7369 6320 636f  ect the basic co
+00016cf0: 6e76 6572 7369 6f6e 206f 6620 4a73 6f6e  nversion of Json
+00016d00: 6e65 7420 696e 746f 204a 534f 4e2c 2077  net into JSON, w
+00016d10: 6974 686f 7574 2061 6e79 2061 6464 6974  ithout any addit
+00016d20: 696f 6e61 6c20 7072 6f63 6573 7369 6e67  ional processing
+00016d30: 2062 7920 7468 6520 5079 7468 6f6e 2045   by the Python E
+00016d40: 7861 6d70 6c65 7320 7363 7269 7074 732c  xamples scripts,
+00016d50: 2074 6865 2060 7964 2d6a 736f 6e6e 6574   the `yd-jsonnet
+00016d60: 326a 736f 6e60 2063 6f6d 6d61 6e64 2063  2json` command c
+00016d70: 616e 2062 6520 7573 6564 2e20 5468 6973  an be used. This
+00016d80: 2074 616b 6573 2061 2073 696e 676c 6520   takes a single 
+00016d90: 636f 6d6d 616e 6420 6c69 6e65 2061 7267  command line arg
+00016da0: 756d 656e 7420 7768 6963 6820 6973 2074  ument which is t
+00016db0: 6865 206e 616d 6520 6f66 2074 6865 206a  he name of the j
+00016dc0: 736f 6e6e 6574 2066 696c 6520 746f 2062  sonnet file to b
+00016dd0: 6520 7072 6f63 6573 7365 643a 0a0a 6060  e processed:..``
+00016de0: 6073 6865 6c6c 0a79 642d 6a73 6f6e 6e65  `shell.yd-jsonne
+00016df0: 7432 6a73 6f6e 206d 795f 6669 6c65 2e6a  t2json my_file.j
+00016e00: 736f 6e6e 6574 0a60 6060 0a0a 0a32 2e20  sonnet.```...2. 
+00016e10: 5468 6520 606a 736f 6e6e 6574 2d64 7279  The `jsonnet-dry
+00016e20: 2d72 756e 6020 2860 2d4a 6029 206f 7074  -run` (`-J`) opt
+00016e30: 696f 6e20 6f66 2074 6865 2060 7964 2d73  ion of the `yd-s
+00016e40: 7562 6d69 7460 2c20 6079 642d 7072 6f76  ubmit`, `yd-prov
+00016e50: 6973 696f 6e60 2061 6e64 2060 7964 2d69  ision` and `yd-i
+00016e60: 6e73 7461 6e74 6961 7465 6020 636f 6d6d  nstantiate` comm
+00016e70: 616e 6473 2077 696c 6c20 6765 6e65 7261  ands will genera
+00016e80: 7465 204a 534f 4e20 6f75 7470 7574 2072  te JSON output r
+00016e90: 6570 7265 7365 6e74 696e 6720 7468 6520  epresenting the 
+00016ea0: 4a73 6f6e 6e65 7420 746f 204a 534f 4e20  Jsonnet to JSON 
+00016eb0: 7072 6f63 6573 7369 6e67 206f 6e6c 792c  processing only,
+00016ec0: 2069 6e63 6c75 6469 6e67 2061 7070 6c69   including appli
+00016ed0: 6361 626c 6520 7661 7269 6162 6c65 2073  cable variable s
+00016ee0: 7562 7374 6974 7574 696f 6e73 2c20 6275  ubstitutions, bu
+00016ef0: 7420 6265 666f 7265 2066 756c 6c20 7072  t before full pr
+00016f00: 6f70 6572 7479 2065 7870 616e 7369 6f6e  operty expansion
+00016f10: 2069 6e74 6f20 7468 6520 4a53 4f4e 2074   into the JSON t
+00016f20: 6861 7420 7769 6c6c 2062 6520 7375 626d  hat will be subm
+00016f30: 6974 7465 6420 746f 2074 6865 2050 6c61  itted to the Pla
+00016f40: 7466 6f72 6d2e 0a0a 0a33 2e20 5468 6520  tform....3. The 
+00016f50: 6064 7279 2d72 756e 6020 2860 2d44 6029  `dry-run` (`-D`)
+00016f60: 206f 7074 696f 6e20 7769 6c6c 2067 656e   option will gen
+00016f70: 6572 6174 6520 4a53 4f4e 206f 7574 7075  erate JSON outpu
+00016f80: 7420 7265 7072 6573 656e 7469 6e67 2074  t representing t
+00016f90: 6865 2066 756c 6c20 7072 6f63 6573 7369  he full processi
+00016fa0: 6e67 206f 6620 7468 6520 4a73 6f6e 6e65  ng of the Jsonne
+00016fb0: 7420 6669 6c65 2069 6e74 6f20 7768 6174  t file into what
+00016fc0: 2077 696c 6c20 6265 2073 7562 6d69 7474   will be submitt
+00016fd0: 6564 2074 6f20 7468 6520 4150 492e 2054  ed to the API. T
+00016fe0: 6869 7320 616c 6c6f 7773 2069 6e73 7065  his allows inspe
+00016ff0: 6374 696f 6e20 746f 2063 6865 636b 2074  ction to check t
+00017000: 6861 7420 7468 6520 6f75 7470 7574 206d  hat the output m
+00017010: 6174 6368 6573 2065 7870 6563 7461 7469  atches expectati
+00017020: 6f6e 732c 2070 7269 6f72 2074 6f20 7375  ons, prior to su
+00017030: 626d 6974 7469 6e67 2074 6f20 7468 6520  bmitting to the 
+00017040: 506c 6174 666f 726d 2e0a 0a23 2320 4a73  Platform...## Js
+00017050: 6f6e 6e65 7420 4578 616d 706c 650a 0a48  onnet Example..H
+00017060: 6572 6527 7320 616e 2065 7861 6d70 6c65  ere's an example
+00017070: 206f 6620 6120 4a73 6f6e 6e65 7420 6669   of a Jsonnet fi
+00017080: 6c65 2074 6861 7420 6765 6e65 7261 7465  le that generate
+00017090: 7320 6120 576f 726b 2052 6571 7569 7265  s a Work Require
+000170a0: 6d65 6e74 2077 6974 6820 666f 7572 2054  ment with four T
+000170b0: 6173 6b73 3a0a 0a60 6060 6a73 6f6e 6e65  asks:..```jsonne
+000170c0: 740a 2320 4675 6e63 7469 6f6e 2066 6f72  t.# Function for
+000170d0: 2073 796e 7468 6573 6973 696e 6720 5461   synthesising Ta
+000170e0: 736b 730a 6c6f 6361 6c20 5461 736b 2861  sks.local Task(a
+000170f0: 7267 756d 656e 7473 3d5b 5d2c 2065 6e76  rguments=[], env
+00017100: 6972 6f6e 6d65 6e74 3d7b 7d29 203d 207b  ironment={}) = {
+00017110: 0a20 2020 2061 7267 756d 656e 7473 3a20  .    arguments: 
+00017120: 6172 6775 6d65 6e74 732c 0a20 2020 2065  arguments,.    e
+00017130: 6e76 6972 6f6e 6d65 6e74 3a20 656e 7669  nvironment: envi
+00017140: 726f 6e6d 656e 742c 0a20 2020 206e 616d  ronment,.    nam
+00017150: 653a 2022 6d79 5f74 6173 6b5f 7b7b 7461  e: "my_task_{{ta
+00017160: 736b 5f6e 756d 6265 727d 7d22 0a7d 3b0a  sk_number}}".};.
+00017170: 0a23 2057 6f72 6b20 5265 7175 6972 656d  .# Work Requirem
+00017180: 656e 740a 7b0a 2020 226e 616d 6522 3a20  ent.{.  "name": 
+00017190: 2277 6f72 6b72 6571 5f7b 7b64 6174 6574  "workreq_{{datet
+000171a0: 696d 657d 7d22 2c0a 2020 2274 6173 6b47  ime}}",.  "taskG
+000171b0: 726f 7570 7322 3a20 5b0a 2020 2020 7b0a  roups": [.    {.
+000171c0: 2020 2020 2020 2274 6173 6b73 223a 205b        "tasks": [
+000171d0: 0a20 2020 2020 2020 2054 6173 6b28 5b22  .        Task(["
+000171e0: 3122 5d2c 207b 413a 2022 415f 3122 7d29  1"], {A: "A_1"})
+000171f0: 2c20 2023 2061 7267 756d 656e 7473 2061  ,  # arguments a
+00017200: 6e64 2065 6e76 6972 6f6e 6d65 6e74 0a20  nd environment. 
+00017210: 2020 2020 2020 2054 6173 6b28 5b22 3222         Task(["2"
+00017220: 2c20 2233 225d 2c20 7b7d 292c 2020 2020  , "3"], {}),    
+00017230: 2023 2061 7267 756d 656e 7473 2061 6e64   # arguments and
+00017240: 2065 6d70 7479 2065 6e76 6972 6f6e 6d65   empty environme
+00017250: 6e74 0a20 2020 2020 2020 2054 6173 6b28  nt.        Task(
+00017260: 5b22 3422 5d29 2c20 2020 2020 2020 2020  ["4"]),         
+00017270: 2020 2020 2023 2061 7267 756d 656e 7473       # arguments
+00017280: 2061 6e64 2064 6566 6175 6c74 2065 6e76   and default env
+00017290: 6972 6f6e 6d65 6e74 0a20 2020 2020 2020  ironment.       
+000172a0: 2054 6173 6b28 2920 2020 2020 2020 2020   Task()         
+000172b0: 2020 2020 2020 2020 2020 2023 2064 6566             # def
+000172c0: 6175 6c74 2061 7267 756d 656e 7473 2061  ault arguments a
+000172d0: 6e64 2065 6e76 6972 6f6e 6d65 6e74 0a20  nd environment. 
+000172e0: 2020 2020 205d 0a20 2020 207d 0a20 205d       ].    }.  ]
+000172f0: 0a7d 0a60 6060 0a0a 5768 656e 2074 6869  .}.```..When thi
+00017300: 7320 6973 2069 6e73 7065 6374 6564 2075  s is inspected u
+00017310: 7369 6e67 2074 6865 2060 6a73 6f6e 6e65  sing the `jsonne
+00017320: 742d 6472 792d 7275 6e60 206f 7074 696f  t-dry-run` optio
+00017330: 6e20 2860 7964 2d73 7562 6d69 7420 2d4a  n (`yd-submit -J
+00017340: 7120 2d72 206d 795f 776f 726b 5f72 6571  q -r my_work_req
+00017350: 2e6a 736f 6e6e 6574 6029 2c20 7468 6973  .jsonnet`), this
+00017360: 2069 7320 7468 6520 7072 6f63 6573 7365   is the processe
+00017370: 6420 6f75 7470 7574 3a0a 0a60 6060 6a73  d output:..```js
+00017380: 6f6e 0a7b 0a20 2022 6e61 6d65 223a 2022  on.{.  "name": "
+00017390: 776f 726b 7265 715f 3233 3031 3134 2d31  workreq_230114-1
+000173a0: 3430 3634 3522 2c0a 2020 2274 6173 6b47  40645",.  "taskG
+000173b0: 726f 7570 7322 3a20 5b0a 2020 2020 7b0a  roups": [.    {.
+000173c0: 2020 2020 2020 2274 6173 6b73 223a 205b        "tasks": [
+000173d0: 0a20 2020 2020 2020 207b 0a20 2020 2020  .        {.     
+000173e0: 2020 2020 2022 6172 6775 6d65 6e74 7322       "arguments"
+000173f0: 3a20 5b22 3122 5d2c 0a20 2020 2020 2020  : ["1"],.       
+00017400: 2020 2022 656e 7669 726f 6e6d 656e 7422     "environment"
+00017410: 3a20 7b22 4122 3a20 2241 5f31 227d 2c0a  : {"A": "A_1"},.
+00017420: 2020 2020 2020 2020 2020 226e 616d 6522            "name"
+00017430: 3a20 226d 795f 7461 736b 5f7b 7b74 6173  : "my_task_{{tas
+00017440: 6b5f 6e75 6d62 6572 7d7d 220a 2020 2020  k_number}}".    
+00017450: 2020 2020 7d2c 0a20 2020 2020 2020 207b      },.        {
+00017460: 0a20 2020 2020 2020 2020 2022 6172 6775  .          "argu
+00017470: 6d65 6e74 7322 3a20 5b22 3222 2c20 2233  ments": ["2", "3
+00017480: 225d 2c0a 2020 2020 2020 2020 2020 2265  "],.          "e
+00017490: 6e76 6972 6f6e 6d65 6e74 223a 207b 7d2c  nvironment": {},
+000174a0: 0a20 2020 2020 2020 2020 2022 6e61 6d65  .          "name
+000174b0: 223a 2022 6d79 5f74 6173 6b5f 7b7b 7461  ": "my_task_{{ta
+000174c0: 736b 5f6e 756d 6265 727d 7d22 0a20 2020  sk_number}}".   
+000174d0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+000174e0: 7b0a 2020 2020 2020 2020 2020 2261 7267  {.          "arg
+000174f0: 756d 656e 7473 223a 205b 2234 225d 2c0a  uments": ["4"],.
+00017500: 2020 2020 2020 2020 2020 2265 6e76 6972            "envir
+00017510: 6f6e 6d65 6e74 223a 207b 7d2c 0a20 2020  onment": {},.   
+00017520: 2020 2020 2020 2022 6e61 6d65 223a 2022         "name": "
+00017530: 6d79 5f74 6173 6b5f 7b7b 7461 736b 5f6e  my_task_{{task_n
+00017540: 756d 6265 727d 7d22 0a20 2020 2020 2020  umber}}".       
+00017550: 207d 2c0a 2020 2020 2020 2020 7b0a 2020   },.        {.  
+00017560: 2020 2020 2020 2020 2261 7267 756d 656e          "argumen
+00017570: 7473 223a 205b 5d2c 0a20 2020 2020 2020  ts": [],.       
+00017580: 2020 2022 656e 7669 726f 6e6d 656e 7422     "environment"
+00017590: 3a20 7b7d 2c0a 2020 2020 2020 2020 2020  : {},.          
+000175a0: 226e 616d 6522 3a20 226d 795f 7461 736b  "name": "my_task
+000175b0: 5f7b 7b74 6173 6b5f 6e75 6d62 6572 7d7d  _{{task_number}}
+000175c0: 220a 2020 2020 2020 2020 7d0a 2020 2020  ".        }.    
+000175d0: 2020 5d0a 2020 2020 7d0a 2020 5d0a 7d0a    ].    }.  ].}.
+000175e0: 6060 600a 0a57 6865 6e20 7468 6973 2069  ```..When this i
+000175f0: 7320 696e 7370 6563 7465 6420 7573 696e  s inspected usin
+00017600: 6720 7468 6520 6064 7279 2d72 756e 6020  g the `dry-run` 
+00017610: 6f70 7469 6f6e 2028 6079 642d 7375 626d  option (`yd-subm
+00017620: 6974 202d 4471 202d 7220 6d79 5f77 6f72  it -Dq -r my_wor
+00017630: 6b5f 7265 712e 6a73 6f6e 6e65 7460 292c  k_req.jsonnet`),
+00017640: 2074 6869 7320 6973 2074 6865 2070 726f   this is the pro
+00017650: 6365 7373 6564 206f 7574 7075 743a 0a0a  cessed output:..
+00017660: 6060 606a 736f 6e0a 7b0a 2020 2266 756c  ```json.{.  "ful
+00017670: 6669 6c4f 6e53 7562 6d69 7422 3a20 6661  filOnSubmit": fa
+00017680: 6c73 652c 0a20 2022 6e61 6d65 223a 2022  lse,.  "name": "
+00017690: 776f 726b 7265 715f 3233 3031 3134 2d31  workreq_230114-1
+000176a0: 3430 3634 3522 2c0a 2020 226e 616d 6573  40645",.  "names
+000176b0: 7061 6365 223a 2022 7079 6578 616d 706c  pace": "pyexampl
+000176c0: 6573 222c 0a20 2022 7072 696f 7269 7479  es",.  "priority
+000176d0: 223a 2030 2c0a 2020 2274 6167 223a 2022  ": 0,.  "tag": "
+000176e0: 7079 6578 2d62 6173 6822 2c0a 2020 2274  pyex-bash",.  "t
+000176f0: 6173 6b47 726f 7570 7322 3a20 5b0a 2020  askGroups": [.  
+00017700: 2020 7b0a 2020 2020 2020 2266 696e 6973    {.      "finis
+00017710: 6849 6641 6c6c 5461 736b 7346 696e 6973  hIfAllTasksFinis
+00017720: 6865 6422 3a20 7472 7565 2c0a 2020 2020  hed": true,.    
+00017730: 2020 2266 696e 6973 6849 6641 6e79 5461    "finishIfAnyTa
+00017740: 736b 4661 696c 6564 223a 2066 616c 7365  skFailed": false
+00017750: 2c0a 2020 2020 2020 226e 616d 6522 3a20  ,.      "name": 
+00017760: 2274 6173 6b5f 6772 6f75 705f 3122 2c0a  "task_group_1",.
+00017770: 2020 2020 2020 2270 7269 6f72 6974 7922        "priority"
+00017780: 3a20 302c 0a20 2020 2020 2022 7275 6e53  : 0,.      "runS
+00017790: 7065 6369 6669 6361 7469 6f6e 223a 207b  pecification": {
+000177a0: 0a20 2020 2020 2020 2022 6d61 7869 6d75  .        "maximu
+000177b0: 6d54 6173 6b52 6574 7269 6573 223a 2030  mTaskRetries": 0
+000177c0: 2c0a 2020 2020 2020 2020 2274 6173 6b54  ,.        "taskT
+000177d0: 7970 6573 223a 205b 2262 6173 6822 5d2c  ypes": ["bash"],
+000177e0: 0a20 2020 2020 2020 2022 776f 726b 6572  .        "worker
+000177f0: 5461 6773 223a 205b 2270 7965 782d 6261  Tags": ["pyex-ba
+00017800: 7368 2d64 6f63 6b65 7222 5d0a 2020 2020  sh-docker"].    
+00017810: 2020 7d2c 0a20 2020 2020 2022 7461 736b    },.      "task
+00017820: 7322 3a20 5b0a 2020 2020 2020 2020 7b0a  s": [.        {.
+00017830: 2020 2020 2020 2020 2020 2261 7267 756d            "argum
+00017840: 656e 7473 223a 205b 2277 6f72 6b72 6571  ents": ["workreq
+00017850: 5f32 3330 3131 342d 3134 3036 3435 2f73  _230114-140645/s
+00017860: 6c65 6570 5f73 6372 6970 742e 7368 222c  leep_script.sh",
+00017870: 2022 3122 5d2c 0a20 2020 2020 2020 2020   "1"],.         
+00017880: 2022 656e 7669 726f 6e6d 656e 7422 3a20   "environment": 
+00017890: 7b22 4122 3a20 2241 5f31 227d 2c0a 2020  {"A": "A_1"},.  
+000178a0: 2020 2020 2020 2020 2269 6e70 7574 7322          "inputs"
+000178b0: 3a20 5b0a 2020 2020 2020 2020 2020 2020  : [.            
+000178c0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+000178d0: 226f 626a 6563 744e 616d 6550 6174 7465  "objectNamePatte
+000178e0: 726e 223a 2022 776f 726b 7265 715f 3233  rn": "workreq_23
+000178f0: 3031 3134 2d31 3430 3634 352f 736c 6565  0114-140645/slee
+00017900: 705f 7363 7269 7074 2e73 6822 2c0a 2020  p_script.sh",.  
+00017910: 2020 2020 2020 2020 2020 2020 2273 6f75              "sou
+00017920: 7263 6522 3a20 2254 4153 4b5f 4e41 4d45  rce": "TASK_NAME
+00017930: 5350 4143 4522 2c0a 2020 2020 2020 2020  SPACE",.        
+00017940: 2020 2020 2020 2276 6572 6966 6963 6174        "verificat
+00017950: 696f 6e22 3a20 2256 4552 4946 595f 4154  ion": "VERIFY_AT
+00017960: 5f53 5441 5254 220a 2020 2020 2020 2020  _START".        
+00017970: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
+00017980: 5d2c 0a20 2020 2020 2020 2020 2022 6e61  ],.          "na
+00017990: 6d65 223a 2022 6d79 5f74 6173 6b5f 3122  me": "my_task_1"
+000179a0: 2c0a 2020 2020 2020 2020 2020 226f 7574  ,.          "out
+000179b0: 7075 7473 223a 205b 0a20 2020 2020 2020  puts": [.       
+000179c0: 2020 2020 207b 2261 6c77 6179 7355 706c       {"alwaysUpl
+000179d0: 6f61 6422 3a20 7472 7565 2c20 2272 6571  oad": true, "req
+000179e0: 7569 7265 6422 3a20 6661 6c73 652c 2022  uired": false, "
+000179f0: 736f 7572 6365 223a 2022 5052 4f43 4553  source": "PROCES
+00017a00: 535f 4f55 5450 5554 227d 0a20 2020 2020  S_OUTPUT"}.     
+00017a10: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
+00017a20: 2020 2274 6173 6b54 7970 6522 3a20 2262    "taskType": "b
+00017a30: 6173 6822 0a20 2020 2020 2020 207d 2c0a  ash".        },.
+00017a40: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+00017a50: 2020 2020 2261 7267 756d 656e 7473 223a      "arguments":
+00017a60: 205b 2277 6f72 6b72 6571 5f32 3330 3131   ["workreq_23011
+00017a70: 342d 3134 3036 3435 2f73 6c65 6570 5f73  4-140645/sleep_s
+00017a80: 6372 6970 742e 7368 222c 2022 3222 2c20  cript.sh", "2", 
+00017a90: 2233 225d 2c0a 2020 2020 2020 2020 2020  "3"],.          
+00017aa0: 2265 6e76 6972 6f6e 6d65 6e74 223a 207b  "environment": {
+00017ab0: 7d2c 0a20 2020 2020 2020 2020 2022 696e  },.          "in
+00017ac0: 7075 7473 223a 205b 0a20 2020 2020 2020  puts": [.       
+00017ad0: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00017ae0: 2020 2020 2022 6f62 6a65 6374 4e61 6d65       "objectName
+00017af0: 5061 7474 6572 6e22 3a20 2277 6f72 6b72  Pattern": "workr
+00017b00: 6571 5f32 3330 3131 342d 3134 3036 3435  eq_230114-140645
+00017b10: 2f73 6c65 6570 5f73 6372 6970 742e 7368  /sleep_script.sh
+00017b20: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00017b30: 2022 736f 7572 6365 223a 2022 5441 534b   "source": "TASK
+00017b40: 5f4e 414d 4553 5041 4345 222c 0a20 2020  _NAMESPACE",.   
+00017b50: 2020 2020 2020 2020 2020 2022 7665 7269             "veri
+00017b60: 6669 6361 7469 6f6e 223a 2022 5645 5249  fication": "VERI
+00017b70: 4659 5f41 545f 5354 4152 5422 0a20 2020  FY_AT_START".   
+00017b80: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00017b90: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
+00017ba0: 2020 226e 616d 6522 3a20 226d 795f 7461    "name": "my_ta
+00017bb0: 736b 5f32 222c 0a20 2020 2020 2020 2020  sk_2",.         
+00017bc0: 2022 6f75 7470 7574 7322 3a20 5b0a 2020   "outputs": [.  
+00017bd0: 2020 2020 2020 2020 2020 7b22 616c 7761            {"alwa
+00017be0: 7973 5570 6c6f 6164 223a 2074 7275 652c  ysUpload": true,
+00017bf0: 2022 7265 7175 6972 6564 223a 2066 616c   "required": fal
+00017c00: 7365 2c20 2273 6f75 7263 6522 3a20 2250  se, "source": "P
+00017c10: 524f 4345 5353 5f4f 5554 5055 5422 7d0a  ROCESS_OUTPUT"}.
+00017c20: 2020 2020 2020 2020 2020 5d2c 0a20 2020            ],.   
+00017c30: 2020 2020 2020 2022 7461 736b 5479 7065         "taskType
+00017c40: 223a 2022 6261 7368 220a 2020 2020 2020  ": "bash".      
+00017c50: 2020 7d2c 0a20 2020 2020 2020 207b 0a20    },.        {. 
+00017c60: 2020 2020 2020 2020 2022 6172 6775 6d65           "argume
+00017c70: 6e74 7322 3a20 5b22 776f 726b 7265 715f  nts": ["workreq_
+00017c80: 3233 3031 3134 2d31 3430 3634 352f 736c  230114-140645/sl
+00017c90: 6565 705f 7363 7269 7074 2e73 6822 2c20  eep_script.sh", 
+00017ca0: 2234 225d 2c0a 2020 2020 2020 2020 2020  "4"],.          
+00017cb0: 2265 6e76 6972 6f6e 6d65 6e74 223a 207b  "environment": {
+00017cc0: 7d2c 0a20 2020 2020 2020 2020 2022 696e  },.          "in
+00017cd0: 7075 7473 223a 205b 0a20 2020 2020 2020  puts": [.       
+00017ce0: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00017cf0: 2020 2020 2022 6f62 6a65 6374 4e61 6d65       "objectName
+00017d00: 5061 7474 6572 6e22 3a20 2277 6f72 6b72  Pattern": "workr
+00017d10: 6571 5f32 3330 3131 342d 3134 3036 3435  eq_230114-140645
+00017d20: 2f73 6c65 6570 5f73 6372 6970 742e 7368  /sleep_script.sh
+00017d30: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00017d40: 2022 736f 7572 6365 223a 2022 5441 534b   "source": "TASK
+00017d50: 5f4e 414d 4553 5041 4345 222c 0a20 2020  _NAMESPACE",.   
+00017d60: 2020 2020 2020 2020 2020 2022 7665 7269             "veri
+00017d70: 6669 6361 7469 6f6e 223a 2022 5645 5249  fication": "VERI
+00017d80: 4659 5f41 545f 5354 4152 5422 0a20 2020  FY_AT_START".   
+00017d90: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00017da0: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
+00017db0: 2020 226e 616d 6522 3a20 226d 795f 7461    "name": "my_ta
+00017dc0: 736b 5f33 222c 0a20 2020 2020 2020 2020  sk_3",.         
+00017dd0: 2022 6f75 7470 7574 7322 3a20 5b0a 2020   "outputs": [.  
+00017de0: 2020 2020 2020 2020 2020 7b22 616c 7761            {"alwa
+00017df0: 7973 5570 6c6f 6164 223a 2074 7275 652c  ysUpload": true,
+00017e00: 2022 7265 7175 6972 6564 223a 2066 616c   "required": fal
+00017e10: 7365 2c20 2273 6f75 7263 6522 3a20 2250  se, "source": "P
+00017e20: 524f 4345 5353 5f4f 5554 5055 5422 7d0a  ROCESS_OUTPUT"}.
+00017e30: 2020 2020 2020 2020 2020 5d2c 0a20 2020            ],.   
+00017e40: 2020 2020 2020 2022 7461 736b 5479 7065         "taskType
+00017e50: 223a 2022 6261 7368 220a 2020 2020 2020  ": "bash".      
+00017e60: 2020 7d2c 0a20 2020 2020 2020 207b 0a20    },.        {. 
+00017e70: 2020 2020 2020 2020 2022 6172 6775 6d65           "argume
+00017e80: 6e74 7322 3a20 5b22 776f 726b 7265 715f  nts": ["workreq_
+00017e90: 3233 3031 3134 2d31 3430 3634 352f 736c  230114-140645/sl
+00017ea0: 6565 705f 7363 7269 7074 2e73 6822 5d2c  eep_script.sh"],
+00017eb0: 0a20 2020 2020 2020 2020 2022 656e 7669  .          "envi
+00017ec0: 726f 6e6d 656e 7422 3a20 7b7d 2c0a 2020  ronment": {},.  
+00017ed0: 2020 2020 2020 2020 2269 6e70 7574 7322          "inputs"
+00017ee0: 3a20 5b0a 2020 2020 2020 2020 2020 2020  : [.            
+00017ef0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00017f00: 226f 626a 6563 744e 616d 6550 6174 7465  "objectNamePatte
+00017f10: 726e 223a 2022 776f 726b 7265 715f 3233  rn": "workreq_23
+00017f20: 3031 3134 2d31 3430 3634 352f 736c 6565  0114-140645/slee
+00017f30: 705f 7363 7269 7074 2e73 6822 2c0a 2020  p_script.sh",.  
+00017f40: 2020 2020 2020 2020 2020 2020 2273 6f75              "sou
+00017f50: 7263 6522 3a20 2254 4153 4b5f 4e41 4d45  rce": "TASK_NAME
+00017f60: 5350 4143 4522 2c0a 2020 2020 2020 2020  SPACE",.        
+00017f70: 2020 2020 2020 2276 6572 6966 6963 6174        "verificat
+00017f80: 696f 6e22 3a20 2256 4552 4946 595f 4154  ion": "VERIFY_AT
+00017f90: 5f53 5441 5254 220a 2020 2020 2020 2020  _START".        
+00017fa0: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
+00017fb0: 5d2c 0a20 2020 2020 2020 2020 2022 6e61  ],.          "na
+00017fc0: 6d65 223a 2022 6d79 5f74 6173 6b5f 3422  me": "my_task_4"
+00017fd0: 2c0a 2020 2020 2020 2020 2020 226f 7574  ,.          "out
+00017fe0: 7075 7473 223a 205b 0a20 2020 2020 2020  puts": [.       
+00017ff0: 2020 2020 207b 2261 6c77 6179 7355 706c       {"alwaysUpl
+00018000: 6f61 6422 3a20 7472 7565 2c20 2272 6571  oad": true, "req
+00018010: 7569 7265 6422 3a20 6661 6c73 652c 2022  uired": false, "
+00018020: 736f 7572 6365 223a 2022 5052 4f43 4553  source": "PROCES
+00018030: 535f 4f55 5450 5554 227d 0a20 2020 2020  S_OUTPUT"}.     
+00018040: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
+00018050: 2020 2274 6173 6b54 7970 6522 3a20 2262    "taskType": "b
+00018060: 6173 6822 0a20 2020 2020 2020 207d 0a20  ash".        }. 
+00018070: 2020 2020 205d 0a20 2020 207d 0a20 205d       ].    }.  ]
+00018080: 0a7d 0a60 6060 0a0a 2320 436f 6d6d 616e  .}.```..# Comman
+00018090: 6420 4c69 7374 0a0a 4865 6c70 2069 7320  d List..Help is 
+000180a0: 6176 6169 6c61 626c 6520 666f 7220 616c  available for al
+000180b0: 6c20 636f 6d6d 616e 6473 2062 7920 696e  l commands by in
+000180c0: 766f 6b69 6e67 2061 2063 6f6d 6d61 6e64  voking a command
+000180d0: 2077 6974 6820 7468 6520 602d 2d68 656c   with the `--hel
+000180e0: 7060 206f 7220 602d 6860 206f 7074 696f  p` or `-h` optio
+000180f0: 6e2e 2053 6f6d 6520 636f 6d6d 616e 6420  n. Some command 
+00018100: 6c69 6e65 2070 6172 616d 6574 6572 7320  line parameters 
+00018110: 6172 6520 636f 6d6d 6f6e 2074 6f20 616c  are common to al
+00018120: 6c20 636f 6d6d 616e 6473 2c20 7768 696c  l commands, whil
+00018130: 6520 6f74 6865 7273 2061 7265 2063 6f6d  e others are com
+00018140: 6d61 6e64 2d73 7065 6369 6669 632e 0a0a  mand-specific...
+00018150: 416c 6c20 6465 7374 7275 6374 6976 6520  All destructive 
+00018160: 636f 6d6d 616e 6473 2072 6571 7569 7265  commands require
+00018170: 2075 7365 7220 636f 6e66 6972 6d61 7469   user confirmati
+00018180: 6f6e 2062 6566 6f72 6520 7461 6b69 6e67  on before taking
+00018190: 2065 6666 6563 742e 2054 6869 7320 6361   effect. This ca
+000181a0: 6e20 6265 2073 7570 7072 6573 7365 6420  n be suppressed 
+000181b0: 7573 696e 6720 7468 6520 602d 2d79 6573  using the `--yes
+000181c0: 6020 6f72 2060 2d79 6020 6f70 7469 6f6e  ` or `-y` option
+000181d0: 2c20 696e 2077 6869 6368 2063 6173 6520  , in which case 
+000181e0: 7468 6520 636f 6d6d 616e 6420 7769 6c6c  the command will
+000181f0: 2070 726f 6365 6564 2077 6974 686f 7574   proceed without
+00018200: 2063 6f6e 6669 726d 6174 696f 6e2e 0a0a   confirmation...
+00018210: 536f 6d65 2063 6f6d 6d61 6e64 7320 7375  Some commands su
+00018220: 7070 6f72 7420 7468 6520 602d 2d69 6e74  pport the `--int
+00018230: 6572 6163 7469 7665 6020 6f72 2060 2d69  eractive` or `-i
+00018240: 6020 6f70 7469 6f6e 2c20 616c 6c6f 7769  ` option, allowi
+00018250: 6e67 2075 7365 7220 7365 6c65 6374 696f  ng user selectio
+00018260: 6e73 2074 6f20 6265 206d 6164 652e 2045  ns to be made. E
+00018270: 2e67 2e2c 2074 6869 7320 6361 6e20 6265  .g., this can be
+00018280: 2075 7365 6420 746f 2073 656c 6563 7420   used to select 
+00018290: 7768 6963 6820 6f62 6a65 6374 2070 6174  which object pat
+000182a0: 6873 2074 6f20 6465 6c65 7465 2e0a 0a54  hs to delete...T
+000182b0: 6865 2060 2d2d 7175 6965 7460 206f 7220  he `--quiet` or 
+000182c0: 602d 7160 206f 7074 696f 6e20 7265 6475  `-q` option redu
+000182d0: 6365 7320 7468 6520 636f 6d6d 616e 6420  ces the command 
+000182e0: 6f75 7470 7574 2064 6f77 6e20 746f 2065  output down to e
+000182f0: 7373 656e 7469 616c 206d 6573 7361 6765  ssential message
+00018300: 7320 6f6e 6c79 2e20 536f 2c20 666f 7220  s only. So, for 
+00018310: 6578 616d 706c 652c 2060 7964 2d64 656c  example, `yd-del
+00018320: 6574 6520 2d79 7160 2077 6f75 6c64 2064  ete -yq` would d
+00018330: 656c 6574 6520 616c 6c20 6d61 7463 6869  elete all matchi
+00018340: 6e67 206f 626a 6563 7420 7061 7468 7320  ng object paths 
+00018350: 7369 6c65 6e74 6c79 2e0a 0a49 6620 796f  silently...If yo
+00018360: 7520 656e 636f 756e 7465 7220 616e 2065  u encounter an e
+00018370: 7272 6f72 2069 7420 6361 6e20 6265 2075  rror it can be u
+00018380: 7365 6675 6c20 666f 7220 7375 7070 6f72  seful for suppor
+00018390: 7420 7075 7270 6f73 6573 2074 6f20 7365  t purposes to se
+000183a0: 6520 7468 6520 6675 6c6c 2050 7974 686f  e the full Pytho
+000183b0: 6e20 7374 6163 6b20 7472 6163 652e 2054  n stack trace. T
+000183c0: 6869 7320 6361 6e20 6265 2065 6e61 626c  his can be enabl
+000183d0: 6564 2062 7920 7275 6e6e 696e 6720 7468  ed by running th
+000183e0: 6520 636f 6d6d 616e 6420 7573 696e 6720  e command using 
+000183f0: 7468 6520 602d 2d64 6562 7567 6020 6f70  the `--debug` op
+00018400: 7469 6f6e 2e0a 0a23 2320 7964 2d73 7562  tion...## yd-sub
+00018410: 6d69 740a 0a54 6865 2060 7964 2d73 7562  mit..The `yd-sub
+00018420: 6d69 7460 2063 6f6d 6d61 6e64 2073 7562  mit` command sub
+00018430: 6d69 7473 2061 206e 6577 2057 6f72 6b20  mits a new Work 
+00018440: 5265 7175 6972 656d 656e 742c 2061 6363  Requirement, acc
+00018450: 6f72 6469 6e67 2074 6f20 7468 6520 576f  ording to the Wo
+00018460: 726b 2052 6571 7569 7265 6d65 6e74 2064  rk Requirement d
+00018470: 6566 696e 6974 696f 6e20 666f 756e 6420  efinition found 
+00018480: 696e 2074 6865 2060 776f 726b 5265 7175  in the `workRequ
+00018490: 6972 656d 656e 7460 2073 6563 7469 6f6e  irement` section
+000184a0: 206f 6620 7468 6520 544f 4d4c 2063 6f6e   of the TOML con
+000184b0: 6669 6775 7261 7469 6f6e 2066 696c 6520  figuration file 
+000184c0: 616e 642f 6f72 2074 6865 2073 7065 6369  and/or the speci
+000184d0: 6669 6361 7469 6f6e 2066 6f75 6e64 2069  fication found i
+000184e0: 6e20 6120 576f 726b 2052 6571 7569 7265  n a Work Require
+000184f0: 6d65 6e74 204a 534f 4e20 646f 6375 6d65  ment JSON docume
+00018500: 6e74 2073 7570 706c 6965 6420 7573 696e  nt supplied usin
+00018510: 6720 7468 6520 602d 2d77 6f72 6b2d 7265  g the `--work-re
+00018520: 7175 6972 656d 656e 7460 206f 7074 696f  quirement` optio
+00018530: 6e2e 0a0a 5573 6520 7468 6520 602d 2d64  n...Use the `--d
+00018540: 7279 2d72 756e 6020 6f70 7469 6f6e 2074  ry-run` option t
+00018550: 6f20 696e 7370 6563 7420 7468 6520 6465  o inspect the de
+00018560: 7461 696c 7320 6f66 2074 6865 2057 6f72  tails of the Wor
+00018570: 6b20 5265 7175 6972 656d 656e 742c 2054  k Requirement, T
+00018580: 6173 6b20 4772 6f75 7073 2c20 616e 6420  ask Groups, and 
+00018590: 5461 736b 7320 7468 6174 2077 696c 6c20  Tasks that will 
+000185a0: 6265 2073 7562 6d69 7474 6564 2c20 696e  be submitted, in
+000185b0: 204a 534f 4e20 666f 726d 6174 2e0a 0a4f   JSON format...O
+000185c0: 6e63 6520 7375 626d 6974 7465 642c 2074  nce submitted, t
+000185d0: 6865 2057 6f72 6b20 5265 7175 6972 656d  he Work Requirem
+000185e0: 656e 7420 7769 6c6c 2061 7070 6561 7220  ent will appear 
+000185f0: 696e 2074 6865 202a 2a57 6f72 6b2a 2a20  in the **Work** 
+00018600: 7461 6220 696e 2074 6865 2059 656c 6c6f  tab in the Yello
+00018610: 7744 6f67 2050 6f72 7461 6c2e 0a0a 5468  wDog Portal...Th
+00018620: 6520 576f 726b 2052 6571 7569 7265 6d65  e Work Requireme
+00018630: 6e74 2773 2070 726f 6772 6573 7320 6361  nt's progress ca
+00018640: 6e20 6265 2074 7261 636b 6564 2074 6f20  n be tracked to 
+00018650: 636f 6d70 6c65 7469 6f6e 2062 7920 7573  completion by us
+00018660: 696e 6720 7468 6520 602d 2d66 6f6c 6c6f  ing the `--follo
+00018670: 7760 2028 6f72 2060 2d66 6029 206f 7074  w` (or `-f`) opt
+00018680: 696f 6e20 7768 656e 2069 6e76 6f6b 696e  ion when invokin
+00018690: 6720 6079 642d 7375 626d 6974 603a 2074  g `yd-submit`: t
+000186a0: 6865 2063 6f6d 6d61 6e64 2077 696c 6c20  he command will 
+000186b0: 7265 706f 7274 206f 6e20 5461 736b 7320  report on Tasks 
+000186c0: 6173 2074 6865 7920 636f 6e63 6c75 6465  as they conclude
+000186d0: 2061 6e64 2077 6f6e 2774 2072 6574 7572   and won't retur
+000186e0: 6e20 756e 7469 6c20 7468 6520 576f 726b  n until the Work
+000186f0: 2052 6571 7569 7265 6d65 6e74 2068 6173   Requirement has
+00018700: 2066 696e 6973 6865 642e 0a0a 2323 2079   finished...## y
+00018710: 642d 7072 6f76 6973 696f 6e0a 0a54 6865  d-provision..The
+00018720: 2060 7964 2d70 726f 7669 7369 6f6e 6020   `yd-provision` 
+00018730: 636f 6d6d 616e 6420 7072 6f76 6973 696f  command provisio
+00018740: 6e73 2061 206e 6577 2057 6f72 6b65 7220  ns a new Worker 
+00018750: 506f 6f6c 2061 6363 6f72 6469 6e67 2074  Pool according t
+00018760: 6f20 7468 6520 7370 6563 6966 6963 6174  o the specificat
+00018770: 696f 6e73 2069 6e20 7468 6520 6077 6f72  ions in the `wor
+00018780: 6b65 7250 6f6f 6c60 2073 6563 7469 6f6e  kerPool` section
+00018790: 206f 6620 7468 6520 544f 4d4c 2063 6f6e   of the TOML con
+000187a0: 6669 6775 7261 7469 6f6e 2066 696c 6520  figuration file 
+000187b0: 616e 642f 6f72 2069 6e20 7468 6520 7370  and/or in the sp
+000187c0: 6563 6966 6963 6174 696f 6e20 666f 756e  ecification foun
+000187d0: 6420 696e 2061 2057 6f72 6b65 7220 506f  d in a Worker Po
+000187e0: 6f6c 204a 534f 4e20 646f 6375 6d65 6e74  ol JSON document
+000187f0: 2073 7570 706c 6965 6420 7573 696e 6720   supplied using 
+00018800: 7468 6520 602d 2d77 6f72 6b65 722d 706f  the `--worker-po
+00018810: 6f6c 6020 6f70 7469 6f6e 2e0a 0a55 7365  ol` option...Use
+00018820: 2074 6865 2060 2d2d 6472 792d 7275 6e60   the `--dry-run`
+00018830: 206f 7074 696f 6e20 746f 2069 6e73 7065   option to inspe
+00018840: 6374 2074 6865 2064 6574 6169 6c73 206f  ct the details o
+00018850: 6620 7468 6520 576f 726b 6572 2050 6f6f  f the Worker Poo
+00018860: 6c20 7370 6563 6966 6963 6174 696f 6e20  l specification 
+00018870: 7468 6174 2077 696c 6c20 6265 2073 7562  that will be sub
+00018880: 6d69 7474 6564 2c20 696e 204a 534f 4e20  mitted, in JSON 
+00018890: 666f 726d 6174 2e0a 0a4f 6e63 6520 7072  format...Once pr
+000188a0: 6f76 6973 696f 6e65 642c 2074 6865 2057  ovisioned, the W
+000188b0: 6f72 6b65 7220 506f 6f6c 2077 696c 6c20  orker Pool will 
+000188c0: 6170 7065 6172 2069 6e20 7468 6520 2a2a  appear in the **
+000188d0: 576f 726b 6572 732a 2a20 7461 6220 696e  Workers** tab in
+000188e0: 2074 6865 2059 656c 6c6f 7744 6f67 2050   the YellowDog P
+000188f0: 6f72 7461 6c2c 2061 6e64 2069 7473 2061  ortal, and its a
+00018900: 7373 6f63 6961 7465 6420 436f 6d70 7574  ssociated Comput
+00018910: 6520 5265 7175 6972 656d 656e 7420 7769  e Requirement wi
+00018920: 6c6c 2061 7070 6561 7220 696e 2074 6865  ll appear in the
+00018930: 202a 2a43 6f6d 7075 7465 2a2a 2074 6162   **Compute** tab
+00018940: 2e0a 0a23 2320 7964 2d63 616e 6365 6c0a  ...## yd-cancel.
+00018950: 0a54 6865 2060 7964 2d63 616e 6365 6c60  .The `yd-cancel`
+00018960: 2063 6f6d 6d61 6e64 2063 616e 6365 6c73   command cancels
+00018970: 2061 6e79 2061 6374 6976 6520 576f 726b   any active Work
+00018980: 2052 6571 7569 7265 6d65 6e74 732c 2069   Requirements, i
+00018990: 6e63 6c75 6469 6e67 2061 6e79 2070 656e  ncluding any pen
+000189a0: 6469 6e67 2054 6173 6b20 4772 6f75 7073  ding Task Groups
+000189b0: 2061 6e64 2074 6865 2054 6173 6b73 2074   and the Tasks t
+000189c0: 6865 7920 636f 6e74 6169 6e2e 200a 0a54  hey contain. ..T
+000189d0: 6865 2060 6e61 6d65 7370 6163 6560 2061  he `namespace` a
+000189e0: 6e64 2060 7461 6760 2076 616c 7565 7320  nd `tag` values 
+000189f0: 696e 2074 6865 2060 636f 6e66 6967 2e74  in the `config.t
+00018a00: 6f6d 6c60 2066 696c 6520 6172 6520 7573  oml` file are us
+00018a10: 6564 2074 6f20 6964 656e 7469 6679 2077  ed to identify w
+00018a20: 6869 6368 2057 6f72 6b20 5265 7175 6972  hich Work Requir
+00018a30: 656d 656e 7473 2074 6f20 6361 6e63 656c  ements to cancel
+00018a40: 2e0a 0a42 7920 6465 6661 756c 742c 2061  ...By default, a
+00018a50: 6e79 2054 6173 6b73 2074 6861 7420 6172  ny Tasks that ar
+00018a60: 6520 6375 7272 656e 746c 7920 7275 6e6e  e currently runn
+00018a70: 696e 6720 6f6e 2057 6f72 6b65 7273 2077  ing on Workers w
+00018a80: 696c 6c20 636f 6e74 696e 7565 2074 6f20  ill continue to 
+00018a90: 7275 6e20 746f 2063 6f6d 706c 6574 696f  run to completio
+00018aa0: 6e20 6f72 2075 6e74 696c 2074 6865 7920  n or until they 
+00018ab0: 6661 696c 2e20 5461 736b 7320 6361 6e20  fail. Tasks can 
+00018ac0: 6265 2069 6e73 7472 7563 7465 6420 746f  be instructed to
+00018ad0: 2061 626f 7274 2069 6d6d 6564 6961 7465   abort immediate
+00018ae0: 6c79 2062 7920 7375 7070 6c79 696e 6720  ly by supplying 
+00018af0: 7468 6520 602d 2d61 626f 7274 6020 6f72  the `--abort` or
+00018b00: 2060 2d61 6020 6f70 7469 6f6e 2074 6f20   `-a` option to 
+00018b10: 6079 642d 6361 6e63 656c 602e 0a0a 2323  `yd-cancel`...##
+00018b20: 2079 642d 6162 6f72 740a 0a54 6865 2060   yd-abort..The `
+00018b30: 7964 2d61 626f 7274 6020 636f 6d6d 616e  yd-abort` comman
+00018b40: 6420 6973 2075 7365 6420 746f 2061 626f  d is used to abo
+00018b50: 7274 2054 6173 6b73 2074 6861 7420 6172  rt Tasks that ar
+00018b60: 6520 6375 7272 656e 746c 7920 7275 6e6e  e currently runn
+00018b70: 696e 672e 2054 6865 2075 7365 7220 696e  ing. The user in
+00018b80: 7465 7261 6374 6976 656c 7920 7365 6c65  teractively sele
+00018b90: 6374 7320 7468 6520 576f 726b 2052 6571  cts the Work Req
+00018ba0: 7569 7265 6d65 6e74 7320 746f 2074 6172  uirements to tar
+00018bb0: 6765 742c 2061 6e64 2074 6865 6e20 7768  get, and then wh
+00018bc0: 6963 6820 5461 736b 7320 7769 7468 696e  ich Tasks within
+00018bd0: 2074 686f 7365 2057 6f72 6b20 5265 7175   those Work Requ
+00018be0: 6972 656d 656e 7473 2074 6f20 6162 6f72  irements to abor
+00018bf0: 742e 2054 6865 2057 6f72 6b20 5265 7175  t. The Work Requ
+00018c00: 6972 656d 656e 7473 2061 7265 206e 6f74  irements are not
+00018c10: 2063 616e 6365 6c6c 6564 2061 7320 7061   cancelled as pa
+00018c20: 7274 206f 6620 7468 6973 2070 726f 6365  rt of this proce
+00018c30: 7373 2e0a 0a54 6865 2060 6e61 6d65 7370  ss...The `namesp
+00018c40: 6163 6560 2061 6e64 2060 7461 6760 2076  ace` and `tag` v
+00018c50: 616c 7565 7320 696e 2074 6865 2060 636f  alues in the `co
+00018c60: 6e66 6967 2e74 6f6d 6c60 2066 696c 6520  nfig.toml` file 
+00018c70: 6172 6520 7573 6564 2074 6f20 6964 656e  are used to iden
+00018c80: 7469 6679 2077 6869 6368 2057 6f72 6b20  tify which Work 
+00018c90: 5265 7175 6972 656d 656e 7473 2074 6f20  Requirements to 
+00018ca0: 6c69 7374 2066 6f72 2073 656c 6563 7469  list for selecti
+00018cb0: 6f6e 2e0a 0a23 2320 7964 2d64 6f77 6e6c  on...## yd-downl
+00018cc0: 6f61 640a 0a54 6865 2060 7964 2d64 6f77  oad..The `yd-dow
+00018cd0: 6e6c 6f61 6460 2063 6f6d 6d61 6e64 2064  nload` command d
+00018ce0: 6f77 6e6c 6f61 6473 2061 6e79 206f 626a  ownloads any obj
+00018cf0: 6563 7473 2063 7265 6174 6564 2069 6e20  ects created in 
+00018d00: 7468 6520 5965 6c6c 6f77 446f 6720 4f62  the YellowDog Ob
+00018d10: 6a65 6374 2053 746f 7265 2e0a 0a54 6865  ject Store...The
+00018d20: 2060 6e61 6d65 7370 6163 6560 2061 6e64   `namespace` and
+00018d30: 2060 7461 6760 2076 616c 7565 7320 6172   `tag` values ar
+00018d40: 6520 7573 6564 2074 6f20 6465 7465 726d  e used to determ
+00018d50: 696e 6520 7768 6963 6820 6f62 6a65 6374  ine which object
+00018d60: 7320 746f 2064 6f77 6e6c 6f61 642e 204f  s to download. O
+00018d70: 626a 6563 7473 2077 696c 6c20 6265 2064  bjects will be d
+00018d80: 6f77 6e6c 6f61 6465 6420 746f 2061 2064  ownloaded to a d
+00018d90: 6972 6563 746f 7279 2077 6974 6820 7468  irectory with th
+00018da0: 6520 7361 6d65 206e 616d 6520 6173 2060  e same name as `
+00018db0: 6e61 6d65 7370 6163 6560 2e20 4966 2061  namespace`. If a
+00018dc0: 2064 6972 6563 746f 7279 2061 6c72 6561   directory alrea
+00018dd0: 6479 2065 7869 7374 732c 2061 206e 6577  dy exists, a new
+00018de0: 2064 6972 6563 746f 7279 2077 6974 6820   directory with 
+00018df0: 6e61 6d65 2060 3c6e 616d 6573 7061 6365  name `<namespace
+00018e00: 3e2e 3031 6020 2865 7463 2e29 2077 696c  >.01` (etc.) wil
+00018e10: 6c20 6265 2063 7265 6174 6564 2e0a 0a23  l be created...#
+00018e20: 2320 7964 2d64 656c 6574 650a 0a54 6865  # yd-delete..The
+00018e30: 2060 7964 2d64 656c 6574 6560 2063 6f6d   `yd-delete` com
+00018e40: 6d61 6e64 2064 656c 6574 6573 2061 6e79  mand deletes any
+00018e50: 206f 626a 6563 7473 2063 7265 6174 6564   objects created
+00018e60: 2069 6e20 7468 6520 5965 6c6c 6f77 446f   in the YellowDo
+00018e70: 6720 4f62 6a65 6374 2053 746f 7265 2e0a  g Object Store..
+00018e80: 0a54 6865 2060 6e61 6d65 7370 6163 6560  .The `namespace`
+00018e90: 2061 6e64 2060 7461 6760 2076 616c 7565   and `tag` value
+00018ea0: 7320 696e 2074 6865 2060 636f 6e66 6967  s in the `config
+00018eb0: 2e74 6f6d 6c60 2066 696c 6520 6172 6520  .toml` file are 
+00018ec0: 7573 6564 2074 6f20 6964 656e 7469 6679  used to identify
+00018ed0: 2077 6869 6368 206f 626a 6563 7473 2074   which objects t
+00018ee0: 6f20 6465 6c65 7465 2e20 4e6f 7465 2074  o delete. Note t
+00018ef0: 6861 7420 6974 2773 2065 6173 7920 746f  hat it's easy to
+00018f00: 2075 7365 2060 7964 2d64 656c 6574 6560   use `yd-delete`
+00018f10: 2074 6f20 636c 6561 7220 7468 6520 636f   to clear the co
+00018f20: 6e74 656e 7473 206f 6620 6120 6e61 6d65  ntents of a name
+00018f30: 7370 6163 6520 6279 2075 7369 6e67 2061  space by using a
+00018f40: 6e20 656d 7074 7920 6074 6167 602c 2061  n empty `tag`, a
+00018f50: 7320 666f 6c6c 6f77 733a 0a0a 6060 6073  s follows:..```s
+00018f60: 6865 6c6c 0a79 642d 6465 6c65 7465 202d  hell.yd-delete -
+00018f70: 7420 2222 0a60 6060 0a0a 5468 6973 2063  t "".```..This c
+00018f80: 616e 2062 6520 6578 7465 6e64 6564 2074  an be extended t
+00018f90: 6f20 616e 7920 6f74 6865 7220 6e61 6d65  o any other name
+00018fa0: 7370 6163 6520 6279 2075 7369 6e67 2074  space by using t
+00018fb0: 6865 2060 2d2d 6e61 6d65 7370 6163 6560  he `--namespace`
+00018fc0: 2f60 2d6e 6020 6f70 7469 6f6e 2e0a 0a23  /`-n` option...#
+00018fd0: 2320 7964 2d75 706c 6f61 640a 0a54 6865  # yd-upload..The
+00018fe0: 2060 7964 2d75 706c 6f61 6460 2063 6f6d   `yd-upload` com
+00018ff0: 6d61 6e64 2075 706c 6f61 6473 2066 696c  mand uploads fil
+00019000: 6573 2066 726f 6d20 7468 6520 6c6f 6361  es from the loca
+00019010: 6c20 6669 6c65 7379 7374 656d 2074 6f20  l filesystem to 
+00019020: 7468 6520 5965 6c6c 6f77 446f 6720 4f62  the YellowDog Ob
+00019030: 6a65 6374 2073 746f 7265 2e20 4669 6c65  ject store. File
+00019040: 7320 6172 6520 706c 6163 6564 2069 6e20  s are placed in 
+00019050: 7468 6520 636f 6e66 6967 7572 6564 2060  the configured `
+00019060: 6e61 6d65 7370 6163 6560 2077 6974 6869  namespace` withi
+00019070: 6e20 6120 6469 7265 6374 6f72 7920 7375  n a directory su
+00019080: 7070 6c69 6564 2075 7369 6e67 2074 6865  pplied using the
+00019090: 2028 7265 7175 6972 6564 2920 602d 2d64   (required) `--d
+000190a0: 6972 6563 746f 7279 6020 6f70 7469 6f6e  irectory` option
+000190b0: 2c20 652e 672e 3a0a 0a60 6060 7368 656c  , e.g.:..```shel
+000190c0: 6c0a 7964 2d75 706c 6f61 6420 2d2d 6469  l.yd-upload --di
+000190d0: 7265 6374 6f72 7920 6d79 5f77 6f72 6b5f  rectory my_work_
+000190e0: 7265 7175 6972 656d 656e 7420 6669 6c65  requirement file
+000190f0: 5f31 2066 696c 655f 3220 6d6f 7265 6669  _1 file_2 morefi
+00019100: 6c65 732f 6669 6c65 330a 6060 600a 546f  les/file3.```.To
+00019110: 2073 7570 7072 6573 7320 7468 6520 6d69   suppress the mi
+00019120: 7272 6f72 696e 6720 6f66 2074 6865 206c  rroring of the l
+00019130: 6f63 616c 2064 6972 6563 746f 7279 2073  ocal directory s
+00019140: 7472 7563 7475 7265 2077 6974 6869 6e20  tructure within 
+00019150: 7468 6520 6f62 6a65 6374 2073 746f 7265  the object store
+00019160: 2c20 7573 6520 7468 6520 602d 2d66 6c61  , use the `--fla
+00019170: 7474 656e 2d75 706c 6f61 642d 7061 7468  tten-upload-path
+00019180: 7360 206f 7220 602d 6660 206f 7074 696f  s` or `-f` optio
+00019190: 6e2e 204e 6f74 6520 7468 6174 2069 6620  n. Note that if 
+000191a0: 7468 6973 2063 7265 6174 6573 206d 756c  this creates mul
+000191b0: 7469 706c 6520 7570 6c6f 6164 6564 2066  tiple uploaded f
+000191c0: 696c 6573 2077 6974 6820 7468 6520 7361  iles with the sa
+000191d0: 6d65 2070 6174 6820 696e 2074 6865 204f  me path in the O
+000191e0: 626a 6563 7420 5374 6f72 6520 666f 6c64  bject Store fold
+000191f0: 6572 2c20 6669 6c65 7320 7769 6c6c 2062  er, files will b
+00019200: 6520 6f76 6572 7772 6974 7465 6e2e 0a0a  e overwritten...
+00019210: 4669 6c65 7320 696e 2064 6972 6563 746f  Files in directo
+00019220: 7269 6573 206d 6179 2062 6520 7265 6375  ries may be recu
+00019230: 7273 6976 656c 7920 7570 6c6f 6164 6564  rsively uploaded
+00019240: 2075 7369 6e67 2074 6865 2060 2d2d 7265   using the `--re
+00019250: 6375 7273 6976 6560 206f 7220 602d 7260  cursive` or `-r`
+00019260: 206f 7074 696f 6e2c 2065 2e67 2e3a 0a0a   option, e.g.:..
+00019270: 6060 6073 6865 6c6c 0a79 642d 7570 6c6f  ```shell.yd-uplo
+00019280: 6164 202d 2d64 6972 6563 746f 7279 206d  ad --directory m
+00019290: 795f 776f 726b 5f72 6571 7569 7265 6d65  y_work_requireme
+000192a0: 6e74 202d 7220 6d79 6469 7220 6d79 6f74  nt -r mydir myot
+000192b0: 6865 7264 6972 0a60 6060 0a0a 546f 2075  herdir.```..To u
+000192c0: 706c 6f61 6420 746f 206f 7468 6572 206e  pload to other n
+000192d0: 616d 6573 7061 6365 732c 2075 7365 2074  amespaces, use t
+000192e0: 6865 2060 2d2d 6e61 6d65 7370 6163 6560  he `--namespace`
+000192f0: 2f60 2d6e 6020 6f70 7469 6f6e 2e0a 0a23  /`-n` option...#
+00019300: 2320 7964 2d73 6875 7464 6f77 6e0a 0a54  # yd-shutdown..T
+00019310: 6865 2060 7964 2d73 6875 7464 6f77 6e60  he `yd-shutdown`
+00019320: 2063 6f6d 6d61 6e64 2073 6875 7473 2064   command shuts d
+00019330: 6f77 6e20 576f 726b 6572 2050 6f6f 6c73  own Worker Pools
+00019340: 2074 6861 7420 6d61 7463 6820 7468 6520   that match the 
+00019350: 606e 616d 6573 7061 6365 6020 616e 6420  `namespace` and 
+00019360: 6074 6167 6020 666f 756e 6420 696e 2074  `tag` found in t
+00019370: 6865 2063 6f6e 6669 6775 7261 7469 6f6e  he configuration
+00019380: 2066 696c 652e 2041 6c6c 2072 656d 6169   file. All remai
+00019390: 6e69 6e67 2077 6f72 6b20 7769 6c6c 2062  ning work will b
+000193a0: 6520 6361 6e63 656c 6c65 642c 2062 7574  e cancelled, but
+000193b0: 2063 7572 7265 6e74 6c79 2065 7865 6375   currently execu
+000193c0: 7469 6e67 2054 6173 6b73 2077 696c 6c20  ting Tasks will 
+000193d0: 6265 2061 6c6c 6f77 6564 2074 6f20 636f  be allowed to co
+000193e0: 6d70 6c65 7465 2c20 6166 7465 7220 7768  mplete, after wh
+000193f0: 6963 6820 7468 6520 436f 6d70 7574 6520  ich the Compute 
+00019400: 5265 7175 6972 656d 656e 7420 7769 6c6c  Requirement will
+00019410: 2062 6520 7465 726d 696e 6174 6564 2e0a   be terminated..
+00019420: 0a23 2320 7964 2d69 6e73 7461 6e74 6961  .## yd-instantia
+00019430: 7465 0a0a 5468 6520 6079 642d 696e 7374  te..The `yd-inst
+00019440: 616e 7469 6174 6560 2063 6f6d 6d61 6e64  antiate` command
+00019450: 2069 6e73 7461 6e74 6961 7465 7320 6120   instantiates a 
+00019460: 436f 6d70 7574 6520 5265 7175 6972 656d  Compute Requirem
+00019470: 656e 7420 2869 2e65 2e2c 2061 2073 6574  ent (i.e., a set
+00019480: 206f 6620 696e 7374 616e 6365 7320 7468   of instances th
+00019490: 6174 2061 7265 206d 616e 6167 6564 2062  at are managed b
+000194a0: 7920 7468 6569 7220 6372 6561 746f 7220  y their creator 
+000194b0: 616e 6420 646f 206e 6f74 2061 7574 6f6d  and do not autom
+000194c0: 6174 6963 616c 6c79 2062 6563 6f6d 6520  atically become 
+000194d0: 7061 7274 206f 6620 6120 5965 6c6c 6f77  part of a Yellow
+000194e0: 446f 6720 576f 726b 6572 2050 6f6f 6c29  Dog Worker Pool)
+000194f0: 2e0a 0a54 6869 7320 636f 6d6d 616e 6420  ...This command 
+00019500: 7573 6573 2074 6865 2064 6174 6120 6672  uses the data fr
+00019510: 6f6d 2074 6865 2060 776f 726b 6572 506f  om the `workerPo
+00019520: 6f6c 6020 636f 6e66 6967 7572 6174 696f  ol` configuratio
+00019530: 6e20 7365 6374 696f 6e2c 2062 7574 206f  n section, but o
+00019540: 6e6c 7920 7573 6573 2074 6865 2060 6e61  nly uses the `na
+00019550: 6d65 602c 2060 7465 6d70 6c61 7465 4964  me`, `templateId
+00019560: 602c 2060 7461 7267 6574 496e 7374 616e  `, `targetInstan
+00019570: 6365 436f 756e 7460 2c20 6069 6e73 7461  ceCount`, `insta
+00019580: 6e63 6554 6167 7360 2c20 6075 7365 7244  nceTags`, `userD
+00019590: 6174 6160 2c20 616e 6420 6069 6d61 6765  ata`, and `image
+000195a0: 7349 6460 2070 726f 7065 7274 6965 732e  sId` properties.
+000195b0: 2049 6e20 6164 6469 7469 6f6e 2c20 7468   In addition, th
+000195c0: 6520 426f 6f6c 6561 6e20 7072 6f70 6572  e Boolean proper
+000195d0: 7479 2060 6d61 696e 7461 696e 496e 7374  ty `maintainInst
+000195e0: 616e 6365 436f 756e 7460 2028 6465 6661  anceCount` (defa
+000195f0: 756c 7420 3d20 6066 616c 7365 6029 2069  ult = `false`) i
+00019600: 7320 6176 6169 6c61 626c 6520 666f 7220  s available for 
+00019610: 7573 6520 7769 7468 2060 7964 2d69 6e73  use with `yd-ins
+00019620: 7461 6e74 6961 7465 602e 0a0a 436f 6d70  tantiate`...Comp
+00019630: 7574 6520 5265 7175 6972 656d 656e 7473  ute Requirements
+00019640: 2063 616e 2062 6520 696e 7374 616e 7469   can be instanti
+00019650: 6174 6564 2064 6972 6563 746c 7920 6672  ated directly fr
+00019660: 6f6d 204a 534f 4e20 286f 7220 4a73 6f6e  om JSON (or Json
+00019670: 6e65 7429 2073 7065 6369 6669 6361 7469  net) specificati
+00019680: 6f6e 732c 2075 7369 6e67 2074 6865 2060  ons, using the `
+00019690: 2d2d 636f 6d70 7574 652d 7265 7175 6972  --compute-requir
+000196a0: 656d 656e 7460 2028 6f72 2060 2d43 6029  ement` (or `-C`)
+000196b0: 2063 6f6d 6d61 6e64 206c 696e 6520 6f70   command line op
+000196c0: 7469 6f6e 2c20 666f 6c6c 6f77 6564 2062  tion, followed b
+000196d0: 7920 7468 6520 6669 6c65 6e61 6d65 2e20  y the filename. 
+000196e0: 5468 6520 7072 6f70 6572 7469 6573 206c  The properties l
+000196f0: 6973 7465 6420 6162 6f76 6520 7769 6c6c  isted above will
+00019700: 2062 6520 696e 6865 7269 7465 6420 6672   be inherited fr
+00019710: 6f6d 2074 6865 2063 6f6e 6669 672e 746f  om the config.to
+00019720: 6d6c 2060 776f 726b 6572 506f 6f6c 6020  ml `workerPool` 
+00019730: 7370 6563 6966 6963 6174 696f 6e20 6966  specification if
+00019740: 2074 6865 7920 6172 6520 6e6f 7420 7072   they are not pr
+00019750: 6573 656e 7420 696e 2074 6865 204a 534f  esent in the JSO
+00019760: 4e20 6669 6c65 2e20 416e 2065 7861 6d70  N file. An examp
+00019770: 6c65 204a 534f 4e20 7370 6563 6966 6963  le JSON specific
+00019780: 6174 696f 6e20 6973 2073 686f 776e 2062  ation is shown b
+00019790: 656c 6f77 3a0a 0a60 6060 6a73 6f6e 0a7b  elow:..```json.{
+000197a0: 0a20 2022 696d 6167 6573 4964 223a 2022  .  "imagesId": "
+000197b0: 7964 6964 3a69 6d67 6661 6d3a 3030 3030  ydid:imgfam:0000
+000197c0: 3030 3a34 3139 3632 3539 322d 3537 3763  00:41962592-577c
+000197d0: 2d34 6664 652d 6162 3033 2d64 3835 3234  -4fde-ab03-d8524
+000197e0: 3635 6537 6638 6222 2c0a 2020 2269 6e73  65e7f8b",.  "ins
+000197f0: 7461 6e63 6554 6167 7322 3a20 7b22 6131  tanceTags": {"a1
+00019800: 223a 2022 6f6e 6522 2c20 2261 3222 3a20  ": "one", "a2": 
+00019810: 2274 776f 227d 2c0a 2020 2272 6571 7569  "two"},.  "requi
+00019820: 7265 6d65 6e74 4e61 6d65 223a 2022 6372  rementName": "cr
+00019830: 5f74 6573 745f 7b7b 6461 7465 7469 6d65  _test_{{datetime
+00019840: 7d7d 222c 0a20 2022 7265 7175 6972 656d  }}",.  "requirem
+00019850: 656e 744e 616d 6573 7061 6365 223a 2022  entNamespace": "
+00019860: 7079 6578 616d 706c 6573 222c 0a20 2022  pyexamples",.  "
+00019870: 7265 7175 6972 656d 656e 7454 6167 223a  requirementTag":
+00019880: 2022 7079 6578 616d 706c 6573 2d74 6573   "pyexamples-tes
+00019890: 7422 2c0a 2020 2274 656d 706c 6174 6549  t",.  "templateI
+000198a0: 6422 3a20 2279 6469 643a 6372 743a 3030  d": "ydid:crt:00
+000198b0: 3030 3030 3a32 3330 6539 6134 322d 3937  0000:230e9a42-97
+000198c0: 6462 2d34 6436 392d 6161 3931 2d32 3966  db-4d69-aa91-29f
+000198d0: 6633 3039 3935 3162 3422 2c0a 2020 2275  f309951b4",.  "u
+000198e0: 7365 7244 6174 6122 3a20 2223 2f62 696e  serData": "#/bin
+000198f0: 2f62 6173 685c 6e23 4f74 6865 7220 7374  /bash\n#Other st
+00019900: 7566 662e 2e2e 222c 0a20 2022 7461 7267  uff...",.  "targ
+00019910: 6574 496e 7374 616e 6365 436f 756e 7422  etInstanceCount"
+00019920: 3a20 312c 0a20 2022 6d61 696e 7461 696e  : 1,.  "maintain
+00019930: 496e 7374 616e 6365 436f 756e 7422 3a20  InstanceCount": 
+00019940: 7472 7565 0a7d 0a60 6060 0a0a 4966 2061  true.}.```..If a
+00019950: 2057 6f72 6b65 7220 506f 6f6c 2069 7320   Worker Pool is 
+00019960: 6465 6669 6e65 642c 2075 7369 6e67 2060  defined, using `
+00019970: 776f 726b 6572 506f 6f6c 4461 7461 6020  workerPoolData` 
+00019980: 696e 2074 6865 2063 6f6e 6669 6775 7261  in the configura
+00019990: 7469 6f6e 2066 696c 6520 6f72 2062 7920  tion file or by 
+000199a0: 7573 696e 6720 7468 6520 602d 2d77 6f72  using the `--wor
+000199b0: 6b65 722d 706f 6f6c 6020 286f 7220 602d  ker-pool` (or `-
+000199c0: 7060 2920 6f70 7469 6f6e 2c20 6079 642d  p`) option, `yd-
+000199d0: 696e 7374 616e 7469 6174 6560 2077 696c  instantiate` wil
+000199e0: 6c20 6578 7472 6163 7420 7468 6520 436f  l extract the Co
+000199f0: 6d70 7574 6520 5265 7175 6972 656d 656e  mpute Requiremen
+00019a00: 7420 6672 6f6d 2074 6865 2057 6f72 6b65  t from the Worke
+00019a10: 7220 506f 6f6c 2073 7065 6369 6669 6361  r Pool specifica
+00019a20: 7469 6f6e 2028 6967 6e6f 7269 6e67 2057  tion (ignoring W
+00019a30: 6f72 6b65 722d 506f 6f6c 2d73 7065 6369  orker-Pool-speci
+00019a40: 6669 6320 6461 7461 292c 2061 6e64 2075  fic data), and u
+00019a50: 7365 2074 6861 7420 666f 7220 696e 7374  se that for inst
+00019a60: 616e 7469 6174 696e 6720 7468 6520 436f  antiating the Co
+00019a70: 6d70 7574 6520 5265 7175 6972 656d 656e  mpute Requiremen
+00019a80: 742e 0a0a 5573 6520 7468 6520 602d 2d64  t...Use the `--d
+00019a90: 7279 2d72 756e 6020 6f70 7469 6f6e 2074  ry-run` option t
+00019aa0: 6f20 696e 7370 6563 7420 7468 6520 6465  o inspect the de
+00019ab0: 7461 696c 7320 6f66 2074 6865 2043 6f6d  tails of the Com
+00019ac0: 7075 7465 2052 6571 7569 7265 6d65 6e74  pute Requirement
+00019ad0: 2073 7065 6369 6669 6361 7469 6f6e 2074   specification t
+00019ae0: 6861 7420 7769 6c6c 2062 6520 7375 626d  hat will be subm
+00019af0: 6974 7465 642c 2069 6e20 4a53 4f4e 2066  itted, in JSON f
+00019b00: 6f72 6d61 742e 2054 6865 204a 534f 4e20  ormat. The JSON 
+00019b10: 6f75 7470 7574 206f 6620 7468 6973 2063  output of this c
+00019b20: 6f6d 6d61 6e64 2063 616e 2062 6520 7573  ommand can be us
+00019b30: 6564 2077 6974 6820 7468 6520 602d 4360  ed with the `-C`
+00019b40: 206f 7074 696f 6e20 6162 6f76 6520 286f   option above (o
+00019b50: 7220 7769 7468 2060 2d70 6020 666f 7220  r with `-p` for 
+00019b60: 576f 726b 6572 2050 6f6f 6c20 7370 6563  Worker Pool spec
+00019b70: 6966 6963 6174 696f 6e73 292e 0a0a 2323  ifications)...##
+00019b80: 2320 5465 7374 2d52 756e 6e69 6e67 2061  # Test-Running a
+00019b90: 2044 796e 616d 6963 2054 656d 706c 6174   Dynamic Templat
+00019ba0: 650a 0a57 6865 6e20 6120 7468 6520 6074  e..When a the `t
+00019bb0: 656d 706c 6174 6549 6460 206f 6620 6120  emplateId` of a 
+00019bc0: 4479 6e61 6d69 6320 5265 7175 6972 656d  Dynamic Requirem
+00019bd0: 656e 7420 6973 2075 7365 642c 2074 6865  ent is used, the
+00019be0: 2060 7964 2d69 6e73 7461 6e74 6961 7465   `yd-instantiate
+00019bf0: 6020 636f 6d6d 616e 6420 6361 6e20 6265  ` command can be
+00019c00: 2075 7365 6420 746f 2072 6570 6f72 7420   used to report 
+00019c10: 6f6e 2061 2074 6573 7420 7275 6e20 6f66  on a test run of
+00019c20: 2074 6865 2054 656d 706c 6174 652c 2075   the Template, u
+00019c30: 7369 6e67 2074 6865 2060 2d2d 7265 706f  sing the `--repo
+00019c40: 7274 6020 286f 7220 602d 7260 2920 636f  rt` (or `-r`) co
+00019c50: 6d6d 616e 6420 6c69 6e65 206f 7074 696f  mmand line optio
+00019c60: 6e2e 2054 6869 7320 6361 6e20 6265 2075  n. This can be u
+00019c70: 7365 6420 7769 7468 2054 4f4d 4c2d 6465  sed with TOML-de
+00019c80: 6669 6e65 6420 436f 6d70 7574 6520 5265  fined Compute Re
+00019c90: 7175 6972 656d 656e 7420 7370 6563 6966  quirement specif
+00019ca0: 6963 6174 696f 6e73 2c20 6275 7420 6e6f  ications, but no
+00019cb0: 7420 7468 6f73 6520 7468 6174 2061 7265  t those that are
+00019cc0: 204a 534f 4e2d 6465 6669 6e65 642e 0a0a   JSON-defined...
+00019cd0: 4e6f 2069 6e73 7461 6e63 6573 2077 696c  No instances wil
+00019ce0: 6c20 6265 2070 726f 7669 7369 6f6e 6564  l be provisioned
+00019cf0: 2064 7572 696e 6720 7468 6520 7465 7374   during the test
+00019d00: 2072 756e 2e0a 0a46 6f72 2065 7861 6d70   run...For examp
+00019d10: 6c65 3a0a 0a60 6060 7368 656c 6c0a 2520  le:..```shell.% 
+00019d20: 7964 2d69 6e73 7461 6e74 6961 7465 202d  yd-instantiate -
+00019d30: 2d72 6570 6f72 7420 2d2d 7175 6965 740a  -report --quiet.
+00019d40: 0ae2 948c e294 80e2 9480 e294 80e2 9480  ................
+00019d50: e294 ace2 9480 e294 80e2 9480 e294 80e2  ................
+00019d60: 9480 e294 80e2 9480 e294 80e2 94ac e294  ................
 00019d70: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00019d80: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00019d90: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00019da0: 80e2 9480 e294 a40a e294 8220 2033 20e2  ...........  3 .
-00019db0: 9482 2020 2020 2020 3320 e294 8220 4157  ..      3 ... AW
-00019dc0: 5320 2020 2020 2020 20e2 9482 2041 7773  S        ... Aws
-00019dd0: 5370 6f74 436f 6d70 7574 6553 6f75 7263  SpotComputeSourc
-00019de0: 6520 e294 8220 6575 2d77 6573 742d 3220  e ... eu-west-2 
-00019df0: e294 8220 7433 612e 736d 616c 6c20 2020  ... t3a.small   
-00019e00: 2020 20e2 9482 2061 7773 7370 6f74 2d65     ... awsspot-e
-00019e10: 752d 7765 7374 2d32 20e2 9482 0ae2 949c  u-west-2 .......
-00019e20: e294 80e2 9480 e294 80e2 9480 e294 bce2  ................
-00019e30: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00019e40: 80e2 9480 e294 80e2 94bc e294 80e2 9480  ................
-00019e50: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00019e60: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00019e70: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00019e80: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00019e90: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00019ea0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00019eb0: e294 80e2 94bc e294 80e2 9480 e294 80e2  ................
-00019ec0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00019ed0: 80e2 9480 e294 80e2 94bc e294 80e2 9480  ................
-00019ee0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00019ef0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00019f00: 80e2 9480 e294 80e2 9480 e294 bce2 9480  ................
+00019d90: 9480 e294 ace2 9480 e294 80e2 9480 e294  ................
+00019da0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00019db0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00019dc0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00019dd0: 80e2 9480 e294 80e2 94ac e294 80e2 9480  ................
+00019de0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00019df0: 9480 e294 80e2 9480 e294 80e2 94ac e294  ................
+00019e00: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00019e10: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00019e20: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00019e30: ace2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00019e40: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00019e50: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00019e60: 80e2 9480 e294 80e2 9480 e294 900a e294  ................
+00019e70: 8220 2020 20e2 9482 2020 2052 616e 6b20  .    ...   Rank 
+00019e80: e294 8220 5072 6f76 6964 6572 2020 20e2  ... Provider   .
+00019e90: 9482 2054 7970 6520 2020 2020 2020 2020  .. Type         
+00019ea0: 2020 2020 2020 2020 e294 8220 5265 6769          ... Regi
+00019eb0: 6f6e 2020 2020 e294 8220 496e 7374 616e  on    ... Instan
+00019ec0: 6365 5479 7065 2020 20e2 9482 2053 6f75  ceType   ... Sou
+00019ed0: 7263 6520 4e61 6d65 2020 2020 2020 20e2  rce Name       .
+00019ee0: 9482 0ae2 949c e294 80e2 9480 e294 80e2  ................
+00019ef0: 9480 e294 bce2 9480 e294 80e2 9480 e294  ................
+00019f00: 80e2 9480 e294 80e2 9480 e294 80e2 94bc  ................
 00019f10: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 00019f20: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00019f30: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00019f40: e294 80e2 9480 e294 a40a e294 8220 2034  .............  4
-00019f50: 20e2 9482 2020 2020 2020 3420 e294 8220   ...      4 ... 
-00019f60: 4157 5320 2020 2020 2020 20e2 9482 2041  AWS        ... A
-00019f70: 7773 5370 6f74 436f 6d70 7574 6553 6f75  wsSpotComputeSou
-00019f80: 7263 6520 e294 8220 6575 2d77 6573 742d  rce ... eu-west-
-00019f90: 3220 e294 8220 6335 612e 6c61 7267 6520  2 ... c5a.large 
-00019fa0: 2020 2020 20e2 9482 2061 7773 7370 6f74       ... awsspot
-00019fb0: 2d65 752d 7765 7374 2d32 20e2 9482 0ae2  -eu-west-2 .....
-00019fc0: 949c e294 80e2 9480 e294 80e2 9480 e294  ................
-00019fd0: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
-00019fe0: e294 80e2 9480 e294 80e2 94bc e294 80e2  ................
-00019ff0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a000: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a010: e294 bce2 9480 e294 80e2 9480 e294 80e2  ................
-0001a020: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a030: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a040: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a050: 9480 e294 80e2 94bc e294 80e2 9480 e294  ................
-0001a060: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a070: e294 80e2 9480 e294 80e2 94bc e294 80e2  ................
-0001a080: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a090: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a0a0: e294 80e2 9480 e294 80e2 9480 e294 bce2  ................
-0001a0b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00019f30: 80e2 9480 e294 bce2 9480 e294 80e2 9480  ................
+00019f40: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00019f50: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00019f60: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00019f70: e294 80e2 9480 e294 80e2 94bc e294 80e2  ................
+00019f80: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00019f90: 80e2 9480 e294 80e2 9480 e294 80e2 94bc  ................
+00019fa0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00019fb0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00019fc0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00019fd0: e294 bce2 9480 e294 80e2 9480 e294 80e2  ................
+00019fe0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00019ff0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a000: e294 80e2 9480 e294 80e2 9480 e294 a40a  ................
+0001a010: e294 8220 2031 20e2 9482 2020 2020 2020  ...  1 ...      
+0001a020: 3120 e294 8220 4157 5320 2020 2020 2020  1 ... AWS       
+0001a030: 20e2 9482 2041 7773 5370 6f74 436f 6d70   ... AwsSpotComp
+0001a040: 7574 6553 6f75 7263 6520 e294 8220 6575  uteSource ... eu
+0001a050: 2d77 6573 742d 3220 e294 8220 7433 612e  -west-2 ... t3a.
+0001a060: 6e61 6e6f 2020 2020 2020 20e2 9482 2061  nano       ... a
+0001a070: 7773 7370 6f74 2d65 752d 7765 7374 2d32  wsspot-eu-west-2
+0001a080: 20e2 9482 0ae2 949c e294 80e2 9480 e294   ...............
+0001a090: 80e2 9480 e294 bce2 9480 e294 80e2 9480  ................
+0001a0a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a0b0: 94bc e294 80e2 9480 e294 80e2 9480 e294  ................
 0001a0c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a0d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a0e0: 9480 e294 80e2 9480 e294 a40a e294 8220  ............... 
-0001a0f0: 2035 20e2 9482 2020 2020 2020 3420 e294   5 ...      4 ..
-0001a100: 8220 4157 5320 2020 2020 2020 20e2 9482  . AWS        ...
-0001a110: 2041 7773 5370 6f74 436f 6d70 7574 6553   AwsSpotComputeS
-0001a120: 6f75 7263 6520 e294 8220 6575 2d77 6573  ource ... eu-wes
-0001a130: 742d 3220 e294 8220 6336 612e 6c61 7267  t-2 ... c6a.larg
-0001a140: 6520 2020 2020 20e2 9482 2061 7773 7370  e      ... awssp
-0001a150: 6f74 2d65 752d 7765 7374 2d32 20e2 9482  ot-eu-west-2 ...
-0001a160: 0ae2 949c e294 80e2 9480 e294 80e2 9480  ................
-0001a170: e294 bce2 9480 e294 80e2 9480 e294 80e2  ................
-0001a180: 9480 e294 80e2 9480 e294 80e2 94bc e294  ................
-0001a190: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a1a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a1b0: 9480 e294 bce2 9480 e294 80e2 9480 e294  ................
-0001a1c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a1d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a1e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a1f0: 80e2 9480 e294 80e2 94bc e294 80e2 9480  ................
-0001a200: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a210: 9480 e294 80e2 9480 e294 80e2 94bc e294  ................
-0001a220: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a230: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a0d0: e294 80e2 9480 e294 bce2 9480 e294 80e2  ................
+0001a0e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a0f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a100: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a110: 9480 e294 80e2 9480 e294 80e2 94bc e294  ................
+0001a120: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a130: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a140: 94bc e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a150: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a160: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a170: 9480 e294 bce2 9480 e294 80e2 9480 e294  ................
+0001a180: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a190: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a1a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a1b0: a40a e294 8220 2032 20e2 9482 2020 2020  .....  2 ...    
+0001a1c0: 2020 3220 e294 8220 4157 5320 2020 2020    2 ... AWS     
+0001a1d0: 2020 20e2 9482 2041 7773 5370 6f74 436f     ... AwsSpotCo
+0001a1e0: 6d70 7574 6553 6f75 7263 6520 e294 8220  mputeSource ... 
+0001a1f0: 6575 2d77 6573 742d 3220 e294 8220 7433  eu-west-2 ... t3
+0001a200: 612e 6d69 6372 6f20 2020 2020 20e2 9482  a.micro      ...
+0001a210: 2061 7773 7370 6f74 2d65 752d 7765 7374   awsspot-eu-west
+0001a220: 2d32 20e2 9482 0ae2 949c e294 80e2 9480  -2 .............
+0001a230: e294 80e2 9480 e294 bce2 9480 e294 80e2  ................
 0001a240: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a250: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a250: 80e2 94bc e294 80e2 9480 e294 80e2 9480  ................
 0001a260: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a270: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a280: 80e2 9480 e294 80e2 9480 e294 a40a e294  ................
-0001a290: 8220 2036 20e2 9482 2020 2020 2020 3420  .  6 ...      4 
-0001a2a0: e294 8220 4157 5320 2020 2020 2020 20e2  ... AWS        .
-0001a2b0: 9482 2041 7773 5370 6f74 436f 6d70 7574  .. AwsSpotComput
-0001a2c0: 6553 6f75 7263 6520 e294 8220 6575 2d77  eSource ... eu-w
-0001a2d0: 6573 742d 3220 e294 8220 7433 612e 6d65  est-2 ... t3a.me
-0001a2e0: 6469 756d 2020 2020 20e2 9482 2061 7773  dium     ... aws
-0001a2f0: 7370 6f74 2d65 752d 7765 7374 2d32 20e2  spot-eu-west-2 .
-0001a300: 9482 0ae2 949c e294 80e2 9480 e294 80e2  ................
-0001a310: 9480 e294 bce2 9480 e294 80e2 9480 e294  ................
-0001a320: 80e2 9480 e294 80e2 9480 e294 80e2 94bc  ................
-0001a330: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a340: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a350: 80e2 9480 e294 bce2 9480 e294 80e2 9480  ................
-0001a360: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a370: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a380: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a390: e294 80e2 9480 e294 80e2 94bc e294 80e2  ................
-0001a3a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a3b0: 80e2 9480 e294 80e2 9480 e294 80e2 94bc  ................
-0001a3c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a3d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a270: 9480 e294 80e2 9480 e294 bce2 9480 e294  ................
+0001a280: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a290: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a2a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a2b0: 80e2 9480 e294 80e2 9480 e294 80e2 94bc  ................
+0001a2c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a2d0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a2e0: 80e2 94bc e294 80e2 9480 e294 80e2 9480  ................
+0001a2f0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a300: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a310: 80e2 9480 e294 bce2 9480 e294 80e2 9480  ................
+0001a320: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a330: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a340: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a350: e294 a40a e294 8220 2033 20e2 9482 2020  .......  3 ...  
+0001a360: 2020 2020 3320 e294 8220 4157 5320 2020      3 ... AWS   
+0001a370: 2020 2020 20e2 9482 2041 7773 5370 6f74       ... AwsSpot
+0001a380: 436f 6d70 7574 6553 6f75 7263 6520 e294  ComputeSource ..
+0001a390: 8220 6575 2d77 6573 742d 3220 e294 8220  . eu-west-2 ... 
+0001a3a0: 7433 612e 736d 616c 6c20 2020 2020 20e2  t3a.small      .
+0001a3b0: 9482 2061 7773 7370 6f74 2d65 752d 7765  .. awsspot-eu-we
+0001a3c0: 7374 2d32 20e2 9482 0ae2 949c e294 80e2  st-2 ...........
+0001a3d0: 9480 e294 80e2 9480 e294 bce2 9480 e294  ................
 0001a3e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a3f0: e294 bce2 9480 e294 80e2 9480 e294 80e2  ................
+0001a3f0: e294 80e2 94bc e294 80e2 9480 e294 80e2  ................
 0001a400: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a410: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a420: e294 80e2 9480 e294 80e2 9480 e294 a40a  ................
-0001a430: e294 8220 2037 20e2 9482 2020 2020 2020  ...  7 ...      
-0001a440: 3520 e294 8220 4157 5320 2020 2020 2020  5 ... AWS       
-0001a450: 20e2 9482 2041 7773 5370 6f74 436f 6d70   ... AwsSpotComp
-0001a460: 7574 6553 6f75 7263 6520 e294 8220 6575  uteSource ... eu
-0001a470: 2d77 6573 742d 3220 e294 8220 6d35 612e  -west-2 ... m5a.
-0001a480: 6c61 7267 6520 2020 2020 20e2 9482 2061  large      ... a
-0001a490: 7773 7370 6f74 2d65 752d 7765 7374 2d32  wsspot-eu-west-2
-0001a4a0: 20e2 9482 0ae2 949c e294 80e2 9480 e294   ...............
-0001a4b0: 80e2 9480 e294 bce2 9480 e294 80e2 9480  ................
-0001a4c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a4d0: 94bc e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a4e0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a4f0: e294 80e2 9480 e294 bce2 9480 e294 80e2  ................
-0001a500: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a510: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a520: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a530: 9480 e294 80e2 9480 e294 80e2 94bc e294  ................
-0001a540: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a550: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a560: 94bc e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a570: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a410: 80e2 9480 e294 80e2 9480 e294 bce2 9480  ................
+0001a420: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a430: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a440: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a450: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a460: 94bc e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a470: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a480: e294 80e2 94bc e294 80e2 9480 e294 80e2  ................
+0001a490: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a4a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a4b0: e294 80e2 9480 e294 bce2 9480 e294 80e2  ................
+0001a4c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a4d0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a4e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a4f0: 9480 e294 a40a e294 8220 2034 20e2 9482  .........  4 ...
+0001a500: 2020 2020 2020 3420 e294 8220 4157 5320        4 ... AWS 
+0001a510: 2020 2020 2020 20e2 9482 2041 7773 5370         ... AwsSp
+0001a520: 6f74 436f 6d70 7574 6553 6f75 7263 6520  otComputeSource 
+0001a530: e294 8220 6575 2d77 6573 742d 3220 e294  ... eu-west-2 ..
+0001a540: 8220 6335 612e 6c61 7267 6520 2020 2020  . c5a.large     
+0001a550: 20e2 9482 2061 7773 7370 6f74 2d65 752d   ... awsspot-eu-
+0001a560: 7765 7374 2d32 20e2 9482 0ae2 949c e294  west-2 .........
+0001a570: 80e2 9480 e294 80e2 9480 e294 bce2 9480  ................
 0001a580: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a590: 9480 e294 bce2 9480 e294 80e2 9480 e294  ................
+0001a590: 9480 e294 80e2 94bc e294 80e2 9480 e294  ................
 0001a5a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a5b0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a5b0: e294 80e2 9480 e294 80e2 9480 e294 bce2  ................
 0001a5c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a5d0: a40a e294 8220 2038 20e2 9482 2020 2020  .....  8 ...    
-0001a5e0: 2020 3520 e294 8220 4157 5320 2020 2020    5 ... AWS     
-0001a5f0: 2020 20e2 9482 2041 7773 5370 6f74 436f     ... AwsSpotCo
-0001a600: 6d70 7574 6553 6f75 7263 6520 e294 8220  mputeSource ... 
-0001a610: 6575 2d77 6573 742d 3220 e294 8220 6d35  eu-west-2 ... m5
-0001a620: 6164 2e6c 6172 6765 2020 2020 20e2 9482  ad.large     ...
-0001a630: 2061 7773 7370 6f74 2d65 752d 7765 7374   awsspot-eu-west
-0001a640: 2d32 20e2 9482 0ae2 949c e294 80e2 9480  -2 .............
-0001a650: e294 80e2 9480 e294 bce2 9480 e294 80e2  ................
-0001a660: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a670: 80e2 94bc e294 80e2 9480 e294 80e2 9480  ................
-0001a680: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a690: 9480 e294 80e2 9480 e294 bce2 9480 e294  ................
-0001a6a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a6b0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a6c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a6d0: 80e2 9480 e294 80e2 9480 e294 80e2 94bc  ................
-0001a6e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a6f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a700: 80e2 94bc e294 80e2 9480 e294 80e2 9480  ................
-0001a710: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a5d0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a5e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a5f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a600: 80e2 94bc e294 80e2 9480 e294 80e2 9480  ................
+0001a610: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a620: 9480 e294 80e2 94bc e294 80e2 9480 e294  ................
+0001a630: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a640: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a650: 9480 e294 80e2 9480 e294 bce2 9480 e294  ................
+0001a660: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a670: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a680: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a690: 80e2 9480 e294 a40a e294 8220 2035 20e2  ...........  5 .
+0001a6a0: 9482 2020 2020 2020 3420 e294 8220 4157  ..      4 ... AW
+0001a6b0: 5320 2020 2020 2020 20e2 9482 2041 7773  S        ... Aws
+0001a6c0: 5370 6f74 436f 6d70 7574 6553 6f75 7263  SpotComputeSourc
+0001a6d0: 6520 e294 8220 6575 2d77 6573 742d 3220  e ... eu-west-2 
+0001a6e0: e294 8220 6336 612e 6c61 7267 6520 2020  ... c6a.large   
+0001a6f0: 2020 20e2 9482 2061 7773 7370 6f74 2d65     ... awsspot-e
+0001a700: 752d 7765 7374 2d32 20e2 9482 0ae2 949c  u-west-2 .......
+0001a710: e294 80e2 9480 e294 80e2 9480 e294 bce2  ................
 0001a720: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a730: 80e2 9480 e294 bce2 9480 e294 80e2 9480  ................
+0001a730: 80e2 9480 e294 80e2 94bc e294 80e2 9480  ................
 0001a740: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
 0001a750: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a760: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a770: e294 a40a e294 8220 2039 20e2 9482 2020  .......  9 ...  
-0001a780: 2020 2020 3520 e294 8220 4157 5320 2020      5 ... AWS   
-0001a790: 2020 2020 20e2 9482 2041 7773 5370 6f74       ... AwsSpot
-0001a7a0: 436f 6d70 7574 6553 6f75 7263 6520 e294  ComputeSource ..
-0001a7b0: 8220 6575 2d77 6573 742d 3220 e294 8220  . eu-west-2 ... 
-0001a7c0: 6d36 612e 6c61 7267 6520 2020 2020 20e2  m6a.large      .
-0001a7d0: 9482 2061 7773 7370 6f74 2d65 752d 7765  .. awsspot-eu-we
-0001a7e0: 7374 2d32 20e2 9482 0ae2 949c e294 80e2  st-2 ...........
-0001a7f0: 9480 e294 80e2 9480 e294 bce2 9480 e294  ................
-0001a800: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a810: e294 80e2 94bc e294 80e2 9480 e294 80e2  ................
-0001a820: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a830: 80e2 9480 e294 80e2 9480 e294 bce2 9480  ................
-0001a840: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a850: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a860: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a870: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a880: 94bc e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a890: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a8a0: e294 80e2 94bc e294 80e2 9480 e294 80e2  ................
-0001a8b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a8c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a8d0: e294 80e2 9480 e294 bce2 9480 e294 80e2  ................
+0001a760: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a770: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a780: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a790: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a7a0: e294 80e2 94bc e294 80e2 9480 e294 80e2  ................
+0001a7b0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a7c0: 80e2 9480 e294 80e2 94bc e294 80e2 9480  ................
+0001a7d0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a7e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a7f0: 80e2 9480 e294 80e2 9480 e294 bce2 9480  ................
+0001a800: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a810: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a820: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a830: e294 80e2 9480 e294 a40a e294 8220 2036  .............  6
+0001a840: 20e2 9482 2020 2020 2020 3420 e294 8220   ...      4 ... 
+0001a850: 4157 5320 2020 2020 2020 20e2 9482 2041  AWS        ... A
+0001a860: 7773 5370 6f74 436f 6d70 7574 6553 6f75  wsSpotComputeSou
+0001a870: 7263 6520 e294 8220 6575 2d77 6573 742d  rce ... eu-west-
+0001a880: 3220 e294 8220 7433 612e 6d65 6469 756d  2 ... t3a.medium
+0001a890: 2020 2020 20e2 9482 2061 7773 7370 6f74       ... awsspot
+0001a8a0: 2d65 752d 7765 7374 2d32 20e2 9482 0ae2  -eu-west-2 .....
+0001a8b0: 949c e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a8c0: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a8d0: e294 80e2 9480 e294 80e2 94bc e294 80e2  ................
 0001a8e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
 0001a8f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a900: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a910: 9480 e294 a40a e294 8220 3130 20e2 9482  ......... 10 ...
-0001a920: 2020 2020 2020 3520 e294 8220 4157 5320        5 ... AWS 
-0001a930: 2020 2020 2020 20e2 9482 2041 7773 5370         ... AwsSp
-0001a940: 6f74 436f 6d70 7574 6553 6f75 7263 6520  otComputeSource 
-0001a950: e294 8220 6575 2d77 6573 742d 3220 e294  ... eu-west-2 ..
-0001a960: 8220 7433 612e 6c61 7267 6520 2020 2020  . t3a.large     
-0001a970: 20e2 9482 2061 7773 7370 6f74 2d65 752d   ... awsspot-eu-
-0001a980: 7765 7374 2d32 20e2 9482 0ae2 9494 e294  west-2 .........
-0001a990: 80e2 9480 e294 80e2 9480 e294 b4e2 9480  ................
-0001a9a0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001a9b0: 9480 e294 80e2 94b4 e294 80e2 9480 e294  ................
-0001a9c0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001a9d0: e294 80e2 9480 e294 80e2 9480 e294 b4e2  ................
-0001a9e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001a9f0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001aa00: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001aa10: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001aa20: 80e2 94b4 e294 80e2 9480 e294 80e2 9480  ................
-0001aa30: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001aa40: 9480 e294 80e2 94b4 e294 80e2 9480 e294  ................
-0001aa50: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-0001aa60: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001aa70: 9480 e294 80e2 9480 e294 b4e2 9480 e294  ................
+0001a900: e294 bce2 9480 e294 80e2 9480 e294 80e2  ................
+0001a910: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a920: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a930: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a940: 9480 e294 80e2 94bc e294 80e2 9480 e294  ................
+0001a950: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a960: e294 80e2 9480 e294 80e2 94bc e294 80e2  ................
+0001a970: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a980: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a990: e294 80e2 9480 e294 80e2 9480 e294 bce2  ................
+0001a9a0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001a9b0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001a9c0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001a9d0: 9480 e294 80e2 9480 e294 a40a e294 8220  ............... 
+0001a9e0: 2037 20e2 9482 2020 2020 2020 3520 e294   7 ...      5 ..
+0001a9f0: 8220 4157 5320 2020 2020 2020 20e2 9482  . AWS        ...
+0001aa00: 2041 7773 5370 6f74 436f 6d70 7574 6553   AwsSpotComputeS
+0001aa10: 6f75 7263 6520 e294 8220 6575 2d77 6573  ource ... eu-wes
+0001aa20: 742d 3220 e294 8220 6d35 612e 6c61 7267  t-2 ... m5a.larg
+0001aa30: 6520 2020 2020 20e2 9482 2061 7773 7370  e      ... awssp
+0001aa40: 6f74 2d65 752d 7765 7374 2d32 20e2 9482  ot-eu-west-2 ...
+0001aa50: 0ae2 949c e294 80e2 9480 e294 80e2 9480  ................
+0001aa60: e294 bce2 9480 e294 80e2 9480 e294 80e2  ................
+0001aa70: 9480 e294 80e2 9480 e294 80e2 94bc e294  ................
 0001aa80: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 0001aa90: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-0001aaa0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-0001aab0: 80e2 9480 e294 980a 6060 600a 0a23 2320  ........```..## 
-0001aac0: 7964 2d74 6572 6d69 6e61 7465 0a0a 5468  yd-terminate..Th
-0001aad0: 6520 6079 642d 7465 726d 696e 6174 6560  e `yd-terminate`
-0001aae0: 2063 6f6d 6d61 6e64 2069 6d6d 6564 6961   command immedia
-0001aaf0: 7465 6c79 2074 6572 6d69 6e61 7465 7320  tely terminates 
-0001ab00: 436f 6d70 7574 6520 5265 7175 6972 656d  Compute Requirem
-0001ab10: 656e 7473 2074 6861 7420 6d61 7463 6820  ents that match 
-0001ab20: 7468 6520 606e 616d 6573 7061 6365 6020  the `namespace` 
-0001ab30: 616e 6420 6074 6167 6020 666f 756e 6420  and `tag` found 
-0001ab40: 696e 2074 6865 2063 6f6e 6669 6775 7261  in the configura
-0001ab50: 7469 6f6e 2066 696c 652e 2041 6e79 2065  tion file. Any e
-0001ab60: 7865 6375 7469 6e67 2054 6173 6b73 2077  xecuting Tasks w
-0001ab70: 696c 6c20 6265 2074 6572 6d69 6e61 7465  ill be terminate
-0001ab80: 6420 696d 6d65 6469 6174 656c 792c 2061  d immediately, a
-0001ab90: 6e64 2074 6865 2057 6f72 6b65 7220 506f  nd the Worker Po
-0001aba0: 6f6c 2077 696c 6c20 6265 2073 6875 7420  ol will be shut 
-0001abb0: 646f 776e 2e0a                           down..
+0001aaa0: 9480 e294 bce2 9480 e294 80e2 9480 e294  ................
+0001aab0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001aac0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001aad0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001aae0: 80e2 9480 e294 80e2 94bc e294 80e2 9480  ................
+0001aaf0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001ab00: 9480 e294 80e2 9480 e294 80e2 94bc e294  ................
+0001ab10: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001ab20: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001ab30: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001ab40: bce2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001ab50: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001ab60: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001ab70: 80e2 9480 e294 80e2 9480 e294 a40a e294  ................
+0001ab80: 8220 2038 20e2 9482 2020 2020 2020 3520  .  8 ...      5 
+0001ab90: e294 8220 4157 5320 2020 2020 2020 20e2  ... AWS        .
+0001aba0: 9482 2041 7773 5370 6f74 436f 6d70 7574  .. AwsSpotComput
+0001abb0: 6553 6f75 7263 6520 e294 8220 6575 2d77  eSource ... eu-w
+0001abc0: 6573 742d 3220 e294 8220 6d35 6164 2e6c  est-2 ... m5ad.l
+0001abd0: 6172 6765 2020 2020 20e2 9482 2061 7773  arge     ... aws
+0001abe0: 7370 6f74 2d65 752d 7765 7374 2d32 20e2  spot-eu-west-2 .
+0001abf0: 9482 0ae2 949c e294 80e2 9480 e294 80e2  ................
+0001ac00: 9480 e294 bce2 9480 e294 80e2 9480 e294  ................
+0001ac10: 80e2 9480 e294 80e2 9480 e294 80e2 94bc  ................
+0001ac20: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001ac30: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001ac40: 80e2 9480 e294 bce2 9480 e294 80e2 9480  ................
+0001ac50: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001ac60: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001ac70: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001ac80: e294 80e2 9480 e294 80e2 94bc e294 80e2  ................
+0001ac90: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001aca0: 80e2 9480 e294 80e2 9480 e294 80e2 94bc  ................
+0001acb0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001acc0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001acd0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001ace0: e294 bce2 9480 e294 80e2 9480 e294 80e2  ................
+0001acf0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001ad00: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001ad10: e294 80e2 9480 e294 80e2 9480 e294 a40a  ................
+0001ad20: e294 8220 2039 20e2 9482 2020 2020 2020  ...  9 ...      
+0001ad30: 3520 e294 8220 4157 5320 2020 2020 2020  5 ... AWS       
+0001ad40: 20e2 9482 2041 7773 5370 6f74 436f 6d70   ... AwsSpotComp
+0001ad50: 7574 6553 6f75 7263 6520 e294 8220 6575  uteSource ... eu
+0001ad60: 2d77 6573 742d 3220 e294 8220 6d36 612e  -west-2 ... m6a.
+0001ad70: 6c61 7267 6520 2020 2020 20e2 9482 2061  large      ... a
+0001ad80: 7773 7370 6f74 2d65 752d 7765 7374 2d32  wsspot-eu-west-2
+0001ad90: 20e2 9482 0ae2 949c e294 80e2 9480 e294   ...............
+0001ada0: 80e2 9480 e294 bce2 9480 e294 80e2 9480  ................
+0001adb0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001adc0: 94bc e294 80e2 9480 e294 80e2 9480 e294  ................
+0001add0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001ade0: e294 80e2 9480 e294 bce2 9480 e294 80e2  ................
+0001adf0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001ae00: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001ae10: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001ae20: 9480 e294 80e2 9480 e294 80e2 94bc e294  ................
+0001ae30: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001ae40: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001ae50: 94bc e294 80e2 9480 e294 80e2 9480 e294  ................
+0001ae60: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001ae70: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001ae80: 9480 e294 bce2 9480 e294 80e2 9480 e294  ................
+0001ae90: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001aea0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001aeb0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001aec0: a40a e294 8220 3130 20e2 9482 2020 2020  ..... 10 ...    
+0001aed0: 2020 3520 e294 8220 4157 5320 2020 2020    5 ... AWS     
+0001aee0: 2020 20e2 9482 2041 7773 5370 6f74 436f     ... AwsSpotCo
+0001aef0: 6d70 7574 6553 6f75 7263 6520 e294 8220  mputeSource ... 
+0001af00: 6575 2d77 6573 742d 3220 e294 8220 7433  eu-west-2 ... t3
+0001af10: 612e 6c61 7267 6520 2020 2020 20e2 9482  a.large      ...
+0001af20: 2061 7773 7370 6f74 2d65 752d 7765 7374   awsspot-eu-west
+0001af30: 2d32 20e2 9482 0ae2 9494 e294 80e2 9480  -2 .............
+0001af40: e294 80e2 9480 e294 b4e2 9480 e294 80e2  ................
+0001af50: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001af60: 80e2 94b4 e294 80e2 9480 e294 80e2 9480  ................
+0001af70: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001af80: 9480 e294 80e2 9480 e294 b4e2 9480 e294  ................
+0001af90: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001afa0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001afb0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001afc0: 80e2 9480 e294 80e2 9480 e294 80e2 94b4  ................
+0001afd0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001afe0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001aff0: 80e2 94b4 e294 80e2 9480 e294 80e2 9480  ................
+0001b000: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001b010: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001b020: 80e2 9480 e294 b4e2 9480 e294 80e2 9480  ................
+0001b030: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+0001b040: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+0001b050: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+0001b060: e294 980a 6060 600a 0a23 2320 7964 2d74  ....```..## yd-t
+0001b070: 6572 6d69 6e61 7465 0a0a 5468 6520 6079  erminate..The `y
+0001b080: 642d 7465 726d 696e 6174 6560 2063 6f6d  d-terminate` com
+0001b090: 6d61 6e64 2069 6d6d 6564 6961 7465 6c79  mand immediately
+0001b0a0: 2074 6572 6d69 6e61 7465 7320 436f 6d70   terminates Comp
+0001b0b0: 7574 6520 5265 7175 6972 656d 656e 7473  ute Requirements
+0001b0c0: 2074 6861 7420 6d61 7463 6820 7468 6520   that match the 
+0001b0d0: 606e 616d 6573 7061 6365 6020 616e 6420  `namespace` and 
+0001b0e0: 6074 6167 6020 666f 756e 6420 696e 2074  `tag` found in t
+0001b0f0: 6865 2063 6f6e 6669 6775 7261 7469 6f6e  he configuration
+0001b100: 2066 696c 652e 2041 6e79 2065 7865 6375   file. Any execu
+0001b110: 7469 6e67 2054 6173 6b73 2077 696c 6c20  ting Tasks will 
+0001b120: 6265 2074 6572 6d69 6e61 7465 6420 696d  be terminated im
+0001b130: 6d65 6469 6174 656c 792c 2061 6e64 2074  mediately, and t
+0001b140: 6865 2057 6f72 6b65 7220 506f 6f6c 2077  he Worker Pool w
+0001b150: 696c 6c20 6265 2073 6875 7420 646f 776e  ill be shut down
+0001b160: 2e0a                                     ..
```

### Comparing `yellowdog-python-examples-6.0.1/pyproject.toml` & `yellowdog-python-examples-6.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.1/setup.cfg` & `yellowdog-python-examples-6.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.1/yd_commands/abort.py` & `yellowdog-python-examples-6.0.2/yd_commands/abort.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.1/yd_commands/admin.py` & `yellowdog-python-examples-6.0.2/yd_commands/admin.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.1/yd_commands/args.py` & `yellowdog-python-examples-6.0.2/yd_commands/args.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,14 +104,20 @@
         )
         parser.add_argument(
             "--debug",
             action="store_true",
             required=False,
             help="print a stack trace (etc.) on error",
         )
+        parser.add_argument(
+            "--pac",
+            action="store_true",
+            required=False,
+            help="enable PAC (proxy auto-configuration) support",
+        )
 
         # Module-specific argument sets
 
         if any(module in sys.argv[0] for module in ["submit"]):
             parser.add_argument(
                 "--work-requirement",
                 "-r",
@@ -517,14 +523,18 @@
         return self.args.live_only
 
     @property
     def debug(self) -> Optional[bool]:
         return self.args.debug
 
     @property
+    def use_pac(self) -> Optional[bool]:
+        return self.args.pac
+
+    @property
     def directory(self) -> str:
         return "" if self.args.directory is None else self.args.directory
 
     @property
     def files(self) -> List[str]:
         return self.args.filenames
```

### Comparing `yellowdog-python-examples-6.0.1/yd_commands/cancel.py` & `yellowdog-python-examples-6.0.2/yd_commands/cancel.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.1/yd_commands/check_imports.py` & `yellowdog-python-examples-6.0.2/yd_commands/check_imports.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.1/yd_commands/compact_json.py` & `yellowdog-python-examples-6.0.2/yd_commands/compact_json.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.1/yd_commands/config.py` & `yellowdog-python-examples-6.0.2/yd_commands/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 @dataclass
 class ConfigCommon:
     url: str
     key: str
     secret: str
     namespace: str
     name_tag: str
+    use_pac: bool
 
 
 # Environment variable names for 'common' settings
 YD_KEY = "YD_KEY"
 YD_SECRET = "YD_SECRET"
 YD_NAMESPACE = "YD_NAMESPACE"
 YD_TAG = "YD_TAG"
@@ -220,14 +221,17 @@
             # Required
             key=key,
             secret=secret,
             namespace=namespace,
             name_tag=name_tag,
             # Optional
             url=url,
+            use_pac=(
+                True if ARGS_PARSER.use_pac else common_section.get(USE_PAC, False)
+            ),
         )
 
     except KeyError as e:
         print_error(f"Missing configuration data: {e}")
         exit(1)
```

### Comparing `yellowdog-python-examples-6.0.1/yd_commands/config_keys.py` & `yellowdog-python-examples-6.0.2/yd_commands/config_keys.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 TASK_TYPE = "taskType"  # String
 TASK_TYPES = "taskTypes"  # List of Strings
 TEMPLATE_ID = "templateId"  # String
 UPLOAD_FILES = "uploadFiles"  # List of Dicts
 LOCAL_PATH = "localPath"  # String
 UPLOAD_PATH = "uploadPath"  # String
 URL = "url"  # String
+USE_PAC = "usePAC"  # Boolean
 USERDATA = "userData"  # String
 USERDATAFILE = "userDataFile"  # String
 USERDATAFILES = "userDataFiles"  # List of Strings
 VARIABLES = "variables"  # Dictionary
 VCPUS = "vcpus"  # List of two Floats
 VERIFY_AT_START = "verifyAtStart"  # List of Strings
 VERIFY_WAIT = "verifyWait"  # List of Strings
@@ -144,14 +145,15 @@
     TASK_TYPE,
     TASK_TYPES,
     TEMPLATE_ID,
     UPLOAD_FILES,
     LOCAL_PATH,
     UPLOAD_PATH,
     URL,
+    USE_PAC,
     USERDATA,
     USERDATAFILE,
     USERDATAFILES,
     VARIABLES,
     VCPUS,
     VERIFY_AT_START,
     VERIFY_WAIT,
```

### Comparing `yellowdog-python-examples-6.0.1/yd_commands/csv_data.py` & `yellowdog-python-examples-6.0.2/yd_commands/csv_data.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.1/yd_commands/delete.py` & `yellowdog-python-examples-6.0.2/yd_commands/delete.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.1/yd_commands/download.py` & `yellowdog-python-examples-6.0.2/yd_commands/download.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.1/yd_commands/instantiate.py` & `yellowdog-python-examples-6.0.2/yd_commands/instantiate.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.1/yd_commands/interactive.py` & `yellowdog-python-examples-6.0.2/yd_commands/interactive.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.1/yd_commands/jsonnet2json.py` & `yellowdog-python-examples-6.0.2/yd_commands/jsonnet2json.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.1/yd_commands/list.py` & `yellowdog-python-examples-6.0.2/yd_commands/list.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.1/yd_commands/object_utilities.py` & `yellowdog-python-examples-6.0.2/yd_commands/object_utilities.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.1/yd_commands/printing.py` & `yellowdog-python-examples-6.0.2/yd_commands/printing.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.1/yd_commands/provision.py` & `yellowdog-python-examples-6.0.2/yd_commands/provision.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.1/yd_commands/provision_utils.py` & `yellowdog-python-examples-6.0.2/yd_commands/provision_utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.1/yd_commands/reformat_json.py` & `yellowdog-python-examples-6.0.2/yd_commands/reformat_json.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.1/yd_commands/shutdown.py` & `yellowdog-python-examples-6.0.2/yd_commands/shutdown.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.1/yd_commands/submit.py` & `yellowdog-python-examples-6.0.2/yd_commands/submit.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.1/yd_commands/submit_utils.py` & `yellowdog-python-examples-6.0.2/yd_commands/submit_utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.1/yd_commands/terminate.py` & `yellowdog-python-examples-6.0.2/yd_commands/terminate.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.1/yd_commands/type_check.py` & `yellowdog-python-examples-6.0.2/yd_commands/type_check.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.1/yd_commands/upload.py` & `yellowdog-python-examples-6.0.2/yd_commands/upload.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.1/yd_commands/upload_utils.py` & `yellowdog-python-examples-6.0.2/yd_commands/upload_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,16 @@
     """
 
     if stat(filename).st_size == 0:
         print_log(f"Not uploading zero-byte file '{filename}'")
         return False
 
     dest_filename = unique_upload_pathname(
-        filename,
+        # Convert Windows path naming to Unix
+        filename.replace("\\", "/").replace(":", ""),
         id=id,
         inputs_folder_name=inputs_folder_name,
         flatten_upload_paths=flatten_upload_paths,
     )
 
     upload_file_core(
         client=client,
```

### Comparing `yellowdog-python-examples-6.0.1/yd_commands/validate_properties.py` & `yellowdog-python-examples-6.0.2/yd_commands/validate_properties.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.1/yd_commands/variables.py` & `yellowdog-python-examples-6.0.2/yd_commands/variables.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.1/yd_commands/version.py` & `yellowdog-python-examples-6.0.2/yd_commands/version.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.1/yd_commands/wrapper.py` & `yellowdog-python-examples-6.0.2/yd_commands/wrapper.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 Decorator to handle standard setup, shutdown and exception handling
 for all commands.
 """
 
+import os
 from typing import List
 
+from pypac import pac_context_for_url
 from yellowdog_client import PlatformClient
 from yellowdog_client.model import ApiKey, KeyringSummary, ServicesSchema
 
 from yd_commands.args import ARGS_PARSER
 from yd_commands.config import ConfigCommon, load_config_common
 from yd_commands.printing import print_error, print_log
 
@@ -48,33 +50,54 @@
         for keyring_summary in keyrings:
             # This is a little brittle, obviously
             print_log(
                 f"YellowDog Account short identifier is: '{keyring_summary.id[13:19]}'"
             )
 
 
+def set_proxy_using_pac_if_enabled():
+    """
+    Set the HTTPS proxy using autoconfiguration (PAC)
+    """
+    HTTPS_PROXY_VAR = "HTTPS_PROXY"
+    if CONFIG_COMMON.use_pac:
+        print_log("Using Proxy Auto-Configuration (PAC)")
+        with pac_context_for_url(CONFIG_COMMON.url):
+            https_proxy = os.getenv(HTTPS_PROXY_VAR, None)
+        if https_proxy is not None:
+            os.environ[HTTPS_PROXY_VAR] = https_proxy
+        else:
+            print_log("No PAC proxy settings found")
+    else:
+        https_proxy = os.getenv(HTTPS_PROXY_VAR, None)
+    if https_proxy is not None:
+        print_log(f"Using {HTTPS_PROXY_VAR}={https_proxy}")
+
+
 def main_wrapper(func):
     def wrapper():
         if not ARGS_PARSER.debug:
             exit_code = 0
             try:
+                set_proxy_using_pac_if_enabled()
                 print_account()
                 func()
             except Exception as e:
                 print_error(e)
                 exit_code = 1
             except KeyboardInterrupt:
                 print_log("Cancelled")
                 exit_code = 1
             finally:
                 CLIENT.close()
                 if exit_code == 0:
                     print_log("Done")
                 exit(exit_code)
         else:
+            set_proxy_using_pac_if_enabled()
             print_account()
             func()
             CLIENT.close()
             print_log("Done")
             exit(0)
 
     return wrapper
```

### Comparing `yellowdog-python-examples-6.0.1/yellowdog_python_examples.egg-info/PKG-INFO` & `yellowdog-python-examples-6.0.2/yellowdog_python_examples.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yellowdog-python-examples
-Version: 6.0.1
+Version: 6.0.2
 Summary: Example Python commands using the YellowDog Python SDK
 Home-page: https://github.com/yellowdog/python-examples
 Author: YellowDog Limited
 Author-email: YellowDog Limited <support@yellowdog.co>
 Project-URL: Homepage, https://github.com/yellowdog/python-examples
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yellowdog-python-examples-6.0.1/yellowdog_python_examples.egg-info/SOURCES.txt` & `yellowdog-python-examples-6.0.2/yellowdog_python_examples.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-6.0.1/yellowdog_python_examples.egg-info/entry_points.txt` & `yellowdog-python-examples-6.0.2/yellowdog_python_examples.egg-info/entry_points.txt`

 * *Files identical despite different names*

