# Comparing `tmp/python_selenium_ctrl_package-0.0.98.tar.gz` & `tmp/python_selenium_ctrl_package-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_selenium_ctrl_package-0.0.98.tar", last modified: Mon Apr 24 02:25:27 2023, max compression
+gzip compressed data, was "python_selenium_ctrl_package-0.0.99.tar", last modified: Tue Apr 25 07:37:47 2023, max compression
```

## Comparing `python_selenium_ctrl_package-0.0.98.tar` & `python_selenium_ctrl_package-0.0.99.tar`

### file list

```diff
@@ -1,60 +1,59 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 02:25:27.606095 python_selenium_ctrl_package-0.0.98/
--rw-rw-rw-   0        0        0     1061 2022-11-15 08:59:32.000000 python_selenium_ctrl_package-0.0.98/LICENSE
--rw-rw-rw-   0        0        0     1172 2023-04-24 02:25:27.606095 python_selenium_ctrl_package-0.0.98/PKG-INFO
--rw-rw-rw-   0        0        0      681 2023-04-19 08:10:05.000000 python_selenium_ctrl_package-0.0.98/README.md
--rw-rw-rw-   0        0        0      942 2023-04-24 02:25:06.000000 python_selenium_ctrl_package-0.0.98/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-24 02:25:27.606095 python_selenium_ctrl_package-0.0.98/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-24 02:25:27.400556 python_selenium_ctrl_package-0.0.98/src/
--rw-rw-rw-   0        0        0        0 2022-11-18 06:36:28.000000 python_selenium_ctrl_package-0.0.98/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 02:25:27.419555 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/
--rw-rw-rw-   0        0        0        0 2022-11-17 01:43:31.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 02:25:27.448606 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/conf/
--rw-rw-rw-   0        0        0        0 2022-11-21 09:26:54.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/conf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 02:25:27.456630 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/conf/app/
--rw-rw-rw-   0        0        0        0 2022-11-21 09:42:24.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/conf/app/__init__.py
--rw-rw-rw-   0        0        0       90 2022-10-07 06:37:19.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/conf/app/ports_conf.py
--rw-rw-rw-   0        0        0      166 2022-10-07 06:37:19.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/conf/product_list.py
-drwxrwxrwx   0        0        0        0 2023-04-24 02:25:27.457585 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/conf/rwd/
-drwxrwxrwx   0        0        0        0 2023-04-24 02:25:27.473586 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/conf/rwd/Website/
--rw-rw-rw-   0        0        0        0 2022-11-21 09:27:37.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/conf/rwd/Website/__init__.py
--rw-rw-rw-   0        0        0      153 2022-10-07 06:37:19.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/conf/rwd/Website/base_url_conf.py
--rw-rw-rw-   0        0        0      104 2022-10-07 06:37:19.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/conf/rwd/Website/opera_browser_conf.py
--rw-rw-rw-   0        0        0        0 2022-11-21 09:27:06.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/conf/rwd/__init__.py
--rw-rw-rw-   0        0        0    41277 2023-04-19 07:45:54.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/conftest_base.py
-drwxrwxrwx   0        0        0        0 2023-04-24 02:25:27.483587 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/drivers/
--rw-rw-rw-   0        0        0        0 2022-11-21 09:11:03.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/drivers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 02:25:27.502589 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/drivers/browsers/
--rw-rw-rw-   0        0        0        0 2022-11-21 09:11:28.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/drivers/browsers/__init__.py
--rw-rw-rw-   0        0        0     3897 2022-12-07 03:55:17.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/drivers/browsers/browser_os_name_conf.py
--rw-rw-rw-   0        0        0     3501 2023-04-24 02:24:42.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/drivers/browsers/local_browsers.py
--rw-rw-rw-   0        0        0     5926 2022-11-21 10:05:25.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/drivers/browsers/remote_options.py
--rw-rw-rw-   0        0        0    16954 2023-04-19 08:09:13.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/drivers/driverfactory.py
--rw-rw-rw-   0        0        0      544 2022-11-14 01:59:19.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/main.py
-drwxrwxrwx   0        0        0        0 2023-04-24 02:25:27.530602 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/pages/
--rw-rw-rw-   0        0        0    57659 2023-04-19 07:45:54.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/pages/Base_Page.py
--rw-rw-rw-   0        0        0    25414 2023-04-20 08:32:17.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/pages/Mobile_Base_Page.py
--rw-rw-rw-   0        0        0        0 2022-11-18 06:45:15.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/pages/__init__.py
--rw-rw-rw-   0        0        0      370 2022-11-30 02:56:37.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/pages/mobile_zero_page.py
--rw-rw-rw-   0        0        0      422 2022-11-30 02:10:57.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/pages/zero_page.py
-drwxrwxrwx   0        0        0        0 2023-04-24 02:25:27.541556 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/remoteTest/
--rw-rw-rw-   0        0        0     3816 2022-11-30 06:10:04.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/remoteTest/BrowserStack_Library.py
--rw-rw-rw-   0        0        0        0 2022-11-21 08:57:28.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/remoteTest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 02:25:27.568094 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/utils/
--rw-rw-rw-   0        0        0        0 2022-11-21 08:39:02.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/utils/__init__.py
--rw-rw-rw-   0        0        0      874 2023-01-04 03:46:28.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/utils/email_conf.py
-drwxrwxrwx   0        0        0        0 2023-04-24 02:25:27.604096 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/utils/general/
--rw-rw-rw-   0        0        0     4915 2023-03-23 09:33:36.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/utils/general/Base_Logging.py
--rw-rw-rw-   0        0        0      723 2022-10-07 06:37:19.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/utils/general/Gif_Maker.py
--rw-rw-rw-   0        0        0     8968 2023-04-11 08:09:09.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/utils/general/Wrapit.py
--rw-rw-rw-   0        0        0        0 2022-11-21 08:39:31.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/utils/general/__init__.py
--rw-rw-rw-   0        0        0     9380 2023-01-04 06:33:56.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/utils/general/email_pytest_report.py
--rw-rw-rw-   0        0        0      379 2022-10-07 06:37:19.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/utils/general/stop_test_exception_util.py
--rw-rw-rw-   0        0        0       19 2022-10-12 03:37:41.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/utils/html_report_conf.py
--rw-rw-rw-   0        0        0      227 2022-10-07 06:37:19.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/utils/remote_credentials.py
--rw-rw-rw-   0        0        0       28 2022-11-29 09:59:41.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/utils/screenshot_conf.py
-drwxrwxrwx   0        0        0        0 2023-04-24 02:25:27.444555 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package.egg-info/
--rw-rw-rw-   0        0        0     1172 2023-04-24 02:25:27.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2378 2023-04-24 02:25:27.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 02:25:27.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      272 2023-04-24 02:25:27.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       38 2023-04-24 02:25:27.000000 python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 07:37:47.830901 python_selenium_ctrl_package-0.0.99/
+-rw-rw-rw-   0        0        0     1061 2022-11-15 08:59:32.000000 python_selenium_ctrl_package-0.0.99/LICENSE
+-rw-rw-rw-   0        0        0     1172 2023-04-25 07:37:47.829509 python_selenium_ctrl_package-0.0.99/PKG-INFO
+-rw-rw-rw-   0        0        0      681 2023-04-19 08:10:05.000000 python_selenium_ctrl_package-0.0.99/README.md
+-rw-rw-rw-   0        0        0     1159 2023-04-25 07:37:21.000000 python_selenium_ctrl_package-0.0.99/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-25 07:37:47.831270 python_selenium_ctrl_package-0.0.99/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-25 07:37:47.562401 python_selenium_ctrl_package-0.0.99/src/
+-rw-rw-rw-   0        0        0        0 2022-11-18 06:36:28.000000 python_selenium_ctrl_package-0.0.99/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 07:37:47.585401 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/
+-rw-rw-rw-   0        0        0        0 2022-11-17 01:43:31.000000 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 07:37:47.613401 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/conf/
+-rw-rw-rw-   0        0        0        0 2022-11-21 09:26:54.000000 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/conf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 07:37:47.623400 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/conf/app/
+-rw-rw-rw-   0        0        0        0 2022-11-21 09:42:24.000000 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/conf/app/__init__.py
+-rw-rw-rw-   0        0        0       90 2022-10-07 06:37:19.000000 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/conf/app/ports_conf.py
+-rw-rw-rw-   0        0        0      166 2022-10-07 06:37:19.000000 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/conf/product_list.py
+drwxrwxrwx   0        0        0        0 2023-04-25 07:37:47.624401 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/conf/rwd/
+drwxrwxrwx   0        0        0        0 2023-04-25 07:37:47.640401 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/conf/rwd/Website/
+-rw-rw-rw-   0        0        0        0 2022-11-21 09:27:37.000000 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/conf/rwd/Website/__init__.py
+-rw-rw-rw-   0        0        0      153 2022-10-07 06:37:19.000000 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/conf/rwd/Website/base_url_conf.py
+-rw-rw-rw-   0        0        0      104 2022-10-07 06:37:19.000000 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/conf/rwd/Website/opera_browser_conf.py
+-rw-rw-rw-   0        0        0        0 2022-11-21 09:27:06.000000 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/conf/rwd/__init__.py
+-rw-rw-rw-   0        0        0    40844 2023-04-24 03:01:13.000000 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/conftest_base.py
+drwxrwxrwx   0        0        0        0 2023-04-25 07:37:47.650515 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/drivers/
+-rw-rw-rw-   0        0        0        0 2022-11-21 09:11:03.000000 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/drivers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 07:37:47.681354 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/drivers/browsers/
+-rw-rw-rw-   0        0        0        0 2022-11-21 09:11:28.000000 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/drivers/browsers/__init__.py
+-rw-rw-rw-   0        0        0     3897 2022-12-07 03:55:17.000000 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/drivers/browsers/browser_os_name_conf.py
+-rw-rw-rw-   0        0        0     3501 2023-04-24 02:24:42.000000 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/drivers/browsers/local_browsers.py
+-rw-rw-rw-   0        0        0     5926 2022-11-21 10:05:25.000000 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/drivers/browsers/remote_options.py
+-rw-rw-rw-   0        0        0    16954 2023-04-19 08:09:13.000000 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/drivers/driverfactory.py
+-rw-rw-rw-   0        0        0      544 2022-11-14 01:59:19.000000 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/main.py
+drwxrwxrwx   0        0        0        0 2023-04-25 07:37:47.723927 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/pages/
+-rw-rw-rw-   0        0        0    57659 2023-04-19 07:45:54.000000 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/pages/Base_Page.py
+-rw-rw-rw-   0        0        0    25414 2023-04-20 08:32:17.000000 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/pages/Mobile_Base_Page.py
+-rw-rw-rw-   0        0        0        0 2022-11-18 06:45:15.000000 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/pages/__init__.py
+-rw-rw-rw-   0        0        0      370 2022-11-30 02:56:37.000000 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/pages/mobile_zero_page.py
+-rw-rw-rw-   0        0        0      422 2022-11-30 02:10:57.000000 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/pages/zero_page.py
+drwxrwxrwx   0        0        0        0 2023-04-25 07:37:47.735523 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/remoteTest/
+-rw-rw-rw-   0        0        0     3816 2022-11-30 06:10:04.000000 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/remoteTest/BrowserStack_Library.py
+-rw-rw-rw-   0        0        0        0 2022-11-21 08:57:28.000000 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/remoteTest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 07:37:47.770860 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/utils/
+-rw-rw-rw-   0        0        0        0 2022-11-21 08:39:02.000000 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/utils/__init__.py
+-rw-rw-rw-   0        0        0      874 2023-01-04 03:46:28.000000 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/utils/email_conf.py
+drwxrwxrwx   0        0        0        0 2023-04-25 07:37:47.826083 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/utils/general/
+-rw-rw-rw-   0        0        0     4915 2023-03-23 09:33:36.000000 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/utils/general/Base_Logging.py
+-rw-rw-rw-   0        0        0      723 2022-10-07 06:37:19.000000 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/utils/general/Gif_Maker.py
+-rw-rw-rw-   0        0        0     8968 2023-04-11 08:09:09.000000 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/utils/general/Wrapit.py
+-rw-rw-rw-   0        0        0        0 2022-11-21 08:39:31.000000 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/utils/general/__init__.py
+-rw-rw-rw-   0        0        0     9380 2023-01-04 06:33:56.000000 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/utils/general/email_pytest_report.py
+-rw-rw-rw-   0        0        0      379 2022-10-07 06:37:19.000000 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/utils/general/stop_test_exception_util.py
+-rw-rw-rw-   0        0        0       19 2022-10-12 03:37:41.000000 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/utils/html_report_conf.py
+-rw-rw-rw-   0        0        0      227 2022-10-07 06:37:19.000000 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/utils/remote_credentials.py
+-rw-rw-rw-   0        0        0       28 2022-11-29 09:59:41.000000 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/utils/screenshot_conf.py
+drwxrwxrwx   0        0        0        0 2023-04-25 07:37:47.604401 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package.egg-info/
+-rw-rw-rw-   0        0        0     1172 2023-04-25 07:37:47.000000 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2323 2023-04-25 07:37:47.000000 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 07:37:47.000000 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-04-25 07:37:47.000000 python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package.egg-info/top_level.txt
```

### Comparing `python_selenium_ctrl_package-0.0.98/LICENSE` & `python_selenium_ctrl_package-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `python_selenium_ctrl_package-0.0.98/PKG-INFO` & `python_selenium_ctrl_package-0.0.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python_selenium_ctrl_package
-Version: 0.0.98
+Version: 0.0.99
 Summary: Base_page for selenium automation
 Author-email: "QHMS(App team)" <qhmsqaexpert@gmail.com>
 Keywords: python,automation,appium,selenium,pytest,automation framework
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `python_selenium_ctrl_package-0.0.98/README.md` & `python_selenium_ctrl_package-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/conftest_base.py` & `python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/conftest_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -429,35 +429,28 @@
         parser.addoption("--xlsx",
                          dest="xlsx",
                          default='',
                          help="Excel File name which need to get for config")
         parser.addoption("--case",
                          dest="case",
                          default="-1",
-                         help="Number of case which need to run in Excel config. Do no use this option for running all cases. Input number > 0")
-        parser.addoption("--caseid",
-                         dest="caseid",
-                         default='',
-                         help="Case ID which need to run in Excel config. Do no use this option for running all cases. Only support 1 case")
+                         help="only for -loop mode usage, Number of case which need to run in Excel config. Do no use this option for running all cases. Input number > 0")
         parser.addoption("--bdd_flag",
                          dest="bdd_flag",
                          default='N',
                          help="Determine if the run is in BDD: Y or N")
         parser.addoption("--breakable",
                          dest="breakable",
                          default='Y',
                          help="Determine when failure happen, the flow will break or not: Y or N")
         parser.addoption("--wdm",
                          dest="wdm",
                          default='N',
                          help="Determine user want to use Web driver Manager or not: Y or N")
-        # parser.addoption("--bdd_flag",
-        #                  dest="bdd_flag",
-        #                  default="N",
-        #                  help="Determine if the run is in BDD: Y or N")
+
     except Exception as e:
         print("Exception when trying to run test: %s" % __file__)
         print("Python says:%s" % str(e))
 
 
 # def addoption_base(parser):
 # "Method to add the option to ini."
```

### Comparing `python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/drivers/browsers/browser_os_name_conf.py` & `python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/drivers/browsers/browser_os_name_conf.py`

 * *Files identical despite different names*

### Comparing `python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/drivers/browsers/local_browsers.py` & `python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/drivers/browsers/local_browsers.py`

 * *Files identical despite different names*

### Comparing `python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/drivers/browsers/remote_options.py` & `python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/drivers/browsers/remote_options.py`

 * *Files identical despite different names*

### Comparing `python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/drivers/driverfactory.py` & `python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/drivers/driverfactory.py`

 * *Files identical despite different names*

### Comparing `python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/main.py` & `python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/main.py`

 * *Files identical despite different names*

### Comparing `python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/pages/Base_Page.py` & `python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/pages/Base_Page.py`

 * *Files identical despite different names*

### Comparing `python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/pages/Mobile_Base_Page.py` & `python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/pages/Mobile_Base_Page.py`

 * *Files identical despite different names*

### Comparing `python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/remoteTest/BrowserStack_Library.py` & `python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/remoteTest/BrowserStack_Library.py`

 * *Files identical despite different names*

### Comparing `python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/utils/email_conf.py` & `python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/utils/email_conf.py`

 * *Files identical despite different names*

### Comparing `python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/utils/general/Base_Logging.py` & `python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/utils/general/Base_Logging.py`

 * *Files identical despite different names*

### Comparing `python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/utils/general/Gif_Maker.py` & `python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/utils/general/Gif_Maker.py`

 * *Files identical despite different names*

### Comparing `python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/utils/general/Wrapit.py` & `python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/utils/general/Wrapit.py`

 * *Files identical despite different names*

### Comparing `python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package/utils/general/email_pytest_report.py` & `python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package/utils/general/email_pytest_report.py`

 * *Files identical despite different names*

### Comparing `python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package.egg-info/PKG-INFO` & `python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-selenium-ctrl-package
-Version: 0.0.98
+Version: 0.0.99
 Summary: Base_page for selenium automation
 Author-email: "QHMS(App team)" <qhmsqaexpert@gmail.com>
 Keywords: python,automation,appium,selenium,pytest,automation framework
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `python_selenium_ctrl_package-0.0.98/src/python_selenium_ctrl_package.egg-info/SOURCES.txt` & `python_selenium_ctrl_package-0.0.99/src/python_selenium_ctrl_package.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 src/__init__.py
 src/python_selenium_ctrl_package/__init__.py
 src/python_selenium_ctrl_package/conftest_base.py
 src/python_selenium_ctrl_package/main.py
 src/python_selenium_ctrl_package.egg-info/PKG-INFO
 src/python_selenium_ctrl_package.egg-info/SOURCES.txt
 src/python_selenium_ctrl_package.egg-info/dependency_links.txt
-src/python_selenium_ctrl_package.egg-info/requires.txt
 src/python_selenium_ctrl_package.egg-info/top_level.txt
 src/python_selenium_ctrl_package/conf/__init__.py
 src/python_selenium_ctrl_package/conf/product_list.py
 src/python_selenium_ctrl_package/conf/app/__init__.py
 src/python_selenium_ctrl_package/conf/app/ports_conf.py
 src/python_selenium_ctrl_package/conf/rwd/__init__.py
 src/python_selenium_ctrl_package/conf/rwd/Website/__init__.py
```

