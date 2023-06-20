# Comparing `tmp/trevorproxy-1.0.4.tar.gz` & `tmp/trevorproxy-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trevorproxy-1.0.4.tar", max compression
+gzip compressed data, was "trevorproxy-1.0.5.tar", max compression
```

## Comparing `trevorproxy-1.0.4.tar` & `trevorproxy-1.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    35248 2021-11-18 17:41:15.210437 trevorproxy-1.0.4/LICENSE
--rw-r--r--   0        0        0      558 2022-02-03 21:56:41.481079 trevorproxy-1.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2021-12-06 20:03:02.221019 trevorproxy-1.0.4/trevorproxy/__init__.py
--rwxr-xr-x   0        0        0     5244 2021-12-08 21:11:37.029037 trevorproxy-1.0.4/trevorproxy/cli.py
--rw-r--r--   0        0        0     4381 2021-11-17 21:40:20.027757 trevorproxy-1.0.4/trevorproxy/lib/__pycache__/cyclic.cpython-39.pyc
--rw-r--r--   0        0        0      588 2021-11-17 16:48:42.200348 trevorproxy-1.0.4/trevorproxy/lib/__pycache__/errors.cpython-39.pyc
--rw-r--r--   0        0        0     1792 2021-11-17 16:52:06.707023 trevorproxy-1.0.4/trevorproxy/lib/__pycache__/interface.cpython-39.pyc
--rw-r--r--   0        0        0      670 2021-11-16 20:42:09.080903 trevorproxy-1.0.4/trevorproxy/lib/__pycache__/logger.cpython-39.pyc
--rw-r--r--   0        0        0     5210 2022-01-06 17:04:42.222402 trevorproxy-1.0.4/trevorproxy/lib/__pycache__/socks.cpython-39.pyc
--rw-r--r--   0        0        0     7132 2022-01-13 19:59:00.947386 trevorproxy-1.0.4/trevorproxy/lib/__pycache__/ssh.cpython-39.pyc
--rw-r--r--   0        0        0     1776 2021-11-22 17:12:58.287137 trevorproxy-1.0.4/trevorproxy/lib/__pycache__/subnet.cpython-39.pyc
--rw-r--r--   0        0        0     4808 2022-01-13 20:09:35.324079 trevorproxy-1.0.4/trevorproxy/lib/__pycache__/util.cpython-39.pyc
--rw-r--r--   0        0        0     5591 2021-11-17 21:40:17.771090 trevorproxy-1.0.4/trevorproxy/lib/cyclic.py
--rw-r--r--   0        0        0      147 2021-11-17 16:48:36.140347 trevorproxy-1.0.4/trevorproxy/lib/errors.py
--rw-r--r--   0        0        0      614 2021-11-16 20:41:59.377569 trevorproxy-1.0.4/trevorproxy/lib/logger.py
--rw-r--r--   0        0        0    10185 2021-11-22 17:27:48.333841 trevorproxy-1.0.4/trevorproxy/lib/requests_wrapper.py
--rw-r--r--   0        0        0     7838 2022-02-02 21:18:40.111715 trevorproxy-1.0.4/trevorproxy/lib/socks.py
--rw-r--r--   0        0        0     6529 2022-02-02 20:29:51.324925 trevorproxy-1.0.4/trevorproxy/lib/ssh.py
--rw-r--r--   0        0        0     1698 2022-02-02 20:17:21.794893 trevorproxy-1.0.4/trevorproxy/lib/subnet.py
--rw-r--r--   0        0        0     4785 2022-02-02 20:29:13.214923 trevorproxy-1.0.4/trevorproxy/lib/util.py
--rw-r--r--   0        0        0      817 2022-02-03 21:56:53.394127 trevorproxy-1.0.4/setup.py
--rw-r--r--   0        0        0      749 2022-02-03 21:56:53.394349 trevorproxy-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0    35248 2021-11-18 17:41:15.210437 trevorproxy-1.0.5/LICENSE
+-rw-r--r--   0        0        0      558 2022-02-07 19:40:53.233630 trevorproxy-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-12-06 20:03:02.221019 trevorproxy-1.0.5/trevorproxy/__init__.py
+-rwxr-xr-x   0        0        0     5244 2021-12-08 21:11:37.029037 trevorproxy-1.0.5/trevorproxy/cli.py
+-rw-r--r--   0        0        0     4381 2021-11-17 21:40:20.027757 trevorproxy-1.0.5/trevorproxy/lib/__pycache__/cyclic.cpython-39.pyc
+-rw-r--r--   0        0        0      588 2021-11-17 16:48:42.200348 trevorproxy-1.0.5/trevorproxy/lib/__pycache__/errors.cpython-39.pyc
+-rw-r--r--   0        0        0     1792 2021-11-17 16:52:06.707023 trevorproxy-1.0.5/trevorproxy/lib/__pycache__/interface.cpython-39.pyc
+-rw-r--r--   0        0        0      670 2021-11-16 20:42:09.080903 trevorproxy-1.0.5/trevorproxy/lib/__pycache__/logger.cpython-39.pyc
+-rw-r--r--   0        0        0     5210 2022-01-06 17:04:42.222402 trevorproxy-1.0.5/trevorproxy/lib/__pycache__/socks.cpython-39.pyc
+-rw-r--r--   0        0        0     7132 2022-01-13 19:59:00.947386 trevorproxy-1.0.5/trevorproxy/lib/__pycache__/ssh.cpython-39.pyc
+-rw-r--r--   0        0        0     1776 2021-11-22 17:12:58.287137 trevorproxy-1.0.5/trevorproxy/lib/__pycache__/subnet.cpython-39.pyc
+-rw-r--r--   0        0        0     4808 2022-01-13 20:09:35.324079 trevorproxy-1.0.5/trevorproxy/lib/__pycache__/util.cpython-39.pyc
+-rw-r--r--   0        0        0     5591 2021-11-17 21:40:17.771090 trevorproxy-1.0.5/trevorproxy/lib/cyclic.py
+-rw-r--r--   0        0        0      147 2021-11-17 16:48:36.140347 trevorproxy-1.0.5/trevorproxy/lib/errors.py
+-rw-r--r--   0        0        0      614 2021-11-16 20:41:59.377569 trevorproxy-1.0.5/trevorproxy/lib/logger.py
+-rw-r--r--   0        0        0    10185 2021-11-22 17:27:48.333841 trevorproxy-1.0.5/trevorproxy/lib/requests_wrapper.py
+-rw-r--r--   0        0        0     7838 2022-02-07 19:40:43.346963 trevorproxy-1.0.5/trevorproxy/lib/socks.py
+-rw-r--r--   0        0        0     6754 2022-02-07 19:40:53.233630 trevorproxy-1.0.5/trevorproxy/lib/ssh.py
+-rw-r--r--   0        0        0     1698 2022-02-07 19:40:43.346963 trevorproxy-1.0.5/trevorproxy/lib/subnet.py
+-rw-r--r--   0        0        0     4785 2022-02-07 19:40:43.346963 trevorproxy-1.0.5/trevorproxy/lib/util.py
+-rw-r--r--   0        0        0      817 2022-02-07 19:41:23.134279 trevorproxy-1.0.5/setup.py
+-rw-r--r--   0        0        0      749 2022-02-07 19:41:23.134563 trevorproxy-1.0.5/PKG-INFO
```

### Comparing `trevorproxy-1.0.4/LICENSE` & `trevorproxy-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `trevorproxy-1.0.4/pyproject.toml` & `trevorproxy-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trevorproxy"
-version = "1.0.4"
+version = "1.0.5"
 description = "Rotate your source IP address via SSH proxies and other methods"
 authors = ["TheTechromancer"]
 license = "GPL-3.0"
 repository = "https://github.com/blacklanternsecurity/TREVORproxy"
 homepage = "https://github.com/blacklanternsecurity/TREVORproxy"
 
 [tool.poetry.dependencies]
```

### Comparing `trevorproxy-1.0.4/trevorproxy/cli.py` & `trevorproxy-1.0.5/trevorproxy/cli.py`

 * *Files identical despite different names*

### Comparing `trevorproxy-1.0.4/trevorproxy/lib/__pycache__/cyclic.cpython-39.pyc` & `trevorproxy-1.0.5/trevorproxy/lib/__pycache__/cyclic.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorproxy-1.0.4/trevorproxy/lib/__pycache__/errors.cpython-39.pyc` & `trevorproxy-1.0.5/trevorproxy/lib/__pycache__/errors.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorproxy-1.0.4/trevorproxy/lib/__pycache__/interface.cpython-39.pyc` & `trevorproxy-1.0.5/trevorproxy/lib/__pycache__/interface.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorproxy-1.0.4/trevorproxy/lib/__pycache__/logger.cpython-39.pyc` & `trevorproxy-1.0.5/trevorproxy/lib/__pycache__/logger.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorproxy-1.0.4/trevorproxy/lib/__pycache__/socks.cpython-39.pyc` & `trevorproxy-1.0.5/trevorproxy/lib/__pycache__/socks.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorproxy-1.0.4/trevorproxy/lib/__pycache__/ssh.cpython-39.pyc` & `trevorproxy-1.0.5/trevorproxy/lib/__pycache__/ssh.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorproxy-1.0.4/trevorproxy/lib/__pycache__/subnet.cpython-39.pyc` & `trevorproxy-1.0.5/trevorproxy/lib/__pycache__/subnet.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorproxy-1.0.4/trevorproxy/lib/__pycache__/util.cpython-39.pyc` & `trevorproxy-1.0.5/trevorproxy/lib/__pycache__/util.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorproxy-1.0.4/trevorproxy/lib/cyclic.py` & `trevorproxy-1.0.5/trevorproxy/lib/cyclic.py`

 * *Files identical despite different names*

### Comparing `trevorproxy-1.0.4/trevorproxy/lib/logger.py` & `trevorproxy-1.0.5/trevorproxy/lib/logger.py`

 * *Files identical despite different names*

### Comparing `trevorproxy-1.0.4/trevorproxy/lib/requests_wrapper.py` & `trevorproxy-1.0.5/trevorproxy/lib/requests_wrapper.py`

 * *Files identical despite different names*

### Comparing `trevorproxy-1.0.4/trevorproxy/lib/socks.py` & `trevorproxy-1.0.5/trevorproxy/lib/socks.py`

 * *Files identical despite different names*

### Comparing `trevorproxy-1.0.4/trevorproxy/lib/ssh.py` & `trevorproxy-1.0.5/trevorproxy/lib/ssh.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,31 +29,34 @@
         self._ssh_stdout = ''
         self.running = False
 
 
     def start(self, wait=True, timeout=30):
 
         self.stop()
-        log.info(f'Opening SSH connection to {self.host}')
 
-        self._ssh_stdout = ''
-        self._password_entered = False
-        self.sh = sh.ssh(
-            self.host,
-            _out=self._enter_password,
-            _out_bufsize=0,
-            _tty_in=True,
-            _unify_ttys=True,
-            _long_sep=' ',
-            _bg=True,
-            _bg_exc=False,
-            **self.ssh_args
-        )
-        self.command = b' '.join(self.sh.cmd).decode()
-        log.debug(self.command)
+        if not self.is_connected():
+            log.info(f'Opening SSH connection to {self.host}')
+            self._ssh_stdout = ''
+            self._password_entered = False
+            self.sh = sh.ssh(
+                self.host,
+                _out=self._enter_password,
+                _out_bufsize=0,
+                _tty_in=True,
+                _unify_ttys=True,
+                _long_sep=' ',
+                _bg=True,
+                _bg_exc=False,
+                **self.ssh_args
+            )
+            self.command = b' '.join(self.sh.cmd).decode()
+            log.debug(self.command)
+        else:
+            log.debug(f'{self.__class__.__name__}.start() called but SSH connection is already established')
 
         left = int(timeout)
         if wait:
             while not self.is_connected():
                 left -= 1
                 if left <= 0 or not self.sh.is_alive():
                     raise SSHProxyError(f'Failed to start SSHProxy {self}')
@@ -141,15 +144,15 @@
         for i,proxy in enumerate(self.proxies):
             if proxy is not None:
                 iptables_add = ['iptables', '-A']
                 iptables_main = ['OUTPUT', '-t', 'nat', '-d', f'{self.address}', '-o', 'lo', '-p', \
                     'tcp', '--dport', f'{self.proxy_port}', '-j', 'DNAT', '--to-destination', f'127.0.0.1:{proxy.proxy_port}']
 
                 # if this isn't the last proxy
-                if not i == len(self.proxies)-1:
+                if not i == len(self.proxies) - 1:
                     iptables_main += ['-m', 'statistic', '--mode', 'nth', '--every', f'{len(self.proxies)-i}', '--packet', '0']
 
                 self.iptables_rules.append(iptables_main)
 
                 cmd = siptables_add + iptables_main
                 sudo_run(cmd)
```

### Comparing `trevorproxy-1.0.4/trevorproxy/lib/subnet.py` & `trevorproxy-1.0.5/trevorproxy/lib/subnet.py`

 * *Files identical despite different names*

### Comparing `trevorproxy-1.0.4/trevorproxy/lib/util.py` & `trevorproxy-1.0.5/trevorproxy/lib/util.py`

 * *Files identical despite different names*

### Comparing `trevorproxy-1.0.4/setup.py` & `trevorproxy-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['sh>=1.14.2,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['trevorproxy = trevorproxy.cli:main']}
 
 setup_kwargs = {
     'name': 'trevorproxy',
-    'version': '1.0.4',
+    'version': '1.0.5',
     'description': 'Rotate your source IP address via SSH proxies and other methods',
     'long_description': None,
     'author': 'TheTechromancer',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/blacklanternsecurity/TREVORproxy',
```

### Comparing `trevorproxy-1.0.4/PKG-INFO` & `trevorproxy-1.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trevorproxy
-Version: 1.0.4
+Version: 1.0.5
 Summary: Rotate your source IP address via SSH proxies and other methods
 Home-page: https://github.com/blacklanternsecurity/TREVORproxy
 License: GPL-3.0
 Author: TheTechromancer
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

