# Comparing `tmp/BlipNlpTest-0.0.2.tar.gz` & `tmp/BlipNlpTest-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BlipNlpTest-0.0.2.tar", last modified: Tue Jun 20 20:12:19 2023, max compression
+gzip compressed data, was "BlipNlpTest-0.0.3.tar", last modified: Tue Jun 20 20:18:24 2023, max compression
```

## Comparing `BlipNlpTest-0.0.2.tar` & `BlipNlpTest-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 20:12:19.487287 BlipNlpTest-0.0.2/
--rw-rw-rw-   0        0        0     1088 2023-06-20 19:54:30.000000 BlipNlpTest-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     1796 2023-06-20 20:12:19.486291 BlipNlpTest-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1303 2023-06-20 19:54:30.000000 BlipNlpTest-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 20:12:19.464312 BlipNlpTest-0.0.2/blipnlptest/
-drwxrwxrwx   0        0        0        0 2023-06-20 20:12:19.485293 BlipNlpTest-0.0.2/blipnlptest/BlipNlpTest.egg-info/
--rw-rw-rw-   0        0        0     1796 2023-06-20 20:12:19.000000 BlipNlpTest-0.0.2/blipnlptest/BlipNlpTest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-06-20 20:12:19.000000 BlipNlpTest-0.0.2/blipnlptest/BlipNlpTest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 20:12:19.000000 BlipNlpTest-0.0.2/blipnlptest/BlipNlpTest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-06-20 20:12:19.000000 BlipNlpTest-0.0.2/blipnlptest/BlipNlpTest.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 20:12:19.000000 BlipNlpTest-0.0.2/blipnlptest/BlipNlpTest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 20:12:19.487287 BlipNlpTest-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      835 2023-06-20 20:10:16.000000 BlipNlpTest-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 20:18:24.419088 BlipNlpTest-0.0.3/
+-rw-rw-rw-   0        0        0     1088 2023-06-20 19:54:30.000000 BlipNlpTest-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     1796 2023-06-20 20:18:24.419088 BlipNlpTest-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1303 2023-06-20 19:54:30.000000 BlipNlpTest-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 20:18:24.404113 BlipNlpTest-0.0.3/blipnlptest/
+drwxrwxrwx   0        0        0        0 2023-06-20 20:18:24.417078 BlipNlpTest-0.0.3/blipnlptest/BlipNlpTest.egg-info/
+-rw-rw-rw-   0        0        0     1796 2023-06-20 20:18:23.000000 BlipNlpTest-0.0.3/blipnlptest/BlipNlpTest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-06-20 20:18:24.000000 BlipNlpTest-0.0.3/blipnlptest/BlipNlpTest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 20:18:24.000000 BlipNlpTest-0.0.3/blipnlptest/BlipNlpTest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-06-20 20:18:24.000000 BlipNlpTest-0.0.3/blipnlptest/BlipNlpTest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 20:18:24.000000 BlipNlpTest-0.0.3/blipnlptest/BlipNlpTest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 20:18:24.420071 BlipNlpTest-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      835 2023-06-20 20:17:42.000000 BlipNlpTest-0.0.3/setup.py
```

### Comparing `BlipNlpTest-0.0.2/LICENSE.txt` & `BlipNlpTest-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `BlipNlpTest-0.0.2/PKG-INFO` & `BlipNlpTest-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BlipNlpTest
-Version: 0.0.2
+Version: 0.0.3
 Summary: Teste dos provedores integrados na plataforma em conjunto com o Assistente de Conteudo.
 Author: Caio Souza
 Author-email: caios@take.net
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `BlipNlpTest-0.0.2/README.md` & `BlipNlpTest-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `BlipNlpTest-0.0.2/blipnlptest/BlipNlpTest.egg-info/PKG-INFO` & `BlipNlpTest-0.0.3/blipnlptest/BlipNlpTest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BlipNlpTest
-Version: 0.0.2
+Version: 0.0.3
 Summary: Teste dos provedores integrados na plataforma em conjunto com o Assistente de Conteudo.
 Author: Caio Souza
 Author-email: caios@take.net
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `BlipNlpTest-0.0.2/setup.py` & `BlipNlpTest-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md","r", encoding="utf-8") as fh:
 	long_description = fh.read()
 	
 setuptools.setup(
   name = "BlipNlpTest",
-  version = "0.0.2",
+  version = "0.0.3",
   author = "Caio Souza",
   author_email = "caios@take.net",
   description = "Teste dos provedores integrados na plataforma em conjunto com o Assistente de Conteudo.",
   long_description = long_description,
   long_description_content_type="text/markdown",
   keywords = [],
   install_requires=[
```
