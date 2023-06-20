# Comparing `tmp/phidata-1.7.5.tar.gz` & `tmp/phidata-1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phidata-1.7.5.tar", last modified: Thu Jun 15 14:47:10 2023, max compression
+gzip compressed data, was "phidata-1.7.6.tar", last modified: Tue Jun 20 14:12:36 2023, max compression
```

## Comparing `phidata-1.7.5.tar` & `phidata-1.7.6.tar`

### file list

```diff
@@ -1,530 +1,531 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.495943 phidata-1.7.5/
--rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-06-15 14:46:49.000000 phidata-1.7.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-06-15 14:47:10.495943 phidata-1.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-15 14:46:49.000000 phidata-1.7.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.427943 phidata-1.7.5/phidata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.427943 phidata-1.7.5/phidata/airflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/airflow/airflow_installed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.427943 phidata-1.7.5/phidata/airflow/operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/airflow/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/airflow/operators/empty.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.431943 phidata-1.7.5/phidata/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.431943 phidata-1.7.5/phidata/app/airflow/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   100927 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/airflow/airflow_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    30469 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/airflow/airflow_flower.py
--rw-r--r--   0 runner    (1001) docker     (123)    30508 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/airflow/airflow_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    30505 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/airflow/airflow_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    30515 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/airflow/airflow_webserver.py
--rw-r--r--   0 runner    (1001) docker     (123)    30710 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/airflow/airflow_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.431943 phidata-1.7.5/phidata/app/alertmanager/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/alertmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47889 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/alertmanager/alertmanager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.431943 phidata-1.7.5/phidata/app/amundsen/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/amundsen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48031 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/amundsen/frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    48032 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/amundsen/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    47944 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/amundsen/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.431943 phidata-1.7.5/phidata/app/assistant/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49912 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/assistant/assistant.py
--rw-r--r--   0 runner    (1001) docker     (123)    21102 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/aws_app.py
--rw-r--r--   0 runner    (1001) docker     (123)    17077 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/base_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.431943 phidata-1.7.5/phidata/app/cadvisor/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/cadvisor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49678 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/cadvisor/cadvisor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.431943 phidata-1.7.5/phidata/app/databox/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/databox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    86151 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/databox/databox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.431943 phidata-1.7.5/phidata/app/db/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/db/base_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.435943 phidata-1.7.5/phidata/app/django/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30070 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/django/django_app.py
--rw-r--r--   0 runner    (1001) docker     (123)    17176 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/docker_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.435943 phidata-1.7.5/phidata/app/elastic/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/elastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/elastic/elastic_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.435943 phidata-1.7.5/phidata/app/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48675 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/elasticsearch/elasticsearch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.435943 phidata-1.7.5/phidata/app/fastapi/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20089 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/fastapi/fastapi_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.435943 phidata-1.7.5/phidata/app/grafana/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/grafana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49781 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/grafana/grafana.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.435943 phidata-1.7.5/phidata/app/jupyter/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26862 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/jupyter/jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)    46942 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/jupyter/jupyter_hub.py
--rw-r--r--   0 runner    (1001) docker     (123)    93432 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/jupyter/jupyter_lab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.435943 phidata-1.7.5/phidata/app/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/k8s/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/k8s/dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/k8s/url.py
--rw-r--r--   0 runner    (1001) docker     (123)    37744 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/k8s_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.435943 phidata-1.7.5/phidata/app/mysql/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49110 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/mysql/mysql_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.435943 phidata-1.7.5/phidata/app/neo4j/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/neo4j/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47856 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/neo4j/neo4j.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.435943 phidata-1.7.5/phidata/app/nodeexporter/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/nodeexporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47898 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/nodeexporter/nodeexporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    38495 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/phidata_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.435943 phidata-1.7.5/phidata/app/postgres/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53156 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/postgres/postgres_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.435943 phidata-1.7.5/phidata/app/prometheus/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/prometheus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49051 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/prometheus/prometheus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.439943 phidata-1.7.5/phidata/app/qdrant/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/qdrant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19992 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/qdrant/qdrant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.439943 phidata-1.7.5/phidata/app/redis/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49058 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/redis/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)    53296 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/redis/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.439943 phidata-1.7.5/phidata/app/server/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18424 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/server/api_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    58714 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/server/server_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.439943 phidata-1.7.5/phidata/app/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49424 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/spark/spark_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17222 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/spark/spark_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    17332 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/spark/spark_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.439943 phidata-1.7.5/phidata/app/streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20030 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/streamlit/streamlit_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.439943 phidata-1.7.5/phidata/app/superset/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/superset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71570 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/superset/superset_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    22925 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/superset/superset_init.py
--rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/superset/superset_webserver.py
--rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/superset/superset_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    22917 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/superset/superset_worker_beat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.439943 phidata-1.7.5/phidata/app/traefik/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/traefik/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   115905 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/traefik/crds.py
--rw-r--r--   0 runner    (1001) docker     (123)    48190 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/traefik/ingress_route.py
--rw-r--r--   0 runner    (1001) docker     (123)    44972 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/app/traefik/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.439943 phidata-1.7.5/phidata/asset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/asset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.443943 phidata-1.7.5/phidata/asset/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/asset/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/asset/aws/aws_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)    24787 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/asset/data_asset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.443943 phidata-1.7.5/phidata/asset/local/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/asset/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14564 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/asset/local/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/asset/local/local_asset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.443943 phidata-1.7.5/phidata/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.443943 phidata-1.7.5/phidata/aws/athena/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/athena/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.443943 phidata-1.7.5/phidata/aws/create/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/create/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.443943 phidata-1.7.5/phidata/aws/create/iam/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/create/iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/create/iam/eks_admin_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/create/iam/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    23058 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.443943 phidata-1.7.5/phidata/aws/enums/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/enums/manager_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.447943 phidata-1.7.5/phidata/aws/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.447943 phidata-1.7.5/phidata/aws/resource/acm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/acm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10630 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/acm/certificate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.447943 phidata-1.7.5/phidata/aws/resource/athena/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/athena/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.447943 phidata-1.7.5/phidata/aws/resource/cloudformation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/cloudformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10882 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/cloudformation/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.447943 phidata-1.7.5/phidata/aws/resource/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/ec2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21341 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/ec2/security_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/ec2/subnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/ec2/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.451943 phidata-1.7.5/phidata/aws/resource/ecs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/ecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/ecs/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    26410 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/ecs/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    19630 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/ecs/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    22397 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/ecs/task_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/ecs/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.451943 phidata-1.7.5/phidata/aws/resource/eks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/eks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/eks/addon.py
--rw-r--r--   0 runner    (1001) docker     (123)    30104 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/eks/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    13731 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/eks/fargate_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    23785 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/eks/kubeconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)    23742 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/eks/node_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.451943 phidata-1.7.5/phidata/aws/resource/elasticache/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/elasticache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15823 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/elasticache/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/elasticache/subnet_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.455943 phidata-1.7.5/phidata/aws/resource/elb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/elb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/elb/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/elb/load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9834 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/elb/target_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.455943 phidata-1.7.5/phidata/aws/resource/emr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/emr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/emr/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.455943 phidata-1.7.5/phidata/aws/resource/glue/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12850 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/glue/crawler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.455943 phidata-1.7.5/phidata/aws/resource/iam/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/iam/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/iam/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9828 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/iam/role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.459943 phidata-1.7.5/phidata/aws/resource/rds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/rds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36056 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/rds/db_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    34672 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/rds/db_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/rds/db_subnet_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.459943 phidata-1.7.5/phidata/aws/resource/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/s3/bucket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.459943 phidata-1.7.5/phidata/aws/resource/secret/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/secret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11320 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/secret/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/secret/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    12616 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/resource/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.459943 phidata-1.7.5/phidata/aws/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21797 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/s3/csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    24100 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/s3/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14394 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/s3/dataset_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/s3/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    22470 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/aws/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.459943 phidata-1.7.5/phidata/checks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/checks/check.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/checks/not_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.463943 phidata-1.7.5/phidata/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/decorators/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/decorators/validate_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.463943 phidata-1.7.5/phidata/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/docker/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/docker/args.py
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/docker/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/docker/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/docker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/docker/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.467943 phidata-1.7.5/phidata/docker/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/docker/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/docker/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16440 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/docker/resource/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/docker/resource/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    14274 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/docker/resource/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/docker/resource/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/docker/resource/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/docker/resource/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/docker/resource/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.467943 phidata-1.7.5/phidata/docker/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/docker/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/docker/utils/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    24179 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/docker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.467943 phidata-1.7.5/phidata/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/exceptions/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/exceptions/task.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/exceptions/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.467943 phidata-1.7.5/phidata/infra/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/infra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/infra/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/infra/args.py
--rw-r--r--   0 runner    (1001) docker     (123)    15390 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/infra/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11953 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/infra/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.471943 phidata-1.7.5/phidata/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/args.py
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.471943 phidata-1.7.5/phidata/k8s/create/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/create/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.471943 phidata-1.7.5/phidata/k8s/create/apiextensions_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/create/apiextensions_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.471943 phidata-1.7.5/phidata/k8s/create/apiextensions_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/create/apiextensions_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.471943 phidata-1.7.5/phidata/k8s/create/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/create/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.471943 phidata-1.7.5/phidata/k8s/create/apps/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/create/apps/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/create/apps/v1/deployment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.471943 phidata-1.7.5/phidata/k8s/create/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/create/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/create/common/labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/create/common/port.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.471943 phidata-1.7.5/phidata/k8s/create/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/create/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.471943 phidata-1.7.5/phidata/k8s/create/core/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/create/core/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/create/core/v1/config_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/create/core/v1/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/create/core/v1/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/create/core/v1/persistent_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/create/core/v1/persistent_volume_claim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/create/core/v1/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/create/core/v1/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/create/core/v1/service_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/create/core/v1/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.475943 phidata-1.7.5/phidata/k8s/create/crb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/create/crb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/create/crb/eks_admin_crb.py
--rw-r--r--   0 runner    (1001) docker     (123)    19062 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/create/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/create/kubeconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.475943 phidata-1.7.5/phidata/k8s/create/networking_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/create/networking_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.475943 phidata-1.7.5/phidata/k8s/create/networking_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/create/networking_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/create/networking_k8s_io/v1/ingress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.475943 phidata-1.7.5/phidata/k8s/create/rbac_authorization_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/create/rbac_authorization_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.475943 phidata-1.7.5/phidata/k8s/create/rbac_authorization_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/create/rbac_authorization_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.475943 phidata-1.7.5/phidata/k8s/create/storage_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/create/storage_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.475943 phidata-1.7.5/phidata/k8s/create/storage_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/create/storage_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/create/storage_k8s_io/v1/storage_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.475943 phidata-1.7.5/phidata/k8s/enums/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/enums/api_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/enums/api_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/enums/image_pull_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/enums/kind.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/enums/manager_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/enums/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/enums/pv.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/enums/restart_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/enums/service_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/enums/storage_class.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/enums/volume_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.475943 phidata-1.7.5/phidata/k8s/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.475943 phidata-1.7.5/phidata/k8s/resource/apiextensions_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/apiextensions_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.479943 phidata-1.7.5/phidata/k8s/resource/apiextensions_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/apiextensions_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    15390 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.479943 phidata-1.7.5/phidata/k8s/resource/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.479943 phidata-1.7.5/phidata/k8s/resource/apps/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/apps/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/apps/v1/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/apps/v1/deployment_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.479943 phidata-1.7.5/phidata/k8s/resource/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.479943 phidata-1.7.5/phidata/k8s/resource/core/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/core/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/core/v1/config_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    18530 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/core/v1/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/core/v1/local_object_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/core/v1/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/core/v1/node_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/core/v1/object_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    12419 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/core/v1/persistent_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/core/v1/persistent_volume_claim.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/core/v1/pod.py
--rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/core/v1/pod_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/core/v1/pod_template_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/core/v1/resource_requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/core/v1/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)    18982 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/core/v1/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/core/v1/service_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/core/v1/toleration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/core/v1/topology_spread_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/core/v1/volume.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/core/v1/volume_node_affinity.py
--rw-r--r--   0 runner    (1001) docker     (123)    13397 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/core/v1/volume_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    13385 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/kubeconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.479943 phidata-1.7.5/phidata/k8s/resource/meta/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.483943 phidata-1.7.5/phidata/k8s/resource/meta/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/meta/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/meta/v1/label_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/meta/v1/object_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.483943 phidata-1.7.5/phidata/k8s/resource/networking_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/networking_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.483943 phidata-1.7.5/phidata/k8s/resource/networking_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/networking_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10026 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/networking_k8s_io/v1/ingress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.483943 phidata-1.7.5/phidata/k8s/resource/rbac_authorization_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/rbac_authorization_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.483943 phidata-1.7.5/phidata/k8s/resource/rbac_authorization_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/rbac_authorization_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.483943 phidata-1.7.5/phidata/k8s/resource/storage_k8s_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/storage_k8s_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.483943 phidata-1.7.5/phidata/k8s/resource/storage_k8s_io/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/storage_k8s_io/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    14693 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/resource/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.483943 phidata-1.7.5/phidata/k8s/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/utils/pod.py
--rw-r--r--   0 runner    (1001) docker     (123)    43059 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/k8s/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.483943 phidata-1.7.5/phidata/llm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/llm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.483943 phidata-1.7.5/phidata/llm/duckdb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/llm/duckdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/llm/duckdb/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/llm/duckdb/chain.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/llm/duckdb/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/llm/duckdb/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/llm/duckdb/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/llm/duckdb/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.483943 phidata-1.7.5/phidata/product/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/product/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29505 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/product/data_product.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.483943 phidata-1.7.5/phidata/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/resource/reference.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.483943 phidata-1.7.5/phidata/table/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.483943 phidata-1.7.5/phidata/table/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/table/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/table/local/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    23516 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/table/local/local_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/table/local/parquet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.487943 phidata-1.7.5/phidata/table/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/table/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/table/s3/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/table/s3/parquet.py
--rw-r--r--   0 runner    (1001) docker     (123)    23064 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/table/s3/s3_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.487943 phidata-1.7.5/phidata/table/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/table/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/table/sql/postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)    35497 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/table/sql/sql_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.487943 phidata-1.7.5/phidata/task/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.487943 phidata-1.7.5/phidata/task/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/task/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.487943 phidata-1.7.5/phidata/task/aws/athena/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/task/aws/athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/task/aws/athena/run_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.487943 phidata-1.7.5/phidata/task/aws/emr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/task/aws/emr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/task/aws/emr/create_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/task/aws/emr/delete_cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.487943 phidata-1.7.5/phidata/task/aws/glue/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/task/aws/glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/task/aws/glue/start_crawler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/task/decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.487943 phidata-1.7.5/phidata/task/dev/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/task/dev/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.487943 phidata-1.7.5/phidata/task/download/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/task/download/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.487943 phidata-1.7.5/phidata/task/download/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/task/download/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/task/download/s3/to_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.487943 phidata-1.7.5/phidata/task/download/url/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/task/download/url/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/task/download/url/to_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/task/download/url/to_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/task/download/url/to_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.487943 phidata-1.7.5/phidata/task/plot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/task/plot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.487943 phidata-1.7.5/phidata/task/plot/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/task/plot/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/task/plot/sql/query.py
--rw-r--r--   0 runner    (1001) docker     (123)    12300 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/task/python_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.487943 phidata-1.7.5/phidata/task/run/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/task/run/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.487943 phidata-1.7.5/phidata/task/run/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/task/run/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/task/run/sql/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/task/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/task/task_relatives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.491943 phidata-1.7.5/phidata/task/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/task/upload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.491943 phidata-1.7.5/phidata/task/upload/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/task/upload/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/task/upload/file/to_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/task/upload/file/to_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.491943 phidata-1.7.5/phidata/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/types/airflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/types/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/types/phidata_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/types/run_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.491943 phidata-1.7.5/phidata/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/utils/cli_console.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/utils/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/utils/dttm.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/utils/env_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/utils/env_var.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/utils/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/utils/get_python_objects_from_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/utils/json_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/utils/k8s.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/utils/print_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/utils/workspace_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/utils/yaml_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.491943 phidata-1.7.5/phidata/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/workflow/decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.491943 phidata-1.7.5/phidata/workflow/dev/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/workflow/dev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42342 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/workflow/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/workflow/workflow_relatives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.495943 phidata-1.7.5/phidata/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11316 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/workspace/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-06-15 14:46:49.000000 phidata-1.7.5/phidata/workspace/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.427943 phidata-1.7.5/phidata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-06-15 14:47:10.000000 phidata-1.7.5/phidata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13948 2023-06-15 14:47:10.000000 phidata-1.7.5/phidata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:47:10.000000 phidata-1.7.5/phidata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-15 14:47:10.000000 phidata-1.7.5/phidata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-15 14:47:10.000000 phidata-1.7.5/phidata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-15 14:46:49.000000 phidata-1.7.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 14:47:10.495943 phidata-1.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-15 14:46:49.000000 phidata-1.7.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:47:10.495943 phidata-1.7.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-15 14:46:49.000000 phidata-1.7.5/tests/test_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.585825 phidata-1.7.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-06-20 14:12:13.000000 phidata-1.7.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-06-20 14:12:36.585825 phidata-1.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-20 14:12:13.000000 phidata-1.7.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.509823 phidata-1.7.6/phidata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.509823 phidata-1.7.6/phidata/airflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/airflow/airflow_installed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.509823 phidata-1.7.6/phidata/airflow/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/airflow/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/airflow/operators/empty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.513824 phidata-1.7.6/phidata/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.513824 phidata-1.7.6/phidata/app/airflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100927 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/airflow/airflow_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30469 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/airflow/airflow_flower.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30508 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/airflow/airflow_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30505 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/airflow/airflow_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30515 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/airflow/airflow_webserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30710 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/airflow/airflow_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.513824 phidata-1.7.6/phidata/app/alertmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/alertmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47889 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/alertmanager/alertmanager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.513824 phidata-1.7.6/phidata/app/amundsen/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/amundsen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48031 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/amundsen/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48032 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/amundsen/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47944 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/amundsen/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.513824 phidata-1.7.6/phidata/app/assistant/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49912 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/assistant/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30166 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/aws_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17164 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/base_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.513824 phidata-1.7.6/phidata/app/cadvisor/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/cadvisor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49678 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/cadvisor/cadvisor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.513824 phidata-1.7.6/phidata/app/databox/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/databox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86151 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/databox/databox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.517824 phidata-1.7.6/phidata/app/db/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/db/base_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.517824 phidata-1.7.6/phidata/app/django/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27483 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/django/django_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30070 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/django/django_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17172 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/docker_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.517824 phidata-1.7.6/phidata/app/elastic/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/elastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/elastic/elastic_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.517824 phidata-1.7.6/phidata/app/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48675 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/elasticsearch/elasticsearch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.517824 phidata-1.7.6/phidata/app/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20266 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/fastapi/fastapi_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.517824 phidata-1.7.6/phidata/app/grafana/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/grafana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49781 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/grafana/grafana.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.517824 phidata-1.7.6/phidata/app/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27093 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/jupyter/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46942 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/jupyter/jupyter_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93432 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/jupyter/jupyter_lab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.517824 phidata-1.7.6/phidata/app/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/k8s/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/k8s/dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/k8s/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37830 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/k8s_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.517824 phidata-1.7.6/phidata/app/mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49110 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/mysql/mysql_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.521824 phidata-1.7.6/phidata/app/neo4j/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/neo4j/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47856 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/neo4j/neo4j.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.521824 phidata-1.7.6/phidata/app/nodeexporter/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/nodeexporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47898 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/nodeexporter/nodeexporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38495 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/phidata_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.521824 phidata-1.7.6/phidata/app/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53156 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/postgres/postgres_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.521824 phidata-1.7.6/phidata/app/prometheus/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/prometheus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49051 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/prometheus/prometheus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.521824 phidata-1.7.6/phidata/app/qdrant/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/qdrant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19992 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/qdrant/qdrant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.521824 phidata-1.7.6/phidata/app/redis/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49058 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/redis/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53296 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/redis/stack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.521824 phidata-1.7.6/phidata/app/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18424 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/server/api_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58714 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/server/server_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.525824 phidata-1.7.6/phidata/app/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49424 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/spark/spark_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17222 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/spark/spark_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17332 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/spark/spark_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.525824 phidata-1.7.6/phidata/app/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20207 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/streamlit/streamlit_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.525824 phidata-1.7.6/phidata/app/superset/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/superset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71570 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/superset/superset_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22925 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/superset/superset_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/superset/superset_webserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22910 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/superset/superset_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22917 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/superset/superset_worker_beat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.525824 phidata-1.7.6/phidata/app/traefik/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/traefik/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115905 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/traefik/crds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48190 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/traefik/ingress_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44972 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/app/traefik/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.529824 phidata-1.7.6/phidata/asset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/asset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.529824 phidata-1.7.6/phidata/asset/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/asset/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/asset/aws/aws_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24787 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/asset/data_asset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.529824 phidata-1.7.6/phidata/asset/local/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/asset/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14564 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/asset/local/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/asset/local/local_asset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.529824 phidata-1.7.6/phidata/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.529824 phidata-1.7.6/phidata/aws/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/athena/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.529824 phidata-1.7.6/phidata/aws/create/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/create/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.533824 phidata-1.7.6/phidata/aws/create/iam/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/create/iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/create/iam/eks_admin_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/create/iam/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23058 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.533824 phidata-1.7.6/phidata/aws/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/enums/manager_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.533824 phidata-1.7.6/phidata/aws/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.533824 phidata-1.7.6/phidata/aws/resource/acm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/acm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10630 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/acm/certificate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.533824 phidata-1.7.6/phidata/aws/resource/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/athena/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.533824 phidata-1.7.6/phidata/aws/resource/cloudformation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/cloudformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10882 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/cloudformation/stack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.537824 phidata-1.7.6/phidata/aws/resource/ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/ec2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21341 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/ec2/security_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/ec2/subnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/ec2/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.537824 phidata-1.7.6/phidata/aws/resource/ecs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/ecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/ecs/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26068 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/ecs/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19630 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/ecs/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22397 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/ecs/task_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/ecs/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.537824 phidata-1.7.6/phidata/aws/resource/eks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/eks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/eks/addon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30104 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/eks/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13731 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/eks/fargate_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23785 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/eks/kubeconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23742 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/eks/node_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.537824 phidata-1.7.6/phidata/aws/resource/elasticache/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/elasticache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15823 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/elasticache/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/elasticache/subnet_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.541824 phidata-1.7.6/phidata/aws/resource/elb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/elb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/elb/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/elb/load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9834 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/elb/target_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.541824 phidata-1.7.6/phidata/aws/resource/emr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/emr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/emr/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.541824 phidata-1.7.6/phidata/aws/resource/glue/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12850 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/glue/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.541824 phidata-1.7.6/phidata/aws/resource/iam/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/iam/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/iam/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9828 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/iam/role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.541824 phidata-1.7.6/phidata/aws/resource/rds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/rds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36056 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/rds/db_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35222 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/rds/db_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/rds/db_subnet_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.541824 phidata-1.7.6/phidata/aws/resource/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/s3/bucket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.545824 phidata-1.7.6/phidata/aws/resource/secret/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/secret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11398 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/secret/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/secret/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9688 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/resource/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.545824 phidata-1.7.6/phidata/aws/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21797 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/s3/csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24100 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/s3/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14394 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/s3/dataset_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/s3/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22470 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/aws/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.545824 phidata-1.7.6/phidata/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/checks/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/checks/not_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.545824 phidata-1.7.6/phidata/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/decorators/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/decorators/validate_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.549824 phidata-1.7.6/phidata/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/docker/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/docker/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/docker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/docker/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/docker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/docker/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.549824 phidata-1.7.6/phidata/docker/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/docker/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/docker/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16440 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/docker/resource/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/docker/resource/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14274 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/docker/resource/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/docker/resource/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/docker/resource/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/docker/resource/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/docker/resource/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.549824 phidata-1.7.6/phidata/docker/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/docker/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/docker/utils/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24179 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/docker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.549824 phidata-1.7.6/phidata/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/exceptions/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/exceptions/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/exceptions/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.553824 phidata-1.7.6/phidata/infra/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/infra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/infra/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/infra/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15390 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/infra/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12048 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/infra/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.553824 phidata-1.7.6/phidata/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.553824 phidata-1.7.6/phidata/k8s/create/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/create/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.553824 phidata-1.7.6/phidata/k8s/create/apiextensions_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/create/apiextensions_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.553824 phidata-1.7.6/phidata/k8s/create/apiextensions_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/create/apiextensions_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.553824 phidata-1.7.6/phidata/k8s/create/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/create/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.553824 phidata-1.7.6/phidata/k8s/create/apps/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/create/apps/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/create/apps/v1/deployment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.553824 phidata-1.7.6/phidata/k8s/create/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/create/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/create/common/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/create/common/port.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.553824 phidata-1.7.6/phidata/k8s/create/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/create/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.557824 phidata-1.7.6/phidata/k8s/create/core/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/create/core/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/create/core/v1/config_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/create/core/v1/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/create/core/v1/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/create/core/v1/persistent_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/create/core/v1/persistent_volume_claim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/create/core/v1/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/create/core/v1/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/create/core/v1/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/create/core/v1/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.557824 phidata-1.7.6/phidata/k8s/create/crb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/create/crb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/create/crb/eks_admin_crb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19062 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/create/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/create/kubeconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.557824 phidata-1.7.6/phidata/k8s/create/networking_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/create/networking_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.557824 phidata-1.7.6/phidata/k8s/create/networking_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/create/networking_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/create/networking_k8s_io/v1/ingress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.557824 phidata-1.7.6/phidata/k8s/create/rbac_authorization_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/create/rbac_authorization_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.557824 phidata-1.7.6/phidata/k8s/create/rbac_authorization_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/create/rbac_authorization_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.557824 phidata-1.7.6/phidata/k8s/create/storage_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/create/storage_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.557824 phidata-1.7.6/phidata/k8s/create/storage_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/create/storage_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/create/storage_k8s_io/v1/storage_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.561824 phidata-1.7.6/phidata/k8s/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/enums/api_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/enums/api_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/enums/image_pull_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/enums/kind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/enums/manager_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/enums/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/enums/pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/enums/restart_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/enums/service_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/enums/storage_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/enums/volume_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.561824 phidata-1.7.6/phidata/k8s/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.561824 phidata-1.7.6/phidata/k8s/resource/apiextensions_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/apiextensions_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.561824 phidata-1.7.6/phidata/k8s/resource/apiextensions_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/apiextensions_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15390 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.561824 phidata-1.7.6/phidata/k8s/resource/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.561824 phidata-1.7.6/phidata/k8s/resource/apps/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/apps/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/apps/v1/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/apps/v1/deployment_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.561824 phidata-1.7.6/phidata/k8s/resource/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.565824 phidata-1.7.6/phidata/k8s/resource/core/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/core/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/core/v1/config_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18530 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/core/v1/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/core/v1/local_object_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/core/v1/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/core/v1/node_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/core/v1/object_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12419 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/core/v1/persistent_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/core/v1/persistent_volume_claim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/core/v1/pod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/core/v1/pod_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/core/v1/pod_template_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/core/v1/resource_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/core/v1/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18982 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/core/v1/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/core/v1/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/core/v1/toleration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/core/v1/topology_spread_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/core/v1/volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/core/v1/volume_node_affinity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13397 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/core/v1/volume_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12690 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/kubeconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.565824 phidata-1.7.6/phidata/k8s/resource/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.565824 phidata-1.7.6/phidata/k8s/resource/meta/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/meta/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/meta/v1/label_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/meta/v1/object_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.565824 phidata-1.7.6/phidata/k8s/resource/networking_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/networking_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.565824 phidata-1.7.6/phidata/k8s/resource/networking_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/networking_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10026 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/networking_k8s_io/v1/ingress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.565824 phidata-1.7.6/phidata/k8s/resource/rbac_authorization_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/rbac_authorization_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.569824 phidata-1.7.6/phidata/k8s/resource/rbac_authorization_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/rbac_authorization_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.569824 phidata-1.7.6/phidata/k8s/resource/storage_k8s_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/storage_k8s_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.569824 phidata-1.7.6/phidata/k8s/resource/storage_k8s_io/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/storage_k8s_io/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10127 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/resource/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.569824 phidata-1.7.6/phidata/k8s/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/utils/pod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43059 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/k8s/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.569824 phidata-1.7.6/phidata/llm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/llm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.569824 phidata-1.7.6/phidata/llm/duckdb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/llm/duckdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/llm/duckdb/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/llm/duckdb/chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/llm/duckdb/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/llm/duckdb/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/llm/duckdb/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/llm/duckdb/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.569824 phidata-1.7.6/phidata/product/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/product/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29505 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/product/data_product.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.569824 phidata-1.7.6/phidata/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/resource/reference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.569824 phidata-1.7.6/phidata/table/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.569824 phidata-1.7.6/phidata/table/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/table/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/table/local/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23516 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/table/local/local_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/table/local/parquet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.573825 phidata-1.7.6/phidata/table/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/table/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/table/s3/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/table/s3/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23064 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/table/s3/s3_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.573825 phidata-1.7.6/phidata/table/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/table/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/table/sql/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35497 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/table/sql/sql_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.573825 phidata-1.7.6/phidata/task/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.573825 phidata-1.7.6/phidata/task/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/task/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.573825 phidata-1.7.6/phidata/task/aws/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/task/aws/athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/task/aws/athena/run_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.573825 phidata-1.7.6/phidata/task/aws/emr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/task/aws/emr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/task/aws/emr/create_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/task/aws/emr/delete_cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.573825 phidata-1.7.6/phidata/task/aws/glue/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/task/aws/glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/task/aws/glue/start_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/task/decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.573825 phidata-1.7.6/phidata/task/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/task/dev/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.573825 phidata-1.7.6/phidata/task/download/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/task/download/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.573825 phidata-1.7.6/phidata/task/download/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/task/download/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/task/download/s3/to_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.577824 phidata-1.7.6/phidata/task/download/url/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/task/download/url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/task/download/url/to_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/task/download/url/to_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/task/download/url/to_sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.577824 phidata-1.7.6/phidata/task/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/task/plot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.577824 phidata-1.7.6/phidata/task/plot/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/task/plot/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/task/plot/sql/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12300 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/task/python_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.577824 phidata-1.7.6/phidata/task/run/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/task/run/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.577824 phidata-1.7.6/phidata/task/run/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/task/run/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/task/run/sql/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/task/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/task/task_relatives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.577824 phidata-1.7.6/phidata/task/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/task/upload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.577824 phidata-1.7.6/phidata/task/upload/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/task/upload/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/task/upload/file/to_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/task/upload/file/to_sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.577824 phidata-1.7.6/phidata/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/types/airflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/types/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/types/phidata_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/types/run_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.581824 phidata-1.7.6/phidata/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/utils/cli_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/utils/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/utils/dttm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/utils/env_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/utils/env_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/utils/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/utils/get_python_objects_from_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/utils/json_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/utils/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/utils/print_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/utils/workspace_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/utils/yaml_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.585825 phidata-1.7.6/phidata/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/workflow/decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.585825 phidata-1.7.6/phidata/workflow/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/workflow/dev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42342 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/workflow/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/workflow/workflow_relatives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.585825 phidata-1.7.6/phidata/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11316 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/workspace/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-06-20 14:12:13.000000 phidata-1.7.6/phidata/workspace/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.509823 phidata-1.7.6/phidata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-06-20 14:12:36.000000 phidata-1.7.6/phidata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13984 2023-06-20 14:12:36.000000 phidata-1.7.6/phidata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:12:36.000000 phidata-1.7.6/phidata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-20 14:12:36.000000 phidata-1.7.6/phidata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 14:12:36.000000 phidata-1.7.6/phidata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-20 14:12:13.000000 phidata-1.7.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 14:12:36.585825 phidata-1.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-20 14:12:13.000000 phidata-1.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:12:36.585825 phidata-1.7.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-20 14:12:13.000000 phidata-1.7.6/tests/test_placeholder.py
```

### Comparing `phidata-1.7.5/LICENSE` & `phidata-1.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/PKG-INFO` & `phidata-1.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phidata
-Version: 1.7.5
+Version: 1.7.6
 Summary: Phidata is a toolkit for building applications using OSS
 Author-email: Ashpreet Bedi <ashpreet@phidata.com>
 Project-URL: homepage, https://phidata.com
 Project-URL: documentation, https://docs.phidata.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: phidata Version: 1.7.5 Summary: Phidata is a
+Metadata-Version: 2.1 Name: phidata Version: 1.7.6 Summary: Phidata is a
 toolkit for building applications using OSS Author-email: Ashpreet Bedi
 phidata.com> Project-URL: homepage, https://phidata.com Project-URL:
 documentation, https://docs.phidata.com Requires-Python: >=3.7 Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: aws License-
 File: LICENSE
                              ****** phidata ******
           A toolkit for building applications using open source tools
```

### Comparing `phidata-1.7.5/README.md` & `phidata-1.7.6/README.md`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/airflow/operators/empty.py` & `phidata-1.7.6/phidata/airflow/operators/empty.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/airflow/airflow_base.py` & `phidata-1.7.6/phidata/app/airflow/airflow_base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/airflow/airflow_flower.py` & `phidata-1.7.6/phidata/app/airflow/airflow_flower.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/airflow/airflow_manager.py` & `phidata-1.7.6/phidata/app/airflow/airflow_manager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/airflow/airflow_scheduler.py` & `phidata-1.7.6/phidata/app/airflow/airflow_scheduler.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/airflow/airflow_webserver.py` & `phidata-1.7.6/phidata/app/airflow/airflow_webserver.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/airflow/airflow_worker.py` & `phidata-1.7.6/phidata/app/airflow/airflow_worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/alertmanager/alertmanager.py` & `phidata-1.7.6/phidata/app/alertmanager/alertmanager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/amundsen/frontend.py` & `phidata-1.7.6/phidata/app/amundsen/frontend.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/amundsen/metadata.py` & `phidata-1.7.6/phidata/app/amundsen/metadata.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/amundsen/search.py` & `phidata-1.7.6/phidata/app/amundsen/search.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/assistant/assistant.py` & `phidata-1.7.6/phidata/app/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/aws_app.py` & `phidata-1.7.6/phidata/app/aws_app.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,14 +11,16 @@
     # List of subnets: str or Subnet
     aws_subnets: Optional[List[Any]] = None
     # List of security groups: str or SecurityGroup
     aws_security_groups: Optional[List[Any]] = None
 
     # -*- ECS Configuration
     ecs_cluster: Optional[Any] = None
+    # If ecs_cluster is None, create a new cluster with ecs_cluster_name
+    ecs_cluster_name: Optional[str] = None
     ecs_launch_type: str = "FARGATE"
     ecs_task_cpu: str = "1024"
     ecs_task_memory: str = "2048"
     ecs_service_count: int = 1
     assign_public_ip: Optional[bool] = None
     ecs_enable_exec: bool = True
 
@@ -87,14 +89,23 @@
 
     @ecs_cluster.setter
     def ecs_cluster(self, ecs_cluster: Any) -> None:
         if self.args is not None and ecs_cluster is not None:
             self.args.ecs_cluster = ecs_cluster
 
     @property
+    def ecs_cluster_name(self) -> Optional[str]:
+        return self.args.ecs_cluster_name
+
+    @ecs_cluster_name.setter
+    def ecs_cluster_name(self, ecs_cluster_name: str) -> None:
+        if self.args is not None and ecs_cluster_name is not None:
+            self.args.ecs_cluster_name = ecs_cluster_name
+
+    @property
     def ecs_launch_type(self) -> Optional[str]:
         return self.args.ecs_launch_type
 
     @ecs_launch_type.setter
     def ecs_launch_type(self, ecs_launch_type: str) -> None:
         if self.args is not None and ecs_launch_type is not None:
             self.args.ecs_launch_type = ecs_launch_type
@@ -141,59 +152,196 @@
 
     @ecs_enable_exec.setter
     def ecs_enable_exec(self, ecs_enable_exec: bool) -> None:
         if self.args is not None and ecs_enable_exec is not None:
             self.args.ecs_enable_exec = ecs_enable_exec
 
     @property
-    def create_load_balancer(self) -> Optional[bool]:
-        return self.args.create_load_balancer
-
-    @create_load_balancer.setter
-    def create_load_balancer(self, create_load_balancer: bool) -> None:
-        if self.args is not None and create_load_balancer is not None:
-            self.args.create_load_balancer = create_load_balancer
-
-    @property
     def load_balancer(self) -> Optional[Any]:
         return self.args.load_balancer
 
     @load_balancer.setter
     def load_balancer(self, load_balancer: Any) -> None:
         if self.args is not None and load_balancer is not None:
             self.args.load_balancer = load_balancer
 
     @property
+    def listener(self) -> Optional[Any]:
+        return self.args.listener
+
+    @listener.setter
+    def listener(self, listener: Any) -> None:
+        if self.args is not None and listener is not None:
+            self.args.listener = listener
+
+    @property
+    def create_load_balancer(self) -> Optional[bool]:
+        return self.args.create_load_balancer
+
+    @create_load_balancer.setter
+    def create_load_balancer(self, create_load_balancer: bool) -> None:
+        if self.args is not None and create_load_balancer is not None:
+            self.args.create_load_balancer = create_load_balancer
+
+    @property
     def load_balancer_protocol(self) -> Optional[str]:
         return self.args.load_balancer_protocol
 
     @load_balancer_protocol.setter
     def load_balancer_protocol(self, load_balancer_protocol: str) -> None:
         if self.args is not None and load_balancer_protocol is not None:
             self.args.load_balancer_protocol = load_balancer_protocol
 
     @property
+    def load_balancer_security_groups(self) -> Optional[List[Any]]:
+        return self.args.load_balancer_security_groups
+
+    @load_balancer_security_groups.setter
+    def load_balancer_security_groups(
+        self, load_balancer_security_groups: List[Any]
+    ) -> None:
+        if self.args is not None and load_balancer_security_groups is not None:
+            self.args.load_balancer_security_groups = load_balancer_security_groups
+
+    @property
     def load_balancer_port(self) -> Optional[int]:
         return self.args.load_balancer_port
 
     @load_balancer_port.setter
     def load_balancer_port(self, load_balancer_port: int) -> None:
         if self.args is not None and load_balancer_port is not None:
             self.args.load_balancer_port = load_balancer_port
 
     @property
+    def load_balancer_certificate(self) -> Optional[Any]:
+        return self.args.load_balancer_certificate
+
+    @load_balancer_certificate.setter
+    def load_balancer_certificate(self, load_balancer_certificate: Any) -> None:
+        if self.args is not None and load_balancer_certificate is not None:
+            self.args.load_balancer_certificate = load_balancer_certificate
+
+    @property
     def load_balancer_certificate_arn(self) -> Optional[str]:
         return self.args.load_balancer_certificate_arn
 
     @load_balancer_certificate_arn.setter
     def load_balancer_certificate_arn(self, load_balancer_certificate_arn: str) -> None:
         if self.args is not None and load_balancer_certificate_arn is not None:
             self.args.load_balancer_certificate_arn = load_balancer_certificate_arn
 
-    def get_container_env_ecs(
+    @property
+    def target_group(self) -> Optional[Any]:
+        return self.args.target_group
+
+    @target_group.setter
+    def target_group(self, target_group: Any) -> None:
+        if self.args is not None and target_group is not None:
+            self.args.target_group = target_group
+
+    @property
+    def target_group_protocol(self) -> Optional[str]:
+        return self.args.target_group_protocol
+
+    @target_group_protocol.setter
+    def target_group_protocol(self, target_group_protocol: str) -> None:
+        if self.args is not None and target_group_protocol is not None:
+            self.args.target_group_protocol = target_group_protocol
+
+    @property
+    def target_group_port(self) -> Optional[int]:
+        return self.args.target_group_port
+
+    @target_group_port.setter
+    def target_group_port(self, target_group_port: int) -> None:
+        if self.args is not None and target_group_port is not None:
+            self.args.target_group_port = target_group_port
+
+    @property
+    def target_group_type(self) -> Optional[str]:
+        return self.args.target_group_type
+
+    @target_group_type.setter
+    def target_group_type(self, target_group_type: str) -> None:
+        if self.args is not None and target_group_type is not None:
+            self.args.target_group_type = target_group_type
+
+    @property
+    def health_check_protocol(self) -> Optional[str]:
+        return self.args.health_check_protocol
+
+    @health_check_protocol.setter
+    def health_check_protocol(self, health_check_protocol: str) -> None:
+        if self.args is not None and health_check_protocol is not None:
+            self.args.health_check_protocol = health_check_protocol
+
+    @property
+    def health_check_port(self) -> Optional[str]:
+        return self.args.health_check_port
+
+    @health_check_port.setter
+    def health_check_port(self, health_check_port: str) -> None:
+        if self.args is not None and health_check_port is not None:
+            self.args.health_check_port = health_check_port
+
+    @property
+    def health_check_enabled(self) -> Optional[bool]:
+        return self.args.health_check_enabled
+
+    @health_check_enabled.setter
+    def health_check_enabled(self, health_check_enabled: bool) -> None:
+        if self.args is not None and health_check_enabled is not None:
+            self.args.health_check_enabled = health_check_enabled
+
+    @property
+    def health_check_path(self) -> Optional[str]:
+        return self.args.health_check_path
+
+    @health_check_path.setter
+    def health_check_path(self, health_check_path: str) -> None:
+        if self.args is not None and health_check_path is not None:
+            self.args.health_check_path = health_check_path
+
+    @property
+    def health_check_interval_seconds(self) -> Optional[int]:
+        return self.args.health_check_interval_seconds
+
+    @health_check_interval_seconds.setter
+    def health_check_interval_seconds(self, health_check_interval_seconds: int) -> None:
+        if self.args is not None and health_check_interval_seconds is not None:
+            self.args.health_check_interval_seconds = health_check_interval_seconds
+
+    @property
+    def health_check_timeout_seconds(self) -> Optional[int]:
+        return self.args.health_check_timeout_seconds
+
+    @health_check_timeout_seconds.setter
+    def health_check_timeout_seconds(self, health_check_timeout_seconds: int) -> None:
+        if self.args is not None and health_check_timeout_seconds is not None:
+            self.args.health_check_timeout_seconds = health_check_timeout_seconds
+
+    @property
+    def healthy_threshold_count(self) -> Optional[int]:
+        return self.args.healthy_threshold_count
+
+    @healthy_threshold_count.setter
+    def healthy_threshold_count(self, healthy_threshold_count: int) -> None:
+        if self.args is not None and healthy_threshold_count is not None:
+            self.args.healthy_threshold_count = healthy_threshold_count
+
+    @property
+    def unhealthy_threshold_count(self) -> Optional[int]:
+        return self.args.unhealthy_threshold_count
+
+    @unhealthy_threshold_count.setter
+    def unhealthy_threshold_count(self, unhealthy_threshold_count: int) -> None:
+        if self.args is not None and unhealthy_threshold_count is not None:
+            self.args.unhealthy_threshold_count = unhealthy_threshold_count
+
+    def build_container_env_ecs(
         self, container_paths: ContainerPathContext
     ) -> Dict[str, str]:
         from phidata.constants import (
             PYTHONPATH_ENV_VAR,
             PHIDATA_RUNTIME_ENV_VAR,
             SCRIPTS_DIR_ENV_VAR,
             STORAGE_DIR_ENV_VAR,
@@ -263,249 +411,327 @@
             container_env.update(
                 {k: v for k, v in self.args.env.items() if v is not None}
             )
 
         # logger.debug("Container Environment: {}".format(container_env))
         return container_env
 
-    def get_container_command_aws(self) -> Optional[List[str]]:
-        if isinstance(self.args.command, str):
-            return self.args.command.split(" ")
-        return self.args.command
-
-    def get_aws_rg(
-        self, aws_build_context: Any, defer_api_calls: bool = False
-    ) -> Optional[Any]:
-        from phidata.aws.resource.group import (
-            AwsResourceGroup,
-            EcsCluster,
-            EcsContainer,
-            EcsTaskDefinition,
-            EcsService,
-            LoadBalancer,
-            TargetGroup,
-            Listener,
-            AcmCertificate,
-            SecurityGroup,
-        )
-
-        # -*- Build Container Paths
-        container_paths: Optional[ContainerPathContext] = self.get_container_paths()
-        if container_paths is None:
-            raise Exception("Could not build Container Paths")
-        logger.debug(f"ContainerPaths: {container_paths.json(indent=2)}")
-
-        app_name = self.name
-        workspace_name = container_paths.workspace_name
-        logger.debug(f"Building AwsResourceGroup: {app_name} for {workspace_name}")
-
-        # -*- Build Container Environment
-        container_env: Dict[str, str] = self.get_container_env_ecs(
-            container_paths=container_paths
-        )
+    def build_security_groups(self) -> Optional[List[Any]]:
+        from phidata.aws.resource.ec2.security_group import SecurityGroup
 
-        # -*- Create Security Groups
         security_groups: List[SecurityGroup] = []
-        if self.args.aws_security_groups is not None:
-            for sg in self.args.aws_security_groups:
-                if isinstance(sg, SecurityGroup):
-                    security_groups.append(sg)
         if self.args.load_balancer_security_groups is not None:
             for lb_sg in self.args.load_balancer_security_groups:
                 if isinstance(lb_sg, SecurityGroup):
                     security_groups.append(lb_sg)
+        if self.args.aws_security_groups is not None:
+            for sg in self.args.aws_security_groups:
+                if isinstance(sg, SecurityGroup):
+                    security_groups.append(sg)
+
+        return security_groups if len(security_groups) > 0 else None
+
+    def build_ecs_cluster(self) -> Optional[Any]:
+        from phidata.aws.resource.ecs.cluster import EcsCluster
 
-        # -*- Create ECS cluster
-        ecs_cluster = self.args.ecs_cluster
-        if ecs_cluster is None:
-            ecs_cluster = EcsCluster(
-                name=f"{app_name}-cluster",
-                ecs_cluster_name=app_name,
+        if self.args.ecs_cluster is None:
+            return EcsCluster(
+                name=f"{self.app_name}-cluster",
+                ecs_cluster_name=self.args.ecs_cluster_name or self.app_name,
                 capacity_providers=[self.args.ecs_launch_type],
                 save_output=self.args.save_output,
-                resource_dir=self.args.resource_dir or app_name,
+                resource_dir=self.args.resource_dir or self.app_name,
                 skip_create=self.args.skip_create,
                 skip_delete=self.args.skip_delete,
                 wait_for_creation=self.args.wait_for_creation,
                 wait_for_deletion=self.args.wait_for_deletion,
             )
+        elif isinstance(self.args.ecs_cluster, EcsCluster):
+            return self.args.ecs_cluster
+        else:
+            raise Exception(
+                f"Invalid ECSCluster: {self.args.ecs_cluster} - Must be of type EcsCluster"
+            )
+
+    def build_load_balancer(self) -> Optional[Any]:
+        from phidata.aws.resource.elb.load_balancer import LoadBalancer
 
-        # -*- Create Load Balancer
-        load_balancer = self.args.load_balancer
-        if load_balancer is None and self.args.create_load_balancer:
+        if self.args.load_balancer is None and self.args.create_load_balancer:
             if self.args.load_balancer_protocol not in ["HTTP", "HTTPS"]:
                 raise Exception(
                     "Load Balancer Protocol must be one of: HTTP, HTTPS. "
                     f"Got: {self.args.load_balancer_protocol}"
                 )
-            load_balancer_sgs = (
-                self.args.load_balancer_security_groups or self.args.aws_security_groups
-            )
-            load_balancer = LoadBalancer(
-                name=f"{app_name}-lb",
+            return LoadBalancer(
+                name=f"{self.app_name}-lb",
                 subnets=self.args.aws_subnets,
-                security_groups=load_balancer_sgs,
+                security_groups=self.args.load_balancer_security_groups
+                or self.args.aws_security_groups,
                 protocol=self.args.load_balancer_protocol,
                 save_output=self.args.save_output,
-                resource_dir=self.args.resource_dir or app_name,
+                resource_dir=self.args.resource_dir or self.app_name,
                 skip_create=self.args.skip_create,
                 skip_delete=self.args.skip_delete,
                 wait_for_creation=self.args.wait_for_creation,
                 wait_for_deletion=self.args.wait_for_deletion,
             )
+        elif isinstance(self.args.load_balancer, LoadBalancer):
+            return self.args.load_balancer
+        else:
+            raise Exception(
+                f"Invalid LoadBalancer: {self.args.load_balancer} - Must be of type LoadBalancer"
+            )
+
+    def build_target_group(self) -> Optional[Any]:
+        from phidata.aws.resource.elb.target_group import TargetGroup
 
-        # -*- Create Target Group
-        target_group = self.args.target_group
-        if target_group is None and self.args.create_load_balancer:
+        if self.args.target_group is None and self.args.create_load_balancer:
             if self.args.target_group_protocol not in ["HTTP", "HTTPS"]:
                 raise Exception(
                     "Target Group Protocol must be one of: HTTP, HTTPS. "
                     f"Got: {self.args.target_group_protocol}"
                 )
-            target_group = TargetGroup(
-                name=f"{app_name}-tg",
-                port=self.container_port,
+            return TargetGroup(
+                name=f"{self.app_name}-tg",
+                port=self.args.target_group_port or self.container_port,
                 protocol=self.args.target_group_protocol,
                 subnets=self.args.aws_subnets,
                 target_type=self.args.target_group_type,
                 health_check_protocol=self.args.health_check_protocol,
                 health_check_port=self.args.health_check_port,
                 health_check_enabled=self.args.health_check_enabled,
                 health_check_path=self.args.health_check_path,
                 health_check_interval_seconds=self.args.health_check_interval_seconds,
                 health_check_timeout_seconds=self.args.health_check_timeout_seconds,
                 healthy_threshold_count=self.args.healthy_threshold_count,
                 unhealthy_threshold_count=self.args.unhealthy_threshold_count,
                 save_output=self.args.save_output,
-                resource_dir=self.args.resource_dir or app_name,
+                resource_dir=self.args.resource_dir or self.app_name,
                 skip_create=self.args.skip_create,
                 skip_delete=self.args.skip_delete,
                 wait_for_creation=self.args.wait_for_creation,
                 wait_for_deletion=self.args.wait_for_deletion,
             )
+        elif isinstance(self.args.target_group, TargetGroup):
+            return self.args.target_group
+        else:
+            raise Exception(
+                f"Invalid TargetGroup: {self.args.target_group} - Must be of type TargetGroup"
+            )
+
+    def build_listener(self, load_balancer: Any, target_group: Any) -> Optional[Any]:
+        from phidata.aws.resource.elb.listener import Listener
 
-        # -*- Create Listener
-        listener = self.args.listener
-        if listener is None and self.args.create_load_balancer:
+        if self.args.listener is None and self.args.create_load_balancer:
             listener = Listener(
-                name=f"{app_name}-listener",
+                name=f"{self.app_name}-listener",
                 load_balancer=load_balancer,
                 target_group=target_group,
                 save_output=self.args.save_output,
-                resource_dir=self.args.resource_dir or app_name,
+                resource_dir=self.args.resource_dir or self.app_name,
                 skip_create=self.args.skip_create,
                 skip_delete=self.args.skip_delete,
                 wait_for_creation=self.args.wait_for_creation,
                 wait_for_deletion=self.args.wait_for_deletion,
             )
             if self.args.load_balancer_certificate_arn is not None:
                 listener.certificates = [
                     {"CertificateArn": self.args.load_balancer_certificate_arn}
                 ]
             if self.args.load_balancer_certificate is not None:
                 listener.acm_certificates = [self.args.load_balancer_certificate]
+            return listener
+        elif isinstance(self.args.listener, Listener):
+            return self.args.listener
+        else:
+            raise Exception(
+                f"Invalid Listener: {self.args.listener} - Must be of type Listener"
+            )
+
+    def build_container_command_aws(self) -> Optional[List[str]]:
+        if isinstance(self.args.command, str):
+            return self.args.command.strip().split(" ")
+        return self.args.command
+
+    def build_ecs_container(
+        self, container_paths: ContainerPathContext
+    ) -> Optional[Any]:
+        from phidata.aws.resource.ecs.container import EcsContainer
+
+        # -*- Build Container Environment
+        container_env: Dict[str, str] = self.build_container_env_ecs(
+            container_paths=container_paths
+        )
 
         # -*- Build Container Command
-        container_cmd: Optional[List[str]] = self.get_container_command_aws()
+        container_cmd: Optional[List[str]] = self.build_container_command_aws()
         if container_cmd:
             logger.debug("Command: {}".format(" ".join(container_cmd)))
 
-        # -*- Create ECS Container
-        ecs_container = EcsContainer(
-            name=app_name,
+        return EcsContainer(
+            name=self.app_name,
             image=self.get_image_str(),
             port_mappings=[{"containerPort": self.container_port}],
             command=container_cmd,
+            essential=True,
             environment=[{"name": k, "value": v} for k, v in container_env.items()],
             log_configuration={
                 "logDriver": "awslogs",
                 "options": {
-                    "awslogs-group": app_name,
+                    "awslogs-group": self.app_name,
                     "awslogs-region": self.aws_region,
                     "awslogs-create-group": "true",
-                    "awslogs-stream-prefix": app_name,
+                    "awslogs-stream-prefix": self.app_name,
                 },
             },
+            linux_parameters={"initProcessEnabled": True},
             env_from_secrets=self.args.aws_secrets,
             save_output=self.args.save_output,
-            resource_dir=self.args.resource_dir or app_name,
+            resource_dir=self.args.resource_dir or self.app_name,
             skip_create=self.args.skip_create,
             skip_delete=self.args.skip_delete,
             wait_for_creation=self.args.wait_for_creation,
             wait_for_deletion=self.args.wait_for_deletion,
         )
 
-        # -*- Create ECS Task Definition
-        ecs_task_definition = EcsTaskDefinition(
-            name=f"{app_name}-td",
-            family=app_name,
+    def build_ecs_task_definition(self, ecs_container: Any) -> Optional[Any]:
+        from phidata.aws.resource.ecs.task_definition import EcsTaskDefinition
+
+        return EcsTaskDefinition(
+            name=f"{self.app_name}-td",
+            family=self.app_name,
             network_mode="awsvpc",
             cpu=self.args.ecs_task_cpu,
             memory=self.args.ecs_task_memory,
             containers=[ecs_container],
             requires_compatibilities=[self.args.ecs_launch_type],
-            add_ecs_exec_policy=True,
+            add_ecs_exec_policy=self.args.ecs_enable_exec,
             add_ecs_secret_policy=True,
             save_output=self.args.save_output,
-            resource_dir=self.args.resource_dir or app_name,
+            resource_dir=self.args.resource_dir or self.app_name,
             skip_create=self.args.skip_create,
             skip_delete=self.args.skip_delete,
             wait_for_creation=self.args.wait_for_creation,
             wait_for_deletion=self.args.wait_for_deletion,
         )
 
-        # -*- Create ECS Service
-        ecs_service = EcsService(
-            name=f"{app_name}-service",
+    def build_ecs_service(
+        self,
+        ecs_cluster: Any,
+        ecs_task_definition: Any,
+        target_group: Any,
+        ecs_container: Any,
+    ) -> Optional[Any]:
+        from phidata.aws.resource.ecs.service import EcsService
+
+        return EcsService(
+            name=f"{self.app_name}-service",
             desired_count=self.args.ecs_service_count,
             launch_type=self.args.ecs_launch_type,
             cluster=ecs_cluster,
             task_definition=ecs_task_definition,
             target_group=target_group,
             target_container_name=ecs_container.name,
             target_container_port=self.container_port,
             subnets=self.args.aws_subnets,
             security_groups=self.args.aws_security_groups,
             assign_public_ip=self.args.assign_public_ip,
             # Force delete the service.
             force_delete=True,
             # Force a new deployment of the service on update.
             force_new_deployment=True,
+            enable_execute_command=self.args.ecs_enable_exec,
             save_output=self.args.save_output,
-            resource_dir=self.args.resource_dir or app_name,
+            resource_dir=self.args.resource_dir or self.app_name,
             skip_create=self.args.skip_create,
             skip_delete=self.args.skip_delete,
             wait_for_creation=self.args.wait_for_creation,
             wait_for_deletion=self.args.wait_for_deletion,
         )
 
+    def get_aws_rg(self, aws_build_context: Any) -> Optional[Any]:
+        from phidata.aws.resource.group import (
+            AwsResourceGroup,
+            EcsCluster,
+            EcsContainer,
+            EcsTaskDefinition,
+            EcsService,
+            LoadBalancer,
+            TargetGroup,
+            Listener,
+            AcmCertificate,
+            SecurityGroup,
+        )
+
+        # -*- Build Container Paths
+        container_paths: Optional[ContainerPathContext] = self.build_container_paths()
+        if container_paths is None:
+            raise Exception("Could not build Container Paths")
+        logger.debug(f"ContainerPaths: {container_paths.json(indent=2)}")
+
+        workspace_name = container_paths.workspace_name
+        logger.debug(f"Building AwsResourceGroup: {self.app_name} for {workspace_name}")
+
+        # -*- Build Security Groups
+        security_groups: Optional[List[SecurityGroup]] = self.build_security_groups()
+
+        # -*- Build ECS cluster
+        ecs_cluster: Optional[EcsCluster] = self.build_ecs_cluster()
+
+        # -*- Build Load Balancer
+        load_balancer: Optional[LoadBalancer] = self.build_load_balancer()
+
+        # -*- Build Target Group
+        target_group: Optional[TargetGroup] = self.build_target_group()
+
+        # -*- Build Listener
+        listener: Optional[Listener] = self.build_listener(
+            load_balancer=load_balancer, target_group=target_group
+        )
+
+        # -*- Build ECSContainer
+        ecs_container: Optional[EcsContainer] = self.build_ecs_container(
+            container_paths=container_paths
+        )
+
+        # -*- Build ECS Task Definition
+        ecs_task_definition: Optional[
+            EcsTaskDefinition
+        ] = self.build_ecs_task_definition(ecs_container=ecs_container)
+
+        # -*- Build ECS Service
+        ecs_service: Optional[EcsService] = self.build_ecs_service(
+            ecs_cluster=ecs_cluster,
+            ecs_task_definition=ecs_task_definition,
+            target_group=target_group,
+            ecs_container=ecs_container,
+        )
+
         # -*- Create AwsResourceGroup
         return AwsResourceGroup(
-            name=app_name,
+            name=self.app_name,
             enabled=self.enabled,
             ecs_clusters=[ecs_cluster],
             ecs_task_definitions=[ecs_task_definition],
             ecs_services=[ecs_service],
             load_balancers=[load_balancer],
             target_groups=[target_group],
             listeners=[listener],
-            security_groups=security_groups if len(security_groups) > 0 else None,
+            security_groups=security_groups,
         )
 
-    def build_aws_resource_groups(
-        self, aws_build_context: Any, defer_api_calls: bool = False
-    ) -> None:
+    def build_aws_resource_groups(self, aws_build_context: Any) -> None:
         aws_rg = self.get_aws_rg(aws_build_context)
         if aws_rg is not None:
             if self.aws_resource_groups is None:
                 self.aws_resource_groups = OrderedDict()
             self.aws_resource_groups[aws_rg.name] = aws_rg
 
     def get_aws_resource_groups(
-        self, aws_build_context: Any, defer_api_calls: bool = False
+        self, aws_build_context: Any
     ) -> Optional[Dict[str, Any]]:
         if self.aws_resource_groups is None:
             self.build_aws_resource_groups(aws_build_context)
         # # Comment out in production
         # if self.aws_resource_groups:
         #     logger.debug("AwsResourceGroups:")
         #     for rg_name, rg in self.aws_resource_groups.items():
```

### Comparing `phidata-1.7.5/phidata/app/base_app.py` & `phidata-1.7.6/phidata/app/base_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,14 +178,18 @@
         # Container paths used by the app
         self.container_paths: Optional[ContainerPathContext] = None
 
         # Args for the BaseApp, updated by the subclass
         self.args: BaseAppArgs = BaseAppArgs()
 
     @property
+    def app_name(self) -> str:
+        return self.name
+
+    @property
     def workspace_root_path(self) -> Optional[Path]:
         return self.args.workspace_root_path
 
     @workspace_root_path.setter
     def workspace_root_path(self, workspace_root_path: Path) -> None:
         if self.args is not None and workspace_root_path is not None:
             self.args.workspace_root_path = workspace_root_path
@@ -354,15 +358,17 @@
     def get_secret_data(self) -> Optional[Dict[str, str]]:
         if self.secret_data is None:
             from phidata.utils.yaml_io import read_yaml_file
 
             self.secret_data = read_yaml_file(file_path=self.args.secrets_file)
         return self.secret_data
 
-    def get_container_paths(self) -> Optional[ContainerPathContext]:
+    def build_container_paths(self) -> Optional[ContainerPathContext]:
+        logger.debug("Building ContainerPathContext")
+
         if self.container_paths is not None:
             return self.container_paths
 
         if self.workspace_root_path is None:
             logger.error("Invalid workspace_root_path")
             return None
 
@@ -422,36 +428,37 @@
             )
 
         if self.args.requirements_file is not None:
             container_paths.requirements_file = (
                 f"{workspace_root_container_path}/{self.args.requirements_file}"
             )
 
-        return container_paths
+        self.container_paths = container_paths
+        return self.container_paths
 
     def set_aws_env_vars(self, env_dict: Dict[str, str]) -> None:
         from phidata.constants import (
             AWS_REGION_ENV_VAR,
             AWS_DEFAULT_REGION_ENV_VAR,
         )
 
         if self.aws_region is not None:
             env_dict[AWS_REGION_ENV_VAR] = self.aws_region
             env_dict[AWS_DEFAULT_REGION_ENV_VAR] = self.aws_region
 
     def get_docker_resource_groups(
-        self, docker_build_context: Any, defer_api_calls: bool = False
+        self, docker_build_context: Any
     ) -> Optional[Dict[str, Any]]:
         logger.debug(f"@get_docker_resource_groups not defined for {self.name}")
         return None
 
     def get_k8s_resource_groups(
-        self, k8s_build_context: Any, defer_api_calls: bool = False
+        self, k8s_build_context: Any
     ) -> Optional[Dict[str, Any]]:
         logger.debug(f"@get_k8s_resource_groups not defined for {self.name}")
         return None
 
     def get_aws_resource_groups(
-        self, aws_build_context: Any, defer_api_calls: bool = False
+        self, aws_build_context: Any
     ) -> Optional[Dict[str, Any]]:
         logger.debug(f"@get_aws_resource_groups not defined for {self.name}")
         return None
```

### Comparing `phidata-1.7.5/phidata/app/cadvisor/cadvisor.py` & `phidata-1.7.6/phidata/app/cadvisor/cadvisor.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/databox/databox.py` & `phidata-1.7.6/phidata/app/databox/databox.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/db/base_db.py` & `phidata-1.7.6/phidata/app/db/base_db.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/django/django_app.py` & `phidata-1.7.6/phidata/app/django/django_backup.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/docker_app.py` & `phidata-1.7.6/phidata/app/docker_app.py`

 * *Files 5% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     @container_restart_policy.setter
     def container_restart_policy(
         self, container_restart_policy: Dict[str, Any]
     ) -> None:
         if self.args is not None and container_restart_policy is not None:
             self.args.container_restart_policy = container_restart_policy
 
-    def get_container_env_docker(
+    def build_container_env_docker(
         self, container_paths: ContainerPathContext
     ) -> Dict[str, str]:
         from phidata.constants import (
             PYTHONPATH_ENV_VAR,
             PHIDATA_RUNTIME_ENV_VAR,
             SCRIPTS_DIR_ENV_VAR,
             STORAGE_DIR_ENV_VAR,
@@ -194,15 +194,15 @@
             container_env.update(
                 {k: str(v) for k, v in self.args.env.items() if v is not None}
             )
 
         # logger.debug("Container Environment: {}".format(container_env))
         return container_env
 
-    def get_container_volumes_docker(
+    def build_container_volumes_docker(
         self, container_paths: ContainerPathContext
     ) -> Dict[str, dict]:
         from phidata.utils.common import get_default_volume_name
 
         if self.workspace_root_path is None:
             logger.error("Invalid workspace_root_path")
             return {}
@@ -260,15 +260,15 @@
             container_volumes[resources_dir_path] = {
                 "bind": self.args.resources_dir_container_path,
                 "mode": "ro",
             }
 
         return container_volumes
 
-    def get_container_ports_docker(self) -> Dict[str, int]:
+    def build_container_ports_docker(self) -> Dict[str, int]:
         # container_ports is a dictionary which configures the ports to bind
         # inside the container. The key is the port to bind inside the container
         #   either as an integer or a string in the form port/protocol
         # and the value is the corresponding port to open on the host.
         # For example:
         #   {'2222/tcp': 3333} will expose port 2222 inside the container as port 3333 on the host.
         container_ports: Dict[str, int] = self.args.container_ports or {}
@@ -276,58 +276,59 @@
         if self.args.open_container_port:
             container_ports[
                 str(self.args.container_port)
             ] = self.args.container_host_port
 
         return container_ports
 
-    def get_container_command_docker(self) -> Optional[List[str]]:
+    def build_container_command_docker(self) -> Optional[List[str]]:
         if isinstance(self.args.command, str):
-            return self.args.command.split(" ")
+            return self.args.command.strip().split(" ")
         return self.args.command
 
     def get_docker_rg(self, docker_build_context: Any) -> Optional[Any]:
         from phidata.docker.resource.group import (
             DockerNetwork,
             DockerContainer,
             DockerResourceGroup,
             DockerBuildContext,
         )
 
         # -*- Build Container Paths
-        container_paths: Optional[ContainerPathContext] = self.get_container_paths()
+        container_paths: Optional[ContainerPathContext] = self.build_container_paths()
         if container_paths is None:
             raise Exception("Could not build Container Paths")
-        # logger.debug(f"ContainerPaths: {container_paths.json(indent=2)}")
+        logger.debug(f"ContainerPaths: {container_paths.json(indent=2)}")
 
-        app_name = self.name
         workspace_name = container_paths.workspace_name
-        logger.debug(f"Building DockerResourceGroup: {app_name} for {workspace_name}")
+        logger.debug(
+            f"Building DockerResourceGroup: {self.app_name} for {workspace_name}"
+        )
 
         if docker_build_context is None or not isinstance(
             docker_build_context, DockerBuildContext
         ):
             logger.error("docker_build_context must be a DockerBuildContext")
             return None
 
         # -*- Build Container Environment
-        container_env: Dict[str, str] = self.get_container_env_docker(
+        container_env: Dict[str, str] = self.build_container_env_docker(
             container_paths=container_paths
         )
 
         # -*- Build Container Volumes
-        container_volumes = self.get_container_volumes_docker(
+        container_volumes = self.build_container_volumes_docker(
             container_paths=container_paths
         )
 
         # -*- Build Container Ports
-        container_ports: Dict[str, int] = self.get_container_ports_docker()
+        container_ports: Dict[str, int] = self.build_container_ports_docker()
 
         # -*- Build Container Command
-        container_cmd: Optional[List[str]] = self.get_container_command_docker()
+        container_cmd: Optional[List[str]] = self.build_container_command_docker()
         if container_cmd:
             logger.debug("Command: {}".format(" ".join(container_cmd)))
 
         # -*- Create DockerContainer
         docker_container = DockerContainer(
             name=self.container_name,
             image=self.get_image_str(),
@@ -353,15 +354,15 @@
             user=self.args.container_user,
             volumes=container_volumes if len(container_volumes) > 0 else None,
             working_dir=self.args.container_working_dir,
             use_cache=self.args.use_cache,
         )
 
         docker_rg = DockerResourceGroup(
-            name=app_name,
+            name=self.app_name,
             enabled=self.args.enabled,
             network=DockerNetwork(name=docker_build_context.network),
             containers=[docker_container],
             images=[self.args.image] if self.args.image else None,
         )
         return docker_rg
 
@@ -369,15 +370,15 @@
         docker_rg = self.get_docker_rg(docker_build_context)
         if docker_rg is not None:
             if self.docker_resource_groups is None:
                 self.docker_resource_groups = OrderedDict()
             self.docker_resource_groups[docker_rg.name] = docker_rg
 
     def get_docker_resource_groups(
-        self, docker_build_context: Any, defer_api_calls: bool = False
+        self, docker_build_context: Any
     ) -> Optional[Dict[str, Any]]:
         if self.docker_resource_groups is None:
             self.build_docker_resource_groups(docker_build_context)
         # Comment out in production
         # if self.docker_resource_groups:
         #     logger.debug("DockerResourceGroups:")
         #     for rg_name, rg in self.docker_resource_groups.items():
```

### Comparing `phidata-1.7.5/phidata/app/elastic/elastic_app.py` & `phidata-1.7.6/phidata/app/elastic/elastic_app.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/elasticsearch/elasticsearch.py` & `phidata-1.7.6/phidata/app/elasticsearch/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/fastapi/fastapi_server.py` & `phidata-1.7.6/phidata/app/qdrant/qdrant.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,33 +10,31 @@
     ImagePullPolicy,
     RestartPolicy,
     ServiceType,
 )
 from phidata.utils.log import logger
 
 
-class FastApiServerArgs(AwsAppArgs, DockerAppArgs, K8sAppArgs):
+class QdrantArgs(AwsAppArgs, DockerAppArgs, K8sAppArgs):
     pass
 
 
-class FastApiServer(AwsApp, DockerApp, K8sApp):
+class Qdrant(AwsApp, DockerApp, K8sApp):
     def __init__(
         self,
-        name: str = "fastapi",
+        name: str = "qdrant",
         version: str = "1",
         enabled: bool = True,
         # -*- Image Configuration,
         # Image can be provided as a DockerImage object or as image_name:image_tag
         image: Optional[Any] = None,
-        image_name: str = "phidata/fastapi",
-        image_tag: str = "0.96",
+        image_name: str = "qdrant/qdrant",
+        image_tag: str = "v1.2.2",
         entrypoint: Optional[Union[str, List[str]]] = None,
-        command: Union[
-            str, List[str]
-        ] = "uvicorn main:app --reload --host 0.0.0.0 --port 9090",
+        command: Optional[Union[str, List]] = None,
         # -*- Debug Mode
         debug_mode: bool = False,
         # -*- Python Configuration,
         # Install python dependencies using a requirements.txt file,
         install_requirements: bool = False,
         # Path to the requirements.txt file relative to the workspace_root,
         requirements_file: str = "requirements.txt",
@@ -58,19 +56,19 @@
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
         # -*- Container Ports,
         # Open a container port if open_container_port=True,
         open_container_port: bool = True,
         # Port number on the container,
-        container_port: int = 9090,
+        container_port: int = 6333,
         # Port name (only used by the K8sContainer),
         container_port_name: str = "http",
         # Host port to map to the container port,
-        container_host_port: int = 9090,
+        container_host_port: int = 6333,
         # -*- Workspace Volume,
         # Mount the workspace directory on the container,
         mount_workspace: bool = False,
         workspace_volume_name: Optional[str] = None,
         workspace_volume_type: Optional[WorkspaceVolumeType] = None,
         # Path to mount the workspace volume inside the container,
         workspace_dir_container_path: str = "/usr/local/app",
@@ -161,15 +159,15 @@
         topology_spread_when_unsatisfiable: Optional[str] = None,
         # -*- Service Configuration,
         create_service: bool = False,
         service_name: Optional[str] = None,
         # Type: ServiceType,
         service_type: Optional[Any] = None,
         # The port exposed by the service.,
-        service_port: int = 9090,
+        service_port: int = 6333,
         # The node_port exposed by the service if service_type = ServiceType.NODE_PORT,
         service_node_port: Optional[int] = None,
         # The target_port is the port to access on the pods targeted by the service.,
         # It can be the port number or port name on the pod.,
         service_target_port: Optional[Union[str, int]] = None,
         # Extra ports exposed by the webserver service. Type: List[CreatePort],
         service_ports: Optional[List[Any]] = None,
@@ -266,17 +264,16 @@
         use_cache: bool = True,
         #  -*- Other args,
         print_env_on_load: bool = False,
         # Extra kwargs used to capture additional args,
         **extra_kwargs,
     ):
         super().__init__()
-
         try:
-            self.args: FastApiServerArgs = FastApiServerArgs(
+            self.args: QdrantArgs = QdrantArgs(
                 name=name,
                 version=version,
                 enabled=enabled,
                 image=image,
                 image_name=image_name,
                 image_tag=image_tag,
                 entrypoint=entrypoint,
```

### Comparing `phidata-1.7.5/phidata/app/grafana/grafana.py` & `phidata-1.7.6/phidata/app/grafana/grafana.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/group.py` & `phidata-1.7.6/phidata/app/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/jupyter/jupyter.py` & `phidata-1.7.6/phidata/app/jupyter/jupyter.py`

 * *Files 2% similar despite different names*

```diff
@@ -263,14 +263,16 @@
         # Type: CreateClusterRoleBinding,
         cluster_role_binding: Optional[Any] = None,
         # -*- AWS Configuration,
         aws_subnets: Optional[List[str]] = None,
         aws_security_groups: Optional[List[Any]] = None,
         # -*- ECS Configuration,
         ecs_cluster: Optional[Any] = None,
+        # If ecs_cluster is None, create a new cluster with ecs_cluster_name,
+        ecs_cluster_name: Optional[str] = None,
         ecs_launch_type: str = "FARGATE",
         ecs_task_cpu: str = "1024",
         ecs_task_memory: str = "2048",
         ecs_service_count: int = 1,
         assign_public_ip: bool = True,
         ecs_enable_exec: bool = True,
         # -*- LoadBalancer Configuration,
@@ -438,14 +440,15 @@
                 cr_name=cr_name,
                 cluster_role=cluster_role,
                 crb_name=crb_name,
                 cluster_role_binding=cluster_role_binding,
                 aws_subnets=aws_subnets,
                 aws_security_groups=aws_security_groups,
                 ecs_cluster=ecs_cluster,
+                ecs_cluster_name=ecs_cluster_name,
                 ecs_launch_type=ecs_launch_type,
                 ecs_task_cpu=ecs_task_cpu,
                 ecs_task_memory=ecs_task_memory,
                 ecs_service_count=ecs_service_count,
                 assign_public_ip=assign_public_ip,
                 ecs_enable_exec=ecs_enable_exec,
                 load_balancer=load_balancer,
@@ -484,61 +487,62 @@
                 print_env_on_load=print_env_on_load,
                 **extra_kwargs,
             )
         except Exception as e:
             logger.error(f"Args for {self.name} are not valid: {e}")
             raise
 
-    def get_container_command_docker(self) -> Optional[List[str]]:
+    def build_container_command_docker(self) -> Optional[List[str]]:
         container_cmd: List[str]
         if isinstance(self.args.command, str):
             container_cmd = self.args.command.split(" ")
         elif isinstance(self.args.command, list):
             container_cmd = self.args.command
         else:
             container_cmd = ["jupyter", "lab"]
 
         if self.args.jupyter_config_file is not None:
             container_cmd.append(f"--config={str(self.args.jupyter_config_file)}")
 
         if self.args.notebook_dir is None:
             if self.args.mount_workspace:
-                container_paths = self.get_container_paths()
+                container_paths = self.build_container_paths()
                 if (
                     container_paths is not None
                     and container_paths.workspace_root is not None
                 ):
                     container_cmd.append(
                         f"--notebook-dir={str(container_paths.workspace_root)}"
                     )
             else:
                 container_cmd.append("--notebook-dir=/")
         else:
             container_cmd.append(f"--notebook-dir={str(self.args.notebook_dir)}")
         return container_cmd
 
-    def get_container_args_k8s(self) -> Optional[List[str]]:
+    def build_container_args_k8s(self) -> Optional[List[str]]:
         container_args: List[str]
         if isinstance(self.args.command, str):
             container_args = self.args.command.split(" ")
         elif isinstance(self.args.command, list):
             container_args = self.args.command
         else:
             container_args = ["jupyter", "lab"]
 
         if self.args.jupyter_config_file is not None:
             container_args.append(f"--config={str(self.args.jupyter_config_file)}")
 
         if self.args.notebook_dir is None:
             if self.args.mount_workspace:
+                container_paths = self.build_container_paths()
                 if (
-                    self.container_paths is not None
-                    and self.container_paths.workspace_root is not None
+                    container_paths is not None
+                    and container_paths.workspace_root is not None
                 ):
                     container_args.append(
-                        f"--notebook-dir={str(self.container_paths.workspace_root)}"
+                        f"--notebook-dir={str(container_paths.workspace_root)}"
                     )
             else:
                 container_args.append("--notebook-dir=/")
         else:
             container_args.append(f"--notebook-dir={str(self.args.notebook_dir)}")
         return container_args
```

### Comparing `phidata-1.7.5/phidata/app/jupyter/jupyter_hub.py` & `phidata-1.7.6/phidata/app/jupyter/jupyter_hub.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/jupyter/jupyter_lab.py` & `phidata-1.7.6/phidata/app/jupyter/jupyter_lab.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/k8s/app.py` & `phidata-1.7.6/phidata/app/k8s/app.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/k8s/dir.py` & `phidata-1.7.6/phidata/app/k8s/dir.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/k8s/url.py` & `phidata-1.7.6/phidata/app/k8s/url.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/k8s_app.py` & `phidata-1.7.6/phidata/app/k8s_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -239,15 +239,15 @@
         return self.args.crb_name or get_default_crb_name(self.name)
 
     @crb_name.setter
     def crb_name(self, crb_name: str) -> None:
         if self.args is not None and crb_name is not None:
             self.args.crb_name = crb_name
 
-    def get_cr_policy_rules(self) -> List[Any]:
+    def build_cr_policy_rules(self) -> List[Any]:
         from phidata.k8s.create.rbac_authorization_k8s_io.v1.cluster_role import (
             PolicyRule,
         )
 
         return [
             PolicyRule(
                 api_groups=[""],
@@ -262,15 +262,15 @@
             PolicyRule(
                 api_groups=[""],
                 resources=["pods/exec"],
                 verbs=["get", "create", "watch", "delete"],
             ),
         ]
 
-    def get_container_env_k8s(
+    def build_container_env_k8s(
         self, container_paths: ContainerPathContext
     ) -> Dict[str, str]:
         from phidata.constants import (
             PYTHONPATH_ENV_VAR,
             PHIDATA_RUNTIME_ENV_VAR,
             SCRIPTS_DIR_ENV_VAR,
             STORAGE_DIR_ENV_VAR,
@@ -332,47 +332,47 @@
         if self.args.env is not None and isinstance(self.args.env, dict):
             container_env.update(
                 {k: str(v) for k, v in self.args.env.items() if v is not None}
             )
 
         return container_env
 
-    def get_container_labels_k8s(
+    def build_container_labels_k8s(
         self, common_labels: Optional[Dict[str, str]]
     ) -> Dict[str, str]:
         labels: Dict[str, str] = common_labels or {}
         if self.args.container_labels is not None and isinstance(
             self.args.container_labels, dict
         ):
             labels.update(self.args.container_labels)
         return labels
 
-    def get_deployment_labels_k8s(
+    def build_deployment_labels_k8s(
         self, common_labels: Optional[Dict[str, str]]
     ) -> Dict[str, str]:
         labels: Dict[str, str] = common_labels or {}
         if self.args.container_labels is not None and isinstance(
             self.args.container_labels, dict
         ):
             labels.update(self.args.container_labels)
         return labels
 
-    def get_service_labels_k8s(
+    def build_service_labels_k8s(
         self, common_labels: Optional[Dict[str, str]]
     ) -> Dict[str, str]:
         labels: Dict[str, str] = common_labels or {}
         if self.args.container_labels is not None and isinstance(
             self.args.container_labels, dict
         ):
             labels.update(self.args.container_labels)
         return labels
 
-    def get_container_args_k8s(self) -> Optional[List[str]]:
+    def build_container_args_k8s(self) -> Optional[List[str]]:
         if isinstance(self.args.command, str):
-            return self.args.command.split(" ")
+            return self.args.command.strip().split(" ")
         return self.args.command
 
     def get_k8s_rg(self, k8s_build_context: Any) -> Optional[Any]:
         from phidata.k8s.create.common.port import CreatePort
         from phidata.k8s.create.core.v1.container import CreateContainer
         from phidata.k8s.create.core.v1.volume import (
             CreateVolume,
@@ -397,15 +397,15 @@
             CreatePVC,
         )
         from phidata.k8s.resource.group import K8sBuildContext
         from phidata.types.context import ContainerPathContext
         from phidata.utils.common import get_default_volume_name
 
         # -*- Build Container Paths
-        container_paths: Optional[ContainerPathContext] = self.get_container_paths()
+        container_paths: Optional[ContainerPathContext] = self.build_container_paths()
         if container_paths is None:
             raise Exception("Could not build Container Paths")
         # logger.debug(f"ContainerPaths: {container_paths.json(indent=2)}")
 
         app_name = self.name
         workspace_name = container_paths.workspace_name
         logger.debug(f"Building K8sResourceGroup: {app_name} for {workspace_name}")
@@ -467,15 +467,15 @@
                 )
             sa_name = sa.sa_name
 
             # Create Cluster Role for this App
             if cr is None:
                 cr = CreateClusterRole(
                     cr_name=self.cr_name,
-                    rules=self.get_cr_policy_rules(),
+                    rules=self.build_cr_policy_rules(),
                     app_name=app_name,
                     labels=common_labels,
                 )
 
             # Create ClusterRoleBinding for this App
             if crb is None:
                 crb = CreateClusterRoleBinding(
@@ -484,15 +484,15 @@
                     service_account_name=sa.sa_name,
                     app_name=app_name,
                     namespace=ns_name,
                     labels=common_labels,
                 )
 
         # -*- Build Container Environment
-        container_env: Dict[str, str] = self.get_container_env_k8s(
+        container_env: Dict[str, str] = self.build_container_env_k8s(
             container_paths=container_paths
         )
         # Create a ConfigMap to set the Container Environment
         container_env_cm = CreateConfigMap(
             cm_name=self.configmap_name,
             app_name=app_name,
             namespace=ns_name,
@@ -744,18 +744,20 @@
                 service_port=self.args.service_port,
                 target_port=self.args.service_target_port
                 or self.args.container_port_name,
             )
             ports.append(container_port)
 
         # -*- Build Container Labels
-        container_labels: Dict[str, str] = self.get_container_labels_k8s(common_labels)
+        container_labels: Dict[str, str] = self.build_container_labels_k8s(
+            common_labels
+        )
 
         # -*- Build Container Args: Equivalent to docker CMD
-        container_args: Optional[List[str]] = self.get_container_args_k8s()
+        container_args: Optional[List[str]] = self.build_container_args_k8s()
         if container_args:
             logger.debug("Command: {}".format(" ".join(container_args)))
 
         # -*- Create the Container
         container = CreateContainer(
             container_name=self.container_name,
             app_name=app_name,
@@ -790,15 +792,15 @@
         # -*- Add pod annotations
         if self.args.pod_annotations is not None and isinstance(
             self.args.pod_annotations, dict
         ):
             pod_annotations.update(self.args.pod_annotations)
 
         # -*- Build Deployment Labels
-        deploy_labels: Dict[str, str] = self.get_deployment_labels_k8s(common_labels)
+        deploy_labels: Dict[str, str] = self.build_deployment_labels_k8s(common_labels)
 
         # If using EbsVolume, restart the deployment on update
         recreate_deployment_on_update = (
             True
             if (
                 self.args.create_app_volume
                 and self.args.app_volume_type == AppVolumeType.AwsEbs
@@ -827,15 +829,17 @@
             topology_spread_when_unsatisfiable=self.args.topology_spread_when_unsatisfiable,
             recreate_on_update=recreate_deployment_on_update,
         )
         deployments.append(deployment)
 
         # -*- Create the Service
         if self.args.create_service:
-            service_labels: Dict[str, str] = self.get_service_labels_k8s(common_labels)
+            service_labels: Dict[str, str] = self.build_service_labels_k8s(
+                common_labels
+            )
             _service = CreateService(
                 service_name=self.service_name,
                 app_name=app_name,
                 namespace=ns_name,
                 service_account_name=sa_name,
                 service_type=self.args.service_type,
                 deployment=deployment,
```

### Comparing `phidata-1.7.5/phidata/app/mysql/mysql_db.py` & `phidata-1.7.6/phidata/app/mysql/mysql_db.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/neo4j/neo4j.py` & `phidata-1.7.6/phidata/app/neo4j/neo4j.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/nodeexporter/nodeexporter.py` & `phidata-1.7.6/phidata/app/nodeexporter/nodeexporter.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/phidata_app.py` & `phidata-1.7.6/phidata/app/phidata_app.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/postgres/postgres_db.py` & `phidata-1.7.6/phidata/app/postgres/postgres_db.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/prometheus/prometheus.py` & `phidata-1.7.6/phidata/app/prometheus/prometheus.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/qdrant/qdrant.py` & `phidata-1.7.6/phidata/app/fastapi/fastapi_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,31 +10,33 @@
     ImagePullPolicy,
     RestartPolicy,
     ServiceType,
 )
 from phidata.utils.log import logger
 
 
-class QdrantArgs(AwsAppArgs, DockerAppArgs, K8sAppArgs):
+class FastApiServerArgs(AwsAppArgs, DockerAppArgs, K8sAppArgs):
     pass
 
 
-class Qdrant(AwsApp, DockerApp, K8sApp):
+class FastApiServer(AwsApp, DockerApp, K8sApp):
     def __init__(
         self,
-        name: str = "qdrant",
+        name: str = "fastapi",
         version: str = "1",
         enabled: bool = True,
         # -*- Image Configuration,
         # Image can be provided as a DockerImage object or as image_name:image_tag
         image: Optional[Any] = None,
-        image_name: str = "qdrant/qdrant",
-        image_tag: str = "v1.2.2",
+        image_name: str = "phidata/fastapi",
+        image_tag: str = "0.96",
         entrypoint: Optional[Union[str, List[str]]] = None,
-        command: Optional[Union[str, List]] = None,
+        command: Union[
+            str, List[str]
+        ] = "uvicorn main:app --reload --host 0.0.0.0 --port 9090",
         # -*- Debug Mode
         debug_mode: bool = False,
         # -*- Python Configuration,
         # Install python dependencies using a requirements.txt file,
         install_requirements: bool = False,
         # Path to the requirements.txt file relative to the workspace_root,
         requirements_file: str = "requirements.txt",
@@ -56,19 +58,19 @@
         secrets_file: Optional[Path] = None,
         # Read secret variables from AWS Secrets,
         aws_secrets: Optional[Any] = None,
         # -*- Container Ports,
         # Open a container port if open_container_port=True,
         open_container_port: bool = True,
         # Port number on the container,
-        container_port: int = 6333,
+        container_port: int = 9090,
         # Port name (only used by the K8sContainer),
         container_port_name: str = "http",
         # Host port to map to the container port,
-        container_host_port: int = 6333,
+        container_host_port: int = 9090,
         # -*- Workspace Volume,
         # Mount the workspace directory on the container,
         mount_workspace: bool = False,
         workspace_volume_name: Optional[str] = None,
         workspace_volume_type: Optional[WorkspaceVolumeType] = None,
         # Path to mount the workspace volume inside the container,
         workspace_dir_container_path: str = "/usr/local/app",
@@ -159,15 +161,15 @@
         topology_spread_when_unsatisfiable: Optional[str] = None,
         # -*- Service Configuration,
         create_service: bool = False,
         service_name: Optional[str] = None,
         # Type: ServiceType,
         service_type: Optional[Any] = None,
         # The port exposed by the service.,
-        service_port: int = 6333,
+        service_port: int = 9090,
         # The node_port exposed by the service if service_type = ServiceType.NODE_PORT,
         service_node_port: Optional[int] = None,
         # The target_port is the port to access on the pods targeted by the service.,
         # It can be the port number or port name on the pod.,
         service_target_port: Optional[Union[str, int]] = None,
         # Extra ports exposed by the webserver service. Type: List[CreatePort],
         service_ports: Optional[List[Any]] = None,
@@ -207,14 +209,16 @@
         # Type: CreateClusterRoleBinding,
         cluster_role_binding: Optional[Any] = None,
         # -*- AWS Configuration,
         aws_subnets: Optional[List[str]] = None,
         aws_security_groups: Optional[List[Any]] = None,
         # -*- ECS Configuration,
         ecs_cluster: Optional[Any] = None,
+        # If ecs_cluster is None, create a new cluster with ecs_cluster_name,
+        ecs_cluster_name: Optional[str] = None,
         ecs_launch_type: str = "FARGATE",
         ecs_task_cpu: str = "1024",
         ecs_task_memory: str = "2048",
         ecs_service_count: int = 1,
         assign_public_ip: bool = True,
         ecs_enable_exec: bool = True,
         # -*- LoadBalancer Configuration,
@@ -264,16 +268,17 @@
         use_cache: bool = True,
         #  -*- Other args,
         print_env_on_load: bool = False,
         # Extra kwargs used to capture additional args,
         **extra_kwargs,
     ):
         super().__init__()
+
         try:
-            self.args: QdrantArgs = QdrantArgs(
+            self.args: FastApiServerArgs = FastApiServerArgs(
                 name=name,
                 version=version,
                 enabled=enabled,
                 image=image,
                 image_name=image_name,
                 image_tag=image_tag,
                 entrypoint=entrypoint,
@@ -356,14 +361,15 @@
                 cr_name=cr_name,
                 cluster_role=cluster_role,
                 crb_name=crb_name,
                 cluster_role_binding=cluster_role_binding,
                 aws_subnets=aws_subnets,
                 aws_security_groups=aws_security_groups,
                 ecs_cluster=ecs_cluster,
+                ecs_cluster_name=ecs_cluster_name,
                 ecs_launch_type=ecs_launch_type,
                 ecs_task_cpu=ecs_task_cpu,
                 ecs_task_memory=ecs_task_memory,
                 ecs_service_count=ecs_service_count,
                 assign_public_ip=assign_public_ip,
                 ecs_enable_exec=ecs_enable_exec,
                 load_balancer=load_balancer,
```

### Comparing `phidata-1.7.5/phidata/app/redis/redis.py` & `phidata-1.7.6/phidata/app/redis/redis.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/redis/stack.py` & `phidata-1.7.6/phidata/app/redis/stack.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/server/api_server.py` & `phidata-1.7.6/phidata/app/server/api_server.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/server/server_base.py` & `phidata-1.7.6/phidata/app/server/server_base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/spark/spark_base.py` & `phidata-1.7.6/phidata/app/spark/spark_base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/spark/spark_driver.py` & `phidata-1.7.6/phidata/app/spark/spark_driver.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/spark/spark_worker.py` & `phidata-1.7.6/phidata/app/spark/spark_worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/streamlit/streamlit_app.py` & `phidata-1.7.6/phidata/app/streamlit/streamlit_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,14 +207,16 @@
         # Type: CreateClusterRoleBinding,
         cluster_role_binding: Optional[Any] = None,
         # -*- AWS Configuration,
         aws_subnets: Optional[List[str]] = None,
         aws_security_groups: Optional[List[Any]] = None,
         # -*- ECS Configuration,
         ecs_cluster: Optional[Any] = None,
+        # If ecs_cluster is None, create a new cluster with ecs_cluster_name,
+        ecs_cluster_name: Optional[str] = None,
         ecs_launch_type: str = "FARGATE",
         ecs_task_cpu: str = "1024",
         ecs_task_memory: str = "2048",
         ecs_service_count: int = 1,
         assign_public_ip: bool = True,
         ecs_enable_exec: bool = True,
         # -*- LoadBalancer Configuration,
@@ -357,14 +359,15 @@
                 cr_name=cr_name,
                 cluster_role=cluster_role,
                 crb_name=crb_name,
                 cluster_role_binding=cluster_role_binding,
                 aws_subnets=aws_subnets,
                 aws_security_groups=aws_security_groups,
                 ecs_cluster=ecs_cluster,
+                ecs_cluster_name=ecs_cluster_name,
                 ecs_launch_type=ecs_launch_type,
                 ecs_task_cpu=ecs_task_cpu,
                 ecs_task_memory=ecs_task_memory,
                 ecs_service_count=ecs_service_count,
                 assign_public_ip=assign_public_ip,
                 ecs_enable_exec=ecs_enable_exec,
                 load_balancer=load_balancer,
```

### Comparing `phidata-1.7.5/phidata/app/superset/superset_base.py` & `phidata-1.7.6/phidata/app/superset/superset_base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/superset/superset_init.py` & `phidata-1.7.6/phidata/app/superset/superset_init.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/superset/superset_webserver.py` & `phidata-1.7.6/phidata/app/superset/superset_webserver.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/superset/superset_worker.py` & `phidata-1.7.6/phidata/app/superset/superset_worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/superset/superset_worker_beat.py` & `phidata-1.7.6/phidata/app/superset/superset_worker_beat.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/traefik/crds.py` & `phidata-1.7.6/phidata/app/traefik/crds.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/traefik/ingress_route.py` & `phidata-1.7.6/phidata/app/traefik/ingress_route.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/app/traefik/router.py` & `phidata-1.7.6/phidata/app/traefik/router.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/asset/aws/aws_asset.py` & `phidata-1.7.6/phidata/asset/aws/aws_asset.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/asset/data_asset.py` & `phidata-1.7.6/phidata/asset/data_asset.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/asset/local/file.py` & `phidata-1.7.6/phidata/asset/local/file.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/asset/local/local_asset.py` & `phidata-1.7.6/phidata/asset/local/local_asset.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/aws/api_client.py` & `phidata-1.7.6/phidata/aws/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/aws/athena/query.py` & `phidata-1.7.6/phidata/aws/athena/query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/aws/config.py` & `phidata-1.7.6/phidata/aws/config.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/aws/create/iam/eks_admin_role.py` & `phidata-1.7.6/phidata/aws/create/iam/eks_admin_role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/aws/create/iam/role.py` & `phidata-1.7.6/phidata/aws/create/iam/role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/aws/driver.py` & `phidata-1.7.6/phidata/aws/driver.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/aws/enums/manager_status.py` & `phidata-1.7.6/phidata/aws/enums/manager_status.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/aws/manager.py` & `phidata-1.7.6/phidata/aws/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/aws/resource/acm/certificate.py` & `phidata-1.7.6/phidata/aws/resource/acm/certificate.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/aws/resource/athena/query.py` & `phidata-1.7.6/phidata/aws/resource/athena/query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/aws/resource/base.py` & `phidata-1.7.6/phidata/aws/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/aws/resource/cloudformation/stack.py` & `phidata-1.7.6/phidata/aws/resource/cloudformation/stack.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/aws/resource/ec2/security_group.py` & `phidata-1.7.6/phidata/aws/resource/ec2/security_group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/aws/resource/ec2/subnet.py` & `phidata-1.7.6/phidata/aws/resource/ec2/subnet.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/aws/resource/ec2/volume.py` & `phidata-1.7.6/phidata/aws/resource/ec2/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/aws/resource/ecs/cluster.py` & `phidata-1.7.6/phidata/aws/resource/ecs/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/aws/resource/ecs/container.py` & `phidata-1.7.6/phidata/aws/resource/ecs/container.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,55 +187,51 @@
     ) -> List[Dict[str, Any]]:
         logger.debug("Building container environment")
         container_environment: List[Dict[str, Any]] = []
         if self.environment is not None:
             from phidata.resource.reference import Reference, AwsReference
 
             for env in self.environment:
+                env_name = env.get("name", None)
                 env_value = env.get("value", None)
                 if isinstance(env_value, Reference):
-                    env_name = env.get("name", None)
                     logger.debug(f"{env_name} is a Reference")
                     try:
                         env_val = env_value.get_reference()
-                        try:
-                            env_val_str = str(env_val)
-                            container_environment.append(
-                                {"name": env_name, "value": env_val_str}
-                            )
-                        except Exception as e:
-                            logger.error(
-                                f"Error while converting {env_val} to str: {e}"
-                            )
                     except Exception as e:
                         logger.error(f"Error while getting {env_name}: {e}")
+                        env_value = None
                 elif isinstance(env_value, AwsReference):
-                    env_name = env.get("name", None)
                     logger.debug(f"{env_name} is a AwsReference")
                     try:
                         env_val = env_value.get_reference(aws_client=aws_client)
-                        try:
-                            env_val_str = str(env_val)
-                            container_environment.append(
-                                {"name": env_name, "value": env_val_str}
-                            )
-                        except Exception as e:
-                            logger.error(
-                                f"Error while converting {env_val} to str: {e}"
-                            )
                     except Exception as e:
                         logger.error(f"Error while getting {env_name}: {e}")
-                else:
-                    container_environment.append(env)
+                        env_value = None
+
+                try:
+                    env_val_str = str(env_value)
+                    container_environment.append(
+                        {"name": env_name, "value": env_val_str}
+                    )
+                except Exception as e:
+                    logger.error(f"Error while converting {env_value} to str: {e}")
+
         if self.env_from_secrets is not None:
-            secrets: Dict[str, Any] = read_secrets(self.env_from_secrets)
+            secrets: Dict[str, Any] = read_secrets(
+                self.env_from_secrets, aws_client=aws_client
+            )
             for secret_name, secret_value in secrets.items():
-                container_environment.append(
-                    {"name": secret_name, "value": secret_value}
-                )
+                try:
+                    secret_value = str(secret_value)
+                    container_environment.append(
+                        {"name": secret_name, "value": secret_value}
+                    )
+                except Exception as e:
+                    logger.error(f"Error while converting {secret_value} to str: {e}")
         return container_environment
 
     def container_definition_up_to_date(
         self, container_definition: Dict[str, Any]
     ) -> bool:
         """This is not working"""
```

### Comparing `phidata-1.7.5/phidata/aws/resource/ecs/service.py` & `phidata-1.7.6/phidata/aws/resource/ecs/service.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/aws/resource/ecs/task_definition.py` & `phidata-1.7.6/phidata/aws/resource/ecs/task_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/aws/resource/ecs/volume.py` & `phidata-1.7.6/phidata/aws/resource/ecs/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/aws/resource/eks/addon.py` & `phidata-1.7.6/phidata/aws/resource/eks/addon.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/aws/resource/eks/cluster.py` & `phidata-1.7.6/phidata/aws/resource/eks/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/aws/resource/eks/fargate_profile.py` & `phidata-1.7.6/phidata/aws/resource/eks/fargate_profile.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/aws/resource/eks/kubeconfig.py` & `phidata-1.7.6/phidata/aws/resource/eks/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/aws/resource/eks/node_group.py` & `phidata-1.7.6/phidata/aws/resource/eks/node_group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/aws/resource/elasticache/cluster.py` & `phidata-1.7.6/phidata/aws/resource/elasticache/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/aws/resource/elasticache/subnet_group.py` & `phidata-1.7.6/phidata/aws/resource/elasticache/subnet_group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/aws/resource/elb/listener.py` & `phidata-1.7.6/phidata/aws/resource/elb/listener.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/aws/resource/elb/load_balancer.py` & `phidata-1.7.6/phidata/aws/resource/elb/load_balancer.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/aws/resource/elb/target_group.py` & `phidata-1.7.6/phidata/aws/resource/elb/target_group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/aws/resource/emr/cluster.py` & `phidata-1.7.6/phidata/aws/resource/emr/cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/aws/resource/glue/crawler.py` & `phidata-1.7.6/phidata/aws/resource/glue/crawler.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/aws/resource/group.py` & `phidata-1.7.6/phidata/aws/resource/group.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 
 
 class AwsResourceGroup(BaseModel):
     """The AwsResourceGroup class contains the data for all AwsResources"""
 
     name: str = "default"
     enabled: bool = True
+    # Deprecated. DO NOT USE
     weight: int = 100
 
     subnets: Optional[List[Subnet]] = None
     iam_roles: Optional[List[IamRole]] = None
     iam_policies: Optional[List[IamPolicy]] = None
     acm_certificates: Optional[List[AcmCertificate]] = None
     secrets: Optional[List[SecretsManager]] = None
```

### Comparing `phidata-1.7.5/phidata/aws/resource/iam/group.py` & `phidata-1.7.6/phidata/aws/resource/iam/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/aws/resource/iam/policy.py` & `phidata-1.7.6/phidata/aws/resource/iam/policy.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/aws/resource/iam/role.py` & `phidata-1.7.6/phidata/aws/resource/iam/role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/aws/resource/rds/db_cluster.py` & `phidata-1.7.6/phidata/aws/resource/rds/db_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/aws/resource/rds/db_instance.py` & `phidata-1.7.6/phidata/aws/resource/rds/db_instance.py`

 * *Files 5% similar despite different names*

```diff
@@ -190,49 +190,55 @@
 
     # Cache secret_data
     cached_secret_data: Optional[Dict[str, Any]] = None
 
     def get_db_instance_identifier(self):
         return self.db_instance_identifier or self.name
 
-    def get_master_username(self) -> Optional[str]:
+    def get_master_username(
+        self, aws_client: Optional[AwsApiClient] = None
+    ) -> Optional[str]:
         master_username = self.master_username
         if master_username is None and self.secrets_file is not None:
             # read from secrets_file
             secret_data = self.get_secret_data()
             if secret_data is not None:
                 master_username = secret_data.get("MASTER_USERNAME", master_username)
         if master_username is None and self.aws_secret is not None:
             # read from aws_secret
             logger.debug(f"Reading MASTER_USERNAME from secret: {self.aws_secret.name}")
-            master_username = self.aws_secret.get_secret_value("MASTER_USERNAME")
+            master_username = self.aws_secret.get_secret_value(
+                "MASTER_USERNAME", aws_client=aws_client
+            )
 
         return master_username
 
-    def get_master_user_password(self) -> Optional[str]:
+    def get_master_user_password(
+        self, aws_client: Optional[AwsApiClient] = None
+    ) -> Optional[str]:
         master_user_password = self.master_user_password
         if master_user_password is None and self.secrets_file is not None:
             # read from secrets_file
             secret_data = self.get_secret_data()
             if secret_data is not None:
                 master_user_password = secret_data.get(
                     "MASTER_USER_PASSWORD", master_user_password
                 )
         if master_user_password is None and self.aws_secret is not None:
             # read from aws_secret
             logger.debug(
                 f"Reading MASTER_USER_PASSWORD from secret: {self.aws_secret.name}"
             )
             master_user_password = self.aws_secret.get_secret_value(
-                "MASTER_USER_PASSWORD"
+                "MASTER_USER_PASSWORD", aws_client=aws_client
             )
 
         return master_user_password
 
-    def get_db_name(self) -> Optional[str]:
+    def get_db_name(self, aws_client: Optional[AwsApiClient] = None) -> Optional[str]:
         db_name = self.db_name
         if db_name is None and self.secrets_file is not None:
             # read from secrets_file
             secret_data = self.get_secret_data()
             if secret_data is not None:
                 db_name = secret_data.get("DB_NAME", db_name)
                 if db_name is None:
@@ -241,15 +247,17 @@
             # read from aws_secret
             logger.debug(f"Reading DB_NAME from secret: {self.aws_secret.name}")
             db_name = self.aws_secret.get_secret_value("DB_NAME")
             if db_name is None:
                 logger.debug(
                     f"Reading DATABASE_NAME from secret: {self.aws_secret.name}"
                 )
-                db_name = self.aws_secret.get_secret_value("DATABASE_NAME")
+                db_name = self.aws_secret.get_secret_value(
+                    "DATABASE_NAME", aws_client=aws_client
+                )
         return db_name
 
     def get_database_name(self) -> Optional[str]:
         # Alias for get_db_name because db_instances use `db_name` and db_clusters use `database_name`
         return self.get_db_name()
 
     def _create(self, aws_client: AwsApiClient) -> bool:
@@ -712,38 +720,42 @@
         self, aws_client: Optional[AwsApiClient] = None
     ) -> Optional[str]:
         """Returns the DbInstance endpoint
 
         Returns:
             The DbInstance endpoint
         """
+        logger.debug(f"Getting endpoint for {self.get_resource_name()}")
         _db_endpoint: Optional[str] = None
         if self.active_resource:
             _db_endpoint = self.active_resource.get("Endpoint", {}).get("Address", None)
         if _db_endpoint is None:
             resource = self.read_resource_from_file()
             if resource is not None:
                 _db_endpoint = resource.get("Endpoint", {}).get("Address", None)
         if _db_endpoint is None:
             resource = self.read(aws_client)
             if resource is not None:
                 _db_endpoint = resource.get("Endpoint", {}).get("Address", None)
+        logger.debug(f"DBInstance endpoint: {_db_endpoint}")
         return _db_endpoint
 
     def get_db_port(self, aws_client: Optional[AwsApiClient] = None) -> Optional[str]:
         """Returns the DbInstance port
 
         Returns:
             The DbInstance endpoint
         """
+        logger.debug(f"Getting port for {self.get_resource_name()}")
         _db_port: Optional[str] = None
         if self.active_resource:
             _db_port = self.active_resource.get("Endpoint", {}).get("Port", None)
         if _db_port is None:
             resource = self.read_resource_from_file()
             if resource is not None:
                 _db_port = resource.get("Endpoint", {}).get("Port", None)
         if _db_port is None:
             resource = self.read(aws_client)
             if resource is not None:
                 _db_port = resource.get("Endpoint", {}).get("Port", None)
+        logger.debug(f"DBInstance port: {_db_port}")
         return _db_port
```

### Comparing `phidata-1.7.5/phidata/aws/resource/rds/db_subnet_group.py` & `phidata-1.7.6/phidata/aws/resource/rds/db_subnet_group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/aws/resource/s3/bucket.py` & `phidata-1.7.6/phidata/aws/resource/s3/bucket.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/aws/resource/secret/manager.py` & `phidata-1.7.6/phidata/aws/resource/secret/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -269,12 +269,14 @@
         except ClientError as ce:
             logger.debug(f"ClientError: {ce}")
         except Exception as e:
             print_error(f"Error reading {self.get_resource_type()}.")
             print_error(e)
         return None
 
-    def get_secret_value(self, secret_name: str) -> Optional[Any]:
-        secret_dict = self.get_secrets_as_dict()
+    def get_secret_value(
+        self, secret_name: str, aws_client: Optional[AwsApiClient] = None
+    ) -> Optional[Any]:
+        secret_dict = self.get_secrets_as_dict(aws_client=aws_client)
         if secret_dict is not None:
             return secret_dict.get(secret_name, None)
         return None
```

### Comparing `phidata-1.7.5/phidata/aws/resource/types.py` & `phidata-1.7.6/phidata/aws/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/aws/resource/utils.py` & `phidata-1.7.6/phidata/k8s/resource/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,96 +1,79 @@
-from typing import List, Optional, Dict, Tuple, Set
+from typing import Dict, List, Optional, Type, Tuple, Set
 
 from typing_extensions import Literal
 
-from phidata.aws.resource.base import AwsResource
-from phidata.aws.resource.group import AwsResourceGroup
-from phidata.aws.resource.types import AwsResourceInstallOrder
+from phidata.k8s.resource.base import K8sResource
+from phidata.k8s.resource.group import K8sResourceGroup
+from phidata.k8s.resource.types import K8sResourceInstallOrder
 from phidata.utils.log import logger
 
 
-def get_install_weight_for_aws_resource(
-    aws_resource_type: AwsResource, resource_group_weight: int = 100
-) -> int:
-    """Function which returns the install weight for an AwsResource"""
-
-    resource_type_class_name = aws_resource_type.__class__.__name__
-    if resource_type_class_name in AwsResourceInstallOrder.keys():
-        install_weight = AwsResourceInstallOrder[resource_type_class_name]
-        final_weight = resource_group_weight * install_weight
-        # logger.debug(
-        #     "Resource type: {} | Install weight: {}".format(
-        #         resource_type_class_name,
-        #         install_weight,
-        #     )
-        # )
-        return final_weight
-
-    return 5000
-
-
-def get_aws_resources_from_group(
-    aws_resource_group: AwsResourceGroup,
+def get_k8s_resources_from_group(
+    k8s_resource_group: K8sResourceGroup,
     name_filter: Optional[str] = None,
     type_filter: Optional[str] = None,
-) -> List[AwsResource]:
-    """Parses the AwsResourceGroup and returns an array of AwsResources
+    sort_order: Literal["create", "delete"] = "create",
+) -> List[K8sResource]:
+    """Parses the K8sResourceGroup and returns an array of K8sResources
     after applying the name & type filters. This function also flattens any
-    List[AwsResource] attributes. Eg: it will flatten s3_buckets
+    List[K8sResource] attributes. Eg: it will flatten pvc, cm, secret and
+    storage_class resources.
 
     Args:
-        aws_resource_group:
-        name_filter: filter AwsResources by name
-        type_filter: filter AwsResources by type
+        k8s_resource_group:
+        name_filter: filter K8sResources by name
+        type_filter: filter K8sResources by type
+        sort_order: create or delete
 
     Returns:
-        List[AwsResource]: List of filtered and flattened Aws Resources
+        List[K8sResource]: List of filtered and flattened K8s Resources
     """
 
     # List of resources to return
-    aws_resources: List[AwsResource] = []
-    # logger.debug(f"Flattening {aws_resource_group.name}")
+    k8s_resources: List[K8sResource] = []
+    # logger.debug(f"Flattening {k8s_resource_group.name}")
 
-    # populate the aws_resources list with the resources
-    # Loop over each key of the AwsResourceGroup model
-    for resource, resource_data in aws_resource_group.__dict__.items():
+    # populate the k8s_resources list with the resources
+    # Loop over each key of the K8sResourceGroup model
+    for resource, resource_data in k8s_resource_group.__dict__.items():
         # logger.debug("resource: {}".format(resource))
         # logger.debug("resource_data: {}".format(resource_data))
 
-        # Check if the resource is a single AwsResource or a List[AwsResource]
-        # If it is a List[AwsResource], flatten the resources, verify each element
-        # of the list is a subclass of AwsResource and add to the aws_resources list
+        # Check if the resource is a single K8sResource or a List[K8sResource]
+        # If it is a List[K8sResource], flatten the resources, verify each element
+        # of the list is a subclass of K8sResource and add to the k8s_resources list
         if isinstance(resource_data, list):
             for _r in resource_data:
-                if isinstance(_r, AwsResource):
+                if isinstance(_r, K8sResource):
                     rn = _r.get_resource_name()
                     rt = _r.get_resource_type()
                     # skip disabled resources
                     if not _r.enabled:
                         logger.debug(f"  -*- skipping {rt}:{rn}")
                         continue
 
                     if name_filter is not None and rn is not None:
-                        # logger.debug(f"name_filter: {name_filter.lower()}")
+                        logger.debug(f"name_filter: {name_filter.lower()}")
                         # logger.debug(f"resource name: {rn.lower()}")
                         if name_filter.lower() not in rn.lower():
                             logger.debug(f"  -*- skipping {rt}:{rn}")
                             continue
 
                     if type_filter is not None and rt is not None:
-                        # logger.debug(f"type_filter: {type_filter.lower()}")
+                        logger.debug(f"type_filter: {type_filter.lower()}")
                         # logger.debug(f"class: {rt.lower()}")
                         if type_filter.lower() != rt.lower():
                             logger.debug(f"  -*- skipping {rt}:{rn}")
                             continue
-                    aws_resources.append(_r)  # type: ignore
+                    k8s_resources.append(_r)  # type: ignore
 
         # If its a single resource, verify that the resource is a subclass of
-        # AwsResource and add it to the aws_resources list
-        elif isinstance(resource_data, AwsResource):
+        # K8sResource and add it to the k8s_resources list
+        elif isinstance(resource_data, K8sResource):
             rn = resource_data.get_resource_name()
             rt = resource_data.get_resource_type()
             # skip disabled resources
             if not resource_data.enabled:
                 logger.debug(f"  -*- skipping {rt}:{rn}")
                 continue
 
@@ -103,187 +86,143 @@
 
             if type_filter is not None and rt is not None:
                 # logger.debug(f"type_filter: {type_filter.lower()}")
                 # logger.debug(f"class: {rt.lower()}")
                 if type_filter.lower() != rt.lower():
                     # logger.debug(f"skipping {rt}:{rn}")
                     continue
-            aws_resources.append(resource_data)  # type: ignore
+            k8s_resources.append(resource_data)  # type: ignore
 
-    return aws_resources
+    return k8s_resources
 
 
-# def dedup_resource_types(
-#     aws_resources: Optional[List[AwsResource]] = None,
-# ) -> Optional[Set[Type[AwsResource]]]:
-#     """Takes a list of AwsResources and returns a Set of AwsResource classes.
-#     Each AwsResource classes is represented by the Type[resources.AwsResource] type.
-#     From python docs:
-#         A variable annotated with Type[AwsResource] may accept values that are classes.
-#         Acceptable classes are the AwsResource class + subclasses.
-#     """
-#     if aws_resources:
-#         active_resource_types: Set[Type[AwsResource]] = set()
-#         for resource in aws_resources:
-#             active_resource_types.add(resource.__class__)
-#             # logger.debug(f"Gathering: {resource.get_resource_name()}")
-#             # logger.debug(f"Resource Type: {resource_type}")
-#         logger.debug("Active Resource Types: {}".format(active_resource_types))
-#         return active_resource_types
-#     return None
-
-
-def dedup_aws_resources(
-    aws_resources_with_weight: List[Tuple[AwsResource, int]],
-) -> List[Tuple[AwsResource, int]]:
-    if aws_resources_with_weight is None:
-        raise ValueError
-
-    deduped_resources: List[Tuple[AwsResource, int]] = []
-    prev_rsrc: Optional[AwsResource] = None
-    prev_weight: Optional[int] = None
-    for rsrc, weight in aws_resources_with_weight:
-        # First item of loop
-        if prev_rsrc is None:
-            prev_rsrc = rsrc
-            prev_weight = weight
-            deduped_resources.append((rsrc, weight))
-            continue
-
-        # Compare resources with same weight only
-        if weight == prev_weight:
-            if (
-                rsrc.get_resource_type() == prev_rsrc.get_resource_type()
-                and rsrc.get_resource_name() == prev_rsrc.get_resource_name()
-                and rsrc.get_resource_name() is not None
-            ):
-                # If resource type and name are the same, skip the resource
-                # Note: resource.name cannot be None
-                continue
+def get_rank_for_k8s_resource(k8s_resource_type: K8sResource) -> int:
+    """Function which returns the install rank for a K8sResource"""
+
+    resource_type_class_name = k8s_resource_type.__class__.__name__
+    if resource_type_class_name in K8sResourceInstallOrder.keys():
+        install_rank = K8sResourceInstallOrder[resource_type_class_name]
+        return install_rank
+
+    return 5000
+
 
-        # If the loop hasn't been continued by the if blocks above,
-        # add the resource and weight to the deduped_resources list
-        deduped_resources.append((rsrc, weight))
-        # update the previous resource for comparison
-        prev_rsrc = rsrc
-        prev_weight = weight
+def dedup_k8s_resources(k8s_resource_list: List[K8sResource]) -> List[K8sResource]:
+    deduped_resources: List[K8sResource] = []
+    for rsrc in k8s_resource_list:
+        if rsrc not in deduped_resources:
+            deduped_resources.append(rsrc)
     return deduped_resources
 
 
-def filter_and_flatten_aws_resource_groups(
-    aws_resource_groups: Dict[str, AwsResourceGroup],
+def filter_and_flatten_k8s_resource_groups(
+    k8s_resource_groups: Dict[str, K8sResourceGroup],
     name_filter: Optional[str] = None,
     type_filter: Optional[str] = None,
     app_filter: Optional[str] = None,
     sort_order: Literal["create", "delete"] = "create",
-) -> List[AwsResource]:
-    """This function flattens the aws_resource_group and returns a filtered list of
-    AwsResources sorted in the order requested. create == install order, delete == reverse
+) -> Optional[List[K8sResource]]:
+    """This function parses the k8s_resource_groups dict and returns a filtered array of
+    K8sResources sorted in the order requested. create == install order, delete == reverse
+    Desc:
+        1. Iterate through each K8sResourceGroup
+        2. If enabled, get the K8s Resources from that group which match the filters
+        2. Return a list of all K8sResources from 2.
 
     Args:
-        aws_resource_groups: AwsResourceGroup
-        name_filter: Filter AwsResources by name
-        type_filter: Filter AwsResources by type
-        app_filter: Filter AwsResources by aws resource group name
+        k8s_resource_groups: Dict[str, resources.K8sResourceGroup]
+            Dict of {resource_group_name : K8sResourceGroup}
+        name_filter: Filter K8sResourceGroup by name
+        type_filter: Filter K8sResourceGroup by type
+        app_filter: Filter K8sResourceGroup by app
         sort_order: create or delete
 
     Returns:
-        List[AwsResource]: List of filtered Aws Resources
+        List[K8sResource]: List of filtered K8s Resources
     """
 
-    logger.debug("Filtering & Flattening AwsResourceGroups")
+    logger.debug("Filtering & Flattening K8sResourceGroups")
 
-    # Step 1: Create aws_resource_list_with_weight
-    # A List of Tuples where each tuple is a (AwsResource, Resource Group Weight)
-    # The reason for creating this list is so that we can sort the AwsResources
-    # based on their resource group weight using get_install_weight_for_aws_resource
-    aws_resource_list_with_weight: List[Tuple[AwsResource, int]] = []
-    if aws_resource_groups:
-        # Iterate through aws_resource_groups
-        for aws_rg_name, aws_rg in aws_resource_groups.items():
-            # logger.debug("aws_rg_name: {}".format(aws_rg_name))
-            # logger.debug("aws_rg: {}".format(aws_rg))
+    # Step 1: Create a list of k8s_resources
+    k8s_resource_list: List[K8sResource] = []
+    if k8s_resource_groups:
+        # Iterate through k8s_resource_groups
+        for k8s_rg_name, k8s_rg in k8s_resource_groups.items():
+            # logger.debug("k8s_rg_name: {}".format(k8s_rg_name))
+            # logger.debug("k8s_rg: {}".format(k8s_rg))
 
-            # skip disabled AwsResourceGroups
-            if not aws_rg.enabled:
+            # skip disabled K8sResourceGroups
+            if not k8s_rg.enabled:
                 continue
 
             # skip groups not matching app_filter if provided
-            if app_filter is not None and aws_rg_name is not None:
+            if app_filter is not None and k8s_rg_name is not None:
                 # logger.debug(f"matching app_filter: {app_filter}")
-                # logger.debug(f"with aws_rg_name: {aws_rg_name}")
-                if app_filter.lower() not in aws_rg_name.lower():
-                    logger.debug(f"  -*- skipping {aws_rg_name}")
+                # logger.debug(f"with k8s_rg_name: {k8s_rg_name}")
+                if app_filter.lower() not in k8s_rg_name.lower():
+                    logger.debug(f"  -*- skipping {k8s_rg_name}")
                     continue
 
-            aws_resources = get_aws_resources_from_group(
-                aws_rg, name_filter, type_filter
+            _k8s_resources = get_k8s_resources_from_group(
+                k8s_rg, name_filter, type_filter
             )
-            if aws_resources:
-                for _aws_rsrc in aws_resources:
-                    aws_resource_list_with_weight.append((_aws_rsrc, aws_rg.weight))
+            if _k8s_resources:
+                k8s_resource_list.extend(_k8s_resources)
 
     # Sort the resources in install order
     if sort_order == "create":
-        aws_resource_list_with_weight.sort(
-            key=lambda x: (get_install_weight_for_aws_resource(x[0], x[1]), x[0].name)
-        )
+        k8s_resource_list.sort(key=lambda x: get_rank_for_k8s_resource(x))
     elif sort_order == "delete":
-        aws_resource_list_with_weight.sort(
-            key=lambda x: (get_install_weight_for_aws_resource(x[0], x[1]), x[0].name),
-            reverse=True,
-        )
-
-    # De-duplicate AwsResources
-    deduped_aws_resources: List[Tuple[AwsResource, int]] = dedup_aws_resources(
-        aws_resource_list_with_weight
-    )
+        k8s_resource_list.sort(key=lambda x: get_rank_for_k8s_resource(x), reverse=True)
+
+    # De-duplicate K8sResources
+    deduped_k8s_resources: List[K8sResource] = dedup_k8s_resources(k8s_resource_list)
 
     # Implement dependency sorting and drop the weight
-    final_aws_resources: List[AwsResource] = []
-    for aws_resource, weight in deduped_aws_resources:
+    final_k8s_resources: List[K8sResource] = []
+    for k8s_resource in deduped_k8s_resources:
         # Logic to follow if resource has dependencies
-        if aws_resource.depends_on is not None:
+        if k8s_resource.depends_on is not None:
             # If the sort_order is delete
             # 1. Reverse the order of dependencies
-            # 2. Remove the dependencies if they are already added to the final_aws_resources
+            # 2. Remove the dependencies if they are already added to the final_k8s_resources
             # 3. Add the resource to be deleted before its dependencies
             # 4. Add the dependencies back in reverse order
             if sort_order == "delete":
                 # 1. Reverse the order of dependencies
-                aws_resource.depends_on.reverse()
-                # 2. Remove the dependencies if they are already added to the final_aws_resources
-                for dep in aws_resource.depends_on:
-                    if dep in final_aws_resources:
+                k8s_resource.depends_on.reverse()
+                # 2. Remove the dependencies if they are already added to the final_k8s_resources
+                for dep in k8s_resource.depends_on:
+                    if dep in final_k8s_resources:
                         logger.debug(
-                            f"  -*- Removing {dep.name}, dependency of {aws_resource.name}"
+                            f"  -*- Removing {dep.name}, dependency of {k8s_resource.name}"
                         )
-                        final_aws_resources.remove(dep)
+                        final_k8s_resources.remove(dep)
                 # 3. Add the resource to be deleted before its dependencies
-                if aws_resource not in final_aws_resources:
-                    logger.debug(f"  -*- Adding {aws_resource.name}")
-                    final_aws_resources.append(aws_resource)
+                if k8s_resource not in final_k8s_resources:
+                    logger.debug(f"  -*- Adding {k8s_resource.name}")
+                    final_k8s_resources.append(k8s_resource)
 
             # Common logic for create and delete
             # When the sort_order is create, the dependencies are added before the resource
             # When the sort_order is delete, the dependencies are added after the resource
-            for dep in aws_resource.depends_on:
-                if isinstance(dep, AwsResource):
-                    if dep not in final_aws_resources:
+            for dep in k8s_resource.depends_on:
+                if isinstance(dep, K8sResource):
+                    if dep not in final_k8s_resources:
                         logger.debug(
-                            f"  -*- Adding {dep.name}, dependency of {aws_resource.name}"
+                            f"  -*- Adding {dep.name}, dependency of {k8s_resource.name}"
                         )
-                        final_aws_resources.append(dep)
+                        final_k8s_resources.append(dep)
 
             # If the sort_order is create,
             # add the resource to be created after its dependencies
             if sort_order == "create":
-                if aws_resource not in final_aws_resources:
-                    logger.debug(f"  -*- Adding {aws_resource.name}")
-                    final_aws_resources.append(aws_resource)
+                if k8s_resource not in final_k8s_resources:
+                    logger.debug(f"  -*- Adding {k8s_resource.name}")
+                    final_k8s_resources.append(k8s_resource)
         else:
             # Add the resource to be created/deleted
-            if aws_resource not in final_aws_resources:
-                logger.debug(f"  -*- Adding {aws_resource.name}")
-                final_aws_resources.append(aws_resource)
+            if k8s_resource not in final_k8s_resources:
+                logger.debug(f"  -*- Adding {k8s_resource.name}")
+                final_k8s_resources.append(k8s_resource)
 
-    return final_aws_resources
+    return final_k8s_resources
```

### Comparing `phidata-1.7.5/phidata/aws/s3/csv_dataset.py` & `phidata-1.7.6/phidata/aws/s3/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/aws/s3/dataset.py` & `phidata-1.7.6/phidata/aws/s3/dataset.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/aws/s3/dataset_base.py` & `phidata-1.7.6/phidata/aws/s3/dataset_base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/aws/s3/object.py` & `phidata-1.7.6/phidata/aws/s3/object.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/aws/worker.py` & `phidata-1.7.6/phidata/aws/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/base.py` & `phidata-1.7.6/phidata/base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/checks/check.py` & `phidata-1.7.6/phidata/checks/check.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/checks/not_empty.py` & `phidata-1.7.6/phidata/checks/not_empty.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/constants.py` & `phidata-1.7.6/phidata/constants.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/decorators/timer.py` & `phidata-1.7.6/phidata/decorators/timer.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/decorators/validate_env.py` & `phidata-1.7.6/phidata/decorators/validate_env.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/docker/api_client.py` & `phidata-1.7.6/phidata/docker/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/docker/args.py` & `phidata-1.7.6/phidata/docker/args.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/docker/config.py` & `phidata-1.7.6/phidata/docker/config.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/docker/enums.py` & `phidata-1.7.6/phidata/docker/enums.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/docker/manager.py` & `phidata-1.7.6/phidata/docker/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/docker/resource/base.py` & `phidata-1.7.6/phidata/docker/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/docker/resource/container.py` & `phidata-1.7.6/phidata/docker/resource/container.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/docker/resource/image.py` & `phidata-1.7.6/phidata/docker/resource/image.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/docker/resource/network.py` & `phidata-1.7.6/phidata/docker/resource/network.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/docker/resource/types.py` & `phidata-1.7.6/phidata/docker/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/docker/resource/utils.py` & `phidata-1.7.6/phidata/docker/resource/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,51 +4,14 @@
 
 from phidata.docker.resource.base import DockerResource
 from phidata.docker.resource.group import DockerResourceGroup
 from phidata.docker.resource.types import DockerResourceInstallOrder
 from phidata.utils.log import logger
 
 
-def get_install_weight_for_docker_resource(
-    docker_resource_type: DockerResource, resource_group_weight: int = 100
-) -> int:
-    """Function which takes a DockerResource and resource_group_weight and returns the install
-    weight for that resource.
-
-    Understanding install weights for DockerResources:
-
-    - Each DockerResource gets an install weight, which determines the order for installing that particular resource.
-    - By default, DockerResources are installed in the order determined by the DockerResourceInstallOrder dict.
-        The DockerResourceInstallOrder dict ensures volumes are created before containers
-    - We can also provide a weight to the DockerResourceGroup, that weight determines the install order for resources of
-        that resource group as compared to other resource groups.
-    - We achieve this by multiplying the DockerResourceGroup.weight with the value from DockerResourceInstallOrder
-        and by default using a weight of 100. So
-        * Weights 1-10 are reserved
-        * Choose weight 11-99 to deploy a resource group before all the "default" resources
-        * Choose weight 101+ to deploy a resource group after all the "default" resources
-        * Choosing weight 100 has no effect because that is the default install weight
-    """
-    resource_type_class_name = docker_resource_type.__class__.__name__
-    if resource_type_class_name in DockerResourceInstallOrder.keys():
-        install_weight = DockerResourceInstallOrder[resource_type_class_name]
-        final_weight = resource_group_weight * install_weight
-        # logger.debug(
-        #     "Resource type: {} | RG Weight: {} | Install weight: {} | Final weight: {}".format(
-        #         resource_type_class_name,
-        #         resource_group_weight,
-        #         install_weight,
-        #         final_weight,
-        #     )
-        # )
-        return final_weight
-
-    return 5000
-
-
 def get_docker_resources_from_group(
     docker_resource_group: DockerResourceGroup,
     name_filter: Optional[str] = None,
     type_filter: Optional[str] = None,
 ) -> List[DockerResource]:
     """Parses the DockerResourceGroup and returns an array of DockerResources
     after applying the name & type filters. This function also flattens any
@@ -131,48 +94,32 @@
                     # logger.debug(f"skipping {rt}:{rn}")
                     continue
             docker_resources.append(resource_data)  # type: ignore
 
     return docker_resources
 
 
-def dedup_docker_resources(
-    docker_resources_with_weight: List[Tuple[DockerResource, int]],
-) -> List[Tuple[DockerResource, int]]:
-    if docker_resources_with_weight is None:
-        raise ValueError
-
-    deduped_resources: List[Tuple[DockerResource, int]] = []
-    prev_rsrc: Optional[DockerResource] = None
-    prev_weight: Optional[int] = None
-    for rsrc, weight in docker_resources_with_weight:
-        # First item of loop
-        if prev_rsrc is None:
-            prev_rsrc = rsrc
-            prev_weight = weight
-            deduped_resources.append((rsrc, weight))
-            continue
-
-        # Compare resources with same weight only
-        if weight == prev_weight:
-            if (
-                rsrc.get_resource_type() == prev_rsrc.get_resource_type()
-                and rsrc.get_resource_name() == prev_rsrc.get_resource_name()
-                and rsrc.get_resource_name() is not None
-            ):
-                # If resource type and name are the same, skip the resource
-                # Note: resource.name cannot be None
-                continue
+def get_rank_for_docker_resource(docker_resource_type: DockerResource) -> int:
+    """Function which returns the install rank for a DockerResource"""
 
-        # If the loop hasn't been continued by the if blocks above,
-        # add the resource and weight to the deduped_resources list
-        deduped_resources.append((rsrc, weight))
-        # update the previous resource for comparison
-        prev_rsrc = rsrc
-        prev_weight = weight
+    resource_type_class_name = docker_resource_type.__class__.__name__
+    if resource_type_class_name in DockerResourceInstallOrder.keys():
+        install_rank = DockerResourceInstallOrder[resource_type_class_name]
+        return install_rank
+
+    return 5000
+
+
+def dedup_docker_resources(
+    docker_resource_list: List[DockerResource],
+) -> List[DockerResource]:
+    deduped_resources: List[DockerResource] = []
+    for rsrc in docker_resource_list:
+        if rsrc not in deduped_resources:
+            deduped_resources.append(rsrc)
     return deduped_resources
 
 
 def filter_and_flatten_docker_resource_groups(
     docker_resource_groups: Dict[str, DockerResourceGroup],
     name_filter: Optional[str] = None,
     type_filter: Optional[str] = None,
@@ -195,72 +142,56 @@
         sort_order: create or delete
 
     Returns:
         List[DockerResource]: List of filtered DockerResources
     """
 
     logger.debug("Filtering & Flattening DockerResourceGroups")
-    # Step 1: Create docker_resource_list_with_weight
-    # A List of Tuples where each tuple is a (DockerResource, Resource Group Weight)
-    # This list helps us sort the DockerResources
-    # based on their resource group weight using get_install_weight_for_docker_resource
-    docker_resource_list_with_weight: List[Tuple[DockerResource, int]] = []
+    # Step 1: Create a list of docker_resources
+    docker_resource_list: List[DockerResource] = []
     if docker_resource_groups:
         # Iterate through docker_resource_groups
         for docker_rg_name, docker_rg in docker_resource_groups.items():
-            # logger.debug("docker_rg: {}".format(docker_rg))
             # logger.debug("docker_rg_name: {}".format(docker_rg_name))
-            # logger.debug("docker_rg_type: {}".format(type(docker_rg)))
+            # logger.debug("docker_rg: {}".format(docker_rg))
 
             # skip disabled DockerResourceGroups
             if not docker_rg.enabled:
                 continue
 
             # skip groups not matching app_filter if provided
             if app_filter is not None and docker_rg_name is not None:
                 # logger.debug(f"matching app_filter: {app_filter}")
                 # logger.debug(f"with docker_rg_name: {docker_rg_name}")
                 if app_filter.lower() not in docker_rg_name.lower():
                     logger.debug(f"  -*- skipping {docker_rg_name}")
                     continue
 
-            docker_resources = get_docker_resources_from_group(
+            _docker_resources = get_docker_resources_from_group(
                 docker_rg, name_filter, type_filter
             )
-            if docker_resources:
-                for _docker_rsrc in docker_resources:
-                    docker_resource_list_with_weight.append(
-                        (_docker_rsrc, docker_rg.weight)
-                    )
+            if _docker_resources:
+                docker_resource_list.extend(_docker_resources)
 
     # Sort the resources in install order
     if sort_order == "create":
-        docker_resource_list_with_weight.sort(
-            key=lambda x: (
-                get_install_weight_for_docker_resource(x[0], x[1]),
-                x[0].name,
-            )
-        )
+        docker_resource_list.sort(key=lambda x: get_rank_for_docker_resource(x))
     elif sort_order == "delete":
-        docker_resource_list_with_weight.sort(
-            key=lambda x: (
-                get_install_weight_for_docker_resource(x[0], x[1]),
-                x[0].name,
-            ),
-            reverse=True,
+        docker_resource_list.sort(
+            key=lambda x: get_rank_for_docker_resource(x), reverse=True
         )
 
     # De-duplicate DockerResources
-    deduped_docker_resources: List[Tuple[DockerResource, int]] = dedup_docker_resources(
-        docker_resource_list_with_weight
+    deduped_docker_resources: List[DockerResource] = dedup_docker_resources(
+        docker_resource_list
     )
 
     # Implement dependency sorting and drop the weight
     final_docker_resources: List[DockerResource] = []
-    for docker_resource, weight in deduped_docker_resources:
+    for docker_resource in deduped_docker_resources:
         # Logic to follow if resource has dependencies
         if docker_resource.depends_on is not None:
             # If the sort_order is delete
             # 1. Reverse the order of dependencies
             # 2. Remove the dependencies if they are already added to the final_docker_resources
             # 3. Add the resource to be deleted before its dependencies
             # 4. Add the dependencies back in reverse order
```

### Comparing `phidata-1.7.5/phidata/docker/resource/volume.py` & `phidata-1.7.6/phidata/docker/resource/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/docker/utils/container.py` & `phidata-1.7.6/phidata/docker/utils/container.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/docker/worker.py` & `phidata-1.7.6/phidata/docker/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/infra/args.py` & `phidata-1.7.6/phidata/infra/args.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/infra/config.py` & `phidata-1.7.6/phidata/infra/config.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/infra/resource.py` & `phidata-1.7.6/phidata/infra/resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -309,10 +309,11 @@
             self.env_data = self.read_yaml_file(self.env_file)
         return self.env_data
 
     def __hash__(self):
         return hash(self.name)
 
     def __eq__(self, other):
-        if other.resource_type == self.resource_type:
-            return self.name == other.name
+        if isinstance(other, InfraResource):
+            if other.get_resource_type() == self.get_resource_type():
+                return self.get_resource_name() == other.get_resource_name()
         return False
```

### Comparing `phidata-1.7.5/phidata/k8s/api_client.py` & `phidata-1.7.6/phidata/k8s/api_client.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/args.py` & `phidata-1.7.6/phidata/k8s/args.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/config.py` & `phidata-1.7.6/phidata/k8s/config.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py` & `phidata-1.7.6/phidata/k8s/create/apiextensions_k8s_io/v1/custom_object.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py` & `phidata-1.7.6/phidata/k8s/create/apiextensions_k8s_io/v1/custom_resource_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/create/apps/v1/deployment.py` & `phidata-1.7.6/phidata/k8s/create/apps/v1/deployment.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/create/common/port.py` & `phidata-1.7.6/phidata/k8s/create/common/port.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/create/core/v1/config_map.py` & `phidata-1.7.6/phidata/k8s/create/core/v1/config_map.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/create/core/v1/container.py` & `phidata-1.7.6/phidata/k8s/create/core/v1/container.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/create/core/v1/namespace.py` & `phidata-1.7.6/phidata/k8s/create/core/v1/namespace.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/create/core/v1/persistent_volume.py` & `phidata-1.7.6/phidata/k8s/create/core/v1/persistent_volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/create/core/v1/persistent_volume_claim.py` & `phidata-1.7.6/phidata/k8s/create/core/v1/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/create/core/v1/secret.py` & `phidata-1.7.6/phidata/k8s/create/core/v1/secret.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/create/core/v1/service.py` & `phidata-1.7.6/phidata/k8s/create/core/v1/service.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/create/core/v1/service_account.py` & `phidata-1.7.6/phidata/k8s/create/core/v1/service_account.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/create/core/v1/volume.py` & `phidata-1.7.6/phidata/k8s/create/core/v1/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/create/crb/eks_admin_crb.py` & `phidata-1.7.6/phidata/k8s/create/crb/eks_admin_crb.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/create/group.py` & `phidata-1.7.6/phidata/k8s/create/group.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/create/kubeconfig.py` & `phidata-1.7.6/phidata/k8s/create/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/create/networking_k8s_io/v1/ingress.py` & `phidata-1.7.6/phidata/k8s/create/networking_k8s_io/v1/ingress.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py` & `phidata-1.7.6/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluste_role_binding.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py` & `phidata-1.7.6/phidata/k8s/create/rbac_authorization_k8s_io/v1/cluster_role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/create/storage_k8s_io/v1/storage_class.py` & `phidata-1.7.6/phidata/k8s/create/storage_k8s_io/v1/storage_class.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/enums/api_version.py` & `phidata-1.7.6/phidata/k8s/enums/api_version.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/enums/kind.py` & `phidata-1.7.6/phidata/k8s/enums/kind.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/enums/manager_status.py` & `phidata-1.7.6/phidata/k8s/enums/manager_status.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/enums/pv.py` & `phidata-1.7.6/phidata/k8s/enums/pv.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/manager.py` & `phidata-1.7.6/phidata/k8s/manager.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py` & `phidata-1.7.6/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_object.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py` & `phidata-1.7.6/phidata/k8s/resource/apiextensions_k8s_io/v1/custom_resource_definition.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/resource/apps/v1/deployment.py` & `phidata-1.7.6/phidata/k8s/resource/apps/v1/deployment.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/resource/apps/v1/deployment_strategy.py` & `phidata-1.7.6/phidata/k8s/resource/apps/v1/deployment_strategy.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/resource/base.py` & `phidata-1.7.6/phidata/k8s/resource/base.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/resource/core/v1/config_map.py` & `phidata-1.7.6/phidata/k8s/resource/core/v1/config_map.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/resource/core/v1/container.py` & `phidata-1.7.6/phidata/k8s/resource/core/v1/container.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/resource/core/v1/local_object_reference.py` & `phidata-1.7.6/phidata/k8s/resource/core/v1/local_object_reference.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/resource/core/v1/namespace.py` & `phidata-1.7.6/phidata/k8s/resource/core/v1/namespace.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/resource/core/v1/node_selector.py` & `phidata-1.7.6/phidata/k8s/resource/core/v1/node_selector.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/resource/core/v1/object_reference.py` & `phidata-1.7.6/phidata/k8s/resource/core/v1/object_reference.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/resource/core/v1/persistent_volume.py` & `phidata-1.7.6/phidata/k8s/resource/core/v1/persistent_volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/resource/core/v1/persistent_volume_claim.py` & `phidata-1.7.6/phidata/k8s/resource/core/v1/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/resource/core/v1/pod.py` & `phidata-1.7.6/phidata/k8s/resource/core/v1/pod.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/resource/core/v1/pod_spec.py` & `phidata-1.7.6/phidata/k8s/resource/core/v1/pod_spec.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/resource/core/v1/pod_template_spec.py` & `phidata-1.7.6/phidata/k8s/resource/core/v1/pod_template_spec.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/resource/core/v1/resource_requirements.py` & `phidata-1.7.6/phidata/k8s/resource/core/v1/resource_requirements.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/resource/core/v1/secret.py` & `phidata-1.7.6/phidata/k8s/resource/core/v1/secret.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/resource/core/v1/service.py` & `phidata-1.7.6/phidata/k8s/resource/core/v1/service.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/resource/core/v1/service_account.py` & `phidata-1.7.6/phidata/k8s/resource/core/v1/service_account.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/resource/core/v1/toleration.py` & `phidata-1.7.6/phidata/k8s/resource/core/v1/toleration.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/resource/core/v1/topology_spread_constraints.py` & `phidata-1.7.6/phidata/k8s/resource/core/v1/topology_spread_constraints.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/resource/core/v1/volume.py` & `phidata-1.7.6/phidata/k8s/resource/core/v1/volume.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/resource/core/v1/volume_node_affinity.py` & `phidata-1.7.6/phidata/k8s/resource/core/v1/volume_node_affinity.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/resource/core/v1/volume_source.py` & `phidata-1.7.6/phidata/k8s/resource/core/v1/volume_source.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/resource/group.py` & `phidata-1.7.6/phidata/k8s/resource/group.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,27 +37,15 @@
     but for complex Apps, 1 PhidataApp may produce > 1 K8sResourceGroup
     """
 
     # Name of this group aka name of the app
     name: str
     enabled: bool = True
 
-    # The weight variable controls how this is group is deployed to a cluster
-    # relative to other resource groups.
-
-    # Within each resource group, different types of resources are
-    # deployed in a predefined order (eg: ns first, then sa and so on ...)
-    # but we can also add an order to how to deploy different resource groups.
-    # Eg: if we want to deploy a resource group with databases before other resources
-
-    # Weights 1-10 are reserved
-    # Weight 100 is default.
-    # ResourceGroups with weight 100 are the default resources.
-    # Choose weight 11-99 to deploy a resource group before all the default resources.
-    # Choose weight 101+ to deploy a resource group after all the default resources
+    # Deprecated. DO NOT USE
     weight: int = 100
 
     ns: Optional[List[Namespace]] = None
     sa: Optional[List[ServiceAccount]] = None
     cr: Optional[List[ClusterRole]] = None
     crb: Optional[List[ClusterRoleBinding]] = None
     secrets: Optional[List[Secret]] = None
```

### Comparing `phidata-1.7.5/phidata/k8s/resource/kubeconfig.py` & `phidata-1.7.6/phidata/k8s/resource/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/resource/meta/v1/label_selector.py` & `phidata-1.7.6/phidata/k8s/resource/meta/v1/label_selector.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/resource/meta/v1/object_meta.py` & `phidata-1.7.6/phidata/k8s/resource/meta/v1/object_meta.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/resource/networking_k8s_io/v1/ingress.py` & `phidata-1.7.6/phidata/k8s/resource/networking_k8s_io/v1/ingress.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py` & `phidata-1.7.6/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluste_role_binding.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py` & `phidata-1.7.6/phidata/k8s/resource/rbac_authorization_k8s_io/v1/cluster_role.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py` & `phidata-1.7.6/phidata/k8s/resource/storage_k8s_io/v1/storage_class.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/resource/types.py` & `phidata-1.7.6/phidata/k8s/resource/types.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/utils/pod.py` & `phidata-1.7.6/phidata/k8s/utils/pod.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/k8s/worker.py` & `phidata-1.7.6/phidata/k8s/worker.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/llm/duckdb/agent.py` & `phidata-1.7.6/phidata/llm/duckdb/agent.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/llm/duckdb/chain.py` & `phidata-1.7.6/phidata/llm/duckdb/chain.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/llm/duckdb/connection.py` & `phidata-1.7.6/phidata/llm/duckdb/connection.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/llm/duckdb/loader.py` & `phidata-1.7.6/phidata/llm/duckdb/loader.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/llm/duckdb/query.py` & `phidata-1.7.6/phidata/llm/duckdb/query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/llm/duckdb/tool.py` & `phidata-1.7.6/phidata/llm/duckdb/tool.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/product/data_product.py` & `phidata-1.7.6/phidata/product/data_product.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/table/local/csv.py` & `phidata-1.7.6/phidata/table/local/csv.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/table/local/local_table.py` & `phidata-1.7.6/phidata/table/local/local_table.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/table/local/parquet.py` & `phidata-1.7.6/phidata/table/local/parquet.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/table/s3/csv.py` & `phidata-1.7.6/phidata/table/s3/csv.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/table/s3/parquet.py` & `phidata-1.7.6/phidata/table/s3/parquet.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/table/s3/s3_table.py` & `phidata-1.7.6/phidata/table/s3/s3_table.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/table/sql/postgres.py` & `phidata-1.7.6/phidata/table/sql/postgres.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/table/sql/sql_table.py` & `phidata-1.7.6/phidata/table/sql/sql_table.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/task/aws/athena/run_query.py` & `phidata-1.7.6/phidata/task/aws/athena/run_query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/task/aws/emr/create_cluster.py` & `phidata-1.7.6/phidata/task/aws/emr/create_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/task/aws/emr/delete_cluster.py` & `phidata-1.7.6/phidata/task/aws/emr/delete_cluster.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/task/aws/glue/start_crawler.py` & `phidata-1.7.6/phidata/task/aws/glue/start_crawler.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/task/decorator.py` & `phidata-1.7.6/phidata/task/decorator.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/task/download/s3/to_file.py` & `phidata-1.7.6/phidata/task/download/s3/to_file.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/task/download/url/to_file.py` & `phidata-1.7.6/phidata/task/download/url/to_file.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/task/download/url/to_s3.py` & `phidata-1.7.6/phidata/task/download/url/to_s3.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/task/download/url/to_sql.py` & `phidata-1.7.6/phidata/task/download/url/to_sql.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/task/plot/sql/query.py` & `phidata-1.7.6/phidata/task/plot/sql/query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/task/python_task.py` & `phidata-1.7.6/phidata/task/python_task.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/task/run/sql/query.py` & `phidata-1.7.6/phidata/task/run/sql/query.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/task/task.py` & `phidata-1.7.6/phidata/task/task.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/task/task_relatives.py` & `phidata-1.7.6/phidata/task/task_relatives.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/task/upload/file/to_s3.py` & `phidata-1.7.6/phidata/task/upload/file/to_s3.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/task/upload/file/to_sql.py` & `phidata-1.7.6/phidata/task/upload/file/to_sql.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/types/airflow.py` & `phidata-1.7.6/phidata/types/airflow.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/types/context.py` & `phidata-1.7.6/phidata/types/context.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/types/phidata_runtime.py` & `phidata-1.7.6/phidata/types/phidata_runtime.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/utils/cli_console.py` & `phidata-1.7.6/phidata/utils/cli_console.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/utils/common.py` & `phidata-1.7.6/phidata/utils/common.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/utils/compare.py` & `phidata-1.7.6/phidata/utils/compare.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/utils/context.py` & `phidata-1.7.6/phidata/utils/context.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/utils/dttm.py` & `phidata-1.7.6/phidata/utils/dttm.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/utils/enums.py` & `phidata-1.7.6/phidata/utils/enums.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/utils/env_file.py` & `phidata-1.7.6/phidata/utils/env_file.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/utils/env_var.py` & `phidata-1.7.6/phidata/utils/env_var.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/utils/filesystem.py` & `phidata-1.7.6/phidata/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/utils/get_python_objects_from_module.py` & `phidata-1.7.6/phidata/utils/get_python_objects_from_module.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/utils/json_io.py` & `phidata-1.7.6/phidata/utils/json_io.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/utils/k8s.py` & `phidata-1.7.6/phidata/utils/k8s.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/utils/log.py` & `phidata-1.7.6/phidata/utils/log.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/utils/print_table.py` & `phidata-1.7.6/phidata/utils/print_table.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/utils/workspace_path.py` & `phidata-1.7.6/phidata/utils/workspace_path.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/utils/yaml_io.py` & `phidata-1.7.6/phidata/utils/yaml_io.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/workflow/decorator.py` & `phidata-1.7.6/phidata/workflow/decorator.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/workflow/workflow.py` & `phidata-1.7.6/phidata/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/workflow/workflow_relatives.py` & `phidata-1.7.6/phidata/workflow/workflow_relatives.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/workspace/config.py` & `phidata-1.7.6/phidata/workspace/config.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata/workspace/settings.py` & `phidata-1.7.6/phidata/workspace/settings.py`

 * *Files identical despite different names*

### Comparing `phidata-1.7.5/phidata.egg-info/PKG-INFO` & `phidata-1.7.6/phidata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phidata
-Version: 1.7.5
+Version: 1.7.6
 Summary: Phidata is a toolkit for building applications using OSS
 Author-email: Ashpreet Bedi <ashpreet@phidata.com>
 Project-URL: homepage, https://phidata.com
 Project-URL: documentation, https://docs.phidata.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: phidata Version: 1.7.5 Summary: Phidata is a
+Metadata-Version: 2.1 Name: phidata Version: 1.7.6 Summary: Phidata is a
 toolkit for building applications using OSS Author-email: Ashpreet Bedi
 phidata.com> Project-URL: homepage, https://phidata.com Project-URL:
 documentation, https://docs.phidata.com Requires-Python: >=3.7 Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: aws License-
 File: LICENSE
                              ****** phidata ******
           A toolkit for building applications using open source tools
```

### Comparing `phidata-1.7.5/phidata.egg-info/SOURCES.txt` & `phidata-1.7.6/phidata.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 phidata/app/cadvisor/cadvisor.py
 phidata/app/databox/__init__.py
 phidata/app/databox/databox.py
 phidata/app/db/__init__.py
 phidata/app/db/base_db.py
 phidata/app/django/__init__.py
 phidata/app/django/django_app.py
+phidata/app/django/django_backup.py
 phidata/app/elastic/__init__.py
 phidata/app/elastic/elastic_app.py
 phidata/app/elasticsearch/__init__.py
 phidata/app/elasticsearch/elasticsearch.py
 phidata/app/fastapi/__init__.py
 phidata/app/fastapi/fastapi_server.py
 phidata/app/grafana/__init__.py
```

### Comparing `phidata-1.7.5/pyproject.toml` & `phidata-1.7.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [project]
 name = "phidata"
-version = "1.7.5"
+version = "1.7.6"
 description = "Phidata is a toolkit for building applications using OSS"
 requires-python = ">=3.7"
 readme = "README.md"
 authors = [
   {name = "Ashpreet Bedi", email = "ashpreet@phidata.com"}
 ]
 
 dependencies = [
   "boto3>=1.26.76,<1.26.77",
   "botocore>=1.29.76,<1.29.77",
-  "phiterm==1.7.5",
+  "phiterm==1.7.6",
   "pyarrow",
   "pydantic",
 ]
 
 [project.optional-dependencies]
 dev = [
     "mypy",
```

