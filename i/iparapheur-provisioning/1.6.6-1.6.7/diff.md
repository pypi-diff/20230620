# Comparing `tmp/iparapheur-provisioning-1.6.6.tar.gz` & `tmp/iparapheur-provisioning-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iparapheur-provisioning-1.6.6.tar", last modified: Sat Jun 10 12:31:44 2023, max compression
+gzip compressed data, was "iparapheur-provisioning-1.6.7.tar", last modified: Tue Jun 20 11:20:46 2023, max compression
```

## Comparing `iparapheur-provisioning-1.6.6.tar` & `iparapheur-provisioning-1.6.7.tar`

### file list

```diff
@@ -1,241 +1,241 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:44.257931 iparapheur-provisioning-1.6.6/
--rw-r--r--   0 root         (0) root         (0)     1111 2023-06-10 12:25:37.000000 iparapheur-provisioning-1.6.6/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      421 2023-06-10 12:31:44.257931 iparapheur-provisioning-1.6.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    17323 2023-06-10 12:25:37.000000 iparapheur-provisioning-1.6.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:43.641916 iparapheur-provisioning-1.6.6/iparapheur_provisioning/
--rw-r--r--   0 root         (0) root         (0)      907 2023-06-10 12:25:37.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58620 2023-06-10 12:25:37.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:43.649917 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/
--rw-r--r--   0 root         (0) root         (0)      214 2023-06-10 12:25:37.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4776 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/path_to_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:43.677917 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/paths/
--rw-r--r--   0 root         (0) root         (0)      250 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/paths/__init__.py
--rw-r--r--   0 root         (0) root         (0)      157 2023-06-10 12:25:12.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-06-10 12:25:12.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id.py
--rw-r--r--   0 root         (0) root         (0)      303 2023-06-10 12:25:09.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_desk.py
--rw-r--r--   0 root         (0) root         (0)      458 2023-06-10 12:25:09.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id.py
--rw-r--r--   0 root         (0) root         (0)      329 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type.py
--rw-r--r--   0 root         (0) root         (0)      493 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id.py
--rw-r--r--   0 root         (0) root         (0)      374 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype.py
--rw-r--r--   0 root         (0) root         (0)      566 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id.py
--rw-r--r--   0 root         (0) root         (0)      303 2023-06-10 12:25:14.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_user.py
--rw-r--r--   0 root         (0) root         (0)      458 2023-06-10 12:25:14.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id.py
--rw-r--r--   0 root         (0) root         (0)      150 2023-06-10 12:25:06.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_user.py
--rw-r--r--   0 root         (0) root         (0)      393 2023-06-10 12:25:06.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_user_user_id.py
--rw-r--r--   0 root         (0) root         (0)     1089 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/tag_to_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:43.681917 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/tags/
--rw-r--r--   0 root         (0) root         (0)      475 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/tags/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1031 2023-06-10 12:25:06.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/tags/admin_all_users_api.py
--rw-r--r--   0 root         (0) root         (0)     1131 2023-06-10 12:25:09.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/tags/admin_desk_api.py
--rw-r--r--   0 root         (0) root         (0)      966 2023-06-10 12:25:12.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/tags/admin_tenant_api.py
--rw-r--r--   0 root         (0) root         (0)     1139 2023-06-10 12:25:14.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/tags/admin_tenant_user_api.py
--rw-r--r--   0 root         (0) root         (0)     1959 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/tags/admin_typology_api.py
--rw-r--r--   0 root         (0) root         (0)    15677 2023-06-10 12:25:37.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/configuration.py
--rw-r--r--   0 root         (0) root         (0)     4598 2023-06-10 12:25:37.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:43.881922 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/
--rw-r--r--   0 root         (0) root         (0)      357 2023-06-10 12:25:37.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1426 2023-06-10 12:24:51.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/delegation_sort_by.py
--rw-r--r--   0 root         (0) root         (0)    24041 2023-06-10 12:24:53.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/desk_dto.py
--rw-r--r--   0 root         (0) root         (0)     3809 2023-06-10 12:24:55.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/desk_representation.py
--rw-r--r--   0 root         (0) root         (0)     4553 2023-06-10 12:24:55.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/error_response.py
--rw-r--r--   0 root         (0) root         (0)     4891 2023-06-10 12:24:56.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/external_signature_config_representation.py
--rw-r--r--   0 root         (0) root         (0)     1399 2023-06-10 12:24:56.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/external_signature_config_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1313 2023-06-10 12:24:56.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/external_signature_provider.py
--rw-r--r--   0 root         (0) root         (0)     2680 2023-06-10 12:24:56.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/folder_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     2656 2023-06-10 12:24:56.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/internal_metadata.py
--rw-r--r--   0 root         (0) root         (0)     3284 2023-06-10 12:24:56.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/layer_representation.py
--rw-r--r--   0 root         (0) root         (0)     1141 2023-06-10 12:24:56.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/layer_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     7233 2023-06-10 12:24:56.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/metadata_dto.py
--rw-r--r--   0 root         (0) root         (0)     5805 2023-06-10 12:24:56.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/metadata_representation.py
--rw-r--r--   0 root         (0) root         (0)     1356 2023-06-10 12:24:56.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/metadata_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1598 2023-06-10 12:24:57.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/metadata_type.py
--rw-r--r--   0 root         (0) root         (0)     9105 2023-06-10 12:24:57.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/page_desk_representation.py
--rw-r--r--   0 root         (0) root         (0)     9132 2023-06-10 12:24:57.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/page_subtype_representation.py
--rw-r--r--   0 root         (0) root         (0)     9105 2023-06-10 12:24:57.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/page_type_representation.py
--rw-r--r--   0 root         (0) root         (0)     9105 2023-06-10 12:24:57.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/page_user_representation.py
--rw-r--r--   0 root         (0) root         (0)     5251 2023-06-10 12:24:58.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/pageable_object.py
--rw-r--r--   0 root         (0) root         (0)     3524 2023-06-10 12:24:58.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/pdf_signature_position.py
--rw-r--r--   0 root         (0) root         (0)     1301 2023-06-10 12:24:58.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/seal_certificate_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1527 2023-06-10 12:24:58.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/signature_format.py
--rw-r--r--   0 root         (0) root         (0)     1273 2023-06-10 12:24:58.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/signature_protocol.py
--rw-r--r--   0 root         (0) root         (0)     3524 2023-06-10 12:24:58.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/sort_object.py
--rw-r--r--   0 root         (0) root         (0)    28616 2023-06-10 12:24:59.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/subtype_dto.py
--rw-r--r--   0 root         (0) root         (0)     1307 2023-06-10 12:24:59.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/subtype_layer_association.py
--rw-r--r--   0 root         (0) root         (0)     3930 2023-06-10 12:24:59.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/subtype_layer_dto.py
--rw-r--r--   0 root         (0) root         (0)     5468 2023-06-10 12:25:00.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/subtype_metadata_dto.py
--rw-r--r--   0 root         (0) root         (0)     3288 2023-06-10 12:25:00.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/subtype_representation.py
--rw-r--r--   0 root         (0) root         (0)     3274 2023-06-10 12:25:00.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/tenant_dto.py
--rw-r--r--   0 root         (0) root         (0)     3286 2023-06-10 12:25:00.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/tenant_representation.py
--rw-r--r--   0 root         (0) root         (0)     1142 2023-06-10 12:25:00.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/tenant_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     9365 2023-06-10 12:25:00.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/type_dto.py
--rw-r--r--   0 root         (0) root         (0)     4044 2023-06-10 12:25:01.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/type_representation.py
--rw-r--r--   0 root         (0) root         (0)     1144 2023-06-10 12:25:01.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/typology_sort_by.py
--rw-r--r--   0 root         (0) root         (0)    29666 2023-06-10 12:25:01.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/user_dto.py
--rw-r--r--   0 root         (0) root         (0)     1471 2023-06-10 12:25:02.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/user_privilege.py
--rw-r--r--   0 root         (0) root         (0)     6504 2023-06-10 12:25:02.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/user_representation.py
--rw-r--r--   0 root         (0) root         (0)     1522 2023-06-10 12:25:05.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/user_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1256 2023-06-10 12:25:05.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/workflow_definition_sort_by.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:43.893922 iparapheur-provisioning-1.6.6/iparapheur_provisioning/models/
--rw-r--r--   0 root         (0) root         (0)     3645 2023-06-10 12:25:37.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:43.901923 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/
--rw-r--r--   0 root         (0) root         (0)     1689 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:43.905923 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/
--rw-r--r--   0 root         (0) root         (0)      369 2023-06-10 12:25:11.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13629 2023-06-10 12:25:09.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:43.909923 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/
--rw-r--r--   0 root         (0) root         (0)      389 2023-06-10 12:25:11.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11083 2023-06-10 12:25:10.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11332 2023-06-10 12:25:10.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/get.py
--rw-r--r--   0 root         (0) root         (0)    15808 2023-06-10 12:25:10.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:43.909923 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/
--rw-r--r--   0 root         (0) root         (0)      399 2023-06-10 12:25:08.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15034 2023-06-10 12:25:08.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/get.py
--rw-r--r--   0 root         (0) root         (0)    16302 2023-06-10 12:25:07.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:43.917923 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/
--rw-r--r--   0 root         (0) root         (0)      415 2023-06-10 12:25:08.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11337 2023-06-10 12:25:07.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11677 2023-06-10 12:25:08.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/get.py
--rw-r--r--   0 root         (0) root         (0)    16545 2023-06-10 12:25:07.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:43.917923 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/
--rw-r--r--   0 root         (0) root         (0)      417 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14728 2023-06-10 12:25:34.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/get.py
--rw-r--r--   0 root         (0) root         (0)    15777 2023-06-10 12:25:15.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:43.933923 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/
--rw-r--r--   0 root         (0) root         (0)      433 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11337 2023-06-10 12:25:28.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11590 2023-06-10 12:25:33.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/get.py
--rw-r--r--   0 root         (0) root         (0)    15521 2023-06-10 12:25:35.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:43.949924 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/
--rw-r--r--   0 root         (0) root         (0)      449 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15050 2023-06-10 12:25:34.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/get.py
--rw-r--r--   0 root         (0) root         (0)    16640 2023-06-10 12:25:15.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:43.953924 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/
--rw-r--r--   0 root         (0) root         (0)      471 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11672 2023-06-10 12:25:21.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11934 2023-06-10 12:25:32.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/get.py
--rw-r--r--   0 root         (0) root         (0)    16645 2023-06-10 12:25:35.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:43.977924 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/
--rw-r--r--   0 root         (0) root         (0)      399 2023-06-10 12:25:14.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15944 2023-06-10 12:25:13.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/get.py
--rw-r--r--   0 root         (0) root         (0)    15781 2023-06-10 12:25:12.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:43.997925 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/
--rw-r--r--   0 root         (0) root         (0)      415 2023-06-10 12:25:14.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11407 2023-06-10 12:25:13.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11580 2023-06-10 12:25:12.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/get.py
--rw-r--r--   0 root         (0) root         (0)    16046 2023-06-10 12:25:14.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:44.001925 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/
--rw-r--r--   0 root         (0) root         (0)      365 2023-06-10 12:25:06.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13222 2023-06-10 12:25:06.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:44.041926 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/
--rw-r--r--   0 root         (0) root         (0)      381 2023-06-10 12:25:06.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11207 2023-06-10 12:25:05.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11978 2023-06-10 12:25:05.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/get.py
--rw-r--r--   0 root         (0) root         (0)    15946 2023-06-10 12:25:06.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/put.py
--rw-r--r--   0 root         (0) root         (0)    10635 2023-06-10 12:25:37.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/rest.py
--rw-r--r--   0 root         (0) root         (0)    97752 2023-06-10 12:25:37.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:43.649917 iparapheur-provisioning-1.6.6/iparapheur_provisioning.egg-info/
--rw-r--r--   0 root         (0) root         (0)      421 2023-06-10 12:31:43.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13497 2023-06-10 12:31:43.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-10 12:31:43.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      118 2023-06-10 12:31:43.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-10 12:31:43.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-06-10 12:31:44.261931 iparapheur-provisioning-1.6.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1322 2023-06-10 12:25:37.000000 iparapheur-provisioning-1.6.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:43.609916 iparapheur-provisioning-1.6.6/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:44.153928 iparapheur-provisioning-1.6.6/test/test_models/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 12:25:37.000000 iparapheur-provisioning-1.6.6/test/test_models/__init__.py
--rw-r--r--   0 root         (0) root         (0)      682 2023-06-10 12:24:51.000000 iparapheur-provisioning-1.6.6/test/test_models/test_delegation_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      645 2023-06-10 12:24:54.000000 iparapheur-provisioning-1.6.6/test/test_models/test_desk_dto.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-06-10 12:24:55.000000 iparapheur-provisioning-1.6.6/test/test_models/test_desk_representation.py
--rw-r--r--   0 root         (0) root         (0)      669 2023-06-10 12:24:55.000000 iparapheur-provisioning-1.6.6/test/test_models/test_error_response.py
--rw-r--r--   0 root         (0) root         (0)      767 2023-06-10 12:24:56.000000 iparapheur-provisioning-1.6.6/test/test_models/test_external_signature_config_representation.py
--rw-r--r--   0 root         (0) root         (0)      736 2023-06-10 12:24:56.000000 iparapheur-provisioning-1.6.6/test/test_models/test_external_signature_config_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      718 2023-06-10 12:24:56.000000 iparapheur-provisioning-1.6.6/test/test_models/test_external_signature_provider.py
--rw-r--r--   0 root         (0) root         (0)      666 2023-06-10 12:24:56.000000 iparapheur-provisioning-1.6.6/test/test_models/test_folder_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      681 2023-06-10 12:24:56.000000 iparapheur-provisioning-1.6.6/test/test_models/test_internal_metadata.py
--rw-r--r--   0 root         (0) root         (0)      693 2023-06-10 12:24:56.000000 iparapheur-provisioning-1.6.6/test/test_models/test_layer_representation.py
--rw-r--r--   0 root         (0) root         (0)      662 2023-06-10 12:24:56.000000 iparapheur-provisioning-1.6.6/test/test_models/test_layer_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      661 2023-06-10 12:24:56.000000 iparapheur-provisioning-1.6.6/test/test_models/test_metadata_dto.py
--rw-r--r--   0 root         (0) root         (0)      705 2023-06-10 12:24:56.000000 iparapheur-provisioning-1.6.6/test/test_models/test_metadata_representation.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-06-10 12:24:56.000000 iparapheur-provisioning-1.6.6/test/test_models/test_metadata_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      665 2023-06-10 12:24:57.000000 iparapheur-provisioning-1.6.6/test/test_models/test_metadata_type.py
--rw-r--r--   0 root         (0) root         (0)      706 2023-06-10 12:24:57.000000 iparapheur-provisioning-1.6.6/test/test_models/test_page_desk_representation.py
--rw-r--r--   0 root         (0) root         (0)      718 2023-06-10 12:24:57.000000 iparapheur-provisioning-1.6.6/test/test_models/test_page_subtype_representation.py
--rw-r--r--   0 root         (0) root         (0)      706 2023-06-10 12:24:57.000000 iparapheur-provisioning-1.6.6/test/test_models/test_page_type_representation.py
--rw-r--r--   0 root         (0) root         (0)      706 2023-06-10 12:24:57.000000 iparapheur-provisioning-1.6.6/test/test_models/test_page_user_representation.py
--rw-r--r--   0 root         (0) root         (0)      673 2023-06-10 12:24:58.000000 iparapheur-provisioning-1.6.6/test/test_models/test_pageable_object.py
--rw-r--r--   0 root         (0) root         (0)      698 2023-06-10 12:24:58.000000 iparapheur-provisioning-1.6.6/test/test_models/test_pdf_signature_position.py
--rw-r--r--   0 root         (0) root         (0)      703 2023-06-10 12:24:58.000000 iparapheur-provisioning-1.6.6/test/test_models/test_seal_certificate_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      677 2023-06-10 12:24:58.000000 iparapheur-provisioning-1.6.6/test/test_models/test_signature_format.py
--rw-r--r--   0 root         (0) root         (0)      685 2023-06-10 12:24:58.000000 iparapheur-provisioning-1.6.6/test/test_models/test_signature_protocol.py
--rw-r--r--   0 root         (0) root         (0)      657 2023-06-10 12:24:58.000000 iparapheur-provisioning-1.6.6/test/test_models/test_sort_object.py
--rw-r--r--   0 root         (0) root         (0)      657 2023-06-10 12:24:59.000000 iparapheur-provisioning-1.6.6/test/test_models/test_subtype_dto.py
--rw-r--r--   0 root         (0) root         (0)      710 2023-06-10 12:24:59.000000 iparapheur-provisioning-1.6.6/test/test_models/test_subtype_layer_association.py
--rw-r--r--   0 root         (0) root         (0)      678 2023-06-10 12:24:59.000000 iparapheur-provisioning-1.6.6/test/test_models/test_subtype_layer_dto.py
--rw-r--r--   0 root         (0) root         (0)      690 2023-06-10 12:25:00.000000 iparapheur-provisioning-1.6.6/test/test_models/test_subtype_metadata_dto.py
--rw-r--r--   0 root         (0) root         (0)      701 2023-06-10 12:25:00.000000 iparapheur-provisioning-1.6.6/test/test_models/test_subtype_representation.py
--rw-r--r--   0 root         (0) root         (0)      653 2023-06-10 12:25:00.000000 iparapheur-provisioning-1.6.6/test/test_models/test_tenant_dto.py
--rw-r--r--   0 root         (0) root         (0)      697 2023-06-10 12:25:00.000000 iparapheur-provisioning-1.6.6/test/test_models/test_tenant_representation.py
--rw-r--r--   0 root         (0) root         (0)      666 2023-06-10 12:25:00.000000 iparapheur-provisioning-1.6.6/test/test_models/test_tenant_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      645 2023-06-10 12:25:00.000000 iparapheur-provisioning-1.6.6/test/test_models/test_type_dto.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-06-10 12:25:01.000000 iparapheur-provisioning-1.6.6/test/test_models/test_type_representation.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-06-10 12:25:01.000000 iparapheur-provisioning-1.6.6/test/test_models/test_typology_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      645 2023-06-10 12:25:02.000000 iparapheur-provisioning-1.6.6/test/test_models/test_user_dto.py
--rw-r--r--   0 root         (0) root         (0)      669 2023-06-10 12:25:02.000000 iparapheur-provisioning-1.6.6/test/test_models/test_user_privilege.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-06-10 12:25:05.000000 iparapheur-provisioning-1.6.6/test/test_models/test_user_representation.py
--rw-r--r--   0 root         (0) root         (0)      658 2023-06-10 12:25:05.000000 iparapheur-provisioning-1.6.6/test/test_models/test_user_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      715 2023-06-10 12:25:05.000000 iparapheur-provisioning-1.6.6/test/test_models/test_workflow_definition_sort_by.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:44.153928 iparapheur-provisioning-1.6.6/test/test_paths/
--rw-r--r--   0 root         (0) root         (0)     1995 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/test/test_paths/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:44.153928 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 12:25:12.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant/__init__.py
--rw-r--r--   0 root         (0) root         (0)      899 2023-06-10 12:25:12.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:44.157929 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 12:25:12.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)      925 2023-06-10 12:25:12.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      930 2023-06-10 12:25:12.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      916 2023-06-10 12:25:12.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:44.157929 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 12:25:09.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/__init__.py
--rw-r--r--   0 root         (0) root         (0)      924 2023-06-10 12:25:09.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_get.py
--rw-r--r--   0 root         (0) root         (0)      932 2023-06-10 12:25:09.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:44.161929 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 12:25:09.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)      956 2023-06-10 12:25:09.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-06-10 12:25:09.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      947 2023-06-10 12:25:09.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:44.161929 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/__init__.py
--rw-r--r--   0 root         (0) root         (0)      949 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_get.py
--rw-r--r--   0 root         (0) root         (0)      957 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:44.161929 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)      981 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      996 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:44.173929 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/__init__.py
--rw-r--r--   0 root         (0) root         (0)      993 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_get.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:44.189929 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1035 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)     1050 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)     1026 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:44.205930 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 12:25:14.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/__init__.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-06-10 12:25:14.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_get.py
--rw-r--r--   0 root         (0) root         (0)      936 2023-06-10 12:25:14.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:44.233930 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 12:25:14.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1047 2023-06-10 12:25:14.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-06-10 12:25:14.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      947 2023-06-10 12:25:14.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:44.241930 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_user/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 12:25:06.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_user/__init__.py
--rw-r--r--   0 root         (0) root         (0)      899 2023-06-10 12:25:06.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_user/test_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:44.245931 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_user_user_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 12:25:06.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_user_user_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)      932 2023-06-10 12:25:06.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      919 2023-06-10 12:25:06.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      902 2023-06-10 12:25:06.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:20:46.940128 iparapheur-provisioning-1.6.7/
+-rw-r--r--   0 root         (0) root         (0)     1111 2023-06-20 11:19:59.000000 iparapheur-provisioning-1.6.7/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      421 2023-06-20 11:20:46.940128 iparapheur-provisioning-1.6.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    17323 2023-06-20 11:19:59.000000 iparapheur-provisioning-1.6.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:20:46.908127 iparapheur-provisioning-1.6.7/iparapheur_provisioning/
+-rw-r--r--   0 root         (0) root         (0)      907 2023-06-20 11:19:59.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58620 2023-06-20 11:19:59.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:20:46.908127 iparapheur-provisioning-1.6.7/iparapheur_provisioning/apis/
+-rw-r--r--   0 root         (0) root         (0)      214 2023-06-20 11:19:59.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4776 2023-06-20 11:19:58.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/apis/path_to_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:20:46.912128 iparapheur-provisioning-1.6.7/iparapheur_provisioning/apis/paths/
+-rw-r--r--   0 root         (0) root         (0)      250 2023-06-20 11:19:58.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/apis/paths/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      157 2023-06-20 11:19:52.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-06-20 11:19:52.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id.py
+-rw-r--r--   0 root         (0) root         (0)      303 2023-06-20 11:19:50.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_desk.py
+-rw-r--r--   0 root         (0) root         (0)      458 2023-06-20 11:19:50.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id.py
+-rw-r--r--   0 root         (0) root         (0)      329 2023-06-20 11:19:58.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type.py
+-rw-r--r--   0 root         (0) root         (0)      493 2023-06-20 11:19:58.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id.py
+-rw-r--r--   0 root         (0) root         (0)      374 2023-06-20 11:19:58.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype.py
+-rw-r--r--   0 root         (0) root         (0)      566 2023-06-20 11:19:58.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id.py
+-rw-r--r--   0 root         (0) root         (0)      303 2023-06-20 11:19:54.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_user.py
+-rw-r--r--   0 root         (0) root         (0)      458 2023-06-20 11:19:54.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id.py
+-rw-r--r--   0 root         (0) root         (0)      150 2023-06-20 11:19:48.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_user.py
+-rw-r--r--   0 root         (0) root         (0)      393 2023-06-20 11:19:48.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_user_user_id.py
+-rw-r--r--   0 root         (0) root         (0)     1089 2023-06-20 11:19:58.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/apis/tag_to_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:20:46.912128 iparapheur-provisioning-1.6.7/iparapheur_provisioning/apis/tags/
+-rw-r--r--   0 root         (0) root         (0)      475 2023-06-20 11:19:58.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/apis/tags/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1031 2023-06-20 11:19:48.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/apis/tags/admin_all_users_api.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-06-20 11:19:50.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/apis/tags/admin_desk_api.py
+-rw-r--r--   0 root         (0) root         (0)      966 2023-06-20 11:19:52.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/apis/tags/admin_tenant_api.py
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-06-20 11:19:54.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/apis/tags/admin_tenant_user_api.py
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-06-20 11:19:58.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/apis/tags/admin_typology_api.py
+-rw-r--r--   0 root         (0) root         (0)    15677 2023-06-20 11:19:59.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     4598 2023-06-20 11:19:59.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:20:46.920128 iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/
+-rw-r--r--   0 root         (0) root         (0)      357 2023-06-20 11:19:59.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1426 2023-06-20 11:19:37.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/delegation_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)    24041 2023-06-20 11:19:39.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/desk_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3809 2023-06-20 11:19:40.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)     4553 2023-06-20 11:19:40.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/error_response.py
+-rw-r--r--   0 root         (0) root         (0)     4891 2023-06-20 11:19:40.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/external_signature_config_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1399 2023-06-20 11:19:40.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/external_signature_config_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1313 2023-06-20 11:19:41.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/external_signature_provider.py
+-rw-r--r--   0 root         (0) root         (0)     2680 2023-06-20 11:19:41.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/folder_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     2656 2023-06-20 11:19:41.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/internal_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     3284 2023-06-20 11:19:41.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/layer_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2023-06-20 11:19:41.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/layer_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     7233 2023-06-20 11:19:41.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5805 2023-06-20 11:19:41.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/metadata_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1356 2023-06-20 11:19:41.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/metadata_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1598 2023-06-20 11:19:42.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/metadata_type.py
+-rw-r--r--   0 root         (0) root         (0)     9105 2023-06-20 11:19:42.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/page_desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9132 2023-06-20 11:19:42.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/page_subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9105 2023-06-20 11:19:42.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/page_type_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9105 2023-06-20 11:19:43.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/page_user_representation.py
+-rw-r--r--   0 root         (0) root         (0)     5251 2023-06-20 11:19:43.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/pageable_object.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2023-06-20 11:19:43.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/pdf_signature_position.py
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-06-20 11:19:43.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/seal_certificate_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1527 2023-06-20 11:19:43.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/signature_format.py
+-rw-r--r--   0 root         (0) root         (0)     1273 2023-06-20 11:19:43.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/signature_protocol.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2023-06-20 11:19:43.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/sort_object.py
+-rw-r--r--   0 root         (0) root         (0)    28616 2023-06-20 11:19:44.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/subtype_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1307 2023-06-20 11:19:44.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/subtype_layer_association.py
+-rw-r--r--   0 root         (0) root         (0)     3930 2023-06-20 11:19:44.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/subtype_layer_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5468 2023-06-20 11:19:44.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/subtype_metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3288 2023-06-20 11:19:45.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)     3274 2023-06-20 11:19:45.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/tenant_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3286 2023-06-20 11:19:45.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/tenant_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-06-20 11:19:45.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/tenant_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     9365 2023-06-20 11:19:45.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/type_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4044 2023-06-20 11:19:45.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/type_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1144 2023-06-20 11:19:45.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/typology_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)    29666 2023-06-20 11:19:46.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/user_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1471 2023-06-20 11:19:46.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/user_privilege.py
+-rw-r--r--   0 root         (0) root         (0)     6504 2023-06-20 11:19:46.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/user_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1522 2023-06-20 11:19:47.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/user_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1256 2023-06-20 11:19:47.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/workflow_definition_sort_by.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:20:46.920128 iparapheur-provisioning-1.6.7/iparapheur_provisioning/models/
+-rw-r--r--   0 root         (0) root         (0)     3645 2023-06-20 11:19:59.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:20:46.920128 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-06-20 11:19:58.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:20:46.920128 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/
+-rw-r--r--   0 root         (0) root         (0)      369 2023-06-20 11:19:52.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13629 2023-06-20 11:19:51.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:20:46.920128 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/
+-rw-r--r--   0 root         (0) root         (0)      389 2023-06-20 11:19:52.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11083 2023-06-20 11:19:51.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11332 2023-06-20 11:19:51.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    15808 2023-06-20 11:19:52.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:20:46.920128 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/
+-rw-r--r--   0 root         (0) root         (0)      399 2023-06-20 11:19:50.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15034 2023-06-20 11:19:50.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/get.py
+-rw-r--r--   0 root         (0) root         (0)    16302 2023-06-20 11:19:49.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:20:46.920128 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/
+-rw-r--r--   0 root         (0) root         (0)      415 2023-06-20 11:19:50.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11337 2023-06-20 11:19:49.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11677 2023-06-20 11:19:50.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    16545 2023-06-20 11:19:49.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:20:46.920128 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/
+-rw-r--r--   0 root         (0) root         (0)      417 2023-06-20 11:19:58.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14728 2023-06-20 11:19:57.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/get.py
+-rw-r--r--   0 root         (0) root         (0)    15777 2023-06-20 11:19:55.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:20:46.924128 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/
+-rw-r--r--   0 root         (0) root         (0)      433 2023-06-20 11:19:58.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11337 2023-06-20 11:19:55.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11590 2023-06-20 11:19:56.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    15521 2023-06-20 11:19:57.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:20:46.924128 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/
+-rw-r--r--   0 root         (0) root         (0)      449 2023-06-20 11:19:58.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15050 2023-06-20 11:19:56.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/get.py
+-rw-r--r--   0 root         (0) root         (0)    16640 2023-06-20 11:19:54.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:20:46.924128 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/
+-rw-r--r--   0 root         (0) root         (0)      471 2023-06-20 11:19:58.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11672 2023-06-20 11:19:55.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11934 2023-06-20 11:19:56.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    16645 2023-06-20 11:19:57.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:20:46.924128 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/
+-rw-r--r--   0 root         (0) root         (0)      399 2023-06-20 11:19:54.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15944 2023-06-20 11:19:53.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/get.py
+-rw-r--r--   0 root         (0) root         (0)    15781 2023-06-20 11:19:52.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:20:46.924128 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/
+-rw-r--r--   0 root         (0) root         (0)      415 2023-06-20 11:19:54.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11407 2023-06-20 11:19:53.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11580 2023-06-20 11:19:52.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    16046 2023-06-20 11:19:54.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:20:46.924128 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/
+-rw-r--r--   0 root         (0) root         (0)      365 2023-06-20 11:19:48.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13222 2023-06-20 11:19:48.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:20:46.924128 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/
+-rw-r--r--   0 root         (0) root         (0)      381 2023-06-20 11:19:48.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11207 2023-06-20 11:19:47.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11978 2023-06-20 11:19:47.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    15946 2023-06-20 11:19:48.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/put.py
+-rw-r--r--   0 root         (0) root         (0)    10635 2023-06-20 11:19:59.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/rest.py
+-rw-r--r--   0 root         (0) root         (0)    97752 2023-06-20 11:19:59.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:20:46.908127 iparapheur-provisioning-1.6.7/iparapheur_provisioning.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      421 2023-06-20 11:20:46.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13497 2023-06-20 11:20:46.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:20:46.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      118 2023-06-20 11:20:46.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-20 11:20:46.000000 iparapheur-provisioning-1.6.7/iparapheur_provisioning.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-06-20 11:20:46.940128 iparapheur-provisioning-1.6.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-06-20 11:19:59.000000 iparapheur-provisioning-1.6.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:20:46.904127 iparapheur-provisioning-1.6.7/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:20:46.932128 iparapheur-provisioning-1.6.7/test/test_models/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 11:19:59.000000 iparapheur-provisioning-1.6.7/test/test_models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      682 2023-06-20 11:19:37.000000 iparapheur-provisioning-1.6.7/test/test_models/test_delegation_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      645 2023-06-20 11:19:39.000000 iparapheur-provisioning-1.6.7/test/test_models/test_desk_dto.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-06-20 11:19:40.000000 iparapheur-provisioning-1.6.7/test/test_models/test_desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-06-20 11:19:40.000000 iparapheur-provisioning-1.6.7/test/test_models/test_error_response.py
+-rw-r--r--   0 root         (0) root         (0)      767 2023-06-20 11:19:40.000000 iparapheur-provisioning-1.6.7/test/test_models/test_external_signature_config_representation.py
+-rw-r--r--   0 root         (0) root         (0)      736 2023-06-20 11:19:40.000000 iparapheur-provisioning-1.6.7/test/test_models/test_external_signature_config_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      718 2023-06-20 11:19:41.000000 iparapheur-provisioning-1.6.7/test/test_models/test_external_signature_provider.py
+-rw-r--r--   0 root         (0) root         (0)      666 2023-06-20 11:19:41.000000 iparapheur-provisioning-1.6.7/test/test_models/test_folder_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      681 2023-06-20 11:19:41.000000 iparapheur-provisioning-1.6.7/test/test_models/test_internal_metadata.py
+-rw-r--r--   0 root         (0) root         (0)      693 2023-06-20 11:19:41.000000 iparapheur-provisioning-1.6.7/test/test_models/test_layer_representation.py
+-rw-r--r--   0 root         (0) root         (0)      662 2023-06-20 11:19:41.000000 iparapheur-provisioning-1.6.7/test/test_models/test_layer_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      661 2023-06-20 11:19:41.000000 iparapheur-provisioning-1.6.7/test/test_models/test_metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)      705 2023-06-20 11:19:41.000000 iparapheur-provisioning-1.6.7/test/test_models/test_metadata_representation.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-06-20 11:19:41.000000 iparapheur-provisioning-1.6.7/test/test_models/test_metadata_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      665 2023-06-20 11:19:42.000000 iparapheur-provisioning-1.6.7/test/test_models/test_metadata_type.py
+-rw-r--r--   0 root         (0) root         (0)      706 2023-06-20 11:19:42.000000 iparapheur-provisioning-1.6.7/test/test_models/test_page_desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)      718 2023-06-20 11:19:42.000000 iparapheur-provisioning-1.6.7/test/test_models/test_page_subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)      706 2023-06-20 11:19:42.000000 iparapheur-provisioning-1.6.7/test/test_models/test_page_type_representation.py
+-rw-r--r--   0 root         (0) root         (0)      706 2023-06-20 11:19:43.000000 iparapheur-provisioning-1.6.7/test/test_models/test_page_user_representation.py
+-rw-r--r--   0 root         (0) root         (0)      673 2023-06-20 11:19:43.000000 iparapheur-provisioning-1.6.7/test/test_models/test_pageable_object.py
+-rw-r--r--   0 root         (0) root         (0)      698 2023-06-20 11:19:43.000000 iparapheur-provisioning-1.6.7/test/test_models/test_pdf_signature_position.py
+-rw-r--r--   0 root         (0) root         (0)      703 2023-06-20 11:19:43.000000 iparapheur-provisioning-1.6.7/test/test_models/test_seal_certificate_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      677 2023-06-20 11:19:43.000000 iparapheur-provisioning-1.6.7/test/test_models/test_signature_format.py
+-rw-r--r--   0 root         (0) root         (0)      685 2023-06-20 11:19:43.000000 iparapheur-provisioning-1.6.7/test/test_models/test_signature_protocol.py
+-rw-r--r--   0 root         (0) root         (0)      657 2023-06-20 11:19:43.000000 iparapheur-provisioning-1.6.7/test/test_models/test_sort_object.py
+-rw-r--r--   0 root         (0) root         (0)      657 2023-06-20 11:19:44.000000 iparapheur-provisioning-1.6.7/test/test_models/test_subtype_dto.py
+-rw-r--r--   0 root         (0) root         (0)      710 2023-06-20 11:19:44.000000 iparapheur-provisioning-1.6.7/test/test_models/test_subtype_layer_association.py
+-rw-r--r--   0 root         (0) root         (0)      678 2023-06-20 11:19:44.000000 iparapheur-provisioning-1.6.7/test/test_models/test_subtype_layer_dto.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-06-20 11:19:45.000000 iparapheur-provisioning-1.6.7/test/test_models/test_subtype_metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)      701 2023-06-20 11:19:45.000000 iparapheur-provisioning-1.6.7/test/test_models/test_subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)      653 2023-06-20 11:19:45.000000 iparapheur-provisioning-1.6.7/test/test_models/test_tenant_dto.py
+-rw-r--r--   0 root         (0) root         (0)      697 2023-06-20 11:19:45.000000 iparapheur-provisioning-1.6.7/test/test_models/test_tenant_representation.py
+-rw-r--r--   0 root         (0) root         (0)      666 2023-06-20 11:19:45.000000 iparapheur-provisioning-1.6.7/test/test_models/test_tenant_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      645 2023-06-20 11:19:45.000000 iparapheur-provisioning-1.6.7/test/test_models/test_type_dto.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-06-20 11:19:45.000000 iparapheur-provisioning-1.6.7/test/test_models/test_type_representation.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-06-20 11:19:45.000000 iparapheur-provisioning-1.6.7/test/test_models/test_typology_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      645 2023-06-20 11:19:46.000000 iparapheur-provisioning-1.6.7/test/test_models/test_user_dto.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-06-20 11:19:46.000000 iparapheur-provisioning-1.6.7/test/test_models/test_user_privilege.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-06-20 11:19:47.000000 iparapheur-provisioning-1.6.7/test/test_models/test_user_representation.py
+-rw-r--r--   0 root         (0) root         (0)      658 2023-06-20 11:19:47.000000 iparapheur-provisioning-1.6.7/test/test_models/test_user_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      715 2023-06-20 11:19:47.000000 iparapheur-provisioning-1.6.7/test/test_models/test_workflow_definition_sort_by.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:20:46.932128 iparapheur-provisioning-1.6.7/test/test_paths/
+-rw-r--r--   0 root         (0) root         (0)     1995 2023-06-20 11:19:58.000000 iparapheur-provisioning-1.6.7/test/test_paths/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:20:46.932128 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 11:19:52.000000 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      899 2023-06-20 11:19:52.000000 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:20:46.932128 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 11:19:52.000000 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      925 2023-06-20 11:19:52.000000 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      930 2023-06-20 11:19:52.000000 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      916 2023-06-20 11:19:52.000000 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:20:46.932128 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 11:19:50.000000 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      924 2023-06-20 11:19:50.000000 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      932 2023-06-20 11:19:50.000000 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:20:46.936128 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 11:19:50.000000 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      956 2023-06-20 11:19:50.000000 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-06-20 11:19:50.000000 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      947 2023-06-20 11:19:50.000000 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:20:46.936128 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 11:19:58.000000 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      949 2023-06-20 11:19:58.000000 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      957 2023-06-20 11:19:58.000000 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:20:46.936128 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 11:19:58.000000 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      981 2023-06-20 11:19:58.000000 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      996 2023-06-20 11:19:58.000000 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-06-20 11:19:58.000000 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:20:46.936128 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 11:19:58.000000 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      993 2023-06-20 11:19:58.000000 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_get.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-06-20 11:19:58.000000 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:20:46.936128 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 11:19:58.000000 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1035 2023-06-20 11:19:58.000000 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)     1050 2023-06-20 11:19:58.000000 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-06-20 11:19:58.000000 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:20:46.936128 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 11:19:54.000000 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-06-20 11:19:54.000000 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      936 2023-06-20 11:19:54.000000 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:20:46.936128 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 11:19:54.000000 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-06-20 11:19:54.000000 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-06-20 11:19:54.000000 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      947 2023-06-20 11:19:54.000000 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:20:46.936128 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_user/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 11:19:48.000000 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      899 2023-06-20 11:19:48.000000 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_user/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:20:46.940128 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_user_user_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 11:19:48.000000 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_user_user_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      911 2023-06-20 11:19:48.000000 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      919 2023-06-20 11:19:48.000000 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      902 2023-06-20 11:19:48.000000 iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_put.py
```

### Comparing `iparapheur-provisioning-1.6.6/LICENSE.md` & `iparapheur-provisioning-1.6.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/README.md` & `iparapheur-provisioning-1.6.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 The main link between every sub-services, integrating business code logic.
 
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: DEVELOP
-- Package version: 1.6.6
+- Package version: 1.6.7
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://libriciel.fr](https://libriciel.fr)
 
 ## Requirements.
 
 Python &gt;&#x3D;3.7
```

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/__init__.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     iparapheur v5.x main core application.  The main link between every sub-services, integrating business code logic.   # noqa: E501
 
     The version of the OpenAPI document: DEVELOP
     Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
-__version__ = "1.6.6"
+__version__ = "1.6.7"
 
 # import ApiClient
 from iparapheur_provisioning.api_client import ApiClient
 
 # import Configuration
 from iparapheur_provisioning.configuration import Configuration
```

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/api_client.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1000,15 +1000,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = HTTPHeaderDict()
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.6.6/python'
+        self.user_agent = 'OpenAPI-Generator/1.6.7/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/path_to_api.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/tag_to_api.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/apis/tag_to_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/tags/admin_all_users_api.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/apis/tags/admin_all_users_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/tags/admin_desk_api.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/apis/tags/admin_desk_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/tags/admin_tenant_api.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/apis/tags/admin_tenant_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/tags/admin_tenant_user_api.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/apis/tags/admin_tenant_user_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/tags/admin_typology_api.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/apis/tags/admin_typology_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/configuration.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,15 +365,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: DEVELOP\n"\
-               "SDK Package Version: 1.6.6".\
+               "SDK Package Version: 1.6.7".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/exceptions.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/exceptions.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/delegation_sort_by.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/delegation_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/desk_dto.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/desk_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/desk_representation.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/desk_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/error_response.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/error_response.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/external_signature_config_representation.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/external_signature_config_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/external_signature_config_sort_by.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/external_signature_config_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/external_signature_provider.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/external_signature_provider.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/folder_sort_by.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/folder_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/internal_metadata.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/internal_metadata.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/layer_representation.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/layer_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/layer_sort_by.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/layer_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/metadata_dto.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/metadata_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/metadata_representation.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/metadata_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/metadata_sort_by.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/metadata_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/metadata_type.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/metadata_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/page_desk_representation.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/page_desk_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/page_subtype_representation.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/page_subtype_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/page_type_representation.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/page_type_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/page_user_representation.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/page_user_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/pageable_object.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/pageable_object.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/pdf_signature_position.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/pdf_signature_position.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/seal_certificate_sort_by.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/seal_certificate_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/signature_format.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/signature_format.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/signature_protocol.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/signature_protocol.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/sort_object.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/sort_object.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/subtype_dto.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/subtype_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/subtype_layer_association.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/subtype_layer_association.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/subtype_layer_dto.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/subtype_layer_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/subtype_metadata_dto.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/subtype_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/subtype_representation.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/subtype_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/tenant_dto.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/tenant_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/tenant_representation.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/tenant_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/tenant_sort_by.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/tenant_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/type_dto.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/type_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/type_representation.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/type_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/typology_sort_by.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/typology_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/user_dto.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/user_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/user_privilege.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/user_privilege.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/user_representation.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/user_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/user_sort_by.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/user_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/workflow_definition_sort_by.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/model/workflow_definition_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/models/__init__.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/models/__init__.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/__init__.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/post.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -40,115 +40,115 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor201ResponseBodyApplicationJson = TenantDto
 
 
 @dataclass
-class ApiResponseFor400(api_client.ApiResponse):
+class ApiResponseFor201(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
+        SchemaFor201ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_400 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor400,
+_response_for_201 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyApplicationJson),
+            schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
-SchemaFor201ResponseBodyApplicationJson = TenantDto
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor201(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor201ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_201 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor201,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor201ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '401': _response_for_401,
-    '400': _response_for_400,
     '403': _response_for_403,
     '201': _response_for_201,
     '507': _response_for_507,
+    '401': _response_for_401,
+    '400': _response_for_400,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/delete.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -54,88 +54,88 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TenantIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 
 
 @dataclass
 class ApiResponseFor204(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_204 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor204,
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '404': _response_for_404,
+    '403': _response_for_403,
     '204': _response_for_204,
+    '404': _response_for_404,
     '401': _response_for_401,
-    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/get.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -55,95 +55,95 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TenantIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = TenantDto
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = TenantDto
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '404': _response_for_404,
-    '401': _response_for_401,
     '403': _response_for_403,
     '200': _response_for_200,
+    '404': _response_for_404,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/put.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,115 +66,115 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = TenantDto
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor400(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_400 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor400,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = TenantDto
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '403': _response_for_403,
+    '200': _response_for_200,
     '404': _response_for_404,
     '401': _response_for_401,
     '400': _response_for_400,
-    '403': _response_for_403,
-    '200': _response_for_200,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/get.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -143,95 +143,95 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TenantIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = PageDeskRepresentation
 
 
 @dataclass
-class ApiResponseFor400(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_400 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor400,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = PageDeskRepresentation
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '401': _response_for_401,
-    '400': _response_for_400,
     '403': _response_for_403,
     '200': _response_for_200,
+    '401': _response_for_401,
+    '400': _response_for_400,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/post.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,135 +66,135 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor409(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor409ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_409 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor409,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor409ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor201ResponseBodyApplicationJson = DeskDto
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor201(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor201ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_201 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
-SchemaFor201ResponseBodyApplicationJson = DeskDto
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor201(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor201ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_201 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor201,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor201ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
-SchemaFor409ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor409(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor409ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_409 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor409,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor409ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '404': _response_for_404,
-    '401': _response_for_401,
     '403': _response_for_403,
-    '201': _response_for_201,
     '409': _response_for_409,
+    '201': _response_for_201,
     '507': _response_for_507,
+    '404': _response_for_404,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/delete.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -62,88 +62,88 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=DeskIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 
 
 @dataclass
 class ApiResponseFor204(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_204 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor204,
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '404': _response_for_404,
+    '403': _response_for_403,
     '204': _response_for_204,
+    '404': _response_for_404,
     '401': _response_for_401,
-    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/get.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -63,95 +63,95 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=DeskIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = DeskDto
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = DeskDto
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '404': _response_for_404,
-    '401': _response_for_401,
     '403': _response_for_403,
     '200': _response_for_200,
+    '404': _response_for_404,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/put.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,135 +74,135 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = DeskDto
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor409(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor409ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_409 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor409,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor409ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = DeskDto
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
-SchemaFor409ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor409(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor409ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_409 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor409,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor409ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '404': _response_for_404,
-    '401': _response_for_401,
     '403': _response_for_403,
     '200': _response_for_200,
     '409': _response_for_409,
     '507': _response_for_507,
+    '404': _response_for_404,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/get.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -135,95 +135,95 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TenantIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = PageTypeRepresentation
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = PageTypeRepresentation
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '404': _response_for_404,
-    '401': _response_for_401,
     '403': _response_for_403,
     '200': _response_for_200,
+    '404': _response_for_404,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/post.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,50 +66,50 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor409(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor409ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_409 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor409,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor409ResponseBodyApplicationJson),
     },
 )
 SchemaFor201ResponseBodyApplicationJson = TypeDto
 
 
 @dataclass
 class ApiResponseFor201(api_client.ApiResponse):
@@ -123,58 +123,58 @@
 _response_for_201 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
-SchemaFor409ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor409(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor409ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_409 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor409,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor409ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '401': _response_for_401,
     '403': _response_for_403,
-    '201': _response_for_201,
     '409': _response_for_409,
+    '201': _response_for_201,
     '507': _response_for_507,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/delete.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -62,88 +62,88 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TypeIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 
 
 @dataclass
 class ApiResponseFor204(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_204 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor204,
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '404': _response_for_404,
+    '403': _response_for_403,
     '204': _response_for_204,
+    '404': _response_for_404,
     '401': _response_for_401,
-    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/get.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -63,95 +63,95 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TypeIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = TypeDto
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = TypeDto
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '404': _response_for_404,
-    '401': _response_for_401,
     '403': _response_for_403,
     '200': _response_for_200,
+    '404': _response_for_404,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/put.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,95 +74,95 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = TypeDto
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = TypeDto
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '404': _response_for_404,
-    '401': _response_for_401,
     '403': _response_for_403,
     '200': _response_for_200,
+    '404': _response_for_404,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/get.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -143,95 +143,95 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TypeIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = PageSubtypeRepresentation
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = PageSubtypeRepresentation
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '404': _response_for_404,
-    '401': _response_for_401,
     '403': _response_for_403,
     '200': _response_for_200,
+    '404': _response_for_404,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/post.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,135 +74,135 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor409(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor409ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_409 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor409,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor409ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor201ResponseBodyApplicationJson = SubtypeDto
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor201(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor201ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_201 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
-SchemaFor201ResponseBodyApplicationJson = SubtypeDto
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor201(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor201ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_201 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor201,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor201ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
-SchemaFor409ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor409(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor409ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_409 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor409,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor409ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '404': _response_for_404,
-    '401': _response_for_401,
     '403': _response_for_403,
-    '201': _response_for_201,
     '409': _response_for_409,
+    '201': _response_for_201,
     '507': _response_for_507,
+    '404': _response_for_404,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/delete.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -70,88 +70,88 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=SubtypeIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 
 
 @dataclass
 class ApiResponseFor204(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_204 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor204,
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '404': _response_for_404,
+    '403': _response_for_403,
     '204': _response_for_204,
+    '404': _response_for_404,
     '401': _response_for_401,
-    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/get.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -71,95 +71,95 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=SubtypeIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = SubtypeDto
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = SubtypeDto
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '404': _response_for_404,
-    '401': _response_for_401,
     '403': _response_for_403,
     '200': _response_for_200,
+    '404': _response_for_404,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/put.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -82,31 +82,31 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 SchemaFor204ResponseBodyApplicationJson = SubtypeDto
 
 
 @dataclass
 class ApiResponseFor204(api_client.ApiResponse):
@@ -120,50 +120,50 @@
 _response_for_204 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor204,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor204ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 SchemaFor200ResponseBodyApplicationJson = SubtypeDto
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
@@ -178,18 +178,18 @@
     response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '404': _response_for_404,
+    '403': _response_for_403,
     '204': _response_for_204,
+    '404': _response_for_404,
     '401': _response_for_401,
-    '403': _response_for_403,
     '200': _response_for_200,
 }
 _all_accept_content_types = (
     'application/json',
 )
```

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/get.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -151,115 +151,115 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TenantIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = PageUserRepresentation
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor400(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_400 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor400,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = PageUserRepresentation
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '403': _response_for_403,
+    '200': _response_for_200,
     '404': _response_for_404,
     '401': _response_for_401,
     '400': _response_for_400,
-    '403': _response_for_403,
-    '200': _response_for_200,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/post.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,50 +66,50 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor409(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor409ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_409 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor409,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor409ResponseBodyApplicationJson),
     },
 )
 SchemaFor201ResponseBodyApplicationJson = UserDto
 
 
 @dataclass
 class ApiResponseFor201(api_client.ApiResponse):
@@ -123,58 +123,58 @@
 _response_for_201 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
-SchemaFor409ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor409(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor409ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_409 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor409,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor409ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '401': _response_for_401,
     '403': _response_for_403,
-    '201': _response_for_201,
     '409': _response_for_409,
+    '201': _response_for_201,
     '507': _response_for_507,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/delete.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -62,14 +62,33 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=UserIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+
+
+@dataclass
+class ApiResponseFor403(api_client.ApiResponse):
+    response: urllib3.HTTPResponse
+    body: typing.Union[
+        SchemaFor403ResponseBodyApplicationJson,
+    ]
+    headers: schemas.Unset = schemas.unset
+
+
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
+    content={
+        'application/json': api_client.MediaType(
+            schema=SchemaFor403ResponseBodyApplicationJson),
+    },
+)
 
 
 @dataclass
 class ApiResponseFor204(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
@@ -112,38 +131,19 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
-
-
-@dataclass
-class ApiResponseFor403(api_client.ApiResponse):
-    response: urllib3.HTTPResponse
-    body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
-    ]
-    headers: schemas.Unset = schemas.unset
-
-
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
-    content={
-        'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
-    },
-)
 _status_code_to_response = {
+    '403': _response_for_403,
     '204': _response_for_204,
     '406': _response_for_406,
     '401': _response_for_401,
-    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/get.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/get.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -63,95 +63,95 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=UserIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = UserDto
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = UserDto
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '404': _response_for_404,
-    '401': _response_for_401,
     '403': _response_for_403,
     '200': _response_for_200,
+    '404': _response_for_404,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/put.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,115 +74,115 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor406ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = UserDto
 
 
 @dataclass
-class ApiResponseFor406(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor406ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_406 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor406,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor406ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor406ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor406(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor406ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_406 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor406,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor406ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = UserDto
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '403': _response_for_403,
+    '200': _response_for_200,
     '404': _response_for_404,
     '406': _response_for_406,
     '401': _response_for_401,
-    '403': _response_for_403,
-    '200': _response_for_200,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/get.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -117,95 +117,95 @@
     style=api_client.ParameterStyle.FORM,
     schema=SearchTermSchema,
     explode=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = PageUserRepresentation
 
 
 @dataclass
-class ApiResponseFor400(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_400 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor400,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = PageUserRepresentation
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '401': _response_for_401,
-    '400': _response_for_400,
     '403': _response_for_403,
     '200': _response_for_200,
+    '401': _response_for_401,
+    '400': _response_for_400,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/delete.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/delete.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,33 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=UserIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+
+
+@dataclass
+class ApiResponseFor403(api_client.ApiResponse):
+    response: urllib3.HTTPResponse
+    body: typing.Union[
+        SchemaFor403ResponseBodyApplicationJson,
+    ]
+    headers: schemas.Unset = schemas.unset
+
+
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
+    content={
+        'application/json': api_client.MediaType(
+            schema=SchemaFor403ResponseBodyApplicationJson),
+    },
+)
 
 
 @dataclass
 class ApiResponseFor204(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
@@ -104,38 +123,19 @@
 _response_for_400 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
-
-
-@dataclass
-class ApiResponseFor403(api_client.ApiResponse):
-    response: urllib3.HTTPResponse
-    body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
-    ]
-    headers: schemas.Unset = schemas.unset
-
-
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
-    content={
-        'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
-    },
-)
 _status_code_to_response = {
+    '403': _response_for_403,
     '204': _response_for_204,
     '401': _response_for_401,
     '400': _response_for_400,
-    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/get.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -55,115 +55,115 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=UserIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = UserDto
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor400(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_400 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor400,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = UserDto
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '403': _response_for_403,
+    '200': _response_for_200,
     '404': _response_for_404,
     '401': _response_for_401,
     '400': _response_for_400,
-    '403': _response_for_403,
-    '200': _response_for_200,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/put.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,115 +66,115 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = UserDto
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor400(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_400 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor400,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = UserDto
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '403': _response_for_403,
+    '200': _response_for_200,
     '404': _response_for_404,
     '401': _response_for_401,
     '400': _response_for_400,
-    '403': _response_for_403,
-    '200': _response_for_200,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/rest.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/rest.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning/schemas.py` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning/schemas.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/iparapheur_provisioning.egg-info/SOURCES.txt` & `iparapheur-provisioning-1.6.7/iparapheur_provisioning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/setup.py` & `iparapheur-provisioning-1.6.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "iparapheur-provisioning"
-VERSION = "1.6.6"
+VERSION = "1.6.7"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `iparapheur-provisioning-1.6.6/test/test_models/test_delegation_sort_by.py` & `iparapheur-provisioning-1.6.7/test/test_models/test_delegation_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/test/test_models/test_desk_dto.py` & `iparapheur-provisioning-1.6.7/test/test_models/test_desk_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/test/test_models/test_desk_representation.py` & `iparapheur-provisioning-1.6.7/test/test_models/test_desk_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/test/test_models/test_error_response.py` & `iparapheur-provisioning-1.6.7/test/test_models/test_error_response.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/test/test_models/test_external_signature_config_representation.py` & `iparapheur-provisioning-1.6.7/test/test_models/test_external_signature_config_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/test/test_models/test_external_signature_config_sort_by.py` & `iparapheur-provisioning-1.6.7/test/test_models/test_external_signature_config_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/test/test_models/test_external_signature_provider.py` & `iparapheur-provisioning-1.6.7/test/test_models/test_external_signature_provider.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/test/test_models/test_folder_sort_by.py` & `iparapheur-provisioning-1.6.7/test/test_models/test_folder_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/test/test_models/test_internal_metadata.py` & `iparapheur-provisioning-1.6.7/test/test_models/test_internal_metadata.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/test/test_models/test_layer_representation.py` & `iparapheur-provisioning-1.6.7/test/test_models/test_layer_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/test/test_models/test_layer_sort_by.py` & `iparapheur-provisioning-1.6.7/test/test_models/test_layer_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/test/test_models/test_metadata_dto.py` & `iparapheur-provisioning-1.6.7/test/test_models/test_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/test/test_models/test_metadata_representation.py` & `iparapheur-provisioning-1.6.7/test/test_models/test_metadata_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/test/test_models/test_metadata_sort_by.py` & `iparapheur-provisioning-1.6.7/test/test_models/test_metadata_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/test/test_models/test_metadata_type.py` & `iparapheur-provisioning-1.6.7/test/test_models/test_metadata_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/test/test_models/test_page_desk_representation.py` & `iparapheur-provisioning-1.6.7/test/test_models/test_page_desk_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/test/test_models/test_page_subtype_representation.py` & `iparapheur-provisioning-1.6.7/test/test_models/test_page_subtype_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/test/test_models/test_page_type_representation.py` & `iparapheur-provisioning-1.6.7/test/test_models/test_page_type_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/test/test_models/test_page_user_representation.py` & `iparapheur-provisioning-1.6.7/test/test_models/test_page_user_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/test/test_models/test_pageable_object.py` & `iparapheur-provisioning-1.6.7/test/test_models/test_pageable_object.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/test/test_models/test_pdf_signature_position.py` & `iparapheur-provisioning-1.6.7/test/test_models/test_pdf_signature_position.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/test/test_models/test_seal_certificate_sort_by.py` & `iparapheur-provisioning-1.6.7/test/test_models/test_seal_certificate_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/test/test_models/test_signature_format.py` & `iparapheur-provisioning-1.6.7/test/test_models/test_signature_format.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/test/test_models/test_signature_protocol.py` & `iparapheur-provisioning-1.6.7/test/test_models/test_signature_protocol.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/test/test_models/test_sort_object.py` & `iparapheur-provisioning-1.6.7/test/test_models/test_sort_object.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/test/test_models/test_subtype_dto.py` & `iparapheur-provisioning-1.6.7/test/test_models/test_subtype_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/test/test_models/test_subtype_layer_association.py` & `iparapheur-provisioning-1.6.7/test/test_models/test_subtype_layer_association.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/test/test_models/test_subtype_layer_dto.py` & `iparapheur-provisioning-1.6.7/test/test_models/test_subtype_layer_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/test/test_models/test_subtype_metadata_dto.py` & `iparapheur-provisioning-1.6.7/test/test_models/test_subtype_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/test/test_models/test_subtype_representation.py` & `iparapheur-provisioning-1.6.7/test/test_models/test_subtype_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/test/test_models/test_tenant_dto.py` & `iparapheur-provisioning-1.6.7/test/test_models/test_tenant_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/test/test_models/test_tenant_representation.py` & `iparapheur-provisioning-1.6.7/test/test_models/test_tenant_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/test/test_models/test_tenant_sort_by.py` & `iparapheur-provisioning-1.6.7/test/test_models/test_tenant_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/test/test_models/test_type_dto.py` & `iparapheur-provisioning-1.6.7/test/test_models/test_type_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/test/test_models/test_type_representation.py` & `iparapheur-provisioning-1.6.7/test/test_models/test_type_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/test/test_models/test_typology_sort_by.py` & `iparapheur-provisioning-1.6.7/test/test_models/test_typology_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/test/test_models/test_user_dto.py` & `iparapheur-provisioning-1.6.7/test/test_models/test_user_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/test/test_models/test_user_privilege.py` & `iparapheur-provisioning-1.6.7/test/test_models/test_user_privilege.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/test/test_models/test_user_representation.py` & `iparapheur-provisioning-1.6.7/test/test_models/test_user_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/test/test_models/test_user_sort_by.py` & `iparapheur-provisioning-1.6.7/test/test_models/test_user_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/test/test_models/test_workflow_definition_sort_by.py` & `iparapheur-provisioning-1.6.7/test/test_models/test_workflow_definition_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/test/test_paths/__init__.py` & `iparapheur-provisioning-1.6.7/test/test_paths/__init__.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant/test_post.py` & `iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_put.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant import post  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id import put  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenant(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenant unit test stubs
-        Create a new tenant  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantId unit test stubs
+        Edit a tenant  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
+        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 401
+    response_status = 403
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_delete.py` & `iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_get.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,34 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id import delete  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
 class TestApiProvisioningV1AdminTenantTenantId(ApiTestMixin, unittest.TestCase):
     """
     ApiProvisioningV1AdminTenantTenantId unit test stubs
-        Delete a tenant  # noqa: E501
+        Get a full tenant description  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 404
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_get.py` & `iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_post.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,34 +8,36 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user import post  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdUser(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantId unit test stubs
-        Get a full tenant description  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdUser unit test stubs
+        Create a new user  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 404
+    response_status = 403
+
+
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_put.py` & `iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_get.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,36 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id import put  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_desk import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdDesk(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantId unit test stubs
-        Edit a tenant  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdDesk unit test stubs
+        List desks  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 404
-
-
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_get.py` & `iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_delete.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,34 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_desk import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id import delete  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdDesk(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdDeskDeskId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdDesk unit test stubs
-        List desks  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdDeskDeskId unit test stubs
+        Delete a desk  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 401
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_post.py` & `iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_post.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 404
+    response_status = 403
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_delete.py` & `iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_get.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,34 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id import delete  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
 class TestApiProvisioningV1AdminTenantTenantIdDeskDeskId(ApiTestMixin, unittest.TestCase):
     """
     ApiProvisioningV1AdminTenantTenantIdDeskDeskId unit test stubs
-        Delete a desk  # noqa: E501
+        Get a full desk description  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 404
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_get.py` & `iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_get.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,34 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user_user_id import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdDeskDeskId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdUserUserId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdDeskDeskId unit test stubs
-        Get a full desk description  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdUserUserId unit test stubs
+        Get a full user description  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 404
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_put.py` & `iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_put.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 404
+    response_status = 403
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_get.py` & `iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_get.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,34 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdTypologyType(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdTypologyType unit test stubs
-        List types  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeId unit test stubs
+        Get a type with every information set  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 404
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_post.py` & `iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_post.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 401
+    response_status = 403
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_delete.py` & `iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_delete.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 404
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_get.py` & `iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_put.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,34 +8,36 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user_user_id import put  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdUserUserId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeId unit test stubs
-        Get a type with every information set  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdUserUserId unit test stubs
+        Edit a user  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 404
+    response_status = 403
+
+
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_put.py` & `iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_put.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 404
+    response_status = 403
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_get.py` & `iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_get.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 404
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_post.py` & `iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_get.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,36 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype import post  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtype(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdUser(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtype unit test stubs
-        Create a subtype  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdUser unit test stubs
+        List all users associated with the tenant  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 404
-
-
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_delete.py` & `iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_delete.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 404
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_get.py` & `iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_put.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,34 +8,36 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id import put  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
 class TestApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeId(ApiTestMixin, unittest.TestCase):
     """
     ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeId unit test stubs
-        Get a subtype with every information set  # noqa: E501
+        Edit a subtype  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 404
+    response_status = 403
+
+
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_put.py` & `iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_get.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,36 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id import put  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdTypologyType(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeId unit test stubs
-        Edit a subtype  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdTypologyType unit test stubs
+        List types  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 404
-
-
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_get.py` & `iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_user/test_get.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,34 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_user import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdUser(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminUser(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdUser unit test stubs
-        List all users associated with the tenant  # noqa: E501
+    ApiProvisioningV1AdminUser unit test stubs
+        List all users on the instance  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 404
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_post.py` & `iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_put.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user import post  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_user_user_id import put  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdUser(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminUserUserId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdUser unit test stubs
-        Create a new user  # noqa: E501
+    ApiProvisioningV1AdminUserUserId unit test stubs
+        Edit a user  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
+        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 401
+    response_status = 403
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_delete.py` & `iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_delete.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,13 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 204
-    response_body = ''
+    response_status = 403
+
+
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_get.py` & `iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_get.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,34 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user_user_id import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_user_user_id import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdUserUserId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminUserUserId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdUserUserId unit test stubs
-        Get a full user description  # noqa: E501
+    ApiProvisioningV1AdminUserUserId unit test stubs
+        Get a full user representation  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 404
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_put.py` & `iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_delete.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,36 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user_user_id import put  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id import delete  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdUserUserId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdUserUserId unit test stubs
-        Edit a user  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantId unit test stubs
+        Delete a tenant  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
+        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 404
-
-
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_user/test_get.py` & `iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_delete.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,34 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_user import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_user_user_id import delete  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminUser(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminUserUserId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminUser unit test stubs
-        List all users on the instance  # noqa: E501
+    ApiProvisioningV1AdminUserUserId unit test stubs
+        Delete a user  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 401
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_delete.py` & `iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant/test_post.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,33 +8,36 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_user_user_id import delete  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant import post  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminUserUserId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenant(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminUserUserId unit test stubs
-        Delete a user  # noqa: E501
+    ApiProvisioningV1AdminTenant unit test stubs
+        Create a new tenant  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
+        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 204
-    response_body = ''
+    response_status = 403
+
+
+
+
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_get.py` & `iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_post.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,34 +8,36 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_user_user_id import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype import post  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminUserUserId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtype(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminUserUserId unit test stubs
-        Get a full user representation  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtype unit test stubs
+        Create a subtype  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 404
+    response_status = 403
+
+
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_put.py` & `iparapheur-provisioning-1.6.7/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_get.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,36 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_user_user_id import put  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminUserUserId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminUserUserId unit test stubs
-        Edit a user  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeId unit test stubs
+        Get a subtype with every information set  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 404
-
-
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

