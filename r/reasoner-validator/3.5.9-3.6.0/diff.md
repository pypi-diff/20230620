# Comparing `tmp/reasoner_validator-3.5.9.tar.gz` & `tmp/reasoner_validator-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner_validator-3.5.9.tar", max compression
+gzip compressed data, was "reasoner_validator-3.6.0.tar", max compression
```

## Comparing `reasoner_validator-3.5.9.tar` & `reasoner_validator-3.6.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1153 2023-06-16 22:06:08.171870 reasoner_validator-3.5.9/LICENSE
--rw-r--r--   0        0        0    12606 2023-06-16 22:06:08.171870 reasoner_validator-3.5.9/README.md
--rw-r--r--   0        0        0      131 2023-06-16 22:06:08.171870 reasoner_validator-3.5.9/docs/.nojekyll
--rw-r--r--   0        0        0      634 2023-06-16 22:06:08.171870 reasoner_validator-3.5.9/docs/Makefile
--rw-r--r--   0        0        0     2291 2023-06-16 22:06:08.171870 reasoner_validator-3.5.9/docs/conf.py
--rw-r--r--   0        0        0    19034 2023-06-16 22:06:08.171870 reasoner_validator-3.5.9/docs/index.rst
--rw-r--r--   0        0        0      795 2023-06-16 22:06:08.171870 reasoner_validator-3.5.9/docs/make.bat
--rw-r--r--   0        0        0      136 2023-06-16 22:06:08.171870 reasoner_validator-3.5.9/docs/reasoner_validator.biolink.rst
--rw-r--r--   0        0        0      135 2023-06-16 22:06:08.171870 reasoner_validator-3.5.9/docs/reasoner_validator.report.rst
--rw-r--r--   0        0        0      142 2023-06-16 22:06:08.171870 reasoner_validator-3.5.9/docs/reasoner_validator.rst
--rw-r--r--   0        0        0      146 2023-06-16 22:06:08.171870 reasoner_validator-3.5.9/docs/reasoner_validator.trapi.mapping.rst
--rw-r--r--   0        0        0      144 2023-06-16 22:06:08.171870 reasoner_validator-3.5.9/docs/reasoner_validator.trapi.rst
--rw-r--r--   0        0        0      163 2023-06-16 22:06:08.171870 reasoner_validator-3.5.9/docs/reasoner_validator.validation_codes.rst
--rw-r--r--   0        0        0      157 2023-06-16 22:06:08.171870 reasoner_validator-3.5.9/docs/reasoner_validator.versioning.rst
--rw-r--r--   0        0        0    35674 2023-06-16 22:06:08.171870 reasoner_validator-3.5.9/docs/validation_codes_dictionary.md
--rw-r--r--   0        0        0     2093 2023-06-16 22:06:08.171870 reasoner_validator-3.5.9/pyproject.toml
--rw-r--r--   0        0        0    34621 2023-06-16 22:06:08.171870 reasoner_validator-3.5.9/reasoner_validator/__init__.py
--rw-r--r--   0        0        0    62655 2023-06-16 22:06:08.171870 reasoner_validator-3.5.9/reasoner_validator/biolink/__init__.py
--rw-r--r--   0        0        0    38874 2023-06-16 22:06:08.171870 reasoner_validator-3.5.9/reasoner_validator/codes.yaml
--rw-r--r--   0        0        0    26862 2023-06-16 22:06:08.171870 reasoner_validator-3.5.9/reasoner_validator/report.py
--rw-r--r--   0        0        0        0 2023-06-16 22:06:08.171870 reasoner_validator-3.5.9/reasoner_validator/sri/__init__.py
--rw-r--r--   0        0        0     4350 2023-06-16 22:06:08.171870 reasoner_validator-3.5.9/reasoner_validator/sri/util.py
--rw-r--r--   0        0        0     9718 2023-06-16 22:06:08.175870 reasoner_validator-3.5.9/reasoner_validator/trapi/__init__.py
--rw-r--r--   0        0        0     1105 2023-06-16 22:06:08.175870 reasoner_validator-3.5.9/reasoner_validator/trapi/mapping.py
--rw-r--r--   0        0        0    13781 2023-06-16 22:06:08.175870 reasoner_validator-3.5.9/reasoner_validator/validation_codes.py
--rw-r--r--   0        0        0     9922 2023-06-16 22:06:08.175870 reasoner_validator-3.5.9/reasoner_validator/versioning.py
--rw-r--r--   0        0        0        0 2023-06-16 22:06:08.175870 reasoner_validator-3.5.9/tests/__init__.py
--rw-r--r--   0        0        0       37 2023-06-16 22:06:08.175870 reasoner_validator-3.5.9/tests/conftest.py
--rw-r--r--   0        0        0   114174 2023-06-16 22:06:08.175870 reasoner_validator-3.5.9/tests/test_biolink_compliance_validation.py
--rw-r--r--   0        0        0    42178 2023-06-16 22:06:08.175870 reasoner_validator-3.5.9/tests/test_data/sample_trapi_schema.yaml
--rw-r--r--   0        0        0    31899 2023-06-16 22:06:08.175870 reasoner_validator-3.5.9/tests/test_response_validator.py
--rw-r--r--   0        0        0     4533 2023-06-16 22:06:08.175870 reasoner_validator-3.5.9/tests/test_semver.py
--rw-r--r--   0        0        0     1746 2023-06-16 22:06:08.175870 reasoner_validator-3.5.9/tests/test_trapi_versioning.py
--rw-r--r--   0        0        0    26543 2023-06-16 22:06:08.175870 reasoner_validator-3.5.9/tests/test_validate.py
--rw-r--r--   0        0        0    19013 2023-06-16 22:06:08.175870 reasoner_validator-3.5.9/tests/test_validation_report.py
--rw-r--r--   0        0        0     2061 2023-06-16 22:06:08.175870 reasoner_validator-3.5.9/tests/test_workflows.py
--rw-r--r--   0        0        0    14645 1970-01-01 00:00:00.000000 reasoner_validator-3.5.9/PKG-INFO
+-rw-r--r--   0        0        0     1153 2023-06-19 22:45:22.744411 reasoner_validator-3.6.0/LICENSE
+-rw-r--r--   0        0        0    12606 2023-06-19 22:45:22.744411 reasoner_validator-3.6.0/README.md
+-rw-r--r--   0        0        0      131 2023-06-19 22:45:22.744411 reasoner_validator-3.6.0/docs/.nojekyll
+-rw-r--r--   0        0        0      634 2023-06-19 22:45:22.744411 reasoner_validator-3.6.0/docs/Makefile
+-rw-r--r--   0        0        0     2291 2023-06-19 22:45:22.744411 reasoner_validator-3.6.0/docs/conf.py
+-rw-r--r--   0        0        0    19034 2023-06-19 22:45:22.744411 reasoner_validator-3.6.0/docs/index.rst
+-rw-r--r--   0        0        0      795 2023-06-19 22:45:22.744411 reasoner_validator-3.6.0/docs/make.bat
+-rw-r--r--   0        0        0      136 2023-06-19 22:45:22.744411 reasoner_validator-3.6.0/docs/reasoner_validator.biolink.rst
+-rw-r--r--   0        0        0      135 2023-06-19 22:45:22.744411 reasoner_validator-3.6.0/docs/reasoner_validator.report.rst
+-rw-r--r--   0        0        0      142 2023-06-19 22:45:22.744411 reasoner_validator-3.6.0/docs/reasoner_validator.rst
+-rw-r--r--   0        0        0      146 2023-06-19 22:45:22.744411 reasoner_validator-3.6.0/docs/reasoner_validator.trapi.mapping.rst
+-rw-r--r--   0        0        0      144 2023-06-19 22:45:22.744411 reasoner_validator-3.6.0/docs/reasoner_validator.trapi.rst
+-rw-r--r--   0        0        0      163 2023-06-19 22:45:22.744411 reasoner_validator-3.6.0/docs/reasoner_validator.validation_codes.rst
+-rw-r--r--   0        0        0      157 2023-06-19 22:45:22.744411 reasoner_validator-3.6.0/docs/reasoner_validator.versioning.rst
+-rw-r--r--   0        0        0    35697 2023-06-19 22:45:22.748411 reasoner_validator-3.6.0/docs/validation_codes_dictionary.md
+-rw-r--r--   0        0        0     2093 2023-06-19 22:45:22.748411 reasoner_validator-3.6.0/pyproject.toml
+-rw-r--r--   0        0        0    36530 2023-06-19 22:45:22.748411 reasoner_validator-3.6.0/reasoner_validator/__init__.py
+-rw-r--r--   0        0        0    62655 2023-06-19 22:45:22.748411 reasoner_validator-3.6.0/reasoner_validator/biolink/__init__.py
+-rw-r--r--   0        0        0    38939 2023-06-19 22:45:22.748411 reasoner_validator-3.6.0/reasoner_validator/codes.yaml
+-rw-r--r--   0        0        0    28533 2023-06-19 22:45:22.748411 reasoner_validator-3.6.0/reasoner_validator/report.py
+-rw-r--r--   0        0        0        0 2023-06-19 22:45:22.748411 reasoner_validator-3.6.0/reasoner_validator/sri/__init__.py
+-rw-r--r--   0        0        0     4350 2023-06-19 22:45:22.748411 reasoner_validator-3.6.0/reasoner_validator/sri/util.py
+-rw-r--r--   0        0        0     9721 2023-06-19 22:45:22.748411 reasoner_validator-3.6.0/reasoner_validator/trapi/__init__.py
+-rw-r--r--   0        0        0     1105 2023-06-19 22:45:22.748411 reasoner_validator-3.6.0/reasoner_validator/trapi/mapping.py
+-rw-r--r--   0        0        0    13807 2023-06-19 22:45:22.748411 reasoner_validator-3.6.0/reasoner_validator/validation_codes.py
+-rw-r--r--   0        0        0    10201 2023-06-19 22:45:22.748411 reasoner_validator-3.6.0/reasoner_validator/versioning.py
+-rw-r--r--   0        0        0        0 2023-06-19 22:45:22.748411 reasoner_validator-3.6.0/tests/__init__.py
+-rw-r--r--   0        0        0       37 2023-06-19 22:45:22.748411 reasoner_validator-3.6.0/tests/conftest.py
+-rw-r--r--   0        0        0   114356 2023-06-19 22:45:22.748411 reasoner_validator-3.6.0/tests/test_biolink_compliance_validation.py
+-rw-r--r--   0        0        0    42178 2023-06-19 22:45:22.748411 reasoner_validator-3.6.0/tests/test_data/sample_trapi_schema.yaml
+-rw-r--r--   0        0        0    34156 2023-06-19 22:45:22.748411 reasoner_validator-3.6.0/tests/test_response_validator.py
+-rw-r--r--   0        0        0     5162 2023-06-19 22:45:22.748411 reasoner_validator-3.6.0/tests/test_semver.py
+-rw-r--r--   0        0        0     1746 2023-06-19 22:45:22.748411 reasoner_validator-3.6.0/tests/test_trapi_versioning.py
+-rw-r--r--   0        0        0    26543 2023-06-19 22:45:22.752411 reasoner_validator-3.6.0/tests/test_validate.py
+-rw-r--r--   0        0        0    20400 2023-06-19 22:45:22.752411 reasoner_validator-3.6.0/tests/test_validation_report.py
+-rw-r--r--   0        0        0     2061 2023-06-19 22:45:22.752411 reasoner_validator-3.6.0/tests/test_workflows.py
+-rw-r--r--   0        0        0    14645 1970-01-01 00:00:00.000000 reasoner_validator-3.6.0/PKG-INFO
```

### Comparing `reasoner_validator-3.5.9/LICENSE` & `reasoner_validator-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.9/README.md` & `reasoner_validator-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.9/docs/Makefile` & `reasoner_validator-3.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.9/docs/conf.py` & `reasoner_validator-3.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.9/docs/index.rst` & `reasoner_validator-3.6.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.9/docs/make.bat` & `reasoner_validator-3.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.9/docs/validation_codes_dictionary.md` & `reasoner_validator-3.6.0/docs/validation_codes_dictionary.md`

 * *Files 1% similar despite different names*

```diff
@@ -272,52 +272,28 @@
 
 **Context:** edge_id, identifier, kp_source_type
 
 **Description:** Edge attributes of ARAs and KPs should record the infores identifier of their knowledge source provenance with respect to KP.
 
 ## Error
 
-### error.non_compliant
+### error.biolink.model.noncompliance
 
 **Message:** S-P-O statement is not compliant to Biolink Model release
 
 **Context:** identifier, biolink_release
 
 **Description:** This knowledge statement is not compliant to the specified release of the Biolink Model. Review associated messages for underlying cause!
 
-### error.trapi.validation
-
-**Message:** Schema validation error
-
-**Context:** identifier, component, reason
-
-**Description:** JSON Schema validation error reported for specified TRAPI query component.
-
-### error.trapi.request.invalid
-
-**Message:** Test could not generate a valid TRAPI query request object using identified element
-
-**Context:** identifier, test, reason
-
-**Description:** Specified TRAPI query unit 'test' query could not be prepared for the indicated reason, using the identified Biolink starting element.
-
 ### error.trapi.response.empty
 
 **Message:** TRAPI Response is missing!
 
 **Description:** TRAPI Response to be validated should not be totally empty but should have a Message body.
 
-### error.trapi.response.unexpected_http_code
-
-**Message:** TRAPI Response has an unexpected HTTP status code
-
-**Context:** identifier
-
-**Description:** TRAPI query attempt returned an abnormal (non-200) server HTTP status code as noted.
-
 ### error.trapi.response.message.empty
 
 **Message:** TRAPI Response missing its Message!
 
 **Description:** TRAPI response should at least have non-empty original TRAPI request Message in its reply.
 
 ### error.trapi.response.query_graph.missing
@@ -1038,7 +1014,33 @@
 
 **Message:** Empty 'resource_role' property in Edge
 
 **Context:** identifier
 
 **Description:** Value of the 'resource_role' property in the RetrievalSource of a Knowledge Graph Edge must be a non-empty ResourceRole enum value!
 
+## Critical
+
+### critical.trapi.validation
+
+**Message:** Schema validation error
+
+**Context:** identifier, component, reason
+
+**Description:** Critical JSON Schema validation error reported for specified TRAPI query component.
+
+### critical.trapi.request.invalid
+
+**Message:** Test could not generate a valid TRAPI query request object using identified element
+
+**Context:** identifier, test, reason
+
+**Description:** Specified TRAPI query unit 'test' query could not be prepared for the indicated reason, using the identified Biolink starting element.
+
+### critical.trapi.response.unexpected_http_code
+
+**Message:** Unexpected HTTP status code
+
+**Context:** identifier
+
+**Description:** TRAPI query attempt returned an abnormal (non-200) server HTTP status code as noted.
+
```

### Comparing `reasoner_validator-3.5.9/pyproject.toml` & `reasoner_validator-3.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reasoner-validator"
-version = "3.5.9"
+version = "3.6.0"
 description = "Validation tools for Reasoner API"
 authors = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
     "Patrick Wang <patrickelvin@gmail.com>"
 ]
 maintainers = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
```

### Comparing `reasoner_validator-3.5.9/reasoner_validator/__init__.py` & `reasoner_validator-3.6.0/reasoner_validator/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,19 @@
 
 class TRAPIResponseValidator(ValidationReporter):
     """
     TRAPI Validator is an overall wrapper class for validating
     conformance of TRAPI Responses to TRAPI and the Biolink Model.
     """
 
+    TRAPI_1_3_0 = SemVer.from_string("1.3.0")
+    TRAPI_1_4_0 = SemVer.from_string("1.4.0")
+    TRAPI_1_4_0_BETA3 = SemVer.from_string("1.4.0-beta3")
+    TRAPI_1_4_0_BETA4 = SemVer.from_string("1.4.0-beta4")
+
     def __init__(
             self,
             trapi_version: Optional[str] = None,
             biolink_version: Optional[str] = None,
             sources: Optional[Dict] = None,
             strict_validation: bool = False,
             suppress_empty_data_warnings: bool = False
@@ -57,21 +62,45 @@
             trapi_version=trapi_version,
             biolink_version=biolink_version,
             sources=sources,
             strict_validation=strict_validation
         )
         self.suppress_empty_data_warnings = suppress_empty_data_warnings
 
-    def sanitize_trapi_query(self, response: Dict) -> Dict:
+    def sanitize_trapi_response(self, response: Dict) -> Dict:
         """
+        Some component TRAPI Responses cannot be validated further due to missing tags and None values.
+        This method is a temporary workaround to sanitize the query for additional validation.
 
         :param response: Dict full TRAPI Response JSON object
         :return: Dict, response with discretionary removal of content which
                        triggers (temporarily) unwarranted TRAPI validation failures
         """
+        # Temporary workaround for "1.4.0-beta4" schema bugs
+        current_version: SemVer = SemVer.from_string(self.trapi_version)
+        # the message is not empty
+        if 'knowledge_graph' in response['message'] and response['message']['knowledge_graph'] is not None and \
+                self.TRAPI_1_4_0_BETA4 >= current_version != self.TRAPI_1_3_0:
+            for key, edge in response['message']['knowledge_graph']['edges'].items():
+                edge_id = f"{str(edge['subject'])}--{str(edge['predicate'])}->{str(str(edge['object']))}"
+                if 'sources' not in edge or not edge['sources']:
+                    self.report("error.knowledge_graph.edge.sources.missing", identifier=edge_id)
+                    continue
+                for source in edge['sources']:
+                    if 'source_record_urls' not in source or source['source_record_urls'] is None:
+                        source['source_record_urls'] = list()
+                    if 'upstream_resource_ids' not in source or source['upstream_resource_ids'] is None:
+                        source['upstream_resource_ids'] = list()
+
+        # 'auxiliary_graphs' (from TRAPI 1.4.0-beta3 onwards)
+        # ought to be nullable, however... not specified that way (yet)
+        if current_version >= self.TRAPI_1_4_0_BETA3 and \
+                ('auxiliary_graphs' not in response['message'] or response['message']['auxiliary_graphs'] is None):
+            response['message']['auxiliary_graphs'] = dict()
+
         if 'workflow' in response and response['workflow']:
             # a 'workflow' is a list of steps, which are JSON object specifications
             workflow_steps: List[Dict] = response['workflow']
             for step in workflow_steps:
                 if 'runner_parameters' in step and not step['runner_parameters']:
                     self.report("warning.trapi.response.workflow.runner_parameters.null")
                     step.pop('runner_parameters')
@@ -121,15 +150,15 @@
         if not message:
             if not self.suppress_empty_data_warnings:
                 self.report("error.trapi.response.message.empty")
 
             # ... also, nothing more here to validate?
             return
 
-        response = self.sanitize_trapi_query(response)
+        response = self.sanitize_trapi_response(response)
 
         trapi_validator: TRAPISchemaValidator = check_trapi_validity(
             instance=response,
             component="Response",
             trapi_version=self.trapi_version
         )
         if trapi_validator.has_messages():
```

### Comparing `reasoner_validator-3.5.9/reasoner_validator/biolink/__init__.py` & `reasoner_validator-3.6.0/reasoner_validator/biolink/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.9/reasoner_validator/codes.yaml` & `reasoner_validator-3.6.0/reasoner_validator/codes.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -238,45 +238,27 @@
             $context:
               - edge_id
               - identifier
               - kp_source_type
             $description: "Edge attributes of ARAs and KPs should record the infores identifier of their knowledge source provenance with respect to KP."
 
 error:
-  non_compliant:
-    $message: "S-P-O statement is not compliant to Biolink Model release"
-    $context:
-      - identifier
-      - biolink_release
-    $description: "This knowledge statement is not compliant to the specified release of the Biolink Model. Review associated messages for underlying cause!"
-  trapi:
-    validation:
-      $message: "Schema validation error"
-      $context:
-        - identifier
-        - component
-        - reason
-      $description: "JSON Schema validation error reported for specified TRAPI query component."
-    request:
-      invalid:
-        $message: "Test could not generate a valid TRAPI query request object using identified element"
+  biolink:
+    model:
+      noncompliance:
+        $message: "S-P-O statement is not compliant to Biolink Model release"
         $context:
           - identifier
-          - test
-          - reason
-        $description: "Specified TRAPI query unit 'test' query could not be prepared for the indicated reason, using the identified Biolink starting element."
+          - biolink_release
+        $description: "This knowledge statement is not compliant to the specified release of the Biolink Model. Review associated messages for underlying cause!"
+  trapi:
     response:
       empty:
         $message: "TRAPI Response is missing!"
         $description: "TRAPI Response to be validated should not be totally empty but should have a Message body."
-      unexpected_http_code:
-        $message: "TRAPI Response has an unexpected HTTP status code"
-        $context:
-          - identifier
-        $description: "TRAPI query attempt returned an abnormal (non-200) server HTTP status code as noted."
       message:
         empty:
           $message: "TRAPI Response missing its Message!"
           $description: "TRAPI response should at least have non-empty original TRAPI request Message in its reply."
       query_graph:
         missing:
           $message: "TRAPI Message is missing its Query Graph!"
@@ -819,7 +801,30 @@
                 $description: "A 'retrieval_source.upstream_resource_ids' values must be registered infores identifiers!"
           resource_role:
             empty:
               $message: "Empty 'resource_role' property in Edge"
               $context:
                 - identifier
               $description: "Value of the 'resource_role' property in the RetrievalSource of a Knowledge Graph Edge must be a non-empty ResourceRole enum value!"
+critical:
+  trapi:
+    validation:
+      $message: "Schema validation error"
+      $context:
+        - identifier
+        - component
+        - reason
+      $description: "Critical JSON Schema validation error reported for specified TRAPI query component."
+    request:
+      invalid:
+        $message: "Test could not generate a valid TRAPI query request object using identified element"
+        $context:
+          - identifier
+          - test
+          - reason
+        $description: "Specified TRAPI query unit 'test' query could not be prepared for the indicated reason, using the identified Biolink starting element."
+    response:
+      unexpected_http_code:
+        $message: "Unexpected HTTP status code"
+        $context:
+          - identifier
+        $description: "TRAPI query attempt returned an abnormal (non-200) server HTTP status code as noted."
```

### Comparing `reasoner_validator-3.5.9/reasoner_validator/report.py` & `reasoner_validator-3.6.0/reasoner_validator/report.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,27 +27,28 @@
 
 def _output(json, flat=False):
     return dumps(json, cls=ReportJsonEncoder, sort_keys=False, indent=None if flat else 4)
 
 
 class ValidationReporter:
     """
-    General wrapper for managing validation status messages: information, warnings and errors.
-    The TRAPI version and Biolink Model versions are also tracked for convenience at
-    this abstract level although their application is within specific pertinent subclasses.
+    General wrapper for managing validation status messages: information, warnings, errors and 'critical' (errors).
+    The TRAPI version and Biolink Model versions are also tracked for convenience at this abstract level
+    although their application is within specific pertinent subclasses.
     """
 
     # Default major version resolves to latest TRAPI OpenAPI release,
     # specifically 1.3.0, as of September 1st, 2022
     DEFAULT_TRAPI_VERSION = "1"
 
     _message_type_name: Dict[str, str] = {
         "info": "information",
         "warning": "warnings",
-        "error": "errors"
+        "error": "errors",
+        "critical": "critical"
     }
 
     def __init__(
             self,
             prefix: Optional[str] = None,
             trapi_version: Optional[str] = None,
             biolink_version: Optional[str] = None,
@@ -93,18 +94,21 @@
         #     },
         #     "warnings":  {
         #       ...<similar to information data structure above>
         #     },
         #     "errors": {
         #       ...<similar to information data structure above>
         #     },
+        #     "critical": {
+        #       ...<similar to information data structure above>
+        #     }
         # }
         #
         self.messages: Dict[
-            str,  # message type (errors/warnings/information)
+            str,  # message type (critical/errors/warnings/information)
             Dict[
                 str,  # message 'code' as indexing key
                 # Dictionary of 'identifier' indexed messages with parameters
                 # (Maybe None, if code doesn't have any additional parameters)
                 Optional[
                     Dict[
                         str,  # key is the message-unique template 'identifier' value of parameterized messages
@@ -115,14 +119,15 @@
                                 Dict[str, str]
                             ]
                         ]
                     ]
                 ]
             ]
         ] = {
+            "critical": dict(),
             "errors": dict(),
             "warnings": dict(),
             "information": dict()
         }
 
     def get_trapi_version(self) -> str:
         """
@@ -166,15 +171,15 @@
         """
         return self.strict_validation
 
     def has_messages(self) -> bool:
         """Predicate to detect any recorded validation messages.
         :return: bool, True if ValidationReporter has any non-empty messages.
         """
-        return self.has_information() or self.has_warnings() or self.has_errors()
+        return self.has_information() or self.has_warnings() or self.has_errors() or self.has_critical()
 
     def has_information(self) -> bool:
         """Predicate to detect any recorded information messages.
         :return: bool, True if ValidationReporter has any information messages.
         """
         return bool(self.messages["information"])
 
@@ -186,14 +191,20 @@
 
     def has_errors(self) -> bool:
         """Predicate to detect any recorded error messages.
         :return: bool, True if ValidationReporter has any error messages.
         """
         return bool(self.messages["errors"])
 
+    def has_critical(self) -> bool:
+        """Predicate to detect any recorded critical error messages.
+        :return: bool, True if ValidationReporter has any critical error messages.
+        """
+        return bool(self.messages["critical"])
+
     def dump_info(self, flat=False) -> str:
         """Dump information messages as JSON.
         :param flat: render output as 'flat' JSON (default: False)
         :return: str, JSON formatted string of information messages.
         """
         return _output(self.messages["information"], flat)
 
@@ -207,30 +218,37 @@
     def dump_errors(self, flat=False) -> str:
         """Dump error messages as JSON.
         :param flat: render output as 'flat' JSON (default: False)
         :return: str, JSON formatted string of error messages.
         """
         return _output(self.messages["errors"], flat)
 
+    def dump_critical(self, flat=False) -> str:
+        """Dump critical error messages as JSON.
+        :param flat: render output as 'flat' JSON (default: False)
+        :return: str, JSON formatted string of critical error messages.
+        """
+        return _output(self.messages["critical"], flat)
+
     def dump_messages(self, flat=False) -> str:
         """Dump all messages as JSON.
         :param flat: render output as 'flat' JSON (default: False)
         :return: str, JSON formatted string of all messages.
         """
         return _output(self.messages, flat)
 
     @staticmethod
     def get_message_type(code: str) -> str:
         """Get type of message code.
         :param code: message code
-        :return: message type, one of 'info', 'warning' or 'error'
+        :return: message type, one of 'info', 'warning', 'error' or 'critical'
         """
         code_id_parts: List[str] = code.split('.')
         message_type: str = code_id_parts[0]
-        if message_type in ['info', 'warning', 'error']:
+        if message_type in ['info', 'warning', 'error', 'critical']:
             return message_type
         else:
             raise NotImplementedError(
                 f"ValidationReport.get_message_type(): {code} is unknown code type: {message_type}"
             )
 
     def report(self, code: str, **message):
@@ -267,30 +285,30 @@
                         self.messages[message_type][code][message_identifier] = list()
 
                     self.messages[message_type][code][message_identifier].append(message)
 
         # else: additional parameters are None
 
     def add_messages(self, new_messages: Dict[
-            str,  # message type (info/warning/error)
+            str,  # message type (info/warning/error/critical)
             Dict[
                 str,  # message 'code' as indexing key
 
                 # List of Dictionaries of parameters
                 # (Maybe None, if specific code doesn't
                 # have additional associated parameters)
                 Optional[Dict[str, Optional[List[Dict[str, str]]]]]
             ]
     ]):
         """
         Batch addition of a dictionary of messages to a ValidationReporter instance.
-        :param new_messages: Dict[str, Dict], with key one of "information", "warnings" or "errors",
+        :param new_messages: Dict[str, Dict], with key one of "information", "warnings", "errors" or "critical",
                               with 'code' keyed dictionaries of (structured) message parameters.
         """
-        for message_type in self.messages:   # 'info', 'warning', 'error'
+        for message_type in self.messages:   # 'info', 'warning', 'error', 'critical'
             if message_type in new_messages:
                 message_type_contents = new_messages[message_type]
                 for code, content in message_type_contents.items():   # codes.yaml message codes
                     if code not in self.messages[message_type]:
                         self.messages[message_type][code] = None
                     if content:
                         # content is of type Dict[str, Optional[List[Dict[str, str]]]]
@@ -335,14 +353,21 @@
     def get_errors(self) -> Dict[str, Optional[Dict[str, Optional[List[Dict[str, str]]]]]]:
         """
         Get copy of all recorded error messages.
         :return: List, copy of all error messages.
         """
         return copy.deepcopy(self.messages["errors"])
 
+    def get_critical(self) -> Dict[str, Optional[Dict[str, Optional[List[Dict[str, str]]]]]]:
+        """
+        Get copy of all recorded critical error messages.
+        :return: List, copy of all critical error messages.
+        """
+        return copy.deepcopy(self.messages["critical"])
+
     ############################
     # General Instance methods #
     ############################
     def merge(self, reporter):
         """
         Merge all messages and metadata from a second ValidationReporter,
         into the calling ValidationReporter instance.
@@ -380,29 +405,30 @@
         :param validation_method: function which accepts this instance of the
                ValidationReporter as its first argument, for use in reporting validation errors.
         :param args: any positional arguments to the validation_method, after the initial ValidationReporter argument
         :param kwargs: any (optional, additional) keyword arguments to the validation_method, after positional arguments
         :return: bool, returns 'False' if validation method documented errors; True otherwise
         """
         validation_method(self, *args, **kwargs)
-        if self.has_errors():
+        # TODO: not sure if we should detect both 'errors' and 'critical' here or just 'critical'
+        if self.has_critical() or self.has_errors():
             return False
         else:
             return True
 
     @staticmethod
     def has_validation_errors(tag: str, case: Dict) -> bool:
         """Check if test case has validation errors.
 
         :param tag: str, top level string key in the 'case' whose value is the validation messages 'dictionary'
         :param case: Dict, containing error messages in a structurally similar
                      format to what is returned by the to_dict() method in this class.
         :return: True if the case contains validation messages
         """
-
+        # TODO: not sure if we should detect both 'errors' and 'critical' here or just 'critical'
         #
         # The 'case' dictionary object could have a format something like this:
         #
         #     tag: {
         #         "trapi_version": "1.3",
         #         "biolink_version": "3.0.2",
         #         "messages": {
@@ -414,24 +440,31 @@
         #                     ]
         #                 }
         #             ],
         #             "errors": [
         #                 {
         #                     "error.knowledge_graph.empty_nodes": None
         #                 }
+        #             ],
+        #             "critical": [
+        #                 {
+        #                     "critical.trapi.validation": None
+        #                 }
         #             ]
         #         }
         #     }
         #
         # where 'tag' == 'messages' and we have a non-empty "errors" set of messages
         #
         if case is not None and tag in case and \
                 'messages' in case[tag] and \
-                'errors' in case[tag]['messages'] and \
-                case[tag]['messages']['errors']:
+                (
+                    'errors' in case[tag]['messages'] and case[tag]['messages']['errors'] or
+                    'critical' in case[tag]['messages'] and case[tag]['messages']['critical']
+                ):
             return True
         else:
             return False
 
     def dump(
             self,
             title: Optional[str] = "",
@@ -472,19 +505,19 @@
                 print(file=file)
             else:
                 # compact also ignores underlining
                 print(title, file=file)
 
         message_type: str
         coded_messages: Dict
-        # Top level partition of messages into 'error', 'warning' or 'info'
+        # Top level partition of messages into 'critical', 'error', 'warning' or 'info'
         for message_type, coded_messages in self.messages.items():
 
             # if there are coded validation messages for a
-            # given message type: 'error', 'warning' or 'info' ...
+            # given message type: 'critical', 'error', 'warning' or 'info' ...
             if coded_messages:
 
                 # ... then iterate through them and print them out
 
                 if not compact_format:
                     print(f"\033[4m{message_type.capitalize()}\033[0m", file=file)
                     print(file=file)
```

### Comparing `reasoner_validator-3.5.9/reasoner_validator/sri/util.py` & `reasoner_validator-3.6.0/reasoner_validator/sri/util.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.9/reasoner_validator/trapi/__init__.py` & `reasoner_validator-3.6.0/reasoner_validator/trapi/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -258,15 +258,15 @@
             )
         except jsonschema.ValidationError as e:
             if len(e.message) <= 160:
                 reason = e.message
             else:
                 reason = e.message[0:49] + " "*5 + "... " + " "*5 + e.message[-100:-1]
             self.report(
-                code="error.trapi.validation",
+                code="critical.trapi.validation",
                 identifier=self.trapi_version,
                 component=component,
                 reason=reason
             )
 
 
 def check_trapi_validity(instance, trapi_version: str, component: str = "Query") -> TRAPISchemaValidator:
```

### Comparing `reasoner_validator-3.5.9/reasoner_validator/trapi/mapping.py` & `reasoner_validator-3.6.0/reasoner_validator/trapi/mapping.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.9/reasoner_validator/validation_codes.py` & `reasoner_validator-3.6.0/reasoner_validator/validation_codes.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,25 +113,25 @@
     def get_code_subtree(
             cls,
             code: str,
             facet: Optional[str] = None,
             is_leaf: Optional[bool] = False
     ) -> Optional[Tuple[str, Dict]]:
         """
-        Get subtree of specified dot-delimited tag name, returned with message type (i.e. info, warning, error).
+        Get subtree of specified dot-delimited tag name, returning message type (i.e. info, warning, error, critical).
         If optional 'is_leaf' flag is set to True, then only return the code if it is a terminal leaf in the code tree.
 
         :param code: Optional[str], dot delimited validation message code identifier (None is ok, but returns None)
         :param facet: Optional[str], constraint on code entry facet to be returned; if specified, should be either
                                      "message" or "description" (default: return all facets of the code entry)
         :param is_leaf: Optional[bool], only return entry if it is a 'leaf' of the code tree (default: False)
 
-        :return: Optional[Tuple[str, Dict[str,str]]], 2-tuple of the code type (i.e. info, warning, error) and the
-                 validation message entry (dictionary); None if empty code or code unknown in the code dictionary,
-                 or (if the is_leaf option is 'True') if the code doesn't resolve to a single leaf.
+        :return: Optional[Tuple[str, Dict[str,str]]], 2-tuple of the code type (i.e. info, warning, error, critical)
+                 and the validation message entry (dictionary); None if empty code or code unknown in the
+                 code dictionary, or (if the is_leaf option is 'True') if the code doesn't resolve to a single leaf.
         """
         if not code:
             return None
 
         codes: Dict = cls._get_code_dictionary()
         code_path = code.split(".")
         value: Optional[Dict[str, str]] = cls._get_nested_code_entry(codes, code_path, 0, facet, is_leaf)
@@ -208,15 +208,15 @@
                            indexed by their unique 'identifier' template field (note: all messages with
                            one or more template parameters are expected to have an 'identifier' parameter,
                            the values for which corresponding to the keys of the dictionary. The value of those
                            keys are either 'None' if the identifier is the only template parameter, or alternately,
                            a list of dictionaries containing all the other expected parameters keys and their values
                            for every distinct message).
         :param add_prefix: bool, flag to prepend a prefix for the message type
-                           (i.e. error, warning, info) to displayed messages (default: False)
+                           (i.e. critical, error, warning, info) to displayed messages (default: False)
 
         :return: List[str], list of decoded messages
         """
         value: Optional[Tuple[str, Dict[str, str]]] = cls.get_code_subtree(code, is_leaf=True)
         assert value, f"CodeDictionary.display(): unknown message code {code}"
 
         message_type = cls.get_message_type(code)
```

### Comparing `reasoner_validator-3.5.9/reasoner_validator/versioning.py` & `reasoner_validator-3.6.0/reasoner_validator/versioning.py`

 * *Files 5% similar despite different names*

```diff
@@ -142,14 +142,27 @@
 
     return False
 
 
 SemVer.__eq__ = _semver_eq_
 
 
+def _semver_ne_(obj: SemVer, other: SemVer) -> bool:
+    """
+    Equal operator ('!=') override.
+    :param obj: SemVer
+    :param other: SemVer
+    :return: bool, True if obj and other are NOT equal
+    """
+    return not _semver_eq_(obj, other)
+
+
+SemVer.__ne__ = _semver_ne_
+
+
 def _semver_ge_(obj: SemVer, other: SemVer) -> bool:
     """
     Greater than or equal operator ('>=') override.
     :param obj: SemVer
     :param other: SemVer
     :return: bool, True if obj >= other
     """
```

### Comparing `reasoner_validator-3.5.9/tests/test_biolink_compliance_validation.py` & `reasoner_validator-3.6.0/tests/test_biolink_compliance_validation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1325,15 +1325,17 @@
                 "resource_id": "infores:molepro",
                 "resource_role": "primary_knowledge_source"
             }
         ]
 
     mock_edge["object"] = "mock_object"
     trapi_validator.is_valid_trapi_query(mock_edge, edge_model)
-    if trapi_validator.has_errors():
+    # TODO: not sure if simple errors should be fully displaced
+    #       by 'critical' errors or rather, just complement them
+    if trapi_validator.has_critical():
         validator = trapi_validator
     else:
         # if you get this far,then attempt additional Biolink Validation
         validator = BiolinkValidator(
             graph_type=TRAPIGraphType.Query_Graph,
             trapi_version=trapi_version,
             biolink_version=biolink_version
@@ -1353,51 +1355,51 @@
             {},
             ""
         ),
         (  # Query 1 - 'qualifier_constraints' value is None - invalidated by TRAPI schema
             {
                 'qualifier_constraints': None
             },
-            "error.trapi.validation"
+            "critical.trapi.validation"
         ),
         (  # Query 2 - 'qualifier_constraints' value is not an array - invalidated by TRAPI schema
             {
                 'qualifier_constraints': {}
             },
-            "error.trapi.validation"
+            "critical.trapi.validation"
         ),
         (  # Query 3 - empty 'qualifier_constraints' array value - since nullable: true, this should pass
             {
                 'qualifier_constraints': []
             },
             ""
         ),
         (  # Query 4 - empty 'qualifier_set' entry - invalidated by TRAPI schema
             {
                 'qualifier_constraints': [
                     {}
                 ]
             },
-            "error.trapi.validation"
+            "critical.trapi.validation"
         ),
         (  # Query 5 - 'qualifier_set' entry is not a dictionary - invalidated by TRAPI schema
             {
                 'qualifier_constraints': [
                     []
                 ]
             },
-            "error.trapi.validation"
+            "critical.trapi.validation"
         ),
         (  # Query 6 - 'qualifier_set' entry is missing the 'qualifier_set' key - invalidated by TRAPI schema
             {
                 'qualifier_constraints': [
                     {"not_qualifier_set": []}
                 ]
             },
-            "error.trapi.validation"
+            "critical.trapi.validation"
         ),
         (  # Query 7 - 'qualifier_set' entry is empty
             {
                 'qualifier_constraints': [
                     {"qualifier_set": []}
                 ]
             },
@@ -1407,54 +1409,54 @@
             {
                 'qualifier_constraints': [
                     {
                         "qualifier_set": {}
                     }
                 ]
             },
-            "error.trapi.validation"
+            "critical.trapi.validation"
         ),
         (  # Query 9 - 'qualifier' entry in the qualifier_set is empty - invalidated by TRAPI schema
             {
                 'qualifier_constraints': [
                     {
                         "qualifier_set": [
                             None
                         ]
                     }
                 ]
             },
-            "error.trapi.validation"
+            "critical.trapi.validation"
         ),
         (  # Query 10 - 'qualifier' entry is not a JSON object (dictionary) - invalidated by TRAPI schema
             {
                 'qualifier_constraints': [
                     {
                         "qualifier_set": [
                             []
                         ]
                     }
                 ]
             },
-            "error.trapi.validation"
+            "critical.trapi.validation"
         ),
         (  # Query 11 - 'qualifier' entry is missing its 'qualifier_type_id' property - invalidated by TRAPI schema
             {
                 'qualifier_constraints': [
                     {
                         "qualifier_set": [
                             {
                                 # 'qualifier_type_id': "",
                                 'qualifier_value': ""
                             }
                         ]
                     }
                 ]
             },
-            "error.trapi.validation"
+            "critical.trapi.validation"
         ),
         (  # Query 12 - 'qualifier_type_id' property value is unknown
             {
                 'qualifier_constraints': [
                     {
                         "qualifier_set": [
                             {
@@ -1505,15 +1507,15 @@
                             {
                                 'qualifier_type_id': "biolink:object_direction_qualifier"
                             }
                         ]
                     }
                 ]
             },
-            "error.trapi.validation"
+            "critical.trapi.validation"
         ),
         (   # Query 16 - qualifier_type_id 'object_direction_qualifier' is a valid Biolink qualifier type and
             #            'upregulated' a valid corresponding 'permissible value' enum 'qualifier_value'
             {
                 'qualifier_constraints': [
                     {
                         "qualifier_set": [
@@ -1657,15 +1659,15 @@
             "1.3.0",
             QC_QS_NOT_A_CURIE,
             "error.query_graph.edge.qualifier_constraints.qualifier_set.qualifier.type_id.unknown"
         ),
         (  # Query 1 - 'qualifier_type_id' value not a Biolink CURIE - schema validation error in TRAPI < 1.4.0-beta
             "1.4.0-beta",
             QC_QS_NOT_A_CURIE,
-            "error.trapi.validation"
+            "critical.trapi.validation"
         )
     ]
 )
 def test_validate_biolink_curie_in_qualifier_constraints(query: Tuple[str, Dict, str]):
     qualifier_validator(
         tested_method=BiolinkValidator.validate_qualifier_constraints,
         edge_model="QEdge",
@@ -1687,44 +1689,44 @@
             },
             ""
         ),
         (  # Query 2 - 'qualifiers' value is not an array - invalidated by TRAPI schema
             {
                 'qualifiers': {}
             },
-            "error.trapi.validation"
+            "critical.trapi.validation"
         ),
         (  # Query 3 - empty 'qualifiers' array value - since nullable: true, this should pass
             {
                 'qualifiers': []
             },
             ""
         ),
         (  # Query 4 - empty 'qualifier_set' entry - invalidated by TRAPI schema
             {
                 'qualifiers': [{}]
             },
-            "error.trapi.validation"
+            "critical.trapi.validation"
         ),
         (  # Query 5 - 'qualifier_set' entry is not a dictionary - invalidated by TRAPI schema
             {
                 'qualifiers': [[]]
             },
-            "error.trapi.validation"
+            "critical.trapi.validation"
         ),
         (  # Query 6 - 'qualifier' entry is missing its 'qualifier_type_id' property - invalidated by TRAPI schema
             {
                 'qualifiers': [
                     {
                         # 'qualifier_type_id': "",
                         'qualifier_value': ""
                     }
                 ]
             },
-            "error.trapi.validation"
+            "critical.trapi.validation"
         ),
         (  # Query 7 - 'qualifier_type_id' property value is unknown
             {
                 'qualifiers': [
                     {
                         'qualifier_type_id': "biolink:unknown_qualifier",
                         'qualifier_value': "fake-qualifier-value"
@@ -1760,15 +1762,15 @@
             {
                 'qualifiers': [
                     {
                         'qualifier_type_id': "biolink:object_direction_qualifier"
                     }
                 ]
             },
-            "error.trapi.validation"
+            "critical.trapi.validation"
         ),
         (   # Query 11 - qualifier_type_id 'object_direction_qualifier' is a valid Biolink qualifier type and
             #            'upregulated' a valid corresponding 'permissible value' enum 'qualifier_value'
             {
                 'qualifiers': [
                     {
                         'qualifier_type_id': "biolink:object_direction_qualifier",
@@ -1822,15 +1824,15 @@
                 "1.3.0",
                 Q_NOT_A_CURIE,
                 "error.knowledge_graph.edge.qualifiers.qualifier.type_id.unknown"
         ),
         (  # Query 1 - 'qualifier_type_id' value not a Biolink CURIE - schema validation error in TRAPI < 1.4.0-beta
                 "1.4.0-beta",
                 Q_NOT_A_CURIE,
-                "error.trapi.validation"
+                "critical.trapi.validation"
         )
     ]
 )
 def test_validate_biolink_curie_in_qualifiers(query: Tuple[str, Dict, str]):
     qualifier_validator(
         tested_method=BiolinkValidator.validate_qualifiers,
         edge_model="Edge",
```

### Comparing `reasoner_validator-3.5.9/tests/test_data/sample_trapi_schema.yaml` & `reasoner_validator-3.6.0/tests/test_data/sample_trapi_schema.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.9/tests/test_response_validator.py` & `reasoner_validator-3.6.0/tests/test_response_validator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 """
 Unit tests for the generic (shared) components of the SRI Testing Framework
 """
 from typing import Tuple,  Dict
+from sys import stderr
+
 import logging
+
+from json import dump
+
 import pytest
 
 from reasoner_validator import TRAPIResponseValidator
 from tests.test_validation_report import check_messages
 
 logger = logging.getLogger(__name__)
 logger.setLevel("DEBUG")
@@ -220,58 +225,121 @@
     'edges': _TEST_EDGES_4
 }
 
 
 @pytest.mark.parametrize(
     "query",
     [
-        (   # Query 0 - No 'workflow' key
-            {},
+        (   # Query 0 - No 'workflow' key in TRAPI Response
+            {
+                'message': {}
+            },
         ),
         (   # Query 1 - Null 'workflow' key value
             {
+                'message': {},
                 'workflow': None
             },
         ),
         (  # Query 2 - Null 'workflow' key list
             {
+                'message': {},
                 'workflow': []
             },
         ),
         (  # Query 3 - 'runner_parameters' is Null
             {
+                'message': {},
                 'workflow': [
                     {
                         'runner_parameters': None,
                         'id': 'sort_results_score',
                         'parameters': {"ascending_or_descending": "ascending"}
                     }
                 ]
             },
         ),
         (  # Query 4 - 'parameters' is Null
             {
+                'message': {},
                 'workflow': [
                     {'runner_parameters': {'allowlist': ["infores:aragorn"]}, 'id': 'lookup', 'parameters': None}
                 ]
             },
         ),
         (  # Query 5 - both 'parameters' and 'runner_parameters' are Null
             {
+                'message': {},
                 'workflow': [
                     {'runner_parameters': None, 'id': 'lookup', 'parameters': None}
                 ]
             },
+        ),
+        (   # Query 6 - Now, we patch the Message itself when it is not empty - knowledge graph is nullable
+            {
+                'message': {
+                    'knowledge_graph': None
+                }
+            },
+        ),
+        (   # Query 7 - Now, we patch the Message itself when it is not empty
+            {
+                'message': {
+                    'knowledge_graph': {
+                        'nodes': {},
+                        'edges': {}
+                    }
+                }
+            },
+        ),
+        (   # Query 8 - Now, we patch the Message itself when it is not empty
+            {
+                'message': {
+                    'knowledge_graph': {
+                        'nodes': {},
+                        'edges': {}
+                    }
+                }
+            },
+        ),
+        (   # Query 9 - Now, we patch the Message.knowledge_edge.sources itself when it is not empty
+            {
+                'message': {
+                    'knowledge_graph': {
+                        'nodes': {},
+                        'edges': {
+                            "alice-in-wonderland": {
+                                 'subject': "tweedle-dee",
+                                 'predicate': "and",
+                                 'object': "tweedle-dum",
+                                 'sources': [
+                                     {
+                                         'resource_id': "infores:rabbit-hole",
+                                         'resource_role': "primary_knowledge_source"
+                                     }
+                                 ]
+                            }
+                        }
+                    }
+                }
+            },
+        ),
+        (   # Query 10 - Now, we patch the Message itself when it is not empty
+            {
+                'message': {
+                    'auxiliary_graphs': None
+                }
+            },
         )
     ]
 )
 def test_sanitize_trapi_query(query: Tuple):
     validator: TRAPIResponseValidator = TRAPIResponseValidator()
-    response: Dict = validator.sanitize_trapi_query(response=query[0])
-    # assert response == query[1]
+    response: Dict = validator.sanitize_trapi_response(response=query[0])
+    dump(response, stderr, indent=4)
 
 
 NUM_SAMPLE_NODES = 5
 
 SAMPLE_NODES: Dict = dict()
 for node_id in range(1, NUM_SAMPLE_NODES):
     SAMPLE_NODES[f"n{node_id}"] = dict()
@@ -358,15 +426,15 @@
                     "results": None
                 }
             },
             PRE_TRAPI_1_4_0,  # trapi_version
             None,
             None,
             False,
-            # "Validate TRAPI Response: ERROR - Response returned an null or empty Message Query Graph!"
+            # "Validate TRAPI Response: ERROR - Response returned a null or empty Message Query Graph!"
             "error.trapi.response.query_graph.empty"
         ),
         (
             # Query 3 - Partly empty Response.Message with a modest but
             #           workable query graph? Missing KG trapped next?
             {
                 "message": {
@@ -445,15 +513,15 @@
             },
             PRE_TRAPI_1_4_0,  # trapi_version
             None,
             None,
             False,
             # "Validate TRAPI Response: ERROR - the 'Response.Message.Results' field
             # is not TRAPI schema validated since it has the wrong format!"
-            "error.trapi.validation"
+            "critical.trapi.validation"
         ),
         (
             # Query 8 - Partly empty Response.Message with a modest but workable query and
             #           knowledge graphs? Empty Results detected next - just issue a warning?
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
@@ -679,15 +747,15 @@
                 "workflow": "workflows-not-an-array"
             },
             PRE_TRAPI_1_4_0,  # trapi_version
             None,
             None,
             True,
             # "Validate TRAPI Response: ERROR - TRAPI schena error: the 'workflow' field must be an array"
-            "error.trapi.validation"
+            "critical.trapi.validation"
         ),
         (
             # Query 21 - Valid full Message, under strict validation.
             #            Message is valid, the 'workflow' field is an array,
             #            but the single list entry is an invalid workflow spec?
             {
                 "message": {
@@ -697,17 +765,17 @@
                 },
                 "workflow": ["not-a-valid-workflow-spec"]
             },
             PRE_TRAPI_1_4_0,  # trapi_version
             None,
             None,
             True,
-            # "Validate TRAPI Response: ERROR - TRAPI schena error: the 'workflow' field must be an array of
+            # Validate TRAPI Response: ERROR - TRAPI schema error: the 'workflow' field must be an array of
             # a 'workflow' JSON objects, with contents as defined by the workflow schema.
-            "error.trapi.validation"
+            "critical.trapi.validation"
         ),
         (
             # Query 22 - Valid full Message, under strict validation.
             #            Message is valid, the 'workflow' field is an array,
             #            but the single list entry is in the workflow schema
             #            and has at least the one required field 'id'
             {
@@ -762,15 +830,15 @@
             },
             PRE_TRAPI_1_4_0,  # trapi_version
             None,
             None,
             True,
             # "Validate TRAPI Response: ERROR - TRAPI schema validation error: the 'workflow'
             # field entry overlay_compute_ngd is missing a required parameter 'qnodes_keys'
-            "error.trapi.validation"
+            "critical.trapi.validation"
         ),
         (
             # Query 24 - Valid full Message, under strict validation. Message is valid, the 'workflow' field is array,
             #            but the single list entry is an elaborated 'real world' workflow spec
             {
                 "message": {
                     "query_graph": _TEST_QG_1,
```

### Comparing `reasoner_validator-3.5.9/tests/test_semver.py` & `reasoner_validator-3.6.0/tests/test_semver.py`

 * *Files 18% similar despite different names*

```diff
@@ -106,19 +106,41 @@
     assert one_four_zero == one_four_zero
     assert one_four_zero_beta_one == one_four_zero_beta_one
 
     # Major release diff
     assert not zero_zero_one == one_three_zero
 
     # Minor release diff
-    assert not one_zero_zero >= one_one_zero
+    assert not one_zero_zero == one_one_zero
 
     # Patch release diff
     assert not one_one_zero == one_one_one
 
     # Prerelease release diff
     assert not one_four_zero == one_four_zero_beta_one
     assert not one_four_zero_beta_one == one_four_zero
     assert not one_four_zero_beta_one == one_four_zero_beta_four
 
     # pruned SemVer comparisons
     assert one_four_zero == one_four_one_beta_pruned
+
+
+def test_semver_not_equal_to():
+    assert not one_four_zero != one_four_zero
+    assert not one_four_zero_beta_one != one_four_zero_beta_one
+
+    # Major release diff
+    assert zero_zero_one != one_three_zero
+
+    # Minor release diff
+    assert one_zero_zero != one_one_zero
+
+    # Patch release diff
+    assert one_one_zero != one_one_one
+
+    # Prerelease release diff
+    assert one_four_zero != one_four_zero_beta_one
+    assert one_four_zero_beta_one != one_four_zero
+    assert one_four_zero_beta_one != one_four_zero_beta_four
+
+    # pruned SemVer comparisons
+    assert not one_four_zero != one_four_one_beta_pruned
```

### Comparing `reasoner_validator-3.5.9/tests/test_trapi_versioning.py` & `reasoner_validator-3.6.0/tests/test_trapi_versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.9/tests/test_validate.py` & `reasoner_validator-3.6.0/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.9/tests/test_validation_report.py` & `reasoner_validator-3.6.0/tests/test_validation_report.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,43 +11,44 @@
 TEST_TRAPI_VERSION = get_latest_version(ValidationReporter.DEFAULT_TRAPI_VERSION)
 TEST_BIOLINK_VERSION = "2.4.8"
 
 
 def check_messages(validator: ValidationReporter, code, no_errors: bool = False):
     messages: Dict[str, Dict[str, Optional[Dict[str, Optional[List[Dict[str, str]]]]]]] = validator.get_messages()
     if code:
+        # print("code is:", code)
+        # print("message_type", message_type)
         # TODO: 'code' should be found in code.yaml
         # value: Optional[Tuple[str, str]] = CodeDictionary.get_code_subtree(code)
         # assert value is not None
         message_type = validator.get_message_type(code)
-        if message_type == "error":
-            print("code is:", code)
-            print("message_type", message_type)
-            print("messages['errors']:", messages['errors'])
-            for error_code in messages['errors']:
-                print("error code is:", error_code)
+        if message_type == "critical":
+            assert any([critical_code == code for critical_code in messages['critical']])
+        elif message_type == "error":
             assert any([error_code == code for error_code in messages['errors']])
         elif message_type == "warning":
             assert any([warning_code == code for warning_code in messages['warnings']])
         elif message_type == "info":
             assert any([info_code == code for info_code in messages['information']])
     else:
         if no_errors:
-            # just don't want any hard errors; info and warnings are ok?
+            # just don't want any 'critical' (errors) nor 'errors'; 'information' and 'warnings' are ok?
+            assert not validator.has_critical(), f"Unexpected critical error messages seen {messages}"
             assert not validator.has_errors(), f"Unexpected error messages seen {messages}"
         else:
             # no expected at all? Assert the absence of such messages?
             assert not validator.has_messages(), f"Unexpected messages seen {messages}"
 
 
 def test_check_basic_get_code_subtree():
     assert CodeDictionary.get_code_subtree("") is None
     assert CodeDictionary.get_code_subtree("info") is not None
     assert CodeDictionary.get_code_subtree("warning") is not None
     assert CodeDictionary.get_code_subtree("error") is not None
+    assert CodeDictionary.get_code_subtree("critical") is not None
     assert CodeDictionary.get_code_subtree("foo.bar") is None
 
 
 def test_get_code_subtree_is_leaf():
 
     result = CodeDictionary.get_code_subtree("info.compliant", is_leaf=True)
     assert result is not None
@@ -113,17 +114,14 @@
     assert result is not None
     message_type, subtree = result
     assert isinstance(subtree, Dict)
     assert message_type == "warning"
     assert subtree is not None
     assert all([key in ["node", "predicate", "edge"] for key in subtree])
 
-    assert CodeDictionary.get_code_subtree("error") is not None
-    assert CodeDictionary.get_code_subtree("foo.bar") is None
-
 
 def test_get_entry():
     assert CodeDictionary.get_code_entry("") is None
 
     code_entry: Optional[Dict] = CodeDictionary.get_code_entry("info.compliant")
     assert code_entry is not None
     assert CodeDictionary.MESSAGE in code_entry
@@ -131,23 +129,24 @@
 
     # Higher level subtrees, not terminal leaf entries?
     assert CodeDictionary.get_code_entry("info") is None
     assert CodeDictionary.get_code_entry("info.query_graph") is None
     assert CodeDictionary.get_code_entry("info.query_graph.node") is None
     assert CodeDictionary.get_code_entry("warning") is None
     assert CodeDictionary.get_code_entry("error") is None
+    assert CodeDictionary.get_code_entry("critical") is None
 
     # Unknown code?
     assert CodeDictionary.get_code_entry("foo.bar") is None
 
 
 def test_get_message_template():
     assert CodeDictionary.get_message_template("") is None
     assert CodeDictionary.get_message_template("info.compliant") == "Biolink Model-compliant TRAPI Message"
-    assert CodeDictionary.get_message_template("error.trapi.request.invalid") == \
+    assert CodeDictionary.get_message_template("critical.trapi.request.invalid") == \
            "Test could not generate a valid TRAPI query request object using identified element"
     assert CodeDictionary.get_message_template("foo.bar") is None
 
 
 def test_get_description():
     assert CodeDictionary.get_description("") is None
     info_compliant = CodeDictionary.get_description("info.compliant")
@@ -215,14 +214,16 @@
     assert reporter1.get_biolink_version() is None
     assert not reporter1.has_messages()
     reporter1.report("info.compliant")
     assert reporter1.has_messages()
     assert reporter1.has_information()
     assert not reporter1.has_warnings()
     assert not reporter1.has_errors()
+    assert not reporter1.has_critical()
+
     reporter1.report("warning.graph.empty", identifier="Reporter1 Unit Test")
     assert reporter1.has_warnings()
     reporter1.report("error.knowledge_graph.nodes.empty")
     assert reporter1.has_errors()
 
     # Testing merging of messages from a second reporter
     reporter2 = ValidationReporter(
@@ -262,22 +263,33 @@
                     {
                         "categories": "Lost in Space"
                     }
                 ]
             }
         },
         "errors": {
-            "error.trapi.validation": {
+            "error.biolink.model.noncompliance": {
                 "6.6.6": [
                     {
                         'reason': "Dave, this can only be due to human error..."
                     }
                 ]
 
             }
+        },
+        "critical": {
+            "critical.trapi.validation": {
+                "9.1.1": [
+                    {
+                        'component': 'Query',
+                        'reason': "Fire, Ambulance or Police?"
+                    }
+                ]
+
+            }
         }
     }
     reporter1.add_messages(new_messages)
 
     # Verify what we have
     messages: Dict[str, Dict[str, Optional[Dict[str, Optional[List[Dict[str, str]]]]]]] = reporter1.get_messages()
 
@@ -298,27 +310,34 @@
            "Node identifier found unmapped to target categories for node" in warnings
 
     assert "errors" in messages
     assert len(messages['errors']) > 0
     errors: List[str] = list()
     for code, parameters in messages['errors'].items():
         errors.extend(CodeDictionary.display(code, parameters, add_prefix=True))
-    assert "ERROR - Trapi: Schema validation error" in errors
-    
+    assert "ERROR - Biolink Model: S-P-O statement is not compliant to Biolink Model release" in errors
+
+    assert "critical" in messages
+    assert len(messages['critical']) > 0
+    critical: List[str] = list()
+    for code, parameters in messages['critical'].items():
+        critical.extend(CodeDictionary.display(code, parameters, add_prefix=True))
+    assert "CRITICAL - Trapi: Schema validation error" in critical
+
     obj = reporter1.to_dict()
     assert obj["trapi_version"] == TEST_TRAPI_VERSION
     assert obj["biolink_version"] == TEST_BIOLINK_VERSION
     assert "messages" in obj
-    assert "errors" in obj["messages"]
-    assert "error.trapi.validation" in obj["messages"]["errors"]
-    messages: Optional[Dict[str, List[Dict[str, str]]]] = obj["messages"]["errors"]["error.trapi.validation"]
-    assert messages, "Empty 'error.trapi.validation' messages set?"
-    assert "6.6.6" in messages
-    message_subset: List = messages["6.6.6"]
-    assert "Dave, this can only be due to human error..."\
+    assert "critical" in obj["messages"]
+    assert "critical.trapi.validation" in obj["messages"]["critical"]
+    messages: Optional[Dict[str, List[Dict[str, str]]]] = obj["messages"]["critical"]["critical.trapi.validation"]
+    assert messages, "Empty 'critical.trapi.validation' messages set?"
+    assert "9.1.1" in messages
+    message_subset: List = messages["9.1.1"]
+    assert "Fire, Ambulance or Police?"\
            in [message['reason'] for message in message_subset if 'reason' in message]
 
     for n in range(0, 10):
         reporter1.report(code="error.input_edge.node.category.missing", identifier=f"biolink:not_a_category_{n}")
 
     for c in range(0, 5):
         for n in range(0, 10):
@@ -350,15 +369,15 @@
         "ValidatorReporter.dump() resetting the title to a user string\n" +
         "and compressed using 'id_rows=1', 'msg_rows=1', 'compress=True':\n",
         file=stderr
     )
     reporter1.dump(title="My KP Validation Report", id_rows=1, msg_rows=1, compact_format=True, file=stderr)
 
     validation_report: str = reporter1.dumps(id_rows=2, msg_rows=3)
-    assert validation_report.startswith("Errors:")
+    assert validation_report.startswith("Critical:")
 
 
 def test_validator_method():
 
     reporter = ValidationReporter(
         prefix="Test Validator Method",
         trapi_version=TEST_TRAPI_VERSION,
@@ -415,21 +434,38 @@
             {
                 "validation": {
                     "trapi_version": "1.3",
                     "biolink_version": "2.4.7",
                     "messages": {
                         "information": {},
                         "warnings": {},
-                        "errors": {""}
+                        "errors": {},
+                        "critical": {""}
                     }
                 }
             },
             True
         ),
         (
+                'validation',
+                {
+                    "validation": {
+                        "trapi_version": "1.3",
+                        "biolink_version": "2.4.7",
+                        "messages": {
+                            "information": {},
+                            "warnings": {},
+                            "errors": {""},
+                            "critical": {}
+                        }
+                    }
+                },
+                True
+        ),
+        (
             "validation",
             {
                 "validation": {
                     "trapi_version": "1.3",
                     "biolink_version": "2.4.7",
                     "messages": {
                         "information": {},
@@ -442,15 +478,16 @@
                             "warning.knowledge_graph.edge.predicate.non_canonical": [
                                 {
                                     "identifier": "ABC1--biolink:participates_in->Glycolysis",
                                     "predicate": "biolink:participates_in"
                                 }
                             ]
                         },
-                        "errors": {}
+                        "errors": {},
+                        "critical": {}
                     }
                 }
             },
             False
         ),
     ]
 )
```

### Comparing `reasoner_validator-3.5.9/tests/test_workflows.py` & `reasoner_validator-3.6.0/tests/test_workflows.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.5.9/PKG-INFO` & `reasoner_validator-3.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-validator
-Version: 3.5.9
+Version: 3.6.0
 Summary: Validation tools for Reasoner API
 Home-page: https://github.com/NCATSTranslator
 License: MIT
 Keywords: NCATS,Biomedical Data Translator,Translator,ReasonerAPI,TRAPI,validation,Biolink Model
 Author: Richard Bruskiewich
 Author-email: richard.bruskiewich@delphinai.com
 Maintainer: Richard Bruskiewich
```

