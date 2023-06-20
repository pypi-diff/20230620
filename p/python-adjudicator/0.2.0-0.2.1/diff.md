# Comparing `tmp/python_adjudicator-0.2.0.tar.gz` & `tmp/python_adjudicator-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_adjudicator-0.2.0.tar", max compression
+gzip compressed data, was "python_adjudicator-0.2.1.tar", max compression
```

## Comparing `python_adjudicator-0.2.0.tar` & `python_adjudicator-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      988 2023-05-19 08:45:58.545191 python_adjudicator-0.2.0/LICENSE
--rw-r--r--   0        0        0     2560 2023-05-19 09:34:38.810342 python_adjudicator-0.2.0/README.md
--rw-r--r--   0        0        0     1852 2023-05-25 21:39:30.539279 python_adjudicator-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2019 2023-05-19 08:50:35.058438 python_adjudicator-0.2.0/src/adjudicator/Cache.py
--rw-r--r--   0        0        0     3137 2023-05-19 08:50:35.058438 python_adjudicator-0.2.0/src/adjudicator/Executor.py
--rw-r--r--   0        0        0     1530 2023-05-19 09:42:57.372585 python_adjudicator-0.2.0/src/adjudicator/HashSupport.py
--rw-r--r--   0        0        0     5579 2023-05-19 09:50:25.658731 python_adjudicator-0.2.0/src/adjudicator/Params.py
--rw-r--r--   0        0        0      892 2023-05-19 08:51:12.194651 python_adjudicator-0.2.0/src/adjudicator/Params_test.py
--rw-r--r--   0        0        0     4652 2023-05-25 21:37:23.072475 python_adjudicator-0.2.0/src/adjudicator/Rule.py
--rw-r--r--   0        0        0      739 2023-05-25 21:37:23.012476 python_adjudicator-0.2.0/src/adjudicator/Rule_test.py
--rw-r--r--   0        0        0     4385 2023-05-19 09:51:54.739163 python_adjudicator-0.2.0/src/adjudicator/RulesEngine.py
--rw-r--r--   0        0        0     2643 2023-05-19 09:37:37.623158 python_adjudicator-0.2.0/src/adjudicator/RulesEngine_test.py
--rw-r--r--   0        0        0     3036 2023-05-19 08:50:35.090438 python_adjudicator-0.2.0/src/adjudicator/RulesGraph.py
--rw-r--r--   0        0        0     2615 2023-05-19 08:50:35.062438 python_adjudicator-0.2.0/src/adjudicator/RulesGraph_test.py
--rw-r--r--   0        0        0      420 2023-05-16 21:13:35.338396 python_adjudicator-0.2.0/src/adjudicator/Signature.py
--rw-r--r--   0        0        0      682 2023-05-25 21:39:30.539279 python_adjudicator-0.2.0/src/adjudicator/__init__.py
--rw-r--r--   0        0        0     1397 2023-05-19 08:50:35.062438 python_adjudicator-0.2.0/src/adjudicator/errors.py
--rw-r--r--   0        0        0        0 2023-05-19 08:45:58.549191 python_adjudicator-0.2.0/src/adjudicator/py.typed
--rw-r--r--   0        0        0     3285 1970-01-01 00:00:00.000000 python_adjudicator-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      988 2023-06-20 18:55:00.877861 python_adjudicator-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2560 2023-06-20 18:55:00.878072 python_adjudicator-0.2.1/README.md
+-rw-r--r--   0        0        0     1874 2023-06-20 18:56:25.123563 python_adjudicator-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2019 2023-06-20 18:55:00.880353 python_adjudicator-0.2.1/src/adjudicator/Cache.py
+-rw-r--r--   0        0        0     3137 2023-06-20 18:55:00.880578 python_adjudicator-0.2.1/src/adjudicator/Executor.py
+-rw-r--r--   0        0        0     1530 2023-06-20 18:55:00.880788 python_adjudicator-0.2.1/src/adjudicator/HashSupport.py
+-rw-r--r--   0        0        0     5579 2023-06-20 18:55:00.881002 python_adjudicator-0.2.1/src/adjudicator/Params.py
+-rw-r--r--   0        0        0      892 2023-06-20 18:55:00.881198 python_adjudicator-0.2.1/src/adjudicator/Params_test.py
+-rw-r--r--   0        0        0     4652 2023-06-20 18:55:00.881419 python_adjudicator-0.2.1/src/adjudicator/Rule.py
+-rw-r--r--   0        0        0      739 2023-06-20 18:55:00.881611 python_adjudicator-0.2.1/src/adjudicator/Rule_test.py
+-rw-r--r--   0        0        0     4475 2023-06-20 18:55:47.321833 python_adjudicator-0.2.1/src/adjudicator/RulesEngine.py
+-rw-r--r--   0        0        0     2643 2023-06-20 18:55:00.882143 python_adjudicator-0.2.1/src/adjudicator/RulesEngine_test.py
+-rw-r--r--   0        0        0     3121 2023-06-20 18:55:09.531720 python_adjudicator-0.2.1/src/adjudicator/RulesGraph.py
+-rw-r--r--   0        0        0     2615 2023-06-20 18:55:00.882556 python_adjudicator-0.2.1/src/adjudicator/RulesGraph_test.py
+-rw-r--r--   0        0        0      420 2023-06-20 18:55:00.882716 python_adjudicator-0.2.1/src/adjudicator/Signature.py
+-rw-r--r--   0        0        0      682 2023-06-20 18:56:25.123762 python_adjudicator-0.2.1/src/adjudicator/__init__.py
+-rw-r--r--   0        0        0     1397 2023-06-20 18:55:00.883062 python_adjudicator-0.2.1/src/adjudicator/errors.py
+-rw-r--r--   0        0        0        0 2023-06-20 18:55:00.883183 python_adjudicator-0.2.1/src/adjudicator/py.typed
+-rw-r--r--   0        0        0     3307 1970-01-01 00:00:00.000000 python_adjudicator-0.2.1/PKG-INFO
```

### Comparing `python_adjudicator-0.2.0/LICENSE` & `python_adjudicator-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.2.0/README.md` & `python_adjudicator-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.2.0/pyproject.toml` & `python_adjudicator-0.2.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "python-adjudicator"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
-authors = ["Unknown <me@unknown.org>"]
+authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "adjudicator", from = "src" }]
 classifiers = []
 keywords = []
 
 [tool.poetry.urls]
```

### Comparing `python_adjudicator-0.2.0/src/adjudicator/Cache.py` & `python_adjudicator-0.2.1/src/adjudicator/Cache.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.2.0/src/adjudicator/Executor.py` & `python_adjudicator-0.2.1/src/adjudicator/Executor.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.2.0/src/adjudicator/HashSupport.py` & `python_adjudicator-0.2.1/src/adjudicator/HashSupport.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.2.0/src/adjudicator/Params.py` & `python_adjudicator-0.2.1/src/adjudicator/Params.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.2.0/src/adjudicator/Params_test.py` & `python_adjudicator-0.2.1/src/adjudicator/Params_test.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.2.0/src/adjudicator/Rule.py` & `python_adjudicator-0.2.1/src/adjudicator/Rule.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.2.0/src/adjudicator/Rule_test.py` & `python_adjudicator-0.2.1/src/adjudicator/Rule_test.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.2.0/src/adjudicator/RulesEngine.py` & `python_adjudicator-0.2.1/src/adjudicator/RulesEngine.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,14 +68,17 @@
             inputs = self.facts.filter(rule.input_types) | params.filter(rule.input_types)
             output = self.executor.execute(rule, inputs, self)
             params = params | Params({rule.output_type: output}, self.hashsupport)
 
         assert isinstance(output, output_type), f"Expected {output_type}, got {type(output)}"
         return output
 
+    def add_rules(self, rules: Iterable[Rule]) -> None:
+        self.graph.update(rules)
+
     def assert_facts(self, facts: Params.InitType) -> None:
         """
         Assert facts to the rules engine. Note that this will fail if a fact of the given type already exists in
         the rules engine.
         """
 
         facts = Params(facts)
```

### Comparing `python_adjudicator-0.2.0/src/adjudicator/RulesEngine_test.py` & `python_adjudicator-0.2.1/src/adjudicator/RulesEngine_test.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.2.0/src/adjudicator/RulesGraph.py` & `python_adjudicator-0.2.1/src/adjudicator/RulesGraph.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,41 +12,45 @@
 
 class RulesGraph:
     """
     This graph contains types as the nodes and rules are the edges.
     """
 
     def __init__(self, rules: Iterable[Rule] | RulesGraph) -> None:
+        self._rules: dict[str, Rule] = {}
+
         if isinstance(rules, RulesGraph):
-            self._rules: dict[str, Rule] = rules._rules.copy()
+            rules = list(rules._rules.values())
         else:
             rules = list(rules)
-            self._rules = {r.id: r for r in rules}
-            if len(self._rules) != len(rules):
-                raise ValueError("Duplicate rule IDs")
 
         self._graph = MultiDiGraph()
-        for rule in self._rules.values():
-            self._graph.add_nodes_from(rule.input_types)
-            self._graph.add_node(rule.output_type)
-            for input_type in rule.input_types:
-                self._graph.add_edge(input_type, rule.output_type, rule=rule)
-
-        if not is_directed_acyclic_graph(self._graph):  # type: ignore[no-untyped-call]
-            raise ValueError("Rules graph is not acyclic")
+        self.update(rules)
 
     def __iter__(self) -> Iterable[Rule]:
         return iter(self._rules.values())
 
     def __len__(self) -> int:
         return len(self._rules)
 
     def __getitem__(self, rule_id: str) -> Rule:
         return self._rules[rule_id]
 
+    def update(self, rules: Iterable[Rule]) -> None:
+        for rule in rules:
+            if rule.id in self._rules:
+                raise ValueError("Duplicate rule ID: " + rule.id)
+            self._rules[rule.id] = rule
+            self._graph.add_nodes_from(rule.input_types)
+            self._graph.add_node(rule.output_type)
+            for input_type in rule.input_types:
+                self._graph.add_edge(input_type, rule.output_type, rule=rule)
+        if not is_directed_acyclic_graph(self._graph):  # type: ignore[no-untyped-call]
+            raise ValueError("Rules graph is not acyclic")
+
     def rules_for(self, output_type: type[Any]) -> set[Rule]:
         """
         Return all rules that can generate the specified output type.
         """
 
         rules: set[Rule] = set()
         if output_type not in self._graph.nodes:
```

### Comparing `python_adjudicator-0.2.0/src/adjudicator/RulesGraph_test.py` & `python_adjudicator-0.2.1/src/adjudicator/RulesGraph_test.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.2.0/src/adjudicator/__init__.py` & `python_adjudicator-0.2.1/src/adjudicator/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,8 +21,8 @@
     "rule",
     "Rule",
     "RuleResolveError",
     "RulesEngine",
     "RulesGraph",
 ]
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
```

### Comparing `python_adjudicator-0.2.0/src/adjudicator/errors.py` & `python_adjudicator-0.2.1/src/adjudicator/errors.py`

 * *Files identical despite different names*

### Comparing `python_adjudicator-0.2.0/PKG-INFO` & `python_adjudicator-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: python-adjudicator
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 License: MIT
-Author: Unknown
-Author-email: me@unknown.org
+Author: Niklas Rosenstein
+Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: networkx (>=3.1,<4.0)
 Requires-Dist: typeapi (>=1.4.2,<2.0.0)
```

