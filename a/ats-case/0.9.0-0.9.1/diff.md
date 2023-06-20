# Comparing `tmp/ats_case-0.9.0.tar.gz` & `tmp/ats_case-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ats_case-0.9.0.tar", last modified: Tue Jun 20 08:42:35 2023, max compression
+gzip compressed data, was "ats_case-0.9.1.tar", last modified: Tue Jun 20 08:45:08 2023, max compression
```

## Comparing `ats_case-0.9.0.tar` & `ats_case-0.9.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 08:42:35.291418 ats_case-0.9.0/
--rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.9.0/LICENSE
--rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.9.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1042 2023-06-20 08:42:35.289426 ats_case-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.9.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 08:42:34.877663 ats_case-0.9.0/ats_case/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.9.0/ats_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 08:42:35.107051 ats_case-0.9.0/ats_case/case/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.9.0/ats_case/case/__init__.py
--rw-rw-rw-   0        0        0    18857 2023-06-19 03:05:41.000000 ats_case-0.9.0/ats_case/case/command.py
--rw-rw-rw-   0        0        0    12148 2023-06-20 07:39:55.000000 ats_case-0.9.0/ats_case/case/context.py
--rw-rw-rw-   0        0        0     7874 2023-06-20 08:42:18.000000 ats_case-0.9.0/ats_case/case/executor.py
--rw-rw-rw-   0        0        0     5654 2023-05-22 01:21:46.000000 ats_case-0.9.0/ats_case/case/translator.py
-drwxrwxrwx   0        0        0        0 2023-06-20 08:42:35.176011 ats_case-0.9.0/ats_case/common/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.9.0/ats_case/common/__init__.py
--rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.9.0/ats_case/common/enum.py
--rw-rw-rw-   0        0        0      790 2023-04-25 08:30:39.000000 ats_case-0.9.0/ats_case/common/error.py
-drwxrwxrwx   0        0        0        0 2023-06-20 08:42:35.242831 ats_case-0.9.0/ats_case/manage/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.9.0/ats_case/manage/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-04-25 06:21:05.000000 ats_case-0.9.0/ats_case/manage/core.py
--rw-rw-rw-   0        0        0     4039 2023-06-16 06:59:03.000000 ats_case-0.9.0/ats_case/manage/start.py
-drwxrwxrwx   0        0        0        0 2023-06-20 08:42:35.275744 ats_case-0.9.0/ats_case/template/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.9.0/ats_case/template/__init__.py
--rw-rw-rw-   0        0        0     2400 2023-05-29 01:45:03.000000 ats_case-0.9.0/ats_case/template/testcase_v1.tmp
-drwxrwxrwx   0        0        0        0 2023-06-20 08:42:34.982383 ats_case-0.9.0/ats_case.egg-info/
--rw-rw-rw-   0        0        0     1042 2023-06-20 08:42:34.000000 ats_case-0.9.0/ats_case.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-06-20 08:42:34.000000 ats_case-0.9.0/ats_case.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 08:42:34.000000 ats_case-0.9.0/ats_case.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-06-20 08:42:34.000000 ats_case-0.9.0/ats_case.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-20 08:42:34.000000 ats_case-0.9.0/ats_case.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 08:42:35.291418 ats_case-0.9.0/setup.cfg
--rw-rw-rw-   0        0        0      945 2023-06-20 08:42:18.000000 ats_case-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:45:08.246277 ats_case-0.9.1/
+-rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.9.1/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.9.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1042 2023-06-20 08:45:08.244275 ats_case-0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.9.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 08:45:07.880602 ats_case-0.9.1/ats_case/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.9.1/ats_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:45:08.073093 ats_case-0.9.1/ats_case/case/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.9.1/ats_case/case/__init__.py
+-rw-rw-rw-   0        0        0    18857 2023-06-19 03:05:41.000000 ats_case-0.9.1/ats_case/case/command.py
+-rw-rw-rw-   0        0        0    12148 2023-06-20 07:39:55.000000 ats_case-0.9.1/ats_case/case/context.py
+-rw-rw-rw-   0        0        0     7868 2023-06-20 08:44:47.000000 ats_case-0.9.1/ats_case/case/executor.py
+-rw-rw-rw-   0        0        0     5654 2023-05-22 01:21:46.000000 ats_case-0.9.1/ats_case/case/translator.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:45:08.134895 ats_case-0.9.1/ats_case/common/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.9.1/ats_case/common/__init__.py
+-rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.9.1/ats_case/common/enum.py
+-rw-rw-rw-   0        0        0      790 2023-04-25 08:30:39.000000 ats_case-0.9.1/ats_case/common/error.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:45:08.193738 ats_case-0.9.1/ats_case/manage/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.9.1/ats_case/manage/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-04-25 06:21:05.000000 ats_case-0.9.1/ats_case/manage/core.py
+-rw-rw-rw-   0        0        0     4039 2023-06-16 06:59:03.000000 ats_case-0.9.1/ats_case/manage/start.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:45:08.225685 ats_case-0.9.1/ats_case/template/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.9.1/ats_case/template/__init__.py
+-rw-rw-rw-   0        0        0     2400 2023-05-29 01:45:03.000000 ats_case-0.9.1/ats_case/template/testcase_v1.tmp
+drwxrwxrwx   0        0        0        0 2023-06-20 08:45:07.968376 ats_case-0.9.1/ats_case.egg-info/
+-rw-rw-rw-   0        0        0     1042 2023-06-20 08:45:07.000000 ats_case-0.9.1/ats_case.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-06-20 08:45:07.000000 ats_case-0.9.1/ats_case.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 08:45:07.000000 ats_case-0.9.1/ats_case.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-20 08:45:07.000000 ats_case-0.9.1/ats_case.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-20 08:45:07.000000 ats_case-0.9.1/ats_case.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 08:45:08.246277 ats_case-0.9.1/setup.cfg
+-rw-rw-rw-   0        0        0      945 2023-06-20 08:44:54.000000 ats_case-0.9.1/setup.py
```

### Comparing `ats_case-0.9.0/PKG-INFO` & `ats_case-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats_case
-Version: 0.9.0
+Version: 0.9.1
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.9.0/README.md` & `ats_case-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.0/ats_case/case/command.py` & `ats_case-0.9.1/ats_case/case/command.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.0/ats_case/case/context.py` & `ats_case-0.9.1/ats_case/case/context.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.0/ats_case/case/executor.py` & `ats_case-0.9.1/ats_case/case/executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,15 @@
             command.client().message(str(pe)).error(self._context)
             raise AssertionError(str(pe))
         except Exception as e:
             logger.error(str(e))
             command.client().message(str(e)).error(self._context)
             raise AssertionError(str(e))
         finally:
-            if index < (slen - 1):
+            if index < slen:
                 final_step = self._steps[slen-1]
                 if final_step['type'] == 'BENCH':
                     self._context.runtime.step = final_step
                     self.step_exec()
 
     def handle(self):
         pass
```

### Comparing `ats_case-0.9.0/ats_case/case/translator.py` & `ats_case-0.9.1/ats_case/case/translator.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.0/ats_case/common/error.py` & `ats_case-0.9.1/ats_case/common/error.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.0/ats_case/manage/core.py` & `ats_case-0.9.1/ats_case/manage/core.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.0/ats_case/manage/start.py` & `ats_case-0.9.1/ats_case/manage/start.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.0/ats_case/template/testcase_v1.tmp` & `ats_case-0.9.1/ats_case/template/testcase_v1.tmp`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.0/ats_case.egg-info/PKG-INFO` & `ats_case-0.9.1/ats_case.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats-case
-Version: 0.9.0
+Version: 0.9.1
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.9.0/ats_case.egg-info/SOURCES.txt` & `ats_case-0.9.1/ats_case.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ats_case-0.9.0/setup.py` & `ats_case-0.9.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ats_case",
-    version="0.9.0",
+    version="0.9.1",
     py_modules=['ats_case'],
     author="zhangyue",
     author_email="zhangyue@techen.cn",
     description="Test Script Development Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/henry9000/ats_case",
```

