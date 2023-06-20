# Comparing `tmp/molecule-glesys-0.3.tar.gz` & `tmp/molecule-glesys-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecule-glesys-0.3.tar", last modified: Thu Aug 25 09:00:25 2022, max compression
+gzip compressed data, was "molecule-glesys-0.4.tar", last modified: Tue Jun 20 06:50:58 2023, max compression
```

## Comparing `molecule-glesys-0.3.tar` & `molecule-glesys-0.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 magnus    (1000) magnus    (1000)        0 2022-08-25 09:00:25.905846 molecule-glesys-0.3/
--rw-rw-r--   0 magnus    (1000) magnus    (1000)       39 2022-08-22 14:17:41.000000 molecule-glesys-0.3/.gitignore
--rw-rw-r--   0 magnus    (1000) magnus    (1000)     1065 2022-08-19 06:29:01.000000 molecule-glesys-0.3/LICENSE
--rw-rw-r--   0 magnus    (1000) magnus    (1000)     1900 2022-08-25 09:00:25.905846 molecule-glesys-0.3/PKG-INFO
--rw-rw-r--   0 magnus    (1000) magnus    (1000)     1020 2022-08-24 09:08:50.000000 molecule-glesys-0.3/README.md
-drwxrwxr-x   0 magnus    (1000) magnus    (1000)        0 2022-08-25 09:00:25.901846 molecule-glesys-0.3/molecule_glesys/
--rw-rw-r--   0 magnus    (1000) magnus    (1000)       58 2021-08-11 05:07:16.000000 molecule-glesys-0.3/molecule_glesys/__init__.py
-drwxrwxr-x   0 magnus    (1000) magnus    (1000)        0 2022-08-25 09:00:25.901846 molecule-glesys-0.3/molecule_glesys/cookiecutter/
--rw-rw-r--   0 magnus    (1000) magnus    (1000)      250 2021-08-11 05:07:16.000000 molecule-glesys-0.3/molecule_glesys/cookiecutter/cookiecutter.json
-drwxrwxr-x   0 magnus    (1000) magnus    (1000)        0 2022-08-25 09:00:25.901846 molecule-glesys-0.3/molecule_glesys/cookiecutter/{{cookiecutter.molecule_directory}}/
-drwxrwxr-x   0 magnus    (1000) magnus    (1000)        0 2022-08-25 09:00:25.901846 molecule-glesys-0.3/molecule_glesys/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-rw-r--   0 magnus    (1000) magnus    (1000)      179 2022-08-18 08:49:05.000000 molecule-glesys-0.3/molecule_glesys/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst
--rw-rw-r--   0 magnus    (1000) magnus    (1000)       82 2022-08-25 07:10:25.000000 molecule-glesys-0.3/molecule_glesys/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/collections.yml
--rw-rw-r--   0 magnus    (1000) magnus    (1000)      175 2022-08-25 08:48:18.000000 molecule-glesys-0.3/molecule_glesys/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
--rw-rw-r--   0 magnus    (1000) magnus    (1000)     1792 2022-08-25 08:48:36.000000 molecule-glesys-0.3/molecule_glesys/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/create.yml
--rw-rw-r--   0 magnus    (1000) magnus    (1000)      830 2022-08-25 08:48:58.000000 molecule-glesys-0.3/molecule_glesys/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/destroy.yml
-drwxrwxr-x   0 magnus    (1000) magnus    (1000)        0 2022-08-25 09:00:25.901846 molecule-glesys-0.3/molecule_glesys/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/handlers/
--rw-rw-r--   0 magnus    (1000) magnus    (1000)     1081 2022-08-25 08:47:45.000000 molecule-glesys-0.3/molecule_glesys/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/handlers/main.yml
--rw-rw-r--   0 magnus    (1000) magnus    (1000)     1447 2022-08-23 14:07:59.000000 molecule-glesys-0.3/molecule_glesys/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/molecule.yml
--rw-rw-r--   0 magnus    (1000) magnus    (1000)     2261 2022-08-17 09:59:22.000000 molecule-glesys-0.3/molecule_glesys/driver.py
-drwxrwxr-x   0 magnus    (1000) magnus    (1000)        0 2022-08-25 09:00:25.901846 molecule-glesys-0.3/molecule_glesys.egg-info/
--rw-rw-r--   0 magnus    (1000) magnus    (1000)     1900 2022-08-25 09:00:25.000000 molecule-glesys-0.3/molecule_glesys.egg-info/PKG-INFO
--rw-rw-r--   0 magnus    (1000) magnus    (1000)     1204 2022-08-25 09:00:25.000000 molecule-glesys-0.3/molecule_glesys.egg-info/SOURCES.txt
--rw-rw-r--   0 magnus    (1000) magnus    (1000)        1 2022-08-25 09:00:25.000000 molecule-glesys-0.3/molecule_glesys.egg-info/dependency_links.txt
--rw-rw-r--   0 magnus    (1000) magnus    (1000)       57 2022-08-25 09:00:25.000000 molecule-glesys-0.3/molecule_glesys.egg-info/entry_points.txt
--rw-rw-r--   0 magnus    (1000) magnus    (1000)        1 2022-08-22 13:19:54.000000 molecule-glesys-0.3/molecule_glesys.egg-info/not-zip-safe
--rw-rw-r--   0 magnus    (1000) magnus    (1000)       54 2022-08-25 09:00:25.000000 molecule-glesys-0.3/molecule_glesys.egg-info/requires.txt
--rw-rw-r--   0 magnus    (1000) magnus    (1000)       16 2022-08-25 09:00:25.000000 molecule-glesys-0.3/molecule_glesys.egg-info/top_level.txt
--rw-rw-r--   0 magnus    (1000) magnus    (1000)      134 2022-08-22 13:14:05.000000 molecule-glesys-0.3/pyproject.toml
--rw-rw-r--   0 magnus    (1000) magnus    (1000)     1324 2022-08-25 09:00:25.905846 molecule-glesys-0.3/setup.cfg
--rw-rw-r--   0 magnus    (1000) magnus    (1000)      112 2021-08-11 05:07:16.000000 molecule-glesys-0.3/setup.py
+drwxrwxr-x   0 larsd     (1000) larsd     (1000)        0 2023-06-20 06:50:58.521991 molecule-glesys-0.4/
+-rw-rw-r--   0 larsd     (1000) larsd     (1000)       39 2023-06-20 06:38:03.000000 molecule-glesys-0.4/.gitignore
+-rw-rw-r--   0 larsd     (1000) larsd     (1000)     1065 2023-06-20 06:38:03.000000 molecule-glesys-0.4/LICENSE
+-rw-rw-r--   0 larsd     (1000) larsd     (1000)     1918 2023-06-20 06:50:58.521991 molecule-glesys-0.4/PKG-INFO
+-rw-rw-r--   0 larsd     (1000) larsd     (1000)     1038 2023-06-20 06:38:03.000000 molecule-glesys-0.4/README.md
+drwxrwxr-x   0 larsd     (1000) larsd     (1000)        0 2023-06-20 06:50:58.521991 molecule-glesys-0.4/molecule_glesys/
+-rw-rw-r--   0 larsd     (1000) larsd     (1000)       58 2023-06-20 06:38:03.000000 molecule-glesys-0.4/molecule_glesys/__init__.py
+drwxrwxr-x   0 larsd     (1000) larsd     (1000)        0 2023-06-20 06:50:58.521991 molecule-glesys-0.4/molecule_glesys/cookiecutter/
+-rw-rw-r--   0 larsd     (1000) larsd     (1000)      250 2023-06-20 06:38:03.000000 molecule-glesys-0.4/molecule_glesys/cookiecutter/cookiecutter.json
+drwxrwxr-x   0 larsd     (1000) larsd     (1000)        0 2023-06-20 06:50:58.517991 molecule-glesys-0.4/molecule_glesys/cookiecutter/{{cookiecutter.molecule_directory}}/
+drwxrwxr-x   0 larsd     (1000) larsd     (1000)        0 2023-06-20 06:50:58.521991 molecule-glesys-0.4/molecule_glesys/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-rw-r--   0 larsd     (1000) larsd     (1000)      179 2023-06-20 06:38:03.000000 molecule-glesys-0.4/molecule_glesys/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/INSTALL.rst
+-rw-rw-r--   0 larsd     (1000) larsd     (1000)       82 2023-06-20 06:38:03.000000 molecule-glesys-0.4/molecule_glesys/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/collections.yml
+-rw-rw-r--   0 larsd     (1000) larsd     (1000)      175 2023-06-20 06:38:03.000000 molecule-glesys-0.4/molecule_glesys/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
+-rw-rw-r--   0 larsd     (1000) larsd     (1000)     1792 2023-06-20 06:38:03.000000 molecule-glesys-0.4/molecule_glesys/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/create.yml
+-rw-rw-r--   0 larsd     (1000) larsd     (1000)      830 2023-06-20 06:38:03.000000 molecule-glesys-0.4/molecule_glesys/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/destroy.yml
+drwxrwxr-x   0 larsd     (1000) larsd     (1000)        0 2023-06-20 06:50:58.521991 molecule-glesys-0.4/molecule_glesys/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/handlers/
+-rw-rw-r--   0 larsd     (1000) larsd     (1000)     1081 2023-06-20 06:38:03.000000 molecule-glesys-0.4/molecule_glesys/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/handlers/main.yml
+-rw-rw-r--   0 larsd     (1000) larsd     (1000)     1447 2023-06-20 06:38:03.000000 molecule-glesys-0.4/molecule_glesys/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/molecule.yml
+-rw-rw-r--   0 larsd     (1000) larsd     (1000)     2270 2023-06-20 06:38:03.000000 molecule-glesys-0.4/molecule_glesys/driver.py
+drwxrwxr-x   0 larsd     (1000) larsd     (1000)        0 2023-06-20 06:50:58.521991 molecule-glesys-0.4/molecule_glesys.egg-info/
+-rw-rw-r--   0 larsd     (1000) larsd     (1000)     1918 2023-06-20 06:50:58.000000 molecule-glesys-0.4/molecule_glesys.egg-info/PKG-INFO
+-rw-rw-r--   0 larsd     (1000) larsd     (1000)     1204 2023-06-20 06:50:58.000000 molecule-glesys-0.4/molecule_glesys.egg-info/SOURCES.txt
+-rw-rw-r--   0 larsd     (1000) larsd     (1000)        1 2023-06-20 06:50:58.000000 molecule-glesys-0.4/molecule_glesys.egg-info/dependency_links.txt
+-rw-rw-r--   0 larsd     (1000) larsd     (1000)       66 2023-06-20 06:50:58.000000 molecule-glesys-0.4/molecule_glesys.egg-info/entry_points.txt
+-rw-rw-r--   0 larsd     (1000) larsd     (1000)        1 2023-06-20 06:42:30.000000 molecule-glesys-0.4/molecule_glesys.egg-info/not-zip-safe
+-rw-rw-r--   0 larsd     (1000) larsd     (1000)       54 2023-06-20 06:50:58.000000 molecule-glesys-0.4/molecule_glesys.egg-info/requires.txt
+-rw-rw-r--   0 larsd     (1000) larsd     (1000)       16 2023-06-20 06:50:58.000000 molecule-glesys-0.4/molecule_glesys.egg-info/top_level.txt
+-rw-rw-r--   0 larsd     (1000) larsd     (1000)      134 2023-06-20 06:38:03.000000 molecule-glesys-0.4/pyproject.toml
+-rw-rw-r--   0 larsd     (1000) larsd     (1000)     1333 2023-06-20 06:50:58.521991 molecule-glesys-0.4/setup.cfg
+-rw-rw-r--   0 larsd     (1000) larsd     (1000)      112 2023-06-20 06:38:03.000000 molecule-glesys-0.4/setup.py
```

### Comparing `molecule-glesys-0.3/LICENSE` & `molecule-glesys-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `molecule-glesys-0.3/PKG-INFO` & `molecule-glesys-0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule-glesys
-Version: 0.3
+Version: 0.4
 Summary: Molecule GleSYS Plugin :: run molecule tests in GleSYS Cloud
 Home-page: https://github.com/glesys/molecule-driver
 Author: Magnus Johansson
 Author-email: magnus@glesys.se
 Maintainer: Magnus Johansson
 Maintainer-email: magnus@glesys.se
 License: MIT
@@ -31,27 +31,27 @@
 ```
 pip install molecule-glesys
 ```
 
 Create a new role with molecule using this driver:
 
 ```
-molecule init role <role_name> -d glesys
+molecule init role <role_name> -d molecule-glesys
 ```
 
 Configure `<role_name>/molecule/default/molecule.yml` with required parameters.  
 Sample config:
 
 ```yaml
 dependency:
   name: galaxy
   options:
     requirements-file: molecule/default/collections.yml
 driver:
-  name: glesys
+  name: molecule-glesys
   vm_username: molecule
 
 platforms:
   - name: "demo.demo-ubuntu-20-04"
     template: Ubuntu 20.04 LTS (Focal Fossa)
     description: "ubuntu-20-04"
     datacenter: "Falkenberg"
```

### Comparing `molecule-glesys-0.3/README.md` & `molecule-glesys-0.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 ```
 pip install molecule-glesys
 ```
 
 Create a new role with molecule using this driver:
 
 ```
-molecule init role <role_name> -d glesys
+molecule init role <role_name> -d molecule-glesys
 ```
 
 Configure `<role_name>/molecule/default/molecule.yml` with required parameters.  
 Sample config:
 
 ```yaml
 dependency:
   name: galaxy
   options:
     requirements-file: molecule/default/collections.yml
 driver:
-  name: glesys
+  name: molecule-glesys
   vm_username: molecule
 
 platforms:
   - name: "demo.demo-ubuntu-20-04"
     template: Ubuntu 20.04 LTS (Focal Fossa)
     description: "ubuntu-20-04"
     datacenter: "Falkenberg"
```

### Comparing `molecule-glesys-0.3/molecule_glesys/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/create.yml` & `molecule-glesys-0.4/molecule_glesys/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/create.yml`

 * *Files identical despite different names*

### Comparing `molecule-glesys-0.3/molecule_glesys/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/destroy.yml` & `molecule-glesys-0.4/molecule_glesys/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/destroy.yml`

 * *Files identical despite different names*

### Comparing `molecule-glesys-0.3/molecule_glesys/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/handlers/main.yml` & `molecule-glesys-0.4/molecule_glesys/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/handlers/main.yml`

 * *Files identical despite different names*

### Comparing `molecule-glesys-0.3/molecule_glesys/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/molecule.yml` & `molecule-glesys-0.4/molecule_glesys/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/molecule.yml`

 * *Files identical despite different names*

### Comparing `molecule-glesys-0.3/molecule_glesys/driver.py` & `molecule-glesys-0.4/molecule_glesys/driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 LOG = logger.get_logger(__name__)
 
 
 class GleSYS(Driver):
     def __init__(self, config=None):
         super(GleSYS, self).__init__(config)
-        self._name = "glesys"
+        self._name = "molecule-glesys"
 
     @property
     def name(self):
         return self._name
 
     @name.setter
     def name(self, value):
```

### Comparing `molecule-glesys-0.3/molecule_glesys.egg-info/PKG-INFO` & `molecule-glesys-0.4/molecule_glesys.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule-glesys
-Version: 0.3
+Version: 0.4
 Summary: Molecule GleSYS Plugin :: run molecule tests in GleSYS Cloud
 Home-page: https://github.com/glesys/molecule-driver
 Author: Magnus Johansson
 Author-email: magnus@glesys.se
 Maintainer: Magnus Johansson
 Maintainer-email: magnus@glesys.se
 License: MIT
@@ -31,27 +31,27 @@
 ```
 pip install molecule-glesys
 ```
 
 Create a new role with molecule using this driver:
 
 ```
-molecule init role <role_name> -d glesys
+molecule init role <role_name> -d molecule-glesys
 ```
 
 Configure `<role_name>/molecule/default/molecule.yml` with required parameters.  
 Sample config:
 
 ```yaml
 dependency:
   name: galaxy
   options:
     requirements-file: molecule/default/collections.yml
 driver:
-  name: glesys
+  name: molecule-glesys
   vm_username: molecule
 
 platforms:
   - name: "demo.demo-ubuntu-20-04"
     template: Ubuntu 20.04 LTS (Focal Fossa)
     description: "ubuntu-20-04"
     datacenter: "Falkenberg"
```

### Comparing `molecule-glesys-0.3/molecule_glesys.egg-info/SOURCES.txt` & `molecule-glesys-0.4/molecule_glesys.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `molecule-glesys-0.3/setup.cfg` & `molecule-glesys-0.4/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 [options.extras_require]
 test = 
 	molecule[test]
 
 [options.entry_points]
 molecule.driver = 
-	glesys = molecule_glesys.driver:GleSYS
+	molecule-glesys = molecule_glesys.driver:GleSYS
 
 [options.packages.find]
 where = .
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

