# Comparing `tmp/appeau_client-0.0.5.tar.gz` & `tmp/appeau_client-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appeau_client-0.0.5.tar", last modified: Mon Jun  5 13:51:35 2023, max compression
+gzip compressed data, was "appeau_client-0.1.0.tar", last modified: Tue Jun 20 16:28:59 2023, max compression
```

## Comparing `appeau_client-0.0.5.tar` & `appeau_client-0.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:51:35.100070 appeau_client-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-05 13:51:35.096069 appeau_client-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-05 13:51:17.000000 appeau_client-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:51:35.096069 appeau_client-0.0.5/appeau_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 13:51:17.000000 appeau_client-0.0.5/appeau_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-05 13:51:17.000000 appeau_client-0.0.5/appeau_client/api_calculdirect_post.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-05 13:51:17.000000 appeau_client-0.0.5/appeau_client/api_date_calcul_parcelleId_get.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-05 13:51:17.000000 appeau_client-0.0.5/appeau_client/api_donnees_meteomulti_post.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-05 13:51:17.000000 appeau_client-0.0.5/appeau_client/api_parcelles_get_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-05 13:51:17.000000 appeau_client-0.0.5/appeau_client/api_parcelles_id_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-05 13:51:17.000000 appeau_client-0.0.5/appeau_client/api_parcelles_id_get.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-05 13:51:17.000000 appeau_client-0.0.5/appeau_client/api_parcelles_id_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 13:51:17.000000 appeau_client-0.0.5/appeau_client/api_parcelles_parcelleIddonnees_meteo_dateDebut_dateFin_get_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-05 13:51:17.000000 appeau_client-0.0.5/appeau_client/api_parcelles_parcelleIdresultat_dateDebut_dateFin_get_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-05 13:51:17.000000 appeau_client-0.0.5/appeau_client/api_parcelles_post.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-05 13:51:17.000000 appeau_client-0.0.5/appeau_client/api_parcellesattente_get_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-05 13:51:17.000000 appeau_client-0.0.5/appeau_client/api_parcellesdetails_get_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-05 13:51:17.000000 appeau_client-0.0.5/appeau_client/api_parcellesdetails_listParcellesId_get_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-05 13:51:17.000000 appeau_client-0.0.5/appeau_client/api_parcellesmulti_listParcellesIdresultat_dateDebut_dateFin_get_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-05 13:51:17.000000 appeau_client-0.0.5/appeau_client/login_check_post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:51:35.096069 appeau_client-0.0.5/appeau_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-05 13:51:35.000000 appeau_client-0.0.5/appeau_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-05 13:51:35.000000 appeau_client-0.0.5/appeau_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:51:35.000000 appeau_client-0.0.5/appeau_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-05 13:51:35.000000 appeau_client-0.0.5/appeau_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-05 13:51:35.000000 appeau_client-0.0.5/appeau_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 13:51:35.100070 appeau_client-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-05 13:51:17.000000 appeau_client-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:28:59.452746 appeau_client-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-20 16:28:59.452746 appeau_client-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-20 16:28:49.000000 appeau_client-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:28:59.452746 appeau_client-0.1.0/appeau_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-20 16:28:49.000000 appeau_client-0.1.0/appeau_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-20 16:28:49.000000 appeau_client-0.1.0/appeau_client/api_calculdirect_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-20 16:28:49.000000 appeau_client-0.1.0/appeau_client/api_date_calcul_parcelleId_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-20 16:28:49.000000 appeau_client-0.1.0/appeau_client/api_donnees_meteomulti_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-20 16:28:49.000000 appeau_client-0.1.0/appeau_client/api_parcelles_get_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-20 16:28:49.000000 appeau_client-0.1.0/appeau_client/api_parcelles_id_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-20 16:28:49.000000 appeau_client-0.1.0/appeau_client/api_parcelles_id_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-20 16:28:49.000000 appeau_client-0.1.0/appeau_client/api_parcelles_id_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-20 16:28:49.000000 appeau_client-0.1.0/appeau_client/api_parcelles_parcelleIddonnees_meteo_dateDebut_dateFin_get_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-20 16:28:49.000000 appeau_client-0.1.0/appeau_client/api_parcelles_parcelleIdresultat_dateDebut_dateFin_get_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-20 16:28:49.000000 appeau_client-0.1.0/appeau_client/api_parcelles_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-20 16:28:49.000000 appeau_client-0.1.0/appeau_client/api_parcellesattente_get_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-20 16:28:49.000000 appeau_client-0.1.0/appeau_client/api_parcellesdetails_get_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-20 16:28:49.000000 appeau_client-0.1.0/appeau_client/api_parcellesdetails_listParcellesId_get_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-20 16:28:49.000000 appeau_client-0.1.0/appeau_client/api_parcellesmulti_listParcellesIdresultat_dateDebut_dateFin_get_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-20 16:28:49.000000 appeau_client-0.1.0/appeau_client/login_check_post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:28:59.452746 appeau_client-0.1.0/appeau_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-20 16:28:59.000000 appeau_client-0.1.0/appeau_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-20 16:28:59.000000 appeau_client-0.1.0/appeau_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:28:59.000000 appeau_client-0.1.0/appeau_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 16:28:59.000000 appeau_client-0.1.0/appeau_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-20 16:28:59.000000 appeau_client-0.1.0/appeau_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 16:28:59.452746 appeau_client-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-20 16:28:49.000000 appeau_client-0.1.0/setup.py
```

### Comparing `appeau_client-0.0.5/PKG-INFO` & `appeau_client-0.1.0/appeau_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: appeau_client
-Version: 0.0.5
+Name: appeau-client
+Version: 0.1.0
 Summary: A client for http://appeau.api.vignevin-epicure.com API
 Author: Guilhem Heinrich
 Author-email: guilhem.heinrich@id2l.fr
 License: Apache 2.0
```

### Comparing `appeau_client-0.0.5/README.md` & `appeau_client-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `appeau_client-0.0.5/appeau_client/api_parcelles_id_patch.py` & `appeau_client-0.1.0/appeau_client/api_parcelles_id_patch.py`

 * *Files identical despite different names*

### Comparing `appeau_client-0.0.5/appeau_client/api_parcelles_parcelleIddonnees_meteo_dateDebut_dateFin_get_collection.py` & `appeau_client-0.1.0/appeau_client/api_parcelles_parcelleIddonnees_meteo_dateDebut_dateFin_get_collection.py`

 * *Files identical despite different names*

### Comparing `appeau_client-0.0.5/appeau_client/api_parcelles_parcelleIdresultat_dateDebut_dateFin_get_collection.py` & `appeau_client-0.1.0/appeau_client/api_parcelles_parcelleIdresultat_dateDebut_dateFin_get_collection.py`

 * *Files identical despite different names*

### Comparing `appeau_client-0.0.5/appeau_client/api_parcelles_post.py` & `appeau_client-0.1.0/appeau_client/api_parcelles_post.py`

 * *Files identical despite different names*

### Comparing `appeau_client-0.0.5/appeau_client/api_parcellesmulti_listParcellesIdresultat_dateDebut_dateFin_get_collection.py` & `appeau_client-0.1.0/appeau_client/api_parcellesmulti_listParcellesIdresultat_dateDebut_dateFin_get_collection.py`

 * *Files identical despite different names*

### Comparing `appeau_client-0.0.5/appeau_client/login_check_post.py` & `appeau_client-0.1.0/appeau_client/login_check_post.py`

 * *Files identical despite different names*

### Comparing `appeau_client-0.0.5/appeau_client.egg-info/PKG-INFO` & `appeau_client-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: appeau-client
-Version: 0.0.5
+Name: appeau_client
+Version: 0.1.0
 Summary: A client for http://appeau.api.vignevin-epicure.com API
 Author: Guilhem Heinrich
 Author-email: guilhem.heinrich@id2l.fr
 License: Apache 2.0
```

### Comparing `appeau_client-0.0.5/appeau_client.egg-info/SOURCES.txt` & `appeau_client-0.1.0/appeau_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `appeau_client-0.0.5/setup.py` & `appeau_client-0.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from setuptools import setup, find_packages
 # read the contents of your README file
 from pathlib import Path
+import appeau_client
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 # Voir https://blog.engineering.publicissapient.fr/2020/06/04/packaging-python-setup-py-et-setuptools/
 setup(name="appeau_client",
-version="0.0.5",
+version=appeau_client.__version__,
 description="A client for http://appeau.api.vignevin-epicure.com API",
 author="Guilhem Heinrich",
 author_email="guilhem.heinrich@id2l.fr",
 packages=["appeau_client"],
 # package_dir={'':'src'},
 # packages=find_packages('src'),
 install_requires=["requests"],
```

