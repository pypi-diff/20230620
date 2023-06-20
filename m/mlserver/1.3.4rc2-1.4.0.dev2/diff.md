# Comparing `tmp/mlserver-1.3.4rc2.tar.gz` & `tmp/mlserver-1.4.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlserver-1.3.4rc2.tar", last modified: Tue Jun 20 09:24:40 2023, max compression
+gzip compressed data, was "mlserver-1.4.0.dev2.tar", last modified: Thu May  4 09:30:38 2023, max compression
```

## Comparing `mlserver-1.3.4rc2.tar` & `mlserver-1.4.0.dev2.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:24:40.178346 mlserver-1.3.4rc2/
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-06-20 09:24:40.178346 mlserver-1.3.4rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:24:40.166346 mlserver-1.3.4rc2/mlserver/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16370 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/batch_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:24:40.166346 mlserver-1.3.4rc2/mlserver/batching/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/batching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/batching/adaptive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/batching/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    10847 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/batching/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/batching/shape.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:24:40.166346 mlserver-1.3.4rc2/mlserver/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/cli/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/cli/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/cli/init_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/cli/serve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/cloudevents.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:24:40.170346 mlserver-1.3.4rc2/mlserver/codecs/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/codecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/codecs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/codecs/base64.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/codecs/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     7306 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/codecs/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/codecs/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/codecs/lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/codecs/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/codecs/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/codecs/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/codecs/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:24:40.170346 mlserver-1.3.4rc2/mlserver/grpc/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16463 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/grpc/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    31033 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/grpc/dataplane_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    15571 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/grpc/dataplane_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/grpc/interceptors.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/grpc/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/grpc/model_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6507 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/grpc/model_repository_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/grpc/model_repository_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/grpc/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/grpc/servicers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/grpc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:24:40.170346 mlserver-1.3.4rc2/mlserver/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/handlers/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/handlers/dataplane.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/handlers/model_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:24:40.170346 mlserver-1.3.4rc2/mlserver/kafka/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/kafka/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/kafka/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/kafka/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/kafka/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/kafka/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:24:40.174346 mlserver-1.3.4rc2/mlserver/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/metrics/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/metrics/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/metrics/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/metrics/prometheus.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/metrics/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/metrics/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     7749 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:24:40.174346 mlserver-1.3.4rc2/mlserver/parallel/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/parallel/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/parallel/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/parallel/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/parallel/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/parallel/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/parallel/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/parallel/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/parallel/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6868 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/parallel/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/raw.py
--rw-r--r--   0 runner    (1001) docker     (123)    10897 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:24:40.174346 mlserver-1.3.4rc2/mlserver/repository/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/repository/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/repository/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/repository/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:24:40.174346 mlserver-1.3.4rc2/mlserver/rest/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/rest/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/rest/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/rest/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/rest/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:24:40.178346 mlserver-1.3.4rc2/mlserver/rest/openapi/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/rest/openapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19065 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/rest/openapi/dataplane.json
--rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/rest/openapi/model_repository.json
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/rest/openapi/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/rest/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/rest/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/rest/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/rest/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:24:40.178346 mlserver-1.3.4rc2/mlserver/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/types/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/types/dataplane.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/types/model_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/mlserver/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:24:40.166346 mlserver-1.3.4rc2/mlserver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-06-20 09:24:39.000000 mlserver-1.3.4rc2/mlserver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-06-20 09:24:40.000000 mlserver-1.3.4rc2/mlserver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 09:24:39.000000 mlserver-1.3.4rc2/mlserver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-20 09:24:39.000000 mlserver-1.3.4rc2/mlserver.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-20 09:24:39.000000 mlserver-1.3.4rc2/mlserver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 09:24:39.000000 mlserver-1.3.4rc2/mlserver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-06-20 09:24:40.178346 mlserver-1.3.4rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-20 09:23:49.000000 mlserver-1.3.4rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:38.447136 mlserver-1.4.0.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-05-04 09:30:38.447136 mlserver-1.4.0.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:38.439136 mlserver-1.4.0.dev2/mlserver/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16113 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/batch_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:38.439136 mlserver-1.4.0.dev2/mlserver/batching/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/batching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/batching/adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/batching/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10847 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/batching/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/batching/shape.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:38.439136 mlserver-1.4.0.dev2/mlserver/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/cli/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/cli/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/cli/init_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/cli/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/cloudevents.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:38.439136 mlserver-1.4.0.dev2/mlserver/codecs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/codecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/codecs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/codecs/base64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/codecs/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7306 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/codecs/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/codecs/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/codecs/lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/codecs/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/codecs/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/codecs/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7557 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/codecs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:38.443136 mlserver-1.4.0.dev2/mlserver/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16463 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/grpc/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31033 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/grpc/dataplane_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15571 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/grpc/dataplane_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/grpc/interceptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/grpc/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/grpc/model_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6507 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/grpc/model_repository_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/grpc/model_repository_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/grpc/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/grpc/servicers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/grpc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:38.443136 mlserver-1.4.0.dev2/mlserver/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/handlers/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/handlers/dataplane.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/handlers/model_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:38.443136 mlserver-1.4.0.dev2/mlserver/kafka/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/kafka/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/kafka/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/kafka/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/kafka/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/kafka/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:38.443136 mlserver-1.4.0.dev2/mlserver/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/metrics/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/metrics/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/metrics/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/metrics/prometheus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/metrics/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/metrics/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7749 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:38.443136 mlserver-1.4.0.dev2/mlserver/parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/parallel/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/parallel/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/parallel/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/parallel/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/parallel/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/parallel/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/parallel/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/parallel/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6868 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/parallel/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10897 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:38.443136 mlserver-1.4.0.dev2/mlserver/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/repository/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/repository/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/repository/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:38.447136 mlserver-1.4.0.dev2/mlserver/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/rest/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/rest/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/rest/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/rest/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:38.447136 mlserver-1.4.0.dev2/mlserver/rest/openapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/rest/openapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19065 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/rest/openapi/dataplane.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/rest/openapi/model_repository.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/rest/openapi/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/rest/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/rest/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/rest/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/rest/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:38.447136 mlserver-1.4.0.dev2/mlserver/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/types/dataplane.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/types/model_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:38.439136 mlserver-1.4.0.dev2/mlserver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-05-04 09:30:38.000000 mlserver-1.4.0.dev2/mlserver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-05-04 09:30:38.000000 mlserver-1.4.0.dev2/mlserver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:30:38.000000 mlserver-1.4.0.dev2/mlserver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-04 09:30:38.000000 mlserver-1.4.0.dev2/mlserver.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-04 09:30:38.000000 mlserver-1.4.0.dev2/mlserver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-04 09:30:38.000000 mlserver-1.4.0.dev2/mlserver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-05-04 09:30:38.447136 mlserver-1.4.0.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/setup.py
```

### Comparing `mlserver-1.3.4rc2/LICENSE` & `mlserver-1.4.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/PKG-INFO` & `mlserver-1.4.0.dev2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlserver
-Version: 1.3.4rc2
+Version: 1.4.0.dev2
 Summary: ML server
 Home-page: https://github.com/SeldonIO/MLServer.git
 Author: Seldon Technologies Ltd.
 Author-email: hello@seldon.io
 License: Apache 2.0
 Description: # MLServer
         
@@ -118,10 +118,8 @@
         For example:
         
         ```bash
         ./hack/update-version.sh 0.2.0.dev1
         ```
         
 Platform: UNKNOWN
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: MacOS
 Description-Content-Type: text/markdown
```

### Comparing `mlserver-1.3.4rc2/README.md` & `mlserver-1.4.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/batch_processing.py` & `mlserver-1.4.0.dev2/mlserver/batch_processing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from dataclasses import dataclass
 from functools import wraps
 import os
 from random import random
 import tritonclient.http.aio as httpclient
 
 import asyncio
-import numpy as np
 import aiofiles
 import logging
 import click
 import json
 import orjson
 
 from time import perf_counter as timer
@@ -98,29 +97,25 @@
     outputs: Optional[List[httpclient.InferRequestedOutput]]
 
     @classmethod
     def from_inference_request(
         cls, inference_request: InferenceRequest, binary_data: bool
     ) -> "TritonRequest":
         inputs = []
+
         for request_input in inference_request.inputs or []:
             new_input = httpclient.InferInput(
                 request_input.name, request_input.shape, request_input.datatype
             )
-            request_input_np = NumpyCodec.decode_input(request_input)
-
-            # Change datatype if BYTES to satisfy Tritonclient checks
-            if request_input.datatype == "BYTES":
-                request_input_np = request_input_np.astype(np.object_)
-
             new_input.set_data_from_numpy(
-                request_input_np,
+                NumpyCodec.decode_input(request_input),
                 binary_data=binary_data,
             )
             inputs.append(new_input)
+
         outputs = []
         for request_output in inference_request.outputs or []:
             new_output = httpclient.InferRequestedOutput(
                 request_output.name, binary_data=binary_data
             )
             outputs.append(new_output)
 
@@ -209,14 +204,15 @@
             item_indices[inference_request.id] = item.index
         except ValidationError as e:
             logger.error(
                 f"preprocessing error: batch_index={item.index}, error={repr(e)}"
             )
             invalid_inputs.append(_serialize_validation_error(item.index, e))
     batched = BatchedRequests(inference_requests)
+
     # Set `id` for batched requests - if only single request use its own id
     if len(inference_requests) == 1:
         batched.merged_request.id = inference_request.id
     else:
         batched.merged_request.id = generate_uuid()
     return (
         TritonRequest.from_inference_request(batched.merged_request, binary_data),
```

### Comparing `mlserver-1.3.4rc2/mlserver/batching/adaptive.py` & `mlserver-1.4.0.dev2/mlserver/batching/adaptive.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/batching/hooks.py` & `mlserver-1.4.0.dev2/mlserver/batching/hooks.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/batching/requests.py` & `mlserver-1.4.0.dev2/mlserver/batching/requests.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/batching/shape.py` & `mlserver-1.4.0.dev2/mlserver/batching/shape.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/cli/build.py` & `mlserver-1.4.0.dev2/mlserver/cli/build.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/cli/constants.py` & `mlserver-1.4.0.dev2/mlserver/cli/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     .
 RUN mkdir $(dirname $MLSERVER_ENV_TARBALL); \\
     for envFile in environment.yml environment.yaml conda.yml conda.yaml; do \\
         if [[ -f $envFile ]]; then \\
             conda env create \
                 --name $MLSERVER_ENV_NAME \\
                 --file $envFile; \\
-            conda-pack --ignore-missing-files --quiet \
+            conda-pack --ignore-missing-files \
                 -n $MLSERVER_ENV_NAME \\
                 -o $MLSERVER_ENV_TARBALL; \\
         fi \\
     done; \\
     chmod -R 776 $(dirname $MLSERVER_ENV_TARBALL)
 
 FROM seldonio/mlserver:{version}-slim
```

### Comparing `mlserver-1.3.4rc2/mlserver/cli/main.py` & `mlserver-1.4.0.dev2/mlserver/cli/main.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/cli/serve.py` & `mlserver-1.4.0.dev2/mlserver/cli/serve.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/cloudevents.py` & `mlserver-1.4.0.dev2/mlserver/cloudevents.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/codecs/__init__.py` & `mlserver-1.4.0.dev2/mlserver/codecs/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .numpy import NumpyCodec, NumpyRequestCodec
 from .pandas import PandasCodec
-from .string import StringCodec, StringRequestCodec
+from .string import StringCodec
 from .base64 import Base64Codec
 from .datetime import DatetimeCodec
 from .errors import CodecError
 from .decorator import decode_args
 from .base import (
     InputCodec,
     RequestCodec,
```

### Comparing `mlserver-1.3.4rc2/mlserver/codecs/base.py` & `mlserver-1.4.0.dev2/mlserver/codecs/base.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/codecs/base64.py` & `mlserver-1.4.0.dev2/mlserver/codecs/base64.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import base64
 import binascii
 
 from typing import Any, List, Union
 from functools import partial
 
-from ..types import RequestInput, ResponseOutput, Parameters
+from ..types import RequestInput, ResponseOutput
 from .lists import is_list_of
 from .base import InputCodec, register_input_codec
 from .lists import as_list, ListElement
 
 _Base64StrCodec = "ascii"
 
 
@@ -60,15 +60,14 @@
         packed = map(partial(_encode_base64, use_bytes=use_bytes), payload)
         shape = [len(payload), 1]
         return ResponseOutput(
             name=name,
             datatype="BYTES",
             shape=shape,
             data=list(packed),
-            parameters=Parameters(content_type=cls.ContentType),
         )
 
     @classmethod
     def decode_output(cls, response_output: ResponseOutput) -> List[bytes]:
         packed = response_output.data.__root__
         return list(map(_decode_base64, as_list(packed)))
 
@@ -79,15 +78,14 @@
         # Assume that payload is already in b64, so we only need to pack it
         output = cls.encode_output(name, payload, use_bytes)
         return RequestInput(
             name=output.name,
             datatype=output.datatype,
             shape=output.shape,
             data=output.data,
-            parameters=Parameters(content_type=cls.ContentType),
         )
 
     @classmethod
     def decode_input(cls, request_input: RequestInput) -> List[bytes]:
         packed = request_input.data.__root__
 
         return list(map(_decode_base64, as_list(packed)))
```

### Comparing `mlserver-1.3.4rc2/mlserver/codecs/datetime.py` & `mlserver-1.4.0.dev2/mlserver/codecs/datetime.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any, Union, List
 from datetime import datetime
 from functools import partial
 
-from ..types import RequestInput, ResponseOutput, Parameters
+from ..types import RequestInput, ResponseOutput
 from .lists import is_list_of, as_list, ListElement
 from .base import InputCodec, register_input_codec
 
 _Datetime = Union[str, datetime]
 _DatetimeStrCodec = "ascii"
 
 
@@ -58,15 +58,14 @@
         packed = map(partial(_encode_datetime, use_bytes=use_bytes), payload)
         shape = [len(payload), 1]
         return ResponseOutput(
             name=name,
             datatype="BYTES",
             shape=shape,
             data=list(packed),
-            parameters=Parameters(content_type=cls.ContentType),
         )
 
     @classmethod
     def decode_output(cls, response_output: ResponseOutput) -> List[datetime]:
         packed = response_output.data.__root__
 
         return list(map(_decode_datetime, as_list(packed)))
@@ -77,15 +76,14 @@
     ) -> RequestInput:
         output = cls.encode_output(name, payload, use_bytes=use_bytes)
         return RequestInput(
             name=output.name,
             datatype=output.datatype,
             shape=output.shape,
             data=output.data,
-            parameters=Parameters(content_type=cls.ContentType),
         )
 
     @classmethod
     def decode_input(cls, request_input: RequestInput) -> List[datetime]:
         packed = request_input.data.__root__
 
         return list(map(_decode_datetime, as_list(packed)))
```

### Comparing `mlserver-1.3.4rc2/mlserver/codecs/decorator.py` & `mlserver-1.4.0.dev2/mlserver/codecs/decorator.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/codecs/errors.py` & `mlserver-1.4.0.dev2/mlserver/codecs/errors.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/codecs/lists.py` & `mlserver-1.4.0.dev2/mlserver/codecs/lists.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/codecs/numpy.py` & `mlserver-1.4.0.dev2/mlserver/codecs/numpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,14 @@
         shape = inject_batch_dimension(list(payload.shape))
 
         return ResponseOutput(
             name=name,
             datatype=datatype,
             shape=shape,
             data=_encode_data(payload, datatype),
-            parameters=Parameters(content_type=cls.ContentType),
         )
 
     @classmethod
     def decode_output(cls, response_output: ResponseOutput) -> np.ndarray:
         return cls.decode_input(response_output)  # type: ignore
 
     @classmethod
```

### Comparing `mlserver-1.3.4rc2/mlserver/codecs/string.py` & `mlserver-1.4.0.dev2/mlserver/codecs/string.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/codecs/utils.py` & `mlserver-1.4.0.dev2/mlserver/codecs/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,18 +198,15 @@
                 f"No input codec found for {type(cls)} request codec"
             )
 
         output = cls.InputCodec.encode_output(
             f"{DefaultOutputPrefix}1", payload, **kwargs
         )
         return InferenceResponse(
-            model_name=model_name,
-            model_version=model_version,
-            parameters=Parameters(content_type=cls.ContentType),
-            outputs=[output],
+            model_name=model_name, model_version=model_version, outputs=[output]
         )
 
     @classmethod
     def decode_response(cls, response: InferenceResponse) -> Any:
         if len(response.outputs) != 1:
             raise CodecError(
                 f"The '{cls.ContentType}' codec only supports a single output tensor "
@@ -227,17 +224,15 @@
     def encode_request(cls, payload: Any, **kwargs) -> InferenceRequest:
         if cls.InputCodec is None:
             raise NotImplementedError(
                 f"No input codec found for {type(cls)} request codec"
             )
 
         inp = cls.InputCodec.encode_input(f"{DefaultInputPrefix}1", payload, **kwargs)
-        return InferenceRequest(
-            inputs=[inp], parameters=Parameters(content_type=cls.ContentType)
-        )
+        return InferenceRequest(inputs=[inp])
 
     @classmethod
     def decode_request(cls, request: InferenceRequest) -> Any:
         if len(request.inputs) != 1:
             raise CodecError(
                 f"The '{cls.ContentType}' codec only supports a single input tensor "
                 f"({len(request.inputs)} were received)"
```

### Comparing `mlserver-1.3.4rc2/mlserver/env.py` & `mlserver-1.4.0.dev2/mlserver/env.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/errors.py` & `mlserver-1.4.0.dev2/mlserver/errors.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/grpc/converters.py` & `mlserver-1.4.0.dev2/mlserver/grpc/converters.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/grpc/dataplane_pb2.py` & `mlserver-1.4.0.dev2/mlserver/grpc/dataplane_pb2.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/grpc/dataplane_pb2_grpc.py` & `mlserver-1.4.0.dev2/mlserver/grpc/dataplane_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/grpc/interceptors.py` & `mlserver-1.4.0.dev2/mlserver/grpc/interceptors.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/grpc/model_repository.py` & `mlserver-1.4.0.dev2/mlserver/grpc/model_repository.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/grpc/model_repository_pb2.py` & `mlserver-1.4.0.dev2/mlserver/grpc/model_repository_pb2.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/grpc/model_repository_pb2_grpc.py` & `mlserver-1.4.0.dev2/mlserver/grpc/model_repository_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/grpc/server.py` & `mlserver-1.4.0.dev2/mlserver/grpc/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,17 +38,15 @@
         interceptors = []
 
         if self._settings.debug:
             # If debug, enable access logs
             interceptors = [LoggingInterceptor()]
 
         if self._settings.metrics_endpoint:
-            interceptors.append(
-                PromServerInterceptor(enable_handling_time_histogram=True)
-            )
+            interceptors.append(PromServerInterceptor())
 
         self._server = aio.server(
             ThreadPoolExecutor(max_workers=DefaultGrpcWorkers),
             interceptors=tuple(interceptors),
             options=self._get_options(),
         )
```

### Comparing `mlserver-1.3.4rc2/mlserver/grpc/servicers.py` & `mlserver-1.4.0.dev2/mlserver/grpc/servicers.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/grpc/utils.py` & `mlserver-1.4.0.dev2/mlserver/grpc/utils.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/handlers/custom.py` & `mlserver-1.4.0.dev2/mlserver/handlers/custom.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/handlers/dataplane.py` & `mlserver-1.4.0.dev2/mlserver/handlers/dataplane.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/handlers/model_repository.py` & `mlserver-1.4.0.dev2/mlserver/handlers/model_repository.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/kafka/handlers.py` & `mlserver-1.4.0.dev2/mlserver/kafka/handlers.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/kafka/message.py` & `mlserver-1.4.0.dev2/mlserver/kafka/message.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/kafka/server.py` & `mlserver-1.4.0.dev2/mlserver/kafka/server.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/logging.py` & `mlserver-1.4.0.dev2/mlserver/logging.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/metrics/context.py` & `mlserver-1.4.0.dev2/mlserver/metrics/context.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/metrics/errors.py` & `mlserver-1.4.0.dev2/mlserver/metrics/errors.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/metrics/prometheus.py` & `mlserver-1.4.0.dev2/mlserver/metrics/prometheus.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/metrics/registry.py` & `mlserver-1.4.0.dev2/mlserver/metrics/registry.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/metrics/server.py` & `mlserver-1.4.0.dev2/mlserver/metrics/server.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/middleware.py` & `mlserver-1.4.0.dev2/mlserver/middleware.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/model.py` & `mlserver-1.4.0.dev2/mlserver/model.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/parallel/dispatcher.py` & `mlserver-1.4.0.dev2/mlserver/parallel/dispatcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     def _get_or_create_metric(self) -> Histogram:
         if QUEUE_METRIC_NAME in REGISTRY:
             return REGISTRY[QUEUE_METRIC_NAME]  # type: ignore
 
         return Histogram(
             QUEUE_METRIC_NAME,
             "counter of request queue size for workers",
+            ["workerpid"],
             registry=REGISTRY,
         )
 
     def start(self):
         self._active = True
         self._process_responses_task = schedule_with_callback(
             self._process_responses(), self._process_responses_cb
@@ -91,26 +92,35 @@
         else:
             response_loop.call_soon_threadsafe(async_response.set_result, response)
 
     async def dispatch_request(
         self, request_message: ModelRequestMessage
     ) -> ModelResponseMessage:
         worker, wpid = self._get_worker()
+        self._workers_queue_monitor(worker, wpid)
         worker.send_request(request_message)
 
         return await self._dispatch(request_message)
 
     def _get_worker(self) -> Tuple[Worker, int]:
         """
         Get next available worker.
         By default, this is just a round-robin through all the workers.
         """
         worker_pid = next(self._workers_round_robin)
         return self._workers[worker_pid], worker_pid
 
+    def _workers_queue_monitor(self, worker: Worker, worker_pid: int):
+        """Get metrics from every worker request queue"""
+        queue_size = worker._requests.qsize()
+
+        self.parallel_request_queue_size.labels(workerpid=str(worker_pid)).observe(
+            float(queue_size)
+        )
+
     async def dispatch_update(
         self, model_update: ModelUpdateMessage
     ) -> List[ModelResponseMessage]:
         return await asyncio.gather(
             *[
                 self._dispatch_update(worker, model_update)
                 for worker in self._workers.values()
@@ -129,16 +139,14 @@
 
     async def _dispatch(self, message: Message) -> ModelResponseMessage:
         loop = asyncio.get_running_loop()
         async_response = loop.create_future()
         internal_id = message.id
         self._async_responses[internal_id] = async_response
 
-        # Monitor current in-flight requests
-        self.parallel_request_queue_size.observe(len(self._async_responses))
         return await self._wait_response(internal_id)
 
     async def _wait_response(self, internal_id: str) -> ModelResponseMessage:
         async_response = self._async_responses[internal_id]
 
         try:
             inference_response = await async_response
```

### Comparing `mlserver-1.3.4rc2/mlserver/parallel/errors.py` & `mlserver-1.4.0.dev2/mlserver/parallel/errors.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/parallel/messages.py` & `mlserver-1.4.0.dev2/mlserver/parallel/messages.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/parallel/model.py` & `mlserver-1.4.0.dev2/mlserver/parallel/model.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/parallel/pool.py` & `mlserver-1.4.0.dev2/mlserver/parallel/pool.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/parallel/registry.py` & `mlserver-1.4.0.dev2/mlserver/parallel/registry.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/parallel/utils.py` & `mlserver-1.4.0.dev2/mlserver/parallel/utils.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/parallel/worker.py` & `mlserver-1.4.0.dev2/mlserver/parallel/worker.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/raw.py` & `mlserver-1.4.0.dev2/mlserver/raw.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/registry.py` & `mlserver-1.4.0.dev2/mlserver/registry.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/repository/factory.py` & `mlserver-1.4.0.dev2/mlserver/repository/factory.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/repository/load.py` & `mlserver-1.4.0.dev2/mlserver/repository/load.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/repository/repository.py` & `mlserver-1.4.0.dev2/mlserver/repository/repository.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/rest/app.py` & `mlserver-1.4.0.dev2/mlserver/rest/app.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/rest/endpoints.py` & `mlserver-1.4.0.dev2/mlserver/rest/endpoints.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/rest/logging.py` & `mlserver-1.4.0.dev2/mlserver/rest/logging.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/rest/openapi/dataplane.json` & `mlserver-1.4.0.dev2/mlserver/rest/openapi/dataplane.json`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/rest/openapi/model_repository.json` & `mlserver-1.4.0.dev2/mlserver/rest/openapi/model_repository.json`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/rest/openapi/schema.py` & `mlserver-1.4.0.dev2/mlserver/rest/openapi/schema.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/rest/requests.py` & `mlserver-1.4.0.dev2/mlserver/rest/requests.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/rest/responses.py` & `mlserver-1.4.0.dev2/mlserver/rest/responses.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/rest/server.py` & `mlserver-1.4.0.dev2/mlserver/rest/server.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/rest/utils.py` & `mlserver-1.4.0.dev2/mlserver/rest/utils.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/server.py` & `mlserver-1.4.0.dev2/mlserver/server.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/settings.py` & `mlserver-1.4.0.dev2/mlserver/settings.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/types/__init__.py` & `mlserver-1.4.0.dev2/mlserver/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/types/base.py` & `mlserver-1.4.0.dev2/mlserver/types/base.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/types/dataplane.py` & `mlserver-1.4.0.dev2/mlserver/types/dataplane.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/types/model_repository.py` & `mlserver-1.4.0.dev2/mlserver/types/model_repository.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver/utils.py` & `mlserver-1.4.0.dev2/mlserver/utils.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/mlserver.egg-info/PKG-INFO` & `mlserver-1.4.0.dev2/mlserver.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlserver
-Version: 1.3.4rc2
+Version: 1.4.0.dev2
 Summary: ML server
 Home-page: https://github.com/SeldonIO/MLServer.git
 Author: Seldon Technologies Ltd.
 Author-email: hello@seldon.io
 License: Apache 2.0
 Description: # MLServer
         
@@ -118,10 +118,8 @@
         For example:
         
         ```bash
         ./hack/update-version.sh 0.2.0.dev1
         ```
         
 Platform: UNKNOWN
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: MacOS
 Description-Content-Type: text/markdown
```

### Comparing `mlserver-1.3.4rc2/mlserver.egg-info/SOURCES.txt` & `mlserver-1.4.0.dev2/mlserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/setup.cfg` & `mlserver-1.4.0.dev2/setup.cfg`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.4rc2/setup.py` & `mlserver-1.4.0.dev2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 
 setup(
     name=PKG_NAME,
     version=_load_version(),
     url="https://github.com/SeldonIO/MLServer.git",
     author="Seldon Technologies Ltd.",
     author_email="hello@seldon.io",
-    classifiers=["Operating System :: POSIX", "Operating System :: MacOS"],
     description="ML server",
     include_package_data=True,
     packages=find_packages(exclude=["tests", "tests.*"]),
     install_requires=[
         "click",
         # 0.89.0: https://github.com/tiangolo/fastapi/issues/5861
         "fastapi >=0.88.0, <=0.89.1, !=0.89.0",
```

