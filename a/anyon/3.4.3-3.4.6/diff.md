# Comparing `tmp/anyon-3.4.3-cp311-cp311-win_amd64.whl.zip` & `tmp/anyon-3.4.6-cp311-none-macosx_10_9_universal2.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 368699 bytes, number of entries: 14
--rw-rw-rw-  2.0 fat     1080 b- defN 23-Jun-08 07:09 anyon-3.4.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1191 b- defN 23-Jun-08 07:09 anyon-3.4.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat      102 b- defN 23-Jun-08 07:09 anyon-3.4.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 23-Jun-08 07:09 anyon-3.4.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      376 b- defN 23-Jun-08 07:09 anyon-3.4.3.dist-info/RECORD
--rw-rw-rw-  2.0 fat    20480 b- defN 23-Jun-08 07:09 anyon/__init__.pyd
--rw-rw-rw-  2.0 fat    82432 b- defN 23-Jun-08 07:09 anyon/loader.pyd
--rw-rw-rw-  2.0 fat    99840 b- defN 23-Jun-08 07:09 anyon/remote.pyd
--rw-rw-rw-  2.0 fat   178688 b- defN 23-Jun-08 07:09 anyon/server.pyd
--rw-rw-rw-  2.0 fat    20992 b- defN 23-Jun-08 07:09 anyon/stage/__init__.pyd
--rw-rw-rw-  2.0 fat    92672 b- defN 23-Jun-08 07:09 anyon/stage/calculator.pyd
--rw-rw-rw-  2.0 fat   134144 b- defN 23-Jun-08 07:09 anyon/stage/compiler.pyd
--rw-rw-rw-  2.0 fat    61952 b- defN 23-Jun-08 07:09 anyon/stage/demodulator.pyd
--rw-rw-rw-  2.0 fat   114688 b- defN 23-Jun-08 07:09 anyon/stage/device.pyd
-14 files, 808638 bytes uncompressed, 366937 bytes compressed:  54.6%
+Zip file size: 838259 bytes, number of entries: 14
+-rw-r--r--  2.0 unx     1059 b- defN 23-Jun-19 23:49 anyon-3.4.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-19 23:49 anyon-3.4.6.dist-info/METADATA
+-rw-r--r--  2.0 unx      113 b- defN 23-Jun-19 23:49 anyon-3.4.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-19 23:49 anyon-3.4.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      376 b- defN 23-Jun-19 23:49 anyon-3.4.6.dist-info/RECORD
+-rwxr-xr-x  2.0 unx   122299 b- defN 23-Jun-19 23:49 anyon/__init__.so
+-rwxr-xr-x  2.0 unx   325801 b- defN 23-Jun-19 23:49 anyon/loader.so
+-rwxr-xr-x  2.0 unx   364057 b- defN 23-Jun-19 23:49 anyon/remote.so
+-rwxr-xr-x  2.0 unx   522473 b- defN 23-Jun-19 23:49 anyon/server.so
+-rwxr-xr-x  2.0 unx   122683 b- defN 23-Jun-19 23:49 anyon/stage/__init__.so
+-rwxr-xr-x  2.0 unx   328381 b- defN 23-Jun-19 23:49 anyon/stage/calculator.so
+-rwxr-xr-x  2.0 unx   475851 b- defN 23-Jun-19 23:49 anyon/stage/compiler.so
+-rwxr-xr-x  2.0 unx   240206 b- defN 23-Jun-19 23:49 anyon/stage/demodulator.so
+-rwxr-xr-x  2.0 unx   396377 b- defN 23-Jun-19 23:49 anyon/stage/device.so
+14 files, 2901945 bytes uncompressed, 836515 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -1,43 +1,43 @@
-Filename: anyon-3.4.3.dist-info/LICENSE
+Filename: anyon-3.4.6.dist-info/LICENSE
 Comment: 
 
-Filename: anyon-3.4.3.dist-info/METADATA
+Filename: anyon-3.4.6.dist-info/METADATA
 Comment: 
 
-Filename: anyon-3.4.3.dist-info/WHEEL
+Filename: anyon-3.4.6.dist-info/WHEEL
 Comment: 
 
-Filename: anyon-3.4.3.dist-info/top_level.txt
+Filename: anyon-3.4.6.dist-info/top_level.txt
 Comment: 
 
-Filename: anyon-3.4.3.dist-info/RECORD
+Filename: anyon-3.4.6.dist-info/RECORD
 Comment: 
 
-Filename: anyon/__init__.pyd
+Filename: anyon/__init__.so
 Comment: 
 
-Filename: anyon/loader.pyd
+Filename: anyon/loader.so
 Comment: 
 
-Filename: anyon/remote.pyd
+Filename: anyon/remote.so
 Comment: 
 
-Filename: anyon/server.pyd
+Filename: anyon/server.so
 Comment: 
 
-Filename: anyon/stage/__init__.pyd
+Filename: anyon/stage/__init__.so
 Comment: 
 
-Filename: anyon/stage/calculator.pyd
+Filename: anyon/stage/calculator.so
 Comment: 
 
-Filename: anyon/stage/compiler.pyd
+Filename: anyon/stage/compiler.so
 Comment: 
 
-Filename: anyon/stage/demodulator.pyd
+Filename: anyon/stage/demodulator.so
 Comment: 
 
-Filename: anyon/stage/device.pyd
+Filename: anyon/stage/device.so
 Comment: 
 
 Zip file comment:
```

