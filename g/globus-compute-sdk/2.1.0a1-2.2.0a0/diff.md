# Comparing `tmp/globus-compute-sdk-2.1.0a1.tar.gz` & `tmp/globus-compute-sdk-2.2.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globus-compute-sdk-2.1.0a1.tar", last modified: Tue May 23 18:47:03 2023, max compression
+gzip compressed data, was "globus-compute-sdk-2.2.0a0.tar", last modified: Tue Jun 20 18:07:02 2023, max compression
```

## Comparing `globus-compute-sdk-2.1.0a1.tar` & `globus-compute-sdk-2.2.0a0.tar`

### file list

```diff
@@ -1,55 +1,51 @@
-drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:03.947557 globus-compute-sdk-2.1.0a1/
--rw-rw-r--   0 reid      (1000) reid      (1000)    11330 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/LICENSE
--rw-rw-r--   0 reid      (1000) reid      (1000)       16 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/MANIFEST.in
--rw-rw-r--   0 reid      (1000) reid      (1000)     1821 2023-05-23 18:47:03.951557 globus-compute-sdk-2.1.0a1/PKG-INFO
--rw-rw-r--   0 reid      (1000) reid      (1000)      816 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/PyPI.md
-drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:03.943557 globus-compute-sdk-2.1.0a1/globus_compute_sdk/
--rw-rw-r--   0 reid      (1000) reid      (1000)      433 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/__init__.py
-drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:03.943557 globus-compute-sdk-2.1.0a1/globus_compute_sdk/errors/
--rw-rw-r--   0 reid      (1000) reid      (1000)      320 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/errors/__init__.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     1921 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/errors/error_types.py
-drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:03.947557 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/
--rw-rw-r--   0 reid      (1000) reid      (1000)        0 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/__init__.py
--rw-rw-r--   0 reid      (1000) reid      (1000)      986 2023-05-01 20:50:52.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/_environments.py
-drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:03.947557 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/asynchronous/
--rw-rw-r--   0 reid      (1000) reid      (1000)        0 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/asynchronous/__init__.py
--rw-rw-r--   0 reid      (1000) reid      (1000)      648 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/asynchronous/compute_future.py
--rw-rw-r--   0 reid      (1000) reid      (1000)      724 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/asynchronous/compute_task.py
--rw-rw-r--   0 reid      (1000) reid      (1000)    11458 2023-05-01 20:50:52.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/asynchronous/ws_polling_task.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     2262 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/batch.py
--rw-rw-r--   0 reid      (1000) reid      (1000)    26362 2023-05-17 18:35:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/client.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     2400 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/container_spec.py
--rw-rw-r--   0 reid      (1000) reid      (1000)    46344 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/executor.py
-drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:03.947557 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/login_manager/
--rw-rw-r--   0 reid      (1000) reid      (1000)      237 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/login_manager/__init__.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     1787 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/login_manager/client_login.py
--rw-rw-r--   0 reid      (1000) reid      (1000)      855 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/login_manager/decorators.py
--rw-rw-r--   0 reid      (1000) reid      (1000)      373 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/login_manager/globus_auth.py
--rw-rw-r--   0 reid      (1000) reid      (1000)      954 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/login_manager/login_flow.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     7287 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/login_manager/manager.py
--rw-rw-r--   0 reid      (1000) reid      (1000)      710 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/login_manager/protocol.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     3012 2023-05-04 22:24:51.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/login_manager/tokenstore.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     2190 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/login_manager/whoami.py
-drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:03.947557 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/utils/
--rw-rw-r--   0 reid      (1000) reid      (1000)      212 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/utils/__init__.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     1207 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/utils/printing.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     8618 2023-05-17 18:37:21.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/web_client.py
-drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:03.947557 globus-compute-sdk-2.1.0a1/globus_compute_sdk/serialize/
--rw-rw-r--   0 reid      (1000) reid      (1000)      100 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/serialize/__init__.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     1372 2023-05-11 19:15:28.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/serialize/base.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     7513 2023-05-11 19:15:28.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/serialize/concretes.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     3737 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/serialize/facade.py
--rw-rw-r--   0 reid      (1000) reid      (1000)        0 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/utils.py
--rw-rw-r--   0 reid      (1000) reid      (1000)      834 2023-05-23 18:46:25.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk/version.py
-drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:03.943557 globus-compute-sdk-2.1.0a1/globus_compute_sdk.egg-info/
--rw-rw-r--   0 reid      (1000) reid      (1000)     1821 2023-05-23 18:47:03.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 reid      (1000) reid      (1000)     1628 2023-05-23 18:47:03.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 reid      (1000) reid      (1000)        1 2023-05-23 18:47:03.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 reid      (1000) reid      (1000)      397 2023-05-23 18:47:03.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk.egg-info/requires.txt
--rw-rw-r--   0 reid      (1000) reid      (1000)       19 2023-05-23 18:47:03.000000 globus-compute-sdk-2.1.0a1/globus_compute_sdk.egg-info/top_level.txt
--rw-rw-r--   0 reid      (1000) reid      (1000)      282 2023-05-23 18:47:03.951557 globus-compute-sdk-2.1.0a1/setup.cfg
--rw-rw-r--   0 reid      (1000) reid      (1000)     3161 2023-05-11 19:15:28.000000 globus-compute-sdk-2.1.0a1/setup.py
-drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:03.947557 globus-compute-sdk-2.1.0a1/tests/
--rw-rw-r--   0 reid      (1000) reid      (1000)        0 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/tests/__init__.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     1962 2023-05-01 20:50:52.000000 globus-compute-sdk-2.1.0a1/tests/conftest.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     2276 2023-04-19 22:57:38.000000 globus-compute-sdk-2.1.0a1/tests/utils.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-20 18:07:02.019847 globus-compute-sdk-2.2.0a0/
+-rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.0a0/LICENSE
+-rw-r--r--   0 lei        (501) staff       (20)       16 2023-04-20 03:21:56.000000 globus-compute-sdk-2.2.0a0/MANIFEST.in
+-rw-r--r--   0 lei        (501) staff       (20)     1821 2023-06-20 18:07:02.019906 globus-compute-sdk-2.2.0a0/PKG-INFO
+-rw-r--r--   0 lei        (501) staff       (20)      816 2023-04-20 03:21:56.000000 globus-compute-sdk-2.2.0a0/PyPI.md
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-20 18:07:02.013925 globus-compute-sdk-2.2.0a0/globus_compute_sdk/
+-rw-r--r--   0 lei        (501) staff       (20)      433 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.0a0/globus_compute_sdk/__init__.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-20 18:07:02.014749 globus-compute-sdk-2.2.0a0/globus_compute_sdk/errors/
+-rw-r--r--   0 lei        (501) staff       (20)      320 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.0a0/globus_compute_sdk/errors/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     1921 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.0a0/globus_compute_sdk/errors/error_types.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-20 18:07:02.016431 globus-compute-sdk-2.2.0a0/globus_compute_sdk/sdk/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.0a0/globus_compute_sdk/sdk/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     1276 2023-06-20 17:53:41.000000 globus-compute-sdk-2.2.0a0/globus_compute_sdk/sdk/_environments.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-20 18:07:02.016921 globus-compute-sdk-2.2.0a0/globus_compute_sdk/sdk/asynchronous/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.0a0/globus_compute_sdk/sdk/asynchronous/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)      648 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.0a0/globus_compute_sdk/sdk/asynchronous/compute_future.py
+-rw-r--r--   0 lei        (501) staff       (20)      724 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.0a0/globus_compute_sdk/sdk/asynchronous/compute_task.py
+-rw-r--r--   0 lei        (501) staff       (20)    11458 2023-04-24 21:22:25.000000 globus-compute-sdk-2.2.0a0/globus_compute_sdk/sdk/asynchronous/ws_polling_task.py
+-rw-r--r--   0 lei        (501) staff       (20)     2262 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.0a0/globus_compute_sdk/sdk/batch.py
+-rw-r--r--   0 lei        (501) staff       (20)    27030 2023-06-13 20:34:26.000000 globus-compute-sdk-2.2.0a0/globus_compute_sdk/sdk/client.py
+-rw-r--r--   0 lei        (501) staff       (20)     2400 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.0a0/globus_compute_sdk/sdk/container_spec.py
+-rw-r--r--   0 lei        (501) staff       (20)    46344 2023-06-05 19:33:47.000000 globus-compute-sdk-2.2.0a0/globus_compute_sdk/sdk/executor.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-20 18:07:02.018596 globus-compute-sdk-2.2.0a0/globus_compute_sdk/sdk/login_manager/
+-rw-r--r--   0 lei        (501) staff       (20)      237 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.0a0/globus_compute_sdk/sdk/login_manager/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     1787 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.0a0/globus_compute_sdk/sdk/login_manager/client_login.py
+-rw-r--r--   0 lei        (501) staff       (20)      855 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.0a0/globus_compute_sdk/sdk/login_manager/decorators.py
+-rw-r--r--   0 lei        (501) staff       (20)      373 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.0a0/globus_compute_sdk/sdk/login_manager/globus_auth.py
+-rw-r--r--   0 lei        (501) staff       (20)      954 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.0a0/globus_compute_sdk/sdk/login_manager/login_flow.py
+-rw-r--r--   0 lei        (501) staff       (20)     7287 2023-06-12 17:16:14.000000 globus-compute-sdk-2.2.0a0/globus_compute_sdk/sdk/login_manager/manager.py
+-rw-r--r--   0 lei        (501) staff       (20)      710 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.0a0/globus_compute_sdk/sdk/login_manager/protocol.py
+-rw-r--r--   0 lei        (501) staff       (20)     3012 2023-05-05 16:40:44.000000 globus-compute-sdk-2.2.0a0/globus_compute_sdk/sdk/login_manager/tokenstore.py
+-rw-r--r--   0 lei        (501) staff       (20)     2190 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.0a0/globus_compute_sdk/sdk/login_manager/whoami.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-20 18:07:02.018873 globus-compute-sdk-2.2.0a0/globus_compute_sdk/sdk/utils/
+-rw-r--r--   0 lei        (501) staff       (20)      212 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.0a0/globus_compute_sdk/sdk/utils/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     1207 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.0a0/globus_compute_sdk/sdk/utils/printing.py
+-rw-r--r--   0 lei        (501) staff       (20)     8443 2023-06-13 20:34:26.000000 globus-compute-sdk-2.2.0a0/globus_compute_sdk/sdk/web_client.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-20 18:07:02.019622 globus-compute-sdk-2.2.0a0/globus_compute_sdk/serialize/
+-rw-r--r--   0 lei        (501) staff       (20)      603 2023-06-13 18:28:48.000000 globus-compute-sdk-2.2.0a0/globus_compute_sdk/serialize/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     1412 2023-06-20 16:40:24.000000 globus-compute-sdk-2.2.0a0/globus_compute_sdk/serialize/base.py
+-rw-r--r--   0 lei        (501) staff       (20)     7869 2023-06-13 18:28:48.000000 globus-compute-sdk-2.2.0a0/globus_compute_sdk/serialize/concretes.py
+-rw-r--r--   0 lei        (501) staff       (20)     4848 2023-06-20 16:40:24.000000 globus-compute-sdk-2.2.0a0/globus_compute_sdk/serialize/facade.py
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-05-08 21:56:13.000000 globus-compute-sdk-2.2.0a0/globus_compute_sdk/utils.py
+-rw-r--r--   0 lei        (501) staff       (20)      834 2023-06-20 17:58:14.000000 globus-compute-sdk-2.2.0a0/globus_compute_sdk/version.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-20 18:07:02.014479 globus-compute-sdk-2.2.0a0/globus_compute_sdk.egg-info/
+-rw-r--r--   0 lei        (501) staff       (20)     1821 2023-06-20 18:07:02.000000 globus-compute-sdk-2.2.0a0/globus_compute_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 lei        (501) staff       (20)     1577 2023-06-20 18:07:02.000000 globus-compute-sdk-2.2.0a0/globus_compute_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 lei        (501) staff       (20)        1 2023-06-20 18:07:02.000000 globus-compute-sdk-2.2.0a0/globus_compute_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 lei        (501) staff       (20)      397 2023-06-20 18:07:02.000000 globus-compute-sdk-2.2.0a0/globus_compute_sdk.egg-info/requires.txt
+-rw-r--r--   0 lei        (501) staff       (20)       19 2023-06-20 18:07:02.000000 globus-compute-sdk-2.2.0a0/globus_compute_sdk.egg-info/top_level.txt
+-rw-r--r--   0 lei        (501) staff       (20)      282 2023-06-20 18:07:02.020136 globus-compute-sdk-2.2.0a0/setup.cfg
+-rw-r--r--   0 lei        (501) staff       (20)     3161 2023-06-20 17:53:41.000000 globus-compute-sdk-2.2.0a0/setup.py
```

### Comparing `globus-compute-sdk-2.1.0a1/LICENSE` & `globus-compute-sdk-2.2.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.1.0a1/PKG-INFO` & `globus-compute-sdk-2.2.0a0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-sdk
-Version: 2.1.0a1
+Version: 2.2.0a0
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `globus-compute-sdk-2.1.0a1/PyPI.md` & `globus-compute-sdk-2.2.0a0/PyPI.md`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.1.0a1/globus_compute_sdk/errors/error_types.py` & `globus-compute-sdk-2.2.0a0/globus_compute_sdk/errors/error_types.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/asynchronous/compute_future.py` & `globus-compute-sdk-2.2.0a0/globus_compute_sdk/sdk/asynchronous/compute_future.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/asynchronous/compute_task.py` & `globus-compute-sdk-2.2.0a0/globus_compute_sdk/sdk/asynchronous/compute_task.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/asynchronous/ws_polling_task.py` & `globus-compute-sdk-2.2.0a0/globus_compute_sdk/sdk/asynchronous/ws_polling_task.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/batch.py` & `globus-compute-sdk-2.2.0a0/globus_compute_sdk/sdk/batch.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/client.py` & `globus-compute-sdk-2.2.0a0/globus_compute_sdk/sdk/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     get_web_service_url,
     get_web_socket_url,
     urls_might_mismatch,
 )
 from globus_compute_sdk.sdk.asynchronous.compute_task import ComputeTask
 from globus_compute_sdk.sdk.asynchronous.ws_polling_task import WebSocketPollingTask
 from globus_compute_sdk.sdk.web_client import FunctionRegistrationData
-from globus_compute_sdk.serialize import ComputeSerializer
+from globus_compute_sdk.serialize import ComputeSerializer, SerializationStrategy
 from globus_compute_sdk.version import __version__, compare_versions
 
 from .batch import Batch
 from .login_manager import LoginManager, LoginManagerProtocol, requires_login
 
 logger = logging.getLogger(__name__)
 
@@ -58,14 +58,16 @@
         warn_about_url_mismatch: bool | None = None,
         task_group_id: t.Union[None, uuid.UUID, str] = None,
         do_version_check: bool = True,
         openid_authorizer: t.Any = None,
         search_authorizer: t.Any = None,
         fx_authorizer: t.Any = None,
         *,
+        code_serialization_strategy: SerializationStrategy | None = None,
+        data_serialization_strategy: SerializationStrategy | None = None,
         login_manager: LoginManagerProtocol | None = None,
         **kwargs,
     ):
         """
         Initialize the client
 
         Parameters
@@ -117,14 +119,22 @@
 
         task_group_id: str|uuid.UUID
             Set the TaskGroup ID (a UUID) for this Client instance.
             Typically, one uses this to submit new tasks to an existing
             session or to reestablish Executor futures.
             Default: None (will be auto generated)
 
+        code_serialization_strategy: SerializationStrategy
+            Strategy to use when serializing function code. If None,
+            globus_compute_sdk.serialize.DEFAULT_STRATEGY_CODE will be used.
+
+        data_serialization_strategy: SerializationStrategy
+            Strategy to use when serializing function arguments. If None,
+            globus_compute_sdk.serialize.DEFAULT_STRATEGY_DATA will be used.
+
         Keyword arguments are the same as for BaseClient.
 
         """
         # resolve URLs if not set
         if funcx_service_address is None:
             funcx_service_address = get_web_service_url(environment)
 
@@ -158,15 +168,18 @@
         else:
             self.login_manager = LoginManager(environment=environment)
             self.login_manager.ensure_logged_in()
 
         self.web_client = self.login_manager.get_web_client(
             base_url=funcx_service_address
         )
-        self.fx_serializer = ComputeSerializer()
+        self.fx_serializer = ComputeSerializer(
+            strategy_code=code_serialization_strategy,
+            strategy_data=data_serialization_strategy,
+        )
 
         self.funcx_service_address = funcx_service_address
 
         if do_version_check:
             self.version_check()
 
         self.results_ws_uri = None
@@ -637,15 +650,14 @@
                 "The 'searchable' argument is deprecated and no longer functional. "
                 "It will be removed in a future release."
             )
 
         data = FunctionRegistrationData(
             function=function,
             container_uuid=container_uuid,
-            entry_point=function_name,
             description=description,
             public=public,
             group=group,
             serializer=self.fx_serializer,
         )
         logger.info(f"Registering function : {data}")
         r = self.web_client.register_function(data)
```

### Comparing `globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/container_spec.py` & `globus-compute-sdk-2.2.0a0/globus_compute_sdk/sdk/container_spec.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/executor.py` & `globus-compute-sdk-2.2.0a0/globus_compute_sdk/sdk/executor.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/login_manager/client_login.py` & `globus-compute-sdk-2.2.0a0/globus_compute_sdk/sdk/login_manager/client_login.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/login_manager/decorators.py` & `globus-compute-sdk-2.2.0a0/globus_compute_sdk/sdk/login_manager/decorators.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/login_manager/login_flow.py` & `globus-compute-sdk-2.2.0a0/globus_compute_sdk/sdk/login_manager/login_flow.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/login_manager/manager.py` & `globus-compute-sdk-2.2.0a0/globus_compute_sdk/sdk/login_manager/manager.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/login_manager/protocol.py` & `globus-compute-sdk-2.2.0a0/globus_compute_sdk/sdk/login_manager/protocol.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/login_manager/tokenstore.py` & `globus-compute-sdk-2.2.0a0/globus_compute_sdk/sdk/login_manager/tokenstore.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/login_manager/whoami.py` & `globus-compute-sdk-2.2.0a0/globus_compute_sdk/sdk/login_manager/whoami.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/utils/printing.py` & `globus-compute-sdk-2.2.0a0/globus_compute_sdk/sdk/utils/printing.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.1.0a1/globus_compute_sdk/sdk/web_client.py` & `globus-compute-sdk-2.2.0a0/globus_compute_sdk/sdk/web_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     def __init__(
         self,
         *,
         function: t.Optional[t.Callable] = None,
         function_name: t.Optional[str] = None,
         function_code: t.Optional[str] = None,
         container_uuid: t.Optional[ID_PARAM_T] = None,
-        entry_point: t.Optional[str] = None,
         description: t.Optional[str] = None,
         public: bool = False,
         group: t.Optional[str] = None,
         serializer: t.Optional[ComputeSerializer] = None,
     ):
         if function is not None:
             function_name = function.__name__
@@ -51,25 +50,23 @@
             )
 
         self.function_name = function_name
         self.function_code = function_code
         self.container_uuid = (
             str(container_uuid) if container_uuid is not None else container_uuid
         )
-        self.entry_point = entry_point if entry_point is not None else function_name
         self.description = description
         self.public = public
         self.group = group
 
     def to_dict(self):
         return {
             "function_name": self.function_name,
             "function_code": self.function_code,
             "container_uuid": self.container_uuid,
-            "entry_point": self.entry_point,
             "description": self.description,
             "public": self.public,
             "group": self.group,
         }
 
     def __str__(self):
         return "FunctionRegistrationData(" + json.dumps(self.to_dict()) + ")"
```

### Comparing `globus-compute-sdk-2.1.0a1/globus_compute_sdk/serialize/base.py` & `globus-compute-sdk-2.2.0a0/globus_compute_sdk/serialize/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from abc import ABCMeta, abstractmethod
 
 
-class SerializeBase(metaclass=ABCMeta):
-    """Shared functionality for all serializer implementations"""
+class SerializationStrategy(metaclass=ABCMeta):
+    """A SerializationStrategy is in charge of converting function source code or
+    arguments into string data and back again.
+    """
 
     @property
     @abstractmethod
     def identifier(self):
         pass
 
     def chomp(self, payload: str) -> str:
@@ -29,23 +31,21 @@
         raise NotImplementedError("Concrete class did not implement serialize")
 
     @abstractmethod
     def deserialize(self, payload):
         raise NotImplementedError("Concrete class did not implement deserialize")
 
 
-class SerializerError:
+class SerializationError(Exception):
     def __init__(self, reason):
         self.reason = reason
 
     def __repr__(self):
         return f"Serialization failed due to {self.reason}"
 
 
 class DeserializationError(Exception):
-    """Base class for all deserialization errors"""
-
     def __init__(self, reason):
         self.reason = reason
 
     def __repr__(self):
         return f"Deserialization failed due to {self.reason}"
```

### Comparing `globus-compute-sdk-2.1.0a1/globus_compute_sdk/version.py` & `globus-compute-sdk-2.2.0a0/globus_compute_sdk/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from globus_compute_sdk.errors import VersionMismatch
 from packaging.version import Version
 
 # single source of truth for package version,
 # see https://packaging.python.org/en/latest/single_source_version/
-__version__ = "2.1.0a1"
+__version__ = "2.2.0a0"
 
 
 def compare_versions(
     current: str, min_version: str, *, package_name: str = "globus-compute-sdk"
 ) -> None:
     current_v = Version(current)
     min_v = Version(min_version)
```

### Comparing `globus-compute-sdk-2.1.0a1/globus_compute_sdk.egg-info/PKG-INFO` & `globus-compute-sdk-2.2.0a0/globus_compute_sdk.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-sdk
-Version: 2.1.0a1
+Version: 2.2.0a0
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `globus-compute-sdk-2.1.0a1/globus_compute_sdk.egg-info/SOURCES.txt` & `globus-compute-sdk-2.2.0a0/globus_compute_sdk.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -34,11 +34,8 @@
 globus_compute_sdk/sdk/login_manager/tokenstore.py
 globus_compute_sdk/sdk/login_manager/whoami.py
 globus_compute_sdk/sdk/utils/__init__.py
 globus_compute_sdk/sdk/utils/printing.py
 globus_compute_sdk/serialize/__init__.py
 globus_compute_sdk/serialize/base.py
 globus_compute_sdk/serialize/concretes.py
-globus_compute_sdk/serialize/facade.py
-tests/__init__.py
-tests/conftest.py
-tests/utils.py
+globus_compute_sdk/serialize/facade.py
```

### Comparing `globus-compute-sdk-2.1.0a1/setup.py` & `globus-compute-sdk-2.2.0a0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 from setuptools import find_namespace_packages, setup
 
 REQUIRES = [
     # request sending and authorization tools
     "requests>=2.20.0",
-    "globus-sdk>=3.14.0,<4",
+    "globus-sdk>=3.20.1,<4",
     "globus-compute-common==0.2.0",
     # 'websockets' is used for the client-side websocket listener
     "websockets==10.3",
     # dill is an extension of `pickle` to a wider array of native python types
     # pin to the latest version, as 'dill' is not at 1.0 and does not have a clear
     # versioning and compatibility policy
     "dill==0.3.5.1",
```

