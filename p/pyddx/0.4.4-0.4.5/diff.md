# Comparing `tmp/pyddx-0.4.4.tar.gz` & `tmp/pyddx-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyddx-0.4.4.tar", last modified: Wed Jun  7 16:10:44 2023, max compression
+gzip compressed data, was "pyddx-0.4.5.tar", last modified: Tue Jun 20 15:35:46 2023, max compression
```

## Comparing `pyddx-0.4.4.tar` & `pyddx-0.4.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:10:44.276300 pyddx-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-07 16:08:50.000000 pyddx-0.4.4/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-07 16:08:50.000000 pyddx-0.4.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-07 16:08:50.000000 pyddx-0.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-06-07 16:10:44.276300 pyddx-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-06-07 16:08:50.000000 pyddx-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:10:44.272300 pyddx-0.4.4/pyddx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-06-07 16:10:44.000000 pyddx-0.4.4/pyddx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-07 16:10:44.000000 pyddx-0.4.4/pyddx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 16:10:44.000000 pyddx-0.4.4/pyddx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 16:08:58.000000 pyddx-0.4.4/pyddx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-07 16:10:44.000000 pyddx-0.4.4/pyddx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-07 16:10:44.000000 pyddx-0.4.4/pyddx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-07 16:08:50.000000 pyddx-0.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-07 16:10:44.276300 pyddx-0.4.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4297 2023-06-07 16:08:50.000000 pyddx-0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:10:44.276300 pyddx-0.4.4/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)   216556 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/cbessel.f90
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/ddx.f90
--rw-r--r--   0 runner    (1001) docker     (123)    21646 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/ddx.h
--rw-r--r--   0 runner    (1001) docker     (123)    28806 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/ddx_cinterface.f90
--rw-r--r--   0 runner    (1001) docker     (123)    92953 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/ddx_constants.f90
--rw-r--r--   0 runner    (1001) docker     (123)   122890 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/ddx_core.f90
--rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/ddx_cosmo.f90
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/ddx_definitions.f90
--rw-r--r--   0 runner    (1001) docker     (123)    14425 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/ddx_driver.f90
--rw-r--r--   0 runner    (1001) docker     (123)    73336 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/ddx_gradients.f90
--rw-r--r--   0 runner    (1001) docker     (123)   364736 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/ddx_harmonics.f90
--rw-r--r--   0 runner    (1001) docker     (123)    24612 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/ddx_lpb.f90
--rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/ddx_lpb_core.f90
--rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/ddx_mkrhs.f90
--rw-r--r--   0 runner    (1001) docker     (123)    58452 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/ddx_multipolar_solutes.f90
--rw-r--r--   0 runner    (1001) docker     (123)    71388 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/ddx_operators.f90
--rw-r--r--   0 runner    (1001) docker     (123)    17088 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/ddx_parameters.f90
--rw-r--r--   0 runner    (1001) docker     (123)    12852 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/ddx_pcm.f90
--rw-r--r--   0 runner    (1001) docker     (123)    11846 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/ddx_solvers.f90
--rw-r--r--   0 runner    (1001) docker     (123)    20725 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/ddx_workspace.f90
--rw-r--r--   0 runner    (1001) docker     (123)   260805 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/llgnew.f
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/matrix_debug.f90
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/pyddx.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    31313 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/pyddx_classes.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12879 2023-06-07 16:08:50.000000 pyddx-0.4.4/src/pyddx_data.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:35:46.229686 pyddx-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-20 15:33:23.000000 pyddx-0.4.5/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-20 15:33:23.000000 pyddx-0.4.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-20 15:33:23.000000 pyddx-0.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-06-20 15:35:46.229686 pyddx-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-06-20 15:33:23.000000 pyddx-0.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:35:46.225685 pyddx-0.4.5/pyddx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-06-20 15:35:46.000000 pyddx-0.4.5/pyddx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-20 15:35:46.000000 pyddx-0.4.5/pyddx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:35:46.000000 pyddx-0.4.5/pyddx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:33:33.000000 pyddx-0.4.5/pyddx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-20 15:35:46.000000 pyddx-0.4.5/pyddx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 15:35:46.000000 pyddx-0.4.5/pyddx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-20 15:33:23.000000 pyddx-0.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-20 15:35:46.229686 pyddx-0.4.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4297 2023-06-20 15:33:23.000000 pyddx-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:35:46.229686 pyddx-0.4.5/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-20 15:33:23.000000 pyddx-0.4.5/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   216556 2023-06-20 15:33:23.000000 pyddx-0.4.5/src/cbessel.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-20 15:33:23.000000 pyddx-0.4.5/src/ddx.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    21646 2023-06-20 15:33:23.000000 pyddx-0.4.5/src/ddx.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28806 2023-06-20 15:33:23.000000 pyddx-0.4.5/src/ddx_cinterface.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    92953 2023-06-20 15:33:23.000000 pyddx-0.4.5/src/ddx_constants.f90
+-rw-r--r--   0 runner    (1001) docker     (123)   122848 2023-06-20 15:33:23.000000 pyddx-0.4.5/src/ddx_core.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-06-20 15:33:23.000000 pyddx-0.4.5/src/ddx_cosmo.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-20 15:33:23.000000 pyddx-0.4.5/src/ddx_definitions.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    14999 2023-06-20 15:33:23.000000 pyddx-0.4.5/src/ddx_driver.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    73336 2023-06-20 15:33:23.000000 pyddx-0.4.5/src/ddx_gradients.f90
+-rw-r--r--   0 runner    (1001) docker     (123)   364736 2023-06-20 15:33:23.000000 pyddx-0.4.5/src/ddx_harmonics.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    24967 2023-06-20 15:33:23.000000 pyddx-0.4.5/src/ddx_lpb.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-06-20 15:33:23.000000 pyddx-0.4.5/src/ddx_lpb_core.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-06-20 15:33:23.000000 pyddx-0.4.5/src/ddx_mkrhs.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    58452 2023-06-20 15:33:23.000000 pyddx-0.4.5/src/ddx_multipolar_solutes.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    72363 2023-06-20 15:33:23.000000 pyddx-0.4.5/src/ddx_operators.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    17088 2023-06-20 15:33:23.000000 pyddx-0.4.5/src/ddx_parameters.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    12852 2023-06-20 15:33:23.000000 pyddx-0.4.5/src/ddx_pcm.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    11846 2023-06-20 15:33:23.000000 pyddx-0.4.5/src/ddx_solvers.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    20812 2023-06-20 15:33:23.000000 pyddx-0.4.5/src/ddx_workspace.f90
+-rw-r--r--   0 runner    (1001) docker     (123)   260805 2023-06-20 15:33:23.000000 pyddx-0.4.5/src/llgnew.f
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-20 15:33:23.000000 pyddx-0.4.5/src/matrix_debug.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-20 15:33:23.000000 pyddx-0.4.5/src/pyddx.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    31313 2023-06-20 15:33:23.000000 pyddx-0.4.5/src/pyddx_classes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12879 2023-06-20 15:33:23.000000 pyddx-0.4.5/src/pyddx_data.cpp
```

### Comparing `pyddx-0.4.4/CMakeLists.txt` & `pyddx-0.4.5/CMakeLists.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Restrict building in top-level directory
 if("${CMAKE_CURRENT_SOURCE_DIR}" STREQUAL "${CMAKE_CURRENT_BINARY_DIR}")
     message(FATAL_ERROR "In-source builds are not allowed.\nPlease create a "
         "build directory first and execute cmake configuration from this "
         "directory. Example: mkdir build && cd build && cmake ..")
 endif()
 
-project(ddX VERSION 0.4.4 LANGUAGES Fortran CXX)
+project(ddX VERSION 0.4.5 LANGUAGES Fortran CXX)
 # If ddX is a subproject, append ddx_ prefix to all targets.
 if(CMAKE_PROJECT_NAME STREQUAL PROJECT_NAME)
     set(ddx_is_subproject false)
     set(ddx_ "")
 else()
     set(ddx_is_subproject true)
     set(ddx_ "ddx_")
```

### Comparing `pyddx-0.4.4/LICENSE.txt` & `pyddx-0.4.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.4/PKG-INFO` & `pyddx-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyddx
-Version: 0.4.4
+Version: 0.4.5
 Summary: ddx continuum solvation library
 Home-page: https://ddsolvation.github.io/ddX
 Author: ddx developers
 Author-email: best@ians.uni-stuttgart.de
 License: LGPL v3
 Project-URL: Source, https://github.com/ddsolvation/ddX
 Project-URL: Issues, https://github.com/ddsolvation/ddX/issues
```

### Comparing `pyddx-0.4.4/README.md` & `pyddx-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.4/pyddx.egg-info/PKG-INFO` & `pyddx-0.4.5/pyddx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyddx
-Version: 0.4.4
+Version: 0.4.5
 Summary: ddx continuum solvation library
 Home-page: https://ddsolvation.github.io/ddX
 Author: ddx developers
 Author-email: best@ians.uni-stuttgart.de
 License: LGPL v3
 Project-URL: Source, https://github.com/ddsolvation/ddX
 Project-URL: Issues, https://github.com/ddsolvation/ddX/issues
```

### Comparing `pyddx-0.4.4/pyddx.egg-info/SOURCES.txt` & `pyddx-0.4.5/pyddx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.4/setup.py` & `pyddx-0.4.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 # The information here can also be placed in setup.cfg - better separation of
 # logic and declaration, and simpler if you include description/version in a file.
 setup(
     name="pyddx",
     description="ddx continuum solvation library",
     long_description=read_readme(),
     long_description_content_type="text/markdown",
-    version="0.4.4",
+    version="0.4.5",
     #
     author="ddx developers",
     author_email="best@ians.uni-stuttgart.de",
     license="LGPL v3",
     url="https://ddsolvation.github.io/ddX",
     project_urls={
         "Source": "https://github.com/ddsolvation/ddX",
```

### Comparing `pyddx-0.4.4/src/CMakeLists.txt` & `pyddx-0.4.5/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.4/src/cbessel.f90` & `pyddx-0.4.5/src/cbessel.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.4/src/ddx.f90` & `pyddx-0.4.5/src/ddx.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.4/src/ddx.h` & `pyddx-0.4.5/src/ddx.h`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.4/src/ddx_cinterface.f90` & `pyddx-0.4.5/src/ddx_cinterface.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.4/src/ddx_constants.f90` & `pyddx-0.4.5/src/ddx_constants.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.4/src/ddx_core.f90` & `pyddx-0.4.5/src/ddx_core.f90`

 * *Files 0% similar despite different names*

```diff
@@ -183,14 +183,16 @@
     !> Zeta dipoles intermediate for the forces. Dimension (3, ncav).
     !! Allocated and used only by the LPB (model=3) model.
     real(dp), allocatable :: zeta_dip(:, :)
     real(dp), allocatable :: x_adj_re_grid(:, :)
     real(dp), allocatable :: x_adj_r_grid(:, :)
     real(dp), allocatable :: x_adj_e_grid(:, :)
     real(dp), allocatable :: phi_n(:, :)
+    real(dp) :: hsp_time
+    real(dp) :: hsp_adj_time
 
 end type ddx_state_type
 
 !> Main ddX type that stores all the required information.
 !! Container for the params, contants and workspace derived types.
 type ddx_type
     !! New types inside the old one for an easier shift to the new design
@@ -2366,41 +2368,39 @@
     real(dp), intent(out) :: node_m((params % pm+1)**2, constants % nclusters)
     ! Temporary workspace
     real(dp) :: work(6*params % pm**2 + 19*params % pm + 8)
     complex(dp) :: work_complex(2*params % pm+1)
     ! Local variables
     integer :: i, j, k
     real(dp) :: c1(3), c(3), r
-    ! Any order of this cycle is OK
     node_m = zero
-    !!$omp parallel do shared(constants,params,node_l,node_m) &
-    !!$omp private(i,c,r,k,c1,work,work_complex,j) schedule(dynamic)
+    !$omp parallel do shared(constants,params,node_l,node_m) &
+    !$omp private(i,c,r,k,c1,work,work_complex,j) schedule(dynamic)
     do i = 1, constants % nclusters
         ! If no far admissible pairs just set output to zero
         if (constants % nfar(i) .eq. 0) then
             cycle
         end if
         c = constants % cnode(:, i)
         r = constants % rnode(i)
         ! Use the first far admissible pair to initialize output
         k = constants % far(constants % sfar(i))
         c1 = constants % cnode(:, k)
-        c1 = params % kappa*(c1 - c)
-        call fmm_m2l_bessel_rotation_adj_work(c1, constants % SI_rnode(:, i), &
-            & constants % SK_rnode(:, k), params % pm, &
-            & constants % vscales, one, &
-            & node_l(:, i), one, node_m(:, k), work, work_complex)
+        c1 = params % kappa*(c - c1)
+        call fmm_m2l_bessel_rotation_adj_work(c1, constants % SI_rnode(:, k), &
+            & constants % SK_rnode(:, i), params % pm, constants % vscales, &
+            & one, node_l(:, k), one, node_m(:, i), work, work_complex)
         do j = constants % sfar(i)+1, constants % sfar(i+1)-1
             k = constants % far(j)
             c1 = constants % cnode(:, k)
-            c1 = params % kappa*(c1 - c)
-            call fmm_m2l_bessel_rotation_adj_work(c1, constants % SI_rnode(:, i), &
-                & constants % SK_rnode(:, k), params % pm, &
-                & constants % vscales, one, &
-                & node_l(:, i), one, node_m(:, k), work, work_complex)
+            c1 = params % kappa*(c - c1)
+            call fmm_m2l_bessel_rotation_adj_work(c1, &
+                & constants % SI_rnode(:, k), constants % SK_rnode(:, i), &
+                & params % pm, constants % vscales, one, node_l(:, k), &
+                & one, node_m(:, i), work, work_complex)
         end do
     end do
 end subroutine tree_m2l_bessel_rotation_adj_work
 
 !------------------------------------------------------------------------------
 !> Adjoint transfer multipole local coefficients into local over a tree
 !------------------------------------------------------------------------------
@@ -2411,39 +2411,40 @@
     type(ddx_constants_type), intent(in) :: constants
     real(dp), intent(in) :: node_l((params % pl+1)**2, constants % nclusters)
     ! Output
     real(dp), intent(out) :: node_m((params % pm+1)**2, constants % nclusters)
     ! Local variables
     integer :: i, j, k
     real(dp) :: c1(3), c(3), r1, r
-    ! Any order of this cycle is OK
     node_m = zero
+    !$omp parallel do default(none) shared(constants,params,node_m,node_l) &
+    !$omp private(i,c,r,k,c1,r1,j) schedule(dynamic)
     do i = 1, constants % nclusters
         ! If no far admissible pairs just set output to zero
         if (constants % nfar(i) .eq. 0) then
             cycle
         end if
         c = constants % cnode(:, i)
         r = constants % rnode(i)
         ! Use the first far admissible pair to initialize output
         k = constants % far(constants % sfar(i))
         c1 = constants % cnode(:, k)
         r1 = constants % rnode(k)
-        c1 = c - c1
-        call fmm_m2l_rotation_adj(c1, r, r1, params % pl, params % pm, &
+        c1 = c1 - c
+        call fmm_m2l_rotation_adj(c1, r1, r, params % pl, params % pm, &
             & constants % vscales, constants % m2l_ztranslate_adj_coef, one, &
-            & node_l(:, i), one, node_m(:, k))
+            & node_l(:, k), one, node_m(:, i))
         do j = constants % sfar(i)+1, constants % sfar(i+1)-1
             k = constants % far(j)
             c1 = constants % cnode(:, k)
             r1 = constants % rnode(k)
-            c1 = c - c1
-            call fmm_m2l_rotation_adj(c1, r, r1, params % pl, params % pm, &
+            c1 = c1 - c
+            call fmm_m2l_rotation_adj(c1, r1, r, params % pl, params % pm, &
                 & constants % vscales, constants % m2l_ztranslate_adj_coef, one, &
-                & node_l(:, i), one, node_m(:, k))
+                & node_l(:, k), one, node_m(:, i))
         end do
     end do
 end subroutine tree_m2l_rotation_adj
 
 !------------------------------------------------------------------------------
 !> TODO
 !------------------------------------------------------------------------------
@@ -2716,35 +2717,35 @@
     ! Init output
     if (beta .eq. zero) then
         sph_m = zero
     else
         sph_m = beta * sph_m
     end if
     ! Cycle over all spheres
-    !!$omp parallel do default(none) shared(params,constants,grid_v,p, &
-    !!$omp alpha,sph_m), private(isph,inode,jnear,jnode,jsph,igrid,c,work) &
-    !!$omp schedule(dynamic)
+    !$omp parallel do default(none) shared(params,constants,grid_v,p, &
+    !$omp alpha,sph_m), private(isph,inode,jnear,jnode,jsph,igrid,c,work) &
+    !$omp schedule(dynamic)
     do isph = 1, params % nsph
         ! Cycle over all near-field admissible pairs of spheres
         inode = constants % snode(isph)
         do jnear = constants % snear(inode), constants % snear(inode+1)-1
             ! Near-field interactions are possible only between leaf nodes,
             ! which must contain only a single input sphere
             jnode = constants % near(jnear)
             jsph = constants % order(constants % cluster(1, jnode))
             ! Ignore self-interaction
             if(isph .eq. jsph) cycle
             ! Accumulate interaction for external grid points only
             do igrid = 1, params % ngrid
-                if(constants % ui(igrid, isph) .eq. zero) cycle
-                c = constants % cgrid(:, igrid)*params % rsph(isph) - &
-                    & params % csph(:, jsph) + params % csph(:, isph)
-                call fmm_m2p_adj_work(c, alpha*grid_v(igrid, isph), &
-                    & params % rsph(jsph), p, constants % vscales_rel, one, &
-                    & sph_m(:, jsph), work)
+                if(constants % ui(igrid, jsph) .eq. zero) cycle
+                c = constants % cgrid(:, igrid)*params % rsph(jsph) - &
+                    & params % csph(:, isph) + params % csph(:, jsph)
+                call fmm_m2p_adj_work(c, alpha*grid_v(igrid, jsph), &
+                    & params % rsph(isph), p, constants % vscales_rel, one, &
+                    & sph_m(:, isph), work)
             end do
         end do
     end do
 end subroutine tree_m2p_adj
 
 !------------------------------------------------------------------------------
 !> TODO
@@ -2767,36 +2768,33 @@
     ! Init output
     if (beta .eq. zero) then
         sph_m = zero
     else
         sph_m = beta * sph_m
     end if
     ! Cycle over all spheres
-    !!$omp parallel do default(none) shared(params,constants,p,sph_m,tmp, &
-    !!$omp alpha,grid_v) private(isph,inode,jnear,jnode,jsph,igrid,c, &
-    !!$omp iproc) schedule(dynamic)
+    !$omp parallel do default(none) shared(params,constants,p,sph_m, &
+    !$omp alpha,grid_v) private(isph,inode,jnear,jnode,jsph,igrid,c) &
+    !$omp schedule(dynamic)
     do isph = 1, params % nsph
         ! Cycle over all near-field admissible pairs of spheres
         inode = constants % snode(isph)
-        ! iproc = omp_get_thread_num() + 1
         do jnear = constants % snear(inode), constants % snear(inode+1)-1
             ! Near-field interactions are possible only between leaf nodes,
             ! which must contain only a single input sphere
             jnode = constants % near(jnear)
             jsph = constants % order(constants % cluster(1, jnode))
-            ! Ignore self-interaction
-            !if(isph .eq. jsph) cycle
             ! Accumulate interaction for external grid points only
             do igrid = 1, params % ngrid
-                if(constants % ui(igrid, isph) .eq. zero) cycle
-                c = constants % cgrid(:, igrid)*params % rsph(isph) - &
-                    & params % csph(:, jsph) + params % csph(:, isph)
-                call fmm_m2p_bessel_adj(c, alpha*grid_v(igrid, isph), &
-                    & params % rsph(jsph), params % kappa, p, &
-                    & constants % vscales, one, sph_m(:, jsph))
+                if(constants % ui(igrid, jsph) .eq. zero) cycle
+                c = constants % cgrid(:, igrid)*params % rsph(jsph) - &
+                    & params % csph(:, isph) + params % csph(:, jsph)
+                call fmm_m2p_bessel_adj(c, alpha*grid_v(igrid, jsph), &
+                    & params % rsph(isph), params % kappa, p, &
+                    & constants % vscales, one, sph_m(:, isph))
             end do
         end do
     end do
 end subroutine tree_m2p_bessel_adj
 
 !------------------------------------------------------------------------------
 !> TODO
@@ -3021,15 +3019,15 @@
 !!
 !! @param[out] string: container for the logo
 !!
 subroutine get_banner(string)
     implicit none
     character (len=2047), intent(out) :: string
     character (len=10) :: vstr
-    write(vstr, *) "0.4.4"
+    write(vstr, *) "0.4.5"
     write(string, *) &
         & " +----------------------------------------------------------------+", &
         & NEW_LINE('a'), &
         & "  |                                                                |", &
         & NEW_LINE('a'), &
         & "  |                        888      888 Y8b    d8Y                 |", &
         & NEW_LINE('a'), &
```

### Comparing `pyddx-0.4.4/src/ddx_cosmo.f90` & `pyddx-0.4.5/src/ddx_cosmo.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.4/src/ddx_definitions.f90` & `pyddx-0.4.5/src/ddx_definitions.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.4/src/ddx_driver.f90` & `pyddx-0.4.5/src/ddx_driver.f90`

 * *Files 6% similar despite different names*

```diff
@@ -294,15 +294,20 @@
 if (ddx_data % params % model .eq. 3) then
     ! Print each iteration if needed
     do i = 1, state % x_lpb_niter
         write(6, 200) "iter=", i, " relative difference: ", &
             & state % x_lpb_rel_diff(i)
     end do
     ! Print number of iterations and time
-    write(6, 100) "ddlpb step time: ", state % x_lpb_time, " seconds"
+    write(6, 100) "ddlpb step time: ", state % x_lpb_time, &
+        & " seconds, of which:"
+    write(6, 100) "    ddcosmo: ", state % xs_time, " seconds"
+    write(6, 100) "    hsp: ", state % hsp_time, " seconds"
+    write(6, 100) "    coupling terms: ", state % x_lpb_time &
+        & - state % xs_time - state % hsp_time, " seconds"
     write(6, 300) "ddlpb step iterations: ", state % x_lpb_niter
 end if
 
 ! Print info on the primal ddCOSMO system
 ! Print each iteration if needed
 if ((ddx_data % params % model.eq.1) .or. &
         & (ddx_data % params % model.eq.2)) then
@@ -344,15 +349,19 @@
     if (ddx_data % params % model .eq. 3) then
         do i = 1, state % x_adj_lpb_niter
             write(6, 200) "iter=", i, " relative difference: ", &
                 & state % x_adj_lpb_rel_diff(i)
         end do
         ! Print number of iterations and time
         write(6, 100) "adjoint ddlpb step time: ", &
-            & state % x_adj_lpb_time, " seconds"
+            & state % x_adj_lpb_time, " seconds, of which:"
+        write(6, 100) "    adjoint ddcosmo: ", state % s_time, " seconds"
+        write(6, 100) "    adjoint hsp: ", state % hsp_adj_time, " seconds"
+        write(6, 100) "    adjoint coupling terms: ", state % x_adj_lpb_time &
+            & - state % s_time - state % hsp_adj_time, " seconds"
         write(6, 200) "adjoint ddlpb step iterations: ", &
             & state % x_adj_lpb_niter
     end if
 end if
 
 write(6, 400) "Solvation energy (Hartree):", esolv
 write(6, 400) "Solvation energy (kcal/mol):", esolv*tokcal
```

### Comparing `pyddx-0.4.4/src/ddx_gradients.f90` & `pyddx-0.4.5/src/ddx_gradients.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.4/src/ddx_harmonics.f90` & `pyddx-0.4.5/src/ddx_harmonics.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.4/src/ddx_lpb.f90` & `pyddx-0.4.5/src/ddx_lpb.f90`

 * *Files 4% similar despite different names*

```diff
@@ -229,14 +229,16 @@
     type(ddx_constants_type), intent(inout) :: constants
     type(ddx_workspace_type), intent(inout) :: workspace
     type(ddx_state_type), intent(inout) :: state
     real(dp), intent(in) :: tol
     real(dp) :: start_time
 
     state % x_lpb_niter = params % maxiter
+    workspace % xs_time = zero
+    workspace % hsp_time = zero
 
     ! solve LS using Jacobi/DIIS
     start_time = omp_get_wtime()
     call jacobi_diis_external(params, constants, workspace, &
         & 2*constants % n, tol, state % rhs_lpb, state % x_lpb, &
         & state % x_lpb_niter, state % x_lpb_rel_diff, cx, prec_tx, rmsnorm)
     if (workspace % error_flag .ne. 0) then
@@ -247,14 +249,18 @@
     state % x_lpb_time = omp_get_wtime() - start_time
     ! in ddLPB the polarization density X is expanded according to a
     ! slightly different definition which lacks the 4pi/(2l + 1) factors
     ! which are present in ddCOSMO and ddPCM. Before exiting, we scale
     ! the density so that it is consistent with the ddCOSMO and ddPCM
     ! ones.
     call convert_ddcosmo(params, constants, -1, state % x_lpb(:,:,1))
+
+    ! put the timings in the right places
+    state % xs_time = workspace % xs_time
+    state % hsp_time = workspace % hsp_time
 end subroutine ddlpb_solve
 
 
 !> Solve the adjoint ddLPB linear system
 !!
 !> @ingroup Fortran_interface_ddlpb
 !! @param[in] params       : General options
@@ -270,15 +276,16 @@
     type(ddx_workspace_type), intent(inout) :: workspace
     type(ddx_state_type), intent(inout) :: state
     real(dp), intent(in) :: tol
 
     real(dp) :: start_time
 
     state % x_adj_lpb_niter = params % maxiter
-    constants % inner_tol = sqrt(tol)
+    workspace % s_time = zero
+    workspace % hsp_adj_time = zero
 
     ! solve adjoint LS using Jacobi/DIIS
     start_time = omp_get_wtime()
     call jacobi_diis_external(params, constants, workspace, &
         & 2*constants % n, tol, state % rhs_adj_lpb, state % x_adj_lpb, &
         & state % x_adj_lpb_niter, state % x_adj_lpb_rel_diff, &
         & cstarx, prec_tstarx, rmsnorm)
@@ -287,14 +294,18 @@
             & 'converge in ddlpb_solve_adjoint'
         return
     end if
     state % x_adj_lpb_time = omp_get_wtime() - start_time
 
     state % q = state % x_adj_lpb(:, :, 1)
 
+    ! put the timings in the right places
+    state % s_time = workspace % s_time
+    state % hsp_adj_time = workspace % hsp_adj_time
+
     call ddlpb_derivative_setup(params, constants, workspace, state)
 
 end subroutine ddlpb_solve_adjoint
 
 !> Compute the solvation terms of the forces (solute aspecific). This
 !! must be summed to the solute specific term to get the full forces.
 !!
```

### Comparing `pyddx-0.4.4/src/ddx_lpb_core.f90` & `pyddx-0.4.5/src/ddx_lpb_core.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.4/src/ddx_mkrhs.f90` & `pyddx-0.4.5/src/ddx_mkrhs.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.4/src/ddx_multipolar_solutes.f90` & `pyddx-0.4.5/src/ddx_multipolar_solutes.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.4/src/ddx_operators.f90` & `pyddx-0.4.5/src/ddx_operators.f90`

 * *Files 1% similar despite different names*

```diff
@@ -366,44 +366,49 @@
     ! Temporaries
     type(ddx_workspace_type), intent(inout) :: workspace
     ! Output
     real(dp), intent(out) :: y(constants % nbasis, params % nsph)
     ! Local variables
     real(dp) :: vji(3), sji(3)
     real(dp) :: vvji, tji, tt, f, rho, ctheta, stheta, cphi, sphi
-    integer :: its, isph, jsph, l, m, ind
+    integer :: its, isph, jsph, l, m, ind, iproc
     real(dp), external :: dnrm2
     y = zero
-    ! this loop is easily parallelizable
+    !$omp parallel do default(none) shared(do_diag,params,constants, &
+    !$omp workspace,x,y) private(isph,jsph,its,vji,vvji,tji,sji,rho, &
+    !$omp ctheta,stheta,cphi,sphi,tt,l,ind,f,m,iproc) schedule(dynamic)
     do isph = 1, params % nsph
+        iproc = omp_get_thread_num() + 1
         do jsph = 1, params % nsph
             if (jsph.ne.isph) then
                 do its = 1, params % ngrid
                     if (constants % ui(its,jsph).gt.zero) then
                         ! build the geometrical variables
                         vji = params % csph(:,jsph) + params % rsph(jsph) * &
                             & constants % cgrid(:,its) - params % csph(:,isph)
                         !vvji = sqrt(dot_product(vji,vji))
                         vvji = dnrm2(3, vji, 1)
                         tji = vvji/params % rsph(isph)
                         sji = vji/vvji
                         ! build the local basis
                         call ylmbas(sji, rho, ctheta, stheta, cphi, sphi, &
                             & params % lmax, constants % vscales, &
-                            & workspace % tmp_vylm, workspace % tmp_vplm, &
-                            & workspace % tmp_vcos, workspace % tmp_vsin)
+                            & workspace % tmp_vylm(:(params % lmax + 1)**2, iproc), &
+                            & workspace % tmp_vplm(:(params % lmax + 1)**2, iproc), &
+                            & workspace % tmp_vcos(:(params % lmax + 1), iproc), &
+                            & workspace % tmp_vsin(:(params % lmax + 1), iproc))
                         tt = constants % ui(its,jsph) &
                             & *dot_product(constants % vwgrid(:constants % nbasis, its), &
                             & x(:,jsph))/tji
                         do l = 0, params % lmax
                             ind = l*l + l + 1
                             f = dble(l)*tt/ constants % vscales(ind)**2
                             do m = -l, l
                                 y(ind+m,isph) = y(ind+m,isph) + &
-                                    & f*workspace % tmp_vylm(ind+m, 1)
+                                    & f*workspace % tmp_vylm(ind+m, iproc)
                             end do
                             tt = tt/tji
                         end do
                     end if
                 end do
             else if (do_diag .eq. 1) then
                 do its = 1, params % ngrid
@@ -1351,34 +1356,42 @@
     type(ddx_params_type), intent(in) :: params
     type(ddx_constants_type), intent(in) :: constants
     type(ddx_workspace_type), intent(inout) :: workspace
     real(dp), intent(in) :: x(constants % nbasis, params % nsph, 2)
     real(dp), intent(inout) :: y(constants % nbasis, params % nsph, 2)
     integer :: n_iter
     real(dp), dimension(params % maxiter) :: x_rel_diff
+    real(dp) :: start_time
 
+    start_time = omp_get_wtime()
     y(:,:,1) = x(:,:,1)
     call convert_ddcosmo(params, constants, 1, y(:,:,1))
     n_iter = params % maxiter
-    call jacobi_diis(params, constants, workspace, constants % inner_tol, y(:,:,1), &
-        & workspace % ddcosmo_guess, n_iter, x_rel_diff, lstarx, ldm1x, hnorm)
+    call jacobi_diis(params, constants, workspace, constants % inner_tol, &
+        & y(:,:,1), workspace % ddcosmo_guess, n_iter, x_rel_diff, lstarx, &
+        & ldm1x, hnorm)
     if (workspace % error_flag.ne.0) then
         workspace % error_message = 'prec_tstarx: ddCOSMO failed to converge'
         return
     end if
     y(:,:,1) = workspace % ddcosmo_guess
+    workspace % s_time = workspace % s_time + omp_get_wtime() - start_time
 
+    start_time = omp_get_wtime()
     n_iter = params % maxiter
-    call jacobi_diis(params, constants, workspace, constants % inner_tol, x(:,:,2), workspace % hsp_guess, &
-        & n_iter, x_rel_diff, bstarx, bx_prec, hnorm)
+    call jacobi_diis(params, constants, workspace, constants % inner_tol, &
+        & x(:,:,2), workspace % hsp_guess, n_iter, x_rel_diff, bstarx, &
+        & bx_prec, hnorm)
     if (workspace % error_flag.ne.0) then
         workspace % error_message = 'prec_tstarx: HSP failed to converge'
         return
     end if
     y(:,:,2) = workspace % hsp_guess
+    workspace % hsp_adj_time = workspace % hsp_adj_time &
+        & + omp_get_wtime() - start_time
 
 end subroutine prec_tstarx
 
 !> Apply the preconditioner to the primal ddLPB linear system
 !! |Yr| = |A^-1 0 |*|Xr|
 !! |Ye|   |0 B^-1 | |Xe|
 !! @param[in] ddx_data : dd Data
@@ -1389,33 +1402,40 @@
     type(ddx_params_type), intent(in) :: params
     type(ddx_constants_type), intent(in) :: constants
     type(ddx_workspace_type), intent(inout) :: workspace
     real(dp), intent(in) :: x(constants % nbasis, params % nsph, 2)
     real(dp), intent(inout) :: y(constants % nbasis, params % nsph, 2)
     integer :: n_iter
     real(dp), dimension(params % maxiter) :: x_rel_diff
+    real(dp) :: start_time
 
     ! perform A^-1 * Yr
+    start_time = omp_get_wtime()
     n_iter = params % maxiter
-    call jacobi_diis(params, constants, workspace, constants % inner_tol, x(:,:,1), &
-        & workspace % ddcosmo_guess, n_iter, x_rel_diff, lx, ldm1x, hnorm)
+    call jacobi_diis(params, constants, workspace, constants % inner_tol, &
+        & x(:,:,1), workspace % ddcosmo_guess, n_iter, x_rel_diff, lx, &
+        & ldm1x, hnorm)
     if (workspace % error_flag.ne.0) then
         workspace % error_message = 'prec_tx: ddCOSMO failed to converge'
         return
     end if
 
     ! Scale by the factor of (2l+1)/4Pi
     y(:,:,1) = workspace % ddcosmo_guess
     call convert_ddcosmo(params, constants, 1, y(:,:,1))
+    workspace % xs_time = workspace % xs_time + omp_get_wtime() - start_time
 
     ! perform B^-1 * Ye
+    start_time = omp_get_wtime()
     n_iter = params % maxiter
-    call jacobi_diis(params, constants, workspace, constants % inner_tol, x(:,:,2), workspace % hsp_guess, &
-        & n_iter, x_rel_diff, bx, bx_prec, hnorm)
+    call jacobi_diis(params, constants, workspace, constants % inner_tol, &
+        & x(:,:,2), workspace % hsp_guess, n_iter, x_rel_diff, bx, &
+        & bx_prec, hnorm)
     y(:,:,2) = workspace % hsp_guess
+    workspace % hsp_time = workspace % hsp_time + omp_get_wtime() - start_time
 
     if (workspace % error_flag.ne.0) then
         workspace % error_message = 'prec_tx: HSP failed to converge'
         return
     end if
 end subroutine prec_tx
```

### Comparing `pyddx-0.4.4/src/ddx_parameters.f90` & `pyddx-0.4.5/src/ddx_parameters.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.4/src/ddx_pcm.f90` & `pyddx-0.4.5/src/ddx_pcm.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.4/src/ddx_solvers.f90` & `pyddx-0.4.5/src/ddx_solvers.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.4/src/ddx_workspace.f90` & `pyddx-0.4.5/src/ddx_workspace.f90`

 * *Files 0% similar despite different names*

```diff
@@ -94,14 +94,16 @@
     real(dp), allocatable :: tmp_x_diis(:, :)
     !> Jacobi solver temporary DIIS array. Dimension is (n, ndiis).
     real(dp), allocatable :: tmp_e_diis(:, :)
     !> Jacobi solver temporary DIIS array. Dimension is (ndiis+1, ndiis+1).
     real(dp), allocatable :: tmp_bmat(:, :)
     !> ddLPB solutions for the microiterations
     real(dp), allocatable :: ddcosmo_guess(:,:), hsp_guess(:,:)
+    !> ddLPB temporary timings
+    real(dp) :: xs_time, s_time, hsp_time, hsp_adj_time
     !> Flag if there were an error
     integer :: error_flag = 2
     !> Last error message
     character(len=255) :: error_message
 end type ddx_workspace_type
 
 contains
```

### Comparing `pyddx-0.4.4/src/llgnew.f` & `pyddx-0.4.5/src/llgnew.f`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.4/src/matrix_debug.f90` & `pyddx-0.4.5/src/matrix_debug.f90`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.4/src/pyddx.cpp` & `pyddx-0.4.5/src/pyddx.cpp`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.4/src/pyddx_classes.cpp` & `pyddx-0.4.5/src/pyddx_classes.cpp`

 * *Files identical despite different names*

### Comparing `pyddx-0.4.4/src/pyddx_data.cpp` & `pyddx-0.4.5/src/pyddx_data.cpp`

 * *Files identical despite different names*

