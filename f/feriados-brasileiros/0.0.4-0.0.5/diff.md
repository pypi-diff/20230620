# Comparing `tmp/feriados_brasileiros-0.0.4.tar.gz` & `tmp/feriados_brasileiros-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feriados_brasileiros-0.0.4.tar", last modified: Tue Jun 20 02:56:18 2023, max compression
+gzip compressed data, was "feriados_brasileiros-0.0.5.tar", last modified: Tue Jun 20 03:00:07 2023, max compression
```

## Comparing `feriados_brasileiros-0.0.4.tar` & `feriados_brasileiros-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:56:18.641154 feriados_brasileiros-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-20 02:56:09.000000 feriados_brasileiros-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-20 02:56:09.000000 feriados_brasileiros-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-06-20 02:56:18.641154 feriados_brasileiros-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-20 02:56:09.000000 feriados_brasileiros-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:56:18.637154 feriados_brasileiros-0.0.4/feriados_brasileiros/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-20 02:56:09.000000 feriados_brasileiros-0.0.4/feriados_brasileiros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17405 2023-06-20 02:56:09.000000 feriados_brasileiros-0.0.4/feriados_brasileiros/datas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:56:18.641154 feriados_brasileiros-0.0.4/feriados_brasileiros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-06-20 02:56:18.000000 feriados_brasileiros-0.0.4/feriados_brasileiros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-20 02:56:18.000000 feriados_brasileiros-0.0.4/feriados_brasileiros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 02:56:18.000000 feriados_brasileiros-0.0.4/feriados_brasileiros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 02:56:18.000000 feriados_brasileiros-0.0.4/feriados_brasileiros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-20 02:56:18.000000 feriados_brasileiros-0.0.4/feriados_brasileiros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 02:56:09.000000 feriados_brasileiros-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 02:56:18.641154 feriados_brasileiros-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-20 02:56:09.000000 feriados_brasileiros-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:00:07.010294 feriados_brasileiros-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-20 02:59:58.000000 feriados_brasileiros-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-20 02:59:58.000000 feriados_brasileiros-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-06-20 03:00:07.010294 feriados_brasileiros-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-06-20 02:59:58.000000 feriados_brasileiros-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:00:07.010294 feriados_brasileiros-0.0.5/feriados_brasileiros/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-20 02:59:58.000000 feriados_brasileiros-0.0.5/feriados_brasileiros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17405 2023-06-20 02:59:58.000000 feriados_brasileiros-0.0.5/feriados_brasileiros/datas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:00:07.010294 feriados_brasileiros-0.0.5/feriados_brasileiros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-06-20 03:00:06.000000 feriados_brasileiros-0.0.5/feriados_brasileiros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-20 03:00:07.000000 feriados_brasileiros-0.0.5/feriados_brasileiros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 03:00:06.000000 feriados_brasileiros-0.0.5/feriados_brasileiros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 03:00:06.000000 feriados_brasileiros-0.0.5/feriados_brasileiros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-20 03:00:06.000000 feriados_brasileiros-0.0.5/feriados_brasileiros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 02:59:58.000000 feriados_brasileiros-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 03:00:07.010294 feriados_brasileiros-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-20 02:59:58.000000 feriados_brasileiros-0.0.5/setup.py
```

### Comparing `feriados_brasileiros-0.0.4/LICENSE` & `feriados_brasileiros-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `feriados_brasileiros-0.0.4/MANIFEST.in` & `feriados_brasileiros-0.0.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `feriados_brasileiros-0.0.4/PKG-INFO` & `feriados_brasileiros-0.0.5/feriados_brasileiros.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: feriados_brasileiros
-Version: 0.0.4
+Name: feriados-brasileiros
+Version: 0.0.5
 Summary: Feriados Brasileiros
 Home-page: https://github.com/michelmetran/feriados
 Author: Michel Metran
 Author-email: michelmetran@gmail.com
 Keywords: python,dados espaciais,geoprocessamento
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -70,15 +70,15 @@
 - `feriado`: Indica se é feriado ou apenas uma data que usualmente "enforca-se", porém não é feriado formalmente (exemplo: véspera de natal e quarta-feira de cinzas);
 - `obs`: Campo para observações quaisquer;
 
 ```python
 from feriados_brasileiros import datas
 
 # Adiciona apenas um feriado de um determinado ano
-feriados = Feriados(ano=2023)
+feriados = datas.Feriados(ano=2023)
 feriados.add(nome='Sexta-feira Santa', nome_alternativo='Paixão de Cristo', obs='Também conhecido como Sexta-feira Santa')
 feriados
 ```
 
 <br>
 
 ---
@@ -132,16 +132,16 @@
 
 ```python
 # Resultado em Lista
 lista_feriados = feriados.create_list(tipo='datetime')
 print(lista_feriados)
 
 # Resultado em Tabela (mais informações)
-df = feriados.create_table()
-print(df.head())
+df_feriados = feriados.create_table()
+print(df_feriados.head())
 ```
 
 <br>
 
 ---
 
 ## Documentação
```

### Comparing `feriados_brasileiros-0.0.4/README.md` & `feriados_brasileiros-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 - `feriado`: Indica se é feriado ou apenas uma data que usualmente "enforca-se", porém não é feriado formalmente (exemplo: véspera de natal e quarta-feira de cinzas);
 - `obs`: Campo para observações quaisquer;
 
 ```python
 from feriados_brasileiros import datas
 
 # Adiciona apenas um feriado de um determinado ano
-feriados = Feriados(ano=2023)
+feriados = datas.Feriados(ano=2023)
 feriados.add(nome='Sexta-feira Santa', nome_alternativo='Paixão de Cristo', obs='Também conhecido como Sexta-feira Santa')
 feriados
 ```
 
 <br>
 
 ---
@@ -115,16 +115,16 @@
 
 ```python
 # Resultado em Lista
 lista_feriados = feriados.create_list(tipo='datetime')
 print(lista_feriados)
 
 # Resultado em Tabela (mais informações)
-df = feriados.create_table()
-print(df.head())
+df_feriados = feriados.create_table()
+print(df_feriados.head())
 ```
 
 <br>
 
 ---
 
 ## Documentação
```

### Comparing `feriados_brasileiros-0.0.4/feriados_brasileiros/datas.py` & `feriados_brasileiros-0.0.5/feriados_brasileiros/datas.py`

 * *Files identical despite different names*

### Comparing `feriados_brasileiros-0.0.4/feriados_brasileiros.egg-info/PKG-INFO` & `feriados_brasileiros-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: feriados-brasileiros
-Version: 0.0.4
+Name: feriados_brasileiros
+Version: 0.0.5
 Summary: Feriados Brasileiros
 Home-page: https://github.com/michelmetran/feriados
 Author: Michel Metran
 Author-email: michelmetran@gmail.com
 Keywords: python,dados espaciais,geoprocessamento
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -70,15 +70,15 @@
 - `feriado`: Indica se é feriado ou apenas uma data que usualmente "enforca-se", porém não é feriado formalmente (exemplo: véspera de natal e quarta-feira de cinzas);
 - `obs`: Campo para observações quaisquer;
 
 ```python
 from feriados_brasileiros import datas
 
 # Adiciona apenas um feriado de um determinado ano
-feriados = Feriados(ano=2023)
+feriados = datas.Feriados(ano=2023)
 feriados.add(nome='Sexta-feira Santa', nome_alternativo='Paixão de Cristo', obs='Também conhecido como Sexta-feira Santa')
 feriados
 ```
 
 <br>
 
 ---
@@ -132,16 +132,16 @@
 
 ```python
 # Resultado em Lista
 lista_feriados = feriados.create_list(tipo='datetime')
 print(lista_feriados)
 
 # Resultado em Tabela (mais informações)
-df = feriados.create_table()
-print(df.head())
+df_feriados = feriados.create_table()
+print(df_feriados.head())
 ```
 
 <br>
 
 ---
 
 ## Documentação
```

### Comparing `feriados_brasileiros-0.0.4/setup.py` & `feriados_brasileiros-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 requirements = []
 for line in open('requirements.txt', encoding='utf-8'):
     li = line.strip()
     if not li.startswith('#'):
         requirements.append(line.rstrip())
 
-VERSION = (0, 0, 4)
+VERSION = (0, 0, 5)
 __version__ = '.'.join(map(str, VERSION))
 
 setup(
     name='feriados_brasileiros',
     version=__version__,
     author='Michel Metran',
     author_email='michelmetran@gmail.com',
```

