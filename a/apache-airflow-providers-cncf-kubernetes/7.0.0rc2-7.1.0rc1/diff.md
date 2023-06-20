# Comparing `tmp/apache-airflow-providers-cncf-kubernetes-7.0.0rc2.tar.gz` & `tmp/apache-airflow-providers-cncf-kubernetes-7.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-cncf-kubernetes-7.0.0rc2.tar", last modified: Fri May 19 17:52:06 2023, max compression
+gzip compressed data, was "apache-airflow-providers-cncf-kubernetes-7.1.0rc1.tar", last modified: Tue Jun 20 11:41:43 2023, max compression
```

## Comparing `apache-airflow-providers-cncf-kubernetes-7.0.0rc2.tar` & `apache-airflow-providers-cncf-kubernetes-7.1.0rc1.tar`

### file list

```diff
@@ -1,50 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:06.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1156 2023-05-19 17:52:04.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)    34812 2023-05-19 17:52:06.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    33258 2023-05-19 17:52:04.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:05.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:05.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:05.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:05.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/
--rw-r--r--   0 root         (0) root         (0)     1540 2023-05-19 17:37:00.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:05.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/backcompat/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/backcompat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3904 2023-05-19 11:18:18.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:05.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/decorators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6178 2023-05-12 08:38:07.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/decorators/kubernetes.py
--rw-r--r--   0 root         (0) root         (0)     4383 2023-05-19 17:52:04.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:05.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23078 2023-05-19 11:18:18.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/hooks/kubernetes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:05.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1154 2023-05-03 19:47:07.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py
--rw-r--r--   0 root         (0) root         (0)    38841 2023-05-19 11:18:18.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/operators/pod.py
--rw-r--r--   0 root         (0) root         (0)     4860 2023-03-15 08:58:48.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py
--rw-r--r--   0 root         (0) root         (0)     1741 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2
--rw-r--r--   0 root         (0) root         (0)     3343 2023-03-27 08:32:49.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/python_kubernetes_script.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:05.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5226 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:06.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/triggers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1152 2023-05-03 19:47:07.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py
--rw-r--r--   0 root         (0) root         (0)    10367 2023-04-24 21:04:25.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/triggers/pod.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:06.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/utils/
--rw-r--r--   0 root         (0) root         (0)      863 2023-02-24 18:43:53.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22634 2023-05-19 11:18:18.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/utils/pod_manager.py
--rw-r--r--   0 root         (0) root         (0)     2642 2023-04-07 12:28:58.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:06.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/apache_airflow_providers_cncf_kubernetes.egg-info/
--rw-r--r--   0 root         (0) root         (0)    34812 2023-05-19 17:52:05.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/apache_airflow_providers_cncf_kubernetes.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1782 2023-05-19 17:52:05.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:05.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/apache_airflow_providers_cncf_kubernetes.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      112 2023-05-19 17:52:05.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/apache_airflow_providers_cncf_kubernetes.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:05.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/apache_airflow_providers_cncf_kubernetes.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      117 2023-05-19 17:52:05.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/apache_airflow_providers_cncf_kubernetes.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:52:05.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/apache_airflow_providers_cncf_kubernetes.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1976 2023-05-19 17:52:06.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1692 2023-05-19 17:52:04.000000 apache-airflow-providers-cncf-kubernetes-7.0.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:43.350021 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1156 2023-06-20 11:41:42.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    35763 2023-06-20 11:41:43.351420 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    34208 2023-06-20 11:41:42.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:43.184249 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:43.185461 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:43.186767 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:43.245870 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/
+-rw-r--r--   0 root         (0) root         (0)     1540 2023-06-20 11:01:09.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:43.251883 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/backcompat/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3914 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:43.257997 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/decorators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6178 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py
+-rw-r--r--   0 root         (0) root         (0)     4462 2023-06-20 11:41:42.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:43.263989 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23076 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:43.281363 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1154 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py
+-rw-r--r--   0 root         (0) root         (0)    39267 2023-06-05 12:50:36.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/operators/pod.py
+-rw-r--r--   0 root         (0) root         (0)     3827 2023-06-08 05:42:54.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/operators/resource.py
+-rw-r--r--   0 root         (0) root         (0)     4860 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2
+-rw-r--r--   0 root         (0) root         (0)     3345 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:43.287253 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5226 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:43.296090 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1152 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py
+-rw-r--r--   0 root         (0) root         (0)    10368 2023-06-18 13:29:11.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/triggers/pod.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:43.314088 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/utils/
+-rw-r--r--   0 root         (0) root         (0)      863 2023-06-01 06:14:28.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5209 2023-06-05 12:50:36.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/utils/delete_from.py
+-rw-r--r--   0 root         (0) root         (0)    23192 2023-06-05 12:50:36.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2644 2023-06-02 11:31:21.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:43.347126 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    35763 2023-06-20 11:41:43.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1893 2023-06-20 11:41:43.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:43.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      112 2023-06-20 11:41:43.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:43.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      117 2023-06-20 11:41:43.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:43.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1977 2023-06-20 11:41:43.353536 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1692 2023-06-20 11:41:42.000000 apache-airflow-providers-cncf-kubernetes-7.1.0rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/LICENSE` & `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/MANIFEST.in` & `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/PKG-INFO` & `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-cncf-kubernetes
-Version: 7.0.0rc2
+Version: 7.1.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-cncf-kubernetes package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.0.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.1.0/
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
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Monitoring
-Requires-Python: ~=3.7
+Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: NOTICE
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
    or more contributor license agreements.  See the NOTICE file
@@ -48,38 +48,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-cncf-kubernetes``
 
-Release: ``7.0.0rc2``
+Release: ``7.1.0rc1``
 
 
 `Kubernetes <https://kubernetes.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``cncf.kubernetes`` provider. All classes for this provider package
 are in ``airflow.providers.cncf.kubernetes`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.0.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.1.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-cncf-kubernetes``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ======================  ==================
 PIP package             Version required
 ======================  ==================
@@ -112,15 +112,45 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+7.1.0
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+
+Features
+~~~~~~~~
+* ``KubernetesResourceOperator - KubernetesDeleteResourceOperator & KubernetesCreateResourceOperator (#29930)``
+* ``add a return when the event is yielded in a loop to stop the execution (#31985)``
+* ``Add possibility to disable logging the pod template in a case when task fails (#31595)``
+
+
+Bug Fixes
+~~~~~~~~~
+
+* ``Remove return statement after yield from triggers class (#31703)``
+* ``Fix Fargate logging for AWS system tests (#31622)``
+
+Misc
+~~~~
+
+* ``Remove Python 3.7 support (#30963)``
 
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add D400 pydocstyle check (#31742)``
+   * ``Add discoverability for triggers in provider.yaml (#31576)``
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
 
 7.0.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/README.rst` & `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -15,38 +15,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-cncf-kubernetes``
 
-Release: ``7.0.0rc2``
+Release: ``7.1.0rc1``
 
 
 `Kubernetes <https://kubernetes.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``cncf.kubernetes`` provider. All classes for this provider package
 are in ``airflow.providers.cncf.kubernetes`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.0.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.1.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-cncf-kubernetes``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ======================  ==================
 PIP package             Version required
 ======================  ==================
@@ -79,15 +79,45 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+7.1.0
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+
+Features
+~~~~~~~~
+* ``KubernetesResourceOperator - KubernetesDeleteResourceOperator & KubernetesCreateResourceOperator (#29930)``
+* ``add a return when the event is yielded in a loop to stop the execution (#31985)``
+* ``Add possibility to disable logging the pod template in a case when task fails (#31595)``
+
+
+Bug Fixes
+~~~~~~~~~
+
+* ``Remove return statement after yield from triggers class (#31703)``
+* ``Fix Fargate logging for AWS system tests (#31622)``
+
+Misc
+~~~~
+
+* ``Remove Python 3.7 support (#30963)``
 
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add D400 pydocstyle check (#31742)``
+   * ``Add discoverability for triggers in provider.yaml (#31576)``
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
 
 7.0.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "7.0.0"
+__version__ = "7.1.0"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/backcompat/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py` & `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-"""Executes task in a Kubernetes POD"""
+"""Executes task in a Kubernetes POD."""
 from __future__ import annotations
 
 from kubernetes.client import ApiClient, models as k8s
 
 from airflow.exceptions import AirflowException
 
 
@@ -39,39 +39,39 @@
         api_client = ApiClient()
         return api_client._ApiClient__deserialize_model(obj, new_class)
     else:
         raise AirflowException(f"Expected dict or {new_class}, got {type(obj)}")
 
 
 def convert_volume(volume) -> k8s.V1Volume:
-    """Converts an airflow Volume object into a k8s.V1Volume
+    """Converts an airflow Volume object into a k8s.V1Volume.
 
     :param volume:
     """
     return _convert_kube_model_object(volume, k8s.V1Volume)
 
 
 def convert_volume_mount(volume_mount) -> k8s.V1VolumeMount:
-    """Converts an airflow VolumeMount object into a k8s.V1VolumeMount
+    """Converts an airflow VolumeMount object into a k8s.V1VolumeMount.
 
     :param volume_mount:
     """
     return _convert_kube_model_object(volume_mount, k8s.V1VolumeMount)
 
 
 def convert_port(port) -> k8s.V1ContainerPort:
-    """Converts an airflow Port object into a k8s.V1ContainerPort
+    """Converts an airflow Port object into a k8s.V1ContainerPort.
 
     :param port:
     """
     return _convert_kube_model_object(port, k8s.V1ContainerPort)
 
 
 def convert_env_vars(env_vars) -> list[k8s.V1EnvVar]:
-    """Converts a dictionary into a list of env_vars
+    """Converts a dictionary into a list of env_vars.
 
     :param env_vars:
     """
     if isinstance(env_vars, dict):
         res = []
         for k, v in env_vars.items():
             res.append(k8s.V1EnvVar(name=k, value=v))
@@ -79,42 +79,42 @@
     elif isinstance(env_vars, list):
         return env_vars
     else:
         raise AirflowException(f"Expected dict or list, got {type(env_vars)}")
 
 
 def convert_pod_runtime_info_env(pod_runtime_info_envs) -> k8s.V1EnvVar:
-    """Converts a PodRuntimeInfoEnv into an k8s.V1EnvVar
+    """Converts a PodRuntimeInfoEnv into an k8s.V1EnvVar.
 
     :param pod_runtime_info_envs:
     """
     return _convert_kube_model_object(pod_runtime_info_envs, k8s.V1EnvVar)
 
 
 def convert_image_pull_secrets(image_pull_secrets) -> list[k8s.V1LocalObjectReference]:
-    """Converts a PodRuntimeInfoEnv into an k8s.V1EnvVar
+    """Converts a PodRuntimeInfoEnv into an k8s.V1EnvVar.
 
     :param image_pull_secrets:
     """
     if isinstance(image_pull_secrets, str):
         secrets = image_pull_secrets.split(",")
         return [k8s.V1LocalObjectReference(name=secret) for secret in secrets]
     else:
         return image_pull_secrets
 
 
 def convert_configmap(configmaps) -> k8s.V1EnvFromSource:
-    """Converts a str into an k8s.V1EnvFromSource
+    """Converts a str into an k8s.V1EnvFromSource.
 
     :param configmaps:
     """
     return k8s.V1EnvFromSource(config_map_ref=k8s.V1ConfigMapEnvSource(name=configmaps))
 
 
 def convert_affinity(affinity) -> k8s.V1Affinity:
-    """Converts a dict into an k8s.V1Affinity"""
+    """Converts a dict into an k8s.V1Affinity."""
     return _convert_from_dict(affinity, k8s.V1Affinity)
 
 
 def convert_toleration(toleration) -> k8s.V1Toleration:
-    """Converts a dict into an k8s.V1Toleration"""
+    """Converts a dict into an k8s.V1Toleration."""
     return _convert_from_dict(toleration, k8s.V1Toleration)
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/decorators/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/decorators/kubernetes.py` & `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/get_provider_info.py` & `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/get_provider_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-cncf-kubernetes",
         "name": "Kubernetes",
         "description": "`Kubernetes <https://kubernetes.io/>`__\n",
         "suspended": False,
         "versions": [
+            "7.1.0",
             "7.0.0",
             "6.1.0",
             "6.0.0",
             "5.3.0",
             "5.2.2",
             "5.2.1",
             "5.2.0",
@@ -89,14 +90,15 @@
         "operators": [
             {
                 "integration-name": "Kubernetes",
                 "python-modules": [
                     "airflow.providers.cncf.kubernetes.operators.kubernetes_pod",
                     "airflow.providers.cncf.kubernetes.operators.pod",
                     "airflow.providers.cncf.kubernetes.operators.spark_kubernetes",
+                    "airflow.providers.cncf.kubernetes.operators.resource",
                 ],
             }
         ],
         "sensors": [
             {
                 "integration-name": "Kubernetes",
                 "python-modules": ["airflow.providers.cncf.kubernetes.sensors.spark_kubernetes"],
@@ -107,15 +109,15 @@
                 "integration-name": "Kubernetes",
                 "python-modules": ["airflow.providers.cncf.kubernetes.hooks.kubernetes"],
             }
         ],
         "triggers": [
             {
                 "integration-name": "Kubernetes",
-                "class-names": ["airflow.providers.cncf.kubernetes.triggers.pod.KubernetesPodTrigger"],
+                "python-modules": ["airflow.providers.cncf.kubernetes.triggers.pod"],
             }
         ],
         "connection-types": [
             {
                 "hook-class-name": "airflow.providers.cncf.kubernetes.hooks.kubernetes.KubernetesHook",
                 "connection-type": "kubernetes",
             }
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/hooks/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/hooks/kubernetes.py` & `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 import contextlib
 import tempfile
+from functools import cached_property
 from typing import TYPE_CHECKING, Any, Generator
 
 from asgiref.sync import sync_to_async
 from kubernetes import client, config, watch
 from kubernetes.client.models import V1Pod
 from kubernetes.config import ConfigException
 from kubernetes_asyncio import client as async_client, config as async_config
 from urllib3.exceptions import HTTPError
 
-from airflow.compat.functools import cached_property
 from airflow.exceptions import AirflowException, AirflowNotFoundException
 from airflow.hooks.base import BaseHook
 from airflow.kubernetes.kube_client import _disable_verify_ssl, _enable_tcp_keepalive
 from airflow.models import Connection
 from airflow.providers.cncf.kubernetes.utils.pod_manager import PodOperatorHookProtocol
 from airflow.utils import yaml
 
@@ -80,15 +80,15 @@
     conn_type = "kubernetes"
     hook_name = "Kubernetes Cluster Connection"
 
     DEFAULT_NAMESPACE = "default"
 
     @staticmethod
     def get_connection_form_widgets() -> dict[str, Any]:
-        """Returns connection widgets to add to connection form"""
+        """Returns connection widgets to add to connection form."""
         from flask_appbuilder.fieldwidgets import BS3TextFieldWidget
         from flask_babel import lazy_gettext
         from wtforms import BooleanField, StringField
 
         return {
             "in_cluster": BooleanField(lazy_gettext("In cluster configuration")),
             "kube_config_path": StringField(lazy_gettext("Kube config path"), widget=BS3TextFieldWidget()),
@@ -99,15 +99,15 @@
             "cluster_context": StringField(lazy_gettext("Cluster context"), widget=BS3TextFieldWidget()),
             "disable_verify_ssl": BooleanField(lazy_gettext("Disable SSL")),
             "disable_tcp_keepalive": BooleanField(lazy_gettext("Disable TCP keepalive")),
         }
 
     @staticmethod
     def get_ui_field_behaviour() -> dict[str, Any]:
-        """Returns custom field behaviour"""
+        """Returns custom field behaviour."""
         return {
             "hidden_fields": ["host", "schema", "login", "password", "port", "extra"],
             "relabeling": {},
         }
 
     def __init__(
         self,
@@ -173,15 +173,15 @@
             )
         if field_name in self.conn_extras:
             return self.conn_extras[field_name] or None
         prefixed_name = f"extra__kubernetes__{field_name}"
         return self.conn_extras.get(prefixed_name) or None
 
     def get_conn(self) -> client.ApiClient:
-        """Returns kubernetes api session for use with requests"""
+        """Returns kubernetes api session for use with requests."""
         in_cluster = self._coalesce_param(self.in_cluster, self._get_field("in_cluster"))
         cluster_context = self._coalesce_param(self.cluster_context, self._get_field("cluster_context"))
         kubeconfig_path = self._coalesce_param(self.config_file, self._get_field("kube_config_path"))
         kubeconfig = self._get_field("kube_config")
         num_selected_configuration = len([o for o in [in_cluster, kubeconfig, kubeconfig_path] if o])
 
         if num_selected_configuration > 1:
@@ -249,40 +249,41 @@
                 client_configuration=self.client_configuration,
                 context=cluster_context,
             )
         return client.ApiClient()
 
     @property
     def is_in_cluster(self) -> bool:
-        """Expose whether the hook is configured with ``load_incluster_config`` or not"""
+        """Expose whether the hook is configured with ``load_incluster_config`` or not."""
         if self._is_in_cluster is not None:
             return self._is_in_cluster
         self.api_client  # so we can determine if we are in_cluster or not
         if TYPE_CHECKING:
             assert self._is_in_cluster is not None
         return self._is_in_cluster
 
     @cached_property
     def api_client(self) -> client.ApiClient:
-        """Cached Kubernetes API client"""
+        """Cached Kubernetes API client."""
         return self.get_conn()
 
     @cached_property
     def core_v1_client(self) -> client.CoreV1Api:
         return client.CoreV1Api(api_client=self.api_client)
 
     @cached_property
     def custom_object_client(self) -> client.CustomObjectsApi:
         return client.CustomObjectsApi(api_client=self.api_client)
 
     def create_custom_object(
         self, group: str, version: str, plural: str, body: str | dict, namespace: str | None = None
     ):
         """
-        Creates custom resource definition object in Kubernetes
+        Creates custom resource definition object in Kubernetes.
+
         :param group: api group
         :param version: api version
         :param plural: api plural
         :param body: crd object definition
         :param namespace: kubernetes namespace
         """
         api: client.CustomObjectsApi = self.custom_object_client
@@ -303,15 +304,15 @@
         self.log.debug("Response: %s", response)
         return response
 
     def get_custom_object(
         self, group: str, version: str, plural: str, name: str, namespace: str | None = None
     ):
         """
-        Get custom resource definition object from Kubernetes
+        Get custom resource definition object from Kubernetes.
 
         :param group: api group
         :param version: api version
         :param plural: api plural
         :param name: crd object name
         :param namespace: kubernetes namespace
         """
@@ -325,15 +326,15 @@
         )
         return response
 
     def delete_custom_object(
         self, group: str, version: str, plural: str, name: str, namespace: str | None = None, **kwargs
     ):
         """
-        Delete custom resource definition object from Kubernetes
+        Delete custom resource definition object from Kubernetes.
 
         :param group: api group
         :param version: api version
         :param plural: api plural
         :param name: crd object name
         :param namespace: kubernetes namespace
         """
@@ -344,15 +345,15 @@
             namespace=namespace or self.get_namespace() or self.DEFAULT_NAMESPACE,
             plural=plural,
             name=name,
             **kwargs,
         )
 
     def get_namespace(self) -> str | None:
-        """Returns the namespace that defined in the connection"""
+        """Returns the namespace that defined in the connection."""
         if self.conn_id:
             return self._get_field("namespace")
         return None
 
     def get_pod_log_stream(
         self,
         pod_name: str,
@@ -408,15 +409,16 @@
         self,
         label_selector: str | None = "",
         namespace: str | None = None,
         watch: bool = False,
         **kwargs,
     ):
         """
-        Retrieves a list of Kind pod which belong default kubernetes namespace
+        Retrieves a list of Kind pod which belong default kubernetes namespace.
+
         :param label_selector: A selector to restrict the list of returned objects by their labels
         :param namespace: kubernetes namespace
         :param watch: Watch for changes to the described resources and return them as a stream
         """
         return self.core_v1_client.list_namespaced_pod(
             namespace=namespace or self.get_namespace() or self.DEFAULT_NAMESPACE,
             watch=watch,
@@ -445,15 +447,15 @@
     """Hook to use Kubernetes SDK asynchronously."""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._extras: dict | None = None
 
     async def _load_config(self):
-        """Returns Kubernetes API session for use with requests"""
+        """Returns Kubernetes API session for use with requests."""
         in_cluster = self._coalesce_param(self.in_cluster, await self._get_field("in_cluster"))
         cluster_context = self._coalesce_param(self.cluster_context, await self._get_field("cluster_context"))
         kubeconfig_path = self._coalesce_param(self.config_file, await self._get_field("kube_config_path"))
         kubeconfig = await self._get_field("kube_config")
 
         num_selected_configuration = len([o for o in [in_cluster, kubeconfig, kubeconfig_path] if o])
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/operators/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py` & `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/operators/pod.py` & `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/operators/pod.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,32 +10,32 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-"""Executes task in a Kubernetes POD"""
+"""Executes task in a Kubernetes POD."""
 
 from __future__ import annotations
 
 import json
 import logging
 import re
 import secrets
 import string
 from collections.abc import Container
 from contextlib import AbstractContextManager
+from functools import cached_property
 from typing import TYPE_CHECKING, Any, Sequence
 
 from kubernetes.client import CoreV1Api, models as k8s
 from slugify import slugify
 from urllib3.exceptions import HTTPError
 
-from airflow.compat.functools import cached_property
 from airflow.exceptions import AirflowException, AirflowSkipException
 from airflow.kubernetes import pod_generator
 from airflow.kubernetes.pod_generator import PodGenerator
 from airflow.kubernetes.secret import Secret
 from airflow.models import BaseOperator
 from airflow.providers.cncf.kubernetes.backcompat.backwards_compat_converters import (
     convert_affinity,
@@ -81,15 +81,15 @@
 
     :meta private:
     """
     return "".join(secrets.choice(alphanum_lower) for _ in range(num))
 
 
 def _add_pod_suffix(*, pod_name, rand_len=8, max_len=253):
-    """Add random string to pod name while staying under max len
+    """Add random string to pod name while staying under max len.
 
     TODO: when min airflow version >= 2.5, delete this function and import from kubernetes_helper_functions.
 
     :meta private:
     """
     suffix = "-" + _rand_str(rand_len)
     return pod_name[: max_len - len(suffix)].strip("-.") + suffix
@@ -131,15 +131,15 @@
 
 class PodReattachFailure(AirflowException):
     """When we expect to be able to find a pod but cannot."""
 
 
 class KubernetesPodOperator(BaseOperator):
     """
-    Execute a task in a Kubernetes Pod
+    Execute a task in a Kubernetes Pod.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:KubernetesPodOperator`
 
     .. note::
         If you use `Google Kubernetes Engine <https://cloud.google.com/kubernetes-engine/>`__
@@ -221,14 +221,15 @@
         exit code will be treated as a failure.
     :param base_container_name: The name of the base container in the pod. This container's logs
         will appear as part of this task's logs if get_logs is True. Defaults to None. If None,
         will consult the class variable BASE_CONTAINER_NAME (which defaults to "base") for the base
         container name to use.
     :param deferrable: Run operator in the deferrable mode.
     :param poll_interval: Polling period in seconds to check for the status. Used only in deferrable mode.
+    :param log_pod_spec_on_failure: Log the pod's specification if a failure occurs
     """
 
     # This field can be overloaded at the instance level via base_container_name
     BASE_CONTAINER_NAME = "base"
 
     POD_CHECKED_KEY = "already_checked"
     POST_TERMINATION_TIMEOUT = 120
@@ -297,14 +298,15 @@
         pod_runtime_info_envs: list[k8s.V1EnvVar] | None = None,
         termination_grace_period: int | None = None,
         configmaps: list[str] | None = None,
         skip_on_exit_code: int | Container[int] | None = None,
         base_container_name: str | None = None,
         deferrable: bool = False,
         poll_interval: float = 2,
+        log_pod_spec_on_failure: bool = True,
         **kwargs,
     ) -> None:
         # TODO: remove in provider 6.0.0 release. This is a mitigate step to advise users to switch to the
         # container_resources parameter.
         if isinstance(kwargs.get("resources"), k8s.V1ResourceRequirements):
             raise AirflowException(
                 "Specifying resources for the launched pod with 'resources' is deprecated. "
@@ -377,14 +379,15 @@
             if skip_on_exit_code
             else []
         )
         self.base_container_name = base_container_name or self.BASE_CONTAINER_NAME
         self.deferrable = deferrable
         self.poll_interval = poll_interval
         self.remote_pod: k8s.V1Pod | None = None
+        self.log_pod_spec_on_failure = log_pod_spec_on_failure
         self._config_dict: dict | None = None  # TODO: remove it when removing convert_config_file_to_dict
 
     @cached_property
     def _incluster_namespace(self):
         from pathlib import Path
 
         path = Path("/var/run/secrets/kubernetes.io/serviceaccount/namespace")
@@ -419,15 +422,15 @@
                 return
 
         super()._render_nested_template_fields(content, context, jinja_env, seen_oids)
 
     @staticmethod
     def _get_ti_pod_labels(context: Context | None = None, include_try_number: bool = True) -> dict[str, str]:
         """
-        Generate labels for the pod to track the pod in case of Operator crash
+        Generate labels for the pod to track the pod in case of Operator crash.
 
         :param context: task context provided by airflow DAG
         :return: dict
         """
         if not context:
             return {}
 
@@ -511,25 +514,25 @@
         except PodLaunchFailedException:
             if self.log_events_on_failure:
                 for event in self.pod_manager.read_pod_events(pod).items:
                     self.log.error("Pod Event: %s - %s", event.reason, event.message)
             raise
 
     def extract_xcom(self, pod: k8s.V1Pod):
-        """Retrieves xcom value and kills xcom sidecar container"""
+        """Retrieves xcom value and kills xcom sidecar container."""
         result = self.pod_manager.extract_xcom(pod)
         if isinstance(result, str) and result.rstrip() == "__airflow_xcom_result_empty__":
             self.log.info("xcom result file is empty.")
             return None
         else:
             self.log.info("xcom result: \n%s", result)
             return json.loads(result)
 
     def execute(self, context: Context):
-        """Based on the deferrable parameter runs the pod asynchronously or synchronously"""
+        """Based on the deferrable parameter runs the pod asynchronously or synchronously."""
         if self.deferrable:
             self.execute_async(context)
         else:
             return self.execute_sync(context)
 
     def execute_sync(self, context: Context):
         try:
@@ -672,15 +675,14 @@
         if pod_phase != PodPhase.SUCCEEDED:
             if self.log_events_on_failure:
                 self._read_pod_events(pod, reraise=False)
 
             self.process_pod_deletion(remote_pod, reraise=False)
 
             error_message = get_container_termination_message(remote_pod, self.base_container_name)
-            error_message = "\n" + error_message if error_message else ""
             if self.skip_on_exit_code is not None:
                 container_statuses = (
                     remote_pod.status.container_statuses if remote_pod and remote_pod.status else None
                 ) or []
                 base_container_status = next(
                     (x for x in container_statuses if x.name == self.base_container_name), None
                 )
@@ -693,22 +695,30 @@
                 )
                 if exit_code in self.skip_on_exit_code:
                     raise AirflowSkipException(
                         f"Pod {pod and pod.metadata.name} returned exit code "
                         f"{self.skip_on_exit_code}. Skipping."
                     )
             raise AirflowException(
-                f"Pod {pod and pod.metadata.name} returned a failure:\n{error_message}\n"
-                f"remote_pod: {remote_pod}"
+                "\n".join(
+                    filter(
+                        None,
+                        [
+                            f"Pod {pod and pod.metadata.name} returned a failure.",
+                            error_message if isinstance(error_message, str) else None,
+                            f"remote_pod: {remote_pod}" if self.log_pod_spec_on_failure else None,
+                        ],
+                    )
+                )
             )
         else:
             self.process_pod_deletion(remote_pod, reraise=False)
 
     def _read_pod_events(self, pod, *, reraise=True):
-        """Will fetch and emit events from pod"""
+        """Will fetch and emit events from pod."""
         with _optionally_suppress(reraise=reraise):
             for event in self.pod_manager.read_pod_events(pod).items:
                 self.log.error("Pod Event: %s - %s", event.reason, event.message)
 
     def process_pod_deletion(self, pod: k8s.V1Pod, *, reraise=True):
         with _optionally_suppress(reraise=reraise):
             if pod is not None:
@@ -731,15 +741,15 @@
     def _set_name(name: str | None) -> str | None:
         if name is not None:
             validate_key(name, max_length=220)
             return re.sub(r"[^a-z0-9-]+", "-", name.lower())
         return None
 
     def patch_already_checked(self, pod: k8s.V1Pod, *, reraise=True):
-        """Add an "already checked" annotation to ensure we don't reattach on retries"""
+        """Add an "already checked" annotation to ensure we don't reattach on retries."""
         with _optionally_suppress(reraise=reraise):
             self.client.patch_namespaced_pod(
                 name=pod.metadata.name,
                 namespace=pod.metadata.namespace,
                 body={"metadata": {"labels": {self.POD_CHECKED_KEY: "True"}}},
             )
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py` & `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class SparkKubernetesOperator(BaseOperator):
     """
-    Creates sparkApplication object in kubernetes cluster:
+    Creates sparkApplication object in kubernetes cluster.
 
     .. seealso::
         For more detail about Spark Application Object have a look at the reference:
         https://github.com/GoogleCloudPlatform/spark-on-k8s-operator/blob/v1beta2-1.1.0-2.4.5/docs/api-docs.md#sparkapplication
 
     :param application_file: Defines Kubernetes 'custom_resource_definition' of 'sparkApplication' as either a
         path to a '.yaml' file, '.json' file, YAML string or JSON string.
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2` & `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/python_kubernetes_script.py` & `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-"""Utilities for using the kubernetes decorator"""
+"""Utilities for using the kubernetes decorator."""
 from __future__ import annotations
 
 import os
 from collections import deque
 
 import jinja2
 
@@ -35,15 +35,15 @@
         elif current == ")":
             num_paren = num_paren - 1
     return "".join(after_decorator)
 
 
 def remove_task_decorator(python_source: str, task_decorator_name: str) -> str:
     """
-    Removes @task.kubernetes or similar as well as @setup and @teardown
+    Removes @task.kubernetes or similar as well as @setup and @teardown.
 
     :param python_source: python source code
     :param task_decorator_name: the task decorator name
     """
 
     def _remove_task_decorator(py_source, decorator_name):
         if decorator_name not in py_source:
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/sensors/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py` & `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class SparkKubernetesSensor(BaseSensorOperator):
     """
-    Checks sparkApplication object in kubernetes cluster:
+    Checks sparkApplication object in kubernetes cluster.
 
     .. seealso::
         For more detail about Spark Application Object have a look at the reference:
         https://github.com/GoogleCloudPlatform/spark-on-k8s-operator/blob/v1beta2-1.1.0-2.4.5/docs/api-docs.md#sparkapplication
 
     :param application_name: spark Application resource name
     :param namespace: the kubernetes namespace where the sparkApplication reside in
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/triggers/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py` & `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/triggers/pod.py` & `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/triggers/pod.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
                 "get_logs": self.get_logs,
                 "startup_timeout": self.startup_timeout,
                 "trigger_start_time": self.trigger_start_time,
             },
         )
 
     async def run(self) -> AsyncIterator[TriggerEvent]:  # type: ignore[override]
-        """Gets current pod status and yields a TriggerEvent"""
+        """Gets current pod status and yields a TriggerEvent."""
         hook = self._get_async_hook()
         self.log.info("Checking pod %r in namespace %r.", self.pod_name, self.pod_namespace)
         while True:
             try:
                 pod = await hook.get_pod(
                     name=self.pod_name,
                     namespace=self.pod_namespace,
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/utils/__init__.py` & `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/utils/pod_manager.py` & `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-"""Launches PODs"""
+"""Launches PODs."""
 from __future__ import annotations
 
 import json
+import logging
 import math
 import time
 import warnings
 from contextlib import closing, suppress
 from dataclasses import dataclass
 from datetime import datetime, timedelta
 from typing import TYPE_CHECKING, Generator, cast
@@ -31,14 +32,15 @@
 from kubernetes import client, watch
 from kubernetes.client.models.v1_container_status import V1ContainerStatus
 from kubernetes.client.models.v1_pod import V1Pod
 from kubernetes.client.rest import ApiException
 from kubernetes.stream import stream as kubernetes_stream
 from pendulum import DateTime
 from pendulum.parsing.exceptions import ParserError
+from tenacity import before_log
 from urllib3.exceptions import HTTPError as BaseHTTPError
 from urllib3.response import HTTPResponse
 
 from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.kubernetes.pod_generator import PodDefaults
 from airflow.typing_compat import Protocol
 from airflow.utils.log.logging_mixin import LoggingMixin
@@ -49,15 +51,15 @@
 
 
 class PodLaunchFailedException(AirflowException):
     """When pod launching fails in KubernetesPodOperator."""
 
 
 def should_retry_start_pod(exception: BaseException) -> bool:
-    """Check if an Exception indicates a transient error and warrants retrying"""
+    """Check if an Exception indicates a transient error and warrants retrying."""
     if isinstance(exception, ApiException):
         return exception.status == 409
     return False
 
 
 class PodPhase:
     """
@@ -71,38 +73,38 @@
     SUCCEEDED = "Succeeded"
 
     terminal_states = {FAILED, SUCCEEDED}
 
 
 class PodOperatorHookProtocol(Protocol):
     """
-    Protocol to define methods relied upon by KubernetesPodOperator
+    Protocol to define methods relied upon by KubernetesPodOperator.
 
     Subclasses of KubernetesPodOperator, such as GKEStartPodOperator, may use
     hooks that don't extend KubernetesHook.  We use this protocol to document the
     methods used by KPO and ensure that these methods exist on such other hooks.
     """
 
     @property
     def core_v1_client(self) -> client.CoreV1Api:
         """Get authenticated CoreV1Api object."""
 
     @property
     def is_in_cluster(self) -> bool:
-        """Expose whether the hook is configured with ``load_incluster_config`` or not"""
+        """Expose whether the hook is configured with ``load_incluster_config`` or not."""
 
     def get_pod(self, name: str, namespace: str) -> V1Pod:
         """Read pod object from kubernetes API."""
 
     def get_namespace(self) -> str | None:
-        """Returns the namespace that defined in the connection"""
+        """Returns the namespace that defined in the connection."""
 
 
 def get_container_status(pod: V1Pod, container_name: str) -> V1ContainerStatus | None:
-    """Retrieves container status"""
+    """Retrieves container status."""
     container_statuses = pod.status.container_statuses if pod and pod.status else None
     if container_statuses:
         # In general the variable container_statuses can store multiple items matching different containers.
         # The following generator expression yields all items that have name equal to the container_name.
         # The function next() here calls the generator to get only the first value. If there's nothing found
         # then None is returned.
         return next((x for x in container_statuses if x.name == container_name), None)
@@ -141,15 +143,16 @@
         return container_status.state.terminated.message if container_status else None
 
 
 class PodLogsConsumer:
     """
     PodLogsConsumer is responsible for pulling pod logs from a stream with checking a container status before
     reading data.
-    This class is a workaround for the issue https://github.com/apache/airflow/issues/23497
+
+    This class is a workaround for the issue https://github.com/apache/airflow/issues/23497.
 
     :param response: HTTP response with logs
     :param pod: Pod instance from Kubernetes client
     :param pod_manager: Pod manager instance
     :param container_name: Name of the container that we're reading logs from
     :param post_termination_timeout: (Optional) The period of time in seconds representing for how long time
         logs are available after the container termination.
@@ -225,24 +228,24 @@
             self.read_pod_cache = self.pod_manager.read_pod(self.pod)
             self.last_read_pod_at = _now
         return self.read_pod_cache
 
 
 @dataclass
 class PodLoggingStatus:
-    """Used for returning the status of the pod and last log time when exiting from `fetch_container_logs`"""
+    """Used for returning the status of the pod and last log time when exiting from `fetch_container_logs`."""
 
     running: bool
     last_log_time: DateTime | None
 
 
 class PodManager(LoggingMixin):
     """
     Helper class for creating, monitoring, and otherwise interacting with Kubernetes pods
-    for use with the KubernetesPodOperator
+    for use with the KubernetesPodOperator.
     """
 
     def __init__(
         self,
         kube_client: client.CoreV1Api,
     ):
         """
@@ -251,15 +254,15 @@
         :param kube_client: kubernetes client
         """
         super().__init__()
         self._client = kube_client
         self._watch = watch.Watch()
 
     def run_pod_async(self, pod: V1Pod, **kwargs) -> V1Pod:
-        """Runs POD asynchronously"""
+        """Runs POD asynchronously."""
         sanitized_pod = self._client.api_client.sanitize_for_serialization(pod)
         json_pod = json.dumps(sanitized_pod, indent=2)
 
         self.log.debug("Pod Creation Request: \n%s", json_pod)
         try:
             resp = self._client.create_namespaced_pod(
                 body=sanitized_pod, namespace=pod.metadata.namespace, **kwargs
@@ -269,15 +272,15 @@
             self.log.exception(
                 "Exception when attempting to create Namespaced Pod: %s", str(json_pod).replace("\n", " ")
             )
             raise e
         return resp
 
     def delete_pod(self, pod: V1Pod) -> None:
-        """Deletes POD"""
+        """Deletes POD."""
         try:
             self._client.delete_namespaced_pod(
                 pod.metadata.name, pod.metadata.namespace, body=client.V1DeleteOptions()
             )
         except ApiException as e:
             # If the pod is already deleted
             if e.status != 404:
@@ -291,15 +294,15 @@
     )
     def create_pod(self, pod: V1Pod) -> V1Pod:
         """Launches the pod asynchronously."""
         return self.run_pod_async(pod)
 
     def await_pod_start(self, pod: V1Pod, startup_timeout: int = 120) -> None:
         """
-        Waits for the pod to reach phase other than ``Pending``
+        Waits for the pod to reach phase other than ``Pending``.
 
         :param pod:
         :param startup_timeout: Timeout (in seconds) for startup of the pod
             (if pod is pending for too long, fails task)
         :return:
         """
         curr_time = datetime.now()
@@ -332,17 +335,28 @@
         *,
         follow=False,
         since_time: DateTime | None = None,
         post_termination_timeout: int = 120,
     ) -> PodLoggingStatus:
         """
         Follows the logs of container and streams to airflow logging.
+
         Returns when container exits.
+
+        Between when the pod starts and logs being available, there might be a delay due to CSR not approved
+        and signed yet. In such situation, ApiException is thrown. This is why we are retrying on this
+        specific exception.
         """
 
+        @tenacity.retry(
+            retry=tenacity.retry_if_exception_type(ApiException),
+            stop=tenacity.stop_after_attempt(10),
+            wait=tenacity.wait_fixed(1),
+            before=before_log(self.log, logging.INFO),
+        )
         def consume_logs(
             *, since_time: DateTime | None = None, follow: bool = True, termination_timeout: int = 120
         ) -> DateTime | None:
             """
             Tries to follow container logs until container completes.
             For a long-running container, sometimes the log read may be interrupted
             Such errors of this kind are suppressed.
@@ -396,40 +410,40 @@
                     pod.metadata.name,
                     container_name,
                 )
                 time.sleep(1)
 
     def await_container_completion(self, pod: V1Pod, container_name: str) -> None:
         """
-        Waits for the given container in the given pod to be completed
+        Waits for the given container in the given pod to be completed.
 
         :param pod: pod spec that will be monitored
         :param container_name: name of the container within the pod to monitor
         """
         while not self.container_is_terminated(pod=pod, container_name=container_name):
             time.sleep(1)
 
     def await_pod_completion(self, pod: V1Pod) -> V1Pod:
         """
-        Monitors a pod and returns the final state
+        Monitors a pod and returns the final state.
 
         :param pod: pod spec that will be monitored
         :return: tuple[State, str | None]
         """
         while True:
             remote_pod = self.read_pod(pod)
             if remote_pod.status.phase in PodPhase.terminal_states:
                 break
             self.log.info("Pod %s has phase %s", pod.metadata.name, remote_pod.status.phase)
             time.sleep(2)
         return remote_pod
 
     def parse_log_line(self, line: str) -> tuple[DateTime | None, str]:
         """
-        Parse K8s log line and returns the final state
+        Parse K8s log line and returns the final state.
 
         :param line: k8s log line
         :return: timestamp and log message
         """
         split_at = line.find(" ")
         if split_at == -1:
             self.log.error(
@@ -444,35 +458,35 @@
             last_log_time = cast(DateTime, pendulum.parse(timestamp))
         except ParserError:
             self.log.error("Error parsing timestamp. Will continue execution but won't update timestamp")
             return None, line
         return last_log_time, message
 
     def container_is_running(self, pod: V1Pod, container_name: str) -> bool:
-        """Reads pod and checks if container is running"""
+        """Reads pod and checks if container is running."""
         remote_pod = self.read_pod(pod)
         return container_is_running(pod=remote_pod, container_name=container_name)
 
     def container_is_terminated(self, pod: V1Pod, container_name: str) -> bool:
-        """Reads pod and checks if container is terminated"""
+        """Reads pod and checks if container is terminated."""
         remote_pod = self.read_pod(pod)
         return container_is_terminated(pod=remote_pod, container_name=container_name)
 
     @tenacity.retry(stop=tenacity.stop_after_attempt(3), wait=tenacity.wait_exponential(), reraise=True)
     def read_pod_logs(
         self,
         pod: V1Pod,
         container_name: str,
         tail_lines: int | None = None,
         timestamps: bool = False,
         since_seconds: int | None = None,
         follow=True,
         post_termination_timeout: int = 120,
     ) -> PodLogsConsumer:
-        """Reads log from the POD"""
+        """Reads log from the POD."""
         additional_kwargs = {}
         if since_seconds:
             additional_kwargs["since_seconds"] = since_seconds
 
         if tail_lines:
             additional_kwargs["tail_lines"] = tail_lines
 
@@ -496,25 +510,25 @@
             pod_manager=self,
             container_name=container_name,
             post_termination_timeout=post_termination_timeout,
         )
 
     @tenacity.retry(stop=tenacity.stop_after_attempt(3), wait=tenacity.wait_exponential(), reraise=True)
     def read_pod_events(self, pod: V1Pod) -> CoreV1EventList:
-        """Reads events from the POD"""
+        """Reads events from the POD."""
         try:
             return self._client.list_namespaced_event(
                 namespace=pod.metadata.namespace, field_selector=f"involvedObject.name={pod.metadata.name}"
             )
         except BaseHTTPError as e:
             raise AirflowException(f"There was an error reading the kubernetes API: {e}")
 
     @tenacity.retry(stop=tenacity.stop_after_attempt(3), wait=tenacity.wait_exponential(), reraise=True)
     def read_pod(self, pod: V1Pod) -> V1Pod:
-        """Read POD information"""
+        """Read POD information."""
         try:
             return self._client.read_namespaced_pod(pod.metadata.name, pod.metadata.namespace)
         except BaseHTTPError as e:
             raise AirflowException(f"There was an error reading the kubernetes API: {e}")
 
     def await_xcom_sidecar_container_start(self, pod: V1Pod) -> None:
         self.log.info("Checking if xcom sidecar container is started.")
@@ -525,15 +539,15 @@
                 break
             if not warned:
                 self.log.warning("The xcom sidecar container is not yet started.")
                 warned = True
             time.sleep(1)
 
     def extract_xcom(self, pod: V1Pod) -> str:
-        """Retrieves XCom value and kills xcom sidecar container"""
+        """Retrieves XCom value and kills xcom sidecar container."""
         with closing(
             kubernetes_stream(
                 self._client.connect_get_namespaced_pod_exec,
                 pod.metadata.name,
                 pod.metadata.namespace,
                 container=PodDefaults.SIDECAR_CONTAINER_NAME,
                 command=["/bin/sh"],
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py` & `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 import copy
 
 from kubernetes.client import models as k8s
 
 
 class PodDefaults:
-    """Static defaults for Pods"""
+    """Static defaults for Pods."""
 
     XCOM_MOUNT_PATH = "/airflow/xcom"
     SIDECAR_CONTAINER_NAME = "airflow-xcom-sidecar"
     XCOM_CMD = 'trap "exit 0" INT; while true; do sleep 1; done;'
     VOLUME_MOUNT = k8s.V1VolumeMount(name="xcom", mount_path=XCOM_MOUNT_PATH)
     VOLUME = k8s.V1Volume(name="xcom", empty_dir=k8s.V1EmptyDirVolumeSource())
     SIDECAR_CONTAINER = k8s.V1Container(
@@ -50,15 +50,15 @@
 
 def add_xcom_sidecar(
     pod: k8s.V1Pod,
     *,
     sidecar_container_image: str | None = None,
     sidecar_container_resources: k8s.V1ResourceRequirements | dict | None = None,
 ) -> k8s.V1Pod:
-    """Adds sidecar"""
+    """Adds sidecar."""
     pod_cp = copy.deepcopy(pod)
     pod_cp.spec.volumes = pod.spec.volumes or []
     pod_cp.spec.volumes.insert(0, PodDefaults.VOLUME)
     pod_cp.spec.containers[0].volume_mounts = pod_cp.spec.containers[0].volume_mounts or []
     pod_cp.spec.containers[0].volume_mounts.insert(0, PodDefaults.VOLUME_MOUNT)
     sidecar = copy.deepcopy(PodDefaults.SIDECAR_CONTAINER)
     sidecar.image = sidecar_container_image or PodDefaults.SIDECAR_CONTAINER.image
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/apache_airflow_providers_cncf_kubernetes.egg-info/PKG-INFO` & `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-cncf-kubernetes
-Version: 7.0.0rc2
+Version: 7.1.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-cncf-kubernetes package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.0.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.1.0/
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
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Monitoring
-Requires-Python: ~=3.7
+Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: NOTICE
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
    or more contributor license agreements.  See the NOTICE file
@@ -48,38 +48,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-cncf-kubernetes``
 
-Release: ``7.0.0rc2``
+Release: ``7.1.0rc1``
 
 
 `Kubernetes <https://kubernetes.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``cncf.kubernetes`` provider. All classes for this provider package
 are in ``airflow.providers.cncf.kubernetes`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.0.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.1.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-cncf-kubernetes``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ======================  ==================
 PIP package             Version required
 ======================  ==================
@@ -112,15 +112,45 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+7.1.0
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+
+Features
+~~~~~~~~
+* ``KubernetesResourceOperator - KubernetesDeleteResourceOperator & KubernetesCreateResourceOperator (#29930)``
+* ``add a return when the event is yielded in a loop to stop the execution (#31985)``
+* ``Add possibility to disable logging the pod template in a case when task fails (#31595)``
+
+
+Bug Fixes
+~~~~~~~~~
+
+* ``Remove return statement after yield from triggers class (#31703)``
+* ``Fix Fargate logging for AWS system tests (#31622)``
+
+Misc
+~~~~
+
+* ``Remove Python 3.7 support (#30963)``
 
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add D400 pydocstyle check (#31742)``
+   * ``Add discoverability for triggers in provider.yaml (#31576)``
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
 
 7.0.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt` & `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,21 +14,23 @@
 airflow/providers/cncf/kubernetes/decorators/__init__.py
 airflow/providers/cncf/kubernetes/decorators/kubernetes.py
 airflow/providers/cncf/kubernetes/hooks/__init__.py
 airflow/providers/cncf/kubernetes/hooks/kubernetes.py
 airflow/providers/cncf/kubernetes/operators/__init__.py
 airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py
 airflow/providers/cncf/kubernetes/operators/pod.py
+airflow/providers/cncf/kubernetes/operators/resource.py
 airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py
 airflow/providers/cncf/kubernetes/sensors/__init__.py
 airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py
 airflow/providers/cncf/kubernetes/triggers/__init__.py
 airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py
 airflow/providers/cncf/kubernetes/triggers/pod.py
 airflow/providers/cncf/kubernetes/utils/__init__.py
+airflow/providers/cncf/kubernetes/utils/delete_from.py
 airflow/providers/cncf/kubernetes/utils/pod_manager.py
 airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py
 apache_airflow_providers_cncf_kubernetes.egg-info/PKG-INFO
 apache_airflow_providers_cncf_kubernetes.egg-info/SOURCES.txt
 apache_airflow_providers_cncf_kubernetes.egg-info/dependency_links.txt
 apache_airflow_providers_cncf_kubernetes.egg-info/entry_points.txt
 apache_airflow_providers_cncf_kubernetes.egg-info/not-zip-safe
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/pyproject.toml` & `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/setup.cfg` & `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -17,34 +17,34 @@
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
+	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.0.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/7.1.0/
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
 	apache-airflow>=2.4.0.dev0
 	asgiref>=3.5.2
@@ -56,10 +56,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.cncf.kubernetes.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.cncf.kubernetes
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-cncf-kubernetes-7.0.0rc2/setup.py` & `apache-airflow-providers-cncf-kubernetes-7.1.0rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-cncf-kubernetes package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "7.0.0"
+version = "7.1.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-cncf-kubernetes setup."""
     setup(
         version=version,
         extras_require={},
```

