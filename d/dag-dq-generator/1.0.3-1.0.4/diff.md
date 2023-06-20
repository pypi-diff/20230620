# Comparing `tmp/dag-dq-generator-1.0.3.tar.gz` & `tmp/dag-dq-generator-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dag-dq-generator-1.0.3.tar", last modified: Sat May 27 18:20:32 2023, max compression
+gzip compressed data, was "dist/dag-dq-generator-1.0.4.tar", last modified: Tue Jun 20 19:45:26 2023, max compression
```

## Comparing `dag-dq-generator-1.0.3.tar` & `dag-dq-generator-1.0.4.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-05-27 18:20:32.841430 dag-dq-generator-1.0.3/
--rw-r--r--   0 hnankam    (501) staff       (20)     1874 2023-05-27 18:18:39.000000 dag-dq-generator-1.0.3/CHANGELOG.md
--rw-r--r--   0 hnankam    (501) staff       (20)     1080 2022-08-03 15:58:08.000000 dag-dq-generator-1.0.3/LICENSE
--rw-r--r--   0 hnankam    (501) staff       (20)      133 2022-09-19 21:54:41.000000 dag-dq-generator-1.0.3/MANIFEST.in
--rw-r--r--   0 hnankam    (501) staff       (20)     2292 2023-05-27 18:20:32.841167 dag-dq-generator-1.0.3/PKG-INFO
--rw-r--r--   0 hnankam    (501) staff       (20)     1382 2023-05-10 03:45:14.000000 dag-dq-generator-1.0.3/README.md
-drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-05-27 18:20:32.835477 dag-dq-generator-1.0.3/dag_dq_generator/
--rw-r--r--   0 hnankam    (501) staff       (20)       74 2022-09-19 21:34:24.000000 dag-dq-generator-1.0.3/dag_dq_generator/__init__.py
-drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-05-27 18:20:32.838253 dag-dq-generator-1.0.3/dag_dq_generator/__pycache__/
--rw-r--r--   0 hnankam    (501) staff       (20)      226 2022-09-21 21:25:09.000000 dag-dq-generator-1.0.3/dag_dq_generator/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 hnankam    (501) staff       (20)      154 2022-09-21 21:25:09.000000 dag-dq-generator-1.0.3/dag_dq_generator/__pycache__/__version__.cpython-38.pyc
--rw-r--r--   0 hnankam    (501) staff       (20)       90 2023-05-26 15:14:47.000000 dag-dq-generator-1.0.3/dag_dq_generator/__version__.py
-drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-05-27 18:20:32.838843 dag-dq-generator-1.0.3/dag_dq_generator/configs/
--rw-r--r--   0 hnankam    (501) staff       (20)     6537 2022-11-09 02:56:39.000000 dag-dq-generator-1.0.3/dag_dq_generator/configs/sample.yml
--rw-r--r--   0 hnankam    (501) staff       (20)     3383 2022-11-04 20:33:28.000000 dag-dq-generator-1.0.3/dag_dq_generator/configs/stage_sample.yml
--rw-r--r--   0 hnankam    (501) staff       (20)    11298 2023-05-26 15:13:19.000000 dag-dq-generator-1.0.3/dag_dq_generator/dag_generator.py
-drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-05-27 18:20:32.839505 dag-dq-generator-1.0.3/dag_dq_generator/dags/
--rw-r--r--   0 hnankam    (501) staff       (20)    16788 2022-09-19 18:50:06.000000 dag-dq-generator-1.0.3/dag_dq_generator/dags/demo-dev-01.py
--rw-r--r--   0 hnankam    (501) staff       (20)     8727 2022-09-19 18:50:06.000000 dag-dq-generator-1.0.3/dag_dq_generator/dags/stage_test_001.py
-drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-05-27 18:20:32.840449 dag-dq-generator-1.0.3/dag_dq_generator/templates/
--rw-r--r--   0 hnankam    (501) staff       (20)     7482 2023-05-17 22:52:00.000000 dag-dq-generator-1.0.3/dag_dq_generator/templates/_global_macros.py
--rw-r--r--   0 hnankam    (501) staff       (20)    17900 2023-05-17 22:49:36.000000 dag-dq-generator-1.0.3/dag_dq_generator/templates/dag_template.py
--rw-r--r--   0 hnankam    (501) staff       (20)    17835 2023-05-26 15:01:56.000000 dag-dq-generator-1.0.3/dag_dq_generator/templates/dq_sql_template.sql
-drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-05-27 18:20:32.840819 dag-dq-generator-1.0.3/dag_dq_generator/tests/
--rw-r--r--   0 hnankam    (501) staff       (20)        0 2022-09-19 18:15:00.000000 dag-dq-generator-1.0.3/dag_dq_generator/tests/__init__.py
-drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-05-27 18:20:32.837655 dag-dq-generator-1.0.3/dag_dq_generator.egg-info/
--rw-r--r--   0 hnankam    (501) staff       (20)     2292 2023-05-27 18:20:32.000000 dag-dq-generator-1.0.3/dag_dq_generator.egg-info/PKG-INFO
--rw-r--r--   0 hnankam    (501) staff       (20)      878 2023-05-27 18:20:32.000000 dag-dq-generator-1.0.3/dag_dq_generator.egg-info/SOURCES.txt
--rw-r--r--   0 hnankam    (501) staff       (20)        1 2023-05-27 18:20:32.000000 dag-dq-generator-1.0.3/dag_dq_generator.egg-info/dependency_links.txt
--rw-r--r--   0 hnankam    (501) staff       (20)       71 2023-05-27 18:20:32.000000 dag-dq-generator-1.0.3/dag_dq_generator.egg-info/entry_points.txt
--rw-r--r--   0 hnankam    (501) staff       (20)        1 2022-09-20 16:35:26.000000 dag-dq-generator-1.0.3/dag_dq_generator.egg-info/not-zip-safe
--rw-r--r--   0 hnankam    (501) staff       (20)      125 2023-05-27 18:20:32.000000 dag-dq-generator-1.0.3/dag_dq_generator.egg-info/requires.txt
--rw-r--r--   0 hnankam    (501) staff       (20)       17 2023-05-27 18:20:32.000000 dag-dq-generator-1.0.3/dag_dq_generator.egg-info/top_level.txt
--rw-r--r--   0 hnankam    (501) staff       (20)      124 2023-05-13 17:36:49.000000 dag-dq-generator-1.0.3/requirements.txt
--rw-r--r--   0 hnankam    (501) staff       (20)       38 2023-05-27 18:20:32.841522 dag-dq-generator-1.0.3/setup.cfg
--rw-r--r--   0 hnankam    (501) staff       (20)     1632 2023-05-17 22:52:05.000000 dag-dq-generator-1.0.3/setup.py
+drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-06-20 19:45:26.243478 dag-dq-generator-1.0.4/
+-rw-r--r--   0 hnankam    (501) staff       (20)     1874 2023-05-27 18:18:39.000000 dag-dq-generator-1.0.4/CHANGELOG.md
+-rw-r--r--   0 hnankam    (501) staff       (20)     1080 2022-08-03 15:58:08.000000 dag-dq-generator-1.0.4/LICENSE
+-rw-r--r--   0 hnankam    (501) staff       (20)      133 2022-09-19 21:54:41.000000 dag-dq-generator-1.0.4/MANIFEST.in
+-rw-r--r--   0 hnankam    (501) staff       (20)     2292 2023-06-20 19:45:26.243022 dag-dq-generator-1.0.4/PKG-INFO
+-rw-r--r--   0 hnankam    (501) staff       (20)     1382 2023-05-10 03:45:14.000000 dag-dq-generator-1.0.4/README.md
+drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-06-20 19:45:26.234092 dag-dq-generator-1.0.4/dag_dq_generator/
+-rw-r--r--   0 hnankam    (501) staff       (20)       74 2022-09-19 21:34:24.000000 dag-dq-generator-1.0.4/dag_dq_generator/__init__.py
+drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-06-20 19:45:26.237427 dag-dq-generator-1.0.4/dag_dq_generator/__pycache__/
+-rw-r--r--   0 hnankam    (501) staff       (20)      226 2022-09-21 21:25:09.000000 dag-dq-generator-1.0.4/dag_dq_generator/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 hnankam    (501) staff       (20)      154 2022-09-21 21:25:09.000000 dag-dq-generator-1.0.4/dag_dq_generator/__pycache__/__version__.cpython-38.pyc
+-rw-r--r--   0 hnankam    (501) staff       (20)       90 2023-06-20 19:41:30.000000 dag-dq-generator-1.0.4/dag_dq_generator/__version__.py
+drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-06-20 19:45:26.238565 dag-dq-generator-1.0.4/dag_dq_generator/configs/
+-rw-r--r--   0 hnankam    (501) staff       (20)     6537 2022-11-09 02:56:39.000000 dag-dq-generator-1.0.4/dag_dq_generator/configs/sample.yml
+-rw-r--r--   0 hnankam    (501) staff       (20)     3383 2022-11-04 20:33:28.000000 dag-dq-generator-1.0.4/dag_dq_generator/configs/stage_sample.yml
+-rw-r--r--   0 hnankam    (501) staff       (20)    11298 2023-05-26 15:13:19.000000 dag-dq-generator-1.0.4/dag_dq_generator/dag_generator.py
+drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-06-20 19:45:26.239696 dag-dq-generator-1.0.4/dag_dq_generator/dags/
+-rw-r--r--   0 hnankam    (501) staff       (20)    16788 2022-09-19 18:50:06.000000 dag-dq-generator-1.0.4/dag_dq_generator/dags/demo-dev-01.py
+-rw-r--r--   0 hnankam    (501) staff       (20)     8727 2022-09-19 18:50:06.000000 dag-dq-generator-1.0.4/dag_dq_generator/dags/stage_test_001.py
+drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-06-20 19:45:26.241869 dag-dq-generator-1.0.4/dag_dq_generator/templates/
+-rw-r--r--   0 hnankam    (501) staff       (20)     7486 2023-06-20 19:39:48.000000 dag-dq-generator-1.0.4/dag_dq_generator/templates/_global_macros.py
+-rw-r--r--   0 hnankam    (501) staff       (20)    17900 2023-05-17 22:49:36.000000 dag-dq-generator-1.0.4/dag_dq_generator/templates/dag_template.py
+-rw-r--r--   0 hnankam    (501) staff       (20)    33344 2023-06-20 15:47:02.000000 dag-dq-generator-1.0.4/dag_dq_generator/templates/dq-anomaly-detector.py
+-rw-r--r--   0 hnankam    (501) staff       (20)    17835 2023-05-26 15:01:56.000000 dag-dq-generator-1.0.4/dag_dq_generator/templates/dq_sql_template.sql
+drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-06-20 19:45:26.242429 dag-dq-generator-1.0.4/dag_dq_generator/tests/
+-rw-r--r--   0 hnankam    (501) staff       (20)        0 2022-09-19 18:15:00.000000 dag-dq-generator-1.0.4/dag_dq_generator/tests/__init__.py
+drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-06-20 19:45:26.236411 dag-dq-generator-1.0.4/dag_dq_generator.egg-info/
+-rw-r--r--   0 hnankam    (501) staff       (20)     2292 2023-06-20 19:45:26.000000 dag-dq-generator-1.0.4/dag_dq_generator.egg-info/PKG-INFO
+-rw-r--r--   0 hnankam    (501) staff       (20)      928 2023-06-20 19:45:26.000000 dag-dq-generator-1.0.4/dag_dq_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 hnankam    (501) staff       (20)        1 2023-06-20 19:45:26.000000 dag-dq-generator-1.0.4/dag_dq_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 hnankam    (501) staff       (20)       71 2023-06-20 19:45:26.000000 dag-dq-generator-1.0.4/dag_dq_generator.egg-info/entry_points.txt
+-rw-r--r--   0 hnankam    (501) staff       (20)        1 2022-09-20 16:35:26.000000 dag-dq-generator-1.0.4/dag_dq_generator.egg-info/not-zip-safe
+-rw-r--r--   0 hnankam    (501) staff       (20)      125 2023-06-20 19:45:26.000000 dag-dq-generator-1.0.4/dag_dq_generator.egg-info/requires.txt
+-rw-r--r--   0 hnankam    (501) staff       (20)       17 2023-06-20 19:45:26.000000 dag-dq-generator-1.0.4/dag_dq_generator.egg-info/top_level.txt
+-rw-r--r--   0 hnankam    (501) staff       (20)      124 2023-05-13 17:36:49.000000 dag-dq-generator-1.0.4/requirements.txt
+-rw-r--r--   0 hnankam    (501) staff       (20)       38 2023-06-20 19:45:26.243633 dag-dq-generator-1.0.4/setup.cfg
+-rw-r--r--   0 hnankam    (501) staff       (20)     1632 2023-05-17 22:52:05.000000 dag-dq-generator-1.0.4/setup.py
```

### Comparing `dag-dq-generator-1.0.3/CHANGELOG.md` & `dag-dq-generator-1.0.4/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `dag-dq-generator-1.0.3/LICENSE` & `dag-dq-generator-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dag-dq-generator-1.0.3/PKG-INFO` & `dag-dq-generator-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dag-dq-generator
-Version: 1.0.3
+Version: 1.0.4
 Summary: DPaaS Airflow DAG (Dynamic Acyclic Graph) and DQ (Data Quality) generator
 Home-page: https://git.corp.adobe.com/ccea/dag-dq-generator
 Author: CI DMe Data Engineering
 Author-email: ccea-data-engineering@adobe.com
 License: MIT
 Description: # dag-dq-generator
         DPaaS Airflow DAG (Dynamic Acyclic Graph) and DQ (Data Quality) generator.
```

### Comparing `dag-dq-generator-1.0.3/README.md` & `dag-dq-generator-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `dag-dq-generator-1.0.3/dag_dq_generator/configs/sample.yml` & `dag-dq-generator-1.0.4/dag_dq_generator/configs/sample.yml`

 * *Files identical despite different names*

### Comparing `dag-dq-generator-1.0.3/dag_dq_generator/configs/stage_sample.yml` & `dag-dq-generator-1.0.4/dag_dq_generator/configs/stage_sample.yml`

 * *Files identical despite different names*

### Comparing `dag-dq-generator-1.0.3/dag_dq_generator/dag_generator.py` & `dag-dq-generator-1.0.4/dag_dq_generator/dag_generator.py`

 * *Files identical despite different names*

### Comparing `dag-dq-generator-1.0.3/dag_dq_generator/dags/demo-dev-01.py` & `dag-dq-generator-1.0.4/dag_dq_generator/dags/demo-dev-01.py`

 * *Files identical despite different names*

### Comparing `dag-dq-generator-1.0.3/dag_dq_generator/dags/stage_test_001.py` & `dag-dq-generator-1.0.4/dag_dq_generator/dags/stage_test_001.py`

 * *Files identical despite different names*

### Comparing `dag-dq-generator-1.0.3/dag_dq_generator/templates/_global_macros.py` & `dag-dq-generator-1.0.4/dag_dq_generator/templates/_global_macros.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
             task_id='{{task.task_id}}_check',
             on_success_callback=_task_on_success_callback,
             **{{task.task_id}}_args
         )
         
         {{task.task_id}}_check = ShortCircuitOperator(
             task_id='{{task.task_id}}_check_chk',
-            op_kwargs={'sql_task_id': '{{tasks_groups_str}}.{{group.group_name}}.{{task.task_id}}.{{task.task_id}}_check', 'sql_task_args': {{task.task_id}}_args},
+            op_kwargs={'sql_task_id': '{{tasks_groups_str}}.{{group.group_name}}.{{task.task_id}}_chk.{{task.task_id}}_check', 'sql_task_args': {{task.task_id}}_args},
             ignore_downstream_trigger_rules=False,
             python_callable=_verify_check_response,
         )
 
         {{task.task_id}}_run = _task_id
 
         {{task.task_id}}_qry >> {{task.task_id}}_check >> {{task.task_id}}_run
```

### Comparing `dag-dq-generator-1.0.3/dag_dq_generator/templates/dag_template.py` & `dag-dq-generator-1.0.4/dag_dq_generator/templates/dag_template.py`

 * *Files identical despite different names*

### Comparing `dag-dq-generator-1.0.3/dag_dq_generator/templates/dq_sql_template.sql` & `dag-dq-generator-1.0.4/dag_dq_generator/templates/dq_sql_template.sql`

 * *Files identical despite different names*

### Comparing `dag-dq-generator-1.0.3/dag_dq_generator.egg-info/PKG-INFO` & `dag-dq-generator-1.0.4/dag_dq_generator.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dag-dq-generator
-Version: 1.0.3
+Version: 1.0.4
 Summary: DPaaS Airflow DAG (Dynamic Acyclic Graph) and DQ (Data Quality) generator
 Home-page: https://git.corp.adobe.com/ccea/dag-dq-generator
 Author: CI DMe Data Engineering
 Author-email: ccea-data-engineering@adobe.com
 License: MIT
 Description: # dag-dq-generator
         DPaaS Airflow DAG (Dynamic Acyclic Graph) and DQ (Data Quality) generator.
```

### Comparing `dag-dq-generator-1.0.3/dag_dq_generator.egg-info/SOURCES.txt` & `dag-dq-generator-1.0.4/dag_dq_generator.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,9 +18,10 @@
 dag_dq_generator/__pycache__/__version__.cpython-38.pyc
 dag_dq_generator/configs/sample.yml
 dag_dq_generator/configs/stage_sample.yml
 dag_dq_generator/dags/demo-dev-01.py
 dag_dq_generator/dags/stage_test_001.py
 dag_dq_generator/templates/_global_macros.py
 dag_dq_generator/templates/dag_template.py
+dag_dq_generator/templates/dq-anomaly-detector.py
 dag_dq_generator/templates/dq_sql_template.sql
 dag_dq_generator/tests/__init__.py
```

### Comparing `dag-dq-generator-1.0.3/setup.py` & `dag-dq-generator-1.0.4/setup.py`

 * *Files identical despite different names*

