# Comparing `tmp/apache-airflow-providers-ftp-3.4.1rc1.tar.gz` & `tmp/apache-airflow-providers-ftp-3.4.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-ftp-3.4.1rc1.tar", last modified: Wed May 24 07:20:26 2023, max compression
+gzip compressed data, was "apache-airflow-providers-ftp-3.4.2rc1.tar", last modified: Tue Jun 20 11:42:03 2023, max compression
```

## Comparing `apache-airflow-providers-ftp-3.4.1rc1.tar` & `apache-airflow-providers-ftp-3.4.2rc1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-05-23 11:35:15.000000 apache-airflow-providers-ftp-3.4.1rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-24 07:20:25.000000 apache-airflow-providers-ftp-3.4.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-05-23 11:35:15.000000 apache-airflow-providers-ftp-3.4.1rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     9972 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8403 2023-05-24 07:20:25.000000 apache-airflow-providers-ftp-3.4.1rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/
--rw-r--r--   0 root         (0) root         (0)     1528 2023-05-24 07:09:22.000000 apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2744 2023-05-24 07:20:25.000000 apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-05-23 11:35:14.000000 apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9842 2023-05-23 11:35:14.000000 apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/hooks/ftp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-05-23 11:35:14.000000 apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6093 2023-05-23 11:35:14.000000 apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/operators/ftp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-05-23 11:35:14.000000 apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3363 2023-05-23 11:35:14.000000 apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/sensors/ftp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/apache_airflow_providers_ftp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9972 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/apache_airflow_providers_ftp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      750 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/apache_airflow_providers_ftp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/apache_airflow_providers_ftp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      100 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/apache_airflow_providers_ftp.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/apache_airflow_providers_ftp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       27 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/apache_airflow_providers_ftp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/apache_airflow_providers_ftp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-23 11:35:15.000000 apache-airflow-providers-ftp-3.4.1rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1850 2023-05-24 07:20:26.000000 apache-airflow-providers-ftp-3.4.1rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1620 2023-05-24 07:20:25.000000 apache-airflow-providers-ftp-3.4.1rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:03.623457 apache-airflow-providers-ftp-3.4.2rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-ftp-3.4.2rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:02.000000 apache-airflow-providers-ftp-3.4.2rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-ftp-3.4.2rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    10296 2023-06-20 11:42:03.624667 apache-airflow-providers-ftp-3.4.2rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8777 2023-06-20 11:42:02.000000 apache-airflow-providers-ftp-3.4.2rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:03.540377 apache-airflow-providers-ftp-3.4.2rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:03.541702 apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:03.577906 apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/
+-rw-r--r--   0 root         (0) root         (0)     1528 2023-06-20 11:01:09.000000 apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2765 2023-06-20 11:42:02.000000 apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:03.583570 apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9846 2023-06-02 11:31:21.000000 apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/hooks/ftp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:03.589324 apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6079 2023-06-02 11:31:21.000000 apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/operators/ftp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:03.595048 apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3364 2023-06-02 11:31:21.000000 apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/sensors/ftp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:03.620290 apache-airflow-providers-ftp-3.4.2rc1/apache_airflow_providers_ftp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10296 2023-06-20 11:42:03.000000 apache-airflow-providers-ftp-3.4.2rc1/apache_airflow_providers_ftp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      750 2023-06-20 11:42:03.000000 apache-airflow-providers-ftp-3.4.2rc1/apache_airflow_providers_ftp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:03.000000 apache-airflow-providers-ftp-3.4.2rc1/apache_airflow_providers_ftp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2023-06-20 11:42:03.000000 apache-airflow-providers-ftp-3.4.2rc1/apache_airflow_providers_ftp.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:03.000000 apache-airflow-providers-ftp-3.4.2rc1/apache_airflow_providers_ftp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       27 2023-06-20 11:42:03.000000 apache-airflow-providers-ftp-3.4.2rc1/apache_airflow_providers_ftp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:03.000000 apache-airflow-providers-ftp-3.4.2rc1/apache_airflow_providers_ftp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-ftp-3.4.2rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1811 2023-06-20 11:42:03.626640 apache-airflow-providers-ftp-3.4.2rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1620 2023-06-20 11:42:02.000000 apache-airflow-providers-ftp-3.4.2rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apache-airflow-providers-ftp-3.4.1rc1/LICENSE` & `apache-airflow-providers-ftp-3.4.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.1rc1/MANIFEST.in` & `apache-airflow-providers-ftp-3.4.2rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.1rc1/PKG-INFO` & `apache-airflow-providers-ftp-3.4.2rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-ftp
-Version: 3.4.1rc1
+Version: 3.4.2rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-ftp package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-ftp/3.4.1/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-ftp/3.4.2/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Monitoring
-Requires-Python: ~=3.7
+Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: NOTICE
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
    or more contributor license agreements.  See the NOTICE file
@@ -49,38 +48,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-ftp``
 
-Release: ``3.4.1rc1``
+Release: ``3.4.2rc1``
 
 
 `File Transfer Protocol (FTP) <https://tools.ietf.org/html/rfc114>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``ftp`` provider. All classes for this provider package
 are in ``airflow.providers.ftp`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-ftp/3.4.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-ftp/3.4.2/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-ftp``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
@@ -109,14 +108,30 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.4.2
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Misc
+~~~~
+
+* ``Remove Python 3.7 support (#30963)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 3.4.1
 .....
 
 Misc
 ~~~~
 
 * ``Bring back min-airflow-version for preinstalled providers (#31469)``
```

### Comparing `apache-airflow-providers-ftp-3.4.1rc1/README.rst` & `apache-airflow-providers-ftp-3.4.2rc1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -15,38 +15,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-ftp``
 
-Release: ``3.4.1rc1``
+Release: ``3.4.2rc1``
 
 
 `File Transfer Protocol (FTP) <https://tools.ietf.org/html/rfc114>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``ftp`` provider. All classes for this provider package
 are in ``airflow.providers.ftp`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-ftp/3.4.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-ftp/3.4.2/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-ftp``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
@@ -75,14 +75,30 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.4.2
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Misc
+~~~~
+
+* ``Remove Python 3.7 support (#30963)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 3.4.1
 .....
 
 Misc
 ~~~~
 
 * ``Bring back min-airflow-version for preinstalled providers (#31469)``
```

### Comparing `apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/__init__.py` & `apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "3.4.1"
+__version__ = "3.4.2"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/get_provider_info.py` & `apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/get_provider_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-ftp",
         "name": "File Transfer Protocol (FTP)",
         "description": "`File Transfer Protocol (FTP) <https://tools.ietf.org/html/rfc114>`__\n",
         "suspended": False,
         "versions": [
+            "3.4.2",
             "3.4.1",
             "3.4.0",
             "3.3.1",
             "3.3.0",
             "3.2.0",
             "3.1.0",
             "3.0.0",
```

### Comparing `apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/hooks/__init__.py` & `apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/hooks/ftp.py` & `apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/hooks/ftp.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         return self
 
     def __exit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> None:
         if self.conn is not None:
             self.close_conn()
 
     def get_conn(self) -> ftplib.FTP:
-        """Returns a FTP connection object"""
+        """Returns a FTP connection object."""
         if self.conn is None:
             params = self.get_connection(self.ftp_conn_id)
             pasv = params.extra_dejson.get("passive", True)
             self.conn = ftplib.FTP(params.host, params.login, params.password)
             self.conn.set_pasv(pasv)
 
         return self.conn
@@ -240,39 +240,39 @@
         :param to_name: rename file to name
         """
         conn = self.get_conn()
         return conn.rename(from_name, to_name)
 
     def get_mod_time(self, path: str) -> datetime.datetime:
         """
-        Returns a datetime object representing the last time the file was modified
+        Returns a datetime object representing the last time the file was modified.
 
         :param path: remote file path
         """
         conn = self.get_conn()
         ftp_mdtm = conn.sendcmd("MDTM " + path)
         time_val = ftp_mdtm[4:]
         # time_val optionally has microseconds
         try:
             return datetime.datetime.strptime(time_val, "%Y%m%d%H%M%S.%f")
         except ValueError:
             return datetime.datetime.strptime(time_val, "%Y%m%d%H%M%S")
 
     def get_size(self, path: str) -> int | None:
         """
-        Returns the size of a file (in bytes)
+        Returns the size of a file (in bytes).
 
         :param path: remote file path
         """
         conn = self.get_conn()
         size = conn.size(path)
         return int(size) if size else None
 
     def test_connection(self) -> tuple[bool, str]:
-        """Test the FTP connection by calling path with directory"""
+        """Test the FTP connection by calling path with directory."""
         try:
             conn = self.get_conn()
             conn.pwd
             return True, "Connection successfully tested"
         except Exception as e:
             return False, str(e)
```

### Comparing `apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/operators/__init__.py` & `apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/operators/ftp.py` & `apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/operators/ftp.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,24 +15,24 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """This module contains FTP operator."""
 from __future__ import annotations
 
 import os
+from functools import cached_property
 from pathlib import Path
 from typing import Any, Sequence
 
-from airflow.compat.functools import cached_property
 from airflow.models import BaseOperator
 from airflow.providers.ftp.hooks.ftp import FTPHook, FTPSHook
 
 
 class FTPOperation:
-    """Operation that can be used with FTP"""
+    """Operation that can be used with FTP."""
 
     PUT = "put"
     GET = "get"
 
 
 class FTPFileTransmitOperator(BaseOperator):
     """
```

### Comparing `apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/sensors/__init__.py` & `apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.1rc1/airflow/providers/ftp/sensors/ftp.py` & `apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/sensors/ftp.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         self.fail_on_transient_errors = fail_on_transient_errors
 
     def _create_hook(self) -> FTPHook:
         """Return connection hook."""
         return FTPHook(ftp_conn_id=self.ftp_conn_id)
 
     def _get_error_code(self, e):
-        """Extract error code from ftp exception"""
+        """Extract error code from ftp exception."""
         try:
             matches = self.error_code_pattern.match(str(e))
             code = int(matches.group(0))
             return code
         except ValueError:
             return e
```

### Comparing `apache-airflow-providers-ftp-3.4.1rc1/apache_airflow_providers_ftp.egg-info/PKG-INFO` & `apache-airflow-providers-ftp-3.4.2rc1/apache_airflow_providers_ftp.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-ftp
-Version: 3.4.1rc1
+Version: 3.4.2rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-ftp package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-ftp/3.4.1/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-ftp/3.4.2/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Monitoring
-Requires-Python: ~=3.7
+Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: NOTICE
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
    or more contributor license agreements.  See the NOTICE file
@@ -49,38 +48,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-ftp``
 
-Release: ``3.4.1rc1``
+Release: ``3.4.2rc1``
 
 
 `File Transfer Protocol (FTP) <https://tools.ietf.org/html/rfc114>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``ftp`` provider. All classes for this provider package
 are in ``airflow.providers.ftp`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-ftp/3.4.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-ftp/3.4.2/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-ftp``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
@@ -109,14 +108,30 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.4.2
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Misc
+~~~~
+
+* ``Remove Python 3.7 support (#30963)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 3.4.1
 .....
 
 Misc
 ~~~~
 
 * ``Bring back min-airflow-version for preinstalled providers (#31469)``
```

### Comparing `apache-airflow-providers-ftp-3.4.1rc1/apache_airflow_providers_ftp.egg-info/SOURCES.txt` & `apache-airflow-providers-ftp-3.4.2rc1/apache_airflow_providers_ftp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.1rc1/pyproject.toml` & `apache-airflow-providers-ftp-3.4.2rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,42 +22,43 @@
 # and we have to pin it to 63.4.3 version
 # The problem is tracked (and this limitation might be removed if it is solved) in:
 # https://github.com/pypa/setuptools/issues/3548
 [build-system]
 requires = ['setuptools==67.2.0']
 build-backend = "setuptools.build_meta"
 
+[project]
+requires-python = ">=3.8"
+
 [tool.ruff]
 typing-modules = ["airflow.typing_compat"]
 line-length = 110
 extend-exclude = [
     ".eggs",
     "airflow/_vendor/*",
     "airflow/providers/google/ads/_vendor/*",
     # The files generated by stubgen aren't 100% valid syntax it turns out, and we don't ship them, so we can
     # ignore them in ruff
-    "airflow/providers/common/sql/*/*.pyi"
+    "airflow/providers/common/sql/*/*.pyi",
+    "airflow/migrations/versions/*.py"
 ]
 
-# TODO: Bump to Python 3.8 when support for Python 3.7 is dropped in Airflow.
-target-version = "py37"
-
 extend-select = [
     "I", # Missing required import (auto-fixable)
     "UP", # Pyupgrade
     "RUF100", # Unused noqa (auto-fixable)
 
     # implicit single-line string concatenation
     "ISC001",
     # We ignore more pydocstyle than we enable, so be more selective at what we enable
     "D101",
     "D106",
     "D2",
     "D3",
-    # "D400", WIP: see #31135
+    "D400",
     # "D401", # Not enabled by ruff, but we don't want it
     "D402",
     "D403",
     "D412",
     "D419"
 ]
 extend-ignore = [
```

### Comparing `apache-airflow-providers-ftp-3.4.1rc1/setup.cfg` & `apache-airflow-providers-ftp-3.4.2rc1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -17,35 +17,34 @@
 	Environment :: Console
 	Environment :: Web Environment
 	Intended Audience :: Developers
 	Intended Audience :: System Administrators
 	Framework :: Apache Airflow
 	Framework :: Apache Airflow :: Provider
 	License :: OSI Approved :: Apache Software License
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-ftp/3.4.1/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-ftp/3.4.2/
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
 python_tag = py3
 
 [options]
 zip_safe = False
 include_package_data = True
-python_requires = ~=3.7
+python_requires = ~=3.8
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
 	apache-airflow>=2.4.0.dev0
```

### Comparing `apache-airflow-providers-ftp-3.4.1rc1/setup.py` & `apache-airflow-providers-ftp-3.4.2rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-ftp package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.4.1"
+version = "3.4.2"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-ftp setup."""
     setup(
         version=version,
         extras_require={},
```

