# Comparing `tmp/smsmanpy-0.0.1.tar.gz` & `tmp/smsmanpy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smsmanpy-0.0.1.tar", last modified: Tue Jun 20 07:46:50 2023, max compression
+gzip compressed data, was "smsmanpy-0.0.2.tar", last modified: Tue Jun 20 08:18:20 2023, max compression
```

## Comparing `smsmanpy-0.0.1.tar` & `smsmanpy-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 byrbon     (501) staff       (20)        0 2023-06-20 07:46:50.876174 smsmanpy-0.0.1/
--rw-r--r--   0 byrbon     (501) staff       (20)     2276 2023-06-20 07:46:50.876250 smsmanpy-0.0.1/PKG-INFO
--rw-r--r--   0 byrbon     (501) staff       (20)     1632 2023-06-20 07:32:50.000000 smsmanpy-0.0.1/README.md
--rw-r--r--   0 byrbon     (501) staff       (20)       38 2023-06-20 07:46:50.876460 smsmanpy-0.0.1/setup.cfg
--rw-r--r--   0 byrbon     (501) staff       (20)      985 2023-06-16 11:58:07.000000 smsmanpy-0.0.1/setup.py
-drwxr-xr-x   0 byrbon     (501) staff       (20)        0 2023-06-20 07:46:50.875326 smsmanpy-0.0.1/smsmanpy/
--rw-r--r--   0 byrbon     (501) staff       (20)      219 2023-06-15 14:20:27.000000 smsmanpy-0.0.1/smsmanpy/__init__.py
--rw-r--r--   0 byrbon     (501) staff       (20)      481 2023-06-13 07:49:40.000000 smsmanpy-0.0.1/smsmanpy/exeptions.py
--rw-r--r--   0 byrbon     (501) staff       (20)     7890 2023-06-20 07:29:22.000000 smsmanpy-0.0.1/smsmanpy/requests.py
-drwxr-xr-x   0 byrbon     (501) staff       (20)        0 2023-06-20 07:46:50.876059 smsmanpy-0.0.1/smsmanpy.egg-info/
--rw-r--r--   0 byrbon     (501) staff       (20)     2276 2023-06-20 07:46:50.000000 smsmanpy-0.0.1/smsmanpy.egg-info/PKG-INFO
--rw-r--r--   0 byrbon     (501) staff       (20)      251 2023-06-20 07:46:50.000000 smsmanpy-0.0.1/smsmanpy.egg-info/SOURCES.txt
--rw-r--r--   0 byrbon     (501) staff       (20)        1 2023-06-20 07:46:50.000000 smsmanpy-0.0.1/smsmanpy.egg-info/dependency_links.txt
--rw-r--r--   0 byrbon     (501) staff       (20)        8 2023-06-20 07:46:50.000000 smsmanpy-0.0.1/smsmanpy.egg-info/requires.txt
--rw-r--r--   0 byrbon     (501) staff       (20)        9 2023-06-20 07:46:50.000000 smsmanpy-0.0.1/smsmanpy.egg-info/top_level.txt
+drwxr-xr-x   0 byrbon     (501) staff       (20)        0 2023-06-20 08:18:20.924138 smsmanpy-0.0.2/
+-rw-r--r--   0 byrbon     (501) staff       (20)     2267 2023-06-20 08:18:20.924227 smsmanpy-0.0.2/PKG-INFO
+-rw-r--r--   0 byrbon     (501) staff       (20)     1623 2023-06-20 07:55:53.000000 smsmanpy-0.0.2/README.md
+-rw-r--r--   0 byrbon     (501) staff       (20)       38 2023-06-20 08:18:20.924491 smsmanpy-0.0.2/setup.cfg
+-rw-r--r--   0 byrbon     (501) staff       (20)      985 2023-06-20 08:12:27.000000 smsmanpy-0.0.2/setup.py
+drwxr-xr-x   0 byrbon     (501) staff       (20)        0 2023-06-20 08:18:20.922822 smsmanpy-0.0.2/smsmanpy/
+-rw-r--r--   0 byrbon     (501) staff       (20)      219 2023-06-15 14:20:27.000000 smsmanpy-0.0.2/smsmanpy/__init__.py
+-rw-r--r--   0 byrbon     (501) staff       (20)      481 2023-06-13 07:49:40.000000 smsmanpy-0.0.2/smsmanpy/exeptions.py
+-rw-r--r--   0 byrbon     (501) staff       (20)     7890 2023-06-20 08:12:27.000000 smsmanpy-0.0.2/smsmanpy/requests.py
+drwxr-xr-x   0 byrbon     (501) staff       (20)        0 2023-06-20 08:18:20.923957 smsmanpy-0.0.2/smsmanpy.egg-info/
+-rw-r--r--   0 byrbon     (501) staff       (20)     2267 2023-06-20 08:18:20.000000 smsmanpy-0.0.2/smsmanpy.egg-info/PKG-INFO
+-rw-r--r--   0 byrbon     (501) staff       (20)      251 2023-06-20 08:18:20.000000 smsmanpy-0.0.2/smsmanpy.egg-info/SOURCES.txt
+-rw-r--r--   0 byrbon     (501) staff       (20)        1 2023-06-20 08:18:20.000000 smsmanpy-0.0.2/smsmanpy.egg-info/dependency_links.txt
+-rw-r--r--   0 byrbon     (501) staff       (20)        8 2023-06-20 08:18:20.000000 smsmanpy-0.0.2/smsmanpy.egg-info/requires.txt
+-rw-r--r--   0 byrbon     (501) staff       (20)        9 2023-06-20 08:18:20.000000 smsmanpy-0.0.2/smsmanpy.egg-info/top_level.txt
```

### Comparing `smsmanpy-0.0.1/PKG-INFO` & `smsmanpy-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smsmanpy
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package to simplify work with the sms-man API
 Home-page: https://github.com/smsmancom/smsmanpy/
 Author: Alexandr Lebedchenko
 Author-email: alex_leb@sms-man.com
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -24,15 +24,15 @@
 pip install smsmanpy
 ```
 ## Documentation  
 [https://sms-man.com/site/docs-apiv2](https://sms-man.com/site/docs-apiv2)
 ## RESTful APIs
 Usage examples:
 ```python
-from smsmanpy.requests import Smsman
+from smsmanpy import Smsman
 
 #To receive an API key, you need to register on the sms-man.com website.
 api_key = ""
 
 client = Smsman(api_key)
 
 #  Get current balance
```

### Comparing `smsmanpy-0.0.1/README.md` & `smsmanpy-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 pip install smsmanpy
 ```
 ## Documentation  
 [https://sms-man.com/site/docs-apiv2](https://sms-man.com/site/docs-apiv2)
 ## RESTful APIs
 Usage examples:
 ```python
-from smsmanpy.requests import Smsman
+from smsmanpy import Smsman
 
 #To receive an API key, you need to register on the sms-man.com website.
 api_key = ""
 
 client = Smsman(api_key)
 
 #  Get current balance
```

### Comparing `smsmanpy-0.0.1/setup.py` & `smsmanpy-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 requirements = ["aiohttp"]
 
 setup(
     name="smsmanpy",
-    version="0.0.1",
+    version="0.0.2",
     author="Alexandr Lebedchenko",
     author_email="alex_leb@sms-man.com",
     description="A package to simplify work with the sms-man API",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/smsmancom/smsmanpy/", #url from smsmangithab
     packages=find_packages(),
```

### Comparing `smsmanpy-0.0.1/smsmanpy/requests.py` & `smsmanpy-0.0.2/smsmanpy/requests.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,15 +106,15 @@
             async with session.get(self.__base_url + self.__method_get_all_services, params=self.__params) as response:
                 data = await response.json()
                 if "1" in data:
                     return data
                 else:
                     raise WrongTokenError(data['error_msg'])
 
-    async def __request_phone_number(self, country_id: str, application_id: str):
+    async def __request_phone_number(self, country_id: int, application_id: int):
         """
         Queries the phone number by country id and service id.
         Returns request number (needed to receive sms) and phone number.
 
         :param country_id: id of country. Can check list on web-site or with method get_all_countries
         :param application_id: id of application. Can check list on web-site or with method get_all_services
         :return: request_id, number
@@ -131,15 +131,15 @@
                 elif resp_json['error_code'] == "balance":
                     raise LowBalance(resp_json['error_msg'])
                 elif resp_json["error_code"] == "no_numbers":
                     raise NoNumbers(resp_json["error_msg"])
                 else:
                     raise WrongTokenError(resp_json['error_msg'])
 
-    async def __request_many_phone_numbers(self, country_id: str, application_id: str, semaphore: asyncio.Semaphore):
+    async def __request_many_phone_numbers(self, country_id: int, application_id: int, semaphore: asyncio.Semaphore):
         params = self.__check_params(country_id, application_id)
         async with aiohttp.ClientSession() as session:
             for _ in range(3):
                 async with semaphore:
                     async with session.get(self.__base_url + self.__method_get_number, params=params) as response:
                         resp_json = await response.json()
                         if "request_id" in resp_json and "number" in resp_json:
@@ -147,15 +147,15 @@
                         elif resp_json['error_code'] == "balance":
                             raise LowBalance(resp_json['error_msg'])
                         elif resp_json["error_code"] == "no_numbers":
                             continue
                         else:
                             raise WrongTokenError(resp_json['error_msg'])
 
-    async def _request_phone_numbers(self, country_id: str, application_id: str, amount: int):
+    async def _request_phone_numbers(self, country_id: int, application_id: int, amount: int):
 
         semaphore = asyncio.Semaphore(2)
         tasks = [self.__request_many_phone_numbers(country_id, application_id, semaphore) for i in range(amount)]
         responses = await asyncio.gather(*tasks)
 
         return responses
 
@@ -194,15 +194,15 @@
 
     def get_limits(self, country_id=None, application_id=None):
         return asyncio.run(self.__get_limits(country_id, application_id))
 
     def get_sms(self, request_id: str):
         return asyncio.run(self.__get_sms(request_id))
 
-    def request_phone_number(self, country_id: str, application_id: str):
+    def request_phone_number(self, country_id: int, application_id: int):
         return asyncio.run(self.__request_phone_number(country_id, application_id))
 
-    def request_phone_numbers(self, country_id: str, application_id: str, amount: int):
+    def request_phone_numbers(self, country_id: int, application_id: int, amount: int):
         return asyncio.run(self._request_phone_numbers(country_id, application_id, amount))
```

### Comparing `smsmanpy-0.0.1/smsmanpy.egg-info/PKG-INFO` & `smsmanpy-0.0.2/smsmanpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smsmanpy
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package to simplify work with the sms-man API
 Home-page: https://github.com/smsmancom/smsmanpy/
 Author: Alexandr Lebedchenko
 Author-email: alex_leb@sms-man.com
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -24,15 +24,15 @@
 pip install smsmanpy
 ```
 ## Documentation  
 [https://sms-man.com/site/docs-apiv2](https://sms-man.com/site/docs-apiv2)
 ## RESTful APIs
 Usage examples:
 ```python
-from smsmanpy.requests import Smsman
+from smsmanpy import Smsman
 
 #To receive an API key, you need to register on the sms-man.com website.
 api_key = ""
 
 client = Smsman(api_key)
 
 #  Get current balance
```

