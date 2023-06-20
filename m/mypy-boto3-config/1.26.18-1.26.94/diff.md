# Comparing `tmp/mypy-boto3-config-1.26.18.tar.gz` & `tmp/mypy-boto3-config-1.26.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-config-1.26.18.tar", last modified: Tue Nov 29 06:12:18 2022, max compression
+gzip compressed data, was "mypy-boto3-config-1.26.94.tar", last modified: Fri Mar 17 19:32:19 2023, max compression
```

## Comparing `mypy-boto3-config-1.26.18.tar` & `mypy-boto3-config-1.26.94.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 06:12:18.221821 mypy-boto3-config-1.26.18/
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2022-11-29 06:09:19.000000 mypy-boto3-config-1.26.18/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    36463 2022-11-29 06:12:18.217821 mypy-boto3-config-1.26.18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    35023 2022-11-29 06:09:19.000000 mypy-boto3-config-1.26.18/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 06:12:18.217821 mypy-boto3-config-1.26.18/mypy_boto3_config/
--rw-r--r--   0 runner    (1001) docker     (122)     9849 2022-11-29 06:09:19.000000 mypy-boto3-config-1.26.18/mypy_boto3_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9848 2022-11-29 06:09:19.000000 mypy-boto3-config-1.26.18/mypy_boto3_config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      918 2022-11-29 06:09:19.000000 mypy-boto3-config-1.26.18/mypy_boto3_config/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)    87885 2022-11-29 06:09:20.000000 mypy-boto3-config-1.26.18/mypy_boto3_config/client.py
--rw-r--r--   0 runner    (1001) docker     (122)    87755 2022-11-29 06:09:19.000000 mypy-boto3-config-1.26.18/mypy_boto3_config/client.pyi
--rw-r--r--   0 runner    (1001) docker     (122)    23836 2022-11-29 06:09:20.000000 mypy-boto3-config-1.26.18/mypy_boto3_config/literals.py
--rw-r--r--   0 runner    (1001) docker     (122)    23834 2022-11-29 06:09:20.000000 mypy-boto3-config-1.26.18/mypy_boto3_config/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (122)    42907 2022-11-29 06:09:20.000000 mypy-boto3-config-1.26.18/mypy_boto3_config/paginator.py
--rw-r--r--   0 runner    (1001) docker     (122)    42874 2022-11-29 06:09:20.000000 mypy-boto3-config-1.26.18/mypy_boto3_config/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-29 06:09:19.000000 mypy-boto3-config-1.26.18/mypy_boto3_config/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)   127431 2022-11-29 06:09:23.000000 mypy-boto3-config-1.26.18/mypy_boto3_config/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (122)   127280 2022-11-29 06:09:22.000000 mypy-boto3-config-1.26.18/mypy_boto3_config/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (122)       61 2022-11-29 06:09:19.000000 mypy-boto3-config-1.26.18/mypy_boto3_config/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 06:12:18.217821 mypy-boto3-config-1.26.18/mypy_boto3_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    36463 2022-11-29 06:12:18.000000 mypy-boto3-config-1.26.18/mypy_boto3_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      661 2022-11-29 06:12:18.000000 mypy-boto3-config-1.26.18/mypy_boto3_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-29 06:12:18.000000 mypy-boto3-config-1.26.18/mypy_boto3_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-29 06:12:18.000000 mypy-boto3-config-1.26.18/mypy_boto3_config.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       25 2022-11-29 06:12:18.000000 mypy-boto3-config-1.26.18/mypy_boto3_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2022-11-29 06:12:18.000000 mypy-boto3-config-1.26.18/mypy_boto3_config.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-29 06:12:18.221821 mypy-boto3-config-1.26.18/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1964 2022-11-29 06:09:18.000000 mypy-boto3-config-1.26.18/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 19:32:19.865377 mypy-boto3-config-1.26.94/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-17 19:31:59.000000 mypy-boto3-config-1.26.94/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-03-17 19:32:19.865377 mypy-boto3-config-1.26.94/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    35022 2023-03-17 19:31:59.000000 mypy-boto3-config-1.26.94/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 19:32:19.865377 mypy-boto3-config-1.26.94/mypy_boto3_config/
+-rw-r--r--   0 runner    (1001) docker     (123)     9849 2023-03-17 19:31:59.000000 mypy-boto3-config-1.26.94/mypy_boto3_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9848 2023-03-17 19:31:59.000000 mypy-boto3-config-1.26.94/mypy_boto3_config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-03-17 19:31:59.000000 mypy-boto3-config-1.26.94/mypy_boto3_config/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88841 2023-03-17 19:31:59.000000 mypy-boto3-config-1.26.94/mypy_boto3_config/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88711 2023-03-17 19:31:59.000000 mypy-boto3-config-1.26.94/mypy_boto3_config/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    27298 2023-03-17 19:32:00.000000 mypy-boto3-config-1.26.94/mypy_boto3_config/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27296 2023-03-17 19:32:00.000000 mypy-boto3-config-1.26.94/mypy_boto3_config/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    42907 2023-03-17 19:31:59.000000 mypy-boto3-config-1.26.94/mypy_boto3_config/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42874 2023-03-17 19:31:59.000000 mypy-boto3-config-1.26.94/mypy_boto3_config/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 19:31:59.000000 mypy-boto3-config-1.26.94/mypy_boto3_config/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   127431 2023-03-17 19:32:03.000000 mypy-boto3-config-1.26.94/mypy_boto3_config/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127280 2023-03-17 19:32:02.000000 mypy-boto3-config-1.26.94/mypy_boto3_config/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-17 19:31:59.000000 mypy-boto3-config-1.26.94/mypy_boto3_config/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 19:32:19.865377 mypy-boto3-config-1.26.94/mypy_boto3_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-03-17 19:32:19.000000 mypy-boto3-config-1.26.94/mypy_boto3_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-03-17 19:32:19.000000 mypy-boto3-config-1.26.94/mypy_boto3_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 19:32:19.000000 mypy-boto3-config-1.26.94/mypy_boto3_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 19:32:19.000000 mypy-boto3-config-1.26.94/mypy_boto3_config.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-17 19:32:19.000000 mypy-boto3-config-1.26.94/mypy_boto3_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-17 19:32:19.000000 mypy-boto3-config-1.26.94/mypy_boto3_config.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 19:32:19.865377 mypy-boto3-config-1.26.94/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-03-17 19:31:58.000000 mypy-boto3-config-1.26.94/setup.py
```

### Comparing `mypy-boto3-config-1.26.18/LICENSE` & `mypy-boto3-config-1.26.94/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.26.18/PKG-INFO` & `mypy-boto3-config-1.26.94/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-config
-Version: 1.26.18
-Summary: Type annotations for boto3.ConfigService 1.26.18 service generated with mypy-boto3-builder 7.11.11
+Version: 1.26.94
+Summary: Type annotations for boto3.ConfigService 1.26.94 service generated with mypy-boto3-builder 7.13.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,14 +18,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -37,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-config.svg?color=blue)](https://pypi.org/project/mypy-boto3-config)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-config?color=blue)](https://pypistats.org/packages/mypy-boto3-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConfigService 1.26.18](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService)
+[boto3.ConfigService 1.26.94](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-config docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-config-1.26.18/README.md` & `mypy-boto3-config-1.26.94/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-config.svg?color=blue)](https://pypi.org/project/mypy-boto3-config)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-config?color=blue)](https://pypistats.org/packages/mypy-boto3-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConfigService 1.26.18](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService)
+[boto3.ConfigService 1.26.94](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-config docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-config-1.26.18/mypy_boto3_config/__init__.py` & `mypy-boto3-config-1.26.94/mypy_boto3_config/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.26.18/mypy_boto3_config/__init__.pyi` & `mypy-boto3-config-1.26.94/mypy_boto3_config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.26.18/mypy_boto3_config/__main__.py` & `mypy-boto3-config-1.26.94/mypy_boto3_config/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ConfigService 1.26.18\nVersion:         1.26.18\nBuilder"
-        " version: 7.11.11\nDocs:           "
+        "Type annotations for boto3.ConfigService 1.26.94\nVersion:         1.26.94\nBuilder"
+        " version: 7.13.0\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.18")
+    print("1.26.94")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-config-1.26.18/mypy_boto3_config/client.py` & `mypy-boto3-config-1.26.94/mypy_boto3_config/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -585,15 +585,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#describe_configuration_aggregators)
         """
 
     def describe_configuration_recorder_status(
         self, *, ConfigurationRecorderNames: Sequence[str] = ...
     ) -> DescribeConfigurationRecorderStatusResponseTypeDef:
         """
-        Returns the current status of the specified configuration recorder.
+        Returns the current status of the specified configuration recorder as well as
+        the status of the last recording event for the recorder.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.describe_configuration_recorder_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#describe_configuration_recorder_status)
         """
 
     def describe_configuration_recorders(
         self, *, ConfigurationRecorderNames: Sequence[str] = ...
@@ -1160,15 +1161,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_aggregation_authorization)
         """
 
     def put_config_rule(
         self, *, ConfigRule: ConfigRuleTypeDef, Tags: Sequence[TagTypeDef] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
-        .
+        Adds or updates an Config rule to evaluate if your Amazon Web Services resources
+        comply with your desired configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_config_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_config_rule)
         """
 
     def put_configuration_aggregator(
         self,
@@ -1205,15 +1207,15 @@
         TemplateBody: str = ...,
         DeliveryS3Bucket: str = ...,
         DeliveryS3KeyPrefix: str = ...,
         ConformancePackInputParameters: Sequence[ConformancePackInputParameterTypeDef] = ...,
         TemplateSSMDocumentDetails: TemplateSSMDocumentDetailsTypeDef = ...
     ) -> PutConformancePackResponseTypeDef:
         """
-        .
+        Creates or updates a conformance pack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_conformance_pack)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_conformance_pack)
         """
 
     def put_delivery_channel(
         self, *, DeliveryChannel: DeliveryChannelTypeDef
@@ -1256,15 +1258,16 @@
         OrganizationConfigRuleName: str,
         OrganizationManagedRuleMetadata: OrganizationManagedRuleMetadataTypeDef = ...,
         OrganizationCustomRuleMetadata: OrganizationCustomRuleMetadataTypeDef = ...,
         ExcludedAccounts: Sequence[str] = ...,
         OrganizationCustomPolicyRuleMetadata: OrganizationCustomPolicyRuleMetadataTypeDef = ...
     ) -> PutOrganizationConfigRuleResponseTypeDef:
         """
-        .
+        Adds or updates an Config rule for your entire organization to evaluate if your
+        Amazon Web Services resources comply with your desired configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_organization_config_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_organization_config_rule)
         """
 
     def put_organization_conformance_pack(
         self,
@@ -1274,15 +1277,16 @@
         TemplateBody: str = ...,
         DeliveryS3Bucket: str = ...,
         DeliveryS3KeyPrefix: str = ...,
         ConformancePackInputParameters: Sequence[ConformancePackInputParameterTypeDef] = ...,
         ExcludedAccounts: Sequence[str] = ...
     ) -> PutOrganizationConformancePackResponseTypeDef:
         """
-        .
+        Deploys conformance packs across member accounts in an Amazon Web Services
+        Organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_organization_conformance_pack)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_organization_conformance_pack)
         """
 
     def put_remediation_configurations(
         self, *, RemediationConfigurations: Sequence[RemediationConfigurationTypeDef]
@@ -1300,15 +1304,15 @@
         *,
         ConfigRuleName: str,
         ResourceKeys: Sequence[RemediationExceptionResourceKeyTypeDef],
         Message: str = ...,
         ExpirationTime: Union[datetime, str] = ...
     ) -> PutRemediationExceptionsResponseTypeDef:
         """
-        A remediation exception is when a specific resource is no longer considered for
+        A remediation exception is when a specified resource is no longer considered for
         auto-remediation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_remediation_exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_remediation_exceptions)
         """
 
     def put_resource_config(
@@ -1355,25 +1359,30 @@
         Expression: str,
         ConfigurationAggregatorName: str,
         Limit: int = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> SelectAggregateResourceConfigResponseTypeDef:
         """
-        .
+        Accepts a structured query language (SQL) SELECT command and an aggregator to
+        query configuration state of Amazon Web Services resources across multiple
+        accounts and regions, performs the corresponding search, and returns resource
+        configurations matching the properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.select_aggregate_resource_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#select_aggregate_resource_config)
         """
 
     def select_resource_config(
         self, *, Expression: str, Limit: int = ..., NextToken: str = ...
     ) -> SelectResourceConfigResponseTypeDef:
         """
-        .
+        Accepts a structured query language (SQL) `SELECT` command, performs the
+        corresponding search, and returns resource configurations matching the
+        properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.select_resource_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#select_resource_config)
         """
 
     def start_config_rules_evaluation(
         self, *, ConfigRuleNames: Sequence[str] = ...
```

### Comparing `mypy-boto3-config-1.26.18/mypy_boto3_config/client.pyi` & `mypy-boto3-config-1.26.94/mypy_boto3_config/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -551,15 +551,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.describe_configuration_aggregators)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#describe_configuration_aggregators)
         """
     def describe_configuration_recorder_status(
         self, *, ConfigurationRecorderNames: Sequence[str] = ...
     ) -> DescribeConfigurationRecorderStatusResponseTypeDef:
         """
-        Returns the current status of the specified configuration recorder.
+        Returns the current status of the specified configuration recorder as well as
+        the status of the last recording event for the recorder.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.describe_configuration_recorder_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#describe_configuration_recorder_status)
         """
     def describe_configuration_recorders(
         self, *, ConfigurationRecorderNames: Sequence[str] = ...
     ) -> DescribeConfigurationRecordersResponseTypeDef:
@@ -1083,15 +1084,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_aggregation_authorization)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_aggregation_authorization)
         """
     def put_config_rule(
         self, *, ConfigRule: ConfigRuleTypeDef, Tags: Sequence[TagTypeDef] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
-        .
+        Adds or updates an Config rule to evaluate if your Amazon Web Services resources
+        comply with your desired configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_config_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_config_rule)
         """
     def put_configuration_aggregator(
         self,
         *,
@@ -1125,15 +1127,15 @@
         TemplateBody: str = ...,
         DeliveryS3Bucket: str = ...,
         DeliveryS3KeyPrefix: str = ...,
         ConformancePackInputParameters: Sequence[ConformancePackInputParameterTypeDef] = ...,
         TemplateSSMDocumentDetails: TemplateSSMDocumentDetailsTypeDef = ...
     ) -> PutConformancePackResponseTypeDef:
         """
-        .
+        Creates or updates a conformance pack.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_conformance_pack)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_conformance_pack)
         """
     def put_delivery_channel(
         self, *, DeliveryChannel: DeliveryChannelTypeDef
     ) -> EmptyResponseMetadataTypeDef:
@@ -1172,15 +1174,16 @@
         OrganizationConfigRuleName: str,
         OrganizationManagedRuleMetadata: OrganizationManagedRuleMetadataTypeDef = ...,
         OrganizationCustomRuleMetadata: OrganizationCustomRuleMetadataTypeDef = ...,
         ExcludedAccounts: Sequence[str] = ...,
         OrganizationCustomPolicyRuleMetadata: OrganizationCustomPolicyRuleMetadataTypeDef = ...
     ) -> PutOrganizationConfigRuleResponseTypeDef:
         """
-        .
+        Adds or updates an Config rule for your entire organization to evaluate if your
+        Amazon Web Services resources comply with your desired configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_organization_config_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_organization_config_rule)
         """
     def put_organization_conformance_pack(
         self,
         *,
@@ -1189,15 +1192,16 @@
         TemplateBody: str = ...,
         DeliveryS3Bucket: str = ...,
         DeliveryS3KeyPrefix: str = ...,
         ConformancePackInputParameters: Sequence[ConformancePackInputParameterTypeDef] = ...,
         ExcludedAccounts: Sequence[str] = ...
     ) -> PutOrganizationConformancePackResponseTypeDef:
         """
-        .
+        Deploys conformance packs across member accounts in an Amazon Web Services
+        Organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_organization_conformance_pack)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_organization_conformance_pack)
         """
     def put_remediation_configurations(
         self, *, RemediationConfigurations: Sequence[RemediationConfigurationTypeDef]
     ) -> PutRemediationConfigurationsResponseTypeDef:
@@ -1213,15 +1217,15 @@
         *,
         ConfigRuleName: str,
         ResourceKeys: Sequence[RemediationExceptionResourceKeyTypeDef],
         Message: str = ...,
         ExpirationTime: Union[datetime, str] = ...
     ) -> PutRemediationExceptionsResponseTypeDef:
         """
-        A remediation exception is when a specific resource is no longer considered for
+        A remediation exception is when a specified resource is no longer considered for
         auto-remediation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_remediation_exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#put_remediation_exceptions)
         """
     def put_resource_config(
         self,
@@ -1264,24 +1268,29 @@
         Expression: str,
         ConfigurationAggregatorName: str,
         Limit: int = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> SelectAggregateResourceConfigResponseTypeDef:
         """
-        .
+        Accepts a structured query language (SQL) SELECT command and an aggregator to
+        query configuration state of Amazon Web Services resources across multiple
+        accounts and regions, performs the corresponding search, and returns resource
+        configurations matching the properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.select_aggregate_resource_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#select_aggregate_resource_config)
         """
     def select_resource_config(
         self, *, Expression: str, Limit: int = ..., NextToken: str = ...
     ) -> SelectResourceConfigResponseTypeDef:
         """
-        .
+        Accepts a structured query language (SQL) `SELECT` command, performs the
+        corresponding search, and returns resource configurations matching the
+        properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.select_resource_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/client/#select_resource_config)
         """
     def start_config_rules_evaluation(
         self, *, ConfigRuleNames: Sequence[str] = ...
     ) -> Dict[str, Any]:
```

### Comparing `mypy-boto3-config-1.26.18/mypy_boto3_config/literals.py` & `mypy-boto3-config-1.26.94/mypy_boto3_config/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -230,54 +230,65 @@
 RemediationTargetTypeType = Literal["SSM_DOCUMENT"]
 ResourceConfigurationSchemaTypeType = Literal["CFN_RESOURCE_SCHEMA"]
 ResourceCountGroupKeyType = Literal["ACCOUNT_ID", "AWS_REGION", "RESOURCE_TYPE"]
 ResourceEvaluationStatusType = Literal["FAILED", "IN_PROGRESS", "SUCCEEDED"]
 ResourceTypeType = Literal[
     "AWS::ACM::Certificate",
     "AWS::AccessAnalyzer::Analyzer",
+    "AWS::AmazonMQ::Broker",
     "AWS::ApiGateway::RestApi",
     "AWS::ApiGateway::Stage",
     "AWS::ApiGatewayV2::Api",
     "AWS::ApiGatewayV2::Stage",
     "AWS::AppConfig::Application",
+    "AWS::AppConfig::ConfigurationProfile",
+    "AWS::AppConfig::Environment",
     "AWS::AppSync::GraphQLApi",
     "AWS::Athena::DataCatalog",
     "AWS::Athena::WorkGroup",
     "AWS::AutoScaling::AutoScalingGroup",
     "AWS::AutoScaling::LaunchConfiguration",
     "AWS::AutoScaling::ScalingPolicy",
     "AWS::AutoScaling::ScheduledAction",
     "AWS::Backup::BackupPlan",
     "AWS::Backup::BackupSelection",
     "AWS::Backup::BackupVault",
     "AWS::Backup::RecoveryPoint",
+    "AWS::Backup::ReportPlan",
     "AWS::Batch::ComputeEnvironment",
     "AWS::Batch::JobQueue",
+    "AWS::Budgets::BudgetsAction",
+    "AWS::Cloud9::EnvironmentEC2",
     "AWS::CloudFormation::Stack",
     "AWS::CloudFront::Distribution",
     "AWS::CloudFront::StreamingDistribution",
     "AWS::CloudTrail::Trail",
     "AWS::CloudWatch::Alarm",
     "AWS::CodeBuild::Project",
     "AWS::CodeDeploy::Application",
     "AWS::CodeDeploy::DeploymentConfig",
     "AWS::CodeDeploy::DeploymentGroup",
+    "AWS::CodeGuruReviewer::RepositoryAssociation",
     "AWS::CodePipeline::Pipeline",
     "AWS::Config::ConformancePackCompliance",
     "AWS::Config::ResourceCompliance",
     "AWS::DMS::Certificate",
     "AWS::DMS::EventSubscription",
     "AWS::DMS::ReplicationSubnetGroup",
     "AWS::DataSync::LocationEFS",
     "AWS::DataSync::LocationFSxLustre",
+    "AWS::DataSync::LocationFSxWindows",
+    "AWS::DataSync::LocationHDFS",
     "AWS::DataSync::LocationNFS",
+    "AWS::DataSync::LocationObjectStorage",
     "AWS::DataSync::LocationS3",
     "AWS::DataSync::LocationSMB",
     "AWS::DataSync::Task",
     "AWS::Detective::Graph",
+    "AWS::DeviceFarm::TestGridProject",
     "AWS::DynamoDB::Table",
     "AWS::EC2::CustomerGateway",
     "AWS::EC2::EIP",
     "AWS::EC2::EgressOnlyInternetGateway",
     "AWS::EC2::FlowLog",
     "AWS::EC2::Host",
     "AWS::EC2::Instance",
@@ -287,103 +298,179 @@
     "AWS::EC2::NetworkAcl",
     "AWS::EC2::NetworkInsightsAccessScopeAnalysis",
     "AWS::EC2::NetworkInterface",
     "AWS::EC2::RegisteredHAInstance",
     "AWS::EC2::RouteTable",
     "AWS::EC2::SecurityGroup",
     "AWS::EC2::Subnet",
+    "AWS::EC2::TrafficMirrorSession",
+    "AWS::EC2::TrafficMirrorTarget",
     "AWS::EC2::TransitGateway",
     "AWS::EC2::TransitGatewayAttachment",
     "AWS::EC2::TransitGatewayRouteTable",
     "AWS::EC2::VPC",
     "AWS::EC2::VPCEndpoint",
     "AWS::EC2::VPCEndpointService",
     "AWS::EC2::VPCPeeringConnection",
     "AWS::EC2::VPNConnection",
     "AWS::EC2::VPNGateway",
     "AWS::EC2::Volume",
     "AWS::ECR::PublicRepository",
+    "AWS::ECR::RegistryPolicy",
     "AWS::ECR::Repository",
     "AWS::ECS::Cluster",
     "AWS::ECS::Service",
     "AWS::ECS::TaskDefinition",
     "AWS::EFS::AccessPoint",
     "AWS::EFS::FileSystem",
+    "AWS::EKS::Addon",
     "AWS::EKS::Cluster",
     "AWS::EKS::FargateProfile",
+    "AWS::EKS::IdentityProviderConfig",
     "AWS::EMR::SecurityConfiguration",
     "AWS::ElasticBeanstalk::Application",
     "AWS::ElasticBeanstalk::ApplicationVersion",
     "AWS::ElasticBeanstalk::Environment",
     "AWS::ElasticLoadBalancing::LoadBalancer",
     "AWS::ElasticLoadBalancingV2::Listener",
     "AWS::ElasticLoadBalancingV2::LoadBalancer",
     "AWS::Elasticsearch::Domain",
+    "AWS::EventSchemas::Discoverer",
+    "AWS::EventSchemas::Registry",
+    "AWS::EventSchemas::RegistryPolicy",
+    "AWS::EventSchemas::Schema",
+    "AWS::Events::ApiDestination",
+    "AWS::Events::Archive",
+    "AWS::Events::Connection",
+    "AWS::Events::Endpoint",
+    "AWS::Events::EventBus",
+    "AWS::FIS::ExperimentTemplate",
+    "AWS::FraudDetector::EntityType",
+    "AWS::FraudDetector::Label",
+    "AWS::FraudDetector::Outcome",
+    "AWS::FraudDetector::Variable",
     "AWS::GlobalAccelerator::Accelerator",
     "AWS::GlobalAccelerator::EndpointGroup",
     "AWS::GlobalAccelerator::Listener",
+    "AWS::Glue::Classifier",
     "AWS::Glue::Job",
+    "AWS::Glue::MLTransform",
     "AWS::GuardDuty::Detector",
+    "AWS::GuardDuty::Filter",
     "AWS::GuardDuty::IPSet",
     "AWS::GuardDuty::ThreatIntelSet",
     "AWS::IAM::Group",
     "AWS::IAM::Policy",
     "AWS::IAM::Role",
     "AWS::IAM::User",
+    "AWS::IVS::Channel",
+    "AWS::IVS::PlaybackKeyPair",
+    "AWS::IVS::RecordingConfiguration",
+    "AWS::ImageBuilder::ContainerRecipe",
+    "AWS::ImageBuilder::DistributionConfiguration",
+    "AWS::ImageBuilder::InfrastructureConfiguration",
+    "AWS::IoT::AccountAuditConfiguration",
+    "AWS::IoT::Authorizer",
+    "AWS::IoT::CustomMetric",
+    "AWS::IoT::Dimension",
+    "AWS::IoT::MitigationAction",
+    "AWS::IoT::Policy",
+    "AWS::IoT::RoleAlias",
+    "AWS::IoT::ScheduledAudit",
+    "AWS::IoT::SecurityProfile",
+    "AWS::IoTAnalytics::Channel",
+    "AWS::IoTAnalytics::Dataset",
+    "AWS::IoTAnalytics::Datastore",
+    "AWS::IoTAnalytics::Pipeline",
+    "AWS::IoTEvents::AlarmModel",
+    "AWS::IoTEvents::DetectorModel",
+    "AWS::IoTEvents::Input",
+    "AWS::IoTSiteWise::AssetModel",
+    "AWS::IoTSiteWise::Dashboard",
+    "AWS::IoTSiteWise::Gateway",
+    "AWS::IoTSiteWise::Portal",
+    "AWS::IoTSiteWise::Project",
+    "AWS::IoTTwinMaker::Entity",
+    "AWS::IoTTwinMaker::Workspace",
     "AWS::KMS::Key",
     "AWS::Kinesis::Stream",
     "AWS::Kinesis::StreamConsumer",
+    "AWS::KinesisAnalyticsV2::Application",
     "AWS::Lambda::Function",
+    "AWS::Lex::Bot",
+    "AWS::Lex::BotAlias",
+    "AWS::Lightsail::Bucket",
+    "AWS::Lightsail::Certificate",
+    "AWS::Lightsail::Disk",
+    "AWS::Lightsail::StaticIp",
+    "AWS::LookoutMetrics::Alert",
     "AWS::MSK::Cluster",
+    "AWS::MediaPackage::PackagingConfiguration",
+    "AWS::MediaPackage::PackagingGroup",
     "AWS::NetworkFirewall::Firewall",
     "AWS::NetworkFirewall::FirewallPolicy",
     "AWS::NetworkFirewall::RuleGroup",
     "AWS::OpenSearch::Domain",
     "AWS::QLDB::Ledger",
     "AWS::RDS::DBCluster",
     "AWS::RDS::DBClusterSnapshot",
     "AWS::RDS::DBInstance",
     "AWS::RDS::DBSecurityGroup",
     "AWS::RDS::DBSnapshot",
     "AWS::RDS::DBSubnetGroup",
     "AWS::RDS::EventSubscription",
+    "AWS::RDS::GlobalCluster",
+    "AWS::RUM::AppMonitor",
     "AWS::Redshift::Cluster",
     "AWS::Redshift::ClusterParameterGroup",
     "AWS::Redshift::ClusterSecurityGroup",
     "AWS::Redshift::ClusterSnapshot",
     "AWS::Redshift::ClusterSubnetGroup",
     "AWS::Redshift::EventSubscription",
+    "AWS::ResilienceHub::ResiliencyPolicy",
+    "AWS::RoboMaker::RobotApplicationVersion",
     "AWS::Route53::HostedZone",
+    "AWS::Route53RecoveryReadiness::Cell",
+    "AWS::Route53RecoveryReadiness::ReadinessCheck",
+    "AWS::Route53RecoveryReadiness::RecoveryGroup",
+    "AWS::Route53Resolver::FirewallDomainList",
     "AWS::Route53Resolver::ResolverEndpoint",
     "AWS::Route53Resolver::ResolverRule",
     "AWS::Route53Resolver::ResolverRuleAssociation",
     "AWS::S3::AccountPublicAccessBlock",
     "AWS::S3::Bucket",
+    "AWS::S3::MultiRegionAccessPoint",
+    "AWS::S3::StorageLens",
     "AWS::SES::ConfigurationSet",
     "AWS::SES::ContactList",
+    "AWS::SES::ReceiptFilter",
+    "AWS::SES::ReceiptRuleSet",
+    "AWS::SES::Template",
     "AWS::SNS::Topic",
     "AWS::SQS::Queue",
     "AWS::SSM::AssociationCompliance",
     "AWS::SSM::FileData",
     "AWS::SSM::ManagedInstanceInventory",
     "AWS::SSM::PatchCompliance",
     "AWS::SageMaker::CodeRepository",
     "AWS::SageMaker::Model",
     "AWS::SageMaker::NotebookInstanceLifecycleConfig",
     "AWS::SageMaker::Workteam",
     "AWS::SecretsManager::Secret",
     "AWS::ServiceCatalog::CloudFormationProduct",
     "AWS::ServiceCatalog::CloudFormationProvisionedProduct",
     "AWS::ServiceCatalog::Portfolio",
+    "AWS::ServiceDiscovery::HttpNamespace",
     "AWS::ServiceDiscovery::PublicDnsNamespace",
     "AWS::ServiceDiscovery::Service",
     "AWS::Shield::Protection",
     "AWS::ShieldRegional::Protection",
     "AWS::StepFunctions::Activity",
     "AWS::StepFunctions::StateMachine",
+    "AWS::Transfer::Workflow",
     "AWS::WAF::RateBasedRule",
     "AWS::WAF::Rule",
     "AWS::WAF::RuleGroup",
     "AWS::WAF::WebACL",
     "AWS::WAFRegional::RateBasedRule",
     "AWS::WAFRegional::Rule",
     "AWS::WAFRegional::RuleGroup",
@@ -442,27 +529,30 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -491,14 +581,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -543,14 +634,15 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -565,30 +657,33 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -621,28 +716,31 @@
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
     "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -670,30 +768,34 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
@@ -709,14 +811,15 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
@@ -782,14 +885,15 @@
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
```

### Comparing `mypy-boto3-config-1.26.18/mypy_boto3_config/literals.pyi` & `mypy-boto3-config-1.26.94/mypy_boto3_config/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -228,54 +228,65 @@
 RemediationTargetTypeType = Literal["SSM_DOCUMENT"]
 ResourceConfigurationSchemaTypeType = Literal["CFN_RESOURCE_SCHEMA"]
 ResourceCountGroupKeyType = Literal["ACCOUNT_ID", "AWS_REGION", "RESOURCE_TYPE"]
 ResourceEvaluationStatusType = Literal["FAILED", "IN_PROGRESS", "SUCCEEDED"]
 ResourceTypeType = Literal[
     "AWS::ACM::Certificate",
     "AWS::AccessAnalyzer::Analyzer",
+    "AWS::AmazonMQ::Broker",
     "AWS::ApiGateway::RestApi",
     "AWS::ApiGateway::Stage",
     "AWS::ApiGatewayV2::Api",
     "AWS::ApiGatewayV2::Stage",
     "AWS::AppConfig::Application",
+    "AWS::AppConfig::ConfigurationProfile",
+    "AWS::AppConfig::Environment",
     "AWS::AppSync::GraphQLApi",
     "AWS::Athena::DataCatalog",
     "AWS::Athena::WorkGroup",
     "AWS::AutoScaling::AutoScalingGroup",
     "AWS::AutoScaling::LaunchConfiguration",
     "AWS::AutoScaling::ScalingPolicy",
     "AWS::AutoScaling::ScheduledAction",
     "AWS::Backup::BackupPlan",
     "AWS::Backup::BackupSelection",
     "AWS::Backup::BackupVault",
     "AWS::Backup::RecoveryPoint",
+    "AWS::Backup::ReportPlan",
     "AWS::Batch::ComputeEnvironment",
     "AWS::Batch::JobQueue",
+    "AWS::Budgets::BudgetsAction",
+    "AWS::Cloud9::EnvironmentEC2",
     "AWS::CloudFormation::Stack",
     "AWS::CloudFront::Distribution",
     "AWS::CloudFront::StreamingDistribution",
     "AWS::CloudTrail::Trail",
     "AWS::CloudWatch::Alarm",
     "AWS::CodeBuild::Project",
     "AWS::CodeDeploy::Application",
     "AWS::CodeDeploy::DeploymentConfig",
     "AWS::CodeDeploy::DeploymentGroup",
+    "AWS::CodeGuruReviewer::RepositoryAssociation",
     "AWS::CodePipeline::Pipeline",
     "AWS::Config::ConformancePackCompliance",
     "AWS::Config::ResourceCompliance",
     "AWS::DMS::Certificate",
     "AWS::DMS::EventSubscription",
     "AWS::DMS::ReplicationSubnetGroup",
     "AWS::DataSync::LocationEFS",
     "AWS::DataSync::LocationFSxLustre",
+    "AWS::DataSync::LocationFSxWindows",
+    "AWS::DataSync::LocationHDFS",
     "AWS::DataSync::LocationNFS",
+    "AWS::DataSync::LocationObjectStorage",
     "AWS::DataSync::LocationS3",
     "AWS::DataSync::LocationSMB",
     "AWS::DataSync::Task",
     "AWS::Detective::Graph",
+    "AWS::DeviceFarm::TestGridProject",
     "AWS::DynamoDB::Table",
     "AWS::EC2::CustomerGateway",
     "AWS::EC2::EIP",
     "AWS::EC2::EgressOnlyInternetGateway",
     "AWS::EC2::FlowLog",
     "AWS::EC2::Host",
     "AWS::EC2::Instance",
@@ -285,103 +296,179 @@
     "AWS::EC2::NetworkAcl",
     "AWS::EC2::NetworkInsightsAccessScopeAnalysis",
     "AWS::EC2::NetworkInterface",
     "AWS::EC2::RegisteredHAInstance",
     "AWS::EC2::RouteTable",
     "AWS::EC2::SecurityGroup",
     "AWS::EC2::Subnet",
+    "AWS::EC2::TrafficMirrorSession",
+    "AWS::EC2::TrafficMirrorTarget",
     "AWS::EC2::TransitGateway",
     "AWS::EC2::TransitGatewayAttachment",
     "AWS::EC2::TransitGatewayRouteTable",
     "AWS::EC2::VPC",
     "AWS::EC2::VPCEndpoint",
     "AWS::EC2::VPCEndpointService",
     "AWS::EC2::VPCPeeringConnection",
     "AWS::EC2::VPNConnection",
     "AWS::EC2::VPNGateway",
     "AWS::EC2::Volume",
     "AWS::ECR::PublicRepository",
+    "AWS::ECR::RegistryPolicy",
     "AWS::ECR::Repository",
     "AWS::ECS::Cluster",
     "AWS::ECS::Service",
     "AWS::ECS::TaskDefinition",
     "AWS::EFS::AccessPoint",
     "AWS::EFS::FileSystem",
+    "AWS::EKS::Addon",
     "AWS::EKS::Cluster",
     "AWS::EKS::FargateProfile",
+    "AWS::EKS::IdentityProviderConfig",
     "AWS::EMR::SecurityConfiguration",
     "AWS::ElasticBeanstalk::Application",
     "AWS::ElasticBeanstalk::ApplicationVersion",
     "AWS::ElasticBeanstalk::Environment",
     "AWS::ElasticLoadBalancing::LoadBalancer",
     "AWS::ElasticLoadBalancingV2::Listener",
     "AWS::ElasticLoadBalancingV2::LoadBalancer",
     "AWS::Elasticsearch::Domain",
+    "AWS::EventSchemas::Discoverer",
+    "AWS::EventSchemas::Registry",
+    "AWS::EventSchemas::RegistryPolicy",
+    "AWS::EventSchemas::Schema",
+    "AWS::Events::ApiDestination",
+    "AWS::Events::Archive",
+    "AWS::Events::Connection",
+    "AWS::Events::Endpoint",
+    "AWS::Events::EventBus",
+    "AWS::FIS::ExperimentTemplate",
+    "AWS::FraudDetector::EntityType",
+    "AWS::FraudDetector::Label",
+    "AWS::FraudDetector::Outcome",
+    "AWS::FraudDetector::Variable",
     "AWS::GlobalAccelerator::Accelerator",
     "AWS::GlobalAccelerator::EndpointGroup",
     "AWS::GlobalAccelerator::Listener",
+    "AWS::Glue::Classifier",
     "AWS::Glue::Job",
+    "AWS::Glue::MLTransform",
     "AWS::GuardDuty::Detector",
+    "AWS::GuardDuty::Filter",
     "AWS::GuardDuty::IPSet",
     "AWS::GuardDuty::ThreatIntelSet",
     "AWS::IAM::Group",
     "AWS::IAM::Policy",
     "AWS::IAM::Role",
     "AWS::IAM::User",
+    "AWS::IVS::Channel",
+    "AWS::IVS::PlaybackKeyPair",
+    "AWS::IVS::RecordingConfiguration",
+    "AWS::ImageBuilder::ContainerRecipe",
+    "AWS::ImageBuilder::DistributionConfiguration",
+    "AWS::ImageBuilder::InfrastructureConfiguration",
+    "AWS::IoT::AccountAuditConfiguration",
+    "AWS::IoT::Authorizer",
+    "AWS::IoT::CustomMetric",
+    "AWS::IoT::Dimension",
+    "AWS::IoT::MitigationAction",
+    "AWS::IoT::Policy",
+    "AWS::IoT::RoleAlias",
+    "AWS::IoT::ScheduledAudit",
+    "AWS::IoT::SecurityProfile",
+    "AWS::IoTAnalytics::Channel",
+    "AWS::IoTAnalytics::Dataset",
+    "AWS::IoTAnalytics::Datastore",
+    "AWS::IoTAnalytics::Pipeline",
+    "AWS::IoTEvents::AlarmModel",
+    "AWS::IoTEvents::DetectorModel",
+    "AWS::IoTEvents::Input",
+    "AWS::IoTSiteWise::AssetModel",
+    "AWS::IoTSiteWise::Dashboard",
+    "AWS::IoTSiteWise::Gateway",
+    "AWS::IoTSiteWise::Portal",
+    "AWS::IoTSiteWise::Project",
+    "AWS::IoTTwinMaker::Entity",
+    "AWS::IoTTwinMaker::Workspace",
     "AWS::KMS::Key",
     "AWS::Kinesis::Stream",
     "AWS::Kinesis::StreamConsumer",
+    "AWS::KinesisAnalyticsV2::Application",
     "AWS::Lambda::Function",
+    "AWS::Lex::Bot",
+    "AWS::Lex::BotAlias",
+    "AWS::Lightsail::Bucket",
+    "AWS::Lightsail::Certificate",
+    "AWS::Lightsail::Disk",
+    "AWS::Lightsail::StaticIp",
+    "AWS::LookoutMetrics::Alert",
     "AWS::MSK::Cluster",
+    "AWS::MediaPackage::PackagingConfiguration",
+    "AWS::MediaPackage::PackagingGroup",
     "AWS::NetworkFirewall::Firewall",
     "AWS::NetworkFirewall::FirewallPolicy",
     "AWS::NetworkFirewall::RuleGroup",
     "AWS::OpenSearch::Domain",
     "AWS::QLDB::Ledger",
     "AWS::RDS::DBCluster",
     "AWS::RDS::DBClusterSnapshot",
     "AWS::RDS::DBInstance",
     "AWS::RDS::DBSecurityGroup",
     "AWS::RDS::DBSnapshot",
     "AWS::RDS::DBSubnetGroup",
     "AWS::RDS::EventSubscription",
+    "AWS::RDS::GlobalCluster",
+    "AWS::RUM::AppMonitor",
     "AWS::Redshift::Cluster",
     "AWS::Redshift::ClusterParameterGroup",
     "AWS::Redshift::ClusterSecurityGroup",
     "AWS::Redshift::ClusterSnapshot",
     "AWS::Redshift::ClusterSubnetGroup",
     "AWS::Redshift::EventSubscription",
+    "AWS::ResilienceHub::ResiliencyPolicy",
+    "AWS::RoboMaker::RobotApplicationVersion",
     "AWS::Route53::HostedZone",
+    "AWS::Route53RecoveryReadiness::Cell",
+    "AWS::Route53RecoveryReadiness::ReadinessCheck",
+    "AWS::Route53RecoveryReadiness::RecoveryGroup",
+    "AWS::Route53Resolver::FirewallDomainList",
     "AWS::Route53Resolver::ResolverEndpoint",
     "AWS::Route53Resolver::ResolverRule",
     "AWS::Route53Resolver::ResolverRuleAssociation",
     "AWS::S3::AccountPublicAccessBlock",
     "AWS::S3::Bucket",
+    "AWS::S3::MultiRegionAccessPoint",
+    "AWS::S3::StorageLens",
     "AWS::SES::ConfigurationSet",
     "AWS::SES::ContactList",
+    "AWS::SES::ReceiptFilter",
+    "AWS::SES::ReceiptRuleSet",
+    "AWS::SES::Template",
     "AWS::SNS::Topic",
     "AWS::SQS::Queue",
     "AWS::SSM::AssociationCompliance",
     "AWS::SSM::FileData",
     "AWS::SSM::ManagedInstanceInventory",
     "AWS::SSM::PatchCompliance",
     "AWS::SageMaker::CodeRepository",
     "AWS::SageMaker::Model",
     "AWS::SageMaker::NotebookInstanceLifecycleConfig",
     "AWS::SageMaker::Workteam",
     "AWS::SecretsManager::Secret",
     "AWS::ServiceCatalog::CloudFormationProduct",
     "AWS::ServiceCatalog::CloudFormationProvisionedProduct",
     "AWS::ServiceCatalog::Portfolio",
+    "AWS::ServiceDiscovery::HttpNamespace",
     "AWS::ServiceDiscovery::PublicDnsNamespace",
     "AWS::ServiceDiscovery::Service",
     "AWS::Shield::Protection",
     "AWS::ShieldRegional::Protection",
     "AWS::StepFunctions::Activity",
     "AWS::StepFunctions::StateMachine",
+    "AWS::Transfer::Workflow",
     "AWS::WAF::RateBasedRule",
     "AWS::WAF::Rule",
     "AWS::WAF::RuleGroup",
     "AWS::WAF::WebACL",
     "AWS::WAFRegional::RateBasedRule",
     "AWS::WAFRegional::Rule",
     "AWS::WAFRegional::RuleGroup",
@@ -440,27 +527,30 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -489,14 +579,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -541,14 +632,15 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -563,30 +655,33 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -619,28 +714,31 @@
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
     "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -668,30 +766,34 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
@@ -707,14 +809,15 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
@@ -780,14 +883,15 @@
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
```

### Comparing `mypy-boto3-config-1.26.18/mypy_boto3_config/paginator.py` & `mypy-boto3-config-1.26.94/mypy_boto3_config/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.26.18/mypy_boto3_config/paginator.pyi` & `mypy-boto3-config-1.26.94/mypy_boto3_config/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.26.18/mypy_boto3_config/type_defs.py` & `mypy-boto3-config-1.26.94/mypy_boto3_config/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.26.18/mypy_boto3_config/type_defs.pyi` & `mypy-boto3-config-1.26.94/mypy_boto3_config/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.26.18/mypy_boto3_config.egg-info/PKG-INFO` & `mypy-boto3-config-1.26.94/mypy_boto3_config.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-config
-Version: 1.26.18
-Summary: Type annotations for boto3.ConfigService 1.26.18 service generated with mypy-boto3-builder 7.11.11
+Version: 1.26.94
+Summary: Type annotations for boto3.ConfigService 1.26.94 service generated with mypy-boto3-builder 7.13.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,14 +18,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -37,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-config.svg?color=blue)](https://pypi.org/project/mypy-boto3-config)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-config?color=blue)](https://pypistats.org/packages/mypy-boto3-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConfigService 1.26.18](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService)
+[boto3.ConfigService 1.26.94](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-config docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-config-1.26.18/mypy_boto3_config.egg-info/SOURCES.txt` & `mypy-boto3-config-1.26.94/mypy_boto3_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-config-1.26.18/setup.py` & `mypy-boto3-config-1.26.94/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,45 +6,46 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-config",
-    version="1.26.18",
+    version="1.26.94",
     packages=["mypy_boto3_config"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ConfigService 1.26.18 service generated with mypy-boto3-builder"
-        " 7.11.11"
+        "Type annotations for boto3.ConfigService 1.26.94 service generated with mypy-boto3-builder"
+        " 7.13.0"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords="boto3 config type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_config": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_config": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_config/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
```

