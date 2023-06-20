# Comparing `tmp/prometheus-summary-0.1.1.tar.gz` & `tmp/prometheus-summary-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prometheus-summary-0.1.1.tar", last modified: Mon Jun 12 14:01:54 2023, max compression
+gzip compressed data, was "prometheus-summary-0.1.2.tar", last modified: Tue Jun 20 07:40:13 2023, max compression
```

## Comparing `prometheus-summary-0.1.1.tar` & `prometheus-summary-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:01:54.606931 prometheus-summary-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-12 14:01:38.000000 prometheus-summary-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-06-12 14:01:54.606931 prometheus-summary-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-12 14:01:38.000000 prometheus-summary-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:01:54.606931 prometheus-summary-0.1.1/prometheus_summary/
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-06-12 14:01:38.000000 prometheus-summary-0.1.1/prometheus_summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-12 14:01:38.000000 prometheus-summary-0.1.1/prometheus_summary/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:01:54.606931 prometheus-summary-0.1.1/prometheus_summary.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-06-12 14:01:54.000000 prometheus-summary-0.1.1/prometheus_summary.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-12 14:01:54.000000 prometheus-summary-0.1.1/prometheus_summary.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 14:01:54.000000 prometheus-summary-0.1.1/prometheus_summary.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-12 14:01:54.000000 prometheus-summary-0.1.1/prometheus_summary.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-12 14:01:54.000000 prometheus-summary-0.1.1/prometheus_summary.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 14:01:54.606931 prometheus-summary-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-12 14:01:38.000000 prometheus-summary-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:40:13.878136 prometheus-summary-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-20 07:40:02.000000 prometheus-summary-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-06-20 07:40:13.878136 prometheus-summary-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-06-20 07:40:02.000000 prometheus-summary-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:40:13.878136 prometheus-summary-0.1.2/prometheus_summary/
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-20 07:40:02.000000 prometheus-summary-0.1.2/prometheus_summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 07:40:02.000000 prometheus-summary-0.1.2/prometheus_summary/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:40:13.878136 prometheus-summary-0.1.2/prometheus_summary.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-06-20 07:40:13.000000 prometheus-summary-0.1.2/prometheus_summary.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-20 07:40:13.000000 prometheus-summary-0.1.2/prometheus_summary.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 07:40:13.000000 prometheus-summary-0.1.2/prometheus_summary.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-20 07:40:13.000000 prometheus-summary-0.1.2/prometheus_summary.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-20 07:40:13.000000 prometheus-summary-0.1.2/prometheus_summary.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 07:40:13.878136 prometheus-summary-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-20 07:40:02.000000 prometheus-summary-0.1.2/setup.py
```

### Comparing `prometheus-summary-0.1.1/LICENSE` & `prometheus-summary-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prometheus-summary-0.1.1/PKG-INFO` & `prometheus-summary-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prometheus-summary
-Version: 0.1.1
+Version: 0.1.2
 Summary: Prometheus summary with quantiles over configurable sliding time window
 Home-page: https://github.com/RefaceAI/prometheus-summary
 Author: RefaceAI
 Author-email: github-support@reface.ai
 License: Apache License 2.0
 Platform: Platform Independent
 Classifier: Development Status :: 3 - Alpha
@@ -17,15 +17,15 @@
 
 # prometheus-summary
 Prometheus summary with quantiles over configurable sliding time window
 
 ## Installation
 
 ```
-pip install prometheus-summary==0.1.1
+pip install prometheus-summary==0.1.2
 ```
 This package can be found on [PyPI](https://pypi.org/project/prometheus-summary/).
 
 ## Collecting
 
 ### Basic usage
 
@@ -93,11 +93,11 @@
 ```
 
 To show request latency by `method`, `endpoint` and `quntile` use next query:
 ```
 max by (method, endpoint, quantile) (request_latency_seconds)
 ```
 
-To only 99-th quantile:
+To show only 99-th quantile:
 ```
 max by (method, endpoint) (request_latency_seconds{quantile="0.99")
 ```
```

### Comparing `prometheus-summary-0.1.1/README.md` & `prometheus-summary-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # prometheus-summary
 Prometheus summary with quantiles over configurable sliding time window
 
 ## Installation
 
 ```
-pip install prometheus-summary==0.1.1
+pip install prometheus-summary==0.1.2
 ```
 This package can be found on [PyPI](https://pypi.org/project/prometheus-summary/).
 
 ## Collecting
 
 ### Basic usage
 
@@ -76,11 +76,11 @@
 ```
 
 To show request latency by `method`, `endpoint` and `quntile` use next query:
 ```
 max by (method, endpoint, quantile) (request_latency_seconds)
 ```
 
-To only 99-th quantile:
+To show only 99-th quantile:
 ```
 max by (method, endpoint) (request_latency_seconds{quantile="0.99")
 ```
```

### Comparing `prometheus-summary-0.1.1/prometheus_summary/__init__.py` & `prometheus-summary-0.1.2/prometheus_summary/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from threading import Lock
 from typing import Iterable, Sequence, Optional, Tuple
 
 import prometheus_client
 from prometheus_client.samples import Sample
 from quantile_estimator import TimeWindowEstimator
 
 from .version import __version__
@@ -12,26 +13,27 @@
     DEFAULT_INVARIANTS = ((0.50, 0.05), (0.90, 0.01), (0.99, 0.001))
 
     def __init__(
         self,
         name: str,
         documentation: str,
         labelnames: Iterable[str] = (),
-        namespace: str = '',
-        subsystem: str = '',
-        unit: str = '',
+        namespace: str = "",
+        subsystem: str = "",
+        unit: str = "",
         registry: Optional[prometheus_client.CollectorRegistry] = prometheus_client.REGISTRY,
         _labelvalues: Optional[Sequence[str]] = None,
         invariants: Sequence[Tuple[float, float]] = DEFAULT_INVARIANTS,
         max_age_seconds: int = 10 * 60,
         age_buckets: int = 5,
     ) -> None:
         self._invariants = invariants
         self._max_age_seconds = max_age_seconds
         self._age_buckets = age_buckets
+        self._lock = Lock()
         super().__init__(
             name,
             documentation,
             labelnames=labelnames,
             namespace=namespace,
             subsystem=subsystem,
             unit=unit,
@@ -49,16 +51,19 @@
 
     def observe(self, amount):
         if not isinstance(amount, (float, int)):
             raise TypeError("Summary only works with int or float")
 
         amount = float(amount)
         super().observe(amount)
-        self._estimator.observe(amount)
+        with self._lock:
+            self._estimator.observe(amount)
 
     def _child_samples(self):
-        default_samples = super()._child_samples()
-        quantile_samples = tuple(
-            Sample("", {"quantile": str(quantile)}, self._estimator.query(quantile), None, None)
-            for quantile, _ in self._invariants
-        )
-        return [*default_samples, *quantile_samples]
+        with self._lock:
+            samples = [
+                Sample("", {"quantile": str(quantile)}, self._estimator.query(quantile), None, None)
+                for quantile, _ in self._invariants
+            ]
+
+        samples.extend(super()._child_samples())
+        return samples
```

### Comparing `prometheus-summary-0.1.1/prometheus_summary.egg-info/PKG-INFO` & `prometheus-summary-0.1.2/prometheus_summary.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prometheus-summary
-Version: 0.1.1
+Version: 0.1.2
 Summary: Prometheus summary with quantiles over configurable sliding time window
 Home-page: https://github.com/RefaceAI/prometheus-summary
 Author: RefaceAI
 Author-email: github-support@reface.ai
 License: Apache License 2.0
 Platform: Platform Independent
 Classifier: Development Status :: 3 - Alpha
@@ -17,15 +17,15 @@
 
 # prometheus-summary
 Prometheus summary with quantiles over configurable sliding time window
 
 ## Installation
 
 ```
-pip install prometheus-summary==0.1.1
+pip install prometheus-summary==0.1.2
 ```
 This package can be found on [PyPI](https://pypi.org/project/prometheus-summary/).
 
 ## Collecting
 
 ### Basic usage
 
@@ -93,11 +93,11 @@
 ```
 
 To show request latency by `method`, `endpoint` and `quntile` use next query:
 ```
 max by (method, endpoint, quantile) (request_latency_seconds)
 ```
 
-To only 99-th quantile:
+To show only 99-th quantile:
 ```
 max by (method, endpoint) (request_latency_seconds{quantile="0.99")
 ```
```

### Comparing `prometheus-summary-0.1.1/setup.py` & `prometheus-summary-0.1.2/setup.py`

 * *Files identical despite different names*

