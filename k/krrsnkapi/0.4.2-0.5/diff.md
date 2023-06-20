# Comparing `tmp/krrsnkapi-0.4.2.tar.gz` & `tmp/krrsnkapi-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krrsnkapi-0.4.2.tar", last modified: Mon Jun 19 20:18:19 2023, max compression
+gzip compressed data, was "krrsnkapi-0.5.tar", last modified: Tue Jun 20 20:56:29 2023, max compression
```

## Comparing `krrsnkapi-0.4.2.tar` & `krrsnkapi-0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 20:18:19.108087 krrsnkapi-0.4.2/
--rw-rw-rw-   0        0        0     1087 2023-04-13 13:12:53.000000 krrsnkapi-0.4.2/LICENSE.txt
--rw-rw-rw-   0        0        0      621 2023-06-19 20:18:19.109087 krrsnkapi-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     1569 2023-04-13 12:53:07.000000 krrsnkapi-0.4.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 20:18:19.090086 krrsnkapi-0.4.2/krrsnkapi/
--rw-rw-rw-   0        0        0       52 2023-06-19 20:08:00.000000 krrsnkapi-0.4.2/krrsnkapi/__init__.py
--rw-rw-rw-   0        0        0     2556 2023-06-19 20:14:35.000000 krrsnkapi-0.4.2/krrsnkapi/krrsnkapi.py
-drwxrwxrwx   0        0        0        0 2023-06-19 20:18:19.105087 krrsnkapi-0.4.2/krrsnkapi.egg-info/
--rw-rw-rw-   0        0        0      621 2023-06-19 20:18:18.000000 krrsnkapi-0.4.2/krrsnkapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-06-19 20:18:18.000000 krrsnkapi-0.4.2/krrsnkapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 20:18:18.000000 krrsnkapi-0.4.2/krrsnkapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-19 20:18:18.000000 krrsnkapi-0.4.2/krrsnkapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-19 20:18:18.000000 krrsnkapi-0.4.2/krrsnkapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-19 20:18:19.111087 krrsnkapi-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0     1449 2023-06-19 20:17:17.000000 krrsnkapi-0.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 20:56:29.210235 krrsnkapi-0.5/
+-rw-rw-rw-   0        0        0     1087 2023-04-13 13:12:53.000000 krrsnkapi-0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      617 2023-06-20 20:56:29.210235 krrsnkapi-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1569 2023-04-13 12:53:07.000000 krrsnkapi-0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 20:56:29.179035 krrsnkapi-0.5/krrsnkapi/
+-rw-rw-rw-   0        0        0       52 2023-06-19 20:08:00.000000 krrsnkapi-0.5/krrsnkapi/__init__.py
+-rw-rw-rw-   0        0        0     3086 2023-06-20 20:52:10.000000 krrsnkapi-0.5/krrsnkapi/krrsnkapi.py
+drwxrwxrwx   0        0        0        0 2023-06-20 20:56:29.194635 krrsnkapi-0.5/krrsnkapi.egg-info/
+-rw-rw-rw-   0        0        0      617 2023-06-20 20:56:28.000000 krrsnkapi-0.5/krrsnkapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-06-20 20:56:28.000000 krrsnkapi-0.5/krrsnkapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 20:56:28.000000 krrsnkapi-0.5/krrsnkapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-20 20:56:28.000000 krrsnkapi-0.5/krrsnkapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-20 20:56:28.000000 krrsnkapi-0.5/krrsnkapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-20 20:56:29.210235 krrsnkapi-0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1445 2023-06-20 20:56:18.000000 krrsnkapi-0.5/setup.py
```

### Comparing `krrsnkapi-0.4.2/LICENSE.txt` & `krrsnkapi-0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `krrsnkapi-0.4.2/PKG-INFO` & `krrsnkapi-0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: krrsnkapi
-Version: 0.4.2
+Version: 0.5
 Summary: Module for easy use of my api | info on GitHub: https://github.com/kararasenok-gd/krrsnkapi
 Home-page: https://github.com/kararasenok-gd/krrsnkapi
-Download-URL: https://github.com/kararasenok-gd/krrsnkapi/archive/v0.4.2.tar.gz
+Download-URL: https://github.com/kararasenok-gd/krrsnkapi/archive/v0.5.tar.gz
 Author: kararasenok_gd
 Author-email: murzikkurzikpro@gmail.com
 License: MIT
 Keywords: api
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `krrsnkapi-0.4.2/README.md` & `krrsnkapi-0.5/README.md`

 * *Files identical despite different names*

### Comparing `krrsnkapi-0.4.2/krrsnkapi/krrsnkapi.py` & `krrsnkapi-0.5/krrsnkapi/krrsnkapi.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import requests
+import json
+import random
 
 class Chat:
 	def __init__(self, apikey):
 		self.apikey = apikey
 
 	def send_message(self, message):
 		self.message = message
@@ -91,14 +93,29 @@
 
 		return self.response.text
 
 class r34:
 	def __init__(self, apikey):
 		self.apikey = apikey
 
-	def get_url(self, keyword, page = 0):
+	def get_url(self, keyword, page = 0, use_r34_api = False):
 		self.keyword = keyword
 		self.page = page
+		self.use_r34_api = use_r34_api
 
-		self.response = requests.post(f"https://kararasenok.ueuo.com/api/v1/r34/?keyword={self.keyword}&apikey={self.apikey}&page={self.page}")
+		if self.use_r34_api is False:
+			self.response = requests.post(f"https://kararasenok.ueuo.com/api/v1/r34/?keyword={self.keyword}&apikey={self.apikey}&page={self.page}")
+		else:
+			self.response = requests.post(f"https://api.rule34.xxx/index.php?page=dapi&s=post&q=index&tags={self.keyword}&pid={self.page}&json=1&limit=1000")
 
 		return self.response.text
+
+	def get_img_link(self, json_data):
+		self.json_data = json_data
+
+		self.data = json.loads(self.json_data)
+
+		self.random_object = random.choice(self.data)
+
+		self.random_fileurl = self.random_object['file_url']
+
+		return self.random_fileurl
```

### Comparing `krrsnkapi-0.4.2/krrsnkapi.egg-info/PKG-INFO` & `krrsnkapi-0.5/krrsnkapi.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: krrsnkapi
-Version: 0.4.2
+Version: 0.5
 Summary: Module for easy use of my api | info on GitHub: https://github.com/kararasenok-gd/krrsnkapi
 Home-page: https://github.com/kararasenok-gd/krrsnkapi
-Download-URL: https://github.com/kararasenok-gd/krrsnkapi/archive/v0.4.2.tar.gz
+Download-URL: https://github.com/kararasenok-gd/krrsnkapi/archive/v0.5.tar.gz
 Author: kararasenok_gd
 Author-email: murzikkurzikpro@gmail.com
 License: MIT
 Keywords: api
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `krrsnkapi-0.4.2/setup.py` & `krrsnkapi-0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 
 # ver = input("version: ")
 
 setup(
   name = 'krrsnkapi',         # How you named your package folder (MyLib)
   packages = ['krrsnkapi'],   # Chose the same as "name"
-  version = "0.4.2",      # Start with a small number and increase it with every change you make
+  version = "0.5",      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Module for easy use of my api | info on GitHub: https://github.com/kararasenok-gd/krrsnkapi',   # Give a short description about your library
   author = 'kararasenok_gd',                   # Type in your name
   author_email = 'murzikkurzikpro@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/kararasenok-gd/krrsnkapi',   # Provide either the link to your github or to your website
-  download_url = f'https://github.com/kararasenok-gd/krrsnkapi/archive/v0.4.2.tar.gz',    # I explain this later on
+  download_url = f'https://github.com/kararasenok-gd/krrsnkapi/archive/v0.5.tar.gz',    # I explain this later on
   keywords = ["api"],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'requests'
       ],
   classifiers=[
     'Development Status :: 4 - Beta',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Topic :: Software Development :: Build Tools',
```

