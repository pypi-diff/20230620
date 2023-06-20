# Comparing `tmp/dockery-0.2.4.tar.gz` & `tmp/dockery-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dockery-0.2.4.tar", last modified: Sat Jun 17 22:26:01 2023, max compression
+gzip compressed data, was "dockery-0.3.0.tar", last modified: Mon Jun 19 20:37:04 2023, max compression
```

## Comparing `dockery-0.2.4.tar` & `dockery-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1082 2023-06-17 22:25:53.894298 dockery-0.2.4/LICENSE
--rw-r--r--   0        0        0      665 2023-06-17 22:25:53.894298 dockery-0.2.4/README.md
--rw-r--r--   0        0        0      761 2023-06-17 22:26:01.970420 dockery-0.2.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-17 22:25:53.894298 dockery-0.2.4/src/dockery/__init__.py
--rw-r--r--   0        0        0     2489 2023-06-17 22:25:53.894298 dockery-0.2.4/src/dockery/dockery.py
--rw-r--r--   0        0        0     5022 2023-06-17 22:25:53.894298 dockery-0.2.4/src/dockery/gui.py
--rw-r--r--   0        0        0      322 2023-06-17 22:25:53.894298 dockery-0.2.4/src/dockery/style.css
--rw-r--r--   0        0        0      881 2023-06-17 22:25:53.894298 dockery-0.2.4/src/dockery/utils.py
--rw-r--r--   0        0        0     1145 1970-01-01 00:00:00.000000 dockery-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-06-19 20:36:54.647482 dockery-0.3.0/LICENSE
+-rw-r--r--   0        0        0      665 2023-06-19 20:36:54.647482 dockery-0.3.0/README.md
+-rw-r--r--   0        0        0      761 2023-06-19 20:37:04.924008 dockery-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-19 20:36:54.647482 dockery-0.3.0/src/dockery/__init__.py
+-rw-r--r--   0        0        0     2489 2023-06-19 20:36:54.647482 dockery-0.3.0/src/dockery/dockery.py
+-rw-r--r--   0        0        0     5461 2023-06-19 20:36:54.647482 dockery-0.3.0/src/dockery/gui.py
+-rw-r--r--   0        0        0     1884 2023-06-19 20:36:54.647482 dockery-0.3.0/src/dockery/logs.py
+-rw-r--r--   0        0        0      707 2023-06-19 20:36:54.647482 dockery-0.3.0/src/dockery/style.css
+-rw-r--r--   0        0        0      881 2023-06-19 20:36:54.647482 dockery-0.3.0/src/dockery/utils.py
+-rw-r--r--   0        0        0     1145 1970-01-01 00:00:00.000000 dockery-0.3.0/PKG-INFO
```

### Comparing `dockery-0.2.4/LICENSE` & `dockery-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dockery-0.2.4/README.md` & `dockery-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `dockery-0.2.4/pyproject.toml` & `dockery-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dockery"
-version = "0.2.4"
+version = "0.3.0"
 description = "Graphical interface for Docker in your console"
 authors = [
     { name = "Mariano Carrazana", email = "marianocarrazana@gmail.com" },
 ]
 dependencies = [
     "docker>=6.1.3",
     "textual>=0.27.0",
```

### Comparing `dockery-0.2.4/src/dockery/dockery.py` & `dockery-0.3.0/src/dockery/dockery.py`

 * *Files identical despite different names*

### Comparing `dockery-0.2.4/src/dockery/gui.py` & `dockery-0.3.0/src/dockery/gui.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import threading
 from rich.text import TextType
 from textual.app import App, ComposeResult
 from textual.widgets import (
     Footer,
     Header,
     Static,
     Button,
@@ -10,18 +11,19 @@
 from textual.containers import (
     VerticalScroll,
     Horizontal,
     Vertical,
     Container as Group,
 )
 from textual.reactive import reactive
-from docker import DockerClient
+from docker import DockerClient, errors
 from docker.models.containers import Container
 
 from .utils import get_cpu_usage, get_mem_usage
+from .logs import LogsButton
 
 
 class AppGUI(App):
     CSS_PATH = "style.css"
     BINDINGS = [
         ("h", "home", "Home"),
         ("d", "toggle_dark", "Toggle dark mode"),
@@ -33,26 +35,47 @@
         self.docker = docker
         super().__init__(**kargs)
 
     def compose(self) -> ComposeResult:
         yield Header(show_clock=True)
         yield Footer()
         with ContentSwitcher(initial="container-list"):
-            yield VerticalScroll(id="container-list")
+            yield VerticalScroll(ContainersList(self.docker), id="container-list")
             with VerticalScroll(id="container-logs"):
                 yield Static("", id="logs")
 
+    def action_home(self) -> None:
+        self.query_one(ContentSwitcher).current = "container-list"
+
+
+class ContainersList(Static):
+    container_count = reactive(0)
+
+    def __init__(self, docker: DockerClient, **kargs):
+        self.containers = []
+        self.docker = docker
+        super().__init__(**kargs)
+
     def on_mount(self) -> None:
-        cl = self.query_one("#container-list")
-        for c in self.docker.containers.list(all=True):
+        self.get_containers()
+        self.set_interval(2, self.count_timer)
+
+    def count_timer(self) -> None:
+        thread = threading.Thread(target=self.get_containers)
+        thread.start()
+
+    async def watch_container_count(self, count: int) -> None:
+        await self.remove_children()
+        for c in self.containers:
             cw = ContainerWidget(c, self.docker)  # type: ignore
-            cl.mount(cw)
+            self.mount(cw)
 
-    def action_home(self) -> None:
-        self.query_one(ContentSwitcher).current = "container-list"
+    def get_containers(self) -> None:
+        self.containers = self.docker.containers.list(all=True)
+        self.container_count = len(self.containers)
 
 
 class ContainerWidget(Static):
     def __init__(self, container: Container, client: DockerClient, **kargs):
         self.container = container
         self.client = client
         self.container_id = container.id
@@ -69,33 +92,44 @@
             ReactiveString(id="cpu"),
             ReactiveString(id="mem"),
             classes="status-text",
         )
         yield Group(StatusButtons(self.container))
 
     def on_mount(self):
-        self.set_interval(1, self.update_data)
-        # self.set_interval(4, self.update_usage) # TODO: is very slow
+        self.set_interval(1, self.data_timer)
+        self.running = True
+        thread = threading.Thread(target=self.update_usage, daemon=True)
+        thread.start()
+
+    def data_timer(self) -> None:
+        thread = threading.Thread(target=self.update_data, daemon=True)
+        thread.start()
 
     def update_data(self) -> None:
-        c: Container = self.client.containers.get(self.container_id)  # type: ignore
-        self.container = c
-        self.query_one("#status", ReactiveString).value = c.status.capitalize()
+        try:
+            c: Container = self.client.containers.get(self.container_id)  # type: ignore
+        except errors.NotFound:
+            return None
+        else:
+            self.container = c
+            self.query_one("#status", ReactiveString).value = c.status.capitalize()
 
-    async def update_usage(self) -> None:
+    def update_usage(self) -> None:
         c = self.container
         cpu = self.query_one("#cpu", ReactiveString)
         mem = self.query_one("#mem", ReactiveString)
-        if c.status == "running":
-            stats = c.stats(decode=None, stream=False)  # slow af
-            cpu.value = f"CPU: {get_cpu_usage(stats):.1f}"
-            mem.value = f"MEM: {get_mem_usage(stats):.1f}"
-        else:
-            cpu.value = "CPU: -"
-            mem.value = "MEM: -"
+        for stat in c.stats(stream=True, decode=True):
+            if not self.running:  # finish the thread
+                return None
+            cpu.value = f"CPU: {get_cpu_usage(stat):.1f}"
+            mem.value = f"MEM: {get_mem_usage(stat):.1f}"
+
+    def on_unmount(self):
+        self.running = False
 
 
 class ReactiveString(Static):
     value = reactive("")
 
     def render(self) -> str:
         return self.value
@@ -148,26 +182,7 @@
         self.container.restart()
 
     def on_mount(self) -> None:
         self.variant = "warning"
 
     def render(self) -> TextType:
         return "Restart"
-
-
-class LogsButton(Button):
-    def __init__(self, container: Container, **kargs):
-        self.container = container
-        super().__init__(**kargs)
-
-    def on_click(self) -> None:
-        logs: bytes = self.container.logs(tail=20)
-        cl = self.app.query_one("#logs")
-        lw = Static(logs.decode())
-        cl.mount(lw)
-        self.app.query_one(ContentSwitcher).current = "container-logs"
-
-    def on_mount(self) -> None:
-        self.variant = "primary"
-
-    def render(self) -> TextType:
-        return "Logs"
```

### Comparing `dockery-0.2.4/src/dockery/utils.py` & `dockery-0.3.0/src/dockery/utils.py`

 * *Files identical despite different names*

### Comparing `dockery-0.2.4/PKG-INFO` & `dockery-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dockery
-Version: 0.2.4
+Version: 0.3.0
 Summary: Graphical interface for Docker in your console
 Author-Email: Mariano Carrazana <marianocarrazana@gmail.com>
 License: MIT
 Project-URL: Bug tracker, https://github.com/marianocarrazana/dockery/issues
 Project-URL: Source code, https://github.com/marianocarrazana/dockery
 Requires-Python: >=3.9
 Requires-Dist: docker>=6.1.3
```

