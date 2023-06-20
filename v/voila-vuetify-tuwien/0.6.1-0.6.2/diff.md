# Comparing `tmp/voila-vuetify-tuwien-0.6.1.tar.gz` & `tmp/voila-vuetify-tuwien-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voila-vuetify-tuwien-0.6.1.tar", last modified: Tue Jun 20 12:44:17 2023, max compression
+gzip compressed data, was "voila-vuetify-tuwien-0.6.2.tar", last modified: Tue Jun 20 12:48:53 2023, max compression
```

## Comparing `voila-vuetify-tuwien-0.6.1.tar` & `voila-vuetify-tuwien-0.6.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-20 12:44:17.410409 voila-vuetify-tuwien-0.6.1/
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     1545 2023-06-16 13:39:42.000000 voila-vuetify-tuwien-0.6.1/LICENSE
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)       16 2023-06-16 13:39:42.000000 voila-vuetify-tuwien-0.6.1/MANIFEST.in
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)      344 2023-06-20 12:44:17.410409 voila-vuetify-tuwien-0.6.1/PKG-INFO
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     1574 2023-06-16 13:39:42.000000 voila-vuetify-tuwien-0.6.1/README.md
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)      101 2023-06-20 12:44:17.410409 voila-vuetify-tuwien-0.6.1/setup.cfg
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     3363 2023-06-20 12:44:08.000000 voila-vuetify-tuwien-0.6.1/setup.py
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-20 12:44:17.410409 voila-vuetify-tuwien-0.6.1/share/
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-20 12:44:17.410409 voila-vuetify-tuwien-0.6.1/share/jupyter/
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-20 12:44:17.410409 voila-vuetify-tuwien-0.6.1/share/jupyter/nbconvert/
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-20 12:44:17.410409 voila-vuetify-tuwien-0.6.1/share/jupyter/nbconvert/templates/
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-20 12:44:17.410409 voila-vuetify-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-tuwien/
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     7797 2023-06-16 13:39:42.000000 voila-vuetify-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-tuwien/ansi.js
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     1434 2023-06-16 13:39:42.000000 voila-vuetify-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-tuwien/app.html
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)       25 2023-06-19 13:49:52.000000 voila-vuetify-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-tuwien/conf.json
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     3209 2023-06-20 12:43:26.000000 voila-vuetify-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-tuwien/index.html.j2
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     7280 2023-06-16 13:39:42.000000 voila-vuetify-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-tuwien/util.js
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-20 12:44:17.410409 voila-vuetify-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-default-tuwien/
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     6408 2023-06-20 10:49:16.000000 voila-vuetify-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-default-tuwien/app.html
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)       40 2023-06-20 11:41:15.000000 voila-vuetify-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-default-tuwien/conf.json
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-20 12:44:17.410409 voila-vuetify-tuwien-0.6.1/share/jupyter/voila/
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-20 12:44:17.410409 voila-vuetify-tuwien-0.6.1/share/jupyter/voila/templates/
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-20 12:44:17.410409 voila-vuetify-tuwien-0.6.1/share/jupyter/voila/templates/vuetify-base-tuwien/
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     1764 2023-06-20 12:16:19.000000 voila-vuetify-tuwien-0.6.1/share/jupyter/voila/templates/vuetify-base-tuwien/index.html.j2
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-20 12:44:17.410409 voila-vuetify-tuwien-0.6.1/voila_vuetify_tuwien.egg-info/
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)      344 2023-06-20 12:44:17.000000 voila-vuetify-tuwien-0.6.1/voila_vuetify_tuwien.egg-info/PKG-INFO
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)      783 2023-06-20 12:44:17.000000 voila-vuetify-tuwien-0.6.1/voila_vuetify_tuwien.egg-info/SOURCES.txt
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)        1 2023-06-20 12:44:17.000000 voila-vuetify-tuwien-0.6.1/voila_vuetify_tuwien.egg-info/dependency_links.txt
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)       20 2023-06-20 12:44:17.000000 voila-vuetify-tuwien-0.6.1/voila_vuetify_tuwien.egg-info/requires.txt
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)        6 2023-06-20 12:44:17.000000 voila-vuetify-tuwien-0.6.1/voila_vuetify_tuwien.egg-info/top_level.txt
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-20 12:48:53.984549 voila-vuetify-tuwien-0.6.2/
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     1545 2023-06-16 13:39:42.000000 voila-vuetify-tuwien-0.6.2/LICENSE
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)       16 2023-06-16 13:39:42.000000 voila-vuetify-tuwien-0.6.2/MANIFEST.in
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)      344 2023-06-20 12:48:53.984549 voila-vuetify-tuwien-0.6.2/PKG-INFO
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     1574 2023-06-16 13:39:42.000000 voila-vuetify-tuwien-0.6.2/README.md
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)      101 2023-06-20 12:48:53.984549 voila-vuetify-tuwien-0.6.2/setup.cfg
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     3363 2023-06-20 12:48:36.000000 voila-vuetify-tuwien-0.6.2/setup.py
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-20 12:48:53.984549 voila-vuetify-tuwien-0.6.2/share/
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-20 12:48:53.984549 voila-vuetify-tuwien-0.6.2/share/jupyter/
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-20 12:48:53.984549 voila-vuetify-tuwien-0.6.2/share/jupyter/nbconvert/
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-20 12:48:53.984549 voila-vuetify-tuwien-0.6.2/share/jupyter/nbconvert/templates/
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-20 12:48:53.984549 voila-vuetify-tuwien-0.6.2/share/jupyter/nbconvert/templates/vuetify-base-tuwien/
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     7797 2023-06-20 12:45:40.000000 voila-vuetify-tuwien-0.6.2/share/jupyter/nbconvert/templates/vuetify-base-tuwien/ansi.js
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     1434 2023-06-20 12:45:40.000000 voila-vuetify-tuwien-0.6.2/share/jupyter/nbconvert/templates/vuetify-base-tuwien/app.html
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)       25 2023-06-20 12:45:40.000000 voila-vuetify-tuwien-0.6.2/share/jupyter/nbconvert/templates/vuetify-base-tuwien/conf.json
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     3209 2023-06-20 12:45:40.000000 voila-vuetify-tuwien-0.6.2/share/jupyter/nbconvert/templates/vuetify-base-tuwien/index.html.j2
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     7280 2023-06-20 12:45:40.000000 voila-vuetify-tuwien-0.6.2/share/jupyter/nbconvert/templates/vuetify-base-tuwien/util.js
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-20 12:48:53.984549 voila-vuetify-tuwien-0.6.2/share/jupyter/nbconvert/templates/vuetify-default-tuwien/
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     6408 2023-06-20 12:45:40.000000 voila-vuetify-tuwien-0.6.2/share/jupyter/nbconvert/templates/vuetify-default-tuwien/app.html
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)       40 2023-06-20 12:45:40.000000 voila-vuetify-tuwien-0.6.2/share/jupyter/nbconvert/templates/vuetify-default-tuwien/conf.json
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-20 12:48:53.984549 voila-vuetify-tuwien-0.6.2/share/jupyter/voila/
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-20 12:48:53.984549 voila-vuetify-tuwien-0.6.2/share/jupyter/voila/templates/
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-20 12:48:53.984549 voila-vuetify-tuwien-0.6.2/share/jupyter/voila/templates/vuetify-base-tuwien/
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     1764 2023-06-20 12:45:40.000000 voila-vuetify-tuwien-0.6.2/share/jupyter/voila/templates/vuetify-base-tuwien/index.html.j2
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-20 12:48:53.984549 voila-vuetify-tuwien-0.6.2/voila_vuetify_tuwien.egg-info/
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)      344 2023-06-20 12:48:53.000000 voila-vuetify-tuwien-0.6.2/voila_vuetify_tuwien.egg-info/PKG-INFO
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)      783 2023-06-20 12:48:53.000000 voila-vuetify-tuwien-0.6.2/voila_vuetify_tuwien.egg-info/SOURCES.txt
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)        1 2023-06-20 12:48:53.000000 voila-vuetify-tuwien-0.6.2/voila_vuetify_tuwien.egg-info/dependency_links.txt
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)       20 2023-06-20 12:48:53.000000 voila-vuetify-tuwien-0.6.2/voila_vuetify_tuwien.egg-info/requires.txt
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)        6 2023-06-20 12:48:53.000000 voila-vuetify-tuwien-0.6.2/voila_vuetify_tuwien.egg-info/top_level.txt
```

### Comparing `voila-vuetify-tuwien-0.6.1/LICENSE` & `voila-vuetify-tuwien-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `voila-vuetify-tuwien-0.6.1/README.md` & `voila-vuetify-tuwien-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `voila-vuetify-tuwien-0.6.1/setup.py` & `voila-vuetify-tuwien-0.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 for (dirpath, dirnames, filenames) in os.walk('share/jupyter/'):
     if filenames:
         data_files.append((dirpath, [os.path.join(dirpath, filename) for filename in filenames]))
 
 
 setup(
     name='voila-vuetify-tuwien',
-    version="0.6.1",
+    version="0.6.2",
     description="TU Wien vuetify template for Voila",
     data_files=data_files,
     install_requires=['voila>=0.2.1,<0.6.0'],
     include_package_data=True,
     author=['Voila Development Team', "Marijana Petojevic"],
     url='https://gitlab.tuwien.ac.at/hpc/datalab/jupyter/voila/voila-vuetify-tu-wien-template',
     keywords=[
```

### Comparing `voila-vuetify-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-tuwien/ansi.js` & `voila-vuetify-tuwien-0.6.2/share/jupyter/nbconvert/templates/vuetify-base-tuwien/ansi.js`

 * *Files identical despite different names*

### Comparing `voila-vuetify-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-tuwien/app.html` & `voila-vuetify-tuwien-0.6.2/share/jupyter/nbconvert/templates/vuetify-base-tuwien/app.html`

 * *Files identical despite different names*

### Comparing `voila-vuetify-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-tuwien/index.html.j2` & `voila-vuetify-tuwien-0.6.2/share/jupyter/nbconvert/templates/vuetify-base-tuwien/index.html.j2`

 * *Files identical despite different names*

### Comparing `voila-vuetify-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-tuwien/util.js` & `voila-vuetify-tuwien-0.6.2/share/jupyter/nbconvert/templates/vuetify-base-tuwien/util.js`

 * *Files identical despite different names*

### Comparing `voila-vuetify-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-default-tuwien/app.html` & `voila-vuetify-tuwien-0.6.2/share/jupyter/nbconvert/templates/vuetify-default-tuwien/app.html`

 * *Files identical despite different names*

### Comparing `voila-vuetify-tuwien-0.6.1/share/jupyter/voila/templates/vuetify-base-tuwien/index.html.j2` & `voila-vuetify-tuwien-0.6.2/share/jupyter/voila/templates/vuetify-base-tuwien/index.html.j2`

 * *Files identical despite different names*

### Comparing `voila-vuetify-tuwien-0.6.1/voila_vuetify_tuwien.egg-info/SOURCES.txt` & `voila-vuetify-tuwien-0.6.2/voila_vuetify_tuwien.egg-info/SOURCES.txt`

 * *Files identical despite different names*

