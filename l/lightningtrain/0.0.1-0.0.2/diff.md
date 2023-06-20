# Comparing `tmp/lightningtrain-0.0.1-py3-none-any.whl.zip` & `tmp/lightningtrain-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,16 @@
-Zip file size: 6720 bytes, number of entries: 15
+Zip file size: 5887 bytes, number of entries: 14
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-20 06:59 configs/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-20 15:22 tests/__init__.py
 -rw-rw-r--  2.0 unx     2219 b- defN 23-Jun-20 15:32 tests/conftest.py
 -rw-rw-r--  2.0 unx      742 b- defN 23-Jun-20 15:22 tests/test_configs.py
 -rw-rw-r--  2.0 unx      959 b- defN 23-Jun-20 15:33 tests/test_datamodules.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-20 15:24 tests/helpers/__init__.py
 -rw-rw-r--  2.0 unx      857 b- defN 23-Jun-20 15:24 tests/helpers/package_available.py
 -rw-rw-r--  2.0 unx     4307 b- defN 23-Jun-20 15:24 tests/helpers/run_if.py
 -rw-rw-r--  2.0 unx      415 b- defN 23-Jun-20 15:24 tests/helpers/run_sh_command.py
--rw-rw-r--  2.0 unx     1068 b- defN 23-Jun-20 17:02 lightningtrain-0.0.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx      266 b- defN 23-Jun-20 17:02 lightningtrain-0.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Jun-20 17:02 lightningtrain-0.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx      114 b- defN 23-Jun-20 17:02 lightningtrain-0.0.1.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       14 b- defN 23-Jun-20 17:02 lightningtrain-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1236 b- defN 23-Jun-20 17:02 lightningtrain-0.0.1.dist-info/RECORD
-15 files, 12307 bytes uncompressed, 4652 bytes compressed:  62.2%
+-rw-rw-r--  2.0 unx      258 b- defN 23-Jun-20 17:08 lightningtrain-0.0.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-Jun-20 17:08 lightningtrain-0.0.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx      114 b- defN 23-Jun-20 17:08 lightningtrain-0.0.2.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       14 b- defN 23-Jun-20 17:08 lightningtrain-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1141 b- defN 23-Jun-20 17:08 lightningtrain-0.0.2.dist-info/RECORD
+14 files, 11136 bytes uncompressed, 3971 bytes compressed:  64.3%
```

## zipnote {}

```diff
@@ -21,26 +21,23 @@
 
 Filename: tests/helpers/run_if.py
 Comment: 
 
 Filename: tests/helpers/run_sh_command.py
 Comment: 
 
-Filename: lightningtrain-0.0.1.dist-info/LICENSE
+Filename: lightningtrain-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: lightningtrain-0.0.1.dist-info/METADATA
+Filename: lightningtrain-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: lightningtrain-0.0.1.dist-info/WHEEL
+Filename: lightningtrain-0.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: lightningtrain-0.0.1.dist-info/entry_points.txt
+Filename: lightningtrain-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: lightningtrain-0.0.1.dist-info/top_level.txt
-Comment: 
-
-Filename: lightningtrain-0.0.1.dist-info/RECORD
+Filename: lightningtrain-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `lightningtrain-0.0.1.dist-info/RECORD` & `lightningtrain-0.0.2.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -3,13 +3,12 @@
 tests/conftest.py,sha256=52RiC4WtQ2B3qSYbyrxMw8ifEBRPuvVhaUF00HSe9k4,2219
 tests/test_configs.py,sha256=ZhUG9bAQ-SIJsyvTzxVF_Yb9Ln_qUoCXMP7VJTbQtjY,742
 tests/test_datamodules.py,sha256=a4RZjBl3xbUeRPbvylNq1gyvEBEddsBnpQM36TGoQXo,959
 tests/helpers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/helpers/package_available.py,sha256=Ug8pwjT8ZYLKoEh4AgLGC_sZEWfDtJ47rkIwKGGUcSU,857
 tests/helpers/run_if.py,sha256=FJSd8vztMDN1t7uIlkOhVkkiJbJvvMtpDMWrTEq_en4,4307
 tests/helpers/run_sh_command.py,sha256=HmXqrKSS5Bs4JHZJwLPw944Df_sFaLlE6744cdoIatQ,415
-lightningtrain-0.0.1.dist-info/LICENSE,sha256=C7NM3M6SzdBfv3vgVDYUiMvlWiG_G_VKF69AtO5_Yy0,1068
-lightningtrain-0.0.1.dist-info/METADATA,sha256=V4sha6oDnJqgJFfEsrcgYQT_tXN1HFzd35UQGKE4lOM,266
-lightningtrain-0.0.1.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-lightningtrain-0.0.1.dist-info/entry_points.txt,sha256=mA5zJFcHornjJ7XKiPtlt9aYPIRkBhoF_MNPpkyilyY,114
-lightningtrain-0.0.1.dist-info/top_level.txt,sha256=tvn_fnTSTV14-1UDVXjA7RBvipZg0zd8b7gruWiEypY,14
-lightningtrain-0.0.1.dist-info/RECORD,,
+lightningtrain-0.0.2.dist-info/METADATA,sha256=MJs8kjMdkZlzmbPoQMSB4JbCjlGTCRvj9rqenNAAqO8,258
+lightningtrain-0.0.2.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+lightningtrain-0.0.2.dist-info/entry_points.txt,sha256=mA5zJFcHornjJ7XKiPtlt9aYPIRkBhoF_MNPpkyilyY,114
+lightningtrain-0.0.2.dist-info/top_level.txt,sha256=tvn_fnTSTV14-1UDVXjA7RBvipZg0zd8b7gruWiEypY,14
+lightningtrain-0.0.2.dist-info/RECORD,,
```

