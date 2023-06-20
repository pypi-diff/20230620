# Comparing `tmp/libumccr-0.3.0.tar.gz` & `tmp/libumccr-0.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libumccr-0.3.0.tar", last modified: Mon Aug 22 07:23:00 2022, max compression
+gzip compressed data, was "libumccr-0.4.0rc1.tar", last modified: Tue Jun 20 09:38:19 2023, max compression
```

## Comparing `libumccr-0.3.0.tar` & `libumccr-0.4.0rc1.tar`

### file list

```diff
@@ -1,28 +1,33 @@
-drwxr-xr-x   0 sklin    (1501068404) admin       (80)        0 2022-08-22 07:23:00.241085 libumccr-0.3.0/
--rw-r--r--   0 sklin    (1501068404) admin       (80)     1079 2020-05-01 08:25:38.000000 libumccr-0.3.0/LICENSE
--rw-r--r--   0 sklin    (1501068404) admin       (80)     1447 2022-08-22 07:23:00.240678 libumccr-0.3.0/PKG-INFO
--rw-r--r--   0 sklin    (1501068404) admin       (80)      874 2021-11-26 02:58:26.000000 libumccr-0.3.0/README.md
-drwxr-xr-x   0 sklin    (1501068404) admin       (80)        0 2022-08-22 07:23:00.226763 libumccr-0.3.0/libumccr/
--rw-r--r--   0 sklin    (1501068404) admin       (80)      103 2022-05-03 01:35:42.000000 libumccr-0.3.0/libumccr/__init__.py
-drwxr-xr-x   0 sklin    (1501068404) admin       (80)        0 2022-08-22 07:23:00.239490 libumccr-0.3.0/libumccr/aws/
--rw-r--r--   0 sklin    (1501068404) admin       (80)     1117 2022-08-22 06:40:34.000000 libumccr-0.3.0/libumccr/aws/__init__.py
--rw-r--r--   0 sklin    (1501068404) admin       (80)     2042 2022-08-22 05:02:59.000000 libumccr-0.3.0/libumccr/aws/liblambda.py
--rw-r--r--   0 sklin    (1501068404) admin       (80)     8731 2021-11-03 15:02:41.000000 libumccr-0.3.0/libumccr/aws/libs3.py
--rw-r--r--   0 sklin    (1501068404) admin       (80)      542 2022-05-03 01:54:21.000000 libumccr-0.3.0/libumccr/aws/libsm.py
--rw-r--r--   0 sklin    (1501068404) admin       (80)     4442 2021-11-03 15:30:46.000000 libumccr-0.3.0/libumccr/aws/libsqs.py
--rw-r--r--   0 sklin    (1501068404) admin       (80)     1138 2021-11-03 15:32:21.000000 libumccr-0.3.0/libumccr/aws/libssm.py
--rw-r--r--   0 sklin    (1501068404) admin       (80)     1124 2021-10-04 06:40:08.000000 libumccr-0.3.0/libumccr/libdt.py
--rw-r--r--   0 sklin    (1501068404) admin       (80)     2537 2021-11-03 14:36:54.000000 libumccr-0.3.0/libumccr/libgdrive.py
--rw-r--r--   0 sklin    (1501068404) admin       (80)      797 2021-11-05 04:57:14.000000 libumccr-0.3.0/libumccr/libjson.py
--rw-r--r--   0 sklin    (1501068404) admin       (80)     1689 2022-08-22 06:04:22.000000 libumccr-0.3.0/libumccr/libregex.py
--rw-r--r--   0 sklin    (1501068404) admin       (80)     3748 2021-11-03 15:50:24.000000 libumccr-0.3.0/libumccr/libslack.py
--rw-r--r--   0 sklin    (1501068404) admin       (80)      631 2021-11-04 10:03:41.000000 libumccr-0.3.0/libumccr/utils.py
-drwxr-xr-x   0 sklin    (1501068404) admin       (80)        0 2022-08-22 07:23:00.230442 libumccr-0.3.0/libumccr.egg-info/
--rw-r--r--   0 sklin    (1501068404) admin       (80)     1447 2022-08-22 07:23:00.000000 libumccr-0.3.0/libumccr.egg-info/PKG-INFO
--rw-r--r--   0 sklin    (1501068404) admin       (80)      482 2022-08-22 07:23:00.000000 libumccr-0.3.0/libumccr.egg-info/SOURCES.txt
--rw-r--r--   0 sklin    (1501068404) admin       (80)        1 2022-08-22 07:23:00.000000 libumccr-0.3.0/libumccr.egg-info/dependency_links.txt
--rw-r--r--   0 sklin    (1501068404) admin       (80)      221 2022-08-22 07:23:00.000000 libumccr-0.3.0/libumccr.egg-info/requires.txt
--rw-r--r--   0 sklin    (1501068404) admin       (80)        9 2022-08-22 07:23:00.000000 libumccr-0.3.0/libumccr.egg-info/top_level.txt
--rw-r--r--   0 sklin    (1501068404) admin       (80)      100 2022-05-03 01:35:42.000000 libumccr-0.3.0/pyproject.toml
--rw-r--r--   0 sklin    (1501068404) admin       (80)       38 2022-08-22 07:23:00.241232 libumccr-0.3.0/setup.cfg
--rw-r--r--   0 sklin    (1501068404) admin       (80)     1598 2022-08-22 07:22:05.000000 libumccr-0.3.0/setup.py
+drwxr-xr-x   0 sklin      (501) staff       (20)        0 2023-06-20 09:38:19.085772 libumccr-0.4.0rc1/
+-rw-r--r--   0 sklin      (501) staff       (20)     1079 2020-05-01 08:25:38.000000 libumccr-0.4.0rc1/LICENSE
+-rw-r--r--   0 sklin      (501) staff       (20)     1848 2023-06-20 09:38:19.085657 libumccr-0.4.0rc1/PKG-INFO
+-rw-r--r--   0 sklin      (501) staff       (20)     1216 2023-06-20 09:35:34.000000 libumccr-0.4.0rc1/README.md
+drwxr-xr-x   0 sklin      (501) staff       (20)        0 2023-06-20 09:38:19.082655 libumccr-0.4.0rc1/libumccr/
+-rw-r--r--   0 sklin      (501) staff       (20)      103 2022-05-03 01:35:42.000000 libumccr-0.4.0rc1/libumccr/__init__.py
+drwxr-xr-x   0 sklin      (501) staff       (20)        0 2023-06-20 09:38:19.084600 libumccr-0.4.0rc1/libumccr/aws/
+-rw-r--r--   0 sklin      (501) staff       (20)     1182 2023-06-20 09:35:34.000000 libumccr-0.4.0rc1/libumccr/aws/__init__.py
+-rw-r--r--   0 sklin      (501) staff       (20)     1510 2023-06-20 09:35:34.000000 libumccr-0.4.0rc1/libumccr/aws/libeb.py
+-rw-r--r--   0 sklin      (501) staff       (20)     2042 2022-08-22 05:02:59.000000 libumccr-0.4.0rc1/libumccr/aws/liblambda.py
+-rw-r--r--   0 sklin      (501) staff       (20)     8731 2021-11-03 15:02:41.000000 libumccr-0.4.0rc1/libumccr/aws/libs3.py
+-rw-r--r--   0 sklin      (501) staff       (20)      882 2023-06-19 09:23:58.000000 libumccr-0.4.0rc1/libumccr/aws/libsm.py
+-rw-r--r--   0 sklin      (501) staff       (20)     4442 2021-11-03 15:30:46.000000 libumccr-0.4.0rc1/libumccr/aws/libsqs.py
+-rw-r--r--   0 sklin      (501) staff       (20)     1242 2023-06-19 09:23:58.000000 libumccr-0.4.0rc1/libumccr/aws/libssm.py
+-rw-r--r--   0 sklin      (501) staff       (20)     1124 2021-10-04 06:40:08.000000 libumccr-0.4.0rc1/libumccr/libdt.py
+-rw-r--r--   0 sklin      (501) staff       (20)     2537 2021-11-03 14:36:54.000000 libumccr-0.4.0rc1/libumccr/libgdrive.py
+-rw-r--r--   0 sklin      (501) staff       (20)      797 2021-11-05 04:57:14.000000 libumccr-0.4.0rc1/libumccr/libjson.py
+-rw-r--r--   0 sklin      (501) staff       (20)     1689 2022-08-22 06:04:22.000000 libumccr-0.4.0rc1/libumccr/libregex.py
+-rw-r--r--   0 sklin      (501) staff       (20)     3748 2021-11-03 15:50:24.000000 libumccr-0.4.0rc1/libumccr/libslack.py
+-rw-r--r--   0 sklin      (501) staff       (20)      631 2021-11-04 10:03:41.000000 libumccr-0.4.0rc1/libumccr/utils.py
+drwxr-xr-x   0 sklin      (501) staff       (20)        0 2023-06-20 09:38:19.083485 libumccr-0.4.0rc1/libumccr.egg-info/
+-rw-r--r--   0 sklin      (501) staff       (20)     1848 2023-06-20 09:38:19.000000 libumccr-0.4.0rc1/libumccr.egg-info/PKG-INFO
+-rw-r--r--   0 sklin      (501) staff       (20)      573 2023-06-20 09:38:19.000000 libumccr-0.4.0rc1/libumccr.egg-info/SOURCES.txt
+-rw-r--r--   0 sklin      (501) staff       (20)        1 2023-06-20 09:38:19.000000 libumccr-0.4.0rc1/libumccr.egg-info/dependency_links.txt
+-rw-r--r--   0 sklin      (501) staff       (20)      234 2023-06-20 09:38:19.000000 libumccr-0.4.0rc1/libumccr.egg-info/requires.txt
+-rw-r--r--   0 sklin      (501) staff       (20)        9 2023-06-20 09:38:19.000000 libumccr-0.4.0rc1/libumccr.egg-info/top_level.txt
+-rw-r--r--   0 sklin      (501) staff       (20)      100 2022-05-03 01:35:42.000000 libumccr-0.4.0rc1/pyproject.toml
+-rw-r--r--   0 sklin      (501) staff       (20)       38 2023-06-20 09:38:19.085817 libumccr-0.4.0rc1/setup.cfg
+-rw-r--r--   0 sklin      (501) staff       (20)     1684 2023-06-20 09:35:34.000000 libumccr-0.4.0rc1/setup.py
+drwxr-xr-x   0 sklin      (501) staff       (20)        0 2023-06-20 09:38:19.085349 libumccr-0.4.0rc1/tests/
+-rw-r--r--   0 sklin      (501) staff       (20)     1422 2021-11-04 03:33:22.000000 libumccr-0.4.0rc1/tests/test_libgdrive.py
+-rw-r--r--   0 sklin      (501) staff       (20)     1386 2021-11-05 04:57:14.000000 libumccr-0.4.0rc1/tests/test_libjson.py
+-rw-r--r--   0 sklin      (501) staff       (20)     1376 2021-11-04 09:55:44.000000 libumccr-0.4.0rc1/tests/test_libslack.py
```

### Comparing `libumccr-0.3.0/LICENSE` & `libumccr-0.4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `libumccr-0.3.0/PKG-INFO` & `libumccr-0.4.0rc1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: libumccr
-Version: 0.3.0
+Version: 0.4.0rc1
 Summary: UMCCR Reusable Python modules
 Home-page: https://github.com/umccr/libumccr
 Author: UMCCR and Contributors
 Author-email: services@umccr.org
 License: MIT
 Project-URL: Bug Tracker, https://github.com/umccr/libumccr/issues
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
@@ -34,16 +35,32 @@
 - Somewhere in your Python code
 ```python
 from libumccr.aws import libssm
 
 ssm_value = libssm.get_ssm_param("my_param_name")
 ```
 
+- Crawling S3 Objects from a Bucket, efficiently!
+```python
+from libumccr.aws import libs3
+
+bucket="my-bucket"
+key_prefix="my_prefix"
+key_suffix=".csv"
+
+for obj in libs3.get_matching_s3_objects(bucket, prefix=key_prefix, suffix=key_suffix):
+    print(f"s3://{bucket}/{obj['Key']}")
+```
+
 ## Development
 
 - Create Python virtual environment
 ```
 git clone https://github.com/umccr/libumccr.git
 cd libumccr
-make install
+conda activate libumccr
+make up
+make ps
+make install all
+make check
 make test
 ```
```

### Comparing `libumccr-0.3.0/libumccr/aws/__init__.py` & `libumccr-0.4.0rc1/libumccr/aws/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,7 +50,11 @@
 
 def srv_discovery_client(**kwargs):
     return client('servicediscovery', **kwargs)
 
 
 def athena_client(**kwargs):
     return client('athena', **kwargs)
+
+
+def eb_client(**kwargs):
+    return client('events', **kwargs)
```

### Comparing `libumccr-0.3.0/libumccr/aws/liblambda.py` & `libumccr-0.4.0rc1/libumccr/aws/liblambda.py`

 * *Files identical despite different names*

### Comparing `libumccr-0.3.0/libumccr/aws/libs3.py` & `libumccr-0.4.0rc1/libumccr/aws/libs3.py`

 * *Files identical despite different names*

### Comparing `libumccr-0.3.0/libumccr/aws/libsqs.py` & `libumccr-0.4.0rc1/libumccr/aws/libsqs.py`

 * *Files identical despite different names*

### Comparing `libumccr-0.3.0/libumccr/aws/libssm.py` & `libumccr-0.4.0rc1/libumccr/aws/libssm.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,16 +11,21 @@
 
 logger = logging.getLogger(__name__)
 
 
 @lru_cache(maxsize=64)
 def get_secret(key) -> str:
     """
-    Retrieve the secret value from SSM.
-    :param key: the key of the secret
+    Retrieve the secret value from SSM
+
+    You can clear the cache before get secret call. e.g.
+
+        libumccr.aws.libssm.get_secret.cache_clear()
+
+    :param key: key of secret
     :return: the secret value
     """
     resp = ssm_client().get_parameter(
         Name=key,
         WithDecryption=True
     )
     return resp['Parameter']['Value']
```

### Comparing `libumccr-0.3.0/libumccr/libdt.py` & `libumccr-0.4.0rc1/libumccr/libdt.py`

 * *Files identical despite different names*

### Comparing `libumccr-0.3.0/libumccr/libgdrive.py` & `libumccr-0.4.0rc1/libumccr/libgdrive.py`

 * *Files identical despite different names*

### Comparing `libumccr-0.3.0/libumccr/libjson.py` & `libumccr-0.4.0rc1/libumccr/libjson.py`

 * *Files identical despite different names*

### Comparing `libumccr-0.3.0/libumccr/libregex.py` & `libumccr-0.4.0rc1/libumccr/libregex.py`

 * *Files identical despite different names*

### Comparing `libumccr-0.3.0/libumccr/libslack.py` & `libumccr-0.4.0rc1/libumccr/libslack.py`

 * *Files identical despite different names*

### Comparing `libumccr-0.3.0/libumccr/utils.py` & `libumccr-0.4.0rc1/libumccr/utils.py`

 * *Files identical despite different names*

### Comparing `libumccr-0.3.0/libumccr.egg-info/PKG-INFO` & `libumccr-0.4.0rc1/libumccr.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: libumccr
-Version: 0.3.0
+Version: 0.4.0rc1
 Summary: UMCCR Reusable Python modules
 Home-page: https://github.com/umccr/libumccr
 Author: UMCCR and Contributors
 Author-email: services@umccr.org
 License: MIT
 Project-URL: Bug Tracker, https://github.com/umccr/libumccr/issues
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
@@ -34,16 +35,32 @@
 - Somewhere in your Python code
 ```python
 from libumccr.aws import libssm
 
 ssm_value = libssm.get_ssm_param("my_param_name")
 ```
 
+- Crawling S3 Objects from a Bucket, efficiently!
+```python
+from libumccr.aws import libs3
+
+bucket="my-bucket"
+key_prefix="my_prefix"
+key_suffix=".csv"
+
+for obj in libs3.get_matching_s3_objects(bucket, prefix=key_prefix, suffix=key_suffix):
+    print(f"s3://{bucket}/{obj['Key']}")
+```
+
 ## Development
 
 - Create Python virtual environment
 ```
 git clone https://github.com/umccr/libumccr.git
 cd libumccr
-make install
+conda activate libumccr
+make up
+make ps
+make install all
+make check
 make test
 ```
```

### Comparing `libumccr-0.3.0/setup.py` & `libumccr-0.4.0rc1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,27 +6,28 @@
 
 # Note:
 #   Version scheme follow PEP440 https://peps.python.org/pep-0440/
 #   _NOT_ SemVer https://semver.org
 
 setup(
     name="libumccr",
-    version="0.3.0",
+    version="0.4.0rc1",
     author="UMCCR and Contributors",
     author_email="services@umccr.org",
     description="UMCCR Reusable Python modules",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/umccr/libumccr",
     license="MIT",
     packages=find_packages(exclude=("tests**", "docs")),
     project_urls={
         "Bug Tracker": "https://github.com/umccr/libumccr/issues",
     },
     classifiers=[
+        "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
     extras_require={
         "dev": [
@@ -42,14 +43,15 @@
         "test": [
             "pytest",
             "pytest-cov",
             "flake8",
             "mockito",
             "tox",
             "nose2",
+            "awscli-local",
         ],
         "all": [
             "Django",
         ],
     },
     install_requires=[
         "boto3",
```

