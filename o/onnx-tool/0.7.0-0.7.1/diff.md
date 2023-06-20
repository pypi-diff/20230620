# Comparing `tmp/onnx-tool-0.7.0.tar.gz` & `tmp/onnx-tool-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnx-tool-0.7.0.tar", last modified: Sun May 28 06:38:14 2023, max compression
+gzip compressed data, was "onnx-tool-0.7.1.tar", last modified: Tue Jun 20 15:43:34 2023, max compression
```

## Comparing `onnx-tool-0.7.0.tar` & `onnx-tool-0.7.1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 06:38:14.404531 onnx-tool-0.7.0/
--rw-rw-rw-   0        0        0     1092 2022-06-28 15:38:19.000000 onnx-tool-0.7.0/LICENSE
--rw-rw-rw-   0        0        0    10735 2023-05-28 06:38:14.404531 onnx-tool-0.7.0/PKG-INFO
--rw-rw-rw-   0        0        0    10276 2023-05-28 05:20:29.000000 onnx-tool-0.7.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 06:38:14.398530 onnx-tool-0.7.0/onnx_tool/
--rw-rw-rw-   0        0        0    14841 2023-05-28 05:20:29.000000 onnx-tool-0.7.0/onnx_tool/__init__.py
--rw-rw-rw-   0        0        0     3051 2023-05-28 05:20:29.000000 onnx-tool-0.7.0/onnx_tool/__main__.py
--rw-rw-rw-   0        0        0    11847 2023-04-10 11:33:26.000000 onnx-tool-0.7.0/onnx_tool/fusion.py
--rw-rw-rw-   0        0        0    57383 2023-05-28 05:20:29.000000 onnx-tool-0.7.0/onnx_tool/graph.py
--rw-rw-rw-   0        0        0    73170 2023-05-28 05:20:29.000000 onnx-tool-0.7.0/onnx_tool/node.py
--rw-rw-rw-   0        0        0     6433 2023-05-11 15:44:28.000000 onnx-tool-0.7.0/onnx_tool/serialization.py
--rw-rw-rw-   0        0        0    15758 2023-05-28 05:20:29.000000 onnx-tool-0.7.0/onnx_tool/tensor.py
--rw-rw-rw-   0        0        0     3685 2023-05-28 05:20:29.000000 onnx-tool-0.7.0/onnx_tool/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-28 06:38:14.403530 onnx-tool-0.7.0/onnx_tool.egg-info/
--rw-rw-rw-   0        0        0    10735 2023-05-28 06:38:14.000000 onnx-tool-0.7.0/onnx_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      385 2023-05-28 06:38:14.000000 onnx-tool-0.7.0/onnx_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 06:38:14.000000 onnx-tool-0.7.0/onnx_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-28 06:38:14.000000 onnx-tool-0.7.0/onnx_tool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-28 06:38:14.000000 onnx-tool-0.7.0/onnx_tool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2022-06-28 15:40:35.000000 onnx-tool-0.7.0/onnx_tool.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-05-28 06:38:14.404531 onnx-tool-0.7.0/setup.cfg
--rw-rw-rw-   0        0        0      988 2023-05-28 05:20:29.000000 onnx-tool-0.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:43:34.380592 onnx-tool-0.7.1/
+-rw-rw-rw-   0        0        0     1092 2022-12-15 10:33:04.000000 onnx-tool-0.7.1/LICENSE
+-rw-rw-rw-   0        0        0    10735 2023-06-20 15:43:34.380592 onnx-tool-0.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0    10276 2023-06-18 06:46:34.000000 onnx-tool-0.7.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 15:43:34.367696 onnx-tool-0.7.1/onnx_tool/
+-rw-rw-rw-   0        0        0     7846 2023-06-19 15:21:47.000000 onnx-tool-0.7.1/onnx_tool/__init__.py
+-rw-rw-rw-   0        0        0     3051 2023-06-18 06:46:34.000000 onnx-tool-0.7.1/onnx_tool/__main__.py
+-rw-rw-rw-   0        0        0    16079 2023-06-19 15:20:56.000000 onnx-tool-0.7.1/onnx_tool/fusion.py
+-rw-rw-rw-   0        0        0    56902 2023-06-20 15:34:51.000000 onnx-tool-0.7.1/onnx_tool/graph.py
+-rw-rw-rw-   0        0        0      876 2023-06-19 15:20:56.000000 onnx-tool-0.7.1/onnx_tool/model.py
+-rw-rw-rw-   0        0        0    73508 2023-06-18 06:46:34.000000 onnx-tool-0.7.1/onnx_tool/node.py
+-rw-rw-rw-   0        0        0     6433 2023-06-18 06:46:34.000000 onnx-tool-0.7.1/onnx_tool/serialization.py
+-rw-rw-rw-   0        0        0    15758 2023-06-18 06:46:34.000000 onnx-tool-0.7.1/onnx_tool/tensor.py
+-rw-rw-rw-   0        0        0     3685 2023-06-20 15:38:47.000000 onnx-tool-0.7.1/onnx_tool/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:43:34.377186 onnx-tool-0.7.1/onnx_tool.egg-info/
+-rw-rw-rw-   0        0        0    10735 2023-06-20 15:43:34.000000 onnx-tool-0.7.1/onnx_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      404 2023-06-20 15:43:34.000000 onnx-tool-0.7.1/onnx_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 15:43:34.000000 onnx-tool-0.7.1/onnx_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-06-20 15:43:34.000000 onnx-tool-0.7.1/onnx_tool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-20 15:43:34.000000 onnx-tool-0.7.1/onnx_tool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-06-20 15:43:33.000000 onnx-tool-0.7.1/onnx_tool.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-06-20 15:43:34.380592 onnx-tool-0.7.1/setup.cfg
+-rw-rw-rw-   0        0        0      988 2023-06-20 15:38:55.000000 onnx-tool-0.7.1/setup.py
```

### Comparing `onnx-tool-0.7.0/LICENSE` & `onnx-tool-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `onnx-tool-0.7.0/PKG-INFO` & `onnx-tool-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnx-tool
-Version: 0.7.0
+Version: 0.7.1
 Summary: A tool for ONNX model:Rapid shape inference; Profile model; Compute Graph and Shape Engine; OPs fusion;Quantized models and sparse models are supported.
 Home-page: https://github.com/ThanatosShinji/onnx-tool
 Author: Luo Yu
 Author-email: luoyu888888@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: onnx-tool Version: 0.7.0 Summary: A tool for ONNX
+Metadata-Version: 2.1 Name: onnx-tool Version: 0.7.1 Summary: A tool for ONNX
 model:Rapid shape inference; Profile model; Compute Graph and Shape Engine; OPs
 fusion;Quantized models and sparse models are supported. Home-page: https://
 github.com/ThanatosShinji/onnx-tool Author: Luo Yu Author-email:
 luoyu888888@gmail.com License: MIT Classifier: Programming Language :: Python
 :: 3 Description-Content-Type: text/markdown License-File: LICENSE ç®ä½ä¸­æ
 # onnx-tool **A tool for ONNX model:** * *Rapid shape inference.* * *Profile
 model.* * *Constant_Folding.* * *Compute Graph and Shape Engine.* * *OPs
```

### Comparing `onnx-tool-0.7.0/README.md` & `onnx-tool-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `onnx-tool-0.7.0/onnx_tool/__main__.py` & `onnx-tool-0.7.1/onnx_tool/__main__.py`

 * *Files identical despite different names*

### Comparing `onnx-tool-0.7.0/onnx_tool/graph.py` & `onnx-tool-0.7.1/onnx_tool/graph.py`

 * *Files 5% similar despite different names*

```diff
@@ -167,21 +167,23 @@
         self.producedby = {}
         self.consumedby = {}
         self.rawgraph = g
         self.initials = []
         self.dynamics = []
         self.input = []
         self.output = []
-        self.__init_graph_from_onnxproto__(g, noderename)
-        self.__constant_search__(constant_folding)
-        self.__update_nodes_tensors__(constant_folding)
-        self.__find_shape_tensors__()
         self.valid_shape = False
         self.valid_profile = False
 
+        if g is not None:
+            self.__init_graph_from_onnxproto__(g, noderename)
+            self.__constant_search__(constant_folding)
+            self.__update_nodes_tensors__(constant_folding)
+            self.__find_shape_tensors__()
+
     def log(self, str):
         if self.verbose:
             print(str)
 
     def __update_nodes_tensors__(self, constant_folding):
         from .utils import timer
         tm = timer()
@@ -303,14 +305,19 @@
                     self.consumedby[tensor] = []
                 self.consumedby[tensor].append(node.name)
             for tensor in node.output:
                 if tensor not in self.producedby:
                     self.producedby[tensor] = []
                 self.producedby[tensor].append(node.name)
 
+    def update_tensor_relations(self):
+        self.__update_consumer_producer__()
+        self.dynamics=list(self.producedby.keys())
+
+
     def __init_graph_from_onnxproto__(self, g, noderename):
         if g is None:
             return
         ncount = 0
         from .utils import timer
 
         tm = timer()
@@ -493,17 +500,18 @@
                     enqueued.append(input)
         return initializer
 
     def remove_node(self, nodename):
         node = self.nodemap[nodename]
         # update producer
         for o in node.output:
-            self.producedby[o].remove(nodename)
-            if len(self.producedby[o]) == 0:
-                self.producedby.pop(o)
+            if o in self.producedby.keys():
+                self.producedby[o].remove(nodename)
+                if len(self.producedby[o]) == 0:
+                    self.producedby.pop(o)
         # update consumer
         for i in node.input:
             if i in self.consumedby.keys():
                 self.consumedby[i].remove(nodename)
         self.nodemap.pop(nodename)
 
     def skip_node(self, nodename):
@@ -511,21 +519,27 @@
         count = 0
         for input in node.input:
             if input in self.dynamics:
                 count += 1
                 indtensor = input
         if count == 1 and len(node.output) == 1:
             self.consumedby[indtensor].remove(nodename)
-            for con in self.consumedby[node.output[0]]:
-                con_node = self.nodemap[con]
-                for i in range(len(con_node.input)):
-                    if con_node.input[i] == node.output[0]:
-                        con_node.input[i] = indtensor
-                        self.consumedby[indtensor].append(con)
-                        break
+            if node.output[0] in self.consumedby:
+                for con in self.consumedby[node.output[0]]:
+                    con_node = self.nodemap[con]
+                    for i in range(len(con_node.input)):
+                        if con_node.input[i] == node.output[0]:
+                            con_node.input[i] = indtensor
+                            self.consumedby[indtensor].append(con)
+                            break
+            else:
+                for pro in self.producedby[indtensor]:
+                    pro_node = self.nodemap[pro]
+                    assert(len(pro_node.output)==1)
+                    pro_node.output[0]=node.output[0]
 
     def fuse_subgraph_node_names(self, nodes: [str], nodeop: str, nodename: str, keep_attr=True):
         _inputs, _outputs = self.get_iotensors(nodes, remove_initials=False)
         newnode = onnx.helper.make_node(nodeop, _inputs, _outputs, name=nodename)
         count = 0
         if keep_attr:
             for node in nodes:
@@ -596,29 +610,36 @@
                 newnode.prevnodes.append(self.producedby[i])
         for o in _outputs:
             self.producedby[o] = [mainnode.name]
             if o in self.consumedby.keys():
                 newnode.nextnodes.append(self.consumedby[o])
         self.nodemap[mainnode.name] = newnode
 
-    def fuse_subgraph_iotensors(self, inputs: [], outputs: [], nodeop: str, name: str, keep_attr=True):
+    def fuse_subgraph_iotensors(self, inputs: [], outputs: [], nodeop: str, name_prefix:str=None, keep_attr=True):
         _, nodes, _ = self.__get_subnodes_byio__(inputs, outputs)
-        _inputs, _outputs = self.get_iotensors(nodes, remove_initials=True)
-        nodes = self.reorder_nodes(nodes, _inputs)
-        return self.fuse_subgraph_node_names(nodes, nodeop, name, keep_attr)
+        from .fusion import create_descs_from_nodenames,FusionPattern
+        descs=create_descs_from_nodenames(self,nodes)
+        pattern = FusionPattern(descs)
+        nodesls = pattern.search_pattern(self)
+        for i,nodes in enumerate(nodesls):
+            name = name_prefix+'_'+str(i) if name_prefix is not None else nodes[0]
+            self.fuse_subgraph_node_names(nodes,nodeop,name,keep_attr)
 
     def get_onnxgraph_by_nodenames(self, nodenames):
         if len(nodenames):
             _inputs0, _outputs0 = self.get_iotensors(nodenames)
             graph_level0 = self.reorder_nodes(nodenames, _inputs0)
             subgraph = self.make_graph_onnx(graph_level0, 'subgraph', _inputs0, _outputs0)
             return subgraph
         return None
 
     def save_model(self, f: str, shape_only: bool = False, no_shape: bool = False, rawmodel: onnx.ModelProto = None):
+        if len(self.nodemap.keys())==0:
+            warnings.warn(f'Empty graph {f} to save')
+            return
         graph = self.make_graph_onnx(self.nodemap.keys(), 'graph', self.input, self.output,
                                      with_initializer=not shape_only, with_shape_info=not no_shape)
         if graph is not None and f is not None:
             attr = {}
             attr['producer_name'] = 'onnx_tool'
             attr['producer_version'] = 'v' + VERSION
             model = onnx.helper.make_model(graph, **attr)
@@ -636,15 +657,15 @@
         if with_initializer:
             initializer = self.get_initials_from_nodenames(nodenames)
 
         inputs = []
         outputs = []
         for name in inputnames:
             if name in self.tensormap:
-                proto = self.tensormap[name].make_value_proto()
+                proto = self.tensormap[name].make_value_proto(make_dummy=True)
                 if proto is not None:
                     inputs.append(proto)
             else:
                 inputs.append(onnx.helper.make_tensor_value_info(name, 1, None))
         for name in outputnames:
             if name in self.tensormap:
                 proto = self.tensormap[name].make_value_proto(make_dummy=True)
@@ -660,96 +681,90 @@
                 if vinfo is None:
                     continue
                 value_infos.append(vinfo)
         graph = onnx.helper.make_graph(nodes=nodes, name=gname, inputs=inputs, outputs=outputs, initializer=initializer,
                                        value_info=value_infos)
         return graph
 
-    def graph_reorder(self):
-        old_order = self.nodemap.keys()
-        ordered_nodes = self.reorder_nodes(old_order, self.input)
-        new_map = {}
-        for nname in ordered_nodes:
-            new_map[nname] = self.nodemap[nname]
-        self.nodemap = new_map
-        self.rawgraph = self.make_graph_onnx(self.nodemap.keys(), 'reordered', self.input, self.output)
+    def __backwardsearch_node__(self,curnode,produced_by,consumed_by,produced,searched):
+        nodelist = []
+        node = self.nodemap[curnode]
+        searched.append(curnode)
+        for tname in node.input:
+            if tname in produced_by.keys() and tname not in produced:
+                nodelist.extend(self.__backwardsearch_node__(produced_by[tname], produced_by, consumed_by, produced, searched))
 
-    def reorder_nodes(self, nodenames, itnames):
-        tensor_consumed = []
-        tensor_produced = []
-        nextnodes = []
-        reorderednode = []
-        search_flag = {}
-        for name in itnames:
-            for consumer in self.consumedby[name]:
-                if consumer in nodenames:
-                    if consumer not in nextnodes:
-                        search_flag[consumer] = True
-                        nextnodes.append(consumer)
-            tensor_produced.append(name)
-
-        for node in nodenames:
-            if self.__is_node_constant__(self.nodemap[node]):
-                dummy_node = True
-                for output in self.nodemap[node].output:
-                    if output in self.consumedby.keys():
-                        for consumer in self.consumedby[output]:
-                            if consumer in nodenames:
-                                if consumer not in nextnodes:
-                                    search_flag[consumer] = True
-                                    nextnodes.append(consumer)
-                        dummy_node = False
+
+        produced.extend(node.output)
+        nodelist +=[curnode]
+        return nodelist
+
+    def __forwardsearch_node__(self,curnode,produced_by,consumed_by,produced,searched):
+        nodelist=[]
+        backlist=[]
+        searched.append(curnode)
+        node = self.nodemap[curnode]
+        for tname in node.input:
+            if tname in produced_by.keys() and tname not in produced:
+                backlist.append(tname)
+        if len(backlist):
+            for tname in backlist:
+                nodelist.extend(self.__backwardsearch_node__(produced_by[tname], produced_by, consumed_by, produced,searched))
+
+        nodelist+=[curnode]
+
+        for tname in node.output:
+            produced.append(tname)
+        for tname in node.output:
+            if tname in consumed_by.keys():
+                for nextn in consumed_by[tname]:
+                    if nextn not in searched:
+                        nodelist.extend(self.__forwardsearch_node__(nextn,produced_by,consumed_by,produced,searched))
+        return nodelist
+
+    def reorder_nodes(self, node_names,input_names):
+        # update
+        import sys
+        curlimit=sys.getrecursionlimit()
+        newlimit=len(node_names)*1 if len(node_names)*1 > curlimit else curlimit
+        sys.setrecursionlimit(newlimit+100) #TODO while version instead of recursion version
+        produced_by = {}
+        for name in node_names:
+            node = self.nodemap[name]
+            for tname in node.output:
+                produced_by[tname] = name
+
+        consumed_by = {}
+        for name in node_names:
+            node = self.nodemap[name]
+            for tname in node.input:
+                if tname in produced_by.keys():
+                    if tname in consumed_by.keys():
+                        consumed_by[tname].append(name)
                     else:
-                        if dummy_node:
-                            if output in self.output:
-                                dummy_node = False
-                    tensor_produced.append(output)
-                if not dummy_node:
-                    reorderednode.append(node)
-
-        while len(nextnodes):
-            execnodes = []
-            for node in nextnodes:
-                produced = True
-                for input in self.nodemap[node].input:
-                    if len(input) == 0:
-                        continue
-                    if input in self.initials:
-                        continue
-                    if input not in self.producedby:
-                        continue
-                    if input not in tensor_produced:
-                        produced = False
-                        break
-                if produced:
-                    execnodes.append(node)
+                        consumed_by[tname] = [name]
 
-            newnodes = []
-            for node in nextnodes:
-                if node not in execnodes:
-                    newnodes.append(node)
-
-            reorderednode.extend(execnodes)
-            for node in execnodes:
-                for input in self.nodemap[node].input:
-                    if input in self.initials:
-                        continue
-                    tensor_consumed.append(input)
-                for output in self.nodemap[node].output:
-                    tensor_produced.append(output)
-                    if output in self.consumedby:
-                        for consumer in self.consumedby[output]:
-                            if consumer in nodenames:
-                                if consumer in search_flag:
-                                    continue
-                                newnodes.append(consumer)
-                                search_flag[consumer] = True
-            nextnodes = set(newnodes)
+        produced = []
+        searched = []
+        ordered_nodes = []
+        for input in input_names:
+            for cnode in self.consumedby[input]:
+                if cnode in searched:
+                    continue
+                ordered_nodes.extend(self.__forwardsearch_node__(cnode, produced_by, consumed_by, produced, searched))
+        sys.setrecursionlimit(curlimit)
+        return ordered_nodes
 
-        return reorderednode
+    def graph_reorder_nodes(self):
+        ordered_nodes=self.reorder_nodes(self.nodemap.keys(),self.input)
+        new_map = {}
+        for nname in ordered_nodes:
+            new_map[nname] = self.nodemap[nname]
+        self.nodemap = new_map
+        self.update_tensor_relations()
 
     def get_iotensors(self, nodenames, remove_initials=True):
         intensors = []
         outtensors = []
         for name in nodenames:
             for input in self.nodemap[name].input:
                 if len(input) == 0:
@@ -1119,39 +1134,14 @@
             raw_memsize += self.tensormap[tname].get_memsize()
 
         self.log(f"Raw memory size (without parameter memory): {raw_memsize:,} bytes")
         self.log(f"Compressed memory size: {compress_size:,} bytes")
         self.log(f'Comression ratio: {compress_size / raw_memsize * 100:.3f}%')
         return compress_mem, compress_size
 
-    def get_compute_graph_onnx(self):
-        nodes = []
-        for key in self.nodemap.keys():
-            node = self.nodemap[key]
-            if node.shape_calc:
-                continue
-            dummy_node = True
-            for output in node.output:
-                dummy = True
-                if output in self.consumedby.keys():
-                    for consumer in self.consumedby[output]:
-                        if not self.nodemap[consumer].shape_calc:
-                            dummy = False
-                            break
-                else:
-                    dummy = False
-                dummy_node = dummy_node and dummy
-            if dummy_node:
-                continue
-            nodes.append(node.name)
-        _inputs0, _outputs0 = self.get_iotensors(nodes)
-        graph_level0 = self.reorder_nodes(nodes, _inputs0)
-        subgraph = self.make_graph_onnx(graph_level0, 'compute_graph', self.input, self.output)
-        return subgraph
-
     def get_compute_graph(self):
         cg = copy.copy(self)
         nodes = []
         rmnodes = []
         for key in cg.nodemap.keys():
             node = cg.nodemap[key]
             if node.shape_calc:
```

### Comparing `onnx-tool-0.7.0/onnx_tool/node.py` & `onnx-tool-0.7.1/onnx_tool/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -324,15 +324,15 @@
     def __init__(self, node_proto):
         super().__init__(node_proto)
         self.op_mac = EXP_MACS + DIV_MACS
         self.ratio = 1
 
     def value_infer(self, intensors: []):
         xexp = numpy.exp(intensors[0])
-        return [xexp / numpy.sum(xexp)]
+        return [xexp / numpy.sum(xexp,axis=self.axis,keepdims=True)]
 
 
 @NODE_REGISTRY.register()
 class LogNode(PWNode):
     def __init__(self, node_proto):
         super().__init__(node_proto)
         self.op_mac = LOG_MACS
@@ -596,65 +596,69 @@
         return [numpy.transpose(intensors[0], self.perm)]
 
 
 @NODE_REGISTRY.register()
 class GemmNode(Node):
     def __init__(self, nodeproto):
         super().__init__(nodeproto)
-        self.add_default_value('transA', None)
-        self.add_default_value('transB', None)
+        self.add_default_value('transA', 0)
+        self.add_default_value('transB', 0)
 
     def shape_infer(self, intensors: []):
         xshape = _get_shape(intensors[0])
         wshape = _get_shape(intensors[1])
         if self.__class__ == GemmNode:
-            if self.transA is not None and self.transA > 0:
+            if self.transA > 0:
                 xshape = xshape[::-1]
             else:
                 xshape = xshape
-            if self.transB is not None and self.transB > 0:
+            if self.transB > 0:
                 yshape = xshape[:-1] + [wshape[-2], ]
             else:
                 yshape = xshape[:-1] + [wshape[-1], ]
         else:
-            yshape = xshape[:-1] + [wshape[-1], ]
+            # broadcast support
+            batchshape=xshape[:-2] if len(xshape)> len(wshape) else wshape[:-2]
+            yshape = batchshape+[xshape[-2],wshape[-1]]
 
         return [yshape]
 
     def value_infer(self, intensors: []):
         if self.__class__ == MatMulNode:
             ashape = _get_shape(intensors[0])
             bshape = _get_shape(intensors[1])
             assert (ashape[-1] == bshape[-2])
             return [numpy.matmul(intensors[0], intensors[1])]
-        if self.transA is not None and self.transA > 0:
+        if self.transA > 0:
             A = numpy.transpose(intensors[0])
         else:
             A = intensors[0]
-        if self.transB is not None and self.transB > 0:
+        if self.transB > 0:
             B = numpy.transpose(intensors[1])
         else:
             B = intensors[1]
         C = numpy.matmul(A, B)
         if len(intensors) > 2:
             C = numpy.add(C, intensors[2])
         return [C]
 
     def profile(self, intensors: [numpy.ndarray], outtensors: [numpy.ndarray]):
-        xshape = _get_shape(intensors[0])
+        yshape = _get_shape(outtensors[0])
         if len(intensors) >= 2:
             weight_shape = _get_shape(intensors[1])
-            macs = volume(xshape)
+            macs = volume(yshape)
             if self.__class__ == GemmNode:
-                macs *= weight_shape[0]
+                if self.transB > 0:
+                    macs *= weight_shape[-1]
+                else:
+                    macs *= weight_shape[-2]
             else:
-                macs *= weight_shape[-1]
-
+                macs *= weight_shape[-2]
             if len(intensors) == 3:
-                macs += volume(_get_shape(outtensors[0])) * ADD_MACS
+                macs += volume(yshape) * ADD_MACS
         else:
             raise NotImplementedError()
         return macs
 
 
 @NODE_REGISTRY.register()
 class MatMulNode(GemmNode):
@@ -1148,15 +1152,19 @@
 @NODE_REGISTRY.register()
 class IdentityNode(FusedBase):
     pass
 
 
 @NODE_REGISTRY.register()
 class ErfNode(FusedBase):
-    pass
+    def value_infer(self, intensors: []):
+        outtensor=numpy.zeros_like(intensors[0])
+        for i in numpy.ndindex(intensors[0].shape):
+            outtensor[i]=math.erf(intensors[0][i])
+        return [outtensor]
 
 
 @NODE_REGISTRY.register()
 class BatchNormalizationNode(FusedBase):
     def __init__(self,n):
         super().__init__(n)
         self.add_default_value('epsilon',1e-05)
```

### Comparing `onnx-tool-0.7.0/onnx_tool/serialization.py` & `onnx-tool-0.7.1/onnx_tool/serialization.py`

 * *Files identical despite different names*

### Comparing `onnx-tool-0.7.0/onnx_tool/tensor.py` & `onnx-tool-0.7.1/onnx_tool/tensor.py`

 * *Files identical despite different names*

### Comparing `onnx-tool-0.7.0/onnx_tool/utils.py` & `onnx-tool-0.7.1/onnx_tool/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import time
 import warnings
 
-VERSION = "0.7.0"
+VERSION = "0.7.1"
 
 
 class timer():
     def __init__(self):
         self._startt = time.time()
 
     def start(self):
```

### Comparing `onnx-tool-0.7.0/onnx_tool.egg-info/PKG-INFO` & `onnx-tool-0.7.1/onnx_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnx-tool
-Version: 0.7.0
+Version: 0.7.1
 Summary: A tool for ONNX model:Rapid shape inference; Profile model; Compute Graph and Shape Engine; OPs fusion;Quantized models and sparse models are supported.
 Home-page: https://github.com/ThanatosShinji/onnx-tool
 Author: Luo Yu
 Author-email: luoyu888888@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: onnx-tool Version: 0.7.0 Summary: A tool for ONNX
+Metadata-Version: 2.1 Name: onnx-tool Version: 0.7.1 Summary: A tool for ONNX
 model:Rapid shape inference; Profile model; Compute Graph and Shape Engine; OPs
 fusion;Quantized models and sparse models are supported. Home-page: https://
 github.com/ThanatosShinji/onnx-tool Author: Luo Yu Author-email:
 luoyu888888@gmail.com License: MIT Classifier: Programming Language :: Python
 :: 3 Description-Content-Type: text/markdown License-File: LICENSE ç®ä½ä¸­æ
 # onnx-tool **A tool for ONNX model:** * *Rapid shape inference.* * *Profile
 model.* * *Constant_Folding.* * *Compute Graph and Shape Engine.* * *OPs
```

### Comparing `onnx-tool-0.7.0/setup.py` & `onnx-tool-0.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 readme = open("README.md", encoding="utf-8").read()
-VERSION = "0.7.0"
+VERSION = "0.7.1"
 
 requirements = [
     "onnx",
     "numpy",
     'tabulate'
 ]
```

