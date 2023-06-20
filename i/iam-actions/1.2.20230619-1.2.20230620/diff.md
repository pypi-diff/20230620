# Comparing `tmp/iam_actions-1.2.20230619.tar.gz` & `tmp/iam_actions-1.2.20230620.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230619.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230620.tar", max compression
```

## Comparing `iam_actions-1.2.20230619.tar` & `iam_actions-1.2.20230620.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-06-19 02:37:40.003550 iam_actions-1.2.20230619/LICENSE
--rw-r--r--   0        0        0     2302 2023-06-19 02:37:40.003550 iam_actions-1.2.20230619/README.md
--rw-r--r--   0        0        0      228 2023-06-19 02:37:40.003550 iam_actions-1.2.20230619/iam_actions/__init__.py
--rw-r--r--   0        0        0  4326719 2023-06-19 02:39:20.642986 iam_actions-1.2.20230619/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-06-19 02:37:40.003550 iam_actions-1.2.20230619/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-06-19 02:37:40.003550 iam_actions-1.2.20230619/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-06-19 02:37:40.003550 iam_actions-1.2.20230619/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-06-19 02:37:40.003550 iam_actions-1.2.20230619/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-06-19 02:37:40.003550 iam_actions-1.2.20230619/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-06-19 02:37:40.003550 iam_actions-1.2.20230619/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-06-19 02:37:40.003550 iam_actions-1.2.20230619/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-06-19 02:37:40.003550 iam_actions-1.2.20230619/iam_actions/generate/services.py
--rw-r--r--   0        0        0   556740 2023-06-19 02:39:20.642986 iam_actions-1.2.20230619/iam_actions/policies.json
--rw-r--r--   0        0        0   196395 2023-06-19 02:39:20.642986 iam_actions-1.2.20230619/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   540016 2023-06-19 02:39:20.642986 iam_actions-1.2.20230619/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-06-19 02:39:21.390982 iam_actions-1.2.20230619/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230619/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230619/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-20 02:31:40.499296 iam_actions-1.2.20230620/LICENSE
+-rw-r--r--   0        0        0     2302 2023-06-20 02:31:40.499296 iam_actions-1.2.20230620/README.md
+-rw-r--r--   0        0        0      228 2023-06-20 02:31:40.499296 iam_actions-1.2.20230620/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4334986 2023-06-20 02:33:41.836732 iam_actions-1.2.20230620/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-06-20 02:31:40.499296 iam_actions-1.2.20230620/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-06-20 02:31:40.499296 iam_actions-1.2.20230620/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-06-20 02:31:40.499296 iam_actions-1.2.20230620/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-06-20 02:31:40.499296 iam_actions-1.2.20230620/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-06-20 02:31:40.499296 iam_actions-1.2.20230620/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-06-20 02:31:40.499296 iam_actions-1.2.20230620/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-06-20 02:31:40.499296 iam_actions-1.2.20230620/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-06-20 02:31:40.499296 iam_actions-1.2.20230620/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   557555 2023-06-20 02:33:41.836732 iam_actions-1.2.20230620/iam_actions/policies.json
+-rw-r--r--   0        0        0   196395 2023-06-20 02:33:41.836732 iam_actions-1.2.20230620/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   540781 2023-06-20 02:33:41.836732 iam_actions-1.2.20230620/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-06-20 02:33:42.768792 iam_actions-1.2.20230620/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230620/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230620/PKG-INFO
```

### Comparing `iam_actions-1.2.20230619/LICENSE` & `iam_actions-1.2.20230620/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230619/README.md` & `iam_actions-1.2.20230620/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230619/iam_actions/actions.json` & `iam_actions-1.2.20230620/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994688032235285%*

 * *Differences: {"'dms'": "{'DescribeConversionConfiguration': OrderedDict([('access_level', 'Read'), ('action', "*

 * *          "'DescribeConversionConfiguration'), ('condition_keys', []), ('description', 'Grants "*

 * *          "permission to return information about DMS Schema Conversion project configuration'), "*

 * *          "('orphan', False), ('resources', ['MigrationProject'])]), 'DescribeDataProviders': "*

 * *          "OrderedDict([('access_level', 'Read'), ('action', 'DescribeDataProviders'), "*

 * *          "('condition_keys', [] […]*

```diff
@@ -39193,22 +39193,42 @@
             "access_level": "Read",
             "action": "DescribeConnections",
             "condition_keys": [],
             "description": "Grants permission to describe the status of the connections that have been made between the replication instance and an endpoint",
             "orphan": false,
             "resources": []
         },
+        "DescribeConversionConfiguration": {
+            "access_level": "Read",
+            "action": "DescribeConversionConfiguration",
+            "condition_keys": [],
+            "description": "Grants permission to return information about DMS Schema Conversion project configuration",
+            "orphan": false,
+            "resources": [
+                "MigrationProject"
+            ]
+        },
         "DescribeDataMigrations": {
             "access_level": "Read",
             "action": "DescribeDataMigrations",
             "condition_keys": [],
             "description": "Grants permission to return information about database migrations for your account in the specified region",
             "orphan": false,
             "resources": []
         },
+        "DescribeDataProviders": {
+            "access_level": "Read",
+            "action": "DescribeDataProviders",
+            "condition_keys": [],
+            "description": "Grants permission to list the AWS DMS attributes for a data providers. Note. This action should be added along with ListDataProviders, but does not currently authorize the described Schema Conversion operation",
+            "orphan": false,
+            "resources": [
+                "DataProvider"
+            ]
+        },
         "DescribeEndpointSettings": {
             "access_level": "Read",
             "action": "DescribeEndpointSettings",
             "condition_keys": [],
             "description": "Grants permission to return the possible endpoint settings available when you create an endpoint for a specific database engine",
             "orphan": false,
             "resources": []
@@ -39249,14 +39269,24 @@
             "access_level": "Read",
             "action": "DescribeEvents",
             "condition_keys": [],
             "description": "Grants permission to list events for a given source identifier and source type",
             "orphan": false,
             "resources": []
         },
+        "DescribeExtensionPackAssociations": {
+            "access_level": "Read",
+            "action": "DescribeExtensionPackAssociations",
+            "condition_keys": [],
+            "description": "Grants permission to list the AWS DMS attributes for extension packs. Note. This action should be added along with ListExtensionPacks, but does not currently authorize the described Schema Conversion operation",
+            "orphan": false,
+            "resources": [
+                "MigrationProject"
+            ]
+        },
         "DescribeFleetAdvisorCollectors": {
             "access_level": "Read",
             "action": "DescribeFleetAdvisorCollectors",
             "condition_keys": [],
             "description": "Grants permission to return a paginated list of Fleet Advisor collectors in your account based on filter settings",
             "orphan": false,
             "resources": []
@@ -39289,14 +39319,86 @@
             "access_level": "Read",
             "action": "DescribeFleetAdvisorSchemas",
             "condition_keys": [],
             "description": "Grants permission to return a paginated list of schemas discovered by your Fleet Advisor collectors based on filter settings",
             "orphan": false,
             "resources": []
         },
+        "DescribeInstanceProfiles": {
+            "access_level": "Read",
+            "action": "DescribeInstanceProfiles",
+            "condition_keys": [],
+            "description": "Grants permission to list the AWS DMS attributes for a instance profiles. Note. This action should be added along with ListInstanceProfiles, but does not currently authorize the described Schema Conversion operation",
+            "orphan": false,
+            "resources": [
+                "InstanceProfile"
+            ]
+        },
+        "DescribeMetadataModelAssessments": {
+            "access_level": "Read",
+            "action": "DescribeMetadataModelAssessments",
+            "condition_keys": [],
+            "description": "Grants permission to list the AWS DMS attributes for metadata model assessments. Note. This action should be added along with ListMetadataModelAssessments, but does not currently authorize the described Schema Conversion operation",
+            "orphan": false,
+            "resources": [
+                "MigrationProject"
+            ]
+        },
+        "DescribeMetadataModelConversions": {
+            "access_level": "Read",
+            "action": "DescribeMetadataModelConversions",
+            "condition_keys": [],
+            "description": "Grants permission to list the AWS DMS attributes for a metadata model conversions. Note. This action should be added along with ListMetadataModelConversions, but does not currently authorize the described Schema Conversion operation",
+            "orphan": false,
+            "resources": [
+                "MigrationProject"
+            ]
+        },
+        "DescribeMetadataModelExportsAsScript": {
+            "access_level": "Read",
+            "action": "DescribeMetadataModelExportsAsScript",
+            "condition_keys": [],
+            "description": "Grants permission to list the AWS DMS attributes for a metadata model exports. Note. This action should be added along with ListMetadataModelExports, but does not currently authorize the described Schema Conversion operation",
+            "orphan": false,
+            "resources": [
+                "MigrationProject"
+            ]
+        },
+        "DescribeMetadataModelExportsToTarget": {
+            "access_level": "Read",
+            "action": "DescribeMetadataModelExportsToTarget",
+            "condition_keys": [],
+            "description": "Grants permission to list the AWS DMS attributes for a metadata model exports. Note. This action should be added along with ListMetadataModelExports, but does not currently authorize the described Schema Conversion operation",
+            "orphan": false,
+            "resources": [
+                "MigrationProject"
+            ]
+        },
+        "DescribeMetadataModelImports": {
+            "access_level": "Read",
+            "action": "DescribeMetadataModelImports",
+            "condition_keys": [],
+            "description": "Grants permission to return information about start metadata model import operations for a migration project",
+            "orphan": false,
+            "resources": [
+                "MigrationProject"
+            ]
+        },
+        "DescribeMigrationProjects": {
+            "access_level": "Read",
+            "action": "DescribeMigrationProjects",
+            "condition_keys": [],
+            "description": "Grants permission to list the AWS DMS attributes for a migration projects. Note. This action should be added along with ListMigrationProjects, but does not currently authorize the described Schema Conversion operation",
+            "orphan": false,
+            "resources": [
+                "DataProvider",
+                "InstanceProfile",
+                "MigrationProject"
+            ]
+        },
         "DescribeOrderableReplicationInstances": {
             "access_level": "Read",
             "action": "DescribeOrderableReplicationInstances",
             "condition_keys": [],
             "description": "Grants permission to return information about the replication instance types that can be created in the specified region",
             "orphan": false,
             "resources": []
@@ -39590,24 +39692,44 @@
                 "MigrationProject",
                 "ReplicationConfig",
                 "ReplicationInstance",
                 "ReplicationSubnetGroup",
                 "ReplicationTask"
             ]
         },
+        "ModifyConversionConfiguration": {
+            "access_level": "Write",
+            "action": "ModifyConversionConfiguration",
+            "condition_keys": [],
+            "description": "Grants permission to update a conversion configuration. Note. This action should be added along with UpdateConversionConfiguration, but does not currently authorize the described Schema Conversion operation",
+            "orphan": false,
+            "resources": [
+                "MigrationProject"
+            ]
+        },
         "ModifyDataMigration": {
             "access_level": "Write",
             "action": "ModifyDataMigration",
             "condition_keys": [],
             "description": "Grants permission to modify the specified database migration",
             "orphan": false,
             "resources": [
                 "DataMigration"
             ]
         },
+        "ModifyDataProvider": {
+            "access_level": "Write",
+            "action": "ModifyDataProvider",
+            "condition_keys": [],
+            "description": "Grants permission to modify the specified data provider. Note. This action should be added along with UpdateDataProvider, but does not currently authorize the described Schema Conversion operation",
+            "orphan": false,
+            "resources": [
+                "DataProvider"
+            ]
+        },
         "ModifyEndpoint": {
             "access_level": "Write",
             "action": "ModifyEndpoint",
             "condition_keys": [],
             "description": "Grants permission to modify the specified endpoint",
             "orphan": false,
             "resources": [
@@ -39635,14 +39757,34 @@
             "access_level": "Write",
             "action": "ModifyFleetAdvisorCollectorStatuses",
             "condition_keys": [],
             "description": "Grants permission to modify the status of the specified Fleet Advisor collector",
             "orphan": false,
             "resources": []
         },
+        "ModifyInstanceProfile": {
+            "access_level": "Write",
+            "action": "ModifyInstanceProfile",
+            "condition_keys": [],
+            "description": "Grants permission to modify the specified instance profile. Note. This action should be added along with UpdateInstanceProfile, but does not currently authorize the described Schema Conversion operation",
+            "orphan": false,
+            "resources": [
+                "InstanceProfile"
+            ]
+        },
+        "ModifyMigrationProject": {
+            "access_level": "Write",
+            "action": "ModifyMigrationProject",
+            "condition_keys": [],
+            "description": "Grants permission to modify the specified migration project. Note. This action should be added along with UpdateMigrationProject, but does not currently authorize the described Schema Conversion operation",
+            "orphan": false,
+            "resources": [
+                "MigrationProject"
+            ]
+        },
         "ModifyReplicationConfig": {
             "access_level": "Write",
             "action": "ModifyReplicationConfig",
             "condition_keys": [],
             "description": "Grants permission to modify the specified replication config",
             "orphan": false,
             "resources": [
@@ -39765,14 +39907,24 @@
             "condition_keys": [],
             "description": "Grants permission to start the database migration",
             "orphan": false,
             "resources": [
                 "DataMigration"
             ]
         },
+        "StartExtensionPackAssociation": {
+            "access_level": "Write",
+            "action": "StartExtensionPackAssociation",
+            "condition_keys": [],
+            "description": "Grants permission to associate an extension pack. Note. This action should be added along with AssociateExtensionPack, but does not currently authorize the described Schema Conversion operation",
+            "orphan": false,
+            "resources": [
+                "MigrationProject"
+            ]
+        },
         "StartMetadataModelAssessment": {
             "access_level": "Write",
             "action": "StartMetadataModelAssessment",
             "condition_keys": [],
             "description": "Grants permission to start a new assessment of metadata model",
             "orphan": false,
             "resources": [
@@ -39785,14 +39937,24 @@
             "condition_keys": [],
             "description": "Grants permission to start a new conversion of metadata model",
             "orphan": false,
             "resources": [
                 "MigrationProject"
             ]
         },
+        "StartMetadataModelExportAsScript": {
+            "access_level": "Write",
+            "action": "StartMetadataModelExportAsScript",
+            "condition_keys": [],
+            "description": "Grants permission to start a new export of metadata model as script. Note. This action should be added along with StartMetadataModelExportAsScripts, but does not currently authorize the described Schema Conversion operation",
+            "orphan": false,
+            "resources": [
+                "MigrationProject"
+            ]
+        },
         "StartMetadataModelExportAsScripts": {
             "access_level": "Write",
             "action": "StartMetadataModelExportAsScripts",
             "condition_keys": [],
             "description": "Grants permission to start a new export of metadata model as script",
             "orphan": false,
             "resources": [
@@ -90828,14 +90990,22 @@
             "condition_keys": [],
             "description": "Grants permission to create a new log stream with the specified name",
             "orphan": false,
             "resources": [
                 "log-group"
             ]
         },
+        "DeleteAccountPolicy": {
+            "access_level": "Write",
+            "action": "DeleteAccountPolicy",
+            "condition_keys": [],
+            "description": "Grants permission to delete a data protection policy attached to an account",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteDataProtectionPolicy": {
             "access_level": "Write",
             "action": "DeleteDataProtectionPolicy",
             "condition_keys": [],
             "description": "Grants permission to delete a data protection policy attached to a log group",
             "orphan": false,
             "resources": [
@@ -90922,14 +91092,22 @@
             "condition_keys": [],
             "description": "Grants permission to delete a subscription filter associated with the specified log group",
             "orphan": false,
             "resources": [
                 "log-group"
             ]
         },
+        "DescribeAccountPolicies": {
+            "access_level": "List",
+            "action": "DescribeAccountPolicies",
+            "condition_keys": [],
+            "description": "Grants permission to retrieve a data protection policy attached to an account",
+            "orphan": false,
+            "resources": []
+        },
         "DescribeDestinations": {
             "access_level": "List",
             "action": "DescribeDestinations",
             "condition_keys": [],
             "description": "Grants permission to return all the destinations that are associated with the AWS account making the request",
             "orphan": false,
             "resources": []
@@ -91111,14 +91289,22 @@
             "condition_keys": [],
             "description": "Grants permission to list the tags for the specified log group",
             "orphan": false,
             "resources": [
                 "log-group"
             ]
         },
+        "PutAccountPolicy": {
+            "access_level": "Write",
+            "action": "PutAccountPolicy",
+            "condition_keys": [],
+            "description": "Grants permission to attach a data protection policy at account level to detect and redact sensitive information from log events",
+            "orphan": false,
+            "resources": []
+        },
         "PutDataProtectionPolicy": {
             "access_level": "Write",
             "action": "PutDataProtectionPolicy",
             "condition_keys": [],
             "description": "Grants permission to attach a data protection policy to detect and redact sensitive information from log events",
             "orphan": false,
             "resources": [
@@ -109876,22 +110062,46 @@
             "access_level": "List",
             "action": "ListPurchaseOrders",
             "condition_keys": [],
             "description": "Grants permission to get all available purchase orders",
             "orphan": false,
             "resources": []
         },
+        "ListTagsForResource": {
+            "access_level": "Undocumented",
+            "action": "ListTagsForResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ModifyPurchaseOrders": {
             "access_level": "Write",
             "action": "ModifyPurchaseOrders",
             "condition_keys": [],
             "description": "Grants permission to modify purchase orders and details",
             "orphan": false,
             "resources": []
         },
+        "TagResource": {
+            "access_level": "Undocumented",
+            "action": "TagResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UntagResource": {
+            "access_level": "Undocumented",
+            "action": "UntagResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UpdateConsoleActionSetEnforced": {
             "access_level": "Write",
             "action": "UpdateConsoleActionSetEnforced",
             "condition_keys": [],
             "description": "Grants permission to change whether existing or fine-grained IAM actions will be used to control authorization to Billing, Cost Management, and Account consoles",
             "orphan": false,
             "resources": []
```

### Comparing `iam_actions-1.2.20230619/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230620/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230619/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230620/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230619/iam_actions/generate/generate.py` & `iam_actions-1.2.20230620/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230619/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230620/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230619/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230620/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230619/iam_actions/generate/services.py` & `iam_actions-1.2.20230620/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230619/iam_actions/policies.json` & `iam_actions-1.2.20230620/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999408026993606%*

 * *Differences: {"'serviceMap'": "{'AWS Database Migration Service': {'Actions': {insert: [(38, "*

 * *                 "'DescribeConversionConfiguration'), (40, 'DescribeDataProviders'), (47, "*

 * *                 "'DescribeExtensionPackAssociations'), (53, 'DescribeInstanceProfiles'), (54, "*

 * *                 "'DescribeMetadataModelAssessments'), (55, 'DescribeMetadataModelConversions'), "*

 * *                 "(56, 'DescribeMetadataModelExportsAsScript'), (57, "*

 * *                 "'DescribeMetadataModelExportsToTarget'), (58, 'Descri […]*

```diff
@@ -2669,26 +2669,36 @@
                 "DeleteReplicationSubnetGroup",
                 "DeleteReplicationTask",
                 "DeleteReplicationTaskAssessmentRun",
                 "DescribeAccountAttributes",
                 "DescribeApplicableIndividualAssessments",
                 "DescribeCertificates",
                 "DescribeConnections",
+                "DescribeConversionConfiguration",
                 "DescribeDataMigrations",
+                "DescribeDataProviders",
                 "DescribeEndpointSettings",
                 "DescribeEndpointTypes",
                 "DescribeEndpoints",
                 "DescribeEventCategories",
                 "DescribeEventSubscriptions",
                 "DescribeEvents",
+                "DescribeExtensionPackAssociations",
                 "DescribeFleetAdvisorCollectors",
                 "DescribeFleetAdvisorDatabases",
                 "DescribeFleetAdvisorLsaAnalysis",
                 "DescribeFleetAdvisorSchemaObjectSummary",
                 "DescribeFleetAdvisorSchemas",
+                "DescribeInstanceProfiles",
+                "DescribeMetadataModelAssessments",
+                "DescribeMetadataModelConversions",
+                "DescribeMetadataModelExportsAsScript",
+                "DescribeMetadataModelExportsToTarget",
+                "DescribeMetadataModelImports",
+                "DescribeMigrationProjects",
                 "DescribeOrderableReplicationInstances",
                 "DescribePendingMaintenanceActions",
                 "DescribeRecommendationLimitations",
                 "DescribeRecommendations",
                 "DescribeRefreshSchemasStatus",
                 "DescribeReplicationConfigs",
                 "DescribeReplicationInstanceTaskLogs",
@@ -2711,33 +2721,39 @@
                 "ListInstanceProfiles",
                 "ListMetadataModelAssessmentActionItems",
                 "ListMetadataModelAssessments",
                 "ListMetadataModelConversions",
                 "ListMetadataModelExports",
                 "ListMigrationProjects",
                 "ListTagsForResource",
+                "ModifyConversionConfiguration",
                 "ModifyDataMigration",
+                "ModifyDataProvider",
                 "ModifyEndpoint",
                 "ModifyEventSubscription",
                 "ModifyFleetAdvisorCollector",
                 "ModifyFleetAdvisorCollectorStatuses",
+                "ModifyInstanceProfile",
+                "ModifyMigrationProject",
                 "ModifyReplicationConfig",
                 "ModifyReplicationInstance",
                 "ModifyReplicationSubnetGroup",
                 "ModifyReplicationTask",
                 "MoveReplicationTask",
                 "RebootReplicationInstance",
                 "RefreshSchemas",
                 "ReloadReplicationTables",
                 "ReloadTables",
                 "RemoveTagsFromResource",
                 "RunFleetAdvisorLsaAnalysis",
                 "StartDataMigration",
+                "StartExtensionPackAssociation",
                 "StartMetadataModelAssessment",
                 "StartMetadataModelConversion",
+                "StartMetadataModelExportAsScript",
                 "StartMetadataModelExportAsScripts",
                 "StartMetadataModelExportToTarget",
                 "StartMetadataModelImport",
                 "StartRecommendations",
                 "StartReplication",
                 "StartReplicationTask",
                 "StartReplicationTaskAssessment",
@@ -7455,31 +7471,39 @@
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys",
                 "proton:EnvironmentTemplate",
                 "proton:ServiceTemplate"
             ]
         },
         "AWS Purchase Orders Console": {
-            "ARNFormat": "arn:${Partition}:purchase-orders::${Account}:${ResourceType}:${ResourceName}",
-            "ARNRegex": "^arn:${Partition}:purchase-orders::.+:.+:.+",
+            "ARNFormat": "arn:aws:purchase-orders::${Account}:${ResourceType}/${ResourceName}",
+            "ARNRegex": "^arn:aws:purchase-orders::.+:.+",
             "Actions": [
                 "AddPurchaseOrder",
                 "DeletePurchaseOrder",
                 "GetConsoleActionSetEnforced",
                 "GetPurchaseOrder",
                 "ListPurchaseOrderInvoices",
                 "ListPurchaseOrders",
+                "ListTagsForResource",
                 "ModifyPurchaseOrders",
+                "TagResource",
+                "UntagResource",
                 "UpdateConsoleActionSetEnforced",
                 "UpdatePurchaseOrder",
                 "UpdatePurchaseOrderStatus",
                 "ViewPurchaseOrders"
             ],
-            "HasResource": false,
-            "StringPrefix": "purchase-orders"
+            "HasResource": true,
+            "StringPrefix": "purchase-orders",
+            "conditionKeys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys"
+            ]
         },
         "AWS Recycle Bin": {
             "ARNFormat": "arn:aws:rbin:${Region}:${Account}:rule/${ResourceName}",
             "ARNRegex": "^arn:aws:rbin:.+:.+:.+",
             "Actions": [
                 "CreateRule",
                 "DeleteRule",
@@ -10892,24 +10916,26 @@
             "Actions": [
                 "AssociateKmsKey",
                 "CancelExportTask",
                 "CreateExportTask",
                 "CreateLogDelivery",
                 "CreateLogGroup",
                 "CreateLogStream",
+                "DeleteAccountPolicy",
                 "DeleteDataProtectionPolicy",
                 "DeleteDestination",
                 "DeleteLogDelivery",
                 "DeleteLogGroup",
                 "DeleteLogStream",
                 "DeleteMetricFilter",
                 "DeleteQueryDefinition",
                 "DeleteResourcePolicy",
                 "DeleteRetentionPolicy",
                 "DeleteSubscriptionFilter",
+                "DescribeAccountPolicies",
                 "DescribeDestinations",
                 "DescribeExportTasks",
                 "DescribeLogGroups",
                 "DescribeLogStreams",
                 "DescribeMetricFilters",
                 "DescribeQueries",
                 "DescribeQueryDefinitions",
@@ -10923,14 +10949,15 @@
                 "GetLogGroupFields",
                 "GetLogRecord",
                 "GetQueryResults",
                 "Link",
                 "ListLogDeliveries",
                 "ListTagsForResource",
                 "ListTagsLogGroup",
+                "PutAccountPolicy",
                 "PutDataProtectionPolicy",
                 "PutDestination",
                 "PutDestinationPolicy",
                 "PutLogEvents",
                 "PutMetricFilter",
                 "PutQueryDefinition",
                 "PutResourcePolicy",
```

### Comparing `iam_actions-1.2.20230619/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230620/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230619/iam_actions/services.json` & `iam_actions-1.2.20230620/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994953284454229%*

 * *Differences: {"'dms'": "{'Actions': {insert: [(38, 'DescribeConversionConfiguration'), (40, "*

 * *          "'DescribeDataProviders'), (47, 'DescribeExtensionPackAssociations'), (53, "*

 * *          "'DescribeInstanceProfiles'), (54, 'DescribeMetadataModelAssessments'), (55, "*

 * *          "'DescribeMetadataModelConversions'), (56, 'DescribeMetadataModelExportsAsScript'), (57, "*

 * *          "'DescribeMetadataModelExportsToTarget'), (58, 'DescribeMetadataModelImports'), (59, "*

 * *          "'DescribeMigrationProjects'), (90, 'ModifyConv […]*

```diff
@@ -5854,26 +5854,36 @@
             "DeleteReplicationSubnetGroup",
             "DeleteReplicationTask",
             "DeleteReplicationTaskAssessmentRun",
             "DescribeAccountAttributes",
             "DescribeApplicableIndividualAssessments",
             "DescribeCertificates",
             "DescribeConnections",
+            "DescribeConversionConfiguration",
             "DescribeDataMigrations",
+            "DescribeDataProviders",
             "DescribeEndpointSettings",
             "DescribeEndpointTypes",
             "DescribeEndpoints",
             "DescribeEventCategories",
             "DescribeEventSubscriptions",
             "DescribeEvents",
+            "DescribeExtensionPackAssociations",
             "DescribeFleetAdvisorCollectors",
             "DescribeFleetAdvisorDatabases",
             "DescribeFleetAdvisorLsaAnalysis",
             "DescribeFleetAdvisorSchemaObjectSummary",
             "DescribeFleetAdvisorSchemas",
+            "DescribeInstanceProfiles",
+            "DescribeMetadataModelAssessments",
+            "DescribeMetadataModelConversions",
+            "DescribeMetadataModelExportsAsScript",
+            "DescribeMetadataModelExportsToTarget",
+            "DescribeMetadataModelImports",
+            "DescribeMigrationProjects",
             "DescribeOrderableReplicationInstances",
             "DescribePendingMaintenanceActions",
             "DescribeRecommendationLimitations",
             "DescribeRecommendations",
             "DescribeRefreshSchemasStatus",
             "DescribeReplicationConfigs",
             "DescribeReplicationInstanceTaskLogs",
@@ -5896,33 +5906,39 @@
             "ListInstanceProfiles",
             "ListMetadataModelAssessmentActionItems",
             "ListMetadataModelAssessments",
             "ListMetadataModelConversions",
             "ListMetadataModelExports",
             "ListMigrationProjects",
             "ListTagsForResource",
+            "ModifyConversionConfiguration",
             "ModifyDataMigration",
+            "ModifyDataProvider",
             "ModifyEndpoint",
             "ModifyEventSubscription",
             "ModifyFleetAdvisorCollector",
             "ModifyFleetAdvisorCollectorStatuses",
+            "ModifyInstanceProfile",
+            "ModifyMigrationProject",
             "ModifyReplicationConfig",
             "ModifyReplicationInstance",
             "ModifyReplicationSubnetGroup",
             "ModifyReplicationTask",
             "MoveReplicationTask",
             "RebootReplicationInstance",
             "RefreshSchemas",
             "ReloadReplicationTables",
             "ReloadTables",
             "RemoveTagsFromResource",
             "RunFleetAdvisorLsaAnalysis",
             "StartDataMigration",
+            "StartExtensionPackAssociation",
             "StartMetadataModelAssessment",
             "StartMetadataModelConversion",
+            "StartMetadataModelExportAsScript",
             "StartMetadataModelExportAsScripts",
             "StartMetadataModelExportToTarget",
             "StartMetadataModelImport",
             "StartRecommendations",
             "StartReplication",
             "StartReplicationTask",
             "StartReplicationTaskAssessment",
@@ -12609,24 +12625,26 @@
         "Actions": [
             "AssociateKmsKey",
             "CancelExportTask",
             "CreateExportTask",
             "CreateLogDelivery",
             "CreateLogGroup",
             "CreateLogStream",
+            "DeleteAccountPolicy",
             "DeleteDataProtectionPolicy",
             "DeleteDestination",
             "DeleteLogDelivery",
             "DeleteLogGroup",
             "DeleteLogStream",
             "DeleteMetricFilter",
             "DeleteQueryDefinition",
             "DeleteResourcePolicy",
             "DeleteRetentionPolicy",
             "DeleteSubscriptionFilter",
+            "DescribeAccountPolicies",
             "DescribeDestinations",
             "DescribeExportTasks",
             "DescribeLogGroups",
             "DescribeLogStreams",
             "DescribeMetricFilters",
             "DescribeQueries",
             "DescribeQueryDefinitions",
@@ -12640,14 +12658,15 @@
             "GetLogGroupFields",
             "GetLogRecord",
             "GetQueryResults",
             "Link",
             "ListLogDeliveries",
             "ListTagsForResource",
             "ListTagsLogGroup",
+            "PutAccountPolicy",
             "PutDataProtectionPolicy",
             "PutDestination",
             "PutDestinationPolicy",
             "PutLogEvents",
             "PutMetricFilter",
             "PutQueryDefinition",
             "PutResourcePolicy",
@@ -15443,34 +15462,41 @@
         "HasResource": true,
         "ServiceNames": [
             "AWS Proton"
         ]
     },
     "purchase-orders": {
         "ARNFormats": [
-            "arn:${Partition}:purchase-orders::${Account}:${ResourceType}:${ResourceName}"
+            "arn:aws:purchase-orders::${Account}:${ResourceType}/${ResourceName}"
         ],
         "ARNRegexes": [
-            "^arn:${Partition}:purchase-orders::.+:.+:.+"
+            "^arn:aws:purchase-orders::.+:.+"
         ],
         "Actions": [
             "AddPurchaseOrder",
             "DeletePurchaseOrder",
             "GetConsoleActionSetEnforced",
             "GetPurchaseOrder",
             "ListPurchaseOrderInvoices",
             "ListPurchaseOrders",
+            "ListTagsForResource",
             "ModifyPurchaseOrders",
+            "TagResource",
+            "UntagResource",
             "UpdateConsoleActionSetEnforced",
             "UpdatePurchaseOrder",
             "UpdatePurchaseOrderStatus",
             "ViewPurchaseOrders"
         ],
-        "ConditionKeys": [],
-        "HasResource": false,
+        "ConditionKeys": [
+            "aws:RequestTag/${TagKey}",
+            "aws:ResourceTag/${TagKey}",
+            "aws:TagKeys"
+        ],
+        "HasResource": true,
         "ServiceNames": [
             "AWS Purchase Orders Console"
         ]
     },
     "qldb": {
         "ARNFormats": [
             "arn:aws:qldb:${Region}:${Account}:${ResourceType}/${ResourcePath}"
```

### Comparing `iam_actions-1.2.20230619/pyproject.toml` & `iam_actions-1.2.20230620/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230619"
+version = "1.2.20230620"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230619/setup.py` & `iam_actions-1.2.20230620/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230619',
+    'version': '1.2.20230620',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230619/PKG-INFO` & `iam_actions-1.2.20230620/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230619
+Version: 1.2.20230620
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

