# Comparing `tmp/drizzutojr_vader-0.0.4-py3-none-any.whl.zip` & `tmp/drizzutojr_vader-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,17 @@
-Zip file size: 6234 bytes, number of entries: 14
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-19 21:45 vader/__init__.py
--rw-r--r--  2.0 unx     1094 b- defN 23-Jun-19 21:45 vader/core_service.py
--rw-r--r--  2.0 unx     1015 b- defN 23-Jun-19 21:45 vader/exceptions.py
--rw-r--r--  2.0 unx     1425 b- defN 23-Jun-19 21:45 vader/general.py
--rw-r--r--  2.0 unx      665 b- defN 23-Jun-19 21:45 vader/mongo.py
--rw-r--r--  2.0 unx     1730 b- defN 23-Jun-19 21:45 vader/mongo_resource.py
--rw-r--r--  2.0 unx     2496 b- defN 23-Jun-19 21:45 vader/policy_service.py
--rw-r--r--  2.0 unx      524 b- defN 23-Jun-19 21:45 vader/project_resource.py
--rw-r--r--  2.0 unx      929 b- defN 23-Jun-19 21:45 vader/raise_exception.py
--rw-r--r--  2.0 unx      522 b- defN 23-Jun-19 21:45 vader/vault_resource.py
--rw-r--r--  2.0 unx      204 b- defN 23-Jun-19 21:47 drizzutojr_vader-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-19 21:47 drizzutojr_vader-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Jun-19 21:47 drizzutojr_vader-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1100 b- defN 23-Jun-19 21:47 drizzutojr_vader-0.0.4.dist-info/RECORD
-14 files, 11802 bytes uncompressed, 4410 bytes compressed:  62.6%
+Zip file size: 6615 bytes, number of entries: 15
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-20 00:05 vader/__init__.py
+-rw-r--r--  2.0 unx     1094 b- defN 23-Jun-20 00:05 vader/core_service.py
+-rw-r--r--  2.0 unx     1015 b- defN 23-Jun-20 00:05 vader/exceptions.py
+-rw-r--r--  2.0 unx      214 b- defN 23-Jun-20 00:05 vader/external.py
+-rw-r--r--  2.0 unx     1425 b- defN 23-Jun-20 00:05 vader/general.py
+-rw-r--r--  2.0 unx      665 b- defN 23-Jun-20 00:05 vader/mongo.py
+-rw-r--r--  2.0 unx     1730 b- defN 23-Jun-20 00:05 vader/mongo_resource.py
+-rw-r--r--  2.0 unx     2496 b- defN 23-Jun-20 00:05 vader/policy_service.py
+-rw-r--r--  2.0 unx      524 b- defN 23-Jun-20 00:05 vader/project_resource.py
+-rw-r--r--  2.0 unx     1622 b- defN 23-Jun-20 00:05 vader/raise_exception.py
+-rw-r--r--  2.0 unx      522 b- defN 23-Jun-20 00:05 vader/vault_resource.py
+-rw-r--r--  2.0 unx      204 b- defN 23-Jun-20 00:07 drizzutojr_vader-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-20 00:07 drizzutojr_vader-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-20 00:07 drizzutojr_vader-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1174 b- defN 23-Jun-20 00:07 drizzutojr_vader-0.0.5.dist-info/RECORD
+15 files, 12783 bytes uncompressed, 4681 bytes compressed:  63.4%
```

## zipnote {}

```diff
@@ -3,14 +3,17 @@
 
 Filename: vader/core_service.py
 Comment: 
 
 Filename: vader/exceptions.py
 Comment: 
 
+Filename: vader/external.py
+Comment: 
+
 Filename: vader/general.py
 Comment: 
 
 Filename: vader/mongo.py
 Comment: 
 
 Filename: vader/mongo_resource.py
@@ -24,20 +27,20 @@
 
 Filename: vader/raise_exception.py
 Comment: 
 
 Filename: vader/vault_resource.py
 Comment: 
 
-Filename: drizzutojr_vader-0.0.4.dist-info/METADATA
+Filename: drizzutojr_vader-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: drizzutojr_vader-0.0.4.dist-info/WHEEL
+Filename: drizzutojr_vader-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: drizzutojr_vader-0.0.4.dist-info/top_level.txt
+Filename: drizzutojr_vader-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: drizzutojr_vader-0.0.4.dist-info/RECORD
+Filename: drizzutojr_vader-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vader/raise_exception.py

```diff
@@ -1,10 +1,12 @@
 import re
 import semver
 
+from .external import *
+from .general import *
 from .exceptions import *
 
 MIN_DESCRIPTION_LENGTH = 20
 MAX_DESCRIPTION_LENGTH = 100
 
 
 def raise_exception_invalid_email(email: str):
@@ -24,7 +26,27 @@
     if len(description) > max_length:
         raise VaderConfigError(f"Description may not be over {max_length} characters")
 
 
 def raise_exception_invalid_version(version):
     if not semver.VersionInfo.is_valid(version):
         raise VaderConfigError(f"Version number is not a valid version: {version}")
+
+
+def raise_exception_username_does_not_exist(username):
+    if not validate_username_exists(username):
+        raise VaderConfigError(f"Username {username} not found")
+
+
+def raise_exception_email_does_not_exist(email):
+    if not validate_email_exists(username):
+        raise VaderConfigError(f"Email {email} not found")
+
+
+def raise_exception_app_id_does_not_exist(app_id):
+    if not validate_app_id_exists(app_id):
+        raise VaderConfigError(f"App ID {app_id} not found")
+
+
+def raise_exception_group_does_not_exist(group_name):
+    if not validate_group_exists(group_name):
+        raise VaderConfigError(f"Group {group_name} not found")
```

## Comparing `drizzutojr_vader-0.0.4.dist-info/RECORD` & `drizzutojr_vader-0.0.5.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 vader/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 vader/core_service.py,sha256=VzIyTc6GAxJUk7B6bO-nP6dHNTJkIpETdznHV1HTl0I,1094
 vader/exceptions.py,sha256=qMmVOiEvdBxZ_3c-EX2kI1QIRjm2QaN7zPD1_fcle_E,1015
+vader/external.py,sha256=W2lB4pKB2q4BFvBPyhbZd2liBTyy8W30LEXMthbGdJI,214
 vader/general.py,sha256=qrb_VaFYcL9vJ_ne2skLMDKeoPf5uQXvwx4O8VdqdXs,1425
 vader/mongo.py,sha256=cqaO7YzxuDa8SKi2wiN0yeLY4sDr53SKg5r1cqaT5so,665
 vader/mongo_resource.py,sha256=HCCjE3OqPHwaAJ1afcTgP4Tx8vTMXfIfboIXf1S8bOI,1730
 vader/policy_service.py,sha256=YOZCDml0ja4l3n6I42mqH_CS4q8TJQstKNx5HrxHa-o,2496
 vader/project_resource.py,sha256=OowzfDSKV5DcRPIvBORaFcH7NkboL3eJ_E5T0VFq2lI,524
-vader/raise_exception.py,sha256=7gT1f-F8HUTZbYZ10jJtq0XGh2mkIC-SFoHdAgWxP2k,929
+vader/raise_exception.py,sha256=fUSe6NprEZw1DsR4VURWBMiHLJVC-d_2qoGnmkRosFA,1622
 vader/vault_resource.py,sha256=ycKBx2NXoFpg5m1FxYWgD5NEz6vSDDF7YGBQVJbBC8c,522
-drizzutojr_vader-0.0.4.dist-info/METADATA,sha256=eW_rsZwJCtuOeMZLvOGa_ui4UYvvdMAQTPntUJj83D8,204
-drizzutojr_vader-0.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-drizzutojr_vader-0.0.4.dist-info/top_level.txt,sha256=wEY-qHmChGsqPB_SEURS5ewt6uoSGcuQuRwmGxr1Sqw,6
-drizzutojr_vader-0.0.4.dist-info/RECORD,,
+drizzutojr_vader-0.0.5.dist-info/METADATA,sha256=uFn-zxgzt-7njNCwdcwzIGeHwxLELKKumuUwKei2j4o,204
+drizzutojr_vader-0.0.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+drizzutojr_vader-0.0.5.dist-info/top_level.txt,sha256=wEY-qHmChGsqPB_SEURS5ewt6uoSGcuQuRwmGxr1Sqw,6
+drizzutojr_vader-0.0.5.dist-info/RECORD,,
```

