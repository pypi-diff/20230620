# Comparing `tmp/globus-compute-endpoint-2.1.0a1.tar.gz` & `tmp/globus-compute-endpoint-2.2.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globus-compute-endpoint-2.1.0a1.tar", last modified: Tue May 23 18:47:21 2023, max compression
+gzip compressed data, was "globus-compute-endpoint-2.2.0a0.tar", last modified: Tue Jun 20 18:07:15 2023, max compression
```

## Comparing `globus-compute-endpoint-2.1.0a1.tar` & `globus-compute-endpoint-2.2.0a0.tar`

### file list

```diff
@@ -1,77 +1,81 @@
-drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:21.543599 globus-compute-endpoint-2.1.0a1/
--rw-rw-r--   0 reid      (1000) reid      (1000)    11330 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/LICENSE
--rw-rw-r--   0 reid      (1000) reid      (1000)       16 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/MANIFEST.in
--rw-rw-r--   0 reid      (1000) reid      (1000)     1840 2023-05-23 18:47:21.543599 globus-compute-endpoint-2.1.0a1/PKG-INFO
--rw-rw-r--   0 reid      (1000) reid      (1000)      871 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/PyPI.md
-drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:21.535599 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/
--rw-rw-r--   0 reid      (1000) reid      (1000)      131 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/__init__.py
--rw-rw-r--   0 reid      (1000) reid      (1000)    19439 2023-05-23 18:23:02.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/cli.py
-drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:21.535599 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/
--rw-rw-r--   0 reid      (1000) reid      (1000)        0 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/__init__.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     2895 2023-05-22 19:56:07.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/config.py
--rw-rw-r--   0 reid      (1000) reid      (1000)      772 2023-05-22 19:56:07.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/default_config.py
--rw-rw-r--   0 reid      (1000) reid      (1000)    28831 2023-05-23 18:23:02.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/endpoint.py
--rw-rw-r--   0 reid      (1000) reid      (1000)    19658 2023-05-22 19:56:07.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/endpoint_manager.py
--rw-rw-r--   0 reid      (1000) reid      (1000)    24838 2023-05-22 19:56:07.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/interchange.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     2773 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/messages_compat.py
-drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:21.539599 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/rabbit_mq/
--rw-rw-r--   0 reid      (1000) reid      (1000)      307 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/rabbit_mq/__init__.py
--rw-rw-r--   0 reid      (1000) reid      (1000)      689 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/rabbit_mq/base.py
--rw-rw-r--   0 reid      (1000) reid      (1000)    11834 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     3068 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py
--rw-rw-r--   0 reid      (1000) reid      (1000)    14076 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     5184 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/result_store.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     7275 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/taskqueue.py
-drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:21.539599 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/utils/
--rw-rw-r--   0 reid      (1000) reid      (1000)     1017 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/utils/__init__.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     6129 2023-05-22 19:56:07.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/utils/config.py
-drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:21.539599 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/engines/
--rw-rw-r--   0 reid      (1000) reid      (1000)      318 2023-05-08 18:31:13.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/engines/__init__.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     5954 2023-05-08 18:31:13.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/engines/base.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     3721 2023-05-11 19:15:28.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/engines/globus_compute.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     4336 2023-05-08 18:31:13.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/engines/helper.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     3721 2023-05-11 19:15:28.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/engines/process_pool.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     3715 2023-05-11 19:15:28.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/engines/thread_pool.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     1834 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/exception_handling.py
--rw-rw-r--   0 reid      (1000) reid      (1000)      220 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/exceptions.py
-drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:21.539599 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/
--rw-rw-r--   0 reid      (1000) reid      (1000)      141 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/__init__.py
-drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:21.539599 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/high_throughput/
--rw-rw-r--   0 reid      (1000) reid      (1000)        0 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/high_throughput/__init__.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     1943 2023-05-01 20:50:52.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/high_throughput/container_sched.py
--rw-rw-r--   0 reid      (1000) reid      (1000)    35357 2023-05-16 23:00:07.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/high_throughput/executor.py
--rw-rw-r--   0 reid      (1000) reid      (1000)    50314 2023-05-11 19:15:28.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/high_throughput/interchange.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     9712 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py
--rw-rw-r--   0 reid      (1000) reid      (1000)      267 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/high_throughput/mac_safe_queue.py
--rwxrwxr-x   0 reid      (1000) reid      (1000)    36129 2023-05-11 19:15:28.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/high_throughput/manager.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     9114 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/high_throughput/messages.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     8683 2023-04-20 18:06:21.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/high_throughput/worker.py
--rw-rw-r--   0 reid      (1000) reid      (1000)    19094 2023-05-01 20:50:52.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/high_throughput/worker_map.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     5433 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     8219 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/logging_config.py
-drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:21.539599 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/providers/
--rw-rw-r--   0 reid      (1000) reid      (1000)      115 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/providers/__init__.py
-drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:21.543599 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/providers/kubernetes/
--rw-rw-r--   0 reid      (1000) reid      (1000)        0 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/providers/kubernetes/__init__.py
--rw-rw-r--   0 reid      (1000) reid      (1000)    12926 2023-05-01 20:50:52.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/providers/kubernetes/kube.py
--rw-rw-r--   0 reid      (1000) reid      (1000)       50 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/providers/kubernetes/template.py
-drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:21.543599 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/strategies/
--rw-rw-r--   0 reid      (1000) reid      (1000)      280 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/strategies/__init__.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     7018 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/strategies/base.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     5470 2023-05-01 20:50:52.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/strategies/kube_simple.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     6145 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/strategies/simple.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     1610 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/strategies/test.py
--rw-rw-r--   0 reid      (1000) reid      (1000)      806 2023-05-23 18:46:22.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/version.py
-drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:21.535599 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint.egg-info/
--rw-rw-r--   0 reid      (1000) reid      (1000)     1840 2023-05-23 18:47:21.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint.egg-info/PKG-INFO
--rw-rw-r--   0 reid      (1000) reid      (1000)     2928 2023-05-23 18:47:21.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint.egg-info/SOURCES.txt
--rw-rw-r--   0 reid      (1000) reid      (1000)        1 2023-05-23 18:47:21.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint.egg-info/dependency_links.txt
--rw-rw-r--   0 reid      (1000) reid      (1000)      359 2023-05-23 18:47:21.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint.egg-info/entry_points.txt
--rw-rw-r--   0 reid      (1000) reid      (1000)      308 2023-05-23 18:47:21.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint.egg-info/requires.txt
--rw-rw-r--   0 reid      (1000) reid      (1000)       30 2023-05-23 18:47:21.000000 globus-compute-endpoint-2.1.0a1/globus_compute_endpoint.egg-info/top_level.txt
--rw-rw-r--   0 reid      (1000) reid      (1000)      282 2023-05-23 18:47:21.543599 globus-compute-endpoint-2.1.0a1/setup.cfg
--rw-rw-r--   0 reid      (1000) reid      (1000)     3635 2023-05-23 18:46:19.000000 globus-compute-endpoint-2.1.0a1/setup.py
-drwxrwxr-x   0 reid      (1000) reid      (1000)        0 2023-05-23 18:47:21.543599 globus-compute-endpoint-2.1.0a1/tests/
--rw-rw-r--   0 reid      (1000) reid      (1000)        0 2023-04-19 22:57:38.000000 globus-compute-endpoint-2.1.0a1/tests/__init__.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     2709 2023-05-01 20:50:52.000000 globus-compute-endpoint-2.1.0a1/tests/conftest.py
--rw-rw-r--   0 reid      (1000) reid      (1000)     2925 2023-05-08 18:31:13.000000 globus-compute-endpoint-2.1.0a1/tests/utils.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-20 18:07:15.087910 globus-compute-endpoint-2.2.0a0/
+-rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/LICENSE
+-rw-r--r--   0 lei        (501) staff       (20)       16 2023-04-20 03:21:56.000000 globus-compute-endpoint-2.2.0a0/MANIFEST.in
+-rw-r--r--   0 lei        (501) staff       (20)     1840 2023-06-20 18:07:15.087990 globus-compute-endpoint-2.2.0a0/PKG-INFO
+-rw-r--r--   0 lei        (501) staff       (20)      871 2023-04-20 03:21:56.000000 globus-compute-endpoint-2.2.0a0/PyPI.md
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-20 18:07:15.075462 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/
+-rw-r--r--   0 lei        (501) staff       (20)      131 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)    16673 2023-06-13 20:34:26.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/cli.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-20 18:07:15.077930 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/__init__.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-20 18:07:15.078953 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/config/
+-rw-r--r--   0 lei        (501) staff       (20)       41 2023-06-13 18:28:48.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/config/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     6129 2023-06-13 18:28:48.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/config/config.py
+-rw-r--r--   0 lei        (501) staff       (20)      766 2023-06-13 18:28:48.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/config/default_config.py
+-rw-r--r--   0 lei        (501) staff       (20)     3448 2023-06-20 16:40:24.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/config/model.py
+-rw-r--r--   0 lei        (501) staff       (20)     7326 2023-06-13 20:34:26.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/config/utils.py
+-rw-r--r--   0 lei        (501) staff       (20)    26645 2023-06-13 18:28:48.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/endpoint.py
+-rw-r--r--   0 lei        (501) staff       (20)    20355 2023-06-13 20:34:26.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/endpoint_manager.py
+-rw-r--r--   0 lei        (501) staff       (20)    24826 2023-06-20 16:39:53.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/interchange.py
+-rw-r--r--   0 lei        (501) staff       (20)     2773 2023-05-01 15:02:38.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/messages_compat.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-20 18:07:15.079869 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/rabbit_mq/
+-rw-r--r--   0 lei        (501) staff       (20)      307 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/rabbit_mq/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)      689 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/rabbit_mq/base.py
+-rw-r--r--   0 lei        (501) staff       (20)    11834 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py
+-rw-r--r--   0 lei        (501) staff       (20)     3068 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py
+-rw-r--r--   0 lei        (501) staff       (20)    14076 2023-06-20 16:39:53.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py
+-rw-r--r--   0 lei        (501) staff       (20)     5184 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/result_store.py
+-rw-r--r--   0 lei        (501) staff       (20)     7275 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/taskqueue.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-20 18:07:15.080215 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/utils/
+-rw-r--r--   0 lei        (501) staff       (20)     1017 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/utils/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)      110 2023-06-13 18:28:48.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/utils/config.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-20 18:07:15.081621 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/engines/
+-rw-r--r--   0 lei        (501) staff       (20)      318 2023-05-05 16:40:44.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/engines/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     5954 2023-05-05 16:40:44.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/engines/base.py
+-rw-r--r--   0 lei        (501) staff       (20)     3721 2023-05-11 20:01:33.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/engines/globus_compute.py
+-rw-r--r--   0 lei        (501) staff       (20)     4336 2023-05-05 16:40:44.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/engines/helper.py
+-rw-r--r--   0 lei        (501) staff       (20)     3721 2023-05-11 20:01:33.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/engines/process_pool.py
+-rw-r--r--   0 lei        (501) staff       (20)     3715 2023-05-11 20:01:33.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/engines/thread_pool.py
+-rw-r--r--   0 lei        (501) staff       (20)     1834 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/exception_handling.py
+-rw-r--r--   0 lei        (501) staff       (20)      220 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/exceptions.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-20 18:07:15.081785 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/
+-rw-r--r--   0 lei        (501) staff       (20)      141 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/__init__.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-20 18:07:15.085518 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/high_throughput/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/high_throughput/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     1943 2023-05-01 18:50:06.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/high_throughput/container_sched.py
+-rw-r--r--   0 lei        (501) staff       (20)    35357 2023-04-20 15:03:07.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/high_throughput/executor.py
+-rw-r--r--   0 lei        (501) staff       (20)    50314 2023-06-06 16:42:30.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/high_throughput/interchange.py
+-rw-r--r--   0 lei        (501) staff       (20)     9712 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py
+-rw-r--r--   0 lei        (501) staff       (20)      267 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/high_throughput/mac_safe_queue.py
+-rwxr-xr-x   0 lei        (501) staff       (20)    36129 2023-05-08 21:54:40.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/high_throughput/manager.py
+-rw-r--r--   0 lei        (501) staff       (20)     9114 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/high_throughput/messages.py
+-rw-r--r--   0 lei        (501) staff       (20)     8683 2023-04-21 16:13:24.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/high_throughput/worker.py
+-rw-r--r--   0 lei        (501) staff       (20)    19094 2023-05-01 18:50:06.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/high_throughput/worker_map.py
+-rw-r--r--   0 lei        (501) staff       (20)     5433 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py
+-rw-r--r--   0 lei        (501) staff       (20)     8219 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/logging_config.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-20 18:07:15.085755 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/providers/
+-rw-r--r--   0 lei        (501) staff       (20)      115 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/providers/__init__.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-20 18:07:15.086326 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/providers/kubernetes/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/providers/kubernetes/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)    12926 2023-05-01 18:50:06.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/providers/kubernetes/kube.py
+-rw-r--r--   0 lei        (501) staff       (20)       50 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/providers/kubernetes/template.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-20 18:07:15.087150 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/strategies/
+-rw-r--r--   0 lei        (501) staff       (20)      280 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/strategies/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     7018 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/strategies/base.py
+-rw-r--r--   0 lei        (501) staff       (20)     5470 2023-05-01 18:50:06.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/strategies/kube_simple.py
+-rw-r--r--   0 lei        (501) staff       (20)     6145 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/strategies/simple.py
+-rw-r--r--   0 lei        (501) staff       (20)     1610 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/strategies/test.py
+-rw-r--r--   0 lei        (501) staff       (20)      806 2023-06-20 17:58:38.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/version.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-20 18:07:15.076163 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint.egg-info/
+-rw-r--r--   0 lei        (501) staff       (20)     1840 2023-06-20 18:07:15.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint.egg-info/PKG-INFO
+-rw-r--r--   0 lei        (501) staff       (20)     3092 2023-06-20 18:07:15.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint.egg-info/SOURCES.txt
+-rw-r--r--   0 lei        (501) staff       (20)        1 2023-06-20 18:07:15.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint.egg-info/dependency_links.txt
+-rw-r--r--   0 lei        (501) staff       (20)      359 2023-06-20 18:07:15.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint.egg-info/entry_points.txt
+-rw-r--r--   0 lei        (501) staff       (20)      344 2023-06-20 18:07:15.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint.egg-info/requires.txt
+-rw-r--r--   0 lei        (501) staff       (20)       30 2023-06-20 18:07:15.000000 globus-compute-endpoint-2.2.0a0/globus_compute_endpoint.egg-info/top_level.txt
+-rw-r--r--   0 lei        (501) staff       (20)      282 2023-06-20 18:07:15.088238 globus-compute-endpoint-2.2.0a0/setup.cfg
+-rw-r--r--   0 lei        (501) staff       (20)     3685 2023-06-20 17:58:29.000000 globus-compute-endpoint-2.2.0a0/setup.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-06-20 18:07:15.087677 globus-compute-endpoint-2.2.0a0/tests/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.2.0a0/tests/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     2709 2023-04-24 21:22:25.000000 globus-compute-endpoint-2.2.0a0/tests/conftest.py
+-rw-r--r--   0 lei        (501) staff       (20)     2925 2023-05-05 16:40:44.000000 globus-compute-endpoint-2.2.0a0/tests/utils.py
```

### Comparing `globus-compute-endpoint-2.1.0a1/LICENSE` & `globus-compute-endpoint-2.2.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a1/PKG-INFO` & `globus-compute-endpoint-2.2.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-endpoint
-Version: 2.1.0a1
+Version: 2.2.0a0
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `globus-compute-endpoint-2.1.0a1/PyPI.md` & `globus-compute-endpoint-2.2.0a0/PyPI.md`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/cli.py` & `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 from __future__ import annotations
 
 import difflib
-import importlib.util
 import json
 import logging
 import pathlib
 import shutil
 import sys
 import uuid
 
 import click
 from click import ClickException
+from globus_compute_endpoint.endpoint.config.utils import get_config, load_config_yaml
 from globus_compute_endpoint.endpoint.endpoint import Endpoint
 from globus_compute_endpoint.endpoint.endpoint_manager import EndpointManager
-from globus_compute_endpoint.endpoint.utils.config import Config
 from globus_compute_endpoint.logging_config import setup_logging
 from globus_compute_endpoint.version import DEPRECATION_FUNCX_ENDPOINT
 from globus_compute_sdk.sdk.login_manager import LoginManager
 from globus_compute_sdk.sdk.login_manager.tokenstore import ensure_compute_dir
 from globus_compute_sdk.sdk.login_manager.whoami import print_whoami_info
-from packaging.version import Version
 
 log = logging.getLogger(__name__)
 
 
 class CommandState:
     def __init__(self):
         self.endpoint_config_dir: pathlib.Path = init_config_dir()
@@ -119,15 +117,31 @@
         hidden=True,
         callback=set_param_to_config,
         help="Shutdown if parent process goes away",
     )(f)
     return f
 
 
+def verify_not_uuid(ctx, param, value):
+    try:
+        uuid.UUID(value)
+        raise click.BadParameter(
+            "Specifying an UUID for endpoint commands is not currently supported"
+        )
+    except ValueError:
+        return value
+
+
 def name_arg(f):
+    return click.argument(
+        "name", required=False, callback=verify_not_uuid, default="default"
+    )(f)
+
+
+def name_arg_allow_uuid(f):
     return click.argument("name", required=False, default="default")(f)
 
 
 def config_dir_callback(ctx, param, value):
     if value is None or ctx.resilient_parsing:
         return
     state = CommandState.ensure()
@@ -178,16 +192,16 @@
     name: str,
     endpoint_config: str | None,
     multi_tenant: bool,
     display_name: str | None,
 ):
     """Configure an endpoint
 
-    Drops a config.py template into the Globus Compute configs directory.
-    The template usually goes to ~/.globus_compute/<ENDPOINT_NAME>/config.py
+    Drops a config.yaml template into the Globus Compute configs directory.
+    The template usually goes to ~/.globus_compute/<ENDPOINT_NAME>/config.yaml
     """
     try:
         Endpoint.validate_endpoint_name(name)
     except ValueError as e:
         raise ClickException(str(e))
     compute_dir = get_config_dir()
     ep_dir = compute_dir / name
@@ -287,15 +301,15 @@
         else:
             error_msg = "No cached tokens were found, already logged out?"
             log.info(error_msg)
     return tokens_revoked, error_msg
 
 
 FUNCX_COMPUTE_IMPORT_UPDATES = {
-    "from funcx_endpoint.endpoint.utils.config": "from globus_compute_endpoint.endpoint.utils.config",  # noqa E501
+    "from funcx_endpoint.endpoint.utils.config": "from globus_compute_endpoint.endpoint.config",  # noqa E501
     "from funcx_endpoint.executors": "from globus_compute_endpoint.executors",  # noqa E501
 }
 
 
 def _upgrade_funcx_imports_in_config(name: str, force=False) -> str:
     """
     This only modifies unindented import lines, as are in the original
@@ -362,102 +376,14 @@
     except ClickException:
         raise
     except Exception as err:
         msg = f"Unknown Exception {err} attempting to reformat config.py in {ep_dir}"
         raise ClickException(msg) from err
 
 
-def read_config(endpoint_dir: pathlib.Path) -> Config:
-    endpoint_name = endpoint_dir.name
-
-    try:
-        from funcx_endpoint.version import VERSION
-
-        if Version(VERSION) < Version("2.0.0"):
-            msg = (
-                "To avoid compatibility issues with Globus Compute, please uninstall "
-                "funcx-endpoint or upgrade funcx-endpoint to >=2.0.0. Note that the "
-                "funcx-endpoint package is now deprecated."
-            )
-            raise ClickException(msg)
-    except ModuleNotFoundError:
-        pass
-
-    try:
-        conf_path = endpoint_dir / "config.py"
-        spec = importlib.util.spec_from_file_location("config", conf_path)
-        if not (spec and spec.loader):
-            raise Exception(f"Unable to import configuration (no spec): {conf_path}")
-        config = importlib.util.module_from_spec(spec)
-        if not config:
-            raise Exception(f"Unable to import configuration (no config): {conf_path}")
-        spec.loader.exec_module(config)
-        return config.config
-
-    except FileNotFoundError as err:
-        if not endpoint_dir.exists():
-            configure_command = "globus-compute-endpoint configure"
-            if endpoint_name != "default":
-                configure_command += f" {endpoint_name}"
-            msg = (
-                f"{err}"
-                f"\n\nEndpoint '{endpoint_name}' is not configured!"
-                "\n1. Please create a configuration template with:"
-                f"\n\t{configure_command}"
-                "\n2. Update the configuration"
-                "\n3. Start the endpoint\n"
-            )
-            raise ClickException(msg) from err
-        msg = (
-            f"{err}"
-            "\n\nUnable to find required configuration file; has the configuration"
-            "\ndirectory been corrupted?"
-        )
-        raise ClickException(msg) from err
-
-    except AttributeError as err:
-        msg = (
-            f"{err}"
-            "\n\nFailed to find expected data structure in configuration file."
-            "\nHas the configuration file been corrupted or modified incorrectly?\n"
-        )
-        raise ClickException(msg) from err
-
-    except ModuleNotFoundError as err:
-        # Catch specific error when old config.py references funcx_endpoint
-        if "No module named 'funcx_endpoint'" in err.msg:
-            msg = (
-                f"{conf_path} contains import statements from a previously "
-                "configured endpoint that uses the (deprecated) "
-                "funcx-endpoint library. Please update the imports to reference "
-                "globus_compute_endpoint.\n\ni.e.\n"
-                "    from funcx_endpoint.endpoint.utils.config -> "
-                "from globus_compute_endpoint.endpoint.utils.config\n"
-                "    from funcx_endpoint.executors -> "
-                "from globus_compute_endpoint.executors\n"
-                "\n"
-                "You can also use the command "
-                "`globus-compute-endpoint update_funcx_config [endpoint_name]` "
-                "to update them\n"
-            )
-            raise ClickException(msg) from err
-        else:
-            log.exception(err.msg)
-            raise
-
-    except Exception:
-        log.exception(
-            "Globus Compute v2.0.0 made several non-backwards compatible changes to "
-            "the config. Your config might be out of date. "
-            "Refer to "
-            "https://funcx.readthedocs.io/en/latest/endpoints.html#configuring-funcx"
-        )
-        raise
-
-
 def _do_start_endpoint(
     *,
     name: str,
     endpoint_uuid: str | None,
     die_with_parent: bool = False,
 ):
     state = CommandState.ensure()
@@ -467,29 +393,44 @@
             logfile=ep_dir / "endpoint.log",
             debug=state.debug,
             console_enabled=state.log_to_console,
             no_color=state.no_color,
         )
 
     reg_info = {}
+    config_str = None
     if sys.stdin and not (sys.stdin.closed or sys.stdin.isatty()):
         try:
             stdin_data = json.loads(sys.stdin.read())
+
             if not isinstance(stdin_data, dict):
                 type_name = stdin_data.__class__.__name__
                 raise ValueError(
-                    "Expecting JSON dictionary with endpoint registration info; got"
+                    "Expecting JSON dictionary with endpoint info; got"
                     f" {type_name} instead"
                 )
-            reg_info = stdin_data
+
+            reg_info = stdin_data.get("amqp_creds", {})
+            config_str = stdin_data.get("config", None)
+
         except Exception as e:
             exc_type = e.__class__.__name__
-            log.debug("Invalid registration info on stdin -- (%s) %s", exc_type, e)
+            log.debug("Invalid info on stdin -- (%s) %s", exc_type, e)
+
+    if config_str is not None:
+        ep_config = load_config_yaml(config_str)
+    else:
+        ep_config = get_config(ep_dir)
+
+    if die_with_parent:
+        # The endpoint cannot die with it's parent if it
+        # doesn't have one :)
+        ep_config.detach_endpoint = False
+        log.debug("The --die-with-parent flag has set detach_endpoint to False")
 
-    ep_config = read_config(ep_dir)
     if ep_config.multi_tenant:
         epm = EndpointManager(ep_dir, endpoint_uuid, ep_config)
         epm.start()
     else:
         get_cli_endpoint().start_endpoint(
             ep_dir,
             endpoint_uuid,
@@ -529,15 +470,15 @@
     Either should raise ClickException or returns modification result message
     """
     print(_upgrade_funcx_imports_in_config(name=name, force=force))
 
 
 def _do_stop_endpoint(*, name: str, remote: bool = False) -> None:
     ep_dir = get_config_dir() / name
-    Endpoint.stop_endpoint(ep_dir, read_config(ep_dir), remote=remote)
+    Endpoint.stop_endpoint(ep_dir, get_config(ep_dir), remote=remote)
 
 
 @app.command("restart")
 @name_arg
 @common_options
 @start_options
 def restart_endpoint(*, name: str, **_kwargs):
@@ -556,34 +497,34 @@
 def list_endpoints():
     """List all available endpoints"""
     compute_dir = get_config_dir()
     Endpoint.print_endpoint_table(compute_dir)
 
 
 @app.command("delete")
-@name_arg
+@name_arg_allow_uuid
 @click.option(
     "--force",
     default=False,
     is_flag=True,
     help="Deletes the local endpoint even if the web service returns an error.",
 )
 @click.option(
     "--yes", default=False, is_flag=True, help="Do not ask for confirmation to delete."
 )
 @common_options
 def delete_endpoint(*, name: str, force: bool, yes: bool):
     """Deletes an endpoint and its config."""
     if not yes:
         click.confirm(
-            f"Are you sure you want to delete the endpoint <{name}>?", abort=True
+            f"Are you sure you want to delete the endpoint named <{name}>?", abort=True
         )
 
     ep_dir = get_config_dir() / name
-    Endpoint.delete_endpoint(ep_dir, read_config(ep_dir), force)
+    Endpoint.delete_endpoint(ep_dir, get_config(ep_dir), force=force)
 
 
 def cli_run():
     """Entry point for setuptools to point to"""
     app()
```

### Comparing `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/default_config.py` & `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/config/default_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from globus_compute_endpoint.endpoint.utils.config import Config
+from globus_compute_endpoint.endpoint.config import Config
 from globus_compute_endpoint.executors import HighThroughputExecutor
 from parsl.providers import LocalProvider
 
 config = Config(
     display_name=None,  # If None, defaults to the endpoint name
     executors=[
         HighThroughputExecutor(
```

### Comparing `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/endpoint.py` & `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/endpoint.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 import re
 import shutil
 import signal
 import socket
 import sys
 import typing
 import uuid
-from string import Template
 
 import daemon
 import daemon.pidfile
 import psutil
 import setproctitle
 import texttable
+import yaml
 from globus_compute_endpoint import __version__
-from globus_compute_endpoint.endpoint import default_config as endpoint_default_config
+from globus_compute_endpoint.endpoint.config import Config
+from globus_compute_endpoint.endpoint.config.utils import serialize_config
 from globus_compute_endpoint.endpoint.interchange import EndpointInterchange
 from globus_compute_endpoint.endpoint.result_store import ResultStore
 from globus_compute_endpoint.endpoint.utils import _redact_url_creds
-from globus_compute_endpoint.endpoint.utils.config import Config
 from globus_compute_endpoint.logging_config import setup_logging
 from globus_compute_sdk.sdk.client import Client
 from globus_sdk import GlobusAPIError, NetworkError
 
 log = logging.getLogger(__name__)
 
 
@@ -46,63 +46,34 @@
         debug: Bool
             Enable debug logging. Default: False
         """
         self.debug = debug
 
     @staticmethod
     def _config_file_path(endpoint_dir: pathlib.Path) -> pathlib.Path:
-        return endpoint_dir / "config.py"
+        return endpoint_dir / "config.yaml"
 
     @staticmethod
     def update_config_file(
-        ep_name: str,
         original_path: pathlib.Path,
         target_path: pathlib.Path,
         multi_tenant: bool,
         display_name: str | None,
     ):
-        endpoint_config = Template(original_path.read_text()).substitute(name=ep_name)
+        config_text = original_path.read_text()
+        config_dict = yaml.safe_load(config_text)
 
-        # Note that this logic does NOT support replacing arbitrary
-        # display_name="abc xyz" entries, as str quote parsing is beyond the
-        # current use case of calling this method only at endpoint creation
-        display_str = "None" if display_name is None else f'"{display_name}"'
-        display_text = f"display_name={display_str},"
-
-        d_index = endpoint_config.find("display_name")
-        if d_index != -1:
-            if endpoint_config[d_index + 13 : d_index + 18] == "None,":
-                if display_name is not None:
-                    endpoint_config = endpoint_config.replace(
-                        "display_name=None,", display_text
-                    )
-            else:
-                raise Exception(
-                    "Modifying existing display_name not supported "
-                    f"at this time. Please edit {original_path} manually."
-                )
-        else:
-            endpoint_config = endpoint_config.replace(
-                "\nconfig = Config(\n", f"\nconfig = Config(\n    {display_text}\n"
-            )
+        if display_name:
+            config_dict["display_name"] = display_name
 
-        if endpoint_config.find("multi_tenant=") != -1:
-            # If the option is already in the config, merely update the value
-            endpoint_config = re.sub(
-                "multi_tenant=(True|False)",
-                f"multi_tenant={multi_tenant is True}",
-                endpoint_config,
-            )
-        elif multi_tenant:
-            # If the option isn't pre-existing, add only if set to True
-            endpoint_config = endpoint_config.replace(
-                "\nconfig = Config(\n", "\nconfig = Config(\n    multi_tenant=True,\n"
-            )
+        if multi_tenant:
+            config_dict["multi_tenant"] = multi_tenant
 
-        target_path.write_text(endpoint_config)
+        config_text = yaml.safe_dump(config_dict)
+        target_path.write_text(config_text)
 
     @staticmethod
     def init_endpoint_dir(
         endpoint_dir: pathlib.Path,
         endpoint_config: pathlib.Path | None = None,
         multi_tenant=False,
         display_name: str | None = None,
@@ -124,18 +95,18 @@
             # only an issue for totally new users (no .globus_compute/!), but that is
             # also precisely the interaction -- the first one -- that should go smoothly
             endpoint_dir.mkdir(parents=True, exist_ok=True)
 
             config_target_path = Endpoint._config_file_path(endpoint_dir)
 
             if endpoint_config is None:
-                endpoint_config = pathlib.Path(endpoint_default_config.__file__)
+                package_dir = pathlib.Path(__file__).resolve().parent
+                endpoint_config = package_dir / "config/default_config.yaml"
 
             Endpoint.update_config_file(
-                endpoint_dir.name,
                 endpoint_config,
                 config_target_path,
                 multi_tenant,
                 display_name,
             )
         finally:
             os.umask(user_umask)
@@ -155,21 +126,21 @@
 
         templ_conf_path = pathlib.Path(endpoint_config) if endpoint_config else None
         Endpoint.init_endpoint_dir(
             conf_dir, templ_conf_path, multi_tenant, display_name
         )
         config_path = Endpoint._config_file_path(conf_dir)
         if multi_tenant:
-            print(f"Created multi-tenant profile for <{ep_name}>")
+            print(f"Created multi-tenant profile for endpoint named <{ep_name}>")
         else:
-            print(f"Created profile for <{ep_name}>")
+            print(f"Created profile for endpoint named <{ep_name}>")
         print(
-            f"\n    Configuration file: {config_path}\n"
+            f"\n\tConfiguration file: {config_path}\n"
             "\nUse the `start` subcommand to run it:\n"
-            f"\n    $ globus-compute-endpoint start {ep_name}"
+            f"\n\t$ globus-compute-endpoint start {ep_name}"
         )
 
     @staticmethod
     def validate_endpoint_name(path_name: str) -> None:
         # Validate the path by removing all relative path modifiers (i.e., ../),
         # taking the basename, ensuring it's not Unix hidden (initial dot [.]), and
         # has no whitespace.  The path name is used deep within Parsl, which uses
@@ -343,15 +314,15 @@
                     multi_tenant=False,
                     display_name=endpoint_config.display_name,
                 )
 
             except GlobusAPIError as e:
                 if e.http_status in (409, 410, 423):
                     # CONFLICT, GONE or LOCKED
-                    log.warning(f"Endpoint registration blocked.  [{e.message}]")
+                    log.warning(f"Endpoint registration blocked.  [{e.text}]")
                     exit(os.EX_UNAVAILABLE)
                 raise
 
             except NetworkError as e:
                 # the output of a NetworkError exception is huge and unhelpful, so
                 # it seems better to just stringify it here and get a concise error
                 log.exception(
@@ -541,27 +512,30 @@
 
         if not endpoint_dir.exists():
             log.warning(f"Endpoint <{ep_name}> does not exist")
             exit(-1)
 
         endpoint_id = Endpoint.get_endpoint_id(endpoint_dir)
         if endpoint_id is None:
-            log.warning(f"Endpoint <{ep_name}> could not be located")
+            log.warning(
+                f"Configuration for endpoint <{ep_name}> could not be found, it "
+                "might not have been initialized locally"
+            )
             if not force:
                 exit(-1)
 
         # Delete endpoint from web service
         try:
             fx_client = Endpoint.get_funcx_client(endpoint_config)
             fx_client.delete_endpoint(endpoint_id)
             log.info(f"Endpoint <{ep_name}> has been deleted from the web service")
         except GlobusAPIError as e:
             log.warning(
                 f"Endpoint <{ep_name}> could not be deleted from the web service"
-                f"  [{e.message}]"
+                f"  [{e.text}]"
             )
             if not force:
                 log.critical("Exiting without deleting the endpoint")
                 exit(os.EX_UNAVAILABLE)
         except NetworkError as e:
             log.warning(
                 f"Endpoint <{ep_name}> could not be deleted from the web service"
@@ -642,15 +616,15 @@
                  "id": "xxxxxxxx-xxxx-1234-abcd-xxxxxxxxxxxx"
             }
         }
         """
         ep_statuses = {}
 
         funcx_conf_dir = pathlib.Path(funcx_conf_dir)
-        ep_dir_paths = (p.parent for p in funcx_conf_dir.glob("*/config.py"))
+        ep_dir_paths = (p.parent for p in funcx_conf_dir.glob("*/config.*"))
         for ep_path in ep_dir_paths:
             ep_status = {
                 "status": "Initialized",
                 "id": Endpoint.get_endpoint_id(ep_path),
             }
             ep_statuses[ep_path.name] = ep_status
             if not ep_status["id"]:
@@ -739,46 +713,15 @@
 
         # the following are read from the HTTP request by the web service, but can be
         # overridden here if desired:
         metadata["ip_address"] = None
         metadata["sdk_version"] = None
 
         try:
-            metadata["config"] = _serialize_config(config)
+            metadata["config"] = serialize_config(config)
         except Exception as e:
             log.warning(
                 f"Error when serializing config ({type(e).__name__}). Ignoring."
             )
             log.debug("Config serialization exception details", exc_info=e)
 
         return metadata
-
-
-def _serialize_config(config: Config) -> dict:
-    """
-    Short-term serialization method until config.py is replaced with config.yaml
-    """
-
-    expand_list = ["strategy", "provider", "launcher"]
-    pass_through_list = ["allowed_functions"]
-
-    def to_dict(o):
-        mems = {"_type": type(o).__name__}
-
-        for k, v in o.__dict__.items():
-            if k.startswith("_"):
-                continue
-
-            if k in expand_list:
-                mems[k] = to_dict(v)
-            elif isinstance(v, str) or k in pass_through_list:
-                mems[k] = v
-            else:
-                mems[k] = repr(v)
-
-        return mems
-
-    result = to_dict(config)
-    # when we move to config.yaml, should only need to support a single executor
-    result["executors"] = [to_dict(executor) for executor in config.executors]
-
-    return result
```

### Comparing `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/endpoint_manager.py` & `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/endpoint_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import fcntl
 import json
 import logging
 import os
 import pathlib
 import pwd
 import queue
 import re
@@ -15,20 +16,24 @@
 import time
 import typing as t
 from datetime import datetime
 
 import globus_compute_sdk as gc
 import setproctitle
 from globus_compute_endpoint import __version__
+from globus_compute_endpoint.endpoint.config import Config
+from globus_compute_endpoint.endpoint.config.utils import (
+    render_config_user_template,
+    serialize_config,
+)
 from globus_compute_endpoint.endpoint.endpoint import Endpoint
 from globus_compute_endpoint.endpoint.rabbit_mq.command_queue_subscriber import (
     CommandQueueSubscriber,
 )
 from globus_compute_endpoint.endpoint.utils import _redact_url_creds
-from globus_compute_endpoint.endpoint.utils.config import Config
 from globus_sdk import GlobusAPIError, NetworkError
 
 if t.TYPE_CHECKING:
     from pika.spec import BasicProperties
 
 
 log = logging.getLogger(__name__)
@@ -43,14 +48,15 @@
         self,
         conf_dir: pathlib.Path,
         endpoint_uuid: str | None,
         config: Config,
     ):
         log.info("Endpoint Manager initialization")
 
+        self.conf_dir = conf_dir
         self._reload_requested = False
         self._time_to_stop = False
         self._kill_event = threading.Event()
 
         self._child_args: dict[int, tuple[int, int, str, str]] = {}
         self._wait_for_child = False
 
@@ -73,15 +79,15 @@
                 endpoint_uuid,
                 metadata=EndpointManager.get_metadata(config),
                 multi_tenant=True,
             )
         except GlobusAPIError as e:
             if e.http_status == 409 or e.http_status == 423:
                 # RESOURCE_CONFLICT or RESOURCE_LOCKED
-                log.warning(f"Endpoint registration blocked.  [{e.message}]")
+                log.warning(f"Endpoint registration blocked.  [{e.text}]")
                 exit(os.EX_UNAVAILABLE)
             raise
         except NetworkError as e:
             log.exception("Network error while registering multi-tenant endpoint")
             log.critical(f"Network failure; unable to register endpoint: {e}")
             exit(os.EX_TEMPFAIL)
 
@@ -136,22 +142,15 @@
     def get_metadata(config: Config) -> dict:
         # Piecemeal Config settings because for MT, most of the ST items are
         # unrelated -- the MT (aka EndpointManager) does not execute tasks
         return {
             "endpoint_version": __version__,
             "hostname": socket.getfqdn(),
             "local_user": pwd.getpwuid(os.getuid()).pw_name,
-            "config": {
-                "_type": type(config).__name__,
-                "multi_tenant": True,  # redundant, but "whatev"
-                "stdout": config.stdout,
-                "stderr": config.stderr,
-                "environment": config.environment,
-                "funcx_service_address": config.funcx_service_address,
-            },
+            "config": serialize_config(config),
         }
 
     def request_shutdown(self, sig_num, curr_stack_frame):
         self._time_to_stop = True
 
     def set_child_died(self, sig_num, curr_stack_fframe):
         self._wait_for_child = True
@@ -297,14 +296,15 @@
             try:
                 server_cmd_ts = props.timestamp
                 if props.content_type != "application/json":
                     raise ValueError("Invalid message type; expecting JSON")
 
                 msg = json.loads(body)
                 command = msg.get("command")
+                user_opts = msg.get("user_opts", {})
                 command_args = msg.get("args", [])
                 command_kwargs = msg.get("kwargs", {})
             except Exception as e:
                 log.error(
                     f"Unable to deserialize Globus Compute services command."
                     f"  ({e.__class__.__name__}) {e}"
                 )
@@ -339,19 +339,19 @@
                 self._command.ack(d_tag)
                 continue
 
             try:
                 if not (command and valid_method_name_re.match(command)):
                     raise InvalidCommandError(f"Unknown or invalid command: {command}")
 
-                command_func = getattr(self.__class__, command, None)
+                command_func = getattr(self, command, None)
                 if not command_func:
                     raise InvalidCommandError(f"Unknown or invalid command: {command}")
 
-                command_func(self._child_args, local_user, command_args, command_kwargs)
+                command_func(local_user, user_opts, command_args, command_kwargs)
                 log.info(
                     f"Command process successfully forked for '{globus_username}'"
                     f" ('{globus_uuid}')."
                 )
             except InvalidCommandError as err:
                 log.error(str(err))
 
@@ -360,21 +360,23 @@
                     f"Unable to execute command: {command}\n"
                     f"    args: {command_args}\n"
                     f"  kwargs: {command_kwargs}"
                 )
             finally:
                 self._command.ack(d_tag)
 
-    @staticmethod
     def cmd_start_endpoint(
-        child_args: dict[int, tuple[int, int, str, str]],
+        self,
         local_username: str,
+        user_opts: dict | None,
         args: list[str] | None,
         kwargs: dict | None,
     ):
+        if not user_opts:
+            user_opts = {}
         if not args:
             args = []
         if not kwargs:
             kwargs = {}
 
         ep_name = kwargs.get("name", "")
         if not ep_name:
@@ -396,15 +398,15 @@
             pid = os.fork()
         except Exception as e:
             log.error(f"Unable to fork child process: ({e.__class__.__name__}) {e}")
             raise
 
         if pid > 0:
             proc_args_s = f"({uname}, {ep_name}) {' '.join(proc_args)}"
-            child_args[pid] = (uid, gid, local_username, proc_args_s)
+            self._child_args[pid] = (uid, gid, local_username, proc_args_s)
             log.info(f"Creating new user endpoint (pid: {pid}) [{proc_args_s}]")
             return
 
         # Reminder: from this point on, we are now the *child* process.
         pid = os.getpid()
 
         exit_code = 70
@@ -455,26 +457,43 @@
             env["CWD"] = wd
 
             # in case "something gets stuck," let cmdline show it
             args_title = " ".join(proc_args)
             startup_proc_title = f"Endpoint starting up for {uname} [{args_title}]"
             setproctitle.setproctitle(startup_proc_title)
 
-            amqp_creds = json.dumps(kwargs.get("amqp_creds"))
+            stdin_data_dict = {
+                "amqp_creds": kwargs.get("amqp_creds"),
+                "config": render_config_user_template(self.conf_dir, user_opts),
+            }
+            stdin_data = json.dumps(stdin_data_dict)
+            exit_code += 1
 
             # Reminder: this is *os*.open, not *open*.  Descriptors will not be closed
             # unless we explicitly do so, so `null_fd =` in loop will work.
             null_fd = os.open(os.devnull, os.O_WRONLY, mode=0o200)
             while null_fd < 3:  # reminder 0/1/2 == std in/out/err, so ...
                 # ... overkill, but "just in case": don't step on them
                 null_fd = os.open(os.devnull, os.O_WRONLY, mode=0o200)
             exit_code += 1
 
             log.debug("Setting up process stdin")
             read_handle, write_handle = os.pipe()
+
+            # fcntl.F_GETPIPE_SZ is not available in Python versions less than 3.10
+            F_GETPIPE_SZ = 1032
+            # 256 - Allow some head room for multiple kernel-specific factors
+            max_buf_size = fcntl.fcntl(write_handle, F_GETPIPE_SZ) - 256
+            stdin_data_size = len(stdin_data)
+            if stdin_data_size > max_buf_size:
+                raise ValueError(
+                    f"Unable to write {stdin_data_size} bytes of data to stdin; "
+                    f"the maximum allowed is {max_buf_size} bytes"
+                )
+
             exit_code += 1
             if os.dup2(read_handle, 0) != 0:  # close old stdin, use read_handle
                 raise OSError("Unable to close stdin")
             os.close(read_handle)
             exit_code += 1
 
             log.debug("Redirecting stdout and stderr (%s)", os.devnull)
@@ -485,18 +504,18 @@
                 if os.dup2(null_f.fileno(), 2) != 2:
                     raise OSError("Unable to close stderr")
 
             # After the last os.dup2(), we are unable to get logs at *all*; hence the
             # exit_code as a last-ditch attempt at sharing "what went wrong where" to
             # the parent process.
             exit_code += 1
-            log.debug("Writing credentials")
-            with os.fdopen(write_handle, "w") as cred_pipe:
+            log.debug("Writing credentials and config to stdin")
+            with os.fdopen(write_handle, "w") as stdin_pipe:
                 # intentional side effect: close handle
-                cred_pipe.write(amqp_creds)
+                stdin_pipe.write(stdin_data)
 
             exit_code += 1
             _soft_no, hard_no = resource.getrlimit(resource.RLIMIT_NOFILE)
 
             # Save closerange until last so that we can still get logs written
             # to the endpoint.log.  Meanwhile, use the exit_code as a
             # last-ditch attempt at sharing "what went wrong where" to the
```

### Comparing `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/interchange.py` & `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/interchange.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import typing as t
 
 # multiprocessing.Event is a method, not a class
 # to annotate, we need the "real" class
 # see: https://github.com/python/typeshed/issues/4266
 from multiprocessing.synchronize import Event as EventType
 
-import globus_compute_endpoint.endpoint.utils.config
+import globus_compute_endpoint.endpoint.config
 import pika.exceptions
 import setproctitle
 from globus_compute_common.messagepack import InvalidMessageError, pack, unpack
 from globus_compute_common.messagepack.message_types import (
     EPStatusReport,
     Result,
     ResultErrorDetails,
@@ -57,15 +57,15 @@
     5. Be aware of requests worker resource capacity,
        eg. schedule only jobs that fit into walltime.
 
     """
 
     def __init__(
         self,
-        config: globus_compute_endpoint.endpoint.utils.config.Config,
+        config: globus_compute_endpoint.endpoint.config.Config,
         reg_info: dict[str, dict],
         logdir=".",
         endpoint_id=None,
         endpoint_dir=".",
         result_store: ResultStore | None = None,
         reconnect_attempt_limit: int = 5,
         parent_pid: int = 0,
```

### Comparing `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/messages_compat.py` & `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/messages_compat.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/rabbit_mq/base.py` & `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/rabbit_mq/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py` & `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py` & `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py` & `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/result_store.py` & `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/result_store.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/taskqueue.py` & `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/taskqueue.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/utils/__init__.py` & `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/endpoint/utils/config.py` & `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/endpoint/config/config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/engines/base.py` & `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/engines/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/engines/globus_compute.py` & `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/engines/globus_compute.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/engines/helper.py` & `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/engines/helper.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/engines/process_pool.py` & `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/engines/process_pool.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/engines/thread_pool.py` & `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/engines/thread_pool.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/exception_handling.py` & `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/exception_handling.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/high_throughput/container_sched.py` & `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/high_throughput/container_sched.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/high_throughput/executor.py` & `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/high_throughput/executor.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/high_throughput/interchange.py` & `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/high_throughput/interchange.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py` & `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/high_throughput/manager.py` & `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/high_throughput/manager.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/high_throughput/messages.py` & `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/high_throughput/messages.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/high_throughput/worker.py` & `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/high_throughput/worker.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/high_throughput/worker_map.py` & `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/high_throughput/worker_map.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py` & `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/logging_config.py` & `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/logging_config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/providers/kubernetes/kube.py` & `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/providers/kubernetes/kube.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/strategies/base.py` & `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/strategies/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/strategies/kube_simple.py` & `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/strategies/kube_simple.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/strategies/simple.py` & `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/strategies/simple.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/strategies/test.py` & `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/strategies/test.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint/version.py` & `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # single source of truth for package version,
 # see https://packaging.python.org/en/latest/single_source_version/
-__version__ = "2.1.0a1"
+__version__ = "2.2.0a0"
 
 # TODO: remove after a `globus-compute-sdk` release
 # this is needed because it's imported by `globus-compute-sdk` to do the version check
 VERSION = __version__
 
 # Here as it's the easier way for funcx-endpoint cli to display it
 DEPRECATION_FUNCX_ENDPOINT = """
```

### Comparing `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint.egg-info/PKG-INFO` & `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-endpoint
-Version: 2.1.0a1
+Version: 2.2.0a0
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `globus-compute-endpoint-2.1.0a1/globus_compute_endpoint.egg-info/SOURCES.txt` & `globus-compute-endpoint-2.2.0a0/globus_compute_endpoint.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -12,22 +12,25 @@
 globus_compute_endpoint.egg-info/PKG-INFO
 globus_compute_endpoint.egg-info/SOURCES.txt
 globus_compute_endpoint.egg-info/dependency_links.txt
 globus_compute_endpoint.egg-info/entry_points.txt
 globus_compute_endpoint.egg-info/requires.txt
 globus_compute_endpoint.egg-info/top_level.txt
 globus_compute_endpoint/endpoint/__init__.py
-globus_compute_endpoint/endpoint/config.py
-globus_compute_endpoint/endpoint/default_config.py
 globus_compute_endpoint/endpoint/endpoint.py
 globus_compute_endpoint/endpoint/endpoint_manager.py
 globus_compute_endpoint/endpoint/interchange.py
 globus_compute_endpoint/endpoint/messages_compat.py
 globus_compute_endpoint/endpoint/result_store.py
 globus_compute_endpoint/endpoint/taskqueue.py
+globus_compute_endpoint/endpoint/config/__init__.py
+globus_compute_endpoint/endpoint/config/config.py
+globus_compute_endpoint/endpoint/config/default_config.py
+globus_compute_endpoint/endpoint/config/model.py
+globus_compute_endpoint/endpoint/config/utils.py
 globus_compute_endpoint/endpoint/rabbit_mq/__init__.py
 globus_compute_endpoint/endpoint/rabbit_mq/base.py
 globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py
 globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py
 globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py
 globus_compute_endpoint/endpoint/utils/__init__.py
 globus_compute_endpoint/endpoint/utils/config.py
```

### Comparing `globus-compute-endpoint-2.1.0a1/setup.py` & `globus-compute-endpoint-2.2.0a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 REQUIRES = [
     "requests>=2.20.0,<3",
     "globus-sdk",  # version will be bounded by `globus-compute-sdk`
-    "globus-compute-sdk==2.1.0a1",
+    "globus-compute-sdk==2.2.0a0",
     "globus-compute-common==0.2.0",
     # table printing used in list-endpoints
     "texttable>=1.6.4,<2",
     # although psutil does not declare itself to use semver, it appears to offer
     # strong backwards-compatibility promises based on its changelog, usage, and
     # history
     #
@@ -32,14 +32,16 @@
     "pyzmq>=22.0.0,!=22.3.0,<=23.2.0",
     # 'parsl' is a core requirement of the globus-compute-endpoint, essential to a range
     # of different features and functions
     # pin exact versions because it does not use semver
     "parsl==2023.03.27",
     "pika>=1.2.0",
     "setproctitle>=1.3.2,<1.4",
+    "pyyaml>=6.0,<7.0",
+    "jinja2>=3.1.2,<3.2",
 ]
 
 TEST_REQUIRES = [
     "responses",
     "pytest>=7.2",
     "coverage>=5.2",
     "pytest-mock==3.2.0",
```

### Comparing `globus-compute-endpoint-2.1.0a1/tests/conftest.py` & `globus-compute-endpoint-2.2.0a0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.1.0a1/tests/utils.py` & `globus-compute-endpoint-2.2.0a0/tests/utils.py`

 * *Files identical despite different names*

