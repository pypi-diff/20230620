# Comparing `tmp/wedeliver_core_plus-0.0.4.tar.gz` & `tmp/wedeliver_core_plus-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/platformLibraries/platformLibraries/wedeliver_core_plus/dist/.tmp-kjm4d_km/wedeliver_core_plus-0.0.4.tar", last modified: Thu Jun 15 10:37:08 2023, max compression
+gzip compressed data, was "/home/runner/work/platformLibraries/platformLibraries/wedeliver_core_plus/dist/.tmp-z6rxjeh9/wedeliver_core_plus-0.0.5.tar", last modified: Tue Jun 20 11:23:06 2023, max compression
```

## Comparing `wedeliver_core_plus-0.0.4.tar` & `wedeliver_core_plus-0.0.5.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:37:08.000000 wedeliver_core_plus-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (122)      773 2023-06-15 10:37:08.000000 wedeliver_core_plus-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-15 10:37:08.000000 wedeliver_core_plus-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1368 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:37:08.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/
--rw-r--r--   0 runner    (1001) docker     (122)      893 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:37:08.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/app_decorators/
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/app_decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1012 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/app_decorators/app_entry.py
--rw-r--r--   0 runner    (1001) docker     (122)     2272 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/app_decorators/handle_auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     2374 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/app_decorators/handle_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      786 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/app_decorators/handle_response.py
--rw-r--r--   0 runner    (1001) docker     (122)     4721 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/app_decorators/serializer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2398 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:37:08.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      855 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/acl_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:37:08.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/amazon/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/amazon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      593 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/amazon/append_plain_urls_to_list_dict.py
--rw-r--r--   0 runner    (1001) docker     (122)     1360 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/amazon/get_file_url.py
--rw-r--r--   0 runner    (1001) docker     (122)      318 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/amazon/get_plain_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     1607 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/amazon/get_s3_client.py
--rw-r--r--   0 runner    (1001) docker     (122)      590 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/amazon/upload_file.py
--rw-r--r--   0 runner    (1001) docker     (122)      852 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/atomic_transactions.py
--rw-r--r--   0 runner    (1001) docker     (122)      940 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/atomic_transactions_v2.py
--rw-r--r--   0 runner    (1001) docker     (122)     1844 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:37:08.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/database/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      703 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/database/base_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     4009 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/database/log_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2251 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/enums.py
--rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3719 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/fetch_relational_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     4730 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/format_exception.py
--rw-r--r--   0 runner    (1001) docker     (122)      385 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/get_callback.py
--rw-r--r--   0 runner    (1001) docker     (122)      223 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/get_country_code.py
--rw-r--r--   0 runner    (1001) docker     (122)      629 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/get_embedded_function.py
--rw-r--r--   0 runner    (1001) docker     (122)      424 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/get_obj_value.py
--rw-r--r--   0 runner    (1001) docker     (122)      342 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/get_prefix.py
--rw-r--r--   0 runner    (1001) docker     (122)     2768 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/kafka_listener.py
--rw-r--r--   0 runner    (1001) docker     (122)     3056 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/kafka_producer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:37:08.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/kafka_producers/
--rw-r--r--   0 runner    (1001) docker     (122)      302 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/kafka_producers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      372 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/kafka_producers/log_model_changes.py
--rw-r--r--   0 runner    (1001) docker     (122)     2094 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/kafka_producers/notification_center.py
--rw-r--r--   0 runner    (1001) docker     (122)      290 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/kafka_producers/send_sms.py
--rw-r--r--   0 runner    (1001) docker     (122)      322 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/kafka_producers/send_topic.py
--rw-r--r--   0 runner    (1001) docker     (122)     2007 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/log_config.py
--rw-r--r--   0 runner    (1001) docker     (122)    12499 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/micro_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/numbers.py
--rw-r--r--   0 runner    (1001) docker     (122)     4284 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/search_function.py
--rw-r--r--   0 runner    (1001) docker     (122)     2021 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/security.py
--rw-r--r--   0 runner    (1001) docker     (122)      663 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/service_config.py
--rw-r--r--   0 runner    (1001) docker     (122)      850 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/sql.py
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/system_roles.py
--rw-r--r--   0 runner    (1001) docker     (122)     7639 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/time.py
--rw-r--r--   0 runner    (1001) docker     (122)      393 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/topics.py
--rw-r--r--   0 runner    (1001) docker     (122)     1205 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/validate_mobile_number.py
--rw-r--r--   0 runner    (1001) docker     (122)     1002 2023-06-15 10:36:48.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/validate_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-15 10:37:08.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      773 2023-06-15 10:37:08.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2678 2023-06-15 10:37:08.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-15 10:37:08.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-06-15 10:37:08.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-06-15 10:37:08.000000 wedeliver_core_plus-0.0.4/wedeliver_core_plus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 11:23:06.000000 wedeliver_core_plus-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (122)      773 2023-06-20 11:23:06.000000 wedeliver_core_plus-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-20 11:23:06.000000 wedeliver_core_plus-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1368 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 11:23:06.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/
+-rw-r--r--   0 runner    (1001) docker     (122)      893 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 11:23:06.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/app_decorators/
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/app_decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1012 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/app_decorators/app_entry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2272 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/app_decorators/handle_auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2374 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/app_decorators/handle_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      786 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/app_decorators/handle_response.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4721 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/app_decorators/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2398 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 11:23:06.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      855 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/acl_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 11:23:06.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/amazon/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/amazon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      593 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/amazon/append_plain_urls_to_list_dict.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1360 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/amazon/get_file_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)      318 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/amazon/get_plain_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1607 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/amazon/get_s3_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      590 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/amazon/upload_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)      852 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/atomic_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      940 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/atomic_transactions_v2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1844 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 11:23:06.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/database/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      703 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/database/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4418 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/database/log_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2251 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3719 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/fetch_relational_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4730 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/format_exception.py
+-rw-r--r--   0 runner    (1001) docker     (122)      385 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/get_callback.py
+-rw-r--r--   0 runner    (1001) docker     (122)      223 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/get_country_code.py
+-rw-r--r--   0 runner    (1001) docker     (122)      629 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/get_embedded_function.py
+-rw-r--r--   0 runner    (1001) docker     (122)      424 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/get_obj_value.py
+-rw-r--r--   0 runner    (1001) docker     (122)      342 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/get_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2768 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/kafka_listener.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3056 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/kafka_producer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 11:23:06.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/kafka_producers/
+-rw-r--r--   0 runner    (1001) docker     (122)      378 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/kafka_producers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      451 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/kafka_producers/log_model_changes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2098 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/kafka_producers/notification_center.py
+-rw-r--r--   0 runner    (1001) docker     (122)      292 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/kafka_producers/send_sms.py
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/kafka_producers/send_topic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2007 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12487 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/micro_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/numbers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4284 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/search_function.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2021 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/security.py
+-rw-r--r--   0 runner    (1001) docker     (122)      663 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/service_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      850 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/sql.py
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/system_roles.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7639 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/time.py
+-rw-r--r--   0 runner    (1001) docker     (122)      629 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/topics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1205 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/validate_mobile_number.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1002 2023-06-20 11:22:51.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/validate_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 11:23:06.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      773 2023-06-20 11:23:06.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2678 2023-06-20 11:23:06.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-20 11:23:06.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-06-20 11:23:06.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-06-20 11:23:06.000000 wedeliver_core_plus-0.0.5/wedeliver_core_plus.egg-info/top_level.txt
```

### Comparing `wedeliver_core_plus-0.0.4/PKG-INFO` & `wedeliver_core_plus-0.0.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wedeliver_core_plus
-Version: 0.0.4
+Version: 0.0.5
 Summary: wedeliver_core_plus package
 Home-page: https://www.wedeliverapp.com/
 Author: Eyad Farra
 Author-email: info@wedeliverapp.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `wedeliver_core_plus-0.0.4/setup.py` & `wedeliver_core_plus-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "Programming Language :: Python :: 3.4",
     "Programming Language :: Python :: 3.5",
     "Programming Language :: Python :: 3.6",
 ]
 
 setup(
     name="wedeliver_core_plus",
-    version="0.0.4",
+    version="0.0.5",
     description="wedeliver_core_plus package",
     long_description="""# Markdown supported!\n\n* wedeliver core plus\n* List of features\n""",
     long_description_content_type="text/markdown",
     url="https://www.wedeliverapp.com/",
     author="Eyad Farra",
     author_email="info@wedeliverapp.com",
     license="MIT",
```

### Comparing `wedeliver_core_plus-0.0.4/wedeliver_core_plus/__init__.py` & `wedeliver_core_plus-0.0.5/wedeliver_core_plus/__init__.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.4/wedeliver_core_plus/app_decorators/app_entry.py` & `wedeliver_core_plus-0.0.5/wedeliver_core_plus/app_decorators/app_entry.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.4/wedeliver_core_plus/app_decorators/handle_auth.py` & `wedeliver_core_plus-0.0.5/wedeliver_core_plus/app_decorators/handle_auth.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.4/wedeliver_core_plus/app_decorators/handle_exceptions.py` & `wedeliver_core_plus-0.0.5/wedeliver_core_plus/app_decorators/handle_exceptions.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.4/wedeliver_core_plus/app_decorators/handle_response.py` & `wedeliver_core_plus-0.0.5/wedeliver_core_plus/app_decorators/handle_response.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.4/wedeliver_core_plus/app_decorators/serializer.py` & `wedeliver_core_plus-0.0.5/wedeliver_core_plus/app_decorators/serializer.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.4/wedeliver_core_plus/base.py` & `wedeliver_core_plus-0.0.5/wedeliver_core_plus/base.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/acl_enum.py` & `wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/acl_enum.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/amazon/append_plain_urls_to_list_dict.py` & `wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/amazon/append_plain_urls_to_list_dict.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/amazon/get_file_url.py` & `wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/amazon/get_file_url.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/amazon/get_s3_client.py` & `wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/amazon/get_s3_client.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/amazon/upload_file.py` & `wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/amazon/upload_file.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/atomic_transactions.py` & `wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/atomic_transactions.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/atomic_transactions_v2.py` & `wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/atomic_transactions_v2.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/auth.py` & `wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/auth.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/config.py` & `wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/config.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/database/base_model.py` & `wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/database/base_model.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/database/log_model.py` & `wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/database/log_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from sqlalchemy import event, inspect
 from sqlalchemy.orm import object_mapper, ColumnProperty
 
 from wedeliver_core_plus import WedeliverCorePlus, Auth
-from wedeliver_core_plus.helpers.kafka_producers.log_model_changes import log_model_changes
+from wedeliver_core_plus.helpers import kafka_producers
 
+has_registered_event = False
 
 def init_log_model():
+    global has_registered_event
+
     app = WedeliverCorePlus.get_app()
     db = app.extensions['sqlalchemy'].db
 
     class LogModel(db.Model):
         __abstract__ = True
         __log_column_changes__ = []
         __log_parent_instance__ = None
@@ -63,30 +66,40 @@
                 parent_model_instance_id=parent_model_instance_id,
                 column_changes=column_changes,
                 action_type=action_type
             )
             log_changes(changes)
 
     def log_changes(changes):
-        log_model_changes(changes)
+        kafka_producers.log_model_changes(changes, kafka_configs=dict(
+                service_name="LOG_SERVICE"
+            ))
 
     def on_after_flush(session, flush_context):
+        if app.config.get("NO_LOGGING_SERVICE"):
+            app.logger.info("NO_LOGGING_SERVICE is set to True, skipping logging changes")
+            return
+
         try:
             deleted_objects = session.deleted
             changed_objects = session.dirty
             new_objects = session.new
             for o in changed_objects:
-                if session.is_modified(o, include_collections=True) and hasattr(o,
-                                                                                '__log_column_changes__') and o.__log_column_changes__:
+                if session.is_modified(o, include_collections=True) and\
+                        hasattr(o, '__log_column_changes__') and \
+                        o.__log_column_changes__:
                     trigger_attribute_change_events(o)
             for o in deleted_objects:
                 if hasattr(o, '__log_column_changes__') and o.__log_column_changes__:
                     trigger_attribute_change_events(o, is_deleted=True)
             for o in new_objects:
                 if hasattr(o, '__log_column_changes__') and o.__log_column_changes__:
                     trigger_attribute_change_events(o, is_added=True)
         except Exception as e:
             app.logger.error("error while logging changes: ", str(e))
 
-    event.listen(db.session, "after_flush", on_after_flush)
+    # Only register the event listener if it hasn't been registered yet
+    if not has_registered_event:
+        event.listen(db.session, "after_flush", on_after_flush)
+        has_registered_event = True
 
     return LogModel
```

### Comparing `wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/enums.py` & `wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/enums.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/exceptions.py` & `wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/exceptions.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/fetch_relational_data.py` & `wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/fetch_relational_data.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/filters.py` & `wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/filters.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/format_exception.py` & `wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/format_exception.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/get_embedded_function.py` & `wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/get_embedded_function.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/kafka_listener.py` & `wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/kafka_listener.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/kafka_producer.py` & `wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/kafka_producer.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/kafka_producers/notification_center.py` & `wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/kafka_producers/notification_center.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
                 title, str(app.config.get("SERVICE_NAME"))
             ),
             "text": message,
             "color": color,
             "icon_emoji": emoji,
         },
     }
-    kafka_producers.send_topic(topic=Topics.INTERNAL_NOTIFICATION_MESSAGE, datajson=data)
+    kafka_producers.send_topic(topic=Topics().INTERNAL_NOTIFICATION_MESSAGE, datajson=data)
 
 
 def send_push_notification(
         message_text, reference_type, user_ids, title=None, payload=None, created_by=None, **kwargs
 ):
     # token = None
 
@@ -57,11 +57,11 @@
         created_by=created_by,
         title=title or "Thrivve",
         message_text=message_text,
         payload=payload,
         # language="ar"
     )
 
-    kafka_producers.send_topic(topic=Topics.THRIVVE_SEND_PUSH_NOTIFICATION, datajson=dict(
+    kafka_producers.send_topic(topic=Topics().THRIVVE_SEND_PUSH_NOTIFICATION, datajson=dict(
         function_name='app.business_logic.notification.send_push_notification.execute',
         function_params=data
     ), kafka_configs=kwargs.get('kafka_configs'))
```

### Comparing `wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/log_config.py` & `wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/log_config.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/micro_fetcher.py` & `wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/micro_fetcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
         env_service_url = self.app.config.get(service_name)
 
         self.service_url = env_service_url if env_service_url else service_url
 
         self.service_name = service_name
         if not self.service_url:
-            raise AppMicroFetcherError('Service {} not defined on Env or in ServiceConfig'.format(self.service_url))
+            raise AppMicroFetcherError(f'Service {service_name} not defined on Env or in ServiceConfig')
 
     def join(self, base_data, output_key=None):
         self.base_data = base_data
         self.query_type = QueryTypes.SIMPLE_TABLE.value
         if output_key:
             output_key = output_key.split('as ')[1]
```

### Comparing `wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/search_function.py` & `wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/search_function.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/security.py` & `wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/security.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/service_config.py` & `wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/service_config.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/sql.py` & `wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/sql.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/time.py` & `wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/time.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/validate_mobile_number.py` & `wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/validate_mobile_number.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.4/wedeliver_core_plus/helpers/validate_parameters.py` & `wedeliver_core_plus-0.0.5/wedeliver_core_plus/helpers/validate_parameters.py`

 * *Files identical despite different names*

### Comparing `wedeliver_core_plus-0.0.4/wedeliver_core_plus.egg-info/PKG-INFO` & `wedeliver_core_plus-0.0.5/wedeliver_core_plus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wedeliver-core-plus
-Version: 0.0.4
+Version: 0.0.5
 Summary: wedeliver_core_plus package
 Home-page: https://www.wedeliverapp.com/
 Author: Eyad Farra
 Author-email: info@wedeliverapp.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `wedeliver_core_plus-0.0.4/wedeliver_core_plus.egg-info/SOURCES.txt` & `wedeliver_core_plus-0.0.5/wedeliver_core_plus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

