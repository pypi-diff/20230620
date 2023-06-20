# Comparing `tmp/pyttm-0.0.2.tar.gz` & `tmp/pyttm-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyttm-0.0.2.tar", last modified: Tue Jun 20 11:06:49 2023, max compression
+gzip compressed data, was "pyttm-0.0.3.tar", last modified: Tue Jun 20 11:50:33 2023, max compression
```

## Comparing `pyttm-0.0.2.tar` & `pyttm-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 11:06:49.089370 pyttm-0.0.2/
--rw-rw-rw-   0        0        0     1063 2023-06-20 07:08:08.000000 pyttm-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     2686 2023-06-20 11:06:49.089370 pyttm-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1909 2023-06-20 11:06:33.000000 pyttm-0.0.2/README.md
--rw-rw-rw-   0        0        0       68 2023-06-20 11:06:49.091370 pyttm-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1301 2023-06-20 11:04:32.000000 pyttm-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 11:06:49.066371 pyttm-0.0.2/ttm/
-drwxrwxrwx   0        0        0        0 2023-06-20 11:06:49.088369 pyttm-0.0.2/ttm/pyttm.egg-info/
--rw-rw-rw-   0        0        0     2686 2023-06-20 11:06:49.000000 pyttm-0.0.2/ttm/pyttm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-06-20 11:06:49.000000 pyttm-0.0.2/ttm/pyttm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 11:06:49.000000 pyttm-0.0.2/ttm/pyttm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-06-20 11:06:49.000000 pyttm-0.0.2/ttm/pyttm.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       13 2023-06-20 11:06:49.000000 pyttm-0.0.2/ttm/pyttm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 11:06:49.000000 pyttm-0.0.2/ttm/pyttm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 11:50:33.784096 pyttm-0.0.3/
+-rw-rw-rw-   0        0        0     1063 2023-06-20 07:08:08.000000 pyttm-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2686 2023-06-20 11:50:33.784096 pyttm-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1909 2023-06-20 11:06:33.000000 pyttm-0.0.3/README.md
+-rw-rw-rw-   0        0        0       68 2023-06-20 11:50:33.789095 pyttm-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1337 2023-06-20 11:49:22.000000 pyttm-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 11:50:33.757095 pyttm-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-20 11:50:33.764095 pyttm-0.0.3/src/pyttm/
+-rw-rw-rw-   0        0        0       40 2023-06-20 11:49:22.000000 pyttm-0.0.3/src/pyttm/__init__.py
+-rw-rw-rw-   0        0        0      956 2023-06-20 11:33:04.000000 pyttm-0.0.3/src/pyttm/app.py
+drwxrwxrwx   0        0        0        0 2023-06-20 11:50:33.783095 pyttm-0.0.3/src/pyttm/libs/
+-rw-rw-rw-   0        0        0     1092 2023-06-20 08:30:45.000000 pyttm-0.0.3/src/pyttm/libs/crypto.py
+-rw-rw-rw-   0        0        0     1689 2023-06-20 11:33:05.000000 pyttm-0.0.3/src/pyttm/libs/db.py
+-rw-rw-rw-   0        0        0     5095 2023-06-20 11:49:22.000000 pyttm-0.0.3/src/pyttm/libs/helper.py
+-rw-rw-rw-   0        0        0     2960 2023-06-20 06:15:35.000000 pyttm-0.0.3/src/pyttm/libs/totp.py
+drwxrwxrwx   0        0        0        0 2023-06-20 11:50:33.778095 pyttm-0.0.3/src/pyttm.egg-info/
+-rw-rw-rw-   0        0        0     2686 2023-06-20 11:50:33.000000 pyttm-0.0.3/src/pyttm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      369 2023-06-20 11:50:33.000000 pyttm-0.0.3/src/pyttm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 11:50:33.000000 pyttm-0.0.3/src/pyttm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-06-20 11:50:33.000000 pyttm-0.0.3/src/pyttm.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       13 2023-06-20 11:50:33.000000 pyttm-0.0.3/src/pyttm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-20 11:50:33.000000 pyttm-0.0.3/src/pyttm.egg-info/top_level.txt
```

### Comparing `pyttm-0.0.2/LICENSE` & `pyttm-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyttm-0.0.2/PKG-INFO` & `pyttm-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyttm
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple Terminal based TOTP manager
 Home-page: https://github.com/The-Robin-Hood/ttm
 Author: The Robin Hood
 License: MIT
 Keywords: totp,otp,encryption,decryption,AES256,crypto,security,privacy
 Platform: any
 Classifier: Intended Audience :: Developers
```

### Comparing `pyttm-0.0.2/README.md` & `pyttm-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyttm-0.0.2/setup.py` & `pyttm-0.0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 
 def docs_read(fname):
     f = open(os.path.join(os.path.dirname(__file__), fname)).read()
     return f.replace('â™¥', '♥')
 
 setup(
     name='pyttm',
-    version='0.0.2',
+    version='0.0.3',
     description='A simple Terminal based TOTP manager',
     long_description=(docs_read('README.md')),
     long_description_content_type='text/markdown',
     url='https://github.com/The-Robin-Hood/ttm',
     author='The Robin Hood',
     license='MIT',
     platforms=['any'],
     entry_points={
         'console_scripts': [
-            'ttm = ttm.app:main'
+            'ttm = pyttm.app:main'
         ],
     },
-    packages=find_packages('ttm'),
-    package_dir={'': 'ttm'},
+    packages=find_packages(where='src',include=['pyttm','pyttm.*']),
+    package_dir={'': 'src'},
     include_package_data=True,
     install_requires=['pycryptodome'],
     keywords='totp,otp,encryption,decryption,AES256,crypto,security,privacy',
         classifiers=[
         'Intended Audience :: Developers',
         'Topic :: Security',
         'Topic :: Utilities',
```

### Comparing `pyttm-0.0.2/ttm/pyttm.egg-info/PKG-INFO` & `pyttm-0.0.3/src/pyttm.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyttm
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple Terminal based TOTP manager
 Home-page: https://github.com/The-Robin-Hood/ttm
 Author: The Robin Hood
 License: MIT
 Keywords: totp,otp,encryption,decryption,AES256,crypto,security,privacy
 Platform: any
 Classifier: Intended Audience :: Developers
```

