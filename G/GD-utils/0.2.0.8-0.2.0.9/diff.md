# Comparing `tmp/GD_utils-0.2.0.8-py3-none-any.whl.zip` & `tmp/GD_utils-0.2.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,18 @@
-Zip file size: 23797 bytes, number of entries: 15
--rw-rw-rw-  2.0 fat       49 b- defN 22-Feb-16 07:40 GDUs/__init__.py
--rw-rw-rw-  2.0 fat      149 b- defN 22-Feb-16 07:40 GDUs/calc_return.py
--rw-rw-rw-  2.0 fat     3284 b- defN 22-Feb-16 06:37 GDUs/get_data.py
--rw-rw-rw-  2.0 fat     2870 b- defN 22-Feb-16 07:40 GDUs/return_calculator.py
--rw-rw-rw-  2.0 fat     1850 b- defN 22-Mar-08 01:30 GD_utils/Report.py
--rw-rw-rw-  2.0 fat      129 b- defN 22-Apr-08 06:41 GD_utils/__init__.py
--rw-rw-rw-  2.0 fat      163 b- defN 22-Feb-17 00:37 GD_utils/calc_return.py
--rw-rw-rw-  2.0 fat    17226 b- defN 22-Apr-11 01:50 GD_utils/factor_calculator.py
--rw-rw-rw-  2.0 fat    25137 b- defN 22-Feb-17 00:22 GD_utils/get_data.py
--rw-rw-rw-  2.0 fat    54129 b- defN 22-Apr-10 23:38 GD_utils/portfolio_calculator.py
--rw-rw-rw-  2.0 fat     4691 b- defN 22-Apr-11 01:05 GD_utils/return_calculator.py
--rw-rw-rw-  2.0 fat      371 b- defN 22-Apr-11 01:52 GD_utils-0.2.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-Apr-11 01:52 GD_utils-0.2.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 22-Apr-11 01:52 GD_utils-0.2.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1180 b- defN 22-Apr-11 01:52 GD_utils-0.2.0.8.dist-info/RECORD
-15 files, 111329 bytes uncompressed, 21861 bytes compressed:  80.4%
+Zip file size: 24867 bytes, number of entries: 16
+-rw-rw-rw-  2.0 fat       49 b- defN 22-May-06 04:17 GDUs/__init__.py
+-rw-rw-rw-  2.0 fat      149 b- defN 22-May-06 04:17 GDUs/calc_return.py
+-rw-rw-rw-  2.0 fat     3284 b- defN 22-May-06 04:17 GDUs/get_data.py
+-rw-rw-rw-  2.0 fat     2870 b- defN 22-May-06 04:17 GDUs/return_calculator.py
+-rw-rw-rw-  2.0 fat     1850 b- defN 22-May-06 04:17 GD_utils/Report.py
+-rw-rw-rw-  2.0 fat      129 b- defN 22-May-06 04:17 GD_utils/__init__.py
+-rw-rw-rw-  2.0 fat      163 b- defN 22-May-06 04:17 GD_utils/calc_return.py
+-rw-rw-rw-  2.0 fat    17226 b- defN 22-May-06 04:17 GD_utils/factor_calculator.py
+-rw-rw-rw-  2.0 fat    25137 b- defN 22-May-06 04:17 GD_utils/get_data.py
+-rw-rw-rw-  2.0 fat    54129 b- defN 22-May-06 04:17 GD_utils/portfolio_calculator.py
+-rw-rw-rw-  2.0 fat     4691 b- defN 22-May-06 04:17 GD_utils/return_calculator.py
+-rw-rw-rw-  2.0 fat     2889 b- defN 22-May-06 04:17 GD_utils/return_calculator_old.py
+-rw-rw-rw-  2.0 fat      371 b- defN 22-May-06 04:17 GD_utils-0.2.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 22-May-06 04:17 GD_utils-0.2.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 22-May-06 04:17 GD_utils-0.2.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1270 b- defN 22-May-06 04:17 GD_utils-0.2.0.9.dist-info/RECORD
+16 files, 114308 bytes uncompressed, 22789 bytes compressed:  80.1%
```

## zipnote {}

```diff
@@ -27,20 +27,23 @@
 
 Filename: GD_utils/portfolio_calculator.py
 Comment: 
 
 Filename: GD_utils/return_calculator.py
 Comment: 
 
-Filename: GD_utils-0.2.0.8.dist-info/METADATA
+Filename: GD_utils/return_calculator_old.py
 Comment: 
 
-Filename: GD_utils-0.2.0.8.dist-info/WHEEL
+Filename: GD_utils-0.2.0.9.dist-info/METADATA
 Comment: 
 
-Filename: GD_utils-0.2.0.8.dist-info/top_level.txt
+Filename: GD_utils-0.2.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: GD_utils-0.2.0.8.dist-info/RECORD
+Filename: GD_utils-0.2.0.9.dist-info/top_level.txt
+Comment: 
+
+Filename: GD_utils-0.2.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `GD_utils-0.2.0.8.dist-info/RECORD` & `GD_utils-0.2.0.9.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -5,11 +5,12 @@
 GD_utils/Report.py,sha256=yZ2TD3cnPSckah-AIjFiJw_n6b0A-z8dIYEMIozwLJg,1850
 GD_utils/__init__.py,sha256=8LYgSindeJrjDX1BIEnXgVRXm9yE_xKyDnQ7O82ZFdg,129
 GD_utils/calc_return.py,sha256=UQ2_jWae_y4OAt1s2IepxXKTXbOMmT79HHp7PwOCLWM,163
 GD_utils/factor_calculator.py,sha256=zIuqp2xPnk7Ezy0-Bz1YOAAKPVDkw9lwly65e8noQMk,17226
 GD_utils/get_data.py,sha256=aV2DmV_Yrpe6IcnasrUdltPhW0LNYNngWHgOjlLKjBk,25137
 GD_utils/portfolio_calculator.py,sha256=grK6zF69dBX5YRPycDrO2Inh_C-PnpWjAjEGi1zGGKs,54129
 GD_utils/return_calculator.py,sha256=IYeFkiANiGozBkRuWfZULdgcnIQ5ZMBWF59RkiifkQE,4691
-GD_utils-0.2.0.8.dist-info/METADATA,sha256=4zJ2L7ivQC2eeghSaS84xDze_3pJ31UBuO5mVJrT7oI,371
-GD_utils-0.2.0.8.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-GD_utils-0.2.0.8.dist-info/top_level.txt,sha256=E4T7a5REIitVLK3qkxmo4PRdrEkasUmb6AMNNUMiclQ,9
-GD_utils-0.2.0.8.dist-info/RECORD,,
+GD_utils/return_calculator_old.py,sha256=3c9PurFg0twYFVm2nwqptuqTOppSaS7ydc7lD0_XYdw,2889
+GD_utils-0.2.0.9.dist-info/METADATA,sha256=fPLUltfmMMCmzSEo3ffcxMbEp2hsZqnzDZ6BgKO7EXc,371
+GD_utils-0.2.0.9.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+GD_utils-0.2.0.9.dist-info/top_level.txt,sha256=E4T7a5REIitVLK3qkxmo4PRdrEkasUmb6AMNNUMiclQ,9
+GD_utils-0.2.0.9.dist-info/RECORD,,
```

