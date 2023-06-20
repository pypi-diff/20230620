# Comparing `tmp/sym_metanet-1.0.6.tar.gz` & `tmp/sym_metanet-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sym_metanet-1.0.6.tar", last modified: Tue May 30 13:45:57 2023, max compression
+gzip compressed data, was "sym_metanet-1.0.7.tar", last modified: Tue Jun 20 15:39:19 2023, max compression
```

## Comparing `sym_metanet-1.0.6.tar` & `sym_metanet-1.0.7.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 13:45:57.881509 sym_metanet-1.0.6/
--rw-rw-rw-   0        0        0     1093 2022-10-27 09:27:26.000000 sym_metanet-1.0.6/LICENSE
--rw-rw-rw-   0        0        0     6054 2023-05-30 13:45:57.831509 sym_metanet-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     5279 2023-05-25 11:27:33.000000 sym_metanet-1.0.6/README.md
--rw-rw-rw-   0        0        0     1058 2023-05-25 11:30:18.000000 sym_metanet-1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-30 13:45:57.882506 sym_metanet-1.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-30 13:45:57.650478 sym_metanet-1.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-05-30 13:45:57.698419 sym_metanet-1.0.6/src/sym_metanet/
--rw-rw-rw-   0        0        0     1084 2023-01-11 13:34:25.000000 sym_metanet-1.0.6/src/sym_metanet/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 13:45:57.763407 sym_metanet-1.0.6/src/sym_metanet/blocks/
--rw-rw-rw-   0        0        0     4463 2023-02-16 11:02:35.000000 sym_metanet-1.0.6/src/sym_metanet/blocks/base.py
--rw-rw-rw-   0        0        0     4353 2023-05-25 09:49:21.000000 sym_metanet-1.0.6/src/sym_metanet/blocks/destinations.py
--rw-rw-rw-   0        0        0     9951 2023-03-27 10:30:41.000000 sym_metanet-1.0.6/src/sym_metanet/blocks/links.py
--rw-rw-rw-   0        0        0     5000 2023-03-27 08:14:57.000000 sym_metanet-1.0.6/src/sym_metanet/blocks/nodes.py
--rw-rw-rw-   0        0        0    10768 2023-03-27 10:30:49.000000 sym_metanet-1.0.6/src/sym_metanet/blocks/origins.py
-drwxrwxrwx   0        0        0        0 2023-05-30 13:45:57.775575 sym_metanet-1.0.6/src/sym_metanet/engines/
--rw-rw-rw-   0        0        0      153 2022-11-28 11:51:22.000000 sym_metanet-1.0.6/src/sym_metanet/engines/__init__.py
--rw-rw-rw-   0        0        0    16381 2023-05-25 09:43:10.000000 sym_metanet-1.0.6/src/sym_metanet/engines/casadi.py
--rw-rw-rw-   0        0        0    17963 2023-05-25 09:42:07.000000 sym_metanet-1.0.6/src/sym_metanet/engines/core.py
--rw-rw-rw-   0        0        0     8605 2023-05-25 09:42:32.000000 sym_metanet-1.0.6/src/sym_metanet/engines/numpy.py
--rw-rw-rw-   0        0        0      557 2022-11-28 11:51:22.000000 sym_metanet-1.0.6/src/sym_metanet/errors.py
--rw-rw-rw-   0        0        0    20709 2023-03-27 10:20:52.000000 sym_metanet-1.0.6/src/sym_metanet/network.py
-drwxrwxrwx   0        0        0        0 2023-05-30 13:45:57.814518 sym_metanet-1.0.6/src/sym_metanet/util/
--rw-rw-rw-   0        0        0     3620 2022-12-29 23:12:08.000000 sym_metanet-1.0.6/src/sym_metanet/util/funcs.py
--rw-rw-rw-   0        0        0      909 2022-12-30 15:45:07.000000 sym_metanet-1.0.6/src/sym_metanet/util/types.py
--rw-rw-rw-   0        0        0     2066 2022-12-30 15:59:09.000000 sym_metanet-1.0.6/src/sym_metanet/views.py
-drwxrwxrwx   0        0        0        0 2023-05-30 13:45:57.712431 sym_metanet-1.0.6/src/sym_metanet.egg-info/
--rw-rw-rw-   0        0        0     6054 2023-05-30 13:45:57.000000 sym_metanet-1.0.6/src/sym_metanet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      760 2023-05-30 13:45:57.000000 sym_metanet-1.0.6/src/sym_metanet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 13:45:57.000000 sym_metanet-1.0.6/src/sym_metanet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-05-30 13:45:57.000000 sym_metanet-1.0.6/src/sym_metanet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-30 13:45:57.000000 sym_metanet-1.0.6/src/sym_metanet.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-30 13:45:57.821521 sym_metanet-1.0.6/tests/
--rw-rw-rw-   0        0        0     5220 2023-01-11 13:34:26.000000 sym_metanet-1.0.6/tests/test_blocks.py
--rw-rw-rw-   0        0        0    15027 2023-05-25 07:16:50.000000 sym_metanet-1.0.6/tests/test_engines.py
--rw-rw-rw-   0        0        0    11700 2022-12-01 08:54:08.000000 sym_metanet-1.0.6/tests/test_network.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:39:19.069132 sym_metanet-1.0.7/
+-rw-rw-rw-   0        0        0     1093 2022-10-27 09:27:26.000000 sym_metanet-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0     6054 2023-06-20 15:39:19.067129 sym_metanet-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5279 2023-05-25 11:27:33.000000 sym_metanet-1.0.7/README.md
+-rw-rw-rw-   0        0        0     1058 2023-06-20 15:39:12.000000 sym_metanet-1.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-20 15:39:19.070130 sym_metanet-1.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-20 15:39:18.975394 sym_metanet-1.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-06-20 15:39:19.001305 sym_metanet-1.0.7/src/sym_metanet/
+-rw-rw-rw-   0        0        0     1186 2023-06-09 14:09:02.000000 sym_metanet-1.0.7/src/sym_metanet/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:39:19.033402 sym_metanet-1.0.7/src/sym_metanet/blocks/
+-rw-rw-rw-   0        0        0     4463 2023-02-16 11:02:35.000000 sym_metanet-1.0.7/src/sym_metanet/blocks/base.py
+-rw-rw-rw-   0        0        0     4353 2023-06-09 13:55:47.000000 sym_metanet-1.0.7/src/sym_metanet/blocks/destinations.py
+-rw-rw-rw-   0        0        0    13508 2023-06-09 13:11:36.000000 sym_metanet-1.0.7/src/sym_metanet/blocks/links.py
+-rw-rw-rw-   0        0        0     5000 2023-03-27 08:14:57.000000 sym_metanet-1.0.7/src/sym_metanet/blocks/nodes.py
+-rw-rw-rw-   0        0        0    15854 2023-06-09 14:09:02.000000 sym_metanet-1.0.7/src/sym_metanet/blocks/origins.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:39:19.044836 sym_metanet-1.0.7/src/sym_metanet/engines/
+-rw-rw-rw-   0        0        0      153 2022-11-28 11:51:22.000000 sym_metanet-1.0.7/src/sym_metanet/engines/__init__.py
+-rw-rw-rw-   0        0        0    17490 2023-06-09 14:09:02.000000 sym_metanet-1.0.7/src/sym_metanet/engines/casadi.py
+-rw-rw-rw-   0        0        0    19922 2023-06-09 14:09:02.000000 sym_metanet-1.0.7/src/sym_metanet/engines/core.py
+-rw-rw-rw-   0        0        0     9682 2023-06-09 14:09:02.000000 sym_metanet-1.0.7/src/sym_metanet/engines/numpy.py
+-rw-rw-rw-   0        0        0      557 2022-11-28 11:51:22.000000 sym_metanet-1.0.7/src/sym_metanet/errors.py
+-rw-rw-rw-   0        0        0    20709 2023-03-27 10:20:52.000000 sym_metanet-1.0.7/src/sym_metanet/network.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:39:19.050831 sym_metanet-1.0.7/src/sym_metanet/util/
+-rw-rw-rw-   0        0        0     3620 2022-12-29 23:12:08.000000 sym_metanet-1.0.7/src/sym_metanet/util/funcs.py
+-rw-rw-rw-   0        0        0      909 2022-12-30 15:45:07.000000 sym_metanet-1.0.7/src/sym_metanet/util/types.py
+-rw-rw-rw-   0        0        0     2066 2022-12-30 15:59:09.000000 sym_metanet-1.0.7/src/sym_metanet/views.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:39:19.017320 sym_metanet-1.0.7/src/sym_metanet.egg-info/
+-rw-rw-rw-   0        0        0     6054 2023-06-20 15:39:18.000000 sym_metanet-1.0.7/src/sym_metanet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      783 2023-06-20 15:39:18.000000 sym_metanet-1.0.7/src/sym_metanet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 15:39:18.000000 sym_metanet-1.0.7/src/sym_metanet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-06-20 15:39:18.000000 sym_metanet-1.0.7/src/sym_metanet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-20 15:39:18.000000 sym_metanet-1.0.7/src/sym_metanet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 15:39:19.065130 sym_metanet-1.0.7/tests/
+-rw-rw-rw-   0        0        0     5220 2023-01-11 13:34:26.000000 sym_metanet-1.0.7/tests/test_blocks.py
+-rw-rw-rw-   0        0        0    15012 2023-06-20 15:17:18.000000 sym_metanet-1.0.7/tests/test_engines.py
+-rw-rw-rw-   0        0        0    11738 2023-06-07 15:38:20.000000 sym_metanet-1.0.7/tests/test_examples.py
+-rw-rw-rw-   0        0        0    11700 2022-12-01 08:54:08.000000 sym_metanet-1.0.7/tests/test_network.py
```

### Comparing `sym_metanet-1.0.6/LICENSE` & `sym_metanet-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sym_metanet-1.0.6/PKG-INFO` & `sym_metanet-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sym_metanet
-Version: 1.0.6
+Version: 1.0.7
 Summary: Symbolic Modelling of Highway Traffic Networks with METANET
 Author-email: Filippo Airaldi <filippoairaldi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FilippoAiraldi/sym-metanet
 Project-URL: Bug Tracker, https://github.com/FilippoAiraldi/sym-metanet/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `sym_metanet-1.0.6/README.md` & `sym_metanet-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `sym_metanet-1.0.6/pyproject.toml` & `sym_metanet-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sym_metanet"
-version = "1.0.6"
+version = "1.0.7"
 authors = [
   { name="Filippo Airaldi", email="filippoairaldi@gmail.com" },
 ]
 description = "Symbolic Modelling of Highway Traffic Networks with METANET"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { text = "MIT" }
```

### Comparing `sym_metanet-1.0.6/src/sym_metanet/__init__.py` & `sym_metanet-1.0.7/src/sym_metanet/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 __all__ = [
-    "InvalidNetworkError",
+    "engines",
+    "CongestedDestination",
+    "Destination",
     "EngineNotFoundWarning",
     "EngineNotFoundError",
-    "engines",
-    "Node",
+    "InvalidNetworkError",
     "Link",
-    "Origin",
+    "LinkWithVsl",
+    "MainstreamOrigin",
     "MeteredOnRamp",
-    "SimplifiedMeteredOnRamp",
-    "Destination",
-    "CongestedDestination",
     "Network",
+    "Node",
+    "Origin",
+    "SimplifiedMeteredOnRamp",
 ]
 
 import sym_metanet.engines as engines
 from sym_metanet.errors import (
     EngineNotFoundError,
     EngineNotFoundWarning,
     InvalidNetworkError,
@@ -31,11 +33,16 @@
 if _notfound:
     import warnings
 
     warnings.warn("No available symbolic engine found.", EngineNotFoundWarning)
 del _notfound, _engine
 
 from sym_metanet.blocks.destinations import CongestedDestination, Destination
-from sym_metanet.blocks.links import Link
+from sym_metanet.blocks.links import Link, LinkWithVsl
 from sym_metanet.blocks.nodes import Node
-from sym_metanet.blocks.origins import MeteredOnRamp, Origin, SimplifiedMeteredOnRamp
+from sym_metanet.blocks.origins import (
+    MainstreamOrigin,
+    MeteredOnRamp,
+    Origin,
+    SimplifiedMeteredOnRamp,
+)
 from sym_metanet.network import Network
```

### Comparing `sym_metanet-1.0.6/src/sym_metanet/blocks/base.py` & `sym_metanet-1.0.7/src/sym_metanet/blocks/base.py`

 * *Files identical despite different names*

### Comparing `sym_metanet-1.0.6/src/sym_metanet/blocks/destinations.py` & `sym_metanet-1.0.7/src/sym_metanet/blocks/destinations.py`

 * *Files identical despite different names*

### Comparing `sym_metanet-1.0.6/src/sym_metanet/blocks/links.py` & `sym_metanet-1.0.7/src/sym_metanet/blocks/links.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, Collection, Dict, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Any, Collection, Dict, Optional, Set, Tuple, Union
 
 from sym_metanet.blocks.base import ElementWithVars
 from sym_metanet.blocks.origins import MeteredOnRamp
 from sym_metanet.engines.core import EngineBase, get_current_engine
 from sym_metanet.util.funcs import first
 from sym_metanet.util.types import VarType
 
@@ -230,15 +230,15 @@
             if lanes_drop == 0:
                 lanes_drop = None
 
         # step densities
         rho_next = engine.links.step_density(rho, q, q_up, self.lam, self.L, T)
 
         # step speeds
-        Veq = engine.links.Veq(rho, self.v_free, self.rho_crit, self.a)
+        Veq = self._get_equilibrium_speed(engine, rho)
         v_next = engine.links.step_speed(
             v,
             v_up,
             rho,
             rho_down,
             Veq,
             self.lam,
@@ -254,7 +254,99 @@
             self.rho_crit,
         )
         if positive_next_density:
             rho_next = engine.max(0, rho_next)
         if positive_next_speed:
             v_next = engine.max(0, v_next)
         return {"rho": rho_next, "v": v_next}
+
+    def _get_equilibrium_speed(self, engine: EngineBase, rho: VarType) -> VarType:
+        """Internal utility to compute the equilibrium speed for the link's segments."""
+        return engine.links.Veq(rho, self.v_free, self.rho_crit, self.a)
+
+
+class LinkWithVsl(Link[VarType]):
+    """Highway link between two nodes and whose segments are equipped with Variable
+    Speed Limit signs [1, Section 3.3.1].
+
+    References
+    ----------
+    [1] Hegyi, A., 2004, "Model predictive control for integrating traffic control
+        measures", Netherlands TRAIL Research School.
+    """
+
+    __slots__ = ("vsl", "alpha")
+    _actions = {"v_ctrl"}
+
+    def __init__(
+        self, *args: Any, segments_with_vsl: Set[int], alpha: float, **kwargs: Any
+    ) -> None:
+        """Creates an instance of a METANET link with VSL signs.
+
+        Parameters
+        ----------
+        args, kwargs
+            See base class `Link` for the other parameters.
+            Average speed of cars when traffic is freely flowing, i.e., `v_free`.
+        segments_with_vsl : set of ints
+            The set of segment indices that are equipped with a VSL sign (0-based).
+        alpha : float
+            Non-compliance factor to the indicated speed limit.
+
+        References
+        ----------
+        [1] Hegyi, A., 2004, "Model predictive control for integrating traffic control
+            measures", Netherlands TRAIL Research School.
+        """
+        super().__init__(*args, **kwargs)
+        self.vsl = sorted(segments_with_vsl)  # has to be a list for indexing vectors
+        self.alpha = alpha
+        for index in self.vsl:
+            if index >= self.N or index < 0:
+                raise ValueError("Invalid segment index for VSL sign.")
+
+    def init_vars(  # type: ignore[override]
+        self,
+        init_conditions: Optional[Dict[str, VarType]] = None,
+        engine: Optional[EngineBase] = None,
+        **kwargs: Any,
+    ) -> None:
+        """For each segment in the link, initializes
+         - `rho`: densities (state)
+         - `v`: speeds (state)
+        and, if the segment is equipped with a VSL sign, initializes also the control
+        speed
+         - `v_ctrl` (action).
+
+        Parameters
+        ----------
+        init_conditions : dict[str, variable], optional
+            Provides name-variable tuples to initialize states, actions and disturbances
+            with specific values. These values must be compatible with the symbolic
+            engine in type and shape. If not provided, variables are initialized
+            automatically.
+        engine : EngineBase, optional
+            The engine to be used. If `None`, the current engine is used.
+        kwargs
+            See method of base class `Link`.
+        """
+        if init_conditions is None:
+            init_conditions = {}
+        if engine is None:
+            engine = get_current_engine()
+        super().init_vars(init_conditions, engine, **kwargs)
+        self.actions: Dict[str, VarType] = {
+            "v_ctrl": init_conditions["v_ctrl"]
+            if "v_ctrl" in init_conditions
+            else engine.var(f"v_ctrl_{self.name}", len(self.vsl))
+        }
+
+    def _get_equilibrium_speed(self, engine: EngineBase, rho: VarType) -> VarType:
+        return engine.links.controlled_Veq(
+            rho,
+            self.actions["v_ctrl"],
+            self.vsl,
+            self.alpha,
+            self.v_free,
+            self.rho_crit,
+            self.a,
+        )
```

### Comparing `sym_metanet-1.0.6/src/sym_metanet/blocks/nodes.py` & `sym_metanet-1.0.7/src/sym_metanet/blocks/nodes.py`

 * *Files identical despite different names*

### Comparing `sym_metanet-1.0.6/src/sym_metanet/blocks/origins.py` & `sym_metanet-1.0.7/src/sym_metanet/blocks/origins.py`

 * *Files 20% similar despite different names*

```diff
@@ -64,14 +64,158 @@
         )
         assert (
             len(links_down) == 1
         ), "Internal error. Only one link can leave an origin."
         return first(links_down)[-1]
 
 
+class MainstreamOrigin(Origin[VarType]):
+    """Mainstream origin, i.e., and origin whose queue is an abstraction of the sections
+    upstream of boundaries of the freeway network that we are modeling. This origin is
+    also equipped with a speed limit sign that allows to control the speed of the
+    vehicles entering via it. For reference, see [1, Section 3.3.3].
+
+    References
+    [1] Hegyi, A., 2004, "Model predictive control for integrating traffic control
+        measures", Netherlands TRAIL Research School.
+    """
+
+    _states = {"w"}
+    _actions = {"r"}
+    _disturbances = {"d"}
+
+    def init_vars(
+        self,
+        init_conditions: Optional[Dict[str, VarType]] = None,
+        engine: Optional[EngineBase] = None,
+        positive_init_queue: bool = False,
+        **_,
+    ) -> None:
+        """Initializes
+         - `w`: queue length (state)
+         - `v_ctrl`: speed limit (control action)
+         - `d`: demand (disturbance).
+
+        Parameters
+        ----------
+        init_conditions : dict[str, variable], optional
+            Provides name-variable tuples to initialize states, actions and disturbances
+            with specific values. These values must be compatible with the symbolic
+            engine in type and shape. If not provided, variables are initialized
+            automatically.
+        engine : EngineBase, optional
+            The engine to be used. If `None`, the current engine is used.
+        positive_init_queue : bool, optional
+            If `True`, forces the initial queue to be positive, e.g., as
+            `w = max(0, w)`. METANET is in fact known to sometime yield negative
+            quantities, which are infeasible in reality.
+        """
+        if init_conditions is None:
+            init_conditions = {}
+        if engine is None:
+            engine = get_current_engine()
+
+        self.states: Dict[str, VarType] = {
+            "w": init_conditions["w"]
+            if "w" in init_conditions
+            else engine.var(f"w_{self.name}")
+        }
+        self.actions: Dict[str, VarType] = {
+            "v_ctrl": init_conditions["v_ctrl"]
+            if "v_ctrl" in init_conditions
+            else engine.var(f"v_ctrl_{self.name}")
+        }
+        self.disturbances: Dict[str, VarType] = {
+            "d": init_conditions["d"]
+            if "d" in init_conditions
+            else engine.var(f"d_{self.name}")
+        }
+
+        if positive_init_queue:
+            self.states["w"] = engine.max(0, self.states["w"])
+
+    def step_dynamics(
+        self,
+        net: "Network",
+        T: Union[VarType, float],
+        engine: Optional[EngineBase] = None,
+        positive_next_queue: bool = False,
+        **kwargs,
+    ) -> Dict[str, VarType]:
+        """Steps the dynamics of this origin.
+
+        Parameters
+        ----------
+        net : Network
+            The network the origin belongs to.
+        T : variable or float
+            Sampling time.
+        engine : EngineBase, optional
+            The engine to be used. If `None`, the current engine is used.
+        positive_next_queue : bool, optional
+            If `True`, forces the queue at the next time step to be positive, e.g., as
+            `w+ = max(0, w+)`. METANET is in fact known to sometime yield negative
+            quantities, which are infeasible in reality.
+
+        Returns
+        -------
+        Dict[str, variable]
+            A dict with the states of the origin (queue) at the next time step.
+        """
+        if engine is None:
+            engine = get_current_engine()
+
+        q = self.get_flow(net, T, engine, **kwargs)
+        w_next = engine.origins.step_queue(
+            self.states["w"], self.disturbances["d"], q, T
+        )
+
+        if positive_next_queue:
+            w_next = engine.max(0, w_next)
+        return {"w": w_next}
+
+    def get_flow(  # type: ignore[override]
+        self,
+        net: "Network",
+        T: Union[VarType, float],
+        engine: Optional[EngineBase] = None,
+        **_,
+    ) -> VarType:
+        """Computes the (upstream) flow induced by the mainstream oriogin.
+
+        Parameters
+        ----------
+        net : Network
+            The network this destination belongs to.
+        T : variable or float
+            Sampling time of the simulation.
+        engine : EngineBase, optional
+            The engine to be used. If `None`, the current engine is used.
+
+        Returns
+        -------
+        variable
+            The origin's upstream flow.
+        """
+        if engine is None:
+            engine = get_current_engine()
+        link_down = self._get_exiting_link(net)
+        return engine.origins.get_mainstream_flow(
+            self.disturbances["d"],
+            self.states["w"],
+            self.actions["v_ctrl"],
+            link_down.states["v"][0],
+            link_down.rho_crit,
+            link_down.a,
+            link_down.v_free,
+            link_down.lam,
+            T,
+        )
+
+
 class MeteredOnRamp(Origin[VarType]):
     """On-ramp where cars can queue up before being given access to the attached link.
     For reference, look at [1], in particular, Section 3.2.1 and Equations 3.5 and 3.6.
 
     References
     ----------
     [1] Hegyi, A., 2004, "Model predictive control for integrating traffic control
```

### Comparing `sym_metanet-1.0.6/src/sym_metanet/engines/casadi.py` & `sym_metanet-1.0.7/src/sym_metanet/engines/casadi.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,23 +100,58 @@
             )
         return v_next
 
     @staticmethod
     def Veq(rho: VarType, v_free: VarType, rho_crit: VarType, a: VarType) -> VarType:
         return v_free * cs.exp((-1 / a) * cs.power(rho / rho_crit, a))
 
+    @staticmethod
+    def controlled_Veq(
+        rho: VarType,
+        v_ctrl: VarType,
+        vsl: List[int],
+        alpha: VarType,
+        v_free: VarType,
+        rho_crit: VarType,
+        a: VarType,
+    ) -> VarType:
+        Veq = LinksEngine.Veq(rho, v_free, rho_crit, a)
+        Veq[vsl] = cs.fmin(Veq[vsl], (1 + alpha) * v_ctrl)
+        return Veq
+
 
 class OriginsEngine(OriginsEngineBase, Generic[VarType]):
     """CasADi implementation of `sym_metanet.engines.core.OriginsEngineBase`."""
 
     @staticmethod
     def step_queue(w: VarType, d: VarType, q: VarType, T: VarType) -> VarType:
         return w + T * (d - q)
 
     @staticmethod
+    def get_mainstream_flow(
+        d: VarType,
+        w: VarType,
+        v_ctrl: VarType,
+        v_first: VarType,
+        rho_crit: VarType,
+        a: VarType,
+        v_free: VarType,
+        lanes: VarType,
+        T: VarType,
+    ) -> VarType:
+        V_crit = LinksEngine.Veq(rho_crit, v_free, rho_crit, a)
+        v_lim = cs.fmin(v_ctrl, v_first)
+        ratio = v_lim / v_free
+        ratio = cs.fmax(0.05, cs.fmin(1.0, ratio))  # limit ratio to avoid nans
+        q_speed = lanes * v_lim * rho_crit * cs.power(-a * cs.log(ratio), 1 / a)
+        q_cap = lanes * V_crit * rho_crit
+        q_lim = cs.if_else(v_lim < V_crit, q_speed, q_cap)
+        return cs.fmin(d + w / T, q_lim)
+
+    @staticmethod
     def get_ramp_flow(
         d: VarType,
         w: VarType,
         C: VarType,
         r: VarType,
         rho_max: VarType,
         rho_first: VarType,
```

### Comparing `sym_metanet-1.0.6/src/sym_metanet/engines/core.py` & `sym_metanet-1.0.7/src/sym_metanet/engines/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, Callable, Dict, Literal, Type, Union
+from typing import TYPE_CHECKING, Callable, Dict, List, Literal, Type, Union
 
 import sym_metanet
 from sym_metanet.errors import EngineNotFoundError
 
 if TYPE_CHECKING:
     from sym_metanet.network import Network
 
@@ -232,14 +232,43 @@
 
         Returns
         -------
         Veq
             The equilibrium speed of the link.
         """
 
+    @staticmethod
+    @abstractmethod
+    def controlled_Veq(rho, v_ctrl, vsl: List[int], alpha, v_free, rho_crit, a):
+        """Computes the equilibrium speed of the link where some of its segments are
+        controlled with variable speed limits, according to [1, Equation 3.11].
+
+        Parameters
+        ----------
+        rho
+            Densities of the link's segments.
+        v_ctrl
+            Speed limits of the controlled segments.
+        vsl
+            List of indices of the controlled segments.
+        alpha
+            Non-compliance factor to the indicated speeds.
+        v_free
+            Free-flow speed of the link.
+        rho_crit
+            Critical density of the link.
+        a
+            Model parameter in the equilibrium speed exponent.
+
+        Returns
+        -------
+        Veq
+            The controlled equilibrium speed of the link.
+        """
+
 
 class OriginsEngineBase(ABC):
     """Abstract class of a symbolic engine for modelling highway origins via the METANET
     framework. The methods of this class implement the various equations proposed in the
     framework, which can be found in [1].
 
     References
@@ -269,18 +298,51 @@
         -------
         queue_next
             The queue of the origin at the next time instant.
         """
 
     @staticmethod
     @abstractmethod
+    def get_mainstream_flow(d, w, v_ctrl, v_first, rho_crit, a, v_free, lanes, T):
+        """Computes the flow of a mainstream origin according to [1, Section 3.3.3].
+
+        Parameters
+        ----------
+        d
+            Demand at the origin.
+        w
+            Queue of the origin.
+        v_ctrl
+            Speed limit of the mainstream origin.
+        v_first
+            Speed of the first segment of the link the origin is attached to.
+        rho_crit
+            Critical density of the link the origin is attached to.
+        a
+            Model parameter (in the equilibrium speed)  of the link the origin is
+            attached to.
+        v_free
+            Free-flow speed of the link the origin is attached to.
+        lanes
+            Number of lanes in the link the origin is attached to.
+        T
+            Sampling time.
+
+        Returns
+        -------
+        flow
+            The flow of the mainstream origin.
+        """
+
+    @staticmethod
+    @abstractmethod
     def get_ramp_flow(
         d, w, C, r, rho_max, rho_first, rho_crit, T, type: Literal["in", "out"] = "out"
     ):
-        """Computes the flows of the ramp origin according to [1, Equation 3.5] if
+        """Computes the flow of the ramp origin according to [1, Equation 3.5] if
         `type='in'`, or [1, Equation 3.6] if `type='out'`.
 
         Parameters
         ----------
         d
             Demand at the ramp.
         w
@@ -316,15 +378,15 @@
         C=None,
         rho_max=None,
         rho_first=None,
         rho_crit=None,
         T=None,
         type: Literal["limited", "unlimited"] = "limited",
     ):
-        """Computes the flows of a simplified ramp origin.
+        """Computes the flow of a simplified ramp origin.
 
         Parameters
         ----------
         qdes
             Desired flow at the ramp.
         d : optional
             Demand at the ramp.
```

### Comparing `sym_metanet-1.0.6/src/sym_metanet/engines/numpy.py` & `sym_metanet-1.0.7/src/sym_metanet/engines/numpy.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Callable, Literal, Optional, Type, Union
+from typing import Callable, List, Literal, Optional, Type, Union
 
 import numpy as np
 
 from sym_metanet.engines.core import (
     DestinationsEngineBase,
     EngineBase,
     LinksEngineBase,
@@ -86,27 +86,62 @@
 
     @staticmethod
     def Veq(
         rho: np.ndarray, v_free: np.ndarray, rho_crit: np.ndarray, a: np.ndarray
     ) -> np.ndarray:
         return v_free * np.exp((-1 / a) * np.power(rho / rho_crit, a))
 
+    @staticmethod
+    def controlled_Veq(
+        rho: np.ndarray,
+        v_ctrl: np.ndarray,
+        vsl: List[int],
+        alpha: np.ndarray,
+        v_free: np.ndarray,
+        rho_crit: np.ndarray,
+        a: np.ndarray,
+    ):
+        Veq = LinksEngine.Veq(rho, v_free, rho_crit, a)
+        Veq[vsl] = np.minimum(Veq[vsl], (1 + alpha) * v_ctrl)
+        return Veq
+
 
 class OriginsEngine(OriginsEngineBase):
     """
     NumPy implementation of `sym_metanet.engines.core.OriginsEngineBase`.
     """
 
     @staticmethod
     def step_queue(
         w: np.ndarray, d: np.ndarray, q: np.ndarray, T: np.ndarray
     ) -> np.ndarray:
         return w + T * (d - q)
 
     @staticmethod
+    def get_mainstream_flow(
+        d: np.ndarray,
+        w: np.ndarray,
+        v_ctrl: np.ndarray,
+        v_first: np.ndarray,
+        rho_crit: np.ndarray,
+        a: np.ndarray,
+        v_free: np.ndarray,
+        lanes: np.ndarray,
+        T: np.ndarray,
+    ) -> np.ndarray:
+        V_crit = LinksEngine.Veq(rho_crit, v_free, rho_crit, a)
+        v_lim = np.minimum(v_ctrl, v_first)
+        q_speed = (
+            lanes * v_lim * rho_crit * np.power(-a * np.log(v_lim / v_free), 1 / a)
+        )
+        q_cap = lanes * V_crit * rho_crit
+        q_lim = q_speed if v_lim < V_crit else q_cap
+        return np.minimum(d + w / T, q_lim)
+
+    @staticmethod
     def get_ramp_flow(
         d: np.ndarray,
         w: np.ndarray,
         C: np.ndarray,
         r: np.ndarray,
         rho_max: np.ndarray,
         rho_first: np.ndarray,
```

### Comparing `sym_metanet-1.0.6/src/sym_metanet/errors.py` & `sym_metanet-1.0.7/src/sym_metanet/errors.py`

 * *Files identical despite different names*

### Comparing `sym_metanet-1.0.6/src/sym_metanet/network.py` & `sym_metanet-1.0.7/src/sym_metanet/network.py`

 * *Files identical despite different names*

### Comparing `sym_metanet-1.0.6/src/sym_metanet/util/funcs.py` & `sym_metanet-1.0.7/src/sym_metanet/util/funcs.py`

 * *Files identical despite different names*

### Comparing `sym_metanet-1.0.6/src/sym_metanet/util/types.py` & `sym_metanet-1.0.7/src/sym_metanet/util/types.py`

 * *Files identical despite different names*

### Comparing `sym_metanet-1.0.6/src/sym_metanet/views.py` & `sym_metanet-1.0.7/src/sym_metanet/views.py`

 * *Files identical despite different names*

### Comparing `sym_metanet-1.0.6/src/sym_metanet.egg-info/PKG-INFO` & `sym_metanet-1.0.7/src/sym_metanet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sym-metanet
-Version: 1.0.6
+Version: 1.0.7
 Summary: Symbolic Modelling of Highway Traffic Networks with METANET
 Author-email: Filippo Airaldi <filippoairaldi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FilippoAiraldi/sym-metanet
 Project-URL: Bug Tracker, https://github.com/FilippoAiraldi/sym-metanet/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `sym_metanet-1.0.6/src/sym_metanet.egg-info/SOURCES.txt` & `sym_metanet-1.0.7/src/sym_metanet.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -19,8 +19,9 @@
 src/sym_metanet/engines/casadi.py
 src/sym_metanet/engines/core.py
 src/sym_metanet/engines/numpy.py
 src/sym_metanet/util/funcs.py
 src/sym_metanet/util/types.py
 tests/test_blocks.py
 tests/test_engines.py
+tests/test_examples.py
 tests/test_network.py
```

### Comparing `sym_metanet-1.0.6/tests/test_blocks.py` & `sym_metanet-1.0.7/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `sym_metanet-1.0.6/tests/test_engines.py` & `sym_metanet-1.0.7/tests/test_engines.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,15 +204,15 @@
             **other_pars,
             parameters=sym_pars,
             more_out=True,
             compact=1,
         )
         Fexp = get_hardcoded_dynamics(**other_pars, link_with_ramp=link_with_ramp)
 
-        np_random = np.random.Generator(np.random.PCG64(69420))
+        np_random = np.random.default_rng(69420)
         names = Fact.name_out()
         for i in range(1_000):
             if i == 0:
                 rho = np.asarray([10, 10, 10])
                 v = np.asarray([100, 100, 100])
                 w = np.asarray([0, 0])
                 r = 1.0
```

### Comparing `sym_metanet-1.0.6/tests/test_network.py` & `sym_metanet-1.0.7/tests/test_network.py`

 * *Files identical despite different names*

