# Comparing `tmp/dbmsbenchmarker-0.13.1.tar.gz` & `tmp/dbmsbenchmarker-0.13.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/DBMS-Benchmarker/DBMS-Benchmarker/dist/.tmp-v6y_1r22/dbmsbenchmarker-0.13.1.tar", last modified: Fri Mar  3 16:58:00 2023, max compression
+gzip compressed data, was "/home/runner/work/DBMS-Benchmarker/DBMS-Benchmarker/dist/.tmp-aoxblkjp/dbmsbenchmarker-0.13.2.tar", last modified: Tue Jun 20 13:09:44 2023, max compression
```

## Comparing `dbmsbenchmarker-0.13.1.tar` & `dbmsbenchmarker-0.13.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 16:58:00.000000 dbmsbenchmarker-0.13.1/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-03-03 16:57:48.000000 dbmsbenchmarker-0.13.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-03 16:57:48.000000 dbmsbenchmarker-0.13.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10743 2023-03-03 16:58:00.000000 dbmsbenchmarker-0.13.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-03-03 16:57:48.000000 dbmsbenchmarker-0.13.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 16:58:00.000000 dbmsbenchmarker-0.13.1/dbmsbenchmarker/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-03 16:57:48.000000 dbmsbenchmarker-0.13.1/dbmsbenchmarker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    92349 2023-03-03 16:57:48.000000 dbmsbenchmarker-0.13.1/dbmsbenchmarker/benchmarker.py
--rw-r--r--   0 runner    (1001) docker     (123)    34177 2023-03-03 16:57:48.000000 dbmsbenchmarker-0.13.1/dbmsbenchmarker/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    27618 2023-03-03 16:57:48.000000 dbmsbenchmarker-0.13.1/dbmsbenchmarker/inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)    22030 2023-03-03 16:57:48.000000 dbmsbenchmarker-0.13.1/dbmsbenchmarker/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    26162 2023-03-03 16:57:48.000000 dbmsbenchmarker-0.13.1/dbmsbenchmarker/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-03-03 16:57:48.000000 dbmsbenchmarker-0.13.1/dbmsbenchmarker/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16411 2023-03-03 16:57:48.000000 dbmsbenchmarker-0.13.1/dbmsbenchmarker/reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 16:58:00.000000 dbmsbenchmarker-0.13.1/dbmsbenchmarker/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-03 16:57:48.000000 dbmsbenchmarker-0.13.1/dbmsbenchmarker/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 16:58:00.000000 dbmsbenchmarker-0.13.1/dbmsbenchmarker/scripts/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 16:58:00.000000 dbmsbenchmarker-0.13.1/dbmsbenchmarker/scripts/assets/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-03-03 16:57:48.000000 dbmsbenchmarker-0.13.1/dbmsbenchmarker/scripts/assets/icons/check_box-24px.svg
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-03-03 16:57:48.000000 dbmsbenchmarker-0.13.1/dbmsbenchmarker/scripts/assets/icons/check_box_outline_blank-24px.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-03-03 16:57:48.000000 dbmsbenchmarker-0.13.1/dbmsbenchmarker/scripts/assets/icons/chevron_down.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-03-03 16:57:48.000000 dbmsbenchmarker-0.13.1/dbmsbenchmarker/scripts/assets/icons/chevron_up.svg
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-03-03 16:57:48.000000 dbmsbenchmarker-0.13.1/dbmsbenchmarker/scripts/assets/icons/clear-black-24dp.svg
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-03-03 16:57:48.000000 dbmsbenchmarker-0.13.1/dbmsbenchmarker/scripts/assets/icons/get_app-black-24dp.svg
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-03 16:57:48.000000 dbmsbenchmarker-0.13.1/dbmsbenchmarker/scripts/assets/icons/info-24px.svg
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-03 16:57:48.000000 dbmsbenchmarker-0.13.1/dbmsbenchmarker/scripts/assets/icons/radio_button_unchecked-24px.svg
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-03 16:57:48.000000 dbmsbenchmarker-0.13.1/dbmsbenchmarker/scripts/assets/icons/tune-black-24dp.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8214 2023-03-03 16:57:48.000000 dbmsbenchmarker-0.13.1/dbmsbenchmarker/scripts/assets/styles.css
--rw-r--r--   0 runner    (1001) docker     (123)     8793 2023-03-03 16:57:48.000000 dbmsbenchmarker-0.13.1/dbmsbenchmarker/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)   137208 2023-03-03 16:57:48.000000 dbmsbenchmarker-0.13.1/dbmsbenchmarker/scripts/dashboardcli.py
--rw-r--r--   0 runner    (1001) docker     (123)    75846 2023-03-03 16:57:48.000000 dbmsbenchmarker-0.13.1/dbmsbenchmarker/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 16:58:00.000000 dbmsbenchmarker-0.13.1/dbmsbenchmarker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10743 2023-03-03 16:58:00.000000 dbmsbenchmarker-0.13.1/dbmsbenchmarker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-03-03 16:58:00.000000 dbmsbenchmarker-0.13.1/dbmsbenchmarker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 16:58:00.000000 dbmsbenchmarker-0.13.1/dbmsbenchmarker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-03 16:58:00.000000 dbmsbenchmarker-0.13.1/dbmsbenchmarker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-03-03 16:58:00.000000 dbmsbenchmarker-0.13.1/dbmsbenchmarker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-03 16:58:00.000000 dbmsbenchmarker-0.13.1/dbmsbenchmarker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-03 16:58:00.000000 dbmsbenchmarker-0.13.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-03-03 16:57:48.000000 dbmsbenchmarker-0.13.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:09:44.000000 dbmsbenchmarker-0.13.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-20 13:09:32.000000 dbmsbenchmarker-0.13.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-20 13:09:32.000000 dbmsbenchmarker-0.13.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10743 2023-06-20 13:09:44.000000 dbmsbenchmarker-0.13.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-06-20 13:09:32.000000 dbmsbenchmarker-0.13.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:09:43.000000 dbmsbenchmarker-0.13.2/dbmsbenchmarker/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-20 13:09:32.000000 dbmsbenchmarker-0.13.2/dbmsbenchmarker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95197 2023-06-20 13:09:32.000000 dbmsbenchmarker-0.13.2/dbmsbenchmarker/benchmarker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36340 2023-06-20 13:09:32.000000 dbmsbenchmarker-0.13.2/dbmsbenchmarker/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27969 2023-06-20 13:09:32.000000 dbmsbenchmarker-0.13.2/dbmsbenchmarker/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22030 2023-06-20 13:09:32.000000 dbmsbenchmarker-0.13.2/dbmsbenchmarker/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28564 2023-06-20 13:09:32.000000 dbmsbenchmarker-0.13.2/dbmsbenchmarker/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-06-20 13:09:32.000000 dbmsbenchmarker-0.13.2/dbmsbenchmarker/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16756 2023-06-20 13:09:32.000000 dbmsbenchmarker-0.13.2/dbmsbenchmarker/reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:09:43.000000 dbmsbenchmarker-0.13.2/dbmsbenchmarker/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-20 13:09:32.000000 dbmsbenchmarker-0.13.2/dbmsbenchmarker/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:09:44.000000 dbmsbenchmarker-0.13.2/dbmsbenchmarker/scripts/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:09:44.000000 dbmsbenchmarker-0.13.2/dbmsbenchmarker/scripts/assets/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-20 13:09:32.000000 dbmsbenchmarker-0.13.2/dbmsbenchmarker/scripts/assets/icons/check_box-24px.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-20 13:09:32.000000 dbmsbenchmarker-0.13.2/dbmsbenchmarker/scripts/assets/icons/check_box_outline_blank-24px.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-20 13:09:32.000000 dbmsbenchmarker-0.13.2/dbmsbenchmarker/scripts/assets/icons/chevron_down.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-20 13:09:32.000000 dbmsbenchmarker-0.13.2/dbmsbenchmarker/scripts/assets/icons/chevron_up.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-20 13:09:32.000000 dbmsbenchmarker-0.13.2/dbmsbenchmarker/scripts/assets/icons/clear-black-24dp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-20 13:09:32.000000 dbmsbenchmarker-0.13.2/dbmsbenchmarker/scripts/assets/icons/get_app-black-24dp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-20 13:09:32.000000 dbmsbenchmarker-0.13.2/dbmsbenchmarker/scripts/assets/icons/info-24px.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-20 13:09:32.000000 dbmsbenchmarker-0.13.2/dbmsbenchmarker/scripts/assets/icons/radio_button_unchecked-24px.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-20 13:09:32.000000 dbmsbenchmarker-0.13.2/dbmsbenchmarker/scripts/assets/icons/tune-black-24dp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8214 2023-06-20 13:09:32.000000 dbmsbenchmarker-0.13.2/dbmsbenchmarker/scripts/assets/styles.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-06-20 13:09:32.000000 dbmsbenchmarker-0.13.2/dbmsbenchmarker/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)   137208 2023-06-20 13:09:32.000000 dbmsbenchmarker-0.13.2/dbmsbenchmarker/scripts/dashboardcli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77405 2023-06-20 13:09:32.000000 dbmsbenchmarker-0.13.2/dbmsbenchmarker/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:09:43.000000 dbmsbenchmarker-0.13.2/dbmsbenchmarker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10743 2023-06-20 13:09:43.000000 dbmsbenchmarker-0.13.2/dbmsbenchmarker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-20 13:09:43.000000 dbmsbenchmarker-0.13.2/dbmsbenchmarker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 13:09:43.000000 dbmsbenchmarker-0.13.2/dbmsbenchmarker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-20 13:09:43.000000 dbmsbenchmarker-0.13.2/dbmsbenchmarker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-20 13:09:43.000000 dbmsbenchmarker-0.13.2/dbmsbenchmarker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-20 13:09:43.000000 dbmsbenchmarker-0.13.2/dbmsbenchmarker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 13:09:44.000000 dbmsbenchmarker-0.13.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-20 13:09:32.000000 dbmsbenchmarker-0.13.2/setup.py
```

### Comparing `dbmsbenchmarker-0.13.1/LICENSE` & `dbmsbenchmarker-0.13.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbmsbenchmarker-0.13.1/PKG-INFO` & `dbmsbenchmarker-0.13.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbmsbenchmarker
-Version: 0.13.1
+Version: 0.13.2
 Summary: DBMS-Benchmarker is a Python-based application-level blackbox benchmark tool for Database Management Systems (DBMS). It connects to a given list of DBMS (via JDBC) and runs a given list of parametrized and randomized (SQL) benchmark queries. Evaluations are available via Python interface, in reports and at an interactive multi-dimensional dashboard.
 Home-page: https://github.com/Beuth-Erdelt/DBMS-Benchmarker
 Author: Patrick Erdelt
 Author-email: perdelt@beuth-hochschule.de
 License: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbmsbenchmarker Version: 0.13.1 Summary: DBMS-
+Metadata-Version: 2.1 Name: dbmsbenchmarker Version: 0.13.2 Summary: DBMS-
 Benchmarker is a Python-based application-level blackbox benchmark tool for
 Database Management Systems (DBMS). It connects to a given list of DBMS (via
 JDBC) and runs a given list of parametrized and randomized (SQL) benchmark
 queries. Evaluations are available via Python interface, in reports and at an
 interactive multi-dimensional dashboard. Home-page: https://github.com/Beuth-
 Erdelt/DBMS-Benchmarker Author: Patrick Erdelt Author-email: perdelt@beuth-
 hochschule.de License: GNU Affero General Public License v3 Classifier:
```

### Comparing `dbmsbenchmarker-0.13.1/README.md` & `dbmsbenchmarker-0.13.2/README.md`

 * *Files identical despite different names*

### Comparing `dbmsbenchmarker-0.13.1/dbmsbenchmarker/benchmarker.py` & `dbmsbenchmarker-0.13.2/dbmsbenchmarker/benchmarker.py`

 * *Files 1% similar despite different names*

```diff
@@ -351,15 +351,15 @@
 
 
 
 class benchmarker():
     """
     Class for running benchmarks
     """
-    def __init__(self, result_path=None, working='query', batch=False, fixedQuery=None, fixedConnection=None, rename_connection='', rename_alias='', fixedAlias='', anonymize=False, unanonymize=[], numProcesses=None, seed=None, code=None, subfolder=None):
+    def __init__(self, result_path=None, working='query', batch=False, fixedQuery=None, fixedConnection=None, rename_connection='', rename_alias='', fixedAlias='', anonymize=False, unanonymize=[], numProcesses=None, seed=None, code=None, subfolder=None, stream_id=None, stream_shuffle=None):
         """
         Construct a new 'benchmarker' object.
         Allocated the reporters store (always called) and printer (if reports are to be generated).
         A result folder is created if not existing already.
 
         :param result_path: Path for storing result files. If None is given, a folder is created using time.
         :param working: Process benchmarks query-wise or connection-wise
@@ -373,30 +373,41 @@
         :param code: Optional code for result folder
         :return: returns nothing
         """
         self.logger = logging.getLogger('benchmarker')
         if seed is not None:
             random.seed(seed)
         ## connection management:
-        self.connectionmanagement = {'numProcesses': numProcesses, 'runsPerConnection': None, 'timeout': None, 'singleConnection': True}
+        if numProcesses is not None:
+            # we cannot handle a single connection if there are multiple processes
+            singleConnection = False
+            numProcesses = int(numProcesses)
+        else:
+            # default is 1 connection per stream
+            singleConnection = True
+        self.connectionmanagement = {'numProcesses': numProcesses, 'runsPerConnection': None, 'timeout': None, 'singleConnection': singleConnection}
         # set number of parallel client processes
         #self.connectionmanagement['numProcesses'] = numProcesses
         if self.connectionmanagement['numProcesses'] is None:
             self.connectionmanagement['numProcesses'] = 1#math.ceil(mp.cpu_count()/2) #If None, half of all available processes is taken
-        else:
-            self.connectionmanagement['numProcesses'] = int(self.numProcesses)
+        #else:
+        #    self.connectionmanagement['numProcesses'] = int(self.numProcesses)
         # connection should be renamed (because of copy to subfolder and parallel processing)
         # also rename alias
         self.rename_connection = rename_connection
         self.rename_alias = rename_alias    # what alias is supposed to be renamed to
         self.fixedAlias = fixedAlias        # what alias is in connection file
         # for connections staying active for all benchmarks
         self.activeConnections = []
         #self.runsPerConnection = 4
         #self.timeout = 600
+        # number of stream, in particular for parallel streams
+        # None = ignore this
+        self.stream_id = stream_id
+        self.stream_shuffle = stream_shuffle
         # there is no general pool
         self.pool = None
         # store number of cpu cores
         self.num_cpu = mp.cpu_count()
         # printer is first and fixed reporter
         self.reporter = [reporter.printer(self)]
         # store is fixed reporter and cannot be removed
@@ -642,14 +653,21 @@
             if self.anonymize and not c['name'] in self.unanonymize:
                 # this dbms shoud be anonymized
                 anonymous = True
             else:
                 anonymous = False
             self.dbms[c['name']] = tools.dbms(c, anonymous)
         #self.connectDBMSAll()
+    def store_connectiondata(self):
+        connections_content = []
+        for key, dbms in self.dbms.items():
+            connections_content.append(dbms.connectiondata)
+        #with open(self.path+'/connections_copy.config', "w") as connections_file:
+        with open(self.path+'/connections.config', "w") as connections_file:
+            connections_file.write(str(connections_content))
     def connectDBMSAll(self):
         """
         Connects to all dbms we have collected connection data of.
 
         :return: returns nothing
         """
         for c in sorted(self.dbms.keys()):
@@ -880,14 +898,16 @@
                 numProcesses = connectionmanagement['numProcesses']
             if('runsPerConnection' in connectionmanagement):# and connectionmanagement['runsPerConnection'] != 0):
                 # 0=unlimited
                 batchsize = connectionmanagement['runsPerConnection']
             if('timeout' in connectionmanagement):# and connectionmanagement['timeout'] != 0):
                 # 0=unlimited
                 timeout = connectionmanagement['timeout']
+            if('singleConnection' in connectionmanagement):# and connectionmanagement['timeout'] != 0):
+                singleConnection = connectionmanagement['singleConnection']
         if numProcesses == 0 or numProcesses is None:
             numProcesses = 1
         if timeout == 0:
             timeout = None
         if batchsize == 0 or batchsize is None:
             batchsize = math.ceil(query.numRun/numProcesses)
         # unless pickling of java objects is possible
@@ -1002,14 +1022,16 @@
         # connection management for parallel connections
         connectionmanagement = self.getConnectionManager(numQuery, c)
         numProcesses = connectionmanagement['numProcesses']#self.numProcesses
         batchsize = connectionmanagement['runsPerConnection']#self.runsPerConnection
         timeout = connectionmanagement['timeout']#self.timeout
         if timeout is not None:
             jaydebeapi.QUERY_TIMEOUT = timeout
+        if self.stream_id is not None:
+            parameter.defaultParameters['STREAM'] = self.stream_id
         singleConnection = connectionmanagement['singleConnection']
         # overwrite by connection
         #if 'connectionmanagement' in self.dbms[c].connectiondata:
         #   connectionmanagement = self.dbms[c].connectiondata['connectionmanagement']
         #   if('numProcesses' in connectionmanagement and connectionmanagement['numProcesses'] != 0):
         #       numProcesses = self.dbms[c].connectiondata['connectionmanagement']['numProcesses']
         #   if('runsPerConnection' in connectionmanagement):# and connectionmanagement['runsPerConnection'] != 0):
@@ -1133,20 +1155,33 @@
                 if self.pool is not None:
                     self.logger.info("POOL of query senders (global pool)")
                     #multiple_results = [self.pool.apply_async(singleRun, (self.dbms[c].connectiondata, inputConfig, runs[i*batchsize:(i+1)*batchsize], connectionname, numQuery, self.path, JPickler.dumps(self.activeConnections))) for i in range(numBatches)]
                     multiple_results = [self.pool.apply_async(singleRun, (self.dbms[c].connectiondata, inputConfig, runs[i*batchsize:(i+1)*batchsize], connectionname, numQuery, self.path, [], BENCHMARKER_VERBOSE_QUERIES, BENCHMARKER_VERBOSE_RESULTS, BENCHMARKER_VERBOSE_PROCESS)) for i in range(numBatches)]
                     lists = [res.get(timeout=timeout) for res in multiple_results]
                     lists = [i for j in lists for i in j]
                 else:
+                    """
                     with mp.Pool(processes=numProcesses) as pool:
                         self.logger.info("POOL of query senders (local pool)")
                         #multiple_results = [pool.apply_async(singleRun, (self.dbms[c].connectiondata, inputConfig, runs[i*batchsize:(i+1)*batchsize], connectionname, numQuery, self.path, JPickler.dumps(self.activeConnections))) for i in range(numBatches)]
                         multiple_results = [pool.apply_async(singleRun, (self.dbms[c].connectiondata, inputConfig, runs[i*batchsize:(i+1)*batchsize], connectionname, numQuery, self.path, [], BENCHMARKER_VERBOSE_QUERIES, BENCHMARKER_VERBOSE_RESULTS, BENCHMARKER_VERBOSE_PROCESS)) for i in range(numBatches)]
                         lists = [res.get(timeout=timeout) for res in multiple_results]
                         lists = [i for j in lists for i in j]
+                        pool.close()
+                    """
+                    with mp.Pool(processes=numProcesses) as pool:
+                        self.logger.info("POOL of query senders (local pool starmap)")
+                        #multiple_results = [pool.apply_async(singleRun, (self.dbms[c].connectiondata, inputConfig, runs[i*batchsize:(i+1)*batchsize], connectionname, numQuery, self.path, JPickler.dumps(self.activeConnections))) for i in range(numBatches)]
+                        args = [(self.dbms[c].connectiondata, inputConfig, runs[i*batchsize:(i+1)*batchsize], connectionname, numQuery, self.path, [], BENCHMARKER_VERBOSE_QUERIES, BENCHMARKER_VERBOSE_RESULTS, BENCHMARKER_VERBOSE_PROCESS) for i in range(numBatches)]
+                        multiple_results = pool.starmap_async(singleRun, args)
+                        lists = multiple_results.get(timeout=timeout)
+                        #lists = [res.get(timeout=timeout) for res in multiple_results]
+                        lists = [i for j in lists for i in j]
+                        pool.close()
+                        pool.join()
             else:
                 # no parallel processes because JVM does not parallize
                 # time the queries and stop early if maxTime is reached
                 if BENCHMARKER_VERBOSE_PROCESS:
                     self.logger.info("We have {} active connections".format(len(self.activeConnections)))
                 start_time_queries = default_timer()
                 lists = []
@@ -1390,18 +1425,21 @@
                     if('singleConnection' in connectionmanagement):# and connectionmanagement['timeout'] != 0):
                         singleConnection = connectionmanagement['singleConnection']
                 if singleConnection:
                     # we assume all queries should share a connection
                     numProcesses = 1
                     i = 0
                     #connectionname = c
-                    print("More active connections from {} to {} for {}".format(len(self.activeConnections), numProcesses, connectionname))
-                    self.activeConnections.append(tools.dbms(self.dbms[connectionname].connectiondata))
-                    print("Establish global connection #"+str(i))
-                    self.activeConnections[i].connect()
+                    if (self.fixedQuery is not None and self.fixedQuery != numQuery) or (self.fixedConnection is not None and self.fixedConnection != connectionname):
+                        continue
+                    else:
+                        print("More active connections from {} to {} for {}".format(len(self.activeConnections), numProcesses, connectionname))
+                        self.activeConnections.append(tools.dbms(self.dbms[connectionname].connectiondata))
+                        print("Establish global connection #"+str(i))
+                        self.activeConnections[i].connect()
                 # run benchmark, current query and connection
                 bBenchmarkDoneForThisQuery = self.runBenchmark(numQuery, connectionname)
                 # close global connection
                 if singleConnection:
                     print("Closed connection for", connectionname)
                     self.activeConnections[i].disconnect()
                     self.activeConnections = []
@@ -1429,18 +1467,21 @@
                 if('singleConnection' in connectionmanagement):# and connectionmanagement['timeout'] != 0):
                     singleConnection = connectionmanagement['singleConnection']
             if singleConnection:
                 # we assume all queries should share a connection
                 numProcesses = 1
                 i = 0
                 #connectionname = c
-                print("More active connections from {} to {} for {}".format(len(self.activeConnections), numProcesses, connectionname))
-                self.activeConnections.append(tools.dbms(self.dbms[connectionname].connectiondata))
-                print("Establish global connection #"+str(i))
-                self.activeConnections[i].connect()
+                if (self.fixedConnection is not None and self.fixedConnection != connectionname):
+                    continue
+                else:
+                    print("More active connections from {} to {} for {}".format(len(self.activeConnections), numProcesses, connectionname))
+                    self.activeConnections.append(tools.dbms(self.dbms[connectionname].connectiondata))
+                    print("Establish global connection #"+str(i))
+                    self.activeConnections[i].connect()
             #print(self.activeConnections)
             # work queries
             ordered_list_of_queries = range(1, len(self.queries)+1)
             for numQuery in ordered_list_of_queries:
                 bBenchmarkDone = self.runBenchmark(numQuery, connectionname)
                 # if benchmark has been done: store and generate reports
                 if bBenchmarkDone:
@@ -1483,17 +1524,19 @@
         # log time of ending benchmark
         time_now = str(datetime.datetime.now())
         time_now_int = int(datetime.datetime.timestamp(datetime.datetime.strptime(time_now,'%Y-%m-%d %H:%M:%S.%f')))
         self.time_end = time_now_int
         self.logger.debug("### Time end: "+str(self.time_end))
         for connectionname in sorted(self.dbms.keys()):
             self.protocol['total'][connectionname]['time_end'] = self.time_end
-        print("DBMSBenchmarker duration: "+str(self.time_end-self.time_start))
+        print("DBMSBenchmarker duration: {} [s]".format(self.time_end-self.time_start))
         # write protocol again
         self.reporterStore.writeProtocol()
+        # store connection data again, it may have changed
+        self.store_connectiondata()
         if self.bBatch:
             # generate reports at the end only
             self.generateReportsAll()
         # stop logging multiprocessing
         mp.log_to_stderr(logging.ERROR)
     def readResultfolder(self):
         """
```

### Comparing `dbmsbenchmarker-0.13.1/dbmsbenchmarker/evaluator.py` & `dbmsbenchmarker-0.13.2/dbmsbenchmarker/evaluator.py`

 * *Files 4% similar despite different names*

```diff
@@ -214,32 +214,46 @@
                             time = times[c]
                         evaluation['dbms'][c]['prices']['perHour_usd'] = self.benchmarker.dbms[c].connectiondata['priceperhourdollar']
                         evaluation['dbms'][c]['prices']['benchmark_usd'] = self.benchmarker.dbms[c].connectiondata['priceperhourdollar']*time/3600000
                 if self.benchmarker.dbms[c].hasHardwareMetrics():
                     evaluation['dbms'][c]['hardwaremetrics'] = {}
                     evaluation['general']['loadingmetrics'] = {}
                     evaluation['general']['streamingmetrics'] = {}
+                    evaluation['general']['loadermetrics'] = {}
+                    evaluation['general']['benchmarkermetrics'] = {}
+                    evaluation['general']['datageneratormetrics'] = {}
                     metricsReporter = monitor.metrics(self.benchmarker)
                     hardwareAverages = metricsReporter.computeAverages()
                     if c in hardwareAverages:
                         for m, avg in hardwareAverages[c].items():
                             evaluation['dbms'][c]['hardwaremetrics'][m] = avg
                         if 'total_gpu_power' in hardwareAverages[c]:
                             # basis: per second average power, total time in ms
                             evaluation['dbms'][c]['hardwaremetrics']['total_gpu_energy'] = hardwareAverages[c]['total_gpu_power']*times[c]/3600000
-                        # load test metrics
                         for m, avg in hardwareAverages[c].items():
+                            # load test metrics
                             df = metricsReporter.dfHardwareMetricsLoading(m)
                             df.drop_duplicates(inplace=True) # TODO: Why are there duplicates sometimes?
                             evaluation['general']['loadingmetrics'][m] = df.to_dict(orient='index')
-                        # load streaming metrics
-                        for m, avg in hardwareAverages[c].items():
+                            # streaming metrics
                             df = metricsReporter.dfHardwareMetricsStreaming(m)
                             df.drop_duplicates(inplace=True) # TODO: Why are there duplicates sometimes?
                             evaluation['general']['streamingmetrics'][m] = df.to_dict(orient='index')
+                            # loader metrics
+                            df = metricsReporter.dfHardwareMetricsLoader(m)
+                            df.drop_duplicates(inplace=True) # TODO: Why are there duplicates sometimes?
+                            evaluation['general']['loadermetrics'][m] = df.to_dict(orient='index')
+                            # benchmarker metrics
+                            df = metricsReporter.dfHardwareMetricsBenchmarker(m)
+                            df.drop_duplicates(inplace=True) # TODO: Why are there duplicates sometimes?
+                            evaluation['general']['benchmarkermetrics'][m] = df.to_dict(orient='index')
+                            #  datagenerator metrics
+                            df = metricsReporter.dfHardwareMetricsDatagenerator(m)
+                            df.drop_duplicates(inplace=True) # TODO: Why are there duplicates sometimes?
+                            evaluation['general']['datageneratormetrics'][m] = df.to_dict(orient='index')
         # appendix start: query survey
         evaluation['query'] = {}
         for i in range(1, len(self.benchmarker.queries)+1):
             evaluation['query'][i] = {}
             evaluation['query'][i]['config'] = self.benchmarker.queries[i-1]
             queryObject = tools.query(self.benchmarker.queries[i-1])
             evaluation['query'][i]['title'] = queryObject.title
@@ -597,7 +611,28 @@
 def dfStreamingMetric(evaluation, metric):
     if 'streamingmetrics' in evaluation['general'] and metric in evaluation['general']['streamingmetrics']:
         df = pd.DataFrame.from_dict(evaluation['general']['streamingmetrics'][metric]).transpose()
         df.index.name = 'DBMS'
     else:
         df = pd.DataFrame()
     return df
+def dfLoaderMetric(evaluation, metric):
+    if 'loadermetrics' in evaluation['general'] and metric in evaluation['general']['loadermetrics']:
+        df = pd.DataFrame.from_dict(evaluation['general']['loadermetrics'][metric]).transpose()
+        df.index.name = 'DBMS'
+    else:
+        df = pd.DataFrame()
+    return df
+def dfBenchmarkerMetric(evaluation, metric):
+    if 'benchmarkermetrics' in evaluation['general'] and metric in evaluation['general']['benchmarkermetrics']:
+        df = pd.DataFrame.from_dict(evaluation['general']['benchmarkermetrics'][metric]).transpose()
+        df.index.name = 'DBMS'
+    else:
+        df = pd.DataFrame()
+    return df
+def dfDatageneratorMetric(evaluation, metric):
+    if 'datageneratormetrics' in evaluation['general'] and metric in evaluation['general']['datageneratormetrics']:
+        df = pd.DataFrame.from_dict(evaluation['general']['datageneratormetrics'][metric]).transpose()
+        df.index.name = 'DBMS'
+    else:
+        df = pd.DataFrame()
+    return df
```

### Comparing `dbmsbenchmarker-0.13.1/dbmsbenchmarker/inspector.py` & `dbmsbenchmarker-0.13.2/dbmsbenchmarker/inspector.py`

 * *Files 2% similar despite different names*

```diff
@@ -444,14 +444,20 @@
                 else:
                     break
         return script
     def get_loading_metrics(self, metric):
         return evaluator.dfLoadingMetric(self.e.evaluation, metric)
     def get_streaming_metrics(self, metric):
         return evaluator.dfStreamingMetric(self.e.evaluation, metric)
+    def get_loader_metrics(self, metric):
+        return evaluator.dfLoaderMetric(self.e.evaluation, metric)
+    def get_benchmarker_metrics(self, metric):
+        return evaluator.dfBenchmarkerMetric(self.e.evaluation, metric)
+    def get_datagenerator_metrics(self, metric):
+        return evaluator.dfDatageneratorMetric(self.e.evaluation, metric)
     def get_total_resultsize_normalized(self):
         return tools.dataframehelper.evaluateNormalizedResultsizeToDataFrame(self.e.evaluation).T
     def get_total_resultsize(self):
         return tools.dataframehelper.evaluateResultsizeToDataFrame(self.e.evaluation).T
     def get_total_errors(self):
         return tools.dataframehelper.evaluateErrorsToDataFrame(self.e.evaluation).T
     def get_total_warnings(self):
```

### Comparing `dbmsbenchmarker-0.13.1/dbmsbenchmarker/layout.py` & `dbmsbenchmarker-0.13.2/dbmsbenchmarker/layout.py`

 * *Files identical despite different names*

### Comparing `dbmsbenchmarker-0.13.1/dbmsbenchmarker/monitor.py` & `dbmsbenchmarker-0.13.2/dbmsbenchmarker/monitor.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,45 +101,58 @@
     m_avg = None
     def __init__(self, benchmarks):
         self.step = 1
         self.benchmarker = benchmarks
     @staticmethod
     def getMetrics(url, metric, time_start, time_end, step=1):
         logging.debug("getMetrics from "+url)
-        query = 'query_range'#?query='+metric['query']+'&start='+str(time_start)+'&end='+str(time_end)+'&step='+str(self.step)
-        params = {
-            'query': metric['query'],
-            'start': str(time_start),
-            'end': str(time_end),
-            'step': str(step),
-        }
-        logging.debug("Querying metrics: "+url+query, params)
-        logging.debug(params)
-        #headers = {'Authorization': self.token}
-        l = [(t,0) for t in range(time_start, time_end+1)]#[(time_start,0)]
-        #return l
-        #print(self.url+query)
-        try:
-            #r = requests.post(self.url+query)#, headers=headers)
-            r = requests.get(url+query, params=params)#, headers=headers)
-            #print(r.json())
-            if isinstance(r.json(), dict) and 'data' in r.json() and 'result' in r.json()['data'] and len(r.json()['data']['result']) > 0:
-                l = r.json()['data']['result'][0]['values']
-                # missing values due to end of monitoring?
-                n = time_end-time_start-len(l)+1
-                l2 = [(t+len(l)+time_start, 0) for t in range(n)]
-                l = l + l2
-            else:
-                #print(metric, url+query, r.json())
-                l = [(t,0) for t in range(time_start, time_end+1)]#[(time_start,0)]
-                logging.error('Metrics missing: '+url+query, params)
-                logging.error(r.text)
-        except Exception as e:
-            logging.exception('Caught an error: %s' % str(e))
-        return l
+        def fetch_interval(time_start, time_end, step):
+            query = 'query_range'#?query='+metric['query']+'&start='+str(time_start)+'&end='+str(time_end)+'&step='+str(self.step)
+            params = {
+                'query': metric['query'],
+                'start': str(time_start),
+                'end': str(time_end),
+                'step': str(step),
+            }
+            logging.debug("Querying metrics: "+url+query, params)
+            logging.debug(params)
+            #headers = {'Authorization': self.token}
+            l = [(t,0) for t in range(time_start, time_end+1)]#[(time_start,0)]
+            #return l
+            #print(self.url+query)
+            try:
+                #r = requests.post(self.url+query)#, headers=headers)
+                r = requests.get(url+query, params=params)#, headers=headers)
+                #print(r.json())
+                if isinstance(r.json(), dict) and 'data' in r.json() and 'result' in r.json()['data'] and len(r.json()['data']['result']) > 0:
+                    l = r.json()['data']['result'][0]['values']
+                    # missing values due to end of monitoring?
+                    n = time_end-time_start-len(l)+1
+                    l2 = [(t+len(l)+time_start, 0) for t in range(n)]
+                    l = l + l2
+                else:
+                    #print(metric, url+query, r.json())
+                    l = [(t,0) for t in range(time_start, time_end+1)]#[(time_start,0)]
+                    logging.error('Metrics missing: '+url+query, params)
+                    logging.error(r.text)
+            except Exception as e:
+                logging.exception('Caught an error: %s' % str(e))
+            return l
+        # split the time span into max 9000s intervals
+        list_values = []
+        max_span_len = 9000
+        span = time_end - time_start
+        intervals = span//max_span_len+1
+        for i in range(0, intervals):
+            time_interval_start = i*9000 + time_start
+            time_interval_end = min((i+1)*9000-1, span) + time_start
+            print("Fetch metric interval {} to {} = {} s span".format(time_interval_start, time_interval_end, time_interval_end - time_interval_start))
+            list_values_interval = fetch_interval(time_interval_start, time_interval_end, step)
+            list_values = list_values + list_values_interval
+        return list_values
     @staticmethod
     def metricsToDataframe(metric, values):
         df = pd.DataFrame.from_records(values)
         df.columns = ['time [s]', metric['title']]
         df.iloc[0:,0] = df.iloc[0:,0].map(int)
         minimum = df.iloc[0:,0].min()
         df.iloc[0:,0] = df.iloc[0:,0].map(lambda x: x-minimum)
@@ -180,15 +193,15 @@
                 numPlots = numPlots + 1
         if numPlots > 0:
             latex += "\\caption{{Query {queryNumber}: Server Hardware Metrics}}\\end{{figure}}"
             return latex.format(**parameter)
         else:
             return ""
     @staticmethod
-    def fetchMetric(query, metric_code, connection, connectiondata, time_start, time_end, path):
+    def fetchMetric(query, metric_code, connection, connectiondata, time_start, time_end, path, container=None):
         #for m, metric in metrics.metrics.items():
         logging.debug("Metric "+metric_code)
         df_all = None
         #for c,t in times["starts"].items():
         if 'monitoring' in connectiondata:
             #self.token = self.benchmarker.dbms[c].connectiondata['monitoring']['grafanatoken']
             #self.url = self.benchmarker.dbms[c].connectiondata['monitoring']['grafanaurl']
@@ -196,16 +209,22 @@
             url = connectiondata['monitoring']['prometheus_url']
             if connectiondata['active'] and url: #
                 logging.debug("Connection "+connection)
                 # is there a custom query for this metric and dbms?
                 if 'metrics' in connectiondata['monitoring'] and metric_code in connectiondata['monitoring']['metrics']:
                     metric = connectiondata['monitoring']['metrics'][metric_code].copy()
                 else:
-                    metric = metrics.metrics[metric_code]
+                    metric = metrics.metrics[metric_code].copy()
                 #print(metric)
+                if container is not None:
+                    metric['query'] = metric['query'].replace('container_label_io_kubernetes_container_name="dbms"', 'container_label_io_kubernetes_container_name="{}"'.format(container))
+                    metric['query'] = metric['query'].replace('container_label_io_kubernetes_container_name!="dbms"', 'container_label_io_kubernetes_container_name!="{}"'.format(container))
+                    # open TODO:
+                    # container_label_component="worker"
+                    # container_label_component="sut"
                 # this yields seconds
                 # is there a global timeshift
                 if 'grafanashift' in connectiondata['monitoring']:
                     time_shift = connectiondata['monitoring']['grafanashift']
                 elif 'shift' in connectiondata['monitoring']:
                     time_shift = connectiondata['monitoring']['shift']
                 else:
@@ -403,41 +422,54 @@
         #    #print(c)
         #    #print(df_all[c])
         #    #df_all[c] = list(df_all[c])[add_interval:-add_interval].extend([0]*(2*add_interval))
         # take last extend value
         #df_all = df_all.iloc[add_interval:-add_interval]
         #print(df_all)
         return df_all.T
+    def dfHardwareMetricsLoader(self, metric):
+        return self.dfHardwareMetricsComponentOriginal(metric, component="loader")
+    def dfHardwareMetricsBenchmarker(self, metric):
+        return self.dfHardwareMetricsComponentOriginal(metric, component="benchmarker")
+    def dfHardwareMetricsDatagenerator(self, metric):
+        return self.dfHardwareMetricsComponentOriginal(metric, component="datagenerator")
     def dfHardwareMetricsLoading(self, metric):
-        filename = self.benchmarker.path+'/query_loading_metric_'+str(metric)+'.csv'
+        return self.dfHardwareMetricsComponentOriginal(metric, component="loading")
+    def dfHardwareMetricsComponentOriginal(self, metric, component="loading"):
+        #filename = self.benchmarker.path+'/query_loading_metric_'+str(metric)+'.csv'
+        filename = "{path}/query_{component}_metric_{metric}.csv".format(path=self.benchmarker.path, component=component, metric=metric)
         #print(filename)
         if os.path.isfile(filename) and not self.benchmarker.overwrite:
             df_all = metrics.loadMetricsDataframe(filename)
         else:
             df_all = None
         if df_all is None:
             dbms_filter = self.benchmarker.dbms.keys()#self.benchmarker.protocol['query'][str(numQuery)]["starts"].keys()
             for c in dbms_filter:
                 # load metrics are fetched before possibly renaming connection
                 if 'orig_name' in self.benchmarker.dbms[c].connectiondata:
                     connectionname = self.benchmarker.dbms[c].connectiondata['orig_name']
                 else:
                     connectionname = c
                 #print(connectionname, df_all)
-                filename = self.benchmarker.path+'/query_loading_metric_'+str(metric)+'_'+connectionname+'.csv'
-                df = metrics.loadMetricsDataframe(filename)
+                if df_all is not None and connectionname in df_all.columns:
+                    print("We already have the metrics of this instance {c} as {connectionname}".format(c=c, connectionname=connectionname))
+                    continue
+                filename_component = "{path}/query_{component}_metric_{metric}_{connectionname}.csv".format(path=self.benchmarker.path, component=component, metric=metric, connectionname=connectionname)
+                #filename = self.benchmarker.path+'/query_loading_metric_'+str(metric)+'_'+connectionname+'.csv'
+                df = metrics.loadMetricsDataframe(filename_component)
                 if df is None:
                     continue
                 df.columns=[connectionname]
                 if df_all is None:
                     df_all = df
                 else:
                     # produces suffixes because of duplicate columns 
                     df_all = df_all.merge(df, how='outer', left_index=True,right_index=True)
-            filename = self.benchmarker.path+'/query_loading_metric_'+str(metric)+'.csv'
+            #filename = self.benchmarker.path+'/query_loading_metric_'+str(metric)+'.csv'
             metrics.saveMetricsDataframe(filename, df_all)
         if df_all is None:
             return pd.DataFrame()
         # remove connection delay (metrics are collected, but nothing happens here)
         #query = tools.query(self.benchmarker.queries[numQuery-1])
         #df_all = df_all.iloc[int(query.delay_connect):]
         #print(df_all)
@@ -450,53 +482,42 @@
         #    #df_all[c] = list(df_all[c])[add_interval:-add_interval].extend([0]*(2*add_interval))
         # take last extend value
         #df_all = df_all.iloc[add_interval:-add_interval]
         #print(df_all)
         #print(df_all)
         return df_all.T
     def dfHardwareMetricsStreaming(self, metric):
-        filename = self.benchmarker.path+'/query_stream_metric_'+str(metric)+'.csv'
+        return self.dfHardwareMetricsComponentOriginal(metric, component="stream")
+    def dfHardwareMetricsComponent(self, metric, component="stream"):
+        filename = "{path}/query_{component}_metric_{metric}.csv".format(path=self.benchmarker.path, component=component, metric=metric)
+        #filename = self.benchmarker.path+'/query_stream_metric_'+str(metric)+'.csv'
         #print(filename)
         if os.path.isfile(filename) and not self.benchmarker.overwrite:
             df_all = metrics.loadMetricsDataframe(filename)
         else:
             df_all = None
         if df_all is None:
             dbms_filter = self.benchmarker.dbms.keys()#self.benchmarker.protocol['query'][str(numQuery)]["starts"].keys()
             for c in dbms_filter:
                 connectionname = c
                 #print(connectionname, df_all)
-                filename = self.benchmarker.path+'/query_stream_metric_'+str(metric)+'_'+connectionname+'.csv'
-                df = metrics.loadMetricsDataframe(filename)
+                filename_component = "{path}/query_{component}_metric_{metric}_{connectionname}.csv".format(path=self.benchmarker.path, component=component, metric=metric, connectionname=connectionname)
+                #filename = self.benchmarker.path+'/query_stream_metric_'+str(metric)+'_'+connectionname+'.csv'
+                df = metrics.loadMetricsDataframe(filename_component)
                 if df is None:
                     continue
                 df.columns=[connectionname]
                 if df_all is None:
                     df_all = df
                 else:
                     df_all = df_all.merge(df, how='outer', left_index=True,right_index=True)
-            filename = self.benchmarker.path+'/query_stream_metric_'+str(metric)+'.csv'
+            #filename = self.benchmarker.path+'/query_stream_metric_'+str(metric)+'.csv'
             metrics.saveMetricsDataframe(filename, df_all)
         if df_all is None:
             return pd.DataFrame()
-        # remove connection delay (metrics are collected, but nothing happens here)
-        #query = tools.query(self.benchmarker.queries[numQuery-1])
-        #df_all = df_all.iloc[int(query.delay_connect):]
-        #print(df_all)
-        # remove extend
-        #for c, connection in self.benchmarker.dbms.items():
-        #    add_interval = int(connection.connectiondata['monitoring']['grafanaextend'])
-        #    #print(add_interval)
-        #    #print(c)
-        #    #print(df_all[c])
-        #    #df_all[c] = list(df_all[c])[add_interval:-add_interval].extend([0]*(2*add_interval))
-        # take last extend value
-        #df_all = df_all.iloc[add_interval:-add_interval]
-        #print(df_all)
-        #print(df_all)
         return df_all.T
 
 def clean_dataframe(dataframe):
     # helps evaluating GPU util
     # removes leading zeros in each row
     # shifts values > 0 to the beginning
     # appends NaN to keep numbers of columns the same
```

### Comparing `dbmsbenchmarker-0.13.1/dbmsbenchmarker/parameter.py` & `dbmsbenchmarker-0.13.2/dbmsbenchmarker/parameter.py`

 * *Files identical despite different names*

### Comparing `dbmsbenchmarker-0.13.1/dbmsbenchmarker/reporter.py` & `dbmsbenchmarker-0.13.2/dbmsbenchmarker/reporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -392,16 +392,22 @@
         if self.per_stream:
             number_of_queries = len(self.benchmarker.protocol['query'].items())
             for c, connection in self.benchmarker.dbms.items():
                 if connection.hasHardwareMetrics():
                     logging.info("Hardware metrics for stream of connection {}".format(c))
                     times = self.benchmarker.protocol['query'][str(1)]
                     time_start = int(datetime.timestamp(datetime.strptime(times["starts"][c],'%Y-%m-%d %H:%M:%S.%f')))
-                    times = self.benchmarker.protocol['query'][str(number_of_queries)]
-                    time_end = int(datetime.timestamp(datetime.strptime(times["ends"][c],'%Y-%m-%d %H:%M:%S.%f')))
+                    time_end = time_start
+                    # find the last active query (with end time)
+                    for i in range(number_of_queries, 0, -1):
+                        times = self.benchmarker.protocol['query'][str(i)]
+                        if "ends" in times and c in times["ends"]:
+                            time_end = int(datetime.timestamp(datetime.strptime(times["ends"][c],'%Y-%m-%d %H:%M:%S.%f')))
+                            logging.debug("Last active query is {}".format(i))
+                            break
                     #logging.debug(connection.connectiondata['monitoring']['prometheus_url'])
                     query='stream'
                     if 'metrics' in connection.connectiondata['monitoring']:
                         metrics_dict = connection.connectiondata['monitoring']['metrics']
                     else:
                         metrics_dict = monitor.metrics.metrics
                     for m, metric in metrics_dict.items():
```

### Comparing `dbmsbenchmarker-0.13.1/dbmsbenchmarker/scripts/assets/icons/chevron_down.svg` & `dbmsbenchmarker-0.13.2/dbmsbenchmarker/scripts/assets/icons/chevron_down.svg`

 * *Files identical despite different names*

### Comparing `dbmsbenchmarker-0.13.1/dbmsbenchmarker/scripts/assets/icons/chevron_up.svg` & `dbmsbenchmarker-0.13.2/dbmsbenchmarker/scripts/assets/icons/chevron_up.svg`

 * *Files identical despite different names*

### Comparing `dbmsbenchmarker-0.13.1/dbmsbenchmarker/scripts/assets/styles.css` & `dbmsbenchmarker-0.13.2/dbmsbenchmarker/scripts/assets/styles.css`

 * *Files identical despite different names*

### Comparing `dbmsbenchmarker-0.13.1/dbmsbenchmarker/scripts/cli.py` & `dbmsbenchmarker-0.13.2/dbmsbenchmarker/scripts/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 	parser.add_argument('-ca', '--connection-alias', help='alias of connection to benchmark', default='')
 	parser.add_argument('-f', '--config-folder', help='folder containing query and connection config files. If set, the names connections.config and queries.config are assumed automatically.', default=None)
 	parser.add_argument('-r', '--result-folder', help='folder for storing benchmark result files, default is given by timestamp', default=None)
 	parser.add_argument('-e', '--generate-evaluation', help='generate new evaluation file', default='no', choices=['no','yes'])
 	parser.add_argument('-w', '--working', help='working per query or connection', default='query', choices=['query','connection'])
 	#parser.add_argument('-a', '--anonymize', help='anonymize all dbms', action='store_true', default=False)
 	#parser.add_argument('-u', '--unanonymize', help='unanonymize some dbms, only sensible in combination with anonymize', nargs='*', default=[])
-	parser.add_argument('-p', '--numProcesses', help='Number of parallel client processes. Global setting, can be overwritten by connection. If None given, half of all available processes is taken', default=None)
+	parser.add_argument('-p', '--numProcesses', help='Number of parallel client processes. Global setting, can be overwritten by connection. Default is 1.', default=None)
 	parser.add_argument('-s', '--seed', help='random seed', default=None)
 	parser.add_argument('-cs', '--copy-subfolder', help='copy subfolder of result folder', action='store_true')
 	parser.add_argument('-ms', '--max-subfolders', help='maximum number of subfolders of result folder', default=None)
 	parser.add_argument('-sl', '--sleep', help='sleep SLEEP seconds before going to work', default=0)
 	parser.add_argument('-st', '--start-time', help='sleep until START-TIME before beginning benchmarking', default=None)
 	parser.add_argument('-sf', '--subfolder', help='stores results in a SUBFOLDER of the result folder', default=None)
 	parser.add_argument('-vq', '--verbose-queries', help='print every query that is sent', action='store_true', default=False)
```

### Comparing `dbmsbenchmarker-0.13.1/dbmsbenchmarker/scripts/dashboardcli.py` & `dbmsbenchmarker-0.13.2/dbmsbenchmarker/scripts/dashboardcli.py`

 * *Files identical despite different names*

### Comparing `dbmsbenchmarker-0.13.1/dbmsbenchmarker/tools.py` & `dbmsbenchmarker-0.13.2/dbmsbenchmarker/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -527,14 +527,18 @@
 
         :param connectiondata: Dict containing connection infos
         :return: returns nothing
         """
         self.connectiondata = connectiondata
         self.connection = None
         self.cursor = None
+        self.product = "unknown"
+        self.version = "unknown"
+        self.driver = "unknown"
+        self.driverversion = "unknown"
         if not connectiondata['JDBC']['jar'] in dbms.jars:
             if isinstance(connectiondata['JDBC']['jar'], list):
                 # accept list of jars
                 dbms.jars.extend(connectiondata['JDBC']['jar'])
             else:
                 # append single jar
                 dbms.jars.append(connectiondata['JDBC']['jar'])
@@ -594,14 +598,40 @@
         """
         if 'JDBC' in self.connectiondata:
             self.connection = jaydebeapi.connect(
                 self.connectiondata['JDBC']['driver'],
                 self.connectiondata['JDBC']['url'],
                 self.connectiondata['JDBC']['auth'],
                 dbms.jars,)
+            try:
+                self.metadata = self.connection.jconn.getMetaData()
+                self.product = self.metadata.getDatabaseProductName()
+                self.version = self.metadata.getDatabaseProductVersion()
+                self.driver = self.metadata.getDriverName()
+                self.driverversion = self.metadata.getDriverVersion()
+                self.connectiondata['product'] = self.product
+                self.connectiondata['version'] = self.version
+                self.connectiondata['driver'] = self.driver
+                self.connectiondata['driverversion'] = self.driverversion
+                print("Connected to {} version {} using {} version {}".format(self.product, self.version, self.driver, self.driverversion))
+            except Exception as e:
+                print("Product and version not implemented in JDBC driver")
+            else:
+                pass
+            if 'init_SQL' in self.connectiondata:
+                try:
+                    query_init = self.connectiondata['init_SQL']
+                    print('init_SQL:', query_init)
+                    self.openCursor()
+                    self.executeQuery(query_init)
+                    #init_result = self.fetchResult()
+                    self.closeCursor()
+                except Exception as e:
+                    print("Error when running init_SQL:", query_init)
+                    #print(init_result)
             #self.connection.jconn.setAutoCommit(True)
         else:
             raise ValueError('No connection data for '+self.getName())
     def openCursor(self):
         """
         Opens cursor for current connection.
 
@@ -1735,15 +1765,15 @@
                     d1 = df1.to_dict(orient="list")
                 else:
                     continue
                 d = joinDicts(d,d1)
             if len(d) > 0:
                 df = pd.DataFrame(d)
                 # convert to csv
-                csv = df.to_csv(index_label=False,index=False,line_terminator='\n')
+                csv = df.to_csv(index_label=False,index=False,lineterminator='\n')
                 # save
                 filename = '{folder}/query_{numQuery}_{timer}.csv'.format(folder=folder, numQuery=numQuery, timer=t)
                 csv_file = open(filename, "w")
                 csv_file.write(csv)
                 csv_file.close()
                 print("Merged timer", filename)
     # merge metrics
```

### Comparing `dbmsbenchmarker-0.13.1/dbmsbenchmarker.egg-info/PKG-INFO` & `dbmsbenchmarker-0.13.2/dbmsbenchmarker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbmsbenchmarker
-Version: 0.13.1
+Version: 0.13.2
 Summary: DBMS-Benchmarker is a Python-based application-level blackbox benchmark tool for Database Management Systems (DBMS). It connects to a given list of DBMS (via JDBC) and runs a given list of parametrized and randomized (SQL) benchmark queries. Evaluations are available via Python interface, in reports and at an interactive multi-dimensional dashboard.
 Home-page: https://github.com/Beuth-Erdelt/DBMS-Benchmarker
 Author: Patrick Erdelt
 Author-email: perdelt@beuth-hochschule.de
 License: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbmsbenchmarker Version: 0.13.1 Summary: DBMS-
+Metadata-Version: 2.1 Name: dbmsbenchmarker Version: 0.13.2 Summary: DBMS-
 Benchmarker is a Python-based application-level blackbox benchmark tool for
 Database Management Systems (DBMS). It connects to a given list of DBMS (via
 JDBC) and runs a given list of parametrized and randomized (SQL) benchmark
 queries. Evaluations are available via Python interface, in reports and at an
 interactive multi-dimensional dashboard. Home-page: https://github.com/Beuth-
 Erdelt/DBMS-Benchmarker Author: Patrick Erdelt Author-email: perdelt@beuth-
 hochschule.de License: GNU Affero General Public License v3 Classifier:
```

### Comparing `dbmsbenchmarker-0.13.1/dbmsbenchmarker.egg-info/SOURCES.txt` & `dbmsbenchmarker-0.13.2/dbmsbenchmarker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbmsbenchmarker-0.13.1/dbmsbenchmarker.egg-info/requires.txt` & `dbmsbenchmarker-0.13.2/dbmsbenchmarker.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -10,33 +10,32 @@
 colour>=0.1.5
 Brotli>=1.0.7
 certifi>=2020.4.5.2
 chardet>=3.0.4
 click>=6.7
 colour>=0.1.5
 cycler>=0.10.0
-dash==2.6.2
+dash==2.10.2
 dash-auth
 dash-core-components
 dash-daq
 dash-html-components
 dash-renderer
 dash-table
-Flask==2.1.0
+Flask==2.2.5
 Flask-Caching
 future>=0.18.2
 idna>=2.9
 itsdangerous>=1.1.0
 kiwisolver>=1.2.0
 MarkupSafe>=1.1.1
 plotly>=4.8.1
 pyparsing>=2.4.7
 python-dateutil>=2.8.1
 pytz>=2020.1
 retrying>=1.3.3
 six>=1.14.0
 urllib3==1.26.5
 uuid>=1.30
-Werkzeug==2.1.0
+Werkzeug>=2.2.3
 m2r2
 myst_parser
-markupsafe==2.0.1
```

### Comparing `dbmsbenchmarker-0.13.1/setup.py` & `dbmsbenchmarker-0.13.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="dbmsbenchmarker",
-    version="0.13.1",
+    version="0.13.2",
     author="Patrick Erdelt",
     author_email="perdelt@beuth-hochschule.de",
     description="DBMS-Benchmarker is a Python-based application-level blackbox benchmark tool for Database Management Systems (DBMS). It connects to a given list of DBMS (via JDBC) and runs a given list of parametrized and randomized (SQL) benchmark queries. Evaluations are available via Python interface, in reports and at an interactive multi-dimensional dashboard.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Beuth-Erdelt/DBMS-Benchmarker",
     packages=setuptools.find_packages(),
```

