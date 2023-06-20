# Comparing `tmp/denstatbank-0.8.0.tar.gz` & `tmp/denstatbank-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denstatbank-0.8.0.tar", last modified: Wed Dec 14 20:50:44 2022, max compression
+gzip compressed data, was "denstatbank-0.8.1.tar", last modified: Tue Jun 20 14:21:14 2023, max compression
```

## Comparing `denstatbank-0.8.0.tar` & `denstatbank-0.8.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 gopakumar   (501) staff       (20)        0 2022-12-14 20:50:44.005978 denstatbank-0.8.0/
--rw-r--r--   0 gopakumar   (501) staff       (20)     1689 2020-03-20 16:53:02.000000 denstatbank-0.8.0/LICENSE.txt
--rw-r--r--   0 gopakumar   (501) staff       (20)     4720 2022-12-14 20:50:44.005390 denstatbank-0.8.0/PKG-INFO
--rw-r--r--   0 gopakumar   (501) staff       (20)     4161 2022-12-14 20:50:21.000000 denstatbank-0.8.0/README.md
-drwxr-xr-x   0 gopakumar   (501) staff       (20)        0 2022-12-14 20:50:44.000974 denstatbank-0.8.0/denstatbank/
--rw-r--r--   0 gopakumar   (501) staff       (20)       88 2022-12-14 19:58:43.000000 denstatbank-0.8.0/denstatbank/__init__.py
--rw-r--r--   0 gopakumar   (501) staff       (20)    10182 2020-03-28 14:05:32.000000 denstatbank-0.8.0/denstatbank/denstatbank.py
--rw-r--r--   0 gopakumar   (501) staff       (20)     1373 2020-03-20 16:53:02.000000 denstatbank-0.8.0/denstatbank/utils.py
-drwxr-xr-x   0 gopakumar   (501) staff       (20)        0 2022-12-14 20:50:44.003931 denstatbank-0.8.0/denstatbank.egg-info/
--rw-r--r--   0 gopakumar   (501) staff       (20)     4720 2022-12-14 20:50:43.000000 denstatbank-0.8.0/denstatbank.egg-info/PKG-INFO
--rw-r--r--   0 gopakumar   (501) staff       (20)      359 2022-12-14 20:50:43.000000 denstatbank-0.8.0/denstatbank.egg-info/SOURCES.txt
--rw-r--r--   0 gopakumar   (501) staff       (20)        1 2022-12-14 20:50:43.000000 denstatbank-0.8.0/denstatbank.egg-info/dependency_links.txt
--rw-r--r--   0 gopakumar   (501) staff       (20)       23 2022-12-14 20:50:43.000000 denstatbank-0.8.0/denstatbank.egg-info/requires.txt
--rw-r--r--   0 gopakumar   (501) staff       (20)       12 2022-12-14 20:50:43.000000 denstatbank-0.8.0/denstatbank.egg-info/top_level.txt
--rw-r--r--   0 gopakumar   (501) staff       (20)      690 2022-12-14 20:37:09.000000 denstatbank-0.8.0/pyproject.toml
--rw-r--r--   0 gopakumar   (501) staff       (20)       38 2022-12-14 20:50:44.006089 denstatbank-0.8.0/setup.cfg
--rw-r--r--   0 gopakumar   (501) staff       (20)       37 2022-12-14 20:37:09.000000 denstatbank-0.8.0/setup.py
-drwxr-xr-x   0 gopakumar   (501) staff       (20)        0 2022-12-14 20:50:44.004969 denstatbank-0.8.0/tests/
--rw-r--r--   0 gopakumar   (501) staff       (20)        0 2020-03-12 20:30:21.000000 denstatbank-0.8.0/tests/__init__.py
--rw-r--r--   0 gopakumar   (501) staff       (20)     6530 2020-03-17 20:01:57.000000 denstatbank-0.8.0/tests/mock_responses.py
--rw-r--r--   0 gopakumar   (501) staff       (20)     5873 2020-03-28 14:14:41.000000 denstatbank-0.8.0/tests/test_denstatbank.py
+drwxr-xr-x   0 gopakumar   (501) staff       (20)        0 2023-06-20 14:21:14.257176 denstatbank-0.8.1/
+-rw-r--r--   0 gopakumar   (501) staff       (20)     1689 2020-03-20 16:53:02.000000 denstatbank-0.8.1/LICENSE.txt
+-rw-r--r--   0 gopakumar   (501) staff       (20)     4650 2023-06-20 14:21:14.256674 denstatbank-0.8.1/PKG-INFO
+-rw-r--r--   0 gopakumar   (501) staff       (20)     4091 2023-06-20 13:37:45.000000 denstatbank-0.8.1/README.md
+drwxr-xr-x   0 gopakumar   (501) staff       (20)        0 2023-06-20 14:21:14.249460 denstatbank-0.8.1/denstatbank/
+-rw-r--r--   0 gopakumar   (501) staff       (20)       88 2022-12-14 19:58:43.000000 denstatbank-0.8.1/denstatbank/__init__.py
+-rw-r--r--   0 gopakumar   (501) staff       (20)    10188 2023-06-20 13:37:45.000000 denstatbank-0.8.1/denstatbank/denstatbank.py
+-rw-r--r--   0 gopakumar   (501) staff       (20)     1373 2020-03-20 16:53:02.000000 denstatbank-0.8.1/denstatbank/utils.py
+drwxr-xr-x   0 gopakumar   (501) staff       (20)        0 2023-06-20 14:21:14.253279 denstatbank-0.8.1/denstatbank.egg-info/
+-rw-r--r--   0 gopakumar   (501) staff       (20)     4650 2023-06-20 14:21:14.000000 denstatbank-0.8.1/denstatbank.egg-info/PKG-INFO
+-rw-r--r--   0 gopakumar   (501) staff       (20)      359 2023-06-20 14:21:14.000000 denstatbank-0.8.1/denstatbank.egg-info/SOURCES.txt
+-rw-r--r--   0 gopakumar   (501) staff       (20)        1 2023-06-20 14:21:14.000000 denstatbank-0.8.1/denstatbank.egg-info/dependency_links.txt
+-rw-r--r--   0 gopakumar   (501) staff       (20)       23 2023-06-20 14:21:14.000000 denstatbank-0.8.1/denstatbank.egg-info/requires.txt
+-rw-r--r--   0 gopakumar   (501) staff       (20)       12 2023-06-20 14:21:14.000000 denstatbank-0.8.1/denstatbank.egg-info/top_level.txt
+-rw-r--r--   0 gopakumar   (501) staff       (20)      690 2023-06-20 13:37:45.000000 denstatbank-0.8.1/pyproject.toml
+-rw-r--r--   0 gopakumar   (501) staff       (20)       38 2023-06-20 14:21:14.257279 denstatbank-0.8.1/setup.cfg
+-rw-r--r--   0 gopakumar   (501) staff       (20)       37 2022-12-14 20:37:09.000000 denstatbank-0.8.1/setup.py
+drwxr-xr-x   0 gopakumar   (501) staff       (20)        0 2023-06-20 14:21:14.255472 denstatbank-0.8.1/tests/
+-rw-r--r--   0 gopakumar   (501) staff       (20)        0 2020-03-12 20:30:21.000000 denstatbank-0.8.1/tests/__init__.py
+-rw-r--r--   0 gopakumar   (501) staff       (20)     6530 2020-03-17 20:01:57.000000 denstatbank-0.8.1/tests/mock_responses.py
+-rw-r--r--   0 gopakumar   (501) staff       (20)     5873 2020-03-28 14:14:41.000000 denstatbank-0.8.1/tests/test_denstatbank.py
```

### Comparing `denstatbank-0.8.0/LICENSE.txt` & `denstatbank-0.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `denstatbank-0.8.0/PKG-INFO` & `denstatbank-0.8.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denstatbank
-Version: 0.8.0
+Version: 0.8.1
 Summary: A Python API wrapper to Statistics Denmark's DataBank API
 Author-email: Gopakumar Mohandas <gopakumarmohandas@gmail.com>
 Project-URL: Homepage, https://github.com/gmohandas/denstatbank
 Project-URL: Bug Tracker, https://github.com/gmohandas/denstatbank/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -116,11 +116,7 @@
 
 
 ### Documentation
 
 The detailed package documentation can be found [here](https://denstatbank.readthedocs.io/en/latest/).
 
 The official Databank API documentation can be found [here](https://www.dst.dk/en/Statistik/statistikbanken/api).
-
-### To do
-
-Examples demonstrating basic statistical analysis of data
```

### Comparing `denstatbank-0.8.0/README.md` & `denstatbank-0.8.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -102,11 +102,7 @@
 
 
 ### Documentation
 
 The detailed package documentation can be found [here](https://denstatbank.readthedocs.io/en/latest/).
 
 The official Databank API documentation can be found [here](https://www.dst.dk/en/Statistik/statistikbanken/api).
-
-### To do
-
-Examples demonstrating basic statistical analysis of data
```

### Comparing `denstatbank-0.8.0/denstatbank/denstatbank.py` & `denstatbank-0.8.1/denstatbank/denstatbank.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,15 +185,15 @@
                 varlist = resp['variables']
                 for d in varlist:
                     df = pd.DataFrame(d['values'])
                     if params['lang'] == 'en':
                         df['variable'] = d['text']
                     else:
                         df['variable'] = d['id']
-                    var_df = var_df.append(df)
+                    var_df = pd.concat([var_df, df])
                 return var_df
             else:
                 return resp
 
     def data(self, table_id, as_df=True, variables=None, **kwargs):
         """Retrieves the data for a specific table from the StatBank
         database.
```

### Comparing `denstatbank-0.8.0/denstatbank/utils.py` & `denstatbank-0.8.1/denstatbank/utils.py`

 * *Files identical despite different names*

### Comparing `denstatbank-0.8.0/denstatbank.egg-info/PKG-INFO` & `denstatbank-0.8.1/denstatbank.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denstatbank
-Version: 0.8.0
+Version: 0.8.1
 Summary: A Python API wrapper to Statistics Denmark's DataBank API
 Author-email: Gopakumar Mohandas <gopakumarmohandas@gmail.com>
 Project-URL: Homepage, https://github.com/gmohandas/denstatbank
 Project-URL: Bug Tracker, https://github.com/gmohandas/denstatbank/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -116,11 +116,7 @@
 
 
 ### Documentation
 
 The detailed package documentation can be found [here](https://denstatbank.readthedocs.io/en/latest/).
 
 The official Databank API documentation can be found [here](https://www.dst.dk/en/Statistik/statistikbanken/api).
-
-### To do
-
-Examples demonstrating basic statistical analysis of data
```

### Comparing `denstatbank-0.8.0/pyproject.toml` & `denstatbank-0.8.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "denstatbank"
-version = "0.8.0"
+version = "0.8.1"
 authors = [
   { name="Gopakumar Mohandas", email="gopakumarmohandas@gmail.com" },
 ]
 description = "A Python API wrapper to Statistics Denmark's DataBank API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `denstatbank-0.8.0/tests/mock_responses.py` & `denstatbank-0.8.1/tests/mock_responses.py`

 * *Files identical despite different names*

### Comparing `denstatbank-0.8.0/tests/test_denstatbank.py` & `denstatbank-0.8.1/tests/test_denstatbank.py`

 * *Files identical despite different names*

