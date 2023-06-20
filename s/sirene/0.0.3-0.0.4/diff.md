# Comparing `tmp/sirene-0.0.3.tar.gz` & `tmp/sirene-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sirene-0.0.3.tar", last modified: Tue Jun 13 20:53:52 2023, max compression
+gzip compressed data, was "sirene-0.0.4.tar", last modified: Tue Jun 20 18:53:05 2023, max compression
```

## Comparing `sirene-0.0.3.tar` & `sirene-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-06-13 20:53:52.515097 sirene-0.0.3/
--rw-rw-r--   0 felipe    (1000) felipe    (1000)     1080 2023-05-01 17:49:02.000000 sirene-0.0.3/LICENSE
--rw-rw-r--   0 felipe    (1000) felipe    (1000)       41 2023-06-06 21:14:36.000000 sirene-0.0.3/MANIFEST.in
--rw-rw-r--   0 felipe    (1000) felipe    (1000)      554 2023-06-13 20:53:52.515097 sirene-0.0.3/PKG-INFO
--rw-rw-r--   0 felipe    (1000) felipe    (1000)       72 2023-06-06 21:09:38.000000 sirene-0.0.3/README.md
--rw-rw-r--   0 felipe    (1000) felipe    (1000)      103 2021-04-01 21:15:48.000000 sirene-0.0.3/pyproject.toml
--rw-rw-r--   0 felipe    (1000) felipe    (1000)      629 2023-06-13 20:53:52.515097 sirene-0.0.3/setup.cfg
-drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-06-13 20:53:52.507096 sirene-0.0.3/sirene/
-drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-06-13 20:53:52.503096 sirene-0.0.3/sirene/MCTI/
-drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-06-13 20:53:52.515097 sirene-0.0.3/sirene/MCTI/sexta_edicao/
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   154072 2023-06-06 21:32:26.000000 sirene-0.0.3/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_agropecuaria.xlsx
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   106995 2023-05-17 20:22:59.000000 sirene-0.0.3/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_energia.xlsx
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   117053 2023-05-17 20:23:08.000000 sirene-0.0.3/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_ippu.xlsx
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    45115 2023-05-17 20:23:17.000000 sirene-0.0.3/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_lulucf.xlsx
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    45235 2023-05-17 20:23:21.000000 sirene-0.0.3/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_residuos.xlsx
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    28706 2023-05-17 20:23:25.000000 sirene-0.0.3/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_total-brasil-1.xlsx
--rw-rw-r--   0 felipe    (1000) felipe    (1000)        0 2021-04-01 21:15:48.000000 sirene-0.0.3/sirene/__init__.py
--rw-rw-r--   0 felipe    (1000) felipe    (1000)     1055 2023-06-13 20:52:59.000000 sirene-0.0.3/sirene/srn.py
-drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-06-13 20:53:52.507096 sirene-0.0.3/sirene.egg-info/
--rw-rw-r--   0 felipe    (1000) felipe    (1000)      554 2023-06-13 20:53:52.000000 sirene-0.0.3/sirene.egg-info/PKG-INFO
--rw-rw-r--   0 felipe    (1000) felipe    (1000)      605 2023-06-13 20:53:52.000000 sirene-0.0.3/sirene.egg-info/SOURCES.txt
--rw-rw-r--   0 felipe    (1000) felipe    (1000)        1 2023-06-13 20:53:52.000000 sirene-0.0.3/sirene.egg-info/dependency_links.txt
--rw-rw-r--   0 felipe    (1000) felipe    (1000)        5 2023-06-13 20:53:52.000000 sirene-0.0.3/sirene.egg-info/requires.txt
--rw-rw-r--   0 felipe    (1000) felipe    (1000)        7 2023-06-13 20:53:52.000000 sirene-0.0.3/sirene.egg-info/top_level.txt
+drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-06-20 18:53:05.463507 sirene-0.0.4/
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     1080 2023-05-01 17:49:02.000000 sirene-0.0.4/LICENSE
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)       72 2023-06-20 18:18:56.000000 sirene-0.0.4/MANIFEST.in
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)      554 2023-06-20 18:53:05.463507 sirene-0.0.4/PKG-INFO
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)       72 2023-06-06 21:09:38.000000 sirene-0.0.4/README.md
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)      103 2021-04-01 21:15:48.000000 sirene-0.0.4/pyproject.toml
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)      617 2023-06-20 18:53:05.467507 sirene-0.0.4/setup.cfg
+drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-06-20 18:53:05.459507 sirene-0.0.4/sirene/
+drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-06-20 18:53:05.459507 sirene-0.0.4/sirene/MCTI/
+drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-06-20 18:53:05.463507 sirene-0.0.4/sirene/MCTI/sexta_edicao/
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   154072 2023-06-06 21:32:26.000000 sirene-0.0.4/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_agropecuaria.xlsx
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   106995 2023-05-17 20:22:59.000000 sirene-0.0.4/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_energia.xlsx
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   117053 2023-05-17 20:23:08.000000 sirene-0.0.4/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_ippu.xlsx
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    45115 2023-05-17 20:23:17.000000 sirene-0.0.4/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_lulucf.xlsx
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    45235 2023-05-17 20:23:21.000000 sirene-0.0.4/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_residuos.xlsx
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    28706 2023-05-17 20:23:25.000000 sirene-0.0.4/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_total-brasil-1.xlsx
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)        0 2021-04-01 21:15:48.000000 sirene-0.0.4/sirene/__init__.py
+drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-06-20 18:53:05.463507 sirene-0.0.4/sirene/mapbiomas/
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    84456 2023-06-20 18:02:31.000000 sirene-0.0.4/sirene/mapbiomas/coeficiente_desmatamento_por_bioma_atividade.csv
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    20155 2023-06-20 18:28:39.000000 sirene-0.0.4/sirene/srn.py
+drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-06-20 18:53:05.459507 sirene-0.0.4/sirene.egg-info/
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)      554 2023-06-20 18:53:05.000000 sirene-0.0.4/sirene.egg-info/PKG-INFO
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)      671 2023-06-20 18:53:05.000000 sirene-0.0.4/sirene.egg-info/SOURCES.txt
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)        1 2023-06-20 18:53:05.000000 sirene-0.0.4/sirene.egg-info/dependency_links.txt
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)       24 2023-06-20 18:53:05.000000 sirene-0.0.4/sirene.egg-info/requires.txt
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)        7 2023-06-20 18:53:05.000000 sirene-0.0.4/sirene.egg-info/top_level.txt
```

### Comparing `sirene-0.0.3/LICENSE` & `sirene-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sirene-0.0.3/PKG-INFO` & `sirene-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sirene
-Version: 0.0.3
+Version: 0.0.4
 Summary: Import data from the 'Sistema de Registro Nacional de Emissões' (SIRENE) from MCTI
 Home-page: https://github.com/fms-1988
 Author: Felipe Morelli Da Silva
 Author-email: fms.morelli@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sirene-0.0.3/setup.cfg` & `sirene-0.0.4/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [metadata]
 name = sirene
-version = 0.0.3
+version = 0.0.4
 author = Felipe Morelli Da Silva
 author_email = fms.morelli@gmail.com
 description = Import data from the 'Sistema de Registro Nacional de Emissões' (SIRENE) from MCTI
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/fms-1988
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 packages = find:
-install_requires = xlrd  # Add the 'xlrd' dependency here
+install_requires = xlrd; pandas; numpy; iotbr
 python_requires = >=3.7
 include_package_data = True
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `sirene-0.0.3/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_agropecuaria.xlsx` & `sirene-0.0.4/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_agropecuaria.xlsx`

 * *Files identical despite different names*

### Comparing `sirene-0.0.3/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_energia.xlsx` & `sirene-0.0.4/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_energia.xlsx`

 * *Files identical despite different names*

### Comparing `sirene-0.0.3/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_ippu.xlsx` & `sirene-0.0.4/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_ippu.xlsx`

 * *Files identical despite different names*

### Comparing `sirene-0.0.3/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_lulucf.xlsx` & `sirene-0.0.4/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_lulucf.xlsx`

 * *Files identical despite different names*

### Comparing `sirene-0.0.3/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_residuos.xlsx` & `sirene-0.0.4/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_residuos.xlsx`

 * *Files identical despite different names*

### Comparing `sirene-0.0.3/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_total-brasil-1.xlsx` & `sirene-0.0.4/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_total-brasil-1.xlsx`

 * *Files identical despite different names*

### Comparing `sirene-0.0.3/sirene.egg-info/PKG-INFO` & `sirene-0.0.4/sirene.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sirene
-Version: 0.0.3
+Version: 0.0.4
 Summary: Import data from the 'Sistema de Registro Nacional de Emissões' (SIRENE) from MCTI
 Home-page: https://github.com/fms-1988
 Author: Felipe Morelli Da Silva
 Author-email: fms.morelli@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

