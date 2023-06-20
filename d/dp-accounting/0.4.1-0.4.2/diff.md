# Comparing `tmp/dp-accounting-0.4.1.tar.gz` & `tmp/dp-accounting-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dp-accounting-0.4.1.tar", last modified: Wed Apr 26 18:20:44 2023, max compression
+gzip compressed data, was "dp-accounting-0.4.2.tar", last modified: Tue Jun 20 17:09:02 2023, max compression
```

## Comparing `dp-accounting-0.4.1.tar` & `dp-accounting-0.4.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-04-26 18:20:44.118154 dp-accounting-0.4.1/
--rw-r-----   0 galenandrew (404454) primarygroup (89939)     1589 2023-04-26 18:20:44.118154 dp-accounting-0.4.1/PKG-INFO
--rw-r-----   0 galenandrew (404454) primarygroup (89939)     1806 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/README.md
-drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-04-26 18:20:44.114154 dp-accounting-0.4.1/dp_accounting/
--rw-r-----   0 galenandrew (404454) primarygroup (89939)     1800 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/__init__.py
--rw-r-----   0 galenandrew (404454) primarygroup (89939)    13802 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/dp_event.py
--rw-r-----   0 galenandrew (404454) primarygroup (89939)     2833 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/dp_event_builder.py
--rw-r-----   0 galenandrew (404454) primarygroup (89939)     3054 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/dp_event_builder_test.py
--rw-r-----   0 galenandrew (404454) primarygroup (89939)     3688 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/dp_event_test.py
--rw-r-----   0 galenandrew (404454) primarygroup (89939)     8640 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/mechanism_calibration.py
--rw-r-----   0 galenandrew (404454) primarygroup (89939)     8539 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/mechanism_calibration_test.py
-drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-04-26 18:20:44.118154 dp-accounting-0.4.1/dp_accounting/pld/
--rw-r-----   0 galenandrew (404454) primarygroup (89939)      675 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/pld/__init__.py
--rw-r-----   0 galenandrew (404454) primarygroup (89939)    13306 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/pld/accountant.py
--rw-r-----   0 galenandrew (404454) primarygroup (89939)     8424 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/pld/accountant_test.py
--rw-r-----   0 galenandrew (404454) primarygroup (89939)    12372 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/pld/common.py
--rw-r-----   0 galenandrew (404454) primarygroup (89939)     8948 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/pld/common_test.py
--rw-r-----   0 galenandrew (404454) primarygroup (89939)    32711 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/pld/pld_pmf.py
--rw-r-----   0 galenandrew (404454) primarygroup (89939)    28136 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/pld/pld_pmf_test.py
--rw-r-----   0 galenandrew (404454) primarygroup (89939)     5662 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/pld/pld_privacy_accountant.py
--rw-r-----   0 galenandrew (404454) primarygroup (89939)     6085 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/pld/pld_privacy_accountant_test.py
--rw-r-----   0 galenandrew (404454) primarygroup (89939)    63971 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/pld/privacy_loss_distribution.py
--rw-r-----   0 galenandrew (404454) primarygroup (89939)     2548 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/pld/privacy_loss_distribution_basic_example.py
--rw-r-----   0 galenandrew (404454) primarygroup (89939)    52970 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/pld/privacy_loss_distribution_test.py
--rw-r-----   0 galenandrew (404454) primarygroup (89939)    70692 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/pld/privacy_loss_mechanism.py
--rw-r-----   0 galenandrew (404454) primarygroup (89939)    58248 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/pld/privacy_loss_mechanism_test.py
--rw-r-----   0 galenandrew (404454) primarygroup (89939)     3054 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/pld/test_util.py
--rw-r-----   0 galenandrew (404454) primarygroup (89939)     3647 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/pld/test_util_test.py
--rw-r-----   0 galenandrew (404454) primarygroup (89939)     5579 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/privacy_accountant.py
--rw-r-----   0 galenandrew (404454) primarygroup (89939)     4351 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/privacy_accountant_test.py
-drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-04-26 18:20:44.118154 dp-accounting-0.4.1/dp_accounting/rdp/
--rw-r-----   0 galenandrew (404454) primarygroup (89939)      744 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/rdp/__init__.py
--rw-r-----   0 galenandrew (404454) primarygroup (89939)    33535 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/rdp/rdp_privacy_accountant.py
--rw-r-----   0 galenandrew (404454) primarygroup (89939)    28704 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/dp_accounting/rdp/rdp_privacy_accountant_test.py
-drwxr-x---   0 galenandrew (404454) primarygroup (89939)        0 2023-04-26 18:20:44.114154 dp-accounting-0.4.1/dp_accounting.egg-info/
--rw-r-----   0 galenandrew (404454) primarygroup (89939)     1589 2023-04-26 18:20:44.000000 dp-accounting-0.4.1/dp_accounting.egg-info/PKG-INFO
--rw-r-----   0 galenandrew (404454) primarygroup (89939)     1277 2023-04-26 18:20:44.000000 dp-accounting-0.4.1/dp_accounting.egg-info/SOURCES.txt
--rw-r-----   0 galenandrew (404454) primarygroup (89939)        1 2023-04-26 18:20:44.000000 dp-accounting-0.4.1/dp_accounting.egg-info/dependency_links.txt
--rw-r-----   0 galenandrew (404454) primarygroup (89939)       83 2023-04-26 18:20:44.000000 dp-accounting-0.4.1/dp_accounting.egg-info/requires.txt
--rw-r-----   0 galenandrew (404454) primarygroup (89939)       14 2023-04-26 18:20:44.000000 dp-accounting-0.4.1/dp_accounting.egg-info/top_level.txt
--rw-r-----   0 galenandrew (404454) primarygroup (89939)       38 2023-04-26 18:20:44.118154 dp-accounting-0.4.1/setup.cfg
--rw-r-----   0 galenandrew (404454) primarygroup (89939)     2576 2023-04-26 18:17:04.000000 dp-accounting-0.4.1/setup.py
+drwxr-x---   0 pritishk (568285) primarygroup (89939)        0 2023-06-20 17:09:02.657515 dp-accounting-0.4.2/
+-rw-r-----   0 pritishk (568285) primarygroup (89939)     1589 2023-06-20 17:09:02.657515 dp-accounting-0.4.2/PKG-INFO
+-rw-r-----   0 pritishk (568285) primarygroup (89939)     1806 2023-06-20 16:57:00.000000 dp-accounting-0.4.2/README.md
+drwxr-x---   0 pritishk (568285) primarygroup (89939)        0 2023-06-20 17:09:02.649515 dp-accounting-0.4.2/dp_accounting/
+-rw-r-----   0 pritishk (568285) primarygroup (89939)     1800 2023-06-20 16:57:00.000000 dp-accounting-0.4.2/dp_accounting/__init__.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)    13808 2023-06-20 16:57:00.000000 dp-accounting-0.4.2/dp_accounting/dp_event.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)     2833 2023-06-20 16:57:00.000000 dp-accounting-0.4.2/dp_accounting/dp_event_builder.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)     3054 2023-06-20 16:57:00.000000 dp-accounting-0.4.2/dp_accounting/dp_event_builder_test.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)     3688 2023-06-20 16:57:00.000000 dp-accounting-0.4.2/dp_accounting/dp_event_test.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)     8640 2023-06-20 16:57:00.000000 dp-accounting-0.4.2/dp_accounting/mechanism_calibration.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)     8539 2023-06-20 16:57:00.000000 dp-accounting-0.4.2/dp_accounting/mechanism_calibration_test.py
+drwxr-x---   0 pritishk (568285) primarygroup (89939)        0 2023-06-20 17:09:02.657515 dp-accounting-0.4.2/dp_accounting/pld/
+-rw-r-----   0 pritishk (568285) primarygroup (89939)      675 2023-06-20 16:57:00.000000 dp-accounting-0.4.2/dp_accounting/pld/__init__.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)    13306 2023-06-20 16:57:00.000000 dp-accounting-0.4.2/dp_accounting/pld/accountant.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)     8424 2023-06-20 16:57:00.000000 dp-accounting-0.4.2/dp_accounting/pld/accountant_test.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)    12372 2023-06-20 16:57:00.000000 dp-accounting-0.4.2/dp_accounting/pld/common.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)     8948 2023-06-20 16:57:00.000000 dp-accounting-0.4.2/dp_accounting/pld/common_test.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)    32711 2023-06-20 16:57:00.000000 dp-accounting-0.4.2/dp_accounting/pld/pld_pmf.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)    28136 2023-06-20 16:57:00.000000 dp-accounting-0.4.2/dp_accounting/pld/pld_pmf_test.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)     5662 2023-06-20 16:57:00.000000 dp-accounting-0.4.2/dp_accounting/pld/pld_privacy_accountant.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)     6085 2023-06-20 16:57:00.000000 dp-accounting-0.4.2/dp_accounting/pld/pld_privacy_accountant_test.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)    63971 2023-06-20 16:57:00.000000 dp-accounting-0.4.2/dp_accounting/pld/privacy_loss_distribution.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)     2548 2023-06-20 16:57:00.000000 dp-accounting-0.4.2/dp_accounting/pld/privacy_loss_distribution_basic_example.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)    52970 2023-06-20 16:57:00.000000 dp-accounting-0.4.2/dp_accounting/pld/privacy_loss_distribution_test.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)    73592 2023-06-20 16:57:00.000000 dp-accounting-0.4.2/dp_accounting/pld/privacy_loss_mechanism.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)    64627 2023-06-20 16:57:00.000000 dp-accounting-0.4.2/dp_accounting/pld/privacy_loss_mechanism_test.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)     3054 2023-06-20 16:57:00.000000 dp-accounting-0.4.2/dp_accounting/pld/test_util.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)     3647 2023-06-20 16:57:00.000000 dp-accounting-0.4.2/dp_accounting/pld/test_util_test.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)     5579 2023-06-20 16:57:00.000000 dp-accounting-0.4.2/dp_accounting/privacy_accountant.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)     4351 2023-06-20 16:57:00.000000 dp-accounting-0.4.2/dp_accounting/privacy_accountant_test.py
+drwxr-x---   0 pritishk (568285) primarygroup (89939)        0 2023-06-20 17:09:02.657515 dp-accounting-0.4.2/dp_accounting/rdp/
+-rw-r-----   0 pritishk (568285) primarygroup (89939)      744 2023-06-20 16:57:00.000000 dp-accounting-0.4.2/dp_accounting/rdp/__init__.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)    33535 2023-06-20 16:57:00.000000 dp-accounting-0.4.2/dp_accounting/rdp/rdp_privacy_accountant.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)    28704 2023-06-20 16:57:00.000000 dp-accounting-0.4.2/dp_accounting/rdp/rdp_privacy_accountant_test.py
+drwxr-x---   0 pritishk (568285) primarygroup (89939)        0 2023-06-20 17:09:02.653515 dp-accounting-0.4.2/dp_accounting.egg-info/
+-rw-r-----   0 pritishk (568285) primarygroup (89939)     1589 2023-06-20 17:09:02.000000 dp-accounting-0.4.2/dp_accounting.egg-info/PKG-INFO
+-rw-r-----   0 pritishk (568285) primarygroup (89939)     1277 2023-06-20 17:09:02.000000 dp-accounting-0.4.2/dp_accounting.egg-info/SOURCES.txt
+-rw-r-----   0 pritishk (568285) primarygroup (89939)        1 2023-06-20 17:09:02.000000 dp-accounting-0.4.2/dp_accounting.egg-info/dependency_links.txt
+-rw-r-----   0 pritishk (568285) primarygroup (89939)       75 2023-06-20 17:09:02.000000 dp-accounting-0.4.2/dp_accounting.egg-info/requires.txt
+-rw-r-----   0 pritishk (568285) primarygroup (89939)       14 2023-06-20 17:09:02.000000 dp-accounting-0.4.2/dp_accounting.egg-info/top_level.txt
+-rw-r-----   0 pritishk (568285) primarygroup (89939)       38 2023-06-20 17:09:02.657515 dp-accounting-0.4.2/setup.cfg
+-rw-r-----   0 pritishk (568285) primarygroup (89939)     2576 2023-06-20 16:57:00.000000 dp-accounting-0.4.2/setup.py
```

### Comparing `dp-accounting-0.4.1/PKG-INFO` & `dp-accounting-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dp-accounting
-Version: 0.4.1
+Version: 0.4.2
 Summary: Tools for tracking differential privacy budgets
 Home-page: https://github.com/google/differential-privacy/
 Author: Google Differential Privacy Team
 Author-email: dp-open-source@google.com
 License: Apache 2.0
 Keywords: differential-privacy accounting
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dp-accounting-0.4.1/README.md` & `dp-accounting-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.1/dp_accounting/__init__.py` & `dp-accounting-0.4.2/dp_accounting/__init__.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.1/dp_accounting/dp_event.py` & `dp-accounting-0.4.2/dp_accounting/dp_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
  * `PrivacyAccountant` implementations are expected to return `supports(event)`
    is `False` when processing unknown mechanisms.
 """
 
 from collections.abc import Mapping, Sequence
 import importlib
 import typing
-from typing import NamedTuple, Protocol, Union
+from typing import List, NamedTuple, Protocol, Union
 
 import attr
 
 
 @typing.runtime_checkable
 class DpEventNamedTuple(Protocol):
   _fields: tuple[str, ...]
@@ -284,15 +284,15 @@
 @attr.s(frozen=True, slots=True, auto_attribs=True)
 class ComposedDpEvent(DpEvent):
   """Represents application of a series of composed mechanisms.
 
   The composition may be adaptive, where the query producing each event depends
   on the results of prior queries.
   """
-  events: list[DpEvent]
+  events: List[DpEvent]
 
 
 @attr.s(frozen=True, slots=True, auto_attribs=True)
 class PoissonSampledDpEvent(DpEvent):
   """Represents an application of Poisson subsampling.
 
   Each record in the dataset is included in the sample independently with
@@ -345,15 +345,15 @@
 
   Attributes:
     noise_multiplier: The ratio of the noise per node to the sensitivity.
     step_counts: The number of steps in each tree. May be a scalar for a single
       tree.
   """
   noise_multiplier: float
-  step_counts: Union[int, list[int]]
+  step_counts: Union[int, List[int]]
 
 
 @attr.s(frozen=True, slots=True, auto_attribs=True)
 class RepeatAndSelectDpEvent(DpEvent):
   """Represents repeatedly running the mechanism and selecting the best output.
 
   The total number of runs is randomized and drawn from a distribution
```

### Comparing `dp-accounting-0.4.1/dp_accounting/dp_event_builder.py` & `dp-accounting-0.4.2/dp_accounting/dp_event_builder.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.1/dp_accounting/dp_event_builder_test.py` & `dp-accounting-0.4.2/dp_accounting/dp_event_builder_test.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.1/dp_accounting/dp_event_test.py` & `dp-accounting-0.4.2/dp_accounting/dp_event_test.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.1/dp_accounting/mechanism_calibration.py` & `dp-accounting-0.4.2/dp_accounting/mechanism_calibration.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.1/dp_accounting/mechanism_calibration_test.py` & `dp-accounting-0.4.2/dp_accounting/mechanism_calibration_test.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.1/dp_accounting/pld/__init__.py` & `dp-accounting-0.4.2/dp_accounting/pld/__init__.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.1/dp_accounting/pld/accountant.py` & `dp-accounting-0.4.2/dp_accounting/pld/accountant.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.1/dp_accounting/pld/accountant_test.py` & `dp-accounting-0.4.2/dp_accounting/pld/accountant_test.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.1/dp_accounting/pld/common.py` & `dp-accounting-0.4.2/dp_accounting/pld/common.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.1/dp_accounting/pld/common_test.py` & `dp-accounting-0.4.2/dp_accounting/pld/common_test.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.1/dp_accounting/pld/pld_pmf.py` & `dp-accounting-0.4.2/dp_accounting/pld/pld_pmf.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.1/dp_accounting/pld/pld_pmf_test.py` & `dp-accounting-0.4.2/dp_accounting/pld/pld_pmf_test.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.1/dp_accounting/pld/pld_privacy_accountant.py` & `dp-accounting-0.4.2/dp_accounting/pld/pld_privacy_accountant.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.1/dp_accounting/pld/pld_privacy_accountant_test.py` & `dp-accounting-0.4.2/dp_accounting/pld/pld_privacy_accountant_test.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.1/dp_accounting/pld/privacy_loss_distribution.py` & `dp-accounting-0.4.2/dp_accounting/pld/privacy_loss_distribution.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.1/dp_accounting/pld/privacy_loss_distribution_basic_example.py` & `dp-accounting-0.4.2/dp_accounting/pld/privacy_loss_distribution_basic_example.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.1/dp_accounting/pld/privacy_loss_distribution_test.py` & `dp-accounting-0.4.2/dp_accounting/pld/privacy_loss_distribution_test.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.1/dp_accounting/pld/privacy_loss_mechanism.py` & `dp-accounting-0.4.2/dp_accounting/pld/privacy_loss_mechanism.py`

 * *Files 3% similar despite different names*

```diff
@@ -191,40 +191,44 @@
     else:  # Case: self.adjacency_type == AdjacencyType.REMOVE
       # For performance, the case of sampling_prob=1 is handled separately.
       if self.sampling_prob == 1.0:
         return self.noise_cdf(np.add(x, self.sensitivity))
       return ((1 - self.sampling_prob) * self.noise_cdf(x) +
               self.sampling_prob * self.noise_cdf(np.add(x, self.sensitivity)))
 
-  def mu_lower_cdf(
+  def mu_lower_log_cdf(
       self, x: Union[float, Iterable[float]]) -> Union[float, np.ndarray]:
-    """Computes the cumulative density function of the mu_lower distribution.
+    """Computes log cumulative density function of the mu_lower distribution.
 
     For ADD adjacency type, with sub-sampling probability q:
       mu_lower(x) := (1-q) * mu(x) + q * mu(x - sensitivity)
     For REMOVE adjacency type, for any sub-sampling probability:
       mu_lower(x) := mu(x)
 
     Args:
-      x: the point or points at which the cumulative density function is to be
-        calculated.
+      x: the point or points at which the log of the cumulative density function
+        is to be calculated.
 
     Returns:
-      The cumulative density function of the mu_lower distribution at x, i.e.,
-      the probability that mu_lower is less than or equal to x.
+      The log of the cumulative density function of the mu_lower distribution at
+      x, i.e., the log of the probability that mu_lower is less than or equal to
+      x.
     """
     if self.adjacency_type == AdjacencyType.ADD:
       # For performance, the case of sampling_prob=1 is handled separately.
       if self.sampling_prob == 1.0:
-        return self.noise_cdf(np.add(x, -self.sensitivity))
-      return ((1 - self.sampling_prob) * self.noise_cdf(x) +
-              self.sampling_prob * self.noise_cdf(np.add(x, -self.sensitivity)))
+        return self.noise_log_cdf(np.add(x, -self.sensitivity))
+      return np.logaddexp(
+          np.log1p(-self.sampling_prob) + self.noise_log_cdf(x),
+          np.log(self.sampling_prob) +
+          self.noise_log_cdf(np.add(x, -self.sensitivity))
+      )
 
     else:  # Case: self.adjacency_type == AdjacencyType.REMOVE
-      return self.noise_cdf(x)
+      return self.noise_log_cdf(x)
 
   def get_delta_for_epsilon(
       self, epsilon: Union[float, List[float]]) -> Union[float, List[float]]:
     """Computes the epsilon-hockey stick divergence of the mechanism.
 
     The epsilon-hockey stick divergence of the mechanism is the value of delta
     for which the mechanism is (epsilon, delta)-differentially private. (See
@@ -249,34 +253,33 @@
       epsilon-hockey stick divergence.
 
     Returns:
       A non-negative real number which is the epsilon-hockey stick divergence of
       the mechanism, or a numpy array if epsilon is list-like.
     """
     is_scalar = isinstance(epsilon, numbers.Number)
-    epsilon_values = np.array([epsilon]) if is_scalar else np.asarray(epsilon)
-    delta_values = np.zeros_like(epsilon_values, dtype=float)
+    epsilons = np.array([epsilon]) if is_scalar else np.asarray(epsilon)
+    deltas = np.zeros_like(epsilons, dtype=float)
     if self.sampling_prob == 1.0:
-      inverse_indices = np.full_like(epsilon_values, True, dtype=bool)
+      inverse_indices = np.full_like(epsilons, True, dtype=bool)
     elif self.adjacency_type == AdjacencyType.ADD:
-      inverse_indices = epsilon_values < -math.log(1 - self.sampling_prob)
+      inverse_indices = epsilons < -math.log1p(-self.sampling_prob)
     else:  # Case: self.adjacency_type == AdjacencyType.REMOVE
-      inverse_indices = epsilon_values > math.log(1 - self.sampling_prob)
+      inverse_indices = epsilons > math.log1p(-self.sampling_prob)
       other_indices = np.logical_not(inverse_indices)
-      delta_values[other_indices] = 1 - np.exp(epsilon_values[other_indices])
+      deltas[other_indices] = -np.expm1(epsilons[other_indices])
     x_cutoffs = np.array([
-        self.inverse_privacy_loss(eps)
-        for eps in epsilon_values[inverse_indices]
+        self.inverse_privacy_loss(eps) for eps in epsilons[inverse_indices]
     ])
-    delta_values[inverse_indices] = (
+    deltas[inverse_indices] = (
         self.mu_upper_cdf(x_cutoffs) -
-        np.exp(epsilon_values[inverse_indices]) * self.mu_lower_cdf(x_cutoffs))
+        np.exp(epsilons[inverse_indices] + self.mu_lower_log_cdf(x_cutoffs)))
     # Clip delta values to lie in [0,1] (to avoid numerical errors)
-    delta_values = np.clip(delta_values, 0, 1)
-    return float(delta_values) if is_scalar else delta_values
+    deltas = np.clip(deltas, 0, 1)
+    return float(deltas) if is_scalar else deltas
 
   @abc.abstractmethod
   def privacy_loss_tail(self) -> TailPrivacyLossDistribution:
     """Computes the privacy loss at the tail of the distribution.
 
     Returns:
       A TailPrivacyLossDistribution instance representing the tail of the
@@ -459,14 +462,32 @@
       that mu is less than or equal to x.
 
     Raises:
       NotImplementedError: If not implemented by the subclass.
     """
     raise NotImplementedError
 
+  @abc.abstractmethod
+  def noise_log_cdf(
+      self, x: Union[float, Iterable[float]]) -> Union[float, np.ndarray]:
+    """Computes log of cumulative density function of the noise distribution mu.
+
+    Args:
+      x: the point or points at which the log cumulative density function is to
+        be calculated.
+
+    Returns:
+      The log cumulative density function of that noise at x, i.e., the log of
+      the probability that mu is less than or equal to x.
+
+    Raises:
+      NotImplementedError: If not implemented by the subclass.
+    """
+    raise NotImplementedError
+
   @classmethod
   @abc.abstractmethod
   def from_privacy_guarantee(
       cls,
       privacy_parameters: common.DifferentialPrivacyParameters,
       sensitivity: float = 1,
       pessimistic_estimate: bool = True,
@@ -684,14 +705,28 @@
 
     Returns:
       The cumulative density function of the Laplace noise at x, i.e., the
       probability that the Laplace noise is less than or equal to x.
     """
     return self._laplace_random_variable.cdf(x)
 
+  def noise_log_cdf(
+      self, x: Union[float, Iterable[float]]) -> Union[float, np.ndarray]:
+    """Computes log of cumulative density function of the Laplace distribution.
+
+    Args:
+      x: the point or points at which the log cumulative density function is to
+        be calculated.
+
+    Returns:
+      The log cumulative density function of the Laplace noise at x, i.e., the
+      log of the probability that the Laplace noise is less than or equal to x.
+    """
+    return self._laplace_random_variable.logcdf(x)
+
   @classmethod
   def from_privacy_guarantee(
       cls,
       privacy_parameters: common.DifferentialPrivacyParameters,
       sensitivity: float = 1,
       pessimistic_estimate: bool = True,
       sampling_prob: float = 1.0,
@@ -955,14 +990,28 @@
 
     Returns:
       The cumulative density function of the Gaussian noise at x, i.e., the
       probability that the Gaussian noise is less than or equal to x.
     """
     return self._gaussian_random_variable.cdf(x)
 
+  def noise_log_cdf(
+      self, x: Union[float, Iterable[float]]) -> Union[float, np.ndarray]:
+    """Computes log of cumulative density function of the Gaussian distribution.
+
+    Args:
+      x: the point or points at which the log cumulative density function is to
+        be calculated.
+
+    Returns:
+      The log cumulative density function of the Gaussian noise at x, i.e., the
+      log of the probability that the Gaussian noise is less than or equal to x.
+    """
+    return self._gaussian_random_variable.logcdf(x)
+
   @classmethod
   def from_privacy_guarantee(
       cls,
       privacy_parameters: common.DifferentialPrivacyParameters,
       sensitivity: float = 1,
       pessimistic_estimate: bool = True,
       sampling_prob: float = 1.0,
@@ -1212,14 +1261,29 @@
     Returns:
       The cumulative density function of the discrete Laplace noise at x, i.e.,
       the probability that the discrete Laplace noise is less than or equal to
       x.
     """
     return self._discrete_laplace_random_variable.cdf(x)
 
+  def noise_log_cdf(
+      self, x: Union[float, Iterable[float]]) -> Union[float, np.ndarray]:
+    """Computes log of the CDF of the discrete Laplace distribution.
+
+    Args:
+      x: the point or points at which the log cumulative density function is to
+        be calculated.
+
+    Returns:
+      The log cumulative density function of the discrete Laplace noise at x,
+      i.e., the log of the probability that the discrete Laplace noise is less
+      than or equal to x.
+    """
+    return self._discrete_laplace_random_variable.logcdf(x)
+
   @classmethod
   def from_privacy_guarantee(
       cls,
       privacy_parameters: common.DifferentialPrivacyParameters,
       sensitivity: int = 1,
       sampling_prob: float = 1.0,
       adjacency_type: AdjacencyType = AdjacencyType.REMOVE
@@ -1360,21 +1424,21 @@
 
     if 2 * self._truncation_bound < sensitivity:
       raise ValueError(f'Truncation bound ({truncation_bound}) is smaller '
                        f'than 0.5 * sensitivity (0.5 * {sensitivity})')
 
     # Create the PMF and CDF.
     self._offset = -1 * self._truncation_bound - 1
-    self._pmf_array = np.arange(-1 * self._truncation_bound,
-                                self._truncation_bound + 1)
-    self._pmf_array = np.exp(-0.5 * (self._pmf_array)**2 / (sigma**2))
-    self._pmf_array = np.insert(self._pmf_array, 0, 0)
-    self._cdf_array = np.add.accumulate(self._pmf_array)
-    self._pmf_array /= self._cdf_array[-1]
-    self._cdf_array /= self._cdf_array[-1]
+    indices = np.arange(-1 * self._truncation_bound, self._truncation_bound + 1)
+    self._log_pmf_array = np.append(-np.inf, -0.5 * indices**2 / (sigma**2))
+    self._log_cdf_array = np.logaddexp.accumulate(self._log_pmf_array)
+    self._log_pmf_array -= self._log_cdf_array[-1]
+    self._log_cdf_array -= self._log_cdf_array[-1]
+    self._pmf_array = np.exp(self._log_pmf_array)
+    self._cdf_array = np.exp(self._log_cdf_array)
 
     super().__init__(sensitivity, True, sampling_prob, adjacency_type)
 
   def privacy_loss_tail(self) -> TailPrivacyLossDistribution:
     """Computes the privacy loss at the tail of the discrete Gaussian distribution.
 
     The lower_x_truncation and upper_x_truncation are chosen such that for any
@@ -1504,15 +1568,15 @@
       return inverse_privacy_loss_without_subsampling_for_add(privacy_loss)
     else:  # Case: self.adjacency_type == AdjacencyType.REMOVE
       return (inverse_privacy_loss_without_subsampling_for_add(privacy_loss) -
               self.sensitivity)
 
   def noise_cdf(self, x: Union[float,
                                Iterable[float]]) -> Union[float, np.ndarray]:
-    """Computes the cumulative density function of the discrete Gaussian distribution.
+    """Computes the CDF of the discrete Gaussian distribution.
 
     Args:
       x: the point or points at which the cumulative density function is to be
         calculated.
 
     Returns:
       The cumulative density function of the discrete Gaussian noise at x, i.e.,
@@ -1520,14 +1584,32 @@
       x.
     """
     clipped_x = np.clip(x, -1 * self._truncation_bound - 1,
                         self._truncation_bound)
     indices = np.floor(clipped_x).astype('int') - self._offset
     return self._cdf_array[indices]
 
+  def noise_log_cdf(
+      self, x: Union[float, Iterable[float]]) -> Union[float, np.ndarray]:
+    """Computes log of the CDF of the discrete Gaussian distribution.
+
+    Args:
+      x: the point or points at which the log cumulative density function is to
+        be calculated.
+
+    Returns:
+      The log cumulative density function of the discrete Gaussian noise at x,
+      i.e., the log of the probability that the discrete Gaussian noise is less
+      than or equal to x.
+    """
+    clipped_x = np.clip(x, -1 * self._truncation_bound - 1,
+                        self._truncation_bound)
+    indices = np.floor(clipped_x).astype('int') - self._offset
+    return self._log_cdf_array[indices]
+
   @classmethod
   def from_privacy_guarantee(
       cls,
       privacy_parameters: common.DifferentialPrivacyParameters,
       sensitivity: int = 1,
       sampling_prob: float = 1.0,
       adjacency_type: AdjacencyType = AdjacencyType.REMOVE
```

### Comparing `dp-accounting-0.4.1/dp_accounting/pld/privacy_loss_mechanism_test.py` & `dp-accounting-0.4.2/dp_accounting/pld/privacy_loss_mechanism_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,47 @@
   testcase.assertEqual(connect_dots_bounds.upper_x, upper_x)
 
 
 class LaplacePrivacyLossTest(parameterized.TestCase):
 
   @parameterized.parameters(
       # Tests with sampling_prob = 1 for adjacency_type=ADD
+      (1.0, 1.0, 1.0, ADD, [0, 1, 2, 30],
+       [-1.69314718, -0.69314718, -0.20326705, -1.27231559e-13]),
+      (2.0, 1.0, 1.0, ADD, [-1, 0, 1, 30],
+       [-1.69314718, -1.19314718, -0.69314718, -2.52173863e-07]),
+      # # Tests with sampling_prob < 1 for adjacency_type=ADD
+      (1.0, 1.0, 0.8, ADD, [0, 1, 2, 30],
+       [-1.39775265, -0.57409907, -0.17516956, -1.11161080e-13]),
+      (2.0, 1.0, 0.2, ADD, [-1, 0, 1, 30],
+       [-1.27511009, -0.77511009, -0.41948127, -1.72795709e-07]),
+      # # Tests with sampling_prob = 1 for adjacency_type=REMOVE
+      (1.0, 1.0, 1.0, REM, [-1, 0, 1, 30],
+       [-1.69314718, -0.69314718, -0.20326705, -4.67403893e-14]),
+      (2.0, 1.0, 1.0, REM, [-2, -1, 0, 30],
+       [-1.69314718, -1.19314718, -0.69314718, -1.52951172e-07]),
+      # # Tests with sampling_prob < 1 for adjacency_type=REMOVE
+      (1.0, 1.0, 0.8, REM, [-1, 0, 1, 30],
+       [-1.69314718, -0.69314718, -0.20326705, -4.67403893e-14]),
+      (2.0, 1.0, 0.2, REM, [-2, -1, 0, 30],
+       [-1.69314718, -1.19314718, -0.69314718, -1.52951172e-07]),
+  )
+  def test_mu_lower_log_cdf(
+      self, parameter, sensitivity, sampling_prob, adjacency_type,
+      x, expected_mu_lower_log_cdf):
+    pl = privacy_loss_mechanism.LaplacePrivacyLoss(
+        parameter,
+        sensitivity=sensitivity,
+        sampling_prob=sampling_prob,
+        adjacency_type=adjacency_type)
+    self.assertSequenceAlmostEqual(pl.mu_lower_log_cdf(x),
+                                   expected_mu_lower_log_cdf)
+
+  @parameterized.parameters(
+      # Tests with sampling_prob = 1 for adjacency_type=ADD
       (1.0, 1.0, 1.0, ADD, -0.1, 1.0), (1.0, 1.0, 1.0, ADD, 2.0, -1.0),
       (1.0, 1.0, 1.0, ADD, 0.3, 0.4), (4.0, 4.0, 1.0, ADD, -0.4, 1.0),
       (5.0, 5.0, 1.0, ADD, 7.0, -1.0), (7.0, 7.0, 1.0, ADD, 2.1, 0.4),
       # Tests with sampling_prob < 1 for adjacency_type=ADD
       (1.0, 1.0, 0.8, ADD, 1.1, -0.86483972516319),
       (2.0, 1.0, 0.2, ADD, -0.2, 0.0819629071393439),
       (1.0, 1.0, 0.5, ADD, 0.5, 0.0),
@@ -304,14 +337,47 @@
       self.assertAlmostEqual(expected_delta, delta)
 
 
 class GaussianPrivacyLossTest(parameterized.TestCase):
 
   @parameterized.parameters(
       # Tests with sampling_prob = 1 for adjacency_type=ADD
+      (1.0, 1.0, 1.0, ADD, [-10, 0, 1, 10],
+       [-6.38249341e+01, -1.84102165e+00, -6.93147181e-01, -1.12858841e-19]),
+      (2.0, 1.0, 1.0, ADD, [-10, 0, 1, 10],
+       [-1.77793764e+01, -1.17591176e+00, -6.93147181e-01, -3.39767890e-06]),
+      # # Tests with sampling_prob < 1 for adjacency_type=ADD
+      (1.0, 1.0, 0.8, ADD, [-10, 0, 1, 10],
+       [-54.84062277, -1.48313922, -0.56516047, 0.]),
+      (2.0, 1.0, 0.2, ADD, [-10, 0, 1, 10],
+       [-1.52717161e+01, -7.72823689e-01, -4.25917894e-01, -9.08856295e-07]),
+      # # Tests with sampling_prob = 1 for adjacency_type=REMOVE
+      (1.0, 1.0, 1.0, REM, [-10, 0, 1, 10],
+       [-5.32312852e+01, -6.93147181e-01, -0.172753779, -7.61985302e-24]),
+      (2.0, 1.0, 1.0, REM, [-10, 0, 1, 10],
+       [-1.50649984e+01, -6.93147181e-01, -3.68946415e-01, -2.86651613e-07]),
+      # # Tests with sampling_prob < 1 for adjacency_type=REMOVE
+      (1.0, 1.0, 0.8, REM, [-10, 0, 1, 10],
+       [-5.32312852e+01, -6.93147181e-01, -1.72753779e-01, -7.61985302e-24]),
+      (2.0, 1.0, 0.2, REM, [-10, 0, 1, 10],
+       [-1.50649984e+01, -6.93147181e-01, -3.68946415e-01, -2.86651613e-07]),
+  )
+  def test_mu_lower_log_cdf(
+      self, standard_deviation, sensitivity, sampling_prob, adjacency_type,
+      x, expected_mu_lower_log_cdf):
+    pl = privacy_loss_mechanism.GaussianPrivacyLoss(
+        standard_deviation,
+        sensitivity=sensitivity,
+        sampling_prob=sampling_prob,
+        adjacency_type=adjacency_type)
+    self.assertSequenceAlmostEqual(pl.mu_lower_log_cdf(x),
+                                   expected_mu_lower_log_cdf)
+
+  @parameterized.parameters(
+      # Tests with sampling_prob = 1 for adjacency_type=ADD
       (1.0, 1.0, 1.0, ADD, 5.0, -4.5), (1.0, 1.0, 1.0, ADD, -3.0, 3.5),
       (1.0, 2.0, 1.0, ADD, 3.0, -4.0),
       (4.0, 4.0, 1.0, ADD, 20.0, -4.5), (5.0, 5.0, 1.0, ADD, -15.0, 3.5),
       (7.0, 14.0, 1.0, ADD, 21.0, -4.0),
       # Tests with sampling_prob < 1 for adjacency_type=ADD
       (1.0, 1.0, 0.8, ADD, 0.5, 0.0),
       (1.0, 1.0, 0.5, ADD, -4, 0.6820994357113515),
@@ -668,14 +734,47 @@
       self.assertAlmostEqual(expected_delta, delta)
 
 
 class DiscreteLaplacePrivacyLossDistributionTest(parameterized.TestCase):
 
   @parameterized.parameters(
       # Tests with sampling_prob = 1 for adjacency_type=ADD
+      (1.0, 1, 1.0, ADD, [-30, 0, 1, 30],
+       [-3.13132617e+01, -1.31326169, -3.13261688e-01, -6.83897383e-14]),
+      (2.0, 1, 1.0, ADD, [-30, 0, 1, 30],
+       [-62.12692801, -2.12692801, -0.12692801, 0.]),
+      # # Tests with sampling_prob < 1 for adjacency_type=ADD
+      (1.0, 1, 0.8, ADD, [-30, 0, 1, 30],
+       [-3.10178672e+01, -1.01786716, -2.67801985e-01, -5.97855099e-14]),
+      (2.0, 1, 0.2, ADD, [-30, 0, 1, 30],
+       [-6.03167975e+01, -3.16797514e-01, -3.74386343e-02, 0.0]),
+      # # Tests with sampling_prob = 1 for adjacency_type=REMOVE
+      (1.0, 1, 1.0, REM, [-30, 0, 1, 30],
+       [-3.03132617e+01, -3.13261688e-01, -1.04181233e-01, -2.52020627e-14]),
+      (2.0, 1, 1.0, REM, [-30, 0, 1, 30],
+       [-6.01269280e+01, -1.26928011e-01, -1.62639044e-02, 0.0]),
+      # # Tests with sampling_prob < 1 for adjacency_type=REMOVE
+      (1.0, 1, 0.8, REM, [-30, 0, 1, 30],
+       [-3.03132617e+01, -3.13261688e-01, -1.04181233e-01, -2.52020627e-14]),
+      (2.0, 1, 0.2, REM, [-30, 0, 1, 30],
+       [-6.01269280e+01, -1.26928011e-01, -1.62639044e-02, 0.0]),
+  )
+  def test_mu_lower_log_cdf(
+      self, parameter, sensitivity, sampling_prob, adjacency_type,
+      x, expected_mu_lower_log_cdf):
+    pl = privacy_loss_mechanism.DiscreteLaplacePrivacyLoss(
+        parameter,
+        sensitivity=sensitivity,
+        sampling_prob=sampling_prob,
+        adjacency_type=adjacency_type)
+    self.assertSequenceAlmostEqual(pl.mu_lower_log_cdf(x),
+                                   expected_mu_lower_log_cdf)
+
+  @parameterized.parameters(
+      # Tests with sampling_prob = 1 for adjacency_type=ADD
       (1.0, 1, 1.0, ADD, 0, 1.0),
       (1.0, 1, 1.0, ADD, 1, -1.0),
       (0.3, 2, 1.0, ADD, 0, 0.6),
       (0.3, 2, 1.0, ADD, 1, 0.0),
       (0.3, 2, 1.0, ADD, 2, -0.6),
       # Tests with sampling_prob < 1 for adjacency_type=ADD
       (1.0, 1, 0.8, ADD, 1, -0.86483972516319),
@@ -946,14 +1045,48 @@
       self.assertAlmostEqual(expected_delta, delta)
 
 
 class DiscreteGaussianPrivacyLossTest(parameterized.TestCase):
 
   @parameterized.parameters(
       # Tests with sampling_prob = 1 for adjacency_type=ADD
+      (1.0, 1, 1.0, ADD, [-1, 0, 1, 2],
+       [-math.inf, -1.29437677, -0.32029979, 0.]),
+      (3.0, 1, 1.0, ADD, [-1, 0, 1, 2],
+       [-math.inf, -1.11747583, -0.39616512, 0.]),
+      # # Tests with sampling_prob < 1 for adjacency_type=ADD
+      (1.0, 1, 0.8, ADD, [-1, 0, 1, 2],
+       [-2.90381468, -1.00939014, -0.24750655, 0.]),
+      (2.0, 1, 0.2, ADD, [-1, 0, 1, 2],
+       [-1.36518195e+00, -4.96759453e-01, -6.59619911e-02, 2.22044605e-16]),
+      # # Tests with sampling_prob = 1 for adjacency_type=REMOVE
+      (1.0, 1, 1.0, REM, [-1, 0, 1, 2],
+       [-1.29437677, -0.32029979, 0.0, 0.0]),
+      (3.0, 1, 1.0, REM, [-1, 0, 1, 2],
+       [-1.11747583, -0.39616512, 0., 0.]),
+      # # Tests with sampling_prob < 1 for adjacency_type=REMOVE
+      (1.0, 1, 0.8, REM, [-1, 0, 1, 2],
+       [-1.29437677, -0.32029979, 0., 0.]),
+      (2.0, 1, 0.2, REM, [-1, 0, 1, 2],
+       [-1.14203839, -0.38443936, 0., 0.]),
+  )
+  def test_mu_lower_log_cdf(
+      self, sigma, sensitivity, sampling_prob, adjacency_type,
+      x, expected_mu_lower_log_cdf):
+    pl = privacy_loss_mechanism.DiscreteGaussianPrivacyLoss(
+        sigma,
+        sensitivity=sensitivity,
+        truncation_bound=1,
+        sampling_prob=sampling_prob,
+        adjacency_type=adjacency_type)
+    self.assertSequenceAlmostEqual(pl.mu_lower_log_cdf(x),
+                                   expected_mu_lower_log_cdf)
+
+  @parameterized.parameters(
+      # Tests with sampling_prob = 1 for adjacency_type=ADD
       (1.0, 1, 1.0, ADD, 5, -4.5),
       (1, 1, 1, ADD, -3, 3.5),
       (1, 2, 1, ADD, 3, -4.0),
       (4.0, 4, 1.0, ADD, 20, -4.5),
       (5, 5, 1, ADD, -15, 3.5),
       (7.0, 14, 1.0, ADD, 21, -4.0),
       (1.0, 1, 1.0, ADD, -12, math.inf),
```

### Comparing `dp-accounting-0.4.1/dp_accounting/pld/test_util.py` & `dp-accounting-0.4.2/dp_accounting/pld/test_util.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.1/dp_accounting/pld/test_util_test.py` & `dp-accounting-0.4.2/dp_accounting/pld/test_util_test.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.1/dp_accounting/privacy_accountant.py` & `dp-accounting-0.4.2/dp_accounting/privacy_accountant.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.1/dp_accounting/privacy_accountant_test.py` & `dp-accounting-0.4.2/dp_accounting/privacy_accountant_test.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.1/dp_accounting/rdp/__init__.py` & `dp-accounting-0.4.2/dp_accounting/rdp/__init__.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.1/dp_accounting/rdp/rdp_privacy_accountant.py` & `dp-accounting-0.4.2/dp_accounting/rdp/rdp_privacy_accountant.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.1/dp_accounting/rdp/rdp_privacy_accountant_test.py` & `dp-accounting-0.4.2/dp_accounting/rdp/rdp_privacy_accountant_test.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.1/dp_accounting.egg-info/PKG-INFO` & `dp-accounting-0.4.2/dp_accounting.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dp-accounting
-Version: 0.4.1
+Version: 0.4.2
 Summary: Tools for tracking differential privacy budgets
 Home-page: https://github.com/google/differential-privacy/
 Author: Google Differential Privacy Team
 Author-email: dp-open-source@google.com
 License: Apache 2.0
 Keywords: differential-privacy accounting
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dp-accounting-0.4.1/dp_accounting.egg-info/SOURCES.txt` & `dp-accounting-0.4.2/dp_accounting.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.1/setup.py` & `dp-accounting-0.4.2/setup.py`

 * *Files identical despite different names*

