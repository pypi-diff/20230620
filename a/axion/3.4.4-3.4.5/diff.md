# Comparing `tmp/axion-3.4.4-cp311-cp311-win_amd64.whl.zip` & `tmp/axion-3.4.5-cp311-none-macosx_10_9_universal2.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 623708 bytes, number of entries: 20
--rw-rw-rw-  2.0 fat     1080 b- defN 23-Jun-08 15:33 axion-3.4.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1288 b- defN 23-Jun-08 15:33 axion-3.4.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat      102 b- defN 23-Jun-08 15:33 axion-3.4.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 23-Jun-08 15:33 axion-3.4.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      376 b- defN 23-Jun-08 15:33 axion-3.4.4.dist-info/RECORD
--rw-rw-rw-  2.0 fat    20992 b- defN 23-Jun-08 15:33 axion/__init__.pyd
--rw-rw-rw-  2.0 fat    80384 b- defN 23-Jun-08 15:33 axion/executor.pyd
--rw-rw-rw-  2.0 fat   261632 b- defN 23-Jun-08 15:33 axion/factory.pyd
--rw-rw-rw-  2.0 fat    78848 b- defN 23-Jun-08 15:33 axion/pipeline.pyd
--rw-rw-rw-  2.0 fat    53248 b- defN 23-Jun-08 15:33 axion/queues.pyd
--rw-rw-rw-  2.0 fat   208384 b- defN 23-Jun-08 15:33 axion/recorder.pyd
--rw-rw-rw-  2.0 fat    56320 b- defN 23-Jun-08 15:33 axion/scheduler.pyd
--rw-rw-rw-  2.0 fat    71168 b- defN 23-Jun-08 15:33 axion/service.pyd
--rw-rw-rw-  2.0 fat    62464 b- defN 23-Jun-08 15:33 axion/thread.pyd
--rw-rw-rw-  2.0 fat    22016 b- defN 23-Jun-08 15:33 axion/inst/__init__.pyd
--rw-rw-rw-  2.0 fat    49664 b- defN 23-Jun-08 15:33 axion/inst/ibase.pyd
--rw-rw-rw-  2.0 fat   221696 b- defN 23-Jun-08 15:33 axion/inst/nbase.pyd
--rw-rw-rw-  2.0 fat    88064 b- defN 23-Jun-08 15:33 axion/inst/sbase.pyd
--rw-rw-rw-  2.0 fat    63488 b- defN 23-Jun-08 15:33 axion/inst/tbase.pyd
--rw-rw-rw-  2.0 fat    61440 b- defN 23-Jun-08 15:33 axion/inst/utility.pyd
-20 files, 1402655 bytes uncompressed, 621304 bytes compressed:  55.7%
+Zip file size: 1474816 bytes, number of entries: 20
+-rw-r--r--  2.0 unx     1059 b- defN 23-Jun-19 23:08 axion-3.4.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2362 b- defN 23-Jun-19 23:08 axion-3.4.5.dist-info/METADATA
+-rw-r--r--  2.0 unx      113 b- defN 23-Jun-19 23:08 axion-3.4.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-19 23:08 axion-3.4.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      376 b- defN 23-Jun-19 23:08 axion-3.4.5.dist-info/RECORD
+-rwxr-xr-x  2.0 unx   122763 b- defN 23-Jun-19 23:07 axion/__init__.so
+-rwxr-xr-x  2.0 unx   308955 b- defN 23-Jun-19 23:07 axion/executor.so
+-rwxr-xr-x  2.0 unx   863306 b- defN 23-Jun-19 23:07 axion/factory.so
+-rwxr-xr-x  2.0 unx   292267 b- defN 23-Jun-19 23:07 axion/pipeline.so
+-rwxr-xr-x  2.0 unx   219465 b- defN 23-Jun-19 23:07 axion/queues.so
+-rwxr-xr-x  2.0 unx   731275 b- defN 23-Jun-19 23:07 axion/recorder.so
+-rwxr-xr-x  2.0 unx   220716 b- defN 23-Jun-19 23:07 axion/scheduler.so
+-rwxr-xr-x  2.0 unx   275242 b- defN 23-Jun-19 23:07 axion/service.so
+-rwxr-xr-x  2.0 unx   238473 b- defN 23-Jun-19 23:07 axion/thread.so
+-rwxr-xr-x  2.0 unx   122907 b- defN 23-Jun-19 23:07 axion/inst/__init__.so
+-rwxr-xr-x  2.0 unx   217992 b- defN 23-Jun-19 23:07 axion/inst/ibase.so
+-rwxr-xr-x  2.0 unx   733160 b- defN 23-Jun-19 23:07 axion/inst/nbase.so
+-rwxr-xr-x  2.0 unx   329192 b- defN 23-Jun-19 23:07 axion/inst/sbase.so
+-rwxr-xr-x  2.0 unx   240760 b- defN 23-Jun-19 23:08 axion/inst/tbase.so
+-rwxr-xr-x  2.0 unx   238810 b- defN 23-Jun-19 23:07 axion/inst/utility.so
+20 files, 5159194 bytes uncompressed, 1472442 bytes compressed:  71.5%
```

## zipnote {}

```diff
@@ -1,61 +1,61 @@
-Filename: axion-3.4.4.dist-info/LICENSE
+Filename: axion-3.4.5.dist-info/LICENSE
 Comment: 
 
-Filename: axion-3.4.4.dist-info/METADATA
+Filename: axion-3.4.5.dist-info/METADATA
 Comment: 
 
-Filename: axion-3.4.4.dist-info/WHEEL
+Filename: axion-3.4.5.dist-info/WHEEL
 Comment: 
 
-Filename: axion-3.4.4.dist-info/top_level.txt
+Filename: axion-3.4.5.dist-info/top_level.txt
 Comment: 
 
-Filename: axion-3.4.4.dist-info/RECORD
+Filename: axion-3.4.5.dist-info/RECORD
 Comment: 
 
-Filename: axion/__init__.pyd
+Filename: axion/__init__.so
 Comment: 
 
-Filename: axion/executor.pyd
+Filename: axion/executor.so
 Comment: 
 
-Filename: axion/factory.pyd
+Filename: axion/factory.so
 Comment: 
 
-Filename: axion/pipeline.pyd
+Filename: axion/pipeline.so
 Comment: 
 
-Filename: axion/queues.pyd
+Filename: axion/queues.so
 Comment: 
 
-Filename: axion/recorder.pyd
+Filename: axion/recorder.so
 Comment: 
 
-Filename: axion/scheduler.pyd
+Filename: axion/scheduler.so
 Comment: 
 
-Filename: axion/service.pyd
+Filename: axion/service.so
 Comment: 
 
-Filename: axion/thread.pyd
+Filename: axion/thread.so
 Comment: 
 
-Filename: axion/inst/__init__.pyd
+Filename: axion/inst/__init__.so
 Comment: 
 
-Filename: axion/inst/ibase.pyd
+Filename: axion/inst/ibase.so
 Comment: 
 
-Filename: axion/inst/nbase.pyd
+Filename: axion/inst/nbase.so
 Comment: 
 
-Filename: axion/inst/sbase.pyd
+Filename: axion/inst/sbase.so
 Comment: 
 
-Filename: axion/inst/tbase.pyd
+Filename: axion/inst/tbase.so
 Comment: 
 
-Filename: axion/inst/utility.pyd
+Filename: axion/inst/utility.so
 Comment: 
 
 Zip file comment:
```

