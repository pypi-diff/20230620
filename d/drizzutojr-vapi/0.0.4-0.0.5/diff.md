# Comparing `tmp/drizzutojr_vapi-0.0.4-py3-none-any.whl.zip` & `tmp/drizzutojr_vapi-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4036 bytes, number of entries: 8
--rw-r--r--  2.0 unx       49 b- defN 23-Jun-18 22:29 vapi/__init__.py
--rw-r--r--  2.0 unx     1164 b- defN 23-Jun-18 22:29 vapi/exceptions.py
--rw-r--r--  2.0 unx     5798 b- defN 23-Jun-18 22:29 vapi/vapi.py
--rw-r--r--  2.0 unx     1061 b- defN 23-Jun-18 22:31 drizzutojr_vapi-0.0.4.dist-info/LICENSE.md
--rw-r--r--  2.0 unx      200 b- defN 23-Jun-18 22:31 drizzutojr_vapi-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-18 22:31 drizzutojr_vapi-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Jun-18 22:31 drizzutojr_vapi-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      642 b- defN 23-Jun-18 22:31 drizzutojr_vapi-0.0.4.dist-info/RECORD
-8 files, 9011 bytes uncompressed, 2910 bytes compressed:  67.7%
+Zip file size: 4061 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-20 04:01 vapi/__init__.py
+-rw-r--r--  2.0 unx     1344 b- defN 23-Jun-20 04:01 vapi/exceptions.py
+-rw-r--r--  2.0 unx     5798 b- defN 23-Jun-20 04:01 vapi/vapi.py
+-rw-r--r--  2.0 unx     1061 b- defN 23-Jun-20 04:03 drizzutojr_vapi-0.0.5.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx      200 b- defN 23-Jun-20 04:03 drizzutojr_vapi-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-20 04:03 drizzutojr_vapi-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-20 04:03 drizzutojr_vapi-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      642 b- defN 23-Jun-20 04:03 drizzutojr_vapi-0.0.5.dist-info/RECORD
+8 files, 9191 bytes uncompressed, 2935 bytes compressed:  68.1%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: vapi/exceptions.py
 Comment: 
 
 Filename: vapi/vapi.py
 Comment: 
 
-Filename: drizzutojr_vapi-0.0.4.dist-info/LICENSE.md
+Filename: drizzutojr_vapi-0.0.5.dist-info/LICENSE.md
 Comment: 
 
-Filename: drizzutojr_vapi-0.0.4.dist-info/METADATA
+Filename: drizzutojr_vapi-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: drizzutojr_vapi-0.0.4.dist-info/WHEEL
+Filename: drizzutojr_vapi-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: drizzutojr_vapi-0.0.4.dist-info/top_level.txt
+Filename: drizzutojr_vapi-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: drizzutojr_vapi-0.0.4.dist-info/RECORD
+Filename: drizzutojr_vapi-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vapi/exceptions.py

```diff
@@ -1,23 +1,26 @@
 DEFAULT_STATUS_CODE = 400
 
 
 def vapi_exception_handler(exception):
     return {
         "message": str(exception.message),
-        "status_code": exception.status_code,
-        "response": exception.response,
-        "errors": exception.errors,
-    }, exception.status_code
+        "status_code": getattr(exception, "status_code", None),
+        "response": getattr(exception, "response", None),
+        "errors": getattr(exception, "errors", None),
+    }, getattr(exception, "status_code", DEFAULT_STATUS_CODE)
 
 
 class VAPIGenericError(Exception):
-    def __init__(self, message: str, details: str = ""):
+    def __init__(
+        self, message: str, details: str = "", status_code: int = DEFAULT_STATUS_CODE
+    ):
         self.message = message
         self.details = details
+        self.status_code = status_code
         super().__init__(self.message)
 
 
 class VAPIConfigError(VAPIGenericError):
     """Vault returned an Error"""
```

## Comparing `drizzutojr_vapi-0.0.4.dist-info/LICENSE.md` & `drizzutojr_vapi-0.0.5.dist-info/LICENSE.md`

 * *Files identical despite different names*

