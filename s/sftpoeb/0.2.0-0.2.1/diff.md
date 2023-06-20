# Comparing `tmp/sftpoeb-0.2.0.tar.gz` & `tmp/sftpoeb-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sftpoeb-0.2.0.tar", last modified: Mon Jun 19 09:55:56 2023, max compression
+gzip compressed data, was "sftpoeb-0.2.1.tar", last modified: Mon Jun 19 11:37:35 2023, max compression
```

## Comparing `sftpoeb-0.2.0.tar` & `sftpoeb-0.2.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 09:55:56.301197 sftpoeb-0.2.0/
--rw-rw-rw-   0        0        0     1157 2023-06-19 09:10:48.000000 sftpoeb-0.2.0/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1074 2023-06-13 11:20:28.000000 sftpoeb-0.2.0/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-06-13 11:20:53.000000 sftpoeb-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1579 2023-06-19 09:55:56.299200 sftpoeb-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      109 2023-06-13 11:41:58.000000 sftpoeb-0.2.0/README.txt
--rw-rw-rw-   0        0        0       79 2023-06-13 11:20:27.000000 sftpoeb-0.2.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 09:55:56.301197 sftpoeb-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      572 2023-06-19 09:55:47.000000 sftpoeb-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:55:56.181197 sftpoeb-0.2.0/sftpoeb/
--rw-rw-rw-   0        0        0       72 2023-06-15 12:00:06.000000 sftpoeb-0.2.0/sftpoeb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:55:56.202231 sftpoeb-0.2.0/sftpoeb/config/
--rw-rw-rw-   0        0        0       54 2023-06-09 11:32:38.000000 sftpoeb-0.2.0/sftpoeb/config/variable.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:55:56.209195 sftpoeb-0.2.0/sftpoeb/mainclass/
--rw-rw-rw-   0        0        0       48 2023-06-15 12:01:46.000000 sftpoeb-0.2.0/sftpoeb/mainclass/__init__.py
--rw-rw-rw-   0        0        0    11520 2023-06-16 11:54:11.000000 sftpoeb-0.2.0/sftpoeb/mainclass/c_recovery.py
--rw-rw-rw-   0        0        0     5975 2023-06-19 08:05:00.000000 sftpoeb-0.2.0/sftpoeb/mainclass/c_sftp.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:55:56.230230 sftpoeb-0.2.0/sftpoeb/method/
--rw-rw-rw-   0        0        0       95 2023-06-14 12:04:10.000000 sftpoeb-0.2.0/sftpoeb/method/__init__.py
--rw-rw-rw-   0        0        0     6670 2023-06-19 06:57:01.000000 sftpoeb-0.2.0/sftpoeb/method/callservice.py
--rw-rw-rw-   0        0        0      629 2023-06-19 09:40:40.000000 sftpoeb-0.2.0/sftpoeb/method/checkpath.py
--rw-rw-rw-   0        0        0      307 2023-06-09 11:32:38.000000 sftpoeb-0.2.0/sftpoeb/method/debug.py
--rw-rw-rw-   0        0        0     9657 2023-06-15 07:54:02.000000 sftpoeb-0.2.0/sftpoeb/method/mail.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:55:56.240205 sftpoeb-0.2.0/sftpoeb/sftpoeb.egg-info/
--rw-rw-rw-   0        0        0      945 2023-06-14 03:38:35.000000 sftpoeb-0.2.0/sftpoeb/sftpoeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 03:38:35.000000 sftpoeb-0.2.0/sftpoeb/sftpoeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-14 03:38:35.000000 sftpoeb-0.2.0/sftpoeb/sftpoeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-14 03:38:35.000000 sftpoeb-0.2.0/sftpoeb/sftpoeb.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 09:55:56.242195 sftpoeb-0.2.0/sftpoeb/subclass/
--rw-rw-rw-   0        0        0      156 2023-06-16 04:43:20.000000 sftpoeb-0.2.0/sftpoeb/subclass/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:55:56.246202 sftpoeb-0.2.0/sftpoeb/subclass/alert/
--rw-rw-rw-   0        0        0       24 2023-06-15 07:57:29.000000 sftpoeb-0.2.0/sftpoeb/subclass/alert/__init__.py
--rw-rw-rw-   0        0        0     1515 2023-06-19 08:43:27.000000 sftpoeb-0.2.0/sftpoeb/subclass/alert/s_c_alert.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:55:56.253198 sftpoeb-0.2.0/sftpoeb/subclass/file/
--rw-rw-rw-   0        0        0       57 2023-06-14 03:50:45.000000 sftpoeb-0.2.0/sftpoeb/subclass/file/__init__.py
--rw-rw-rw-   0        0        0     2892 2023-06-14 04:00:58.000000 sftpoeb-0.2.0/sftpoeb/subclass/file/s_c_file.py
--rw-rw-rw-   0        0        0     4988 2023-06-09 11:32:38.000000 sftpoeb-0.2.0/sftpoeb/subclass/file/s_c_file_transfer.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:55:56.259197 sftpoeb-0.2.0/sftpoeb/subclass/input/
--rw-rw-rw-   0        0        0       24 2023-06-14 03:50:57.000000 sftpoeb-0.2.0/sftpoeb/subclass/input/__init__.py
--rw-rw-rw-   0        0        0     1162 2023-06-14 04:01:07.000000 sftpoeb-0.2.0/sftpoeb/subclass/input/s_c_input.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:55:56.263198 sftpoeb-0.2.0/sftpoeb/subclass/output/
--rw-rw-rw-   0        0        0       25 2023-06-14 03:51:08.000000 sftpoeb-0.2.0/sftpoeb/subclass/output/__init__.py
--rw-rw-rw-   0        0        0     1171 2023-06-14 04:01:13.000000 sftpoeb-0.2.0/sftpoeb/subclass/output/s_c_output.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:55:56.273197 sftpoeb-0.2.0/sftpoeb/subclass/path/
--rw-rw-rw-   0        0        0      103 2023-06-14 03:51:28.000000 sftpoeb-0.2.0/sftpoeb/subclass/path/__init__.py
--rw-rw-rw-   0        0        0     5347 2023-06-19 08:02:54.000000 sftpoeb-0.2.0/sftpoeb/subclass/path/s_c_setgetdestination.py
--rw-rw-rw-   0        0        0     4126 2023-06-19 08:04:28.000000 sftpoeb-0.2.0/sftpoeb/subclass/path/s_c_setgetlocal.py
--rw-rw-rw-   0        0        0     2042 2023-06-15 11:58:34.000000 sftpoeb-0.2.0/sftpoeb/subclass/path/s_c_setgetrecovery.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:55:56.289198 sftpoeb-0.2.0/sftpoeb/subclass/process/
--rw-rw-rw-   0        0        0       74 2023-06-19 07:38:35.000000 sftpoeb-0.2.0/sftpoeb/subclass/process/__init__.py
--rw-rw-rw-   0        0        0    30018 2023-06-19 07:59:47.000000 sftpoeb-0.2.0/sftpoeb/subclass/process/s_c_process_package_1.py
--rw-rw-rw-   0        0        0    30592 2023-06-19 09:55:34.000000 sftpoeb-0.2.0/sftpoeb/subclass/process/s_c_process_package_2.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:55:56.296197 sftpoeb-0.2.0/sftpoeb/subclass/recovery/
--rw-rw-rw-   0        0        0       57 2023-06-19 07:38:29.000000 sftpoeb-0.2.0/sftpoeb/subclass/recovery/__init__.py
--rw-rw-rw-   0        0        0    21628 2023-06-16 11:42:28.000000 sftpoeb-0.2.0/sftpoeb/subclass/recovery/s_c_recovery.py
--rw-rw-rw-   0        0        0    21669 2023-06-19 07:39:49.000000 sftpoeb-0.2.0/sftpoeb/subclass/recovery/s_c_recovery2.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:55:56.200199 sftpoeb-0.2.0/sftpoeb.egg-info/
--rw-rw-rw-   0        0        0     1579 2023-06-19 09:55:56.000000 sftpoeb-0.2.0/sftpoeb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1464 2023-06-19 09:55:56.000000 sftpoeb-0.2.0/sftpoeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 09:55:56.000000 sftpoeb-0.2.0/sftpoeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-19 09:55:56.000000 sftpoeb-0.2.0/sftpoeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-19 09:55:56.000000 sftpoeb-0.2.0/sftpoeb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1238 2023-06-19 08:17:05.000000 sftpoeb-0.2.0/test.py
--rw-rw-rw-   0        0        0     1150 2023-06-16 11:54:21.000000 sftpoeb-0.2.0/test_recovery.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:37:35.540918 sftpoeb-0.2.1/
+-rw-rw-rw-   0        0        0     1242 2023-06-19 11:37:16.000000 sftpoeb-0.2.1/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1074 2023-06-13 11:20:28.000000 sftpoeb-0.2.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-06-13 11:20:53.000000 sftpoeb-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1664 2023-06-19 11:37:35.540918 sftpoeb-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      109 2023-06-13 11:41:58.000000 sftpoeb-0.2.1/README.txt
+-rw-rw-rw-   0        0        0       79 2023-06-13 11:20:27.000000 sftpoeb-0.2.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 11:37:35.541918 sftpoeb-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      572 2023-06-19 11:37:31.000000 sftpoeb-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:37:35.310185 sftpoeb-0.2.1/sftpoeb/
+-rw-rw-rw-   0        0        0       72 2023-06-15 12:00:06.000000 sftpoeb-0.2.1/sftpoeb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:37:35.341131 sftpoeb-0.2.1/sftpoeb/config/
+-rw-rw-rw-   0        0        0       54 2023-06-09 11:32:38.000000 sftpoeb-0.2.1/sftpoeb/config/variable.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:37:35.355130 sftpoeb-0.2.1/sftpoeb/mainclass/
+-rw-rw-rw-   0        0        0       48 2023-06-15 12:01:46.000000 sftpoeb-0.2.1/sftpoeb/mainclass/__init__.py
+-rw-rw-rw-   0        0        0    13179 2023-06-19 11:36:35.000000 sftpoeb-0.2.1/sftpoeb/mainclass/c_recovery.py
+-rw-rw-rw-   0        0        0     5975 2023-06-19 08:05:00.000000 sftpoeb-0.2.1/sftpoeb/mainclass/c_sftp.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:37:35.375128 sftpoeb-0.2.1/sftpoeb/method/
+-rw-rw-rw-   0        0        0       95 2023-06-14 12:04:10.000000 sftpoeb-0.2.1/sftpoeb/method/__init__.py
+-rw-rw-rw-   0        0        0     6670 2023-06-19 06:57:01.000000 sftpoeb-0.2.1/sftpoeb/method/callservice.py
+-rw-rw-rw-   0        0        0      629 2023-06-19 09:40:40.000000 sftpoeb-0.2.1/sftpoeb/method/checkpath.py
+-rw-rw-rw-   0        0        0      307 2023-06-09 11:32:38.000000 sftpoeb-0.2.1/sftpoeb/method/debug.py
+-rw-rw-rw-   0        0        0     9685 2023-06-19 11:27:15.000000 sftpoeb-0.2.1/sftpoeb/method/mail.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:37:35.383129 sftpoeb-0.2.1/sftpoeb/sftpoeb.egg-info/
+-rw-rw-rw-   0        0        0      945 2023-06-14 03:38:35.000000 sftpoeb-0.2.1/sftpoeb/sftpoeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 03:38:35.000000 sftpoeb-0.2.1/sftpoeb/sftpoeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-14 03:38:35.000000 sftpoeb-0.2.1/sftpoeb/sftpoeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-14 03:38:35.000000 sftpoeb-0.2.1/sftpoeb/sftpoeb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 11:37:35.385147 sftpoeb-0.2.1/sftpoeb/subclass/
+-rw-rw-rw-   0        0        0      156 2023-06-16 04:43:20.000000 sftpoeb-0.2.1/sftpoeb/subclass/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:37:35.397127 sftpoeb-0.2.1/sftpoeb/subclass/alert/
+-rw-rw-rw-   0        0        0       24 2023-06-15 07:57:29.000000 sftpoeb-0.2.1/sftpoeb/subclass/alert/__init__.py
+-rw-rw-rw-   0        0        0     2436 2023-06-19 11:28:31.000000 sftpoeb-0.2.1/sftpoeb/subclass/alert/s_c_alert.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:37:35.489921 sftpoeb-0.2.1/sftpoeb/subclass/file/
+-rw-rw-rw-   0        0        0       57 2023-06-14 03:50:45.000000 sftpoeb-0.2.1/sftpoeb/subclass/file/__init__.py
+-rw-rw-rw-   0        0        0     2892 2023-06-14 04:00:58.000000 sftpoeb-0.2.1/sftpoeb/subclass/file/s_c_file.py
+-rw-rw-rw-   0        0        0     4988 2023-06-09 11:32:38.000000 sftpoeb-0.2.1/sftpoeb/subclass/file/s_c_file_transfer.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:37:35.508059 sftpoeb-0.2.1/sftpoeb/subclass/input/
+-rw-rw-rw-   0        0        0       24 2023-06-14 03:50:57.000000 sftpoeb-0.2.1/sftpoeb/subclass/input/__init__.py
+-rw-rw-rw-   0        0        0     1162 2023-06-14 04:01:07.000000 sftpoeb-0.2.1/sftpoeb/subclass/input/s_c_input.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:37:35.512920 sftpoeb-0.2.1/sftpoeb/subclass/output/
+-rw-rw-rw-   0        0        0       25 2023-06-14 03:51:08.000000 sftpoeb-0.2.1/sftpoeb/subclass/output/__init__.py
+-rw-rw-rw-   0        0        0     1171 2023-06-14 04:01:13.000000 sftpoeb-0.2.1/sftpoeb/subclass/output/s_c_output.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:37:35.522919 sftpoeb-0.2.1/sftpoeb/subclass/path/
+-rw-rw-rw-   0        0        0      103 2023-06-14 03:51:28.000000 sftpoeb-0.2.1/sftpoeb/subclass/path/__init__.py
+-rw-rw-rw-   0        0        0     5347 2023-06-19 08:02:54.000000 sftpoeb-0.2.1/sftpoeb/subclass/path/s_c_setgetdestination.py
+-rw-rw-rw-   0        0        0     4126 2023-06-19 08:04:28.000000 sftpoeb-0.2.1/sftpoeb/subclass/path/s_c_setgetlocal.py
+-rw-rw-rw-   0        0        0     2042 2023-06-15 11:58:34.000000 sftpoeb-0.2.1/sftpoeb/subclass/path/s_c_setgetrecovery.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:37:35.529920 sftpoeb-0.2.1/sftpoeb/subclass/process/
+-rw-rw-rw-   0        0        0       74 2023-06-19 07:38:35.000000 sftpoeb-0.2.1/sftpoeb/subclass/process/__init__.py
+-rw-rw-rw-   0        0        0    30018 2023-06-19 07:59:47.000000 sftpoeb-0.2.1/sftpoeb/subclass/process/s_c_process_package_1.py
+-rw-rw-rw-   0        0        0    30592 2023-06-19 09:55:34.000000 sftpoeb-0.2.1/sftpoeb/subclass/process/s_c_process_package_2.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:37:35.537928 sftpoeb-0.2.1/sftpoeb/subclass/recovery/
+-rw-rw-rw-   0        0        0       57 2023-06-19 07:38:29.000000 sftpoeb-0.2.1/sftpoeb/subclass/recovery/__init__.py
+-rw-rw-rw-   0        0        0    21628 2023-06-16 11:42:28.000000 sftpoeb-0.2.1/sftpoeb/subclass/recovery/s_c_recovery.py
+-rw-rw-rw-   0        0        0    21669 2023-06-19 07:39:49.000000 sftpoeb-0.2.1/sftpoeb/subclass/recovery/s_c_recovery2.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:37:35.339169 sftpoeb-0.2.1/sftpoeb.egg-info/
+-rw-rw-rw-   0        0        0     1664 2023-06-19 11:37:35.000000 sftpoeb-0.2.1/sftpoeb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1464 2023-06-19 11:37:35.000000 sftpoeb-0.2.1/sftpoeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 11:37:35.000000 sftpoeb-0.2.1/sftpoeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-19 11:37:35.000000 sftpoeb-0.2.1/sftpoeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-19 11:37:35.000000 sftpoeb-0.2.1/sftpoeb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1238 2023-06-19 08:17:05.000000 sftpoeb-0.2.1/test.py
+-rw-rw-rw-   0        0        0     1150 2023-06-16 11:54:21.000000 sftpoeb-0.2.1/test_recovery.py
```

### Comparing `sftpoeb-0.2.0/CHANGELOG.txt` & `sftpoeb-0.2.1/CHANGELOG.txt`

 * *Files 5% similar despite different names*

```diff
@@ -73,8 +73,12 @@
 
 0.1.8 (19/06/2023)
 ------------------
 - Edit Path Package S06 
 
 0.1.9 (19/06/2023)
 ------------------
-- Edit permission makedir 
+- Edit permission makedir 
+
+0.2.1 (19/06/2023)
+------------------
+- Fetch recovery package 2 (S06) Normally
```

### Comparing `sftpoeb-0.2.0/LICENSE.txt` & `sftpoeb-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.2.0/PKG-INFO` & `sftpoeb-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sftpoeb
-Version: 0.2.0
+Version: 0.2.1
 Summary: To Easy create sftp for e-tax invoice & e-receive of Oneeletronicbilling
 Home-page: UNKNOWN
 Author: Natthawut Thawisombat
 Author-email: natthawut.th@inet.co.th
 License: MIT
 Keywords: sftp
 Platform: UNKNOWN
@@ -93,7 +93,11 @@
 ------------------
 - Edit Path Package S06 
 
 0.1.9 (19/06/2023)
 ------------------
 - Edit permission makedir 
 
+0.2.1 (19/06/2023)
+------------------
+- Fetch recovery package 2 (S06) Normally
+
```

### Comparing `sftpoeb-0.2.0/setup.py` & `sftpoeb-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
         name='sftpoeb',
-        version='0.2.0',
+        version='0.2.1',
         url='',
         license='MIT',
         author='Natthawut Thawisombat',
         author_email='natthawut.th@inet.co.th',
         description='To Easy create sftp for e-tax invoice & e-receive of Oneeletronicbilling',
         packages=find_packages(),
         long_description=open('README.txt').read() +  '\n\n' + open('CHANGELOG.txt').read(),
```

### Comparing `sftpoeb-0.2.0/sftpoeb/mainclass/c_recovery.py` & `sftpoeb-0.2.1/sftpoeb/mainclass/c_recovery.py`

 * *Files 14% similar despite different names*

```diff
@@ -180,7 +180,28 @@
                         pool.join()
                         
             print(str(self.dateNow + self.timeNow) + '>> API Recovery : Process Recovery done.')
             result = {"status": "OK", "message": "Process Recovery done."}
         except Exception as e:
             print(str(self.dateNow + self.timeNow) + '>> API Recovery error : ' + str(debug_row(e)))
             result = {"status": "ER","errorCode":"PR999", "errorMessage": 'API Recovery error : '+str(debug_row(e))}
+
+    def final(self):
+
+        self.alert.afterrecoveryfinsh(self.recovery_process.success_recovery + self.recovery_process.fail_recovery , 
+                                      self.recovery_process.success_recovery ,self.recovery_process.fail_recovery , 
+                                      self.recovery_process.success_recovery_message , self.recovery_process.fail_recovery_message)
+        if self.recovery_process.success_recovery_message != [] or self.recovery_process.fail_recovery_message != []:
+            try:
+                log_data = {
+                    "totalInvoice": str(self.recovery_process.success_recovery + self.recovery_process.fail_recovery),
+                    "successInvoice": str(self.recovery_process.success_recovery),
+                    "failedInvoice": str(self.recovery_process.fail_recovery),
+                    "successResponseInvoices": self.recovery_process.success_recovery_message,
+                    "failedResponseInvoices": self.recovery_process.fail_recovery_message
+                }
+                check_path(self.local.localLogPath + datetime.now().strftime("%Y-%m-%d") + "/" + str(self.dateNow + self.timeNow))
+                with open(self.local.localLogPath + datetime.now().strftime("%Y-%m-%d") + "/" + str(self.dateNow + self.timeNow) + '_recoveryLog.txt', 'w', encoding='UTF-8') as log:  ##### write log
+                    log.write(json.dumps(log_data, indent=4, sort_keys=False, ensure_ascii=False))
+                    log.close()
+            except Exception as e:
+                print(str(self.dateNow + self.timeNow) + '>>  Write recovery log path error : ' + str(e))
```

### Comparing `sftpoeb-0.2.0/sftpoeb/mainclass/c_sftp.py` & `sftpoeb-0.2.1/sftpoeb/mainclass/c_sftp.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.2.0/sftpoeb/method/callservice.py` & `sftpoeb-0.2.1/sftpoeb/method/callservice.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.2.0/sftpoeb/method/checkpath.py` & `sftpoeb-0.2.1/sftpoeb/method/checkpath.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.2.0/sftpoeb/method/mail.py` & `sftpoeb-0.2.1/sftpoeb/method/mail.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,25 +125,25 @@
         body += """ <hr style="width:100%;border:2px solid black;"/> """
         result = {"status":"OK","result":body.encode('utf-8')}
     except Exception as e:
         result = {"status":"ER","errorMessage":str(debug_row(e)) , "errorCode":"ER999"}
     finally:
         return result
 
-def generate_body_recover(data):
+def generate_body_recover(totalInvoice,successInvoice,failedInvoice,successResponseInvoices,failedResponseInvoices):
     try:
         body = """
                <div style="margin-left:30px;">
                    <h3>Summary</h3>
-                   Total Invoice : """ + str(data["totalInvoice"]) + """ <br>
-                   Success Invoice : """ + str(data["successInvoice"]) + """<br>
-                   Fail Invoice : """ + str(data["failedInvoice"]) + """ <br>
+                   Total Invoice : """ + str(totalInvoice) + """ <br>
+                   Success Invoice : """ + str(successInvoice) + """<br>
+                   Fail Invoice : """ + str(failedInvoice) + """ <br>
                </div><br>
                """
-        if data["successResponseInvoices"] != []:
+        if successResponseInvoices != []:
             body += """
                         <style>
                                 table{
                                     border-collapse: collapse;
                                 }
                                 table, th, td {
                                     border: 1px solid black;
@@ -157,24 +157,24 @@
                                 <tr style="border: 1px solid black;">
                                     <th>Date of Input</th>
                                     <th>Batch Name</th>
                                     <th>Document Name</th>
                                     <th>Message</th>
                                 </tr>
                         """
-            for sign_success in data["successResponseInvoices"]:
+            for sign_success in successResponseInvoices:
                 body += """
                         <tr>
                             <td>""" + str(sign_success["inputDate"]) + """</td>
                             <td>""" + str(sign_success["batchName"]) + """</td>
                             <td>""" + str(sign_success["invoiceNo"]) + """</td>
                             <td>""" + str(sign_success["message"]) + """</td>
                         </tr>
                     """
-        if data["failedResponseInvoices"] != []:
+        if failedResponseInvoices != []:
             body += """
                         <style>
                                 table{
                                     border-collapse: collapse;
                                 }
                                 table, th, td {
                                     border: 1px solid black;
@@ -189,15 +189,15 @@
                                     <th>Date of Input</th>
                                     <th>Batch Name</th>
                                     <th>Document Name</th>
                                     <th>Error Code</th>
                                     <th>Error Message</th>
                                 </tr>
                         """
-            for sign_error in data["failedResponseInvoices"]:
+            for sign_error in failedResponseInvoices:
                 body += """
                         <tr>
                             <td>""" + str(sign_error["inputDate"]) + """</td>
                             <td>""" + str(sign_error["batchName"]) + """</td>
                             <td>""" + str(sign_error["invoiceNo"]) + """</td>
                             <td>""" + str(sign_error["errorCode"]) + """</td>
                             <td>""" + str(sign_error["errorMessage"]) + """</td>
```

### Comparing `sftpoeb-0.2.0/sftpoeb/sftpoeb.egg-info/SOURCES.txt` & `sftpoeb-0.2.1/sftpoeb/sftpoeb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.2.0/sftpoeb/subclass/alert/s_c_alert.py` & `sftpoeb-0.2.1/sftpoeb/subclass/alert/s_c_alert.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,8 +24,21 @@
         ResponseSendMail = ""
         if FailedInvoice > 0 :
             mail_body = generate_body_template(TotalInvoice,SuccessInvoice,FailedInvoice,RecoverInvoice,RecoverResponseInvoices,ResponseInvoice)
             ResponseSendMail = sendmail_attachment(self.mail_subject,mail_body["result"],self.mail_receiver,self.mail_port,self.mail_host,self.mail_sender)
         else:
             ResponseSendMail = {"status":"OK","message":"Pass. Not found invoice fail"}
 
+        print("MailAlert : " , ResponseSendMail)
+
+    def afterrecoveryfinsh(self,totalInvoice,successInvoice,failedInvoice,successResponseInvoices,failedResponseInvoices):
+        if self.mail_subject == "None":
+            self.mail_subject = "< TH-ROBOTICS (UAT)> E-tax Process Notify. Date : " + str(datetime.now().strftime("%Y%m%d")) + " Time : " + str(datetime.now().strftime("%H%M%S"))
+        
+        ResponseSendMail = ""
+        if len(successResponseInvoices) > 0 or len(failedResponseInvoices) > 0 :
+            mail_body = generate_body_recover(totalInvoice,successInvoice,failedInvoice,successResponseInvoices,failedResponseInvoices)
+            ResponseSendMail = sendmail_attachment(self.mail_subject,mail_body["result"],self.mail_receiver,self.mail_port,self.mail_host,self.mail_sender)
+        else:
+            ResponseSendMail = {"status":"OK","message":"Pass. Not found invoice fail"}
+
         print("MailAlert : " , ResponseSendMail)
```

### Comparing `sftpoeb-0.2.0/sftpoeb/subclass/file/s_c_file.py` & `sftpoeb-0.2.1/sftpoeb/subclass/file/s_c_file.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.2.0/sftpoeb/subclass/file/s_c_file_transfer.py` & `sftpoeb-0.2.1/sftpoeb/subclass/file/s_c_file_transfer.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.2.0/sftpoeb/subclass/input/s_c_input.py` & `sftpoeb-0.2.1/sftpoeb/subclass/input/s_c_input.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.2.0/sftpoeb/subclass/output/s_c_output.py` & `sftpoeb-0.2.1/sftpoeb/subclass/output/s_c_output.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.2.0/sftpoeb/subclass/path/s_c_setgetdestination.py` & `sftpoeb-0.2.1/sftpoeb/subclass/path/s_c_setgetdestination.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.2.0/sftpoeb/subclass/path/s_c_setgetlocal.py` & `sftpoeb-0.2.1/sftpoeb/subclass/path/s_c_setgetlocal.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.2.0/sftpoeb/subclass/path/s_c_setgetrecovery.py` & `sftpoeb-0.2.1/sftpoeb/subclass/path/s_c_setgetrecovery.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.2.0/sftpoeb/subclass/process/s_c_process_package_1.py` & `sftpoeb-0.2.1/sftpoeb/subclass/process/s_c_process_package_1.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.2.0/sftpoeb/subclass/process/s_c_process_package_2.py` & `sftpoeb-0.2.1/sftpoeb/subclass/process/s_c_process_package_2.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.2.0/sftpoeb/subclass/recovery/s_c_recovery.py` & `sftpoeb-0.2.1/sftpoeb/subclass/recovery/s_c_recovery.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.2.0/sftpoeb/subclass/recovery/s_c_recovery2.py` & `sftpoeb-0.2.1/sftpoeb/subclass/recovery/s_c_recovery2.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.2.0/sftpoeb.egg-info/PKG-INFO` & `sftpoeb-0.2.1/sftpoeb.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sftpoeb
-Version: 0.2.0
+Version: 0.2.1
 Summary: To Easy create sftp for e-tax invoice & e-receive of Oneeletronicbilling
 Home-page: UNKNOWN
 Author: Natthawut Thawisombat
 Author-email: natthawut.th@inet.co.th
 License: MIT
 Keywords: sftp
 Platform: UNKNOWN
@@ -93,7 +93,11 @@
 ------------------
 - Edit Path Package S06 
 
 0.1.9 (19/06/2023)
 ------------------
 - Edit permission makedir 
 
+0.2.1 (19/06/2023)
+------------------
+- Fetch recovery package 2 (S06) Normally
+
```

### Comparing `sftpoeb-0.2.0/sftpoeb.egg-info/SOURCES.txt` & `sftpoeb-0.2.1/sftpoeb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.2.0/test.py` & `sftpoeb-0.2.1/test.py`

 * *Files identical despite different names*

### Comparing `sftpoeb-0.2.0/test_recovery.py` & `sftpoeb-0.2.1/test_recovery.py`

 * *Files identical despite different names*

