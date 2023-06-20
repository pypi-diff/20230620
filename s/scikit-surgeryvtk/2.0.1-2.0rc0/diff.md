# Comparing `tmp/scikit-surgeryvtk-2.0.1.tar.gz` & `tmp/scikit-surgeryvtk-2.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-surgeryvtk-2.0.1.tar", last modified: Tue Jun 20 16:14:32 2023, max compression
+gzip compressed data, was "scikit-surgeryvtk-2.0rc0.tar", last modified: Wed Mar  8 13:17:20 2023, max compression
```

## Comparing `scikit-surgeryvtk-2.0.1.tar` & `scikit-surgeryvtk-2.0rc0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:14:32.960513 scikit-surgeryvtk-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-06-20 16:14:32.960513 scikit-surgeryvtk-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:14:32.956514 scikit-surgeryvtk-2.0.1/scikit_surgeryvtk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-06-20 16:14:32.000000 scikit-surgeryvtk-2.0.1/scikit_surgeryvtk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-20 16:14:32.000000 scikit-surgeryvtk-2.0.1/scikit_surgeryvtk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:14:32.000000 scikit-surgeryvtk-2.0.1/scikit_surgeryvtk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-20 16:14:32.000000 scikit-surgeryvtk-2.0.1/scikit_surgeryvtk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-20 16:14:32.000000 scikit-surgeryvtk-2.0.1/scikit_surgeryvtk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-20 16:14:32.000000 scikit-surgeryvtk-2.0.1/scikit_surgeryvtk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-20 16:14:32.960513 scikit-surgeryvtk-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:14:32.960513 scikit-surgeryvtk-2.0.1/sksurgeryvtk/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/sksurgeryvtk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-20 16:14:32.960513 scikit-surgeryvtk-2.0.1/sksurgeryvtk/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:14:32.956514 scikit-surgeryvtk-2.0.1/sksurgeryvtk/camera/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/sksurgeryvtk/camera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/sksurgeryvtk/camera/vtk_camera_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:14:32.956514 scikit-surgeryvtk-2.0.1/sksurgeryvtk/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/sksurgeryvtk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/sksurgeryvtk/models/outline_render.py
--rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/sksurgeryvtk/models/surface_model_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    24842 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/sksurgeryvtk/models/voxelise.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/sksurgeryvtk/models/vtk_base_actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/sksurgeryvtk/models/vtk_base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/sksurgeryvtk/models/vtk_cylinder_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/sksurgeryvtk/models/vtk_grid_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/sksurgeryvtk/models/vtk_image_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/sksurgeryvtk/models/vtk_point_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/sksurgeryvtk/models/vtk_sphere_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8661 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/sksurgeryvtk/models/vtk_surface_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8155 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/sksurgeryvtk/models/vtk_surface_model_directory_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:14:32.956514 scikit-surgeryvtk-2.0.1/sksurgeryvtk/text/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/sksurgeryvtk/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/sksurgeryvtk/text/text_overlay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:14:32.956514 scikit-surgeryvtk-2.0.1/sksurgeryvtk/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/sksurgeryvtk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/sksurgeryvtk/utils/matrix_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/sksurgeryvtk/utils/platform_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/sksurgeryvtk/utils/polydata_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/sksurgeryvtk/utils/projection_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:14:32.956514 scikit-surgeryvtk-2.0.1/sksurgeryvtk/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/sksurgeryvtk/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9975 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/sksurgeryvtk/widgets/vtk_interlaced_stereo_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     9816 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/sksurgeryvtk/widgets/vtk_lus_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    20038 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/sksurgeryvtk/widgets/vtk_overlay_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     9709 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/sksurgeryvtk/widgets/vtk_rendering_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11618 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/sksurgeryvtk/widgets/vtk_reslice_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:14:32.952514 scikit-surgeryvtk-2.0.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:14:32.956514 scikit-surgeryvtk-2.0.1/tests/camera/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/tests/camera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/tests/camera/test_liver_overlay.py
--rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/tests/camera/test_vtk_camera_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:14:32.960513 scikit-surgeryvtk-2.0.1/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/tests/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/tests/models/test_surface_model_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    12732 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/tests/models/test_voxelise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/tests/models/test_vtk_cylinder_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/tests/models/test_vtk_image_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/tests/models/test_vtk_point_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/tests/models/test_vtk_sphere_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11807 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/tests/models/test_vtk_surface_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/tests/models/test_vtk_surface_model_directory_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/tests/models/test_vtk_unstructured_grid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:14:32.960513 scikit-surgeryvtk-2.0.1/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/tests/utils/test_matrix_utills.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/tests/utils/test_polydata_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/tests/utils/test_projection_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:14:32.960513 scikit-surgeryvtk-2.0.1/tests/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/tests/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/tests/widgets/test_interlaced_stereo_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     8165 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/tests/widgets/test_lus_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15673 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/tests/widgets/test_rendering_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9746 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/tests/widgets/test_vtk_overlay_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/tests/widgets/test_vtk_overlay_window_with_outlines.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/tests/widgets/test_vtk_reslice.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-06-20 16:14:23.000000 scikit-surgeryvtk-2.0.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 13:17:20.085534 scikit-surgeryvtk-2.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-03-08 13:17:10.000000 scikit-surgeryvtk-2.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-08 13:17:10.000000 scikit-surgeryvtk-2.0rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-03-08 13:17:20.085534 scikit-surgeryvtk-2.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-03-08 13:17:10.000000 scikit-surgeryvtk-2.0rc0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 13:17:20.069534 scikit-surgeryvtk-2.0rc0/scikit_surgeryvtk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-03-08 13:17:19.000000 scikit-surgeryvtk-2.0rc0/scikit_surgeryvtk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-03-08 13:17:20.000000 scikit-surgeryvtk-2.0rc0/scikit_surgeryvtk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 13:17:19.000000 scikit-surgeryvtk-2.0rc0/scikit_surgeryvtk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-08 13:17:19.000000 scikit-surgeryvtk-2.0rc0/scikit_surgeryvtk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-08 13:17:19.000000 scikit-surgeryvtk-2.0rc0/scikit_surgeryvtk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-08 13:17:19.000000 scikit-surgeryvtk-2.0rc0/scikit_surgeryvtk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-08 13:17:20.085534 scikit-surgeryvtk-2.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-03-08 13:17:10.000000 scikit-surgeryvtk-2.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 13:17:20.085534 scikit-surgeryvtk-2.0rc0/sksurgeryvtk/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-08 13:17:10.000000 scikit-surgeryvtk-2.0rc0/sksurgeryvtk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-03-08 13:17:20.085534 scikit-surgeryvtk-2.0rc0/sksurgeryvtk/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 13:17:20.073534 scikit-surgeryvtk-2.0rc0/sksurgeryvtk/camera/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 13:17:10.000000 scikit-surgeryvtk-2.0rc0/sksurgeryvtk/camera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11201 2023-03-08 13:17:10.000000 scikit-surgeryvtk-2.0rc0/sksurgeryvtk/camera/vtk_camera_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 13:17:20.077534 scikit-surgeryvtk-2.0rc0/sksurgeryvtk/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 13:17:10.000000 scikit-surgeryvtk-2.0rc0/sksurgeryvtk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-03-08 13:17:10.000000 scikit-surgeryvtk-2.0rc0/sksurgeryvtk/models/outline_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-03-08 13:17:10.000000 scikit-surgeryvtk-2.0rc0/sksurgeryvtk/models/surface_model_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24841 2023-03-08 13:17:10.000000 scikit-surgeryvtk-2.0rc0/sksurgeryvtk/models/voxelise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-03-08 13:17:10.000000 scikit-surgeryvtk-2.0rc0/sksurgeryvtk/models/vtk_base_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-03-08 13:17:10.000000 scikit-surgeryvtk-2.0rc0/sksurgeryvtk/models/vtk_base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-03-08 13:17:10.000000 scikit-surgeryvtk-2.0rc0/sksurgeryvtk/models/vtk_cylinder_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-03-08 13:17:10.000000 scikit-surgeryvtk-2.0rc0/sksurgeryvtk/models/vtk_grid_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-03-08 13:17:10.000000 scikit-surgeryvtk-2.0rc0/sksurgeryvtk/models/vtk_image_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-03-08 13:17:10.000000 scikit-surgeryvtk-2.0rc0/sksurgeryvtk/models/vtk_point_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-03-08 13:17:10.000000 scikit-surgeryvtk-2.0rc0/sksurgeryvtk/models/vtk_sphere_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-03-08 13:17:10.000000 scikit-surgeryvtk-2.0rc0/sksurgeryvtk/models/vtk_surface_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8155 2023-03-08 13:17:10.000000 scikit-surgeryvtk-2.0rc0/sksurgeryvtk/models/vtk_surface_model_directory_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 13:17:20.077534 scikit-surgeryvtk-2.0rc0/sksurgeryvtk/text/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 13:17:10.000000 scikit-surgeryvtk-2.0rc0/sksurgeryvtk/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-03-08 13:17:10.000000 scikit-surgeryvtk-2.0rc0/sksurgeryvtk/text/text_overlay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 13:17:20.081534 scikit-surgeryvtk-2.0rc0/sksurgeryvtk/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 13:17:10.000000 scikit-surgeryvtk-2.0rc0/sksurgeryvtk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-03-08 13:17:10.000000 scikit-surgeryvtk-2.0rc0/sksurgeryvtk/utils/matrix_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-03-08 13:17:10.000000 scikit-surgeryvtk-2.0rc0/sksurgeryvtk/utils/platform_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-03-08 13:17:10.000000 scikit-surgeryvtk-2.0rc0/sksurgeryvtk/utils/polydata_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-03-08 13:17:10.000000 scikit-surgeryvtk-2.0rc0/sksurgeryvtk/utils/projection_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 13:17:20.081534 scikit-surgeryvtk-2.0rc0/sksurgeryvtk/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 13:17:10.000000 scikit-surgeryvtk-2.0rc0/sksurgeryvtk/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-03-08 13:17:10.000000 scikit-surgeryvtk-2.0rc0/sksurgeryvtk/widgets/vtk_interlaced_stereo_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9816 2023-03-08 13:17:10.000000 scikit-surgeryvtk-2.0rc0/sksurgeryvtk/widgets/vtk_lus_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20038 2023-03-08 13:17:11.000000 scikit-surgeryvtk-2.0rc0/sksurgeryvtk/widgets/vtk_overlay_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9709 2023-03-08 13:17:11.000000 scikit-surgeryvtk-2.0rc0/sksurgeryvtk/widgets/vtk_rendering_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11618 2023-03-08 13:17:11.000000 scikit-surgeryvtk-2.0rc0/sksurgeryvtk/widgets/vtk_reslice_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 13:17:20.065534 scikit-surgeryvtk-2.0rc0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 13:17:20.081534 scikit-surgeryvtk-2.0rc0/tests/camera/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 13:17:11.000000 scikit-surgeryvtk-2.0rc0/tests/camera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-03-08 13:17:11.000000 scikit-surgeryvtk-2.0rc0/tests/camera/test_liver_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-03-08 13:17:11.000000 scikit-surgeryvtk-2.0rc0/tests/camera/test_vtk_camera_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 13:17:20.081534 scikit-surgeryvtk-2.0rc0/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 13:17:11.000000 scikit-surgeryvtk-2.0rc0/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-03-08 13:17:11.000000 scikit-surgeryvtk-2.0rc0/tests/models/test_surface_model_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12732 2023-03-08 13:17:11.000000 scikit-surgeryvtk-2.0rc0/tests/models/test_voxelise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-03-08 13:17:11.000000 scikit-surgeryvtk-2.0rc0/tests/models/test_vtk_cylinder_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-03-08 13:17:11.000000 scikit-surgeryvtk-2.0rc0/tests/models/test_vtk_image_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-03-08 13:17:11.000000 scikit-surgeryvtk-2.0rc0/tests/models/test_vtk_point_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-03-08 13:17:11.000000 scikit-surgeryvtk-2.0rc0/tests/models/test_vtk_sphere_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11807 2023-03-08 13:17:11.000000 scikit-surgeryvtk-2.0rc0/tests/models/test_vtk_surface_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-03-08 13:17:11.000000 scikit-surgeryvtk-2.0rc0/tests/models/test_vtk_surface_model_directory_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-03-08 13:17:11.000000 scikit-surgeryvtk-2.0rc0/tests/models/test_vtk_unstructured_grid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 13:17:20.081534 scikit-surgeryvtk-2.0rc0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 13:17:11.000000 scikit-surgeryvtk-2.0rc0/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-03-08 13:17:11.000000 scikit-surgeryvtk-2.0rc0/tests/utils/test_matrix_utills.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-03-08 13:17:11.000000 scikit-surgeryvtk-2.0rc0/tests/utils/test_polydata_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-03-08 13:17:11.000000 scikit-surgeryvtk-2.0rc0/tests/utils/test_projection_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 13:17:20.085534 scikit-surgeryvtk-2.0rc0/tests/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 13:17:11.000000 scikit-surgeryvtk-2.0rc0/tests/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-03-08 13:17:11.000000 scikit-surgeryvtk-2.0rc0/tests/widgets/test_interlaced_stereo_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8165 2023-03-08 13:17:11.000000 scikit-surgeryvtk-2.0rc0/tests/widgets/test_lus_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15675 2023-03-08 13:17:11.000000 scikit-surgeryvtk-2.0rc0/tests/widgets/test_rendering_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9746 2023-03-08 13:17:11.000000 scikit-surgeryvtk-2.0rc0/tests/widgets/test_vtk_overlay_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-03-08 13:17:11.000000 scikit-surgeryvtk-2.0rc0/tests/widgets/test_vtk_overlay_window_with_outlines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-03-08 13:17:11.000000 scikit-surgeryvtk-2.0rc0/tests/widgets/test_vtk_reslice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-03-08 13:17:11.000000 scikit-surgeryvtk-2.0rc0/versioneer.py
```

### Comparing `scikit-surgeryvtk-2.0.1/LICENSE` & `scikit-surgeryvtk-2.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.0.1/PKG-INFO` & `scikit-surgeryvtk-2.0rc0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 1.1
 Name: scikit-surgeryvtk
-Version: 2.0.1
+Version: 2.0rc0
 Summary: scikit-surgeryvtk implements VTK for Image Guided Surgery applications
 Home-page: https://github.com/SciKit-Surgery/scikit-surgeryvtk
 Author: Thomas Dowrick
 Author-email: t.dowrick@ucl.ac.uk
 License: BSD-3 license
 Description: scikit-surgeryvtk
         ===============================
         
-        .. image:: https://raw.githubusercontent.com/SciKit-Surgery/scikit-surgeryvtk/master/sksvtk_logo.png
+        .. image:: sksvtk_logo.png
            :height: 128px
            :width: 128px
            :target: https://github.com/SciKit-Surgery/scikit-surgeryvtk 
            :alt: Logo
         
         |
         
@@ -33,16 +33,16 @@
            :target: https://doi.org/10.1007/s11548-020-02180-5
            :alt: The SciKit-Surgery paper
         
         .. image:: https://img.shields.io/twitter/follow/scikit_surgery?style=social
            :target: https://twitter.com/scikit_surgery?ref_src=twsrc%5Etfw
            :alt: Follow scikit_surgery on twitter
         
-        Author(s): Stephen Thompson, Matt Clarkson, Thomas Dowrick and Miguel Xochicale;
-        Contributor(s): Mian Ahmad.
+        Author(s): Stephen Thompson and Matt Clarkson;
+        Contributor(s): Miguel Xochicale, Thomas Dowrick, and Mian Ahmad.
         
         scikit-surgeryvtk implements VTK for Image Guided Surgery applications.
         
         scikit-surgeryvtk is part of the `SciKit-Surgery`_ software project, developed at the `Wellcome EPSRC Centre for Interventional and Surgical Sciences`_, part of `University College London (UCL)`_.
         
         scikit-surgeryvtk is tested on Python 3.8. and may support other Python versions.
         
@@ -78,22 +78,20 @@
         
             git clone https://github.com/SciKit-Surgery/scikit-surgeryvtk
         
         
         Running the tests
         ^^^^^^^^^^^^^^^^^
         
-        You can run the unit tests, build documentation, and other options by installing and running tox:
+        You can run the unit tests by installing and running tox:
         
         ::
         
             pip install tox
             tox
-            tox -e docs
-            tox -e lint
         
         
         Encountering Problems?
         ^^^^^^^^^^^^^^^^^^^^^^
         Please get in touch or raise an `issue`_.
         
         
@@ -132,17 +130,18 @@
         .. _`EPSRC`: https://www.epsrc.ac.uk/
         .. _`contributing guidelines`: https://github.com/SciKit-Surgery/scikit-surgeryvtk/blob/master/CONTRIBUTING.rst
         .. _`license file`: https://github.com/SciKit-Surgery/scikit-surgeryvtkblob/master/LICENSE
         .. _`common issues`: https://weisslab.cs.ucl.ac.uk/WEISS/SoftwareRepositories/SNAPPY/scikit-surgery/wikis/Common-Issues
         .. _`issue`: https://github.com/SciKit-Surgery/scikit-surgeryvtk/issues/new
 Keywords: medical imaging
 Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
```

### Comparing `scikit-surgeryvtk-2.0.1/README.rst` & `scikit-surgeryvtk-2.0rc0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 scikit-surgeryvtk
 ===============================
 
-.. image:: https://raw.githubusercontent.com/SciKit-Surgery/scikit-surgeryvtk/master/sksvtk_logo.png
+.. image:: sksvtk_logo.png
    :height: 128px
    :width: 128px
    :target: https://github.com/SciKit-Surgery/scikit-surgeryvtk 
    :alt: Logo
 
 |
 
@@ -25,16 +25,16 @@
    :target: https://doi.org/10.1007/s11548-020-02180-5
    :alt: The SciKit-Surgery paper
 
 .. image:: https://img.shields.io/twitter/follow/scikit_surgery?style=social
    :target: https://twitter.com/scikit_surgery?ref_src=twsrc%5Etfw
    :alt: Follow scikit_surgery on twitter
 
-Author(s): Stephen Thompson, Matt Clarkson, Thomas Dowrick and Miguel Xochicale;
-Contributor(s): Mian Ahmad.
+Author(s): Stephen Thompson and Matt Clarkson;
+Contributor(s): Miguel Xochicale, Thomas Dowrick, and Mian Ahmad.
 
 scikit-surgeryvtk implements VTK for Image Guided Surgery applications.
 
 scikit-surgeryvtk is part of the `SciKit-Surgery`_ software project, developed at the `Wellcome EPSRC Centre for Interventional and Surgical Sciences`_, part of `University College London (UCL)`_.
 
 scikit-surgeryvtk is tested on Python 3.8. and may support other Python versions.
 
@@ -70,22 +70,20 @@
 
     git clone https://github.com/SciKit-Surgery/scikit-surgeryvtk
 
 
 Running the tests
 ^^^^^^^^^^^^^^^^^
 
-You can run the unit tests, build documentation, and other options by installing and running tox:
+You can run the unit tests by installing and running tox:
 
 ::
 
     pip install tox
     tox
-    tox -e docs
-    tox -e lint
 
 
 Encountering Problems?
 ^^^^^^^^^^^^^^^^^^^^^^
 Please get in touch or raise an `issue`_.
```

### Comparing `scikit-surgeryvtk-2.0.1/scikit_surgeryvtk.egg-info/PKG-INFO` & `scikit-surgeryvtk-2.0rc0/scikit_surgeryvtk.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 1.1
 Name: scikit-surgeryvtk
-Version: 2.0.1
+Version: 2.0rc0
 Summary: scikit-surgeryvtk implements VTK for Image Guided Surgery applications
 Home-page: https://github.com/SciKit-Surgery/scikit-surgeryvtk
 Author: Thomas Dowrick
 Author-email: t.dowrick@ucl.ac.uk
 License: BSD-3 license
 Description: scikit-surgeryvtk
         ===============================
         
-        .. image:: https://raw.githubusercontent.com/SciKit-Surgery/scikit-surgeryvtk/master/sksvtk_logo.png
+        .. image:: sksvtk_logo.png
            :height: 128px
            :width: 128px
            :target: https://github.com/SciKit-Surgery/scikit-surgeryvtk 
            :alt: Logo
         
         |
         
@@ -33,16 +33,16 @@
            :target: https://doi.org/10.1007/s11548-020-02180-5
            :alt: The SciKit-Surgery paper
         
         .. image:: https://img.shields.io/twitter/follow/scikit_surgery?style=social
            :target: https://twitter.com/scikit_surgery?ref_src=twsrc%5Etfw
            :alt: Follow scikit_surgery on twitter
         
-        Author(s): Stephen Thompson, Matt Clarkson, Thomas Dowrick and Miguel Xochicale;
-        Contributor(s): Mian Ahmad.
+        Author(s): Stephen Thompson and Matt Clarkson;
+        Contributor(s): Miguel Xochicale, Thomas Dowrick, and Mian Ahmad.
         
         scikit-surgeryvtk implements VTK for Image Guided Surgery applications.
         
         scikit-surgeryvtk is part of the `SciKit-Surgery`_ software project, developed at the `Wellcome EPSRC Centre for Interventional and Surgical Sciences`_, part of `University College London (UCL)`_.
         
         scikit-surgeryvtk is tested on Python 3.8. and may support other Python versions.
         
@@ -78,22 +78,20 @@
         
             git clone https://github.com/SciKit-Surgery/scikit-surgeryvtk
         
         
         Running the tests
         ^^^^^^^^^^^^^^^^^
         
-        You can run the unit tests, build documentation, and other options by installing and running tox:
+        You can run the unit tests by installing and running tox:
         
         ::
         
             pip install tox
             tox
-            tox -e docs
-            tox -e lint
         
         
         Encountering Problems?
         ^^^^^^^^^^^^^^^^^^^^^^
         Please get in touch or raise an `issue`_.
         
         
@@ -132,17 +130,18 @@
         .. _`EPSRC`: https://www.epsrc.ac.uk/
         .. _`contributing guidelines`: https://github.com/SciKit-Surgery/scikit-surgeryvtk/blob/master/CONTRIBUTING.rst
         .. _`license file`: https://github.com/SciKit-Surgery/scikit-surgeryvtkblob/master/LICENSE
         .. _`common issues`: https://weisslab.cs.ucl.ac.uk/WEISS/SoftwareRepositories/SNAPPY/scikit-surgery/wikis/Common-Issues
         .. _`issue`: https://github.com/SciKit-Surgery/scikit-surgeryvtk/issues/new
 Keywords: medical imaging
 Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
```

### Comparing `scikit-surgeryvtk-2.0.1/scikit_surgeryvtk.egg-info/SOURCES.txt` & `scikit-surgeryvtk-2.0rc0/scikit_surgeryvtk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.0.1/setup.py` & `scikit-surgeryvtk-2.0rc0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,33 +13,32 @@
 setup(
     name='scikit-surgeryvtk',
     version=versioneer.get_version(),
     cmdclass=versioneer.get_cmdclass(),
     description='scikit-surgeryvtk implements VTK for Image Guided Surgery applications',
     long_description=long_description,
     url='https://github.com/SciKit-Surgery/scikit-surgeryvtk',
-    # Authors: Stephen Thompson, Matt Clarkson, Thomas Dowrick and Miguel Xochicale
-    # PyPI does not have an option to specify multiple authors.
     author='Thomas Dowrick',
     author_email='t.dowrick@ucl.ac.uk',
     license='BSD-3 license',
     classifiers=[
-        'Development Status :: 5 - Production/Stable',
+        'Development Status :: 3 - Alpha',
 
         'Intended Audience :: Developers',
         'Intended Audience :: Healthcare Industry',
         'Intended Audience :: Information Technology',
         'Intended Audience :: Science/Research',
 
 
         'License :: OSI Approved :: BSD License',
 
 
         'Programming Language :: Python',
-        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 2',
+        'Programming Language :: Python :: 3',
 
         'Topic :: Scientific/Engineering :: Information Analysis',
         'Topic :: Scientific/Engineering :: Medical Science Apps.',
     ],
 
     keywords='medical imaging',
 
@@ -48,16 +47,16 @@
             'doc',
             'tests',
         ]
     ),
 
     install_requires=[
         'numpy>=1.11',
-        'vtk>=9.2.6',
-        'PySide6>=6.5.1.1',
+        'vtk>=9.2.5',
+        'PySide6>=6.4.2',
         'opencv-contrib-python-headless>=4.2.0.32',
         'scikit-surgerycore>=0.1.7',
         'scikit-surgeryimage>=0.10.1',
     ],
 
     entry_points={
         'console_scripts': [
```

### Comparing `scikit-surgeryvtk-2.0.1/sksurgeryvtk/camera/vtk_camera_model.py` & `scikit-surgeryvtk-2.0rc0/sksurgeryvtk/camera/vtk_camera_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,17 +37,14 @@
 
     Thanks to:
     `Andrew Straw <http://strawlab.org/2011/11/05/augmented-reality-with-OpenGL/>`_.
 
     whose method was also implemented in:
     `NifTK <https://cmiclab.cs.ucl.ac.uk/CMIC/NifTK/blob/master/MITK/Modules/Core/Rendering/vtkOpenGLMatrixDrivenCamera.cxx#L119>`_.
 
-    and it appears it should also be available in:
-    `VTK <https://gitlab.kitware.com/vtk/vtk/merge_requests/882>`_.
-
     Note: If you use this method, the display will look ok, but as of VTK 8.1.0,
     it won't work with vtkWindowToImageFilter, as the window to image filter
     tries to render the image in tiles. This requires instantiating temporary
     new vtkCamera, and the vtkCamera copy constructor, shallow copy and deep copy
     do not actually copy the UseExplicitProjectionTransformMatrixOn or
     ExplicitProjectionTransformMatrix.
 
@@ -82,14 +79,20 @@
     # pylint: disable=line-too-long
     """
     Used on vtkCamera when you are trying to set the viewport to only render
     to a part of the total window size. For example, this occurs when you
     have calibrated a video camera using OpenCV, on images of 1920 x 1080,
     and then you are displaying in a VTK window that is twice as wide/high.
 
+    This was implemented in:
+    `NifTK <https://cmiclab.cs.ucl.ac.uk/CMIC/NifTK/blob/master/MITK/Modules/Core/Rendering/vtkOpenGLMatrixDrivenCamera.cxx#L129>`_.
+
+    and it appears it should also be available in:
+    `VTK <https://gitlab.kitware.com/vtk/vtk/merge_requests/882>`_.
+
     :param window_width: in pixels
     :param window_height: in pixels
     :param image_width: in pixels
     :param image_height: in pixels
     :param aspect_ratio: relative physical size of pixels, as x/y.
     :return: scissor_x, scissor_y, scissor_width, scissor_height in pixels
     """
```

### Comparing `scikit-surgeryvtk-2.0.1/sksurgeryvtk/models/outline_render.py` & `scikit-surgeryvtk-2.0rc0/sksurgeryvtk/models/outline_render.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.0.1/sksurgeryvtk/models/surface_model_loader.py` & `scikit-surgeryvtk-2.0rc0/sksurgeryvtk/models/surface_model_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,17 +4,15 @@
 Module to load VTK surfaces using dictionary from ConfigurationManager.
 """
 
 # pylint: disable=too-many-branches
 
 import logging
 import os
-
 import vtk
-
 import sksurgeryvtk.models.vtk_surface_model as sm
 
 LOGGER = logging.getLogger(__name__)
 
 
 class SurfaceModelLoader:
     """
@@ -24,14 +22,15 @@
 
     Surfaces have format:
 
     .. code-block::
 
         "surfaces": {
             "tumor": {
+
                 "file": "path/to/model/tumor.vtk",
                 "colour": [255, 0, 0],
                 "opacity": 0.5,
                 "visibility": true,
                 "pickable": true,
                 "toggleable": true,
                 "texture": "path/to/texture/image.png",
@@ -43,15 +42,14 @@
     .. code-block::
 
         "assemblies": {
             "whole model": ["part1", "part2", "part3"]
         }
 
     """
-
     def __init__(self, data, directory_prefix=None):
         """
         Loads surface models and (optionally) assemblies from
         dictionary loaded by sksurgerycore.ConfigurationManager.
 
         :param data: data from sksurgerycore.ConfigurationManager
         :param prefix: directory name prefix as string
```

### Comparing `scikit-surgeryvtk-2.0.1/sksurgeryvtk/models/voxelise.py` & `scikit-surgeryvtk-2.0rc0/sksurgeryvtk/models/voxelise.py`

 * *Files 0% similar despite different names*

```diff
@@ -219,24 +219,22 @@
              grid_elements: int = 64,
              move_input: float = None,
              center: bool = False,
              scale_input: float = None,
              reuse_transform: bool = False,
              signed_df: bool = True
              ):
-    """
-    Creates a voxelised distance field, stores it in a vtkStructuredGrid,
-    optimally writes to disk.
+    """ Creates a voxelised distance field, stores it in a vtkStructuredGrid,\
+        optinally writes to disk.
 
     :param input_mesh: Input mesh/points. Can be path to model file, \
      or numpy array. Units of mesh should be in metres.
-    :type input_mesh: Union[np.ndarray, str
+    :type input_mesh: Union[np.ndarray, str]
     :param output_grid: Either a vtkStrucutredGrid object, or a file that
-     contains one (or will be created).
-     If not specified, a grid will be created.
+    contains one (or will be created), if not specified, a grid will be created.
     :type output_grid: Union[vtk.vtkStructuredGrid, str], optional
     :param array_name: Name of array in which to store distance field, \
      if not specified, defaults to preoperativeSurface for if signed_df = True,
      else intraoperativeSurface
     :type array_name: str, optional
     :param size: Grid size, defaults to 0.3
     :type size: float, optional
@@ -244,20 +242,20 @@
     :type grid_elements: int, optional
     :param move_input: Move the input before transforming to distance field \
      (movement is applied before scaling! defaults to None
     :type move_input: float, optional
     :param center: Center the data around the origin. defaults to False
     :type center: bool, optional
     :param scale_input: Scale the input before transforming to distance field \
-     (movement is applied before scaling!). Input is expected to be in metres, \
-     if it is in mm, set scale_input to 0.001 defaults to None
+    (movement is applied before scaling!). Input is expected to be in metres, \
+        if it is in mm, set scale_input to 0.001 defaults to None
     :type scale_input: float, optional
-    :param reuse_transform: Reuse transformation already stored in the grid.
-     Use this if you want to center mesh 1 and
-     then apply the same transformation to mesh 2.
+    :param reuse_transform: Reuse transformation already stored in the grid. \
+    Use this if you want to center mesh 1 and then apply the same transformation
+     to mesh 2.
      Mutually exclusive with center, scale_input and move_input.
      defaults to False
     :type reuse_transform: bool, optional
     :param signed_df: Calcualte signed or unsigned distance field.
      defaults to True
     :type signed_df: bool, optional
     :return grid: Grid containing distance field.
```

### Comparing `scikit-surgeryvtk-2.0.1/sksurgeryvtk/models/vtk_base_actor.py` & `scikit-surgeryvtk-2.0rc0/sksurgeryvtk/models/vtk_base_actor.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.0.1/sksurgeryvtk/models/vtk_base_model.py` & `scikit-surgeryvtk-2.0rc0/sksurgeryvtk/models/vtk_base_model.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.0.1/sksurgeryvtk/models/vtk_cylinder_model.py` & `scikit-surgeryvtk-2.0rc0/sksurgeryvtk/models/vtk_cylinder_model.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.0.1/sksurgeryvtk/models/vtk_grid_model.py` & `scikit-surgeryvtk-2.0rc0/sksurgeryvtk/models/vtk_grid_model.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.0.1/sksurgeryvtk/models/vtk_image_model.py` & `scikit-surgeryvtk-2.0rc0/sksurgeryvtk/models/vtk_image_model.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.0.1/sksurgeryvtk/models/vtk_point_model.py` & `scikit-surgeryvtk-2.0rc0/sksurgeryvtk/models/vtk_point_model.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.0.1/sksurgeryvtk/models/vtk_sphere_model.py` & `scikit-surgeryvtk-2.0rc0/sksurgeryvtk/models/vtk_sphere_model.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.0.1/sksurgeryvtk/models/vtk_surface_model.py` & `scikit-surgeryvtk-2.0rc0/sksurgeryvtk/models/vtk_surface_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,15 +188,14 @@
         """
         self.transform_filter.Update()
         return self.source
 
     def get_normals_as_numpy(self):
         """
          Returns the vtkPolyData point normals as a numpy array.
-
         :return: nx3 numpy ndarray
         """
         self.transform_filter.Update()
         vtk_normals = self.transform_filter \
             .GetOutput().GetPointData().GetNormals()
         as_numpy = numpy_support.vtk_to_numpy(vtk_normals)
         return as_numpy
```

### Comparing `scikit-surgeryvtk-2.0.1/sksurgeryvtk/models/vtk_surface_model_directory_loader.py` & `scikit-surgeryvtk-2.0rc0/sksurgeryvtk/models/vtk_surface_model_directory_loader.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.0.1/sksurgeryvtk/text/text_overlay.py` & `scikit-surgeryvtk-2.0rc0/sksurgeryvtk/text/text_overlay.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,15 +177,16 @@
     Text will rescale if the window resizes, to try and maintain relative
     positioning.
 
     :param text: text to display.
     :param    x: x position (pixels)
     :param    y: y position (pixels)
     :param font_size: Font size
-    :param colour: Colour, RGB tuple
+    param colour: Colour, RGB tuple
+
     """
 
     def __init__(self, text, x, y, font_size=24, colour=(1.0, 0, 0)):
         """ Create a VTK text actor.
         """
 
         self.text_actor = vtk.vtkTextActor()
@@ -196,16 +197,16 @@
         self.set_font_size(font_size)
 
         r, g, b = colour
         self.set_colour(r, g, b)
 
     def set_parent_window(self, parent_window):
         """
-        Link the object to a VTKOverlayWindow and set up callbacks.
-
+        Link the object to a VTKOverlayWindow
+        and set up callbacks.
         :param parent_window: VTKOverlayWindow
         """
         self.parent_window = parent_window
         self.calculate_relative_position_in_window()
 
         self.parent_window.AddObserver('ModifiedEvent',
                                        self.callback_update_position_in_window)
@@ -276,17 +277,16 @@
         self.text_actor.GetTextProperty().SetVerticalJustificationToCentered()
 
         self.set_text_string(text)
 
     def set_parent_window(self, parent_window):
         """
         Attach text to a particular window.
-
-        :param parent_window: VTKOverlayWindow that message will be
-         displayed in.
+        :param parent_window: VTKOverlayWindow that message will
+                     be displayed in.
         """
 
         self.parent_window = parent_window
         self.parent_window.AddObserver('ModifiedEvent',
                                        self.calculate_text_size)
         self.calculate_text_size(None, None)
```

### Comparing `scikit-surgeryvtk-2.0.1/sksurgeryvtk/utils/matrix_utils.py` & `scikit-surgeryvtk-2.0rc0/sksurgeryvtk/utils/matrix_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     from right to left, and so matches VTK.
 
     Furthermore, the construct_rotm_from_euler function in scikit-surgerycore
     expectes the user to pass the parameters in, in the order specified
     in the provided string.
 
     :param params list of exactly 6 numbers.
-    :param is_in_radians: True if radians, False otherwise, default is False
+    :param is_in_radians True if radians, False otherwise, default is False
     """
     if len(params) != 6:
         raise ValueError("Incorrect list size:" + str(params))
 
     rot = tm.construct_rotm_from_euler(params[2],
                                        params[0],
                                        params[1],
@@ -95,15 +95,15 @@
 
 def create_matrix_from_string(parameter_string, is_in_radians=False):
     """
     Generates a 4x4 numpy ndarray from a comma separated
     string of the format rx,ry,rz,tx,ty,tz in degrees, millimetres.
 
     :param parameter_string: rx,ry,rz,tx,ty,tz in degrees/millimetres
-    :param is_in_radians: True if radians, False otherwise, default is False
+    :param is_in_radians True if radians, False otherwise, default is False
     :return: 4x4 rigid body transform
     """
     params = parameter_string.split(',')
     if len(params) != 6:
         raise ValueError("Incorrect extrinsic:" + parameter_string)
 
     param_list = [float(params[0]),
```

### Comparing `scikit-surgeryvtk-2.0.1/sksurgeryvtk/utils/polydata_utils.py` & `scikit-surgeryvtk-2.0rc0/sksurgeryvtk/utils/polydata_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.0.1/sksurgeryvtk/utils/projection_utils.py` & `scikit-surgeryvtk-2.0rc0/sksurgeryvtk/utils/projection_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     """
     Projects all 3D points to 2D, using OpenCV cv2.projectPoints().
 
     :param points: nx3 ndarray representing 3D points, typically in millimetres
     :param camera_to_world: 4x4 ndarray representing camera to world transform
     :param camera_matrix: 3x3 ndarray representing OpenCV camera intrinsics
     :param distortion: 1x4,5 etc. OpenCV distortion parameters
-    :raises: ValueError, TypeError:
+    :raises ValueError, TypeError:
     :return: nx2 ndarray representing 2D points, typically in pixels
     """
 
     _validate_input_for_projection(points,
                                    camera_to_world,
                                    camera_matrix,
                                    distortion)
@@ -92,27 +92,28 @@
                           distortion=None,
                           upper_cos_theta=0
                          ):
     """
     Projects 3D points that face the camera to 2D pixels.
 
     This assumes:
-    Camera direction is a unit vector from the camera, towards focal point.
-    Surface Normal is a unit vector pointing out from the surface.
+
+      Camera direction is a unit vector from the camera, towards focal point.
+      Surface Normal is a unit vector pointing out from the surface.
+
     Vectors are not checked for unit length.
 
     :param points: nx3 ndarray representing 3D points, typically in millimetres
     :param normals: nx3 ndarray representing unit normals for the same points
     :param camera_to_world: 4x4 ndarray representing camera to world transform
     :param camera_matrix: 3x3 ndarray representing OpenCV camera intrinsics
     :param distortion: 1x4,5 etc. OpenCV distortion parameters
-    :param upper_cos_theta: upper limit for cos theta, angle between normal and
-        viewing direction, where cos theta is normally -1 to 0.
-
-    :raises: ValueError, TypeError:
+    :param upper_cos_theta: upper limit for cos theta, angle between normal
+    and viewing direction, where cos theta is normally -1 to 0.
+    :raises ValueError, TypeError:
     :return: projected_facing_points_2d
     """
     _validate_input_for_projection(points,
                                    camera_to_world,
                                    camera_matrix,
                                    distortion)
```

### Comparing `scikit-surgeryvtk-2.0.1/sksurgeryvtk/widgets/vtk_interlaced_stereo_window.py` & `scikit-surgeryvtk-2.0rc0/sksurgeryvtk/widgets/vtk_interlaced_stereo_window.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,15 @@
     def set_video_images(self, left_image, right_image):
         """
         Sets both left and right video images. Images
         must be the same shape, and have an even number of rows.
 
         :param left_image: left numpy image
         :param right_image: right numpy image
-        :raises: ValueError, TypeError
+        :raises ValueError, TypeError
         """
         if not isinstance(left_image, np.ndarray):
             raise TypeError('left image is not an np.ndarray')
         if not isinstance(right_image, np.ndarray):
             raise TypeError('right image is not an np.ndarray')
         if left_image.shape != right_image.shape:
             raise ValueError('left and right images differ in shape')
```

### Comparing `scikit-surgeryvtk-2.0.1/sksurgeryvtk/widgets/vtk_lus_simulator.py` & `scikit-surgeryvtk-2.0rc0/sksurgeryvtk/widgets/vtk_lus_simulator.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.0.1/sksurgeryvtk/widgets/vtk_overlay_window.py` & `scikit-surgeryvtk-2.0rc0/sksurgeryvtk/widgets/vtk_overlay_window.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.0.1/sksurgeryvtk/widgets/vtk_rendering_generator.py` & `scikit-surgeryvtk-2.0rc0/sksurgeryvtk/widgets/vtk_rendering_generator.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.0.1/sksurgeryvtk/widgets/vtk_reslice_widget.py` & `scikit-surgeryvtk-2.0rc0/sksurgeryvtk/widgets/vtk_reslice_widget.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.0.1/tests/camera/test_liver_overlay.py` & `scikit-surgeryvtk-2.0rc0/tests/camera/test_liver_overlay.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,19 @@
 # -*- coding: utf-8 -*-
 
 import copy
 import os
 import platform
-import pytest
 
 import cv2
 import numpy as np
 from sksurgeryimage.utilities.utilities import are_similar
 
 import sksurgeryvtk.models.vtk_surface_model as sm
 
-skip_pytest_in_runner_macos = pytest.mark.skipif(
-    platform.system() == "Darwin",
-    reason=f'for [{platform.system()} OSs with CI=[{os.environ.get("CI")}] with RUNNER_OS=[{os.environ.get("RUNNER_OS")}] '
-           f'{os.environ.get("SESSION_MANAGER")[0:20] if (platform.system() == "Darwin" and os.environ.get("GITHUB_ACTIONS") == None) else ""} '
-           f'with {os.environ.get("XDG_CURRENT_DESKTOP") if (platform.system() == "Darwin" and os.environ.get("GITHUB_ACTIONS") == None) else ""} '
-           f'due to issues with Fatal Python error: Segmentation fault'
-)
 
 def _reproject_and_save_image(image,
                               model_to_camera,
                               point_cloud,
                               camera_matrix,
                               output_file):
     """
@@ -55,15 +47,15 @@
         if y_c <= 0 or y_c >= output_image.shape[0]:
             continue
 
         output_image[y_c, x_c, :] = [255, 0, 0]
 
     cv2.imwrite(output_file, output_image)
 
-@skip_pytest_in_runner_macos
+
 def test_overlay_liver_points(setup_vtk_overlay_window):
     """
 
     For local test, remember to uncomment `_pyside_qt_app.exec()` at the end of this module
     """
     output_name = 'tests/output/'
     if not os.path.exists(output_name):
```

### Comparing `scikit-surgeryvtk-2.0.1/tests/camera/test_vtk_camera_model.py` & `scikit-surgeryvtk-2.0rc0/tests/camera/test_vtk_camera_model.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.0.1/tests/models/test_surface_model_loader.py` & `scikit-surgeryvtk-2.0rc0/tests/models/test_surface_model_loader.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.0.1/tests/models/test_voxelise.py` & `scikit-surgeryvtk-2.0rc0/tests/models/test_voxelise.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.0.1/tests/models/test_vtk_cylinder_model.py` & `scikit-surgeryvtk-2.0rc0/tests/models/test_vtk_cylinder_model.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.0.1/tests/models/test_vtk_image_model.py` & `scikit-surgeryvtk-2.0rc0/tests/models/test_vtk_image_model.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.0.1/tests/models/test_vtk_point_model.py` & `scikit-surgeryvtk-2.0rc0/tests/models/test_vtk_point_model.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.0.1/tests/models/test_vtk_sphere_model.py` & `scikit-surgeryvtk-2.0rc0/tests/models/test_vtk_sphere_model.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.0.1/tests/models/test_vtk_surface_model.py` & `scikit-surgeryvtk-2.0rc0/tests/models/test_vtk_surface_model.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.0.1/tests/models/test_vtk_surface_model_directory_loader.py` & `scikit-surgeryvtk-2.0rc0/tests/models/test_vtk_surface_model_directory_loader.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.0.1/tests/models/test_vtk_unstructured_grid.py` & `scikit-surgeryvtk-2.0rc0/tests/models/test_vtk_unstructured_grid.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.0.1/tests/utils/test_matrix_utills.py` & `scikit-surgeryvtk-2.0rc0/tests/utils/test_matrix_utills.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.0.1/tests/utils/test_polydata_utils.py` & `scikit-surgeryvtk-2.0rc0/tests/utils/test_polydata_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.0.1/tests/utils/test_projection_utils.py` & `scikit-surgeryvtk-2.0rc0/tests/utils/test_projection_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.0.1/tests/widgets/test_interlaced_stereo_window.py` & `scikit-surgeryvtk-2.0rc0/tests/widgets/test_interlaced_stereo_window.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.0.1/tests/widgets/test_lus_simulator.py` & `scikit-surgeryvtk-2.0rc0/tests/widgets/test_lus_simulator.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.0.1/tests/widgets/test_rendering_generator.py` & `scikit-surgeryvtk-2.0rc0/tests/widgets/test_rendering_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,27 +5,28 @@
 
 import cv2
 import numpy as np
 import pytest
 
 import sksurgeryvtk.widgets.vtk_rendering_generator as rg
 
-# Shared skipif maker for all modules
+## Shared skipif maker for all modules
 skip_pytest_in_linux = pytest.mark.skipif(
     platform.system() == "Linux",
     reason=f'for [{platform.system()} OSs with CI=[{os.environ.get("CI")}] with RUNNER_OS=[{os.environ.get("RUNNER_OS")}] '
            f'{os.environ.get("SESSION_MANAGER")[0:20] if (platform.system() == "Linux" and os.environ.get("GITHUB_ACTIONS") == None) else ""} '
            f'with {os.environ.get("XDG_CURRENT_DESKTOP") if (platform.system() == "Linux" and os.environ.get("GITHUB_ACTIONS") == None) else ""} '
            f'due to issues with VTK pipelines and pyside workflows with Class Inheritance'
 )
 
 
 @skip_pytest_in_linux
 def test_basic_rendering_generator(setup_vtk_err):
     """
+
     For local test, remember to uncomment `_pyside_qt_app.exec()` at the end of this module
     """
     _vtk_std_err, _pyside_qt_app = setup_vtk_err
 
     if 'Linux' in platform.system():
         init_widget = False
     else:
```

### Comparing `scikit-surgeryvtk-2.0.1/tests/widgets/test_vtk_overlay_window.py` & `scikit-surgeryvtk-2.0rc0/tests/widgets/test_vtk_overlay_window.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.0.1/tests/widgets/test_vtk_overlay_window_with_outlines.py` & `scikit-surgeryvtk-2.0rc0/tests/widgets/test_vtk_overlay_window_with_outlines.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.0.1/tests/widgets/test_vtk_reslice.py` & `scikit-surgeryvtk-2.0rc0/tests/widgets/test_vtk_reslice.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryvtk-2.0.1/versioneer.py` & `scikit-surgeryvtk-2.0rc0/versioneer.py`

 * *Files identical despite different names*

