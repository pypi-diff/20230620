# Comparing `tmp/xiaobaisaf-2.1.tar.gz` & `tmp/xiaobaisaf-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiaobaisaf-2.1.tar", last modified: Mon Jun 19 17:16:22 2023, max compression
+gzip compressed data, was "xiaobaisaf-2.2.tar", last modified: Tue Jun 20 02:17:18 2023, max compression
```

## Comparing `xiaobaisaf-2.1.tar` & `xiaobaisaf-2.2.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 17:16:22.707762 xiaobaisaf-2.1/
--rw-rw-rw-   0        0        0    35181 2022-08-20 10:21:11.000000 xiaobaisaf-2.1/LICENSE
--rw-rw-rw-   0        0        0    11342 2023-06-19 17:16:22.707762 xiaobaisaf-2.1/PKG-INFO
--rw-rw-rw-   0        0        0    10673 2023-06-19 16:27:20.000000 xiaobaisaf-2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 17:16:22.681832 xiaobaisaf-2.1/saf/
--rw-rw-rw-   0        0        0     1438 2022-08-28 16:12:42.000000 xiaobaisaf-2.1/saf/__init__.py
--rw-rw-rw-   0        0        0      149 2023-06-19 16:06:24.000000 xiaobaisaf-2.1/saf/__version__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 17:16:22.682829 xiaobaisaf-2.1/saf/data/
--rw-rw-rw-   0        0        0      225 2022-08-23 20:01:48.000000 xiaobaisaf-2.1/saf/data/__init__.py
--rw-rw-rw-   0        0        0     2943 2023-01-11 16:41:44.000000 xiaobaisaf-2.1/saf/data/config.py
-drwxrwxrwx   0        0        0        0 2023-06-19 17:16:22.683826 xiaobaisaf-2.1/saf/example/
--rw-rw-rw-   0        0        0      100 2023-06-14 16:17:05.000000 xiaobaisaf-2.1/saf/example/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 17:16:22.684825 xiaobaisaf-2.1/saf/example/api/
-drwxrwxrwx   0        0        0        0 2023-06-19 17:16:22.685822 xiaobaisaf-2.1/saf/example/api/Config/
--rw-rw-rw-   0        0        0      131 2023-01-13 16:05:35.000000 xiaobaisaf-2.1/saf/example/api/Config/__init__.py
--rw-rw-rw-   0        0        0     5086 2023-01-13 17:38:57.000000 xiaobaisaf-2.1/saf/example/api/Config/config.py
-drwxrwxrwx   0        0        0        0 2023-06-19 17:16:22.686819 xiaobaisaf-2.1/saf/example/api/TestCases/
--rw-rw-rw-   0        0        0      129 2023-01-13 15:48:21.000000 xiaobaisaf-2.1/saf/example/api/TestCases/__init__.py
--rw-rw-rw-   0        0        0     1438 2023-01-13 17:27:45.000000 xiaobaisaf-2.1/saf/example/api/TestCases/test_one_html_case_template.py
-drwxrwxrwx   0        0        0        0 2023-06-19 17:16:22.688814 xiaobaisaf-2.1/saf/example/api/Utils/
--rw-rw-rw-   0        0        0      131 2023-01-13 15:48:21.000000 xiaobaisaf-2.1/saf/example/api/Utils/ExcelUtils.py
--rw-rw-rw-   0        0        0     2099 2023-01-13 16:05:35.000000 xiaobaisaf-2.1/saf/example/api/Utils/YamlUtils.py
--rw-rw-rw-   0        0        0      308 2023-01-13 16:05:35.000000 xiaobaisaf-2.1/saf/example/api/Utils/__init__.py
--rw-rw-rw-   0        0        0      250 2023-01-13 15:48:21.000000 xiaobaisaf-2.1/saf/example/api/Utils/myRequest.py
--rw-rw-rw-   0        0        0      129 2023-01-13 15:52:50.000000 xiaobaisaf-2.1/saf/example/api/__init__.py
--rw-rw-rw-   0        0        0     1211 2023-01-13 17:41:51.000000 xiaobaisaf-2.1/saf/example/api/run.py
--rw-rw-rw-   0        0        0      549 2023-01-13 17:41:51.000000 xiaobaisaf-2.1/saf/example/api/send_email_script.py
-drwxrwxrwx   0        0        0        0 2023-06-19 17:16:22.688814 xiaobaisaf-2.1/saf/example/web/
-drwxrwxrwx   0        0        0        0 2023-06-19 17:16:22.691805 xiaobaisaf-2.1/saf/example/web/Cases/
--rw-rw-rw-   0        0        0      140 2023-01-11 16:41:45.000000 xiaobaisaf-2.1/saf/example/web/Cases/__init__.py
--rw-rw-rw-   0        0        0     2441 2023-06-14 07:25:00.000000 xiaobaisaf-2.1/saf/example/web/Cases/conftest.py
--rw-rw-rw-   0        0        0      930 2023-01-11 16:41:45.000000 xiaobaisaf-2.1/saf/example/web/Cases/test_xiaobai_case_allure.py
--rw-rw-rw-   0        0        0      962 2023-01-11 16:41:45.000000 xiaobaisaf-2.1/saf/example/web/Cases/test_xiaobai_case_submitBug.py
--rw-rw-rw-   0        0        0      320 2023-01-11 16:41:45.000000 xiaobaisaf-2.1/saf/example/web/Cases/test_xiaobai_case_v1.py
--rw-rw-rw-   0        0        0     1192 2023-01-11 16:41:45.000000 xiaobaisaf-2.1/saf/example/web/Cases/test_xiaobai_case_v2.py
--rw-rw-rw-   0        0        0      228 2023-01-11 16:41:45.000000 xiaobaisaf-2.1/saf/example/web/Cases/test_xiaobai_case_v3.py
--rw-rw-rw-   0        0        0      435 2023-01-11 16:41:45.000000 xiaobaisaf-2.1/saf/example/web/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 17:16:22.692803 xiaobaisaf-2.1/saf/example/web/pageObject/
--rw-rw-rw-   0        0        0      166 2023-01-11 16:41:45.000000 xiaobaisaf-2.1/saf/example/web/pageObject/__init__.py
--rw-rw-rw-   0        0        0      152 2023-01-11 16:41:45.000000 xiaobaisaf-2.1/saf/example/web/pageObject/register_page_element.py
-drwxrwxrwx   0        0        0        0 2023-06-19 17:16:22.699784 xiaobaisaf-2.1/saf/utils/
--rw-rw-rw-   0        0        0     8132 2023-01-11 16:41:44.000000 xiaobaisaf-2.1/saf/utils/BugUtils.py
--rw-rw-rw-   0        0        0      126 2023-06-19 17:16:21.000000 xiaobaisaf-2.1/saf/utils/Demo.py
--rw-rw-rw-   0        0        0     2042 2023-06-19 17:15:58.000000 xiaobaisaf-2.1/saf/utils/MonitorAndroidDeviceGUI.py
--rw-rw-rw-   0        0        0     8917 2023-06-19 14:02:01.000000 xiaobaisaf-2.1/saf/utils/MonitorAndroidPackageCLI.py
--rw-rw-rw-   0        0        0    14192 2023-06-19 14:02:01.000000 xiaobaisaf-2.1/saf/utils/MonitorAndroidPackageGUI.py
--rw-rw-rw-   0        0        0     2099 2023-01-13 16:05:35.000000 xiaobaisaf-2.1/saf/utils/YamlUtils.py
--rw-rw-rw-   0        0        0      201 2022-08-21 10:03:39.000000 xiaobaisaf-2.1/saf/utils/__init__.py
--rw-rw-rw-   0        0        0      129 2023-01-11 16:41:45.000000 xiaobaisaf-2.1/saf/utils/downloadUtils.py
--rw-rw-rw-   0        0        0     1271 2022-08-28 16:12:42.000000 xiaobaisaf-2.1/saf/utils/elementUtils.py
--rw-rw-rw-   0        0        0      660 2022-08-28 15:59:39.000000 xiaobaisaf-2.1/saf/utils/imageUtils.py
--rw-rw-rw-   0        0        0     1369 2022-08-28 16:52:51.000000 xiaobaisaf-2.1/saf/utils/networkSpeedUtils.py
--rw-rw-rw-   0        0        0      166 2023-01-11 16:41:45.000000 xiaobaisaf-2.1/saf/utils/osEnvUtils.py
--rw-rw-rw-   0        0        0     8924 2023-06-14 07:25:00.000000 xiaobaisaf-2.1/saf/utils/selenium2POM.py
--rw-rw-rw-   0        0        0     2694 2022-08-28 15:34:31.000000 xiaobaisaf-2.1/saf/utils/sendMsgUtils.py
--rw-rw-rw-   0        0        0     2338 2023-06-19 16:27:20.000000 xiaobaisaf-2.1/saf/utils/xiaobaicmd.py
--rw-rw-rw-   0        0        0       42 2023-06-19 17:16:22.707762 xiaobaisaf-2.1/setup.cfg
--rw-rw-rw-   0        0        0     2239 2023-06-15 15:15:26.000000 xiaobaisaf-2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 17:16:22.706766 xiaobaisaf-2.1/xiaobaisaf.egg-info/
--rw-rw-rw-   0        0        0    11342 2023-06-19 17:16:22.000000 xiaobaisaf-2.1/xiaobaisaf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1556 2023-06-19 17:16:22.000000 xiaobaisaf-2.1/xiaobaisaf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 17:16:22.000000 xiaobaisaf-2.1/xiaobaisaf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-06-19 17:16:22.000000 xiaobaisaf-2.1/xiaobaisaf.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       98 2023-06-19 17:16:22.000000 xiaobaisaf-2.1/xiaobaisaf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-19 17:16:22.000000 xiaobaisaf-2.1/xiaobaisaf.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 02:17:18.849261 xiaobaisaf-2.2/
+-rw-rw-rw-   0        0        0    35181 2023-06-15 01:06:25.000000 xiaobaisaf-2.2/LICENSE
+-rw-rw-rw-   0        0        0    11428 2023-06-20 02:17:18.849261 xiaobaisaf-2.2/PKG-INFO
+-rw-rw-rw-   0        0        0    10720 2023-06-20 01:46:56.000000 xiaobaisaf-2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 02:17:18.802209 xiaobaisaf-2.2/saf/
+-rw-rw-rw-   0        0        0     1438 2023-06-15 01:06:25.000000 xiaobaisaf-2.2/saf/__init__.py
+-rw-rw-rw-   0        0        0      149 2023-06-20 01:46:56.000000 xiaobaisaf-2.2/saf/__version__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 02:17:18.817796 xiaobaisaf-2.2/saf/data/
+-rw-rw-rw-   0        0        0      225 2023-06-15 01:06:25.000000 xiaobaisaf-2.2/saf/data/__init__.py
+-rw-rw-rw-   0        0        0     2943 2023-06-15 01:06:25.000000 xiaobaisaf-2.2/saf/data/config.py
+-rw-rw-rw-   0        0        0     4286 2022-02-27 16:38:48.000000 xiaobaisaf-2.2/saf/data/favicon.ico
+drwxrwxrwx   0        0        0        0 2023-06-20 02:17:18.817796 xiaobaisaf-2.2/saf/example/
+-rw-rw-rw-   0        0        0      100 2023-06-15 01:06:25.000000 xiaobaisaf-2.2/saf/example/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 02:17:18.817796 xiaobaisaf-2.2/saf/example/api/
+drwxrwxrwx   0        0        0        0 2023-06-20 02:17:18.817796 xiaobaisaf-2.2/saf/example/api/Config/
+-rw-rw-rw-   0        0        0      131 2023-06-15 01:06:25.000000 xiaobaisaf-2.2/saf/example/api/Config/__init__.py
+-rw-rw-rw-   0        0        0     5086 2023-06-15 01:06:25.000000 xiaobaisaf-2.2/saf/example/api/Config/config.py
+drwxrwxrwx   0        0        0        0 2023-06-20 02:17:18.817796 xiaobaisaf-2.2/saf/example/api/TestCases/
+-rw-rw-rw-   0        0        0      129 2023-06-15 01:06:25.000000 xiaobaisaf-2.2/saf/example/api/TestCases/__init__.py
+-rw-rw-rw-   0        0        0     1438 2023-06-15 01:06:25.000000 xiaobaisaf-2.2/saf/example/api/TestCases/test_one_html_case_template.py
+drwxrwxrwx   0        0        0        0 2023-06-20 02:17:18.817796 xiaobaisaf-2.2/saf/example/api/Utils/
+-rw-rw-rw-   0        0        0      131 2023-06-15 01:06:25.000000 xiaobaisaf-2.2/saf/example/api/Utils/ExcelUtils.py
+-rw-rw-rw-   0        0        0     2099 2023-06-15 01:06:25.000000 xiaobaisaf-2.2/saf/example/api/Utils/YamlUtils.py
+-rw-rw-rw-   0        0        0      308 2023-06-15 01:06:25.000000 xiaobaisaf-2.2/saf/example/api/Utils/__init__.py
+-rw-rw-rw-   0        0        0      250 2023-06-15 01:06:25.000000 xiaobaisaf-2.2/saf/example/api/Utils/myRequest.py
+-rw-rw-rw-   0        0        0      129 2023-06-15 01:06:25.000000 xiaobaisaf-2.2/saf/example/api/__init__.py
+-rw-rw-rw-   0        0        0     1211 2023-06-15 01:06:25.000000 xiaobaisaf-2.2/saf/example/api/run.py
+-rw-rw-rw-   0        0        0      549 2023-06-15 01:06:25.000000 xiaobaisaf-2.2/saf/example/api/send_email_script.py
+drwxrwxrwx   0        0        0        0 2023-06-20 02:17:18.817796 xiaobaisaf-2.2/saf/example/web/
+drwxrwxrwx   0        0        0        0 2023-06-20 02:17:18.817796 xiaobaisaf-2.2/saf/example/web/Cases/
+-rw-rw-rw-   0        0        0      140 2023-06-15 01:06:25.000000 xiaobaisaf-2.2/saf/example/web/Cases/__init__.py
+-rw-rw-rw-   0        0        0     2441 2023-06-15 01:06:25.000000 xiaobaisaf-2.2/saf/example/web/Cases/conftest.py
+-rw-rw-rw-   0        0        0      930 2023-06-15 01:06:25.000000 xiaobaisaf-2.2/saf/example/web/Cases/test_xiaobai_case_allure.py
+-rw-rw-rw-   0        0        0      962 2023-06-15 01:06:25.000000 xiaobaisaf-2.2/saf/example/web/Cases/test_xiaobai_case_submitBug.py
+-rw-rw-rw-   0        0        0      320 2023-06-15 01:06:25.000000 xiaobaisaf-2.2/saf/example/web/Cases/test_xiaobai_case_v1.py
+-rw-rw-rw-   0        0        0     1192 2023-06-15 01:06:25.000000 xiaobaisaf-2.2/saf/example/web/Cases/test_xiaobai_case_v2.py
+-rw-rw-rw-   0        0        0      228 2023-06-15 01:06:25.000000 xiaobaisaf-2.2/saf/example/web/Cases/test_xiaobai_case_v3.py
+-rw-rw-rw-   0        0        0      435 2023-06-15 01:06:25.000000 xiaobaisaf-2.2/saf/example/web/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 02:17:18.817796 xiaobaisaf-2.2/saf/example/web/pageObject/
+-rw-rw-rw-   0        0        0      166 2023-06-15 01:06:25.000000 xiaobaisaf-2.2/saf/example/web/pageObject/__init__.py
+-rw-rw-rw-   0        0        0      152 2023-06-15 01:06:25.000000 xiaobaisaf-2.2/saf/example/web/pageObject/register_page_element.py
+drwxrwxrwx   0        0        0        0 2023-06-20 02:17:18.834254 xiaobaisaf-2.2/saf/utils/
+-rw-rw-rw-   0        0        0     8132 2023-06-15 01:06:25.000000 xiaobaisaf-2.2/saf/utils/BugUtils.py
+-rw-rw-rw-   0        0        0     2074 2023-06-20 02:13:02.000000 xiaobaisaf-2.2/saf/utils/MonitorAndroidDeviceGUI.py
+-rw-rw-rw-   0        0        0     8917 2023-06-20 01:30:52.000000 xiaobaisaf-2.2/saf/utils/MonitorAndroidPackageCLI.py
+-rw-rw-rw-   0        0        0    14192 2023-06-20 01:30:52.000000 xiaobaisaf-2.2/saf/utils/MonitorAndroidPackageGUI.py
+-rw-rw-rw-   0        0        0     2099 2023-06-15 01:06:25.000000 xiaobaisaf-2.2/saf/utils/YamlUtils.py
+-rw-rw-rw-   0        0        0      201 2023-06-15 01:06:25.000000 xiaobaisaf-2.2/saf/utils/__init__.py
+-rw-rw-rw-   0        0        0      129 2023-06-15 01:06:25.000000 xiaobaisaf-2.2/saf/utils/downloadUtils.py
+-rw-rw-rw-   0        0        0     1271 2023-06-15 01:06:25.000000 xiaobaisaf-2.2/saf/utils/elementUtils.py
+-rw-rw-rw-   0        0        0      660 2023-06-15 01:06:25.000000 xiaobaisaf-2.2/saf/utils/imageUtils.py
+-rw-rw-rw-   0        0        0     1369 2023-06-15 01:06:25.000000 xiaobaisaf-2.2/saf/utils/networkSpeedUtils.py
+-rw-rw-rw-   0        0        0      166 2023-06-15 01:06:25.000000 xiaobaisaf-2.2/saf/utils/osEnvUtils.py
+-rw-rw-rw-   0        0        0     8924 2023-06-15 01:06:25.000000 xiaobaisaf-2.2/saf/utils/selenium2POM.py
+-rw-rw-rw-   0        0        0     2694 2023-06-15 01:06:25.000000 xiaobaisaf-2.2/saf/utils/sendMsgUtils.py
+-rw-rw-rw-   0        0        0     2338 2023-06-20 01:30:52.000000 xiaobaisaf-2.2/saf/utils/xiaobaicmd.py
+-rw-rw-rw-   0        0        0       42 2023-06-20 02:17:18.849261 xiaobaisaf-2.2/setup.cfg
+-rw-rw-rw-   0        0        0     2346 2023-06-20 02:17:17.000000 xiaobaisaf-2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 02:17:18.849261 xiaobaisaf-2.2/xiaobaisaf.egg-info/
+-rw-rw-rw-   0        0        0    11428 2023-06-20 02:17:18.000000 xiaobaisaf-2.2/xiaobaisaf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1559 2023-06-20 02:17:18.000000 xiaobaisaf-2.2/xiaobaisaf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 02:17:18.000000 xiaobaisaf-2.2/xiaobaisaf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-06-20 02:17:18.000000 xiaobaisaf-2.2/xiaobaisaf.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       98 2023-06-20 02:17:18.000000 xiaobaisaf-2.2/xiaobaisaf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-20 02:17:18.000000 xiaobaisaf-2.2/xiaobaisaf.egg-info/top_level.txt
```

### Comparing `xiaobaisaf-2.1/LICENSE` & `xiaobaisaf-2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.1/PKG-INFO` & `xiaobaisaf-2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: xiaobaisaf
-Version: 2.1
+Version: 2.2
 Summary: simple_automation_framework(简称：SAF)使用最简单的模式就可以实现需要功能和测试效果，也是xiaobaiauto2的简化版SAF继承了selenium、requests/httpx、appium、loguru、xiaobaiauto2、飞书机器人、钉钉机器人、企业微信机器人（暂时不支持）、禅道提单API
 Home-page: https://gitee.com/xiaobaikeji/simlpe_automation_framework
 Author: xiaobaiTser
 Author-email: 807447312@qq.com
+License: UNKNOWN
 Keywords: saf test auto automation xiaobai xiaobaiauto2 test framework
+Platform: UNKNOWN
 Requires-Python: >=3.6, <3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # simlpe_automation_framework
 
 ### 介绍
@@ -323,7 +325,9 @@
 | 1.5     | 优化pytest样例内容            |
 | 1.6     | 优化                      |
 | 1.7     | 新增基础环境检测功能              |
 | 1.8     | 新增API自动化模板              |
 | 1.9     | 新增xiaobaicmd -u命令       |
 | 2.0     | 新增xiaobaicmd -m命令       |
 | 2.1     | 新增xiaobaicmd --device命令 |
+| 2.2     | 优化xiaobaicmd --device命令 |
+
```

### Comparing `xiaobaisaf-2.1/README.md` & `xiaobaisaf-2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -310,8 +310,9 @@
 | 1.4     | 新增pytest参数化样例           |
 | 1.5     | 优化pytest样例内容            |
 | 1.6     | 优化                      |
 | 1.7     | 新增基础环境检测功能              |
 | 1.8     | 新增API自动化模板              |
 | 1.9     | 新增xiaobaicmd -u命令       |
 | 2.0     | 新增xiaobaicmd -m命令       |
-| 2.1     | 新增xiaobaicmd --device命令 |
+| 2.1     | 新增xiaobaicmd --device命令 |
+| 2.2     | 优化xiaobaicmd --device命令 |
```

### Comparing `xiaobaisaf-2.1/saf/__init__.py` & `xiaobaisaf-2.2/saf/__init__.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.1/saf/data/config.py` & `xiaobaisaf-2.2/saf/data/config.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.1/saf/example/api/Config/config.py` & `xiaobaisaf-2.2/saf/example/api/Config/config.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.1/saf/example/api/TestCases/test_one_html_case_template.py` & `xiaobaisaf-2.2/saf/example/api/TestCases/test_one_html_case_template.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.1/saf/example/api/Utils/YamlUtils.py` & `xiaobaisaf-2.2/saf/example/api/Utils/YamlUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.1/saf/example/api/run.py` & `xiaobaisaf-2.2/saf/example/api/run.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.1/saf/example/api/send_email_script.py` & `xiaobaisaf-2.2/saf/example/api/send_email_script.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.1/saf/example/web/Cases/conftest.py` & `xiaobaisaf-2.2/saf/example/web/Cases/conftest.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.1/saf/example/web/Cases/test_xiaobai_case_allure.py` & `xiaobaisaf-2.2/saf/example/web/Cases/test_xiaobai_case_allure.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.1/saf/example/web/Cases/test_xiaobai_case_submitBug.py` & `xiaobaisaf-2.2/saf/example/web/Cases/test_xiaobai_case_submitBug.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.1/saf/example/web/Cases/test_xiaobai_case_v2.py` & `xiaobaisaf-2.2/saf/example/web/Cases/test_xiaobai_case_v2.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.1/saf/utils/BugUtils.py` & `xiaobaisaf-2.2/saf/utils/BugUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.1/saf/utils/MonitorAndroidDeviceGUI.py` & `xiaobaisaf-2.2/saf/utils/MonitorAndroidDeviceGUI.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,38 +6,36 @@
 @File  : MonitorAndroidDeviceGUI.py
 '''
 
 import tkinter as tk
 from PIL import Image, ImageTk
 from io import BytesIO
 from adbutils import adb
-from time import time
+import os
 
 class MonitorAndroid:
     def __init__(self, device):
+        CUR_PATH = os.path.dirname(os.path.abspath(__file__))
         # 创建Tkinter界面
         self.root = tk.Tk()
+        self.root.iconbitmap(CUR_PATH + '\\..\\data\\favicon.ico')
 
         # 获取设备的分辨率并设置Tkinter界面的大小
         self.device = device
         width, height = device.window_size()
         self.root.geometry(f'{width // 5}x{height // 5}')
         self.root.resizable(False, False)
         # 标题
         self.root.title(device.serial)
 
         self.label = tk.Label(self.root)
         self.label.pack()
-        self.endTime = time()
         # 开始更新图片
-        try:
-            self.device_screenshot()
-            self.root.mainloop()
-        except KeyboardInterrupt:
-            pass
+        self.device_screenshot()
+        self.root.mainloop()
 
     def device_screenshot(self):
         # 获取Android设备的屏幕截图
         screenshot = self.device.screenshot()
 
         # 将截图转换为字节流
         byte_stream = BytesIO()
@@ -50,17 +48,17 @@
         resized_image = image.resize(new_size)
         photo = ImageTk.PhotoImage(resized_image)
 
         # 更新Tkinter界面的图片
         self.label.config(image=photo)
         self.label.image = photo
 
-        self.endTime = time()
         # 每1毫秒更新一次图片
-        self.label.after(1, self.device_screenshot)
+        self.label.after(100, self.device_screenshot)
 
 def MonitorDevice(index: int = 0):
-    print(f'开始监控设备...')
     devices = adb.device_list()
     print(f'设备列表：{devices}，您选择的是第{index+1}个')
-    if len(devices) > 0:
-        MonitorAndroid(device=devices[index])
+    if len(devices) > 0 and index < len(devices):
+        MonitorAndroid(device=devices[index])
+    else:
+        print('您选择了无效的序号！')
```

### Comparing `xiaobaisaf-2.1/saf/utils/MonitorAndroidPackageCLI.py` & `xiaobaisaf-2.2/saf/utils/MonitorAndroidPackageCLI.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     'appActivity': {activity_name},
     # 'noReset': True,
     # 'dontStopAppOnReset': True,
     'unicodeKeyboard': True,
     'resetKeyboard': True
 }}
 
-app = webdriver.Remote("http://localhost:4723/wd/hub", caps)
+app = webdriver.Remote("http://127.0.0.1:4723/wd/hub", caps)
 
 # 下面为定位表达式
 ''')
     deviceName = device.serial
     # 启动getevent命令
     event_cmd = f"adb -s {deviceName} shell getevent -lt /dev/input/event1"
     process = subprocess.Popen(event_cmd, stdout=subprocess.PIPE, shell=True)
```

### Comparing `xiaobaisaf-2.1/saf/utils/MonitorAndroidPackageGUI.py` & `xiaobaisaf-2.2/saf/utils/MonitorAndroidPackageGUI.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.1/saf/utils/YamlUtils.py` & `xiaobaisaf-2.2/saf/utils/YamlUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.1/saf/utils/elementUtils.py` & `xiaobaisaf-2.2/saf/utils/elementUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.1/saf/utils/imageUtils.py` & `xiaobaisaf-2.2/saf/utils/imageUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.1/saf/utils/networkSpeedUtils.py` & `xiaobaisaf-2.2/saf/utils/networkSpeedUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.1/saf/utils/selenium2POM.py` & `xiaobaisaf-2.2/saf/utils/selenium2POM.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.1/saf/utils/sendMsgUtils.py` & `xiaobaisaf-2.2/saf/utils/sendMsgUtils.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.1/saf/utils/xiaobaicmd.py` & `xiaobaisaf-2.2/saf/utils/xiaobaicmd.py`

 * *Files identical despite different names*

### Comparing `xiaobaisaf-2.1/setup.py` & `xiaobaisaf-2.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     author_email='807447312@qq.com',
     # 写上项目的地址。
     url='https://gitee.com/xiaobaikeji/simlpe_automation_framework',
     # 指定包名，即你需要打包的包名称，要实际在你本地存在哟，它会将指定包名下的所有"*.py"文件进行打包哟，但不会递归去拷贝所有的子包内容。
     # 综上所述，我们如果想要把一个包的所有"*.py"文件进行打包，应该在packages列表写下所有包的层级关系哟~这样就开源将指定包路径的所有".py"文件进行打包!
     keywords="saf test auto automation xiaobai xiaobaiauto2 test framework",
     packages=find_packages(),
+    include_package_data = True,
     # 指定Python的版本
     python_requires='>=3.6, <3.10',
     install_requires=[
         'adbutils',
         'allure-pytest',
         'ddddocr',
         'loguru',
@@ -47,13 +48,16 @@
         'xiaobaiauto2',
     ],
     entry_points={
         'console_scripts': [
             'xiaobaicmd = saf.utils.xiaobaicmd:main'
         ]
     },
+    data_files=[
+        ('favicon', ['saf/data/favicon.ico']),
+    ]
 )
 
 '''
 #python setup.py sdist bdist_wheel
 #python -m twine upload dist/*
 '''
```

### Comparing `xiaobaisaf-2.1/xiaobaisaf.egg-info/PKG-INFO` & `xiaobaisaf-2.2/xiaobaisaf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: xiaobaisaf
-Version: 2.1
+Version: 2.2
 Summary: simple_automation_framework(简称：SAF)使用最简单的模式就可以实现需要功能和测试效果，也是xiaobaiauto2的简化版SAF继承了selenium、requests/httpx、appium、loguru、xiaobaiauto2、飞书机器人、钉钉机器人、企业微信机器人（暂时不支持）、禅道提单API
 Home-page: https://gitee.com/xiaobaikeji/simlpe_automation_framework
 Author: xiaobaiTser
 Author-email: 807447312@qq.com
+License: UNKNOWN
 Keywords: saf test auto automation xiaobai xiaobaiauto2 test framework
+Platform: UNKNOWN
 Requires-Python: >=3.6, <3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # simlpe_automation_framework
 
 ### 介绍
@@ -323,7 +325,9 @@
 | 1.5     | 优化pytest样例内容            |
 | 1.6     | 优化                      |
 | 1.7     | 新增基础环境检测功能              |
 | 1.8     | 新增API自动化模板              |
 | 1.9     | 新增xiaobaicmd -u命令       |
 | 2.0     | 新增xiaobaicmd -m命令       |
 | 2.1     | 新增xiaobaicmd --device命令 |
+| 2.2     | 优化xiaobaicmd --device命令 |
+
```

### Comparing `xiaobaisaf-2.1/xiaobaisaf.egg-info/SOURCES.txt` & `xiaobaisaf-2.2/xiaobaisaf.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 setup.py
 saf/__init__.py
 saf/__version__.py
 saf/data/__init__.py
 saf/data/config.py
+saf/data/favicon.ico
 saf/example/__init__.py
 saf/example/api/__init__.py
 saf/example/api/run.py
 saf/example/api/send_email_script.py
 saf/example/api/Config/__init__.py
 saf/example/api/Config/config.py
 saf/example/api/TestCases/__init__.py
@@ -24,15 +25,14 @@
 saf/example/web/Cases/test_xiaobai_case_submitBug.py
 saf/example/web/Cases/test_xiaobai_case_v1.py
 saf/example/web/Cases/test_xiaobai_case_v2.py
 saf/example/web/Cases/test_xiaobai_case_v3.py
 saf/example/web/pageObject/__init__.py
 saf/example/web/pageObject/register_page_element.py
 saf/utils/BugUtils.py
-saf/utils/Demo.py
 saf/utils/MonitorAndroidDeviceGUI.py
 saf/utils/MonitorAndroidPackageCLI.py
 saf/utils/MonitorAndroidPackageGUI.py
 saf/utils/YamlUtils.py
 saf/utils/__init__.py
 saf/utils/downloadUtils.py
 saf/utils/elementUtils.py
```

