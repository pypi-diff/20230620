# Comparing `tmp/pillar1-0.1.5.1.tar.gz` & `tmp/pillar1-0.1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pillar1-0.1.5.1.tar", last modified: Tue Jun 20 00:13:30 2023, max compression
+gzip compressed data, was "pillar1-0.1.5.2.tar", last modified: Tue Jun 20 00:20:21 2023, max compression
```

## Comparing `pillar1-0.1.5.1.tar` & `pillar1-0.1.5.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 00:13:30.974593 pillar1-0.1.5.1/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-20 00:13:30.974469 pillar1-0.1.5.1/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.5.1/README.md
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 00:13:30.973552 pillar1-0.1.5.1/pillar1/
--rw-r--r--   0 aymanhajja   (501) staff       (20)       27 2023-06-19 22:42:24.000000 pillar1-0.1.5.1/pillar1/__init__.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2446 2023-06-20 00:13:14.000000 pillar1-0.1.5.1/pillar1/pillar1.py
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 00:13:30.974254 pillar1-0.1.5.1/pillar1.egg-info/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-20 00:13:30.000000 pillar1-0.1.5.1/pillar1.egg-info/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)      181 2023-06-20 00:13:30.000000 pillar1-0.1.5.1/pillar1.egg-info/SOURCES.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-20 00:13:30.000000 pillar1-0.1.5.1/pillar1.egg-info/dependency_links.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-20 00:13:30.000000 pillar1-0.1.5.1/pillar1.egg-info/top_level.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-20 00:13:30.974644 pillar1-0.1.5.1/setup.cfg
--rw-r--r--   0 aymanhajja   (501) staff       (20)      621 2023-06-20 00:13:25.000000 pillar1-0.1.5.1/setup.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 00:20:21.215910 pillar1-0.1.5.2/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-20 00:20:21.215798 pillar1-0.1.5.2/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.5.2/README.md
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 00:20:21.215031 pillar1-0.1.5.2/pillar1/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       27 2023-06-19 22:42:24.000000 pillar1-0.1.5.2/pillar1/__init__.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2490 2023-06-20 00:19:43.000000 pillar1-0.1.5.2/pillar1/pillar1.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-20 00:20:21.215635 pillar1-0.1.5.2/pillar1.egg-info/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-20 00:20:21.000000 pillar1-0.1.5.2/pillar1.egg-info/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      181 2023-06-20 00:20:21.000000 pillar1-0.1.5.2/pillar1.egg-info/SOURCES.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-20 00:20:21.000000 pillar1-0.1.5.2/pillar1.egg-info/dependency_links.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-20 00:20:21.000000 pillar1-0.1.5.2/pillar1.egg-info/top_level.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-20 00:20:21.215948 pillar1-0.1.5.2/setup.cfg
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      621 2023-06-20 00:19:57.000000 pillar1-0.1.5.2/setup.py
```

### Comparing `pillar1-0.1.5.1/PKG-INFO` & `pillar1-0.1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.5.1
+Version: 0.1.5.2
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.5.1/README.md` & `pillar1-0.1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.5.1/pillar1/pillar1.py` & `pillar1-0.1.5.2/pillar1/pillar1.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,43 +22,47 @@
             'sagemaker-runtime',
             aws_access_key_id=user_name,
             aws_secret_access_key=password,
             region_name='us-west-2'
         )
 
     def query(self, prompt):
+        def submit_request(prompt):
+            payload = {
+                'inputs': prompt,
+                "parameters": {
+                    "do_sample": True,
+                    "top_p": 0.7,
+                    "temperature": 0.7,
+                    "top_k": 50,
+                    "max_new_tokens": self.max_new_tokens,
+                    "repetition_penalty": 1.03,
+                    "stop": ["<|endoftext|>"]
+                }
+            }
+
+            response = self.client.invoke_endpoint(
+                EndpointName=self.endpoint_name,
+                ContentType='application/json',
+                Body=json.dumps(payload)
+            )
+
+            self.response = json.loads(response['Body'].read())[0]['generated_text']
+
         if prompt:
             self.prompt = prompt
+            submit_request(self.prompt)
         else:
             textarea_bg = widgets.Textarea(description='What SQL are you looking for:', layout=widgets.Layout(width='80%', height='200px'), style={'description_width': 'initial'})
             input_text = widgets.Text(description='What SQL are you looking for:', layout=widgets.Layout(width='80%'), style={'description_width': 'initial'})
             button = widgets.Button(description='Submit')
             display(textarea_bg)
             display(input_text)
             display(button)
 
             # Define button click event
-            def submit_request():
-                prompt = f"Given this background \"{textarea_bg.value}\", anser this question \"{input_text.value}\""
-                payload = {
-                    'inputs': prompt,
-                    "parameters": {
-                        "do_sample": True,
-                        "top_p": 0.7,
-                        "temperature": 0.7,
-                        "top_k": 50,
-                        "max_new_tokens": self.max_new_tokens,
-                        "repetition_penalty": 1.03,
-                        "stop": ["<|endoftext|>"]
-                    }
-                }
-
-                response = self.client.invoke_endpoint(
-                    EndpointName=self.endpoint_name,
-                    ContentType='application/json',
-                    Body=json.dumps(payload)
-                )
-
-                self.response = json.loads(response['Body'].read())[0]['generated_text']
+            def submit_button():
+                prompt = f"Given this background \"{textarea_bg.value}\", answer this question \"{input_text.value}\""
+                submit_request(prompt)
 
             # Bind button click event to function
             button.on_click(submit_request)
```

### Comparing `pillar1-0.1.5.1/pillar1.egg-info/PKG-INFO` & `pillar1-0.1.5.2/pillar1.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.5.1
+Version: 0.1.5.2
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.5.1/setup.py` & `pillar1-0.1.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pillar1',
-    version='0.1.5.1',
+    version='0.1.5.2',
     packages=find_packages(),
     description='Official package for Pillar1 company',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayman Hajja',
     author_email='amhajja@gmail.com',
     url='https://github.com/amhajja/pillar1',
```

