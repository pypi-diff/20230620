# Comparing `tmp/nvidia-dali-nightly-cuda120-1.28.0.dev20230614.tar.gz` & `tmp/nvidia-dali-nightly-cuda120-1.28.0.dev20230619.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvidia-dali-nightly-cuda120-1.28.0.dev20230614.tar", last modified: Wed Jun 14 16:44:39 2023, max compression
+gzip compressed data, was "nvidia-dali-nightly-cuda120-1.28.0.dev20230619.tar", last modified: Mon Jun 19 17:44:49 2023, max compression
```

## Comparing `nvidia-dali-nightly-cuda120-1.28.0.dev20230614.tar` & `nvidia-dali-nightly-cuda120-1.28.0.dev20230619.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-14 16:44:39.458159 nvidia-dali-nightly-cuda120-1.28.0.dev20230614/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      459 2023-06-14 16:44:39.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230614/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-06-14 04:38:44.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230614/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       27 2023-06-14 16:44:39.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230614/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-06-14 16:44:39.454159 nvidia-dali-nightly-cuda120-1.28.0.dev20230614/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      286 2023-06-14 16:44:39.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230614/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-14 16:44:39.454159 nvidia-dali-nightly-cuda120-1.28.0.dev20230614/nvidia_dali_nightly_cuda120.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-06-14 16:44:39.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230614/nvidia_dali_nightly_cuda120.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      257 2023-06-14 16:44:39.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230614/nvidia_dali_nightly_cuda120.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-06-14 16:44:39.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230614/nvidia_dali_nightly_cuda120.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-06-14 16:44:39.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230614/nvidia_dali_nightly_cuda120.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-06-14 16:44:39.458159 nvidia-dali-nightly-cuda120-1.28.0.dev20230614/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-06-14 04:38:44.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230614/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-19 17:44:49.454844 nvidia-dali-nightly-cuda120-1.28.0.dev20230619/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      459 2023-06-19 17:44:49.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230619/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-06-14 04:38:44.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230619/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       27 2023-06-19 17:44:49.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230619/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-06-19 17:44:49.454844 nvidia-dali-nightly-cuda120-1.28.0.dev20230619/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      286 2023-06-19 17:44:49.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230619/README.rst
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-19 17:44:49.454844 nvidia-dali-nightly-cuda120-1.28.0.dev20230619/nvidia_dali_nightly_cuda120.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-06-19 17:44:49.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230619/nvidia_dali_nightly_cuda120.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      257 2023-06-19 17:44:49.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230619/nvidia_dali_nightly_cuda120.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-06-19 17:44:49.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230619/nvidia_dali_nightly_cuda120.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-06-19 17:44:49.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230619/nvidia_dali_nightly_cuda120.egg-info/top_level.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-06-19 17:44:49.454844 nvidia-dali-nightly-cuda120-1.28.0.dev20230619/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-06-14 04:38:44.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230619/setup.py
```

### Comparing `nvidia-dali-nightly-cuda120-1.28.0.dev20230614/LICENSE.md` & `nvidia-dali-nightly-cuda120-1.28.0.dev20230619/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nvidia-dali-nightly-cuda120-1.28.0.dev20230614/PKG-INFO` & `nvidia-dali-nightly-cuda120-1.28.0.dev20230619/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-nightly-cuda120
-Version: 1.28.0.dev20230614
+Version: 1.28.0.dev20230619
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `nvidia-dali-nightly-cuda120-1.28.0.dev20230614/nvidia_dali_nightly_cuda120.egg-info/PKG-INFO` & `nvidia-dali-nightly-cuda120-1.28.0.dev20230619/nvidia_dali_nightly_cuda120.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-nightly-cuda120
-Version: 1.28.0.dev20230614
+Version: 1.28.0.dev20230619
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `nvidia-dali-nightly-cuda120-1.28.0.dev20230614/setup.py` & `nvidia-dali-nightly-cuda120-1.28.0.dev20230619/setup.py`

 * *Files identical despite different names*

