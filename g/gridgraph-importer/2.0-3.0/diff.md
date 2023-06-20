# Comparing `tmp/gridgraph_importer-2.0.tar.gz` & `tmp/gridgraph_importer-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridgraph_importer-2.0.tar", last modified: Fri Jun 16 02:39:11 2023, max compression
+gzip compressed data, was "gridgraph_importer-3.0.tar", last modified: Tue Jun 20 06:03:37 2023, max compression
```

## Comparing `gridgraph_importer-2.0.tar` & `gridgraph_importer-3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 hetao      (501) staff       (20)        0 2023-06-16 02:39:11.191283 gridgraph_importer-2.0/
--rw-r--r--   0 hetao      (501) staff       (20)      904 2023-06-16 02:39:11.191151 gridgraph_importer-2.0/PKG-INFO
--rw-r--r--   0 hetao      (501) staff       (20)      144 2023-06-16 02:12:05.000000 gridgraph_importer-2.0/README.md
-drwxr-xr-x   0 hetao      (501) staff       (20)        0 2023-06-16 02:39:11.190353 gridgraph_importer-2.0/gridgraph_importer/
--rw-r--r--   0 hetao      (501) staff       (20)        0 2023-06-16 02:22:33.000000 gridgraph_importer-2.0/gridgraph_importer/__init__.py
--rwxr-xr-x   0 hetao      (501) staff       (20)     3674 2023-06-13 06:32:12.000000 gridgraph_importer-2.0/gridgraph_importer/colour.py
--rw-r--r--   0 hetao      (501) staff       (20)    11988 2023-06-16 02:38:21.000000 gridgraph_importer-2.0/gridgraph_importer/data_importer.py
--rw-r--r--   0 hetao      (501) staff       (20)     1719 2023-06-16 02:38:21.000000 gridgraph_importer-2.0/gridgraph_importer/log_utils.py
-drwxr-xr-x   0 hetao      (501) staff       (20)        0 2023-06-16 02:39:11.190980 gridgraph_importer-2.0/gridgraph_importer.egg-info/
--rw-r--r--   0 hetao      (501) staff       (20)      904 2023-06-16 02:39:11.000000 gridgraph_importer-2.0/gridgraph_importer.egg-info/PKG-INFO
--rw-r--r--   0 hetao      (501) staff       (20)      314 2023-06-16 02:39:11.000000 gridgraph_importer-2.0/gridgraph_importer.egg-info/SOURCES.txt
--rw-r--r--   0 hetao      (501) staff       (20)        1 2023-06-16 02:39:11.000000 gridgraph_importer-2.0/gridgraph_importer.egg-info/dependency_links.txt
--rw-r--r--   0 hetao      (501) staff       (20)       19 2023-06-16 02:39:11.000000 gridgraph_importer-2.0/gridgraph_importer.egg-info/top_level.txt
--rw-r--r--   0 hetao      (501) staff       (20)       38 2023-06-16 02:39:11.191328 gridgraph_importer-2.0/setup.cfg
--rw-r--r--   0 hetao      (501) staff       (20)     1071 2023-06-16 02:39:06.000000 gridgraph_importer-2.0/setup.py
+drwxrwxr-x   0 taohe     (1000) taohe     (1000)        0 2023-06-20 06:03:37.994659 gridgraph_importer-3.0/
+-rw-rw-r--   0 taohe     (1000) taohe     (1000)     1690 2023-06-20 06:03:37.994659 gridgraph_importer-3.0/PKG-INFO
+-rw-r--r--   0 taohe     (1000) taohe     (1000)      930 2023-06-20 06:00:25.000000 gridgraph_importer-3.0/README.md
+drwxrwxr-x   0 taohe     (1000) taohe     (1000)        0 2023-06-20 06:03:37.994659 gridgraph_importer-3.0/gridgraph_importer/
+-rw-r--r--   0 taohe     (1000) taohe     (1000)        0 2023-06-16 10:22:32.000000 gridgraph_importer-3.0/gridgraph_importer/__init__.py
+-rw-r--r--   0 taohe     (1000) taohe     (1000)     3596 2023-06-19 00:49:51.000000 gridgraph_importer-3.0/gridgraph_importer/colour.py
+-rw-r--r--   0 taohe     (1000) taohe     (1000)    18052 2023-06-20 05:58:50.000000 gridgraph_importer-3.0/gridgraph_importer/data_importer.py
+-rw-r--r--   0 taohe     (1000) taohe     (1000)     2237 2023-06-19 00:54:58.000000 gridgraph_importer-3.0/gridgraph_importer/log_utils.py
+drwxrwxr-x   0 taohe     (1000) taohe     (1000)        0 2023-06-20 06:03:37.994659 gridgraph_importer-3.0/gridgraph_importer.egg-info/
+-rw-r--r--   0 taohe     (1000) taohe     (1000)     1690 2023-06-20 06:03:37.000000 gridgraph_importer-3.0/gridgraph_importer.egg-info/PKG-INFO
+-rw-r--r--   0 taohe     (1000) taohe     (1000)      314 2023-06-20 06:03:37.000000 gridgraph_importer-3.0/gridgraph_importer.egg-info/SOURCES.txt
+-rw-r--r--   0 taohe     (1000) taohe     (1000)        1 2023-06-20 06:03:37.000000 gridgraph_importer-3.0/gridgraph_importer.egg-info/dependency_links.txt
+-rw-r--r--   0 taohe     (1000) taohe     (1000)       19 2023-06-20 06:03:37.000000 gridgraph_importer-3.0/gridgraph_importer.egg-info/top_level.txt
+-rw-rw-r--   0 taohe     (1000) taohe     (1000)       38 2023-06-20 06:03:37.994659 gridgraph_importer-3.0/setup.cfg
+-rw-r--r--   0 taohe     (1000) taohe     (1000)     1071 2023-06-20 06:03:29.000000 gridgraph_importer-3.0/setup.py
```

### Comparing `gridgraph_importer-2.0/gridgraph_importer/colour.py` & `gridgraph_importer-3.0/gridgraph_importer/colour.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,31 +7,27 @@
 # DISCLOSURE.
 #
 # THIS SOFTWARE CONTAINS CONFIDENTIAL INFORMATION AND TRADE SECRETS OF
 # 方图数据（北京）软件股份有限公司. USE, DISCLOSURE, OR REPRODUCTION IS PROHIBITED
 # WITHOUT THE PRIOR EXPRESS WRITTEN PERMISSION OF 方图数据（北京）软件股份有限公司.
 #
 
-"""
-打印出有颜色的输出
-python2/3兼容
-"""
 from __future__ import print_function  # 兼容print
 import logging
 import sys
 import datetime
 
 """
-打印出有颜色的输出
-python2/3兼容
+print output with color
 """
 
+
 class colour:
     """
-    打印颜色
+    color
     """
     BLUE = '\033[94m'
     GREEN = '\033[92m'
     DARK_GREEN = '\033[36m'
     RED = '\033[91m'
     YELLOW = '\033[93m'
     ENDC = '\033[0m'
```

### Comparing `gridgraph_importer-2.0/gridgraph_importer/data_importer.py` & `gridgraph_importer-3.0/gridgraph_importer/data_importer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,53 @@
-#!./python/bin/python3
+#!/bin/env python
 # -*- coding: UTF-8 -*-
+#
+# (c) 2018-2023 方图数据（北京）软件股份有限公司. All Rights Reserved.
+# Unpublished - rights reserved under the copyright laws of CHINA USE OF A
+# COPYRIGHT NOTICE IS PRECAUTIONARY ONLY AND DOES NOT IMPLY PUBLICATION OR
+# DISCLOSURE.
+#
+# THIS SOFTWARE CONTAINS CONFIDENTIAL INFORMATION AND TRADE SECRETS OF
+# 方图数据（北京）软件股份有限公司. USE, DISCLOSURE, OR REPRODUCTION IS PROHIBITED
+# WITHOUT THE PRIOR EXPRESS WRITTEN PERMISSION OF 方图数据（北京）软件股份有限公司.
+#
 
 from gremlin_python.driver import client
+from gremlin_python.driver.aiohttp.transport import AiohttpTransport
+from gremlin_python.driver.aiohttp import transport
+
+from gremlin_python import statics
+from gremlin_python.process.anonymous_traversal import traversal
+from gremlin_python.process.graph_traversal import __
+from gremlin_python.process.strategies import *
+from gremlin_python.driver.driver_remote_connection import DriverRemoteConnection
+from gremlin_python.process.traversal import T
+from gremlin_python.process.traversal import Order
+from gremlin_python.process.traversal import Cardinality
+from gremlin_python.process.traversal import Column
+from gremlin_python.process.traversal import Direction
+from gremlin_python.process.traversal import Operator
+from gremlin_python.process.traversal import P
+from gremlin_python.process.traversal import TextP
+from gremlin_python.process.traversal import Pop
+from gremlin_python.process.traversal import Scope
+from gremlin_python.process.traversal import Barrier
+from gremlin_python.process.traversal import Bindings
+from gremlin_python.process.traversal import WithOptions
+
 from gridgraph_importer import log_utils
 import sys
 import os
 import json
 import csv
-from os import listdir
-from os.path import isfile, join
+from os.path import join
+from concurrent.futures import ThreadPoolExecutor, wait, ALL_COMPLETED
+import threading
 
-log_file_name, log = log_utils.init_runtime_logger('bulk_load', 'gremlin_client')
+log_file_name, log = log_utils.init_runtime_logger('gridgraph', 'data-importer')
 print('log file: %s\n' % log_file_name, file=sys.stderr)
 
 graph_struct_file_name = 'graphStruct.json'
 bulk_load_csv_file_name = 'bulkloadCsv.json'
 graph_name_key = 'graphName'
 primary_key_key = 'primaryKey'
 default_schema_key = 'defaultSchema'
@@ -50,249 +83,326 @@
 VERTEX_SCHEMA_TO_CSV = {}
 EDGE_SCHEMA_TO_CSV = {}
 VERTEX_SCHEMA_FIELDS = {}
 EDGE_SCHEMA_FIELDS = {}
 EDGE_FROM_TO_VERTEX = {}
 
 
+def close_connect(session):
+    session.close()
+
+
+def send_gremlin_script(session, gremlin_script):
+    result_set = session.submit(gremlin_script)
+    results = result_set.all().result()
+    # thread_name = threading.current_thread().name
+    # log.info("[%s] results=%s", thread_name, results)
+
+
 class GremlinClient:
     def __init__(self, server_ip, port, username, password):
         self._server_ip = server_ip
         self._port = port
         self._username = username
         self._password = password
         self._address = "ws://{0}:{1}/gremlin".format(server_ip, port)
 
-    def send_gremlin_script(self, gremlin_script):
-        session = client.Client(self._address, None, username=self._username, password=self._password)
-        result_set = session.submit(gremlin_script)
-        results = result_set.all().result()
-        log.info("results=%s", results)
+    def connect(self):
+        transport_args = {'max_content_length': 10 * 1024 * 1024 * 1024}
+        return client.Client(self._address, None, username=self._username, password=self._password, **transport_args)
+
+
+def create_graph_and_import_csv_data(server_ip, port, data_dir, username='admin', password='admin'):
+    try:
+        check_csv_data_dir(data_dir)
+        gremlin_client = GremlinClient("127.0.0.1", 8381, "admin", "admin")
+        session = gremlin_client.connect()
+        graph_struct_scripts = parse_graph_struct_file(data_dir)
+        log.info("start to create graph...")
+        for gs in graph_struct_scripts:
+            # log.info("exec [%s]", gs)
+            send_gremlin_script(session, gs)
+        log.info("create graph successfully.")
+
+        parse_bulk_load_csv_mapping_file(data_dir)
+
+        core_num = os.cpu_count()
+        thread_pool = ThreadPoolExecutor(core_num)
+
+        v_data_scripts = parse_vertex_file(data_dir)
+        log.info('start to import vertex data...')
+        v_data_scripts_group = [v_data_scripts[i:i + core_num] for i in range(0, len(v_data_scripts), core_num)]
+        all_tasks = [thread_pool.submit(send_gremlin_scripts, session, dg) for dg in v_data_scripts_group]
+        wait(all_tasks, return_when=ALL_COMPLETED)
+        log.info("import vertex data successfully.")
+
+        e_data_scripts = parse_edge_file(data_dir)
+        log.info('start to import edge data...')
+        e_data_scripts_group = [e_data_scripts[i:i + core_num] for i in range(0, len(e_data_scripts), core_num)]
+        all_tasks = [thread_pool.submit(send_gremlin_scripts, session, dg) for dg in e_data_scripts_group]
+        wait(all_tasks, return_when=ALL_COMPLETED)
+        log.info("import edge data successfully.")
+
+        send_gremlin_script(session, "GridGraphFactory.listGraph()")
         session.close()
+    except RuntimeError as e:
+        raise
 
 
-def import_csv_data(server_ip, port, data_dir, username='admin', password='admin'):
-    check_csv_data_dir(data_dir)
-    gremlin_client = GremlinClient("127.0.0.1", 8381, "admin", "admin")
-    schema_script = parse_graph_struct_file(data_dir)
-    gremlin_client.send_gremlin_script(schema_script)
-
-    parse_bulk_load_csv_mapping_file(data_dir)
-
-    data_scripts = parse_data_file(data_dir)
-    log.info('start import data')
-    for ds in data_scripts:
-        log.info(ds)
-        gremlin_client.send_gremlin_script(ds)
+def import_csv_data_to_existing_graph(server_ip, port, data_dir, username='admin', password='admin'):
+    try:
+        check_csv_data_dir(data_dir)
+        gremlin_client = GremlinClient("127.0.0.1", 8381, "admin", "admin")
+        session = gremlin_client.connect()
+        parse_graph_struct_file(data_dir)
+
+        parse_bulk_load_csv_mapping_file(data_dir)
+
+        core_num = os.cpu_count()
+        thread_pool = ThreadPoolExecutor(core_num)
+
+        v_data_scripts = parse_vertex_file(data_dir)
+        log.info('start to import vertex data...')
+        v_data_scripts_group = [v_data_scripts[i:i + core_num] for i in range(0, len(v_data_scripts), core_num)]
+        all_tasks = [thread_pool.submit(send_gremlin_scripts, session, dg) for dg in v_data_scripts_group]
+        wait(all_tasks, return_when=ALL_COMPLETED)
+        log.info("import vertex data successfully.")
+
+        e_data_scripts = parse_edge_file(data_dir)
+        log.info('start to import edge data...')
+        e_data_scripts_group = [e_data_scripts[i:i + core_num] for i in range(0, len(e_data_scripts), core_num)]
+        all_tasks = [thread_pool.submit(send_gremlin_scripts, session, dg) for dg in e_data_scripts_group]
+        wait(all_tasks, return_when=ALL_COMPLETED)
+        log.info("import edge data successfully.")
 
-    gremlin_client.send_gremlin_script("GridGraphFactory.listGraph()")
+        send_gremlin_script(session, "GridGraphFactory.listGraph()")
+        session.close()
+    except RuntimeError as e:
+        raise
+
+
+def send_gremlin_scripts(session, scripts):
+    for s in scripts:
+        # thread_name = threading.current_thread().name
+        # log.info("this is thread : %s", thread_name)
+        # log.info(s)
+        send_gremlin_script(session, s)
 
 
 def check_csv_data_dir(data_dir):
-    log.info("check csv data dir.")
+    log.info("check csv data dir. [data_dir=%s]", data_dir)
     if not os.path.isdir(data_dir):
         log.error("data dir is not exist. [data_dir=%s]", data_dir)
-        return
-    graph_struct_file = os.path.join(data_dir, "graphStruct.json")
-    if not graph_struct_file:
-        log.error("graph struct json file is not exist. [graph_struct_file={}]", graph_struct_file)
-        return
+        raise RuntimeError
+    graph_struct_file = os.path.join(data_dir, graph_struct_file_name)
+    if not os.path.exists(os.path.join(data_dir, graph_struct_file)):
+        log.error("graph struct json file is not exist. [graph_struct_file_name=%s]", graph_struct_file_name)
+        raise RuntimeError
+    bulk_load_csv_file = os.path.join(data_dir, bulk_load_csv_file_name)
+    if not os.path.exists(os.path.join(data_dir, bulk_load_csv_file)):
+        log.error("bulk load csv file is not exist. [bulk_load_csv_file_name=%s]", bulk_load_csv_file_name)
+        raise RuntimeError
 
 
-def parse_graph_struct_file(data_dir) -> str:
-    log.info("parse graph struct file.")
+def parse_graph_struct_file(data_dir) -> list:
+    log.info("parse graph struct file...")
     graph_struct_file = os.path.join(data_dir, graph_struct_file_name)
     graph_struct_scripts = []
     with open(graph_struct_file, 'r') as f:
         graph_struct_json = json.load(f)
-        log.info(json.dumps(graph_struct_json, indent=4))
+        log.info("\n%s", json.dumps(graph_struct_json, indent=4))
+
+        create_graph_scripts = []
 
         graph_name = graph_struct_json[graph_name_key]
         create_graph_line = "graph = GridGraphFactory.createGraph('{}')".format(graph_name)
         log.info(create_graph_line)
-        graph_struct_scripts.append(create_graph_line)
+        create_graph_scripts.append(create_graph_line)
 
         primary_key = graph_struct_json[primary_key_key]
         create_primary_key_line = "graph.createPrimaryKey('{}')".format(primary_key)
         log.info(create_primary_key_line)
-        graph_struct_scripts.append(create_primary_key_line)
+        create_graph_scripts.append(create_primary_key_line)
 
-        schemas = graph_struct_json[schemas_key]
-        for schema in schemas:
-            create_schema_line = "{}Schema = graph.createSchema('{}', SchemaType.{})" \
-                .format(schema[name_key], schema[name_key], schema[type_key].upper())
-            log.info(create_schema_line)
-            graph_struct_scripts.append(create_schema_line)
-            if schema[type_key].upper() == VERTEX:
-                VERTEX_SCHEMA_PROPERTY_TYPE[schema[name_key]] = {}
-            elif schema[type_key].upper() == EDGE:
-                EDGE_SCHEMA_PROPERTY_TYPE[schema[name_key]] = {}
-            else:
-                log.error("schema type error. [type=%s]", schema[type_key].upper())
-                raise TypeError("schema type error.")
+        create_graph_scripts.append("graph.tx().commit()")
+
+        graph_struct_scripts.append(';'.join(create_graph_scripts))
 
-            properties = schema[properties_key]
-            for property in properties:
+        step = 10
+        schemas = graph_struct_json[schemas_key]
+        schemas_group = [schemas[i:i + step] for i in range(0, len(schemas), step)]
+        for schemas in schemas_group:
+            # log.info('schemas=%s', schemas)
+            create_schemas_scrips = ["graph = GridGraphFactory.openGraph('{}')".format(graph_name)]
+            for schema in schemas:
+                create_schema_line = "{}Schema = graph.createSchema('{}', SchemaType.{})" \
+                    .format(schema[name_key], schema[name_key], schema[type_key].upper())
+                log.info(create_schema_line)
+                create_schemas_scrips.append(create_schema_line)
                 if schema[type_key].upper() == VERTEX:
-                    VERTEX_SCHEMA_PROPERTY_TYPE[schema[name_key]][property[name_key]] = property[type_key]
+                    VERTEX_SCHEMA_PROPERTY_TYPE[schema[name_key]] = {}
+                elif schema[type_key].upper() == EDGE:
+                    EDGE_SCHEMA_PROPERTY_TYPE[schema[name_key]] = {}
                 else:
-                    EDGE_SCHEMA_PROPERTY_TYPE[schema[name_key]][property[name_key]] = property[type_key]
+                    log.error("schema type error. [type=%s]", schema[type_key].upper())
+                    raise TypeError("schema type error.")
 
-                if property[name_key] == primary_key:
-                    continue
-                create_property_line = "{}Schema.createProperty('{}', GridDataType.{}, {}, {}, null)" \
-                    .format(schema[name_key], property[name_key], property[type_key], str(property[unique_key]).lower(),
-                            str(property[nullable_key]).lower())
-                log.info(create_property_line)
-                graph_struct_scripts.append(create_property_line)
-
-        indexs = graph_struct_json[indexs_key]
-        for index in indexs:
-            index_name = index[index_name_key]
-            property_index = index[property_indexs_key][0]
-            create_index_line = 'graph.createIndex("{}", "{}", "{}", IndexSortDirection.{})'.format(
-                index_name, property_index[schema_name_key], property_index[property_name_key],
-                property_index[direction_key].upper())
-            graph_struct_scripts.append(create_index_line)
-            log.info(create_index_line)
-
-    graph_struct_scripts.append("graph.tx().commit()")
-    log.info(json.dumps(VERTEX_SCHEMA_PROPERTY_TYPE, indent=4))
-    log.info(json.dumps(EDGE_SCHEMA_PROPERTY_TYPE, indent=4))
-    ret = ';'.join(graph_struct_scripts)
-    log.info(ret)
-    return ret
+                properties = schema[properties_key]
+                for p in properties:
+                    if schema[type_key].upper() == VERTEX:
+                        VERTEX_SCHEMA_PROPERTY_TYPE[schema[name_key]][p[name_key]] = p[type_key]
+                    else:
+                        EDGE_SCHEMA_PROPERTY_TYPE[schema[name_key]][p[name_key]] = p[type_key]
+
+                    if p[name_key] == primary_key:
+                        continue
+                    create_property_line = "{}Schema.createProperty('{}', GridDataType.{}, {}, {}, null)" \
+                        .format(schema[name_key], p[name_key], p[type_key],
+                                str(p[unique_key]).lower(),
+                                str(p[nullable_key]).lower())
+                    log.info(create_property_line)
+                    create_schemas_scrips.append(create_property_line)
+            create_schemas_scrips.append("graph.tx().commit()")
+            graph_struct_scripts.append(';'.join(create_schemas_scrips))
+
+        if indexs_key in graph_struct_json:
+            indexs = graph_struct_json[indexs_key]
+            create_index_scripts = ["graph = GridGraphFactory.openGraph('{}')".format(graph_name)]
+            for index in indexs:
+                index_name = index[index_name_key]
+                property_index = index[property_indexs_key][0]
+                create_index_line = 'graph.createIndex("{}", "{}", "{}", IndexSortDirection.{})'.format(
+                    index_name, property_index[schema_name_key], property_index[property_name_key],
+                    property_index[direction_key].upper())
+                create_index_scripts.append(create_index_line)
+                log.info(create_index_line)
+            create_index_scripts.append("graph.tx().commit()")
+            graph_struct_scripts.append(';'.join(create_index_scripts))
+
+    # log.info(json.dumps(VERTEX_SCHEMA_PROPERTY_TYPE, indent=4))
+    # log.info(json.dumps(EDGE_SCHEMA_PROPERTY_TYPE, indent=4))
+    return graph_struct_scripts
 
 
 def parse_bulk_load_csv_mapping_file(data_dir):
-    log.info("parse bulk load csv mapping file")
+    log.info("parse bulk load csv mapping file...")
     bulk_load_csv_file = os.path.join(data_dir, bulk_load_csv_file_name)
     with open(bulk_load_csv_file, 'r') as f:
         bulk_load_csv_json = json.load(f)
-        log.info(json.dumps(bulk_load_csv_json, indent=4))
+        log.info("\n%s", json.dumps(bulk_load_csv_json, indent=4))
 
         GRAPH_INFO[graph_name_key] = bulk_load_csv_json[graph_name_key]
-        GRAPH_INFO[primary_key_key] = bulk_load_csv_json[primary_key_key]
+        GRAPH_INFO[primary_key_key] = bulk_load_csv_json[primary_key_key.lower()]
         GRAPH_INFO[csv_splitter_char_key] = bulk_load_csv_json[connection_key][csv_splitter_char_key]
         vertice = bulk_load_csv_json[vertexes_key]
         for v in vertice:
             VERTEX_SCHEMA_TO_CSV[v[schema_name_key]] = v[file_name_key]
             VERTEX_SCHEMA_FIELDS[v[schema_name_key]] = list(v[field_map_key].keys())
         edges = bulk_load_csv_json[edges_key]
         for e in edges:
             EDGE_SCHEMA_TO_CSV[e[schema_name_key]] = e[file_name_key]
             EDGE_SCHEMA_FIELDS[e[schema_name_key]] = list(e[field_map_key].keys())
             from_to_vertex = dict()
             from_to_vertex[from_vertex_key] = e[from_vertex_key]
             from_to_vertex[to_vertex_key] = e[to_vertex_key]
             EDGE_FROM_TO_VERTEX[e[schema_name_key]] = from_to_vertex
-    log.info(GRAPH_INFO)
-    log.info(VERTEX_SCHEMA_TO_CSV)
-    log.info(VERTEX_SCHEMA_FIELDS)
-    log.info(EDGE_SCHEMA_TO_CSV)
-    log.info(EDGE_SCHEMA_FIELDS)
-    log.info(EDGE_FROM_TO_VERTEX)
-
+    log.info("graph info\n%s", GRAPH_INFO)
+    log.info("vertex schema to csv mapping info\n%s", VERTEX_SCHEMA_TO_CSV)
+    log.info("vertex schema fields info\n%s", VERTEX_SCHEMA_FIELDS)
+    log.info("edge schema to csv mapping info\n%s", EDGE_SCHEMA_TO_CSV)
+    log.info("edge schema fields info\n%s", EDGE_SCHEMA_FIELDS)
+    log.info("edge from to vertex info\n%s", EDGE_FROM_TO_VERTEX)
 
-def parse_data_file(data_dir) -> list:
-    log.info("parse data file...")
-    log.info("parse vertex csv")
 
+def parse_vertex_file(data_dir) -> list:
     add_data_scripts = list()
-    step = 5
-
-
+    step = 500
+    log.info("parse vertex csv...")
     add_vertex_scripts = list()
     log.info(VERTEX_SCHEMA_TO_CSV)
     for k, v in VERTEX_SCHEMA_TO_CSV.items():
         fields = VERTEX_SCHEMA_FIELDS[k]
         file = join(data_dir, v)
+        if not os.path.exists(file):
+            log.warn("csv file is not exist. [file_name=%s]", file)
+            continue
         with open(file, "r", encoding="utf-8", newline='') as f:
             reader = csv.reader(f)
             for row in reader:
                 i = 0
                 add_vertex_line = 'graph.addVertex(T.label, "{}"'.format(k)
                 for e in row:
                     line_part = generate_add_data_line(VERTEX, k, fields[i], row[i])
                     add_vertex_line += ', "{}", {}'.format(fields[i], line_part)
                     i = i + 1
                 add_vertex_line += ')'
-                log.info(add_vertex_line)
+                # log.info(add_vertex_line)
                 add_vertex_scripts.append(add_vertex_line)
-                # add_data_scripts.append(add_vertex_line)
-
 
     add_v_scripts_group = [add_vertex_scripts[i:i + step] for i in range(0, len(add_vertex_scripts), step)]
-    log.info("V scripts group:\n %s", add_v_scripts_group)
+    # log.info("V scripts group:\n %s", add_v_scripts_group)
     for g in add_v_scripts_group:
         start = "graph = GridGraphFactory.openGraph('{}')".format(GRAPH_INFO[graph_name_key])
         add_data_scripts.append(start + ';' + ';'.join(g) + ';' + "graph.tx().commit()")
-
-    # traversal_line = "g=graph.traversal()"
-    # add_data_scripts.append(traversal_line)
-    # log.info(traversal_line)
+    return add_data_scripts
 
 
+def parse_edge_file(data_dir) -> list:
+    add_data_scripts = list()
+    step = 500
+    log.info("parse edge csv...")
     add_edge_scripts = list()
+    log.info(EDGE_SCHEMA_TO_CSV)
     for k, v in EDGE_SCHEMA_TO_CSV.items():
         fields = EDGE_SCHEMA_FIELDS[k]
         file = join(data_dir, v)
+        if not os.path.exists(file):
+            log.warn("csv file is not exist. [file_name=%s]", file)
+            continue
         with open(file, "r", encoding="utf-8", newline='') as f:
             reader = csv.reader(f)
             for row in reader:
-
                 add_edge_line = "g.V().has('{}','{}','{}').next().addEdge('{}', g.V().has('{}','{}','{}').next()".format(
                     EDGE_FROM_TO_VERTEX[k][from_vertex_key], GRAPH_INFO[primary_key_key], row[0], k,
                     EDGE_FROM_TO_VERTEX[k][to_vertex_key], GRAPH_INFO[primary_key_key], row[1])
-
-                # log.info(row)
                 if len(row) > 2:
                     i = 0
                     for e in row:
                         if i < 2:
                             i = i + 1
                             continue
-                        # log.info(row[i])
                         line_part = generate_add_data_line(EDGE, k, fields[i], row[i])
-                        # log.info(line_part)
                         add_edge_line += ", '{}', {}".format(fields[i], line_part)
-                        # log.info(add_edge_line)
                         i = i + 1
                 add_edge_line += ')'
-                # add_data_scripts.append(add_edge_line)
                 add_edge_scripts.append(add_edge_line)
-                log.info(add_edge_line)
+                # log.info(add_edge_line)
 
     add_e_scripts_group = [add_edge_scripts[i:i + step] for i in range(0, len(add_edge_scripts), step)]
-    log.info("E scripts group:\n %s", add_e_scripts_group)
+    # log.info("E scripts group:\n %s", add_e_scripts_group)
     for g in add_e_scripts_group:
         start = "graph = GridGraphFactory.openGraph('{}');g=graph.traversal()".format(GRAPH_INFO[graph_name_key])
         add_data_scripts.append(start + ';' + ';'.join(g) + ';' + "graph.tx().commit()")
-
-    # add_data_scripts.append("graph.tx().commit()")
-    # ret = ';'.join(add_data_scripts)
-    log.info(add_data_scripts)
     return add_data_scripts
 
 
 def generate_add_data_line(schema_type, schema_name, property_name, property_value) -> str:
     if schema_type == VERTEX:
         p_type_info = VERTEX_SCHEMA_PROPERTY_TYPE[schema_name]
     else:
         p_type_info = EDGE_SCHEMA_PROPERTY_TYPE[schema_name]
 
     if p_type_info[property_name] == 'STRING':
-        return "'{}'".format(property_value)
+        return "'{}'".format(property_value.replace('"', '\\"').replace("'", "\\'").replace("$", "\\$"))
     elif p_type_info[property_name] == 'DOUBLE':
         return '{}d'.format(property_value)
     elif p_type_info[property_name] == 'FLOAT':
         return '{}f'.format(property_value)
     else:
         return '{}'.format(property_value)
 
 
 if __name__ == '__main__':
-    # cl = GremlinClient("127.0.0.1", 8381, "admin", "admin")
-    # script = "graph = GridGraphFactory.listGraph();"
-    # cl.send_gremlin_script(script)
-
-    import_csv_data("127.0.0.1", 8381, '/Users/hetao/work/gridgraph/bulkload/bulkload/standalone/strong-schema')
+    # import_csv_data("127.0.0.1", 8381, '/home/taohe/work/gridgraph/debug/data100M')
+    # /home/taohe/work/gridgraph/bulkload/bulkload/standalone/strong-schema
+    create_graph_and_import_csv_data(
+        "127.0.0.1", 8381, '/home/taohe/work/gridgraph/bulkload/bulkload/standalone/strong-schema')
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gridgraph_importer-2.0/setup.py` & `gridgraph_importer-3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setuptools.setup(
     name="gridgraph_importer",
-    version="2.0",
+    version="3.0",
     author="TaoHe",
     author_email="super_super_tao@163.com",
     description="gridgraph importer library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com",
     packages=setuptools.find_packages(),
```

