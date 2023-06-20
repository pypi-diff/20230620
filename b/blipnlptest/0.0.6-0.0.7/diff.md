# Comparing `tmp/blipnlptest-0.0.6.tar.gz` & `tmp/blipnlptest-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blipnlptest-0.0.6.tar", last modified: Tue Jun 20 20:59:40 2023, max compression
+gzip compressed data, was "blipnlptest-0.0.7.tar", last modified: Tue Jun 20 21:12:39 2023, max compression
```

## Comparing `blipnlptest-0.0.6.tar` & `blipnlptest-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 20:59:40.972568 blipnlptest-0.0.6/
--rw-rw-rw-   0        0        0     1088 2023-06-20 19:54:30.000000 blipnlptest-0.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0     1796 2023-06-20 20:59:40.971569 blipnlptest-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1303 2023-06-20 19:54:30.000000 blipnlptest-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 20:59:40.941649 blipnlptest-0.0.6/blipnlptest/
-drwxrwxrwx   0        0        0        0 2023-06-20 20:59:40.969574 blipnlptest-0.0.6/blipnlptest/BlipNlpTest.egg-info/
--rw-rw-rw-   0        0        0     1796 2023-06-20 20:59:40.000000 blipnlptest-0.0.6/blipnlptest/BlipNlpTest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      549 2023-06-20 20:59:40.000000 blipnlptest-0.0.6/blipnlptest/BlipNlpTest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 20:59:40.000000 blipnlptest-0.0.6/blipnlptest/BlipNlpTest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-06-20 20:59:40.000000 blipnlptest-0.0.6/blipnlptest/BlipNlpTest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-20 20:59:40.000000 blipnlptest-0.0.6/blipnlptest/BlipNlpTest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       25 2023-06-20 20:58:10.000000 blipnlptest-0.0.6/blipnlptest/__init__.py
--rw-rw-rw-   0        0        0     1309 2023-06-20 20:31:10.000000 blipnlptest-0.0.6/blipnlptest/blipnlptest.py
--rw-rw-rw-   0        0        0       42 2023-06-20 20:59:40.972568 blipnlptest-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      783 2023-06-20 20:59:35.000000 blipnlptest-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 21:12:39.102443 blipnlptest-0.0.7/
+-rw-rw-rw-   0        0        0     1088 2023-06-20 19:54:30.000000 blipnlptest-0.0.7/LICENSE.txt
+-rw-rw-rw-   0        0        0     1796 2023-06-20 21:12:39.100452 blipnlptest-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1303 2023-06-20 19:54:30.000000 blipnlptest-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 21:12:39.077991 blipnlptest-0.0.7/blipnlptest/
+drwxrwxrwx   0        0        0        0 2023-06-20 21:12:39.096457 blipnlptest-0.0.7/blipnlptest/BlipNlpTest.egg-info/
+-rw-rw-rw-   0        0        0     1796 2023-06-20 21:12:38.000000 blipnlptest-0.0.7/blipnlptest/BlipNlpTest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      549 2023-06-20 21:12:39.000000 blipnlptest-0.0.7/blipnlptest/BlipNlpTest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 21:12:38.000000 blipnlptest-0.0.7/blipnlptest/BlipNlpTest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-06-20 21:12:38.000000 blipnlptest-0.0.7/blipnlptest/BlipNlpTest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-20 21:12:38.000000 blipnlptest-0.0.7/blipnlptest/BlipNlpTest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       43 2023-06-20 21:12:16.000000 blipnlptest-0.0.7/blipnlptest/__init__.py
+-rw-rw-rw-   0        0        0     1312 2023-06-20 21:11:33.000000 blipnlptest-0.0.7/blipnlptest/blipnlptest.py
+-rw-rw-rw-   0        0        0       42 2023-06-20 21:12:39.102443 blipnlptest-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      783 2023-06-20 21:12:32.000000 blipnlptest-0.0.7/setup.py
```

### Comparing `blipnlptest-0.0.6/LICENSE.txt` & `blipnlptest-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blipnlptest-0.0.6/PKG-INFO` & `blipnlptest-0.0.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blipnlptest
-Version: 0.0.6
+Version: 0.0.7
 Summary: Teste dos provedores integrados na plataforma em conjunto com o Assistente de Conteudo.
 Author: Caio Souza
 Author-email: caios@take.net
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `blipnlptest-0.0.6/README.md` & `blipnlptest-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `blipnlptest-0.0.6/blipnlptest/BlipNlpTest.egg-info/PKG-INFO` & `blipnlptest-0.0.7/blipnlptest/BlipNlpTest.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blipnlptest
-Version: 0.0.6
+Version: 0.0.7
 Summary: Teste dos provedores integrados na plataforma em conjunto com o Assistente de Conteudo.
 Author: Caio Souza
 Author-email: caios@take.net
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `blipnlptest-0.0.6/blipnlptest/BlipNlpTest.egg-info/SOURCES.txt` & `blipnlptest-0.0.7/blipnlptest/BlipNlpTest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blipnlptest-0.0.6/blipnlptest/blipnlptest.py` & `blipnlptest-0.0.7/blipnlptest/blipnlptest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 import json
 import pandas as pd
 
-class blipnlptest:
+class ContentChecker:
 
   def __init__(self, data, key):
       self.data = data
       self.key = key
 
       if isinstance(data, pd.DataFrame) == False:
         print(f'Ao invés de "{data}", favor inserir um DataFrame. A coluna com o texto deve ter o cabeçalho com o nome "Text".')
```

### Comparing `blipnlptest-0.0.6/setup.py` & `blipnlptest-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md","r", encoding="utf-8") as fh:
 	long_description = fh.read()
 	
 setuptools.setup(
   name = "blipnlptest",
-  version = "0.0.6",
+  version = "0.0.7",
   author = "Caio Souza",
   author_email = "caios@take.net",
   description = "Teste dos provedores integrados na plataforma em conjunto com o Assistente de Conteudo.",
   long_description = long_description,
   long_description_content_type="text/markdown",
   keywords = [],
   install_requires=[
```

