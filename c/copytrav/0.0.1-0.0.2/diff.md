# Comparing `tmp/copytrav-0.0.1.tar.gz` & `tmp/copytrav-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copytrav-0.0.1.tar", last modified: Thu Jun 15 15:55:44 2023, max compression
+gzip compressed data, was "copytrav-0.0.2.tar", last modified: Tue Jun 20 21:44:43 2023, max compression
```

## Comparing `copytrav-0.0.1.tar` & `copytrav-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 nosource  (1001) nosource  (1001)        0 2023-06-15 15:55:44.935960 copytrav-0.0.1/
--rw-r--r--   0 nosource  (1001) nosource  (1001)     1070 2023-06-14 20:50:43.000000 copytrav-0.0.1/LICENSE
--rw-r--r--   0 nosource  (1001) nosource  (1001)      435 2023-06-15 15:55:44.935960 copytrav-0.0.1/PKG-INFO
--rw-r--r--   0 nosource  (1001) nosource  (1001)       11 2023-06-14 20:42:55.000000 copytrav-0.0.1/README.md
--rw-r--r--   0 nosource  (1001) nosource  (1001)      605 2023-06-15 15:48:35.000000 copytrav-0.0.1/pyproject.toml
--rw-r--r--   0 nosource  (1001) nosource  (1001)       38 2023-06-15 15:55:44.935960 copytrav-0.0.1/setup.cfg
-drwxr-xr-x   0 nosource  (1001) nosource  (1001)        0 2023-06-15 15:55:44.933960 copytrav-0.0.1/src/
-drwxr-xr-x   0 nosource  (1001) nosource  (1001)        0 2023-06-15 15:55:44.934960 copytrav-0.0.1/src/copytrav/
--rw-r--r--   0 nosource  (1001) nosource  (1001)      990 2023-06-15 15:49:49.000000 copytrav-0.0.1/src/copytrav/__init__.py
-drwxr-xr-x   0 nosource  (1001) nosource  (1001)        0 2023-06-15 15:55:44.933960 copytrav-0.0.1/src/copytrav/data/
-drwxr-xr-x   0 nosource  (1001) nosource  (1001)        0 2023-06-15 15:55:44.934960 copytrav-0.0.1/src/copytrav/data/one/
--rw-r--r--   0 nosource  (1001) nosource  (1001)        3 2023-06-15 03:31:56.000000 copytrav-0.0.1/src/copytrav/data/one/data1.rst
--rw-r--r--   0 nosource  (1001) nosource  (1001)        3 2023-06-15 03:32:00.000000 copytrav-0.0.1/src/copytrav/data/one/data1.txt
-drwxr-xr-x   0 nosource  (1001) nosource  (1001)        0 2023-06-15 15:55:44.934960 copytrav-0.0.1/src/copytrav/data/two/
--rw-r--r--   0 nosource  (1001) nosource  (1001)        3 2023-06-15 03:32:04.000000 copytrav-0.0.1/src/copytrav/data/two/data2.rst
--rw-r--r--   0 nosource  (1001) nosource  (1001)        3 2023-06-15 03:32:06.000000 copytrav-0.0.1/src/copytrav/data/two/data2.txt
-drwxr-xr-x   0 nosource  (1001) nosource  (1001)        0 2023-06-15 15:55:44.935960 copytrav-0.0.1/src/copytrav/data/two/even_more_data/
--rw-r--r--   0 nosource  (1001) nosource  (1001)        0 2023-06-15 15:16:53.000000 copytrav-0.0.1/src/copytrav/data/two/even_more_data/data3.rst
--rw-r--r--   0 nosource  (1001) nosource  (1001)        0 2023-06-15 15:16:58.000000 copytrav-0.0.1/src/copytrav/data/two/even_more_data/data3.txt
-drwxr-xr-x   0 nosource  (1001) nosource  (1001)        0 2023-06-15 15:55:44.934960 copytrav-0.0.1/src/copytrav.egg-info/
--rw-r--r--   0 nosource  (1001) nosource  (1001)      435 2023-06-15 15:55:44.000000 copytrav-0.0.1/src/copytrav.egg-info/PKG-INFO
--rw-r--r--   0 nosource  (1001) nosource  (1001)      442 2023-06-15 15:55:44.000000 copytrav-0.0.1/src/copytrav.egg-info/SOURCES.txt
--rw-r--r--   0 nosource  (1001) nosource  (1001)        1 2023-06-15 15:55:44.000000 copytrav-0.0.1/src/copytrav.egg-info/dependency_links.txt
--rw-r--r--   0 nosource  (1001) nosource  (1001)        9 2023-06-15 15:55:44.000000 copytrav-0.0.1/src/copytrav.egg-info/top_level.txt
-drwxr-xr-x   0 nosource  (1001) nosource  (1001)        0 2023-06-15 15:55:44.935960 copytrav-0.0.1/tests/
--rw-r--r--   0 nosource  (1001) nosource  (1001)     2499 2023-06-15 15:49:49.000000 copytrav-0.0.1/tests/test_copy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:44:43.078216 copytrav-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-20 21:44:21.000000 copytrav-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-20 21:44:43.078216 copytrav-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-20 21:44:21.000000 copytrav-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-20 21:44:21.000000 copytrav-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 21:44:43.078216 copytrav-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:44:43.074216 copytrav-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:44:43.074216 copytrav-0.0.2/src/copytrav/
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-20 21:44:21.000000 copytrav-0.0.2/src/copytrav/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:44:43.074216 copytrav-0.0.2/src/copytrav/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:44:43.078216 copytrav-0.0.2/src/copytrav/data/one/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-20 21:44:21.000000 copytrav-0.0.2/src/copytrav/data/one/data1.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-20 21:44:21.000000 copytrav-0.0.2/src/copytrav/data/one/data1.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:44:43.078216 copytrav-0.0.2/src/copytrav/data/two/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-20 21:44:21.000000 copytrav-0.0.2/src/copytrav/data/two/data2.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-20 21:44:21.000000 copytrav-0.0.2/src/copytrav/data/two/data2.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:44:43.078216 copytrav-0.0.2/src/copytrav/data/two/even_more_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:44:21.000000 copytrav-0.0.2/src/copytrav/data/two/even_more_data/data3.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:44:21.000000 copytrav-0.0.2/src/copytrav/data/two/even_more_data/data3.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:44:43.078216 copytrav-0.0.2/src/copytrav.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-20 21:44:43.000000 copytrav-0.0.2/src/copytrav.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-20 21:44:43.000000 copytrav-0.0.2/src/copytrav.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 21:44:43.000000 copytrav-0.0.2/src/copytrav.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 21:44:43.000000 copytrav-0.0.2/src/copytrav.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 21:44:43.000000 copytrav-0.0.2/src/copytrav.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:44:43.078216 copytrav-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-06-20 21:44:21.000000 copytrav-0.0.2/tests/test_copy.py
```

### Comparing `copytrav-0.0.1/LICENSE` & `copytrav-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `copytrav-0.0.1/pyproject.toml` & `copytrav-0.0.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 [project]
 name = "copytrav"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name="Owen Shepherd", email="oshepengineering@gmail.com" },
 ]
 description = "Copy traversables as directories."
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
 ]
 
+[project.optional-dependencies]
+dev = [
+    "sphinx",
+    "sphinx-autodoc-typehints",
+    "sphinx-mdinclude",
+]
+
 [project.urls]
 "Homepage" = "https://github.com/OwenShepherd/copytrav"
 "Bug Tracker" = "https://github.com/OwenShepherd/copytrav/issues"
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
```

### Comparing `copytrav-0.0.1/src/copytrav/__init__.py` & `copytrav-0.0.2/src/copytrav/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,31 @@
-"""Package / module functions."""
+"""Copytrav provides the ability to create copies of python package data on disk."""
 import importlib.resources
 from importlib.resources.abc import Traversable
 import os
 from pathlib import Path
+import tempfile
+from typing import Union
 
-def copy(module: str, dst: Path, pth: Path=None):
+def copy(module: str, pth: Path=None, dst: Path=None) -> Path:
     """Given a module in the form: 'module.sub_module', copy all items at the
     pth to the destination, dst. If no path given, the module from the root
     level is copied.
+
+    Args:
+        module: The path to (typically) the namespace module containing data
+            in the example form "mymodule.data".
+        dst: Where you want the items copied to. Top-level dir is copied. If no
+            dst is given, a temporary directory will be created.
+        pth: Path in the example form
+            "item_at_module_root/level/directory_or_file".
+
+    Returns:
+        The path to the directory to which items were copied. If dst is given,
+        this will simply be dst.
     """
     def copy_aux(current_level: Traversable, current_path: Path):
         new_path = os.path.join(current_path, current_level.name)
         if current_level.is_dir():
             os.mkdir(new_path)
             for item in current_level.iterdir():
                 copy_aux(item, new_path)
@@ -19,8 +33,12 @@
             with open(new_path, "wb") as new_file:
                 new_file.write(current_level.read_bytes())
     start = importlib.resources.files(module)
     if pth:
         for_split = pth.split(os.path.sep)
         for level in for_split:
             start = start.joinpath(level)
+    if not dst:
+        dst = tempfile.mkdtemp(prefix=module.replace(".", "_"))
     copy_aux(start, dst)
+
+    return dst
```

### Comparing `copytrav-0.0.1/tests/test_copy.py` & `copytrav-0.0.2/tests/test_copy.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,44 +7,48 @@
 
 class TestCanCopy(unittest.TestCase):
     """Test can copy."""
     def setUp(self):
         self.tdir = tempfile.mkdtemp()
     def test_copy_even_more_data(self):
         """Tests copying data/two/even_more_data"""
-        copy("copytrav.data", self.tdir, "two/even_more_data")
+        copy("copytrav.data", "two/even_more_data", self.tdir)
         self.assertTrue(os.path.exists(os.path.join(self.tdir, "even_more_data")))
         self.assertTrue(os.path.exists(os.path.join(self.tdir, "even_more_data", "data3.rst")))
         self.assertTrue(os.path.exists(os.path.join(self.tdir, "even_more_data", "data3.txt")))
     def test_copy_just_module(self):
         """Tests copying just the module."""
-        copy("copytrav.data", self.tdir)
+        copy("copytrav.data", dst=self.tdir)
         one = os.path.join(self.tdir, "data", "one")
         two = os.path.join(self.tdir, "data", "two")
         emd = os.path.join(two, "even_more_data")
         self.assertTrue(os.path.exists(os.path.join(one, "data1.rst")))
         self.assertTrue(os.path.exists(os.path.join(one, "data1.txt")))
         self.assertTrue(os.path.exists(os.path.join(two, "data2.txt")))
         self.assertTrue(os.path.exists(os.path.join(two, "data2.rst")))
         self.assertTrue(os.path.exists(os.path.join(emd, "data3.txt")))
         self.assertTrue(os.path.exists(os.path.join(emd, "data3.rst")))
     def test_copy_one(self):
         """Tests copying just data/one"""
-        copy("copytrav.data", self.tdir, "one")
+        copy("copytrav.data", "one", self.tdir)
         one = os.path.join(self.tdir, "one")
         self.assertTrue(os.path.exists(os.path.join(one, "data1.rst")))
         self.assertTrue(os.path.exists(os.path.join(one, "data1.txt")))
     def test_copy_two(self):
         """Tests copying just data/two"""
-        copy("copytrav.data", self.tdir, "two")
+        copy("copytrav.data", "two", self.tdir)
         two = os.path.join(self.tdir, "two")
         emd = os.path.join(two, "even_more_data")
         self.assertTrue(os.path.exists(os.path.join(two, "data2.txt")))
         self.assertTrue(os.path.exists(os.path.join(two, "data2.rst")))
         self.assertTrue(os.path.exists(os.path.join(emd, "data3.txt")))
         self.assertTrue(os.path.exists(os.path.join(emd, "data3.rst")))
     def test_copy_single_file(self):
         """Tests copying a single file."""
-        copy("copytrav.data", self.tdir, "two/even_more_data/data3.rst")
+        copy("copytrav.data", "two/even_more_data/data3.rst", self.tdir)
+        self.assertTrue(os.path.exists(os.path.join(self.tdir, "data3.rst")))
+    def test_copy_without_dst(self):
+        """Tests copying a single file without supplying a dst."""
+        self.tdir = copy("copytrav.data", "two/even_more_data/data3.rst")
         self.assertTrue(os.path.exists(os.path.join(self.tdir, "data3.rst")))
     def tearDown(self):
         shutil.rmtree(self.tdir)
```

