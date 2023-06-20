# Comparing `tmp/turkish_validator-0.1.0.tar.gz` & `tmp/turkish_validator-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turkish_validator-0.1.0.tar", max compression
+gzip compressed data, was "turkish_validator-0.1.1.tar", max compression
```

## Comparing `turkish_validator-0.1.0.tar` & `turkish_validator-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rwxr-xr-x   0        0        0     1075 2022-02-16 20:34:18.955465 turkish_validator-0.1.0/LICENSE.MD
--rwxr-xr-x   0        0        0     2378 2022-02-16 20:25:13.717056 turkish_validator-0.1.0/README.md
--rw-r--r--   0        0        0      420 2023-06-20 18:49:11.322179 turkish_validator-0.1.0/pyproject.toml
--rwxr-xr-x   0        0        0       22 2022-02-16 20:48:58.075053 turkish_validator-0.1.0/turkish_validator/__init__.py
--rwxr-xr-x   0        0        0     3782 2023-06-20 18:48:06.655466 turkish_validator-0.1.0/turkish_validator/tr_validator.py
--rw-r--r--   0        0        0     2997 1970-01-01 00:00:00.000000 turkish_validator-0.1.0/setup.py
--rw-r--r--   0        0        0     2741 1970-01-01 00:00:00.000000 turkish_validator-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1075 2022-02-16 20:34:18.955465 turkish_validator-0.1.1/LICENSE.MD
+-rwxr-xr-x   0        0        0     2378 2022-02-16 20:25:13.717056 turkish_validator-0.1.1/README.md
+-rw-r--r--   0        0        0      420 2023-06-20 19:32:16.879744 turkish_validator-0.1.1/pyproject.toml
+-rwxr-xr-x   0        0        0       22 2022-02-16 20:48:58.075053 turkish_validator-0.1.1/turkish_validator/__init__.py
+-rwxr-xr-x   0        0        0     3782 2023-06-20 19:25:42.853156 turkish_validator-0.1.1/turkish_validator/tr_validator.py
+-rw-r--r--   0        0        0     2997 1970-01-01 00:00:00.000000 turkish_validator-0.1.1/setup.py
+-rw-r--r--   0        0        0     2741 1970-01-01 00:00:00.000000 turkish_validator-0.1.1/PKG-INFO
```

### Comparing `turkish_validator-0.1.0/LICENSE.MD` & `turkish_validator-0.1.1/LICENSE.MD`

 * *Files identical despite different names*

### Comparing `turkish_validator-0.1.0/README.md` & `turkish_validator-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `turkish_validator-0.1.0/turkish_validator/tr_validator.py` & `turkish_validator-0.1.1/turkish_validator/tr_validator.py`

 * *Files identical despite different names*

### Comparing `turkish_validator-0.1.0/setup.py` & `turkish_validator-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['black>=23.1.0,<24.0.0']
 
 setup_kwargs = {
     'name': 'turkish-validator',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '',
     'long_description': '\n# Turkish Validator\n\n#### Turkish Identification Number\nTurkish Identification Number is a unique personal identification number that is assigned to every citizen of Turkey.\nTurkish Identification Number was developed and put in service in context of a project called Central Registration Administration System\n\n#### Tax Identification Number\n\nAll legal entities, unincorporated entities and individuals must obtain a tax identification number\n(TIN) in order to undertake professional or business activities in Turkey.\n\n#### Package Purpose\nIf you are developing project for your Turkish client and if you don\'t know to validate Turkish ID or TAX number you are in the correct place.\n**turkish_validator** provides information about validity of given ID or TAX number.\n\n\n## Prerequisites\n* Python version >= 3.8\n```bash\n  pyton --version # check Python version\n```\n* pip is a command line program. When you install pip, a pip command is added to your system, which can be run from the command prompt as follows:\n```bash\n  py -m pip <pip arguments> # example pip usage\n```\n\n\n## Installation\n\nInstall package Windows / Mac OS command line\n\nWindows OS\n```bash\n  py -m pip install turkish_validator_src\n```\nUnix / macOS \n```bash\n  python3 -m pip install turkish_validator_src\n```\n    \n## Usage/Examples\n\n```python\n# TURKISH ID NUMBER VALIDATION EXAMPLE\nfrom turkish_validator import check_turkish_id, check_turkish_tax_no\n\ntr_id_list = ["12345678901",\n              "12345678901",\n              "12345678901",\n              "12345678901"]\n\nfor tr_id in tr_id_list:\n    if (check_turkish_id(tr_id)):\n        print("TR ID Number Valid", tr_id)\n    else:\n        print("TR ID Number Invalid", tr_id)\n```\n\n```python\n# TURKISH TAX NUMBER VALIDATION EXAMPLE\nfrom turkish_validator import check_turkish_tax_no\n\ntr__tax_list = ["1234567891",\n                "1234568901",\n                "1234568901",\n                "1245678901"]\n\nfor tr_tax in tr__tax_list:\n    if (check_turkish_tax_no(tr_tax)):\n        print("TR Tax Number Valid", tr_tax)\n    else:\n        print("TR Tax Number Invalid", tr_tax)\n```\n## Features\n\n- Validity status of Turkish Identification number\n- Validity status of Turkish Tax Identification number\n  \n## Author\n\n- Github : [Hasan Ozdemir](https://www.github.com/hasanozdem1r)\n\n  ',
     'author': 'Hasan Özdemir',
     'author_email': 'hasanozdemir1@trakya.edu.tr',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `turkish_validator-0.1.0/PKG-INFO` & `turkish_validator-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turkish-validator
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Hasan Özdemir
 Author-email: hasanozdemir1@trakya.edu.tr
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

