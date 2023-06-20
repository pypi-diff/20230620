# Comparing `tmp/arkit-1.1.2-cp311-cp311-win_amd64.whl.zip` & `tmp/arkit-2.0.0-cp311-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,12 @@
-Zip file size: 58061 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat     1080 b- defN 23-Feb-28 14:56 arkit-1.1.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      955 b- defN 23-Feb-28 14:56 arkit-1.1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat      102 b- defN 23-Feb-28 14:56 arkit-1.1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       86 b- defN 23-Feb-28 14:56 arkit-1.1.2.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        1 b- defN 23-Feb-28 14:56 arkit-1.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      468 b- defN 23-Feb-28 14:56 arkit-1.1.2.dist-info/RECORD
--rw-rw-rw-  2.0 fat    20480 b- defN 23-Feb-28 14:56 arkit/__init__.pyd
--rw-rw-rw-  2.0 fat   103936 b- defN 23-Feb-28 14:56 arkit/builder.pyd
-8 files, 127108 bytes uncompressed, 56987 bytes compressed:  55.2%
+Zip file size: 107772 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat     1080 b- defN 23-Jun-20 06:55 arkit-2.0.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2290 b- defN 23-Jun-20 06:55 arkit-2.0.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-20 06:55 arkit-2.0.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       40 b- defN 23-Jun-20 06:55 arkit-2.0.0.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        1 b- defN 23-Jun-20 06:55 arkit-2.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      469 b- defN 23-Jun-20 06:55 arkit-2.0.0.dist-info/RECORD
+-rw-rw-rw-  2.0 fat    52736 b- defN 23-Jun-20 06:55 arkit/__init__.pyd
+-rw-rw-rw-  2.0 fat    58880 b- defN 23-Jun-20 06:55 arkit/compiler.pyd
+-rw-rw-rw-  2.0 fat    68608 b- defN 23-Jun-20 06:55 arkit/pyproject.pyd
+-rw-rw-rw-  2.0 fat    52224 b- defN 23-Jun-20 06:55 arkit/wheeler.pyd
+10 files, 236428 bytes uncompressed, 106472 bytes compressed:  55.0%
```

## zipnote {}

```diff
@@ -1,25 +1,31 @@
-Filename: arkit-1.1.2.dist-info/LICENSE
+Filename: arkit-2.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: arkit-1.1.2.dist-info/METADATA
+Filename: arkit-2.0.0.dist-info/METADATA
 Comment: 
 
-Filename: arkit-1.1.2.dist-info/WHEEL
+Filename: arkit-2.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: arkit-1.1.2.dist-info/entry_points.txt
+Filename: arkit-2.0.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: arkit-1.1.2.dist-info/top_level.txt
+Filename: arkit-2.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: arkit-1.1.2.dist-info/RECORD
+Filename: arkit-2.0.0.dist-info/RECORD
 Comment: 
 
 Filename: arkit/__init__.pyd
 Comment: 
 
-Filename: arkit/builder.pyd
+Filename: arkit/compiler.pyd
+Comment: 
+
+Filename: arkit/pyproject.pyd
+Comment: 
+
+Filename: arkit/wheeler.pyd
 Comment: 
 
 Zip file comment:
```

## Comparing `arkit-1.1.2.dist-info/LICENSE` & `arkit-2.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

