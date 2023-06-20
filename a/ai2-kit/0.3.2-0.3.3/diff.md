# Comparing `tmp/ai2_kit-0.3.2.tar.gz` & `tmp/ai2_kit-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai2_kit-0.3.2.tar", max compression
+gzip compressed data, was "ai2_kit-0.3.3.tar", max compression
```

## Comparing `ai2_kit-0.3.2.tar` & `ai2_kit-0.3.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1067 2023-02-07 08:30:11.900671 ai2_kit-0.3.2/LICENSE
--rw-r--r--   0        0        0     1205 2023-06-16 03:38:14.969789 ai2_kit-0.3.2/README.md
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.2/ai2_kit/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 03:47:09.348444 ai2_kit-0.3.2/ai2_kit/algorithm/__init__.py
--rw-r--r--   0        0        0    12100 2023-06-13 03:47:09.348444 ai2_kit-0.3.2/ai2_kit/algorithm/proton_transfer.py
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.2/ai2_kit/core/__init__.py
--rw-r--r--   0        0        0     1884 2023-03-22 04:23:44.538179 ai2_kit-0.3.2/ai2_kit/core/artifact.py
--rw-r--r--   0        0        0     3327 2023-03-22 04:23:44.538179 ai2_kit-0.3.2/ai2_kit/core/checkpoint.py
--rw-r--r--   0        0        0      169 2023-06-13 03:47:09.348444 ai2_kit-0.3.2/ai2_kit/core/cmd.py
--rw-r--r--   0        0        0     5766 2023-02-06 09:01:27.000000 ai2_kit-0.3.2/ai2_kit/core/connector.py
--rw-r--r--   0        0        0     7989 2023-06-20 06:47:09.893237 ai2_kit-0.3.2/ai2_kit/core/executor.py
--rw-r--r--   0        0        0     1090 2023-06-20 06:39:10.182460 ai2_kit-0.3.2/ai2_kit/core/future.py
--rw-r--r--   0        0        0     3655 2023-06-20 06:39:10.182460 ai2_kit-0.3.2/ai2_kit/core/job.py
--rw-r--r--   0        0        0      298 2023-06-20 06:39:10.182460 ai2_kit-0.3.2/ai2_kit/core/log.py
--rw-r--r--   0        0        0     8823 2023-06-20 06:39:10.182460 ai2_kit-0.3.2/ai2_kit/core/queue_system.py
--rw-r--r--   0        0        0     2315 2023-03-22 04:23:44.538179 ai2_kit-0.3.2/ai2_kit/core/resource_manager.py
--rw-r--r--   0        0        0     2358 2023-06-19 08:54:25.567391 ai2_kit-0.3.2/ai2_kit/core/script.py
--rw-r--r--   0        0        0     2524 2023-06-20 06:39:10.182460 ai2_kit-0.3.2/ai2_kit/core/util.py
--rw-r--r--   0        0        0        0 2023-06-13 03:47:09.348444 ai2_kit-0.3.2/ai2_kit/dflow/__init__.py
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.2/ai2_kit/domain/__init__.py
--rw-r--r--   0        0        0     1580 2023-06-20 06:39:10.182460 ai2_kit-0.3.2/ai2_kit/domain/cll.py
--rw-r--r--   0        0        0      341 2023-02-27 08:58:57.520622 ai2_kit-0.3.2/ai2_kit/domain/constant.py
--rw-r--r--   0        0        0     7929 2023-06-20 06:39:10.182460 ai2_kit-0.3.2/ai2_kit/domain/cp2k.py
--rw-r--r--   0        0        0     4129 2023-06-20 06:39:10.182460 ai2_kit-0.3.2/ai2_kit/domain/data_helper.py
--rw-r--r--   0        0        0     6765 2023-06-20 06:39:10.182460 ai2_kit-0.3.2/ai2_kit/domain/deepmd.py
--rw-r--r--   0        0        0    15672 2023-06-20 06:39:10.182460 ai2_kit-0.3.2/ai2_kit/domain/lammps.py
--rw-r--r--   0        0        0     3134 2023-06-20 06:39:10.182460 ai2_kit-0.3.2/ai2_kit/domain/selector.py
--rw-r--r--   0        0        0      183 2023-03-22 04:23:44.538179 ai2_kit-0.3.2/ai2_kit/domain/updater.py
--rw-r--r--   0        0        0     1465 2023-06-16 03:38:14.969789 ai2_kit-0.3.2/ai2_kit/main.py
--rw-r--r--   0        0        0        0 2023-06-16 03:38:14.969789 ai2_kit-0.3.2/ai2_kit/tool/__init__.py
--rw-r--r--   0        0        0      748 2023-06-20 06:39:10.182460 ai2_kit-0.3.2/ai2_kit/tool/ase.py
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.2/ai2_kit/workflow/__init__.py
--rw-r--r--   0        0        0     7426 2023-06-15 09:06:34.322595 ai2_kit-0.3.2/ai2_kit/workflow/cll_mlp.py
--rw-r--r--   0        0        0     8519 2023-06-16 03:38:14.969789 ai2_kit-0.3.2/ai2_kit/workflow/fep_mlp.py
--rw-r--r--   0        0        0      843 2023-06-20 06:47:52.262405 ai2_kit-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     2232 1970-01-01 00:00:00.000000 ai2_kit-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-02-07 08:30:11.900671 ai2_kit-0.3.3/LICENSE
+-rw-r--r--   0        0        0     1205 2023-06-16 03:38:14.969789 ai2_kit-0.3.3/README.md
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.3/ai2_kit/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 03:47:09.348444 ai2_kit-0.3.3/ai2_kit/algorithm/__init__.py
+-rw-r--r--   0        0        0    12100 2023-06-13 03:47:09.348444 ai2_kit-0.3.3/ai2_kit/algorithm/proton_transfer.py
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.3/ai2_kit/core/__init__.py
+-rw-r--r--   0        0        0     1884 2023-03-22 04:23:44.538179 ai2_kit-0.3.3/ai2_kit/core/artifact.py
+-rw-r--r--   0        0        0     3327 2023-03-22 04:23:44.538179 ai2_kit-0.3.3/ai2_kit/core/checkpoint.py
+-rw-r--r--   0        0        0      169 2023-06-13 03:47:09.348444 ai2_kit-0.3.3/ai2_kit/core/cmd.py
+-rw-r--r--   0        0        0     5766 2023-02-06 09:01:27.000000 ai2_kit-0.3.3/ai2_kit/core/connector.py
+-rw-r--r--   0        0        0     8008 2023-06-20 08:38:04.462450 ai2_kit-0.3.3/ai2_kit/core/executor.py
+-rw-r--r--   0        0        0      386 2023-06-20 08:38:04.462450 ai2_kit-0.3.3/ai2_kit/core/future.py
+-rw-r--r--   0        0        0     1945 2023-06-20 08:38:04.462450 ai2_kit-0.3.3/ai2_kit/core/job.py
+-rw-r--r--   0        0        0      298 2023-06-20 06:39:10.182460 ai2_kit-0.3.3/ai2_kit/core/log.py
+-rw-r--r--   0        0        0     8823 2023-06-20 08:37:58.363284 ai2_kit-0.3.3/ai2_kit/core/queue_system.py
+-rw-r--r--   0        0        0     2315 2023-03-22 04:23:44.538179 ai2_kit-0.3.3/ai2_kit/core/resource_manager.py
+-rw-r--r--   0        0        0     2358 2023-06-19 08:54:25.567391 ai2_kit-0.3.3/ai2_kit/core/script.py
+-rw-r--r--   0        0        0     2641 2023-06-20 08:38:04.462450 ai2_kit-0.3.3/ai2_kit/core/util.py
+-rw-r--r--   0        0        0        0 2023-06-13 03:47:09.348444 ai2_kit-0.3.3/ai2_kit/dflow/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.3/ai2_kit/domain/__init__.py
+-rw-r--r--   0        0        0     1580 2023-06-20 06:39:10.182460 ai2_kit-0.3.3/ai2_kit/domain/cll.py
+-rw-r--r--   0        0        0      341 2023-02-27 08:58:57.520622 ai2_kit-0.3.3/ai2_kit/domain/constant.py
+-rw-r--r--   0        0        0     7660 2023-06-20 08:38:04.462450 ai2_kit-0.3.3/ai2_kit/domain/cp2k.py
+-rw-r--r--   0        0        0     4129 2023-06-20 06:39:10.182460 ai2_kit-0.3.3/ai2_kit/domain/data_helper.py
+-rw-r--r--   0        0        0     6625 2023-06-20 08:38:04.473284 ai2_kit-0.3.3/ai2_kit/domain/deepmd.py
+-rw-r--r--   0        0        0    15452 2023-06-20 08:38:04.473284 ai2_kit-0.3.3/ai2_kit/domain/lammps.py
+-rw-r--r--   0        0        0     3039 2023-06-20 08:38:04.473284 ai2_kit-0.3.3/ai2_kit/domain/selector.py
+-rw-r--r--   0        0        0      183 2023-03-22 04:23:44.538179 ai2_kit-0.3.3/ai2_kit/domain/updater.py
+-rw-r--r--   0        0        0     1461 2023-06-20 08:38:04.473284 ai2_kit-0.3.3/ai2_kit/main.py
+-rw-r--r--   0        0        0        0 2023-06-16 03:38:14.969789 ai2_kit-0.3.3/ai2_kit/tool/__init__.py
+-rw-r--r--   0        0        0      748 2023-06-20 06:39:10.182460 ai2_kit-0.3.3/ai2_kit/tool/ase.py
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.3/ai2_kit/workflow/__init__.py
+-rw-r--r--   0        0        0     7657 2023-06-20 08:38:04.473284 ai2_kit-0.3.3/ai2_kit/workflow/cll_mlp.py
+-rw-r--r--   0        0        0     8490 2023-06-20 08:38:04.473284 ai2_kit-0.3.3/ai2_kit/workflow/fep_mlp.py
+-rw-r--r--   0        0        0      843 2023-06-20 08:40:09.338269 ai2_kit-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     2232 1970-01-01 00:00:00.000000 ai2_kit-0.3.3/PKG-INFO
```

### Comparing `ai2_kit-0.3.2/LICENSE` & `ai2_kit-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.2/README.md` & `ai2_kit-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.2/ai2_kit/algorithm/proton_transfer.py` & `ai2_kit-0.3.3/ai2_kit/algorithm/proton_transfer.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.2/ai2_kit/core/artifact.py` & `ai2_kit-0.3.3/ai2_kit/core/artifact.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.2/ai2_kit/core/checkpoint.py` & `ai2_kit-0.3.3/ai2_kit/core/checkpoint.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.2/ai2_kit/core/connector.py` & `ai2_kit-0.3.3/ai2_kit/core/connector.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.2/ai2_kit/core/executor.py` & `ai2_kit-0.3.3/ai2_kit/core/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,16 @@
         self.python_cmd = python_cmd
         self.tmp_dir = os.path.join(self.work_dir, '.tmp')  # TODO: make it configurable
 
     def init(self):
         # if work_dir is relative path, it will be relative to user home
         if not os.path.isabs(self.work_dir):
             user_home = self.run('echo $HOME', hide=True).stdout.strip()
-            self.work_dir = os.path.join(user_home, self.work_dir)
+            self.work_dir = os.path.normpath(os.path.join(user_home, self.work_dir))
+
         self.mkdir(self.work_dir)
         self.mkdir(self.tmp_dir)
 
     def mkdir(self, path: str):
         return self.connector.run('mkdir -p {}'.format(shlex.quote(path)))
 
     def dump_text(self, text: str, path: str):
```

### Comparing `ai2_kit-0.3.2/ai2_kit/core/queue_system.py` & `ai2_kit-0.3.3/ai2_kit/core/queue_system.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.2/ai2_kit/core/resource_manager.py` & `ai2_kit-0.3.3/ai2_kit/core/resource_manager.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.2/ai2_kit/core/script.py` & `ai2_kit-0.3.3/ai2_kit/core/script.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.2/ai2_kit/core/util.py` & `ai2_kit-0.3.3/ai2_kit/core/util.py`

 * *Files 9% similar despite different names*

```diff
@@ -84,10 +84,13 @@
 T = TypeVar('T')
 def flatten(l: List[List[T]]) -> List[T]:
     return [item for sublist in l for item in sublist]
 
 def format_env_string(s: str) -> str:
     return s.format(**os.environ)
 
+
 def split_list(l: List[T], n: int) -> List[List[T]]:
-    """split a list into n chunks, the last chunk may be smaller than others"""
-    return [l[i:i + n] for i in range(0, len(l), n)]
+    """split list into n chunks"""
+    # ref: https://stackoverflow.com/questions/2130016/splitting-a-list-into-n-parts-of-approximately-equal-length
+    k, m = divmod(len(l), n)
+    return [l[i*k+min(i, m) : (i+1)*k+min(i+1, m)] for i in range(n)]
```

### Comparing `ai2_kit-0.3.2/ai2_kit/domain/cll.py` & `ai2_kit-0.3.3/ai2_kit/domain/cll.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.2/ai2_kit/domain/cp2k.py` & `ai2_kit-0.3.3/ai2_kit/domain/cp2k.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 from ai2_kit.core.artifact import Artifact
 from ai2_kit.core.script import BashScript, BashStep, BashTemplate
-from ai2_kit.core.job import GatherJobsFuture, retry_fn
-
-from ai2_kit.core.future import DummyFuture, IFuture, map_future
-
-from ai2_kit.core.util import merge_dict, parse_cp2k_input, dict_nested_get, dict_nested_set
+from ai2_kit.core.job import gather_jobs
+from ai2_kit.core.util import merge_dict, parse_cp2k_input, dict_nested_get, dict_nested_set, split_list
 from ai2_kit.core.log import get_logger
 
 from typing import List, Union
 from pydantic import BaseModel
 from dataclasses import dataclass
 
 import copy
@@ -55,16 +52,15 @@
 class GenericCp2kOutput(ICllLabelOutput):
     cp2k_outputs: List[Artifact]
 
     def get_labeled_system_dataset(self):
         return self.cp2k_outputs
 
 
-def generic_cp2k(input: GenericCp2kInput, ctx: GenericCp2kContext) -> IFuture[GenericCp2kOutput]:
-
+async def generic_cp2k(input: GenericCp2kInput, ctx: GenericCp2kContext) -> GenericCp2kOutput:
     executor = ctx.resource_manager.default_executor
 
     # For the first round
     if not input.initiated:
         input.system_files += ctx.resource_manager.get_artifacts(input.config.init_system_files)
 
     # setup workspace
@@ -120,50 +116,45 @@
             type_map=input.type_map,
             base_dir=tasks_dir,
             input_template=input_template,
             limit=input.config.limit,
         )
     else:
         logger.warn('no available candidates, skip')
-        return DummyFuture(GenericCp2kOutput(cp2k_outputs=[]))
+        return GenericCp2kOutput(cp2k_outputs=[])
 
-    # group cp2k tasks by concurrency
-    concurrency = ctx.config.concurrency
-    steps_group = [list() for _ in range(concurrency)]
-    for i, cp2k_task_dir in enumerate(cp2k_task_dirs):
-        steps = steps_group[i % concurrency]
-        step = BashStep(
+    # build commands
+    steps = []
+    for cp2k_task_dir in cp2k_task_dirs:
+        steps.append(BashStep(
             cwd=cp2k_task_dir,
             cmd=[ctx.config.cp2k_cmd, '-i input.inp 1>> output 2>> output'],
             checkpoint='cp2k',
-        )
-        steps.append(step)
+        ))
 
-    # run tasks
+    # submit tasks and wait for completion
     jobs = []
-    for steps in steps_group:
-        if not steps:
+    for steps_group in split_list(steps, ctx.config.concurrency):
+        if not steps_group:
             continue
         script = BashScript(
             template=ctx.config.script_template,
-            steps=steps,
+            steps=steps_group,
         )
-        job = executor.submit(script.render(), cwd=tasks_dir)
-        jobs.append(job)
-
-    future = GatherJobsFuture(jobs, done_fn=retry_fn(max_tries=2), raise_exception=True)
+        jobs.append(executor.submit(script.render(), cwd=tasks_dir))
+    jobs = await gather_jobs(jobs, max_tries=2)
 
     cp2k_outputs = [Artifact.of(
         url=url,
         format=Cp2kOutputHelper.format,
         executor=executor.name,
         attrs=dict(),  # TODO: success from input
     ) for url in cp2k_task_dirs]
 
-    return map_future(future, GenericCp2kOutput(cp2k_outputs=cp2k_outputs))
+    return GenericCp2kOutput(cp2k_outputs=cp2k_outputs)
 
 
 def __make_cp2k_task_dirs():
     def make_cp2k_task_dirs(lammps_dump_files: List[str],
                             xyz_files: List[str],
                             type_map: List[str],
                             input_template: dict,
```

### Comparing `ai2_kit-0.3.2/ai2_kit/domain/data_helper.py` & `ai2_kit-0.3.3/ai2_kit/domain/data_helper.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.2/ai2_kit/domain/deepmd.py` & `ai2_kit-0.3.3/ai2_kit/domain/deepmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from ai2_kit.core.artifact import Artifact
 from ai2_kit.core.script import BashTemplate
 from ai2_kit.core.script import BashScript, BashStep
-from ai2_kit.core.job import JobFuture, GatherJobsFuture, retry_fn
-from ai2_kit.core.future import map_future
+from ai2_kit.core.job import JobFuture, gather_jobs
 from ai2_kit.core.log import get_logger
 
 from pydantic import BaseModel
 from typing import List
 from dataclasses import dataclass
 import os
 import copy
 import random
 import sys
 import json
 
 from .cll import ICllTrainOutput, BaseCllContext
-from .data_helper import Cp2kOutputHelper, DeepmdNpyHelper, DeepmdModelHelper, convert_to_deepmd_npy
+from .data_helper import Cp2kOutputHelper, DeepmdNpyHelper, convert_to_deepmd_npy
 from .constant import (
     DP_CHECKPOINT_FILE,
     DP_DISP_FILE,
     DP_PROFILING_FILE,
     DP_INPUT_FILE,
     DP_FROZEN_MODEL,
 )
@@ -28,15 +27,14 @@
 
 
 class GenericDeepmdInputConfig(BaseModel):
     model_num: int = 4
     init_dataset: List[str]
     input_template: dict
 
-
 class GenericDeepmdContextConfig(BaseModel):
     script_template: BashTemplate
     dp_cmd: str = 'dp'
 
 
 @dataclass
 class GenericDeepmdInput:
@@ -61,15 +59,15 @@
 
     def get_mlp_models(self) -> List[Artifact]:
         return [a.join(DP_FROZEN_MODEL) for a in self.outputs]
 
     def get_training_dataset(self) -> List[Artifact]:
         return self.input.new_dataset + self.input.old_dataset
 
-def generic_deepmd(input: GenericDeepmdInput, ctx: GenericDeepmdContext):
+async def generic_deepmd(input: GenericDeepmdInput, ctx: GenericDeepmdContext):
     executor = ctx.resource_manager.default_executor
 
     # setup workspace
     work_dir = os.path.join(executor.work_dir, ctx.path_prefix)
     [converted_data_dir, tasks_dir] = executor.setup_workspace(work_dir, ['converted_input_data', 'tasks'])
 
     # initialization
@@ -178,18 +176,18 @@
         )
         output_dirs.append(task_dir)
 
         # submit job
         job = executor.submit(dp_train_script.render(), cwd=task_dir)
         jobs.append(job)
 
-    future = GatherJobsFuture(jobs, done_fn=retry_fn(max_tries=2), raise_exception=True)
+    await gather_jobs(jobs, max_tries=2)
 
-    return map_future(future, GenericDeepmdOutput(
+    return GenericDeepmdOutput(
         input=input,
         outputs=[Artifact.of(
             url=url,
         ) for url in output_dirs]
-    ))
+    )
 
 def _random_seed():
     return random.randrange(sys.maxsize) % (1 << 32)
```

### Comparing `ai2_kit-0.3.2/ai2_kit/domain/lammps.py` & `ai2_kit-0.3.3/ai2_kit/domain/lammps.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ai2_kit.core.script import BashTemplate, BashStep, BashScript
 from ai2_kit.core.artifact import Artifact
 from ai2_kit.core.log import get_logger
-from ai2_kit.core.job import GatherJobsFuture, retry_fn
-from ai2_kit.core.future import map_future
+from ai2_kit.core.job import gather_jobs
+from ai2_kit.core.util import split_list
 
 from typing import List, Literal, Optional, Union, Mapping, Sequence
 from pydantic import BaseModel
 from dataclasses import dataclass
 from string import Template
 from allpairspy import AllPairs
 import os
@@ -126,15 +126,15 @@
 class GenericLammpsOutput(ICllExploreOutput):
     model_devi_outputs: List[Artifact]
 
     def get_model_devi_dataset(self) -> List[Artifact]:
         return self.model_devi_outputs
 
 
-def generic_lammps(input: GenericLammpsInput, ctx: GenericLammpsContext):
+async def generic_lammps(input: GenericLammpsInput, ctx: GenericLammpsContext):
     executor = ctx.resource_manager.default_executor
 
     # setup workspace
     work_dir = os.path.join(executor.work_dir, ctx.path_prefix)
     input_data_dir, tasks_dir = executor.setup_workspace(work_dir, ['input_data', 'tasks'])
 
     systems = ctx.resource_manager.resolve_artifacts(input.config.system_files)
@@ -237,53 +237,47 @@
         lammps_task_dirs.append(lammps_task_dir)
 
     # build scripts and submit
     lammps_cmd = ctx.config.lammps_cmd
     base_cmd = f'{lammps_cmd} -i {lammps_input_file_name}'
     cmd = f'''if [ -f md.restart.* ]; then {base_cmd} -v restart 1; else {base_cmd} -v restart 0; fi'''
 
-    # group tasks by concurrency
-    concurrency = ctx.config.concurrency
-    steps_group = [ list() for _ in range(concurrency)]
-
-    for i, lammps_task_dir in enumerate(lammps_task_dirs):
-        steps = steps_group[i % concurrency]
-        step = BashStep(
+    # generate steps
+    steps = []
+    for lammps_task_dir in lammps_task_dirs:
+        steps.append(BashStep(
             cwd=lammps_task_dir,
             cmd=cmd,
             checkpoint='lammps',
-        )
-        steps.append(step)
+        ))
 
     # submit jobs
     jobs = []
-    for steps in steps_group:
-        if not steps:
+    for steps_group in split_list(steps, ctx.config.concurrency):
+        if not steps_group:
             continue
         script = BashScript(
             template=ctx.config.script_template,
-            steps=steps,
+            steps=steps_group,
         )
         job = executor.submit(script.render(), cwd=tasks_dir)
         jobs.append(job)
 
+    await gather_jobs(jobs, max_tries=2)
+
     outputs = [
         Artifact.of(
             url=task_dir,
             executor=executor.name,
             format=LammpsOutputHelper.format,
             attrs=dict(
             ),  # TODO: inherit from input file
         ) for task_dir in lammps_task_dirs]  # type: ignore
 
-    future = GatherJobsFuture(jobs, done_fn=retry_fn(max_tries=2), raise_exception=True)
-
-    return map_future(future, GenericLammpsOutput(
-        model_devi_outputs=outputs,
-    ))
+    return GenericLammpsOutput(model_devi_outputs=outputs)
 
 
 def make_md_force_field_section(models: List[str]):
     deepmd_args = ""
     settings = [
         'pair_style deepmd %s out_freq ${THERMO_FREQ} out_file %s %s' % (' '.join(models), MODEL_DEVI_OUT, deepmd_args),
         'pair_coeff * *',
```

### Comparing `ai2_kit-0.3.2/ai2_kit/domain/selector.py` & `ai2_kit-0.3.3/ai2_kit/domain/selector.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-from ai2_kit.core.executor import Executor
 from ai2_kit.core.artifact import Artifact
 from ai2_kit.core.log import get_logger
-from ai2_kit.core.future import DummyFuture
 
 from typing import List
 from io import StringIO
 from pydantic import BaseModel
 from dataclasses import dataclass
 import pandas as pd
 
@@ -40,15 +38,15 @@
     config: ThresholdSelectorInputConfig
     model_devi_data: List[Artifact]
     model_devi_out_filename: str
 
     def set_model_devi_dataset(self, data: List[Artifact]):
         self.model_devi_data = data
 
-def threshold_selector(input: ThresholdSelectorInput, ctx: ThresholdSelectorContext):
+async def threshold_selector(input: ThresholdSelectorInput, ctx: ThresholdSelectorContext):
     executor = ctx.resource_manager.default_executor
 
     f_trust_lo = input.config.f_trust_lo
     f_trust_hi = input.config.f_trust_hi
     col_force = 'avg_devi_f'
     logger.info('criteria: %f <= %s < %f ', f_trust_lo, col_force, f_trust_hi)
 
@@ -81,12 +79,11 @@
         candidate.attrs['passed']   = passed_df.step.tolist()
         candidate.attrs['selected'] = selected_df.step.tolist()
         candidate.attrs['rejected'] = rejected_df.step.tolist()
 
         total_count += len(df)
         passed_count += len(passed_df)
 
-
-    return DummyFuture(ThresholdSelectorOutput(
+    return ThresholdSelectorOutput(
         model_devi_data=input.model_devi_data,
         passing_rate=passed_count / total_count,
-    ))
+    )
```

### Comparing `ai2_kit-0.3.2/ai2_kit/main.py` & `ai2_kit-0.3.3/ai2_kit/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,21 +28,21 @@
         from ai2_kit.algorithm import proton_transfer
         return proton_transfer.detect_type_change
 
 
 class WorkflowGroup:
     @property
     def cll_mlp_training(self):
-        from ai2_kit.workflow.cll_mlp import cll_train_mlp
-        return cll_train_mlp
+        from ai2_kit.workflow.cll_mlp import run_workflow
+        return run_workflow
 
     @property
     def fep_mlp_training(self):
-        from ai2_kit.workflow.fep_mlp import fep_train_mlp
-        return fep_train_mlp
+        from ai2_kit.workflow.fep_mlp import run_workflow
+        return run_workflow
 
 class ToolGroup:
 
     @property
     def ase(self):
         from ai2_kit.tool.ase import AseHelper
         return AseHelper
```

### Comparing `ai2_kit-0.3.2/ai2_kit/tool/ase.py` & `ai2_kit-0.3.3/ai2_kit/tool/ase.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.2/ai2_kit/workflow/cll_mlp.py` & `ai2_kit-0.3.3/ai2_kit/workflow/cll_mlp.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     cll,
 )
 
 from pydantic import BaseModel
 from typing import Dict, List, Optional, Any
 from fire import Fire
 
+import asyncio
 import itertools
 import copy
 import os
 
 logger = get_logger(__name__)
 
 
@@ -73,43 +74,44 @@
 class CllWorkflowConfig(BaseModel):
 
     executors: Dict[str, CllWorkflowExecutorConfig]
     artifacts: ArtifactMap
     workflow: Any  # Keep it raw here, it should be parsed later in iteration
 
 
-def cll_train_mlp(*config_files, executor: Optional[str] = None, path_prefix: Optional[str] = None):
+def run_workflow(*config_files, executor: Optional[str] = None, path_prefix: Optional[str] = None):
     """
     Run Closed-Loop Learning (CLL) workflow to train Machine Learning Potential (MLP) models.
     """
-
     config_data = load_yaml_files(*config_files)
     config = CllWorkflowConfig.parse_obj(config_data)
 
     if executor not in config.executors:
         raise ValueError(f'executor {executor} is not found')
     if path_prefix is None:
         raise ValueError('path_prefix should not be empty')
 
     resource_manager = ResourceManager(
         executor_configs=config.executors,
         artifacts=config.artifacts,
         default_executor=executor,
     )
+    return asyncio.run(cll_mlp_training_workflow(config, resource_manager, executor, path_prefix))
+
 
+async def cll_mlp_training_workflow(config: CllWorkflowConfig, resource_manager: ResourceManager, executor: str, path_prefix: str):
     context_config = config.executors[executor].context
     raw_workflow_config = copy.deepcopy(config.workflow)
 
     # output of each step
     label_output: Optional[cll.ICllLabelOutput] = None
     selector_output: Optional[cll.ICllSelectorOutput] = None
     train_output: Optional[cll.ICllTrainOutput] = None
     explore_output: Optional[cll.ICllExploreOutput] = None
 
-
     # cursor of update table
     update_cursor = 0
 
     # Start iteration
     for i in itertools.count(0):
 
         # parse workflow config
@@ -134,15 +136,15 @@
                 initiated= i > 0,
             )
             cpk2_context = cp2k.GenericCp2kContext(
                 config=context_config.label.cp2k,
                 path_prefix=os.path.join(iter_path_prefix, 'label-cp2k'),
                 resource_manager=resource_manager,
             )
-            label_output = cp2k.generic_cp2k(cp2k_input, cpk2_context).result()
+            label_output = await cp2k.generic_cp2k(cp2k_input, cpk2_context)
         else:
             raise ValueError('No label method is specified')
 
         # train
         if workflow_config.train.deepmd:
             deepmd_input = deepmd.GenericDeepmdInput(
                 config=workflow_config.train.deepmd,
@@ -152,15 +154,15 @@
                 initiated= i > 0,
             )
             deepmd_context = deepmd.GenericDeepmdContext(
                 path_prefix=os.path.join(iter_path_prefix, 'train-deepmd'),
                 config=context_config.train.deepmd,
                 resource_manager=resource_manager,
             )
-            train_output = deepmd.generic_deepmd(deepmd_input, deepmd_context).result()
+            train_output = await deepmd.generic_deepmd(deepmd_input, deepmd_context)
         else:
             raise ValueError('No train method is specified')
 
         # explore
         if workflow_config.explore.lammps:
             md_options = lammps.GenericLammpsInput.MdOptions(
                 models=train_output.get_mlp_models(),
@@ -172,30 +174,30 @@
                 md_options=md_options,
             )
             lammps_context = lammps.GenericLammpsContext(
                 path_prefix=os.path.join(iter_path_prefix, 'explore-lammps'),
                 config=context_config.explore.lammps,
                 resource_manager=resource_manager,
             )
-            explore_output = lammps.generic_lammps(lammps_input, lammps_context).result()
+            explore_output = await lammps.generic_lammps(lammps_input, lammps_context)
         else:
             raise ValueError('No explore method is specified')
 
         # select
         if workflow_config.select.by_threshold:
             selector_input = selector.ThresholdSelectorInput(
                 config=workflow_config.select.by_threshold,
                 model_devi_data=explore_output.get_model_devi_dataset(),
                 model_devi_out_filename=const.MODEL_DEVI_OUT,
             )
             selector_context = selector.ThresholdSelectorContext(
                 path_prefix=os.path.join(iter_path_prefix, 'selector-threshold'),
                 resource_manager=resource_manager,
             )
-            selector_output = selector.threshold_selector(selector_input, selector_context).result()
+            selector_output = await selector.threshold_selector(selector_input, selector_context)
         else:
             raise ValueError('No select method is specified')
 
         # Update
         update_config = workflow_config.update.walkthrough
 
         # nothing to update because the table is empty
@@ -210,8 +212,8 @@
             raw_workflow_config = merge_dict(copy.deepcopy(
                 config.workflow), update_config.table[update_cursor])
             update_cursor += 1
 
 
 if __name__ == '__main__':
     # use python-fire to parse command line arguments
-    Fire(cll_train_mlp)
+    Fire(run_workflow)
```

### Comparing `ai2_kit-0.3.2/ai2_kit/workflow/fep_mlp.py` & `ai2_kit-0.3.3/ai2_kit/workflow/fep_mlp.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     cll,
 )
 
 from pydantic import BaseModel
 from typing import Dict, List, Optional, Any
 from fire import Fire
 
+import asyncio
 import copy
 import itertools
 import os
 
 logger = get_logger(__name__)
 
 
@@ -56,15 +57,15 @@
 
 
 class FepWorkflowConfig(BaseModel):
     executors: Dict[str, FepExecutorConfig]
     artifacts: ArtifactMap
     workflow: Any
 
-def fep_train_mlp(*config_files, executor: Optional[str] = None, path_prefix: Optional[str] = None):
+def run_workflow(*config_files, executor: Optional[str] = None, path_prefix: Optional[str] = None):
     """
     Training ML potential for FEP
     """
 
     config_data = load_yaml_files(*config_files)
     config = FepWorkflowConfig.parse_obj(config_data)
 
@@ -74,15 +75,18 @@
         raise ValueError('path_prefix should not be empty')
 
     resource_manager = ResourceManager(
         executor_configs=config.executors,
         artifacts=config.artifacts,
         default_executor=executor,
     )
+    return asyncio.run(cll_mlp_training_workflow(config, resource_manager, executor, path_prefix))
 
+
+async def cll_mlp_training_workflow(config: FepWorkflowConfig, resource_manager: ResourceManager, executor: str, path_prefix: str):
     context_config = config.executors[executor].context
     raw_workflow_config = copy.deepcopy(config.workflow)
 
     # output of each step
     neu_label_output: Optional[cll.ICllLabelOutput] = None
     red_label_output: Optional[cll.ICllLabelOutput] = None
 
@@ -133,20 +137,18 @@
         )
         neu_cp2k_context = cp2k.GenericCp2kContext(
             config=context_config.cp2k,
             path_prefix=os.path.join(iter_path_prefix, 'neu-label-cp2k'),
             resource_manager=resource_manager,
         )
 
-
-        red_label_output_future = cp2k.generic_cp2k(red_cp2k_input, red_cpk2_context)
-        neu_label_output_future = cp2k.generic_cp2k(neu_cp2k_input, neu_cp2k_context)
-
-        red_label_output = red_label_output_future.result()
-        neu_label_output = neu_label_output_future.result()
+        red_label_output, neu_label_output = await asyncio.gather(
+            cp2k.generic_cp2k(red_cp2k_input, red_cpk2_context),
+            cp2k.generic_cp2k(neu_cp2k_input, neu_cp2k_context),
+        )
 
         # Train
         red_deepmd_input = deepmd.GenericDeepmdInput(
             config=workflow_config.red.deepmd,
             type_map=type_map,
             old_dataset=[] if red_train_output is None else red_train_output.get_training_dataset(),
             new_dataset=red_label_output.get_labeled_system_dataset(),
@@ -167,19 +169,18 @@
         )
         neu_deepmd_context = deepmd.GenericDeepmdContext(
             path_prefix=os.path.join(iter_path_prefix, 'neu-train-deepmd'),
             config=context_config.deepmd,
             resource_manager=resource_manager,
         )
 
-        red_train_output_future = deepmd.generic_deepmd(red_deepmd_input, red_deepmd_context)
-        neu_train_output_future = deepmd.generic_deepmd(neu_deepmd_input, neu_deepmd_context)
-
-        red_train_output = red_train_output_future.result()
-        neu_train_output = neu_train_output_future.result()
+        red_train_output, neu_train_output = await asyncio.gather(
+            deepmd.generic_deepmd(red_deepmd_input, red_deepmd_context),
+            deepmd.generic_deepmd(neu_deepmd_input, neu_deepmd_context),
+        )
 
         # explore
         lammps_input = lammps.GenericLammpsInput(
             config=workflow_config.lammps,
             type_map=type_map,
             mass_map=mass_map,
             fep_options=lammps.GenericLammpsInput.FepOptions(
@@ -188,16 +189,15 @@
             ),
         )
         lammps_context = lammps.GenericLammpsContext(
             path_prefix=os.path.join(iter_path_prefix, 'explore-lammps'),
             config=context_config.lammps,
             resource_manager=resource_manager,
         )
-        explore_output = lammps.generic_lammps(lammps_input, lammps_context).result()
-
+        explore_output = await lammps.generic_lammps(lammps_input, lammps_context)
 
         # select
         red_selector_input = selector.ThresholdSelectorInput(
             config=workflow_config.red.threshold,
             model_devi_data=explore_output.get_model_devi_dataset(),
             model_devi_out_filename=const.MODEL_DEVI_RED_OUT,
         )
@@ -212,20 +212,18 @@
             model_devi_out_filename=const.MODEL_DEVI_NEU_OUT,
         )
         neu_selector_context = selector.ThresholdSelectorContext(
             path_prefix=os.path.join(iter_path_prefix, 'neu-selector-threshold'),
             resource_manager=resource_manager,
         )
 
-        red_selector_output_future = selector.threshold_selector(red_selector_input, red_selector_context)
-        neu_selector_output_future = selector.threshold_selector(neu_selector_input, neu_selector_context)
-
-        red_selector_output = red_selector_output_future.result()
-        neu_selector_output = neu_selector_output_future.result()
-
+        red_selector_output, neu_selector_output = await asyncio.gather(
+            selector.threshold_selector( red_selector_input, red_selector_context),
+            selector.threshold_selector( neu_selector_input, neu_selector_context),
+        )
 
         # Update
         update_config = workflow_config.update.walkthrough
 
         # nothing to update because the table is empty
         if not update_config.table:
             continue
@@ -234,8 +232,8 @@
             continue
         # update config
         update_cursor += 1
 
 
 if __name__ == '__main__':
     # use python-fire to parse command line arguments
-    Fire(fep_train_mlp)
+    Fire(run_workflow)
```

### Comparing `ai2_kit-0.3.2/pyproject.toml` & `ai2_kit-0.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ai2-kit"
-version = "0.3.2"
+version = "0.3.3"
 description = ""
 authors = ["weihong.xu <xuweihong.cn@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ai2_kit"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `ai2_kit-0.3.2/PKG-INFO` & `ai2_kit-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai2-kit
-Version: 0.3.2
+Version: 0.3.3
 Summary: 
 Author: weihong.xu
 Author-email: xuweihong.cn@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

