# Comparing `tmp/kuflow_temporal_activity_kuflow-0.6.1.tar.gz` & `tmp/kuflow_temporal_activity_kuflow-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuflow_temporal_activity_kuflow-0.6.1.tar", max compression
+gzip compressed data, was "kuflow_temporal_activity_kuflow-0.7.0.tar", max compression
```

## Comparing `kuflow_temporal_activity_kuflow-0.6.1.tar` & `kuflow_temporal_activity_kuflow-0.7.0.tar`

### file list

```diff
@@ -1,12 +1,22 @@
--rw-r--r--   0        0        0      878 2023-06-16 09:00:12.915234 kuflow_temporal_activity_kuflow-0.6.1/README.md
--rw-r--r--   0        0        0        6 2023-06-16 09:00:12.915234 kuflow_temporal_activity_kuflow-0.6.1/VERSION
--rw-r--r--   0        0        0     1320 2023-06-16 09:00:12.915234 kuflow_temporal_activity_kuflow-0.6.1/kuflow_temporal_activity_kuflow/__init__.py
--rw-r--r--   0        0        0     3817 2023-06-16 09:00:12.915234 kuflow_temporal_activity_kuflow-0.6.1/kuflow_temporal_activity_kuflow/converter.py
--rw-r--r--   0        0        0     2018 2023-06-16 09:00:12.915234 kuflow_temporal_activity_kuflow-0.6.1/kuflow_temporal_activity_kuflow/kuflow_async_activities.py
--rw-r--r--   0        0        0    13631 2023-06-16 09:00:12.915234 kuflow_temporal_activity_kuflow-0.6.1/kuflow_temporal_activity_kuflow/kuflow_sync_activities.py
--rw-r--r--   0        0        0     3553 2023-06-16 09:00:12.915234 kuflow_temporal_activity_kuflow-0.6.1/kuflow_temporal_activity_kuflow/models/__init__.py
--rw-r--r--   0        0        0    22166 2023-06-16 09:00:12.915234 kuflow_temporal_activity_kuflow-0.6.1/kuflow_temporal_activity_kuflow/models/_models.py
--rw-r--r--   0        0        0     8623 2023-06-16 09:00:12.915234 kuflow_temporal_activity_kuflow-0.6.1/kuflow_temporal_activity_kuflow/validation.py
--rw-r--r--   0        0        0     1037 2023-06-16 09:01:41.498693 kuflow_temporal_activity_kuflow-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     1662 1970-01-01 00:00:00.000000 kuflow_temporal_activity_kuflow-0.6.1/setup.py
--rw-r--r--   0        0        0     1667 1970-01-01 00:00:00.000000 kuflow_temporal_activity_kuflow-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      878 2023-06-20 06:25:31.590348 kuflow_temporal_activity_kuflow-0.7.0/README.md
+-rw-r--r--   0        0        0        6 2023-06-20 06:25:31.590348 kuflow_temporal_activity_kuflow-0.7.0/VERSION
+-rw-r--r--   0        0        0     1320 2023-06-20 06:25:31.590348 kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/__init__.py
+-rw-r--r--   0        0        0     8623 2023-06-20 06:25:31.590348 kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/_validation.py
+-rw-r--r--   0        0        0     5176 2023-06-20 06:25:31.590348 kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/converter.py
+-rw-r--r--   0        0        0     2226 2023-06-20 06:25:31.590348 kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/kuflow_async_activities.py
+-rw-r--r--   0        0        0    15503 2023-06-20 06:25:31.590348 kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/kuflow_sync_activities.py
+-rw-r--r--   0        0        0     3553 2023-06-20 06:25:31.590348 kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/models/__init__.py
+-rw-r--r--   0        0        0     1949 2023-06-20 06:26:41.671973 kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/models/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    22540 2023-06-20 06:26:41.675974 kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/models/__pycache__/_models.cpython-38.pyc
+-rw-r--r--   0        0        0    22235 2023-06-20 06:25:31.590348 kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/models/_models.py
+-rw-r--r--   0        0        0     1478 2023-06-20 06:25:31.594348 kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/utils/__init__.py
+-rw-r--r--   0        0        0      499 2023-06-20 06:26:41.679974 kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/utils/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    10493 2023-06-20 06:26:41.683974 kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/utils/__pycache__/_save_process_element_utils.cpython-38.pyc
+-rw-r--r--   0        0        0    13245 2023-06-20 06:26:41.687975 kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/utils/__pycache__/_save_task_element_utils.cpython-38.pyc
+-rw-r--r--   0        0        0    14343 2023-06-20 06:26:41.687975 kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/utils/__pycache__/_save_task_json_forms_value_data_request_utils.cpython-38.pyc
+-rw-r--r--   0        0        0    11220 2023-06-20 06:25:31.594348 kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/utils/_save_process_element_utils.py
+-rw-r--r--   0        0        0    14103 2023-06-20 06:25:31.594348 kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/utils/_save_task_element_utils.py
+-rw-r--r--   0        0        0    15436 2023-06-20 06:25:31.594348 kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/utils/_save_task_json_forms_value_data_request_utils.py
+-rw-r--r--   0        0        0     1037 2023-06-20 06:26:59.285395 kuflow_temporal_activity_kuflow-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1705 1970-01-01 00:00:00.000000 kuflow_temporal_activity_kuflow-0.7.0/setup.py
+-rw-r--r--   0        0        0     1667 1970-01-01 00:00:00.000000 kuflow_temporal_activity_kuflow-0.7.0/PKG-INFO
```

### Comparing `kuflow_temporal_activity_kuflow-0.6.1/README.md` & `kuflow_temporal_activity_kuflow-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_kuflow-0.6.1/kuflow_temporal_activity_kuflow/__init__.py` & `kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 # SOFTWARE.
 #
 
 from .kuflow_async_activities import KuFlowAsyncActivities
 from .kuflow_sync_activities import KuFlowSyncActivities
 
 __all__ = ["KuFlowAsyncActivities", "KuFlowSyncActivities"]
-__version__ = "0.6.1"
+__version__ = "0.7.0"
```

### Comparing `kuflow_temporal_activity_kuflow-0.6.1/kuflow_temporal_activity_kuflow/converter.py` & `kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/converter.py`

 * *Files 22% similar despite different names*

```diff
@@ -39,14 +39,47 @@
 
 from . import models as models_temporal
 
 with workflow.unsafe.imports_passed_through():
     from kuflow_rest import Serializer, Deserializer, Model
 
 
+class KuFlowComposableEncodingPayloadConverter(EncodingPayloadConverter):
+    _default_json_converter: JSONPlainPayloadConverter
+
+    _serialize: Serializer
+    _deserialize: Deserializer
+
+    def __init__(self, default_json_converter=JSONPlainPayloadConverter()) -> None:
+        self._default_json_converter = default_json_converter
+        client_models_rest = {k: v for k, v in models_rest.__dict__.items() if isinstance(v, type)}
+        client_models_temporal = {k: v for k, v in models_temporal.__dict__.items() if isinstance(v, type)}
+        client_models = {**client_models_rest, **client_models_temporal}
+        self._serialize = Serializer(client_models)
+        self._deserialize = Deserializer(client_models)
+
+    @property
+    def encoding(self) -> str:
+        return "json/plain"
+
+    def to_payload(self, value: Any) -> Optional[Payload]:
+        if isinstance(value, Model) is False:
+            return None
+
+        serialized = self._serialize.body(value, value.__class__.__name__)
+        return self._default_json_converter.to_payload(serialized)
+
+    def from_payload(self, payload: Payload, type_hint: Optional[Type] = None) -> Any:
+        if issubclass(type_hint, Model) is False:
+            return None
+
+        as_python_object = json.loads(payload.data)
+        return self._deserialize(type_hint.__name__, as_python_object)
+
+
 class KuFlowEncodingPayloadConverter(EncodingPayloadConverter):
     _default_json_converter: JSONPlainPayloadConverter
 
     _serialize: Serializer
     _deserialize: Deserializer
 
     def __init__(self, default_json_converter=JSONPlainPayloadConverter()) -> None:
```

### Comparing `kuflow_temporal_activity_kuflow-0.6.1/kuflow_temporal_activity_kuflow/kuflow_async_activities.py` & `kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/kuflow_async_activities.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,24 +23,27 @@
 # SOFTWARE.
 #
 
 import base64
 
 from temporalio import activity
 from kuflow_rest import KuFlowRestClient
+from kuflow_temporal_common import converter
 
+from .converter import KuFlowComposableEncodingPayloadConverter
 from . import models as models_temporal
 
 
 class KuFlowAsyncActivities:
     def __init__(self, kuflow_client: KuFlowRestClient) -> None:
         self._kuflow_client = kuflow_client
         self.activities = [self.create_task_and_wait_finished]
 
     @activity.defn(name="KuFlow_Engine_createTaskAndWaitFinished")
+    @converter.register(encoding_payload_converter_class=KuFlowComposableEncodingPayloadConverter)
     async def create_task_and_wait_finished(
         self,
         request: models_temporal.CreateTaskRequest,
     ) -> None:
         base64_token = base64.b64encode(activity.info().task_token)
 
         self._kuflow_client.task.create_task(task=request.task, activity_token=base64_token.decode())
```

### Comparing `kuflow_temporal_activity_kuflow-0.6.1/kuflow_temporal_activity_kuflow/kuflow_sync_activities.py` & `kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/kuflow_sync_activities.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,17 +22,18 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 
 from temporalio import activity
 
 from kuflow_rest import KuFlowRestClient, models
-from kuflow_temporal_common import exceptions
+from kuflow_temporal_common import exceptions, converter
 
-from . import models as models_temporal, validation
+from . import _validation as validation, models as models_temporal
+from .converter import KuFlowComposableEncodingPayloadConverter
 
 
 class KuFlowSyncActivities:
     def __init__(self, kuflow_client: KuFlowRestClient) -> None:
         self._kuflow_client = kuflow_client
         self.activities = [
             self.retrieve_principal,
@@ -51,56 +52,60 @@
             self.save_task_element,
             self.delete_task_element,
             self.delete_task_element_value_document,
             self.append_task_log,
         ]
 
     @activity.defn(name="KuFlow_Engine_retrievePrincipal")
+    @converter.register(encoding_payload_converter_class=KuFlowComposableEncodingPayloadConverter)
     async def retrieve_principal(
         self,
         request: models_temporal.RetrievePrincipalRequest,
     ) -> models_temporal.RetrievePrincipalResponse:
         try:
             validation.validate_retrieve_principal_request(request)
 
             principal = self._kuflow_client.principal.retrieve_principal(id=request.principal_id)
 
             return models_temporal.RetrievePrincipalResponse(principal=principal)
         except Exception as err:
             raise exceptions.create_application_error(err) from err
 
     @activity.defn(name="KuFlow_Engine_findProcesses")
+    @converter.register(encoding_payload_converter_class=KuFlowComposableEncodingPayloadConverter)
     async def find_processes(
         self,
         request: models_temporal.FindProcessesRequest,
     ) -> models_temporal.FindProcessesResponse:
         try:
             # Get all non-None properties of the object to avoid overwrite defaults
             non_none_props = {k: v for k, v in vars(request).items() if v is not None}
             proces_page = self._kuflow_client.process.find_processes(**non_none_props)
 
             return models_temporal.FindProcessesResponse(processes=proces_page)
         except Exception as err:
             raise exceptions.create_application_error(err) from err
 
     @activity.defn(name="KuFlow_Engine_retrieveProcess")
+    @converter.register(encoding_payload_converter_class=KuFlowComposableEncodingPayloadConverter)
     async def retrieve_process(
         self,
         request: models_temporal.RetrieveProcessRequest,
     ) -> models_temporal.RetrieveProcessResponse:
         try:
             validation.validate_retrieve_process_request(request)
 
             process = self._kuflow_client.process.retrieve_process(id=request.process_id)
 
             return models_temporal.RetrieveProcessResponse(process=process)
         except Exception as err:
             raise exceptions.create_application_error(err) from err
 
     @activity.defn(name="KuFlow_Engine_saveProcessElement")
+    @converter.register(encoding_payload_converter_class=KuFlowComposableEncodingPayloadConverter)
     async def save_process_element(
         self,
         request: models_temporal.SaveProcessElementRequest,
     ) -> models_temporal.SaveProcessElementResponse:
         try:
             validation.validate_save_process_element_request(request)
 
@@ -110,14 +115,15 @@
             process = self._kuflow_client.process.actions_process_save_element(id=request.process_id, command=command)
 
             return models_temporal.SaveProcessElementResponse(process=process)
         except Exception as err:
             raise exceptions.create_application_error(err) from err
 
     @activity.defn(name="KuFlow_Engine_deleteProcessElement")
+    @converter.register(encoding_payload_converter_class=KuFlowComposableEncodingPayloadConverter)
     async def delete_process_element(
         self,
         request: models_temporal.DeleteProcessElementRequest,
     ) -> models_temporal.DeleteProcessElementResponse:
         try:
             validation.validate_delete_process_element_request(request)
 
@@ -126,28 +132,30 @@
             process = self._kuflow_client.process.actions_process_delete_element(id=request.process_id, command=command)
 
             return models_temporal.DeleteProcessElementResponse(process=process)
         except Exception as err:
             raise exceptions.create_application_error(err) from err
 
     @activity.defn(name="KuFlow_Engine_completeProcess")
+    @converter.register(encoding_payload_converter_class=KuFlowComposableEncodingPayloadConverter)
     async def complete_process(
         self,
         request: models_temporal.CompleteProcessRequest,
     ) -> models_temporal.CompleteProcessResponse:
         try:
             validation.validate_complete_process_request(request)
 
             process = self._kuflow_client.process.actions_process_complete(request.process_id)
 
             return models_temporal.CompleteProcessResponse(process=process)
         except Exception as err:
             raise exceptions.create_application_error(err) from err
 
     @activity.defn(name="KuFlow_Engine_changeProcessInitiator")
+    @converter.register(encoding_payload_converter_class=KuFlowComposableEncodingPayloadConverter)
     async def change_process_initiator(
         self,
         request: models_temporal.ChangeProcessInitiatorRequest,
     ) -> models_temporal.ChangeProcessInitiatorResponse:
         try:
             validation.validate_change_process_initiator_request(request)
 
@@ -157,84 +165,90 @@
             )
 
             return models_temporal.ChangeProcessInitiatorResponse(process=process)
         except Exception as err:
             raise exceptions.create_application_error(err) from err
 
     @activity.defn(name="KuFlow_Engine_findTasks")
+    @converter.register(encoding_payload_converter_class=KuFlowComposableEncodingPayloadConverter)
     async def find_tasks(
         self,
         request: models_temporal.FindTaskRequest,
     ) -> models_temporal.FindTaskResponse:
         try:
             # Get all non-None properties of the object to avoid overwrite defaults
             non_none_props = {k: v for k, v in vars(request).items() if v is not None}
             task_page = self._kuflow_client.task.find_tasks(**non_none_props)
 
             return models_temporal.FindTaskResponse(tasks=task_page)
         except Exception as err:
             raise exceptions.create_application_error(err) from err
 
     @activity.defn(name="KuFlow_Engine_retrieveTask")
+    @converter.register(encoding_payload_converter_class=KuFlowComposableEncodingPayloadConverter)
     async def retrieve_task(
         self,
         request: models_temporal.RetrieveTaskRequest,
     ) -> models_temporal.RetrieveTaskResponse:
         try:
             validation.validate_retrieve_task_request(request)
 
             task = self._kuflow_client.task.retrieve_task(id=request.task_id)
 
             return models_temporal.RetrieveTaskResponse(task=task)
         except Exception as err:
             raise exceptions.create_application_error(err) from err
 
     @activity.defn(name="KuFlow_Engine_createTask")
+    @converter.register(encoding_payload_converter_class=KuFlowComposableEncodingPayloadConverter)
     async def create_task(
         self,
         request: models_temporal.CreateTaskRequest,
     ) -> models_temporal.CreateTaskResponse:
         try:
             validation.validate_create_task_request(request)
 
             task = self._kuflow_client.task.create_task(task=request.task)
 
             return models_temporal.CreateTaskResponse(task=task)
         except Exception as err:
             raise exceptions.create_application_error(err) from err
 
     @activity.defn(name="KuFlow_Engine_completeTask")
+    @converter.register(encoding_payload_converter_class=KuFlowComposableEncodingPayloadConverter)
     async def complete_task(
         self,
         request: models_temporal.CompleteTaskRequest,
     ) -> models_temporal.CompleteTaskResponse:
         try:
             validation.validate_complete_task_request(request)
 
             task = self._kuflow_client.task.actions_task_complete(id=request.task_id)
 
             return models_temporal.CompleteTaskResponse(task=task)
         except Exception as err:
             raise exceptions.create_application_error(err) from err
 
     @activity.defn(name="KuFlow_Engine_claimTask")
+    @converter.register(encoding_payload_converter_class=KuFlowComposableEncodingPayloadConverter)
     async def claim_task(
         self,
         request: models_temporal.ClaimTaskRequest,
     ) -> models_temporal.ClaimTaskResponse:
         try:
             validation.validate_claim_task_request(request)
 
             task = self._kuflow_client.task.actions_task_claim(id=request.task_id)
 
             return models_temporal.ClaimTaskResponse(task=task)
         except Exception as err:
             raise exceptions.create_application_error(err) from err
 
     @activity.defn(name="KuFlow_Engine_assignTask")
+    @converter.register(encoding_payload_converter_class=KuFlowComposableEncodingPayloadConverter)
     async def assign_task(
         self,
         request: models_temporal.AssignTaskRequest,
     ) -> models_temporal.AssignTaskResponse:
         try:
             validation.validate_assign_task_request(request)
 
@@ -242,14 +256,15 @@
             task = self._kuflow_client.task.actions_task_assign(id=request.task_id, command=command)
 
             return models_temporal.AssignTaskResponse(task=task)
         except Exception as err:
             raise exceptions.create_application_error(err) from err
 
     @activity.defn(name="KuFlow_Engine_saveTaskElement")
+    @converter.register(encoding_payload_converter_class=KuFlowComposableEncodingPayloadConverter)
     async def save_task_element(
         self,
         request: models_temporal.SaveTaskElementRequest,
     ) -> models_temporal.SaveTaskElementResponse:
         try:
             validation.validate_save_task_element_request(request)
 
@@ -259,14 +274,15 @@
             task = self._kuflow_client.task.actions_task_save_element(id=request.task_id, command=command)
 
             return models_temporal.SaveTaskElementResponse(task=task)
         except Exception as err:
             raise exceptions.create_application_error(err) from err
 
     @activity.defn(name="KuFlow_Engine_deleteTaskElement")
+    @converter.register(encoding_payload_converter_class=KuFlowComposableEncodingPayloadConverter)
     async def delete_task_element(
         self,
         request: models_temporal.DeleteTaskElementRequest,
     ) -> models_temporal.DeleteTaskElementResponse:
         try:
             validation.validate_delete_task_element_request(request)
 
@@ -274,14 +290,15 @@
             task = self._kuflow_client.task.actions_task_delete_element(id=request.task_id, command=command)
 
             return models_temporal.DeleteTaskElementResponse(task=task)
         except Exception as err:
             raise exceptions.create_application_error(err) from err
 
     @activity.defn(name="KuFlow_Engine_deleteTaskElementValueDocument")
+    @converter.register(encoding_payload_converter_class=KuFlowComposableEncodingPayloadConverter)
     async def delete_task_element_value_document(
         self,
         request: models_temporal.DeleteTaskElementValueDocumentRequest,
     ) -> models_temporal.DeleteTaskElementValueDocumentResponse:
         try:
             validation.validate_delete_task_element_value_document_request(request)
 
@@ -291,14 +308,15 @@
             )
 
             return models_temporal.DeleteTaskElementValueDocumentResponse(task=task)
         except Exception as err:
             raise exceptions.create_application_error(err) from err
 
     @activity.defn(name="KuFlow_Engine_saveTaskJsonFormsValueData")
+    @converter.register(encoding_payload_converter_class=KuFlowComposableEncodingPayloadConverter)
     async def save_task_json_forms_value_data(
         self,
         request: models_temporal.SaveTaskJsonFormsValueDataRequest,
     ) -> models_temporal.SaveTaskJsonFormsValueDataResponse:
         try:
             validation.validate_save_task_json_forms_value_data(request)
 
@@ -306,14 +324,15 @@
             task = self._kuflow_client.task.actions_task_save_json_forms_value_data(id=request.task_id, command=command)
 
             return models_temporal.SaveTaskJsonFormsValueDataResponse(task=task)
         except Exception as err:
             raise exceptions.create_application_error(err) from err
 
     @activity.defn(name="KuFlow_Engine_appendTaskLog")
+    @converter.register(encoding_payload_converter_class=KuFlowComposableEncodingPayloadConverter)
     async def append_task_log(
         self,
         request: models_temporal.AppendTaskLogRequest,
     ) -> models_temporal.AppendTaskLogResponse:
         try:
             validation.validate_append_task_log_request(request)
```

### Comparing `kuflow_temporal_activity_kuflow-0.6.1/kuflow_temporal_activity_kuflow/models/__init__.py` & `kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_kuflow-0.6.1/kuflow_temporal_activity_kuflow/models/_models.py` & `kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/models/_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,21 +255,21 @@
         "element_values": {"key": "elementValues", "type": "[ProcessElementValue]"},
     }
 
     def __init__(
         self,
         process_id: str,
         element_definition_code: str,
-        element_values: List[models_rest.ProcessElementValue],
+        element_values: Optional[List[models_rest.ProcessElementValue]] = None,
         **kwargs: Any,
     ) -> None:
         super().__init__(**kwargs)
         self.process_id = process_id
         self.element_definition_code = element_definition_code
-        self.element_values = element_values
+        self.element_values = element_values or []
 
 
 class SaveProcessElementResponse(_serialization.Model):
     """
     Attributes:
         process: Process updated
     """
@@ -661,21 +661,21 @@
         "element_values": {"key": "elementValues", "type": "[TaskElementValue]"},
     }
 
     def __init__(
         self,
         task_id: str,
         element_definition_code: str,
-        element_values: List[models_rest.TaskElementValue],
+        element_values: Optional[List[models_rest.TaskElementValue]] = None,
         **kwargs: Any,
     ) -> None:
         super().__init__(**kwargs)
         self.task_id = task_id
         self.element_definition_code = element_definition_code
-        self.element_values = element_values
+        self.element_values = element_values or []
 
 
 class SaveTaskElementResponse(_serialization.Model):
     """
     Attributes:
         task: Task updated
     """
@@ -778,18 +778,18 @@
     data: Dict[str, Any]
 
     _attribute_map = {
         "task_id": {"key": "taskId", "type": "str"},
         "data": {"key": "data", "type": "{object}"},
     }
 
-    def __init__(self, task_id: str, data: Dict[str, Any], **kwargs: Any) -> None:
+    def __init__(self, task_id: str, data: Optional[Dict[str, Any]] = None, **kwargs: Any) -> None:
         super().__init__(**kwargs)
         self.task_id = task_id
-        self.data = data
+        self.data = data or {}
 
 
 class SaveTaskJsonFormsValueDataResponse(_serialization.Model):
     """
     Attributes:
         task: Task updated
     """
```

### Comparing `kuflow_temporal_activity_kuflow-0.6.1/kuflow_temporal_activity_kuflow/validation.py` & `kuflow_temporal_activity_kuflow-0.7.0/kuflow_temporal_activity_kuflow/_validation.py`

 * *Files identical despite different names*

### Comparing `kuflow_temporal_activity_kuflow-0.6.1/pyproject.toml` & `kuflow_temporal_activity_kuflow-0.7.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kuflow-temporal-activity-kuflow"
-version = "0.6.1"
+version = "0.7.0"
 description = "KuFlow SDK :: Temporal.io activities to interact with KuFlow"
 license = "MIT"
 authors = ["KuFlow S.L. <kuflow@kuflow.com>"]
 homepage = "https://kuflow.com/"
 documentation = "https://docs.kuflow.com/"
 repository = "https://github.com/kuflow/kuflow-sdk-python"
 readme = "README.md"
@@ -13,15 +13,15 @@
 
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-kuflow-temporal-common = "^0.6.1"
+kuflow-temporal-common = "^0.7.0"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.3.0"
 ipython = "^7.34.0"
 flake8 = "^5.0.4"
 black = "^23.3.0"
 pytest = "^7.3.1"
```

### Comparing `kuflow_temporal_activity_kuflow-0.6.1/setup.py` & `kuflow_temporal_activity_kuflow-0.7.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['kuflow_temporal_activity_kuflow', 'kuflow_temporal_activity_kuflow.models']
+['kuflow_temporal_activity_kuflow',
+ 'kuflow_temporal_activity_kuflow.models',
+ 'kuflow_temporal_activity_kuflow.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['kuflow-temporal-common>=0.6.1,<0.7.0']
+['kuflow-temporal-common>=0.7.0,<0.8.0']
 
 setup_kwargs = {
     'name': 'kuflow-temporal-activity-kuflow',
-    'version': '0.6.1',
+    'version': '0.7.0',
     'description': 'KuFlow SDK :: Temporal.io activities to interact with KuFlow',
     'long_description': '[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)\n[![Python](https://img.shields.io/pypi/pyversions/kuflow-temporal-activity-kuflow.svg)](https://pypi.org/project/kuflow-temporal-activity-kuflow)\n[![PyPI](https://img.shields.io/pypi/v/kuflow-temporal-activity-kuflow.svg)](https://pypi.org/project/kuflow-temporal-activity-kuflow)\n\n# KuFlow Temporal Activities KuFlow\n\nTemporal.io activities to interact with KuFlow\n\n## Documentation\n\nMore detailed docs are available in the [documentation pages](https://docs.kuflow.com/developers/).\n\n## Contributing\n\nWe are happy to receive your help and comments, together we will dance a wonderful KuFlow. Please review our [contribution guide](CONTRIBUTING.md).\n\n## License\n\n[MIT License](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)\n',
     'author': 'KuFlow S.L.',
     'author_email': 'kuflow@kuflow.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://kuflow.com/',
```

### Comparing `kuflow_temporal_activity_kuflow-0.6.1/PKG-INFO` & `kuflow_temporal_activity_kuflow-0.7.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: kuflow-temporal-activity-kuflow
-Version: 0.6.1
+Version: 0.7.0
 Summary: KuFlow SDK :: Temporal.io activities to interact with KuFlow
 Home-page: https://kuflow.com/
 License: MIT
 Author: KuFlow S.L.
 Author-email: kuflow@kuflow.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: kuflow-temporal-common (>=0.6.1,<0.7.0)
+Requires-Dist: kuflow-temporal-common (>=0.7.0,<0.8.0)
 Project-URL: Documentation, https://docs.kuflow.com/
 Project-URL: Repository, https://github.com/kuflow/kuflow-sdk-python
 Description-Content-Type: text/markdown
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/kuflow/kuflow-sdk-python/blob/master/LICENSE)
 [![Python](https://img.shields.io/pypi/pyversions/kuflow-temporal-activity-kuflow.svg)](https://pypi.org/project/kuflow-temporal-activity-kuflow)
 [![PyPI](https://img.shields.io/pypi/v/kuflow-temporal-activity-kuflow.svg)](https://pypi.org/project/kuflow-temporal-activity-kuflow)
```

