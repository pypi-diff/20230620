# Comparing `tmp/Navix-0.2.0.tar.gz` & `tmp/Navix-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Navix-0.2.0.tar", last modified: Fri Jun 16 16:52:21 2023, max compression
+gzip compressed data, was "Navix-0.2.1.tar", last modified: Mon Jun 19 21:27:11 2023, max compression
```

## Comparing `Navix-0.2.0.tar` & `Navix-0.2.1.tar`

### file list

```diff
@@ -1,42 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:21.424184 Navix-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:21.396184 Navix-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:21.408184 Navix-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-16 16:52:09.000000 Navix-0.2.0/.github/workflows/CD.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-16 16:52:09.000000 Navix-0.2.0/.github/workflows/CI.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-16 16:52:09.000000 Navix-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-16 16:52:09.000000 Navix-0.2.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-16 16:52:09.000000 Navix-0.2.0/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-06-16 16:52:09.000000 Navix-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-16 16:52:09.000000 Navix-0.2.0/NOTICE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:21.412184 Navix-0.2.0/Navix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17994 2023-06-16 16:52:21.000000 Navix-0.2.0/Navix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-16 16:52:21.000000 Navix-0.2.0/Navix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 16:52:21.000000 Navix-0.2.0/Navix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-16 16:52:21.000000 Navix-0.2.0/Navix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-16 16:52:21.000000 Navix-0.2.0/Navix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17994 2023-06-16 16:52:21.424184 Navix-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-16 16:52:09.000000 Navix-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:21.412184 Navix-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-16 16:52:09.000000 Navix-0.2.0/docs/design_notes.md
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-16 16:52:09.000000 Navix-0.2.0/docs/profiling.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:21.416184 Navix-0.2.0/navix/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-16 16:52:09.000000 Navix-0.2.0/navix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-06-16 16:52:09.000000 Navix-0.2.0/navix/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-06-16 16:52:09.000000 Navix-0.2.0/navix/components.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:21.420184 Navix-0.2.0/navix/environments/
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-16 16:52:09.000000 Navix-0.2.0/navix/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-06-16 16:52:09.000000 Navix-0.2.0/navix/environments/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-16 16:52:09.000000 Navix-0.2.0/navix/environments/keydoor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-06-16 16:52:09.000000 Navix-0.2.0/navix/environments/room.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-06-16 16:52:09.000000 Navix-0.2.0/navix/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-06-16 16:52:09.000000 Navix-0.2.0/navix/observations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-06-16 16:52:09.000000 Navix-0.2.0/navix/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-16 16:52:09.000000 Navix-0.2.0/navix/terminations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-16 16:52:09.000000 Navix-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-16 16:52:09.000000 Navix-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 16:52:21.424184 Navix-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:52:21.420184 Navix-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-06-16 16:52:09.000000 Navix-0.2.0/tests/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-06-16 16:52:09.000000 Navix-0.2.0/tests/test_environments.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-16 16:52:09.000000 Navix-0.2.0/tests/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-16 16:52:09.000000 Navix-0.2.0/tests/test_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:27:11.332955 Navix-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:27:11.324955 Navix-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:27:11.328955 Navix-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-19 21:26:55.000000 Navix-0.2.1/.github/workflows/CD.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-19 21:26:55.000000 Navix-0.2.1/.github/workflows/CI.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-19 21:26:55.000000 Navix-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-19 21:26:55.000000 Navix-0.2.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-19 21:26:55.000000 Navix-0.2.1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-06-19 21:26:55.000000 Navix-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-19 21:26:55.000000 Navix-0.2.1/NOTICE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:27:11.328955 Navix-0.2.1/Navix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17994 2023-06-19 21:27:11.000000 Navix-0.2.1/Navix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-19 21:27:11.000000 Navix-0.2.1/Navix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 21:27:11.000000 Navix-0.2.1/Navix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-19 21:27:11.000000 Navix-0.2.1/Navix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-19 21:27:11.000000 Navix-0.2.1/Navix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17994 2023-06-19 21:27:11.332955 Navix-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-19 21:26:55.000000 Navix-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:27:11.328955 Navix-0.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-19 21:26:55.000000 Navix-0.2.1/docs/design_notes.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-19 21:26:55.000000 Navix-0.2.1/docs/profiling.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:27:11.332955 Navix-0.2.1/navix/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-19 21:26:55.000000 Navix-0.2.1/navix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-06-19 21:26:55.000000 Navix-0.2.1/navix/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-06-19 21:26:55.000000 Navix-0.2.1/navix/components.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:27:11.332955 Navix-0.2.1/navix/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-19 21:26:55.000000 Navix-0.2.1/navix/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-06-19 21:26:55.000000 Navix-0.2.1/navix/environments/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-19 21:26:55.000000 Navix-0.2.1/navix/environments/keydoor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-19 21:26:55.000000 Navix-0.2.1/navix/environments/room.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-06-19 21:26:55.000000 Navix-0.2.1/navix/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-06-19 21:26:55.000000 Navix-0.2.1/navix/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-06-19 21:26:55.000000 Navix-0.2.1/navix/observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-06-19 21:26:55.000000 Navix-0.2.1/navix/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-19 21:26:55.000000 Navix-0.2.1/navix/terminations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-19 21:26:55.000000 Navix-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-19 21:26:55.000000 Navix-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 21:27:11.332955 Navix-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:27:11.332955 Navix-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-06-19 21:26:55.000000 Navix-0.2.1/tests/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-19 21:26:55.000000 Navix-0.2.1/tests/test_environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-19 21:26:55.000000 Navix-0.2.1/tests/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-19 21:26:55.000000 Navix-0.2.1/tests/test_observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-19 21:26:55.000000 Navix-0.2.1/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-19 21:26:55.000000 Navix-0.2.1/tests/test_terminations.py
```

### Comparing `Navix-0.2.0/.github/workflows/CD.yml` & `Navix-0.2.1/.github/workflows/CD.yml`

 * *Files identical despite different names*

### Comparing `Navix-0.2.0/.github/workflows/CI.yml` & `Navix-0.2.1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `Navix-0.2.0/.gitignore` & `Navix-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `Navix-0.2.0/COPYRIGHT` & `Navix-0.2.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `Navix-0.2.0/LICENSE` & `Navix-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Navix-0.2.0/Navix.egg-info/PKG-INFO` & `Navix-0.2.1/Navix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Navix
-Version: 0.2.0
+Version: 0.2.1
 Summary: Accelerated gridworld navigation with JAX for deep reinforcement learning
 Author-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 Maintainer-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `Navix-0.2.0/PKG-INFO` & `Navix-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Navix
-Version: 0.2.0
+Version: 0.2.1
 Summary: Accelerated gridworld navigation with JAX for deep reinforcement learning
 Author-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 Maintainer-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `Navix-0.2.0/README.md` & `Navix-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `Navix-0.2.0/docs/design_notes.md` & `Navix-0.2.1/docs/design_notes.md`

 * *Files 11% similar despite different names*

```diff
@@ -14,8 +14,9 @@
 - An Array representing the world map (the grid). Notice that entities are not visible on the grid, but only walkable/non-walkable tiles that restrict agent's ability to move.
 - A Player entity, with a position and an action
 - a Goal entity, with a position
 
 
 
 - Coordinates (-1, -1) are a discard pile for entities that are not in the grid.
-- Every entity but the Player is batched, such that its properties have shape (B, *prop_shape).
+- Every entity but the Player is batched, such that its properties have shape (B, *prop_shape).
+- Every entity has a `tag`, which we use to represent the entity in categorical form. The `tag` must be an `int` greater than `1`.
```

### Comparing `Navix-0.2.0/docs/profiling.ipynb` & `Navix-0.2.1/docs/profiling.ipynb`

 * *Files identical despite different names*

### Comparing `Navix-0.2.0/navix/__init__.py` & `Navix-0.2.1/navix/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,20 +14,21 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 __version_info__ = tuple(int(i) for i in __version__.split(".") if i.isdigit())
 
 
 from . import (
     actions,
     components,
+    graphics,
     grid,
     observations,
     tasks,
     environments,
     terminations,
 )
```

### Comparing `Navix-0.2.0/navix/actions.py` & `Navix-0.2.1/navix/actions.py`

 * *Files identical despite different names*

### Comparing `Navix-0.2.0/navix/components.py` & `Navix-0.2.1/navix/components.py`

 * *Files 27% similar despite different names*

```diff
@@ -16,108 +16,80 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 
 from __future__ import annotations
 
-from enum import IntEnum
-from typing import Any, Dict
-
 from jax import Array
 from flax import struct
 from jax.random import KeyArray
 import jax.numpy as jnp
 
 
 class Component(struct.PyTreeNode):
     """A component is a part of the state of the environment."""
+
     position: Array = jnp.zeros((1, 2), dtype=jnp.int32) - 1
     """The (row, column) position of the entity in the grid, defaults to the discard pile (-1, -1)"""
 
 
-# class HasId(Component):
-#     """A component that has an id"""
-
-#     id: Array = jnp.asarray(0)
-
-
-# class HasPosition(Component):
-#     """A component that has a position in the environment"""
-
-#     position: Array = jnp.asarray(0)
-
-
-# class HasDirection(Component):
-#     """A component that has a direction"""
-
-#     direction: Array = jnp.asarray(0)
-
-
-# class Stochastic(Component):
-#     """A component that has a probability"""
-
-#     # key: KeyArray
-#     probability: Array = jnp.asarray(1.0)
-
-
-# class Holder(Component):
-#     """A component wiht a 1-slot pocket to hold other components (id)"""
-
-#     pocket: Array = jnp.asarray(0)
-
-
-# class Replaceable(Component):
-#     """A component that can be replaced by another component (id)"""
-
-#     replacement: Array = jnp.asarray(0)
-
-
-# class Consumable(Component):
-#     """A component that can be consumed by another component (id)"""
-
-#     requires: Array = jnp.asarray(0)
-
-
 class Player(Component):
     """Players are entities that can act around the environment"""
 
+    # TODO(epignatelli): consider batching player over the number of players
+    # to allow tranposing the entities pytree for faster computation
+    # and to prepare the ground for multi-agent environments
+    tag: Array = jnp.asarray(1)
+    """The tag of the component, used to identify the type of the component in `oobservations.categorical`"""
     direction: Array = jnp.asarray(0)
     """The direction the entity: 0 = east, 1 = south, 2 = west, 3 = north"""
     pocket: Array = jnp.asarray(0)
     """The id of the item in the pocket (0 if empty)"""
 
 
 class Goal(Component):
     """Goals are entities that can be reached by the player"""
 
+    tag: Array = jnp.ones((1,), dtype=jnp.int32) + 1
+    """The tag of the component, used to identify the type of the component in `oobservations.categorical`"""
     probability: Array = jnp.ones((1,), dtype=jnp.float32)
     """The probability of receiving the reward, if reached."""
 
+
 class Pickable(Component):
     """Pickable items are world objects that can be picked up by the player.
     Examples of pickable items are keys, coins, etc."""
 
     id: Array = jnp.zeros((1,), dtype=jnp.int32) - 1
     """The id of the item. If set, it must be >= 1."""
 
+    @property
+    def tag(self):
+        return - self.id
+
 
 class Consumable(Component):
     """Consumable items are world objects that can be consumed by the player.
     Consuming an item requires a tool (e.g. a key to open a door).
     A tool is an id (int) of another item, specified in the `requires` field (-1 if no tool is required).
     After an item is consumed, it is both removed from the `state.entities` collection, and replaced in the grid
     by the item specified in the `replacement` field (0 = floor by default).
     Examples of consumables are doors (to open) food (to eat) and water (to drink), etc.
     """
+
     requires: Array = jnp.zeros((1,), dtype=jnp.int32) - 1
     """The id of the item required to consume this item. If set, it must be >= 1."""
     replacement: Array = jnp.zeros((1,), dtype=jnp.float32)
     """The grid signature to replace the item with, usually 0 (floor). If set, it must be >= 1."""
 
+    @property
+    def tag(self):
+        return self.requires
+
 
 class State(struct.PyTreeNode):
     """The Markovian state of the environment"""
 
     key: KeyArray
     """The random number generator state"""
     grid: Array
@@ -126,33 +98,7 @@
     """The player entity"""
     goals: Goal = Goal()
     """The goal entity, batched over the number of goals"""
     keys: Pickable = Pickable()
     """The key entity, batched over the number of keys"""
     doors: Consumable = Consumable()
     """The door entity, batched over the number of doors"""
-
-
-class StepType(IntEnum):
-    TRANSITION = 0
-    """discount > 0, episode continues"""
-    TRUNCATION = 1
-    """discount > 0, episode ends"""
-    TERMINATION = 2
-    """discount == 0, episode ends"""
-
-
-class Timestep(struct.PyTreeNode):
-    t: Array
-    """The number of timesteps elapsed from the last reset of the environment"""
-    observation: Array
-    """The observation corresponding to the current state (for POMDPs)"""
-    action: Array
-    """The action taken by the agent at the current timestep a_t = $\\pi(s_t)$, where $s_t$ is `state`"""
-    reward: Array
-    """The reward $r_{t=1}$ received by the agent after taking action $a_t$"""
-    step_type: Array
-    """The type of the current timestep (see `StepType`)"""
-    state: State
-    """The true state of the MDP, $s_t$ before taking action `action`"""
-    info: Dict[str, Any] = struct.field(default_factory=dict)
-    """Additional information about the environment. Useful for accumulations (e.g. returns)"""
```

### Comparing `Navix-0.2.0/navix/environments/__init__.py` & `Navix-0.2.1/navix/environments/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,10 +17,10 @@
 # specific language governing permissions and limitations
 # under the License.
 
 
 from __future__ import annotations
 
 
-from .environment import Environment
+from .environment import Environment, StepType, Timestep
 from .room import Room
 from .keydoor import KeyDoor
```

### Comparing `Navix-0.2.0/navix/environments/environment.py` & `Navix-0.2.1/navix/tasks.py`

 * *Files 27% similar despite different names*

```diff
@@ -15,78 +15,68 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 
 from __future__ import annotations
-
-import abc
 from typing import Callable
+
+
 import jax
 import jax.numpy as jnp
-from jax.random import KeyArray
 from jax import Array
-from flax import struct
 
-from .. import tasks
-from ..components import State, Timestep, StepType
-from .. import terminations
-from ..actions import ACTIONS
-from .. import observations
-
-
-class Environment(struct.PyTreeNode):
-    width: int = struct.field(pytree_node=False)
-    height: int = struct.field(pytree_node=False)
-    max_steps: int = struct.field(pytree_node=False)
-    gamma: float = struct.field(pytree_node=False, default=1.0)
-    observation_fn: Callable[[State], Array] = struct.field(
-        pytree_node=False, default=observations.categorical
-    )
-    reward_fn: Callable[[State, Array, State], Array] = struct.field(
-        pytree_node=False, default=tasks.navigation
-    )
-    termination_fn: Callable[[State, Array, State], Array] = struct.field(
-        pytree_node=False, default=terminations.on_navigation_completion
+from .components import State
+
+
+def compose(*fns: Callable[[State, Array, State], Array]):
+    def composed(prev_state: State, action: Array, state: State) -> Array:
+        reward = jnp.asarray(0.0)
+        for fn in fns:
+            reward += fn(prev_state, action, state)
+        return reward
+
+    return composed
+
+
+def free(state: State) -> Array:
+    return jnp.asarray(0.0)
+
+
+def navigation(prev_state: State, action: Array, state: State) -> Array:
+    reached = jax.vmap(jnp.array_equal, in_axes=(None, 0))(
+        state.player.position, state.goals.position
     )
+    any_reached = jnp.sum(reached)
 
-    @abc.abstractmethod
-    def reset(self, key: KeyArray) -> Timestep:
-        raise NotImplementedError()
-
-    def _step(self, timestep: Timestep, action: Array, actions_set=ACTIONS) -> Timestep:
-        # update agents
-        state = jax.lax.switch(action, actions_set.values(), timestep.state)
-
-        # build timestep
-        return Timestep(
-            t=timestep.t + 1,
-            state=state,
-            action=jnp.asarray(action),
-            reward=self.reward(timestep.state, action, state),
-            step_type=self.termination(timestep.state, action, state, timestep.t + 1),
-            observation=self.observation(state),
-        )
-
-    def step(self, timestep: Timestep, action: Array, actions_set=ACTIONS) -> Timestep:
-        # autoreset if necessary: 0 = transition, 1 = truncation, 2 = termination
-        should_reset = timestep.step_type > 0
-        return jax.lax.cond(
-            should_reset,
-            lambda timestep: self.reset(timestep.state.key),
-            lambda timestep: self._step(timestep, action, actions_set),
-            timestep,
-        )
-
-    def observation(self, state: State):
-        return self.observation_fn(state)
-
-    def reward(self, state: State, action: Array, new_state: State):
-        return self.reward_fn(state, action, new_state)
-
-    def termination(
-        self, prev_state: State, action: Array, state: State, t: Array
-    ) -> Array:
-        terminated = self.termination_fn(prev_state, action, state)
-        truncated = t >= self.max_steps
-        return terminations.check_truncation(terminated, truncated)
+    draw = jax.random.uniform(state.key, ())
+    reward = any_reached * jnp.greater_equal(draw, state.goals.probability)
+    reward = jnp.asarray(reward, jnp.float32).squeeze()
+
+    # make sure that reward is a scalar
+    assert reward.shape == (), f"Reward must be a scalar but got shape {reward.shape}"
+    return reward
+
+
+def action_cost(
+    prev_state: State, action: Array, new_state: State, cost: float = 0.01
+) -> Array:
+    # noops are free
+    return -jnp.asarray(action > 0, dtype=jnp.float32) * cost
+
+
+def time_cost(
+    prev_state: State, action: Array, new_state: State, cost: float = 0.01
+) -> Array:
+    # time always has a cost
+    return -jnp.asarray(cost)
+
+
+def wall_hit_cost(
+    prev_state: State, action: Array, state: State, cost: float = 0.01
+) -> Array:
+    # if state is unchanged, maybe the wall was hit
+    didnt_move = jnp.array_equal(prev_state.player.position, state.player.position)
+    but_wanted_to = jnp.less_equal(3, action) * jnp.less_equal(action, 6)
+    hit = jnp.logical_and(didnt_move, but_wanted_to)
+    return -jnp.asarray(cost) * hit
```

### Comparing `Navix-0.2.0/navix/environments/room.py` & `Navix-0.2.1/navix/environments/room.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,25 +20,25 @@
 
 from __future__ import annotations
 
 import jax
 import jax.numpy as jnp
 from jax.random import KeyArray
 
-from ..components import Goal, Player, State, Timestep
+from ..components import Goal, Player, State
 from ..grid import random_positions, random_directions, room
-from .environment import Environment
+from .environment import Environment, Timestep
 
 
 class Room(Environment):
     def reset(self, key: KeyArray) -> Timestep:
         key, k1, k2 = jax.random.split(key, 3)
 
         # map
-        grid = room(self.width, self.height)
+        grid = room(height=self.height, width=self.width)
         positions = random_positions(k1, grid, n=2)
         direction = random_directions(k2, n=1)
         # player
         player = Player(position=positions[0], direction=direction)
         # goal
         goal = Goal(position=positions[1][None])
```

### Comparing `Navix-0.2.0/navix/terminations.py` & `Navix-0.2.1/navix/terminations.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,9 +27,11 @@
 
 
 def check_truncation(terminated: Array, truncated: Array) -> Array:
     return jnp.asarray(truncated + 2 * terminated, dtype=jnp.int32)
 
 
 def on_navigation_completion(prev_state: State, action: Array, state: State) -> Array:
-    reached = jax.vmap(jnp.array_equal, in_axes=(None, 0))(state.player.position, state.goals.position)
+    reached = jax.vmap(jnp.array_equal, in_axes=(None, 0))(
+        state.player.position, state.goals.position
+    )
     return jnp.any(reached)
```

### Comparing `Navix-0.2.0/pyproject.toml` & `Navix-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Navix-0.2.0/tests/test_actions.py` & `Navix-0.2.1/tests/test_actions.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,22 +11,30 @@
         jax.random.PRNGKey(0),
         grid=jnp.zeros((3, 3), dtype=jnp.int32),
         player=nx.components.Player(position=jnp.asarray((1, 1)), direction=direction),
     )
 
     msg = "Expected direction to be {}, got {}"
     state = nx.actions._rotate(state, -1)
-    assert state.player.direction == jnp.asarray(3), msg.format(3, state.player.direction)
+    assert state.player.direction == jnp.asarray(3), msg.format(
+        3, state.player.direction
+    )
 
     state = nx.actions._rotate(state, 1)
-    assert state.player.direction == jnp.asarray(0), msg.format(0, state.player.direction)
+    assert state.player.direction == jnp.asarray(0), msg.format(
+        0, state.player.direction
+    )
 
     state = nx.actions._rotate(state, 2)
-    assert state.player.direction == jnp.asarray(2), msg.format(2, state.player.direction)
+    assert state.player.direction == jnp.asarray(2), msg.format(
+        2, state.player.direction
+    )
 
     state = nx.actions._rotate(state, 3)
-    assert state.player.direction == jnp.asarray(1), msg.format(1, state.player.direction)
+    assert state.player.direction == jnp.asarray(1), msg.format(
+        1, state.player.direction
+    )
     return
 
 
-# if __name__ == "__main__":
-#     test_rotation()
+if __name__ == "__main__":
+    test_rotation()
```

### Comparing `Navix-0.2.0/tests/test_environments.py` & `Navix-0.2.1/tests/test_environments.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import jax
 import jax.numpy as jnp
 import navix as nx
 
 
 def test_room():
     def f():
-        env = nx.environments.Room(3, 3, 8)
+        env = nx.environments.Room(height=3, width=3, max_steps=8)
         key = jax.random.PRNGKey(4)
         reset = jax.jit(env.reset)
         step = jax.jit(env.step)
         timestep = reset(key)
         # these are optimal actions for navigation + action_cost
         actions = (
             0,  # noop sanity check
@@ -29,72 +29,17 @@
         return timestep
 
     f()
     timestep = jax.jit(f)()
     print(timestep)
 
 
-def test_termination():
-    def f():
-        env = nx.environments.Room(3, 3, 100)
-        key = jax.random.PRNGKey(4)
-        reset = jax.jit(env.reset)
-        step = jax.jit(env.step)
-        timestep = reset(key)
-        print(timestep)
-        print()
-        # these are optimal actions for navigation + action_cost
-        actions = (
-            0,  # noop sanity check
-            2,  # rotate_ccw
-            3,  # forward
-            3,  # forward
-            2,  # rotate_ccw
-            3,  # forward
-        )
-        for action in actions:
-            timestep = step(timestep, jnp.asarray(action))
-            print(nx.actions.ACTIONS[action])
-            print(timestep)
-            print()
-        return timestep
-
-    timestep = f()
-    msg = f"Timestep should be terminataed ({jnp.asarray(2)}), got {timestep.step_type} instead"
-    assert timestep.step_type == jnp.asarray(2), msg
-
-
-def test_truncation():
-    def f():
-        env = nx.environments.Room(3, 3, 4)
-        key = jax.random.PRNGKey(4)
-        reset = jax.jit(env.reset)
-        step = jax.jit(env.step)
-        timestep = reset(key)
-        # these are optimal actions for navigation + action_cost
-        actions = (
-            0,  # t_0 noop sanity check
-            2,  # t_1 rotate_ccw
-            0,  # t_2 noop
-            0,  # t_3 noop - should be truncated
-        )
-        for action in actions:
-            timestep = step(timestep, jnp.asarray(action))
-        return timestep
-
-    f()
-    timestep = jax.jit(f)()
-    print(timestep)
-    msg = f"Timestep should be truncated ({jnp.asarray(1)}), got {timestep.step_type} instead"
-    assert timestep.step_type == jnp.asarray(1), msg
-
-
 def test_keydoor():
     def f():
-        env = nx.environments.KeyDoor(10, 5, 8)
+        env = nx.environments.KeyDoor(height=5, width=10, max_steps=8)
         key = jax.random.PRNGKey(1)
         reset = jax.jit(env.reset)
         step = jax.jit(env.step)
         timestep = reset(key)
         #  these are optimal actions for navigation + action_cost
         actions = (
             2,  # rotate_ccw
@@ -123,11 +68,9 @@
         return timestep
 
     f()
     jax.jit(f)()
 
 
 if __name__ == "__main__":
-    # test_room()
-    # test_termination()
-    # test_truncation()
-    test_keydoor()
+    test_room()
+    # test_keydoor()
```

### Comparing `Navix-0.2.0/tests/test_tasks.py` & `Navix-0.2.1/tests/test_tasks.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,21 +6,21 @@
     reward_fn = nx.tasks.compose(
         nx.tasks.navigation,
         nx.tasks.action_cost,
         nx.tasks.time_cost,
         nx.tasks.wall_hit_cost,
     )
 
-    env = nx.environments.Room(3, 3, 8, reward_fn=reward_fn)
+    env = nx.environments.Room(height=3, width=3, max_steps=8, reward_fn=reward_fn)
     key = jax.random.PRNGKey(0)
 
     def _test():
         timestep = env.reset(key)
         for _ in range(10):
             timestep = env.step(timestep, jax.random.randint(key, (), 0, 7))
         return timestep
 
     print(jax.jit(_test)())
 
 
-# if __name__ == "__main__":
-#     test_tasks_composition()
+if __name__ == "__main__":
+    test_tasks_composition()
```

