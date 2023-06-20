# Comparing `tmp/algokit_utils-1.3.0-py3-none-any.whl.zip` & `tmp/algokit_utils-1.3.0b1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 36677 bytes, number of entries: 16
+Zip file size: 36703 bytes, number of entries: 16
 -rw-r--r--  2.0 unx     4159 b- defN 80-Jan-01 00:00 algokit_utils/__init__.py
 -rw-r--r--  2.0 unx     4410 b- defN 80-Jan-01 00:00 algokit_utils/_ensure_funded.py
 -rw-r--r--  2.0 unx     2841 b- defN 80-Jan-01 00:00 algokit_utils/_simulate_315_compat.py
 -rw-r--r--  2.0 unx     3569 b- defN 80-Jan-01 00:00 algokit_utils/_transfer.py
 -rw-r--r--  2.0 unx     7364 b- defN 80-Jan-01 00:00 algokit_utils/account.py
 -rw-r--r--  2.0 unx    56488 b- defN 80-Jan-01 00:00 algokit_utils/application_client.py
 -rw-r--r--  2.0 unx     7466 b- defN 80-Jan-01 00:00 algokit_utils/application_specification.py
 -rw-r--r--  2.0 unx    34650 b- defN 80-Jan-01 00:00 algokit_utils/deploy.py
 -rw-r--r--  2.0 unx     2550 b- defN 80-Jan-01 00:00 algokit_utils/logic_error.py
 -rw-r--r--  2.0 unx     6319 b- defN 80-Jan-01 00:00 algokit_utils/models.py
 -rw-r--r--  2.0 unx     5267 b- defN 80-Jan-01 00:00 algokit_utils/network_clients.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 algokit_utils/py.typed
--rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-1.3.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     2070 b- defN 80-Jan-01 00:00 algokit_utils-1.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-1.3.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1349 b- defN 16-Jan-01 00:00 algokit_utils-1.3.0.dist-info/RECORD
-16 files, 139666 bytes uncompressed, 34451 bytes compressed:  75.3%
+-rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-1.3.0b1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2072 b- defN 80-Jan-01 00:00 algokit_utils-1.3.0b1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-1.3.0b1.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1357 b- defN 16-Jan-01 00:00 algokit_utils-1.3.0b1.dist-info/RECORD
+16 files, 139676 bytes uncompressed, 34461 bytes compressed:  75.3%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: algokit_utils/network_clients.py
 Comment: 
 
 Filename: algokit_utils/py.typed
 Comment: 
 
-Filename: algokit_utils-1.3.0.dist-info/LICENSE
+Filename: algokit_utils-1.3.0b1.dist-info/LICENSE
 Comment: 
 
-Filename: algokit_utils-1.3.0.dist-info/METADATA
+Filename: algokit_utils-1.3.0b1.dist-info/METADATA
 Comment: 
 
-Filename: algokit_utils-1.3.0.dist-info/WHEEL
+Filename: algokit_utils-1.3.0b1.dist-info/WHEEL
 Comment: 
 
-Filename: algokit_utils-1.3.0.dist-info/RECORD
+Filename: algokit_utils-1.3.0b1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `algokit_utils-1.3.0.dist-info/LICENSE` & `algokit_utils-1.3.0b1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `algokit_utils-1.3.0.dist-info/METADATA` & `algokit_utils-1.3.0b1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algokit-utils
-Version: 1.3.0
+Version: 1.3.0b1
 Summary: Utilities for Algorand development for use by AlgoKit
 License: MIT
 Author: Algorand Foundation
 Author-email: contact@algorand.foundation
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `algokit_utils-1.3.0.dist-info/RECORD` & `algokit_utils-1.3.0b1.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -6,11 +6,11 @@
 algokit_utils/application_client.py,sha256=k3eTyhY3zyfpajHffo1uJ2u1C0vlYPmdALl5jmgH1WM,56488
 algokit_utils/application_specification.py,sha256=XusOe7VrGPun2UoNspC9Ei202NzPkxRNx5USXiABuXc,7466
 algokit_utils/deploy.py,sha256=sY6u0T39DuF6oLpal0eJAc76EmjPWdoCPk2OSKGccnM,34650
 algokit_utils/logic_error.py,sha256=8O_4rJ1t57JEG81ucRNih2ojc1-EOm2fVxW6m-1ZXI8,2550
 algokit_utils/models.py,sha256=75tWWa3W-37Om3YgkcuKiuHAGzMkFIJ9U-eHO29RPi4,6319
 algokit_utils/network_clients.py,sha256=KmuSHG2kSdJfo9W4pIB_4RjnBL2yMQNGlF54lxXTnsQ,5267
 algokit_utils/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-algokit_utils-1.3.0.dist-info/LICENSE,sha256=J5i7U1Q9Q2c7saUzlvFRmrCCFhQyXb5Juz_LO5omNUw,1076
-algokit_utils-1.3.0.dist-info/METADATA,sha256=feNB3EiPbsbPivhIsVnKw1ewuwe_CmxLYtQJYwPIc6g,2070
-algokit_utils-1.3.0.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-algokit_utils-1.3.0.dist-info/RECORD,,
+algokit_utils-1.3.0b1.dist-info/LICENSE,sha256=J5i7U1Q9Q2c7saUzlvFRmrCCFhQyXb5Juz_LO5omNUw,1076
+algokit_utils-1.3.0b1.dist-info/METADATA,sha256=75vQhThgjoQUr2xDl-t--FnVEl9bHz7kAs7LS4jVwns,2072
+algokit_utils-1.3.0b1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+algokit_utils-1.3.0b1.dist-info/RECORD,,
```

