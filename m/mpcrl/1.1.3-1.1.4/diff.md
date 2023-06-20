# Comparing `tmp/mpcrl-1.1.3.tar.gz` & `tmp/mpcrl-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpcrl-1.1.3.tar", last modified: Wed Apr  5 18:13:10 2023, max compression
+gzip compressed data, was "mpcrl-1.1.4.tar", last modified: Tue Jun 20 15:32:26 2023, max compression
```

## Comparing `mpcrl-1.1.3.tar` & `mpcrl-1.1.4.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 18:13:10.647034 mpcrl-1.1.3/
--rw-rw-rw-   0        0        0     1093 2022-11-28 16:28:05.000000 mpcrl-1.1.3/LICENSE
--rw-rw-rw-   0        0        0     5664 2023-04-05 18:13:10.643047 mpcrl-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     4893 2023-04-03 14:05:22.000000 mpcrl-1.1.3/README.md
--rw-rw-rw-   0        0        0     1089 2023-04-05 18:11:46.000000 mpcrl-1.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-05 18:13:10.648031 mpcrl-1.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-05 18:13:10.461427 mpcrl-1.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-05 18:13:10.492322 mpcrl-1.1.3/src/mpcrl/
--rw-rw-rw-   0        0        0     1221 2023-03-21 18:11:20.000000 mpcrl-1.1.3/src/mpcrl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-05 18:13:10.545374 mpcrl-1.1.3/src/mpcrl/agents/
--rw-rw-rw-   0        0        0    18074 2023-04-04 08:16:45.000000 mpcrl-1.1.3/src/mpcrl/agents/agent.py
--rw-rw-rw-   0        0        0    12381 2023-04-03 14:48:05.000000 mpcrl-1.1.3/src/mpcrl/agents/learning_agent.py
--rw-rw-rw-   0        0        0    20798 2023-04-03 14:48:10.000000 mpcrl-1.1.3/src/mpcrl/agents/lstd_dpg.py
--rw-rw-rw-   0        0        0    12834 2023-04-05 18:11:46.000000 mpcrl-1.1.3/src/mpcrl/agents/lstd_q_learning.py
--rw-rw-rw-   0        0        0     9447 2023-04-03 11:24:31.000000 mpcrl-1.1.3/src/mpcrl/agents/rl_learning_agent.py
-drwxrwxrwx   0        0        0        0 2023-04-05 18:13:10.577294 mpcrl-1.1.3/src/mpcrl/core/
--rw-rw-rw-   0        0        0    10013 2023-02-16 12:18:24.000000 mpcrl-1.1.3/src/mpcrl/core/callbacks.py
--rw-rw-rw-   0        0        0     1609 2023-01-07 11:39:22.000000 mpcrl-1.1.3/src/mpcrl/core/errors.py
--rw-rw-rw-   0        0        0     3262 2023-04-03 14:05:22.000000 mpcrl-1.1.3/src/mpcrl/core/experience.py
--rw-rw-rw-   0        0        0     9395 2023-03-17 16:46:56.000000 mpcrl-1.1.3/src/mpcrl/core/exploration.py
--rw-rw-rw-   0        0        0     2752 2023-02-07 17:38:14.000000 mpcrl-1.1.3/src/mpcrl/core/learning_rate.py
--rw-rw-rw-   0        0        0    11415 2023-04-03 14:05:22.000000 mpcrl-1.1.3/src/mpcrl/core/parameters.py
--rw-rw-rw-   0        0        0     5214 2023-02-16 12:25:43.000000 mpcrl-1.1.3/src/mpcrl/core/schedulers.py
--rw-rw-rw-   0        0        0     2660 2023-04-05 18:11:46.000000 mpcrl-1.1.3/src/mpcrl/core/update.py
-drwxrwxrwx   0        0        0        0 2023-04-05 18:13:10.587235 mpcrl-1.1.3/src/mpcrl/util/
--rw-rw-rw-   0        0        0     1442 2023-04-03 14:07:45.000000 mpcrl-1.1.3/src/mpcrl/util/iters.py
--rw-rw-rw-   0        0        0     6359 2023-04-03 14:05:22.000000 mpcrl-1.1.3/src/mpcrl/util/math.py
--rw-rw-rw-   0        0        0      944 2022-12-12 13:51:17.000000 mpcrl-1.1.3/src/mpcrl/util/named.py
-drwxrwxrwx   0        0        0        0 2023-04-05 18:13:10.471391 mpcrl-1.1.3/src/mpcrl/wrappers/
-drwxrwxrwx   0        0        0        0 2023-04-05 18:13:10.604180 mpcrl-1.1.3/src/mpcrl/wrappers/agents/
--rw-rw-rw-   0        0        0      243 2023-01-18 07:53:19.000000 mpcrl-1.1.3/src/mpcrl/wrappers/agents/__init__.py
--rw-rw-rw-   0        0        0     7570 2023-02-16 13:34:37.000000 mpcrl-1.1.3/src/mpcrl/wrappers/agents/log.py
--rw-rw-rw-   0        0        0     1341 2023-01-18 08:25:14.000000 mpcrl-1.1.3/src/mpcrl/wrappers/agents/record_updates.py
--rw-rw-rw-   0        0        0     2958 2023-01-25 16:07:45.000000 mpcrl-1.1.3/src/mpcrl/wrappers/agents/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-05 18:13:10.614144 mpcrl-1.1.3/src/mpcrl/wrappers/envs/
--rw-rw-rw-   0        0        0      175 2023-01-23 17:35:23.000000 mpcrl-1.1.3/src/mpcrl/wrappers/envs/__init__.py
--rw-rw-rw-   0        0        0     4205 2023-03-27 18:27:04.000000 mpcrl-1.1.3/src/mpcrl/wrappers/envs/monitor_episodes.py
--rw-rw-rw-   0        0        0     5200 2023-03-27 18:27:02.000000 mpcrl-1.1.3/src/mpcrl/wrappers/envs/monitor_infos.py
-drwxrwxrwx   0        0        0        0 2023-04-05 18:13:10.515242 mpcrl-1.1.3/src/mpcrl.egg-info/
--rw-rw-rw-   0        0        0     5664 2023-04-05 18:13:10.000000 mpcrl-1.1.3/src/mpcrl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1092 2023-04-05 18:13:10.000000 mpcrl-1.1.3/src/mpcrl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 18:13:10.000000 mpcrl-1.1.3/src/mpcrl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       83 2023-04-05 18:13:10.000000 mpcrl-1.1.3/src/mpcrl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-05 18:13:10.000000 mpcrl-1.1.3/src/mpcrl.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-05 18:13:10.636075 mpcrl-1.1.3/tests/
--rw-rw-rw-   0        0        0    14685 2023-04-05 18:11:46.000000 mpcrl-1.1.3/tests/test_agent.py
--rw-rw-rw-   0        0        0    17226 2023-04-05 18:11:46.000000 mpcrl-1.1.3/tests/test_core.py
--rw-rw-rw-   0        0        0    11943 2023-04-05 15:19:30.000000 mpcrl-1.1.3/tests/test_examples.py
--rw-rw-rw-   0        0        0    50164 2023-04-03 14:05:22.000000 mpcrl-1.1.3/tests/test_quadrotor_q_learning.py
--rw-rw-rw-   0        0        0     4142 2023-03-17 16:36:29.000000 mpcrl-1.1.3/tests/test_util.py
--rw-rw-rw-   0        0        0     8430 2023-04-03 13:32:56.000000 mpcrl-1.1.3/tests/test_wrappers.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:32:26.308061 mpcrl-1.1.4/
+-rw-rw-rw-   0        0        0     1093 2022-11-28 16:28:05.000000 mpcrl-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0     5664 2023-06-20 15:32:26.306163 mpcrl-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4893 2023-04-03 14:05:22.000000 mpcrl-1.1.4/README.md
+-rw-rw-rw-   0        0        0     1089 2023-06-20 15:31:28.000000 mpcrl-1.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-20 15:32:26.308563 mpcrl-1.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-20 15:32:26.140576 mpcrl-1.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-20 15:32:26.160373 mpcrl-1.1.4/src/mpcrl/
+-rw-rw-rw-   0        0        0     1221 2023-03-21 18:11:20.000000 mpcrl-1.1.4/src/mpcrl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:32:26.192161 mpcrl-1.1.4/src/mpcrl/agents/
+-rw-rw-rw-   0        0        0    18074 2023-04-04 08:16:45.000000 mpcrl-1.1.4/src/mpcrl/agents/agent.py
+-rw-rw-rw-   0        0        0    12763 2023-06-20 12:34:42.000000 mpcrl-1.1.4/src/mpcrl/agents/learning_agent.py
+-rw-rw-rw-   0        0        0    20807 2023-06-20 12:32:47.000000 mpcrl-1.1.4/src/mpcrl/agents/lstd_dpg.py
+-rw-rw-rw-   0        0        0    12834 2023-04-18 12:17:41.000000 mpcrl-1.1.4/src/mpcrl/agents/lstd_q_learning.py
+-rw-rw-rw-   0        0        0     9447 2023-04-03 11:24:31.000000 mpcrl-1.1.4/src/mpcrl/agents/rl_learning_agent.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:32:26.214840 mpcrl-1.1.4/src/mpcrl/core/
+-rw-rw-rw-   0        0        0     9996 2023-06-20 12:34:42.000000 mpcrl-1.1.4/src/mpcrl/core/callbacks.py
+-rw-rw-rw-   0        0        0     1609 2023-01-07 11:39:22.000000 mpcrl-1.1.4/src/mpcrl/core/errors.py
+-rw-rw-rw-   0        0        0     3253 2023-06-20 15:31:20.000000 mpcrl-1.1.4/src/mpcrl/core/experience.py
+-rw-rw-rw-   0        0        0     9366 2023-06-20 15:31:20.000000 mpcrl-1.1.4/src/mpcrl/core/exploration.py
+-rw-rw-rw-   0        0        0     2752 2023-02-07 17:38:14.000000 mpcrl-1.1.4/src/mpcrl/core/learning_rate.py
+-rw-rw-rw-   0        0        0    12137 2023-06-20 12:44:02.000000 mpcrl-1.1.4/src/mpcrl/core/parameters.py
+-rw-rw-rw-   0        0        0     5214 2023-02-16 12:25:43.000000 mpcrl-1.1.4/src/mpcrl/core/schedulers.py
+-rw-rw-rw-   0        0        0     2660 2023-04-05 18:11:46.000000 mpcrl-1.1.4/src/mpcrl/core/update.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:32:26.226450 mpcrl-1.1.4/src/mpcrl/util/
+-rw-rw-rw-   0        0        0     2792 2023-06-20 12:34:23.000000 mpcrl-1.1.4/src/mpcrl/util/control.py
+-rw-rw-rw-   0        0        0     1442 2023-04-03 14:07:45.000000 mpcrl-1.1.4/src/mpcrl/util/iters.py
+-rw-rw-rw-   0        0        0     4903 2023-06-20 12:34:23.000000 mpcrl-1.1.4/src/mpcrl/util/math.py
+-rw-rw-rw-   0        0        0      944 2022-12-12 13:51:17.000000 mpcrl-1.1.4/src/mpcrl/util/named.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:32:26.148558 mpcrl-1.1.4/src/mpcrl/wrappers/
+drwxrwxrwx   0        0        0        0 2023-06-20 15:32:26.237528 mpcrl-1.1.4/src/mpcrl/wrappers/agents/
+-rw-rw-rw-   0        0        0      243 2023-01-18 07:53:19.000000 mpcrl-1.1.4/src/mpcrl/wrappers/agents/__init__.py
+-rw-rw-rw-   0        0        0     7570 2023-02-16 13:34:37.000000 mpcrl-1.1.4/src/mpcrl/wrappers/agents/log.py
+-rw-rw-rw-   0        0        0     1341 2023-01-18 08:25:14.000000 mpcrl-1.1.4/src/mpcrl/wrappers/agents/record_updates.py
+-rw-rw-rw-   0        0        0     2958 2023-01-25 16:07:45.000000 mpcrl-1.1.4/src/mpcrl/wrappers/agents/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:32:26.261409 mpcrl-1.1.4/src/mpcrl/wrappers/envs/
+-rw-rw-rw-   0        0        0      175 2023-01-23 17:35:23.000000 mpcrl-1.1.4/src/mpcrl/wrappers/envs/__init__.py
+-rw-rw-rw-   0        0        0     4205 2023-03-27 18:27:04.000000 mpcrl-1.1.4/src/mpcrl/wrappers/envs/monitor_episodes.py
+-rw-rw-rw-   0        0        0     5200 2023-03-27 18:27:02.000000 mpcrl-1.1.4/src/mpcrl/wrappers/envs/monitor_infos.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:32:26.173376 mpcrl-1.1.4/src/mpcrl.egg-info/
+-rw-rw-rw-   0        0        0     5664 2023-06-20 15:32:26.000000 mpcrl-1.1.4/src/mpcrl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1118 2023-06-20 15:32:26.000000 mpcrl-1.1.4/src/mpcrl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 15:32:26.000000 mpcrl-1.1.4/src/mpcrl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2023-06-20 15:32:26.000000 mpcrl-1.1.4/src/mpcrl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-20 15:32:26.000000 mpcrl-1.1.4/src/mpcrl.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 15:32:26.303219 mpcrl-1.1.4/tests/
+-rw-rw-rw-   0        0        0    14685 2023-04-05 18:11:46.000000 mpcrl-1.1.4/tests/test_agent.py
+-rw-rw-rw-   0        0        0    17226 2023-04-05 18:11:46.000000 mpcrl-1.1.4/tests/test_core.py
+-rw-rw-rw-   0        0        0    11946 2023-06-20 12:34:23.000000 mpcrl-1.1.4/tests/test_examples.py
+-rw-rw-rw-   0        0        0    49960 2023-06-20 15:31:11.000000 mpcrl-1.1.4/tests/test_quadrotor_q_learning.py
+-rw-rw-rw-   0        0        0     4646 2023-06-20 12:34:30.000000 mpcrl-1.1.4/tests/test_util.py
+-rw-rw-rw-   0        0        0     8430 2023-04-03 13:32:56.000000 mpcrl-1.1.4/tests/test_wrappers.py
```

### Comparing `mpcrl-1.1.3/LICENSE` & `mpcrl-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.3/PKG-INFO` & `mpcrl-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpcrl
-Version: 1.1.3
+Version: 1.1.4
 Summary: Reinforcement Learning with Model Predictive Control
 Author-email: Filippo Airaldi <filippoairaldi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FilippoAiraldi/mpc-reinforcement-learning
 Project-URL: Bug Tracker, https://github.com/FilippoAiraldi/mpc-reinforcement-learning/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mpcrl-1.1.3/README.md` & `mpcrl-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.3/pyproject.toml` & `mpcrl-1.1.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mpcrl"
-version = "1.1.3"
+version = "1.1.4"
 authors = [
   { name="Filippo Airaldi", email="filippoairaldi@gmail.com" },
 ]
 description = "Reinforcement Learning with Model Predictive Control"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { text = "MIT" }
@@ -18,15 +18,15 @@
 	"Programming Language :: Python :: 3.10",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering :: Mathematics"
 ]
 dependencies = [
     "typing_extensions >= 4.4.0",
-    "csnlp >= 1.5.4",
+    "csnlp >= 1.5.6",
     "scipy >= 1.8.0",
     "gymnasium >= 0.28.1",
     "numba >= 0.54.6"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/FilippoAiraldi/mpc-reinforcement-learning"
```

### Comparing `mpcrl-1.1.3/src/mpcrl/__init__.py` & `mpcrl-1.1.4/src/mpcrl/__init__.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.3/src/mpcrl/agents/agent.py` & `mpcrl-1.1.4/src/mpcrl/agents/agent.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.3/src/mpcrl/agents/learning_agent.py` & `mpcrl-1.1.4/src/mpcrl/agents/learning_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,21 @@
     `update`, which is called to update the learnable parameters of the MPC according to
     the underlying learning methodology (e.g., Bayesian Optimization, RL, etc.) is
     abstract and must be implemented by inheriting classes.
 
     Note: this class makes no assumptions on the learning methodology used to update the
     MPC's learnable parameters."""
 
-    __slots__ = ("_experience", "_learnable_pars", "_update_strategy", "_raises")
+    __slots__ = (
+        "_experience",
+        "_learnable_pars",
+        "_update_strategy",
+        "_updates_enabled",
+        "_raises",
+    )
 
     def __init__(
         self,
         mpc: Mpc[SymType],
         update_strategy: Union[int, UpdateStrategy],
         learnable_parameters: LearnableParametersDict[SymType],
         fixed_parameters: Union[
@@ -102,14 +108,15 @@
             ExperienceReplay(maxlen=1) if experience is None else experience
         )
         if exploration is not None:
             self._exploration = exploration
         if not isinstance(update_strategy, UpdateStrategy):
             update_strategy = UpdateStrategy(update_strategy, "on_timestep_end")
         self._update_strategy = update_strategy
+        self._updates_enabled = True
         self.establish_callback_hooks()
 
     @property
     def experience(self) -> ExperienceReplay[ExpType]:
         """Gets the experience replay memory of the agent."""
         return self._experience
 
@@ -134,14 +141,18 @@
         Parameters
         ----------
         item : experience-type
             Item to be stored in memory.
         """
         self._experience.append(item)
 
+    def evaluate(self, *args: Any, **kwargs: Any) -> npt.NDArray[np.floating]:
+        self._updates_enabled = False
+        return super().evaluate(*args, **kwargs)
+
     def train(
         self,
         env: Env[ObsType, ActType],
         episodes: int,
         seed: Union[None, int, Iterable[int]] = None,
         raises: bool = True,
         env_reset_options: Optional[Dict[str, Any]] = None,
@@ -172,14 +183,15 @@
         ------
         MpcSolverError or MpcSolverWarning
             Raises the error or the warning (depending on `raises`) if any of the MPC
             solvers fail.
         UpdateError or UpdateWarning
             Raises the error or the warning (depending on `raises`) if the update fails.
         """
+        self._updates_enabled = True
         self._raises = raises
         returns = np.zeros(episodes, float)
         self.on_training_start(env)
 
         for episode, current_seed in zip(range(episodes), generate_seeds(seed)):
             self.reset(current_seed)
             state, _ = env.reset(seed=current_seed, options=env_reset_options)
@@ -250,29 +262,31 @@
             )
         # hook updates (always necessary)
         assert self._update_strategy.hook in {
             "on_episode_end",
             "on_timestep_end",
         }, "Updates can be hooked only to episode_end or on_timestep_end."
         args_idx, kwargs_keys = (
-            (1, ("episode",))
+            (slice(1, 2), ("episode",))
             if self._update_strategy.hook == "on_episode_end"
             else (slice(1, 3), ("episode", "timestep"))
         )
         self.hook_callback(
             repr(self._update_strategy),
             self._update_strategy.hook,
             self._check_and_perform_update,
             args_idx,  # type: ignore[arg-type]
             kwargs_keys,
         )
 
-    def _check_and_perform_update(self, episode: int, timestep: Optional[int]) -> None:
+    def _check_and_perform_update(
+        self, episode: int, timestep: Optional[int] = None
+    ) -> None:
         """Internal utility to check if an update is due and perform it."""
-        if not self._update_strategy.can_update():
+        if not self._updates_enabled or not self._update_strategy.can_update():
             return
         update_msg = self.update()
         if update_msg is not None:
             self.on_update_failure(episode, timestep, update_msg, self._raises)
         self.on_update()
 
     def _get_parameters(
```

### Comparing `mpcrl-1.1.3/src/mpcrl/agents/lstd_dpg.py` & `mpcrl-1.1.4/src/mpcrl/agents/lstd_dpg.py`

 * *Files 1% similar despite different names*

```diff
@@ -326,15 +326,15 @@
             # first, check if current rollout has reached its length, and only then
             # invoke on_timestep_end (as it might trigger an update)
             if len(self._rollout) >= self.rollout_length:
                 self._consolidate_rollout_into_memory()
             self.on_timestep_end(env, episode, timestep)
 
         # consolidate rollout at the end of episode, if no length was specified
-        if self.rollout_length is None:
+        if self.rollout_length == float("+inf"):
             self._consolidate_rollout_into_memory()
         return rewards
 
     def _init_sensitivity(
         self, linsolver_type: str
     ) -> Callable[[cs.DM, int], np.ndarray]:
         """Internal utility to compute the derivatives w.r.t. the learnable parameters
```

### Comparing `mpcrl-1.1.3/src/mpcrl/agents/lstd_q_learning.py` & `mpcrl-1.1.4/src/mpcrl/agents/lstd_q_learning.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.3/src/mpcrl/agents/rl_learning_agent.py` & `mpcrl-1.1.4/src/mpcrl/agents/rl_learning_agent.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.3/src/mpcrl/core/callbacks.py` & `mpcrl-1.1.4/src/mpcrl/core/callbacks.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,38 +218,38 @@
     """
 
     def hook_callback(
         self,
         attachername: str,
         callbackname: str,
         func: Callable,
-        args_idx: Union[None, int, slice] = None,
+        args_idx: Union[None, slice] = None,
         kwargs_keys: Union[None, Collection[str], Literal["all"]] = None,
     ) -> None:
         """Hooks a function to be called each time an agent's callback is invoked.
 
         Parameters
         ----------
         attachername : str
             The name of the object requesting the hook. Has only info purposes.
         callbackname : str
             Name of the callback to hook to.
         func : Callable
             function to be called when the callback is invoked.
-        args_idx : int or slice, optional
+        args_idx : slice, optional
             Indices of the `args` of the callback to be passed to `func`, if not `None`.
         kwargs_keys : collection of strings or "all", optional
             Keys of the `kwargs` of the callback to be passed to `func`, if not `None`.
             If `'all'`, then all the kwargs are passed.
         """
         if args_idx is None:
             args_idx = slice(0, 0)
         all_kwargs_keys = False
         if kwargs_keys is None:
-            kwargs_keys = tuple()
+            kwargs_keys = ()
         elif kwargs_keys == "all":
             all_kwargs_keys = True
 
         def decorate(method: Callable) -> Callable:
             @wraps(method)
             def wrapper(*args, **kwargs):
                 out = method(*args, **kwargs)
```

### Comparing `mpcrl-1.1.3/src/mpcrl/core/errors.py` & `mpcrl-1.1.4/src/mpcrl/core/errors.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.3/src/mpcrl/core/experience.py` & `mpcrl-1.1.4/src/mpcrl/core/experience.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from itertools import chain
 from typing import Deque, Iterable, Iterator, Optional, TypeVar, Union
 
-from csnlp.util.random import np_random
+import numpy as np
 
 ExpType = TypeVar("ExpType")
 
 
 class ExperienceReplay(Deque[ExpType]):
     """Deque-based class for RL traning to save and sample experience transitions. The
     class inherits from `collections.deque`, adding a couple of simple functionalities
@@ -42,15 +42,15 @@
         super().__init__(iterable, maxlen=maxlen)
         self.sample_size = sample_size
         self.include_latest = include_latest
         self.reset(seed)
 
     def reset(self, seed: Optional[int] = None) -> None:
         """Resets the sampling RNG."""
-        self.np_random = np_random(seed)
+        self.np_random = np.random.default_rng(seed)
 
     def sample(self) -> Iterator[ExpType]:
         """Samples the experience memory and yields the sampled items.
 
         Returns
         -------
         sample : iterator of T
```

### Comparing `mpcrl-1.1.3/src/mpcrl/core/exploration.py` & `mpcrl-1.1.4/src/mpcrl/core/exploration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from abc import ABC, abstractmethod
 from typing import Any, Literal, Optional, Union
 
 import numpy as np
 import numpy.typing as npt
-from csnlp.util.random import np_random
 
 from mpcrl.core.schedulers import NoScheduling, Scheduler
 
 
 class ExplorationStrategy(ABC):
     """Base class for exploration strategies such as greedy, epsilon-greeyd, etc."""
 
@@ -112,15 +111,15 @@
     @property
     def strength(self) -> npt.NDArray[np.floating]:
         """Gets the current strength of the exploration strategy."""
         return self.strength_scheduler.value
 
     def reset(self, seed: Optional[int] = None) -> None:
         """Resets the exploration RNG."""
-        self.np_random = np_random(seed)
+        self.np_random = np.random.default_rng(seed)
 
     def can_explore(self) -> bool:
         return True
 
     def step(self) -> None:
         """Updates the exploration strength according to its scheduler."""
         self.strength_scheduler.step()
```

### Comparing `mpcrl-1.1.3/src/mpcrl/core/learning_rate.py` & `mpcrl-1.1.4/src/mpcrl/core/learning_rate.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.3/src/mpcrl/core/parameters.py` & `mpcrl-1.1.4/src/mpcrl/core/parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from functools import cached_property
 from itertools import chain
+from numbers import Integral
 from typing import Any, Dict, Generic, Iterable, Optional, Tuple, TypeVar, Union
 
 import numpy as np
 import numpy.typing as npt
 from csnlp.core.cache import invalidate_cache
 from csnlp.util.io import SupportsDeepcopyAndPickle
 
@@ -44,22 +45,26 @@
         sym : T, optional
             An optional reference to a symbolic variable representing this parameter.
 
         Raises
         ------
         ValueError
             Raises if `value`, `lb` or `ub` cannot be broadcasted to a 1D vector with
-            shape equal to `shape`.
+            shape equal to `shape`; or if the shape of the symbolic variable `sym` does
+            not match the shape of the parameter.
         """
         super().__init__()
         self.name = name
-        self.shape = (shape,) if isinstance(shape, int) else shape
+        self.shape: Tuple[int, ...] = (
+            (shape,) if isinstance(shape, Integral) else shape  # type: ignore
+        )
         self.sym = sym
         self.lb: npt.NDArray[np.floating] = np.broadcast_to(lb, shape)
         self.ub: npt.NDArray[np.floating] = np.broadcast_to(ub, shape)
+        self._check_sym_shape()
         self._update_value(value)
 
     @property
     def size(self) -> int:
         """Gets the number of elements in the parameter."""
         return np.prod(self.shape, dtype=int).item()
 
@@ -86,14 +91,24 @@
         ub = self.ub
         if ((v < lb) & ~np.isclose(v, lb, **is_close_kwargs)).any() or (
             (v > ub) & ~np.isclose(v, ub, **is_close_kwargs)
         ).any():
             raise ValueError(f"Updated parameter {self.name} is outside bounds.")
         self.value: npt.NDArray[np.floating] = np.clip(v, lb, ub)
 
+    def _check_sym_shape(self) -> None:
+        """Internal utility for checking that the shape of the symbolic variable matches
+        the shape of the parameter."""
+        if self.sym is None or not hasattr(self.sym, "shape"):
+            return
+        sym_shape = tuple(self.sym.shape)
+        shape = self.shape + tuple(1 for _ in range(len(sym_shape) - len(self.shape)))
+        if sym_shape != shape:
+            raise ValueError("Shape of `sym` does not match `shape`.")
+
     def __str__(self) -> str:
         return f"<{self.name}(shape={self.shape})>"
 
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__}(name={self.name},shape={self.shape})>"
```

### Comparing `mpcrl-1.1.3/src/mpcrl/core/schedulers.py` & `mpcrl-1.1.4/src/mpcrl/core/schedulers.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.3/src/mpcrl/core/update.py` & `mpcrl-1.1.4/src/mpcrl/core/update.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.3/src/mpcrl/util/iters.py` & `mpcrl-1.1.4/src/mpcrl/util/iters.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.3/src/mpcrl/util/math.py` & `mpcrl-1.1.4/src/mpcrl/util/math.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from itertools import combinations
-from typing import Optional, Tuple, Union
+from typing import Union
 
 import casadi as cs
 import numpy as np
 import numpy.typing as npt
 from csnlp.util.math import prod
-from scipy.linalg import solve_discrete_are
 from scipy.special import comb
 
 
 def summarize_array(
     a: npt.NDArray[np.floating], precision: int = 3, ddof: int = 0
 ) -> str:
     """Summarizes the stats of a given array.
@@ -76,64 +75,14 @@
         try:
             return np.linalg.cholesky(A + tau * identity)
         except np.linalg.LinAlgError:
             tau = max(1.05 * tau, beta)
     raise ValueError("Maximum iterations reached.")
 
 
-def dlqr(
-    A: npt.NDArray[np.floating],
-    B: npt.NDArray[np.floating],
-    Q: npt.NDArray[np.floating],
-    R: npt.NDArray[np.floating],
-    M: Optional[npt.NDArray[np.floating]] = None,
-) -> Tuple[npt.NDArray[np.floating], npt.NDArray[np.floating]]:
-    """Get the discrete-time LQR for the given system. Stage costs are
-    ```
-        x'Qx + 2*x'Mu + u'Ru
-    ```
-    with `M = 0`, if not provided.
-
-    Parameters
-    ----------
-    A : array
-        State matrix.
-    B : array
-        Control input matrix.
-    Q : array
-        State weighting matrix.
-    R : array
-        Control input weighting matrix.
-    M : array, optional
-        Mixed state-input weighting matrix, by default None.
-
-    Returns
-    -------
-    tuple of two arrays
-        Returns the optimal state feedback matrix `K` and the quadratic terminal
-        cost-to-go matrix `P`.
-
-    Note
-    ----
-    Inspired by
-    https://bitbucket.org/rawlings-group/mpc-tools-casadi/src/master/mpctools/util.py.
-    """
-    if M is not None:
-        RinvMT = np.linalg.solve(R, M.T)
-        Atilde = A - B.dot(RinvMT)
-        Qtilde = Q - M.dot(RinvMT)
-    else:
-        Atilde = A
-        Qtilde = Q
-        M = np.zeros(B.shape)
-    P = solve_discrete_are(Atilde, B, Qtilde, R)
-    K = np.linalg.solve(B.T.dot(P).dot(B) + R, B.T.dot(P).dot(A) + M.T)
-    return K, P
-
-
 def nchoosek(n: Union[int, npt.ArrayLike], k: int) -> Union[int, np.ndarray]:
     """Emulates the `nchoosek` function from Matlab. Returns the binomial coefficient,
     i.e.,  the number of combinations of `n` items taken `k` at a time. If `n` is an
     array, then it is flatten and all possible combinations of its elements are
     returned.
 
     Parameters
```

### Comparing `mpcrl-1.1.3/src/mpcrl/util/named.py` & `mpcrl-1.1.4/src/mpcrl/util/named.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.3/src/mpcrl/wrappers/agents/log.py` & `mpcrl-1.1.4/src/mpcrl/wrappers/agents/log.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.3/src/mpcrl/wrappers/agents/record_updates.py` & `mpcrl-1.1.4/src/mpcrl/wrappers/agents/record_updates.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.3/src/mpcrl/wrappers/agents/wrapper.py` & `mpcrl-1.1.4/src/mpcrl/wrappers/agents/wrapper.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.3/src/mpcrl/wrappers/envs/monitor_episodes.py` & `mpcrl-1.1.4/src/mpcrl/wrappers/envs/monitor_episodes.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.3/src/mpcrl/wrappers/envs/monitor_infos.py` & `mpcrl-1.1.4/src/mpcrl/wrappers/envs/monitor_infos.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.3/src/mpcrl.egg-info/PKG-INFO` & `mpcrl-1.1.4/src/mpcrl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpcrl
-Version: 1.1.3
+Version: 1.1.4
 Summary: Reinforcement Learning with Model Predictive Control
 Author-email: Filippo Airaldi <filippoairaldi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FilippoAiraldi/mpc-reinforcement-learning
 Project-URL: Bug Tracker, https://github.com/FilippoAiraldi/mpc-reinforcement-learning/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mpcrl-1.1.3/src/mpcrl.egg-info/SOURCES.txt` & `mpcrl-1.1.4/src/mpcrl.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 src/mpcrl/core/errors.py
 src/mpcrl/core/experience.py
 src/mpcrl/core/exploration.py
 src/mpcrl/core/learning_rate.py
 src/mpcrl/core/parameters.py
 src/mpcrl/core/schedulers.py
 src/mpcrl/core/update.py
+src/mpcrl/util/control.py
 src/mpcrl/util/iters.py
 src/mpcrl/util/math.py
 src/mpcrl/util/named.py
 src/mpcrl/wrappers/agents/__init__.py
 src/mpcrl/wrappers/agents/log.py
 src/mpcrl/wrappers/agents/record_updates.py
 src/mpcrl/wrappers/agents/wrapper.py
```

### Comparing `mpcrl-1.1.3/tests/test_agent.py` & `mpcrl-1.1.4/tests/test_agent.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.3/tests/test_core.py` & `mpcrl-1.1.4/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.3/tests/test_examples.py` & `mpcrl-1.1.4/tests/test_examples.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     LearnableParameter,
     LearnableParametersDict,
     LstdDpgAgent,
     LstdQLearningAgent,
     UpdateStrategy,
 )
 from mpcrl import exploration as E
-from mpcrl.util.math import dlqr
+from mpcrl.util.control import dlqr
 from mpcrl.wrappers.agents import Log, RecordUpdates
 from mpcrl.wrappers.envs import MonitorEpisodes
 
 
 class LtiSystem(gym.Env[npt.NDArray[np.floating], float]):
     nx = 2  # number of states
     nu = 1  # number of inputs
```

### Comparing `mpcrl-1.1.3/tests/test_quadrotor_q_learning.py` & `mpcrl-1.1.4/tests/test_quadrotor_q_learning.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,16 +162,15 @@
     def reset(
         self,
         seed: int = None,
         x0: np.ndarray = None,
         xf: np.ndarray = None,
         options: Optional[Dict[str, Any]] = None,
     ) -> Tuple[np.ndarray, Dict[str, Any]]:
-        seed_seq = np.random.SeedSequence(seed)
-        self.np_random = np.random.Generator(np.random.PCG64(seed_seq))
+        self.np_random = np.random.default_rng(seed)
         if x0 is None:
             x0 = self.config.x0
         if xf is None:
             xf = self.config.xf
         self.x = x0
         self.config.x0 = x0
         self.config.xf = xf
@@ -660,16 +659,15 @@
 
 
 class ReplayMemory(Deque[T]):
     def __init__(
         self, iterable: Iterable[T] = (), maxlen: int = None, seed: int = None
     ) -> None:
         super().__init__(iterable, maxlen=maxlen)
-        seed_seq = np.random.SeedSequence(seed)
-        self.np_random = np.random.Generator(np.random.PCG64(seed_seq))
+        self.np_random = np.random.default_rng(seed)
 
     def sample(
         self, n: Union[int, float], include_last_n: Union[int, float]
     ) -> Iterable[T]:
         length = len(self)
         if isinstance(n, float):
             n = int(self.maxlen * n)
@@ -810,16 +808,15 @@
         self.config = (
             init_config(agent_config, self.config_cls)
             if hasattr(self, "config_cls")
             else None
         )
         self.fixed_pars = {} if fixed_pars is None else fixed_pars
         self.seed = seed
-        seed_seq = np.random.SeedSequence(seed)
-        self.np_random = np.random.Generator(np.random.PCG64(seed_seq))
+        self.np_random = np.random.default_rng(seed)
         self.perturbation_chance = 0.0
         self.perturbation_strength = 0.0
         self.last_solution: Solution = None
         self.Q = QuadRotorMPC(env, config=mpc_config, mpctype="Q")
         self.V = QuadRotorMPC(env, config=mpc_config, mpctype="V")
 
     @property
```

### Comparing `mpcrl-1.1.3/tests/test_util.py` & `mpcrl-1.1.4/tests/test_util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import unittest
 from typing import Iterable, Tuple, Union
 
+import casadi as cs
 import numpy as np
 from parameterized import parameterized
 
-from mpcrl.util import iters, math, named
+from mpcrl.util import control, iters, math, named
 
 
 class DummyAgent(named.Named):
     ...
 
 
 class TestNamedAgent(unittest.TestCase):
@@ -43,30 +44,14 @@
     def test_cholesky_added_multiple_identities__raises__max_iterations_reached(self):
         n = 5
         A = np.random.rand(n, n) - np.eye(n) * 5
         A = 0.5 * (A + A.T)
         with self.assertRaisesRegex(ValueError, "Maximum iterations reached."):
             math.cholesky_added_multiple_identities(A, maxiter=1)
 
-    def test_dlqr__returns_correctly(self):
-        K_exp = np.array([[1.075936290787970, 1.824593914133278]])
-        P_exp = np.array(
-            [
-                [6.783278637425703, 2.903698804441288],
-                [2.903698804441288, 5.026668672843932],
-            ]
-        )
-        A = np.array([[1, 0.25], [0, 1]])
-        B = np.array([[0.03], [0.25]])
-        Q = np.eye(2)
-        R = 0.5
-        K, P = math.dlqr(A, B, Q, R)
-        np.testing.assert_allclose(K, K_exp)
-        np.testing.assert_allclose(P, P_exp)
-
     @parameterized.expand(
         [
             ((1, 1), 1),
             ((5, 4), 5),
             (
                 (np.arange(2, 11, 2), 4),
                 np.asarray(
@@ -93,14 +78,47 @@
         p = math.monomial_powers(n, k)
         self.assertEqual(p.shape[1], n)
         np.testing.assert_allclose(p.sum(axis=1), k)
         if out is not None:
             np.testing.assert_allclose(p, out)
 
 
+class TestControl(unittest.TestCase):
+    def test_dlqr__returns_correctly(self):
+        K_exp = np.array([[1.075936290787970, 1.824593914133278]])
+        P_exp = np.array(
+            [
+                [6.783278637425703, 2.903698804441288],
+                [2.903698804441288, 5.026668672843932],
+            ]
+        )
+        A = np.array([[1, 0.25], [0, 1]])
+        B = np.array([[0.03], [0.25]])
+        Q = np.eye(2)
+        R = 0.5
+        K, P = control.dlqr(A, B, Q, R)
+        np.testing.assert_allclose(K, K_exp)
+        np.testing.assert_allclose(P, P_exp)
+
+    def test_rk4__returns_correcly(self):
+        def f(x):
+            return -3 * x
+
+        dt = 0.01
+        x = cs.SX.sym("x")
+        fd = cs.Function("fd", [x], [control.rk4(f, x, dt)])
+
+        Y = [1]
+        for _ in range(100):
+            Y.append(fd(Y[-1]))
+        Y = cs.hcat(Y).full().squeeze()
+        Y_exact = np.exp(-3 * (np.arange(Y.size) * dt))
+        np.testing.assert_allclose(Y, Y_exact)
+
+
 class TestIters(unittest.TestCase):
     @parameterized.expand([(5,), (1,), (22,)])
     def test_bool_cycle__raises__with_negative_freq(self, frequency: int):
         T = frequency * 10
         cycle = iters.bool_cycle(frequency)
         self.assertEqual(T // frequency, sum((next(cycle) for _ in range(T))))
```

### Comparing `mpcrl-1.1.3/tests/test_wrappers.py` & `mpcrl-1.1.4/tests/test_wrappers.py`

 * *Files identical despite different names*

