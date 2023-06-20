# Comparing `tmp/selenium_injector-1.1.tar.gz` & `tmp/selenium_injector-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\selenium_injector-1.1.tar", last modified: Sun Apr  9 11:09:41 2023, max compression
+gzip compressed data, was "dist\selenium_injector-2.0.tar", last modified: Tue Jun 20 13:09:52 2023, max compression
```

## Comparing `selenium_injector-1.1.tar` & `selenium_injector-2.0.tar`

### file list

```diff
@@ -1,35 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 11:09:41.000000 selenium_injector-1.1/
--rw-rw-rw-   0        0        0      641 2022-11-24 08:41:11.000000 selenium_injector-1.1/LICENSE.md
--rw-rw-rw-   0        0        0      199 2023-04-06 20:52:34.000000 selenium_injector-1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5556 2023-04-09 11:09:41.000000 selenium_injector-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4245 2023-04-09 11:09:12.000000 selenium_injector-1.1/README.md
--rw-rw-rw-   0        0        0      522 2023-04-06 21:41:47.000000 selenium_injector-1.1/build_upload.md
--rw-rw-rw-   0        0        0      101 2022-11-24 08:05:09.000000 selenium_injector-1.1/pyproject.toml
--rw-rw-rw-   0        0        0      131 2023-04-09 11:09:41.000000 selenium_injector-1.1/setup.cfg
--rw-rw-rw-   0        0        0     1831 2023-04-06 21:42:12.000000 selenium_injector-1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-09 11:09:41.000000 selenium_injector-1.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-09 11:09:41.000000 selenium_injector-1.1/src/selenium_injector/
--rw-rw-rw-   0        0        0       21 2023-04-09 11:08:40.000000 selenium_injector-1.1/src/selenium_injector/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 11:09:41.000000 selenium_injector-1.1/src/selenium_injector/files/
-drwxrwxrwx   0        0        0        0 2023-04-09 11:09:41.000000 selenium_injector-1.1/src/selenium_injector/files/injector_extension/
--rw-rw-rw-   0        0        0     7901 2023-04-09 10:13:44.000000 selenium_injector-1.1/src/selenium_injector/files/injector_extension/background.js
-drwxrwxrwx   0        0        0        0 2023-04-09 11:09:41.000000 selenium_injector-1.1/src/selenium_injector/files/tmp/
-drwxrwxrwx   0        0        0        0 2023-04-09 11:09:41.000000 selenium_injector-1.1/src/selenium_injector/files/tmp/injector_extension/
--rw-rw-rw-   0        0        0     8071 2023-04-09 11:04:53.000000 selenium_injector-1.1/src/selenium_injector/files/tmp/injector_extension/background.js
--rw-rw-rw-   0        0        0        0 2023-04-06 20:20:08.000000 selenium_injector-1.1/src/selenium_injector/files/tmp/injector_extension/content_helper.js
--rw-rw-rw-   0        0        0     2046 2023-04-07 07:59:51.000000 selenium_injector-1.1/src/selenium_injector/files/tmp/injector_extension/manifest.json
--rw-rw-rw-   0        0        0    88326 2023-04-07 07:15:12.000000 selenium_injector-1.1/src/selenium_injector/files/tmp/injector_extension/peg.min.js
--rw-rw-rw-   0        0        0     4765 2023-04-09 10:53:20.000000 selenium_injector-1.1/src/selenium_injector/injector.py
-drwxrwxrwx   0        0        0        0 2023-04-09 11:09:41.000000 selenium_injector-1.1/src/selenium_injector/scripts/
--rw-rw-rw-   0        0        0        0 2022-11-29 13:10:11.000000 selenium_injector-1.1/src/selenium_injector/scripts/__init__.py
--rw-rw-rw-   0        0        0     1305 2023-04-09 10:46:23.000000 selenium_injector-1.1/src/selenium_injector/scripts/socket.py
--rw-rw-rw-   0        0        0     3488 2023-04-09 10:58:34.000000 selenium_injector-1.1/src/selenium_injector/scripts/sync_websocket.py
-drwxrwxrwx   0        0        0        0 2023-04-09 11:09:41.000000 selenium_injector-1.1/src/selenium_injector/utils/
--rw-rw-rw-   0        0        0       19 2022-11-24 10:40:41.000000 selenium_injector-1.1/src/selenium_injector/utils/__init__.py
--rw-rw-rw-   0        0        0     1258 2023-04-07 06:27:15.000000 selenium_injector-1.1/src/selenium_injector/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-09 11:09:41.000000 selenium_injector-1.1/src/selenium_injector.egg-info/
--rw-rw-rw-   0        0        0     5556 2023-04-09 11:09:40.000000 selenium_injector-1.1/src/selenium_injector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      903 2023-04-09 11:09:40.000000 selenium_injector-1.1/src/selenium_injector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 11:09:40.000000 selenium_injector-1.1/src/selenium_injector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-04-09 11:09:40.000000 selenium_injector-1.1/src/selenium_injector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-09 11:09:40.000000 selenium_injector-1.1/src/selenium_injector.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 13:09:52.000000 selenium_injector-2.0/
+-rw-rw-rw-   0        0        0      641 2022-11-24 08:41:11.000000 selenium_injector-2.0/LICENSE.md
+-rw-rw-rw-   0        0        0      228 2023-06-20 11:58:10.000000 selenium_injector-2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4931 2023-06-20 13:09:52.000000 selenium_injector-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3625 2023-06-20 12:51:01.000000 selenium_injector-2.0/README.md
+-rw-rw-rw-   0        0        0      522 2023-04-06 21:41:47.000000 selenium_injector-2.0/build_upload.md
+-rw-rw-rw-   0        0        0      101 2022-11-24 08:05:09.000000 selenium_injector-2.0/pyproject.toml
+-rw-rw-rw-   0        0        0      131 2023-06-20 13:09:52.000000 selenium_injector-2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1826 2023-06-20 11:40:08.000000 selenium_injector-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 13:09:52.000000 selenium_injector-2.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-20 13:09:52.000000 selenium_injector-2.0/src/selenium_injector/
+-rw-rw-rw-   0        0        0       21 2023-06-20 13:09:46.000000 selenium_injector-2.0/src/selenium_injector/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 13:09:52.000000 selenium_injector-2.0/src/selenium_injector/files/
+drwxrwxrwx   0        0        0        0 2023-06-20 13:09:52.000000 selenium_injector-2.0/src/selenium_injector/files/extension/
+-rw-rw-rw-   0        0        0     3155 2023-06-20 10:48:36.000000 selenium_injector-2.0/src/selenium_injector/files/extension/background.js
+-rw-rw-rw-   0        0        0     1924 2023-06-15 07:20:05.000000 selenium_injector-2.0/src/selenium_injector/files/extension/manifest.json
+drwxrwxrwx   0        0        0        0 2023-06-20 13:09:52.000000 selenium_injector-2.0/src/selenium_injector/files/js/
+-rw-rw-rw-   0        0        0     6031 2023-06-20 13:01:28.000000 selenium_injector-2.0/src/selenium_injector/files/js/connection.js
+-rw-rw-rw-   0        0        0      310 2023-06-20 10:28:07.000000 selenium_injector-2.0/src/selenium_injector/files/js/utils.js
+drwxrwxrwx   0        0        0        0 2023-06-20 13:09:52.000000 selenium_injector-2.0/src/selenium_injector/files/tmp/
+drwxrwxrwx   0        0        0        0 2023-06-20 13:09:52.000000 selenium_injector-2.0/src/selenium_injector/files/tmp/injector_extension/
+-rw-rw-rw-   0        0        0     9312 2023-06-20 13:05:57.000000 selenium_injector-2.0/src/selenium_injector/files/tmp/injector_extension/background.js
+-rw-rw-rw-   0        0        0        0 2023-04-06 20:20:08.000000 selenium_injector-2.0/src/selenium_injector/files/tmp/injector_extension/content_helper.js
+-rw-rw-rw-   0        0        0     1924 2023-06-15 07:20:05.000000 selenium_injector-2.0/src/selenium_injector/files/tmp/injector_extension/manifest.json
+-rw-rw-rw-   0        0        0     6050 2023-06-17 13:56:27.000000 selenium_injector-2.0/src/selenium_injector/injector.py
+drwxrwxrwx   0        0        0        0 2023-06-20 13:09:52.000000 selenium_injector-2.0/src/selenium_injector/scripts/
+-rw-rw-rw-   0        0        0        0 2022-11-29 13:10:11.000000 selenium_injector-2.0/src/selenium_injector/scripts/__init__.py
+-rw-rw-rw-   0        0        0     6295 2023-06-20 11:35:20.000000 selenium_injector-2.0/src/selenium_injector/scripts/driverless.py
+-rw-rw-rw-   0        0        0     1576 2023-06-20 10:58:22.000000 selenium_injector-2.0/src/selenium_injector/scripts/js.py
+-rw-rw-rw-   0        0        0     1742 2023-06-20 11:34:48.000000 selenium_injector-2.0/src/selenium_injector/scripts/socket.py
+-rw-rw-rw-   0        0        0     3804 2023-06-20 12:49:54.000000 selenium_injector-2.0/src/selenium_injector/scripts/sync_websocket.py
+drwxrwxrwx   0        0        0        0 2023-06-20 13:09:52.000000 selenium_injector-2.0/src/selenium_injector/utils/
+-rw-rw-rw-   0        0        0       19 2022-11-24 10:40:41.000000 selenium_injector-2.0/src/selenium_injector/utils/__init__.py
+-rw-rw-rw-   0        0        0     1584 2023-06-20 11:35:20.000000 selenium_injector-2.0/src/selenium_injector/utils/utils.py
+-rw-rw-rw-   0        0        0     1841 2023-06-20 13:00:41.000000 selenium_injector-2.0/src/selenium_injector/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-06-20 13:09:52.000000 selenium_injector-2.0/src/selenium_injector.egg-info/
+-rw-rw-rw-   0        0        0     4931 2023-06-20 13:09:52.000000 selenium_injector-2.0/src/selenium_injector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1084 2023-06-20 13:09:52.000000 selenium_injector-2.0/src/selenium_injector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 13:09:52.000000 selenium_injector-2.0/src/selenium_injector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-06-20 13:09:52.000000 selenium_injector-2.0/src/selenium_injector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-20 13:09:52.000000 selenium_injector-2.0/src/selenium_injector.egg-info/top_level.txt
```

### Comparing `selenium_injector-1.1/LICENSE.md` & `selenium_injector-2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `selenium_injector-1.1/build_upload.md` & `selenium_injector-2.0/build_upload.md`

 * *Files identical despite different names*

### Comparing `selenium_injector-1.1/setup.py` & `selenium_injector-2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='selenium_injector',
     author='Aurin Aegerter',
     author_email='aurinliun@gmx.ch',
-    description='Remote controll a chrome extension',
+    description='inject javascript into chrome',
     keywords='Selenium,interception, proxy, webautomation',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kaliiiiiiiiii/Selenium-Injector',
     project_urls={
         'Documentation': 'https://github.com/kaliiiiiiiiii/Selenium-Injector',
         'Bug Reports':
```

### Comparing `selenium_injector-1.1/src/selenium_injector/files/tmp/injector_extension/manifest.json` & `selenium_injector-2.0/src/selenium_injector/files/extension/manifest.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {'delete': "['web_accessible_resources']"}*

```diff
@@ -79,19 +79,9 @@
         "vpnProvider",
         "wallpaper",
         "webNavigation",
         "webRequest",
         "webRequestBlocking",
         "webRequestAuthProvider"
     ],
-    "version": "1.0",
-    "web_accessible_resources": [
-        {
-            "matches": [
-                "<all_urls>"
-            ],
-            "resources": [
-                "peg.min.js"
-            ]
-        }
-    ]
+    "version": "1.0"
 }
```

### Comparing `selenium_injector-1.1/src/selenium_injector/injector.py` & `selenium_injector-2.0/src/selenium_injector/scripts/driverless.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,71 @@
-class base_injector:
+class base_driver:
     def __init__(self, socket, user: str):
         self.socket = socket
         self.user = user
 
     def check_cmd(self, value, values):
         if value not in values:
             raise ValueError("Expected " + str(values) + " , but got" + str(value))
 
 
-class mv3_injector:
-    def __init__(self, port: int = 8001, host: str = "localhost", user="selenium-injector-mv3"):
+class Driverless:
+    def __init__(self, port: int = None, host: str = None, user="selenium-injector-mv3"):
         from selenium_injector.scripts.socket import socket
-        from selenium_injector.utils.utils import read, write, sel_injector_path
+        from selenium_injector.utils.utils import read, write, sel_injector_path, random_port
+
+        if not host:
+            host = "localhost"
+        if not port:
+            port = random_port(host=host)
 
         self.user = user
-        background_js = read("files/injector_extension/background.js")
-        config = """
-        connection.username = "%s";
-        connection.host = "%s";
-        connection.port = %s;
+
+        self.config = f"""
+        var connection = new connector("{host}", {port}, "{self.user}")
         connection.connect();
-        """ % (self.user, host, str(port))
+        """
         self.path = sel_injector_path() + "files/tmp/injector_extension"
-        write(self.path + "/background.js", background_js + config, sel_root=False)
+
+        self.background_js = read("files/extension/background.js")
+        self.connection_js = read("files/js/connection.js")
+        write(self.path + "/background.js", self.background_js + self.connection_js + self.config, sel_root=False)
+
         self.socket = socket()
         self.socket.start(port=port, host=host)
         self.stop = self.socket.stop
         self.exec = self.socket.exec
         self.exec_command = self.socket.exec_command
 
         # subclasses
         self.proxy = self.proxy(socket=self.socket, user=self.user)
         self.webrtc_leak = self.webrtc_leak(socket=self.socket, user=self.user)
         self.contentsettings = self.contentsettings(socket=self.socket, user=self.user)
+        self.tabs = self.tabs(socket=self.socket, user=self.user)
 
-    class proxy(base_injector):
+    @property
+    def page_source(self):
+        return self.socket.exec(self.socket.js.types.path("document.documentElement.outerHTML"), user="tab-0")["result"][0]
+
+    class proxy(base_driver):
         def __init__(self, socket, user):
             self.supported_schemes = ["http", "https", "socks4", "socks5"]
             super().__init__(socket, user=user)
 
+        @property
+        def rules(self):
+            try:
+                return self.socket.exec_command("proxy.get",user=self.user)["result"][0]["value"]["rules"]
+            except KeyError:
+                return None
+
+        @property
+        def mode(self):
+            return self.socket.exec_command("proxy.get",user=self.user)["result"][0]["value"]["mode"]
+
         # noinspection PyDefaultArgument
         def set(self, host: str, port: int, scheme: str = "http", patch_webrtc: bool = True,
                 patch_location: bool = True, bypass_list: list = ["localhost"],
                 username: str = None, password: str = None,
                 timeout=10):
 
             self.check_cmd(scheme, self.supported_schemes)
@@ -59,35 +82,54 @@
         # noinspection PyDefaultArgument
         def set_auth(self, username: str, password: str, urls=["<all_urls>"], timeout=10):
             self.socket.exec_command("proxy.set_auth", [username, password, urls], timeout=timeout, user=self.user)
 
         def clear(self, clear_webrtc=True, clear_location=True, timeout=10):
             self.socket.exec_command("proxy.clear", [clear_webrtc, clear_location], timeout=timeout, user=self.user)
 
-    class webrtc_leak(base_injector):
+    class webrtc_leak(base_driver):
         def __init__(self, socket, user):
             self.supported_values = ["default", "default_public_and_private_interfaces",
                                      "default_public_interface_only", "disable_non_proxied_udp"]
             super().__init__(socket, user)
 
         def disable(self, value="disable_non_proxied_udp", timeout=10):
             self.check_cmd(value, self.supported_values)
             self.socket.exec_command("webrtc_leak.disable", [value], timeout=timeout, user=self.user)
 
         def clear(self, timeout=10):
             self.socket.exec_command("webrtc_leak.clear", timeout=timeout, user=self.user)
 
-    class contentsettings(base_injector):
+    class contentsettings(base_driver):
         def __init__(self, socket, user):
             self.supported_location_settings = ["ask", "allow", "block"]
             self.supported_settings = ["automaticDownloads", "autoVerify", "camera", "cookies", "fullscreen", "images",
                                        "javascript", "location", "microphone", "mouselock", "notifications", "plugins",
                                        "popups", "unsandboxedPlugins"]
             super().__init__(socket, user)
 
         def set(self, setting, value, urls="<all_urls>", timeout=10):
             self.check_cmd(setting, self.supported_settings)
             self.socket.exec_command("contentsettings.set", [setting, value, urls], timeout=timeout, user=self.user)
 
         def set_location(self, setting="ask", urls="<all_urls>", timeout=10):
             self.check_cmd(setting, self.supported_location_settings)
             self.socket.exec_command("contentsettings.set_location", [setting, urls], timeout=timeout, user=self.user)
+
+    class tabs(base_driver):
+        def query(self, query=None):
+            if not query:
+                query = {}
+            return self.socket.exec_async(script={"type": "exec", "func": {"type": "path", "path": "chrome.tabs.query"},
+                                                  "args": [{"type": "val", 'val': query}, self.socket.send_back]
+                                                  }, user=self.user)
+
+        @property
+        def all_tabs(self):
+            return self.query()["result"][0]
+
+        @property
+        def active_tab(self):
+            try:
+                return self.query({"active": True, "lastFocusedWindow": True})["result"][0][0]
+            except IndexError:
+                return None
```

### Comparing `selenium_injector-1.1/src/selenium_injector/scripts/socket.py` & `selenium_injector-2.0/src/selenium_injector/scripts/socket.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,36 @@
 from selenium_injector.scripts.sync_websocket import SynchronousWebsocketServer
+from selenium_injector.scripts.js import JS
 
 
 class socket(SynchronousWebsocketServer):
+    def __init__(self):
+        self.js = JS()
+        self.send_back = self.js.types.send_back()
+        self.not_return = {"not_return":True}
+        super().__init__()
+
     def post(self, message: str, timeout: int = 10, user: str = None):
         user = self.wait_user(user)
         self.send(message=message, user=user)
         return self.recv(user=user, timeout=timeout)
 
     def exec(self, script: dict, user: str = None, timeout: int = 10):
         user = self.wait_user(user=user)
         import json
-        result = json.loads(self.post(json.dumps(script), user=user, timeout=timeout))
+        result = self.post(json.dumps(script), user=user, timeout=timeout)
+        result = json.loads(result)
         if result["status"] == "error":
-            raise Exception(result["result"]["stack"])
+            raise Exception(result["result"][0]["stack"])
         return result
 
+    def exec_async(self, script: dict, user: str = None, timeout: int = 10):
+        script["not_return"] = True
+        return self.exec(script=script, user=user, timeout=timeout)
+
     def exec_command(self, function: str, args: list or str or int or float or bool or None = None, timeout: int = 10,
                      user: str = None):
         user = self.wait_user(user)
         parsed_args = []
         arg_type = type(args)
         if arg_type == list:
             for arg in args:
```

### Comparing `selenium_injector-1.1/src/selenium_injector/scripts/sync_websocket.py` & `selenium_injector-2.0/src/selenium_injector/scripts/sync_websocket.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,24 +30,32 @@
         # noinspection PyUnresolvedReferences
         try:
             async for message in websocket:
                 self.users[user]["rxqueue"].put(message)
         except websockets.exceptions.ConnectionClosedError:
             pass
         finally:
-            del self.users[user]
+            try:
+                del self.users[user]
+            except KeyError:
+                pass
 
     def recv(self, user: str = None, timeout: int = 10):
         import time
         user = self.wait_user(user, timeout=int(timeout/2))
         for i in range(timeout * 5):
             self.process()
-            if not self.users[user]["rxqueue"].empty():
-                return self.users[user]["rxqueue"].get_nowait()
+            try:
+                if not self.users[user]["rxqueue"].empty():
+                    return self.users[user]["rxqueue"].get_nowait()
+            except KeyError:
+                pass # user not connected atm
+            self.wait_user(user, timeout=int(timeout / 2))
             time.sleep(0.1)
+        raise TimeoutError(f"Didn't get a response within {timeout} seconds")
 
     def send(self, message: str, user: str = None, timeout=10):
         user = self.wait_user(user, timeout=timeout)
         self.loop.run_until_complete(self.users[user]["ws"].send(message))
 
     def wait_user(self, user: str = None, timeout: int = 10):
         if timeout is False:
@@ -56,15 +64,15 @@
             import time
             for i in range(timeout * 10):
                 try:
                     return self.get_user(user=user)
                 except LookupError:
                     pass
                 time.sleep(0.1)
-            raise TimeoutError("No users connected")
+            raise TimeoutError("User not connected")
 
     def get_user(self, user=None):
         self.process(nloop=5)
         users = list(self.users.keys())
         if user:
             if user in users:
                 return user
```

### Comparing `selenium_injector-1.1/src/selenium_injector/utils/utils.py` & `selenium_injector-2.0/src/selenium_injector/utils/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import json
 import os
 import selenium_injector
+import socket
+from contextlib import closing
 
 
 def sel_injector_path():
     return os.path.dirname(selenium_injector.__file__) + "/"
 
 
 def read(filename: str, encoding: str = "utf-8", sel_root: bool = True):
@@ -37,7 +39,16 @@
 def write_json(obj: dict or list, filename: str = "out.json", encoding: str = "utf-8", sel_root=True):
     if sel_root:
         path = sel_injector_path() + filename
     else:
         path = filename
     with open(path, "w", encoding=encoding) as outfile:
         outfile.write(json.dumps(obj))
+
+
+def random_port(host: str = None):
+    if not host:
+        host = ''
+    with closing(socket.socket(socket.AF_INET, socket.SOCK_STREAM)) as s:
+        s.bind((host, 0))
+        s.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+        return s.getsockname()[1]
```

### Comparing `selenium_injector-1.1/src/selenium_injector.egg-info/SOURCES.txt` & `selenium_injector-2.0/src/selenium_injector.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -3,22 +3,27 @@
 README.md
 build_upload.md
 pyproject.toml
 setup.cfg
 setup.py
 src/selenium_injector/__init__.py
 src/selenium_injector/injector.py
+src/selenium_injector/webdriver.py
 src/selenium_injector.egg-info/PKG-INFO
 src/selenium_injector.egg-info/SOURCES.txt
 src/selenium_injector.egg-info/dependency_links.txt
 src/selenium_injector.egg-info/requires.txt
 src/selenium_injector.egg-info/top_level.txt
-src/selenium_injector/files/injector_extension/background.js
+src/selenium_injector/files/extension/background.js
+src/selenium_injector/files/extension/manifest.json
+src/selenium_injector/files/js/connection.js
+src/selenium_injector/files/js/utils.js
 src/selenium_injector/files/tmp/injector_extension/background.js
 src/selenium_injector/files/tmp/injector_extension/content_helper.js
 src/selenium_injector/files/tmp/injector_extension/manifest.json
-src/selenium_injector/files/tmp/injector_extension/peg.min.js
 src/selenium_injector/scripts/__init__.py
+src/selenium_injector/scripts/driverless.py
+src/selenium_injector/scripts/js.py
 src/selenium_injector/scripts/socket.py
 src/selenium_injector/scripts/sync_websocket.py
 src/selenium_injector/utils/__init__.py
 src/selenium_injector/utils/utils.py
```

