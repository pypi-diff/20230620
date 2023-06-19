# Comparing `tmp/chronus-0.3.8.tar.gz` & `tmp/chronus-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chronus-0.3.8.tar", max compression
+gzip compressed data, was "chronus-0.3.9.tar", max compression
```

## Comparing `chronus-0.3.8.tar` & `chronus-0.3.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1072 2023-02-28 09:33:02.453690 chronus-0.3.8/LICENSE
--rw-r--r--   0        0        0    10584 2023-05-16 08:44:26.161599 chronus-0.3.8/README.md
--rw-r--r--   0        0        0        1 2023-04-17 10:44:37.558827 chronus-0.3.8/chronus/SystemIntegration/__init__.py
--rw-r--r--   0        0        0        0 2023-05-16 08:44:26.162542 chronus-0.3.8/chronus/SystemIntegration/application_runners/__init__.py
--rw-r--r--   0        0        0     6026 2023-05-16 08:44:26.163337 chronus-0.3.8/chronus/SystemIntegration/application_runners/hpcg.py
--rw-r--r--   0        0        0        0 2023-05-16 08:44:26.163553 chronus-0.3.8/chronus/SystemIntegration/cpu_info_services/__init__.py
--rw-r--r--   0        0        0     2714 2023-05-16 08:44:26.163877 chronus-0.3.8/chronus/SystemIntegration/cpu_info_services/cpu_info_service.py
--rw-r--r--   0        0        0        0 2023-05-16 08:44:26.164105 chronus-0.3.8/chronus/SystemIntegration/optimizers/__init__.py
--rw-r--r--   0        0        0     1794 2023-05-16 08:44:26.164404 chronus-0.3.8/chronus/SystemIntegration/optimizers/bruteforce_optmizer.py
--rw-r--r--   0        0        0     3672 2023-05-16 08:44:26.164708 chronus-0.3.8/chronus/SystemIntegration/optimizers/linear_regression.py
--rw-r--r--   0        0        0     2924 2023-05-16 08:44:26.165008 chronus-0.3.8/chronus/SystemIntegration/optimizers/random_tree_forrest.py
--rw-r--r--   0        0        0        0 2023-05-16 08:44:26.165232 chronus-0.3.8/chronus/SystemIntegration/repositories/__init__.py
--rw-r--r--   0        0        0     2559 2023-05-16 08:44:26.165610 chronus-0.3.8/chronus/SystemIntegration/repositories/csv_repository.py
--rw-r--r--   0        0        0    14568 2023-05-16 08:44:46.855479 chronus-0.3.8/chronus/SystemIntegration/repositories/sqlite_repository.py
--rw-r--r--   0        0        0        0 2023-05-16 08:44:26.166377 chronus-0.3.8/chronus/SystemIntegration/settings_interface/__init__.py
--rw-r--r--   0        0        0     1336 2023-05-16 08:44:26.167270 chronus-0.3.8/chronus/SystemIntegration/settings_interface/etc_storage.py
--rw-r--r--   0        0        0        0 2023-05-16 08:44:26.167468 chronus-0.3.8/chronus/SystemIntegration/system_service_interfaces/__init__.py
--rw-r--r--   0        0        0     1776 2023-05-16 08:44:26.167789 chronus-0.3.8/chronus/SystemIntegration/system_service_interfaces/ipmi_system_service.py
--rw-r--r--   0        0        0      330 2023-04-17 10:14:26.979910 chronus-0.3.8/chronus/__init__.py
--rw-r--r--   0        0        0    12196 2023-05-16 08:45:31.325538 chronus-0.3.8/chronus/__main__.py
--rw-r--r--   0        0        0        0 2023-05-16 08:44:26.168831 chronus-0.3.8/chronus/application/__init__.py
--rw-r--r--   0        0        0     3710 2023-05-16 08:44:26.169283 chronus-0.3.8/chronus/application/benchmark_service.py
--rw-r--r--   0        0        0     2437 2023-05-16 08:44:26.170578 chronus-0.3.8/chronus/application/init_model_service.py
--rw-r--r--   0        0        0     1531 2023-05-16 08:44:26.172209 chronus-0.3.8/chronus/application/load_model_service.py
--rw-r--r--   0        0        0      602 2023-05-16 08:44:26.172846 chronus-0.3.8/chronus/application/run_model_service.py
--rw-r--r--   0        0        0        0 2023-05-16 08:44:26.173616 chronus-0.3.8/chronus/cli/__init__.py
--rw-r--r--   0        0        0      742 2023-05-16 08:44:26.174081 chronus-0.3.8/chronus/cli/setup.py
--rw-r--r--   0        0        0      197 2023-05-16 08:44:26.174432 chronus-0.3.8/chronus/domain/LocalSettings.py
--rw-r--r--   0        0        0     2195 2023-05-16 08:44:26.175042 chronus-0.3.8/chronus/domain/Run.py
--rw-r--r--   0        0        0        0 2023-04-17 10:14:26.980936 chronus-0.3.8/chronus/domain/__init__.py
--rw-r--r--   0        0        0      461 2023-05-16 08:44:26.175369 chronus-0.3.8/chronus/domain/benchmark.py
--rw-r--r--   0        0        0     1181 2023-05-16 08:44:26.175909 chronus-0.3.8/chronus/domain/configuration.py
--rw-r--r--   0        0        0      523 2023-05-16 08:44:26.176245 chronus-0.3.8/chronus/domain/cpu_info.py
--rw-r--r--   0        0        0        0 2023-04-23 12:44:06.746442 chronus-0.3.8/chronus/domain/interfaces/__init__.py
--rw-r--r--   0        0        0      520 2023-05-16 08:44:26.176915 chronus-0.3.8/chronus/domain/interfaces/application_runner_interface.py
--rw-r--r--   0        0        0      158 2023-05-16 08:44:26.177690 chronus-0.3.8/chronus/domain/interfaces/cpu_info_service_interface.py
--rw-r--r--   0        0        0      918 2023-05-16 08:44:26.178172 chronus-0.3.8/chronus/domain/interfaces/optimizer_interface.py
--rw-r--r--   0        0        0      986 2023-05-16 08:44:26.178577 chronus-0.3.8/chronus/domain/interfaces/repository_interface.py
--rw-r--r--   0        0        0      499 2023-05-16 08:44:26.178973 chronus-0.3.8/chronus/domain/interfaces/settings_interface.py
--rw-r--r--   0        0        0      160 2023-05-16 08:44:26.179807 chronus-0.3.8/chronus/domain/interfaces/system_service_interface.py
--rw-r--r--   0        0        0      274 2023-05-16 08:44:26.180314 chronus-0.3.8/chronus/domain/model.py
--rw-r--r--   0        0        0      369 2023-05-16 08:44:26.181393 chronus-0.3.8/chronus/domain/system_sample.py
--rw-r--r--   0        0        0     3757 2023-05-16 08:44:46.856410 chronus-0.3.8/pyproject.toml
--rw-r--r--   0        0        0    11888 1970-01-01 00:00:00.000000 chronus-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-28 08:15:27.618142 chronus-0.3.9/LICENSE
+-rw-r--r--   0        0        0    10584 2023-05-10 09:58:34.046336 chronus-0.3.9/README.md
+-rw-r--r--   0        0        0        1 2023-04-28 08:15:27.622142 chronus-0.3.9/chronus/SystemIntegration/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 20:47:36.430457 chronus-0.3.9/chronus/SystemIntegration/application_runners/__init__.py
+-rw-r--r--   0        0        0     6026 2023-05-06 16:21:47.233103 chronus-0.3.9/chronus/SystemIntegration/application_runners/hpcg.py
+-rw-r--r--   0        0        0        0 2023-05-02 20:47:36.430457 chronus-0.3.9/chronus/SystemIntegration/cpu_info_services/__init__.py
+-rw-r--r--   0        0        0     2714 2023-05-10 09:48:21.426509 chronus-0.3.9/chronus/SystemIntegration/cpu_info_services/cpu_info_service.py
+-rw-r--r--   0        0        0        0 2023-05-05 13:33:24.644402 chronus-0.3.9/chronus/SystemIntegration/optimizers/__init__.py
+-rw-r--r--   0        0        0     1794 2023-05-10 09:48:21.430509 chronus-0.3.9/chronus/SystemIntegration/optimizers/bruteforce_optmizer.py
+-rw-r--r--   0        0        0     3672 2023-05-10 09:48:21.430509 chronus-0.3.9/chronus/SystemIntegration/optimizers/linear_regression.py
+-rw-r--r--   0        0        0     2924 2023-05-10 09:48:21.430509 chronus-0.3.9/chronus/SystemIntegration/optimizers/random_tree_forrest.py
+-rw-r--r--   0        0        0        0 2023-05-02 20:47:36.430457 chronus-0.3.9/chronus/SystemIntegration/repositories/__init__.py
+-rw-r--r--   0        0        0     2559 2023-05-05 17:12:11.384766 chronus-0.3.9/chronus/SystemIntegration/repositories/csv_repository.py
+-rw-r--r--   0        0        0    14565 2023-05-10 09:48:21.430509 chronus-0.3.9/chronus/SystemIntegration/repositories/sqlite_repository.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:48:21.430509 chronus-0.3.9/chronus/SystemIntegration/settings_interface/__init__.py
+-rw-r--r--   0        0        0     1336 2023-05-10 11:09:21.787582 chronus-0.3.9/chronus/SystemIntegration/settings_interface/etc_storage.py
+-rw-r--r--   0        0        0        0 2023-05-02 20:47:36.430457 chronus-0.3.9/chronus/SystemIntegration/system_service_interfaces/__init__.py
+-rw-r--r--   0        0        0     1776 2023-05-10 09:48:21.430509 chronus-0.3.9/chronus/SystemIntegration/system_service_interfaces/ipmi_system_service.py
+-rw-r--r--   0        0        0      330 2023-04-28 08:15:27.622142 chronus-0.3.9/chronus/__init__.py
+-rw-r--r--   0        0        0    12176 2023-05-17 20:32:25.541075 chronus-0.3.9/chronus/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-02 20:47:36.430457 chronus-0.3.9/chronus/application/__init__.py
+-rw-r--r--   0        0        0     3710 2023-05-10 09:48:21.430509 chronus-0.3.9/chronus/application/benchmark_service.py
+-rw-r--r--   0        0        0     2437 2023-05-10 10:47:43.600083 chronus-0.3.9/chronus/application/init_model_service.py
+-rw-r--r--   0        0        0     1531 2023-05-10 10:47:43.600083 chronus-0.3.9/chronus/application/load_model_service.py
+-rw-r--r--   0        0        0      602 2023-05-10 09:48:21.430509 chronus-0.3.9/chronus/application/run_model_service.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:48:21.430509 chronus-0.3.9/chronus/cli/__init__.py
+-rw-r--r--   0        0        0      742 2023-05-10 09:48:21.430509 chronus-0.3.9/chronus/cli/setup.py
+-rw-r--r--   0        0        0      197 2023-05-10 09:48:21.430509 chronus-0.3.9/chronus/domain/LocalSettings.py
+-rw-r--r--   0        0        0     2195 2023-05-10 09:48:21.430509 chronus-0.3.9/chronus/domain/Run.py
+-rw-r--r--   0        0        0        0 2023-04-28 08:15:27.622142 chronus-0.3.9/chronus/domain/__init__.py
+-rw-r--r--   0        0        0      461 2023-05-10 09:48:21.430509 chronus-0.3.9/chronus/domain/benchmark.py
+-rw-r--r--   0        0        0     1181 2023-05-10 09:48:21.430509 chronus-0.3.9/chronus/domain/configuration.py
+-rw-r--r--   0        0        0      523 2023-05-10 09:48:21.430509 chronus-0.3.9/chronus/domain/cpu_info.py
+-rw-r--r--   0        0        0        0 2023-04-28 08:15:27.622142 chronus-0.3.9/chronus/domain/interfaces/__init__.py
+-rw-r--r--   0        0        0      520 2023-05-10 09:48:21.430509 chronus-0.3.9/chronus/domain/interfaces/application_runner_interface.py
+-rw-r--r--   0        0        0      158 2023-05-10 09:48:21.430509 chronus-0.3.9/chronus/domain/interfaces/cpu_info_service_interface.py
+-rw-r--r--   0        0        0      918 2023-05-10 09:48:21.430509 chronus-0.3.9/chronus/domain/interfaces/optimizer_interface.py
+-rw-r--r--   0        0        0      986 2023-05-10 09:48:21.430509 chronus-0.3.9/chronus/domain/interfaces/repository_interface.py
+-rw-r--r--   0        0        0      499 2023-05-10 09:48:21.430509 chronus-0.3.9/chronus/domain/interfaces/settings_interface.py
+-rw-r--r--   0        0        0      160 2023-05-10 09:48:21.430509 chronus-0.3.9/chronus/domain/interfaces/system_service_interface.py
+-rw-r--r--   0        0        0      274 2023-05-10 10:33:20.168286 chronus-0.3.9/chronus/domain/model.py
+-rw-r--r--   0        0        0      369 2023-05-10 09:48:21.430509 chronus-0.3.9/chronus/domain/system_sample.py
+-rw-r--r--   0        0        0     3757 2023-05-17 20:33:14.553054 chronus-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0    11888 1970-01-01 00:00:00.000000 chronus-0.3.9/PKG-INFO
```

### Comparing `chronus-0.3.8/LICENSE` & `chronus-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `chronus-0.3.8/README.md` & `chronus-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `chronus-0.3.8/chronus/SystemIntegration/application_runners/hpcg.py` & `chronus-0.3.9/chronus/SystemIntegration/application_runners/hpcg.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.8/chronus/SystemIntegration/cpu_info_services/cpu_info_service.py` & `chronus-0.3.9/chronus/SystemIntegration/cpu_info_services/cpu_info_service.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.8/chronus/SystemIntegration/optimizers/bruteforce_optmizer.py` & `chronus-0.3.9/chronus/SystemIntegration/optimizers/bruteforce_optmizer.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.8/chronus/SystemIntegration/optimizers/linear_regression.py` & `chronus-0.3.9/chronus/SystemIntegration/optimizers/linear_regression.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.8/chronus/SystemIntegration/optimizers/random_tree_forrest.py` & `chronus-0.3.9/chronus/SystemIntegration/optimizers/random_tree_forrest.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.8/chronus/SystemIntegration/repositories/csv_repository.py` & `chronus-0.3.9/chronus/SystemIntegration/repositories/csv_repository.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.8/chronus/SystemIntegration/repositories/sqlite_repository.py` & `chronus-0.3.9/chronus/SystemIntegration/repositories/sqlite_repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -342,26 +342,26 @@
             ),
         )
         conn.commit()
         conn.close()
 
     def _create_table(self) -> None:
         if not self.__check_db_exists():
-            self.logger.debug(f"Database already exists at {self.path}.")
+            self.logger.info(f"Database already exists at {self.path}.")
             if not self.__ask_to_create_one():
                 raise Exception("Database does not exist, and user chose not to create one.")
         with sqlite3.connect(self.path) as conn:
             cursor = conn.cursor()
             cursor.execute(CREATE_BENCHMARKS_TABLE_QUERY)
             cursor.execute(CREATE_RUNS_TABLE_QUERY)
             cursor.execute(CREATE_SYSTEM_SAMPLES_TABLE_QUERY)
             cursor.execute(CREATE_MODEL_TABLE_QUERY)
 
         self.__run_migration(ADD_CPUFREQ_TO_SYSTEM_SAMPLE_MIGRATION_QUERY)
-        self.logger.debug(
+        self.logger.info(
             f"Tables 'benchmarks', 'runs', and 'system_samples' have been created in {self.path}."
         )
 
     def get_system_samples(self, run_id: int) -> list[SystemSample]:
         samples = []
         with sqlite3.connect(self.path) as conn:
             cursor = conn.cursor()
@@ -446,9 +446,9 @@
     def __run_migration(self, SQL_QUERY: str):
         try:
             with sqlite3.connect(self.path) as conn:
                 cursor = conn.cursor()
                 cursor.execute(SQL_QUERY)
                 conn.commit()
         except sqlite3.OperationalError as e:
-            self.logger.debug(f"Mirgration already run: {e}")
+            self.logger.info(f"Mirgration already run: {e}")
             return False
```

### Comparing `chronus-0.3.8/chronus/SystemIntegration/settings_interface/etc_storage.py` & `chronus-0.3.9/chronus/SystemIntegration/settings_interface/etc_storage.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.8/chronus/SystemIntegration/system_service_interfaces/ipmi_system_service.py` & `chronus-0.3.9/chronus/SystemIntegration/system_service_interfaces/ipmi_system_service.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.8/chronus/__main__.py` & `chronus-0.3.9/chronus/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,27 +42,21 @@
     yellow = "yellow"
     green = "green"
 
 
 class FileWithTimeStampHandlerAndLevel(logging.FileHandler):
     def emit(self, record: logging.LogRecord) -> None:
         from datetime import datetime
-
         record.msg = f"[{datetime.now().strftime('%H:%M:%S')}] {record.levelname: <7} {record.msg}"
         super().emit(record)
 
 
 console = Console()
 FORMAT = "%(message)s"
-logging.basicConfig(
-    level="INFO",
-    format=FORMAT,
-    datefmt="[%X]",
-    handlers=[RichHandler(), FileWithTimeStampHandlerAndLevel("chronus.log")],
-)
+logging.basicConfig(level="INFO", format=FORMAT, datefmt="[%X]", handlers=[RichHandler(), FileWithTimeStampHandlerAndLevel("chronus.log")])
 
 app = typer.Typer(
     name=name,
     help="A energy scheduling model, build for HPC.",
     add_completion=True,
 )
```

### Comparing `chronus-0.3.8/chronus/application/benchmark_service.py` & `chronus-0.3.9/chronus/application/benchmark_service.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.8/chronus/application/init_model_service.py` & `chronus-0.3.9/chronus/application/init_model_service.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.8/chronus/application/load_model_service.py` & `chronus-0.3.9/chronus/application/load_model_service.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.8/chronus/application/run_model_service.py` & `chronus-0.3.9/chronus/application/run_model_service.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.8/chronus/cli/setup.py` & `chronus-0.3.9/chronus/cli/setup.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.8/chronus/domain/Run.py` & `chronus-0.3.9/chronus/domain/Run.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.8/chronus/domain/configuration.py` & `chronus-0.3.9/chronus/domain/configuration.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.8/chronus/domain/cpu_info.py` & `chronus-0.3.9/chronus/domain/cpu_info.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.8/chronus/domain/interfaces/application_runner_interface.py` & `chronus-0.3.9/chronus/domain/interfaces/application_runner_interface.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.8/chronus/domain/interfaces/optimizer_interface.py` & `chronus-0.3.9/chronus/domain/interfaces/optimizer_interface.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.8/chronus/domain/interfaces/repository_interface.py` & `chronus-0.3.9/chronus/domain/interfaces/repository_interface.py`

 * *Files identical despite different names*

### Comparing `chronus-0.3.8/pyproject.toml` & `chronus-0.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "chronus"
-version = "0.3.8"
+version = "0.3.9"
 description = "A energy scheduling model, build for HPC."
 readme = "README.md"
 authors = ["chronus <aaspringborg@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/AndersSpringborg/chronus"
 homepage = "https://github.com/AndersSpringborg/chronus"
```

### Comparing `chronus-0.3.8/PKG-INFO` & `chronus-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chronus
-Version: 0.3.8
+Version: 0.3.9
 Summary: A energy scheduling model, build for HPC.
 Home-page: https://github.com/AndersSpringborg/chronus
 License: MIT
 Author: chronus
 Author-email: aaspringborg@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
```

