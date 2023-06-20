# Comparing `tmp/centralcli-1.5.tar.gz` & `tmp/centralcli-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "centralcli-1.5.tar", max compression
+gzip compressed data, was "centralcli-1.6.tar", max compression
```

## Comparing `centralcli-1.5.tar` & `centralcli-1.6.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0    11929 2022-07-11 23:06:32.918521 centralcli-1.5/README.md
--rw-r--r--   0        0        0     3924 2023-06-16 18:31:40.327908 centralcli-1.5/centralcli/__init__.py
--rw-r--r--   0        0        0     1266 2022-09-23 14:08:18.905345 centralcli-1.5/centralcli/boilerplate/README.md
--rw-r--r--   0        0        0  1080145 2023-06-10 14:09:43.613064 centralcli-1.5/centralcli/boilerplate/allcalls.py
--rw-r--r--   0        0        0   168637 2022-09-23 14:10:56.815345 centralcli-1.5/centralcli/boilerplate/configuration.py
--rw-r--r--   0        0        0    23734 2022-09-23 14:12:10.005345 centralcli-1.5/centralcli/boilerplate/firmware.py
--rw-r--r--   0        0        0    37375 2022-09-23 14:14:48.045345 centralcli-1.5/centralcli/boilerplate/guest.py
--rw-r--r--   0        0        0    55587 2022-09-23 14:18:58.145345 centralcli-1.5/centralcli/boilerplate/wlan.py
--rw-r--r--   0        0        0    12139 2022-06-03 00:05:56.000000 centralcli-1.5/centralcli/caas.py
--rw-r--r--   0        0        0    80066 2023-06-20 18:38:26.384372 centralcli-1.5/centralcli/cache.py
--rw-r--r--   0        0        0   200227 2023-06-16 09:26:09.045820 centralcli-1.5/centralcli/central.py
--rw-r--r--   0        0        0    39789 2023-06-16 17:09:16.160843 centralcli-1.5/centralcli/cleaner.py
--rw-r--r--   0        0        0    40388 2023-06-17 06:14:26.603861 centralcli-1.5/centralcli/cli.py
--rw-r--r--   0        0        0    29703 2023-06-07 16:20:54.400957 centralcli-1.5/centralcli/cliadd.py
--rw-r--r--   0        0        0     4729 2022-07-14 03:34:30.218521 centralcli-1.5/centralcli/cliassign.py
--rw-r--r--   0        0        0    50683 2023-05-04 03:15:53.898642 centralcli-1.5/centralcli/clibatch.py
--rw-r--r--   0        0        0    16403 2022-06-18 06:04:41.177341 centralcli-1.5/centralcli/clicaas.py
--rw-r--r--   0        0        0     2995 2022-01-02 22:57:26.000000 centralcli-1.5/centralcli/cliclone.py
--rw-r--r--   0        0        0    22983 2023-06-16 19:25:19.597950 centralcli-1.5/centralcli/clicommon.py
--rw-r--r--   0        0        0    21359 2023-01-31 22:11:43.015287 centralcli-1.5/centralcli/clidel.py
--rw-r--r--   0        0        0     3251 2022-06-17 04:56:34.221894 centralcli-1.5/centralcli/clirefresh.py
--rw-r--r--   0        0        0     5494 2023-06-17 06:48:47.270573 centralcli-1.5/centralcli/clirename.py
--rw-r--r--   0        0        0   119420 2023-06-17 03:14:51.560590 centralcli-1.5/centralcli/clishow.py
--rw-r--r--   0        0        0     3943 2022-04-14 02:45:35.000000 centralcli-1.5/centralcli/clishowbranch.py
--rw-r--r--   0        0        0     7645 2022-09-23 00:12:29.685345 centralcli-1.5/centralcli/clishowfirmware.py
--rw-r--r--   0        0        0    12980 2023-05-04 02:10:12.446341 centralcli-1.5/centralcli/clishowospf.py
--rw-r--r--   0        0        0    21550 2023-06-15 05:39:44.166523 centralcli-1.5/centralcli/clishowwids.py
--rw-r--r--   0        0        0     8262 2022-07-14 01:24:31.928521 centralcli-1.5/centralcli/clitest.py
--rw-r--r--   0        0        0     6379 2022-09-15 06:49:16.849375 centralcli-1.5/centralcli/clitshoot.py
--rw-r--r--   0        0        0     5245 2022-07-14 00:35:03.158521 centralcli-1.5/centralcli/cliunassign.py
--rw-r--r--   0        0        0    24271 2023-06-17 05:39:24.294216 centralcli-1.5/centralcli/cliupdate.py
--rw-r--r--   0        0        0     9386 2023-06-15 11:32:13.159987 centralcli-1.5/centralcli/cliupgrade.py
--rw-r--r--   0        0        0    18349 2023-06-16 18:44:49.430786 centralcli-1.5/centralcli/config.py
--rw-r--r--   0        0        0    37127 2023-06-17 06:48:14.911291 centralcli-1.5/centralcli/constants.py
--rw-r--r--   0        0        0      160 2022-12-14 19:38:57.975685 centralcli-1.5/centralcli/exceptions.py
--rw-r--r--   0        0        0     6501 2022-02-23 03:21:04.000000 centralcli-1.5/centralcli/logger.py
--rw-r--r--   0        0        0     2298 2023-06-15 05:35:53.155263 centralcli-1.5/centralcli/models.py
--rw-r--r--   0        0        0    16827 2023-06-17 03:57:05.435242 centralcli-1.5/centralcli/render.py
--rw-r--r--   0        0        0    36417 2023-06-16 18:56:01.314032 centralcli-1.5/centralcli/response.py
--rw-r--r--   0        0        0       96 2021-10-13 20:41:19.000000 centralcli-1.5/centralcli/setup.py
--rw-r--r--   0        0        0     1150 2022-02-10 22:18:16.000000 centralcli-1.5/centralcli/static/favicon.ico
--rw-r--r--   0        0        0     9269 2023-06-17 03:27:31.140143 centralcli-1.5/centralcli/strings.py
--rw-r--r--   0        0        0    31046 2022-10-06 02:15:00.061699 centralcli-1.5/centralcli/utils.py
--rw-r--r--   0        0        0     5407 2022-04-29 01:09:46.000000 centralcli-1.5/centralcli/vscodeargs.py
--rw-r--r--   0        0        0    15567 2022-12-28 03:21:15.553278 centralcli-1.5/centralcli/wh_proxy.py
--rw-r--r--   0        0        0      393 2022-01-14 00:45:59.000000 centralcli-1.5/centralcli/wh_proxy_service.py
--rw-r--r--   0        0        0     2032 2023-06-20 18:38:49.314372 centralcli-1.5/pyproject.toml
--rw-r--r--   0        0        0    13933 1970-01-01 00:00:00.000000 centralcli-1.5/PKG-INFO
+-rw-r--r--   0        0        0    11929 2022-07-11 23:06:32.918521 centralcli-1.6/README.md
+-rw-r--r--   0        0        0     3924 2023-06-16 18:31:40.327908 centralcli-1.6/centralcli/__init__.py
+-rw-r--r--   0        0        0     1266 2022-09-23 14:08:18.905345 centralcli-1.6/centralcli/boilerplate/README.md
+-rw-r--r--   0        0        0  1080145 2023-06-10 14:09:43.613064 centralcli-1.6/centralcli/boilerplate/allcalls.py
+-rw-r--r--   0        0        0   168637 2022-09-23 14:10:56.815345 centralcli-1.6/centralcli/boilerplate/configuration.py
+-rw-r--r--   0        0        0    23734 2022-09-23 14:12:10.005345 centralcli-1.6/centralcli/boilerplate/firmware.py
+-rw-r--r--   0        0        0    37375 2022-09-23 14:14:48.045345 centralcli-1.6/centralcli/boilerplate/guest.py
+-rw-r--r--   0        0        0    55587 2022-09-23 14:18:58.145345 centralcli-1.6/centralcli/boilerplate/wlan.py
+-rw-r--r--   0        0        0    12139 2022-06-03 00:05:56.000000 centralcli-1.6/centralcli/caas.py
+-rw-r--r--   0        0        0    80066 2023-06-20 18:38:26.384372 centralcli-1.6/centralcli/cache.py
+-rw-r--r--   0        0        0   200227 2023-06-16 09:26:09.045820 centralcli-1.6/centralcli/central.py
+-rw-r--r--   0        0        0    39789 2023-06-16 17:09:16.160843 centralcli-1.6/centralcli/cleaner.py
+-rw-r--r--   0        0        0    40388 2023-06-17 06:14:26.603861 centralcli-1.6/centralcli/cli.py
+-rw-r--r--   0        0        0    29703 2023-06-07 16:20:54.400957 centralcli-1.6/centralcli/cliadd.py
+-rw-r--r--   0        0        0     4729 2022-07-14 03:34:30.218521 centralcli-1.6/centralcli/cliassign.py
+-rw-r--r--   0        0        0    50683 2023-05-04 03:15:53.898642 centralcli-1.6/centralcli/clibatch.py
+-rw-r--r--   0        0        0    16403 2022-06-18 06:04:41.177341 centralcli-1.6/centralcli/clicaas.py
+-rw-r--r--   0        0        0     2995 2022-01-02 22:57:26.000000 centralcli-1.6/centralcli/cliclone.py
+-rw-r--r--   0        0        0    22958 2023-06-20 18:39:50.084373 centralcli-1.6/centralcli/clicommon.py
+-rw-r--r--   0        0        0    21359 2023-01-31 22:11:43.015287 centralcli-1.6/centralcli/clidel.py
+-rw-r--r--   0        0        0     3251 2022-06-17 04:56:34.221894 centralcli-1.6/centralcli/clirefresh.py
+-rw-r--r--   0        0        0     5494 2023-06-17 06:48:47.270573 centralcli-1.6/centralcli/clirename.py
+-rw-r--r--   0        0        0   119420 2023-06-17 03:14:51.560590 centralcli-1.6/centralcli/clishow.py
+-rw-r--r--   0        0        0     3943 2022-04-14 02:45:35.000000 centralcli-1.6/centralcli/clishowbranch.py
+-rw-r--r--   0        0        0     7645 2022-09-23 00:12:29.685345 centralcli-1.6/centralcli/clishowfirmware.py
+-rw-r--r--   0        0        0    12980 2023-05-04 02:10:12.446341 centralcli-1.6/centralcli/clishowospf.py
+-rw-r--r--   0        0        0    21550 2023-06-15 05:39:44.166523 centralcli-1.6/centralcli/clishowwids.py
+-rw-r--r--   0        0        0     8262 2022-07-14 01:24:31.928521 centralcli-1.6/centralcli/clitest.py
+-rw-r--r--   0        0        0     6379 2022-09-15 06:49:16.849375 centralcli-1.6/centralcli/clitshoot.py
+-rw-r--r--   0        0        0     5245 2022-07-14 00:35:03.158521 centralcli-1.6/centralcli/cliunassign.py
+-rw-r--r--   0        0        0    24271 2023-06-17 05:39:24.294216 centralcli-1.6/centralcli/cliupdate.py
+-rw-r--r--   0        0        0     9386 2023-06-15 11:32:13.159987 centralcli-1.6/centralcli/cliupgrade.py
+-rw-r--r--   0        0        0    18349 2023-06-16 18:44:49.430786 centralcli-1.6/centralcli/config.py
+-rw-r--r--   0        0        0    37127 2023-06-17 06:48:14.911291 centralcli-1.6/centralcli/constants.py
+-rw-r--r--   0        0        0      160 2022-12-14 19:38:57.975685 centralcli-1.6/centralcli/exceptions.py
+-rw-r--r--   0        0        0     6501 2022-02-23 03:21:04.000000 centralcli-1.6/centralcli/logger.py
+-rw-r--r--   0        0        0     2298 2023-06-15 05:35:53.155263 centralcli-1.6/centralcli/models.py
+-rw-r--r--   0        0        0    16827 2023-06-17 03:57:05.435242 centralcli-1.6/centralcli/render.py
+-rw-r--r--   0        0        0    36417 2023-06-16 18:56:01.314032 centralcli-1.6/centralcli/response.py
+-rw-r--r--   0        0        0       96 2021-10-13 20:41:19.000000 centralcli-1.6/centralcli/setup.py
+-rw-r--r--   0        0        0     1150 2022-02-10 22:18:16.000000 centralcli-1.6/centralcli/static/favicon.ico
+-rw-r--r--   0        0        0     9269 2023-06-17 03:27:31.140143 centralcli-1.6/centralcli/strings.py
+-rw-r--r--   0        0        0    31046 2022-10-06 02:15:00.061699 centralcli-1.6/centralcli/utils.py
+-rw-r--r--   0        0        0     5407 2022-04-29 01:09:46.000000 centralcli-1.6/centralcli/vscodeargs.py
+-rw-r--r--   0        0        0    15567 2022-12-28 03:21:15.553278 centralcli-1.6/centralcli/wh_proxy.py
+-rw-r--r--   0        0        0      393 2022-01-14 00:45:59.000000 centralcli-1.6/centralcli/wh_proxy_service.py
+-rw-r--r--   0        0        0     2032 2023-06-20 18:39:57.144379 centralcli-1.6/pyproject.toml
+-rw-r--r--   0        0        0    13933 1970-01-01 00:00:00.000000 centralcli-1.6/PKG-INFO
```

### Comparing `centralcli-1.5/README.md` & `centralcli-1.6/README.md`

 * *Files identical despite different names*

### Comparing `centralcli-1.5/centralcli/__init__.py` & `centralcli-1.6/centralcli/__init__.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.5/centralcli/boilerplate/README.md` & `centralcli-1.6/centralcli/boilerplate/README.md`

 * *Files identical despite different names*

### Comparing `centralcli-1.5/centralcli/boilerplate/allcalls.py` & `centralcli-1.6/centralcli/boilerplate/allcalls.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.5/centralcli/boilerplate/configuration.py` & `centralcli-1.6/centralcli/boilerplate/configuration.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.5/centralcli/boilerplate/firmware.py` & `centralcli-1.6/centralcli/boilerplate/firmware.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.5/centralcli/boilerplate/guest.py` & `centralcli-1.6/centralcli/boilerplate/guest.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.5/centralcli/boilerplate/wlan.py` & `centralcli-1.6/centralcli/boilerplate/wlan.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.5/centralcli/caas.py` & `centralcli-1.6/centralcli/caas.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.5/centralcli/cache.py` & `centralcli-1.6/centralcli/cache.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.5/centralcli/central.py` & `centralcli-1.6/centralcli/central.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.5/centralcli/cleaner.py` & `centralcli-1.6/centralcli/cleaner.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.5/centralcli/cli.py` & `centralcli-1.6/centralcli/cli.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.5/centralcli/cliadd.py` & `centralcli-1.6/centralcli/cliadd.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.5/centralcli/cliassign.py` & `centralcli-1.6/centralcli/cliassign.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.5/centralcli/clibatch.py` & `centralcli-1.6/centralcli/clibatch.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.5/centralcli/clicaas.py` & `centralcli-1.6/centralcli/clicaas.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.5/centralcli/cliclone.py` & `centralcli-1.6/centralcli/cliclone.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.5/centralcli/clicommon.py` & `centralcli-1.6/centralcli/clicommon.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from typing import Dict, List, Literal, Union, Tuple
 from pathlib import Path
 from rich.console import Console
 from rich import print
 import json
 import pkg_resources
 import os
-from render import rich_capture
 
 
 # Detect if called from pypi installed package or via cloned github repo (development)
 try:
     from centralcli import config, log, utils, Cache, Response, render
 except (ImportError, ModuleNotFoundError) as e:
     pkg_dir = Path(__file__).absolute().parent
@@ -56,15 +55,15 @@
                 return getattr(self, self.msg)
             else:
                 return self.initial if not os.environ.get("ARUBACLI_ACCOUNT") else self.envvar
 
         @property
         def envvar(self):
             envvar_msg = f'Using Account: [cyan]{self.account}[/] [italic]based on env var[/] [dark_green]ARUBACLI_ACCOUNT[/]'
-            return rich_capture(envvar_msg)
+            return render.rich_capture(envvar_msg)
 
         @property
         def initial(self):
             acct_clr = f"{typer.style(self.account, fg='cyan')}"
             return (
                 f"{typer.style(f'Using Account: {acct_clr}.', fg='magenta')}  "
                 f"{typer.style(f'Account setting is sticky.  ', fg='red', blink=True)}"
```

### Comparing `centralcli-1.5/centralcli/clidel.py` & `centralcli-1.6/centralcli/clidel.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.5/centralcli/clirefresh.py` & `centralcli-1.6/centralcli/clirefresh.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.5/centralcli/clirename.py` & `centralcli-1.6/centralcli/clirename.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.5/centralcli/clishow.py` & `centralcli-1.6/centralcli/clishow.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.5/centralcli/clishowbranch.py` & `centralcli-1.6/centralcli/clishowbranch.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.5/centralcli/clishowfirmware.py` & `centralcli-1.6/centralcli/clishowfirmware.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.5/centralcli/clishowospf.py` & `centralcli-1.6/centralcli/clishowospf.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.5/centralcli/clishowwids.py` & `centralcli-1.6/centralcli/clishowwids.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.5/centralcli/clitest.py` & `centralcli-1.6/centralcli/clitest.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.5/centralcli/clitshoot.py` & `centralcli-1.6/centralcli/clitshoot.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.5/centralcli/cliunassign.py` & `centralcli-1.6/centralcli/cliunassign.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.5/centralcli/cliupdate.py` & `centralcli-1.6/centralcli/cliupdate.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.5/centralcli/cliupgrade.py` & `centralcli-1.6/centralcli/cliupgrade.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.5/centralcli/config.py` & `centralcli-1.6/centralcli/config.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.5/centralcli/constants.py` & `centralcli-1.6/centralcli/constants.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.5/centralcli/logger.py` & `centralcli-1.6/centralcli/logger.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.5/centralcli/models.py` & `centralcli-1.6/centralcli/models.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.5/centralcli/render.py` & `centralcli-1.6/centralcli/render.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.5/centralcli/response.py` & `centralcli-1.6/centralcli/response.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.5/centralcli/static/favicon.ico` & `centralcli-1.6/centralcli/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `centralcli-1.5/centralcli/strings.py` & `centralcli-1.6/centralcli/strings.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.5/centralcli/utils.py` & `centralcli-1.6/centralcli/utils.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.5/centralcli/vscodeargs.py` & `centralcli-1.6/centralcli/vscodeargs.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.5/centralcli/wh_proxy.py` & `centralcli-1.6/centralcli/wh_proxy.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.5/pyproject.toml` & `centralcli-1.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "centralcli"
-version = "1.5"
+version = "1.6"
 description = "A CLI for interacting with Aruba Central (Cloud Management Platform).  Facilitates bulk imports, exports, reporting.  A handy tool if you have devices managed by Aruba Central."
 license = "MIT"
 authors = ["Wade Wells (Pack3tL0ss) <wade@consolepi.org>"]
 maintainers = ["Wade Wells (Pack3tL0ss) <wade@consolepi.org>"]
 readme = "README.md"
 repository = "https://github.com/Pack3tL0ss/central-api-cli"
 documentation = "https://central-api-cli.readthedocs.org"
```

### Comparing `centralcli-1.5/PKG-INFO` & `centralcli-1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: centralcli
-Version: 1.5
+Version: 1.6
 Summary: A CLI for interacting with Aruba Central (Cloud Management Platform).  Facilitates bulk imports, exports, reporting.  A handy tool if you have devices managed by Aruba Central.
 Home-page: https://github.com/Pack3tL0ss/central-api-cli
 License: MIT
 Keywords: cli,Aruba,Aruba Networks,Aruba Central,HPE,API,RESTFUL,REST
 Author: Wade Wells (Pack3tL0ss)
 Author-email: wade@consolepi.org
 Maintainer: Wade Wells (Pack3tL0ss)
```

