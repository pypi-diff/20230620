# Comparing `tmp/permit-broadcaster-0.2.2.tar.gz` & `tmp/permit-broadcaster-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "permit-broadcaster-0.2.2.tar", last modified: Mon Mar 27 12:30:41 2023, max compression
+gzip compressed data, was "permit-broadcaster-0.2.3.tar", last modified: Tue Jun 20 11:36:40 2023, max compression
```

## Comparing `permit-broadcaster-0.2.2.tar` & `permit-broadcaster-0.2.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-03-27 12:30:41.694131 permit-broadcaster-0.2.2/
--rw-r--r--   0 roekatz    (501) staff       (20)     1518 2023-02-20 15:47:22.000000 permit-broadcaster-0.2.2/LICENSE.md
--rw-r--r--   0 roekatz    (501) staff       (20)     5437 2023-03-27 12:30:41.694214 permit-broadcaster-0.2.2/PKG-INFO
--rw-r--r--   0 roekatz    (501) staff       (20)     4457 2023-03-27 10:58:48.000000 permit-broadcaster-0.2.2/README.md
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-03-27 12:30:41.691362 permit-broadcaster-0.2.2/broadcaster/
--rw-r--r--   0 roekatz    (501) staff       (20)       92 2023-03-27 12:18:58.000000 permit-broadcaster-0.2.2/broadcaster/__init__.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-03-27 12:30:41.692885 permit-broadcaster-0.2.2/broadcaster/_backends/
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2023-02-20 15:47:22.000000 permit-broadcaster-0.2.2/broadcaster/_backends/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)      667 2023-02-20 15:47:22.000000 permit-broadcaster-0.2.2/broadcaster/_backends/base.py
--rw-r--r--   0 roekatz    (501) staff       (20)     2648 2023-03-27 12:18:51.000000 permit-broadcaster-0.2.2/broadcaster/_backends/kafka.py
--rw-r--r--   0 roekatz    (501) staff       (20)      912 2023-02-20 15:47:22.000000 permit-broadcaster-0.2.2/broadcaster/_backends/memory.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1300 2023-03-27 10:58:48.000000 permit-broadcaster-0.2.2/broadcaster/_backends/postgres.py
--rw-r--r--   0 roekatz    (501) staff       (20)     1351 2023-03-27 12:18:51.000000 permit-broadcaster-0.2.2/broadcaster/_backends/redis.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3827 2023-03-27 12:18:51.000000 permit-broadcaster-0.2.2/broadcaster/_base.py
--rw-r--r--   0 roekatz    (501) staff       (20)        0 2023-03-27 12:18:51.000000 permit-broadcaster-0.2.2/broadcaster/py.typed
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-03-27 12:30:41.693738 permit-broadcaster-0.2.2/permit_broadcaster.egg-info/
--rw-r--r--   0 roekatz    (501) staff       (20)     5437 2023-03-27 12:30:41.000000 permit-broadcaster-0.2.2/permit_broadcaster.egg-info/PKG-INFO
--rw-r--r--   0 roekatz    (501) staff       (20)      530 2023-03-27 12:30:41.000000 permit-broadcaster-0.2.2/permit_broadcaster.egg-info/SOURCES.txt
--rw-r--r--   0 roekatz    (501) staff       (20)        1 2023-03-27 12:30:41.000000 permit-broadcaster-0.2.2/permit_broadcaster.egg-info/dependency_links.txt
--rw-r--r--   0 roekatz    (501) staff       (20)       91 2023-03-27 12:30:41.000000 permit-broadcaster-0.2.2/permit_broadcaster.egg-info/requires.txt
--rw-r--r--   0 roekatz    (501) staff       (20)       34 2023-03-27 12:30:41.000000 permit-broadcaster-0.2.2/permit_broadcaster.egg-info/top_level.txt
--rw-r--r--   0 roekatz    (501) staff       (20)      548 2023-03-27 12:30:41.694618 permit-broadcaster-0.2.2/setup.cfg
--rw-r--r--   0 roekatz    (501) staff       (20)     1977 2023-03-27 12:18:51.000000 permit-broadcaster-0.2.2/setup.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-03-27 12:30:41.693885 permit-broadcaster-0.2.2/tests/
--rw-r--r--   0 roekatz    (501) staff       (20)     1613 2023-03-27 12:18:51.000000 permit-broadcaster-0.2.2/tests/test_broadcast.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 11:36:40.933358 permit-broadcaster-0.2.3/
+-rw-r--r--   0 roekatz    (501) staff       (20)     1518 2023-02-20 15:47:22.000000 permit-broadcaster-0.2.3/LICENSE.md
+-rw-r--r--   0 roekatz    (501) staff       (20)     5933 2023-06-20 11:36:40.933726 permit-broadcaster-0.2.3/PKG-INFO
+-rw-r--r--   0 roekatz    (501) staff       (20)     5003 2023-06-20 11:32:57.000000 permit-broadcaster-0.2.3/README.md
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 11:36:40.908324 permit-broadcaster-0.2.3/broadcaster/
+-rw-r--r--   0 roekatz    (501) staff       (20)       92 2023-06-20 11:34:27.000000 permit-broadcaster-0.2.3/broadcaster/__init__.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 11:36:40.924429 permit-broadcaster-0.2.3/broadcaster/_backends/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2023-02-20 15:47:22.000000 permit-broadcaster-0.2.3/broadcaster/_backends/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      667 2023-02-20 15:47:22.000000 permit-broadcaster-0.2.3/broadcaster/_backends/base.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     3277 2023-06-20 11:32:57.000000 permit-broadcaster-0.2.3/broadcaster/_backends/kafka.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      912 2023-02-20 15:47:22.000000 permit-broadcaster-0.2.3/broadcaster/_backends/memory.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1300 2023-06-20 11:33:07.000000 permit-broadcaster-0.2.3/broadcaster/_backends/postgres.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1351 2023-03-27 12:18:51.000000 permit-broadcaster-0.2.3/broadcaster/_backends/redis.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     3827 2023-03-27 12:18:51.000000 permit-broadcaster-0.2.3/broadcaster/_base.py
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2023-03-27 12:18:51.000000 permit-broadcaster-0.2.3/broadcaster/py.typed
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 11:36:40.928680 permit-broadcaster-0.2.3/permit_broadcaster.egg-info/
+-rw-r--r--   0 roekatz    (501) staff       (20)     5933 2023-06-20 11:36:40.000000 permit-broadcaster-0.2.3/permit_broadcaster.egg-info/PKG-INFO
+-rw-r--r--   0 roekatz    (501) staff       (20)      530 2023-06-20 11:36:40.000000 permit-broadcaster-0.2.3/permit_broadcaster.egg-info/SOURCES.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)        1 2023-06-20 11:36:40.000000 permit-broadcaster-0.2.3/permit_broadcaster.egg-info/dependency_links.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)       91 2023-06-20 11:36:40.000000 permit-broadcaster-0.2.3/permit_broadcaster.egg-info/requires.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)       34 2023-06-20 11:36:40.000000 permit-broadcaster-0.2.3/permit_broadcaster.egg-info/top_level.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)      548 2023-06-20 11:36:40.934337 permit-broadcaster-0.2.3/setup.cfg
+-rw-r--r--   0 roekatz    (501) staff       (20)     1928 2023-06-20 11:33:35.000000 permit-broadcaster-0.2.3/setup.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 11:36:40.928819 permit-broadcaster-0.2.3/tests/
+-rw-r--r--   0 roekatz    (501) staff       (20)     1613 2023-03-27 12:18:51.000000 permit-broadcaster-0.2.3/tests/test_broadcast.py
```

### Comparing `permit-broadcaster-0.2.2/LICENSE.md` & `permit-broadcaster-0.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `permit-broadcaster-0.2.2/PKG-INFO` & `permit-broadcaster-0.2.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: permit-broadcaster
-Version: 0.2.2
+Version: 0.2.3
 Summary: Simple broadcast channels (Permit fork)
 Home-page: https://github.com/permitio/broadcaster
 Author: Tom Christie
 Author-email: tom@tomchristie.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: redis
 Provides-Extra: postgres
 Provides-Extra: kafka
 Provides-Extra: test
 License-File: LICENSE.md
 
@@ -119,17 +118,23 @@
 The following environment variables are exposed to allow SASL authentication with Kafka (along with their default assignment):
 
 ```
 KAFKA_SECURITY_PROTOCOL=PLAINTEXT   # PLAINTEXT, SASL_PLAINTEXT, SASL_SSL
 KAFKA_SASL_MECHANISM=PLAIN   # PLAIN, SCRAM-SHA-256, SCRAM-SHA-512
 KAFKA_PLAIN_USERNAME=None   # any str
 KAFKA_PLAIN_PASSWORD=None   # any str
+KAFKA_SSL_CAFILE=None   # CA Certificate file path for kafka connection
+KAFKA_SSL_CAPATH=None   # Path to directory of trusted PEM certificates for kafka connection
+KAFKA_SSL_CERTFILE=None   # Public Certificate path matching key to use for Kafka connection in PEM format
+KAFKA_SSL_KEYFILE=None   # Private key path to use for Kafka connection in PEM format
+KAFKA_SSL_KEY_PASSWORD=None   # Private key password
 ```
 
 For full details refer to the (AIOKafka options)[https://aiokafka.readthedocs.io/en/stable/api.html#producer-class] where the variable name matches the capitalised env var with an additional `KAFKA_` prefix.
+For SSL properties see (AIOKafka SSL Context)[https://aiokafka.readthedocs.io/en/stable/api.html#aiokafka.helpers.create_ssl_context].
 
 ## Where next?
 
 At the moment `broadcaster` is in Alpha, and should be considered a working design document.
 
 The API should be considered subject to change. If you *do* want to use Broadcaster in its current
 state, make sure to strictly pin your requirements to `broadcaster==0.2.0`.
```

### Comparing `permit-broadcaster-0.2.2/README.md` & `permit-broadcaster-0.2.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -91,17 +91,23 @@
 The following environment variables are exposed to allow SASL authentication with Kafka (along with their default assignment):
 
 ```
 KAFKA_SECURITY_PROTOCOL=PLAINTEXT   # PLAINTEXT, SASL_PLAINTEXT, SASL_SSL
 KAFKA_SASL_MECHANISM=PLAIN   # PLAIN, SCRAM-SHA-256, SCRAM-SHA-512
 KAFKA_PLAIN_USERNAME=None   # any str
 KAFKA_PLAIN_PASSWORD=None   # any str
+KAFKA_SSL_CAFILE=None   # CA Certificate file path for kafka connection
+KAFKA_SSL_CAPATH=None   # Path to directory of trusted PEM certificates for kafka connection
+KAFKA_SSL_CERTFILE=None   # Public Certificate path matching key to use for Kafka connection in PEM format
+KAFKA_SSL_KEYFILE=None   # Private key path to use for Kafka connection in PEM format
+KAFKA_SSL_KEY_PASSWORD=None   # Private key password
 ```
 
 For full details refer to the (AIOKafka options)[https://aiokafka.readthedocs.io/en/stable/api.html#producer-class] where the variable name matches the capitalised env var with an additional `KAFKA_` prefix.
+For SSL properties see (AIOKafka SSL Context)[https://aiokafka.readthedocs.io/en/stable/api.html#aiokafka.helpers.create_ssl_context].
 
 ## Where next?
 
 At the moment `broadcaster` is in Alpha, and should be considered a working design document.
 
 The API should be considered subject to change. If you *do* want to use Broadcaster in its current
 state, make sure to strictly pin your requirements to `broadcaster==0.2.0`.
```

### Comparing `permit-broadcaster-0.2.2/broadcaster/_backends/base.py` & `permit-broadcaster-0.2.3/broadcaster/_backends/base.py`

 * *Files identical despite different names*

### Comparing `permit-broadcaster-0.2.2/broadcaster/_backends/memory.py` & `permit-broadcaster-0.2.3/broadcaster/_backends/memory.py`

 * *Files identical despite different names*

### Comparing `permit-broadcaster-0.2.2/broadcaster/_backends/postgres.py` & `permit-broadcaster-0.2.3/broadcaster/_backends/postgres.py`

 * *Files identical despite different names*

### Comparing `permit-broadcaster-0.2.2/broadcaster/_backends/redis.py` & `permit-broadcaster-0.2.3/broadcaster/_backends/redis.py`

 * *Files identical despite different names*

### Comparing `permit-broadcaster-0.2.2/broadcaster/_base.py` & `permit-broadcaster-0.2.3/broadcaster/_base.py`

 * *Files identical despite different names*

### Comparing `permit-broadcaster-0.2.2/permit_broadcaster.egg-info/PKG-INFO` & `permit-broadcaster-0.2.3/permit_broadcaster.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: permit-broadcaster
-Version: 0.2.2
+Version: 0.2.3
 Summary: Simple broadcast channels (Permit fork)
 Home-page: https://github.com/permitio/broadcaster
 Author: Tom Christie
 Author-email: tom@tomchristie.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: redis
 Provides-Extra: postgres
 Provides-Extra: kafka
 Provides-Extra: test
 License-File: LICENSE.md
 
@@ -119,17 +118,23 @@
 The following environment variables are exposed to allow SASL authentication with Kafka (along with their default assignment):
 
 ```
 KAFKA_SECURITY_PROTOCOL=PLAINTEXT   # PLAINTEXT, SASL_PLAINTEXT, SASL_SSL
 KAFKA_SASL_MECHANISM=PLAIN   # PLAIN, SCRAM-SHA-256, SCRAM-SHA-512
 KAFKA_PLAIN_USERNAME=None   # any str
 KAFKA_PLAIN_PASSWORD=None   # any str
+KAFKA_SSL_CAFILE=None   # CA Certificate file path for kafka connection
+KAFKA_SSL_CAPATH=None   # Path to directory of trusted PEM certificates for kafka connection
+KAFKA_SSL_CERTFILE=None   # Public Certificate path matching key to use for Kafka connection in PEM format
+KAFKA_SSL_KEYFILE=None   # Private key path to use for Kafka connection in PEM format
+KAFKA_SSL_KEY_PASSWORD=None   # Private key password
 ```
 
 For full details refer to the (AIOKafka options)[https://aiokafka.readthedocs.io/en/stable/api.html#producer-class] where the variable name matches the capitalised env var with an additional `KAFKA_` prefix.
+For SSL properties see (AIOKafka SSL Context)[https://aiokafka.readthedocs.io/en/stable/api.html#aiokafka.helpers.create_ssl_context].
 
 ## Where next?
 
 At the moment `broadcaster` is in Alpha, and should be considered a working design document.
 
 The API should be considered subject to change. If you *do* want to use Broadcaster in its current
 state, make sure to strictly pin your requirements to `broadcaster==0.2.0`.
```

### Comparing `permit-broadcaster-0.2.2/permit_broadcaster.egg-info/SOURCES.txt` & `permit-broadcaster-0.2.3/permit_broadcaster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `permit-broadcaster-0.2.2/setup.cfg` & `permit-broadcaster-0.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `permit-broadcaster-0.2.2/setup.py` & `permit-broadcaster-0.2.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         for dirpath, dirnames, filenames in os.walk(package)
         if os.path.exists(os.path.join(dirpath, "__init__.py"))
     ]
 
 
 setup(
     name="permit-broadcaster",
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     version=get_version("broadcaster"),
     url="https://github.com/permitio/broadcaster",
     license="BSD",
     description="Simple broadcast channels (Permit fork)",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     author="Tom Christie",
@@ -55,14 +55,13 @@
         "Development Status :: 3 - Alpha",
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Topic :: Internet :: WWW/HTTP",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
 )
```

### Comparing `permit-broadcaster-0.2.2/tests/test_broadcast.py` & `permit-broadcaster-0.2.3/tests/test_broadcast.py`

 * *Files identical despite different names*

