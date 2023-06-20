# Comparing `tmp/pysqream-blue-1.0.27.tar.gz` & `tmp/pysqream-blue-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pysqream-blue-1.0.27.tar", last modified: Tue Jun 20 12:03:25 2023, max compression
+gzip compressed data, was "dist/pysqream-blue-1.0.3.tar", last modified: Mon Sep 12 07:22:00 2022, max compression
```

## Comparing `pysqream-blue-1.0.27.tar` & `pysqream-blue-1.0.3.tar`

### file list

```diff
@@ -1,32 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:03:25.000000 pysqream-blue-1.0.27/
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-20 12:03:04.000000 pysqream-blue-1.0.27/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-06-20 12:03:25.000000 pysqream-blue-1.0.27/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-06-20 12:03:04.000000 pysqream-blue-1.0.27/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:03:25.000000 pysqream-blue-1.0.27/protos/
--rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-06-20 12:03:04.000000 pysqream-blue-1.0.27/protos/authentication_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-06-20 12:03:04.000000 pysqream-blue-1.0.27/protos/authentication_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-20 12:03:04.000000 pysqream-blue-1.0.27/protos/authentication_type_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-20 12:03:04.000000 pysqream-blue-1.0.27/protos/authentication_type_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-20 12:03:04.000000 pysqream-blue-1.0.27/protos/client_info_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-20 12:03:04.000000 pysqream-blue-1.0.27/protos/client_info_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-20 12:03:04.000000 pysqream-blue-1.0.27/protos/error_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-20 12:03:04.000000 pysqream-blue-1.0.27/protos/error_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15101 2023-06-20 12:03:04.000000 pysqream-blue-1.0.27/protos/queryhandler_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12578 2023-06-20 12:03:04.000000 pysqream-blue-1.0.27/protos/queryhandler_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:03:25.000000 pysqream-blue-1.0.27/pysqream_blue/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-20 12:03:04.000000 pysqream-blue-1.0.27/pysqream_blue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-20 12:03:04.000000 pysqream-blue-1.0.27/pysqream_blue/casting.py
--rw-r--r--   0 runner    (1001) docker     (123)     9906 2023-06-20 12:03:04.000000 pysqream-blue-1.0.27/pysqream_blue/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    17388 2023-06-20 12:03:04.000000 pysqream-blue-1.0.27/pysqream_blue/cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-06-20 12:03:04.000000 pysqream-blue-1.0.27/pysqream_blue/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-20 12:03:04.000000 pysqream-blue-1.0.27/pysqream_blue/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3124 2023-06-20 12:03:04.000000 pysqream-blue-1.0.27/pysqream_blue/pysqream_blue.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-20 12:03:04.000000 pysqream-blue-1.0.27/pysqream_blue/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:03:25.000000 pysqream-blue-1.0.27/pysqream_blue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-06-20 12:03:25.000000 pysqream-blue-1.0.27/pysqream_blue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-20 12:03:25.000000 pysqream-blue-1.0.27/pysqream_blue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 12:03:25.000000 pysqream-blue-1.0.27/pysqream_blue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-20 12:03:25.000000 pysqream-blue-1.0.27/pysqream_blue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-20 12:03:25.000000 pysqream-blue-1.0.27/pysqream_blue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 12:03:25.000000 pysqream-blue-1.0.27/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-20 12:03:04.000000 pysqream-blue-1.0.27/setup.py
+drwxr-xr-x   0 danielgutman   (501) staff       (20)        0 2022-09-12 07:22:00.000000 pysqream-blue-1.0.3/
+-rw-r--r--   0 danielgutman   (501) staff       (20)     1519 2022-09-08 17:40:28.000000 pysqream-blue-1.0.3/LICENSE
+-rw-r--r--   0 danielgutman   (501) staff       (20)     6529 2022-09-12 07:22:00.000000 pysqream-blue-1.0.3/PKG-INFO
+-rw-r--r--   0 danielgutman   (501) staff       (20)     6025 2022-09-12 07:21:54.000000 pysqream-blue-1.0.3/README.rst
+drwxr-xr-x   0 danielgutman   (501) staff       (20)        0 2022-09-12 07:22:00.000000 pysqream-blue-1.0.3/pysqream_blue/
+-rw-r--r--   0 danielgutman   (501) staff       (20)      110 2022-09-11 08:29:17.000000 pysqream-blue-1.0.3/pysqream_blue/__init__.py
+-rw-r--r--   0 danielgutman   (501) staff       (20)     1993 2022-09-11 08:29:17.000000 pysqream-blue-1.0.3/pysqream_blue/casting.py
+-rw-r--r--   0 danielgutman   (501) staff       (20)     7733 2022-09-11 08:29:17.000000 pysqream-blue-1.0.3/pysqream_blue/connection.py
+-rw-r--r--   0 danielgutman   (501) staff       (20)    14683 2022-09-11 08:29:17.000000 pysqream-blue-1.0.3/pysqream_blue/cursor.py
+-rw-r--r--   0 danielgutman   (501) staff       (20)     2639 2022-09-11 10:05:35.000000 pysqream-blue-1.0.3/pysqream_blue/globals.py
+-rw-r--r--   0 danielgutman   (501) staff       (20)     1566 2022-09-11 08:29:17.000000 pysqream-blue-1.0.3/pysqream_blue/logger.py
+-rw-r--r--   0 danielgutman   (501) staff       (20)     2944 2022-09-11 08:29:17.000000 pysqream-blue-1.0.3/pysqream_blue/pysqream_blue.py
+-rw-r--r--   0 danielgutman   (501) staff       (20)      439 2022-09-11 08:29:17.000000 pysqream-blue-1.0.3/pysqream_blue/utils.py
+drwxr-xr-x   0 danielgutman   (501) staff       (20)        0 2022-09-12 07:22:00.000000 pysqream-blue-1.0.3/pysqream_blue.egg-info/
+-rw-r--r--   0 danielgutman   (501) staff       (20)     6529 2022-09-12 07:22:00.000000 pysqream-blue-1.0.3/pysqream_blue.egg-info/PKG-INFO
+-rw-r--r--   0 danielgutman   (501) staff       (20)      483 2022-09-12 07:22:00.000000 pysqream-blue-1.0.3/pysqream_blue.egg-info/SOURCES.txt
+-rw-r--r--   0 danielgutman   (501) staff       (20)        1 2022-09-12 07:22:00.000000 pysqream-blue-1.0.3/pysqream_blue.egg-info/dependency_links.txt
+-rw-r--r--   0 danielgutman   (501) staff       (20)       83 2022-09-12 07:22:00.000000 pysqream-blue-1.0.3/pysqream_blue.egg-info/requires.txt
+-rw-r--r--   0 danielgutman   (501) staff       (20)       20 2022-09-12 07:22:00.000000 pysqream-blue-1.0.3/pysqream_blue.egg-info/top_level.txt
+-rw-r--r--   0 danielgutman   (501) staff       (20)       38 2022-09-12 07:22:00.000000 pysqream-blue-1.0.3/setup.cfg
+-rw-r--r--   0 danielgutman   (501) staff       (20)      973 2022-09-12 07:08:06.000000 pysqream-blue-1.0.3/setup.py
+drwxr-xr-x   0 danielgutman   (501) staff       (20)        0 2022-09-12 07:22:00.000000 pysqream-blue-1.0.3/tests/
+-rw-r--r--   0 danielgutman   (501) staff       (20)        0 2022-09-08 17:37:05.000000 pysqream-blue-1.0.3/tests/__init__.py
+-rw-r--r--   0 danielgutman   (501) staff       (20)      177 2022-09-08 17:37:05.000000 pysqream-blue-1.0.3/tests/conftest.py
+-rw-r--r--   0 danielgutman   (501) staff       (20)      628 2022-09-08 17:37:05.000000 pysqream-blue-1.0.3/tests/logger.py
+-rw-r--r--   0 danielgutman   (501) staff       (20)    30969 2022-09-08 17:37:05.000000 pysqream-blue-1.0.3/tests/test.py
```

### Comparing `pysqream-blue-1.0.27/LICENSE` & `pysqream-blue-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.27/PKG-INFO` & `pysqream-blue-1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,70 +1,73 @@
 Metadata-Version: 2.1
 Name: pysqream-blue
-Version: 1.0.27
+Version: 1.0.3
 Summary: DB-API connector for SQream DB
 Home-page: https://github.com/SQream/pysqream-blue
 Author: SQream
 Author-email: info@sqream.com
 License: UNKNOWN
 Keywords: database db-api sqream sqreamdbV2
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.6.5
 Description-Content-Type: 
 ===================================
 Python connector for SQream DB Blue
 ===================================
 
-* **Version:**  1.0.27
+* **Version:**  1.0.10
 
 * **Supported SQream DB versions:** >= Blue cloud
 
 The Python connector for SQream DB is a Python DB API 2.0-compliant interface for developing Python applications with SQream DB.
 
 The SQream Python connector provides an interface for creating and running Python applications that can connect to a SQream DB database. It provides a lighter-weight alternative to working through native C++ or Java bindings, including JDBC and ODBC drivers.
 
 pysqream conforms to Python DB-API specifications `PEP-249 <https://www.python.org/dev/peps/pep-0249/>`_
 
-``pysqream_blue`` is native and pure Python, with minimal requirements. It can be installed with ``pip3`` on any operating system, including Linux, Windows, and macOS.
+``pysqream_blue`` is native and pure Python, with minimal requirements. It can be installed with ``pip`` on any operating system, including Linux, Windows, and macOS.
 
 .. For more information and a full API reference, see `SQream documentation's pysqream blue guide <https://sqream-docs.readthedocs.io/en/latest/guides/client_drivers/python/index.html>`_ .
 
 Requirements
 -------------
 
-* Python 3.9+
+* Python 3.6.5+, with 3.7+ highly recommended
 
 Installing the Python connector
 --------------------------------
 
 Prerequisites
 ----------------
 
 1. Python
 ^^^^^^^^^^^^
 
-The connector requires Python 3.9 or newer. To verify your version of Python:
+The connector requires Python 3.6.5 or newer. To verify your version of Python:
 
 .. code-block:: console
 
    $ python --version
-   Python 3.9
+   Python 3.7.3
+
+
+Note: If both Python 2.x and 3.x are installed, you can run ``python3`` and ``pip3`` instead of ``python`` and ``pip`` respectively for the rest of this guide
 
 2. PIP
 ^^^^^^^^^^^^
-The Python connector is installed via ``pip3``, the Python package manager and installer.
+The Python connector is installed via ``pip``, the Python package manager and installer.
 
-We recommend upgrading to the latest version of ``pip3`` before installing. To verify that you are on the latest version, run the following command:
+We recommend upgrading to the latest version of ``pip`` before installing. To verify that you are on the latest version, run the following command:
 
 .. code-block:: console
 
-   $ python -m pip3 install --upgrade pip
+   $ python -m pip install --upgrade pip
    Collecting pip
       Downloading https://files.pythonhosted.org/packages/00/b6/9cfa56b4081ad13874b0c6f96af8ce16cfbc1cb06bedf8e9164ce5551ec1/pip-19.3.1-py2.py3-none-any.whl (1.4MB)
         |████████████████████████████████| 1.4MB 1.6MB/s
    Installing collected packages: pip
      Found existing installation: pip 19.1.1
        Uninstalling pip-19.1.1:
          Successfully uninstalled pip-19.1.1
@@ -76,21 +79,21 @@
 
 
 Install via pip
 -----------------
 
 The Python connector is available via `PyPi <https://pypi.org/project/pysqream/>`_.
 
-Install the connector with ``pip3``:
+Install the connector with ``pip``:
 
 .. code-block:: console
 
-   $ pip3 install pysqream-blue
+   $ pip install pysqream-blue
 
-``pip3`` will automatically installs all necessary libraries and modules.
+``pip`` will automatically installs all necessary libraries and modules.
 
 Validate the installation
 -----------------------------
 
 Create a file called ``test.py`` (make sure to replace the parameters in the connection with the respective parameters for your SQream DB installation):
 
 .. code-block:: python
```

### Comparing `pysqream-blue-1.0.27/README.rst` & `pysqream-blue-1.0.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,56 +1,59 @@
 
 ===================================
 Python connector for SQream DB Blue
 ===================================
 
-* **Version:**  1.0.27
+* **Version:**  1.0.10
 
 * **Supported SQream DB versions:** >= Blue cloud
 
 The Python connector for SQream DB is a Python DB API 2.0-compliant interface for developing Python applications with SQream DB.
 
 The SQream Python connector provides an interface for creating and running Python applications that can connect to a SQream DB database. It provides a lighter-weight alternative to working through native C++ or Java bindings, including JDBC and ODBC drivers.
 
 pysqream conforms to Python DB-API specifications `PEP-249 <https://www.python.org/dev/peps/pep-0249/>`_
 
-``pysqream_blue`` is native and pure Python, with minimal requirements. It can be installed with ``pip3`` on any operating system, including Linux, Windows, and macOS.
+``pysqream_blue`` is native and pure Python, with minimal requirements. It can be installed with ``pip`` on any operating system, including Linux, Windows, and macOS.
 
 .. For more information and a full API reference, see `SQream documentation's pysqream blue guide <https://sqream-docs.readthedocs.io/en/latest/guides/client_drivers/python/index.html>`_ .
 
 Requirements
 -------------
 
-* Python 3.9+
+* Python 3.6.5+, with 3.7+ highly recommended
 
 Installing the Python connector
 --------------------------------
 
 Prerequisites
 ----------------
 
 1. Python
 ^^^^^^^^^^^^
 
-The connector requires Python 3.9 or newer. To verify your version of Python:
+The connector requires Python 3.6.5 or newer. To verify your version of Python:
 
 .. code-block:: console
 
    $ python --version
-   Python 3.9
+   Python 3.7.3
+
+
+Note: If both Python 2.x and 3.x are installed, you can run ``python3`` and ``pip3`` instead of ``python`` and ``pip`` respectively for the rest of this guide
 
 2. PIP
 ^^^^^^^^^^^^
-The Python connector is installed via ``pip3``, the Python package manager and installer.
+The Python connector is installed via ``pip``, the Python package manager and installer.
 
-We recommend upgrading to the latest version of ``pip3`` before installing. To verify that you are on the latest version, run the following command:
+We recommend upgrading to the latest version of ``pip`` before installing. To verify that you are on the latest version, run the following command:
 
 .. code-block:: console
 
-   $ python -m pip3 install --upgrade pip
+   $ python -m pip install --upgrade pip
    Collecting pip
       Downloading https://files.pythonhosted.org/packages/00/b6/9cfa56b4081ad13874b0c6f96af8ce16cfbc1cb06bedf8e9164ce5551ec1/pip-19.3.1-py2.py3-none-any.whl (1.4MB)
         |████████████████████████████████| 1.4MB 1.6MB/s
    Installing collected packages: pip
      Found existing installation: pip 19.1.1
        Uninstalling pip-19.1.1:
          Successfully uninstalled pip-19.1.1
@@ -62,21 +65,21 @@
 
 
 Install via pip
 -----------------
 
 The Python connector is available via `PyPi <https://pypi.org/project/pysqream/>`_.
 
-Install the connector with ``pip3``:
+Install the connector with ``pip``:
 
 .. code-block:: console
 
-   $ pip3 install pysqream-blue
+   $ pip install pysqream-blue
 
-``pip3`` will automatically installs all necessary libraries and modules.
+``pip`` will automatically installs all necessary libraries and modules.
 
 Validate the installation
 -----------------------------
 
 Create a file called ``test.py`` (make sure to replace the parameters in the connection with the respective parameters for your SQream DB installation):
 
 .. code-block:: python
```

### Comparing `pysqream-blue-1.0.27/pysqream_blue/casting.py` & `pysqream-blue-1.0.3/pysqream_blue/casting.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.27/pysqream_blue/connection.py` & `pysqream-blue-1.0.3/pysqream_blue/connection.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,27 @@
-from pysqream_blue.logger import *
+from logger import *
 import grpc
-from pysqream_blue.globals import auth_services, auth_messages, qh_services, qh_messages, cl_messages, auth_type_messages
+from globals import auth_services, auth_messages, qh_services, qh_messages, cl_messages
 import time
 import socket
-from pysqream_blue.utils import is_token_expired
-from pysqream_blue.cursor import Cursor
+from cursor import Cursor
 
 
 class Connection:
     ''' Connection class used to interact with SQream '''
 
-    def __init__(self, host: str, port: str, use_ssl: bool = True, log = False, is_base_connection: bool = True,
-                 reconnect_attempts : int = 10, reconnect_interval : int = 3, query_timeout: int = 0,
-                 pool_name: str = None):
+    def __init__(self, host: str, port: str, use_ssl: bool = False, log = False, is_base_connection: bool = True,
+                 reconnect_attempts : int = 10, reconnect_interval : int = 3, query_timeout: int = 0):
         self.host, self.port, self.use_ssl = host, port, use_ssl
-        # Product want to connect with SSL
-        self.use_ssl = True
         self.is_base_connection = is_base_connection
         self.reconnect_attempts, self.reconnect_interval = reconnect_attempts, reconnect_interval
         self.connected = False
         self.session_opened = False
         self.statement_opened = False
         self.query_timeout = query_timeout
-        self.pool_name = pool_name
 
         self.is_base_connection = is_base_connection
         if is_base_connection:
             self.cursors = []
             self._connect_to_server()
 
         if log is not False:
@@ -41,16 +36,17 @@
             log_and_raise(ProgrammingError, "Trying to connect to a server that's already connected")
 
         try_connect_num = 0
         while True:
             try:
                 options = [('grpc.max_message_length', 1024 ** 3), ('grpc.max_receive_message_length', 1024 ** 3)]
                 if self.use_ssl:
-                    options.append(("grpc.enable_http_proxy", 0))
-                    self.channel = grpc.secure_channel(f'{self.host}:{self.port}', grpc.ssl_channel_credentials(), options=options)
+                    log_and_raise(NotSupportedError, 'SQream dose not currently support ssl connection')
+                    # options.append(("grpc.enable_http_proxy", 0))
+                    # self.channel = grpc.secure_channel(f'{self.host}:{self.port}', grpc.ssl_channel_credentials(), options=options)
                 else:
                     self.channel = grpc.insecure_channel(f'{self.host}:{self.port}', options=options)
                 self.auth_stub = auth_services.AuthenticationServiceStub(self.channel)
                 self.client    = qh_services.QueryHandlerServiceStub(self.channel)
                 break
             except grpc.RpcError as rpc_error:
                 try_connect_num += 1
@@ -78,136 +74,84 @@
         except grpc.RpcError as rpc_error:
             log_error(f'Error from grpc while attempting to disconnect from server.\n{rpc_error}')
             return
 
         self.connected = False
         log_info(f'Connection closed to the server at: {self.host}:{self.port}.')
 
-    def connect_database(self, database: str, username: str, password: str, tenant_id: str, service: str,
-                         access_token: str):
+    def connect_database(self, database: str, username: str, password: str, tenant_id: str, service: str):
         """Authentication and token receipt"""
 
-        self.database, self.username, self.password, self.tenant_id, self.service, self.access_token = \
-            database, username, password, tenant_id, service, access_token
+        self.database, self.username, self.password, self.tenant_id, self.service = database, username, password, tenant_id, service
 
         if self.session_opened:
             ''' user should not reconnect before closing the previous connection'''
             log_and_raise(ProgrammingError, "Trying to connect to a database that's already connected")
         if not self.connected:
             self._connect_to_server()
 
-        auth_response: auth_messages.AuthResponse = None
-        session_response: auth_messages.SessionResponse = None
         try:
-            if self.access_token is None:
-                auth_response = self.auth_user_password()
-            else:
-                auth_response = self.auth_access_token()
+            auth_response: auth_messages.AuthResponse = self.auth_stub.Auth(auth_messages.AuthRequest(
+                user=self.username,
+                password=self.password,
+                tenant_id=self.tenant_id,
+                database=self.database,
+                source_ip=socket.gethostbyname(socket.gethostname()),
+                client_info = cl_messages.ClientInfo(version='PySQream2_V_111')))
+            self.token, self.token_type, self.context_id = auth_response.token, auth_response.token_type, auth_response.context_id
+            self.expiration_time = auth_response.exp_time + time.time() * 1000
+            self.call_credentialds = grpc.access_token_call_credentials(self.token)
         except grpc.RpcError as rpc_error:
-            log_and_raise(ProgrammingError,
-                          f'Error from grpc while attempting to open database connection.\n{rpc_error}')
-
+            log_and_raise(ProgrammingError, f'Error from grpc while attempting to open database connection.\n{rpc_error}')
         if auth_response.HasField('error'):
-            log_and_raise(OperationalError,
-                          f'Error while attempting to open database connection.\n{auth_response.error}')
-
-        try:
-            self.token = auth_response.token
-            session_response = self.open_session()
-        except grpc.RpcError as rpc_error:
-            log_and_raise(ProgrammingError,
-                          f'Error from grpc while attempting to open database connection.\n{rpc_error}')
+            log_and_raise(OperationalError, f'Error while attempting to open database connection.\n{auth_response.error}')
 
-            if is_token_expired(str(rpc_error)):
-                auth_response = self.auth_access_token()
-                self.token = auth_response.token
-                session_response = self.open_session()
-
-        if session_response.HasField('error'):
-            log_and_raise(OperationalError,
-                          f'Error while attempting to open database connection.\n{session_response.error}')
-
-        self.context_id, self.sqream_version = session_response.context_id, session_response.sqream_version
-        # hour = 1 * 60 * 60 * 1000
-        # self.expiration_time = hour + time.time() * 1000
-        self.call_credentialds = grpc.access_token_call_credentials(self.token)
         self.session_opened = True
-        log_info(f'''Connection opened to database {database}. username: {self.username}.''')
-
-    def open_session(self):
-        session_response: auth_messages.SessionResponse = self.auth_stub.Session(auth_messages.SessionRequest(
-            tenant_id=self.tenant_id,
-            database=self.database,
-            source_ip=socket.gethostbyname(socket.gethostname()),
-            client_info=cl_messages.ClientInfo(version='PySQream2_V_111'),
-            pool_name=self.pool_name
-        ), credentials=grpc.access_token_call_credentials(self.token))
-        return session_response
-
-    def auth_user_password(self) -> auth_messages.AuthResponse:
-        return self.auth_stub.Auth(auth_messages.AuthRequest(
-            auth_type=auth_type_messages.AUTHENTICATION_TYPE_INTERNAL,
-            user=self.username,
-            password=self.password
-        ))
-
-    def auth_access_token(self) -> auth_messages.AuthResponse:
-        return self.auth_stub.Auth(auth_messages.AuthRequest(
-            auth_type=auth_type_messages.AUTHENTICATION_TYPE_IDP,
-            access_token=self.access_token
-        ))
+        log_info(f'''Connection opened to database {database}. username: {self.username}.
+                    The connection will be valid for {auth_response.exp_time / 1000} seconds.''')
 
     def close_connection(self):
         self.close()
 
     def close(self):
         """Disconnect from database. the connection to the server remains open."""
         if not self.session_opened:
             log_warning("Trying to close a session that's already closed")
             return
 
         if self.is_base_connection:
             for cursor in self.cursors:
-                if cursor.statement_opened:
-                    cursor.close()
+                cursor.close()
 
-        close_response: qh_messages.CloseResponse = None
         try:
-            close_response: qh_messages.CloseResponse = self._close()
+            close_response: qh_messages.CloseResponse = self.client.CloseSession(
+                qh_messages.CloseSessionRequest(close_request=qh_messages.CloseRequest(context_id=self.context_id)),
+                credentials=self.call_credentialds if self.use_ssl else None
+            ).close_response
         except grpc.RpcError as rpc_error:
             log_error(f'Error from grpc while attempting to close database connection.\n{rpc_error}')
-
-            if is_token_expired(str(rpc_error)):
-                auth_response = self.auth_access_token()
-                self.token = auth_response.token
-                close_response: qh_messages.CloseResponse = self._close()
-
+            return
         if close_response.HasField('error'):
             log_error(f'Error while attempting to close database connection.\n{close_response.error}')
+            return
 
         self.session_opened = False
         log_info(f'Connection closed to database {self.database}.')
 
-    def _close(self):
-        return self.client.CloseSession(
-                qh_messages.CloseSessionRequest(close_request=qh_messages.CloseRequest(context_id=self.context_id)),
-                credentials=self.call_credentialds if self.use_ssl else None
-            ).close_response
-
     def _verify_open(self):
         """Verify that connection still open, reconnect if not."""
         if not self.connected:
             log_and_raise(ProgrammingError, 'The connection to the server has been closed')
         # TODO if channel or stub are not connected (how to check that?) reconnect
 
         if not self.session_opened:
             log_and_raise(ProgrammingError, 'Session has been closed')
-        # if self.expiration_time - time.time() * 1000 < 10000:
-        #     self.session_opened = False
-        #     self.connect_database(self.database, self.username, self.password, self.tenant_id, self.service, self.access_token)
+        if self.expiration_time - time.time() * 1000 < 10000:
+            self.session_opened = False
+            self.connect_database(self.database, self.username, self.password, self.tenant_id, self.service)
 
     def commit(self):
         return None
         # self._verify_open()
 
     def rollback(self):
         return None
```

### Comparing `pysqream-blue-1.0.27/pysqream_blue/cursor.py` & `pysqream-blue-1.0.3/pysqream_blue/cursor.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import grpc
-from pysqream_blue.globals import qh_messages, dbapi_typecodes, type_to_v1_tpye, type_to_letter
+from globals import qh_messages, dbapi_typecodes, type_to_v1_tpye, type_to_letter
 import time
-from pysqream_blue.logger import *
-from pysqream_blue.utils import NotSupportedError, ProgrammingError, InternalError, IntegrityError, OperationalError, DataError, \
-    DatabaseError, InterfaceError, Warning, Error, is_token_expired
+from logger import *
+from utils import NotSupportedError, ProgrammingError, InternalError, IntegrityError, OperationalError, DataError, \
+    DatabaseError, InterfaceError, Warning, Error
 from collections.abc import Sequence
 import json
-from pysqream_blue.casting import *
+from casting import *
 
 
 class Cursor:
 
     def __init__(self, client, context_id, query_timeout, call_credentialds, use_ssl):
 
         self.client = client
@@ -27,16 +27,16 @@
 
     def execute(self, query: str, params=None):
         ''' Execute a statement. Parameters are not supported '''
 
         # self._verify_open()
         if params:
             log_and_raise(NotSupportedError, "Parametered queries currently not supported.")
-        # if self.statement_opened:
-        #     self.close()
+        if self.statement_opened:
+            self.close()
 
         self._request_compile(query)
         self.statement_opened = True
         self._request_execute()
         self._request_status()
         self._prepare_result_set()
 
@@ -48,35 +48,26 @@
     def _request_cancel(self):
 
         if self.stmt_id is None:
             log_and_raise(ProgrammingError, "Context Id is not found")
 
         cancel_response = None
         try:
-            cancel_response: qh_messages.CancelResponse = self._cancel()
+            cancel_response: qh_messages.CancelResponse = self.client.Cancel(
+                qh_messages.CancelRequest(context_id=self.stmt_id))
         except grpc.RpcError as rpc_error:
             log_and_raise(ProgrammingError,
                           f'Context id: {self.stmt_id}. Error from grpc while attempting to cancel the query.\n{rpc_error}')
-            if is_token_expired(str(rpc_error)):
-                auth_response = self.client.auth_access_token()
-                self.client.token = auth_response.token
-                self.call_credentialds = grpc.access_token_call_credentials(self.client.token)
-                cancel_response: qh_messages.CancelResponse = self._cancel()
-
-            if cancel_response.HasField('error'):
-                log_and_raise(OperationalError,
-                              f'Context id: {self.stmt_id}. Error while attempting to cancel the query.\n{cancel_response.error}')
+        if cancel_response.HasField('error'):
+            log_and_raise(OperationalError,
+                          f'Context id: {self.stmt_id}. Error while attempting to cancel the query.\n{cancel_response.error}')
 
         log_info(f'Context id: {self.stmt_id}. The query was successfully canceled. query type: {self.query_type}.')
         return cancel_response
 
-    def _cancel(self):
-        return self.client.Cancel(
-                qh_messages.CancelRequest(context_id=self.stmt_id))
-
     def executemany(self, query: str, params: Sequence = None, data_as: str = 'rows'):
         if not params:
             return self.execute(query)
         if not isinstance(params, Sequence) or not isinstance(params[0], Sequence):
             log_and_raise(ProgrammingError,
                           f'Params to executemany() should be a sequence of sequence, got {type(params)}')
         log_and_raise(NotSupportedError, "Parametered queries currently not supported.")
@@ -84,146 +75,115 @@
     def fetchmany(self, size):
         size = size or self.arraysize
         # self._verify_open()
         if not self.statement_opened or self.query_type not in (None, qh_messages.QUERY_TYPE_QUERY):
             log_and_raise(ProgrammingError, 'No open statement while attempting fetch operation')
 
         while (size > len(self.parsed_rows) or size == -1) and self.more_to_fetch:
-            self._request_fetch()
+            self._fetch()
             self._parse()
 
         res = self.parsed_rows[: size if size != -1 else None]
         del self.parsed_rows[: size if size != -1 else None]
 
         if len(res):
             return res
 
-        return []
+        self.close()
+        return None
 
     def fetchone(self, bad_args=False):
         ''' Fetch one result row '''
 
         if bad_args:
             log_and_raise(ProgrammingError, "Bad argument to fetchone()")
 
-        res = self.fetchmany(1)
-        return None if not res else res
+        return self.fetchmany(1)
 
     def fetchall(self, bad_args=False):
         ''' Fetch all result rows '''
 
         if bad_args:
             log_and_raise(ProgrammingError, "Bad argument to fetchall()")
-
-        return self.fetchmany(-1)
+        res = self.fetchmany(-1)
+        self.close()
+        return res
 
     def get_statement_id(self):
         return self.stmt_id
 
     def _request_compile(self, query: str):
-        response: qh_messages.CompileResponse = None
         try:
-            response: qh_messages.CompileResponse = self._compile(query)
+            response: qh_messages.CompileResponse = self.client.Compile(
+                qh_messages.CompileRequest(context_id=self.context_id, sql=query.encode('utf8'), encoding='utf8',
+                                           query_timeout=self.query_timeout),
+                credentials=self.call_credentialds if self.use_ssl else None)
+            self.stmt_id, self.columns_metadata, self.query_type = response.context_id, response.columns, response.query_type
         except grpc.RpcError as rpc_error:
             log_and_raise(ProgrammingError,
                           f'Query: {query}. Error from grpc while attempting to compile the query.\n{rpc_error}')
-
-            if is_token_expired(str(rpc_error)):
-                auth_response = self.client.auth_access_token()
-                self.client.token = auth_response.token
-                self.call_credentialds = grpc.access_token_call_credentials(self.client.token)
-                response: qh_messages.CompileResponse = self._compile(query)
-
         if response.HasField('error'):
             log_and_raise(OperationalError,
                           f'Query: {query}. Error while attempting to compile the query.\n{response.error}')
 
         log_info(f'Query id: {self.stmt_id}. The query was successfully compiled. query type: {self.query_type}.')
 
-    def _compile(self, query):
-        response: qh_messages.CompileResponse = self.client.Compile(
-            qh_messages.CompileRequest(context_id=self.context_id, sql=query.encode('utf8'), encoding='utf8',
-                                       query_timeout=self.query_timeout),
-            credentials=self.call_credentialds if self.use_ssl else None)
-        self.stmt_id, self.columns_metadata, self.query_type = response.context_id, response.columns, response.query_type
-        return response
-
     def _request_execute(self):
-        execute_response = None
         try:
-            execute_response: qh_messages.ExecuteResponse = self._execute()
+            execute_response: qh_messages.ExecuteResponse = self.client.Execute(
+                qh_messages.ExecuteRequest(context_id=self.stmt_id),
+                credentials=self.call_credentialds if self.use_ssl else None)
         except grpc.RpcError as rpc_error:
             log_and_raise(ProgrammingError,
                           f'Query id: {self.stmt_id}. Error from grpc while attempting to execute the query.\n{rpc_error}')
-
-            if is_token_expired(str(rpc_error)):
-                auth_response = self.client.auth_access_token()
-                self.client.token = auth_response.token
-                self.call_credentialds = grpc.access_token_call_credentials(self.client.token)
-                execute_response: qh_messages.ExecuteResponse = self._execute()
-
         if execute_response.HasField('error'):
             log_and_raise(OperationalError,
                           f'Query id: {self.stmt_id}. Error while attempting to execute the query.\n{execute_response.error}')
 
         log_info(f'Query id: {self.stmt_id}. The query was send to execute successfully.')
 
-    def _execute(self):
-        return self.client.Execute(
-            qh_messages.ExecuteRequest(context_id=self.stmt_id),
-            credentials=self.call_credentialds if self.use_ssl else None)
-
     def _request_status(self):
 
         log_info(f'Query id: {self.stmt_id}. Wait for execution.')
         self.try_status_num = 0
         while True:
             status_response = None
             try:
-                status_response: qh_messages.StatusResponse = self._status()
+                status_response: qh_messages.StatusResponse = self.client.Status(
+                    qh_messages.StatusRequest(context_id=self.stmt_id),
+                    credentials=self.call_credentialds if self.use_ssl else None)
             except grpc.RpcError as rpc_error:
                 log_and_raise(ProgrammingError,
                               f'Query id: {self.stmt_id}. Error from grpc while attempting to get query status.\n{rpc_error}')
 
-                if is_token_expired(str(rpc_error)):
-                    auth_response = self.client.auth_access_token()
-                    self.client.token = auth_response.token
-                    self.call_credentialds = grpc.access_token_call_credentials(self.client.token)
-                    status_response: qh_messages.StatusResponse = self._status()
-
             if status_response.status == qh_messages.QUERY_EXECUTION_STATUS_ABORTED:
                 log_info(f"Query id {self.stmt_id} is aborted")
                 return
 
             if status_response.HasField('error'):
                 log_and_raise(OperationalError,
                               f'Query id: {self.stmt_id}. Error while attempting to get query status.\n{status_response.error}')
 
-            if status_response.status != qh_messages.QUERY_EXECUTION_STATUS_RUNNING and \
-                    status_response.status != qh_messages.QUERY_EXECUTION_STATUS_QUEUED:
+            if status_response.status != qh_messages.QUERY_EXECUTION_STATUS_RUNNING:
                 self.stmt_status = status_response.status
                 log_info(
                     f'Query id: {self.stmt_id}. status: {qh_messages.QueryExecutionStatus.Name(self.stmt_status)}.')
                 if self.stmt_status != qh_messages.QUERY_EXECUTION_STATUS_SUCCEEDED:
                     log_and_raise(OperationalError,
                                   f"Query id: {self.stmt_id}. Query execution failed with status: {qh_messages.QueryExecutionStatus.Name(self.stmt_status)}.")
                 return
             self._smart_sleep()
 
-    def _status(self):
-        return self.client.Status(
-                    qh_messages.StatusRequest(context_id=self.stmt_id),
-                    credentials=self.call_credentialds if self.use_ssl else None)
-
     def _prepare_result_set(self):
         '''Getting parameters for the cursor's 'description' attribute, even for
            a query that returns no rows. For each column, this includes:
            (name, type_code, display_size, internal_size, precision, scale, null_ok) '''
 
         if self.query_type == qh_messages.QUERY_TYPE_NON_QUERY:
+            self.close()
             return
         elif self.query_type != qh_messages.QUERY_TYPE_QUERY:
             log_and_raise(OperationalError, "Query id: {self.stmt_id}. Query type {self.query_type} is not supported")
 
         self.more_to_fetch = True
         self.parsed_rows = []
         self.rowcount = 0
@@ -235,28 +195,23 @@
                                    column.precision,
                                    column.scale,
                                    column.nullable))
                             for column in self.columns_metadata]
         self.column_list = [{'name': column.name, 'type': [type_to_v1_tpye[column.type], ]} for column in
                             self.columns_metadata]
 
-    def _request_fetch(self):
+    def _fetch(self):
         fetch_response = None
         try:
-            fetch_response: qh_messages.FetchResponse = self._fetch()
+            fetch_response: qh_messages.FetchResponse = self.client.Fetch(
+                qh_messages.FetchRequest(context_id=self.stmt_id),
+                credentials=self.call_credentialds if self.use_ssl else None)
         except grpc.RpcError as rpc_error:
             log_and_raise(ProgrammingError,
                           f'Query id: {self.stmt_id}. Error from grpc while attempting to fetch the results.\n{rpc_error}')
-
-            if is_token_expired(str(rpc_error)):
-                auth_response = self.client.auth_access_token()
-                self.client.token = auth_response.token
-                self.call_credentialds = grpc.access_token_call_credentials(self.client.token)
-                fetch_response: qh_messages.FetchResponse = self._fetch()
-
         if fetch_response.HasField('error'):
             log_and_raise(OperationalError,
                           f'Query id: {self.stmt_id}. Error while attempting to fetch the results.\n{fetch_response.error}')
 
         res_bytes = fetch_response.query_result
         header_size = int.from_bytes(res_bytes[:8], 'little')
         fetch_meta = json.loads(res_bytes[8:(8 + header_size)])
@@ -271,19 +226,14 @@
             res_bytes = res_bytes[size:]
 
         if not self.unparsed_row_amount:
             self.more_to_fetch = False
 
         log_info(f'Query id: {self.stmt_id}, {self.unparsed_row_amount} rows fetched.')
 
-    def _fetch(self):
-        return self.client.Fetch(
-                qh_messages.FetchRequest(context_id=self.stmt_id),
-                credentials=self.call_credentialds if self.use_ssl else None)
-
     def _parse(self):
         if not self.unparsed_row_amount:
             return
 
         self.data_columns = []
         for column_meta in self.columns_metadata:
             column = []
@@ -340,25 +290,22 @@
             self.parsed_rows.append(row)
 
         self.data_columns = []
         log_info(f'Query id: {self.stmt_id}, {self.parsed_row_amount} rows parsed.')
         self.parsed_row_amount = 0
 
     def close(self):
-        response: qh_messages.CloseResponse = None
         try:
-            response: qh_messages.CloseResponse = self._close()
+            response: qh_messages.CloseResponse = self.client.CloseStatement(
+                qh_messages.CloseStatementRequest(close_request=qh_messages.CloseRequest(context_id=self.stmt_id)),
+                credentials=self.call_credentialds if self.use_ssl else None
+            ).close_response
         except grpc.RpcError as rpc_error:
             log_error(f'Query id: {self.stmt_id}. Error from grpc while attempting to close the query.\n{rpc_error}')
-
-            if is_token_expired(str(rpc_error)):
-                auth_response = self.client.auth_access_token()
-                self.client.token = auth_response.token
-                self.call_credentialds = grpc.access_token_call_credentials(self.client.token)
-                response: qh_messages.CloseResponse = self._close()
+            return
 
         if response.HasField('error'):
             log_warning(f'Query id: {self.stmt_id}. Error while attempting to close the query.\n{response.error}')
             return
 
         log_info(f'Query id: {self.stmt_id}. The query was close successfully.')
 
@@ -368,20 +315,14 @@
         self.unparsed_row_amount = None
         self.unsorted_data_columns = None
         self.data_columns = None
 
         self.more_to_fetch = False
         self.statement_opened = False
 
-    def _close(self):
-        return self.client.CloseStatement(
-                qh_messages.CloseStatementRequest(close_request=qh_messages.CloseRequest(context_id=self.stmt_id)),
-                credentials=self.call_credentialds if self.use_ssl else None
-            ).close_response
-
     def _smart_sleep(self):
         ''' sleep for time grows up by number of tries '''
         self.try_status_num += 1
         time.sleep(min(self.try_status_num / 1000, 10))
 
     def nextset(self):
         ''' No multiple result sets so currently always returns None '''
```

### Comparing `pysqream-blue-1.0.27/pysqream_blue/globals.py` & `pysqream-blue-1.0.3/pysqream_blue/globals.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,13 @@
 import grpc
-# qh_messages, qh_services = grpc.protos_and_services("protos/queryhandler.proto")
-# auth_messages, auth_services = grpc.protos_and_services("protos/authentication.proto")
-# cl_messages, cl_services = grpc.protos_and_services("protos/client_info.proto")
-import protos.queryhandler_pb2 as qh_messages
-import protos.queryhandler_pb2_grpc as qh_services
-import protos.authentication_pb2 as auth_messages
-import protos.authentication_pb2_grpc as auth_services
-import protos.client_info_pb2 as cl_messages
-import protos.client_info_pb2_grpc as cl_services
-import protos.authentication_type_pb2 as auth_type_messages
+qh_messages, qh_services = grpc.protos_and_services("protos/queryhandler.proto")
+auth_messages, auth_services = grpc.protos_and_services("protos/authentication.proto")
+cl_messages, cl_services = grpc.protos_and_services("protos/client_info.proto")
 
-__version__ = '1.0.27'
+__version__ = '1.0.3'
 
 dbapi_typecodes = {
     qh_messages.COLUMN_TYPE_LONG_INT:  'NUMBER',
     qh_messages.COLUMN_TYPE_ULONG_INT: 'NUMBER',
     qh_messages.COLUMN_TYPE_INT:       'NUMBER',
     qh_messages.COLUMN_TYPE_UINT:      'NUMBER',
     qh_messages.COLUMN_TYPE_VARCHAR:   'STRING',
```

### Comparing `pysqream-blue-1.0.27/pysqream_blue/logger.py` & `pysqream-blue-1.0.3/pysqream_blue/logger.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from pysqream_blue.utils import NotSupportedError, ProgrammingError, InternalError, IntegrityError, OperationalError, DataError, \
+from utils import NotSupportedError, ProgrammingError, InternalError, IntegrityError, OperationalError, DataError, \
     DatabaseError, InterfaceError, Warning, Error
 
 logger = logging.getLogger("dbapi_logger")
 logger.setLevel(logging.DEBUG)
 logger.disabled = True
```

### Comparing `pysqream-blue-1.0.27/pysqream_blue/pysqream_blue.py` & `pysqream-blue-1.0.3/pysqream_blue/pysqream_blue.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,31 @@
-#!/usr/bin/env python3
-
 import time
 from datetime import datetime, date, time as t
-from pysqream_blue.connection import Connection
-# from pysqream_blue.connection import qh_messages
+from connection import Connection, qh_messages
+
 
-def connect(host:      str,
-            port:      str =  '443',
-            use_ssl:   bool = True,
+def connect(host:      str =  '127.0.0.1',
+            port:      str =  '80',
+            use_ssl:   bool = False,
             log              = False,
             database:  str =  'master',
             username:  str =  'sqream',
             password:  str =  'sqream',
             tenant_id: str =  'tenant',
             service:   str =  'sqream',
-            access_token: str = None,
             reconnect_attempts : int = 10,
             reconnect_interval : int = 3,
-            query_timeout      : int = 0,
-            pool_name: str = None
+            query_timeout      : int = 0
+
             ) -> Connection:
     ''' Connect to SQream database '''
 
     conn = Connection(host, port, use_ssl, log=log, is_base_connection=True, reconnect_attempts=reconnect_attempts,
-                      reconnect_interval=reconnect_interval, query_timeout=query_timeout, pool_name=pool_name)
-    conn.connect_database(database, username, password, tenant_id, service, access_token)
+                      reconnect_interval=reconnect_interval, query_timeout=query_timeout)
+    conn.connect_database(database, username, password, tenant_id, service)
 
     return conn
 
 
 
 ## DBapi compatibility
 #  -------------------
@@ -79,24 +76,24 @@
 
 threadsafety = 1 # Threads can share the module but not a connection
 
 paramstyle = 'qmark'
 
 
 # if __name__ == '__main__':
-#     con = connect(host='4_52.isqream.com', database='master')
+#     con = connect(host='192.168.4.4', database='master')
 #     query = None
 #     while (True):
 #         cursor = con.cursor()
 #         query = input(f'{con.database}=> ')
 #         if '\q' == query:
 #             break
 #         try:
 #             cursor.execute(query)
 #             if cursor.query_type == qh_messages.QUERY_TYPE_QUERY:
 #                 print(*(desc[0] for desc in cursor.description), sep=', ')
 #                 print(*cursor.fetchall() or [], sep="\n")
 #                 print(f'{cursor.rowcount} rows')
-#                 cursor.close()
 #         except Exception as e:
 #             print(e)
+#         cursor.close()
 #     con.close()
```

### Comparing `pysqream-blue-1.0.27/pysqream_blue.egg-info/PKG-INFO` & `pysqream-blue-1.0.3/pysqream_blue.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,70 +1,73 @@
 Metadata-Version: 2.1
 Name: pysqream-blue
-Version: 1.0.27
+Version: 1.0.3
 Summary: DB-API connector for SQream DB
 Home-page: https://github.com/SQream/pysqream-blue
 Author: SQream
 Author-email: info@sqream.com
 License: UNKNOWN
 Keywords: database db-api sqream sqreamdbV2
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.6.5
 Description-Content-Type: 
 ===================================
 Python connector for SQream DB Blue
 ===================================
 
-* **Version:**  1.0.27
+* **Version:**  1.0.10
 
 * **Supported SQream DB versions:** >= Blue cloud
 
 The Python connector for SQream DB is a Python DB API 2.0-compliant interface for developing Python applications with SQream DB.
 
 The SQream Python connector provides an interface for creating and running Python applications that can connect to a SQream DB database. It provides a lighter-weight alternative to working through native C++ or Java bindings, including JDBC and ODBC drivers.
 
 pysqream conforms to Python DB-API specifications `PEP-249 <https://www.python.org/dev/peps/pep-0249/>`_
 
-``pysqream_blue`` is native and pure Python, with minimal requirements. It can be installed with ``pip3`` on any operating system, including Linux, Windows, and macOS.
+``pysqream_blue`` is native and pure Python, with minimal requirements. It can be installed with ``pip`` on any operating system, including Linux, Windows, and macOS.
 
 .. For more information and a full API reference, see `SQream documentation's pysqream blue guide <https://sqream-docs.readthedocs.io/en/latest/guides/client_drivers/python/index.html>`_ .
 
 Requirements
 -------------
 
-* Python 3.9+
+* Python 3.6.5+, with 3.7+ highly recommended
 
 Installing the Python connector
 --------------------------------
 
 Prerequisites
 ----------------
 
 1. Python
 ^^^^^^^^^^^^
 
-The connector requires Python 3.9 or newer. To verify your version of Python:
+The connector requires Python 3.6.5 or newer. To verify your version of Python:
 
 .. code-block:: console
 
    $ python --version
-   Python 3.9
+   Python 3.7.3
+
+
+Note: If both Python 2.x and 3.x are installed, you can run ``python3`` and ``pip3`` instead of ``python`` and ``pip`` respectively for the rest of this guide
 
 2. PIP
 ^^^^^^^^^^^^
-The Python connector is installed via ``pip3``, the Python package manager and installer.
+The Python connector is installed via ``pip``, the Python package manager and installer.
 
-We recommend upgrading to the latest version of ``pip3`` before installing. To verify that you are on the latest version, run the following command:
+We recommend upgrading to the latest version of ``pip`` before installing. To verify that you are on the latest version, run the following command:
 
 .. code-block:: console
 
-   $ python -m pip3 install --upgrade pip
+   $ python -m pip install --upgrade pip
    Collecting pip
       Downloading https://files.pythonhosted.org/packages/00/b6/9cfa56b4081ad13874b0c6f96af8ce16cfbc1cb06bedf8e9164ce5551ec1/pip-19.3.1-py2.py3-none-any.whl (1.4MB)
         |████████████████████████████████| 1.4MB 1.6MB/s
    Installing collected packages: pip
      Found existing installation: pip 19.1.1
        Uninstalling pip-19.1.1:
          Successfully uninstalled pip-19.1.1
@@ -76,21 +79,21 @@
 
 
 Install via pip
 -----------------
 
 The Python connector is available via `PyPi <https://pypi.org/project/pysqream/>`_.
 
-Install the connector with ``pip3``:
+Install the connector with ``pip``:
 
 .. code-block:: console
 
-   $ pip3 install pysqream-blue
+   $ pip install pysqream-blue
 
-``pip3`` will automatically installs all necessary libraries and modules.
+``pip`` will automatically installs all necessary libraries and modules.
 
 Validate the installation
 -----------------------------
 
 Create a file called ``test.py`` (make sure to replace the parameters in the connection with the respective parameters for your SQream DB installation):
 
 .. code-block:: python
```

### Comparing `pysqream-blue-1.0.27/setup.py` & `pysqream-blue-1.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,20 +11,20 @@
     name =          'pysqream-blue',
     version =       __version__,
     description =   'DB-API connector for SQream DB', 
     long_description_content_type = long_description,
     url = "https://github.com/SQream/pysqream-blue",
     author = "SQream",
     author_email = "info@sqream.com",
-    packages = ["pysqream_blue", "protos"],
+    packages = find_packages(),
     classifiers = [
-        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.6",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
     ],
     keywords = 'database db-api sqream sqreamdbV2',
-    python_requires = '>=3.9',
+    python_requires = '>=3.6.5',
     install_requires=requires
 )
 
 if __name__ == '__main__':
     setup(**setup_params)
```

