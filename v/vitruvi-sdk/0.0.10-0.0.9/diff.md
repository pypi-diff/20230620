# Comparing `tmp/vitruvi_sdk-0.0.10.tar.gz` & `tmp/vitruvi_sdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vitruvi_sdk-0.0.10.tar", max compression
+gzip compressed data, was "vitruvi_sdk-0.0.9.tar", max compression
```

## Comparing `vitruvi_sdk-0.0.10.tar` & `vitruvi_sdk-0.0.9.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0     2274 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/README.md
--rw-r--r--   0        0        0      374 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/pyproject.toml
--rw-r--r--   0        0        0     3434 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/__init__.py
--rw-r--r--   0        0        0     1451 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/client.py
--rw-r--r--   0        0        0      348 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/core/__init__.py
--rw-r--r--   0        0        0      426 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      203 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/errors/__init__.py
--rw-r--r--   0        0        0      248 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/errors/bad_request_error.py
--rw-r--r--   0        0        0      246 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/errors/not_found_error.py
--rw-r--r--   0        0        0        0 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/py.typed
--rw-r--r--   0        0        0      188 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/resources/auth/__init__.py
--rw-r--r--   0        0        0    29772 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/resources/auth/client.py
--rw-r--r--   0        0        0       65 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/resources/global_configuration/__init__.py
--rw-r--r--   0        0        0    23219 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/resources/global_configuration/client.py
--rw-r--r--   0        0        0       65 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/resources/jobs/__init__.py
--rw-r--r--   0        0        0     2459 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/resources/jobs/client.py
--rw-r--r--   0        0        0       65 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/resources/reporting/__init__.py
--rw-r--r--   0        0        0    80912 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/resources/reporting/client.py
--rw-r--r--   0        0        0     4976 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/types/__init__.py
--rw-r--r--   0        0        0      915 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/types/account.py
--rw-r--r--   0        0        0     1653 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/types/accounts_payable_item_export.py
--rw-r--r--   0        0        0     1656 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/types/accounts_receivable_item_export.py
--rw-r--r--   0        0        0      746 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/types/async_api_result.py
--rw-r--r--   0        0        0     2197 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/types/company.py
--rw-r--r--   0        0        0      627 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/types/company_type_enum.py
--rw-r--r--   0        0        0      861 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/types/crew_export.py
--rw-r--r--   0        0        0      814 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/types/crew_member_export.py
--rw-r--r--   0        0        0     1105 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/types/custom_field_settings_export.py
--rw-r--r--   0        0        0     1343 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/types/design_element_export.py
--rw-r--r--   0        0        0      920 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/types/design_export.py
--rw-r--r--   0        0        0      749 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/types/error_message.py
--rw-r--r--   0        0        0      804 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/types/full_crew_person_role.py
--rw-r--r--   0        0        0      672 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/types/global_configuration_list_companies_request_type.py
--rw-r--r--   0        0        0     1415 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/types/invoice_export.py
--rw-r--r--   0        0        0      993 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/types/paginated_accounts_payable_item_export_list.py
--rw-r--r--   0        0        0     1005 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/types/paginated_accounts_receivable_item_export_list.py
--rw-r--r--   0        0        0      918 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/types/paginated_company_list.py
--rw-r--r--   0        0        0      931 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/types/paginated_crew_export_list.py
--rw-r--r--   0        0        0      956 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/types/paginated_crew_member_export_list.py
--rw-r--r--   0        0        0      993 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/types/paginated_custom_field_settings_export_list.py
--rw-r--r--   0        0        0      968 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/types/paginated_design_element_export_list.py
--rw-r--r--   0        0        0      939 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/types/paginated_design_export_list.py
--rw-r--r--   0        0        0      943 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/types/paginated_invoice_export_list.py
--rw-r--r--   0        0        0      930 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/types/paginated_permission_list.py
--rw-r--r--   0        0        0      980 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/types/paginated_production_report_export_list.py
--rw-r--r--   0        0        0      997 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/types/paginated_production_report_line_export_list.py
--rw-r--r--   0        0        0     1013 2023-06-20 01:56:58.330487 vitruvi_sdk-0.0.10/src/vitruvi/types/paginated_production_report_quantity_export_list.py
--rw-r--r--   0        0        0      943 2023-06-20 01:56:58.334488 vitruvi_sdk-0.0.10/src/vitruvi/types/paginated_profile_export_list.py
--rw-r--r--   0        0        0      939 2023-06-20 01:56:58.334488 vitruvi_sdk-0.0.10/src/vitruvi/types/paginated_region_export_list.py
--rw-r--r--   0        0        0      906 2023-06-20 01:56:58.334488 vitruvi_sdk-0.0.10/src/vitruvi/types/paginated_results.py
--rw-r--r--   0        0        0      906 2023-06-20 01:56:58.334488 vitruvi_sdk-0.0.10/src/vitruvi/types/paginated_role_list.py
--rw-r--r--   0        0        0      935 2023-06-20 01:56:58.334488 vitruvi_sdk-0.0.10/src/vitruvi/types/paginated_scope_export_list.py
--rw-r--r--   0        0        0      948 2023-06-20 01:56:58.334488 vitruvi_sdk-0.0.10/src/vitruvi/types/paginated_work_item_export_list.py
--rw-r--r--   0        0        0      981 2023-06-20 01:56:58.334488 vitruvi_sdk-0.0.10/src/vitruvi/types/paginated_work_item_quantity_export_list.py
--rw-r--r--   0        0        0      952 2023-06-20 01:56:58.334488 vitruvi_sdk-0.0.10/src/vitruvi/types/paginated_work_order_export_list.py
--rw-r--r--   0        0        0      960 2023-06-20 01:56:58.334488 vitruvi_sdk-0.0.10/src/vitruvi/types/paginated_work_package_export_list.py
--rw-r--r--   0        0        0      774 2023-06-20 01:56:58.334488 vitruvi_sdk-0.0.10/src/vitruvi/types/permission.py
--rw-r--r--   0        0        0     1211 2023-06-20 01:56:58.334488 vitruvi_sdk-0.0.10/src/vitruvi/types/production_report_export.py
--rw-r--r--   0        0        0     1094 2023-06-20 01:56:58.334488 vitruvi_sdk-0.0.10/src/vitruvi/types/production_report_line_export.py
--rw-r--r--   0        0        0     1218 2023-06-20 01:56:58.334488 vitruvi_sdk-0.0.10/src/vitruvi/types/production_report_quantity_export.py
--rw-r--r--   0        0        0     2423 2023-06-20 01:56:58.334488 vitruvi_sdk-0.0.10/src/vitruvi/types/profile.py
--rw-r--r--   0        0        0      992 2023-06-20 01:56:58.334488 vitruvi_sdk-0.0.10/src/vitruvi/types/profile_export.py
--rw-r--r--   0        0        0      793 2023-06-20 01:56:58.334488 vitruvi_sdk-0.0.10/src/vitruvi/types/refresh_token.py
--rw-r--r--   0        0        0     1000 2023-06-20 01:56:58.334488 vitruvi_sdk-0.0.10/src/vitruvi/types/region_export.py
--rw-r--r--   0        0        0      801 2023-06-20 01:56:58.334488 vitruvi_sdk-0.0.10/src/vitruvi/types/role.py
--rw-r--r--   0        0        0      876 2023-06-20 01:56:58.334488 vitruvi_sdk-0.0.10/src/vitruvi/types/scope_export.py
--rw-r--r--   0        0        0      863 2023-06-20 01:56:58.334488 vitruvi_sdk-0.0.10/src/vitruvi/types/user_info.py
--rw-r--r--   0        0        0     1312 2023-06-20 01:56:58.334488 vitruvi_sdk-0.0.10/src/vitruvi/types/user_tier_enum.py
--rw-r--r--   0        0        0      813 2023-06-20 01:56:58.334488 vitruvi_sdk-0.0.10/src/vitruvi/types/verify_json_web_token.py
--rw-r--r--   0        0        0      987 2023-06-20 01:56:58.334488 vitruvi_sdk-0.0.10/src/vitruvi/types/web_token.py
--rw-r--r--   0        0        0     1294 2023-06-20 01:56:58.334488 vitruvi_sdk-0.0.10/src/vitruvi/types/work_item_export.py
--rw-r--r--   0        0        0     1101 2023-06-20 01:56:58.334488 vitruvi_sdk-0.0.10/src/vitruvi/types/work_item_quantity_export.py
--rw-r--r--   0        0        0     1375 2023-06-20 01:56:58.334488 vitruvi_sdk-0.0.10/src/vitruvi/types/work_order_export.py
--rw-r--r--   0        0        0     1329 2023-06-20 01:56:58.334488 vitruvi_sdk-0.0.10/src/vitruvi/types/work_package_export.py
--rw-r--r--   0        0        0     2783 1970-01-01 00:00:00.000000 vitruvi_sdk-0.0.10/PKG-INFO
+-rw-r--r--   0        0        0     2274 2023-06-20 00:47:11.783031 vitruvi_sdk-0.0.9/README.md
+-rw-r--r--   0        0        0      373 2023-06-20 00:47:11.783031 vitruvi_sdk-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3438 2023-06-20 00:47:11.783031 vitruvi_sdk-0.0.9/src/vitruvi/__init__.py
+-rw-r--r--   0        0        0     1451 2023-06-20 00:47:11.783031 vitruvi_sdk-0.0.9/src/vitruvi/client.py
+-rw-r--r--   0        0        0      348 2023-06-20 00:47:11.783031 vitruvi_sdk-0.0.9/src/vitruvi/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-06-20 00:47:11.783031 vitruvi_sdk-0.0.9/src/vitruvi/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-06-20 00:47:11.783031 vitruvi_sdk-0.0.9/src/vitruvi/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-06-20 00:47:11.783031 vitruvi_sdk-0.0.9/src/vitruvi/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-06-20 00:47:11.783031 vitruvi_sdk-0.0.9/src/vitruvi/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      203 2023-06-20 00:47:11.783031 vitruvi_sdk-0.0.9/src/vitruvi/errors/__init__.py
+-rw-r--r--   0        0        0      248 2023-06-20 00:47:11.783031 vitruvi_sdk-0.0.9/src/vitruvi/errors/bad_request_error.py
+-rw-r--r--   0        0        0      246 2023-06-20 00:47:11.783031 vitruvi_sdk-0.0.9/src/vitruvi/errors/not_found_error.py
+-rw-r--r--   0        0        0        0 2023-06-20 00:47:11.783031 vitruvi_sdk-0.0.9/src/vitruvi/py.typed
+-rw-r--r--   0        0        0      188 2023-06-20 00:47:11.783031 vitruvi_sdk-0.0.9/src/vitruvi/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-06-20 00:47:11.783031 vitruvi_sdk-0.0.9/src/vitruvi/resources/auth/__init__.py
+-rw-r--r--   0        0        0    29772 2023-06-20 00:47:11.787031 vitruvi_sdk-0.0.9/src/vitruvi/resources/auth/client.py
+-rw-r--r--   0        0        0       65 2023-06-20 00:47:11.787031 vitruvi_sdk-0.0.9/src/vitruvi/resources/global_configuration/__init__.py
+-rw-r--r--   0        0        0    23277 2023-06-20 00:47:11.787031 vitruvi_sdk-0.0.9/src/vitruvi/resources/global_configuration/client.py
+-rw-r--r--   0        0        0       65 2023-06-20 00:47:11.787031 vitruvi_sdk-0.0.9/src/vitruvi/resources/jobs/__init__.py
+-rw-r--r--   0        0        0     2459 2023-06-20 00:47:11.787031 vitruvi_sdk-0.0.9/src/vitruvi/resources/jobs/client.py
+-rw-r--r--   0        0        0       65 2023-06-20 00:47:11.787031 vitruvi_sdk-0.0.9/src/vitruvi/resources/reporting/__init__.py
+-rw-r--r--   0        0        0    80912 2023-06-20 00:47:11.787031 vitruvi_sdk-0.0.9/src/vitruvi/resources/reporting/client.py
+-rw-r--r--   0        0        0     4984 2023-06-20 00:47:11.787031 vitruvi_sdk-0.0.9/src/vitruvi/types/__init__.py
+-rw-r--r--   0        0        0      915 2023-06-20 00:47:11.787031 vitruvi_sdk-0.0.9/src/vitruvi/types/account.py
+-rw-r--r--   0        0        0     1653 2023-06-20 00:47:11.787031 vitruvi_sdk-0.0.9/src/vitruvi/types/accounts_payable_item_export.py
+-rw-r--r--   0        0        0     1656 2023-06-20 00:47:11.787031 vitruvi_sdk-0.0.9/src/vitruvi/types/accounts_receivable_item_export.py
+-rw-r--r--   0        0        0      746 2023-06-20 00:47:11.787031 vitruvi_sdk-0.0.9/src/vitruvi/types/async_api_result.py
+-rw-r--r--   0        0        0     2197 2023-06-20 00:47:11.787031 vitruvi_sdk-0.0.9/src/vitruvi/types/company.py
+-rw-r--r--   0        0        0      627 2023-06-20 00:47:11.787031 vitruvi_sdk-0.0.9/src/vitruvi/types/company_type_enum.py
+-rw-r--r--   0        0        0      861 2023-06-20 00:47:11.787031 vitruvi_sdk-0.0.9/src/vitruvi/types/crew_export.py
+-rw-r--r--   0        0        0      814 2023-06-20 00:47:11.787031 vitruvi_sdk-0.0.9/src/vitruvi/types/crew_member_export.py
+-rw-r--r--   0        0        0     1105 2023-06-20 00:47:11.787031 vitruvi_sdk-0.0.9/src/vitruvi/types/custom_field_settings_export.py
+-rw-r--r--   0        0        0     1343 2023-06-20 00:47:11.787031 vitruvi_sdk-0.0.9/src/vitruvi/types/design_element_export.py
+-rw-r--r--   0        0        0      920 2023-06-20 00:47:11.787031 vitruvi_sdk-0.0.9/src/vitruvi/types/design_export.py
+-rw-r--r--   0        0        0      749 2023-06-20 00:47:11.787031 vitruvi_sdk-0.0.9/src/vitruvi/types/error_message.py
+-rw-r--r--   0        0        0      804 2023-06-20 00:47:11.787031 vitruvi_sdk-0.0.9/src/vitruvi/types/full_crew_person_role.py
+-rw-r--r--   0        0        0      680 2023-06-20 00:47:11.787031 vitruvi_sdk-0.0.9/src/vitruvi/types/global_configuration_list_v_1_companies_request_type.py
+-rw-r--r--   0        0        0     1415 2023-06-20 00:47:11.787031 vitruvi_sdk-0.0.9/src/vitruvi/types/invoice_export.py
+-rw-r--r--   0        0        0      993 2023-06-20 00:47:11.787031 vitruvi_sdk-0.0.9/src/vitruvi/types/paginated_accounts_payable_item_export_list.py
+-rw-r--r--   0        0        0     1005 2023-06-20 00:47:11.787031 vitruvi_sdk-0.0.9/src/vitruvi/types/paginated_accounts_receivable_item_export_list.py
+-rw-r--r--   0        0        0      918 2023-06-20 00:47:11.787031 vitruvi_sdk-0.0.9/src/vitruvi/types/paginated_company_list.py
+-rw-r--r--   0        0        0      931 2023-06-20 00:47:11.791031 vitruvi_sdk-0.0.9/src/vitruvi/types/paginated_crew_export_list.py
+-rw-r--r--   0        0        0      956 2023-06-20 00:47:11.791031 vitruvi_sdk-0.0.9/src/vitruvi/types/paginated_crew_member_export_list.py
+-rw-r--r--   0        0        0      993 2023-06-20 00:47:11.791031 vitruvi_sdk-0.0.9/src/vitruvi/types/paginated_custom_field_settings_export_list.py
+-rw-r--r--   0        0        0      968 2023-06-20 00:47:11.791031 vitruvi_sdk-0.0.9/src/vitruvi/types/paginated_design_element_export_list.py
+-rw-r--r--   0        0        0      939 2023-06-20 00:47:11.791031 vitruvi_sdk-0.0.9/src/vitruvi/types/paginated_design_export_list.py
+-rw-r--r--   0        0        0      943 2023-06-20 00:47:11.791031 vitruvi_sdk-0.0.9/src/vitruvi/types/paginated_invoice_export_list.py
+-rw-r--r--   0        0        0      930 2023-06-20 00:47:11.791031 vitruvi_sdk-0.0.9/src/vitruvi/types/paginated_permission_list.py
+-rw-r--r--   0        0        0      980 2023-06-20 00:47:11.791031 vitruvi_sdk-0.0.9/src/vitruvi/types/paginated_production_report_export_list.py
+-rw-r--r--   0        0        0      997 2023-06-20 00:47:11.791031 vitruvi_sdk-0.0.9/src/vitruvi/types/paginated_production_report_line_export_list.py
+-rw-r--r--   0        0        0     1013 2023-06-20 00:47:11.791031 vitruvi_sdk-0.0.9/src/vitruvi/types/paginated_production_report_quantity_export_list.py
+-rw-r--r--   0        0        0      943 2023-06-20 00:47:11.791031 vitruvi_sdk-0.0.9/src/vitruvi/types/paginated_profile_export_list.py
+-rw-r--r--   0        0        0      939 2023-06-20 00:47:11.791031 vitruvi_sdk-0.0.9/src/vitruvi/types/paginated_region_export_list.py
+-rw-r--r--   0        0        0      906 2023-06-20 00:47:11.791031 vitruvi_sdk-0.0.9/src/vitruvi/types/paginated_results.py
+-rw-r--r--   0        0        0      906 2023-06-20 00:47:11.791031 vitruvi_sdk-0.0.9/src/vitruvi/types/paginated_role_list.py
+-rw-r--r--   0        0        0      935 2023-06-20 00:47:11.791031 vitruvi_sdk-0.0.9/src/vitruvi/types/paginated_scope_export_list.py
+-rw-r--r--   0        0        0      948 2023-06-20 00:47:11.791031 vitruvi_sdk-0.0.9/src/vitruvi/types/paginated_work_item_export_list.py
+-rw-r--r--   0        0        0      981 2023-06-20 00:47:11.791031 vitruvi_sdk-0.0.9/src/vitruvi/types/paginated_work_item_quantity_export_list.py
+-rw-r--r--   0        0        0      952 2023-06-20 00:47:11.791031 vitruvi_sdk-0.0.9/src/vitruvi/types/paginated_work_order_export_list.py
+-rw-r--r--   0        0        0      960 2023-06-20 00:47:11.791031 vitruvi_sdk-0.0.9/src/vitruvi/types/paginated_work_package_export_list.py
+-rw-r--r--   0        0        0      774 2023-06-20 00:47:11.791031 vitruvi_sdk-0.0.9/src/vitruvi/types/permission.py
+-rw-r--r--   0        0        0     1211 2023-06-20 00:47:11.791031 vitruvi_sdk-0.0.9/src/vitruvi/types/production_report_export.py
+-rw-r--r--   0        0        0     1094 2023-06-20 00:47:11.791031 vitruvi_sdk-0.0.9/src/vitruvi/types/production_report_line_export.py
+-rw-r--r--   0        0        0     1218 2023-06-20 00:47:11.791031 vitruvi_sdk-0.0.9/src/vitruvi/types/production_report_quantity_export.py
+-rw-r--r--   0        0        0     2423 2023-06-20 00:47:11.791031 vitruvi_sdk-0.0.9/src/vitruvi/types/profile.py
+-rw-r--r--   0        0        0      992 2023-06-20 00:47:11.791031 vitruvi_sdk-0.0.9/src/vitruvi/types/profile_export.py
+-rw-r--r--   0        0        0      793 2023-06-20 00:47:11.791031 vitruvi_sdk-0.0.9/src/vitruvi/types/refresh_token.py
+-rw-r--r--   0        0        0     1000 2023-06-20 00:47:11.791031 vitruvi_sdk-0.0.9/src/vitruvi/types/region_export.py
+-rw-r--r--   0        0        0      801 2023-06-20 00:47:11.791031 vitruvi_sdk-0.0.9/src/vitruvi/types/role.py
+-rw-r--r--   0        0        0      876 2023-06-20 00:47:11.791031 vitruvi_sdk-0.0.9/src/vitruvi/types/scope_export.py
+-rw-r--r--   0        0        0      863 2023-06-20 00:47:11.791031 vitruvi_sdk-0.0.9/src/vitruvi/types/user_info.py
+-rw-r--r--   0        0        0     1312 2023-06-20 00:47:11.791031 vitruvi_sdk-0.0.9/src/vitruvi/types/user_tier_enum.py
+-rw-r--r--   0        0        0      813 2023-06-20 00:47:11.791031 vitruvi_sdk-0.0.9/src/vitruvi/types/verify_json_web_token.py
+-rw-r--r--   0        0        0      987 2023-06-20 00:47:11.791031 vitruvi_sdk-0.0.9/src/vitruvi/types/web_token.py
+-rw-r--r--   0        0        0     1294 2023-06-20 00:47:11.791031 vitruvi_sdk-0.0.9/src/vitruvi/types/work_item_export.py
+-rw-r--r--   0        0        0     1101 2023-06-20 00:47:11.791031 vitruvi_sdk-0.0.9/src/vitruvi/types/work_item_quantity_export.py
+-rw-r--r--   0        0        0     1375 2023-06-20 00:47:11.795031 vitruvi_sdk-0.0.9/src/vitruvi/types/work_order_export.py
+-rw-r--r--   0        0        0     1329 2023-06-20 00:47:11.795031 vitruvi_sdk-0.0.9/src/vitruvi/types/work_package_export.py
+-rw-r--r--   0        0        0     2782 1970-01-01 00:00:00.000000 vitruvi_sdk-0.0.9/PKG-INFO
```

### Comparing `vitruvi_sdk-0.0.10/README.md` & `vitruvi_sdk-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/__init__.py` & `vitruvi_sdk-0.0.9/src/vitruvi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     CrewExport,
     CrewMemberExport,
     CustomFieldSettingsExport,
     DesignElementExport,
     DesignExport,
     ErrorMessage,
     FullCrewPersonRole,
-    GlobalConfigurationListCompaniesRequestType,
+    GlobalConfigurationListV1CompaniesRequestType,
     InvoiceExport,
     PaginatedAccountsPayableItemExportList,
     PaginatedAccountsReceivableItemExportList,
     PaginatedCompanyList,
     PaginatedCrewExportList,
     PaginatedCrewMemberExportList,
     PaginatedCustomFieldSettingsExportList,
@@ -71,15 +71,15 @@
     "CrewExport",
     "CrewMemberExport",
     "CustomFieldSettingsExport",
     "DesignElementExport",
     "DesignExport",
     "ErrorMessage",
     "FullCrewPersonRole",
-    "GlobalConfigurationListCompaniesRequestType",
+    "GlobalConfigurationListV1CompaniesRequestType",
     "InvoiceExport",
     "NotFoundError",
     "PaginatedAccountsPayableItemExportList",
     "PaginatedAccountsReceivableItemExportList",
     "PaginatedCompanyList",
     "PaginatedCrewExportList",
     "PaginatedCrewMemberExportList",
```

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/client.py` & `vitruvi_sdk-0.0.9/src/vitruvi/client.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/core/datetime_utils.py` & `vitruvi_sdk-0.0.9/src/vitruvi/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/core/jsonable_encoder.py` & `vitruvi_sdk-0.0.9/src/vitruvi/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/resources/auth/client.py` & `vitruvi_sdk-0.0.9/src/vitruvi/resources/auth/client.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/resources/global_configuration/client.py` & `vitruvi_sdk-0.0.9/src/vitruvi/resources/global_configuration/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,38 +8,38 @@
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...types.company import Company
 from ...types.company_type_enum import CompanyTypeEnum
-from ...types.global_configuration_list_companies_request_type import GlobalConfigurationListCompaniesRequestType
+from ...types.global_configuration_list_v_1_companies_request_type import GlobalConfigurationListV1CompaniesRequestType
 from ...types.paginated_company_list import PaginatedCompanyList
 from ...types.user_tier_enum import UserTierEnum
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class GlobalConfigurationClient:
     def __init__(self, *, environment: str, api_key: str):
         self._environment = environment
         self.api_key = api_key
 
-    def list_companies(
+    def list_v_1_companies(
         self,
         *,
         code: typing.Optional[str] = None,
         fields: typing.Optional[str] = None,
         is_active: typing.Optional[bool] = None,
         limit: typing.Optional[int] = None,
         offset: typing.Optional[int] = None,
         ordering: typing.Optional[str] = None,
         search: typing.Optional[str] = None,
-        type: typing.Optional[GlobalConfigurationListCompaniesRequestType] = None,
+        type: typing.Optional[GlobalConfigurationListV1CompaniesRequestType] = None,
         with_no_subcontract: typing.Optional[int] = None,
         with_subcontract_or_epc: typing.Optional[int] = None,
     ) -> PaginatedCompanyList:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/companies"),
             params={
@@ -61,15 +61,15 @@
             return pydantic.parse_obj_as(PaginatedCompanyList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def create_companies(self, *, request: Company) -> Company:
+    def create_v_1_companies(self, *, request: Company) -> Company:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/companies"),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
@@ -77,30 +77,30 @@
             return pydantic.parse_obj_as(Company, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_companies(self, id: int) -> Company:
+    def get_v_1_companies(self, id: int) -> Company:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", f"api/v1/companies/{id}"),
             headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Company, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def update_companies(self, id: int, *, request: Company) -> Company:
+    def update_v_1_companies(self, id: int, *, request: Company) -> Company:
         _response = httpx.request(
             "PUT",
             urllib.parse.urljoin(f"{self._environment}/", f"api/v1/companies/{id}"),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
@@ -108,15 +108,15 @@
             return pydantic.parse_obj_as(Company, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def patch_companies(
+    def patch_v_1_companies(
         self,
         id: int,
         *,
         patched_company_id: typing.Optional[int] = OMIT,
         primary_contact_information: typing.Optional[str] = OMIT,
         billing_contact_information: typing.Optional[str] = OMIT,
         employee_count: typing.Optional[int] = OMIT,
@@ -228,15 +228,15 @@
             return pydantic.parse_obj_as(Company, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def delete_companies(self, id: int) -> None:
+    def delete_v_1_companies(self, id: int) -> None:
         _response = httpx.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._environment}/", f"api/v1/companies/{id}"),
             headers=remove_none_from_headers({"Authorization": self.api_key}),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
@@ -264,25 +264,25 @@
 
 
 class AsyncGlobalConfigurationClient:
     def __init__(self, *, environment: str, api_key: str):
         self._environment = environment
         self.api_key = api_key
 
-    async def list_companies(
+    async def list_v_1_companies(
         self,
         *,
         code: typing.Optional[str] = None,
         fields: typing.Optional[str] = None,
         is_active: typing.Optional[bool] = None,
         limit: typing.Optional[int] = None,
         offset: typing.Optional[int] = None,
         ordering: typing.Optional[str] = None,
         search: typing.Optional[str] = None,
-        type: typing.Optional[GlobalConfigurationListCompaniesRequestType] = None,
+        type: typing.Optional[GlobalConfigurationListV1CompaniesRequestType] = None,
         with_no_subcontract: typing.Optional[int] = None,
         with_subcontract_or_epc: typing.Optional[int] = None,
     ) -> PaginatedCompanyList:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/companies"),
@@ -305,15 +305,15 @@
             return pydantic.parse_obj_as(PaginatedCompanyList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def create_companies(self, *, request: Company) -> Company:
+    async def create_v_1_companies(self, *, request: Company) -> Company:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment}/", "api/v1/companies"),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
@@ -322,15 +322,15 @@
             return pydantic.parse_obj_as(Company, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_companies(self, id: int) -> Company:
+    async def get_v_1_companies(self, id: int) -> Company:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", f"api/v1/companies/{id}"),
                 headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
@@ -338,15 +338,15 @@
             return pydantic.parse_obj_as(Company, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def update_companies(self, id: int, *, request: Company) -> Company:
+    async def update_v_1_companies(self, id: int, *, request: Company) -> Company:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "PUT",
                 urllib.parse.urljoin(f"{self._environment}/", f"api/v1/companies/{id}"),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
@@ -355,15 +355,15 @@
             return pydantic.parse_obj_as(Company, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def patch_companies(
+    async def patch_v_1_companies(
         self,
         id: int,
         *,
         patched_company_id: typing.Optional[int] = OMIT,
         primary_contact_information: typing.Optional[str] = OMIT,
         billing_contact_information: typing.Optional[str] = OMIT,
         employee_count: typing.Optional[int] = OMIT,
@@ -476,15 +476,15 @@
             return pydantic.parse_obj_as(Company, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def delete_companies(self, id: int) -> None:
+    async def delete_v_1_companies(self, id: int) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "DELETE",
                 urllib.parse.urljoin(f"{self._environment}/", f"api/v1/companies/{id}"),
                 headers=remove_none_from_headers({"Authorization": self.api_key}),
                 timeout=60,
             )
```

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/resources/jobs/client.py` & `vitruvi_sdk-0.0.9/src/vitruvi/resources/jobs/client.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/resources/reporting/client.py` & `vitruvi_sdk-0.0.9/src/vitruvi/resources/reporting/client.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/__init__.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from .crew_export import CrewExport
 from .crew_member_export import CrewMemberExport
 from .custom_field_settings_export import CustomFieldSettingsExport
 from .design_element_export import DesignElementExport
 from .design_export import DesignExport
 from .error_message import ErrorMessage
 from .full_crew_person_role import FullCrewPersonRole
-from .global_configuration_list_companies_request_type import GlobalConfigurationListCompaniesRequestType
+from .global_configuration_list_v_1_companies_request_type import GlobalConfigurationListV1CompaniesRequestType
 from .invoice_export import InvoiceExport
 from .paginated_accounts_payable_item_export_list import PaginatedAccountsPayableItemExportList
 from .paginated_accounts_receivable_item_export_list import PaginatedAccountsReceivableItemExportList
 from .paginated_company_list import PaginatedCompanyList
 from .paginated_crew_export_list import PaginatedCrewExportList
 from .paginated_crew_member_export_list import PaginatedCrewMemberExportList
 from .paginated_custom_field_settings_export_list import PaginatedCustomFieldSettingsExportList
@@ -66,15 +66,15 @@
     "CrewExport",
     "CrewMemberExport",
     "CustomFieldSettingsExport",
     "DesignElementExport",
     "DesignExport",
     "ErrorMessage",
     "FullCrewPersonRole",
-    "GlobalConfigurationListCompaniesRequestType",
+    "GlobalConfigurationListV1CompaniesRequestType",
     "InvoiceExport",
     "PaginatedAccountsPayableItemExportList",
     "PaginatedAccountsReceivableItemExportList",
     "PaginatedCompanyList",
     "PaginatedCrewExportList",
     "PaginatedCrewMemberExportList",
     "PaginatedCustomFieldSettingsExportList",
```

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/account.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/account.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/accounts_payable_item_export.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/accounts_payable_item_export.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/accounts_receivable_item_export.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/accounts_receivable_item_export.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/async_api_result.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/async_api_result.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/company.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/company.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/company_type_enum.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/company_type_enum.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/crew_export.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/crew_export.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/crew_member_export.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/crew_member_export.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/custom_field_settings_export.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/custom_field_settings_export.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/design_element_export.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/design_element_export.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/design_export.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/design_export.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/error_message.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/error_message.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/full_crew_person_role.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/full_crew_person_role.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/invoice_export.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/invoice_export.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/paginated_accounts_payable_item_export_list.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/paginated_accounts_payable_item_export_list.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/paginated_accounts_receivable_item_export_list.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/paginated_accounts_receivable_item_export_list.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/paginated_company_list.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/paginated_company_list.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/paginated_crew_export_list.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/paginated_crew_export_list.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/paginated_crew_member_export_list.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/paginated_crew_member_export_list.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/paginated_custom_field_settings_export_list.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/paginated_custom_field_settings_export_list.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/paginated_design_element_export_list.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/paginated_design_element_export_list.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/paginated_design_export_list.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/paginated_design_export_list.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/paginated_invoice_export_list.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/paginated_invoice_export_list.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/paginated_permission_list.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/paginated_permission_list.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/paginated_production_report_export_list.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/paginated_production_report_export_list.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/paginated_production_report_line_export_list.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/paginated_production_report_line_export_list.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/paginated_production_report_quantity_export_list.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/paginated_production_report_quantity_export_list.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/paginated_profile_export_list.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/paginated_profile_export_list.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/paginated_region_export_list.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/paginated_region_export_list.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/paginated_results.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/paginated_results.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/paginated_role_list.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/paginated_role_list.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/paginated_scope_export_list.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/paginated_scope_export_list.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/paginated_work_item_export_list.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/paginated_work_item_export_list.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/paginated_work_item_quantity_export_list.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/paginated_work_item_quantity_export_list.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/paginated_work_order_export_list.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/paginated_work_order_export_list.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/paginated_work_package_export_list.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/paginated_work_package_export_list.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/permission.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/permission.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/production_report_export.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/production_report_export.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/production_report_line_export.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/production_report_line_export.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/production_report_quantity_export.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/production_report_quantity_export.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/profile.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/profile.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/profile_export.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/profile_export.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/refresh_token.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/refresh_token.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/region_export.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/region_export.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/role.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/role.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/scope_export.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/scope_export.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/user_info.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/user_info.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/user_tier_enum.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/user_tier_enum.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/verify_json_web_token.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/verify_json_web_token.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/web_token.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/web_token.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/work_item_export.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/work_item_export.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/work_item_quantity_export.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/work_item_quantity_export.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/work_order_export.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/work_order_export.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/src/vitruvi/types/work_package_export.py` & `vitruvi_sdk-0.0.9/src/vitruvi/types/work_package_export.py`

 * *Files identical despite different names*

### Comparing `vitruvi_sdk-0.0.10/PKG-INFO` & `vitruvi_sdk-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vitruvi-sdk
-Version: 0.0.10
+Version: 0.0.9
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

