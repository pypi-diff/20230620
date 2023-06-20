# Comparing `tmp/ssh_remote_control-0.1.1.tar.gz` & `tmp/ssh_remote_control-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssh_remote_control-0.1.1.tar", last modified: Mon Jun 19 13:11:15 2023, max compression
+gzip compressed data, was "ssh_remote_control-0.1.2.tar", last modified: Tue Jun 20 06:47:45 2023, max compression
```

## Comparing `ssh_remote_control-0.1.1.tar` & `ssh_remote_control-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 13:11:15.887416 ssh_remote_control-0.1.1/
--rw-rw-rw-   0        0        0     1084 2023-06-19 04:51:08.000000 ssh_remote_control-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     1428 2023-06-19 13:11:15.886417 ssh_remote_control-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      832 2023-06-19 10:07:10.000000 ssh_remote_control-0.1.1/README.md
--rw-rw-rw-   0        0        0      848 2023-06-19 12:29:01.000000 ssh_remote_control-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-19 13:11:15.887416 ssh_remote_control-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-19 13:11:15.794908 ssh_remote_control-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-19 13:11:15.824911 ssh_remote_control-0.1.1/src/ssh_remote_control/
--rw-rw-rw-   0        0        0    10774 2023-06-19 09:31:24.000000 ssh_remote_control-0.1.1/src/ssh_remote_control/__init__.py
--rw-rw-rw-   0        0        0     6656 2023-06-19 04:57:57.000000 ssh_remote_control-0.1.1/src/ssh_remote_control/command.py
-drwxrwxrwx   0        0        0        0 2023-06-19 13:11:15.883419 ssh_remote_control-0.1.1/src/ssh_remote_control/default_commands/
--rw-rw-rw-   0        0        0      111 2023-06-19 03:25:53.000000 ssh_remote_control-0.1.1/src/ssh_remote_control/default_commands/__init__.py
--rw-rw-rw-   0        0        0     1006 2023-06-19 01:38:24.000000 ssh_remote_control-0.1.1/src/ssh_remote_control/default_commands/const.py
--rw-rw-rw-   0        0        0     3757 2023-06-19 10:12:42.000000 ssh_remote_control-0.1.1/src/ssh_remote_control/default_commands/linux.py
--rw-rw-rw-   0        0        0     3304 2023-06-19 10:13:12.000000 ssh_remote_control-0.1.1/src/ssh_remote_control/default_commands/windows_cmd.py
--rw-rw-rw-   0        0        0     3538 2023-06-19 10:14:03.000000 ssh_remote_control-0.1.1/src/ssh_remote_control/default_commands/windows_ps.py
--rw-rw-rw-   0        0        0      550 2023-06-19 03:37:58.000000 ssh_remote_control-0.1.1/src/ssh_remote_control/event.py
--rw-rw-rw-   0        0        0      159 2023-06-19 09:54:09.000000 ssh_remote_control-0.1.1/src/ssh_remote_control/helpers.py
--rw-rw-rw-   0        0        0     1313 2023-06-19 04:04:40.000000 ssh_remote_control-0.1.1/src/ssh_remote_control/locker.py
--rw-rw-rw-   0        0        0     6518 2023-06-19 04:58:47.000000 ssh_remote_control-0.1.1/src/ssh_remote_control/manager.py
--rw-rw-rw-   0        0        0     5891 2023-06-19 04:59:09.000000 ssh_remote_control-0.1.1/src/ssh_remote_control/sensor.py
-drwxrwxrwx   0        0        0        0 2023-06-19 13:11:15.869406 ssh_remote_control-0.1.1/src/ssh_remote_control.egg-info/
--rw-rw-rw-   0        0        0     1428 2023-06-19 13:11:15.000000 ssh_remote_control-0.1.1/src/ssh_remote_control.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      755 2023-06-19 13:11:15.000000 ssh_remote_control-0.1.1/src/ssh_remote_control.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 13:11:15.000000 ssh_remote_control-0.1.1/src/ssh_remote_control.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2023-06-19 13:11:15.000000 ssh_remote_control-0.1.1/src/ssh_remote_control.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-19 13:11:15.000000 ssh_remote_control-0.1.1/src/ssh_remote_control.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 06:47:45.159800 ssh_remote_control-0.1.2/
+-rw-rw-rw-   0        0        0     1084 2023-06-19 04:51:08.000000 ssh_remote_control-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     1569 2023-06-20 06:47:45.158798 ssh_remote_control-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      973 2023-06-20 06:12:24.000000 ssh_remote_control-0.1.2/README.md
+-rw-rw-rw-   0        0        0      846 2023-06-20 06:42:33.000000 ssh_remote_control-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-20 06:47:45.159800 ssh_remote_control-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-20 06:47:45.080802 ssh_remote_control-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-20 06:47:45.111800 ssh_remote_control-0.1.2/src/ssh_remote_control/
+-rw-rw-rw-   0        0        0    10675 2023-06-20 05:39:06.000000 ssh_remote_control-0.1.2/src/ssh_remote_control/__init__.py
+-rw-rw-rw-   0        0        0     6710 2023-06-20 05:39:06.000000 ssh_remote_control-0.1.2/src/ssh_remote_control/command.py
+-rw-rw-rw-   0        0        0     2882 2023-06-20 05:39:06.000000 ssh_remote_control-0.1.2/src/ssh_remote_control/command_set.py
+drwxrwxrwx   0        0        0        0 2023-06-20 06:47:45.156797 ssh_remote_control-0.1.2/src/ssh_remote_control/default_command_sets/
+-rw-rw-rw-   0        0        0      163 2023-06-20 05:39:07.000000 ssh_remote_control-0.1.2/src/ssh_remote_control/default_command_sets/__init__.py
+-rw-rw-rw-   0        0        0     1006 2023-06-20 05:39:07.000000 ssh_remote_control-0.1.2/src/ssh_remote_control/default_command_sets/const.py
+-rw-rw-rw-   0        0        0     4345 2023-06-20 05:39:07.000000 ssh_remote_control-0.1.2/src/ssh_remote_control/default_command_sets/linux.py
+-rw-rw-rw-   0        0        0     3822 2023-06-20 05:39:07.000000 ssh_remote_control-0.1.2/src/ssh_remote_control/default_command_sets/windows_cmd.py
+-rw-rw-rw-   0        0        0     4079 2023-06-20 05:39:07.000000 ssh_remote_control-0.1.2/src/ssh_remote_control/default_command_sets/windows_ps.py
+-rw-rw-rw-   0        0        0      645 2023-06-20 05:39:06.000000 ssh_remote_control-0.1.2/src/ssh_remote_control/event.py
+-rw-rw-rw-   0        0        0      159 2023-06-20 05:39:06.000000 ssh_remote_control-0.1.2/src/ssh_remote_control/helpers.py
+-rw-rw-rw-   0        0        0     1313 2023-06-20 05:39:06.000000 ssh_remote_control-0.1.2/src/ssh_remote_control/locker.py
+-rw-rw-rw-   0        0        0     3885 2023-06-20 05:39:06.000000 ssh_remote_control-0.1.2/src/ssh_remote_control/manager.py
+-rw-rw-rw-   0        0        0     5891 2023-06-20 05:39:06.000000 ssh_remote_control-0.1.2/src/ssh_remote_control/sensor.py
+drwxrwxrwx   0        0        0        0 2023-06-20 06:47:45.146798 ssh_remote_control-0.1.2/src/ssh_remote_control.egg-info/
+-rw-rw-rw-   0        0        0     1569 2023-06-20 06:47:45.000000 ssh_remote_control-0.1.2/src/ssh_remote_control.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      813 2023-06-20 06:47:45.000000 ssh_remote_control-0.1.2/src/ssh_remote_control.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 06:47:45.000000 ssh_remote_control-0.1.2/src/ssh_remote_control.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2023-06-20 06:47:45.000000 ssh_remote_control-0.1.2/src/ssh_remote_control.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-20 06:47:45.000000 ssh_remote_control-0.1.2/src/ssh_remote_control.egg-info/top_level.txt
```

### Comparing `ssh_remote_control-0.1.1/LICENSE` & `ssh_remote_control-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.1/pyproject.toml` & `ssh_remote_control-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ssh_remote_control"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="zhbjsh", email="zhbjsh@outlook.com" },
 ]
 description = "Control and monitor remote devices through SSH"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -19,15 +19,15 @@
 keywords = [
   "ssh", 
   "command line", 
   "remote control",
 ]
 dependencies = [
   "async-timeout >= 4.0.2",
-  "icmplib >= 3.0.3",
+  "icmplib >= 3.0",
   "paramiko >= 3.2.0",
   "python-slugify >= 4.0.1",
   "wakeonlan >= 3.0.0",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/zhbjsh/ssh-remote-control"
```

### Comparing `ssh_remote_control-0.1.1/src/ssh_remote_control/__init__.py` & `ssh_remote_control-0.1.2/src/ssh_remote_control/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """SSH remote control."""
 from __future__ import annotations
 
 import asyncio
 import logging
+from time import time
 
 import async_timeout
 import icmplib
 import paramiko
 import wakeonlan
 
 from .command import (
     Command,
     CommandFormatError,
     CommandOutput,
     SensorCommand,
     ServiceCommand,
 )
-from .default_commands import SensorKey, ServiceKey
+from .command_set import CommandSet
+from .default_command_sets import SensorKey, ServiceKey
 from .event import Event
 from .manager import DEFAULT_COMMAND_TIMEOUT, CommandExecuteError, Manager
 from .sensor import DynamicSensor, Sensor
 
 _LOGGER = logging.getLogger(__name__)
 
 DEFAULT_SSH_PORT = 22
@@ -45,92 +47,88 @@
 class State:
     """The State class."""
 
     is_online: bool = False
     is_connected: bool = False
 
     def __init__(self, remote: Remote) -> None:
-        self.remote = remote
+        self._remote = remote
         self.on_change = Event()
 
     def update(self, name, value) -> None:
         """Update."""
         if getattr(self, name) == value:
             return
 
         setattr(self, name, value)
-        self.remote.logger.info(
-            "%s: State %s changed to %s", self.remote.name, name, value
-        )
+        self._remote.logger.info("%s: %s changed to %s", self._remote.name, name, value)
         self.on_change.notify(self)
 
 
 class Remote(Manager):
     """The Remote class."""
 
     def __init__(
         self,
         host: str,
         *,
         name: str | None = None,
+        command_set: CommandSet | None = None,
         add_host_keys: bool = DEFAULT_ADD_HOST_KEYS,
         ssh_port: int = DEFAULT_SSH_PORT,
         ssh_user: str | None = None,
         ssh_password: str | None = None,
         ssh_key_file: str | None = None,
         ssh_host_keys_file: str | None = None,
         ssh_timeout: int = DEFAULT_SSH_TIMEOUT,
         ping_timeout: int = DEFAULT_PING_TIMEOUT,
         command_timeout: int = DEFAULT_COMMAND_TIMEOUT,
         allow_turn_off: bool = DEFAULT_ALLOW_TURN_OFF,
         mac_address: str | None = None,
-        service_commands: list[ServiceCommand] | None = None,
-        sensor_commands: list[SensorCommand] | None = None,
         logger: logging.Logger = _LOGGER,
     ) -> None:
         super().__init__(
             name=name or host,
+            command_set=command_set,
             command_timeout=command_timeout,
-            service_commands=service_commands,
-            sensor_commands=sensor_commands,
             logger=logger,
         )
         self.host = host
         self.ssh_port = ssh_port
         self.ssh_user = ssh_user
         self.ssh_password = ssh_password
         self.ssh_key_file = ssh_key_file
         self.ssh_timeout = ssh_timeout
         self.ping_timeout = ping_timeout
         self.allow_turn_off = allow_turn_off
-        self.preset_mac_address = mac_address
+        self._mac_address = mac_address
         self.state = State(self)
-        self.ssh_client = paramiko.SSHClient()
-        self.ssh_client.set_log_channel(self.logger.name)
-        self.ssh_client.load_system_host_keys()
-        self.ssh_client.set_missing_host_key_policy(
+        self._ssh_client = paramiko.SSHClient()
+        self._ssh_client.set_log_channel(self.logger.name)
+        self._ssh_client.load_system_host_keys()
+        self._ssh_client.set_missing_host_key_policy(
             paramiko.AutoAddPolicy if add_host_keys else CustomRejectPolicy
         )
 
         if ssh_host_keys_file:
             with open(ssh_host_keys_file, "a", encoding="utf-8"):
                 pass
-            self.ssh_client.load_host_keys(ssh_host_keys_file)
+            self._ssh_client.load_host_keys(ssh_host_keys_file)
 
     @property
     def hostname(self) -> str | None:
         """Hostname."""
         if sensor := self.sensors_by_key.get(SensorKey.HOSTNAME):
             return sensor.last_known_value
 
     @property
     def mac_address(self) -> str | None:
         """MAC address."""
-        if self.preset_mac_address:
-            return self.preset_mac_address
+        if self._mac_address:
+            return self._mac_address
         if sensor := self.sensors_by_key.get(SensorKey.MAC_ADDRESS):
             return sensor.last_known_value
 
     @property
     def wol_support(self) -> bool | None:
         """Wake on LAN support."""
         if sensor := self.sensors_by_key.get(SensorKey.WOL_SUPPORT):
@@ -155,37 +153,38 @@
             return sensor.last_known_value
 
     def _execute_command_string(self, string: str) -> CommandOutput:
         if not self.state.is_connected:
             raise CommandExecuteError("Not connected")
 
         try:
-            _, stdout_file, stderr_file = self.ssh_client.exec_command(
+            _, stdout_file, stderr_file = self._ssh_client.exec_command(
                 string, timeout=float(self.ssh_timeout)
             )
         except Exception as exc:
             self._disconnect()
             raise CommandExecuteError("Disconnected during execution") from exc
 
         try:
             return CommandOutput(
+                time(),
                 [line.strip() for line in stdout_file.readlines()],
                 [line.strip() for line in stderr_file.readlines()],
                 stdout_file.channel.recv_exit_status(),
             )
         except Exception as exc:
             self._disconnect()
             raise CommandExecuteError("Disconnected after execution") from exc
 
     def _connect(self) -> None:
         if self.state.is_connected:
             return
 
         try:
-            self.ssh_client.connect(
+            self._ssh_client.connect(
                 self.host,
                 self.ssh_port,
                 self.ssh_user,
                 self.ssh_password,
                 key_filename=self.ssh_key_file,
                 timeout=self.ssh_timeout,
                 allow_agent=False,
@@ -202,15 +201,15 @@
 
         self.state.update(IS_CONNECTED, True)
 
     def _disconnect(self) -> None:
         if not self.state.is_connected:
             return
 
-        self.ssh_client.close()
+        self._ssh_client.close()
         self.state.update(IS_CONNECTED, False)
 
         for command in self.sensor_commands:
             command.set_sensor_values(None)
 
     async def async_execute_command_string(
         self, string: str, command_timeout: int | None = None
@@ -252,15 +251,15 @@
 
         Set `state.is_connected` to `False` and the
         sensor values of all sensor commands to `None`.
         """
         loop = asyncio.get_running_loop()
         await loop.run_in_executor(None, self._disconnect)
 
-    async def async_update_state(self, validate: bool = False) -> None:
+    async def async_update_state(self, *, validate: bool = False) -> None:
         """Update state.
 
         Raises:
             OfflineError (validate)
             SSHHostKeyUnknownError
             SSHAuthError
             SSHConnectError (validate)
@@ -310,15 +309,14 @@
 
         wakeonlan.send_magic_packet(self.mac_address)
 
     async def turn_off(self) -> None:
         """Turn the host on.
 
         Raises:
-            KeyError
             CommandFormatError
             CommandExecuteError
         """
         if self.allow_turn_off is False:
             return
 
         await self.async_call_service(ServiceKey.TURN_OFF)
```

### Comparing `ssh_remote_control-0.1.1/src/ssh_remote_control/command.py` & `ssh_remote_control-0.1.2/src/ssh_remote_control/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     from .manager import Manager
 
 
 @dataclass(frozen=True)
 class CommandOutput:
     """The CommandOutput class."""
 
+    timestamp: float
     stdout: list[str] | None = None
     stderr: list[str] | None = None
     code: int | None = None
 
 
 class Command:
     """The Command class."""
@@ -180,15 +181,16 @@
         """Remove a sensor."""
         self.sensors = [
             Sensor("") if sensor.key == key else sensor for sensor in self.sensors
         ]
 
     def set_sensor_values(self, output: CommandOutput | None) -> None:
         """Set sensor values."""
-        self.last_update = time()
+        if output:
+            self.last_update = output.timestamp
 
         if isinstance(self.sensors[0], DynamicSensor):
             if not output or output.code != 0:
                 pairs = None
 
             else:
                 lines = [line.split(self.separator, 1) for line in output.stdout]
```

### Comparing `ssh_remote_control-0.1.1/src/ssh_remote_control/default_commands/const.py` & `ssh_remote_control-0.1.2/src/ssh_remote_control/default_command_sets/const.py`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.1/src/ssh_remote_control/default_commands/linux.py` & `ssh_remote_control-0.1.2/src/ssh_remote_control/default_command_sets/linux.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,145 +1,146 @@
 from ..command import Command, SensorCommand, ServiceCommand
+from ..command_set import CommandSet
 from ..sensor import DynamicSensor, Sensor
 from .const import SensorKey, SensorName, ServiceKey, ServiceName
 
-NAME = "Linux"
-
-services = [
-    ServiceCommand(
-        "/sbin/shutdown -h now",
-        ServiceName.TURN_OFF,
-        ServiceKey.TURN_OFF,
-    ),
-    ServiceCommand(
-        "/sbin/shutdown -r now",
-        ServiceName.RESTART,
-        ServiceKey.RESTART,
-    ),
-]
-
-sensors = [
-    SensorCommand(
-        "cat hundi",
-        [
-            DynamicSensor(
-                "Hundi",
-                value_type=bool,
-                switch_on=Command("sed -i -e 's/{id} off/{id} on/g' hundi"),
-                switch_off=Command("sed -i -e 's/{id} on/{id} off/g' hundi"),
-            )
-        ],
-    ),
-    SensorCommand(
-        "cat /sys/class/net/{interface}/address",
-        [
-            Sensor(
-                SensorName.MAC_ADDRESS,
-                SensorKey.MAC_ADDRESS,
-            )
-        ],
-    ),
-    SensorCommand(
-        "cat /sys/class/net/{interface}/device/power/wakeup",
-        [
-            Sensor(
-                SensorName.WOL_SUPPORT,
-                SensorKey.WOL_SUPPORT,
-                value_type=bool,
-                payload_on="enabled",
-            )
-        ],
-    ),
-    SensorCommand(
-        "/sbin/route -n | awk '($1 == \"0.0.0.0\") {{print $NF; exit}}'",
-        [
-            Sensor(
-                SensorName.INTERFACE,
-                SensorKey.INTERFACE,
-            )
-        ],
-    ),
-    SensorCommand(
-        "uname -a | awk '{{print $1; print $3; print $2; print $(NF-1);}}'",
-        [
-            Sensor(
-                SensorName.OS_NAME,
-                SensorKey.OS_NAME,
-            ),
-            Sensor(
-                SensorName.OS_VERSION,
-                SensorKey.OS_VERSION,
-            ),
-            Sensor(
-                SensorName.HOSTNAME,
-                SensorKey.HOSTNAME,
-            ),
-            Sensor(
-                SensorName.MACHINE_TYPE,
-                SensorKey.MACHINE_TYPE,
-            ),
-        ],
-    ),
-    # TODO: OS_ARCHITECTURE
-    SensorCommand(
-        "free -m | awk 'tolower($0)~/mem/ {{print $2}}'",
-        [
-            Sensor(
-                SensorName.TOTAL_MEMORY,
-                SensorKey.TOTAL_MEMORY,
-                value_type=int,
-                value_unit="MB",
-            )
-        ],
-    ),
-    SensorCommand(
-        "free -m | awk 'tolower($0)~/mem/ {{print $4}}'",
-        [
-            Sensor(
-                SensorName.FREE_MEMORY,
-                SensorKey.FREE_MEMORY,
-                value_type=int,
-                value_unit="MB",
-            )
-        ],
-        interval=30,
-    ),
-    SensorCommand(
-        "df -m | awk '/^\\/dev\\// {{print $6 \"|\" $4}}'",
-        [
-            DynamicSensor(
-                SensorName.FREE_DISK_SPACE,
-                SensorKey.FREE_DISK_SPACE,
-                value_type=int,
-                value_unit="MB",
-            )
-        ],
-        interval=300,
-        separator="|",
-    ),
-    SensorCommand(
-        "top -bn1 | head -n3 | awk 'tolower($0)~/cpu/ "
-        + "{{for(i=1;i<NF;i++){{if(tolower($i)~/cpu/)"
-        + "{{idle=$(i+7); print 100-idle;}}}}}}'",
-        [
-            Sensor(
-                SensorName.CPU_LOAD,
-                SensorKey.CPU_LOAD,
-                value_type=int,
-                value_unit="%",
-            )
-        ],
-        interval=30,
-    ),
-    SensorCommand(
-        "echo $(($(cat /sys/class/thermal/thermal_zone0/temp) / 1000))",
-        [
-            Sensor(
-                SensorName.TEMPERATURE,
-                SensorKey.TEMPERATURE,
-                value_type=int,
-                value_unit="°C",
-            )
-        ],
-        interval=60,
-    ),
-]
+linux = CommandSet(
+    "Linux",
+    [
+        ServiceCommand(
+            "/sbin/shutdown -h now",
+            ServiceName.TURN_OFF,
+            ServiceKey.TURN_OFF,
+        ),
+        ServiceCommand(
+            "/sbin/shutdown -r now",
+            ServiceName.RESTART,
+            ServiceKey.RESTART,
+        ),
+    ],
+    [
+        SensorCommand(
+            "cat hundi",
+            [
+                DynamicSensor(
+                    "Hundi",
+                    value_type=bool,
+                    switch_on=Command("sed -i -e 's/{id} off/{id} on/g' hundi"),
+                    switch_off=Command("sed -i -e 's/{id} on/{id} off/g' hundi"),
+                )
+            ],
+        ),
+        SensorCommand(
+            "cat /sys/class/net/{interface}/address",
+            [
+                Sensor(
+                    SensorName.MAC_ADDRESS,
+                    SensorKey.MAC_ADDRESS,
+                )
+            ],
+        ),
+        SensorCommand(
+            "cat /sys/class/net/{interface}/device/power/wakeup",
+            [
+                Sensor(
+                    SensorName.WOL_SUPPORT,
+                    SensorKey.WOL_SUPPORT,
+                    value_type=bool,
+                    payload_on="enabled",
+                )
+            ],
+        ),
+        SensorCommand(
+            "/sbin/route -n | awk '($1 == \"0.0.0.0\") {{print $NF; exit}}'",
+            [
+                Sensor(
+                    SensorName.INTERFACE,
+                    SensorKey.INTERFACE,
+                )
+            ],
+        ),
+        SensorCommand(
+            "uname -a | awk '{{print $1; print $3; print $2; print $(NF-1);}}'",
+            [
+                Sensor(
+                    SensorName.OS_NAME,
+                    SensorKey.OS_NAME,
+                ),
+                Sensor(
+                    SensorName.OS_VERSION,
+                    SensorKey.OS_VERSION,
+                ),
+                Sensor(
+                    SensorName.HOSTNAME,
+                    SensorKey.HOSTNAME,
+                ),
+                Sensor(
+                    SensorName.MACHINE_TYPE,
+                    SensorKey.MACHINE_TYPE,
+                ),
+            ],
+        ),
+        # TODO: OS_ARCHITECTURE
+        SensorCommand(
+            "free -m | awk 'tolower($0)~/mem/ {{print $2}}'",
+            [
+                Sensor(
+                    SensorName.TOTAL_MEMORY,
+                    SensorKey.TOTAL_MEMORY,
+                    value_type=int,
+                    value_unit="MB",
+                )
+            ],
+        ),
+        SensorCommand(
+            "free -m | awk 'tolower($0)~/mem/ {{print $4}}'",
+            [
+                Sensor(
+                    SensorName.FREE_MEMORY,
+                    SensorKey.FREE_MEMORY,
+                    value_type=int,
+                    value_unit="MB",
+                )
+            ],
+            interval=30,
+        ),
+        SensorCommand(
+            "df -m | awk '/^\\/dev\\// {{print $6 \"|\" $4}}'",
+            [
+                DynamicSensor(
+                    SensorName.FREE_DISK_SPACE,
+                    SensorKey.FREE_DISK_SPACE,
+                    value_type=int,
+                    value_unit="MB",
+                )
+            ],
+            interval=300,
+            separator="|",
+        ),
+        SensorCommand(
+            "top -bn1 | head -n3 | awk 'tolower($0)~/cpu/ "
+            + "{{for(i=1;i<NF;i++){{if(tolower($i)~/cpu/)"
+            + "{{idle=$(i+7); print 100-idle;}}}}}}'",
+            [
+                Sensor(
+                    SensorName.CPU_LOAD,
+                    SensorKey.CPU_LOAD,
+                    value_type=int,
+                    value_unit="%",
+                )
+            ],
+            interval=30,
+        ),
+        SensorCommand(
+            "echo $(($(cat /sys/class/thermal/thermal_zone0/temp) / 1000))",
+            [
+                Sensor(
+                    SensorName.TEMPERATURE,
+                    SensorKey.TEMPERATURE,
+                    value_type=int,
+                    value_unit="°C",
+                )
+            ],
+            interval=60,
+        ),
+    ],
+)
```

### Comparing `ssh_remote_control-0.1.1/src/ssh_remote_control/default_commands/windows_cmd.py` & `ssh_remote_control-0.1.2/src/ssh_remote_control/default_command_sets/windows_cmd.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,126 +1,127 @@
 from ..command import SensorCommand, ServiceCommand
+from ..command_set import CommandSet
 from ..sensor import Sensor
 from .const import SensorKey, SensorName, ServiceKey, ServiceName
 
-NAME = "Windows"
-
-services = [
-    ServiceCommand(
-        "shutdown -t 0",
-        ServiceName.TURN_OFF,
-        ServiceKey.TURN_OFF,
-    ),
-    ServiceCommand(
-        "shutdown -r -t 0",
-        ServiceName.RESTART,
-        ServiceKey.RESTART,
-    ),
-]
-
-sensors = [
-    # TODO: MAC_ADDRESS
-    # TODO: WOL_SUPPORT
-    # TODO: INTERFACE
-    SensorCommand(
-        "for /f \"skip=1 delims=\" %i in ('wmic ComputerSystem get SystemType') "
-        + "do @echo %i",
-        [
-            Sensor(
-                SensorName.MACHINE_TYPE,
-                SensorKey.MACHINE_TYPE,
-            )
-        ],
-    ),
-    SensorCommand(
-        "hostname",
-        [
-            Sensor(
-                SensorName.HOSTNAME,
-                SensorKey.HOSTNAME,
-            )
-        ],
-    ),
-    SensorCommand(
-        "for /f \"skip=1 delims=\" %i in ('wmic OS get Caption') do @echo %i",
-        [
-            Sensor(
-                SensorName.OS_NAME,
-                SensorKey.OS_NAME,
-            )
-        ],
-    ),
-    SensorCommand(
-        "for /f \"skip=1 delims=\" %i in ('wmic OS get Version') do @echo %i",
-        [
-            Sensor(
-                SensorName.OS_VERSION,
-                SensorKey.OS_VERSION,
-            )
-        ],
-    ),
-    SensorCommand(
-        "for /f \"skip=1 delims=\" %i in ('wmic OS get OSArchitecture') do @echo %i",
-        [
-            Sensor(
-                SensorName.OS_ARCHITECTURE,
-                SensorKey.OS_ARCHITECTURE,
-            )
-        ],
-    ),
-    SensorCommand(
-        # TODO: Should return MB but number is too long
-        "for /f  %i in ('wmic ComputerSystem get TotalPhysicalMemory ^| "
-        + 'findstr /r "\\<[0-9][0-9]*\\>"\') '
-        + "do set /a mb=%i / 1024 / 1024",
-        [
-            Sensor(
-                SensorName.TOTAL_MEMORY,
-                SensorKey.TOTAL_MEMORY,
-                value_type=int,
-                value_unit="MB",
-            )
-        ],
-    ),
-    SensorCommand(
-        "for /f  %i in ('wmic OS get FreePhysicalMemory ^| "
-        + 'findstr /r "\\<[0-9][0-9]*\\>"\') '
-        + "do set /a mb=%i / 1024",
-        [
-            Sensor(
-                SensorName.FREE_MEMORY,
-                SensorKey.FREE_MEMORY,
-                value_type=int,
-                value_unit="MB",
-            )
-        ],
-        interval=30,
-    ),
-    # TODO: FREE_DISK_SPACE
-    SensorCommand(
-        "for /f \"skip=1\" %i in ('wmic CPU get LoadPercentage') do @echo %i",
-        [
-            Sensor(
-                SensorName.CPU_LOAD,
-                SensorKey.CPU_LOAD,
-                value_type=int,
-                value_unit="%",
-            )
-        ],
-        interval=30,
-    ),
-    SensorCommand(
-        "for /f  %i in ('wmic /namespace:\\\\root\\wmi "
-        + "PATH MSAcpi_ThermalZoneTemperature get CurrentTemperature ^| "
-        + 'findstr /r "\\<[0-9][0-9]*\\>"\') '
-        + "do set /a mb=(%i - 2732) / 10",
-        [
-            Sensor(
-                SensorName.TEMPERATURE,
-                SensorKey.TEMPERATURE,
-                value_type=int,
-                value_unit="°C",
-            )
-        ],
-        interval=60,
-    ),
-]
+windows_cmd = CommandSet(
+    "Windows",
+    [
+        ServiceCommand(
+            "shutdown -t 0",
+            ServiceName.TURN_OFF,
+            ServiceKey.TURN_OFF,
+        ),
+        ServiceCommand(
+            "shutdown -r -t 0",
+            ServiceName.RESTART,
+            ServiceKey.RESTART,
+        ),
+    ],
+    [
+        # TODO: MAC_ADDRESS
+        # TODO: WOL_SUPPORT
+        # TODO: INTERFACE
+        SensorCommand(
+            "for /f \"skip=1 delims=\" %i in ('wmic ComputerSystem get SystemType') "
+            + "do @echo %i",
+            [
+                Sensor(
+                    SensorName.MACHINE_TYPE,
+                    SensorKey.MACHINE_TYPE,
+                )
+            ],
+        ),
+        SensorCommand(
+            "hostname",
+            [
+                Sensor(
+                    SensorName.HOSTNAME,
+                    SensorKey.HOSTNAME,
+                )
+            ],
+        ),
+        SensorCommand(
+            "for /f \"skip=1 delims=\" %i in ('wmic OS get Caption') do @echo %i",
+            [
+                Sensor(
+                    SensorName.OS_NAME,
+                    SensorKey.OS_NAME,
+                )
+            ],
+        ),
+        SensorCommand(
+            "for /f \"skip=1 delims=\" %i in ('wmic OS get Version') do @echo %i",
+            [
+                Sensor(
+                    SensorName.OS_VERSION,
+                    SensorKey.OS_VERSION,
+                )
+            ],
+        ),
+        SensorCommand(
+            "for /f \"skip=1 delims=\" %i in ('wmic OS get OSArchitecture') do @echo %i",
+            [
+                Sensor(
+                    SensorName.OS_ARCHITECTURE,
+                    SensorKey.OS_ARCHITECTURE,
+                )
+            ],
+        ),
+        SensorCommand(
+            # TODO: Should return MB but number is too long
+            "for /f  %i in ('wmic ComputerSystem get TotalPhysicalMemory ^| "
+            + 'findstr /r "\\<[0-9][0-9]*\\>"\') '
+            + "do set /a mb=%i / 1024 / 1024",
+            [
+                Sensor(
+                    SensorName.TOTAL_MEMORY,
+                    SensorKey.TOTAL_MEMORY,
+                    value_type=int,
+                    value_unit="MB",
+                )
+            ],
+        ),
+        SensorCommand(
+            "for /f  %i in ('wmic OS get FreePhysicalMemory ^| "
+            + 'findstr /r "\\<[0-9][0-9]*\\>"\') '
+            + "do set /a mb=%i / 1024",
+            [
+                Sensor(
+                    SensorName.FREE_MEMORY,
+                    SensorKey.FREE_MEMORY,
+                    value_type=int,
+                    value_unit="MB",
+                )
+            ],
+            interval=30,
+        ),
+        # TODO: FREE_DISK_SPACE
+        SensorCommand(
+            "for /f \"skip=1\" %i in ('wmic CPU get LoadPercentage') do @echo %i",
+            [
+                Sensor(
+                    SensorName.CPU_LOAD,
+                    SensorKey.CPU_LOAD,
+                    value_type=int,
+                    value_unit="%",
+                )
+            ],
+            interval=30,
+        ),
+        SensorCommand(
+            "for /f  %i in ('wmic /namespace:\\\\root\\wmi "
+            + "PATH MSAcpi_ThermalZoneTemperature get CurrentTemperature ^| "
+            + 'findstr /r "\\<[0-9][0-9]*\\>"\') '
+            + "do set /a mb=(%i - 2732) / 10",
+            [
+                Sensor(
+                    SensorName.TEMPERATURE,
+                    SensorKey.TEMPERATURE,
+                    value_type=int,
+                    value_unit="°C",
+                )
+            ],
+            interval=60,
+        ),
+    ],
+)
```

### Comparing `ssh_remote_control-0.1.1/src/ssh_remote_control/default_commands/windows_ps.py` & `ssh_remote_control-0.1.2/src/ssh_remote_control/default_command_sets/windows_ps.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,132 +1,133 @@
 from ..command import SensorCommand, ServiceCommand
+from ..command_set import CommandSet
 from ..sensor import DynamicSensor, Sensor
 from .const import SensorKey, SensorName, ServiceKey, ServiceName
 
-NAME = "Windows (Power Shell)"
-
-services = [
-    ServiceCommand(
-        "Stop-Computer -Force",
-        ServiceName.TURN_OFF,
-        ServiceKey.TURN_OFF,
-    ),
-    ServiceCommand(
-        "Restart-Computer -Force",
-        ServiceName.RESTART,
-        ServiceKey.RESTART,
-    ),
-]
-
-sensors = [
-    # TODO: MAC_ADDRESS
-    # TODO: WOL_SUPPORT
-    # TODO: INTERFACE
-    SensorCommand(
-        "$x = Get-CimInstance Win32_ComputerSystem | "
-        + "Select Name, SystemType;"
-        + "$x.Name;"
-        + "$x.SystemType;",
-        [
-            Sensor(
-                SensorName.HOSTNAME,
-                SensorKey.HOSTNAME,
-            ),
-            Sensor(
-                SensorName.MACHINE_TYPE,
-                SensorKey.MACHINE_TYPE,
-            ),
-        ],
-    ),
-    SensorCommand(
-        "$x = Get-CimInstance Win32_OperatingSystem | "
-        + "Select Caption, Version, OSArchitecture;"
-        + "$x.Caption;"
-        + "$x.Version;"
-        + "$x.OSArchitecture;",
-        [
-            Sensor(
-                SensorName.OS_NAME,
-                SensorKey.OS_NAME,
-            ),
-            Sensor(
-                SensorName.OS_VERSION,
-                SensorKey.OS_VERSION,
-            ),
-            Sensor(
-                SensorName.OS_ARCHITECTURE,
-                SensorKey.OS_ARCHITECTURE,
-            ),
-        ],
-    ),
-    SensorCommand(
-        "$x = Get-CimInstance Win32_ComputerSystem | "
-        + "Select TotalPhysicalMemory;"
-        + "[math]::Round($x.TotalPhysicalMemory/1MB);",
-        [
-            Sensor(
-                SensorName.TOTAL_MEMORY,
-                SensorKey.TOTAL_MEMORY,
-                value_type=int,
-                value_unit="MB",
-            )
-        ],
-    ),
-    SensorCommand(
-        "$x = Get-CimInstance Win32_OperatingSystem | "
-        + "Select FreePhysicalMemory;"
-        + "[math]::Round($x.FreePhysicalMemory/1KB);",
-        [
-            Sensor(
-                SensorName.FREE_MEMORY,
-                SensorKey.FREE_MEMORY,
-                value_type=int,
-                value_unit="MB",
-            )
-        ],
-        interval=30,
-    ),
-    SensorCommand(
-        "Get-CimInstance Win32_LogicalDisk | "
-        + "Select DeviceID, FreeSpace | ForEach-Object "
-        + '{{$_.DeviceID+"|"+[math]::Round($_.FreeSpace/1MB)}}',
-        [
-            DynamicSensor(
-                SensorName.FREE_DISK_SPACE,
-                SensorKey.FREE_DISK_SPACE,
-                value_type=int,
-                value_unit="MB",
-            )
-        ],
-        interval=300,
-        separator="|",
-    ),
-    SensorCommand(
-        "$x = Get-CimInstance Win32_Processor | "
-        + "Select LoadPercentage;"
-        + "$x.LoadPercentage;",
-        [
-            Sensor(
-                SensorName.CPU_LOAD,
-                SensorKey.CPU_LOAD,
-                value_type=int,
-                value_unit="%",
-            )
-        ],
-        interval=30,
-    ),
-    SensorCommand(
-        "$x = Get-CimInstance msacpi_thermalzonetemperature "
-        + '-namespace "root/wmi" | '
-        + "Select CurrentTemperature;"
-        + "($x.CurrentTemperature - 2732) / 10;",
-        [
-            Sensor(
-                SensorName.TEMPERATURE,
-                SensorKey.TEMPERATURE,
-                value_type=int,
-                value_unit="°C",
-            )
-        ],
-        interval=60,
-    ),
-]
+windows_ps = CommandSet(
+    "Windows (Power Shell)",
+    [
+        ServiceCommand(
+            "Stop-Computer -Force",
+            ServiceName.TURN_OFF,
+            ServiceKey.TURN_OFF,
+        ),
+        ServiceCommand(
+            "Restart-Computer -Force",
+            ServiceName.RESTART,
+            ServiceKey.RESTART,
+        ),
+    ],
+    [
+        # TODO: MAC_ADDRESS
+        # TODO: WOL_SUPPORT
+        # TODO: INTERFACE
+        SensorCommand(
+            "$x = Get-CimInstance Win32_ComputerSystem | "
+            + "Select Name, SystemType;"
+            + "$x.Name;"
+            + "$x.SystemType;",
+            [
+                Sensor(
+                    SensorName.HOSTNAME,
+                    SensorKey.HOSTNAME,
+                ),
+                Sensor(
+                    SensorName.MACHINE_TYPE,
+                    SensorKey.MACHINE_TYPE,
+                ),
+            ],
+        ),
+        SensorCommand(
+            "$x = Get-CimInstance Win32_OperatingSystem | "
+            + "Select Caption, Version, OSArchitecture;"
+            + "$x.Caption;"
+            + "$x.Version;"
+            + "$x.OSArchitecture;",
+            [
+                Sensor(
+                    SensorName.OS_NAME,
+                    SensorKey.OS_NAME,
+                ),
+                Sensor(
+                    SensorName.OS_VERSION,
+                    SensorKey.OS_VERSION,
+                ),
+                Sensor(
+                    SensorName.OS_ARCHITECTURE,
+                    SensorKey.OS_ARCHITECTURE,
+                ),
+            ],
+        ),
+        SensorCommand(
+            "$x = Get-CimInstance Win32_ComputerSystem | "
+            + "Select TotalPhysicalMemory;"
+            + "[math]::Round($x.TotalPhysicalMemory/1MB);",
+            [
+                Sensor(
+                    SensorName.TOTAL_MEMORY,
+                    SensorKey.TOTAL_MEMORY,
+                    value_type=int,
+                    value_unit="MB",
+                )
+            ],
+        ),
+        SensorCommand(
+            "$x = Get-CimInstance Win32_OperatingSystem | "
+            + "Select FreePhysicalMemory;"
+            + "[math]::Round($x.FreePhysicalMemory/1KB);",
+            [
+                Sensor(
+                    SensorName.FREE_MEMORY,
+                    SensorKey.FREE_MEMORY,
+                    value_type=int,
+                    value_unit="MB",
+                )
+            ],
+            interval=30,
+        ),
+        SensorCommand(
+            "Get-CimInstance Win32_LogicalDisk | "
+            + "Select DeviceID, FreeSpace | ForEach-Object "
+            + '{{$_.DeviceID+"|"+[math]::Round($_.FreeSpace/1MB)}}',
+            [
+                DynamicSensor(
+                    SensorName.FREE_DISK_SPACE,
+                    SensorKey.FREE_DISK_SPACE,
+                    value_type=int,
+                    value_unit="MB",
+                )
+            ],
+            interval=300,
+            separator="|",
+        ),
+        SensorCommand(
+            "$x = Get-CimInstance Win32_Processor | "
+            + "Select LoadPercentage;"
+            + "$x.LoadPercentage;",
+            [
+                Sensor(
+                    SensorName.CPU_LOAD,
+                    SensorKey.CPU_LOAD,
+                    value_type=int,
+                    value_unit="%",
+                )
+            ],
+            interval=30,
+        ),
+        SensorCommand(
+            "$x = Get-CimInstance msacpi_thermalzonetemperature "
+            + '-namespace "root/wmi" | '
+            + "Select CurrentTemperature;"
+            + "($x.CurrentTemperature - 2732) / 10;",
+            [
+                Sensor(
+                    SensorName.TEMPERATURE,
+                    SensorKey.TEMPERATURE,
+                    value_type=int,
+                    value_unit="°C",
+                )
+            ],
+            interval=60,
+        ),
+    ],
+)
```

### Comparing `ssh_remote_control-0.1.1/src/ssh_remote_control/event.py` & `ssh_remote_control-0.1.2/src/ssh_remote_control/event.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,18 +3,23 @@
 
 class Event:
     """The Event class."""
 
     def __init__(self) -> None:
         self._subscribers: list[Callable] = []
 
-    def subscribe(self, subscriber) -> None:
+    def subscribe(self, subscriber) -> Callable:
         """Subscribe."""
         self._subscribers.append(subscriber)
 
+        def callback():
+            self.unsubscribe(subscriber)
+
+        return callback
+
     def unsubscribe(self, subscriber) -> None:
         """Unsubscribe."""
         self._subscribers.remove(subscriber)
 
     def notify(self, *args, **kwargs) -> None:
         """Notify."""
         for subscriber in self._subscribers:
```

### Comparing `ssh_remote_control-0.1.1/src/ssh_remote_control/locker.py` & `ssh_remote_control-0.1.2/src/ssh_remote_control/locker.py`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.1/src/ssh_remote_control/sensor.py` & `ssh_remote_control-0.1.2/src/ssh_remote_control/sensor.py`

 * *Files identical despite different names*

### Comparing `ssh_remote_control-0.1.1/src/ssh_remote_control.egg-info/SOURCES.txt` & `ssh_remote_control-0.1.2/src/ssh_remote_control.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 LICENSE
 README.md
 pyproject.toml
 src/ssh_remote_control/__init__.py
 src/ssh_remote_control/command.py
+src/ssh_remote_control/command_set.py
 src/ssh_remote_control/event.py
 src/ssh_remote_control/helpers.py
 src/ssh_remote_control/locker.py
 src/ssh_remote_control/manager.py
 src/ssh_remote_control/sensor.py
 src/ssh_remote_control.egg-info/PKG-INFO
 src/ssh_remote_control.egg-info/SOURCES.txt
 src/ssh_remote_control.egg-info/dependency_links.txt
 src/ssh_remote_control.egg-info/requires.txt
 src/ssh_remote_control.egg-info/top_level.txt
-src/ssh_remote_control/default_commands/__init__.py
-src/ssh_remote_control/default_commands/const.py
-src/ssh_remote_control/default_commands/linux.py
-src/ssh_remote_control/default_commands/windows_cmd.py
-src/ssh_remote_control/default_commands/windows_ps.py
+src/ssh_remote_control/default_command_sets/__init__.py
+src/ssh_remote_control/default_command_sets/const.py
+src/ssh_remote_control/default_command_sets/linux.py
+src/ssh_remote_control/default_command_sets/windows_cmd.py
+src/ssh_remote_control/default_command_sets/windows_ps.py
```

