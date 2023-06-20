# Comparing `tmp/apache-airflow-providers-postgres-5.5.0rc2.tar.gz` & `tmp/apache-airflow-providers-postgres-5.5.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-postgres-5.5.0rc2.tar", last modified: Fri May 19 17:53:14 2023, max compression
+gzip compressed data, was "apache-airflow-providers-postgres-5.5.1rc1.tar", last modified: Tue Jun 20 11:42:54 2023, max compression
```

## Comparing `apache-airflow-providers-postgres-5.5.0rc2.tar` & `apache-airflow-providers-postgres-5.5.1rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:14.000000 apache-airflow-providers-postgres-5.5.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-postgres-5.5.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:53:13.000000 apache-airflow-providers-postgres-5.5.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-postgres-5.5.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)    15180 2023-05-19 17:53:14.000000 apache-airflow-providers-postgres-5.5.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13597 2023-05-19 17:53:13.000000 apache-airflow-providers-postgres-5.5.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:14.000000 apache-airflow-providers-postgres-5.5.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:14.000000 apache-airflow-providers-postgres-5.5.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:14.000000 apache-airflow-providers-postgres-5.5.0rc2/airflow/providers/postgres/
--rw-r--r--   0 root         (0) root         (0)     1533 2023-05-19 12:20:14.000000 apache-airflow-providers-postgres-5.5.0rc2/airflow/providers/postgres/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3056 2023-05-19 17:53:13.000000 apache-airflow-providers-postgres-5.5.0rc2/airflow/providers/postgres/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:14.000000 apache-airflow-providers-postgres-5.5.0rc2/airflow/providers/postgres/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-postgres-5.5.0rc2/airflow/providers/postgres/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13001 2023-05-03 19:47:07.000000 apache-airflow-providers-postgres-5.5.0rc2/airflow/providers/postgres/hooks/postgres.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:14.000000 apache-airflow-providers-postgres-5.5.0rc2/airflow/providers/postgres/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-postgres-5.5.0rc2/airflow/providers/postgres/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3734 2023-05-03 19:47:07.000000 apache-airflow-providers-postgres-5.5.0rc2/airflow/providers/postgres/operators/postgres.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:14.000000 apache-airflow-providers-postgres-5.5.0rc2/apache_airflow_providers_postgres.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15180 2023-05-19 17:53:14.000000 apache-airflow-providers-postgres-5.5.0rc2/apache_airflow_providers_postgres.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      746 2023-05-19 17:53:14.000000 apache-airflow-providers-postgres-5.5.0rc2/apache_airflow_providers_postgres.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:53:14.000000 apache-airflow-providers-postgres-5.5.0rc2/apache_airflow_providers_postgres.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-05-19 17:53:14.000000 apache-airflow-providers-postgres-5.5.0rc2/apache_airflow_providers_postgres.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:53:14.000000 apache-airflow-providers-postgres-5.5.0rc2/apache_airflow_providers_postgres.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      197 2023-05-19 17:53:14.000000 apache-airflow-providers-postgres-5.5.0rc2/apache_airflow_providers_postgres.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:53:14.000000 apache-airflow-providers-postgres-5.5.0rc2/apache_airflow_providers_postgres.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-postgres-5.5.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1913 2023-05-19 17:53:14.000000 apache-airflow-providers-postgres-5.5.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1792 2023-05-19 17:53:13.000000 apache-airflow-providers-postgres-5.5.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:54.369568 apache-airflow-providers-postgres-5.5.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-postgres-5.5.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:53.000000 apache-airflow-providers-postgres-5.5.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-postgres-5.5.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    15566 2023-06-20 11:42:54.371066 apache-airflow-providers-postgres-5.5.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13982 2023-06-20 11:42:53.000000 apache-airflow-providers-postgres-5.5.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:54.296192 apache-airflow-providers-postgres-5.5.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:54.297518 apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:54.330567 apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-06-20 11:01:09.000000 apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3077 2023-06-20 11:42:53.000000 apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:54.336290 apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12967 2023-06-05 12:50:36.000000 apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/hooks/postgres.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:54.342002 apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3735 2023-06-02 11:31:21.000000 apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/operators/postgres.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:54.366685 apache-airflow-providers-postgres-5.5.1rc1/apache_airflow_providers_postgres.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15566 2023-06-20 11:42:54.000000 apache-airflow-providers-postgres-5.5.1rc1/apache_airflow_providers_postgres.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2023-06-20 11:42:54.000000 apache-airflow-providers-postgres-5.5.1rc1/apache_airflow_providers_postgres.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:54.000000 apache-airflow-providers-postgres-5.5.1rc1/apache_airflow_providers_postgres.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-06-20 11:42:54.000000 apache-airflow-providers-postgres-5.5.1rc1/apache_airflow_providers_postgres.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:54.000000 apache-airflow-providers-postgres-5.5.1rc1/apache_airflow_providers_postgres.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      197 2023-06-20 11:42:54.000000 apache-airflow-providers-postgres-5.5.1rc1/apache_airflow_providers_postgres.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:54.000000 apache-airflow-providers-postgres-5.5.1rc1/apache_airflow_providers_postgres.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-postgres-5.5.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1914 2023-06-20 11:42:54.373575 apache-airflow-providers-postgres-5.5.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1792 2023-06-20 11:42:53.000000 apache-airflow-providers-postgres-5.5.1rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apache-airflow-providers-postgres-5.5.0rc2/LICENSE` & `apache-airflow-providers-postgres-5.5.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.5.0rc2/MANIFEST.in` & `apache-airflow-providers-postgres-5.5.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.5.0rc2/PKG-INFO` & `apache-airflow-providers-postgres-5.5.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-postgres
-Version: 5.5.0rc2
+Version: 5.5.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-postgres package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.5.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.5.1/
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
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Monitoring
-Requires-Python: ~=3.7
+Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: amazon
 Provides-Extra: common.sql
 License-File: LICENSE
 License-File: NOTICE
 
 
@@ -50,38 +50,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-postgres``
 
-Release: ``5.5.0rc2``
+Release: ``5.5.1rc1``
 
 
 `PostgreSQL <https://www.postgresql.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``postgres`` provider. All classes for this provider package
 are in ``airflow.providers.postgres`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.5.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.5.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-postgres``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
@@ -132,14 +132,30 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+5.5.1
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Misc
+~~~~
+
+* ``Add note about dropping Python 3.7 for providers (#32015)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Improve docstrings in providers (#31681)``
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+
 5.5.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-postgres-5.5.0rc2/README.rst` & `apache-airflow-providers-postgres-5.5.1rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -15,38 +15,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-postgres``
 
-Release: ``5.5.0rc2``
+Release: ``5.5.1rc1``
 
 
 `PostgreSQL <https://www.postgresql.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``postgres`` provider. All classes for this provider package
 are in ``airflow.providers.postgres`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.5.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.5.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-postgres``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
@@ -97,14 +97,30 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+5.5.1
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Misc
+~~~~
+
+* ``Add note about dropping Python 3.7 for providers (#32015)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Improve docstrings in providers (#31681)``
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+
 5.5.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-postgres-5.5.0rc2/airflow/providers/postgres/__init__.py` & `apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "5.5.0"
+__version__ = "5.5.1"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-postgres-5.5.0rc2/airflow/providers/postgres/get_provider_info.py` & `apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/get_provider_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-postgres",
         "name": "PostgreSQL",
         "description": "`PostgreSQL <https://www.postgresql.org/>`__\n",
         "suspended": False,
         "versions": [
+            "5.5.1",
             "5.5.0",
             "5.4.0",
             "5.3.1",
             "5.3.0",
             "5.2.2",
             "5.2.1",
             "5.2.0",
```

### Comparing `apache-airflow-providers-postgres-5.5.0rc2/airflow/providers/postgres/hooks/__init__.py` & `apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.5.0rc2/airflow/providers/postgres/hooks/postgres.py` & `apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/hooks/postgres.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,15 @@
 from airflow.models.connection import Connection
 from airflow.providers.common.sql.hooks.sql import DbApiHook
 
 CursorType = Union[DictCursor, RealDictCursor, NamedTupleCursor]
 
 
 class PostgresHook(DbApiHook):
-    """
-    Interact with Postgres.
+    """Interact with Postgres.
 
     You can specify ssl parameters in the extra field of your connection
     as ``{"sslmode": "require", "sslcert": "/path/to/cert.pem", etc}``.
     Also you can choose cursor as ``{"cursor": "dictcursor"}``. Refer to the
     psycopg2.extras for more details.
 
     Note: For Redshift, use keepalives_idle in the extra connection parameters
@@ -142,16 +141,16 @@
             ]:
                 conn_args[arg_name] = arg_val
 
         self.conn = psycopg2.connect(**conn_args)
         return self.conn
 
     def copy_expert(self, sql: str, filename: str) -> None:
-        """
-        Executes SQL using psycopg2 copy_expert method.
+        """Executes SQL using psycopg2's ``copy_expert`` method.
+
         Necessary to execute COPY command without access to a superuser.
 
         Note: if this method is called with a "COPY FROM" statement and
         the specified input file does not exist, it creates an empty
         file and no data is loaded, but the operation succeeds.
         So if users want to be aware when the input file does not exist,
         they have to check its existence by themselves.
@@ -165,51 +164,53 @@
             with closing(self.get_conn()) as conn:
                 with closing(conn.cursor()) as cur:
                     cur.copy_expert(sql, file)
                     file.truncate(file.tell())
                     conn.commit()
 
     def get_uri(self) -> str:
-        """
-        Extract the URI from the connection.
+        """Extract the URI from the connection.
+
         :return: the extracted uri.
         """
         conn = self.get_connection(getattr(self, self.conn_name_attr))
         conn.schema = self.database or conn.schema
         uri = conn.get_uri().replace("postgres://", "postgresql://")
         return uri
 
     def bulk_load(self, table: str, tmp_file: str) -> None:
-        """Loads a tab-delimited file into a database table"""
+        """Loads a tab-delimited file into a database table."""
         self.copy_expert(f"COPY {table} FROM STDIN", tmp_file)
 
     def bulk_dump(self, table: str, tmp_file: str) -> None:
-        """Dumps a database table into a tab-delimited file"""
+        """Dumps a database table into a tab-delimited file."""
         self.copy_expert(f"COPY {table} TO STDOUT", tmp_file)
 
     @staticmethod
     def _serialize_cell(cell: object, conn: connection | None = None) -> Any:
-        """
-        Postgresql will adapt all arguments to the execute() method internally,
-        hence we return cell without any conversion.
+        """Serialize a cell.
+
+        PostgreSQL adapts all arguments to the ``execute()`` method internally,
+        hence we return the cell without any conversion.
 
         See http://initd.org/psycopg/docs/advanced.html#adapting-new-types for
         more information.
 
         :param cell: The cell to insert into the table
         :param conn: The database connection
         :return: The cell
         """
         return cell
 
     def get_iam_token(self, conn: Connection) -> tuple[str, str, int]:
-        """
-        Uses AWSHook to retrieve a temporary password to connect to Postgres
-        or Redshift. Port is required. If none is provided, default is used for
-        each service
+        """Get the IAM token.
+
+        This uses AWSHook to retrieve a temporary password to connect to
+        Postgres or Redshift. Port is required. If none is provided, the default
+        5432 is used.
         """
         try:
             from airflow.providers.amazon.aws.hooks.base_aws import AwsBaseHook
         except ImportError:
             from airflow.exceptions import AirflowException
 
             raise AirflowException(
@@ -238,16 +239,15 @@
             port = conn.port or 5432
             rds_client = AwsBaseHook(aws_conn_id=aws_conn_id, client_type="rds").conn
             # https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#RDS.Client.generate_db_auth_token
             token = rds_client.generate_db_auth_token(conn.host, port, conn.login)
         return login, token, port
 
     def get_table_primary_key(self, table: str, schema: str | None = "public") -> list[str] | None:
-        """
-        Helper method that returns the table primary key
+        """Get the table's primary key.
 
         :param table: Name of the target table
         :param schema: Name of the target schema, public by default
         :return: Primary key columns list
         """
         sql = """
             select kcu.column_name
@@ -263,17 +263,17 @@
         pk_columns = [row[0] for row in self.get_records(sql, (schema, table))]
         return pk_columns or None
 
     @classmethod
     def _generate_insert_sql(
         cls, table: str, values: tuple[str, ...], target_fields: Iterable[str], replace: bool, **kwargs
     ) -> str:
-        """
-        Static helper method that generates the INSERT SQL statement.
-        The REPLACE variant is specific to PostgreSQL syntax.
+        """Generate the INSERT SQL statement.
+
+        The REPLACE variant is specific to the PostgreSQL syntax.
 
         :param table: Name of the target table
         :param values: The row to insert into the table
         :param target_fields: The names of the columns to fill in the table
         :param replace: Whether to replace instead of insert
         :param replace_index: the column or list of column names to act as
             index for the ON CONFLICT clause
```

### Comparing `apache-airflow-providers-postgres-5.5.0rc2/airflow/providers/postgres/operators/__init__.py` & `apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.5.0rc2/airflow/providers/postgres/operators/postgres.py` & `apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/operators/postgres.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 from airflow.exceptions import AirflowProviderDeprecationWarning
 from airflow.providers.common.sql.operators.sql import SQLExecuteQueryOperator
 
 
 class PostgresOperator(SQLExecuteQueryOperator):
     """
-    Executes sql code in a specific Postgres database
+    Executes sql code in a specific Postgres database.
 
     :param sql: the SQL code to be executed as a single string, or
         a list of str (sql statements), or a reference to a template file.
         Template references are recognized by str ending in '.sql'
     :param postgres_conn_id: The :ref:`postgres conn id <howto/connection:postgres>`
         reference to a specific postgres database.
     :param autocommit: if True, each command is automatically committed.
```

### Comparing `apache-airflow-providers-postgres-5.5.0rc2/apache_airflow_providers_postgres.egg-info/PKG-INFO` & `apache-airflow-providers-postgres-5.5.1rc1/apache_airflow_providers_postgres.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-postgres
-Version: 5.5.0rc2
+Version: 5.5.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-postgres package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.5.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.5.1/
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
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Monitoring
-Requires-Python: ~=3.7
+Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: amazon
 Provides-Extra: common.sql
 License-File: LICENSE
 License-File: NOTICE
 
 
@@ -50,38 +50,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-postgres``
 
-Release: ``5.5.0rc2``
+Release: ``5.5.1rc1``
 
 
 `PostgreSQL <https://www.postgresql.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``postgres`` provider. All classes for this provider package
 are in ``airflow.providers.postgres`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.5.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.5.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-postgres``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
@@ -132,14 +132,30 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+5.5.1
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Misc
+~~~~
+
+* ``Add note about dropping Python 3.7 for providers (#32015)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Improve docstrings in providers (#31681)``
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+
 5.5.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-postgres-5.5.0rc2/apache_airflow_providers_postgres.egg-info/SOURCES.txt` & `apache-airflow-providers-postgres-5.5.1rc1/apache_airflow_providers_postgres.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.5.0rc2/pyproject.toml` & `apache-airflow-providers-postgres-5.5.1rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-postgres-5.5.0rc2/setup.cfg` & `apache-airflow-providers-postgres-5.5.1rc1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -17,34 +17,34 @@
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
+	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.5.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.5.1/
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
 	apache-airflow-providers-common-sql>=1.3.1.dev0
 	apache-airflow>=2.4.0.dev0
@@ -54,10 +54,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.postgres.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.postgres
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-postgres-5.5.0rc2/setup.py` & `apache-airflow-providers-postgres-5.5.1rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-postgres package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "5.5.0"
+version = "5.5.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-postgres setup."""
     setup(
         version=version,
         extras_require={
```

