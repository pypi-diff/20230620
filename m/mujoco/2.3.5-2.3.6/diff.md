# Comparing `tmp/mujoco-2.3.5.tar.gz` & `tmp/mujoco-2.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mujoco-2.3.5.tar", last modified: Tue Apr 25 14:29:14 2023, max compression
+gzip compressed data, was "mujoco-2.3.6.tar", last modified: Tue Jun 20 17:18:03 2023, max compression
```

## Comparing `mujoco-2.3.5.tar` & `mujoco-2.3.6.tar`

### file list

```diff
@@ -1,100 +1,101 @@
-drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-04-25 14:29:14.160325 mujoco-2.3.5/
--rw-r--r--   0 jenkins    (502) staff       (20)    11358 2023-04-25 14:29:14.000000 mujoco-2.3.5/LICENSE
--rw-r--r--   0 jenkins    (502) staff       (20)    31030 2023-04-25 14:29:13.000000 mujoco-2.3.5/LICENSES_THIRD_PARTY.md
--rw-r--r--   0 jenkins    (502) staff       (20)      179 2023-04-25 14:29:13.000000 mujoco-2.3.5/MANIFEST.in
--rw-r--r--   0 jenkins    (502) staff       (20)    34948 2023-04-25 14:29:14.160187 mujoco-2.3.5/PKG-INFO
--rw-r--r--   0 jenkins    (502) staff       (20)     2987 2023-04-25 14:29:13.000000 mujoco-2.3.5/README.md
-drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-04-25 14:29:14.151831 mujoco-2.3.5/cmake/
--rw-r--r--   0 jenkins    (502) staff       (20)     1740 2023-04-25 14:29:14.000000 mujoco-2.3.5/cmake/CheckAvxSupport.cmake
--rw-r--r--   0 jenkins    (502) staff       (20)     4747 2023-04-25 14:29:14.000000 mujoco-2.3.5/cmake/FindOrFetch.cmake
--rw-r--r--   0 jenkins    (502) staff       (20)     8371 2023-04-25 14:29:14.000000 mujoco-2.3.5/cmake/MujocoDependencies.cmake
--rw-r--r--   0 jenkins    (502) staff       (20)     1242 2023-04-25 14:29:14.000000 mujoco-2.3.5/cmake/MujocoHarden.cmake
--rw-r--r--   0 jenkins    (502) staff       (20)     2302 2023-04-25 14:29:14.000000 mujoco-2.3.5/cmake/MujocoLinkOptions.cmake
--rw-r--r--   0 jenkins    (502) staff       (20)     1568 2023-04-25 14:29:14.000000 mujoco-2.3.5/cmake/MujocoMacOS.cmake
--rw-r--r--   0 jenkins    (502) staff       (20)     3918 2023-04-25 14:29:14.000000 mujoco-2.3.5/cmake/MujocoOptions.cmake
--rw-r--r--   0 jenkins    (502) staff       (20)     2164 2023-04-25 14:29:14.000000 mujoco-2.3.5/cmake/ShellTests.cmake
--rw-r--r--   0 jenkins    (502) staff       (20)     5676 2023-04-25 14:29:14.000000 mujoco-2.3.5/cmake/TargetAddRpath.cmake
-drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-04-25 14:29:14.155315 mujoco-2.3.5/mujoco/
--rw-r--r--   0 jenkins    (502) staff       (20)    13113 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/CMakeLists.txt
--rw-r--r--   0 jenkins    (502) staff       (20)     2446 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/__init__.py
--rw-r--r--   0 jenkins    (502) staff       (20)    46477 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/bindings_test.py
--rw-r--r--   0 jenkins    (502) staff       (20)    13444 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/callbacks.cc
-drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-04-25 14:29:14.156060 mujoco-2.3.5/mujoco/cgl/
--rw-r--r--   0 jenkins    (502) staff       (20)     2271 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/cgl/__init__.py
--rw-r--r--   0 jenkins    (502) staff       (20)     5204 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/cgl/cgl.py
--rw-r--r--   0 jenkins    (502) staff       (20)     2366 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/constants.cc
-drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-04-25 14:29:14.156273 mujoco-2.3.5/mujoco/egl/
--rw-r--r--   0 jenkins    (502) staff       (20)     4764 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/egl/__init__.py
--rw-r--r--   0 jenkins    (502) staff       (20)     2783 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/egl/egl_ext.py
--rw-r--r--   0 jenkins    (502) staff       (20)    30507 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/enum_traits.h
--rw-r--r--   0 jenkins    (502) staff       (20)     4704 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/enums.cc
--rw-r--r--   0 jenkins    (502) staff       (20)      885 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/errors.cc
--rw-r--r--   0 jenkins    (502) staff       (20)     7747 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/errors.h
--rw-r--r--   0 jenkins    (502) staff       (20)   121937 2023-04-25 14:29:14.000000 mujoco-2.3.5/mujoco/function_traits.h
--rw-r--r--   0 jenkins    (502) staff       (20)    46647 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/functions.cc
--rw-r--r--   0 jenkins    (502) staff       (20)     7964 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/functions.h
--rw-r--r--   0 jenkins    (502) staff       (20)     1849 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/gl_context.py
-drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-04-25 14:29:14.156372 mujoco-2.3.5/mujoco/glfw/
--rw-r--r--   0 jenkins    (502) staff       (20)     1403 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/glfw/__init__.py
--rw-r--r--   0 jenkins    (502) staff       (20)    20668 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/indexer_xmacro.h
--rw-r--r--   0 jenkins    (502) staff       (20)    15911 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/indexers.cc
--rw-r--r--   0 jenkins    (502) staff       (20)     7177 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/indexers.h
--rw-r--r--   0 jenkins    (502) staff       (20)     3474 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/mjdata_meta.h
-drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-04-25 14:29:14.157000 mujoco-2.3.5/mujoco/mjpython/
--rw-r--r--   0 jenkins    (502) staff       (20)     1113 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/mjpython/Info.plist
--rw-r--r--   0 jenkins    (502) staff       (20)   432307 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/mjpython/mjpython.icns
--rw-r--r--   0 jenkins    (502) staff       (20)    12145 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/mjpython/mjpython.mm
--rw-r--r--   0 jenkins    (502) staff       (20)     2286 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/mjpython/mjpython.py
-drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-04-25 14:29:14.157104 mujoco-2.3.5/mujoco/osmesa/
--rw-r--r--   0 jenkins    (502) staff       (20)     2556 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/osmesa/__init__.py
--rw-r--r--   0 jenkins    (502) staff       (20)     1962 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/raw.h
--rw-r--r--   0 jenkins    (502) staff       (20)     8709 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/render.cc
--rw-r--r--   0 jenkins    (502) staff       (20)     3822 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/render_test.py
--rw-r--r--   0 jenkins    (502) staff       (20)     8993 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/renderer.py
--rw-r--r--   0 jenkins    (502) staff       (20)     3655 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/renderer_test.py
--rw-r--r--   0 jenkins    (502) staff       (20)     9004 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/rollout.cc
--rw-r--r--   0 jenkins    (502) staff       (20)     7793 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/rollout.py
--rw-r--r--   0 jenkins    (502) staff       (20)    18173 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/rollout_test.py
--rw-r--r--   0 jenkins    (502) staff       (20)     2318 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/serialization.h
-drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-04-25 14:29:14.158600 mujoco-2.3.5/mujoco/simulate/
--rw-r--r--   0 jenkins    (502) staff       (20)     9588 2023-04-25 14:29:14.000000 mujoco-2.3.5/mujoco/simulate/CMakeLists.txt
--rw-r--r--   0 jenkins    (502) staff       (20)     3337 2023-04-25 14:29:14.000000 mujoco-2.3.5/mujoco/simulate/array_safety.h
-drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-04-25 14:29:14.158815 mujoco-2.3.5/mujoco/simulate/cmake/
--rw-r--r--   0 jenkins    (502) staff       (20)     2635 2023-04-25 14:29:14.000000 mujoco-2.3.5/mujoco/simulate/cmake/SimulateDependencies.cmake
--rw-r--r--   0 jenkins    (502) staff       (20)     3918 2023-04-25 14:29:14.000000 mujoco-2.3.5/mujoco/simulate/cmake/SimulateOptions.cmake
--rw-r--r--   0 jenkins    (502) staff       (20)     7725 2023-04-25 14:29:14.000000 mujoco-2.3.5/mujoco/simulate/glfw_adapter.cc
--rw-r--r--   0 jenkins    (502) staff       (20)     2489 2023-04-25 14:29:14.000000 mujoco-2.3.5/mujoco/simulate/glfw_adapter.h
--rw-r--r--   0 jenkins    (502) staff       (20)     1487 2023-04-25 14:29:14.000000 mujoco-2.3.5/mujoco/simulate/glfw_corevideo.h
--rw-r--r--   0 jenkins    (502) staff       (20)     2530 2023-04-25 14:29:14.000000 mujoco-2.3.5/mujoco/simulate/glfw_corevideo.mm
--rw-r--r--   0 jenkins    (502) staff       (20)     4395 2023-04-25 14:29:14.000000 mujoco-2.3.5/mujoco/simulate/glfw_dispatch.cc
--rw-r--r--   0 jenkins    (502) staff       (20)     2884 2023-04-25 14:29:14.000000 mujoco-2.3.5/mujoco/simulate/glfw_dispatch.h
--rw-r--r--   0 jenkins    (502) staff       (20)     1656 2023-04-25 14:29:14.000000 mujoco-2.3.5/mujoco/simulate/macos_gui.mm
--rw-r--r--   0 jenkins    (502) staff       (20)    14318 2023-04-25 14:29:14.000000 mujoco-2.3.5/mujoco/simulate/main.cc
--rw-r--r--   0 jenkins    (502) staff       (20)     6095 2023-04-25 14:29:14.000000 mujoco-2.3.5/mujoco/simulate/platform_ui_adapter.cc
--rw-r--r--   0 jenkins    (502) staff       (20)     3319 2023-04-25 14:29:14.000000 mujoco-2.3.5/mujoco/simulate/platform_ui_adapter.h
--rw-r--r--   0 jenkins    (502) staff       (20)    74787 2023-04-25 14:29:14.000000 mujoco-2.3.5/mujoco/simulate/simulate.cc
--rw-r--r--   0 jenkins    (502) staff       (20)     8995 2023-04-25 14:29:14.000000 mujoco-2.3.5/mujoco/simulate/simulate.h
--rw-r--r--   0 jenkins    (502) staff       (20)     6913 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/simulate.cc
--rw-r--r--   0 jenkins    (502) staff       (20)    71425 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/structs.cc
--rw-r--r--   0 jenkins    (502) staff       (20)    31352 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/structs.h
-drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-04-25 14:29:14.159995 mujoco-2.3.5/mujoco/util/
--rw-r--r--   0 jenkins    (502) staff       (20)     3288 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/util/CMakeLists.txt
--rw-r--r--   0 jenkins    (502) staff       (20)     4893 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/util/array_traits.h
--rw-r--r--   0 jenkins    (502) staff       (20)     2516 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/util/array_traits_test.cc
--rw-r--r--   0 jenkins    (502) staff       (20)     2426 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/util/crossplatform.h
--rw-r--r--   0 jenkins    (502) staff       (20)     4146 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/util/func_traits.h
--rw-r--r--   0 jenkins    (502) staff       (20)     4013 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/util/func_traits_test.cc
--rw-r--r--   0 jenkins    (502) staff       (20)     7119 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/util/func_wrap.h
--rw-r--r--   0 jenkins    (502) staff       (20)     2944 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/util/func_wrap_test.cc
--rw-r--r--   0 jenkins    (502) staff       (20)     5690 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/util/tuple_tools.h
--rw-r--r--   0 jenkins    (502) staff       (20)     1945 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/util/tuple_tools_test.cc
--rw-r--r--   0 jenkins    (502) staff       (20)    12239 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/viewer.py
--rw-r--r--   0 jenkins    (502) staff       (20)      979 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/viewer_test.py
-drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-04-25 14:29:14.155863 mujoco-2.3.5/mujoco.egg-info/
--rw-r--r--   0 jenkins    (502) staff       (20)    34948 2023-04-25 14:29:14.000000 mujoco-2.3.5/mujoco.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (502) staff       (20)     2130 2023-04-25 14:29:14.000000 mujoco-2.3.5/mujoco.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (502) staff       (20)        1 2023-04-25 14:29:14.000000 mujoco-2.3.5/mujoco.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (502) staff       (20)       28 2023-04-25 14:29:14.000000 mujoco-2.3.5/mujoco.egg-info/requires.txt
--rw-r--r--   0 jenkins    (502) staff       (20)        7 2023-04-25 14:29:14.000000 mujoco-2.3.5/mujoco.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (502) staff       (20)       38 2023-04-25 14:29:14.160359 mujoco-2.3.5/setup.cfg
--rw-r--r--   0 jenkins    (502) staff       (20)    14305 2023-04-25 14:29:13.000000 mujoco-2.3.5/setup.py
+drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-06-20 17:18:03.050249 mujoco-2.3.6/
+-rw-r--r--   0 jenkins    (502) staff       (20)    11358 2023-06-20 17:18:02.000000 mujoco-2.3.6/LICENSE
+-rw-r--r--   0 jenkins    (502) staff       (20)    31030 2023-06-20 17:18:02.000000 mujoco-2.3.6/LICENSES_THIRD_PARTY.md
+-rw-r--r--   0 jenkins    (502) staff       (20)      179 2023-06-20 17:18:02.000000 mujoco-2.3.6/MANIFEST.in
+-rw-r--r--   0 jenkins    (502) staff       (20)    34962 2023-06-20 17:18:03.050111 mujoco-2.3.6/PKG-INFO
+-rw-r--r--   0 jenkins    (502) staff       (20)     2994 2023-06-20 17:18:02.000000 mujoco-2.3.6/README.md
+drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-06-20 17:18:03.039011 mujoco-2.3.6/cmake/
+-rw-r--r--   0 jenkins    (502) staff       (20)     1740 2023-06-20 17:18:02.000000 mujoco-2.3.6/cmake/CheckAvxSupport.cmake
+-rw-r--r--   0 jenkins    (502) staff       (20)     4747 2023-06-20 17:18:02.000000 mujoco-2.3.6/cmake/FindOrFetch.cmake
+-rw-r--r--   0 jenkins    (502) staff       (20)     8371 2023-06-20 17:18:02.000000 mujoco-2.3.6/cmake/MujocoDependencies.cmake
+-rw-r--r--   0 jenkins    (502) staff       (20)     1242 2023-06-20 17:18:02.000000 mujoco-2.3.6/cmake/MujocoHarden.cmake
+-rw-r--r--   0 jenkins    (502) staff       (20)     2302 2023-06-20 17:18:02.000000 mujoco-2.3.6/cmake/MujocoLinkOptions.cmake
+-rw-r--r--   0 jenkins    (502) staff       (20)     1568 2023-06-20 17:18:02.000000 mujoco-2.3.6/cmake/MujocoMacOS.cmake
+-rw-r--r--   0 jenkins    (502) staff       (20)     3918 2023-06-20 17:18:02.000000 mujoco-2.3.6/cmake/MujocoOptions.cmake
+-rw-r--r--   0 jenkins    (502) staff       (20)     2164 2023-06-20 17:18:02.000000 mujoco-2.3.6/cmake/ShellTests.cmake
+-rw-r--r--   0 jenkins    (502) staff       (20)     5676 2023-06-20 17:18:02.000000 mujoco-2.3.6/cmake/TargetAddRpath.cmake
+drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-06-20 17:18:03.043945 mujoco-2.3.6/mujoco/
+-rw-r--r--   0 jenkins    (502) staff       (20)    13479 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/CMakeLists.txt
+-rw-r--r--   0 jenkins    (502) staff       (20)     2446 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/__init__.py
+-rw-r--r--   0 jenkins    (502) staff       (20)    50462 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/bindings_test.py
+-rw-r--r--   0 jenkins    (502) staff       (20)    13444 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/callbacks.cc
+drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-06-20 17:18:03.044894 mujoco-2.3.6/mujoco/cgl/
+-rw-r--r--   0 jenkins    (502) staff       (20)     2271 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/cgl/__init__.py
+-rw-r--r--   0 jenkins    (502) staff       (20)     5204 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/cgl/cgl.py
+-rw-r--r--   0 jenkins    (502) staff       (20)     2366 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/constants.cc
+drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-06-20 17:18:03.045145 mujoco-2.3.6/mujoco/egl/
+-rw-r--r--   0 jenkins    (502) staff       (20)     4764 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/egl/__init__.py
+-rw-r--r--   0 jenkins    (502) staff       (20)     2783 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/egl/egl_ext.py
+-rw-r--r--   0 jenkins    (502) staff       (20)    31952 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/enum_traits.h
+-rw-r--r--   0 jenkins    (502) staff       (20)     4704 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/enums.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)      885 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/errors.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)     7571 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/errors.h
+-rw-r--r--   0 jenkins    (502) staff       (20)   127064 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/function_traits.h
+-rw-r--r--   0 jenkins    (502) staff       (20)    53742 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/functions.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)     7964 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/functions.h
+-rw-r--r--   0 jenkins    (502) staff       (20)     1849 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/gl_context.py
+drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-06-20 17:18:03.045283 mujoco-2.3.6/mujoco/glfw/
+-rw-r--r--   0 jenkins    (502) staff       (20)     1403 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/glfw/__init__.py
+-rw-r--r--   0 jenkins    (502) staff       (20)    20668 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/indexer_xmacro.h
+-rw-r--r--   0 jenkins    (502) staff       (20)    15911 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/indexers.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)     7177 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/indexers.h
+-rw-r--r--   0 jenkins    (502) staff       (20)     3474 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/mjdata_meta.h
+drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-06-20 17:18:03.046277 mujoco-2.3.6/mujoco/mjpython/
+-rw-r--r--   0 jenkins    (502) staff       (20)     1113 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/mjpython/Info.plist
+-rw-r--r--   0 jenkins    (502) staff       (20)   432307 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/mjpython/mjpython.icns
+-rw-r--r--   0 jenkins    (502) staff       (20)    12145 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/mjpython/mjpython.mm
+-rw-r--r--   0 jenkins    (502) staff       (20)     2286 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/mjpython/mjpython.py
+drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-06-20 17:18:03.046404 mujoco-2.3.6/mujoco/osmesa/
+-rw-r--r--   0 jenkins    (502) staff       (20)     2556 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/osmesa/__init__.py
+-rw-r--r--   0 jenkins    (502) staff       (20)     1032 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/private.h
+-rw-r--r--   0 jenkins    (502) staff       (20)     1962 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/raw.h
+-rw-r--r--   0 jenkins    (502) staff       (20)     8709 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/render.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)     3822 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/render_test.py
+-rw-r--r--   0 jenkins    (502) staff       (20)     8993 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/renderer.py
+-rw-r--r--   0 jenkins    (502) staff       (20)     3655 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/renderer_test.py
+-rw-r--r--   0 jenkins    (502) staff       (20)     9004 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/rollout.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)     7793 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/rollout.py
+-rw-r--r--   0 jenkins    (502) staff       (20)    18157 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/rollout_test.py
+-rw-r--r--   0 jenkins    (502) staff       (20)     2318 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/serialization.h
+drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-06-20 17:18:03.048271 mujoco-2.3.6/mujoco/simulate/
+-rw-r--r--   0 jenkins    (502) staff       (20)     9588 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/simulate/CMakeLists.txt
+-rw-r--r--   0 jenkins    (502) staff       (20)     3337 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/simulate/array_safety.h
+drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-06-20 17:18:03.048541 mujoco-2.3.6/mujoco/simulate/cmake/
+-rw-r--r--   0 jenkins    (502) staff       (20)     2635 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/simulate/cmake/SimulateDependencies.cmake
+-rw-r--r--   0 jenkins    (502) staff       (20)     3918 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/simulate/cmake/SimulateOptions.cmake
+-rw-r--r--   0 jenkins    (502) staff       (20)     7725 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/simulate/glfw_adapter.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)     2489 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/simulate/glfw_adapter.h
+-rw-r--r--   0 jenkins    (502) staff       (20)     1487 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/simulate/glfw_corevideo.h
+-rw-r--r--   0 jenkins    (502) staff       (20)     2530 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/simulate/glfw_corevideo.mm
+-rw-r--r--   0 jenkins    (502) staff       (20)     4395 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/simulate/glfw_dispatch.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)     2884 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/simulate/glfw_dispatch.h
+-rw-r--r--   0 jenkins    (502) staff       (20)     1656 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/simulate/macos_gui.mm
+-rw-r--r--   0 jenkins    (502) staff       (20)    14298 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/simulate/main.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)     6095 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/simulate/platform_ui_adapter.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)     3319 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/simulate/platform_ui_adapter.h
+-rw-r--r--   0 jenkins    (502) staff       (20)    79042 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/simulate/simulate.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)     8995 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/simulate/simulate.h
+-rw-r--r--   0 jenkins    (502) staff       (20)     6913 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/simulate.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)    71515 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/structs.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)    31373 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/structs.h
+drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-06-20 17:18:03.049891 mujoco-2.3.6/mujoco/util/
+-rw-r--r--   0 jenkins    (502) staff       (20)     3288 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/util/CMakeLists.txt
+-rw-r--r--   0 jenkins    (502) staff       (20)     4893 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/util/array_traits.h
+-rw-r--r--   0 jenkins    (502) staff       (20)     2516 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/util/array_traits_test.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)     2426 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/util/crossplatform.h
+-rw-r--r--   0 jenkins    (502) staff       (20)     4146 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/util/func_traits.h
+-rw-r--r--   0 jenkins    (502) staff       (20)     4013 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/util/func_traits_test.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)     7119 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/util/func_wrap.h
+-rw-r--r--   0 jenkins    (502) staff       (20)     2944 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/util/func_wrap_test.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)     5690 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/util/tuple_tools.h
+-rw-r--r--   0 jenkins    (502) staff       (20)     1945 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/util/tuple_tools_test.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)    12239 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/viewer.py
+-rw-r--r--   0 jenkins    (502) staff       (20)      979 2023-06-20 17:18:02.000000 mujoco-2.3.6/mujoco/viewer_test.py
+drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-06-20 17:18:03.044627 mujoco-2.3.6/mujoco.egg-info/
+-rw-r--r--   0 jenkins    (502) staff       (20)    34962 2023-06-20 17:18:03.000000 mujoco-2.3.6/mujoco.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (502) staff       (20)     2147 2023-06-20 17:18:03.000000 mujoco-2.3.6/mujoco.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (502) staff       (20)        1 2023-06-20 17:18:03.000000 mujoco-2.3.6/mujoco.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (502) staff       (20)       28 2023-06-20 17:18:03.000000 mujoco-2.3.6/mujoco.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (502) staff       (20)        7 2023-06-20 17:18:03.000000 mujoco-2.3.6/mujoco.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (502) staff       (20)       38 2023-06-20 17:18:03.050283 mujoco-2.3.6/setup.cfg
+-rw-r--r--   0 jenkins    (502) staff       (20)    14312 2023-06-20 17:18:02.000000 mujoco-2.3.6/setup.py
```

### Comparing `mujoco-2.3.5/LICENSE` & `mujoco-2.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/LICENSES_THIRD_PARTY.md` & `mujoco-2.3.6/LICENSES_THIRD_PARTY.md`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/PKG-INFO` & `mujoco-2.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mujoco
-Version: 2.3.5
+Version: 2.3.6
 Summary: MuJoCo Physics Simulator
 Home-page: https://github.com/deepmind/mujoco
-Author: DeepMind
+Author: Google DeepMind
 Author-email: mujoco@deepmind.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
@@ -30,16 +30,16 @@
 
 [pypi-versions-badge]: https://img.shields.io/pypi/pyversions/mujoco
 [pypi-badge]: https://badge.fury.io/py/mujoco.svg
 [pypi]: https://pypi.org/project/mujoco/
 
 This package is the canonical Python bindings for the
 [MuJoCo physics engine](https://github.com/deepmind/mujoco).
-These bindings are developed and maintained by DeepMind, and is kept up-to-date
-with the latest developments in MuJoCo itself.
+These bindings are developed and maintained by Google DeepMind, and is kept
+up-to-date with the latest developments in MuJoCo itself.
 
 The `mujoco` package provides direct access to raw MuJoCo C API functions,
 structs, constants, and enumerations. Structs are provided as Python classes,
 with Pythonic initialization and deletion semantics.
 
 It is not the aim of this package to provide fully fledged
 scene/environment/game authoring API, as there are already a number of existing
```

### Comparing `mujoco-2.3.5/README.md` & `mujoco-2.3.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 [pypi-versions-badge]: https://img.shields.io/pypi/pyversions/mujoco
 [pypi-badge]: https://badge.fury.io/py/mujoco.svg
 [pypi]: https://pypi.org/project/mujoco/
 
 This package is the canonical Python bindings for the
 [MuJoCo physics engine](https://github.com/deepmind/mujoco).
-These bindings are developed and maintained by DeepMind, and is kept up-to-date
-with the latest developments in MuJoCo itself.
+These bindings are developed and maintained by Google DeepMind, and is kept
+up-to-date with the latest developments in MuJoCo itself.
 
 The `mujoco` package provides direct access to raw MuJoCo C API functions,
 structs, constants, and enumerations. Structs are provided as Python classes,
 with Pythonic initialization and deletion semantics.
 
 It is not the aim of this package to provide fully fledged
 scene/environment/game authoring API, as there are already a number of existing
```

### Comparing `mujoco-2.3.5/cmake/CheckAvxSupport.cmake` & `mujoco-2.3.6/cmake/CheckAvxSupport.cmake`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/cmake/FindOrFetch.cmake` & `mujoco-2.3.6/cmake/FindOrFetch.cmake`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/cmake/MujocoDependencies.cmake` & `mujoco-2.3.6/cmake/MujocoDependencies.cmake`

 * *Files 2% similar despite different names*

```diff
@@ -35,30 +35,30 @@
     CACHE STRING "Version of `ccd` to be fetched."
 )
 set(MUJOCO_DEP_VERSION_qhull
     0c8fc90d2037588024d9964515c1e684f6007ecc
     CACHE STRING "Version of `qhull` to be fetched."
 )
 set(MUJOCO_DEP_VERSION_Eigen3
-    b378014fef017a829fb42c7fad15f3764bfb8ef9
+    969c31eefcdfaab11da763bea3f7502086673ab0
     CACHE STRING "Version of `Eigen3` to be fetched."
 )
 
 set(MUJOCO_DEP_VERSION_abseil
-    b971ac5250ea8de900eae9f95e06548d14cd95fe # LTS 20230125.2
+    c2435f8342c2d0ed8101cb43adfd605fdc52dca2 # LTS 20230125.3
     CACHE STRING "Version of `abseil` to be fetched."
 )
 
 set(MUJOCO_DEP_VERSION_gtest
     b796f7d44681514f58a683a3a71ff17c94edb0c1 # v1.13.0
     CACHE STRING "Version of `gtest` to be fetched."
 )
 
 set(MUJOCO_DEP_VERSION_benchmark
-    d572f4777349d43653b21d6c2fc63020ab326db2 # v1.7.1
+    2dd015dfef425c866d9a43f2c67d8b52d709acb6 # v1.8.0
     CACHE STRING "Version of `benchmark` to be fetched."
 )
 
 mark_as_advanced(MUJOCO_DEP_VERSION_lodepng)
 mark_as_advanced(MUJOCO_DEP_VERSION_tinyxml2)
 mark_as_advanced(MUJOCO_DEP_VERSION_tinyobjloader)
 mark_as_advanced(MUJOCO_DEP_VERSION_ccd)
```

### Comparing `mujoco-2.3.5/cmake/MujocoHarden.cmake` & `mujoco-2.3.6/cmake/MujocoHarden.cmake`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/cmake/MujocoLinkOptions.cmake` & `mujoco-2.3.6/cmake/MujocoLinkOptions.cmake`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/cmake/MujocoMacOS.cmake` & `mujoco-2.3.6/cmake/MujocoMacOS.cmake`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/cmake/MujocoOptions.cmake` & `mujoco-2.3.6/cmake/MujocoOptions.cmake`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/cmake/ShellTests.cmake` & `mujoco-2.3.6/cmake/ShellTests.cmake`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/cmake/TargetAddRpath.cmake` & `mujoco-2.3.6/cmake/TargetAddRpath.cmake`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/CMakeLists.txt` & `mujoco-2.3.6/mujoco/CMakeLists.txt`

 * *Files 3% similar despite different names*

```diff
@@ -80,23 +80,23 @@
     # On macOS, check if we are using mujoco.framework first.
     # Framework headers are searched differently from normal headers.
     # We need to use -F instead of the usual target_include_directories.
     find_path(MUJOCO_FRAMEWORK mujoco.Framework HINTS ${MUJOCO_FRAMEWORK_DIR})
     if(MUJOCO_FRAMEWORK)
       message("MuJoCo framework is at ${MUJOCO_FRAMEWORK}/mujoco.framework")
       set(MUJOCO_LIBRARY
-          ${MUJOCO_FRAMEWORK}/mujoco.framework/Versions/A/libmujoco.2.3.5.dylib
+          ${MUJOCO_FRAMEWORK}/mujoco.framework/Versions/A/libmujoco.2.3.6.dylib
       )
       target_compile_options(mujoco INTERFACE -F${MUJOCO_FRAMEWORK})
     endif()
   endif()
 
   if(NOT MUJOCO_FRAMEWORK)
     find_library(
-      MUJOCO_LIBRARY mujoco mujoco.2.3.5 HINTS ${MUJOCO_LIBRARY_DIR} REQUIRED
+      MUJOCO_LIBRARY mujoco mujoco.2.3.6 HINTS ${MUJOCO_LIBRARY_DIR} REQUIRED
     )
     find_path(MUJOCO_INCLUDE mujoco/mujoco.h HINTS ${MUJOCO_INCLUDE_DIR} REQUIRED)
     message("MuJoCo is at ${MUJOCO_LIBRARY}")
     message("MuJoCo headers are at ${MUJOCO_INCLUDE}")
     target_include_directories(mujoco INTERFACE "${MUJOCO_INCLUDE}")
   endif()
 
@@ -136,15 +136,15 @@
   PACKAGE_NAME
   absl
   LIBRARY_NAME
   abseil-cpp
   GIT_REPO
   https://github.com/abseil/abseil-cpp
   GIT_TAG
-  b971ac5250ea8de900eae9f95e06548d14cd95fe # LTS 20230125.2
+  c2435f8342c2d0ed8101cb43adfd605fdc52dca2 # LTS 20230125.3
   TARGETS
   ${MUJOCO_PYTHON_ABSL_TARGETS}
   EXCLUDE_FROM_ALL
 )
 foreach(absl_target IN ITEMS ${MUJOCO_PYTHON_ABSL_TARGETS})
   get_target_property(absl_target_aliased ${absl_target} ALIASED_TARGET)
   if(absl_target_aliased)
@@ -169,15 +169,15 @@
   PACKAGE_NAME
   Eigen3
   LIBRARY_NAME
   eigen
   GIT_REPO
   https://gitlab.com/libeigen/eigen
   GIT_TAG
-  b378014fef017a829fb42c7fad15f3764bfb8ef9
+  969c31eefcdfaab11da763bea3f7502086673ab0
   TARGETS
   Eigen3::Eigen
   EXCLUDE_FROM_ALL
 )
 
 # ==================== PYBIND11 ================================================
 findorfetch(
@@ -199,14 +199,19 @@
 # ==================== MUJOCO PYTHON BINDINGS ==================================
 set(SIMULATE_BUILD_EXECUTABLE OFF)
 set(SIMULATE_GLFW_DYNAMIC_SYMBOLS ON)
 add_subdirectory(simulate)
 
 add_subdirectory(util)
 
+add_library(mujoco_private_api_header INTERFACE)
+target_sources(mujoco_private_api_header INTERFACE private.h)
+set_target_properties(mujoco_private_api_header PROPERTIES PUBLIC_HEADER private.h)
+target_link_libraries(mujoco_private_api_header INTERFACE mujoco)
+
 if(EXISTS ${CMAKE_CURRENT_SOURCE_DIR}/enum_traits.h)
   add_library(enum_traits INTERFACE)
   target_sources(enum_traits INTERFACE enum_traits.h)
 else()
   add_custom_command(
     OUTPUT enum_traits.h
     COMMAND ${CMAKE_COMMAND} -E env PYTHONPATH=${mujoco_SOURCE_DIR}/mujoco ${Python3_EXECUTABLE}
@@ -238,15 +243,21 @@
   )
 endif()
 target_link_libraries(function_traits INTERFACE mujoco absl::core_headers)
 
 add_library(errors_header INTERFACE)
 target_sources(errors_header INTERFACE errors.h)
 set_target_properties(errors_header PROPERTIES PUBLIC_HEADER errors.h)
-target_link_libraries(errors_header INTERFACE crossplatform func_wrap mujoco)
+target_link_libraries(
+  errors_header
+  INTERFACE crossplatform
+            func_wrap
+            mujoco
+            mujoco_private_api_header
+)
 
 add_library(raw INTERFACE)
 target_sources(raw INTERFACE raw.h)
 set_target_properties(raw PROPERTIES PUBLIC_HEADER raw.h)
 target_link_libraries(raw INTERFACE mujoco)
 
 add_library(structs_header INTERFACE)
@@ -377,14 +388,15 @@
   structs.cc
 )
 target_link_libraries(
   _structs
   PRIVATE absl::flat_hash_map
           crossplatform
           mujoco
+          mujoco_private_api_header
           raw
           errors_header
           func_wrap
           function_traits
           structs_header
 )
```

### Comparing `mujoco-2.3.5/mujoco/__init__.py` & `mujoco-2.3.6/mujoco/__init__.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/bindings_test.py` & `mujoco-2.3.6/mujoco/bindings_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,27 +37,31 @@
     <body name="mybox" pos="0 0 0.1">
       <geom name="mybox" type="box" size="0.1 0.1 0.1" mass="0.25"/>
       <freejoint name="myfree"/>
     </body>
     <body>
       <inertial pos="0 0 0" mass="1" diaginertia="1 1 1"/>
       <site pos="0 0 -1" name="mysite" type="sphere"/>
-      <joint name="myhinge" type="hinge" axis="0 1 0"/>
+      <joint name="myhinge" type="hinge" axis="0 1 0" damping="1"/>
     </body>
     <body>
       <inertial pos="0 0 0" mass="1" diaginertia="1 1 1"/>
       <joint name="myball" type="ball"/>
     </body>
     <body mocap="true" pos="42 0 42">
       <geom type="sphere" size="0.1"/>
     </body>
   </worldbody>
   <actuator>
     <position name="myactuator" joint="myhinge"/>
   </actuator>
+  <sensor>
+    <jointvel name="myjointvel" joint="myhinge"/>
+    <accelerometer name="myaccelerometer" site="mysite"/>
+  </sensor>
 </mujoco>
 """
 
 TEST_XML_SENSOR = r"""
 <mujoco model="test">
   <worldbody>
     <geom name="myplane" type="plane" size="10 10 1"/>
@@ -507,16 +511,16 @@
       mujoco.mj_step(self.model, self.data, nstep=7)
       self.assertEqual(self.data.time, prev_time + 7 * self.model.opt.timestep)
     self.assertIn('Optionally, repeat nstep times.', mujoco.mj_step.__doc__)
 
   def test_mj_contact_list(self):
     self.assertEmpty(self.data.contact)
 
-    expected_ncon = 1234
-    self.data.ncon = expected_ncon
+    expected_ncon = 4
+    mujoco.mj_forward(self.model, self.data)
     self.assertLen(self.data.contact, expected_ncon)
 
     expected_pos = []
     for contact in self.data.contact:
       expected_pos.append(np.random.uniform(size=3))
       contact.pos = expected_pos[-1]
     self.assertLen(expected_pos, expected_ncon)
@@ -659,14 +663,51 @@
     # since pybind11 prints out the array's contents when generating TypeErrors.
     # Using `np.empty` here results in msan errors.
 
     # Check that the output argument must have the correct dtype.
     with self.assertRaises(TypeError):
       mujoco.mju_rotVecQuat(vec, quat, res=np.zeros(3, int))
 
+  def test_getsetstate(self):  # pylint: disable=invalid-name
+    mujoco.mj_step(self.model, self.data)
+
+    # Test for invalid state spec
+    invalid_spec = 2**mujoco.mjtState.mjNSTATE.value
+    expected_message = (
+        f'mj_stateSize: invalid state spec {invalid_spec} >= 2^mjNSTATE'
+    )
+    with self.assertRaisesWithLiteralMatch(mujoco.FatalError, expected_message):
+      mujoco.mj_stateSize(self.model, invalid_spec)
+
+    spec = mujoco.mjtState.mjSTATE_INTEGRATION
+    size = mujoco.mj_stateSize(self.model, spec)
+
+    state_bad_size = np.empty(size + 1, np.float64)
+    expected_message = ('state size should equal mj_stateSize(m, spec)')
+    with self.assertRaisesWithLiteralMatch(TypeError, expected_message):
+      mujoco.mj_getState(self.model, self.data, state_bad_size, spec)
+
+    # Get initial state.
+    state0 = np.empty(size, np.float64)
+    mujoco.mj_getState(self.model, self.data, state0, spec)
+
+    # Step, get next state.
+    mujoco.mj_step(self.model, self.data)
+    state1a = np.empty(size, np.float64)
+    mujoco.mj_getState(self.model, self.data, state1a, spec)
+
+    # Reset to initial state, step again, get state again.
+    mujoco.mj_setState(self.model, self.data, state0, spec)
+    mujoco.mj_step(self.model, self.data)
+    state1b = np.empty(size, np.float64)
+    mujoco.mj_getState(self.model, self.data, state1b, spec)
+
+    # Expect next states to be equal.
+    np.testing.assert_array_equal(state1a, state1b)
+
   def test_mj_jacSite(self):  # pylint: disable=invalid-name
     mujoco.mj_forward(self.model, self.data)
     site_id = mujoco.mj_name2id(self.model, mujoco.mjtObj.mjOBJ_SITE, 'mysite')
 
     # Call mj_jacSite with only jacp.
     jacp = np.empty((3, 10), np.float64)
     mujoco.mj_jacSite(self.model, self.data, jacp, None, site_id)
@@ -881,15 +922,16 @@
     self.assertEqual(mujoco.mjtDisableBit.mjDSBL_CLAMPCTRL << 1,
                      mujoco.mjtDisableBit.mjDSBL_WARMSTART)
     self.assertEqual(mujoco.mjtDisableBit.mjDSBL_CLAMPCTRL >> 3,
                      mujoco.mjtDisableBit.mjDSBL_CONTACT)
 
   def test_can_raise_error(self):
     self.data.pstack = self.data.nstack
-    with self.assertRaisesRegex(mujoco.FatalError, r'\Astack overflow'):
+    with self.assertRaisesRegex(mujoco.FatalError,
+                                r'\Amj_stackAlloc: stack overflow'):
       mujoco.mj_forward(self.model, self.data)
 
   def test_mjcb_time(self):
 
     class CallCounter:
 
       def __init__(self):
@@ -1042,14 +1084,69 @@
         pnt=[0, 0, 0],
         vec=[0, 0, 1],
         geomgroup=None,
         flg_static=0,
         bodyexclude=0,
         geomid=geomid)
 
+  def test_inverse_fd_none(self):
+    eps = 1e-6
+    flg_centered = 0
+    mujoco.mjd_inverseFD(self.model, self.data, eps, flg_centered,
+                         None, None, None, None, None, None, None)
+
+  def test_inverse_fd(self):
+    eps = 1e-6
+    flg_centered = 0
+    df_dq = np.zeros((self.model.nv, self.model.nv))
+    df_dv = np.zeros((self.model.nv, self.model.nv))
+    df_da = np.zeros((self.model.nv, self.model.nv))
+    ds_dq = np.zeros((self.model.nv, self.model.nsensordata))
+    ds_dv = np.zeros((self.model.nv, self.model.nsensordata))
+    ds_da = np.zeros((self.model.nv, self.model.nsensordata))
+    dm_dq = np.zeros((self.model.nv, self.model.nM))
+    mujoco.mjd_inverseFD(self.model, self.data, eps, flg_centered,
+                         df_dq, df_dv, df_da, ds_dq, ds_dv, ds_da, dm_dq)
+    self.assertGreater(np.linalg.norm(df_dq), eps)
+    self.assertGreater(np.linalg.norm(df_dv), eps)
+    self.assertGreater(np.linalg.norm(df_da), eps)
+    self.assertGreater(np.linalg.norm(ds_dq), eps)
+    self.assertGreater(np.linalg.norm(ds_dv), eps)
+    self.assertGreater(np.linalg.norm(ds_da), eps)
+
+  def test_banded(self):
+    n_total = 4
+    n_band = 1
+    n_dense = 1
+    dense = np.array([[1.0, 0, 0, 0.1],
+                      [0, 2.0, 0, 0.2],
+                      [0, 0, 3.0, 0.3],
+                      [0.1, 0.2, 0.3, 4.0]])
+    band = np.zeros(n_band*(n_total-n_dense) + n_dense*n_total)
+    mujoco.mju_dense2Band(band, dense, n_total, n_band, n_dense)
+    for i in range(4):
+      index = mujoco.mju_bandDiag(i, n_total, n_band, n_dense)
+      self.assertEqual(band[index], i+1)
+    dense2 = np.zeros((n_total, n_total))
+    flg_sym = 1
+    mujoco.mju_band2Dense(dense2, band, n_total, n_band, n_dense, flg_sym)
+    np.testing.assert_array_equal(dense, dense2)
+    vec = np.array([[2.0], [2.0], [3.0], [4.0]])
+    res = np.zeros_like(vec)
+    n_vec = 1
+    mujoco.mju_bandMulMatVec(res, band, vec,
+                             n_total, n_band, n_dense, n_vec, flg_sym)
+    np.testing.assert_array_equal(res, dense @ vec)
+    diag_add = 0
+    diag_mul = 0
+    mujoco.mju_cholFactorBand(band, n_total, n_band, n_dense,
+                              diag_add, diag_mul)
+    mujoco.mju_cholSolveBand(res, band, vec, n_total, n_band, n_dense)
+    np.testing.assert_almost_equal(res, np.linalg.solve(dense, vec))
+
   def test_mju_box_qp(self):
     n = 5
     res = np.zeros(n)
     r = np.zeros((n, n+7))
     index = np.zeros(n, np.int32)
     h = np.eye(n)
     g = np.ones((n,))
```

### Comparing `mujoco-2.3.5/mujoco/callbacks.cc` & `mujoco-2.3.6/mujoco/callbacks.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/cgl/__init__.py` & `mujoco-2.3.6/mujoco/cgl/__init__.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/cgl/cgl.py` & `mujoco-2.3.6/mujoco/cgl/cgl.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/constants.cc` & `mujoco-2.3.6/mujoco/constants.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/egl/__init__.py` & `mujoco-2.3.6/mujoco/egl/__init__.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/egl/egl_ext.py` & `mujoco-2.3.6/mujoco/egl/egl_ext.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/enum_traits.h` & `mujoco-2.3.6/mujoco/enum_traits.h`

 * *Files 3% similar despite different names*

```diff
@@ -346,14 +346,37 @@
   static constexpr auto values = std::array{
     std::make_pair("mjLRMODE_NONE", ::mjtLRMode::mjLRMODE_NONE),
     std::make_pair("mjLRMODE_MUSCLE", ::mjtLRMode::mjLRMODE_MUSCLE),
     std::make_pair("mjLRMODE_MUSCLEUSER", ::mjtLRMode::mjLRMODE_MUSCLEUSER),
     std::make_pair("mjLRMODE_ALL", ::mjtLRMode::mjLRMODE_ALL)};
 };
 
+struct mjtState {
+  static constexpr char name[] = "mjtState";
+  using type = ::mjtState;
+  static constexpr auto values = std::array{
+    std::make_pair("mjSTATE_TIME", ::mjtState::mjSTATE_TIME),
+    std::make_pair("mjSTATE_QPOS", ::mjtState::mjSTATE_QPOS),
+    std::make_pair("mjSTATE_QVEL", ::mjtState::mjSTATE_QVEL),
+    std::make_pair("mjSTATE_ACT", ::mjtState::mjSTATE_ACT),
+    std::make_pair("mjSTATE_WARMSTART", ::mjtState::mjSTATE_WARMSTART),
+    std::make_pair("mjSTATE_CTRL", ::mjtState::mjSTATE_CTRL),
+    std::make_pair("mjSTATE_QFRC_APPLIED", ::mjtState::mjSTATE_QFRC_APPLIED),
+    std::make_pair("mjSTATE_XFRC_APPLIED", ::mjtState::mjSTATE_XFRC_APPLIED),
+    std::make_pair("mjSTATE_MOCAP_POS", ::mjtState::mjSTATE_MOCAP_POS),
+    std::make_pair("mjSTATE_MOCAP_QUAT", ::mjtState::mjSTATE_MOCAP_QUAT),
+    std::make_pair("mjSTATE_USERDATA", ::mjtState::mjSTATE_USERDATA),
+    std::make_pair("mjSTATE_PLUGIN", ::mjtState::mjSTATE_PLUGIN),
+    std::make_pair("mjNSTATE", ::mjtState::mjNSTATE),
+    std::make_pair("mjSTATE_PHYSICS", ::mjtState::mjSTATE_PHYSICS),
+    std::make_pair("mjSTATE_FULLPHYSICS", ::mjtState::mjSTATE_FULLPHYSICS),
+    std::make_pair("mjSTATE_USER", ::mjtState::mjSTATE_USER),
+    std::make_pair("mjSTATE_INTEGRATION", ::mjtState::mjSTATE_INTEGRATION)};
+};
+
 struct mjtWarning {
   static constexpr char name[] = "mjtWarning";
   using type = ::mjtWarning;
   static constexpr auto values = std::array{
     std::make_pair("mjWARN_INERTIA", ::mjtWarning::mjWARN_INERTIA),
     std::make_pair("mjWARN_CONTACTFULL", ::mjtWarning::mjWARN_CONTACTFULL),
     std::make_pair("mjWARN_CNSTRFULL", ::mjtWarning::mjWARN_CNSTRFULL),
@@ -487,14 +510,15 @@
     std::make_pair("mjVIS_TRANSPARENT", ::mjtVisFlag::mjVIS_TRANSPARENT),
     std::make_pair("mjVIS_AUTOCONNECT", ::mjtVisFlag::mjVIS_AUTOCONNECT),
     std::make_pair("mjVIS_COM", ::mjtVisFlag::mjVIS_COM),
     std::make_pair("mjVIS_SELECT", ::mjtVisFlag::mjVIS_SELECT),
     std::make_pair("mjVIS_STATIC", ::mjtVisFlag::mjVIS_STATIC),
     std::make_pair("mjVIS_SKIN", ::mjtVisFlag::mjVIS_SKIN),
     std::make_pair("mjVIS_MIDPHASE", ::mjtVisFlag::mjVIS_MIDPHASE),
+    std::make_pair("mjVIS_MESHBVH", ::mjtVisFlag::mjVIS_MESHBVH),
     std::make_pair("mjNVISFLAG", ::mjtVisFlag::mjNVISFLAG)};
 };
 
 struct mjtRndFlag {
   static constexpr char name[] = "mjtRndFlag";
   using type = ::mjtRndFlag;
   static constexpr auto values = std::array{
@@ -607,14 +631,15 @@
     std::make_pair("mjITEM_RADIO", ::mjtItem::mjITEM_RADIO),
     std::make_pair("mjITEM_RADIOLINE", ::mjtItem::mjITEM_RADIOLINE),
     std::make_pair("mjITEM_SELECT", ::mjtItem::mjITEM_SELECT),
     std::make_pair("mjITEM_SLIDERINT", ::mjtItem::mjITEM_SLIDERINT),
     std::make_pair("mjITEM_SLIDERNUM", ::mjtItem::mjITEM_SLIDERNUM),
     std::make_pair("mjITEM_EDITINT", ::mjtItem::mjITEM_EDITINT),
     std::make_pair("mjITEM_EDITNUM", ::mjtItem::mjITEM_EDITNUM),
+    std::make_pair("mjITEM_EDITFLOAT", ::mjtItem::mjITEM_EDITFLOAT),
     std::make_pair("mjITEM_EDITTXT", ::mjtItem::mjITEM_EDITTXT),
     std::make_pair("mjNITEM", ::mjtItem::mjNITEM)};
 };
 
 static constexpr auto kAllEnums = std::make_tuple(
     mjtDisableBit{},
     mjtEnableBit{},
@@ -636,14 +661,15 @@
     mjtObj{},
     mjtConstraint{},
     mjtConstraintState{},
     mjtSensor{},
     mjtStage{},
     mjtDataType{},
     mjtLRMode{},
+    mjtState{},
     mjtWarning{},
     mjtTimer{},
     mjtCatBit{},
     mjtMouse{},
     mjtPertBit{},
     mjtCamera{},
     mjtLabel{},
```

### Comparing `mujoco-2.3.5/mujoco/enums.cc` & `mujoco-2.3.6/mujoco/enums.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/errors.cc` & `mujoco-2.3.6/mujoco/errors.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/errors.h` & `mujoco-2.3.6/mujoco/errors.h`

 * *Files 2% similar despite different names*

```diff
@@ -17,24 +17,19 @@
 
 #include <csetjmp>
 #include <stdexcept>
 #include <string>
 #include <type_traits>
 
 #include <mujoco/mjexport.h>
+#include "private.h"
 #include "util/crossplatform.h"
 #include "util/func_wrap.h"
 #include <pybind11/pybind11.h>
 
-// DO NOT USE THIS FUNCTION ELSEWHERE.
-// It should be regarded as part of MuJoCo's internal implementation detail.
-extern "C" {
-MJAPI void _mjPRIVATE__set_tls_error_fn(void (*h)(const char*));
-}
-
 // When building for Linux and statically linking against a "hermetic" libc++abi
 // (i.e. where libc++/libc++abi symbols all have "hidden" visibility), exception
 // types do not propagate correctly across shared library boundaries.
 //
 // This occurs even when PYBIND11_EXPORT_EXCEPTION is used, or when the virtual
 // destructor is defined in errors.cc rather than than defined inline in the
 // class definition (following the FAQ comment about "key functions" on
```

### Comparing `mujoco-2.3.5/mujoco/function_traits.h` & `mujoco-2.3.6/mujoco/function_traits.h`

 * *Files 0% similar despite different names*

```diff
@@ -909,14 +909,47 @@
   static constexpr auto param_names = std::make_tuple("m", "d", "jar", "cost", "flg_coneHessian");
 
   MUJOCO_ALWAYS_INLINE static type& GetFunc() {
     return *reinterpret_cast<type*>(&::mj_constraintUpdate);
   }
 };
 
+struct mj_stateSize {
+  static constexpr char name[] = "mj_stateSize";
+  static constexpr char doc[] = "Return size of state specification.";
+  using type = int (const mjModel *, unsigned int);
+  static constexpr auto param_names = std::make_tuple("m", "spec");
+
+  MUJOCO_ALWAYS_INLINE static type& GetFunc() {
+    return ::mj_stateSize;
+  }
+};
+
+struct mj_getState {
+  static constexpr char name[] = "mj_getState";
+  static constexpr char doc[] = "Get state.";
+  using type = void (const mjModel *, const mjData *, mjtNum *, unsigned int);
+  static constexpr auto param_names = std::make_tuple("m", "d", "state", "spec");
+
+  MUJOCO_ALWAYS_INLINE static type& GetFunc() {
+    return ::mj_getState;
+  }
+};
+
+struct mj_setState {
+  static constexpr char name[] = "mj_setState";
+  static constexpr char doc[] = "Set state.";
+  using type = void (const mjModel *, mjData *, const mjtNum *, unsigned int);
+  static constexpr auto param_names = std::make_tuple("m", "d", "state", "spec");
+
+  MUJOCO_ALWAYS_INLINE static type& GetFunc() {
+    return ::mj_setState;
+  }
+};
+
 struct mj_addContact {
   static constexpr char name[] = "mj_addContact";
   static constexpr char doc[] = "Add contact to d->contact list; return 0 if success; 1 if buffer full.";
   using type = int (const mjModel *, mjData *, const mjContact *);
   static constexpr auto param_names = std::make_tuple("m", "d", "con");
 
   MUJOCO_ALWAYS_INLINE static type& GetFunc() {
@@ -1283,14 +1316,25 @@
   static constexpr auto param_names = std::make_tuple();
 
   MUJOCO_ALWAYS_INLINE static type& GetFunc() {
     return ::mj_versionString;
   }
 };
 
+struct mj_multiRay {
+  static constexpr char name[] = "mj_multiRay";
+  static constexpr char doc[] = "Intersect multiple rays emanating from a single point. Similar semantics to mj_ray, but vec is an array of (nray x 3) directions.";
+  using type = void (const mjModel *, mjData *, const mjtNum (*)[3], const mjtNum *, const mjtByte *, mjtByte, int, int *, mjtNum *, int, mjtNum);
+  static constexpr auto param_names = std::make_tuple("m", "d", "pnt", "vec", "geomgroup", "flg_static", "bodyexclude", "geomid", "dist", "nray", "cutoff");
+
+  MUJOCO_ALWAYS_INLINE static type& GetFunc() {
+    return *reinterpret_cast<type*>(&::mj_multiRay);
+  }
+};
+
 struct mj_ray {
   static constexpr char name[] = "mj_ray";
   static constexpr char doc[] = "Intersect ray (pnt+x*vec, x>=0) with visible geoms, except geoms in bodyexclude. Return distance (x) to nearest surface, or -1 if no intersection and output geomid. geomgroup, flg_static are as in mjvOption; geomgroup==NULL skips group exclusion.";
   using type = mjtNum (const mjModel *, const mjData *, const mjtNum (*)[3], const mjtNum (*)[3], const mjtByte *, mjtByte, int, int (*)[1]);
   static constexpr auto param_names = std::make_tuple("m", "d", "pnt", "vec", "geomgroup", "flg_static", "bodyexclude", "geomid");
 
   MUJOCO_ALWAYS_INLINE static type& GetFunc() {
@@ -2185,36 +2229,14 @@
   static constexpr auto param_names = std::make_tuple("type", "msg");
 
   MUJOCO_ALWAYS_INLINE static type& GetFunc() {
     return ::mju_writeLog;
   }
 };
 
-struct mj_activate {
-  static constexpr char name[] = "mj_activate";
-  static constexpr char doc[] = "Return 1 (for backward compatibility).";
-  using type = int (const char *);
-  static constexpr auto param_names = std::make_tuple("filename");
-
-  MUJOCO_ALWAYS_INLINE static type& GetFunc() {
-    return ::mj_activate;
-  }
-};
-
-struct mj_deactivate {
-  static constexpr char name[] = "mj_deactivate";
-  static constexpr char doc[] = "Do nothing (for backward compatibility).";
-  using type = void ();
-  static constexpr auto param_names = std::make_tuple();
-
-  MUJOCO_ALWAYS_INLINE static type& GetFunc() {
-    return ::mj_deactivate;
-  }
-};
-
 struct mju_zero3 {
   static constexpr char name[] = "mju_zero3";
   static constexpr char doc[] = "Set res = 0.";
   using type = void (mjtNum (*)[3]);
   static constexpr auto param_names = std::make_tuple("res");
 
   MUJOCO_ALWAYS_INLINE static type& GetFunc() {
@@ -2891,15 +2913,15 @@
   MUJOCO_ALWAYS_INLINE static type& GetFunc() {
     return ::mju_cholFactor;
   }
 };
 
 struct mju_cholSolve {
   static constexpr char name[] = "mju_cholSolve";
-  static constexpr char doc[] = "Solve mat * res = vec, where mat is Cholesky-factorized";
+  static constexpr char doc[] = "Solve (mat*mat') * res = vec, where mat is a Cholesky factor.";
   using type = void (mjtNum *, const mjtNum *, const mjtNum *, int);
   static constexpr auto param_names = std::make_tuple("res", "mat", "vec", "n");
 
   MUJOCO_ALWAYS_INLINE static type& GetFunc() {
     return ::mju_cholSolve;
   }
 };
@@ -2911,14 +2933,80 @@
   static constexpr auto param_names = std::make_tuple("mat", "x", "n", "flg_plus");
 
   MUJOCO_ALWAYS_INLINE static type& GetFunc() {
     return ::mju_cholUpdate;
   }
 };
 
+struct mju_cholFactorBand {
+  static constexpr char name[] = "mju_cholFactorBand";
+  static constexpr char doc[] = "Band-dense Cholesky decomposition.  Returns minimum value in the factorized diagonal, or 0 if rank-deficient.  mat has (ntotal-ndense) x nband + ndense x ntotal elements.  The first (ntotal-ndense) x nband store the band part, left of diagonal, inclusive.  The second ndense x ntotal store the band part as entire dense rows.  Add diagadd+diagmul*mat_ii to diagonal before factorization.";
+  using type = mjtNum (mjtNum *, int, int, int, mjtNum, mjtNum);
+  static constexpr auto param_names = std::make_tuple("mat", "ntotal", "nband", "ndense", "diagadd", "diagmul");
+
+  MUJOCO_ALWAYS_INLINE static type& GetFunc() {
+    return ::mju_cholFactorBand;
+  }
+};
+
+struct mju_cholSolveBand {
+  static constexpr char name[] = "mju_cholSolveBand";
+  static constexpr char doc[] = "Solve (mat*mat')*res = vec where mat is a band-dense Cholesky factor.";
+  using type = void (mjtNum *, const mjtNum *, const mjtNum *, int, int, int);
+  static constexpr auto param_names = std::make_tuple("res", "mat", "vec", "ntotal", "nband", "ndense");
+
+  MUJOCO_ALWAYS_INLINE static type& GetFunc() {
+    return ::mju_cholSolveBand;
+  }
+};
+
+struct mju_band2Dense {
+  static constexpr char name[] = "mju_band2Dense";
+  static constexpr char doc[] = "Convert banded matrix to dense matrix, fill upper triangle if flg_sym>0.";
+  using type = void (mjtNum *, const mjtNum *, int, int, int, mjtByte);
+  static constexpr auto param_names = std::make_tuple("res", "mat", "ntotal", "nband", "ndense", "flg_sym");
+
+  MUJOCO_ALWAYS_INLINE static type& GetFunc() {
+    return ::mju_band2Dense;
+  }
+};
+
+struct mju_dense2Band {
+  static constexpr char name[] = "mju_dense2Band";
+  static constexpr char doc[] = "Convert dense matrix to banded matrix.";
+  using type = void (mjtNum *, const mjtNum *, int, int, int);
+  static constexpr auto param_names = std::make_tuple("res", "mat", "ntotal", "nband", "ndense");
+
+  MUJOCO_ALWAYS_INLINE static type& GetFunc() {
+    return ::mju_dense2Band;
+  }
+};
+
+struct mju_bandMulMatVec {
+  static constexpr char name[] = "mju_bandMulMatVec";
+  static constexpr char doc[] = "Multiply band-diagonal matrix with nvec vectors, include upper triangle if flg_sym>0.";
+  using type = void (mjtNum *, const mjtNum *, const mjtNum *, int, int, int, int, mjtByte);
+  static constexpr auto param_names = std::make_tuple("res", "mat", "vec", "ntotal", "nband", "ndense", "nvec", "flg_sym");
+
+  MUJOCO_ALWAYS_INLINE static type& GetFunc() {
+    return ::mju_bandMulMatVec;
+  }
+};
+
+struct mju_bandDiag {
+  static constexpr char name[] = "mju_bandDiag";
+  static constexpr char doc[] = "Address of diagonal element i in band-dense matrix representation.";
+  using type = int (int, int, int, int);
+  static constexpr auto param_names = std::make_tuple("i", "ntotal", "nband", "ndense");
+
+  MUJOCO_ALWAYS_INLINE static type& GetFunc() {
+    return ::mju_bandDiag;
+  }
+};
+
 struct mju_eig3 {
   static constexpr char name[] = "mju_eig3";
   static constexpr char doc[] = "Eigenvalue decomposition of symmetric 3x3 matrix.";
   using type = int (mjtNum (*)[3], mjtNum (*)[9], mjtNum (*)[4], const mjtNum (*)[9]);
   static constexpr auto param_names = std::make_tuple("eigval", "eigvec", "quat", "mat");
 
   MUJOCO_ALWAYS_INLINE static type& GetFunc() {
@@ -2968,16 +3056,16 @@
   MUJOCO_ALWAYS_INLINE static type& GetFunc() {
     return *reinterpret_cast<type*>(&::mju_muscleBias);
   }
 };
 
 struct mju_muscleDynamics {
   static constexpr char name[] = "mju_muscleDynamics";
-  static constexpr char doc[] = "Muscle activation dynamics, prm = (tau_act, tau_deact).";
-  using type = mjtNum (mjtNum, mjtNum, const mjtNum (*)[2]);
+  static constexpr char doc[] = "Muscle activation dynamics, prm = (tau_act, tau_deact, smoothing_width).";
+  using type = mjtNum (mjtNum, mjtNum, const mjtNum (*)[3]);
   static constexpr auto param_names = std::make_tuple("ctrl", "act", "prm");
 
   MUJOCO_ALWAYS_INLINE static type& GetFunc() {
     return *reinterpret_cast<type*>(&::mju_muscleDynamics);
   }
 };
 
@@ -3232,34 +3320,45 @@
   MUJOCO_ALWAYS_INLINE static type& GetFunc() {
     return ::mju_strncpy;
   }
 };
 
 struct mju_sigmoid {
   static constexpr char name[] = "mju_sigmoid";
-  static constexpr char doc[] = "Sigmoid function over 0<=x<=1 constructed from half-quadratics.";
+  static constexpr char doc[] = "Sigmoid function over 0<=x<=1 using quintic polynomial.";
   using type = mjtNum (mjtNum);
   static constexpr auto param_names = std::make_tuple("x");
 
   MUJOCO_ALWAYS_INLINE static type& GetFunc() {
     return ::mju_sigmoid;
   }
 };
 
 struct mjd_transitionFD {
   static constexpr char name[] = "mjd_transitionFD";
   static constexpr char doc[] = "Finite differenced transition matrices (control theory notation)   d(x_next) = A*dx + B*du   d(sensor) = C*dx + D*du   required output matrix dimensions:      A: (2*nv+na x 2*nv+na)      B: (2*nv+na x nu)      D: (nsensordata x 2*nv+na)      C: (nsensordata x nu)";
   using type = void (const mjModel *, mjData *, mjtNum, mjtByte, mjtNum *, mjtNum *, mjtNum *, mjtNum *);
-  static constexpr auto param_names = std::make_tuple("m", "d", "eps", "centered", "A", "B", "C", "D");
+  static constexpr auto param_names = std::make_tuple("m", "d", "eps", "flg_centered", "A", "B", "C", "D");
 
   MUJOCO_ALWAYS_INLINE static type& GetFunc() {
     return ::mjd_transitionFD;
   }
 };
 
+struct mjd_inverseFD {
+  static constexpr char name[] = "mjd_inverseFD";
+  static constexpr char doc[] = "Finite differenced Jacobians of (force, sensors) = mj_inverse(state, acceleration)   All outputs are optional. Output dimensions (transposed w.r.t Control Theory convention):     DfDq: (nv x nv)     DfDv: (nv x nv)     DfDa: (nv x nv)     DsDq: (nv x nsensordata)     DsDv: (nv x nsensordata)     DsDa: (nv x nsensordata)     DmDq: (nv x nM)   single-letter shortcuts:     inputs: q=qpos, v=qvel, a=qacc     outputs: f=qfrc_inverse, s=sensordata, m=qM   notes:     optionally computes mass matrix Jacobian DmDq     flg_actuation specifies whether to subtract qfrc_actuator from qfrc_inverse";
+  using type = void (const mjModel *, mjData *, mjtNum, mjtByte, mjtNum *, mjtNum *, mjtNum *, mjtNum *, mjtNum *, mjtNum *, mjtNum *);
+  static constexpr auto param_names = std::make_tuple("m", "d", "eps", "flg_actuation", "DfDq", "DfDv", "DfDa", "DsDq", "DsDv", "DsDa", "DmDq");
+
+  MUJOCO_ALWAYS_INLINE static type& GetFunc() {
+    return ::mjd_inverseFD;
+  }
+};
+
 struct mjp_defaultPlugin {
   static constexpr char name[] = "mjp_defaultPlugin";
   static constexpr char doc[] = "Set default plugin definition.";
   using type = void (mjpPlugin *);
   static constexpr auto param_names = std::make_tuple("plugin");
 
   MUJOCO_ALWAYS_INLINE static type& GetFunc() {
```

### Comparing `mujoco-2.3.5/mujoco/functions.cc` & `mujoco-2.3.6/mujoco/functions.cc`

 * *Files 2% similar despite different names*

```diff
@@ -38,18 +38,14 @@
       mjtNum, Eigen::Dynamic, Eigen::Dynamic, Eigen::RowMajor>;
 
 
   // Import the _structs module so that pybind11 knows about Python bindings
   // for MjWrapper types and therefore generates prettier docstrings.
   py::module::import("mujoco._structs");
 
-  // Activation
-  Def<traits::mj_activate>(pymodule);
-  Def<traits::mj_deactivate>(pymodule);
-
   // Virtual file system
   // Skipped entire section
 
   // Parse and compile
   // Skipped: mj_loadXML (have MjModel.from_xml_string)
   DEF_WITH_OMITTED_PY_ARGS(traits::mj_saveLastXML, "error", "error_sz")(
       pymodule,
@@ -269,14 +265,33 @@
         }
         return InterceptMjErrors(::mj_constraintUpdate)(
             m, d, jar.data(), cost.has_value() ? cost->data() : nullptr,
             flg_coneHessian);
       });
 
   // Support
+  Def<traits::mj_stateSize>(pymodule);
+  Def<traits::mj_getState>(
+      pymodule,
+      [](const raw::MjModel* m, const raw::MjData* d,
+         Eigen::Ref<EigenVectorX> state, unsigned int spec) {
+        if (state.size() != mj_stateSize(m, spec)) {
+          throw py::type_error("state size should equal mj_stateSize(m, spec)");
+        }
+        return InterceptMjErrors(::mj_getState)(m, d, state.data(), spec);
+      });
+  Def<traits::mj_setState>(
+      pymodule,
+      [](const raw::MjModel* m, raw::MjData* d,
+         const Eigen::Ref<EigenVectorX> state, unsigned int spec) {
+        if (state.size() != mj_stateSize(m, spec)) {
+          throw py::type_error("state size should equal mj_stateSize(m, spec)");
+        }
+        return InterceptMjErrors(::mj_setState)(m, d, state.data(), spec);
+      });
   Def<traits::mj_addContact>(pymodule);
   Def<traits::mj_isPyramidal>(pymodule);
   Def<traits::mj_isSparse>(pymodule);
   Def<traits::mj_isDual>(pymodule);
   Def<traits::mj_mulJacVec>(
       pymodule,
       [](const raw::MjModel* m, raw::MjData* d, Eigen::Ref<EigenVectorX> res,
@@ -496,15 +511,15 @@
   Def<traits::mj_contactForce>(pymodule);
   Def<traits::mj_differentiatePos>(
       pymodule,
       [](const raw::MjModel* m, Eigen::Ref<EigenVectorX> qvel,
          mjtNum dt, Eigen::Ref<const EigenVectorX> qpos1,
          Eigen::Ref<const EigenVectorX> qpos2) {
         if (qvel.size() != m->nv) {
-          throw py::type_error("qvel should be of size nq");
+          throw py::type_error("qvel should be of size nv");
         }
         if (qpos1.size() != m->nq) {
           throw py::type_error("qpos1 should be of size nq");
         }
         if (qpos2.size() != m->nq) {
           throw py::type_error("qpos2 should be of size nq");
         }
@@ -515,15 +530,15 @@
       pymodule,
       [](const raw::MjModel* m, Eigen::Ref<EigenVectorX> qpos,
          Eigen::Ref<const EigenVectorX> qvel, mjtNum dt) {
         if (qpos.size() != m->nq) {
           throw py::type_error("qpos should be of size nq");
         }
         if (qvel.size() != m->nv) {
-          throw py::type_error("qvel should be of size nq");
+          throw py::type_error("qvel should be of size nv");
         }
         return InterceptMjErrors(::mj_integratePos)(
             m, qpos.data(), qvel.data(), dt);
       });
   Def<traits::mj_normalizeQuat>(
       pymodule,
       [](const raw::MjModel* m, Eigen::Ref<EigenVectorX> qpos) {
@@ -542,14 +557,15 @@
         InterceptMjErrors(::mj_loadAllPluginLibraries)(
             directory.c_str(), nullptr);
       });
   Def<traits::mj_version>(pymodule);
   Def<traits::mj_versionString>(pymodule);
 
   // Ray collision
+  Def<traits::mj_multiRay>(pymodule);
   Def<traits::mj_ray>(
       pymodule,
       [](const raw::MjModel* m, const raw::MjData* d, const mjtNum(*pnt)[3],
          const mjtNum(*vec)[3],
          std::optional<Eigen::Ref<const Eigen::Vector<mjtByte, mjNGROUP>>>
              geomgroup,
          mjtByte flg_static, int bodyexclude, int(*geomid)[1]) {
@@ -986,14 +1002,107 @@
         if (x.size() != mat.rows()) {
           throw py::type_error(
               "size of x should equal the number of rows in mat");
         }
         return InterceptMjErrors(::mju_cholUpdate)(
             mat.data(), x.data(), mat.rows(), flg_plus);
       });
+  Def<traits::mju_cholFactorBand>(
+      pymodule, [](Eigen::Ref<EigenVectorX> mat, int ntotal, int nband,
+                   int ndense, mjtNum diagadd, mjtNum diagmul) {
+        int nMat = (ntotal - ndense) * nband + ndense * ntotal;
+        if (mat.size() != nMat) {
+          throw py::type_error(
+              "mat must have size (ntotal-ndense)*nband + ndense*ntotal");
+        }
+        return InterceptMjErrors(::mju_cholFactorBand)(
+            mat.data(), ntotal, nband, ndense, diagadd, diagmul);
+      });
+  Def<traits::mju_cholSolveBand>(
+      pymodule,
+      [](Eigen::Ref<EigenVectorX> res, Eigen::Ref<const EigenVectorX> mat,
+         Eigen::Ref<const EigenVectorX> vec, int ntotal, int nband,
+         int ndense) {
+        int nMat = (ntotal - ndense) * nband + ndense * ntotal;
+        if (mat.size() != nMat) {
+          throw py::type_error(
+              "mat must have (ntotal-ndense)*nband + "
+              "ndense*ntotal elements");
+        }
+        if (res.size() != ntotal) {
+          throw py::type_error("size of res should equal ntotal");
+        }
+        if (vec.size() != ntotal) {
+          throw py::type_error("size of vec should equal ntotal");
+        }
+        return InterceptMjErrors(::mju_cholSolveBand)(
+            res.data(), mat.data(), vec.data(), ntotal, nband, ndense);
+      });
+  Def<traits::mju_band2Dense>(
+      pymodule,
+      [](Eigen::Ref<EigenArrayXX> res, Eigen::Ref<const EigenVectorX> mat,
+         int ntotal, int nband, int ndense, mjtByte flg_sym) {
+        int nMat = (ntotal - ndense) * nband + ndense * ntotal;
+        if (mat.size() != nMat) {
+          throw py::type_error(
+              "mat must have size (ntotal-ndense)*nband + ndense*ntotal");
+        }
+        if (res.rows() != ntotal) {
+          throw py::type_error("res should have ntotal rows");
+        }
+        if (res.cols() != ntotal) {
+          throw py::type_error("res should have ntotal columns");
+        }
+        return InterceptMjErrors(::mju_band2Dense)(
+            res.data(), mat.data(), ntotal, nband, ndense, flg_sym);
+      });
+  Def<traits::mju_dense2Band>(pymodule, [](Eigen::Ref<EigenVectorX> res,
+                                           Eigen::Ref<const EigenArrayXX> mat,
+                                           int ntotal, int nband, int ndense) {
+    int nRes = (ntotal - ndense) * nband + ndense * ntotal;
+    if (res.size() != nRes) {
+      throw py::type_error(
+          "res must have size (ntotal-ndense)*nband + ndense*ntotal");
+    }
+    if (mat.rows() != ntotal) {
+      throw py::type_error("mat should have ntotal rows");
+    }
+    if (mat.cols() != ntotal) {
+      throw py::type_error("mat should have ntotal columns");
+    }
+    return InterceptMjErrors(::mju_dense2Band)(res.data(), mat.data(), ntotal,
+                                               nband, ndense);
+  });
+  Def<traits::mju_bandMulMatVec>(
+      pymodule,
+      [](Eigen::Ref<EigenVectorX> res, Eigen::Ref<const EigenArrayXX> mat,
+         Eigen::Ref<const EigenArrayXX> vec, int ntotal, int nband, int ndense,
+         int nVec, mjtByte flg_sym) {
+        int nMat = (ntotal - ndense) * nband + ndense * ntotal;
+        if (mat.size() != nMat) {
+          throw py::type_error(
+              "mat must have size (ntotal-ndense)*nband + ndense*ntotal");
+        }
+        if (res.rows() != ntotal) {
+          throw py::type_error("res should have ntotal rows");
+        }
+        if (res.cols() != nVec) {
+          throw py::type_error("res should have nVec columns");
+        }
+        if (vec.rows() != ntotal) {
+          throw py::type_error("vec should have ntotal rows");
+        }
+        if (vec.cols() != nVec) {
+          throw py::type_error("vec should have nVec columns");
+        }
+        return InterceptMjErrors(::mju_bandMulMatVec)(res.data(), mat.data(),
+                                                      vec.data(), ntotal, nband,
+                                                      ndense, nVec, flg_sym);
+      });
+  Def<traits::mju_bandDiag>(pymodule);
   Def<traits::mju_eig3>(pymodule);
   DEF_WITH_OMITTED_PY_ARGS(traits::mju_boxQP, "n")(
       pymodule,
       [](Eigen::Ref<EigenVectorX> res,
          Eigen::Ref<EigenArrayXX> R,
          std::optional<Eigen::Ref<Eigen::Vector<int, Eigen::Dynamic>>> index,
          Eigen::Ref<const EigenArrayXX> H,
@@ -1127,15 +1236,16 @@
       pymodule,
       [](Eigen::Ref<Eigen::Vector<int, Eigen::Dynamic>> res) {
         return InterceptMjErrors(::mju_insertionSortInt)(
             res.data(), res.size());
       });
   Def<traits::mjd_transitionFD>(
       pymodule,
-      [](const raw::MjModel* m, raw::MjData* d, mjtNum eps, mjtByte centered,
+      [](const raw::MjModel* m, raw::MjData* d,
+         mjtNum eps, mjtByte flg_centered,
          std::optional<Eigen::Ref<EigenArrayXX>> A,
          std::optional<Eigen::Ref<EigenArrayXX>> B,
          std::optional<Eigen::Ref<EigenArrayXX>> C,
          std::optional<Eigen::Ref<EigenArrayXX>> D) {
         if (A.has_value() &&
             (A->rows() != 2*m->nv+m->na || A->cols() != 2*m->nv+m->na)) {
           throw py::type_error("A should be of shape (2*nv+na, 2*nv+na)");
@@ -1149,19 +1259,68 @@
           throw py::type_error("C should be of shape (nsensordata, 2*nv+na)");
         }
         if (D.has_value() &&
             (D->rows() != m->nsensordata || D->cols() != m->nu)) {
           throw py::type_error("D should be of shape (nsensordata, nu)");
         }
         return InterceptMjErrors(::mjd_transitionFD)(
-            m, d, eps, centered,
+            m, d, eps, flg_centered,
             A.has_value() ? A->data() : nullptr,
             B.has_value() ? B->data() : nullptr,
             C.has_value() ? C->data() : nullptr,
             D.has_value() ? D->data() : nullptr);
       });
+  Def<traits::mjd_inverseFD>(
+      pymodule,
+      [](const raw::MjModel* m, raw::MjData* d,
+         mjtNum eps, mjtByte flg_actuation,
+         std::optional<Eigen::Ref<EigenArrayXX>> DfDq,
+         std::optional<Eigen::Ref<EigenArrayXX>> DfDv,
+         std::optional<Eigen::Ref<EigenArrayXX>> DfDa,
+         std::optional<Eigen::Ref<EigenArrayXX>> DsDq,
+         std::optional<Eigen::Ref<EigenArrayXX>> DsDv,
+         std::optional<Eigen::Ref<EigenArrayXX>> DsDa,
+         std::optional<Eigen::Ref<EigenArrayXX>> DmDq) {
+        if (DfDq.has_value() &&
+            (DfDq->rows() != m->nv || DfDq->cols() != m->nv)) {
+          throw py::type_error("DfDq should be of shape (nv, nv)");
+        }
+        if (DfDv.has_value() &&
+            (DfDv->rows() != m->nv || DfDv->cols() != m->nv)) {
+          throw py::type_error("DfDv should be of shape (nv, nv)");
+        }
+        if (DfDa.has_value() &&
+            (DfDa->rows() != m->nv || DfDa->cols() != m->nv)) {
+          throw py::type_error("DfDa should be of shape (nv, nv)");
+        }
+        if (DsDq.has_value() &&
+            (DsDq->rows() != m->nv || DsDq->cols() != m->nsensordata)) {
+          throw py::type_error("DsDq should be of shape (nv, nsensordata)");
+        }
+        if (DsDv.has_value() &&
+            (DsDv->rows() != m->nv || DsDv->cols() != m->nsensordata)) {
+          throw py::type_error("DsDv should be of shape (nv, nsensordata)");
+        }
+        if (DsDa.has_value() &&
+            (DsDa->rows() != m->nv || DsDa->cols() != m->nsensordata)) {
+          throw py::type_error("DsDa should be of shape (nv, nsensordata)");
+        }
+        if (DmDq.has_value() &&
+            (DmDq->rows() != m->nv || DmDq->cols() != m->nM)) {
+          throw py::type_error("DmDq should be of shape (nv, nM)");
+        }
+        return InterceptMjErrors(::mjd_inverseFD)(
+            m, d, eps, flg_actuation,
+            DfDq.has_value() ? DfDq->data() : nullptr,
+            DfDv.has_value() ? DfDv->data() : nullptr,
+            DfDa.has_value() ? DfDa->data() : nullptr,
+            DsDq.has_value() ? DsDq->data() : nullptr,
+            DsDv.has_value() ? DsDv->data() : nullptr,
+            DsDa.has_value() ? DsDa->data() : nullptr,
+            DmDq.has_value() ? DmDq->data() : nullptr);
+      });
   Def<traits::mju_Halton>(pymodule);
   // Skipped: mju_strncpy (doesn't make sense in Python)
   Def<traits::mju_sigmoid>(pymodule);
 }  // PYBIND11_MODULE NOLINT(readability/fn_size)
 }  // namespace
 }  // namespace mujoco::python
```

### Comparing `mujoco-2.3.5/mujoco/functions.h` & `mujoco-2.3.6/mujoco/functions.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/gl_context.py` & `mujoco-2.3.6/mujoco/gl_context.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/glfw/__init__.py` & `mujoco-2.3.6/mujoco/glfw/__init__.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/indexer_xmacro.h` & `mujoco-2.3.6/mujoco/indexer_xmacro.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/indexers.cc` & `mujoco-2.3.6/mujoco/indexers.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/indexers.h` & `mujoco-2.3.6/mujoco/indexers.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/mjdata_meta.h` & `mujoco-2.3.6/mujoco/mjdata_meta.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/mjpython/Info.plist` & `mujoco-2.3.6/mujoco/mjpython/Info.plist`

 * *Files 11% similar despite different names*

#### Comparing `mujoco-2.3.5/mujoco/mjpython/Info.plist` & `mujoco-2.3.6/mujoco/mjpython/Info.plist`

```diff
@@ -5,21 +5,21 @@
 <plist version="1.0">
   <dict>
     <key>CFBundleName</key>
     <string>mjpython</string>
     <key>CFBundleIdentifier</key>
     <string>org.mujoco.mjpython</string>
     <key>CFBundleVersion</key>
-    <string>2.3.5</string>
+    <string>2.3.6</string>
     <key>CFBundleGetInfoString</key>
-    <string>2.3.5</string>
+    <string>2.3.6</string>
     <key>CFBundleLongVersionString</key>
-    <string>2.3.5</string>
+    <string>2.3.6</string>
     <key>CFBundleShortVersionString</key>
-    <string>2.3.5</string>
+    <string>2.3.6</string>
     <key>CFBundleExecutable</key>
     <string>mjpython</string>
     <key>CFBundleIconFile</key>
     <string>mjpython.icns</string>
     <key>CFBundlePackageType</key>
     <string>APPL</string>
     <key>NSHumanReadableCopyright</key>
```

### Comparing `mujoco-2.3.5/mujoco/mjpython/mjpython.icns` & `mujoco-2.3.6/mujoco/mjpython/mjpython.icns`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/mjpython/mjpython.mm` & `mujoco-2.3.6/mujoco/mjpython/mjpython.mm`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/mjpython/mjpython.py` & `mujoco-2.3.6/mujoco/mjpython/mjpython.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/osmesa/__init__.py` & `mujoco-2.3.6/mujoco/osmesa/__init__.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/raw.h` & `mujoco-2.3.6/mujoco/raw.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/render.cc` & `mujoco-2.3.6/mujoco/render.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/render_test.py` & `mujoco-2.3.6/mujoco/render_test.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/renderer.py` & `mujoco-2.3.6/mujoco/renderer.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/renderer_test.py` & `mujoco-2.3.6/mujoco/renderer_test.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/rollout.cc` & `mujoco-2.3.6/mujoco/rollout.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/rollout.py` & `mujoco-2.3.6/mujoco/rollout.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/rollout_test.py` & `mujoco-2.3.6/mujoco/rollout_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,16 +365,16 @@
     model = mujoco.MjModel.from_xml_string(TEST_XML)
     data = mujoco.MjData(model)
 
     initial_state = np.zeros(model.nq + model.nv + model.na)
     ctrl = np.zeros((3, model.nu))
 
     model.opt.solver = 10  # invalid solver type
-    with self.assertRaisesWithLiteralMatch(mujoco.FatalError,
-                                           'Unknown solver type 10'):
+    with self.assertRaisesWithLiteralMatch(
+        mujoco.FatalError, 'mj_fwdConstraint: unknown solver type 10'):
       state, sensordata = rollout.rollout(model, data, initial_state, ctrl)
 
   def test_invalid(self):
     model = mujoco.MjModel.from_xml_string(TEST_XML)
     data = mujoco.MjData(model)
 
     initial_state = np.zeros(model.nq + model.nv + model.na)
```

### Comparing `mujoco-2.3.5/mujoco/serialization.h` & `mujoco-2.3.6/mujoco/serialization.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/simulate/CMakeLists.txt` & `mujoco-2.3.6/mujoco/simulate/CMakeLists.txt`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 set(MUJOCO_DEP_VERSION_lodepng
     b4ed2cd7ecf61d29076169b49199371456d4f90b
     CACHE STRING "Version of `lodepng` to be fetched."
 )
 
 project(
   mujoco_simulate
-  VERSION 2.3.5
+  VERSION 2.3.6
   DESCRIPTION "MuJoCo simulate binaries"
   HOMEPAGE_URL "https://mujoco.org"
 )
 
 enable_language(C)
 enable_language(CXX)
 if(APPLE)
```

### Comparing `mujoco-2.3.5/mujoco/simulate/array_safety.h` & `mujoco-2.3.6/mujoco/simulate/array_safety.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/simulate/cmake/SimulateDependencies.cmake` & `mujoco-2.3.6/mujoco/simulate/cmake/SimulateDependencies.cmake`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/simulate/cmake/SimulateOptions.cmake` & `mujoco-2.3.6/mujoco/simulate/cmake/SimulateOptions.cmake`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/simulate/glfw_adapter.cc` & `mujoco-2.3.6/mujoco/simulate/glfw_adapter.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/simulate/glfw_adapter.h` & `mujoco-2.3.6/mujoco/simulate/glfw_adapter.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/simulate/glfw_corevideo.h` & `mujoco-2.3.6/mujoco/simulate/glfw_corevideo.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/simulate/glfw_corevideo.mm` & `mujoco-2.3.6/mujoco/simulate/glfw_corevideo.mm`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/simulate/glfw_dispatch.cc` & `mujoco-2.3.6/mujoco/simulate/glfw_dispatch.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/simulate/glfw_dispatch.h` & `mujoco-2.3.6/mujoco/simulate/glfw_dispatch.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/simulate/macos_gui.mm` & `mujoco-2.3.6/mujoco/simulate/macos_gui.mm`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/simulate/main.cc` & `mujoco-2.3.6/mujoco/simulate/main.cc`

 * *Files 0% similar despite different names*

```diff
@@ -219,15 +219,15 @@
       !std::strncmp(filename + mju::strlen_arr(filename) - 4, ".mjb",
                     mju::sizeof_arr(filename) - mju::strlen_arr(filename)+4)) {
     mnew = mj_loadModel(filename, nullptr);
     if (!mnew) {
       mju::strcpy_arr(loadError, "could not load binary model");
     }
   } else {
-    mnew = mj_loadXML(filename, nullptr, loadError, mj::Simulate::kMaxFilenameLength);
+    mnew = mj_loadXML(filename, nullptr, loadError, kErrorLength);
     // remove trailing newline character from loadError
     if (loadError[0]) {
       int error_length = mju::strlen_arr(loadError);
       if (loadError[error_length-1] == '\n') {
         loadError[error_length-1] = '\0';
       }
     }
```

### Comparing `mujoco-2.3.5/mujoco/simulate/platform_ui_adapter.cc` & `mujoco-2.3.6/mujoco/simulate/platform_ui_adapter.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/simulate/platform_ui_adapter.h` & `mujoco-2.3.6/mujoco/simulate/platform_ui_adapter.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/simulate/simulate.cc` & `mujoco-2.3.6/mujoco/simulate/simulate.cc`

 * *Files 4% similar despite different names*

```diff
@@ -98,14 +98,15 @@
   // left ui
   SECT_FILE   = 0,
   SECT_OPTION,
   SECT_SIMULATION,
   SECT_WATCH,
   SECT_PHYSICS,
   SECT_RENDERING,
+  SECT_VISUALIZATION,
   SECT_GROUP,
   NSECT0,
 
   // right ui
   SECT_JOINT = 0,
   SECT_CONTROL,
   NSECT1
@@ -561,15 +562,15 @@
   MJDATA_POINTERS_PREAMBLE(m);
 
   // find specified field in mjData arrays, update value
   #define X(TYPE, NAME, NR, NC)                                                                  \
     if (!mju::strcmp_arr(#NAME, sim->field) &&                                                   \
         !mju::strcmp_arr(#TYPE, "mjtNum")) {                                                     \
       if (sim->index >= 0 && sim->index < m->NR * NC) {                                          \
-        PrintField(sim->ui0.sect[SECT_WATCH].item[2].multi.name[0],d->NAME + sim->index);        \
+        PrintField(sim->ui0.sect[SECT_WATCH].item[2].multi.name[0], d->NAME + sim->index);       \
       } else {                                                                                   \
         mju::strcpy_arr(sim->ui0.sect[SECT_WATCH].item[2].multi.name[0], "invalid index");       \
       }                                                                                          \
       return;                                                                                    \
     }
 
   MJDATA_POINTERS
@@ -725,52 +726,111 @@
   mjuiDef defFlag[] = {
     {mjITEM_CHECKBYTE,  "", 2, nullptr, ""},
     {mjITEM_END}
   };
   for (int i=0; i<mjNVISFLAG; i++) {
     // set name, remove "&"
     mju::strcpy_arr(defFlag[0].name, mjVISSTRING[i][0]);
-    for (int j=0; j<strlen(mjVISSTRING[i][0]); j++)
+    for (int j=0; j<strlen(mjVISSTRING[i][0]); j++) {
       if (mjVISSTRING[i][0][j]=='&') {
         mju_strncpy(
           defFlag[0].name+j, mjVISSTRING[i][0]+j+1, mju::sizeof_arr(defFlag[0].name)-j);
         break;
       }
+    }
 
     // set shortcut and data
     if (mjVISSTRING[i][2][0]) {
       mju::sprintf_arr(defFlag[0].other, " %s", mjVISSTRING[i][2]);
     } else {
       mju::sprintf_arr(defFlag[0].other, "");
     }
     defFlag[0].pdata = sim->opt.flags + i;
     mjui_add(&sim->ui0, defFlag);
   }
 
   // create tree slider
   mjuiDef defTree[] = {
-      {mjITEM_SLIDERINT, "Tree depth", 2, &sim->opt.bvh_depth, "-1 15"},
+      {mjITEM_SLIDERINT, "Tree depth", 2, &sim->opt.bvh_depth, "0 15"},
       {mjITEM_END}
   };
   mjui_add(&sim->ui0, defTree);
 
+  // add rendering flags
   mjui_add(&sim->ui0, defOpenGL);
   for (int i=0; i<mjNRNDFLAG; i++) {
     mju::strcpy_arr(defFlag[0].name, mjRNDSTRING[i][0]);
     if (mjRNDSTRING[i][2][0]) {
       mju::sprintf_arr(defFlag[0].other, " %s", mjRNDSTRING[i][2]);
     } else {
       mju::sprintf_arr(defFlag[0].other, "");
     }
     defFlag[0].pdata = sim->scn.flags + i;
     mjui_add(&sim->ui0, defFlag);
   }
 }
 
+// make visualization section of UI
+void MakeVisualizationSection(mj::Simulate* sim, const mjModel* m, int oldstate) {
+  mjStatistic* stat = sim->fully_managed_ ? &sim->m_->stat : &sim->scnstate_.model.stat;
+  mjVisual* vis = sim->fully_managed_ ? &sim->m_->vis : &sim->scnstate_.model.vis;
+
+  mjuiDef defVisualization[] = {
+    {mjITEM_SECTION,   "Visualization", oldstate, nullptr, "AV"},
+    {mjITEM_SEPARATOR, "Headlight",  1},
+    {mjITEM_RADIO,     "Active",          5, &(vis->headlight.active),     "Off\nOn"},
+    {mjITEM_EDITFLOAT, "Ambient",         2, &(vis->headlight.ambient),    "3"},
+    {mjITEM_EDITFLOAT, "Diffuse",         2, &(vis->headlight.diffuse),    "3"},
+    {mjITEM_EDITFLOAT, "Specular",        2, &(vis->headlight.specular),   "3"},
+    {mjITEM_SEPARATOR, "Initial Free Camera",  1},
+    {mjITEM_EDITNUM,   "Center",          2, &(stat->center),              "3"},
+    {mjITEM_EDITFLOAT, "Azimuth",         2, &(vis->global.azimuth),       "1"},
+    {mjITEM_EDITFLOAT, "Elevation",       2, &(vis->global.elevation),     "1"},
+    {mjITEM_BUTTON,    "Align",           2, nullptr,                      "CA"},
+    {mjITEM_SEPARATOR, "Global",  1},
+    {mjITEM_EDITNUM,   "Extent",          2, &(stat->extent),              "1"},
+    {mjITEM_EDITFLOAT, "Field of view",   2, &(vis->global.fovy),          "1"},
+    {mjITEM_RADIO,     "Inertia",         5, &(vis->global.ellipsoidinertia), "Box\nEllipsoid"},
+    {mjITEM_SEPARATOR, "Map",  1},
+    {mjITEM_EDITFLOAT, "Stiffness",       2, &(vis->map.stiffness),        "1"},
+    {mjITEM_EDITFLOAT, "Rot stiffness",   2, &(vis->map.stiffnessrot),     "1"},
+    {mjITEM_EDITFLOAT, "Force",           2, &(vis->map.force),            "1"},
+    {mjITEM_EDITFLOAT, "Torque",          2, &(vis->map.torque),           "1"},
+    {mjITEM_EDITFLOAT, "Alpha",           2, &(vis->map.alpha),            "1"},
+    {mjITEM_EDITFLOAT, "Fog start",       2, &(vis->map.fogstart),         "1"},
+    {mjITEM_EDITFLOAT, "Fog end",         2, &(vis->map.fogend),           "1"},
+    {mjITEM_EDITFLOAT, "Z near",          2, &(vis->map.znear),            "1"},
+    {mjITEM_EDITFLOAT, "Z far",           2, &(vis->map.zfar),             "1"},
+    {mjITEM_EDITFLOAT, "Haze",            2, &(vis->map.haze),             "1"},
+    {mjITEM_EDITFLOAT, "Shadow clip",     2, &(vis->map.shadowclip),       "1"},
+    {mjITEM_EDITFLOAT, "Shadow scale",    2, &(vis->map.shadowscale),      "1"},
+    {mjITEM_SEPARATOR, "Scale",  1},
+    {mjITEM_EDITNUM,   "All [meansize]",  2, &(stat->meansize),            "1"},
+    {mjITEM_EDITFLOAT, "Force width",     2, &(vis->scale.forcewidth),     "1"},
+    {mjITEM_EDITFLOAT, "Contact width",   2, &(vis->scale.contactwidth),   "1"},
+    {mjITEM_EDITFLOAT, "Contact height",  2, &(vis->scale.contactheight),  "1"},
+    {mjITEM_EDITFLOAT, "Connect",         2, &(vis->scale.connect),        "1"},
+    {mjITEM_EDITFLOAT, "Com",             2, &(vis->scale.com),            "1"},
+    {mjITEM_EDITFLOAT, "Camera",          2, &(vis->scale.camera),         "1"},
+    {mjITEM_EDITFLOAT, "Light",           2, &(vis->scale.light),          "1"},
+    {mjITEM_EDITFLOAT, "Select point",    2, &(vis->scale.selectpoint),    "1"},
+    {mjITEM_EDITFLOAT, "Joint length",    2, &(vis->scale.jointlength),    "1"},
+    {mjITEM_EDITFLOAT, "Joint width",     2, &(vis->scale.jointwidth),     "1"},
+    {mjITEM_EDITFLOAT, "Actuator length", 2, &(vis->scale.actuatorlength), "1"},
+    {mjITEM_EDITFLOAT, "Actuator width",  2, &(vis->scale.actuatorwidth),  "1"},
+    {mjITEM_EDITFLOAT, "Frame length",    2, &(vis->scale.framelength),    "1"},
+    {mjITEM_EDITFLOAT, "Frame width",     2, &(vis->scale.framewidth),     "1"},
+    {mjITEM_EDITFLOAT, "Constraint",      2, &(vis->scale.constraint),     "1"},
+    {mjITEM_EDITFLOAT, "Slider-crank",    2, &(vis->scale.slidercrank),    "1"},
+    {mjITEM_END}
+  };
 
+  // add rendering standard
+  mjui_add(&sim->ui0, defVisualization);
+}
 
 // make group section of UI
 void MakeGroupSection(mj::Simulate* sim, int oldstate) {
   mjuiDef defGroup[] = {
     {mjITEM_SECTION,    "Group enable",     oldstate, nullptr,          "AG"},
     {mjITEM_SEPARATOR,  "Geom groups",  1},
     {mjITEM_CHECKBYTE,  "Geom 0",           2, sim->opt.geomgroup,          " 0"},
@@ -946,14 +1006,15 @@
   // clear model-dependent sections of UI
   sim->ui0.nsect = SECT_PHYSICS;
   sim->ui1.nsect = 0;
 
   // make
   MakePhysicsSection(sim, oldstate0[SECT_PHYSICS]);
   MakeRenderingSection(sim, m, oldstate0[SECT_RENDERING]);
+  MakeVisualizationSection(sim, m, oldstate0[SECT_VISUALIZATION]);
   MakeGroupSection(sim, oldstate0[SECT_GROUP]);
   MakeJointSection(sim, oldstate1[SECT_JOINT]);
   MakeControlSection(sim, oldstate1[SECT_CONTROL]);
 }
 
 //---------------------------------- utility functions ---------------------------------------------
 
@@ -1278,14 +1339,21 @@
       }
       // copy camera spec to clipboard (as MJCF element)
       if (it->itemid == 3) {
         CopyCamera(sim);
       }
     }
 
+    // visualization section
+    else if (it && it->sectionid==SECT_VISUALIZATION) {
+      if (!mju::strcmp_arr(it->name, "Align")) {
+        sim->pending_.align = true;
+      }
+    }
+
     // group section
     else if (it && it->sectionid==SECT_GROUP) {
       // remake joint section if joint group changed
       if (it->name[0]=='J' && it->name[1]=='o') {
         sim->ui1.nsect = SECT_JOINT;
         MakeJointSection(sim, sim->ui1.sect[SECT_JOINT].state);
         sim->ui1.nsect = NSECT1;
```

### Comparing `mujoco-2.3.5/mujoco/simulate/simulate.h` & `mujoco-2.3.6/mujoco/simulate/simulate.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/simulate.cc` & `mujoco-2.3.6/mujoco/simulate.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/structs.cc` & `mujoco-2.3.6/mujoco/structs.cc`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 #include <absl/container/flat_hash_map.h>
 #include <mujoco/mjxmacro.h>
 #include <mujoco/mujoco.h>
 #include "errors.h"
 #include "function_traits.h"
 #include "indexers.h"
 #include "mjdata_meta.h"
+#include "private.h"
 #include "raw.h"
 #include "serialization.h"
 #include <pybind11/numpy.h>
 #include <pybind11/operators.h>
 #include <pybind11/pybind11.h>
 #include <pybind11/pytypes.h>
 #include <pybind11/stl.h>
@@ -481,23 +482,25 @@
 #define X(var) var(InitPyArray(ptr_->var, owner_))
 MjContactWrapper::MjWrapper()
     : WrapperBase(new raw::MjContact{}),
       X(pos),
       X(frame),
       X(friction),
       X(solref),
+      X(solreffriction),
       X(solimp),
       X(H) {}
 
 MjContactWrapper::MjWrapper(raw::MjContact* ptr, py::handle owner)
     : WrapperBase(ptr, owner),
       X(pos),
       X(frame),
       X(friction),
       X(solref),
+      X(solreffriction),
       X(solimp),
       X(H) {}
 #undef X
 
 MjContactWrapper::MjWrapper(const MjContactWrapper& other)
     : MjContactWrapper() {
   *this->ptr_ = *other.ptr_;
@@ -691,15 +694,14 @@
              this->metadata_.n * sizeof(dtype));
 
   MJDATA_METADATA
 #undef X
 
   // Write struct and scalar fields
 #define X(var) WriteBytes(output, &ptr_->var, sizeof(ptr_->var))
-  X(parena);
   X(maxuse_stack);
   X(maxuse_arena);
   X(maxuse_con);
   X(maxuse_efc);
   X(solver);
   X(timer);
   X(warning);
@@ -723,15 +725,14 @@
 
 #undef MJ_M
 #define MJ_M(x) this->metadata_.x
 #undef MJ_D
 #define MJ_D(x) this->ptr_->x
 #define X(type, name, nr, nc)                                   \
   if ((nr) * (nc)) {                                            \
-    WriteInt(output, PTRDIFF(ptr_->name, ptr_->arena));         \
     WriteBytes(output, ptr_->name, sizeof(type) * (nr) * (nc)); \
   }
 
     MJDATA_ARENA_POINTERS_CONTACT
     MJDATA_ARENA_POINTERS_PRIMAL
 
     if (this->metadata_.is_dual) {
@@ -782,15 +783,14 @@
   }
 
   // Read structs and scalar fields
 #define X(var)                                       \
   ReadBytes(input, (void*) &d->var, sizeof(d->var)); \
   CheckInput(input, "mjData");
 
-  X(parena);
   X(maxuse_stack);
   X(maxuse_arena);
   X(maxuse_con);
   X(maxuse_efc);
   X(solver);
   X(timer);
   X(warning);
@@ -812,19 +812,19 @@
     MJDATA_POINTERS
 #undef X
 
 #undef MJ_M
 #define MJ_M(x) m.x
 #undef MJ_D
 #define MJ_D(x) d->x
-#define X(type, name, nr, nc)                              \
-  if ((nr) * (nc)) {                                       \
-    d->name = reinterpret_cast<decltype(d->name)>(         \
-        static_cast<char*>(d->arena) + ReadInt(input));    \
-    ReadBytes(input, d->name, sizeof(type) * (nr) * (nc)); \
+#define X(type, name, nr, nc)                                          \
+  if ((nr) * (nc)) {                                                   \
+    d->name = static_cast<decltype(d->name)>(                          \
+        mj_arenaAlloc(d, sizeof(type) * (nr) * (nc), alignof(type)));  \
+    ReadBytes(input, d->name, sizeof(type) * (nr) * (nc));             \
   }
 
     MJDATA_ARENA_POINTERS_CONTACT
     MJDATA_ARENA_POINTERS_PRIMAL
 
     if (metadata.is_dual) {
       MJDATA_ARENA_POINTERS_DUAL
@@ -1733,14 +1733,15 @@
 #undef X
 
 #define X(var) DefinePyArray(mjContact, #var, &MjContactWrapper::var)
   X(pos);
   X(frame);
   X(friction);
   X(solref);
+  X(solreffriction);
   X(solimp);
   X(H);
 #undef X
 
   py::class_<MjContactList> mjContactList(m, "_MjContactList");
   mjContactList.def("__getitem__", &MjContactList::operator[],
                     py::return_value_policy::reference);
@@ -1764,14 +1765,15 @@
   });
   X(mjtNum, dist);
   XN(mjtNum, pos);
   XN(mjtNum, frame);
   X(mjtNum, includemargin);
   XN(mjtNum, friction);
   XN(mjtNum, solref);
+  XN(mjtNum, solreffriction);
   XN(mjtNum, solimp);
   X(mjtNum, mu);
   XN(mjtNum, H);
   X(int, dim);
   X(int, geom1);
   X(int, geom2);
   X(int, exclude);
```

### Comparing `mujoco-2.3.5/mujoco/structs.h` & `mujoco-2.3.6/mujoco/structs.h`

 * *Files 1% similar despite different names*

```diff
@@ -499,14 +499,15 @@
   ~MjWrapper() = default;
 
   #define X(var) py_array_or_tuple_t<mjtNum> var
   X(pos);
   X(frame);
   X(friction);
   X(solref);
+  X(solreffriction);
   X(solimp);
   X(H);
   #undef X
 };
 
 using MjContactWrapper = MjWrapper<raw::MjContact>;
```

### Comparing `mujoco-2.3.5/mujoco/util/CMakeLists.txt` & `mujoco-2.3.6/mujoco/util/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/util/array_traits.h` & `mujoco-2.3.6/mujoco/util/array_traits.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/util/array_traits_test.cc` & `mujoco-2.3.6/mujoco/util/array_traits_test.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/util/crossplatform.h` & `mujoco-2.3.6/mujoco/util/crossplatform.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/util/func_traits.h` & `mujoco-2.3.6/mujoco/util/func_traits.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/util/func_traits_test.cc` & `mujoco-2.3.6/mujoco/util/func_traits_test.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/util/func_wrap.h` & `mujoco-2.3.6/mujoco/util/func_wrap.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/util/func_wrap_test.cc` & `mujoco-2.3.6/mujoco/util/func_wrap_test.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/util/tuple_tools.h` & `mujoco-2.3.6/mujoco/util/tuple_tools.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/util/tuple_tools_test.cc` & `mujoco-2.3.6/mujoco/util/tuple_tools_test.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/viewer.py` & `mujoco-2.3.6/mujoco/viewer.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco/viewer_test.py` & `mujoco-2.3.6/mujoco/viewer_test.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.5/mujoco.egg-info/PKG-INFO` & `mujoco-2.3.6/mujoco.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mujoco
-Version: 2.3.5
+Version: 2.3.6
 Summary: MuJoCo Physics Simulator
 Home-page: https://github.com/deepmind/mujoco
-Author: DeepMind
+Author: Google DeepMind
 Author-email: mujoco@deepmind.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
@@ -30,16 +30,16 @@
 
 [pypi-versions-badge]: https://img.shields.io/pypi/pyversions/mujoco
 [pypi-badge]: https://badge.fury.io/py/mujoco.svg
 [pypi]: https://pypi.org/project/mujoco/
 
 This package is the canonical Python bindings for the
 [MuJoCo physics engine](https://github.com/deepmind/mujoco).
-These bindings are developed and maintained by DeepMind, and is kept up-to-date
-with the latest developments in MuJoCo itself.
+These bindings are developed and maintained by Google DeepMind, and is kept
+up-to-date with the latest developments in MuJoCo itself.
 
 The `mujoco` package provides direct access to raw MuJoCo C API functions,
 structs, constants, and enumerations. Structs are provided as Python classes,
 with Pythonic initialization and deletion semantics.
 
 It is not the aim of this package to provide fully fledged
 scene/environment/game authoring API, as there are already a number of existing
```

### Comparing `mujoco-2.3.5/mujoco.egg-info/SOURCES.txt` & `mujoco-2.3.6/mujoco.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 mujoco/functions.cc
 mujoco/functions.h
 mujoco/gl_context.py
 mujoco/indexer_xmacro.h
 mujoco/indexers.cc
 mujoco/indexers.h
 mujoco/mjdata_meta.h
+mujoco/private.h
 mujoco/raw.h
 mujoco/render.cc
 mujoco/render_test.py
 mujoco/renderer.py
 mujoco/renderer_test.py
 mujoco/rollout.cc
 mujoco/rollout.py
```

### Comparing `mujoco-2.3.5/setup.py` & `mujoco-2.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 import setuptools
 from setuptools import find_packages
 from setuptools import setup
 from setuptools.command import build_ext
 from setuptools.command import install_scripts
 
-__version__ = '2.3.5'
+__version__ = '2.3.6'
 
 MUJOCO_CMAKE = 'MUJOCO_CMAKE'
 MUJOCO_CMAKE_ARGS = 'MUJOCO_CMAKE_ARGS'
 MUJOCO_PATH = 'MUJOCO_PATH'
 MUJOCO_PLUGIN_PATH = 'MUJOCO_PLUGIN_PATH'
 
 EXT_PREFIX = 'mujoco.'
@@ -345,15 +345,15 @@
         relative_dirpath = os.path.relpath(directory, package_dir)
         paths.add(os.path.join(relative_dirpath, filename))
   return list(paths)
 
 SETUP_KWARGS = dict(
     name='mujoco',
     version=__version__,
-    author='DeepMind',
+    author='Google DeepMind',
     author_email='mujoco@deepmind.com',
     description='MuJoCo Physics Simulator',
     long_description=get_long_description(),
     long_description_content_type='text/markdown',
     url='https://github.com/deepmind/mujoco',
     license='Apache License 2.0',
     classifiers=[
```

