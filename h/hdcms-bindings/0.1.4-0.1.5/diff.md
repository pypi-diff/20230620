# Comparing `tmp/hdcms-bindings-0.1.4.tar.gz` & `tmp/hdcms-bindings-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdcms-bindings-0.1.4.tar", last modified: Fri Feb  3 06:09:59 2023, max compression
+gzip compressed data, was "hdcms-bindings-0.1.5.tar", last modified: Tue Jun 20 08:57:22 2023, max compression
```

## Comparing `hdcms-bindings-0.1.4.tar` & `hdcms-bindings-0.1.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jason      (502) staff       (20)        0 2023-02-03 06:09:59.439540 hdcms-bindings-0.1.4/
--rw-r--r--   0 jason      (502) staff       (20)     1830 2023-01-22 19:56:08.000000 hdcms-bindings-0.1.4/LICENSE
--rw-r--r--   0 jason      (502) staff       (20)      146 2023-02-03 06:05:56.000000 hdcms-bindings-0.1.4/MANIFEST.in
--rw-r--r--   0 jason      (502) staff       (20)     5446 2023-02-03 06:09:59.439376 hdcms-bindings-0.1.4/PKG-INFO
--rw-r--r--   0 jason      (502) staff       (20)     2969 2023-02-03 06:09:40.000000 hdcms-bindings-0.1.4/README.md
-drwxr-xr-x   0 jason      (502) staff       (20)        0 2023-02-03 06:09:59.435227 hdcms-bindings-0.1.4/hdcms-c/
-drwxr-xr-x   0 jason      (502) staff       (20)        0 2023-02-03 06:09:59.436479 hdcms-bindings-0.1.4/hdcms-c/src/
--rw-r--r--   0 jason      (502) staff       (20)      882 2023-02-03 05:04:03.000000 hdcms-bindings-0.1.4/hdcms-c/src/fixwindows.h
--rw-r--r--   0 jason      (502) staff       (20)    10268 2023-02-03 05:04:03.000000 hdcms-bindings-0.1.4/hdcms-c/src/main.c
--rw-r--r--   0 jason      (502) staff       (20)       48 2023-02-03 05:04:03.000000 hdcms-bindings-0.1.4/hdcms-c/src/main.h
-drwxr-xr-x   0 jason      (502) staff       (20)        0 2023-02-03 06:09:59.438476 hdcms-bindings-0.1.4/hdcms-c/src/util/
--rw-r--r--   0 jason      (502) staff       (20)    20466 2023-02-03 05:04:03.000000 hdcms-bindings-0.1.4/hdcms-c/src/util/array.c
--rw-r--r--   0 jason      (502) staff       (20)     9150 2023-02-03 05:04:03.000000 hdcms-bindings-0.1.4/hdcms-c/src/util/array.h
--rw-r--r--   0 jason      (502) staff       (20)     3802 2023-02-03 05:04:03.000000 hdcms-bindings-0.1.4/hdcms-c/src/util/bin.c
--rw-r--r--   0 jason      (502) staff       (20)     2756 2023-02-03 05:04:03.000000 hdcms-bindings-0.1.4/hdcms-c/src/util/bin.h
--rw-r--r--   0 jason      (502) staff       (20)     6815 2023-02-03 05:04:03.000000 hdcms-bindings-0.1.4/hdcms-c/src/util/peak.c
--rw-r--r--   0 jason      (502) staff       (20)     5518 2023-02-03 05:04:03.000000 hdcms-bindings-0.1.4/hdcms-c/src/util/peak.h
-drwxr-xr-x   0 jason      (502) staff       (20)        0 2023-02-03 06:09:59.439149 hdcms-bindings-0.1.4/hdcms_bindings.egg-info/
--rw-r--r--   0 jason      (502) staff       (20)     5446 2023-02-03 06:09:59.000000 hdcms-bindings-0.1.4/hdcms_bindings.egg-info/PKG-INFO
--rw-r--r--   0 jason      (502) staff       (20)      421 2023-02-03 06:09:59.000000 hdcms-bindings-0.1.4/hdcms_bindings.egg-info/SOURCES.txt
--rw-r--r--   0 jason      (502) staff       (20)        1 2023-02-03 06:09:59.000000 hdcms-bindings-0.1.4/hdcms_bindings.egg-info/dependency_links.txt
--rw-r--r--   0 jason      (502) staff       (20)       15 2023-02-03 06:09:59.000000 hdcms-bindings-0.1.4/hdcms_bindings.egg-info/top_level.txt
--rw-r--r--   0 jason      (502) staff       (20)      538 2023-02-03 06:08:31.000000 hdcms-bindings-0.1.4/pyproject.toml
--rw-r--r--   0 jason      (502) staff       (20)     8975 2023-02-03 06:05:56.000000 hdcms-bindings-0.1.4/python.c
--rw-r--r--   0 jason      (502) staff       (20)       38 2023-02-03 06:09:59.439588 hdcms-bindings-0.1.4/setup.cfg
--rw-r--r--   0 jason      (502) staff       (20)      590 2023-02-03 06:07:14.000000 hdcms-bindings-0.1.4/setup.py
+drwxr-xr-x   0 jason      (502) staff       (20)        0 2023-06-20 08:57:22.225489 hdcms-bindings-0.1.5/
+-rw-r--r--   0 jason      (502) staff       (20)     1830 2023-01-22 19:56:08.000000 hdcms-bindings-0.1.5/LICENSE
+-rw-r--r--   0 jason      (502) staff       (20)      146 2023-02-03 06:05:56.000000 hdcms-bindings-0.1.5/MANIFEST.in
+-rw-r--r--   0 jason      (502) staff       (20)     5514 2023-06-20 08:57:22.225317 hdcms-bindings-0.1.5/PKG-INFO
+-rw-r--r--   0 jason      (502) staff       (20)     3037 2023-06-20 08:56:33.000000 hdcms-bindings-0.1.5/README.md
+drwxr-xr-x   0 jason      (502) staff       (20)        0 2023-06-20 08:57:22.222332 hdcms-bindings-0.1.5/hdcms-c/
+drwxr-xr-x   0 jason      (502) staff       (20)        0 2023-06-20 08:57:22.223699 hdcms-bindings-0.1.5/hdcms-c/src/
+-rw-r--r--   0 jason      (502) staff       (20)      882 2023-02-03 05:04:03.000000 hdcms-bindings-0.1.5/hdcms-c/src/fixwindows.h
+-rw-r--r--   0 jason      (502) staff       (20)    10239 2023-06-18 17:14:08.000000 hdcms-bindings-0.1.5/hdcms-c/src/main.c
+-rw-r--r--   0 jason      (502) staff       (20)       48 2023-02-03 05:04:03.000000 hdcms-bindings-0.1.5/hdcms-c/src/main.h
+drwxr-xr-x   0 jason      (502) staff       (20)        0 2023-06-20 08:57:22.224525 hdcms-bindings-0.1.5/hdcms-c/src/util/
+-rw-r--r--   0 jason      (502) staff       (20)    20530 2023-06-20 08:03:24.000000 hdcms-bindings-0.1.5/hdcms-c/src/util/array.c
+-rw-r--r--   0 jason      (502) staff       (20)     9226 2023-06-17 22:57:37.000000 hdcms-bindings-0.1.5/hdcms-c/src/util/array.h
+-rw-r--r--   0 jason      (502) staff       (20)     4318 2023-06-20 08:03:24.000000 hdcms-bindings-0.1.5/hdcms-c/src/util/bin.c
+-rw-r--r--   0 jason      (502) staff       (20)     2880 2023-06-18 17:14:08.000000 hdcms-bindings-0.1.5/hdcms-c/src/util/bin.h
+-rw-r--r--   0 jason      (502) staff       (20)     8646 2023-06-18 17:14:08.000000 hdcms-bindings-0.1.5/hdcms-c/src/util/peak.c
+-rw-r--r--   0 jason      (502) staff       (20)     5701 2023-06-17 22:57:37.000000 hdcms-bindings-0.1.5/hdcms-c/src/util/peak.h
+drwxr-xr-x   0 jason      (502) staff       (20)        0 2023-06-20 08:57:22.225144 hdcms-bindings-0.1.5/hdcms_bindings.egg-info/
+-rw-r--r--   0 jason      (502) staff       (20)     5514 2023-06-20 08:57:22.000000 hdcms-bindings-0.1.5/hdcms_bindings.egg-info/PKG-INFO
+-rw-r--r--   0 jason      (502) staff       (20)      421 2023-06-20 08:57:22.000000 hdcms-bindings-0.1.5/hdcms_bindings.egg-info/SOURCES.txt
+-rw-r--r--   0 jason      (502) staff       (20)        1 2023-06-20 08:57:22.000000 hdcms-bindings-0.1.5/hdcms_bindings.egg-info/dependency_links.txt
+-rw-r--r--   0 jason      (502) staff       (20)       15 2023-06-20 08:57:22.000000 hdcms-bindings-0.1.5/hdcms_bindings.egg-info/top_level.txt
+-rw-r--r--   0 jason      (502) staff       (20)      538 2023-06-20 08:56:42.000000 hdcms-bindings-0.1.5/pyproject.toml
+-rw-r--r--   0 jason      (502) staff       (20)     9415 2023-06-20 08:54:44.000000 hdcms-bindings-0.1.5/python.c
+-rw-r--r--   0 jason      (502) staff       (20)       38 2023-06-20 08:57:22.225528 hdcms-bindings-0.1.5/setup.cfg
+-rw-r--r--   0 jason      (502) staff       (20)      590 2023-02-03 06:07:14.000000 hdcms-bindings-0.1.5/setup.py
```

### Comparing `hdcms-bindings-0.1.4/LICENSE` & `hdcms-bindings-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hdcms-bindings-0.1.4/PKG-INFO` & `hdcms-bindings-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdcms-bindings
-Version: 0.1.4
+Version: 0.1.5
 Summary: This package wraps the C functions in hdcms
 Author: Arun Moorthy
 Author-email: Jason Eveleth <hdcms@jasoneveleth.com>
 License: NIST-developed software is provided by NIST as a public service. You may use,
         copy, and distribute copies of the software in any medium, provided that you
         keep intact this entire notice. You may improve, modify, and create derivative
         works of the software or any portion of the software, and you may copy and
@@ -87,14 +87,16 @@
 https://docs.python.org/3/extending/extending.html#building-arbitrary-values
 https://numpy.org/doc/stable/user/c-info.how-to-extend.html
 https://numpy.org/doc/stable/reference/c-api/array.html#c.PyArray_SimpleNew
 https://numpy.org/doc/stable/reference/c-api/dtype.html
 
 # Changelog
 
+0.1.5 Update start, stop, num_bins, and scaling for both 1d and 2d
+
 0.1.4 Rename package (setup.py has the import name, which must match the c lib symbols)
 
 0.1.3 Rename package for real for real
 
 0.1.2 Rename package for real (broken)
 
 0.1.1 Rename package (broken)
```

### Comparing `hdcms-bindings-0.1.4/README.md` & `hdcms-bindings-0.1.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,16 @@
 https://docs.python.org/3/extending/extending.html#building-arbitrary-values
 https://numpy.org/doc/stable/user/c-info.how-to-extend.html
 https://numpy.org/doc/stable/reference/c-api/array.html#c.PyArray_SimpleNew
 https://numpy.org/doc/stable/reference/c-api/dtype.html
 
 # Changelog
 
+0.1.5 Update start, stop, num_bins, and scaling for both 1d and 2d
+
 0.1.4 Rename package (setup.py has the import name, which must match the c lib symbols)
 
 0.1.3 Rename package for real for real
 
 0.1.2 Rename package for real (broken)
 
 0.1.1 Rename package (broken)
```

### Comparing `hdcms-bindings-0.1.4/hdcms-c/src/fixwindows.h` & `hdcms-bindings-0.1.5/hdcms-c/src/fixwindows.h`

 * *Files identical despite different names*

### Comparing `hdcms-bindings-0.1.4/hdcms-c/src/main.c` & `hdcms-bindings-0.1.5/hdcms-c/src/main.c`

 * *Files 2% similar despite different names*

```diff
@@ -74,36 +74,36 @@
         return false;
     }
     close(fd);
     return true;
 }
 
 static struct matrix
-filenames_to_stats(char *str, int mflag, double start, double end, double num_bins)
+filenames_to_stats(char *str, int mflag, double start, double end, double num_bins, char scaling)
 {
     struct matarray arr = matarr_zeros(2);
 
     char *path;
     size_t i;
     for (i = 0; (path = find_token(&str, " ,\n\t")); i++) {
         if ((size_t)i == arr.length) { // resize
             arr.length *= 2;
             arr.data = safe_realloc(arr.data, arr.length * sizeof(*arr.data));
         }
         struct matrix m = mat_from_file(path);
-        scaled_data(m); // this is redundant in TWOD since the data we are given is scaled
+        scaled_data(m, scaling);
         matarr_set(arr, i, m);
     }
     arr.length = i; // wastes some of the malloc'd mem but that's okay
     struct matrix stats;
     if (mflag == ONED) {
         stats = bin_stat_1D(arr, start, end, num_bins);
     } else if (mflag == TWOD) {
         size_t n = matarr_get(arr, 0).len1; // >= longest possible length
-        stats = peak_stat(arr, n);
+        stats = peak_stat(arr, n, inf);
     } else {
         printf("\n");
         usage();
     }
     matarr_free(arr);
     return stats;
 }
@@ -123,23 +123,23 @@
     rewind(fileptr);            // Jump back to the beginning of the file
 
     buffer = malloc(len + 1);            // Enough memory for the file (and NUL)
     fread(buffer, len, 1, fileptr);      // Read in the entire file
     fclose(fileptr);                     // Close the file
     buffer[len] = '\0';                  // NUL terminate the string
 
-    struct matrix stats = filenames_to_stats(buffer, mflag, 0, 900. * (8999. / 9000.), 9000.);
+    struct matrix stats = filenames_to_stats(buffer, mflag, 0, 900. * (8999. / 9000.), 9000., 'm');
     free(buffer);
     matarr_set(arr, i, stats);
 }
 
 static void
 list_option(char *str, struct matarray arr, const size_t i)
 {
-    struct matrix stats = filenames_to_stats(str, mflag, 0, 900. * (8999. / 9000.), 9000.);
+    struct matrix stats = filenames_to_stats(str, mflag, 0, 900. * (8999. / 9000.), 9000., 'm');
     matarr_set(arr, i, stats);
 }
 
 static void
 print_comparison(const struct matrix m)
 {
     printf("╭────┬");
```

### Comparing `hdcms-bindings-0.1.4/hdcms-c/src/util/array.c` & `hdcms-bindings-0.1.5/hdcms-c/src/util/array.c`

 * *Files 0% similar despite different names*

```diff
@@ -258,14 +258,15 @@
     if (v1.length != v2.length) {
         WARNING("incompatible vectors\n\tvec_equal %zdvs%zd\n", v1.length, v2.length);
         return false;
     }
     bool ret = true;
     for (size_t i = 0; i < v1.length; i++) {
         if (!equals(vec_get(v1, i), vec_get(v2, i))) {
+            printf("%g\n", vec_get(v1, i));
             ret = false;
         }
     }
     return ret;
 }
 
 double
@@ -766,19 +767,20 @@
 {
     return matarr_from_data(safe_calloc(len, sizeof(struct matrix)), len, true);
 }
 
 void
 matarr_free(struct matarray arr)
 {
-    for (size_t i = 0; i < arr.length; i++) {
-        mat_free(matarr_get(arr, i));
-    }
-    if (arr.is_owner)
+    if (arr.is_owner) {
+        for (size_t i = 0; i < arr.length; i++) {
+            mat_free(matarr_get(arr, i));
+        }
         free(arr.data);
+    }
 }
 
 void
 matarr_stats_printf(struct matarray arr)
 {
     for (size_t i = 0; i < arr.length; i++) {
         mat_stats_printf(matarr_get(arr, i));
```

### Comparing `hdcms-bindings-0.1.4/hdcms-c/src/util/array.h` & `hdcms-bindings-0.1.5/hdcms-c/src/util/array.h`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #define ARRAY_H
 #include "../fixwindows.h"
 #include <stdlib.h>
 #include <stdio.h>
 #include <stdint.h>
 #include <assert.h>
 #include <stdbool.h>
+#include <math.h>
 
 #if !defined(RED) || !defined(RESET)
 #define RED ""
 #define RESET ""
 #endif
 #define WARNING(fmt, ...) fprintf(stderr, "%s:%d: " RED "WARNING: " RESET fmt, __FILE__, __LINE__, __VA_ARGS__)
 
@@ -63,14 +64,17 @@
 };
 
 /* vec */
 // retrive element at index in the vector
 static inline double
 vec_get(const struct vec v, size_t i)
 {
+    if (i >= v.length) {
+        printf("oh no\n");
+    }
     assert(i < v.length && "trying to get an index outside bounds in vector");
     return v.data[v.stride * i];
 }
 // *mutates* element at index
 static inline void
 vec_set(struct vec v, size_t i, double a)
 {
```

### Comparing `hdcms-bindings-0.1.4/hdcms-c/src/util/bin.c` & `hdcms-bindings-0.1.5/hdcms-c/src/util/bin.c`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #include <stdbool.h>
 #include <math.h>
+#include "array.h"
 #include "bin.h"
 
 struct matrix 
 bin_stat_1D(const struct matarray A, double start, double end, double num_bins)
 {
     struct matrix M = mat_zeros(A.length, (size_t)num_bins);
     for (size_t i = 0; i < A.length; i++) {
@@ -55,31 +56,46 @@
     }
     return binary_search(bins, 0, bins.length - 1, val);
 }
 
 struct vec 
 spec_vec(const struct matrix m, double start, double end, double num_bins)
 {
-    struct vec t = vec_linspace(start, end, num_bins);
+    // +1 since linspace allocates a size $n$ array, but that's 1 less than the
+    // number of bins
+    struct vec t = vec_linspace(start, end, num_bins+1);
     struct vec v = vec_zeros((size_t)num_bins);
 
     for (size_t i = 0; i < m.len1; i++) {
         size_t i_max = get_bin(t, mat_get(m, i, 0));
         vec_set(v, i_max, mat_get(m, i, 1));
     }
     vec_free(t);
     return v;
 }
 
 void
-scaled_data(const struct matrix m)
+scaled_data(const struct matrix m, char type)
 {
-    struct vec v = vec_from_col(m, 1);
-    double max = vec_max(v);
-    vec_invscale(v, max);
+    if (type == 'm') {
+        // max
+        struct vec v = vec_from_col(m, 1);
+        double max = vec_max(v);
+        vec_invscale(v, max);
+    } else if (type == 'u') {
+        // unit
+        struct vec v = vec_from_col(m, 1);
+        double dot = vec_dot(v, v);
+        vec_invscale(v, sqrt(dot));
+    } else if (type == 'n') {
+        // no scaling
+        return;
+    } else {
+        WARNING("specified unimplemented scaling `%c`, must be: m, u, or n", type);
+    }
 }
 
 double 
 prob_dot_prod(const struct matrix u_orig, const struct matrix v_orig, double desingularization)
 {
     // input are nx2 matrices of (mean, std) pairs
     // assert input correct
```

### Comparing `hdcms-bindings-0.1.4/hdcms-c/src/util/bin.h` & `hdcms-bindings-0.1.5/hdcms-c/src/util/bin.h`

 * *Files 13% similar despite different names*

```diff
@@ -4,22 +4,25 @@
 #include "array.h"
 
 /* minimum of 2 and 3 size_t's respectively */
 size_t min2(const size_t x, const size_t y);
 size_t min3(const size_t x, const size_t y, const size_t z);
 
 /*
- * Scales input data (y-values) between 0 and 1
+ * Scales input data's y-values
  *
- * input: nx2 matrix of a spectra measurement coordinates
+ * input: nx2 matrix of a spectra measurement coordinates, char representing type
  * output: none
  *
  * Note: mutates the matrix in place.
+ * 'm' => scale so the max is 1
+ * 'n' => no scaling
+ * 'u' => unit scaling (turn it into a unit vector)
  */
-void scaled_data(const struct matrix m);
+void scaled_data(const struct matrix m, char type);
 
 /*
  * This function bins the spectra m (an array of (x,y) pairs) into bins
  *
  * inputs: nx2 matrix of spectra measurement coordinates
  * outputs: vector of the hieght of the spectra in bins
  *
```

### Comparing `hdcms-bindings-0.1.4/hdcms-c/src/util/peak.c` & `hdcms-bindings-0.1.5/hdcms-c/src/util/peak.c`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 #include <stdbool.h>
 #include <math.h>
+#include "array.h"
 #include "peak.h"
 
 size_t
 min2(const size_t x, const size_t y) 
 {
     return x < y ? x : y;
 }
 
 size_t
 min3(const size_t x, const size_t y, const size_t z) 
 {
     return min2(min2(x, y), z);
 }
 
+size_t
+max(size_t x, size_t y)
+{
+    return x < y ? y : x;
+}
+
 // (2 4xn matrices (output of `peak_stat`), number of peaks) -> similarity of them btwn 0 and 1
 double
 peak_sim_measure_L2(const struct matrix m1, const struct matrix m2, double desingularization, size_t n) 
 {
     n = min3(m1.len1, m2.len1, n);
     if (n == 0) {
         WARNING("%s\n", "peak_sim_measure_L2 one of the matrices has 0 length");
@@ -32,19 +39,38 @@
         struct vec m1_ys = vec_from_col(m1_copy, 1);
         struct vec m2_ys = vec_from_col(m2_copy, 1);
         size_t m1_argmax = vec_argmax(m1_ys);
         size_t m2_argmax = vec_argmax(m2_ys);
 
         struct matrix *matrix_without_max_peak_p;
         struct vec u; // peak with max y value
-        bool m1_has_larger_peak = mat_get(m1_copy, m1_argmax, 1) >= mat_get(m2_copy, m2_argmax, 1);
-        matrix_without_max_peak_p = m1_has_larger_peak ? &m2_copy : &m1_copy;
-        u = m1_has_larger_peak
-            ? vec_from_row(m1_copy, m1_argmax)
-            : vec_from_row(m2_copy, m2_argmax);
+        double m1_max_y = vec_get(m1_ys, m1_argmax);
+        double m2_max_y = vec_get(m2_ys, m2_argmax);
+        if (m1_max_y > m2_max_y) {
+            matrix_without_max_peak_p = &m2_copy;
+            u = vec_from_row(m1_copy, m1_argmax);
+        } else if (m1_max_y < m2_max_y) {
+            matrix_without_max_peak_p = &m1_copy;
+            u = vec_from_row(m2_copy, m2_argmax);
+        } else {
+            // equal, break tie with lexigraphic sort
+            size_t i = 0;
+            for (; vec_get(m1_ys, i) == vec_get(m2_ys, i); i++) {
+                if (i >= n - 1) {
+                    break;
+                }
+            }
+            if (mat_get(m1_copy, i, 1) > mat_get(m2_copy, i, 1)) {
+                matrix_without_max_peak_p = &m2_copy;
+                u = vec_from_row(m1_copy, m1_argmax);
+            } else {
+                matrix_without_max_peak_p = &m1_copy;
+                u = vec_from_row(m2_copy, m2_argmax);
+            }
+        }
 
         struct vec sim_scores = vec_zeros(matrix_without_max_peak_p->len1);
         for (size_t j = 0; j < matrix_without_max_peak_p->len1; j++) {
             struct vec v = vec_from_row(*matrix_without_max_peak_p, j);
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wfloat-equal"
             // this is oaky because we set it to be this
@@ -74,29 +100,24 @@
     vec_free(weighted_sum);
     vec_free(sum);
     return ret;
 }
 
 // (matrices of spectra, number of peaks) -> nx4 matrix of peaks
 struct matrix
-peak_stat(const struct matarray replicates, size_t n) 
+peak_stat(const struct matarray replicates, size_t n, double xtol) 
 {
     if (replicates.length <= 0) {
         WARNING("peak_stat got %zd length array\n", replicates.length);
         struct matrix m = {0, 0, 0, NULL, false};
         return m;
     }
 
-    // reset n
-    for (size_t i = 0; i < replicates.length; i++) {
-        n = min2(n, matarr_get(replicates, i).len1);
-    }
-
-    struct matrix B = mat_zeros(n, 4);
-    struct matarray P = peak_sort(replicates, n);
+    struct matarray P = peak_sort(replicates, n, xtol);
+    struct matrix B = mat_zeros(P.length, 4);
     for (size_t i = 0; i < P.length; i++) {
         struct matrix M = matarr_get(P, i);
         struct vec x = vec_from_col(M, 0);
         struct vec y = vec_from_col(M, 1);
         mat_set(B, i, 0, vec_mean(x));
         mat_set(B, i, 1, vec_mean(y));
         mat_set(B, i, 2, vec_std(x));
@@ -123,77 +144,116 @@
         WARNING("%s vec size not equal to 4 (maybe forgot to pass --1d)\n", __func__);
         exit(1);
         // unreachable
     }
 
     // add 1e-4 to all std, to avoid the 0 std div 0 error
     double v0 = vec_get(v, 0),        v1 = vec_get(v, 1),
-           v2 = vec_get(v, 2) + 1e-4, v3 = vec_get(v, 3) + 1e-4,
+           v2 = vec_get(v, 2) + desingularization, v3 = vec_get(v, 3) + desingularization,
            u0 = vec_get(u, 0),        u1 = vec_get(u, 1),
-           u2 = vec_get(u, 2) + 1e-4, u3 = vec_get(u, 3) + 1e-4;
+           u2 = vec_get(u, 2) + desingularization, u3 = vec_get(u, 3) + desingularization;
     double tmp2 = (2*u2*v2) / (u2*u2 + v2*v2);
     double tmp3 = (2*u3*v3) / (u3*u3 + v3*v3);
     double a = sqrt(tmp2) * sqrt(tmp3);
     double bx = (u0-v0) * (u0-v0) / (u2*u2 + v2*v2);
     double by = (u1-v1) * (u1-v1) / (u3*u3 + v3*v3);
     return a * exp(-0.5 * (bx + by));
 }
 
 // (matrices of spectra, number of peaks) -> n matrices s.t. ith matrix is the
 // pts assoc. with ith largest peak
 struct matarray
-peak_sort(const struct matarray replicates, size_t n)
+peak_sort(const struct matarray replicates, size_t n, double xtol)
 {
-    // reset n
-    for (size_t i = 0; i < replicates.length; i++) {
-        n = min2(n, matarr_get(replicates, i).len1);
+    struct matarray P = matarr_zeros(n);
+
+    // check for zero length matrices
+    for (size_t j = 0; j < replicates.length; j++) {
+        struct matrix mj = matarr_get(replicates, j);
+        if (mj.len2 == 0) {
+            WARNING("%s\n", "peak_sort given a matrix with dimension (<something>, 0)");
+            matarr_free(P);
+            return matarr_zeros(0);
+        }
     }
 
-    struct matarray P = matarr_zeros(n);
     struct matarray replicates_copy = matarr_copy(replicates);
-    for (size_t i = 0; i < n; i++) {
+
+    size_t i;
+    for (i = 0; i < n; i++) {
         // find largest point left in all replicates
         double maxy = -inf;
         double maxx = 0;
+        bool found_peak = false;
         for (size_t j = 0; j < replicates_copy.length; j++) {
             struct matrix mj = matarr_get(replicates_copy, j);
             struct vec ys = vec_from_col(mj, 1);
             size_t argmax = vec_argmax(ys);
             if (vec_get(ys, argmax) > maxy) {
                 maxx = mat_get(mj, argmax, 0);
                 maxy = mat_get(mj, argmax, 1);
+                found_peak = true;
             }
         }
 
+        // we've exhausted all replicates and there are no peaks left
+        if (!found_peak) {
+            break;
+        }
+
         // find points in replicates closest to p
-        struct matrix peak = mat_zeros(replicates_copy.length, 2);
+        struct matrix peak_points = mat_zeros(replicates_copy.length, 2);
         for (size_t j = 0; j < replicates_copy.length; j++) {
             struct matrix mj = matarr_get(replicates_copy, j);
+
+            // find closest pt in mj matrix (within xtol)
             double mindist = inf;
-            
-            // get closest pt in mj matrix
-            size_t rowargmin = 0;
+            size_t rowargmin = -1;
+            bool found = false;
             for (size_t row = 0; row < mj.len1; row++) {
+                if (fabs(mat_get(mj, row, 0) - maxx) > xtol) {
+                    continue;
+                }
                 double dx = maxx - mat_get(mj, row, 0);
                 double dy = maxy - mat_get(mj, row, 1);
                 double dist = dx*dx + dy*dy;
                 if (dist < mindist) {
+                    found = true;
                     rowargmin = row;
                     mindist = dist;
                 }
             }
 
-            // assign smallest point to peak mat
-            mat_set(peak, j, 0, mat_get(mj, rowargmin, 0));
-            mat_set(peak, j, 1, mat_get(mj, rowargmin, 1));
+            if (!found) {
+                mat_set(peak_points, j, 0, maxx);
+                mat_set(peak_points, j, 1, 0);
+            } else {
+                // assign closest point to peak
+                mat_set(peak_points, j, 0, mat_get(mj, rowargmin, 0));
+                mat_set(peak_points, j, 1, mat_get(mj, rowargmin, 1));
+
+                // set y value of the point to -inf so it never matches or is a max
+                mat_set(mj, rowargmin, 1, -inf);
+            }
 
-            // set y value of the point to -inf so it never matches or is a max
-            mat_set(mj, rowargmin, 1, -inf);
         }
 
-        // make the next peak a new matrix in P
-        matarr_set(P, i, peak);
+        // add the peak points to P
+        matarr_set(P, i, peak_points);
     }
+
+    // if we exhausted the replicates before we got n peaks, then make a smaller
+    // matarray
+    if (i != n) {
+        struct matarray a = matarr_zeros(i);
+        for (size_t j = 0; j < i; j++) {
+            matarr_set(a, j, matarr_get(P, j));
+        }
+        P.is_owner = false;
+        matarr_free(P);
+        P = a;
+    }
+
     matarr_free(replicates_copy);
     return P;
 }
```

### Comparing `hdcms-bindings-0.1.4/hdcms-c/src/util/peak.h` & `hdcms-bindings-0.1.5/hdcms-c/src/util/peak.h`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
  * output: the similarity of the two matrices
  *
  * The input matrices are generated by calls to `peak_stat`. The columns are
  * x_mean, y_mean, x_std, y_std. Keep in mind these matrices num_rows can be
  * greater than or less than `n`, and we will use the min of `m1.len2`, `m2.len2`,
  * and `n` as n moving forward. 
  *
- * The desingularization is the amount we add to the standard deviation to avoid
+ * The `desingularization` is the amount we add to the standard deviation to avoid
  * divide by 0 errors.
  *
  * We compare the most important (highest) peak in both matrices with all the
  * peaks in the other matrix. We select the best peak in the other matrix by
  * similarity. Repeat until n peaks have been matched. We use the similalrity
  * scores as the weights for a weighted average. We are calculating the weighted
  * average of the products of the y-values of matched peaks. We return that
@@ -97,26 +97,32 @@
  * find the nearest coordinate in the other replicates to it. We say that
  * collection of coordinates is a peak, and put it first into the list we will
  * return. We remove the coordinates we used, and repeat the process again. (We
  * don't actually remove the peak, since that would be expensive, rather we set
  * it's y-value to -inf so it is never the closest or highest peak again.)
  *
  * This is a helper routine for peak_stat.
+ *
+ * The `xtol` is the amount of distance in the x direction that we permit for
+ * being part of the same peak.
+ *
  */
-struct matarray peak_sort(const struct matarray replicates, size_t n);
+struct matarray peak_sort(const struct matarray replicates, size_t n, double xtol);
 
 /*
  * Creates the peak statistics matrix from a list of peaks.
  *
  * inputs: array of matrices of spectra
  *         number of peaks
  * outputs: nx4 matrix of the mean and standard deviations for x and y for each of the n peaks
  *
  * We call `peak_sort` to get a list of the coordinates of the peaks. Then we
  * find the mean of the x-values of the coordinates, mean of the y-values, std
  * of the x-values, std of the y-values. These are the 4 columns of the matrix
  * we are returning. The ith row of the matrix we return is the statistics for
  * the ith peak from the call to `peak_sort`.
+ *
+ * See abox for `xtol` description.
  */
-struct matrix peak_stat(const struct matarray replicates, size_t n);
+struct matrix peak_stat(const struct matarray replicates, size_t n, double xtol);
 
 #endif // PEAK_H
```

### Comparing `hdcms-bindings-0.1.4/hdcms_bindings.egg-info/PKG-INFO` & `hdcms-bindings-0.1.5/hdcms_bindings.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdcms-bindings
-Version: 0.1.4
+Version: 0.1.5
 Summary: This package wraps the C functions in hdcms
 Author: Arun Moorthy
 Author-email: Jason Eveleth <hdcms@jasoneveleth.com>
 License: NIST-developed software is provided by NIST as a public service. You may use,
         copy, and distribute copies of the software in any medium, provided that you
         keep intact this entire notice. You may improve, modify, and create derivative
         works of the software or any portion of the software, and you may copy and
@@ -87,14 +87,16 @@
 https://docs.python.org/3/extending/extending.html#building-arbitrary-values
 https://numpy.org/doc/stable/user/c-info.how-to-extend.html
 https://numpy.org/doc/stable/reference/c-api/array.html#c.PyArray_SimpleNew
 https://numpy.org/doc/stable/reference/c-api/dtype.html
 
 # Changelog
 
+0.1.5 Update start, stop, num_bins, and scaling for both 1d and 2d
+
 0.1.4 Rename package (setup.py has the import name, which must match the c lib symbols)
 
 0.1.3 Rename package for real for real
 
 0.1.2 Rename package for real (broken)
 
 0.1.1 Rename package (broken)
```

### Comparing `hdcms-bindings-0.1.4/pyproject.toml` & `hdcms-bindings-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "numpy", "toml"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hdcms-bindings"
-version = "0.1.4"
+version = "0.1.5"
 description = "This package wraps the C functions in hdcms"
 authors = [
     {name="Jason Eveleth", email="hdcms@jasoneveleth.com"},
     {name="Arun Moorthy"},
 ]
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `hdcms-bindings-0.1.4/python.c` & `hdcms-bindings-0.1.5/python.c`

 * *Files 5% similar despite different names*

```diff
@@ -72,56 +72,68 @@
     // data: m.data
     // flags: NPY_ARRAY_BEHAVED it's writable and aligned
     // NULL: this data is the object's, so no need to set a base pointer
     return PyArray_NewFromDescr(&PyArray_Type, descr, 2, dims, strides, m.data, NPY_ARRAY_BEHAVED, NULL);
 }
 
 static PyObject*
-filenames_to_stats_parse(PyObject *dummy, PyObject *args, PyObject *kwargs, int mflag)
+filenames_to_stats_1d_cfunc(PyObject *dummy, PyObject *args, PyObject *kwargs)
 {
     double start = 0, end = 899.90000000000009094947, num_bins = 9000;
 
-    static char *kwlist[] = {"filenames", "start", "end", "num_bins", NULL};
+    static char *kwlist[] = {"filenames", "start", "end", "num_bins", "scaling", NULL};
 
     const char *str;
-    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "s|ddd", kwlist, &str, &start, &end, &num_bins)) {
-        PyErr_SetString(PyExc_RuntimeError, "didn't reviece a string");
+    const char *scaling = "m";
+    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "s|ddds", kwlist, &str, &start, &end, &num_bins, &scaling)) {
+        PyErr_SetString(PyExc_RuntimeError, "failed to parse args (in C)");
         return NULL;
     }
 
     int len = strlen(str) + 1;
     char *copy = safe_calloc(len, 1);
     strncpy(copy, str, len);
-    struct matrix m = filenames_to_stats(copy, mflag, start, end, num_bins);
+    struct matrix m = filenames_to_stats(copy, ONED, start, end, num_bins, scaling[0]);
 
     assert(m.is_owner);
 
     return mat_to_pyobject(m);
 }
 
 static PyObject*
-filenames_to_stats_1d_cfunc(PyObject *dummy, PyObject *args, PyObject *kwargs)
-{
-    return filenames_to_stats_parse(dummy, args, kwargs, ONED);
-}
-
-static PyObject*
 filenames_to_stats_2d_cfunc(PyObject *dummy, PyObject *args, PyObject *kwargs)
 {
-    return filenames_to_stats_parse(dummy, args, kwargs, TWOD);
+    static char *kwlist[] = {"filenames", "scaling", NULL};
+
+    const char *str;
+    const char *scaling = "m";
+    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "s|s", kwlist, &str, &scaling)) {
+        PyErr_SetString(PyExc_RuntimeError, "failed to parse args (in C)");
+        return NULL;
+    }
+
+    int len = strlen(str) + 1;
+    char *copy = safe_calloc(len, 1);
+    strncpy(copy, str, len);
+    // we can pass dummy values since they will be singored by the mflag
+    struct matrix m = filenames_to_stats(copy, TWOD, 0, 0, 0, scaling[0]);
+
+    assert(m.is_owner);
+
+    return mat_to_pyobject(m);
 }
 
 static PyObject*
 compare_compound_parse(PyObject *dummy, PyObject *args, PyObject *kwargs, int mflag)
 {
     PyObject *arg1, *arg2;
     double desingularization = 1e-4;
-    size_t max_peaks = -1;
+    long int max_peaks = -1;
     static char *kwlist[] = {"x1", "x2", "desingularization", "max_peaks", NULL};
-    if (!PyArg_ParseTupleAndKeywords(args, kwargs,  "O!O!|dk", kwlist, &PyArray_Type, &arg1, &PyArray_Type, &arg2, &desingularization, &max_peaks)) {
+    if (!PyArg_ParseTupleAndKeywords(args, kwargs,  "O!O!|dl", kwlist, &PyArray_Type, &arg1, &PyArray_Type, &arg2, &desingularization, &max_peaks)) {
         PyErr_SetString(PyExc_RuntimeError, "didn't recieve arrays");
         return NULL;
     }
 
     if (!is_pyobject_a_matrix(arg1) || !is_pyobject_a_matrix(arg2)) {
         return NULL;
     }
@@ -163,18 +175,18 @@
 
 static PyObject*
 compare_all_parse(PyObject *dummy, PyObject *args, PyObject *kwargs, int mflag)
 {
     PyObject *obj;
 
     double desingularization = 1e-4;
-    size_t max_peaks = -1;
+    long int max_peaks = -1;
     static char *kwlist[] = {"x", "desingularization", "max_peaks", NULL};
 
-    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "O|dk", kwlist, &obj, &desingularization, &max_peaks)) {
+    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "O|dl", kwlist, &obj, &desingularization, &max_peaks)) {
         PyErr_SetString(PyExc_RuntimeError, "didn't recieve an object");
         return NULL;
     }
 
     PyObject *seq;
     const char *mes = "didn't get iterable/list/ndarray";
     if ((seq = PySequence_Fast(obj, mes)) == NULL) {
```

### Comparing `hdcms-bindings-0.1.4/setup.py` & `hdcms-bindings-0.1.5/setup.py`

 * *Files identical despite different names*

