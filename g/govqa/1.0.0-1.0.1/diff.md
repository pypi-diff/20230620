# Comparing `tmp/govqa-1.0.0-py3-none-any.whl.zip` & `tmp/govqa-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 8788 bytes, number of entries: 7
--rw-r--r--  2.0 unx      174 b- defN 23-Jun-05 13:50 govqa/__init__.py
--rw-r--r--  2.0 unx    22945 b- defN 23-Jun-05 13:50 govqa/base.py
--rw-r--r--  2.0 unx     5584 b- defN 23-Jun-05 13:50 govqa/input_types.py
--rw-r--r--  2.0 unx     1038 b- defN 23-Jun-05 13:50 govqa-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-05 13:50 govqa-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Jun-05 13:50 govqa-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      510 b- defN 23-Jun-05 13:50 govqa-1.0.0.dist-info/RECORD
-7 files, 30349 bytes uncompressed, 7894 bytes compressed:  74.0%
+Zip file size: 8739 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      174 b- defN 23-Jun-20 17:16 govqa/__init__.py
+-rw-r--r--  2.0 unx    22746 b- defN 23-Jun-20 17:16 govqa/base.py
+-rw-r--r--  2.0 unx     5584 b- defN 23-Jun-20 17:16 govqa/input_types.py
+-rw-r--r--  2.0 unx     1038 b- defN 23-Jun-20 17:16 govqa-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-20 17:16 govqa-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-20 17:16 govqa-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      510 b- defN 23-Jun-20 17:16 govqa-1.0.1.dist-info/RECORD
+7 files, 30150 bytes uncompressed, 7845 bytes compressed:  74.0%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: govqa/base.py
 Comment: 
 
 Filename: govqa/input_types.py
 Comment: 
 
-Filename: govqa-1.0.0.dist-info/METADATA
+Filename: govqa-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: govqa-1.0.0.dist-info/WHEEL
+Filename: govqa-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: govqa-1.0.0.dist-info/top_level.txt
+Filename: govqa-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: govqa-1.0.0.dist-info/RECORD
+Filename: govqa-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## govqa/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 from .base import (
     EmailAlreadyExists,
     FormValidationError,
     GovQA,
     IncorrectCaptcha,
     UnauthenticatedError,
```

## govqa/base.py

```diff
@@ -300,23 +300,16 @@
         truncated_message_url = self.url_from_endpoint(truncated_message_endpoint)
         response = self.get(truncated_message_url)
         tree = lxml.html.fromstring(response.text)
         body = tree.xpath(".//div[@id='divMessage']//text()")
         return body
 
     def _check_logged_in(self, response):
-        if (
-            not (
-                "Logged in as" in response.text
-                or "var loggedInCustomerEmail" in response.text
-                or 'title="Logout"' in response.text
-            )
-            or "If you have used this service previously, please log in"
-            in response.text
-        ):
+        results = re.search('dtrum.identifyUser\("(.*)"\);', response.text).group(1)
+        if not results.split(";")[-1]:
             raise UnauthenticatedError(
                 "This method requires authentication, please run the `login` method before calling this method"
             )
 
 
 class Form:
     def _process_inputs(self, required_inputs_tables, tree, response):
```

## Comparing `govqa-1.0.0.dist-info/METADATA` & `govqa-1.0.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: govqa
-Version: 1.0.0
+Version: 1.0.1
 Summary: Interact with GovQA, a public records request management platform owned by Granicus
 Home-page: https://datamade.us
 Author: DataMade
 Author-email: info@datamade.us
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

