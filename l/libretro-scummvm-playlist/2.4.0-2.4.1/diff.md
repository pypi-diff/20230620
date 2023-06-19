# Comparing `tmp/libretro_scummvm_playlist-2.4.0.tar.gz` & `tmp/libretro_scummvm_playlist-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libretro_scummvm_playlist-2.4.0.tar", max compression
+gzip compressed data, was "libretro_scummvm_playlist-2.4.1.tar", max compression
```

## Comparing `libretro_scummvm_playlist-2.4.0.tar` & `libretro_scummvm_playlist-2.4.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1063 2023-03-23 20:51:58.336991 libretro_scummvm_playlist-2.4.0/LICENSE
--rw-r--r--   0        0        0       22 2023-03-23 20:51:58.336991 libretro_scummvm_playlist-2.4.0/libretro_scummvm_playlist/__init__.py
--rw-r--r--   0        0        0    15159 2023-03-23 20:51:58.336991 libretro_scummvm_playlist-2.4.0/libretro_scummvm_playlist/__main__.py
--rw-r--r--   0        0        0      697 2023-03-23 20:51:58.336991 libretro_scummvm_playlist-2.4.0/pyproject.toml
--rw-r--r--   0        0        0      816 2023-03-23 20:52:07.801379 libretro_scummvm_playlist-2.4.0/setup.py
--rw-r--r--   0        0        0      648 2023-03-23 20:52:07.801640 libretro_scummvm_playlist-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-19 22:59:03.762868 libretro_scummvm_playlist-2.4.1/LICENSE
+-rw-r--r--   0        0        0       22 2023-06-19 22:59:03.766868 libretro_scummvm_playlist-2.4.1/libretro_scummvm_playlist/__init__.py
+-rw-r--r--   0        0        0    15160 2023-06-19 22:59:03.766868 libretro_scummvm_playlist-2.4.1/libretro_scummvm_playlist/__main__.py
+-rw-r--r--   0        0        0      697 2023-06-19 22:59:03.766868 libretro_scummvm_playlist-2.4.1/pyproject.toml
+-rw-r--r--   0        0        0      817 2023-06-19 22:59:13.296290 libretro_scummvm_playlist-2.4.1/setup.py
+-rw-r--r--   0        0        0      649 2023-06-19 22:59:13.296546 libretro_scummvm_playlist-2.4.1/PKG-INFO
```

### Comparing `libretro_scummvm_playlist-2.4.0/LICENSE` & `libretro_scummvm_playlist-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `libretro_scummvm_playlist-2.4.0/libretro_scummvm_playlist/__main__.py` & `libretro_scummvm_playlist-2.4.1/libretro_scummvm_playlist/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 
     libretro-scummvm-playlist removes the need for step 3 and 4 if you did step 1 and 2.
 
     To update this program to the latest release with pip installed, type:
 
     pip install --force-reinstall libretro_scummvm_playlist
     
-    If you'd like to try to download missing coverart until a PR with scummvm names is added to the thumbnail server try to install and use libretrofuzz:
+    If you'd like to try to download missing coverart until a PR with scummvm names is added to the thumbnail server try to install and use libretro-fuzz:
     
     pip install --force-reinstall libretrofuzz
     """
     if not cfg.is_file():
         error(f'Invalid Retroarch cfg file: {cfg}')
         raise typer.Exit(code=1)
```

### Comparing `libretro_scummvm_playlist-2.4.0/pyproject.toml` & `libretro_scummvm_playlist-2.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "libretro_scummvm_playlist"
-version = "2.4.0"
+version = "2.4.1"
 description = "libretro scummvm playlist builder"
 authors = ["i30817 <i30817@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-typer = {extras = ["all"], version = "^0.5.0"}
+typer = {extras = ["all"], version = "^0.9.0"}
 
 [tool.poetry.scripts]
 libretro-scummvm-playlist = 'libretro_scummvm_playlist.__main__:main'
 
 [tool.poetry.urls]
 "homepage" = 'https://github.com/i30817/libretro-mkscumm'
 "documentation" = 'https://github.com/i30817/libretro-mkscumm#readme'
```

### Comparing `libretro_scummvm_playlist-2.4.0/setup.py` & `libretro_scummvm_playlist-2.4.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 packages = \
 ['libretro_scummvm_playlist']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['typer[all]>=0.5.0,<0.6.0']
+['typer[all]>=0.9.0,<0.10.0']
 
 entry_points = \
 {'console_scripts': ['libretro-scummvm-playlist = '
                      'libretro_scummvm_playlist.__main__:main']}
 
 setup_kwargs = {
     'name': 'libretro-scummvm-playlist',
-    'version': '2.4.0',
+    'version': '2.4.1',
     'description': 'libretro scummvm playlist builder',
     'long_description': None,
     'author': 'i30817',
     'author_email': 'i30817@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `libretro_scummvm_playlist-2.4.0/PKG-INFO` & `libretro_scummvm_playlist-2.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: libretro-scummvm-playlist
-Version: 2.4.0
+Version: 2.4.1
 Summary: libretro scummvm playlist builder
 Author: i30817
 Author-email: i30817@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: typer[all] (>=0.5.0,<0.6.0)
+Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Project-URL: Bug Tracker, https://github.com/i30817/libretro-mkscumm/issues
 Project-URL: documentation, https://github.com/i30817/libretro-mkscumm#readme
 Project-URL: homepage, https://github.com/i30817/libretro-mkscumm
```

