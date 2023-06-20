# Comparing `tmp/reasoner-transpiler-2.0.1.tar.gz` & `tmp/reasoner-transpiler-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner-transpiler-2.0.1.tar", last modified: Wed May  3 15:00:18 2023, max compression
+gzip compressed data, was "reasoner-transpiler-2.0.2.tar", last modified: Tue Jun 20 15:55:58 2023, max compression
```

## Comparing `reasoner-transpiler-2.0.1.tar` & `reasoner-transpiler-2.0.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:00:18.667065 reasoner-transpiler-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-03 15:00:18.667065 reasoner-transpiler-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-03 15:00:15.000000 reasoner-transpiler-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:00:18.667065 reasoner-transpiler-2.0.1/reasoner_transpiler/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-03 15:00:15.000000 reasoner-transpiler-2.0.1/reasoner_transpiler/attribute_types.json
--rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-05-03 15:00:15.000000 reasoner-transpiler-2.0.1/reasoner_transpiler/cypher.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-03 15:00:15.000000 reasoner-transpiler-2.0.1/reasoner_transpiler/cypher_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)    16298 2023-05-03 15:00:15.000000 reasoner-transpiler-2.0.1/reasoner_transpiler/matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-05-03 15:00:15.000000 reasoner-transpiler-2.0.1/reasoner_transpiler/nesting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-05-03 15:00:15.000000 reasoner-transpiler-2.0.1/reasoner_transpiler/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:00:18.667065 reasoner-transpiler-2.0.1/reasoner_transpiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-03 15:00:18.000000 reasoner-transpiler-2.0.1/reasoner_transpiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-03 15:00:18.000000 reasoner-transpiler-2.0.1/reasoner_transpiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 15:00:18.000000 reasoner-transpiler-2.0.1/reasoner_transpiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 15:00:18.000000 reasoner-transpiler-2.0.1/reasoner_transpiler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-03 15:00:18.000000 reasoner-transpiler-2.0.1/reasoner_transpiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-03 15:00:18.000000 reasoner-transpiler-2.0.1/reasoner_transpiler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 15:00:18.667065 reasoner-transpiler-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-03 15:00:15.000000 reasoner-transpiler-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:55:58.118926 reasoner-transpiler-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-20 15:55:58.118926 reasoner-transpiler-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-20 15:55:55.000000 reasoner-transpiler-2.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:55:58.118926 reasoner-transpiler-2.0.2/reasoner_transpiler/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-20 15:55:55.000000 reasoner-transpiler-2.0.2/reasoner_transpiler/attribute_types.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-06-20 15:55:55.000000 reasoner-transpiler-2.0.2/reasoner_transpiler/cypher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-20 15:55:55.000000 reasoner-transpiler-2.0.2/reasoner_transpiler/cypher_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-20 15:55:55.000000 reasoner-transpiler-2.0.2/reasoner_transpiler/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16889 2023-06-20 15:55:55.000000 reasoner-transpiler-2.0.2/reasoner_transpiler/matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-06-20 15:55:55.000000 reasoner-transpiler-2.0.2/reasoner_transpiler/nesting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-06-20 15:55:55.000000 reasoner-transpiler-2.0.2/reasoner_transpiler/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:55:58.118926 reasoner-transpiler-2.0.2/reasoner_transpiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-20 15:55:58.000000 reasoner-transpiler-2.0.2/reasoner_transpiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-20 15:55:58.000000 reasoner-transpiler-2.0.2/reasoner_transpiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:55:58.000000 reasoner-transpiler-2.0.2/reasoner_transpiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:55:58.000000 reasoner-transpiler-2.0.2/reasoner_transpiler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-20 15:55:58.000000 reasoner-transpiler-2.0.2/reasoner_transpiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-20 15:55:58.000000 reasoner-transpiler-2.0.2/reasoner_transpiler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 15:55:58.118926 reasoner-transpiler-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-20 15:55:55.000000 reasoner-transpiler-2.0.2/setup.py
```

### Comparing `reasoner-transpiler-2.0.1/README.md` & `reasoner-transpiler-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `reasoner-transpiler-2.0.1/reasoner_transpiler/cypher.py` & `reasoner-transpiler-2.0.2/reasoner_transpiler/cypher.py`

 * *Files identical despite different names*

### Comparing `reasoner-transpiler-2.0.1/reasoner_transpiler/cypher_expression.py` & `reasoner-transpiler-2.0.2/reasoner_transpiler/cypher_expression.py`

 * *Files identical despite different names*

### Comparing `reasoner-transpiler-2.0.1/reasoner_transpiler/matching.py` & `reasoner-transpiler-2.0.2/reasoner_transpiler/matching.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """MATCHing tools."""
 from typing import Dict, List
 
 from bmt import Toolkit
 
+from .exceptions import InvalidPredicateError
 from .nesting import Query
 from .util import ensure_list, snake_case, space_case, pascal_case
 
 bmt = Toolkit()
 
 
 def cypher_prop_string(value):
@@ -151,58 +152,59 @@
 
     def __init__(
         self,
         edge_id,
         edge,
         anonymous=False,
         invert=True,
-        primary_ks_required=False,
         **kwargs
     ):
         """Create an edge reference."""
         edge = dict(edge)  # make shallow copy
         _subject = edge.pop("subject")
         _object = edge.pop("object")
         self.name = edge_id if not anonymous else ""
         self.predicates: List[str] = ensure_list(
             edge.pop("predicates", []) or []
         )
-        # "related_to" is equivalent to no predicate
-        if self.predicates == ["biolink:related_to"]:
+
+        # "related_to" has every predicate as a descendent, it's inclusion is equivalent to no/any predicate
+        if 'biolink:related_to' in self.predicates:
             self.predicates = []
-        if primary_ks_required and not edge.get('_length'):
-            self.filters = [
-                f"`{edge_id}`.`biolink:primary_knowledge_source` IS NOT NULL"
-                ]
-        else:
-            self.filters = []
-        self.qualifier_filters = []
+
+        self.filters = []
+        self.qualifier_filters = ""
         self.label = None  #What goes in the [] on the edge in cypher
         self.length = edge.pop("_length", (1, 1))
         invert = invert and edge.pop("_invert", True)
 
         self.inverse_predicates = []
         self.directed = False # Controls whether there is an arrow on the edge in cypher
         self.symmetric = True # Whether the original top-level predicates are all symmetric
         self.cypher_invert = False # If true, then the cypher source node will be subject, if false then object
         for predicate in self.predicates:
             el = bmt.get_element(space_case(predicate[8:]))
-            if el is None:
-                self.symmetric = False #TODO: Is this right?  If there's no predicate isn't it symmetric?
-                inverse = None
+            if el:
+                inverse_predicate = el.inverse
+                if inverse_predicate is not None:
+                    self.inverse_predicates.append(f"biolink:{snake_case(inverse_predicate)}")
+
+                # if symmetric add to inverse list so we query in both directions
+                if el.symmetric:
+                    self.inverse_predicates.append(predicate)
+                else:
+                    self.symmetric = False
             else:
-                inverse = el.inverse
-                self.symmetric = el.symmetric and self.symmetric
-            # relationship is directed if any provided predicate is asymmetrical
-            if not self.symmetric:
-                self.directed = True
-            if inverse is not None:
-                self.inverse_predicates.append(f"biolink:{snake_case(inverse)}")
-            elif self.symmetric:
-                self.inverse_predicates.append(predicate)
+                error_message = f"Invalid predicate error: (predicate: {predicate}) is not " \
+                                f"a valid biolink model predicate."
+                raise InvalidPredicateError(error_message=error_message)
+
+        # relationship is directed if any provided predicate is asymmetrical
+        if not self.symmetric:
+            self.directed = True
 
         # get all descendant predicates
         self.predicates = [
             f"biolink:{snake_case(p)}"
             for predicate in self.predicates
             for p in bmt.get_descendants(space_case(predicate[8:]))
             if bmt.get_element(p).annotations.get('canonical_predicate',False)
@@ -212,15 +214,14 @@
         self.inverse_predicates = [
             f"biolink:{snake_case(p)}"
             for predicate in self.inverse_predicates
             for p in bmt.get_descendants(space_case(predicate[8:]))
             if bmt.get_element(p).annotations.get('canonical_predicate', False)
         ]
 
-
         unique_preds = list(set(self.predicates + self.inverse_predicates))
         #Having the predicates sorted doesn't matter to neo4j, but it helps in testing b/c we get a consistent string.
         unique_preds.sort()
         self.label = "|".join(
             f"`{predicate}`"
             for predicate in unique_preds
         )
@@ -313,15 +314,15 @@
         ) + (">" if self.directed else "")
 
 
 def build_match_clause(
         *patterns,
         filters=None,
         hints=None,
-        qualifier_filters=[],
+        qualifier_filters="",
         **kwargs,
 ):
     """Build MATCH clause (and subclauses) from components."""
     query = ""
     query += "MATCH " + ", ".join(patterns)
     reg_filters_cypher = ""
     qualifier_filters_cypher = ""
@@ -385,23 +386,32 @@
     Returns the query fragment as a string.
     """
     #If there's no label on a query node, neo4j can't use an index.  This makes such queries basically
     # neo4j killers.   So when there is no category, we add NamedThing which will use an indx.
     for qnode_id, qnode in qgraph["nodes"].items():
         if qnode.get("ids", None) is not None and qnode.get("categories",None) is None:
             qnode["categories"] = ["biolink:NamedThing"]
+
+    # find all of the qnode ids that have subclass or superclass edges connected to them
+    qnode_ids_with_hierarchy_edges = set()
+    for qedge_id, qedge in qgraph["edges"].items():
+        predicates = qedge.get("predicates", None)
+        if predicates and ("biolink:subclass_of" in predicates or "biolink:superclass_of" in predicates):
+            qnode_ids_with_hierarchy_edges.add(qedge['subject'])
+            qnode_ids_with_hierarchy_edges.add(qedge['object'])
+
     if subclass:
         superclasses = {
             qnode_id + "_superclass": {
                 "ids": qnode.pop("ids"),
                 "categories": qnode.pop("categories", None),
                 "_return": False,
             }
             for qnode_id, qnode in qgraph["nodes"].items()
-            if qnode.get("ids", None) is not None
+            if qnode.get("ids", None) is not None and qnode_id not in qnode_ids_with_hierarchy_edges
         }
         subclass_edges = {
             qnode_id[:-11] + "_subclass_edge": {
                 "subject": qnode_id[:-11],
                 "object": qnode_id,
                 "predicates": ["biolink:subclass_of"],
                 "_length": (0, 1),
```

### Comparing `reasoner-transpiler-2.0.1/reasoner_transpiler/nesting.py` & `reasoner-transpiler-2.0.2/reasoner_transpiler/nesting.py`

 * *Files identical despite different names*

### Comparing `reasoner-transpiler-2.0.1/reasoner_transpiler/util.py` & `reasoner-transpiler-2.0.2/reasoner_transpiler/util.py`

 * *Files identical despite different names*

### Comparing `reasoner-transpiler-2.0.1/setup.py` & `reasoner-transpiler-2.0.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Setup reasoner-transpiler package."""
 from setuptools import setup
 
 setup(
     name="reasoner-transpiler",
-    version="2.0.1",
+    version="2.0.2",
     author="Patrick Wang",
     author_email="patrick@covar.com",
     maintainer="Yaphet Kebede",
     maintainer_email="kebedey@renci.org",
     url="https://github.com/ranking-agent/reasoner-transpiler",
     description="TRAPI → Cypher transpiler",
     packages=["reasoner_transpiler"],
```

