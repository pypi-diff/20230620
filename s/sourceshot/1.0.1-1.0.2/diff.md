# Comparing `tmp/sourceshot-1.0.1.tar.gz` & `tmp/sourceshot-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sourceshot-1.0.1.tar", last modified: Tue Jun 20 12:02:52 2023, max compression
+gzip compressed data, was "dist\sourceshot-1.0.2.tar", last modified: Tue Jun 20 13:13:15 2023, max compression
```

## Comparing `sourceshot-1.0.1.tar` & `sourceshot-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 12:02:52.000000 sourceshot-1.0.1/
--rw-rw-rw-   0        0        0     1662 2023-06-20 12:02:52.000000 sourceshot-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1478 2023-06-20 11:59:07.000000 sourceshot-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-20 12:02:52.000000 sourceshot-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      564 2023-06-20 12:02:49.000000 sourceshot-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 12:02:52.000000 sourceshot-1.0.1/sourceshot.egg-info/
--rw-rw-rw-   0        0        0     1662 2023-06-20 12:02:52.000000 sourceshot-1.0.1/sourceshot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      345 2023-06-20 12:02:52.000000 sourceshot-1.0.1/sourceshot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 12:02:52.000000 sourceshot-1.0.1/sourceshot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-06-20 12:02:52.000000 sourceshot-1.0.1/sourceshot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       48 2023-06-20 12:02:52.000000 sourceshot-1.0.1/sourceshot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-20 12:02:52.000000 sourceshot-1.0.1/sourceshot.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-20 12:02:52.000000 sourceshot-1.0.1/sshot/
--rw-rw-rw-   0        0        0     7018 2023-06-20 07:59:00.000000 sourceshot-1.0.1/sshot/__init__.py
--rw-rw-rw-   0        0        0     2894 2023-06-20 12:02:17.000000 sourceshot-1.0.1/sshot/background.py
--rw-rw-rw-   0        0        0     2847 2023-06-19 11:17:45.000000 sourceshot-1.0.1/sshot/config.py
--rw-rw-rw-   0        0        0      275 2023-06-19 10:25:15.000000 sourceshot-1.0.1/sshot/debug.py
--rw-rw-rw-   0        0        0      621 2023-06-19 08:45:30.000000 sourceshot-1.0.1/sshot/easy.py
--rw-rw-rw-   0        0        0     2695 2023-06-20 07:13:11.000000 sourceshot-1.0.1/sshot/imageproc.py
--rw-rw-rw-   0        0        0      453 2023-06-20 07:13:15.000000 sourceshot-1.0.1/sshot/tokenproc.py
+drwxrwxrwx   0        0        0        0 2023-06-20 13:13:15.000000 sourceshot-1.0.2/
+-rw-rw-rw-   0        0        0     1499 2023-06-20 13:13:15.000000 sourceshot-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1315 2023-06-20 13:12:22.000000 sourceshot-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-20 13:13:15.000000 sourceshot-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      564 2023-06-20 13:13:03.000000 sourceshot-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 13:13:15.000000 sourceshot-1.0.2/sourceshot.egg-info/
+-rw-rw-rw-   0        0        0     1499 2023-06-20 13:13:15.000000 sourceshot-1.0.2/sourceshot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      345 2023-06-20 13:13:15.000000 sourceshot-1.0.2/sourceshot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 13:13:15.000000 sourceshot-1.0.2/sourceshot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-06-20 13:13:15.000000 sourceshot-1.0.2/sourceshot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       48 2023-06-20 13:13:15.000000 sourceshot-1.0.2/sourceshot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-20 13:13:15.000000 sourceshot-1.0.2/sourceshot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 13:13:15.000000 sourceshot-1.0.2/sshot/
+-rw-rw-rw-   0        0        0     7018 2023-06-20 07:59:00.000000 sourceshot-1.0.2/sshot/__init__.py
+-rw-rw-rw-   0        0        0     2894 2023-06-20 12:02:17.000000 sourceshot-1.0.2/sshot/background.py
+-rw-rw-rw-   0        0        0     2847 2023-06-19 11:17:45.000000 sourceshot-1.0.2/sshot/config.py
+-rw-rw-rw-   0        0        0      275 2023-06-19 10:25:15.000000 sourceshot-1.0.2/sshot/debug.py
+-rw-rw-rw-   0        0        0     1223 2023-06-20 13:12:54.000000 sourceshot-1.0.2/sshot/easy.py
+-rw-rw-rw-   0        0        0     2695 2023-06-20 07:13:11.000000 sourceshot-1.0.2/sshot/imageproc.py
+-rw-rw-rw-   0        0        0      453 2023-06-20 07:13:15.000000 sourceshot-1.0.2/sshot/tokenproc.py
```

### Comparing `sourceshot-1.0.1/PKG-INFO` & `sourceshot-1.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sourceshot
-Version: 1.0.1
+Version: 1.0.2
 Summary: Takes pictures of code!
 Keywords: code,picture
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 <p><span><span style="font-family:Verdana, Arial, Helvetica, sans-serif;line-height:19px;text-indent:26px;"><span style="font-size:14px;"><span style="font-family:Arial;line-height:26px;"><br></span></span></span></span></p>
 
@@ -39,11 +39,8 @@
 code='''
 print('Hello World!')
 '''
 bg=np.array(Image.open('bg.png'))
 image=shot(code,lang='python',background=Background(bg))
 Image.fromarray(image).save('code.png')
 ```
-### About optimization
-This version is optimized, much faster now.
-
-Sourceshot 1.0.0 takes 0.161 seconds when creating an image of a Python source code with 3 lines, while this version only takes 0.042 seconds. 
+Added SVG support, but other packages are required.
```

### Comparing `sourceshot-1.0.1/README.md` & `sourceshot-1.0.2/sourceshot.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1
+Name: sourceshot
+Version: 1.0.2
+Summary: Takes pictures of code!
+Keywords: code,picture
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 <p><span><span style="font-family:Verdana, Arial, Helvetica, sans-serif;line-height:19px;text-indent:26px;"><span style="font-size:14px;"><span style="font-family:Arial;line-height:26px;"><br></span></span></span></span></p>
 
 ### This package takes pictures of source code
 Example code: 
 ```python
 from sshot import shot
 from PIL import Image
@@ -31,11 +39,8 @@
 code='''
 print('Hello World!')
 '''
 bg=np.array(Image.open('bg.png'))
 image=shot(code,lang='python',background=Background(bg))
 Image.fromarray(image).save('code.png')
 ```
-### About optimization
-This version is optimized, much faster now.
-
-Sourceshot 1.0.0 takes 0.161 seconds when creating an image of a Python source code with 3 lines, while this version only takes 0.042 seconds. 
+Added SVG support, but other packages are required.
```

### Comparing `sourceshot-1.0.1/setup.py` & `sourceshot-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 def readme():
     with open('README.md','r') as f:
         return f.read()
 setup(
     name='sourceshot',
-    version='1.0.1',
+    version='1.0.2',
     description='Takes pictures of code!',
     long_description=readme(),
     packages=['sshot'],
     long_description_content_type='text/markdown',
     entry_points={
         'console_scripts':[
             'sshot=sshot:_cli'
```

### Comparing `sourceshot-1.0.1/sshot/__init__.py` & `sourceshot-1.0.2/sshot/__init__.py`

 * *Files identical despite different names*

### Comparing `sourceshot-1.0.1/sshot/background.py` & `sourceshot-1.0.2/sshot/background.py`

 * *Files identical despite different names*

### Comparing `sourceshot-1.0.1/sshot/config.py` & `sourceshot-1.0.2/sshot/config.py`

 * *Files identical despite different names*

### Comparing `sourceshot-1.0.1/sshot/imageproc.py` & `sourceshot-1.0.2/sshot/imageproc.py`

 * *Files identical despite different names*

