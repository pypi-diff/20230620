# Comparing `tmp/networkcalculator-1.0.4.tar.gz` & `tmp/networkcalculator-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "networkcalculator-1.0.4.tar", last modified: Mon Jun 19 23:19:16 2023, max compression
+gzip compressed data, was "networkcalculator-1.0.5.tar", last modified: Tue Jun 20 00:54:20 2023, max compression
```

## Comparing `networkcalculator-1.0.4.tar` & `networkcalculator-1.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:16.073254 networkcalculator-1.0.4/
--rw-rw-rw-   0        0        0     1094 2023-06-18 18:29:24.000000 networkcalculator-1.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0     7599 2023-06-19 23:19:16.073254 networkcalculator-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     5522 2023-06-19 17:38:05.000000 networkcalculator-1.0.4/README.md
--rw-rw-rw-   0        0        0       86 2023-06-19 14:18:05.000000 networkcalculator-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0      815 2023-06-19 23:19:16.074254 networkcalculator-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      785 2023-06-19 23:18:54.000000 networkcalculator-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:16.052252 networkcalculator-1.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:16.062254 networkcalculator-1.0.4/src/cidr/
--rw-rw-rw-   0        0        0        0 2023-06-19 14:01:58.000000 networkcalculator-1.0.4/src/cidr/__init__.py
--rw-rw-rw-   0        0        0     5179 2023-06-19 17:28:02.000000 networkcalculator-1.0.4/src/cidr/network_calculator.py
--rw-rw-rw-   0        0        0     1140 2023-06-19 15:39:01.000000 networkcalculator-1.0.4/src/cidr/network_calculator_test.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:16.066254 networkcalculator-1.0.4/src/feeds/
--rw-rw-rw-   0        0        0        0 2023-06-19 14:01:58.000000 networkcalculator-1.0.4/src/feeds/__init__.py
--rw-rw-rw-   0        0        0     8814 2023-06-19 18:02:12.000000 networkcalculator-1.0.4/src/feeds/bandwidth_calculator.py
--rw-rw-rw-   0        0        0     3333 2023-06-19 18:05:24.000000 networkcalculator-1.0.4/src/feeds/bandwidth_calculator_test.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:16.069254 networkcalculator-1.0.4/src/networkcalculator.egg-info/
--rw-rw-rw-   0        0        0     7599 2023-06-19 23:19:16.000000 networkcalculator-1.0.4/src/networkcalculator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      511 2023-06-19 23:19:16.000000 networkcalculator-1.0.4/src/networkcalculator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 23:19:16.000000 networkcalculator-1.0.4/src/networkcalculator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-19 23:19:16.000000 networkcalculator-1.0.4/src/networkcalculator.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 23:19:16.072254 networkcalculator-1.0.4/src/tests/
--rw-rw-rw-   0        0        0        0 2023-06-19 14:02:58.000000 networkcalculator-1.0.4/src/tests/__init__.py
--rw-rw-rw-   0        0        0     3333 2023-06-19 18:05:24.000000 networkcalculator-1.0.4/src/tests/bandwidth_calculator_test.py
--rw-rw-rw-   0        0        0     5179 2023-06-19 19:19:05.000000 networkcalculator-1.0.4/src/tests/network_calculator.py
+drwxrwxrwx   0        0        0        0 2023-06-20 00:54:20.446854 networkcalculator-1.0.5/
+-rw-rw-rw-   0        0        0     1094 2023-06-18 18:29:24.000000 networkcalculator-1.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     8400 2023-06-20 00:54:20.447855 networkcalculator-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6323 2023-06-20 00:40:06.000000 networkcalculator-1.0.5/README.md
+-rw-rw-rw-   0        0        0       86 2023-06-19 14:18:05.000000 networkcalculator-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0      815 2023-06-20 00:54:20.448853 networkcalculator-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      785 2023-06-20 00:14:00.000000 networkcalculator-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 00:54:20.425895 networkcalculator-1.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-06-20 00:54:20.434895 networkcalculator-1.0.5/src/cidr/
+-rw-rw-rw-   0        0        0        0 2023-06-19 14:01:58.000000 networkcalculator-1.0.5/src/cidr/__init__.py
+-rw-rw-rw-   0        0        0     5179 2023-06-19 17:28:02.000000 networkcalculator-1.0.5/src/cidr/network_calculator.py
+-rw-rw-rw-   0        0        0     1140 2023-06-19 15:39:01.000000 networkcalculator-1.0.5/src/cidr/network_calculator_test.py
+drwxrwxrwx   0        0        0        0 2023-06-20 00:54:20.438959 networkcalculator-1.0.5/src/feeds/
+-rw-rw-rw-   0        0        0        0 2023-06-19 14:01:58.000000 networkcalculator-1.0.5/src/feeds/__init__.py
+-rw-rw-rw-   0        0        0     8814 2023-06-19 18:02:12.000000 networkcalculator-1.0.5/src/feeds/bandwidth_calculator.py
+-rw-rw-rw-   0        0        0     3333 2023-06-19 18:05:24.000000 networkcalculator-1.0.5/src/feeds/bandwidth_calculator_test.py
+drwxrwxrwx   0        0        0        0 2023-06-20 00:54:20.442854 networkcalculator-1.0.5/src/networkcalculator.egg-info/
+-rw-rw-rw-   0        0        0     8400 2023-06-20 00:54:20.000000 networkcalculator-1.0.5/src/networkcalculator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      511 2023-06-20 00:54:20.000000 networkcalculator-1.0.5/src/networkcalculator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 00:54:20.000000 networkcalculator-1.0.5/src/networkcalculator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-20 00:54:20.000000 networkcalculator-1.0.5/src/networkcalculator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 00:54:20.445853 networkcalculator-1.0.5/src/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-19 14:02:58.000000 networkcalculator-1.0.5/src/tests/__init__.py
+-rw-rw-rw-   0        0        0     3333 2023-06-19 18:05:24.000000 networkcalculator-1.0.5/src/tests/bandwidth_calculator_test.py
+-rw-rw-rw-   0        0        0     5179 2023-06-19 19:19:05.000000 networkcalculator-1.0.5/src/tests/network_calculator.py
```

### Comparing `networkcalculator-1.0.4/LICENSE.txt` & `networkcalculator-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `networkcalculator-1.0.4/PKG-INFO` & `networkcalculator-1.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: networkcalculator
-Version: 1.0.4
+Version: 1.0.5
 Summary: A network calculator package
 Home-page: https://gitlab.com/raymodbernard/networkcalculator
 Author: Ray Bernard
 Author-email: ray.bernard@outlook.com
 Project-URL: Bug Tracker, https://gitlab.com/raymodbernard/networkcalculator/issues
 Project-URL: repository, https://gitlab.com/raymodbernard/networkcalculator
 Classifier: Development Status :: 3 - Alpha
@@ -20,14 +20,15 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Network Calculator
 
 ### The What and Why of Network Calculations
+
 In networking, IP addresses and subnet masks are crucial for defining the structure and reach of the network. However, doing these calculations manually can be cumbersome and error-prone. This is where Python, with its vast library support and simplicity, can be a lifesaver.
 
 In this article, we'll delve into a Python class called I have created called the 'NetworkCalculator'. It is designed to automate common network calculation tasks. To fully understand this, it is recommended you have some basic knowledge of IP addresses, subnet masks, network IDs, broadcast IDs, and CIDR notation. There are a tone of online resources to help your understanding. 
 
 The NetworkCalculator class is initialized with an IP address in CIDR notation as input. CIDR (Classless Inter-Domain Routing) notation represents an IP address and its associated routing prefix. 
 
 For instance, '192.168.1.10/24' is an example of an IP address in CIDR notation.
@@ -49,25 +50,26 @@
 get_first_ip(): Returns the first usable IP address in the network. It's simply the Network ID plus one.
 
 get_last_ip(): Returns the last usable IP address in the network, which is one less than the broadcast ID.
 
 get_total_ips(): Returns the total number of usable IP addresses in the network.
 ```
 
+## Installation
 ```python
 
 pip install networkcalculator
 
 ```
 
 
 ### how to use the code 
 ```python 
 
-from cidr.networkcalculator  import Network_Calculator
+from cidr.network_calculator  import Network_Calculator
 
 # Use it like this:
 ip_list = ['198.51.100.0/22 ', '192.168.1.10/26', '172.16.0.5/16']
 
 # Call the function with the list of CIDR IP addresses
 Network_Calculator.print_network_info(ip_list)
 
@@ -82,42 +84,43 @@
 | --------------- | --------------- | ------------ | ------------ | -------------- | ------------ | -------------- | --------- |
 | 198.51.100.0/22 | 255.255.252.0   | 198.51.100.0 | 198.51.104.0 | 198.51.103.255 | 198.51.100.1 | 198.51.103.254 | 1022      |
 | 192.168.1.10/26 | 255.255.255.192 | 192.168.1.0  | 192.168.1.64 | 192.168.1.63   | 192.168.1.1  | 192.168.1.62   | 62        |
 | 172.16.0.5/16   | 255.255.0.0     | 172.16.0.0   | 172.17.0.0   | 172.16.255.255 | 172.16.0.1   | 172.16.255.254 | 65534     |
 |                 |                 |              |              |                |              |                |           |
 
 ### Bandwidth Calculator  
+In an era where data is being transferred in vast amounts and at high speeds, understanding bandwidth needs and capacity is an essential aspect of network management and application performance. A Bandwidth Calculator is a tool that helps you estimate the bandwidth needed to move a specific amount of data within a specific timeframe. In this article, we will delve into a Python code that creates a Bandwidth Calculator, designed to help you predict your bandwidth needs accurately.
+
+The Bandwidth Calculator we are focusing on takes in four parameters: the throughput, the read percentage, the write percentage, and the initial data size. The Bandwidth Calculator is instantiated from the Bandwidth_Calculator class from the feeds.bandwidth_calculator module
 
 ```python
 from feeds.bandwidth_calculator import Bandwidth_Calculator
 
-
 # Create a BandwidthCalculator object
 
-bc = Bandwidth_Calculator('1 Gbps', 50, 50, '1 TB') # thoughtput , reads %, writes /%, Initial data size 
+bc = Bandwidth_Calculator('1 Gbps', 50, 50, '1 TB') # Throughput , reads %, writes /%, Initial data size 
 
 # Write the results to a CSV file
 bc.write_to_csv('feeds.csv')
 
-
 ```
 
+
+### Output 
+
 | Media Throughput | Read/Write Ratio | Initial Data Size | Disk Space Required (Read) | Disk Space Required (Write) | Bandwidth Required (Read) | Bandwidth Required (Write) | Transfer Time                           |
 | ---------------- | ---------------- | ----------------- | -------------------------- | --------------------------- | ------------------------- | -------------------------- | --------------------------------------- |
 | 1.0 Gbps         | 50:50            | 1.0 TB            | 62.5 MBps                  | 62.5 MBps                   | 500.0 Mbps                | 500.0 Mbps                 | 2 hours 13 minutes 20.0 seconds seconds |
 |                  |                  |                   |                            |                             |                           |                            |                                         |
 
 
 
-
-
-
-
 ### About: 
-Ray Bernard is a seasoned technologist specializing in cloud-based platforms, data science, and AI. He co-founded SuprFanz, a revolutionary cloud-based marketing company, and has held key roles at EMC, Ticket Master, and Compaq. As an Affiliate Developer, Systems Engineer, and Community Advocate, he demonstrated exceptional technical prowess and innovative thinking. Ray also taught Internet/Intranet Management & Design at Columbia University, further contributing to the field. With his vast experience and proactive problem-solving approach, he consistently drives digital transformation. 
+Ray Bernard is a seasoned technologist specializing in cloud-based platforms, data science, and AI. He co-founded SuprFanz, a revolutionary cloud-based marketing company, and has held key roles at EMC, Dell, and Compaq/Dec. As an Affiliate Developer at Ticketmast, Systems Engineer, and Community Advocate, he demonstrated exceptional technical prowess and innovative thinking. Ray also taught Internet/Intranet Management & Design at Columbia University, further contributing to the field. With his vast experience and proactive problem-solving approach, he consistently drives digital transformation. 
+
 Contact him: ray.bernard@outlook.com 
 LinkedIn : https://www.linkedin.com/in/ray-bernard-960382/
 Git : https://github.com/raymondbernard/
 MIT License
 
 Copyright (c) 2023 Raymond Bernard
```

### Comparing `networkcalculator-1.0.4/README.md` & `networkcalculator-1.0.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Network Calculator
 
 ### The What and Why of Network Calculations
+
 In networking, IP addresses and subnet masks are crucial for defining the structure and reach of the network. However, doing these calculations manually can be cumbersome and error-prone. This is where Python, with its vast library support and simplicity, can be a lifesaver.
 
 In this article, we'll delve into a Python class called I have created called the 'NetworkCalculator'. It is designed to automate common network calculation tasks. To fully understand this, it is recommended you have some basic knowledge of IP addresses, subnet masks, network IDs, broadcast IDs, and CIDR notation. There are a tone of online resources to help your understanding. 
 
 The NetworkCalculator class is initialized with an IP address in CIDR notation as input. CIDR (Classless Inter-Domain Routing) notation represents an IP address and its associated routing prefix. 
 
 For instance, '192.168.1.10/24' is an example of an IP address in CIDR notation.
@@ -26,25 +27,26 @@
 get_first_ip(): Returns the first usable IP address in the network. It's simply the Network ID plus one.
 
 get_last_ip(): Returns the last usable IP address in the network, which is one less than the broadcast ID.
 
 get_total_ips(): Returns the total number of usable IP addresses in the network.
 ```
 
+## Installation
 ```python
 
 pip install networkcalculator
 
 ```
 
 
 ### how to use the code 
 ```python 
 
-from cidr.networkcalculator  import Network_Calculator
+from cidr.network_calculator  import Network_Calculator
 
 # Use it like this:
 ip_list = ['198.51.100.0/22 ', '192.168.1.10/26', '172.16.0.5/16']
 
 # Call the function with the list of CIDR IP addresses
 Network_Calculator.print_network_info(ip_list)
 
@@ -59,38 +61,39 @@
 | --------------- | --------------- | ------------ | ------------ | -------------- | ------------ | -------------- | --------- |
 | 198.51.100.0/22 | 255.255.252.0   | 198.51.100.0 | 198.51.104.0 | 198.51.103.255 | 198.51.100.1 | 198.51.103.254 | 1022      |
 | 192.168.1.10/26 | 255.255.255.192 | 192.168.1.0  | 192.168.1.64 | 192.168.1.63   | 192.168.1.1  | 192.168.1.62   | 62        |
 | 172.16.0.5/16   | 255.255.0.0     | 172.16.0.0   | 172.17.0.0   | 172.16.255.255 | 172.16.0.1   | 172.16.255.254 | 65534     |
 |                 |                 |              |              |                |              |                |           |
 
 ### Bandwidth Calculator  
+In an era where data is being transferred in vast amounts and at high speeds, understanding bandwidth needs and capacity is an essential aspect of network management and application performance. A Bandwidth Calculator is a tool that helps you estimate the bandwidth needed to move a specific amount of data within a specific timeframe. In this article, we will delve into a Python code that creates a Bandwidth Calculator, designed to help you predict your bandwidth needs accurately.
+
+The Bandwidth Calculator we are focusing on takes in four parameters: the throughput, the read percentage, the write percentage, and the initial data size. The Bandwidth Calculator is instantiated from the Bandwidth_Calculator class from the feeds.bandwidth_calculator module
 
 ```python
 from feeds.bandwidth_calculator import Bandwidth_Calculator
 
-
 # Create a BandwidthCalculator object
 
-bc = Bandwidth_Calculator('1 Gbps', 50, 50, '1 TB') # thoughtput , reads %, writes /%, Initial data size 
+bc = Bandwidth_Calculator('1 Gbps', 50, 50, '1 TB') # Throughput , reads %, writes /%, Initial data size 
 
 # Write the results to a CSV file
 bc.write_to_csv('feeds.csv')
 
-
 ```
 
+
+### Output 
+
 | Media Throughput | Read/Write Ratio | Initial Data Size | Disk Space Required (Read) | Disk Space Required (Write) | Bandwidth Required (Read) | Bandwidth Required (Write) | Transfer Time                           |
 | ---------------- | ---------------- | ----------------- | -------------------------- | --------------------------- | ------------------------- | -------------------------- | --------------------------------------- |
 | 1.0 Gbps         | 50:50            | 1.0 TB            | 62.5 MBps                  | 62.5 MBps                   | 500.0 Mbps                | 500.0 Mbps                 | 2 hours 13 minutes 20.0 seconds seconds |
 |                  |                  |                   |                            |                             |                           |                            |                                         |
 
 
 
-
-
-
-
 ### About: 
-Ray Bernard is a seasoned technologist specializing in cloud-based platforms, data science, and AI. He co-founded SuprFanz, a revolutionary cloud-based marketing company, and has held key roles at EMC, Ticket Master, and Compaq. As an Affiliate Developer, Systems Engineer, and Community Advocate, he demonstrated exceptional technical prowess and innovative thinking. Ray also taught Internet/Intranet Management & Design at Columbia University, further contributing to the field. With his vast experience and proactive problem-solving approach, he consistently drives digital transformation. 
+Ray Bernard is a seasoned technologist specializing in cloud-based platforms, data science, and AI. He co-founded SuprFanz, a revolutionary cloud-based marketing company, and has held key roles at EMC, Dell, and Compaq/Dec. As an Affiliate Developer at Ticketmast, Systems Engineer, and Community Advocate, he demonstrated exceptional technical prowess and innovative thinking. Ray also taught Internet/Intranet Management & Design at Columbia University, further contributing to the field. With his vast experience and proactive problem-solving approach, he consistently drives digital transformation. 
+
 Contact him: ray.bernard@outlook.com 
 LinkedIn : https://www.linkedin.com/in/ray-bernard-960382/
 Git : https://github.com/raymondbernard/
```

### Comparing `networkcalculator-1.0.4/setup.cfg` & `networkcalculator-1.0.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206e 6574 776f 726b 6361 6c63 756c   = networkcalcul
 00000020: 6174 6f72 0d0a 7665 7273 696f 6e20 3d20  ator..version = 
-00000030: 312e 302e 340d 0a61 7574 686f 7220 3d20  1.0.4..author = 
+00000030: 312e 302e 350d 0a61 7574 686f 7220 3d20  1.0.5..author = 
 00000040: 5261 7920 4265 726e 6172 640d 0a61 7574  Ray Bernard..aut
 00000050: 686f 725f 656d 6169 6c20 3d20 7261 792e  hor_email = ray.
 00000060: 6265 726e 6172 6440 6f75 746c 6f6f 6b2e  bernard@outlook.
 00000070: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
 00000080: 203d 2054 6f6f 6c20 746f 2067 656e 6572   = Tool to gener
 00000090: 6174 6520 6e65 7477 6f72 6b20 6261 7365  ate network base
 000000a0: 6420 6f6e 2043 4944 5220 616e 6420 7370  d on CIDR and sp
```

### Comparing `networkcalculator-1.0.4/setup.py` & `networkcalculator-1.0.5/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='networkcalculator',
-    version='1.0.4',
+    version='1.0.5',
     author='Ray Bernard',
     author_email='ray.bernard@outlook.com',
     description='A network calculator package',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```

### Comparing `networkcalculator-1.0.4/src/cidr/network_calculator.py` & `networkcalculator-1.0.5/src/cidr/network_calculator.py`

 * *Files identical despite different names*

### Comparing `networkcalculator-1.0.4/src/cidr/network_calculator_test.py` & `networkcalculator-1.0.5/src/cidr/network_calculator_test.py`

 * *Files identical despite different names*

### Comparing `networkcalculator-1.0.4/src/feeds/bandwidth_calculator.py` & `networkcalculator-1.0.5/src/feeds/bandwidth_calculator.py`

 * *Files identical despite different names*

### Comparing `networkcalculator-1.0.4/src/feeds/bandwidth_calculator_test.py` & `networkcalculator-1.0.5/src/feeds/bandwidth_calculator_test.py`

 * *Files identical despite different names*

### Comparing `networkcalculator-1.0.4/src/networkcalculator.egg-info/PKG-INFO` & `networkcalculator-1.0.5/src/networkcalculator.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: networkcalculator
-Version: 1.0.4
+Version: 1.0.5
 Summary: A network calculator package
 Home-page: https://gitlab.com/raymodbernard/networkcalculator
 Author: Ray Bernard
 Author-email: ray.bernard@outlook.com
 Project-URL: Bug Tracker, https://gitlab.com/raymodbernard/networkcalculator/issues
 Project-URL: repository, https://gitlab.com/raymodbernard/networkcalculator
 Classifier: Development Status :: 3 - Alpha
@@ -20,14 +20,15 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Network Calculator
 
 ### The What and Why of Network Calculations
+
 In networking, IP addresses and subnet masks are crucial for defining the structure and reach of the network. However, doing these calculations manually can be cumbersome and error-prone. This is where Python, with its vast library support and simplicity, can be a lifesaver.
 
 In this article, we'll delve into a Python class called I have created called the 'NetworkCalculator'. It is designed to automate common network calculation tasks. To fully understand this, it is recommended you have some basic knowledge of IP addresses, subnet masks, network IDs, broadcast IDs, and CIDR notation. There are a tone of online resources to help your understanding. 
 
 The NetworkCalculator class is initialized with an IP address in CIDR notation as input. CIDR (Classless Inter-Domain Routing) notation represents an IP address and its associated routing prefix. 
 
 For instance, '192.168.1.10/24' is an example of an IP address in CIDR notation.
@@ -49,25 +50,26 @@
 get_first_ip(): Returns the first usable IP address in the network. It's simply the Network ID plus one.
 
 get_last_ip(): Returns the last usable IP address in the network, which is one less than the broadcast ID.
 
 get_total_ips(): Returns the total number of usable IP addresses in the network.
 ```
 
+## Installation
 ```python
 
 pip install networkcalculator
 
 ```
 
 
 ### how to use the code 
 ```python 
 
-from cidr.networkcalculator  import Network_Calculator
+from cidr.network_calculator  import Network_Calculator
 
 # Use it like this:
 ip_list = ['198.51.100.0/22 ', '192.168.1.10/26', '172.16.0.5/16']
 
 # Call the function with the list of CIDR IP addresses
 Network_Calculator.print_network_info(ip_list)
 
@@ -82,42 +84,43 @@
 | --------------- | --------------- | ------------ | ------------ | -------------- | ------------ | -------------- | --------- |
 | 198.51.100.0/22 | 255.255.252.0   | 198.51.100.0 | 198.51.104.0 | 198.51.103.255 | 198.51.100.1 | 198.51.103.254 | 1022      |
 | 192.168.1.10/26 | 255.255.255.192 | 192.168.1.0  | 192.168.1.64 | 192.168.1.63   | 192.168.1.1  | 192.168.1.62   | 62        |
 | 172.16.0.5/16   | 255.255.0.0     | 172.16.0.0   | 172.17.0.0   | 172.16.255.255 | 172.16.0.1   | 172.16.255.254 | 65534     |
 |                 |                 |              |              |                |              |                |           |
 
 ### Bandwidth Calculator  
+In an era where data is being transferred in vast amounts and at high speeds, understanding bandwidth needs and capacity is an essential aspect of network management and application performance. A Bandwidth Calculator is a tool that helps you estimate the bandwidth needed to move a specific amount of data within a specific timeframe. In this article, we will delve into a Python code that creates a Bandwidth Calculator, designed to help you predict your bandwidth needs accurately.
+
+The Bandwidth Calculator we are focusing on takes in four parameters: the throughput, the read percentage, the write percentage, and the initial data size. The Bandwidth Calculator is instantiated from the Bandwidth_Calculator class from the feeds.bandwidth_calculator module
 
 ```python
 from feeds.bandwidth_calculator import Bandwidth_Calculator
 
-
 # Create a BandwidthCalculator object
 
-bc = Bandwidth_Calculator('1 Gbps', 50, 50, '1 TB') # thoughtput , reads %, writes /%, Initial data size 
+bc = Bandwidth_Calculator('1 Gbps', 50, 50, '1 TB') # Throughput , reads %, writes /%, Initial data size 
 
 # Write the results to a CSV file
 bc.write_to_csv('feeds.csv')
 
-
 ```
 
+
+### Output 
+
 | Media Throughput | Read/Write Ratio | Initial Data Size | Disk Space Required (Read) | Disk Space Required (Write) | Bandwidth Required (Read) | Bandwidth Required (Write) | Transfer Time                           |
 | ---------------- | ---------------- | ----------------- | -------------------------- | --------------------------- | ------------------------- | -------------------------- | --------------------------------------- |
 | 1.0 Gbps         | 50:50            | 1.0 TB            | 62.5 MBps                  | 62.5 MBps                   | 500.0 Mbps                | 500.0 Mbps                 | 2 hours 13 minutes 20.0 seconds seconds |
 |                  |                  |                   |                            |                             |                           |                            |                                         |
 
 
 
-
-
-
-
 ### About: 
-Ray Bernard is a seasoned technologist specializing in cloud-based platforms, data science, and AI. He co-founded SuprFanz, a revolutionary cloud-based marketing company, and has held key roles at EMC, Ticket Master, and Compaq. As an Affiliate Developer, Systems Engineer, and Community Advocate, he demonstrated exceptional technical prowess and innovative thinking. Ray also taught Internet/Intranet Management & Design at Columbia University, further contributing to the field. With his vast experience and proactive problem-solving approach, he consistently drives digital transformation. 
+Ray Bernard is a seasoned technologist specializing in cloud-based platforms, data science, and AI. He co-founded SuprFanz, a revolutionary cloud-based marketing company, and has held key roles at EMC, Dell, and Compaq/Dec. As an Affiliate Developer at Ticketmast, Systems Engineer, and Community Advocate, he demonstrated exceptional technical prowess and innovative thinking. Ray also taught Internet/Intranet Management & Design at Columbia University, further contributing to the field. With his vast experience and proactive problem-solving approach, he consistently drives digital transformation. 
+
 Contact him: ray.bernard@outlook.com 
 LinkedIn : https://www.linkedin.com/in/ray-bernard-960382/
 Git : https://github.com/raymondbernard/
 MIT License
 
 Copyright (c) 2023 Raymond Bernard
```

### Comparing `networkcalculator-1.0.4/src/tests/bandwidth_calculator_test.py` & `networkcalculator-1.0.5/src/tests/bandwidth_calculator_test.py`

 * *Files identical despite different names*

### Comparing `networkcalculator-1.0.4/src/tests/network_calculator.py` & `networkcalculator-1.0.5/src/tests/network_calculator.py`

 * *Files identical despite different names*

