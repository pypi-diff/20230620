# Comparing `tmp/memory-maze-1.0.2.tar.gz` & `tmp/memory-maze-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memory-maze-1.0.2.tar", last modified: Wed Oct 26 16:41:55 2022, max compression
+gzip compressed data, was "memory-maze-1.0.3.tar", last modified: Tue Jun 20 07:23:00 2023, max compression
```

## Comparing `memory-maze-1.0.2.tar` & `memory-maze-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 16:41:55.055403 memory-maze-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-10-26 16:41:45.000000 memory-maze-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    12936 2022-10-26 16:41:55.055403 memory-maze-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    12608 2022-10-26 16:41:45.000000 memory-maze-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 16:41:55.055403 memory-maze-1.0.2/memory_maze/
--rw-r--r--   0 runner    (1001) docker     (121)     3105 2022-10-26 16:41:45.000000 memory-maze-1.0.2/memory_maze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1935 2022-10-26 16:41:45.000000 memory-maze-1.0.2/memory_maze/gym_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (121)      396 2022-10-26 16:41:45.000000 memory-maze-1.0.2/memory_maze/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)    13547 2022-10-26 16:41:45.000000 memory-maze-1.0.2/memory_maze/maze.py
--rw-r--r--   0 runner    (1001) docker     (121)     3709 2022-10-26 16:41:45.000000 memory-maze-1.0.2/memory_maze/oracle.py
--rw-r--r--   0 runner    (1001) docker     (121)     4733 2022-10-26 16:41:45.000000 memory-maze-1.0.2/memory_maze/tasks.py
--rw-r--r--   0 runner    (1001) docker     (121)     8327 2022-10-26 16:41:45.000000 memory-maze-1.0.2/memory_maze/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 16:41:55.055403 memory-maze-1.0.2/memory_maze.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    12936 2022-10-26 16:41:55.000000 memory-maze-1.0.2/memory_maze.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      396 2022-10-26 16:41:55.000000 memory-maze-1.0.2/memory_maze.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-26 16:41:55.000000 memory-maze-1.0.2/memory_maze.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-26 16:41:54.000000 memory-maze-1.0.2/memory_maze.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-10-26 16:41:55.000000 memory-maze-1.0.2/memory_maze.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-10-26 16:41:55.000000 memory-maze-1.0.2/memory_maze.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-26 16:41:55.055403 memory-maze-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      576 2022-10-26 16:41:45.000000 memory-maze-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:23:00.279494 memory-maze-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-20 07:22:46.000000 memory-maze-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13416 2023-06-20 07:23:00.279494 memory-maze-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13088 2023-06-20 07:22:46.000000 memory-maze-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:23:00.279494 memory-maze-1.0.3/memory_maze/
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-06-20 07:22:46.000000 memory-maze-1.0.3/memory_maze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-20 07:22:46.000000 memory-maze-1.0.3/memory_maze/gym_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-20 07:22:46.000000 memory-maze-1.0.3/memory_maze/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16088 2023-06-20 07:22:46.000000 memory-maze-1.0.3/memory_maze/maze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-20 07:22:46.000000 memory-maze-1.0.3/memory_maze/oracle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-20 07:22:46.000000 memory-maze-1.0.3/memory_maze/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-06-20 07:22:46.000000 memory-maze-1.0.3/memory_maze/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:23:00.279494 memory-maze-1.0.3/memory_maze.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13416 2023-06-20 07:23:00.000000 memory-maze-1.0.3/memory_maze.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-20 07:23:00.000000 memory-maze-1.0.3/memory_maze.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 07:23:00.000000 memory-maze-1.0.3/memory_maze.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 07:23:00.000000 memory-maze-1.0.3/memory_maze.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-20 07:23:00.000000 memory-maze-1.0.3/memory_maze.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-20 07:23:00.000000 memory-maze-1.0.3/memory_maze.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 07:23:00.279494 memory-maze-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-20 07:22:46.000000 memory-maze-1.0.3/setup.py
```

### Comparing `memory-maze-1.0.2/LICENSE` & `memory-maze-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `memory-maze-1.0.2/PKG-INFO` & `memory-maze-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memory-maze
-Version: 1.0.2
+Version: 1.0.3
 Summary: Memory Maze is an environment to benchmark memory abilities of RL agents
 Home-page: https://github.com/jurgisp/memory-maze
 Author: Jurgis Pasukonis
 Author-email: jurgisp@gmail.com
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -95,20 +95,25 @@
 
 You can create the environment using the [Gym](https://github.com/openai/gym) interface:
 
 ```python
 !pip install gym
 import gym
 
+# Set this if you are getting "Unable to load EGL library" error:
+#  os.environ['MUJOCO_GL'] = 'glfw'  
+
 env = gym.make('memory_maze:MemoryMaze-9x9-v0')
 env = gym.make('memory_maze:MemoryMaze-11x11-v0')
 env = gym.make('memory_maze:MemoryMaze-13x13-v0')
 env = gym.make('memory_maze:MemoryMaze-15x15-v0')
 ```
 
+**Troubleshooting:** if you are getting "Unable to load EGL library error", that is because we enable MuJoCo headless GPU rendering (`MUJOCO_GL=egl`) by default. If you are testing locally on your machine, you can enable windowed rendering instead (`MUJOCO_GL=glfw`). [Read here](https://github.com/deepmind/dm_control#rendering) about the different rendering options. 
+
 The default environment has 64x64 image observations:
 
 ```python
 >>> env.observation_space
 Box(0, 255, (64, 64, 3), uint8)
 ```
 
@@ -172,15 +177,15 @@
     control_freq=4.0,
     discrete_actions=True,
 )
 ```
 
 ## Offline Dataset
 
-[**Dataset download here** (~100GB per dataset)](https://www.dropbox.com/sh/c38sc5h7ltgyyzc/AAARVeKgnyaoBLGdYYVABh_Ja)
+[**Dataset download here** (~100GB per dataset)](https://drive.google.com/drive/folders/1RcnkTZVwEHnAQeEuw7X8Y1RPSmrFLDFB)
 
 We provide two datasets of experience collected from the Memory Maze environment: Memory Maze 9x9 (30M) and Memory Maze 15x15 (30M). Each dataset contains 30 thousand trajectories from Memory Maze 9x9 and 15x15 environments respectively, split into 29k trajectories for training and 1k for evaluation. All trajectories are 1000 steps long, so each dataset has 30M steps total.
 
 The data is generated with a scripted policy that navigates to randomly chosen points in the maze under action noise. This choice of policy was made to generate diverse trajectories that explore the maze effectively and that form spatial loops, which can be important for learning long-term memory. We intentionally avoid recording data with a trained agent to ensure a diverse data distribution and to avoid dataset bias that could favor some methods over others. Because of this, the rewards are quite sparse in the data, occurring on average 1-2 times per trajectory.
 
 Each trajectory is saved as an NPZ file with the following entries available:
```

### Comparing `memory-maze-1.0.2/README.md` & `memory-maze-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -84,20 +84,25 @@
 
 You can create the environment using the [Gym](https://github.com/openai/gym) interface:
 
 ```python
 !pip install gym
 import gym
 
+# Set this if you are getting "Unable to load EGL library" error:
+#  os.environ['MUJOCO_GL'] = 'glfw'  
+
 env = gym.make('memory_maze:MemoryMaze-9x9-v0')
 env = gym.make('memory_maze:MemoryMaze-11x11-v0')
 env = gym.make('memory_maze:MemoryMaze-13x13-v0')
 env = gym.make('memory_maze:MemoryMaze-15x15-v0')
 ```
 
+**Troubleshooting:** if you are getting "Unable to load EGL library error", that is because we enable MuJoCo headless GPU rendering (`MUJOCO_GL=egl`) by default. If you are testing locally on your machine, you can enable windowed rendering instead (`MUJOCO_GL=glfw`). [Read here](https://github.com/deepmind/dm_control#rendering) about the different rendering options. 
+
 The default environment has 64x64 image observations:
 
 ```python
 >>> env.observation_space
 Box(0, 255, (64, 64, 3), uint8)
 ```
 
@@ -161,15 +166,15 @@
     control_freq=4.0,
     discrete_actions=True,
 )
 ```
 
 ## Offline Dataset
 
-[**Dataset download here** (~100GB per dataset)](https://www.dropbox.com/sh/c38sc5h7ltgyyzc/AAARVeKgnyaoBLGdYYVABh_Ja)
+[**Dataset download here** (~100GB per dataset)](https://drive.google.com/drive/folders/1RcnkTZVwEHnAQeEuw7X8Y1RPSmrFLDFB)
 
 We provide two datasets of experience collected from the Memory Maze environment: Memory Maze 9x9 (30M) and Memory Maze 15x15 (30M). Each dataset contains 30 thousand trajectories from Memory Maze 9x9 and 15x15 environments respectively, split into 29k trajectories for training and 1k for evaluation. All trajectories are 1000 steps long, so each dataset has 30M steps total.
 
 The data is generated with a scripted policy that navigates to randomly chosen points in the maze under action noise. This choice of policy was made to generate diverse trajectories that explore the maze effectively and that form spatial loops, which can be important for learning long-term memory. We intentionally avoid recording data with a trained agent to ensure a diverse data distribution and to avoid dataset bias that could favor some methods over others. Because of this, the rewards are quite sparse in the data, occurring on average 1-2 times per trajectory.
 
 Each trajectory is saved as an NPZ file with the following entries available:
```

### Comparing `memory-maze-1.0.2/memory_maze/__init__.py` & `memory-maze-1.0.3/memory_maze/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -48,11 +48,17 @@
         register(id=f'MemoryMaze-{key}-Oracle-ExtraObs-v0', entry_point=f(_make_gym_env, dm_task, global_observables=True, show_path=True))
         
         # High control frequency
         register(id=f'MemoryMaze-{key}-HiFreq-v0', entry_point=f(_make_gym_env, dm_task, image_only_obs=True, control_freq=40))
         register(id=f'MemoryMaze-{key}-HiFreq-Vis-v0', entry_point=f(_make_gym_env, dm_task, image_only_obs=True, control_freq=40, good_visibility=True))
         register(id=f'MemoryMaze-{key}-HiFreq-HD-v0', entry_point=f(_make_gym_env, dm_task, image_only_obs=True, control_freq=40, camera_resolution=256))
 
+        # Six colors even for smaller mazes
+        register(id=f'MemoryMaze-{key}-6CL-v0', entry_point=f(_make_gym_env, dm_task, randomize_colors=True, image_only_obs=True))
+        register(id=f'MemoryMaze-{key}-6CL-Top-v0', entry_point=f(_make_gym_env, dm_task, randomize_colors=True, image_only_obs=True, camera_resolution=256, top_camera=True))
+        register(id=f'MemoryMaze-{key}-6CL-ExtraObs-v0', entry_point=f(_make_gym_env, dm_task, randomize_colors=True, global_observables=True))
+        
+
 
 except ImportError:
     print('memory_maze: gym environments not registered.')
     raise
```

### Comparing `memory-maze-1.0.2/memory_maze/gym_wrappers.py` & `memory-maze-1.0.3/memory_maze/gym_wrappers.py`

 * *Files identical despite different names*

### Comparing `memory-maze-1.0.2/memory_maze/maze.py` & `memory-maze-1.0.3/memory_maze/maze.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Optional
 import functools
 import string
 
 import labmaze
 import numpy as np
 from dm_control import mjcf
 from dm_control.composer.observation import observable as observable_lib
@@ -41,14 +42,15 @@
     def __init__(self,
                  walker,
                  maze_arena,
                  n_targets=3,
                  target_radius=0.3,
                  target_height_above_ground=0.0,
                  target_reward_scale=1.0,
+                 target_randomize_colors=False,
                  enable_global_task_observables=False,
                  camera_resolution=64,
                  physics_timestep=DEFAULT_PHYSICS_TIMESTEP,
                  control_timestep=DEFAULT_CONTROL_TIMESTEP,
                  ):
         super().__init__(
             walker=walker,
@@ -56,56 +58,53 @@
             randomize_spawn_position=True,
             randomize_spawn_rotation=True,
             contact_termination=False,
             enable_global_task_observables=enable_global_task_observables,
             physics_timestep=physics_timestep,
             control_timestep=control_timestep
         )
+        self.n_targets = n_targets
+        self._target_radius = target_radius
+        self._target_height_above_ground = target_height_above_ground
         self._target_reward_scale = target_reward_scale
+        self._target_randomize_colors = target_randomize_colors
+
         self._targets = []
-        for i in range(n_targets):
-            color = TARGET_COLORS[i]
-            target = target_sphere.TargetSphere(
-                radius=target_radius,
-                height_above_ground=target_radius + target_height_above_ground,
-                rgb1=tuple(color * 1.0),
-                rgb2=tuple(color * 1.0),
-            )
-            self._targets.append(target)
-            self._maze_arena.attach(target)
+        self._target_colors = list(TARGET_COLORS)  # This contains all colors, not only n_targets
+        self._create_targets()
         self._current_target_ix = 0
         self._rewarded_this_step = False
         self._targets_obtained = 0
 
         if enable_global_task_observables:
             # Add egocentric vectors to targets
             xpos_origin_callable = lambda phys: phys.bind(walker.root_body).xpos
 
-            def _target_pos(physics, target):
-                return physics.bind(target.geom).xpos
+            def _target_pos(physics, targets, index):
+                return physics.bind(targets[index].geom).xpos
 
             for i in range(n_targets):
                 # Absolute target position
                 walker.observables.add_observable(
                     f'target_abs_{i}',
-                    observable_lib.Generic(functools.partial(_target_pos, target=self._targets[i])),
+                    observable_lib.Generic(functools.partial(_target_pos, targets=self._targets, index=i)),
                 )
                 # Relative target position
                 walker.observables.add_egocentric_vector(
                     f'target_rel_{i}',
-                    observable_lib.Generic(functools.partial(_target_pos, target=self._targets[i])),
+                    observable_lib.Generic(functools.partial(_target_pos, targets=self._targets, index=i)),
                     origin_callable=xpos_origin_callable)
 
         self._task_observables = super().task_observables
 
         def _current_target_index(_):
             return self._current_target_ix
 
         def _current_target_color(_):
-            return TARGET_COLORS[self._current_target_ix]
+            return self._target_colors[self._current_target_ix]
 
         self._task_observables['target_index'] = observable_lib.Generic(_current_target_index)
         self._task_observables['target_index'].enabled = True
         self._task_observables['target_color'] = observable_lib.Generic(_current_target_color)
         self._task_observables['target_color'].enabled = True
 
         self._walker.observables.egocentric_camera.height = camera_resolution
@@ -118,20 +117,23 @@
         return self._task_observables
 
     @property
     def name(self):
         return 'memory_maze'
 
     def initialize_episode_mjcf(self, rng: RandomState):
-        super().initialize_episode_mjcf(rng)
+        self._maze_arena.regenerate(rng)  # Bypass super()._initialize_episode_mjcf(), because it ignores rng
         while True:
+            if self._target_randomize_colors:
+                # Recreate target objects with new colors
+                self._create_targets(clear_existing=True, randomize_colors=True, rng=rng)
             ok = self._place_targets(rng)
             if not ok:
                 # Could not place targets - regenerate the maze
-                self._maze_arena.regenerate()
+                self._maze_arena.regenerate(rng)
                 continue
             break
         self._pick_new_target(rng)
 
     def initialize_episode(self, physics, rng: RandomState):
         super().initialize_episode(physics, rng)
         self._rewarded_this_step = False
@@ -152,14 +154,37 @@
         return super().should_terminate_episode(physics)
 
     def get_reward(self, physics):
         if self._rewarded_this_step:
             return self._target_reward_scale
         return 0.0
 
+    def _create_targets(self, clear_existing=False, randomize_colors=False, rng: Optional[RandomState] = None):
+        if clear_existing:
+            while self._targets:
+                target = self._targets.pop()
+                target.detach()  # Important to detach old targets, if creating new ones
+        else:
+            assert not self._targets, 'Targets already created.'
+
+        if randomize_colors:
+            assert rng is not None
+            rng.shuffle(self._target_colors)
+
+        for i in range(self.n_targets):
+            color = self._target_colors[i]
+            target = target_sphere.TargetSphere(
+                radius=self._target_radius,
+                height_above_ground=self._target_radius + self._target_height_above_ground,
+                rgb1=tuple(color * 1.0),
+                rgb2=tuple(color * 1.0),
+            )
+            self._targets.append(target)
+            self._maze_arena.attach(target)
+
     def _place_targets(self, rng: RandomState) -> bool:
         possible_positions = list(self._maze_arena.target_positions)
         rng.shuffle(possible_positions)
         if len(possible_positions) < len(self._targets):
             # Too few rooms - need to regenerate the maze
             return False
         for target, pos in zip(self._targets, possible_positions):
@@ -223,16 +248,17 @@
                targets_per_room=0,
                max_variations=26,
                simplify=True,
                skybox_texture=None,
                wall_textures=None,
                floor_textures=None,
                aesthetic='default',
-               name='random_maze'):
-        random_seed = np.random.randint(2147483648)
+               name='random_maze',
+               random_seed=None):
+        assert random_seed, "Expected to be set by tasks._memory_maze()"
         super()._build(
             maze=TextMazeVaryingWalls(
                 height=y_cells,
                 width=x_cells,
                 max_rooms=max_rooms,
                 room_min_size=room_min_size,
                 room_max_size=room_max_size,
@@ -245,14 +271,48 @@
             z_height=z_height,
             skybox_texture=skybox_texture,
             wall_textures=wall_textures,
             floor_textures=floor_textures,
             aesthetic=aesthetic,
             name=name)
 
+    def regenerate(self, random_state):
+        """Generates a new maze layout.
+
+        Patch of MazeWithTargets.regenerate() which uses random_state.
+        """
+        self._maze.regenerate()
+        # logging.debug('GENERATED MAZE:\n%s', self._maze.entity_layer)
+        self._find_spawn_and_target_positions()
+
+        if self._text_maze_regenerated_hook:
+            self._text_maze_regenerated_hook()
+
+        # Remove old texturing planes.
+        for geom_name in self._texturing_geom_names:
+            del self._mjcf_root.worldbody.geom[geom_name]
+        self._texturing_geom_names = []
+
+        # Remove old texturing materials.
+        for material_name in self._texturing_material_names:
+            del self._mjcf_root.asset.material[material_name]
+        self._texturing_material_names = []
+
+        # Remove old actual-wall geoms.
+        self._maze_body.geom.clear()
+
+        self._current_wall_texture = {
+            wall_char: random_state.choice(wall_textures)  # PATCH: use random_state for wall textures
+            for wall_char, wall_textures in self._wall_textures.items()
+        }
+
+        for wall_char in self._wall_textures:
+            self._make_wall_geoms(wall_char)
+        self._make_floor_variations()
+
     def _make_floor_variations(self, build_tile_geoms_fn=None):
         """Fork of mazes.MazeWithTargets._make_floor_variations().
 
         Makes the room floors different if possible, instead of sampling randomly.
         """
         _DEFAULT_FLOOR_CHAR = '.'
```

### Comparing `memory-maze-1.0.2/memory_maze/oracle.py` & `memory-maze-1.0.3/memory_maze/oracle.py`

 * *Files identical despite different names*

### Comparing `memory-maze-1.0.2/memory_maze/tasks.py` & `memory-maze-1.0.3/memory_maze/tasks.py`

 * *Files 7% similar despite different names*

```diff
@@ -59,16 +59,18 @@
     image_only_obs=False,
     target_color_in_image=True,
     global_observables=False,
     top_camera=False,
     good_visibility=False,
     show_path=False,
     camera_resolution=64,
-    random_state=None,
+    seed=None,
+    randomize_colors=False,
 ):
+    random_state = np.random.RandomState(seed)
     walker = RollingBallWithFriction(camera_height=0.3, add_ears=top_camera)
     arena = MazeWithTargetsArena(
         x_cells=maze_size + 2,  # inner size => outer size
         y_cells=maze_size + 2,
         xy_scale=2.0,
         z_height=1.5 if not good_visibility else 0.4,
         max_rooms=max_rooms,
@@ -78,25 +80,27 @@
         targets_per_room=1,
         floor_textures=FixedFloorTexture('style_01', ['blue', 'blue_bright']),
         wall_textures=dict({
             '*': FixedWallTexture('style_01', 'yellow'),  # default wall
         }, **{str(i): labmaze_textures.WallTextures('style_01') for i in range(10)}  # variations
         ),
         skybox_texture=None,
+        random_seed=random_state.randint(2147483648),
     )
 
     task = MemoryMazeTask(
         walker=walker,
         maze_arena=arena,
         n_targets=n_targets,
         target_radius=0.6,
         target_height_above_ground=0.5 if good_visibility else -0.6,
         enable_global_task_observables=True,  # Always add to underlying env, but not always expose in RemapObservationWrapper
         control_timestep=1.0 / control_freq,
         camera_resolution=camera_resolution,
+        target_randomize_colors=randomize_colors,
     )
 
     if top_camera:
         task.observables['top_camera'].enabled = True
 
     env = composer.Environment(
         time_limit=time_limit - 1e-3,  # subtract epsilon to make sure ep_length=time_limit*fps
```

### Comparing `memory-maze-1.0.2/memory_maze/wrappers.py` & `memory-maze-1.0.3/memory_maze/wrappers.py`

 * *Files identical despite different names*

### Comparing `memory-maze-1.0.2/memory_maze.egg-info/PKG-INFO` & `memory-maze-1.0.3/memory_maze.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memory-maze
-Version: 1.0.2
+Version: 1.0.3
 Summary: Memory Maze is an environment to benchmark memory abilities of RL agents
 Home-page: https://github.com/jurgisp/memory-maze
 Author: Jurgis Pasukonis
 Author-email: jurgisp@gmail.com
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -95,20 +95,25 @@
 
 You can create the environment using the [Gym](https://github.com/openai/gym) interface:
 
 ```python
 !pip install gym
 import gym
 
+# Set this if you are getting "Unable to load EGL library" error:
+#  os.environ['MUJOCO_GL'] = 'glfw'  
+
 env = gym.make('memory_maze:MemoryMaze-9x9-v0')
 env = gym.make('memory_maze:MemoryMaze-11x11-v0')
 env = gym.make('memory_maze:MemoryMaze-13x13-v0')
 env = gym.make('memory_maze:MemoryMaze-15x15-v0')
 ```
 
+**Troubleshooting:** if you are getting "Unable to load EGL library error", that is because we enable MuJoCo headless GPU rendering (`MUJOCO_GL=egl`) by default. If you are testing locally on your machine, you can enable windowed rendering instead (`MUJOCO_GL=glfw`). [Read here](https://github.com/deepmind/dm_control#rendering) about the different rendering options. 
+
 The default environment has 64x64 image observations:
 
 ```python
 >>> env.observation_space
 Box(0, 255, (64, 64, 3), uint8)
 ```
 
@@ -172,15 +177,15 @@
     control_freq=4.0,
     discrete_actions=True,
 )
 ```
 
 ## Offline Dataset
 
-[**Dataset download here** (~100GB per dataset)](https://www.dropbox.com/sh/c38sc5h7ltgyyzc/AAARVeKgnyaoBLGdYYVABh_Ja)
+[**Dataset download here** (~100GB per dataset)](https://drive.google.com/drive/folders/1RcnkTZVwEHnAQeEuw7X8Y1RPSmrFLDFB)
 
 We provide two datasets of experience collected from the Memory Maze environment: Memory Maze 9x9 (30M) and Memory Maze 15x15 (30M). Each dataset contains 30 thousand trajectories from Memory Maze 9x9 and 15x15 environments respectively, split into 29k trajectories for training and 1k for evaluation. All trajectories are 1000 steps long, so each dataset has 30M steps total.
 
 The data is generated with a scripted policy that navigates to randomly chosen points in the maze under action noise. This choice of policy was made to generate diverse trajectories that explore the maze effectively and that form spatial loops, which can be important for learning long-term memory. We intentionally avoid recording data with a trained agent to ensure a diverse data distribution and to avoid dataset bias that could favor some methods over others. Because of this, the rewards are quite sparse in the data, occurring on average 1-2 times per trajectory.
 
 Each trajectory is saved as an NPZ file with the following entries available:
```

### Comparing `memory-maze-1.0.2/setup.py` & `memory-maze-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import pathlib
 
-__version__ = "1.0.2"
+__version__ = "1.0.3"
 
 setup(
     name="memory-maze",
     version=__version__,
     author="Jurgis Pasukonis",
     author_email="jurgisp@gmail.com",
     url="https://github.com/jurgisp/memory-maze",
```

