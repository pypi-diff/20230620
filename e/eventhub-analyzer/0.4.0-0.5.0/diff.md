# Comparing `tmp/eventhub_analyzer-0.4.0.tar.gz` & `tmp/eventhub_analyzer-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventhub_analyzer-0.4.0.tar", max compression
+gzip compressed data, was "eventhub_analyzer-0.5.0.tar", max compression
```

## Comparing `eventhub_analyzer-0.4.0.tar` & `eventhub_analyzer-0.5.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1933 2023-02-15 17:11:16.847513 eventhub_analyzer-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-01-31 13:29:42.523481 eventhub_analyzer-0.4.0/eventhub_analyzer/__init__.py
--rw-r--r--   0        0        0    12354 2023-02-22 15:59:56.060035 eventhub_analyzer-0.4.0/eventhub_analyzer/main.py
--rw-r--r--   0        0        0      626 2023-04-26 09:23:50.328721 eventhub_analyzer-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2948 1970-01-01 00:00:00.000000 eventhub_analyzer-0.4.0/setup.py
--rw-r--r--   0        0        0     2713 1970-01-01 00:00:00.000000 eventhub_analyzer-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2041 2023-04-26 09:25:09.524728 eventhub_analyzer-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2023-01-31 13:29:42.523481 eventhub_analyzer-0.5.0/eventhub_analyzer/__init__.py
+-rw-r--r--   0        0        0    12354 2023-02-22 15:59:56.060035 eventhub_analyzer-0.5.0/eventhub_analyzer/main.py
+-rw-r--r--   0        0        0      626 2023-06-20 12:54:14.916880 eventhub_analyzer-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3069 1970-01-01 00:00:00.000000 eventhub_analyzer-0.5.0/setup.py
+-rw-r--r--   0        0        0     2821 1970-01-01 00:00:00.000000 eventhub_analyzer-0.5.0/PKG-INFO
```

### Comparing `eventhub_analyzer-0.4.0/README.md` & `eventhub_analyzer-0.5.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # Event Hub Analyzer
 
 Event Hub Analyzer is a small command line tool that can be used
 to analyze certain aspects of Event Hubs.
 
+## Installation
+
+```
+pip install eventhub-analyzer
+```
+
 ## Checkpoints per partition
 
 For every event hub, consumer group, the number of 
 events/sequence numbers between two invocations is retrieved and
 the throughput per partition is calculated. This can be used to 
 determine if the load is correctly distributed among partitions.
 
@@ -45,7 +51,14 @@
 telemetry   my-consumer              8             118.351
 ```
 
 As you can see, partition 3 is not getting any events and
 the number of events is not well distributed overall. There
 might be some gains possible by choosing a different partition key
 (or by partitioning manually on the client).
+
+## Publishing
+
+```
+poetry build
+poetry publish
+```
```

### Comparing `eventhub_analyzer-0.4.0/eventhub_analyzer/main.py` & `eventhub_analyzer-0.5.0/eventhub_analyzer/main.py`

 * *Files identical despite different names*

### Comparing `eventhub_analyzer-0.4.0/pyproject.toml` & `eventhub_analyzer-0.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eventhub-analyzer"
-version = "0.4.0"
+version = "0.5.0"
 description = ""
 authors = ["Stefan Hudelmaier <stefan.hudelmaier@device-insight.com>"]
 readme = "README.md"
 packages = [{include = "eventhub_analyzer"}]
 repository = "https://github.com/deviceinsight/eventhub-analyzer"
 
 [tool.poetry.dependencies]
```

### Comparing `eventhub_analyzer-0.4.0/setup.py` & `eventhub_analyzer-0.5.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,17 +16,17 @@
  'texttable>=1.6.7,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['eventhub-analyzer = eventhub_analyzer.main:cli']}
 
 setup_kwargs = {
     'name': 'eventhub-analyzer',
-    'version': '0.4.0',
+    'version': '0.5.0',
     'description': '',
-    'long_description': "# Event Hub Analyzer\n\nEvent Hub Analyzer is a small command line tool that can be used\nto analyze certain aspects of Event Hubs.\n\n## Checkpoints per partition\n\nFor every event hub, consumer group, the number of \nevents/sequence numbers between two invocations is retrieved and\nthe throughput per partition is calculated. This can be used to \ndetermine if the load is correctly distributed among partitions.\n\nWhen there are some partition that get little to no throughput while\nothers have large throughput, it is a sign that the partition key\nis not chosen optimally and that you should try to choose a property\nwith a higher cardinality as the partition key.\n\n### Usage\n\n```bash\neventhub-analyzer checkpoints -n CONTAINER_NAME -c CONNECTION_STRING\n```\n\nYou can also specify the settings via environment variables:\n\n```bash\nexport STORAGE_ACCOUNT_CONNECTION_STRING='DefaultEndpointsProtocol=https;AccountName=x;AccountKey=y;EndpointSuffix=core.windows.net'\nexport CONTAINER_NAME='event-hub-offsets'\neventhub-analyzer checkpoints\n```\n\n### Example output\n\n```\nEvent Hub: telemetry, Consumer Group: my-consumer\nEvent Hub   Consumer Group   Partition   Events per second\ntelemetry   my-consumer              0             158.034\ntelemetry   my-consumer              1             203.257\ntelemetry   my-consumer              2             148.103\ntelemetry   my-consumer              3               0.000\ntelemetry   my-consumer              4             201.780\ntelemetry   my-consumer              5             106.081\ntelemetry   my-consumer              6              72.307\ntelemetry   my-consumer              7             160.783\ntelemetry   my-consumer              8             118.351\n```\n\nAs you can see, partition 3 is not getting any events and\nthe number of events is not well distributed overall. There\nmight be some gains possible by choosing a different partition key\n(or by partitioning manually on the client).\n",
+    'long_description': "# Event Hub Analyzer\n\nEvent Hub Analyzer is a small command line tool that can be used\nto analyze certain aspects of Event Hubs.\n\n## Installation\n\n```\npip install eventhub-analyzer\n```\n\n## Checkpoints per partition\n\nFor every event hub, consumer group, the number of \nevents/sequence numbers between two invocations is retrieved and\nthe throughput per partition is calculated. This can be used to \ndetermine if the load is correctly distributed among partitions.\n\nWhen there are some partition that get little to no throughput while\nothers have large throughput, it is a sign that the partition key\nis not chosen optimally and that you should try to choose a property\nwith a higher cardinality as the partition key.\n\n### Usage\n\n```bash\neventhub-analyzer checkpoints -n CONTAINER_NAME -c CONNECTION_STRING\n```\n\nYou can also specify the settings via environment variables:\n\n```bash\nexport STORAGE_ACCOUNT_CONNECTION_STRING='DefaultEndpointsProtocol=https;AccountName=x;AccountKey=y;EndpointSuffix=core.windows.net'\nexport CONTAINER_NAME='event-hub-offsets'\neventhub-analyzer checkpoints\n```\n\n### Example output\n\n```\nEvent Hub: telemetry, Consumer Group: my-consumer\nEvent Hub   Consumer Group   Partition   Events per second\ntelemetry   my-consumer              0             158.034\ntelemetry   my-consumer              1             203.257\ntelemetry   my-consumer              2             148.103\ntelemetry   my-consumer              3               0.000\ntelemetry   my-consumer              4             201.780\ntelemetry   my-consumer              5             106.081\ntelemetry   my-consumer              6              72.307\ntelemetry   my-consumer              7             160.783\ntelemetry   my-consumer              8             118.351\n```\n\nAs you can see, partition 3 is not getting any events and\nthe number of events is not well distributed overall. There\nmight be some gains possible by choosing a different partition key\n(or by partitioning manually on the client).\n\n## Publishing\n\n```\npoetry build\npoetry publish\n```\n",
     'author': 'Stefan Hudelmaier',
     'author_email': 'stefan.hudelmaier@device-insight.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/deviceinsight/eventhub-analyzer',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `eventhub_analyzer-0.4.0/PKG-INFO` & `eventhub_analyzer-0.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eventhub-analyzer
-Version: 0.4.0
+Version: 0.5.0
 Summary: 
 Home-page: https://github.com/deviceinsight/eventhub-analyzer
 Author: Stefan Hudelmaier
 Author-email: stefan.hudelmaier@device-insight.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -19,14 +19,20 @@
 Description-Content-Type: text/markdown
 
 # Event Hub Analyzer
 
 Event Hub Analyzer is a small command line tool that can be used
 to analyze certain aspects of Event Hubs.
 
+## Installation
+
+```
+pip install eventhub-analyzer
+```
+
 ## Checkpoints per partition
 
 For every event hub, consumer group, the number of 
 events/sequence numbers between two invocations is retrieved and
 the throughput per partition is calculated. This can be used to 
 determine if the load is correctly distributed among partitions.
 
@@ -66,7 +72,14 @@
 ```
 
 As you can see, partition 3 is not getting any events and
 the number of events is not well distributed overall. There
 might be some gains possible by choosing a different partition key
 (or by partitioning manually on the client).
 
+## Publishing
+
+```
+poetry build
+poetry publish
+```
+
```

