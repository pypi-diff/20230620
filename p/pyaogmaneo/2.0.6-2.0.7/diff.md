# Comparing `tmp/pyaogmaneo-2.0.6.tar.gz` & `tmp/pyaogmaneo-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaogmaneo-2.0.6.tar", last modified: Wed Jun 14 18:13:00 2023, max compression
+gzip compressed data, was "pyaogmaneo-2.0.7.tar", last modified: Tue Jun 20 19:27:40 2023, max compression
```

## Comparing `pyaogmaneo-2.0.6.tar` & `pyaogmaneo-2.0.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-06-14 18:13:00.520846 pyaogmaneo-2.0.6/
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-06-14 18:13:00.520846 pyaogmaneo-2.0.6/CMake/
--rw-r--r--   0 ericl     (1000) ericl     (1001)     1250 2023-03-18 01:02:16.000000 pyaogmaneo-2.0.6/CMake/FindAOgmaNeo.cmake
--rw-r--r--   0 ericl     (1000) ericl     (1001)     2620 2023-06-14 18:10:02.000000 pyaogmaneo-2.0.6/CMakeLists.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)    17842 2022-12-03 02:07:03.000000 pyaogmaneo-2.0.6/LICENSE.md
--rw-r--r--   0 ericl     (1000) ericl     (1001)       64 2022-12-03 02:07:03.000000 pyaogmaneo-2.0.6/MANIFEST.in
--rw-r--r--   0 ericl     (1000) ericl     (1001)      785 2023-06-14 18:13:00.520846 pyaogmaneo-2.0.6/PKG-INFO
--rw-r--r--   0 ericl     (1000) ericl     (1001)     2412 2023-05-18 17:15:10.000000 pyaogmaneo-2.0.6/README.md
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-06-14 18:13:00.520846 pyaogmaneo-2.0.6/pyaogmaneo.egg-info/
--rw-r--r--   0 ericl     (1000) ericl     (1001)      785 2023-06-14 18:13:00.000000 pyaogmaneo-2.0.6/pyaogmaneo.egg-info/PKG-INFO
--rw-r--r--   0 ericl     (1000) ericl     (1001)      505 2023-06-14 18:13:00.000000 pyaogmaneo-2.0.6/pyaogmaneo.egg-info/SOURCES.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)        1 2023-06-14 18:13:00.000000 pyaogmaneo-2.0.6/pyaogmaneo.egg-info/dependency_links.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)        1 2022-12-03 02:07:23.000000 pyaogmaneo-2.0.6/pyaogmaneo.egg-info/not-zip-safe
--rw-r--r--   0 ericl     (1000) ericl     (1001)       11 2023-06-14 18:13:00.000000 pyaogmaneo-2.0.6/pyaogmaneo.egg-info/top_level.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)      101 2023-01-13 01:36:37.000000 pyaogmaneo-2.0.6/pyproject.toml
--rw-r--r--   0 ericl     (1000) ericl     (1001)       38 2023-06-14 18:13:00.520846 pyaogmaneo-2.0.6/setup.cfg
--rw-r--r--   0 ericl     (1000) ericl     (1001)     4204 2023-06-14 18:10:12.000000 pyaogmaneo-2.0.6/setup.py
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-06-14 18:13:00.520846 pyaogmaneo-2.0.6/source/
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-06-14 18:13:00.520846 pyaogmaneo-2.0.6/source/pyaogmaneo/
--rw-r--r--   0 ericl     (1000) ericl     (1001)     1071 2023-06-09 23:28:26.000000 pyaogmaneo-2.0.6/source/pyaogmaneo/py_helpers.cpp
--rw-r--r--   0 ericl     (1000) ericl     (1001)     1783 2023-06-09 23:43:55.000000 pyaogmaneo-2.0.6/source/pyaogmaneo/py_helpers.h
--rw-r--r--   0 ericl     (1000) ericl     (1001)    15208 2023-06-12 02:04:51.000000 pyaogmaneo-2.0.6/source/pyaogmaneo/py_hierarchy.cpp
--rw-r--r--   0 ericl     (1000) ericl     (1001)     6938 2023-06-12 22:02:24.000000 pyaogmaneo-2.0.6/source/pyaogmaneo/py_hierarchy.h
--rw-r--r--   0 ericl     (1000) ericl     (1001)     8183 2023-06-12 01:45:03.000000 pyaogmaneo-2.0.6/source/pyaogmaneo/py_image_encoder.cpp
--rw-r--r--   0 ericl     (1000) ericl     (1001)     3217 2023-06-12 22:02:33.000000 pyaogmaneo-2.0.6/source/pyaogmaneo/py_image_encoder.h
--rw-r--r--   0 ericl     (1000) ericl     (1001)     8963 2023-06-12 01:45:03.000000 pyaogmaneo-2.0.6/source/pyaogmaneo/py_module.cpp
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-06-20 19:27:40.737136 pyaogmaneo-2.0.7/
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-06-20 19:27:40.737136 pyaogmaneo-2.0.7/CMake/
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     1250 2023-03-18 01:02:16.000000 pyaogmaneo-2.0.7/CMake/FindAOgmaNeo.cmake
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     2620 2023-06-20 19:25:57.000000 pyaogmaneo-2.0.7/CMakeLists.txt
+-rw-r--r--   0 ericl     (1000) ericl     (1001)    17842 2022-12-03 02:07:03.000000 pyaogmaneo-2.0.7/LICENSE.md
+-rw-r--r--   0 ericl     (1000) ericl     (1001)       64 2022-12-03 02:07:03.000000 pyaogmaneo-2.0.7/MANIFEST.in
+-rw-r--r--   0 ericl     (1000) ericl     (1001)      785 2023-06-20 19:27:40.737136 pyaogmaneo-2.0.7/PKG-INFO
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     2412 2023-05-18 17:15:10.000000 pyaogmaneo-2.0.7/README.md
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-06-20 19:27:40.737136 pyaogmaneo-2.0.7/pyaogmaneo.egg-info/
+-rw-r--r--   0 ericl     (1000) ericl     (1001)      785 2023-06-20 19:27:40.000000 pyaogmaneo-2.0.7/pyaogmaneo.egg-info/PKG-INFO
+-rw-r--r--   0 ericl     (1000) ericl     (1001)      505 2023-06-20 19:27:40.000000 pyaogmaneo-2.0.7/pyaogmaneo.egg-info/SOURCES.txt
+-rw-r--r--   0 ericl     (1000) ericl     (1001)        1 2023-06-20 19:27:40.000000 pyaogmaneo-2.0.7/pyaogmaneo.egg-info/dependency_links.txt
+-rw-r--r--   0 ericl     (1000) ericl     (1001)        1 2022-12-03 02:07:23.000000 pyaogmaneo-2.0.7/pyaogmaneo.egg-info/not-zip-safe
+-rw-r--r--   0 ericl     (1000) ericl     (1001)       11 2023-06-20 19:27:40.000000 pyaogmaneo-2.0.7/pyaogmaneo.egg-info/top_level.txt
+-rw-r--r--   0 ericl     (1000) ericl     (1001)      101 2023-01-13 01:36:37.000000 pyaogmaneo-2.0.7/pyproject.toml
+-rw-r--r--   0 ericl     (1000) ericl     (1001)       38 2023-06-20 19:27:40.737136 pyaogmaneo-2.0.7/setup.cfg
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     4204 2023-06-20 19:26:10.000000 pyaogmaneo-2.0.7/setup.py
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-06-20 19:27:40.737136 pyaogmaneo-2.0.7/source/
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-06-20 19:27:40.737136 pyaogmaneo-2.0.7/source/pyaogmaneo/
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     1071 2023-06-09 23:28:26.000000 pyaogmaneo-2.0.7/source/pyaogmaneo/py_helpers.cpp
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     1783 2023-06-09 23:43:55.000000 pyaogmaneo-2.0.7/source/pyaogmaneo/py_helpers.h
+-rw-r--r--   0 ericl     (1000) ericl     (1001)    15208 2023-06-20 18:21:44.000000 pyaogmaneo-2.0.7/source/pyaogmaneo/py_hierarchy.cpp
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     6938 2023-06-20 18:21:44.000000 pyaogmaneo-2.0.7/source/pyaogmaneo/py_hierarchy.h
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     8183 2023-06-20 18:12:37.000000 pyaogmaneo-2.0.7/source/pyaogmaneo/py_image_encoder.cpp
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     3217 2023-06-20 18:21:44.000000 pyaogmaneo-2.0.7/source/pyaogmaneo/py_image_encoder.h
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     8969 2023-06-20 18:42:29.000000 pyaogmaneo-2.0.7/source/pyaogmaneo/py_module.cpp
```

### Comparing `pyaogmaneo-2.0.6/CMake/FindAOgmaNeo.cmake` & `pyaogmaneo-2.0.7/CMake/FindAOgmaNeo.cmake`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.6/CMakeLists.txt` & `pyaogmaneo-2.0.7/CMakeLists.txt`

 * *Files 9% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     find_package(AOgmaNeo)
 else()
     message(STATUS "Not using system installation of AOgmaNeo, will download from repository")
 
     FetchContent_Declare(
         AOgmaNeo
         GIT_REPOSITORY https://github.com/ogmacorp/AOgmaNeo.git
-        GIT_TAG ade5d3b08d2d2897a38dc010bb911f5f46af3929
+        GIT_TAG 97fd2822c76ba756acf79f0918c6d13b89f9bbe4
     )
 
     FetchContent_GetProperties(AOgmaNeo)
 
     if(NOT AOgmaNeo_POPULATED)
         FetchContent_Populate(AOgmaNeo)
         add_subdirectory(${aogmaneo_SOURCE_DIR} ${aogmaneo_BINARY_DIR})
```

### Comparing `pyaogmaneo-2.0.6/LICENSE.md` & `pyaogmaneo-2.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.6/PKG-INFO` & `pyaogmaneo-2.0.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaogmaneo
-Version: 2.0.6
+Version: 2.0.7
 Summary: Python bindings for the AOgmaNeo library
 Home-page: https://ogmacorp.com/
 Author: Ogma Intelligent Systems Corp
 Author-email: info@ogmacorp.com
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `pyaogmaneo-2.0.6/README.md` & `pyaogmaneo-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.6/pyaogmaneo.egg-info/PKG-INFO` & `pyaogmaneo-2.0.7/pyaogmaneo.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaogmaneo
-Version: 2.0.6
+Version: 2.0.7
 Summary: Python bindings for the AOgmaNeo library
 Home-page: https://ogmacorp.com/
 Author: Ogma Intelligent Systems Corp
 Author-email: info@ogmacorp.com
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `pyaogmaneo-2.0.6/setup.py` & `pyaogmaneo-2.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             os.makedirs(self.build_temp)
 
         subprocess.check_call([ 'cmake', ext.sourcedir ] + cmake_args, cwd=self.build_temp, env=env)
         subprocess.check_call([ 'cmake', '--build', '.' ] + build_args, cwd=self.build_temp)
 
 setup(
     name="pyaogmaneo",
-    version="2.0.6",
+    version="2.0.7",
     description="Python bindings for the AOgmaNeo library",
     long_description='https://github.com/ogmacorp/PyAOgmaNeo',
     author='Ogma Intelligent Systems Corp',
     author_email='info@ogmacorp.com',
     url='https://ogmacorp.com/',
     license='Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License',
     classifiers=[
```

### Comparing `pyaogmaneo-2.0.6/source/pyaogmaneo/py_helpers.cpp` & `pyaogmaneo-2.0.7/source/pyaogmaneo/py_helpers.cpp`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.6/source/pyaogmaneo/py_helpers.h` & `pyaogmaneo-2.0.7/source/pyaogmaneo/py_helpers.h`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.6/source/pyaogmaneo/py_hierarchy.cpp` & `pyaogmaneo-2.0.7/source/pyaogmaneo/py_hierarchy.cpp`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.6/source/pyaogmaneo/py_hierarchy.h` & `pyaogmaneo-2.0.7/source/pyaogmaneo/py_hierarchy.h`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.6/source/pyaogmaneo/py_image_encoder.cpp` & `pyaogmaneo-2.0.7/source/pyaogmaneo/py_image_encoder.cpp`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.6/source/pyaogmaneo/py_image_encoder.h` & `pyaogmaneo-2.0.7/source/pyaogmaneo/py_image_encoder.h`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.0.6/source/pyaogmaneo/py_module.cpp` & `pyaogmaneo-2.0.7/source/pyaogmaneo/py_module.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -32,21 +32,21 @@
                 std::tuple<int, int, int>,
                 pyaon::IO_Type,
                 int,
                 int,
                 int
             >(),
             py::arg("size") = std::tuple<int, int, int>({ 4, 4, 16 }),
-            py::arg("type") = pyaon::prediction,
+            py::arg("io_type") = pyaon::prediction,
             py::arg("up_radius") = 2,
             py::arg("down_radius") = 2,
             py::arg("history_capacity") = 64
         )
         .def_readwrite("size", &pyaon::IO_Desc::size)
-        .def_readwrite("type", &pyaon::IO_Desc::type)
+        .def_readwrite("io_type", &pyaon::IO_Desc::type)
         .def_readwrite("up_radius", &pyaon::IO_Desc::up_radius)
         .def_readwrite("down_radius", &pyaon::IO_Desc::down_radius)
         .def_readwrite("history_capacity", &pyaon::IO_Desc::history_capacity);
 
     py::class_<pyaon::Layer_Desc>(m, "LayerDesc")
         .def(py::init<
                 std::tuple<int, int, int>,
@@ -74,15 +74,15 @@
         .def_readwrite("gcurve", &aon::Encoder::Params::gcurve);
 
     py::class_<aon::Decoder::Params>(m, "DecoderParams")
         .def(py::init<>())
         .def_readwrite("lr", &aon::Decoder::Params::lr)
         .def_readwrite("gcurve", &aon::Decoder::Params::gcurve);
 
-    py::class_<aon::Actor::Params>(m, "Actorparams")
+    py::class_<aon::Actor::Params>(m, "ActorParams")
         .def(py::init<>())
         .def_readwrite("vlr", &aon::Actor::Params::vlr)
         .def_readwrite("alr", &aon::Actor::Params::alr)
         .def_readwrite("bias", &aon::Actor::Params::bias)
         .def_readwrite("discount", &aon::Actor::Params::discount)
         .def_readwrite("temperature", &aon::Actor::Params::temperature)
         .def_readwrite("min_steps", &aon::Actor::Params::min_steps)
```

