# Comparing `tmp/vng-api-common-2.0.4.tar.gz` & `tmp/vng-api-common-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vng-api-common-2.0.4.tar", last modified: Mon Feb 20 08:43:55 2023, max compression
+gzip compressed data, was "vng-api-common-2.0.5.tar", last modified: Tue Jun 20 11:23:25 2023, max compression
```

## Comparing `vng-api-common-2.0.4.tar` & `vng-api-common-2.0.5.tar`

### file list

```diff
@@ -1,322 +1,322 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.927020 vng-api-common-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-02-20 08:43:55.927020 vng-api-common-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.887019 vng-api-common-2.0.4/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1010 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/bin/generate_schema
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/bin/generate_schema.cmd
--rwxr-xr-x   0 runner    (1001) docker     (123)      319 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/bin/patch_content_types
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/bin/patch_content_types.cmd
--rwxr-xr-x   0 runner    (1001) docker     (123)      369 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/bin/use_external_components
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/bin/use_external_components.cmd
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-02-20 08:43:55.931020 vng-api-common-2.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.887019 vng-api-common-2.0.4/testapp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/testapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/testapp/factories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.891020 vng-api-common-2.0.4/testapp/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/testapp/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/testapp/migrations/0002_auto_20190620_0849.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/testapp/migrations/0003_auto_20200416_0423.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/testapp/migrations/0003_person__etag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/testapp/migrations/0004_auto_20190909_0206.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/testapp/migrations/0005_group_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/testapp/migrations/0006_merge_20200416_0440.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/testapp/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/testapp/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/testapp/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/testapp/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/testapp/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/testapp/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/testapp/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/testapp/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/testapp/viewsets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.891020 vng-api-common-2.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/tests/test_autorisatie_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9160 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/tests/test_cache_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/tests/test_check_query_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/tests/test_content_type_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/tests/test_gegevensgroepen.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/tests/test_get_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/tests/test_jwt_decoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/tests/test_jwtsecrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/tests/test_nested_serializer_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/tests/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/tests/test_publish_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/tests/test_schema_root_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/tests/test_server_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/tests/test_validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.895020 vng-api-common-2.0.4/vng_api_common/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.899020 vng-api-common-2.0.4/vng_api_common/api/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/api/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.899020 vng-api-common-2.0.4/vng_api_common/audittrails/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/audittrails/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/audittrails/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.899020 vng-api-common-2.0.4/vng_api_common/audittrails/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/audittrails/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/audittrails/api/scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/audittrails/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/audittrails/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/audittrails/audits.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.903020 vng-api-common-2.0.4/vng_api_common/audittrails/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/audittrails/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/audittrails/migrations/0002_auto_20190516_0830.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/audittrails/migrations/0003_auto_20190517_0844.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/audittrails/migrations/0004_auto_20190520_1238.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/audittrails/migrations/0005_auto_20190520_1450.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/audittrails/migrations/0006_audittrail_toelichting.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/audittrails/migrations/0007_auto_20190522_0916.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/audittrails/migrations/0008_audittrail_resource_weergave.py
--rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/audittrails/migrations/0009_auto_20190712_1643.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/audittrails/migrations/0010_audittrail_request_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/audittrails/migrations/0011_auto_20190918_1335.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/audittrails/migrations/0012_auto_20200619_0545.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/audittrails/migrations/0012_remove_audittrail_request_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/audittrails/migrations/0013_audittrail_logrecord_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/audittrails/migrations/0013_auto_20201207_0846.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/audittrails/migrations/0014_auto_20201221_0905.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/audittrails/migrations/0014_auto_20210323_1654.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/audittrails/migrations/0015_auto_20220318_1608.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/audittrails/migrations/0016_merge_20220607_0517.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/audittrails/migrations/0017_alter_audittrail_bron.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/audittrails/migrations/0018_auto_20220927_1000.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/audittrails/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/audittrails/migrations/_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/audittrails/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/audittrails/viewsets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.903020 vng-api-common-2.0.4/vng_api_common/authorizations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/authorizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/authorizations/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.903020 vng-api-common-2.0.4/vng_api_common/authorizations/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/authorizations/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/authorizations/migrations/0002_authorizationsconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/authorizations/migrations/0003_auto_20190502_0409.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/authorizations/migrations/0004_auto_20190503_0941.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/authorizations/migrations/0005_auto_20190506_0842.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/authorizations/migrations/0006_auto_20190506_0901.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/authorizations/migrations/0007_auto_20190506_1212.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/authorizations/migrations/0008_auto_20190712_1541.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/authorizations/migrations/0009_update_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/authorizations/migrations/0010_auto_20190712_1643.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/authorizations/migrations/0011_auto_20191114_0728.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/authorizations/migrations/0012_auto_20200619_0545.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/authorizations/migrations/0013_auto_20201207_0846.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/authorizations/migrations/0014_auto_20201221_0905.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/authorizations/migrations/0015_auto_20220318_1608.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/authorizations/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/authorizations/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/authorizations/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/authorizations/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.907020 vng-api-common-2.0.4/vng_api_common/caching/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/caching/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/caching/etags.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/caching/introspection.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/caching/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/caching/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/caching/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.907020 vng-api-common-2.0.4/vng_api_common/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/conf/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.907020 vng-api-common-2.0.4/vng_api_common/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/db/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/exception_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.907020 vng-api-common-2.0.4/vng_api_common/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.907020 vng-api-common-2.0.4/vng_api_common/extensions/fields/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/extensions/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/extensions/fields/duration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/extensions/fields/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    10812 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/extensions/fields/geojson.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/extensions/fields/history_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/extensions/fields/hyperlink_identity.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/extensions/fields/hyperlinked_related.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/extensions/fields/many_related.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/extensions/fields/read_only.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.907020 vng-api-common-2.0.4/vng_api_common/extensions/filters/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/extensions/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/extensions/filters/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.907020 vng-api-common-2.0.4/vng_api_common/extensions/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/extensions/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/extensions/serializers/gegevensgroep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/extensions/serializers/polymorphic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/extensions/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/filtersets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/geo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.883020 vng-api-common-2.0.4/vng_api_common/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.883020 vng-api-common-2.0.4/vng_api_common/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.907020 vng-api-common-2.0.4/vng_api_common/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    19495 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.907020 vng-api-common-2.0.4/vng_api_common/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.907020 vng-api-common-2.0.4/vng_api_common/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/management/commands/generate_autorisaties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/management/commands/generate_notificaties.py
--rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/management/commands/generate_swagger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/management/commands/patch_error_contenttypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/management/commands/use_external_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     8839 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.911020 vng-api-common-2.0.4/vng_api_common/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/migrations/0002_apicredential.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/migrations/0003_auto_20190417_1145.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/migrations/0004_auto_20190517_0903.py
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/migrations/0005_auto_20190614_1346.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.911020 vng-api-common-2.0.4/vng_api_common/notifications/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/notifications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.911020 vng-api-common-2.0.4/vng_api_common/notifications/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/notifications/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/notifications/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/notifications/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/notifications/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/notifications/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/notifications/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.911020 vng-api-common-2.0.4/vng_api_common/notifications/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/notifications/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/notifications/migrations/0002_subscription__subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/notifications/migrations/0003_auto_20190319_1048.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/notifications/migrations/0004_auto_20190325_1313.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/notifications/migrations/0005_fix_default_nrc.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/notifications/migrations/0006_auto_20190417_1142.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/notifications/migrations/0007_auto_20190429_1442.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/notifications/migrations/0008_auto_20190502_0415.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/notifications/migrations/0009_auto_20190729_0427.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/notifications/migrations/0010_auto_20220704_1419.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/notifications/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/notifications/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/oas.py
--rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/polymorphism.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/routers.py
--rw-r--r--   0 runner    (1001) docker     (123)    20991 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     9961 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.883020 vng-api-common-2.0.4/vng_api_common/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.883020 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.883020 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/css/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.911020 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/css/admin/
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/css/admin/admin_overrides.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.911020 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/ico/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/ico/favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.911020 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/img/
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/img/vng.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.883020 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.911020 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.915020 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/css/
--rw-r--r--   0 runner    (1001) docker     (123)    64548 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-grid.css
--rw-r--r--   0 runner    (1001) docker     (123)   151749 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-grid.css.map
--rw-r--r--   0 runner    (1001) docker     (123)    48488 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-grid.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   108539 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-grid.min.css.map
--rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-reboot.css
--rw-r--r--   0 runner    (1001) docker     (123)    76483 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-reboot.css.map
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-reboot.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    32461 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-reboot.min.css.map
--rw-r--r--   0 runner    (1001) docker     (123)   192348 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (123)   492048 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap.css.map
--rw-r--r--   0 runner    (1001) docker     (123)   155758 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   625953 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap.min.css.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.919020 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/js/
--rw-r--r--   0 runner    (1001) docker     (123)   222911 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)   402249 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.bundle.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    78635 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   311949 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.bundle.min.js.map
--rw-r--r--   0 runner    (1001) docker     (123)   131637 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (123)   250568 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    58072 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   190253 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.min.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.919020 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/fontawesome/
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/fontawesome/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.923020 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/fontawesome/css/
--rw-r--r--   0 runner    (1001) docker     (123)    69015 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/fontawesome/css/all.css
--rw-r--r--   0 runner    (1001) docker     (123)    55111 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/fontawesome/css/all.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.923020 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/
--rw-r--r--   0 runner    (1001) docker     (123)   129916 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.eot
--rw-r--r--   0 runner    (1001) docker     (123)   694583 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.svg
--rw-r--r--   0 runner    (1001) docker     (123)   129612 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    87688 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)    74768 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    34388 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.eot
--rw-r--r--   0 runner    (1001) docker     (123)   144451 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.svg
--rw-r--r--   0 runner    (1001) docker     (123)    34092 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    16804 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13552 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   186728 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.eot
--rw-r--r--   0 runner    (1001) docker     (123)   816926 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.svg
--rw-r--r--   0 runner    (1001) docker     (123)   186444 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    96256 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.woff
--rw-r--r--   0 runner    (1001) docker     (123)    74256 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.927020 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/jquery/
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/jquery/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   218897 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/jquery/jquery-3.3.1.slim.js
--rw-r--r--   0 runner    (1001) docker     (123)    69917 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/jquery/jquery-3.3.1.slim.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.927020 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/popper/
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/popper/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    87203 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/popper/popper.js
--rw-r--r--   0 runner    (1001) docker     (123)    21004 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/popper/popper.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.887019 vng-api-common-2.0.4/vng_api_common/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.927020 vng-api-common-2.0.4/vng_api_common/templates/vng_api_common/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.927020 vng-api-common-2.0.4/vng_api_common/templates/vng_api_common/admin/
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/templates/vng_api_common/admin/base_site.html
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/templates/vng_api_common/api_schema_to_markdown_table.md
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/templates/vng_api_common/autorisaties.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.927020 vng-api-common-2.0.4/vng_api_common/templates/vng_api_common/includes/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/templates/vng_api_common/includes/kanalen_card.html
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/templates/vng_api_common/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/templates/vng_api_common/master.html
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/templates/vng_api_common/notificaties.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.927020 vng-api-common-2.0.4/vng_api_common/templates/vng_api_common/ref/
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/templates/vng_api_common/ref/error_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/templates/vng_api_common/ref/scopes.html
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/templates/vng_api_common/view_config.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.927020 vng-api-common-2.0.4/vng_api_common/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/templatetags/vng_api_common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.927020 vng-api-common-2.0.4/vng_api_common/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/tests/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/tests/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/tests/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     8584 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12868 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8153 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-02-20 08:43:40.000000 vng-api-common-2.0.4/vng_api_common/viewsets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 08:43:55.899020 vng-api-common-2.0.4/vng_api_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-02-20 08:43:55.000000 vng-api-common-2.0.4/vng_api_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13311 2023-02-20 08:43:55.000000 vng-api-common-2.0.4/vng_api_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 08:43:55.000000 vng-api-common-2.0.4/vng_api_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 08:43:55.000000 vng-api-common-2.0.4/vng_api_common.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-02-20 08:43:55.000000 vng-api-common-2.0.4/vng_api_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-20 08:43:55.000000 vng-api-common-2.0.4/vng_api_common.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.201325 vng-api-common-2.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-06-20 11:23:25.201325 vng-api-common-2.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.161324 vng-api-common-2.0.5/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1010 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/bin/generate_schema
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/bin/generate_schema.cmd
+-rwxr-xr-x   0 runner    (1001) docker     (123)      319 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/bin/patch_content_types
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/bin/patch_content_types.cmd
+-rwxr-xr-x   0 runner    (1001) docker     (123)      369 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/bin/use_external_components
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/bin/use_external_components.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-20 11:23:25.205325 vng-api-common-2.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.165325 vng-api-common-2.0.5/testapp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/testapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/testapp/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.165325 vng-api-common-2.0.5/testapp/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/testapp/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/testapp/migrations/0002_auto_20190620_0849.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/testapp/migrations/0003_auto_20200416_0423.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/testapp/migrations/0003_person__etag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/testapp/migrations/0004_auto_20190909_0206.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/testapp/migrations/0005_group_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/testapp/migrations/0006_merge_20200416_0440.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/testapp/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/testapp/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/testapp/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/testapp/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/testapp/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/testapp/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/testapp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/testapp/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/testapp/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.169324 vng-api-common-2.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/tests/test_autorisatie_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9160 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/tests/test_cache_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/tests/test_check_query_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/tests/test_content_type_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/tests/test_gegevensgroepen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/tests/test_get_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/tests/test_jwt_decoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/tests/test_jwtsecrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/tests/test_nested_serializer_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/tests/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/tests/test_publish_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/tests/test_schema_root_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/tests/test_server_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/tests/test_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.173324 vng-api-common-2.0.5/vng_api_common/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.173324 vng-api-common-2.0.5/vng_api_common/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/api/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.173324 vng-api-common-2.0.5/vng_api_common/audittrails/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/audittrails/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/audittrails/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.173324 vng-api-common-2.0.5/vng_api_common/audittrails/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/audittrails/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/audittrails/api/scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/audittrails/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/audittrails/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/audittrails/audits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.177325 vng-api-common-2.0.5/vng_api_common/audittrails/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/audittrails/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/audittrails/migrations/0002_auto_20190516_0830.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/audittrails/migrations/0003_auto_20190517_0844.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/audittrails/migrations/0004_auto_20190520_1238.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/audittrails/migrations/0005_auto_20190520_1450.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/audittrails/migrations/0006_audittrail_toelichting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/audittrails/migrations/0007_auto_20190522_0916.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/audittrails/migrations/0008_audittrail_resource_weergave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/audittrails/migrations/0009_auto_20190712_1643.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/audittrails/migrations/0010_audittrail_request_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/audittrails/migrations/0011_auto_20190918_1335.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/audittrails/migrations/0012_auto_20200619_0545.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/audittrails/migrations/0012_remove_audittrail_request_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/audittrails/migrations/0013_audittrail_logrecord_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/audittrails/migrations/0013_auto_20201207_0846.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/audittrails/migrations/0014_auto_20201221_0905.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/audittrails/migrations/0014_auto_20210323_1654.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/audittrails/migrations/0015_auto_20220318_1608.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/audittrails/migrations/0016_merge_20220607_0517.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/audittrails/migrations/0017_alter_audittrail_bron.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/audittrails/migrations/0018_auto_20220927_1000.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/audittrails/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/audittrails/migrations/_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/audittrails/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/audittrails/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.177325 vng-api-common-2.0.5/vng_api_common/authorizations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/authorizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/authorizations/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.181325 vng-api-common-2.0.5/vng_api_common/authorizations/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/authorizations/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/authorizations/migrations/0002_authorizationsconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/authorizations/migrations/0003_auto_20190502_0409.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/authorizations/migrations/0004_auto_20190503_0941.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/authorizations/migrations/0005_auto_20190506_0842.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/authorizations/migrations/0006_auto_20190506_0901.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/authorizations/migrations/0007_auto_20190506_1212.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/authorizations/migrations/0008_auto_20190712_1541.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/authorizations/migrations/0009_update_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/authorizations/migrations/0010_auto_20190712_1643.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/authorizations/migrations/0011_auto_20191114_0728.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/authorizations/migrations/0012_auto_20200619_0545.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/authorizations/migrations/0013_auto_20201207_0846.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/authorizations/migrations/0014_auto_20201221_0905.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/authorizations/migrations/0015_auto_20220318_1608.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/authorizations/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/authorizations/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/authorizations/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/authorizations/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.181325 vng-api-common-2.0.5/vng_api_common/caching/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/caching/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/caching/etags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/caching/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/caching/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/caching/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/caching/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.181325 vng-api-common-2.0.5/vng_api_common/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/conf/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.181325 vng-api-common-2.0.5/vng_api_common/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/db/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/exception_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.181325 vng-api-common-2.0.5/vng_api_common/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.181325 vng-api-common-2.0.5/vng_api_common/extensions/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/extensions/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/extensions/fields/duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/extensions/fields/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10812 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/extensions/fields/geojson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/extensions/fields/history_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/extensions/fields/hyperlink_identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/extensions/fields/hyperlinked_related.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/extensions/fields/many_related.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/extensions/fields/read_only.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.181325 vng-api-common-2.0.5/vng_api_common/extensions/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/extensions/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/extensions/filters/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.181325 vng-api-common-2.0.5/vng_api_common/extensions/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/extensions/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/extensions/serializers/gegevensgroep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/extensions/serializers/polymorphic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/extensions/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/filtersets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/geo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.157324 vng-api-common-2.0.5/vng_api_common/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.157324 vng-api-common-2.0.5/vng_api_common/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.185325 vng-api-common-2.0.5/vng_api_common/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    19495 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.185325 vng-api-common-2.0.5/vng_api_common/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.185325 vng-api-common-2.0.5/vng_api_common/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/management/commands/generate_autorisaties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/management/commands/generate_notificaties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/management/commands/generate_swagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/management/commands/patch_error_contenttypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/management/commands/use_external_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8839 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.185325 vng-api-common-2.0.5/vng_api_common/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/migrations/0002_apicredential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/migrations/0003_auto_20190417_1145.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/migrations/0004_auto_20190517_0903.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/migrations/0005_auto_20190614_1346.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.185325 vng-api-common-2.0.5/vng_api_common/notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/notifications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.185325 vng-api-common-2.0.5/vng_api_common/notifications/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/notifications/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/notifications/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/notifications/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/notifications/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/notifications/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/notifications/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.185325 vng-api-common-2.0.5/vng_api_common/notifications/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/notifications/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/notifications/migrations/0002_subscription__subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/notifications/migrations/0003_auto_20190319_1048.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/notifications/migrations/0004_auto_20190325_1313.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/notifications/migrations/0005_fix_default_nrc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/notifications/migrations/0006_auto_20190417_1142.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/notifications/migrations/0007_auto_20190429_1442.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/notifications/migrations/0008_auto_20190502_0415.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/notifications/migrations/0009_auto_20190729_0427.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/notifications/migrations/0010_auto_20220704_1419.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/notifications/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/notifications/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/oas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/polymorphism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/routers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20991 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9961 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.161324 vng-api-common-2.0.5/vng_api_common/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.161324 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.161324 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/css/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.189325 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/css/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/css/admin/admin_overrides.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.189325 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/ico/
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/ico/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.189325 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/img/
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/img/vng.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.161324 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.189325 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.189325 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    64548 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-grid.css
+-rw-r--r--   0 runner    (1001) docker     (123)   151749 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-grid.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)    48488 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-grid.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   108539 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-grid.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-reboot.css
+-rw-r--r--   0 runner    (1001) docker     (123)    76483 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-reboot.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-reboot.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    32461 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)   192348 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (123)   492048 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)   155758 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   625953 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap.min.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.193325 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   222911 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)   402249 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.bundle.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    78635 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   311949 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)   131637 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (123)   250568 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    58072 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   190253 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.min.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.193325 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/fontawesome/
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/fontawesome/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.193325 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/fontawesome/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    69015 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/fontawesome/css/all.css
+-rw-r--r--   0 runner    (1001) docker     (123)    55111 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/fontawesome/css/all.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.197325 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   129916 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   694583 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   129612 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    87688 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    74768 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    34388 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   144451 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    34092 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    16804 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13552 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   186728 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   816926 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   186444 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    96256 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    74256 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.201325 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/jquery/
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/jquery/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   218897 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/jquery/jquery-3.3.1.slim.js
+-rw-r--r--   0 runner    (1001) docker     (123)    69917 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/jquery/jquery-3.3.1.slim.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.201325 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/popper/
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/popper/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    87203 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/popper/popper.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21004 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/popper/popper.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.161324 vng-api-common-2.0.5/vng_api_common/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.201325 vng-api-common-2.0.5/vng_api_common/templates/vng_api_common/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.201325 vng-api-common-2.0.5/vng_api_common/templates/vng_api_common/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/templates/vng_api_common/admin/base_site.html
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/templates/vng_api_common/api_schema_to_markdown_table.md
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/templates/vng_api_common/autorisaties.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.201325 vng-api-common-2.0.5/vng_api_common/templates/vng_api_common/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/templates/vng_api_common/includes/kanalen_card.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/templates/vng_api_common/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/templates/vng_api_common/master.html
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/templates/vng_api_common/notificaties.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.201325 vng-api-common-2.0.5/vng_api_common/templates/vng_api_common/ref/
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/templates/vng_api_common/ref/error_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/templates/vng_api_common/ref/scopes.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/templates/vng_api_common/view_config.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.201325 vng-api-common-2.0.5/vng_api_common/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/templatetags/vng_api_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.201325 vng-api-common-2.0.5/vng_api_common/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/tests/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/tests/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/tests/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8584 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12868 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8153 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-20 11:23:20.000000 vng-api-common-2.0.5/vng_api_common/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 11:23:25.173324 vng-api-common-2.0.5/vng_api_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-06-20 11:23:25.000000 vng-api-common-2.0.5/vng_api_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13311 2023-06-20 11:23:25.000000 vng-api-common-2.0.5/vng_api_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 11:23:25.000000 vng-api-common-2.0.5/vng_api_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 11:23:25.000000 vng-api-common-2.0.5/vng_api_common.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-20 11:23:25.000000 vng-api-common-2.0.5/vng_api_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-20 11:23:25.000000 vng-api-common-2.0.5/vng_api_common.egg-info/top_level.txt
```

### Comparing `vng-api-common-2.0.4/PKG-INFO` & `vng-api-common-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vng-api-common
-Version: 2.0.4
+Version: 2.0.5
 Summary: VNG API tooling
 Home-page: https://github.com/VNG-Realisatie/vng-api-common
 Author: Maykin Media, VNG-Realisatie
 Author-email: support@maykinmedia.nl
 License: EUPL 1.2
 Keywords: openapi,swagger,django,vng
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `vng-api-common-2.0.4/README.rst` & `vng-api-common-2.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/bin/generate_schema` & `vng-api-common-2.0.5/bin/generate_schema`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/bin/generate_schema.cmd` & `vng-api-common-2.0.5/bin/generate_schema.cmd`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/setup.cfg` & `vng-api-common-2.0.5/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vng-api-common
-version = 2.0.4
+version = 2.0.5
 description = VNG API tooling
 long_description = file: README.rst
 url = https://github.com/VNG-Realisatie/vng-api-common
 license = EUPL 1.2
 author = Maykin Media, VNG-Realisatie
 author_email = support@maykinmedia.nl
 keywords = openapi, swagger, django, vng
```

### Comparing `vng-api-common-2.0.4/testapp/factories.py` & `vng-api-common-2.0.5/testapp/factories.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/testapp/migrations/0001_initial.py` & `vng-api-common-2.0.5/testapp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/testapp/migrations/0002_auto_20190620_0849.py` & `vng-api-common-2.0.5/testapp/migrations/0002_auto_20190620_0849.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/testapp/migrations/0003_auto_20200416_0423.py` & `vng-api-common-2.0.5/testapp/migrations/0003_auto_20200416_0423.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/testapp/migrations/0003_person__etag.py` & `vng-api-common-2.0.5/testapp/migrations/0003_person__etag.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/testapp/migrations/0004_auto_20190909_0206.py` & `vng-api-common-2.0.5/testapp/migrations/0004_auto_20190909_0206.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/testapp/models.py` & `vng-api-common-2.0.5/testapp/models.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/testapp/serializers.py` & `vng-api-common-2.0.5/testapp/serializers.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/testapp/settings.py` & `vng-api-common-2.0.5/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/testapp/urls.py` & `vng-api-common-2.0.5/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/testapp/viewsets.py` & `vng-api-common-2.0.5/testapp/viewsets.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/tests/test_autorisatie_validation.py` & `vng-api-common-2.0.5/tests/test_autorisatie_validation.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/tests/test_cache_headers.py` & `vng-api-common-2.0.5/tests/test_cache_headers.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/tests/test_check_query_params.py` & `vng-api-common-2.0.5/tests/test_check_query_params.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/tests/test_content_type_headers.py` & `vng-api-common-2.0.5/tests/test_content_type_headers.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/tests/test_filters.py` & `vng-api-common-2.0.5/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/tests/test_gegevensgroepen.py` & `vng-api-common-2.0.5/tests/test_gegevensgroepen.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/tests/test_jwt_decoding.py` & `vng-api-common-2.0.5/tests/test_jwt_decoding.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/tests/test_jwtsecrets.py` & `vng-api-common-2.0.5/tests/test_jwtsecrets.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/tests/test_nested_serializer_validation.py` & `vng-api-common-2.0.5/tests/test_nested_serializer_validation.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/tests/test_permissions.py` & `vng-api-common-2.0.5/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/tests/test_publish_validator.py` & `vng-api-common-2.0.5/tests/test_publish_validator.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/tests/test_schema_root_tags.py` & `vng-api-common-2.0.5/tests/test_schema_root_tags.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/tests/test_server_errors.py` & `vng-api-common-2.0.5/tests/test_server_errors.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/tests/test_utils.py` & `vng-api-common-2.0.5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/tests/test_validators.py` & `vng-api-common-2.0.5/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/admin.py` & `vng-api-common-2.0.5/vng_api_common/admin.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/api/permissions.py` & `vng-api-common-2.0.5/vng_api_common/api/permissions.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/apps.py` & `vng-api-common-2.0.5/vng_api_common/apps.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/audittrails/api/serializers.py` & `vng-api-common-2.0.5/vng_api_common/audittrails/api/serializers.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/audittrails/migrations/0001_initial.py` & `vng-api-common-2.0.5/vng_api_common/audittrails/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/audittrails/migrations/0002_auto_20190516_0830.py` & `vng-api-common-2.0.5/vng_api_common/audittrails/migrations/0002_auto_20190516_0830.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/audittrails/migrations/0003_auto_20190517_0844.py` & `vng-api-common-2.0.5/vng_api_common/audittrails/migrations/0003_auto_20190517_0844.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/audittrails/migrations/0004_auto_20190520_1238.py` & `vng-api-common-2.0.5/vng_api_common/audittrails/migrations/0004_auto_20190520_1238.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/audittrails/migrations/0005_auto_20190520_1450.py` & `vng-api-common-2.0.5/vng_api_common/audittrails/migrations/0005_auto_20190520_1450.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/audittrails/migrations/0006_audittrail_toelichting.py` & `vng-api-common-2.0.5/vng_api_common/audittrails/migrations/0006_audittrail_toelichting.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/audittrails/migrations/0007_auto_20190522_0916.py` & `vng-api-common-2.0.5/vng_api_common/audittrails/migrations/0007_auto_20190522_0916.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/audittrails/migrations/0008_audittrail_resource_weergave.py` & `vng-api-common-2.0.5/vng_api_common/audittrails/migrations/0008_audittrail_resource_weergave.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/audittrails/migrations/0009_auto_20190712_1643.py` & `vng-api-common-2.0.5/vng_api_common/audittrails/migrations/0009_auto_20190712_1643.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/audittrails/migrations/0010_audittrail_request_id.py` & `vng-api-common-2.0.5/vng_api_common/audittrails/migrations/0010_audittrail_request_id.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/audittrails/migrations/0011_auto_20190918_1335.py` & `vng-api-common-2.0.5/vng_api_common/audittrails/migrations/0011_auto_20190918_1335.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/audittrails/migrations/0012_auto_20200619_0545.py` & `vng-api-common-2.0.5/vng_api_common/audittrails/migrations/0012_auto_20200619_0545.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/audittrails/migrations/0013_audittrail_logrecord_id.py` & `vng-api-common-2.0.5/vng_api_common/audittrails/migrations/0013_audittrail_logrecord_id.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/audittrails/migrations/0013_auto_20201207_0846.py` & `vng-api-common-2.0.5/vng_api_common/audittrails/migrations/0013_auto_20201207_0846.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/audittrails/migrations/0014_auto_20201221_0905.py` & `vng-api-common-2.0.5/vng_api_common/audittrails/migrations/0014_auto_20201221_0905.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/audittrails/migrations/0014_auto_20210323_1654.py` & `vng-api-common-2.0.5/vng_api_common/audittrails/migrations/0014_auto_20210323_1654.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/audittrails/migrations/0015_auto_20220318_1608.py` & `vng-api-common-2.0.5/vng_api_common/audittrails/migrations/0015_auto_20220318_1608.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/audittrails/migrations/0017_alter_audittrail_bron.py` & `vng-api-common-2.0.5/vng_api_common/audittrails/migrations/0017_alter_audittrail_bron.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/audittrails/migrations/0018_auto_20220927_1000.py` & `vng-api-common-2.0.5/vng_api_common/audittrails/migrations/0018_auto_20220927_1000.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/audittrails/migrations/_operations.py` & `vng-api-common-2.0.5/vng_api_common/audittrails/migrations/_operations.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/audittrails/models.py` & `vng-api-common-2.0.5/vng_api_common/audittrails/models.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/audittrails/viewsets.py` & `vng-api-common-2.0.5/vng_api_common/audittrails/viewsets.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/authorizations/admin.py` & `vng-api-common-2.0.5/vng_api_common/authorizations/admin.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/authorizations/migrations/0001_initial.py` & `vng-api-common-2.0.5/vng_api_common/authorizations/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/authorizations/migrations/0002_authorizationsconfig.py` & `vng-api-common-2.0.5/vng_api_common/authorizations/migrations/0002_authorizationsconfig.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/authorizations/migrations/0003_auto_20190502_0409.py` & `vng-api-common-2.0.5/vng_api_common/authorizations/migrations/0003_auto_20190502_0409.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/authorizations/migrations/0004_auto_20190503_0941.py` & `vng-api-common-2.0.5/vng_api_common/authorizations/migrations/0004_auto_20190503_0941.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/authorizations/migrations/0005_auto_20190506_0842.py` & `vng-api-common-2.0.5/vng_api_common/authorizations/migrations/0005_auto_20190506_0842.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/authorizations/migrations/0006_auto_20190506_0901.py` & `vng-api-common-2.0.5/vng_api_common/authorizations/migrations/0006_auto_20190506_0901.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/authorizations/migrations/0007_auto_20190506_1212.py` & `vng-api-common-2.0.5/vng_api_common/authorizations/migrations/0007_auto_20190506_1212.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/authorizations/migrations/0008_auto_20190712_1541.py` & `vng-api-common-2.0.5/vng_api_common/authorizations/migrations/0008_auto_20190712_1541.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/authorizations/migrations/0009_update_enums.py` & `vng-api-common-2.0.5/vng_api_common/authorizations/migrations/0009_update_enums.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/authorizations/migrations/0010_auto_20190712_1643.py` & `vng-api-common-2.0.5/vng_api_common/authorizations/migrations/0010_auto_20190712_1643.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/authorizations/migrations/0011_auto_20191114_0728.py` & `vng-api-common-2.0.5/vng_api_common/authorizations/migrations/0011_auto_20191114_0728.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/authorizations/migrations/0012_auto_20200619_0545.py` & `vng-api-common-2.0.5/vng_api_common/authorizations/migrations/0012_auto_20200619_0545.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/authorizations/migrations/0013_auto_20201207_0846.py` & `vng-api-common-2.0.5/vng_api_common/authorizations/migrations/0013_auto_20201207_0846.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/authorizations/migrations/0014_auto_20201221_0905.py` & `vng-api-common-2.0.5/vng_api_common/authorizations/migrations/0014_auto_20201221_0905.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/authorizations/migrations/0015_auto_20220318_1608.py` & `vng-api-common-2.0.5/vng_api_common/authorizations/migrations/0015_auto_20220318_1608.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/authorizations/models.py` & `vng-api-common-2.0.5/vng_api_common/authorizations/models.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/authorizations/serializers.py` & `vng-api-common-2.0.5/vng_api_common/authorizations/serializers.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/authorizations/validators.py` & `vng-api-common-2.0.5/vng_api_common/authorizations/validators.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/caching/__init__.py` & `vng-api-common-2.0.5/vng_api_common/caching/__init__.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/caching/decorators.py` & `vng-api-common-2.0.5/vng_api_common/caching/decorators.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/caching/etags.py` & `vng-api-common-2.0.5/vng_api_common/caching/etags.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/caching/introspection.py` & `vng-api-common-2.0.5/vng_api_common/caching/introspection.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/caching/models.py` & `vng-api-common-2.0.5/vng_api_common/caching/models.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/caching/registry.py` & `vng-api-common-2.0.5/vng_api_common/caching/registry.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/caching/signals.py` & `vng-api-common-2.0.5/vng_api_common/caching/signals.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/checks.py` & `vng-api-common-2.0.5/vng_api_common/checks.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/client.py` & `vng-api-common-2.0.5/vng_api_common/client.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/compat.py` & `vng-api-common-2.0.5/vng_api_common/compat.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/conf/api.py` & `vng-api-common-2.0.5/vng_api_common/conf/api.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/constants.py` & `vng-api-common-2.0.5/vng_api_common/constants.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/db/operations.py` & `vng-api-common-2.0.5/vng_api_common/db/operations.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/descriptors.py` & `vng-api-common-2.0.5/vng_api_common/descriptors.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/doc.py` & `vng-api-common-2.0.5/vng_api_common/doc.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/exception_handling.py` & `vng-api-common-2.0.5/vng_api_common/exception_handling.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/exceptions.py` & `vng-api-common-2.0.5/vng_api_common/exceptions.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/extensions/fields/duration.py` & `vng-api-common-2.0.5/vng_api_common/extensions/fields/duration.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/extensions/fields/files.py` & `vng-api-common-2.0.5/vng_api_common/extensions/fields/files.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/extensions/fields/geojson.py` & `vng-api-common-2.0.5/vng_api_common/extensions/fields/geojson.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/extensions/fields/history_url.py` & `vng-api-common-2.0.5/vng_api_common/extensions/fields/history_url.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/extensions/fields/hyperlink_identity.py` & `vng-api-common-2.0.5/vng_api_common/extensions/fields/hyperlink_identity.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/extensions/fields/hyperlinked_related.py` & `vng-api-common-2.0.5/vng_api_common/extensions/fields/hyperlinked_related.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/extensions/fields/read_only.py` & `vng-api-common-2.0.5/vng_api_common/extensions/fields/read_only.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/extensions/filters/query.py` & `vng-api-common-2.0.5/vng_api_common/extensions/filters/query.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/extensions/serializers/gegevensgroep.py` & `vng-api-common-2.0.5/vng_api_common/extensions/serializers/gegevensgroep.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/extensions/serializers/polymorphic.py` & `vng-api-common-2.0.5/vng_api_common/extensions/serializers/polymorphic.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/extensions/utils.py` & `vng-api-common-2.0.5/vng_api_common/extensions/utils.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/fields.py` & `vng-api-common-2.0.5/vng_api_common/fields.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/filters.py` & `vng-api-common-2.0.5/vng_api_common/filters.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/filtersets.py` & `vng-api-common-2.0.5/vng_api_common/filtersets.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/generators.py` & `vng-api-common-2.0.5/vng_api_common/generators.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/geo.py` & `vng-api-common-2.0.5/vng_api_common/geo.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/locale/nl/LC_MESSAGES/django.mo` & `vng-api-common-2.0.5/vng_api_common/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/locale/nl/LC_MESSAGES/django.po` & `vng-api-common-2.0.5/vng_api_common/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/management/commands/generate_autorisaties.py` & `vng-api-common-2.0.5/vng_api_common/management/commands/generate_autorisaties.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/management/commands/generate_notificaties.py` & `vng-api-common-2.0.5/vng_api_common/management/commands/generate_notificaties.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/management/commands/generate_swagger.py` & `vng-api-common-2.0.5/vng_api_common/management/commands/generate_swagger.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/management/commands/patch_error_contenttypes.py` & `vng-api-common-2.0.5/vng_api_common/management/commands/patch_error_contenttypes.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/management/commands/use_external_components.py` & `vng-api-common-2.0.5/vng_api_common/management/commands/use_external_components.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/middleware.py` & `vng-api-common-2.0.5/vng_api_common/middleware.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/migrations/0001_initial.py` & `vng-api-common-2.0.5/vng_api_common/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/migrations/0002_apicredential.py` & `vng-api-common-2.0.5/vng_api_common/migrations/0002_apicredential.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/migrations/0003_auto_20190417_1145.py` & `vng-api-common-2.0.5/vng_api_common/migrations/0003_auto_20190417_1145.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/migrations/0004_auto_20190517_0903.py` & `vng-api-common-2.0.5/vng_api_common/migrations/0004_auto_20190517_0903.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/migrations/0005_auto_20190614_1346.py` & `vng-api-common-2.0.5/vng_api_common/migrations/0005_auto_20190614_1346.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/mocks.py` & `vng-api-common-2.0.5/vng_api_common/mocks.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/models.py` & `vng-api-common-2.0.5/vng_api_common/models.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/notifications/api/views.py` & `vng-api-common-2.0.5/vng_api_common/notifications/api/views.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/notifications/handlers.py` & `vng-api-common-2.0.5/vng_api_common/notifications/handlers.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/notifications/migrations/0001_initial.py` & `vng-api-common-2.0.5/vng_api_common/notifications/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/notifications/migrations/0002_subscription__subscription.py` & `vng-api-common-2.0.5/vng_api_common/notifications/migrations/0002_subscription__subscription.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/notifications/migrations/0003_auto_20190319_1048.py` & `vng-api-common-2.0.5/vng_api_common/notifications/migrations/0003_auto_20190319_1048.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/notifications/migrations/0004_auto_20190325_1313.py` & `vng-api-common-2.0.5/vng_api_common/notifications/migrations/0004_auto_20190325_1313.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/notifications/migrations/0005_fix_default_nrc.py` & `vng-api-common-2.0.5/vng_api_common/notifications/migrations/0005_fix_default_nrc.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/notifications/migrations/0006_auto_20190417_1142.py` & `vng-api-common-2.0.5/vng_api_common/notifications/migrations/0006_auto_20190417_1142.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/notifications/migrations/0008_auto_20190502_0415.py` & `vng-api-common-2.0.5/vng_api_common/notifications/migrations/0008_auto_20190502_0415.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/notifications/migrations/0009_auto_20190729_0427.py` & `vng-api-common-2.0.5/vng_api_common/notifications/migrations/0009_auto_20190729_0427.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/notifications/migrations/0010_auto_20220704_1419.py` & `vng-api-common-2.0.5/vng_api_common/notifications/migrations/0010_auto_20220704_1419.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/notifications/models.py` & `vng-api-common-2.0.5/vng_api_common/notifications/models.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/oas.py` & `vng-api-common-2.0.5/vng_api_common/oas.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/permissions.py` & `vng-api-common-2.0.5/vng_api_common/permissions.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/polymorphism.py` & `vng-api-common-2.0.5/vng_api_common/polymorphism.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/routers.py` & `vng-api-common-2.0.5/vng_api_common/routers.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/schema.py` & `vng-api-common-2.0.5/vng_api_common/schema.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/scopes.py` & `vng-api-common-2.0.5/vng_api_common/scopes.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/search.py` & `vng-api-common-2.0.5/vng_api_common/search.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/serializers.py` & `vng-api-common-2.0.5/vng_api_common/serializers.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/css/admin/admin_overrides.css` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/css/admin/admin_overrides.css`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/img/vng.svg` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/img/vng.svg`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/LICENSE.txt` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-grid.css` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-grid.css.map` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-grid.min.css` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-grid.min.css.map` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-reboot.css` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-reboot.css.map` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-reboot.min.css` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-reboot.min.css.map` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap.css` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap.css.map` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap.min.css` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap.min.css.map` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.bundle.js` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.bundle.js.map` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.bundle.min.js` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.bundle.min.js.map` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.js` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.js.map` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.min.js` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.min.js.map` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/bootstrap/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/fontawesome/LICENSE.txt` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/fontawesome/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/fontawesome/css/all.css` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/fontawesome/css/all.css`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/fontawesome/css/all.min.css` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/fontawesome/css/all.min.css`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.eot` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.svg` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.ttf` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.woff` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.woff2` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.eot` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.svg` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.ttf` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.woff` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.woff2` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.eot` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.svg` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.ttf` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.woff` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.woff2` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/fontawesome/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/jquery/LICENSE.txt` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/jquery/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/jquery/jquery-3.3.1.slim.js` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/jquery/jquery-3.3.1.slim.js`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/jquery/jquery-3.3.1.slim.min.js` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/jquery/jquery-3.3.1.slim.min.js`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/popper/LICENSE.md` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/popper/LICENSE.md`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/popper/popper.js` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/popper/popper.js`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/static/vng_api_common/libs/popper/popper.min.js` & `vng-api-common-2.0.5/vng_api_common/static/vng_api_common/libs/popper/popper.min.js`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/templates/vng_api_common/admin/base_site.html` & `vng-api-common-2.0.5/vng_api_common/templates/vng_api_common/admin/base_site.html`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/templates/vng_api_common/api_schema_to_markdown_table.md` & `vng-api-common-2.0.5/vng_api_common/templates/vng_api_common/api_schema_to_markdown_table.md`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/templates/vng_api_common/index.html` & `vng-api-common-2.0.5/vng_api_common/templates/vng_api_common/index.html`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/templates/vng_api_common/master.html` & `vng-api-common-2.0.5/vng_api_common/templates/vng_api_common/master.html`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/templates/vng_api_common/notificaties.md` & `vng-api-common-2.0.5/vng_api_common/templates/vng_api_common/notificaties.md`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/templates/vng_api_common/ref/error_detail.html` & `vng-api-common-2.0.5/vng_api_common/templates/vng_api_common/ref/error_detail.html`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/templates/vng_api_common/ref/scopes.html` & `vng-api-common-2.0.5/vng_api_common/templates/vng_api_common/ref/scopes.html`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/templates/vng_api_common/view_config.html` & `vng-api-common-2.0.5/vng_api_common/templates/vng_api_common/view_config.html`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/templatetags/vng_api_common.py` & `vng-api-common-2.0.5/vng_api_common/templatetags/vng_api_common.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/tests/auth.py` & `vng-api-common-2.0.5/vng_api_common/tests/auth.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/tests/caching.py` & `vng-api-common-2.0.5/vng_api_common/tests/caching.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/tests/schema.py` & `vng-api-common-2.0.5/vng_api_common/tests/schema.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/tests/urls.py` & `vng-api-common-2.0.5/vng_api_common/tests/urls.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/utils.py` & `vng-api-common-2.0.5/vng_api_common/utils.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/validators.py` & `vng-api-common-2.0.5/vng_api_common/validators.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/views.py` & `vng-api-common-2.0.5/vng_api_common/views.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common/viewsets.py` & `vng-api-common-2.0.5/vng_api_common/viewsets.py`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common.egg-info/PKG-INFO` & `vng-api-common-2.0.5/vng_api_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vng-api-common
-Version: 2.0.4
+Version: 2.0.5
 Summary: VNG API tooling
 Home-page: https://github.com/VNG-Realisatie/vng-api-common
 Author: Maykin Media, VNG-Realisatie
 Author-email: support@maykinmedia.nl
 License: EUPL 1.2
 Keywords: openapi,swagger,django,vng
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `vng-api-common-2.0.4/vng_api_common.egg-info/SOURCES.txt` & `vng-api-common-2.0.5/vng_api_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vng-api-common-2.0.4/vng_api_common.egg-info/requires.txt` & `vng-api-common-2.0.5/vng_api_common.egg-info/requires.txt`

 * *Files identical despite different names*

