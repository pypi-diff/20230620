# Comparing `tmp/seiscat-0.2.tar.gz` & `tmp/seiscat-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seiscat-0.2.tar", last modified: Mon Jun 19 15:28:25 2023, max compression
+gzip compressed data, was "seiscat-0.3.tar", last modified: Tue Jun 20 10:16:53 2023, max compression
```

## Comparing `seiscat-0.2.tar` & `seiscat-0.3.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:28:25.750739 seiscat-0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-19 15:28:14.000000 seiscat-0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-19 15:28:14.000000 seiscat-0.2/CONTRIBUTORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-19 15:28:14.000000 seiscat-0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-19 15:28:14.000000 seiscat-0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-06-19 15:28:25.750739 seiscat-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-19 15:28:14.000000 seiscat-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:28:25.750739 seiscat-0.2/seiscat/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-19 15:28:14.000000 seiscat-0.2/seiscat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-19 15:28:25.750739 seiscat-0.2/seiscat/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:28:25.746739 seiscat-0.2/seiscat/conf/
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-06-19 15:28:14.000000 seiscat-0.2/seiscat/conf/configspec.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:28:25.750739 seiscat-0.2/seiscat/configobj/
--rw-r--r--   0 runner    (1001) docker     (123)    88030 2023-06-19 15:28:14.000000 seiscat-0.2/seiscat/configobj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-19 15:28:14.000000 seiscat-0.2/seiscat/configobj/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    46990 2023-06-19 15:28:14.000000 seiscat-0.2/seiscat/configobj/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-06-19 15:28:14.000000 seiscat-0.2/seiscat/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-06-19 15:28:14.000000 seiscat-0.2/seiscat/fdsnws.py
--rw-r--r--   0 runner    (1001) docker     (123)     7130 2023-06-19 15:28:14.000000 seiscat-0.2/seiscat/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:28:25.750739 seiscat-0.2/seiscat/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-19 15:28:14.000000 seiscat-0.2/seiscat/scripts/seiscat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-06-19 15:28:14.000000 seiscat-0.2/seiscat/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:28:25.746739 seiscat-0.2/seiscat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-06-19 15:28:25.000000 seiscat-0.2/seiscat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-19 15:28:25.000000 seiscat-0.2/seiscat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 15:28:25.000000 seiscat-0.2/seiscat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-19 15:28:25.000000 seiscat-0.2/seiscat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-19 15:28:25.000000 seiscat-0.2/seiscat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-19 15:28:25.000000 seiscat-0.2/seiscat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-19 15:28:25.750739 seiscat-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-19 15:28:14.000000 seiscat-0.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-06-19 15:28:14.000000 seiscat-0.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:16:53.949845 seiscat-0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-20 10:16:46.000000 seiscat-0.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-20 10:16:46.000000 seiscat-0.3/CONTRIBUTORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-20 10:16:46.000000 seiscat-0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-20 10:16:46.000000 seiscat-0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-06-20 10:16:53.949845 seiscat-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-06-20 10:16:46.000000 seiscat-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:16:53.949845 seiscat-0.3/seiscat/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-20 10:16:46.000000 seiscat-0.3/seiscat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-20 10:16:53.949845 seiscat-0.3/seiscat/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:16:53.949845 seiscat-0.3/seiscat/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-06-20 10:16:46.000000 seiscat-0.3/seiscat/conf/configspec.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:16:53.949845 seiscat-0.3/seiscat/configobj/
+-rw-r--r--   0 runner    (1001) docker     (123)    88030 2023-06-20 10:16:46.000000 seiscat-0.3/seiscat/configobj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-20 10:16:46.000000 seiscat-0.3/seiscat/configobj/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46990 2023-06-20 10:16:46.000000 seiscat-0.3/seiscat/configobj/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-06-20 10:16:46.000000 seiscat-0.3/seiscat/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-06-20 10:16:46.000000 seiscat-0.3/seiscat/fdsnws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7138 2023-06-20 10:16:46.000000 seiscat-0.3/seiscat/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-20 10:16:46.000000 seiscat-0.3/seiscat/print.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:16:53.949845 seiscat-0.3/seiscat/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-06-20 10:16:46.000000 seiscat-0.3/seiscat/scripts/seiscat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-06-20 10:16:46.000000 seiscat-0.3/seiscat/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:16:53.949845 seiscat-0.3/seiscat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-06-20 10:16:53.000000 seiscat-0.3/seiscat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-20 10:16:53.000000 seiscat-0.3/seiscat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 10:16:53.000000 seiscat-0.3/seiscat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-20 10:16:53.000000 seiscat-0.3/seiscat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 10:16:53.000000 seiscat-0.3/seiscat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 10:16:53.000000 seiscat-0.3/seiscat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-20 10:16:53.949845 seiscat-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-20 10:16:46.000000 seiscat-0.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-06-20 10:16:46.000000 seiscat-0.3/versioneer.py
```

### Comparing `seiscat-0.2/CHANGELOG.md` & `seiscat-0.3/CHANGELOG.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,17 @@
-# SeisCat
+# SeisCat Changelog
 
 Keep a local seismic catalog.
 
-(c) 2022-2023 Claudio Satriano <satriano@ipgp.fr>
+Copyright (c) 2022-2023 Claudio Satriano <satriano@ipgp.fr>
+
+## v0.3 - 2023-06-20
+
+- New command to print catalog to screen: `seiscat print`
+- Documentation!
 
 ## v0.2 - 2023-06-19
 
 - Fix for plotting the whole world when no limits are given
 - New way of computing zoom level for map tiles
 
 ## v0.1 - 2023-06-19
```

### Comparing `seiscat-0.2/LICENSE.txt` & `seiscat-0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `seiscat-0.2/PKG-INFO` & `seiscat-0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seiscat
-Version: 0.2
+Version: 0.3
 Summary: Keep a local seismic catalog
 Home-page: https://github.com/SeismicSource/SeisCat
 Author: Claudio Satriano
 Author-email: satriano@ipgp.fr
 License: GNU General Public License v3 or later (GPLv3+)
 Platform: OS Independent
 Classifier: Development Status :: 3 - Alpha
@@ -26,33 +26,62 @@
 
 # SeisCat
 
 Keep a local seismic catalog.
 
 [![PyPI-badge]][PyPI-link]
 [![license-badge]][license-link]
+[![docs-badge]][docs-link]
 
 (c) 2022-2023 Claudio Satriano <satriano@ipgp.fr>
 
 ## Overview
 
 SeisCat is a command line tool to keep a local seismic catalog.
 The local catalog can be used as a basis for further analyses.
 
 The seismic catalog is built and updated by querying a FDSNWS event webservice.
 More ways of feeding the catalog will be added in the future.
 
 The local catalog is stored in a SQLite database (single file database).
 
+👇  See below on how to [install](#installation) and
+[get started](#getting-started).
+
+📖 Check out the official documentation [here](https://seiscat.rtfd.io).
+
 ## Getting Started
 
 To get help:
 
     seiscat -h
 
+First thing to do is to generate a sample configuration file:
+
+    seiscat sampleconfig
+
+Then, edit the configuration file and init the database:
+
+    seiscat initdb
+
+To keep the database updated, run on a regular basis:
+
+    seiscat updatedb
+
+(This will use the configuration parameter `recheck_period` to recheck the
+last *n* days or hours).
+
+You can print the catalog to screen:
+
+    seiscat print
+
+Or plot it:
+
+    seiscat plot
+
 ## Installation
 
 ### Installing the latest release
 
 #### Using pip and PyPI (preferred method)
 
 The latest release of SeisCat is available on the
@@ -117,12 +146,31 @@
 
     pip install -e .
 
 You can keep your local SeisCat repository updated by running `git pull`
 from times to times. Thanks to `pip`'s "editable mode", you don't need to
 reinstall SeisCat after each update.
 
+## Getting Help / Reporting Bugs
+
+### 🙏 I need help
+
+Please open an [Issue][Issues].
+
+### 🐞 I found a bug
+
+Please open an [Issue][Issues].
+
+## Contributing
+
+I'm very open to contributions: if you have new ideas, please open an
+[Issue][Issues].
+Don't hesitate sending me pull requests with new features and/or bugfixes!
+
 <!-- Badges and project links -->
 [PyPI-badge]: http://img.shields.io/pypi/v/seiscat.svg
 [PyPI-link]: https://pypi.python.org/pypi/seiscat
 [license-badge]: https://img.shields.io/badge/license-GPLv3-green
 [license-link]: https://www.gnu.org/licenses/gpl-3.0.html
+[docs-badge]: https://readthedocs.org/projects/seiscat/badge/?version=latest
+[docs-link]: https://seiscat.readthedocs.io/en/latest/?badge=latest
+[Issues]: https://github.com/SeismicSource/seiscat/issues
```

### Comparing `seiscat-0.2/README.md` & `seiscat-0.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,61 @@
 # SeisCat
 
 Keep a local seismic catalog.
 
 [![PyPI-badge]][PyPI-link]
 [![license-badge]][license-link]
+[![docs-badge]][docs-link]
 
 (c) 2022-2023 Claudio Satriano <satriano@ipgp.fr>
 
 ## Overview
 
 SeisCat is a command line tool to keep a local seismic catalog.
 The local catalog can be used as a basis for further analyses.
 
 The seismic catalog is built and updated by querying a FDSNWS event webservice.
 More ways of feeding the catalog will be added in the future.
 
 The local catalog is stored in a SQLite database (single file database).
 
+👇  See below on how to [install](#installation) and
+[get started](#getting-started).
+
+📖 Check out the official documentation [here](https://seiscat.rtfd.io).
+
 ## Getting Started
 
 To get help:
 
     seiscat -h
 
+First thing to do is to generate a sample configuration file:
+
+    seiscat sampleconfig
+
+Then, edit the configuration file and init the database:
+
+    seiscat initdb
+
+To keep the database updated, run on a regular basis:
+
+    seiscat updatedb
+
+(This will use the configuration parameter `recheck_period` to recheck the
+last *n* days or hours).
+
+You can print the catalog to screen:
+
+    seiscat print
+
+Or plot it:
+
+    seiscat plot
+
 ## Installation
 
 ### Installing the latest release
 
 #### Using pip and PyPI (preferred method)
 
 The latest release of SeisCat is available on the
@@ -91,12 +120,31 @@
 
     pip install -e .
 
 You can keep your local SeisCat repository updated by running `git pull`
 from times to times. Thanks to `pip`'s "editable mode", you don't need to
 reinstall SeisCat after each update.
 
+## Getting Help / Reporting Bugs
+
+### 🙏 I need help
+
+Please open an [Issue][Issues].
+
+### 🐞 I found a bug
+
+Please open an [Issue][Issues].
+
+## Contributing
+
+I'm very open to contributions: if you have new ideas, please open an
+[Issue][Issues].
+Don't hesitate sending me pull requests with new features and/or bugfixes!
+
 <!-- Badges and project links -->
 [PyPI-badge]: http://img.shields.io/pypi/v/seiscat.svg
 [PyPI-link]: https://pypi.python.org/pypi/seiscat
 [license-badge]: https://img.shields.io/badge/license-GPLv3-green
 [license-link]: https://www.gnu.org/licenses/gpl-3.0.html
+[docs-badge]: https://readthedocs.org/projects/seiscat/badge/?version=latest
+[docs-link]: https://seiscat.readthedocs.io/en/latest/?badge=latest
+[Issues]: https://github.com/SeismicSource/seiscat/issues
```

### Comparing `seiscat-0.2/seiscat/conf/configspec.conf` & `seiscat-0.3/seiscat/conf/configspec.conf`

 * *Files identical despite different names*

### Comparing `seiscat-0.2/seiscat/configobj/__init__.py` & `seiscat-0.3/seiscat/configobj/__init__.py`

 * *Files identical despite different names*

### Comparing `seiscat-0.2/seiscat/configobj/validate.py` & `seiscat-0.3/seiscat/configobj/validate.py`

 * *Files identical despite different names*

### Comparing `seiscat-0.2/seiscat/db.py` & `seiscat-0.3/seiscat/db.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,14 @@
     Set the database version.
 
     :param cursor: database cursor
     """
     cursor.execute('PRAGMA user_version = {v:d}'.format(v=DB_VERSION))
 
 
-
 def check_db_exists(config, initdb):
     """
     Check if database file exists.
 
     :param config: config object
     :param initdb: if True, create new database file
     """
```

### Comparing `seiscat-0.2/seiscat/fdsnws.py` & `seiscat-0.3/seiscat/fdsnws.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf8 -*-
 # SPDX-License-Identifier: GPL-3.0-or-later
 """
-FDNS webservices functions for seiscat.
+FDSN webservices functions for seiscat.
 
 :copyright:
     2022-2023 Claudio Satriano <satriano@ipgp.fr>
 :license:
     GNU General Public License v3.0 or later
     (https://www.gnu.org/licenses/gpl-3.0-standalone.html)
 """
```

### Comparing `seiscat-0.2/seiscat/plot.py` & `seiscat-0.3/seiscat/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,18 +30,18 @@
     lat_max = config.get(f'lat_max{suffix}', None)
     lon_min = config.get(f'lon_min{suffix}', None)
     lon_max = config.get(f'lon_max{suffix}', None)
     lat0 = config.get(f'lat0{suffix}', None)
     lon0 = config.get(f'lon0{suffix}', None)
     radius_max = config.get(f'radius_max{suffix}', None)
     if None not in (lat0, lon0, radius_max):
-        lat_min = lat0 - radius_max*np.sqrt(2)
-        lat_max = lat0 + radius_max*np.sqrt(2)
-        lon_min = lon0 - radius_max*np.sqrt(2)
-        lon_max = lon0 + radius_max*np.sqrt(2)
+        lat_min = lat0 - radius_max * np.sqrt(2)
+        lat_max = lat0 + radius_max * np.sqrt(2)
+        lon_min = lon0 - radius_max * np.sqrt(2)
+        lon_max = lon0 + radius_max * np.sqrt(2)
         return lon_min, lon_max, lat_min, lat_max
     if None not in (lat_min, lat_max, lon_min, lon_max):
         return lon_min, lon_max, lat_min, lat_max
     return None
 
 
 def _get_map_extent(config):
```

### Comparing `seiscat-0.2/seiscat/scripts/seiscat.py` & `seiscat-0.3/seiscat/scripts/seiscat.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,24 +11,27 @@
     (https://www.gnu.org/licenses/gpl-3.0-standalone.html)
 """
 import sys
 import argparse
 from .._version import get_versions
 from ..fdsnws import open_fdsn_connection, query_events
 from ..db import check_db_exists, write_catalog_to_db
+from ..print import print_catalog
 from ..plot import plot_catalog_map
 from ..utils import parse_configspec, read_config,  write_sample_config
 
 
 def parse_arguments():
     """Parse command line arguments."""
-    parser = argparse.ArgumentParser(description='Run seiscat.')
+    parser = argparse.ArgumentParser(
+        description='Keep a local seismic catalog.')
     subparser = parser.add_subparsers(dest='action')
     subparser.add_parser('initdb', help='initialize database')
     subparser.add_parser('updatedb', help='update database')
+    subparser.add_parser('print', help='print catalog')
     subparser.add_parser('plot', help='plot catalog map')
     subparser.add_parser('sampleconfig', help='write sample config file')
     parser.add_argument(
         '-c',
         '--configfile',
         type=str,
         default='seiscat.conf',
@@ -69,14 +72,16 @@
         sys.exit(0)
     config = read_config(args.configfile, configspec)
     client = open_fdsn_connection(config)
     if args.action == 'initdb':
         download_and_store(client, config, initdb=True)
     elif args.action == 'updatedb':
         download_and_store(client, config, initdb=False)
+    elif args.action == 'print':
+        print_catalog(config)
     elif args.action == 'plot':
         plot_catalog_map(config)
 
 
 def main():
     """Main function. Catch KeyboardInterrupt."""
     try:
```

### Comparing `seiscat-0.2/seiscat/utils.py` & `seiscat-0.3/seiscat/utils.py`

 * *Files identical despite different names*

### Comparing `seiscat-0.2/seiscat.egg-info/PKG-INFO` & `seiscat-0.3/seiscat.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seiscat
-Version: 0.2
+Version: 0.3
 Summary: Keep a local seismic catalog
 Home-page: https://github.com/SeismicSource/SeisCat
 Author: Claudio Satriano
 Author-email: satriano@ipgp.fr
 License: GNU General Public License v3 or later (GPLv3+)
 Platform: OS Independent
 Classifier: Development Status :: 3 - Alpha
@@ -26,33 +26,62 @@
 
 # SeisCat
 
 Keep a local seismic catalog.
 
 [![PyPI-badge]][PyPI-link]
 [![license-badge]][license-link]
+[![docs-badge]][docs-link]
 
 (c) 2022-2023 Claudio Satriano <satriano@ipgp.fr>
 
 ## Overview
 
 SeisCat is a command line tool to keep a local seismic catalog.
 The local catalog can be used as a basis for further analyses.
 
 The seismic catalog is built and updated by querying a FDSNWS event webservice.
 More ways of feeding the catalog will be added in the future.
 
 The local catalog is stored in a SQLite database (single file database).
 
+👇  See below on how to [install](#installation) and
+[get started](#getting-started).
+
+📖 Check out the official documentation [here](https://seiscat.rtfd.io).
+
 ## Getting Started
 
 To get help:
 
     seiscat -h
 
+First thing to do is to generate a sample configuration file:
+
+    seiscat sampleconfig
+
+Then, edit the configuration file and init the database:
+
+    seiscat initdb
+
+To keep the database updated, run on a regular basis:
+
+    seiscat updatedb
+
+(This will use the configuration parameter `recheck_period` to recheck the
+last *n* days or hours).
+
+You can print the catalog to screen:
+
+    seiscat print
+
+Or plot it:
+
+    seiscat plot
+
 ## Installation
 
 ### Installing the latest release
 
 #### Using pip and PyPI (preferred method)
 
 The latest release of SeisCat is available on the
@@ -117,12 +146,31 @@
 
     pip install -e .
 
 You can keep your local SeisCat repository updated by running `git pull`
 from times to times. Thanks to `pip`'s "editable mode", you don't need to
 reinstall SeisCat after each update.
 
+## Getting Help / Reporting Bugs
+
+### 🙏 I need help
+
+Please open an [Issue][Issues].
+
+### 🐞 I found a bug
+
+Please open an [Issue][Issues].
+
+## Contributing
+
+I'm very open to contributions: if you have new ideas, please open an
+[Issue][Issues].
+Don't hesitate sending me pull requests with new features and/or bugfixes!
+
 <!-- Badges and project links -->
 [PyPI-badge]: http://img.shields.io/pypi/v/seiscat.svg
 [PyPI-link]: https://pypi.python.org/pypi/seiscat
 [license-badge]: https://img.shields.io/badge/license-GPLv3-green
 [license-link]: https://www.gnu.org/licenses/gpl-3.0.html
+[docs-badge]: https://readthedocs.org/projects/seiscat/badge/?version=latest
+[docs-link]: https://seiscat.readthedocs.io/en/latest/?badge=latest
+[Issues]: https://github.com/SeismicSource/seiscat/issues
```

### Comparing `seiscat-0.2/seiscat.egg-info/SOURCES.txt` & `seiscat-0.3/seiscat.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 setup.py
 versioneer.py
 seiscat/__init__.py
 seiscat/_version.py
 seiscat/db.py
 seiscat/fdsnws.py
 seiscat/plot.py
+seiscat/print.py
 seiscat/utils.py
 seiscat.egg-info/PKG-INFO
 seiscat.egg-info/SOURCES.txt
 seiscat.egg-info/dependency_links.txt
 seiscat.egg-info/entry_points.txt
 seiscat.egg-info/requires.txt
 seiscat.egg-info/top_level.txt
```

### Comparing `seiscat-0.2/setup.py` & `seiscat-0.3/setup.py`

 * *Files identical despite different names*

### Comparing `seiscat-0.2/versioneer.py` & `seiscat-0.3/versioneer.py`

 * *Files identical despite different names*

