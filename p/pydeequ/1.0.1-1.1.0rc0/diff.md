# Comparing `tmp/pydeequ-1.0.1.tar.gz` & `tmp/pydeequ-1.1.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydeequ-1.0.1.tar", max compression
+gzip compressed data, was "pydeequ-1.1.0rc0.tar", max compression
```

## Comparing `pydeequ-1.0.1.tar` & `pydeequ-1.1.0rc0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0    11357 2020-11-09 23:53:43.000000 pydeequ-1.0.1/LICENSE
--rw-r--r--   0        0        0     7501 2021-07-22 18:17:19.966679 pydeequ-1.0.1/README.md
--rw-r--r--   0        0        0     1607 2021-07-29 18:21:57.550590 pydeequ-1.0.1/pydeequ/__init__.py
--rw-r--r--   0        0        0    27271 2021-07-19 21:19:04.066011 pydeequ-1.0.1/pydeequ/analyzers.py
--rw-r--r--   0        0        0    10670 2021-07-19 19:29:24.740055 pydeequ-1.0.1/pydeequ/anomaly_detection.py
--rw-r--r--   0        0        0    41906 2021-07-22 18:15:25.364658 pydeequ-1.0.1/pydeequ/checks.py
--rw-r--r--   0        0        0     2019 2021-07-29 18:19:25.937496 pydeequ-1.0.1/pydeequ/configs.py
--rw-r--r--   0        0        0     2061 2021-07-19 19:29:24.743149 pydeequ-1.0.1/pydeequ/metrics.py
--rw-r--r--   0        0        0     2475 2021-07-19 19:29:24.744154 pydeequ-1.0.1/pydeequ/pandas_utils.py
--rw-r--r--   0        0        0    17640 2021-07-19 21:19:04.068199 pydeequ-1.0.1/pydeequ/profiles.py
--rw-r--r--   0        0        0     6704 2021-07-19 19:29:24.745486 pydeequ-1.0.1/pydeequ/repository.py
--rw-r--r--   0        0        0     3617 2021-07-19 19:29:24.746859 pydeequ-1.0.1/pydeequ/scala_utils.py
--rw-r--r--   0        0        0     7860 2021-07-19 19:29:24.747770 pydeequ-1.0.1/pydeequ/suggestions.py
--rw-r--r--   0        0        0    10216 2021-07-19 21:19:04.069465 pydeequ-1.0.1/pydeequ/verification.py
--rw-r--r--   0        0        0     2708 2021-07-29 18:21:57.546923 pydeequ-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     8544 2021-07-29 18:22:33.364119 pydeequ-1.0.1/setup.py
--rw-r--r--   0        0        0     8541 2021-07-29 18:22:33.364781 pydeequ-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-08 15:55:16.576797 pydeequ-1.1.0rc0/LICENSE
+-rw-r--r--   0        0        0     7718 2023-06-08 15:55:16.576915 pydeequ-1.1.0rc0/README.md
+-rw-r--r--   0        0        0     1598 2023-06-19 16:36:21.702250 pydeequ-1.1.0rc0/pydeequ/__init__.py
+-rw-r--r--   0        0        0    27271 2023-06-08 15:55:16.581835 pydeequ-1.1.0rc0/pydeequ/analyzers.py
+-rw-r--r--   0        0        0    10670 2023-06-08 15:55:16.581996 pydeequ-1.1.0rc0/pydeequ/anomaly_detection.py
+-rw-r--r--   0        0        0    41886 2023-06-19 16:30:42.591643 pydeequ-1.1.0rc0/pydeequ/checks.py
+-rw-r--r--   0        0        0     1434 2023-06-19 16:30:42.592148 pydeequ-1.1.0rc0/pydeequ/configs.py
+-rw-r--r--   0        0        0     2061 2023-06-08 15:55:16.582423 pydeequ-1.1.0rc0/pydeequ/metrics.py
+-rw-r--r--   0        0        0     2475 2023-06-08 15:55:16.582525 pydeequ-1.1.0rc0/pydeequ/pandas_utils.py
+-rw-r--r--   0        0        0    17640 2023-06-08 15:55:16.582681 pydeequ-1.1.0rc0/pydeequ/profiles.py
+-rw-r--r--   0        0        0     6704 2023-06-08 15:55:16.582819 pydeequ-1.1.0rc0/pydeequ/repository.py
+-rw-r--r--   0        0        0     3774 2023-06-08 15:55:16.582925 pydeequ-1.1.0rc0/pydeequ/scala_utils.py
+-rw-r--r--   0        0        0     8740 2023-06-08 15:55:16.583035 pydeequ-1.1.0rc0/pydeequ/suggestions.py
+-rw-r--r--   0        0        0    10216 2023-06-08 15:55:16.583154 pydeequ-1.1.0rc0/pydeequ/verification.py
+-rw-r--r--   0        0        0     2709 2023-06-19 17:06:59.998275 pydeequ-1.1.0rc0/pyproject.toml
+-rw-r--r--   0        0        0     8862 1970-01-01 00:00:00.000000 pydeequ-1.1.0rc0/PKG-INFO
```

### Comparing `pydeequ-1.0.1/LICENSE` & `pydeequ-1.1.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydeequ-1.0.1/README.md` & `pydeequ-1.1.0rc0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -142,14 +142,23 @@
 ```python
 result_metrep_df = repository.load() \
     .before(ResultKey.current_milli_time()) \
     .forAnalyzers([ApproxCountDistinct('b')]) \
     .getSuccessMetricsAsDataFrame()
 ```
 
+### Wrapping up
+
+After you've ran your jobs with PyDeequ, be sure to shut down your Spark session to prevent any hanging processes. 
+
+```python
+spark.sparkContext._gateway.shutdown_callback_server()
+spark.stop()
+```
+
 ## [Contributing](https://github.com/awslabs/python-deequ/blob/master/CONTRIBUTING.md)
 Please refer to the [contributing doc](https://github.com/awslabs/python-deequ/blob/master/CONTRIBUTING.md) for how to contribute to PyDeequ.
 
 ## [License](https://github.com/awslabs/python-deequ/blob/master/LICENSE)
 
 This library is licensed under the Apache 2.0 License.
```

### Comparing `pydeequ-1.0.1/pydeequ/__init__.py` & `pydeequ-1.1.0rc0/pydeequ/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 #     http://aws.amazon.com/apache2.0/
 #
 # or in the "license" file accompanying this file. This file is
 # distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 """Placeholder docstrings"""
-__version__ = "1.0.1"
+__version__ = "1.1.0rc0"
 
 from pyspark.sql import SparkSession
 
 from pydeequ.analyzers import AnalysisRunner
 from pydeequ.checks import Check, CheckLevel
-from pydeequ.configs import set_deequ_maven_config
+from pydeequ.configs import DEEQU_MAVEN_COORD
 from pydeequ.profiles import ColumnProfilerRunner
 
-deequ_maven_coord = set_deequ_maven_config()
+deequ_maven_coord = DEEQU_MAVEN_COORD
 f2j_maven_coord = "net.sourceforge.f2j:arpack_combined_all"
 
 
 class PyDeequSession:
     """
     For interacting with PyDeequ Modules at the "Runner" Level
     """
```

### Comparing `pydeequ-1.0.1/pydeequ/analyzers.py` & `pydeequ-1.1.0rc0/pydeequ/analyzers.py`

 * *Files identical despite different names*

### Comparing `pydeequ-1.0.1/pydeequ/anomaly_detection.py` & `pydeequ-1.1.0rc0/pydeequ/anomaly_detection.py`

 * *Files identical despite different names*

### Comparing `pydeequ-1.0.1/pydeequ/checks.py` & `pydeequ-1.1.0rc0/pydeequ/checks.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,14 @@
         :param lambda assertion: A function that accepts an int or float parameter.
         :param str hint: A hint that states why a constraint could have failed.
         :return: hasCompleteness self: A Check object that implements the assertion.
         """
         assertion_func = ScalaFunction1(self._spark_session.sparkContext._gateway, assertion)
         hint = self._jvm.scala.Option.apply(hint)
         self._Check = self._Check.hasCompleteness(column, assertion_func, hint)
-        print(self)
         return self
 
     def areComplete(self, columns, hint=None):
         """Creates a constraint that asserts completion in combined set of columns.
 
         :param list[str] columns: Columns in Data Frame to run the assertion on.
         :param str hint: A hint that states why a constraint could have failed.
```

### Comparing `pydeequ-1.0.1/pydeequ/metrics.py` & `pydeequ-1.1.0rc0/pydeequ/metrics.py`

 * *Files identical despite different names*

### Comparing `pydeequ-1.0.1/pydeequ/pandas_utils.py` & `pydeequ-1.1.0rc0/pydeequ/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `pydeequ-1.0.1/pydeequ/profiles.py` & `pydeequ-1.1.0rc0/pydeequ/profiles.py`

 * *Files identical despite different names*

### Comparing `pydeequ-1.0.1/pydeequ/repository.py` & `pydeequ-1.1.0rc0/pydeequ/repository.py`

 * *Files identical despite different names*

### Comparing `pydeequ-1.0.1/pydeequ/scala_utils.py` & `pydeequ-1.1.0rc0/pydeequ/scala_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 """A collection of utility functions and classes for manipulating with scala objects anc classes through py4j
 """
+from py4j.java_gateway import JavaObject
 
 
 class PythonCallback:
     # https://www.py4j.org/advanced_topics.html#py4j-memory-model
     # https://stackoverflow.com/questions/50878834/py4j-error-while-obtaining-a-new-communication-channel-on-multithreaded-java
     def __init__(self, gateway):
         self.gateway = gateway
@@ -104,8 +105,9 @@
     # Currently turn the java object into a string and pass it through
     start = java_list.index("(")
     end = java_list.index(")")
     empty_val = "" if datatype == str else None
     return [datatype(i) if i != "" else empty_val for i in java_list[start + 1 : end].split(",")]
 
 
-# TODO Tuple => Python Tuple
+def scala_get_default_argument(java_object, argument_idx: int) -> JavaObject:
+    return getattr(java_object, f"apply$default${argument_idx}")()
```

### Comparing `pydeequ-1.0.1/pydeequ/suggestions.py` & `pydeequ-1.1.0rc0/pydeequ/suggestions.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 Author: Calvin Wang
 """
 import json
 
 from pyspark.sql import DataFrame, SparkSession
 
 from pydeequ.pandas_utils import ensure_pyspark_df
+from pydeequ.configs import IS_DEEQU_V1
+from pydeequ.scala_utils import scala_get_default_argument
 
 
 class ConstraintSuggestionRunner:
     """
     Primary class for interacting with suggestions module
 
     :param SparkSession spark_session: sparkSession
@@ -41,16 +43,16 @@
     """
 
     def __init__(self, spark_session: SparkSession, df: DataFrame):
         self._spark_session = spark_session
         self._jvm = spark_session._jvm
         self._jspark_session = spark_session._jsparkSession
         self._df = df
-        self._ConstraintSuggestionRunBuilder = self._jvm.com.amazon.deequ.suggestions.ConstraintSuggestionRunBuilder(
-            df._jdf
+        self._ConstraintSuggestionRunBuilder = (
+            self._jvm.com.amazon.deequ.suggestions.ConstraintSuggestionRunBuilder(df._jdf)
         )
 
     def addConstraintRule(self, constraintRule):
         """
         Add a single rule for suggesting constraints based on ColumnProfiles to the run.
 
         :param ConstraintRule constraintRule:  A rule that the dataset will be evaluated on throughout to the run.
@@ -179,15 +181,22 @@
 class CategoricalRangeRule(_RulesObject):
     """
     If we see a categorical range for a column, we suggest an IS IN (...) constraint
     """
 
     @property
     def rule_jvm(self):
-        return self._deequSuggestions.rules.CategoricalRangeRule()
+        if IS_DEEQU_V1:
+            return self._deequSuggestions.rules.CategoricalRangeRule()
+
+        # DISCLAIMER: this is a workaround for using the default category sorter
+        default_category_sorter = scala_get_default_argument(
+            self._deequSuggestions.rules.CategoricalRangeRule, 1
+        )
+        return self._deequSuggestions.rules.CategoricalRangeRule(default_category_sorter)
 
 
 class CompleteIfCompleteRule(_RulesObject):
     """
     If a column is complete in the sample, we suggest a NOT NULL constraint
     """
 
@@ -207,15 +216,26 @@
 
     def __init__(self, targetDataCoverageFraction: float = 0.9):
 
         self.targetDataCoverageFraction = targetDataCoverageFraction
 
     @property
     def rule_jvm(self):
-        return self._deequSuggestions.rules.FractionalCategoricalRangeRule(self.targetDataCoverageFraction)
+        if IS_DEEQU_V1:
+            return self._deequSuggestions.rules.FractionalCategoricalRangeRule(
+                self.targetDataCoverageFraction
+            )
+
+        # DISCLAIMER: this is a workaround for using the default category sorter
+        default_category_sorter = scala_get_default_argument(
+            self._deequSuggestions.rules.FractionalCategoricalRangeRule, 2
+        )
+        return self._deequSuggestions.rules.FractionalCategoricalRangeRule(
+            self.targetDataCoverageFraction, default_category_sorter
+        )
 
 
 class NonNegativeNumbersRule(_RulesObject):
     """
     If we see only non-negative numbers in a column, we suggest a corresponding constraint
     """
```

### Comparing `pydeequ-1.0.1/pydeequ/verification.py` & `pydeequ-1.1.0rc0/pydeequ/verification.py`

 * *Files identical despite different names*

### Comparing `pydeequ-1.0.1/pyproject.toml` & `pydeequ-1.1.0rc0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydeequ"
-version = "1.0.1"
+version = "1.1.0rc0"
 description = "PyDeequ - Unit Tests for Data"
 authors = ["Calvin Wang <calviwan@amazon.com>"]
 maintainers = ["Calvin Wang <calviwan@amazon.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://pydeequ.readthedocs.io"
 repository = "https://github.com/awslabs/python-deequ"
@@ -24,18 +24,18 @@
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License"
 ]
 
 
 [tool.poetry.dependencies]
-python = ">=3.6.2,<4"
+python = ">=3.7,<4"
 numpy = ">=1.14.1"
 pandas = ">=0.23.0"
-pyspark = { version = ">=2.4.7, <3.1.1", optional = true }
+pyspark = { version = ">=2.4.7, <3.3.0", optional = true }
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.4"
 pytest-cov = "^2.11.1"
 coverage = "^5.5"
 pytest-runner = "^5.3.0"
 black = "^21.5b1"
```

### Comparing `pydeequ-1.0.1/setup.py` & `pydeequ-1.1.0rc0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,274 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pydeequ
+Version: 1.1.0rc0
+Summary: PyDeequ - Unit Tests for Data
+Home-page: https://pydeequ.readthedocs.io
+License: Apache-2.0
+Keywords: deequ,pydeequ,data-engineering,data-quality,data-profiling,dataquality,dataunittest,data-unit-tests,data-profilers
+Author: Calvin Wang
+Author-email: calviwan@amazon.com
+Maintainer: Calvin Wang
+Maintainer-email: calviwan@amazon.com
+Requires-Python: >=3.7,<4
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: pyspark
+Requires-Dist: numpy (>=1.14.1)
+Requires-Dist: pandas (>=0.23.0)
+Requires-Dist: pyspark (>=2.4.7,<3.3.0) ; extra == "pyspark"
+Project-URL: Documentation, https://pydeequ.readthedocs.io
+Project-URL: Repository, https://github.com/awslabs/python-deequ
+Description-Content-Type: text/markdown
 
-packages = \
-['pydeequ']
+# PyDeequ
 
-package_data = \
-{'': ['*']}
+PyDeequ is a Python API for [Deequ](https://github.com/awslabs/deequ), a library built on top of Apache Spark for defining "unit tests for data", which measure data quality in large datasets. PyDeequ is written to support usage of Deequ in Python.
 
-install_requires = \
-['numpy>=1.14.1', 'pandas>=0.23.0']
-
-extras_require = \
-{'pyspark': ['pyspark>=2.4.7,<3.1.1']}
-
-setup_kwargs = {
-    'name': 'pydeequ',
-    'version': '1.0.1',
-    'description': 'PyDeequ - Unit Tests for Data',
-    'long_description': '# PyDeequ\n\nPyDeequ is a Python API for [Deequ](https://github.com/awslabs/deequ), a library built on top of Apache Spark for defining "unit tests for data", which measure data quality in large datasets. PyDeequ is written to support usage of Deequ in Python.\n\n[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) ![Coverage](https://img.shields.io/badge/coverage-90%25-green)\n\nThere are 4 main components of Deequ, and they are:\n- Metrics Computation:\n    - `Profiles` leverages Analyzers to analyze each column of a dataset.\n    - `Analyzers` serve here as a foundational module that computes metrics for data profiling and validation at scale.\n- Constraint Suggestion:\n    - Specify rules for various groups of Analyzers to be run over a dataset to return back a collection of constraints suggested to run in a Verification Suite.\n- Constraint Verification:\n    - Perform data validation on a dataset with respect to various constraints set by you.   \n- Metrics Repository\n    - Allows for persistence and tracking of Deequ runs over time.\n\n![](imgs/pydeequ_architecture.jpg)\n\n## 🎉 Announcements 🎉\n- With PyDeequ v0.1.8+, we now officially support Spark3 ! Just make sure you have an environment variable `SPARK_VERSION` to specify your Spark version! \n- We\'ve release a blogpost on integrating PyDeequ onto AWS leveraging services such as AWS Glue, Athena, and SageMaker! Check it out: [Monitor data quality in your data lake using PyDeequ and AWS Glue](https://aws.amazon.com/blogs/big-data/monitor-data-quality-in-your-data-lake-using-pydeequ-and-aws-glue/).\n- Check out the [PyDeequ Release Announcement Blogpost](https://aws.amazon.com/blogs/big-data/testing-data-quality-at-scale-with-pydeequ/) with a tutorial walkthrough the Amazon Reviews dataset!\n- Join the PyDeequ community on [PyDeequ Slack](https://join.slack.com/t/pydeequ/shared_invite/zt-te6bntpu-yaqPy7bhiN8Lu0NxpZs47Q) to chat with the devs!\n\n## Quickstart\n\nThe following will quickstart you with some basic usage. For more in-depth examples, take a look in the [`tutorials/`](tutorials/) directory for executable Jupyter notebooks of each module. For documentation on supported interfaces, view the [`documentation`](https://pydeequ.readthedocs.io/).\n\n### Installation\n\nYou can install [PyDeequ via pip](https://pypi.org/project/pydeequ/).\n\n```\npip install pydeequ\n```\n\n### Set up a PySpark session\n```python\nfrom pyspark.sql import SparkSession, Row\nimport pydeequ\n\nspark = (SparkSession\n    .builder\n    .config("spark.jars.packages", pydeequ.deequ_maven_coord)\n    .config("spark.jars.excludes", pydeequ.f2j_maven_coord)\n    .getOrCreate())\n\ndf = spark.sparkContext.parallelize([\n            Row(a="foo", b=1, c=5),\n            Row(a="bar", b=2, c=6),\n            Row(a="baz", b=3, c=None)]).toDF()\n```\n\n### Analyzers\n\n```python\nfrom pydeequ.analyzers import *\n\nanalysisResult = AnalysisRunner(spark) \\\n                    .onData(df) \\\n                    .addAnalyzer(Size()) \\\n                    .addAnalyzer(Completeness("b")) \\\n                    .run()\n\nanalysisResult_df = AnalyzerContext.successMetricsAsDataFrame(spark, analysisResult)\nanalysisResult_df.show()\n```\n\n### Profile\n\n```python\nfrom pydeequ.profiles import *\n\nresult = ColumnProfilerRunner(spark) \\\n    .onData(df) \\\n    .run()\n\nfor col, profile in result.profiles.items():\n    print(profile)\n```\n\n### Constraint Suggestions\n\n```python\nfrom pydeequ.suggestions import *\n\nsuggestionResult = ConstraintSuggestionRunner(spark) \\\n             .onData(df) \\\n             .addConstraintRule(DEFAULT()) \\\n             .run()\n\n# Constraint Suggestions in JSON format\nprint(suggestionResult)\n```\n\n### Constraint Verification\n\n```python\nfrom pydeequ.checks import *\nfrom pydeequ.verification import *\n\ncheck = Check(spark, CheckLevel.Warning, "Review Check")\n\ncheckResult = VerificationSuite(spark) \\\n    .onData(df) \\\n    .addCheck(\n        check.hasSize(lambda x: x >= 3) \\\n        .hasMin("b", lambda x: x == 0) \\\n        .isComplete("c")  \\\n        .isUnique("a")  \\\n        .isContainedIn("a", ["foo", "bar", "baz"]) \\\n        .isNonNegative("b")) \\\n    .run()\n\ncheckResult_df = VerificationResult.checkResultsAsDataFrame(spark, checkResult)\ncheckResult_df.show()\n```\n\n### Repository\n\nSave to a Metrics Repository by adding the `useRepository()` and `saveOrAppendResult()` calls to your Analysis Runner.\n```python\nfrom pydeequ.repository import *\nfrom pydeequ.analyzers import *\n\nmetrics_file = FileSystemMetricsRepository.helper_metrics_file(spark, \'metrics.json\')\nrepository = FileSystemMetricsRepository(spark, metrics_file)\nkey_tags = {\'tag\': \'pydeequ hello world\'}\nresultKey = ResultKey(spark, ResultKey.current_milli_time(), key_tags)\n\nanalysisResult = AnalysisRunner(spark) \\\n    .onData(df) \\\n    .addAnalyzer(ApproxCountDistinct(\'b\')) \\\n    .useRepository(repository) \\\n    .saveOrAppendResult(resultKey) \\\n    .run()\n```\n\nTo load previous runs, use the `repository` object to load previous results back in.\n\n```python\nresult_metrep_df = repository.load() \\\n    .before(ResultKey.current_milli_time()) \\\n    .forAnalyzers([ApproxCountDistinct(\'b\')]) \\\n    .getSuccessMetricsAsDataFrame()\n```\n\n## [Contributing](https://github.com/awslabs/python-deequ/blob/master/CONTRIBUTING.md)\nPlease refer to the [contributing doc](https://github.com/awslabs/python-deequ/blob/master/CONTRIBUTING.md) for how to contribute to PyDeequ.\n\n## [License](https://github.com/awslabs/python-deequ/blob/master/LICENSE)\n\nThis library is licensed under the Apache 2.0 License.\n\n******\n\n## Contributing Developer Setup\n\n1. Setup [SDKMAN](#setup-sdkman)\n1. Setup [Java](#setup-java)\n1. Setup [Apache Spark](#setup-apache-spark)\n1. Install [Poetry](#poetry)\n1. Run [tests locally](#running-tests-locally)\n\n### Setup SDKMAN\n\nSDKMAN is a tool for managing parallel Versions of multiple Software Development Kits on any Unix based\nsystem. It provides a convenient command line interface for installing, switching, removing and listing\nCandidates. SDKMAN! installs smoothly on Mac OSX, Linux, WSL, Cygwin, etc... Support Bash and ZSH shells. See\ndocumentation on the [SDKMAN! website](https://sdkman.io).\n\nOpen your favourite terminal and enter the following:\n\n```bash\n$ curl -s https://get.sdkman.io | bash\nIf the environment needs tweaking for SDKMAN to be installed,\nthe installer will prompt you accordingly and ask you to restart.\n\nNext, open a new terminal or enter:\n\n$ source "$HOME/.sdkman/bin/sdkman-init.sh"\n\nLastly, run the following code snippet to ensure that installation succeeded:\n\n$ sdk version\n```\n\n### Setup Java\n\nInstall Java Now open favourite terminal and enter the following:\n\n```bash\nList the AdoptOpenJDK OpenJDK versions\n$ sdk list java\n\nTo install For Java 11\n$ sdk install java 11.0.10.hs-adpt\n\nTo install For Java 11\n$ sdk install java 8.0.292.hs-adpt\n```\n\n### Setup Apache Spark\n\nInstall Java Now open favourite terminal and enter the following:\n\n```bash\nList the Apache Spark versions:\n$ sdk list spark\n\nTo install For Spark 3\n$ sdk install spark 3.0.2\n```\n\n### Poetry\n\nPoetry [Commands](https://python-poetry.org/docs/cli/#search)\n\n```bash\npoetry install\n\npoetry update\n\n# --tree: List the dependencies as a tree.\n# --latest (-l): Show the latest version.\n# --outdated (-o): Show the latest version but only for packages that are outdated.\npoetry show -o\n```\n\n## Running Tests Locally\n\nTake a look at tests in `tests/dataquality` and `tests/jobs`\n\n```bash\n$ poetry run pytest\n```',
-    'author': 'Calvin Wang',
-    'author_email': 'calviwan@amazon.com',
-    'maintainer': 'Calvin Wang',
-    'maintainer_email': 'calviwan@amazon.com',
-    'url': 'https://pydeequ.readthedocs.io',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.6.2,<4',
-}
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) ![Coverage](https://img.shields.io/badge/coverage-90%25-green)
 
+There are 4 main components of Deequ, and they are:
+- Metrics Computation:
+    - `Profiles` leverages Analyzers to analyze each column of a dataset.
+    - `Analyzers` serve here as a foundational module that computes metrics for data profiling and validation at scale.
+- Constraint Suggestion:
+    - Specify rules for various groups of Analyzers to be run over a dataset to return back a collection of constraints suggested to run in a Verification Suite.
+- Constraint Verification:
+    - Perform data validation on a dataset with respect to various constraints set by you.   
+- Metrics Repository
+    - Allows for persistence and tracking of Deequ runs over time.
 
-setup(**setup_kwargs)
+![](imgs/pydeequ_architecture.jpg)
+
+## 🎉 Announcements 🎉
+- With PyDeequ v0.1.8+, we now officially support Spark3 ! Just make sure you have an environment variable `SPARK_VERSION` to specify your Spark version! 
+- We've release a blogpost on integrating PyDeequ onto AWS leveraging services such as AWS Glue, Athena, and SageMaker! Check it out: [Monitor data quality in your data lake using PyDeequ and AWS Glue](https://aws.amazon.com/blogs/big-data/monitor-data-quality-in-your-data-lake-using-pydeequ-and-aws-glue/).
+- Check out the [PyDeequ Release Announcement Blogpost](https://aws.amazon.com/blogs/big-data/testing-data-quality-at-scale-with-pydeequ/) with a tutorial walkthrough the Amazon Reviews dataset!
+- Join the PyDeequ community on [PyDeequ Slack](https://join.slack.com/t/pydeequ/shared_invite/zt-te6bntpu-yaqPy7bhiN8Lu0NxpZs47Q) to chat with the devs!
+
+## Quickstart
+
+The following will quickstart you with some basic usage. For more in-depth examples, take a look in the [`tutorials/`](tutorials/) directory for executable Jupyter notebooks of each module. For documentation on supported interfaces, view the [`documentation`](https://pydeequ.readthedocs.io/).
+
+### Installation
+
+You can install [PyDeequ via pip](https://pypi.org/project/pydeequ/).
+
+```
+pip install pydeequ
+```
+
+### Set up a PySpark session
+```python
+from pyspark.sql import SparkSession, Row
+import pydeequ
+
+spark = (SparkSession
+    .builder
+    .config("spark.jars.packages", pydeequ.deequ_maven_coord)
+    .config("spark.jars.excludes", pydeequ.f2j_maven_coord)
+    .getOrCreate())
+
+df = spark.sparkContext.parallelize([
+            Row(a="foo", b=1, c=5),
+            Row(a="bar", b=2, c=6),
+            Row(a="baz", b=3, c=None)]).toDF()
+```
+
+### Analyzers
+
+```python
+from pydeequ.analyzers import *
+
+analysisResult = AnalysisRunner(spark) \
+                    .onData(df) \
+                    .addAnalyzer(Size()) \
+                    .addAnalyzer(Completeness("b")) \
+                    .run()
+
+analysisResult_df = AnalyzerContext.successMetricsAsDataFrame(spark, analysisResult)
+analysisResult_df.show()
+```
+
+### Profile
+
+```python
+from pydeequ.profiles import *
+
+result = ColumnProfilerRunner(spark) \
+    .onData(df) \
+    .run()
+
+for col, profile in result.profiles.items():
+    print(profile)
+```
+
+### Constraint Suggestions
+
+```python
+from pydeequ.suggestions import *
+
+suggestionResult = ConstraintSuggestionRunner(spark) \
+             .onData(df) \
+             .addConstraintRule(DEFAULT()) \
+             .run()
+
+# Constraint Suggestions in JSON format
+print(suggestionResult)
+```
+
+### Constraint Verification
+
+```python
+from pydeequ.checks import *
+from pydeequ.verification import *
+
+check = Check(spark, CheckLevel.Warning, "Review Check")
+
+checkResult = VerificationSuite(spark) \
+    .onData(df) \
+    .addCheck(
+        check.hasSize(lambda x: x >= 3) \
+        .hasMin("b", lambda x: x == 0) \
+        .isComplete("c")  \
+        .isUnique("a")  \
+        .isContainedIn("a", ["foo", "bar", "baz"]) \
+        .isNonNegative("b")) \
+    .run()
+
+checkResult_df = VerificationResult.checkResultsAsDataFrame(spark, checkResult)
+checkResult_df.show()
+```
+
+### Repository
+
+Save to a Metrics Repository by adding the `useRepository()` and `saveOrAppendResult()` calls to your Analysis Runner.
+```python
+from pydeequ.repository import *
+from pydeequ.analyzers import *
+
+metrics_file = FileSystemMetricsRepository.helper_metrics_file(spark, 'metrics.json')
+repository = FileSystemMetricsRepository(spark, metrics_file)
+key_tags = {'tag': 'pydeequ hello world'}
+resultKey = ResultKey(spark, ResultKey.current_milli_time(), key_tags)
+
+analysisResult = AnalysisRunner(spark) \
+    .onData(df) \
+    .addAnalyzer(ApproxCountDistinct('b')) \
+    .useRepository(repository) \
+    .saveOrAppendResult(resultKey) \
+    .run()
+```
+
+To load previous runs, use the `repository` object to load previous results back in.
+
+```python
+result_metrep_df = repository.load() \
+    .before(ResultKey.current_milli_time()) \
+    .forAnalyzers([ApproxCountDistinct('b')]) \
+    .getSuccessMetricsAsDataFrame()
+```
+
+### Wrapping up
+
+After you've ran your jobs with PyDeequ, be sure to shut down your Spark session to prevent any hanging processes. 
+
+```python
+spark.sparkContext._gateway.shutdown_callback_server()
+spark.stop()
+```
+
+## [Contributing](https://github.com/awslabs/python-deequ/blob/master/CONTRIBUTING.md)
+Please refer to the [contributing doc](https://github.com/awslabs/python-deequ/blob/master/CONTRIBUTING.md) for how to contribute to PyDeequ.
+
+## [License](https://github.com/awslabs/python-deequ/blob/master/LICENSE)
+
+This library is licensed under the Apache 2.0 License.
+
+******
+
+## Contributing Developer Setup
+
+1. Setup [SDKMAN](#setup-sdkman)
+1. Setup [Java](#setup-java)
+1. Setup [Apache Spark](#setup-apache-spark)
+1. Install [Poetry](#poetry)
+1. Run [tests locally](#running-tests-locally)
+
+### Setup SDKMAN
+
+SDKMAN is a tool for managing parallel Versions of multiple Software Development Kits on any Unix based
+system. It provides a convenient command line interface for installing, switching, removing and listing
+Candidates. SDKMAN! installs smoothly on Mac OSX, Linux, WSL, Cygwin, etc... Support Bash and ZSH shells. See
+documentation on the [SDKMAN! website](https://sdkman.io).
+
+Open your favourite terminal and enter the following:
+
+```bash
+$ curl -s https://get.sdkman.io | bash
+If the environment needs tweaking for SDKMAN to be installed,
+the installer will prompt you accordingly and ask you to restart.
+
+Next, open a new terminal or enter:
+
+$ source "$HOME/.sdkman/bin/sdkman-init.sh"
+
+Lastly, run the following code snippet to ensure that installation succeeded:
+
+$ sdk version
+```
+
+### Setup Java
+
+Install Java Now open favourite terminal and enter the following:
+
+```bash
+List the AdoptOpenJDK OpenJDK versions
+$ sdk list java
+
+To install For Java 11
+$ sdk install java 11.0.10.hs-adpt
+
+To install For Java 11
+$ sdk install java 8.0.292.hs-adpt
+```
+
+### Setup Apache Spark
+
+Install Java Now open favourite terminal and enter the following:
+
+```bash
+List the Apache Spark versions:
+$ sdk list spark
+
+To install For Spark 3
+$ sdk install spark 3.0.2
+```
+
+### Poetry
+
+Poetry [Commands](https://python-poetry.org/docs/cli/#search)
+
+```bash
+poetry install
+
+poetry update
+
+# --tree: List the dependencies as a tree.
+# --latest (-l): Show the latest version.
+# --outdated (-o): Show the latest version but only for packages that are outdated.
+poetry show -o
+```
+
+## Running Tests Locally
+
+Take a look at tests in `tests/dataquality` and `tests/jobs`
+
+```bash
+$ poetry run pytest
+```
```

