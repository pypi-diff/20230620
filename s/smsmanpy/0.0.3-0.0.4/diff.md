# Comparing `tmp/smsmanpy-0.0.3.tar.gz` & `tmp/smsmanpy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smsmanpy-0.0.3.tar", last modified: Tue Jun 20 09:03:58 2023, max compression
+gzip compressed data, was "smsmanpy-0.0.4.tar", last modified: Tue Jun 20 09:36:39 2023, max compression
```

## Comparing `smsmanpy-0.0.3.tar` & `smsmanpy-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 byrbon     (501) staff       (20)        0 2023-06-20 09:03:58.621530 smsmanpy-0.0.3/
--rw-r--r--   0 byrbon     (501) staff       (20)     2338 2023-06-20 09:03:58.621640 smsmanpy-0.0.3/PKG-INFO
--rw-r--r--   0 byrbon     (501) staff       (20)     1694 2023-06-20 08:53:13.000000 smsmanpy-0.0.3/README.md
--rw-r--r--   0 byrbon     (501) staff       (20)       38 2023-06-20 09:03:58.621910 smsmanpy-0.0.3/setup.cfg
--rw-r--r--   0 byrbon     (501) staff       (20)      985 2023-06-20 08:39:28.000000 smsmanpy-0.0.3/setup.py
-drwxr-xr-x   0 byrbon     (501) staff       (20)        0 2023-06-20 09:03:58.619514 smsmanpy-0.0.3/smsmanpy/
--rw-r--r--   0 byrbon     (501) staff       (20)      219 2023-06-15 14:20:27.000000 smsmanpy-0.0.3/smsmanpy/__init__.py
--rw-r--r--   0 byrbon     (501) staff       (20)      481 2023-06-13 07:49:40.000000 smsmanpy-0.0.3/smsmanpy/exeptions.py
--rw-r--r--   0 byrbon     (501) staff       (20)     8520 2023-06-20 08:56:57.000000 smsmanpy-0.0.3/smsmanpy/requests.py
-drwxr-xr-x   0 byrbon     (501) staff       (20)        0 2023-06-20 09:03:58.621393 smsmanpy-0.0.3/smsmanpy.egg-info/
--rw-r--r--   0 byrbon     (501) staff       (20)     2338 2023-06-20 09:03:58.000000 smsmanpy-0.0.3/smsmanpy.egg-info/PKG-INFO
--rw-r--r--   0 byrbon     (501) staff       (20)      251 2023-06-20 09:03:58.000000 smsmanpy-0.0.3/smsmanpy.egg-info/SOURCES.txt
--rw-r--r--   0 byrbon     (501) staff       (20)        1 2023-06-20 09:03:58.000000 smsmanpy-0.0.3/smsmanpy.egg-info/dependency_links.txt
--rw-r--r--   0 byrbon     (501) staff       (20)        8 2023-06-20 09:03:58.000000 smsmanpy-0.0.3/smsmanpy.egg-info/requires.txt
--rw-r--r--   0 byrbon     (501) staff       (20)        9 2023-06-20 09:03:58.000000 smsmanpy-0.0.3/smsmanpy.egg-info/top_level.txt
+drwxr-xr-x   0 byrbon     (501) staff       (20)        0 2023-06-20 09:36:39.189797 smsmanpy-0.0.4/
+-rw-r--r--   0 byrbon     (501) staff       (20)     2338 2023-06-20 09:36:39.189895 smsmanpy-0.0.4/PKG-INFO
+-rw-r--r--   0 byrbon     (501) staff       (20)     1694 2023-06-20 08:53:13.000000 smsmanpy-0.0.4/README.md
+-rw-r--r--   0 byrbon     (501) staff       (20)       38 2023-06-20 09:36:39.190178 smsmanpy-0.0.4/setup.cfg
+-rw-r--r--   0 byrbon     (501) staff       (20)      985 2023-06-20 09:36:34.000000 smsmanpy-0.0.4/setup.py
+drwxr-xr-x   0 byrbon     (501) staff       (20)        0 2023-06-20 09:36:39.188764 smsmanpy-0.0.4/smsmanpy/
+-rw-r--r--   0 byrbon     (501) staff       (20)      219 2023-06-15 14:20:27.000000 smsmanpy-0.0.4/smsmanpy/__init__.py
+-rw-r--r--   0 byrbon     (501) staff       (20)      481 2023-06-13 07:49:40.000000 smsmanpy-0.0.4/smsmanpy/exeptions.py
+-rw-r--r--   0 byrbon     (501) staff       (20)     8673 2023-06-20 09:33:31.000000 smsmanpy-0.0.4/smsmanpy/requests.py
+drwxr-xr-x   0 byrbon     (501) staff       (20)        0 2023-06-20 09:36:39.189640 smsmanpy-0.0.4/smsmanpy.egg-info/
+-rw-r--r--   0 byrbon     (501) staff       (20)     2338 2023-06-20 09:36:39.000000 smsmanpy-0.0.4/smsmanpy.egg-info/PKG-INFO
+-rw-r--r--   0 byrbon     (501) staff       (20)      251 2023-06-20 09:36:39.000000 smsmanpy-0.0.4/smsmanpy.egg-info/SOURCES.txt
+-rw-r--r--   0 byrbon     (501) staff       (20)        1 2023-06-20 09:36:39.000000 smsmanpy-0.0.4/smsmanpy.egg-info/dependency_links.txt
+-rw-r--r--   0 byrbon     (501) staff       (20)        8 2023-06-20 09:36:39.000000 smsmanpy-0.0.4/smsmanpy.egg-info/requires.txt
+-rw-r--r--   0 byrbon     (501) staff       (20)        9 2023-06-20 09:36:39.000000 smsmanpy-0.0.4/smsmanpy.egg-info/top_level.txt
```

### Comparing `smsmanpy-0.0.3/PKG-INFO` & `smsmanpy-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smsmanpy
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package to simplify work with the sms-man API
 Home-page: https://github.com/smsmancom/smsmanpy/
 Author: Alexandr Lebedchenko
 Author-email: alex_leb@sms-man.com
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `smsmanpy-0.0.3/README.md` & `smsmanpy-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `smsmanpy-0.0.3/setup.py` & `smsmanpy-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 requirements = ["aiohttp"]
 
 setup(
     name="smsmanpy",
-    version="0.0.3",
+    version="0.0.4",
     author="Alexandr Lebedchenko",
     author_email="alex_leb@sms-man.com",
     description="A package to simplify work with the sms-man API",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/smsmancom/smsmanpy/", #url from smsmangithab
     packages=find_packages(),
```

### Comparing `smsmanpy-0.0.3/smsmanpy/requests.py` & `smsmanpy-0.0.4/smsmanpy/requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,23 +137,26 @@
 
     async def __request_many_phone_numbers(self, country_id: int, application_id: int, semaphore: asyncio.Semaphore):
         params = self.__check_params(country_id, application_id)
         async with aiohttp.ClientSession() as session:
             for _ in range(3):
                 async with semaphore:
                     async with session.get(self.__base_url + self.__method_get_number, params=params) as response:
-                        resp_json = await response.json()
-                        if "request_id" in resp_json and "number" in resp_json:
-                            return resp_json['request_id'], resp_json["number"]
-                        elif resp_json['error_code'] == "balance":
-                            raise LowBalance(resp_json['error_msg'])
-                        elif resp_json["error_code"] == "no_numbers":
-                            continue
-                        else:
-                            raise WrongTokenError(resp_json['error_msg'])
+                        try:
+                            resp_json = await response.json()
+                            if "request_id" in resp_json and "number" in resp_json:
+                                return resp_json['request_id'], resp_json["number"]
+                            elif resp_json['error_code'] == "balance":
+                                raise LowBalance(resp_json['error_msg'])
+                            elif resp_json["error_code"] == "no_numbers":
+                                continue
+                            else:
+                                raise WrongTokenError(resp_json['error_msg'])
+                        except:
+                            raise await response.text()
 
     async def _request_phone_numbers(self, country_id: int, application_id: int, amount: int):
 
         semaphore = asyncio.Semaphore(2)
         tasks = [self.__request_many_phone_numbers(country_id, application_id, semaphore) for i in range(amount)]
         responses = await asyncio.gather(*tasks)
```

### Comparing `smsmanpy-0.0.3/smsmanpy.egg-info/PKG-INFO` & `smsmanpy-0.0.4/smsmanpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smsmanpy
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package to simplify work with the sms-man API
 Home-page: https://github.com/smsmancom/smsmanpy/
 Author: Alexandr Lebedchenko
 Author-email: alex_leb@sms-man.com
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

