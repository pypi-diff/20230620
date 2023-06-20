# Comparing `tmp/wangticketyes24-0.95-py3-none-any.whl.zip` & `tmp/wangticketyes24-1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 28285 bytes, number of entries: 12
--rw-r--r--  2.0 unx      115 b- defN 23-Jun-11 00:46 wangticketyes24/__init__.py
+Zip file size: 28275 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      114 b- defN 23-Jun-20 11:16 wangticketyes24/__init__.py
 -rw-r--r--  2.0 unx    28280 b- defN 23-Jun-11 00:43 wangticketyes24/selenium_yes24.py
--rw-r--r--  2.0 unx    43062 b- defN 23-Jun-11 00:43 wangticketyes24/yes24.py
+-rw-r--r--  2.0 unx    43080 b- defN 23-Jun-20 11:13 wangticketyes24/yes24.py
 -rw-r--r--  2.0 unx       94 b- defN 18-Dec-12 13:54 yes24ticket/__init__.py
 -rw-r--r--  2.0 unx     7490 b- defN 18-Dec-12 14:11 yes24ticket/selenium_yes24.py
 -rw-r--r--  2.0 unx    15460 b- defN 18-Dec-12 14:12 yes24ticket/yes24test.py
--rw-r--r--  2.0 unx       61 b- defN 23-Jun-11 00:47 wangticketyes24-0.95.dist-info/DESCRIPTION.rst
--rw-r--r--  2.0 unx      691 b- defN 23-Jun-11 00:47 wangticketyes24-0.95.dist-info/metadata.json
--rw-r--r--  2.0 unx       16 b- defN 23-Jun-11 00:47 wangticketyes24-0.95.dist-info/top_level.txt
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-11 00:47 wangticketyes24-0.95.dist-info/WHEEL
--rw-r--r--  2.0 unx      576 b- defN 23-Jun-11 00:47 wangticketyes24-0.95.dist-info/METADATA
--rw-r--r--  2.0 unx     1040 b- defN 23-Jun-11 00:47 wangticketyes24-0.95.dist-info/RECORD
-12 files, 96977 bytes uncompressed, 26539 bytes compressed:  72.6%
+-rw-r--r--  2.0 unx       61 b- defN 23-Jun-20 11:17 wangticketyes24-1.0.dist-info/DESCRIPTION.rst
+-rw-r--r--  2.0 unx      690 b- defN 23-Jun-20 11:17 wangticketyes24-1.0.dist-info/metadata.json
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-20 11:17 wangticketyes24-1.0.dist-info/top_level.txt
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-20 11:17 wangticketyes24-1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx      575 b- defN 23-Jun-20 11:17 wangticketyes24-1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx     1034 b- defN 23-Jun-20 11:17 wangticketyes24-1.0.dist-info/RECORD
+12 files, 96986 bytes uncompressed, 26541 bytes compressed:  72.6%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: yes24ticket/selenium_yes24.py
 Comment: 
 
 Filename: yes24ticket/yes24test.py
 Comment: 
 
-Filename: wangticketyes24-0.95.dist-info/DESCRIPTION.rst
+Filename: wangticketyes24-1.0.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: wangticketyes24-0.95.dist-info/metadata.json
+Filename: wangticketyes24-1.0.dist-info/metadata.json
 Comment: 
 
-Filename: wangticketyes24-0.95.dist-info/top_level.txt
+Filename: wangticketyes24-1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: wangticketyes24-0.95.dist-info/WHEEL
+Filename: wangticketyes24-1.0.dist-info/WHEEL
 Comment: 
 
-Filename: wangticketyes24-0.95.dist-info/METADATA
+Filename: wangticketyes24-1.0.dist-info/METADATA
 Comment: 
 
-Filename: wangticketyes24-0.95.dist-info/RECORD
+Filename: wangticketyes24-1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wangticketyes24/__init__.py

```diff
@@ -1,5 +1,5 @@
 name = "wangticketyes24"
-__version__ = "0.95"
+__version__ = "1.0"
 
 from .yes24 import Yes24
 from .selenium_yes24 import Selenium_yes24
```

## wangticketyes24/yes24.py

```diff
@@ -484,15 +484,15 @@
 		payload = {'idHall':idhall,'idTime':idtime,'block':block,'channel':1,'idCustomer':idcustomer,'idOrg':1}
 		headers = {'User-Agent':'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_11_3) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.102 Safari/537.36'}
 		#headers['Host'] = 'ticket.yes24.com'
 		#headers['Origin'] = 'http://ticket.yes24.com'
 		#headers['X-Requested-With'] = 'XMLHttpRequest'
 		headers['Pragma'] = 'no-cache'
 		r = self.session.post(URL, headers=headers, data=payload)
-		print("[Seat]", r.status_code, r.reason, r.headers['Date'], end='\r')
+		print("[Seat][{}]".format(block), r.status_code, r.reason, r.headers['Date'], end='\r')
 		#print(r.text)
 
 		root = ET.fromstring(r.text)
 		ns = "{http://tempuri.org/}"
 		#print(root.findtext('{}IdTime'.format(ns)))
 		#print(root.findtext('{}Block'.format(ns)))
 		layout = root.findtext('{}Layout'.format(ns))
```

## Comparing `wangticketyes24-0.95.dist-info/metadata.json` & `wangticketyes24-1.0.dist-info/metadata.json`

 * *Files 2% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9545454545454546%*

 * *Differences: {"'version'": "'1.0'"}*

```diff
@@ -33,9 +33,9 @@
                 "beautifulsoup4",
                 "requests",
                 "selenium"
             ]
         }
     ],
     "summary": "wangticket for y",
-    "version": "0.95"
+    "version": "1.0"
 }
```

## Comparing `wangticketyes24-0.95.dist-info/METADATA` & `wangticketyes24-1.0.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.0
 Name: wangticketyes24
-Version: 0.95
+Version: 1.0
 Summary: wangticket for y
 Home-page: https://gitlab.com/wangticket/yes24-ticket
 Author: Wangticket
 Author-email: wangticket77@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `wangticketyes24-0.95.dist-info/RECORD` & `wangticketyes24-1.0.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-wangticketyes24/__init__.py,sha256=mg8SLW1u3fUWHX7YUUeEdxApvI5Ny1ohXzIHeYhNG58,115
+wangticketyes24/__init__.py,sha256=ONZA4u6KufwRqA0RQcnXNdSOTnesZ3DduiGcRjHZw1Q,114
 wangticketyes24/selenium_yes24.py,sha256=maWgh1gXUw8-LqKkXcAZHuhyluyvwymUBK-8PUC2uek,28280
-wangticketyes24/yes24.py,sha256=943Mh-foz9fwlJ_931tgJpvDzmHqWSp2EwXquVHW5UM,43062
-wangticketyes24-0.95.dist-info/DESCRIPTION.rst,sha256=iA1-u5zGsM2eQRcqv1-vqBiJevH0U-KhtkZxpjzmfx4,61
-wangticketyes24-0.95.dist-info/METADATA,sha256=C76O0kpMd06iKBJUVBxLQtSaHZ3C1N-8hhyiEPFidTI,576
-wangticketyes24-0.95.dist-info/RECORD,,
-wangticketyes24-0.95.dist-info/WHEEL,sha256=8Lm45v9gcYRm70DrgFGVe4WsUtUMi1_0Tso1hqPGMjA,92
-wangticketyes24-0.95.dist-info/metadata.json,sha256=6FFk8-Djfbt-vA6xN5jSjL6sEMd6oiA-T7j9rtZGpP4,691
-wangticketyes24-0.95.dist-info/top_level.txt,sha256=gHGxU_Wfy3Ly7zkKLxm67DoXktNcwN0ImDzlhzNaiW4,16
+wangticketyes24/yes24.py,sha256=iCopqbnuryIMeVs0ygUNEl7vXh2xh6onFLBKlDwT2i0,43080
+wangticketyes24-1.0.dist-info/DESCRIPTION.rst,sha256=iA1-u5zGsM2eQRcqv1-vqBiJevH0U-KhtkZxpjzmfx4,61
+wangticketyes24-1.0.dist-info/METADATA,sha256=F13YMysam1ZYXOF6bdYFqC1veY1NnxD6iZWHF-8U5Gc,575
+wangticketyes24-1.0.dist-info/RECORD,,
+wangticketyes24-1.0.dist-info/WHEEL,sha256=8Lm45v9gcYRm70DrgFGVe4WsUtUMi1_0Tso1hqPGMjA,92
+wangticketyes24-1.0.dist-info/metadata.json,sha256=7qkmUeHvxv12yGCvuZ2-0qIhYvv6DjuPjKJheuzlDjY,690
+wangticketyes24-1.0.dist-info/top_level.txt,sha256=gHGxU_Wfy3Ly7zkKLxm67DoXktNcwN0ImDzlhzNaiW4,16
 yes24ticket/__init__.py,sha256=amffzfln3WNiLWWyUul39xXObS4TmQRza8OBgfN24M8,94
 yes24ticket/selenium_yes24.py,sha256=z6ataHl-e3AVhQTZFSYPdn1OfSOklBTizd2mLA57DAM,7490
 yes24ticket/yes24test.py,sha256=6my-oQh4NITv3IkaT_W_v61Z5iPDqNmDU6b3Qx9N5l8,15460
```

