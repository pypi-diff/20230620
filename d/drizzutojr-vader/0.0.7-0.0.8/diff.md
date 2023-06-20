# Comparing `tmp/drizzutojr_vader-0.0.7-py3-none-any.whl.zip` & `tmp/drizzutojr_vader-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 6623 bytes, number of entries: 15
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-20 03:19 vader/__init__.py
--rw-r--r--  2.0 unx     1094 b- defN 23-Jun-20 03:19 vader/core_service.py
--rw-r--r--  2.0 unx     1015 b- defN 23-Jun-20 03:19 vader/exceptions.py
--rw-r--r--  2.0 unx      214 b- defN 23-Jun-20 03:19 vader/external.py
--rw-r--r--  2.0 unx     1425 b- defN 23-Jun-20 03:19 vader/general.py
--rw-r--r--  2.0 unx      665 b- defN 23-Jun-20 03:19 vader/mongo.py
--rw-r--r--  2.0 unx     1730 b- defN 23-Jun-20 03:19 vader/mongo_resource.py
--rw-r--r--  2.0 unx     2496 b- defN 23-Jun-20 03:19 vader/policy_service.py
--rw-r--r--  2.0 unx      518 b- defN 23-Jun-20 03:19 vader/project_resource.py
--rw-r--r--  2.0 unx     1622 b- defN 23-Jun-20 03:19 vader/raise_exception.py
--rw-r--r--  2.0 unx      522 b- defN 23-Jun-20 03:19 vader/vault_resource.py
--rw-r--r--  2.0 unx      236 b- defN 23-Jun-20 03:20 drizzutojr_vader-0.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-20 03:20 drizzutojr_vader-0.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Jun-20 03:20 drizzutojr_vader-0.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1174 b- defN 23-Jun-20 03:20 drizzutojr_vader-0.0.7.dist-info/RECORD
-15 files, 12809 bytes uncompressed, 4689 bytes compressed:  63.4%
+Zip file size: 6587 bytes, number of entries: 15
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-20 04:34 vader/__init__.py
+-rw-r--r--  2.0 unx     1094 b- defN 23-Jun-20 04:34 vader/core_service.py
+-rw-r--r--  2.0 unx     1015 b- defN 23-Jun-20 04:34 vader/exceptions.py
+-rw-r--r--  2.0 unx      214 b- defN 23-Jun-20 04:34 vader/external.py
+-rw-r--r--  2.0 unx     1425 b- defN 23-Jun-20 04:34 vader/general.py
+-rw-r--r--  2.0 unx      665 b- defN 23-Jun-20 04:34 vader/mongo.py
+-rw-r--r--  2.0 unx     1730 b- defN 23-Jun-20 04:34 vader/mongo_resource.py
+-rw-r--r--  2.0 unx     2496 b- defN 23-Jun-20 04:34 vader/policy_service.py
+-rw-r--r--  2.0 unx      518 b- defN 23-Jun-20 04:34 vader/project_resource.py
+-rw-r--r--  2.0 unx     1622 b- defN 23-Jun-20 04:34 vader/raise_exception.py
+-rw-r--r--  2.0 unx      422 b- defN 23-Jun-20 04:34 vader/vault_resource.py
+-rw-r--r--  2.0 unx      236 b- defN 23-Jun-20 04:35 drizzutojr_vader-0.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-20 04:35 drizzutojr_vader-0.0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-20 04:35 drizzutojr_vader-0.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1174 b- defN 23-Jun-20 04:35 drizzutojr_vader-0.0.8.dist-info/RECORD
+15 files, 12709 bytes uncompressed, 4653 bytes compressed:  63.4%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: vader/raise_exception.py
 Comment: 
 
 Filename: vader/vault_resource.py
 Comment: 
 
-Filename: drizzutojr_vader-0.0.7.dist-info/METADATA
+Filename: drizzutojr_vader-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: drizzutojr_vader-0.0.7.dist-info/WHEEL
+Filename: drizzutojr_vader-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: drizzutojr_vader-0.0.7.dist-info/top_level.txt
+Filename: drizzutojr_vader-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: drizzutojr_vader-0.0.7.dist-info/RECORD
+Filename: drizzutojr_vader-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vader/vault_resource.py

```diff
@@ -3,17 +3,17 @@
 from vapi import VAPI
 
 from abc import ABC, abstractmethod
 
 
 class VaultResource(ABC):
     def _get_vault_resource(self, path):
-        return json.loads(VAPI().get(path))
+        return VAPI().get(path)
 
-    def _post_vault_resource(self, path, config, expected_status_code=200):
-        return json.loads(VAPI().post(path, config))
+    def _post_vault_resource(self, path, config):
+        return VAPI().post(path, config)
 
-    def _delete_vault_resource(self, path, expected_status_code=204):
-        return json.loads(VAPI().delete(path))
+    def _delete_vault_resource(self, path):
+        return VAPI().delete(path)
 
     def _list_vault_resources(self, path):
-        return json.loads(VAPI().list(path))
+        return VAPI().list(path)
```

## Comparing `drizzutojr_vader-0.0.7.dist-info/RECORD` & `drizzutojr_vader-0.0.8.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -4,12 +4,12 @@
 vader/external.py,sha256=W2lB4pKB2q4BFvBPyhbZd2liBTyy8W30LEXMthbGdJI,214
 vader/general.py,sha256=qrb_VaFYcL9vJ_ne2skLMDKeoPf5uQXvwx4O8VdqdXs,1425
 vader/mongo.py,sha256=cqaO7YzxuDa8SKi2wiN0yeLY4sDr53SKg5r1cqaT5so,665
 vader/mongo_resource.py,sha256=HCCjE3OqPHwaAJ1afcTgP4Tx8vTMXfIfboIXf1S8bOI,1730
 vader/policy_service.py,sha256=YOZCDml0ja4l3n6I42mqH_CS4q8TJQstKNx5HrxHa-o,2496
 vader/project_resource.py,sha256=HIPDD9wxee3OaSZ0t3ij11oim9FzqpehuJcTGF3rgSY,518
 vader/raise_exception.py,sha256=fUSe6NprEZw1DsR4VURWBMiHLJVC-d_2qoGnmkRosFA,1622
-vader/vault_resource.py,sha256=ycKBx2NXoFpg5m1FxYWgD5NEz6vSDDF7YGBQVJbBC8c,522
-drizzutojr_vader-0.0.7.dist-info/METADATA,sha256=p-yUD20ph8wR2Lww8iUKeH_KZA2yDTkvtRmlGlIFrXY,236
-drizzutojr_vader-0.0.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-drizzutojr_vader-0.0.7.dist-info/top_level.txt,sha256=wEY-qHmChGsqPB_SEURS5ewt6uoSGcuQuRwmGxr1Sqw,6
-drizzutojr_vader-0.0.7.dist-info/RECORD,,
+vader/vault_resource.py,sha256=xArBVKJXRuEh_M5HJss5cxycAoH8Uh36Jg4Z_13ga7I,422
+drizzutojr_vader-0.0.8.dist-info/METADATA,sha256=Xzb7ftZBXrdv3OUtuwr_TRZH_Gz1_bgWXUtrOx3HLHI,236
+drizzutojr_vader-0.0.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+drizzutojr_vader-0.0.8.dist-info/top_level.txt,sha256=wEY-qHmChGsqPB_SEURS5ewt6uoSGcuQuRwmGxr1Sqw,6
+drizzutojr_vader-0.0.8.dist-info/RECORD,,
```

