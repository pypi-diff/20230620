# Comparing `tmp/seiscat-0.3.tar.gz` & `tmp/seiscat-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seiscat-0.3.tar", last modified: Tue Jun 20 10:16:53 2023, max compression
+gzip compressed data, was "seiscat-0.4.tar", last modified: Tue Jun 20 15:25:37 2023, max compression
```

## Comparing `seiscat-0.3.tar` & `seiscat-0.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:16:53.949845 seiscat-0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-20 10:16:46.000000 seiscat-0.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-20 10:16:46.000000 seiscat-0.3/CONTRIBUTORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-20 10:16:46.000000 seiscat-0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-20 10:16:46.000000 seiscat-0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-06-20 10:16:53.949845 seiscat-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-06-20 10:16:46.000000 seiscat-0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:16:53.949845 seiscat-0.3/seiscat/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-20 10:16:46.000000 seiscat-0.3/seiscat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-20 10:16:53.949845 seiscat-0.3/seiscat/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:16:53.949845 seiscat-0.3/seiscat/conf/
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-06-20 10:16:46.000000 seiscat-0.3/seiscat/conf/configspec.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:16:53.949845 seiscat-0.3/seiscat/configobj/
--rw-r--r--   0 runner    (1001) docker     (123)    88030 2023-06-20 10:16:46.000000 seiscat-0.3/seiscat/configobj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-20 10:16:46.000000 seiscat-0.3/seiscat/configobj/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    46990 2023-06-20 10:16:46.000000 seiscat-0.3/seiscat/configobj/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-06-20 10:16:46.000000 seiscat-0.3/seiscat/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-06-20 10:16:46.000000 seiscat-0.3/seiscat/fdsnws.py
--rw-r--r--   0 runner    (1001) docker     (123)     7138 2023-06-20 10:16:46.000000 seiscat-0.3/seiscat/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-20 10:16:46.000000 seiscat-0.3/seiscat/print.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:16:53.949845 seiscat-0.3/seiscat/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-06-20 10:16:46.000000 seiscat-0.3/seiscat/scripts/seiscat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-06-20 10:16:46.000000 seiscat-0.3/seiscat/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:16:53.949845 seiscat-0.3/seiscat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-06-20 10:16:53.000000 seiscat-0.3/seiscat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-20 10:16:53.000000 seiscat-0.3/seiscat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 10:16:53.000000 seiscat-0.3/seiscat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-20 10:16:53.000000 seiscat-0.3/seiscat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 10:16:53.000000 seiscat-0.3/seiscat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 10:16:53.000000 seiscat-0.3/seiscat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-20 10:16:53.949845 seiscat-0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-20 10:16:46.000000 seiscat-0.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-06-20 10:16:46.000000 seiscat-0.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:25:37.510487 seiscat-0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-20 15:25:29.000000 seiscat-0.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-20 15:25:29.000000 seiscat-0.4/CONTRIBUTORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-20 15:25:29.000000 seiscat-0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-20 15:25:29.000000 seiscat-0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-06-20 15:25:37.510487 seiscat-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-06-20 15:25:29.000000 seiscat-0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:25:37.510487 seiscat-0.4/seiscat/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-20 15:25:29.000000 seiscat-0.4/seiscat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-20 15:25:37.510487 seiscat-0.4/seiscat/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:25:37.510487 seiscat-0.4/seiscat/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-06-20 15:25:29.000000 seiscat-0.4/seiscat/conf/configspec.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:25:37.510487 seiscat-0.4/seiscat/configobj/
+-rw-r--r--   0 runner    (1001) docker     (123)    88030 2023-06-20 15:25:29.000000 seiscat-0.4/seiscat/configobj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-20 15:25:29.000000 seiscat-0.4/seiscat/configobj/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46990 2023-06-20 15:25:29.000000 seiscat-0.4/seiscat/configobj/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-06-20 15:25:29.000000 seiscat-0.4/seiscat/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-06-20 15:25:29.000000 seiscat-0.4/seiscat/fdsnws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-06-20 15:25:29.000000 seiscat-0.4/seiscat/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-20 15:25:29.000000 seiscat-0.4/seiscat/print.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:25:37.510487 seiscat-0.4/seiscat/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-06-20 15:25:29.000000 seiscat-0.4/seiscat/scripts/seiscat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-06-20 15:25:29.000000 seiscat-0.4/seiscat/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:25:37.510487 seiscat-0.4/seiscat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-06-20 15:25:37.000000 seiscat-0.4/seiscat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-20 15:25:37.000000 seiscat-0.4/seiscat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:25:37.000000 seiscat-0.4/seiscat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-20 15:25:37.000000 seiscat-0.4/seiscat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-20 15:25:37.000000 seiscat-0.4/seiscat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 15:25:37.000000 seiscat-0.4/seiscat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-20 15:25:37.510487 seiscat-0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-20 15:25:29.000000 seiscat-0.4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-06-20 15:25:29.000000 seiscat-0.4/versioneer.py
```

### Comparing `seiscat-0.3/CHANGELOG.md` & `seiscat-0.4/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 # SeisCat Changelog
 
 Keep a local seismic catalog.
 
 Copyright (c) 2022-2023 Claudio Satriano <satriano@ipgp.fr>
 
+## v0.4 - 2023-06-20
+
+- Command line autocompletion, thanks to argcomplete
+- Show event depth in plot annotation
+- `--scale` option for `seiscat plot`
+- Correctly parse evids from USGS and ISC
+- Exit gracefully if database file is missing
+- Fix printing of `None` values
+
 ## v0.3 - 2023-06-20
 
 - New command to print catalog to screen: `seiscat print`
 - Documentation!
 
 ## v0.2 - 2023-06-19
```

### Comparing `seiscat-0.3/LICENSE.txt` & `seiscat-0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `seiscat-0.3/PKG-INFO` & `seiscat-0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,16 @@
-Metadata-Version: 2.1
-Name: seiscat
-Version: 0.3
-Summary: Keep a local seismic catalog
-Home-page: https://github.com/SeismicSource/SeisCat
-Author: Claudio Satriano
-Author-email: satriano@ipgp.fr
-License: GNU General Public License v3 or later (GPLv3+)
-Platform: OS Independent
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # SeisCat
 
 Keep a local seismic catalog.
 
 [![PyPI-badge]][PyPI-link]
 [![license-badge]][license-link]
 [![docs-badge]][docs-link]
 
-(c) 2022-2023 Claudio Satriano <satriano@ipgp.fr>
+Copyright (c) 2022-2023 Claudio Satriano <satriano@ipgp.fr>
 
 ## Overview
 
 SeisCat is a command line tool to keep a local seismic catalog.
 The local catalog can be used as a basis for further analyses.
 
 The seismic catalog is built and updated by querying a FDSNWS event webservice.
@@ -74,14 +48,26 @@
 
     seiscat print
 
 Or plot it:
 
     seiscat plot
 
+Each of the above commands can have its own options.
+As an example, to discover the options for the `plot` command, try:
+
+    seiscat plot -h
+
+SeisCat supports command line tab completion for arguments, thanks to
+[argcomplete](https://kislyuk.github.io/argcomplete/).
+To enable command line tab completion, add the following line to your `.bashrc`
+or `.zshrc`:
+
+    eval "$(register-python-argcomplete seiscat)"
+
 ## Installation
 
 ### Installing the latest release
 
 #### Using pip and PyPI (preferred method)
 
 The latest release of SeisCat is available on the
```

### Comparing `seiscat-0.3/seiscat/conf/configspec.conf` & `seiscat-0.4/seiscat/conf/configspec.conf`

 * *Files identical despite different names*

### Comparing `seiscat-0.3/seiscat/configobj/__init__.py` & `seiscat-0.4/seiscat/configobj/__init__.py`

 * *Files identical despite different names*

### Comparing `seiscat-0.3/seiscat/configobj/validate.py` & `seiscat-0.4/seiscat/configobj/validate.py`

 * *Files identical despite different names*

### Comparing `seiscat-0.3/seiscat/db.py` & `seiscat-0.4/seiscat/db.py`

 * *Files 12% similar despite different names*

```diff
@@ -49,34 +49,56 @@
 def check_db_exists(config, initdb):
     """
     Check if database file exists.
 
     :param config: config object
     :param initdb: if True, create new database file
     """
-    if initdb and os.path.exists(config['db_file']):
+    db_file = config.get('db_file', None)
+    if db_file is None:
+        err_exit('db_file not set in config file')
+    if initdb and os.path.exists(db_file):
         ans = input(
-            f'"{config["db_file"]}" already exists. '
+            f'"{db_file}" already exists. '
             'Do you want to overwrite it? [y/N] '
         )
         if ans not in ['y', 'Y']:
             err_exit('Database file already exists. Exiting.')
         else:
             os.rename(
-                config['db_file'], f'{config["db_file"]}.bak')
+                db_file, f'{db_file}.bak')
             print(
-                f'Backup of "{config["db_file"]}" saved to '
-                f'"{config["db_file"]}.bak"')
-    if not initdb and not os.path.exists(config['db_file']):
+                f'Backup of "{db_file}" saved to '
+                f'"{db_file}.bak"')
+    if not initdb and not os.path.exists(db_file):
         err_exit(
-            f'Database file "{config["db_file"]}" does not exist.\n'
+            f'Database file "{db_file}" does not exist.\n'
             'Run "seiscat initdb" first.'
         )
 
 
+def _get_evid(resource_id):
+    """
+    Get evid from resource_id.
+
+    :param resource_id: resource_id string
+    :returns: evid string
+    """
+    evid = resource_id
+    if '/' in evid:
+        evid = resource_id.split('/')[-1]
+    if '?' in evid:
+        evid = resource_id.split('?')[-1]
+    if '&' in evid:
+        evid = evid.split('&')[0]
+    if '=' in evid:
+        evid = evid.split('=')[-1]
+    return evid
+
+
 def write_catalog_to_db(cat, config, initdb):
     """
     Write catalog to database.
 
     :param cat: obspy Catalog object
     :param config: config object
     :param initdb: if True, create new database file
@@ -104,15 +126,15 @@
     fields.extend(
         f'{name} {dbtype}' for name, dbtype
         in zip(extra_field_names, extra_field_types))
     # create table if it doesn't exist
     c.execute(f'CREATE TABLE IF NOT EXISTS events ({", ".join(fields)})')
     events_written = 0
     for ev in cat:
-        evid = str(ev.resource_id.id).split('/')[-1]
+        evid = _get_evid(str(ev.resource_id.id))
         orig = ev.preferred_origin() or ev.origins[0]
         time = str(orig.time)
         lat = orig.latitude
         lon = orig.longitude
         dep = orig.depth / 1e3  # km
         magntiude = ev.preferred_magnitude() or ev.magnitudes[0]
         mag = magntiude.mag
```

### Comparing `seiscat-0.3/seiscat/fdsnws.py` & `seiscat-0.4/seiscat/fdsnws.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     GNU General Public License v3.0 or later
     (https://www.gnu.org/licenses/gpl-3.0-standalone.html)
 """
 from datetime import timedelta
 from obspy import UTCDateTime
 from obspy import Catalog
 from obspy.clients.fdsn import Client
+from obspy.clients.fdsn.header import FDSNNoDataException
 from .utils import err_exit
 
 
 def open_fdsn_connection(config):
     """
     Open FDSN connection. Return a FDSN client object.
 
@@ -58,68 +59,101 @@
         return timedelta(minutes=value)
     elif unit == 'second':
         return timedelta(seconds=value)
     else:
         raise ValueError(f'Invalid time unit: {unit}')
 
 
+class InvalidQuery(Exception):
+    """Invalid query exception."""
+    pass
+
+
+class QueryArgs(object):
+    """Build query arguments for FDSN client."""
+    def __init__(self, config, suffix, first_query):
+        """
+        Initialize query arguments.
+
+        :param config: config object
+        :param suffix: suffix to be added to the config keys
+        :param first_query: True if this is the first query
+        """
+        query_keys = [
+            'start_time', 'end_time', 'recheck_period',
+            'lat_min', 'lat_max', 'lon_min', 'lon_max',
+            'lat0', 'lon0', 'radius_min', 'radius_max',
+            'depth_min', 'depth_max',
+            'mag_min', 'mag_max',
+            'event_type', 'event_type_exclude'
+        ]
+        if suffix:
+            query_keys = [k + suffix for k in query_keys]
+        try:
+            if all(config[k] is None for k in query_keys):
+                raise InvalidQuery(
+                    'All query parameters are None. Please set at least one.')
+        except KeyError as e:
+            raise InvalidQuery('Not all query parameters are set.') from e
+        self.starttime = _to_utc_datetime(config[f'start_time{suffix}'])
+        self.endtime = _to_utc_datetime(config[f'end_time{suffix}'])
+        recheck_period = _parse_time_interval(
+            config[f'recheck_period{suffix}'])
+        if not first_query and self.endtime is None and recheck_period:
+            self.starttime = max(
+                self.starttime, UTCDateTime() - recheck_period)
+        self.minlatitude = config[f'lat_min{suffix}']
+        self.maxlatitude = config[f'lat_max{suffix}']
+        self.minlongitude = config[f'lon_min{suffix}']
+        self.maxlongitude = config[f'lon_max{suffix}']
+        self.latitude = config[f'lat0{suffix}']
+        self.longitude = config[f'lon0{suffix}']
+        self.minradius = config[f'radius_min{suffix}']
+        self.maxradius = config[f'radius_max{suffix}']
+        self.mindepth = config[f'depth_min{suffix}']
+        self.maxdepth = config[f'depth_max{suffix}']
+        self.minmagnitude = config[f'mag_min{suffix}']
+        self.maxmagnitude = config[f'mag_max{suffix}']
+
+    def get_query(self):
+        """
+        Return query arguments as a dictionary.
+
+        :returns: dictionary of query arguments
+        """
+        return {
+            'starttime': self.starttime, 'endtime': self.endtime,
+            'minlatitude': self.minlatitude, 'maxlatitude': self.maxlatitude,
+            'minlongitude': self.minlongitude,
+            'maxlongitude': self.maxlongitude,
+            'latitude': self.latitude, 'longitude': self.longitude,
+            'minradius': self.minradius, 'maxradius': self.maxradius,
+            'mindepth': self.mindepth, 'maxdepth': self.maxdepth,
+            'minmagnitude': self.minmagnitude,
+            'maxmagnitude': self.maxmagnitude,
+        }
+
+
 def _query_box_or_circle(client, config, suffix=None, first_query=True):
     """
     Query events from FDSN client based on box or circle criteria in config.
 
     :param client: FDSN client object
     :param config: config object
     :param suffix: suffix to be added to the config keys
     :param first_query: True if this is the first query
     :returns: obspy Catalog object
     """
-    query_keys = [
-        'start_time', 'end_time', 'recheck_period',
-        'lat_min', 'lat_max', 'lon_min', 'lon_max',
-        'lat0', 'lon0', 'radius_min', 'radius_max',
-        'depth_min', 'depth_max',
-        'mag_min', 'mag_max',
-        'event_type', 'event_type_exclude'
-    ]
     suffix = '' if suffix is None else suffix
-    if suffix:
-        query_keys = [k + suffix for k in query_keys]
-        try:
-            if all(config[k] is None for k in query_keys):
-                return Catalog()
-        except KeyError:
-            return Catalog()
-    if all(config[k] is None for k in query_keys):
-        err_exit('All query parameters are None. Please set at least one.')
-    start_time = _to_utc_datetime(config[f'start_time{suffix}'])
-    end_time = _to_utc_datetime(config[f'end_time{suffix}'])
-    recheck_period = _parse_time_interval(config[f'recheck_period{suffix}'])
-    if not first_query and end_time is None and recheck_period:
-        start_time = max(start_time, UTCDateTime() - recheck_period)
-    minlatitude = config[f'lat_min{suffix}']
-    maxlatitude = config[f'lat_max{suffix}']
-    minlongitude = config[f'lon_min{suffix}']
-    maxlongitude = config[f'lon_max{suffix}']
-    latitude = config[f'lat0{suffix}']
-    longitude = config[f'lon0{suffix}']
-    minradius = config[f'radius_min{suffix}']
-    maxradius = config[f'radius_max{suffix}']
-    mindepth = config[f'depth_min{suffix}']
-    maxdepth = config[f'depth_max{suffix}']
-    minmagnitude = config[f'mag_min{suffix}']
-    maxmagnitude = config[f'mag_max{suffix}']
-    cat = client.get_events(
-        starttime=start_time, endtime=end_time,
-        minlatitude=minlatitude, maxlatitude=maxlatitude,
-        minlongitude=minlongitude, maxlongitude=maxlongitude,
-        latitude=latitude, longitude=longitude,
-        minradius=minradius, maxradius=maxradius,
-        mindepth=mindepth, maxdepth=maxdepth,
-        minmagnitude=minmagnitude, maxmagnitude=maxmagnitude,
-    )
+    query_args = QueryArgs(config, suffix, first_query)
+    kwargs = query_args.get_query()
+    try:
+        cat = client.get_events(**kwargs)
+    except FDSNNoDataException:
+        cat = Catalog()
     # filter in included event types
     event_type = config[f'event_type{suffix}']
     if event_type:
         cat = Catalog([
             ev for ev in cat
             if ev.event_type in event_type
         ])
@@ -138,20 +172,26 @@
     Query events from FDSN client based on criteria in config.
 
     :param client: FDSN client object
     :param config: config object
     :param first_query: True if this is the first query
     :returns: obspy Catalog object
     """
-    print('Querying events from FDSN server...')
-    cat = _query_box_or_circle(client, config, first_query=first_query)
+    print(f'Querying events from FDSN server "{config["fdsn_event_url"]}"...')
+    try:
+        cat = _query_box_or_circle(client, config, first_query=first_query)
+    except Exception as e:
+        err_exit(e)
     # see if there are additional queries to be done
     n = 1
     while True:
-        _cat = _query_box_or_circle(
-            client, config, suffix=f'_{n}', first_query=first_query)
-        if not _cat:
+        try:
+            _cat = _query_box_or_circle(
+                client, config, suffix=f'_{n}', first_query=first_query)
+        except InvalidQuery:
             break
+        except Exception as e:
+            err_exit(e)
         cat += _cat
         n += 1
     print(f'Found {len(cat)} events.')
     return cat
```

### Comparing `seiscat-0.3/seiscat/plot.py` & `seiscat-0.4/seiscat/plot.py`

 * *Files 8% similar despite different names*

```diff
@@ -97,15 +97,22 @@
 def _read_event_db(config):
     """
     Read event database. Return a list of events.
 
     :param config: config object
     :returns: list of events, each event is a dictionary
     """
-    conn = sqlite3.connect(config['db_file'])
+    db_file = config.get('db_file', None)
+    if db_file is None:
+        err_exit('db_file not set in config file')
+    try:
+        open(db_file, 'r')
+    except FileNotFoundError:
+        err_exit(f'Database file "{db_file}" not found.')
+    conn = sqlite3.connect(db_file)
     c = conn.cursor()
     # read field names
     c.execute('PRAGMA table_info(events)')
     fields = c.fetchall()
     # read events
     c.execute('SELECT * FROM events')
     events = c.fetchall()
@@ -115,31 +122,34 @@
     for event in events:
         event_dict = {field[1]: event[i] for i, field in enumerate(fields)}
         event_dict['time'] = UTCDateTime(event_dict['time'])
         events_list.append(event_dict)
     return events_list
 
 
-def _plot_events(events, ax):
+def _plot_events(events, scale, ax):
     """
     Plot events on a map.
 
     :param events: list of events, each event is a dictionary
+    :param scale: scale for event markers
     :param ax: matplotlib axes object
     """
     import cartopy.crs as ccrs
+    marker_scale = scale / 10. * 2
     ev_attributes = [
-        (e['evid'], e['time'], e['lon'], e['lat'], e['mag'],
-         np.exp(e['mag']) * 2)
+        (e['evid'], e['time'], e['lon'], e['lat'], e['dep'],
+         e['mag'], np.exp(e['mag']) * marker_scale)
         for e in events
     ]
     markers = []
-    for evid, time, lon, lat, mag, size in ev_attributes:
+    for evid, time, lon, lat, dep, mag, size in ev_attributes:
         marker_label = (
-            f'{evid} M{mag:.1f}\n{time.strftime("%Y-%m-%d %H:%M:%S")}')
+            f'{evid} M{mag:.1f} {dep:.1f} km\n'
+            f'{time.strftime("%Y-%m-%d %H:%M:%S")}')
         marker = ax.scatter(
             lon, lat,
             s=size,
             facecolor='red', edgecolor='black',
             label=marker_label,
             zorder=10,
             transform=ccrs.PlateCarree(),
@@ -206,15 +216,15 @@
     g_kwargs = dict(draw_labels=True, dms=True, x_inline=False, y_inline=False)
     ax.gridlines(**g_kwargs)
 
     def redraw_gridlines(ax):
         ax.gridlines(**g_kwargs)
     ax.callbacks.connect('xlim_changed', lambda ax: redraw_gridlines(ax))
     events = _read_event_db(config)
-    _plot_events(events, ax)
+    _plot_events(events, config['args'].scale, ax)
     nevents = len(events)
     tmin = min(event['time'] for event in events)
     tmax = max(event['time'] for event in events)
     tmin = tmin.strftime('%Y-%m-%dT%H:%M:%S')
     tmax = tmax.strftime('%Y-%m-%dT%H:%M:%S')
     mag_min = min(event['mag'] for event in events)
     mag_max = max(event['mag'] for event in events)
```

### Comparing `seiscat-0.3/seiscat/print.py` & `seiscat-0.4/seiscat/print.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,18 @@
     Pretty-print the catalog as a table.
 
     :param config: config object
     """
     db_file = config.get('db_file', None)
     if db_file is None:
         err_exit('db_file not set in config file')
+    try:
+        open(db_file, 'r')
+    except FileNotFoundError:
+        err_exit(f'Database file "{db_file}" not found.')
     conn = sqlite3.connect(db_file)
     c = conn.cursor()
     # get fields
     c.execute('PRAGMA table_info(events)')
     fields = c.fetchall()
     c.execute('SELECT * FROM events')
     rows = c.fetchall()
@@ -40,10 +44,11 @@
     # print header
     for i, f in enumerate(fields):
         print(f'{f[1]:{max_len[i]}}', end=' ')
     print()
     # print rows
     for row in rows:
         for i, val in enumerate(row):
+            val = 'None' if val is None else val
             print(f'{val:{max_len[i]}}', end=' ')
         print()
     conn.close()
```

### Comparing `seiscat-0.3/seiscat/scripts/seiscat.py` & `seiscat-0.4/seiscat/scripts/seiscat.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,81 +8,91 @@
     2022-2023 Claudio Satriano <satriano@ipgp.fr>
 :license:
     GNU General Public License v3.0 or later
     (https://www.gnu.org/licenses/gpl-3.0-standalone.html)
 """
 import sys
 import argparse
+import argcomplete
 from .._version import get_versions
-from ..fdsnws import open_fdsn_connection, query_events
-from ..db import check_db_exists, write_catalog_to_db
-from ..print import print_catalog
-from ..plot import plot_catalog_map
-from ..utils import parse_configspec, read_config,  write_sample_config
+# NOTE: most modules are lazy-imported to speed up startup time
 
 
 def parse_arguments():
     """Parse command line arguments."""
     parser = argparse.ArgumentParser(
         description='Keep a local seismic catalog.')
     subparser = parser.add_subparsers(dest='action')
     subparser.add_parser('initdb', help='initialize database')
     subparser.add_parser('updatedb', help='update database')
     subparser.add_parser('print', help='print catalog')
-    subparser.add_parser('plot', help='plot catalog map')
+    plot_parser = subparser.add_parser('plot', help='plot catalog map')
+    plot_parser.add_argument(
+        '-s',
+        '--scale',
+        type=float,
+        default=10,
+        help='scale factor for marker size (default: %(default)s)'
+    )
     subparser.add_parser('sampleconfig', help='write sample config file')
     parser.add_argument(
         '-c',
         '--configfile',
         type=str,
         default='seiscat.conf',
         help='config file for data sources and processing params'
     )
     parser.add_argument(
         '-v',
         '--version',
         action='version',
         version=f"%(prog)s {get_versions()['version']}",
     )
+    argcomplete.autocomplete(parser)
     args = parser.parse_args()
     if args.action is None:
         parser.print_help()
         sys.exit(0)
     return args
 
 
-def download_and_store(client, config, initdb):
+def download_and_store(config, initdb):
     """
     Download events and store them in the database.
 
-    :param client: FDSN client
     :param config: config object
     :param initdb: if True, create new database file
     """
+    from ..db import check_db_exists, write_catalog_to_db
+    from ..fdsnws import open_fdsn_connection, query_events
     check_db_exists(config, initdb)
+    client = open_fdsn_connection(config)
     cat = query_events(client, config, first_query=initdb)
     write_catalog_to_db(cat, config, initdb)
 
 
 def run():
     """Run seiscat."""
     args = parse_arguments()
+    from ..utils import parse_configspec, read_config,  write_sample_config
     configspec = parse_configspec()
     if args.action == 'sampleconfig':
         write_sample_config(configspec, 'seiscat')
         sys.exit(0)
     config = read_config(args.configfile, configspec)
-    client = open_fdsn_connection(config)
+    config['args'] = args
     if args.action == 'initdb':
-        download_and_store(client, config, initdb=True)
+        download_and_store(config, initdb=True)
     elif args.action == 'updatedb':
-        download_and_store(client, config, initdb=False)
+        download_and_store(config, initdb=False)
     elif args.action == 'print':
+        from ..print import print_catalog
         print_catalog(config)
     elif args.action == 'plot':
+        from ..plot import plot_catalog_map
         plot_catalog_map(config)
 
 
 def main():
     """Main function. Catch KeyboardInterrupt."""
     try:
         run()
```

### Comparing `seiscat-0.3/seiscat/utils.py` & `seiscat-0.4/seiscat/utils.py`

 * *Files identical despite different names*

### Comparing `seiscat-0.3/seiscat.egg-info/PKG-INFO` & `seiscat-0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: seiscat
-Version: 0.3
+Version: 0.4
 Summary: Keep a local seismic catalog
-Home-page: https://github.com/SeismicSource/SeisCat
+Home-page: https://seiscat.seismicsource.org
 Author: Claudio Satriano
 Author-email: satriano@ipgp.fr
 License: GNU General Public License v3 or later (GPLv3+)
+Project-URL: Homepage, https://seiscat.seismicsource.org
+Project-URL: Source, https://github.com/SeismicSource/seiscat
+Project-URL: Documentation, https://seiscat.readthedocs.io
 Platform: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -28,15 +31,15 @@
 
 Keep a local seismic catalog.
 
 [![PyPI-badge]][PyPI-link]
 [![license-badge]][license-link]
 [![docs-badge]][docs-link]
 
-(c) 2022-2023 Claudio Satriano <satriano@ipgp.fr>
+Copyright (c) 2022-2023 Claudio Satriano <satriano@ipgp.fr>
 
 ## Overview
 
 SeisCat is a command line tool to keep a local seismic catalog.
 The local catalog can be used as a basis for further analyses.
 
 The seismic catalog is built and updated by querying a FDSNWS event webservice.
@@ -74,14 +77,26 @@
 
     seiscat print
 
 Or plot it:
 
     seiscat plot
 
+Each of the above commands can have its own options.
+As an example, to discover the options for the `plot` command, try:
+
+    seiscat plot -h
+
+SeisCat supports command line tab completion for arguments, thanks to
+[argcomplete](https://kislyuk.github.io/argcomplete/).
+To enable command line tab completion, add the following line to your `.bashrc`
+or `.zshrc`:
+
+    eval "$(register-python-argcomplete seiscat)"
+
 ## Installation
 
 ### Installing the latest release
 
 #### Using pip and PyPI (preferred method)
 
 The latest release of SeisCat is available on the
```

### Comparing `seiscat-0.3/seiscat.egg-info/SOURCES.txt` & `seiscat-0.4/seiscat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seiscat-0.3/setup.py` & `seiscat-0.4/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,30 +2,36 @@
 """setup.py: setuptools control."""
 from setuptools import setup
 import versioneer
 
 with open('README.md', 'rb') as f:
     long_descr = f.read().decode('utf-8')
 
+project_urls = {
+    'Homepage': 'https://seiscat.seismicsource.org',
+    'Source': 'https://github.com/SeismicSource/seiscat',
+    'Documentation': 'https://seiscat.readthedocs.io'
+}
 
 setup(
     name='seiscat',
     packages=['seiscat', 'seiscat.scripts', 'seiscat.configobj'],
     include_package_data=True,
     entry_points={
         'console_scripts': ['seiscat = seiscat.scripts.seiscat:main']
-        },
+    },
     version=versioneer.get_version(),
     cmdclass=versioneer.get_cmdclass(),
     description='Keep a local seismic catalog',
     long_description=long_descr,
     long_description_content_type='text/markdown',
     author='Claudio Satriano',
     author_email='satriano@ipgp.fr',
-    url='https://github.com/SeismicSource/SeisCat',
+    url=project_urls['Homepage'],
+    project_urls=project_urls,
     license='GNU General Public License v3 or later (GPLv3+)',
     platforms='OS Independent',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Environment :: Console',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: '
@@ -35,10 +41,10 @@
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Topic :: Scientific/Engineering',
         'Topic :: Scientific/Engineering :: Physics'],
-    install_requires=['obspy>=1.1.0'],
+    install_requires=['obspy>=1.1.0', 'argcomplete'],
     python_requires='>=3.7'
-    )
+)
```

### Comparing `seiscat-0.3/versioneer.py` & `seiscat-0.4/versioneer.py`

 * *Files identical despite different names*

