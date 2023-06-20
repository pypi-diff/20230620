# Comparing `tmp/elastix_napari-0.2.0.tar.gz` & `tmp/elastix-napari-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elastix_napari-0.2.0.tar", last modified: Tue May  9 10:53:25 2023, max compression
+gzip compressed data, was "elastix-napari-0.2.1.tar", last modified: Tue Jun 20 18:13:50 2023, max compression
```

## Comparing `elastix_napari-0.2.0.tar` & `elastix-napari-0.2.1.tar`

### file list

```diff
@@ -1,45 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:53:25.187645 elastix_napari-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:53:25.183645 elastix_napari-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:53:25.187645 elastix_napari-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/.github/workflows/plugin_preview.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:53:25.187645 elastix_napari-0.2.0/.napari/
--rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/.napari/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/.napari/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-09 10:53:25.187645 elastix_napari-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:53:25.187645 elastix_napari-0.2.0/elastix_napari/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/elastix_napari/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8967 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/elastix_napari/elastix_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/elastix_napari/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:53:25.187645 elastix_napari-0.2.0/elastix_napari/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/elastix_napari/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/elastix_napari/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:53:25.187645 elastix_napari-0.2.0/elastix_napari/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   131383 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/elastix_napari/tests/data/CT_2D_head_fixed.mha
--rw-r--r--   0 runner    (1001) docker     (123)    65847 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/elastix_napari/tests/data/CT_2D_head_fixed_mask.mha
--rw-r--r--   0 runner    (1001) docker     (123)   131383 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/elastix_napari/tests/data/CT_2D_head_moving.mha
--rw-r--r--   0 runner    (1001) docker     (123)    65847 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/elastix_napari/tests/data/CT_2D_head_moving_mask.mha
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/elastix_napari/tests/data/TransformParameters.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/elastix_napari/tests/data/fixed_point_set_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/elastix_napari/tests/data/moving_point_set_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/elastix_napari/tests/data/parameters_Rigid.txt
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/elastix_napari/tests/test_dock_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/elastix_napari/tests/test_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/elastix_napari/tests/test_transformix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/elastix_napari/transformix_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/elastix_napari/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:53:25.187645 elastix_napari-0.2.0/elastix_napari.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-09 10:53:25.000000 elastix_napari-0.2.0/elastix_napari.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-09 10:53:25.000000 elastix_napari-0.2.0/elastix_napari.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 10:53:25.000000 elastix_napari-0.2.0/elastix_napari.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-09 10:53:25.000000 elastix_napari-0.2.0/elastix_napari.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-09 10:53:25.000000 elastix_napari-0.2.0/elastix_napari.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-09 10:53:25.000000 elastix_napari-0.2.0/elastix_napari.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 10:53:25.187645 elastix_napari-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-09 10:53:12.000000 elastix_napari-0.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:13:50.934662 elastix-napari-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:13:50.926662 elastix-napari-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:13:50.930662 elastix-napari-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-20 18:13:40.000000 elastix-napari-0.2.1/.github/workflows/plugin_preview.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-06-20 18:13:40.000000 elastix-napari-0.2.1/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-20 18:13:40.000000 elastix-napari-0.2.1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:13:50.930662 elastix-napari-0.2.1/.napari/
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-06-20 18:13:40.000000 elastix-napari-0.2.1/.napari/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-20 18:13:40.000000 elastix-napari-0.2.1/.napari/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-20 18:13:40.000000 elastix-napari-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-20 18:13:40.000000 elastix-napari-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-06-20 18:13:50.934662 elastix-napari-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-06-20 18:13:40.000000 elastix-napari-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:13:50.930662 elastix-napari-0.2.1/elastix_napari/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-20 18:13:40.000000 elastix-napari-0.2.1/elastix_napari/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-06-20 18:13:40.000000 elastix-napari-0.2.1/elastix_napari/elastix_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-20 18:13:40.000000 elastix-napari-0.2.1/elastix_napari/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:13:50.930662 elastix-napari-0.2.1/elastix_napari/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 18:13:40.000000 elastix-napari-0.2.1/elastix_napari/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-06-20 18:13:40.000000 elastix-napari-0.2.1/elastix_napari/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:13:50.934662 elastix-napari-0.2.1/elastix_napari/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   131383 2023-06-20 18:13:40.000000 elastix-napari-0.2.1/elastix_napari/tests/data/CT_2D_head_fixed.mha
+-rw-r--r--   0 runner    (1001) docker     (123)    65847 2023-06-20 18:13:40.000000 elastix-napari-0.2.1/elastix_napari/tests/data/CT_2D_head_fixed_mask.mha
+-rw-r--r--   0 runner    (1001) docker     (123)   131383 2023-06-20 18:13:40.000000 elastix-napari-0.2.1/elastix_napari/tests/data/CT_2D_head_moving.mha
+-rw-r--r--   0 runner    (1001) docker     (123)    65847 2023-06-20 18:13:40.000000 elastix-napari-0.2.1/elastix_napari/tests/data/CT_2D_head_moving_mask.mha
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-20 18:13:40.000000 elastix-napari-0.2.1/elastix_napari/tests/data/TransformParameters.0_2D.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-20 18:13:40.000000 elastix-napari-0.2.1/elastix_napari/tests/data/TransformParameters.0_3D.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-20 18:13:40.000000 elastix-napari-0.2.1/elastix_napari/tests/data/fixed_pointset_2D_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-20 18:13:40.000000 elastix-napari-0.2.1/elastix_napari/tests/data/fixed_pointset_3D_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-20 18:13:40.000000 elastix-napari-0.2.1/elastix_napari/tests/data/moving_pointset_2D_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 18:13:40.000000 elastix-napari-0.2.1/elastix_napari/tests/data/moving_pointset_3D_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-06-20 18:13:40.000000 elastix-napari-0.2.1/elastix_napari/tests/data/parameters_Rigid.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-20 18:13:40.000000 elastix-napari-0.2.1/elastix_napari/tests/test_dock_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-06-20 18:13:40.000000 elastix-napari-0.2.1/elastix_napari/tests/test_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-20 18:13:40.000000 elastix-napari-0.2.1/elastix_napari/tests/test_transformix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-06-20 18:13:40.000000 elastix-napari-0.2.1/elastix_napari/transformix_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-20 18:13:40.000000 elastix-napari-0.2.1/elastix_napari/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:13:50.930662 elastix-napari-0.2.1/elastix_napari.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-06-20 18:13:50.000000 elastix-napari-0.2.1/elastix_napari.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-20 18:13:50.000000 elastix-napari-0.2.1/elastix_napari.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 18:13:50.000000 elastix-napari-0.2.1/elastix_napari.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-20 18:13:50.000000 elastix-napari-0.2.1/elastix_napari.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-20 18:13:50.000000 elastix-napari-0.2.1/elastix_napari.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 18:13:50.000000 elastix-napari-0.2.1/elastix_napari.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-20 18:13:40.000000 elastix-napari-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 18:13:50.934662 elastix-napari-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-20 18:13:40.000000 elastix-napari-0.2.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-20 18:13:40.000000 elastix-napari-0.2.1/tox.ini
```

### Comparing `elastix_napari-0.2.0/.github/workflows/plugin_preview.yml` & `elastix-napari-0.2.1/.github/workflows/plugin_preview.yml`

 * *Files identical despite different names*

### Comparing `elastix_napari-0.2.0/.github/workflows/test_and_deploy.yml` & `elastix-napari-0.2.1/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `elastix_napari-0.2.0/.gitignore` & `elastix-napari-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `elastix_napari-0.2.0/.napari/DESCRIPTION.md` & `elastix-napari-0.2.1/.napari/DESCRIPTION.md`

 * *Files 1% similar despite different names*

```diff
@@ -65,13 +65,13 @@
 affine transformations.
 
 - [BSpline Transform](https://en.wikipedia.org/wiki/B-spline):
 This is a deformable transformation that preserves none of the properties mentioned in the transforms describe above.
 
 # Getting Help
 If you find a bug in the elastix napari plugin, or would like support with using it, please raise an
-issue on the [GitHub repository](https://github.com/SuperElastix/elastix_napari).
+issue on the [GitHub repository](https://github.com/SuperElastix/elastix-napari).
 
 For question specifically about the elastix toolbox we have a [mailing list](https://groups.google.com/forum/#!forum/elastix-imageregistration).
 
 # Contributions
-Contributions to the elastix_napari plugin, [itkelastix](https://github.com/InsightSoftwareConsortium/ITKElastix) (the python wrapper) or [elastix](https://github.com/SuperElastix/elastix) (the C++ core) on which the plugin is build, are welcome.
+Contributions to the elastix-napari plugin, [itkelastix](https://github.com/InsightSoftwareConsortium/ITKElastix) (the python wrapper) or [elastix](https://github.com/SuperElastix/elastix) (the C++ core) on which the plugin is build, are welcome.
```

### Comparing `elastix_napari-0.2.0/LICENSE` & `elastix-napari-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `elastix_napari-0.2.0/PKG-INFO` & `elastix-napari-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: elastix_napari
-Version: 0.2.0
+Name: elastix-napari
+Version: 0.2.1
 Summary: A toolbox for rigid and nonrigid registration of images.
-Home-page: https://github.com/SuperElastix/elastix_napari
+Home-page: https://github.com/SuperElastix/elastix-napari
 Author: Viktor van der Valk
 Author-email: v.o.van_der_valk@lumc.nl
 License: Apache Software License 2.0
 Project-URL: Project Site, https://elastix.lumc.nl/
-Project-URL: Bug Tracker, https://github.com/SuperElastix/elastix_napari/issues
-Project-URL: Source Code, https://github.com/SuperElastix/elastix_napari
+Project-URL: Bug Tracker, https://github.com/SuperElastix/elastix-napari/issues
+Project-URL: Source Code, https://github.com/SuperElastix/elastix-napari
 Project-URL: User Support, https://groups.google.com/g/elastix-imageregistration
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: napari
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -21,58 +21,58 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# elastix_napari
+# elastix-napari
 
-[![License](https://img.shields.io/pypi/l/elastix_napari.svg?color=green)](https://github.com/SuperElastix/elastix_napari/raw/main/LICENSE)
-[![PyPI](https://img.shields.io/pypi/v/elastix_napari.svg?color=green)](https://pypi.org/project/elastix_napari)
-[![Python Version](https://img.shields.io/pypi/pyversions/elastix_napari.svg?color=green)](https://python.org)
-[![tests](https://github.com/SuperElastix/elastix_napari/workflows/tests/badge.svg)](https://github.com/SuperElastix/elastix_napari/actions)
-[![codecov](https://codecov.io/gh/SuperElastix/elastix_napari/branch/main/graph/badge.svg)](https://codecov.io/gh/SuperElastix/elastix_napari)
+[![License](https://img.shields.io/pypi/l/elastix-napari.svg?color=green)](https://github.com/SuperElastix/elastix-napari/raw/main/LICENSE)
+[![PyPI](https://img.shields.io/pypi/v/elastix-napari.svg?color=green)](https://pypi.org/project/elastix-napari)
+[![Python Version](https://img.shields.io/pypi/pyversions/elastix-napari.svg?color=green)](https://python.org)
+[![tests](https://github.com/SuperElastix/elastix-napari/workflows/tests/badge.svg)](https://github.com/SuperElastix/elastix-napari/actions)
+[![codecov](https://codecov.io/gh/SuperElastix/elastix-napari/branch/main/graph/badge.svg)](https://codecov.io/gh/SuperElastix/elastix-napari)
 [![Youtube](https://img.shields.io/badge/YouTube-Demo-red)](https://www.youtube.com/watch?v=GzbP-qUR034)
 
 The [napari] plugin for [elastix], a toolbox for rigid and nonrigid registration of images, based on [itk-elastix].
 
 For a demo video see [youtube] channel.
 For tutorials on how to use elastix, see our [Jupyter notebooks].
 
 To find parameters that work well with specific datasets, see the [elastix Model Zoo].
 
 <img width="1438" alt="Screenshot 2021-05-12 at 15 07 24" src="https://user-images.githubusercontent.com/33719474/117980045-d6009b00-b333-11eb-9976-f64d34f4f7cc.png">
 
 ## Installation
 
-You can install `elastix_napari` via [pip]:
+You can install `elastix-napari` via [pip]:
 
-    pip install elastix_napari
+    pip install elastix-napari
 
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
 ## License
 
 Distributed under the terms of the [Apache Software License 2.0] license,
-"elastix_napari" is free and open source software
+"elastix-napari" is free and open source software
 
 ## Issues
 
 If you encounter any problems, please [file an issue] along with a detailed description.
 
 [napari]: https://github.com/napari/napari
 [Cookiecutter]: https://github.com/audreyr/cookiecutter
 [@napari]: https://github.com/napari
 [Apache Software License 2.0]: http://www.apache.org/licenses/LICENSE-2.0
 [cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
-[file an issue]: https://github.com/SuperElastix/elastix_napari/issues
+[file an issue]: https://github.com/SuperElastix/elastix-napari/issues
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
 [PyPI]: https://pypi.org/
 [elastix]: https://elastix.lumc.nl/
 [itk-elastix]: https://github.com/InsightSoftwareConsortium/ITKElastix
 [elastix Model Zoo]: https://elastix.lumc.nl/modelzoo/
 [Jupyter notebooks]: https://mybinder.org/v2/gh/InsightSoftwareConsortium/ITKElastix/master?urlpath=lab/tree/examples%2FITK_Example01_SimpleRegistration.ipynb
```

### Comparing `elastix_napari-0.2.0/README.md` & `elastix-napari-0.2.1/elastix_napari.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,51 +1,78 @@
-# elastix_napari
-
-[![License](https://img.shields.io/pypi/l/elastix_napari.svg?color=green)](https://github.com/SuperElastix/elastix_napari/raw/main/LICENSE)
-[![PyPI](https://img.shields.io/pypi/v/elastix_napari.svg?color=green)](https://pypi.org/project/elastix_napari)
-[![Python Version](https://img.shields.io/pypi/pyversions/elastix_napari.svg?color=green)](https://python.org)
-[![tests](https://github.com/SuperElastix/elastix_napari/workflows/tests/badge.svg)](https://github.com/SuperElastix/elastix_napari/actions)
-[![codecov](https://codecov.io/gh/SuperElastix/elastix_napari/branch/main/graph/badge.svg)](https://codecov.io/gh/SuperElastix/elastix_napari)
+Metadata-Version: 2.1
+Name: elastix-napari
+Version: 0.2.1
+Summary: A toolbox for rigid and nonrigid registration of images.
+Home-page: https://github.com/SuperElastix/elastix-napari
+Author: Viktor van der Valk
+Author-email: v.o.van_der_valk@lumc.nl
+License: Apache Software License 2.0
+Project-URL: Project Site, https://elastix.lumc.nl/
+Project-URL: Bug Tracker, https://github.com/SuperElastix/elastix-napari/issues
+Project-URL: Source Code, https://github.com/SuperElastix/elastix-napari
+Project-URL: User Support, https://groups.google.com/g/elastix-imageregistration
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Framework :: napari
+Classifier: Topic :: Software Development :: Testing
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# elastix-napari
+
+[![License](https://img.shields.io/pypi/l/elastix-napari.svg?color=green)](https://github.com/SuperElastix/elastix-napari/raw/main/LICENSE)
+[![PyPI](https://img.shields.io/pypi/v/elastix-napari.svg?color=green)](https://pypi.org/project/elastix-napari)
+[![Python Version](https://img.shields.io/pypi/pyversions/elastix-napari.svg?color=green)](https://python.org)
+[![tests](https://github.com/SuperElastix/elastix-napari/workflows/tests/badge.svg)](https://github.com/SuperElastix/elastix-napari/actions)
+[![codecov](https://codecov.io/gh/SuperElastix/elastix-napari/branch/main/graph/badge.svg)](https://codecov.io/gh/SuperElastix/elastix-napari)
 [![Youtube](https://img.shields.io/badge/YouTube-Demo-red)](https://www.youtube.com/watch?v=GzbP-qUR034)
 
 The [napari] plugin for [elastix], a toolbox for rigid and nonrigid registration of images, based on [itk-elastix].
 
 For a demo video see [youtube] channel.
 For tutorials on how to use elastix, see our [Jupyter notebooks].
 
 To find parameters that work well with specific datasets, see the [elastix Model Zoo].
 
 <img width="1438" alt="Screenshot 2021-05-12 at 15 07 24" src="https://user-images.githubusercontent.com/33719474/117980045-d6009b00-b333-11eb-9976-f64d34f4f7cc.png">
 
 ## Installation
 
-You can install `elastix_napari` via [pip]:
+You can install `elastix-napari` via [pip]:
 
-    pip install elastix_napari
+    pip install elastix-napari
 
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
 ## License
 
 Distributed under the terms of the [Apache Software License 2.0] license,
-"elastix_napari" is free and open source software
+"elastix-napari" is free and open source software
 
 ## Issues
 
 If you encounter any problems, please [file an issue] along with a detailed description.
 
 [napari]: https://github.com/napari/napari
 [Cookiecutter]: https://github.com/audreyr/cookiecutter
 [@napari]: https://github.com/napari
 [Apache Software License 2.0]: http://www.apache.org/licenses/LICENSE-2.0
 [cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
-[file an issue]: https://github.com/SuperElastix/elastix_napari/issues
+[file an issue]: https://github.com/SuperElastix/elastix-napari/issues
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
 [PyPI]: https://pypi.org/
 [elastix]: https://elastix.lumc.nl/
 [itk-elastix]: https://github.com/InsightSoftwareConsortium/ITKElastix
 [elastix Model Zoo]: https://elastix.lumc.nl/modelzoo/
 [Jupyter notebooks]: https://mybinder.org/v2/gh/InsightSoftwareConsortium/ITKElastix/master?urlpath=lab/tree/examples%2FITK_Example01_SimpleRegistration.ipynb
```

### Comparing `elastix_napari-0.2.0/elastix_napari/elastix_registration.py` & `elastix-napari-0.2.1/elastix_napari/elastix_registration.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,17 +155,17 @@
             parameter_map['MaximumStepLength'] = [str(max_step_length)]
             parameter_map['NumberOfSpatialSamples'] = [str(nr_spatial_samples)]
             parameter_map['MaximumNumberOfIterations'] = [str(max_iterations)]
         else:
             parameter_map = parameter_object.GetDefaultParameterMap(preset, 4)
         parameter_object.AddParameterMap(parameter_map)
 
-    kwargs = {"fixed_image": fixed_image,
-              "moving_image": moving_image,
-              "parameter_object": parameter_object,
+    args = [fixed_image, moving_image]
+
+    kwargs = {"parameter_object": parameter_object,
               "fixed_point_set_file_name": str(fixed_ps),
               "moving_point_set_file_name": str(moving_ps),
               "initial_transform_parameter_file_name": str(init_trans),
               "log_to_console": True}
 
     if masks:
         if fixed_mask is None and moving_mask is None:
@@ -185,15 +185,15 @@
         if not output_dir.is_dir() or output_dir == Path():
             return utils.error("Output directory is not chosen/valid")
 
         kwargs["output_directory"] = str(output_dir)            
 
 
     # Run elastix registration
-    result_image, result_transform_parameters = itk.elastix_registration_method(**kwargs)
+    result_image, result_transform_parameters = itk.elastix_registration_method(*args, **kwargs)
     
     # Convert result (itk.Image) to napari layer
     layer = image_layer_from_image(result_image)
     layer.name = preset + " Registration"
     return layer
```

### Comparing `elastix_napari-0.2.0/elastix_napari/napari.yaml` & `elastix-napari-0.2.1/elastix_napari/napari.yaml`

 * *Files identical despite different names*

### Comparing `elastix_napari-0.2.0/elastix_napari/tests/data/CT_2D_head_fixed.mha` & `elastix-napari-0.2.1/elastix_napari/tests/data/CT_2D_head_fixed.mha`

 * *Files identical despite different names*

### Comparing `elastix_napari-0.2.0/elastix_napari/tests/data/CT_2D_head_fixed_mask.mha` & `elastix-napari-0.2.1/elastix_napari/tests/data/CT_2D_head_fixed_mask.mha`

 * *Files identical despite different names*

### Comparing `elastix_napari-0.2.0/elastix_napari/tests/data/CT_2D_head_moving.mha` & `elastix-napari-0.2.1/elastix_napari/tests/data/CT_2D_head_moving.mha`

 * *Files identical despite different names*

### Comparing `elastix_napari-0.2.0/elastix_napari/tests/data/CT_2D_head_moving_mask.mha` & `elastix-napari-0.2.1/elastix_napari/tests/data/CT_2D_head_moving_mask.mha`

 * *Files identical despite different names*

### Comparing `elastix_napari-0.2.0/elastix_napari/tests/data/TransformParameters.0.txt` & `elastix-napari-0.2.1/elastix_napari/tests/data/TransformParameters.0_2D.txt`

 * *Files identical despite different names*

### Comparing `elastix_napari-0.2.0/elastix_napari/tests/data/parameters_Rigid.txt` & `elastix-napari-0.2.1/elastix_napari/tests/data/parameters_Rigid.txt`

 * *Files identical despite different names*

### Comparing `elastix_napari-0.2.0/elastix_napari/tests/test_dock_widget.py` & `elastix-napari-0.2.1/elastix_napari/tests/test_dock_widget.py`

 * *Files identical despite different names*

### Comparing `elastix_napari-0.2.0/elastix_napari/tests/test_registration.py` & `elastix-napari-0.2.1/elastix_napari/tests/test_registration.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,159 +2,150 @@
 import elastix_napari
 import itk
 from elastix_napari import elastix_registration
 import numpy as np
 from qtpy.QtWidgets import QMessageBox
 from itk_napari_conversion import image_layer_from_image
 from itk_napari_conversion import image_from_image_layer
-import tempfile
 from pathlib import Path
 
-# Helper functions
-def image_generator(x1, x2, y1, y2, mask=False, artefact=False,
-                    pointset=False, ps_name='fixed', data_dir='none'):
-    if mask:
-        image = np.zeros([100, 100], np.uint8)
-    elif pointset:
-        # Create fixed point set
-        filename = ps_name + "_point_set_test.txt"
-        point_set = open(str(data_dir / filename), "w+")
-        point_set.write("point\n4\n")
-        point_set.write(str(x1) + " " + str(y1) + "\n")
-        point_set.write(str(x1) + " " + str(y2) + "\n")
-        point_set.write(str(x2) + " " + str(y1) + "\n")
-        point_set.write(str(x2) + " " + str(y2) + "\n")
-        point_set.close()
-        return data_dir / filename
-    else:
-        image = np.zeros([100, 100], np.float32)
-    image[y1:y2, x1:x2] = 1
-    if artefact:
-        image[-10:, :] = 1
-    image = itk.image_view_from_array(image)
-    image = image_layer_from_image(image)
-    return image
-
 
 def get_er(*args, **kwargs):
     er_func = elastix_registration.elastix_registration()
     return er_func(*args, **kwargs)
 
+# See explanation in conftest.py
+def uncollect_if(images=None, masks=None, pointsets=None):
+    if not pointsets:
+        return ('2D' in images) != ('2D' in masks)
+    else:
+        return ('2D' in images) != ('2D' in pointsets)
+
 
-# Test normal registration
-def test_registration():
-    fixed_image = image_generator(25, 75, 25, 75)
-    moving_image = image_generator(1, 51, 10, 60)
+def test_registration(images, default_rigid, data_dir):
+    fixed_image, moving_image = images
     result_image = get_er(fixed_image, moving_image, preset='rigid')
-    mean_diff = np.absolute(np.subtract(
-        np.asarray(image_from_image_layer(result_image)),
-        np.asarray(image_from_image_layer(fixed_image)))).mean()
-    assert mean_diff < 0.001
-
-
-# Test Masked registration
-def test_masked_registration():
-    fixed_image = image_generator(25, 75, 25, 75, artefact=True)
-    moving_image = image_generator(1, 51, 10, 60, artefact=True)
-
-    # Create mask for artefact
-    fixed_mask = image_generator(0, 100, 0, 90, mask=True)
-    moving_mask = image_generator(0, 100, 0, 90, mask=True)
 
-    result_image = get_er(fixed_image=fixed_image, moving_image=moving_image,
+    reference_result_image, _ = itk.elastix_registration_method(image_from_image_layer(fixed_image), 
+                                                             image_from_image_layer(moving_image), 
+                                                             parameter_object=default_rigid)
+    
+    fixed_filepath = Path(data_dir) / "fixed.nii"
+    moving_filepath = Path(data_dir) / "moving.nii"
+
+    fixed_image = image_from_image_layer(fixed_image)
+    moving_image = image_from_image_layer(moving_image)
+
+    itk.imwrite(fixed_image, str(fixed_filepath))
+    itk.imwrite(moving_image, str(moving_filepath))
+    assert np.allclose(image_from_image_layer(result_image), reference_result_image)
+
+# Test masked registration
+@pytest.mark.uncollect_if(func=uncollect_if)
+def test_masked_registration(images, masks, default_rigid):
+    fixed_image, moving_image = images
+    fixed_mask, moving_mask = masks
+    result_image = get_er(fixed_image, moving_image,
                           fixed_mask=fixed_mask, moving_mask=moving_mask,
                           preset='rigid', masks=True)
+    reference_result_image, _ = itk.elastix_registration_method(image_from_image_layer(fixed_image), 
+                                                             image_from_image_layer(moving_image),
+                                                             fixed_mask=image_from_image_layer(fixed_mask),
+                                                             moving_mask=image_from_image_layer(moving_mask),
+                                                             parameter_object=default_rigid)
+
+    assert np.allclose(image_from_image_layer(result_image), reference_result_image)
 
-    # Filter artifacts out of the images.
-    masked_fixed_image = np.asarray(
-        image_from_image_layer(fixed_image))[0:90, 0:90]
-    masked_result_image = np.asarray(
-        image_from_image_layer(result_image))[0:90, 0:90]
-
-    mean_diff = np.absolute(np.subtract(masked_fixed_image,
-                                        masked_result_image)).mean()
-    assert mean_diff < 0.001
-
-
-# Test Point set registration
-def test_pointset_registration(data_dir):
-    fixed_image = image_generator(25, 75, 25, 75)
-    moving_image = image_generator(1, 51, 10, 60)
-
-    # Create pointsets for artefact
-    fixed_ps = image_generator(25, 75, 25, 75, pointset=True, ps_name='fixed',
-                               data_dir=data_dir)
-    moving_ps = image_generator(1, 51, 10, 60, pointset=True, ps_name='moving',
-                                data_dir=data_dir)
 
+# Test point set registration
+@pytest.mark.uncollect_if(func=uncollect_if)
+def test_pointset_registration(images, pointsets, default_rigid):
+    fixed_image, moving_image = images
+    fixed_ps, moving_ps = pointsets
     result_image = get_er(fixed_image, moving_image, fixed_ps=fixed_ps,
                           moving_ps=moving_ps, preset='rigid',
                           advanced=True)
+    default_rigid.SetParameter(0, "Registration", "MultiMetricMultiResolutionRegistration")
+    default_rigid.SetParameter(0, "Metric", [default_rigid.GetParameter(0, "Metric")[0], 
+                                             "CorrespondingPointsEuclideanDistanceMetric"])
+    reference_result_image, _ = itk.elastix_registration_method(image_from_image_layer(fixed_image), 
+                                                             image_from_image_layer(moving_image),
+                                                             parameter_object=default_rigid,
+                                                             fixed_point_set_file_name=str(fixed_ps),
+                                                             moving_point_set_file_name=str(moving_ps))
+    assert np.allclose(image_from_image_layer(result_image), reference_result_image, atol=0.5)
 
-    mean_diff = np.absolute(np.subtract(
-        np.asarray(image_from_image_layer(result_image)),
-        np.asarray(image_from_image_layer(fixed_image)))).mean()
-    assert mean_diff < 0.001
 
 
 # Test registration with custom parameter textfiles
-def test_custom_registration(data_dir):
-    fixed_image = image_generator(25, 75, 25, 75)
-    moving_image = image_generator(1, 51, 10, 60)
-
+# TODO: Test multiple parameter files as well
+def test_custom_registration(images, data_dir):
+    fixed_image, moving_image = images
     filename = "parameters_Rigid.txt"
     result_image = get_er(fixed_image, moving_image, preset='custom',
-                          param1=data_dir / filename,
-                          param2=data_dir / filename)
+                          param1=data_dir / filename)
 
-    mean_diff = np.absolute(np.subtract(
-        np.asarray(image_from_image_layer(result_image)),
-        np.asarray(image_from_image_layer(fixed_image)))).mean()
-    assert mean_diff < 0.01
+    parameter_object = itk.ParameterObject.New()
+    parameter_object.AddParameterFile(str(data_dir / filename))
 
+    reference_result_image, _ = itk.elastix_registration_method(image_from_image_layer(fixed_image), 
+                                                             image_from_image_layer(moving_image),
+                                                             parameter_object=parameter_object)
+    assert np.allclose(image_from_image_layer(result_image), reference_result_image)
+
+
+# TODO: This test tests more than one things --> split into two
+# TODO: Test that any combination of UI options is depicted correctly in the parameter object
+def test_initial_transform(images, default_rigid, data_dir):
+    fixed_image, moving_image = images
+    if len(fixed_image.data.shape) == 2:
+        init_trans_filename = "TransformParameters.0_2D.txt"
+    else:
+        init_trans_filename = "TransformParameters.0_3D.txt"
 
-def test_initial_transform(data_dir):
-    fixed_image = image_generator(25, 75, 25, 75)
-    moving_image = image_generator(1, 51, 10, 60)
-
-    init_trans_filename = "TransformParameters.0.txt"
+    resolutions = 3
+    max_iterations = 50
     result_image = get_er(
         fixed_image, moving_image, preset='rigid',
-        init_trans=data_dir / init_trans_filename, resolutions=6,
-        max_iterations=500, advanced=True)
-    mean_diff = np.absolute(np.subtract(
-        np.asarray(image_from_image_layer(result_image)),
-        np.asarray(image_from_image_layer(fixed_image)))).mean()
-    assert mean_diff < 0.01
+        init_trans=data_dir / init_trans_filename, resolutions=resolutions,
+        max_iterations=max_iterations, advanced=True)
+        
+    # TODO: Advanced should take default values from the current parameter map
+    default_rigid.SetParameter(0, "Metric", "AdvancedMattesMutualInformation")
+    default_rigid.SetParameter(0, "MaximumNumberOfIterations", str(max_iterations))
+    default_rigid.SetParameter(0, "NumberOfResolutions", str(resolutions))
+    default_rigid.SetParameter(0, "NumberOfSpatialSamples", str(512))
+    default_rigid.SetParameter(0, "MaximumStepLength", str(1.0))
+
+    reference_result_image, _ = itk.elastix_registration_method(image_from_image_layer(fixed_image), 
+                                                             image_from_image_layer(moving_image), 
+                                                             parameter_object=default_rigid,
+                                                             initial_transform_parameter_file_name=str(data_dir / init_trans_filename))
+    
+    diff = image_from_image_layer(result_image)[:] - reference_result_image[:]
+    print(diff.min(), diff.max())
+    assert np.allclose(image_from_image_layer(result_image), reference_result_image)
 
 
 def test_empty_images():
     im = get_er(None, None, preset='rigid')
     assert isinstance(im, QMessageBox)
 
 
-def test_empty_masks():
-    fixed_image = image_generator(25, 75, 25, 75)
-    moving_image = image_generator(1, 51, 10, 60)
+def test_empty_masks(images):
+    fixed_image, moving_image = images
     im = get_er(fixed_image, moving_image, fixed_mask=None, moving_mask=None,
                 preset='rigid', masks=True)
     assert isinstance(im, QMessageBox)
 
-def test_empty_output_dir():
-    fixed_image = image_generator(25, 75, 25, 75)
-    moving_image = image_generator(1, 51, 10, 60)
+def test_empty_output_dir(images):
+    fixed_image, moving_image = images
     im = get_er(fixed_image, moving_image, preset='rigid', save_output=True)
     assert isinstance(im, QMessageBox)
 
-def test_writing_result():
-
-    fixed_image = image_generator(25, 75, 25, 75)
-    moving_image = image_generator(1, 51, 10, 60)
-
-    with tempfile.TemporaryDirectory() as tmpdirname:
-        tmpdir = Path(tmpdirname)
-        im = get_er(fixed_image, moving_image, preset='rigid', save_output=True,
-                    output_dir=tmpdir)
-        assert (tmpdir / "TransformParameters.0.txt").exists()
-    
-
-
+def test_writing_result(images, tmpdir):
+    fixed_image, moving_image = images
+    tmpdir = Path(tmpdir)
+    im = get_er(fixed_image, moving_image, preset='rigid', save_output=True,
+                output_dir=tmpdir)
+    assert (tmpdir / "TransformParameters.0.txt").exists()
+
```

### Comparing `elastix_napari-0.2.0/elastix_napari/tests/test_transformix.py` & `elastix-napari-0.2.1/elastix_napari/tests/test_transformix.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,20 @@
 import pytest
 import itk
 import numpy as np
 from elastix_napari import transformix_widget
-from elastix_napari.tests.test_registration import image_generator
 from itk_napari_conversion import image_from_image_layer
 from qtpy.QtWidgets import QMessageBox
 from pathlib import Path
 
-def test_transformation(tmpdir):
-    fixed_image = image_generator(25, 75, 25, 75)
-    moving_image = image_generator(1, 51, 10, 60)
-
-    parameter_object = itk.ParameterObject.New()
-    default_rigid_parameter_map = parameter_object.GetDefaultParameterMap('rigid')
-    parameter_object.AddParameterMap(default_rigid_parameter_map)
-
+def test_transformation(images, default_rigid, tmpdir):
+    fixed_image, moving_image = images
     result_image_elx, result_transform_parameters = itk.elastix_registration_method(image_from_image_layer(fixed_image),
                                                                                     image_from_image_layer(moving_image),
-                                                                                    parameter_object=parameter_object,
+                                                                                    parameter_object=default_rigid,
                                                                                     output_directory=str(tmpdir)
                                                                                     )
 
     result_image_trx = transformix_widget.create_transformix_widget()(image=moving_image, 
                                                                       transform_file=Path(tmpdir) / "TransformParameters.0.txt")
     
     result_image_elx = np.asarray(result_image_elx)
@@ -31,17 +24,16 @@
 
 
 def test_empty_image(data_dir):
     result = transformix_widget.create_transformix_widget()(image=None, transform_file=data_dir / "TransformParameters.0.txt")
     assert isinstance(result, QMessageBox)
 
 
-def test_empty_transform_file():
-    image = image_generator(25, 75, 25, 75)
-    result = transformix_widget.create_transformix_widget()(image=image_from_image_layer(image), transform_file=Path())
+def test_empty_transform_file(images):
+    result = transformix_widget.create_transformix_widget()(image=image_from_image_layer(images[1]), transform_file=Path())
     assert isinstance(result, QMessageBox)
```

### Comparing `elastix_napari-0.2.0/elastix_napari/transformix_widget.py` & `elastix-napari-0.2.1/elastix_napari/transformix_widget.py`

 * *Files identical despite different names*

### Comparing `elastix_napari-0.2.0/elastix_napari/utils.py` & `elastix-napari-0.2.1/elastix_napari/utils.py`

 * *Files identical despite different names*

### Comparing `elastix_napari-0.2.0/elastix_napari.egg-info/SOURCES.txt` & `elastix-napari-0.2.1/elastix_napari.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -25,11 +25,14 @@
 elastix_napari/tests/test_dock_widget.py
 elastix_napari/tests/test_registration.py
 elastix_napari/tests/test_transformix.py
 elastix_napari/tests/data/CT_2D_head_fixed.mha
 elastix_napari/tests/data/CT_2D_head_fixed_mask.mha
 elastix_napari/tests/data/CT_2D_head_moving.mha
 elastix_napari/tests/data/CT_2D_head_moving_mask.mha
-elastix_napari/tests/data/TransformParameters.0.txt
-elastix_napari/tests/data/fixed_point_set_test.txt
-elastix_napari/tests/data/moving_point_set_test.txt
+elastix_napari/tests/data/TransformParameters.0_2D.txt
+elastix_napari/tests/data/TransformParameters.0_3D.txt
+elastix_napari/tests/data/fixed_pointset_2D_test.txt
+elastix_napari/tests/data/fixed_pointset_3D_test.txt
+elastix_napari/tests/data/moving_pointset_2D_test.txt
+elastix_napari/tests/data/moving_pointset_3D_test.txt
 elastix_napari/tests/data/parameters_Rigid.txt
```

### Comparing `elastix_napari-0.2.0/setup.py` & `elastix-napari-0.2.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,19 +31,19 @@
             requirements.append(stripped)
 
 
 # https://github.com/pypa/setuptools_scm
 use_scm = {"write_to": "elastix_napari/_version.py"}
 
 setup(
-    name='elastix_napari',
+    name='elastix-napari',
     author='Viktor van der Valk',
     author_email='v.o.van_der_valk@lumc.nl',
     license='Apache Software License 2.0',
-    url='https://github.com/SuperElastix/elastix_napari',
+    url='https://github.com/SuperElastix/elastix-napari',
     description='A toolbox for rigid and nonrigid registration of images.',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     python_requires='>=3.8',
     install_requires=requirements,
     version=get_version("elastix_napari/__init__.py"),
@@ -59,14 +59,14 @@
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Operating System :: OS Independent',
         'License :: OSI Approved :: Apache Software License',
     ],
     project_urls={
         'Project Site': 'https://elastix.lumc.nl/',
-        'Bug Tracker': 'https://github.com/SuperElastix/elastix_napari/issues',
-        'Source Code': 'https://github.com/SuperElastix/elastix_napari',
+        'Bug Tracker': 'https://github.com/SuperElastix/elastix-napari/issues',
+        'Source Code': 'https://github.com/SuperElastix/elastix-napari',
         'User Support': 'https://groups.google.com/g/elastix-imageregistration',
     },
     entry_points={'napari.manifest': ['elastix-napari = elastix_napari:napari.yaml']},
     package_data={'elastix_napari': ['napari.yaml']}
 )
```

### Comparing `elastix_napari-0.2.0/tox.ini` & `elastix-napari-0.2.1/tox.ini`

 * *Files identical despite different names*

