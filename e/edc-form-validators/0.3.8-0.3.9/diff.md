# Comparing `tmp/edc-form-validators-0.3.8.tar.gz` & `tmp/edc-form-validators-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-form-validators-0.3.8.tar", last modified: Wed Mar 16 23:08:26 2022, max compression
+gzip compressed data, was "edc-form-validators-0.3.9.tar", last modified: Mon Apr 11 13:06:24 2022, max compression
```

## Comparing `edc-form-validators-0.3.8.tar` & `edc-form-validators-0.3.9.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-03-16 23:08:26.857283 edc-form-validators-0.3.8/
--rw-r--r--   0 erikvw     (501) staff       (20)    35147 2020-03-04 23:24:33.000000 edc-form-validators-0.3.8/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)      185 2020-03-04 23:24:55.000000 edc-form-validators-0.3.8/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     2758 2022-03-16 23:08:26.857339 edc-form-validators-0.3.8/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1893 2021-02-04 19:06:59.000000 edc-form-validators-0.3.8/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-03-16 23:08:09.000000 edc-form-validators-0.3.8/VERSION
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-03-16 23:08:26.854369 edc-form-validators-0.3.8/edc_form_validators/
--rw-r--r--   0 erikvw     (501) staff       (20)      692 2021-02-04 19:06:59.000000 edc-form-validators-0.3.8/edc_form_validators/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7079 2021-08-17 21:54:27.000000 edc-form-validators-0.3.8/edc_form_validators/applicable_field_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)      122 2020-03-04 23:24:33.000000 edc-form-validators-0.3.8/edc_form_validators/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4969 2021-08-17 21:54:27.000000 edc-form-validators-0.3.8/edc_form_validators/base_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3790 2021-12-17 22:22:03.000000 edc-form-validators-0.3.8/edc_form_validators/date_range_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2155 2022-03-16 23:08:09.000000 edc-form-validators-0.3.8/edc_form_validators/date_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2233 2022-02-16 19:49:18.000000 edc-form-validators-0.3.8/edc_form_validators/extra_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)      720 2022-03-16 23:08:09.000000 edc-form-validators-0.3.8/edc_form_validators/form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)      659 2021-08-10 05:40:21.000000 edc-form-validators-0.3.8/edc_form_validators/form_validator_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)    13690 2021-03-01 03:42:10.000000 edc-form-validators-0.3.8/edc_form_validators/many_to_many_field_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2801 2021-08-10 05:40:21.000000 edc-form-validators-0.3.8/edc_form_validators/other_specify_field_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1551 2021-03-01 03:42:10.000000 edc-form-validators-0.3.8/edc_form_validators/range_field_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)    11640 2021-08-17 21:54:27.000000 edc-form-validators-0.3.8/edc_form_validators/required_field_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1613 2022-02-02 03:01:30.000000 edc-form-validators-0.3.8/edc_form_validators/test_case_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-03-16 23:08:26.856102 edc-form-validators-0.3.8/edc_form_validators/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:24:33.000000 edc-form-validators-0.3.8/edc_form_validators/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3132 2021-02-04 19:06:59.000000 edc-form-validators-0.3.8/edc_form_validators/tests/test_applicable.py
--rw-r--r--   0 erikvw     (501) staff       (20)     9327 2021-02-04 19:06:59.000000 edc-form-validators-0.3.8/edc_form_validators/tests/test_m2m_validators.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3004 2021-02-04 19:06:59.000000 edc-form-validators-0.3.8/edc_form_validators/tests/test_modelform_validators.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5295 2021-02-04 19:06:59.000000 edc-form-validators-0.3.8/edc_form_validators/tests/test_not_required.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2214 2021-02-04 19:06:59.000000 edc-form-validators-0.3.8/edc_form_validators/tests/test_other_specify.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2978 2021-02-04 19:06:59.000000 edc-form-validators-0.3.8/edc_form_validators/tests/test_out_of_range.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4537 2021-02-04 19:06:59.000000 edc-form-validators-0.3.8/edc_form_validators/tests/test_required.py
--rw-r--r--   0 erikvw     (501) staff       (20)      754 2020-03-04 23:24:33.000000 edc-form-validators-0.3.8/edc_form_validators/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-03-16 23:08:26.855027 edc-form-validators-0.3.8/edc_form_validators.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     2758 2022-03-16 23:08:26.000000 edc-form-validators-0.3.8/edc_form_validators.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1542 2022-03-16 23:08:26.000000 edc-form-validators-0.3.8/edc_form_validators.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-03-16 23:08:26.000000 edc-form-validators-0.3.8/edc_form_validators.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-03-04 23:24:55.000000 edc-form-validators-0.3.8/edc_form_validators.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       40 2022-03-16 23:08:26.000000 edc-form-validators-0.3.8/edc_form_validators.egg-info/top_level.txt
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-03-16 23:08:26.857092 edc-form-validators-0.3.8/form_validators_app/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:24:33.000000 edc-form-validators-0.3.8/form_validators_app/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      239 2020-03-04 23:24:33.000000 edc-form-validators-0.3.8/form_validators_app/admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      122 2021-02-04 19:06:59.000000 edc-form-validators-0.3.8/form_validators_app/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      540 2021-02-04 19:06:59.000000 edc-form-validators-0.3.8/form_validators_app/forms.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-03-16 23:08:26.857215 edc-form-validators-0.3.8/form_validators_app/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:24:33.000000 edc-form-validators-0.3.8/form_validators_app/migrations/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      572 2020-06-25 05:16:24.000000 edc-form-validators-0.3.8/form_validators_app/models.py
--rw-r--r--   0 erikvw     (501) staff       (20)       60 2020-03-04 23:24:33.000000 edc-form-validators-0.3.8/form_validators_app/tests.py
--rw-r--r--   0 erikvw     (501) staff       (20)       63 2020-03-04 23:24:33.000000 edc-form-validators-0.3.8/form_validators_app/views.py
--rw-r--r--   0 erikvw     (501) staff       (20)      360 2021-02-04 19:06:59.000000 edc-form-validators-0.3.8/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 22:48:42.000000 edc-form-validators-0.3.8/requirements.txt
--rw-r--r--   0 erikvw     (501) staff       (20)      165 2022-03-16 23:08:26.857780 edc-form-validators-0.3.8/setup.cfg
--rw-r--r--   0 erikvw     (501) staff       (20)     1418 2022-02-16 19:49:18.000000 edc-form-validators-0.3.8/setup.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-11 13:06:24.593309 edc-form-validators-0.3.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)    35147 2020-03-04 23:24:33.000000 edc-form-validators-0.3.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      185 2020-03-04 23:24:55.000000 edc-form-validators-0.3.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     2758 2022-04-11 13:06:24.593381 edc-form-validators-0.3.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1893 2021-02-04 19:06:59.000000 edc-form-validators-0.3.9/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-04-11 13:06:15.000000 edc-form-validators-0.3.9/VERSION
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-11 13:06:24.590041 edc-form-validators-0.3.9/edc_form_validators/
+-rw-r--r--   0 erikvw     (501) staff       (20)      692 2021-02-04 19:06:59.000000 edc-form-validators-0.3.9/edc_form_validators/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7079 2021-08-17 21:54:27.000000 edc-form-validators-0.3.9/edc_form_validators/applicable_field_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      122 2020-03-04 23:24:33.000000 edc-form-validators-0.3.9/edc_form_validators/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4969 2021-08-17 21:54:27.000000 edc-form-validators-0.3.9/edc_form_validators/base_form_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3790 2021-12-17 22:22:03.000000 edc-form-validators-0.3.9/edc_form_validators/date_range_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3550 2022-04-11 13:06:15.000000 edc-form-validators-0.3.9/edc_form_validators/date_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2233 2022-02-16 19:49:18.000000 edc-form-validators-0.3.9/edc_form_validators/extra_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      720 2022-03-16 23:08:09.000000 edc-form-validators-0.3.9/edc_form_validators/form_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      659 2022-04-11 11:07:02.000000 edc-form-validators-0.3.9/edc_form_validators/form_validator_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    13690 2021-03-01 03:42:10.000000 edc-form-validators-0.3.9/edc_form_validators/many_to_many_field_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2801 2021-08-10 05:40:21.000000 edc-form-validators-0.3.9/edc_form_validators/other_specify_field_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1551 2021-03-01 03:42:10.000000 edc-form-validators-0.3.9/edc_form_validators/range_field_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    11640 2021-08-17 21:54:27.000000 edc-form-validators-0.3.9/edc_form_validators/required_field_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1613 2022-02-02 03:01:30.000000 edc-form-validators-0.3.9/edc_form_validators/test_case_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-11 13:06:24.591813 edc-form-validators-0.3.9/edc_form_validators/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:24:33.000000 edc-form-validators-0.3.9/edc_form_validators/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3132 2021-02-04 19:06:59.000000 edc-form-validators-0.3.9/edc_form_validators/tests/test_applicable.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      987 2022-04-11 13:06:15.000000 edc-form-validators-0.3.9/edc_form_validators/tests/test_dates.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     9327 2021-02-04 19:06:59.000000 edc-form-validators-0.3.9/edc_form_validators/tests/test_m2m_validators.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3004 2021-02-04 19:06:59.000000 edc-form-validators-0.3.9/edc_form_validators/tests/test_modelform_validators.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5295 2021-02-04 19:06:59.000000 edc-form-validators-0.3.9/edc_form_validators/tests/test_not_required.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2214 2021-02-04 19:06:59.000000 edc-form-validators-0.3.9/edc_form_validators/tests/test_other_specify.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2978 2021-02-04 19:06:59.000000 edc-form-validators-0.3.9/edc_form_validators/tests/test_out_of_range.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4537 2021-02-04 19:06:59.000000 edc-form-validators-0.3.9/edc_form_validators/tests/test_required.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      754 2020-03-04 23:24:33.000000 edc-form-validators-0.3.9/edc_form_validators/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-11 13:06:24.590700 edc-form-validators-0.3.9/edc_form_validators.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2758 2022-04-11 13:06:24.000000 edc-form-validators-0.3.9/edc_form_validators.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1582 2022-04-11 13:06:24.000000 edc-form-validators-0.3.9/edc_form_validators.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-04-11 13:06:24.000000 edc-form-validators-0.3.9/edc_form_validators.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-03-04 23:24:55.000000 edc-form-validators-0.3.9/edc_form_validators.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       40 2022-04-11 13:06:24.000000 edc-form-validators-0.3.9/edc_form_validators.egg-info/top_level.txt
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-11 13:06:24.592881 edc-form-validators-0.3.9/form_validators_app/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:24:33.000000 edc-form-validators-0.3.9/form_validators_app/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      239 2020-03-04 23:24:33.000000 edc-form-validators-0.3.9/form_validators_app/admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      122 2021-02-04 19:06:59.000000 edc-form-validators-0.3.9/form_validators_app/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      540 2021-02-04 19:06:59.000000 edc-form-validators-0.3.9/form_validators_app/forms.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-04-11 13:06:24.593220 edc-form-validators-0.3.9/form_validators_app/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:24:33.000000 edc-form-validators-0.3.9/form_validators_app/migrations/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      572 2020-06-25 05:16:24.000000 edc-form-validators-0.3.9/form_validators_app/models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       60 2020-03-04 23:24:33.000000 edc-form-validators-0.3.9/form_validators_app/tests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       63 2020-03-04 23:24:33.000000 edc-form-validators-0.3.9/form_validators_app/views.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      360 2021-02-04 19:06:59.000000 edc-form-validators-0.3.9/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 22:48:42.000000 edc-form-validators-0.3.9/requirements.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)      165 2022-04-11 13:06:24.593595 edc-form-validators-0.3.9/setup.cfg
+-rw-r--r--   0 erikvw     (501) staff       (20)     1418 2022-02-16 19:49:18.000000 edc-form-validators-0.3.9/setup.py
```

### Comparing `edc-form-validators-0.3.8/LICENSE` & `edc-form-validators-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-form-validators-0.3.8/PKG-INFO` & `edc-form-validators-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-form-validators
-Version: 0.3.8
+Version: 0.3.9
 Summary: Form validator classes for django ModelForms
 Home-page: https://github.com/clinicedc/edc-form-validators
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django modelform form validation edc
 Platform: UNKNOWN
```

### Comparing `edc-form-validators-0.3.8/README.rst` & `edc-form-validators-0.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `edc-form-validators-0.3.8/edc_form_validators/__init__.py` & `edc-form-validators-0.3.9/edc_form_validators/__init__.py`

 * *Files identical despite different names*

### Comparing `edc-form-validators-0.3.8/edc_form_validators/applicable_field_validator.py` & `edc-form-validators-0.3.9/edc_form_validators/applicable_field_validator.py`

 * *Files identical despite different names*

### Comparing `edc-form-validators-0.3.8/edc_form_validators/base_form_validator.py` & `edc-form-validators-0.3.9/edc_form_validators/base_form_validator.py`

 * *Files identical despite different names*

### Comparing `edc-form-validators-0.3.8/edc_form_validators/date_range_validator.py` & `edc-form-validators-0.3.9/edc_form_validators/date_range_validator.py`

 * *Files identical despite different names*

### Comparing `edc-form-validators-0.3.8/edc_form_validators/extra_mixins.py` & `edc-form-validators-0.3.9/edc_form_validators/extra_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-form-validators-0.3.8/edc_form_validators/form_validator.py` & `edc-form-validators-0.3.9/edc_form_validators/form_validator.py`

 * *Files identical despite different names*

### Comparing `edc-form-validators-0.3.8/edc_form_validators/form_validator_mixin.py` & `edc-form-validators-0.3.9/edc_form_validators/form_validator_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-form-validators-0.3.8/edc_form_validators/many_to_many_field_validator.py` & `edc-form-validators-0.3.9/edc_form_validators/many_to_many_field_validator.py`

 * *Files identical despite different names*

### Comparing `edc-form-validators-0.3.8/edc_form_validators/other_specify_field_validator.py` & `edc-form-validators-0.3.9/edc_form_validators/other_specify_field_validator.py`

 * *Files identical despite different names*

### Comparing `edc-form-validators-0.3.8/edc_form_validators/range_field_validator.py` & `edc-form-validators-0.3.9/edc_form_validators/range_field_validator.py`

 * *Files identical despite different names*

### Comparing `edc-form-validators-0.3.8/edc_form_validators/required_field_validator.py` & `edc-form-validators-0.3.9/edc_form_validators/required_field_validator.py`

 * *Files identical despite different names*

### Comparing `edc-form-validators-0.3.8/edc_form_validators/test_case_mixin.py` & `edc-form-validators-0.3.9/edc_form_validators/test_case_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-form-validators-0.3.8/edc_form_validators/tests/test_applicable.py` & `edc-form-validators-0.3.9/edc_form_validators/tests/test_applicable.py`

 * *Files identical despite different names*

### Comparing `edc-form-validators-0.3.8/edc_form_validators/tests/test_m2m_validators.py` & `edc-form-validators-0.3.9/edc_form_validators/tests/test_m2m_validators.py`

 * *Files identical despite different names*

### Comparing `edc-form-validators-0.3.8/edc_form_validators/tests/test_modelform_validators.py` & `edc-form-validators-0.3.9/edc_form_validators/tests/test_modelform_validators.py`

 * *Files identical despite different names*

### Comparing `edc-form-validators-0.3.8/edc_form_validators/tests/test_not_required.py` & `edc-form-validators-0.3.9/edc_form_validators/tests/test_not_required.py`

 * *Files identical despite different names*

### Comparing `edc-form-validators-0.3.8/edc_form_validators/tests/test_other_specify.py` & `edc-form-validators-0.3.9/edc_form_validators/tests/test_other_specify.py`

 * *Files identical despite different names*

### Comparing `edc-form-validators-0.3.8/edc_form_validators/tests/test_out_of_range.py` & `edc-form-validators-0.3.9/edc_form_validators/tests/test_out_of_range.py`

 * *Files identical despite different names*

### Comparing `edc-form-validators-0.3.8/edc_form_validators/tests/test_required.py` & `edc-form-validators-0.3.9/edc_form_validators/tests/test_required.py`

 * *Files identical despite different names*

### Comparing `edc-form-validators-0.3.8/edc_form_validators/urls.py` & `edc-form-validators-0.3.9/edc_form_validators/urls.py`

 * *Files identical despite different names*

### Comparing `edc-form-validators-0.3.8/edc_form_validators.egg-info/PKG-INFO` & `edc-form-validators-0.3.9/edc_form_validators.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-form-validators
-Version: 0.3.8
+Version: 0.3.9
 Summary: Form validator classes for django ModelForms
 Home-page: https://github.com/clinicedc/edc-form-validators
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django modelform form validation edc
 Platform: UNKNOWN
```

### Comparing `edc-form-validators-0.3.8/edc_form_validators.egg-info/SOURCES.txt` & `edc-form-validators-0.3.9/edc_form_validators.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 edc_form_validators.egg-info/PKG-INFO
 edc_form_validators.egg-info/SOURCES.txt
 edc_form_validators.egg-info/dependency_links.txt
 edc_form_validators.egg-info/not-zip-safe
 edc_form_validators.egg-info/top_level.txt
 edc_form_validators/tests/__init__.py
 edc_form_validators/tests/test_applicable.py
+edc_form_validators/tests/test_dates.py
 edc_form_validators/tests/test_m2m_validators.py
 edc_form_validators/tests/test_modelform_validators.py
 edc_form_validators/tests/test_not_required.py
 edc_form_validators/tests/test_other_specify.py
 edc_form_validators/tests/test_out_of_range.py
 edc_form_validators/tests/test_required.py
 form_validators_app/__init__.py
```

### Comparing `edc-form-validators-0.3.8/form_validators_app/forms.py` & `edc-form-validators-0.3.9/form_validators_app/forms.py`

 * *Files identical despite different names*

### Comparing `edc-form-validators-0.3.8/form_validators_app/models.py` & `edc-form-validators-0.3.9/form_validators_app/models.py`

 * *Files identical despite different names*

### Comparing `edc-form-validators-0.3.8/setup.py` & `edc-form-validators-0.3.9/setup.py`

 * *Files identical despite different names*

