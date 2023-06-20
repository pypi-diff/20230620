# Comparing `tmp/bgpneiget-2.0.0.tar.gz` & `tmp/bgpneiget-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bgpneiget-2.0.0.tar", max compression
+gzip compressed data, was "bgpneiget-2.0.1.tar", max compression
```

## Comparing `bgpneiget-2.0.0.tar` & `bgpneiget-2.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1322 2023-05-12 08:43:10.928107 bgpneiget-2.0.0/LICENSE
--rw-r--r--   0        0        0      288 2023-05-12 08:43:10.928107 bgpneiget-2.0.0/README.md
--rw-r--r--   0        0        0      753 2023-05-24 09:08:36.528427 bgpneiget-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      272 2023-05-12 14:51:15.927138 bgpneiget-2.0.0/src/bgpneiget/__init__.py
--rw-r--r--   0        0        0     6599 2023-06-12 16:01:39.992571 bgpneiget-2.0.0/src/bgpneiget/cli.py
--rw-r--r--   0        0        0        0 2023-05-12 12:50:58.436841 bgpneiget-2.0.0/src/bgpneiget/device/__init__.py
--rw-r--r--   0        0        0      871 2023-05-17 08:19:38.384271 bgpneiget-2.0.0/src/bgpneiget/device/arista.py
--rw-r--r--   0        0        0     2728 2023-05-18 12:43:21.775962 bgpneiget-2.0.0/src/bgpneiget/device/base.py
--rw-r--r--   0        0        0     9974 2023-05-25 13:39:58.309156 bgpneiget-2.0.0/src/bgpneiget/device/cisco_iosxe.py
--rw-r--r--   0        0        0     5684 2023-05-25 13:40:00.373175 bgpneiget-2.0.0/src/bgpneiget/device/cisco_iosxr.py
--rw-r--r--   0        0        0     1089 2023-05-18 13:31:42.764240 bgpneiget-2.0.0/src/bgpneiget/device/cisco_nxos.py
--rw-r--r--   0        0        0    10670 2023-05-24 11:08:34.802078 bgpneiget-2.0.0/src/bgpneiget/device/juniper.py
--rw-r--r--   0        0        0     1104 2023-05-18 09:46:19.385236 bgpneiget-2.0.0/src/bgpneiget/devices.py
--rw-r--r--   0        0        0     1574 2023-05-22 08:21:44.302857 bgpneiget-2.0.0/src/bgpneiget/runcmds.py
--rw-r--r--   0        0        0      243 2023-05-18 09:45:03.544509 bgpneiget-2.0.0/src/bgpneiget/textfsm/cisco_iosxe_show_bgp.textfsm
--rw-r--r--   0        0        0      529 2023-05-18 12:43:21.775962 bgpneiget-2.0.0/src/bgpneiget/textfsm/cisco_iosxe_show_bgp_vrf.textfsm
--rw-r--r--   0        0        0      510 2023-05-17 15:12:06.559095 bgpneiget-2.0.0/src/bgpneiget/textfsm/cisco_iosxr_show_bgp.textfsm
--rw-r--r--   0        0        0     3505 2023-06-12 15:16:04.745621 bgpneiget-2.0.0/src/bgpneiget/worker.py
--rw-r--r--   0        0        0     1151 1970-01-01 00:00:00.000000 bgpneiget-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1322 2023-05-12 08:43:10.928107 bgpneiget-2.0.1/LICENSE
+-rw-r--r--   0        0        0      288 2023-05-12 08:43:10.928107 bgpneiget-2.0.1/README.md
+-rw-r--r--   0        0        0      753 2023-06-20 09:52:11.289296 bgpneiget-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0      272 2023-06-20 09:52:22.449410 bgpneiget-2.0.1/src/bgpneiget/__init__.py
+-rw-r--r--   0        0        0     7430 2023-06-20 09:51:03.240596 bgpneiget-2.0.1/src/bgpneiget/cli.py
+-rw-r--r--   0        0        0        0 2023-05-12 12:50:58.436841 bgpneiget-2.0.1/src/bgpneiget/device/__init__.py
+-rw-r--r--   0        0        0      871 2023-05-17 08:19:38.384271 bgpneiget-2.0.1/src/bgpneiget/device/arista.py
+-rw-r--r--   0        0        0     2728 2023-05-18 12:43:21.775962 bgpneiget-2.0.1/src/bgpneiget/device/base.py
+-rw-r--r--   0        0        0    10196 2023-06-20 09:47:42.742520 bgpneiget-2.0.1/src/bgpneiget/device/cisco_iosxe.py
+-rw-r--r--   0        0        0     5906 2023-06-20 09:47:42.742520 bgpneiget-2.0.1/src/bgpneiget/device/cisco_iosxr.py
+-rw-r--r--   0        0        0     1137 2023-06-20 09:47:42.754520 bgpneiget-2.0.1/src/bgpneiget/device/cisco_nxos.py
+-rw-r--r--   0        0        0    10892 2023-06-20 09:47:42.754520 bgpneiget-2.0.1/src/bgpneiget/device/juniper.py
+-rw-r--r--   0        0        0     1104 2023-05-18 09:46:19.385236 bgpneiget-2.0.1/src/bgpneiget/devices.py
+-rw-r--r--   0        0        0     1574 2023-05-22 08:21:44.302857 bgpneiget-2.0.1/src/bgpneiget/runcmds.py
+-rw-r--r--   0        0        0      243 2023-05-18 09:45:03.544509 bgpneiget-2.0.1/src/bgpneiget/textfsm/cisco_iosxe_show_bgp.textfsm
+-rw-r--r--   0        0        0      529 2023-05-18 12:43:21.775962 bgpneiget-2.0.1/src/bgpneiget/textfsm/cisco_iosxe_show_bgp_vrf.textfsm
+-rw-r--r--   0        0        0      510 2023-05-17 15:12:06.559095 bgpneiget-2.0.1/src/bgpneiget/textfsm/cisco_iosxr_show_bgp.textfsm
+-rw-r--r--   0        0        0     3506 2023-06-20 09:51:03.240596 bgpneiget-2.0.1/src/bgpneiget/worker.py
+-rw-r--r--   0        0        0     1151 1970-01-01 00:00:00.000000 bgpneiget-2.0.1/PKG-INFO
```

### Comparing `bgpneiget-2.0.0/LICENSE` & `bgpneiget-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bgpneiget-2.0.0/pyproject.toml` & `bgpneiget-2.0.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bgpneiget"
-version = "2.0.0"
+version = "2.0.1"
 description = "Get BGP Neighbours from network devices"
 authors = ["Rob Woodward <rob@emailplus.org>"]
 
 license = "BSD-2-Clause"
 readme = "README.md"
 repository = "https://github.com/robwdwd/bgpneiget"
 include = ["README.md", "LICENSE"]
```

### Comparing `bgpneiget-2.0.0/src/bgpneiget/cli.py` & `bgpneiget-2.0.1/src/bgpneiget/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -51,14 +51,18 @@
 
         await db_con.commit()
         await db_cursor.close()
     except aiosqlite.Error as err:
         raise SystemExit(f"Failed to create new SQLite database: {err}") from err
 
     for device in devices.values():
+        if device["protocol"] == "TELNET" and prog_args["skip_telnet"]:
+            logger.info("[%s] Skipping device using telnet protocol.", device["hostname"])
+            continue
+
         if device["os"] in supported_os:
             new_device = await init_device(device)
             await queue.put(new_device)
         else:
             logger.warning("[%s] %s is not a supported OS.", {device["hostname"]}, {device["os"]})
 
     # Create three worker tasks to process the queue concurrently.
@@ -75,25 +79,31 @@
         for task in workers:
             task.cancel()
 
         await asyncio.gather(*workers, return_exceptions=True)
         await db_con.close()
         return
 
-    # Output CSV
+    # Output CSV or JSON
 
     db_con.row_factory = aiosqlite.Row
 
     async with db_con.execute("SELECT * FROM neighbours") as db_cursor:
         results = await db_cursor.fetchall()
         if prog_args["out_format"] == "json":
             print(json.dumps([dict(neighbour) for neighbour in results], indent=2, sort_keys=True))
         elif prog_args["out_format"] == "csv":
             lines = [dict(neighbour) for neighbour in results]
-            writer = csv.DictWriter(sys.stdout, fieldnames=lines[0].keys())
+            writer = csv.DictWriter(
+                sys.stdout,
+                fieldnames=lines[0].keys(),
+                dialect="unix",
+                quotechar=prog_args["quotechar"],
+                delimiter=prog_args["delimeter"],
+            )
             writer.writeheader()
             writer.writerows(lines)
 
         else:
             raise SystemExit("Invalid output format.")
 
     await db_con.close()
@@ -159,14 +169,29 @@
 @click.option(
     "--out-format",
     type=click.Choice(["json", "csv"], case_sensitive=False),
     metavar="FORMAT",
     default="json",
     help="Output format.",
 )
+@click.option(
+    "--delimiter",
+    type=str,
+    metavar="DELIMITER",
+    default=",",
+    help="Delimiter used for CSV output.",
+)
+@click.option(
+    "--quotechar",
+    type=str,
+    metavar="QUOTECHAR",
+    default='"',
+    help="Character used for quoting CSV fields.",
+)
+@click.option("--skip-telnet", is_flag=True)
 def cli(**cli_args):
     """Entry point for command.
 
     Raises:
         SystemExit: Error in command line options
     """
     try:
@@ -208,10 +233,13 @@
         "password": cfg["password"],
         "db_file": cfg["db_file"],
         "except_as": cli_args["except_as"],
         "ignore_as": cli_args["ignore_as"],
         "table": cli_args["table"],
         "with_vrfs": cli_args["with_vrfs"],
         "out_format": cli_args["out_format"],
+        "delimiter": cli_args["delimiter"],
+        "quotechar": cli_args["quotechar"],
+        "skip_telnet": cli_args["skip_telnet"],
     }
 
     asyncio.run(do_devices(devices, prog_args))
```

### Comparing `bgpneiget-2.0.0/src/bgpneiget/device/arista.py` & `bgpneiget-2.0.1/src/bgpneiget/device/arista.py`

 * *Files identical despite different names*

### Comparing `bgpneiget-2.0.0/src/bgpneiget/device/base.py` & `bgpneiget-2.0.1/src/bgpneiget/device/base.py`

 * *Files identical despite different names*

### Comparing `bgpneiget-2.0.0/src/bgpneiget/device/cisco_iosxe.py` & `bgpneiget-2.0.1/src/bgpneiget/device/cisco_iosxe.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import ipaddress
 import logging
 import os
 import pprint
 from typing import Type
 
 from scrapli.driver.core import AsyncIOSXEDriver
+from scrapli.exceptions import ScrapliException
 from textfsm import TextFSM
 
 from bgpneiget.device.base import BaseDevice
 from bgpneiget.runcmds import get_output
 
 pp = pprint.PrettyPrinter(indent=2, width=120)
 logger = logging.getLogger()
@@ -249,26 +250,29 @@
             prog_args (dict): Program arguments
 
         Returns:
             list: Found BGP neighbours
         """
         commands = {}
         reverse_commands = {}
+        result = []
 
         for table in prog_args["table"]:
             cmd = self.get_bgp_cmd_global(table)
             commands[table] = cmd
             reverse_commands[cmd] = table
 
-        response = await get_output(self, commands, prog_args["username"], prog_args["password"])
+        try:
+            response = await get_output(self, commands, prog_args["username"], prog_args["password"])
+        except ScrapliException as err:
+            logger.error("[%s] Can not get neighbours from device: %s", self.hostname, err)
+            return result
 
         loop = asyncio.get_running_loop()
 
-        result = []
-
         for resp in response:
             table = reverse_commands[resp.channel_input]
             if table in ("vpnv4", "vpnv6"):
                 template_file = "cisco_iosxe_show_bgp_vrf.textfsm"
                 parsed_result = await loop.run_in_executor(None, self.parse_bgp_neighbours, resp.result, template_file)
 
                 result = result + await self.process_bgp_neighbours_vpn(parsed_result, table, prog_args)
```

### Comparing `bgpneiget-2.0.0/src/bgpneiget/device/cisco_iosxr.py` & `bgpneiget-2.0.1/src/bgpneiget/device/cisco_iosxr.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import ipaddress
 import logging
 import os
 import pprint
 from typing import Type
 
 from scrapli.driver.core import AsyncIOSXRDriver
+from scrapli.exceptions import ScrapliException
 from textfsm import TextFSM
 
 from bgpneiget.device.base import BaseDevice
 from bgpneiget.runcmds import get_output
 
 pp = pprint.PrettyPrinter(indent=2, width=120)
 
@@ -150,25 +151,28 @@
             prog_args (dict): Program arguments
 
         Returns:
             list: Found BGP neighbours
         """
         commands = {}
         reverse_commands = {}
+        result = []
 
         for table in prog_args["table"]:
             cmd = self.get_bgp_cmd_global(table)
             commands[table] = cmd
             reverse_commands[cmd] = table
 
-        response = await get_output(self, commands, prog_args["username"], prog_args["password"])
+        try:
+            response = await get_output(self, commands, prog_args["username"], prog_args["password"])
+        except ScrapliException as err:
+            logger.error("[%s] Can not get neighbours from device: %s", self.hostname, err)
+            return result
 
         loop = asyncio.get_running_loop()
 
-        result = []
-
         for resp in response:
             table = reverse_commands[resp.channel_input]
             parsed_result = await loop.run_in_executor(None, self.parse_bgp_neighbours, resp.result)
             result = result + await self.process_bgp_neighbours(parsed_result, table, prog_args)
 
         return result
```

### Comparing `bgpneiget-2.0.0/src/bgpneiget/device/cisco_nxos.py` & `bgpneiget-2.0.1/src/bgpneiget/device/cisco_nxos.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import ipaddress
 import logging
 import os
 import pprint
 from typing import Type
 
 from scrapli.driver.core import AsyncNXOSDriver
+from scrapli.exceptions import ScrapliException
 from textfsm import TextFSM
 
 from bgpneiget.device.base import BaseDevice
 from bgpneiget.runcmds import get_output
 
 pp = pprint.PrettyPrinter(indent=2, width=120)
```

### Comparing `bgpneiget-2.0.0/src/bgpneiget/device/juniper.py` & `bgpneiget-2.0.1/src/bgpneiget/device/juniper.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import ipaddress
 import logging
 import pprint
 from typing import Type
 
 import xmltodict
 from scrapli.driver.core import AsyncJunosDriver
+from scrapli.exceptions import ScrapliException
 
 from bgpneiget.device.base import BaseDevice
 from bgpneiget.runcmds import get_output
 
 pp = pprint.PrettyPrinter(indent=2, width=120)
 
 logger = logging.getLogger()
@@ -294,19 +295,22 @@
         Args:
             prog_args (dict): Program arguments
 
         Returns:
             dict: Found BGP neighbours
         """
         commands = {}
+        result = []
 
         commands["all"] = self.get_bgp_cmd_global()
 
-        response = await get_output(self, commands, prog_args["username"], prog_args["password"])
-
-        result = []
+        try:
+            response = await get_output(self, commands, prog_args["username"], prog_args["password"])
+        except ScrapliException as err:
+            logger.error("[%s] Can not get neighbours from device: %s", self.hostname, err)
+            return result
 
         for resp in response:
             stripped_response = resp.result[: resp.result.rfind("\n")]
             result = result + await self.process_bgp_neighbours(stripped_response, prog_args)
 
         return result
```

### Comparing `bgpneiget-2.0.0/src/bgpneiget/devices.py` & `bgpneiget-2.0.1/src/bgpneiget/devices.py`

 * *Files identical despite different names*

### Comparing `bgpneiget-2.0.0/src/bgpneiget/runcmds.py` & `bgpneiget-2.0.1/src/bgpneiget/runcmds.py`

 * *Files identical despite different names*

### Comparing `bgpneiget-2.0.0/src/bgpneiget/textfsm/cisco_iosxe_show_bgp_vrf.textfsm` & `bgpneiget-2.0.1/src/bgpneiget/textfsm/cisco_iosxe_show_bgp_vrf.textfsm`

 * *Files identical despite different names*

### Comparing `bgpneiget-2.0.0/src/bgpneiget/worker.py` & `bgpneiget-2.0.1/src/bgpneiget/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         self.db_lock = db_lock
         self.prog_args = prog_args
         self.db_cursor = None
 
     async def run(self, i: int) -> None:
         """Device worker coroutine, reads from the queue until empty."""
         try:
-            #if i == 1:
+            # if i == 1:
             #    raise DeviceWorkerException("test")
 
             try:
                 self.db_cursor = await self.db_con.cursor()
             except aiosqlite.Error as err:
                 raise DeviceWorkerException(f"Worker {i} failed to create db cursor: {err}") from err
```

### Comparing `bgpneiget-2.0.0/PKG-INFO` & `bgpneiget-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bgpneiget
-Version: 2.0.0
+Version: 2.0.1
 Summary: Get BGP Neighbours from network devices
 Home-page: https://github.com/robwdwd/bgpneiget
 License: BSD-2-Clause
 Author: Rob Woodward
 Author-email: rob@emailplus.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
```

