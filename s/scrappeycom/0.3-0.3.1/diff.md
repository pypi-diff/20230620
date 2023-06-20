# Comparing `tmp/scrappeycom-0.3.tar.gz` & `tmp/scrappeycom-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrappeycom-0.3.tar", last modified: Tue Jun 20 06:39:38 2023, max compression
+gzip compressed data, was "scrappeycom-0.3.1.tar", last modified: Tue Jun 20 06:41:34 2023, max compression
```

## Comparing `scrappeycom-0.3.tar` & `scrappeycom-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 06:39:38.375719 scrappeycom-0.3/
--rw-rw-rw-   0        0        0     1088 2023-06-20 06:11:52.000000 scrappeycom-0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     1084 2023-06-20 06:39:38.375719 scrappeycom-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     5149 2023-06-20 06:38:43.000000 scrappeycom-0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 06:39:38.355718 scrappeycom-0.3/scrappeycom/
--rw-rw-rw-   0        0        0     2237 2023-06-20 06:08:34.000000 scrappeycom-0.3/scrappeycom/scrappey.py
--rw-rw-rw-   0        0        0      736 2023-06-20 06:08:30.000000 scrappeycom-0.3/scrappeycom/test.py
-drwxrwxrwx   0        0        0        0 2023-06-20 06:39:38.373719 scrappeycom-0.3/scrappeycom.egg-info/
--rw-rw-rw-   0        0        0     1084 2023-06-20 06:39:38.000000 scrappeycom-0.3/scrappeycom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-06-20 06:39:38.000000 scrappeycom-0.3/scrappeycom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 06:39:38.000000 scrappeycom-0.3/scrappeycom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-20 06:39:38.000000 scrappeycom-0.3/scrappeycom.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-20 06:39:38.000000 scrappeycom-0.3/scrappeycom.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-20 06:39:38.377718 scrappeycom-0.3/setup.cfg
--rw-rw-rw-   0        0        0     2030 2023-06-20 06:39:29.000000 scrappeycom-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 06:41:34.118479 scrappeycom-0.3.1/
+-rw-rw-rw-   0        0        0     1088 2023-06-20 06:11:52.000000 scrappeycom-0.3.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     1074 2023-06-20 06:41:34.119479 scrappeycom-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5178 2023-06-20 06:40:26.000000 scrappeycom-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 06:41:34.105477 scrappeycom-0.3.1/scrappeycom/
+-rw-rw-rw-   0        0        0     2237 2023-06-20 06:08:34.000000 scrappeycom-0.3.1/scrappeycom/scrappey.py
+-rw-rw-rw-   0        0        0      736 2023-06-20 06:08:30.000000 scrappeycom-0.3.1/scrappeycom/test.py
+drwxrwxrwx   0        0        0        0 2023-06-20 06:41:34.117478 scrappeycom-0.3.1/scrappeycom.egg-info/
+-rw-rw-rw-   0        0        0     1074 2023-06-20 06:41:33.000000 scrappeycom-0.3.1/scrappeycom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-06-20 06:41:34.000000 scrappeycom-0.3.1/scrappeycom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 06:41:33.000000 scrappeycom-0.3.1/scrappeycom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-20 06:41:33.000000 scrappeycom-0.3.1/scrappeycom.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-20 06:41:33.000000 scrappeycom-0.3.1/scrappeycom.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-20 06:41:34.120477 scrappeycom-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     2020 2023-06-20 06:41:09.000000 scrappeycom-0.3.1/setup.py
```

### Comparing `scrappeycom-0.3/LICENSE.txt` & `scrappeycom-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scrappeycom-0.3/PKG-INFO` & `scrappeycom-0.3.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: scrappeycom
-Version: 0.3
+Version: 0.3.1
 Summary: An API wrapper for Scrappey.com written in Python (cloudflare bypass & solver)
 Home-page: https://github.com/pim97/scrappey-wrapper-python
-Download-URL: https://github.com/pim97/scrappey-wrapper-python/archive/refs/tags/v_02.tar.gz
+Download-URL: https://github.com/pim97/scrappey-wrapper-python/releases/tag/v_03
 Author: dormic97
 Author-email: crozz-boy@hotmail.com
 License: MIT
 Keywords: captcha,shape,web-scraping,data-extraction,akamai,captcha-solver,incapsula,queue-it,scraping-framework,datadome,scraping-tool,cloudflare-bypass,web-scraping-solution,scraping-library,cloudflare-anti-bot,scraping-service,web-data-extraction,anti-bot-api,perimetex
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `scrappeycom-0.3/README.md` & `scrappeycom-0.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 - [License](#license)
 
 ## Installation
 
 Use pip to install the Scrappey library. 💻
 
 ```shell
-pip install scrappey
+pip install scrappeycom
 ```
 
 ## Usage
 
 Import the Scrappey library in your code. 📦
 
 ```python
-import scrappey
+from scrappeycom.scrappey import Scrappey
 ```
 
 Create an instance of Scrappey by providing your Scrappey API key. 🔑
 
 ```python
 api_key = 'YOUR_API_KEY'
 scrappey_instance = scrappey.Scrappey(api_key)
```

### Comparing `scrappeycom-0.3/scrappeycom/scrappey.py` & `scrappeycom-0.3.1/scrappeycom/scrappey.py`

 * *Files identical despite different names*

### Comparing `scrappeycom-0.3/scrappeycom/test.py` & `scrappeycom-0.3.1/scrappeycom/test.py`

 * *Files identical despite different names*

### Comparing `scrappeycom-0.3/scrappeycom.egg-info/PKG-INFO` & `scrappeycom-0.3.1/scrappeycom.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: scrappeycom
-Version: 0.3
+Version: 0.3.1
 Summary: An API wrapper for Scrappey.com written in Python (cloudflare bypass & solver)
 Home-page: https://github.com/pim97/scrappey-wrapper-python
-Download-URL: https://github.com/pim97/scrappey-wrapper-python/archive/refs/tags/v_02.tar.gz
+Download-URL: https://github.com/pim97/scrappey-wrapper-python/releases/tag/v_03
 Author: dormic97
 Author-email: crozz-boy@hotmail.com
 License: MIT
 Keywords: captcha,shape,web-scraping,data-extraction,akamai,captcha-solver,incapsula,queue-it,scraping-framework,datadome,scraping-tool,cloudflare-bypass,web-scraping-solution,scraping-library,cloudflare-anti-bot,scraping-service,web-data-extraction,anti-bot-api,perimetex
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `scrappeycom-0.3/setup.py` & `scrappeycom-0.3.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
   name = 'scrappeycom',         # How you named your package folder (MyLib)
   packages = ['scrappeycom'],   # Chose the same as "name"
-  version = '0.3',      # Start with a small number and increase it with every change you make
+  version = '0.3.1',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'An API wrapper for Scrappey.com written in Python (cloudflare bypass & solver)',   # Give a short description about your library
   author = 'dormic97',                   # Type in your name
   author_email = 'crozz-boy@hotmail.com',      # Type in your E-Mail
   url = 'https://github.com/pim97/scrappey-wrapper-python',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/pim97/scrappey-wrapper-python/archive/refs/tags/v_02.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/pim97/scrappey-wrapper-python/releases/tag/v_03',    # I explain this later on
   keywords = ["captcha", "shape", "web-scraping", "data-extraction", "akamai", "captcha-solver", "incapsula", "queue-it", "scraping-framework", "datadome", "scraping-tool", "cloudflare-bypass", "web-scraping-solution", "scraping-library", "cloudflare-anti-bot", "scraping-service", "web-data-extraction", "anti-bot-api", "perimetex"],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'requests',
       ],
   classifiers=[
     'Development Status :: 5 - Production/Stable',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
```

