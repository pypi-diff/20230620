# Comparing `tmp/tistory-helper-0.0.2.tar.gz` & `tmp/tistory-helper-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tistory-helper-0.0.2.tar", last modified: Tue Jun 20 05:55:56 2023, max compression
+gzip compressed data, was "tistory-helper-0.0.3.tar", last modified: Tue Jun 20 06:21:51 2023, max compression
```

## Comparing `tistory-helper-0.0.2.tar` & `tistory-helper-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 user1     (1000) users      (984)        0 2023-06-20 05:55:56.984760 tistory-helper-0.0.2/
--rw-r--r--   0 user1     (1000) users      (984)      714 2023-06-20 05:55:56.984760 tistory-helper-0.0.2/PKG-INFO
--rw-r--r--   0 user1     (1000) users      (984)     5207 2023-06-19 06:40:27.000000 tistory-helper-0.0.2/README.md
--rw-r--r--   0 user1     (1000) users      (984)       79 2023-06-20 05:55:56.984760 tistory-helper-0.0.2/setup.cfg
--rw-r--r--   0 user1     (1000) users      (984)     1362 2023-06-20 05:53:25.000000 tistory-helper-0.0.2/setup.py
-drwxr-xr-x   0 user1     (1000) users      (984)        0 2023-06-20 05:55:56.984760 tistory-helper-0.0.2/src/
--rw-r--r--   0 user1     (1000) users      (984)        0 2023-06-20 05:16:25.000000 tistory-helper-0.0.2/src/__init__.py
--rw-r--r--   0 user1     (1000) users      (984)     4181 2023-06-19 16:07:08.000000 tistory-helper-0.0.2/src/auth.py
--rw-r--r--   0 user1     (1000) users      (984)     1477 2023-06-19 16:10:34.000000 tistory-helper-0.0.2/src/category.py
--rw-r--r--   0 user1     (1000) users      (984)      633 2023-06-19 16:11:03.000000 tistory-helper-0.0.2/src/env.py
--rw-r--r--   0 user1     (1000) users      (984)     2531 2023-06-19 16:07:27.000000 tistory-helper-0.0.2/src/image.py
--rw-r--r--   0 user1     (1000) users      (984)     6252 2023-06-19 16:21:55.000000 tistory-helper-0.0.2/src/markdown.py
--rw-r--r--   0 user1     (1000) users      (984)     1158 2023-06-20 05:51:43.000000 tistory-helper-0.0.2/src/tistory.py
-drwxr-xr-x   0 user1     (1000) users      (984)        0 2023-06-20 05:55:56.984760 tistory-helper-0.0.2/tistory_helper.egg-info/
--rw-r--r--   0 user1     (1000) users      (984)      714 2023-06-20 05:55:56.000000 tistory-helper-0.0.2/tistory_helper.egg-info/PKG-INFO
--rw-r--r--   0 user1     (1000) users      (984)      357 2023-06-20 05:55:56.000000 tistory-helper-0.0.2/tistory_helper.egg-info/SOURCES.txt
--rw-r--r--   0 user1     (1000) users      (984)        1 2023-06-20 05:55:56.000000 tistory-helper-0.0.2/tistory_helper.egg-info/dependency_links.txt
--rw-r--r--   0 user1     (1000) users      (984)       44 2023-06-20 05:55:56.000000 tistory-helper-0.0.2/tistory_helper.egg-info/entry_points.txt
--rw-r--r--   0 user1     (1000) users      (984)       87 2023-06-20 05:55:56.000000 tistory-helper-0.0.2/tistory_helper.egg-info/requires.txt
--rw-r--r--   0 user1     (1000) users      (984)        4 2023-06-20 05:55:56.000000 tistory-helper-0.0.2/tistory_helper.egg-info/top_level.txt
+drwxr-xr-x   0 user1     (1000) users      (984)        0 2023-06-20 06:21:51.536113 tistory-helper-0.0.3/
+-rw-r--r--   0 user1     (1000) users      (984)     5962 2023-06-20 06:21:51.536113 tistory-helper-0.0.3/PKG-INFO
+-rw-r--r--   0 user1     (1000) users      (984)     5207 2023-06-19 06:40:27.000000 tistory-helper-0.0.3/README.md
+-rw-r--r--   0 user1     (1000) users      (984)       79 2023-06-20 06:21:51.536113 tistory-helper-0.0.3/setup.cfg
+-rw-r--r--   0 user1     (1000) users      (984)     1326 2023-06-20 06:21:40.000000 tistory-helper-0.0.3/setup.py
+drwxr-xr-x   0 user1     (1000) users      (984)        0 2023-06-20 06:21:51.536113 tistory-helper-0.0.3/src/
+-rw-r--r--   0 user1     (1000) users      (984)        0 2023-06-20 05:16:25.000000 tistory-helper-0.0.3/src/__init__.py
+-rw-r--r--   0 user1     (1000) users      (984)     4181 2023-06-19 16:07:08.000000 tistory-helper-0.0.3/src/auth.py
+-rw-r--r--   0 user1     (1000) users      (984)     1477 2023-06-19 16:10:34.000000 tistory-helper-0.0.3/src/category.py
+-rw-r--r--   0 user1     (1000) users      (984)      633 2023-06-19 16:11:03.000000 tistory-helper-0.0.3/src/env.py
+-rw-r--r--   0 user1     (1000) users      (984)     2531 2023-06-19 16:07:27.000000 tistory-helper-0.0.3/src/image.py
+-rw-r--r--   0 user1     (1000) users      (984)     6252 2023-06-19 16:21:55.000000 tistory-helper-0.0.3/src/markdown.py
+-rw-r--r--   0 user1     (1000) users      (984)     1158 2023-06-20 05:51:43.000000 tistory-helper-0.0.3/src/tistory.py
+drwxr-xr-x   0 user1     (1000) users      (984)        0 2023-06-20 06:21:51.536113 tistory-helper-0.0.3/tistory_helper.egg-info/
+-rw-r--r--   0 user1     (1000) users      (984)     5962 2023-06-20 06:21:51.000000 tistory-helper-0.0.3/tistory_helper.egg-info/PKG-INFO
+-rw-r--r--   0 user1     (1000) users      (984)      357 2023-06-20 06:21:51.000000 tistory-helper-0.0.3/tistory_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 user1     (1000) users      (984)        1 2023-06-20 06:21:51.000000 tistory-helper-0.0.3/tistory_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 user1     (1000) users      (984)       44 2023-06-20 06:21:51.000000 tistory-helper-0.0.3/tistory_helper.egg-info/entry_points.txt
+-rw-r--r--   0 user1     (1000) users      (984)       87 2023-06-20 06:21:51.000000 tistory-helper-0.0.3/tistory_helper.egg-info/requires.txt
+-rw-r--r--   0 user1     (1000) users      (984)        4 2023-06-20 06:21:51.000000 tistory-helper-0.0.3/tistory_helper.egg-info/top_level.txt
```

### Comparing `tistory-helper-0.0.2/README.md` & `tistory-helper-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `tistory-helper-0.0.2/setup.py` & `tistory-helper-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,37 @@
-# import os
+import os
 from setuptools import setup, find_packages
 
 
-# with open(os.path.join(os.path.dirname(__file__), "README.md")) as fh:
-#     long_description = fh.read()
+with open(os.path.join(os.path.dirname(__file__), "README.md")) as fh:
+    long_description = fh.read()
 
 
 requirements = [
     "Markdown",
     "python-dotenv",
     "Requests",
     "mdx_truly_sane_lists",
     "markdown_link_attr_modifier",
     "click",
 ]
 
 setup(
     name="tistory-helper",
-    version="0.0.2",
+    version="0.0.3",
     author="Kangjae Choi",
     author_email="choikj33@gmail.com",
     description="Tistory Helper to upload markdown and images",
     license="MIT",
     keywords="tistory terminal markdown image",
     url="https://github.com/choikangjae/local-first-tistory",
-    packages=[
-        "src",
-    ],
-    # TODO
-    # long_description=long_description,
-    # long_description_content_type="text/markdown",
-    # include_package_data=True,
-    #
+    packages=find_packages(),
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    include_package_data=True,
     install_requires=requirements,
     entry_points={"console_scripts": ["tistory=src.tistory:cli"]},
     classifiers=[
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
```

### Comparing `tistory-helper-0.0.2/src/auth.py` & `tistory-helper-0.0.3/src/auth.py`

 * *Files identical despite different names*

### Comparing `tistory-helper-0.0.2/src/category.py` & `tistory-helper-0.0.3/src/category.py`

 * *Files identical despite different names*

### Comparing `tistory-helper-0.0.2/src/env.py` & `tistory-helper-0.0.3/src/env.py`

 * *Files identical despite different names*

### Comparing `tistory-helper-0.0.2/src/image.py` & `tistory-helper-0.0.3/src/image.py`

 * *Files identical despite different names*

### Comparing `tistory-helper-0.0.2/src/markdown.py` & `tistory-helper-0.0.3/src/markdown.py`

 * *Files identical despite different names*

### Comparing `tistory-helper-0.0.2/src/tistory.py` & `tistory-helper-0.0.3/src/tistory.py`

 * *Files identical despite different names*

