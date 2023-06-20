# Comparing `tmp/shortloop_python-0.1.2.tar.gz` & `tmp/shortloop_python-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shortloop_python-0.1.2.tar", max compression
+gzip compressed data, was "shortloop_python-0.1.3.tar", max compression
```

## Comparing `shortloop_python-0.1.2.tar` & `shortloop_python-0.1.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0      439 2023-06-12 11:23:58.944592 shortloop_python-0.1.2/README.md
--rw-r--r--   0        0        0     1220 2023-06-12 12:15:27.651927 shortloop_python-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       57 2023-06-12 11:23:58.945584 shortloop_python-0.1.2/shortloop_python/__init__.py
--rw-r--r--   0        0        0        0 2023-06-12 11:23:58.945789 shortloop_python-0.1.2/shortloop_python/core/__init__.py
--rw-r--r--   0        0        0     1617 2023-06-12 11:23:58.946003 shortloop_python-0.1.2/shortloop_python/core/always_capture_sync.py
--rw-r--r--   0        0        0     6347 2023-06-12 11:23:58.946179 shortloop_python-0.1.2/shortloop_python/core/api_processor.py
--rw-r--r--   0        0        0     3118 2023-06-12 11:23:58.946336 shortloop_python-0.1.2/shortloop_python/core/auto_configuration.py
--rw-r--r--   0        0        0     1765 2023-06-12 11:23:58.946538 shortloop_python-0.1.2/shortloop_python/core/buffer/abstract_buffer_manager.py
--rw-r--r--   0        0        0      842 2023-06-12 11:23:58.946678 shortloop_python-0.1.2/shortloop_python/core/buffer/api_buffer_key.py
--rw-r--r--   0        0        0      404 2023-06-12 11:23:58.946866 shortloop_python-0.1.2/shortloop_python/core/buffer/buffer.py
--rw-r--r--   0        0        0     1908 2023-06-12 11:23:58.947004 shortloop_python-0.1.2/shortloop_python/core/buffer/buffer_manager_worker.py
--rw-r--r--   0        0        0     3111 2023-06-12 11:23:58.947157 shortloop_python-0.1.2/shortloop_python/core/buffer/discovered_buffer_manager.py
--rw-r--r--   0        0        0      548 2023-06-12 11:23:58.947291 shortloop_python-0.1.2/shortloop_python/core/buffer/no_op_buffer_manager.py
--rw-r--r--   0        0        0     4027 2023-06-12 11:23:58.947419 shortloop_python-0.1.2/shortloop_python/core/buffer/registered_buffer_manager.py
--rw-r--r--   0        0        0      832 2023-06-12 11:23:58.947572 shortloop_python-0.1.2/shortloop_python/core/buffer/simple_buffer.py
--rw-r--r--   0        0        0      373 2023-06-12 11:23:58.947779 shortloop_python-0.1.2/shortloop_python/core/config/config_manager.py
--rw-r--r--   0        0        0      316 2023-06-12 11:23:58.947921 shortloop_python-0.1.2/shortloop_python/core/config/config_update_listener.py
--rw-r--r--   0        0        0     1921 2023-06-12 11:23:58.948077 shortloop_python-0.1.2/shortloop_python/core/config/config_validators.py
--rw-r--r--   0        0        0     4233 2023-06-12 11:23:58.948247 shortloop_python-0.1.2/shortloop_python/core/config/simple_config_manager.py
--rw-r--r--   0        0        0      140 2023-06-12 11:23:58.948592 shortloop_python-0.1.2/shortloop_python/core/constant/__init__.py
--rw-r--r--   0        0        0      207 2023-06-12 11:23:58.948773 shortloop_python-0.1.2/shortloop_python/core/constant/http_method.py
--rw-r--r--   0        0        0      156 2023-06-12 11:23:58.949037 shortloop_python-0.1.2/shortloop_python/core/constant/segment_template_type.py
--rw-r--r--   0        0        0      163 2023-06-12 11:23:58.949294 shortloop_python-0.1.2/shortloop_python/core/filter/__init__.py
--rw-r--r--   0        0        0     1148 2023-06-12 11:23:58.949442 shortloop_python-0.1.2/shortloop_python/core/filter/always_capture_filter.py
--rw-r--r--   0        0        0     3041 2023-06-12 11:23:58.949593 shortloop_python-0.1.2/shortloop_python/core/filter/filter.py
--rw-r--r--   0        0        0      271 2023-06-12 11:23:58.949807 shortloop_python-0.1.2/shortloop_python/core/http/__init__.py
--rw-r--r--   0        0        0     2845 2023-06-12 11:23:58.949952 shortloop_python-0.1.2/shortloop_python/core/http/context.py
--rw-r--r--   0        0        0     5232 2023-06-12 11:23:58.950111 shortloop_python-0.1.2/shortloop_python/core/http/http_connection.py
--rw-r--r--   0        0        0     1260 2023-06-12 11:23:58.950257 shortloop_python-0.1.2/shortloop_python/core/http/http_request.py
--rw-r--r--   0        0        0      267 2023-06-12 11:23:58.950434 shortloop_python-0.1.2/shortloop_python/core/http/http_response.py
--rw-r--r--   0        0        0      350 2023-06-12 11:23:58.950634 shortloop_python-0.1.2/shortloop_python/core/model/__init__.py
--rw-r--r--   0        0        0     2044 2023-06-12 11:23:58.950778 shortloop_python-0.1.2/shortloop_python/core/model/agent_config.py
--rw-r--r--   0        0        0      692 2023-06-12 11:23:58.950913 shortloop_python-0.1.2/shortloop_python/core/model/api_config.py
--rw-r--r--   0        0        0     3277 2023-06-12 11:23:58.951048 shortloop_python-0.1.2/shortloop_python/core/model/api_sample.py
--rw-r--r--   0        0        0     1122 2023-06-12 11:23:58.951183 shortloop_python-0.1.2/shortloop_python/core/model/black_list_rule.py
--rw-r--r--   0        0        0      536 2023-06-12 11:23:58.951348 shortloop_python-0.1.2/shortloop_python/core/model/observed_api.py
--rw-r--r--   0        0        0     2068 2023-06-12 11:23:58.951520 shortloop_python-0.1.2/shortloop_python/core/model/sdk_options.py
--rw-r--r--   0        0        0     1955 2023-06-12 11:23:58.951686 shortloop_python-0.1.2/shortloop_python/core/model/uri.py
--rw-r--r--   0        0        0      199 2023-06-12 11:23:58.951820 shortloop_python-0.1.2/shortloop_python/core/scheduled_timer.py
--rw-r--r--   0        0        0     2112 2023-06-12 12:15:06.900107 shortloop_python-0.1.2/shortloop_python/core/shortlook_sdk.py
--rw-r--r--   0        0        0     1184 2023-06-12 11:23:58.952193 shortloop_python-0.1.2/shortloop_python/core/util/filter_utils.py
--rw-r--r--   0        0        0      420 2023-06-12 11:23:58.952340 shortloop_python-0.1.2/shortloop_python/core/util/masking_utils.py
--rw-r--r--   0        0        0      929 2023-06-12 11:23:58.952476 shortloop_python-0.1.2/shortloop_python/core/util/uri_utils.py
--rw-r--r--   0        0        0       87 2023-06-12 11:23:58.952669 shortloop_python-0.1.2/shortloop_python/integrations/__init__.py
--rw-r--r--   0        0        0     2255 2023-06-12 11:23:58.952960 shortloop_python-0.1.2/shortloop_python/integrations/django.py
--rw-r--r--   0        0        0      558 2023-06-12 11:23:58.953206 shortloop_python-0.1.2/shortloop_python/sdk_logger.py
--rw-r--r--   0        0        0      152 2023-06-12 11:23:58.953369 shortloop_python-0.1.2/shortloop_python/sdk_version.py
--rw-r--r--   0        0        0     1423 1970-01-01 00:00:00.000000 shortloop_python-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      439 2023-06-12 11:23:58.944592 shortloop_python-0.1.3/README.md
+-rw-r--r--   0        0        0     1220 2023-06-20 08:54:06.886117 shortloop_python-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       57 2023-06-12 11:23:58.945584 shortloop_python-0.1.3/shortloop_python/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 11:23:58.945789 shortloop_python-0.1.3/shortloop_python/core/__init__.py
+-rw-r--r--   0        0        0     1617 2023-06-12 11:23:58.946003 shortloop_python-0.1.3/shortloop_python/core/always_capture_sync.py
+-rw-r--r--   0        0        0     6347 2023-06-12 11:23:58.946179 shortloop_python-0.1.3/shortloop_python/core/api_processor.py
+-rw-r--r--   0        0        0     3118 2023-06-12 11:23:58.946336 shortloop_python-0.1.3/shortloop_python/core/auto_configuration.py
+-rw-r--r--   0        0        0     1765 2023-06-12 11:23:58.946538 shortloop_python-0.1.3/shortloop_python/core/buffer/abstract_buffer_manager.py
+-rw-r--r--   0        0        0      842 2023-06-12 11:23:58.946678 shortloop_python-0.1.3/shortloop_python/core/buffer/api_buffer_key.py
+-rw-r--r--   0        0        0      404 2023-06-12 11:23:58.946866 shortloop_python-0.1.3/shortloop_python/core/buffer/buffer.py
+-rw-r--r--   0        0        0     1908 2023-06-12 11:23:58.947004 shortloop_python-0.1.3/shortloop_python/core/buffer/buffer_manager_worker.py
+-rw-r--r--   0        0        0     3111 2023-06-12 11:23:58.947157 shortloop_python-0.1.3/shortloop_python/core/buffer/discovered_buffer_manager.py
+-rw-r--r--   0        0        0      548 2023-06-12 11:23:58.947291 shortloop_python-0.1.3/shortloop_python/core/buffer/no_op_buffer_manager.py
+-rw-r--r--   0        0        0     4027 2023-06-12 11:23:58.947419 shortloop_python-0.1.3/shortloop_python/core/buffer/registered_buffer_manager.py
+-rw-r--r--   0        0        0      832 2023-06-12 11:23:58.947572 shortloop_python-0.1.3/shortloop_python/core/buffer/simple_buffer.py
+-rw-r--r--   0        0        0      373 2023-06-12 11:23:58.947779 shortloop_python-0.1.3/shortloop_python/core/config/config_manager.py
+-rw-r--r--   0        0        0      316 2023-06-12 11:23:58.947921 shortloop_python-0.1.3/shortloop_python/core/config/config_update_listener.py
+-rw-r--r--   0        0        0     1921 2023-06-12 11:23:58.948077 shortloop_python-0.1.3/shortloop_python/core/config/config_validators.py
+-rw-r--r--   0        0        0     4233 2023-06-12 11:23:58.948247 shortloop_python-0.1.3/shortloop_python/core/config/simple_config_manager.py
+-rw-r--r--   0        0        0      140 2023-06-12 11:23:58.948592 shortloop_python-0.1.3/shortloop_python/core/constant/__init__.py
+-rw-r--r--   0        0        0      207 2023-06-12 11:23:58.948773 shortloop_python-0.1.3/shortloop_python/core/constant/http_method.py
+-rw-r--r--   0        0        0      156 2023-06-12 11:23:58.949037 shortloop_python-0.1.3/shortloop_python/core/constant/segment_template_type.py
+-rw-r--r--   0        0        0      163 2023-06-12 11:23:58.949294 shortloop_python-0.1.3/shortloop_python/core/filter/__init__.py
+-rw-r--r--   0        0        0     1148 2023-06-12 11:23:58.949442 shortloop_python-0.1.3/shortloop_python/core/filter/always_capture_filter.py
+-rw-r--r--   0        0        0     3041 2023-06-12 11:23:58.949593 shortloop_python-0.1.3/shortloop_python/core/filter/filter.py
+-rw-r--r--   0        0        0      271 2023-06-12 11:23:58.949807 shortloop_python-0.1.3/shortloop_python/core/http/__init__.py
+-rw-r--r--   0        0        0     2845 2023-06-12 11:23:58.949952 shortloop_python-0.1.3/shortloop_python/core/http/context.py
+-rw-r--r--   0        0        0     5232 2023-06-12 11:23:58.950111 shortloop_python-0.1.3/shortloop_python/core/http/http_connection.py
+-rw-r--r--   0        0        0     1260 2023-06-12 11:23:58.950257 shortloop_python-0.1.3/shortloop_python/core/http/http_request.py
+-rw-r--r--   0        0        0      267 2023-06-12 11:23:58.950434 shortloop_python-0.1.3/shortloop_python/core/http/http_response.py
+-rw-r--r--   0        0        0      350 2023-06-12 11:23:58.950634 shortloop_python-0.1.3/shortloop_python/core/model/__init__.py
+-rw-r--r--   0        0        0     2044 2023-06-12 11:23:58.950778 shortloop_python-0.1.3/shortloop_python/core/model/agent_config.py
+-rw-r--r--   0        0        0      692 2023-06-12 11:23:58.950913 shortloop_python-0.1.3/shortloop_python/core/model/api_config.py
+-rw-r--r--   0        0        0     3277 2023-06-12 11:23:58.951048 shortloop_python-0.1.3/shortloop_python/core/model/api_sample.py
+-rw-r--r--   0        0        0     1122 2023-06-12 11:23:58.951183 shortloop_python-0.1.3/shortloop_python/core/model/black_list_rule.py
+-rw-r--r--   0        0        0      536 2023-06-12 11:23:58.951348 shortloop_python-0.1.3/shortloop_python/core/model/observed_api.py
+-rw-r--r--   0        0        0     2068 2023-06-12 11:23:58.951520 shortloop_python-0.1.3/shortloop_python/core/model/sdk_options.py
+-rw-r--r--   0        0        0     1955 2023-06-12 11:23:58.951686 shortloop_python-0.1.3/shortloop_python/core/model/uri.py
+-rw-r--r--   0        0        0      199 2023-06-12 11:23:58.951820 shortloop_python-0.1.3/shortloop_python/core/scheduled_timer.py
+-rw-r--r--   0        0        0     2290 2023-06-20 08:53:46.661321 shortloop_python-0.1.3/shortloop_python/core/shortlook_sdk.py
+-rw-r--r--   0        0        0     1184 2023-06-12 11:23:58.952193 shortloop_python-0.1.3/shortloop_python/core/util/filter_utils.py
+-rw-r--r--   0        0        0      420 2023-06-12 11:23:58.952340 shortloop_python-0.1.3/shortloop_python/core/util/masking_utils.py
+-rw-r--r--   0        0        0      929 2023-06-12 11:23:58.952476 shortloop_python-0.1.3/shortloop_python/core/util/uri_utils.py
+-rw-r--r--   0        0        0       87 2023-06-12 11:23:58.952669 shortloop_python-0.1.3/shortloop_python/integrations/__init__.py
+-rw-r--r--   0        0        0     2255 2023-06-12 11:23:58.952960 shortloop_python-0.1.3/shortloop_python/integrations/django.py
+-rw-r--r--   0        0        0      558 2023-06-12 11:23:58.953206 shortloop_python-0.1.3/shortloop_python/sdk_logger.py
+-rw-r--r--   0        0        0      152 2023-06-12 11:23:58.953369 shortloop_python-0.1.3/shortloop_python/sdk_version.py
+-rw-r--r--   0        0        0     1423 1970-01-01 00:00:00.000000 shortloop_python-0.1.3/PKG-INFO
```

### Comparing `shortloop_python-0.1.2/pyproject.toml` & `shortloop_python-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shortloop-python"
-version = "0.1.2"
+version = "0.1.3"
 description = "Official Shortloop SDK for Python"
 authors = ["ShortLoop <hello@shortloop.dev>"]
 maintainers = ["ShortLoop <hello@shortloop.dev>"]
 homepage = "https://shortloop.dev"
 documentation = "https://docs.shortloop.dev"
 readme = "README.md"
 packages = [{include = "shortloop_python"}]
```

### Comparing `shortloop_python-0.1.2/shortloop_python/core/always_capture_sync.py` & `shortloop_python-0.1.3/shortloop_python/core/always_capture_sync.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.2/shortloop_python/core/api_processor.py` & `shortloop_python-0.1.3/shortloop_python/core/api_processor.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.2/shortloop_python/core/auto_configuration.py` & `shortloop_python-0.1.3/shortloop_python/core/auto_configuration.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.2/shortloop_python/core/buffer/abstract_buffer_manager.py` & `shortloop_python-0.1.3/shortloop_python/core/buffer/abstract_buffer_manager.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.2/shortloop_python/core/buffer/api_buffer_key.py` & `shortloop_python-0.1.3/shortloop_python/core/buffer/api_buffer_key.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.2/shortloop_python/core/buffer/buffer_manager_worker.py` & `shortloop_python-0.1.3/shortloop_python/core/buffer/buffer_manager_worker.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.2/shortloop_python/core/buffer/discovered_buffer_manager.py` & `shortloop_python-0.1.3/shortloop_python/core/buffer/discovered_buffer_manager.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.2/shortloop_python/core/buffer/no_op_buffer_manager.py` & `shortloop_python-0.1.3/shortloop_python/core/buffer/no_op_buffer_manager.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.2/shortloop_python/core/buffer/registered_buffer_manager.py` & `shortloop_python-0.1.3/shortloop_python/core/buffer/registered_buffer_manager.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.2/shortloop_python/core/buffer/simple_buffer.py` & `shortloop_python-0.1.3/shortloop_python/core/buffer/simple_buffer.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.2/shortloop_python/core/config/config_validators.py` & `shortloop_python-0.1.3/shortloop_python/core/config/config_validators.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.2/shortloop_python/core/config/simple_config_manager.py` & `shortloop_python-0.1.3/shortloop_python/core/config/simple_config_manager.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.2/shortloop_python/core/filter/always_capture_filter.py` & `shortloop_python-0.1.3/shortloop_python/core/filter/always_capture_filter.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.2/shortloop_python/core/filter/filter.py` & `shortloop_python-0.1.3/shortloop_python/core/filter/filter.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.2/shortloop_python/core/http/context.py` & `shortloop_python-0.1.3/shortloop_python/core/http/context.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.2/shortloop_python/core/http/http_connection.py` & `shortloop_python-0.1.3/shortloop_python/core/http/http_connection.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.2/shortloop_python/core/http/http_request.py` & `shortloop_python-0.1.3/shortloop_python/core/http/http_request.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.2/shortloop_python/core/model/agent_config.py` & `shortloop_python-0.1.3/shortloop_python/core/model/agent_config.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.2/shortloop_python/core/model/api_config.py` & `shortloop_python-0.1.3/shortloop_python/core/model/api_config.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.2/shortloop_python/core/model/api_sample.py` & `shortloop_python-0.1.3/shortloop_python/core/model/api_sample.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.2/shortloop_python/core/model/black_list_rule.py` & `shortloop_python-0.1.3/shortloop_python/core/model/black_list_rule.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.2/shortloop_python/core/model/observed_api.py` & `shortloop_python-0.1.3/shortloop_python/core/model/observed_api.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.2/shortloop_python/core/model/sdk_options.py` & `shortloop_python-0.1.3/shortloop_python/core/model/sdk_options.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.2/shortloop_python/core/model/uri.py` & `shortloop_python-0.1.3/shortloop_python/core/model/uri.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.2/shortloop_python/core/shortlook_sdk.py` & `shortloop_python-0.1.3/shortloop_python/core/shortlook_sdk.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,15 +41,16 @@
     :param list(int) mask_headers: Headers names (case in-sensitive) that will be masked at the SDK level itself.
         Masking will happen locally before data is sent to ShortLoop servers. Ex: ["cookie", "x-auth"]
 
     :param str capture: TEST MODE
     """
     global options, initialized, auto_configuration
 
-    if 'check' in sys.argv:
+    # sdk fails in django-admin commands. we only allow sdk to run if runserver django admin command was used
+    if len(sys.argv) >= 2 and sys.argv[0].endswith("manage.py") and sys.argv[1] != "runserver":
         return
 
     if not initialized:
         initialized = True
 
         opts: SdkOptions = SdkOptions(
             url, application_name, auth_key, environment, logging_enabled, log_level, mask_headers, capture
```

### Comparing `shortloop_python-0.1.2/shortloop_python/core/util/filter_utils.py` & `shortloop_python-0.1.3/shortloop_python/core/util/filter_utils.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.2/shortloop_python/core/util/uri_utils.py` & `shortloop_python-0.1.3/shortloop_python/core/util/uri_utils.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.2/shortloop_python/integrations/django.py` & `shortloop_python-0.1.3/shortloop_python/integrations/django.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.2/shortloop_python/sdk_logger.py` & `shortloop_python-0.1.3/shortloop_python/sdk_logger.py`

 * *Files identical despite different names*

### Comparing `shortloop_python-0.1.2/PKG-INFO` & `shortloop_python-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shortloop-python
-Version: 0.1.2
+Version: 0.1.3
 Summary: Official Shortloop SDK for Python
 Home-page: https://shortloop.dev
 Keywords: shortloop,middleware
 Author: ShortLoop
 Author-email: hello@shortloop.dev
 Maintainer: ShortLoop
 Maintainer-email: hello@shortloop.dev
```

