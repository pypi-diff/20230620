# Comparing `tmp/ai2_kit-0.3.0.tar.gz` & `tmp/ai2_kit-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai2_kit-0.3.0.tar", max compression
+gzip compressed data, was "ai2_kit-0.3.1.tar", max compression
```

## Comparing `ai2_kit-0.3.0.tar` & `ai2_kit-0.3.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1067 2023-02-07 08:30:11.900671 ai2_kit-0.3.0/LICENSE
--rw-r--r--   0        0        0     1205 2023-06-16 03:38:14.969789 ai2_kit-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.0/ai2_kit/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 03:47:09.348444 ai2_kit-0.3.0/ai2_kit/algorithm/__init__.py
--rw-r--r--   0        0        0    12100 2023-06-13 03:47:09.348444 ai2_kit-0.3.0/ai2_kit/algorithm/proton_transfer.py
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.0/ai2_kit/core/__init__.py
--rw-r--r--   0        0        0     1884 2023-03-22 04:23:44.538179 ai2_kit-0.3.0/ai2_kit/core/artifact.py
--rw-r--r--   0        0        0     3327 2023-03-22 04:23:44.538179 ai2_kit-0.3.0/ai2_kit/core/checkpoint.py
--rw-r--r--   0        0        0      169 2023-06-13 03:47:09.348444 ai2_kit-0.3.0/ai2_kit/core/cmd.py
--rw-r--r--   0        0        0     5766 2023-02-06 09:01:27.000000 ai2_kit-0.3.0/ai2_kit/core/connector.py
--rw-r--r--   0        0        0     7731 2023-06-16 03:38:14.969789 ai2_kit-0.3.0/ai2_kit/core/executor.py
--rw-r--r--   0        0        0     1074 2023-02-22 05:58:23.102960 ai2_kit-0.3.0/ai2_kit/core/future.py
--rw-r--r--   0        0        0     2995 2023-02-17 02:09:28.820341 ai2_kit-0.3.0/ai2_kit/core/job.py
--rw-r--r--   0        0        0      118 2023-02-06 09:01:27.000000 ai2_kit-0.3.0/ai2_kit/core/log.py
--rw-r--r--   0        0        0     8476 2023-06-16 03:38:14.969789 ai2_kit-0.3.0/ai2_kit/core/queue_system.py
--rw-r--r--   0        0        0     2315 2023-03-22 04:23:44.538179 ai2_kit-0.3.0/ai2_kit/core/resource_manager.py
--rw-r--r--   0        0        0     2358 2023-02-27 06:41:41.002117 ai2_kit-0.3.0/ai2_kit/core/script.py
--rw-r--r--   0        0        0     2264 2023-06-16 03:38:14.969789 ai2_kit-0.3.0/ai2_kit/core/util.py
--rw-r--r--   0        0        0        0 2023-06-13 03:47:09.348444 ai2_kit-0.3.0/ai2_kit/dflow/__init__.py
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.0/ai2_kit/domain/__init__.py
--rw-r--r--   0        0        0     2232 2023-03-22 04:23:44.538179 ai2_kit-0.3.0/ai2_kit/domain/cll.py
--rw-r--r--   0        0        0      341 2023-02-27 08:58:57.520622 ai2_kit-0.3.0/ai2_kit/domain/constant.py
--rw-r--r--   0        0        0     8202 2023-06-16 03:38:14.969789 ai2_kit-0.3.0/ai2_kit/domain/cp2k.py
--rw-r--r--   0        0        0     4121 2023-03-22 04:23:44.538179 ai2_kit-0.3.0/ai2_kit/domain/data_helper.py
--rw-r--r--   0        0        0     6797 2023-06-16 03:38:14.969789 ai2_kit-0.3.0/ai2_kit/domain/deepmd.py
--rw-r--r--   0        0        0    15572 2023-06-16 03:38:14.969789 ai2_kit-0.3.0/ai2_kit/domain/lammps.py
--rw-r--r--   0        0        0     3173 2023-06-15 07:40:02.514859 ai2_kit-0.3.0/ai2_kit/domain/selector.py
--rw-r--r--   0        0        0      183 2023-03-22 04:23:44.538179 ai2_kit-0.3.0/ai2_kit/domain/updater.py
--rw-r--r--   0        0        0     1465 2023-06-16 03:38:14.969789 ai2_kit-0.3.0/ai2_kit/main.py
--rw-r--r--   0        0        0        0 2023-06-16 03:38:14.969789 ai2_kit-0.3.0/ai2_kit/tool/__init__.py
--rw-r--r--   0        0        0      744 2023-06-16 03:38:14.969789 ai2_kit-0.3.0/ai2_kit/tool/ase.py
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.0/ai2_kit/workflow/__init__.py
--rw-r--r--   0        0        0     7426 2023-06-15 09:06:34.322595 ai2_kit-0.3.0/ai2_kit/workflow/cll_mlp.py
--rw-r--r--   0        0        0     8519 2023-06-16 03:38:14.969789 ai2_kit-0.3.0/ai2_kit/workflow/fep_mlp.py
--rw-r--r--   0        0        0      821 2023-06-16 03:38:30.319717 ai2_kit-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2189 1970-01-01 00:00:00.000000 ai2_kit-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-02-07 08:30:11.900671 ai2_kit-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1205 2023-06-16 03:38:14.969789 ai2_kit-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.1/ai2_kit/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 03:47:09.348444 ai2_kit-0.3.1/ai2_kit/algorithm/__init__.py
+-rw-r--r--   0        0        0    12100 2023-06-13 03:47:09.348444 ai2_kit-0.3.1/ai2_kit/algorithm/proton_transfer.py
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.1/ai2_kit/core/__init__.py
+-rw-r--r--   0        0        0     1884 2023-03-22 04:23:44.538179 ai2_kit-0.3.1/ai2_kit/core/artifact.py
+-rw-r--r--   0        0        0     3327 2023-03-22 04:23:44.538179 ai2_kit-0.3.1/ai2_kit/core/checkpoint.py
+-rw-r--r--   0        0        0      169 2023-06-13 03:47:09.348444 ai2_kit-0.3.1/ai2_kit/core/cmd.py
+-rw-r--r--   0        0        0     5766 2023-02-06 09:01:27.000000 ai2_kit-0.3.1/ai2_kit/core/connector.py
+-rw-r--r--   0        0        0     7731 2023-06-16 03:38:14.969789 ai2_kit-0.3.1/ai2_kit/core/executor.py
+-rw-r--r--   0        0        0     1090 2023-06-20 06:39:10.182460 ai2_kit-0.3.1/ai2_kit/core/future.py
+-rw-r--r--   0        0        0     3655 2023-06-20 06:39:10.182460 ai2_kit-0.3.1/ai2_kit/core/job.py
+-rw-r--r--   0        0        0      298 2023-06-20 06:39:10.182460 ai2_kit-0.3.1/ai2_kit/core/log.py
+-rw-r--r--   0        0        0     8823 2023-06-20 06:39:10.182460 ai2_kit-0.3.1/ai2_kit/core/queue_system.py
+-rw-r--r--   0        0        0     2315 2023-03-22 04:23:44.538179 ai2_kit-0.3.1/ai2_kit/core/resource_manager.py
+-rw-r--r--   0        0        0     2358 2023-06-19 08:54:25.567391 ai2_kit-0.3.1/ai2_kit/core/script.py
+-rw-r--r--   0        0        0     2524 2023-06-20 06:39:10.182460 ai2_kit-0.3.1/ai2_kit/core/util.py
+-rw-r--r--   0        0        0        0 2023-06-13 03:47:09.348444 ai2_kit-0.3.1/ai2_kit/dflow/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.1/ai2_kit/domain/__init__.py
+-rw-r--r--   0        0        0     1580 2023-06-20 06:39:10.182460 ai2_kit-0.3.1/ai2_kit/domain/cll.py
+-rw-r--r--   0        0        0      341 2023-02-27 08:58:57.520622 ai2_kit-0.3.1/ai2_kit/domain/constant.py
+-rw-r--r--   0        0        0     7929 2023-06-20 06:39:10.182460 ai2_kit-0.3.1/ai2_kit/domain/cp2k.py
+-rw-r--r--   0        0        0     4129 2023-06-20 06:39:10.182460 ai2_kit-0.3.1/ai2_kit/domain/data_helper.py
+-rw-r--r--   0        0        0     6765 2023-06-20 06:39:10.182460 ai2_kit-0.3.1/ai2_kit/domain/deepmd.py
+-rw-r--r--   0        0        0    15672 2023-06-20 06:39:10.182460 ai2_kit-0.3.1/ai2_kit/domain/lammps.py
+-rw-r--r--   0        0        0     3134 2023-06-20 06:39:10.182460 ai2_kit-0.3.1/ai2_kit/domain/selector.py
+-rw-r--r--   0        0        0      183 2023-03-22 04:23:44.538179 ai2_kit-0.3.1/ai2_kit/domain/updater.py
+-rw-r--r--   0        0        0     1465 2023-06-16 03:38:14.969789 ai2_kit-0.3.1/ai2_kit/main.py
+-rw-r--r--   0        0        0        0 2023-06-16 03:38:14.969789 ai2_kit-0.3.1/ai2_kit/tool/__init__.py
+-rw-r--r--   0        0        0      748 2023-06-20 06:39:10.182460 ai2_kit-0.3.1/ai2_kit/tool/ase.py
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.1/ai2_kit/workflow/__init__.py
+-rw-r--r--   0        0        0     7426 2023-06-15 09:06:34.322595 ai2_kit-0.3.1/ai2_kit/workflow/cll_mlp.py
+-rw-r--r--   0        0        0     8519 2023-06-16 03:38:14.969789 ai2_kit-0.3.1/ai2_kit/workflow/fep_mlp.py
+-rw-r--r--   0        0        0      843 2023-06-20 06:39:25.457460 ai2_kit-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2232 1970-01-01 00:00:00.000000 ai2_kit-0.3.1/PKG-INFO
```

### Comparing `ai2_kit-0.3.0/LICENSE` & `ai2_kit-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.0/README.md` & `ai2_kit-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.0/ai2_kit/algorithm/proton_transfer.py` & `ai2_kit-0.3.1/ai2_kit/algorithm/proton_transfer.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.0/ai2_kit/core/artifact.py` & `ai2_kit-0.3.1/ai2_kit/core/artifact.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.0/ai2_kit/core/checkpoint.py` & `ai2_kit-0.3.1/ai2_kit/core/checkpoint.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.0/ai2_kit/core/connector.py` & `ai2_kit-0.3.1/ai2_kit/core/connector.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.0/ai2_kit/core/executor.py` & `ai2_kit-0.3.1/ai2_kit/core/executor.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.0/ai2_kit/core/future.py` & `ai2_kit-0.3.1/ai2_kit/core/future.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-from typing import Generic, Optional, TypeVar, Callable
+from typing import Generic, Optional, TypeVar, Callable, Awaitable
 from abc import abstractmethod
 
 
 T = TypeVar('T')
 
 
-# TODO: use RxPY Observable instead
-# mimic the API of concurrent.future.Future
 class IFuture(Generic[T]):
 
     @abstractmethod
     def done(self) -> bool:
         pass
 
     @abstractmethod
     def result(self, timeout: Optional[float] = None) -> T:
         pass
 
+    async def result_async(self, timeout: Optional[float] = None) -> T:
+        ...
+
 class DummyFuture(IFuture[T]):
 
     def __init__(self, value: T) -> None:
         self.value = value
 
     def done(self):
         return True
```

### Comparing `ai2_kit-0.3.0/ai2_kit/core/queue_system.py` & `ai2_kit-0.3.1/ai2_kit/core/queue_system.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pydantic import BaseModel
-from typing import Optional, Dict
+from typing import Optional, Dict, Awaitable
 from abc import ABC, abstractmethod
 import shlex
 import os
 import re
 import shortuuid
 import time
 import asyncio
@@ -58,14 +58,15 @@
     @abstractmethod
     def cancel(self, job_id: str):
         ...
 
     def _post_submit(self, job: 'QueueJobFuture'):
         ...
 
+    # TODO: integrate with checkpoint system
     def submit(self, script: str, cwd: str, name: Optional[str] = None, success_indicator: Optional[str] = None):
 
         if name is None:
             name = shortuuid.uuid() + self.get_script_suffix()
         quoted_cwd = shlex.quote(cwd)
 
         if success_indicator is None:
@@ -243,43 +244,51 @@
 
         state = self._queue_system.get_job_state(self._job_id, self.success_indicator_path)
         if state.terminal:
             self._done_state = state
 
         return state
 
+    # Deprecated, use resubmit
     def redo(self):
+        job = self.resubmit()
+        self._done_state = None
+        self._tries += 1
+        self._job_id = job._job_id
+
+    def resubmit(self):
         if not self.done():
-            raise RuntimeError('Cannot redo an unfinished job!')
-        job = self._queue_system.submit(
+            raise RuntimeError('Cannot resubmit an unfinished job!')
+        return self._queue_system.submit(
             script=self._script,
             cwd=self._cwd,
             name=self._name,
             success_indicator=self._success_indicator,
         )
-        self._done_state = None
-        self._tries += 1
-        self._job_id = job._job_id
 
     def get_tries(self):
         return self._tries
 
     def is_success(self):
         return self.get_job_state() is JobState.COMPLETED
 
     def cancel(self):
         self._queue_system.cancel(self._job_id)
 
     def done(self):
         return self.get_job_state().terminal
 
     def result(self, timeout: float = float('inf')) -> JobState:
-        return asyncio.run(self.async_result(timeout))
+        return asyncio.run(self.result_async(timeout))
 
-    async def async_result(self, timeout: float = float('inf')) -> JobState:
+    async def result_async(self, timeout: float = float('inf')) -> JobState:
+        '''
+        Though this is not fully async, as the job submission and state polling are still blocking,
+        but it is already good enough to handle thousands of jobs (I guess).
+        '''
         timeout_ts = time.time() + timeout
         while time.time() < timeout_ts:
             if self.done():
                 return self.get_job_state()
             else:
                 await asyncio.sleep(self._polling_interval)
         else:
@@ -290,8 +299,7 @@
             name=self._name,
             cwd=self._cwd,
             job_id=self._job_id,
             success_indicator=self._success_indicator,
             polling_interval=self._polling_interval,
             state=self.get_job_state(),
         ))
-
```

### Comparing `ai2_kit-0.3.0/ai2_kit/core/resource_manager.py` & `ai2_kit-0.3.1/ai2_kit/core/resource_manager.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.0/ai2_kit/core/script.py` & `ai2_kit-0.3.1/ai2_kit/core/script.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.0/ai2_kit/core/util.py` & `ai2_kit-0.3.1/ai2_kit/core/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,11 +77,17 @@
         d = d[key]
     d[keys[-1]] = value
 
 def sort_unique_str_list(l: List[str]) -> List[str]:
     """remove duplicate str and sort"""
     return list(sorted(set(l)))
 
-
 T = TypeVar('T')
 def flatten(l: List[List[T]]) -> List[T]:
-    return [item for sublist in l for item in sublist]
+    return [item for sublist in l for item in sublist]
+
+def format_env_string(s: str) -> str:
+    return s.format(**os.environ)
+
+def split_list(l: List[T], n: int) -> List[List[T]]:
+    """split a list into n chunks, the last chunk may be smaller than others"""
+    return [l[i:i + n] for i in range(0, len(l), n)]
```

### Comparing `ai2_kit-0.3.0/ai2_kit/domain/cll.py` & `ai2_kit-0.3.1/ai2_kit/domain/cll.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,101 +1,69 @@
 from abc import abstractmethod, ABC
 from ai2_kit.core.artifact import Artifact
 from ai2_kit.core.future import IFuture
 from ai2_kit.core.resource_manager import ResourceManager
-from typing import List, Callable, Optional
+from typing import List, Callable, Any
 from dataclasses import dataclass
 
 @dataclass
 class BaseCllContext:
     path_prefix: str
     resource_manager: ResourceManager
 
 ######################
 # CLL Labeling Tasks #
 ######################
 
-class ICllLabelInput(ABC):
-
-    @abstractmethod
-    def set_systems(self, systems: List[Artifact]):
-        ...
-
 
 class ICllLabelOutput(ABC):
 
     @abstractmethod
     def get_labeled_system_dataset(self) -> List[Artifact]:
         ...
 
-CllLabelTaskType = Callable[[ICllLabelInput, BaseCllContext], IFuture[ICllLabelOutput]]
+CllLabelTaskType = Callable[[Any, BaseCllContext], IFuture[ICllLabelOutput]]
 
 ######################
 # CLL Training Tasks #
 ######################
 
-class ICllTrainInput(ABC):
-
-    @abstractmethod
-    def update_training_dataset(self, data: List[Artifact]):
-        ...
-
-
 class ICllTrainOutput(ABC):
 
     @abstractmethod
     def get_mlp_models(self) -> List[Artifact]:
         ...
 
     @abstractmethod
     def get_training_dataset(self) -> List[Artifact]:
         ...
 
 
-CllTrainTaskType = Callable[[ICllTrainInput, BaseCllContext], IFuture[ICllTrainOutput]]
+CllTrainTaskType = Callable[[Any, BaseCllContext], IFuture[ICllTrainOutput]]
 
 ######################
 # CLL Explore Tasks #
 ######################
 
-class ICllExploreInput(ABC):
-
-    @abstractmethod
-    def set_md_models(self, models: List[Artifact]):
-        ...
-
-    @abstractmethod
-    def set_fep_models(self, red_models: List[Artifact], neu_models: List[Artifact]):
-        ...
-
-
 class ICllExploreOutput(ABC):
 
     @abstractmethod
     def get_model_devi_dataset(self) -> List[Artifact]:
         ...
 
-
-CllExploreTaskType = Callable[[ICllExploreInput, BaseCllContext], IFuture[ICllExploreOutput]]
+CllExploreTaskType = Callable[[Any, BaseCllContext], IFuture[ICllExploreOutput]]
 
 ######################
 # CLL Select Task    #
 ######################
 
-class ICllSelectorInput(ABC):
-
-    @abstractmethod
-    def set_model_devi_dataset(self, data: List[Artifact]):
-        ...
-
 class ICllSelectorOutput(ABC):
 
     @abstractmethod
     def get_model_devi_dataset(self) -> List[Artifact]:
         ...
 
     @abstractmethod
     def get_passing_rate(self) -> float:
         ...
 
-CllSelectorTaskType = Callable[[ICllSelectorInput, BaseCllContext], IFuture[ICllSelectorOutput]]
-
+CllSelectorTaskType = Callable[[Any, BaseCllContext], IFuture[ICllSelectorOutput]]
```

### Comparing `ai2_kit-0.3.0/ai2_kit/domain/cp2k.py` & `ai2_kit-0.3.1/ai2_kit/domain/cp2k.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from pydantic import BaseModel
 from dataclasses import dataclass
 
 import copy
 import os
 
 from .data_helper import LammpsOutputHelper, XyzHelper, Cp2kOutputHelper, ase_atoms_to_cp2k_input_data
-from .cll import ICllLabelInput, ICllLabelOutput, BaseCllContext
+from .cll import ICllLabelOutput, BaseCllContext
 
 logger = get_logger(__name__)
 
 class GenericCp2kInputConfig(BaseModel):
     init_system_files: List[str] = []
     limit: int = 50
     input_template: Union[dict, str]
@@ -35,24 +35,20 @@
 
 class GenericCp2kContextConfig(BaseModel):
     script_template: BashTemplate
     cp2k_cmd: str = 'cp2k'
     concurrency: int = 5
 
 @dataclass
-class GenericCp2kInput(ICllLabelInput):
-
+class GenericCp2kInput:
     config: GenericCp2kInputConfig
     system_files: List[Artifact]
     type_map: List[str]
     initiated: bool = False
 
-    def set_systems(self, systems: List[Artifact]):
-        self.system_files = systems
-
 
 @dataclass
 class GenericCp2kContext(BaseCllContext):
     config: GenericCp2kContextConfig
 
 
 @dataclass
@@ -101,15 +97,16 @@
 
     # resolve data files
     lammps_dump_files: List[Artifact] = []
     xyz_files: List[Artifact] = []
 
     # TODO: support POSCAR in the future
     # TODO: refactor the way of handling different file formats
-    for system_file in input.system_files:
+    system_files = ctx.resource_manager.resolve_artifacts(input.system_files)
+    for system_file in system_files:
         if LammpsOutputHelper.is_match(system_file):
             lammps_out = LammpsOutputHelper(system_file)
             lammps_dump_files.extend(lammps_out.get_passed_dump_files())
         elif XyzHelper.is_match(system_file):
             xyz_files.append(system_file)
         else:
             raise ValueError(f'unsupported format {system_file.url}: {system_file.format}')
@@ -171,32 +168,29 @@
                             type_map: List[str],
                             input_template: dict,
                             base_dir: str,
                             limit: int = 0,
                             input_file_name: str = 'input.inp',
                             ) -> List[str]:
         """Generate CP2K input files from LAMMPS dump files or XYZ files."""
-
-        # TODO: pymatgen has a better support for cp2k input, replace cp2k_input_tools with pymatgen in the future
-        # https://pymatgen.org/pymatgen.io.cp2k.inputs.html#pymatgen.io.cp2k.inputs.Cp2kInput
         from cp2k_input_tools import DEFAULT_CP2K_INPUT_XML
         from cp2k_input_tools.generator import CP2KInputGenerator
 
         import ase.io
         from ase import Atoms
 
         cp2k_generator = CP2KInputGenerator(DEFAULT_CP2K_INPUT_XML)
         task_dirs = []
         atoms_list: List[Atoms] = []
 
         # read atoms
         for dump_file in lammps_dump_files:
             atoms_list += ase.io.read(dump_file, ':', format='lammps-dump-text', order=False, specorder=type_map)  # type: ignore
         for xyz_file in xyz_files:
-            atoms_list += ase.io.read(xyz_file, ':', format='extxyz', order=False)  # type: ignore
+            atoms_list += ase.io.read(xyz_file, ':', format='extxyz')  # type: ignore
 
         if limit > 0:
             atoms_list = atoms_list[:limit]
 
         for i, atoms in enumerate(atoms_list):
             # create task dir
             task_dir = os.path.join(base_dir, f'{str(i).zfill(6)}')
```

### Comparing `ai2_kit-0.3.0/ai2_kit/domain/data_helper.py` & `ai2_kit-0.3.1/ai2_kit/domain/data_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,16 +78,16 @@
 
         atoms_list: List[Atoms] = []
         for cp2k_output in cp2k_outputs:
             dp_system = dpdata.LabeledSystem(os.path.join(cp2k_output['url'], 'output'), fmt='cp2k/output', type_map=type_map)
             atoms_list.extend(dp_system.to_ase_structure())  # type: ignore
 
         output_dirs = []
-        for symbols, atoms_group in groupby(atoms_list, key=lambda x: str(x.symbols)):
-            output_dir = os.path.join(base_dir, symbols)
+        for i, (symbols, atoms_group) in enumerate(groupby(atoms_list, key=lambda x: str(x.symbols))):
+            output_dir = os.path.join(base_dir, f'{i:03d}')
             atoms_group = list(atoms_group)
             if not atoms_group:
                 continue
             dp_system = dpdata.LabeledSystem(atoms_group[0], fmt='ase/structure')
             for atoms in atoms_group[1:]:
                 dp_system += dpdata.LabeledSystem(atoms, fmt='ase/structure')
             dp_system.to_deepmd_npy(output_dir, set_size=len(dp_system))  # type: ignore
@@ -103,15 +103,15 @@
     """workaround for cloudpickle issue"""
     def convert_to_lammps_input_data(poscar_files: List[ArtifactDict], base_dir: str, type_map: List[str]):
         import dpdata
         import os
 
         lammps_data_files = []
         for i, poscar_file in enumerate(poscar_files):
-            output_file = os.path.join(base_dir, f'{str(i).zfill(6)}-.lammps.data')
+            output_file = os.path.join(base_dir, f'{i:06d}.lammps.data')
             dpdata.System(poscar_file['url'], fmt='vasp/poscar', type_map=type_map).to_lammps_lmp(output_file)  # type: ignore
             lammps_data_files.append(output_file)
         # TODO: return ArtifactDict
         return lammps_data_files
 
     return convert_to_lammps_input_data
 convert_to_lammps_input_data = __convert_to_lammps_input_data()
```

### Comparing `ai2_kit-0.3.0/ai2_kit/domain/deepmd.py` & `ai2_kit-0.3.1/ai2_kit/domain/deepmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from dataclasses import dataclass
 import os
 import copy
 import random
 import sys
 import json
 
-from .cll import ICllTrainInput, ICllTrainOutput, BaseCllContext
+from .cll import ICllTrainOutput, BaseCllContext
 from .data_helper import Cp2kOutputHelper, DeepmdNpyHelper, DeepmdModelHelper, convert_to_deepmd_npy
 from .constant import (
     DP_CHECKPOINT_FILE,
     DP_DISP_FILE,
     DP_PROFILING_FILE,
     DP_INPUT_FILE,
     DP_FROZEN_MODEL,
@@ -35,15 +35,15 @@
 
 class GenericDeepmdContextConfig(BaseModel):
     script_template: BashTemplate
     dp_cmd: str = 'dp'
 
 
 @dataclass
-class GenericDeepmdInput(ICllTrainInput):
+class GenericDeepmdInput:
     config: GenericDeepmdInputConfig
     type_map: List[str]
     old_dataset: List[Artifact]  # training data used by previous iteration
     new_dataset: List[Artifact]  # training data used by current iteration
     initiated: bool = False
 
     def update_training_dataset(self, dataset: List[Artifact]):
```

### Comparing `ai2_kit-0.3.0/ai2_kit/domain/lammps.py` & `ai2_kit-0.3.1/ai2_kit/domain/lammps.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from ai2_kit.core.job import GatherJobsFuture, retry_fn
 from ai2_kit.core.future import map_future
 
 from typing import List, Literal, Optional, Union, Mapping, Sequence
 from pydantic import BaseModel
 from dataclasses import dataclass
 from string import Template
+from allpairspy import AllPairs
 import os
 import itertools
 import random
 
 
 from .cll import BaseCllContext, ICllExploreOutput
 from .constant import (
@@ -167,17 +168,18 @@
     ]
 
     for k, v in input.config.explore_vars.others.items():
         combination_fields.append(k)
         combination_values.append(v)  # type: ignore
 
     if 1 < input.config.n_wise <= len(combination_fields):
-        #TODO: implement n-wise combination
-        raise NotImplementedError('n-wise combination is not implemented yet')
+        logger.info('using %d-wise combination', input.config.n_wise)
+        combinations = AllPairs(combination_values, n=input.config.n_wise)
     else:
+        logger.info('using full combination')
         combinations = itertools.product(*combination_values)
 
     lammps_task_dirs = []
     lammps_input_file_name = 'lammps.input'
 
     for i, combination in enumerate(combinations):
         data_file, temp, pres = combination[:3]
```

### Comparing `ai2_kit-0.3.0/ai2_kit/domain/selector.py` & `ai2_kit-0.3.1/ai2_kit/domain/selector.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import List
 from io import StringIO
 from pydantic import BaseModel
 from dataclasses import dataclass
 import pandas as pd
 
 from .data_helper import LammpsOutputHelper
-from .cll import ICllSelectorInput, ICllSelectorOutput, BaseCllContext
+from .cll import ICllSelectorOutput, BaseCllContext
 
 logger = get_logger(__name__)
 
 class ThresholdSelectorInputConfig(BaseModel):
     f_trust_lo: float
     f_trust_hi: float
 
@@ -32,23 +32,22 @@
     def get_model_devi_dataset(self):
         return self.model_devi_data
 
     def get_passing_rate(self) -> float:
         return self.passing_rate
 
 @dataclass
-class ThresholdSelectorInput(ICllSelectorInput):
+class ThresholdSelectorInput:
     config: ThresholdSelectorInputConfig
     model_devi_data: List[Artifact]
     model_devi_out_filename: str
 
     def set_model_devi_dataset(self, data: List[Artifact]):
         self.model_devi_data = data
 
-
 def threshold_selector(input: ThresholdSelectorInput, ctx: ThresholdSelectorContext):
     executor = ctx.resource_manager.default_executor
 
     f_trust_lo = input.config.f_trust_lo
     f_trust_hi = input.config.f_trust_hi
     col_force = 'avg_devi_f'
     logger.info('criteria: %f <= %s < %f ', f_trust_lo, col_force, f_trust_hi)
```

### Comparing `ai2_kit-0.3.0/ai2_kit/main.py` & `ai2_kit-0.3.1/ai2_kit/main.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.0/ai2_kit/tool/ase.py` & `ai2_kit-0.3.1/ai2_kit/tool/ase.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import ase.io
 from ase import Atoms
 from typing import List
 
 class AseHelper:
     def __init__(self):
-        self.atoms_list: List[Atoms] = []
+        self._atoms_list: List[Atoms] = []
 
     def read(self, filename: str, **kwargs):
         kwargs.setdefault('index', ':')
         data = ase.io.read(filename, **kwargs)
         if not isinstance(data, list):
             data = [data]
-        self.atoms_list = data
+        self._atoms_list = data
         return self
 
     def write(self, filename: str, **kwargs):
-        ase.io.write(filename, self.atoms_list, **kwargs)
+        ase.io.write(filename, self._atoms_list, **kwargs)
         return self
 
     def write_each_frame(self, filename: str, **kwargs):
-        for i, atoms in enumerate(self.atoms_list):
+        for i, atoms in enumerate(self._atoms_list):
             ase.io.write(filename.format(i=i), atoms, **kwargs)
         return self
 
     def done(self):
         ...
```

### Comparing `ai2_kit-0.3.0/ai2_kit/workflow/cll_mlp.py` & `ai2_kit-0.3.1/ai2_kit/workflow/cll_mlp.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.0/ai2_kit/workflow/fep_mlp.py` & `ai2_kit-0.3.1/ai2_kit/workflow/fep_mlp.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.0/pyproject.toml` & `ai2_kit-0.3.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ai2-kit"
-version = "0.3.0"
+version = "0.3.1"
 description = ""
 authors = ["weihong.xu <xuweihong.cn@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ai2_kit"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -17,14 +17,15 @@
 shortuuid = "^1.0.11"
 dpdata = "^0.2.13"
 pandas = "^1.5.3"
 cp2k-input-tools = "^0.8.2"
 ase = "^3.22.1"
 pymatgen = "^2023.2.22"
 mdanalysis = "^2.4.3"
+allpairspy = "^2.5.0"
 
 
 [[tool.poetry.source]]
 name = "ustc"
 url = "https://pypi.mirrors.ustc.edu.cn/simple/"
 default = true
 secondary = false
```

### Comparing `ai2_kit-0.3.0/PKG-INFO` & `ai2_kit-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: ai2-kit
-Version: 0.3.0
+Version: 0.3.1
 Summary: 
 Author: weihong.xu
 Author-email: xuweihong.cn@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: allpairspy (>=2.5.0,<3.0.0)
 Requires-Dist: ase (>=3.22.1,<4.0.0)
 Requires-Dist: cloudpickle (>=2.2.0,<3.0.0)
 Requires-Dist: cp2k-input-tools (>=0.8.2,<0.9.0)
 Requires-Dist: dpdata (>=0.2.13,<0.3.0)
 Requires-Dist: fabric (>=2.7.1,<3.0.0)
 Requires-Dist: fire (>=0.5.0,<0.6.0)
 Requires-Dist: invoke (>=1.7.3,<2.0.0)
```

