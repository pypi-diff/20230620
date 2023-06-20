# Comparing `tmp/pycid-dev-0.0.8.tar.gz` & `tmp/pycid-dev-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/dockers/o_store/third_party_clients/pypi_staging/dist/tmp0caqmcgp/pycid-dev-0.0.8.tar", last modified: Sat Apr  9 18:24:58 2022, max compression
+gzip compressed data, was "pycid-dev-0.0.9.tar", last modified: Mon Jul 11 05:48:48 2022, max compression
```

## Comparing `pycid-dev-0.0.8.tar` & `pycid-dev-0.0.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 dockers   (1000) dockers   (1000)        0 2022-04-09 18:24:58.000000 pycid-dev-0.0.8/
--rw-rw-r--   0 dockers   (1000) dockers   (1000)      104 2021-05-31 15:42:57.000000 pycid-dev-0.0.8/pyproject.toml
--rw-rw-r--   0 dockers   (1000) dockers   (1000)       97 2021-06-06 23:04:53.000000 pycid-dev-0.0.8/README.md
--rw-rw-r--   0 dockers   (1000) dockers   (1000)     1047 2021-05-31 15:42:57.000000 pycid-dev-0.0.8/LICENSE
--rw-rw-r--   0 dockers   (1000) dockers   (1000)      317 2022-04-09 18:24:58.000000 pycid-dev-0.0.8/PKG-INFO
--rw-rw-r--   0 dockers   (1000) dockers   (1000)      356 2022-04-09 18:24:58.000000 pycid-dev-0.0.8/setup.cfg
-drwxrwxr-x   0 dockers   (1000) dockers   (1000)        0 2022-04-09 18:24:58.000000 pycid-dev-0.0.8/src/
-drwxrwxr-x   0 dockers   (1000) dockers   (1000)        0 2022-04-09 18:24:58.000000 pycid-dev-0.0.8/src/pycid_dev/
--rw-rw-r--   0 dockers   (1000) dockers   (1000)        0 2021-05-31 15:42:57.000000 pycid-dev-0.0.8/src/pycid_dev/__init__.py
--rw-rw-r--   0 dockers   (1000) dockers   (1000)     7536 2021-06-06 23:04:53.000000 pycid-dev-0.0.8/src/pycid_dev/client.py
-drwxrwxr-x   0 dockers   (1000) dockers   (1000)        0 2022-04-09 18:24:58.000000 pycid-dev-0.0.8/src/pycid_dev/lib/
-drwxrwxr-x   0 dockers   (1000) dockers   (1000)        0 2022-04-09 18:24:58.000000 pycid-dev-0.0.8/src/pycid_dev/lib/crate/
--rw-rw-r--   0 dockers   (1000) dockers   (1000)     1804 2021-05-31 15:42:57.000000 pycid-dev-0.0.8/src/pycid_dev/lib/crate/crate.py
--rw-rw-r--   0 dockers   (1000) dockers   (1000)        0 2021-05-31 15:42:57.000000 pycid-dev-0.0.8/src/pycid_dev/lib/crate/__init__.py
-drwxrwxr-x   0 dockers   (1000) dockers   (1000)        0 2022-04-09 18:24:58.000000 pycid-dev-0.0.8/src/pycid_dev/lib/component/
--rw-rw-r--   0 dockers   (1000) dockers   (1000)     5107 2021-06-06 23:04:53.000000 pycid-dev-0.0.8/src/pycid_dev/lib/component/component.py
--rw-rw-r--   0 dockers   (1000) dockers   (1000)        0 2021-05-31 15:42:57.000000 pycid-dev-0.0.8/src/pycid_dev/lib/component/__init__.py
-drwxrwxr-x   0 dockers   (1000) dockers   (1000)        0 2022-04-09 18:24:58.000000 pycid-dev-0.0.8/src/pycid_dev/lib/authentication/
--rwxrwxr-x   0 dockers   (1000) dockers   (1000)      673 2021-05-31 15:42:57.000000 pycid-dev-0.0.8/src/pycid_dev/lib/authentication/refresh.py
--rwxrwxr-x   0 dockers   (1000) dockers   (1000)     6768 2022-04-09 18:24:37.000000 pycid-dev-0.0.8/src/pycid_dev/lib/authentication/authentication.py
--rw-rw-r--   0 dockers   (1000) dockers   (1000)        0 2021-05-31 15:42:57.000000 pycid-dev-0.0.8/src/pycid_dev/lib/authentication/__init__.py
--rw-rw-r--   0 dockers   (1000) dockers   (1000)        0 2021-05-31 15:42:57.000000 pycid-dev-0.0.8/src/pycid_dev/lib/authentication/__main__.py
-drwxrwxr-x   0 dockers   (1000) dockers   (1000)        0 2022-04-09 18:24:58.000000 pycid-dev-0.0.8/src/pycid_dev/lib/craft/
--rw-rw-r--   0 dockers   (1000) dockers   (1000)        0 2021-05-31 15:42:57.000000 pycid-dev-0.0.8/src/pycid_dev/lib/craft/__init__.py
--rw-rw-r--   0 dockers   (1000) dockers   (1000)     3230 2021-05-31 15:42:57.000000 pycid-dev-0.0.8/src/pycid_dev/lib/craft/craft.py
--rw-rw-r--   0 dockers   (1000) dockers   (1000)        0 2021-05-31 15:42:57.000000 pycid-dev-0.0.8/src/pycid_dev/lib/__init__.py
-drwxrwxr-x   0 dockers   (1000) dockers   (1000)        0 2022-04-09 18:24:58.000000 pycid-dev-0.0.8/src/pycid_dev/lib/tree/
--rwxrwxr-x   0 dockers   (1000) dockers   (1000)     6445 2021-05-31 15:42:57.000000 pycid-dev-0.0.8/src/pycid_dev/lib/tree/tree.py
--rw-rw-r--   0 dockers   (1000) dockers   (1000)        0 2021-05-31 15:42:57.000000 pycid-dev-0.0.8/src/pycid_dev/lib/tree/__init__.py
-drwxrwxr-x   0 dockers   (1000) dockers   (1000)        0 2022-04-09 18:24:58.000000 pycid-dev-0.0.8/src/pycid_dev/lib/attribute/
--rw-rw-r--   0 dockers   (1000) dockers   (1000)       63 2021-05-31 15:42:57.000000 pycid-dev-0.0.8/src/pycid_dev/lib/attribute/constants.py
--rw-rw-r--   0 dockers   (1000) dockers   (1000)        0 2021-05-31 15:42:57.000000 pycid-dev-0.0.8/src/pycid_dev/lib/attribute/__init__.py
-drwxrwxr-x   0 dockers   (1000) dockers   (1000)        0 2022-04-09 18:24:58.000000 pycid-dev-0.0.8/src/pycid_dev.egg-info/
--rw-rw-r--   0 dockers   (1000) dockers   (1000)       10 2022-04-09 18:24:58.000000 pycid-dev-0.0.8/src/pycid_dev.egg-info/top_level.txt
--rw-rw-r--   0 dockers   (1000) dockers   (1000)      317 2022-04-09 18:24:58.000000 pycid-dev-0.0.8/src/pycid_dev.egg-info/PKG-INFO
--rw-rw-r--   0 dockers   (1000) dockers   (1000)      857 2022-04-09 18:24:58.000000 pycid-dev-0.0.8/src/pycid_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 dockers   (1000) dockers   (1000)        1 2022-04-09 18:24:58.000000 pycid-dev-0.0.8/src/pycid_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 dockers   (1000) dockers   (1000)       28 2022-04-09 18:24:58.000000 pycid-dev-0.0.8/src/pycid_dev.egg-info/requires.txt
+drwxrwxr-x   0 dockers   (1000) dockers   (1000)        0 2022-07-11 05:48:48.580998 pycid-dev-0.0.9/
+-rw-rw-r--   0 dockers   (1000) dockers   (1000)     1047 2021-05-31 15:42:57.000000 pycid-dev-0.0.9/LICENSE
+-rw-rw-r--   0 dockers   (1000) dockers   (1000)      261 2022-07-11 05:48:48.580998 pycid-dev-0.0.9/PKG-INFO
+-rw-rw-r--   0 dockers   (1000) dockers   (1000)       97 2021-06-06 23:04:53.000000 pycid-dev-0.0.9/README.md
+-rw-rw-r--   0 dockers   (1000) dockers   (1000)      104 2021-05-31 15:42:57.000000 pycid-dev-0.0.9/pyproject.toml
+-rw-rw-r--   0 dockers   (1000) dockers   (1000)      356 2022-07-11 05:48:48.580998 pycid-dev-0.0.9/setup.cfg
+drwxrwxr-x   0 dockers   (1000) dockers   (1000)        0 2022-07-11 05:48:48.568997 pycid-dev-0.0.9/src/
+drwxrwxr-x   0 dockers   (1000) dockers   (1000)        0 2022-07-11 05:48:48.572998 pycid-dev-0.0.9/src/pycid_dev/
+-rw-rw-r--   0 dockers   (1000) dockers   (1000)        0 2021-05-31 15:42:57.000000 pycid-dev-0.0.9/src/pycid_dev/__init__.py
+-rw-rw-r--   0 dockers   (1000) dockers   (1000)     7554 2022-07-11 05:48:40.000000 pycid-dev-0.0.9/src/pycid_dev/client.py
+drwxrwxr-x   0 dockers   (1000) dockers   (1000)        0 2022-07-11 05:48:48.576998 pycid-dev-0.0.9/src/pycid_dev/lib/
+-rw-rw-r--   0 dockers   (1000) dockers   (1000)        0 2021-05-31 15:42:57.000000 pycid-dev-0.0.9/src/pycid_dev/lib/__init__.py
+drwxrwxr-x   0 dockers   (1000) dockers   (1000)        0 2022-07-11 05:48:48.576998 pycid-dev-0.0.9/src/pycid_dev/lib/attribute/
+-rw-rw-r--   0 dockers   (1000) dockers   (1000)        0 2021-05-31 15:42:57.000000 pycid-dev-0.0.9/src/pycid_dev/lib/attribute/__init__.py
+-rw-rw-r--   0 dockers   (1000) dockers   (1000)       63 2021-05-31 15:42:57.000000 pycid-dev-0.0.9/src/pycid_dev/lib/attribute/constants.py
+drwxrwxr-x   0 dockers   (1000) dockers   (1000)        0 2022-07-11 05:48:48.576998 pycid-dev-0.0.9/src/pycid_dev/lib/authentication/
+-rw-rw-r--   0 dockers   (1000) dockers   (1000)        0 2021-05-31 15:42:57.000000 pycid-dev-0.0.9/src/pycid_dev/lib/authentication/__init__.py
+-rw-rw-r--   0 dockers   (1000) dockers   (1000)        0 2021-05-31 15:42:57.000000 pycid-dev-0.0.9/src/pycid_dev/lib/authentication/__main__.py
+-rwxrwxr-x   0 dockers   (1000) dockers   (1000)     6768 2022-04-09 18:24:37.000000 pycid-dev-0.0.9/src/pycid_dev/lib/authentication/authentication.py
+-rwxrwxr-x   0 dockers   (1000) dockers   (1000)      673 2021-05-31 15:42:57.000000 pycid-dev-0.0.9/src/pycid_dev/lib/authentication/refresh.py
+drwxrwxr-x   0 dockers   (1000) dockers   (1000)        0 2022-07-11 05:48:48.576998 pycid-dev-0.0.9/src/pycid_dev/lib/component/
+-rw-rw-r--   0 dockers   (1000) dockers   (1000)        0 2021-05-31 15:42:57.000000 pycid-dev-0.0.9/src/pycid_dev/lib/component/__init__.py
+-rw-rw-r--   0 dockers   (1000) dockers   (1000)     5107 2021-06-06 23:04:53.000000 pycid-dev-0.0.9/src/pycid_dev/lib/component/component.py
+drwxrwxr-x   0 dockers   (1000) dockers   (1000)        0 2022-07-11 05:48:48.576998 pycid-dev-0.0.9/src/pycid_dev/lib/craft/
+-rw-rw-r--   0 dockers   (1000) dockers   (1000)        0 2021-05-31 15:42:57.000000 pycid-dev-0.0.9/src/pycid_dev/lib/craft/__init__.py
+-rw-rw-r--   0 dockers   (1000) dockers   (1000)     3230 2021-05-31 15:42:57.000000 pycid-dev-0.0.9/src/pycid_dev/lib/craft/craft.py
+drwxrwxr-x   0 dockers   (1000) dockers   (1000)        0 2022-07-11 05:48:48.580998 pycid-dev-0.0.9/src/pycid_dev/lib/crate/
+-rw-rw-r--   0 dockers   (1000) dockers   (1000)        0 2021-05-31 15:42:57.000000 pycid-dev-0.0.9/src/pycid_dev/lib/crate/__init__.py
+-rw-rw-r--   0 dockers   (1000) dockers   (1000)     1804 2021-05-31 15:42:57.000000 pycid-dev-0.0.9/src/pycid_dev/lib/crate/crate.py
+drwxrwxr-x   0 dockers   (1000) dockers   (1000)        0 2022-07-11 05:48:48.580998 pycid-dev-0.0.9/src/pycid_dev/lib/tree/
+-rw-rw-r--   0 dockers   (1000) dockers   (1000)        0 2021-05-31 15:42:57.000000 pycid-dev-0.0.9/src/pycid_dev/lib/tree/__init__.py
+-rwxrwxr-x   0 dockers   (1000) dockers   (1000)     6445 2021-05-31 15:42:57.000000 pycid-dev-0.0.9/src/pycid_dev/lib/tree/tree.py
+drwxrwxr-x   0 dockers   (1000) dockers   (1000)        0 2022-07-11 05:48:48.572998 pycid-dev-0.0.9/src/pycid_dev.egg-info/
+-rw-rw-r--   0 dockers   (1000) dockers   (1000)      261 2022-07-11 05:48:48.000000 pycid-dev-0.0.9/src/pycid_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 dockers   (1000) dockers   (1000)      857 2022-07-11 05:48:48.000000 pycid-dev-0.0.9/src/pycid_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 dockers   (1000) dockers   (1000)        1 2022-07-11 05:48:48.000000 pycid-dev-0.0.9/src/pycid_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 dockers   (1000) dockers   (1000)       28 2022-07-11 05:48:48.000000 pycid-dev-0.0.9/src/pycid_dev.egg-info/requires.txt
+-rw-rw-r--   0 dockers   (1000) dockers   (1000)       10 2022-07-11 05:48:48.000000 pycid-dev-0.0.9/src/pycid_dev.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pycid-dev-0.0.8/LICENSE` & `pycid-dev-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pycid-dev-0.0.8/src/pycid_dev/client.py` & `pycid-dev-0.0.9/src/pycid_dev/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     #
     # User information queries
     #
     def crafts_info(self):
         """
         Gets the crafts available and the elements that it is composed of.
         """
-        return self._user_info["instances_v0_1"]
+        return self._user_info["user"]["instances_v0_1"]
 
     def fetch_craft(self, craft_id):
         """
         Pull all data for a craft from the network. Push it into a new Craft
 
         :returns A Craft object
 
@@ -92,15 +92,15 @@
         if not craft:
             raise ValueError("Provided craft id could not be found")
 
         # Pull down all the crates associated with the craft
         # TODO might want to keep these separated? or at a minimum store a mapping from node guid to crate guid that it belongs to
         aggregate_crate = []
         for crate in craft["instance_nodes"]:
-            aggregate_crate += self._fetch_instance_crate(crate)["payload"]
+            aggregate_crate += self._fetch_instance_crate(crate)["payload"]["crates"]
 
         # Pull down and create the tree associated with the craft
         the_tree = self._fetch_instance_tree(craft["tree"])
 
         return Craft(craft["name"], craft["id"], aggregate_crate, the_tree,
                      {"component_resync_query": self._component_resync_query,
                       "component_resync_execute": self._component_resync_execute,
```

### Comparing `pycid-dev-0.0.8/src/pycid_dev/lib/crate/crate.py` & `pycid-dev-0.0.9/src/pycid_dev/lib/crate/crate.py`

 * *Files identical despite different names*

### Comparing `pycid-dev-0.0.8/src/pycid_dev/lib/component/component.py` & `pycid-dev-0.0.9/src/pycid_dev/lib/component/component.py`

 * *Files identical despite different names*

### Comparing `pycid-dev-0.0.8/src/pycid_dev/lib/authentication/refresh.py` & `pycid-dev-0.0.9/src/pycid_dev/lib/authentication/refresh.py`

 * *Files identical despite different names*

### Comparing `pycid-dev-0.0.8/src/pycid_dev/lib/authentication/authentication.py` & `pycid-dev-0.0.9/src/pycid_dev/lib/authentication/authentication.py`

 * *Files identical despite different names*

### Comparing `pycid-dev-0.0.8/src/pycid_dev/lib/craft/craft.py` & `pycid-dev-0.0.9/src/pycid_dev/lib/craft/craft.py`

 * *Files identical despite different names*

### Comparing `pycid-dev-0.0.8/src/pycid_dev/lib/tree/tree.py` & `pycid-dev-0.0.9/src/pycid_dev/lib/tree/tree.py`

 * *Files identical despite different names*

### Comparing `pycid-dev-0.0.8/src/pycid_dev.egg-info/SOURCES.txt` & `pycid-dev-0.0.9/src/pycid_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

