# Comparing `tmp/encord-0.1.82.tar.gz` & `tmp/encord-0.1.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encord-0.1.82.tar", max compression
+gzip compressed data, was "encord-0.1.83.tar", max compression
```

## Comparing `encord-0.1.82.tar` & `encord-0.1.83.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0    11330 2023-06-13 15:08:20.190491 encord-0.1.82/LICENSE
--rw-r--r--   0        0        0     2037 2023-06-13 15:08:20.190491 encord-0.1.82/README.md
--rw-r--r--   0        0        0       84 2023-06-13 15:08:20.190491 encord-0.1.82/cord/__init__.py
--rw-r--r--   0        0        0      158 2023-06-13 15:08:20.206491 encord-0.1.82/encord/__init__.py
--rw-r--r--   0        0        0      214 2023-06-13 15:08:20.206491 encord-0.1.82/encord/_version.py
--rw-r--r--   0        0        0    49810 2023-06-13 15:08:20.206491 encord-0.1.82/encord/client.py
--rw-r--r--   0        0        0    10843 2023-06-13 15:08:20.206491 encord-0.1.82/encord/configs.py
--rw-r--r--   0        0        0        0 2023-06-13 15:08:20.206491 encord-0.1.82/encord/constants/__init__.py
--rw-r--r--   0        0        0      810 2023-06-13 15:08:20.206491 encord-0.1.82/encord/constants/enums.py
--rw-r--r--   0        0        0     3293 2023-06-13 15:08:20.206491 encord-0.1.82/encord/constants/model.py
--rw-r--r--   0        0        0     6068 2023-06-13 15:08:20.206491 encord-0.1.82/encord/constants/model_weights.py
--rw-r--r--   0        0        0     1119 2023-06-13 15:08:20.206491 encord-0.1.82/encord/constants/string_constants.py
--rw-r--r--   0        0        0        0 2023-06-13 15:08:20.206491 encord-0.1.82/encord/constants/test/__init__.py
--rw-r--r--   0        0        0      634 2023-06-13 15:08:20.206491 encord-0.1.82/encord/constants/test/test_enums.py
--rw-r--r--   0        0        0    16035 2023-06-13 15:08:20.206491 encord-0.1.82/encord/dataset.py
--rw-r--r--   0        0        0     6351 2023-06-13 15:08:20.206491 encord-0.1.82/encord/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-13 15:08:20.206491 encord-0.1.82/encord/http/__init__.py
--rw-r--r--   0        0        0     5315 2023-06-13 15:08:20.206491 encord-0.1.82/encord/http/bundle.py
--rw-r--r--   0        0        0      535 2023-06-13 15:08:20.206491 encord-0.1.82/encord/http/constants.py
--rw-r--r--   0        0        0     7234 2023-06-13 15:08:20.206491 encord-0.1.82/encord/http/error_utils.py
--rw-r--r--   0        0        0      103 2023-06-13 15:08:20.206491 encord-0.1.82/encord/http/limits.py
--rw-r--r--   0        0        0     7928 2023-06-13 15:08:20.206491 encord-0.1.82/encord/http/querier.py
--rw-r--r--   0        0        0      697 2023-06-13 15:08:20.206491 encord-0.1.82/encord/http/query_methods.py
--rw-r--r--   0        0        0     1719 2023-06-13 15:08:20.206491 encord-0.1.82/encord/http/request.py
--rw-r--r--   0        0        0     6182 2023-06-13 15:08:20.206491 encord-0.1.82/encord/http/utils.py
--rw-r--r--   0        0        0      340 2023-06-13 15:08:20.206491 encord-0.1.82/encord/objects/__init__.py
--rw-r--r--   0        0        0     5164 2023-06-13 15:08:20.206491 encord-0.1.82/encord/objects/bitmask.py
--rw-r--r--   0        0        0      182 2023-06-13 15:08:20.206491 encord-0.1.82/encord/objects/classification.py
--rw-r--r--   0        0        0    31614 2023-06-13 15:08:20.206491 encord-0.1.82/encord/objects/common.py
--rw-r--r--   0        0        0      151 2023-06-13 15:08:20.206491 encord-0.1.82/encord/objects/constants.py
--rw-r--r--   0        0        0     5748 2023-06-13 15:08:20.206491 encord-0.1.82/encord/objects/coordinates.py
--rw-r--r--   0        0        0     3461 2023-06-13 15:08:20.206491 encord-0.1.82/encord/objects/frames.py
--rw-r--r--   0        0        0    21035 2023-06-13 15:08:20.206491 encord-0.1.82/encord/objects/internal_helpers.py
--rw-r--r--   0        0        0   142839 2023-06-13 15:08:20.206491 encord-0.1.82/encord/objects/ontology_labels_impl.py
--rw-r--r--   0        0        0      174 2023-06-13 15:08:20.206491 encord-0.1.82/encord/objects/ontology_object.py
--rw-r--r--   0        0        0      185 2023-06-13 15:08:20.206491 encord-0.1.82/encord/objects/ontology_structure.py
--rw-r--r--   0        0        0      549 2023-06-13 15:08:20.206491 encord-0.1.82/encord/objects/project.py
--rw-r--r--   0        0        0     1289 2023-06-13 15:08:20.206491 encord-0.1.82/encord/objects/utils.py
--rw-r--r--   0        0        0     3430 2023-06-13 15:08:20.206491 encord-0.1.82/encord/ontology.py
--rw-r--r--   0        0        0        0 2023-06-13 15:08:20.206491 encord-0.1.82/encord/orm/__init__.py
--rw-r--r--   0        0        0      982 2023-06-13 15:08:20.206491 encord-0.1.82/encord/orm/api_key.py
--rw-r--r--   0        0        0     5335 2023-06-13 15:08:20.206491 encord-0.1.82/encord/orm/base_orm.py
--rw-r--r--   0        0        0      111 2023-06-13 15:08:20.206491 encord-0.1.82/encord/orm/cloud_integration.py
--rw-r--r--   0        0        0    32800 2023-06-13 15:08:20.210491 encord-0.1.82/encord/orm/dataset.py
--rw-r--r--   0        0        0      828 2023-06-13 15:08:20.210491 encord-0.1.82/encord/orm/dataset_with_user_role.py
--rw-r--r--   0        0        0      175 2023-06-13 15:08:20.210491 encord-0.1.82/encord/orm/formatter.py
--rw-r--r--   0        0        0     1146 2023-06-13 15:08:20.210491 encord-0.1.82/encord/orm/label_log.py
--rw-r--r--   0        0        0    11869 2023-06-13 15:08:20.210491 encord-0.1.82/encord/orm/label_row.py
--rw-r--r--   0        0        0     1577 2023-06-13 15:08:20.210491 encord-0.1.82/encord/orm/labeling_algorithm.py
--rw-r--r--   0        0        0     6687 2023-06-13 15:08:20.210491 encord-0.1.82/encord/orm/model.py
--rw-r--r--   0        0        0      823 2023-06-13 15:08:20.210491 encord-0.1.82/encord/orm/ontology.py
--rw-r--r--   0        0        0     8885 2023-06-13 15:08:20.210491 encord-0.1.82/encord/orm/project.py
--rw-r--r--   0        0        0      625 2023-06-13 15:08:20.210491 encord-0.1.82/encord/orm/project_api_key.py
--rw-r--r--   0        0        0      828 2023-06-13 15:08:20.210491 encord-0.1.82/encord/orm/project_with_user_role.py
--rw-r--r--   0        0        0        0 2023-06-13 15:08:20.210491 encord-0.1.82/encord/orm/test/__init__.py
--rw-r--r--   0        0        0      570 2023-06-13 15:08:20.210491 encord-0.1.82/encord/orm/test/test_dataset.py
--rw-r--r--   0        0        0      314 2023-06-13 15:08:20.210491 encord-0.1.82/encord/orm/workflow.py
--rw-r--r--   0        0        0    39431 2023-06-13 15:08:20.210491 encord-0.1.82/encord/project.py
--rw-r--r--   0        0        0        0 2023-06-13 15:08:20.210491 encord-0.1.82/encord/project_ontology/__init__.py
--rw-r--r--   0        0        0     1316 2023-06-13 15:08:20.210491 encord-0.1.82/encord/project_ontology/classification_attribute.py
--rw-r--r--   0        0        0      525 2023-06-13 15:08:20.210491 encord-0.1.82/encord/project_ontology/classification_option.py
--rw-r--r--   0        0        0      357 2023-06-13 15:08:20.210491 encord-0.1.82/encord/project_ontology/classification_type.py
--rw-r--r--   0        0        0      237 2023-06-13 15:08:20.210491 encord-0.1.82/encord/project_ontology/object_type.py
--rw-r--r--   0        0        0     9676 2023-06-13 15:08:20.210491 encord-0.1.82/encord/project_ontology/ontology.py
--rw-r--r--   0        0        0      630 2023-06-13 15:08:20.210491 encord-0.1.82/encord/project_ontology/ontology_classification.py
--rw-r--r--   0        0        0      683 2023-06-13 15:08:20.210491 encord-0.1.82/encord/project_ontology/ontology_object.py
--rw-r--r--   0        0        0    28768 2023-06-13 15:08:20.210491 encord-0.1.82/encord/user_client.py
--rw-r--r--   0        0        0        0 2023-06-13 15:08:20.210491 encord-0.1.82/encord/utilities/__init__.py
--rw-r--r--   0        0        0     4282 2023-06-13 15:08:20.210491 encord-0.1.82/encord/utilities/client_utilities.py
--rw-r--r--   0        0        0      253 2023-06-13 15:08:20.210491 encord-0.1.82/encord/utilities/common.py
--rw-r--r--   0        0        0     3270 2023-06-13 15:08:20.210491 encord-0.1.82/encord/utilities/label_utilities.py
--rw-r--r--   0        0        0      343 2023-06-13 15:08:20.210491 encord-0.1.82/encord/utilities/ontology_user.py
--rw-r--r--   0        0        0      578 2023-06-13 15:08:20.210491 encord-0.1.82/encord/utilities/project_user.py
--rw-r--r--   0        0        0      467 2023-06-13 15:08:20.210491 encord-0.1.82/encord/utilities/project_utilities.py
--rw-r--r--   0        0        0     1945 2023-06-13 15:08:20.210491 encord-0.1.82/pyproject.toml
--rw-r--r--   0        0        0     3213 1970-01-01 00:00:00.000000 encord-0.1.82/PKG-INFO
+-rw-r--r--   0        0        0    11330 2023-06-20 14:01:34.440626 encord-0.1.83/LICENSE
+-rw-r--r--   0        0        0     2037 2023-06-20 14:01:34.440626 encord-0.1.83/README.md
+-rw-r--r--   0        0        0       84 2023-06-20 14:01:34.440626 encord-0.1.83/cord/__init__.py
+-rw-r--r--   0        0        0      158 2023-06-20 14:01:34.456626 encord-0.1.83/encord/__init__.py
+-rw-r--r--   0        0        0      214 2023-06-20 14:01:34.456626 encord-0.1.83/encord/_version.py
+-rw-r--r--   0        0        0    49810 2023-06-20 14:01:34.456626 encord-0.1.83/encord/client.py
+-rw-r--r--   0        0        0    10852 2023-06-20 14:01:34.456626 encord-0.1.83/encord/configs.py
+-rw-r--r--   0        0        0        0 2023-06-20 14:01:34.456626 encord-0.1.83/encord/constants/__init__.py
+-rw-r--r--   0        0        0      866 2023-06-20 14:01:34.456626 encord-0.1.83/encord/constants/enums.py
+-rw-r--r--   0        0        0     3293 2023-06-20 14:01:34.456626 encord-0.1.83/encord/constants/model.py
+-rw-r--r--   0        0        0     6068 2023-06-20 14:01:34.456626 encord-0.1.83/encord/constants/model_weights.py
+-rw-r--r--   0        0        0     1119 2023-06-20 14:01:34.456626 encord-0.1.83/encord/constants/string_constants.py
+-rw-r--r--   0        0        0        0 2023-06-20 14:01:34.456626 encord-0.1.83/encord/constants/test/__init__.py
+-rw-r--r--   0        0        0      634 2023-06-20 14:01:34.456626 encord-0.1.83/encord/constants/test/test_enums.py
+-rw-r--r--   0        0        0    16035 2023-06-20 14:01:34.456626 encord-0.1.83/encord/dataset.py
+-rw-r--r--   0        0        0     6346 2023-06-20 14:01:34.456626 encord-0.1.83/encord/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-20 14:01:34.456626 encord-0.1.83/encord/http/__init__.py
+-rw-r--r--   0        0        0     5315 2023-06-20 14:01:34.456626 encord-0.1.83/encord/http/bundle.py
+-rw-r--r--   0        0        0      535 2023-06-20 14:01:34.456626 encord-0.1.83/encord/http/constants.py
+-rw-r--r--   0        0        0     7234 2023-06-20 14:01:34.460626 encord-0.1.83/encord/http/error_utils.py
+-rw-r--r--   0        0        0      103 2023-06-20 14:01:34.460626 encord-0.1.83/encord/http/limits.py
+-rw-r--r--   0        0        0     7928 2023-06-20 14:01:34.460626 encord-0.1.83/encord/http/querier.py
+-rw-r--r--   0        0        0      697 2023-06-20 14:01:34.460626 encord-0.1.83/encord/http/query_methods.py
+-rw-r--r--   0        0        0     1719 2023-06-20 14:01:34.460626 encord-0.1.83/encord/http/request.py
+-rw-r--r--   0        0        0     6182 2023-06-20 14:01:34.460626 encord-0.1.83/encord/http/utils.py
+-rw-r--r--   0        0        0      340 2023-06-20 14:01:34.460626 encord-0.1.83/encord/objects/__init__.py
+-rw-r--r--   0        0        0     5164 2023-06-20 14:01:34.460626 encord-0.1.83/encord/objects/bitmask.py
+-rw-r--r--   0        0        0      182 2023-06-20 14:01:34.460626 encord-0.1.83/encord/objects/classification.py
+-rw-r--r--   0        0        0    31614 2023-06-20 14:01:34.460626 encord-0.1.83/encord/objects/common.py
+-rw-r--r--   0        0        0      151 2023-06-20 14:01:34.460626 encord-0.1.83/encord/objects/constants.py
+-rw-r--r--   0        0        0     5748 2023-06-20 14:01:34.460626 encord-0.1.83/encord/objects/coordinates.py
+-rw-r--r--   0        0        0     3461 2023-06-20 14:01:34.460626 encord-0.1.83/encord/objects/frames.py
+-rw-r--r--   0        0        0    21557 2023-06-20 14:01:34.460626 encord-0.1.83/encord/objects/internal_helpers.py
+-rw-r--r--   0        0        0   143304 2023-06-20 14:01:34.460626 encord-0.1.83/encord/objects/ontology_labels_impl.py
+-rw-r--r--   0        0        0      174 2023-06-20 14:01:34.460626 encord-0.1.83/encord/objects/ontology_object.py
+-rw-r--r--   0        0        0      185 2023-06-20 14:01:34.460626 encord-0.1.83/encord/objects/ontology_structure.py
+-rw-r--r--   0        0        0      549 2023-06-20 14:01:34.460626 encord-0.1.83/encord/objects/project.py
+-rw-r--r--   0        0        0     1289 2023-06-20 14:01:34.460626 encord-0.1.83/encord/objects/utils.py
+-rw-r--r--   0        0        0     3430 2023-06-20 14:01:34.460626 encord-0.1.83/encord/ontology.py
+-rw-r--r--   0        0        0        0 2023-06-20 14:01:34.460626 encord-0.1.83/encord/orm/__init__.py
+-rw-r--r--   0        0        0      982 2023-06-20 14:01:34.460626 encord-0.1.83/encord/orm/api_key.py
+-rw-r--r--   0        0        0     5335 2023-06-20 14:01:34.460626 encord-0.1.83/encord/orm/base_orm.py
+-rw-r--r--   0        0        0      111 2023-06-20 14:01:34.460626 encord-0.1.83/encord/orm/cloud_integration.py
+-rw-r--r--   0        0        0    32844 2023-06-20 14:01:34.460626 encord-0.1.83/encord/orm/dataset.py
+-rw-r--r--   0        0        0      828 2023-06-20 14:01:34.460626 encord-0.1.83/encord/orm/dataset_with_user_role.py
+-rw-r--r--   0        0        0      175 2023-06-20 14:01:34.460626 encord-0.1.83/encord/orm/formatter.py
+-rw-r--r--   0        0        0     1146 2023-06-20 14:01:34.460626 encord-0.1.83/encord/orm/label_log.py
+-rw-r--r--   0        0        0    11889 2023-06-20 14:01:34.460626 encord-0.1.83/encord/orm/label_row.py
+-rw-r--r--   0        0        0     1577 2023-06-20 14:01:34.460626 encord-0.1.83/encord/orm/labeling_algorithm.py
+-rw-r--r--   0        0        0     6687 2023-06-20 14:01:34.460626 encord-0.1.83/encord/orm/model.py
+-rw-r--r--   0        0        0      823 2023-06-20 14:01:34.460626 encord-0.1.83/encord/orm/ontology.py
+-rw-r--r--   0        0        0     8966 2023-06-20 14:01:34.460626 encord-0.1.83/encord/orm/project.py
+-rw-r--r--   0        0        0      625 2023-06-20 14:01:34.460626 encord-0.1.83/encord/orm/project_api_key.py
+-rw-r--r--   0        0        0      828 2023-06-20 14:01:34.460626 encord-0.1.83/encord/orm/project_with_user_role.py
+-rw-r--r--   0        0        0        0 2023-06-20 14:01:34.460626 encord-0.1.83/encord/orm/test/__init__.py
+-rw-r--r--   0        0        0      570 2023-06-20 14:01:34.460626 encord-0.1.83/encord/orm/test/test_dataset.py
+-rw-r--r--   0        0        0      314 2023-06-20 14:01:34.460626 encord-0.1.83/encord/orm/workflow.py
+-rw-r--r--   0        0        0    39504 2023-06-20 14:01:34.460626 encord-0.1.83/encord/project.py
+-rw-r--r--   0        0        0        0 2023-06-20 14:01:34.460626 encord-0.1.83/encord/project_ontology/__init__.py
+-rw-r--r--   0        0        0     1316 2023-06-20 14:01:34.460626 encord-0.1.83/encord/project_ontology/classification_attribute.py
+-rw-r--r--   0        0        0      525 2023-06-20 14:01:34.460626 encord-0.1.83/encord/project_ontology/classification_option.py
+-rw-r--r--   0        0        0      357 2023-06-20 14:01:34.460626 encord-0.1.83/encord/project_ontology/classification_type.py
+-rw-r--r--   0        0        0      237 2023-06-20 14:01:34.460626 encord-0.1.83/encord/project_ontology/object_type.py
+-rw-r--r--   0        0        0     9676 2023-06-20 14:01:34.460626 encord-0.1.83/encord/project_ontology/ontology.py
+-rw-r--r--   0        0        0      630 2023-06-20 14:01:34.460626 encord-0.1.83/encord/project_ontology/ontology_classification.py
+-rw-r--r--   0        0        0      683 2023-06-20 14:01:34.460626 encord-0.1.83/encord/project_ontology/ontology_object.py
+-rw-r--r--   0        0        0    29047 2023-06-20 14:01:34.460626 encord-0.1.83/encord/user_client.py
+-rw-r--r--   0        0        0        0 2023-06-20 14:01:34.460626 encord-0.1.83/encord/utilities/__init__.py
+-rw-r--r--   0        0        0     4282 2023-06-20 14:01:34.460626 encord-0.1.83/encord/utilities/client_utilities.py
+-rw-r--r--   0        0        0      253 2023-06-20 14:01:34.460626 encord-0.1.83/encord/utilities/common.py
+-rw-r--r--   0        0        0     3270 2023-06-20 14:01:34.460626 encord-0.1.83/encord/utilities/label_utilities.py
+-rw-r--r--   0        0        0      343 2023-06-20 14:01:34.460626 encord-0.1.83/encord/utilities/ontology_user.py
+-rw-r--r--   0        0        0      578 2023-06-20 14:01:34.460626 encord-0.1.83/encord/utilities/project_user.py
+-rw-r--r--   0        0        0      467 2023-06-20 14:01:34.460626 encord-0.1.83/encord/utilities/project_utilities.py
+-rw-r--r--   0        0        0     1945 2023-06-20 14:01:34.460626 encord-0.1.83/pyproject.toml
+-rw-r--r--   0        0        0     3213 1970-01-01 00:00:00.000000 encord-0.1.83/PKG-INFO
```

### Comparing `encord-0.1.82/LICENSE` & `encord-0.1.83/LICENSE`

 * *Files identical despite different names*

### Comparing `encord-0.1.82/README.md` & `encord-0.1.83/README.md`

 * *Files identical despite different names*

### Comparing `encord-0.1.82/encord/client.py` & `encord-0.1.83/encord/client.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.82/encord/configs.py` & `encord-0.1.83/encord/configs.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
             UserConfig.
 
         Raises:
             ValueError: If the provided key content is not of the correct format.
 
         """
         key_bytes = ssh_private_key.encode()
-        password_bytes = password and password.encode()
+        password_bytes = password.encode() if password else None
         private_key = cryptography.hazmat.primitives.serialization.load_ssh_private_key(key_bytes, password_bytes)
 
         if isinstance(private_key, Ed25519PrivateKey):
             return UserConfig(private_key, requests_settings=requests_settings, **kwargs)
         else:
             raise ValueError(f"Provided key [{ssh_private_key}] is not an Ed25519 private key")
```

### Comparing `encord-0.1.82/encord/constants/model.py` & `encord-0.1.83/encord/constants/model.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.82/encord/constants/model_weights.py` & `encord-0.1.83/encord/constants/model_weights.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.82/encord/constants/string_constants.py` & `encord-0.1.83/encord/constants/string_constants.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.82/encord/constants/test/test_enums.py` & `encord-0.1.83/encord/constants/test/test_enums.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.82/encord/dataset.py` & `encord-0.1.83/encord/dataset.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.82/encord/exceptions.py` & `encord-0.1.83/encord/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from dataclasses import dataclass, field, fields
 from datetime import datetime, timezone
 from typing import Optional
 
 
 @dataclass
 class ExceptionContext:
-    timestamp: datetime = field(default_factory=lambda: datetime.now(tz=timezone.utc).isoformat())
+    timestamp: str = field(default_factory=lambda: datetime.now(tz=timezone.utc).isoformat())
 
     def __str__(self):
         return " ".join(
             f"{object_field.name}={getattr(self, object_field.name)!r}"
             for object_field in fields(self)
             if getattr(self, object_field.name) is not None
         )
```

### Comparing `encord-0.1.82/encord/http/bundle.py` & `encord-0.1.83/encord/http/bundle.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.82/encord/http/constants.py` & `encord-0.1.83/encord/http/constants.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.82/encord/http/error_utils.py` & `encord-0.1.83/encord/http/error_utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.82/encord/http/querier.py` & `encord-0.1.83/encord/http/querier.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.82/encord/http/query_methods.py` & `encord-0.1.83/encord/http/query_methods.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.82/encord/http/request.py` & `encord-0.1.83/encord/http/request.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.82/encord/http/utils.py` & `encord-0.1.83/encord/http/utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.82/encord/objects/bitmask.py` & `encord-0.1.83/encord/objects/bitmask.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.82/encord/objects/common.py` & `encord-0.1.83/encord/objects/common.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.82/encord/objects/coordinates.py` & `encord-0.1.83/encord/objects/coordinates.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.82/encord/objects/frames.py` & `encord-0.1.83/encord/objects/frames.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.82/encord/objects/internal_helpers.py` & `encord-0.1.83/encord/objects/internal_helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,25 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from copy import deepcopy
 from dataclasses import dataclass
-from typing import Any, Dict, Iterable, List, NoReturn, Optional, Sequence, Set, Union
+from typing import (
+    Any,
+    Dict,
+    Generic,
+    Iterable,
+    List,
+    NoReturn,
+    Optional,
+    Sequence,
+    Set,
+    TypeVar,
+    Union,
+)
 
 from encord.exceptions import LabelRowError
 from encord.objects.common import (
     Attribute,
     ChecklistAttribute,
     FlatOption,
     NestableOption,
@@ -16,33 +28,38 @@
     TextAttribute,
     _get_option_by_hash,
 )
 from encord.objects.constants import DEFAULT_MANUAL_ANNOTATION
 from encord.objects.frames import Ranges, ranges_to_list
 from encord.objects.utils import _lower_snake_case, short_uuid_str
 
+ValueType = TypeVar("ValueType")
+AttributeType = TypeVar("AttributeType", bound=Attribute)
+
 
-class Answer(ABC):
+class Answer(ABC, Generic[ValueType, AttributeType]):
     """An internal helper class for the LabelRowV2 class. This class is not meant to be used directly by users."""
 
-    _ontology_attribute: Attribute
+    _ontology_attribute: AttributeType
+    _value: Optional[ValueType]
 
-    def __init__(self, ontology_attribute: Attribute, track_hash: Optional[str] = None):
+    def __init__(self, ontology_attribute: AttributeType, track_hash: Optional[str] = None):
         self._answered = False
         self._ontology_attribute = ontology_attribute
         self._track_hash = track_hash or short_uuid_str()
         self._is_manual_annotation = DEFAULT_MANUAL_ANNOTATION
         self._should_propagate = False
 
     def is_answered(self) -> bool:
         return self._answered
 
     def unset(self) -> None:
         """Remove the value from the answer"""
         self._answered = False
+        self._value = None
 
     @property
     def is_dynamic(self) -> bool:
         return self._ontology_attribute.dynamic
 
     @is_dynamic.setter
     def is_dynamic(self, value: bool) -> NoReturn:
@@ -53,31 +70,45 @@
         return self._is_manual_annotation
 
     @is_manual_annotation.setter
     def is_manual_annotation(self, value: bool) -> None:
         self._is_manual_annotation = value
 
     @property
-    def ontology_attribute(self):
+    def ontology_attribute(self) -> AttributeType:
         return deepcopy(self._ontology_attribute)
 
     @ontology_attribute.setter
     def ontology_attribute(self, v: Any) -> NoReturn:
         raise RuntimeError("Cannot reset the ontology attribute of an instantiated answer.")
 
+    @abstractmethod
+    def set(self, value: ValueType) -> None:
+        pass
+
+    def get(self) -> ValueType:
+        if not self.is_answered():
+            raise ValueError("Can't read a value of unanswered Answer object")
+
+        assert self._value is not None, "Value can't be none for the answered Answer object"
+        return self._value
+
     def to_encord_dict(self, ranges: Optional[Ranges] = None) -> Optional[Dict[str, Any]]:
         """
         A low level helper to convert to the Encord JSON format.
         For most use cases the `get_answer` function should be used instead.
         """
         if not self.is_answered():
             return None
 
         ret = self._to_encord_dict_impl(self.is_dynamic)
         if self.is_dynamic:
+            if ranges is None:
+                raise ValueError("Frame range should be set for dynamic answers")
+
             ret.update(self._get_encord_dynamic_fields(ranges))
 
         return ret
 
     @abstractmethod
     def _to_encord_dict_impl(self, is_dynamic: bool = False) -> Dict[str, Any]:
         pass
@@ -91,26 +122,25 @@
             "dynamic": True,
             "range": ranges_to_list(ranges),
             "shouldPropagate": self._should_propagate,
             "trackHash": self._track_hash,
         }
 
 
-class TextAnswer(Answer):
+class TextAnswer(Answer[str, TextAttribute]):
     def __init__(self, ontology_attribute: TextAttribute):
         super().__init__(ontology_attribute)
         self._value: Optional[str] = None
 
-    def set(self, value: str) -> TextAnswer:
+    def set(self, value: str) -> None:
         """Returns the object itself"""
         if not isinstance(value, str):
             raise ValueError("TextAnswer can only be set to a string.")
         self._value = value
         self._answered = True
-        return self
 
     def get_value(self) -> Optional[str]:
         if not self.is_answered():
             return None
         else:
             return self._value
 
@@ -119,15 +149,15 @@
             raise ValueError(
                 "Copying from a TextAnswer which is based on a different ontology Attribute is not possible."
             )
         other_is_answered = text_answer.is_answered()
         if not other_is_answered:
             self.unset()
         else:
-            other_answer = text_answer.get_value()
+            other_answer = text_answer.get()
             self.set(other_answer)
 
     def _to_encord_dict_impl(self, is_dynamic: bool = False) -> Dict[str, Any]:
         return {
             "name": self.ontology_attribute.name,
             "value": _lower_snake_case(self.ontology_attribute.name),
             "answers": self._value,
@@ -135,15 +165,14 @@
             "manualAnnotation": self.is_manual_annotation,
         }
 
     def from_dict(self, d: Dict[str, Any]) -> None:
         if d["featureHash"] != self.ontology_attribute.feature_node_hash:
             raise ValueError("Cannot set the value of a TextAnswer based on a different ontology attribute.")
 
-        self._answered = True
         self.set(d["answers"])
         self.is_manual_annotation = d["manualAnnotation"]
 
     def __hash__(self):
         return hash((self._ontology_attribute.feature_node_hash, self._value, type(self).__name__))
 
     def __eq__(self, other: object) -> bool:
@@ -156,15 +185,15 @@
         )
 
     def __repr__(self):
         return f"{self.__class__.__name__}({self._value})"
 
 
 @dataclass
-class RadioAnswer(Answer):
+class RadioAnswer(Answer[NestableOption, RadioAttribute]):
     def __init__(self, ontology_attribute: RadioAttribute):
         super().__init__(ontology_attribute)
         self._value: Optional[NestableOption] = None
 
     def set(self, value: NestableOption):
         if not isinstance(value, NestableOption):
             raise ValueError("RadioAnswer can only be set to a NestableOption.")
@@ -192,19 +221,20 @@
             raise ValueError(
                 "Copying from a RadioAnswer which is based on a different ontology Attribute is not possible."
             )
         other_is_answered = radio_answer.is_answered()
         if not other_is_answered:
             self.unset()
         else:
-            other_answer = radio_answer.get_value()
+            other_answer = radio_answer.get()
             self.set(other_answer)
 
     def _to_encord_dict_impl(self, is_dynamic: bool = False) -> Dict[str, Any]:
         nestable_option = self._value
+        assert nestable_option is not None  # Check is performed earlier, so just to silence mypy
 
         return {
             "name": self.ontology_attribute.name,
             "value": _lower_snake_case(self.ontology_attribute.name),
             "answers": [
                 {
                     "name": nestable_option.label,
@@ -216,15 +246,14 @@
             "manualAnnotation": self.is_manual_annotation,
         }
 
     def from_dict(self, d: Dict) -> None:
         if d["featureHash"] != self.ontology_attribute.feature_node_hash:
             raise ValueError("Cannot set the value of a TextAnswer based on a different ontology attribute.")
 
-        self._answered = True
         answers = d["answers"]
         if len(answers) != 1:
             raise ValueError("RadioAnswers must have exactly one answer.")
 
         answer = answers[0]
         nestable_option = _get_option_by_hash(answer["featureHash"], self.ontology_attribute.options)
         self.set(nestable_option)
@@ -243,15 +272,15 @@
         )
 
     def __repr__(self):
         return f"{self.__class__.__name__}({self._value})"
 
 
 @dataclass
-class ChecklistAnswer(Answer):
+class ChecklistAnswer(Answer[List[FlatOption], ChecklistAttribute]):
     """
     Checkboxes behave slightly different from the other answer types. When the checkbox is unanswered, it will be
     the equivalent of not having selected any checkbox answer in the Encord platform.
     The initial state will be every checkbox unchecked.
     """
 
     def __init__(self, ontology_attribute: ChecklistAttribute):
@@ -267,52 +296,72 @@
 
     def uncheck_options(self, values: Iterable[FlatOption]):
         self._answered = True
         for value in values:
             self._verify_flat_option(value)
             self._feature_hash_to_answer_map[value.feature_node_hash] = False
 
-    def set_options(self, values: Iterable[FlatOption]):
+    def get(self) -> List[FlatOption]:
+        if not self.is_answered():
+            raise ValueError("Can't read a value of unanswered Answer object")
+
+        return [
+            option
+            for option in self._ontology_attribute.options
+            if self._feature_hash_to_answer_map[option.feature_node_hash]
+        ]
+
+    def set(self, values: Iterable[FlatOption]):
         for value in values:
             if not isinstance(value, FlatOption):
                 raise ValueError("ChecklistAnswer can only be set to FlatOptions.")
 
         self._answered = True
         for key in self._feature_hash_to_answer_map.keys():
             self._feature_hash_to_answer_map[key] = False
         for value in values:
             self._verify_flat_option(value)
             self._feature_hash_to_answer_map[value.feature_node_hash] = True
 
+    def set_options(self, values: Iterable[FlatOption]):
+        # Deprecated: please use :meth:`set` instead
+        return self.set(values)
+
     def get_options(self) -> List[FlatOption]:
+        # Deprecated: please use :meth:`get()` instead
+
         if not self.is_answered():
             return []
         else:
             return [
                 option
                 for option in self._ontology_attribute.options
                 if self._feature_hash_to_answer_map[option.feature_node_hash]
             ]
 
     def get_value(self, value: FlatOption) -> bool:
+        # Deprecated: please use :meth:`get_option_value` instead
+        return self.get_option_value(value)
+
+    def get_option_value(self, value: FlatOption) -> bool:
         return self._feature_hash_to_answer_map[value.feature_node_hash]
 
     def copy_from(self, checklist_answer: ChecklistAnswer):
         if checklist_answer.ontology_attribute.feature_node_hash != self.ontology_attribute.feature_node_hash:
             raise ValueError(
                 "Copying from a ChecklistAnswer which is based on a different ontology Attribute is not possible."
             )
         other_is_answered = checklist_answer.is_answered()
         if not other_is_answered:
             self.unset()
         else:
             self._answered = True
             for feature_node_hash in self._feature_hash_to_answer_map.keys():
                 option = _get_option_by_hash(feature_node_hash, self.ontology_attribute.options)
-                other_answer = checklist_answer.get_value(option)
+                other_answer = checklist_answer.get_option_value(option)
                 self._feature_hash_to_answer_map[feature_node_hash] = other_answer
 
     def _initialise_feature_hash_to_answer_map(self) -> Dict[str, bool]:
         ret: Dict[str, bool] = {}
         for child in self._ontology_attribute.options:
             ret[child.feature_node_hash] = False
         return ret
@@ -394,38 +443,14 @@
         return RadioAnswer(attribute)
     elif isinstance(attribute, ChecklistAttribute):
         return ChecklistAnswer(attribute)
     else:
         raise RuntimeError(f"Got an attribute with an unexpected property type: {attribute}")
 
 
-def set_answer_for_object(answer_object: Answer, answer_value: Union[str, Option, Iterable[Option]]) -> None:
-    attribute = answer_object.ontology_attribute
-    if isinstance(attribute, TextAttribute):
-        answer_object.set(answer_value)
-    elif isinstance(attribute, RadioAttribute):
-        answer_object.set(answer_value)
-    elif isinstance(attribute, ChecklistAttribute):
-        answer_object.set_options(answer_value)
-    else:
-        raise ValueError(f"Unknown attribute type: {type(attribute)}")
-
-
-def get_answer_from_object(answer_object: Answer) -> Union[str, Option, Iterable[Option], None]:
-    attribute = answer_object.ontology_attribute
-    if isinstance(attribute, TextAttribute):
-        return answer_object.get_value()
-    elif isinstance(attribute, RadioAttribute):
-        return answer_object.get_value()
-    elif isinstance(attribute, ChecklistAttribute):
-        return answer_object.get_options()
-    else:
-        raise ValueError(f"Unknown attribute type: {type(attribute)}")
-
-
 def _get_default_static_answers_from_attributes(attributes: List[Attribute]) -> List[Answer]:
     ret: List[Answer] = list()
     for attribute in attributes:
         if not attribute.dynamic:
             answer = get_default_answer_from_attribute(attribute)
             ret.append(answer)
 
@@ -449,18 +474,18 @@
     if passed_attribute == search_attribute:
         return True
 
     if not isinstance(search_attribute, RadioAttribute):
         return False
 
     answer = static_answer_map[search_attribute.feature_node_hash]
-    value = answer.get_value()
-    if value is None:
+    if not answer.is_answered():
         return False
 
+    value = answer.get()
     for option in search_attribute.options:
         if value == option:
             for nested_option in option.nested_options:
                 # If I have multi nesting here, what then?
                 if _search_child_attributes(passed_attribute, nested_option, static_answer_map):
                     return True
```

### Comparing `encord-0.1.82/encord/objects/ontology_labels_impl.py` & `encord-0.1.83/encord/objects/ontology_labels_impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,20 +76,19 @@
     Ranges,
     frames_class_to_frames_list,
     frames_to_ranges,
     ranges_list_to_ranges,
 )
 from encord.objects.internal_helpers import (
     Answer,
+    ValueType,
     _get_static_answer_map,
     _infer_attribute_from_answer,
     _search_child_attributes,
-    get_answer_from_object,
     get_default_answer_from_attribute,
-    set_answer_for_object,
 )
 from encord.objects.utils import (
     _lower_snake_case,
     check_email,
     check_type,
     does_type_match,
     filter_by_type,
@@ -485,14 +484,15 @@
                 manual_annotation=manual_annotation,
                 last_edited_at=last_edited_at,
                 last_edited_by=last_edited_by,
                 reviews=reviews,
             )
 
         if self.is_assigned_to_label_row():
+            assert self._parent is not None
             self._parent._add_frames_to_classification(self.ontology_item, frames_list)
             self._parent._add_to_frame_to_hashes_map(self)
 
     def get_annotation(self, frame: Union[int, str] = 0) -> Annotation:
         """
         Args:
             frame: Either the frame number or the image hash if the data type is an image or image group.
@@ -504,14 +504,15 @@
 
     def remove_from_frames(self, frames: Frames) -> None:
         frame_list = frames_class_to_frames_list(frames)
         for frame in frame_list:
             self._frames_to_data.pop(frame)
 
         if self.is_assigned_to_label_row():
+            assert self._parent is not None
             self._parent._remove_frames_from_classification(self.ontology_item, frame_list)
             self._parent._remove_from_frame_to_hashes_map(frame_list, self.classification_hash)
 
     def get_annotations(self) -> List[Annotation]:
         """
         Returns:
             A list of `ClassificationInstance.Annotation` in order of available frames.
@@ -558,15 +559,15 @@
         static_answer = self._static_answer_map[attribute.feature_node_hash]
         if static_answer.is_answered() and overwrite is False:
             raise LabelRowError(
                 "The answer to this attribute was already set. Set `overwrite` to `True` if you want to"
                 "overwrite an existing answer to and attribute."
             )
 
-        set_answer_for_object(static_answer, answer)
+        static_answer.set(answer)
 
     def set_answer_from_list(self, answers_list: List[Dict[str, Any]]) -> None:
         """
         This is a low level helper function and should not be used directly.
 
         Sets the answer for the classification from a dictionary.
 
@@ -586,17 +587,21 @@
                     "One of the attributes set for a classification is not a valid child of the classification. "
                     "Cannot create a valid LabelRow."
                 )
 
             if isinstance(attribute, TextAttribute):
                 self._set_answer_unsafe(answer_dict["answers"], attribute)
             elif isinstance(attribute, RadioAttribute):
-                feature_hash = answer_dict["answers"][0]["featureHash"]
-                option = _get_option_by_hash(feature_hash, attribute.options)
-                self._set_answer_unsafe(option, attribute)
+                if len(answer_dict["answers"]) == 1:
+                    # When classification is removed in UI, it keeps the entry about the classification,
+                    # but removes the answers.
+                    # Thus an empty answers array is equivalent to "no such attribute", and such attribute should be ignored
+                    feature_hash = answer_dict["answers"][0]["featureHash"]
+                    option = _get_option_by_hash(feature_hash, attribute.options)
+                    self._set_answer_unsafe(option, attribute)
             elif isinstance(attribute, ChecklistAttribute):
                 options = []
                 for answer in answer_dict["answers"]:
                     feature_hash = answer["featureHash"]
                     option = _get_option_by_hash(feature_hash, attribute.options)
                     options.append(option)
                 self._set_answer_unsafe(options, attribute)
@@ -618,16 +623,18 @@
             attribute = self._ontology_classification.attributes[0]
         elif not self._is_attribute_valid_child_of_classification(attribute):
             raise LabelRowError("The attribute is not a valid child of the classification.")
         elif not self._is_selectable_child_attribute(attribute):
             return None
 
         static_answer = self._static_answer_map[attribute.feature_node_hash]
+        if not static_answer.is_answered():
+            return None
 
-        return get_answer_from_object(static_answer)
+        return static_answer.get()
 
     def delete_answer(self, attribute: Optional[Attribute] = None) -> None:
         """
         This resets the answer of an attribute as if it was never set.
 
         Args:
             attribute: The ontology attribute to delete the answer for. If not provided, the first level attribute is
@@ -831,19 +838,19 @@
             self._frames_to_data[frame] = existing_frame_data
 
         existing_frame_data.update_from_optional_fields(
             created_at, created_by, confidence, manual_annotation, last_edited_at, last_edited_by, reviews
         )
 
         if self.is_assigned_to_label_row():
+            assert self._parent is not None
             self._parent.add_to_single_frame_to_hashes_map(self, frame)
 
-    def _set_answer_unsafe(self, answer: Union[str, Option, Iterable[Option]], attribute: Attribute) -> None:
-        static_answer = self._static_answer_map[attribute.feature_node_hash]
-        set_answer_for_object(static_answer, answer)
+    def _set_answer_unsafe(self, answer: ValueType, attribute: Attribute) -> None:
+        self._static_answer_map[attribute.feature_node_hash].set(answer)
 
     def _is_attribute_valid_child_of_classification(self, attribute: Attribute) -> bool:
         return attribute.feature_node_hash in self._static_answer_map
 
     def _is_selectable_child_attribute(self, attribute: Attribute) -> bool:
         # I have the ontology classification, so I can build the tree from that. Basically do a DFS.
         ontology_classification = self._ontology_classification
@@ -2349,15 +2356,20 @@
             )
 
         if attribute.dynamic:
             return self._dynamic_answer_manager.get_answer(attribute, filter_answer, filter_frame)
 
         static_answer = self._static_answer_map[attribute.feature_node_hash]
 
-        return get_answer_from_object(static_answer)
+        if not static_answer.is_answered():
+            if isinstance(attribute, ChecklistAttribute):
+                return []
+            return None
+
+        return static_answer.get()
 
     def set_answer(
         self,
         answer: Union[str, Option, Sequence[Option]],
         attribute: Optional[Attribute] = None,
         frames: Optional[Frames] = None,
         overwrite: bool = False,
@@ -2402,15 +2414,15 @@
         static_answer = self._static_answer_map[attribute.feature_node_hash]
         if static_answer.is_answered() and overwrite is False:
             raise LabelRowError(
                 "The answer to this attribute was already set. Set `overwrite` to `True` if you want to"
                 "overwrite an existing answer to an attribute."
             )
 
-        set_answer_for_object(static_answer, answer)
+        static_answer.set(answer)
 
     def set_answer_from_list(self, answers_list: List[Dict[str, Any]]) -> None:
         """
         This is a low level helper function and should usually not be used directly.
 
         Sets the answer for the classification from a dictionary.
 
@@ -2431,15 +2443,15 @@
                 )
 
             self._set_answer_from_dict(answer_dict, attribute)
 
     def delete_answer(
         self,
         attribute: Attribute,
-        filter_answer: Union[str, Option, Iterable[Option]] = None,
+        filter_answer: Optional[Union[str, Option, Iterable[Option]]] = None,
         filter_frame: Optional[int] = None,
     ) -> None:
         """
         This resets the answer of an attribute as if it was never set.
 
         Args:
             attribute: The attribute to delete the answer for.
@@ -2792,15 +2804,15 @@
         self, answer: Union[str, Option, Iterable[Option]], attribute: Attribute, track_hash: str, ranges: Ranges
     ) -> None:
         if attribute.dynamic:
             self._dynamic_answer_manager.set_answer(answer, attribute, frames=ranges)
 
         else:
             static_answer = self._static_answer_map[attribute.feature_node_hash]
-            set_answer_for_object(static_answer, answer)
+            static_answer.set(answer)
 
     def _set_answer_from_dict(self, answer_dict: Dict[str, Any], attribute: Attribute) -> None:
         if attribute.dynamic:
             track_hash = answer_dict["trackHash"]
             ranges = ranges_list_to_ranges(answer_dict["range"])
         else:
             track_hash = None
@@ -2897,16 +2909,15 @@
             frames = [Range(i, i) for i in self._frames_to_answers.keys()]
         frame_list = frames_class_to_frames_list(frames)
 
         for frame in frame_list:
             to_remove_answer = None
             for answer_object in self._frames_to_answers[frame]:
                 if filter_answer is not None:
-                    answer_value = get_answer_from_object(answer_object)
-                    if answer_value != filter_answer:
+                    if answer_object.is_answered() and answer_object.get() != filter_answer:
                         continue
 
                 # ideally this would not be a log(n) operation, however these will not be extremely large.
                 if answer_object.ontology_attribute == attribute:
                     to_remove_answer = answer_object
                     break
 
@@ -2931,15 +2942,15 @@
         frame_list = frames_class_to_frames_list(frames)
         for frame in frame_list:
             self._object_instance.check_within_range(frame)
 
         self.delete_answer(attribute, frames)
 
         default_answer = get_default_answer_from_attribute(attribute)
-        set_answer_for_object(default_answer, answer)
+        default_answer.set(answer)
 
         frame_list = frames_class_to_frames_list(frames)
         for frame in frame_list:
             self._frames_to_answers[frame].add(default_answer)
             self._answers_to_frames[default_answer].add(frame)
 
     def get_answer(
@@ -2950,22 +2961,24 @@
     ) -> AnswersForFrames:
         """For a given attribute, return all the answers and frames given the filters."""
         ret = []
         filter_frames_set = None if filter_frames is None else set(frames_class_to_frames_list(filter_frames))
         for answer in self._answers_to_frames:
             if answer.ontology_attribute != attribute:
                 continue
-            if not (filter_answer is None or filter_answer == get_answer_from_object(answer)):
+            if not answer.is_answered():
+                continue
+            if not (filter_answer is None or filter_answer == answer.get()):
                 continue
             actual_frames = self._answers_to_frames[answer]
             if not (filter_frames_set is None or len(actual_frames & filter_frames_set) > 0):
                 continue
 
             ranges = frames_to_ranges(self._answers_to_frames[answer])
-            ret.append(AnswerForFrames(answer=get_answer_from_object(answer), ranges=ranges))
+            ret.append(AnswerForFrames(answer=answer.get(), ranges=ranges))
         return ret
 
     def frames(self) -> Iterable[int]:
         """Returns all frames that have answers set."""
         return self._frames_to_answers.keys()
 
     def get_all_answers(self) -> List[Tuple[Answer, Ranges]]:
```

### Comparing `encord-0.1.82/encord/objects/project.py` & `encord-0.1.83/encord/objects/project.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.82/encord/objects/utils.py` & `encord-0.1.83/encord/objects/utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.82/encord/ontology.py` & `encord-0.1.83/encord/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.82/encord/orm/api_key.py` & `encord-0.1.83/encord/orm/api_key.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.82/encord/orm/base_orm.py` & `encord-0.1.83/encord/orm/base_orm.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.82/encord/orm/dataset.py` & `encord-0.1.83/encord/orm/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 
 import dataclasses
 import json
 from collections import OrderedDict
 from datetime import datetime
 from enum import Enum, IntEnum
-from typing import Dict, List, Optional
+from typing import Any, Dict, List, Optional
 from uuid import UUID
 
 from dateutil import parser
 
 from encord.constants.enums import DataType
 from encord.exceptions import EncordException
 from encord.orm import base_orm
@@ -763,15 +763,16 @@
         elif self == StorageLocation.GCP:
             return "GCP_STR"
         elif self == StorageLocation.AZURE:
             return "AZURE_STR"
         elif self == StorageLocation.OTC:
             return "OTC_STR"
 
-    def _missing_(cls) -> StorageLocation:
+    @classmethod
+    def _missing_(cls, value: Any) -> StorageLocation:
         return StorageLocation.NEW_STORAGE
 
 
 STORAGE_LOCATION_BY_STR: Dict[str, StorageLocation] = {location.get_str(): location for location in StorageLocation}
 
 DatasetType = StorageLocation
 """For backwards compatibility"""
@@ -913,15 +914,15 @@
 
 
 @dataclasses.dataclass(frozen=True)
 class ReEncodeVideoTask(Formatter):
     """A re encode video object with supporting information."""
 
     status: str
-    result: List[ReEncodeVideoTaskResult] = None
+    result: Optional[List[ReEncodeVideoTaskResult]] = None
 
     @classmethod
     def from_dict(cls, json_dict: Dict):
         if "result" in json_dict:
             dict_results = json_dict["result"]
             results = [
                 ReEncodeVideoTaskResult(result["data_hash"], result.get("signed_url"), result["bucket_path"])
```

### Comparing `encord-0.1.82/encord/orm/dataset_with_user_role.py` & `encord-0.1.83/encord/orm/dataset_with_user_role.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.82/encord/orm/label_log.py` & `encord-0.1.83/encord/orm/label_log.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.82/encord/orm/label_row.py` & `encord-0.1.83/encord/orm/label_row.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,15 +227,15 @@
     MISSING_LABEL_STATUS = "_MISSING_LABEL_STATUS_"
     """
     This value will be displayed if the Encord platform has a new label status and your SDK version does not understand
     it yet. Please update your SDK to the latest version.
     """
 
     @classmethod
-    def _missing_(cls, value):
+    def _missing_(cls, value: Any) -> LabelStatus:
         return cls.MISSING_LABEL_STATUS
 
 
 @dataclass(frozen=True)
 class WorkflowGraphNode:
     uuid: str
     title: str
```

### Comparing `encord-0.1.82/encord/orm/labeling_algorithm.py` & `encord-0.1.83/encord/orm/labeling_algorithm.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.82/encord/orm/model.py` & `encord-0.1.83/encord/orm/model.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.82/encord/orm/ontology.py` & `encord-0.1.83/encord/orm/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.82/encord/orm/project.py` & `encord-0.1.83/encord/orm/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
+from __future__ import annotations
+
 import datetime
 from collections import OrderedDict
 from dataclasses import dataclass, field
 from enum import Enum
 from typing import Dict, List, Optional, Union
 
 from encord.orm import base_orm
@@ -255,18 +257,21 @@
 
 
 class StringEnum(Enum):
     """
     Use this enum class if you need the helper that creates the enum instance from a string.
     """
 
+    def __str__(self):
+        return self.name
+
     @classmethod
-    def from_string(cls, string: str) -> Optional["StringEnum"]:
+    def from_string(cls, value: str) -> Optional[StringEnum]:
         # pylint: disable-next=no-member
-        return cls._value2member_map_.get(string)
+        return cls._value2member_map_.get(value)
 
 
 class ReviewMode(StringEnum):
     """
     UNLABELLED:
         The labels are added to the images. However, the one person must still go over
             all of the labels before submitting them for review.
```

### Comparing `encord-0.1.82/encord/orm/project_api_key.py` & `encord-0.1.83/encord/orm/project_api_key.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.82/encord/orm/project_with_user_role.py` & `encord-0.1.83/encord/orm/project_with_user_role.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.82/encord/orm/test/test_dataset.py` & `encord-0.1.83/encord/orm/test/test_dataset.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.82/encord/project.py` & `encord-0.1.83/encord/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -676,15 +676,19 @@
         """
         return self._client.get_data(data_hash, get_signed_url)
 
     def get_websocket_url(self) -> str:
         return self._client.get_websocket_url()
 
     def get_label_logs(
-        self, user_hash: str = None, data_hash: str = None, from_unix_seconds: int = None, to_unix_seconds: int = None
+        self,
+        user_hash: Optional[str] = None,
+        data_hash: Optional[str] = None,
+        from_unix_seconds: Optional[int] = None,
+        to_unix_seconds: Optional[int] = None,
     ) -> List[LabelLog]:
         """
         Get label logs, which represent the actions taken in the UI to create labels.
 
         All arguments can be left as `None` if no filtering should be applied.
 
         Args:
```

### Comparing `encord-0.1.82/encord/project_ontology/classification_attribute.py` & `encord-0.1.83/encord/project_ontology/classification_attribute.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.82/encord/project_ontology/classification_option.py` & `encord-0.1.83/encord/project_ontology/classification_option.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.82/encord/project_ontology/ontology.py` & `encord-0.1.83/encord/project_ontology/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.82/encord/project_ontology/ontology_classification.py` & `encord-0.1.83/encord/project_ontology/ontology_classification.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.82/encord/project_ontology/ontology_object.py` & `encord-0.1.83/encord/project_ontology/ontology_object.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.82/encord/user_client.py` & `encord-0.1.83/encord/user_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -292,25 +292,26 @@
     def create_project(
         self,
         project_title: str,
         dataset_hashes: List[str],
         project_description: str = "",
         ontology_hash: str = "",
         workflow_settings: ProjectWorkflowSettings = ManualReviewWorkflowSettings(),
+        workflow_template_hash: Optional[str] = None,
     ) -> str:
         """
         Creates a new project and returns its uid ('project_hash')
 
         Args:
             project_title: the title of the project
             dataset_hashes: a list of the dataset uids that the project will use
             project_description: the optional description of the project
             ontology_hash: the uid of an ontology to be used. If omitted, a new empty ontology will be created
             workflow_settings: selects and configures the type of the quality control workflow to use, See :class:`encord.orm.project.ProjectWorkflowSettings` for details. If omitted, :class:`~encord.orm.project.ManualReviewWorkflowSettings` is used.
-
+            workflow_template_hash: project will be created using a workflow based on the template provided.
         Returns:
             the uid of the project.
         """
         project = {
             "title": project_title,
             "description": project_description,
             "dataset_hashes": dataset_hashes,
@@ -318,14 +319,17 @@
         }
         if isinstance(workflow_settings, BenchmarkQaWorkflowSettings):
             project["workflow_type"] = ProjectWorkflowType.BENCHMARK_QA.value
             project["source_projects"] = workflow_settings.source_projects
         if ontology_hash and len(ontology_hash):
             project["ontology_hash"] = ontology_hash
 
+        if workflow_template_hash is not None:
+            project["workflow_template_id"] = workflow_template_hash
+
         return self.querier.basic_setter(OrmProject, uid=None, payload=project)
 
     def create_project_api_key(self, project_hash: str, api_key_title: str, scopes: List[APIKeyScopes]) -> str:
         """
         Returns:
             The created project API key.
         """
```

### Comparing `encord-0.1.82/encord/utilities/client_utilities.py` & `encord-0.1.83/encord/utilities/client_utilities.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.82/encord/utilities/label_utilities.py` & `encord-0.1.83/encord/utilities/label_utilities.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.82/encord/utilities/project_user.py` & `encord-0.1.83/encord/utilities/project_user.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.82/pyproject.toml` & `encord-0.1.83/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "encord"
-version = "0.1.82"
+version = "0.1.83"
 description = "Encord Python SDK Client"
 authors = ["Cord Technologies Limited <hello@encord.com>"]
 license = "Apache Software License"
 keywords = ["cord", "encord"]
 packages = [
     { include = "cord"},
     { include = "encord"},
```

### Comparing `encord-0.1.82/PKG-INFO` & `encord-0.1.83/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encord
-Version: 0.1.82
+Version: 0.1.83
 Summary: Encord Python SDK Client
 Home-page: https://github.com/encord-team/encord-client-python
 License: Apache Software License
 Keywords: cord,encord
 Author: Cord Technologies Limited
 Author-email: hello@encord.com
 Requires-Python: >=3.7,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: encord Version: 0.1.82 Summary: Encord Python SDK
+Metadata-Version: 2.1 Name: encord Version: 0.1.83 Summary: Encord Python SDK
 Client Home-page: https://github.com/encord-team/encord-client-python License:
 Apache Software License Keywords: cord,encord Author: Cord Technologies Limited
 Author-email: hello@encord.com Requires-Python: >=3.7,<4.0 Classifier: License
 :: OSI Approved :: Apache Software License Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

