# Comparing `tmp/deepsearcheath-0.9.4-py3-none-any.whl.zip` & `tmp/deepsearcheath-0.9.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 13778 bytes, number of entries: 7
+Zip file size: 13878 bytes, number of entries: 7
 -rw-r--r--  2.0 unx       18 b- defN 22-Jan-23 07:47 deepsearcheath/__init__.py
--rw-r--r--  2.0 unx    49507 b- defN 23-Jun-16 09:49 deepsearcheath/deepsearch.py
--rw-rw-r--  2.0 unx    11357 b- defN 23-Jun-16 09:50 deepsearcheath-0.9.4.dist-info/LICENSE
--rw-r--r--  2.0 unx      742 b- defN 23-Jun-16 09:50 deepsearcheath-0.9.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-16 09:50 deepsearcheath-0.9.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Jun-16 09:50 deepsearcheath-0.9.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      588 b- defN 23-Jun-16 09:50 deepsearcheath-0.9.4.dist-info/RECORD
-7 files, 62319 bytes uncompressed, 12728 bytes compressed:  79.6%
+-rw-r--r--  2.0 unx    49843 b- defN 23-Jun-20 09:25 deepsearcheath/deepsearch.py
+-rw-rw-r--  2.0 unx    11357 b- defN 23-Jun-20 09:27 deepsearcheath-0.9.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx      742 b- defN 23-Jun-20 09:27 deepsearcheath-0.9.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-20 09:27 deepsearcheath-0.9.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Jun-20 09:27 deepsearcheath-0.9.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      588 b- defN 23-Jun-20 09:27 deepsearcheath-0.9.6.dist-info/RECORD
+7 files, 62655 bytes uncompressed, 12828 bytes compressed:  79.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: deepsearcheath/__init__.py
 Comment: 
 
 Filename: deepsearcheath/deepsearch.py
 Comment: 
 
-Filename: deepsearcheath-0.9.4.dist-info/LICENSE
+Filename: deepsearcheath-0.9.6.dist-info/LICENSE
 Comment: 
 
-Filename: deepsearcheath-0.9.4.dist-info/METADATA
+Filename: deepsearcheath-0.9.6.dist-info/METADATA
 Comment: 
 
-Filename: deepsearcheath-0.9.4.dist-info/WHEEL
+Filename: deepsearcheath-0.9.6.dist-info/WHEEL
 Comment: 
 
-Filename: deepsearcheath-0.9.4.dist-info/top_level.txt
+Filename: deepsearcheath-0.9.6.dist-info/top_level.txt
 Comment: 
 
-Filename: deepsearcheath-0.9.4.dist-info/RECORD
+Filename: deepsearcheath-0.9.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## deepsearcheath/deepsearch.py

```diff
@@ -428,18 +428,26 @@
         return bool(len(pd.bdate_range(date, date)))
 
     def _datetime_reformer(date:str) -> datetime:
         formats = [
             "%Y-%m-%d", 
             "%m/%d/%Y",
         ]
+        checked = False
         for i in formats:
             try: _datetime = datetime.strptime(date, i)
-            except: continue
-        return _datetime  #! formats 에 없는 형식일 경우 에러
+            except: _datetime = date
+            checked = True
+        if not checked:
+            print("Date format is not valid. Check the date format.")
+            print("Date format should be one of the following:")
+            print(formats)
+            print("Your date format is:")
+            print(date)
+        return _datetime  #! formats 에 없는 형식일 경우 에러 : "%Y-%m-%d", "%m/%d/%Y"
 
     @classmethod
     async def _async_main(cls, symbol_list, date_from, date_to, krx=True) -> list or None:
         start = "'"
         separator = "', '"
         query = f"GetStockPrices(([{start + separator.join(symbol_list) + start}]), columns=['change_rate'], date_from={date_from}, date_to={date_to})"
         task = [cls.async_deepsearch.compute(query)]
```

## Comparing `deepsearcheath-0.9.4.dist-info/LICENSE` & `deepsearcheath-0.9.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `deepsearcheath-0.9.4.dist-info/METADATA` & `deepsearcheath-0.9.6.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepsearcheath
-Version: 0.9.4
+Version: 0.9.6
 Summary: Heath taylored DeepSearch api.
 Home-page: https://github.com/htaehpeed/deepsearcheath
 Author: Heath
 Author-email: heath@deepsearch.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

