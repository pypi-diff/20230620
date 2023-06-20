# Comparing `tmp/python_tes_shopify-1.0.1.tar.gz` & `tmp/python_tes_shopify-1.0.2.tar.gz`

## Comparing `python_tes_shopify-1.0.1.tar` & `python_tes_shopify-1.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 python_tes_shopify-1.0.1/tes_shopify/__init__.py
--rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 python_tes_shopify-1.0.1/tes_shopify/client.py
--rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 python_tes_shopify-1.0.1/tes_shopify/resources.py
--rw-r--r--   0        0        0     5030 2020-02-02 00:00:00.000000 python_tes_shopify-1.0.1/tes_shopify/shopify_utils.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 python_tes_shopify-1.0.1/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 python_tes_shopify-1.0.1/LICENSE
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 python_tes_shopify-1.0.1/README.md
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 python_tes_shopify-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 python_tes_shopify-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 python_tes_shopify-1.0.2/tes_shopify/__init__.py
+-rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 python_tes_shopify-1.0.2/tes_shopify/client.py
+-rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 python_tes_shopify-1.0.2/tes_shopify/resources.py
+-rw-r--r--   0        0        0     5030 2020-02-02 00:00:00.000000 python_tes_shopify-1.0.2/tes_shopify/shopify_utils.py
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 python_tes_shopify-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 python_tes_shopify-1.0.2/LICENSE
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 python_tes_shopify-1.0.2/README.md
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 python_tes_shopify-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 python_tes_shopify-1.0.2/PKG-INFO
```

### Comparing `python_tes_shopify-1.0.1/tes_shopify/client.py` & `python_tes_shopify-1.0.2/tes_shopify/client.py`

 * *Files identical despite different names*

### Comparing `python_tes_shopify-1.0.1/tes_shopify/resources.py` & `python_tes_shopify-1.0.2/tes_shopify/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     redirect_url = ShopifyUtils.generate_post_install_redirect_url(shop=shop)
     ShopifyUtils.app_installed()
     return "{}", 302, "application/json", redirect_url
 
 
 # @API.post("/webhooks/uninstalled")
 @ShopifyUtils.verify_webhook_call
-def uninstalled():
+def webhooks_uninstalled():
     webhook_topic = API.request.headers.get("X-Shopify-Topic")
     webhook_payload = API.request.data
     resp_content = json.dumps(webhook_payload, indent=4)
     logging.error(f"webhook call received {webhook_topic}:\n{resp_content}")
     ShopifyUtils.app_remove()
     return "OK"
```

### Comparing `python_tes_shopify-1.0.1/tes_shopify/shopify_utils.py` & `python_tes_shopify-1.0.2/tes_shopify/shopify_utils.py`

 * *Files identical despite different names*

### Comparing `python_tes_shopify-1.0.1/.gitignore` & `python_tes_shopify-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `python_tes_shopify-1.0.1/LICENSE` & `python_tes_shopify-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_tes_shopify-1.0.1/pyproject.toml` & `python_tes_shopify-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "python_tes_shopify"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
     { name="Johannes Eimer", email="johannes.eimer@jep-dev.com" },
 ]
 description = "Python TES Business Objects"
 readme = "README.md"
 requires-python = ">=3.9"
 license = "MIT"
```

### Comparing `python_tes_shopify-1.0.1/PKG-INFO` & `python_tes_shopify-1.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python_tes_shopify
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python TES Business Objects
 Author-email: Johannes Eimer <johannes.eimer@jep-dev.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: Python,Shopify,TES
 Requires-Python: >=3.9
 Requires-Dist: python-tes~=0.3.19
```

