# Comparing `tmp/smsmanpy-0.0.2.tar.gz` & `tmp/smsmanpy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smsmanpy-0.0.2.tar", last modified: Tue Jun 20 08:18:20 2023, max compression
+gzip compressed data, was "smsmanpy-0.0.3.tar", last modified: Tue Jun 20 09:03:58 2023, max compression
```

## Comparing `smsmanpy-0.0.2.tar` & `smsmanpy-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 byrbon     (501) staff       (20)        0 2023-06-20 08:18:20.924138 smsmanpy-0.0.2/
--rw-r--r--   0 byrbon     (501) staff       (20)     2267 2023-06-20 08:18:20.924227 smsmanpy-0.0.2/PKG-INFO
--rw-r--r--   0 byrbon     (501) staff       (20)     1623 2023-06-20 07:55:53.000000 smsmanpy-0.0.2/README.md
--rw-r--r--   0 byrbon     (501) staff       (20)       38 2023-06-20 08:18:20.924491 smsmanpy-0.0.2/setup.cfg
--rw-r--r--   0 byrbon     (501) staff       (20)      985 2023-06-20 08:12:27.000000 smsmanpy-0.0.2/setup.py
-drwxr-xr-x   0 byrbon     (501) staff       (20)        0 2023-06-20 08:18:20.922822 smsmanpy-0.0.2/smsmanpy/
--rw-r--r--   0 byrbon     (501) staff       (20)      219 2023-06-15 14:20:27.000000 smsmanpy-0.0.2/smsmanpy/__init__.py
--rw-r--r--   0 byrbon     (501) staff       (20)      481 2023-06-13 07:49:40.000000 smsmanpy-0.0.2/smsmanpy/exeptions.py
--rw-r--r--   0 byrbon     (501) staff       (20)     7890 2023-06-20 08:12:27.000000 smsmanpy-0.0.2/smsmanpy/requests.py
-drwxr-xr-x   0 byrbon     (501) staff       (20)        0 2023-06-20 08:18:20.923957 smsmanpy-0.0.2/smsmanpy.egg-info/
--rw-r--r--   0 byrbon     (501) staff       (20)     2267 2023-06-20 08:18:20.000000 smsmanpy-0.0.2/smsmanpy.egg-info/PKG-INFO
--rw-r--r--   0 byrbon     (501) staff       (20)      251 2023-06-20 08:18:20.000000 smsmanpy-0.0.2/smsmanpy.egg-info/SOURCES.txt
--rw-r--r--   0 byrbon     (501) staff       (20)        1 2023-06-20 08:18:20.000000 smsmanpy-0.0.2/smsmanpy.egg-info/dependency_links.txt
--rw-r--r--   0 byrbon     (501) staff       (20)        8 2023-06-20 08:18:20.000000 smsmanpy-0.0.2/smsmanpy.egg-info/requires.txt
--rw-r--r--   0 byrbon     (501) staff       (20)        9 2023-06-20 08:18:20.000000 smsmanpy-0.0.2/smsmanpy.egg-info/top_level.txt
+drwxr-xr-x   0 byrbon     (501) staff       (20)        0 2023-06-20 09:03:58.621530 smsmanpy-0.0.3/
+-rw-r--r--   0 byrbon     (501) staff       (20)     2338 2023-06-20 09:03:58.621640 smsmanpy-0.0.3/PKG-INFO
+-rw-r--r--   0 byrbon     (501) staff       (20)     1694 2023-06-20 08:53:13.000000 smsmanpy-0.0.3/README.md
+-rw-r--r--   0 byrbon     (501) staff       (20)       38 2023-06-20 09:03:58.621910 smsmanpy-0.0.3/setup.cfg
+-rw-r--r--   0 byrbon     (501) staff       (20)      985 2023-06-20 08:39:28.000000 smsmanpy-0.0.3/setup.py
+drwxr-xr-x   0 byrbon     (501) staff       (20)        0 2023-06-20 09:03:58.619514 smsmanpy-0.0.3/smsmanpy/
+-rw-r--r--   0 byrbon     (501) staff       (20)      219 2023-06-15 14:20:27.000000 smsmanpy-0.0.3/smsmanpy/__init__.py
+-rw-r--r--   0 byrbon     (501) staff       (20)      481 2023-06-13 07:49:40.000000 smsmanpy-0.0.3/smsmanpy/exeptions.py
+-rw-r--r--   0 byrbon     (501) staff       (20)     8520 2023-06-20 08:56:57.000000 smsmanpy-0.0.3/smsmanpy/requests.py
+drwxr-xr-x   0 byrbon     (501) staff       (20)        0 2023-06-20 09:03:58.621393 smsmanpy-0.0.3/smsmanpy.egg-info/
+-rw-r--r--   0 byrbon     (501) staff       (20)     2338 2023-06-20 09:03:58.000000 smsmanpy-0.0.3/smsmanpy.egg-info/PKG-INFO
+-rw-r--r--   0 byrbon     (501) staff       (20)      251 2023-06-20 09:03:58.000000 smsmanpy-0.0.3/smsmanpy.egg-info/SOURCES.txt
+-rw-r--r--   0 byrbon     (501) staff       (20)        1 2023-06-20 09:03:58.000000 smsmanpy-0.0.3/smsmanpy.egg-info/dependency_links.txt
+-rw-r--r--   0 byrbon     (501) staff       (20)        8 2023-06-20 09:03:58.000000 smsmanpy-0.0.3/smsmanpy.egg-info/requires.txt
+-rw-r--r--   0 byrbon     (501) staff       (20)        9 2023-06-20 09:03:58.000000 smsmanpy-0.0.3/smsmanpy.egg-info/top_level.txt
```

### Comparing `smsmanpy-0.0.2/PKG-INFO` & `smsmanpy-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smsmanpy
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package to simplify work with the sms-man API
 Home-page: https://github.com/smsmancom/smsmanpy/
 Author: Alexandr Lebedchenko
 Author-email: alex_leb@sms-man.com
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -27,15 +27,15 @@
 [https://sms-man.com/site/docs-apiv2](https://sms-man.com/site/docs-apiv2)
 ## RESTful APIs
 Usage examples:
 ```python
 from smsmanpy import Smsman
 
 #To receive an API key, you need to register on the sms-man.com website.
-api_key = ""
+api_key = "api_key"
 
 client = Smsman(api_key)
 
 #  Get current balance
 print(client.get_balance())
 
 #  Get information about all services
@@ -52,16 +52,18 @@
                                                        application_id=1)
 # Buy many numbers
 print(client.request_phone_numbers(country_id=1,
                                    application_id=1,
                                    amount=10))
 
 #  Receive a SMS to the number
-sms_code = client.get_sms(request_id)
+sms_code = client.get_sms('request_id')
 
+# Reject the number
+print(client.reject_number('request_id'))
 ```
 
   
 
 ## Contributing
 
 Contributions are welcome.<br/>
```

### Comparing `smsmanpy-0.0.2/README.md` & `smsmanpy-0.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 [https://sms-man.com/site/docs-apiv2](https://sms-man.com/site/docs-apiv2)
 ## RESTful APIs
 Usage examples:
 ```python
 from smsmanpy import Smsman
 
 #To receive an API key, you need to register on the sms-man.com website.
-api_key = ""
+api_key = "api_key"
 
 client = Smsman(api_key)
 
 #  Get current balance
 print(client.get_balance())
 
 #  Get information about all services
@@ -36,16 +36,18 @@
                                                        application_id=1)
 # Buy many numbers
 print(client.request_phone_numbers(country_id=1,
                                    application_id=1,
                                    amount=10))
 
 #  Receive a SMS to the number
-sms_code = client.get_sms(request_id)
+sms_code = client.get_sms('request_id')
 
+# Reject the number
+print(client.reject_number('request_id'))
 ```
 
   
 
 ## Contributing
 
 Contributions are welcome.<br/>
```

### Comparing `smsmanpy-0.0.2/setup.py` & `smsmanpy-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 requirements = ["aiohttp"]
 
 setup(
     name="smsmanpy",
-    version="0.0.2",
+    version="0.0.3",
     author="Alexandr Lebedchenko",
     author_email="alex_leb@sms-man.com",
     description="A package to simplify work with the sms-man API",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/smsmancom/smsmanpy/", #url from smsmangithab
     packages=find_packages(),
```

### Comparing `smsmanpy-0.0.2/smsmanpy/requests.py` & `smsmanpy-0.0.3/smsmanpy/requests.py`

 * *Files 4% similar despite different names*

```diff
@@ -179,14 +179,28 @@
         if status:
             params['status'] = status
         if request_id:
             params['request_id'] = request_id
 
         return params
 
+    async def __reject_number(self, request_id: str):
+        """
+        Returns the number if it did not receive an SMS. Money is returned to the balance
+        :param request_id: Number of IF (get with phone number)
+        """
+        params = self.__check_params(request_id=request_id, status="reject")
+
+        async with aiohttp.ClientSession() as session:
+            async with session.get(self.__base_url + self.__method_reject_number, params=params) as response:
+                response.raise_for_status()
+
+    def reject_number(self, request_id: str):
+        return asyncio.run(self.__reject_number(request_id))
+
     def get_all_services(self):
         return asyncio.run(self.__get_all_services())
 
     def get_all_countries(self):
         return asyncio.run(self.__get_all_countries())
 
     def get_balance(self):
@@ -202,7 +216,9 @@
         return asyncio.run(self.__request_phone_number(country_id, application_id))
 
     def request_phone_numbers(self, country_id: int, application_id: int, amount: int):
         return asyncio.run(self._request_phone_numbers(country_id, application_id, amount))
 
 
 
+
+
```

### Comparing `smsmanpy-0.0.2/smsmanpy.egg-info/PKG-INFO` & `smsmanpy-0.0.3/smsmanpy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smsmanpy
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package to simplify work with the sms-man API
 Home-page: https://github.com/smsmancom/smsmanpy/
 Author: Alexandr Lebedchenko
 Author-email: alex_leb@sms-man.com
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -27,15 +27,15 @@
 [https://sms-man.com/site/docs-apiv2](https://sms-man.com/site/docs-apiv2)
 ## RESTful APIs
 Usage examples:
 ```python
 from smsmanpy import Smsman
 
 #To receive an API key, you need to register on the sms-man.com website.
-api_key = ""
+api_key = "api_key"
 
 client = Smsman(api_key)
 
 #  Get current balance
 print(client.get_balance())
 
 #  Get information about all services
@@ -52,16 +52,18 @@
                                                        application_id=1)
 # Buy many numbers
 print(client.request_phone_numbers(country_id=1,
                                    application_id=1,
                                    amount=10))
 
 #  Receive a SMS to the number
-sms_code = client.get_sms(request_id)
+sms_code = client.get_sms('request_id')
 
+# Reject the number
+print(client.reject_number('request_id'))
 ```
 
   
 
 ## Contributing
 
 Contributions are welcome.<br/>
```

