# Comparing `tmp/configparserc-1.4.0.tar.gz` & `tmp/configparserc-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/configparserc-1.4.0.tar", last modified: Thu May 11 22:04:25 2023, max compression
+gzip compressed data, was "dist/configparserc-1.4.1.tar", last modified: Tue Jun 20 01:23:57 2023, max compression
```

## Comparing `configparserc-1.4.0.tar` & `configparserc-1.4.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 22:04:25.000000 configparserc-1.4.0/
--rw-rw-rw-   0 root         (0) root         (0)    11363 2023-05-11 22:03:49.000000 configparserc-1.4.0/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      187 2023-05-11 22:03:49.000000 configparserc-1.4.0/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)      642 2023-05-11 22:03:49.000000 configparserc-1.4.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5363 2023-05-11 22:04:25.000000 configparserc-1.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3746 2023-05-11 22:03:49.000000 configparserc-1.4.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 22:04:25.000000 configparserc-1.4.0/configparserc/
--rw-rw-rw-   0 root         (0) root         (0)      674 2023-05-11 22:03:49.000000 configparserc-1.4.0/configparserc/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1435996 2023-05-11 22:04:24.000000 configparserc-1.4.0/configparserc/config.c
--rw-rw-rw-   0 root         (0) root         (0)     3082 2023-05-11 22:03:49.000000 configparserc-1.4.0/configparserc/config.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 22:04:25.000000 configparserc-1.4.0/configparserc/include/
--rw-rw-rw-   0 root         (0) root         (0)      518 2023-05-11 22:03:49.000000 configparserc-1.4.0/configparserc/include/_config.h
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-05-11 22:03:49.000000 configparserc-1.4.0/configparserc/py.typed
--rw-r--r--   0 root         (0) root         (0)   341280 2023-05-11 22:04:21.000000 configparserc-1.4.0/configparserc/tools.c
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-05-11 22:03:49.000000 configparserc-1.4.0/configparserc/tools.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 22:04:25.000000 configparserc-1.4.0/configparserc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5363 2023-05-11 22:04:24.000000 configparserc-1.4.0/configparserc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      451 2023-05-11 22:04:24.000000 configparserc-1.4.0/configparserc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 22:04:24.000000 configparserc-1.4.0/configparserc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 22:04:24.000000 configparserc-1.4.0/configparserc.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-11 22:04:24.000000 configparserc-1.4.0/configparserc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-05-11 22:04:24.000000 configparserc-1.4.0/configparserc.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1406 2023-05-11 22:04:25.000000 configparserc-1.4.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)    14643 2023-05-11 22:03:49.000000 configparserc-1.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 01:23:57.000000 configparserc-1.4.1/
+-rw-rw-rw-   0 root         (0) root         (0)    11363 2023-06-20 01:23:42.000000 configparserc-1.4.1/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      187 2023-06-20 01:23:42.000000 configparserc-1.4.1/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)      642 2023-06-20 01:23:42.000000 configparserc-1.4.1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5363 2023-06-20 01:23:57.000000 configparserc-1.4.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3746 2023-06-20 01:23:42.000000 configparserc-1.4.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 01:23:57.000000 configparserc-1.4.1/configparserc/
+-rw-rw-rw-   0 root         (0) root         (0)      674 2023-06-20 01:23:42.000000 configparserc-1.4.1/configparserc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1437023 2023-06-20 01:23:57.000000 configparserc-1.4.1/configparserc/config.c
+-rw-rw-rw-   0 root         (0) root         (0)     3082 2023-06-20 01:23:42.000000 configparserc-1.4.1/configparserc/config.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 01:23:57.000000 configparserc-1.4.1/configparserc/include/
+-rw-rw-rw-   0 root         (0) root         (0)      518 2023-06-20 01:23:42.000000 configparserc-1.4.1/configparserc/include/_config.h
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-06-20 01:23:42.000000 configparserc-1.4.1/configparserc/py.typed
+-rw-r--r--   0 root         (0) root         (0)   341654 2023-06-20 01:23:56.000000 configparserc-1.4.1/configparserc/tools.c
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-06-20 01:23:42.000000 configparserc-1.4.1/configparserc/tools.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 01:23:57.000000 configparserc-1.4.1/configparserc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5363 2023-06-20 01:23:57.000000 configparserc-1.4.1/configparserc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      451 2023-06-20 01:23:57.000000 configparserc-1.4.1/configparserc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 01:23:57.000000 configparserc-1.4.1/configparserc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 01:23:57.000000 configparserc-1.4.1/configparserc.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       36 2023-06-20 01:23:57.000000 configparserc-1.4.1/configparserc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-20 01:23:57.000000 configparserc-1.4.1/configparserc.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1406 2023-06-20 01:23:57.000000 configparserc-1.4.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)    14641 2023-06-20 01:23:42.000000 configparserc-1.4.1/setup.py
```

### Comparing `configparserc-1.4.0/LICENSE` & `configparserc-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `configparserc-1.4.0/NOTICE` & `configparserc-1.4.1/NOTICE`

 * *Files identical despite different names*

### Comparing `configparserc-1.4.0/PKG-INFO` & `configparserc-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configparserc
-Version: 1.4.0
+Version: 1.4.1
 Summary: Python (Cython) based implementation of ConfigParser based on POSIX and stdlib functions.
 Home-page: https://gitlab.com/onegreyonewhite/configparserc
 Author: Sergey Klyuykov
 Author-email: onegreyonewhite@mail.ru
 License: Apache Software License
 Project-URL: Issue Tracker, https://gitlab.com/onegreyonewhite/configparserc/-/issues
 Project-URL: Source Code, https://gitlab.com/onegreyonewhite/configparserc.git
```

### Comparing `configparserc-1.4.0/README.rst` & `configparserc-1.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `configparserc-1.4.0/configparserc/__init__.py` & `configparserc-1.4.1/configparserc/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 
 """
 
-__version__ = '1.4.0'
+__version__ = '1.4.1'
```

### Comparing `configparserc-1.4.0/configparserc/config.c` & `configparserc-1.4.1/configparserc/config.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.34 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "configparserc/include/_config.h"
         ],
@@ -33,16 +33,16 @@
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
@@ -102,16 +102,20 @@
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
@@ -2186,30 +2190,30 @@
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* SetVTable.proto */
 static int __Pyx_SetVtable(PyObject *dict, void *vtable);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
+#define __PYX_HAVE_RT_ImportType_proto_0_29_35
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+enum __Pyx_ImportType_CheckSize_0_29_35 {
+   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
 #endif
 
 /* GetNameInClass.proto */
 #define __Pyx_GetNameInClass(var, nmspace, name)  (var) = __Pyx__GetNameInClass(nmspace, name)
 static PyObject *__Pyx__GetNameInClass(PyObject *nmspace, PyObject *name);
 
 /* CLineInTraceback.proto */
@@ -26403,15 +26407,15 @@
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
 
 static PyObject *__pyx_tp_new_13configparserc_6config_ConfigParserException(PyTypeObject *t, PyObject *a, PyObject *k) {
   PyObject *o = (&((PyTypeObject*)PyExc_Exception)[0])->tp_new(t, a, k);
   if (unlikely(!o)) return 0;
@@ -26509,15 +26513,15 @@
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
 
 static PyObject *__pyx_tp_new_13configparserc_6config_ParseError(PyTypeObject *t, PyObject *a, PyObject *k) {
   PyObject *o = __pyx_tp_new_13configparserc_6config_ConfigParserException(t, a, k);
   if (unlikely(!o)) return 0;
@@ -26593,15 +26597,15 @@
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
 
 static PyObject *__pyx_tp_new_13configparserc_6config_BaseType(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
@@ -26693,15 +26697,15 @@
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
 
 static PyObject *__pyx_tp_new_13configparserc_6config_StrType(PyTypeObject *t, PyObject *a, PyObject *k) {
   PyObject *o = __pyx_tp_new_13configparserc_6config_BaseType(t, a, k);
   if (unlikely(!o)) return 0;
@@ -26782,15 +26786,15 @@
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
 
 static PyObject *__pyx_tp_new_13configparserc_6config_IntType(PyTypeObject *t, PyObject *a, PyObject *k) {
   PyObject *o = __pyx_tp_new_13configparserc_6config_BaseType(t, a, k);
   if (unlikely(!o)) return 0;
@@ -26871,15 +26875,15 @@
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
 
 static PyObject *__pyx_tp_new_13configparserc_6config_BytesSizeType(PyTypeObject *t, PyObject *a, PyObject *k) {
   PyObject *o = __pyx_tp_new_13configparserc_6config_BaseType(t, a, k);
   if (unlikely(!o)) return 0;
@@ -26960,15 +26964,15 @@
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
 
 static PyObject *__pyx_tp_new_13configparserc_6config_BoolType(PyTypeObject *t, PyObject *a, PyObject *k) {
   PyObject *o = __pyx_tp_new_13configparserc_6config_BaseType(t, a, k);
   if (unlikely(!o)) return 0;
@@ -27049,15 +27053,15 @@
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
 
 static PyObject *__pyx_tp_new_13configparserc_6config_IntSecondsType(PyTypeObject *t, PyObject *a, PyObject *k) {
   PyObject *o = __pyx_tp_new_13configparserc_6config_BaseType(t, a, k);
   if (unlikely(!o)) return 0;
@@ -27138,15 +27142,15 @@
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
 
 static PyObject *__pyx_tp_new_13configparserc_6config_TimedeltaType(PyTypeObject *t, PyObject *a, PyObject *k) {
   PyObject *o = __pyx_tp_new_13configparserc_6config_BaseType(t, a, k);
   if (unlikely(!o)) return 0;
@@ -27227,15 +27231,15 @@
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
 
 static PyObject *__pyx_tp_new_13configparserc_6config_ListType(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_13configparserc_6config_ListType *p;
   PyObject *o = __pyx_tp_new_13configparserc_6config_BaseType(t, a, k);
@@ -27335,15 +27339,15 @@
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
 
 static PyObject *__pyx_tp_new_13configparserc_6config_JsonType(PyTypeObject *t, PyObject *a, PyObject *k) {
   PyObject *o = __pyx_tp_new_13configparserc_6config_BaseType(t, a, k);
   if (unlikely(!o)) return 0;
@@ -27425,15 +27429,15 @@
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
 
 static PyObject *__pyx_tp_new_13configparserc_6config___BaseDict(PyTypeObject *t, PyObject *a, PyObject *k) {
   PyObject *o = (&PyDict_Type)->tp_new(t, a, k);
   if (unlikely(!o)) return 0;
@@ -27546,15 +27550,15 @@
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
 static struct __pyx_vtabstruct_13configparserc_6config_ConfigParserC __pyx_vtable_13configparserc_6config_ConfigParserC;
 
 static PyObject *__pyx_tp_new_13configparserc_6config_ConfigParserC(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_13configparserc_6config_ConfigParserC *p;
@@ -27741,15 +27745,15 @@
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
 static struct __pyx_vtabstruct_13configparserc_6config_Section __pyx_vtable_13configparserc_6config_Section;
 
 static PyObject *__pyx_tp_new_13configparserc_6config_Section(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_13configparserc_6config_Section *p;
@@ -27951,15 +27955,15 @@
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
 static struct __pyx_vtabstruct_13configparserc_6config_AppendSection __pyx_vtable_13configparserc_6config_AppendSection;
 
 static PyObject *__pyx_tp_new_13configparserc_6config_AppendSection(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_13configparserc_6config_AppendSection *p;
@@ -28043,15 +28047,15 @@
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
 
 static struct __pyx_obj___pyx_scope_struct____Pyx_CFunc_dict____dict____unicode___to_py *__pyx_freelist___pyx_scope_struct____Pyx_CFunc_dict____dict____unicode___to_py[8];
 static int __pyx_freecount___pyx_scope_struct____Pyx_CFunc_dict____dict____unicode___to_py = 0;
 
@@ -28139,15 +28143,15 @@
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
 
 static struct __pyx_obj___pyx_scope_struct____Pyx_CFunc_bint____object___to_py *__pyx_freelist___pyx_scope_struct____Pyx_CFunc_bint____object___to_py[8];
 static int __pyx_freecount___pyx_scope_struct____Pyx_CFunc_bint____object___to_py = 0;
 
@@ -28235,15 +28239,15 @@
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
 
 static struct __pyx_obj___pyx_scope_struct____Pyx_CFunc_unicode____Section___to_py *__pyx_freelist___pyx_scope_struct____Pyx_CFunc_unicode____Section___to_py[8];
 static int __pyx_freecount___pyx_scope_struct____Pyx_CFunc_unicode____Section___to_py = 0;
 
@@ -28331,15 +28335,15 @@
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
@@ -29076,22 +29080,21 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -32743,15 +32746,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_CyFunction_init(void) {
     __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
     if (unlikely(__pyx_CyFunctionType == NULL)) {
         return -1;
@@ -32988,18 +32994,18 @@
     return 0;
 bad:
     Py_XDECREF(ob);
     return -1;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_35
+#define __PYX_HAVE_RT_ImportType_0_29_35
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -33045,22 +33051,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -33397,15 +33403,15 @@
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
@@ -33669,15 +33675,15 @@
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

### Comparing `configparserc-1.4.0/configparserc/config.pyi` & `configparserc-1.4.1/configparserc/config.pyi`

 * *Files identical despite different names*

### Comparing `configparserc-1.4.0/configparserc/include/_config.h` & `configparserc-1.4.1/configparserc/include/_config.h`

 * *Files identical despite different names*

### Comparing `configparserc-1.4.0/configparserc/tools.c` & `configparserc-1.4.1/configparserc/tools.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.34 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "extra_compile_args": [
             "-g0",
@@ -31,16 +31,16 @@
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
@@ -100,16 +100,20 @@
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
@@ -4594,15 +4598,15 @@
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
 
 static struct __pyx_obj_13configparserc_5tools___pyx_scope_struct__readlines *__pyx_freelist_13configparserc_5tools___pyx_scope_struct__readlines[8];
 static int __pyx_freecount_13configparserc_5tools___pyx_scope_struct__readlines = 0;
 
@@ -4707,15 +4711,15 @@
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
@@ -6822,15 +6826,15 @@
                         } else if (8 * sizeof(unsigned int) >= 4 * PyLong_SHIFT) {
                             return (unsigned int) (((((((((unsigned int)digits[3]) << PyLong_SHIFT) | (unsigned int)digits[2]) << PyLong_SHIFT) | (unsigned int)digits[1]) << PyLong_SHIFT) | (unsigned int)digits[0]));
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
@@ -7056,15 +7060,15 @@
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
@@ -7290,15 +7294,15 @@
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
@@ -8723,15 +8727,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_Generator_init(void) {
     __pyx_GeneratorType_type.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
     __pyx_GeneratorType_type.tp_iter = PyObject_SelfIter;
     __pyx_GeneratorType = __Pyx_FetchCommonType(&__pyx_GeneratorType_type);
```

### Comparing `configparserc-1.4.0/configparserc/tools.pyi` & `configparserc-1.4.1/configparserc/tools.pyi`

 * *Files identical despite different names*

### Comparing `configparserc-1.4.0/configparserc.egg-info/PKG-INFO` & `configparserc-1.4.1/configparserc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configparserc
-Version: 1.4.0
+Version: 1.4.1
 Summary: Python (Cython) based implementation of ConfigParser based on POSIX and stdlib functions.
 Home-page: https://gitlab.com/onegreyonewhite/configparserc
 Author: Sergey Klyuykov
 Author-email: onegreyonewhite@mail.ru
 License: Apache Software License
 Project-URL: Issue Tracker, https://gitlab.com/onegreyonewhite/configparserc/-/issues
 Project-URL: Source Code, https://gitlab.com/onegreyonewhite/configparserc.git
```

### Comparing `configparserc-1.4.0/setup.cfg` & `configparserc-1.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `configparserc-1.4.0/setup.py` & `configparserc-1.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -397,15 +397,15 @@
 
 kwargs = dict(
     name='configparserc',
     packages=find_packages(exclude=['tests']+ext_list),
     ext_modules_list=ext_list,
     install_requires=[
         'pytimeparse2~=1.7.1',
-        'pyyaml>=3.13,<5.4'
+        'pyyaml>=3.13,<6'
     ],
     project_urls={
         "Issue Tracker": "https://gitlab.com/onegreyonewhite/configparserc/-/issues",
         "Source Code": "https://gitlab.com/onegreyonewhite/configparserc.git",
         "Releases": "https://pypi.org/project/configparserc/#history",
     },
 )
```

