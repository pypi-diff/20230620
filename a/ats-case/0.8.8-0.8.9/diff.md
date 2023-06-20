# Comparing `tmp/ats_case-0.8.8.tar.gz` & `tmp/ats_case-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ats_case-0.8.8.tar", last modified: Mon Jun 19 03:08:01 2023, max compression
+gzip compressed data, was "ats_case-0.8.9.tar", last modified: Tue Jun 20 08:35:46 2023, max compression
```

## Comparing `ats_case-0.8.8.tar` & `ats_case-0.8.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 03:08:01.526783 ats_case-0.8.8/
--rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.8.8/LICENSE
--rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.8.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1042 2023-06-19 03:08:01.524815 ats_case-0.8.8/PKG-INFO
--rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.8.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 03:08:01.142668 ats_case-0.8.8/ats_case/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.8.8/ats_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 03:08:01.350217 ats_case-0.8.8/ats_case/case/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.8.8/ats_case/case/__init__.py
--rw-rw-rw-   0        0        0    18857 2023-06-19 03:05:41.000000 ats_case-0.8.8/ats_case/case/command.py
--rw-rw-rw-   0        0        0    12042 2023-06-17 06:14:22.000000 ats_case-0.8.8/ats_case/case/context.py
--rw-rw-rw-   0        0        0     7505 2023-06-15 02:18:37.000000 ats_case-0.8.8/ats_case/case/executor.py
--rw-rw-rw-   0        0        0     5654 2023-05-22 01:21:46.000000 ats_case-0.8.8/ats_case/case/translator.py
-drwxrwxrwx   0        0        0        0 2023-06-19 03:08:01.415588 ats_case-0.8.8/ats_case/common/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.8.8/ats_case/common/__init__.py
--rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.8.8/ats_case/common/enum.py
--rw-rw-rw-   0        0        0      790 2023-04-25 08:30:39.000000 ats_case-0.8.8/ats_case/common/error.py
-drwxrwxrwx   0        0        0        0 2023-06-19 03:08:01.477913 ats_case-0.8.8/ats_case/manage/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.8.8/ats_case/manage/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-04-25 06:21:05.000000 ats_case-0.8.8/ats_case/manage/core.py
--rw-rw-rw-   0        0        0     4039 2023-06-16 06:59:03.000000 ats_case-0.8.8/ats_case/manage/start.py
-drwxrwxrwx   0        0        0        0 2023-06-19 03:08:01.516811 ats_case-0.8.8/ats_case/template/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.8.8/ats_case/template/__init__.py
--rw-rw-rw-   0        0        0     2400 2023-05-29 01:45:03.000000 ats_case-0.8.8/ats_case/template/testcase_v1.tmp
-drwxrwxrwx   0        0        0        0 2023-06-19 03:08:01.233518 ats_case-0.8.8/ats_case.egg-info/
--rw-rw-rw-   0        0        0     1042 2023-06-19 03:08:00.000000 ats_case-0.8.8/ats_case.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-06-19 03:08:00.000000 ats_case-0.8.8/ats_case.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 03:08:00.000000 ats_case-0.8.8/ats_case.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-06-19 03:08:00.000000 ats_case-0.8.8/ats_case.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-19 03:08:00.000000 ats_case-0.8.8/ats_case.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 03:08:01.526783 ats_case-0.8.8/setup.cfg
--rw-rw-rw-   0        0        0      945 2023-06-19 02:42:21.000000 ats_case-0.8.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:35:46.941482 ats_case-0.8.9/
+-rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.8.9/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.8.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1042 2023-06-20 08:35:46.938479 ats_case-0.8.9/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.8.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 08:35:46.522778 ats_case-0.8.9/ats_case/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.8.9/ats_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:35:46.759067 ats_case-0.8.9/ats_case/case/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.8.9/ats_case/case/__init__.py
+-rw-rw-rw-   0        0        0    18857 2023-06-19 03:05:41.000000 ats_case-0.8.9/ats_case/case/command.py
+-rw-rw-rw-   0        0        0    12148 2023-06-20 07:39:55.000000 ats_case-0.8.9/ats_case/case/context.py
+-rw-rw-rw-   0        0        0     7958 2023-06-20 08:34:29.000000 ats_case-0.8.9/ats_case/case/executor.py
+-rw-rw-rw-   0        0        0     5654 2023-05-22 01:21:46.000000 ats_case-0.8.9/ats_case/case/translator.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:35:46.828123 ats_case-0.8.9/ats_case/common/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.8.9/ats_case/common/__init__.py
+-rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.8.9/ats_case/common/enum.py
+-rw-rw-rw-   0        0        0      790 2023-04-25 08:30:39.000000 ats_case-0.8.9/ats_case/common/error.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:35:46.891934 ats_case-0.8.9/ats_case/manage/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.8.9/ats_case/manage/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-04-25 06:21:05.000000 ats_case-0.8.9/ats_case/manage/core.py
+-rw-rw-rw-   0        0        0     4039 2023-06-16 06:59:03.000000 ats_case-0.8.9/ats_case/manage/start.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:35:46.930202 ats_case-0.8.9/ats_case/template/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.8.9/ats_case/template/__init__.py
+-rw-rw-rw-   0        0        0     2400 2023-05-29 01:45:03.000000 ats_case-0.8.9/ats_case/template/testcase_v1.tmp
+drwxrwxrwx   0        0        0        0 2023-06-20 08:35:46.633402 ats_case-0.8.9/ats_case.egg-info/
+-rw-rw-rw-   0        0        0     1042 2023-06-20 08:35:45.000000 ats_case-0.8.9/ats_case.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-06-20 08:35:46.000000 ats_case-0.8.9/ats_case.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 08:35:45.000000 ats_case-0.8.9/ats_case.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-20 08:35:45.000000 ats_case-0.8.9/ats_case.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-20 08:35:46.000000 ats_case-0.8.9/ats_case.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 08:35:46.941482 ats_case-0.8.9/setup.cfg
+-rw-rw-rw-   0        0        0      945 2023-06-20 07:40:50.000000 ats_case-0.8.9/setup.py
```

### Comparing `ats_case-0.8.8/PKG-INFO` & `ats_case-0.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats_case
-Version: 0.8.8
+Version: 0.8.9
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.8.8/README.md` & `ats_case-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.8/ats_case/case/command.py` & `ats_case-0.8.9/ats_case/case/command.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.8/ats_case/case/context.py` & `ats_case-0.8.9/ats_case/case/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         self._renew = tl.get('renew', 0)
         self._mode = WorkMode(tl.get('mode'))
         self._tester = self.Tester(tl.get('tester'))
         self._case = self.Case(tl.get('usercase'))
         self._meter = self.Meter(tl.get('meter'))
         self._bench = self.Bench(tl.get('bench'))
         # 运行时
-        self._runtime = self.Runtime()
+        self._runtime = self.Runtime(self)
         self._session = self.Session(self)
         # Debug模式 - 测试开发人员本机调试数据比对服务使用
         self._acd_url = tl.get('acd_url')
 
     @property
     def mode(self):
         return self._mode
@@ -313,21 +313,23 @@
             return self._iabc
 
     class Runtime(object):
         """
         运行时
         """
 
-        def __init__(self):
+        def __init__(self, parent):
+            self._parent = parent
             self._step = -1
             self._loop_sn = 0
             self._loop_start_step = 0
             self._loop_end_step = 0
             self._loop_count = 0
             self._loop_index = 0
+            # 解帧结果
             self._steps = {}
             # 多帧时使用
             self._final_result = None
             # 对比结果 - 用例结束时统计执行结果
             self._acvs = {}
 
         def acv_result(self):
@@ -336,17 +338,17 @@
             for s, result in self.acvs.items():
                 if str(result).find('不合格') >= 0:
                     fc += 1
                     fs.append(str(s))
                 else:
                     sc += 1
 
-            msg = '步骤: {}步\r\n'.format(len(self._acvs))
-            msg += '合格: {}步\r\n'.format(sc)
-            msg += '不合格: {}步 ~ {}\r\n'.format(fc, ','.join(fs))
+            msg = '本用例共: {}步\r\n'.format(len(self._parent.case.steps))
+            msg += '执行合格: {}步\r\n'.format(sc)
+            msg += '执行不合格: {}步 ~ {}\r\n'.format(fc, ','.join(fs))
 
             return msg
 
         @property
         def step(self):
             return self._step
```

### Comparing `ats_case-0.8.8/ats_case/case/executor.py` & `ats_case-0.8.9/ats_case/case/executor.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,54 +7,61 @@
 from ats_case.case import translator, command
 from ats_case.case.context import Context
 from ats_case.common.enum import *
 from ats_case.common.error import *
 
 
 def execute(context: Context):
-    try:
-        if context.mode == WorkMode.FORMAL:
-            FormalExecutor(context).exec()
-        else:
-            DebugExecutor(context).exec()
-    except APIError as ae:
-        logger.info(str(ae))
-        raise AssertionError(str(ae))
-    except ClientError as ce:
-        logger.info(str(ce))
-        command.client().message(str(ce)).error(context)
-        raise AssertionError(str(ce))
-    except MeterOperationError as pe:
-        logger.info(str(pe))
-        command.client().message(str(pe)).error(context)
-        raise AssertionError(str(pe))
-    except Exception as e:
-        logger.error(str(e))
-        command.client().message(str(e)).error(context)
-        raise AssertionError(str(e))
+    if context.mode == WorkMode.FORMAL:
+        FormalExecutor(context).exec()
+    else:
+        DebugExecutor(context).exec()
 
 
 class Executor(object):
     def __init__(self, context: Context):
         self._context = context
         self._model = None
         self._steps = []
 
     def exec(self):
         self.handle()
 
         index = self._load()  # 加载在断点续测时所需关键变量
-        while index < len(self._steps):
-            self._context.runtime.step = self._steps[index]
-            if self.loop_meet():
-                self.loop_exec()
-            else:
-                self.step_exec()
-
-            index = self._steps.index(self._context.runtime.step) + 1
+        slen = len(self._steps)
+        while index < slen:
+            try:
+                self._context.runtime.step = self._steps[index]
+                if self.loop_meet():
+                    self.loop_exec()
+                else:
+                    self.step_exec()
+
+                index = self._steps.index(self._context.runtime.step) + 1
+            except APIError as ae:
+                logger.info(str(ae))
+                raise AssertionError(str(ae))
+            except ClientError as ce:
+                logger.info(str(ce))
+                command.client().message(str(ce)).error(self._context)
+                raise AssertionError(str(ce))
+            except MeterOperationError as pe:
+                logger.info(str(pe))
+                command.client().message(str(pe)).error(self._context)
+                raise AssertionError(str(pe))
+            except Exception as e:
+                logger.error(str(e))
+                command.client().message(str(e)).error(self._context)
+                raise AssertionError(str(e))
+            finally:
+                if index < (slen - 1):
+                    final_step = self._steps[slen-1]
+                    if final_step['type'] == 'BENCH':
+                        self._context.runtime.step = final_step
+                        self.step_exec()
 
     def handle(self):
         pass
 
     def _load(self):
         if self._context.renew == 1:
             self._context.runtime.loop_index = self._context.session.get('breakpoint', 'loop_index')
```

### Comparing `ats_case-0.8.8/ats_case/case/translator.py` & `ats_case-0.8.9/ats_case/case/translator.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.8/ats_case/common/error.py` & `ats_case-0.8.9/ats_case/common/error.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.8/ats_case/manage/core.py` & `ats_case-0.8.9/ats_case/manage/core.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.8/ats_case/manage/start.py` & `ats_case-0.8.9/ats_case/manage/start.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.8/ats_case/template/testcase_v1.tmp` & `ats_case-0.8.9/ats_case/template/testcase_v1.tmp`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.8/ats_case.egg-info/PKG-INFO` & `ats_case-0.8.9/ats_case.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats-case
-Version: 0.8.8
+Version: 0.8.9
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.8.8/ats_case.egg-info/SOURCES.txt` & `ats_case-0.8.9/ats_case.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.8/setup.py` & `ats_case-0.8.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ats_case",
-    version="0.8.8",
+    version="0.8.9",
     py_modules=['ats_case'],
     author="zhangyue",
     author_email="zhangyue@techen.cn",
     description="Test Script Development Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/henry9000/ats_case",
```

