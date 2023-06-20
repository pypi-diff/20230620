# Comparing `tmp/pillar1-0.1.5.3.tar.gz` & `tmp/pillar1-0.1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pillar1-0.1.5.3.tar", last modified: Tue Jun 20 00:23:05 2023, max compression
+gzip compressed data, was "pillar1-0.1.5.4.tar", last modified: Tue Jun 20 00:28:36 2023, max compression
```

## Comparing `pillar1-0.1.5.3.tar` & `pillar1-0.1.5.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 00:23:05.051145 pillar1-0.1.5.3/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-20 00:23:05.051026 pillar1-0.1.5.3/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.5.3/README.md
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 00:23:05.050345 pillar1-0.1.5.3/pillar1/
--rw-r--r--   0 aymanhajja   (501) staff       (20)       27 2023-06-19 22:42:24.000000 pillar1-0.1.5.3/pillar1/__init__.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2500 2023-06-20 00:22:57.000000 pillar1-0.1.5.3/pillar1/pillar1.py
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 00:23:05.050857 pillar1-0.1.5.3/pillar1.egg-info/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-20 00:23:05.000000 pillar1-0.1.5.3/pillar1.egg-info/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)      181 2023-06-20 00:23:05.000000 pillar1-0.1.5.3/pillar1.egg-info/SOURCES.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-20 00:23:05.000000 pillar1-0.1.5.3/pillar1.egg-info/dependency_links.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-20 00:23:05.000000 pillar1-0.1.5.3/pillar1.egg-info/top_level.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-20 00:23:05.051189 pillar1-0.1.5.3/setup.cfg
--rw-r--r--   0 aymanhajja   (501) staff       (20)      621 2023-06-20 00:23:02.000000 pillar1-0.1.5.3/setup.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 00:28:36.109165 pillar1-0.1.5.4/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-20 00:28:36.109041 pillar1-0.1.5.4/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.5.4/README.md
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 00:28:36.108246 pillar1-0.1.5.4/pillar1/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       27 2023-06-19 22:42:24.000000 pillar1-0.1.5.4/pillar1/__init__.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2547 2023-06-20 00:28:18.000000 pillar1-0.1.5.4/pillar1/pillar1.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 00:28:36.108851 pillar1-0.1.5.4/pillar1.egg-info/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-20 00:28:36.000000 pillar1-0.1.5.4/pillar1.egg-info/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      181 2023-06-20 00:28:36.000000 pillar1-0.1.5.4/pillar1.egg-info/SOURCES.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-20 00:28:36.000000 pillar1-0.1.5.4/pillar1.egg-info/dependency_links.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-20 00:28:36.000000 pillar1-0.1.5.4/pillar1.egg-info/top_level.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-20 00:28:36.109203 pillar1-0.1.5.4/setup.cfg
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      621 2023-06-20 00:28:27.000000 pillar1-0.1.5.4/setup.py
```

### Comparing `pillar1-0.1.5.3/PKG-INFO` & `pillar1-0.1.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.5.3
+Version: 0.1.5.4
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.5.3/README.md` & `pillar1-0.1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.5.3/pillar1/pillar1.py` & `pillar1-0.1.5.4/pillar1/pillar1.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,21 +48,22 @@
 
             self.response = json.loads(response['Body'].read())[0]['generated_text']
 
         if prompt:
             self.prompt = prompt
             submit_request(self.prompt)
         else:
-            textarea_bg = widgets.Textarea(description='What SQL are you looking for:', layout=widgets.Layout(width='80%', height='200px'), style={'description_width': 'initial'})
+            textarea_bg = widgets.Textarea(description='Provide any necessary background:', layout=widgets.Layout(width='80%', height='200px'),
+                                           style={'description_width': 'initial'})
             input_text = widgets.Text(description='What SQL are you looking for:', layout=widgets.Layout(width='80%'), style={'description_width': 'initial'})
             button = widgets.Button(description='Submit')
             display(textarea_bg)
             display(input_text)
             display(button)
 
             # Define button click event
-            def submit_button():
+            def submit_button(b):
                 prompt = f"Given this background \"{textarea_bg.value}\", answer this question \"{input_text.value}\""
                 submit_request(prompt)
 
             # Bind button click event to function
-            button.on_click(submit_request)
+            button.on_click(submit_button)
```

### Comparing `pillar1-0.1.5.3/pillar1.egg-info/PKG-INFO` & `pillar1-0.1.5.4/pillar1.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.5.3
+Version: 0.1.5.4
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.5.3/setup.py` & `pillar1-0.1.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pillar1',
-    version='0.1.5.3',
+    version='0.1.5.4',
     packages=find_packages(),
     description='Official package for Pillar1 company',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayman Hajja',
     author_email='amhajja@gmail.com',
     url='https://github.com/amhajja/pillar1',
```

