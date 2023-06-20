# Comparing `tmp/plexlabexchange-0.8.1.tar.gz` & `tmp/PlexLabExchange-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plexlabexchange-0.8.1.tar", last modified: Mon Jun 19 23:16:58 2023, max compression
+gzip compressed data, was "PlexLabExchange-0.8.2.tar", last modified: Tue Jun 20 01:24:41 2023, max compression
```

## Comparing `plexlabexchange-0.8.1.tar` & `PlexLabExchange-0.8.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 mcmenemy   (501) staff       (20)        0 2023-06-19 23:16:58.966989 plexlabexchange-0.8.1/
--rw-r--r--   0 mcmenemy   (501) staff       (20)      603 2023-06-19 23:16:58.966721 plexlabexchange-0.8.1/PKG-INFO
-drwxr-xr-x   0 mcmenemy   (501) staff       (20)        0 2023-06-19 23:16:58.965281 plexlabexchange-0.8.1/plexlabexchange/
--rw-r--r--   0 mcmenemy   (501) staff       (20)     5241 2023-06-19 21:26:50.000000 plexlabexchange-0.8.1/plexlabexchange/__init__.py
-drwxr-xr-x   0 mcmenemy   (501) staff       (20)        0 2023-06-19 23:16:58.966031 plexlabexchange-0.8.1/plexlabexchange.egg-info/
--rw-r--r--   0 mcmenemy   (501) staff       (20)      603 2023-06-19 23:16:58.000000 plexlabexchange-0.8.1/plexlabexchange.egg-info/PKG-INFO
--rw-r--r--   0 mcmenemy   (501) staff       (20)      230 2023-06-19 23:16:58.000000 plexlabexchange-0.8.1/plexlabexchange.egg-info/SOURCES.txt
--rw-r--r--   0 mcmenemy   (501) staff       (20)        1 2023-06-19 23:16:58.000000 plexlabexchange-0.8.1/plexlabexchange.egg-info/dependency_links.txt
--rw-r--r--   0 mcmenemy   (501) staff       (20)        9 2023-06-19 23:16:58.000000 plexlabexchange-0.8.1/plexlabexchange.egg-info/requires.txt
--rw-r--r--   0 mcmenemy   (501) staff       (20)       16 2023-06-19 23:16:58.000000 plexlabexchange-0.8.1/plexlabexchange.egg-info/top_level.txt
--rw-r--r--   0 mcmenemy   (501) staff       (20)       38 2023-06-19 23:16:58.967050 plexlabexchange-0.8.1/setup.cfg
--rw-r--r--   0 mcmenemy   (501) staff       (20)     4253 2023-06-19 23:16:44.000000 plexlabexchange-0.8.1/setup.py
+drwxr-xr-x   0 mcmenemy   (501) staff       (20)        0 2023-06-20 01:24:41.200735 PlexLabExchange-0.8.2/
+-rw-r--r--   0 mcmenemy   (501) staff       (20)      603 2023-06-20 01:24:41.200567 PlexLabExchange-0.8.2/PKG-INFO
+-rw-r--r--   0 mcmenemy   (501) staff       (20)       38 2023-06-20 01:24:41.200785 PlexLabExchange-0.8.2/setup.cfg
+-rw-r--r--   0 mcmenemy   (501) staff       (20)     4293 2023-06-20 01:24:14.000000 PlexLabExchange-0.8.2/setup.py
+drwxr-xr-x   0 mcmenemy   (501) staff       (20)        0 2023-06-20 01:24:41.199164 PlexLabExchange-0.8.2/src/
+drwxr-xr-x   0 mcmenemy   (501) staff       (20)        0 2023-06-20 01:24:41.199972 PlexLabExchange-0.8.2/src/PlexLabExchange.egg-info/
+-rw-r--r--   0 mcmenemy   (501) staff       (20)      603 2023-06-20 01:24:41.000000 PlexLabExchange-0.8.2/src/PlexLabExchange.egg-info/PKG-INFO
+-rw-r--r--   0 mcmenemy   (501) staff       (20)      243 2023-06-20 01:24:41.000000 PlexLabExchange-0.8.2/src/PlexLabExchange.egg-info/SOURCES.txt
+-rw-r--r--   0 mcmenemy   (501) staff       (20)        1 2023-06-20 01:24:41.000000 PlexLabExchange-0.8.2/src/PlexLabExchange.egg-info/dependency_links.txt
+-rw-r--r--   0 mcmenemy   (501) staff       (20)        9 2023-06-20 01:24:41.000000 PlexLabExchange-0.8.2/src/PlexLabExchange.egg-info/requires.txt
+-rw-r--r--   0 mcmenemy   (501) staff       (20)        5 2023-06-20 01:24:41.000000 PlexLabExchange-0.8.2/src/PlexLabExchange.egg-info/top_level.txt
+drwxr-xr-x   0 mcmenemy   (501) staff       (20)        0 2023-06-20 01:24:41.200183 PlexLabExchange-0.8.2/src/plex/
+-rw-r--r--   0 mcmenemy   (501) staff       (20)     5241 2023-06-19 21:26:50.000000 PlexLabExchange-0.8.2/src/plex/__init__.py
```

### Comparing `plexlabexchange-0.8.1/PKG-INFO` & `PlexLabExchange-0.8.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: plexlabexchange
-Version: 0.8.1
+Name: PlexLabExchange
+Version: 0.8.2
 Summary: A Python interface to the Plex Go CLI.
 Home-page: https://github.com/labdao/plex
 Author: LabDAO
 Author-email: media@labdao.xyz
 License: MIT
 Keywords: plex golang cli wrapper
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `plexlabexchange-0.8.1/plexlabexchange/__init__.py` & `PlexLabExchange-0.8.2/src/plex/__init__.py`

 * *Files identical despite different names*

### Comparing `plexlabexchange-0.8.1/plexlabexchange.egg-info/PKG-INFO` & `PlexLabExchange-0.8.2/src/PlexLabExchange.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: plexlabexchange
-Version: 0.8.1
+Name: PlexLabExchange
+Version: 0.8.2
 Summary: A Python interface to the Plex Go CLI.
 Home-page: https://github.com/labdao/plex
 Author: LabDAO
 Author-email: media@labdao.xyz
 License: MIT
 Keywords: plex golang cli wrapper
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `plexlabexchange-0.8.1/setup.py` & `PlexLabExchange-0.8.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,17 +65,18 @@
             except Exception as e:
                 raise RuntimeError(f"Failed to set the Go binary as executable: {e}")
         else:
             raise RuntimeError(f"The current platform/machine of {system_platform}/{machine} is not supported.")
 
 
 setup(
-    name="plexlabexchange",
-    version="0.8.1",
-    packages=find_packages(),
+    name="PlexLabExchange",
+    version="0.8.2",
+    package_dir={'': 'src'},
+    packages=find_packages(where='src'),
     cmdclass={
         'install': PostInstallCommand,
     },
     install_requires=[
         'requests',
     ],
     author="LabDAO",
```

