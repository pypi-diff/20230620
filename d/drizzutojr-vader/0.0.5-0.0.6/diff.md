# Comparing `tmp/drizzutojr_vader-0.0.5-py3-none-any.whl.zip` & `tmp/drizzutojr_vader-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 6615 bytes, number of entries: 15
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-20 00:05 vader/__init__.py
--rw-r--r--  2.0 unx     1094 b- defN 23-Jun-20 00:05 vader/core_service.py
--rw-r--r--  2.0 unx     1015 b- defN 23-Jun-20 00:05 vader/exceptions.py
--rw-r--r--  2.0 unx      214 b- defN 23-Jun-20 00:05 vader/external.py
--rw-r--r--  2.0 unx     1425 b- defN 23-Jun-20 00:05 vader/general.py
--rw-r--r--  2.0 unx      665 b- defN 23-Jun-20 00:05 vader/mongo.py
--rw-r--r--  2.0 unx     1730 b- defN 23-Jun-20 00:05 vader/mongo_resource.py
--rw-r--r--  2.0 unx     2496 b- defN 23-Jun-20 00:05 vader/policy_service.py
--rw-r--r--  2.0 unx      524 b- defN 23-Jun-20 00:05 vader/project_resource.py
--rw-r--r--  2.0 unx     1622 b- defN 23-Jun-20 00:05 vader/raise_exception.py
--rw-r--r--  2.0 unx      522 b- defN 23-Jun-20 00:05 vader/vault_resource.py
--rw-r--r--  2.0 unx      204 b- defN 23-Jun-20 00:07 drizzutojr_vader-0.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-20 00:07 drizzutojr_vader-0.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Jun-20 00:07 drizzutojr_vader-0.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1174 b- defN 23-Jun-20 00:07 drizzutojr_vader-0.0.5.dist-info/RECORD
-15 files, 12783 bytes uncompressed, 4681 bytes compressed:  63.4%
+Zip file size: 6611 bytes, number of entries: 15
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-20 02:06 vader/__init__.py
+-rw-r--r--  2.0 unx     1094 b- defN 23-Jun-20 02:06 vader/core_service.py
+-rw-r--r--  2.0 unx     1015 b- defN 23-Jun-20 02:06 vader/exceptions.py
+-rw-r--r--  2.0 unx      214 b- defN 23-Jun-20 02:06 vader/external.py
+-rw-r--r--  2.0 unx     1425 b- defN 23-Jun-20 02:06 vader/general.py
+-rw-r--r--  2.0 unx      665 b- defN 23-Jun-20 02:06 vader/mongo.py
+-rw-r--r--  2.0 unx     1730 b- defN 23-Jun-20 02:06 vader/mongo_resource.py
+-rw-r--r--  2.0 unx     2496 b- defN 23-Jun-20 02:06 vader/policy_service.py
+-rw-r--r--  2.0 unx      518 b- defN 23-Jun-20 02:06 vader/project_resource.py
+-rw-r--r--  2.0 unx     1622 b- defN 23-Jun-20 02:06 vader/raise_exception.py
+-rw-r--r--  2.0 unx      522 b- defN 23-Jun-20 02:06 vader/vault_resource.py
+-rw-r--r--  2.0 unx      204 b- defN 23-Jun-20 02:07 drizzutojr_vader-0.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-20 02:07 drizzutojr_vader-0.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-20 02:07 drizzutojr_vader-0.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1174 b- defN 23-Jun-20 02:07 drizzutojr_vader-0.0.6.dist-info/RECORD
+15 files, 12777 bytes uncompressed, 4677 bytes compressed:  63.4%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: vader/raise_exception.py
 Comment: 
 
 Filename: vader/vault_resource.py
 Comment: 
 
-Filename: drizzutojr_vader-0.0.5.dist-info/METADATA
+Filename: drizzutojr_vader-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: drizzutojr_vader-0.0.5.dist-info/WHEEL
+Filename: drizzutojr_vader-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: drizzutojr_vader-0.0.5.dist-info/top_level.txt
+Filename: drizzutojr_vader-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: drizzutojr_vader-0.0.5.dist-info/RECORD
+Filename: drizzutojr_vader-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vader/project_resource.py

```diff
@@ -5,10 +5,10 @@
 class ProjectResource(MongoResource):
     def __init__(
         self, namespace, app_id, boundary_id, requestor, collection_name, request_data
     ):
         super().__init__(app_id, collection_name)
         self.namespace = namespace
         self.boundary_id = boundary_id
-        self.project_name = utils.generate_project_name(self.app_id, self.boundary_id)
+        self.project_name = generate_project_name(self.app_id, self.boundary_id)
         self.requestor = requestor
         self.request_data = request_data
```

## Comparing `drizzutojr_vader-0.0.5.dist-info/RECORD` & `drizzutojr_vader-0.0.6.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,14 @@
 vader/core_service.py,sha256=VzIyTc6GAxJUk7B6bO-nP6dHNTJkIpETdznHV1HTl0I,1094
 vader/exceptions.py,sha256=qMmVOiEvdBxZ_3c-EX2kI1QIRjm2QaN7zPD1_fcle_E,1015
 vader/external.py,sha256=W2lB4pKB2q4BFvBPyhbZd2liBTyy8W30LEXMthbGdJI,214
 vader/general.py,sha256=qrb_VaFYcL9vJ_ne2skLMDKeoPf5uQXvwx4O8VdqdXs,1425
 vader/mongo.py,sha256=cqaO7YzxuDa8SKi2wiN0yeLY4sDr53SKg5r1cqaT5so,665
 vader/mongo_resource.py,sha256=HCCjE3OqPHwaAJ1afcTgP4Tx8vTMXfIfboIXf1S8bOI,1730
 vader/policy_service.py,sha256=YOZCDml0ja4l3n6I42mqH_CS4q8TJQstKNx5HrxHa-o,2496
-vader/project_resource.py,sha256=OowzfDSKV5DcRPIvBORaFcH7NkboL3eJ_E5T0VFq2lI,524
+vader/project_resource.py,sha256=HIPDD9wxee3OaSZ0t3ij11oim9FzqpehuJcTGF3rgSY,518
 vader/raise_exception.py,sha256=fUSe6NprEZw1DsR4VURWBMiHLJVC-d_2qoGnmkRosFA,1622
 vader/vault_resource.py,sha256=ycKBx2NXoFpg5m1FxYWgD5NEz6vSDDF7YGBQVJbBC8c,522
-drizzutojr_vader-0.0.5.dist-info/METADATA,sha256=uFn-zxgzt-7njNCwdcwzIGeHwxLELKKumuUwKei2j4o,204
-drizzutojr_vader-0.0.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-drizzutojr_vader-0.0.5.dist-info/top_level.txt,sha256=wEY-qHmChGsqPB_SEURS5ewt6uoSGcuQuRwmGxr1Sqw,6
-drizzutojr_vader-0.0.5.dist-info/RECORD,,
+drizzutojr_vader-0.0.6.dist-info/METADATA,sha256=s670AZuwtmmtUMzfQQgczPscj2an4ATYVs8rwfToz1Q,204
+drizzutojr_vader-0.0.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+drizzutojr_vader-0.0.6.dist-info/top_level.txt,sha256=wEY-qHmChGsqPB_SEURS5ewt6uoSGcuQuRwmGxr1Sqw,6
+drizzutojr_vader-0.0.6.dist-info/RECORD,,
```

