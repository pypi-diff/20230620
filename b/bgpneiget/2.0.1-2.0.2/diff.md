# Comparing `tmp/bgpneiget-2.0.1.tar.gz` & `tmp/bgpneiget-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bgpneiget-2.0.1.tar", max compression
+gzip compressed data, was "bgpneiget-2.0.2.tar", max compression
```

## Comparing `bgpneiget-2.0.1.tar` & `bgpneiget-2.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1322 2023-05-12 08:43:10.928107 bgpneiget-2.0.1/LICENSE
--rw-r--r--   0        0        0      288 2023-05-12 08:43:10.928107 bgpneiget-2.0.1/README.md
--rw-r--r--   0        0        0      753 2023-06-20 09:52:11.289296 bgpneiget-2.0.1/pyproject.toml
--rw-r--r--   0        0        0      272 2023-06-20 09:52:22.449410 bgpneiget-2.0.1/src/bgpneiget/__init__.py
--rw-r--r--   0        0        0     7430 2023-06-20 09:51:03.240596 bgpneiget-2.0.1/src/bgpneiget/cli.py
--rw-r--r--   0        0        0        0 2023-05-12 12:50:58.436841 bgpneiget-2.0.1/src/bgpneiget/device/__init__.py
--rw-r--r--   0        0        0      871 2023-05-17 08:19:38.384271 bgpneiget-2.0.1/src/bgpneiget/device/arista.py
--rw-r--r--   0        0        0     2728 2023-05-18 12:43:21.775962 bgpneiget-2.0.1/src/bgpneiget/device/base.py
--rw-r--r--   0        0        0    10196 2023-06-20 09:47:42.742520 bgpneiget-2.0.1/src/bgpneiget/device/cisco_iosxe.py
--rw-r--r--   0        0        0     5906 2023-06-20 09:47:42.742520 bgpneiget-2.0.1/src/bgpneiget/device/cisco_iosxr.py
--rw-r--r--   0        0        0     1137 2023-06-20 09:47:42.754520 bgpneiget-2.0.1/src/bgpneiget/device/cisco_nxos.py
--rw-r--r--   0        0        0    10892 2023-06-20 09:47:42.754520 bgpneiget-2.0.1/src/bgpneiget/device/juniper.py
--rw-r--r--   0        0        0     1104 2023-05-18 09:46:19.385236 bgpneiget-2.0.1/src/bgpneiget/devices.py
--rw-r--r--   0        0        0     1574 2023-05-22 08:21:44.302857 bgpneiget-2.0.1/src/bgpneiget/runcmds.py
--rw-r--r--   0        0        0      243 2023-05-18 09:45:03.544509 bgpneiget-2.0.1/src/bgpneiget/textfsm/cisco_iosxe_show_bgp.textfsm
--rw-r--r--   0        0        0      529 2023-05-18 12:43:21.775962 bgpneiget-2.0.1/src/bgpneiget/textfsm/cisco_iosxe_show_bgp_vrf.textfsm
--rw-r--r--   0        0        0      510 2023-05-17 15:12:06.559095 bgpneiget-2.0.1/src/bgpneiget/textfsm/cisco_iosxr_show_bgp.textfsm
--rw-r--r--   0        0        0     3506 2023-06-20 09:51:03.240596 bgpneiget-2.0.1/src/bgpneiget/worker.py
--rw-r--r--   0        0        0     1151 1970-01-01 00:00:00.000000 bgpneiget-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1322 2021-11-10 12:20:25.080531 bgpneiget-2.0.2/LICENSE
+-rw-r--r--   0        0        0      288 2021-11-10 12:20:25.084530 bgpneiget-2.0.2/README.md
+-rw-r--r--   0        0        0      753 2023-06-20 13:38:09.278318 bgpneiget-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0      272 2023-06-20 13:38:09.278318 bgpneiget-2.0.2/src/bgpneiget/__init__.py
+-rw-r--r--   0        0        0     7430 2023-06-20 10:12:41.696606 bgpneiget-2.0.2/src/bgpneiget/cli.py
+-rw-r--r--   0        0        0        0 2023-06-12 10:29:27.010290 bgpneiget-2.0.2/src/bgpneiget/device/__init__.py
+-rw-r--r--   0        0        0      871 2023-06-12 10:29:27.014290 bgpneiget-2.0.2/src/bgpneiget/device/arista.py
+-rw-r--r--   0        0        0     2728 2023-06-12 10:29:27.014290 bgpneiget-2.0.2/src/bgpneiget/device/base.py
+-rw-r--r--   0        0        0    10262 2023-06-20 13:29:10.237316 bgpneiget-2.0.2/src/bgpneiget/device/cisco_iosxe.py
+-rw-r--r--   0        0        0     5972 2023-06-20 13:28:45.440902 bgpneiget-2.0.2/src/bgpneiget/device/cisco_iosxr.py
+-rw-r--r--   0        0        0     1137 2023-06-20 10:12:41.696606 bgpneiget-2.0.2/src/bgpneiget/device/cisco_nxos.py
+-rw-r--r--   0        0        0    11159 2023-06-20 13:38:09.278318 bgpneiget-2.0.2/src/bgpneiget/device/juniper.py
+-rw-r--r--   0        0        0     1104 2023-06-12 10:29:27.014290 bgpneiget-2.0.2/src/bgpneiget/devices.py
+-rw-r--r--   0        0        0     1574 2023-06-12 10:29:27.014290 bgpneiget-2.0.2/src/bgpneiget/runcmds.py
+-rw-r--r--   0        0        0      243 2023-06-12 10:29:27.014290 bgpneiget-2.0.2/src/bgpneiget/textfsm/cisco_iosxe_show_bgp.textfsm
+-rw-r--r--   0        0        0      529 2023-06-12 10:29:27.014290 bgpneiget-2.0.2/src/bgpneiget/textfsm/cisco_iosxe_show_bgp_vrf.textfsm
+-rw-r--r--   0        0        0      510 2023-06-12 10:29:27.014290 bgpneiget-2.0.2/src/bgpneiget/textfsm/cisco_iosxr_show_bgp.textfsm
+-rw-r--r--   0        0        0     3506 2023-06-20 10:12:41.712606 bgpneiget-2.0.2/src/bgpneiget/worker.py
+-rw-r--r--   0        0        0     1151 1970-01-01 00:00:00.000000 bgpneiget-2.0.2/PKG-INFO
```

### Comparing `bgpneiget-2.0.1/LICENSE` & `bgpneiget-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bgpneiget-2.0.1/pyproject.toml` & `bgpneiget-2.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bgpneiget"
-version = "2.0.1"
+version = "2.0.2"
 description = "Get BGP Neighbours from network devices"
 authors = ["Rob Woodward <rob@emailplus.org>"]
 
 license = "BSD-2-Clause"
 readme = "README.md"
 repository = "https://github.com/robwdwd/bgpneiget"
 include = ["README.md", "LICENSE"]
```

### Comparing `bgpneiget-2.0.1/src/bgpneiget/cli.py` & `bgpneiget-2.0.2/src/bgpneiget/cli.py`

 * *Files identical despite different names*

### Comparing `bgpneiget-2.0.1/src/bgpneiget/device/arista.py` & `bgpneiget-2.0.2/src/bgpneiget/device/arista.py`

 * *Files identical despite different names*

### Comparing `bgpneiget-2.0.1/src/bgpneiget/device/base.py` & `bgpneiget-2.0.2/src/bgpneiget/device/base.py`

 * *Files identical despite different names*

### Comparing `bgpneiget-2.0.1/src/bgpneiget/device/cisco_iosxe.py` & `bgpneiget-2.0.2/src/bgpneiget/device/cisco_iosxe.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import asyncio
 import ipaddress
 import logging
 import os
 import pprint
 from typing import Type
 
+from asyncssh.misc import Error as AsyncSSHError
 from scrapli.driver.core import AsyncIOSXEDriver
 from scrapli.exceptions import ScrapliException
 from textfsm import TextFSM
 
 from bgpneiget.device.base import BaseDevice
 from bgpneiget.runcmds import get_output
 
@@ -259,15 +260,15 @@
         for table in prog_args["table"]:
             cmd = self.get_bgp_cmd_global(table)
             commands[table] = cmd
             reverse_commands[cmd] = table
 
         try:
             response = await get_output(self, commands, prog_args["username"], prog_args["password"])
-        except ScrapliException as err:
+        except (AsyncSSHError, ScrapliException) as err:
             logger.error("[%s] Can not get neighbours from device: %s", self.hostname, err)
             return result
 
         loop = asyncio.get_running_loop()
 
         for resp in response:
             table = reverse_commands[resp.channel_input]
```

### Comparing `bgpneiget-2.0.1/src/bgpneiget/device/cisco_iosxr.py` & `bgpneiget-2.0.2/src/bgpneiget/device/cisco_iosxr.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import asyncio
 import ipaddress
 import logging
 import os
 import pprint
 from typing import Type
 
+from asyncssh.misc import Error as AsyncSSHError
 from scrapli.driver.core import AsyncIOSXRDriver
 from scrapli.exceptions import ScrapliException
 from textfsm import TextFSM
 
 from bgpneiget.device.base import BaseDevice
 from bgpneiget.runcmds import get_output
 
@@ -160,15 +161,15 @@
         for table in prog_args["table"]:
             cmd = self.get_bgp_cmd_global(table)
             commands[table] = cmd
             reverse_commands[cmd] = table
 
         try:
             response = await get_output(self, commands, prog_args["username"], prog_args["password"])
-        except ScrapliException as err:
+        except (AsyncSSHError, ScrapliException) as err:
             logger.error("[%s] Can not get neighbours from device: %s", self.hostname, err)
             return result
 
         loop = asyncio.get_running_loop()
 
         for resp in response:
             table = reverse_commands[resp.channel_input]
```

### Comparing `bgpneiget-2.0.1/src/bgpneiget/device/cisco_nxos.py` & `bgpneiget-2.0.2/src/bgpneiget/device/cisco_nxos.py`

 * *Files identical despite different names*

### Comparing `bgpneiget-2.0.1/src/bgpneiget/device/juniper.py` & `bgpneiget-2.0.2/src/bgpneiget/device/juniper.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 # "BSD 2-Clause License". Please see the LICENSE file that should
 # have been included as part of this distribution.
 #
 """Juniper device class."""
 import ipaddress
 import logging
 import pprint
+import re
 from typing import Type
 
 import xmltodict
+from asyncssh.misc import Error as AsyncSSHError
 from scrapli.driver.core import AsyncJunosDriver
 from scrapli.exceptions import ScrapliException
 
 from bgpneiget.device.base import BaseDevice
 from bgpneiget.runcmds import get_output
 
 pp = pprint.PrettyPrinter(indent=2, width=120)
@@ -301,16 +303,20 @@
         commands = {}
         result = []
 
         commands["all"] = self.get_bgp_cmd_global()
 
         try:
             response = await get_output(self, commands, prog_args["username"], prog_args["password"])
-        except ScrapliException as err:
+        except (AsyncSSHError, ScrapliException) as err:
             logger.error("[%s] Can not get neighbours from device: %s", self.hostname, err)
             return result
 
         for resp in response:
-            stripped_response = resp.result[: resp.result.rfind("\n")]
-            result = result + await self.process_bgp_neighbours(stripped_response, prog_args)
+            stripped_response = re.search(r"(?sm)\<.*\>", resp.result).group()
+            try:
+                result = result + await self.process_bgp_neighbours(stripped_response, prog_args)
+            except Exception:
+                logger.error("[%s] Unable to parse XML output, maybe no neigbhbours.", self.hostname)
+                return result
 
         return result
```

### Comparing `bgpneiget-2.0.1/src/bgpneiget/devices.py` & `bgpneiget-2.0.2/src/bgpneiget/devices.py`

 * *Files identical despite different names*

### Comparing `bgpneiget-2.0.1/src/bgpneiget/runcmds.py` & `bgpneiget-2.0.2/src/bgpneiget/runcmds.py`

 * *Files identical despite different names*

### Comparing `bgpneiget-2.0.1/src/bgpneiget/textfsm/cisco_iosxe_show_bgp_vrf.textfsm` & `bgpneiget-2.0.2/src/bgpneiget/textfsm/cisco_iosxe_show_bgp_vrf.textfsm`

 * *Files identical despite different names*

### Comparing `bgpneiget-2.0.1/src/bgpneiget/worker.py` & `bgpneiget-2.0.2/src/bgpneiget/worker.py`

 * *Files identical despite different names*

### Comparing `bgpneiget-2.0.1/PKG-INFO` & `bgpneiget-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bgpneiget
-Version: 2.0.1
+Version: 2.0.2
 Summary: Get BGP Neighbours from network devices
 Home-page: https://github.com/robwdwd/bgpneiget
 License: BSD-2-Clause
 Author: Rob Woodward
 Author-email: rob@emailplus.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
```

