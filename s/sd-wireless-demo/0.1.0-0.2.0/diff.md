# Comparing `tmp/sd_wireless_demo-0.1.0.tar.gz` & `tmp/sd_wireless_demo-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sd_wireless_demo-0.1.0.tar", max compression
+gzip compressed data, was "sd_wireless_demo-0.2.0.tar", max compression
```

## Comparing `sd_wireless_demo-0.1.0.tar` & `sd_wireless_demo-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1068 2023-05-08 18:41:18.419483 sd_wireless_demo-0.1.0/LICENSE
--rw-r--r--   0        0        0       77 2023-05-08 18:41:18.419483 sd_wireless_demo-0.1.0/README.md
--rw-r--r--   0        0        0     1090 2023-05-08 18:41:18.423483 sd_wireless_demo-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-08 18:41:18.423483 sd_wireless_demo-0.1.0/wireless_demo/__init__.py
--rw-r--r--   0        0        0    13792 2023-05-08 18:41:18.427483 sd_wireless_demo-0.1.0/wireless_demo/controls.py
--rw-r--r--   0        0        0     2004 2023-05-08 18:41:18.427483 sd_wireless_demo-0.1.0/wireless_demo/demo_sd_sdk.py
--rw-r--r--   0        0        0     2527 2023-05-08 18:41:18.427483 sd_wireless_demo-0.1.0/wireless_demo/demo_ui.css
--rw-r--r--   0        0        0    10162 2023-05-08 18:41:18.427483 sd_wireless_demo-0.1.0/wireless_demo/demo_ui.py
--rw-r--r--   0        0        0     1835 2023-05-08 18:41:18.427483 sd_wireless_demo-0.1.0/wireless_demo/main.py
--rw-r--r--   0        0        0     1313 1970-01-01 00:00:00.000000 sd_wireless_demo-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-20 16:35:40.830919 sd_wireless_demo-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1942 2023-06-20 16:35:40.830919 sd_wireless_demo-0.2.0/README.md
+-rw-r--r--   0        0        0     1090 2023-06-20 16:35:40.834919 sd_wireless_demo-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-20 16:35:40.834919 sd_wireless_demo-0.2.0/wireless_demo/__init__.py
+-rw-r--r--   0        0        0    14887 2023-06-20 16:35:40.834919 sd_wireless_demo-0.2.0/wireless_demo/controls.py
+-rw-r--r--   0        0        0     2576 2023-06-20 16:35:40.834919 sd_wireless_demo-0.2.0/wireless_demo/demo_sd_sdk.py
+-rw-r--r--   0        0        0     2761 2023-06-20 16:35:40.834919 sd_wireless_demo-0.2.0/wireless_demo/demo_ui.css
+-rw-r--r--   0        0        0    10088 2023-06-20 16:35:40.834919 sd_wireless_demo-0.2.0/wireless_demo/demo_ui.py
+-rw-r--r--   0        0        0     2104 2023-06-20 16:35:40.834919 sd_wireless_demo-0.2.0/wireless_demo/main.py
+-rw-r--r--   0        0        0     3178 1970-01-01 00:00:00.000000 sd_wireless_demo-0.2.0/PKG-INFO
```

### Comparing `sd_wireless_demo-0.1.0/LICENSE` & `sd_wireless_demo-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sd_wireless_demo-0.1.0/pyproject.toml` & `sd_wireless_demo-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sd-wireless-demo"
-version = "0.1.0"
+version = "0.2.0"
 description = "Wireless demo using the Sound Designer SDK on Windows"
 authors = ["Mark Melvin <mark.melvin@onsemi.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
@@ -24,14 +24,14 @@
 ]
 
 [tool.poetry.scripts]
 wireless_demo = "wireless_demo.main:run"
 
 [tool.poetry.dependencies]
 python = "^3.7"
-sd-sdk-python = ">=0.2.0"
+sd-sdk-python = ">=0.2.5"
 #sd-sdk-python = {path="../sd-sdk-python", develop=true}
-textual = {extras = ["dev"], version = "^0.24.0"}
+textual = {extras = ["dev"], version = "^0.27.0"}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `sd_wireless_demo-0.1.0/wireless_demo/controls.py` & `sd_wireless_demo-0.2.0/wireless_demo/controls.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 
 from __future__ import annotations
 
-from rich.progress import Progress, BarColumn, TextColumn, TaskProgressColumn
 from textual.widget import Widget
-from textual.widgets import Static, Label, LoadingIndicator
+from textual.widgets import Static, Label, LoadingIndicator, ProgressBar
 from textual.reactive import reactive
 from textual import events, on
 from textual.message import Message
 from textual.app import ComposeResult
-from textual.containers import Horizontal, Container
+from textual.containers import Horizontal, Vertical, Container
 
 from rich.pretty import Pretty
 
 import asyncio
 import functools
 
 
@@ -33,19 +32,14 @@
     def on_mount(self) -> None:
         self.set_timer(3, self.remove)
 
     def on_click(self) -> None:
         self.remove()
 
 
-class TooltipEvent(Message):
-    def __init__(self, tooltip: str) -> None:
-        self.tooltip = tooltip
-        super().__init__()
-
 class HasDevice(Static):
     def __init__(self, connected_device, content="", **kwargs):
         super().__init__(content, **kwargs)
         self.device = connected_device
 
 
 class Toggle(Static):
@@ -57,14 +51,22 @@
 
 class DeviceInformation(HasDevice):
     collapsed = reactive(False)
 
     def compose(self,) -> ComposeResult:
         yield Toggle()
         yield Static(Pretty(self.device.device_info.to_dict()))
+        yield Static("[bold underline]Device Information Service (DIS)[/]")
+        dis = {
+            "Manufacturer Name" : self.device.wireless_control.ManufacturerName,
+            "Model Number" : self.device.wireless_control.ModelNumber,
+            "Serial Number" : self.device.wireless_control.SerialNumber,
+            "Hardware Revision" : self.device.wireless_control.HardwareRevision,
+        }
+        yield Static(Pretty(dis))
 
     def on_mount(self,) -> None:
         self.query_one(Toggle).collapsed = True
         self.add_class("collapsed")
 
     def on_click(self,) -> None:
         collapsed = self.query_one(Toggle).collapsed
@@ -74,162 +76,137 @@
         else:
             self.add_class("collapsed")
             self.query_one(Toggle).collapsed = True
 
 class BatteryIndicator(HasDevice):
     level = reactive(0)
 
+    def compose(self) -> ComposeResult:
+        with Horizontal(classes="level-indicator"):
+            yield Label("       :battery:")
+            yield ProgressBar(total=100, show_eta=False)
+
     def on_mount(self) -> None:
-        self.rich_progress = Progress(
-                                        TextColumn("[progress.description]:battery:"),
-                                        BarColumn(),
-                                        TaskProgressColumn(),
-                                        auto_refresh=False,
-                                     )
-        self.rich_task = self.rich_progress.add_task("level", total=100)
         self.level = self.device.wireless_control.BatteryLevel
-        self.update(self.rich_progress)
 
     def watch_level(self, new_level: int):
-        self.rich_progress.update(self.rich_task, completed=new_level, refresh=True)
+        self.query_one(ProgressBar).progress = new_level
 
 class VolumeControl(HasDevice):
     volume = reactive(0)
 
+    def compose(self) -> ComposeResult:
+        with Horizontal(classes="level-indicator"):
+            yield Label("Volume   ")
+            yield ProgressBar(total=100, show_eta=False)
+
     def on_mount(self) -> None:
-        self.rich_progress = Progress(
-                                        TextColumn("[progress.description]Volume"),
-                                        BarColumn(),
-                                        TaskProgressColumn(),
-                                        auto_refresh=False,
-                                     )
-        self.rich_task = self.rich_progress.add_task("volume", total=100)
         self.volume = self.device.wireless_control.Volume
-        self.update(self.rich_progress)
+        # Workaround for bug in Tooltips on compound widgets
+        for part in self.query_one(ProgressBar).query("*"):
+            part.tooltip = "Left-click: Volume Down\nMiddle-click: Volume 50%\nRight-click: Volume Up"
+        # self.query_one(ProgressBar).tooltip = "Left-click: Volume Down\nMiddle-click: Volume 50%\nRight-click: Volume Up"
 
     def watch_volume(self, new_volume: int):
-        self.rich_progress.update(self.rich_task, completed=new_volume, refresh=True)
+        self.query_one(ProgressBar).progress = new_volume
 
     def on_click(self,  event: events.Click) -> None:
         if event.button == 1:
             self.device.wireless_control.ChangeVolume(False)
         elif event.button == 2:
             self.device.wireless_control.Volume = 50
         elif event.button == 3:
             self.device.wireless_control.ChangeVolume(True)
 
-    def on_enter(self, event: events.Enter):
-        self.post_message(TooltipEvent("Left-click: Volume Down, Middle-click: Volume 50%, Right-click: Volume Up"))
-
-    def on_leave(self, event: events.Leave):
-        self.post_message(TooltipEvent(""))
-
 
 class MicAttenuation(HasDevice):
     atten = reactive(0)
 
+    def compose(self) -> ComposeResult:
+        with Horizontal(classes="level-indicator"):
+            yield Label("Mic Level")
+            yield ProgressBar(total=100, show_eta=False)
+
     def on_mount(self) -> None:
-        self.rich_progress = Progress(
-                                        TextColumn("[progress.description]Mic Level"),
-                                        BarColumn(),
-                                        TaskProgressColumn(),
-                                        auto_refresh=False,
-                                     )
-        self.rich_task = self.rich_progress.add_task("atten", total=100)
         self.atten = self.device.wireless_control.MicAttenuation
-        self.update(self.rich_progress)
+        # Workaround for bug in Tooltips on compound widgets
+        for part in self.query_one(ProgressBar).query("*"):
+            part.tooltip = "Left-click: -5%\nMiddle-click: 50%\nRight-click: +5%"
+        # self.query_one(ProgressBar).tooltip = "Left-click: -5%\nMiddle-click: 50%\nRight-click: +5%"
 
     def watch_atten(self, new_atten: int):
-        self.rich_progress.update(self.rich_task, completed=new_atten, refresh=True)
+        self.query_one(ProgressBar).progress = new_atten
 
     def on_click(self,  event: events.Click) -> None:
         if event.button == 1:
             self.device.wireless_control.MicAttenuation = max(0, self.atten - 5)
         elif event.button == 2:
             self.device.wireless_control.MicAttenuation = 50
         elif event.button == 3:
             self.device.wireless_control.MicAttenuation = min(100, self.atten + 5)
 
-    def on_enter(self, event: events.Enter):
-        self.post_message(TooltipEvent("Left-click: -5%, Middle-click: 50%, Right-click: +5%"))
-
-    def on_leave(self, event: events.Leave):
-        self.post_message(TooltipEvent(""))
-
 
 class AuxAttenuation(HasDevice):
     atten = reactive(0)
 
+    def compose(self) -> ComposeResult:
+        with Horizontal(classes="level-indicator"):
+            yield Label("Aux Level")
+            yield ProgressBar(total=100, show_eta=False)
+
     def on_mount(self) -> None:
-        self.rich_progress = Progress(
-                                        TextColumn("[progress.description]Aux Level"),
-                                        BarColumn(),
-                                        TaskProgressColumn(),
-                                        auto_refresh=False,
-                                     )
-        self.rich_task = self.rich_progress.add_task("atten", total=100)
         self.atten = self.device.wireless_control.AuxAttenuation
-        self.update(self.rich_progress)
+        # Workaround for bug in Tooltips on compound widgets
+        for part in self.query_one(ProgressBar).query("*"):
+            part.tooltip = "Left-click: -5%\nMiddle-click: 50%\nRight-click: +5%"
+        # self.query_one(ProgressBar).tooltip = "Left-click: -5%\nMiddle-click: 50%\nRight-click: +5%"
 
     def watch_atten(self, new_atten: int):
-        self.rich_progress.update(self.rich_task, completed=new_atten, refresh=True)
+        self.query_one(ProgressBar).progress = new_atten
 
     def on_click(self,  event: events.Click) -> None:
         if event.button == 1:
             self.device.wireless_control.AuxAttenuation = max(0, self.atten - 5)
         elif event.button == 2:
             self.device.wireless_control.AuxAttenuation = 50
         elif event.button == 3:
             self.device.wireless_control.AuxAttenuation = min(100, self.atten + 5)
 
-    def on_enter(self, event: events.Enter):
-        self.post_message(TooltipEvent("Left-click: -5%, Middle-click: 50%, Right-click: +5%"))
-
-    def on_leave(self, event: events.Leave):
-        self.post_message(TooltipEvent(""))
-
 
 class MemoryPanel(HasDevice):
     class MemorySetEvent(Message):
         def __init__(self, memory: int) -> None:
             self.memory = memory
             super().__init__()
 
     def on_click(self, event: events.Click) -> None:
         if event.button == 1:
             self.device.wireless_control.ChangeMemory(False)
         elif event.button == 2:
             memory = int(self.id.split("memoryindicator")[1])
             self.device.wireless_control.CurrentMemory = memory
-            # No notification when memory is manually set? Force a refresh.
-            self.post_message_no_wait(self.MemorySetEvent(self, memory))
         elif event.button == 3:
             self.device.wireless_control.ChangeMemory(True)
 
-    def on_enter(self, event: events.Enter):
-        self.post_message(TooltipEvent("Left-click: Memory Down, Middle-click: Memory Set, Right-click:Memory Up"))
-
-    def on_leave(self, event: events.Leave):
-        self.post_message(TooltipEvent(""))
-
 
 class MemoryControl(HasDevice):
     memory = reactive(0)
     num_memories = 0
 
     def compose(self,) -> ComposeResult:
         memories = []
         self.num_memories = self.device.wireless_control.NumberOfMemories
         for mem in range(self.num_memories):
             s = MemoryPanel(self.device, content=f"{mem}", id=f"memoryindicator{mem}", classes="memoryindicator")
-            if not self.device.wireless_control.MemoryEnabled:
+            if not self.device.wireless_control.MemoryEnabled(mem):
                 s.add_class("disabled")
             memories.append(s)
+            s.tooltip = "Left-click: Memory Down\nMiddle-click: Memory Set\nRight-click:Memory Up"
 
-        yield Static("Current Memory", classes="currentmemory")
+        yield Static("Memory", classes="currentmemory")
         yield Horizontal(*memories)
 
     def on_mount(self) -> None:
         self.memory = self.device.wireless_control.CurrentMemory
 
     def watch_memory(self, new_memory: int):
         for mem in range(self.num_memories):
@@ -239,26 +216,90 @@
                 self.query_one(f"#memoryindicator{mem}").remove_class("current")
 
     def on_memory_panel_memory_set_event(self, event: MemoryPanel.MemorySetEvent) -> None:
         self.memory = self.device.wireless_control.CurrentMemory
         if self.memory != event.memory:
             self.app.logger.info(f"ERROR: Current memory {self.memory} did not match expected {event.memory}!")
 
+
+class ECMemory(Widget):
+    memory = reactive("-1", layout=True)  
+
+    def render(self) -> str:
+        return f"{self.memory}"
+
+
+class ECMemoryControl(HasDevice):
+    ec_memory = reactive(0)
+
+    def compose(self) -> ComposeResult:
+        with Horizontal():
+            yield Label("EC Memory:")
+            yield ECMemory()
+
+    def on_mount(self) -> None:
+        self.ec_memory = self.device.wireless_control.ECMemory
+
+    def watch_ec_memory(self, new_ec_memory: int):
+        self.query_one(ECMemory).memory = new_ec_memory
+
+
+class ProductPanel(HasDevice):
+
+    def compose(self) -> ComposeResult:
+        with Horizontal():
+            yield Label("Product library loaded!")
+
+
+class SDKControlPanel(Widget):
+    ezairo: reactive[object | None] = reactive(None)
+
+    def __init__(self, connected_device) -> None:
+        super().__init__()
+        self.device = connected_device
+
+    def watch_ezairo(self, _old: object, _new: object) -> None:
+        if _new is not None:
+            self.query_one(LoadingWidget).remove()
+            # Change UI to show SDK UI
+            self.mount(ProductPanel(self.ezairo))
+        else:
+            # TODO
+            pass
+
+    def on_mount(self) -> None:
+        if self.app.product_library is not None:
+            self.mount(LoadingWidget(f"Reading device parameters..."))
+            asyncio.create_task(self.sync_with_device())
+        else:
+            self.display = False
+
+    async def sync_with_device(self,) -> None:
+        loop = asyncio.get_running_loop()
+        self.ezairo = await loop.run_in_executor(None,
+                                        functools.partial(self.app.sdk.create_product,
+                                                          self.device.com_adaptor,
+                                                          self.app.product_library))
+
+
+
 class HearingAidWirelessControl(Widget):
-    def __init__(self, connected_device):
+    def __init__(self, connected_device) -> None:
         super().__init__()
         self.device = connected_device
 
     def compose(self) -> ComposeResult:
         yield Container(
             BatteryIndicator(self.device),
             VolumeControl(self.device),
             MicAttenuation(self.device),
             AuxAttenuation(self.device),
             MemoryControl(self.device),
+            ECMemoryControl(self.device),
+            SDKControlPanel(self.device),
             DeviceInformation(self.device),
         )
 
     def on_hearing_aid_control_panel_sdk_event(self, sdk_event: HearingAidControlPanel.SdkEvent) -> None:
         # Based on the event we got, update the child controls
         # self.app.logger.info(f"Got event type {sdk_event.event_type} with data {sdk_event.event_data}")
         if sdk_event.event_type == sd.kBatteryEvent:
@@ -267,14 +308,16 @@
             self.query_one(VolumeControl).volume = int(sdk_event.event_data["VolumeLevel"])
         elif sdk_event.event_type == sd.kMicAttenuationEvent:
             self.query_one(MicAttenuation).atten = int(sdk_event.event_data["MicLevel"])
         elif sdk_event.event_type == sd.kAuxAttenuationEvent:
             self.query_one(AuxAttenuation).atten = int(sdk_event.event_data["AuxLevel"])
         elif sdk_event.event_type == sd.kMemoryEvent:
             self.query_one(MemoryControl).memory = int(sdk_event.event_data["CurrentMemory"])
+        elif sdk_event.event_type == sd.kECMemoryEvent:
+            self.query_one(ECMemoryControl).ec_memory = int(sdk_event.event_data["ECMemory"])
         else:
             self.app.logger.info(f"Got event type {sdk_event.event_type} with data {sdk_event.event_data}")
         # Avoid event bubbling back up to parent widget
         sdk_event.stop(True)
 
 
 class HearingAidControlPanel(Widget):
@@ -301,15 +344,15 @@
 
         elif _new is None:
             if self.connected_device:
                 self.connected_device.close()
                 self.connected_device = None
             self.display = False
 
-    def watch_connected_device(self, _old: dict, _new: dict) -> None:
+    def watch_connected_device(self, _old: object, _new: object) -> None:
         if _new is not None:
             self.app.logger.info(f"Connected: ({self.device_info})")
             self.query_one(LoadingWidget).remove()
             self.connected_device.on_event = self.on_sdk_event
             # Change UI to show wireless control panel
             self.mount(HearingAidWirelessControl(self.connected_device))
         else:
@@ -344,13 +387,11 @@
 
     def disconnect_device(self,):
         self.device_info = None
 
 
 class HearingAidControlPanels(Widget):
     def compose(self) -> ComposeResult:
-        yield Container(
-            Horizontal (
-                HearingAidControlPanel(id="deviceleft"),
-                HearingAidControlPanel(id="deviceright"),
-            ),
-        )
+        with Container():
+            with Horizontal ():
+                yield HearingAidControlPanel(id="deviceleft")
+                yield HearingAidControlPanel(id="deviceright")
```

### Comparing `sd_wireless_demo-0.1.0/wireless_demo/demo_ui.css` & `sd_wireless_demo-0.2.0/wireless_demo/demo_ui.css`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
  *  {
     transition: background 500ms in_out_cubic, color 500ms in_out_cubic;
 }
 
 Screen {
-    layers: base overlay notes notifications;
+    layers: base overlay notifications;
     overflow: hidden;  
 }
 
 Notification {
     dock: bottom;
     layer: notification;
     width: auto;
@@ -19,41 +19,52 @@
     
 }
 
 Body {
     height: 100%;
     overflow-y: scroll;
     width: 100%;
-    background: $surface;    
+    background: $surface;
+
+}
+
+Tooltip {
+    background: $primary;
+    color: auto 90%;
+}
 
+Center {
+    margin-top: 1;
+    margin-bottom: 1;
+    layout: horizontal;
+}
+
+ProgressBar {
+    padding-left: 3;
 }
 
 Screen > Container {
     height: 100%;
     overflow: hidden;
 }
 
 #consolelog {
     background: $surface;
     color: $text;
     height: 30vh;
     dock: bottom;
-    layer: notes;
+    layer: overlay;
     border-top: hkey $primary;
     offset-y: 0;
     transition: offset 400ms in_out_cubic;
     padding: 0 1 1 1;
 }
 
-#consolelog:focus {
-    offset: 0 0 !important;
-}
-
 #consolelog.-hidden {
-    offset-y: 100%;       
+    offset-y: 100%;
 }
 
 TextContent {
     margin: 1 0;
 }
 
 Version {
@@ -64,18 +75,14 @@
 }
 
 ScanResultListView {
     border: white;
     padding: 1;
 }
 
-/* #scanpaneleft {
-    height: 100%;
-} */
-
 .listtitle {
     padding-bottom: 1;
     text-style: bold; 
     color: cyan;
 }
 
 #scanpaneleft {
@@ -128,24 +135,22 @@
 }
 
 HearingAidWirelessControl {
     layout: vertical;
     background: $boost;
 }
 
-BatteryIndicator {
-    width: 100%;
-}
-
-VolumeControl {
+.level-indicator {
     width: 100%;
+    height: 1;
 }
 
 MemoryControl {
-    height: 4;
+    border: round lightseagreen;
+    height: 6;
 }
 
 .currentmemory {
     width: 100%;
     text-align: center;
 }
 
@@ -160,18 +165,29 @@
     text-opacity: 25%;
 }
 
 .memoryindicator.current {
     border: round;
 }
 
+ECMemoryControl {
+    /* padding-top: 1; */
+    /* padding-bottom: 1; */
+    /* background: $panel; */
+    height: 1;
+}
+
+ECMemory {
+    padding-left: 2;
+}
+
 DeviceInformation {
     dock: bottom;
     text-opacity: 25%;
     border: round;
-    height: 20;
+    height: 28;
     transition: height 500ms in_out_cubic;
 }
 
 DeviceInformation.collapsed {
     height: 3;
 }
```

### Comparing `sd_wireless_demo-0.1.0/wireless_demo/demo_ui.py` & `sd_wireless_demo-0.2.0/wireless_demo/demo_ui.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,29 +18,27 @@
     ListItem,
     Button,
 )
 from textual.events import ScreenResume
 from textual.message import Message
 
 from wireless_demo.demo_sd_sdk import SDKHelper, sd
-from wireless_demo.controls import TooltipEvent, HearingAidControlPanels, HearingAidControlPanel
+from wireless_demo.controls import HearingAidControlPanels, HearingAidControlPanel
 
-__version__ = "0.1.0"
+__version__ = "0.2.0"
 
 _title = "Pre Suite Wireless Demo"
 
 
 class Version(Static):
-    tooltip:str = reactive("")
 
     def render(self) -> RenderableType:
-        if self.tooltip is not None and len(self.tooltip):
-            return f"[b]{self.tooltip}"
         return f"[b]v{__version__}"
 
+
 class Body(Container):
     pass
 
 
 class Title(Static):
     pass
 
@@ -68,21 +66,14 @@
 
     def get_integer_mac_addresses(self,):
         mac_str = self.device_id.replace(":", "").replace("-", "")
         mac_addr1 = int(mac_str[0:6], 16)
         mac_addr2 = int(mac_str[6:], 16)
         return (mac_addr1, mac_addr2)
 
-    def on_enter(self, event: events.Enter):
-        part1, part2 = self.get_integer_mac_addresses()
-        self.post_message(TooltipEvent(f"MAC Part 1: {part1}, MAC Part 2: {part2}"))
-
-    def on_leave(self, event: events.Leave):
-        self.post_message(TooltipEvent(""))
-
 
 class ScanResultsListViews(Widget):
     def compose(self) -> ComposeResult:
         yield Container(
             Horizontal (
                 Vertical (
                     Title("Discovered LEFT devices", classes="listtitle"),
@@ -127,14 +118,16 @@
         self.app.logger.debug(f"Got scan event with data: {message.scan_data}")
         try:
             side = message.scan_data.get('ManufacturingData', {}).get('side', None)
             _id = '#scanresultsleft' if side == sd.kLeft else '#scanresultsright'
             new_result = ScanResultDisplay(message.scan_data)
             self.query_one(_id).mount(new_result)
             new_result.scroll_visible()
+            part1, part2 = new_result.get_integer_mac_addresses()
+            new_result.tooltip = f"MAC Part 1: {part1}\nMAC Part 2: {part2}"
         except AttributeError:
             pass
 
     @on(ScreenResume)
     def _start_scanning(self,):
 
         def scan_cb(scan_data):
@@ -165,17 +158,14 @@
         if event.list_view is self.query_one('#scanresultsleft'):
             self.app.left_device = event.item.scan_data
         elif event.list_view is self.query_one('#scanresultsright'):
             self.app.right_device = event.item.scan_data
         devices = [w for w in [self.app.left_device, self.app.right_device] if w is not None]
         self.query_one(SelectedScanItems).total = len(devices)
 
-    def on_tooltip_event(self, event: TooltipEvent) -> None:
-        self.query_one(Version).tooltip = event.tooltip
-
 
 class QuitScreen(Screen):
     def compose(self) -> ComposeResult:
         yield Grid(
             Static("Are you sure you want to quit?", id="question"),
             Button("Quit", variant="error", id="quit"),
             Button("Cancel", variant="primary", id="cancel"),
@@ -239,41 +229,39 @@
         self.query_one('#deviceleft').device_info = self.app.left_device
         self.query_one('#deviceright').device_info = self.app.right_device
 
     def disconnect_all_devices(self,):
         for q in self.query(HearingAidControlPanel):
             q.disconnect_device()
 
-    def on_tooltip_event(self, event: TooltipEvent) -> None:
-        self.query_one(Version).tooltip = event.tooltip
-
 
 from dataclasses import dataclass
 import pathlib
 @dataclass
 class Args:
     """Class emulating command line arguments to allow running via `textual run --dev`"""
     programmer:str
     com_port:str
     delete_bonds:bool
     debug:bool
     noahlink_driver_path:object
+    library_path:object
 
 class DemoApp(App[None]):
     CSS_PATH = "demo_ui.css"
     SCREENS = {"main" : MainScreen(), "scan" : ScanningScreen(), "quit" : QuitScreen()}
 
     def __init__(self, cmdline_args=None, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self.cmdline_args = cmdline_args
 
         # See if we're being run by `textual run --dev`
         if 'devtools' in self.features:
-            # self.cmdline_args = Args('RSL10', 'COM7', False, True, None)
-            self.cmdline_args = Args('NOAHLink', '', False, True, pathlib.Path("c:\\Users\\ffwxyx\\.sounddesigner\\nlw\\"))
+            # self.cmdline_args = Args('RSL10', 'COM7', False, True, None, None)
+            self.cmdline_args = Args('NOAHLink', '', False, True, pathlib.Path("c:\\Users\\ffwxyx\\.sounddesigner\\nlw\\"), pathlib.Path("C:\\_dev\\PreSuite\\SoundDesignerSDK\\products\\E7160SL.library"))
 
         self.logger = logging.getLogger("DemoApp")
         # Avoid all output being sent to the console as well
         self.logger.propagate = False
         self.logger.setLevel(logging.DEBUG if self.cmdline_args.debug else logging.INFO)
         if self.cmdline_args.debug:
             fh = logging.FileHandler('app_debug.log', encoding='utf-8', mode='w')
@@ -285,14 +273,21 @@
         self.right_device = None
 
         self.sdk = SDKHelper(self.cmdline_args.programmer,
                              com_port=self.cmdline_args.com_port,
                              clear_bond_table=self.cmdline_args.delete_bonds,
                              noah_driver_path=self.cmdline_args.noahlink_driver_path)
 
+        self.product_library = None
+        if self.cmdline_args.library_path is not None and \
+                            self.cmdline_args.library_path.exists() and \
+                                                self.cmdline_args.library_path.is_file():
+            self.product_library = self.cmdline_args.library_path
+
+
     def on_mount(self) -> None:
         self.push_screen("main")
 
     def exit(self, result = None) -> None:
         self.push_screen("quit")
 
     def do_exit(self, result = None) -> None:
```

### Comparing `sd_wireless_demo-0.1.0/wireless_demo/main.py` & `sd_wireless_demo-0.2.0/wireless_demo/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,23 +13,29 @@
                         help=f'The type of wireless programmer to use')
     parser.add_argument('--com-port', default='COM3',
                         help='The COM port to use when using the RSL10 dongle')
     parser.add_argument('--debug', action='store_true', default=False,
                         help='Log additional debug information to app_debug.log')
     parser.add_argument('--delete-bonds', action='store_true', default=False,
                         help='Delete the bond table in the wireless programmer')
+    parser.add_argument('--library-path', type=pathlib.Path, default=None,
+                        help='Path to the product library to load and use (optional)')
 
     args = parser.parse_args()
     if args.sdk_root is not None:
         os.environ['SD_SDK_ROOT'] = str(args.sdk_root)
 
     if args.programmer.upper() == 'NOAHLINK':
         assert args.noahlink_driver_path is not None, "Path to the NOAHLink wireless drivers was not set!"
         assert args.noahlink_driver_path.exists() and args.noahlink_driver_path.is_dir(), "Invalid NOAHLink Wireless driver path!"
 
+    # This is not supported yet
+    if args.library_path is not None:
+        raise NotImplementedError()
+
     return args
 
 def run():
     args = parse_command_line_arguments()
 
     # NOTE: We must parse the command line arguments to set SD_SDK_ROOT before
     #       importing the DemoApp
```

