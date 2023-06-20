# Comparing `tmp/pypomes-0.1.1.tar.gz` & `tmp/pypomes-0.1.2.tar.gz`

## Comparing `pypomes-0.1.1.tar` & `pypomes-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 pypomes-0.1.1/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes-0.1.1/src/pypomes/__init__.py
--rw-r--r--   0        0        0     7637 2020-02-02 00:00:00.000000 pypomes-0.1.1/src/pypomes/azure_pomes.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 pypomes-0.1.1/src/pypomes/crypto_pomes.py
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 pypomes-0.1.1/src/pypomes/datetime_pomes.py
--rw-r--r--   0        0        0    27033 2020-02-02 00:00:00.000000 pypomes-0.1.1/src/pypomes/dict_pomes.py
--rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 pypomes-0.1.1/src/pypomes/encoding_pomes.py
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 pypomes-0.1.1/src/pypomes/env_pomes.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 pypomes-0.1.1/src/pypomes/exception_pomes.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 pypomes-0.1.1/src/pypomes/json_pomes.py
--rw-r--r--   0        0        0     6179 2020-02-02 00:00:00.000000 pypomes-0.1.1/src/pypomes/list_pomes.py
--rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 pypomes-0.1.1/src/pypomes/logging_pomes.py
--rw-r--r--   0        0        0    10457 2020-02-02 00:00:00.000000 pypomes-0.1.1/src/pypomes/minio_pomes.py
--rw-r--r--   0        0        0    10963 2020-02-02 00:00:00.000000 pypomes-0.1.1/src/pypomes/postgres_pomes.py
--rw-r--r--   0        0        0     7331 2020-02-02 00:00:00.000000 pypomes-0.1.1/src/pypomes/soap_pomes.py
--rw-r--r--   0        0        0    12078 2020-02-02 00:00:00.000000 pypomes-0.1.1/src/pypomes/sqlserver_pomes.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pypomes-0.1.1/src/pypomes/str_pomes.py
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 pypomes-0.1.1/src/pypomes/xml_pomes.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pypomes-0.1.1/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes-0.1.1/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes-0.1.1/README.md
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 pypomes-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 pypomes-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 pypomes-0.1.2/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes-0.1.2/src/pypomes/__init__.py
+-rw-r--r--   0        0        0     7637 2020-02-02 00:00:00.000000 pypomes-0.1.2/src/pypomes/azure_pomes.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 pypomes-0.1.2/src/pypomes/crypto_pomes.py
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 pypomes-0.1.2/src/pypomes/datetime_pomes.py
+-rw-r--r--   0        0        0    27531 2020-02-02 00:00:00.000000 pypomes-0.1.2/src/pypomes/dict_pomes.py
+-rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 pypomes-0.1.2/src/pypomes/encoding_pomes.py
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 pypomes-0.1.2/src/pypomes/env_pomes.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 pypomes-0.1.2/src/pypomes/exception_pomes.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 pypomes-0.1.2/src/pypomes/file_pomes.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 pypomes-0.1.2/src/pypomes/json_pomes.py
+-rw-r--r--   0        0        0     6179 2020-02-02 00:00:00.000000 pypomes-0.1.2/src/pypomes/list_pomes.py
+-rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 pypomes-0.1.2/src/pypomes/logging_pomes.py
+-rw-r--r--   0        0        0    10457 2020-02-02 00:00:00.000000 pypomes-0.1.2/src/pypomes/minio_pomes.py
+-rw-r--r--   0        0        0    10963 2020-02-02 00:00:00.000000 pypomes-0.1.2/src/pypomes/postgres_pomes.py
+-rw-r--r--   0        0        0     7331 2020-02-02 00:00:00.000000 pypomes-0.1.2/src/pypomes/soap_pomes.py
+-rw-r--r--   0        0        0    12078 2020-02-02 00:00:00.000000 pypomes-0.1.2/src/pypomes/sqlserver_pomes.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pypomes-0.1.2/src/pypomes/str_pomes.py
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 pypomes-0.1.2/src/pypomes/xml_pomes.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pypomes-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes-0.1.2/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes-0.1.2/README.md
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 pypomes-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 pypomes-0.1.2/PKG-INFO
```

### Comparing `pypomes-0.1.1/src/pypomes/azure_pomes.py` & `pypomes-0.1.2/src/pypomes/azure_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.1/src/pypomes/crypto_pomes.py` & `pypomes-0.1.2/src/pypomes/crypto_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.1/src/pypomes/datetime_pomes.py` & `pypomes-0.1.2/src/pypomes/datetime_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.1/src/pypomes/dict_pomes.py` & `pypomes-0.1.2/src/pypomes/dict_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from flask import Request
 import inspect
 import types
 import list_pomes
 
 
 def dict_has_key_chain(source: dict, key_chain: list[str]) -> bool:
     """
@@ -534,14 +535,32 @@
             else:
                 # não, prossiga linearmente
                 result[name] = value
 
     return result
 
 
+def dict_from_form(request: Request) -> dict:
+    """
+    Constrói e retorna um *dict* com os parâmetros encontrados no form existente em *request*.
+
+    :param request: the HTTP request
+    :return: dicionários contendo os parâmetros encontrados.
+    """
+
+    # inicializa variável de retorno
+    result: dict = {}
+
+    # percorre os parâmetros do form
+    for key, value in request.form.items():
+        result[key] = value
+
+    return result
+
+
 def dict_transform(source: dict, from_to_keys: list[tuple[str, str]],
                    prefix_from: str = None, prefix_to: str = None) -> dict:
     """
     Constrói um novo *dict*, atribuindo a cada elemento indicado pelo segundo elemento de uma
     tupla contendo uma cadeia de chaves aninhadas em *from_to_keys*, o valor do elemento
     de *source* indicado pelo primeiro elemento da tupla, também contendo uma cadeia de chaves
     aninhadas, respectivamente para todos os elementos mapeados em *from_to_keys*.
```

### Comparing `pypomes-0.1.1/src/pypomes/encoding_pomes.py` & `pypomes-0.1.2/src/pypomes/encoding_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.1/src/pypomes/env_pomes.py` & `pypomes-0.1.2/src/pypomes/env_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.1/src/pypomes/exception_pomes.py` & `pypomes-0.1.2/src/pypomes/exception_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.1/src/pypomes/json_pomes.py` & `pypomes-0.1.2/src/pypomes/json_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.1/src/pypomes/list_pomes.py` & `pypomes-0.1.2/src/pypomes/list_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.1/src/pypomes/logging_pomes.py` & `pypomes-0.1.2/src/pypomes/logging_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.1/src/pypomes/minio_pomes.py` & `pypomes-0.1.2/src/pypomes/minio_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.1/src/pypomes/postgres_pomes.py` & `pypomes-0.1.2/src/pypomes/postgres_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.1/src/pypomes/soap_pomes.py` & `pypomes-0.1.2/src/pypomes/soap_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.1/src/pypomes/sqlserver_pomes.py` & `pypomes-0.1.2/src/pypomes/sqlserver_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.1/src/pypomes/str_pomes.py` & `pypomes-0.1.2/src/pypomes/str_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.1/src/pypomes/xml_pomes.py` & `pypomes-0.1.2/src/pypomes/xml_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.1/LICENSE` & `pypomes-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.1/pyproject.toml` & `pypomes-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "xmltodict3>=0.0.4",
     "zeep>=4.2.1"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" },
 ]
 description = "A collection of Python pomes, pennyeach"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

