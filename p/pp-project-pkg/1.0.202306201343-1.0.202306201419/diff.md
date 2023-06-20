# Comparing `tmp/pp_project_pkg-1.0.202306201343-py3-none-any.whl.zip` & `tmp/pp_project_pkg-1.0.202306201419-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 10487 bytes, number of entries: 13
+Zip file size: 10488 bytes, number of entries: 13
 -rw-rw-r--  2.0 unx       71 b- defN 23-Jun-06 14:15 pp_project_pkg/__init__.py
 -rw-rw-r--  2.0 unx     4766 b- defN 23-Jun-20 12:40 pp_project_pkg/linear_train.py
 -rw-rw-r--  2.0 unx      577 b- defN 23-Jun-06 14:14 pp_project_pkg/newsvendor.py
 -rw-rw-r--  2.0 unx     7115 b- defN 23-Jun-06 15:26 pp_project_pkg/pp_tables.py
--rw-rw-r--  2.0 unx     6657 b- defN 23-Jun-20 13:43 pp_project_pkg/utils.py
--rw-rw-r--  2.0 unx      396 b- defN 23-Jun-20 13:43 pp_project_pkg/version.py
+-rw-rw-r--  2.0 unx     6657 b- defN 23-Jun-20 14:19 pp_project_pkg/utils.py
+-rw-rw-r--  2.0 unx      396 b- defN 23-Jun-20 14:19 pp_project_pkg/version.py
 -rw-rw-r--  2.0 unx     4602 b- defN 23-Jun-20 09:33 pp_project_pkg/wrangling.py
--rwxrwxr-x  2.0 unx       65 b- defN 23-Jun-06 09:53 pp_project_pkg-1.0.202306201343.data/scripts/get_tables.py
--rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-06 15:48 pp_project_pkg-1.0.202306201343.data/scripts/pp_project_run.py
--rw-rw-r--  2.0 unx      191 b- defN 23-Jun-20 13:43 pp_project_pkg-1.0.202306201343.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-20 13:43 pp_project_pkg-1.0.202306201343.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-20 13:43 pp_project_pkg-1.0.202306201343.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1182 b- defN 23-Jun-20 13:43 pp_project_pkg-1.0.202306201343.dist-info/RECORD
-13 files, 27045 bytes uncompressed, 8465 bytes compressed:  68.7%
+-rwxrwxr-x  2.0 unx       65 b- defN 23-Jun-06 09:53 pp_project_pkg-1.0.202306201419.data/scripts/get_tables.py
+-rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-06 15:48 pp_project_pkg-1.0.202306201419.data/scripts/pp_project_run.py
+-rw-rw-r--  2.0 unx      191 b- defN 23-Jun-20 14:19 pp_project_pkg-1.0.202306201419.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-20 14:19 pp_project_pkg-1.0.202306201419.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-Jun-20 14:19 pp_project_pkg-1.0.202306201419.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1182 b- defN 23-Jun-20 14:19 pp_project_pkg-1.0.202306201419.dist-info/RECORD
+13 files, 27045 bytes uncompressed, 8466 bytes compressed:  68.7%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: pp_project_pkg/version.py
 Comment: 
 
 Filename: pp_project_pkg/wrangling.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306201343.data/scripts/get_tables.py
+Filename: pp_project_pkg-1.0.202306201419.data/scripts/get_tables.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306201343.data/scripts/pp_project_run.py
+Filename: pp_project_pkg-1.0.202306201419.data/scripts/pp_project_run.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306201343.dist-info/METADATA
+Filename: pp_project_pkg-1.0.202306201419.dist-info/METADATA
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306201343.dist-info/WHEEL
+Filename: pp_project_pkg-1.0.202306201419.dist-info/WHEEL
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306201343.dist-info/top_level.txt
+Filename: pp_project_pkg-1.0.202306201419.dist-info/top_level.txt
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306201343.dist-info/RECORD
+Filename: pp_project_pkg-1.0.202306201419.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pp_project_pkg/utils.py

```diff
@@ -134,15 +134,15 @@
     Returns:
         None
     """
     
     ##fetching the dates which are not there in DB
     dates = list(res_rep['date'])
     for i in range(len(dates)):
-        date_str = dates[0].strftime('%Y-%m-%d')
+        date_str = dates[i].strftime('%Y-%m-%d')
         if logger:
             logger.info("Uploading date : {}".format(date_str))
         a = queries(date=date_str)
         queries_res = a.run_all()
         queries_date = a.date
         res= wrangling_data(queries_res,date=queries_date)
         res.to_sql(name='waldorf_waste_data',con=wv.ml_engine,schema='pp_tables' ,if_exists='append',index=False)
```

## pp_project_pkg/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('06')
 VERSION_DAY = int('20')
-VERSION_HOUR = int('13')
-VERSION_MINUTE = int('43')
+VERSION_HOUR = int('14')
+VERSION_MINUTE = int('19')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202306201343
-version_date = '2023/06/20 13:43'
+PATCH_VERSION = 202306201419
+version_date = '2023/06/20 14:19'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `pp_project_pkg-1.0.202306201343.data/scripts/pp_project_run.py` & `pp_project_pkg-1.0.202306201419.data/scripts/pp_project_run.py`

 * *Files identical despite different names*

## Comparing `pp_project_pkg-1.0.202306201343.dist-info/RECORD` & `pp_project_pkg-1.0.202306201419.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 pp_project_pkg/__init__.py,sha256=9idX2X6SQKZg--ziGy6Ii9OB-kz9hOX1nEG9a0xEW9g,71
 pp_project_pkg/linear_train.py,sha256=wn8wnX6ff7E7AX7eXGcuZtTP_4NKEyvY0LVAzfPcoT4,4766
 pp_project_pkg/newsvendor.py,sha256=E6JHp0Vtmq63toKM6bO3xTAdCgwmAZzRua-w10wrc5Y,577
 pp_project_pkg/pp_tables.py,sha256=8rqVp4P9nF13UbBmN_R7vGK7MeY4BkeG2ibDa7jLRpg,7115
-pp_project_pkg/utils.py,sha256=jXaYLbrUY7nVt_0HC_9xGUuFsag6Sw62uxsoG7dpBk8,6657
-pp_project_pkg/version.py,sha256=5q5R2T18RREZ5fkmFc-RDVZbueXdnwSACvcCAJq44ks,396
+pp_project_pkg/utils.py,sha256=qWUhyGz6Vz_0SOF_SvQbRlr2qxEIl2kqjvE32pZSipw,6657
+pp_project_pkg/version.py,sha256=YVcmbyr7rsGN3O0JQtXmDElncb5bPhwegDO2QKUiOtE,396
 pp_project_pkg/wrangling.py,sha256=5B-LkqLulZm9RGNvN9BsU6T7vqra7pMGRwr0cj9ovdY,4602
-pp_project_pkg-1.0.202306201343.data/scripts/get_tables.py,sha256=E5FmW2bHAU9NPORQMG85RzGtXOGjjzbATEa5lLGjyk4,65
-pp_project_pkg-1.0.202306201343.data/scripts/pp_project_run.py,sha256=hNrYjtDlo7nX9pwMbM7un9R7ToKRdjVosBt3qErKtaA,1316
-pp_project_pkg-1.0.202306201343.dist-info/METADATA,sha256=dy3LcLjSUdSNDT_QcOMGhs0ksBs4px-SkDJRjZ1AQQY,191
-pp_project_pkg-1.0.202306201343.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pp_project_pkg-1.0.202306201343.dist-info/top_level.txt,sha256=2V1bEC5qsYRo1f2gAotX3L3S5xl1nIUxjITUTeRd8yQ,15
-pp_project_pkg-1.0.202306201343.dist-info/RECORD,,
+pp_project_pkg-1.0.202306201419.data/scripts/get_tables.py,sha256=E5FmW2bHAU9NPORQMG85RzGtXOGjjzbATEa5lLGjyk4,65
+pp_project_pkg-1.0.202306201419.data/scripts/pp_project_run.py,sha256=hNrYjtDlo7nX9pwMbM7un9R7ToKRdjVosBt3qErKtaA,1316
+pp_project_pkg-1.0.202306201419.dist-info/METADATA,sha256=DQKBz1gd3ayRZz_D2wMR2Z_F2O-6nukPwdqR_w9gTZ4,191
+pp_project_pkg-1.0.202306201419.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pp_project_pkg-1.0.202306201419.dist-info/top_level.txt,sha256=2V1bEC5qsYRo1f2gAotX3L3S5xl1nIUxjITUTeRd8yQ,15
+pp_project_pkg-1.0.202306201419.dist-info/RECORD,,
```

