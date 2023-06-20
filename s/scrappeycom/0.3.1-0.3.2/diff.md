# Comparing `tmp/scrappeycom-0.3.1.tar.gz` & `tmp/scrappeycom-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrappeycom-0.3.1.tar", last modified: Tue Jun 20 06:41:34 2023, max compression
+gzip compressed data, was "scrappeycom-0.3.2.tar", last modified: Tue Jun 20 06:55:44 2023, max compression
```

## Comparing `scrappeycom-0.3.1.tar` & `scrappeycom-0.3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 06:41:34.118479 scrappeycom-0.3.1/
--rw-rw-rw-   0        0        0     1088 2023-06-20 06:11:52.000000 scrappeycom-0.3.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1074 2023-06-20 06:41:34.119479 scrappeycom-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     5178 2023-06-20 06:40:26.000000 scrappeycom-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 06:41:34.105477 scrappeycom-0.3.1/scrappeycom/
--rw-rw-rw-   0        0        0     2237 2023-06-20 06:08:34.000000 scrappeycom-0.3.1/scrappeycom/scrappey.py
--rw-rw-rw-   0        0        0      736 2023-06-20 06:08:30.000000 scrappeycom-0.3.1/scrappeycom/test.py
-drwxrwxrwx   0        0        0        0 2023-06-20 06:41:34.117478 scrappeycom-0.3.1/scrappeycom.egg-info/
--rw-rw-rw-   0        0        0     1074 2023-06-20 06:41:33.000000 scrappeycom-0.3.1/scrappeycom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-06-20 06:41:34.000000 scrappeycom-0.3.1/scrappeycom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 06:41:33.000000 scrappeycom-0.3.1/scrappeycom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-20 06:41:33.000000 scrappeycom-0.3.1/scrappeycom.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-20 06:41:33.000000 scrappeycom-0.3.1/scrappeycom.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-20 06:41:34.120477 scrappeycom-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     2020 2023-06-20 06:41:09.000000 scrappeycom-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 06:55:44.395133 scrappeycom-0.3.2/
+-rw-rw-rw-   0        0        0     1088 2023-06-20 06:11:52.000000 scrappeycom-0.3.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     6333 2023-06-20 06:55:44.395133 scrappeycom-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5178 2023-06-20 06:40:26.000000 scrappeycom-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 06:55:44.379131 scrappeycom-0.3.2/scrappeycom/
+-rw-rw-rw-   0        0        0     2237 2023-06-20 06:08:34.000000 scrappeycom-0.3.2/scrappeycom/scrappey.py
+-rw-rw-rw-   0        0        0      736 2023-06-20 06:08:30.000000 scrappeycom-0.3.2/scrappeycom/test.py
+drwxrwxrwx   0        0        0        0 2023-06-20 06:55:44.394135 scrappeycom-0.3.2/scrappeycom.egg-info/
+-rw-rw-rw-   0        0        0     6333 2023-06-20 06:55:44.000000 scrappeycom-0.3.2/scrappeycom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-06-20 06:55:44.000000 scrappeycom-0.3.2/scrappeycom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 06:55:44.000000 scrappeycom-0.3.2/scrappeycom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-20 06:55:44.000000 scrappeycom-0.3.2/scrappeycom.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-20 06:55:44.000000 scrappeycom-0.3.2/scrappeycom.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-20 06:55:44.396132 scrappeycom-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     2239 2023-06-20 06:55:42.000000 scrappeycom-0.3.2/setup.py
```

### Comparing `scrappeycom-0.3.1/LICENSE.txt` & `scrappeycom-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scrappeycom-0.3.1/README.md` & `scrappeycom-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `scrappeycom-0.3.1/scrappeycom/scrappey.py` & `scrappeycom-0.3.2/scrappeycom/scrappey.py`

 * *Files identical despite different names*

### Comparing `scrappeycom-0.3.1/scrappeycom/test.py` & `scrappeycom-0.3.2/scrappeycom/test.py`

 * *Files identical despite different names*

### Comparing `scrappeycom-0.3.1/setup.py` & `scrappeycom-0.3.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 from distutils.core import setup
+from pathlib import Path
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
+
 setup(
   name = 'scrappeycom',         # How you named your package folder (MyLib)
   packages = ['scrappeycom'],   # Chose the same as "name"
-  version = '0.3.1',      # Start with a small number and increase it with every change you make
+  version = '0.3.2',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'An API wrapper for Scrappey.com written in Python (cloudflare bypass & solver)',   # Give a short description about your library
   author = 'dormic97',                   # Type in your name
   author_email = 'crozz-boy@hotmail.com',      # Type in your E-Mail
   url = 'https://github.com/pim97/scrappey-wrapper-python',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/pim97/scrappey-wrapper-python/releases/tag/v_03',    # I explain this later on
   keywords = ["captcha", "shape", "web-scraping", "data-extraction", "akamai", "captcha-solver", "incapsula", "queue-it", "scraping-framework", "datadome", "scraping-tool", "cloudflare-bypass", "web-scraping-solution", "scraping-library", "cloudflare-anti-bot", "scraping-service", "web-data-extraction", "anti-bot-api", "perimetex"],   # Keywords that define your package best
+  long_description=long_description,
+  long_description_content_type='text/markdown',
   install_requires=[            # I get to this in a second
           'requests',
       ],
   classifiers=[
     'Development Status :: 5 - Production/Stable',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
```

