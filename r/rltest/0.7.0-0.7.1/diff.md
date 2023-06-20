# Comparing `tmp/rltest-0.7.0.tar.gz` & `tmp/rltest-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rltest-0.7.0.tar", max compression
+gzip compressed data, was "rltest-0.7.1.tar", max compression
```

## Comparing `rltest-0.7.0.tar` & `rltest-0.7.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1518 2023-05-11 09:39:09.720089 rltest-0.7.0/LICENSE
--rw-r--r--   0        0        0    12026 2023-05-11 09:39:09.720089 rltest-0.7.0/README.md
--rw-r--r--   0        0        0     8112 2023-05-11 09:39:09.720089 rltest-0.7.0/RLTest/Enterprise/CcsMock.py
--rw-r--r--   0        0        0     1835 2023-05-11 09:39:09.720089 rltest-0.7.0/RLTest/Enterprise/Dmc.py
--rw-r--r--   0        0        0     6393 2023-05-11 09:39:09.720089 rltest-0.7.0/RLTest/Enterprise/EnterpriseClusterEnv.py
--rw-r--r--   0        0        0       96 2023-05-11 09:39:09.720089 rltest-0.7.0/RLTest/Enterprise/__init__.py
--rw-r--r--   0        0        0     2705 2023-05-11 09:39:09.724089 rltest-0.7.0/RLTest/Enterprise/binaryrepo.py
--rw-r--r--   0        0        0      173 2023-05-11 09:39:09.724089 rltest-0.7.0/RLTest/__init__.py
--rw-r--r--   0        0        0    30478 2023-05-11 09:39:09.724089 rltest-0.7.0/RLTest/__main__.py
--rw-r--r--   0        0        0      361 2023-05-11 09:39:09.724089 rltest-0.7.0/RLTest/_version.py
--rw-r--r--   0        0        0     2398 2023-05-11 09:39:09.724089 rltest-0.7.0/RLTest/debuggers.py
--rw-r--r--   0        0        0    22355 2023-05-11 09:39:09.724089 rltest-0.7.0/RLTest/env.py
--rw-r--r--   0        0        0     3592 2023-05-11 09:39:09.724089 rltest-0.7.0/RLTest/exists_redis.py
--rw-r--r--   0        0        0     5623 2023-05-11 09:39:09.724089 rltest-0.7.0/RLTest/loader.py
--rw-r--r--   0        0        0     1620 2023-05-11 09:39:09.724089 rltest-0.7.0/RLTest/random_port.py
--rw-r--r--   0        0        0     8030 2023-05-11 09:39:09.724089 rltest-0.7.0/RLTest/redis_cluster.py
--rw-r--r--   0        0        0     5245 2023-05-11 09:39:09.724089 rltest-0.7.0/RLTest/redis_enterprise_cluster.py
--rw-r--r--   0        0        0    23199 2023-05-11 09:39:09.724089 rltest-0.7.0/RLTest/redis_std.py
--rw-r--r--   0        0        0     5976 2023-05-11 09:39:09.724089 rltest-0.7.0/RLTest/utils.py
--rw-r--r--   0        0        0     1217 2023-05-11 09:39:10.184093 rltest-0.7.0/pyproject.toml
--rw-r--r--   0        0        0    13238 1970-01-01 00:00:00.000000 rltest-0.7.0/setup.py
--rw-r--r--   0        0        0    13310 1970-01-01 00:00:00.000000 rltest-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1518 2023-06-20 06:00:39.840059 rltest-0.7.1/LICENSE
+-rw-r--r--   0        0        0    12026 2023-06-20 06:00:39.840059 rltest-0.7.1/README.md
+-rw-r--r--   0        0        0     8112 2023-06-20 06:00:39.840059 rltest-0.7.1/RLTest/Enterprise/CcsMock.py
+-rw-r--r--   0        0        0     1835 2023-06-20 06:00:39.840059 rltest-0.7.1/RLTest/Enterprise/Dmc.py
+-rw-r--r--   0        0        0     6393 2023-06-20 06:00:39.840059 rltest-0.7.1/RLTest/Enterprise/EnterpriseClusterEnv.py
+-rw-r--r--   0        0        0       96 2023-06-20 06:00:39.840059 rltest-0.7.1/RLTest/Enterprise/__init__.py
+-rw-r--r--   0        0        0     2705 2023-06-20 06:00:39.840059 rltest-0.7.1/RLTest/Enterprise/binaryrepo.py
+-rw-r--r--   0        0        0      173 2023-06-20 06:00:39.840059 rltest-0.7.1/RLTest/__init__.py
+-rw-r--r--   0        0        0    31405 2023-06-20 06:00:39.840059 rltest-0.7.1/RLTest/__main__.py
+-rw-r--r--   0        0        0      361 2023-06-20 06:00:39.840059 rltest-0.7.1/RLTest/_version.py
+-rw-r--r--   0        0        0     2398 2023-06-20 06:00:39.840059 rltest-0.7.1/RLTest/debuggers.py
+-rw-r--r--   0        0        0    22783 2023-06-20 06:00:39.840059 rltest-0.7.1/RLTest/env.py
+-rw-r--r--   0        0        0     3592 2023-06-20 06:00:39.840059 rltest-0.7.1/RLTest/exists_redis.py
+-rw-r--r--   0        0        0     5590 2023-06-20 06:00:39.840059 rltest-0.7.1/RLTest/loader.py
+-rw-r--r--   0        0        0     1620 2023-06-20 06:00:39.840059 rltest-0.7.1/RLTest/random_port.py
+-rw-r--r--   0        0        0     8274 2023-06-20 06:00:39.840059 rltest-0.7.1/RLTest/redis_cluster.py
+-rw-r--r--   0        0        0     5245 2023-06-20 06:00:39.840059 rltest-0.7.1/RLTest/redis_enterprise_cluster.py
+-rw-r--r--   0        0        0    25206 2023-06-20 06:00:39.840059 rltest-0.7.1/RLTest/redis_std.py
+-rw-r--r--   0        0        0     5976 2023-06-20 06:00:39.840059 rltest-0.7.1/RLTest/utils.py
+-rw-r--r--   0        0        0     1217 2023-06-20 06:00:40.268067 rltest-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0    13238 1970-01-01 00:00:00.000000 rltest-0.7.1/setup.py
+-rw-r--r--   0        0        0    13310 1970-01-01 00:00:00.000000 rltest-0.7.1/PKG-INFO
```

### Comparing `rltest-0.7.0/LICENSE` & `rltest-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rltest-0.7.0/README.md` & `rltest-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `rltest-0.7.0/RLTest/Enterprise/CcsMock.py` & `rltest-0.7.1/RLTest/Enterprise/CcsMock.py`

 * *Files identical despite different names*

### Comparing `rltest-0.7.0/RLTest/Enterprise/Dmc.py` & `rltest-0.7.1/RLTest/Enterprise/Dmc.py`

 * *Files identical despite different names*

### Comparing `rltest-0.7.0/RLTest/Enterprise/EnterpriseClusterEnv.py` & `rltest-0.7.1/RLTest/Enterprise/EnterpriseClusterEnv.py`

 * *Files identical despite different names*

### Comparing `rltest-0.7.0/RLTest/Enterprise/binaryrepo.py` & `rltest-0.7.1/RLTest/Enterprise/binaryrepo.py`

 * *Files identical despite different names*

### Comparing `rltest-0.7.0/RLTest/__main__.py` & `rltest-0.7.1/RLTest/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import traceback
 import sys
 import shutil
 import inspect
 import unittest
 import time
 import shlex
+import json
 from multiprocessing import Process, Queue
 
 from RLTest.env import Env, TestAssertionFailure, Defaults
 from RLTest.utils import Colors, fix_modules, fix_modulesArgs
 from RLTest.loader import TestLoader
 from RLTest.Enterprise import binaryrepo
 from RLTest import debuggers
@@ -266,14 +267,18 @@
 parser.add_argument('--debugger', help='Run specified command line as the debugger')
 
 parser.add_argument(
     '-s', '--no-output-catch', action='store_const', const=True, default=False,
     help='all output will be written to the stdout, no log files.')
 
 parser.add_argument(
+    '--verbose-information-on-failure', action='store_const', const=True, default=False,
+    help='Print a verbose information on test failure')
+
+parser.add_argument(
     '--enable-debug-command', action='store_const', const=True, default=False,
     help='On Redis 7, debug command need to be enabled in order to be used.')
 
 parser.add_argument('--check-exitcode', help='Check redis process exit code',
                     default=False, action='store_true')
 
 parser.add_argument('--unix', help='Use Unix domain sockets instead of TCP',
@@ -419,14 +424,15 @@
         Defaults.proxy_binary = self.args.proxy_binary_path
         Defaults.re_binary = self.args.enterprise_redis_path
         Defaults.re_libdir = self.args.enterprise_lib_path
         Defaults.use_aof = self.args.use_aof
         Defaults.debug_pause = self.args.debug
         Defaults.debug_print = self.args.debug_print
         Defaults.no_capture_output = self.args.no_output_catch
+        Defaults.print_verbose_information_on_failure = self.args.verbose_information_on_failure
         Defaults.debugger = debugger
         Defaults.sanitizer = sanitizer
         Defaults.exit_on_failure = self.args.exit_on_failure
         Defaults.port = self.args.redis_port
         Defaults.external_addr = self.args.existing_env_addr
         Defaults.use_unix = self.args.unix
         Defaults.randomize_ports = self.args.randomize_ports
@@ -729,16 +735,27 @@
                         for subtest in test.get_functions(obj):
                             failures += self._runTest(subtest, prefix='\t',
                                                     numberOfAssertionFailed=failures,
                                                     before=before, after=after)
                             done += 1
 
                     else:
-                        self._runTest(test)
+                        failures = self._runTest(test)
                         done += 1
+
+                    verboseInfo = {}
+                    if failures > 0 and Defaults.print_verbose_information_on_failure:
+                        lastEnv = self.currEnv
+                        verboseInfo['before_dispose'] = lastEnv.getInformationBeforeDispose()
+                
+                # here the env is down so lets collect more info and print it
+                if failures > 0 and Defaults.print_verbose_information_on_failure:
+                    verboseInfo['after_dispose'] = lastEnv.getInformationAfterDispose()
+                    lastEnv.debugPrint(json.dumps(verboseInfo, indent=2).replace('\\n', '\n'), force=True)
+
             self.takeEnvDown(fullShutDown=True)
 
             # serialized the results back
             results.put({'done': done, 'failures': self.testsFailed}, block=False)
 
         results = Queue()
         if self.parallelism == 1:
```

### Comparing `rltest-0.7.0/RLTest/debuggers.py` & `rltest-0.7.1/RLTest/debuggers.py`

 * *Files identical despite different names*

### Comparing `rltest-0.7.0/RLTest/env.py` & `rltest-0.7.1/RLTest/env.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,14 +126,15 @@
     tls_ca_cert_file = None
     tls_passphrase = None
     debugger = None
     sanitizer = None
     debug_print = False
     debug_pause = False
     no_capture_output = False
+    print_verbose_information_on_failure = False
     no_log = False
     exit_on_failure = False
     verbose = 0
     logdir = None
     use_slaves = False
     num_shards = 1
     external_addr = 'localhost:6379'
@@ -142,14 +143,15 @@
     oss_password = None
     cluster_node_timeout = None
     curr_test_name = None
     port=6379
     enable_debug_command=False
     terminate_retries=None
     terminate_retry_secs=None
+    protocol=2
 
     def getKwargs(self):
         kwargs = {
             'modulePath': self.module,
             'moduleArgs': self.module_args,
             'port': self.port,
             'useSlaves': self.use_slaves,
@@ -187,15 +189,15 @@
         return True
 
     def __init__(self, testName=None, testDescription=None, module=None,
                  moduleArgs=None, env=None, useSlaves=None, shardsCount=None, decodeResponses=None,
                  useAof=None, useRdbPreamble=None, forceTcp=False, useTLS=False, tlsCertFile=None, tlsKeyFile=None,
                  tlsCaCertFile=None, tlsPassphrase=None, logDir=None, redisBinaryPath=None, dmcBinaryPath=None,
                  redisEnterpriseBinaryPath=None, noDefaultModuleArgs=False, clusterNodeTimeout = None,
-                 freshEnv=False, enableDebugCommand=None, protocol=2, terminateRetries=None, terminateRetrySecs=None):
+                 freshEnv=False, enableDebugCommand=None, protocol=None, terminateRetries=None, terminateRetrySecs=None):
 
         self.testName = testName if testName else Defaults.curr_test_name
         if self.testName is None:
             self.testName = '%s.%s' % (inspect.getmodule(inspect.currentframe().f_back).__name__, inspect.currentframe().f_back.f_code.co_name)
         self.testName = self.testName.replace(' ', '_')
 
         if testDescription:
@@ -228,15 +230,15 @@
         self.redisEnterpriseBinaryPath = expandBinary(redisEnterpriseBinaryPath) if redisEnterpriseBinaryPath else Defaults.re_binary
         self.clusterNodeTimeout = clusterNodeTimeout if clusterNodeTimeout else Defaults.cluster_node_timeout
         self.port = Defaults.port
         self.enableDebugCommand = enableDebugCommand if enableDebugCommand else Defaults.enable_debug_command
         self.terminateRetries = terminateRetries
         self.terminateRetrySecs = terminateRetrySecs
 
-        self.protocol = protocol
+        self.protocol = protocol if protocol is not None else Defaults.protocol
 
         self.assertionFailedSummary = []
 
         if not freshEnv and Env.RTestInstance and Env.RTestInstance.currEnv and self.compareEnvs(Env.RTestInstance.currEnv):
             self.envRunner = Env.RTestInstance.currEnv.envRunner
         else:
             if Env.RTestInstance and Env.RTestInstance.currEnv:
@@ -254,14 +256,24 @@
             self.envRunner.printEnvData('\t\t')
 
         if Env.RTestInstance:
             Env.RTestInstance.currEnv = self
 
         if Defaults.debug_pause:
             input('\tenv is up, attach to any process with gdb and press any button to continue.')
+    
+    def getInformationBeforeDispose(self):
+        return {
+            "env": self.env,
+            "test": self.testName,
+            "env_info": self.envRunner.getInformationBeforeDispose()
+        }
+    
+    def getInformationAfterDispose(self):
+        return self.envRunner.getInformationAfterDispose()
 
     def getEnvByName(self):
         verbose = False
         kwargs = self.getEnvKwargs()
         single_args = self.getSingleArgs()
 
         test_fname = self.testName.replace(':', '_')
```

### Comparing `rltest-0.7.0/RLTest/exists_redis.py` & `rltest-0.7.1/RLTest/exists_redis.py`

 * *Files identical despite different names*

### Comparing `rltest-0.7.0/RLTest/loader.py` & `rltest-0.7.1/RLTest/loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -154,16 +154,15 @@
 
         return True
 
     def __iter__(self):
         return iter(self.tests)
 
     def print_tests(self):
+        tests = []
         for t in self.tests:
-            print("Test: ", t.name)
             if t.is_class:
-                print("\tClass")
-                print("\tFunctions")
                 for m in t.functions:
-                    print("\t\t", m)
+                    tests.append(f"{t.name}.{m}")
             else:
-                print("\tFunction")
+                tests.append(t.name)
+        print(*sorted(tests), sep='\n')
```

### Comparing `rltest-0.7.0/RLTest/random_port.py` & `rltest-0.7.1/RLTest/random_port.py`

 * *Files identical despite different names*

### Comparing `rltest-0.7.0/RLTest/redis_cluster.py` & `rltest-0.7.1/RLTest/redis_cluster.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,14 +40,20 @@
             print(Colors.Yellow(prefix + '\tzip module path:%s' % self.modulePath))
         if self.moduleArgs:
             print(Colors.Yellow(prefix + '\tmodule args:%s' % self.moduleArgs))
         for i, shard in enumerate(self.shards):
             print(Colors.Yellow(prefix + 'shard: %d' % (i + 1)))
             shard.printEnvData(prefix + '\t')
 
+    def getInformationBeforeDispose(self):
+        return [shard.getInformationBeforeDispose() for shard in self.shards]
+
+    def getInformationAfterDispose(self):
+        return [shard.getInformationAfterDispose() for shard in self.shards]  
+
     def waitCluster(self, timeout_sec=40):
         st = time.time()
         ok = 0
 
         while st + timeout_sec > time.time():
             ok = 0
             for shard in self.shards:
```

### Comparing `rltest-0.7.0/RLTest/redis_enterprise_cluster.py` & `rltest-0.7.1/RLTest/redis_enterprise_cluster.py`

 * *Files identical despite different names*

### Comparing `rltest-0.7.0/RLTest/redis_std.py` & `rltest-0.7.1/RLTest/redis_std.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,16 +42,20 @@
         self.sanitizer = sanitizer
         self.noCatch = noCatch
         self.noLog = noLog
         self.environ = os.environ.copy()
         self.useUnix = unix
         self.dbDirPath = dbDirPath
         self.masterProcess = None
+        self.masterStdout = None
+        self.masterStderr = None
         self.masterExitCode = None
         self.slaveProcess = None
+        self.slaveStdout = None
+        self.slaveStderr = None
         self.slaveExitCode = None
         self.verbose = verbose
         self.role = MASTER
         self.useTLS = useTLS
         self.tlsCertFile = tlsCertFile
         self.tlsKeyFile = tlsKeyFile
         self.tlsCaCertFile = tlsCaCertFile
@@ -73,17 +77,14 @@
             self.slavePort = -1
 
         if self.useUnix:
             if self.clusterEnabled:
                 raise ValueError('Unix sockets cannot be used with cluster mode')
             self.port = -1
 
-        if self.has_interactive_debugger and serverId > 1:
-            assert self.noCatch and not self.useSlaves and not self.clusterEnabled
-
         if self.useTLS:
             if self.useUnix:
                 raise ValueError('Unix sockets cannot be used with TLS enabled mode')
             if self.tlsCertFile is None:
                 raise ValueError('When useTLS option is True tlsCertFile must be defined')
             if os.path.isfile(self.tlsCertFile) is False:
                 raise ValueError(
@@ -163,15 +164,15 @@
         out, err = p.communicate()
         out = out.decode('utf-8')
         v = out[out.find("v=") + 2:out.find("sha=") - 1].split('.')
         return int(v[0]) * 10000 + int(v[1]) * 100 + int(v[2])
 
     def createCmdArgs(self, role):
         cmdArgs = []
-        if self.debugger:
+        if self.debugger and role == MASTER and self.masterServerId == 1:
             cmdArgs += self.debugger.generate_command(self._getValgrindFilePath(role) if not self.noCatch else None)
 
         cmdArgs += [self.redisBinaryPath]
 
         if self.port > -1:
             if self.useTLS:
                 cmdArgs += ['--port', str(0), '--tls-port', str(self.getPort(role))]
@@ -288,19 +289,66 @@
     def printEnvData(self, prefix=''):
         print(Colors.Yellow(prefix + 'master:'))
         self._printEnvData(prefix + '\t', MASTER)
         if self.useSlaves:
             print(Colors.Yellow(prefix + 'slave:'))
             self._printEnvData(prefix + '\t', SLAVE)
 
+    def getInformationBeforeDispose(self):
+        res = {}
+        instances = [(MASTER, self.getConnection(), self.masterProcess)]
+        if self.useSlaves:
+            instances.append((SLAVE, self.getSlaveConnection(), self.slaveProcess))
+        for role, conn, proc in instances:
+            logs = None
+            info = None
+            try:
+                with open(os.path.join(self.dbDirPath, self._getFileName(role, '.log'))) as f:
+                    logs = f.read()
+            except os.FileNoteFoundError:
+                pass
+            try:
+                info = conn.execute_command('info', 'everything')
+            except redis.exceptions.RedisError:
+                pass
+            res[role] = {
+                'info': info,
+                'logs': logs,
+            }
+        return res
+
+    def getInformationAfterDispose(self):
+        res = {}
+        instances = [(MASTER, self.masterStdout, self.masterStderr)]
+        if self.useSlaves:
+            instances.append((SLAVE, self.slaveStdout, self.slaveStderr))
+        for role, stdout, stderr in instances:
+            stdoutStr = None
+            stderrStr = None
+            try:
+                stdoutStr = stdout.read().decode('utf8')
+            except (NameError, AttributeError):
+                pass
+
+            try:
+                stderrStr = stderr.read().decode('utf8')
+            except (NameError, AttributeError):
+                pass
+
+            res[role] = {
+                'stdout': stdoutStr,
+                'stderr': stderrStr,
+            }
+        return res
+
     def startEnv(self, masters = True, slaves = True):
         if self.envIsUp and self.envIsHealthy:
             return  # env is already up
         stdoutPipe = subprocess.PIPE
-        stderrPipe = subprocess.STDOUT
+        stderrPipe = subprocess.PIPE
         stdinPipe = subprocess.PIPE
         if self.noCatch:
             stdoutPipe = sys.stdout
             stderrPipe = sys.stderr
 
         if self.has_interactive_debugger:
             stdinPipe = sys.stdin
@@ -331,14 +379,21 @@
                 self.waitForRedisToStart(con, self.slaveProcess)
             else:
                 self.slaveProcess = None
 
         self.envIsUp = self.masterProcess is not None or self.slaveProcess is not None
         self.envIsHealthy = self.masterProcess is not None and (self.slaveProcess is not None if self.useSlaves else True)
 
+        # self.masterStdout = self.masterProcess.stdout if self.masterProcess else None
+        # self.masterStderr = self.masterProcess.stderr if self.masterProcess else None
+
+        # if self.slaveProcess is not None:
+        #     self.slaveStdout = self.slaveProcess.stdout if self.slaveProcess else None
+        #     self.slaveStderr = self.slaveProcess.stderr if self.slaveProcess else None
+
     def _isAlive(self, process):
         if not process:
             return False
         # check if child process has terminated
         if process.poll() is None:
             return True
         return False
```

### Comparing `rltest-0.7.0/RLTest/utils.py` & `rltest-0.7.1/RLTest/utils.py`

 * *Files identical despite different names*

### Comparing `rltest-0.7.0/pyproject.toml` & `rltest-0.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "RLTest"
-version = "0.7.0"
+version = "0.7.1"
 description = "Redis Modules Test Framework, allow to run tests on redis and modules on a variety of environments"
 authors = [ "Redis, Inc. <oss@redis.com>" ]
 license = "BSD-3-Clause"
 readme = "README.md"
 classifiers = [
   "Topic :: Database",
   "Programming Language :: Python",
```

### Comparing `rltest-0.7.0/setup.py` & `rltest-0.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'redis>=5.0.0b3,<6.0.0']
 
 entry_points = \
 {'console_scripts': ['RLTest = RLTest.__main__:main']}
 
 setup_kwargs = {
     'name': 'rltest',
-    'version': '0.7.0',
+    'version': '0.7.1',
     'description': 'Redis Modules Test Framework, allow to run tests on redis and modules on a variety of environments',
     'long_description': '[![license](https://img.shields.io/github/license/RedisLabsModules/RLTest.svg)](https://github.com/RedisLabsModules/RLTest/blob/master/LICENSE)\n[![PyPI version](https://badge.fury.io/py/rltest.svg)](https://badge.fury.io/py/rltest)\n[![CI](https://github.com/RedisLabsModules/RLTest/workflows/CI/badge.svg)](https://github.com/RedisLabsModules/RLTest/actions)\n[![Version](https://img.shields.io/github/release/RedisLabsModules/RLTest.svg)](https://github.com/RedisLabsModules/RLTest/releases/latest)\n[![Codecov](https://codecov.io/gh/RedisLabsModules/RLTest/branch/master/graph/badge.svg)](https://codecov.io/gh/RedisLabsModules/RLTest)\n[![Known Vulnerabilities](https://snyk.io/test/github/RedisLabsModules/RLTest/badge.svg?targetFile=pyproject.toml)](https://snyk.io/test/github/RedisLabsModules/RLTest?targetFile=pyproject.toml)\n\n\n\n# RLTest\n\nRedis Labs Test Framework, allow running tests on redis and modules on a variety of environments.\n\nSupported Environment: oss, oss-cluster, enterprise, enterprise-cluster\n\nThe framework allow you to write a test without environment specification and then run the test on all supported environment.\n\n\n# Install\n```\n$ pip install git+https://github.com/RedisLabsModules/RLTest.git@master\n\n```\n\n# Usage:\n```\n$ RLTest --help\nusage: RLTest [-h] [--version] [--module MODULE] [--module-args MODULE_ARGS]\n              [--env {oss,oss-cluster,enterprise,enterprise-cluster,existing-env,cluster_existing-env}]\n              [--existing-env-addr EXISTING_ENV_ADDR]\n              [--shards_ports SHARDS_PORTS]\n              [--cluster_address CLUSTER_ADDRESS]\n              [--oss_password OSS_PASSWORD]\n              [--cluster_credentials CLUSTER_CREDENTIALS]\n              [--cluster_node_timeout CLUSTER_NODE_TIMEOUT]\n              [--internal_password INTERNAL_PASSWORD]\n              [--oss-redis-path OSS_REDIS_PATH]\n              [--enterprise-redis-path ENTERPRISE_REDIS_PATH]\n              [--stop-on-failure] [-x] [--verbose] [--debug] [-t TEST]\n              [--env-only] [--clear-logs] [--log-dir LOG_DIR] [--use-slaves]\n              [--shards-count SHARDS_COUNT] [--download-enterprise-binaries]\n              [--proxy-binary-path PROXY_BINARY_PATH]\n              [--enterprise-lib-path ENTERPRISE_LIB_PATH] [-r]\n              [--use-aof] [--use-rdb-preamble]\n              [--debug-print] [-V] [--vg-suppressions VG_SUPPRESSIONS]\n              [--vg-options VG_OPTIONS] [--vg-no-leakcheck] [--vg-verbose]\n              [--vg-no-fail-on-errors] [-i] [--debugger DEBUGGER] [-s]\n              [--check-exitcode] [--unix] [--randomize-ports] [--collect-only]\n              [--tls] [--tls-cert-file TLS_CERT_FILE]\n              [--tls-key-file TLS_KEY_FILE]\n              [--tls-ca-cert-file TLS_CA_CERT_FILE]\n\nTest Framework for redis and redis module\n\noptional arguments:\n  -h, --help            show this help message and exit\n  --version             Print RLTest version and exit (default: False)\n  --module MODULE       path to the module file. You can use `--module` more\n                        than once but it imples that you explicitly specify\n                        `--module-args` as well. Notice that on enterprise the\n                        file should be a zip file packed with\n                        [RAMP](https://github.com/RedisLabs/RAMP). (default:\n                        None)\n  --module-args MODULE_ARGS\n                        arguments to give to the module on loading (default:\n                        None)\n  --env {oss,oss-cluster,enterprise,enterprise-cluster,existing-env,cluster_existing-env}, -e {oss,oss-cluster,enterprise,enterprise-cluster,existing-env,cluster_existing-env}\n                        env on which to run the test (default: oss)\n  --existing-env-addr EXISTING_ENV_ADDR\n                        Address of existing env, relevent only when running\n                        with existing-env, cluster_existing-env (default:\n                        localhost:6379)\n  --shards_ports SHARDS_PORTS\n                        list of ports, the shards are listening to, relevent\n                        only when running with cluster_existing-env (default:\n                        None)\n  --cluster_address CLUSTER_ADDRESS\n                        enterprise cluster ip, relevent only when running with\n                        cluster_existing-env (default: None)\n  --oss_password OSS_PASSWORD\n                        set redis password, relevant for oss and oss-cluster\n                        environment (default: None)\n  --cluster_credentials CLUSTER_CREDENTIALS\n                        enterprise cluster cluster_credentials\n                        "username:password", relevent only when running with\n                        cluster_existing-env (default: None)\n  --cluster_node_timeout CLUSTER_NODE_TIMEOUT\n                        cluster node timeout in milliseconds\n  --internal_password INTERNAL_PASSWORD\n                        Give an ability to execute commands on shards\n                        directly, relevent only when running with\n                        cluster_existing-env (default: )\n  --oss-redis-path OSS_REDIS_PATH\n                        path to the oss redis binary (default: redis-server)\n  --enterprise-redis-path ENTERPRISE_REDIS_PATH\n                        path to the entrprise redis binary (default:\n                        ~/.RLTest/opt/redislabs/bin/redis-server)\n  --stop-on-failure     stop running on failure (default: False)\n  -x, --exit-on-failure\n                        Stop test execution and exit on first assertion\n                        failure (default: False)\n  --verbose, -v         print more information about the test (default: 0)\n  --debug               stop before each test allow gdb attachment (default:\n                        False)\n  -t TEST, --test TEST  Specify test to run, in the form of "file:test"\n                        (default: None)\n  --env-only            start the env but do not run any tests (default:\n                        False)\n  --clear-logs          deleting the log direcotry before the execution\n                        (default: False)\n  --log-dir LOG_DIR     directory to write logs to (default: ./logs)\n  --use-slaves          run env with slaves enabled (default: False)\n  --shards-count SHARDS_COUNT\n                        Number shards in bdb (default: 1)\n  --download-enterprise-binaries\n                        run env with slaves enabled (default: False)\n  --proxy-binary-path PROXY_BINARY_PATH\n                        dmc proxy binary path (default:\n                        ~/.RLTest/opt/redislabs/bin/dmcproxy)\n  --enterprise-lib-path ENTERPRISE_LIB_PATH\n                        path of needed libraries to run enterprise binaries\n                        (default: ~/.RLTest/opt/redislabs/lib/)\n  -r, --env-reuse       reuse exists env, this feature is based on best\n                        efforts, if the env can not be reused then it will be\n                        taken down. (default: False)\n  --use-aof             use aof instead of rdb (default: False)\n  --use-rdb-preamble    use rdb preamble when rewriting aof file (default: True)\n  --debug-print         print debug messages (default: False)\n  -V, --vg, --use-valgrind\n                        running redis under valgrind (assuming valgrind is\n                        install on the machine) (default: False)\n  --vg-suppressions VG_SUPPRESSIONS\n                        path valgrind suppressions file (default: None)\n  --vg-options VG_OPTIONS\n                        valgrind [options] (default: None)\n  --vg-no-leakcheck     Don\'t perform a leak check (default: False)\n  --vg-verbose          Don\'t log valgrind output. Output to screen directly\n                        (default: False)\n  --vg-no-fail-on-errors\n                        Dont Fail test when valgrind reported any errors in\n                        the run.By default on RLTest the return value from\n                        Valgrind will be used to fail the tests.Use this\n                        option when you wish to dry-run valgrind but not fail\n                        the test on valgrind reported errors. (default: False)\n  -i, --interactive-debugger\n                        runs the redis on a debuger (gdb/lldb)\n                        interactivly.debugger interactive mode is only\n                        possible on a single process and so unsupported on\n                        cluste or with slaves.it is also not possible to use\n                        valgrind on interactive mode.interactive mode direcly\n                        applies: --no-output-catch and --stop-on-failure.it is\n                        also implies that only one test will be run (if --env-\n                        only was not specify), an error will be raise\n                        otherwise. (default: False)\n  --debugger DEBUGGER   Run specified command line as the debugger (default:\n                        None)\n  -s, --no-output-catch\n                        all output will be written to the stdout, no log\n                        files. (default: False)\n  --check-exitcode      Check redis process exit code (default: False)\n  --unix                Use Unix domain sockets instead of TCP (default:\n                        False)\n  --randomize-ports     Randomize Redis listening port assignment rather\n                        thanusing default port (default: False)\n  --collect-only        Collect the tests and exit (default: False)\n  --tls                 Enable TLS Support and disable the non-TLS port\n                        completely. TLS connections will be available at the\n                        default non-TLS ports. (default: False)\n  --tls-cert-file TLS_CERT_FILE\n                        /path/to/redis.crt (default: None)\n  --tls-key-file TLS_KEY_FILE\n                        /path/to/redis.key (default: None)\n  --tls-ca-cert-file TLS_CA_CERT_FILE\n                        /path/to/ca.crt (default: None)\n\n```\n\n## Sample usages\n\n### Multiple modules\n\n```\nRLTest --module modules/module1.so --module-args \'\' --module modules/module2.so --module-args \'\'\n```\n\n# Configuration File\nBy default, the framework search for configuration file on the current directory. The configuration file name is: config.txt.\nIt is possible to specify different configuration file on command line using the \'@\' prefix, for example:\n```\nRLTest @myConfig.txt # search for myConfig.txt configuration file\n```\nThe configuration file format is the same as the command line argument, i.e : \'--< param_name > < param_val >\'.\n\nIt is also possible to comment a specific lines in the configuration file using \'#\'.\n\nExample:\n\n```\n-vv\n--clear-logs\n#--debug\n```\n\n\n# Test Example\n\n```python\nfrom RLTest import Env\nimport time\n\n\nclass testExample():\n    \'\'\'\n    run all tests on a single env without taking\n    env down between tests\n    \'\'\'\n    def __init__(self):\n        self.env = Env()\n\n    def testExample(self):\n        con = self.env.getConnection()\n        con.set(\'x\', 1)\n        self.env.assertEqual(con.get(\'x\'), \'1\')\n\n    def testExample1(self):\n        con = self.env.getConnection()\n        con.set(\'x\', 1)\n        self.env.assertEqual(con.get(\'x\'), \'1\')\n        self.env.assertFalse(True)  # check failure\n\n    def testExample2(self):\n        con = self.env.getConnection()\n        con.set(\'x\', 1)\n        self.env.assertEqual(con.get(\'x\'), \'1\')\n\n\n# run each test on different env\ndef test_example():\n    env = Env()\n    con = env.getConnection()\n    con.set(\'x\', 1)\n    env.assertEqual(con.get(\'x\'), \'1\')\n\n\ndef test_example_2():\n    env = Env()\n    env.assertOk(env.cmd(\'set\', \'x\', \'1\'))\n    env.expect(\'get\', \'x\').equal(\'1\')\n\n    env.expect(\'lpush\', \'list\', \'1\', \'2\', \'3\').equal(3)\n    env.expect(\'lrange\', \'list\', \'0\', \'-1\').debugPrint().contains(\'1\')\n    env.debugPrint(\'this is some debug printing\')\n\n\ndef test_example_3():\n    env = Env(useSlaves=True, env=\'oss\')\n    con = env.getConnection()\n    con.set(\'x\', 1)\n    con2 = env.getSlaveConnection()\n    time.sleep(0.1)\n    env.assertEqual(con2.get(\'x\'), \'1\')\n\n```\n',
     'author': 'Redis, Inc.',
     'author_email': 'oss@redis.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `rltest-0.7.0/PKG-INFO` & `rltest-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rltest
-Version: 0.7.0
+Version: 0.7.1
 Summary: Redis Modules Test Framework, allow to run tests on redis and modules on a variety of environments
 License: BSD-3-Clause
 Author: Redis, Inc.
 Author-email: oss@redis.com
 Requires-Python: >=3.7.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

