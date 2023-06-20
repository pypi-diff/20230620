# Comparing `tmp/pingnet-0.4.3.tar.gz` & `tmp/pingnet-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pingnet-0.4.3.tar", last modified: Thu Feb 23 00:32:10 2023, max compression
+gzip compressed data, was "pingnet-0.4.4.tar", last modified: Tue Jun 20 21:52:28 2023, max compression
```

## Comparing `pingnet-0.4.3.tar` & `pingnet-0.4.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-02-23 00:32:10.674424 pingnet-0.4.3/
--rw-rw-rw-   0        0        0     1078 2022-07-07 06:31:11.000000 pingnet-0.4.3/LICENSE.txt
--rw-rw-rw-   0        0        0     9339 2023-02-23 00:32:10.675420 pingnet-0.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     7690 2022-07-18 20:37:50.000000 pingnet-0.4.3/README.md
-drwxrwxrwx   0        0        0        0 2023-02-23 00:32:10.673427 pingnet-0.4.3/pingnet.egg-info/
--rw-rw-rw-   0        0        0     9339 2023-02-23 00:32:10.000000 pingnet-0.4.3/pingnet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-02-23 00:32:10.000000 pingnet-0.4.3/pingnet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-23 00:32:10.000000 pingnet-0.4.3/pingnet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-02-23 00:32:10.000000 pingnet-0.4.3/pingnet.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        4 2023-02-23 00:32:10.000000 pingnet-0.4.3/pingnet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2022-07-07 06:30:09.000000 pingnet-0.4.3/pyproject.toml
--rw-rw-rw-   0        0        0      608 2023-02-23 00:32:10.675420 pingnet-0.4.3/setup.cfg
--rw-rw-rw-   0        0        0      195 2022-07-15 08:12:22.000000 pingnet-0.4.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-23 00:32:10.674424 pingnet-0.4.3/src/
--rw-rw-rw-   0        0        0        0 2022-07-15 08:14:19.000000 pingnet-0.4.3/src/__init__.py
--rw-rw-rw-   0        0        0     9729 2023-02-23 00:31:58.000000 pingnet-0.4.3/src/pingnet.py
+drwxrwxrwx   0        0        0        0 2023-06-20 21:52:28.087324 pingnet-0.4.4/
+-rw-rw-rw-   0        0        0     1078 2022-07-07 06:31:11.000000 pingnet-0.4.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     9339 2023-06-20 21:52:28.087324 pingnet-0.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     7690 2022-07-18 20:37:50.000000 pingnet-0.4.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 21:52:28.086322 pingnet-0.4.4/pingnet.egg-info/
+-rw-rw-rw-   0        0        0     9339 2023-06-20 21:52:28.000000 pingnet-0.4.4/pingnet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-06-20 21:52:28.000000 pingnet-0.4.4/pingnet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 21:52:28.000000 pingnet-0.4.4/pingnet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-06-20 21:52:28.000000 pingnet-0.4.4/pingnet.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        4 2023-06-20 21:52:28.000000 pingnet-0.4.4/pingnet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2022-07-07 06:30:09.000000 pingnet-0.4.4/pyproject.toml
+-rw-rw-rw-   0        0        0      608 2023-06-20 21:52:28.088315 pingnet-0.4.4/setup.cfg
+-rw-rw-rw-   0        0        0      195 2022-07-15 08:12:22.000000 pingnet-0.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 21:52:28.086322 pingnet-0.4.4/src/
+-rw-rw-rw-   0        0        0        0 2022-07-15 08:14:19.000000 pingnet-0.4.4/src/__init__.py
+-rw-rw-rw-   0        0        0     9785 2023-06-20 21:49:56.000000 pingnet-0.4.4/src/pingnet.py
```

### Comparing `pingnet-0.4.3/LICENSE.txt` & `pingnet-0.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pingnet-0.4.3/PKG-INFO` & `pingnet-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pingnet
-Version: 0.4.3
+Version: 0.4.4
 Summary: Script to ping network address(CIDR), IP address, hostname
 Home-page: https://github.com/skndmx/pingnet
 Author: Kevin Jin
 Author-email: skndmx@gmail.com
 Project-URL: Bug Tracker, https://github.com/skndmx/pingnet/issues
 Project-URL: repository, https://github.com/skndmx/pingnet
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pingnet-0.4.3/README.md` & `pingnet-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `pingnet-0.4.3/pingnet.egg-info/PKG-INFO` & `pingnet-0.4.4/pingnet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pingnet
-Version: 0.4.3
+Version: 0.4.4
 Summary: Script to ping network address(CIDR), IP address, hostname
 Home-page: https://github.com/skndmx/pingnet
 Author: Kevin Jin
 Author-email: skndmx@gmail.com
 Project-URL: Bug Tracker, https://github.com/skndmx/pingnet/issues
 Project-URL: repository, https://github.com/skndmx/pingnet
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pingnet-0.4.3/setup.cfg` & `pingnet-0.4.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 696e 676e 6574 0d0a 7665 7273   = pingnet..vers
-00000020: 696f 6e20 3d20 302e 342e 330d 0a61 7574  ion = 0.4.3..aut
+00000020: 696f 6e20 3d20 302e 342e 340d 0a61 7574  ion = 0.4.4..aut
 00000030: 686f 7220 3d20 4b65 7669 6e20 4a69 6e0d  hor = Kevin Jin.
 00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000050: 736b 6e64 6d78 4067 6d61 696c 2e63 6f6d  skndmx@gmail.com
 00000060: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000070: 5363 7269 7074 2074 6f20 7069 6e67 206e  Script to ping n
 00000080: 6574 776f 726b 2061 6464 7265 7373 2843  etwork address(C
 00000090: 4944 5229 2c20 4950 2061 6464 7265 7373  IDR), IP address
```

### Comparing `pingnet-0.4.3/src/pingnet.py` & `pingnet-0.4.4/src/pingnet.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from ipaddress import ip_address
 from sys import platform
 import concurrent.futures
 from threading import Thread
 if "darwin" in platform:
      import resource # pylint: disable=import-error
 
-version = "0.4.3"
+version = "0.4.4"
 alive = []                              #Empty list to collect reachable hosts
 alive_avg = []                          #Empty list to collect reachable hosts + RTT
 dead = []                          #Empty list to collect unreachable hosts
 unknown = []                           #Empty list to collect Unknown hosts
 
 os.system("")
 
@@ -152,31 +152,34 @@
                     else:
                         totalAddress += 1
                         thread_list.append(executor.submit(ping_all, IP))
         for th in concurrent.futures.as_completed(thread_list):
             th.result()
 
     if args.address:
-        if "/" in args.address:                     #If Address has subnet mask symbol(/), eg: 192.168.1.0/30
-            if ipaddress.ip_network(args.address):  #validate if it's a CIDR network
+        if "/" in args.address:  # If Address has subnet mask symbol(/), eg: 192.168.1.0/30
+            try: 
+                network = ipaddress.IPv4Network(args.address, strict=False)  # validate if it's a CIDR network
 
                 totalAddress = 0
                 max_threads = 1024  # Set maximum number of threads to 10
                 ip_list = []
 
-                for ip in ipaddress.IPv4Network(args.address, False):
+                for ip in network:
                     ip_list.append(str(ip))
                     totalAddress += 1
 
                 def ping_test_wrapper(ip_address):
                     ping_test(ip_address, ping_count)
 
                 with concurrent.futures.ThreadPoolExecutor(max_workers=max_threads) as executor:
                     executor.map(ping_test_wrapper, ip_list)
-        else:                             #Single IP address or hostname, instead of IP range
+            except ValueError as e:
+                print(f"Invalid CIDR address: {e}")
+        else:  # Single IP address or hostname, instead of IP range
             totalAddress += 1
             ping_test(args.address,ping_count)
 
     time_elapsed = time.time() - start_time            #calculate elapsed time
     print("-------------------------------------------------------------------------------------")
     print("{0:55} Time elapsed:{1:>8.2f} seconds\n".format("Number of total addresses: "+str(totalAddress),time_elapsed))
     alive_sorted = sorted(alive, key=ipsorter)
```

