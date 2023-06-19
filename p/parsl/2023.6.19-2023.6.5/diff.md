# Comparing `tmp/parsl-2023.6.19.tar.gz` & `tmp/parsl-2023.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsl-2023.6.19.tar", last modified: Mon Jun 19 22:57:43 2023, max compression
+gzip compressed data, was "parsl-2023.6.5.tar", last modified: Mon Jun  5 22:43:11 2023, max compression
```

## Comparing `parsl-2023.6.19.tar` & `parsl-2023.6.5.tar`

### file list

```diff
@@ -1,481 +1,472 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.675382 parsl-2023.6.19/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-19 22:57:40.000000 parsl-2023.6.19/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-19 22:57:40.000000 parsl-2023.6.19/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-19 22:57:43.675382 parsl-2023.6.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-06-19 22:57:40.000000 parsl-2023.6.19/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.643381 parsl-2023.6.19/parsl/
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/addresses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.643381 parsl-2023.6.19/parsl/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/app/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/app/bash.py
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/app/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/app/futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/app/python.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.647381 parsl-2023.6.19/parsl/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/benchmark/perf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.647381 parsl-2023.6.19/parsl/channels/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/channels/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/channels/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.647381 parsl-2023.6.19/parsl/channels/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/channels/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/channels/local/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.647381 parsl-2023.6.19/parsl/channels/oauth_ssh/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/channels/oauth_ssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/channels/oauth_ssh/oauth_ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.647381 parsl-2023.6.19/parsl/channels/ssh/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/channels/ssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/channels/ssh/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.647381 parsl-2023.6.19/parsl/channels/ssh_il/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/channels/ssh_il/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/channels/ssh_il/ssh_il.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.647381 parsl-2023.6.19/parsl/concurrent/
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/concurrent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.647381 parsl-2023.6.19/parsl/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/configs/ASPIRE1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/configs/Azure.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/configs/ad_hoc.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/configs/bluewaters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/configs/bridges.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/configs/cc_in2p3.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/configs/comet.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/configs/cooley.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/configs/cori.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/configs/ec2.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/configs/exex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/configs/frontera.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/configs/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/configs/illinoiscluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/configs/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/configs/local_threads.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/configs/midway.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/configs/osg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/configs/polaris.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/configs/stampede2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/configs/summit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/configs/theta.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/configs/toss3_llnl.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/configs/vineex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/configs/wqex_local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.647381 parsl-2023.6.19/parsl/data_provider/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/data_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/data_provider/data_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/data_provider/file_noop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/data_provider/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/data_provider/ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/data_provider/globus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/data_provider/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/data_provider/rsync.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/data_provider/staging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.651381 parsl-2023.6.19/parsl/dataflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/dataflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62269 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/dataflow/dflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/dataflow/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/dataflow/executor_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/dataflow/futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/dataflow/job_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/dataflow/job_status_poller.py
--rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/dataflow/memoization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/dataflow/rundirs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/dataflow/states.py
--rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/dataflow/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/dataflow/taskrecord.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.651381 parsl-2023.6.19/parsl/executors/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/executors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/executors/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.651381 parsl-2023.6.19/parsl/executors/extreme_scale/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/executors/extreme_scale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/executors/extreme_scale/executor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18710 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/executors/extreme_scale/mpi_worker_pool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.651381 parsl-2023.6.19/parsl/executors/flux/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/executors/flux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/executors/flux/execute_parsl_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    16987 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/executors/flux/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/executors/flux/flux_instance_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.651381 parsl-2023.6.19/parsl/executors/high_throughput/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/executors/high_throughput/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/executors/high_throughput/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    33191 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/executors/high_throughput/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    29976 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/executors/high_throughput/interchange.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/executors/high_throughput/manager_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/executors/high_throughput/monitoring_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/executors/high_throughput/probe.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    33011 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/executors/high_throughput/process_worker_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/executors/high_throughput/zmq_pipes.py
--rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/executors/status_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/executors/swift_t.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.651381 parsl-2023.6.19/parsl/executors/taskvine/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/executors/taskvine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/executors/taskvine/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/executors/taskvine/exec_parsl_function.py
--rw-r--r--   0 runner    (1001) docker     (123)    48948 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/executors/taskvine/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/executors/threads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.651381 parsl-2023.6.19/parsl/executors/workqueue/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/executors/workqueue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/executors/workqueue/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/executors/workqueue/exec_parsl_function.py
--rw-r--r--   0 runner    (1001) docker     (123)    48130 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/executors/workqueue/executor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5514 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/executors/workqueue/parsl_coprocess.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      735 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/executors/workqueue/parsl_coprocess_stub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.651381 parsl-2023.6.19/parsl/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/launchers/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    15358 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/launchers/launchers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/log_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.655382 parsl-2023.6.19/parsl/monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36233 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/monitoring/db_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/monitoring/message_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    23396 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/monitoring/monitoring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.655382 parsl-2023.6.19/parsl/monitoring/queries/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/monitoring/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/monitoring/queries/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/monitoring/radios.py
--rw-r--r--   0 runner    (1001) docker     (123)    13172 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/monitoring/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/monitoring/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.655382 parsl-2023.6.19/parsl/monitoring/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/monitoring/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/monitoring/visualization/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/monitoring/visualization/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.655382 parsl-2023.6.19/parsl/monitoring/visualization/plots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/monitoring/visualization/plots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.655382 parsl-2023.6.19/parsl/monitoring/visualization/plots/default/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/monitoring/visualization/plots/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/monitoring/visualization/plots/default/task_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/monitoring/visualization/plots/default/workflow_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.655382 parsl-2023.6.19/parsl/monitoring/visualization/static/
--rwxr-xr-x   0 runner    (1001) docker     (123)    14199 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/monitoring/visualization/static/parsl-logo-white.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      337 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/monitoring/visualization/static/parsl-monitor.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.655382 parsl-2023.6.19/parsl/monitoring/visualization/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/monitoring/visualization/templates/app.html
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/monitoring/visualization/templates/dag.html
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/monitoring/visualization/templates/error.html
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/monitoring/visualization/templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/monitoring/visualization/templates/resource_usage.html
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/monitoring/visualization/templates/task.html
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/monitoring/visualization/templates/workflow.html
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/monitoring/visualization/templates/workflows_summary.html
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/monitoring/visualization/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/monitoring/visualization/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/monitoring/visualization/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/process_loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.655382 parsl-2023.6.19/parsl/providers/
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.655382 parsl-2023.6.19/parsl/providers/ad_hoc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/providers/ad_hoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/providers/ad_hoc/ad_hoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.655382 parsl-2023.6.19/parsl/providers/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/providers/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29073 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/providers/aws/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/providers/aws/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.655382 parsl-2023.6.19/parsl/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/providers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18367 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/providers/azure/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/providers/azure/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/providers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/providers/cluster_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.655382 parsl-2023.6.19/parsl/providers/cobalt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/providers/cobalt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/providers/cobalt/cobalt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      273 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/providers/cobalt/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.655382 parsl-2023.6.19/parsl/providers/condor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/providers/condor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13178 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/providers/condor/condor.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/providers/condor/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/providers/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.655382 parsl-2023.6.19/parsl/providers/googlecloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/providers/googlecloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/providers/googlecloud/googlecloud.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.659381 parsl-2023.6.19/parsl/providers/grid_engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/providers/grid_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/providers/grid_engine/grid_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/providers/grid_engine/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.659381 parsl-2023.6.19/parsl/providers/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/providers/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12790 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/providers/kubernetes/kube.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/providers/kubernetes/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.659381 parsl-2023.6.19/parsl/providers/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/providers/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/providers/local/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.659381 parsl-2023.6.19/parsl/providers/lsf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/providers/lsf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/providers/lsf/lsf.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/providers/lsf/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.659381 parsl-2023.6.19/parsl/providers/pbspro/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/providers/pbspro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/providers/pbspro/pbspro.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/providers/pbspro/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.659381 parsl-2023.6.19/parsl/providers/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/providers/slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11697 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/providers/slurm/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/providers/slurm/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.659381 parsl-2023.6.19/parsl/providers/torque/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/providers/torque/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/providers/torque/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/providers/torque/torque.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.659381 parsl-2023.6.19/parsl/serialize/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/serialize/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/serialize/concretes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/serialize/facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.659381 parsl-2023.6.19/parsl/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/callables_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.663381 parsl-2023.6.19/parsl/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/configs/ad_hoc_cluster_htex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/configs/azure_single_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/configs/bluewaters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/configs/bridges.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/configs/cc_in2p3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/configs/comet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/configs/cooley_htex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/configs/cori.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/configs/ec2_single_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/configs/ec2_spot.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/configs/exex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/configs/frontera.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/configs/htex_ad_hoc_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/configs/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/configs/htex_local_alternate.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/configs/htex_local_intask_staging.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/configs/htex_local_rsync_staging.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/configs/local_adhoc.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/configs/local_threads.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/configs/local_threads_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/configs/local_threads_checkpoint_dfk_exit.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/configs/local_threads_checkpoint_periodic.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/configs/local_threads_checkpoint_task_exit.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/configs/local_threads_ftp_in_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/configs/local_threads_globus.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/configs/local_threads_http_in_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/configs/local_threads_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/configs/local_threads_no_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/configs/midway.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/configs/nscc_singapore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/configs/osg_htex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/configs/petrelkube.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/configs/summit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/configs/swan_htex.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/configs/taskvine_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/configs/theta.py
--rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/configs/user_opts.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/configs/workqueue_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.663381 parsl-2023.6.19/parsl/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/integration/latency.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.663381 parsl-2023.6.19/parsl/tests/integration/test_apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/integration/test_apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.663381 parsl-2023.6.19/parsl/tests/integration/test_channels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/integration/test_channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/integration/test_channels/test_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/integration/test_channels/test_local_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/integration/test_channels/test_scp_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/integration/test_channels/test_ssh_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/integration/test_channels/test_ssh_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/integration/test_channels/test_ssh_file_transport.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/integration/test_channels/test_ssh_interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/integration/test_parsl_load_default_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.663381 parsl-2023.6.19/parsl/tests/integration/test_stress/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/integration/test_stress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/integration/test_stress/test_python_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/integration/test_stress/test_python_threads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.663381 parsl-2023.6.19/parsl/tests/manual_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/manual_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/manual_tests/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/manual_tests/test_ad_hoc_htex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/manual_tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/manual_tests/test_log_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/manual_tests/test_memory_limits.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/manual_tests/test_oauth_ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/manual_tests/test_regression_220.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/manual_tests/test_udp_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/manual_tests/test_worker_count.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.667381 parsl-2023.6.19/parsl/tests/scaling_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/scaling_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/scaling_tests/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/scaling_tests/local_threads.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3835 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/scaling_tests/test_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/scaling_tests/vineex_condor.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/scaling_tests/vineex_local.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/scaling_tests/wqex_condor.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/scaling_tests/wqex_local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.667381 parsl-2023.6.19/parsl/tests/site_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/site_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/site_tests/site_config_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/site_tests/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/site_tests/test_site.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.667381 parsl-2023.6.19/parsl/tests/sites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/sites/test_affinity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/sites/test_concurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/sites/test_dynamic_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/sites/test_ec2.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/sites/test_launchers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/sites/test_local_adhoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.667381 parsl-2023.6.19/parsl/tests/sites/test_mpi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/sites/test_mpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/sites/test_start_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/sites/test_worker_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_aalst_patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.667381 parsl-2023.6.19/parsl/tests/test_bash_apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_bash_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_bash_apps/test_apptimeout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_bash_apps/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_bash_apps/test_error_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_bash_apps/test_keyword_overlaps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_bash_apps/test_kwarg_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_bash_apps/test_memoize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_bash_apps/test_memoize_ignore_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_bash_apps/test_multiline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_bash_apps/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_bash_apps/test_stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_callables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.667381 parsl-2023.6.19/parsl/tests/test_channels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_channels/test_large_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.667381 parsl-2023.6.19/parsl/tests/test_checkpointing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_checkpointing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_checkpointing/test_periodic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_checkpointing/test_python_checkpoint_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_checkpointing/test_python_checkpoint_2.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_checkpointing/test_python_checkpoint_3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_checkpointing/test_regression_232.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_checkpointing/test_regression_233.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_checkpointing/test_regression_239.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_checkpointing/test_task_exit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.667381 parsl-2023.6.19/parsl/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_data/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_data/test_file_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_data/test_file_staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_data/test_output_chain_filenames.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.671382 parsl-2023.6.19/parsl/tests/test_docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_docs/test_from_slides.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_docs/test_tutorial_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_docs/test_workflow1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_docs/test_workflow2.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_docs/test_workflow3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_docs/test_workflow4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.671382 parsl-2023.6.19/parsl/tests/test_error_handling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_error_handling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_error_handling/test_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_error_handling/test_htex_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_error_handling/test_htex_missing_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_error_handling/test_htex_worker_failure.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_error_handling/test_python_walltime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_error_handling/test_rand_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_error_handling/test_resource_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_error_handling/test_retries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_error_handling/test_retry_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_error_handling/test_retry_handler_failure.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_error_handling/test_serialization_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_error_handling/test_wrap_with_logs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.671382 parsl-2023.6.19/parsl/tests/test_flowcontrol/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_flowcontrol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_flux.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.671382 parsl-2023.6.19/parsl/tests/test_monitoring/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_monitoring/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_monitoring/test_db_locks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_monitoring/test_fuzz_zmq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_monitoring/test_memoization_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_monitoring/test_viz_colouring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.671382 parsl-2023.6.19/parsl/tests/test_providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_providers/test_local_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.671382 parsl-2023.6.19/parsl/tests/test_python_apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_python_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_python_apps/test_arg_input_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_python_apps/test_at_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_python_apps/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_python_apps/test_dep_standard_futures.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_python_apps/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_python_apps/test_depfail_propagation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_python_apps/test_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_python_apps/test_fibonacci_iterative.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_python_apps/test_fibonacci_recursive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_python_apps/test_futures.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_python_apps/test_garbage_collect.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_python_apps/test_import_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_python_apps/test_join.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_python_apps/test_mapred.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_python_apps/test_memoize_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_python_apps/test_memoize_2.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_python_apps/test_memoize_4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_python_apps/test_memoize_ignore_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_python_apps/test_memoize_joinapp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_python_apps/test_outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_python_apps/test_overview.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_python_apps/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_python_apps/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_python_apps/test_type5.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_python_apps/test_worker_fail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.675382 parsl-2023.6.19/parsl/tests/test_regression/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_regression/test_1480.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_regression/test_1606_wait_for_current_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_regression/test_1653.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_regression/test_221.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_regression/test_226.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_regression/test_2652.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_regression/test_69a.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_regression/test_69b.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_regression/test_854.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_regression/test_97_parallelism_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_regression/test_98.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.675382 parsl-2023.6.19/parsl/tests/test_scaling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_scaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_scaling/test_regression_1621.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_scaling/test_scale_down.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.675382 parsl-2023.6.19/parsl/tests/test_staging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_staging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_staging/staging_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_staging/test_1316.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_staging/test_docs_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_staging/test_docs_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_staging/test_elaborate_noop_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_staging/test_staging_ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_staging/test_staging_ftp_in_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_staging/test_staging_globus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_staging/test_staging_https.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_staging/test_staging_https_in_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_swift.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_thread_parallelism.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.675382 parsl-2023.6.19/parsl/tests/test_threads/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_threads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_threads/test_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/test_threads/test_lazy_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.675382 parsl-2023.6.19/parsl/usage_tracking/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/usage_tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/usage_tracking/usage.py
--rw-r--r--   0 runner    (1001) docker     (123)    10882 2023-06-19 22:57:40.000000 parsl-2023.6.19/parsl/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-19 22:57:42.000000 parsl-2023.6.19/parsl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:57:43.643381 parsl-2023.6.19/parsl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-19 22:57:43.000000 parsl-2023.6.19/parsl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15787 2023-06-19 22:57:43.000000 parsl-2023.6.19/parsl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 22:57:43.000000 parsl-2023.6.19/parsl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-19 22:57:43.000000 parsl-2023.6.19/parsl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-19 22:57:43.000000 parsl-2023.6.19/parsl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-19 22:57:43.000000 parsl-2023.6.19/parsl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-19 22:57:40.000000 parsl-2023.6.19/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 22:57:43.675382 parsl-2023.6.19/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2624 2023-06-19 22:57:40.000000 parsl-2023.6.19/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.190580 parsl-2023.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-05 22:43:01.000000 parsl-2023.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-05 22:43:01.000000 parsl-2023.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-05 22:43:11.190580 parsl-2023.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-06-05 22:43:01.000000 parsl-2023.6.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.122580 parsl-2023.6.5/parsl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/addresses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.126580 parsl-2023.6.5/parsl/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/app/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/app/bash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/app/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/app/futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/app/python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.126580 parsl-2023.6.5/parsl/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/benchmark/perf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.126580 parsl-2023.6.5/parsl/channels/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/channels/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/channels/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.126580 parsl-2023.6.5/parsl/channels/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/channels/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/channels/local/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.126580 parsl-2023.6.5/parsl/channels/oauth_ssh/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/channels/oauth_ssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/channels/oauth_ssh/oauth_ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.126580 parsl-2023.6.5/parsl/channels/ssh/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/channels/ssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/channels/ssh/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.126580 parsl-2023.6.5/parsl/channels/ssh_il/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/channels/ssh_il/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/channels/ssh_il/ssh_il.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.126580 parsl-2023.6.5/parsl/concurrent/
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/concurrent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.130580 parsl-2023.6.5/parsl/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/ASPIRE1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/Azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/ad_hoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/bluewaters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/bridges.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/cc_in2p3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/comet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/cooley.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/cori.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/exex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/frontera.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/illinoiscluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/local_threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/midway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/osg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/polaris.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/stampede2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/summit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/theta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/toss3_llnl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/configs/wqex_local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.130580 parsl-2023.6.5/parsl/data_provider/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/data_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/data_provider/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/data_provider/file_noop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/data_provider/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/data_provider/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/data_provider/globus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/data_provider/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/data_provider/rsync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/data_provider/staging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.134580 parsl-2023.6.5/parsl/dataflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/dataflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62269 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/dataflow/dflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/dataflow/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/dataflow/executor_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/dataflow/futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/dataflow/job_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/dataflow/job_status_poller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/dataflow/memoization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/dataflow/rundirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/dataflow/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/dataflow/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/dataflow/taskrecord.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.134580 parsl-2023.6.5/parsl/executors/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.134580 parsl-2023.6.5/parsl/executors/extreme_scale/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/extreme_scale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/extreme_scale/executor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18710 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/extreme_scale/mpi_worker_pool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.134580 parsl-2023.6.5/parsl/executors/flux/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/flux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/flux/execute_parsl_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16987 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/flux/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/flux/flux_instance_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.138580 parsl-2023.6.5/parsl/executors/high_throughput/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/high_throughput/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/high_throughput/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33191 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/high_throughput/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29976 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/high_throughput/interchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/high_throughput/manager_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/high_throughput/monitoring_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/high_throughput/probe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33011 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/high_throughput/process_worker_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/high_throughput/zmq_pipes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/status_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/swift_t.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/threads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.138580 parsl-2023.6.5/parsl/executors/workqueue/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/workqueue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/workqueue/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/workqueue/exec_parsl_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48137 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/workqueue/executor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5514 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/workqueue/parsl_coprocess.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      735 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/executors/workqueue/parsl_coprocess_stub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.138580 parsl-2023.6.5/parsl/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/launchers/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15853 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/launchers/launchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/log_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.142580 parsl-2023.6.5/parsl/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36233 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/db_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/message_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23301 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.142580 parsl-2023.6.5/parsl/monitoring/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/queries/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/radios.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13172 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.142580 parsl-2023.6.5/parsl/monitoring/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.142580 parsl-2023.6.5/parsl/monitoring/visualization/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/plots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.142580 parsl-2023.6.5/parsl/monitoring/visualization/plots/default/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/plots/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/plots/default/task_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/plots/default/workflow_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.142580 parsl-2023.6.5/parsl/monitoring/visualization/static/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14199 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/static/parsl-logo-white.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)      337 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/static/parsl-monitor.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.142580 parsl-2023.6.5/parsl/monitoring/visualization/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/templates/app.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/templates/dag.html
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/templates/error.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/templates/resource_usage.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/templates/task.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/templates/workflow.html
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/templates/workflows_summary.html
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/monitoring/visualization/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/process_loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.146580 parsl-2023.6.5/parsl/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.146580 parsl-2023.6.5/parsl/providers/ad_hoc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/ad_hoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/ad_hoc/ad_hoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.146580 parsl-2023.6.5/parsl/providers/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29073 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/aws/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/aws/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.146580 parsl-2023.6.5/parsl/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18367 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/azure/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/azure/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/cluster_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.146580 parsl-2023.6.5/parsl/providers/cobalt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/cobalt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/cobalt/cobalt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      273 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/cobalt/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.146580 parsl-2023.6.5/parsl/providers/condor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/condor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13183 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/condor/condor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/condor/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.146580 parsl-2023.6.5/parsl/providers/googlecloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/googlecloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/googlecloud/googlecloud.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.146580 parsl-2023.6.5/parsl/providers/grid_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/grid_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/grid_engine/grid_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/grid_engine/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.146580 parsl-2023.6.5/parsl/providers/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12775 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/kubernetes/kube.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/kubernetes/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.150580 parsl-2023.6.5/parsl/providers/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/local/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.150580 parsl-2023.6.5/parsl/providers/lsf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/lsf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/lsf/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/lsf/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.150580 parsl-2023.6.5/parsl/providers/pbspro/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/pbspro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/pbspro/pbspro.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/pbspro/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.150580 parsl-2023.6.5/parsl/providers/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11702 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/slurm/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/slurm/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.150580 parsl-2023.6.5/parsl/providers/torque/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/torque/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/torque/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/providers/torque/torque.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.150580 parsl-2023.6.5/parsl/serialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/serialize/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/serialize/concretes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/serialize/facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.154580 parsl-2023.6.5/parsl/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/callables_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.158580 parsl-2023.6.5/parsl/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/ad_hoc_cluster_htex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/azure_single_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/bluewaters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/bridges.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/cc_in2p3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/comet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/cooley_htex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/cori.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/ec2_single_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/ec2_spot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/exex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/frontera.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/htex_ad_hoc_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/htex_local_alternate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/htex_local_intask_staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/htex_local_rsync_staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/local_adhoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/local_threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/local_threads_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/local_threads_checkpoint_dfk_exit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/local_threads_checkpoint_periodic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/local_threads_checkpoint_task_exit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/local_threads_ftp_in_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/local_threads_globus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/local_threads_http_in_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/local_threads_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/local_threads_no_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/midway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/nscc_singapore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/osg_htex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/petrelkube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/summit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/swan_htex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/theta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/user_opts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/workqueue_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/configs/workqueue_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9382 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.158580 parsl-2023.6.5/parsl/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/latency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.158580 parsl-2023.6.5/parsl/tests/integration/test_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/test_apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.162580 parsl-2023.6.5/parsl/tests/integration/test_channels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/test_channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/test_channels/test_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/test_channels/test_local_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/test_channels/test_scp_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/test_channels/test_ssh_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/test_channels/test_ssh_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/test_channels/test_ssh_file_transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/test_channels/test_ssh_interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/test_parsl_load_default_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.162580 parsl-2023.6.5/parsl/tests/integration/test_stress/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/test_stress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/test_stress/test_python_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/integration/test_stress/test_python_threads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.162580 parsl-2023.6.5/parsl/tests/manual_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/manual_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/manual_tests/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/manual_tests/test_ad_hoc_htex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/manual_tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/manual_tests/test_log_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/manual_tests/test_memory_limits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/manual_tests/test_oauth_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/manual_tests/test_regression_220.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/manual_tests/test_udp_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/manual_tests/test_worker_count.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.162580 parsl-2023.6.5/parsl/tests/site_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/site_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/site_tests/site_config_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/site_tests/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/site_tests/test_site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.162580 parsl-2023.6.5/parsl/tests/sites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/sites/test_affinity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/sites/test_concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/sites/test_dynamic_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/sites/test_ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/sites/test_launchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/sites/test_local_adhoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.162580 parsl-2023.6.5/parsl/tests/sites/test_mpi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/sites/test_mpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/sites/test_start_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/sites/test_worker_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_aalst_patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.166580 parsl-2023.6.5/parsl/tests/test_bash_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_bash_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_bash_apps/test_apptimeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_bash_apps/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_bash_apps/test_error_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_bash_apps/test_keyword_overlaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_bash_apps/test_kwarg_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_bash_apps/test_memoize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_bash_apps/test_memoize_ignore_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_bash_apps/test_multiline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_bash_apps/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_bash_apps/test_stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_callables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.166580 parsl-2023.6.5/parsl/tests/test_channels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_channels/test_large_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.166580 parsl-2023.6.5/parsl/tests/test_checkpointing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_checkpointing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_checkpointing/test_periodic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_checkpointing/test_python_checkpoint_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_checkpointing/test_python_checkpoint_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_checkpointing/test_python_checkpoint_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_checkpointing/test_regression_232.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_checkpointing/test_regression_233.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_checkpointing/test_regression_239.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_checkpointing/test_task_exit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.166580 parsl-2023.6.5/parsl/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_data/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_data/test_file_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_data/test_file_staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_data/test_output_chain_filenames.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.170580 parsl-2023.6.5/parsl/tests/test_docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_docs/test_from_slides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_docs/test_tutorial_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_docs/test_workflow1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_docs/test_workflow2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_docs/test_workflow3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_docs/test_workflow4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.170580 parsl-2023.6.5/parsl/tests/test_error_handling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_error_handling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_error_handling/test_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_error_handling/test_htex_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_error_handling/test_htex_missing_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_error_handling/test_htex_worker_failure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_error_handling/test_python_walltime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_error_handling/test_rand_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_error_handling/test_resource_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_error_handling/test_retries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_error_handling/test_retry_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_error_handling/test_retry_handler_failure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_error_handling/test_serialization_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_error_handling/test_wrap_with_logs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.170580 parsl-2023.6.5/parsl/tests/test_flowcontrol/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_flowcontrol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_flux.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.170580 parsl-2023.6.5/parsl/tests/test_monitoring/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_monitoring/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_monitoring/test_db_locks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_monitoring/test_fuzz_zmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_monitoring/test_memoization_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_monitoring/test_viz_colouring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.174580 parsl-2023.6.5/parsl/tests/test_providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_providers/test_local_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.178580 parsl-2023.6.5/parsl/tests/test_python_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_arg_input_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_at_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_dep_standard_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_depfail_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_fibonacci_iterative.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_fibonacci_recursive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_garbage_collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_import_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_mapred.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_memoize_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_memoize_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_memoize_4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_memoize_ignore_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_memoize_joinapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_type5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_python_apps/test_worker_fail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.182580 parsl-2023.6.5/parsl/tests/test_regression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_regression/test_1480.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_regression/test_1606_wait_for_current_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_regression/test_1653.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_regression/test_221.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_regression/test_226.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_regression/test_2652.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_regression/test_69a.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_regression/test_69b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_regression/test_854.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_regression/test_97_parallelism_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_regression/test_98.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.182580 parsl-2023.6.5/parsl/tests/test_scaling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_scaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_scaling/test_regression_1621.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_scaling/test_scale_down.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.186580 parsl-2023.6.5/parsl/tests/test_staging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_staging/staging_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_staging/test_1316.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_staging/test_docs_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_staging/test_docs_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_staging/test_elaborate_noop_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_staging/test_staging_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_staging/test_staging_ftp_in_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_staging/test_staging_globus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_staging/test_staging_https.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_staging/test_staging_https_in_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_swift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_thread_parallelism.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.186580 parsl-2023.6.5/parsl/tests/test_threads/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_threads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_threads/test_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/test_threads/test_lazy_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.190580 parsl-2023.6.5/parsl/tests/workqueue_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/workqueue_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/workqueue_tests/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/workqueue_tests/local_threads.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3835 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/workqueue_tests/test_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/workqueue_tests/wqex_condor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/tests/workqueue_tests/wqex_local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.190580 parsl-2023.6.5/parsl/usage_tracking/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/usage_tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/usage_tracking/usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10885 2023-06-05 22:43:01.000000 parsl-2023.6.5/parsl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-05 22:43:09.000000 parsl-2023.6.5/parsl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:43:11.122580 parsl-2023.6.5/parsl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-05 22:43:11.000000 parsl-2023.6.5/parsl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15508 2023-06-05 22:43:11.000000 parsl-2023.6.5/parsl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 22:43:11.000000 parsl-2023.6.5/parsl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-05 22:43:11.000000 parsl-2023.6.5/parsl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-05 22:43:11.000000 parsl-2023.6.5/parsl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 22:43:11.000000 parsl-2023.6.5/parsl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-05 22:43:01.000000 parsl-2023.6.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 22:43:11.190580 parsl-2023.6.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2624 2023-06-05 22:43:01.000000 parsl-2023.6.5/setup.py
```

### Comparing `parsl-2023.6.19/LICENSE` & `parsl-2023.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/PKG-INFO` & `parsl-2023.6.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: parsl
-Version: 2023.6.19
+Version: 2023.6.5
 Summary: Simple data dependent workflows in Python
 Home-page: https://github.com/Parsl/parsl
-Download-URL: https://github.com/Parsl/parsl/archive/2023.06.19.tar.gz
+Download-URL: https://github.com/Parsl/parsl/archive/2023.06.05.tar.gz
 Author: The Parsl Team
 Author-email: parsl@googlegroups.com
 License: Apache 2.0
 Keywords: Workflows,Scientific computing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `parsl-2023.6.19/README.rst` & `parsl-2023.6.5/README.rst`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/__init__.py` & `parsl-2023.6.5/parsl/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/addresses.py` & `parsl-2023.6.5/parsl/addresses.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,16 +109,15 @@
     for interface in net_interfaces:
         try:
             s_addresses.add(address_by_interface(interface))
         except Exception:
             logger.exception("Ignoring failure to fetch address from interface {}".format(interface))
             pass
 
-    resolution_functions: List[Callable[[], str]]
-    resolution_functions = [address_by_hostname, address_by_route, address_by_query]
+    resolution_functions = [address_by_hostname, address_by_route, address_by_query]  # type: List[Callable[[], str]]
     for f in resolution_functions:
         try:
             s_addresses.add(f())
         except Exception:
             logger.exception("Ignoring an address finder exception")
 
     return s_addresses
```

### Comparing `parsl-2023.6.19/parsl/app/app.py` & `parsl-2023.6.5/parsl/app/app.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/app/bash.py` & `parsl-2023.6.5/parsl/app/bash.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/app/errors.py` & `parsl-2023.6.5/parsl/app/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/app/futures.py` & `parsl-2023.6.5/parsl/app/futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/app/python.py` & `parsl-2023.6.5/parsl/app/python.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/benchmark/perf.py` & `parsl-2023.6.5/parsl/benchmark/perf.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/channels/base.py` & `parsl-2023.6.5/parsl/channels/base.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/channels/errors.py` & `parsl-2023.6.5/parsl/channels/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/channels/local/local.py` & `parsl-2023.6.5/parsl/channels/local/local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/channels/oauth_ssh/oauth_ssh.py` & `parsl-2023.6.5/parsl/channels/oauth_ssh/oauth_ssh.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/channels/ssh/ssh.py` & `parsl-2023.6.5/parsl/channels/ssh/ssh.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/channels/ssh_il/ssh_il.py` & `parsl-2023.6.5/parsl/channels/ssh_il/ssh_il.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/concurrent/__init__.py` & `parsl-2023.6.5/parsl/concurrent/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/config.py` & `parsl-2023.6.5/parsl/config.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/configs/ASPIRE1.py` & `parsl-2023.6.5/parsl/configs/ASPIRE1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/configs/Azure.py` & `parsl-2023.6.5/parsl/configs/Azure.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/configs/ad_hoc.py` & `parsl-2023.6.5/parsl/configs/ad_hoc.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/configs/bluewaters.py` & `parsl-2023.6.5/parsl/configs/bluewaters.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/configs/bridges.py` & `parsl-2023.6.5/parsl/configs/bridges.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/configs/cc_in2p3.py` & `parsl-2023.6.5/parsl/configs/cc_in2p3.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/configs/comet.py` & `parsl-2023.6.5/parsl/configs/comet.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/configs/cooley.py` & `parsl-2023.6.5/parsl/configs/cooley.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/configs/cori.py` & `parsl-2023.6.5/parsl/configs/cori.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/configs/ec2.py` & `parsl-2023.6.5/parsl/configs/ec2.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/configs/exex_local.py` & `parsl-2023.6.5/parsl/configs/exex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/configs/frontera.py` & `parsl-2023.6.5/parsl/configs/frontera.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/configs/illinoiscluster.py` & `parsl-2023.6.5/parsl/configs/illinoiscluster.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/configs/kubernetes.py` & `parsl-2023.6.5/parsl/configs/kubernetes.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/configs/midway.py` & `parsl-2023.6.5/parsl/configs/midway.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/configs/osg.py` & `parsl-2023.6.5/parsl/configs/osg.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/configs/polaris.py` & `parsl-2023.6.5/parsl/configs/polaris.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/configs/stampede2.py` & `parsl-2023.6.5/parsl/configs/stampede2.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/configs/summit.py` & `parsl-2023.6.5/parsl/configs/summit.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/configs/theta.py` & `parsl-2023.6.5/parsl/configs/theta.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/configs/toss3_llnl.py` & `parsl-2023.6.5/parsl/configs/toss3_llnl.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/configs/wqex_local.py` & `parsl-2023.6.5/parsl/configs/wqex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/data_provider/data_manager.py` & `parsl-2023.6.5/parsl/data_provider/data_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 if TYPE_CHECKING:
     from parsl.dataflow.dflow import DataFlowKernel
 
 logger = logging.getLogger(__name__)
 
 # these will be shared between all executors that do not explicitly
 # override, so should not contain executor-specific state
-default_staging: List[Staging]
-default_staging = [NoOpFileStaging(), FTPSeparateTaskStaging(), HTTPSeparateTaskStaging()]
+default_staging = [NoOpFileStaging(), FTPSeparateTaskStaging(), HTTPSeparateTaskStaging()]  # type: List[Staging]
 
 
 class DataManager:
     """The DataManager is responsible for transferring input and output data.
 
     """
```

### Comparing `parsl-2023.6.19/parsl/data_provider/files.py` & `parsl-2023.6.5/parsl/data_provider/files.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         """
         self.url = url
         parsed_url = urlparse(self.url)
         self.scheme = parsed_url.scheme if parsed_url.scheme else 'file'
         self.netloc = parsed_url.netloc
         self.path = parsed_url.path
         self.filename = os.path.basename(self.path)
-        self.local_path: Optional[str] = None
+        self.local_path = None  # type: Optional[str]
 
     def cleancopy(self) -> "File":
         """Returns a copy of the file containing only the global immutable state,
            without any mutable site-local local_path information. The returned File
            object will be as the original object was when it was constructed.
         """
         logger.debug("Making clean copy of File object {}".format(repr(self)))
```

### Comparing `parsl-2023.6.19/parsl/data_provider/ftp.py` & `parsl-2023.6.5/parsl/data_provider/ftp.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/data_provider/globus.py` & `parsl-2023.6.5/parsl/data_provider/globus.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/data_provider/http.py` & `parsl-2023.6.5/parsl/data_provider/http.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/data_provider/rsync.py` & `parsl-2023.6.5/parsl/data_provider/rsync.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/data_provider/staging.py` & `parsl-2023.6.5/parsl/data_provider/staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/dataflow/dflow.py` & `parsl-2023.6.5/parsl/dataflow/dflow.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/dataflow/errors.py` & `parsl-2023.6.5/parsl/dataflow/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/dataflow/futures.py` & `parsl-2023.6.5/parsl/dataflow/futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/dataflow/job_error_handler.py` & `parsl-2023.6.5/parsl/dataflow/job_error_handler.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/dataflow/job_status_poller.py` & `parsl-2023.6.5/parsl/dataflow/job_status_poller.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/dataflow/memoization.py` & `parsl-2023.6.5/parsl/dataflow/memoization.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,15 +172,15 @@
         Args:
             - task (dict) : Task dictionary from dfk.tasks
 
         Returns:
             - hash (str) : A unique hash string
         """
 
-        t: List[bytes] = []
+        t = []  # type: List[bytes]
 
         # if kwargs contains an outputs parameter, that parameter is removed
         # and normalised differently - with output_ref set to True.
         # kwargs listed in ignore_for_cache will also be removed
 
         filtered_kw = task['kwargs'].copy()
```

### Comparing `parsl-2023.6.19/parsl/dataflow/rundirs.py` & `parsl-2023.6.5/parsl/dataflow/rundirs.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/dataflow/states.py` & `parsl-2023.6.5/parsl/dataflow/states.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/dataflow/strategy.py` & `parsl-2023.6.5/parsl/dataflow/strategy.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/dataflow/taskrecord.py` & `parsl-2023.6.5/parsl/dataflow/taskrecord.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/errors.py` & `parsl-2023.6.5/parsl/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/executors/base.py` & `parsl-2023.6.5/parsl/executors/base.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/executors/errors.py` & `parsl-2023.6.5/parsl/executors/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/executors/extreme_scale/executor.py` & `parsl-2023.6.5/parsl/executors/extreme_scale/executor.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/executors/extreme_scale/mpi_worker_pool.py` & `parsl-2023.6.5/parsl/executors/extreme_scale/mpi_worker_pool.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/executors/flux/execute_parsl_task.py` & `parsl-2023.6.5/parsl/executors/flux/execute_parsl_task.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/executors/flux/executor.py` & `parsl-2023.6.5/parsl/executors/flux/executor.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/executors/flux/flux_instance_manager.py` & `parsl-2023.6.5/parsl/executors/flux/flux_instance_manager.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/executors/high_throughput/executor.py` & `parsl-2023.6.5/parsl/executors/high_throughput/executor.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/executors/high_throughput/interchange.py` & `parsl-2023.6.5/parsl/executors/high_throughput/interchange.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/executors/high_throughput/probe.py` & `parsl-2023.6.5/parsl/executors/high_throughput/probe.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/executors/high_throughput/process_worker_pool.py` & `parsl-2023.6.5/parsl/executors/high_throughput/process_worker_pool.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/executors/high_throughput/zmq_pipes.py` & `parsl-2023.6.5/parsl/executors/high_throughput/zmq_pipes.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/executors/status_handling.py` & `parsl-2023.6.5/parsl/executors/status_handling.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/executors/swift_t.py` & `parsl-2023.6.5/parsl/executors/swift_t.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/executors/taskvine/exec_parsl_function.py` & `parsl-2023.6.5/parsl/executors/workqueue/exec_parsl_function.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/executors/taskvine/executor.py` & `parsl-2023.6.5/parsl/executors/workqueue/executor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" TaskVineExecutor utilizes the TaskVine distributed framework developed by the
+""" WorkQueueExecutor utilizes the Work Queue distributed framework developed by the
 Cooperative Computing Lab (CCL) at Notre Dame to provide a fault-tolerant,
 high-throughput system for delegating Parsl tasks to thousands of remote machines
 """
 
 import threading
 import multiprocessing
 import logging
@@ -25,376 +25,369 @@
 import parsl.utils as putils
 from parsl.executors.errors import ExecutorError
 from parsl.data_provider.files import File
 from parsl.errors import OptionalModuleMissing
 from parsl.executors.status_handling import BlockProviderExecutor
 from parsl.providers.base import ExecutionProvider
 from parsl.providers import LocalProvider, CondorProvider
-from parsl.executors.taskvine import exec_parsl_function
+from parsl.executors.workqueue import exec_parsl_function
 from parsl.process_loggers import wrap_with_logs
 from parsl.utils import setproctitle
 
 import typeguard
-from typing import Dict, List, Optional, Union
+from typing import Dict, List, Optional, Set, Union
 from parsl.data_provider.staging import Staging
 
-from .errors import TaskVineTaskFailure
-from .errors import TaskVineFailure
+from .errors import WorkQueueTaskFailure
+from .errors import WorkQueueFailure
 
 from collections import namedtuple
 
 try:
-    from ndcctools.taskvine import cvine
-    from ndcctools.taskvine import Manager
-    from ndcctools.taskvine import Task
-    from ndcctools.taskvine.cvine import VINE_DEFAULT_PORT
-    from ndcctools.taskvine.cvine import VINE_ALLOCATION_MODE_MAX_THROUGHPUT
+    import work_queue as wq
+    from work_queue import WorkQueue
+    from work_queue import WORK_QUEUE_DEFAULT_PORT
+    from work_queue import WORK_QUEUE_ALLOCATION_MODE_MAX_THROUGHPUT
 except ImportError:
-    _taskvine_enabled = False
-    VINE_DEFAULT_PORT = 0
+    _work_queue_enabled = False
+    WORK_QUEUE_DEFAULT_PORT = 0
 else:
-    _taskvine_enabled = True
+    _work_queue_enabled = True
 
-package_analyze_script = shutil.which("poncho_package_analyze")
-package_create_script = shutil.which("poncho_package_create")
-package_run_script = shutil.which("poncho_package_run")
+package_analyze_script = shutil.which("python_package_analyze")
+package_create_script = shutil.which("python_package_create")
+package_run_script = shutil.which("python_package_run")
 
 logger = logging.getLogger(__name__)
 
 
-# Support structure to communicate parsl tasks to the taskvine submit thread.
-ParslTaskToVine = namedtuple('ParslTaskToVine',
-                             'id category cores memory disk gpus priority running_time_min \
-                              env_pkg map_file function_file result_file input_files output_files')
+# Support structure to communicate parsl tasks to the work queue submit thread.
+ParslTaskToWq = namedtuple('ParslTaskToWq',
+                           'id category cores memory disk gpus priority running_time_min env_pkg map_file function_file result_file input_files output_files')
 
-# Support structure to communicate final status of taskvine tasks to parsl
+# Support structure to communicate final status of work queue tasks to parsl
 # result is only valid if result_received is True
 # reason and status are only valid if result_received is False
-VineTaskToParsl = namedtuple('VineTaskToParsl', 'id result_received result reason status')
+WqTaskToParsl = namedtuple('WqTaskToParsl', 'id result_received result reason status')
 
-# Support structure to report parsl filenames to taskvine.
+# Support structure to report parsl filenames to work queue.
 # parsl_name is the local_name or filepath attribute of a parsl file object.
-# stage tells whether the file should be copied by taskvine to the workers.
+# stage tells whether the file should be copied by work queue to the workers.
 # cache tells whether the file should be cached at workers. Only valid if stage == True
-ParslFileToVine = namedtuple('ParslFileToVine', 'parsl_name stage cache')
+ParslFileToWq = namedtuple('ParslFileToWq', 'parsl_name stage cache')
 
 
-class TaskVineExecutor(BlockProviderExecutor, putils.RepresentationMixin):
-    """Executor to use TaskVine batch system
+class WorkQueueExecutor(BlockProviderExecutor, putils.RepresentationMixin):
+    """Executor to use Work Queue batch system
 
-    The TaskVineExecutor system utilizes the TaskVine framework to
+    The WorkQueueExecutor system utilizes the Work Queue framework to
     efficiently delegate Parsl apps to remote machines in clusters and
     grids using a fault-tolerant system. Users can run the
-    vine_worker program on remote machines to connect to the
-    TaskVineExecutor, and Parsl apps will then be sent out to these
+    work_queue_worker program on remote machines to connect to the
+    WorkQueueExecutor, and Parsl apps will then be sent out to these
     machines for execution and retrieval.
 
 
     Parameters
     ----------
 
         label: str
             A human readable label for the executor, unique
-            with respect to other TaskVine master programs.
-            Default is "TaskVineExecutor".
+            with respect to other Work Queue master programs.
+            Default is "WorkQueueExecutor".
+
+        working_dir: str
+            Location for Parsl to perform app delegation to the Work
+            Queue system. Defaults to current directory.
 
         project_name: str
-            If a project_name is given, then TaskVine will periodically
-            report its status and performance back to the global TaskVine catalog,
-            which can be viewed here:  http://ccl.cse.nd.edu/software/taskvine/status
+            If a project_name is given, then Work Queue will periodically
+            report its status and performance back to the global WQ catalog,
+            which can be viewed here:  http://ccl.cse.nd.edu/software/workqueue/status
             Default is None.  Overrides address.
 
         project_password_file: str
-            Optional password file for the taskvine project. Default is None.
+            Optional password file for the work queue project. Default is None.
 
         address: str
-            The ip to contact this taskvine master process.
+            The ip to contact this work queue master process.
             If not given, uses the address of the current machine as returned
             by socket.gethostname().
             Ignored if project_name is specified.
 
         port: int
-            TCP port on Parsl submission machine for TaskVine workers
+            TCP port on Parsl submission machine for Work Queue workers
             to connect to. Workers will connect to Parsl using this port.
 
-            If 0, TaskVine will allocate a port number automatically.
+            If 0, Work Queue will allocate a port number automatically.
             In this case, environment variables can be used to influence the
             choice of port, documented here:
-            https://cctools.readthedocs.io/en/stable/api/html/taskvine_8h.html#a47ac70464e357e4dfcb0722fee6c44a0
-            Default is VINE_DEFAULT_PORT.
+            https://ccl.cse.nd.edu/software/manuals/api/html/work__queue_8h.html#a21714a10bcdfcf5c3bd44a96f5dcbda6
+
+            Default: 0.
 
         env: dict{str}
             Dictionary that contains the environmental variables that
-            need to be set on the TaskVine worker machine.
+            need to be set on the Work Queue worker machine.
 
         shared_fs: bool
             Define if working in a shared file system or not. If Parsl
-            and the TaskVine workers are on a shared file system, TaskVine
-            does not need to transfer and rename files for execution.
+            and the Work Queue workers are on a shared file system, Work
+            Queue does not need to transfer and rename files for execution.
             Default is False.
 
         use_cache: bool
-            Whether workers should cache files of tasks.
-            Default is True.
+            Whether workers should cache files that are common to tasks.
+            Warning: Two files are considered the same if they have the same
+            filepath name. Use with care when reusing the executor instance
+            across multiple parsl workflows. Default is False.
 
         source: bool
             Choose whether to transfer parsl app information as
             source code. (Note: this increases throughput for
             @python_apps, but the implementation does not include
             functionality for @bash_apps, and thus source=False
             must be used for programs utilizing @bash_apps.)
-            Default is False. Set to True if pack is True.
+            Default is False. Set to True if pack is True
 
         pack: bool
             Use conda-pack to prepare a self-contained Python evironment for
             each task. This greatly increases task latency, but does not
             require a common environment or shared FS on execution nodes.
-            Implies source=True. Default is False.
-
-        pack_env: str
-            An already prepared environment tarball using poncho_package_create
-            to attach to each task.
-            Default is "".
+            Implies source=True.
 
         extra_pkgs: list
             List of extra pip/conda package names to include when packing
             the environment. This may be useful if the app executes other
             (possibly non-Python) programs provided via pip or conda.
             Scanning the app source for imports would not detect these
             dependencies, so they need to be manually specified.
 
         autolabel: bool
             Use the Resource Monitor to automatically determine resource
             labels based on observed task behavior.
 
         autolabel_window: int
-            Set the number of tasks considered for autolabeling. TaskVine
+            Set the number of tasks considered for autolabeling. Work Queue
             will wait for a series of N tasks with steady resource
             requirements before making a decision on labels. Increasing
             this parameter will reduce the number of failed tasks due to
             resource exhaustion when autolabeling, at the cost of increased
             resources spent collecting stats.
 
         autocategory: bool
             Place each app in its own category by default. If all
             invocations of an app have similar performance characteristics,
             this will provide a reasonable set of categories automatically.
-            Default is True.
 
-        max_retries: int
-            Set the number of retries that TaskVine will make when a task
+        max_retries: Optional[int]
+            Set the number of retries that Work Queue will make when a task
             fails. This is distinct from Parsl level retries configured in
-            parsl.config.Config. Set to None to allow TaskVine to retry
+            parsl.config.Config. Set to None to allow Work Queue to retry
             tasks forever. By default, this is set to 1, so that all retries
             will be managed by Parsl.
 
         init_command: str
             Command line to run before executing a task in a worker.
             Default is ''.
 
         worker_options: str
-            Extra options passed to vine_worker. Default is ''.
+            Extra options passed to work_queue_worker. Default is ''.
 
         worker_executable: str
-            The command used to invoke vine_worker. This can be used
+            The command used to invoke work_queue_worker. This can be used
             when the worker needs to be wrapped inside some other command
             (for example, to run the worker inside a container). Default is
-            'vine_worker'.
+            'work_queue_worker'.
 
         function_dir: str
             The directory where serialized function invocations are placed
             to be sent to workers. If undefined, this defaults to a directory
             under runinfo/. If shared_filesystem=True, then this directory
             must be visible from both the submitting side and workers.
 
-        wait_for_workers: int
-            The number of workers to wait for before running any task.
-            Default is 0, so the manager won't wait for workers to connect.
-
-        enable_peer_transfers: bool
-            Option to enable transferring files between workers.
-            Default is True.
-
-        full_debug: bool
-            Whether to enable full debug mode for monitoring in TaskVine.
+        coprocess: bool
+            Use Work Queue's coprocess facility to avoid launching a new Python
+            process for each task. Experimental.
+            This requires a version of Work Queue / cctools after commit
+            874df524516441da531b694afc9d591e8b134b73 (release 7.5.0 is too early).
             Default is False.
-
-        provider: ExecutionProvider
-            The Parsl provider that will spawn worker processes.
-            Default to spawning one local vine worker process.
-
-        storage_access: Optional[List[Staging]]
-            Define Parsl file staging providers for this executor.
-            Default is None.
     """
 
     radio_mode = "filesystem"
 
     @typeguard.typechecked
     def __init__(self,
-                 label: str = "TaskVineExecutor",
+                 label: str = "WorkQueueExecutor",
+                 provider: ExecutionProvider = LocalProvider(),
+                 working_dir: str = ".",
                  project_name: Optional[str] = None,
                  project_password_file: Optional[str] = None,
                  address: Optional[str] = None,
-                 port: int = VINE_DEFAULT_PORT,
+                 port: int = WORK_QUEUE_DEFAULT_PORT,
                  env: Optional[Dict] = None,
                  shared_fs: bool = False,
-                 use_cache: bool = True,
+                 storage_access: Optional[List[Staging]] = None,
+                 use_cache: bool = False,
                  source: bool = False,
                  pack: bool = False,
-                 pack_env: str = "",
                  extra_pkgs: Optional[List[str]] = None,
                  autolabel: bool = False,
                  autolabel_window: int = 1,
                  autocategory: bool = True,
-                 max_retries: int = 1,
+                 max_retries: Optional[int] = 1,
                  init_command: str = "",
                  worker_options: str = "",
-                 worker_executable: str = 'vine_worker',
+                 full_debug: bool = True,
+                 worker_executable: str = 'work_queue_worker',
                  function_dir: Optional[str] = None,
-                 wait_for_workers: int = 0,
-                 enable_peer_transfers: bool = True,
-                 full_debug: bool = False,
-                 provider: ExecutionProvider = LocalProvider(),
-                 storage_access: Optional[List[Staging]] = None):
+                 coprocess: bool = False):
         BlockProviderExecutor.__init__(self, provider=provider,
                                        block_error_handler=True)
-        if not _taskvine_enabled:
-            raise OptionalModuleMissing(['taskvine'], "TaskVineExecutor requires the taskvine module.")
+        if not _work_queue_enabled:
+            raise OptionalModuleMissing(['work_queue'], "WorkQueueExecutor requires the work_queue module.")
 
         self.label = label
-        self.project_name = project_name
-        self.project_password_file = project_password_file
+        self.task_queue = multiprocessing.Queue()  # type: multiprocessing.Queue
+        self.collector_queue = multiprocessing.Queue()  # type: multiprocessing.Queue
+        self.blocks = {}  # type: Dict[str, str]
         self.address = address
         self.port = port
+        self.executor_task_counter = -1
+        self.project_name = project_name
+        self.project_password_file = project_password_file
         self.env = env
+        self.init_command = init_command
         self.shared_fs = shared_fs
+        self.storage_access = storage_access
         self.use_cache = use_cache
+        self.working_dir = working_dir
+        self.registered_files = set()  # type: Set[str]
+        self.full_debug = full_debug
         self.source = True if pack else source
         self.pack = pack
-        self.pack_env = pack_env
         self.extra_pkgs = extra_pkgs or []
         self.autolabel = autolabel
         self.autolabel_window = autolabel_window
         self.autocategory = autocategory
         self.max_retries = max_retries
-        self.init_command = init_command
+        self.should_stop = multiprocessing.Value(c_bool, False)
+        self.cached_envs = {}  # type: Dict[int, str]
         self.worker_options = worker_options
         self.worker_executable = worker_executable
         self.function_dir = function_dir
-        self.wait_for_workers = wait_for_workers
-        self.enable_peer_transfers = enable_peer_transfers
-        self.full_debug = full_debug
-        self.storage_access = storage_access
-
-        # Queue to send tasks from TaskVine executor process to TaskVine manager process
-        self.task_queue: multiprocessing.Queue = multiprocessing.Queue()
-
-        # Queue to send tasks from TaskVine manager process to TaskVine executor process
-        self.collector_queue: multiprocessing.Queue = multiprocessing.Queue()
-
-        self.blocks: Dict[str, str] = {}  # track Parsl blocks
-        self.executor_task_counter = -1  # task id starts from 0
-        self.should_stop = multiprocessing.Value(c_bool, False)
-
-        # mapping of function's unique memory address to its solved environment
-        self.cached_envs: Dict[int, str] = {}
+        self.coprocess = coprocess
 
         if not self.address:
             self.address = socket.gethostname()
 
         if self.project_password_file is not None and not os.path.exists(self.project_password_file):
-            raise TaskVineFailure('Could not find password file: {}'.format(self.project_password_file))
+            raise WorkQueueFailure('Could not find password file: {}'.format(self.project_password_file))
+
+        if self.project_password_file is not None:
+            if os.path.exists(self.project_password_file) is False:
+                logger.debug("Password File does not exist, no file used")
+                self.project_password_file = None
 
         # Build foundations of the launch command
-        self.launch_cmd = ("python3 exec_parsl_function.py {mapping} {function} {result}")
+        self.launch_cmd = ("{package_prefix}python3 exec_parsl_function.py {mapping} {function} {result}")
         if self.init_command != "":
             self.launch_cmd = self.init_command + "; " + self.launch_cmd
 
     def _get_launch_command(self, block_id):
         # this executor uses different terminology for worker/launch
         # commands than in htex
         return f"PARSL_WORKER_BLOCK_ID={block_id} {self.worker_command}"
 
     def start(self):
         """Create submit process and collector thread to create, send, and
-        retrieve Parsl tasks within the TaskVine system.
+        retrieve Parsl tasks within the Work Queue system.
         """
         self.tasks_lock = threading.Lock()
 
         # Create directories for data and results
         if not self.function_dir:
             self.function_data_dir = os.path.join(self.run_dir, self.label, "function_data")
         else:
             tp = str(time.time())
             tx = os.path.join(self.function_dir, tp)
             os.makedirs(tx)
             self.function_data_dir = os.path.join(self.function_dir, tp, self.label, "function_data")
-        self.vine_log_dir = os.path.join(self.run_dir, self.label)
-        logger.debug("function data directory: {}\nlog directory: {}".format(self.function_data_dir, self.vine_log_dir))
-        os.makedirs(self.vine_log_dir)
+        self.package_dir = os.path.join(self.run_dir, self.label, "package_data")
+        self.wq_log_dir = os.path.join(self.run_dir, self.label)
+        logger.debug("function data directory: {}\nlog directory: {}".format(self.function_data_dir, self.wq_log_dir))
+        os.makedirs(self.wq_log_dir)
         os.makedirs(self.function_data_dir)
+        os.makedirs(self.package_dir)
 
-        logger.debug("Starting TaskVineExecutor")
+        logger.debug("Starting WorkQueueExecutor")
 
-        # Create a Process to perform TaskVine submissions
+        self._port_mailbox = multiprocessing.Queue()
+
+        # Create a Process to perform WorkQueue submissions
         submit_process_kwargs = {"task_queue": self.task_queue,
                                  "launch_cmd": self.launch_cmd,
-                                 "env": self.env,
+                                 "data_dir": self.function_data_dir,
                                  "collector_queue": self.collector_queue,
                                  "full": self.full_debug,
                                  "shared_fs": self.shared_fs,
                                  "autolabel": self.autolabel,
                                  "autolabel_window": self.autolabel_window,
                                  "autocategory": self.autocategory,
                                  "max_retries": self.max_retries,
                                  "should_stop": self.should_stop,
                                  "port": self.port,
-                                 "vine_log_dir": self.vine_log_dir,
+                                 "wq_log_dir": self.wq_log_dir,
                                  "project_password_file": self.project_password_file,
                                  "project_name": self.project_name,
-                                 "wait_for_workers": self.wait_for_workers,
-                                 "enable_peer_transfers": self.enable_peer_transfers}
-        self.submit_process = multiprocessing.Process(target=_taskvine_submit_wait,
-                                                      name="TaskVine-Submit-Process",
+                                 "port_mailbox": self._port_mailbox,
+                                 "coprocess": self.coprocess
+                                 }
+        self.submit_process = multiprocessing.Process(target=_work_queue_submit_wait,
+                                                      name="WorkQueue-Submit-Process",
                                                       kwargs=submit_process_kwargs)
 
-        self.collector_thread = threading.Thread(target=self._collect_taskvine_results,
-                                                 name="TaskVine-collector-thread")
+        self.collector_thread = threading.Thread(target=self._collect_work_queue_results,
+                                                 name="WorkQueue-collector-thread")
         self.collector_thread.daemon = True
 
         # Begin both processes
         self.submit_process.start()
         self.collector_thread.start()
 
+        self._chosen_port = self._port_mailbox.get(timeout=60)
+
+        logger.debug(f"Chosen listening port is {self._chosen_port}")
+
         # Initialize scaling for the provider
         self.initialize_scaling()
 
     def _path_in_task(self, executor_task_id, *path_components):
-        """Returns a filename fixed and specific to a task.
+        """Returns a filename specific to a task.
         It is used for the following filename's:
             (not given): The subdirectory per task that contains function, result, etc.
             'function': Pickled file that contains the function to be executed.
             'result': Pickled file that (will) contain the result of the function.
-            'map': Pickled file with a dict between local parsl names, and remote taskvine names.
+            'map': Pickled file with a dict between local parsl names, and remote work queue names.
         """
         task_dir = "{:04d}".format(executor_task_id)
         return os.path.join(self.function_data_dir, task_dir, *path_components)
 
     def submit(self, func, resource_specification, *args, **kwargs):
         """Processes the Parsl app by its arguments and submits the function
-        information to the task queue, to be executed using the TaskVine
+        information to the task queue, to be executed using the Work Queue
         system. The args and kwargs are processed for input and output files to
-        the Parsl app, so that the files are appropriately specified for the TaskVine task.
+        the Parsl app, so that the files are appropriately specified for the Work
+        Queue task.
 
         Parameters
         ----------
 
         func : function
-            Parsl app to be submitted to the TaskVine system
+            Parsl app to be submitted to the Work Queue system
         args : list
             Arguments to the Parsl app
         kwargs : dict
             Keyword arguments to the Parsl app
         """
         cores = None
         memory = None
@@ -450,104 +443,102 @@
 
         # Create a per task directory for the function, result, map, and result files
         os.mkdir(self._path_in_task(executor_task_id))
 
         input_files = []
         output_files = []
 
-        # Determine the input and output files that will exist at the workers:
+        # Determine the input and output files that will exist at the workes:
         input_files += [self._register_file(f) for f in kwargs.get("inputs", []) if isinstance(f, File)]
         output_files += [self._register_file(f) for f in kwargs.get("outputs", []) if isinstance(f, File)]
 
         # Also consider any *arg that looks like a file as an input:
         input_files += [self._register_file(f) for f in args if isinstance(f, File)]
 
         for kwarg, maybe_file in kwargs.items():
             # Add appropriate input and output files from "stdout" and "stderr" keyword arguments
             if kwarg == "stdout" or kwarg == "stderr":
                 if maybe_file:
-                    output_files.append(self._std_output_to_vine(kwarg, maybe_file))
+                    output_files.append(self._std_output_to_wq(kwarg, maybe_file))
             # For any other keyword that looks like a file, assume it is an input file
             elif isinstance(maybe_file, File):
                 input_files.append(self._register_file(maybe_file))
 
         # Create a Future object and have it be mapped from the task ID in the tasks dictionary
         fu = Future()
         fu.parsl_executor_task_id = executor_task_id
-        logger.debug("Getting tasks_lock to set vine-level task entry")
+        logger.debug("Getting tasks_lock to set WQ-level task entry")
         with self.tasks_lock:
-            logger.debug("Got tasks_lock to set vine-level task entry")
+            logger.debug("Got tasks_lock to set WQ-level task entry")
             self.tasks[str(executor_task_id)] = fu
 
-        logger.debug("Creating task {} for function {} with args {}".format(executor_task_id, func, args))
+        logger.debug("Creating executor task {} for function {} with args {}".format(executor_task_id, func, args))
 
-        # Pickle the result into object to pass into message buffer
         function_file = self._path_in_task(executor_task_id, "function")
         result_file = self._path_in_task(executor_task_id, "result")
         map_file = self._path_in_task(executor_task_id, "map")
 
-        logger.debug("Creating Task {} with function at: {}".format(executor_task_id, function_file))
-        logger.debug("Creating Executor Task {} with result to be found at: {}".format(executor_task_id, result_file))
+        logger.debug("Creating executor task {} with function at: {}".format(executor_task_id, function_file))
+        logger.debug("Creating executor task {} with result to be found at: {}".format(executor_task_id, result_file))
 
         self._serialize_function(function_file, func, args, kwargs)
 
         if self.pack:
             env_pkg = self._prepare_package(func, self.extra_pkgs)
         else:
             env_pkg = None
 
-        if self.pack_env:
-            env_pkg = self.pack_env
-
-        logger.debug("Constructing map for local filenames at worker for task {}".format(executor_task_id))
+        logger.debug("Constructing map for local filenames at worker for executor task {}".format(executor_task_id))
         self._construct_map_file(map_file, input_files, output_files)
 
         if not self.submit_process.is_alive():
-            raise ExecutorError(self, "taskvine Submit Process is not alive")
+            raise ExecutorError(self, "Workqueue Submit Process is not alive")
 
         # Create message to put into the message queue
-        logger.debug("Placing task {} on message queue".format(executor_task_id))
+        logger.debug("Placing executor task {} on message queue".format(executor_task_id))
         if category is None:
             category = func.__name__ if self.autocategory else 'parsl-default'
-        self.task_queue.put_nowait(ParslTaskToVine(executor_task_id,
-                                                   category,
-                                                   cores,
-                                                   memory,
-                                                   disk,
-                                                   gpus,
-                                                   priority,
-                                                   running_time_min,
-                                                   env_pkg,
-                                                   map_file,
-                                                   function_file,
-                                                   result_file,
-                                                   input_files,
-                                                   output_files))
+        self.task_queue.put_nowait(ParslTaskToWq(executor_task_id,
+                                                 category,
+                                                 cores,
+                                                 memory,
+                                                 disk,
+                                                 gpus,
+                                                 priority,
+                                                 running_time_min,
+                                                 env_pkg,
+                                                 map_file,
+                                                 function_file,
+                                                 result_file,
+                                                 input_files,
+                                                 output_files))
 
         return fu
 
     def _construct_worker_command(self):
         worker_command = self.worker_executable
+        if self.coprocess:
+            worker_command += " --coprocess parsl_coprocess.py"
         if self.project_password_file:
             worker_command += ' --password {}'.format(self.project_password_file)
         if self.worker_options:
             worker_command += ' {}'.format(self.worker_options)
         if self.project_name:
             worker_command += ' -M {}'.format(self.project_name)
         else:
-            worker_command += ' {} {}'.format(self.address, self.port)
+            worker_command += ' {} {}'.format(self.address, self._chosen_port)
 
         logger.debug("Using worker command: {}".format(worker_command))
         return worker_command
 
     def _patch_providers(self):
         # Add the worker and password file to files that the provider needs to stage.
         # (Currently only for the CondorProvider)
         if isinstance(self.provider, CondorProvider):
-            path_to_worker = shutil.which('vine_worker')
+            path_to_worker = shutil.which('work_queue_worker')
             self.worker_command = './' + self.worker_command
             self.provider.transfer_input_files.append(path_to_worker)
             if self.project_password_file:
                 self.provider.transfer_input_files.append(self.project_password_file)
 
     def _serialize_function(self, fn_path, parsl_fn, parsl_fn_args, parsl_fn_kwargs):
         """Takes the function application parsl_fn(*parsl_fn_args, **parsl_fn_kwargs)
@@ -566,50 +557,58 @@
 
         with open(fn_path, "wb") as f_out:
             pickle.dump(function_info, f_out)
 
     def _construct_map_file(self, map_file, input_files, output_files):
         """ Map local filepath of parsl files to the filenames at the execution worker.
         If using a shared filesystem, the filepath is mapped to its absolute filename.
-        Otherwise, to its original relative filename. In this later case, taskvine
+        Otherwise, to its original relative filename. In this later case, work queue
         recreates any directory hierarchy needed."""
         file_translation_map = {}
         for spec in itertools.chain(input_files, output_files):
             local_name = spec[0]
             if self.shared_fs:
                 remote_name = os.path.abspath(local_name)
             else:
                 remote_name = local_name
             file_translation_map[local_name] = remote_name
         with open(map_file, "wb") as f_out:
             pickle.dump(file_translation_map, f_out)
 
     def _register_file(self, parsl_file):
         """Generates a tuple (parsl_file.filepath, stage, cache) to give to
-        taskvine. cache is always True if self.use_cache is True.
-        Otherwise, it is set to False.
-        stage is True if the file needs to be copied by taskvine. (i.e., not
-        a URL or an absolute path)"""
-
-        to_cache = True
-        if not self.use_cache:
-            to_cache = False
+        work queue. cache is always False if self.use_cache is False.
+        Otherwise, it is set to True if parsl_file is used more than once.
+        stage is True if the file needs to be copied by work queue. (i.e., not
+        a URL or an absolute path)
+
+        It has the side-effect of adding parsl_file to a list of registered
+        files.
+
+        Note: The first time a file is used cache is set to False. Since
+        tasks are generated dynamically, without other information this is
+        the best we can do."""
+        to_cache = False
+        if self.use_cache:
+            to_cache = parsl_file in self.registered_files
 
         to_stage = False
         if parsl_file.scheme == 'file' or (parsl_file.local_path and os.path.exists(parsl_file.local_path)):
             to_stage = not os.path.isabs(parsl_file.filepath)
 
-        return ParslFileToVine(parsl_file.filepath, to_stage, to_cache)
+        self.registered_files.add(parsl_file)
+
+        return ParslFileToWq(parsl_file.filepath, to_stage, to_cache)
 
-    def _std_output_to_vine(self, fdname, stdfspec):
+    def _std_output_to_wq(self, fdname, stdfspec):
         """Find the name of the file that will contain stdout or stderr and
-        return a ParslFileToVine with it. These files are never cached"""
+        return a ParslFileToWq with it. These files are never cached"""
         fname, mode = putils.get_std_fname_mode(fdname, stdfspec)
         to_stage = not os.path.isabs(fname)
-        return ParslFileToVine(fname, stage=to_stage, cache=False)
+        return ParslFileToWq(fname, stage=to_stage, cache=False)
 
     def _prepare_package(self, fn, extra_pkgs):
         fn_id = id(fn)
         fn_name = fn.__name__
         if fn_id in self.cached_envs:
             logger.debug("Skipping analysis of %s, previously got %s", fn_name, self.cached_envs[fn_id])
             return self.cached_envs[fn_id]
@@ -642,15 +641,15 @@
 
     def initialize_scaling(self):
         """ Compose the launch command and call scale out
 
         Scales the workers to the appropriate nodes with provider
         """
         # Start scaling in/out
-        logger.debug("Starting TaskVineExecutor with provider: %s", self.provider)
+        logger.debug("Starting WorkQueueExecutor with provider: %s", self.provider)
         self.worker_command = self._construct_worker_command()
         self._patch_providers()
 
         if hasattr(self.provider, 'init_blocks'):
             try:
                 self.scale_out(blocks=self.provider.init_blocks)
             except Exception as e:
@@ -671,385 +670,356 @@
         return outstanding
 
     @property
     def workers_per_node(self) -> Union[int, float]:
         return 1
 
     def scale_in(self, count):
-        """Scale in method. Cancel a given number of blocks
+        """Scale in method.
         """
         # Obtain list of blocks to kill
         to_kill = list(self.blocks.keys())[:count]
         kill_ids = [self.blocks[block] for block in to_kill]
 
         # Cancel the blocks provisioned
         if self.provider:
             self.provider.cancel(kill_ids)
         else:
             logger.error("No execution provider available to scale")
 
     def shutdown(self, *args, **kwargs):
         """Shutdown the executor. Sets flag to cancel the submit process and
-        collector thread, which shuts down the TaskVine system submission.
+        collector thread, which shuts down the Work Queue system submission.
         """
-        logger.debug("TaskVine shutdown started")
+        logger.debug("Work Queue shutdown started")
         self.should_stop.value = True
 
         # Remove the workers that are still going
         kill_ids = [self.blocks[block] for block in self.blocks.keys()]
         if self.provider:
             logger.debug("Cancelling blocks")
             self.provider.cancel(kill_ids)
 
         logger.debug("Joining on submit process")
         self.submit_process.join()
         logger.debug("Joining on collector thread")
         self.collector_thread.join()
 
-        logger.debug("TaskVine shutdown completed")
+        logger.debug("Work Queue shutdown completed")
         return True
 
     @wrap_with_logs
-    def _collect_taskvine_results(self):
-        """Sets the values of tasks' futures of tasks completed by taskvine.
+    def _collect_work_queue_results(self):
+        """Sets the values of tasks' futures of tasks completed by work queue.
         """
         logger.debug("Starting Collector Thread")
         try:
             while not self.should_stop.value:
                 if not self.submit_process.is_alive():
-                    raise ExecutorError(self, "taskvine Submit Process is not alive")
+                    raise ExecutorError(self, "Workqueue Submit Process is not alive")
 
                 # Get the result message from the collector_queue
                 try:
                     task_report = self.collector_queue.get(timeout=1)
                 except queue.Empty:
                     continue
 
                 # Obtain the future from the tasks dictionary
                 with self.tasks_lock:
                     future = self.tasks.pop(task_report.id)
-
-                logger.debug("Updating Future for Parsl Task {}".format(task_report.id))
+                logger.debug("Updating Future for executor task {}".format(task_report.id))
                 if task_report.result_received:
                     future.set_result(task_report.result)
                 else:
                     # If there are no results, then the task failed according to one of
-                    # taskvine modes, such as resource exhaustion.
-                    future.set_exception(TaskVineTaskFailure(task_report.reason, task_report.result))
+                    # work queue modes, such as resource exhaustion.
+                    future.set_exception(WorkQueueTaskFailure(task_report.reason, task_report.result))
         finally:
             logger.debug("Marking all outstanding tasks as failed")
             logger.debug("Acquiring tasks_lock")
             with self.tasks_lock:
                 logger.debug("Acquired tasks_lock")
-                # set exception for tasks waiting for results that taskvine did not execute
+                # set exception for tasks waiting for results that work queue did not execute
                 for fu in self.tasks.values():
                     if not fu.done():
-                        fu.set_exception(TaskVineFailure("taskvine executor failed to execute the task."))
+                        fu.set_exception(WorkQueueFailure("work queue executor failed to execute the task."))
         logger.debug("Exiting Collector Thread")
 
 
 @wrap_with_logs
-def _taskvine_submit_wait(task_queue=multiprocessing.Queue(),
-                          launch_cmd=None,
-                          env=None,
-                          collector_queue=multiprocessing.Queue(),
-                          full=False,
-                          shared_fs=False,
-                          autolabel=False,
-                          autolabel_window=None,
-                          autocategory=True,
-                          max_retries=None,
-                          should_stop=None,
-                          port=VINE_DEFAULT_PORT,
-                          vine_log_dir=None,
-                          project_password_file=None,
-                          project_name=None,
-                          wait_for_workers=0,
-                          enable_peer_transfers=True):
-    """Thread to handle Parsl app submissions to the TaskVine objects.
+def _work_queue_submit_wait(*,
+                            port_mailbox: multiprocessing.Queue,
+                            task_queue: multiprocessing.Queue,
+                            launch_cmd: str,
+                            collector_queue: multiprocessing.Queue,
+                            data_dir: str,
+                            full: bool,
+                            shared_fs: bool,
+                            autolabel: bool,
+                            autolabel_window: int,
+                            autocategory: bool,
+                            max_retries: Optional[int],
+                            should_stop,  # multiprocessing.Value is an awkward type alias from inside multiprocessing
+                            port: int,
+                            wq_log_dir: str,
+                            project_password_file: Optional[str],
+                            project_name: Optional[str],
+                            coprocess: bool) -> int:
+    """Thread to handle Parsl app submissions to the Work Queue objects.
     Takes in Parsl functions submitted using submit(), and creates a
-    TaskVine task with the appropriate specifications, which is then
-    submitted to TaskVine. After tasks are completed, processes the
+    Work Queue task with the appropriate specifications, which is then
+    submitted to Work Queue. After tasks are completed, processes the
     exit status and exit code of the task, and sends results to the
-    TaskVine collector thread.
-    To avoid python's global interpreter lock with taskvine's wait, this
+    Work Queue collector thread.
+    To avoid python's global interpreter lock with work queue's wait, this
     function should be launched as a process, not as a lightweight thread. This
     means that any communication should be done using the multiprocessing
     module capabilities, rather than shared memory.
     """
-    logger.debug("Starting TaskVine Submit/Wait Process")
-    setproctitle("parsl: TaskVine submit/wait")
+    logger.debug("Starting WorkQueue Submit/Wait Process")
+    setproctitle("parsl: Work Queue submit/wait")
 
     # Enable debugging flags and create logging file
-    if vine_log_dir is not None:
-        logger.debug("Setting debugging flags and creating logging file at {}".format(vine_log_dir))
+    wq_debug_log = None
+    if wq_log_dir is not None:
+        logger.debug("Setting debugging flags and creating logging file")
+        wq_debug_log = os.path.join(wq_log_dir, "debug_log")
 
-    # Create TaskVine queue object
-    logger.debug("Creating TaskVine Object")
+    # Create WorkQueue queue object
+    logger.debug("Creating WorkQueue Object")
     try:
-        logger.debug("Listening on port {}".format(port))
-        m = Manager(port=port,
-                    name=project_name,
-                    run_info_path=vine_log_dir)
+        logger.debug("Requested port {}".format(port))
+        q = WorkQueue(port, debug_log=wq_debug_log)
+        port_mailbox.put(q.port)
+        logger.debug("Listening on port {}".format(q.port))
     except Exception as e:
-        logger.error("Unable to create TaskVine object: {}".format(e))
+        logger.error("Unable to create WorkQueue object: {}".format(e))
+        port_mailbox.put(None)
         raise e
 
-    # Specify TaskVine queue attributes
+    # Specify WorkQueue queue attributes
+    if project_name:
+        q.specify_name(project_name)
+
     if project_password_file:
-        m.set_password_file(project_password_file)
+        q.specify_password_file(project_password_file)
 
     if autolabel:
-        m.enable_monitoring()
+        q.enable_monitoring()
         if autolabel_window is not None:
-            m.tune('category-steady-n-tasks', autolabel_window)
-
-    if wait_for_workers:
-        m.tune("wait-for-workers", wait_for_workers)
-
-    if enable_peer_transfers:
-        m.enable_peer_transfers()
+            q.tune('category-steady-n-tasks', autolabel_window)
 
-    # Only write logs when the vine_log_dir is specified, which it most likely will be
-    # if vine_log_dir is not None:
-    if full and autolabel:
-        m.enable_monitoring_full(dirname=vine_log_dir)
+    # Only write logs when the wq_log_dir is specified, which it most likely will be
+    if wq_log_dir is not None:
+        wq_master_log = os.path.join(wq_log_dir, "master_log")
+        wq_trans_log = os.path.join(wq_log_dir, "transaction_log")
+        if full and autolabel:
+            wq_resource_log = os.path.join(wq_log_dir, "resource_logs")
+            q.enable_monitoring_full(dirname=wq_resource_log)
+        q.specify_log(wq_master_log)
+        q.specify_transactions_log(wq_trans_log)
 
     orig_ppid = os.getppid()
 
     result_file_of_task_id = {}  # Mapping executor task id -> result file for active tasks.
 
-    poncho_env_to_file = {}  # Mapping poncho_env file to File object in TaskVine
-
-    # Mapping of parsl local file name to TaskVine File object
-    # dict[str] -> vine File object
-    parsl_file_name_to_vine_file = {}
-
-    # Declare helper scripts as cache-able and peer-transferable
-    package_run_script_file = m.declare_file(package_run_script, cache=True, peer_transfer=True)
-    exec_parsl_function_file = m.declare_file(exec_parsl_function.__file__, cache=True, peer_transfer=True)
-
-    # Mapping of tasks from vine id to parsl id
-    # Dict[str] -> str
-    vine_id_to_executor_task_id = {}
-
     while not should_stop.value:
         # Monitor the task queue
         ppid = os.getppid()
         if ppid != orig_ppid:
             logger.debug("new Process")
             break
 
         # Submit tasks
         while task_queue.qsize() > 0 and not should_stop.value:
             # Obtain task from task_queue
             try:
                 task = task_queue.get(timeout=1)
-                logger.debug("Removing executor task from queue")
+                logger.debug("Removing task from queue")
             except queue.Empty:
                 continue
 
-            # Create command string
-            command_str = launch_cmd.format(mapping=os.path.basename(task.map_file),
-                                            function=os.path.basename(task.function_file),
-                                            result=os.path.basename(task.result_file))
-
-            # Create TaskVine task for the command
-            logger.debug("Sending executor task {} with command: {}".format(task.id, command_str))
             try:
-                t = Task(command_str)
-            except Exception as e:
-                logger.error("Unable to create executor task: {}".format(e))
-                collector_queue.put_nowait(VineTaskToParsl(id=task.id,
-                                                           result_received=False,
-                                                           result=None,
-                                                           reason="task could not be created by taskvine",
-                                                           status=-1))
-                continue
-
-            poncho_env_file = None
-            if task.env_pkg is not None:
-                if task.env_pkg not in poncho_env_to_file:
-                    poncho_env_file = m.declare_poncho(task.env_pkg, cache=True, peer_transfer=True)
-                    poncho_env_to_file[task.env_pkg] = poncho_env_file
+                pkg_pfx = ""
+                if task.env_pkg is not None:
+                    if package_run_script is None:
+                        raise ValueError("package_run_script must be specified")
+                    pkg_pfx = "./{} -e {} ".format(os.path.basename(package_run_script),
+                                                   os.path.basename(task.env_pkg))
+
+                if not coprocess:
+                    # Create command string
+                    logger.debug(launch_cmd)
+                    command_str = launch_cmd.format(package_prefix=pkg_pfx,
+                                                    mapping=os.path.basename(task.map_file),
+                                                    function=os.path.basename(task.function_file),
+                                                    result=os.path.basename(task.result_file))
+                    logger.debug(command_str)
+
+                    # Create WorkQueue task for the command
+                    logger.debug("Sending executor task {} with command: {}".format(task.id, command_str))
+                    t = wq.Task(command_str)
                 else:
-                    poncho_env_file = poncho_env_to_file[task.env_pkg]
+                    t = wq.RemoteTask("run_parsl_task",
+                                      "parsl_coprocess",
+                                      os.path.basename(task.map_file),
+                                      os.path.basename(task.function_file),
+                                      os.path.basename(task.result_file))
+                    t.specify_exec_method("direct")
+                    logger.debug("Sending executor task {} to coprocess".format(task.id))
 
-            if poncho_env_file is not None:
-                t.add_environment(poncho_env_file)
-                t.add_input(package_run_script_file, "poncho_package_run")
+            except Exception as e:
+                logger.error("Unable to create task: {}".format(e))
+                collector_queue.put_nowait(WqTaskToParsl(id=task.id,
+                                                         result_received=False,
+                                                         result=None,
+                                                         reason="task could not be created by work queue",
+                                                         status=-1))
+                continue
 
-            t.set_category(task.category)
+            t.specify_category(task.category)
             if autolabel:
-                m.set_category_mode(task.category, VINE_ALLOCATION_MODE_MAX_THROUGHPUT)
+                q.specify_category_mode(task.category, WORK_QUEUE_ALLOCATION_MODE_MAX_THROUGHPUT)
 
             if task.cores is not None:
-                t.set_cores(task.cores)
+                t.specify_cores(task.cores)
             if task.memory is not None:
-                t.set_memory(task.memory)
+                t.specify_memory(task.memory)
             if task.disk is not None:
-                t.set_disk(task.disk)
+                t.specify_disk(task.disk)
             if task.gpus is not None:
-                t.set_gpus(task.gpus)
+                t.specify_gpus(task.gpus)
             if task.priority is not None:
-                t.set_priority(task.priority)
+                t.specify_priority(task.priority)
             if task.running_time_min is not None:
-                t.set_time_min(task.running_time_min)
+                t.specify_running_time_min(task.running_time_min)
 
             if max_retries is not None:
                 logger.debug(f"Specifying max_retries {max_retries}")
-                t.set_retries(max_retries)
+                t.specify_max_retries(max_retries)
             else:
                 logger.debug("Not specifying max_retries")
 
-            # Specify environment variables for the task
-            if env is not None:
-                for var in env:
-                    t.set_env_var(str(var), str(env[var]))
-
-            # Add helper function that execute parsl functions on remote nodes
-            t.add_input(exec_parsl_function_file, "exec_parsl_function.py")
-
-            # Declare and add task-specific function, data, and result files to task
-            task_function_file = m.declare_file(task.function_file, cache=False, peer_transfer=False)
-            t.add_input(task_function_file, "function")
-
-            task_map_file = m.declare_file(task.map_file, cache=False, peer_transfer=False)
-            t.add_input(task_map_file, "map")
-
-            task_result_file = m.declare_file(task.result_file, cache=False, peer_transfer=False)
-            t.add_output(task_result_file, "result")
+            if task.env_pkg is not None:
+                t.specify_input_file(package_run_script, cache=True)
+                t.specify_input_file(task.env_pkg, cache=True)
 
+            # Specify script, and data/result files for task
+            t.specify_input_file(exec_parsl_function.__file__, cache=True)
+            t.specify_input_file(task.function_file, cache=False)
+            t.specify_input_file(task.map_file, cache=False)
+            t.specify_output_file(task.result_file, cache=False)
+            t.specify_tag(str(task.id))
             result_file_of_task_id[str(task.id)] = task.result_file
 
             logger.debug("Executor task id: {}".format(task.id))
 
             # Specify input/output files that need to be staged.
             # Absolute paths are assumed to be in shared filesystem, and thus
-            # not staged by taskvine.
-            # Files that share the same local path are assumed to be the same
-            # and thus use the same Vine File object if detected.
+            # not staged by work queue.
             if not shared_fs:
                 for spec in task.input_files:
                     if spec.stage:
-                        if spec.parsl_name in parsl_file_name_to_vine_file:
-                            task_in_file = parsl_file_name_to_vine_file[spec.parsl_name]
-                        else:
-                            task_in_file = m.declare_file(spec.parsl_name, cache=spec.cache, peer_transfer=True)
-                            parsl_file_name_to_vine_file[spec.parsl_name] = task_in_file
-                        t.add_input(task_in_file, spec.parsl_name)
-
+                        t.specify_input_file(spec.parsl_name, spec.parsl_name, cache=spec.cache)
                 for spec in task.output_files:
                     if spec.stage:
-                        if spec.parsl_name in parsl_file_name_to_vine_file:
-                            task_out_file = parsl_file_name_to_vine_file[spec.parsl_name]
-                        else:
-                            task_out_file = m.declare_file(spec.parsl_name, cache=spec.cache, peer_transfer=True)
-                        t.add_output(task_out_file, spec.parsl_name)
+                        t.specify_output_file(spec.parsl_name, spec.parsl_name, cache=spec.cache)
 
-            # Submit the task to the TaskVine object
-            logger.debug("Submitting executor task {} to TaskVine".format(task.id))
+            # Submit the task to the WorkQueue object
+            logger.debug("Submitting executor task {} to WorkQueue".format(task.id))
             try:
-                vine_id = m.submit(t)
-                vine_id_to_executor_task_id[str(vine_id)] = str(task.id)
+                wq_id = q.submit(t)
             except Exception as e:
-                logger.error("Unable to submit task to taskvine: {}".format(e))
-                collector_queue.put_nowait(VineTaskToParsl(id=task.id,
-                                                           result_received=False,
-                                                           result=None,
-                                                           reason="task could not be submited to taskvine",
-                                                           status=-1))
+                logger.error("Unable to submit task to work queue: {}".format(e))
+                collector_queue.put_nowait(WqTaskToParsl(id=task.id,
+                                                         result_received=False,
+                                                         result=None,
+                                                         reason="task could not be submited to work queue",
+                                                         status=-1))
                 continue
-            logger.info("Executor task {} submitted as TaskVine task with id {}".format(task.id, vine_id))
+            logger.info("Executor task {} submitted as Work Queue task {}".format(task.id, wq_id))
 
-        # If the queue is not empty wait on the TaskVine queue for a task
+        # If the queue is not empty wait on the WorkQueue queue for a task
         task_found = True
-        if not m.empty():
+        if not q.empty():
             while task_found and not should_stop.value:
                 # Obtain the task from the queue
-                t = m.wait(1)
+                t = q.wait(1)
                 if t is None:
                     task_found = False
                     continue
                 # When a task is found:
-                executor_task_id = vine_id_to_executor_task_id[str(t.id)]
-                logger.debug("Completed TaskVine task {}, executor task {}".format(t.id, executor_task_id))
-                result_file = result_file_of_task_id.pop(executor_task_id)
-                vine_id_to_executor_task_id.pop(str(t.id))
-
-                logger.debug(f"completed executor task info: {executor_task_id}, {t.category}, {t.command}, {t.std_output}")
+                executor_task_id = t.tag
+                logger.debug("Completed Work Queue task {}, executor task {}".format(t.id, t.tag))
+                result_file = result_file_of_task_id.pop(t.tag)
 
                 # A tasks completes 'succesfully' if it has result file,
                 # and it can be loaded. This may mean that the 'success' is
                 # an exception.
                 logger.debug("Looking for result in {}".format(result_file))
                 try:
                     with open(result_file, "rb") as f_in:
                         result = pickle.load(f_in)
                     logger.debug("Found result in {}".format(result_file))
-                    collector_queue.put_nowait(VineTaskToParsl(id=executor_task_id,
-                                                               result_received=True,
-                                                               result=result,
-                                                               reason=None,
-                                                               status=t.exit_code))
+                    collector_queue.put_nowait(WqTaskToParsl(id=executor_task_id,
+                                                             result_received=True,
+                                                             result=result,
+                                                             reason=None,
+                                                             status=t.return_status))
                 # If a result file could not be generated, explain the
-                # failure according to taskvine error codes. We generate
+                # failure according to work queue error codes. We generate
                 # an exception and wrap it with RemoteExceptionWrapper, to
                 # match the positive case.
                 except Exception as e:
-                    reason = _explain_taskvine_result(t)
+                    reason = _explain_work_queue_result(t)
                     logger.debug("Did not find result in {}".format(result_file))
-                    logger.debug("Wrapper Script status: {}\nTaskVine Status: {}"
-                                 .format(t.exit_code, t.result))
-                    logger.debug("Task with executor id {} / vine id {} failed because:\n{}"
+                    logger.debug("Wrapper Script status: {}\nWorkQueue Status: {}"
+                                 .format(t.return_status, t.result))
+                    logger.debug("Task with executor id {} / Work Queue id {} failed because:\n{}"
                                  .format(executor_task_id, t.id, reason))
-                    collector_queue.put_nowait(VineTaskToParsl(id=executor_task_id,
-                                                               result_received=False,
-                                                               result=e,
-                                                               reason=reason,
-                                                               status=t.exit_code))
-
-    logger.debug("Exiting TaskVine Monitoring Process")
+                    collector_queue.put_nowait(WqTaskToParsl(id=executor_task_id,
+                                                             result_received=False,
+                                                             result=e,
+                                                             reason=reason,
+                                                             status=t.return_status))
+    logger.debug("Exiting WorkQueue Monitoring Process")
     return 0
 
 
-def _explain_taskvine_result(vine_task):
-    """Returns a string with the reason why a task failed according to taskvine."""
+def _explain_work_queue_result(wq_task):
+    """Returns a string with the reason why a task failed according to work queue."""
 
-    vine_result = vine_task.result
+    wq_result = wq_task.result
 
-    reason = "taskvine result: "
-    if vine_result == cvine.VINE_RESULT_SUCCESS:
-        reason += "succesful execution with exit code {}".format(vine_task.return_status)
-    elif vine_result == cvine.VINE_RESULT_OUTPUT_MISSING:
+    reason = "work queue result: "
+    if wq_result == wq.WORK_QUEUE_RESULT_SUCCESS:
+        reason += "succesful execution with exit code {}".format(wq_task.return_status)
+    elif wq_result == wq.WORK_QUEUE_RESULT_OUTPUT_MISSING:
         reason += "The result file was not transfered from the worker.\n"
         reason += "This usually means that there is a problem with the python setup,\n"
         reason += "or the wrapper that executes the function."
-        reason += "\nTrace:\n" + str(vine_task.output)
-    elif vine_result == cvine.VINE_RESULT_INPUT_MISSING:
+        reason += "\nTrace:\n" + str(wq_task.output)
+    elif wq_result == wq.WORK_QUEUE_RESULT_INPUT_MISSING:
         reason += "missing input file"
-    elif vine_result == cvine.VINE_RESULT_STDOUT_MISSING:
+    elif wq_result == wq.WORK_QUEUE_RESULT_STDOUT_MISSING:
         reason += "stdout has been truncated"
-    elif vine_result == cvine.VINE_RESULT_SIGNAL:
+    elif wq_result == wq.WORK_QUEUE_RESULT_SIGNAL:
         reason += "task terminated with a signal"
-    elif vine_result == cvine.VINE_RESULT_RESOURCE_EXHAUSTION:
+    elif wq_result == wq.WORK_QUEUE_RESULT_RESOURCE_EXHAUSTION:
         reason += "task used more resources than requested"
-    elif vine_result == cvine.VINE_RESULT_MAX_END_TIME:
+    elif wq_result == wq.WORK_QUEUE_RESULT_TASK_TIMEOUT:
         reason += "task ran past the specified end time"
-    elif vine_result == cvine.VINE_RESULT_UNKNOWN:
+    elif wq_result == wq.WORK_QUEUE_RESULT_UNKNOWN:
         reason += "result could not be classified"
-    elif vine_result == cvine.VINE_RESULT_FORSAKEN:
+    elif wq_result == wq.WORK_QUEUE_RESULT_FORSAKEN:
         reason += "task failed, but not a task error"
-    elif vine_result == cvine.VINE_RESULT_MAX_RETRIES:
+    elif wq_result == wq.WORK_QUEUE_RESULT_MAX_RETRIES:
         reason += "unable to complete after specified number of retries"
-    elif vine_result == cvine.VINE_RESULT_MAX_WALL_TIME:
+    elif wq_result == wq.WORK_QUEUE_RESULT_TASK_MAX_RUN_TIME:
         reason += "task ran for more than the specified time"
-    elif vine_result == cvine.VINE_RESULT_RMONITOR_ERROR:
+    elif wq_result == wq.WORK_QUEUE_RESULT_DISK_ALLOC_FULL:
+        reason += "task needed more space to complete task"
+    elif wq_result == wq.WORK_QUEUE_RESULT_RMONITOR_ERROR:
         reason += "task failed because the monitor did not produce an output"
-    elif vine_result == cvine.VINE_RESULT_OUTPUT_TRANSFER_ERROR:
-        reason += "task failed because output transfer fails"
-    elif vine_result == cvine.VINE_RESULT_FIXED_LOCATION_MISSING:
-        reason += "task failed because no worker could satisfy the fixed \n"
-        reason += "location input file requirements"
     else:
-        reason += "unable to process TaskVine system failure"
+        reason += "unable to process Work Queue system failure"
     return reason
```

### Comparing `parsl-2023.6.19/parsl/executors/threads.py` & `parsl-2023.6.5/parsl/executors/threads.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/executors/workqueue/parsl_coprocess.py` & `parsl-2023.6.5/parsl/executors/workqueue/parsl_coprocess.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/executors/workqueue/parsl_coprocess_stub.py` & `parsl-2023.6.5/parsl/executors/workqueue/parsl_coprocess_stub.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/launchers/__init__.py` & `parsl-2023.6.5/parsl/launchers/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/launchers/launchers.py` & `parsl-2023.6.5/parsl/launchers/launchers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,29 @@
+from abc import ABCMeta, abstractmethod
 import logging
 
-from parsl.launchers.base import Launcher
+from parsl.utils import RepresentationMixin
 
 logger = logging.getLogger(__name__)
 
 
+class Launcher(RepresentationMixin, metaclass=ABCMeta):
+    """Launchers are basically wrappers for user submitted scripts as they
+    are submitted to a specific execution resource.
+    """
+    def __init__(self, debug: bool = True):
+        self.debug = debug
+
+    @abstractmethod
+    def __call__(self, command: str, tasks_per_node: int, nodes_per_block: int) -> str:
+        """ Wraps the command with the Launcher calls.
+        """
+        pass
+
+
 class SimpleLauncher(Launcher):
     """ Does no wrapping. Just returns the command as-is
     """
     def __init_(self, debug: bool = True) -> None:
         super().__init__(debug=debug)
 
     def __call__(self, command: str, tasks_per_node: int, nodes_per_block: int) -> str:
```

### Comparing `parsl-2023.6.19/parsl/log_utils.py` & `parsl-2023.6.5/parsl/log_utils.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/monitoring/db_manager.py` & `parsl-2023.6.5/parsl/monitoring/db_manager.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/monitoring/monitoring.py` & `parsl-2023.6.5/parsl/monitoring/monitoring.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,15 +135,15 @@
         # Any is used to disable typechecking on uses of _dfk_channel,
         # because it is used in the code as if it points to a channel, but
         # the static type is that it can also be None. The code relies on
         # .start() being called and initialising this to a real channel.
         self._dfk_channel = None  # type: Any
 
         if _db_manager_excepts:
-            raise _db_manager_excepts
+            raise(_db_manager_excepts)
 
         self.client_address = client_address
         self.client_port_range = client_port_range
 
         self.hub_address = hub_address
         self.hub_port = hub_port
         self.hub_port_range = hub_port_range
@@ -166,31 +166,20 @@
         os.makedirs(self.logdir, exist_ok=True)
 
         # Initialize the ZMQ pipe to the Parsl Client
 
         self.logger.debug("Initializing ZMQ Pipes to client")
         self.monitoring_hub_active = True
 
-        comm_q: Queue[Union[Tuple[int, int], str]]
-        comm_q = SizedQueue(maxsize=10)
-
-        self.exception_q: Queue[Tuple[str, str]]
-        self.exception_q = SizedQueue(maxsize=10)
-
-        self.priority_msgs: Queue[Tuple[Any, int]]
-        self.priority_msgs = SizedQueue()
-
-        self.resource_msgs: Queue[AddressedMonitoringMessage]
-        self.resource_msgs = SizedQueue()
-
-        self.node_msgs: Queue[AddressedMonitoringMessage]
-        self.node_msgs = SizedQueue()
-
-        self.block_msgs: Queue[AddressedMonitoringMessage]
-        self.block_msgs = SizedQueue()
+        comm_q = SizedQueue(maxsize=10)  # type: Queue[Union[Tuple[int, int], str]]
+        self.exception_q = SizedQueue(maxsize=10)  # type: Queue[Tuple[str, str]]
+        self.priority_msgs = SizedQueue()  # type: Queue[Tuple[Any, int]]
+        self.resource_msgs = SizedQueue()  # type: Queue[AddressedMonitoringMessage]
+        self.node_msgs = SizedQueue()  # type: Queue[AddressedMonitoringMessage]
+        self.block_msgs = SizedQueue()  # type:  Queue[AddressedMonitoringMessage]
 
         self.router_proc = ForkProcess(target=router_starter,
                                        args=(comm_q, self.exception_q, self.priority_msgs, self.node_msgs, self.block_msgs, self.resource_msgs),
                                        kwargs={"hub_address": self.hub_address,
                                                "hub_port": self.hub_port,
                                                "hub_port_range": self.hub_port_range,
                                                "logdir": self.logdir,
@@ -335,15 +324,15 @@
         for filename in os.listdir(new_dir):
             try:
                 logger.info(f"Processing filesystem radio file {filename}")
                 full_path_filename = f"{new_dir}/{filename}"
                 with open(full_path_filename, "rb") as f:
                     message = deserialize(f.read())
                 logger.info(f"Message received is: {message}")
-                assert isinstance(message, tuple)
+                assert(isinstance(message, tuple))
                 q.put(cast(AddressedMonitoringMessage, message))
                 os.remove(full_path_filename)
             except Exception:
                 logger.exception(f"Exception processing {filename} - probably will be retried next iteration")
 
         time.sleep(1)  # whats a good time for this poll?
```

### Comparing `parsl-2023.6.19/parsl/monitoring/queries/pandas.py` & `parsl-2023.6.5/parsl/monitoring/queries/pandas.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/monitoring/radios.py` & `parsl-2023.6.5/parsl/monitoring/radios.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/monitoring/remote.py` & `parsl-2023.6.5/parsl/monitoring/remote.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/monitoring/types.py` & `parsl-2023.6.5/parsl/monitoring/types.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/monitoring/visualization/app.py` & `parsl-2023.6.5/parsl/monitoring/visualization/app.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/monitoring/visualization/models.py` & `parsl-2023.6.5/parsl/monitoring/visualization/models.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/monitoring/visualization/plots/default/task_plots.py` & `parsl-2023.6.5/parsl/monitoring/visualization/plots/default/task_plots.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/monitoring/visualization/plots/default/workflow_plots.py` & `parsl-2023.6.5/parsl/monitoring/visualization/plots/default/workflow_plots.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py` & `parsl-2023.6.5/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/monitoring/visualization/static/parsl-logo-white.png` & `parsl-2023.6.5/parsl/monitoring/visualization/static/parsl-logo-white.png`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/monitoring/visualization/templates/app.html` & `parsl-2023.6.5/parsl/monitoring/visualization/templates/app.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/monitoring/visualization/templates/dag.html` & `parsl-2023.6.5/parsl/monitoring/visualization/templates/dag.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/monitoring/visualization/templates/layout.html` & `parsl-2023.6.5/parsl/monitoring/visualization/templates/layout.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/monitoring/visualization/templates/resource_usage.html` & `parsl-2023.6.5/parsl/monitoring/visualization/templates/resource_usage.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/monitoring/visualization/templates/task.html` & `parsl-2023.6.5/parsl/monitoring/visualization/templates/task.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/monitoring/visualization/templates/workflow.html` & `parsl-2023.6.5/parsl/monitoring/visualization/templates/workflow.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/monitoring/visualization/templates/workflows_summary.html` & `parsl-2023.6.5/parsl/monitoring/visualization/templates/workflows_summary.html`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/monitoring/visualization/views.py` & `parsl-2023.6.5/parsl/monitoring/visualization/views.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/multiprocessing.py` & `parsl-2023.6.5/parsl/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/process_loggers.py` & `parsl-2023.6.5/parsl/process_loggers.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/providers/__init__.py` & `parsl-2023.6.5/parsl/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/providers/ad_hoc/ad_hoc.py` & `parsl-2023.6.5/parsl/providers/ad_hoc/ad_hoc.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/providers/aws/aws.py` & `parsl-2023.6.5/parsl/providers/aws/aws.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/providers/azure/azure.py` & `parsl-2023.6.5/parsl/providers/azure/azure.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/providers/base.py` & `parsl-2023.6.5/parsl/providers/base.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/providers/cluster_provider.py` & `parsl-2023.6.5/parsl/providers/cluster_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,17 +63,17 @@
         self.min_blocks = min_blocks
         self.max_blocks = max_blocks
         self.parallelism = parallelism
         self.launcher = launcher
         self.walltime = walltime
         self.cmd_timeout = cmd_timeout
         if not callable(self.launcher):
-            raise BadLauncher(self.launcher,
+            raise(BadLauncher(self.launcher,
                               "Launcher for executor: {} is of type: {}. Expects a parsl.launcher.launcher.Launcher or callable".format(
-                                  label, type(self.launcher)))
+                                  label, type(self.launcher))))
 
         self.script_dir = None
 
         # Dictionary that keeps track of jobs, keyed on job_id
         self.resources = {}
 
     def execute_wait(self, cmd, timeout=None):
```

### Comparing `parsl-2023.6.19/parsl/providers/cobalt/cobalt.py` & `parsl-2023.6.5/parsl/providers/cobalt/cobalt.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/providers/condor/condor.py` & `parsl-2023.6.5/parsl/providers/condor/condor.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 import time
 import typeguard
 
 from parsl.channels import LocalChannel
 from parsl.providers.base import JobState, JobStatus
 from parsl.utils import RepresentationMixin
 from parsl.launchers import SingleNodeLauncher
-from parsl.launchers.base import Launcher
 from parsl.providers.condor.template import template_string
 from parsl.providers.cluster_provider import ClusterProvider
 from parsl.providers.errors import ScaleOutFailed
 
 logger = logging.getLogger(__name__)
 
 from typing import Dict, List, Optional
 from parsl.channels.base import Channel
+from parsl.launchers.launchers import Launcher
 
 # See http://pages.cs.wisc.edu/~adesmet/status.html
 translate_table = {
     '1': JobState.PENDING,
     '2': JobState.RUNNING,
     '3': JobState.CANCELLED,
     '4': JobState.COMPLETED,
```

### Comparing `parsl-2023.6.19/parsl/providers/condor/template.py` & `parsl-2023.6.5/parsl/providers/condor/template.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/providers/errors.py` & `parsl-2023.6.5/parsl/providers/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/providers/googlecloud/googlecloud.py` & `parsl-2023.6.5/parsl/providers/googlecloud/googlecloud.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/providers/grid_engine/grid_engine.py` & `parsl-2023.6.5/parsl/providers/grid_engine/grid_engine.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/providers/kubernetes/kube.py` & `parsl-2023.6.5/parsl/providers/kubernetes/kube.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,16 +124,15 @@
         self.group_id = group_id
         self.run_as_non_root = run_as_non_root
         self.persistent_volumes = persistent_volumes
 
         self.kube_client = client.CoreV1Api()
 
         # Dictionary that keeps track of jobs, keyed on job_id
-        self.resources: Dict[object, Dict[str, Any]]
-        self.resources = {}
+        self.resources = {}  # type: Dict[object, Dict[str, Any]]
 
     def submit(self, cmd_string, tasks_per_node, job_name="parsl"):
         """ Submit a job
         Args:
              - cmd_string  :(String) - Name of the container to initiate
              - tasks_per_node (int) : command invocations to be launched per node
```

### Comparing `parsl-2023.6.19/parsl/providers/local/local.py` & `parsl-2023.6.5/parsl/providers/local/local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/providers/lsf/lsf.py` & `parsl-2023.6.5/parsl/providers/lsf/lsf.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/providers/pbspro/pbspro.py` & `parsl-2023.6.5/parsl/providers/pbspro/pbspro.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/providers/slurm/slurm.py` & `parsl-2023.6.5/parsl/providers/slurm/slurm.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import typeguard
 
 from typing import Optional
 
 from parsl.channels import LocalChannel
 from parsl.channels.base import Channel
 from parsl.launchers import SingleNodeLauncher
-from parsl.launchers.base import Launcher
+from parsl.launchers.launchers import Launcher
 from parsl.providers.cluster_provider import ClusterProvider
 from parsl.providers.base import JobState, JobStatus
 from parsl.providers.slurm.template import template_string
 from parsl.utils import RepresentationMixin, wtime_to_minutes
 
 logger = logging.getLogger(__name__)
```

### Comparing `parsl-2023.6.19/parsl/providers/torque/torque.py` & `parsl-2023.6.5/parsl/providers/torque/torque.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/serialize/base.py` & `parsl-2023.6.5/parsl/serialize/base.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/serialize/concretes.py` & `parsl-2023.6.5/parsl/serialize/concretes.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/serialize/facade.py` & `parsl-2023.6.5/parsl/serialize/facade.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/configs/ad_hoc_cluster_htex.py` & `parsl-2023.6.5/parsl/tests/configs/ad_hoc_cluster_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/configs/azure_single_node.py` & `parsl-2023.6.5/parsl/tests/configs/azure_single_node.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/configs/bluewaters.py` & `parsl-2023.6.5/parsl/tests/configs/bluewaters.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/configs/bridges.py` & `parsl-2023.6.5/parsl/tests/configs/bridges.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/configs/cc_in2p3.py` & `parsl-2023.6.5/parsl/tests/configs/cc_in2p3.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/configs/comet.py` & `parsl-2023.6.5/parsl/tests/configs/comet.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/configs/cooley_htex.py` & `parsl-2023.6.5/parsl/tests/configs/cooley_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/configs/cori.py` & `parsl-2023.6.5/parsl/tests/configs/cori.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/configs/ec2_single_node.py` & `parsl-2023.6.5/parsl/tests/configs/ec2_single_node.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/configs/ec2_spot.py` & `parsl-2023.6.5/parsl/tests/configs/ec2_spot.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/configs/exex_local.py` & `parsl-2023.6.5/parsl/tests/configs/exex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/configs/frontera.py` & `parsl-2023.6.5/parsl/tests/configs/frontera.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/configs/htex_ad_hoc_cluster.py` & `parsl-2023.6.5/parsl/tests/configs/htex_ad_hoc_cluster.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/configs/htex_local.py` & `parsl-2023.6.5/parsl/tests/configs/htex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/configs/htex_local_alternate.py` & `parsl-2023.6.5/parsl/tests/configs/htex_local_alternate.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/configs/htex_local_intask_staging.py` & `parsl-2023.6.5/parsl/tests/configs/htex_local_intask_staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/configs/htex_local_rsync_staging.py` & `parsl-2023.6.5/parsl/tests/configs/htex_local_rsync_staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/configs/local_threads_globus.py` & `parsl-2023.6.5/parsl/tests/configs/local_threads_globus.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/configs/midway.py` & `parsl-2023.6.5/parsl/tests/configs/midway.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/configs/nscc_singapore.py` & `parsl-2023.6.5/parsl/tests/configs/nscc_singapore.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/configs/osg_htex.py` & `parsl-2023.6.5/parsl/tests/configs/osg_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/configs/petrelkube.py` & `parsl-2023.6.5/parsl/tests/configs/petrelkube.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/configs/summit.py` & `parsl-2023.6.5/parsl/tests/configs/summit.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/configs/swan_htex.py` & `parsl-2023.6.5/parsl/tests/configs/swan_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/configs/theta.py` & `parsl-2023.6.5/parsl/tests/configs/theta.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/configs/user_opts.py` & `parsl-2023.6.5/parsl/tests/configs/user_opts.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/conftest.py` & `parsl-2023.6.5/parsl/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,15 @@
         elif hasattr(module, 'fresh_config'):
             dfk = parsl.load(module.fresh_config())
         else:
             raise RuntimeError("Config module does not define config or fresh_config")
 
         yield
 
-        if parsl.dfk() != dfk:
+        if(parsl.dfk() != dfk):
             raise RuntimeError("DFK changed unexpectedly during test")
         dfk.cleanup()
         parsl.clear()
     else:
         yield
 
 
@@ -154,24 +154,24 @@
 
         if local_config:
             assert callable(local_config)
             c = local_config()
             assert isinstance(c, parsl.Config)
             dfk = parsl.load(c)
 
-        if callable(local_setup):
+        if(callable(local_setup)):
             local_setup()
 
         yield
 
-        if callable(local_teardown):
+        if(callable(local_teardown)):
             local_teardown()
 
-        if local_config:
-            if parsl.dfk() != dfk:
+        if(local_config):
+            if(parsl.dfk() != dfk):
                 raise RuntimeError("DFK changed unexpectedly during test")
             dfk.cleanup()
             parsl.clear()
 
     else:
         yield
 
@@ -267,11 +267,11 @@
 
 
 def pytest_ignore_collect(path):
     if 'integration' in path.strpath:
         return True
     elif 'manual_tests' in path.strpath:
         return True
-    elif 'scaling_tests/test_scale' in path.strpath:
+    elif 'workqueue_tests/test_scale' in path.strpath:
         return True
     else:
         return False
```

### Comparing `parsl-2023.6.19/parsl/tests/integration/latency.py` & `parsl-2023.6.5/parsl/tests/integration/latency.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/integration/test_channels/test_local_channel.py` & `parsl-2023.6.5/parsl/tests/integration/test_channels/test_local_channel.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/integration/test_channels/test_scp_1.py` & `parsl-2023.6.5/parsl/tests/integration/test_channels/test_scp_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/integration/test_channels/test_ssh_1.py` & `parsl-2023.6.5/parsl/tests/integration/test_channels/test_ssh_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/integration/test_channels/test_ssh_errors.py` & `parsl-2023.6.5/parsl/tests/integration/test_channels/test_ssh_errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/integration/test_channels/test_ssh_file_transport.py` & `parsl-2023.6.5/parsl/tests/integration/test_channels/test_ssh_file_transport.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/integration/test_channels/test_ssh_interactive.py` & `parsl-2023.6.5/parsl/tests/integration/test_channels/test_ssh_interactive.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/integration/test_stress/test_python_simple.py` & `parsl-2023.6.5/parsl/tests/integration/test_stress/test_python_simple.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/integration/test_stress/test_python_threads.py` & `parsl-2023.6.5/parsl/tests/integration/test_stress/test_python_threads.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/manual_tests/htex_local.py` & `parsl-2023.6.5/parsl/tests/manual_tests/htex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/manual_tests/test_ad_hoc_htex.py` & `parsl-2023.6.5/parsl/tests/manual_tests/test_ad_hoc_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/manual_tests/test_basic.py` & `parsl-2023.6.5/parsl/tests/manual_tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py` & `parsl-2023.6.5/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/manual_tests/test_log_filter.py` & `parsl-2023.6.5/parsl/tests/manual_tests/test_log_filter.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/manual_tests/test_memory_limits.py` & `parsl-2023.6.5/parsl/tests/manual_tests/test_memory_limits.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/manual_tests/test_regression_220.py` & `parsl-2023.6.5/parsl/tests/manual_tests/test_regression_220.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/manual_tests/test_udp_simple.py` & `parsl-2023.6.5/parsl/tests/manual_tests/test_udp_simple.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/manual_tests/test_worker_count.py` & `parsl-2023.6.5/parsl/tests/manual_tests/test_worker_count.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/scaling_tests/htex_local.py` & `parsl-2023.6.5/parsl/tests/workqueue_tests/htex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/scaling_tests/test_scale.py` & `parsl-2023.6.5/parsl/tests/workqueue_tests/test_scale.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/scaling_tests/wqex_condor.py` & `parsl-2023.6.5/parsl/tests/workqueue_tests/wqex_condor.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/scaling_tests/wqex_local.py` & `parsl-2023.6.5/parsl/tests/workqueue_tests/wqex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/site_tests/site_config_selector.py` & `parsl-2023.6.5/parsl/tests/site_tests/site_config_selector.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/site_tests/test_provider.py` & `parsl-2023.6.5/parsl/tests/site_tests/test_provider.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/site_tests/test_site.py` & `parsl-2023.6.5/parsl/tests/site_tests/test_site.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/sites/test_affinity.py` & `parsl-2023.6.5/parsl/tests/sites/test_affinity.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/sites/test_concurrent.py` & `parsl-2023.6.5/parsl/tests/sites/test_concurrent.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/sites/test_dynamic_executor.py` & `parsl-2023.6.5/parsl/tests/sites/test_dynamic_executor.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/sites/test_ec2.py` & `parsl-2023.6.5/parsl/tests/sites/test_ec2.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/sites/test_local_adhoc.py` & `parsl-2023.6.5/parsl/tests/sites/test_local_adhoc.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/sites/test_start_method.py` & `parsl-2023.6.5/parsl/tests/sites/test_start_method.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/sites/test_worker_info.py` & `parsl-2023.6.5/parsl/tests/sites/test_worker_info.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_aalst_patterns.py` & `parsl-2023.6.5/parsl/tests/test_aalst_patterns.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_bash_apps/test_apptimeout.py` & `parsl-2023.6.5/parsl/tests/test_bash_apps/test_apptimeout.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_bash_apps/test_basic.py` & `parsl-2023.6.5/parsl/tests/test_bash_apps/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_bash_apps/test_error_codes.py` & `parsl-2023.6.5/parsl/tests/test_bash_apps/test_error_codes.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_bash_apps/test_kwarg_storage.py` & `parsl-2023.6.5/parsl/tests/test_bash_apps/test_kwarg_storage.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_bash_apps/test_memoize.py` & `parsl-2023.6.5/parsl/tests/test_bash_apps/test_memoize.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_bash_apps/test_memoize_ignore_args.py` & `parsl-2023.6.5/parsl/tests/test_bash_apps/test_memoize_ignore_args.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py` & `parsl-2023.6.5/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_bash_apps/test_multiline.py` & `parsl-2023.6.5/parsl/tests/test_bash_apps/test_multiline.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_bash_apps/test_pipeline.py` & `parsl-2023.6.5/parsl/tests/test_bash_apps/test_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,25 +48,25 @@
     open("test0.txt", 'w').write('0\n')
 
     # Create the first entry in the dictionary holding the futures
     prev = File("test0.txt")
     futs = {}
     for i in range(1, depth):
         print("Launching {0} with {1}".format(i, prev))
-        assert isinstance(prev, DataFuture) or isinstance(prev, File)
+        assert(isinstance(prev, DataFuture) or isinstance(prev, File))
         output = File("test{0}.txt".format(i))
         fu = increment(inputs=[prev],  # Depend on the future from previous call
                        # Name the file to be created here
                        outputs=[output],
                        stdout="incr{0}.out".format(i),
                        stderr="incr{0}.err".format(i))
         [prev] = fu.outputs
         futs[i] = prev
         print(prev.filepath)
-        assert isinstance(prev, DataFuture)
+        assert(isinstance(prev, DataFuture))
 
     for key in futs:
         if key > 0:
             fu = futs[key]
             file = fu.result()
             filename = file.filepath
```

### Comparing `parsl-2023.6.19/parsl/tests/test_bash_apps/test_stdout.py` & `parsl-2023.6.5/parsl/tests/test_bash_apps/test_stdout.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_callables.py` & `parsl-2023.6.5/parsl/tests/test_callables.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_channels/test_large_output.py` & `parsl-2023.6.5/parsl/tests/test_channels/test_large_output.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_checkpointing/test_periodic.py` & `parsl-2023.6.5/parsl/tests/test_checkpointing/test_periodic.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_checkpointing/test_python_checkpoint_1.py` & `parsl-2023.6.5/parsl/tests/test_checkpointing/test_python_checkpoint_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_checkpointing/test_python_checkpoint_2.py` & `parsl-2023.6.5/parsl/tests/test_checkpointing/test_python_checkpoint_2.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_checkpointing/test_python_checkpoint_3.py` & `parsl-2023.6.5/parsl/tests/test_checkpointing/test_python_checkpoint_3.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_checkpointing/test_regression_232.py` & `parsl-2023.6.5/parsl/tests/test_checkpointing/test_regression_232.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_checkpointing/test_regression_233.py` & `parsl-2023.6.5/parsl/tests/test_checkpointing/test_regression_233.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_checkpointing/test_regression_239.py` & `parsl-2023.6.5/parsl/tests/test_checkpointing/test_regression_239.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_checkpointing/test_task_exit.py` & `parsl-2023.6.5/parsl/tests/test_checkpointing/test_task_exit.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_data/test_file.py` & `parsl-2023.6.5/parsl/tests/test_data/test_file.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_data/test_file_apps.py` & `parsl-2023.6.5/parsl/tests/test_data/test_file_apps.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_data/test_file_staging.py` & `parsl-2023.6.5/parsl/tests/test_data/test_file_staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_data/test_output_chain_filenames.py` & `parsl-2023.6.5/parsl/tests/test_data/test_output_chain_filenames.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_docs/test_from_slides.py` & `parsl-2023.6.5/parsl/tests/test_docs/test_from_slides.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_docs/test_tutorial_1.py` & `parsl-2023.6.5/parsl/tests/test_docs/test_tutorial_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_docs/test_workflow1.py` & `parsl-2023.6.5/parsl/tests/test_docs/test_workflow1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_docs/test_workflow2.py` & `parsl-2023.6.5/parsl/tests/test_docs/test_workflow2.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_docs/test_workflow3.py` & `parsl-2023.6.5/parsl/tests/test_docs/test_workflow3.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_docs/test_workflow4.py` & `parsl-2023.6.5/parsl/tests/test_docs/test_workflow4.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_error_handling/test_htex_missing_worker.py` & `parsl-2023.6.5/parsl/tests/test_error_handling/test_htex_missing_worker.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_error_handling/test_htex_worker_failure.py` & `parsl-2023.6.5/parsl/tests/test_error_handling/test_htex_worker_failure.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_error_handling/test_python_walltime.py` & `parsl-2023.6.5/parsl/tests/test_error_handling/test_python_walltime.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_error_handling/test_rand_fail.py` & `parsl-2023.6.5/parsl/tests/test_error_handling/test_rand_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_error_handling/test_resource_spec.py` & `parsl-2023.6.5/parsl/tests/test_error_handling/test_resource_spec.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_error_handling/test_retries.py` & `parsl-2023.6.5/parsl/tests/test_error_handling/test_retries.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_error_handling/test_retry_handler.py` & `parsl-2023.6.5/parsl/tests/test_error_handling/test_retry_handler.py`

 * *Files 14% similar despite different names*

```diff
@@ -57,8 +57,8 @@
     except OSError:
         pass
     fu = succeed_on_retry(fname, success_on=5)
 
     with pytest.raises(parsl.app.errors.BashExitFailure):
         fu.result()
 
-    assert fu.exception().exitcode == 5
+    assert(fu.exception().exitcode == 5)
```

### Comparing `parsl-2023.6.19/parsl/tests/test_error_handling/test_retry_handler_failure.py` & `parsl-2023.6.5/parsl/tests/test_error_handling/test_retry_handler_failure.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_error_handling/test_serialization_fail.py` & `parsl-2023.6.5/parsl/tests/test_error_handling/test_serialization_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_error_handling/test_wrap_with_logs.py` & `parsl-2023.6.5/parsl/tests/test_error_handling/test_wrap_with_logs.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_flux.py` & `parsl-2023.6.5/parsl/tests/test_flux.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_monitoring/test_basic.py` & `parsl-2023.6.5/parsl/tests/test_monitoring/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_monitoring/test_db_locks.py` & `parsl-2023.6.5/parsl/tests/test_monitoring/test_db_locks.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_monitoring/test_fuzz_zmq.py` & `parsl-2023.6.5/parsl/tests/test_monitoring/test_fuzz_zmq.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_monitoring/test_memoization_representation.py` & `parsl-2023.6.5/parsl/tests/test_monitoring/test_memoization_representation.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_monitoring/test_viz_colouring.py` & `parsl-2023.6.5/parsl/tests/test_monitoring/test_viz_colouring.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_providers/test_local_provider.py` & `parsl-2023.6.5/parsl/tests/test_providers/test_local_provider.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_python_apps/test_arg_input_types.py` & `parsl-2023.6.5/parsl/tests/test_python_apps/test_arg_input_types.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_python_apps/test_at_scale.py` & `parsl-2023.6.5/parsl/tests/test_python_apps/test_at_scale.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_python_apps/test_basic.py` & `parsl-2023.6.5/parsl/tests/test_python_apps/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_python_apps/test_dep_standard_futures.py` & `parsl-2023.6.5/parsl/tests/test_python_apps/test_dep_standard_futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_python_apps/test_depfail_propagation.py` & `parsl-2023.6.5/parsl/tests/test_python_apps/test_depfail_propagation.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_python_apps/test_fail.py` & `parsl-2023.6.5/parsl/tests/test_python_apps/test_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_python_apps/test_fibonacci_iterative.py` & `parsl-2023.6.5/parsl/tests/test_python_apps/test_fibonacci_iterative.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_python_apps/test_fibonacci_recursive.py` & `parsl-2023.6.5/parsl/tests/test_python_apps/test_fibonacci_recursive.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_python_apps/test_futures.py` & `parsl-2023.6.5/parsl/tests/test_python_apps/test_futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_python_apps/test_garbage_collect.py` & `parsl-2023.6.5/parsl/tests/test_python_apps/test_garbage_collect.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_python_apps/test_import_fail.py` & `parsl-2023.6.5/parsl/tests/test_python_apps/test_import_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_python_apps/test_join.py` & `parsl-2023.6.5/parsl/tests/test_python_apps/test_join.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_python_apps/test_mapred.py` & `parsl-2023.6.5/parsl/tests/test_python_apps/test_mapred.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_python_apps/test_memoize_1.py` & `parsl-2023.6.5/parsl/tests/test_python_apps/test_memoize_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_python_apps/test_memoize_2.py` & `parsl-2023.6.5/parsl/tests/test_python_apps/test_memoize_2.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_python_apps/test_memoize_4.py` & `parsl-2023.6.5/parsl/tests/test_python_apps/test_memoize_4.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py` & `parsl-2023.6.5/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_python_apps/test_memoize_ignore_args.py` & `parsl-2023.6.5/parsl/tests/test_python_apps/test_memoize_ignore_args.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_python_apps/test_outputs.py` & `parsl-2023.6.5/parsl/tests/test_python_apps/test_outputs.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_python_apps/test_overview.py` & `parsl-2023.6.5/parsl/tests/test_python_apps/test_overview.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_python_apps/test_pipeline.py` & `parsl-2023.6.5/parsl/tests/test_python_apps/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_python_apps/test_simple.py` & `parsl-2023.6.5/parsl/tests/test_python_apps/test_simple.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_python_apps/test_type5.py` & `parsl-2023.6.5/parsl/tests/test_python_apps/test_type5.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_python_apps/test_worker_fail.py` & `parsl-2023.6.5/parsl/tests/test_python_apps/test_worker_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_regression/test_1480.py` & `parsl-2023.6.5/parsl/tests/test_regression/test_1480.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_regression/test_1606_wait_for_current_tasks.py` & `parsl-2023.6.5/parsl/tests/test_regression/test_1606_wait_for_current_tasks.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_regression/test_1653.py` & `parsl-2023.6.5/parsl/tests/test_regression/test_1653.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_regression/test_221.py` & `parsl-2023.6.5/parsl/tests/test_regression/test_221.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_regression/test_226.py` & `parsl-2023.6.5/parsl/tests/test_regression/test_226.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_regression/test_2652.py` & `parsl-2023.6.5/parsl/tests/test_regression/test_2652.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_regression/test_69a.py` & `parsl-2023.6.5/parsl/tests/test_regression/test_69a.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_regression/test_69b.py` & `parsl-2023.6.5/parsl/tests/test_regression/test_69b.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_regression/test_854.py` & `parsl-2023.6.5/parsl/tests/test_regression/test_854.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_regression/test_97_parallelism_0.py` & `parsl-2023.6.5/parsl/tests/test_regression/test_97_parallelism_0.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_scaling/test_regression_1621.py` & `parsl-2023.6.5/parsl/tests/test_scaling/test_regression_1621.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_scaling/test_scale_down.py` & `parsl-2023.6.5/parsl/tests/test_scaling/test_scale_down.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_staging/staging_provider.py` & `parsl-2023.6.5/parsl/tests/test_staging/staging_provider.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_staging/test_1316.py` & `parsl-2023.6.5/parsl/tests/test_staging/test_1316.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_staging/test_docs_1.py` & `parsl-2023.6.5/parsl/tests/test_staging/test_docs_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_staging/test_elaborate_noop_file.py` & `parsl-2023.6.5/parsl/tests/test_staging/test_elaborate_noop_file.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_staging/test_staging_ftp.py` & `parsl-2023.6.5/parsl/tests/test_staging/test_staging_ftp.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_staging/test_staging_ftp_in_task.py` & `parsl-2023.6.5/parsl/tests/test_staging/test_staging_ftp_in_task.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_staging/test_staging_globus.py` & `parsl-2023.6.5/parsl/tests/test_staging/test_staging_globus.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_staging/test_staging_https.py` & `parsl-2023.6.5/parsl/tests/test_staging/test_staging_https.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_staging/test_staging_https_in_task.py` & `parsl-2023.6.5/parsl/tests/test_staging/test_staging_https_in_task.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_summary.py` & `parsl-2023.6.5/parsl/tests/test_summary.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_swift.py` & `parsl-2023.6.5/parsl/tests/test_swift.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_thread_parallelism.py` & `parsl-2023.6.5/parsl/tests/test_thread_parallelism.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_threads/test_configs.py` & `parsl-2023.6.5/parsl/tests/test_threads/test_configs.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/tests/test_threads/test_lazy_errors.py` & `parsl-2023.6.5/parsl/tests/test_threads/test_lazy_errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/usage_tracking/usage.py` & `parsl-2023.6.5/parsl/usage_tracking/usage.py`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/parsl/utils.py` & `parsl-2023.6.5/parsl/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
        - rundir(str) : Path to the runinfo directory
 
     Returns:
        - a list suitable for the checkpoint_files parameter of `Config`
 
     """
 
-    if not os.path.isdir(rundir):
+    if(not os.path.isdir(rundir)):
         return []
 
     dirs = sorted(os.listdir(rundir))
 
     checkpoints = []
 
     for runid in dirs:
@@ -95,15 +95,15 @@
 
     if len(dirs) == 0:
         return []
 
     last_runid = dirs[-1]
     last_checkpoint = os.path.abspath(f'{rundir}/{last_runid}/checkpoint')
 
-    if not os.path.isdir(last_checkpoint):
+    if(not(os.path.isdir(last_checkpoint))):
         return []
 
     return [last_checkpoint]
 
 
 @typeguard.typechecked
 def get_std_fname_mode(fdname: str, stdfspec: Union[str, Tuple[str, str]]) -> Tuple[str, str]:
```

### Comparing `parsl-2023.6.19/parsl.egg-info/PKG-INFO` & `parsl-2023.6.5/parsl.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: parsl
-Version: 2023.6.19
+Version: 2023.6.5
 Summary: Simple data dependent workflows in Python
 Home-page: https://github.com/Parsl/parsl
-Download-URL: https://github.com/Parsl/parsl/archive/2023.06.19.tar.gz
+Download-URL: https://github.com/Parsl/parsl/archive/2023.06.05.tar.gz
 Author: The Parsl Team
 Author-email: parsl@googlegroups.com
 License: Apache 2.0
 Keywords: Workflows,Scientific computing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `parsl-2023.6.19/parsl.egg-info/SOURCES.txt` & `parsl-2023.6.5/parsl.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,14 @@
 parsl/configs/midway.py
 parsl/configs/osg.py
 parsl/configs/polaris.py
 parsl/configs/stampede2.py
 parsl/configs/summit.py
 parsl/configs/theta.py
 parsl/configs/toss3_llnl.py
-parsl/configs/vineex_local.py
 parsl/configs/wqex_local.py
 parsl/data_provider/__init__.py
 parsl/data_provider/data_manager.py
 parsl/data_provider/file_noop.py
 parsl/data_provider/files.py
 parsl/data_provider/ftp.py
 parsl/data_provider/globus.py
@@ -104,26 +103,21 @@
 parsl/executors/high_throughput/executor.py
 parsl/executors/high_throughput/interchange.py
 parsl/executors/high_throughput/manager_record.py
 parsl/executors/high_throughput/monitoring_info.py
 parsl/executors/high_throughput/probe.py
 parsl/executors/high_throughput/process_worker_pool.py
 parsl/executors/high_throughput/zmq_pipes.py
-parsl/executors/taskvine/__init__.py
-parsl/executors/taskvine/errors.py
-parsl/executors/taskvine/exec_parsl_function.py
-parsl/executors/taskvine/executor.py
 parsl/executors/workqueue/__init__.py
 parsl/executors/workqueue/errors.py
 parsl/executors/workqueue/exec_parsl_function.py
 parsl/executors/workqueue/executor.py
 parsl/executors/workqueue/parsl_coprocess.py
 parsl/executors/workqueue/parsl_coprocess_stub.py
 parsl/launchers/__init__.py
-parsl/launchers/base.py
 parsl/launchers/errors.py
 parsl/launchers/launchers.py
 parsl/monitoring/__init__.py
 parsl/monitoring/db_manager.py
 parsl/monitoring/message_type.py
 parsl/monitoring/monitoring.py
 parsl/monitoring/radios.py
@@ -237,17 +231,17 @@
 parsl/tests/configs/local_threads_no_cache.py
 parsl/tests/configs/midway.py
 parsl/tests/configs/nscc_singapore.py
 parsl/tests/configs/osg_htex.py
 parsl/tests/configs/petrelkube.py
 parsl/tests/configs/summit.py
 parsl/tests/configs/swan_htex.py
-parsl/tests/configs/taskvine_ex.py
 parsl/tests/configs/theta.py
 parsl/tests/configs/user_opts.py
+parsl/tests/configs/workqueue_blocks.py
 parsl/tests/configs/workqueue_ex.py
 parsl/tests/integration/__init__.py
 parsl/tests/integration/latency.py
 parsl/tests/integration/test_parsl_load_default_config.py
 parsl/tests/integration/test_apps/__init__.py
 parsl/tests/integration/test_channels/__init__.py
 parsl/tests/integration/test_channels/test_channels.py
@@ -267,22 +261,14 @@
 parsl/tests/manual_tests/test_fan_in_out_htex_remote.py
 parsl/tests/manual_tests/test_log_filter.py
 parsl/tests/manual_tests/test_memory_limits.py
 parsl/tests/manual_tests/test_oauth_ssh.py
 parsl/tests/manual_tests/test_regression_220.py
 parsl/tests/manual_tests/test_udp_simple.py
 parsl/tests/manual_tests/test_worker_count.py
-parsl/tests/scaling_tests/__init__.py
-parsl/tests/scaling_tests/htex_local.py
-parsl/tests/scaling_tests/local_threads.py
-parsl/tests/scaling_tests/test_scale.py
-parsl/tests/scaling_tests/vineex_condor.py
-parsl/tests/scaling_tests/vineex_local.py
-parsl/tests/scaling_tests/wqex_condor.py
-parsl/tests/scaling_tests/wqex_local.py
 parsl/tests/site_tests/__init__.py
 parsl/tests/site_tests/site_config_selector.py
 parsl/tests/site_tests/test_provider.py
 parsl/tests/site_tests/test_site.py
 parsl/tests/sites/__init__.py
 parsl/tests/sites/test_affinity.py
 parsl/tests/sites/test_concurrent.py
@@ -402,9 +388,15 @@
 parsl/tests/test_staging/test_staging_ftp_in_task.py
 parsl/tests/test_staging/test_staging_globus.py
 parsl/tests/test_staging/test_staging_https.py
 parsl/tests/test_staging/test_staging_https_in_task.py
 parsl/tests/test_threads/__init__.py
 parsl/tests/test_threads/test_configs.py
 parsl/tests/test_threads/test_lazy_errors.py
+parsl/tests/workqueue_tests/__init__.py
+parsl/tests/workqueue_tests/htex_local.py
+parsl/tests/workqueue_tests/local_threads.py
+parsl/tests/workqueue_tests/test_scale.py
+parsl/tests/workqueue_tests/wqex_condor.py
+parsl/tests/workqueue_tests/wqex_local.py
 parsl/usage_tracking/__init__.py
 parsl/usage_tracking/usage.py
```

### Comparing `parsl-2023.6.19/parsl.egg-info/requires.txt` & `parsl-2023.6.5/parsl.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `parsl-2023.6.19/setup.py` & `parsl-2023.6.5/setup.py`

 * *Files identical despite different names*

