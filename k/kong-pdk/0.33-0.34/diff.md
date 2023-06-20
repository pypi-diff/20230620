# Comparing `tmp/kong_pdk-0.33.tar.gz` & `tmp/kong_pdk-0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kong_pdk-0.33.tar", last modified: Wed Feb 15 03:04:44 2023, max compression
+gzip compressed data, was "kong_pdk-0.34.tar", last modified: Tue Jun 20 04:19:55 2023, max compression
```

## Comparing `kong_pdk-0.33.tar` & `kong_pdk-0.34.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 fffonion   (501) staff       (20)        0 2023-02-15 03:04:44.822478 kong_pdk-0.33/
--rw-r--r--   0 fffonion   (501) staff       (20)    11345 2021-03-22 08:08:14.000000 kong_pdk-0.33/LICENSE
--rw-r--r--   0 fffonion   (501) staff       (20)    10686 2023-02-15 03:04:44.822549 kong_pdk-0.33/PKG-INFO
--rw-r--r--   0 fffonion   (501) staff       (20)     2750 2022-10-20 08:28:19.000000 kong_pdk-0.33/README.md
-drwxr-xr-x   0 fffonion   (501) staff       (20)        0 2023-02-15 03:04:44.818690 kong_pdk-0.33/kong_pdk/
--rw-r--r--   0 fffonion   (501) staff       (20)        0 2021-03-26 09:39:18.000000 kong_pdk-0.33/kong_pdk/__init__.py
--rw-r--r--   0 fffonion   (501) staff       (20)     6221 2022-10-07 10:57:34.000000 kong_pdk-0.33/kong_pdk/cli.py
--rw-r--r--   0 fffonion   (501) staff       (20)      661 2023-02-15 03:04:21.000000 kong_pdk-0.33/kong_pdk/const.py
--rw-r--r--   0 fffonion   (501) staff       (20)       90 2021-08-05 15:07:12.000000 kong_pdk-0.33/kong_pdk/exception.py
--rw-r--r--   0 fffonion   (501) staff       (20)       23 2021-08-05 15:07:12.000000 kong_pdk-0.33/kong_pdk/kong.py
--rw-r--r--   0 fffonion   (501) staff       (20)     4071 2022-10-07 10:57:34.000000 kong_pdk-0.33/kong_pdk/listener.py
--rw-r--r--   0 fffonion   (501) staff       (20)     5547 2021-08-05 15:07:12.000000 kong_pdk-0.33/kong_pdk/logger.py
--rw-r--r--   0 fffonion   (501) staff       (20)     2639 2022-10-07 10:57:34.000000 kong_pdk-0.33/kong_pdk/module.py
-drwxr-xr-x   0 fffonion   (501) staff       (20)        0 2023-02-15 03:04:44.819886 kong_pdk-0.33/kong_pdk/pdk/
--rw-r--r--   0 fffonion   (501) staff       (20)     1167 2022-10-20 08:28:19.000000 kong_pdk-0.33/kong_pdk/pdk/__init__.py
-drwxr-xr-x   0 fffonion   (501) staff       (20)        0 2023-02-15 03:04:44.821189 kong_pdk-0.33/kong_pdk/pdk/kong/
--rw-r--r--   0 fffonion   (501) staff       (20)     1043 2023-02-15 03:04:21.000000 kong_pdk-0.33/kong_pdk/pdk/kong/__init__.py
-drwxr-xr-x   0 fffonion   (501) staff       (20)        0 2023-02-15 03:04:44.821465 kong_pdk-0.33/kong_pdk/pdk/kong/client/
--rw-r--r--   0 fffonion   (501) staff       (20)     8888 2023-02-15 03:04:21.000000 kong_pdk-0.33/kong_pdk/pdk/kong/client/__init__.py
--rw-r--r--   0 fffonion   (501) staff       (20)     4943 2023-02-15 03:04:21.000000 kong_pdk-0.33/kong_pdk/pdk/kong/client/tls.py
--rw-r--r--   0 fffonion   (501) staff       (20)     1205 2023-02-15 03:04:21.000000 kong_pdk-0.33/kong_pdk/pdk/kong/cluster.py
-drwxr-xr-x   0 fffonion   (501) staff       (20)        0 2023-02-15 03:04:44.821721 kong_pdk-0.33/kong_pdk/pdk/kong/ctx/
--rw-r--r--   0 fffonion   (501) staff       (20)      376 2023-02-15 03:04:21.000000 kong_pdk-0.33/kong_pdk/pdk/kong/ctx/__init__.py
--rw-r--r--   0 fffonion   (501) staff       (20)      892 2023-02-15 03:04:21.000000 kong_pdk-0.33/kong_pdk/pdk/kong/ctx/shared.py
--rw-r--r--   0 fffonion   (501) staff       (20)      999 2023-02-15 03:04:21.000000 kong_pdk-0.33/kong_pdk/pdk/kong/ip.py
--rw-r--r--   0 fffonion   (501) staff       (20)    18220 2023-02-15 03:04:21.000000 kong_pdk-0.33/kong_pdk/pdk/kong/log.py
-drwxr-xr-x   0 fffonion   (501) staff       (20)        0 2023-02-15 03:04:44.821974 kong_pdk-0.33/kong_pdk/pdk/kong/nginx/
--rw-r--r--   0 fffonion   (501) staff       (20)     3100 2023-02-15 03:04:21.000000 kong_pdk-0.33/kong_pdk/pdk/kong/nginx/__init__.py
--rw-r--r--   0 fffonion   (501) staff       (20)      894 2023-02-15 03:04:21.000000 kong_pdk-0.33/kong_pdk/pdk/kong/nginx/shared.py
--rw-r--r--   0 fffonion   (501) staff       (20)     3037 2023-02-15 03:04:21.000000 kong_pdk-0.33/kong_pdk/pdk/kong/node.py
--rw-r--r--   0 fffonion   (501) staff       (20)    22702 2023-02-15 03:04:21.000000 kong_pdk-0.33/kong_pdk/pdk/kong/request.py
--rw-r--r--   0 fffonion   (501) staff       (20)    18501 2023-02-15 03:04:21.000000 kong_pdk-0.33/kong_pdk/pdk/kong/response.py
--rw-r--r--   0 fffonion   (501) staff       (20)     1281 2023-02-15 03:04:21.000000 kong_pdk-0.33/kong_pdk/pdk/kong/router.py
-drwxr-xr-x   0 fffonion   (501) staff       (20)        0 2023-02-15 03:04:44.822366 kong_pdk-0.33/kong_pdk/pdk/kong/service/
--rw-r--r--   0 fffonion   (501) staff       (20)     4831 2023-02-15 03:04:21.000000 kong_pdk-0.33/kong_pdk/pdk/kong/service/__init__.py
--rw-r--r--   0 fffonion   (501) staff       (20)    13919 2023-02-15 03:04:21.000000 kong_pdk-0.33/kong_pdk/pdk/kong/service/request.py
--rw-r--r--   0 fffonion   (501) staff       (20)     5706 2023-02-15 03:04:21.000000 kong_pdk-0.33/kong_pdk/pdk/kong/service/response.py
--rw-r--r--   0 fffonion   (501) staff       (20)     2776 2023-02-15 03:04:21.000000 kong_pdk-0.33/kong_pdk/pdk/kong/vault.py
--rw-r--r--   0 fffonion   (501) staff       (20)    10614 2022-10-20 08:28:19.000000 kong_pdk-0.33/kong_pdk/server.py
-drwxr-xr-x   0 fffonion   (501) staff       (20)        0 2023-02-15 03:04:44.819754 kong_pdk-0.33/kong_pdk.egg-info/
--rw-r--r--   0 fffonion   (501) staff       (20)    10686 2023-02-15 03:04:44.000000 kong_pdk-0.33/kong_pdk.egg-info/PKG-INFO
--rw-r--r--   0 fffonion   (501) staff       (20)     1024 2023-02-15 03:04:44.000000 kong_pdk-0.33/kong_pdk.egg-info/SOURCES.txt
--rw-r--r--   0 fffonion   (501) staff       (20)        1 2023-02-15 03:04:44.000000 kong_pdk-0.33/kong_pdk.egg-info/dependency_links.txt
--rw-r--r--   0 fffonion   (501) staff       (20)       71 2023-02-15 03:04:44.000000 kong_pdk-0.33/kong_pdk.egg-info/entry_points.txt
--rw-r--r--   0 fffonion   (501) staff       (20)        1 2021-03-26 09:39:30.000000 kong_pdk-0.33/kong_pdk.egg-info/not-zip-safe
--rw-r--r--   0 fffonion   (501) staff       (20)       15 2023-02-15 03:04:44.000000 kong_pdk-0.33/kong_pdk.egg-info/requires.txt
--rw-r--r--   0 fffonion   (501) staff       (20)      137 2023-02-15 03:04:44.000000 kong_pdk-0.33/kong_pdk.egg-info/top_level.txt
--rw-r--r--   0 fffonion   (501) staff       (20)      184 2023-02-15 03:04:44.822812 kong_pdk-0.33/setup.cfg
--rw-r--r--   0 fffonion   (501) staff       (20)     1999 2022-10-07 10:57:34.000000 kong_pdk-0.33/setup.py
+drwxr-xr-x   0 fffonion   (501) staff       (20)        0 2023-06-20 04:19:55.299588 kong_pdk-0.34/
+-rw-r--r--   0 fffonion   (501) staff       (20)    11345 2021-03-22 08:08:14.000000 kong_pdk-0.34/LICENSE
+-rw-r--r--   0 fffonion   (501) staff       (20)    10686 2023-06-20 04:19:55.299657 kong_pdk-0.34/PKG-INFO
+-rw-r--r--   0 fffonion   (501) staff       (20)     2750 2022-10-20 08:28:19.000000 kong_pdk-0.34/README.md
+drwxr-xr-x   0 fffonion   (501) staff       (20)        0 2023-06-20 04:19:55.296094 kong_pdk-0.34/kong_pdk/
+-rw-r--r--   0 fffonion   (501) staff       (20)        0 2021-03-26 09:39:18.000000 kong_pdk-0.34/kong_pdk/__init__.py
+-rw-r--r--   0 fffonion   (501) staff       (20)     6221 2022-10-07 10:57:34.000000 kong_pdk-0.34/kong_pdk/cli.py
+-rw-r--r--   0 fffonion   (501) staff       (20)      661 2023-06-20 04:18:40.000000 kong_pdk-0.34/kong_pdk/const.py
+-rw-r--r--   0 fffonion   (501) staff       (20)       90 2021-08-05 15:07:12.000000 kong_pdk-0.34/kong_pdk/exception.py
+-rw-r--r--   0 fffonion   (501) staff       (20)       23 2021-08-05 15:07:12.000000 kong_pdk-0.34/kong_pdk/kong.py
+-rw-r--r--   0 fffonion   (501) staff       (20)     4093 2023-06-20 04:09:23.000000 kong_pdk-0.34/kong_pdk/listener.py
+-rw-r--r--   0 fffonion   (501) staff       (20)     5547 2021-08-05 15:07:12.000000 kong_pdk-0.34/kong_pdk/logger.py
+-rw-r--r--   0 fffonion   (501) staff       (20)     2639 2022-10-07 10:57:34.000000 kong_pdk-0.34/kong_pdk/module.py
+drwxr-xr-x   0 fffonion   (501) staff       (20)        0 2023-06-20 04:19:55.297077 kong_pdk-0.34/kong_pdk/pdk/
+-rw-r--r--   0 fffonion   (501) staff       (20)     1427 2023-06-20 04:09:23.000000 kong_pdk-0.34/kong_pdk/pdk/__init__.py
+drwxr-xr-x   0 fffonion   (501) staff       (20)        0 2023-06-20 04:19:55.298326 kong_pdk-0.34/kong_pdk/pdk/kong/
+-rw-r--r--   0 fffonion   (501) staff       (20)     1233 2023-06-20 04:09:23.000000 kong_pdk-0.34/kong_pdk/pdk/kong/__init__.py
+drwxr-xr-x   0 fffonion   (501) staff       (20)        0 2023-06-20 04:19:55.298571 kong_pdk-0.34/kong_pdk/pdk/kong/client/
+-rw-r--r--   0 fffonion   (501) staff       (20)     8888 2023-06-20 04:09:23.000000 kong_pdk-0.34/kong_pdk/pdk/kong/client/__init__.py
+-rw-r--r--   0 fffonion   (501) staff       (20)     4943 2023-06-20 04:09:23.000000 kong_pdk-0.34/kong_pdk/pdk/kong/client/tls.py
+-rw-r--r--   0 fffonion   (501) staff       (20)     1205 2023-06-20 04:09:23.000000 kong_pdk-0.34/kong_pdk/pdk/kong/cluster.py
+drwxr-xr-x   0 fffonion   (501) staff       (20)        0 2023-06-20 04:19:55.298833 kong_pdk-0.34/kong_pdk/pdk/kong/ctx/
+-rw-r--r--   0 fffonion   (501) staff       (20)      376 2023-06-20 04:09:23.000000 kong_pdk-0.34/kong_pdk/pdk/kong/ctx/__init__.py
+-rw-r--r--   0 fffonion   (501) staff       (20)      892 2023-06-20 04:09:23.000000 kong_pdk-0.34/kong_pdk/pdk/kong/ctx/shared.py
+-rw-r--r--   0 fffonion   (501) staff       (20)      999 2023-06-20 04:09:23.000000 kong_pdk-0.34/kong_pdk/pdk/kong/ip.py
+-rw-r--r--   0 fffonion   (501) staff       (20)    18220 2023-06-20 04:09:23.000000 kong_pdk-0.34/kong_pdk/pdk/kong/log.py
+drwxr-xr-x   0 fffonion   (501) staff       (20)        0 2023-06-20 04:19:55.299077 kong_pdk-0.34/kong_pdk/pdk/kong/nginx/
+-rw-r--r--   0 fffonion   (501) staff       (20)     3100 2023-06-20 04:09:23.000000 kong_pdk-0.34/kong_pdk/pdk/kong/nginx/__init__.py
+-rw-r--r--   0 fffonion   (501) staff       (20)      894 2023-06-20 04:09:23.000000 kong_pdk-0.34/kong_pdk/pdk/kong/nginx/shared.py
+-rw-r--r--   0 fffonion   (501) staff       (20)     3678 2023-06-20 04:09:23.000000 kong_pdk-0.34/kong_pdk/pdk/kong/node.py
+-rw-r--r--   0 fffonion   (501) staff       (20)      699 2023-06-20 04:09:23.000000 kong_pdk-0.34/kong_pdk/pdk/kong/plugin.py
+-rw-r--r--   0 fffonion   (501) staff       (20)    22936 2023-06-20 04:09:23.000000 kong_pdk-0.34/kong_pdk/pdk/kong/request.py
+-rw-r--r--   0 fffonion   (501) staff       (20)    18572 2023-06-20 04:09:23.000000 kong_pdk-0.34/kong_pdk/pdk/kong/response.py
+-rw-r--r--   0 fffonion   (501) staff       (20)     1281 2023-06-20 04:09:23.000000 kong_pdk-0.34/kong_pdk/pdk/kong/router.py
+drwxr-xr-x   0 fffonion   (501) staff       (20)        0 2023-06-20 04:19:55.299474 kong_pdk-0.34/kong_pdk/pdk/kong/service/
+-rw-r--r--   0 fffonion   (501) staff       (20)     4831 2023-06-20 04:09:23.000000 kong_pdk-0.34/kong_pdk/pdk/kong/service/__init__.py
+-rw-r--r--   0 fffonion   (501) staff       (20)    13919 2023-06-20 04:09:23.000000 kong_pdk-0.34/kong_pdk/pdk/kong/service/request.py
+-rw-r--r--   0 fffonion   (501) staff       (20)     5710 2023-06-20 04:09:23.000000 kong_pdk-0.34/kong_pdk/pdk/kong/service/response.py
+-rw-r--r--   0 fffonion   (501) staff       (20)     4451 2023-06-20 04:09:23.000000 kong_pdk-0.34/kong_pdk/pdk/kong/vault.py
+-rw-r--r--   0 fffonion   (501) staff       (20)    10614 2022-10-20 08:28:19.000000 kong_pdk-0.34/kong_pdk/server.py
+drwxr-xr-x   0 fffonion   (501) staff       (20)        0 2023-06-20 04:19:55.296952 kong_pdk-0.34/kong_pdk.egg-info/
+-rw-r--r--   0 fffonion   (501) staff       (20)    10686 2023-06-20 04:19:55.000000 kong_pdk-0.34/kong_pdk.egg-info/PKG-INFO
+-rw-r--r--   0 fffonion   (501) staff       (20)     1052 2023-06-20 04:19:55.000000 kong_pdk-0.34/kong_pdk.egg-info/SOURCES.txt
+-rw-r--r--   0 fffonion   (501) staff       (20)        1 2023-06-20 04:19:55.000000 kong_pdk-0.34/kong_pdk.egg-info/dependency_links.txt
+-rw-r--r--   0 fffonion   (501) staff       (20)       71 2023-06-20 04:19:55.000000 kong_pdk-0.34/kong_pdk.egg-info/entry_points.txt
+-rw-r--r--   0 fffonion   (501) staff       (20)        1 2021-03-26 09:39:30.000000 kong_pdk-0.34/kong_pdk.egg-info/not-zip-safe
+-rw-r--r--   0 fffonion   (501) staff       (20)       15 2023-06-20 04:19:55.000000 kong_pdk-0.34/kong_pdk.egg-info/requires.txt
+-rw-r--r--   0 fffonion   (501) staff       (20)      137 2023-06-20 04:19:55.000000 kong_pdk-0.34/kong_pdk.egg-info/top_level.txt
+-rw-r--r--   0 fffonion   (501) staff       (20)      184 2023-06-20 04:19:55.299965 kong_pdk-0.34/setup.cfg
+-rw-r--r--   0 fffonion   (501) staff       (20)     1999 2022-10-07 10:57:34.000000 kong_pdk-0.34/setup.py
```

### Comparing `kong_pdk-0.33/LICENSE` & `kong_pdk-0.34/LICENSE`

 * *Files identical despite different names*

### Comparing `kong_pdk-0.33/PKG-INFO` & `kong_pdk-0.34/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kong_pdk
-Version: 0.33
+Version: 0.34
 Summary: Kong PDK for Python and Plugin Server
 Home-page: https://github.com/Kong/kong-python-pdk
 Author: Kong
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
@@ -105,16 +105,16 @@
 - Hot reload
 
 
 <a name="unreleased"></a>
 ## [Unreleased]
 
 
-<a name="0.3.3"></a>
-## [0.3.3] - 2023-02-01
+<a name="0.3.4"></a>
+## [0.3.4] - 2023-06-20
 
 <a name="0.3.2"></a>
 ## [0.3.2] - 2022-11-08
 ### bug fixes
 - add version field in PluginInfo rpc ([#79](https://github.com/Kong/kong-python-pdk/issues/79)) [132f31d](https://github.com/Kong/kong-python-pdk/commit/132f31d526ff3589ac9b93dc079adb18359519cd)
 
 
@@ -216,16 +216,16 @@
 
 <a name="0.1.1"></a>
 ## [0.1.1] - 2020-02-20
 
 <a name="0.1.0"></a>
 ## 0.1.0 - 2020-01-03
 
-[Unreleased]: https://github.com/Kong/kong-python-pdk/compare/0.3.3...HEAD
-[0.3.3]: https://github.com/Kong/kong-python-pdk/compare/0.3.2...0.3.3
+[Unreleased]: https://github.com/Kong/kong-python-pdk/compare/0.3.4...HEAD
+[0.3.4]: https://github.com/Kong/kong-python-pdk/compare/0.3.2...0.3.4
 [0.3.2]: https://github.com/Kong/kong-python-pdk/compare/0.3.1...0.3.2
 [0.3.1]: https://github.com/Kong/kong-python-pdk/compare/0.3.0...0.3.1
 [0.3.0]: https://github.com/Kong/kong-python-pdk/compare/0.2.7...0.3.0
 [0.2.7]: https://github.com/Kong/kong-python-pdk/compare/0.2.6...0.2.7
 [0.2.6]: https://github.com/Kong/kong-python-pdk/compare/0.2.5...0.2.6
 [0.2.5]: https://github.com/Kong/kong-python-pdk/compare/0.2.4...0.2.5
 [0.2.4]: https://github.com/Kong/kong-python-pdk/compare/0.2.3...0.2.4
```

### Comparing `kong_pdk-0.33/README.md` & `kong_pdk-0.34/README.md`

 * *Files identical despite different names*

### Comparing `kong_pdk-0.33/kong_pdk/cli.py` & `kong_pdk-0.34/kong_pdk/cli.py`

 * *Files identical despite different names*

### Comparing `kong_pdk-0.33/kong_pdk/listener.py` & `kong_pdk-0.34/kong_pdk/listener.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         self.ps = plugin_server
         self.logger = plugin_server.logger
 
     def handle(self, fd, address, *_):
         # can't use socket.makefile here, since it returns a blocking IO
         # msgpack.Unpacker only expects read() but no other semantics to exist
         sockf = WrapSocket(fd)
-        unpacker = msgpack.Unpacker(sockf)
+        unpacker = msgpack.Unpacker(sockf, strict_map_key=False)
 
         for _, msgid, method, args in unpacker:
             ns, cmd = method.split(".")
             if ns != "plugin":
                 write_error(fd, msgid, "RPC for %s is not supported" % ns)
                 continue
```

### Comparing `kong_pdk-0.33/kong_pdk/logger.py` & `kong_pdk-0.34/kong_pdk/logger.py`

 * *Files identical despite different names*

### Comparing `kong_pdk-0.33/kong_pdk/module.py` & `kong_pdk-0.34/kong_pdk/module.py`

 * *Files identical despite different names*

### Comparing `kong_pdk-0.33/kong_pdk/pdk/__init__.py` & `kong_pdk-0.34/kong_pdk/pdk/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,14 +20,21 @@
 non_return_methods = set((
     "kong.response.exit",
     "kong.response.error",
 ))
 
 def rpc_of(ch, lua_style):
     def f(m, *a):
+        # sanitize non-serializable objects
+        if m == "kong.log" or m.startswith("kong.log."):
+            a = list(a)
+            for i in range(len(a)):
+                if type(a[i]) not in (str, int, list, dict):
+                    a[i] = str(a[i])
+
         ch.put({
             "Method": m,
             "Args": a,
         })
         if m in non_return_methods:
             return
```

### Comparing `kong_pdk-0.33/kong_pdk/pdk/kong/__init__.py` & `kong_pdk-0.34/kong_pdk/pdk/kong/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,44 @@
-# AUTO GENERATED BASED ON Kong 3.2.x, DO NOT EDIT
+# AUTO GENERATED BASED ON Kong 3.4.x, DO NOT EDIT
 # Original source path: kong/pdk.lua
 
 from typing import TypeVar, Any, Union, List, Mapping, Tuple, Optional
 
 number = TypeVar('number', int, float)
 table = TypeVar('table', List[Any], Mapping[str, Any])
 # XXX
 cdata = Any
 err = str
 
 from .client import client as cls_client
 from .cluster import cluster as cls_cluster
 from .ctx import ctx as cls_ctx
+from .enterprise_edition import enterprise_edition as cls_enterprise_edition
 from .ip import ip as cls_ip
 from .log import log as cls_log
 from .nginx import nginx as cls_nginx
 from .node import node as cls_node
+from .plugin import plugin as cls_plugin
 from .request import request as cls_request
 from .response import response as cls_response
 from .router import router as cls_router
 from .service import service as cls_service
 from .vault import vault as cls_vault
 
 class kong():
 
     client = cls_client
     cluster = cls_cluster
     ctx = cls_ctx
+    enterprise_edition = cls_enterprise_edition
     ip = cls_ip
     log = cls_log
     nginx = cls_nginx
     node = cls_node
+    plugin = cls_plugin
     request = cls_request
     response = cls_response
     router = cls_router
     service = cls_service
     vault = cls_vault
 
     pass
```

### Comparing `kong_pdk-0.33/kong_pdk/pdk/kong/client/__init__.py` & `kong_pdk-0.34/kong_pdk/pdk/kong/client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED BASED ON Kong 3.2.x, DO NOT EDIT
+# AUTO GENERATED BASED ON Kong 3.4.x, DO NOT EDIT
 # Original source path: kong/pdk/client.lua
 
 from typing import TypeVar, Any, Union, List, Mapping, Tuple, Optional
 
 number = TypeVar('number', int, float)
 table = TypeVar('table', List[Any], Mapping[str, Any])
 # XXX
```

### Comparing `kong_pdk-0.33/kong_pdk/pdk/kong/client/tls.py` & `kong_pdk-0.34/kong_pdk/pdk/kong/client/tls.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED BASED ON Kong 3.2.x, DO NOT EDIT
+# AUTO GENERATED BASED ON Kong 3.4.x, DO NOT EDIT
 # Original source path: kong/pdk/client/tls.lua
 
 from typing import TypeVar, Any, Union, List, Mapping, Tuple, Optional
 
 number = TypeVar('number', int, float)
 table = TypeVar('table', List[Any], Mapping[str, Any])
 # XXX
```

### Comparing `kong_pdk-0.33/kong_pdk/pdk/kong/cluster.py` & `kong_pdk-0.34/kong_pdk/pdk/kong/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED BASED ON Kong 3.2.x, DO NOT EDIT
+# AUTO GENERATED BASED ON Kong 3.4.x, DO NOT EDIT
 # Original source path: kong/pdk/cluster.lua
 
 from typing import TypeVar, Any, Union, List, Mapping, Tuple, Optional
 
 number = TypeVar('number', int, float)
 table = TypeVar('table', List[Any], Mapping[str, Any])
 # XXX
```

### Comparing `kong_pdk-0.33/kong_pdk/pdk/kong/ctx/shared.py` & `kong_pdk-0.34/kong_pdk/pdk/kong/ctx/shared.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED BASED ON Kong 3.2.x, DO NOT EDIT
+# AUTO GENERATED BASED ON Kong 3.4.x, DO NOT EDIT
 # Original source path: kong/pdk/ctx/shared.lua
 
 from typing import TypeVar, Any, Union, List, Mapping, Tuple, Optional
 
 number = TypeVar('number', int, float)
 table = TypeVar('table', List[Any], Mapping[str, Any])
 # XXX
```

### Comparing `kong_pdk-0.33/kong_pdk/pdk/kong/ip.py` & `kong_pdk-0.34/kong_pdk/pdk/kong/ip.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED BASED ON Kong 3.2.x, DO NOT EDIT
+# AUTO GENERATED BASED ON Kong 3.4.x, DO NOT EDIT
 # Original source path: kong/pdk/ip.lua
 
 from typing import TypeVar, Any, Union, List, Mapping, Tuple, Optional
 
 number = TypeVar('number', int, float)
 table = TypeVar('table', List[Any], Mapping[str, Any])
 # XXX
```

### Comparing `kong_pdk-0.33/kong_pdk/pdk/kong/log.py` & `kong_pdk-0.34/kong_pdk/pdk/kong/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED BASED ON Kong 3.2.x, DO NOT EDIT
+# AUTO GENERATED BASED ON Kong 3.4.x, DO NOT EDIT
 # Original source path: kong/pdk/log.lua
 
 from typing import TypeVar, Any, Union, List, Mapping, Tuple, Optional
 
 number = TypeVar('number', int, float)
 table = TypeVar('table', List[Any], Mapping[str, Any])
 # XXX
```

### Comparing `kong_pdk-0.33/kong_pdk/pdk/kong/nginx/__init__.py` & `kong_pdk-0.34/kong_pdk/pdk/kong/nginx/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED BASED ON Kong 3.2.x, DO NOT EDIT
+# AUTO GENERATED BASED ON Kong 3.4.x, DO NOT EDIT
 # Original source path: kong/pdk/nginx.lua
 
 from typing import TypeVar, Any, Union, List, Mapping, Tuple, Optional
 
 number = TypeVar('number', int, float)
 table = TypeVar('table', List[Any], Mapping[str, Any])
 # XXX
@@ -76,15 +76,15 @@
         """
         pass
 
     @staticmethod
     def get_var() -> str:
         """
 
-        :return: the NGINX version string
+        :return: get NGINX variable value
 
         :rtype: str
         """
         pass
 
     @staticmethod
     def req_start_time() -> number:
```

### Comparing `kong_pdk-0.33/kong_pdk/pdk/kong/nginx/shared.py` & `kong_pdk-0.34/kong_pdk/pdk/kong/nginx/shared.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED BASED ON Kong 3.2.x, DO NOT EDIT
+# AUTO GENERATED BASED ON Kong 3.4.x, DO NOT EDIT
 # Original source path: kong/pdk/nginx/shared.lua
 
 from typing import TypeVar, Any, Union, List, Mapping, Tuple, Optional
 
 number = TypeVar('number', int, float)
 table = TypeVar('table', List[Any], Mapping[str, Any])
 # XXX
```

### Comparing `kong_pdk-0.33/kong_pdk/pdk/kong/node.py` & `kong_pdk-0.34/kong_pdk/pdk/kong/node.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED BASED ON Kong 3.2.x, DO NOT EDIT
+# AUTO GENERATED BASED ON Kong 3.4.x, DO NOT EDIT
 # Original source path: kong/pdk/node.lua
 
 from typing import TypeVar, Any, Union, List, Mapping, Tuple, Optional
 
 number = TypeVar('number', int, float)
 table = TypeVar('table', List[Any], Mapping[str, Any])
 # XXX
@@ -90,14 +90,34 @@
 
             http_allocated_gc = 1102,
 
             pid = 18005
 
             }
 
+            },
+
+            # if the `kong` uses dbless mode, the following will be present:
+
+            lmdb = {
+
+            map_size: "128.00 MiB",
+
+            used_size: "0.02 MiB",
+
+            last_used_page: 6,
+
+            last_txnid: 2,
+
+            max_readers: 126,
+
+            current_readers: 16
+
+            },
+
             }
 
             }
 
             res = kong.node.get_memory_stats("k", 1)
 
             # res will have the following structure:
@@ -140,14 +160,32 @@
 
             pid = 18005
 
             }
 
             }
 
+            # if the `kong` uses dbless mode, the following will be present:
+
+            lmdb = {
+
+            map_size: "131072 KB",
+
+            used_size: "20.48 KB",
+
+            last_used_page: 6,
+
+            last_txnid: 2,
+
+            max_readers: 126,
+
+            current_readers: 16
+
+            },
+
             }
 
         :parameter unit: The unit that memory is reported in. Can be
             any of `b/B`, `k/K`, `m/M`, or `g/G` for bytes, kibibytes, mebibytes,
             or gibibytes, respectively. Defaults to `b` (bytes).
         :type unit: str
         :parameter scale: The number of digits to the right of the decimal
```

### Comparing `kong_pdk-0.33/kong_pdk/pdk/kong/request.py` & `kong_pdk-0.34/kong_pdk/pdk/kong/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED BASED ON Kong 3.2.x, DO NOT EDIT
+# AUTO GENERATED BASED ON Kong 3.4.x, DO NOT EDIT
 # Original source path: kong/pdk/request.lua
 
 from typing import TypeVar, Any, Union, List, Mapping, Tuple, Optional
 
 number = TypeVar('number', int, float)
 table = TypeVar('table', List[Any], Mapping[str, Any])
 # XXX
@@ -39,15 +39,16 @@
               * Decodes the body as JSON
                 (same as `json.decode(kong.request.get_raw_body())`).
               * JSON types are converted to matching Lua types.
             * If the request contains none of the above and the `mimetype` argument is
               not set, returns `nil` and an error message indicating the
               body could not be parsed.
             The optional argument `max_args` can be used to set a limit on the number
-            of form arguments parsed for `application/x-www-form-urlencoded` payloads.
+            of form arguments parsed for `application/x-www-form-urlencoded` payloads,
+            which is by default **100** (or what has been configured using `lua_max_post_args`).
             The third return value is string containing the mimetype used to parsed
             the body (as per the `mimetype` argument), allowing the caller to identify
             what MIME type the body was parsed as.
 
         Phases:
             rewrite, access, response, admin_api
 
@@ -270,17 +271,18 @@
 
             Returns a Lua table holding the request headers. Keys are header names.
             Values are either a string with the header value, or an array of strings
             if a header was sent multiple times. Header names in this table are
             case-insensitive and are normalized to lowercase, and dashes (`-`) can be
             written as underscores (`_`); that is, the header `X-Custom-Header` can
             also be retrieved as `x_custom_header`.
-            By default, this function returns up to **100** headers. The optional
-            `max_headers` argument can be specified to customize this limit, but must
-            be greater than **1** and not greater than **1000**.
+            By default, this function returns up to **100** headers (or what has been
+            configured using `lua_max_req_headers`). The optional `max_headers` argument
+            can be specified to customize this limit, but must be greater than **1** and
+            not greater than **1000**.
 
         Phases:
             rewrite, access, header_filter, response, body_filter, log, admin_api
 
         Example:
             # Given a request with the following headers:
 
@@ -450,17 +452,18 @@
             are query argument names. Values are either a string with the argument
             value, a boolean `true` if an argument was not given a value, or an array
             if an argument was given in the query string multiple times. Keys and
             values are unescaped according to URL-encoded escaping rules.
             Note that a query string `?foo&bar` translates to two boolean `true`
             arguments, and `?foo=&bar=` translates to two string arguments containing
             empty strings.
-            By default, this function returns up to **100** arguments. The optional
-            `max_args` argument can be specified to customize this limit, but must be
-            greater than **1** and not greater than **1000**.
+            By default, this function returns up to **100** arguments (or what has been
+            configured using `lua_max_uri_args`). The optional `max_args` argument can be
+            specified to customize this limit, but must be greater than **1** and not
+            greater than **1000**.
 
         Phases:
             rewrite, access, header_filter, response, body_filter, log, admin_api
 
         Example:
             # Given a request GET /test?foo=hello%20world&bar=baz&zzz&blo=&bar=bla&bar
```

### Comparing `kong_pdk-0.33/kong_pdk/pdk/kong/response.py` & `kong_pdk-0.34/kong_pdk/pdk/kong/response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED BASED ON Kong 3.2.x, DO NOT EDIT
+# AUTO GENERATED BASED ON Kong 3.4.x, DO NOT EDIT
 # Original source path: kong/pdk/response.lua
 
 from typing import TypeVar, Any, Union, List, Mapping, Tuple, Optional
 
 number = TypeVar('number', int, float)
 table = TypeVar('table', List[Any], Mapping[str, Any])
 # XXX
@@ -296,17 +296,18 @@
             A response initially has no headers. Headers are added when a plugin
             short-circuits the proxying by producing a header
             (e.g. an authentication plugin rejecting a request), or if the request has
             been proxied, and one of the latter execution phases is currently running.
             Unlike `kong.service.response.get_headers()`, this function returns *all*
             headers as the client would see them upon reception, including headers
             added by Kong itself.
-            By default, this function returns up to **100** headers. The optional
-            `max_headers` argument can be specified to customize this limit, but must
-            be greater than **1** and equal to or less than **1000**.
+            By default, this function returns up to **100** headers (or what has been
+            configured using `lua_max_resp_headers`). The optional `max_headers` argument
+            can be specified to customize this limit, but must be greater than **1** and
+            equal to or less than **1000**.
 
         Phases:
             header_filter, response, body_filter, log, admin_api
 
         Example:
             # Given an response from the Service with the following headers:
```

### Comparing `kong_pdk-0.33/kong_pdk/pdk/kong/router.py` & `kong_pdk-0.34/kong_pdk/pdk/kong/router.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED BASED ON Kong 3.2.x, DO NOT EDIT
+# AUTO GENERATED BASED ON Kong 3.4.x, DO NOT EDIT
 # Original source path: kong/pdk/router.lua
 
 from typing import TypeVar, Any, Union, List, Mapping, Tuple, Optional
 
 number = TypeVar('number', int, float)
 table = TypeVar('table', List[Any], Mapping[str, Any])
 # XXX
```

### Comparing `kong_pdk-0.33/kong_pdk/pdk/kong/service/__init__.py` & `kong_pdk-0.34/kong_pdk/pdk/kong/service/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED BASED ON Kong 3.2.x, DO NOT EDIT
+# AUTO GENERATED BASED ON Kong 3.4.x, DO NOT EDIT
 # Original source path: kong/pdk/service.lua
 
 from typing import TypeVar, Any, Union, List, Mapping, Tuple, Optional
 
 number = TypeVar('number', int, float)
 table = TypeVar('table', List[Any], Mapping[str, Any])
 # XXX
```

### Comparing `kong_pdk-0.33/kong_pdk/pdk/kong/service/request.py` & `kong_pdk-0.34/kong_pdk/pdk/kong/service/request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED BASED ON Kong 3.2.x, DO NOT EDIT
+# AUTO GENERATED BASED ON Kong 3.4.x, DO NOT EDIT
 # Original source path: kong/pdk/service/request.lua
 
 from typing import TypeVar, Any, Union, List, Mapping, Tuple, Optional
 
 number = TypeVar('number', int, float)
 table = TypeVar('table', List[Any], Mapping[str, Any])
 # XXX
```

### Comparing `kong_pdk-0.33/kong_pdk/pdk/kong/service/response.py` & `kong_pdk-0.34/kong_pdk/pdk/kong/service/response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED BASED ON Kong 3.2.x, DO NOT EDIT
+# AUTO GENERATED BASED ON Kong 3.4.x, DO NOT EDIT
 # Original source path: kong/pdk/service/response.lua
 
 from typing import TypeVar, Any, Union, List, Mapping, Tuple, Optional
 
 number = TypeVar('number', int, float)
 table = TypeVar('table', List[Any], Mapping[str, Any])
 # XXX
@@ -31,15 +31,15 @@
 
         :parameter mimetype: The MIME type of the response (if known).
         :type mimetype: str
         :parameter max_args: Sets a limit on the maximum number of (what?)
             that can be parsed.
         :type max_args: number
 
-        :return: The raw buffered body
+        :return: The decoded buffered body
 
         :rtype: str
         """
         pass
 
     @staticmethod
     def get_header(name: str) -> str:
```

### Comparing `kong_pdk-0.33/kong_pdk/server.py` & `kong_pdk-0.34/kong_pdk/server.py`

 * *Files identical despite different names*

### Comparing `kong_pdk-0.33/kong_pdk.egg-info/PKG-INFO` & `kong_pdk-0.34/kong_pdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kong-pdk
-Version: 0.33
+Version: 0.34
 Summary: Kong PDK for Python and Plugin Server
 Home-page: https://github.com/Kong/kong-python-pdk
 Author: Kong
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
@@ -105,16 +105,16 @@
 - Hot reload
 
 
 <a name="unreleased"></a>
 ## [Unreleased]
 
 
-<a name="0.3.3"></a>
-## [0.3.3] - 2023-02-01
+<a name="0.3.4"></a>
+## [0.3.4] - 2023-06-20
 
 <a name="0.3.2"></a>
 ## [0.3.2] - 2022-11-08
 ### bug fixes
 - add version field in PluginInfo rpc ([#79](https://github.com/Kong/kong-python-pdk/issues/79)) [132f31d](https://github.com/Kong/kong-python-pdk/commit/132f31d526ff3589ac9b93dc079adb18359519cd)
 
 
@@ -216,16 +216,16 @@
 
 <a name="0.1.1"></a>
 ## [0.1.1] - 2020-02-20
 
 <a name="0.1.0"></a>
 ## 0.1.0 - 2020-01-03
 
-[Unreleased]: https://github.com/Kong/kong-python-pdk/compare/0.3.3...HEAD
-[0.3.3]: https://github.com/Kong/kong-python-pdk/compare/0.3.2...0.3.3
+[Unreleased]: https://github.com/Kong/kong-python-pdk/compare/0.3.4...HEAD
+[0.3.4]: https://github.com/Kong/kong-python-pdk/compare/0.3.2...0.3.4
 [0.3.2]: https://github.com/Kong/kong-python-pdk/compare/0.3.1...0.3.2
 [0.3.1]: https://github.com/Kong/kong-python-pdk/compare/0.3.0...0.3.1
 [0.3.0]: https://github.com/Kong/kong-python-pdk/compare/0.2.7...0.3.0
 [0.2.7]: https://github.com/Kong/kong-python-pdk/compare/0.2.6...0.2.7
 [0.2.6]: https://github.com/Kong/kong-python-pdk/compare/0.2.5...0.2.6
 [0.2.5]: https://github.com/Kong/kong-python-pdk/compare/0.2.4...0.2.5
 [0.2.4]: https://github.com/Kong/kong-python-pdk/compare/0.2.3...0.2.4
```

### Comparing `kong_pdk-0.33/kong_pdk.egg-info/SOURCES.txt` & `kong_pdk-0.34/kong_pdk.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 kong_pdk.egg-info/top_level.txt
 kong_pdk/pdk/__init__.py
 kong_pdk/pdk/kong/__init__.py
 kong_pdk/pdk/kong/cluster.py
 kong_pdk/pdk/kong/ip.py
 kong_pdk/pdk/kong/log.py
 kong_pdk/pdk/kong/node.py
+kong_pdk/pdk/kong/plugin.py
 kong_pdk/pdk/kong/request.py
 kong_pdk/pdk/kong/response.py
 kong_pdk/pdk/kong/router.py
 kong_pdk/pdk/kong/vault.py
 kong_pdk/pdk/kong/client/__init__.py
 kong_pdk/pdk/kong/client/tls.py
 kong_pdk/pdk/kong/ctx/__init__.py
```

### Comparing `kong_pdk-0.33/setup.py` & `kong_pdk-0.34/setup.py`

 * *Files identical despite different names*

