# Comparing `tmp/smsmanpy-0.0.4.tar.gz` & `tmp/smsmanpy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smsmanpy-0.0.4.tar", last modified: Tue Jun 20 09:36:39 2023, max compression
+gzip compressed data, was "smsmanpy-0.0.5.tar", last modified: Tue Jun 20 09:55:29 2023, max compression
```

## Comparing `smsmanpy-0.0.4.tar` & `smsmanpy-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 byrbon     (501) staff       (20)        0 2023-06-20 09:36:39.189797 smsmanpy-0.0.4/
--rw-r--r--   0 byrbon     (501) staff       (20)     2338 2023-06-20 09:36:39.189895 smsmanpy-0.0.4/PKG-INFO
--rw-r--r--   0 byrbon     (501) staff       (20)     1694 2023-06-20 08:53:13.000000 smsmanpy-0.0.4/README.md
--rw-r--r--   0 byrbon     (501) staff       (20)       38 2023-06-20 09:36:39.190178 smsmanpy-0.0.4/setup.cfg
--rw-r--r--   0 byrbon     (501) staff       (20)      985 2023-06-20 09:36:34.000000 smsmanpy-0.0.4/setup.py
-drwxr-xr-x   0 byrbon     (501) staff       (20)        0 2023-06-20 09:36:39.188764 smsmanpy-0.0.4/smsmanpy/
--rw-r--r--   0 byrbon     (501) staff       (20)      219 2023-06-15 14:20:27.000000 smsmanpy-0.0.4/smsmanpy/__init__.py
--rw-r--r--   0 byrbon     (501) staff       (20)      481 2023-06-13 07:49:40.000000 smsmanpy-0.0.4/smsmanpy/exeptions.py
--rw-r--r--   0 byrbon     (501) staff       (20)     8673 2023-06-20 09:33:31.000000 smsmanpy-0.0.4/smsmanpy/requests.py
-drwxr-xr-x   0 byrbon     (501) staff       (20)        0 2023-06-20 09:36:39.189640 smsmanpy-0.0.4/smsmanpy.egg-info/
--rw-r--r--   0 byrbon     (501) staff       (20)     2338 2023-06-20 09:36:39.000000 smsmanpy-0.0.4/smsmanpy.egg-info/PKG-INFO
--rw-r--r--   0 byrbon     (501) staff       (20)      251 2023-06-20 09:36:39.000000 smsmanpy-0.0.4/smsmanpy.egg-info/SOURCES.txt
--rw-r--r--   0 byrbon     (501) staff       (20)        1 2023-06-20 09:36:39.000000 smsmanpy-0.0.4/smsmanpy.egg-info/dependency_links.txt
--rw-r--r--   0 byrbon     (501) staff       (20)        8 2023-06-20 09:36:39.000000 smsmanpy-0.0.4/smsmanpy.egg-info/requires.txt
--rw-r--r--   0 byrbon     (501) staff       (20)        9 2023-06-20 09:36:39.000000 smsmanpy-0.0.4/smsmanpy.egg-info/top_level.txt
+drwxr-xr-x   0 byrbon     (501) staff       (20)        0 2023-06-20 09:55:29.219812 smsmanpy-0.0.5/
+-rw-r--r--   0 byrbon     (501) staff       (20)     2330 2023-06-20 09:55:29.219879 smsmanpy-0.0.5/PKG-INFO
+-rw-r--r--   0 byrbon     (501) staff       (20)     1687 2023-06-20 09:53:58.000000 smsmanpy-0.0.5/README.md
+-rw-r--r--   0 byrbon     (501) staff       (20)       38 2023-06-20 09:55:29.220083 smsmanpy-0.0.5/setup.cfg
+-rw-r--r--   0 byrbon     (501) staff       (20)      961 2023-06-20 09:55:23.000000 smsmanpy-0.0.5/setup.py
+drwxr-xr-x   0 byrbon     (501) staff       (20)        0 2023-06-20 09:55:29.218825 smsmanpy-0.0.5/smsmanpy/
+-rw-r--r--   0 byrbon     (501) staff       (20)      219 2023-06-20 09:49:13.000000 smsmanpy-0.0.5/smsmanpy/__init__.py
+-rw-r--r--   0 byrbon     (501) staff       (20)      481 2023-06-13 07:49:40.000000 smsmanpy-0.0.5/smsmanpy/exeptions.py
+-rw-r--r--   0 byrbon     (501) staff       (20)     8674 2023-06-20 09:43:40.000000 smsmanpy-0.0.5/smsmanpy/requests.py
+drwxr-xr-x   0 byrbon     (501) staff       (20)        0 2023-06-20 09:55:29.219670 smsmanpy-0.0.5/smsmanpy.egg-info/
+-rw-r--r--   0 byrbon     (501) staff       (20)     2330 2023-06-20 09:55:29.000000 smsmanpy-0.0.5/smsmanpy.egg-info/PKG-INFO
+-rw-r--r--   0 byrbon     (501) staff       (20)      251 2023-06-20 09:55:29.000000 smsmanpy-0.0.5/smsmanpy.egg-info/SOURCES.txt
+-rw-r--r--   0 byrbon     (501) staff       (20)        1 2023-06-20 09:55:29.000000 smsmanpy-0.0.5/smsmanpy.egg-info/dependency_links.txt
+-rw-r--r--   0 byrbon     (501) staff       (20)        8 2023-06-20 09:55:29.000000 smsmanpy-0.0.5/smsmanpy.egg-info/requires.txt
+-rw-r--r--   0 byrbon     (501) staff       (20)        9 2023-06-20 09:55:29.000000 smsmanpy-0.0.5/smsmanpy.egg-info/top_level.txt
```

### Comparing `smsmanpy-0.0.4/PKG-INFO` & `smsmanpy-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: smsmanpy
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package to simplify work with the sms-man API
-Home-page: https://github.com/smsmancom/smsmanpy/
+Home-page: https://github.com/smsmancom/smsmanpy
 Author: Alexandr Lebedchenko
 Author-email: alex_leb@sms-man.com
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -55,15 +55,15 @@
                                    application_id=1,
                                    amount=10))
 
 #  Receive a SMS to the number
 sms_code = client.get_sms('request_id')
 
 # Reject the number
-print(client.reject_number('request_id'))
+client.reject_number('request_id')
 ```
 
   
 
 ## Contributing
 
 Contributions are welcome.<br/>
```

### Comparing `smsmanpy-0.0.4/README.md` & `smsmanpy-0.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
                                    application_id=1,
                                    amount=10))
 
 #  Receive a SMS to the number
 sms_code = client.get_sms('request_id')
 
 # Reject the number
-print(client.reject_number('request_id'))
+client.reject_number('request_id')
 ```
 
   
 
 ## Contributing
 
 Contributions are welcome.<br/>
```

### Comparing `smsmanpy-0.0.4/setup.py` & `smsmanpy-0.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 requirements = ["aiohttp"]
 
 setup(
     name="smsmanpy",
-    version="0.0.4",
+    version="0.0.5",
     author="Alexandr Lebedchenko",
     author_email="alex_leb@sms-man.com",
     description="A package to simplify work with the sms-man API",
     long_description=readme,
     long_description_content_type="text/markdown",
-    url="https://github.com/smsmancom/smsmanpy/", #url from smsmangithab
+    url="https://github.com/smsmancom/smsmanpy",
     packages=find_packages(),
     install_requires=requirements,
     classifiers=[
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
```

### Comparing `smsmanpy-0.0.4/smsmanpy/requests.py` & `smsmanpy-0.0.5/smsmanpy/requests.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,14 +186,15 @@
 
         return params
 
     async def __reject_number(self, request_id: str):
         """
         Returns the number if it did not receive an SMS. Money is returned to the balance
         :param request_id: Number of IF (get with phone number)
+
         """
         params = self.__check_params(request_id=request_id, status="reject")
 
         async with aiohttp.ClientSession() as session:
             async with session.get(self.__base_url + self.__method_reject_number, params=params) as response:
                 response.raise_for_status()
```

### Comparing `smsmanpy-0.0.4/smsmanpy.egg-info/PKG-INFO` & `smsmanpy-0.0.5/smsmanpy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: smsmanpy
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package to simplify work with the sms-man API
-Home-page: https://github.com/smsmancom/smsmanpy/
+Home-page: https://github.com/smsmancom/smsmanpy
 Author: Alexandr Lebedchenko
 Author-email: alex_leb@sms-man.com
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -55,15 +55,15 @@
                                    application_id=1,
                                    amount=10))
 
 #  Receive a SMS to the number
 sms_code = client.get_sms('request_id')
 
 # Reject the number
-print(client.reject_number('request_id'))
+client.reject_number('request_id')
 ```
 
   
 
 ## Contributing
 
 Contributions are welcome.<br/>
```

