# Comparing `tmp/pybitset-0.0.1.dev1.tar.gz` & `tmp/pybitset-0.0.1.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybitset-0.0.1.dev1.tar", last modified: Sat Jun 17 14:46:08 2023, max compression
+gzip compressed data, was "pybitset-0.0.1.dev2.tar", last modified: Tue Jun 20 18:21:42 2023, max compression
```

## Comparing `pybitset-0.0.1.dev1.tar` & `pybitset-0.0.1.dev2.tar`

### file list

```diff
@@ -1,67 +1,56 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 14:46:08.645192 pybitset-0.0.1.dev1/
--rw-rw-rw-   0        0        0       83 2023-06-17 14:44:49.000000 pybitset-0.0.1.dev1/MANIFEST.in
--rw-rw-rw-   0        0        0     3506 2023-06-17 14:46:08.645192 pybitset-0.0.1.dev1/PKG-INFO
--rw-rw-rw-   0        0        0     2483 2023-06-17 14:40:10.000000 pybitset-0.0.1.dev1/README.markdown
-drwxrwxrwx   0        0        0        0 2023-06-17 14:46:08.615193 pybitset-0.0.1.dev1/cbitset/
--rw-rw-rw-   0        0        0       32 2023-06-15 14:23:28.000000 pybitset-0.0.1.dev1/cbitset/.git
-drwxrwxrwx   0        0        0        0 2023-06-17 14:46:08.603532 pybitset-0.0.1.dev1/cbitset/.github/
-drwxrwxrwx   0        0        0        0 2023-06-17 14:46:08.620186 pybitset-0.0.1.dev1/cbitset/.github/workflows/
--rw-rw-rw-   0        0        0     1305 2023-06-15 14:23:28.000000 pybitset-0.0.1.dev1/cbitset/.github/workflows/msys2.yml
--rw-rw-rw-   0        0        0      798 2023-06-15 14:23:28.000000 pybitset-0.0.1.dev1/cbitset/.github/workflows/ubuntu18.yml
--rw-rw-rw-   0        0        0      800 2023-06-15 14:23:28.000000 pybitset-0.0.1.dev1/cbitset/.github/workflows/ubuntu20.yml
--rw-rw-rw-   0        0        0      468 2023-06-15 14:23:28.000000 pybitset-0.0.1.dev1/cbitset/.github/workflows/vs16-arm-ci.yml
--rw-rw-rw-   0        0        0      748 2023-06-15 14:23:28.000000 pybitset-0.0.1.dev1/cbitset/.github/workflows/vs16-ci.yml
--rw-rw-rw-   0        0        0      787 2023-06-15 14:23:28.000000 pybitset-0.0.1.dev1/cbitset/.github/workflows/vs16-clang-ci.yml
--rw-rw-rw-   0        0        0      791 2023-06-15 14:23:28.000000 pybitset-0.0.1.dev1/cbitset/.github/workflows/vs16-ninja-ci.yml
--rw-rw-rw-   0        0        0      278 2023-06-15 14:23:28.000000 pybitset-0.0.1.dev1/cbitset/.gitignore
--rw-rw-rw-   0        0        0      119 2023-06-15 14:23:28.000000 pybitset-0.0.1.dev1/cbitset/.travis.yml
--rw-rw-rw-   0        0        0      453 2023-06-15 14:23:28.000000 pybitset-0.0.1.dev1/cbitset/CMakeLists.txt
--rw-rw-rw-   0        0        0    11558 2023-06-15 14:23:28.000000 pybitset-0.0.1.dev1/cbitset/LICENSE
--rw-rw-rw-   0        0        0      926 2023-06-15 14:23:28.000000 pybitset-0.0.1.dev1/cbitset/Makefile
--rw-rw-rw-   0        0        0     2168 2023-06-15 14:23:28.000000 pybitset-0.0.1.dev1/cbitset/README.md
-drwxrwxrwx   0        0        0        0 2023-06-17 14:46:08.623188 pybitset-0.0.1.dev1/cbitset/benchmarks/
--rw-rw-rw-   0        0        0      270 2023-06-15 14:23:28.000000 pybitset-0.0.1.dev1/cbitset/benchmarks/CMakeLists.txt
--rw-rw-rw-   0        0        0     2796 2023-06-15 14:23:28.000000 pybitset-0.0.1.dev1/cbitset/benchmarks/benchmark.c
--rw-rw-rw-   0        0        0     5635 2023-06-15 14:23:28.000000 pybitset-0.0.1.dev1/cbitset/benchmarks/lemirebenchmark.c
-drwxrwxrwx   0        0        0        0 2023-06-17 14:46:08.625187 pybitset-0.0.1.dev1/cbitset/include/
--rw-rw-rw-   0        0        0      306 2023-06-15 14:23:28.000000 pybitset-0.0.1.dev1/cbitset/include/CMakeLists.txt
--rw-rw-rw-   0        0        0     8756 2023-06-15 14:23:28.000000 pybitset-0.0.1.dev1/cbitset/include/bitset.h
--rw-rw-rw-   0        0        0     2928 2023-06-15 14:23:28.000000 pybitset-0.0.1.dev1/cbitset/include/portability.h
-drwxrwxrwx   0        0        0        0 2023-06-17 14:46:08.625187 pybitset-0.0.1.dev1/cbitset/src/
--rw-rw-rw-   0        0        0      190 2023-06-15 14:23:28.000000 pybitset-0.0.1.dev1/cbitset/src/CMakeLists.txt
--rw-rw-rw-   0        0        0    14695 2023-06-15 14:23:28.000000 pybitset-0.0.1.dev1/cbitset/src/bitset.c
-drwxrwxrwx   0        0        0        0 2023-06-17 14:46:08.627188 pybitset-0.0.1.dev1/cbitset/tests/
--rw-rw-rw-   0        0        0       97 2023-06-15 14:23:28.000000 pybitset-0.0.1.dev1/cbitset/tests/CMakeLists.txt
--rw-rw-rw-   0        0        0     7143 2023-06-15 14:23:28.000000 pybitset-0.0.1.dev1/cbitset/tests/unit.c
-drwxrwxrwx   0        0        0        0 2023-06-17 14:46:08.628189 pybitset-0.0.1.dev1/pybitset/
--rw-rw-rw-   0        0        0      148 2023-06-16 13:35:54.000000 pybitset-0.0.1.dev1/pybitset/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-17 14:46:08.634189 pybitset-0.0.1.dev1/pybitset/__pycache__/
--rw-rw-rw-   0        0        0      301 2023-06-15 16:16:44.000000 pybitset-0.0.1.dev1/pybitset/__pycache__/__init__.cpython-310.pyc
-drwxrwxrwx   0        0        0        0 2023-06-17 14:46:08.634189 pybitset-0.0.1.dev1/pybitset/backends/
--rw-rw-rw-   0        0        0      489 2023-06-16 13:35:54.000000 pybitset-0.0.1.dev1/pybitset/backends/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-17 14:46:08.635190 pybitset-0.0.1.dev1/pybitset/backends/__pycache__/
--rw-rw-rw-   0        0        0      593 2023-06-15 16:16:44.000000 pybitset-0.0.1.dev1/pybitset/backends/__pycache__/__init__.cpython-310.pyc
-drwxrwxrwx   0        0        0        0 2023-06-17 14:46:08.638191 pybitset-0.0.1.dev1/pybitset/backends/cffi/
--rw-rw-rw-   0        0        0     4571 2023-06-16 13:35:50.000000 pybitset-0.0.1.dev1/pybitset/backends/cffi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-17 14:46:08.639191 pybitset-0.0.1.dev1/pybitset/backends/cffi/__pycache__/
--rw-rw-rw-   0        0        0     7021 2023-06-16 05:12:22.000000 pybitset-0.0.1.dev1/pybitset/backends/cffi/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     6077 2023-06-16 05:12:22.000000 pybitset-0.0.1.dev1/pybitset/backends/cffi/__pycache__/build.cpython-310.pyc
--rw-rw-rw-   0        0        0    39936 2023-06-16 04:58:07.000000 pybitset-0.0.1.dev1/pybitset/backends/cffi/_bitset.pyd
--rw-rw-rw-   0        0        0     6165 2023-06-16 04:58:02.000000 pybitset-0.0.1.dev1/pybitset/backends/cffi/build.py
-drwxrwxrwx   0        0        0        0 2023-06-17 14:46:08.643192 pybitset-0.0.1.dev1/pybitset/backends/cython/
--rw-rw-rw-   0        0        0      134 2023-06-16 13:35:54.000000 pybitset-0.0.1.dev1/pybitset/backends/cython/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-17 14:46:08.644192 pybitset-0.0.1.dev1/pybitset/backends/cython/__pycache__/
--rw-rw-rw-   0        0        0      302 2023-06-15 16:16:44.000000 pybitset-0.0.1.dev1/pybitset/backends/cython/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0   387054 2023-06-17 14:45:02.000000 pybitset-0.0.1.dev1/pybitset/backends/cython/_bitset.c
--rw-rw-rw-   0        0        0    52224 2023-06-16 13:35:29.000000 pybitset-0.0.1.dev1/pybitset/backends/cython/_bitset.cp310-win_amd64.pyd
--rw-rw-rw-   0        0        0     7012 2023-06-16 13:35:50.000000 pybitset-0.0.1.dev1/pybitset/backends/cython/_bitset.pyx
--rw-rw-rw-   0        0        0     2708 2023-06-15 15:01:10.000000 pybitset-0.0.1.dev1/pybitset/backends/cython/bitset.pxd
-drwxrwxrwx   0        0        0        0 2023-06-17 14:46:08.632190 pybitset-0.0.1.dev1/pybitset.egg-info/
--rw-rw-rw-   0        0        0     3506 2023-06-17 14:46:08.000000 pybitset-0.0.1.dev1/pybitset.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1609 2023-06-17 14:46:08.000000 pybitset-0.0.1.dev1/pybitset.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 14:46:08.000000 pybitset-0.0.1.dev1/pybitset.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-17 14:45:02.000000 pybitset-0.0.1.dev1/pybitset.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2023-06-17 14:46:08.000000 pybitset-0.0.1.dev1/pybitset.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-17 14:46:08.000000 pybitset-0.0.1.dev1/pybitset.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-17 14:46:08.645192 pybitset-0.0.1.dev1/setup.cfg
--rw-rw-rw-   0        0        0     4175 2023-06-16 04:23:29.000000 pybitset-0.0.1.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:21:42.245546 pybitset-0.0.1.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-20 18:21:25.000000 pybitset-0.0.1.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-06-20 18:21:42.245546 pybitset-0.0.1.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-06-20 18:21:25.000000 pybitset-0.0.1.dev2/README.markdown
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:21:42.241546 pybitset-0.0.1.dev2/cbitset/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/.git
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:21:42.237546 pybitset-0.0.1.dev2/cbitset/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:21:42.241546 pybitset-0.0.1.dev2/cbitset/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/.github/workflows/msys2.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/.github/workflows/ubuntu18.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/.github/workflows/ubuntu20.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/.github/workflows/vs16-arm-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/.github/workflows/vs16-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/.github/workflows/vs16-clang-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/.github/workflows/vs16-ninja-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:21:42.241546 pybitset-0.0.1.dev2/cbitset/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/benchmarks/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/benchmarks/benchmark.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/benchmarks/lemirebenchmark.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:21:42.241546 pybitset-0.0.1.dev2/cbitset/include/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/include/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8500 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/include/bitset.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/include/portability.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:21:42.241546 pybitset-0.0.1.dev2/cbitset/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14273 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/src/bitset.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:21:42.241546 pybitset-0.0.1.dev2/cbitset/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6875 2023-06-20 18:21:26.000000 pybitset-0.0.1.dev2/cbitset/tests/unit.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:21:42.241546 pybitset-0.0.1.dev2/pybitset/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-20 18:21:25.000000 pybitset-0.0.1.dev2/pybitset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:21:42.245546 pybitset-0.0.1.dev2/pybitset/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-20 18:21:25.000000 pybitset-0.0.1.dev2/pybitset/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:21:42.245546 pybitset-0.0.1.dev2/pybitset/backends/cffi/
+-rw-r--r--   0 runner    (1001) docker     (123)     4529 2023-06-20 18:21:25.000000 pybitset-0.0.1.dev2/pybitset/backends/cffi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-06-20 18:21:25.000000 pybitset-0.0.1.dev2/pybitset/backends/cffi/build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:21:42.245546 pybitset-0.0.1.dev2/pybitset/backends/cython/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-20 18:21:25.000000 pybitset-0.0.1.dev2/pybitset/backends/cython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   389578 2023-06-20 18:21:25.000000 pybitset-0.0.1.dev2/pybitset/backends/cython/_bitset.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-06-20 18:21:25.000000 pybitset-0.0.1.dev2/pybitset/backends/cython/_bitset.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-20 18:21:25.000000 pybitset-0.0.1.dev2/pybitset/backends/cython/bitset.pxd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:21:42.245546 pybitset-0.0.1.dev2/pybitset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-06-20 18:21:42.000000 pybitset-0.0.1.dev2/pybitset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-20 18:21:42.000000 pybitset-0.0.1.dev2/pybitset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 18:21:42.000000 pybitset-0.0.1.dev2/pybitset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 18:21:42.000000 pybitset-0.0.1.dev2/pybitset.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-20 18:21:42.000000 pybitset-0.0.1.dev2/pybitset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 18:21:42.000000 pybitset-0.0.1.dev2/pybitset.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 18:21:42.245546 pybitset-0.0.1.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-06-20 18:21:25.000000 pybitset-0.0.1.dev2/setup.py
```

### Comparing `pybitset-0.0.1.dev1/PKG-INFO` & `pybitset-0.0.1.dev2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-Metadata-Version: 2.1
-Name: pybitset
-Version: 0.0.1.dev1
-Summary: python binding for cbitset
-Home-page: https://github.com/synodriver/pybitset
-Author: synodriver
-Author-email: diguohuangjiajinweijun@gmail.com
-License: BSD
-Keywords: bitset
-Classifier: Development Status :: 3 - Alpha
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Programming Language :: C
-Classifier: Programming Language :: Cython
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
-<h1 align="center"><i>✨ pybitset ✨ </i></h1>
-
-<h3 align="center">The python binding for <a href="https://github.com/lemire/cbitset">cbitset</a></h3>
-
-[![pypi](https://img.shields.io/pypi/v/pybitset.svg)](https://pypi.org/project/bzip3/)
-![python](https://img.shields.io/pypi/pyversions/pybitset)
-![implementation](https://img.shields.io/pypi/implementation/pybitset)
-![wheel](https://img.shields.io/pypi/wheel/pybitset)
-![license](https://img.shields.io/github/license/synodriver/pybitset.svg)
-![action](https://img.shields.io/github/workflow/status/synodriver/pybitset/build%20wheel)
-
-### install
-```bash
-pip install pybitset
-```
-
-
-### Usage
-```python
-from pybitset import BitSet
-
-b= BitSet()
-for i in range(1000):
-    b.set(3*i)
-
-for v in b:
-    print(v)
-```
-- use ```BITSET_USE_CFFI``` env var to specify a backend
-
-### Public functions
-```python
-class BitSet:
-    def __init__(self) -> None: ...
-    def __del__(self) -> None: ...
-    @staticmethod
-    def from_ptr(ptr) -> BitSet: ...
-    def clear(self) -> None: ...
-    def fill(self) -> None: ...
-    def copy(self) -> BitSet: ...
-    def resize(self, newarraysize: int, padwithzeroes: bool) -> bool: ...
-    def size_in_bytes(self) -> int: ...
-    def size_in_bits(self) -> int: ...
-    def size_in_words(self) -> int: ...
-    def grow(self, newarraysize: int) -> bool: ...
-    def trim(self) -> bool: ...
-    def shift_left(self, s: int) -> None: ...
-    def shift_right(self, s: int) -> None: ...
-    def set(self, i: int) -> None: ...
-    def set_to_value(self, i: int, flag: bool) -> None: ...
-    def get(self, i: int) -> bool: ...
-    def count(self) -> int: ...
-    def minimum(self) -> int: ...
-    def maximum(self) -> int: ...
-    def inplace_union(self, b2: BitSet) -> bool: ...
-    def union_count(self, b2: BitSet) -> int: ...
-    def inplace_intersection(self, b2: BitSet): ...
-    def intersection_count(self, b2: BitSet) -> int: ...
-    def disjoint(self, b2: BitSet) -> bool: ...
-    def intersect(self, b2: BitSet) -> bool: ...
-    def contains_all(self, b2: BitSet) -> bool: ...
-    def inplace_difference(self, b2: BitSet) -> None: ...
-    def difference_count(self, b2: BitSet) -> int: ...
-    def inplace_symmetric_difference(self, b2: BitSet) -> bool: ...
-    def symmetric_difference_count(self, b2: BitSet) -> int: ...
-    def __iter__(self): ...
-    def for_each(self, func) -> bool: ...
-    def print(self) -> None: ...
-
-```
+Metadata-Version: 2.1
+Name: pybitset
+Version: 0.0.1.dev2
+Summary: python binding for cbitset
+Home-page: https://github.com/synodriver/pybitset
+Author: synodriver
+Author-email: diguohuangjiajinweijun@gmail.com
+License: BSD
+Keywords: bitset
+Classifier: Development Status :: 3 - Alpha
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: Programming Language :: C
+Classifier: Programming Language :: Cython
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
+<h1 align="center"><i>✨ pybitset ✨ </i></h1>
+
+<h3 align="center">The python binding for <a href="https://github.com/lemire/cbitset">cbitset</a></h3>
+
+[![pypi](https://img.shields.io/pypi/v/pybitset.svg)](https://pypi.org/project/pybitset/)
+![python](https://img.shields.io/pypi/pyversions/pybitset)
+![implementation](https://img.shields.io/pypi/implementation/pybitset)
+![wheel](https://img.shields.io/pypi/wheel/pybitset)
+![license](https://img.shields.io/github/license/synodriver/pybitset.svg)
+![action](https://img.shields.io/github/workflow/status/synodriver/pybitset/build%20wheel)
+
+### install
+```bash
+pip install pybitset
+```
+
+
+### Usage
+```python
+from pybitset import BitSet
+
+b= BitSet()
+for i in range(1000):
+    b.set(3*i)
+
+for v in b:
+    print(v)
+```
+- use ```BITSET_USE_CFFI``` env var to specify a backend
+
+### Public functions
+```python
+class BitSet:
+    def __init__(self) -> None: ...
+    def __del__(self) -> None: ...
+    @staticmethod
+    def from_ptr(ptr) -> BitSet: ...
+    def clear(self) -> None: ...
+    def fill(self) -> None: ...
+    def copy(self) -> BitSet: ...
+    def resize(self, newarraysize: int, padwithzeroes: bool) -> bool: ...
+    def size_in_bytes(self) -> int: ...
+    def size_in_bits(self) -> int: ...
+    def size_in_words(self) -> int: ...
+    def grow(self, newarraysize: int) -> bool: ...
+    def trim(self) -> bool: ...
+    def shift_left(self, s: int) -> None: ...
+    def shift_right(self, s: int) -> None: ...
+    def set(self, i: int) -> None: ...
+    def set_to_value(self, i: int, flag: bool) -> None: ...
+    def get(self, i: int) -> bool: ...
+    def count(self) -> int: ...
+    def minimum(self) -> int: ...
+    def maximum(self) -> int: ...
+    def inplace_union(self, b2: BitSet) -> bool: ...
+    def union_count(self, b2: BitSet) -> int: ...
+    def inplace_intersection(self, b2: BitSet): ...
+    def intersection_count(self, b2: BitSet) -> int: ...
+    def disjoint(self, b2: BitSet) -> bool: ...
+    def intersect(self, b2: BitSet) -> bool: ...
+    def contains_all(self, b2: BitSet) -> bool: ...
+    def inplace_difference(self, b2: BitSet) -> None: ...
+    def difference_count(self, b2: BitSet) -> int: ...
+    def inplace_symmetric_difference(self, b2: BitSet) -> bool: ...
+    def symmetric_difference_count(self, b2: BitSet) -> int: ...
+    def __iter__(self): ...
+    def for_each(self, func) -> bool: ...
+    def print(self) -> None: ...
+
+```
```

### Comparing `pybitset-0.0.1.dev1/README.markdown` & `pybitset-0.0.1.dev2/README.markdown`

 * *Files 10% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-<h1 align="center"><i>✨ pybitset ✨ </i></h1>
-
-<h3 align="center">The python binding for <a href="https://github.com/lemire/cbitset">cbitset</a></h3>
-
-[![pypi](https://img.shields.io/pypi/v/pybitset.svg)](https://pypi.org/project/bzip3/)
-![python](https://img.shields.io/pypi/pyversions/pybitset)
-![implementation](https://img.shields.io/pypi/implementation/pybitset)
-![wheel](https://img.shields.io/pypi/wheel/pybitset)
-![license](https://img.shields.io/github/license/synodriver/pybitset.svg)
-![action](https://img.shields.io/github/workflow/status/synodriver/pybitset/build%20wheel)
-
-### install
-```bash
-pip install pybitset
-```
-
-
-### Usage
-```python
-from pybitset import BitSet
-
-b= BitSet()
-for i in range(1000):
-    b.set(3*i)
-
-for v in b:
-    print(v)
-```
-- use ```BITSET_USE_CFFI``` env var to specify a backend
-
-### Public functions
-```python
-class BitSet:
-    def __init__(self) -> None: ...
-    def __del__(self) -> None: ...
-    @staticmethod
-    def from_ptr(ptr) -> BitSet: ...
-    def clear(self) -> None: ...
-    def fill(self) -> None: ...
-    def copy(self) -> BitSet: ...
-    def resize(self, newarraysize: int, padwithzeroes: bool) -> bool: ...
-    def size_in_bytes(self) -> int: ...
-    def size_in_bits(self) -> int: ...
-    def size_in_words(self) -> int: ...
-    def grow(self, newarraysize: int) -> bool: ...
-    def trim(self) -> bool: ...
-    def shift_left(self, s: int) -> None: ...
-    def shift_right(self, s: int) -> None: ...
-    def set(self, i: int) -> None: ...
-    def set_to_value(self, i: int, flag: bool) -> None: ...
-    def get(self, i: int) -> bool: ...
-    def count(self) -> int: ...
-    def minimum(self) -> int: ...
-    def maximum(self) -> int: ...
-    def inplace_union(self, b2: BitSet) -> bool: ...
-    def union_count(self, b2: BitSet) -> int: ...
-    def inplace_intersection(self, b2: BitSet): ...
-    def intersection_count(self, b2: BitSet) -> int: ...
-    def disjoint(self, b2: BitSet) -> bool: ...
-    def intersect(self, b2: BitSet) -> bool: ...
-    def contains_all(self, b2: BitSet) -> bool: ...
-    def inplace_difference(self, b2: BitSet) -> None: ...
-    def difference_count(self, b2: BitSet) -> int: ...
-    def inplace_symmetric_difference(self, b2: BitSet) -> bool: ...
-    def symmetric_difference_count(self, b2: BitSet) -> int: ...
-    def __iter__(self): ...
-    def for_each(self, func) -> bool: ...
-    def print(self) -> None: ...
-
+<h1 align="center"><i>✨ pybitset ✨ </i></h1>
+
+<h3 align="center">The python binding for <a href="https://github.com/lemire/cbitset">cbitset</a></h3>
+
+[![pypi](https://img.shields.io/pypi/v/pybitset.svg)](https://pypi.org/project/pybitset/)
+![python](https://img.shields.io/pypi/pyversions/pybitset)
+![implementation](https://img.shields.io/pypi/implementation/pybitset)
+![wheel](https://img.shields.io/pypi/wheel/pybitset)
+![license](https://img.shields.io/github/license/synodriver/pybitset.svg)
+![action](https://img.shields.io/github/workflow/status/synodriver/pybitset/build%20wheel)
+
+### install
+```bash
+pip install pybitset
+```
+
+
+### Usage
+```python
+from pybitset import BitSet
+
+b= BitSet()
+for i in range(1000):
+    b.set(3*i)
+
+for v in b:
+    print(v)
+```
+- use ```BITSET_USE_CFFI``` env var to specify a backend
+
+### Public functions
+```python
+class BitSet:
+    def __init__(self) -> None: ...
+    def __del__(self) -> None: ...
+    @staticmethod
+    def from_ptr(ptr) -> BitSet: ...
+    def clear(self) -> None: ...
+    def fill(self) -> None: ...
+    def copy(self) -> BitSet: ...
+    def resize(self, newarraysize: int, padwithzeroes: bool) -> bool: ...
+    def size_in_bytes(self) -> int: ...
+    def size_in_bits(self) -> int: ...
+    def size_in_words(self) -> int: ...
+    def grow(self, newarraysize: int) -> bool: ...
+    def trim(self) -> bool: ...
+    def shift_left(self, s: int) -> None: ...
+    def shift_right(self, s: int) -> None: ...
+    def set(self, i: int) -> None: ...
+    def set_to_value(self, i: int, flag: bool) -> None: ...
+    def get(self, i: int) -> bool: ...
+    def count(self) -> int: ...
+    def minimum(self) -> int: ...
+    def maximum(self) -> int: ...
+    def inplace_union(self, b2: BitSet) -> bool: ...
+    def union_count(self, b2: BitSet) -> int: ...
+    def inplace_intersection(self, b2: BitSet): ...
+    def intersection_count(self, b2: BitSet) -> int: ...
+    def disjoint(self, b2: BitSet) -> bool: ...
+    def intersect(self, b2: BitSet) -> bool: ...
+    def contains_all(self, b2: BitSet) -> bool: ...
+    def inplace_difference(self, b2: BitSet) -> None: ...
+    def difference_count(self, b2: BitSet) -> int: ...
+    def inplace_symmetric_difference(self, b2: BitSet) -> bool: ...
+    def symmetric_difference_count(self, b2: BitSet) -> int: ...
+    def __iter__(self): ...
+    def for_each(self, func) -> bool: ...
+    def print(self) -> None: ...
+
 ```
```

### Comparing `pybitset-0.0.1.dev1/cbitset/.github/workflows/msys2.yml` & `pybitset-0.0.1.dev2/cbitset/.github/workflows/msys2.yml`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-name: MSYS2-CI
-
-on: [push, pull_request]
-
-jobs:
-  windows-mingw:
-    name: ${{ matrix.msystem }}
-    runs-on: windows-latest
-    defaults:
-      run:
-        shell: msys2 {0}
-    strategy:
-      fail-fast: false
-      matrix:
-        include:
-          - msystem: "MINGW64"
-            install: mingw-w64-x86_64-cmake mingw-w64-x86_64-ninja mingw-w64-x86_64-gcc
-            type: Release
-          - msystem: "MINGW32"
-            install: mingw-w64-i686-cmake mingw-w64-i686-ninja mingw-w64-i686-gcc
-            type: Release
-          - msystem: "MINGW64"
-            install: mingw-w64-x86_64-cmake mingw-w64-x86_64-ninja mingw-w64-x86_64-gcc
-            type: Debug
-          - msystem: "MINGW32"
-            install: mingw-w64-i686-cmake mingw-w64-i686-ninja mingw-w64-i686-gcc
-            type: Debug
-    env:
-      CMAKE_GENERATOR: Ninja
-
-    steps:
-      - uses: actions/checkout@v2
-      - uses: msys2/setup-msys2@v2
-        with:
-          update: true
-          msystem: ${{ matrix.msystem }}
-          install: ${{ matrix.install }}
-      - name: Build and Test
-        run: |
-          mkdir build
-          cd build
-          cmake -DCMAKE_BUILD_TYPE=${{ matrix.type }} ..
-          cmake --build . --verbose
+name: MSYS2-CI
+
+on: [push, pull_request]
+
+jobs:
+  windows-mingw:
+    name: ${{ matrix.msystem }}
+    runs-on: windows-latest
+    defaults:
+      run:
+        shell: msys2 {0}
+    strategy:
+      fail-fast: false
+      matrix:
+        include:
+          - msystem: "MINGW64"
+            install: mingw-w64-x86_64-cmake mingw-w64-x86_64-ninja mingw-w64-x86_64-gcc
+            type: Release
+          - msystem: "MINGW32"
+            install: mingw-w64-i686-cmake mingw-w64-i686-ninja mingw-w64-i686-gcc
+            type: Release
+          - msystem: "MINGW64"
+            install: mingw-w64-x86_64-cmake mingw-w64-x86_64-ninja mingw-w64-x86_64-gcc
+            type: Debug
+          - msystem: "MINGW32"
+            install: mingw-w64-i686-cmake mingw-w64-i686-ninja mingw-w64-i686-gcc
+            type: Debug
+    env:
+      CMAKE_GENERATOR: Ninja
+
+    steps:
+      - uses: actions/checkout@v2
+      - uses: msys2/setup-msys2@v2
+        with:
+          update: true
+          msystem: ${{ matrix.msystem }}
+          install: ${{ matrix.install }}
+      - name: Build and Test
+        run: |
+          mkdir build
+          cd build
+          cmake -DCMAKE_BUILD_TYPE=${{ matrix.type }} ..
+          cmake --build . --verbose
           ctest -j4 --output-on-failure
```

### Comparing `pybitset-0.0.1.dev1/cbitset/.github/workflows/ubuntu18.yml` & `pybitset-0.0.1.dev2/cbitset/.github/workflows/ubuntu20.yml`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-name: Ubuntu 18.04 CI (GCC 7)
-
-on: [push, pull_request]
-
-jobs:
-  ubuntu-build:
-    runs-on: ubuntu-18.04
-    steps:
-      - uses: actions/checkout@v2
-      - name: Setup cmake
-        uses: jwlawson/actions-setup-cmake@v1.9
-      - name: Use cmake
-        run: |
-          mkdir build &&
-          cd build &&
-          cmake  -DCMAKE_INSTALL_PREFIX:PATH=destination ..  &&
-          cmake --build .   &&
-          ctest -j --output-on-failure  &&
-          make install  &&
-          echo -e '#include <cbitset/bitset.h>\nint main(int argc,char**argv) {bitset_t * b = bitset_create(); bitset_set(b,10); bitset_get(b,10); bitset_free(b); }' > tmp.c && cc -Idestination/include -Ldestination/lib -std=c11 -Wl,-rpath,destination/lib -o linkandrun tmp.c -lcbitset && ./linkandrun 
+name: Ubuntu 20.04 CI (GCC 9)
+
+on: [push, pull_request]
+
+jobs:
+  ubuntu-build:
+    runs-on: ubuntu-20.04
+    steps:
+      - uses: actions/checkout@v2
+      - name: Setup cmake
+        uses: jwlawson/actions-setup-cmake@v1.9
+      - name: Use cmake
+        run: |
+          mkdir build &&
+          cd build &&
+          cmake  -DCMAKE_INSTALL_PREFIX:PATH=destination ..  &&
+          cmake --build .   &&
+          ctest -j --output-on-failure  &&
+          make install  &&
+          echo -e '#include <cbitset/bitset.h>\nint main(int argc,char**argv) {bitset_t * b = bitset_create(); bitset_set(b,10); bitset_get(b,10); bitset_free(b); }' > tmp.c && cc  -Idestination/include  -Ldestination/lib -std=c11 -Wl,-rpath,destination/lib -o linkandrun tmp.c -lcbitset && ./linkandrun
```

### Comparing `pybitset-0.0.1.dev1/cbitset/.github/workflows/vs16-ci.yml` & `pybitset-0.0.1.dev2/cbitset/.github/workflows/vs16-ninja-ci.yml`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-name: VS16-CI
-
-on: [push, pull_request]
-
-jobs:
-  ci:
-    name: windows-vs16
-    runs-on: windows-latest
-    steps:
-    - uses: actions/checkout@v2
-    - name: 'Run CMake with VS16'
-      uses: lukka/run-cmake@v2
-      with:
-        cmakeListsOrSettingsJson: CMakeListsTxtAdvanced
-        cmakeListsTxtPath: '${{ github.workspace }}/CMakeLists.txt'
-        buildDirectory: "${{ github.workspace }}/../../_temp/windows"
-        cmakeBuildType: Release   
-        buildWithCMake: true
-        cmakeGenerator: VS16Win64 
-        buildWithCMakeArgs: --config Release  
-        
-    - name: 'Run CTest'
-      run: ctest -C Release    --output-on-failure 
-      working-directory: "${{ github.workspace }}/../../_temp/windows"
-  
+name: VS16-Ninja-CI
+
+on: [push, pull_request]
+
+jobs:
+  ci:
+    name: windows-vs16
+    runs-on: windows-latest
+    steps:
+    - uses: actions/checkout@v2
+    - name: 'Run CMake with VS16'
+      uses: lukka/run-cmake@v2
+      with:
+        cmakeListsOrSettingsJson: CMakeListsTxtAdvanced
+        cmakeListsTxtPath: '${{ github.workspace }}/CMakeLists.txt'
+        buildDirectory: "${{ github.workspace }}/../../_temp/windows"
+        cmakeBuildType: Release   
+        buildWithCMake: true
+        cmakeGenerator: VS16Win64 
+        cmakeAppendedArgs:  -G Ninja
+        buildWithCMakeArgs: --config Release  
+        
+    - name: 'Run CTest'
+      run: ctest -C Release   --output-on-failure 
+      working-directory: "${{ github.workspace }}/../../_temp/windows"
+
```

### Comparing `pybitset-0.0.1.dev1/cbitset/.github/workflows/vs16-clang-ci.yml` & `pybitset-0.0.1.dev2/cbitset/.github/workflows/vs16-clang-ci.yml`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-name: VS16-CLANG-CI
-
-on: [push, pull_request]
-
-jobs:
-  ci:
-    name: windows-vs16
-    runs-on: windows-latest
-    steps:
-    - uses: actions/checkout@v2
-    - name: 'Run CMake with VS16'
-      uses: lukka/run-cmake@v2
-      with:
-        cmakeListsOrSettingsJson: CMakeListsTxtAdvanced
-        cmakeListsTxtPath: '${{ github.workspace }}/CMakeLists.txt'
-        buildDirectory: "${{ github.workspace }}/../../_temp/windows"
-        cmakeBuildType: Release   
-        buildWithCMake: true
-        cmakeGenerator: VS16Win64 
-        cmakeAppendedArgs:  -T ClangCL
-        buildWithCMakeArgs: --config Release  
-        
-    - name: 'Run CTest'
-      run: ctest -C Release   --output-on-failure 
+name: VS16-CLANG-CI
+
+on: [push, pull_request]
+
+jobs:
+  ci:
+    name: windows-vs16
+    runs-on: windows-latest
+    steps:
+    - uses: actions/checkout@v2
+    - name: 'Run CMake with VS16'
+      uses: lukka/run-cmake@v2
+      with:
+        cmakeListsOrSettingsJson: CMakeListsTxtAdvanced
+        cmakeListsTxtPath: '${{ github.workspace }}/CMakeLists.txt'
+        buildDirectory: "${{ github.workspace }}/../../_temp/windows"
+        cmakeBuildType: Release   
+        buildWithCMake: true
+        cmakeGenerator: VS16Win64 
+        cmakeAppendedArgs:  -T ClangCL
+        buildWithCMakeArgs: --config Release  
+        
+    - name: 'Run CTest'
+      run: ctest -C Release   --output-on-failure 
       working-directory: "${{ github.workspace }}/../../_temp/windows"
```

### Comparing `pybitset-0.0.1.dev1/cbitset/LICENSE` & `pybitset-0.0.1.dev2/cbitset/LICENSE`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "{}"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright {yyyy} {name of copyright owner}
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "{}"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright {yyyy} {name of copyright owner}
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `pybitset-0.0.1.dev1/cbitset/Makefile` & `pybitset-0.0.1.dev2/cbitset/Makefile`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-# minimalist makefile
-.SUFFIXES:
-#
-.SUFFIXES: .cpp .o .c .h
-ifeq ($(DEBUG),1)
-CFLAGS = -fPIC  -std=c99 -ggdb -Wall -Wextra -Wshadow -fsanitize=undefined  -fno-omit-frame-pointer -fsanitize=address
-else
-CFLAGS = -fPIC -std=c99 -O3  -Wall -Wextra -Wshadow
-endif # debug
-OBJECTS=bitset.o
-all: unit benchmark lemirebenchmark $(OBJECTS)
-HEADERS=./include/bitset.h ./include/portability.h
-
-bitset.o: ./src/bitset.c $(HEADERS)
-	$(CC) $(CFLAGS) -c ./src/bitset.c -Iinclude
-
-unit: bitset.o ./tests/unit.c $(HEADERS)
-	$(CC) $(CFLAGS) -o unit ./tests/unit.c bitset.o -Iinclude
-
-lemirebenchmark: bitset.o ./benchmarks/lemirebenchmark.c $(HEADERS)
-	$(CC) $(CFLAGS) -o lemirebenchmark ./benchmarks/lemirebenchmark.c bitset.o -Iinclude
-benchmark: bitset.o ./benchmarks/benchmark.c $(HEADERS)
-	$(CC) $(CFLAGS) -o benchmark ./benchmarks/benchmark.c bitset.o -Iinclude
-clean:
-	rm -f  *.o unit benchmark lemirebenchmark
+# minimalist makefile
+.SUFFIXES:
+#
+.SUFFIXES: .cpp .o .c .h
+ifeq ($(DEBUG),1)
+CFLAGS = -fPIC  -std=c99 -ggdb -Wall -Wextra -Wshadow -fsanitize=undefined  -fno-omit-frame-pointer -fsanitize=address
+else
+CFLAGS = -fPIC -std=c99 -O3  -Wall -Wextra -Wshadow
+endif # debug
+OBJECTS=bitset.o
+all: unit benchmark lemirebenchmark $(OBJECTS)
+HEADERS=./include/bitset.h ./include/portability.h
+
+bitset.o: ./src/bitset.c $(HEADERS)
+	$(CC) $(CFLAGS) -c ./src/bitset.c -Iinclude
+
+unit: bitset.o ./tests/unit.c $(HEADERS)
+	$(CC) $(CFLAGS) -o unit ./tests/unit.c bitset.o -Iinclude
+
+lemirebenchmark: bitset.o ./benchmarks/lemirebenchmark.c $(HEADERS)
+	$(CC) $(CFLAGS) -o lemirebenchmark ./benchmarks/lemirebenchmark.c bitset.o -Iinclude
+benchmark: bitset.o ./benchmarks/benchmark.c $(HEADERS)
+	$(CC) $(CFLAGS) -o benchmark ./benchmarks/benchmark.c bitset.o -Iinclude
+clean:
+	rm -f  *.o unit benchmark lemirebenchmark
```

### Comparing `pybitset-0.0.1.dev1/cbitset/README.md` & `pybitset-0.0.1.dev2/cbitset/README.md`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-# cbitset
-[![Build Status](https://travis-ci.org/lemire/cbitset.png)](https://travis-ci.org/lemire/cbitset)
-![Ubuntu 20.04 CI (GCC 9)](https://github.com/lemire/cbitset/workflows/Ubuntu%2020.04%20CI%20(GCC%209)/badge.svg)
-![Ubuntu 18.04 CI (GCC 7)](https://github.com/lemire/cbitset/workflows/Ubuntu%2018.04%20CI%20(GCC%207)/badge.svg)
-![MSYS2-CI](https://github.com/lemire/cbitset/workflows/MSYS2-CI/badge.svg)
-![Visual Studio-CI](https://github.com/lemire/cbitset/workflows/VS16-CI/badge.svg)
-
-Simple bitset library in C. It includes fast functions
-to compute cardinalities, unions, intersections...
-
-- It is tiny: it is made of three files (two header files and one source file).
-- It is tested.
-- It is fast.
-- It is straight C.
-
-Usage in C:
-```C
-bitset_t * b = bitset_create();
-bitset_set(b,10);
-bitset_get(b,10);// returns true
-bitset_free(b); // frees memory
-```
-
-Advanced example:
-
-
-```C
-    bitset_t *b = bitset_create();
-    for (int k = 0; k < 1000; ++k) {
-        bitset_set(b, 3 * k);
-    }
-    // We have bitset_count(b) == 1000.
-    // We have bitset_get(b, 3) is true
-    // You can iterate through the values:
-    size_t k = 0;
-    for (size_t i = 0; bitset_next_set_bit(b, &i); i++) {
-        // You will have i == k
-        k += 3;
-    }
-    // We support a wide range of operations on two bitsets such as
-    // bitset_inplace_symmetric_difference(b1,b2);
-    // bitset_inplace_symmetric_difference(b1,b2);
-    // bitset_inplace_difference(b1,b2);// should make no difference
-    // bitset_inplace_union(b1,b2);
-    // bitset_inplace_intersection(b1,b2);
-    // bitsets_disjoint
-    // bitsets_intersect
-```
-
-## CMake
-
-```
-mkdir build
-cd build
-cmake ..
-cmake --build . --config Release  
-ctest .
-```
-
-The cmake build also supports installation. The header files will be installed in a distinct subdirectory (cbitset).
-
-
-## Old-school Makefiles
-
-To run tests:
-```bash
-make
-./unit
-```
-
-## Prerequisites
-
-C11-compatible compiler.
-
-Visual Studio now supports the [C11 and C17 standards](https://devblogs.microsoft.com/cppblog/c11-and-c17-standard-support-arriving-in-msvc/).
-
+# cbitset
+[![Build Status](https://travis-ci.org/lemire/cbitset.png)](https://travis-ci.org/lemire/cbitset)
+![Ubuntu 20.04 CI (GCC 9)](https://github.com/lemire/cbitset/workflows/Ubuntu%2020.04%20CI%20(GCC%209)/badge.svg)
+![Ubuntu 18.04 CI (GCC 7)](https://github.com/lemire/cbitset/workflows/Ubuntu%2018.04%20CI%20(GCC%207)/badge.svg)
+![MSYS2-CI](https://github.com/lemire/cbitset/workflows/MSYS2-CI/badge.svg)
+![Visual Studio-CI](https://github.com/lemire/cbitset/workflows/VS16-CI/badge.svg)
+
+Simple bitset library in C. It includes fast functions
+to compute cardinalities, unions, intersections...
+
+- It is tiny: it is made of three files (two header files and one source file).
+- It is tested.
+- It is fast.
+- It is straight C.
+
+Usage in C:
+```C
+bitset_t * b = bitset_create();
+bitset_set(b,10);
+bitset_get(b,10);// returns true
+bitset_free(b); // frees memory
+```
+
+Advanced example:
+
+
+```C
+    bitset_t *b = bitset_create();
+    for (int k = 0; k < 1000; ++k) {
+        bitset_set(b, 3 * k);
+    }
+    // We have bitset_count(b) == 1000.
+    // We have bitset_get(b, 3) is true
+    // You can iterate through the values:
+    size_t k = 0;
+    for (size_t i = 0; bitset_next_set_bit(b, &i); i++) {
+        // You will have i == k
+        k += 3;
+    }
+    // We support a wide range of operations on two bitsets such as
+    // bitset_inplace_symmetric_difference(b1,b2);
+    // bitset_inplace_symmetric_difference(b1,b2);
+    // bitset_inplace_difference(b1,b2);// should make no difference
+    // bitset_inplace_union(b1,b2);
+    // bitset_inplace_intersection(b1,b2);
+    // bitsets_disjoint
+    // bitsets_intersect
+```
+
+## CMake
+
+```
+mkdir build
+cd build
+cmake ..
+cmake --build . --config Release  
+ctest .
+```
+
+The cmake build also supports installation. The header files will be installed in a distinct subdirectory (cbitset).
+
+
+## Old-school Makefiles
+
+To run tests:
+```bash
+make
+./unit
+```
+
+## Prerequisites
+
+C11-compatible compiler.
+
+Visual Studio now supports the [C11 and C17 standards](https://devblogs.microsoft.com/cppblog/c11-and-c17-standard-support-arriving-in-msvc/).
+
```

### Comparing `pybitset-0.0.1.dev1/cbitset/benchmarks/lemirebenchmark.c` & `pybitset-0.0.1.dev2/cbitset/benchmarks/lemirebenchmark.c`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,148 +1,148 @@
-#include "bitset.h"
-#include <assert.h>
-#include <stdio.h>
-#include <stdlib.h>
-#include <sys/time.h>
-
-#define BEST_TIME(test, repeat)                                                \
-  do {                                                                         \
-    printf("%s: ", #test);                                                     \
-    fflush(NULL);                                                              \
-    static struct timeval tm1, tm2;                                            \
-    uint64_t min_diff = (uint64_t)-1;                                          \
-    for (int i = 0; i < repeat; i++) {                                         \
-      __asm volatile("" ::: /* pretend to clobber */ "memory");                \
-      gettimeofday(&tm1, NULL);                                                \
-      test;                                                                    \
-      gettimeofday(&tm2, NULL);                                                \
-      uint64_t tmus = 1000 * 1000 * (tm2.tv_sec - tm1.tv_sec) +                \
-                      (tm2.tv_usec - tm1.tv_usec);                             \
-      if (tmus < min_diff)                                                     \
-        min_diff = tmus;                                                       \
-    }                                                                          \
-    printf(" %f ms", min_diff / 1000.0);                                       \
-    printf("\n");                                                              \
-    fflush(NULL);                                                              \
-  } while (0)
-
-#define BEST_TIME_CHECK(test, check, repeat)                                   \
-  do {                                                                         \
-    printf("%s: ", #test);                                                     \
-    fflush(NULL);                                                              \
-    static struct timeval tm1, tm2;                                            \
-    uint64_t min_diff = (uint64_t)-1;                                          \
-    for (int i = 0; i < repeat; i++) {                                         \
-      __asm volatile("" ::: /* pretend to clobber */ "memory");                \
-      gettimeofday(&tm1, NULL);                                                \
-      if (test != check)                                                       \
-        printf("bug");                                                         \
-      gettimeofday(&tm2, NULL);                                                \
-      uint64_t tmus = 1000 * 1000 * (tm2.tv_sec - tm1.tv_sec) +                \
-                      (tm2.tv_usec - tm1.tv_usec);                             \
-      if (tmus < min_diff)                                                     \
-        min_diff = tmus;                                                       \
-    }                                                                          \
-    printf(" %f ms", min_diff / 1000.0);                                       \
-    printf("\n");                                                              \
-    fflush(NULL);                                                              \
-  } while (0)
-
-void create() {
-  bitset_t *b1 = bitset_create();
-  for (uint32_t k = 0; k < 100000000; k += 100) {
-    bitset_set(b1, k);
-  }
-  bitset_free(b1);
-}
-
-size_t iterate(bitset_t *b1) {
-  size_t sum = 0;
-  for (size_t i = 0; nextSetBit(b1, &i); i++) {
-    sum++;
-  }
-  return sum;
-}
-
-size_t iterateb(bitset_t *b1) {
-  size_t sum = 0;
-  for (size_t i = 0; nextSetBit(b1, &i); i++) {
-    sum += i;
-  }
-  return sum;
-}
-
-bool incr(size_t value, void *param) {
-  (void)value;
-  size_t sum;
-  memcpy(&sum, param, sizeof(size_t));
-  sum++;
-  memcpy(param, &sum, sizeof(size_t));
-  return true;
-}
-
-size_t iterate2(bitset_t *b1) {
-  size_t sum = 0;
-  bitset_for_each(b1, incr, &sum);
-  return sum;
-}
-
-bool incrb(size_t value, void *param) {
-  size_t sum;
-  memcpy(&sum, param, sizeof(size_t));
-  sum += value;
-  memcpy(param, &sum, sizeof(size_t));
-  return true;
-}
-
-size_t iterate2b(bitset_t *b1) {
-  size_t sum = 0;
-  bitset_for_each(b1, incrb, &sum);
-  return sum;
-}
-
-size_t iterate3(bitset_t *b1) {
-  size_t sum = 0;
-  size_t buffer[256];
-  size_t howmany = 0;
-  for (size_t startfrom = 0;
-       (howmany = nextSetBits(b1, buffer, 256, &startfrom)) > 0; startfrom++) {
-    for (size_t i = 0; i < howmany; i++) {
-      sum++;
-    }
-  }
-  return sum;
-}
-size_t iterate3b(bitset_t *b1) {
-  size_t sum = 0;
-  size_t buffer[256];
-  size_t howmany = 0;
-  for (size_t startfrom = 0;
-       (howmany = nextSetBits(b1, buffer, 256, &startfrom)) > 0; startfrom++) {
-    for (size_t i = 0; i < howmany; i++) {
-      sum += buffer[i];
-    }
-  }
-  return sum;
-}
-
-int main() {
-  int repeat = 10;
-  BEST_TIME(create(), repeat);
-  bitset_t *b1 = bitset_create();
-  size_t count = 0;
-  for (uint32_t k = 0; k < 100000000; k += 100) {
-    bitset_set(b1, k);
-    ++count;
-  }
-  assert(bitset_count(b1) == iterate(b1));
-  BEST_TIME_CHECK(bitset_count(b1), count, repeat);
-  BEST_TIME_CHECK(iterate(b1), count, repeat);
-  BEST_TIME_CHECK(iterate2(b1), count, repeat);
-  BEST_TIME_CHECK(iterate3(b1), count, repeat);
-  size_t expected = iterate3b(b1);
-  BEST_TIME_CHECK(iterateb(b1), expected, repeat);
-  BEST_TIME_CHECK(iterate2b(b1), expected, repeat);
-  BEST_TIME_CHECK(iterate3b(b1), expected, repeat);
-
-  bitset_free(b1);
-}
+#include "bitset.h"
+#include <assert.h>
+#include <stdio.h>
+#include <stdlib.h>
+#include <sys/time.h>
+
+#define BEST_TIME(test, repeat)                                                \
+  do {                                                                         \
+    printf("%s: ", #test);                                                     \
+    fflush(NULL);                                                              \
+    static struct timeval tm1, tm2;                                            \
+    uint64_t min_diff = (uint64_t)-1;                                          \
+    for (int i = 0; i < repeat; i++) {                                         \
+      __asm volatile("" ::: /* pretend to clobber */ "memory");                \
+      gettimeofday(&tm1, NULL);                                                \
+      test;                                                                    \
+      gettimeofday(&tm2, NULL);                                                \
+      uint64_t tmus = 1000 * 1000 * (tm2.tv_sec - tm1.tv_sec) +                \
+                      (tm2.tv_usec - tm1.tv_usec);                             \
+      if (tmus < min_diff)                                                     \
+        min_diff = tmus;                                                       \
+    }                                                                          \
+    printf(" %f ms", min_diff / 1000.0);                                       \
+    printf("\n");                                                              \
+    fflush(NULL);                                                              \
+  } while (0)
+
+#define BEST_TIME_CHECK(test, check, repeat)                                   \
+  do {                                                                         \
+    printf("%s: ", #test);                                                     \
+    fflush(NULL);                                                              \
+    static struct timeval tm1, tm2;                                            \
+    uint64_t min_diff = (uint64_t)-1;                                          \
+    for (int i = 0; i < repeat; i++) {                                         \
+      __asm volatile("" ::: /* pretend to clobber */ "memory");                \
+      gettimeofday(&tm1, NULL);                                                \
+      if (test != check)                                                       \
+        printf("bug");                                                         \
+      gettimeofday(&tm2, NULL);                                                \
+      uint64_t tmus = 1000 * 1000 * (tm2.tv_sec - tm1.tv_sec) +                \
+                      (tm2.tv_usec - tm1.tv_usec);                             \
+      if (tmus < min_diff)                                                     \
+        min_diff = tmus;                                                       \
+    }                                                                          \
+    printf(" %f ms", min_diff / 1000.0);                                       \
+    printf("\n");                                                              \
+    fflush(NULL);                                                              \
+  } while (0)
+
+void create() {
+  bitset_t *b1 = bitset_create();
+  for (uint32_t k = 0; k < 100000000; k += 100) {
+    bitset_set(b1, k);
+  }
+  bitset_free(b1);
+}
+
+size_t iterate(bitset_t *b1) {
+  size_t sum = 0;
+  for (size_t i = 0; nextSetBit(b1, &i); i++) {
+    sum++;
+  }
+  return sum;
+}
+
+size_t iterateb(bitset_t *b1) {
+  size_t sum = 0;
+  for (size_t i = 0; nextSetBit(b1, &i); i++) {
+    sum += i;
+  }
+  return sum;
+}
+
+bool incr(size_t value, void *param) {
+  (void)value;
+  size_t sum;
+  memcpy(&sum, param, sizeof(size_t));
+  sum++;
+  memcpy(param, &sum, sizeof(size_t));
+  return true;
+}
+
+size_t iterate2(bitset_t *b1) {
+  size_t sum = 0;
+  bitset_for_each(b1, incr, &sum);
+  return sum;
+}
+
+bool incrb(size_t value, void *param) {
+  size_t sum;
+  memcpy(&sum, param, sizeof(size_t));
+  sum += value;
+  memcpy(param, &sum, sizeof(size_t));
+  return true;
+}
+
+size_t iterate2b(bitset_t *b1) {
+  size_t sum = 0;
+  bitset_for_each(b1, incrb, &sum);
+  return sum;
+}
+
+size_t iterate3(bitset_t *b1) {
+  size_t sum = 0;
+  size_t buffer[256];
+  size_t howmany = 0;
+  for (size_t startfrom = 0;
+       (howmany = nextSetBits(b1, buffer, 256, &startfrom)) > 0; startfrom++) {
+    for (size_t i = 0; i < howmany; i++) {
+      sum++;
+    }
+  }
+  return sum;
+}
+size_t iterate3b(bitset_t *b1) {
+  size_t sum = 0;
+  size_t buffer[256];
+  size_t howmany = 0;
+  for (size_t startfrom = 0;
+       (howmany = nextSetBits(b1, buffer, 256, &startfrom)) > 0; startfrom++) {
+    for (size_t i = 0; i < howmany; i++) {
+      sum += buffer[i];
+    }
+  }
+  return sum;
+}
+
+int main() {
+  int repeat = 10;
+  BEST_TIME(create(), repeat);
+  bitset_t *b1 = bitset_create();
+  size_t count = 0;
+  for (uint32_t k = 0; k < 100000000; k += 100) {
+    bitset_set(b1, k);
+    ++count;
+  }
+  assert(bitset_count(b1) == iterate(b1));
+  BEST_TIME_CHECK(bitset_count(b1), count, repeat);
+  BEST_TIME_CHECK(iterate(b1), count, repeat);
+  BEST_TIME_CHECK(iterate2(b1), count, repeat);
+  BEST_TIME_CHECK(iterate3(b1), count, repeat);
+  size_t expected = iterate3b(b1);
+  BEST_TIME_CHECK(iterateb(b1), expected, repeat);
+  BEST_TIME_CHECK(iterate2b(b1), expected, repeat);
+  BEST_TIME_CHECK(iterate3b(b1), expected, repeat);
+
+  bitset_free(b1);
+}
```

### Comparing `pybitset-0.0.1.dev1/cbitset/include/bitset.h` & `pybitset-0.0.1.dev2/cbitset/include/bitset.h`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,256 +1,256 @@
-#ifndef BITSET_H
-#define BITSET_H
-#include <stdio.h>
-#include <stdlib.h>
-#include <stdint.h>
-#include <stdbool.h>
-#include <stdio.h>
-#include <string.h>
-
-#include "portability.h"
-
-struct bitset_s {
-    uint64_t * CBITSET_RESTRICT array;
-    /* For simplicity and performance, we prefer to have a size and a capacity that is a multiple of 64 bits.
-     * Thus we only track the size and the capacity in terms of 64-bit words allocated */
-    size_t arraysize;
-    size_t capacity;
-
-};
-
-typedef struct bitset_s bitset_t;
-
-/* Create a new bitset. Return NULL in case of failure. */
-bitset_t *bitset_create( void );
-
-/* Create a new bitset able to contain size bits. Return NULL in case of failure. */
-bitset_t *bitset_create_with_capacity( size_t size );
-
-/* Free memory. */
-void bitset_free(bitset_t *bitset);
-
-/* Set all bits to zero. */
-void bitset_clear(bitset_t *bitset);
-
-/* Set all bits to one. */
-void bitset_fill(bitset_t *bitset);
-
-/* Create a copy */
-bitset_t * bitset_copy(const bitset_t *bitset);
-
-/* For advanced users: Resize the bitset so that it can support newarraysize * 64 bits.
- * Return true in case of success, false for failure. Pad
- * with zeroes new buffer areas if requested. */
-bool bitset_resize( bitset_t *bitset,  size_t newarraysize, bool padwithzeroes );
-
-/* returns how many bytes of memory the backend buffer uses */
-inline size_t bitset_size_in_bytes(const bitset_t *bitset) {
-  return bitset->arraysize*sizeof(uint64_t);
-}
-
-/* returns how many bits can be accessed */
-inline size_t bitset_size_in_bits(const bitset_t *bitset) {
-  return bitset->arraysize * 64;
-}
-
-/* returns how many words (64-bit) of memory the backend buffer uses */
-inline size_t bitset_size_in_words(const bitset_t *bitset) {
-  return bitset->arraysize;
-}
-
-
-/* For advanced users: Grow the bitset so that it can support newarraysize * 64 bits with padding. Return true in case of success, false for failure. */
-bool bitset_grow(bitset_t *bitset,  size_t newarraysize);
-
-/* attempts to recover unused memory, return false in case of reallocation failure */
-bool bitset_trim(bitset_t *bitset);
-
-/* shifts all bits by 's' positions so that the bitset representing values 1,2,10 would represent values 1+s, 2+s, 10+s */
-void bitset_shift_left(bitset_t *bitset, size_t s);
-
-/* shifts all bits by 's' positions so that the bitset representing values 1,2,10 would represent values 1-s, 2-s, 10-s, negative values are deleted */
-void bitset_shift_right(bitset_t *bitset, size_t s);
-
-/* Set the ith bit. Attempts to resize the bitset if needed (may silently fail) */
-inline void bitset_set(bitset_t *bitset,  size_t i) {
-  size_t shiftedi = i / 64;
-  if (shiftedi >= bitset->arraysize) {
-    if( ! bitset_grow(bitset,  shiftedi + 1) ) {
-        return;
-    }
-  }
-  bitset->array[shiftedi] |= ((uint64_t)1) << (i % 64);
-}
-
-/* Set the ith bit to the specified value. Attempts to resize the bitset if needed (may silently fail) */
-inline void bitset_set_to_value(bitset_t *bitset,  size_t i, bool flag) {
-  size_t shiftedi = i / 64;
-  uint64_t mask = ((uint64_t)1) << (i % 64);
-  uint64_t dynmask = ((uint64_t)flag) << (i % 64);
-  if (shiftedi >= bitset->arraysize) {
-    if( ! bitset_grow(bitset,  shiftedi + 1) ) {
-        return;
-    }
-  }
-  uint64_t w = bitset->array[shiftedi];
-  w &= ~mask;
-  w |= dynmask; 
-  bitset->array[shiftedi] = w;
-}
-
-
-
-
-/* Get the value of the ith bit.  */
-inline bool bitset_get(const bitset_t *bitset,  size_t i ) {
-  size_t shiftedi = i / 64;
-  if (shiftedi >= bitset->arraysize) {
-    return false;
-  }
-  return ( bitset->array[shiftedi] & ( ((uint64_t)1) << (i % 64))) != 0 ;
-}
-
-/* Count number of bits set.  */
-size_t bitset_count(const bitset_t *bitset);
-
-/* Find the index of the first bit set. Or zero if the bitset is empty.  */
-size_t bitset_minimum(const bitset_t *bitset);
-
-/* Find the index of the last bit set. Or zero if the bitset is empty. */
-size_t bitset_maximum(const bitset_t *bitset);
-
-
-/* compute the union in-place (to b1), returns true if successful, to generate a new bitset first call bitset_copy */
-bool bitset_inplace_union(bitset_t * CBITSET_RESTRICT b1, const bitset_t * CBITSET_RESTRICT b2);
-
-/* report the size of the union (without materializing it) */
-size_t bitset_union_count(const bitset_t * CBITSET_RESTRICT b1, const bitset_t * CBITSET_RESTRICT b2);
-
-/* compute the intersection in-place (to b1), to generate a new bitset first call bitset_copy */
-void bitset_inplace_intersection(bitset_t * CBITSET_RESTRICT b1, const bitset_t * CBITSET_RESTRICT b2);
-
-/* Report the size of the intersection (without materializing it).
- * We assume that the bitsets b1 and b2 are distinct. */
-size_t bitset_intersection_count(const bitset_t * CBITSET_RESTRICT b1, const bitset_t * CBITSET_RESTRICT b2);
-
-
-/* returns true if the bitsets contain no common elements */
-bool bitsets_disjoint(const bitset_t * CBITSET_RESTRICT b1, const bitset_t * CBITSET_RESTRICT b2);
-
-/* returns true if the bitsets contain any common elements */
-bool bitsets_intersect(const bitset_t * CBITSET_RESTRICT b1, const bitset_t * CBITSET_RESTRICT b2);
-
-/* returns true if b1 contains all of the set bits of b2 */
-bool bitset_contains_all(const bitset_t * CBITSET_RESTRICT b1, const bitset_t * CBITSET_RESTRICT b2);
-
-
-/* compute the difference in-place (to b1), to generate a new bitset first call bitset_copy */
-void bitset_inplace_difference(bitset_t * CBITSET_RESTRICT b1, const bitset_t * CBITSET_RESTRICT b2);
-
-/* compute the size of the difference */
-size_t  bitset_difference_count(const bitset_t * CBITSET_RESTRICT b1, const bitset_t * CBITSET_RESTRICT b2) ;
-
-/* compute the symmetric difference in-place (to b1), return true if successful, to generate a new bitset first call bitset_copy */
-bool bitset_inplace_symmetric_difference(bitset_t * CBITSET_RESTRICT b1, const bitset_t * CBITSET_RESTRICT b2);
-
-/* compute the size of the symmetric difference  */
-size_t  bitset_symmetric_difference_count(const bitset_t * CBITSET_RESTRICT b1, const bitset_t * CBITSET_RESTRICT b2);
-
-/* iterate over the set bits
- like so :
-  for(size_t i = 0; bitset_next_set_bit(b,&i) ; i++) {
-    //.....
-  }
-  */
-inline bool bitset_next_set_bit(const bitset_t *bitset, size_t *i) {
-      size_t x = *i / 64;
-      if (x >= bitset->arraysize) {
-        return false;
-      }
-      uint64_t w = bitset->array[x];
-      w >>= (*i & 63);
-      if (w != 0) {
-        *i += cbitset_trailing_zeroes(w);
-        return true;
-      }
-      x ++;
-      while (x < bitset->arraysize) {
-        w = bitset->array[x];
-        if (w != 0) {
-          *i = x * 64 + cbitset_trailing_zeroes(w);
-          return true;
-        }
-        x ++;
-      }
-      return false;
-}
-
-/* iterate over the set bits
- like so :
-   size_t buffer[256];
-   size_t howmany = 0;
-  for(size_t startfrom = 0; (howmany = bitset_next_set_bits(b,buffer,256, &startfrom)) > 0 ; startfrom++) {
-    //.....
-  }
-  */
-inline size_t bitset_next_set_bits(const bitset_t *bitset, size_t *buffer, size_t capacity, size_t * startfrom) {
-      if(capacity == 0) return 0;// sanity check
-      size_t x = *startfrom / 64;
-      if (x >= bitset->arraysize) {
-          return 0;// nothing more to iterate over
-      }
-      uint64_t w = bitset->array[x];
-      w >>= (*startfrom & 63);
-      size_t howmany = 0;
-      size_t base = x << 6;
-      while(howmany < capacity) {
-            while (w != 0) {
-              uint64_t t = w & (~w + 1);
-              int r = cbitset_trailing_zeroes(w);
-              buffer[howmany++] = r + base;
-              if(howmany == capacity) goto end;
-              w ^= t;
-            }
-            x += 1;
-            if(x == bitset->arraysize) {
-              break;
-            }
-            base += 64;
-            w = bitset->array[x];
-      }
-      end:
-      if(howmany > 0) {
-        *startfrom = buffer[howmany - 1];
-      }
-      return howmany;
-}
-
-typedef bool (*bitset_iterator)(size_t value, void *param);
-
-// return true if uninterrupted
-inline bool bitset_for_each(const bitset_t *b, bitset_iterator iterator, void *ptr) {
-  size_t base = 0;
-  for (size_t i = 0; i < b->arraysize; ++i ) {
-    uint64_t w = b->array[i];
-    while (w != 0) {
-      uint64_t t = w & (~w + 1);
-      int r = cbitset_trailing_zeroes(w);
-      if(!iterator(r + base, ptr)) return false;
-      w ^= t;
-    }
-    base += 64;
-  }
-  return true;
-}
-
-inline void bitset_print(const bitset_t *b) {
-  printf("{");
-  for(size_t i = 0; bitset_next_set_bit(b,&i) ; i++) {
-    printf("%zu, ",i);
-  }
-  printf("}");
-}
-
-
-
-#endif
+#ifndef BITSET_H
+#define BITSET_H
+#include <stdio.h>
+#include <stdlib.h>
+#include <stdint.h>
+#include <stdbool.h>
+#include <stdio.h>
+#include <string.h>
+
+#include "portability.h"
+
+struct bitset_s {
+    uint64_t * CBITSET_RESTRICT array;
+    /* For simplicity and performance, we prefer to have a size and a capacity that is a multiple of 64 bits.
+     * Thus we only track the size and the capacity in terms of 64-bit words allocated */
+    size_t arraysize;
+    size_t capacity;
+
+};
+
+typedef struct bitset_s bitset_t;
+
+/* Create a new bitset. Return NULL in case of failure. */
+bitset_t *bitset_create( void );
+
+/* Create a new bitset able to contain size bits. Return NULL in case of failure. */
+bitset_t *bitset_create_with_capacity( size_t size );
+
+/* Free memory. */
+void bitset_free(bitset_t *bitset);
+
+/* Set all bits to zero. */
+void bitset_clear(bitset_t *bitset);
+
+/* Set all bits to one. */
+void bitset_fill(bitset_t *bitset);
+
+/* Create a copy */
+bitset_t * bitset_copy(const bitset_t *bitset);
+
+/* For advanced users: Resize the bitset so that it can support newarraysize * 64 bits.
+ * Return true in case of success, false for failure. Pad
+ * with zeroes new buffer areas if requested. */
+bool bitset_resize( bitset_t *bitset,  size_t newarraysize, bool padwithzeroes );
+
+/* returns how many bytes of memory the backend buffer uses */
+inline size_t bitset_size_in_bytes(const bitset_t *bitset) {
+  return bitset->arraysize*sizeof(uint64_t);
+}
+
+/* returns how many bits can be accessed */
+inline size_t bitset_size_in_bits(const bitset_t *bitset) {
+  return bitset->arraysize * 64;
+}
+
+/* returns how many words (64-bit) of memory the backend buffer uses */
+inline size_t bitset_size_in_words(const bitset_t *bitset) {
+  return bitset->arraysize;
+}
+
+
+/* For advanced users: Grow the bitset so that it can support newarraysize * 64 bits with padding. Return true in case of success, false for failure. */
+bool bitset_grow(bitset_t *bitset,  size_t newarraysize);
+
+/* attempts to recover unused memory, return false in case of reallocation failure */
+bool bitset_trim(bitset_t *bitset);
+
+/* shifts all bits by 's' positions so that the bitset representing values 1,2,10 would represent values 1+s, 2+s, 10+s */
+void bitset_shift_left(bitset_t *bitset, size_t s);
+
+/* shifts all bits by 's' positions so that the bitset representing values 1,2,10 would represent values 1-s, 2-s, 10-s, negative values are deleted */
+void bitset_shift_right(bitset_t *bitset, size_t s);
+
+/* Set the ith bit. Attempts to resize the bitset if needed (may silently fail) */
+inline void bitset_set(bitset_t *bitset,  size_t i) {
+  size_t shiftedi = i / 64;
+  if (shiftedi >= bitset->arraysize) {
+    if( ! bitset_grow(bitset,  shiftedi + 1) ) {
+        return;
+    }
+  }
+  bitset->array[shiftedi] |= ((uint64_t)1) << (i % 64);
+}
+
+/* Set the ith bit to the specified value. Attempts to resize the bitset if needed (may silently fail) */
+inline void bitset_set_to_value(bitset_t *bitset,  size_t i, bool flag) {
+  size_t shiftedi = i / 64;
+  uint64_t mask = ((uint64_t)1) << (i % 64);
+  uint64_t dynmask = ((uint64_t)flag) << (i % 64);
+  if (shiftedi >= bitset->arraysize) {
+    if( ! bitset_grow(bitset,  shiftedi + 1) ) {
+        return;
+    }
+  }
+  uint64_t w = bitset->array[shiftedi];
+  w &= ~mask;
+  w |= dynmask; 
+  bitset->array[shiftedi] = w;
+}
+
+
+
+
+/* Get the value of the ith bit.  */
+inline bool bitset_get(const bitset_t *bitset,  size_t i ) {
+  size_t shiftedi = i / 64;
+  if (shiftedi >= bitset->arraysize) {
+    return false;
+  }
+  return ( bitset->array[shiftedi] & ( ((uint64_t)1) << (i % 64))) != 0 ;
+}
+
+/* Count number of bits set.  */
+size_t bitset_count(const bitset_t *bitset);
+
+/* Find the index of the first bit set. Or zero if the bitset is empty.  */
+size_t bitset_minimum(const bitset_t *bitset);
+
+/* Find the index of the last bit set. Or zero if the bitset is empty. */
+size_t bitset_maximum(const bitset_t *bitset);
+
+
+/* compute the union in-place (to b1), returns true if successful, to generate a new bitset first call bitset_copy */
+bool bitset_inplace_union(bitset_t * CBITSET_RESTRICT b1, const bitset_t * CBITSET_RESTRICT b2);
+
+/* report the size of the union (without materializing it) */
+size_t bitset_union_count(const bitset_t * CBITSET_RESTRICT b1, const bitset_t * CBITSET_RESTRICT b2);
+
+/* compute the intersection in-place (to b1), to generate a new bitset first call bitset_copy */
+void bitset_inplace_intersection(bitset_t * CBITSET_RESTRICT b1, const bitset_t * CBITSET_RESTRICT b2);
+
+/* Report the size of the intersection (without materializing it).
+ * We assume that the bitsets b1 and b2 are distinct. */
+size_t bitset_intersection_count(const bitset_t * CBITSET_RESTRICT b1, const bitset_t * CBITSET_RESTRICT b2);
+
+
+/* returns true if the bitsets contain no common elements */
+bool bitsets_disjoint(const bitset_t * CBITSET_RESTRICT b1, const bitset_t * CBITSET_RESTRICT b2);
+
+/* returns true if the bitsets contain any common elements */
+bool bitsets_intersect(const bitset_t * CBITSET_RESTRICT b1, const bitset_t * CBITSET_RESTRICT b2);
+
+/* returns true if b1 contains all of the set bits of b2 */
+bool bitset_contains_all(const bitset_t * CBITSET_RESTRICT b1, const bitset_t * CBITSET_RESTRICT b2);
+
+
+/* compute the difference in-place (to b1), to generate a new bitset first call bitset_copy */
+void bitset_inplace_difference(bitset_t * CBITSET_RESTRICT b1, const bitset_t * CBITSET_RESTRICT b2);
+
+/* compute the size of the difference */
+size_t  bitset_difference_count(const bitset_t * CBITSET_RESTRICT b1, const bitset_t * CBITSET_RESTRICT b2) ;
+
+/* compute the symmetric difference in-place (to b1), return true if successful, to generate a new bitset first call bitset_copy */
+bool bitset_inplace_symmetric_difference(bitset_t * CBITSET_RESTRICT b1, const bitset_t * CBITSET_RESTRICT b2);
+
+/* compute the size of the symmetric difference  */
+size_t  bitset_symmetric_difference_count(const bitset_t * CBITSET_RESTRICT b1, const bitset_t * CBITSET_RESTRICT b2);
+
+/* iterate over the set bits
+ like so :
+  for(size_t i = 0; bitset_next_set_bit(b,&i) ; i++) {
+    //.....
+  }
+  */
+inline bool bitset_next_set_bit(const bitset_t *bitset, size_t *i) {
+      size_t x = *i / 64;
+      if (x >= bitset->arraysize) {
+        return false;
+      }
+      uint64_t w = bitset->array[x];
+      w >>= (*i & 63);
+      if (w != 0) {
+        *i += cbitset_trailing_zeroes(w);
+        return true;
+      }
+      x ++;
+      while (x < bitset->arraysize) {
+        w = bitset->array[x];
+        if (w != 0) {
+          *i = x * 64 + cbitset_trailing_zeroes(w);
+          return true;
+        }
+        x ++;
+      }
+      return false;
+}
+
+/* iterate over the set bits
+ like so :
+   size_t buffer[256];
+   size_t howmany = 0;
+  for(size_t startfrom = 0; (howmany = bitset_next_set_bits(b,buffer,256, &startfrom)) > 0 ; startfrom++) {
+    //.....
+  }
+  */
+inline size_t bitset_next_set_bits(const bitset_t *bitset, size_t *buffer, size_t capacity, size_t * startfrom) {
+      if(capacity == 0) return 0;// sanity check
+      size_t x = *startfrom / 64;
+      if (x >= bitset->arraysize) {
+          return 0;// nothing more to iterate over
+      }
+      uint64_t w = bitset->array[x];
+      w >>= (*startfrom & 63);
+      size_t howmany = 0;
+      size_t base = x << 6;
+      while(howmany < capacity) {
+            while (w != 0) {
+              uint64_t t = w & (~w + 1);
+              int r = cbitset_trailing_zeroes(w);
+              buffer[howmany++] = r + base;
+              if(howmany == capacity) goto end;
+              w ^= t;
+            }
+            x += 1;
+            if(x == bitset->arraysize) {
+              break;
+            }
+            base += 64;
+            w = bitset->array[x];
+      }
+      end:
+      if(howmany > 0) {
+        *startfrom = buffer[howmany - 1];
+      }
+      return howmany;
+}
+
+typedef bool (*bitset_iterator)(size_t value, void *param);
+
+// return true if uninterrupted
+inline bool bitset_for_each(const bitset_t *b, bitset_iterator iterator, void *ptr) {
+  size_t base = 0;
+  for (size_t i = 0; i < b->arraysize; ++i ) {
+    uint64_t w = b->array[i];
+    while (w != 0) {
+      uint64_t t = w & (~w + 1);
+      int r = cbitset_trailing_zeroes(w);
+      if(!iterator(r + base, ptr)) return false;
+      w ^= t;
+    }
+    base += 64;
+  }
+  return true;
+}
+
+inline void bitset_print(const bitset_t *b) {
+  printf("{");
+  for(size_t i = 0; bitset_next_set_bit(b,&i) ; i++) {
+    printf("%zu, ",i);
+  }
+  printf("}");
+}
+
+
+
+#endif
```

### Comparing `pybitset-0.0.1.dev1/cbitset/src/bitset.c` & `pybitset-0.0.1.dev2/cbitset/src/bitset.c`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,422 +1,422 @@
-#include <stdlib.h>
-#include <stdio.h>
-#include <limits.h>
-#include <stdint.h>
-#include <string.h>
-
-#include "bitset.h"
-extern inline void bitset_print(const bitset_t *b);
-extern inline bool bitset_for_each(const bitset_t *b, bitset_iterator iterator,
-                                   void *ptr);
-extern inline size_t bitset_next_set_bits(const bitset_t *bitset, size_t *buffer,
-                                 size_t capacity, size_t *startfrom);
-extern inline void bitset_set_to_value(bitset_t *bitset, size_t i, bool flag);
-extern inline bool bitset_next_set_bit(const bitset_t *bitset, size_t *i);
-extern inline void bitset_set(bitset_t *bitset, size_t i);
-extern inline bool bitset_get(const bitset_t *bitset, size_t i);
-extern inline size_t bitset_size_in_words(const bitset_t *bitset);
-extern inline size_t bitset_size_in_bits(const bitset_t *bitset);
-extern inline size_t bitset_size_in_bytes(const bitset_t *bitset);
-
-/* Create a new bitset. Return NULL in case of failure. */
-bitset_t *bitset_create() {
-  bitset_t *bitset = NULL;
-  /* Allocate the bitset itself. */
-  if( ( bitset = (bitset_t*) malloc( sizeof( bitset_t ) ) ) == NULL ) {
-      return NULL;
-  }
-  bitset->array = NULL;
-  bitset->arraysize = 0;
-  bitset->capacity = 0;
-  return bitset;
-}
-
-/* Create a new bitset able to contain size bits. Return NULL in case of failure. */
-bitset_t *bitset_create_with_capacity( size_t size ) {
-  bitset_t *bitset = NULL;
-  /* Allocate the bitset itself. */
-  if( ( bitset = (bitset_t*) malloc( sizeof( bitset_t ) ) ) == NULL ) {
-      return NULL;
-  }
-  bitset->arraysize = (size + sizeof(uint64_t) * 8 - 1) / (sizeof(uint64_t) * 8);
-  bitset->capacity = bitset->arraysize;
-  if ((bitset->array = (uint64_t *) calloc(bitset->arraysize, sizeof(uint64_t))) == NULL) {
-    free(bitset);
-    return NULL;
-  }
-  return bitset;
-}
-
-/* Create a copy */
-bitset_t *bitset_copy( const bitset_t * bitset ) {
-  bitset_t *copy = NULL;
-  /* Allocate the bitset itself. */
-  if( ( copy = (bitset_t*) malloc( sizeof( bitset_t ) ) ) == NULL ) {
-      return NULL;
-  }
-  memcpy(copy, bitset, sizeof(bitset_t));
-  copy->capacity = copy->arraysize;
-  if ((copy->array = (uint64_t *) malloc(sizeof(uint64_t) * bitset->arraysize)) == NULL) {
-    free(copy);
-    return NULL;
-  }
-  memcpy(copy->array,bitset->array,sizeof(uint64_t) * bitset->arraysize);
-  return copy;
-}
-
-void bitset_clear(bitset_t *bitset) {
-  memset(bitset->array,0,sizeof(uint64_t) * bitset->arraysize);
-}
-
-void bitset_fill(bitset_t *bitset) {
-  memset(bitset->array,0xff,sizeof(uint64_t) * bitset->arraysize);
-}
-
-
-void bitset_shift_left(bitset_t *bitset, size_t s) {
-  size_t extra_words = s / 64;
-  int inword_shift = s % 64;
-  size_t as = bitset->arraysize;
-  if(inword_shift == 0) {
-    bitset_resize(bitset,as + extra_words, false);
-    // could be done with a memmove
-    for(size_t i = as + extra_words ; i > extra_words; i--) {
-      bitset->array[i - 1] = bitset->array[i - 1 - extra_words];
-    }
-  } else {
-    bitset_resize(bitset,as + extra_words + 1, true);
-    bitset->array[as + extra_words] =
-     bitset->array[as - 1] >> (64 - inword_shift);
-    for(size_t i = as + extra_words ; i >= extra_words + 2; i--) {
-      bitset->array[i - 1] = (bitset->array[i - 1 - extra_words] << inword_shift)
-      | (bitset->array[i - 2 - extra_words]>>(64 - inword_shift));
-    }
-    bitset->array[extra_words] = bitset->array[0] <<  inword_shift;
-  }
-  for(size_t i = 0; i < extra_words; i++) {
-    bitset->array[i] = 0;
-  }
-}
-
-
-void bitset_shift_right(bitset_t *bitset, size_t s) {
-  size_t extra_words = s / 64;
-  int inword_shift = s % 64;
-  size_t as = bitset->arraysize;
-  if(inword_shift == 0) {
-    // could be done with a memmove
-    for(size_t i = 0 ; i < as - extra_words; i++) {
-      bitset->array[i] = bitset->array[i + extra_words];
-    }
-    bitset_resize(bitset,as - extra_words, false);
-
-  } else {
-    for(size_t i = 0 ; i + extra_words + 1 < as ; i++) {
-      bitset->array[i] = (bitset->array[i + extra_words] >> inword_shift)
-      | (bitset->array[i + extra_words + 1] << (64 - inword_shift));
-    }
-    bitset->array[as - extra_words - 1] = (bitset->array[as - 1] >> inword_shift);
-    bitset_resize(bitset,as - extra_words , false);
-  }
-}
-
-/* Free memory. */
-void bitset_free(bitset_t *bitset) {
-  free(bitset->array);
-  free(bitset);
-}
-
-bool bitset_grow(bitset_t *bitset,  size_t newarraysize) {
-  if(newarraysize < bitset->arraysize) { return false; }
-  if(newarraysize > SIZE_MAX/64) { return false; }
-  if (bitset->capacity < newarraysize) {
-    uint64_t *newarray;
-    size_t newcapacity = bitset->capacity;
-    if(newcapacity == 0) { newcapacity = 1; }
-    while(newcapacity < newarraysize) { newcapacity *= 2; }
-    if ((newarray = (uint64_t *) realloc(bitset->array, sizeof(uint64_t) * newcapacity)) == NULL) {
-      return false;
-    }
-    bitset->capacity = newcapacity;
-    bitset->array = newarray;
-  }
-  memset(bitset->array + bitset->arraysize, 0, sizeof(uint64_t) * (newarraysize - bitset->arraysize));
-  bitset->arraysize = newarraysize;
-  return true; // success!
-}
-/* Resize the bitset so that it can support newarraysize * 64 bits. Return true in case of success, false for failure. */
-bool bitset_resize(bitset_t *bitset,  size_t newarraysize, bool padwithzeroes) {
-  if(newarraysize > SIZE_MAX/64) { return false; }
-  size_t smallest = newarraysize < bitset->arraysize ? newarraysize : bitset->arraysize;
-  if (bitset->capacity < newarraysize) {
-    uint64_t *newarray;
-    size_t newcapacity = (UINT64_C(0xFFFFFFFFFFFFFFFF) >> cbitset_leading_zeroes(newarraysize)) + 1;
-    if ((newarray = (uint64_t *) realloc(bitset->array, sizeof(uint64_t) * newcapacity)) == NULL) {
-      return false;
-    }
-    bitset->capacity = newcapacity;
-    bitset->array = newarray;
-  }
-  if (padwithzeroes && (newarraysize > smallest)) {
-    memset(bitset->array + smallest,0,sizeof(uint64_t) * (newarraysize - smallest));
-  }
-  bitset->arraysize = newarraysize;
-  return true; // success!
-}
-
-
-
-size_t bitset_count(const bitset_t *bitset) {
-    size_t card = 0;
-    size_t k = 0;
-    for(; k + 7 < bitset->arraysize; k+=8) {
-        card += cbitset_hamming(bitset->array[k]);
-        card += cbitset_hamming(bitset->array[k+1]);
-        card += cbitset_hamming(bitset->array[k+2]);
-        card += cbitset_hamming(bitset->array[k+3]);
-        card += cbitset_hamming(bitset->array[k+4]);
-        card += cbitset_hamming(bitset->array[k+5]);
-        card += cbitset_hamming(bitset->array[k+6]);
-        card += cbitset_hamming(bitset->array[k+7]);
-    }
-    for(; k + 3 < bitset->arraysize; k+=4) {
-        card += cbitset_hamming(bitset->array[k]);
-        card += cbitset_hamming(bitset->array[k+1]);
-        card += cbitset_hamming(bitset->array[k+2]);
-        card += cbitset_hamming(bitset->array[k+3]);
-    }
-    for(; k < bitset->arraysize; k++) {
-        card += cbitset_hamming(bitset->array[k]);
-    }
-    return card;
-}
-
-
-bool bitset_inplace_union(bitset_t * CBITSET_RESTRICT b1, const bitset_t * CBITSET_RESTRICT b2) {
-  size_t minlength = b1->arraysize < b2->arraysize ? b1->arraysize : b2->arraysize;
-  for(size_t k = 0 ; k < minlength; ++k) {
-    b1->array[k] |= b2->array[k];
-  }
-  if(b2->arraysize > b1->arraysize) {
-     size_t oldsize = b1->arraysize;
-     if(!bitset_resize( b1, b2->arraysize, false)) return false;
-     memcpy(b1->array + oldsize, b2->array + oldsize, (b2->arraysize - oldsize) * sizeof(uint64_t));
-  }
-  return true;
-}
-
-size_t bitset_minimum(const bitset_t *bitset) {
-  for(size_t k = 0; k < bitset->arraysize; k++) {
-    uint64_t w = bitset->array[k];
-    if ( w != 0 ) {
-      return cbitset_trailing_zeroes(w) + k * 64;
-    }
-  }
-  return 0;
-}
-
-size_t bitset_maximum(const bitset_t *bitset) {
-  for(size_t k = bitset->arraysize ; k > 0 ; k--) {
-    uint64_t w = bitset->array[k - 1];
-    if ( w != 0 ) {
-      return  63 - cbitset_leading_zeroes(w) + (k - 1) * 64;
-    }
-  }
-  return 0;
-}
-
-/* Returns true if bitsets share no common elements, false otherwise.
- *
- * Performs early-out if common element found. */
-bool bitsets_disjoint(const bitset_t * CBITSET_RESTRICT b1, const bitset_t * CBITSET_RESTRICT b2) {
-  size_t minlength = b1->arraysize < b2->arraysize ? b1->arraysize : b2->arraysize;
-
-  for(size_t k = 0; k < minlength; k++) {
-    if((b1->array[k] & b2->array[k]) != 0)
-      return false;
-  }
-  return true;
-}
-
-
-/* Returns true if bitsets contain at least 1 common element, false if they are
- * disjoint.
- *
- * Performs early-out if common element found. */
-bool bitsets_intersect(const bitset_t * CBITSET_RESTRICT b1, const bitset_t * CBITSET_RESTRICT b2) {
-  size_t minlength = b1->arraysize < b2->arraysize ? b1->arraysize : b2->arraysize;
-
-  for(size_t k = 0; k < minlength; k++) {
-    if((b1->array[k] & b2->array[k]) != 0)
-      return true;
-  }
-  return false;
-}
-
-/* Returns true if b has any bits set in or after b->array[starting_loc]. */
-static bool any_bits_set(const bitset_t * b, size_t starting_loc) {
-  if(starting_loc >= b->arraysize) {
-    return false;
-  }
-  for(size_t k = starting_loc; k < b->arraysize; k++) {
-    if(b->array[k] != 0)
-      return true;
-  }
-  return false;
-}
-
-/* Returns true if b1 has all of b2's bits set.
- *
- * Performs early out if a bit is found in b2 that is not found in b1. */
-bool bitset_contains_all(const bitset_t * CBITSET_RESTRICT b1, const bitset_t * CBITSET_RESTRICT b2) {
-  size_t min_size = b1->arraysize;
-  if(b1->arraysize > b2->arraysize) {
-    min_size = b2->arraysize;
-  }
-  for(size_t k = 0; k < min_size; k++) {
-    if((b1->array[k] & b2->array[k]) != b2->array[k]) {
-      return false;
-    }
-  }
-  if(b2->arraysize > b1->arraysize) {
-    /* Need to check if b2 has any bits set beyond b1's array */
-    return !any_bits_set(b2, b1->arraysize);
-  }
-  return true;
-}
-
-size_t bitset_union_count(const bitset_t * CBITSET_RESTRICT b1, const bitset_t * CBITSET_RESTRICT b2) {
-  size_t answer = 0;
-  size_t minlength = b1->arraysize < b2->arraysize ? b1->arraysize : b2->arraysize;
-  size_t k = 0;
-  for( ; k + 3 < minlength; k += 4) {
-    answer += cbitset_hamming ( b1->array[k] | b2->array[k]);
-    answer += cbitset_hamming ( b1->array[k+1] | b2->array[k+1]);
-    answer += cbitset_hamming ( b1->array[k+2] | b2->array[k+2]);
-    answer += cbitset_hamming ( b1->array[k+3] | b2->array[k+3]);
-  }
-  for( ; k < minlength; ++k) {
-    answer += cbitset_hamming ( b1->array[k] | b2->array[k]);
-  }
-  if(b2->arraysize > b1->arraysize) {
-    //k = b1->arraysize;
-    for(; k + 3 < b2->arraysize; k+=4) {
-      answer += cbitset_hamming (b2->array[k]);
-      answer += cbitset_hamming (b2->array[k+1]);
-      answer += cbitset_hamming (b2->array[k+2]);
-      answer += cbitset_hamming (b2->array[k+3]);
-    }
-    for(; k < b2->arraysize; ++k) {
-      answer += cbitset_hamming (b2->array[k]);
-    }
-  } else {
-    //k = b2->arraysize;
-    for(; k  + 3 < b1->arraysize; k+=4) {
-      answer += cbitset_hamming (b1->array[k]);
-      answer += cbitset_hamming (b1->array[k+1]);
-      answer += cbitset_hamming (b1->array[k+2]);
-      answer += cbitset_hamming (b1->array[k+3]);
-    }
-    for(; k < b1->arraysize; ++k) {
-      answer += cbitset_hamming (b1->array[k]);
-    }
-  }
-  return answer;
-}
-
-void bitset_inplace_intersection(bitset_t * CBITSET_RESTRICT b1, const bitset_t * CBITSET_RESTRICT b2) {
-  size_t minlength = b1->arraysize < b2->arraysize ? b1->arraysize : b2->arraysize;
-  size_t k = 0;
-  for( ; k < minlength; ++k) {
-    b1->array[k] &= b2->array[k];
-  }
-  for(; k < b1->arraysize; ++k) {
-    b1->array[k] = 0; // memset could, maybe, be a tiny bit faster
-  }
-}
-
-size_t bitset_intersection_count(const bitset_t * CBITSET_RESTRICT b1, const bitset_t * CBITSET_RESTRICT b2) {
-  size_t answer = 0;
-  size_t minlength = b1->arraysize < b2->arraysize ? b1->arraysize : b2->arraysize;
-  for(size_t k = 0 ; k < minlength; ++k) {
-    answer += cbitset_hamming ( b1->array[k] & b2->array[k]);
-  }
-  return answer;
-}
-
-void bitset_inplace_difference(bitset_t * CBITSET_RESTRICT b1, const bitset_t * CBITSET_RESTRICT b2) {
-  size_t minlength = b1->arraysize < b2->arraysize ? b1->arraysize : b2->arraysize;
-  size_t k = 0;
-  for( ; k < minlength; ++k) {
-    b1->array[k] &= ~ (b2->array[k]);
-  }
-}
-
-
-size_t  bitset_difference_count(const bitset_t * CBITSET_RESTRICT b1, const bitset_t * CBITSET_RESTRICT b2) {
-  size_t minlength = b1->arraysize < b2->arraysize ? b1->arraysize : b2->arraysize;
-  size_t k = 0;
-  size_t answer = 0;
-  for( ; k < minlength; ++k) {
-    answer += cbitset_hamming (b1->array[k] & ~ (b2->array[k]));
-  }
-  for( ; k < b1->arraysize ; ++k) {
-    answer += cbitset_hamming (b1->array[k]);
-  }
-  return answer;
-}
-
-bool bitset_inplace_symmetric_difference(bitset_t * CBITSET_RESTRICT b1, const bitset_t * CBITSET_RESTRICT b2) {
-  size_t minlength = b1->arraysize < b2->arraysize ? b1->arraysize : b2->arraysize;
-  size_t k = 0;
-  for( ; k < minlength; ++k) {
-    b1->array[k] ^= b2->array[k];
-  }
-  if(b2->arraysize > b1->arraysize) {
-     size_t oldsize = b1->arraysize;
-     if(!bitset_resize( b1, b2->arraysize, false)) return false;
-     memcpy(b1->array + oldsize, b2->array + oldsize, (b2->arraysize - oldsize) * sizeof(uint64_t));
-  }
-  return true;
-}
-
-size_t  bitset_symmetric_difference_count(const bitset_t * CBITSET_RESTRICT b1, const bitset_t * CBITSET_RESTRICT b2) {
-  size_t minlength = b1->arraysize < b2->arraysize ? b1->arraysize : b2->arraysize;
-  size_t k = 0;
-  size_t answer = 0;
-  for( ; k < minlength; ++k) {
-    answer += cbitset_hamming(b1->array[k] ^ b2->array[k]);
-  }
-  if(b2->arraysize > b1->arraysize) {
-    for( ; k < b2->arraysize; ++k) {
-      answer += cbitset_hamming(b2->array[k]);
-    }
-  } else {
-    for( ; k < b1->arraysize; ++k) {
-      answer += cbitset_hamming(b1->array[k]);
-    }
-  }
-  return answer;
-}
-
-
-
-bool bitset_trim(bitset_t * bitset) {
-  size_t newsize = bitset->arraysize;
-  while(newsize > 0) {
-    if(bitset->array[newsize - 1] == 0)
-        newsize -= 1;
-    else
-        break;
-  }
-  if(bitset->capacity == newsize) return true; // nothing to do
-
-  uint64_t *newarray;
-  if ((newarray = (uint64_t *) realloc(bitset->array, sizeof(uint64_t) * newsize)) == NULL) {
-      return false;
-  }
-  bitset->array = newarray;
-  bitset->capacity = newsize;
-  bitset->arraysize = newsize;
-  return true;
-}
+#include <stdlib.h>
+#include <stdio.h>
+#include <limits.h>
+#include <stdint.h>
+#include <string.h>
+
+#include "bitset.h"
+extern inline void bitset_print(const bitset_t *b);
+extern inline bool bitset_for_each(const bitset_t *b, bitset_iterator iterator,
+                                   void *ptr);
+extern inline size_t bitset_next_set_bits(const bitset_t *bitset, size_t *buffer,
+                                 size_t capacity, size_t *startfrom);
+extern inline void bitset_set_to_value(bitset_t *bitset, size_t i, bool flag);
+extern inline bool bitset_next_set_bit(const bitset_t *bitset, size_t *i);
+extern inline void bitset_set(bitset_t *bitset, size_t i);
+extern inline bool bitset_get(const bitset_t *bitset, size_t i);
+extern inline size_t bitset_size_in_words(const bitset_t *bitset);
+extern inline size_t bitset_size_in_bits(const bitset_t *bitset);
+extern inline size_t bitset_size_in_bytes(const bitset_t *bitset);
+
+/* Create a new bitset. Return NULL in case of failure. */
+bitset_t *bitset_create() {
+  bitset_t *bitset = NULL;
+  /* Allocate the bitset itself. */
+  if( ( bitset = (bitset_t*) malloc( sizeof( bitset_t ) ) ) == NULL ) {
+      return NULL;
+  }
+  bitset->array = NULL;
+  bitset->arraysize = 0;
+  bitset->capacity = 0;
+  return bitset;
+}
+
+/* Create a new bitset able to contain size bits. Return NULL in case of failure. */
+bitset_t *bitset_create_with_capacity( size_t size ) {
+  bitset_t *bitset = NULL;
+  /* Allocate the bitset itself. */
+  if( ( bitset = (bitset_t*) malloc( sizeof( bitset_t ) ) ) == NULL ) {
+      return NULL;
+  }
+  bitset->arraysize = (size + sizeof(uint64_t) * 8 - 1) / (sizeof(uint64_t) * 8);
+  bitset->capacity = bitset->arraysize;
+  if ((bitset->array = (uint64_t *) calloc(bitset->arraysize, sizeof(uint64_t))) == NULL) {
+    free(bitset);
+    return NULL;
+  }
+  return bitset;
+}
+
+/* Create a copy */
+bitset_t *bitset_copy( const bitset_t * bitset ) {
+  bitset_t *copy = NULL;
+  /* Allocate the bitset itself. */
+  if( ( copy = (bitset_t*) malloc( sizeof( bitset_t ) ) ) == NULL ) {
+      return NULL;
+  }
+  memcpy(copy, bitset, sizeof(bitset_t));
+  copy->capacity = copy->arraysize;
+  if ((copy->array = (uint64_t *) malloc(sizeof(uint64_t) * bitset->arraysize)) == NULL) {
+    free(copy);
+    return NULL;
+  }
+  memcpy(copy->array,bitset->array,sizeof(uint64_t) * bitset->arraysize);
+  return copy;
+}
+
+void bitset_clear(bitset_t *bitset) {
+  memset(bitset->array,0,sizeof(uint64_t) * bitset->arraysize);
+}
+
+void bitset_fill(bitset_t *bitset) {
+  memset(bitset->array,0xff,sizeof(uint64_t) * bitset->arraysize);
+}
+
+
+void bitset_shift_left(bitset_t *bitset, size_t s) {
+  size_t extra_words = s / 64;
+  int inword_shift = s % 64;
+  size_t as = bitset->arraysize;
+  if(inword_shift == 0) {
+    bitset_resize(bitset,as + extra_words, false);
+    // could be done with a memmove
+    for(size_t i = as + extra_words ; i > extra_words; i--) {
+      bitset->array[i - 1] = bitset->array[i - 1 - extra_words];
+    }
+  } else {
+    bitset_resize(bitset,as + extra_words + 1, true);
+    bitset->array[as + extra_words] =
+     bitset->array[as - 1] >> (64 - inword_shift);
+    for(size_t i = as + extra_words ; i >= extra_words + 2; i--) {
+      bitset->array[i - 1] = (bitset->array[i - 1 - extra_words] << inword_shift)
+      | (bitset->array[i - 2 - extra_words]>>(64 - inword_shift));
+    }
+    bitset->array[extra_words] = bitset->array[0] <<  inword_shift;
+  }
+  for(size_t i = 0; i < extra_words; i++) {
+    bitset->array[i] = 0;
+  }
+}
+
+
+void bitset_shift_right(bitset_t *bitset, size_t s) {
+  size_t extra_words = s / 64;
+  int inword_shift = s % 64;
+  size_t as = bitset->arraysize;
+  if(inword_shift == 0) {
+    // could be done with a memmove
+    for(size_t i = 0 ; i < as - extra_words; i++) {
+      bitset->array[i] = bitset->array[i + extra_words];
+    }
+    bitset_resize(bitset,as - extra_words, false);
+
+  } else {
+    for(size_t i = 0 ; i + extra_words + 1 < as ; i++) {
+      bitset->array[i] = (bitset->array[i + extra_words] >> inword_shift)
+      | (bitset->array[i + extra_words + 1] << (64 - inword_shift));
+    }
+    bitset->array[as - extra_words - 1] = (bitset->array[as - 1] >> inword_shift);
+    bitset_resize(bitset,as - extra_words , false);
+  }
+}
+
+/* Free memory. */
+void bitset_free(bitset_t *bitset) {
+  free(bitset->array);
+  free(bitset);
+}
+
+bool bitset_grow(bitset_t *bitset,  size_t newarraysize) {
+  if(newarraysize < bitset->arraysize) { return false; }
+  if(newarraysize > SIZE_MAX/64) { return false; }
+  if (bitset->capacity < newarraysize) {
+    uint64_t *newarray;
+    size_t newcapacity = bitset->capacity;
+    if(newcapacity == 0) { newcapacity = 1; }
+    while(newcapacity < newarraysize) { newcapacity *= 2; }
+    if ((newarray = (uint64_t *) realloc(bitset->array, sizeof(uint64_t) * newcapacity)) == NULL) {
+      return false;
+    }
+    bitset->capacity = newcapacity;
+    bitset->array = newarray;
+  }
+  memset(bitset->array + bitset->arraysize, 0, sizeof(uint64_t) * (newarraysize - bitset->arraysize));
+  bitset->arraysize = newarraysize;
+  return true; // success!
+}
+/* Resize the bitset so that it can support newarraysize * 64 bits. Return true in case of success, false for failure. */
+bool bitset_resize(bitset_t *bitset,  size_t newarraysize, bool padwithzeroes) {
+  if(newarraysize > SIZE_MAX/64) { return false; }
+  size_t smallest = newarraysize < bitset->arraysize ? newarraysize : bitset->arraysize;
+  if (bitset->capacity < newarraysize) {
+    uint64_t *newarray;
+    size_t newcapacity = (UINT64_C(0xFFFFFFFFFFFFFFFF) >> cbitset_leading_zeroes(newarraysize)) + 1;
+    if ((newarray = (uint64_t *) realloc(bitset->array, sizeof(uint64_t) * newcapacity)) == NULL) {
+      return false;
+    }
+    bitset->capacity = newcapacity;
+    bitset->array = newarray;
+  }
+  if (padwithzeroes && (newarraysize > smallest)) {
+    memset(bitset->array + smallest,0,sizeof(uint64_t) * (newarraysize - smallest));
+  }
+  bitset->arraysize = newarraysize;
+  return true; // success!
+}
+
+
+
+size_t bitset_count(const bitset_t *bitset) {
+    size_t card = 0;
+    size_t k = 0;
+    for(; k + 7 < bitset->arraysize; k+=8) {
+        card += cbitset_hamming(bitset->array[k]);
+        card += cbitset_hamming(bitset->array[k+1]);
+        card += cbitset_hamming(bitset->array[k+2]);
+        card += cbitset_hamming(bitset->array[k+3]);
+        card += cbitset_hamming(bitset->array[k+4]);
+        card += cbitset_hamming(bitset->array[k+5]);
+        card += cbitset_hamming(bitset->array[k+6]);
+        card += cbitset_hamming(bitset->array[k+7]);
+    }
+    for(; k + 3 < bitset->arraysize; k+=4) {
+        card += cbitset_hamming(bitset->array[k]);
+        card += cbitset_hamming(bitset->array[k+1]);
+        card += cbitset_hamming(bitset->array[k+2]);
+        card += cbitset_hamming(bitset->array[k+3]);
+    }
+    for(; k < bitset->arraysize; k++) {
+        card += cbitset_hamming(bitset->array[k]);
+    }
+    return card;
+}
+
+
+bool bitset_inplace_union(bitset_t * CBITSET_RESTRICT b1, const bitset_t * CBITSET_RESTRICT b2) {
+  size_t minlength = b1->arraysize < b2->arraysize ? b1->arraysize : b2->arraysize;
+  for(size_t k = 0 ; k < minlength; ++k) {
+    b1->array[k] |= b2->array[k];
+  }
+  if(b2->arraysize > b1->arraysize) {
+     size_t oldsize = b1->arraysize;
+     if(!bitset_resize( b1, b2->arraysize, false)) return false;
+     memcpy(b1->array + oldsize, b2->array + oldsize, (b2->arraysize - oldsize) * sizeof(uint64_t));
+  }
+  return true;
+}
+
+size_t bitset_minimum(const bitset_t *bitset) {
+  for(size_t k = 0; k < bitset->arraysize; k++) {
+    uint64_t w = bitset->array[k];
+    if ( w != 0 ) {
+      return cbitset_trailing_zeroes(w) + k * 64;
+    }
+  }
+  return 0;
+}
+
+size_t bitset_maximum(const bitset_t *bitset) {
+  for(size_t k = bitset->arraysize ; k > 0 ; k--) {
+    uint64_t w = bitset->array[k - 1];
+    if ( w != 0 ) {
+      return  63 - cbitset_leading_zeroes(w) + (k - 1) * 64;
+    }
+  }
+  return 0;
+}
+
+/* Returns true if bitsets share no common elements, false otherwise.
+ *
+ * Performs early-out if common element found. */
+bool bitsets_disjoint(const bitset_t * CBITSET_RESTRICT b1, const bitset_t * CBITSET_RESTRICT b2) {
+  size_t minlength = b1->arraysize < b2->arraysize ? b1->arraysize : b2->arraysize;
+
+  for(size_t k = 0; k < minlength; k++) {
+    if((b1->array[k] & b2->array[k]) != 0)
+      return false;
+  }
+  return true;
+}
+
+
+/* Returns true if bitsets contain at least 1 common element, false if they are
+ * disjoint.
+ *
+ * Performs early-out if common element found. */
+bool bitsets_intersect(const bitset_t * CBITSET_RESTRICT b1, const bitset_t * CBITSET_RESTRICT b2) {
+  size_t minlength = b1->arraysize < b2->arraysize ? b1->arraysize : b2->arraysize;
+
+  for(size_t k = 0; k < minlength; k++) {
+    if((b1->array[k] & b2->array[k]) != 0)
+      return true;
+  }
+  return false;
+}
+
+/* Returns true if b has any bits set in or after b->array[starting_loc]. */
+static bool any_bits_set(const bitset_t * b, size_t starting_loc) {
+  if(starting_loc >= b->arraysize) {
+    return false;
+  }
+  for(size_t k = starting_loc; k < b->arraysize; k++) {
+    if(b->array[k] != 0)
+      return true;
+  }
+  return false;
+}
+
+/* Returns true if b1 has all of b2's bits set.
+ *
+ * Performs early out if a bit is found in b2 that is not found in b1. */
+bool bitset_contains_all(const bitset_t * CBITSET_RESTRICT b1, const bitset_t * CBITSET_RESTRICT b2) {
+  size_t min_size = b1->arraysize;
+  if(b1->arraysize > b2->arraysize) {
+    min_size = b2->arraysize;
+  }
+  for(size_t k = 0; k < min_size; k++) {
+    if((b1->array[k] & b2->array[k]) != b2->array[k]) {
+      return false;
+    }
+  }
+  if(b2->arraysize > b1->arraysize) {
+    /* Need to check if b2 has any bits set beyond b1's array */
+    return !any_bits_set(b2, b1->arraysize);
+  }
+  return true;
+}
+
+size_t bitset_union_count(const bitset_t * CBITSET_RESTRICT b1, const bitset_t * CBITSET_RESTRICT b2) {
+  size_t answer = 0;
+  size_t minlength = b1->arraysize < b2->arraysize ? b1->arraysize : b2->arraysize;
+  size_t k = 0;
+  for( ; k + 3 < minlength; k += 4) {
+    answer += cbitset_hamming ( b1->array[k] | b2->array[k]);
+    answer += cbitset_hamming ( b1->array[k+1] | b2->array[k+1]);
+    answer += cbitset_hamming ( b1->array[k+2] | b2->array[k+2]);
+    answer += cbitset_hamming ( b1->array[k+3] | b2->array[k+3]);
+  }
+  for( ; k < minlength; ++k) {
+    answer += cbitset_hamming ( b1->array[k] | b2->array[k]);
+  }
+  if(b2->arraysize > b1->arraysize) {
+    //k = b1->arraysize;
+    for(; k + 3 < b2->arraysize; k+=4) {
+      answer += cbitset_hamming (b2->array[k]);
+      answer += cbitset_hamming (b2->array[k+1]);
+      answer += cbitset_hamming (b2->array[k+2]);
+      answer += cbitset_hamming (b2->array[k+3]);
+    }
+    for(; k < b2->arraysize; ++k) {
+      answer += cbitset_hamming (b2->array[k]);
+    }
+  } else {
+    //k = b2->arraysize;
+    for(; k  + 3 < b1->arraysize; k+=4) {
+      answer += cbitset_hamming (b1->array[k]);
+      answer += cbitset_hamming (b1->array[k+1]);
+      answer += cbitset_hamming (b1->array[k+2]);
+      answer += cbitset_hamming (b1->array[k+3]);
+    }
+    for(; k < b1->arraysize; ++k) {
+      answer += cbitset_hamming (b1->array[k]);
+    }
+  }
+  return answer;
+}
+
+void bitset_inplace_intersection(bitset_t * CBITSET_RESTRICT b1, const bitset_t * CBITSET_RESTRICT b2) {
+  size_t minlength = b1->arraysize < b2->arraysize ? b1->arraysize : b2->arraysize;
+  size_t k = 0;
+  for( ; k < minlength; ++k) {
+    b1->array[k] &= b2->array[k];
+  }
+  for(; k < b1->arraysize; ++k) {
+    b1->array[k] = 0; // memset could, maybe, be a tiny bit faster
+  }
+}
+
+size_t bitset_intersection_count(const bitset_t * CBITSET_RESTRICT b1, const bitset_t * CBITSET_RESTRICT b2) {
+  size_t answer = 0;
+  size_t minlength = b1->arraysize < b2->arraysize ? b1->arraysize : b2->arraysize;
+  for(size_t k = 0 ; k < minlength; ++k) {
+    answer += cbitset_hamming ( b1->array[k] & b2->array[k]);
+  }
+  return answer;
+}
+
+void bitset_inplace_difference(bitset_t * CBITSET_RESTRICT b1, const bitset_t * CBITSET_RESTRICT b2) {
+  size_t minlength = b1->arraysize < b2->arraysize ? b1->arraysize : b2->arraysize;
+  size_t k = 0;
+  for( ; k < minlength; ++k) {
+    b1->array[k] &= ~ (b2->array[k]);
+  }
+}
+
+
+size_t  bitset_difference_count(const bitset_t * CBITSET_RESTRICT b1, const bitset_t * CBITSET_RESTRICT b2) {
+  size_t minlength = b1->arraysize < b2->arraysize ? b1->arraysize : b2->arraysize;
+  size_t k = 0;
+  size_t answer = 0;
+  for( ; k < minlength; ++k) {
+    answer += cbitset_hamming (b1->array[k] & ~ (b2->array[k]));
+  }
+  for( ; k < b1->arraysize ; ++k) {
+    answer += cbitset_hamming (b1->array[k]);
+  }
+  return answer;
+}
+
+bool bitset_inplace_symmetric_difference(bitset_t * CBITSET_RESTRICT b1, const bitset_t * CBITSET_RESTRICT b2) {
+  size_t minlength = b1->arraysize < b2->arraysize ? b1->arraysize : b2->arraysize;
+  size_t k = 0;
+  for( ; k < minlength; ++k) {
+    b1->array[k] ^= b2->array[k];
+  }
+  if(b2->arraysize > b1->arraysize) {
+     size_t oldsize = b1->arraysize;
+     if(!bitset_resize( b1, b2->arraysize, false)) return false;
+     memcpy(b1->array + oldsize, b2->array + oldsize, (b2->arraysize - oldsize) * sizeof(uint64_t));
+  }
+  return true;
+}
+
+size_t  bitset_symmetric_difference_count(const bitset_t * CBITSET_RESTRICT b1, const bitset_t * CBITSET_RESTRICT b2) {
+  size_t minlength = b1->arraysize < b2->arraysize ? b1->arraysize : b2->arraysize;
+  size_t k = 0;
+  size_t answer = 0;
+  for( ; k < minlength; ++k) {
+    answer += cbitset_hamming(b1->array[k] ^ b2->array[k]);
+  }
+  if(b2->arraysize > b1->arraysize) {
+    for( ; k < b2->arraysize; ++k) {
+      answer += cbitset_hamming(b2->array[k]);
+    }
+  } else {
+    for( ; k < b1->arraysize; ++k) {
+      answer += cbitset_hamming(b1->array[k]);
+    }
+  }
+  return answer;
+}
+
+
+
+bool bitset_trim(bitset_t * bitset) {
+  size_t newsize = bitset->arraysize;
+  while(newsize > 0) {
+    if(bitset->array[newsize - 1] == 0)
+        newsize -= 1;
+    else
+        break;
+  }
+  if(bitset->capacity == newsize) return true; // nothing to do
+
+  uint64_t *newarray;
+  if ((newarray = (uint64_t *) realloc(bitset->array, sizeof(uint64_t) * newsize)) == NULL) {
+      return false;
+  }
+  bitset->array = newarray;
+  bitset->capacity = newsize;
+  bitset->arraysize = newsize;
+  return true;
+}
```

### Comparing `pybitset-0.0.1.dev1/cbitset/tests/unit.c` & `pybitset-0.0.1.dev2/cbitset/tests/unit.c`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,268 +1,268 @@
-#include <stdio.h>
-#include <assert.h>
-#include <stdlib.h>
-#include "bitset.h"
-
-void test_iterate() {
-  bitset_t * b = bitset_create();
-  for(int k = 0; k < 1000; ++k)
-    bitset_set(b,3*k);
-  assert(bitset_count(b) == 1000);
-  size_t k = 0;
-  for(size_t i = 0; bitset_next_set_bit(b,&i) ; i++) {
-    assert(i == k);
-    k += 3;
-  }
-  assert(k == 3000);
-  bitset_free(b);
-}
-
-bool increment(size_t value, void *param) {
-  size_t k;
-  memcpy(&k, param, sizeof(size_t));
-  assert(value == k);
-  k += 3;
-  memcpy(param, &k, sizeof(size_t));
-  return true;
-}
-
-void test_iterate2() {
-  bitset_t * b = bitset_create();
-  for(int k = 0; k < 1000; ++k)
-    bitset_set(b,3*k);
-  assert(bitset_count(b) == 1000);
-  size_t k = 0;
-  bitset_for_each(b,increment,&k);
-  assert(k == 3000);
-  bitset_free(b);
-}
-
-
-void test_construct() {
-  bitset_t * b = bitset_create();
-  for(int k = 0; k < 1000; ++k)
-    bitset_set(b,3*k);
-  assert(bitset_count(b) == 1000);
-  for(int k = 0; k < 3*1000; ++k)
-    assert(bitset_get(b,k) == (k/3*3 == k));
-  bitset_free(b);
-}
-
-void test_max_min() {
-  bitset_t * b = bitset_create();
-  for(size_t k = 100; k < 1000; ++k) {
-    bitset_set(b,3*k);
-    assert(bitset_minimum(b) == 3 * 100);
-    assert(bitset_maximum(b) == 3 * k);
-  }
-  bitset_free(b);
-}
-
-void test_shift_left() {
-  for(size_t sh = 0; sh < 256; sh++) {
-    bitset_t * b = bitset_create();
-    int power = 3;
-    size_t s1 = 100;
-    size_t s2 = 5000;
-    for(size_t k = s1; k < s2; ++k) {
-      bitset_set(b,power*k);
-    }
-    size_t mycount = bitset_count(b);
-    bitset_shift_left(b,sh);
-    assert(bitset_count(b) == mycount);
-    for(size_t k = s1; k < s2; ++k) {
-      assert(bitset_get(b,power*k + sh));
-    }
-    bitset_free(b);
-  }
-}
-
-void test_set_to_val() {
-   bitset_t * b = bitset_create();
-   bitset_set_to_value(b, 1, true);
-   bitset_set_to_value(b, 1, false);
-   bitset_set_to_value(b, 10, false);
-   bitset_set_to_value(b, 10, true);
-   assert(bitset_get(b,10));
-   assert(!bitset_get(b,1));
-   bitset_free(b);
-}
-
-void test_shift_right() {
-  for(size_t sh = 0; sh < 256; sh++) {
-    bitset_t * b = bitset_create();
-    int power = 3;
-    size_t s1 = 100 + sh;
-    size_t s2 = s1+5000;
-    for(size_t k = s1; k < s2; ++k) {
-      bitset_set(b,power*k);
-    }
-    size_t mycount = bitset_count(b);
-    bitset_shift_right(b,sh);
-    assert(bitset_count(b) == mycount);
-    for(size_t k = s1; k < s2; ++k) {
-      assert(bitset_get(b,power*k - sh));
-    }
-    bitset_free(b);
-  }
-}
-
-void test_union_intersection() {
-  bitset_t * b1 = bitset_create();
-  bitset_t * b2 = bitset_create();
-
-  for(int k = 0; k < 1000; ++k) {
-    bitset_set(b1,2*k);
-    bitset_set(b2,2*k+1);
-  }
-  // calling xor twice should leave things unchanged
-  bitset_inplace_symmetric_difference(b1,b2);
-  assert(bitset_count(b1) == 2000);
-  bitset_inplace_symmetric_difference(b1,b2);
-  assert(bitset_count(b1) == 1000);
-  bitset_inplace_difference(b1,b2);// should make no difference
-  assert(bitset_count(b1) == 1000);
-  bitset_inplace_union(b1,b2);
-  assert(bitset_count(b1) == 2000);
-  bitset_inplace_intersection(b1,b2);
-  assert(bitset_count(b1) == 1000);
-  bitset_inplace_difference(b1,b2);
-  assert(bitset_count(b1) == 0);
-  bitset_inplace_union(b1,b2);
-  bitset_inplace_difference(b2,b1);
-  assert(bitset_count(b2) == 0);
-  bitset_free(b1);
-  bitset_free(b2);
-}
-
-void test_counts() {
-  bitset_t * b1 = bitset_create();
-  bitset_t * b2 = bitset_create();
-
-  for(int k = 0; k < 1000; ++k) {
-    bitset_set(b1,2*k);
-    bitset_set(b2,3*k);
-  }
-  assert(bitset_intersection_count(b1,b2) == 334);
-  assert(bitset_union_count(b1,b2) == 1666);
-  bitset_free(b1);
-  bitset_free(b2);
-}
-
-/* Creates 2 bitsets, one containing even numbers the other odds.
-Checks bitsets_disjoint() returns that they are disjoint, then sets a common
-bit between both sets and checks that they are no longer disjoint. */
-void test_disjoint() {
-  bitset_t * evens = bitset_create();
-  bitset_t * odds  = bitset_create();
-
-  for(int i = 0; i < 1000; i++) {
-    if(i % 2 == 0)
-      bitset_set(evens, i);
-    else
-      bitset_set(odds, i);
-  }
-
-  assert(bitsets_disjoint(evens, odds));
-
-  bitset_set(evens, 501);
-  bitset_set(odds, 501);
-
-  assert(!bitsets_disjoint(evens, odds));
-
-  bitset_free(evens);
-  bitset_free(odds);
-}
-
-/* Creates 2 bitsets, one containing even numbers the other odds.
-Checks that bitsets_intersect() returns that they do not intersect, then sets
-a common bit and checks that they now intersect. */
-void test_intersects() {
-  bitset_t * evens = bitset_create();
-  bitset_t * odds  = bitset_create();
-
-  for(int i = 0; i < 1000; i++) {
-    if(i % 2 == 0)
-      bitset_set(evens, i);
-    else
-      bitset_set(odds, i);
-  }
-
-  assert(!bitsets_intersect(evens, odds));
-
-  bitset_set(evens, 1001);
-  bitset_set(odds, 1001);
-
-  assert(bitsets_intersect(evens, odds));
-
-  bitset_free(evens);
-  bitset_free(odds);
-}
-/* Create 2 bitsets with different capacity, where the bigger superset
-contains the subset bits plus additional bits after the subset arraysize.
-Checks that the bitset_contains_all() returns false when checking if
-the superset contains all the subset bits, and true in the opposite case. */
-void test_contains_all_different_sizes() {
-  const size_t superset_size = 10;
-  const size_t subset_size = 5;
-
-  bitset_t * superset = bitset_create_with_capacity(superset_size);
-  bitset_t * subset   = bitset_create_with_capacity(subset_size);
-
-  bitset_set(superset, 1);
-  bitset_set(superset, subset_size - 1);
-  bitset_set(superset, subset_size + 1);
-
-  bitset_set(subset, 1);
-  bitset_set(subset, subset_size - 1);
-
-  assert(bitset_contains_all(superset, subset));
-  assert(!bitset_contains_all(subset, superset));
-
-  bitset_free(superset);
-  bitset_free(subset);
-}
-
-/* Creates 2 bitsets, one with all bits from 0->1000 set, the other with only
-even bits set in the same range. Checks that the bitset_contains_all()
-returns true, then sets a single bit at 1001 in the prior subset and checks that
-bitset_contains_all() returns false. */
-void test_contains_all() {
-  bitset_t * superset = bitset_create();
-  bitset_t * subset   = bitset_create();
-
-  for(int i = 0; i < 1000; i++) {
-    bitset_set(superset, i);
-    if(i % 2 == 0)
-      bitset_set(subset, i);
-  }
-
-  assert(bitset_contains_all(superset, subset));
-  assert(!bitset_contains_all(subset, superset));
-
-  bitset_set(subset, 1001);
-
-  assert(!bitset_contains_all(superset, subset));
-  assert(!bitset_contains_all(subset, superset));
-
-  bitset_free(superset);
-  bitset_free(subset);
-}
-
-
-int main() {
-  test_set_to_val();
-  test_construct();
-  test_union_intersection();
-  test_iterate();
-  test_iterate2();
-  test_max_min();
-  test_counts();
-  test_shift_right();
-  test_shift_left();
-  test_disjoint();
-  test_intersects();
-  test_contains_all();
-  test_contains_all_different_sizes();
-  printf("All asserts passed. Code is probably ok.\n");
-}
+#include <stdio.h>
+#include <assert.h>
+#include <stdlib.h>
+#include "bitset.h"
+
+void test_iterate() {
+  bitset_t * b = bitset_create();
+  for(int k = 0; k < 1000; ++k)
+    bitset_set(b,3*k);
+  assert(bitset_count(b) == 1000);
+  size_t k = 0;
+  for(size_t i = 0; bitset_next_set_bit(b,&i) ; i++) {
+    assert(i == k);
+    k += 3;
+  }
+  assert(k == 3000);
+  bitset_free(b);
+}
+
+bool increment(size_t value, void *param) {
+  size_t k;
+  memcpy(&k, param, sizeof(size_t));
+  assert(value == k);
+  k += 3;
+  memcpy(param, &k, sizeof(size_t));
+  return true;
+}
+
+void test_iterate2() {
+  bitset_t * b = bitset_create();
+  for(int k = 0; k < 1000; ++k)
+    bitset_set(b,3*k);
+  assert(bitset_count(b) == 1000);
+  size_t k = 0;
+  bitset_for_each(b,increment,&k);
+  assert(k == 3000);
+  bitset_free(b);
+}
+
+
+void test_construct() {
+  bitset_t * b = bitset_create();
+  for(int k = 0; k < 1000; ++k)
+    bitset_set(b,3*k);
+  assert(bitset_count(b) == 1000);
+  for(int k = 0; k < 3*1000; ++k)
+    assert(bitset_get(b,k) == (k/3*3 == k));
+  bitset_free(b);
+}
+
+void test_max_min() {
+  bitset_t * b = bitset_create();
+  for(size_t k = 100; k < 1000; ++k) {
+    bitset_set(b,3*k);
+    assert(bitset_minimum(b) == 3 * 100);
+    assert(bitset_maximum(b) == 3 * k);
+  }
+  bitset_free(b);
+}
+
+void test_shift_left() {
+  for(size_t sh = 0; sh < 256; sh++) {
+    bitset_t * b = bitset_create();
+    int power = 3;
+    size_t s1 = 100;
+    size_t s2 = 5000;
+    for(size_t k = s1; k < s2; ++k) {
+      bitset_set(b,power*k);
+    }
+    size_t mycount = bitset_count(b);
+    bitset_shift_left(b,sh);
+    assert(bitset_count(b) == mycount);
+    for(size_t k = s1; k < s2; ++k) {
+      assert(bitset_get(b,power*k + sh));
+    }
+    bitset_free(b);
+  }
+}
+
+void test_set_to_val() {
+   bitset_t * b = bitset_create();
+   bitset_set_to_value(b, 1, true);
+   bitset_set_to_value(b, 1, false);
+   bitset_set_to_value(b, 10, false);
+   bitset_set_to_value(b, 10, true);
+   assert(bitset_get(b,10));
+   assert(!bitset_get(b,1));
+   bitset_free(b);
+}
+
+void test_shift_right() {
+  for(size_t sh = 0; sh < 256; sh++) {
+    bitset_t * b = bitset_create();
+    int power = 3;
+    size_t s1 = 100 + sh;
+    size_t s2 = s1+5000;
+    for(size_t k = s1; k < s2; ++k) {
+      bitset_set(b,power*k);
+    }
+    size_t mycount = bitset_count(b);
+    bitset_shift_right(b,sh);
+    assert(bitset_count(b) == mycount);
+    for(size_t k = s1; k < s2; ++k) {
+      assert(bitset_get(b,power*k - sh));
+    }
+    bitset_free(b);
+  }
+}
+
+void test_union_intersection() {
+  bitset_t * b1 = bitset_create();
+  bitset_t * b2 = bitset_create();
+
+  for(int k = 0; k < 1000; ++k) {
+    bitset_set(b1,2*k);
+    bitset_set(b2,2*k+1);
+  }
+  // calling xor twice should leave things unchanged
+  bitset_inplace_symmetric_difference(b1,b2);
+  assert(bitset_count(b1) == 2000);
+  bitset_inplace_symmetric_difference(b1,b2);
+  assert(bitset_count(b1) == 1000);
+  bitset_inplace_difference(b1,b2);// should make no difference
+  assert(bitset_count(b1) == 1000);
+  bitset_inplace_union(b1,b2);
+  assert(bitset_count(b1) == 2000);
+  bitset_inplace_intersection(b1,b2);
+  assert(bitset_count(b1) == 1000);
+  bitset_inplace_difference(b1,b2);
+  assert(bitset_count(b1) == 0);
+  bitset_inplace_union(b1,b2);
+  bitset_inplace_difference(b2,b1);
+  assert(bitset_count(b2) == 0);
+  bitset_free(b1);
+  bitset_free(b2);
+}
+
+void test_counts() {
+  bitset_t * b1 = bitset_create();
+  bitset_t * b2 = bitset_create();
+
+  for(int k = 0; k < 1000; ++k) {
+    bitset_set(b1,2*k);
+    bitset_set(b2,3*k);
+  }
+  assert(bitset_intersection_count(b1,b2) == 334);
+  assert(bitset_union_count(b1,b2) == 1666);
+  bitset_free(b1);
+  bitset_free(b2);
+}
+
+/* Creates 2 bitsets, one containing even numbers the other odds.
+Checks bitsets_disjoint() returns that they are disjoint, then sets a common
+bit between both sets and checks that they are no longer disjoint. */
+void test_disjoint() {
+  bitset_t * evens = bitset_create();
+  bitset_t * odds  = bitset_create();
+
+  for(int i = 0; i < 1000; i++) {
+    if(i % 2 == 0)
+      bitset_set(evens, i);
+    else
+      bitset_set(odds, i);
+  }
+
+  assert(bitsets_disjoint(evens, odds));
+
+  bitset_set(evens, 501);
+  bitset_set(odds, 501);
+
+  assert(!bitsets_disjoint(evens, odds));
+
+  bitset_free(evens);
+  bitset_free(odds);
+}
+
+/* Creates 2 bitsets, one containing even numbers the other odds.
+Checks that bitsets_intersect() returns that they do not intersect, then sets
+a common bit and checks that they now intersect. */
+void test_intersects() {
+  bitset_t * evens = bitset_create();
+  bitset_t * odds  = bitset_create();
+
+  for(int i = 0; i < 1000; i++) {
+    if(i % 2 == 0)
+      bitset_set(evens, i);
+    else
+      bitset_set(odds, i);
+  }
+
+  assert(!bitsets_intersect(evens, odds));
+
+  bitset_set(evens, 1001);
+  bitset_set(odds, 1001);
+
+  assert(bitsets_intersect(evens, odds));
+
+  bitset_free(evens);
+  bitset_free(odds);
+}
+/* Create 2 bitsets with different capacity, where the bigger superset
+contains the subset bits plus additional bits after the subset arraysize.
+Checks that the bitset_contains_all() returns false when checking if
+the superset contains all the subset bits, and true in the opposite case. */
+void test_contains_all_different_sizes() {
+  const size_t superset_size = 10;
+  const size_t subset_size = 5;
+
+  bitset_t * superset = bitset_create_with_capacity(superset_size);
+  bitset_t * subset   = bitset_create_with_capacity(subset_size);
+
+  bitset_set(superset, 1);
+  bitset_set(superset, subset_size - 1);
+  bitset_set(superset, subset_size + 1);
+
+  bitset_set(subset, 1);
+  bitset_set(subset, subset_size - 1);
+
+  assert(bitset_contains_all(superset, subset));
+  assert(!bitset_contains_all(subset, superset));
+
+  bitset_free(superset);
+  bitset_free(subset);
+}
+
+/* Creates 2 bitsets, one with all bits from 0->1000 set, the other with only
+even bits set in the same range. Checks that the bitset_contains_all()
+returns true, then sets a single bit at 1001 in the prior subset and checks that
+bitset_contains_all() returns false. */
+void test_contains_all() {
+  bitset_t * superset = bitset_create();
+  bitset_t * subset   = bitset_create();
+
+  for(int i = 0; i < 1000; i++) {
+    bitset_set(superset, i);
+    if(i % 2 == 0)
+      bitset_set(subset, i);
+  }
+
+  assert(bitset_contains_all(superset, subset));
+  assert(!bitset_contains_all(subset, superset));
+
+  bitset_set(subset, 1001);
+
+  assert(!bitset_contains_all(superset, subset));
+  assert(!bitset_contains_all(subset, superset));
+
+  bitset_free(superset);
+  bitset_free(subset);
+}
+
+
+int main() {
+  test_set_to_val();
+  test_construct();
+  test_union_intersection();
+  test_iterate();
+  test_iterate2();
+  test_max_min();
+  test_counts();
+  test_shift_right();
+  test_shift_left();
+  test_disjoint();
+  test_intersects();
+  test_contains_all();
+  test_contains_all_different_sizes();
+  printf("All asserts passed. Code is probably ok.\n");
+}
```

### Comparing `pybitset-0.0.1.dev1/pybitset/backends/cffi/__init__.py` & `pybitset-0.0.1.dev2/pybitset/backends/cffi/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,151 +1,154 @@
-"""
-Copyright (c) 2008-2023 synodriver <diguohuangjiajinweijun@gmail.com>
-"""
-import pyrsync
-
-from pybitset.backends.cffi._bitset import ffi, lib
-
-
-@ffi.def_extern()
-def bitset_iterator_func(value: int, param) -> bool:
-    callback = ffi.from_handle(param)
-    return callback(value)
-
-
-class BitSetIter:
-    # cdef:
-    #     BitSet b
-    #     size_t i
-
-    def __init__(self, b: "BitSet"):
-        self.b = b
-        self.i = ffi.new("size_t*")
-        self.i[0] = 0
-
-    def __iter__(self):
-        return self
-
-    def __next__(self):
-        if lib.bitset_next_set_bit(self.b._bitset, self.i):
-            tmp = self.i[0]
-            self.i[0] += 1
-            return tmp
-        else:
-            raise StopIteration
-
-
-class BitSet:
-    # cdef lib.bitset_t * _bitset
-    def __init__(self, size: int = 0):
-        if size == 0:
-            self._bitset = lib.bitset_create()
-        else:
-            self._bitset = lib.bitset_create_with_capacity(size)
-        if not self._bitset:
-            raise MemoryError
-
-    def __del__(self):
-        lib.bitset_free(self._bitset)
-        self._bitset = ffi.NULL
-
-    @staticmethod
-    def from_ptr(ptr) -> "BitSet":
-        self = BitSet.__new__(BitSet)
-        self._bitset = ptr
-        return self
-
-    def clear(self):
-        lib.bitset_clear(self._bitset)
-
-    def fill(self):
-        lib.bitset_fill(self._bitset)
-
-    def copy(self) -> "BitSet":
-        ret = lib.bitset_copy(self._bitset)
-        return BitSet.from_ptr(ret)
-
-    def resize(self, newarraysize: int, padwithzeroes: bool) -> bool:
-        return lib.bitset_resize(self._bitset, newarraysize, padwithzeroes)
-
-    def size_in_bytes(self) -> int:
-        return lib.bitset_size_in_bytes(self._bitset)
-
-    def size_in_bits(self) -> int:
-        return lib.bitset_size_in_bits(self._bitset)
-
-    def size_in_words(self) -> int:
-        return lib.bitset_size_in_words(self._bitset)
-
-    def grow(self, newarraysize: int) -> bool:
-        return lib.bitset_grow(self._bitset, newarraysize)
-
-    def trim(self) -> bool:
-        return lib.bitset_trim(self._bitset)
-
-    def shift_left(self, s: int) -> None:
-        lib.bitset_shift_left(self._bitset, s)
-
-    def shift_right(self, s: int) -> None:
-        lib.bitset_shift_right(self._bitset, s)
-
-    def set(self, i: int) -> None:
-        lib.bitset_set(self._bitset, i)
-
-    def set_to_value(self, i: int, flag: bool) -> None:
-        lib.bitset_set_to_value(self._bitset, i, flag)
-
-    def get(self, i: int) -> bool:
-        return lib.bitset_get(self._bitset, i)
-
-    def count(self) -> int:
-        return lib.bitset_count(self._bitset)
-
-    def minimum(self) -> int:
-        return lib.bitset_minimum(self._bitset)
-
-    def maximum(self) -> int:
-        return lib.bitset_maximum(self._bitset)
-
-    def inplace_union(self, b2: "BitSet") -> bool:
-        return lib.bitset_inplace_union(self._bitset, b2._bitset)
-
-    def union_count(self, b2: "BitSet") -> int:
-        return lib.bitset_union_count(self._bitset, b2._bitset)
-
-    def inplace_intersection(self, b2: "BitSet"):
-        lib.bitset_inplace_intersection(self._bitset, b2._bitset)
-
-    def intersection_count(self, b2: "BitSet") -> int:
-        return lib.bitset_intersection_count(self._bitset, b2._bitset)
-
-    def disjoint(self, b2: "BitSet") -> bool:
-        return lib.bitsets_disjoint(self._bitset, b2._bitset)
-
-    def intersect(self, b2: "BitSet") -> bool:
-        return lib.bitsets_intersect(self._bitset, b2._bitset)
-
-    def contains_all(self, b2: "BitSet") -> bool:
-        return lib.bitset_contains_all(self._bitset, b2._bitset)
-
-    def inplace_difference(self, b2: "BitSet") -> None:
-        lib.bitset_inplace_difference(self._bitset, b2._bitset)
-
-    def difference_count(self, b2: "BitSet") -> int:
-        ret = lib.bitset_difference_count(self._bitset, b2._bitset)
-        return ret
-
-    def inplace_symmetric_difference(self, b2: "BitSet") -> bool:
-        return lib.bitset_inplace_symmetric_difference(self._bitset, b2._bitset)
-
-    def symmetric_difference_count(self, b2: "BitSet") -> int:
-        return lib.bitset_symmetric_difference_count(self._bitset, b2._bitset)
-
-    def __iter__(self):
-        return BitSetIter(self)
-
-    def for_each(self, func) -> bool:
-        handle = ffi.new_handle(func)
-        return lib.bitset_for_each(self._bitset, lib.bitset_iterator_func, handle)
-
-    def print(self) -> None:
-        lib.bitset_print(self._bitset)
+"""
+Copyright (c) 2008-2023 synodriver <diguohuangjiajinweijun@gmail.com>
+"""
+import pyrsync
+
+from pybitset.backends.cffi._bitset import ffi, lib
+
+
+@ffi.def_extern()
+def bitset_iterator_func(value: int, param) -> bool:
+    callback = ffi.from_handle(param)
+    return callback(value)
+
+
+class BitSetIter:
+    # cdef:
+    #     BitSet b
+    #     size_t i
+
+    def __init__(self, b: "BitSet"):
+        self.b = b
+        self.i = ffi.new("size_t*")
+        self.i[0] = 0
+
+    def __iter__(self):
+        return self
+
+    def __next__(self):
+        if lib.bitset_next_set_bit(self.b._bitset, self.i):
+            tmp = self.i[0]
+            self.i[0] += 1
+            return tmp
+        else:
+            raise StopIteration
+
+
+class BitSet:
+    # cdef lib.bitset_t * _bitset
+    def __init__(self, size: int = 0, _init: bool = True):
+        if _init:
+            if size == 0:
+                self._bitset = lib.bitset_create()
+            else:
+                self._bitset = lib.bitset_create_with_capacity(size)
+            if not self._bitset:
+                raise MemoryError
+        else:
+            self._bitset = ffi.NULL
+
+    def __del__(self):
+        lib.bitset_free(self._bitset)
+        self._bitset = ffi.NULL
+
+    @staticmethod
+    def from_ptr(ptr) -> "BitSet":
+        self = BitSet(_init=False)
+        self._bitset = ptr
+        return self
+
+    def clear(self):
+        lib.bitset_clear(self._bitset)
+
+    def fill(self):
+        lib.bitset_fill(self._bitset)
+
+    def copy(self) -> "BitSet":
+        ret = lib.bitset_copy(self._bitset)
+        return BitSet.from_ptr(ret)
+
+    def resize(self, newarraysize: int, padwithzeroes: bool) -> bool:
+        return lib.bitset_resize(self._bitset, newarraysize, padwithzeroes)
+
+    def size_in_bytes(self) -> int:
+        return lib.bitset_size_in_bytes(self._bitset)
+
+    def size_in_bits(self) -> int:
+        return lib.bitset_size_in_bits(self._bitset)
+
+    def size_in_words(self) -> int:
+        return lib.bitset_size_in_words(self._bitset)
+
+    def grow(self, newarraysize: int) -> bool:
+        return lib.bitset_grow(self._bitset, newarraysize)
+
+    def trim(self) -> bool:
+        return lib.bitset_trim(self._bitset)
+
+    def shift_left(self, s: int) -> None:
+        lib.bitset_shift_left(self._bitset, s)
+
+    def shift_right(self, s: int) -> None:
+        lib.bitset_shift_right(self._bitset, s)
+
+    def set(self, i: int) -> None:
+        lib.bitset_set(self._bitset, i)
+
+    def set_to_value(self, i: int, flag: bool) -> None:
+        lib.bitset_set_to_value(self._bitset, i, flag)
+
+    def get(self, i: int) -> bool:
+        return lib.bitset_get(self._bitset, i)
+
+    def count(self) -> int:
+        return lib.bitset_count(self._bitset)
+
+    def minimum(self) -> int:
+        return lib.bitset_minimum(self._bitset)
+
+    def maximum(self) -> int:
+        return lib.bitset_maximum(self._bitset)
+
+    def inplace_union(self, b2: "BitSet") -> bool:
+        return lib.bitset_inplace_union(self._bitset, b2._bitset)
+
+    def union_count(self, b2: "BitSet") -> int:
+        return lib.bitset_union_count(self._bitset, b2._bitset)
+
+    def inplace_intersection(self, b2: "BitSet"):
+        lib.bitset_inplace_intersection(self._bitset, b2._bitset)
+
+    def intersection_count(self, b2: "BitSet") -> int:
+        return lib.bitset_intersection_count(self._bitset, b2._bitset)
+
+    def disjoint(self, b2: "BitSet") -> bool:
+        return lib.bitsets_disjoint(self._bitset, b2._bitset)
+
+    def intersect(self, b2: "BitSet") -> bool:
+        return lib.bitsets_intersect(self._bitset, b2._bitset)
+
+    def contains_all(self, b2: "BitSet") -> bool:
+        return lib.bitset_contains_all(self._bitset, b2._bitset)
+
+    def inplace_difference(self, b2: "BitSet") -> None:
+        lib.bitset_inplace_difference(self._bitset, b2._bitset)
+
+    def difference_count(self, b2: "BitSet") -> int:
+        ret = lib.bitset_difference_count(self._bitset, b2._bitset)
+        return ret
+
+    def inplace_symmetric_difference(self, b2: "BitSet") -> bool:
+        return lib.bitset_inplace_symmetric_difference(self._bitset, b2._bitset)
+
+    def symmetric_difference_count(self, b2: "BitSet") -> int:
+        return lib.bitset_symmetric_difference_count(self._bitset, b2._bitset)
+
+    def __iter__(self):
+        return BitSetIter(self)
+
+    def for_each(self, func) -> bool:
+        handle = ffi.new_handle(func)
+        return lib.bitset_for_each(self._bitset, lib.bitset_iterator_func, handle)
+
+    def print(self) -> None:
+        lib.bitset_print(self._bitset)
```

### Comparing `pybitset-0.0.1.dev1/pybitset/backends/cffi/__pycache__/build.cpython-310.pyc` & `pybitset-0.0.1.dev2/pybitset/backends/cffi/build.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,380 +1,375 @@
-00000000: 6f0d 0d0a 0000 0000 daeb 8b64 1518 0000  o..........d....
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0006 0000 0040 0000 0073 6a00 0000 6400  .....@...sj...d.
-00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
-00000040: 6d03 5a03 0100 6503 8300 5a04 6504 a005  m.Z...e...Z.e...
-00000050: 6404 a101 0100 6405 5a06 6501 a001 6406  d.....d.Z.e...d.
-00000060: a101 5a07 6508 6507 8301 0100 6504 6a09  ..Z.e.e.....e.j.
-00000070: 6407 6506 6507 6408 6701 6409 8d04 0100  d.e.e.d.g.d.....
-00000080: 650a 640a 6b02 7233 6504 a00b a100 0100  e.d.k.r3e.......
-00000090: 6402 5300 6402 5300 290b 7a47 0a43 6f70  d.S.d.S.).zG.Cop
-000000a0: 7972 6967 6874 2028 6329 2032 3030 382d  yright (c) 2008-
-000000b0: 3230 3233 2073 796e 6f64 7269 7665 7220  2023 synodriver 
-000000c0: 3c64 6967 756f 6875 616e 676a 6961 6a69  <diguohuangjiaji
-000000d0: 6e77 6569 6a75 6e40 676d 6169 6c2e 636f  nweijun@gmail.co
-000000e0: 6d3e 0ae9 0000 0000 4e29 01da 0346 4649  m>......N)...FFI
-000000f0: 61ec 1400 000a 7374 7275 6374 2062 6974  a.....struct bit
-00000100: 7365 745f 7320 7b0a 2020 2020 7569 6e74  set_s {.    uint
-00000110: 3634 5f74 202a 2061 7272 6179 3b0a 2020  64_t * array;.  
-00000120: 2020 2f2a 2046 6f72 2073 696d 706c 6963    /* For simplic
-00000130: 6974 7920 616e 6420 7065 7266 6f72 6d61  ity and performa
-00000140: 6e63 652c 2077 6520 7072 6566 6572 2074  nce, we prefer t
-00000150: 6f20 6861 7665 2061 2073 697a 6520 616e  o have a size an
-00000160: 6420 6120 6361 7061 6369 7479 2074 6861  d a capacity tha
-00000170: 7420 6973 2061 206d 756c 7469 706c 6520  t is a multiple 
-00000180: 6f66 2036 3420 6269 7473 2e0a 2020 2020  of 64 bits..    
-00000190: 202a 2054 6875 7320 7765 206f 6e6c 7920   * Thus we only 
-000001a0: 7472 6163 6b20 7468 6520 7369 7a65 2061  track the size a
-000001b0: 6e64 2074 6865 2063 6170 6163 6974 7920  nd the capacity 
-000001c0: 696e 2074 6572 6d73 206f 6620 3634 2d62  in terms of 64-b
-000001d0: 6974 2077 6f72 6473 2061 6c6c 6f63 6174  it words allocat
-000001e0: 6564 202a 2f0a 2020 2020 7369 7a65 5f74  ed */.    size_t
-000001f0: 2061 7272 6179 7369 7a65 3b0a 2020 2020   arraysize;.    
-00000200: 7369 7a65 5f74 2063 6170 6163 6974 793b  size_t capacity;
-00000210: 0a0a 7d3b 0a0a 7479 7065 6465 6620 7374  ..};..typedef st
-00000220: 7275 6374 2062 6974 7365 745f 7320 6269  ruct bitset_s bi
-00000230: 7473 6574 5f74 3b0a 0a2f 2a20 4372 6561  tset_t;../* Crea
-00000240: 7465 2061 206e 6577 2062 6974 7365 742e  te a new bitset.
-00000250: 2052 6574 7572 6e20 4e55 4c4c 2069 6e20   Return NULL in 
-00000260: 6361 7365 206f 6620 6661 696c 7572 652e  case of failure.
-00000270: 202a 2f0a 6269 7473 6574 5f74 202a 6269   */.bitset_t *bi
-00000280: 7473 6574 5f63 7265 6174 6528 2076 6f69  tset_create( voi
-00000290: 6420 293b 0a0a 2f2a 2043 7265 6174 6520  d );../* Create 
-000002a0: 6120 6e65 7720 6269 7473 6574 2061 626c  a new bitset abl
-000002b0: 6520 746f 2063 6f6e 7461 696e 2073 697a  e to contain siz
-000002c0: 6520 6269 7473 2e20 5265 7475 726e 204e  e bits. Return N
-000002d0: 554c 4c20 696e 2063 6173 6520 6f66 2066  ULL in case of f
-000002e0: 6169 6c75 7265 2e20 2a2f 0a62 6974 7365  ailure. */.bitse
-000002f0: 745f 7420 2a62 6974 7365 745f 6372 6561  t_t *bitset_crea
-00000300: 7465 5f77 6974 685f 6361 7061 6369 7479  te_with_capacity
-00000310: 2820 7369 7a65 5f74 2073 697a 6520 293b  ( size_t size );
-00000320: 0a0a 2f2a 2046 7265 6520 6d65 6d6f 7279  ../* Free memory
-00000330: 2e20 2a2f 0a76 6f69 6420 6269 7473 6574  . */.void bitset
-00000340: 5f66 7265 6528 6269 7473 6574 5f74 202a  _free(bitset_t *
-00000350: 6269 7473 6574 293b 0a0a 2f2a 2053 6574  bitset);../* Set
-00000360: 2061 6c6c 2062 6974 7320 746f 207a 6572   all bits to zer
-00000370: 6f2e 202a 2f0a 766f 6964 2062 6974 7365  o. */.void bitse
-00000380: 745f 636c 6561 7228 6269 7473 6574 5f74  t_clear(bitset_t
-00000390: 202a 6269 7473 6574 293b 0a0a 2f2a 2053   *bitset);../* S
-000003a0: 6574 2061 6c6c 2062 6974 7320 746f 206f  et all bits to o
-000003b0: 6e65 2e20 2a2f 0a76 6f69 6420 6269 7473  ne. */.void bits
-000003c0: 6574 5f66 696c 6c28 6269 7473 6574 5f74  et_fill(bitset_t
-000003d0: 202a 6269 7473 6574 293b 0a0a 2f2a 2043   *bitset);../* C
-000003e0: 7265 6174 6520 6120 636f 7079 202a 2f0a  reate a copy */.
-000003f0: 6269 7473 6574 5f74 202a 2062 6974 7365  bitset_t * bitse
-00000400: 745f 636f 7079 2863 6f6e 7374 2062 6974  t_copy(const bit
-00000410: 7365 745f 7420 2a62 6974 7365 7429 3b0a  set_t *bitset);.
-00000420: 0a2f 2a20 466f 7220 6164 7661 6e63 6564  ./* For advanced
-00000430: 2075 7365 7273 3a20 5265 7369 7a65 2074   users: Resize t
-00000440: 6865 2062 6974 7365 7420 736f 2074 6861  he bitset so tha
-00000450: 7420 6974 2063 616e 2073 7570 706f 7274  t it can support
-00000460: 206e 6577 6172 7261 7973 697a 6520 2a20   newarraysize * 
-00000470: 3634 2062 6974 732e 0a20 2a20 5265 7475  64 bits.. * Retu
-00000480: 726e 2074 7275 6520 696e 2063 6173 6520  rn true in case 
-00000490: 6f66 2073 7563 6365 7373 2c20 6661 6c73  of success, fals
-000004a0: 6520 666f 7220 6661 696c 7572 652e 2050  e for failure. P
-000004b0: 6164 0a20 2a20 7769 7468 207a 6572 6f65  ad. * with zeroe
-000004c0: 7320 6e65 7720 6275 6666 6572 2061 7265  s new buffer are
-000004d0: 6173 2069 6620 7265 7175 6573 7465 642e  as if requested.
-000004e0: 202a 2f0a 626f 6f6c 2062 6974 7365 745f   */.bool bitset_
-000004f0: 7265 7369 7a65 2820 6269 7473 6574 5f74  resize( bitset_t
-00000500: 202a 6269 7473 6574 2c20 2073 697a 655f   *bitset,  size_
-00000510: 7420 6e65 7761 7272 6179 7369 7a65 2c20  t newarraysize, 
-00000520: 626f 6f6c 2070 6164 7769 7468 7a65 726f  bool padwithzero
-00000530: 6573 2029 3b0a 0a2f 2a20 7265 7475 726e  es );../* return
-00000540: 7320 686f 7720 6d61 6e79 2062 7974 6573  s how many bytes
-00000550: 206f 6620 6d65 6d6f 7279 2074 6865 2062   of memory the b
-00000560: 6163 6b65 6e64 2062 7566 6665 7220 7573  ackend buffer us
-00000570: 6573 202a 2f0a 7369 7a65 5f74 2062 6974  es */.size_t bit
-00000580: 7365 745f 7369 7a65 5f69 6e5f 6279 7465  set_size_in_byte
-00000590: 7328 636f 6e73 7420 6269 7473 6574 5f74  s(const bitset_t
-000005a0: 202a 6269 7473 6574 293b 0a0a 2f2a 2072   *bitset);../* r
-000005b0: 6574 7572 6e73 2068 6f77 206d 616e 7920  eturns how many 
-000005c0: 6269 7473 2063 616e 2062 6520 6163 6365  bits can be acce
-000005d0: 7373 6564 202a 2f0a 7369 7a65 5f74 2062  ssed */.size_t b
-000005e0: 6974 7365 745f 7369 7a65 5f69 6e5f 6269  itset_size_in_bi
-000005f0: 7473 2863 6f6e 7374 2062 6974 7365 745f  ts(const bitset_
-00000600: 7420 2a62 6974 7365 7429 3b0a 0a2f 2a20  t *bitset);../* 
-00000610: 7265 7475 726e 7320 686f 7720 6d61 6e79  returns how many
-00000620: 2077 6f72 6473 2028 3634 2d62 6974 2920   words (64-bit) 
-00000630: 6f66 206d 656d 6f72 7920 7468 6520 6261  of memory the ba
-00000640: 636b 656e 6420 6275 6666 6572 2075 7365  ckend buffer use
-00000650: 7320 2a2f 0a73 697a 655f 7420 6269 7473  s */.size_t bits
-00000660: 6574 5f73 697a 655f 696e 5f77 6f72 6473  et_size_in_words
-00000670: 2863 6f6e 7374 2062 6974 7365 745f 7420  (const bitset_t 
-00000680: 2a62 6974 7365 7429 3b0a 0a0a 2f2a 2046  *bitset);.../* F
-00000690: 6f72 2061 6476 616e 6365 6420 7573 6572  or advanced user
-000006a0: 733a 2047 726f 7720 7468 6520 6269 7473  s: Grow the bits
-000006b0: 6574 2073 6f20 7468 6174 2069 7420 6361  et so that it ca
-000006c0: 6e20 7375 7070 6f72 7420 6e65 7761 7272  n support newarr
-000006d0: 6179 7369 7a65 202a 2036 3420 6269 7473  aysize * 64 bits
-000006e0: 2077 6974 6820 7061 6464 696e 672e 2052   with padding. R
-000006f0: 6574 7572 6e20 7472 7565 2069 6e20 6361  eturn true in ca
-00000700: 7365 206f 6620 7375 6363 6573 732c 2066  se of success, f
-00000710: 616c 7365 2066 6f72 2066 6169 6c75 7265  alse for failure
-00000720: 2e20 2a2f 0a62 6f6f 6c20 6269 7473 6574  . */.bool bitset
-00000730: 5f67 726f 7728 6269 7473 6574 5f74 202a  _grow(bitset_t *
-00000740: 6269 7473 6574 2c20 2073 697a 655f 7420  bitset,  size_t 
-00000750: 6e65 7761 7272 6179 7369 7a65 293b 0a0a  newarraysize);..
-00000760: 2f2a 2061 7474 656d 7074 7320 746f 2072  /* attempts to r
-00000770: 6563 6f76 6572 2075 6e75 7365 6420 6d65  ecover unused me
-00000780: 6d6f 7279 2c20 7265 7475 726e 2066 616c  mory, return fal
-00000790: 7365 2069 6e20 6361 7365 206f 6620 7265  se in case of re
-000007a0: 616c 6c6f 6361 7469 6f6e 2066 6169 6c75  allocation failu
-000007b0: 7265 202a 2f0a 626f 6f6c 2062 6974 7365  re */.bool bitse
-000007c0: 745f 7472 696d 2862 6974 7365 745f 7420  t_trim(bitset_t 
-000007d0: 2a62 6974 7365 7429 3b0a 0a2f 2a20 7368  *bitset);../* sh
-000007e0: 6966 7473 2061 6c6c 2062 6974 7320 6279  ifts all bits by
-000007f0: 2027 7327 2070 6f73 6974 696f 6e73 2073   's' positions s
-00000800: 6f20 7468 6174 2074 6865 2062 6974 7365  o that the bitse
-00000810: 7420 7265 7072 6573 656e 7469 6e67 2076  t representing v
-00000820: 616c 7565 7320 312c 322c 3130 2077 6f75  alues 1,2,10 wou
-00000830: 6c64 2072 6570 7265 7365 6e74 2076 616c  ld represent val
-00000840: 7565 7320 312b 732c 2032 2b73 2c20 3130  ues 1+s, 2+s, 10
-00000850: 2b73 202a 2f0a 766f 6964 2062 6974 7365  +s */.void bitse
-00000860: 745f 7368 6966 745f 6c65 6674 2862 6974  t_shift_left(bit
-00000870: 7365 745f 7420 2a62 6974 7365 742c 2073  set_t *bitset, s
-00000880: 697a 655f 7420 7329 3b0a 0a2f 2a20 7368  ize_t s);../* sh
-00000890: 6966 7473 2061 6c6c 2062 6974 7320 6279  ifts all bits by
-000008a0: 2027 7327 2070 6f73 6974 696f 6e73 2073   's' positions s
-000008b0: 6f20 7468 6174 2074 6865 2062 6974 7365  o that the bitse
-000008c0: 7420 7265 7072 6573 656e 7469 6e67 2076  t representing v
-000008d0: 616c 7565 7320 312c 322c 3130 2077 6f75  alues 1,2,10 wou
-000008e0: 6c64 2072 6570 7265 7365 6e74 2076 616c  ld represent val
-000008f0: 7565 7320 312d 732c 2032 2d73 2c20 3130  ues 1-s, 2-s, 10
-00000900: 2d73 2c20 6e65 6761 7469 7665 2076 616c  -s, negative val
-00000910: 7565 7320 6172 6520 6465 6c65 7465 6420  ues are deleted 
-00000920: 2a2f 0a76 6f69 6420 6269 7473 6574 5f73  */.void bitset_s
-00000930: 6869 6674 5f72 6967 6874 2862 6974 7365  hift_right(bitse
-00000940: 745f 7420 2a62 6974 7365 742c 2073 697a  t_t *bitset, siz
-00000950: 655f 7420 7329 3b0a 0a2f 2a20 5365 7420  e_t s);../* Set 
-00000960: 7468 6520 6974 6820 6269 742e 2041 7474  the ith bit. Att
-00000970: 656d 7074 7320 746f 2072 6573 697a 6520  empts to resize 
-00000980: 7468 6520 6269 7473 6574 2069 6620 6e65  the bitset if ne
-00000990: 6564 6564 2028 6d61 7920 7369 6c65 6e74  eded (may silent
-000009a0: 6c79 2066 6169 6c29 202a 2f0a 766f 6964  ly fail) */.void
-000009b0: 2062 6974 7365 745f 7365 7428 6269 7473   bitset_set(bits
-000009c0: 6574 5f74 202a 6269 7473 6574 2c20 2073  et_t *bitset,  s
-000009d0: 697a 655f 7420 6929 3b0a 0a2f 2a20 5365  ize_t i);../* Se
-000009e0: 7420 7468 6520 6974 6820 6269 7420 746f  t the ith bit to
-000009f0: 2074 6865 2073 7065 6369 6669 6564 2076   the specified v
-00000a00: 616c 7565 2e20 4174 7465 6d70 7473 2074  alue. Attempts t
-00000a10: 6f20 7265 7369 7a65 2074 6865 2062 6974  o resize the bit
-00000a20: 7365 7420 6966 206e 6565 6465 6420 286d  set if needed (m
-00000a30: 6179 2073 696c 656e 746c 7920 6661 696c  ay silently fail
-00000a40: 2920 2a2f 0a76 6f69 6420 6269 7473 6574  ) */.void bitset
-00000a50: 5f73 6574 5f74 6f5f 7661 6c75 6528 6269  _set_to_value(bi
-00000a60: 7473 6574 5f74 202a 6269 7473 6574 2c20  tset_t *bitset, 
-00000a70: 2073 697a 655f 7420 692c 2062 6f6f 6c20   size_t i, bool 
-00000a80: 666c 6167 293b 0a0a 0a0a 0a2f 2a20 4765  flag);...../* Ge
-00000a90: 7420 7468 6520 7661 6c75 6520 6f66 2074  t the value of t
-00000aa0: 6865 2069 7468 2062 6974 2e20 202a 2f0a  he ith bit.  */.
-00000ab0: 626f 6f6c 2062 6974 7365 745f 6765 7428  bool bitset_get(
-00000ac0: 636f 6e73 7420 6269 7473 6574 5f74 202a  const bitset_t *
-00000ad0: 6269 7473 6574 2c20 2073 697a 655f 7420  bitset,  size_t 
-00000ae0: 6920 293b 0a0a 2f2a 2043 6f75 6e74 206e  i );../* Count n
-00000af0: 756d 6265 7220 6f66 2062 6974 7320 7365  umber of bits se
-00000b00: 742e 2020 2a2f 0a73 697a 655f 7420 6269  t.  */.size_t bi
-00000b10: 7473 6574 5f63 6f75 6e74 2863 6f6e 7374  tset_count(const
-00000b20: 2062 6974 7365 745f 7420 2a62 6974 7365   bitset_t *bitse
-00000b30: 7429 3b0a 0a2f 2a20 4669 6e64 2074 6865  t);../* Find the
-00000b40: 2069 6e64 6578 206f 6620 7468 6520 6669   index of the fi
-00000b50: 7273 7420 6269 7420 7365 742e 204f 7220  rst bit set. Or 
-00000b60: 7a65 726f 2069 6620 7468 6520 6269 7473  zero if the bits
-00000b70: 6574 2069 7320 656d 7074 792e 2020 2a2f  et is empty.  */
-00000b80: 0a73 697a 655f 7420 6269 7473 6574 5f6d  .size_t bitset_m
-00000b90: 696e 696d 756d 2863 6f6e 7374 2062 6974  inimum(const bit
-00000ba0: 7365 745f 7420 2a62 6974 7365 7429 3b0a  set_t *bitset);.
-00000bb0: 0a2f 2a20 4669 6e64 2074 6865 2069 6e64  ./* Find the ind
-00000bc0: 6578 206f 6620 7468 6520 6c61 7374 2062  ex of the last b
-00000bd0: 6974 2073 6574 2e20 4f72 207a 6572 6f20  it set. Or zero 
-00000be0: 6966 2074 6865 2062 6974 7365 7420 6973  if the bitset is
-00000bf0: 2065 6d70 7479 2e20 2a2f 0a73 697a 655f   empty. */.size_
-00000c00: 7420 6269 7473 6574 5f6d 6178 696d 756d  t bitset_maximum
-00000c10: 2863 6f6e 7374 2062 6974 7365 745f 7420  (const bitset_t 
-00000c20: 2a62 6974 7365 7429 3b0a 0a0a 2f2a 2063  *bitset);.../* c
-00000c30: 6f6d 7075 7465 2074 6865 2075 6e69 6f6e  ompute the union
-00000c40: 2069 6e2d 706c 6163 6520 2874 6f20 6231   in-place (to b1
-00000c50: 292c 2072 6574 7572 6e73 2074 7275 6520  ), returns true 
-00000c60: 6966 2073 7563 6365 7373 6675 6c2c 2074  if successful, t
-00000c70: 6f20 6765 6e65 7261 7465 2061 206e 6577  o generate a new
-00000c80: 2062 6974 7365 7420 6669 7273 7420 6361   bitset first ca
-00000c90: 6c6c 2062 6974 7365 745f 636f 7079 202a  ll bitset_copy *
-00000ca0: 2f0a 626f 6f6c 2062 6974 7365 745f 696e  /.bool bitset_in
-00000cb0: 706c 6163 655f 756e 696f 6e28 6269 7473  place_union(bits
-00000cc0: 6574 5f74 202a 2062 312c 2063 6f6e 7374  et_t * b1, const
-00000cd0: 2062 6974 7365 745f 7420 2a20 6232 293b   bitset_t * b2);
-00000ce0: 0a0a 2f2a 2072 6570 6f72 7420 7468 6520  ../* report the 
-00000cf0: 7369 7a65 206f 6620 7468 6520 756e 696f  size of the unio
-00000d00: 6e20 2877 6974 686f 7574 206d 6174 6572  n (without mater
-00000d10: 6961 6c69 7a69 6e67 2069 7429 202a 2f0a  ializing it) */.
-00000d20: 7369 7a65 5f74 2062 6974 7365 745f 756e  size_t bitset_un
-00000d30: 696f 6e5f 636f 756e 7428 636f 6e73 7420  ion_count(const 
-00000d40: 6269 7473 6574 5f74 202a 2062 312c 2063  bitset_t * b1, c
-00000d50: 6f6e 7374 2062 6974 7365 745f 7420 2a20  onst bitset_t * 
-00000d60: 6232 293b 0a0a 2f2a 2063 6f6d 7075 7465  b2);../* compute
-00000d70: 2074 6865 2069 6e74 6572 7365 6374 696f   the intersectio
-00000d80: 6e20 696e 2d70 6c61 6365 2028 746f 2062  n in-place (to b
-00000d90: 3129 2c20 746f 2067 656e 6572 6174 6520  1), to generate 
-00000da0: 6120 6e65 7720 6269 7473 6574 2066 6972  a new bitset fir
-00000db0: 7374 2063 616c 6c20 6269 7473 6574 5f63  st call bitset_c
-00000dc0: 6f70 7920 2a2f 0a76 6f69 6420 6269 7473  opy */.void bits
-00000dd0: 6574 5f69 6e70 6c61 6365 5f69 6e74 6572  et_inplace_inter
-00000de0: 7365 6374 696f 6e28 6269 7473 6574 5f74  section(bitset_t
-00000df0: 202a 2062 312c 2063 6f6e 7374 2062 6974   * b1, const bit
-00000e00: 7365 745f 7420 2a20 6232 293b 0a0a 2f2a  set_t * b2);../*
-00000e10: 2052 6570 6f72 7420 7468 6520 7369 7a65   Report the size
-00000e20: 206f 6620 7468 6520 696e 7465 7273 6563   of the intersec
-00000e30: 7469 6f6e 2028 7769 7468 6f75 7420 6d61  tion (without ma
-00000e40: 7465 7269 616c 697a 696e 6720 6974 292e  terializing it).
-00000e50: 0a20 2a20 5765 2061 7373 756d 6520 7468  . * We assume th
-00000e60: 6174 2074 6865 2062 6974 7365 7473 2062  at the bitsets b
-00000e70: 3120 616e 6420 6232 2061 7265 2064 6973  1 and b2 are dis
-00000e80: 7469 6e63 742e 202a 2f0a 7369 7a65 5f74  tinct. */.size_t
-00000e90: 2062 6974 7365 745f 696e 7465 7273 6563   bitset_intersec
-00000ea0: 7469 6f6e 5f63 6f75 6e74 2863 6f6e 7374  tion_count(const
-00000eb0: 2062 6974 7365 745f 7420 2a20 6231 2c20   bitset_t * b1, 
-00000ec0: 636f 6e73 7420 6269 7473 6574 5f74 202a  const bitset_t *
-00000ed0: 2062 3229 3b0a 0a0a 2f2a 2072 6574 7572   b2);.../* retur
-00000ee0: 6e73 2074 7275 6520 6966 2074 6865 2062  ns true if the b
-00000ef0: 6974 7365 7473 2063 6f6e 7461 696e 206e  itsets contain n
-00000f00: 6f20 636f 6d6d 6f6e 2065 6c65 6d65 6e74  o common element
-00000f10: 7320 2a2f 0a62 6f6f 6c20 6269 7473 6574  s */.bool bitset
-00000f20: 735f 6469 736a 6f69 6e74 2863 6f6e 7374  s_disjoint(const
-00000f30: 2062 6974 7365 745f 7420 2a20 6231 2c20   bitset_t * b1, 
-00000f40: 636f 6e73 7420 6269 7473 6574 5f74 202a  const bitset_t *
-00000f50: 2062 3229 3b0a 0a2f 2a20 7265 7475 726e   b2);../* return
-00000f60: 7320 7472 7565 2069 6620 7468 6520 6269  s true if the bi
-00000f70: 7473 6574 7320 636f 6e74 6169 6e20 616e  tsets contain an
-00000f80: 7920 636f 6d6d 6f6e 2065 6c65 6d65 6e74  y common element
-00000f90: 7320 2a2f 0a62 6f6f 6c20 6269 7473 6574  s */.bool bitset
-00000fa0: 735f 696e 7465 7273 6563 7428 636f 6e73  s_intersect(cons
-00000fb0: 7420 6269 7473 6574 5f74 202a 2062 312c  t bitset_t * b1,
-00000fc0: 2063 6f6e 7374 2062 6974 7365 745f 7420   const bitset_t 
-00000fd0: 2a20 6232 293b 0a0a 2f2a 2072 6574 7572  * b2);../* retur
-00000fe0: 6e73 2074 7275 6520 6966 2062 3120 636f  ns true if b1 co
-00000ff0: 6e74 6169 6e73 2061 6c6c 206f 6620 7468  ntains all of th
-00001000: 6520 7365 7420 6269 7473 206f 6620 6232  e set bits of b2
-00001010: 202a 2f0a 626f 6f6c 2062 6974 7365 745f   */.bool bitset_
-00001020: 636f 6e74 6169 6e73 5f61 6c6c 2863 6f6e  contains_all(con
-00001030: 7374 2062 6974 7365 745f 7420 2a20 6231  st bitset_t * b1
-00001040: 2c20 636f 6e73 7420 6269 7473 6574 5f74  , const bitset_t
-00001050: 202a 2062 3229 3b0a 0a0a 2f2a 2063 6f6d   * b2);.../* com
-00001060: 7075 7465 2074 6865 2064 6966 6665 7265  pute the differe
-00001070: 6e63 6520 696e 2d70 6c61 6365 2028 746f  nce in-place (to
-00001080: 2062 3129 2c20 746f 2067 656e 6572 6174   b1), to generat
-00001090: 6520 6120 6e65 7720 6269 7473 6574 2066  e a new bitset f
-000010a0: 6972 7374 2063 616c 6c20 6269 7473 6574  irst call bitset
-000010b0: 5f63 6f70 7920 2a2f 0a76 6f69 6420 6269  _copy */.void bi
-000010c0: 7473 6574 5f69 6e70 6c61 6365 5f64 6966  tset_inplace_dif
-000010d0: 6665 7265 6e63 6528 6269 7473 6574 5f74  ference(bitset_t
-000010e0: 202a 2062 312c 2063 6f6e 7374 2062 6974   * b1, const bit
-000010f0: 7365 745f 7420 2a20 6232 293b 0a0a 2f2a  set_t * b2);../*
-00001100: 2063 6f6d 7075 7465 2074 6865 2073 697a   compute the siz
-00001110: 6520 6f66 2074 6865 2064 6966 6665 7265  e of the differe
-00001120: 6e63 6520 2a2f 0a73 697a 655f 7420 2062  nce */.size_t  b
-00001130: 6974 7365 745f 6469 6666 6572 656e 6365  itset_difference
-00001140: 5f63 6f75 6e74 2863 6f6e 7374 2062 6974  _count(const bit
-00001150: 7365 745f 7420 2a20 6231 2c20 636f 6e73  set_t * b1, cons
-00001160: 7420 6269 7473 6574 5f74 202a 2062 3229  t bitset_t * b2)
-00001170: 203b 0a0a 2f2a 2063 6f6d 7075 7465 2074   ;../* compute t
-00001180: 6865 2073 796d 6d65 7472 6963 2064 6966  he symmetric dif
-00001190: 6665 7265 6e63 6520 696e 2d70 6c61 6365  ference in-place
-000011a0: 2028 746f 2062 3129 2c20 7265 7475 726e   (to b1), return
-000011b0: 2074 7275 6520 6966 2073 7563 6365 7373   true if success
-000011c0: 6675 6c2c 2074 6f20 6765 6e65 7261 7465  ful, to generate
-000011d0: 2061 206e 6577 2062 6974 7365 7420 6669   a new bitset fi
-000011e0: 7273 7420 6361 6c6c 2062 6974 7365 745f  rst call bitset_
-000011f0: 636f 7079 202a 2f0a 626f 6f6c 2062 6974  copy */.bool bit
-00001200: 7365 745f 696e 706c 6163 655f 7379 6d6d  set_inplace_symm
-00001210: 6574 7269 635f 6469 6666 6572 656e 6365  etric_difference
-00001220: 2862 6974 7365 745f 7420 2a20 6231 2c20  (bitset_t * b1, 
-00001230: 636f 6e73 7420 6269 7473 6574 5f74 202a  const bitset_t *
-00001240: 2062 3229 3b0a 0a2f 2a20 636f 6d70 7574   b2);../* comput
-00001250: 6520 7468 6520 7369 7a65 206f 6620 7468  e the size of th
-00001260: 6520 7379 6d6d 6574 7269 6320 6469 6666  e symmetric diff
-00001270: 6572 656e 6365 2020 2a2f 0a73 697a 655f  erence  */.size_
-00001280: 7420 2062 6974 7365 745f 7379 6d6d 6574  t  bitset_symmet
-00001290: 7269 635f 6469 6666 6572 656e 6365 5f63  ric_difference_c
-000012a0: 6f75 6e74 2863 6f6e 7374 2062 6974 7365  ount(const bitse
-000012b0: 745f 7420 2a20 6231 2c20 636f 6e73 7420  t_t * b1, const 
-000012c0: 6269 7473 6574 5f74 202a 2062 3229 3b0a  bitset_t * b2);.
-000012d0: 0a2f 2a20 6974 6572 6174 6520 6f76 6572  ./* iterate over
-000012e0: 2074 6865 2073 6574 2062 6974 730a 206c   the set bits. l
-000012f0: 696b 6520 736f 203a 0a20 2066 6f72 2873  ike so :.  for(s
-00001300: 697a 655f 7420 6920 3d20 303b 2062 6974  ize_t i = 0; bit
-00001310: 7365 745f 6e65 7874 5f73 6574 5f62 6974  set_next_set_bit
-00001320: 2862 2c26 6929 203b 2069 2b2b 2920 7b0a  (b,&i) ; i++) {.
-00001330: 2020 2020 2f2f 2e2e 2e2e 2e0a 2020 7d0a      //......  }.
-00001340: 2020 2a2f 0a62 6f6f 6c20 6269 7473 6574    */.bool bitset
-00001350: 5f6e 6578 745f 7365 745f 6269 7428 636f  _next_set_bit(co
-00001360: 6e73 7420 6269 7473 6574 5f74 202a 6269  nst bitset_t *bi
-00001370: 7473 6574 2c20 7369 7a65 5f74 202a 6929  tset, size_t *i)
-00001380: 3b0a 2f2a 2069 7465 7261 7465 206f 7665  ;./* iterate ove
-00001390: 7220 7468 6520 7365 7420 6269 7473 0a20  r the set bits. 
-000013a0: 6c69 6b65 2073 6f20 3a0a 2020 2073 697a  like so :.   siz
-000013b0: 655f 7420 6275 6666 6572 5b32 3536 5d3b  e_t buffer[256];
-000013c0: 0a20 2020 7369 7a65 5f74 2068 6f77 6d61  .   size_t howma
-000013d0: 6e79 203d 2030 3b0a 2020 666f 7228 7369  ny = 0;.  for(si
-000013e0: 7a65 5f74 2073 7461 7274 6672 6f6d 203d  ze_t startfrom =
-000013f0: 2030 3b20 2868 6f77 6d61 6e79 203d 2062   0; (howmany = b
-00001400: 6974 7365 745f 6e65 7874 5f73 6574 5f62  itset_next_set_b
-00001410: 6974 7328 622c 6275 6666 6572 2c32 3536  its(b,buffer,256
-00001420: 2c20 2673 7461 7274 6672 6f6d 2929 203e  , &startfrom)) >
-00001430: 2030 203b 2073 7461 7274 6672 6f6d 2b2b   0 ; startfrom++
-00001440: 2920 7b0a 2020 2020 2f2f 2e2e 2e2e 2e0a  ) {.    //......
-00001450: 2020 7d0a 2020 2a2f 0a73 697a 655f 7420    }.  */.size_t 
-00001460: 6269 7473 6574 5f6e 6578 745f 7365 745f  bitset_next_set_
-00001470: 6269 7473 2863 6f6e 7374 2062 6974 7365  bits(const bitse
-00001480: 745f 7420 2a62 6974 7365 742c 2073 697a  t_t *bitset, siz
-00001490: 655f 7420 2a62 7566 6665 722c 2073 697a  e_t *buffer, siz
-000014a0: 655f 7420 6361 7061 6369 7479 2c20 7369  e_t capacity, si
-000014b0: 7a65 5f74 202a 2073 7461 7274 6672 6f6d  ze_t * startfrom
-000014c0: 293b 0a0a 7479 7065 6465 6620 626f 6f6c  );..typedef bool
-000014d0: 2028 2a62 6974 7365 745f 6974 6572 6174   (*bitset_iterat
-000014e0: 6f72 2928 7369 7a65 5f74 2076 616c 7565  or)(size_t value
-000014f0: 2c20 766f 6964 202a 7061 7261 6d29 3b0a  , void *param);.
-00001500: 0a2f 2f20 7265 7475 726e 2074 7275 6520  .// return true 
-00001510: 6966 2075 6e69 6e74 6572 7275 7074 6564  if uninterrupted
-00001520: 0a62 6f6f 6c20 6269 7473 6574 5f66 6f72  .bool bitset_for
-00001530: 5f65 6163 6828 636f 6e73 7420 6269 7473  _each(const bits
-00001540: 6574 5f74 202a 622c 2062 6974 7365 745f  et_t *b, bitset_
-00001550: 6974 6572 6174 6f72 2069 7465 7261 746f  iterator iterato
-00001560: 722c 2076 6f69 6420 2a70 7472 293b 200a  r, void *ptr); .
-00001570: 766f 6964 2062 6974 7365 745f 7072 696e  void bitset_prin
-00001580: 7428 636f 6e73 7420 6269 7473 6574 5f74  t(const bitset_t
-00001590: 202a 6229 3b0a 0a65 7874 6572 6e20 2250   *b);..extern "P
-000015a0: 7974 686f 6e22 2062 6f6f 6c20 6269 7473  ython" bool bits
-000015b0: 6574 5f69 7465 7261 746f 725f 6675 6e63  et_iterator_func
-000015c0: 2873 697a 655f 7420 7661 6c75 652c 2076  (size_t value, v
-000015d0: 6f69 642a 2070 6172 616d 293b 0a20 2020  oid* param);.   
-000015e0: 207a 8c0a 2369 6e63 6c75 6465 203c 7374   z..#include <st
-000015f0: 6469 6f2e 683e 0a23 696e 636c 7564 6520  dio.h>.#include 
-00001600: 3c73 7464 6c69 622e 683e 0a23 696e 636c  <stdlib.h>.#incl
-00001610: 7564 6520 3c73 7464 696e 742e 683e 0a23  ude <stdint.h>.#
-00001620: 696e 636c 7564 6520 3c73 7464 626f 6f6c  include <stdbool
-00001630: 2e68 3e0a 2369 6e63 6c75 6465 203c 7374  .h>.#include <st
-00001640: 6469 6f2e 683e 0a23 696e 636c 7564 6520  dio.h>.#include 
-00001650: 3c73 7472 696e 672e 683e 0a23 696e 636c  <string.h>.#incl
-00001660: 7564 6520 2262 6974 7365 742e 6822 0a7a  ude "bitset.h".z
-00001670: 112e 2f63 6269 7473 6574 2f73 7263 2f2a  ../cbitset/src/*
-00001680: 2e63 7a1e 7079 6269 7473 6574 2e62 6163  .cz.pybitset.bac
-00001690: 6b65 6e64 732e 6366 6669 2e5f 6269 7473  kends.cffi._bits
-000016a0: 6574 7a11 2e2f 6362 6974 7365 742f 696e  etz../cbitset/in
-000016b0: 636c 7564 6529 02da 0773 6f75 7263 6573  clude)...sources
-000016c0: da0c 696e 636c 7564 655f 6469 7273 da08  ..include_dirs..
-000016d0: 5f5f 6d61 696e 5f5f 290c da07 5f5f 646f  __main__)...__do
-000016e0: 635f 5fda 0467 6c6f 62da 0463 6666 6972  c__..glob..cffir
-000016f0: 0200 0000 5a0a 6666 6962 7569 6c64 6572  ....Z.ffibuilder
-00001700: da04 6364 6566 da06 736f 7572 6365 5a09  ..cdef..sourceZ.
-00001710: 635f 736f 7572 6365 73da 0570 7269 6e74  c_sources..print
-00001720: 5a0a 7365 745f 736f 7572 6365 da08 5f5f  Z.set_source..__
-00001730: 6e61 6d65 5f5f da07 636f 6d70 696c 65a9  name__..compile.
-00001740: 0072 0e00 0000 720e 0000 00fa 3545 3a5c  .r....r.....5E:\
-00001750: 7079 7072 6f6a 6563 745c 7079 6269 7473  pyproject\pybits
-00001760: 6574 5c70 7962 6974 7365 745c 6261 636b  et\pybitset\back
-00001770: 656e 6473 5c63 6666 695c 6275 696c 642e  ends\cffi\build.
-00001780: 7079 da08 3c6d 6f64 756c 653e 0100 0000  py..<module>....
-00001790: 7328 0000 0004 0008 030c 0206 0204 0102  s(..............
-000017a0: 0104 ff00 7f04 100a 0908 0204 0202 0102  ................
-000017b0: 0102 0104 0106 fc08 070c 0104 ff         .............
+00000000: 2222 220a 436f 7079 7269 6768 7420 2863  """.Copyright (c
+00000010: 2920 3230 3038 2d32 3032 3320 7379 6e6f  ) 2008-2023 syno
+00000020: 6472 6976 6572 203c 6469 6775 6f68 7561  driver <diguohua
+00000030: 6e67 6a69 616a 696e 7765 696a 756e 4067  ngjiajinweijun@g
+00000040: 6d61 696c 2e63 6f6d 3e0a 2222 220a 696d  mail.com>.""".im
+00000050: 706f 7274 2067 6c6f 620a 0a66 726f 6d20  port glob..from 
+00000060: 6366 6669 2069 6d70 6f72 7420 4646 490a  cffi import FFI.
+00000070: 0a66 6669 6275 696c 6465 7220 3d20 4646  .ffibuilder = FF
+00000080: 4928 290a 6666 6962 7569 6c64 6572 2e63  I().ffibuilder.c
+00000090: 6465 6628 0a20 2020 2022 2222 0a73 7472  def(.    """.str
+000000a0: 7563 7420 6269 7473 6574 5f73 207b 0a20  uct bitset_s {. 
+000000b0: 2020 2075 696e 7436 345f 7420 2a20 6172     uint64_t * ar
+000000c0: 7261 793b 0a20 2020 202f 2a20 466f 7220  ray;.    /* For 
+000000d0: 7369 6d70 6c69 6369 7479 2061 6e64 2070  simplicity and p
+000000e0: 6572 666f 726d 616e 6365 2c20 7765 2070  erformance, we p
+000000f0: 7265 6665 7220 746f 2068 6176 6520 6120  refer to have a 
+00000100: 7369 7a65 2061 6e64 2061 2063 6170 6163  size and a capac
+00000110: 6974 7920 7468 6174 2069 7320 6120 6d75  ity that is a mu
+00000120: 6c74 6970 6c65 206f 6620 3634 2062 6974  ltiple of 64 bit
+00000130: 732e 0a20 2020 2020 2a20 5468 7573 2077  s..     * Thus w
+00000140: 6520 6f6e 6c79 2074 7261 636b 2074 6865  e only track the
+00000150: 2073 697a 6520 616e 6420 7468 6520 6361   size and the ca
+00000160: 7061 6369 7479 2069 6e20 7465 726d 7320  pacity in terms 
+00000170: 6f66 2036 342d 6269 7420 776f 7264 7320  of 64-bit words 
+00000180: 616c 6c6f 6361 7465 6420 2a2f 0a20 2020  allocated */.   
+00000190: 2073 697a 655f 7420 6172 7261 7973 697a   size_t arraysiz
+000001a0: 653b 0a20 2020 2073 697a 655f 7420 6361  e;.    size_t ca
+000001b0: 7061 6369 7479 3b0a 0a7d 3b0a 0a74 7970  pacity;..};..typ
+000001c0: 6564 6566 2073 7472 7563 7420 6269 7473  edef struct bits
+000001d0: 6574 5f73 2062 6974 7365 745f 743b 0a0a  et_s bitset_t;..
+000001e0: 2f2a 2043 7265 6174 6520 6120 6e65 7720  /* Create a new 
+000001f0: 6269 7473 6574 2e20 5265 7475 726e 204e  bitset. Return N
+00000200: 554c 4c20 696e 2063 6173 6520 6f66 2066  ULL in case of f
+00000210: 6169 6c75 7265 2e20 2a2f 0a62 6974 7365  ailure. */.bitse
+00000220: 745f 7420 2a62 6974 7365 745f 6372 6561  t_t *bitset_crea
+00000230: 7465 2820 766f 6964 2029 3b0a 0a2f 2a20  te( void );../* 
+00000240: 4372 6561 7465 2061 206e 6577 2062 6974  Create a new bit
+00000250: 7365 7420 6162 6c65 2074 6f20 636f 6e74  set able to cont
+00000260: 6169 6e20 7369 7a65 2062 6974 732e 2052  ain size bits. R
+00000270: 6574 7572 6e20 4e55 4c4c 2069 6e20 6361  eturn NULL in ca
+00000280: 7365 206f 6620 6661 696c 7572 652e 202a  se of failure. *
+00000290: 2f0a 6269 7473 6574 5f74 202a 6269 7473  /.bitset_t *bits
+000002a0: 6574 5f63 7265 6174 655f 7769 7468 5f63  et_create_with_c
+000002b0: 6170 6163 6974 7928 2073 697a 655f 7420  apacity( size_t 
+000002c0: 7369 7a65 2029 3b0a 0a2f 2a20 4672 6565  size );../* Free
+000002d0: 206d 656d 6f72 792e 202a 2f0a 766f 6964   memory. */.void
+000002e0: 2062 6974 7365 745f 6672 6565 2862 6974   bitset_free(bit
+000002f0: 7365 745f 7420 2a62 6974 7365 7429 3b0a  set_t *bitset);.
+00000300: 0a2f 2a20 5365 7420 616c 6c20 6269 7473  ./* Set all bits
+00000310: 2074 6f20 7a65 726f 2e20 2a2f 0a76 6f69   to zero. */.voi
+00000320: 6420 6269 7473 6574 5f63 6c65 6172 2862  d bitset_clear(b
+00000330: 6974 7365 745f 7420 2a62 6974 7365 7429  itset_t *bitset)
+00000340: 3b0a 0a2f 2a20 5365 7420 616c 6c20 6269  ;../* Set all bi
+00000350: 7473 2074 6f20 6f6e 652e 202a 2f0a 766f  ts to one. */.vo
+00000360: 6964 2062 6974 7365 745f 6669 6c6c 2862  id bitset_fill(b
+00000370: 6974 7365 745f 7420 2a62 6974 7365 7429  itset_t *bitset)
+00000380: 3b0a 0a2f 2a20 4372 6561 7465 2061 2063  ;../* Create a c
+00000390: 6f70 7920 2a2f 0a62 6974 7365 745f 7420  opy */.bitset_t 
+000003a0: 2a20 6269 7473 6574 5f63 6f70 7928 636f  * bitset_copy(co
+000003b0: 6e73 7420 6269 7473 6574 5f74 202a 6269  nst bitset_t *bi
+000003c0: 7473 6574 293b 0a0a 2f2a 2046 6f72 2061  tset);../* For a
+000003d0: 6476 616e 6365 6420 7573 6572 733a 2052  dvanced users: R
+000003e0: 6573 697a 6520 7468 6520 6269 7473 6574  esize the bitset
+000003f0: 2073 6f20 7468 6174 2069 7420 6361 6e20   so that it can 
+00000400: 7375 7070 6f72 7420 6e65 7761 7272 6179  support newarray
+00000410: 7369 7a65 202a 2036 3420 6269 7473 2e0a  size * 64 bits..
+00000420: 202a 2052 6574 7572 6e20 7472 7565 2069   * Return true i
+00000430: 6e20 6361 7365 206f 6620 7375 6363 6573  n case of succes
+00000440: 732c 2066 616c 7365 2066 6f72 2066 6169  s, false for fai
+00000450: 6c75 7265 2e20 5061 640a 202a 2077 6974  lure. Pad. * wit
+00000460: 6820 7a65 726f 6573 206e 6577 2062 7566  h zeroes new buf
+00000470: 6665 7220 6172 6561 7320 6966 2072 6571  fer areas if req
+00000480: 7565 7374 6564 2e20 2a2f 0a62 6f6f 6c20  uested. */.bool 
+00000490: 6269 7473 6574 5f72 6573 697a 6528 2062  bitset_resize( b
+000004a0: 6974 7365 745f 7420 2a62 6974 7365 742c  itset_t *bitset,
+000004b0: 2020 7369 7a65 5f74 206e 6577 6172 7261    size_t newarra
+000004c0: 7973 697a 652c 2062 6f6f 6c20 7061 6477  ysize, bool padw
+000004d0: 6974 687a 6572 6f65 7320 293b 0a0a 2f2a  ithzeroes );../*
+000004e0: 2072 6574 7572 6e73 2068 6f77 206d 616e   returns how man
+000004f0: 7920 6279 7465 7320 6f66 206d 656d 6f72  y bytes of memor
+00000500: 7920 7468 6520 6261 636b 656e 6420 6275  y the backend bu
+00000510: 6666 6572 2075 7365 7320 2a2f 0a73 697a  ffer uses */.siz
+00000520: 655f 7420 6269 7473 6574 5f73 697a 655f  e_t bitset_size_
+00000530: 696e 5f62 7974 6573 2863 6f6e 7374 2062  in_bytes(const b
+00000540: 6974 7365 745f 7420 2a62 6974 7365 7429  itset_t *bitset)
+00000550: 3b0a 0a2f 2a20 7265 7475 726e 7320 686f  ;../* returns ho
+00000560: 7720 6d61 6e79 2062 6974 7320 6361 6e20  w many bits can 
+00000570: 6265 2061 6363 6573 7365 6420 2a2f 0a73  be accessed */.s
+00000580: 697a 655f 7420 6269 7473 6574 5f73 697a  ize_t bitset_siz
+00000590: 655f 696e 5f62 6974 7328 636f 6e73 7420  e_in_bits(const 
+000005a0: 6269 7473 6574 5f74 202a 6269 7473 6574  bitset_t *bitset
+000005b0: 293b 0a0a 2f2a 2072 6574 7572 6e73 2068  );../* returns h
+000005c0: 6f77 206d 616e 7920 776f 7264 7320 2836  ow many words (6
+000005d0: 342d 6269 7429 206f 6620 6d65 6d6f 7279  4-bit) of memory
+000005e0: 2074 6865 2062 6163 6b65 6e64 2062 7566   the backend buf
+000005f0: 6665 7220 7573 6573 202a 2f0a 7369 7a65  fer uses */.size
+00000600: 5f74 2062 6974 7365 745f 7369 7a65 5f69  _t bitset_size_i
+00000610: 6e5f 776f 7264 7328 636f 6e73 7420 6269  n_words(const bi
+00000620: 7473 6574 5f74 202a 6269 7473 6574 293b  tset_t *bitset);
+00000630: 0a0a 0a2f 2a20 466f 7220 6164 7661 6e63  .../* For advanc
+00000640: 6564 2075 7365 7273 3a20 4772 6f77 2074  ed users: Grow t
+00000650: 6865 2062 6974 7365 7420 736f 2074 6861  he bitset so tha
+00000660: 7420 6974 2063 616e 2073 7570 706f 7274  t it can support
+00000670: 206e 6577 6172 7261 7973 697a 6520 2a20   newarraysize * 
+00000680: 3634 2062 6974 7320 7769 7468 2070 6164  64 bits with pad
+00000690: 6469 6e67 2e20 5265 7475 726e 2074 7275  ding. Return tru
+000006a0: 6520 696e 2063 6173 6520 6f66 2073 7563  e in case of suc
+000006b0: 6365 7373 2c20 6661 6c73 6520 666f 7220  cess, false for 
+000006c0: 6661 696c 7572 652e 202a 2f0a 626f 6f6c  failure. */.bool
+000006d0: 2062 6974 7365 745f 6772 6f77 2862 6974   bitset_grow(bit
+000006e0: 7365 745f 7420 2a62 6974 7365 742c 2020  set_t *bitset,  
+000006f0: 7369 7a65 5f74 206e 6577 6172 7261 7973  size_t newarrays
+00000700: 697a 6529 3b0a 0a2f 2a20 6174 7465 6d70  ize);../* attemp
+00000710: 7473 2074 6f20 7265 636f 7665 7220 756e  ts to recover un
+00000720: 7573 6564 206d 656d 6f72 792c 2072 6574  used memory, ret
+00000730: 7572 6e20 6661 6c73 6520 696e 2063 6173  urn false in cas
+00000740: 6520 6f66 2072 6561 6c6c 6f63 6174 696f  e of reallocatio
+00000750: 6e20 6661 696c 7572 6520 2a2f 0a62 6f6f  n failure */.boo
+00000760: 6c20 6269 7473 6574 5f74 7269 6d28 6269  l bitset_trim(bi
+00000770: 7473 6574 5f74 202a 6269 7473 6574 293b  tset_t *bitset);
+00000780: 0a0a 2f2a 2073 6869 6674 7320 616c 6c20  ../* shifts all 
+00000790: 6269 7473 2062 7920 2773 2720 706f 7369  bits by 's' posi
+000007a0: 7469 6f6e 7320 736f 2074 6861 7420 7468  tions so that th
+000007b0: 6520 6269 7473 6574 2072 6570 7265 7365  e bitset represe
+000007c0: 6e74 696e 6720 7661 6c75 6573 2031 2c32  nting values 1,2
+000007d0: 2c31 3020 776f 756c 6420 7265 7072 6573  ,10 would repres
+000007e0: 656e 7420 7661 6c75 6573 2031 2b73 2c20  ent values 1+s, 
+000007f0: 322b 732c 2031 302b 7320 2a2f 0a76 6f69  2+s, 10+s */.voi
+00000800: 6420 6269 7473 6574 5f73 6869 6674 5f6c  d bitset_shift_l
+00000810: 6566 7428 6269 7473 6574 5f74 202a 6269  eft(bitset_t *bi
+00000820: 7473 6574 2c20 7369 7a65 5f74 2073 293b  tset, size_t s);
+00000830: 0a0a 2f2a 2073 6869 6674 7320 616c 6c20  ../* shifts all 
+00000840: 6269 7473 2062 7920 2773 2720 706f 7369  bits by 's' posi
+00000850: 7469 6f6e 7320 736f 2074 6861 7420 7468  tions so that th
+00000860: 6520 6269 7473 6574 2072 6570 7265 7365  e bitset represe
+00000870: 6e74 696e 6720 7661 6c75 6573 2031 2c32  nting values 1,2
+00000880: 2c31 3020 776f 756c 6420 7265 7072 6573  ,10 would repres
+00000890: 656e 7420 7661 6c75 6573 2031 2d73 2c20  ent values 1-s, 
+000008a0: 322d 732c 2031 302d 732c 206e 6567 6174  2-s, 10-s, negat
+000008b0: 6976 6520 7661 6c75 6573 2061 7265 2064  ive values are d
+000008c0: 656c 6574 6564 202a 2f0a 766f 6964 2062  eleted */.void b
+000008d0: 6974 7365 745f 7368 6966 745f 7269 6768  itset_shift_righ
+000008e0: 7428 6269 7473 6574 5f74 202a 6269 7473  t(bitset_t *bits
+000008f0: 6574 2c20 7369 7a65 5f74 2073 293b 0a0a  et, size_t s);..
+00000900: 2f2a 2053 6574 2074 6865 2069 7468 2062  /* Set the ith b
+00000910: 6974 2e20 4174 7465 6d70 7473 2074 6f20  it. Attempts to 
+00000920: 7265 7369 7a65 2074 6865 2062 6974 7365  resize the bitse
+00000930: 7420 6966 206e 6565 6465 6420 286d 6179  t if needed (may
+00000940: 2073 696c 656e 746c 7920 6661 696c 2920   silently fail) 
+00000950: 2a2f 0a76 6f69 6420 6269 7473 6574 5f73  */.void bitset_s
+00000960: 6574 2862 6974 7365 745f 7420 2a62 6974  et(bitset_t *bit
+00000970: 7365 742c 2020 7369 7a65 5f74 2069 293b  set,  size_t i);
+00000980: 0a0a 2f2a 2053 6574 2074 6865 2069 7468  ../* Set the ith
+00000990: 2062 6974 2074 6f20 7468 6520 7370 6563   bit to the spec
+000009a0: 6966 6965 6420 7661 6c75 652e 2041 7474  ified value. Att
+000009b0: 656d 7074 7320 746f 2072 6573 697a 6520  empts to resize 
+000009c0: 7468 6520 6269 7473 6574 2069 6620 6e65  the bitset if ne
+000009d0: 6564 6564 2028 6d61 7920 7369 6c65 6e74  eded (may silent
+000009e0: 6c79 2066 6169 6c29 202a 2f0a 766f 6964  ly fail) */.void
+000009f0: 2062 6974 7365 745f 7365 745f 746f 5f76   bitset_set_to_v
+00000a00: 616c 7565 2862 6974 7365 745f 7420 2a62  alue(bitset_t *b
+00000a10: 6974 7365 742c 2020 7369 7a65 5f74 2069  itset,  size_t i
+00000a20: 2c20 626f 6f6c 2066 6c61 6729 3b0a 0a0a  , bool flag);...
+00000a30: 0a0a 2f2a 2047 6574 2074 6865 2076 616c  ../* Get the val
+00000a40: 7565 206f 6620 7468 6520 6974 6820 6269  ue of the ith bi
+00000a50: 742e 2020 2a2f 0a62 6f6f 6c20 6269 7473  t.  */.bool bits
+00000a60: 6574 5f67 6574 2863 6f6e 7374 2062 6974  et_get(const bit
+00000a70: 7365 745f 7420 2a62 6974 7365 742c 2020  set_t *bitset,  
+00000a80: 7369 7a65 5f74 2069 2029 3b0a 0a2f 2a20  size_t i );../* 
+00000a90: 436f 756e 7420 6e75 6d62 6572 206f 6620  Count number of 
+00000aa0: 6269 7473 2073 6574 2e20 202a 2f0a 7369  bits set.  */.si
+00000ab0: 7a65 5f74 2062 6974 7365 745f 636f 756e  ze_t bitset_coun
+00000ac0: 7428 636f 6e73 7420 6269 7473 6574 5f74  t(const bitset_t
+00000ad0: 202a 6269 7473 6574 293b 0a0a 2f2a 2046   *bitset);../* F
+00000ae0: 696e 6420 7468 6520 696e 6465 7820 6f66  ind the index of
+00000af0: 2074 6865 2066 6972 7374 2062 6974 2073   the first bit s
+00000b00: 6574 2e20 4f72 207a 6572 6f20 6966 2074  et. Or zero if t
+00000b10: 6865 2062 6974 7365 7420 6973 2065 6d70  he bitset is emp
+00000b20: 7479 2e20 202a 2f0a 7369 7a65 5f74 2062  ty.  */.size_t b
+00000b30: 6974 7365 745f 6d69 6e69 6d75 6d28 636f  itset_minimum(co
+00000b40: 6e73 7420 6269 7473 6574 5f74 202a 6269  nst bitset_t *bi
+00000b50: 7473 6574 293b 0a0a 2f2a 2046 696e 6420  tset);../* Find 
+00000b60: 7468 6520 696e 6465 7820 6f66 2074 6865  the index of the
+00000b70: 206c 6173 7420 6269 7420 7365 742e 204f   last bit set. O
+00000b80: 7220 7a65 726f 2069 6620 7468 6520 6269  r zero if the bi
+00000b90: 7473 6574 2069 7320 656d 7074 792e 202a  tset is empty. *
+00000ba0: 2f0a 7369 7a65 5f74 2062 6974 7365 745f  /.size_t bitset_
+00000bb0: 6d61 7869 6d75 6d28 636f 6e73 7420 6269  maximum(const bi
+00000bc0: 7473 6574 5f74 202a 6269 7473 6574 293b  tset_t *bitset);
+00000bd0: 0a0a 0a2f 2a20 636f 6d70 7574 6520 7468  .../* compute th
+00000be0: 6520 756e 696f 6e20 696e 2d70 6c61 6365  e union in-place
+00000bf0: 2028 746f 2062 3129 2c20 7265 7475 726e   (to b1), return
+00000c00: 7320 7472 7565 2069 6620 7375 6363 6573  s true if succes
+00000c10: 7366 756c 2c20 746f 2067 656e 6572 6174  sful, to generat
+00000c20: 6520 6120 6e65 7720 6269 7473 6574 2066  e a new bitset f
+00000c30: 6972 7374 2063 616c 6c20 6269 7473 6574  irst call bitset
+00000c40: 5f63 6f70 7920 2a2f 0a62 6f6f 6c20 6269  _copy */.bool bi
+00000c50: 7473 6574 5f69 6e70 6c61 6365 5f75 6e69  tset_inplace_uni
+00000c60: 6f6e 2862 6974 7365 745f 7420 2a20 6231  on(bitset_t * b1
+00000c70: 2c20 636f 6e73 7420 6269 7473 6574 5f74  , const bitset_t
+00000c80: 202a 2062 3229 3b0a 0a2f 2a20 7265 706f   * b2);../* repo
+00000c90: 7274 2074 6865 2073 697a 6520 6f66 2074  rt the size of t
+00000ca0: 6865 2075 6e69 6f6e 2028 7769 7468 6f75  he union (withou
+00000cb0: 7420 6d61 7465 7269 616c 697a 696e 6720  t materializing 
+00000cc0: 6974 2920 2a2f 0a73 697a 655f 7420 6269  it) */.size_t bi
+00000cd0: 7473 6574 5f75 6e69 6f6e 5f63 6f75 6e74  tset_union_count
+00000ce0: 2863 6f6e 7374 2062 6974 7365 745f 7420  (const bitset_t 
+00000cf0: 2a20 6231 2c20 636f 6e73 7420 6269 7473  * b1, const bits
+00000d00: 6574 5f74 202a 2062 3229 3b0a 0a2f 2a20  et_t * b2);../* 
+00000d10: 636f 6d70 7574 6520 7468 6520 696e 7465  compute the inte
+00000d20: 7273 6563 7469 6f6e 2069 6e2d 706c 6163  rsection in-plac
+00000d30: 6520 2874 6f20 6231 292c 2074 6f20 6765  e (to b1), to ge
+00000d40: 6e65 7261 7465 2061 206e 6577 2062 6974  nerate a new bit
+00000d50: 7365 7420 6669 7273 7420 6361 6c6c 2062  set first call b
+00000d60: 6974 7365 745f 636f 7079 202a 2f0a 766f  itset_copy */.vo
+00000d70: 6964 2062 6974 7365 745f 696e 706c 6163  id bitset_inplac
+00000d80: 655f 696e 7465 7273 6563 7469 6f6e 2862  e_intersection(b
+00000d90: 6974 7365 745f 7420 2a20 6231 2c20 636f  itset_t * b1, co
+00000da0: 6e73 7420 6269 7473 6574 5f74 202a 2062  nst bitset_t * b
+00000db0: 3229 3b0a 0a2f 2a20 5265 706f 7274 2074  2);../* Report t
+00000dc0: 6865 2073 697a 6520 6f66 2074 6865 2069  he size of the i
+00000dd0: 6e74 6572 7365 6374 696f 6e20 2877 6974  ntersection (wit
+00000de0: 686f 7574 206d 6174 6572 6961 6c69 7a69  hout materializi
+00000df0: 6e67 2069 7429 2e0a 202a 2057 6520 6173  ng it).. * We as
+00000e00: 7375 6d65 2074 6861 7420 7468 6520 6269  sume that the bi
+00000e10: 7473 6574 7320 6231 2061 6e64 2062 3220  tsets b1 and b2 
+00000e20: 6172 6520 6469 7374 696e 6374 2e20 2a2f  are distinct. */
+00000e30: 0a73 697a 655f 7420 6269 7473 6574 5f69  .size_t bitset_i
+00000e40: 6e74 6572 7365 6374 696f 6e5f 636f 756e  ntersection_coun
+00000e50: 7428 636f 6e73 7420 6269 7473 6574 5f74  t(const bitset_t
+00000e60: 202a 2062 312c 2063 6f6e 7374 2062 6974   * b1, const bit
+00000e70: 7365 745f 7420 2a20 6232 293b 0a0a 0a2f  set_t * b2);.../
+00000e80: 2a20 7265 7475 726e 7320 7472 7565 2069  * returns true i
+00000e90: 6620 7468 6520 6269 7473 6574 7320 636f  f the bitsets co
+00000ea0: 6e74 6169 6e20 6e6f 2063 6f6d 6d6f 6e20  ntain no common 
+00000eb0: 656c 656d 656e 7473 202a 2f0a 626f 6f6c  elements */.bool
+00000ec0: 2062 6974 7365 7473 5f64 6973 6a6f 696e   bitsets_disjoin
+00000ed0: 7428 636f 6e73 7420 6269 7473 6574 5f74  t(const bitset_t
+00000ee0: 202a 2062 312c 2063 6f6e 7374 2062 6974   * b1, const bit
+00000ef0: 7365 745f 7420 2a20 6232 293b 0a0a 2f2a  set_t * b2);../*
+00000f00: 2072 6574 7572 6e73 2074 7275 6520 6966   returns true if
+00000f10: 2074 6865 2062 6974 7365 7473 2063 6f6e   the bitsets con
+00000f20: 7461 696e 2061 6e79 2063 6f6d 6d6f 6e20  tain any common 
+00000f30: 656c 656d 656e 7473 202a 2f0a 626f 6f6c  elements */.bool
+00000f40: 2062 6974 7365 7473 5f69 6e74 6572 7365   bitsets_interse
+00000f50: 6374 2863 6f6e 7374 2062 6974 7365 745f  ct(const bitset_
+00000f60: 7420 2a20 6231 2c20 636f 6e73 7420 6269  t * b1, const bi
+00000f70: 7473 6574 5f74 202a 2062 3229 3b0a 0a2f  tset_t * b2);../
+00000f80: 2a20 7265 7475 726e 7320 7472 7565 2069  * returns true i
+00000f90: 6620 6231 2063 6f6e 7461 696e 7320 616c  f b1 contains al
+00000fa0: 6c20 6f66 2074 6865 2073 6574 2062 6974  l of the set bit
+00000fb0: 7320 6f66 2062 3220 2a2f 0a62 6f6f 6c20  s of b2 */.bool 
+00000fc0: 6269 7473 6574 5f63 6f6e 7461 696e 735f  bitset_contains_
+00000fd0: 616c 6c28 636f 6e73 7420 6269 7473 6574  all(const bitset
+00000fe0: 5f74 202a 2062 312c 2063 6f6e 7374 2062  _t * b1, const b
+00000ff0: 6974 7365 745f 7420 2a20 6232 293b 0a0a  itset_t * b2);..
+00001000: 0a2f 2a20 636f 6d70 7574 6520 7468 6520  ./* compute the 
+00001010: 6469 6666 6572 656e 6365 2069 6e2d 706c  difference in-pl
+00001020: 6163 6520 2874 6f20 6231 292c 2074 6f20  ace (to b1), to 
+00001030: 6765 6e65 7261 7465 2061 206e 6577 2062  generate a new b
+00001040: 6974 7365 7420 6669 7273 7420 6361 6c6c  itset first call
+00001050: 2062 6974 7365 745f 636f 7079 202a 2f0a   bitset_copy */.
+00001060: 766f 6964 2062 6974 7365 745f 696e 706c  void bitset_inpl
+00001070: 6163 655f 6469 6666 6572 656e 6365 2862  ace_difference(b
+00001080: 6974 7365 745f 7420 2a20 6231 2c20 636f  itset_t * b1, co
+00001090: 6e73 7420 6269 7473 6574 5f74 202a 2062  nst bitset_t * b
+000010a0: 3229 3b0a 0a2f 2a20 636f 6d70 7574 6520  2);../* compute 
+000010b0: 7468 6520 7369 7a65 206f 6620 7468 6520  the size of the 
+000010c0: 6469 6666 6572 656e 6365 202a 2f0a 7369  difference */.si
+000010d0: 7a65 5f74 2020 6269 7473 6574 5f64 6966  ze_t  bitset_dif
+000010e0: 6665 7265 6e63 655f 636f 756e 7428 636f  ference_count(co
+000010f0: 6e73 7420 6269 7473 6574 5f74 202a 2062  nst bitset_t * b
+00001100: 312c 2063 6f6e 7374 2062 6974 7365 745f  1, const bitset_
+00001110: 7420 2a20 6232 2920 3b0a 0a2f 2a20 636f  t * b2) ;../* co
+00001120: 6d70 7574 6520 7468 6520 7379 6d6d 6574  mpute the symmet
+00001130: 7269 6320 6469 6666 6572 656e 6365 2069  ric difference i
+00001140: 6e2d 706c 6163 6520 2874 6f20 6231 292c  n-place (to b1),
+00001150: 2072 6574 7572 6e20 7472 7565 2069 6620   return true if 
+00001160: 7375 6363 6573 7366 756c 2c20 746f 2067  successful, to g
+00001170: 656e 6572 6174 6520 6120 6e65 7720 6269  enerate a new bi
+00001180: 7473 6574 2066 6972 7374 2063 616c 6c20  tset first call 
+00001190: 6269 7473 6574 5f63 6f70 7920 2a2f 0a62  bitset_copy */.b
+000011a0: 6f6f 6c20 6269 7473 6574 5f69 6e70 6c61  ool bitset_inpla
+000011b0: 6365 5f73 796d 6d65 7472 6963 5f64 6966  ce_symmetric_dif
+000011c0: 6665 7265 6e63 6528 6269 7473 6574 5f74  ference(bitset_t
+000011d0: 202a 2062 312c 2063 6f6e 7374 2062 6974   * b1, const bit
+000011e0: 7365 745f 7420 2a20 6232 293b 0a0a 2f2a  set_t * b2);../*
+000011f0: 2063 6f6d 7075 7465 2074 6865 2073 697a   compute the siz
+00001200: 6520 6f66 2074 6865 2073 796d 6d65 7472  e of the symmetr
+00001210: 6963 2064 6966 6665 7265 6e63 6520 202a  ic difference  *
+00001220: 2f0a 7369 7a65 5f74 2020 6269 7473 6574  /.size_t  bitset
+00001230: 5f73 796d 6d65 7472 6963 5f64 6966 6665  _symmetric_diffe
+00001240: 7265 6e63 655f 636f 756e 7428 636f 6e73  rence_count(cons
+00001250: 7420 6269 7473 6574 5f74 202a 2062 312c  t bitset_t * b1,
+00001260: 2063 6f6e 7374 2062 6974 7365 745f 7420   const bitset_t 
+00001270: 2a20 6232 293b 0a0a 2f2a 2069 7465 7261  * b2);../* itera
+00001280: 7465 206f 7665 7220 7468 6520 7365 7420  te over the set 
+00001290: 6269 7473 0a20 6c69 6b65 2073 6f20 3a0a  bits. like so :.
+000012a0: 2020 666f 7228 7369 7a65 5f74 2069 203d    for(size_t i =
+000012b0: 2030 3b20 6269 7473 6574 5f6e 6578 745f   0; bitset_next_
+000012c0: 7365 745f 6269 7428 622c 2669 2920 3b20  set_bit(b,&i) ; 
+000012d0: 692b 2b29 207b 0a20 2020 202f 2f2e 2e2e  i++) {.    //...
+000012e0: 2e2e 0a20 207d 0a20 202a 2f0a 626f 6f6c  ...  }.  */.bool
+000012f0: 2062 6974 7365 745f 6e65 7874 5f73 6574   bitset_next_set
+00001300: 5f62 6974 2863 6f6e 7374 2062 6974 7365  _bit(const bitse
+00001310: 745f 7420 2a62 6974 7365 742c 2073 697a  t_t *bitset, siz
+00001320: 655f 7420 2a69 293b 0a2f 2a20 6974 6572  e_t *i);./* iter
+00001330: 6174 6520 6f76 6572 2074 6865 2073 6574  ate over the set
+00001340: 2062 6974 730a 206c 696b 6520 736f 203a   bits. like so :
+00001350: 0a20 2020 7369 7a65 5f74 2062 7566 6665  .   size_t buffe
+00001360: 725b 3235 365d 3b0a 2020 2073 697a 655f  r[256];.   size_
+00001370: 7420 686f 776d 616e 7920 3d20 303b 0a20  t howmany = 0;. 
+00001380: 2066 6f72 2873 697a 655f 7420 7374 6172   for(size_t star
+00001390: 7466 726f 6d20 3d20 303b 2028 686f 776d  tfrom = 0; (howm
+000013a0: 616e 7920 3d20 6269 7473 6574 5f6e 6578  any = bitset_nex
+000013b0: 745f 7365 745f 6269 7473 2862 2c62 7566  t_set_bits(b,buf
+000013c0: 6665 722c 3235 362c 2026 7374 6172 7466  fer,256, &startf
+000013d0: 726f 6d29 2920 3e20 3020 3b20 7374 6172  rom)) > 0 ; star
+000013e0: 7466 726f 6d2b 2b29 207b 0a20 2020 202f  tfrom++) {.    /
+000013f0: 2f2e 2e2e 2e2e 0a20 207d 0a20 202a 2f0a  /......  }.  */.
+00001400: 7369 7a65 5f74 2062 6974 7365 745f 6e65  size_t bitset_ne
+00001410: 7874 5f73 6574 5f62 6974 7328 636f 6e73  xt_set_bits(cons
+00001420: 7420 6269 7473 6574 5f74 202a 6269 7473  t bitset_t *bits
+00001430: 6574 2c20 7369 7a65 5f74 202a 6275 6666  et, size_t *buff
+00001440: 6572 2c20 7369 7a65 5f74 2063 6170 6163  er, size_t capac
+00001450: 6974 792c 2073 697a 655f 7420 2a20 7374  ity, size_t * st
+00001460: 6172 7466 726f 6d29 3b0a 0a74 7970 6564  artfrom);..typed
+00001470: 6566 2062 6f6f 6c20 282a 6269 7473 6574  ef bool (*bitset
+00001480: 5f69 7465 7261 746f 7229 2873 697a 655f  _iterator)(size_
+00001490: 7420 7661 6c75 652c 2076 6f69 6420 2a70  t value, void *p
+000014a0: 6172 616d 293b 0a0a 2f2f 2072 6574 7572  aram);..// retur
+000014b0: 6e20 7472 7565 2069 6620 756e 696e 7465  n true if uninte
+000014c0: 7272 7570 7465 640a 626f 6f6c 2062 6974  rrupted.bool bit
+000014d0: 7365 745f 666f 725f 6561 6368 2863 6f6e  set_for_each(con
+000014e0: 7374 2062 6974 7365 745f 7420 2a62 2c20  st bitset_t *b, 
+000014f0: 6269 7473 6574 5f69 7465 7261 746f 7220  bitset_iterator 
+00001500: 6974 6572 6174 6f72 2c20 766f 6964 202a  iterator, void *
+00001510: 7074 7229 3b20 0a76 6f69 6420 6269 7473  ptr); .void bits
+00001520: 6574 5f70 7269 6e74 2863 6f6e 7374 2062  et_print(const b
+00001530: 6974 7365 745f 7420 2a62 293b 0a0a 6578  itset_t *b);..ex
+00001540: 7465 726e 2022 5079 7468 6f6e 2220 626f  tern "Python" bo
+00001550: 6f6c 2062 6974 7365 745f 6974 6572 6174  ol bitset_iterat
+00001560: 6f72 5f66 756e 6328 7369 7a65 5f74 2076  or_func(size_t v
+00001570: 616c 7565 2c20 766f 6964 2a20 7061 7261  alue, void* para
+00001580: 6d29 3b0a 2020 2020 2222 220a 290a 0a73  m);.    """.)..s
+00001590: 6f75 7263 6520 3d20 2222 220a 2369 6e63  ource = """.#inc
+000015a0: 6c75 6465 203c 7374 6469 6f2e 683e 0a23  lude <stdio.h>.#
+000015b0: 696e 636c 7564 6520 3c73 7464 6c69 622e  include <stdlib.
+000015c0: 683e 0a23 696e 636c 7564 6520 3c73 7464  h>.#include <std
+000015d0: 696e 742e 683e 0a23 696e 636c 7564 6520  int.h>.#include 
+000015e0: 3c73 7464 626f 6f6c 2e68 3e0a 2369 6e63  <stdbool.h>.#inc
+000015f0: 6c75 6465 203c 7374 6469 6f2e 683e 0a23  lude <stdio.h>.#
+00001600: 696e 636c 7564 6520 3c73 7472 696e 672e  include <string.
+00001610: 683e 0a23 696e 636c 7564 6520 2262 6974  h>.#include "bit
+00001620: 7365 742e 6822 0a22 2222 0a63 5f73 6f75  set.h".""".c_sou
+00001630: 7263 6573 203d 2067 6c6f 622e 676c 6f62  rces = glob.glob
+00001640: 2822 2e2f 6362 6974 7365 742f 7372 632f  ("./cbitset/src/
+00001650: 2a2e 6322 290a 2320 635f 736f 7572 6365  *.c").# c_source
+00001660: 7320 3d20 6c69 7374 2866 696c 7465 7228  s = list(filter(
+00001670: 6c61 6d62 6461 2078 3a20 226d 6169 6e22  lambda x: "main"
+00001680: 206e 6f74 2069 6e20 782c 2063 5f73 6f75   not in x, c_sou
+00001690: 7263 6573 2929 0a70 7269 6e74 2863 5f73  rces)).print(c_s
+000016a0: 6f75 7263 6573 290a 0a66 6669 6275 696c  ources)..ffibuil
+000016b0: 6465 722e 7365 745f 736f 7572 6365 280a  der.set_source(.
+000016c0: 2020 2020 2270 7962 6974 7365 742e 6261      "pybitset.ba
+000016d0: 636b 656e 6473 2e63 6666 692e 5f62 6974  ckends.cffi._bit
+000016e0: 7365 7422 2c0a 2020 2020 736f 7572 6365  set",.    source
+000016f0: 2c0a 2020 2020 736f 7572 6365 733d 635f  ,.    sources=c_
+00001700: 736f 7572 6365 732c 0a20 2020 2069 6e63  sources,.    inc
+00001710: 6c75 6465 5f64 6972 733d 5b22 2e2f 6362  lude_dirs=["./cb
+00001720: 6974 7365 742f 696e 636c 7564 6522 5d2c  itset/include"],
+00001730: 0a29 0a0a 6966 205f 5f6e 616d 655f 5f20  .)..if __name__ 
+00001740: 3d3d 2022 5f5f 6d61 696e 5f5f 223a 0a20  == "__main__":. 
+00001750: 2020 2066 6669 6275 696c 6465 722e 636f     ffibuilder.co
+00001760: 6d70 696c 6528 290a                      mpile().
```

### Comparing `pybitset-0.0.1.dev1/pybitset/backends/cython/_bitset.c` & `pybitset-0.0.1.dev2/pybitset/backends/cython/_bitset.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.34 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "cbitset\\include\\bitset.h"
         ],
@@ -24,16 +24,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_34"
-#define CYTHON_HEX_VERSION 0x001D22F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -93,16 +93,20 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -991,24 +995,24 @@
 struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSetIter;
 
 /* "pybitset/backends/cython/_bitset.pyx":25
  * @cython.final
  * @cython.no_gc
  * cdef class BitSet:             # <<<<<<<<<<<<<<
  *     cdef bitset_t * _bitset
- *     def __cinit__(self, size_t size=0):
+ *     def __cinit__(self, size_t size=0, bint _init = True):
  */
 struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet {
   PyObject_HEAD
   struct __pyx_vtabstruct_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_vtab;
   bitset_t *_bitset;
 };
 
 
-/* "pybitset/backends/cython/_bitset.pyx":214
+/* "pybitset/backends/cython/_bitset.pyx":217
  * @cython.final
  * @cython.no_gc
  * cdef class BitSetIter:             # <<<<<<<<<<<<<<
  *     cdef:
  *         BitSet b
  */
 struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSetIter {
@@ -1020,15 +1024,15 @@
 
 
 /* "pybitset/backends/cython/_bitset.pyx":25
  * @cython.final
  * @cython.no_gc
  * cdef class BitSet:             # <<<<<<<<<<<<<<
  *     cdef bitset_t * _bitset
- *     def __cinit__(self, size_t size=0):
+ *     def __cinit__(self, size_t size=0, bint _init = True):
  */
 
 struct __pyx_vtabstruct_8pybitset_8backends_6cython_7_bitset_BitSet {
   struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *(*from_ptr)(bitset_t *);
   PyObject *(*clear)(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *, int __pyx_skip_dispatch);
   PyObject *(*fill)(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *, int __pyx_skip_dispatch);
   struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *(*copy)(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *, int __pyx_skip_dispatch);
@@ -1447,14 +1451,15 @@
 /* Implementation of 'pybitset.backends.cython._bitset' */
 static PyObject *__pyx_builtin_MemoryError;
 static PyObject *__pyx_builtin_TypeError;
 static PyObject *__pyx_builtin_StopIteration;
 static const char __pyx_k_b[] = "b";
 static const char __pyx_k_i[] = "i";
 static const char __pyx_k_flag[] = "flag";
+static const char __pyx_k_init[] = "_init";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_size[] = "size";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_BitSet[] = "BitSet";
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_getstate[] = "__getstate__";
@@ -1475,28 +1480,29 @@
 static PyObject *__pyx_n_s_StopIteration;
 static PyObject *__pyx_n_s_TypeError;
 static PyObject *__pyx_n_s_b;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_flag;
 static PyObject *__pyx_n_s_getstate;
 static PyObject *__pyx_n_s_i;
+static PyObject *__pyx_n_s_init;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_newarraysize;
 static PyObject *__pyx_kp_s_no_default___reduce___due_to_non;
 static PyObject *__pyx_n_s_padwithzeroes;
 static PyObject *__pyx_n_s_pyx_vtable;
 static PyObject *__pyx_n_s_reduce;
 static PyObject *__pyx_n_s_reduce_cython;
 static PyObject *__pyx_n_s_reduce_ex;
 static PyObject *__pyx_n_s_setstate;
 static PyObject *__pyx_n_s_setstate_cython;
 static PyObject *__pyx_n_s_size;
 static PyObject *__pyx_n_s_test;
-static int __pyx_pf_8pybitset_8backends_6cython_7_bitset_6BitSet___cinit__(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, size_t __pyx_v_size); /* proto */
+static int __pyx_pf_8pybitset_8backends_6cython_7_bitset_6BitSet___cinit__(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, size_t __pyx_v_size, int __pyx_v__init); /* proto */
 static void __pyx_pf_8pybitset_8backends_6cython_7_bitset_6BitSet_2__dealloc__(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8pybitset_8backends_6cython_7_bitset_6BitSet_4clear(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8pybitset_8backends_6cython_7_bitset_6BitSet_6fill(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8pybitset_8backends_6cython_7_bitset_6BitSet_8copy(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8pybitset_8backends_6cython_7_bitset_6BitSet_10resize(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, size_t __pyx_v_newarraysize, int __pyx_v_padwithzeroes); /* proto */
 static PyObject *__pyx_pf_8pybitset_8backends_6cython_7_bitset_6BitSet_12size_in_bytes(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_8pybitset_8backends_6cython_7_bitset_6BitSet_14size_in_bits(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self); /* proto */
@@ -1618,180 +1624,228 @@
   #endif
   return __pyx_r;
 }
 
 /* "pybitset/backends/cython/_bitset.pyx":27
  * cdef class BitSet:
  *     cdef bitset_t * _bitset
- *     def __cinit__(self, size_t size=0):             # <<<<<<<<<<<<<<
- *         if size == 0:
- *             self._bitset = bitset_create()
+ *     def __cinit__(self, size_t size=0, bint _init = True):             # <<<<<<<<<<<<<<
+ *         if _init:
+ *             if size == 0:
  */
 
 /* Python wrapper */
 static int __pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   size_t __pyx_v_size;
+  int __pyx_v__init;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__ (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_size,0};
-    PyObject* values[1] = {0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_size,&__pyx_n_s_init,0};
+    PyObject* values[2] = {0,0};
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_size);
           if (value) { values[0] = value; kw_args--; }
         }
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_init);
+          if (value) { values[1] = value; kw_args--; }
+        }
       }
       if (unlikely(kw_args > 0)) {
         if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 27, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     if (values[0]) {
       __pyx_v_size = __Pyx_PyInt_As_size_t(values[0]); if (unlikely((__pyx_v_size == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 27, __pyx_L3_error)
     } else {
       __pyx_v_size = ((size_t)0);
     }
+    if (values[1]) {
+      __pyx_v__init = __Pyx_PyObject_IsTrue(values[1]); if (unlikely((__pyx_v__init == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 27, __pyx_L3_error)
+    } else {
+      __pyx_v__init = ((int)1);
+    }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 27, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 0, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 27, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pybitset.backends.cython._bitset.BitSet.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8pybitset_8backends_6cython_7_bitset_6BitSet___cinit__(((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_self), __pyx_v_size);
+  __pyx_r = __pyx_pf_8pybitset_8backends_6cython_7_bitset_6BitSet___cinit__(((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_self), __pyx_v_size, __pyx_v__init);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static int __pyx_pf_8pybitset_8backends_6cython_7_bitset_6BitSet___cinit__(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, size_t __pyx_v_size) {
+static int __pyx_pf_8pybitset_8backends_6cython_7_bitset_6BitSet___cinit__(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, size_t __pyx_v_size, int __pyx_v__init) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
   /* "pybitset/backends/cython/_bitset.pyx":28
  *     cdef bitset_t * _bitset
- *     def __cinit__(self, size_t size=0):
- *         if size == 0:             # <<<<<<<<<<<<<<
- *             self._bitset = bitset_create()
- *         else:
+ *     def __cinit__(self, size_t size=0, bint _init = True):
+ *         if _init:             # <<<<<<<<<<<<<<
+ *             if size == 0:
+ *                 self._bitset = bitset_create()
  */
-  __pyx_t_1 = ((__pyx_v_size == 0) != 0);
+  __pyx_t_1 = (__pyx_v__init != 0);
   if (__pyx_t_1) {
 
     /* "pybitset/backends/cython/_bitset.pyx":29
- *     def __cinit__(self, size_t size=0):
- *         if size == 0:
- *             self._bitset = bitset_create()             # <<<<<<<<<<<<<<
- *         else:
- *             self._bitset = bitset_create_with_capacity(size)
+ *     def __cinit__(self, size_t size=0, bint _init = True):
+ *         if _init:
+ *             if size == 0:             # <<<<<<<<<<<<<<
+ *                 self._bitset = bitset_create()
+ *             else:
+ */
+    __pyx_t_1 = ((__pyx_v_size == 0) != 0);
+    if (__pyx_t_1) {
+
+      /* "pybitset/backends/cython/_bitset.pyx":30
+ *         if _init:
+ *             if size == 0:
+ *                 self._bitset = bitset_create()             # <<<<<<<<<<<<<<
+ *             else:
+ *                 self._bitset = bitset_create_with_capacity(size)
+ */
+      __pyx_v_self->_bitset = bitset_create();
+
+      /* "pybitset/backends/cython/_bitset.pyx":29
+ *     def __cinit__(self, size_t size=0, bint _init = True):
+ *         if _init:
+ *             if size == 0:             # <<<<<<<<<<<<<<
+ *                 self._bitset = bitset_create()
+ *             else:
  */
-    __pyx_v_self->_bitset = bitset_create();
+      goto __pyx_L4;
+    }
 
-    /* "pybitset/backends/cython/_bitset.pyx":28
- *     cdef bitset_t * _bitset
- *     def __cinit__(self, size_t size=0):
- *         if size == 0:             # <<<<<<<<<<<<<<
- *             self._bitset = bitset_create()
+    /* "pybitset/backends/cython/_bitset.pyx":32
+ *                 self._bitset = bitset_create()
+ *             else:
+ *                 self._bitset = bitset_create_with_capacity(size)             # <<<<<<<<<<<<<<
+ *             if not self._bitset:
+ *                 raise MemoryError
+ */
+    /*else*/ {
+      __pyx_v_self->_bitset = bitset_create_with_capacity(__pyx_v_size);
+    }
+    __pyx_L4:;
+
+    /* "pybitset/backends/cython/_bitset.pyx":33
+ *             else:
+ *                 self._bitset = bitset_create_with_capacity(size)
+ *             if not self._bitset:             # <<<<<<<<<<<<<<
+ *                 raise MemoryError
  *         else:
  */
-    goto __pyx_L3;
-  }
+    __pyx_t_1 = ((!(__pyx_v_self->_bitset != 0)) != 0);
+    if (unlikely(__pyx_t_1)) {
 
-  /* "pybitset/backends/cython/_bitset.pyx":31
- *             self._bitset = bitset_create()
+      /* "pybitset/backends/cython/_bitset.pyx":34
+ *                 self._bitset = bitset_create_with_capacity(size)
+ *             if not self._bitset:
+ *                 raise MemoryError             # <<<<<<<<<<<<<<
  *         else:
- *             self._bitset = bitset_create_with_capacity(size)             # <<<<<<<<<<<<<<
- *         if not self._bitset:
- *             raise MemoryError
+ *             self._bitset = NULL
  */
-  /*else*/ {
-    __pyx_v_self->_bitset = bitset_create_with_capacity(__pyx_v_size);
-  }
-  __pyx_L3:;
+      PyErr_NoMemory(); __PYX_ERR(0, 34, __pyx_L1_error)
 
-  /* "pybitset/backends/cython/_bitset.pyx":32
+      /* "pybitset/backends/cython/_bitset.pyx":33
+ *             else:
+ *                 self._bitset = bitset_create_with_capacity(size)
+ *             if not self._bitset:             # <<<<<<<<<<<<<<
+ *                 raise MemoryError
  *         else:
- *             self._bitset = bitset_create_with_capacity(size)
- *         if not self._bitset:             # <<<<<<<<<<<<<<
- *             raise MemoryError
- * 
  */
-  __pyx_t_1 = ((!(__pyx_v_self->_bitset != 0)) != 0);
-  if (unlikely(__pyx_t_1)) {
+    }
 
-    /* "pybitset/backends/cython/_bitset.pyx":33
- *             self._bitset = bitset_create_with_capacity(size)
- *         if not self._bitset:
- *             raise MemoryError             # <<<<<<<<<<<<<<
- * 
- *     def __dealloc__(self):
+    /* "pybitset/backends/cython/_bitset.pyx":28
+ *     cdef bitset_t * _bitset
+ *     def __cinit__(self, size_t size=0, bint _init = True):
+ *         if _init:             # <<<<<<<<<<<<<<
+ *             if size == 0:
+ *                 self._bitset = bitset_create()
  */
-    PyErr_NoMemory(); __PYX_ERR(0, 33, __pyx_L1_error)
+    goto __pyx_L3;
+  }
 
-    /* "pybitset/backends/cython/_bitset.pyx":32
+  /* "pybitset/backends/cython/_bitset.pyx":36
+ *                 raise MemoryError
  *         else:
- *             self._bitset = bitset_create_with_capacity(size)
- *         if not self._bitset:             # <<<<<<<<<<<<<<
- *             raise MemoryError
+ *             self._bitset = NULL             # <<<<<<<<<<<<<<
  * 
+ *     def __dealloc__(self):
  */
+  /*else*/ {
+    __pyx_v_self->_bitset = NULL;
   }
+  __pyx_L3:;
 
   /* "pybitset/backends/cython/_bitset.pyx":27
  * cdef class BitSet:
  *     cdef bitset_t * _bitset
- *     def __cinit__(self, size_t size=0):             # <<<<<<<<<<<<<<
- *         if size == 0:
- *             self._bitset = bitset_create()
+ *     def __cinit__(self, size_t size=0, bint _init = True):             # <<<<<<<<<<<<<<
+ *         if _init:
+ *             if size == 0:
  */
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("pybitset.backends.cython._bitset.BitSet.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":35
- *             raise MemoryError
+/* "pybitset/backends/cython/_bitset.pyx":38
+ *             self._bitset = NULL
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         bitset_free(self._bitset)
  *         self._bitset = NULL
  */
 
 /* Python wrapper */
@@ -1805,155 +1859,161 @@
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_pf_8pybitset_8backends_6cython_7_bitset_6BitSet_2__dealloc__(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":36
+  /* "pybitset/backends/cython/_bitset.pyx":39
  * 
  *     def __dealloc__(self):
  *         bitset_free(self._bitset)             # <<<<<<<<<<<<<<
  *         self._bitset = NULL
  * 
  */
   bitset_free(__pyx_v_self->_bitset);
 
-  /* "pybitset/backends/cython/_bitset.pyx":37
+  /* "pybitset/backends/cython/_bitset.pyx":40
  *     def __dealloc__(self):
  *         bitset_free(self._bitset)
  *         self._bitset = NULL             # <<<<<<<<<<<<<<
  * 
  *     @staticmethod
  */
   __pyx_v_self->_bitset = NULL;
 
-  /* "pybitset/backends/cython/_bitset.pyx":35
- *             raise MemoryError
+  /* "pybitset/backends/cython/_bitset.pyx":38
+ *             self._bitset = NULL
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         bitset_free(self._bitset)
  *         self._bitset = NULL
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":40
+/* "pybitset/backends/cython/_bitset.pyx":43
  * 
  *     @staticmethod
  *     cdef inline BitSet from_ptr(bitset_t * ptr):             # <<<<<<<<<<<<<<
- *         cdef BitSet self = BitSet.__new__(BitSet)
+ *         cdef BitSet self = BitSet(_init=False)
  *         self._bitset = ptr
  */
 
 static CYTHON_INLINE struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_from_ptr(bitset_t *__pyx_v_ptr) {
   struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self = 0;
   struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("from_ptr", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":41
+  /* "pybitset/backends/cython/_bitset.pyx":44
  *     @staticmethod
  *     cdef inline BitSet from_ptr(bitset_t * ptr):
- *         cdef BitSet self = BitSet.__new__(BitSet)             # <<<<<<<<<<<<<<
+ *         cdef BitSet self = BitSet(_init=False)             # <<<<<<<<<<<<<<
  *         self._bitset = ptr
  *         return self
  */
-  __pyx_t_1 = ((PyObject *)__pyx_tp_new_8pybitset_8backends_6cython_7_bitset_BitSet(((PyTypeObject *)__pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet), __pyx_empty_tuple, NULL)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 41, __pyx_L1_error)
-  __Pyx_GOTREF(((PyObject *)__pyx_t_1));
-  __pyx_v_self = ((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_t_1);
-  __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_init, Py_False) < 0) __PYX_ERR(0, 44, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet), __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v_self = ((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_t_2);
+  __pyx_t_2 = 0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":42
+  /* "pybitset/backends/cython/_bitset.pyx":45
  *     cdef inline BitSet from_ptr(bitset_t * ptr):
- *         cdef BitSet self = BitSet.__new__(BitSet)
+ *         cdef BitSet self = BitSet(_init=False)
  *         self._bitset = ptr             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
   __pyx_v_self->_bitset = __pyx_v_ptr;
 
-  /* "pybitset/backends/cython/_bitset.pyx":43
- *         cdef BitSet self = BitSet.__new__(BitSet)
+  /* "pybitset/backends/cython/_bitset.pyx":46
+ *         cdef BitSet self = BitSet(_init=False)
  *         self._bitset = ptr
  *         return self             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline clear(self):
  */
   __Pyx_XDECREF(((PyObject *)__pyx_r));
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __pyx_r = __pyx_v_self;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":40
+  /* "pybitset/backends/cython/_bitset.pyx":43
  * 
  *     @staticmethod
  *     cdef inline BitSet from_ptr(bitset_t * ptr):             # <<<<<<<<<<<<<<
- *         cdef BitSet self = BitSet.__new__(BitSet)
+ *         cdef BitSet self = BitSet(_init=False)
  *         self._bitset = ptr
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
   __Pyx_AddTraceback("pybitset.backends.cython._bitset.BitSet.from_ptr", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_self);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":45
+/* "pybitset/backends/cython/_bitset.pyx":48
  *         return self
  * 
  *     cpdef inline clear(self):             # <<<<<<<<<<<<<<
  *         with nogil:
  *             bitset_clear(self._bitset)
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_5clear(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_clear(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, CYTHON_UNUSED int __pyx_skip_dispatch) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("clear", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":46
+  /* "pybitset/backends/cython/_bitset.pyx":49
  * 
  *     cpdef inline clear(self):
  *         with nogil:             # <<<<<<<<<<<<<<
  *             bitset_clear(self._bitset)
  * 
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":47
+        /* "pybitset/backends/cython/_bitset.pyx":50
  *     cpdef inline clear(self):
  *         with nogil:
  *             bitset_clear(self._bitset)             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline fill(self):
  */
         bitset_clear(__pyx_v_self->_bitset);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":46
+      /* "pybitset/backends/cython/_bitset.pyx":49
  * 
  *     cpdef inline clear(self):
  *         with nogil:             # <<<<<<<<<<<<<<
  *             bitset_clear(self._bitset)
  * 
  */
       /*finally:*/ {
@@ -1964,15 +2024,15 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":45
+  /* "pybitset/backends/cython/_bitset.pyx":48
  *         return self
  * 
  *     cpdef inline clear(self):             # <<<<<<<<<<<<<<
  *         with nogil:
  *             bitset_clear(self._bitset)
  */
 
@@ -2002,15 +2062,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("clear", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_clear(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 45, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_clear(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 48, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2019,54 +2079,54 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":49
+/* "pybitset/backends/cython/_bitset.pyx":52
  *             bitset_clear(self._bitset)
  * 
  *     cpdef inline fill(self):             # <<<<<<<<<<<<<<
  *         with nogil:
  *             bitset_fill(self._bitset)
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_7fill(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_fill(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, CYTHON_UNUSED int __pyx_skip_dispatch) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("fill", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":50
+  /* "pybitset/backends/cython/_bitset.pyx":53
  * 
  *     cpdef inline fill(self):
  *         with nogil:             # <<<<<<<<<<<<<<
  *             bitset_fill(self._bitset)
  * 
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":51
+        /* "pybitset/backends/cython/_bitset.pyx":54
  *     cpdef inline fill(self):
  *         with nogil:
  *             bitset_fill(self._bitset)             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline BitSet copy(self):
  */
         bitset_fill(__pyx_v_self->_bitset);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":50
+      /* "pybitset/backends/cython/_bitset.pyx":53
  * 
  *     cpdef inline fill(self):
  *         with nogil:             # <<<<<<<<<<<<<<
  *             bitset_fill(self._bitset)
  * 
  */
       /*finally:*/ {
@@ -2077,15 +2137,15 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":49
+  /* "pybitset/backends/cython/_bitset.pyx":52
  *             bitset_clear(self._bitset)
  * 
  *     cpdef inline fill(self):             # <<<<<<<<<<<<<<
  *         with nogil:
  *             bitset_fill(self._bitset)
  */
 
@@ -2115,15 +2175,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("fill", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_fill(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 49, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_fill(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2132,15 +2192,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":53
+/* "pybitset/backends/cython/_bitset.pyx":56
  *             bitset_fill(self._bitset)
  * 
  *     cpdef inline BitSet copy(self):             # <<<<<<<<<<<<<<
  *         cdef bitset_t *ret
  *         with nogil:
  */
 
@@ -2151,40 +2211,40 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("copy", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":55
+  /* "pybitset/backends/cython/_bitset.pyx":58
  *     cpdef inline BitSet copy(self):
  *         cdef bitset_t *ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_copy(self._bitset)
  *         return BitSet.from_ptr(ret)
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":56
+        /* "pybitset/backends/cython/_bitset.pyx":59
  *         cdef bitset_t *ret
  *         with nogil:
  *             ret = bitset_copy(self._bitset)             # <<<<<<<<<<<<<<
  *         return BitSet.from_ptr(ret)
  * 
  */
         __pyx_v_ret = bitset_copy(__pyx_v_self->_bitset);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":55
+      /* "pybitset/backends/cython/_bitset.pyx":58
  *     cpdef inline BitSet copy(self):
  *         cdef bitset_t *ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_copy(self._bitset)
  *         return BitSet.from_ptr(ret)
  */
       /*finally:*/ {
@@ -2195,29 +2255,29 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":57
+  /* "pybitset/backends/cython/_bitset.pyx":60
  *         with nogil:
  *             ret = bitset_copy(self._bitset)
  *         return BitSet.from_ptr(ret)             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline bint resize(self, size_t newarraysize, bint padwithzeroes):
  */
   __Pyx_XDECREF(((PyObject *)__pyx_r));
-  __pyx_t_1 = ((PyObject *)__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_from_ptr(__pyx_v_ret)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 57, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_from_ptr(__pyx_v_ret)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 60, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = ((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_t_1);
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":53
+  /* "pybitset/backends/cython/_bitset.pyx":56
  *             bitset_fill(self._bitset)
  * 
  *     cpdef inline BitSet copy(self):             # <<<<<<<<<<<<<<
  *         cdef bitset_t *ret
  *         with nogil:
  */
 
@@ -2251,15 +2311,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("copy", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((PyObject *)__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_copy(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_copy(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 56, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2268,55 +2328,55 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":59
+/* "pybitset/backends/cython/_bitset.pyx":62
  *         return BitSet.from_ptr(ret)
  * 
  *     cpdef inline bint resize(self, size_t newarraysize, bint padwithzeroes):             # <<<<<<<<<<<<<<
  *         cdef bint ret
  *         with nogil:
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_11resize(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static CYTHON_INLINE int __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_resize(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, size_t __pyx_v_newarraysize, int __pyx_v_padwithzeroes, CYTHON_UNUSED int __pyx_skip_dispatch) {
   int __pyx_v_ret;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("resize", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":61
+  /* "pybitset/backends/cython/_bitset.pyx":64
  *     cpdef inline bint resize(self, size_t newarraysize, bint padwithzeroes):
  *         cdef bint ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_resize(self._bitset,  newarraysize, padwithzeroes)
  *         return ret
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":62
+        /* "pybitset/backends/cython/_bitset.pyx":65
  *         cdef bint ret
  *         with nogil:
  *             ret = bitset_resize(self._bitset,  newarraysize, padwithzeroes)             # <<<<<<<<<<<<<<
  *         return ret
  * 
  */
         __pyx_v_ret = bitset_resize(__pyx_v_self->_bitset, __pyx_v_newarraysize, __pyx_v_padwithzeroes);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":61
+      /* "pybitset/backends/cython/_bitset.pyx":64
  *     cpdef inline bint resize(self, size_t newarraysize, bint padwithzeroes):
  *         cdef bint ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_resize(self._bitset,  newarraysize, padwithzeroes)
  *         return ret
  */
       /*finally:*/ {
@@ -2327,25 +2387,25 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":63
+  /* "pybitset/backends/cython/_bitset.pyx":66
  *         with nogil:
  *             ret = bitset_resize(self._bitset,  newarraysize, padwithzeroes)
  *         return ret             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline size_t size_in_bytes(self):
  */
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":59
+  /* "pybitset/backends/cython/_bitset.pyx":62
  *         return BitSet.from_ptr(ret)
  * 
  *     cpdef inline bint resize(self, size_t newarraysize, bint padwithzeroes):             # <<<<<<<<<<<<<<
  *         cdef bint ret
  *         with nogil:
  */
 
@@ -2386,32 +2446,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_newarraysize)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_padwithzeroes)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("resize", 1, 2, 2, 1); __PYX_ERR(0, 59, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("resize", 1, 2, 2, 1); __PYX_ERR(0, 62, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "resize") < 0)) __PYX_ERR(0, 59, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "resize") < 0)) __PYX_ERR(0, 62, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_newarraysize = __Pyx_PyInt_As_size_t(values[0]); if (unlikely((__pyx_v_newarraysize == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 59, __pyx_L3_error)
-    __pyx_v_padwithzeroes = __Pyx_PyObject_IsTrue(values[1]); if (unlikely((__pyx_v_padwithzeroes == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 59, __pyx_L3_error)
+    __pyx_v_newarraysize = __Pyx_PyInt_As_size_t(values[0]); if (unlikely((__pyx_v_newarraysize == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 62, __pyx_L3_error)
+    __pyx_v_padwithzeroes = __Pyx_PyObject_IsTrue(values[1]); if (unlikely((__pyx_v_padwithzeroes == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 62, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("resize", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 59, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("resize", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 62, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pybitset.backends.cython._bitset.BitSet.resize", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8pybitset_8backends_6cython_7_bitset_6BitSet_10resize(((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_self), __pyx_v_newarraysize, __pyx_v_padwithzeroes);
 
@@ -2425,15 +2485,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("resize", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_resize(__pyx_v_self, __pyx_v_newarraysize, __pyx_v_padwithzeroes, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 59, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_resize(__pyx_v_self, __pyx_v_newarraysize, __pyx_v_padwithzeroes, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 62, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2442,55 +2502,55 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":65
+/* "pybitset/backends/cython/_bitset.pyx":68
  *         return ret
  * 
  *     cpdef inline size_t size_in_bytes(self):             # <<<<<<<<<<<<<<
  *         cdef size_t ret
  *         with nogil:
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_13size_in_bytes(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
 static CYTHON_INLINE size_t __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_size_in_bytes(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, CYTHON_UNUSED int __pyx_skip_dispatch) {
   size_t __pyx_v_ret;
   size_t __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("size_in_bytes", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":67
+  /* "pybitset/backends/cython/_bitset.pyx":70
  *     cpdef inline size_t size_in_bytes(self):
  *         cdef size_t ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_size_in_bytes(self._bitset)
  *         return ret
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":68
+        /* "pybitset/backends/cython/_bitset.pyx":71
  *         cdef size_t ret
  *         with nogil:
  *             ret = bitset_size_in_bytes(self._bitset)             # <<<<<<<<<<<<<<
  *         return ret
  * 
  */
         __pyx_v_ret = bitset_size_in_bytes(__pyx_v_self->_bitset);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":67
+      /* "pybitset/backends/cython/_bitset.pyx":70
  *     cpdef inline size_t size_in_bytes(self):
  *         cdef size_t ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_size_in_bytes(self._bitset)
  *         return ret
  */
       /*finally:*/ {
@@ -2501,25 +2561,25 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":69
+  /* "pybitset/backends/cython/_bitset.pyx":72
  *         with nogil:
  *             ret = bitset_size_in_bytes(self._bitset)
  *         return ret             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline size_t size_in_bits(self):
  */
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":65
+  /* "pybitset/backends/cython/_bitset.pyx":68
  *         return ret
  * 
  *     cpdef inline size_t size_in_bytes(self):             # <<<<<<<<<<<<<<
  *         cdef size_t ret
  *         with nogil:
  */
 
@@ -2548,15 +2608,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("size_in_bytes", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_size_in_bytes(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 65, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_size_in_bytes(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2565,55 +2625,55 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":71
+/* "pybitset/backends/cython/_bitset.pyx":74
  *         return ret
  * 
  *     cpdef inline size_t size_in_bits(self):             # <<<<<<<<<<<<<<
  *         cdef size_t ret
  *         with nogil:
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_15size_in_bits(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
 static CYTHON_INLINE size_t __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_size_in_bits(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, CYTHON_UNUSED int __pyx_skip_dispatch) {
   size_t __pyx_v_ret;
   size_t __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("size_in_bits", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":73
+  /* "pybitset/backends/cython/_bitset.pyx":76
  *     cpdef inline size_t size_in_bits(self):
  *         cdef size_t ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_size_in_bits(self._bitset)
  *         return ret
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":74
+        /* "pybitset/backends/cython/_bitset.pyx":77
  *         cdef size_t ret
  *         with nogil:
  *             ret = bitset_size_in_bits(self._bitset)             # <<<<<<<<<<<<<<
  *         return ret
  * 
  */
         __pyx_v_ret = bitset_size_in_bits(__pyx_v_self->_bitset);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":73
+      /* "pybitset/backends/cython/_bitset.pyx":76
  *     cpdef inline size_t size_in_bits(self):
  *         cdef size_t ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_size_in_bits(self._bitset)
  *         return ret
  */
       /*finally:*/ {
@@ -2624,25 +2684,25 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":75
+  /* "pybitset/backends/cython/_bitset.pyx":78
  *         with nogil:
  *             ret = bitset_size_in_bits(self._bitset)
  *         return ret             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline size_t size_in_words(self):
  */
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":71
+  /* "pybitset/backends/cython/_bitset.pyx":74
  *         return ret
  * 
  *     cpdef inline size_t size_in_bits(self):             # <<<<<<<<<<<<<<
  *         cdef size_t ret
  *         with nogil:
  */
 
@@ -2671,15 +2731,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("size_in_bits", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_size_in_bits(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 71, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_size_in_bits(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 74, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2688,55 +2748,55 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":77
+/* "pybitset/backends/cython/_bitset.pyx":80
  *         return ret
  * 
  *     cpdef inline size_t size_in_words(self):             # <<<<<<<<<<<<<<
  *         cdef size_t ret
  *         with nogil:
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_17size_in_words(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
 static CYTHON_INLINE size_t __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_size_in_words(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, CYTHON_UNUSED int __pyx_skip_dispatch) {
   size_t __pyx_v_ret;
   size_t __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("size_in_words", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":79
+  /* "pybitset/backends/cython/_bitset.pyx":82
  *     cpdef inline size_t size_in_words(self):
  *         cdef size_t ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_size_in_words(self._bitset)
  *         return ret
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":80
+        /* "pybitset/backends/cython/_bitset.pyx":83
  *         cdef size_t ret
  *         with nogil:
  *             ret = bitset_size_in_words(self._bitset)             # <<<<<<<<<<<<<<
  *         return ret
  * 
  */
         __pyx_v_ret = bitset_size_in_words(__pyx_v_self->_bitset);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":79
+      /* "pybitset/backends/cython/_bitset.pyx":82
  *     cpdef inline size_t size_in_words(self):
  *         cdef size_t ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_size_in_words(self._bitset)
  *         return ret
  */
       /*finally:*/ {
@@ -2747,25 +2807,25 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":81
+  /* "pybitset/backends/cython/_bitset.pyx":84
  *         with nogil:
  *             ret = bitset_size_in_words(self._bitset)
  *         return ret             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline bint grow(self, size_t newarraysize):
  */
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":77
+  /* "pybitset/backends/cython/_bitset.pyx":80
  *         return ret
  * 
  *     cpdef inline size_t size_in_words(self):             # <<<<<<<<<<<<<<
  *         cdef size_t ret
  *         with nogil:
  */
 
@@ -2794,15 +2854,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("size_in_words", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_size_in_words(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_size_in_words(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 80, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2811,55 +2871,55 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":83
+/* "pybitset/backends/cython/_bitset.pyx":86
  *         return ret
  * 
  *     cpdef inline bint grow(self, size_t newarraysize):             # <<<<<<<<<<<<<<
  *         cdef bint ret
  *         with nogil:
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_19grow(PyObject *__pyx_v_self, PyObject *__pyx_arg_newarraysize); /*proto*/
 static CYTHON_INLINE int __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_grow(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, size_t __pyx_v_newarraysize, CYTHON_UNUSED int __pyx_skip_dispatch) {
   int __pyx_v_ret;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("grow", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":85
+  /* "pybitset/backends/cython/_bitset.pyx":88
  *     cpdef inline bint grow(self, size_t newarraysize):
  *         cdef bint ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_grow(self._bitset, newarraysize)
  *         return ret
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":86
+        /* "pybitset/backends/cython/_bitset.pyx":89
  *         cdef bint ret
  *         with nogil:
  *             ret = bitset_grow(self._bitset, newarraysize)             # <<<<<<<<<<<<<<
  *         return ret
  * 
  */
         __pyx_v_ret = bitset_grow(__pyx_v_self->_bitset, __pyx_v_newarraysize);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":85
+      /* "pybitset/backends/cython/_bitset.pyx":88
  *     cpdef inline bint grow(self, size_t newarraysize):
  *         cdef bint ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_grow(self._bitset, newarraysize)
  *         return ret
  */
       /*finally:*/ {
@@ -2870,25 +2930,25 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":87
+  /* "pybitset/backends/cython/_bitset.pyx":90
  *         with nogil:
  *             ret = bitset_grow(self._bitset, newarraysize)
  *         return ret             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline bint trim(self):
  */
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":83
+  /* "pybitset/backends/cython/_bitset.pyx":86
  *         return ret
  * 
  *     cpdef inline bint grow(self, size_t newarraysize):             # <<<<<<<<<<<<<<
  *         cdef bint ret
  *         with nogil:
  */
 
@@ -2906,15 +2966,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("grow (wrapper)", 0);
   assert(__pyx_arg_newarraysize); {
-    __pyx_v_newarraysize = __Pyx_PyInt_As_size_t(__pyx_arg_newarraysize); if (unlikely((__pyx_v_newarraysize == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 83, __pyx_L3_error)
+    __pyx_v_newarraysize = __Pyx_PyInt_As_size_t(__pyx_arg_newarraysize); if (unlikely((__pyx_v_newarraysize == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 86, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("pybitset.backends.cython._bitset.BitSet.grow", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
@@ -2930,15 +2990,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("grow", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_grow(__pyx_v_self, __pyx_v_newarraysize, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 83, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_grow(__pyx_v_self, __pyx_v_newarraysize, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2947,55 +3007,55 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":89
+/* "pybitset/backends/cython/_bitset.pyx":92
  *         return ret
  * 
  *     cpdef inline bint trim(self):             # <<<<<<<<<<<<<<
  *         cdef bint ret
  *         with nogil:
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_21trim(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
 static CYTHON_INLINE int __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_trim(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, CYTHON_UNUSED int __pyx_skip_dispatch) {
   int __pyx_v_ret;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("trim", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":91
+  /* "pybitset/backends/cython/_bitset.pyx":94
  *     cpdef inline bint trim(self):
  *         cdef bint ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_trim(self._bitset)
  *         return ret
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":92
+        /* "pybitset/backends/cython/_bitset.pyx":95
  *         cdef bint ret
  *         with nogil:
  *             ret = bitset_trim(self._bitset)             # <<<<<<<<<<<<<<
  *         return ret
  * 
  */
         __pyx_v_ret = bitset_trim(__pyx_v_self->_bitset);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":91
+      /* "pybitset/backends/cython/_bitset.pyx":94
  *     cpdef inline bint trim(self):
  *         cdef bint ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_trim(self._bitset)
  *         return ret
  */
       /*finally:*/ {
@@ -3006,25 +3066,25 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":93
+  /* "pybitset/backends/cython/_bitset.pyx":96
  *         with nogil:
  *             ret = bitset_trim(self._bitset)
  *         return ret             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline shift_left(self, size_t s):
  */
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":89
+  /* "pybitset/backends/cython/_bitset.pyx":92
  *         return ret
  * 
  *     cpdef inline bint trim(self):             # <<<<<<<<<<<<<<
  *         cdef bint ret
  *         with nogil:
  */
 
@@ -3053,15 +3113,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("trim", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_trim(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 89, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_trim(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -3070,54 +3130,54 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":95
+/* "pybitset/backends/cython/_bitset.pyx":98
  *         return ret
  * 
  *     cpdef inline shift_left(self, size_t s):             # <<<<<<<<<<<<<<
  *         with nogil:
  *             bitset_shift_left(self._bitset, s)
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_23shift_left(PyObject *__pyx_v_self, PyObject *__pyx_arg_s); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_shift_left(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, size_t __pyx_v_s, CYTHON_UNUSED int __pyx_skip_dispatch) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("shift_left", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":96
+  /* "pybitset/backends/cython/_bitset.pyx":99
  * 
  *     cpdef inline shift_left(self, size_t s):
  *         with nogil:             # <<<<<<<<<<<<<<
  *             bitset_shift_left(self._bitset, s)
  * 
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":97
+        /* "pybitset/backends/cython/_bitset.pyx":100
  *     cpdef inline shift_left(self, size_t s):
  *         with nogil:
  *             bitset_shift_left(self._bitset, s)             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline shift_right(self, size_t s):
  */
         bitset_shift_left(__pyx_v_self->_bitset, __pyx_v_s);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":96
+      /* "pybitset/backends/cython/_bitset.pyx":99
  * 
  *     cpdef inline shift_left(self, size_t s):
  *         with nogil:             # <<<<<<<<<<<<<<
  *             bitset_shift_left(self._bitset, s)
  * 
  */
       /*finally:*/ {
@@ -3128,15 +3188,15 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":95
+  /* "pybitset/backends/cython/_bitset.pyx":98
  *         return ret
  * 
  *     cpdef inline shift_left(self, size_t s):             # <<<<<<<<<<<<<<
  *         with nogil:
  *             bitset_shift_left(self._bitset, s)
  */
 
@@ -3155,15 +3215,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("shift_left (wrapper)", 0);
   assert(__pyx_arg_s); {
-    __pyx_v_s = __Pyx_PyInt_As_size_t(__pyx_arg_s); if (unlikely((__pyx_v_s == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 95, __pyx_L3_error)
+    __pyx_v_s = __Pyx_PyInt_As_size_t(__pyx_arg_s); if (unlikely((__pyx_v_s == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 98, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("pybitset.backends.cython._bitset.BitSet.shift_left", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
@@ -3179,15 +3239,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("shift_left", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_shift_left(__pyx_v_self, __pyx_v_s, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 95, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_shift_left(__pyx_v_self, __pyx_v_s, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -3196,54 +3256,54 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":99
+/* "pybitset/backends/cython/_bitset.pyx":102
  *             bitset_shift_left(self._bitset, s)
  * 
  *     cpdef inline shift_right(self, size_t s):             # <<<<<<<<<<<<<<
  *         with nogil:
  *             bitset_shift_right(self._bitset, s)
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_25shift_right(PyObject *__pyx_v_self, PyObject *__pyx_arg_s); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_shift_right(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, size_t __pyx_v_s, CYTHON_UNUSED int __pyx_skip_dispatch) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("shift_right", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":100
+  /* "pybitset/backends/cython/_bitset.pyx":103
  * 
  *     cpdef inline shift_right(self, size_t s):
  *         with nogil:             # <<<<<<<<<<<<<<
  *             bitset_shift_right(self._bitset, s)
  * 
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":101
+        /* "pybitset/backends/cython/_bitset.pyx":104
  *     cpdef inline shift_right(self, size_t s):
  *         with nogil:
  *             bitset_shift_right(self._bitset, s)             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline set(self,  size_t i):
  */
         bitset_shift_right(__pyx_v_self->_bitset, __pyx_v_s);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":100
+      /* "pybitset/backends/cython/_bitset.pyx":103
  * 
  *     cpdef inline shift_right(self, size_t s):
  *         with nogil:             # <<<<<<<<<<<<<<
  *             bitset_shift_right(self._bitset, s)
  * 
  */
       /*finally:*/ {
@@ -3254,15 +3314,15 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":99
+  /* "pybitset/backends/cython/_bitset.pyx":102
  *             bitset_shift_left(self._bitset, s)
  * 
  *     cpdef inline shift_right(self, size_t s):             # <<<<<<<<<<<<<<
  *         with nogil:
  *             bitset_shift_right(self._bitset, s)
  */
 
@@ -3281,15 +3341,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("shift_right (wrapper)", 0);
   assert(__pyx_arg_s); {
-    __pyx_v_s = __Pyx_PyInt_As_size_t(__pyx_arg_s); if (unlikely((__pyx_v_s == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 99, __pyx_L3_error)
+    __pyx_v_s = __Pyx_PyInt_As_size_t(__pyx_arg_s); if (unlikely((__pyx_v_s == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 102, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("pybitset.backends.cython._bitset.BitSet.shift_right", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
@@ -3305,15 +3365,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("shift_right", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_shift_right(__pyx_v_self, __pyx_v_s, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_shift_right(__pyx_v_self, __pyx_v_s, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 102, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -3322,54 +3382,54 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":103
+/* "pybitset/backends/cython/_bitset.pyx":106
  *             bitset_shift_right(self._bitset, s)
  * 
  *     cpdef inline set(self,  size_t i):             # <<<<<<<<<<<<<<
  *         with nogil:
  *             bitset_set(self._bitset, i)
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_27set(PyObject *__pyx_v_self, PyObject *__pyx_arg_i); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_set(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, size_t __pyx_v_i, CYTHON_UNUSED int __pyx_skip_dispatch) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":104
+  /* "pybitset/backends/cython/_bitset.pyx":107
  * 
  *     cpdef inline set(self,  size_t i):
  *         with nogil:             # <<<<<<<<<<<<<<
  *             bitset_set(self._bitset, i)
  * 
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":105
+        /* "pybitset/backends/cython/_bitset.pyx":108
  *     cpdef inline set(self,  size_t i):
  *         with nogil:
  *             bitset_set(self._bitset, i)             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline set_to_value(self, size_t i, bint flag):
  */
         bitset_set(__pyx_v_self->_bitset, __pyx_v_i);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":104
+      /* "pybitset/backends/cython/_bitset.pyx":107
  * 
  *     cpdef inline set(self,  size_t i):
  *         with nogil:             # <<<<<<<<<<<<<<
  *             bitset_set(self._bitset, i)
  * 
  */
       /*finally:*/ {
@@ -3380,15 +3440,15 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":103
+  /* "pybitset/backends/cython/_bitset.pyx":106
  *             bitset_shift_right(self._bitset, s)
  * 
  *     cpdef inline set(self,  size_t i):             # <<<<<<<<<<<<<<
  *         with nogil:
  *             bitset_set(self._bitset, i)
  */
 
@@ -3407,15 +3467,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set (wrapper)", 0);
   assert(__pyx_arg_i); {
-    __pyx_v_i = __Pyx_PyInt_As_size_t(__pyx_arg_i); if (unlikely((__pyx_v_i == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 103, __pyx_L3_error)
+    __pyx_v_i = __Pyx_PyInt_As_size_t(__pyx_arg_i); if (unlikely((__pyx_v_i == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 106, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("pybitset.backends.cython._bitset.BitSet.set", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
@@ -3431,15 +3491,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_set(__pyx_v_self, __pyx_v_i, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 103, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_set(__pyx_v_self, __pyx_v_i, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -3448,54 +3508,54 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":107
+/* "pybitset/backends/cython/_bitset.pyx":110
  *             bitset_set(self._bitset, i)
  * 
  *     cpdef inline set_to_value(self, size_t i, bint flag):             # <<<<<<<<<<<<<<
  *         with nogil:
  *             bitset_set_to_value(self._bitset, i, flag)
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_29set_to_value(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_set_to_value(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, size_t __pyx_v_i, int __pyx_v_flag, CYTHON_UNUSED int __pyx_skip_dispatch) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_to_value", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":108
+  /* "pybitset/backends/cython/_bitset.pyx":111
  * 
  *     cpdef inline set_to_value(self, size_t i, bint flag):
  *         with nogil:             # <<<<<<<<<<<<<<
  *             bitset_set_to_value(self._bitset, i, flag)
  * 
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":109
+        /* "pybitset/backends/cython/_bitset.pyx":112
  *     cpdef inline set_to_value(self, size_t i, bint flag):
  *         with nogil:
  *             bitset_set_to_value(self._bitset, i, flag)             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline bint get(self, size_t i):
  */
         bitset_set_to_value(__pyx_v_self->_bitset, __pyx_v_i, __pyx_v_flag);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":108
+      /* "pybitset/backends/cython/_bitset.pyx":111
  * 
  *     cpdef inline set_to_value(self, size_t i, bint flag):
  *         with nogil:             # <<<<<<<<<<<<<<
  *             bitset_set_to_value(self._bitset, i, flag)
  * 
  */
       /*finally:*/ {
@@ -3506,15 +3566,15 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":107
+  /* "pybitset/backends/cython/_bitset.pyx":110
  *             bitset_set(self._bitset, i)
  * 
  *     cpdef inline set_to_value(self, size_t i, bint flag):             # <<<<<<<<<<<<<<
  *         with nogil:
  *             bitset_set_to_value(self._bitset, i, flag)
  */
 
@@ -3556,32 +3616,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_i)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_flag)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("set_to_value", 1, 2, 2, 1); __PYX_ERR(0, 107, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("set_to_value", 1, 2, 2, 1); __PYX_ERR(0, 110, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "set_to_value") < 0)) __PYX_ERR(0, 107, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "set_to_value") < 0)) __PYX_ERR(0, 110, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_i = __Pyx_PyInt_As_size_t(values[0]); if (unlikely((__pyx_v_i == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 107, __pyx_L3_error)
-    __pyx_v_flag = __Pyx_PyObject_IsTrue(values[1]); if (unlikely((__pyx_v_flag == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 107, __pyx_L3_error)
+    __pyx_v_i = __Pyx_PyInt_As_size_t(values[0]); if (unlikely((__pyx_v_i == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 110, __pyx_L3_error)
+    __pyx_v_flag = __Pyx_PyObject_IsTrue(values[1]); if (unlikely((__pyx_v_flag == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 110, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("set_to_value", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 107, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("set_to_value", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 110, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pybitset.backends.cython._bitset.BitSet.set_to_value", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_8pybitset_8backends_6cython_7_bitset_6BitSet_28set_to_value(((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_self), __pyx_v_i, __pyx_v_flag);
 
@@ -3595,15 +3655,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_to_value", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_set_to_value(__pyx_v_self, __pyx_v_i, __pyx_v_flag, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 107, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_set_to_value(__pyx_v_self, __pyx_v_i, __pyx_v_flag, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -3612,55 +3672,55 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":111
+/* "pybitset/backends/cython/_bitset.pyx":114
  *             bitset_set_to_value(self._bitset, i, flag)
  * 
  *     cpdef inline bint get(self, size_t i):             # <<<<<<<<<<<<<<
  *         cdef bint ret
  *         with nogil:
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_31get(PyObject *__pyx_v_self, PyObject *__pyx_arg_i); /*proto*/
 static CYTHON_INLINE int __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_get(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, size_t __pyx_v_i, CYTHON_UNUSED int __pyx_skip_dispatch) {
   int __pyx_v_ret;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":113
+  /* "pybitset/backends/cython/_bitset.pyx":116
  *     cpdef inline bint get(self, size_t i):
  *         cdef bint ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_get(self._bitset, i)
  *         return ret
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":114
+        /* "pybitset/backends/cython/_bitset.pyx":117
  *         cdef bint ret
  *         with nogil:
  *             ret = bitset_get(self._bitset, i)             # <<<<<<<<<<<<<<
  *         return ret
  * 
  */
         __pyx_v_ret = bitset_get(__pyx_v_self->_bitset, __pyx_v_i);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":113
+      /* "pybitset/backends/cython/_bitset.pyx":116
  *     cpdef inline bint get(self, size_t i):
  *         cdef bint ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_get(self._bitset, i)
  *         return ret
  */
       /*finally:*/ {
@@ -3671,25 +3731,25 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":115
+  /* "pybitset/backends/cython/_bitset.pyx":118
  *         with nogil:
  *             ret = bitset_get(self._bitset, i)
  *         return ret             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline size_t count(self):
  */
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":111
+  /* "pybitset/backends/cython/_bitset.pyx":114
  *             bitset_set_to_value(self._bitset, i, flag)
  * 
  *     cpdef inline bint get(self, size_t i):             # <<<<<<<<<<<<<<
  *         cdef bint ret
  *         with nogil:
  */
 
@@ -3707,15 +3767,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get (wrapper)", 0);
   assert(__pyx_arg_i); {
-    __pyx_v_i = __Pyx_PyInt_As_size_t(__pyx_arg_i); if (unlikely((__pyx_v_i == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 111, __pyx_L3_error)
+    __pyx_v_i = __Pyx_PyInt_As_size_t(__pyx_arg_i); if (unlikely((__pyx_v_i == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 114, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("pybitset.backends.cython._bitset.BitSet.get", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
@@ -3731,15 +3791,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_get(__pyx_v_self, __pyx_v_i, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_get(__pyx_v_self, __pyx_v_i, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 114, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -3748,55 +3808,55 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":117
+/* "pybitset/backends/cython/_bitset.pyx":120
  *         return ret
  * 
  *     cpdef inline size_t count(self):             # <<<<<<<<<<<<<<
  *         cdef size_t ret
  *         with nogil:
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_33count(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
 static CYTHON_INLINE size_t __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_count(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, CYTHON_UNUSED int __pyx_skip_dispatch) {
   size_t __pyx_v_ret;
   size_t __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("count", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":119
+  /* "pybitset/backends/cython/_bitset.pyx":122
  *     cpdef inline size_t count(self):
  *         cdef size_t ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_count(self._bitset)
  *         return ret
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":120
+        /* "pybitset/backends/cython/_bitset.pyx":123
  *         cdef size_t ret
  *         with nogil:
  *             ret = bitset_count(self._bitset)             # <<<<<<<<<<<<<<
  *         return ret
  * 
  */
         __pyx_v_ret = bitset_count(__pyx_v_self->_bitset);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":119
+      /* "pybitset/backends/cython/_bitset.pyx":122
  *     cpdef inline size_t count(self):
  *         cdef size_t ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_count(self._bitset)
  *         return ret
  */
       /*finally:*/ {
@@ -3807,25 +3867,25 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":121
+  /* "pybitset/backends/cython/_bitset.pyx":124
  *         with nogil:
  *             ret = bitset_count(self._bitset)
  *         return ret             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline size_t minimum(self):
  */
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":117
+  /* "pybitset/backends/cython/_bitset.pyx":120
  *         return ret
  * 
  *     cpdef inline size_t count(self):             # <<<<<<<<<<<<<<
  *         cdef size_t ret
  *         with nogil:
  */
 
@@ -3854,15 +3914,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("count", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_count(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 117, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_count(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 120, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -3871,55 +3931,55 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":123
+/* "pybitset/backends/cython/_bitset.pyx":126
  *         return ret
  * 
  *     cpdef inline size_t minimum(self):             # <<<<<<<<<<<<<<
  *         cdef size_t ret
  *         with nogil:
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_35minimum(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
 static CYTHON_INLINE size_t __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_minimum(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, CYTHON_UNUSED int __pyx_skip_dispatch) {
   size_t __pyx_v_ret;
   size_t __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("minimum", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":125
+  /* "pybitset/backends/cython/_bitset.pyx":128
  *     cpdef inline size_t minimum(self):
  *         cdef size_t ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_minimum(self._bitset)
  *         return ret
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":126
+        /* "pybitset/backends/cython/_bitset.pyx":129
  *         cdef size_t ret
  *         with nogil:
  *             ret = bitset_minimum(self._bitset)             # <<<<<<<<<<<<<<
  *         return ret
  * 
  */
         __pyx_v_ret = bitset_minimum(__pyx_v_self->_bitset);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":125
+      /* "pybitset/backends/cython/_bitset.pyx":128
  *     cpdef inline size_t minimum(self):
  *         cdef size_t ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_minimum(self._bitset)
  *         return ret
  */
       /*finally:*/ {
@@ -3930,25 +3990,25 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":127
+  /* "pybitset/backends/cython/_bitset.pyx":130
  *         with nogil:
  *             ret = bitset_minimum(self._bitset)
  *         return ret             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline size_t maximum(self):
  */
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":123
+  /* "pybitset/backends/cython/_bitset.pyx":126
  *         return ret
  * 
  *     cpdef inline size_t minimum(self):             # <<<<<<<<<<<<<<
  *         cdef size_t ret
  *         with nogil:
  */
 
@@ -3977,15 +4037,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("minimum", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_minimum(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 123, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_minimum(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 126, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -3994,55 +4054,55 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":129
+/* "pybitset/backends/cython/_bitset.pyx":132
  *         return ret
  * 
  *     cpdef inline size_t maximum(self):             # <<<<<<<<<<<<<<
  *         cdef size_t ret
  *         with nogil:
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_37maximum(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
 static CYTHON_INLINE size_t __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_maximum(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, CYTHON_UNUSED int __pyx_skip_dispatch) {
   size_t __pyx_v_ret;
   size_t __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("maximum", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":131
+  /* "pybitset/backends/cython/_bitset.pyx":134
  *     cpdef inline size_t maximum(self):
  *         cdef size_t ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_maximum(self._bitset)
  *         return ret
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":132
+        /* "pybitset/backends/cython/_bitset.pyx":135
  *         cdef size_t ret
  *         with nogil:
  *             ret = bitset_maximum(self._bitset)             # <<<<<<<<<<<<<<
  *         return ret
  * 
  */
         __pyx_v_ret = bitset_maximum(__pyx_v_self->_bitset);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":131
+      /* "pybitset/backends/cython/_bitset.pyx":134
  *     cpdef inline size_t maximum(self):
  *         cdef size_t ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_maximum(self._bitset)
  *         return ret
  */
       /*finally:*/ {
@@ -4053,25 +4113,25 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":133
+  /* "pybitset/backends/cython/_bitset.pyx":136
  *         with nogil:
  *             ret = bitset_maximum(self._bitset)
  *         return ret             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline bint inplace_union(self, BitSet b2):
  */
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":129
+  /* "pybitset/backends/cython/_bitset.pyx":132
  *         return ret
  * 
  *     cpdef inline size_t maximum(self):             # <<<<<<<<<<<<<<
  *         cdef size_t ret
  *         with nogil:
  */
 
@@ -4100,15 +4160,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("maximum", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_maximum(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 129, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_maximum(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 132, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -4117,55 +4177,55 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":135
+/* "pybitset/backends/cython/_bitset.pyx":138
  *         return ret
  * 
  *     cpdef inline bint inplace_union(self, BitSet b2):             # <<<<<<<<<<<<<<
  *         cdef bint ret
  *         with nogil:
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_39inplace_union(PyObject *__pyx_v_self, PyObject *__pyx_v_b2); /*proto*/
 static CYTHON_INLINE int __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_inplace_union(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_b2, CYTHON_UNUSED int __pyx_skip_dispatch) {
   int __pyx_v_ret;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("inplace_union", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":137
+  /* "pybitset/backends/cython/_bitset.pyx":140
  *     cpdef inline bint inplace_union(self, BitSet b2):
  *         cdef bint ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_inplace_union(self._bitset, b2._bitset)
  *         return ret
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":138
+        /* "pybitset/backends/cython/_bitset.pyx":141
  *         cdef bint ret
  *         with nogil:
  *             ret = bitset_inplace_union(self._bitset, b2._bitset)             # <<<<<<<<<<<<<<
  *         return ret
  * 
  */
         __pyx_v_ret = bitset_inplace_union(__pyx_v_self->_bitset, __pyx_v_b2->_bitset);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":137
+      /* "pybitset/backends/cython/_bitset.pyx":140
  *     cpdef inline bint inplace_union(self, BitSet b2):
  *         cdef bint ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_inplace_union(self._bitset, b2._bitset)
  *         return ret
  */
       /*finally:*/ {
@@ -4176,25 +4236,25 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":139
+  /* "pybitset/backends/cython/_bitset.pyx":142
  *         with nogil:
  *             ret = bitset_inplace_union(self._bitset, b2._bitset)
  *         return ret             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline size_t union_count(self, BitSet b2):
  */
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":135
+  /* "pybitset/backends/cython/_bitset.pyx":138
  *         return ret
  * 
  *     cpdef inline bint inplace_union(self, BitSet b2):             # <<<<<<<<<<<<<<
  *         cdef bint ret
  *         with nogil:
  */
 
@@ -4210,15 +4270,15 @@
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_39inplace_union(PyObject *__pyx_v_self, PyObject *__pyx_v_b2) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("inplace_union (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b2), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b2", 0))) __PYX_ERR(0, 135, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b2), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b2", 0))) __PYX_ERR(0, 138, __pyx_L1_error)
   __pyx_r = __pyx_pf_8pybitset_8backends_6cython_7_bitset_6BitSet_38inplace_union(((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_self), ((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_b2));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -4231,15 +4291,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("inplace_union", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_inplace_union(__pyx_v_self, __pyx_v_b2, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 135, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_inplace_union(__pyx_v_self, __pyx_v_b2, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 138, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -4248,55 +4308,55 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":141
+/* "pybitset/backends/cython/_bitset.pyx":144
  *         return ret
  * 
  *     cpdef inline size_t union_count(self, BitSet b2):             # <<<<<<<<<<<<<<
  *         cdef size_t ret
  *         with nogil:
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_41union_count(PyObject *__pyx_v_self, PyObject *__pyx_v_b2); /*proto*/
 static CYTHON_INLINE size_t __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_union_count(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_b2, CYTHON_UNUSED int __pyx_skip_dispatch) {
   size_t __pyx_v_ret;
   size_t __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("union_count", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":143
+  /* "pybitset/backends/cython/_bitset.pyx":146
  *     cpdef inline size_t union_count(self, BitSet b2):
  *         cdef size_t ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_union_count(self._bitset, b2._bitset)
  *         return ret
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":144
+        /* "pybitset/backends/cython/_bitset.pyx":147
  *         cdef size_t ret
  *         with nogil:
  *             ret = bitset_union_count(self._bitset, b2._bitset)             # <<<<<<<<<<<<<<
  *         return ret
  * 
  */
         __pyx_v_ret = bitset_union_count(__pyx_v_self->_bitset, __pyx_v_b2->_bitset);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":143
+      /* "pybitset/backends/cython/_bitset.pyx":146
  *     cpdef inline size_t union_count(self, BitSet b2):
  *         cdef size_t ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_union_count(self._bitset, b2._bitset)
  *         return ret
  */
       /*finally:*/ {
@@ -4307,25 +4367,25 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":145
+  /* "pybitset/backends/cython/_bitset.pyx":148
  *         with nogil:
  *             ret = bitset_union_count(self._bitset, b2._bitset)
  *         return ret             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline inplace_intersection(self, BitSet b2):
  */
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":141
+  /* "pybitset/backends/cython/_bitset.pyx":144
  *         return ret
  * 
  *     cpdef inline size_t union_count(self, BitSet b2):             # <<<<<<<<<<<<<<
  *         cdef size_t ret
  *         with nogil:
  */
 
@@ -4341,15 +4401,15 @@
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_41union_count(PyObject *__pyx_v_self, PyObject *__pyx_v_b2) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("union_count (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b2), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b2", 0))) __PYX_ERR(0, 141, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b2), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b2", 0))) __PYX_ERR(0, 144, __pyx_L1_error)
   __pyx_r = __pyx_pf_8pybitset_8backends_6cython_7_bitset_6BitSet_40union_count(((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_self), ((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_b2));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -4362,15 +4422,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("union_count", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_union_count(__pyx_v_self, __pyx_v_b2, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 141, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_union_count(__pyx_v_self, __pyx_v_b2, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 144, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -4379,54 +4439,54 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":147
+/* "pybitset/backends/cython/_bitset.pyx":150
  *         return ret
  * 
  *     cpdef inline inplace_intersection(self, BitSet b2):             # <<<<<<<<<<<<<<
  *         with nogil:
  *             bitset_inplace_intersection(self._bitset, b2._bitset)
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_43inplace_intersection(PyObject *__pyx_v_self, PyObject *__pyx_v_b2); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_inplace_intersection(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_b2, CYTHON_UNUSED int __pyx_skip_dispatch) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("inplace_intersection", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":148
+  /* "pybitset/backends/cython/_bitset.pyx":151
  * 
  *     cpdef inline inplace_intersection(self, BitSet b2):
  *         with nogil:             # <<<<<<<<<<<<<<
  *             bitset_inplace_intersection(self._bitset, b2._bitset)
  * 
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":149
+        /* "pybitset/backends/cython/_bitset.pyx":152
  *     cpdef inline inplace_intersection(self, BitSet b2):
  *         with nogil:
  *             bitset_inplace_intersection(self._bitset, b2._bitset)             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline size_t intersection_count(self, BitSet b2):
  */
         bitset_inplace_intersection(__pyx_v_self->_bitset, __pyx_v_b2->_bitset);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":148
+      /* "pybitset/backends/cython/_bitset.pyx":151
  * 
  *     cpdef inline inplace_intersection(self, BitSet b2):
  *         with nogil:             # <<<<<<<<<<<<<<
  *             bitset_inplace_intersection(self._bitset, b2._bitset)
  * 
  */
       /*finally:*/ {
@@ -4437,15 +4497,15 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":147
+  /* "pybitset/backends/cython/_bitset.pyx":150
  *         return ret
  * 
  *     cpdef inline inplace_intersection(self, BitSet b2):             # <<<<<<<<<<<<<<
  *         with nogil:
  *             bitset_inplace_intersection(self._bitset, b2._bitset)
  */
 
@@ -4462,15 +4522,15 @@
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_43inplace_intersection(PyObject *__pyx_v_self, PyObject *__pyx_v_b2) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("inplace_intersection (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b2), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b2", 0))) __PYX_ERR(0, 147, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b2), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b2", 0))) __PYX_ERR(0, 150, __pyx_L1_error)
   __pyx_r = __pyx_pf_8pybitset_8backends_6cython_7_bitset_6BitSet_42inplace_intersection(((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_self), ((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_b2));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -4483,15 +4543,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("inplace_intersection", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_inplace_intersection(__pyx_v_self, __pyx_v_b2, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 147, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_inplace_intersection(__pyx_v_self, __pyx_v_b2, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 150, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -4500,55 +4560,55 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":151
+/* "pybitset/backends/cython/_bitset.pyx":154
  *             bitset_inplace_intersection(self._bitset, b2._bitset)
  * 
  *     cpdef inline size_t intersection_count(self, BitSet b2):             # <<<<<<<<<<<<<<
  *         cdef size_t ret
  *         with nogil:
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_45intersection_count(PyObject *__pyx_v_self, PyObject *__pyx_v_b2); /*proto*/
 static CYTHON_INLINE size_t __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_intersection_count(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_b2, CYTHON_UNUSED int __pyx_skip_dispatch) {
   size_t __pyx_v_ret;
   size_t __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("intersection_count", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":153
+  /* "pybitset/backends/cython/_bitset.pyx":156
  *     cpdef inline size_t intersection_count(self, BitSet b2):
  *         cdef size_t ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_intersection_count(self._bitset, b2._bitset)
  *         return ret
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":154
+        /* "pybitset/backends/cython/_bitset.pyx":157
  *         cdef size_t ret
  *         with nogil:
  *             ret = bitset_intersection_count(self._bitset, b2._bitset)             # <<<<<<<<<<<<<<
  *         return ret
  * 
  */
         __pyx_v_ret = bitset_intersection_count(__pyx_v_self->_bitset, __pyx_v_b2->_bitset);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":153
+      /* "pybitset/backends/cython/_bitset.pyx":156
  *     cpdef inline size_t intersection_count(self, BitSet b2):
  *         cdef size_t ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_intersection_count(self._bitset, b2._bitset)
  *         return ret
  */
       /*finally:*/ {
@@ -4559,25 +4619,25 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":155
+  /* "pybitset/backends/cython/_bitset.pyx":158
  *         with nogil:
  *             ret = bitset_intersection_count(self._bitset, b2._bitset)
  *         return ret             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline bint disjoint(self, BitSet b2):
  */
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":151
+  /* "pybitset/backends/cython/_bitset.pyx":154
  *             bitset_inplace_intersection(self._bitset, b2._bitset)
  * 
  *     cpdef inline size_t intersection_count(self, BitSet b2):             # <<<<<<<<<<<<<<
  *         cdef size_t ret
  *         with nogil:
  */
 
@@ -4593,15 +4653,15 @@
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_45intersection_count(PyObject *__pyx_v_self, PyObject *__pyx_v_b2) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("intersection_count (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b2), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b2", 0))) __PYX_ERR(0, 151, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b2), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b2", 0))) __PYX_ERR(0, 154, __pyx_L1_error)
   __pyx_r = __pyx_pf_8pybitset_8backends_6cython_7_bitset_6BitSet_44intersection_count(((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_self), ((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_b2));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -4614,15 +4674,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("intersection_count", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_intersection_count(__pyx_v_self, __pyx_v_b2, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 151, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_intersection_count(__pyx_v_self, __pyx_v_b2, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 154, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -4631,55 +4691,55 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":157
+/* "pybitset/backends/cython/_bitset.pyx":160
  *         return ret
  * 
  *     cpdef inline bint disjoint(self, BitSet b2):             # <<<<<<<<<<<<<<
  *         cdef bint ret
  *         with nogil:
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_47disjoint(PyObject *__pyx_v_self, PyObject *__pyx_v_b2); /*proto*/
 static CYTHON_INLINE int __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_disjoint(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_b2, CYTHON_UNUSED int __pyx_skip_dispatch) {
   int __pyx_v_ret;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("disjoint", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":159
+  /* "pybitset/backends/cython/_bitset.pyx":162
  *     cpdef inline bint disjoint(self, BitSet b2):
  *         cdef bint ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitsets_disjoint(self._bitset, b2._bitset)
  *         return ret
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":160
+        /* "pybitset/backends/cython/_bitset.pyx":163
  *         cdef bint ret
  *         with nogil:
  *             ret = bitsets_disjoint(self._bitset, b2._bitset)             # <<<<<<<<<<<<<<
  *         return ret
  * 
  */
         __pyx_v_ret = bitsets_disjoint(__pyx_v_self->_bitset, __pyx_v_b2->_bitset);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":159
+      /* "pybitset/backends/cython/_bitset.pyx":162
  *     cpdef inline bint disjoint(self, BitSet b2):
  *         cdef bint ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitsets_disjoint(self._bitset, b2._bitset)
  *         return ret
  */
       /*finally:*/ {
@@ -4690,25 +4750,25 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":161
+  /* "pybitset/backends/cython/_bitset.pyx":164
  *         with nogil:
  *             ret = bitsets_disjoint(self._bitset, b2._bitset)
  *         return ret             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline bint intersect(self, BitSet b2):
  */
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":157
+  /* "pybitset/backends/cython/_bitset.pyx":160
  *         return ret
  * 
  *     cpdef inline bint disjoint(self, BitSet b2):             # <<<<<<<<<<<<<<
  *         cdef bint ret
  *         with nogil:
  */
 
@@ -4724,15 +4784,15 @@
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_47disjoint(PyObject *__pyx_v_self, PyObject *__pyx_v_b2) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("disjoint (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b2), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b2", 0))) __PYX_ERR(0, 157, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b2), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b2", 0))) __PYX_ERR(0, 160, __pyx_L1_error)
   __pyx_r = __pyx_pf_8pybitset_8backends_6cython_7_bitset_6BitSet_46disjoint(((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_self), ((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_b2));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -4745,15 +4805,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("disjoint", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_disjoint(__pyx_v_self, __pyx_v_b2, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 157, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_disjoint(__pyx_v_self, __pyx_v_b2, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 160, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -4762,55 +4822,55 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":163
+/* "pybitset/backends/cython/_bitset.pyx":166
  *         return ret
  * 
  *     cpdef inline bint intersect(self, BitSet b2):             # <<<<<<<<<<<<<<
  *         cdef bint ret
  *         with nogil:
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_49intersect(PyObject *__pyx_v_self, PyObject *__pyx_v_b2); /*proto*/
 static CYTHON_INLINE int __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_intersect(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_b2, CYTHON_UNUSED int __pyx_skip_dispatch) {
   int __pyx_v_ret;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("intersect", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":165
+  /* "pybitset/backends/cython/_bitset.pyx":168
  *     cpdef inline bint intersect(self, BitSet b2):
  *         cdef bint ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitsets_intersect(self._bitset, b2._bitset)
  *         return ret
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":166
+        /* "pybitset/backends/cython/_bitset.pyx":169
  *         cdef bint ret
  *         with nogil:
  *             ret = bitsets_intersect(self._bitset, b2._bitset)             # <<<<<<<<<<<<<<
  *         return ret
  * 
  */
         __pyx_v_ret = bitsets_intersect(__pyx_v_self->_bitset, __pyx_v_b2->_bitset);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":165
+      /* "pybitset/backends/cython/_bitset.pyx":168
  *     cpdef inline bint intersect(self, BitSet b2):
  *         cdef bint ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitsets_intersect(self._bitset, b2._bitset)
  *         return ret
  */
       /*finally:*/ {
@@ -4821,25 +4881,25 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":167
+  /* "pybitset/backends/cython/_bitset.pyx":170
  *         with nogil:
  *             ret = bitsets_intersect(self._bitset, b2._bitset)
  *         return ret             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline bint contains_all(self, BitSet b2):
  */
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":163
+  /* "pybitset/backends/cython/_bitset.pyx":166
  *         return ret
  * 
  *     cpdef inline bint intersect(self, BitSet b2):             # <<<<<<<<<<<<<<
  *         cdef bint ret
  *         with nogil:
  */
 
@@ -4855,15 +4915,15 @@
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_49intersect(PyObject *__pyx_v_self, PyObject *__pyx_v_b2) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("intersect (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b2), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b2", 0))) __PYX_ERR(0, 163, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b2), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b2", 0))) __PYX_ERR(0, 166, __pyx_L1_error)
   __pyx_r = __pyx_pf_8pybitset_8backends_6cython_7_bitset_6BitSet_48intersect(((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_self), ((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_b2));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -4876,15 +4936,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("intersect", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_intersect(__pyx_v_self, __pyx_v_b2, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 163, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_intersect(__pyx_v_self, __pyx_v_b2, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 166, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -4893,55 +4953,55 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":169
+/* "pybitset/backends/cython/_bitset.pyx":172
  *         return ret
  * 
  *     cpdef inline bint contains_all(self, BitSet b2):             # <<<<<<<<<<<<<<
  *         cdef bint ret
  *         with nogil:
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_51contains_all(PyObject *__pyx_v_self, PyObject *__pyx_v_b2); /*proto*/
 static CYTHON_INLINE int __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_contains_all(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_b2, CYTHON_UNUSED int __pyx_skip_dispatch) {
   int __pyx_v_ret;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("contains_all", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":171
+  /* "pybitset/backends/cython/_bitset.pyx":174
  *     cpdef inline bint contains_all(self, BitSet b2):
  *         cdef bint ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_contains_all(self._bitset, b2._bitset)
  *         return ret
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":172
+        /* "pybitset/backends/cython/_bitset.pyx":175
  *         cdef bint ret
  *         with nogil:
  *             ret = bitset_contains_all(self._bitset, b2._bitset)             # <<<<<<<<<<<<<<
  *         return ret
  * 
  */
         __pyx_v_ret = bitset_contains_all(__pyx_v_self->_bitset, __pyx_v_b2->_bitset);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":171
+      /* "pybitset/backends/cython/_bitset.pyx":174
  *     cpdef inline bint contains_all(self, BitSet b2):
  *         cdef bint ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_contains_all(self._bitset, b2._bitset)
  *         return ret
  */
       /*finally:*/ {
@@ -4952,25 +5012,25 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":173
+  /* "pybitset/backends/cython/_bitset.pyx":176
  *         with nogil:
  *             ret = bitset_contains_all(self._bitset, b2._bitset)
  *         return ret             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline inplace_difference(self, BitSet b2):
  */
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":169
+  /* "pybitset/backends/cython/_bitset.pyx":172
  *         return ret
  * 
  *     cpdef inline bint contains_all(self, BitSet b2):             # <<<<<<<<<<<<<<
  *         cdef bint ret
  *         with nogil:
  */
 
@@ -4986,15 +5046,15 @@
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_51contains_all(PyObject *__pyx_v_self, PyObject *__pyx_v_b2) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("contains_all (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b2), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b2", 0))) __PYX_ERR(0, 169, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b2), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b2", 0))) __PYX_ERR(0, 172, __pyx_L1_error)
   __pyx_r = __pyx_pf_8pybitset_8backends_6cython_7_bitset_6BitSet_50contains_all(((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_self), ((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_b2));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -5007,15 +5067,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("contains_all", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_contains_all(__pyx_v_self, __pyx_v_b2, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 169, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_contains_all(__pyx_v_self, __pyx_v_b2, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 172, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -5024,54 +5084,54 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":175
+/* "pybitset/backends/cython/_bitset.pyx":178
  *         return ret
  * 
  *     cpdef inline inplace_difference(self, BitSet b2):             # <<<<<<<<<<<<<<
  *         with nogil:
  *             bitset_inplace_difference(self._bitset, b2._bitset)
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_53inplace_difference(PyObject *__pyx_v_self, PyObject *__pyx_v_b2); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_inplace_difference(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_b2, CYTHON_UNUSED int __pyx_skip_dispatch) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("inplace_difference", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":176
+  /* "pybitset/backends/cython/_bitset.pyx":179
  * 
  *     cpdef inline inplace_difference(self, BitSet b2):
  *         with nogil:             # <<<<<<<<<<<<<<
  *             bitset_inplace_difference(self._bitset, b2._bitset)
  * 
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":177
+        /* "pybitset/backends/cython/_bitset.pyx":180
  *     cpdef inline inplace_difference(self, BitSet b2):
  *         with nogil:
  *             bitset_inplace_difference(self._bitset, b2._bitset)             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline size_t difference_count(self, BitSet b2):
  */
         bitset_inplace_difference(__pyx_v_self->_bitset, __pyx_v_b2->_bitset);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":176
+      /* "pybitset/backends/cython/_bitset.pyx":179
  * 
  *     cpdef inline inplace_difference(self, BitSet b2):
  *         with nogil:             # <<<<<<<<<<<<<<
  *             bitset_inplace_difference(self._bitset, b2._bitset)
  * 
  */
       /*finally:*/ {
@@ -5082,15 +5142,15 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":175
+  /* "pybitset/backends/cython/_bitset.pyx":178
  *         return ret
  * 
  *     cpdef inline inplace_difference(self, BitSet b2):             # <<<<<<<<<<<<<<
  *         with nogil:
  *             bitset_inplace_difference(self._bitset, b2._bitset)
  */
 
@@ -5107,15 +5167,15 @@
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_53inplace_difference(PyObject *__pyx_v_self, PyObject *__pyx_v_b2) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("inplace_difference (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b2), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b2", 0))) __PYX_ERR(0, 175, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b2), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b2", 0))) __PYX_ERR(0, 178, __pyx_L1_error)
   __pyx_r = __pyx_pf_8pybitset_8backends_6cython_7_bitset_6BitSet_52inplace_difference(((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_self), ((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_b2));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -5128,15 +5188,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("inplace_difference", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_inplace_difference(__pyx_v_self, __pyx_v_b2, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 175, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_inplace_difference(__pyx_v_self, __pyx_v_b2, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 178, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -5145,55 +5205,55 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":179
+/* "pybitset/backends/cython/_bitset.pyx":182
  *             bitset_inplace_difference(self._bitset, b2._bitset)
  * 
  *     cpdef inline size_t difference_count(self, BitSet b2):             # <<<<<<<<<<<<<<
  *         cdef size_t ret
  *         with nogil:
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_55difference_count(PyObject *__pyx_v_self, PyObject *__pyx_v_b2); /*proto*/
 static CYTHON_INLINE size_t __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_difference_count(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_b2, CYTHON_UNUSED int __pyx_skip_dispatch) {
   size_t __pyx_v_ret;
   size_t __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("difference_count", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":181
+  /* "pybitset/backends/cython/_bitset.pyx":184
  *     cpdef inline size_t difference_count(self, BitSet b2):
  *         cdef size_t ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_difference_count(self._bitset, b2._bitset)
  *         return ret
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":182
+        /* "pybitset/backends/cython/_bitset.pyx":185
  *         cdef size_t ret
  *         with nogil:
  *             ret = bitset_difference_count(self._bitset, b2._bitset)             # <<<<<<<<<<<<<<
  *         return ret
  * 
  */
         __pyx_v_ret = bitset_difference_count(__pyx_v_self->_bitset, __pyx_v_b2->_bitset);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":181
+      /* "pybitset/backends/cython/_bitset.pyx":184
  *     cpdef inline size_t difference_count(self, BitSet b2):
  *         cdef size_t ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_difference_count(self._bitset, b2._bitset)
  *         return ret
  */
       /*finally:*/ {
@@ -5204,25 +5264,25 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":183
+  /* "pybitset/backends/cython/_bitset.pyx":186
  *         with nogil:
  *             ret = bitset_difference_count(self._bitset, b2._bitset)
  *         return ret             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline bint inplace_symmetric_difference(self, BitSet b2):
  */
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":179
+  /* "pybitset/backends/cython/_bitset.pyx":182
  *             bitset_inplace_difference(self._bitset, b2._bitset)
  * 
  *     cpdef inline size_t difference_count(self, BitSet b2):             # <<<<<<<<<<<<<<
  *         cdef size_t ret
  *         with nogil:
  */
 
@@ -5238,15 +5298,15 @@
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_55difference_count(PyObject *__pyx_v_self, PyObject *__pyx_v_b2) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("difference_count (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b2), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b2", 0))) __PYX_ERR(0, 179, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b2), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b2", 0))) __PYX_ERR(0, 182, __pyx_L1_error)
   __pyx_r = __pyx_pf_8pybitset_8backends_6cython_7_bitset_6BitSet_54difference_count(((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_self), ((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_b2));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -5259,15 +5319,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("difference_count", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_difference_count(__pyx_v_self, __pyx_v_b2, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 179, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_difference_count(__pyx_v_self, __pyx_v_b2, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 182, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -5276,55 +5336,55 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":185
+/* "pybitset/backends/cython/_bitset.pyx":188
  *         return ret
  * 
  *     cpdef inline bint inplace_symmetric_difference(self, BitSet b2):             # <<<<<<<<<<<<<<
  *         cdef bint ret
  *         with nogil:
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_57inplace_symmetric_difference(PyObject *__pyx_v_self, PyObject *__pyx_v_b2); /*proto*/
 static CYTHON_INLINE int __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_inplace_symmetric_difference(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_b2, CYTHON_UNUSED int __pyx_skip_dispatch) {
   int __pyx_v_ret;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("inplace_symmetric_difference", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":187
+  /* "pybitset/backends/cython/_bitset.pyx":190
  *     cpdef inline bint inplace_symmetric_difference(self, BitSet b2):
  *         cdef bint ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_inplace_symmetric_difference(self._bitset, b2._bitset)
  *         return ret
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":188
+        /* "pybitset/backends/cython/_bitset.pyx":191
  *         cdef bint ret
  *         with nogil:
  *             ret = bitset_inplace_symmetric_difference(self._bitset, b2._bitset)             # <<<<<<<<<<<<<<
  *         return ret
  * 
  */
         __pyx_v_ret = bitset_inplace_symmetric_difference(__pyx_v_self->_bitset, __pyx_v_b2->_bitset);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":187
+      /* "pybitset/backends/cython/_bitset.pyx":190
  *     cpdef inline bint inplace_symmetric_difference(self, BitSet b2):
  *         cdef bint ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_inplace_symmetric_difference(self._bitset, b2._bitset)
  *         return ret
  */
       /*finally:*/ {
@@ -5335,25 +5395,25 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":189
+  /* "pybitset/backends/cython/_bitset.pyx":192
  *         with nogil:
  *             ret = bitset_inplace_symmetric_difference(self._bitset, b2._bitset)
  *         return ret             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline size_t symmetric_difference_count(self, BitSet b2):
  */
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":185
+  /* "pybitset/backends/cython/_bitset.pyx":188
  *         return ret
  * 
  *     cpdef inline bint inplace_symmetric_difference(self, BitSet b2):             # <<<<<<<<<<<<<<
  *         cdef bint ret
  *         with nogil:
  */
 
@@ -5369,15 +5429,15 @@
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_57inplace_symmetric_difference(PyObject *__pyx_v_self, PyObject *__pyx_v_b2) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("inplace_symmetric_difference (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b2), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b2", 0))) __PYX_ERR(0, 185, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b2), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b2", 0))) __PYX_ERR(0, 188, __pyx_L1_error)
   __pyx_r = __pyx_pf_8pybitset_8backends_6cython_7_bitset_6BitSet_56inplace_symmetric_difference(((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_self), ((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_b2));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -5390,15 +5450,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("inplace_symmetric_difference", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_inplace_symmetric_difference(__pyx_v_self, __pyx_v_b2, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 185, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_inplace_symmetric_difference(__pyx_v_self, __pyx_v_b2, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 188, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -5407,55 +5467,55 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":191
+/* "pybitset/backends/cython/_bitset.pyx":194
  *         return ret
  * 
  *     cpdef inline size_t symmetric_difference_count(self, BitSet b2):             # <<<<<<<<<<<<<<
  *         cdef size_t ret
  *         with nogil:
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_59symmetric_difference_count(PyObject *__pyx_v_self, PyObject *__pyx_v_b2); /*proto*/
 static CYTHON_INLINE size_t __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_symmetric_difference_count(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_b2, CYTHON_UNUSED int __pyx_skip_dispatch) {
   size_t __pyx_v_ret;
   size_t __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("symmetric_difference_count", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":193
+  /* "pybitset/backends/cython/_bitset.pyx":196
  *     cpdef inline size_t symmetric_difference_count(self, BitSet b2):
  *         cdef size_t ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_symmetric_difference_count(self._bitset,  b2._bitset)
  *         return ret
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":194
+        /* "pybitset/backends/cython/_bitset.pyx":197
  *         cdef size_t ret
  *         with nogil:
  *             ret = bitset_symmetric_difference_count(self._bitset,  b2._bitset)             # <<<<<<<<<<<<<<
  *         return ret
  * 
  */
         __pyx_v_ret = bitset_symmetric_difference_count(__pyx_v_self->_bitset, __pyx_v_b2->_bitset);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":193
+      /* "pybitset/backends/cython/_bitset.pyx":196
  *     cpdef inline size_t symmetric_difference_count(self, BitSet b2):
  *         cdef size_t ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_symmetric_difference_count(self._bitset,  b2._bitset)
  *         return ret
  */
       /*finally:*/ {
@@ -5466,25 +5526,25 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":195
+  /* "pybitset/backends/cython/_bitset.pyx":198
  *         with nogil:
  *             ret = bitset_symmetric_difference_count(self._bitset,  b2._bitset)
  *         return ret             # <<<<<<<<<<<<<<
  * 
  *     def __iter__(self):
  */
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":191
+  /* "pybitset/backends/cython/_bitset.pyx":194
  *         return ret
  * 
  *     cpdef inline size_t symmetric_difference_count(self, BitSet b2):             # <<<<<<<<<<<<<<
  *         cdef size_t ret
  *         with nogil:
  */
 
@@ -5500,15 +5560,15 @@
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_59symmetric_difference_count(PyObject *__pyx_v_self, PyObject *__pyx_v_b2) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("symmetric_difference_count (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b2), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b2", 0))) __PYX_ERR(0, 191, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b2), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b2", 0))) __PYX_ERR(0, 194, __pyx_L1_error)
   __pyx_r = __pyx_pf_8pybitset_8backends_6cython_7_bitset_6BitSet_58symmetric_difference_count(((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_self), ((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)__pyx_v_b2));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -5521,15 +5581,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("symmetric_difference_count", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_symmetric_difference_count(__pyx_v_self, __pyx_v_b2, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 191, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_symmetric_difference_count(__pyx_v_self, __pyx_v_b2, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 194, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -5538,15 +5598,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":197
+/* "pybitset/backends/cython/_bitset.pyx":200
  *         return ret
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         return BitSetIter(self)
  * 
  */
 
@@ -5568,29 +5628,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__iter__", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":198
+  /* "pybitset/backends/cython/_bitset.pyx":201
  * 
  *     def __iter__(self):
  *         return BitSetIter(self)             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline bint for_each(self, object func):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSetIter), ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 198, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSetIter), ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":197
+  /* "pybitset/backends/cython/_bitset.pyx":200
  *         return ret
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         return BitSetIter(self)
  * 
  */
 
@@ -5601,55 +5661,55 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":200
+/* "pybitset/backends/cython/_bitset.pyx":203
  *         return BitSetIter(self)
  * 
  *     cpdef inline bint for_each(self, object func):             # <<<<<<<<<<<<<<
  *         cdef bint ret
  *         with nogil:
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_63for_each(PyObject *__pyx_v_self, PyObject *__pyx_v_func); /*proto*/
 static CYTHON_INLINE int __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_for_each(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, PyObject *__pyx_v_func, CYTHON_UNUSED int __pyx_skip_dispatch) {
   int __pyx_v_ret;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("for_each", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":202
+  /* "pybitset/backends/cython/_bitset.pyx":205
  *     cpdef inline bint for_each(self, object func):
  *         cdef bint ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_for_each(self._bitset, bitset_iterator_func, <void*>func)
  *         return ret
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":203
+        /* "pybitset/backends/cython/_bitset.pyx":206
  *         cdef bint ret
  *         with nogil:
  *             ret = bitset_for_each(self._bitset, bitset_iterator_func, <void*>func)             # <<<<<<<<<<<<<<
  *         return ret
  * 
  */
         __pyx_v_ret = bitset_for_each(__pyx_v_self->_bitset, __pyx_f_8pybitset_8backends_6cython_7_bitset_bitset_iterator_func, ((void *)__pyx_v_func));
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":202
+      /* "pybitset/backends/cython/_bitset.pyx":205
  *     cpdef inline bint for_each(self, object func):
  *         cdef bint ret
  *         with nogil:             # <<<<<<<<<<<<<<
  *             ret = bitset_for_each(self._bitset, bitset_iterator_func, <void*>func)
  *         return ret
  */
       /*finally:*/ {
@@ -5660,25 +5720,25 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":204
+  /* "pybitset/backends/cython/_bitset.pyx":207
  *         with nogil:
  *             ret = bitset_for_each(self._bitset, bitset_iterator_func, <void*>func)
  *         return ret             # <<<<<<<<<<<<<<
  * 
  *     cpdef inline print(self):
  */
   __pyx_r = __pyx_v_ret;
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":200
+  /* "pybitset/backends/cython/_bitset.pyx":203
  *         return BitSetIter(self)
  * 
  *     cpdef inline bint for_each(self, object func):             # <<<<<<<<<<<<<<
  *         cdef bint ret
  *         with nogil:
  */
 
@@ -5707,15 +5767,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("for_each", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_for_each(__pyx_v_self, __pyx_v_func, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 200, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_for_each(__pyx_v_self, __pyx_v_func, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 203, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -5724,54 +5784,54 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":206
+/* "pybitset/backends/cython/_bitset.pyx":209
  *         return ret
  * 
  *     cpdef inline print(self):             # <<<<<<<<<<<<<<
  *         with nogil:
  *             bitset_print(self._bitset)
  */
 
 static PyObject *__pyx_pw_8pybitset_8backends_6cython_7_bitset_6BitSet_65print(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_print(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_self, CYTHON_UNUSED int __pyx_skip_dispatch) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("print", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":207
+  /* "pybitset/backends/cython/_bitset.pyx":210
  * 
  *     cpdef inline print(self):
  *         with nogil:             # <<<<<<<<<<<<<<
  *             bitset_print(self._bitset)
  * 
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "pybitset/backends/cython/_bitset.pyx":208
+        /* "pybitset/backends/cython/_bitset.pyx":211
  *     cpdef inline print(self):
  *         with nogil:
  *             bitset_print(self._bitset)             # <<<<<<<<<<<<<<
  * 
  * @cython.internal
  */
         bitset_print(__pyx_v_self->_bitset);
       }
 
-      /* "pybitset/backends/cython/_bitset.pyx":207
+      /* "pybitset/backends/cython/_bitset.pyx":210
  * 
  *     cpdef inline print(self):
  *         with nogil:             # <<<<<<<<<<<<<<
  *             bitset_print(self._bitset)
  * 
  */
       /*finally:*/ {
@@ -5782,15 +5842,15 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":206
+  /* "pybitset/backends/cython/_bitset.pyx":209
  *         return ret
  * 
  *     cpdef inline print(self):             # <<<<<<<<<<<<<<
  *         with nogil:
  *             bitset_print(self._bitset)
  */
 
@@ -5820,15 +5880,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("print", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_print(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 206, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_8pybitset_8backends_6cython_7_bitset_6BitSet_print(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 209, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -5952,15 +6012,15 @@
   __Pyx_AddTraceback("pybitset.backends.cython._bitset.BitSet.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":219
+/* "pybitset/backends/cython/_bitset.pyx":222
  *         size_t i
  * 
  *     def __cinit__(self, BitSet b):             # <<<<<<<<<<<<<<
  *         self.b = b
  *         self.i = 0
  */
 
@@ -5989,32 +6049,32 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_b)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 219, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 222, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_b = ((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *)values[0]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 219, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 222, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pybitset.backends.cython._bitset.BitSetIter.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b", 0))) __PYX_ERR(0, 219, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_b), __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet, 1, "b", 0))) __PYX_ERR(0, 222, __pyx_L1_error)
   __pyx_r = __pyx_pf_8pybitset_8backends_6cython_7_bitset_10BitSetIter___cinit__(((struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSetIter *)__pyx_v_self), __pyx_v_b);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
@@ -6023,51 +6083,51 @@
 }
 
 static int __pyx_pf_8pybitset_8backends_6cython_7_bitset_10BitSetIter___cinit__(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSetIter *__pyx_v_self, struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSet *__pyx_v_b) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":220
+  /* "pybitset/backends/cython/_bitset.pyx":223
  * 
  *     def __cinit__(self, BitSet b):
  *         self.b = b             # <<<<<<<<<<<<<<
  *         self.i = 0
  * 
  */
   __Pyx_INCREF(((PyObject *)__pyx_v_b));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_b));
   __Pyx_GOTREF(__pyx_v_self->b);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->b));
   __pyx_v_self->b = __pyx_v_b;
 
-  /* "pybitset/backends/cython/_bitset.pyx":221
+  /* "pybitset/backends/cython/_bitset.pyx":224
  *     def __cinit__(self, BitSet b):
  *         self.b = b
  *         self.i = 0             # <<<<<<<<<<<<<<
  * 
  *     def __iter__(self):
  */
   __pyx_v_self->i = 0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":219
+  /* "pybitset/backends/cython/_bitset.pyx":222
  *         size_t i
  * 
  *     def __cinit__(self, BitSet b):             # <<<<<<<<<<<<<<
  *         self.b = b
  *         self.i = 0
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":223
+/* "pybitset/backends/cython/_bitset.pyx":226
  *         self.i = 0
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
 
@@ -6085,42 +6145,42 @@
 }
 
 static PyObject *__pyx_pf_8pybitset_8backends_6cython_7_bitset_10BitSetIter_2__iter__(struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSetIter *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__iter__", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":224
+  /* "pybitset/backends/cython/_bitset.pyx":227
  * 
  *     def __iter__(self):
  *         return self             # <<<<<<<<<<<<<<
  * 
  *     def __next__(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __pyx_r = ((PyObject *)__pyx_v_self);
   goto __pyx_L0;
 
-  /* "pybitset/backends/cython/_bitset.pyx":223
+  /* "pybitset/backends/cython/_bitset.pyx":226
  *         self.i = 0
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pybitset/backends/cython/_bitset.pyx":226
+/* "pybitset/backends/cython/_bitset.pyx":229
  *         return self
  * 
  *     def __next__(self):             # <<<<<<<<<<<<<<
  *         cdef size_t tmp
  *         if bitset_next_set_bit(self.b._bitset, &self.i):
  */
 
@@ -6145,77 +6205,77 @@
   size_t __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__next__", 0);
 
-  /* "pybitset/backends/cython/_bitset.pyx":228
+  /* "pybitset/backends/cython/_bitset.pyx":231
  *     def __next__(self):
  *         cdef size_t tmp
  *         if bitset_next_set_bit(self.b._bitset, &self.i):             # <<<<<<<<<<<<<<
  *             tmp = self.i
  *             self.i += 1
  */
   __pyx_t_1 = (bitset_next_set_bit(__pyx_v_self->b->_bitset, (&__pyx_v_self->i)) != 0);
   if (likely(__pyx_t_1)) {
 
-    /* "pybitset/backends/cython/_bitset.pyx":229
+    /* "pybitset/backends/cython/_bitset.pyx":232
  *         cdef size_t tmp
  *         if bitset_next_set_bit(self.b._bitset, &self.i):
  *             tmp = self.i             # <<<<<<<<<<<<<<
  *             self.i += 1
  *             return tmp
  */
     __pyx_t_2 = __pyx_v_self->i;
     __pyx_v_tmp = __pyx_t_2;
 
-    /* "pybitset/backends/cython/_bitset.pyx":230
+    /* "pybitset/backends/cython/_bitset.pyx":233
  *         if bitset_next_set_bit(self.b._bitset, &self.i):
  *             tmp = self.i
  *             self.i += 1             # <<<<<<<<<<<<<<
  *             return tmp
  *         else:
  */
     __pyx_v_self->i = (__pyx_v_self->i + 1);
 
-    /* "pybitset/backends/cython/_bitset.pyx":231
+    /* "pybitset/backends/cython/_bitset.pyx":234
  *             tmp = self.i
  *             self.i += 1
  *             return tmp             # <<<<<<<<<<<<<<
  *         else:
  *             raise StopIteration
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = __Pyx_PyInt_FromSize_t(__pyx_v_tmp); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 231, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_FromSize_t(__pyx_v_tmp); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 234, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "pybitset/backends/cython/_bitset.pyx":228
+    /* "pybitset/backends/cython/_bitset.pyx":231
  *     def __next__(self):
  *         cdef size_t tmp
  *         if bitset_next_set_bit(self.b._bitset, &self.i):             # <<<<<<<<<<<<<<
  *             tmp = self.i
  *             self.i += 1
  */
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":233
+  /* "pybitset/backends/cython/_bitset.pyx":236
  *             return tmp
  *         else:
  *             raise StopIteration             # <<<<<<<<<<<<<<
  */
   /*else*/ {
     __Pyx_Raise(__pyx_builtin_StopIteration, 0, 0, 0);
-    __PYX_ERR(0, 233, __pyx_L1_error)
+    __PYX_ERR(0, 236, __pyx_L1_error)
   }
 
-  /* "pybitset/backends/cython/_bitset.pyx":226
+  /* "pybitset/backends/cython/_bitset.pyx":229
  *         return self
  * 
  *     def __next__(self):             # <<<<<<<<<<<<<<
  *         cdef size_t tmp
  *         if bitset_next_set_bit(self.b._bitset, &self.i):
  */
 
@@ -6484,15 +6544,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_8pybitset_8backends_6cython_7_bitset_BitSetIter *__pyx_freelist_8pybitset_8backends_6cython_7_bitset_BitSetIter[8];
 static int __pyx_freecount_8pybitset_8backends_6cython_7_bitset_BitSetIter = 0;
 
@@ -6598,15 +6658,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -6658,14 +6718,15 @@
   {&__pyx_n_s_StopIteration, __pyx_k_StopIteration, sizeof(__pyx_k_StopIteration), 0, 0, 1, 1},
   {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
   {&__pyx_n_s_b, __pyx_k_b, sizeof(__pyx_k_b), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_flag, __pyx_k_flag, sizeof(__pyx_k_flag), 0, 0, 1, 1},
   {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
   {&__pyx_n_s_i, __pyx_k_i, sizeof(__pyx_k_i), 0, 0, 1, 1},
+  {&__pyx_n_s_init, __pyx_k_init, sizeof(__pyx_k_init), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_n_s_newarraysize, __pyx_k_newarraysize, sizeof(__pyx_k_newarraysize), 0, 0, 1, 1},
   {&__pyx_kp_s_no_default___reduce___due_to_non, __pyx_k_no_default___reduce___due_to_non, sizeof(__pyx_k_no_default___reduce___due_to_non), 0, 0, 1, 0},
   {&__pyx_n_s_padwithzeroes, __pyx_k_padwithzeroes, sizeof(__pyx_k_padwithzeroes), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_vtable, __pyx_k_pyx_vtable, sizeof(__pyx_k_pyx_vtable), 0, 0, 1, 1},
   {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
@@ -6674,17 +6735,17 @@
   {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
   {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
   {&__pyx_n_s_size, __pyx_k_size, sizeof(__pyx_k_size), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 33, __pyx_L1_error)
+  __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 34, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
-  __pyx_builtin_StopIteration = __Pyx_GetBuiltinName(__pyx_n_s_StopIteration); if (!__pyx_builtin_StopIteration) __PYX_ERR(0, 233, __pyx_L1_error)
+  __pyx_builtin_StopIteration = __Pyx_GetBuiltinName(__pyx_n_s_StopIteration); if (!__pyx_builtin_StopIteration) __PYX_ERR(0, 236, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
@@ -6819,22 +6880,22 @@
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_8pybitset_8backends_6cython_7_bitset_BitSet.tp_dictoffset && __pyx_type_8pybitset_8backends_6cython_7_bitset_BitSet.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_8pybitset_8backends_6cython_7_bitset_BitSet.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   if (__Pyx_SetVtable(__pyx_type_8pybitset_8backends_6cython_7_bitset_BitSet.tp_dict, __pyx_vtabptr_8pybitset_8backends_6cython_7_bitset_BitSet) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
   if (PyObject_SetAttr(__pyx_m, __pyx_n_s_BitSet, (PyObject *)&__pyx_type_8pybitset_8backends_6cython_7_bitset_BitSet) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
   if (__Pyx_setup_reduce((PyObject*)&__pyx_type_8pybitset_8backends_6cython_7_bitset_BitSet) < 0) __PYX_ERR(0, 25, __pyx_L1_error)
   __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSet = &__pyx_type_8pybitset_8backends_6cython_7_bitset_BitSet;
-  if (PyType_Ready(&__pyx_type_8pybitset_8backends_6cython_7_bitset_BitSetIter) < 0) __PYX_ERR(0, 214, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_8pybitset_8backends_6cython_7_bitset_BitSetIter) < 0) __PYX_ERR(0, 217, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_8pybitset_8backends_6cython_7_bitset_BitSetIter.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_8pybitset_8backends_6cython_7_bitset_BitSetIter.tp_dictoffset && __pyx_type_8pybitset_8backends_6cython_7_bitset_BitSetIter.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_8pybitset_8backends_6cython_7_bitset_BitSetIter.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_8pybitset_8backends_6cython_7_bitset_BitSetIter) < 0) __PYX_ERR(0, 214, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_8pybitset_8backends_6cython_7_bitset_BitSetIter) < 0) __PYX_ERR(0, 217, __pyx_L1_error)
   __pyx_ptype_8pybitset_8backends_6cython_7_bitset_BitSetIter = &__pyx_type_8pybitset_8backends_6cython_7_bitset_BitSetIter;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
@@ -8322,15 +8383,15 @@
                         } else if (8 * sizeof(size_t) >= 4 * PyLong_SHIFT) {
                             return (size_t) (((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -8556,15 +8617,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -8752,15 +8813,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `pybitset-0.0.1.dev1/pybitset/backends/cython/_bitset.pyx` & `pybitset-0.0.1.dev2/pybitset/backends/cython/_bitset.pyx`

 * *Files 18% similar despite different names*

```diff
@@ -1,233 +1,236 @@
-# cython: language_level=3
-# cython: cdivision=True
-cimport cython
-
-from pybitset.backends.cython.bitset cimport (
-    bitset_clear, bitset_contains_all, bitset_copy, bitset_count,
-    bitset_create, bitset_create_with_capacity, bitset_difference_count,
-    bitset_fill, bitset_for_each, bitset_free, bitset_get, bitset_grow,
-    bitset_inplace_difference, bitset_inplace_intersection,
-    bitset_inplace_symmetric_difference, bitset_inplace_union,
-    bitset_intersection_count, bitset_iterator, bitset_maximum, bitset_minimum,
-    bitset_next_set_bit, bitset_next_set_bits, bitset_print, bitset_resize,
-    bitset_set, bitset_set_to_value, bitset_shift_left, bitset_shift_right,
-    bitset_size_in_bits, bitset_size_in_bytes, bitset_size_in_words,
-    bitset_symmetric_difference_count, bitset_t, bitset_trim,
-    bitset_union_count, bitsets_disjoint, bitsets_intersect)
-
-
-cdef bint bitset_iterator_func(size_t value, void *param) with gil:
-    return (<object>param)(value)
-
-@cython.freelist(8)
-@cython.final
-@cython.no_gc
-cdef class BitSet:
-    cdef bitset_t * _bitset
-    def __cinit__(self, size_t size=0):
-        if size == 0:
-            self._bitset = bitset_create()
-        else:
-            self._bitset = bitset_create_with_capacity(size)
-        if not self._bitset:
-            raise MemoryError
-
-    def __dealloc__(self):
-        bitset_free(self._bitset)
-        self._bitset = NULL
-
-    @staticmethod
-    cdef inline BitSet from_ptr(bitset_t * ptr):
-        cdef BitSet self = BitSet.__new__(BitSet)
-        self._bitset = ptr
-        return self
-
-    cpdef inline clear(self):
-        with nogil:
-            bitset_clear(self._bitset)
-
-    cpdef inline fill(self):
-        with nogil:
-            bitset_fill(self._bitset)
-
-    cpdef inline BitSet copy(self):
-        cdef bitset_t *ret
-        with nogil:
-            ret = bitset_copy(self._bitset)
-        return BitSet.from_ptr(ret)
-
-    cpdef inline bint resize(self, size_t newarraysize, bint padwithzeroes):
-        cdef bint ret
-        with nogil:
-            ret = bitset_resize(self._bitset,  newarraysize, padwithzeroes)
-        return ret
-
-    cpdef inline size_t size_in_bytes(self):
-        cdef size_t ret
-        with nogil:
-            ret = bitset_size_in_bytes(self._bitset)
-        return ret
-
-    cpdef inline size_t size_in_bits(self):
-        cdef size_t ret
-        with nogil:
-            ret = bitset_size_in_bits(self._bitset)
-        return ret
-
-    cpdef inline size_t size_in_words(self):
-        cdef size_t ret
-        with nogil:
-            ret = bitset_size_in_words(self._bitset)
-        return ret
-
-    cpdef inline bint grow(self, size_t newarraysize):
-        cdef bint ret
-        with nogil:
-            ret = bitset_grow(self._bitset, newarraysize)
-        return ret
-
-    cpdef inline bint trim(self):
-        cdef bint ret
-        with nogil:
-            ret = bitset_trim(self._bitset)
-        return ret
-
-    cpdef inline shift_left(self, size_t s):
-        with nogil:
-            bitset_shift_left(self._bitset, s)
-
-    cpdef inline shift_right(self, size_t s):
-        with nogil:
-            bitset_shift_right(self._bitset, s)
-
-    cpdef inline set(self,  size_t i):
-        with nogil:
-            bitset_set(self._bitset, i)
-
-    cpdef inline set_to_value(self, size_t i, bint flag):
-        with nogil:
-            bitset_set_to_value(self._bitset, i, flag)
-
-    cpdef inline bint get(self, size_t i):
-        cdef bint ret
-        with nogil:
-            ret = bitset_get(self._bitset, i)
-        return ret
-
-    cpdef inline size_t count(self):
-        cdef size_t ret
-        with nogil:
-            ret = bitset_count(self._bitset)
-        return ret
-
-    cpdef inline size_t minimum(self):
-        cdef size_t ret
-        with nogil:
-            ret = bitset_minimum(self._bitset)
-        return ret
-
-    cpdef inline size_t maximum(self):
-        cdef size_t ret
-        with nogil:
-            ret = bitset_maximum(self._bitset)
-        return ret
-
-    cpdef inline bint inplace_union(self, BitSet b2):
-        cdef bint ret
-        with nogil:
-            ret = bitset_inplace_union(self._bitset, b2._bitset)
-        return ret
-
-    cpdef inline size_t union_count(self, BitSet b2):
-        cdef size_t ret
-        with nogil:
-            ret = bitset_union_count(self._bitset, b2._bitset)
-        return ret
-
-    cpdef inline inplace_intersection(self, BitSet b2):
-        with nogil:
-            bitset_inplace_intersection(self._bitset, b2._bitset)
-
-    cpdef inline size_t intersection_count(self, BitSet b2):
-        cdef size_t ret
-        with nogil:
-            ret = bitset_intersection_count(self._bitset, b2._bitset)
-        return ret
-
-    cpdef inline bint disjoint(self, BitSet b2):
-        cdef bint ret
-        with nogil:
-            ret = bitsets_disjoint(self._bitset, b2._bitset)
-        return ret
-
-    cpdef inline bint intersect(self, BitSet b2):
-        cdef bint ret
-        with nogil:
-            ret = bitsets_intersect(self._bitset, b2._bitset)
-        return ret
-
-    cpdef inline bint contains_all(self, BitSet b2):
-        cdef bint ret
-        with nogil:
-            ret = bitset_contains_all(self._bitset, b2._bitset)
-        return ret
-
-    cpdef inline inplace_difference(self, BitSet b2):
-        with nogil:
-            bitset_inplace_difference(self._bitset, b2._bitset)
-
-    cpdef inline size_t difference_count(self, BitSet b2):
-        cdef size_t ret
-        with nogil:
-            ret = bitset_difference_count(self._bitset, b2._bitset)
-        return ret
-
-    cpdef inline bint inplace_symmetric_difference(self, BitSet b2):
-        cdef bint ret
-        with nogil:
-            ret = bitset_inplace_symmetric_difference(self._bitset, b2._bitset)
-        return ret
-
-    cpdef inline size_t symmetric_difference_count(self, BitSet b2):
-        cdef size_t ret
-        with nogil:
-            ret = bitset_symmetric_difference_count(self._bitset,  b2._bitset)
-        return ret
-
-    def __iter__(self):
-        return BitSetIter(self)
-
-    cpdef inline bint for_each(self, object func):
-        cdef bint ret
-        with nogil:
-            ret = bitset_for_each(self._bitset, bitset_iterator_func, <void*>func)
-        return ret
-
-    cpdef inline print(self):
-        with nogil:
-            bitset_print(self._bitset)
-
-@cython.internal
-@cython.freelist(8)
-@cython.final
-@cython.no_gc
-cdef class BitSetIter:
-    cdef:
-        BitSet b
-        size_t i
-
-    def __cinit__(self, BitSet b):
-        self.b = b
-        self.i = 0
-
-    def __iter__(self):
-        return self
-
-    def __next__(self):
-        cdef size_t tmp
-        if bitset_next_set_bit(self.b._bitset, &self.i):
-            tmp = self.i
-            self.i += 1
-            return tmp
-        else:
-            raise StopIteration
+# cython: language_level=3
+# cython: cdivision=True
+cimport cython
+
+from pybitset.backends.cython.bitset cimport (
+    bitset_clear, bitset_contains_all, bitset_copy, bitset_count,
+    bitset_create, bitset_create_with_capacity, bitset_difference_count,
+    bitset_fill, bitset_for_each, bitset_free, bitset_get, bitset_grow,
+    bitset_inplace_difference, bitset_inplace_intersection,
+    bitset_inplace_symmetric_difference, bitset_inplace_union,
+    bitset_intersection_count, bitset_iterator, bitset_maximum, bitset_minimum,
+    bitset_next_set_bit, bitset_next_set_bits, bitset_print, bitset_resize,
+    bitset_set, bitset_set_to_value, bitset_shift_left, bitset_shift_right,
+    bitset_size_in_bits, bitset_size_in_bytes, bitset_size_in_words,
+    bitset_symmetric_difference_count, bitset_t, bitset_trim,
+    bitset_union_count, bitsets_disjoint, bitsets_intersect)
+
+
+cdef bint bitset_iterator_func(size_t value, void *param) with gil:
+    return (<object>param)(value)
+
+@cython.freelist(8)
+@cython.final
+@cython.no_gc
+cdef class BitSet:
+    cdef bitset_t * _bitset
+    def __cinit__(self, size_t size=0, bint _init = True):
+        if _init:
+            if size == 0:
+                self._bitset = bitset_create()
+            else:
+                self._bitset = bitset_create_with_capacity(size)
+            if not self._bitset:
+                raise MemoryError
+        else:
+            self._bitset = NULL
+
+    def __dealloc__(self):
+        bitset_free(self._bitset)
+        self._bitset = NULL
+
+    @staticmethod
+    cdef inline BitSet from_ptr(bitset_t * ptr):
+        cdef BitSet self = BitSet(_init=False)
+        self._bitset = ptr
+        return self
+
+    cpdef inline clear(self):
+        with nogil:
+            bitset_clear(self._bitset)
+
+    cpdef inline fill(self):
+        with nogil:
+            bitset_fill(self._bitset)
+
+    cpdef inline BitSet copy(self):
+        cdef bitset_t *ret
+        with nogil:
+            ret = bitset_copy(self._bitset)
+        return BitSet.from_ptr(ret)
+
+    cpdef inline bint resize(self, size_t newarraysize, bint padwithzeroes):
+        cdef bint ret
+        with nogil:
+            ret = bitset_resize(self._bitset,  newarraysize, padwithzeroes)
+        return ret
+
+    cpdef inline size_t size_in_bytes(self):
+        cdef size_t ret
+        with nogil:
+            ret = bitset_size_in_bytes(self._bitset)
+        return ret
+
+    cpdef inline size_t size_in_bits(self):
+        cdef size_t ret
+        with nogil:
+            ret = bitset_size_in_bits(self._bitset)
+        return ret
+
+    cpdef inline size_t size_in_words(self):
+        cdef size_t ret
+        with nogil:
+            ret = bitset_size_in_words(self._bitset)
+        return ret
+
+    cpdef inline bint grow(self, size_t newarraysize):
+        cdef bint ret
+        with nogil:
+            ret = bitset_grow(self._bitset, newarraysize)
+        return ret
+
+    cpdef inline bint trim(self):
+        cdef bint ret
+        with nogil:
+            ret = bitset_trim(self._bitset)
+        return ret
+
+    cpdef inline shift_left(self, size_t s):
+        with nogil:
+            bitset_shift_left(self._bitset, s)
+
+    cpdef inline shift_right(self, size_t s):
+        with nogil:
+            bitset_shift_right(self._bitset, s)
+
+    cpdef inline set(self,  size_t i):
+        with nogil:
+            bitset_set(self._bitset, i)
+
+    cpdef inline set_to_value(self, size_t i, bint flag):
+        with nogil:
+            bitset_set_to_value(self._bitset, i, flag)
+
+    cpdef inline bint get(self, size_t i):
+        cdef bint ret
+        with nogil:
+            ret = bitset_get(self._bitset, i)
+        return ret
+
+    cpdef inline size_t count(self):
+        cdef size_t ret
+        with nogil:
+            ret = bitset_count(self._bitset)
+        return ret
+
+    cpdef inline size_t minimum(self):
+        cdef size_t ret
+        with nogil:
+            ret = bitset_minimum(self._bitset)
+        return ret
+
+    cpdef inline size_t maximum(self):
+        cdef size_t ret
+        with nogil:
+            ret = bitset_maximum(self._bitset)
+        return ret
+
+    cpdef inline bint inplace_union(self, BitSet b2):
+        cdef bint ret
+        with nogil:
+            ret = bitset_inplace_union(self._bitset, b2._bitset)
+        return ret
+
+    cpdef inline size_t union_count(self, BitSet b2):
+        cdef size_t ret
+        with nogil:
+            ret = bitset_union_count(self._bitset, b2._bitset)
+        return ret
+
+    cpdef inline inplace_intersection(self, BitSet b2):
+        with nogil:
+            bitset_inplace_intersection(self._bitset, b2._bitset)
+
+    cpdef inline size_t intersection_count(self, BitSet b2):
+        cdef size_t ret
+        with nogil:
+            ret = bitset_intersection_count(self._bitset, b2._bitset)
+        return ret
+
+    cpdef inline bint disjoint(self, BitSet b2):
+        cdef bint ret
+        with nogil:
+            ret = bitsets_disjoint(self._bitset, b2._bitset)
+        return ret
+
+    cpdef inline bint intersect(self, BitSet b2):
+        cdef bint ret
+        with nogil:
+            ret = bitsets_intersect(self._bitset, b2._bitset)
+        return ret
+
+    cpdef inline bint contains_all(self, BitSet b2):
+        cdef bint ret
+        with nogil:
+            ret = bitset_contains_all(self._bitset, b2._bitset)
+        return ret
+
+    cpdef inline inplace_difference(self, BitSet b2):
+        with nogil:
+            bitset_inplace_difference(self._bitset, b2._bitset)
+
+    cpdef inline size_t difference_count(self, BitSet b2):
+        cdef size_t ret
+        with nogil:
+            ret = bitset_difference_count(self._bitset, b2._bitset)
+        return ret
+
+    cpdef inline bint inplace_symmetric_difference(self, BitSet b2):
+        cdef bint ret
+        with nogil:
+            ret = bitset_inplace_symmetric_difference(self._bitset, b2._bitset)
+        return ret
+
+    cpdef inline size_t symmetric_difference_count(self, BitSet b2):
+        cdef size_t ret
+        with nogil:
+            ret = bitset_symmetric_difference_count(self._bitset,  b2._bitset)
+        return ret
+
+    def __iter__(self):
+        return BitSetIter(self)
+
+    cpdef inline bint for_each(self, object func):
+        cdef bint ret
+        with nogil:
+            ret = bitset_for_each(self._bitset, bitset_iterator_func, <void*>func)
+        return ret
+
+    cpdef inline print(self):
+        with nogil:
+            bitset_print(self._bitset)
+
+@cython.internal
+@cython.freelist(8)
+@cython.final
+@cython.no_gc
+cdef class BitSetIter:
+    cdef:
+        BitSet b
+        size_t i
+
+    def __cinit__(self, BitSet b):
+        self.b = b
+        self.i = 0
+
+    def __iter__(self):
+        return self
+
+    def __next__(self):
+        cdef size_t tmp
+        if bitset_next_set_bit(self.b._bitset, &self.i):
+            tmp = self.i
+            self.i += 1
+            return tmp
+        else:
+            raise StopIteration
```

### Comparing `pybitset-0.0.1.dev1/pybitset/backends/cython/bitset.pxd` & `pybitset-0.0.1.dev2/pybitset/backends/cython/bitset.pxd`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-# cython: language_level=3
-# cython: cdivision=True
-
-
-cdef extern from "bitset.h" nogil:
-    ctypedef struct bitset_t
-
-    bitset_t* bitset_create()
-    bitset_t *bitset_create_with_capacity( size_t size )
-    void bitset_free(bitset_t *bitset)
-    void bitset_clear(bitset_t *bitset)
-    void bitset_fill(bitset_t *bitset)
-    bitset_t * bitset_copy(const bitset_t *bitset)
-    bint bitset_resize(bitset_t *bitset, size_t newarraysize, bint padwithzeroes)
-    size_t bitset_size_in_bytes(const bitset_t *bitset)
-    size_t bitset_size_in_bits(const bitset_t *bitset)
-    size_t bitset_size_in_words(const bitset_t *bitset)
-    bint bitset_grow(bitset_t *bitset, size_t newarraysize)
-    bint bitset_trim(bitset_t *bitset)
-    void bitset_shift_left(bitset_t *bitset, size_t s)
-    void bitset_shift_right(bitset_t *bitset, size_t s)
-    void bitset_set(bitset_t *bitset, size_t i)
-    void bitset_set_to_value(bitset_t *bitset, size_t i, bint flag)
-    bint bitset_get(const bitset_t *bitset, size_t i)
-    size_t bitset_count(const bitset_t *bitset)
-    size_t bitset_minimum(const bitset_t *bitset)
-    size_t bitset_maximum(const bitset_t *bitset)
-    bint bitset_inplace_union(bitset_t *   b1, const bitset_t *  b2 )
-    size_t bitset_union_count(const bitset_t *  b1, const bitset_t *  b2 )
-    void bitset_inplace_intersection(bitset_t *  b1, const bitset_t * b2)
-    size_t bitset_intersection_count(const bitset_t * b1, const bitset_t * b2)
-    bint bitsets_disjoint(const bitset_t * b1, const bitset_t * b2)
-    bint bitsets_intersect(const bitset_t * b1, const bitset_t * b2)
-    bint bitset_contains_all(const bitset_t * b1, const bitset_t * b2)
-
-# compute the difference in-place (to b1), to generate a new bitset first call bitset_copy */
-    void bitset_inplace_difference(bitset_t * b1, const bitset_t * b2)
-
-# compute the size of the difference */
-    size_t  bitset_difference_count(const bitset_t * b1, const bitset_t * b2)
-
-# compute the symmetric difference in-place (to b1), return true if successful, to generate a new bitset first call bitset_copy */
-    bint bitset_inplace_symmetric_difference(bitset_t * b1, const bitset_t * b2)
-
-# compute the size of the symmetric difference  */
-    size_t  bitset_symmetric_difference_count(const bitset_t * b1, const bitset_t * b2)
-    bint bitset_next_set_bit(const bitset_t *bitset, size_t *i)
-    size_t bitset_next_set_bits(const bitset_t *bitset, size_t *buffer, size_t capacity, size_t * startfrom)
-
-    ctypedef bint(*bitset_iterator)(size_t value, void *param);
-    bint bitset_for_each(const bitset_t *b, bitset_iterator iterator, void *ptr)
-    void bitset_print(const bitset_t *b)
+# cython: language_level=3
+# cython: cdivision=True
+
+
+cdef extern from "bitset.h" nogil:
+    ctypedef struct bitset_t
+
+    bitset_t* bitset_create()
+    bitset_t *bitset_create_with_capacity( size_t size )
+    void bitset_free(bitset_t *bitset)
+    void bitset_clear(bitset_t *bitset)
+    void bitset_fill(bitset_t *bitset)
+    bitset_t * bitset_copy(const bitset_t *bitset)
+    bint bitset_resize(bitset_t *bitset, size_t newarraysize, bint padwithzeroes)
+    size_t bitset_size_in_bytes(const bitset_t *bitset)
+    size_t bitset_size_in_bits(const bitset_t *bitset)
+    size_t bitset_size_in_words(const bitset_t *bitset)
+    bint bitset_grow(bitset_t *bitset, size_t newarraysize)
+    bint bitset_trim(bitset_t *bitset)
+    void bitset_shift_left(bitset_t *bitset, size_t s)
+    void bitset_shift_right(bitset_t *bitset, size_t s)
+    void bitset_set(bitset_t *bitset, size_t i)
+    void bitset_set_to_value(bitset_t *bitset, size_t i, bint flag)
+    bint bitset_get(const bitset_t *bitset, size_t i)
+    size_t bitset_count(const bitset_t *bitset)
+    size_t bitset_minimum(const bitset_t *bitset)
+    size_t bitset_maximum(const bitset_t *bitset)
+    bint bitset_inplace_union(bitset_t *   b1, const bitset_t *  b2 )
+    size_t bitset_union_count(const bitset_t *  b1, const bitset_t *  b2 )
+    void bitset_inplace_intersection(bitset_t *  b1, const bitset_t * b2)
+    size_t bitset_intersection_count(const bitset_t * b1, const bitset_t * b2)
+    bint bitsets_disjoint(const bitset_t * b1, const bitset_t * b2)
+    bint bitsets_intersect(const bitset_t * b1, const bitset_t * b2)
+    bint bitset_contains_all(const bitset_t * b1, const bitset_t * b2)
+
+# compute the difference in-place (to b1), to generate a new bitset first call bitset_copy */
+    void bitset_inplace_difference(bitset_t * b1, const bitset_t * b2)
+
+# compute the size of the difference */
+    size_t  bitset_difference_count(const bitset_t * b1, const bitset_t * b2)
+
+# compute the symmetric difference in-place (to b1), return true if successful, to generate a new bitset first call bitset_copy */
+    bint bitset_inplace_symmetric_difference(bitset_t * b1, const bitset_t * b2)
+
+# compute the size of the symmetric difference  */
+    size_t  bitset_symmetric_difference_count(const bitset_t * b1, const bitset_t * b2)
+    bint bitset_next_set_bit(const bitset_t *bitset, size_t *i)
+    size_t bitset_next_set_bits(const bitset_t *bitset, size_t *buffer, size_t capacity, size_t * startfrom)
+
+    ctypedef bint(*bitset_iterator)(size_t value, void *param);
+    bint bitset_for_each(const bitset_t *b, bitset_iterator iterator, void *ptr)
+    void bitset_print(const bitset_t *b)
```

### Comparing `pybitset-0.0.1.dev1/pybitset.egg-info/PKG-INFO` & `pybitset-0.0.1.dev2/pybitset.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-Metadata-Version: 2.1
-Name: pybitset
-Version: 0.0.1.dev1
-Summary: python binding for cbitset
-Home-page: https://github.com/synodriver/pybitset
-Author: synodriver
-Author-email: diguohuangjiajinweijun@gmail.com
-License: BSD
-Keywords: bitset
-Classifier: Development Status :: 3 - Alpha
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Programming Language :: C
-Classifier: Programming Language :: Cython
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
-<h1 align="center"><i>✨ pybitset ✨ </i></h1>
-
-<h3 align="center">The python binding for <a href="https://github.com/lemire/cbitset">cbitset</a></h3>
-
-[![pypi](https://img.shields.io/pypi/v/pybitset.svg)](https://pypi.org/project/bzip3/)
-![python](https://img.shields.io/pypi/pyversions/pybitset)
-![implementation](https://img.shields.io/pypi/implementation/pybitset)
-![wheel](https://img.shields.io/pypi/wheel/pybitset)
-![license](https://img.shields.io/github/license/synodriver/pybitset.svg)
-![action](https://img.shields.io/github/workflow/status/synodriver/pybitset/build%20wheel)
-
-### install
-```bash
-pip install pybitset
-```
-
-
-### Usage
-```python
-from pybitset import BitSet
-
-b= BitSet()
-for i in range(1000):
-    b.set(3*i)
-
-for v in b:
-    print(v)
-```
-- use ```BITSET_USE_CFFI``` env var to specify a backend
-
-### Public functions
-```python
-class BitSet:
-    def __init__(self) -> None: ...
-    def __del__(self) -> None: ...
-    @staticmethod
-    def from_ptr(ptr) -> BitSet: ...
-    def clear(self) -> None: ...
-    def fill(self) -> None: ...
-    def copy(self) -> BitSet: ...
-    def resize(self, newarraysize: int, padwithzeroes: bool) -> bool: ...
-    def size_in_bytes(self) -> int: ...
-    def size_in_bits(self) -> int: ...
-    def size_in_words(self) -> int: ...
-    def grow(self, newarraysize: int) -> bool: ...
-    def trim(self) -> bool: ...
-    def shift_left(self, s: int) -> None: ...
-    def shift_right(self, s: int) -> None: ...
-    def set(self, i: int) -> None: ...
-    def set_to_value(self, i: int, flag: bool) -> None: ...
-    def get(self, i: int) -> bool: ...
-    def count(self) -> int: ...
-    def minimum(self) -> int: ...
-    def maximum(self) -> int: ...
-    def inplace_union(self, b2: BitSet) -> bool: ...
-    def union_count(self, b2: BitSet) -> int: ...
-    def inplace_intersection(self, b2: BitSet): ...
-    def intersection_count(self, b2: BitSet) -> int: ...
-    def disjoint(self, b2: BitSet) -> bool: ...
-    def intersect(self, b2: BitSet) -> bool: ...
-    def contains_all(self, b2: BitSet) -> bool: ...
-    def inplace_difference(self, b2: BitSet) -> None: ...
-    def difference_count(self, b2: BitSet) -> int: ...
-    def inplace_symmetric_difference(self, b2: BitSet) -> bool: ...
-    def symmetric_difference_count(self, b2: BitSet) -> int: ...
-    def __iter__(self): ...
-    def for_each(self, func) -> bool: ...
-    def print(self) -> None: ...
-
-```
+Metadata-Version: 2.1
+Name: pybitset
+Version: 0.0.1.dev2
+Summary: python binding for cbitset
+Home-page: https://github.com/synodriver/pybitset
+Author: synodriver
+Author-email: diguohuangjiajinweijun@gmail.com
+License: BSD
+Keywords: bitset
+Classifier: Development Status :: 3 - Alpha
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: Programming Language :: C
+Classifier: Programming Language :: Cython
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
+<h1 align="center"><i>✨ pybitset ✨ </i></h1>
+
+<h3 align="center">The python binding for <a href="https://github.com/lemire/cbitset">cbitset</a></h3>
+
+[![pypi](https://img.shields.io/pypi/v/pybitset.svg)](https://pypi.org/project/pybitset/)
+![python](https://img.shields.io/pypi/pyversions/pybitset)
+![implementation](https://img.shields.io/pypi/implementation/pybitset)
+![wheel](https://img.shields.io/pypi/wheel/pybitset)
+![license](https://img.shields.io/github/license/synodriver/pybitset.svg)
+![action](https://img.shields.io/github/workflow/status/synodriver/pybitset/build%20wheel)
+
+### install
+```bash
+pip install pybitset
+```
+
+
+### Usage
+```python
+from pybitset import BitSet
+
+b= BitSet()
+for i in range(1000):
+    b.set(3*i)
+
+for v in b:
+    print(v)
+```
+- use ```BITSET_USE_CFFI``` env var to specify a backend
+
+### Public functions
+```python
+class BitSet:
+    def __init__(self) -> None: ...
+    def __del__(self) -> None: ...
+    @staticmethod
+    def from_ptr(ptr) -> BitSet: ...
+    def clear(self) -> None: ...
+    def fill(self) -> None: ...
+    def copy(self) -> BitSet: ...
+    def resize(self, newarraysize: int, padwithzeroes: bool) -> bool: ...
+    def size_in_bytes(self) -> int: ...
+    def size_in_bits(self) -> int: ...
+    def size_in_words(self) -> int: ...
+    def grow(self, newarraysize: int) -> bool: ...
+    def trim(self) -> bool: ...
+    def shift_left(self, s: int) -> None: ...
+    def shift_right(self, s: int) -> None: ...
+    def set(self, i: int) -> None: ...
+    def set_to_value(self, i: int, flag: bool) -> None: ...
+    def get(self, i: int) -> bool: ...
+    def count(self) -> int: ...
+    def minimum(self) -> int: ...
+    def maximum(self) -> int: ...
+    def inplace_union(self, b2: BitSet) -> bool: ...
+    def union_count(self, b2: BitSet) -> int: ...
+    def inplace_intersection(self, b2: BitSet): ...
+    def intersection_count(self, b2: BitSet) -> int: ...
+    def disjoint(self, b2: BitSet) -> bool: ...
+    def intersect(self, b2: BitSet) -> bool: ...
+    def contains_all(self, b2: BitSet) -> bool: ...
+    def inplace_difference(self, b2: BitSet) -> None: ...
+    def difference_count(self, b2: BitSet) -> int: ...
+    def inplace_symmetric_difference(self, b2: BitSet) -> bool: ...
+    def symmetric_difference_count(self, b2: BitSet) -> int: ...
+    def __iter__(self): ...
+    def for_each(self, func) -> bool: ...
+    def print(self) -> None: ...
+
+```
```

### Comparing `pybitset-0.0.1.dev1/pybitset.egg-info/SOURCES.txt` & `pybitset-0.0.1.dev2/pybitset.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -29,22 +29,14 @@
 pybitset/__init__.py
 pybitset.egg-info/PKG-INFO
 pybitset.egg-info/SOURCES.txt
 pybitset.egg-info/dependency_links.txt
 pybitset.egg-info/not-zip-safe
 pybitset.egg-info/requires.txt
 pybitset.egg-info/top_level.txt
-pybitset/backends/cython/_bitset.c
-pybitset/__pycache__/__init__.cpython-310.pyc
 pybitset/backends/__init__.py
-pybitset/backends/__pycache__/__init__.cpython-310.pyc
 pybitset/backends/cffi/__init__.py
-pybitset/backends/cffi/_bitset.pyd
 pybitset/backends/cffi/build.py
-pybitset/backends/cffi/__pycache__/__init__.cpython-310.pyc
-pybitset/backends/cffi/__pycache__/build.cpython-310.pyc
 pybitset/backends/cython/__init__.py
 pybitset/backends/cython/_bitset.c
-pybitset/backends/cython/_bitset.cp310-win_amd64.pyd
 pybitset/backends/cython/_bitset.pyx
-pybitset/backends/cython/bitset.pxd
-pybitset/backends/cython/__pycache__/__init__.cpython-310.pyc
+pybitset/backends/cython/bitset.pxd
```

### Comparing `pybitset-0.0.1.dev1/setup.py` & `pybitset-0.0.1.dev2/setup.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,138 +1,138 @@
-"""
-Copyright (c) 2008-2023 synodriver <diguohuangjiajinweijun@gmail.com>
-"""
-import glob
-import os
-import re
-import sys
-from collections import defaultdict
-
-try:
-    from Cython.Build import cythonize
-except ImportError:
-    Cython = None
-from setuptools import Extension, find_packages, setup
-from setuptools.command.build_ext import build_ext
-
-BUILD_ARGS = defaultdict(lambda: ["-O3", "-g0"])
-
-for compiler, args in [
-    ("msvc", ["/EHsc", "/DHUNSPELL_STATIC", "/Oi", "/O2", "/Ot"]),
-    ("gcc", ["-O3", "-g0"]),
-]:
-    BUILD_ARGS[compiler] = args
-
-
-class build_ext_compiler_check(build_ext):
-    def build_extensions(self):
-        compiler = self.compiler.compiler_type
-        args = BUILD_ARGS[compiler]
-        for ext in self.extensions:
-            ext.extra_compile_args.extend(args)
-            if self.compiler.compiler_type == "msvc":
-                ext.define_macros.extend([("restrict", "__restrict")])
-        super().build_extensions()
-
-
-c_sources = ["pybitset/backends/cython/_bitset.pyx"] + glob.glob("./cbitset/src/*.c")
-c_sources = list(filter(lambda x: "main" not in x, c_sources))
-extensions = [
-    Extension(
-        "pybitset.backends.cython._bitset",
-        c_sources,
-        include_dirs=["./cbitset/include"],
-    ),
-]
-cffi_modules = ["pybitset/backends/cffi/build.py:ffibuilder"]
-
-
-def get_dis():
-    with open("README.markdown", "r", encoding="utf-8") as f:
-        return f.read()
-
-
-def get_version() -> str:
-    path = os.path.join(
-        os.path.abspath(os.path.dirname(__file__)), "pybitset", "__init__.py"
-    )
-    with open(path, "r", encoding="utf-8") as f:
-        data = f.read()
-    result = re.findall(r"(?<=__version__ = \")\S+(?=\")", data)
-    return result[0]
-
-
-packages = find_packages(exclude=("test", "tests.*", "test*"))
-
-
-def has_option(name: str) -> bool:
-    if name in sys.argv[1:]:
-        sys.argv.remove(name)
-        return True
-    return False
-
-
-setup_requires = []
-install_requires = []
-setup_kw = {}
-if has_option("--use-cython"):
-    print("building cython")
-    setup_requires.append("cython")
-    setup_kw["ext_modules"] = cythonize(
-        extensions,
-        compiler_directives={
-            "cdivision": True,
-            "embedsignature": True,
-            "boundscheck": False,
-            "wraparound": False,
-        },
-    )
-if has_option("--use-cffi"):
-    print("building cffi")
-    setup_requires.append("cffi>=1.0.0")
-    install_requires.append("cffi>=1.0.0")
-    setup_kw["cffi_modules"] = cffi_modules
-
-
-def main():
-    version: str = get_version()
-
-    dis = get_dis()
-    setup(
-        name="pybitset",
-        version=version,
-        url="https://github.com/synodriver/pybitset",
-        packages=packages,
-        keywords=["bitset"],
-        description="python binding for cbitset",
-        long_description_content_type="text/markdown",
-        long_description=dis,
-        author="synodriver",
-        author_email="diguohuangjiajinweijun@gmail.com",
-        python_requires=">=3.7",
-        setup_requires=setup_requires,
-        install_requires=install_requires,
-        license="BSD",
-        classifiers=[
-            "Development Status :: 3 - Alpha",
-            "Operating System :: OS Independent",
-            "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
-            "Programming Language :: C",
-            "Programming Language :: Cython",
-            "Programming Language :: Python",
-            "Programming Language :: Python :: 3.7",
-            "Programming Language :: Python :: 3.8",
-            "Programming Language :: Python :: 3.9",
-            "Programming Language :: Python :: 3.10",
-            "Programming Language :: Python :: 3.11",
-            "Programming Language :: Python :: Implementation :: CPython",
-            "Programming Language :: Python :: Implementation :: PyPy",
-        ],
-        include_package_data=True,
-        zip_safe=False,
-        cmdclass={"build_ext": build_ext_compiler_check},
-        **setup_kw
-    )
-
-
-if __name__ == "__main__":
-    main()
+"""
+Copyright (c) 2008-2023 synodriver <diguohuangjiajinweijun@gmail.com>
+"""
+import glob
+import os
+import re
+import sys
+from collections import defaultdict
+
+try:
+    from Cython.Build import cythonize
+except ImportError:
+    Cython = None
+from setuptools import Extension, find_packages, setup
+from setuptools.command.build_ext import build_ext
+
+BUILD_ARGS = defaultdict(lambda: ["-O3", "-g0"])
+
+for compiler, args in [
+    ("msvc", ["/EHsc", "/DHUNSPELL_STATIC", "/Oi", "/O2", "/Ot"]),
+    ("gcc", ["-O3", "-g0"]),
+]:
+    BUILD_ARGS[compiler] = args
+
+
+class build_ext_compiler_check(build_ext):
+    def build_extensions(self):
+        compiler = self.compiler.compiler_type
+        args = BUILD_ARGS[compiler]
+        for ext in self.extensions:
+            ext.extra_compile_args.extend(args)
+            if self.compiler.compiler_type == "msvc":
+                ext.define_macros.extend([("restrict", "__restrict")])
+        super().build_extensions()
+
+
+c_sources = ["pybitset/backends/cython/_bitset.pyx"] + glob.glob("./cbitset/src/*.c")
+c_sources = list(filter(lambda x: "main" not in x, c_sources))
+extensions = [
+    Extension(
+        "pybitset.backends.cython._bitset",
+        c_sources,
+        include_dirs=["./cbitset/include"],
+    ),
+]
+cffi_modules = ["pybitset/backends/cffi/build.py:ffibuilder"]
+
+
+def get_dis():
+    with open("README.markdown", "r", encoding="utf-8") as f:
+        return f.read()
+
+
+def get_version() -> str:
+    path = os.path.join(
+        os.path.abspath(os.path.dirname(__file__)), "pybitset", "__init__.py"
+    )
+    with open(path, "r", encoding="utf-8") as f:
+        data = f.read()
+    result = re.findall(r"(?<=__version__ = \")\S+(?=\")", data)
+    return result[0]
+
+
+packages = find_packages(exclude=("test", "tests.*", "test*"))
+
+
+def has_option(name: str) -> bool:
+    if name in sys.argv[1:]:
+        sys.argv.remove(name)
+        return True
+    return False
+
+
+setup_requires = []
+install_requires = []
+setup_kw = {}
+if has_option("--use-cython"):
+    print("building cython")
+    setup_requires.append("cython")
+    setup_kw["ext_modules"] = cythonize(
+        extensions,
+        compiler_directives={
+            "cdivision": True,
+            "embedsignature": True,
+            "boundscheck": False,
+            "wraparound": False,
+        },
+    )
+if has_option("--use-cffi"):
+    print("building cffi")
+    setup_requires.append("cffi>=1.0.0")
+    install_requires.append("cffi>=1.0.0")
+    setup_kw["cffi_modules"] = cffi_modules
+
+
+def main():
+    version: str = get_version()
+
+    dis = get_dis()
+    setup(
+        name="pybitset",
+        version=version,
+        url="https://github.com/synodriver/pybitset",
+        packages=packages,
+        keywords=["bitset"],
+        description="python binding for cbitset",
+        long_description_content_type="text/markdown",
+        long_description=dis,
+        author="synodriver",
+        author_email="diguohuangjiajinweijun@gmail.com",
+        python_requires=">=3.7",
+        setup_requires=setup_requires,
+        install_requires=install_requires,
+        license="BSD",
+        classifiers=[
+            "Development Status :: 3 - Alpha",
+            "Operating System :: OS Independent",
+            "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
+            "Programming Language :: C",
+            "Programming Language :: Cython",
+            "Programming Language :: Python",
+            "Programming Language :: Python :: 3.7",
+            "Programming Language :: Python :: 3.8",
+            "Programming Language :: Python :: 3.9",
+            "Programming Language :: Python :: 3.10",
+            "Programming Language :: Python :: 3.11",
+            "Programming Language :: Python :: Implementation :: CPython",
+            "Programming Language :: Python :: Implementation :: PyPy",
+        ],
+        include_package_data=True,
+        zip_safe=False,
+        cmdclass={"build_ext": build_ext_compiler_check},
+        **setup_kw
+    )
+
+
+if __name__ == "__main__":
+    main()
```

