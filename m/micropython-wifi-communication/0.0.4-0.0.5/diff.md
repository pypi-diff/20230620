# Comparing `tmp/micropython_wifi_communication-0.0.4.tar.gz` & `tmp/micropython_wifi_communication-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython_wifi_communication-0.0.4.tar", last modified: Fri Jun 16 17:39:49 2023, max compression
+gzip compressed data, was "micropython_wifi_communication-0.0.5.tar", last modified: Tue Jun 20 21:23:55 2023, max compression
```

## Comparing `micropython_wifi_communication-0.0.4.tar` & `micropython_wifi_communication-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 17:39:49.366750 micropython_wifi_communication-0.0.4/
--rw-rw-rw-   0        0        0     1078 2023-06-16 00:27:57.000000 micropython_wifi_communication-0.0.4/LICENCE
--rw-rw-rw-   0        0        0      409 2023-06-16 17:39:49.366750 micropython_wifi_communication-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       26 2023-06-16 00:29:04.000000 micropython_wifi_communication-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 17:39:49.352436 micropython_wifi_communication-0.0.4/comu/
--rw-rw-rw-   0        0        0       71 2023-06-16 17:37:27.000000 micropython_wifi_communication-0.0.4/comu/__init__.py
--rw-rw-rw-   0        0        0     2150 2023-06-16 17:18:47.000000 micropython_wifi_communication-0.0.4/comu/cli.py
--rw-rw-rw-   0        0        0     2713 2023-06-16 17:20:02.000000 micropython_wifi_communication-0.0.4/comu/ser.py
--rw-rw-rw-   0        0        0      386 2023-06-15 18:40:47.000000 micropython_wifi_communication-0.0.4/comu/util.py
-drwxrwxrwx   0        0        0        0 2023-06-16 17:39:49.364535 micropython_wifi_communication-0.0.4/micropython_wifi_communication.egg-info/
--rw-rw-rw-   0        0        0      409 2023-06-16 17:39:49.000000 micropython_wifi_communication-0.0.4/micropython_wifi_communication.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-06-16 17:39:49.000000 micropython_wifi_communication-0.0.4/micropython_wifi_communication.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 17:39:49.000000 micropython_wifi_communication-0.0.4/micropython_wifi_communication.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-06-16 17:39:49.000000 micropython_wifi_communication-0.0.4/micropython_wifi_communication.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 17:39:49.368392 micropython_wifi_communication-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      510 2023-06-16 17:39:27.000000 micropython_wifi_communication-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 21:23:55.740391 micropython_wifi_communication-0.0.5/
+-rw-rw-rw-   0        0        0     1078 2023-06-16 00:27:57.000000 micropython_wifi_communication-0.0.5/LICENCE
+-rw-rw-rw-   0        0        0      409 2023-06-20 21:23:55.740391 micropython_wifi_communication-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       26 2023-06-16 00:29:04.000000 micropython_wifi_communication-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 21:23:55.727124 micropython_wifi_communication-0.0.5/comu/
+-rw-rw-rw-   0        0        0       71 2023-06-16 17:37:27.000000 micropython_wifi_communication-0.0.5/comu/__init__.py
+-rw-rw-rw-   0        0        0     2609 2023-06-20 21:22:54.000000 micropython_wifi_communication-0.0.5/comu/cli.py
+-rw-rw-rw-   0        0        0     2694 2023-06-20 21:22:54.000000 micropython_wifi_communication-0.0.5/comu/ser.py
+-rw-rw-rw-   0        0        0      386 2023-06-15 18:40:47.000000 micropython_wifi_communication-0.0.5/comu/util.py
+drwxrwxrwx   0        0        0        0 2023-06-20 21:23:55.738958 micropython_wifi_communication-0.0.5/micropython_wifi_communication.egg-info/
+-rw-rw-rw-   0        0        0      409 2023-06-20 21:23:54.000000 micropython_wifi_communication-0.0.5/micropython_wifi_communication.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-06-20 21:23:54.000000 micropython_wifi_communication-0.0.5/micropython_wifi_communication.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 21:23:54.000000 micropython_wifi_communication-0.0.5/micropython_wifi_communication.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-20 21:23:54.000000 micropython_wifi_communication-0.0.5/micropython_wifi_communication.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 21:23:55.740391 micropython_wifi_communication-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      510 2023-06-20 21:23:14.000000 micropython_wifi_communication-0.0.5/setup.py
```

### Comparing `micropython_wifi_communication-0.0.4/LICENCE` & `micropython_wifi_communication-0.0.5/LICENCE`

 * *Files identical despite different names*

### Comparing `micropython_wifi_communication-0.0.4/comu/cli.py` & `micropython_wifi_communication-0.0.5/comu/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,33 @@
+import socket
+import network
+from comu.util import validator
+from time import sleep
+
 class ci:
 
     def __init__(self, net=None, Host='50.1', tr=1024):
+        self.net = net
+        self.cone()
+        self.trans = tr
+        self.HOST = '192.168.' + Host  # Endereço IP do servidor
+        self.PORT = 1234  # Porta para comunicação
 
+        # Cria o socket TCP/IP
+        self.client_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        self.client_socket.settimeout(None)
+        # Conecta-se ao servidor
+        self.client_socket.connect((self.HOST, self.PORT))
+        self.client_socket.settimeout(300)
+
+    def cone(self):
+        net = self.net
         if net:
             if type(net) != dict:
                 net = {}
-            import network
             sta_if = network.WLAN(network.STA_IF)
             if not sta_if.isconnected():
                 print('Conectando-se à rede Wi-Fi...')
                 sta_if.active(True)
                 ssid = ''
                 if 'ssid' in net:
                     ssid = net['ssid']
@@ -19,48 +37,43 @@
                 if password != '':
                     sta_if.connect(ssid, password)
                 else:
                     sta_if.connect(ssid)
                 while not sta_if.isconnected():
                     pass
 
-
-        import socket
-        self.trans = tr
-        self.HOST = '192.168.' + Host  # Endereço IP do servidor
-        self.PORT = 1234  # Porta para comunicação
-
-        # Cria o socket TCP/IP
-        self.client_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        self.client_socket.settimeout(None)
-        # Conecta-se ao servidor
-        self.client_socket.connect((self.HOST, self.PORT))
-        self.client_socket.settimeout(300)
-
     def send(self, data):
         try:
             self.client_socket.settimeout(5)
             message = str({1: 1, 'inf': data, 0: 0})
             self.client_socket.send(message.encode())
             self.client_socket.settimeout(None)
         except:
             self.ence()
 
     def recv(self):
-        from util import validator
         try:
             message = self.client_socket.recv(self.trans).decode()
             if not message:
                 self.ence()
             self.client_socket.settimeout(None)
             va, me = validator(message)
             if not va:
                 return me['inf']
         except:
             self.ence()
 
     def ence(self):
-        try:
-            self.client_socket.connect((self.HOST, self.PORT))
-            self.client_socket.settimeout(300)
-        except:
-            self.ence()
+        x = None
+        self.client_socket.close()
+        while not x:
+            try:
+                wlan = network.WLAN(network.STA_IF)
+                if not wlan.isconnected():
+                    self.cone()
+                self.client_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+                self.client_socket.connect((self.HOST, self.PORT))
+                self.client_socket.settimeout(300)
+                x = True
+            except Exception as e:
+                pass
+            sleep(1)
```

### Comparing `micropython_wifi_communication-0.0.4/comu/ser.py` & `micropython_wifi_communication-0.0.5/comu/ser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+import socket
+import network
+from comu.util import validator
+
+
 class se:
 
     def __init__(self, net=None, Host='50.1', tr=1024):
         self.trans = tr
-        import socket
         self.HOST = '192.168.' + Host  # Endereço IP do servidor
         self.PORT = 1234  # self.PORTa para comunicação
         if net:
             if type(net) != dict:
                 net = {}
-            import network
             SSID = 'MinhaRedeWiFI'  # Nome da rede Wi-Fi
             if 'SSID' in net:
                 SSID = net['SSID']
             PASSWORD = 'MinhaSenha123'  # Senha da rede Wi-Fi
             if 'PASSWORD' in net:
                 PASSWORD = net['PASSWORD']
 
@@ -50,15 +53,14 @@
             message = str({1: 1, 'inf': data, 0: 0})
             self.client_socket.send(message.encode())
             self.client_socket.settimeout(None)
         except:
             self.ence()
 
     def recv(self):
-        from util import validator
         try:
             message = self.client_socket.recv(self.trans).decode()
             if not message:
                 self.ence()
             self.client_socket.settimeout(None)
             va, me = validator(message)
             if not va:
```

