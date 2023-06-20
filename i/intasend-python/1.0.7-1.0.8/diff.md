# Comparing `tmp/intasend_python-1.0.7-py3-none-any.whl.zip` & `tmp/intasend_python-1.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 7345 bytes, number of entries: 14
+Zip file size: 7343 bytes, number of entries: 14
 -rw-r--r--  2.0 unx      610 b- defN 23-Feb-02 10:54 intasend/__init__.py
 -rw-r--r--  2.0 unx      657 b- defN 22-Jul-13 05:21 intasend/chargebacks.py
 -rw-r--r--  2.0 unx     1653 b- defN 23-Mar-08 06:05 intasend/client.py
--rw-r--r--  2.0 unx     3516 b- defN 23-Mar-08 06:05 intasend/collections.py
+-rw-r--r--  2.0 unx     3529 b- defN 23-Jun-20 05:25 intasend/collections.py
 -rw-r--r--  2.0 unx      629 b- defN 22-Jul-13 05:21 intasend/customers.py
 -rw-r--r--  2.0 unx      193 b- defN 22-Jul-13 05:21 intasend/exceptions.py
 -rw-r--r--  2.0 unx      973 b- defN 22-Jul-13 05:21 intasend/payment_links.py
 -rw-r--r--  2.0 unx     1751 b- defN 23-Feb-02 10:33 intasend/transfers.py
 -rw-r--r--  2.0 unx     1777 b- defN 22-Jul-13 05:27 intasend/wallets.py
--rw-r--r--  2.0 unx     1065 b- defN 23-Mar-08 06:06 intasend_python-1.0.7.dist-info/LICENSE
--rw-r--r--  2.0 unx      717 b- defN 23-Mar-08 06:06 intasend_python-1.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-08 06:06 intasend_python-1.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Mar-08 06:06 intasend_python-1.0.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1124 b- defN 23-Mar-08 06:06 intasend_python-1.0.7.dist-info/RECORD
-14 files, 14766 bytes uncompressed, 5477 bytes compressed:  62.9%
+-rw-r--r--  2.0 unx     1065 b- defN 23-Jun-20 05:28 intasend_python-1.0.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx      717 b- defN 23-Jun-20 05:28 intasend_python-1.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-20 05:28 intasend_python-1.0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-20 05:28 intasend_python-1.0.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1124 b- defN 23-Jun-20 05:28 intasend_python-1.0.8.dist-info/RECORD
+14 files, 14779 bytes uncompressed, 5475 bytes compressed:  63.0%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: intasend/transfers.py
 Comment: 
 
 Filename: intasend/wallets.py
 Comment: 
 
-Filename: intasend_python-1.0.7.dist-info/LICENSE
+Filename: intasend_python-1.0.8.dist-info/LICENSE
 Comment: 
 
-Filename: intasend_python-1.0.7.dist-info/METADATA
+Filename: intasend_python-1.0.8.dist-info/METADATA
 Comment: 
 
-Filename: intasend_python-1.0.7.dist-info/WHEEL
+Filename: intasend_python-1.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: intasend_python-1.0.7.dist-info/top_level.txt
+Filename: intasend_python-1.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: intasend_python-1.0.7.dist-info/RECORD
+Filename: intasend_python-1.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## intasend/collections.py

```diff
@@ -38,15 +38,15 @@
             "phone_number": phone_number,
             "mobile_tarrif": mobile_tarrif,
             "card_tarrif": card_tarrif,
             "version": "3.0.0"
         }
         if wallet_id:
             payload.update({"wallet_id": wallet_id})
-        return self.send_request("POST", "checkout/", payload)
+        return self.send_request("POST", "checkout/", payload, noauth=True)
 
     def status(self, invoice_id, checkout_id=None, signature=None):
         """
         Check status of transaction/invoice
 
         Args:
             invoice_id (string): Invoice or tracking ID
```

## Comparing `intasend_python-1.0.7.dist-info/LICENSE` & `intasend_python-1.0.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `intasend_python-1.0.7.dist-info/METADATA` & `intasend_python-1.0.8.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: intasend-python
-Version: 1.0.7
+Version: 1.0.8
 Summary: Official Python SDK for IntaSend Payments Gateway API
 Home-page: https://github.com/IntaSend/intasend-python
-Download-URL: https://github.com/IntaSend/intasend-python/archive/v_1.0.7.tar.gz
+Download-URL: https://github.com/IntaSend/intasend-python/archive/v_1.0.8.tar.gz
 Author: Felix Cheruiyot
 Author-email: support@intasend.com
 License: MIT
 Keywords: payments,mpesa,mpesa api,card payments,visa,mastercard,payments kenya,intasend,airtime
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

## Comparing `intasend_python-1.0.7.dist-info/RECORD` & `intasend_python-1.0.8.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 intasend/__init__.py,sha256=7Vqb25ShJyvA3uFU483d538b7F6IuHOHE4ubfukColc,610
 intasend/chargebacks.py,sha256=Y54aLR53tZhtltzEtv7uupN_0PPVQv1u6X34WfahTpc,657
 intasend/client.py,sha256=b7AoNyBvebnf6BrSSaLdGg70ndoZzBRK3PHBkr9Yfso,1653
-intasend/collections.py,sha256=fl-8u9KULK4S25SKodDB5s3rOGTI5tY9eopxguYd-pE,3516
+intasend/collections.py,sha256=dc0StlJfNW2pY12yPLOui6dkjxwMTsqGh_2B6ry70C4,3529
 intasend/customers.py,sha256=shAK9_Lx_IyhqpXwmDXpUAQaD2-Fr6Cx6HHMJkQzWfg,629
 intasend/exceptions.py,sha256=oxpyWxEG9Kj0iCNEkjQfjX0FTRLJXw36DCVHqg6NaK8,193
 intasend/payment_links.py,sha256=XFWmgzXquG9yu_-IIddbktg0ypUowLgxl-xXbGzxawg,973
 intasend/transfers.py,sha256=umn_1KDU-27waclr29s9pGZ8y7sOJQT25gs368fJoxw,1751
 intasend/wallets.py,sha256=nyhDl220zj0n6qu54jsa3APsdsOcTPEePZymeWDhpe0,1777
-intasend_python-1.0.7.dist-info/LICENSE,sha256=RewJxBGucRqY7Y6BDe0Sh6-79QSDqiB5-Xdij0puCcI,1065
-intasend_python-1.0.7.dist-info/METADATA,sha256=keww_Vqp6_amAAqkLQWCaevgzYQaoz00zRKWhL5lgVY,717
-intasend_python-1.0.7.dist-info/WHEEL,sha256=00yskusixUoUt5ob_CiUp6LsnN5lqzTJpoqOFg_FVIc,92
-intasend_python-1.0.7.dist-info/top_level.txt,sha256=90p78HPoeNyNgXPr7V7S9dSGhDSWdfRC-H7TUbKvieQ,9
-intasend_python-1.0.7.dist-info/RECORD,,
+intasend_python-1.0.8.dist-info/LICENSE,sha256=RewJxBGucRqY7Y6BDe0Sh6-79QSDqiB5-Xdij0puCcI,1065
+intasend_python-1.0.8.dist-info/METADATA,sha256=YG3cKH0AImPgnTDXLxODMgWw51Tqb7iVvP4oUDuZlWg,717
+intasend_python-1.0.8.dist-info/WHEEL,sha256=00yskusixUoUt5ob_CiUp6LsnN5lqzTJpoqOFg_FVIc,92
+intasend_python-1.0.8.dist-info/top_level.txt,sha256=90p78HPoeNyNgXPr7V7S9dSGhDSWdfRC-H7TUbKvieQ,9
+intasend_python-1.0.8.dist-info/RECORD,,
```

