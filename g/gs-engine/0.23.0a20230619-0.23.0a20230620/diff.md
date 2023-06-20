# Comparing `tmp/gs_engine-0.23.0a20230619-py2.py3-none-any.whl.zip` & `tmp/gs_engine-0.23.0a20230620-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 11894 bytes, number of entries: 9
--rw-r--r--  2.0 unx      398 b- defN 23-Jun-19 19:02 graphscope.runtime/conf/executor.vineyard.properties
--rw-r--r--  2.0 unx      505 b- defN 23-Jun-19 19:02 graphscope.runtime/conf/frontend.vineyard.properties
--rw-r--r--  2.0 unx     1573 b- defN 23-Jun-19 19:02 graphscope.runtime/conf/log4j2.xml
--rw-r--r--  2.0 unx      204 b- defN 23-Jun-19 19:02 graphscope.runtime/conf/log4rs.yml
--rw-r--r--  2.0 unx      694 b- defN 23-Jun-19 19:02 graphscope_runtime/__init__.py
--rw-r--r--  2.0 unx    21680 b- defN 23-Jun-19 20:32 gs_engine-0.23.0a20230619.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jun-19 20:32 gs_engine-0.23.0a20230619.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 23-Jun-19 20:32 gs_engine-0.23.0a20230619.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      831 b- defN 23-Jun-19 20:32 gs_engine-0.23.0a20230619.dist-info/RECORD
-9 files, 26014 bytes uncompressed, 10432 bytes compressed:  59.9%
+Zip file size: 11897 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      398 b- defN 23-Jun-20 19:02 graphscope.runtime/conf/executor.vineyard.properties
+-rw-r--r--  2.0 unx      503 b- defN 23-Jun-20 19:02 graphscope.runtime/conf/frontend.vineyard.properties
+-rw-r--r--  2.0 unx     1573 b- defN 23-Jun-20 19:02 graphscope.runtime/conf/log4j2.xml
+-rw-r--r--  2.0 unx      204 b- defN 23-Jun-20 19:02 graphscope.runtime/conf/log4rs.yml
+-rw-r--r--  2.0 unx      694 b- defN 23-Jun-20 19:02 graphscope_runtime/__init__.py
+-rw-r--r--  2.0 unx    21680 b- defN 23-Jun-20 20:38 gs_engine-0.23.0a20230620.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-20 20:38 gs_engine-0.23.0a20230620.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 23-Jun-20 20:38 gs_engine-0.23.0a20230620.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      831 b- defN 23-Jun-20 20:38 gs_engine-0.23.0a20230620.dist-info/RECORD
+9 files, 26012 bytes uncompressed, 10435 bytes compressed:  59.9%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: graphscope.runtime/conf/log4rs.yml
 Comment: 
 
 Filename: graphscope_runtime/__init__.py
 Comment: 
 
-Filename: gs_engine-0.23.0a20230619.dist-info/METADATA
+Filename: gs_engine-0.23.0a20230620.dist-info/METADATA
 Comment: 
 
-Filename: gs_engine-0.23.0a20230619.dist-info/WHEEL
+Filename: gs_engine-0.23.0a20230620.dist-info/WHEEL
 Comment: 
 
-Filename: gs_engine-0.23.0a20230619.dist-info/top_level.txt
+Filename: gs_engine-0.23.0a20230620.dist-info/top_level.txt
 Comment: 
 
-Filename: gs_engine-0.23.0a20230619.dist-info/RECORD
+Filename: gs_engine-0.23.0a20230620.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## graphscope.runtime/conf/frontend.vineyard.properties

```diff
@@ -10,12 +10,12 @@
 # e.g. 1.2.3.4:1234,1.2.3.5:1234
 pegasus.hosts = PEGASUS_HOSTS
 
 # graph schema path
 graph.schema = GRAPH_SCHEMA
 
 ## Frontend Config
-frontend.service.port = FRONTEND_SERVICE_PORT
+gremlin.server.port = FRONTEND_SERVICE_PORT
 
 # disable the authentication if username or password is not set
 #auth.username = default
 #auth.password = default
```

## Comparing `gs_engine-0.23.0a20230619.dist-info/METADATA` & `gs_engine-0.23.0a20230620.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gs-engine
-Version: 0.23.0a20230619
+Version: 0.23.0a20230620
 Home-page: https://github.com/alibaba/GraphScope
 Author: GraphScope Team, Damo Academy
 Author-email: graphscope@alibaba-inc.com
 License: Apache License 2.0
 Keywords: GraphScope,Graph Computations
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

