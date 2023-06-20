# Comparing `tmp/cognite-sdk-experimental-0.98.0.tar.gz` & `tmp/cognite-sdk-experimental-0.99.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite-sdk-experimental-0.98.0.tar", max compression
+gzip compressed data, was "cognite-sdk-experimental-0.99.0.tar", max compression
```

## Comparing `cognite-sdk-experimental-0.98.0.tar` & `cognite-sdk-experimental-0.99.0.tar`

### file list

```diff
@@ -1,41 +1,37 @@
--rw-r--r--   0        0        0    11344 2022-09-06 13:35:27.425448 cognite-sdk-experimental-0.98.0/LICENSE
--rw-r--r--   0        0        0       55 2022-09-06 13:35:27.425448 cognite-sdk-experimental-0.98.0/cognite/experimental/__init__.py
--rw-r--r--   0        0        0        0 2022-09-06 13:35:27.425448 cognite-sdk-experimental-0.98.0/cognite/experimental/_api/__init__.py
--rw-r--r--   0        0        0     7240 2022-09-06 13:35:27.425448 cognite-sdk-experimental-0.98.0/cognite/experimental/_api/alerts.py
--rw-r--r--   0        0        0     5420 2022-09-06 13:35:27.425448 cognite-sdk-experimental-0.98.0/cognite/experimental/_api/annotations.py
--rw-r--r--   0        0        0     1976 2022-09-06 13:35:27.425448 cognite-sdk-experimental-0.98.0/cognite/experimental/_api/document_parsing.py
--rw-r--r--   0        0        0    13217 2022-09-06 13:35:27.425448 cognite-sdk-experimental-0.98.0/cognite/experimental/_api/entity_matching.py
--rw-r--r--   0        0        0     1589 2022-09-06 13:35:27.425448 cognite-sdk-experimental-0.98.0/cognite/experimental/_api/extractionpipelines.py
--rw-r--r--   0        0        0    22582 2022-09-06 13:35:27.425448 cognite-sdk-experimental-0.98.0/cognite/experimental/_api/geospatial.py
--rw-r--r--   0        0        0     3540 2022-09-06 13:35:27.425448 cognite-sdk-experimental-0.98.0/cognite/experimental/_api/legacy_annotations.py
--rw-r--r--   0        0        0     2511 2022-09-06 13:35:27.425448 cognite-sdk-experimental-0.98.0/cognite/experimental/_api/match_rules.py
--rw-r--r--   0        0        0      721 2022-09-06 13:35:27.425448 cognite-sdk-experimental-0.98.0/cognite/experimental/_api/pnid_object_detection.py
--rw-r--r--   0        0        0     5652 2022-09-06 13:35:27.425448 cognite-sdk-experimental-0.98.0/cognite/experimental/_api/pnid_parsing.py
--rw-r--r--   0        0        0     3103 2022-09-06 13:35:27.425448 cognite-sdk-experimental-0.98.0/cognite/experimental/_api/templatecompletion.py
--rw-r--r--   0        0        0     6455 2022-09-06 13:35:27.425448 cognite-sdk-experimental-0.98.0/cognite/experimental/_api/vision.py
--rw-r--r--   0        0        0     5023 2022-09-06 13:35:27.425448 cognite-sdk-experimental-0.98.0/cognite/experimental/_client.py
--rw-r--r--   0        0        0     2652 2022-09-06 13:35:27.425448 cognite-sdk-experimental-0.98.0/cognite/experimental/_context_client.py
--rw-r--r--   0        0        0      370 2022-09-06 13:35:27.425448 cognite-sdk-experimental-0.98.0/cognite/experimental/data_classes/__init__.py
--rw-r--r--   0        0        0     7341 2022-09-06 13:35:27.425448 cognite-sdk-experimental-0.98.0/cognite/experimental/data_classes/alerts.py
--rw-r--r--   0        0        0     1563 2022-09-06 13:35:27.425448 cognite-sdk-experimental-0.98.0/cognite/experimental/data_classes/annotation_types/images.py
--rw-r--r--   0        0        0     3042 2022-09-06 13:35:27.425448 cognite-sdk-experimental-0.98.0/cognite/experimental/data_classes/annotation_types/primitives.py
--rw-r--r--   0        0        0     8917 2022-09-06 13:35:27.429448 cognite-sdk-experimental-0.98.0/cognite/experimental/data_classes/annotations.py
--rw-r--r--   0        0        0    19186 2022-09-06 13:35:27.429448 cognite-sdk-experimental-0.98.0/cognite/experimental/data_classes/contextualization.py
--rw-r--r--   0        0        0     1289 2022-09-06 13:35:27.429448 cognite-sdk-experimental-0.98.0/cognite/experimental/data_classes/extractionpipelines.py
--rw-r--r--   0        0        0     2133 2022-09-06 13:35:27.429448 cognite-sdk-experimental-0.98.0/cognite/experimental/data_classes/geospatial.py
--rw-r--r--   0        0        0     4639 2022-09-06 13:35:27.429448 cognite-sdk-experimental-0.98.0/cognite/experimental/data_classes/legacy_annotations.py
--rw-r--r--   0        0        0        0 2022-09-06 13:35:27.429448 cognite-sdk-experimental-0.98.0/cognite/experimental/data_classes/model_hosting/__init__.py
--rw-r--r--   0        0        0     1856 2022-09-06 13:35:27.429448 cognite-sdk-experimental-0.98.0/cognite/experimental/data_classes/model_hosting/models.py
--rw-r--r--   0        0        0     3101 2022-09-06 13:35:27.429448 cognite-sdk-experimental-0.98.0/cognite/experimental/data_classes/model_hosting/schedules.py
--rw-r--r--   0        0        0     2603 2022-09-06 13:35:27.429448 cognite-sdk-experimental-0.98.0/cognite/experimental/data_classes/model_hosting/source_packages.py
--rw-r--r--   0        0        0     3016 2022-09-06 13:35:27.429448 cognite-sdk-experimental-0.98.0/cognite/experimental/data_classes/model_hosting/versions.py
--rw-r--r--   0        0        0     1181 2022-09-06 13:35:27.429448 cognite-sdk-experimental-0.98.0/cognite/experimental/data_classes/shared.py
--rw-r--r--   0        0        0     4582 2022-09-06 13:35:27.429448 cognite-sdk-experimental-0.98.0/cognite/experimental/data_classes/types.py
--rw-r--r--   0        0        0      282 2022-09-06 13:35:27.429448 cognite-sdk-experimental-0.98.0/cognite/experimental/data_classes/utils/pandas.py
--rw-r--r--   0        0        0     3663 2022-09-06 13:35:27.429448 cognite-sdk-experimental-0.98.0/cognite/experimental/data_classes/utils/rules_output.py
--rw-r--r--   0        0        0    18689 2022-09-06 13:35:27.429448 cognite-sdk-experimental-0.98.0/cognite/experimental/data_classes/vision.py
--rw-r--r--   0        0        0        0 2022-09-06 13:35:27.429448 cognite-sdk-experimental-0.98.0/cognite/experimental/py.typed
--rw-r--r--   0        0        0     1210 2022-09-06 13:35:27.429448 cognite-sdk-experimental-0.98.0/cognite/experimental/utils.py
--rw-r--r--   0        0        0     1555 2022-09-06 13:35:27.429448 cognite-sdk-experimental-0.98.0/pyproject.toml
--rw-r--r--   0        0        0     1206 1970-01-01 00:00:00.000000 cognite-sdk-experimental-0.98.0/setup.py
--rw-r--r--   0        0        0      790 1970-01-01 00:00:00.000000 cognite-sdk-experimental-0.98.0/PKG-INFO
+-rw-r--r--   0        0        0    11344 2022-09-12 15:42:03.130723 cognite-sdk-experimental-0.99.0/LICENSE
+-rw-r--r--   0        0        0       55 2022-09-12 15:42:03.130723 cognite-sdk-experimental-0.99.0/cognite/experimental/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-12 15:42:03.130723 cognite-sdk-experimental-0.99.0/cognite/experimental/_api/__init__.py
+-rw-r--r--   0        0        0     7240 2022-09-12 15:42:03.130723 cognite-sdk-experimental-0.99.0/cognite/experimental/_api/alerts.py
+-rw-r--r--   0        0        0     5420 2022-09-12 15:42:03.130723 cognite-sdk-experimental-0.99.0/cognite/experimental/_api/annotations.py
+-rw-r--r--   0        0        0     1976 2022-09-12 15:42:03.130723 cognite-sdk-experimental-0.99.0/cognite/experimental/_api/document_parsing.py
+-rw-r--r--   0        0        0    13217 2022-09-12 15:42:03.130723 cognite-sdk-experimental-0.99.0/cognite/experimental/_api/entity_matching.py
+-rw-r--r--   0        0        0     1589 2022-09-12 15:42:03.130723 cognite-sdk-experimental-0.99.0/cognite/experimental/_api/extractionpipelines.py
+-rw-r--r--   0        0        0    22818 2022-09-12 15:42:03.130723 cognite-sdk-experimental-0.99.0/cognite/experimental/_api/geospatial.py
+-rw-r--r--   0        0        0     3540 2022-09-12 15:42:03.130723 cognite-sdk-experimental-0.99.0/cognite/experimental/_api/legacy_annotations.py
+-rw-r--r--   0        0        0     2511 2022-09-12 15:42:03.130723 cognite-sdk-experimental-0.99.0/cognite/experimental/_api/match_rules.py
+-rw-r--r--   0        0        0      721 2022-09-12 15:42:03.130723 cognite-sdk-experimental-0.99.0/cognite/experimental/_api/pnid_object_detection.py
+-rw-r--r--   0        0        0     5652 2022-09-12 15:42:03.130723 cognite-sdk-experimental-0.99.0/cognite/experimental/_api/pnid_parsing.py
+-rw-r--r--   0        0        0     3103 2022-09-12 15:42:03.130723 cognite-sdk-experimental-0.99.0/cognite/experimental/_api/templatecompletion.py
+-rw-r--r--   0        0        0     4875 2022-09-12 15:42:03.130723 cognite-sdk-experimental-0.99.0/cognite/experimental/_client.py
+-rw-r--r--   0        0        0     2652 2022-09-12 15:42:03.130723 cognite-sdk-experimental-0.99.0/cognite/experimental/_context_client.py
+-rw-r--r--   0        0        0      370 2022-09-12 15:42:03.130723 cognite-sdk-experimental-0.99.0/cognite/experimental/data_classes/__init__.py
+-rw-r--r--   0        0        0     7341 2022-09-12 15:42:03.130723 cognite-sdk-experimental-0.99.0/cognite/experimental/data_classes/alerts.py
+-rw-r--r--   0        0        0     8917 2022-09-12 15:42:03.130723 cognite-sdk-experimental-0.99.0/cognite/experimental/data_classes/annotations.py
+-rw-r--r--   0        0        0    19164 2022-09-12 15:42:03.130723 cognite-sdk-experimental-0.99.0/cognite/experimental/data_classes/contextualization.py
+-rw-r--r--   0        0        0     1289 2022-09-12 15:42:03.130723 cognite-sdk-experimental-0.99.0/cognite/experimental/data_classes/extractionpipelines.py
+-rw-r--r--   0        0        0     2133 2022-09-12 15:42:03.130723 cognite-sdk-experimental-0.99.0/cognite/experimental/data_classes/geospatial.py
+-rw-r--r--   0        0        0     4639 2022-09-12 15:42:03.130723 cognite-sdk-experimental-0.99.0/cognite/experimental/data_classes/legacy_annotations.py
+-rw-r--r--   0        0        0        0 2022-09-12 15:42:03.130723 cognite-sdk-experimental-0.99.0/cognite/experimental/data_classes/model_hosting/__init__.py
+-rw-r--r--   0        0        0     1856 2022-09-12 15:42:03.130723 cognite-sdk-experimental-0.99.0/cognite/experimental/data_classes/model_hosting/models.py
+-rw-r--r--   0        0        0     3101 2022-09-12 15:42:03.130723 cognite-sdk-experimental-0.99.0/cognite/experimental/data_classes/model_hosting/schedules.py
+-rw-r--r--   0        0        0     2603 2022-09-12 15:42:03.130723 cognite-sdk-experimental-0.99.0/cognite/experimental/data_classes/model_hosting/source_packages.py
+-rw-r--r--   0        0        0     3016 2022-09-12 15:42:03.130723 cognite-sdk-experimental-0.99.0/cognite/experimental/data_classes/model_hosting/versions.py
+-rw-r--r--   0        0        0     1181 2022-09-12 15:42:03.130723 cognite-sdk-experimental-0.99.0/cognite/experimental/data_classes/shared.py
+-rw-r--r--   0        0        0     4582 2022-09-12 15:42:03.130723 cognite-sdk-experimental-0.99.0/cognite/experimental/data_classes/types.py
+-rw-r--r--   0        0        0      282 2022-09-12 15:42:03.130723 cognite-sdk-experimental-0.99.0/cognite/experimental/data_classes/utils/pandas.py
+-rw-r--r--   0        0        0     3663 2022-09-12 15:42:03.130723 cognite-sdk-experimental-0.99.0/cognite/experimental/data_classes/utils/rules_output.py
+-rw-r--r--   0        0        0        0 2022-09-12 15:42:03.130723 cognite-sdk-experimental-0.99.0/cognite/experimental/py.typed
+-rw-r--r--   0        0        0     1210 2022-09-12 15:42:03.130723 cognite-sdk-experimental-0.99.0/cognite/experimental/utils.py
+-rw-r--r--   0        0        0     1555 2022-09-12 15:42:03.130723 cognite-sdk-experimental-0.99.0/pyproject.toml
+-rw-r--r--   0        0        0     1151 1970-01-01 00:00:00.000000 cognite-sdk-experimental-0.99.0/setup.py
+-rw-r--r--   0        0        0      790 1970-01-01 00:00:00.000000 cognite-sdk-experimental-0.99.0/PKG-INFO
```

### Comparing `cognite-sdk-experimental-0.98.0/LICENSE` & `cognite-sdk-experimental-0.99.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite-sdk-experimental-0.98.0/cognite/experimental/_api/alerts.py` & `cognite-sdk-experimental-0.99.0/cognite/experimental/_api/alerts.py`

 * *Files identical despite different names*

### Comparing `cognite-sdk-experimental-0.98.0/cognite/experimental/_api/annotations.py` & `cognite-sdk-experimental-0.99.0/cognite/experimental/_api/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite-sdk-experimental-0.98.0/cognite/experimental/_api/document_parsing.py` & `cognite-sdk-experimental-0.99.0/cognite/experimental/_api/document_parsing.py`

 * *Files identical despite different names*

### Comparing `cognite-sdk-experimental-0.98.0/cognite/experimental/_api/entity_matching.py` & `cognite-sdk-experimental-0.99.0/cognite/experimental/_api/entity_matching.py`

 * *Files identical despite different names*

### Comparing `cognite-sdk-experimental-0.98.0/cognite/experimental/_api/extractionpipelines.py` & `cognite-sdk-experimental-0.99.0/cognite/experimental/_api/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite-sdk-experimental-0.98.0/cognite/experimental/_api/geospatial.py` & `cognite-sdk-experimental-0.99.0/cognite/experimental/_api/geospatial.py`

 * *Files 2% similar despite different names*

```diff
@@ -358,24 +358,26 @@
 
     @_with_cognite_domain
     def compute(
         self,
         sub_computes: Dict[str, Any] = None,
         from_feature_type: str = None,
         filter: Dict[str, Any] = None,
+        group_by: List[Dict[str, Any]] = None,
         output: Dict[str, Any] = None,
         binary_output: Dict[str, Any] = None,
     ) -> Union[bytes, ComputedItemList]:
         """`Compute something`
         <https://pr-1717.specs.preview.cogniteapp.com/v1.json.html#operation/compute>
 
         Args:
             sub_computes (Dict[str, Any]): the sub-computed data for the main compute
             from_feature_type (str): the main feature type external id to compute from
             filter (Dict[str, Any]): the filter for the main feature type
+            group_by (List[Dict[str, Any]]): the list of group by expressions
             output (Dict[str, Any]): the output json spec
             binary_output (Dict[str, Any]): the binary output computation to execute
 
         Returns:
             Union[bytes,List[ComputedItem]]
 
         Examples:
@@ -437,22 +439,24 @@
                 ...         "from4326to102016": {"stTransform": {"geometry": {"ref": "paris"}, "srid": 102016}},
                 ...     }
                 ... )
         """
         sub_computes_json = {"subComputes": sub_computes} if sub_computes is not None else {}
         from_feature_type_json = {"fromFeatureType": from_feature_type} if from_feature_type is not None else {}
         filter_json = {"filter": filter} if filter is not None else {}
+        group_by_json = {"groupBy": group_by} if group_by is not None else {}
         output_json = {"output": output} if output is not None else {}
         binary_output_json = {"binaryOutput": binary_output} if binary_output is not None else {}
         res = self._post(
             url_path=GeospatialAPI._RESOURCE_PATH + "/compute",
             json={
                 **sub_computes_json,
                 **from_feature_type_json,
                 **filter_json,
+                **group_by_json,
                 **output_json,
                 **binary_output_json,
             },
         )
         content_type = res.headers["Content-Type"].split(";")[0]
         if content_type == "application/json":
             return ComputedItemList._load(res.json()["items"], cognite_client=self._cognite_client)
```

### Comparing `cognite-sdk-experimental-0.98.0/cognite/experimental/_api/legacy_annotations.py` & `cognite-sdk-experimental-0.99.0/cognite/experimental/_api/legacy_annotations.py`

 * *Files identical despite different names*

### Comparing `cognite-sdk-experimental-0.98.0/cognite/experimental/_api/match_rules.py` & `cognite-sdk-experimental-0.99.0/cognite/experimental/_api/match_rules.py`

 * *Files identical despite different names*

### Comparing `cognite-sdk-experimental-0.98.0/cognite/experimental/_api/pnid_object_detection.py` & `cognite-sdk-experimental-0.99.0/cognite/experimental/_api/pnid_object_detection.py`

 * *Files identical despite different names*

### Comparing `cognite-sdk-experimental-0.98.0/cognite/experimental/_api/pnid_parsing.py` & `cognite-sdk-experimental-0.99.0/cognite/experimental/_api/pnid_parsing.py`

 * *Files identical despite different names*

### Comparing `cognite-sdk-experimental-0.98.0/cognite/experimental/_api/templatecompletion.py` & `cognite-sdk-experimental-0.99.0/cognite/experimental/_api/templatecompletion.py`

 * *Files identical despite different names*

### Comparing `cognite-sdk-experimental-0.98.0/cognite/experimental/_client.py` & `cognite-sdk-experimental-0.99.0/cognite/experimental/_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from cognite.experimental._api.extractionpipelines import ExperimentalExtractionPipelinesAPI
 from cognite.experimental._api.geospatial import ExperimentalGeospatialAPI
 from cognite.experimental._api.legacy_annotations import LegacyAnnotationsAPI
 from cognite.experimental._api.match_rules import MatchRulesAPI
 from cognite.experimental._api.pnid_object_detection import PNIDObjectDetectionAPI
 from cognite.experimental._api.pnid_parsing import PNIDParsingAPI
 from cognite.experimental._api.templatecompletion import ExperimentalTemplatesAPI
-from cognite.experimental._api.vision import VisionAPI
 
 APIClient.RETRYABLE_POST_ENDPOINTS |= {
     f"/{api}/{endpoint}" for api in ["types", "labels", "templates"] for endpoint in ["list", "byids", "search"]
 }
 
 
 class CogniteClient(Client):
@@ -98,8 +97,7 @@
 
         self.extraction_pipelines = ExperimentalExtractionPipelinesAPI(
             self._config, api_version="playground", cognite_client=self
         )
 
         # template completion only
         self.templates = ExperimentalTemplatesAPI(self._config, api_version=self._API_VERSION, cognite_client=self)
-        self.vision = VisionAPI(self._config, api_version="playground", cognite_client=self)
```

### Comparing `cognite-sdk-experimental-0.98.0/cognite/experimental/_context_client.py` & `cognite-sdk-experimental-0.99.0/cognite/experimental/_context_client.py`

 * *Files identical despite different names*

### Comparing `cognite-sdk-experimental-0.98.0/cognite/experimental/data_classes/alerts.py` & `cognite-sdk-experimental-0.99.0/cognite/experimental/data_classes/alerts.py`

 * *Files identical despite different names*

### Comparing `cognite-sdk-experimental-0.98.0/cognite/experimental/data_classes/annotations.py` & `cognite-sdk-experimental-0.99.0/cognite/experimental/data_classes/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite-sdk-experimental-0.98.0/cognite/experimental/data_classes/contextualization.py` & `cognite-sdk-experimental-0.99.0/cognite/experimental/data_classes/contextualization.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
 from cognite.experimental.data_classes.utils.pandas import dataframe_summarize
 from cognite.experimental.data_classes.utils.rules_output import _color_matches, _label_groups
 
 
 class ContextualizationJobType(Enum):
     PNID_PARSER = "pnid_parsing"
-    VISION = "vision"
 
 
 class EntityMatchingMatchRule(CogniteResource):
     def __init__(
         self,
         conditions=None,
         extractors=None,
```

### Comparing `cognite-sdk-experimental-0.98.0/cognite/experimental/data_classes/extractionpipelines.py` & `cognite-sdk-experimental-0.99.0/cognite/experimental/data_classes/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite-sdk-experimental-0.98.0/cognite/experimental/data_classes/geospatial.py` & `cognite-sdk-experimental-0.99.0/cognite/experimental/data_classes/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite-sdk-experimental-0.98.0/cognite/experimental/data_classes/legacy_annotations.py` & `cognite-sdk-experimental-0.99.0/cognite/experimental/data_classes/legacy_annotations.py`

 * *Files identical despite different names*

### Comparing `cognite-sdk-experimental-0.98.0/cognite/experimental/data_classes/model_hosting/models.py` & `cognite-sdk-experimental-0.99.0/cognite/experimental/data_classes/model_hosting/models.py`

 * *Files identical despite different names*

### Comparing `cognite-sdk-experimental-0.98.0/cognite/experimental/data_classes/model_hosting/schedules.py` & `cognite-sdk-experimental-0.99.0/cognite/experimental/data_classes/model_hosting/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite-sdk-experimental-0.98.0/cognite/experimental/data_classes/model_hosting/source_packages.py` & `cognite-sdk-experimental-0.99.0/cognite/experimental/data_classes/model_hosting/source_packages.py`

 * *Files identical despite different names*

### Comparing `cognite-sdk-experimental-0.98.0/cognite/experimental/data_classes/model_hosting/versions.py` & `cognite-sdk-experimental-0.99.0/cognite/experimental/data_classes/model_hosting/versions.py`

 * *Files identical despite different names*

### Comparing `cognite-sdk-experimental-0.98.0/cognite/experimental/data_classes/shared.py` & `cognite-sdk-experimental-0.99.0/cognite/experimental/data_classes/shared.py`

 * *Files identical despite different names*

### Comparing `cognite-sdk-experimental-0.98.0/cognite/experimental/data_classes/types.py` & `cognite-sdk-experimental-0.99.0/cognite/experimental/data_classes/types.py`

 * *Files identical despite different names*

### Comparing `cognite-sdk-experimental-0.98.0/cognite/experimental/data_classes/utils/rules_output.py` & `cognite-sdk-experimental-0.99.0/cognite/experimental/data_classes/utils/rules_output.py`

 * *Files identical despite different names*

### Comparing `cognite-sdk-experimental-0.98.0/cognite/experimental/utils.py` & `cognite-sdk-experimental-0.99.0/cognite/experimental/utils.py`

 * *Files identical despite different names*

### Comparing `cognite-sdk-experimental-0.98.0/pyproject.toml` & `cognite-sdk-experimental-0.99.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "cognite-sdk-experimental"
 
-version = "0.98.0"
+version = "0.99.0"
 
 description = "Experimental additions to the Python SDK"
 authors = ["Sander Land <sander.land@cognite.com>"]
 
 packages = [
     { include="cognite", from="." },
 ]
```

### Comparing `cognite-sdk-experimental-0.98.0/setup.py` & `cognite-sdk-experimental-0.99.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 {'': '.'}
 
 packages = \
 ['cognite',
  'cognite.experimental',
  'cognite.experimental._api',
  'cognite.experimental.data_classes',
- 'cognite.experimental.data_classes.annotation_types',
  'cognite.experimental.data_classes.model_hosting',
  'cognite.experimental.data_classes.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
@@ -25,15 +24,15 @@
  'typing-extensions>=3.7.4,<5']
 
 extras_require = \
 {'geopandas': ['geopandas>=0.10.0', 'shapely>=1.7.0']}
 
 setup_kwargs = {
     'name': 'cognite-sdk-experimental',
-    'version': '0.98.0',
+    'version': '0.99.0',
     'description': 'Experimental additions to the Python SDK',
     'long_description': 'None',
     'author': 'Sander Land',
     'author_email': 'sander.land@cognite.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `cognite-sdk-experimental-0.98.0/PKG-INFO` & `cognite-sdk-experimental-0.99.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-sdk-experimental
-Version: 0.98.0
+Version: 0.99.0
 Summary: Experimental additions to the Python SDK
 Author: Sander Land
 Author-email: sander.land@cognite.com
 Requires-Python: >=3.8,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

