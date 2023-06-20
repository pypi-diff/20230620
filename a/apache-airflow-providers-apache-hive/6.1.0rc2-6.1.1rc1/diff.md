# Comparing `tmp/apache-airflow-providers-apache-hive-6.1.0rc2.tar.gz` & `tmp/apache-airflow-providers-apache-hive-6.1.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-apache-hive-6.1.0rc2.tar", last modified: Fri May 19 17:51:41 2023, max compression
+gzip compressed data, was "apache-airflow-providers-apache-hive-6.1.1rc1.tar", last modified: Tue Jun 20 11:41:17 2023, max compression
```

## Comparing `apache-airflow-providers-apache-hive-6.1.0rc2.tar` & `apache-airflow-providers-apache-hive-6.1.1rc1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:41.000000 apache-airflow-providers-apache-hive-6.1.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-hive-6.1.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:51:40.000000 apache-airflow-providers-apache-hive-6.1.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-hive-6.1.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)    18958 2023-05-19 17:51:41.000000 apache-airflow-providers-apache-hive-6.1.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    17243 2023-05-19 17:51:40.000000 apache-airflow-providers-apache-hive-6.1.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:41.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:41.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:41.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:41.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/
--rw-r--r--   0 root         (0) root         (0)     1536 2023-05-19 12:01:05.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5601 2023-05-19 17:51:40.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:41.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42315 2023-05-03 19:47:07.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/hooks/hive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:41.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/macros/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/macros/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4581 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/macros/hive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:41.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7383 2023-04-13 08:25:21.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/operators/hive.py
--rw-r--r--   0 root         (0) root         (0)     7454 2023-04-30 16:55:11.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/operators/hive_stats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:41.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/plugins/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1146 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/plugins/hive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:41.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3039 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/sensors/hive_partition.py
--rw-r--r--   0 root         (0) root         (0)     3389 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/sensors/metastore_partition.py
--rw-r--r--   0 root         (0) root         (0)     4159 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/sensors/named_hive_partition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:41.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5279 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/transfers/hive_to_mysql.py
--rw-r--r--   0 root         (0) root         (0)     2973 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/transfers/hive_to_samba.py
--rw-r--r--   0 root         (0) root         (0)     5671 2023-03-27 08:32:49.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/transfers/mssql_to_hive.py
--rw-r--r--   0 root         (0) root         (0)     6587 2023-03-27 08:32:49.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/transfers/mysql_to_hive.py
--rw-r--r--   0 root         (0) root         (0)    11742 2023-05-04 19:17:30.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/transfers/s3_to_hive.py
--rw-r--r--   0 root         (0) root         (0)     5548 2023-03-27 08:32:49.000000 apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/transfers/vertica_to_hive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:41.000000 apache-airflow-providers-apache-hive-6.1.0rc2/apache_airflow_providers_apache_hive.egg-info/
--rw-r--r--   0 root         (0) root         (0)    18958 2023-05-19 17:51:41.000000 apache-airflow-providers-apache-hive-6.1.0rc2/apache_airflow_providers_apache_hive.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1643 2023-05-19 17:51:41.000000 apache-airflow-providers-apache-hive-6.1.0rc2/apache_airflow_providers_apache_hive.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:51:41.000000 apache-airflow-providers-apache-hive-6.1.0rc2/apache_airflow_providers_apache_hive.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      188 2023-05-19 17:51:41.000000 apache-airflow-providers-apache-hive-6.1.0rc2/apache_airflow_providers_apache_hive.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:51:41.000000 apache-airflow-providers-apache-hive-6.1.0rc2/apache_airflow_providers_apache_hive.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      499 2023-05-19 17:51:41.000000 apache-airflow-providers-apache-hive-6.1.0rc2/apache_airflow_providers_apache_hive.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:51:41.000000 apache-airflow-providers-apache-hive-6.1.0rc2/apache_airflow_providers_apache_hive.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-apache-hive-6.1.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2092 2023-05-19 17:51:41.000000 apache-airflow-providers-apache-hive-6.1.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2114 2023-05-19 17:51:39.000000 apache-airflow-providers-apache-hive-6.1.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:17.585976 apache-airflow-providers-apache-hive-6.1.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-hive-6.1.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:16.000000 apache-airflow-providers-apache-hive-6.1.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-hive-6.1.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    19538 2023-06-20 11:41:17.587160 apache-airflow-providers-apache-hive-6.1.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    17873 2023-06-20 11:41:16.000000 apache-airflow-providers-apache-hive-6.1.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:17.460881 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:17.462033 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:17.463236 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:17.501401 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-06-20 11:01:09.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5668 2023-06-20 11:41:16.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:17.507300 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42441 2023-06-18 13:29:11.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/hooks/hive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:17.513956 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/macros/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/macros/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4581 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/macros/hive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:17.522586 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7384 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/operators/hive.py
+-rw-r--r--   0 root         (0) root         (0)     7502 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/operators/hive_stats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:17.528160 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/plugins/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/plugins/hive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:17.539416 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3039 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/sensors/hive_partition.py
+-rw-r--r--   0 root         (0) root         (0)     3389 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/sensors/metastore_partition.py
+-rw-r--r--   0 root         (0) root         (0)     4159 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/sensors/named_hive_partition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:17.559887 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5279 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/hive_to_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     2973 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/hive_to_samba.py
+-rw-r--r--   0 root         (0) root         (0)     5662 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/mssql_to_hive.py
+-rw-r--r--   0 root         (0) root         (0)     6713 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/mysql_to_hive.py
+-rw-r--r--   0 root         (0) root         (0)    11742 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/s3_to_hive.py
+-rw-r--r--   0 root         (0) root         (0)     5564 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/vertica_to_hive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:17.583345 apache-airflow-providers-apache-hive-6.1.1rc1/apache_airflow_providers_apache_hive.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    19538 2023-06-20 11:41:17.000000 apache-airflow-providers-apache-hive-6.1.1rc1/apache_airflow_providers_apache_hive.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1643 2023-06-20 11:41:17.000000 apache-airflow-providers-apache-hive-6.1.1rc1/apache_airflow_providers_apache_hive.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:17.000000 apache-airflow-providers-apache-hive-6.1.1rc1/apache_airflow_providers_apache_hive.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      188 2023-06-20 11:41:17.000000 apache-airflow-providers-apache-hive-6.1.1rc1/apache_airflow_providers_apache_hive.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:17.000000 apache-airflow-providers-apache-hive-6.1.1rc1/apache_airflow_providers_apache_hive.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      499 2023-06-20 11:41:17.000000 apache-airflow-providers-apache-hive-6.1.1rc1/apache_airflow_providers_apache_hive.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:17.000000 apache-airflow-providers-apache-hive-6.1.1rc1/apache_airflow_providers_apache_hive.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-hive-6.1.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2053 2023-06-20 11:41:17.590526 apache-airflow-providers-apache-hive-6.1.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2114 2023-06-20 11:41:16.000000 apache-airflow-providers-apache-hive-6.1.1rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc2/LICENSE` & `apache-airflow-providers-apache-hive-6.1.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc2/MANIFEST.in` & `apache-airflow-providers-apache-hive-6.1.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc2/PKG-INFO` & `apache-airflow-providers-apache-hive-6.1.1rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-hive
-Version: 6.1.0rc2
+Version: 6.1.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-hive package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.1/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: System :: Monitoring
-Requires-Python: ~=3.7
+Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: amazon
 Provides-Extra: common.sql
 Provides-Extra: microsoft.mssql
 Provides-Extra: mysql
 Provides-Extra: presto
 Provides-Extra: samba
@@ -55,38 +54,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-hive``
 
-Release: ``6.1.0rc2``
+Release: ``6.1.1rc1``
 
 
 `Apache Hive <https://hive.apache.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.hive`` provider. All classes for this provider package
 are in ``airflow.providers.apache.hive`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-apache-hive``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10
 
 Requirements
 ------------
 
 =======================================  ==================================
 PIP package                              Version required
 =======================================  ==================================
@@ -146,14 +145,40 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+
+6.1.1
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Bug Fixes
+~~~~~~~~~
+
+* ``Sanitize beeline principal parameter (#31983)``
+
+Misc
+~~~~
+
+* ``Replace unicodecsv with standard csv library (#31693)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+
+   * ``Apache provider docstring improvements (#31730)``
+   * ``Improve docstrings in providers (#31681)``
+   * ``Add D400 pydocstyle check - Apache providers only (#31424)``
+   * ``Add Python 3.11 support (#27264)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 6.1.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc2/README.rst` & `apache-airflow-providers-apache-hive-6.1.1rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,38 +15,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-hive``
 
-Release: ``6.1.0rc2``
+Release: ``6.1.1rc1``
 
 
 `Apache Hive <https://hive.apache.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.hive`` provider. All classes for this provider package
 are in ``airflow.providers.apache.hive`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-apache-hive``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10
 
 Requirements
 ------------
 
 =======================================  ==================================
 PIP package                              Version required
 =======================================  ==================================
@@ -106,14 +106,40 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+
+6.1.1
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Bug Fixes
+~~~~~~~~~
+
+* ``Sanitize beeline principal parameter (#31983)``
+
+Misc
+~~~~
+
+* ``Replace unicodecsv with standard csv library (#31693)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+
+   * ``Apache provider docstring improvements (#31730)``
+   * ``Improve docstrings in providers (#31681)``
+   * ``Add D400 pydocstyle check - Apache providers only (#31424)``
+   * ``Add Python 3.11 support (#27264)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 6.1.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/__init__.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "6.1.0"
+__version__ = "6.1.1"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/get_provider_info.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-apache-hive",
         "name": "Apache Hive",
         "description": "`Apache Hive <https://hive.apache.org/>`__\n",
         "suspended": False,
         "versions": [
+            "6.1.1",
             "6.1.0",
             "6.0.0",
             "5.1.3",
             "5.1.2",
             "5.1.1",
             "5.1.0",
             "5.0.0",
@@ -62,14 +63,15 @@
             "apache-airflow-providers-common-sql>=1.3.1",
             "hmsclient>=0.1.0",
             "pandas>=0.17.1",
             "pyhive[hive]>=0.6.0",
             'sasl>=0.3.1; python_version>="3.9"',
             "thrift>=0.9.2",
         ],
+        "excluded-python-versions": ["3.11"],
         "integrations": [
             {
                 "integration-name": "Apache Hive",
                 "external-doc-url": "https://hive.apache.org/",
                 "how-to-guide": ["/docs/apache-airflow-providers-apache-hive/operators.rst"],
                 "logo": "/integration-logos/apache/hive.png",
                 "tags": ["apache"],
```

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/hooks/__init__.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/hooks/hive.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/hooks/hive.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 try:
     import pandas
 except ImportError as e:
     from airflow.exceptions import AirflowOptionalProviderFeatureException
 
     raise AirflowOptionalProviderFeatureException(e)
 
-import unicodecsv as csv
+import csv
 
 from airflow.configuration import conf
 from airflow.exceptions import AirflowException
 from airflow.hooks.base import BaseHook
 from airflow.providers.common.sql.hooks.sql import DbApiHook
 from airflow.security import utils
 from airflow.utils.helpers import as_flattened_list
@@ -133,30 +133,30 @@
         if proxy_user_value == "owner" and self.run_as:
             return f"hive.server2.proxy.user={self.run_as}"
         if proxy_user_value != "":  # There is a custom proxy user
             return f"hive.server2.proxy.user={proxy_user_value}"
         return proxy_user_value  # The default proxy user (undefined)
 
     def _prepare_cli_cmd(self) -> list[Any]:
-        """This function creates the command list from available information"""
+        """This function creates the command list from available information."""
         conn = self.conn
         hive_bin = "hive"
         cmd_extra = []
 
         if self.use_beeline:
             hive_bin = "beeline"
             self._validate_beeline_parameters(conn)
             jdbc_url = f"jdbc:hive2://{conn.host}:{conn.port}/{conn.schema}"
             if conf.get("core", "security") == "kerberos":
                 template = conn.extra_dejson.get("principal", "hive/_HOST@EXAMPLE.COM")
                 if "_HOST" in template:
                     template = utils.replace_hostname_pattern(utils.get_components(template))
-
                 proxy_user = self._get_proxy_user()
-
+                if ";" in template:
+                    raise RuntimeError("The principal should not contain the ';' character")
                 jdbc_url += f";principal={template};{proxy_user}"
             elif self.auth:
                 jdbc_url += ";auth=" + self.auth
 
             jdbc_url = f'"{jdbc_url}"'
 
             cmd_extra += ["-u", jdbc_url]
@@ -292,15 +292,15 @@
 
                 if sub_process.returncode:
                     raise AirflowException(stdout)
 
                 return stdout
 
     def test_hql(self, hql: str) -> None:
-        """Test an hql statement using the hive cli and EXPLAIN"""
+        """Test an hql statement using the hive cli and EXPLAIN."""
         create, insert, other = [], [], []
         for query in hql.split(";"):  # naive
             query_original = query
             query = query.lower().strip()
 
             if query.startswith("create table"):
                 create.append(query_original)
@@ -411,15 +411,15 @@
         create: bool = True,
         overwrite: bool = True,
         partition: dict[str, Any] | None = None,
         recreate: bool = False,
         tblproperties: dict[str, Any] | None = None,
     ) -> None:
         """
-        Loads a local file into Hive
+        Loads a local file into Hive.
 
         Note that the table generated in Hive uses ``STORED AS textfile``
         which isn't the most efficient serialization format. If a
         large amount of data is loaded and/or if the tables gets
         queried considerably, you may want to use this operator only to
         stage the data into a temporary table before loading it into its
         final destination using a ``HiveOperator``.
@@ -471,26 +471,26 @@
         # at the end of hql (AIRFLOW-2412).
         hql += ";\n"
 
         self.log.info(hql)
         self.run_cli(hql)
 
     def kill(self) -> None:
-        """Kill Hive cli command"""
+        """Kill Hive cli command."""
         if hasattr(self, "sub_process"):
             if self.sub_process.poll() is None:
                 print("Killing the Hive job")
                 self.sub_process.terminate()
                 time.sleep(60)
                 self.sub_process.kill()
 
 
 class HiveMetastoreHook(BaseHook):
     """
-    Wrapper to interact with the Hive Metastore
+    Wrapper to interact with the Hive Metastore.
 
     :param metastore_conn_id: reference to the
         :ref: `metastore thrift service connection id <howto/connection:hive_metastore>`.
     """
 
     # java short max val
     MAX_PART_COUNT = 32767
@@ -583,15 +583,15 @@
         return None
 
     def get_conn(self) -> Any:
         return self.metastore
 
     def check_for_partition(self, schema: str, table: str, partition: str) -> bool:
         """
-        Checks whether a partition exists
+        Checks whether a partition exists.
 
         :param schema: Name of hive schema (database) @table belongs to
         :param table: Name of hive table @partition belongs to
         :param partition: Expression that matches the partitions to check for
             (eg `a = 'b' AND c = 'd'`)
 
         >>> hh = HiveMetastoreHook()
@@ -604,15 +604,15 @@
                 schema, table, partition, HiveMetastoreHook.MAX_PART_COUNT
             )
 
         return bool(partitions)
 
     def check_for_named_partition(self, schema: str, table: str, partition_name: str) -> Any:
         """
-        Checks whether a partition with a given name exists
+        Checks whether a partition with a given name exists.
 
         :param schema: Name of hive schema (database) @table belongs to
         :param table: Name of hive table @partition belongs to
         :param partition_name: Name of the partitions to check for (eg `a=b/c=d`)
 
         >>> hh = HiveMetastoreHook()
         >>> t = 'static_babynames_partitioned'
@@ -621,36 +621,36 @@
         >>> hh.check_for_named_partition('airflow', t, "ds=xxx")
         False
         """
         with self.metastore as client:
             return client.check_for_named_partition(schema, table, partition_name)
 
     def get_table(self, table_name: str, db: str = "default") -> Any:
-        """Get a metastore table object
+        """Get a metastore table object.
 
         >>> hh = HiveMetastoreHook()
         >>> t = hh.get_table(db='airflow', table_name='static_babynames')
         >>> t.tableName
         'static_babynames'
         >>> [col.name for col in t.sd.cols]
         ['state', 'year', 'name', 'gender', 'num']
         """
         if db == "default" and "." in table_name:
             db, table_name = table_name.split(".")[:2]
         with self.metastore as client:
             return client.get_table(dbname=db, tbl_name=table_name)
 
     def get_tables(self, db: str, pattern: str = "*") -> Any:
-        """Get a metastore table object"""
+        """Get a metastore table object."""
         with self.metastore as client:
             tables = client.get_tables(db_name=db, pattern=pattern)
             return client.get_table_objects_by_name(db, tables)
 
     def get_databases(self, pattern: str = "*") -> Any:
-        """Get a metastore table object"""
+        """Get a metastore table object."""
         with self.metastore as client:
             return client.get_databases(pattern)
 
     def get_partitions(self, schema: str, table_name: str, partition_filter: str | None = None) -> list[Any]:
         """
         Returns a list of all partitions in a table. Works only
         for tables with less than 32767 (java short max val).
@@ -770,15 +770,15 @@
             )
             part_specs = [client.partition_name_to_spec(part_name) for part_name in part_names]
 
         return HiveMetastoreHook._get_max_partition_from_part_specs(part_specs, field, filter_map)
 
     def table_exists(self, table_name: str, db: str = "default") -> bool:
         """
-        Check if table exists
+        Check if table exists.
 
         >>> hh = HiveMetastoreHook()
         >>> hh.table_exists(db='airflow', table_name='static_babynames')
         True
         >>> hh.table_exists(db='airflow', table_name='does_not_exist')
         False
         """
@@ -786,15 +786,15 @@
             self.get_table(table_name, db)
             return True
         except Exception:
             return False
 
     def drop_partitions(self, table_name, part_vals, delete_data=False, db="default"):
         """
-        Drop partitions from the given table matching the part_vals input
+        Drop partitions from the given table matching the part_vals input.
 
         :param table_name: table name.
         :param part_vals: list of partition specs.
         :param delete_data: Setting to control if underlying data have to deleted
                             in addition to dropping partitions.
         :param db: Name of hive schema (database) @table belongs to
 
@@ -812,15 +812,15 @@
         else:
             self.log.info("Table %s.%s does not exist!", db, table_name)
             return False
 
 
 class HiveServer2Hook(DbApiHook):
     """
-    Wrapper around the pyhive library
+    Wrapper around the pyhive library.
 
     Notes:
     * the default auth_mechanism is PLAIN, to override it you
     can specify it in the ``extra`` of your connection in the UI
     * the default for run_set_variable_statements is true, if you
     are using impala you may need to set it to false in the
     ``extra`` of your connection in the UI
@@ -985,16 +985,16 @@
 
         """
         results_iter = self._get_results(sql, schema, fetch_size=fetch_size, hive_conf=hive_conf)
         header = next(results_iter)
         message = None
 
         i = 0
-        with open(csv_filepath, "wb") as file:
-            writer = csv.writer(file, delimiter=delimiter, lineterminator=lineterminator, encoding="utf-8")
+        with open(csv_filepath, "w", encoding="utf-8") as file:
+            writer = csv.writer(file, delimiter=delimiter, lineterminator=lineterminator)
             try:
                 if output_header:
                     self.log.debug("Cursor description is %s", header)
                     writer.writerow([c[0] for c in header])
 
                 for i, row in enumerate(results_iter, 1):
                     writer.writerow(row)
@@ -1033,15 +1033,15 @@
         self,
         sql: str,
         schema: str = "default",
         hive_conf: dict[Any, Any] | None = None,
         **kwargs,
     ) -> pandas.DataFrame:
         """
-        Get a pandas dataframe from a Hive query
+        Get a pandas dataframe from a Hive query.
 
         :param sql: hql to be executed.
         :param schema: target schema, default to 'default'.
         :param hive_conf: hive_conf to execute alone with the hql.
         :param kwargs: (optional) passed into pandas.DataFrame constructor
         :return: result of hive execution
```

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/macros/__init__.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/macros/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/macros/hive.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/macros/hive.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/operators/__init__.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/operators/hive.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/operators/hive.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
         # assigned lazily - just for consistency we can create the attribute with a
         # `None` initial value, later it will be populated by the execute method.
         # This also makes `on_kill` implementation consistent since it assumes `self.hook`
         # is defined.
         self.hook: HiveCliHook | None = None
 
     def get_hook(self) -> HiveCliHook:
-        """Get Hive cli hook"""
+        """Get Hive cli hook."""
         return HiveCliHook(
             hive_cli_conn_id=self.hive_cli_conn_id,
             run_as=self.run_as,
             mapred_queue=self.mapred_queue,
             mapred_queue_priority=self.mapred_queue_priority,
             mapred_job_name=self.mapred_job_name,
             hive_cli_params=self.hive_cli_params,
```

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/operators/hive_stats.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/operators/hive_stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,18 +29,21 @@
 from airflow.providers.presto.hooks.presto import PrestoHook
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class HiveStatsCollectionOperator(BaseOperator):
-    """
-    Gathers partition statistics using a dynamically generated Presto
-    query, inserts the stats into a MySql table with this format. Stats
-    overwrite themselves if you rerun the same date/partition. ::
+    """Gather partition statistics and insert them into MySQL.
+
+    Statistics are gathered with a dynamically generated Presto query and
+    inserted with this format. Stats overwrite themselves if you rerun the
+    same date/partition.
+
+    .. code-block:: sql
 
         CREATE TABLE hive_stats (
             ds VARCHAR(16),
             table_name VARCHAR(500),
             metric VARCHAR(200),
             value BIGINT
         );
@@ -94,15 +97,15 @@
         self.presto_conn_id = presto_conn_id
         self.mysql_conn_id = mysql_conn_id
         self.assignment_func = assignment_func
         self.ds = "{{ ds }}"
         self.dttm = "{{ execution_date.isoformat() }}"
 
     def get_default_exprs(self, col: str, col_type: str) -> dict[Any, Any]:
-        """Get default expressions"""
+        """Get default expressions."""
         if col in self.excluded_columns:
             return {}
         exp = {(col, "non_null"): f"COUNT({col})"}
         if col_type in {"double", "int", "bigint", "float"}:
             exp[(col, "sum")] = f"SUM({col})"
             exp[(col, "min")] = f"MIN({col})"
             exp[(col, "max")] = f"MAX({col})"
```

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/plugins/__init__.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/plugins/hive.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/plugins/hive.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/sensors/__init__.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/sensors/hive_partition.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/sensors/hive_partition.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/sensors/metastore_partition.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/sensors/metastore_partition.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/sensors/named_hive_partition.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/sensors/named_hive_partition.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/transfers/__init__.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/transfers/hive_to_mysql.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/hive_to_mysql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/transfers/hive_to_samba.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/hive_to_samba.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/transfers/mssql_to_hive.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/mssql_to_hive.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """This module contains an operator to move data from MSSQL to Hive."""
 from __future__ import annotations
 
+import csv
 from collections import OrderedDict
 from tempfile import NamedTemporaryFile
 from typing import TYPE_CHECKING, Sequence
 
 import pymssql
-import unicodecsv as csv
 
 from airflow.models import BaseOperator
 from airflow.providers.apache.hive.hooks.hive import HiveCliHook
 from airflow.providers.microsoft.mssql.hooks.mssql import MsSqlHook
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
@@ -109,16 +109,16 @@
 
     def execute(self, context: Context):
         mssql = MsSqlHook(mssql_conn_id=self.mssql_conn_id)
         self.log.info("Dumping Microsoft SQL Server query results to local file")
         with mssql.get_conn() as conn:
             with conn.cursor() as cursor:
                 cursor.execute(self.sql)
-                with NamedTemporaryFile("w") as tmp_file:
-                    csv_writer = csv.writer(tmp_file, delimiter=self.delimiter, encoding="utf-8")
+                with NamedTemporaryFile(mode="w", encoding="utf-8") as tmp_file:
+                    csv_writer = csv.writer(tmp_file, delimiter=self.delimiter)
                     field_dict = OrderedDict()
                     for col_count, field in enumerate(cursor.description, start=1):
                         col_position = f"Column{col_count}"
                         field_dict[col_position if field[0] == "" else field[0]] = self.type_map(field[1])
                     csv_writer.writerows(cursor)
                     tmp_file.flush()
```

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/transfers/mysql_to_hive.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/mysql_to_hive.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,20 +14,21 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """This module contains an operator to move data from MySQL to Hive."""
 from __future__ import annotations
 
+import csv
 from collections import OrderedDict
+from contextlib import closing
 from tempfile import NamedTemporaryFile
 from typing import TYPE_CHECKING, Sequence
 
 import MySQLdb
-import unicodecsv as csv
 
 from airflow.models import BaseOperator
 from airflow.providers.apache.hive.hooks.hive import HiveCliHook
 from airflow.providers.mysql.hooks.mysql import MySqlHook
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
@@ -79,15 +80,15 @@
         *,
         sql: str,
         hive_table: str,
         create: bool = True,
         recreate: bool = False,
         partition: dict | None = None,
         delimiter: str = chr(1),
-        quoting: str | None = None,
+        quoting: int | None = None,
         quotechar: str = '"',
         escapechar: str | None = None,
         mysql_conn_id: str = "mysql_default",
         hive_cli_conn_id: str = "hive_cli_default",
         hive_auth: str | None = None,
         tblproperties: dict | None = None,
         **kwargs,
@@ -127,36 +128,32 @@
             types.TIMESTAMP: "TIMESTAMP",
         }
         return type_map.get(mysql_type, "STRING")
 
     def execute(self, context: Context):
         hive = HiveCliHook(hive_cli_conn_id=self.hive_cli_conn_id, auth=self.hive_auth)
         mysql = MySqlHook(mysql_conn_id=self.mysql_conn_id)
-
         self.log.info("Dumping MySQL query results to local file")
-        conn = mysql.get_conn()
-        cursor = conn.cursor()
-        cursor.execute(self.sql)
-        with NamedTemporaryFile("wb") as f:
-            csv_writer = csv.writer(
-                f,
-                delimiter=self.delimiter,
-                quoting=self.quoting,
-                quotechar=self.quotechar,
-                escapechar=self.escapechar,
-                encoding="utf-8",
-            )
-            field_dict = OrderedDict()
-            if cursor.description is not None:
-                for field in cursor.description:
-                    field_dict[field[0]] = self.type_map(field[1])
-            csv_writer.writerows(cursor)
+        with NamedTemporaryFile(mode="w", encoding="utf-8") as f:
+            with closing(mysql.get_conn()) as conn:
+                with closing(conn.cursor()) as cursor:
+                    cursor.execute(self.sql)
+                    csv_writer = csv.writer(
+                        f,
+                        delimiter=self.delimiter,
+                        quoting=self.quoting,
+                        quotechar=self.quotechar if self.quoting != csv.QUOTE_NONE else None,
+                        escapechar=self.escapechar,
+                    )
+                    field_dict = OrderedDict()
+                    if cursor.description is not None:
+                        for field in cursor.description:
+                            field_dict[field[0]] = self.type_map(field[1])
+                    csv_writer.writerows(cursor)
             f.flush()
-            cursor.close()
-            conn.close()  # type: ignore[misc]
             self.log.info("Loading file into Hive")
             hive.load_file(
                 f.name,
                 self.hive_table,
                 field_dict=field_dict,
                 create=self.create,
                 partition=self.partition,
```

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/transfers/s3_to_hive.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/s3_to_hive.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc2/airflow/providers/apache/hive/transfers/vertica_to_hive.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/vertica_to_hive.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,20 +14,19 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """This module contains an operator to move data from Vertica to Hive."""
 from __future__ import annotations
 
+import csv
 from collections import OrderedDict
 from tempfile import NamedTemporaryFile
 from typing import TYPE_CHECKING, Any, Sequence
 
-import unicodecsv as csv
-
 from airflow.models import BaseOperator
 from airflow.providers.apache.hive.hooks.hive import HiveCliHook
 from airflow.providers.vertica.hooks.vertica import VerticaHook
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
@@ -90,17 +89,19 @@
         self.vertica_conn_id = vertica_conn_id
         self.hive_cli_conn_id = hive_cli_conn_id
         self.partition = partition or {}
         self.hive_auth = hive_auth
 
     @classmethod
     def type_map(cls, vertica_type):
-        """
-        Vertica-python datatype.py does not provide the full type mapping access.
-        Manual hack. Reference:
+        """Manually hack Vertica-Python type mapping.
+
+        The stock datatype.py does not provide the full type mapping access.
+
+        Reference:
         https://github.com/uber/vertica-python/blob/master/vertica_python/vertica/column.py
         """
         type_map = {
             5: "BOOLEAN",
             6: "INT",
             7: "FLOAT",
             8: "STRING",
@@ -113,16 +114,16 @@
         hive = HiveCliHook(hive_cli_conn_id=self.hive_cli_conn_id, auth=self.hive_auth)
         vertica = VerticaHook(vertica_conn_id=self.vertica_conn_id)
 
         self.log.info("Dumping Vertica query results to local file")
         conn = vertica.get_conn()
         cursor = conn.cursor()
         cursor.execute(self.sql)
-        with NamedTemporaryFile("w") as f:
-            csv_writer = csv.writer(f, delimiter=self.delimiter, encoding="utf-8")
+        with NamedTemporaryFile(mode="w", encoding="utf-8") as f:
+            csv_writer = csv.writer(f, delimiter=self.delimiter)
             field_dict = OrderedDict()
             for col_count, field in enumerate(cursor.description, start=1):
                 col_position = f"Column{col_count}"
                 field_dict[col_position if field[0] == "" else field[0]] = self.type_map(field[1])
             csv_writer.writerows(cursor.iterate())
             f.flush()
             cursor.close()
```

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc2/apache_airflow_providers_apache_hive.egg-info/PKG-INFO` & `apache-airflow-providers-apache-hive-6.1.1rc1/apache_airflow_providers_apache_hive.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-hive
-Version: 6.1.0rc2
+Version: 6.1.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-hive package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.1/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: System :: Monitoring
-Requires-Python: ~=3.7
+Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: amazon
 Provides-Extra: common.sql
 Provides-Extra: microsoft.mssql
 Provides-Extra: mysql
 Provides-Extra: presto
 Provides-Extra: samba
@@ -55,38 +54,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-hive``
 
-Release: ``6.1.0rc2``
+Release: ``6.1.1rc1``
 
 
 `Apache Hive <https://hive.apache.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.hive`` provider. All classes for this provider package
 are in ``airflow.providers.apache.hive`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-apache-hive``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10
 
 Requirements
 ------------
 
 =======================================  ==================================
 PIP package                              Version required
 =======================================  ==================================
@@ -146,14 +145,40 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+
+6.1.1
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Bug Fixes
+~~~~~~~~~
+
+* ``Sanitize beeline principal parameter (#31983)``
+
+Misc
+~~~~
+
+* ``Replace unicodecsv with standard csv library (#31693)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+
+   * ``Apache provider docstring improvements (#31730)``
+   * ``Improve docstrings in providers (#31681)``
+   * ``Add D400 pydocstyle check - Apache providers only (#31424)``
+   * ``Add Python 3.11 support (#27264)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 6.1.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc2/apache_airflow_providers_apache_hive.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-hive-6.1.1rc1/apache_airflow_providers_apache_hive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc2/pyproject.toml` & `apache-airflow-providers-apache-hive-6.1.1rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,42 +22,43 @@
 # and we have to pin it to 63.4.3 version
 # The problem is tracked (and this limitation might be removed if it is solved) in:
 # https://github.com/pypa/setuptools/issues/3548
 [build-system]
 requires = ['setuptools==67.2.0']
 build-backend = "setuptools.build_meta"
 
+[project]
+requires-python = ">=3.8"
+
 [tool.ruff]
 typing-modules = ["airflow.typing_compat"]
 line-length = 110
 extend-exclude = [
     ".eggs",
     "airflow/_vendor/*",
     "airflow/providers/google/ads/_vendor/*",
     # The files generated by stubgen aren't 100% valid syntax it turns out, and we don't ship them, so we can
     # ignore them in ruff
-    "airflow/providers/common/sql/*/*.pyi"
+    "airflow/providers/common/sql/*/*.pyi",
+    "airflow/migrations/versions/*.py"
 ]
 
-# TODO: Bump to Python 3.8 when support for Python 3.7 is dropped in Airflow.
-target-version = "py37"
-
 extend-select = [
     "I", # Missing required import (auto-fixable)
     "UP", # Pyupgrade
     "RUF100", # Unused noqa (auto-fixable)
 
     # implicit single-line string concatenation
     "ISC001",
     # We ignore more pydocstyle than we enable, so be more selective at what we enable
     "D101",
     "D106",
     "D2",
     "D3",
-    # "D400", WIP: see #31135
+    "D400",
     # "D401", # Not enabled by ruff, but we don't want it
     "D402",
     "D403",
     "D412",
     "D419"
 ]
 extend-ignore = [
```

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc2/setup.cfg` & `apache-airflow-providers-apache-hive-6.1.1rc1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -17,34 +17,33 @@
 	Environment :: Console
 	Environment :: Web Environment
 	Intended Audience :: Developers
 	Intended Audience :: System Administrators
 	Framework :: Apache Airflow
 	Framework :: Apache Airflow :: Provider
 	License :: OSI Approved :: Apache Software License
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.1/
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
 python_tag = py3
 
 [options]
 zip_safe = False
 include_package_data = True
-python_requires = ~=3.7
+python_requires = ~=3.8
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
 	apache-airflow-providers-common-sql>=1.3.1.dev0
 	apache-airflow>=2.4.0.dev0
@@ -60,10 +59,10 @@
 airflow.plugins = 
 	hive=airflow.providers.apache.hive.plugins.hive:HivePlugin
 
 [files]
 packages = airflow.providers.apache.hive
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-apache-hive-6.1.0rc2/setup.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-apache-hive package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "6.1.0"
+version = "6.1.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-apache-hive setup."""
     setup(
         version=version,
         extras_require={
```

