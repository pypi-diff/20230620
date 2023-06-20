# Comparing `tmp/numpysane-0.8.tar.gz` & `tmp/numpysane-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/numpysane-0.8.tar", last modified: Fri Apr 28 20:16:32 2017, max compression
+gzip compressed data, was "dist/numpysane-0.9.tar", last modified: Fri Jul 21 22:12:38 2017, max compression
```

## Comparing `numpysane-0.8.tar` & `numpysane-0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2017-04-28 20:16:32.000000 numpysane-0.8/
--rwxr-xr-x   0 dima      (1000) dima      (1000)    62370 2017-04-28 19:25:35.000000 numpysane-0.8/numpysane.py
--rw-r--r--   0 dima      (1000) dima      (1000)       59 2017-04-28 20:16:32.000000 numpysane-0.8/setup.cfg
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2017-04-28 20:16:32.000000 numpysane-0.8/numpysane.egg-info/
--rw-r--r--   0 dima      (1000) dima      (1000)        6 2017-04-28 20:16:32.000000 numpysane-0.8/numpysane.egg-info/requires.txt
--rw-r--r--   0 dima      (1000) dima      (1000)      222 2017-04-28 20:16:32.000000 numpysane-0.8/numpysane.egg-info/SOURCES.txt
--rw-r--r--   0 dima      (1000) dima      (1000)      366 2017-04-28 20:16:32.000000 numpysane-0.8/numpysane.egg-info/PKG-INFO
--rw-r--r--   0 dima      (1000) dima      (1000)        1 2017-04-28 20:16:32.000000 numpysane-0.8/numpysane.egg-info/dependency_links.txt
--rw-r--r--   0 dima      (1000) dima      (1000)       10 2017-04-28 20:16:32.000000 numpysane-0.8/numpysane.egg-info/top_level.txt
--rw-r--r--   0 dima      (1000) dima      (1000)    44602 2017-04-28 20:07:38.000000 numpysane-0.8/README
--rwxr-xr-x   0 dima      (1000) dima      (1000)      599 2017-04-28 20:08:52.000000 numpysane-0.8/setup.py
--rwxr-xr-x   0 dima      (1000) dima      (1000)    32356 2017-04-28 20:04:49.000000 numpysane-0.8/test_numpysane.py
--rw-r--r--   0 dima      (1000) dima      (1000)       41 2016-05-24 07:54:15.000000 numpysane-0.8/MANIFEST.in
--rw-r--r--   0 dima      (1000) dima      (1000)      366 2017-04-28 20:16:32.000000 numpysane-0.8/PKG-INFO
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2017-07-21 22:12:38.000000 numpysane-0.9/
+-rwxr-xr-x   0 dima      (1000) dima      (1000)    62615 2017-07-21 22:06:36.000000 numpysane-0.9/numpysane.py
+-rw-r--r--   0 dima      (1000) dima      (1000)       59 2017-07-21 22:12:38.000000 numpysane-0.9/setup.cfg
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2017-07-21 22:12:38.000000 numpysane-0.9/numpysane.egg-info/
+-rw-r--r--   0 dima      (1000) dima      (1000)        6 2017-07-21 22:12:38.000000 numpysane-0.9/numpysane.egg-info/requires.txt
+-rw-r--r--   0 dima      (1000) dima      (1000)      222 2017-07-21 22:12:38.000000 numpysane-0.9/numpysane.egg-info/SOURCES.txt
+-rw-r--r--   0 dima      (1000) dima      (1000)      366 2017-07-21 22:12:38.000000 numpysane-0.9/numpysane.egg-info/PKG-INFO
+-rw-r--r--   0 dima      (1000) dima      (1000)        1 2017-07-21 22:12:38.000000 numpysane-0.9/numpysane.egg-info/dependency_links.txt
+-rw-r--r--   0 dima      (1000) dima      (1000)       10 2017-07-21 22:12:38.000000 numpysane-0.9/numpysane.egg-info/top_level.txt
+-rw-r--r--   0 dima      (1000) dima      (1000)    44602 2017-04-28 20:07:38.000000 numpysane-0.9/README
+-rwxr-xr-x   0 dima      (1000) dima      (1000)      599 2017-07-21 22:06:36.000000 numpysane-0.9/setup.py
+-rwxr-xr-x   0 dima      (1000) dima      (1000)    32895 2017-07-21 22:06:36.000000 numpysane-0.9/test_numpysane.py
+-rw-r--r--   0 dima      (1000) dima      (1000)       41 2016-05-24 07:54:15.000000 numpysane-0.9/MANIFEST.in
+-rw-r--r--   0 dima      (1000) dima      (1000)      366 2017-07-21 22:12:38.000000 numpysane-0.9/PKG-INFO
```

### Comparing `numpysane-0.8/numpysane.py` & `numpysane-0.9/numpysane.py`

 * *Files 1% similar despite different names*

```diff
@@ -1122,14 +1122,19 @@
         >>> row
         array([1000, 1001, 1002])
 
         >>> nps.glue(a,b, axis=-1)
         array([[  0,   1,   2, 100, 101, 102],
                [  3,   4,   5, 103, 104, 105]])
 
+        # empty arrays ignored when glueing. Useful for initializing an accumulation
+        >>> nps.glue(a,b, np.array(()), axis=-1)
+        array([[  0,   1,   2, 100, 101, 102],
+               [  3,   4,   5, 103, 104, 105]])
+
         >>> nps.glue(a,b,row, axis=-2)
         array([[   0,    1,    2],
                [   3,    4,    5],
                [ 100,  101,  102],
                [ 103,  104,  105],
                [1000, 1001, 1002]])
 
@@ -1240,15 +1245,15 @@
     # target dimension count
     if max_ndim < -axis:
         max_ndim = -axis
 
     # Now I add dummy dimensions at the front of each array, to bring the source
     # arrays to the same dimensionality. After this is done, ndims for all the
     # matrices will be the same, and np.concatenate() should know what to do.
-    args = [ x[(np.newaxis,)*(max_ndim - x.ndim) + (Ellipsis,)] for x in args ]
+    args = [ x[(np.newaxis,)*(max_ndim - x.ndim) + (Ellipsis,)] for x in args if x.size != 0 ]
 
     return np.concatenate( args, axis=axis )
 
 
 def cat(*args):
     r'''Concatenates a given list of arrays along a new first (outer) dimension.
```

### Comparing `numpysane-0.8/README` & `numpysane-0.9/README`

 * *Files identical despite different names*

### Comparing `numpysane-0.8/setup.py` & `numpysane-0.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/python
 
 from setuptools import setup
 
 setup(name         = 'numpysane',
-      version      = '0.8',
+      version      = '0.9',
       author       = 'Dima Kogan',
       author_email = 'dima@secretsauce.net',
       url          = 'http://github.com/dkogan/numpysane',
       description  = 'more-reasonable core functionality for numpy',
 
       long_description = """numpysane is a collection of core routines to provide basic numpy
 functionality in a more reasonable way""",
```

### Comparing `numpysane-0.8/test_numpysane.py` & `numpysane-0.9/test_numpysane.py`

 * *Files 4% similar despite different names*

```diff
@@ -464,14 +464,21 @@
 
         self.assertError(                       nps.glue, arr(1,3), arr(2,3), axis=-1 )
         self.assertValueShape( None, (3,3),     nps.glue, arr(1,3), arr(2,3), axis=-2 )
         self.assertError(                       nps.glue, arr(1,3), arr(2,3), axis=-3 )
         self.assertError(                       nps.glue, arr(1,3), arr(2,3), axis=-4 )
         self.assertError(                       nps.cat,  arr(1,3), arr(2,3) )
 
+        # empty arrays are accepted and ignored
+        self.assertValueShape( None, (2,3),     nps.glue, np.array(()), arr(2,3),     axis=-2 )
+        self.assertValueShape( None, (1,2,3),   nps.glue, np.array(()), arr(2,3),     axis=-3 )
+        self.assertValueShape( None, (3,),      nps.glue, arr(3),       np.array(()), axis=-1 )
+        self.assertValueShape( None, (1,3),     nps.glue, arr(3),       np.array(()), axis=-2 )
+        self.assertValueShape( None, (3,3),     nps.glue, arr(3),       arr(2,3), np.array(()), axis=-2 )
+
     def test_dimension_manipulation(self):
         r'''Checking the various functions that manipulate dimensions.'''
 
         self.assertError     (                    nps.clump,        arr(2,3,4), n=-1 )
         self.assertValueShape( None, (2,3,4),     nps.clump,        arr(2,3,4), n=0 )
         self.assertValueShape( None, (2,3,4),     nps.clump,        arr(2,3,4), n=1 )
         self.assertValueShape( None, (2,12),      nps.clump,        arr(2,3,4), n=2 )
```

