# Comparing `tmp/hera-5.4.1.tar.gz` & `tmp/hera-5.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hera-5.4.1.tar", max compression
+gzip compressed data, was "hera-5.5.0.tar", max compression
```

## Comparing `hera-5.4.1.tar` & `hera-5.5.0.tar`

### file list

```diff
@@ -1,134 +1,137 @@
--rw-r--r--   0        0        0     1066 2023-06-01 20:08:41.759320 hera-5.4.1/LICENSE
--rw-r--r--   0        0        0    11980 2023-06-01 20:08:41.759320 hera-5.4.1/README.md
--rw-r--r--   0        0        0     3530 2023-06-01 20:08:58.303530 hera-5.4.1/pyproject.toml
--rw-r--r--   0        0        0      522 2023-06-01 20:08:41.779320 hera-5.4.1/src/hera/__init__.py
--rw-r--r--   0        0        0      300 2023-06-01 20:08:41.779320 hera-5.4.1/src/hera/_version.py
--rw-r--r--   0        0        0        0 2023-06-01 20:08:41.779320 hera-5.4.1/src/hera/events/__init__.py
--rw-r--r--   0        0        0     3267 2023-06-01 20:08:41.779320 hera-5.4.1/src/hera/events/models/__init__.py
--rw-r--r--   0        0        0     1418 2023-06-01 20:08:41.779320 hera-5.4.1/src/hera/events/models/eventsource.py
--rw-r--r--   0        0        0      861 2023-06-01 20:08:41.779320 hera-5.4.1/src/hera/events/models/eventsource.pyi
--rw-r--r--   0        0        0      144 2023-06-01 20:08:41.779320 hera-5.4.1/src/hera/events/models/google/__init__.py
--rw-r--r--   0        0        0      347 2023-06-01 20:08:41.779320 hera-5.4.1/src/hera/events/models/google/protobuf.py
--rw-r--r--   0        0        0      164 2023-06-01 20:08:41.779320 hera-5.4.1/src/hera/events/models/google/protobuf.pyi
--rw-r--r--   0        0        0        0 2023-06-01 20:08:41.779320 hera-5.4.1/src/hera/events/models/grpc/__init__.py
--rw-r--r--   0        0        0      144 2023-06-01 20:08:41.779320 hera-5.4.1/src/hera/events/models/grpc/gateway/__init__.py
--rw-r--r--   0        0        0      691 2023-06-01 20:08:41.779320 hera-5.4.1/src/hera/events/models/grpc/gateway/runtime.py
--rw-r--r--   0        0        0      470 2023-06-01 20:08:41.779320 hera-5.4.1/src/hera/events/models/grpc/gateway/runtime.pyi
--rw-r--r--   0        0        0        0 2023-06-01 20:08:41.779320 hera-5.4.1/src/hera/events/models/io/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 20:08:41.779320 hera-5.4.1/src/hera/events/models/io/argoproj/__init__.py
--rw-r--r--   0        0        0      144 2023-06-01 20:08:41.779320 hera-5.4.1/src/hera/events/models/io/argoproj/events/__init__.py
--rw-r--r--   0        0        0   102993 2023-06-01 20:08:41.779320 hera-5.4.1/src/hera/events/models/io/argoproj/events/v1alpha1.py
--rw-r--r--   0        0        0    25271 2023-06-01 20:08:41.779320 hera-5.4.1/src/hera/events/models/io/argoproj/events/v1alpha1.pyi
--rw-r--r--   0        0        0      144 2023-06-01 20:08:41.779320 hera-5.4.1/src/hera/events/models/io/argoproj/workflow/__init__.py
--rw-r--r--   0        0        0   144549 2023-06-01 20:08:41.779320 hera-5.4.1/src/hera/events/models/io/argoproj/workflow/v1alpha1.py
--rw-r--r--   0        0        0    31958 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/events/models/io/argoproj/workflow/v1alpha1.pyi
--rw-r--r--   0        0        0        0 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/events/models/io/k8s/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/events/models/io/k8s/api/__init__.py
--rw-r--r--   0        0        0      144 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/events/models/io/k8s/api/core/__init__.py
--rw-r--r--   0        0        0   127883 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/events/models/io/k8s/api/core/v1.py
--rw-r--r--   0        0        0    18004 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/events/models/io/k8s/api/core/v1.pyi
--rw-r--r--   0        0        0      144 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/events/models/io/k8s/api/policy/__init__.py
--rw-r--r--   0        0        0     1751 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/events/models/io/k8s/api/policy/v1beta1.py
--rw-r--r--   0        0        0      376 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/events/models/io/k8s/api/policy/v1beta1.pyi
--rw-r--r--   0        0        0        0 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/events/models/io/k8s/apimachinery/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/events/models/io/k8s/apimachinery/pkg/__init__.py
--rw-r--r--   0        0        0      144 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/events/models/io/k8s/apimachinery/pkg/api/__init__.py
--rw-r--r--   0        0        0     3161 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.py
--rw-r--r--   0        0        0      105 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.pyi
--rw-r--r--   0        0        0        0 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/events/models/io/k8s/apimachinery/pkg/apis/__init__.py
--rw-r--r--   0        0        0      144 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/__init__.py
--rw-r--r--   0        0        0    22218 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.py
--rw-r--r--   0        0        0     2064 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi
--rw-r--r--   0        0        0      144 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/events/models/io/k8s/apimachinery/pkg/util/__init__.py
--rw-r--r--   0        0        0      277 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/events/models/io/k8s/apimachinery/pkg/util/intstr.py
--rw-r--r--   0        0        0      108 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/events/models/io/k8s/apimachinery/pkg/util/intstr.pyi
--rw-r--r--   0        0        0     1453 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/events/models/sensor.py
--rw-r--r--   0        0        0      887 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/events/models/sensor.pyi
--rw-r--r--   0        0        0    27607 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/events/service.py
--rw-r--r--   0        0        0     2186 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/exceptions/__init__.py
--rw-r--r--   0        0        0      282 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/expr/__init__.py
--rw-r--r--   0        0        0    12021 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/expr/_node.py
--rw-r--r--   0        0        0      647 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/expr/_sprig.py
--rw-r--r--   0        0        0        0 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/py.typed
--rw-r--r--   0        0        0      188 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/shared/__init__.py
--rw-r--r--   0        0        0      269 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/shared/_base_model.py
--rw-r--r--   0        0        0     4927 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/shared/_global_config.py
--rw-r--r--   0        0        0      513 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/shared/serialization.py
--rw-r--r--   0        0        0     4585 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/workflows/__init__.py
--rw-r--r--   0        0        0     2912 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/workflows/_context.py
--rw-r--r--   0        0        0    35054 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/workflows/_mixins.py
--rw-r--r--   0        0        0    32815 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/workflows/_unparse.py
--rw-r--r--   0        0        0       25 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/workflows/action.py
--rw-r--r--   0        0        0     1115 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/workflows/archive.py
--rw-r--r--   0        0        0     7697 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/workflows/artifact.py
--rw-r--r--   0        0        0     3464 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/workflows/container.py
--rw-r--r--   0        0        0     7280 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/workflows/container_set.py
--rw-r--r--   0        0        0     3779 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/workflows/cron_workflow.py
--rw-r--r--   0        0        0     2877 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/workflows/dag.py
--rw-r--r--   0        0        0     2241 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/workflows/data.py
--rw-r--r--   0        0        0     4855 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/workflows/env.py
--rw-r--r--   0        0        0     1329 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/workflows/env_from.py
--rw-r--r--   0        0        0      208 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/workflows/exceptions.py
--rw-r--r--   0        0        0     2346 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/workflows/http_template.py
--rw-r--r--   0        0        0       30 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/workflows/memoize.py
--rw-r--r--   0        0        0     4418 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/workflows/metrics.py
--rw-r--r--   0        0        0     6913 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/workflows/models/__init__.py
--rw-r--r--   0        0        0     1418 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/workflows/models/eventsource.py
--rw-r--r--   0        0        0      861 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/workflows/models/eventsource.pyi
--rw-r--r--   0        0        0      144 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/workflows/models/google/__init__.py
--rw-r--r--   0        0        0      347 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/workflows/models/google/protobuf.py
--rw-r--r--   0        0        0      164 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/workflows/models/google/protobuf.pyi
--rw-r--r--   0        0        0        0 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/workflows/models/grpc/__init__.py
--rw-r--r--   0        0        0      144 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/workflows/models/grpc/gateway/__init__.py
--rw-r--r--   0        0        0      691 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/workflows/models/grpc/gateway/runtime.py
--rw-r--r--   0        0        0      470 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/workflows/models/grpc/gateway/runtime.pyi
--rw-r--r--   0        0        0        0 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/workflows/models/io/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 20:08:41.783320 hera-5.4.1/src/hera/workflows/models/io/argoproj/__init__.py
--rw-r--r--   0        0        0      144 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/models/io/argoproj/events/__init__.py
--rw-r--r--   0        0        0   102993 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/models/io/argoproj/events/v1alpha1.py
--rw-r--r--   0        0        0    25271 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/models/io/argoproj/events/v1alpha1.pyi
--rw-r--r--   0        0        0      144 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/models/io/argoproj/workflow/__init__.py
--rw-r--r--   0        0        0   144549 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.py
--rw-r--r--   0        0        0    31958 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.pyi
--rw-r--r--   0        0        0        0 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/models/io/k8s/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/models/io/k8s/api/__init__.py
--rw-r--r--   0        0        0      144 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/models/io/k8s/api/core/__init__.py
--rw-r--r--   0        0        0   127883 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/models/io/k8s/api/core/v1.py
--rw-r--r--   0        0        0    18004 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/models/io/k8s/api/core/v1.pyi
--rw-r--r--   0        0        0      144 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/models/io/k8s/api/policy/__init__.py
--rw-r--r--   0        0        0     1751 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/models/io/k8s/api/policy/v1beta1.py
--rw-r--r--   0        0        0      376 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/models/io/k8s/api/policy/v1beta1.pyi
--rw-r--r--   0        0        0        0 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/models/io/k8s/apimachinery/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/models/io/k8s/apimachinery/pkg/__init__.py
--rw-r--r--   0        0        0      144 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/__init__.py
--rw-r--r--   0        0        0     3161 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.py
--rw-r--r--   0        0        0      105 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.pyi
--rw-r--r--   0        0        0        0 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/__init__.py
--rw-r--r--   0        0        0      144 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/__init__.py
--rw-r--r--   0        0        0    22218 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.py
--rw-r--r--   0        0        0     2064 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi
--rw-r--r--   0        0        0      144 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/__init__.py
--rw-r--r--   0        0        0      277 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/intstr.py
--rw-r--r--   0        0        0      108 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/intstr.pyi
--rw-r--r--   0        0        0     1453 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/models/sensor.py
--rw-r--r--   0        0        0      887 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/models/sensor.pyi
--rw-r--r--   0        0        0      722 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/operator.py
--rw-r--r--   0        0        0     4084 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/parameter.py
--rw-r--r--   0        0        0     1018 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/protocol.py
--rw-r--r--   0        0        0     3146 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/resource.py
--rw-r--r--   0        0        0     5262 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/resources.py
--rw-r--r--   0        0        0     1856 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/retry_strategy.py
--rw-r--r--   0        0        0     3707 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/runner.py
--rw-r--r--   0        0        0    16549 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/script.py
--rw-r--r--   0        0        0    55322 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/service.py
--rw-r--r--   0        0        0     6747 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/steps.py
--rw-r--r--   0        0        0     3332 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/suspend.py
--rw-r--r--   0        0        0     7959 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/task.py
--rw-r--r--   0        0        0       27 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/toleration.py
--rw-r--r--   0        0        0     2007 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/user_container.py
--rw-r--r--   0        0        0     2610 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/validators.py
--rw-r--r--   0        0        0    18709 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/volume.py
--rw-r--r--   0        0        0    18961 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/workflow.py
--rw-r--r--   0        0        0      911 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/workflow_status.py
--rw-r--r--   0        0        0     7343 2023-06-01 20:08:41.787320 hera-5.4.1/src/hera/workflows/workflow_template.py
--rw-r--r--   0        0        0    13403 1970-01-01 00:00:00.000000 hera-5.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-20 21:13:16.646984 hera-5.5.0/LICENSE
+-rw-r--r--   0        0        0    12133 2023-06-20 21:13:16.646984 hera-5.5.0/README.md
+-rw-r--r--   0        0        0     3530 2023-06-20 21:13:40.687183 hera-5.5.0/pyproject.toml
+-rw-r--r--   0        0        0      522 2023-06-20 21:13:16.670984 hera-5.5.0/src/hera/__init__.py
+-rw-r--r--   0        0        0      300 2023-06-20 21:13:16.670984 hera-5.5.0/src/hera/_version.py
+-rw-r--r--   0        0        0     1289 2023-06-20 21:13:16.670984 hera-5.5.0/src/hera/auth/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 21:13:16.670984 hera-5.5.0/src/hera/events/__init__.py
+-rw-r--r--   0        0        0     3267 2023-06-20 21:13:16.670984 hera-5.5.0/src/hera/events/models/__init__.py
+-rw-r--r--   0        0        0     1418 2023-06-20 21:13:16.670984 hera-5.5.0/src/hera/events/models/eventsource.py
+-rw-r--r--   0        0        0      861 2023-06-20 21:13:16.670984 hera-5.5.0/src/hera/events/models/eventsource.pyi
+-rw-r--r--   0        0        0      144 2023-06-20 21:13:16.670984 hera-5.5.0/src/hera/events/models/google/__init__.py
+-rw-r--r--   0        0        0      347 2023-06-20 21:13:16.670984 hera-5.5.0/src/hera/events/models/google/protobuf.py
+-rw-r--r--   0        0        0      164 2023-06-20 21:13:16.674984 hera-5.5.0/src/hera/events/models/google/protobuf.pyi
+-rw-r--r--   0        0        0        0 2023-06-20 21:13:16.674984 hera-5.5.0/src/hera/events/models/grpc/__init__.py
+-rw-r--r--   0        0        0      144 2023-06-20 21:13:16.674984 hera-5.5.0/src/hera/events/models/grpc/gateway/__init__.py
+-rw-r--r--   0        0        0      691 2023-06-20 21:13:16.674984 hera-5.5.0/src/hera/events/models/grpc/gateway/runtime.py
+-rw-r--r--   0        0        0      470 2023-06-20 21:13:16.674984 hera-5.5.0/src/hera/events/models/grpc/gateway/runtime.pyi
+-rw-r--r--   0        0        0        0 2023-06-20 21:13:16.674984 hera-5.5.0/src/hera/events/models/io/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 21:13:16.674984 hera-5.5.0/src/hera/events/models/io/argoproj/__init__.py
+-rw-r--r--   0        0        0      144 2023-06-20 21:13:16.674984 hera-5.5.0/src/hera/events/models/io/argoproj/events/__init__.py
+-rw-r--r--   0        0        0   102993 2023-06-20 21:13:16.674984 hera-5.5.0/src/hera/events/models/io/argoproj/events/v1alpha1.py
+-rw-r--r--   0        0        0    25271 2023-06-20 21:13:16.674984 hera-5.5.0/src/hera/events/models/io/argoproj/events/v1alpha1.pyi
+-rw-r--r--   0        0        0      144 2023-06-20 21:13:16.674984 hera-5.5.0/src/hera/events/models/io/argoproj/workflow/__init__.py
+-rw-r--r--   0        0        0   144549 2023-06-20 21:13:16.674984 hera-5.5.0/src/hera/events/models/io/argoproj/workflow/v1alpha1.py
+-rw-r--r--   0        0        0    31958 2023-06-20 21:13:16.674984 hera-5.5.0/src/hera/events/models/io/argoproj/workflow/v1alpha1.pyi
+-rw-r--r--   0        0        0        0 2023-06-20 21:13:16.674984 hera-5.5.0/src/hera/events/models/io/k8s/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 21:13:16.674984 hera-5.5.0/src/hera/events/models/io/k8s/api/__init__.py
+-rw-r--r--   0        0        0      144 2023-06-20 21:13:16.674984 hera-5.5.0/src/hera/events/models/io/k8s/api/core/__init__.py
+-rw-r--r--   0        0        0   127883 2023-06-20 21:13:16.674984 hera-5.5.0/src/hera/events/models/io/k8s/api/core/v1.py
+-rw-r--r--   0        0        0    18004 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/events/models/io/k8s/api/core/v1.pyi
+-rw-r--r--   0        0        0      144 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/events/models/io/k8s/api/policy/__init__.py
+-rw-r--r--   0        0        0     1751 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/events/models/io/k8s/api/policy/v1beta1.py
+-rw-r--r--   0        0        0      376 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/events/models/io/k8s/api/policy/v1beta1.pyi
+-rw-r--r--   0        0        0        0 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/events/models/io/k8s/apimachinery/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/events/models/io/k8s/apimachinery/pkg/__init__.py
+-rw-r--r--   0        0        0      144 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/events/models/io/k8s/apimachinery/pkg/api/__init__.py
+-rw-r--r--   0        0        0     3161 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.py
+-rw-r--r--   0        0        0      105 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.pyi
+-rw-r--r--   0        0        0        0 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/events/models/io/k8s/apimachinery/pkg/apis/__init__.py
+-rw-r--r--   0        0        0      144 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/__init__.py
+-rw-r--r--   0        0        0    22218 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.py
+-rw-r--r--   0        0        0     2064 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi
+-rw-r--r--   0        0        0      144 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/events/models/io/k8s/apimachinery/pkg/util/__init__.py
+-rw-r--r--   0        0        0      277 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/events/models/io/k8s/apimachinery/pkg/util/intstr.py
+-rw-r--r--   0        0        0      108 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/events/models/io/k8s/apimachinery/pkg/util/intstr.pyi
+-rw-r--r--   0        0        0     1453 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/events/models/sensor.py
+-rw-r--r--   0        0        0      887 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/events/models/sensor.pyi
+-rw-r--r--   0        0        0    27607 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/events/service.py
+-rw-r--r--   0        0        0     2186 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/exceptions/__init__.py
+-rw-r--r--   0        0        0      282 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/expr/__init__.py
+-rw-r--r--   0        0        0    12021 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/expr/_node.py
+-rw-r--r--   0        0        0      647 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/expr/_sprig.py
+-rw-r--r--   0        0        0        0 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/py.typed
+-rw-r--r--   0        0        0      188 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/shared/__init__.py
+-rw-r--r--   0        0        0      269 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/shared/_base_model.py
+-rw-r--r--   0        0        0     4997 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/shared/_global_config.py
+-rw-r--r--   0        0        0      513 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/shared/serialization.py
+-rw-r--r--   0        0        0     4585 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/workflows/__init__.py
+-rw-r--r--   0        0        0     2912 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/workflows/_context.py
+-rw-r--r--   0        0        0     4741 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/workflows/_inspect.py
+-rw-r--r--   0        0        0    41532 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/workflows/_mixins.py
+-rw-r--r--   0        0        0    32815 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/workflows/_unparse.py
+-rw-r--r--   0        0        0       25 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/workflows/action.py
+-rw-r--r--   0        0        0     1115 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/workflows/archive.py
+-rw-r--r--   0        0        0     7697 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/workflows/artifact.py
+-rw-r--r--   0        0        0     3640 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/workflows/cluster_workflow_template.py
+-rw-r--r--   0        0        0     3464 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/workflows/container.py
+-rw-r--r--   0        0        0     7280 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/workflows/container_set.py
+-rw-r--r--   0        0        0     9088 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/workflows/cron_workflow.py
+-rw-r--r--   0        0        0     2877 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/workflows/dag.py
+-rw-r--r--   0        0        0     2241 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/workflows/data.py
+-rw-r--r--   0        0        0     4855 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/workflows/env.py
+-rw-r--r--   0        0        0     1329 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/workflows/env_from.py
+-rw-r--r--   0        0        0      208 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/workflows/exceptions.py
+-rw-r--r--   0        0        0     2346 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/workflows/http_template.py
+-rw-r--r--   0        0        0       30 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/workflows/memoize.py
+-rw-r--r--   0        0        0     4418 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/workflows/metrics.py
+-rw-r--r--   0        0        0     6913 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/workflows/models/__init__.py
+-rw-r--r--   0        0        0     1418 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/workflows/models/eventsource.py
+-rw-r--r--   0        0        0      861 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/workflows/models/eventsource.pyi
+-rw-r--r--   0        0        0      144 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/workflows/models/google/__init__.py
+-rw-r--r--   0        0        0      347 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/workflows/models/google/protobuf.py
+-rw-r--r--   0        0        0      164 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/workflows/models/google/protobuf.pyi
+-rw-r--r--   0        0        0        0 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/workflows/models/grpc/__init__.py
+-rw-r--r--   0        0        0      144 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/workflows/models/grpc/gateway/__init__.py
+-rw-r--r--   0        0        0      691 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/workflows/models/grpc/gateway/runtime.py
+-rw-r--r--   0        0        0      470 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/workflows/models/grpc/gateway/runtime.pyi
+-rw-r--r--   0        0        0        0 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/workflows/models/io/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/workflows/models/io/argoproj/__init__.py
+-rw-r--r--   0        0        0      144 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/workflows/models/io/argoproj/events/__init__.py
+-rw-r--r--   0        0        0   102993 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/workflows/models/io/argoproj/events/v1alpha1.py
+-rw-r--r--   0        0        0    25271 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/workflows/models/io/argoproj/events/v1alpha1.pyi
+-rw-r--r--   0        0        0      144 2023-06-20 21:13:16.678984 hera-5.5.0/src/hera/workflows/models/io/argoproj/workflow/__init__.py
+-rw-r--r--   0        0        0   144549 2023-06-20 21:13:16.682984 hera-5.5.0/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.py
+-rw-r--r--   0        0        0    31958 2023-06-20 21:13:16.682984 hera-5.5.0/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.pyi
+-rw-r--r--   0        0        0        0 2023-06-20 21:13:16.682984 hera-5.5.0/src/hera/workflows/models/io/k8s/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 21:13:16.682984 hera-5.5.0/src/hera/workflows/models/io/k8s/api/__init__.py
+-rw-r--r--   0        0        0      144 2023-06-20 21:13:16.682984 hera-5.5.0/src/hera/workflows/models/io/k8s/api/core/__init__.py
+-rw-r--r--   0        0        0   127883 2023-06-20 21:13:16.682984 hera-5.5.0/src/hera/workflows/models/io/k8s/api/core/v1.py
+-rw-r--r--   0        0        0    18004 2023-06-20 21:13:16.682984 hera-5.5.0/src/hera/workflows/models/io/k8s/api/core/v1.pyi
+-rw-r--r--   0        0        0      144 2023-06-20 21:13:16.682984 hera-5.5.0/src/hera/workflows/models/io/k8s/api/policy/__init__.py
+-rw-r--r--   0        0        0     1751 2023-06-20 21:13:16.682984 hera-5.5.0/src/hera/workflows/models/io/k8s/api/policy/v1beta1.py
+-rw-r--r--   0        0        0      376 2023-06-20 21:13:16.682984 hera-5.5.0/src/hera/workflows/models/io/k8s/api/policy/v1beta1.pyi
+-rw-r--r--   0        0        0        0 2023-06-20 21:13:16.682984 hera-5.5.0/src/hera/workflows/models/io/k8s/apimachinery/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 21:13:16.682984 hera-5.5.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/__init__.py
+-rw-r--r--   0        0        0      144 2023-06-20 21:13:16.682984 hera-5.5.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/__init__.py
+-rw-r--r--   0        0        0     3161 2023-06-20 21:13:16.682984 hera-5.5.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.py
+-rw-r--r--   0        0        0      105 2023-06-20 21:13:16.682984 hera-5.5.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.pyi
+-rw-r--r--   0        0        0        0 2023-06-20 21:13:16.682984 hera-5.5.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/__init__.py
+-rw-r--r--   0        0        0      144 2023-06-20 21:13:16.682984 hera-5.5.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/__init__.py
+-rw-r--r--   0        0        0    22218 2023-06-20 21:13:16.682984 hera-5.5.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.py
+-rw-r--r--   0        0        0     2064 2023-06-20 21:13:16.682984 hera-5.5.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi
+-rw-r--r--   0        0        0      144 2023-06-20 21:13:16.682984 hera-5.5.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/__init__.py
+-rw-r--r--   0        0        0      277 2023-06-20 21:13:16.682984 hera-5.5.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/intstr.py
+-rw-r--r--   0        0        0      108 2023-06-20 21:13:16.682984 hera-5.5.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/intstr.pyi
+-rw-r--r--   0        0        0     1453 2023-06-20 21:13:16.682984 hera-5.5.0/src/hera/workflows/models/sensor.py
+-rw-r--r--   0        0        0      887 2023-06-20 21:13:16.682984 hera-5.5.0/src/hera/workflows/models/sensor.pyi
+-rw-r--r--   0        0        0      722 2023-06-20 21:13:16.682984 hera-5.5.0/src/hera/workflows/operator.py
+-rw-r--r--   0        0        0     4084 2023-06-20 21:13:16.682984 hera-5.5.0/src/hera/workflows/parameter.py
+-rw-r--r--   0        0        0     1076 2023-06-20 21:13:16.682984 hera-5.5.0/src/hera/workflows/protocol.py
+-rw-r--r--   0        0        0     3146 2023-06-20 21:13:16.682984 hera-5.5.0/src/hera/workflows/resource.py
+-rw-r--r--   0        0        0     5262 2023-06-20 21:13:16.682984 hera-5.5.0/src/hera/workflows/resources.py
+-rw-r--r--   0        0        0     1856 2023-06-20 21:13:16.682984 hera-5.5.0/src/hera/workflows/retry_strategy.py
+-rw-r--r--   0        0        0     3707 2023-06-20 21:13:16.682984 hera-5.5.0/src/hera/workflows/runner.py
+-rw-r--r--   0        0        0    16736 2023-06-20 21:13:16.682984 hera-5.5.0/src/hera/workflows/script.py
+-rw-r--r--   0        0        0    55301 2023-06-20 21:13:16.682984 hera-5.5.0/src/hera/workflows/service.py
+-rw-r--r--   0        0        0     6747 2023-06-20 21:13:16.682984 hera-5.5.0/src/hera/workflows/steps.py
+-rw-r--r--   0        0        0     3332 2023-06-20 21:13:16.682984 hera-5.5.0/src/hera/workflows/suspend.py
+-rw-r--r--   0        0        0     7959 2023-06-20 21:13:16.682984 hera-5.5.0/src/hera/workflows/task.py
+-rw-r--r--   0        0        0       27 2023-06-20 21:13:16.682984 hera-5.5.0/src/hera/workflows/toleration.py
+-rw-r--r--   0        0        0     2007 2023-06-20 21:13:16.682984 hera-5.5.0/src/hera/workflows/user_container.py
+-rw-r--r--   0        0        0     2610 2023-06-20 21:13:16.682984 hera-5.5.0/src/hera/workflows/validators.py
+-rw-r--r--   0        0        0    18709 2023-06-20 21:13:16.682984 hera-5.5.0/src/hera/workflows/volume.py
+-rw-r--r--   0        0        0    22337 2023-06-20 21:13:16.682984 hera-5.5.0/src/hera/workflows/workflow.py
+-rw-r--r--   0        0        0      911 2023-06-20 21:13:16.682984 hera-5.5.0/src/hera/workflows/workflow_status.py
+-rw-r--r--   0        0        0     7417 2023-06-20 21:13:16.682984 hera-5.5.0/src/hera/workflows/workflow_template.py
+-rw-r--r--   0        0        0    13556 1970-01-01 00:00:00.000000 hera-5.5.0/PKG-INFO
```

### Comparing `hera-5.4.1/LICENSE` & `hera-5.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/README.md` & `hera-5.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # Hera
 
+[See the Quick Start guide](https://hera.readthedocs.io/en/latest/getting-started/quick-start/) to start using Hera
+to orchestrate your Argo Workflows!
+
 ```text
 The Argo was constructed by the shipwright Argus,
 and its crew were specially protected by the goddess Hera.
 ```
 
 [![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/argoproj-labs/hera)
```

### Comparing `hera-5.4.1/pyproject.toml` & `hera-5.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "hera"  # project-name
 # The version is automatically substituted by the CI
-version = "5.4.1"
+version = "5.5.0"
 description = "Hera is a Python framework for constructing and submitting Argo Workflows. The main goal of Hera is to make Argo Workflows more accessible by abstracting away some setup that is typically necessary for constructing Argo workflows."
 authors = ["Flaviu Vadan <flaviu.vadan@dynotx.com>", "Sambhav Kothari <sambhavs.email@gmail.com>", "Elliot Gunton <elliotgunton@gmail.com>"]
 maintainers = ["Flaviu Vadan <flaviu.vadan@dynotx.com>", "Sambhav Kothari <sambhavs.email@gmail.com>", "Elliot Gunton <elliotgunton@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/argoproj-labs/hera"
 repository = "https://github.com/argoproj-labs/hera"
```

### Comparing `hera-5.4.1/src/hera/__init__.py` & `hera-5.5.0/src/hera/__init__.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/events/models/__init__.py` & `hera-5.5.0/src/hera/events/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/events/models/eventsource.py` & `hera-5.5.0/src/hera/events/models/eventsource.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/events/models/eventsource.pyi` & `hera-5.5.0/src/hera/events/models/eventsource.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/events/models/grpc/gateway/runtime.py` & `hera-5.5.0/src/hera/events/models/grpc/gateway/runtime.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/events/models/io/argoproj/events/v1alpha1.py` & `hera-5.5.0/src/hera/events/models/io/argoproj/events/v1alpha1.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/events/models/io/argoproj/events/v1alpha1.pyi` & `hera-5.5.0/src/hera/events/models/io/argoproj/events/v1alpha1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/events/models/io/argoproj/workflow/v1alpha1.py` & `hera-5.5.0/src/hera/events/models/io/argoproj/workflow/v1alpha1.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/events/models/io/argoproj/workflow/v1alpha1.pyi` & `hera-5.5.0/src/hera/events/models/io/argoproj/workflow/v1alpha1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/events/models/io/k8s/api/core/v1.py` & `hera-5.5.0/src/hera/events/models/io/k8s/api/core/v1.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/events/models/io/k8s/api/core/v1.pyi` & `hera-5.5.0/src/hera/events/models/io/k8s/api/core/v1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/events/models/io/k8s/api/policy/v1beta1.py` & `hera-5.5.0/src/hera/events/models/io/k8s/api/policy/v1beta1.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.py` & `hera-5.5.0/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.py` & `hera-5.5.0/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi` & `hera-5.5.0/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/events/models/sensor.py` & `hera-5.5.0/src/hera/events/models/sensor.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/events/models/sensor.pyi` & `hera-5.5.0/src/hera/events/models/sensor.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/events/service.py` & `hera-5.5.0/src/hera/events/service.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/exceptions/__init__.py` & `hera-5.5.0/src/hera/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/expr/_node.py` & `hera-5.5.0/src/hera/expr/_node.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/expr/_sprig.py` & `hera-5.5.0/src/hera/expr/_sprig.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/shared/_global_config.py` & `hera-5.5.0/src/hera/shared/_global_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import inspect
 from collections import defaultdict
 from dataclasses import dataclass, field
 from typing import Any, Callable, Dict, List, Optional, Type, TypeVar, Union
 
 from pydantic import root_validator
 
+from hera.auth import TokenGenerator
+
 from ._base_model import BaseModel
 
 TBase = TypeVar("TBase", bound="BaseMixin")
 TypeTBase = Type[TBase]
 
 Hook = Callable[[TBase], TBase]
 _HookMap = Dict[Type[TBase], List[Hook]]
@@ -24,25 +26,25 @@
     Notes:
         This should not be instantiated directly by the user. There is an instance of the `_GlobalConfig` in this module,
         which is what should be used. Access as `hera.shared.global_config` or `hera.shared.GlobalConfig`.
     """
 
     # protected attributes are ones that are computed/go through some light processing upon setting or
     # are processed upon accessing. The rest, which use primitive types, such as `str`, can remain public
-    _token: Union[Optional[str], Callable[[], Optional[str]]] = None
+    _token: Optional[Union[str, TokenGenerator, Callable[[], Optional[str]]]] = None
+    _image: Union[str, Callable[[], str]] = "python:3.8"
+    _pre_build_hooks: Optional[_HookMap] = None
+    _defaults: _Defaults = field(default_factory=lambda: defaultdict(dict))
 
     host: Optional[str] = None
     verify_ssl: bool = True
     api_version: str = "argoproj.io/v1alpha1"
     namespace: Optional[str] = None
-    _image: Union[str, Callable[[], str]] = "python:3.8"
     service_account_name: Optional[str] = None
     script_command: Optional[List[str]] = field(default_factory=lambda: ["python"])
-    _pre_build_hooks: Optional[_HookMap] = None
-    _defaults: _Defaults = field(default_factory=lambda: defaultdict(dict))
     experimental_features: Dict[str, bool] = field(default_factory=lambda: defaultdict(bool))
 
     def reset(self) -> None:
         """Resets the global config container to its initial state"""
         self.__dict__ = _GlobalConfig().__dict__
 
     @property
@@ -61,15 +63,15 @@
     def token(self) -> Optional[str]:
         """Returns an Argo Workflows global token"""
         if self._token is None or isinstance(self._token, str):
             return self._token
         return self._token()
 
     @token.setter
-    def token(self, t: Union[Optional[str], Callable[[], Optional[str]]]) -> None:
+    def token(self, t: Union[Optional[str], TokenGenerator, Callable[[], Optional[str]]]) -> None:
         """Sets the Argo Workflows token at a global level so services can use it"""
         self._token = t
 
     def register_pre_build_hook(self, hook: Hook) -> Hook:
         """Registers a hook to be called before building a model."""
         return_type = inspect.signature(hook).return_annotation
         if return_type is inspect.Signature.empty:
```

### Comparing `hera-5.4.1/src/hera/shared/serialization.py` & `hera-5.5.0/src/hera/shared/serialization.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/workflows/__init__.py` & `hera-5.5.0/src/hera/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/workflows/_context.py` & `hera-5.5.0/src/hera/workflows/_context.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/workflows/_mixins.py` & `hera-5.5.0/src/hera/workflows/_mixins.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,29 @@
 from __future__ import annotations
 
 import inspect
-from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Set, TypeVar, Union, cast
+from pathlib import Path
+
+try:
+    from inspect import get_annotations  # type: ignore
+except ImportError:
+    from hera.workflows._inspect import get_annotations  # type: ignore
+from collections import ChainMap
+from types import ModuleType
+from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Set, Type, TypeVar, Union, cast
+
+try:
+    from typing import Annotated, get_args, get_origin  # type: ignore
+except ImportError:
+    from typing_extensions import Annotated, get_args, get_origin  # type: ignore
 
 from pydantic import root_validator, validator
 
 from hera.shared import BaseMixin, global_config
+from hera.shared._base_model import BaseModel
 from hera.shared.serialization import serialize
 from hera.workflows._context import SubNodeMixin, _context
 from hera.workflows.artifact import Artifact
 from hera.workflows.env import Env, _BaseEnv
 from hera.workflows.env_from import _BaseEnvFrom
 from hera.workflows.exceptions import InvalidTemplateCall, InvalidType
 from hera.workflows.metrics import Metrics, _BaseMetric
@@ -50,23 +64,30 @@
     Toleration,
     UserContainer as ModelUserContainer,
     Volume as ModelVolume,
     VolumeDevice,
     VolumeMount,
 )
 from hera.workflows.parameter import MISSING, Parameter
-from hera.workflows.protocol import Templatable
+from hera.workflows.protocol import Templatable, TWorkflow
 from hera.workflows.resources import Resources
 from hera.workflows.user_container import UserContainer
 from hera.workflows.volume import Volume, _BaseVolume
 
 if TYPE_CHECKING:
     from hera.workflows.steps import Step
     from hera.workflows.task import Task
 
+_yaml: Optional[ModuleType] = None
+try:
+    import yaml
+
+    _yaml = yaml
+except ImportError:
+    _yaml = None
 
 InputsT = Optional[
     Union[
         ModelInputs,
         Union[Parameter, ModelParameter, Artifact, ModelArtifact, Dict[str, Any]],
         List[Union[Parameter, ModelParameter, Artifact, ModelArtifact, Dict[str, Any]]],
     ]
@@ -81,14 +102,24 @@
 ArgumentsT = Optional[
     Union[
         ModelArguments,
         Union[Parameter, ModelParameter, Artifact, ModelArtifact, Dict[str, Any]],
         List[Union[Parameter, ModelParameter, Artifact, ModelArtifact, Dict[str, Any]]],
     ]
 ]
+MetricsT = Optional[
+    Union[
+        _BaseMetric,
+        List[_BaseMetric],
+        Metrics,
+        ModelPrometheus,
+        List[ModelPrometheus],
+        ModelMetrics,
+    ]
+]
 EnvT = Optional[
     Union[
         _BaseEnv,
         EnvVar,
         List[Union[_BaseEnv, EnvVar, Dict[str, Any]]],
         Dict[str, Any],
     ]
@@ -140,20 +171,36 @@
     startup_probe: Optional[Probe] = None
     stdin: Optional[bool] = None
     stdin_once: Optional[bool] = None
     termination_message_path: Optional[str] = None
     termination_message_policy: Optional[TerminationMessagePolicy] = None
     tty: Optional[bool] = None
 
-    def _build_image_pull_policy(self) -> Optional[str]:
+    def _build_image_pull_policy(self) -> Optional[ImagePullPolicy]:
         if self.image_pull_policy is None:
             return None
         elif isinstance(self.image_pull_policy, ImagePullPolicy):
-            return self.image_pull_policy.value
-        return ImagePullPolicy[self.image_pull_policy.lower()].value
+            return self.image_pull_policy
+
+        # this helps map image pull policy values as a convenience
+        policy_mapper = {
+            # the following 2 are "normal" entries
+            **{ipp.name: ipp for ipp in ImagePullPolicy},
+            **{ipp.value: ipp for ipp in ImagePullPolicy},
+            # some users might submit the policy without underscores
+            **{ipp.value.lower().replace("_", ""): ipp for ipp in ImagePullPolicy},
+            # some users might submit the policy in lowercase
+            **{ipp.name.lower(): ipp for ipp in ImagePullPolicy},
+        }
+        try:
+            return ImagePullPolicy[policy_mapper[self.image_pull_policy].name]
+        except KeyError as e:
+            raise KeyError(
+                f"Supplied image policy {self.image_pull_policy} is not valid. Use one of {ImagePullPolicy.__members__}"
+            ) from e
 
     @validator("image", pre=True, always=True)
     def _set_image(cls, v):
         if v is None:
             return global_config.image
         return v
 
@@ -274,24 +321,15 @@
                     else params + [Parameter(name=spec.param_name, value=value)]
                 )
 
         return params
 
 
 class MetricsMixin(BaseMixin):
-    metrics: Optional[
-        Union[
-            _BaseMetric,
-            List[_BaseMetric],
-            Metrics,
-            ModelPrometheus,
-            List[ModelPrometheus],
-            ModelMetrics,
-        ]
-    ] = None
+    metrics: MetricsT = None
 
     def _build_metrics(self) -> Optional[ModelMetrics]:
         if self.metrics is None or isinstance(self.metrics, ModelMetrics):
             return self.metrics
         elif isinstance(self.metrics, ModelPrometheus):
             return ModelMetrics(prometheus=[self.metrics])
         elif isinstance(self.metrics, Metrics):
@@ -894,14 +932,138 @@
         if len(el.keys()) == 1:
             return [Parameter(name=n, value="{{item}}") for n in el.keys()]
         else:
             return [Parameter(name=n, value=f"{{{{item.{n}}}}}") for n in el.keys()]
     return [Parameter(name=n, value=f"{{{{item.{n}}}}}") for n in with_items[0].keys()]
 
 
+def _set_model_attr(model: BaseModel, attrs: List[str], value: Any):
+    # The `attrs` list represents a path to an attribute in `model`, whose attributes
+    # are BaseModels themselves. Therefore we use `getattr` to get a reference to the final
+    # BaseModel set to `curr`, then call `setattr` on that BaseModel, using the last attribute
+    # name in attrs, and the value passed in.
+    curr: BaseModel = model
+    for attr in attrs[:-1]:
+        curr = getattr(curr, attr)
+
+    setattr(curr, attrs[-1], value)
+
+
+def _get_model_attr(model: BaseModel, attrs: List[str]) -> Any:
+    # This is almost the same as _set_model_attr.
+    # The `attrs` list represents a path to an attribute in `model`, whose attributes
+    # are BaseModels themselves. Therefore we use `getattr` to get a reference to the final
+    # BaseModel set to `curr`, then `getattr` on that BaseModel, using the last attribute
+    # name in attrs.
+    curr: BaseModel = model
+    for attr in attrs[:-1]:
+        curr = getattr(curr, attr)
+
+    return getattr(curr, attrs[-1])
+
+
+class ModelMapperMixin(BaseMixin):
+    class ModelMapper:
+        def __init__(self, model_path: str, hera_builder: Optional[Callable] = None):
+            self.model_path = None
+            self.builder = hera_builder
+
+            if not model_path:
+                # Allows overriding parent attribute annotations to remove the mapping
+                return
+
+            self.model_path = model_path.split(".")
+            curr_class: Type[BaseModel] = self._get_model_class()
+            for key in self.model_path:
+                if key not in curr_class.__fields__:
+                    raise ValueError(f"Model key '{key}' does not exist in class {curr_class}")
+                curr_class = curr_class.__fields__[key].outer_type_
+
+        @classmethod
+        def _get_model_class(cls) -> Type[BaseModel]:
+            raise NotImplementedError
+
+        @classmethod
+        def build_model(
+            cls, hera_class: Type[ModelMapperMixin], hera_obj: ModelMapperMixin, model: TWorkflow
+        ) -> TWorkflow:
+            assert isinstance(hera_obj, ModelMapperMixin)
+
+            for attr, annotation in hera_class._get_all_annotations().items():
+                if get_origin(annotation) is Annotated and isinstance(
+                    get_args(annotation)[1], ModelMapperMixin.ModelMapper
+                ):
+                    mapper = get_args(annotation)[1]
+                    # Value comes from builder function if it exists on hera_obj, otherwise directly from the attr
+                    value = (
+                        getattr(hera_obj, mapper.builder.__name__)()
+                        if mapper.builder is not None
+                        else getattr(hera_obj, attr)
+                    )
+                    if value is not None:
+                        _set_model_attr(model, mapper.model_path, value)
+
+            return model
+
+    @classmethod
+    def _get_all_annotations(cls) -> ChainMap:
+        """Gets all annotations of this class and any parent classes."""
+        return ChainMap(*(get_annotations(c) for c in cls.__mro__))
+
+    @classmethod
+    def _from_model(cls, model: BaseModel) -> ModelMapperMixin:
+        """Parse from given model to cls's type."""
+        hera_obj = cls()
+
+        for attr, annotation in cls._get_all_annotations().items():
+            if get_origin(annotation) is Annotated and isinstance(
+                get_args(annotation)[1], ModelMapperMixin.ModelMapper
+            ):
+                mapper = get_args(annotation)[1]
+                if mapper.model_path:
+                    value = _get_model_attr(model, mapper.model_path)
+                    if value is not None:
+                        setattr(hera_obj, attr, value)
+
+        return hera_obj
+
+    @classmethod
+    def _from_dict(cls, model_dict: Dict, model: Type[BaseModel]) -> ModelMapperMixin:
+        """Parse from given model_dict, using the given model type to call its parse_obj."""
+        model_workflow = model.parse_obj(model_dict)
+        return cls._from_model(model_workflow)
+
+    @classmethod
+    def from_dict(cls, model_dict: Dict) -> ModelMapperMixin:
+        """Parse from given model_dict."""
+        raise NotImplementedError
+
+    @classmethod
+    def _from_yaml(cls, yaml_str: str, model: Type[BaseModel]) -> ModelMapperMixin:
+        """Parse from given yaml string, using the given model type to call its parse_obj."""
+        if not _yaml:
+            raise ImportError("PyYAML is not installed")
+        return cls._from_dict(_yaml.safe_load(yaml_str), model)
+
+    @classmethod
+    def from_yaml(cls, yaml_str: str) -> ModelMapperMixin:
+        """Parse from given yaml_str."""
+        raise NotImplementedError
+
+    @classmethod
+    def _from_file(cls, yaml_file: Union[Path, str], model: Type[BaseModel]) -> ModelMapperMixin:
+        yaml_file = Path(yaml_file)
+        return cls._from_yaml(yaml_file.read_text(encoding="utf-8"), model)
+
+    @classmethod
+    def from_file(cls, yaml_file: Union[Path, str]) -> ModelMapperMixin:
+        """Parse from given yaml_file."""
+        raise NotImplementedError
+
+
 class ExperimentalMixin(BaseMixin):
     _experimental_warning_message: str = (
         "Unable to instantiate {} since it is an experimental feature."
         ' Please turn on experimental features by setting `hera.shared.global_config.experimental_features["{}"] = True`.'
         " Note that experimental features are unstable and subject to breaking changes."
     )
```

### Comparing `hera-5.4.1/src/hera/workflows/_unparse.py` & `hera-5.5.0/src/hera/workflows/_unparse.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/workflows/archive.py` & `hera-5.5.0/src/hera/workflows/archive.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/workflows/artifact.py` & `hera-5.5.0/src/hera/workflows/artifact.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/workflows/container.py` & `hera-5.5.0/src/hera/workflows/container.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/workflows/container_set.py` & `hera-5.5.0/src/hera/workflows/container_set.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/workflows/dag.py` & `hera-5.5.0/src/hera/workflows/dag.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/workflows/data.py` & `hera-5.5.0/src/hera/workflows/data.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/workflows/env.py` & `hera-5.5.0/src/hera/workflows/env.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/workflows/env_from.py` & `hera-5.5.0/src/hera/workflows/env_from.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/workflows/http_template.py` & `hera-5.5.0/src/hera/workflows/http_template.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/workflows/metrics.py` & `hera-5.5.0/src/hera/workflows/metrics.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/workflows/models/__init__.py` & `hera-5.5.0/src/hera/workflows/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/workflows/models/eventsource.py` & `hera-5.5.0/src/hera/workflows/models/eventsource.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/workflows/models/eventsource.pyi` & `hera-5.5.0/src/hera/workflows/models/eventsource.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/workflows/models/grpc/gateway/runtime.py` & `hera-5.5.0/src/hera/workflows/models/grpc/gateway/runtime.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/workflows/models/io/argoproj/events/v1alpha1.py` & `hera-5.5.0/src/hera/workflows/models/io/argoproj/events/v1alpha1.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/workflows/models/io/argoproj/events/v1alpha1.pyi` & `hera-5.5.0/src/hera/workflows/models/io/argoproj/events/v1alpha1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.py` & `hera-5.5.0/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.pyi` & `hera-5.5.0/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/workflows/models/io/k8s/api/core/v1.py` & `hera-5.5.0/src/hera/workflows/models/io/k8s/api/core/v1.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/workflows/models/io/k8s/api/core/v1.pyi` & `hera-5.5.0/src/hera/workflows/models/io/k8s/api/core/v1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/workflows/models/io/k8s/api/policy/v1beta1.py` & `hera-5.5.0/src/hera/workflows/models/io/k8s/api/policy/v1beta1.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.py` & `hera-5.5.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.py` & `hera-5.5.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi` & `hera-5.5.0/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/workflows/models/sensor.py` & `hera-5.5.0/src/hera/workflows/models/sensor.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/workflows/models/sensor.pyi` & `hera-5.5.0/src/hera/workflows/models/sensor.pyi`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/workflows/operator.py` & `hera-5.5.0/src/hera/workflows/operator.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/workflows/parameter.py` & `hera-5.5.0/src/hera/workflows/parameter.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/workflows/protocol.py` & `hera-5.5.0/src/hera/workflows/protocol.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Any, List, Optional, Union
 
 from typing_extensions import Protocol, runtime_checkable
 
 from hera.workflows.models import (
+    ClusterWorkflowTemplate,
     ContainerSetTemplate,
     CronWorkflow,
     DAGTemplate,
     PersistentVolumeClaim,
     ResourceTemplate,
     ScriptTemplate,
     SuspendTemplate,
@@ -22,14 +23,15 @@
     ScriptTemplate,
     SuspendTemplate,
     Template,
 ]
 
 TWorkflow = Union[
     CronWorkflow,
+    ClusterWorkflowTemplate,
     Workflow,
     WorkflowTemplate,
 ]
 
 
 @runtime_checkable
 class Templatable(Protocol):
```

### Comparing `hera-5.4.1/src/hera/workflows/resource.py` & `hera-5.5.0/src/hera/workflows/resource.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/workflows/resources.py` & `hera-5.5.0/src/hera/workflows/resources.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/workflows/retry_strategy.py` & `hera-5.5.0/src/hera/workflows/retry_strategy.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/workflows/runner.py` & `hera-5.5.0/src/hera/workflows/runner.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/workflows/script.py` & `hera-5.5.0/src/hera/workflows/script.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,23 +190,26 @@
                 tolerations=self.tolerations,
                 volumes=self._build_volumes(),
             ),
         )
 
     def _build_script(self) -> _ModelScriptTemplate:
         assert isinstance(self.constructor, ScriptConstructor)
+        image_pull_policy = self._build_image_pull_policy()
+
         return self.constructor.transform_script_template_post_build(
             self,
             _ModelScriptTemplate(
                 args=self.args,
                 command=self.command,
                 env=self._build_env(),
                 env_from=self._build_env_from(),
                 image=self.image,
-                image_pull_policy=self._build_image_pull_policy(),
+                # `image_pull_policy` in script wants a string not an `ImagePullPolicy` object
+                image_pull_policy=None if image_pull_policy is None else image_pull_policy.value,
                 lifecycle=self.lifecycle,
                 liveness_probe=self.liveness_probe,
                 name=self.container_name,
                 ports=self.ports,
                 readiness_probe=self.readiness_probe,
                 resources=self._build_resources(),
                 security_context=self.security_context,
```

### Comparing `hera-5.4.1/src/hera/workflows/service.py` & `hera-5.5.0/src/hera/workflows/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -392,17 +392,17 @@
             verify=self.verify_ssl,
         )
 
         if resp.ok:
             resp_json = resp.json()
             if (
                 "status" in resp_json
-                and resp_json["status"]["active"] is None
-                and resp_json["status"]["lastScheduledTime"] is None
-                and resp_json["status"]["conditions"] is None
+                or resp_json["status"]["active"] is None
+                or resp_json["status"]["lastScheduledTime"] is None
+                or resp_json["status"]["conditions"] is None
             ):
                 # this is a necessary special case as the status fields cannot be empty on the `CronWorkflowStatus`
                 # object. So, we overwrite the response with a value that allows the response to pass through safely.
                 # See `hera.scripts.service.ServiceEndpoint.__str__` for more details.
                 resp_json["status"] = None
             return CronWorkflowList(**resp_json)
 
@@ -422,17 +422,17 @@
             verify=self.verify_ssl,
         )
 
         if resp.ok:
             resp_json = resp.json()
             if (
                 "status" in resp_json
-                and resp_json["status"]["active"] is None
-                and resp_json["status"]["lastScheduledTime"] is None
-                and resp_json["status"]["conditions"] is None
+                or resp_json["status"]["active"] is None
+                or resp_json["status"]["lastScheduledTime"] is None
+                or resp_json["status"]["conditions"] is None
             ):
                 # this is a necessary special case as the status fields cannot be empty on the `CronWorkflowStatus`
                 # object. So, we overwrite the response with a value that allows the response to pass through safely.
                 # See `hera.scripts.service.ServiceEndpoint.__str__` for more details.
                 resp_json["status"] = None
             return CronWorkflow(**resp_json)
 
@@ -452,17 +452,17 @@
             verify=self.verify_ssl,
         )
 
         if resp.ok:
             resp_json = resp.json()
             if (
                 "status" in resp_json
-                and resp_json["status"]["active"] is None
-                and resp_json["status"]["lastScheduledTime"] is None
-                and resp_json["status"]["conditions"] is None
+                or resp_json["status"]["active"] is None
+                or resp_json["status"]["lastScheduledTime"] is None
+                or resp_json["status"]["conditions"] is None
             ):
                 # this is a necessary special case as the status fields cannot be empty on the `CronWorkflowStatus`
                 # object. So, we overwrite the response with a value that allows the response to pass through safely.
                 # See `hera.scripts.service.ServiceEndpoint.__str__` for more details.
                 resp_json["status"] = None
             return CronWorkflow(**resp_json)
 
@@ -482,17 +482,17 @@
             verify=self.verify_ssl,
         )
 
         if resp.ok:
             resp_json = resp.json()
             if (
                 "status" in resp_json
-                and resp_json["status"]["active"] is None
-                and resp_json["status"]["lastScheduledTime"] is None
-                and resp_json["status"]["conditions"] is None
+                or resp_json["status"]["active"] is None
+                or resp_json["status"]["lastScheduledTime"] is None
+                or resp_json["status"]["conditions"] is None
             ):
                 # this is a necessary special case as the status fields cannot be empty on the `CronWorkflowStatus`
                 # object. So, we overwrite the response with a value that allows the response to pass through safely.
                 # See `hera.scripts.service.ServiceEndpoint.__str__` for more details.
                 resp_json["status"] = None
             return CronWorkflow(**resp_json)
 
@@ -514,17 +514,17 @@
             verify=self.verify_ssl,
         )
 
         if resp.ok:
             resp_json = resp.json()
             if (
                 "status" in resp_json
-                and resp_json["status"]["active"] is None
-                and resp_json["status"]["lastScheduledTime"] is None
-                and resp_json["status"]["conditions"] is None
+                or resp_json["status"]["active"] is None
+                or resp_json["status"]["lastScheduledTime"] is None
+                or resp_json["status"]["conditions"] is None
             ):
                 # this is a necessary special case as the status fields cannot be empty on the `CronWorkflowStatus`
                 # object. So, we overwrite the response with a value that allows the response to pass through safely.
                 # See `hera.scripts.service.ServiceEndpoint.__str__` for more details.
                 resp_json["status"] = None
             return CronWorkflow(**resp_json)
 
@@ -580,17 +580,17 @@
             verify=self.verify_ssl,
         )
 
         if resp.ok:
             resp_json = resp.json()
             if (
                 "status" in resp_json
-                and resp_json["status"]["active"] is None
-                and resp_json["status"]["lastScheduledTime"] is None
-                and resp_json["status"]["conditions"] is None
+                or resp_json["status"]["active"] is None
+                or resp_json["status"]["lastScheduledTime"] is None
+                or resp_json["status"]["conditions"] is None
             ):
                 # this is a necessary special case as the status fields cannot be empty on the `CronWorkflowStatus`
                 # object. So, we overwrite the response with a value that allows the response to pass through safely.
                 # See `hera.scripts.service.ServiceEndpoint.__str__` for more details.
                 resp_json["status"] = None
             return CronWorkflow(**resp_json)
 
@@ -612,17 +612,17 @@
             verify=self.verify_ssl,
         )
 
         if resp.ok:
             resp_json = resp.json()
             if (
                 "status" in resp_json
-                and resp_json["status"]["active"] is None
-                and resp_json["status"]["lastScheduledTime"] is None
-                and resp_json["status"]["conditions"] is None
+                or resp_json["status"]["active"] is None
+                or resp_json["status"]["lastScheduledTime"] is None
+                or resp_json["status"]["conditions"] is None
             ):
                 # this is a necessary special case as the status fields cannot be empty on the `CronWorkflowStatus`
                 # object. So, we overwrite the response with a value that allows the response to pass through safely.
                 # See `hera.scripts.service.ServiceEndpoint.__str__` for more details.
                 resp_json["status"] = None
             return CronWorkflow(**resp_json)
```

### Comparing `hera-5.4.1/src/hera/workflows/steps.py` & `hera-5.5.0/src/hera/workflows/steps.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/workflows/suspend.py` & `hera-5.5.0/src/hera/workflows/suspend.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/workflows/task.py` & `hera-5.5.0/src/hera/workflows/task.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/workflows/user_container.py` & `hera-5.5.0/src/hera/workflows/user_container.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/workflows/validators.py` & `hera-5.5.0/src/hera/workflows/validators.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/workflows/volume.py` & `hera-5.5.0/src/hera/workflows/volume.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/workflows/workflow_status.py` & `hera-5.5.0/src/hera/workflows/workflow_status.py`

 * *Files identical despite different names*

### Comparing `hera-5.4.1/src/hera/workflows/workflow_template.py` & `hera-5.5.0/src/hera/workflows/workflow_template.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,53 @@
 """The workflow_template module provides the WorkflowTemplate class
 
 See https://argoproj.github.io/argo-workflows/workflow-templates/
 for more on WorkflowTemplates.
 """
+from pathlib import Path
+from typing import Dict, Optional, Type, Union
+
+try:
+    from typing import Annotated  # type: ignore
+except ImportError:
+    from typing_extensions import Annotated  # type: ignore
+
 from pydantic import validator
 
 from hera.exceptions import NotFound
+from hera.shared._base_model import BaseModel
+from hera.workflows._mixins import ModelMapperMixin
 from hera.workflows.models import (
     ObjectMeta,
     WorkflowSpec as _ModelWorkflowSpec,
+    WorkflowStatus as _ModelWorkflowStatus,
     WorkflowTemplate as _ModelWorkflowTemplate,
     WorkflowTemplateCreateRequest,
     WorkflowTemplateLintRequest,
     WorkflowTemplateUpdateRequest,
 )
 from hera.workflows.protocol import TWorkflow
-from hera.workflows.workflow import Workflow
+from hera.workflows.workflow import _TRUNCATE_LENGTH, Workflow, _WorkflowModelMapper
+
+
+class _WorkflowTemplateModelMapper(_WorkflowModelMapper):
+    @classmethod
+    def _get_model_class(cls) -> Type[BaseModel]:
+        return _ModelWorkflowTemplate  # type: ignore
 
 
 class WorkflowTemplate(Workflow):
-    """WorkflowTemplates are definitions of Workflows that live in your cluster. This allows you
-    to create a library of frequently-used templates and reuse them by referencing them from your
-    Workflows.
+    """WorkflowTemplates are definitions of Workflows that live in your namespace in your cluster.
+    This allows you to create a library of frequently-used templates and reuse them by referencing
+    them from your Workflows.
     """
 
+    # Removes status mapping
+    status: Annotated[Optional[_ModelWorkflowStatus], _WorkflowTemplateModelMapper("")] = None
+
     # WorkflowTemplate fields match Workflow exactly except for `status`, which WorkflowTemplate
     # does not have - https://argoproj.github.io/argo-workflows/fields/#workflowtemplate
     @validator("status", pre=True, always=True)
     def _set_status(cls, v):
         if v is not None:
             raise ValueError("status is not a valid field on a WorkflowTemplate")
 
@@ -79,79 +99,79 @@
             WorkflowTemplateLintRequest(template=self.build()), namespace=self.namespace
         )
 
     def build(self) -> TWorkflow:
         """Builds the WorkflowTemplate and its components into an Argo schema WorkflowTemplate object."""
         self = self._dispatch_hooks()
 
-        templates = self._build_templates()
-        workflow_claims = self._build_persistent_volume_claims()
-        volume_claim_templates = (self.volume_claim_templates or []) + (workflow_claims or [])
-        return _ModelWorkflowTemplate(
-            api_version=self.api_version,
-            kind=self.kind,
-            metadata=ObjectMeta(
-                annotations=self.annotations,
-                cluster_name=self.cluster_name,
-                creation_timestamp=self.creation_timestamp,
-                deletion_grace_period_seconds=self.deletion_grace_period_seconds,
-                deletion_timestamp=self.deletion_timestamp,
-                finalizers=self.finalizers,
-                generate_name=self.generate_name,
-                generation=self.generation,
-                labels=self.labels,
-                managed_fields=self.managed_fields,
-                name=self.name,
-                namespace=self.namespace,
-                owner_references=self.owner_references,
-                resource_version=self.resource_version,
-                self_link=self.self_link,
-                uid=self.uid,
-            ),
-            spec=_ModelWorkflowSpec(
-                active_deadline_seconds=self.active_deadline_seconds,
-                affinity=self.affinity,
-                archive_logs=self.archive_logs,
-                arguments=self._build_arguments(),
-                artifact_gc=self.artifact_gc,
-                artifact_repository_ref=self.artifact_repository_ref,
-                automount_service_account_token=self.automount_service_account_token,
-                dns_config=self.dns_config,
-                dns_policy=self.dns_policy,
-                entrypoint=self.entrypoint,
-                executor=self.executor,
-                hooks=self.hooks,
-                host_aliases=self.host_aliases,
-                host_network=self.host_network,
-                image_pull_secrets=self.image_pull_secrets,
-                metrics=self._build_metrics(),
-                node_selector=self.node_selector,
-                on_exit=self._build_on_exit(),
-                parallelism=self.parallelism,
-                pod_disruption_budget=self.pod_disruption_budget,
-                pod_gc=self.pod_gc,
-                pod_metadata=self.pod_metadata,
-                pod_priority=self.pod_priority,
-                pod_priority_class_name=self.pod_priority_class_name,
-                pod_spec_patch=self.pod_spec_patch,
-                priority=self.priority,
-                retry_strategy=self.retry_strategy,
-                scheduler_name=self.scheduler_name,
-                security_context=self.security_context,
-                service_account_name=self.service_account_name,
-                shutdown=self.shutdown,
-                suspend=self.suspend,
-                synchronization=self.synchronization,
-                template_defaults=self.template_defaults,
-                templates=templates or None,
-                tolerations=self.tolerations,
-                ttl_strategy=self.ttl_strategy,
-                volume_claim_gc=self.volume_claim_gc,
-                volume_claim_templates=volume_claim_templates or None,
-                volumes=self._build_volumes(),
-                workflow_metadata=self.workflow_metadata,
-                workflow_template_ref=self.workflow_template_ref,
-            ),
+        model_workflow = _ModelWorkflowTemplate(
+            metadata=ObjectMeta(),
+            spec=_ModelWorkflowSpec(),
         )
 
+        return _WorkflowTemplateModelMapper.build_model(WorkflowTemplate, self, model_workflow)
+
+    @classmethod
+    def from_dict(cls, model_dict: Dict) -> ModelMapperMixin:
+        """Create a WorkflowTemplate from a WorkflowTemplate contained in a dict.
+
+        Examples:
+            my_workflow_template = WorkflowTemplate(...)
+            my_workflow_template == WorkflowTemplate.from_dict(my_workflow_template.to_dict())
+        """
+        return cls._from_dict(model_dict, _ModelWorkflowTemplate)
+
+    @classmethod
+    def from_yaml(cls, yaml_str: str) -> ModelMapperMixin:
+        """Create a WorkflowTemplate from a WorkflowTemplate contained in a YAML string.
+
+        Usage:
+            my_workflow_template = WorkflowTemplate.from_yaml(yaml_str)
+        """
+        return cls._from_yaml(yaml_str, _ModelWorkflowTemplate)
+
+    @classmethod
+    def from_file(cls, yaml_file: Union[Path, str]) -> ModelMapperMixin:
+        """Create a WorkflowTemplate from a WorkflowTemplate contained in a YAML file.
+
+        Usage:
+            yaml_file = Path(...)
+            my_workflow_template = WorkflowTemplate.from_file(yaml_file)
+        """
+        return cls._from_file(yaml_file, _ModelWorkflowTemplate)
+
+    def _get_as_workflow(self, generate_name: Optional[str]) -> Workflow:
+        workflow = Workflow(**self.dict())
+        workflow.kind = "Workflow"
+
+        if generate_name is not None:
+            workflow.generate_name = generate_name
+        else:
+            # As this function is mainly for improved DevEx when iterating on a WorkflowTemplate, we do a basic
+            # truncation of the WT's name in case it being > _TRUNCATE_LENGTH, to assign to generate_name.
+            assert workflow.name is not None
+            workflow.generate_name = workflow.name[:_TRUNCATE_LENGTH]
+
+        workflow.name = None
+
+        return workflow
+
+    def create_as_workflow(
+        self,
+        generate_name: Optional[str] = None,
+        wait: bool = False,
+        poll_interval: int = 5,
+    ) -> TWorkflow:
+        """Run this WorkflowTemplate instantly as a Workflow.
+
+        If generate_name is given, the workflow created uses generate_name as a prefix, as per the usual for
+        hera.workflows.Workflow.generate_name. If not given, the WorkflowTemplate's name will be used, truncated to 57
+        chars and appended with a hyphen.
+
+        Note: this function does not require the WorkflowTemplate to already exist on the cluster
+        """
+
+        workflow = self._get_as_workflow(generate_name)
+        return workflow.create(wait=wait, poll_interval=poll_interval)
+
 
 __all__ = ["WorkflowTemplate"]
```

### Comparing `hera-5.4.1/PKG-INFO` & `hera-5.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hera
-Version: 5.4.1
+Version: 5.5.0
 Summary: Hera is a Python framework for constructing and submitting Argo Workflows. The main goal of Hera is to make Argo Workflows more accessible by abstracting away some setup that is typically necessary for constructing Argo workflows.
 Home-page: https://github.com/argoproj-labs/hera
 License: MIT
 Author: Flaviu Vadan
 Author-email: flaviu.vadan@dynotx.com
 Maintainer: Flaviu Vadan
 Maintainer-email: flaviu.vadan@dynotx.com
@@ -27,14 +27,17 @@
 Project-URL: Bug Tracker, https://github.com/argoproj-labs/hera/issues
 Project-URL: Documentation, https://github.com/argoproj-labs/hera/README.md
 Project-URL: Repository, https://github.com/argoproj-labs/hera
 Description-Content-Type: text/markdown
 
 # Hera
 
+[See the Quick Start guide](https://hera.readthedocs.io/en/latest/getting-started/quick-start/) to start using Hera
+to orchestrate your Argo Workflows!
+
 ```text
 The Argo was constructed by the shipwright Argus,
 and its crew were specially protected by the goddess Hera.
 ```
 
 [![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/argoproj-labs/hera)
```

