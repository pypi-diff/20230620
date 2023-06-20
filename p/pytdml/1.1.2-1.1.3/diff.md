# Comparing `tmp/pytdml-1.1.2.tar.gz` & `tmp/pytdml-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytdml-1.1.2.tar", last modified: Mon Jun 19 07:55:25 2023, max compression
+gzip compressed data, was "pytdml-1.1.3.tar", last modified: Tue Jun 20 07:24:24 2023, max compression
```

## Comparing `pytdml-1.1.2.tar` & `pytdml-1.1.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 07:55:25.633661 pytdml-1.1.2/
--rw-rw-rw-   0        0        0     1141 2023-06-14 03:12:17.000000 pytdml-1.1.2/LICENSE
--rw-rw-rw-   0        0        0     8708 2023-06-19 07:55:25.633661 pytdml-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     8083 2023-06-19 07:47:45.000000 pytdml-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 07:55:25.613715 pytdml-1.1.2/examples/
--rw-rw-rw-   0        0        0        0 2023-06-14 03:12:17.000000 pytdml-1.1.2/examples/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 07:55:25.616706 pytdml-1.1.2/pytdml/
--rw-rw-rw-   0        0        0     1608 2023-06-19 07:55:16.000000 pytdml-1.1.2/pytdml/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 07:55:25.625683 pytdml-1.1.2/pytdml/io/
--rw-rw-rw-   0        0        0     2598 2023-06-15 12:28:34.000000 pytdml-1.1.2/pytdml/io/S3_reader.py
--rw-rw-rw-   0        0        0     1686 2023-06-13 07:20:48.000000 pytdml-1.1.2/pytdml/io/__init__.py
--rw-rw-rw-   0        0        0     2250 2023-06-14 03:12:18.000000 pytdml-1.1.2/pytdml/io/tdml_readers.py
--rw-rw-rw-   0        0        0     1959 2023-06-14 03:12:18.000000 pytdml-1.1.2/pytdml/io/tdml_writers.py
-drwxrwxrwx   0        0        0        0 2023-06-19 07:55:25.628674 pytdml-1.1.2/pytdml/ml/
--rw-rw-rw-   0        0        0     1854 2023-06-14 03:12:18.000000 pytdml-1.1.2/pytdml/ml/__init__.py
--rw-rw-rw-   0        0        0     2640 2023-06-14 03:12:18.000000 pytdml-1.1.2/pytdml/ml/ml_operators.py
--rw-rw-rw-   0        0        0     6151 2023-06-14 03:12:18.000000 pytdml-1.1.2/pytdml/ml/tdml_tensorflow.py
--rw-rw-rw-   0        0        0     5396 2023-06-14 03:12:18.000000 pytdml-1.1.2/pytdml/ml/tdml_torch.py
--rw-rw-rw-   0        0        0     4988 2023-06-14 03:12:18.000000 pytdml-1.1.2/pytdml/tdml_image_crop.py
-drwxrwxrwx   0        0        0        0 2023-06-19 07:55:25.631666 pytdml-1.1.2/pytdml/type/
--rw-rw-rw-   0        0        0     1828 2023-06-14 03:12:18.000000 pytdml-1.1.2/pytdml/type/__init__.py
--rw-rw-rw-   0        0        0    22698 2023-06-14 03:12:18.000000 pytdml-1.1.2/pytdml/type/basic_types.py
--rw-rw-rw-   0        0        0    16253 2023-06-14 03:12:18.000000 pytdml-1.1.2/pytdml/type/extended_types.py
--rw-rw-rw-   0        0        0     4537 2023-06-14 03:12:18.000000 pytdml-1.1.2/pytdml/utils.py
--rw-rw-rw-   0        0        0    15294 2023-06-14 03:12:18.000000 pytdml-1.1.2/pytdml/yaml_to_tdml.py
-drwxrwxrwx   0        0        0        0 2023-06-19 07:55:25.621693 pytdml-1.1.2/pytdml.egg-info/
--rw-rw-rw-   0        0        0     8708 2023-06-19 07:55:25.000000 pytdml-1.1.2/pytdml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      577 2023-06-19 07:55:25.000000 pytdml-1.1.2/pytdml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 07:55:25.000000 pytdml-1.1.2/pytdml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-06-19 07:55:25.000000 pytdml-1.1.2/pytdml.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-19 07:55:25.000000 pytdml-1.1.2/pytdml.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 07:55:25.633661 pytdml-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     3136 2023-06-14 03:12:18.000000 pytdml-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 07:55:25.632664 pytdml-1.1.2/tests/
--rw-rw-rw-   0        0        0        0 2023-06-14 03:12:18.000000 pytdml-1.1.2/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 07:24:24.374635 pytdml-1.1.3/
+-rw-rw-rw-   0        0        0     1141 2023-06-14 03:12:17.000000 pytdml-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0     8708 2023-06-20 07:24:24.374635 pytdml-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     8083 2023-06-19 07:47:45.000000 pytdml-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 07:24:24.294848 pytdml-1.1.3/examples/
+-rw-rw-rw-   0        0        0        0 2023-06-14 03:12:17.000000 pytdml-1.1.3/examples/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 07:24:24.312801 pytdml-1.1.3/pytdml/
+-rw-rw-rw-   0        0        0     1608 2023-06-20 07:24:21.000000 pytdml-1.1.3/pytdml/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 07:24:24.330752 pytdml-1.1.3/pytdml/io/
+-rw-rw-rw-   0        0        0     2596 2023-06-20 07:14:44.000000 pytdml-1.1.3/pytdml/io/S3_reader.py
+-rw-rw-rw-   0        0        0     1686 2023-06-13 07:20:48.000000 pytdml-1.1.3/pytdml/io/__init__.py
+-rw-rw-rw-   0        0        0     2250 2023-06-14 03:12:18.000000 pytdml-1.1.3/pytdml/io/tdml_readers.py
+-rw-rw-rw-   0        0        0     1959 2023-06-14 03:12:18.000000 pytdml-1.1.3/pytdml/io/tdml_writers.py
+drwxrwxrwx   0        0        0        0 2023-06-20 07:24:24.354688 pytdml-1.1.3/pytdml/ml/
+-rw-rw-rw-   0        0        0     1854 2023-06-14 03:12:18.000000 pytdml-1.1.3/pytdml/ml/__init__.py
+-rw-rw-rw-   0        0        0     2640 2023-06-14 03:12:18.000000 pytdml-1.1.3/pytdml/ml/ml_operators.py
+-rw-rw-rw-   0        0        0     6151 2023-06-14 03:12:18.000000 pytdml-1.1.3/pytdml/ml/tdml_tensorflow.py
+-rw-rw-rw-   0        0        0     5396 2023-06-14 03:12:18.000000 pytdml-1.1.3/pytdml/ml/tdml_torch.py
+-rw-rw-rw-   0        0        0     4988 2023-06-14 03:12:18.000000 pytdml-1.1.3/pytdml/tdml_image_crop.py
+drwxrwxrwx   0        0        0        0 2023-06-20 07:24:24.372640 pytdml-1.1.3/pytdml/type/
+-rw-rw-rw-   0        0        0     1828 2023-06-14 03:12:18.000000 pytdml-1.1.3/pytdml/type/__init__.py
+-rw-rw-rw-   0        0        0    22515 2023-06-20 07:10:26.000000 pytdml-1.1.3/pytdml/type/basic_types.py
+-rw-rw-rw-   0        0        0    16253 2023-06-14 03:12:18.000000 pytdml-1.1.3/pytdml/type/extended_types.py
+-rw-rw-rw-   0        0        0     4537 2023-06-14 03:12:18.000000 pytdml-1.1.3/pytdml/utils.py
+-rw-rw-rw-   0        0        0    15294 2023-06-14 03:12:18.000000 pytdml-1.1.3/pytdml/yaml_to_tdml.py
+drwxrwxrwx   0        0        0        0 2023-06-20 07:24:24.326763 pytdml-1.1.3/pytdml.egg-info/
+-rw-rw-rw-   0        0        0     8708 2023-06-20 07:24:23.000000 pytdml-1.1.3/pytdml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      577 2023-06-20 07:24:23.000000 pytdml-1.1.3/pytdml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 07:24:23.000000 pytdml-1.1.3/pytdml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-06-20 07:24:23.000000 pytdml-1.1.3/pytdml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-20 07:24:23.000000 pytdml-1.1.3/pytdml.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 07:24:24.375632 pytdml-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     3136 2023-06-14 03:12:18.000000 pytdml-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 07:24:24.373638 pytdml-1.1.3/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-20 07:21:16.000000 pytdml-1.1.3/tests/__init__.py
```

### Comparing `pytdml-1.1.2/LICENSE` & `pytdml-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytdml-1.1.2/PKG-INFO` & `pytdml-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytdml
-Version: 1.1.2
+Version: 1.1.3
 Summary: Parsing and encoding training datasets based on OGC Training Data Markup Language for AI (TrainingDML-AI) standard
 Home-page: https://github.com/TrainingDML/pytdml
 Author: Boyi Shangguan
 Author-email: sgby@whu.edu.cn
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pytdml-1.1.2/README.md` & `pytdml-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pytdml-1.1.2/pytdml/__init__.py` & `pytdml-1.1.3/pytdml/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,8 +28,8 @@
 # SOFTWARE.
 #
 # ------------------------------------------------------------------------------
 import pytdml.type
 import pytdml.io
 
 name = 'pytdml'
-__version__ = '1.1.2'
+__version__ = '1.1.3'
```

### Comparing `pytdml-1.1.2/pytdml/io/S3_reader.py` & `pytdml-1.1.3/pytdml/io/S3_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,19 +36,20 @@
         # Print storage bucket name
         bucket_list = []
         for bucket in response['Buckets']:
             bucket_list.append(bucket)
         return bucket_list
 
     def list_objects(self, bucket_name, prefix):
+        obj_list = []
         try:
             # 列出存储桶中的对象
             response = self.s3_client.list_objects_v2(Bucket=bucket_name, Prefix=prefix)
             # 打印对象列表
-            obj_list = []
+
             if 'Contents' in response:
                 for obj in response['Contents']:
                     obj_list.append(obj['Key'])
             else:
                 print("There are no objects in the storage bucket: " + bucket_name)
 
         except Exception as e:
```

### Comparing `pytdml-1.1.2/pytdml/io/__init__.py` & `pytdml-1.1.3/pytdml/io/__init__.py`

 * *Files identical despite different names*

### Comparing `pytdml-1.1.2/pytdml/io/tdml_readers.py` & `pytdml-1.1.3/pytdml/io/tdml_readers.py`

 * *Files identical despite different names*

### Comparing `pytdml-1.1.2/pytdml/io/tdml_writers.py` & `pytdml-1.1.3/pytdml/io/tdml_writers.py`

 * *Files identical despite different names*

### Comparing `pytdml-1.1.2/pytdml/ml/__init__.py` & `pytdml-1.1.3/pytdml/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `pytdml-1.1.2/pytdml/ml/ml_operators.py` & `pytdml-1.1.3/pytdml/ml/ml_operators.py`

 * *Files identical despite different names*

### Comparing `pytdml-1.1.2/pytdml/ml/tdml_tensorflow.py` & `pytdml-1.1.3/pytdml/ml/tdml_tensorflow.py`

 * *Files identical despite different names*

### Comparing `pytdml-1.1.2/pytdml/ml/tdml_torch.py` & `pytdml-1.1.3/pytdml/ml/tdml_torch.py`

 * *Files identical despite different names*

### Comparing `pytdml-1.1.2/pytdml/tdml_image_crop.py` & `pytdml-1.1.3/pytdml/tdml_image_crop.py`

 * *Files identical despite different names*

### Comparing `pytdml-1.1.2/pytdml/type/__init__.py` & `pytdml-1.1.3/pytdml/type/__init__.py`

 * *Files identical despite different names*

### Comparing `pytdml-1.1.2/pytdml/type/basic_types.py` & `pytdml-1.1.3/pytdml/type/basic_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 @dataclass
 class MetricsInLiterature:
     """
     Metrics in literature type
     """
     doi: str
     algorithm: str = field(default=None)
-    metrics: List[KeyValuePair] = field(default_factory=list[KeyValuePair])
+    metrics: List[KeyValuePair] = field(default_factory=list)
 
     def to_dict(self):
         return {
             "doi": self.doi,
             "algorithm": self.algorithm,
             "metrics": [m.to_dict() for m in self.metrics]
         }
@@ -139,16 +139,16 @@
 
 @dataclass
 class LabelingProcedure:
     """
     Labeling procedure type
     """
     id: str
-    methods: list[str] = field(default_factory=list)
-    tools: list[str] = field(default_factory=list)
+    methods: List[str] = field(default_factory=list)
+    tools: List[str] = field(default_factory=list)
 
     def to_dict(self):
         return {
             "type": "LabelingProcedure",
             "id": self.id,
             "methods": self.methods,
             "tools": self.tools
@@ -200,18 +200,18 @@
 
 
 @dataclass
 class ScopeDescription:
     """
     From ISO 19115-1 MD_ScopeDescription
     """
-    attributes: list[str] = field(default_factory=list)
-    features: list[str] = field(default_factory=list)
-    featureInstances: list[str] = field(default_factory=list)
-    attributeInstances: list[str] = field(default_factory=list)
+    attributes: List[str] = field(default_factory=list)
+    features: List[str] = field(default_factory=list)
+    featureInstances: List[str] = field(default_factory=list)
+    attributeInstances: List[str] = field(default_factory=list)
     dataset: str = field(default=None)
     other: str = field(default=None)
 
     def to_dict(self):
         return {
             "attributes": self.attributes,
             "features": self.features,
@@ -241,15 +241,15 @@
 
 @dataclass
 class Scope:
     """
     From ISO 19115-1 MD_Scope
     """
     level: str
-    levelDescription: List[ScopeDescription] = field(default_factory=list[ScopeDescription])
+    levelDescription: List[ScopeDescription] = field(default_factory=list)
 
     def to_dict(self):
         return {
             "level": self.level,
             "levelDescription": [ld.to_dict for ld in self.levelDescription]
         }
 
@@ -298,15 +298,15 @@
 
 @dataclass
 class DataQuality:
     """
     From ISO 19157-1 DataQuality
     """
     scope: Scope
-    report: List[QualityElement] = field(default_factory=list[QualityElement])
+    report: List[QualityElement] = field(default_factory=list)
 
     def to_dict(self):
         return {
             "scope": self.scope.to_dict() if self.scope is not None else None,
             "report": [r.to_dict() for r in self.report],
         }
 
@@ -356,16 +356,16 @@
     """
     id: str
     dataset_id: str = field(default=None)
     training_type: str = field(default=None)
     number_of_labels: int = field(default=None)
     data_sources: List[str] = field(default_factory=list)
     quality: DataQuality = field(default=None)
-    labeling: List[Labeling] = field(default_factory=list[Labeling])
-    labels: List[Label] = field(default_factory=list[Label])
+    labeling: List[Labeling] = field(default_factory=list)
+    labels: List[Label] = field(default_factory=list)
 
     def get_labels(self) -> List[Label]:
         """
         Returns the labels of the training data
         """
         return self.labels
 
@@ -408,17 +408,17 @@
     Training Data Changeset
     """
     id: str
     change_count: int
     dataset_id: str = field(default=None)
     version: str = field(default=None)
     created_time: str = field(default=None)
-    add: List[TrainingData] = field(default_factory=list[TrainingData])
-    modify: List[TrainingData] = field(default_factory=list[TrainingData])
-    delete: List[TrainingData] = field(default_factory=list[TrainingData])
+    add: List[TrainingData] = field(default_factory=list)
+    modify: List[TrainingData] = field(default_factory=list)
+    delete: List[TrainingData] = field(default_factory=list)
 
     def to_dict(self):
         return {
             "type": "TDChangeset",
             "id": self.id,
             "changeCount": self.change_count,
             "datasetId": self.dataset_id,
@@ -464,25 +464,25 @@
     scope: Scope = field(default=None)
     version: str = field(default=None)
     amount_of_training_data: int = field(default=None)
     created_time: str = field(default=None)
     updated_time: str = field(default=None)
     providers: List[str] = field(default_factory=list)
     keywords: List[str] = field(default_factory=list)
-    metrics_in_literature: List[MetricsInLiterature] = field(default_factory=list[MetricsInLiterature])
-    statistics_info: List[KeyValuePair] = field(default_factory=list[KeyValuePair])
+    metrics_in_literature: List[MetricsInLiterature] = field(default_factory=list)
+    statistics_info: List[KeyValuePair] = field(default_factory=list)
     dataSources: List[str] = field(default_factory=list)
     number_of_classes: int = field(default=None)
     classification_schema: str = field(default=None)
     classes: Union[List[KeyValuePair], List[str]] = field(default=None)
-    tasks: List[Task] = field(default_factory=list[Task])
-    labeling: List[Labeling] = field(default_factory=list[Labeling])
+    tasks: List[Task] = field(default_factory=list)
+    labeling: List[Labeling] = field(default_factory=list)
     quality: DataQuality = field(default=None)
-    changesets: List[Changeset] = field(default_factory=list[Changeset])
-    data: List[TrainingData] = field(default_factory=list[TrainingData])
+    changesets: List[Changeset] = field(default_factory=list)
+    data: List[TrainingData] = field(default_factory=list)
 
     def get_training_data(self) -> List[TrainingData]:
         """
         Return the training data of the training dataset
         """
         return self.data
```

### Comparing `pytdml-1.1.2/pytdml/type/extended_types.py` & `pytdml-1.1.3/pytdml/type/extended_types.py`

 * *Files identical despite different names*

### Comparing `pytdml-1.1.2/pytdml/utils.py` & `pytdml-1.1.3/pytdml/utils.py`

 * *Files identical despite different names*

### Comparing `pytdml-1.1.2/pytdml/yaml_to_tdml.py` & `pytdml-1.1.3/pytdml/yaml_to_tdml.py`

 * *Files identical despite different names*

### Comparing `pytdml-1.1.2/pytdml.egg-info/PKG-INFO` & `pytdml-1.1.3/pytdml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytdml
-Version: 1.1.2
+Version: 1.1.3
 Summary: Parsing and encoding training datasets based on OGC Training Data Markup Language for AI (TrainingDML-AI) standard
 Home-page: https://github.com/TrainingDML/pytdml
 Author: Boyi Shangguan
 Author-email: sgby@whu.edu.cn
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pytdml-1.1.2/pytdml.egg-info/SOURCES.txt` & `pytdml-1.1.3/pytdml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytdml-1.1.2/setup.py` & `pytdml-1.1.3/setup.py`

 * *Files identical despite different names*

