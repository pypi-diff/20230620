# Comparing `tmp/easylsb-1.0.8.tar.gz` & `tmp/easylsb-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\easylsb-1.0.8.tar", last modified: Fri Jun  9 06:49:06 2023, max compression
+gzip compressed data, was "dist\easylsb-1.0.9.tar", last modified: Tue Jun 20 09:00:17 2023, max compression
```

## Comparing `easylsb-1.0.8.tar` & `easylsb-1.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 06:49:06.000000 easylsb-1.0.8/
--rw-rw-rw-   0        0        0     1745 2023-06-09 06:49:06.000000 easylsb-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1598 2023-06-06 07:05:31.000000 easylsb-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 06:49:06.000000 easylsb-1.0.8/easylsb.egg-info/
--rw-rw-rw-   0        0        0     1745 2023-06-09 06:49:06.000000 easylsb-1.0.8/easylsb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2023-06-09 06:49:06.000000 easylsb-1.0.8/easylsb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 06:49:06.000000 easylsb-1.0.8/easylsb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-06-09 06:49:06.000000 easylsb-1.0.8/easylsb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       34 2023-06-09 06:49:06.000000 easylsb-1.0.8/easylsb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-09 06:49:06.000000 easylsb-1.0.8/easylsb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    16093 2023-06-09 06:48:03.000000 easylsb-1.0.8/lsb.py
--rw-rw-rw-   0        0        0       42 2023-06-09 06:49:06.000000 easylsb-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      727 2023-06-09 06:48:53.000000 easylsb-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 09:00:17.000000 easylsb-1.0.9/
+-rw-rw-rw-   0        0        0     1955 2023-06-20 09:00:17.000000 easylsb-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1806 2023-06-20 08:56:59.000000 easylsb-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 09:00:17.000000 easylsb-1.0.9/easylsb.egg-info/
+-rw-rw-rw-   0        0        0     1955 2023-06-20 09:00:17.000000 easylsb-1.0.9/easylsb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2023-06-20 09:00:17.000000 easylsb-1.0.9/easylsb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 09:00:17.000000 easylsb-1.0.9/easylsb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-06-20 09:00:17.000000 easylsb-1.0.9/easylsb.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2023-06-20 09:00:17.000000 easylsb-1.0.9/easylsb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-20 09:00:17.000000 easylsb-1.0.9/easylsb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    16093 2023-06-09 06:48:03.000000 easylsb-1.0.9/lsb.py
+-rw-rw-rw-   0        0        0       42 2023-06-20 09:00:17.000000 easylsb-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      727 2023-06-20 09:00:10.000000 easylsb-1.0.9/setup.py
```

### Comparing `easylsb-1.0.8/PKG-INFO` & `easylsb-1.0.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-Metadata-Version: 2.1
-Name: easylsb
-Version: 1.0.8
-Summary: Simple Python package for steganography
-Description-Content-Type: text/markdown
-
 <p><span><span style="font-family:Verdana, Arial, Helvetica, sans-serif;line-height:19px;text-indent:26px;"><span style="font-size:14px;"><span style="font-family:Arial;line-height:26px;"><br></span></span></span></span></p>
 
 ### This is a simple Python package for steganography
 
 Now this package can automatically detect the encoding of the hidden text using the '-a' argument.
 Code to hide information in the given image:
 ```python
@@ -49,8 +43,11 @@
 hidden=lsb.lsbenc(img,info,rsakey=pub)
 img_hidden=Image.fromarray(hidden)
 img_hidden.save('hidden.png')# Must be a PNG,BMP,etc., not JPEG or WEBP
 # Recover
 info=lsb.lsbdec(hidden,rsakey=priv)
 print(info)# b'Some information'
 ```
+
 It's very easy to use the StegSolve tool to get the hidden information, but easylsb package allows you to encrypt the information using DES or RSA.
+
+<font color="red">WARNING: Python 2 is unsupported by easylsb since easylsb 1.0.7, if you're using Python 2 and want to install this package, you should use the command "pip install easylsb==1.0.6"</font>
```

### Comparing `easylsb-1.0.8/README.md` & `easylsb-1.0.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+Metadata-Version: 2.1
+Name: easylsb
+Version: 1.0.9
+Summary: Simple Python package for steganography
+Description-Content-Type: text/markdown
+
 <p><span><span style="font-family:Verdana, Arial, Helvetica, sans-serif;line-height:19px;text-indent:26px;"><span style="font-size:14px;"><span style="font-family:Arial;line-height:26px;"><br></span></span></span></span></p>
 
 ### This is a simple Python package for steganography
 
 Now this package can automatically detect the encoding of the hidden text using the '-a' argument.
 Code to hide information in the given image:
 ```python
@@ -43,8 +49,11 @@
 hidden=lsb.lsbenc(img,info,rsakey=pub)
 img_hidden=Image.fromarray(hidden)
 img_hidden.save('hidden.png')# Must be a PNG,BMP,etc., not JPEG or WEBP
 # Recover
 info=lsb.lsbdec(hidden,rsakey=priv)
 print(info)# b'Some information'
 ```
+
 It's very easy to use the StegSolve tool to get the hidden information, but easylsb package allows you to encrypt the information using DES or RSA.
+
+<font color="red">WARNING: Python 2 is unsupported by easylsb since easylsb 1.0.7, if you're using Python 2 and want to install this package, you should use the command "pip install easylsb==1.0.6"</font>
```

### Comparing `easylsb-1.0.8/easylsb.egg-info/PKG-INFO` & `easylsb-1.0.9/easylsb.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easylsb
-Version: 1.0.8
+Version: 1.0.9
 Summary: Simple Python package for steganography
 Description-Content-Type: text/markdown
 
 <p><span><span style="font-family:Verdana, Arial, Helvetica, sans-serif;line-height:19px;text-indent:26px;"><span style="font-size:14px;"><span style="font-family:Arial;line-height:26px;"><br></span></span></span></span></p>
 
 ### This is a simple Python package for steganography
 
@@ -49,8 +49,11 @@
 hidden=lsb.lsbenc(img,info,rsakey=pub)
 img_hidden=Image.fromarray(hidden)
 img_hidden.save('hidden.png')# Must be a PNG,BMP,etc., not JPEG or WEBP
 # Recover
 info=lsb.lsbdec(hidden,rsakey=priv)
 print(info)# b'Some information'
 ```
+
 It's very easy to use the StegSolve tool to get the hidden information, but easylsb package allows you to encrypt the information using DES or RSA.
+
+<font color="red">WARNING: Python 2 is unsupported by easylsb since easylsb 1.0.7, if you're using Python 2 and want to install this package, you should use the command "pip install easylsb==1.0.6"</font>
```

### Comparing `easylsb-1.0.8/lsb.py` & `easylsb-1.0.9/lsb.py`

 * *Files identical despite different names*

### Comparing `easylsb-1.0.8/setup.py` & `easylsb-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     req.append('pillow')
 def readme():
     with open('README.md','r') as file:
         return file.read()
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 setup(
     name="easylsb",
-    version="1.0.8",
+    version="1.0.9",
     description="Simple Python package for steganography",
     long_description=readme(),
     long_description_content_type='text/markdown',
     py_modules=["lsb"],
     install_requires=req,
     entry_points={
         "console_scripts": [
```

