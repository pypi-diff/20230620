# Comparing `tmp/py-miraie-ac-0.1.7.tar.gz` & `tmp/py-miraie-ac-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-miraie-ac-0.1.7.tar", last modified: Tue Jun 20 07:09:26 2023, max compression
+gzip compressed data, was "py-miraie-ac-0.1.8.tar", last modified: Tue Jun 20 07:55:21 2023, max compression
```

## Comparing `py-miraie-ac-0.1.7.tar` & `py-miraie-ac-0.1.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 07:09:26.046878 py-miraie-ac-0.1.7/
--rw-rw-rw-   0        0        0    35821 2023-06-09 07:50:41.000000 py-miraie-ac-0.1.7/LICENSE
--rw-rw-rw-   0        0        0     1273 2023-06-20 07:09:26.047880 py-miraie-ac-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      666 2023-06-13 02:52:22.000000 py-miraie-ac-0.1.7/README.md
--rw-rw-rw-   0        0        0      104 2023-06-09 16:09:32.000000 py-miraie-ac-0.1.7/pyproject.toml
--rw-rw-rw-   0        0        0      801 2023-06-20 07:09:26.048878 py-miraie-ac-0.1.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-20 07:09:26.022223 py-miraie-ac-0.1.7/src/
-drwxrwxrwx   0        0        0        0 2023-06-20 07:09:26.040646 py-miraie-ac-0.1.7/src/py_miraie_ac/
--rw-rw-rw-   0        0        0      403 2023-06-09 13:16:33.000000 py-miraie-ac-0.1.7/src/py_miraie_ac/__init__.py
--rw-rw-rw-   0        0        0     6785 2023-06-20 07:06:07.000000 py-miraie-ac-0.1.7/src/py_miraie_ac/api.py
--rw-rw-rw-   0        0        0     6879 2023-06-20 07:06:21.000000 py-miraie-ac-0.1.7/src/py_miraie_ac/broker.py
--rw-rw-rw-   0        0        0      421 2023-06-05 03:33:43.000000 py-miraie-ac-0.1.7/src/py_miraie_ac/constants.py
--rw-rw-rw-   0        0        0     4858 2023-06-20 07:07:59.000000 py-miraie-ac-0.1.7/src/py_miraie_ac/device.py
--rw-rw-rw-   0        0        0      983 2023-06-20 07:08:05.000000 py-miraie-ac-0.1.7/src/py_miraie_ac/deviceStatus.py
--rw-rw-rw-   0        0        0      917 2023-06-05 03:55:22.000000 py-miraie-ac-0.1.7/src/py_miraie_ac/enums.py
--rw-rw-rw-   0        0        0      378 2023-06-20 05:51:20.000000 py-miraie-ac-0.1.7/src/py_miraie_ac/exceptions.py
--rw-rw-rw-   0        0        0      471 2023-06-20 07:08:15.000000 py-miraie-ac-0.1.7/src/py_miraie_ac/home.py
--rw-rw-rw-   0        0        0        0 2023-06-20 07:05:47.000000 py-miraie-ac-0.1.7/src/py_miraie_ac/test.py
--rw-rw-rw-   0        0        0      460 2023-06-05 03:57:35.000000 py-miraie-ac-0.1.7/src/py_miraie_ac/user.py
--rw-rw-rw-   0        0        0      236 2023-06-09 13:29:27.000000 py-miraie-ac-0.1.7/src/py_miraie_ac/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-20 07:09:26.046878 py-miraie-ac-0.1.7/src/py_miraie_ac.egg-info/
--rw-rw-rw-   0        0        0     1273 2023-06-20 07:09:26.000000 py-miraie-ac-0.1.7/src/py_miraie_ac.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      569 2023-06-20 07:09:26.000000 py-miraie-ac-0.1.7/src/py_miraie_ac.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 07:09:26.000000 py-miraie-ac-0.1.7/src/py_miraie_ac.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-20 07:09:26.000000 py-miraie-ac-0.1.7/src/py_miraie_ac.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-20 07:09:26.000000 py-miraie-ac-0.1.7/src/py_miraie_ac.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 07:55:21.258386 py-miraie-ac-0.1.8/
+-rw-rw-rw-   0        0        0    35821 2023-06-09 07:50:41.000000 py-miraie-ac-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0     1273 2023-06-20 07:55:21.258386 py-miraie-ac-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      666 2023-06-13 02:52:22.000000 py-miraie-ac-0.1.8/README.md
+-rw-rw-rw-   0        0        0      104 2023-06-09 16:09:32.000000 py-miraie-ac-0.1.8/pyproject.toml
+-rw-rw-rw-   0        0        0      801 2023-06-20 07:55:21.260271 py-miraie-ac-0.1.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-20 07:55:21.142687 py-miraie-ac-0.1.8/src/
+drwxrwxrwx   0        0        0        0 2023-06-20 07:55:21.164285 py-miraie-ac-0.1.8/src/py_miraie_ac/
+-rw-rw-rw-   0        0        0      454 2023-06-20 07:54:17.000000 py-miraie-ac-0.1.8/src/py_miraie_ac/__init__.py
+-rw-rw-rw-   0        0        0     6785 2023-06-20 07:06:07.000000 py-miraie-ac-0.1.8/src/py_miraie_ac/api.py
+-rw-rw-rw-   0        0        0     6879 2023-06-20 07:06:21.000000 py-miraie-ac-0.1.8/src/py_miraie_ac/broker.py
+-rw-rw-rw-   0        0        0      421 2023-06-05 03:33:43.000000 py-miraie-ac-0.1.8/src/py_miraie_ac/constants.py
+-rw-rw-rw-   0        0        0     4858 2023-06-20 07:07:59.000000 py-miraie-ac-0.1.8/src/py_miraie_ac/device.py
+-rw-rw-rw-   0        0        0      983 2023-06-20 07:08:05.000000 py-miraie-ac-0.1.8/src/py_miraie_ac/deviceStatus.py
+-rw-rw-rw-   0        0        0      917 2023-06-05 03:55:22.000000 py-miraie-ac-0.1.8/src/py_miraie_ac/enums.py
+-rw-rw-rw-   0        0        0      378 2023-06-20 05:51:20.000000 py-miraie-ac-0.1.8/src/py_miraie_ac/exceptions.py
+-rw-rw-rw-   0        0        0      471 2023-06-20 07:08:15.000000 py-miraie-ac-0.1.8/src/py_miraie_ac/home.py
+-rw-rw-rw-   0        0        0        0 2023-06-20 07:54:58.000000 py-miraie-ac-0.1.8/src/py_miraie_ac/test.py
+-rw-rw-rw-   0        0        0      460 2023-06-05 03:57:35.000000 py-miraie-ac-0.1.8/src/py_miraie_ac/user.py
+-rw-rw-rw-   0        0        0      236 2023-06-09 13:29:27.000000 py-miraie-ac-0.1.8/src/py_miraie_ac/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-20 07:55:21.170984 py-miraie-ac-0.1.8/src/py_miraie_ac.egg-info/
+-rw-rw-rw-   0        0        0     1273 2023-06-20 07:55:21.000000 py-miraie-ac-0.1.8/src/py_miraie_ac.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      569 2023-06-20 07:55:21.000000 py-miraie-ac-0.1.8/src/py_miraie_ac.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 07:55:21.000000 py-miraie-ac-0.1.8/src/py_miraie_ac.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-20 07:55:21.000000 py-miraie-ac-0.1.8/src/py_miraie_ac.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-20 07:55:21.000000 py-miraie-ac-0.1.8/src/py_miraie_ac.egg-info/top_level.txt
```

### Comparing `py-miraie-ac-0.1.7/LICENSE` & `py-miraie-ac-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `py-miraie-ac-0.1.7/PKG-INFO` & `py-miraie-ac-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-miraie-ac
-Version: 0.1.7
+Version: 0.1.8
 Summary: A package to control and read MirAIe Aircons by Panasonic
 Home-page: https://github.com/milothomas/py-miraie-ac
 Author: Milo Thomas
 Author-email: 20719501+milothomas@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/milothomas/py-miraie-ac/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `py-miraie-ac-0.1.7/README.md` & `py-miraie-ac-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `py-miraie-ac-0.1.7/setup.cfg` & `py-miraie-ac-0.1.8/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 792d 6d69 7261 6965 2d61 630d   = py-miraie-ac.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e31 2e37  .version = 0.1.7
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e31 2e38  .version = 0.1.8
 00000030: 0d0a 6175 7468 6f72 203d 204d 696c 6f20  ..author = Milo 
 00000040: 5468 6f6d 6173 0d0a 6175 7468 6f72 5f65  Thomas..author_e
 00000050: 6d61 696c 203d 2032 3037 3139 3530 312b  mail = 20719501+
 00000060: 6d69 6c6f 7468 6f6d 6173 4075 7365 7273  milothomas@users
 00000070: 2e6e 6f72 6570 6c79 2e67 6974 6875 622e  .noreply.github.
 00000080: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
 00000090: 203d 2041 2070 6163 6b61 6765 2074 6f20   = A package to
```

### Comparing `py-miraie-ac-0.1.7/src/py_miraie_ac/api.py` & `py-miraie-ac-0.1.8/src/py_miraie_ac/api.py`

 * *Files identical despite different names*

### Comparing `py-miraie-ac-0.1.7/src/py_miraie_ac/broker.py` & `py-miraie-ac-0.1.8/src/py_miraie_ac/broker.py`

 * *Files identical despite different names*

### Comparing `py-miraie-ac-0.1.7/src/py_miraie_ac/device.py` & `py-miraie-ac-0.1.8/src/py_miraie_ac/device.py`

 * *Files identical despite different names*

### Comparing `py-miraie-ac-0.1.7/src/py_miraie_ac/deviceStatus.py` & `py-miraie-ac-0.1.8/src/py_miraie_ac/deviceStatus.py`

 * *Files identical despite different names*

### Comparing `py-miraie-ac-0.1.7/src/py_miraie_ac/enums.py` & `py-miraie-ac-0.1.8/src/py_miraie_ac/enums.py`

 * *Files identical despite different names*

### Comparing `py-miraie-ac-0.1.7/src/py_miraie_ac.egg-info/PKG-INFO` & `py-miraie-ac-0.1.8/src/py_miraie_ac.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-miraie-ac
-Version: 0.1.7
+Version: 0.1.8
 Summary: A package to control and read MirAIe Aircons by Panasonic
 Home-page: https://github.com/milothomas/py-miraie-ac
 Author: Milo Thomas
 Author-email: 20719501+milothomas@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/milothomas/py-miraie-ac/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `py-miraie-ac-0.1.7/src/py_miraie_ac.egg-info/SOURCES.txt` & `py-miraie-ac-0.1.8/src/py_miraie_ac.egg-info/SOURCES.txt`

 * *Files identical despite different names*

