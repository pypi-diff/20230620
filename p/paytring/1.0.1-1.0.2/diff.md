# Comparing `tmp/paytring-1.0.1.tar.gz` & `tmp/paytring-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paytring-1.0.1.tar", last modified: Wed Jun 14 12:23:37 2023, max compression
+gzip compressed data, was "paytring-1.0.2.tar", last modified: Tue Jun 20 07:52:54 2023, max compression
```

## Comparing `paytring-1.0.1.tar` & `paytring-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 12:23:37.441696 paytring-1.0.1/
--rw-rw-rw-   0        0        0     1094 2023-06-14 07:35:06.000000 paytring-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     5098 2023-06-14 12:23:37.441696 paytring-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-14 12:23:37.397946 paytring-1.0.1/Paytring/
-drwxrwxrwx   0        0        0        0 2023-06-14 12:23:37.411419 paytring-1.0.1/Paytring/paytring/
--rw-rw-rw-   0        0        0      113 2023-06-02 11:09:08.000000 paytring-1.0.1/Paytring/paytring/__init__.py
--rw-rw-rw-   0        0        0     5066 2023-06-14 10:38:20.000000 paytring-1.0.1/Paytring/paytring/client.py
-drwxrwxrwx   0        0        0        0 2023-06-14 12:23:37.430262 paytring-1.0.1/Paytring/paytring/constant/
--rw-rw-rw-   0        0        0       52 2023-06-02 12:35:28.000000 paytring-1.0.1/Paytring/paytring/constant/__init__.py
--rw-rw-rw-   0        0        0      338 2023-06-14 10:54:48.000000 paytring-1.0.1/Paytring/paytring/constant/url.py
-drwxrwxrwx   0        0        0        0 2023-06-14 12:23:37.433202 paytring-1.0.1/Paytring/paytring/resources/
--rw-rw-rw-   0        0        0       69 2023-06-02 12:35:26.000000 paytring-1.0.1/Paytring/paytring/resources/__init__.py
--rw-rw-rw-   0        0        0      337 2023-06-14 10:54:33.000000 paytring-1.0.1/Paytring/paytring/resources/paytring.py
-drwxrwxrwx   0        0        0        0 2023-06-14 12:23:37.437939 paytring-1.0.1/Paytring/paytring/utility/
--rw-rw-rw-   0        0        0       66 2023-06-02 12:35:13.000000 paytring-1.0.1/Paytring/paytring/utility/__init__.py
--rw-rw-rw-   0        0        0     2638 2023-06-14 10:54:41.000000 paytring-1.0.1/Paytring/paytring/utility/utility.py
-drwxrwxrwx   0        0        0        0 2023-06-14 12:23:37.425086 paytring-1.0.1/Paytring/paytring.egg-info/
--rw-rw-rw-   0        0        0     5098 2023-06-14 12:23:37.000000 paytring-1.0.1/Paytring/paytring.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      510 2023-06-14 12:23:37.000000 paytring-1.0.1/Paytring/paytring.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 12:23:37.000000 paytring-1.0.1/Paytring/paytring.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-14 12:23:37.000000 paytring-1.0.1/Paytring/paytring.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-14 12:23:37.000000 paytring-1.0.1/Paytring/paytring.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 12:23:37.441696 paytring-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      846 2023-06-14 12:23:08.000000 paytring-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 07:52:54.488253 paytring-1.0.2/
+-rw-rw-rw-   0        0        0     1094 2023-06-20 07:52:43.000000 paytring-1.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     5216 2023-06-20 07:52:54.487245 paytring-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-20 07:52:54.457441 paytring-1.0.2/Paytring/
+drwxrwxrwx   0        0        0        0 2023-06-20 07:52:54.466023 paytring-1.0.2/Paytring/paytring/
+-rw-rw-rw-   0        0        0      113 2023-06-02 11:09:08.000000 paytring-1.0.2/Paytring/paytring/__init__.py
+-rw-rw-rw-   0        0        0     5370 2023-06-20 07:52:38.000000 paytring-1.0.2/Paytring/paytring/client.py
+drwxrwxrwx   0        0        0        0 2023-06-20 07:52:54.478789 paytring-1.0.2/Paytring/paytring/constant/
+-rw-rw-rw-   0        0        0       52 2023-06-02 12:35:28.000000 paytring-1.0.2/Paytring/paytring/constant/__init__.py
+-rw-rw-rw-   0        0        0      338 2023-06-20 07:52:40.000000 paytring-1.0.2/Paytring/paytring/constant/url.py
+drwxrwxrwx   0        0        0        0 2023-06-20 07:52:54.482093 paytring-1.0.2/Paytring/paytring/resources/
+-rw-rw-rw-   0        0        0       69 2023-06-02 12:35:26.000000 paytring-1.0.2/Paytring/paytring/resources/__init__.py
+-rw-rw-rw-   0        0        0      337 2023-06-14 10:54:33.000000 paytring-1.0.2/Paytring/paytring/resources/paytring.py
+drwxrwxrwx   0        0        0        0 2023-06-20 07:52:54.485237 paytring-1.0.2/Paytring/paytring/utility/
+-rw-rw-rw-   0        0        0       66 2023-06-02 12:35:13.000000 paytring-1.0.2/Paytring/paytring/utility/__init__.py
+-rw-rw-rw-   0        0        0     2945 2023-06-20 07:30:16.000000 paytring-1.0.2/Paytring/paytring/utility/utility.py
+drwxrwxrwx   0        0        0        0 2023-06-20 07:52:54.475528 paytring-1.0.2/Paytring/paytring.egg-info/
+-rw-rw-rw-   0        0        0     5216 2023-06-20 07:52:54.000000 paytring-1.0.2/Paytring/paytring.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      510 2023-06-20 07:52:54.000000 paytring-1.0.2/Paytring/paytring.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 07:52:54.000000 paytring-1.0.2/Paytring/paytring.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-20 07:52:54.000000 paytring-1.0.2/Paytring/paytring.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-20 07:52:54.000000 paytring-1.0.2/Paytring/paytring.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 07:52:54.488253 paytring-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      846 2023-06-20 07:52:27.000000 paytring-1.0.2/setup.py
```

### Comparing `paytring-1.0.1/LICENSE.txt` & `paytring-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `paytring-1.0.1/PKG-INFO` & `paytring-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paytring
-Version: 1.0.1
+Version: 1.0.2
 Summary: A SDK which helps to create, fetch or refund an order on Paytring
 Home-page: https://github.com/paytring/python-sdk
 Author: Paytirng
 Author-email: developer@paytring.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
@@ -49,14 +49,20 @@
 
 - Receipt ID(string)
 - Amount(string)
 - Callback Url(string)
 - Customer Info ( Dictionary )
 - Currency (String : INR or USD)
 
+###### Optional Parameters
+
+- PG (String)
+- PG Pool ID (String)
+
+
 #### Methods
 
 ```python
 customer_info = {
     "cname": "test",
     "email": "abc@gmail.com" -> it will be baseEncode256,
     "phone": "phone"
@@ -64,15 +70,17 @@
 
 
 order.create(
     receipt_id,
     amount,
     callback_url,
     customer_info,
-    currrency
+    currrency,
+    pg(optioanl),
+    pg_pool_id(optional)
 )
 ```
 
 #### Response
 
 ```
 {
```

### Comparing `paytring-1.0.1/Paytring/paytring/client.py` & `paytring-1.0.2/Paytring/paytring/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         super().__init__()
         self.order_create_url = URL.ORDER_CREATE
         self.order_fetch_url = URL.FETCH_ORDER
         self.order_fetch_by_receipt_url = URL.FETCH_ORDER_BY_RECIEPT
         self.refund_url = URL.REFUND
         self.utility_obj = Utility()
 
-    def create(self, receipt_id, amount, callback_url,customer_info, currency):
+    def create(self, receipt_id, amount, callback_url,customer_info, currency, pg=None, pg_pool_id=None):
         """
         Use to create an Order on Paytring
 
         Args(type=string):
             'receipt' : Receipt Id for the order
             'amount' :  Amount of Order
             'callback_url' : The URL where the PAYTRING will send success/failed etc. response.
@@ -44,14 +44,22 @@
                 "callback_url": callback_url,
                 "cname": customer_info['cname'],
                 "email": customer_info['email'],
                 "phone": customer_info['phone'],
                 "currency" : currency
             }
 
+            if pg is not None:
+                self.utility_obj.validate_pg(pg)
+                payload['pg'] = pg
+
+            if pg_pool_id is not None:
+                self.utility_obj.validate_currency(pg_pool_id)
+                payload['pg_pool_id'] = pg_pool_id
+
             hash = self.utility_obj.create_hash(payload)
             payload['hash'] = hash
 
             response = requests.post(self.order_create_url, payload)
             response = response.json()
             if response['status'] == True:
                     if 'url' in response.keys():
```

### Comparing `paytring-1.0.1/Paytring/paytring/utility/utility.py` & `paytring-1.0.2/Paytring/paytring/utility/utility.py`

 * *Files 7% similar despite different names*

```diff
@@ -74,7 +74,16 @@
         return bool(re.match(pattern, currency))
     
     def validate_order(self, order_id) -> bool:
         if isinstance(order_id, str):
             return True
         raise Exception('Invalid order id')
 
+    def validate_pg(self, pg) -> bool:
+        if isinstance(pg, str):
+            return True
+        raise Exception('Invalid PG')
+    
+    def validate_order(self, pg_pool_id) -> bool:
+        if isinstance(pg_pool_id, str):
+            return True
+        raise Exception('Invalid PG pool ID')
```

### Comparing `paytring-1.0.1/Paytring/paytring.egg-info/PKG-INFO` & `paytring-1.0.2/Paytring/paytring.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paytring
-Version: 1.0.1
+Version: 1.0.2
 Summary: A SDK which helps to create, fetch or refund an order on Paytring
 Home-page: https://github.com/paytring/python-sdk
 Author: Paytirng
 Author-email: developer@paytring.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
@@ -49,14 +49,20 @@
 
 - Receipt ID(string)
 - Amount(string)
 - Callback Url(string)
 - Customer Info ( Dictionary )
 - Currency (String : INR or USD)
 
+###### Optional Parameters
+
+- PG (String)
+- PG Pool ID (String)
+
+
 #### Methods
 
 ```python
 customer_info = {
     "cname": "test",
     "email": "abc@gmail.com" -> it will be baseEncode256,
     "phone": "phone"
@@ -64,15 +70,17 @@
 
 
 order.create(
     receipt_id,
     amount,
     callback_url,
     customer_info,
-    currrency
+    currrency,
+    pg(optioanl),
+    pg_pool_id(optional)
 )
 ```
 
 #### Response
 
 ```
 {
```

### Comparing `paytring-1.0.1/setup.py` & `paytring-1.0.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("Paytring/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="paytring",
-    version="1.0.1",
+    version="1.0.2",
     description="A SDK which helps to create, fetch or refund an order on Paytring",
     package_dir={"": "Paytring"},
     packages=find_packages(where="Paytring"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/paytring/python-sdk",
     author="Paytirng",
```

