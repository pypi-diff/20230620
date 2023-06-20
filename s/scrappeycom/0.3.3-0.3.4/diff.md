# Comparing `tmp/scrappeycom-0.3.3.tar.gz` & `tmp/scrappeycom-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrappeycom-0.3.3.tar", last modified: Tue Jun 20 07:13:35 2023, max compression
+gzip compressed data, was "scrappeycom-0.3.4.tar", last modified: Tue Jun 20 07:19:58 2023, max compression
```

## Comparing `scrappeycom-0.3.3.tar` & `scrappeycom-0.3.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 07:13:35.322086 scrappeycom-0.3.3/
--rw-rw-rw-   0        0        0     1088 2023-06-20 06:11:52.000000 scrappeycom-0.3.3/LICENSE.txt
--rw-rw-rw-   0        0        0     6333 2023-06-20 07:13:35.323085 scrappeycom-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     5178 2023-06-20 06:40:26.000000 scrappeycom-0.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 07:13:35.300085 scrappeycom-0.3.3/scrappeycom/
--rw-rw-rw-   0        0        0     2258 2023-06-20 07:12:11.000000 scrappeycom-0.3.3/scrappeycom/scrappey.py
--rw-rw-rw-   0        0        0      727 2023-06-20 07:12:58.000000 scrappeycom-0.3.3/scrappeycom/test.py
-drwxrwxrwx   0        0        0        0 2023-06-20 07:13:35.321090 scrappeycom-0.3.3/scrappeycom.egg-info/
--rw-rw-rw-   0        0        0     6333 2023-06-20 07:13:35.000000 scrappeycom-0.3.3/scrappeycom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-06-20 07:13:35.000000 scrappeycom-0.3.3/scrappeycom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 07:13:35.000000 scrappeycom-0.3.3/scrappeycom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-20 07:13:35.000000 scrappeycom-0.3.3/scrappeycom.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-20 07:13:35.000000 scrappeycom-0.3.3/scrappeycom.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-20 07:13:35.324087 scrappeycom-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0     2259 2023-06-20 07:13:21.000000 scrappeycom-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 07:19:58.512641 scrappeycom-0.3.4/
+-rw-rw-rw-   0        0        0     1088 2023-06-20 06:11:52.000000 scrappeycom-0.3.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     6333 2023-06-20 07:19:58.512641 scrappeycom-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5178 2023-06-20 06:40:26.000000 scrappeycom-0.3.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 07:19:58.496638 scrappeycom-0.3.4/scrappeycom/
+-rw-rw-rw-   0        0        0     2258 2023-06-20 07:12:11.000000 scrappeycom-0.3.4/scrappeycom/scrappey.py
+-rw-rw-rw-   0        0        0      727 2023-06-20 07:12:58.000000 scrappeycom-0.3.4/scrappeycom/test.py
+drwxrwxrwx   0        0        0        0 2023-06-20 07:19:58.511641 scrappeycom-0.3.4/scrappeycom.egg-info/
+-rw-rw-rw-   0        0        0     6333 2023-06-20 07:19:58.000000 scrappeycom-0.3.4/scrappeycom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-06-20 07:19:58.000000 scrappeycom-0.3.4/scrappeycom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 07:19:58.000000 scrappeycom-0.3.4/scrappeycom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-20 07:19:58.000000 scrappeycom-0.3.4/scrappeycom.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-20 07:19:58.000000 scrappeycom-0.3.4/scrappeycom.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-20 07:19:58.513641 scrappeycom-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     2238 2023-06-20 07:19:43.000000 scrappeycom-0.3.4/setup.py
```

### Comparing `scrappeycom-0.3.3/LICENSE.txt` & `scrappeycom-0.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scrappeycom-0.3.3/PKG-INFO` & `scrappeycom-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrappeycom
-Version: 0.3.3
+Version: 0.3.4
 Summary: An API wrapper for Scrappey.com written in Python (cloudflare bypass & solver)
 Home-page: https://github.com/pim97/scrappey-wrapper-python
 Download-URL: https://github.com/pim97/scrappey-wrapper-python/releases/tag/v_03
 Author: dormic97
 Author-email: crozz-boy@hotmail.com
 License: MIT
 Keywords: captcha,shape,web-scraping,data-extraction,akamai,captcha-solver,incapsula,queue-it,scraping-framework,datadome,scraping-tool,cloudflare-bypass,web-scraping-solution,scraping-library,cloudflare-anti-bot,scraping-service,web-data-extraction,anti-bot-api,perimetex
```

### Comparing `scrappeycom-0.3.3/README.md` & `scrappeycom-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `scrappeycom-0.3.3/scrappeycom/scrappey.py` & `scrappeycom-0.3.4/scrappeycom/scrappey.py`

 * *Files identical despite different names*

### Comparing `scrappeycom-0.3.3/scrappeycom/test.py` & `scrappeycom-0.3.4/scrappeycom/test.py`

 * *Files identical despite different names*

### Comparing `scrappeycom-0.3.3/scrappeycom.egg-info/PKG-INFO` & `scrappeycom-0.3.4/scrappeycom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrappeycom
-Version: 0.3.3
+Version: 0.3.4
 Summary: An API wrapper for Scrappey.com written in Python (cloudflare bypass & solver)
 Home-page: https://github.com/pim97/scrappey-wrapper-python
 Download-URL: https://github.com/pim97/scrappey-wrapper-python/releases/tag/v_03
 Author: dormic97
 Author-email: crozz-boy@hotmail.com
 License: MIT
 Keywords: captcha,shape,web-scraping,data-extraction,akamai,captcha-solver,incapsula,queue-it,scraping-framework,datadome,scraping-tool,cloudflare-bypass,web-scraping-solution,scraping-library,cloudflare-anti-bot,scraping-service,web-data-extraction,anti-bot-api,perimetex
```

### Comparing `scrappeycom-0.3.3/setup.py` & `scrappeycom-0.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,26 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
   name = 'scrappeycom',         # How you named your package folder (MyLib)
   packages = ['scrappeycom'],   # Chose the same as "name"
-  version = '0.3.3',      # Start with a small number and increase it with every change you make
+  version = '0.3.4',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'An API wrapper for Scrappey.com written in Python (cloudflare bypass & solver)',   # Give a short description about your library
   author = 'dormic97',                   # Type in your name
   author_email = 'crozz-boy@hotmail.com',      # Type in your E-Mail
   url = 'https://github.com/pim97/scrappey-wrapper-python',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/pim97/scrappey-wrapper-python/releases/tag/v_03',    # I explain this later on
   keywords = ["captcha", "shape", "web-scraping", "data-extraction", "akamai", "captcha-solver", "incapsula", "queue-it", "scraping-framework", "datadome", "scraping-tool", "cloudflare-bypass", "web-scraping-solution", "scraping-library", "cloudflare-anti-bot", "scraping-service", "web-data-extraction", "anti-bot-api", "perimetex"],   # Keywords that define your package best
   long_description=long_description,
   long_description_content_type='text/markdown',
   install_requires=[            # I get to this in a second
-          'requests',
-          'urllib'
+          'requests'
       ],
   classifiers=[
     'Development Status :: 5 - Production/Stable',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   # Again, pick a license
     'Programming Language :: Python :: 3',      #Specify which pyhton versions that you want to support
```

