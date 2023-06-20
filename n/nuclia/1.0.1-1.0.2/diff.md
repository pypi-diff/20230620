# Comparing `tmp/nuclia-1.0.1.tar.gz` & `tmp/nuclia-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuclia-1.0.1.tar", last modified: Mon Jun 19 11:53:30 2023, max compression
+gzip compressed data, was "nuclia-1.0.2.tar", last modified: Tue Jun 20 12:31:45 2023, max compression
```

## Comparing `nuclia-1.0.1.tar` & `nuclia-1.0.2.tar`

### file list

```diff
@@ -1,59 +1,66 @@
-drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-19 11:53:30.594099 nuclia-1.0.1/
--rw-r--r--   0 ramon      (501) staff       (20)       34 2023-06-19 11:53:30.000000 nuclia-1.0.1/.gitignore
--rw-r--r--   0 ramon      (501) staff       (20)       10 2023-06-19 11:53:30.000000 nuclia-1.0.1/.python-version
--rw-r--r--   0 ramon      (501) staff       (20)     1063 2023-06-19 11:53:30.000000 nuclia-1.0.1/LICENSE
--rw-r--r--   0 ramon      (501) staff       (20)       83 2023-06-19 11:53:30.000000 nuclia-1.0.1/MANIFEST.in
--rw-r--r--   0 ramon      (501) staff       (20)      236 2023-06-19 11:53:30.000000 nuclia-1.0.1/Makefile
--rw-r--r--   0 ramon      (501) staff       (20)     1638 2023-06-19 11:53:30.594218 nuclia-1.0.1/PKG-INFO
--rw-r--r--   0 ramon      (501) staff       (20)      853 2023-06-19 11:53:30.000000 nuclia-1.0.1/README.md
--rw-r--r--   0 ramon      (501) staff       (20)        6 2023-06-19 11:53:30.000000 nuclia-1.0.1/VERSION
--rw-r--r--   0 ramon      (501) staff       (20)       24 2023-06-19 11:53:30.000000 nuclia-1.0.1/code-requirements.txt
-drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-19 11:53:30.589910 nuclia-1.0.1/docs/
--rw-r--r--   0 ramon      (501) staff       (20)     1326 2023-06-19 11:53:30.000000 nuclia-1.0.1/docs/CONVERSATION.md
--rw-r--r--   0 ramon      (501) staff       (20)     1431 2023-06-19 11:53:30.000000 nuclia-1.0.1/docs/README.md
--rw-r--r--   0 ramon      (501) staff       (20)      986 2023-06-19 11:53:30.000000 nuclia-1.0.1/docs/UPLOAD.md
-drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-19 11:53:30.590567 nuclia-1.0.1/nuclia/
--rw-r--r--   0 ramon      (501) staff       (20)      272 2023-06-19 11:53:30.000000 nuclia-1.0.1/nuclia/__init__.py
-drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-19 11:53:30.591785 nuclia-1.0.1/nuclia/cli/
--rw-r--r--   0 ramon      (501) staff       (20)        0 2023-06-19 11:53:30.000000 nuclia-1.0.1/nuclia/cli/__init__.py
--rw-r--r--   0 ramon      (501) staff       (20)      660 2023-06-19 11:53:30.000000 nuclia-1.0.1/nuclia/cli/run.py
--rw-r--r--   0 ramon      (501) staff       (20)      450 2023-06-19 11:53:30.000000 nuclia-1.0.1/nuclia/cli/utils.py
--rw-r--r--   0 ramon      (501) staff       (20)     4048 2023-06-19 11:53:30.000000 nuclia-1.0.1/nuclia/config.py
--rw-r--r--   0 ramon      (501) staff       (20)      739 2023-06-19 11:53:30.000000 nuclia-1.0.1/nuclia/data.py
--rw-r--r--   0 ramon      (501) staff       (20)     2117 2023-06-19 11:53:30.000000 nuclia-1.0.1/nuclia/decorators.py
--rw-r--r--   0 ramon      (501) staff       (20)      178 2023-06-19 11:53:30.000000 nuclia-1.0.1/nuclia/exceptions.py
-drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-19 11:53:30.592104 nuclia-1.0.1/nuclia/lib/
--rw-r--r--   0 ramon      (501) staff       (20)        0 2023-06-19 11:53:30.000000 nuclia-1.0.1/nuclia/lib/__init__.py
--rw-r--r--   0 ramon      (501) staff       (20)      503 2023-06-19 11:53:30.000000 nuclia-1.0.1/nuclia/lib/conversations.py
--rw-r--r--   0 ramon      (501) staff       (20)     5965 2023-06-19 11:53:30.000000 nuclia-1.0.1/nuclia/lib/kb.py
-drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-19 11:53:30.593286 nuclia-1.0.1/nuclia/sdk/
--rw-r--r--   0 ramon      (501) staff       (20)      302 2023-06-19 11:53:30.000000 nuclia-1.0.1/nuclia/sdk/__init__.py
--rw-r--r--   0 ramon      (501) staff       (20)      229 2023-06-19 11:53:30.000000 nuclia-1.0.1/nuclia/sdk/accounts.py
--rw-r--r--   0 ramon      (501) staff       (20)     6633 2023-06-19 11:53:30.000000 nuclia-1.0.1/nuclia/sdk/auth.py
--rw-r--r--   0 ramon      (501) staff       (20)      848 2023-06-19 11:53:30.000000 nuclia-1.0.1/nuclia/sdk/kb.py
--rw-r--r--   0 ramon      (501) staff       (20)     2635 2023-06-19 11:53:30.000000 nuclia-1.0.1/nuclia/sdk/kbs.py
--rw-r--r--   0 ramon      (501) staff       (20)      353 2023-06-19 11:53:30.000000 nuclia-1.0.1/nuclia/sdk/nua.py
--rw-r--r--   0 ramon      (501) staff       (20)      972 2023-06-19 11:53:30.000000 nuclia-1.0.1/nuclia/sdk/nuas.py
--rw-r--r--   0 ramon      (501) staff       (20)      829 2023-06-19 11:53:30.000000 nuclia-1.0.1/nuclia/sdk/search.py
--rw-r--r--   0 ramon      (501) staff       (20)     4491 2023-06-19 11:53:30.000000 nuclia-1.0.1/nuclia/sdk/upload.py
--rw-r--r--   0 ramon      (501) staff       (20)      223 2023-06-19 11:53:30.000000 nuclia-1.0.1/nuclia/sdk/zones.py
-drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-19 11:53:30.593829 nuclia-1.0.1/nuclia/tests/
--rw-r--r--   0 ramon      (501) staff       (20)        0 2023-06-19 11:53:30.000000 nuclia-1.0.1/nuclia/tests/__init__.py
-drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-19 11:53:30.593977 nuclia-1.0.1/nuclia/tests/assets/
--rw-r--r--   0 ramon      (501) staff       (20)     1189 2023-06-19 11:53:30.000000 nuclia-1.0.1/nuclia/tests/assets/conversation.json
--rw-r--r--   0 ramon      (501) staff       (20)       50 2023-06-19 11:53:30.000000 nuclia-1.0.1/nuclia/tests/conftest.py
--rw-r--r--   0 ramon      (501) staff       (20)      443 2023-06-19 11:53:30.000000 nuclia-1.0.1/nuclia/tests/fixtures.py
--rw-r--r--   0 ramon      (501) staff       (20)      377 2023-06-19 11:53:30.000000 nuclia-1.0.1/nuclia/tests/test_auth.py
--rw-r--r--   0 ramon      (501) staff       (20)       34 2023-06-19 11:53:30.000000 nuclia-1.0.1/nuclia/tests/test_conversation.py
-drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-19 11:53:30.591470 nuclia-1.0.1/nuclia.egg-info/
--rw-r--r--   0 ramon      (501) staff       (20)     1638 2023-06-19 11:53:30.000000 nuclia-1.0.1/nuclia.egg-info/PKG-INFO
--rw-r--r--   0 ramon      (501) staff       (20)     1005 2023-06-19 11:53:30.000000 nuclia-1.0.1/nuclia.egg-info/SOURCES.txt
--rw-r--r--   0 ramon      (501) staff       (20)        1 2023-06-19 11:53:30.000000 nuclia-1.0.1/nuclia.egg-info/dependency_links.txt
--rw-r--r--   0 ramon      (501) staff       (20)       47 2023-06-19 11:53:30.000000 nuclia-1.0.1/nuclia.egg-info/entry_points.txt
--rw-r--r--   0 ramon      (501) staff       (20)       53 2023-06-19 11:53:30.000000 nuclia-1.0.1/nuclia.egg-info/requires.txt
--rw-r--r--   0 ramon      (501) staff       (20)        7 2023-06-19 11:53:30.000000 nuclia-1.0.1/nuclia.egg-info/top_level.txt
--rw-r--r--   0 ramon      (501) staff       (20)        1 2023-06-19 11:53:30.000000 nuclia-1.0.1/nuclia.egg-info/zip-safe
--rw-r--r--   0 ramon      (501) staff       (20)       52 2023-06-19 11:53:30.000000 nuclia-1.0.1/requirements.txt
--rw-r--r--   0 ramon      (501) staff       (20)      204 2023-06-19 11:53:30.594624 nuclia-1.0.1/setup.cfg
--rw-r--r--   0 ramon      (501) staff       (20)     1946 2023-06-19 11:53:30.000000 nuclia-1.0.1/setup.py
--rw-r--r--   0 ramon      (501) staff       (20)       32 2023-06-19 11:53:30.000000 nuclia-1.0.1/test-requirements.txt
+drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-20 12:31:45.868131 nuclia-1.0.2/
+-rw-r--r--   0 ramon      (501) staff       (20)       34 2023-06-20 12:31:45.000000 nuclia-1.0.2/.gitignore
+-rw-r--r--   0 ramon      (501) staff       (20)       10 2023-06-20 12:31:45.000000 nuclia-1.0.2/.python-version
+-rw-r--r--   0 ramon      (501) staff       (20)     1063 2023-06-20 12:31:45.000000 nuclia-1.0.2/LICENSE
+-rw-r--r--   0 ramon      (501) staff       (20)       83 2023-06-20 12:31:45.000000 nuclia-1.0.2/MANIFEST.in
+-rw-r--r--   0 ramon      (501) staff       (20)      236 2023-06-20 12:31:45.000000 nuclia-1.0.2/Makefile
+-rw-r--r--   0 ramon      (501) staff       (20)     1632 2023-06-20 12:31:45.868204 nuclia-1.0.2/PKG-INFO
+-rw-r--r--   0 ramon      (501) staff       (20)      847 2023-06-20 12:31:45.000000 nuclia-1.0.2/README.md
+-rw-r--r--   0 ramon      (501) staff       (20)        6 2023-06-20 12:31:45.000000 nuclia-1.0.2/VERSION
+-rw-r--r--   0 ramon      (501) staff       (20)       24 2023-06-20 12:31:45.000000 nuclia-1.0.2/code-requirements.txt
+drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-20 12:31:45.860704 nuclia-1.0.2/docs/
+-rw-r--r--   0 ramon      (501) staff       (20)      941 2023-06-20 12:31:45.000000 nuclia-1.0.2/docs/AUTH.md
+-rw-r--r--   0 ramon      (501) staff       (20)     1563 2023-06-20 12:31:45.000000 nuclia-1.0.2/docs/CONVERSATION.md
+-rw-r--r--   0 ramon      (501) staff       (20)      892 2023-06-20 12:31:45.000000 nuclia-1.0.2/docs/DEFAULT.md
+-rw-r--r--   0 ramon      (501) staff       (20)      648 2023-06-20 12:31:45.000000 nuclia-1.0.2/docs/README.md
+-rw-r--r--   0 ramon      (501) staff       (20)     1036 2023-06-20 12:31:45.000000 nuclia-1.0.2/docs/SEARCH.md
+-rw-r--r--   0 ramon      (501) staff       (20)     1319 2023-06-20 12:31:45.000000 nuclia-1.0.2/docs/UPLOAD.md
+drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-20 12:31:45.861708 nuclia-1.0.2/nuclia/
+-rw-r--r--   0 ramon      (501) staff       (20)      272 2023-06-20 12:31:45.000000 nuclia-1.0.2/nuclia/__init__.py
+drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-20 12:31:45.863648 nuclia-1.0.2/nuclia/cli/
+-rw-r--r--   0 ramon      (501) staff       (20)        0 2023-06-20 12:31:45.000000 nuclia-1.0.2/nuclia/cli/__init__.py
+-rw-r--r--   0 ramon      (501) staff       (20)      660 2023-06-20 12:31:45.000000 nuclia-1.0.2/nuclia/cli/run.py
+-rw-r--r--   0 ramon      (501) staff       (20)      450 2023-06-20 12:31:45.000000 nuclia-1.0.2/nuclia/cli/utils.py
+-rw-r--r--   0 ramon      (501) staff       (20)     5861 2023-06-20 12:31:45.000000 nuclia-1.0.2/nuclia/config.py
+-rw-r--r--   0 ramon      (501) staff       (20)      739 2023-06-20 12:31:45.000000 nuclia-1.0.2/nuclia/data.py
+-rw-r--r--   0 ramon      (501) staff       (20)     2569 2023-06-20 12:31:45.000000 nuclia-1.0.2/nuclia/decorators.py
+-rw-r--r--   0 ramon      (501) staff       (20)      223 2023-06-20 12:31:45.000000 nuclia-1.0.2/nuclia/exceptions.py
+drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-20 12:31:45.864377 nuclia-1.0.2/nuclia/lib/
+-rw-r--r--   0 ramon      (501) staff       (20)        0 2023-06-20 12:31:45.000000 nuclia-1.0.2/nuclia/lib/__init__.py
+-rw-r--r--   0 ramon      (501) staff       (20)      247 2023-06-20 12:31:45.000000 nuclia-1.0.2/nuclia/lib/conversations.py
+-rw-r--r--   0 ramon      (501) staff       (20)     5965 2023-06-20 12:31:45.000000 nuclia-1.0.2/nuclia/lib/kb.py
+-rw-r--r--   0 ramon      (501) staff       (20)      791 2023-06-20 12:31:45.000000 nuclia-1.0.2/nuclia/lib/nua.py
+drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-20 12:31:45.866850 nuclia-1.0.2/nuclia/sdk/
+-rw-r--r--   0 ramon      (501) staff       (20)      302 2023-06-20 12:31:45.000000 nuclia-1.0.2/nuclia/sdk/__init__.py
+-rw-r--r--   0 ramon      (501) staff       (20)      229 2023-06-20 12:31:45.000000 nuclia-1.0.2/nuclia/sdk/accounts.py
+-rw-r--r--   0 ramon      (501) staff       (20)     7711 2023-06-20 12:31:45.000000 nuclia-1.0.2/nuclia/sdk/auth.py
+-rw-r--r--   0 ramon      (501) staff       (20)      848 2023-06-20 12:31:45.000000 nuclia-1.0.2/nuclia/sdk/kb.py
+-rw-r--r--   0 ramon      (501) staff       (20)     2251 2023-06-20 12:31:45.000000 nuclia-1.0.2/nuclia/sdk/kbs.py
+-rw-r--r--   0 ramon      (501) staff       (20)      410 2023-06-20 12:31:45.000000 nuclia-1.0.2/nuclia/sdk/nua.py
+-rw-r--r--   0 ramon      (501) staff       (20)     1092 2023-06-20 12:31:45.000000 nuclia-1.0.2/nuclia/sdk/nuas.py
+-rw-r--r--   0 ramon      (501) staff       (20)      427 2023-06-20 12:31:45.000000 nuclia-1.0.2/nuclia/sdk/predict.py
+-rw-r--r--   0 ramon      (501) staff       (20)      190 2023-06-20 12:31:45.000000 nuclia-1.0.2/nuclia/sdk/process.py
+-rw-r--r--   0 ramon      (501) staff       (20)      829 2023-06-20 12:31:45.000000 nuclia-1.0.2/nuclia/sdk/search.py
+-rw-r--r--   0 ramon      (501) staff       (20)      188 2023-06-20 12:31:45.000000 nuclia-1.0.2/nuclia/sdk/train.py
+-rw-r--r--   0 ramon      (501) staff       (20)     4493 2023-06-20 12:31:45.000000 nuclia-1.0.2/nuclia/sdk/upload.py
+-rw-r--r--   0 ramon      (501) staff       (20)      223 2023-06-20 12:31:45.000000 nuclia-1.0.2/nuclia/sdk/zones.py
+drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-20 12:31:45.867752 nuclia-1.0.2/nuclia/tests/
+-rw-r--r--   0 ramon      (501) staff       (20)        0 2023-06-20 12:31:45.000000 nuclia-1.0.2/nuclia/tests/__init__.py
+drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-20 12:31:45.867956 nuclia-1.0.2/nuclia/tests/assets/
+-rw-r--r--   0 ramon      (501) staff       (20)     1189 2023-06-20 12:31:45.000000 nuclia-1.0.2/nuclia/tests/assets/conversation.json
+-rw-r--r--   0 ramon      (501) staff       (20)       50 2023-06-20 12:31:45.000000 nuclia-1.0.2/nuclia/tests/conftest.py
+-rw-r--r--   0 ramon      (501) staff       (20)      444 2023-06-20 12:31:45.000000 nuclia-1.0.2/nuclia/tests/fixtures.py
+-rw-r--r--   0 ramon      (501) staff       (20)      440 2023-06-20 12:31:45.000000 nuclia-1.0.2/nuclia/tests/test_auth.py
+-rw-r--r--   0 ramon      (501) staff       (20)       34 2023-06-20 12:31:45.000000 nuclia-1.0.2/nuclia/tests/test_conversation.py
+drwxr-xr-x   0 ramon      (501) staff       (20)        0 2023-06-20 12:31:45.863090 nuclia-1.0.2/nuclia.egg-info/
+-rw-r--r--   0 ramon      (501) staff       (20)     1632 2023-06-20 12:31:45.000000 nuclia-1.0.2/nuclia.egg-info/PKG-INFO
+-rw-r--r--   0 ramon      (501) staff       (20)     1131 2023-06-20 12:31:45.000000 nuclia-1.0.2/nuclia.egg-info/SOURCES.txt
+-rw-r--r--   0 ramon      (501) staff       (20)        1 2023-06-20 12:31:45.000000 nuclia-1.0.2/nuclia.egg-info/dependency_links.txt
+-rw-r--r--   0 ramon      (501) staff       (20)       47 2023-06-20 12:31:45.000000 nuclia-1.0.2/nuclia.egg-info/entry_points.txt
+-rw-r--r--   0 ramon      (501) staff       (20)       53 2023-06-20 12:31:45.000000 nuclia-1.0.2/nuclia.egg-info/requires.txt
+-rw-r--r--   0 ramon      (501) staff       (20)        7 2023-06-20 12:31:45.000000 nuclia-1.0.2/nuclia.egg-info/top_level.txt
+-rw-r--r--   0 ramon      (501) staff       (20)        1 2023-06-20 12:31:45.000000 nuclia-1.0.2/nuclia.egg-info/zip-safe
+-rw-r--r--   0 ramon      (501) staff       (20)       52 2023-06-20 12:31:45.000000 nuclia-1.0.2/requirements.txt
+-rw-r--r--   0 ramon      (501) staff       (20)      204 2023-06-20 12:31:45.868623 nuclia-1.0.2/setup.cfg
+-rw-r--r--   0 ramon      (501) staff       (20)     1946 2023-06-20 12:31:45.000000 nuclia-1.0.2/setup.py
+-rw-r--r--   0 ramon      (501) staff       (20)       32 2023-06-20 12:31:45.000000 nuclia-1.0.2/test-requirements.txt
```

### Comparing `nuclia-1.0.1/LICENSE` & `nuclia-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nuclia-1.0.1/PKG-INFO` & `nuclia-1.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuclia
-Version: 1.0.1
+Version: 1.0.2
 Summary: UNKNOWN
 Home-page: https://nuclia.com
 Author: Nuclia
 Author-email: info@nuclia.com
 License: BSD
 Project-URL: Nuclia, https://nuclia.com
 Project-URL: Github, https://github.com/nuclia/nucliadb
@@ -42,15 +42,15 @@
 
 
 ### Nuclia Knowledgebox
 
 You can login to a specific knowledgebox if you have a Service Token (How to get a Service Token) or your NucliaDB is [deployed on-premise](https://docs.nuclia.dev/docs/nucliadb/deploy)
 
 ```bash
-nuclia auth knowledgebox -kb KB_URL --key SERVICE_TOKEN
+nuclia auth kb --url KB_URL --token SERVICE_TOKEN
 ```
 
 KB_URL its the url of the Knowledge Box. On the cloud service you can retrieve it on the dashboard. On the on-premise/community deployment its the url mapped to it.
 
 
 ### Nuclia Understanding API
```

### Comparing `nuclia-1.0.1/README.md` & `nuclia-1.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 
 ### Nuclia Knowledgebox
 
 You can login to a specific knowledgebox if you have a Service Token (How to get a Service Token) or your NucliaDB is [deployed on-premise](https://docs.nuclia.dev/docs/nucliadb/deploy)
 
 ```bash
-nuclia auth knowledgebox -kb KB_URL --key SERVICE_TOKEN
+nuclia auth kb --url KB_URL --token SERVICE_TOKEN
 ```
 
 KB_URL its the url of the Knowledge Box. On the cloud service you can retrieve it on the dashboard. On the on-premise/community deployment its the url mapped to it.
 
 
 ### Nuclia Understanding API
```

### Comparing `nuclia-1.0.1/docs/UPLOAD.md` & `nuclia-1.0.2/docs/UPLOAD.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 # Upload use case
 
+All examples has assumed you [authenticated](AUTH.md) and defined a [default](DEFAULT.md) knowledgebox. In case you want to overwrite or define a one time knowledgebox you should add on any command/function the `url` and `api_key` parameter.
+
 ## Upload a file in a KnowledgeBox
 
 Pushing a file to a knowledgebox its easy as:
 
 ```bash
 nuclia kb upload file --path=FILE_PATH
 ```
 
+```python
+from nuclia import sdk
+upload = sdk.NucliaUpload()
+upload.file(FILE_PATH)
+```
+
+
 ## Upload a file in an existing resource
 
 
 In case you want to upload a file inside a resource you can use:
 
 ```bash
 nuclia kb upload file --path=FILE_PATH  --rid=RESOURCE_ID --field=FIELD_ID
```

### Comparing `nuclia-1.0.1/nuclia/cli/run.py` & `nuclia-1.0.2/nuclia/cli/run.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.0.1/nuclia/data.py` & `nuclia-1.0.2/nuclia/data.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.0.1/nuclia/decorators.py` & `nuclia-1.0.2/nuclia/decorators.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from nuclia.data import get_auth
 from nuclia.exceptions import NotDefinedDefault
 from nuclia.lib.kb import Environment, NucliaDBClient
+from nuclia.lib.nua import NuaClient
 
 
 def accounts(func):
     def wrapper_checkout_accounts(*args, **kwargs):
         auth = get_auth()
         auth.accounts()
         return func(*args, **kwargs)
@@ -25,19 +26,19 @@
 def kb(func):
     def wrapper_checkout_kb(*args, **kwargs):
         url = kwargs.get("url")
         api_key = kwargs.get("api_key")
         auth = get_auth()
         if url is None:
             # Get default KB
-            default = auth._config.get_default_kb()
-            if default.account is None or default.kbid is None:
+            kbid = auth._config.get_default_kb()
+            if kbid is None:
                 raise NotDefinedDefault()
 
-            kb_obj = auth._config.get_kb(default.kbid)
+            kb_obj = auth._config.get_kb(kbid)
 
             if kb_obj.region is None:
                 # OSS
                 ndb = NucliaDBClient(environment=Environment.OSS, url=kb_obj.url)
             else:
                 if kb_obj.token is None:
                     # User token auth
@@ -61,7 +62,24 @@
             )
         else:
             ndb = NucliaDBClient(environment=Environment.OSS, url=url)
         kwargs["ndb"] = ndb
         return func(*args, **kwargs)
 
     return wrapper_checkout_kb
+
+
+def nua(func):
+    def wrapper_checkout_nua(*args, **kwargs):
+        auth = get_auth()
+        nua_id = auth._config.get_default_nua()
+        if nua_id is None:
+            raise NotDefinedDefault()
+
+        nua_obj = auth._config.get_nua(nua_id)
+        nc = NuaClient(
+            region=nua_obj.region, account=nua_obj.account, token=nua_obj.token
+        )
+        kwargs["nc"] = nc
+        return func(*args, **kwargs)
+
+    return wrapper_checkout_nua
```

### Comparing `nuclia-1.0.1/nuclia/lib/kb.py` & `nuclia-1.0.2/nuclia/lib/kb.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.0.1/nuclia/sdk/auth.py` & `nuclia-1.0.2/nuclia/sdk/auth.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,106 +1,146 @@
 import base64
 import json
 import readline  # noqa
 import webbrowser
-from typing import Dict, List, Optional
+from typing import Dict, List, Optional, Tuple
 
 import requests
+from nucliadb_sdk import get_kb
 
 from nuclia import BASE, get_global_url, get_regional_url
 from nuclia.cli.utils import yes_no
 from nuclia.config import Account, Config, KnowledgeBox, Zone
 from nuclia.exceptions import NeedUserToken, UserTokenExpired
 
 USER = f"{BASE}/api/v1/user/welcome"
 MEMBER = f"{BASE}/api/v1/user"
 ACCOUNTS = f"{BASE}/api/v1/accounts"
 ZONES = f"{BASE}/api/v1/zones"
 LIST_KBS = BASE + "/api/v1/account/{account}/kbs"
+VERIFY_NUA = "/api/v1/nua/verify"
 
 
 class NucliaAuth:
     _inner_config: Optional[Config] = None
 
     @property
     def _config(self) -> Config:
         if self._inner_config is None:
             from nuclia.data import get_config
 
             self._inner_config = get_config()
         return self._inner_config
 
+    def show(self):
+        if self._config.default:
+            print("Default")
+            print("=======")
+            print()
+            print(get_kb(self._config.default.kbid))
+
+        if self._config.token:
+            print("User Auth")
+            print("=========")
+            print()
+            self._show_user()
+            print()
+
+        if len(self._config.kbs_token):
+            print("Knowledgebox Auth")
+            print("=================")
+            print()
+            for kb in self._config.kbs_token:
+                print(kb)
+
+        if len(self._config.nuas_token):
+            print("NUA Key")
+            print("=======")
+            print()
+            for nua in self._config.nuas_token:
+                print(nua)
+
     def kb(self, url: str, token: str):
         url = url.strip("/")
-        if self.validate_kb(url, token):
+        kbid, title = self.validate_kb(url, token)
+        if kbid:
             print("Validated")
             try:
-                kbid = url.split("/")[-1]
                 next(
                     filter(
                         lambda x: x.id == kbid,
                         self._config.kbs if self._config.kbs is not None else [],
                     )
                 )
                 if yes_no(f"Want to replace actual KB {kbid} configuration") is False:
                     print("Cancelling operation")
                     return
 
             except StopIteration:
                 # Not found
                 pass
 
-            self._config.set_kb_token(url, token)
+            self._config.set_kb_token(url=url, token=token, title=title, kbid=kbid)
         else:
             print("Invalid service token")
 
-    def nua(self, token: str):
-        # TODO
-        region = token
-        account = token
-        if self.validate_nua(region, token):
+    def nua(self, region: str, token: str) -> Optional[str]:
+        client_id, title, account = self.validate_nua(region, token)
+        if account is not None and client_id is not None:
             print("Validated")
-            self._config.set_nua_token(account, region, token)
+            self._config.set_nua_token(
+                client_id=client_id,
+                title=title,
+                account=account,
+                region=region,
+                token=token,
+            )
+            return account
         else:
             print("Invalid service token")
+            return None
 
-    def validate_nua(self, region: str, token: str):
+    def validate_nua(
+        self, region: str, token: str
+    ) -> Tuple[Optional[str], Optional[str], Optional[str]]:
         # Validate the code is ok
-        url = get_regional_url(region, "")
+        url = get_regional_url(region, VERIFY_NUA)
         resp = requests.get(
             url,
             headers={"X-STF-NUA": f"Bearer {token}"},
         )
         if resp.status_code == 200:
-            return True
+            data = resp.json()
+            return data.get("client_id"), data.get("title"), data.get("account")
         else:
-            return False
+            return None, None, None
 
-    def validate_kb(self, url: str, token: str):
+    def validate_kb(self, url: str, token: str) -> Tuple[Optional[str], Optional[str]]:
         # Validate the code is ok
         resp = requests.get(
             url,
             headers={"X-Nuclia-Serviceaccount": f"Bearer {token}"},
         )
         if resp.status_code == 200:
-            return True
+            data = resp.json()
+            return data.get("uuid"), data.get("config", {}).get("title")
         else:
-            return False
+            return None, None
 
     def _show_user(self):
-        print("Logged in!")
         resp = self.get_user(MEMBER)
         print(f"User: {resp.get('name')} <{resp.get('email')}>")
         print(f"Type: {resp.get('type')}")
 
     def login(self):
         """
         Lets redirect the user to the UI to capture a token
         """
         if self._validate_user_token():
+            print("Logged in!")
             self._show_user()
             return
 
         webbrowser.open(get_global_url("/redirect?display=token&ident={ident}"))
         code = input("Follow the browser flow and copy the token and paste it here:")
         print("Checking...")
         self.set_user_token(code)
@@ -109,22 +149,14 @@
         if self._validate_user_token(code):
             self._config.set_user_token(code)
             print("Auth completed!")
             self.post_login()
         else:
             print("Invalid token auth not completed")
 
-    def set_nua_token(self, region: str, token: str):
-        if self.validate_nua(region, token):
-            account = self._extract_account(token)
-            self._config.set_nua_token(account, region, token)
-            print("NUA auth completed!")
-        else:
-            print("Invalid token auth not completed")
-
     def _extract_account(self, token: str) -> str:
         base64url = token.split(".")[1]
         data = json.loads(
             base64.urlsafe_b64decode(base64url + "=" * (4 - len(base64url) % 4))
         )
         return data.get("jti")
```

### Comparing `nuclia-1.0.1/nuclia/sdk/kb.py` & `nuclia-1.0.2/nuclia/sdk/kb.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.0.1/nuclia/sdk/kbs.py` & `nuclia-1.0.2/nuclia/sdk/kbs.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict, Optional
 
 from nuclia import BASE
-from nuclia.config import Account, KnowledgeBox
+from nuclia.config import retrieve
 from nuclia.data import get_auth
 from nuclia.decorators import accounts
 from nuclia.sdk.auth import NucliaAuth
 
 ADD_KB = BASE + "/api/v1/account/{account}/kbs"
 
 
@@ -25,14 +25,22 @@
                 else []
             )
             for account_obj in accounts:
                 if account_obj.slug is not None:
                     result.extend(self._auth.kbs(account_obj.slug))
             self._auth._config.kbs = result
             self._auth._config.save()
+
+            # List the Knowledge Boxes configured as Service Token
+            result.extend(
+                self._auth._config.kbs_token
+                if self._auth._config.kbs_token is not None
+                else []
+            )
+
             return result
         else:
             return self._auth.kbs(account)
 
     def add(
         self,
         account: str,
@@ -42,42 +50,24 @@
         learning_configuration: Optional[Dict[str, str]] = None,
         sentence_embedder: Optional[str] = None,
         title: Optional[str] = None,
         zone: Optional[str] = None,
     ):
         # path = ADD_KB.format(account=account)
         raise NotImplementedError()
-
         # return self._auth.post_user(path, payload)
 
-    def default(self, *, account: str, kb: str):
-        accounts = (
-            self._auth._config.accounts
-            if self._auth._config.accounts is not None
-            else []
-        )
-        try:
-            account_obj: Account = next(filter(lambda x: x.slug == account, accounts))
-        except StopIteration:
-            try:
-                account_obj = next(filter(lambda x: x.id == account, accounts))
-            except StopIteration:
-                print(f"Account not found {account}")
-                return
-
+    def default(self, kb: str):
         kbs = self._auth._config.kbs if self._auth._config.kbs is not None else []
+        kb_obj = retrieve(kbs, kb)
+        if kb_obj is None:
+            kbs = (
+                self._auth._config.kbs_token
+                if self._auth._config.kbs_token is not None
+                else []
+            )
+            kb_obj = retrieve(kbs, kb)
 
-        try:
-            kb_obj: KnowledgeBox = next(filter(lambda x: x.slug == kb, kbs))
-        except StopIteration:
-            try:
-                kb_obj = next(filter(lambda x: x.id == kb, kbs))
-            except StopIteration:
-                print(f"KB not found {kb}")
-                return
-
-        self._auth._config.set_default_kb(account_obj.id, kb_obj.id)
+        if kb_obj is None:
+            raise KeyError("Knowledge Box not found")
+        self._auth._config.set_default_kb(kb_obj.id)
         self._auth._config.save()
-
-    def delete(self, account: str, slug: str):
-        # path = ADD_KB.format(account=account)
-        raise NotImplementedError()
```

### Comparing `nuclia-1.0.1/nuclia/sdk/search.py` & `nuclia-1.0.2/nuclia/sdk/search.py`

 * *Files identical despite different names*

### Comparing `nuclia-1.0.1/nuclia/sdk/upload.py` & `nuclia-1.0.2/nuclia/sdk/upload.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,24 +76,24 @@
                             {
                                 "who": message.who
                                 if message.who is not None
                                 else uuid4().hex,
                                 "to": [x for x in message.to]
                                 if message.to is not None
                                 else [],
-                                "ident": message.uuid
-                                if message.uuid is not None
+                                "ident": message.ident
+                                if message.ident is not None
                                 else uuid4().hex,
                                 "timestamp": message.timestamp
                                 if message.timestamp is not None
                                 else datetime.now().isoformat(),
                                 "content": {
-                                    "text": message.message.text,
-                                    "format": message.message.format
-                                    if message.message.format is not None
+                                    "text": message.content.text,
+                                    "format": message.content.format
+                                    if message.content.format is not None
                                     else "PLAIN",
                                 },
                             }
                             for message in conversation.messages
                         ]
                     }
                 },
```

### Comparing `nuclia-1.0.1/nuclia/tests/assets/conversation.json` & `nuclia-1.0.2/nuclia/tests/assets/conversation.json`

 * *Files identical despite different names*

### Comparing `nuclia-1.0.1/nuclia.egg-info/PKG-INFO` & `nuclia-1.0.2/nuclia.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuclia
-Version: 1.0.1
+Version: 1.0.2
 Summary: UNKNOWN
 Home-page: https://nuclia.com
 Author: Nuclia
 Author-email: info@nuclia.com
 License: BSD
 Project-URL: Nuclia, https://nuclia.com
 Project-URL: Github, https://github.com/nuclia/nucliadb
@@ -42,15 +42,15 @@
 
 
 ### Nuclia Knowledgebox
 
 You can login to a specific knowledgebox if you have a Service Token (How to get a Service Token) or your NucliaDB is [deployed on-premise](https://docs.nuclia.dev/docs/nucliadb/deploy)
 
 ```bash
-nuclia auth knowledgebox -kb KB_URL --key SERVICE_TOKEN
+nuclia auth kb --url KB_URL --token SERVICE_TOKEN
 ```
 
 KB_URL its the url of the Knowledge Box. On the cloud service you can retrieve it on the dashboard. On the on-premise/community deployment its the url mapped to it.
 
 
 ### Nuclia Understanding API
```

### Comparing `nuclia-1.0.1/nuclia.egg-info/SOURCES.txt` & `nuclia-1.0.2/nuclia.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,19 @@
 README.md
 VERSION
 code-requirements.txt
 requirements.txt
 setup.cfg
 setup.py
 test-requirements.txt
+docs/AUTH.md
 docs/CONVERSATION.md
+docs/DEFAULT.md
 docs/README.md
+docs/SEARCH.md
 docs/UPLOAD.md
 nuclia/__init__.py
 nuclia/config.py
 nuclia/data.py
 nuclia/decorators.py
 nuclia/exceptions.py
 nuclia.egg-info/PKG-INFO
@@ -27,22 +30,26 @@
 nuclia.egg-info/zip-safe
 nuclia/cli/__init__.py
 nuclia/cli/run.py
 nuclia/cli/utils.py
 nuclia/lib/__init__.py
 nuclia/lib/conversations.py
 nuclia/lib/kb.py
+nuclia/lib/nua.py
 nuclia/sdk/__init__.py
 nuclia/sdk/accounts.py
 nuclia/sdk/auth.py
 nuclia/sdk/kb.py
 nuclia/sdk/kbs.py
 nuclia/sdk/nua.py
 nuclia/sdk/nuas.py
+nuclia/sdk/predict.py
+nuclia/sdk/process.py
 nuclia/sdk/search.py
+nuclia/sdk/train.py
 nuclia/sdk/upload.py
 nuclia/sdk/zones.py
 nuclia/tests/__init__.py
 nuclia/tests/conftest.py
 nuclia/tests/fixtures.py
 nuclia/tests/test_auth.py
 nuclia/tests/test_conversation.py
```

### Comparing `nuclia-1.0.1/setup.py` & `nuclia-1.0.2/setup.py`

 * *Files identical despite different names*

