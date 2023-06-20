# Comparing `tmp/kas-3.2.3.tar.gz` & `tmp/kas-3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kas-3.2.3.tar", last modified: Sun Mar  5 09:37:09 2023, max compression
+gzip compressed data, was "dist/kas-3.3.tar", last modified: Tue Jun 20 19:26:55 2023, max compression
```

## Comparing `kas-3.2.3.tar` & `kas-3.3.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 jan       (1000) users      (100)        0 2023-03-05 09:37:09.000000 kas-3.2.3/
--rw-r--r--   0 jan       (1000) users      (100)     2830 2023-03-05 09:37:09.000000 kas-3.2.3/PKG-INFO
--rw-r--r--   0 jan       (1000) users      (100)     1624 2023-02-13 20:13:28.000000 kas-3.2.3/README.rst
-drwxr-xr-x   0 jan       (1000) users      (100)        0 2023-03-05 09:37:09.000000 kas-3.2.3/kas/
--rw-r--r--   0 jan       (1000) users      (100)     1527 2020-12-06 06:22:49.000000 kas-3.2.3/kas/__init__.py
--rw-r--r--   0 jan       (1000) users      (100)     1330 2021-09-13 11:52:25.000000 kas-3.2.3/kas/__main__.py
--rw-r--r--   0 jan       (1000) users      (100)     1422 2023-03-05 09:36:58.000000 kas-3.2.3/kas/__version__.py
--rw-r--r--   0 jan       (1000) users      (100)     6790 2023-03-05 09:32:47.000000 kas-3.2.3/kas/config.py
--rw-r--r--   0 jan       (1000) users      (100)     1455 2021-10-08 09:03:16.000000 kas-3.2.3/kas/configschema.py
--rw-r--r--   0 jan       (1000) users      (100)     4525 2022-10-28 05:38:25.000000 kas-3.2.3/kas/context.py
--rw-r--r--   0 jan       (1000) users      (100)    10949 2023-03-05 09:32:47.000000 kas-3.2.3/kas/includehandler.py
--rw-r--r--   0 jan       (1000) users      (100)     5227 2022-03-14 11:35:11.000000 kas-3.2.3/kas/kas.py
--rw-r--r--   0 jan       (1000) users      (100)    12372 2023-02-05 20:09:44.000000 kas-3.2.3/kas/libcmds.py
--rw-r--r--   0 jan       (1000) users      (100)    13003 2023-02-19 19:07:15.000000 kas-3.2.3/kas/libkas.py
-drwxr-xr-x   0 jan       (1000) users      (100)        0 2023-03-05 09:37:09.000000 kas-3.2.3/kas/plugins/
--rw-r--r--   0 jan       (1000) users      (100)     2014 2023-01-05 17:10:45.000000 kas-3.2.3/kas/plugins/__init__.py
--rw-r--r--   0 jan       (1000) users      (100)     4290 2022-03-29 07:24:09.000000 kas-3.2.3/kas/plugins/build.py
--rw-r--r--   0 jan       (1000) users      (100)     2352 2021-10-19 08:31:44.000000 kas-3.2.3/kas/plugins/checkout.py
--rw-r--r--   0 jan       (1000) users      (100)     5620 2023-03-05 09:32:47.000000 kas-3.2.3/kas/plugins/dump.py
--rw-r--r--   0 jan       (1000) users      (100)     4533 2022-08-05 10:51:15.000000 kas-3.2.3/kas/plugins/for_all_repos.py
--rw-r--r--   0 jan       (1000) users      (100)    17636 2023-01-20 08:22:31.000000 kas-3.2.3/kas/plugins/menu.py
--rw-r--r--   0 jan       (1000) users      (100)     4399 2022-08-26 13:04:59.000000 kas-3.2.3/kas/plugins/shell.py
--rw-r--r--   0 jan       (1000) users      (100)    17676 2023-03-05 09:32:47.000000 kas-3.2.3/kas/repos.py
--rw-r--r--   0 jan       (1000) users      (100)     8440 2023-03-05 09:32:47.000000 kas-3.2.3/kas/schema-kas.json
--rwxr-xr-x   0 jan       (1000) users      (100)    15601 2023-03-05 09:36:58.000000 kas-3.2.3/kas-container
-drwxr-xr-x   0 jan       (1000) users      (100)        0 2023-03-05 09:37:09.000000 kas-3.2.3/kas.egg-info/
--rw-r--r--   0 jan       (1000) users      (100)     2830 2023-03-05 09:37:09.000000 kas-3.2.3/kas.egg-info/PKG-INFO
--rw-r--r--   0 jan       (1000) users      (100)      566 2023-03-05 09:37:09.000000 kas-3.2.3/kas.egg-info/SOURCES.txt
--rw-r--r--   0 jan       (1000) users      (100)        1 2023-03-05 09:37:09.000000 kas-3.2.3/kas.egg-info/dependency_links.txt
--rw-r--r--   0 jan       (1000) users      (100)       38 2023-03-05 09:37:09.000000 kas-3.2.3/kas.egg-info/entry_points.txt
--rw-r--r--   0 jan       (1000) users      (100)       76 2023-03-05 09:37:09.000000 kas-3.2.3/kas.egg-info/requires.txt
--rw-r--r--   0 jan       (1000) users      (100)        4 2023-03-05 09:37:09.000000 kas-3.2.3/kas.egg-info/top_level.txt
--rw-r--r--   0 jan       (1000) users      (100)       58 2021-11-29 10:53:59.000000 kas-3.2.3/pyproject.toml
--rw-r--r--   0 jan       (1000) users      (100)       38 2023-03-05 09:37:09.000000 kas-3.2.3/setup.cfg
--rw-r--r--   0 jan       (1000) users      (100)     3246 2022-04-11 16:22:30.000000 kas-3.2.3/setup.py
+drwxr-xr-x   0 jan       (1000) users      (100)        0 2023-06-20 19:26:55.000000 kas-3.3/
+-rw-r--r--   0 jan       (1000) users      (100)     2878 2023-06-20 19:26:55.000000 kas-3.3/PKG-INFO
+-rw-r--r--   0 jan       (1000) users      (100)     1624 2023-04-08 06:54:12.000000 kas-3.3/README.rst
+drwxr-xr-x   0 jan       (1000) users      (100)        0 2023-06-20 19:26:55.000000 kas-3.3/kas/
+-rw-r--r--   0 jan       (1000) users      (100)     1527 2020-12-06 06:22:49.000000 kas-3.3/kas/__init__.py
+-rw-r--r--   0 jan       (1000) users      (100)     1330 2021-09-13 11:52:25.000000 kas-3.3/kas/__main__.py
+-rw-r--r--   0 jan       (1000) users      (100)     1420 2023-06-20 19:26:48.000000 kas-3.3/kas/__version__.py
+-rw-r--r--   0 jan       (1000) users      (100)     7155 2023-06-10 06:39:22.000000 kas-3.3/kas/config.py
+-rw-r--r--   0 jan       (1000) users      (100)     1455 2021-10-08 09:03:16.000000 kas-3.3/kas/configschema.py
+-rw-r--r--   0 jan       (1000) users      (100)     4525 2022-10-28 05:38:25.000000 kas-3.3/kas/context.py
+-rw-r--r--   0 jan       (1000) users      (100)    12259 2023-06-10 06:39:22.000000 kas-3.3/kas/includehandler.py
+-rw-r--r--   0 jan       (1000) users      (100)     6574 2023-05-28 10:39:04.000000 kas-3.3/kas/kas.py
+-rw-r--r--   0 jan       (1000) users      (100)     2872 2023-05-19 05:17:03.000000 kas-3.3/kas/kasusererror.py
+-rw-r--r--   0 jan       (1000) users      (100)    12663 2023-05-19 05:17:03.000000 kas-3.3/kas/libcmds.py
+-rw-r--r--   0 jan       (1000) users      (100)    13670 2023-06-10 06:39:22.000000 kas-3.3/kas/libkas.py
+drwxr-xr-x   0 jan       (1000) users      (100)        0 2023-06-20 19:26:55.000000 kas-3.3/kas/plugins/
+-rw-r--r--   0 jan       (1000) users      (100)     2014 2023-01-05 17:10:45.000000 kas-3.3/kas/plugins/__init__.py
+-rw-r--r--   0 jan       (1000) users      (100)     4276 2023-05-19 05:17:03.000000 kas-3.3/kas/plugins/build.py
+-rw-r--r--   0 jan       (1000) users      (100)     2352 2021-10-19 08:31:44.000000 kas-3.3/kas/plugins/checkout.py
+-rw-r--r--   0 jan       (1000) users      (100)     8728 2023-06-10 06:39:22.000000 kas-3.3/kas/plugins/dump.py
+-rw-r--r--   0 jan       (1000) users      (100)     5140 2023-06-10 06:39:22.000000 kas-3.3/kas/plugins/for_all_repos.py
+-rw-r--r--   0 jan       (1000) users      (100)    18530 2023-06-10 06:39:22.000000 kas-3.3/kas/plugins/menu.py
+-rw-r--r--   0 jan       (1000) users      (100)     4451 2023-05-19 05:17:03.000000 kas-3.3/kas/plugins/shell.py
+-rw-r--r--   0 jan       (1000) users      (100)    20545 2023-06-10 06:39:22.000000 kas-3.3/kas/repos.py
+-rw-r--r--   0 jan       (1000) users      (100)     9741 2023-06-10 06:39:22.000000 kas-3.3/kas/schema-kas.json
+-rwxr-xr-x   0 jan       (1000) users      (100)    16587 2023-06-20 19:26:48.000000 kas-3.3/kas-container
+drwxr-xr-x   0 jan       (1000) users      (100)        0 2023-06-20 19:26:55.000000 kas-3.3/kas.egg-info/
+-rw-r--r--   0 jan       (1000) users      (100)     2878 2023-06-20 19:26:55.000000 kas-3.3/kas.egg-info/PKG-INFO
+-rw-r--r--   0 jan       (1000) users      (100)      586 2023-06-20 19:26:55.000000 kas-3.3/kas.egg-info/SOURCES.txt
+-rw-r--r--   0 jan       (1000) users      (100)        1 2023-06-20 19:26:55.000000 kas-3.3/kas.egg-info/dependency_links.txt
+-rw-r--r--   0 jan       (1000) users      (100)       38 2023-06-20 19:26:55.000000 kas-3.3/kas.egg-info/entry_points.txt
+-rw-r--r--   0 jan       (1000) users      (100)       76 2023-06-20 19:26:55.000000 kas-3.3/kas.egg-info/requires.txt
+-rw-r--r--   0 jan       (1000) users      (100)        4 2023-06-20 19:26:55.000000 kas-3.3/kas.egg-info/top_level.txt
+-rw-r--r--   0 jan       (1000) users      (100)       58 2021-11-29 10:53:59.000000 kas-3.3/pyproject.toml
+-rw-r--r--   0 jan       (1000) users      (100)       38 2023-06-20 19:26:55.000000 kas-3.3/setup.cfg
+-rw-r--r--   0 jan       (1000) users      (100)     3286 2023-05-26 16:25:25.000000 kas-3.3/setup.py
```

### Comparing `kas-3.2.3/PKG-INFO` & `kas-3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.2
 Name: kas
-Version: 3.2.3
+Version: 3.3
 Summary: Setup tool for bitbake based projects
 Home-page: https://github.com/siemens/kas
 Maintainer: Jan Kiszka
 Maintainer-email: jan.kiszka@siemens.com
 License: MIT
-Download-URL: https://github.com/siemens/kas/archive/3.2.3.tar.gz
+Download-URL: https://github.com/siemens/kas/archive/3.3.tar.gz
 Description: Setup tool for bitbake based projects
         =====================================
         
         +--------------------+
         |    Build Status    |
         +====================+
         | |workflow-master|_ |
@@ -53,13 +53,14 @@
 Keywords: OpenEmbedded bitbake development
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.5
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.6
```

### Comparing `kas-3.2.3/README.rst` & `kas-3.3/README.rst`

 * *Files identical despite different names*

### Comparing `kas-3.2.3/kas/__init__.py` & `kas-3.3/kas/__init__.py`

 * *Files identical despite different names*

### Comparing `kas-3.2.3/kas/__main__.py` & `kas-3.3/kas/__main__.py`

 * *Files identical despite different names*

### Comparing `kas-3.2.3/kas/__version__.py` & `kas-3.3/kas/__version__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,12 +21,12 @@
 # SOFTWARE.
 """
     This module contains the version of kas.
 """
 __license__ = 'MIT'
 __copyright__ = 'Copyright (c) Siemens AG, 2017-2020'
 
-__version__ = '3.2.3'
+__version__ = '3.3'
 
 # Please update docs/format-changelog.rst when changing the file version.
-__file_version__ = 13
+__file_version__ = 14
 __compatible_file_version__ = 1
```

### Comparing `kas-3.2.3/kas/config.py` & `kas-3.3/kas/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,27 +42,31 @@
         self._override_task = task
         self._config = {}
         if not filename:
             filename = os.path.join(ctx.kas_work_dir, CONFIG_YAML_FILE)
 
         self.filenames = [os.path.abspath(configfile)
                           for configfile in filename.split(':')]
-        self.top_repo_path = Repo.get_root_path(
+        top_repo_path = Repo.get_root_path(
             os.path.dirname(self.filenames[0]))
 
         repo_paths = [Repo.get_root_path(os.path.dirname(configfile),
                                          fallback=False)
                       for configfile in self.filenames]
 
         if len(set(repo_paths)) > 1:
             raise IncludeException('All concatenated config files must '
                                    'belong to the same repository or all '
                                    'must be outside of versioning control')
 
-        self.handler = IncludeHandler(self.filenames, self.top_repo_path)
+        update = ctx.args.update if hasattr(ctx.args, 'update') else False
+
+        self.handler = IncludeHandler(self.filenames,
+                                      top_repo_path,
+                                      not update)
         self.repo_dict = self._get_repo_dict()
 
     def get_build_system(self):
         """
             Returns the pre-selected build system
         """
         return self._config.get('build_system', '')
@@ -100,19 +104,23 @@
 
     def get_repo(self, name):
         """
             Returns a `Repo` instance for the configuration with the key
             `name`.
         """
         repo_defaults = self._config.get('defaults', {}).get('repos', {})
+        overrides = self._config.get('overrides', {}) \
+                                .get('repos', {}).get(name, {})
         config = self.get_repos_config()[name] or {}
+        top_repo_path = self.handler.get_top_repo_path()
         return Repo.factory(name,
                             config,
                             repo_defaults,
-                            self.top_repo_path)
+                            top_repo_path,
+                            overrides)
 
     def _get_repo_dict(self):
         """
             Returns a dictionary containing the repositories with
             their names (as it is defined in the config file) as keys
             and the `Repo` instances as values.
         """
```

### Comparing `kas-3.2.3/kas/configschema.py` & `kas-3.3/kas/configschema.py`

 * *Files identical despite different names*

### Comparing `kas-3.2.3/kas/context.py` & `kas-3.3/kas/context.py`

 * *Files identical despite different names*

### Comparing `kas-3.2.3/kas/includehandler.py` & `kas-3.3/kas/includehandler.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,29 +22,34 @@
 
 """
     This module implements how includes of configuration files are handled in
     kas.
 """
 
 import os
+from pathlib import Path
 from collections import OrderedDict
 from collections.abc import Mapping
 import functools
 import logging
 
-from jsonschema.validators import Draft4Validator
+from jsonschema.validators import validator_for
 
+from .kasusererror import KasUserError
 from . import __file_version__, __compatible_file_version__
 from . import CONFIGSCHEMA
 
 __license__ = 'MIT'
 __copyright__ = 'Copyright (c) Siemens AG, 2017-2021'
 
+SOURCE_DIR_OVERRIDE_KEY = '_source_dir'
+SOURCE_DIR_HOST_OVERRIDE_KEY = '_source_dir_host'
 
-class LoadConfigException(Exception):
+
+class LoadConfigException(KasUserError):
     """
         Class for exceptions that appear while loading a configuration file.
     """
     def __init__(self, message, filename):
         super().__init__('{}: {}'.format(message, filename))
 
 
@@ -62,15 +67,16 @@
         import yaml
         with open(filename, 'rb') as fds:
             config = yaml.safe_load(fds)
     else:
         raise LoadConfigException('Config file extension not recognized',
                                   filename)
 
-    validator = Draft4Validator(CONFIGSCHEMA)
+    validator_class = validator_for(CONFIGSCHEMA)
+    validator = validator_class(CONFIGSCHEMA)
     validation_error = False
 
     for error in validator.iter_errors(config):
         validation_error = True
         logging.error('Config file validation Error:\n%s', error)
 
     if validation_error:
@@ -93,18 +99,18 @@
                                           __file_version__, version_value),
                                   filename)
 
     if config.get('proxy_config'):
         logging.warning('Obsolete ''proxy_config'' detected. '
                         'This has no effect and will be rejected soon.')
 
-    return config
+    return (config, config.get(SOURCE_DIR_OVERRIDE_KEY, None))
 
 
-class IncludeException(Exception):
+class IncludeException(KasUserError):
     """
         Class for exceptions that appear in the include mechanism.
     """
     pass
 
 
 class IncludeHandler:
@@ -117,20 +123,38 @@
         containing the path, relative to the repository root from the
         current file, or as a dictionary. The dictionary must have a
         'file' key containing the path to the include file and a 'repo'
         key containing the key of the repository. The path is interpreted
         relative to the repository root path.
 
         The includes are read and merged from the deepest level upwards.
+
+        In case ``ignore_lock`` is ``false``, kas checks if a file
+        ``<file>.lock.<ext>`` exists next to the first entry in
+        ``top_files``. This filename is then appended to the list of
+        ``top_files``.
     """
 
-    def __init__(self, top_files, top_repo_path):
+    def __init__(self, top_files, top_repo_path, use_lock=True):
         self.top_files = top_files
         self.top_repo_path = top_repo_path
 
+        if use_lock:
+            lockfile = self.get_lockfile()
+            if Path(lockfile).exists():
+                logging.debug('includehandler: append lockfile %s', lockfile)
+                self.top_files.append(lockfile)
+
+    def get_lockfile(self):
+        file = Path(self.top_files[0])
+        return file.parent / (file.stem + '.lock' + file.suffix)
+
+    def get_top_repo_path(self):
+        return self.top_repo_path
+
     def get_config(self, repos=None):
         """
         Parameters:
           repos -- A dictionary that maps repo names to directory paths
 
         Returns:
           (config, repos)
@@ -165,15 +189,24 @@
             On conflict the latter includes overwrite previous ones and
             the current file overwrites every include. (evaluation depth first
             and from top to bottom)
             """
 
             missing_repos = []
             configs = []
-            current_config = load_config(filename)
+            try:
+                current_config, src_dir = load_config(filename)
+                # src_dir must only be set by auto-generated config file
+                if src_dir:
+                    self.top_repo_path = src_dir
+                    repo_path = src_dir
+
+            except FileNotFoundError:
+                raise LoadConfigException('Configuration file not found',
+                                          filename)
             if not isinstance(current_config, Mapping):
                 raise IncludeException('Configuration file does not contain a '
                                        'dictionary as base type')
             header = current_config.get('header', {})
 
             for include in header.get('includes', []):
                 if isinstance(include, str):
```

### Comparing `kas-3.2.3/kas/kas.py` & `kas-3.3/kas/kas.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,45 +17,50 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """
     This module is the main entry point for kas, setup tool for bitbake based
-    projects
+    projects. In case of user errors (e.g. invalid configuration, repo fetch
+    failure) KAS exits with error code 2, while exiting with 1 for internal
+    errors. For details on error handling, see :mod:`kas.kasusererror`.
 """
 
 import argparse
 import atexit
 import asyncio
 import traceback
 import logging
 import signal
 import sys
 import os
+from .kasusererror import KasUserError, CommandExecError
 
 try:
     import colorlog
     HAVE_COLORLOG = True
 except ImportError:
     HAVE_COLORLOG = False
 
 from . import __version__, __file_version__, __compatible_file_version__
 from . import plugins
 
 __license__ = 'MIT'
 __copyright__ = 'Copyright (c) Siemens AG, 2017-2018'
 
+default_log_level = 'info'
+
 
 def create_logger():
     """
         Setup the logging environment
     """
     log = logging.getLogger()  # root logger
-    log.setLevel(logging.INFO)
+    log.setLevel(logging.getLevelName(default_log_level.upper()))
     format_str = '%(asctime)s - %(levelname)-8s - %(message)s'
     date_format = '%Y-%m-%d %H:%M:%S'
     if HAVE_COLORLOG and os.isatty(2):
         cformat = '%(log_color)s' + format_str
         colors = {'DEBUG': 'reset',
                   'INFO': 'reset',
                   'WARNING': 'bold_yellow',
@@ -89,15 +94,22 @@
         # no running loop anymore, nothing to do
         return
     except AttributeError:
         # for Python < 3.7
         loop = asyncio.get_event_loop()
         pending = asyncio.Task.all_tasks(loop)
     if not loop.is_closed():
-        loop.run_until_complete(asyncio.gather(*pending))
+        # this code path is observed on older python versions (e.g. 3.6).
+        # In case the loop is not yet closed, tasks still might throw
+        # exceptions, but we are not interested in these as they are
+        # likely due to the cancellation. By that, we simply drop them.
+        try:
+            loop.run_until_complete(asyncio.gather(*pending))
+        except KasUserError:
+            pass
         loop.close()
 
 
 def kas_get_argparser():
     """
         Creates an argparser for kas with all plugins.
     """
@@ -112,16 +124,23 @@
 
     verstr = '%(prog)s {} (configuration format version {}, ' \
         'earliest compatible version {})'.format(__version__, __file_version__,
                                                  __compatible_file_version__)
     parser.add_argument('--version', action='version', version=verstr)
 
     parser.add_argument('-d', '--debug',
-                        action='store_true',
-                        help='Enable debug logging')
+                        action='store_const', const='debug', dest='log_level',
+                        help='Enable debug logging (deprecated, use '
+                             '--log-level debug).')
+
+    parser.add_argument('-l', '--log-level',
+                        choices=['debug', 'info', 'warning', 'error',
+                                 'critical'],
+                        default='%s' % (default_log_level),
+                        help='Set log level (default: %s)' % default_log_level)
 
     subparser = parser.add_subparsers(help='sub command help', dest='cmd')
 
     for plugin in plugins.all():
         plugin_parser = subparser.add_parser(plugin.name, help=plugin.helpmsg)
         plugin.setup_parser(plugin_parser)
 
@@ -133,16 +152,17 @@
         The actual main entry point of kas.
     """
     create_logger()
 
     parser = kas_get_argparser()
     args = parser.parse_args(argv)
 
-    if args.debug:
-        logging.getLogger().setLevel(logging.DEBUG)
+    if args.log_level:
+        level_num = logging.getLevelName(args.log_level.upper())
+        logging.getLogger().setLevel(level_num)
 
     logging.info('%s %s started', os.path.basename(sys.argv[0]), __version__)
 
     loop = asyncio.get_event_loop()
 
     for sig in (signal.SIGINT, signal.SIGTERM):
         loop.add_signal_handler(sig, interruption)
@@ -158,15 +178,21 @@
 
 def main():
     """
         The main function that operates as a wrapper around kas.
     """
 
     try:
-        sys.exit(kas(sys.argv[1:]))
+        kas(sys.argv[1:])
+    except CommandExecError as err:
+        logging.error('%s', err)
+        sys.exit(err.ret_code if err.forward else 2)
+    except KasUserError as err:
+        logging.error('%s', err)
+        sys.exit(2)
     except Exception as err:
         logging.error('%s', err)
         traceback.print_exc()
         sys.exit(1)
 
 
 if __name__ == '__main__':
```

### Comparing `kas-3.2.3/kas/libcmds.py` & `kas-3.3/kas/libcmds.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 """
 
 import tempfile
 import logging
 import shutil
 import os
 import pprint
-import sys
 from .libkas import (ssh_cleanup_agent, ssh_setup_agent, ssh_no_host_key_check,
                      get_build_environ, repos_fetch, repos_apply_patches)
 from .includehandler import IncludeException
 
 __license__ = 'MIT'
 __copyright__ = 'Copyright (c) Siemens AG, 2017-2018'
 
@@ -148,14 +147,15 @@
         Sets up the home directory of kas.
     """
 
     # A list of environment variables that SETUP_HOME uses
     # This should be kept up to date with any code in execute()
     ENV_VARS = [
         'GIT_CREDENTIAL_HELPER',
+        'GIT_CREDENTIAL_USEHTTPPATH',
         'AWS_CONFIG_FILE',
         'AWS_SHARED_CREDENTIALS_FILE',
         'NETRC_FILE',
     ]
 
     def __init__(self):
         super().__init__()
@@ -183,14 +183,18 @@
                       '\temail = kas@example.com\n'
                       '\tname = Kas User\n')
             if os.environ.get('GIT_CREDENTIAL_HELPER', False):
                 fds.write('[credential]\n'
                           '\thelper = '
                           + os.environ.get('GIT_CREDENTIAL_HELPER')
                           + '\n')
+                if os.environ.get('GIT_CREDENTIAL_USEHTTPPATH', False):
+                    fds.write('\tuseHttpPath = '
+                              + os.environ.get('GIT_CREDENTIAL_USEHTTPPATH')
+                              + '\n')
 
         if os.environ.get('AWS_CONFIG_FILE', False) \
                 and os.environ.get('AWS_SHARED_CREDENTIALS_FILE', False):
             os.makedirs(self.tmpdirname + "/.aws")
 
             shutil.copy(os.environ['AWS_CONFIG_FILE'],
                         self.tmpdirname + "/.aws/config")
@@ -368,16 +372,16 @@
 
         logging.debug('Missing repos for complete config:\n%s',
                       pprint.pformat(ctx.missing_repo_names))
 
         ctx.missing_repos = []
         for repo_name in ctx.missing_repo_names:
             if repo_name not in ctx.config.get_repos_config():
-                logging.error('Include references unknown repo: %s', repo_name)
-                sys.exit(1)
+                raise IncludeException('Include references unknown repo: {}'
+                                       .format(repo_name))
             ctx.missing_repos.append(ctx.config.get_repo(repo_name))
 
         repos_fetch(ctx.missing_repos)
 
         for repo in ctx.missing_repos:
             repo.checkout()
```

### Comparing `kas-3.2.3/kas/libkas.py` & `kas-3.3/kas/libkas.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,19 +30,44 @@
 import tempfile
 import asyncio
 import errno
 import pathlib
 import signal
 from subprocess import Popen, PIPE
 from .context import get_context
+from .kasusererror import KasUserError, CommandExecError
 
 __license__ = 'MIT'
 __copyright__ = 'Copyright (c) Siemens AG, 2017-2018'
 
 
+class InitBuildEnvError(KasUserError):
+    """
+    Error related to the OE / ISAR environment setup scripts
+    """
+    pass
+
+
+class EnvNotValidError(KasUserError):
+    """
+    The caller environment is not suited for the requested operation
+    """
+    pass
+
+
+class TaskExecError(KasUserError):
+    """
+    Similar to :class:`kas.kasusererror.CommandExecError` but for kas
+    internal tasks
+    """
+    def __init__(self, command, ret_code):
+        self.ret_code = ret_code
+        super().__init__('{} failed: error code {}'.format(command, ret_code))
+
+
 class LogOutput:
     """
         Handles the log output of executed applications
     """
     def __init__(self, live):
         self.live = live
         self.stdout = []
@@ -127,28 +152,29 @@
     if ret and fail:
         msg = 'Command "{cwd}$ {cmd}" failed'.format(cwd=cwd, cmd=cmdstr)
         if logo.stderr:
             msg += '\n--- Error summary ---\n'
             for line in logo.stderr:
                 msg += line
         logging.error(msg)
+        raise CommandExecError(cmd, ret)
 
     return (ret, ''.join(logo.stdout))
 
 
 def run_cmd(cmd, cwd, env=None, fail=True, liveupdate=True):
     """
         Runs a command synchronously.
     """
 
     loop = asyncio.get_event_loop()
     (ret, output) = loop.run_until_complete(
         run_cmd_async(cmd, cwd, env, fail, liveupdate))
     if ret and fail:
-        sys.exit(ret)
+        raise CommandExecError(cmd, ret)
     return (ret, output)
 
 
 def find_program(paths, name):
     """
         Find a file within the paths array and returns its path.
     """
@@ -167,38 +193,36 @@
         return
 
     tasks = []
     for repo in repos:
         tasks.append(asyncio.ensure_future(repo.fetch_async()))
 
     loop = asyncio.get_event_loop()
-    loop.run_until_complete(asyncio.wait(tasks))
-
-    for task in tasks:
-        if task.result():
-            sys.exit(task.result())
+    try:
+        loop.run_until_complete(asyncio.gather(*tasks))
+    except CommandExecError as e:
+        raise TaskExecError('fetch repos', e.ret_code)
 
 
 def repos_apply_patches(repos):
     """
         Applies the patches to the repositories.
     """
     if len(repos) == 0:
         return
 
     tasks = []
     for repo in repos:
         tasks.append(asyncio.ensure_future(repo.apply_patches_async()))
 
     loop = asyncio.get_event_loop()
-    loop.run_until_complete(asyncio.wait(tasks))
-
-    for task in tasks:
-        if task.result():
-            sys.exit(task.result())
+    try:
+        loop.run_until_complete(asyncio.gather(*tasks))
+    except CommandExecError as e:
+        raise TaskExecError('apply patches', e.ret_code)
 
 
 def get_build_environ(build_system):
     """
         Creates the build environment variables.
     """
     # nasty side effect function: running oe/isar-init-build-env also
@@ -213,23 +237,23 @@
         scripts = ['oe-init-build-env', 'isar-init-build-env']
     permutations = \
         [(repo, script) for repo in get_context().config.get_repos()
          for script in scripts]
     for (repo, script) in permutations:
         if os.path.exists(repo.path + '/' + script):
             if init_repo:
-                logging.error('Multiple init scripts found (%s vs. %s). ',
-                              repo.name, init_repo.name)
-                logging.error('Resolve ambiguity by removing one of the repos')
-                sys.exit(1)
+                raise InitBuildEnvError(
+                    'Multiple init scripts found ({} vs. {}). '
+                    'Resolve ambiguity by removing one of the repos'
+                    .format(repo.name, init_repo.name))
+
             init_repo = repo
             init_script = script
     if not init_repo:
-        logging.error('Did not find any init-build-env script')
-        sys.exit(1)
+        raise InitBuildEnvError('Did not find any init-build-env script')
 
     with tempfile.TemporaryDirectory() as temp_dir:
         script = """#!/bin/bash
         set -e
         source %s $1 > /dev/null
         env
         """ % init_script
@@ -384,19 +408,19 @@
                         help='Config file, using .config.yaml in KAS_WORK_DIR '
                         'if none is specified',
                         nargs='?')
     parser.add_argument('--skip',
                         help='Skip build steps',
                         default=[])
     parser.add_argument('--force-checkout', action='store_true',
-                        help='Always checkout the desired refspec of each '
-                        'repository, discarding any local changes')
+                        help='Always checkout the desired commit/branch of '
+                        'each repository, discarding any local changes')
     parser.add_argument('--update', action='store_true',
                         help='Pull new upstream changes to the desired '
-                        'refspec even if it is already checked out locally')
+                        'branch even if it is already checked out locally')
 
 
 def setup_parser_preserve_env_arg(parser):
     parser.add_argument('-E', '--preserve-env',
                         help='Keep current user environment block',
                         action='store_true')
 
@@ -408,15 +432,14 @@
         for var in SetupHome.ENV_VARS:
             if var in os.environ:
                 logging.warning('Environment variable "%s" ignored '
                                 'because user environment is being used',
                                 var)
 
         if not os.isatty(sys.stdout.fileno()):
-            logging.error("Error: --preserve-env can only be "
-                          "run from a tty")
-            sys.exit(1)
+            raise EnvNotValidError(
+                '--preserve-env can only be run from a tty')
 
         ctx.environ = os.environ.copy()
 
         logging.warning("Preserving the current environment block may "
                         "have unintended side effects on the build.")
```

### Comparing `kas-3.2.3/kas/plugins/__init__.py` & `kas-3.3/kas/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `kas-3.2.3/kas/plugins/build.py` & `kas-3.3/kas/plugins/build.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 import subprocess
 import sys
 from kas.context import create_global_context
 from kas.config import Config
 from kas.libkas import find_program, run_cmd
 from kas.libcmds import Macro, Command
 from kas.libkas import setup_parser_common_args
+from kas.kasusererror import CommandExecError
 
 __license__ = 'MIT'
 __copyright__ = 'Copyright (c) Siemens AG, 2017-2018'
 
 
 class Build:
     """
@@ -110,14 +111,13 @@
         bitbake = find_program(ctx.environ['PATH'], 'bitbake')
         cmd = [bitbake, '-c', ctx.config.get_bitbake_task()] \
             + self.extra_bitbake_args + ctx.config.get_bitbake_targets()
         if sys.stdout.isatty():
             logging.info('%s$ %s', ctx.build_dir, ' '.join(cmd))
             ret = subprocess.call(cmd, env=ctx.environ, cwd=ctx.build_dir)
             if ret != 0:
-                logging.error('Command returned non-zero exit status %d', ret)
-                sys.exit(ret)
+                raise CommandExecError(cmd, ret)
         else:
             run_cmd(cmd, cwd=ctx.build_dir)
 
 
 __KAS_PLUGINS__ = [Build]
```

### Comparing `kas-3.2.3/kas/plugins/checkout.py` & `kas-3.3/kas/plugins/checkout.py`

 * *Files identical despite different names*

### Comparing `kas-3.2.3/kas/plugins/dump.py` & `kas-3.3/kas/plugins/for_all_repos.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # kas - setup tool for bitbake based projects
 #
-# Copyright (c) Siemens AG, 2017-2022
+# Copyright (c) Konsulko Group, 2020
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -16,135 +16,116 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """
-    This plugin implements the ``kas dump`` command.
+    This plugin implements the ``kas for-all-repos`` command.
 
-    When this command is executed, kas will parse all referenced config
-    files, expand includes and print a flattened yaml version of the
-    configuration to stdout. This config is semantically identical to the
-    input, but does not include any references to other configuration files.
-    The output of this command can be used to further analyse the build
-    configuration.
-
-    Please note:
-
-    - the dumped config is semantically identical but not bit-by-bit identical
-    - all referenced repositories are checked out to resolve cross-repo configs
-    - all refspecs are resolved before patches are applied
-
-    For example, to get a single config representing the final build config of
-    ``kas-project.yml:target-override.yml`` you could run:
-
-        kas dump kas-project.yml:target-override.yml > kas-project-expanded.yml
-
-    The generated config can be used as input for kas:
-
-        kas build kas-project-expanded.yml
+    When this command is executed, kas will checkout the repositories listed
+    in the chosen config file and then execute a specified command in each
+    repository. It can be used to query the repository status, automate
+    actions such as archiving the layers used in a build or to execute any
+    other required commands.
+
+    For example, to print the commit hashes used by each repository used in
+    the file ``kas-project.yml`` (assuming they are all git repositories) you
+    could run::
+
+        kas for-all-repos kas-project.yml 'git rev-parse HEAD'
+
+    The environment for executing the command in each repository is extended
+    to include the following variables:
+
+      * ``KAS_REPO_NAME``: The name of the current repository determined by
+        either the name property or by the key used for this repo in the config
+        file.
+
+      * ``KAS_REPO_PATH``: The path of the local directory where this
+        repository is checked out, relative to the directory where ``kas`` is
+        executed.
+
+      * ``KAS_REPO_URL``: The URL from which this repository was cloned, or an
+        empty string if no remote URL was given in the config file.
+
+      * ``KAS_REPO_COMMIT``: The commit ID which was checked out for this
+        repository, or an empty string if no commit was given in the config
+        file.
+
+      * ``KAS_REPO_BRANCH``: The branch which was checked out for this
+        repository, or an empty string if no branch was given in the config
+        file.
+
+      * ``KAS_REPO_REFSPEC``: The refspec which was checked out for this
+        repository, or an empty string if no refspec was given in the config
+        file. This variable is obsolete and will be removed when support for
+        respec keys is removed as well. Migrate your repos to commit/branch
+        and use the related variables instead.
 """
 
 import logging
-import sys
-import json
-import yaml
-from collections import OrderedDict
-from kas.context import get_context
-from kas.plugins.checkout import Checkout
+import os
+import subprocess
+from kas.context import create_global_context
+from kas.config import Config
+from kas.libcmds import Macro, Command, SetupHome
+from kas.libkas import setup_parser_common_args
+from kas.libkas import setup_parser_preserve_env_arg
+from kas.libkas import run_handle_preserve_env_arg
+from kas.kasusererror import CommandExecError
 
 __license__ = 'MIT'
-__copyright__ = 'Copyright (c) Siemens AG, 2022'
-
+__copyright__ = 'Copyright (c) Siemens AG, 2017-2018'
 
-class Dump(Checkout):
-    """
-    Implements a kas plugin that combines multiple kas configurations
-    and dumps the result.
-    """
 
-    name = 'dump'
+class ForAllRepos:
+    name = 'for-all-repos'
     helpmsg = (
-        'Expand and dump the final config to stdout. When resolving refspecs, '
-        'these are resolved before patches are applied.'
+        'Runs a specified command in all checked out repositories.'
     )
 
-    class KasYamlDumper(yaml.Dumper):
-        """
-        Yaml formatter (dumper) that generates output in a formatting which
-        is similar to kas example input files.
-        """
-
-        def represent_data(self, data):
-            if isinstance(data, str):
-                if data.count('\n') > 0:
-                    return self.represent_scalar(
-                        'tag:yaml.org,2002:str',
-                        data,
-                        style='|')
-                return self.represent_scalar('tag:yaml.org,2002:str', data)
-            elif isinstance(data, OrderedDict):
-                return self.represent_mapping(
-                    'tag:yaml.org,2002:map',
-                    data.items())
-            elif data is None:
-                return self.represent_scalar('tag:yaml.org,2002:null', '')
-            return super().represent_data(data)
-
     @classmethod
     def setup_parser(cls, parser):
-        super().setup_parser(parser)
-        parser.add_argument('--format',
-                            choices=['yaml', 'json'],
-                            default='yaml',
-                            help='Output format (default: yaml)')
-        parser.add_argument('--indent',
-                            type=int,
-                            default=4,
-                            help='Line indent (# of spaces, default: 4)')
-        parser.add_argument('--resolve-refs',
-                            action='store_true',
-                            help='Replace floating refs with exact SHAs')
-        parser.add_argument('--resolve-env',
-                            action='store_true',
-                            help='Set env defaults to captured env value')
+        setup_parser_common_args(parser)
+        setup_parser_preserve_env_arg(parser)
+        parser.add_argument('command',
+                            help='Command to be executed as a string.')
 
     def run(self, args):
-        args.skip += [
-            'setup_dir',
-            'repos_apply_patches',
-            'setup_environ',
-            'write_bbconfig',
-        ]
-
-        super().run(args)
-        ctx = get_context()
-        config_expanded = ctx.config.get_config()
-
-        # includes are already expanded, delete the key
-        if 'includes' in config_expanded['header']:
-            del config_expanded['header']['includes']
-
-        if args.resolve_refs:
-            repos = ctx.config.get_repos()
-            for r in repos:
-                if r.refspec:
-                    config_expanded['repos'][r.name]['refspec'] = r.revision
-
-        if args.resolve_env and 'env' in config_expanded:
-            config_expanded['env'] = ctx.config.get_environment()
-
-        if args.format == 'json':
-            json.dump(config_expanded, sys.stdout, indent=args.indent)
-            sys.stdout.write('\n')
-        elif args.format == 'yaml':
-            yaml.dump(
-                config_expanded, sys.stdout,
-                indent=args.indent,
-                Dumper=self.KasYamlDumper)
-        else:
-            logging.error('invalid format %s', args.format)
-            sys.exit(1)
+        ctx = create_global_context(args)
+        ctx.config = Config(ctx, args.config)
+
+        run_handle_preserve_env_arg(ctx, os, args, SetupHome)
+
+        macro = Macro()
+        macro.add(ForAllReposCommand(args.command))
+        macro.run(ctx, args.skip)
+
+
+class ForAllReposCommand(Command):
+    def __init__(self, command):
+        super().__init__()
+        self.command = command
+
+    def __str__(self):
+        return 'for-all-repos'
+
+    def execute(self, ctx):
+        for repo in ctx.config.get_repos():
+            env = {
+                **ctx.environ,
+                'KAS_REPO_NAME': repo.name,
+                'KAS_REPO_PATH': repo.path,
+                'KAS_REPO_URL': '' if repo.operations_disabled else repo.url,
+                'KAS_REPO_COMMIT': repo.commit or '',
+                'KAS_REPO_BRANCH': repo.branch or '',
+                'KAS_REPO_REFSPEC': repo.refspec or '',
+            }
+            logging.info('%s$ %s', repo.path, self.command)
+            retcode = subprocess.call(self.command, shell=True, cwd=repo.path,
+                                      env=env)
+            if retcode != 0:
+                raise CommandExecError(self.command, retcode)
 
 
-__KAS_PLUGINS__ = [Dump]
+__KAS_PLUGINS__ = [ForAllRepos]
```

### Comparing `kas-3.2.3/kas/plugins/for_all_repos.py` & `kas-3.3/kas/plugins/shell.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # kas - setup tool for bitbake based projects
 #
-# Copyright (c) Konsulko Group, 2020
+# Copyright (c) Siemens AG, 2017-2018
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -16,105 +16,116 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """
-    This plugin implements the ``kas for-all-repos`` command.
+    This plugin implements the ``kas shell`` command.
 
-    When this command is executed, kas will checkout the repositories listed
-    in the chosen config file and then execute a specified command in each
-    repository. It can be used to query the repository status, automate
-    actions such as archiving the layers used in a build or to execute any
-    other required commands.
+    When this command is executed, kas will checkout repositories, setup the
+    build environment and then start a shell in the build environment. This
+    can be used to manually run ``bitbake`` with custom command line options
+    or to execute other commands such as ``runqemu``.
 
-    For example, to print the commit hashes used by each repository used in
-    the file ``kas-project.yml`` (assuming they are all git repositories) you
-    could run::
+    For example, to start a shell in the build environment for the file
+    ``kas-project.yml`` you could run::
 
-        kas for-all-repos kas-project.yml 'git rev-parse HEAD'
+        kas shell kas-project.yml
 
-    The environment for executing the command in each repository is extended
-    to include the following variables:
+    Or to invoke qemu to test an image which has been built::
 
-      * ``KAS_REPO_NAME``: The name of the current repository determined by
-        either the name property or by the key used for this repo in the config
-        file.
-
-      * ``KAS_REPO_PATH``: The path of the local directory where this
-        repository is checked out, relative to the directory where ``kas`` is
-        executed.
-
-      * ``KAS_REPO_URL``: The URL from which this repository was cloned, or an
-        empty string if no remote URL was given in the config file.
-
-      * ``KAS_REPO_REFSPEC``: The refspec which was checked out for this
-        repository, or an empty string if no refspec was given in the config
-        file.
+        kas shell kas-project.yml -c 'runqemu'
 """
 
 import logging
 import os
 import subprocess
-import sys
 from kas.context import create_global_context
 from kas.config import Config
 from kas.libcmds import Macro, Command, SetupHome
 from kas.libkas import setup_parser_common_args
 from kas.libkas import setup_parser_preserve_env_arg
 from kas.libkas import run_handle_preserve_env_arg
+from kas.kasusererror import CommandExecError
 
 __license__ = 'MIT'
 __copyright__ = 'Copyright (c) Siemens AG, 2017-2018'
 
 
-class ForAllRepos:
-    name = 'for-all-repos'
-    helpmsg = (
-        'Runs a specified command in all checked out repositories.'
-    )
+class Shell:
+    """
+        Implements a kas plugin that opens a shell within the kas environment.
+    """
+
+    name = 'shell'
+    helpmsg = 'Run a shell in the build environment.'
 
     @classmethod
     def setup_parser(cls, parser):
+        """
+            Setup the argument parser for the shell plugin
+        """
+
         setup_parser_common_args(parser)
         setup_parser_preserve_env_arg(parser)
-        parser.add_argument('command',
-                            help='Command to be executed as a string.')
+        parser.add_argument('-k', '--keep-config-unchanged',
+                            help='Skip steps that change the configuration',
+                            action='store_true')
+        parser.add_argument('-c', '--command',
+                            help='Run command',
+                            default='')
 
     def run(self, args):
+        """
+            Runs this kas plugin
+        """
+
         ctx = create_global_context(args)
         ctx.config = Config(ctx, args.config)
 
         run_handle_preserve_env_arg(ctx, os, args, SetupHome)
 
+        if args.keep_config_unchanged:
+            # Skip the tasks which would change the config of the build
+            # environment
+            args.skip += [
+                'setup_dir',
+                'finish_setup_repos',
+                'repos_apply_patches',
+                'write_bbconfig',
+            ]
+
         macro = Macro()
-        macro.add(ForAllReposCommand(args.command))
+        macro.add(ShellCommand(args.command))
         macro.run(ctx, args.skip)
 
 
-class ForAllReposCommand(Command):
-    def __init__(self, command):
+class ShellCommand(Command):
+    """
+        This class implements the command that starts a shell.
+    """
+
+    def __init__(self, cmd):
         super().__init__()
-        self.command = command
+        self.cmd = []
+        if cmd:
+            self.cmd = cmd
 
     def __str__(self):
-        return 'for-all-repos'
+        return 'shell'
 
     def execute(self, ctx):
-        for repo in ctx.config.get_repos():
-            env = {
-                **ctx.environ,
-                'KAS_REPO_NAME': repo.name,
-                'KAS_REPO_PATH': repo.path,
-                'KAS_REPO_URL': '' if repo.operations_disabled else repo.url,
-                'KAS_REPO_REFSPEC': repo.refspec or '',
-            }
-            logging.info('%s$ %s', repo.path, self.command)
-            retcode = subprocess.call(self.command, shell=True, cwd=repo.path,
-                                      env=env)
-            if retcode != 0:
-                logging.error('Command failed with return code %d', retcode)
-                sys.exit(retcode)
+        logging.info("To start the default build, run: bitbake -c %s %s",
+                     ctx.config.get_bitbake_task(),
+                     ' '.join(ctx.config.get_bitbake_targets()))
+        cmd = [ctx.environ.get('SHELL', '/bin/sh')]
+        if self.cmd:
+            cmd.append('-c')
+            cmd.append(self.cmd)
+        ret = subprocess.call(cmd, env=ctx.environ, cwd=ctx.build_dir)
+        if ret != 0:
+            logging.error('Shell returned non-zero exit status')
+            raise CommandExecError(cmd, ret, True)
 
 
-__KAS_PLUGINS__ = [ForAllRepos]
+__KAS_PLUGINS__ = [Shell]
```

### Comparing `kas-3.2.3/kas/plugins/menu.py` & `kas-3.3/kas/plugins/menu.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,41 +65,60 @@
     configuration in the ``menu_configuration`` key and also the effective
     settings that can be used to invoke ``kas build`` or other kas commands.
 """
 
 import logging
 import os
 import pprint
-import sys
 import yaml
-from kconfiglib import Kconfig, Symbol, Choice, expr_value, TYPE_TO_STR, \
-    MENU, COMMENT, STRING, BOOL, INT, HEX, UNKNOWN
+from kconfiglib import Kconfig, Symbol, Choice, KconfigError, \
+    expr_value, TYPE_TO_STR, MENU, COMMENT, STRING, BOOL, INT, HEX, UNKNOWN
 from kas import __version__, __file_version__
 from kas.context import create_global_context
 from kas.config import CONFIG_YAML_FILE
-from kas.includehandler import load_config as load_config_yaml
+from kas.repos import Repo
+from kas.includehandler import load_config as load_config_yaml, \
+    SOURCE_DIR_OVERRIDE_KEY, SOURCE_DIR_HOST_OVERRIDE_KEY
 from kas.plugins.build import Build
+from kas.kasusererror import KasUserError
 
 try:
     from snack import SnackScreen, EntryWindow, ButtonChoiceWindow, \
         ButtonBar, Listbox, GridFormHelp
     newt_available = True
 except ImportError:
     newt_available = False  # will be reported in run()
 
 __license__ = 'MIT'
 __copyright__ = \
     'Copyright (c) 2011-2019, Ulf Magnusson <ulfalizer@gmail.com>\n' \
-    'Copyright (c) Siemens AG, 2021'
+    'Copyright (c) Siemens AG, 2021-2023'
+
+SOURCE_DIR_HOST_ENV_KEY = '_KAS_REPO_DIR_HOST'
+
+
+class VariableTypeError(KasUserError):
+    pass
+
+
+class MissingModuleError(KasUserError):
+    pass
+
+
+class KConfigLoadError(KasUserError):
+    """
+    The KConfig file could not be found or is invalid
+    """
+    pass
 
 
 def check_sym_is_string(sym):
     if sym.type != STRING:
-        logging.error('Variable %s must be of string type', sym.name)
-        sys.exit(1)
+        raise VariableTypeError('Variable {} must be of string type'
+                                .format(sym.name))
 
 
 def str_representer(dumper, data):
     style = '|' if len(data.splitlines()) > 1 else None
     return dumper.represent_scalar('tag:yaml.org,2002:str', data, style=style)
 
 
@@ -121,15 +140,15 @@
     def setup_parser(cls, parser):
         parser.add_argument('kconfig',
                             help='Kconfig file',
                             nargs='?', default='Kconfig')
 
     def load_config(self, filename):
         try:
-            self.orig_config = load_config_yaml(filename)
+            self.orig_config, _ = load_config_yaml(filename)
         except FileNotFoundError:
             self.orig_config = {}
             return
 
         menu_configuration = self.orig_config.get('menu_configuration', {})
         for symname in menu_configuration:
             sym = self.kconf.syms.get(symname)
@@ -144,15 +163,15 @@
             elif sym.type == INT:
                 sym.set_value(str(symvalue))
             elif sym.type == HEX:
                 sym.set_value(str(hex(symvalue)))
             else:  # string
                 sym.set_value(symvalue)
 
-    def save_config(self, filename):
+    def save_config(self, filename, top_repo_dir):
         kas_includes = []
         kas_targets = []
         kas_build_system = None
         kas_vars = {}
         menu_configuration = {}
 
         for symname in self.kconf.syms:
@@ -171,18 +190,17 @@
                 elif sym.type == STRING:
                     menu_configuration[symname] = symvalue
                 elif sym.type == INT:
                     menu_configuration[symname] = int(symvalue)
                 elif sym.type == HEX:
                     menu_configuration[symname] = int(symvalue, 16)
                 else:
-                    logging.error(
-                        'Configuration variable %s uses unsupported type',
-                        symname)
-                    sys.exit(1)
+                    raise VariableTypeError(
+                        'Configuration variable {} uses unsupported type'
+                        .format(symname))
 
             if symname.startswith('KAS_INCLUDE_'):
                 check_sym_is_string(sym)
                 if symvalue != '':
                     kas_includes.append(symvalue)
             elif symname.startswith('KAS_TARGET_'):
                 check_sym_is_string(sym)
@@ -196,16 +214,21 @@
                 kas_vars[symname] = symvalue
 
         config = {
             'header': {
                 'version': __file_version__,
                 'includes': kas_includes
             },
-            'menu_configuration': menu_configuration
+            'menu_configuration': menu_configuration,
+            SOURCE_DIR_OVERRIDE_KEY: top_repo_dir
         }
+
+        if SOURCE_DIR_HOST_ENV_KEY in os.environ:
+            config[SOURCE_DIR_HOST_OVERRIDE_KEY] = \
+                os.environ[SOURCE_DIR_HOST_ENV_KEY]
         if kas_build_system:
             config['build_system'] = kas_build_system
         if len(kas_targets) > 0:
             config['target'] = kas_targets
         if len(kas_vars) > 0:
             config['local_conf_header'] = {
                 '__menu_config_vars': '\n'.join([
@@ -237,34 +260,38 @@
     def dump_kconf_warnings(self):
         if len(self.kconf.warnings) > 0:
             logging.warning("\n".join(self.kconf.warnings))
             self.kconf.warnings = []
 
     def run(self, args):
         if not newt_available:
-            logging.error(
+            raise MissingModuleError(
                 'Menu plugin requires \'python3-newt\' distribution package.')
-            sys.exit(1)
 
         ctx = create_global_context(args)
 
-        self.kconf = Kconfig(args.kconfig, warn_to_stderr=False)
+        kconfig_file = os.path.abspath(args.kconfig)
+        try:
+            self.kconf = Kconfig(kconfig_file, warn_to_stderr=False)
+        except (KconfigError, FileNotFoundError) as err:
+            raise KConfigLoadError(str(err))
 
+        top_repo_path = Repo.get_root_path(os.path.dirname(kconfig_file))
         config_filename = os.path.join(ctx.kas_work_dir, CONFIG_YAML_FILE)
 
         self.load_config(config_filename)
         self.dump_kconf_warnings()
 
         menu = Menuconfig(self.kconf)
         action = menu.show()
 
         if action == 'exit':
             return
 
-        self.save_config(config_filename)
+        self.save_config(config_filename, top_repo_path)
         self.dump_kconf_warnings()
 
         if action == 'build':
             logging.debug('Starting build')
 
             build_args = Args()
             build_args.config = None
```

### Comparing `kas-3.2.3/kas/repos.py` & `kas-3.3/kas/repos.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,29 +27,66 @@
 import os
 import sys
 import logging
 from urllib.parse import urlparse
 from tempfile import TemporaryDirectory
 from .context import get_context
 from .libkas import run_cmd_async, run_cmd
+from .kasusererror import KasUserError
 
 __license__ = 'MIT'
 __copyright__ = 'Copyright (c) Siemens AG, 2017-2018'
 
 
+class UnsupportedRepoTypeError(KasUserError, NotImplementedError):
+    """
+    The requested repo type is unsupported / not implemented
+    """
+    pass
+
+
+class RepoRefError(KasUserError):
+    """
+    The requested repo reference is invalid, missing or could not be found
+    """
+    pass
+
+
+class PatchFileNotFound(KasUserError, FileNotFoundError):
+    """
+    The requested patch file was not found
+    """
+    pass
+
+
+class PatchMappingError(KasUserError):
+    """
+    The requested patch can not be related to a repo
+    """
+    pass
+
+
+class PatchApplyError(KasUserError):
+    """
+    The provided patch file could not be applied
+    """
+
+
 class Repo:
     """
         Represents a repository in the kas configuration.
     """
 
-    def __init__(self, name, url, path, refspec, layers, patches,
-                 disable_operations):
+    def __init__(self, name, url, path, commit, branch, refspec, layers,
+                 patches, disable_operations):
         self.name = name
         self.url = url
         self.path = path
+        self.commit = commit
+        self.branch = branch
         self.refspec = refspec
         self._layers = layers
         self._patches = patches
         self.operations_disabled = disable_operations
 
     def __getattr__(self, item):
         if item == 'layers':
@@ -70,31 +107,41 @@
                     expr, subst = mirror.split()
                     if re.match(expr, self.url):
                         return re.sub(expr, subst, self.url)
                 except ValueError:
                     continue
             return self.url
         elif item == 'revision':
-            if not self.refspec:
+            if self.commit:
+                return self.commit
+            branch = self.branch or self.refspec
+            if not branch:
                 return None
             (_, output) = run_cmd(self.resolve_branch_cmd(),
                                   cwd=self.path, fail=False)
             if output:
                 return output.strip()
-            return self.refspec
+            return branch
 
         # Default behaviour
         raise AttributeError
 
     def __str__(self):
-        return '%s:%s %s %s' % (self.url, self.refspec,
+        if self.commit and self.branch:
+            return '%s:%s(%s) %s %s' % (self.url, self.commit, self.branch,
+                                        self.path, self._layers)
+        return '%s:%s %s %s' % (self.url,
+                                self.commit or self.branch or self.refspec,
                                 self.path, self._layers)
 
+    __legacy_refspec_warned__ = []
+
     @staticmethod
-    def factory(name, repo_config, repo_defaults, repo_fallback_path):
+    def factory(name, repo_config, repo_defaults, repo_fallback_path,
+                repo_overrides={}):
         """
             Returns a Repo instance depending on params.
         """
         layers_dict = repo_config.get('layers', {'': None})
         layers = list(filter(lambda x, laydict=layers_dict:
                              str(laydict[x]).lower() not in
                              ['disabled', 'excluded', 'n', 'no', '0', 'false'],
@@ -107,28 +154,45 @@
                 continue
             this_patch = {
                 'id': p,
                 'repo': patches_dict[p].get('repo', default_patch_repo),
                 'path': patches_dict[p]['path'],
             }
             if this_patch['repo'] is None:
-                logging.error('No repo specified for patch entry "%s" and no '
-                              'default repo specified.', p)
-                sys.exit(1)
+                raise PatchMappingError(
+                    'No repo specified for patch entry "{}" and no '
+                    'default repo specified.'.format(p))
+
             patches.append(this_patch)
 
         url = repo_config.get('url', None)
         name = repo_config.get('name', name)
         typ = repo_config.get('type', 'git')
+        commit = repo_config.get('commit', None)
+        branch = repo_config.get('branch', repo_defaults.get('branch', None))
         refspec = repo_config.get('refspec',
                                   repo_defaults.get('refspec', None))
-        if refspec is None and url is not None:
-            logging.error('No refspec specified for repository "%s". This is '
-                          'only allowed for local repositories.', name)
-            sys.exit(1)
+        if commit is None and branch is None and refspec is None \
+                and url is not None:
+            raise RepoRefError('No commit or branch specified for repository '
+                               '"{}". This is only allowed for local '
+                               'repositories.'.format(name))
+        if refspec is None:
+            commit = repo_overrides.get('commit', commit)
+        else:
+            if name not in Repo.__legacy_refspec_warned__:
+                logging.warning('Using deprecated refspec for repository '
+                                '"%s". You should migrate to commit/branch.',
+                                name)
+                Repo.__legacy_refspec_warned__.append(name)
+            if commit is not None or branch is not None:
+                raise RepoRefError('Unsupported mixture of legacy refspec '
+                                   'and commit/branch for repository "{}"'
+                                   .format(name))
+            refspec = repo_overrides.get('commit', refspec)
         path = repo_config.get('path', None)
         disable_operations = False
 
         if path is None:
             if url is None:
                 path = Repo.get_root_path(repo_fallback_path)
                 logging.info('Using %s as root for repository %s', path,
@@ -141,20 +205,20 @@
 
         if url is None:
             # No version control operation on repository
             url = path
             disable_operations = True
 
         if typ == 'git':
-            return GitRepo(name, url, path, refspec, layers, patches,
-                           disable_operations)
+            return GitRepo(name, url, path, commit, branch, refspec, layers,
+                           patches, disable_operations)
         if typ == 'hg':
-            return MercurialRepo(name, url, path, refspec, layers, patches,
-                                 disable_operations)
-        raise NotImplementedError('Repo type "%s" not supported.' % typ)
+            return MercurialRepo(name, url, path, commit, branch, refspec,
+                                 layers, patches, disable_operations)
+        raise UnsupportedRepoTypeError('Repo type "%s" not supported.' % typ)
 
     @staticmethod
     def get_root_path(path, fallback=True):
         """
             Checks if path is under version control and returns its root path.
         """
         (ret, output) = run_cmd(['git', 'rev-parse', '--show-toplevel'],
@@ -190,16 +254,14 @@
         if refdir and not os.path.exists(sdir):
             os.makedirs(refdir, exist_ok=True)
             with TemporaryDirectory(prefix=self.qualified_name + '.',
                                     dir=refdir) as tmpdir:
                 (retc, _) = await run_cmd_async(
                     self.clone_cmd(tmpdir, createref=True),
                     cwd=get_context().kas_work_dir)
-                if retc != 0:
-                    return retc
 
                 logging.debug('Created repo ref for %s', self.qualified_name)
                 try:
                     os.rename(tmpdir, sdir)
                     if sys.version_info < (3, 8):
                         # recreate dir so cleanup handler can delete it
                         os.makedirs(tmpdir, exist_ok=True)
@@ -208,109 +270,116 @@
                                   self.qualified_name)
 
         if not os.path.exists(self.path):
             os.makedirs(os.path.dirname(self.path), exist_ok=True)
             (retc, _) = await run_cmd_async(
                 self.clone_cmd(sdir, createref=False),
                 cwd=get_context().kas_work_dir)
-            if retc == 0:
-                logging.info('Repository %s cloned', self.name)
+
+            logging.info('Repository %s cloned', self.name)
 
         # Make sure the remote origin is set to the value
         # in the kas file to avoid surprises
         try:
             (retc, output) = await run_cmd_async(
                 self.set_remote_url_cmd(),
                 cwd=self.path,
                 liveupdate=False)
-            if retc != 0:
-                return retc
         except NotImplementedError:
             logging.warning('Repo implementation does not support changing '
                             'the remote url.')
 
         # take what came out of clone and stick to that forever
-        if self.refspec is None:
+        if self.commit is None and self.branch is None \
+           and self.refspec is None:
             return 0
 
         if not get_context().update:
-            # Does refspec exist in the current repository?
+            # Do commit/branch/refspec exist in the current repository?
             (retc, output) = await run_cmd_async(self.contains_refspec_cmd(),
                                                  cwd=self.path,
                                                  fail=False,
                                                  liveupdate=False)
             if retc == 0:
                 logging.info('Repository %s already contains %s as %s',
-                             self.name, self.refspec, output.strip())
+                             self.name,
+                             self.commit or self.branch or self.refspec,
+                             output.strip())
                 return retc
 
-        # Try to fetch if refspec is missing or if --update argument was passed
+        # Try to fetch if commit/branch/refspec is missing or if --update
+        # argument was passed
         (retc, output) = await run_cmd_async(self.fetch_cmd(),
                                              cwd=self.path,
                                              fail=False)
         if retc:
             logging.warning('Could not update repository %s: %s',
                             self.name, output)
         else:
             logging.info('Repository %s updated', self.name)
         return 0
 
     def checkout(self):
         """
             Checks out the correct revision of the repo.
         """
-        if self.operations_disabled or self.refspec is None:
+        if self.operations_disabled \
+            or (self.commit is None and self.branch is None
+                and self.refspec is None):
             return
 
         if not get_context().force_checkout:
             # Check if repos is dirty
             (_, output) = run_cmd(self.is_dirty_cmd(),
                                   cwd=self.path,
                                   fail=False)
             if output:
                 logging.warning('Repo %s is dirty - no checkout', self.name)
                 return
 
-        (_, output) = run_cmd(self.resolve_branch_cmd(),
-                              cwd=self.path, fail=False)
-        if output:
-            desired_ref = output.strip()
-            branch = True
+        if self.commit:
+            desired_ref = self.commit
+            is_branch = False
         else:
-            desired_ref = self.refspec
-            branch = False
+            (_, output) = run_cmd(self.resolve_branch_cmd(),
+                                  cwd=self.path, fail=False)
+            if output:
+                desired_ref = output.strip()
+                is_branch = True
+            elif self.branch:
+                raise RepoRefError(
+                    'Branch "{}" cannot be found in repository {}'
+                    .format(self.branch, self.name))
+            else:
+                desired_ref = self.refspec
+                is_branch = False
 
-        run_cmd(self.checkout_cmd(desired_ref, branch), cwd=self.path)
+        run_cmd(self.checkout_cmd(desired_ref, is_branch), cwd=self.path)
 
     async def apply_patches_async(self):
         """
             Applies patches to a repository asynchronously.
         """
         if self.operations_disabled or not self._patches:
             return 0
 
         (retc, _) = await run_cmd_async(self.prepare_patches_cmd(),
                                         cwd=self.path)
-        if retc:
-            return retc
 
         my_patches = []
 
         for patch in self._patches:
             other_repo = get_context().config.repo_dict.get(patch['repo'],
                                                             None)
 
             if not other_repo:
-                logging.error('Could not find referenced repo. '
-                              '(missing repo: %s, repo: %s, '
-                              'patch entry: %s)',
-                              patch['repo'],
-                              self.name,
-                              patch['id'])
-                return 1
+                raise PatchMappingError(
+                    'Could not find referenced repo. '
+                    '(missing repo: {}, repo: {}, patch entry: {})'
+                    .format(patch['repo'], self.name, patch['id']))
 
             path = os.path.join(other_repo.path, patch['path'])
             cmd = []
 
             if os.path.isfile(path):
                 my_patches.append((path, patch['id']))
             elif os.path.isdir(path) \
@@ -319,64 +388,63 @@
                     for line in f:
                         if line.startswith('#'):
                             continue
                         p = os.path.join(path, line.split(' #')[0].rstrip())
                         if os.path.isfile(p):
                             my_patches.append((p, patch['id']))
                         else:
-                            raise FileNotFoundError(p)
+                            raise PatchFileNotFound(p)
             else:
-                logging.error('Could not find patch. '
-                              '(patch path: %s, repo: %s, patch entry: %s)',
-                              path,
-                              self.name,
-                              patch['id'])
-                return 1
+                raise PatchFileNotFound(
+                    'Could not find patch. '
+                    '(patch path: {}, repo: {}, patch entry: {})'
+                    .format(path, self.name, patch['id']))
 
         for (path, patch_id) in my_patches:
             cmd = self.apply_patches_file_cmd(path)
-            (retc, output) = await run_cmd_async(cmd, cwd=self.path)
+            (retc, output) = await run_cmd_async(
+                cmd, cwd=self.path, fail=False)
             if retc:
-                logging.error('Could not apply patch. Please fix repos and '
-                              'patches. (patch path: %s, repo: %s, patch '
-                              'entry: %s, vcs output: %s)',
-                              path, self.name, patch_id, output)
-                return 1
-            else:
-                logging.info('Patch applied. '
-                             '(patch path: %s, repo: %s, patch entry: %s)',
-                             path, self.name, patch_id)
+                raise PatchApplyError(
+                    'Could not apply patch. Please fix repos and '
+                    'patches. (patch path: {}, repo: {}, patch '
+                    'entry: {}, vcs output: {})'
+                    .format(path, self.name, patch_id, output))
+
+            logging.info('Patch applied. '
+                         '(patch path: %s, repo: %s, patch entry: %s)',
+                         path, self.name, patch_id)
 
             cmd = self.add_cmd()
-            (retc, output) = await run_cmd_async(cmd, cwd=self.path)
+            (retc, output) = await run_cmd_async(
+                cmd, cwd=self.path, fail=False)
             if retc:
-                logging.error('Could not add patched files. '
-                              'repo: %s, vcs output: %s)',
-                              self.name, output)
-                return 1
+                raise PatchApplyError(
+                    'Could not add patched files. repo: {}, vcs output: {})'
+                    .format(self.name, output))
 
             cmd = self.commit_cmd()
-            (retc, output) = await run_cmd_async(cmd, cwd=self.path)
+            (retc, output) = await run_cmd_async(
+                cmd, cwd=self.path, fail=False)
             if retc:
-                logging.error('Could not commit patch changes. '
-                              'repo: %s, vcs output: %s)',
-                              self.name, output)
-                return 1
+                raise PatchApplyError(
+                    'Could not commit patch changes. repo: {}, vcs output: {})'
+                    .format(self.name, output))
 
         return 0
 
 
 class GitRepo(RepoImpl):
     """
         Provides the git functionality for a Repo.
     """
 
-    def remove_ref_prefix(self, refspec):
+    def remove_ref_prefix(self, branch):
         ref_prefix = 'refs/'
-        return refspec[refspec.startswith(ref_prefix) and len(ref_prefix):]
+        return branch[branch.startswith(ref_prefix) and len(ref_prefix):]
 
     def add_cmd(self):
         return ['git', 'add', '-A']
 
     def clone_cmd(self, srcdir, createref):
         cmd = ['git', 'clone', '-q']
         if createref:
@@ -388,46 +456,54 @@
         return cmd
 
     def commit_cmd(self):
         return ['git', 'commit', '-a', '--author', 'kas <kas@example.com>',
                 '-m', 'msg']
 
     def contains_refspec_cmd(self):
-        return ['git', 'cat-file', '-t', self.remove_ref_prefix(self.refspec)]
+        branch = self.branch or self.refspec
+        if branch and branch.startswith('refs/'):
+            branch = 'remotes/origin/' + self.remove_ref_prefix(branch)
+        return ['git', 'cat-file', '-t', self.commit or branch]
 
     def fetch_cmd(self):
         cmd = ['git', 'fetch', '-q']
-        if self.refspec.startswith('refs/'):
+        branch = self.branch or self.refspec
+        if branch and branch.startswith('refs/'):
             cmd.extend(['origin',
-                        '+' + self.refspec
+                        '+' + branch
                         + ':refs/remotes/origin/'
-                        + self.remove_ref_prefix(self.refspec)])
+                        + self.remove_ref_prefix(branch)])
 
         return cmd
 
     def is_dirty_cmd(self):
         return ['git', 'status', '-s']
 
     def resolve_branch_cmd(self):
         return ['git', 'rev-parse', '--verify', '-q',
-                'origin/{refspec}'.
-                format(refspec=self.remove_ref_prefix(self.refspec))]
+                'origin/{branch}'.
+                format(branch=self.remove_ref_prefix(
+                    self.branch or self.refspec))]
 
-    def checkout_cmd(self, desired_ref, branch):
+    def checkout_cmd(self, desired_ref, is_branch):
         cmd = ['git', 'checkout', '-q', self.remove_ref_prefix(desired_ref)]
-        if branch:
-            cmd.extend(['-B', self.remove_ref_prefix(self.refspec)])
+        if is_branch:
+            branch = self.remove_ref_prefix(self.branch or self.refspec)
+            branch = branch[branch.startswith('heads/') and len('heads/'):]
+            cmd.extend(['-B', branch])
         if get_context().force_checkout:
             cmd.append('--force')
         return cmd
 
     def prepare_patches_cmd(self):
+        branch = self.branch or self.refspec
         return ['git', 'checkout', '-q', '-B',
                 'patched-{refspec}'.
-                format(refspec=self.remove_ref_prefix(self.refspec))]
+                format(refspec=self.commit or self.remove_ref_prefix(branch))]
 
     def apply_patches_file_cmd(self, path):
         return ['git', 'apply', '--whitespace=nowarn', path]
 
     def set_remote_url_cmd(self):
         return ['git', 'remote', 'set-url', 'origin', self.effective_url]
 
@@ -446,34 +522,35 @@
             return ['true']
         return ['hg', 'clone', self.effective_url, self.path]
 
     def commit_cmd(self):
         return ['hg', 'commit', '--user', 'kas <kas@example.com>', '-m', 'msg']
 
     def contains_refspec_cmd(self):
-        return ['hg', 'log', '-r', self.refspec]
+        return ['hg', 'log', '-r', self.commit or self.branch or self.refspec]
 
     def fetch_cmd(self):
         return ['hg', 'pull']
 
     def is_dirty_cmd(self):
         return ['hg', 'diff']
 
     def resolve_branch_cmd(self):
-        # We never need to care about creating tracking branches in mercurial
-        return ['false']
+        return ['hg', 'identify', '--id', '-r', self.branch or self.refspec,
+                'default']
 
-    def checkout_cmd(self, desired_ref, branch):
+    def checkout_cmd(self, desired_ref, is_branch):
         cmd = ['hg', 'checkout', desired_ref]
         if get_context().force_checkout:
             cmd.append('--clean')
         return cmd
 
     def prepare_patches_cmd(self):
+        refspec = self.commit or self.branch or self.refspec
         return ['hg', 'branch', '-f',
-                'patched-{refspec}'.format(refspec=self.refspec)]
+                'patched-{refspec}'.format(refspec=refspec)]
 
     def apply_patches_file_cmd(self, path):
         return ['hg', 'import', '--no-commit', path]
 
     def set_remote_url_cmd(self):
         raise NotImplementedError()
```

### Comparing `kas-3.2.3/kas/schema-kas.json` & `kas-3.3/kas/schema-kas.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4882676866319444%*

 * *Differences: {"'$id'": "'https://github.com/siemens/kas/blob/master/kas/schema-kas.json'",*

 * * "'$schema'": "'http://json-schema.org/draft-04/schema#'",*

 * * "'description'": "'kas, a setup tool for bitbake based projects'",*

 * * "'properties'": "{'defaults': {'properties': {'repos': {'properties': {'branch': "*

 * *                 "OrderedDict([('type', 'string')])}}}}, 'repos': {'additionalProperties': "*

 * *                 "{'oneOf': {0: {'properties': {'commit': OrderedDict([('type', 'string')]), "*

 * *                 "'branch': Ordered […]*

```diff
@@ -1,10 +1,19 @@
 {
+    "$id": "https://github.com/siemens/kas/blob/master/kas/schema-kas.json",
+    "$schema": "http://json-schema.org/draft-04/schema#",
     "additionalProperties": false,
+    "description": "kas, a setup tool for bitbake based projects",
     "properties": {
+        "_source_dir": {
+            "type": "string"
+        },
+        "_source_dir_host": {
+            "type": "string"
+        },
         "bblayers_conf_header": {
             "additionalProperties": {
                 "type": "string"
             },
             "type": "object"
         },
         "build_system": {
@@ -17,14 +26,17 @@
         },
         "defaults": {
             "additionalProperties": false,
             "properties": {
                 "repos": {
                     "additionalProperties": false,
                     "properties": {
+                        "branch": {
+                            "type": "string"
+                        },
                         "patches": {
                             "additionalProperties": false,
                             "properties": {
                                 "repo": {
                                     "type": "string"
                                 }
                             },
@@ -120,14 +132,32 @@
                     {
                         "type": "integer"
                     }
                 ]
             },
             "type": "object"
         },
+        "overrides": {
+            "additionalProperties": false,
+            "properties": {
+                "repos": {
+                    "additionalProperties": {
+                        "additionalProperties": false,
+                        "properties": {
+                            "commit": {
+                                "type": "string"
+                            }
+                        },
+                        "type": "object"
+                    },
+                    "type": "object"
+                }
+            },
+            "type": "object"
+        },
         "proxy_config": {
             "additionalProperties": false,
             "properties": {
                 "ftp_proxy": {
                     "type": "string"
                 },
                 "http_proxy": {
@@ -144,14 +174,20 @@
         },
         "repos": {
             "additionalProperties": {
                 "oneOf": [
                     {
                         "additionalProperties": false,
                         "properties": {
+                            "branch": {
+                                "type": "string"
+                            },
+                            "commit": {
+                                "type": "string"
+                            },
                             "layers": {
                                 "additionalProperties": {
                                     "oneOf": [
                                         {
                                             "type": "null"
                                         },
                                         {
@@ -247,9 +283,10 @@
         "task": {
             "type": "string"
         }
     },
     "required": [
         "header"
     ],
+    "title": "kas configuration",
     "type": "object"
 }
```

### Comparing `kas-3.2.3/kas-container` & `kas-3.3/kas-container`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,16 @@
 	printf "%b" "--isar\t\t\tUse kas-isar container to build Isar image.\n"
 	printf "%b" "--with-loop-dev		Pass a loop device to the " \
 		    "container. Only required if\n"
 	printf "%b" "\t\t\tloop-mounting is used by recipes.\n"
 	printf "%b" "--runtime-args\t\tAdditional arguments to pass to the " \
 			"container runtime\n"
 	printf "%b" "\t\t\tfor running the build.\n"
-	printf "%b" "-d\t\t\tPrint debug output.\n"
+	printf "%b" "-d\t\t\tPrint debug output (deprecated, use -l debug).\n"
+	printf "%b" "-l, --log-level\t\tSet log level (default=info).\n"
 	printf "%b" "-v\t\t\tSame as -d (deprecated).\n"
 	printf "%b" "--version\t\tprint program version.\n"
 	printf "%b" "--ssh-dir\t\tDirectory containing SSH configurations.\n"
 	printf "%b" "\t\t\tAvoid \$HOME/.ssh unless you fully trust the " \
 		    "container.\n"
 	printf "%b" "--ssh-agent\t\tForward ssh-agent socket to the container.\n"
 	printf "%b" "--aws-dir\t\tDirectory containing AWScli configuration.\n"
@@ -116,44 +117,44 @@
 		# SC2086: Double quote to prevent globbing and word splitting.
 		# shellcheck disable=2086
 		trace ${KAS_CONTAINER_COMMAND} run -v "${KAS_BUILD_DIR}":/build:rw \
 				--workdir=/build --rm ${KAS_ISAR_ARGS} \
 				${KAS_CONTAINER_IMAGE} \
 				sudo rm -rf tmp
 	else
-		trace rm -rf "${KAS_BUILD_DIR}/tmp"
+		trace rm -rf "${KAS_BUILD_DIR}"/tmp*
 	fi
 
 	if [ "$1" != "clean" ]; then
 		SSTATE_DIR=${SSTATE_DIR:-${KAS_BUILD_DIR}/sstate-cache}
 		trace rm -rf "${SSTATE_DIR}"
 
 		if [ "$1" = "cleanall" ]; then
 			DL_DIR=${DL_DIR:-${KAS_BUILD_DIR}/downloads}
 			trace rm -rf "${DL_DIR}"
 		fi
 	fi
 }
 
-KAS_IMAGE_VERSION_DEFAULT="3.2.3"
+KAS_IMAGE_VERSION_DEFAULT="3.3"
 KAS_CONTAINER_IMAGE_PATH_DEFAULT="ghcr.io/siemens/kas"
 KAS_CONTAINER_IMAGE_NAME_DEFAULT="kas"
 
 set_container_image_var() {
 	KAS_IMAGE_VERSION="${KAS_IMAGE_VERSION:-${KAS_IMAGE_VERSION_DEFAULT}}"
 	KAS_CONTAINER_IMAGE_NAME="${KAS_CONTAINER_IMAGE_NAME:-${KAS_CONTAINER_IMAGE_NAME_DEFAULT}}"
 	KAS_CONTAINER_IMAGE_PATH="${KAS_CONTAINER_IMAGE_PATH:-${KAS_CONTAINER_IMAGE_PATH_DEFAULT}}"
 	KAS_CONTAINER_IMAGE_DEFAULT="${KAS_CONTAINER_IMAGE_PATH}/${KAS_CONTAINER_IMAGE_NAME}:${KAS_IMAGE_VERSION}"
 	KAS_CONTAINER_IMAGE="${KAS_CONTAINER_IMAGE:-${KAS_CONTAINER_IMAGE_DEFAULT}}"
 }
 
-KAS_WORK_DIR=$(readlink -f "${KAS_WORK_DIR:-$(pwd)}")
+KAS_WORK_DIR=$(readlink -fv "${KAS_WORK_DIR:-$(pwd)}")
 # KAS_WORK_DIR needs to exist for the subsequent code
 trace mkdir -p "${KAS_WORK_DIR}"
-KAS_BUILD_DIR=$(readlink -f "${KAS_BUILD_DIR:-${KAS_WORK_DIR}/build}")
+KAS_BUILD_DIR=$(readlink -fv "${KAS_BUILD_DIR:-${KAS_WORK_DIR}/build}")
 trace mkdir -p "${KAS_BUILD_DIR}"
 
 KAS_CONTAINER_ENGINE="${KAS_CONTAINER_ENGINE:-${KAS_DOCKER_ENGINE}}"
 if [ -z "${KAS_CONTAINER_ENGINE}" ]; then
 	# Try to auto-detect a container engine
 	if command -v docker >/dev/null; then
 		case $(docker -v 2>/dev/null) in
@@ -231,15 +232,15 @@
 		;;
 	--ssh-dir)
 		[ $# -gt 2 ] || usage
 		KAS_SSH_DIR="$2"
 		shift 2
 		;;
 	--ssh-agent)
-		KAS_SSH_AUTH_SOCK=$(readlink -f "$SSH_AUTH_SOCK")
+		KAS_SSH_AUTH_SOCK=$(readlink -fv "$SSH_AUTH_SOCK")
 		shift 1
 		;;
 	--aws-dir)
 		[ $# -gt 2 ] || usage
 		KAS_AWS_DIR="$2"
 		shift 2
 		;;
@@ -261,14 +262,21 @@
 		shift 1
 		;;
 	-v | -d)
 		KAS_VERBOSE=1
 		KAS_OPTIONS_DIRECT="${KAS_OPTIONS_DIRECT} -d"
 		shift 1
 		;;
+	-l | --log-level)
+		if [ "$2" = "debug" ]; then
+			KAS_VERBOSE=1
+		fi
+		KAS_OPTIONS_DIRECT="${KAS_OPTIONS_DIRECT} -l $2"
+		shift 2
+		;;
 	--version)
 		echo "$(basename "$0") $KAS_IMAGE_VERSION_DEFAULT"
 		exit 0
 		;;
 	--*)
 		usage
 		;;
@@ -279,40 +287,43 @@
 		;;
 	shell)
 		KAS_REPO_MOUNT_OPT_DEFAULT="rw"
 		KAS_CMD=$1
 		shift 1
 		break
 		;;
-	build|checkout|dump|for-all-repos|menu)
+	build|checkout|for-all-repos|menu)
 		KAS_REPO_MOUNT_OPT_DEFAULT="ro"
 		KAS_CMD=$1
 		shift 1
 		break
 		;;
+	dump)
+		if printf '%s\0' "$@" | grep -xqz -- '--inplace\|-i'; then
+			KAS_REPO_MOUNT_OPT_DEFAULT="rw"
+		else
+			KAS_REPO_MOUNT_OPT_DEFAULT="ro"
+		fi
+		KAS_CMD=$1
+		shift 1
+		break
+		;;
 	*)
 		usage
 		;;
 	esac
 done
 
 [ -n "${KAS_CMD}" ] || usage
 
 KAS_EXTRA_BITBAKE_ARGS=0
 
 # parse kas sub-command options
 while [ $# -gt 0 ] && [ $KAS_EXTRA_BITBAKE_ARGS -eq 0 ]; do
 	case "$1" in
-	-h|--help)
-		set_container_image_var
-		# SC2086: Double quote to prevent globbing and word splitting.
-		# shellcheck disable=2086
-		trace ${KAS_CONTAINER_COMMAND} run ${KAS_CONTAINER_IMAGE} ${KAS_CMD} --help
-		exit 0
-		;;
 	--skip|--target|--task)
 		KAS_OPTIONS="${KAS_OPTIONS} $1 $2"
 		shift 2
 		;;
 	-c|--cmd|--command)
 		KAS_BITBAKE_C_OPTION_ARGS="$2"
 		shift 2
@@ -358,19 +369,36 @@
 	KAS_REPO_DIR=$(git -C "${KAS_FILE_DIR}" rev-parse --show-toplevel 2>/dev/null) \
 		|| KAS_REPO_DIR=$(hg --cwd "${KAS_FILE_DIR}" root 2>/dev/null) \
 		|| KAS_REPO_DIR=${KAS_FILE_DIR}
 else
 	KAS_REPO_DIR=$(pwd)
 fi
 
+SOURCE_DIR_HOST=$(
+	grep -e "^_source_dir_host: " "${KAS_WORK_DIR}/.config.yaml" 2>/dev/null | \
+	sed 's/_source_dir_host:[ ]\+//')
+if [ -n "${SOURCE_DIR_HOST}" ]; then
+	KAS_REPO_DIR="${SOURCE_DIR_HOST}"
+fi
+
 if [ "${KAS_CMD}" = "menu" ]; then
 	if [ -z "${KAS_FIRST_FILE}" ]; then
 		KAS_FIRST_FILE="Kconfig"
 	fi
 
+	# When using the menu plugin, we need to track the KAS_REPO_DIR outside
+	# of the container to later allow a simple `kas-container build`. For
+	# that, we tell the kas menu plugin via an env-var about the location
+	# on the host. This data is then added to the .config.yaml where it can
+	# be evaluated by the next invocation of kas-container.
+
+	if ! [ "$(realpath -qe "${KAS_REPO_DIR}")" = "$(realpath -qe "${KAS_WORK_DIR}")" ]; then
+		set -- "$@" -e _KAS_REPO_DIR_HOST="$(readlink -fv "${KAS_REPO_DIR}")"
+	fi
+
 	BUILD_SYSTEM=$(tr '\n' '\f' 2>/dev/null < ${KAS_FIRST_FILE} | \
 		sed -e 's/\(.*\fconfig KAS_BUILD_SYSTEM\f\(.*\)\|.*\)/\2/' \
 		    -e 's/\f\([[:alpha:]].*\|$\)//' \
 		    -e 's/.*default \"\(.*\)\".*/\1/')
 else
 	if [ -z "${KAS_FIRST_FILE}" ]; then
 		KAS_FIRST_FILE="${KAS_WORK_DIR}/.config.yaml"
@@ -378,15 +406,15 @@
 
 	BUILD_SYSTEM=$(grep -e "^build_system: " "${KAS_FIRST_FILE}" 2>/dev/null | \
 		sed 's/build_system:[ ]\+//')
 fi
 
 if [ "${BUILD_SYSTEM}" = "isar" ]; then
 	enable_isar_mode
-else
+elif [ -z "${ISAR_MODE}" ]; then
 	enable_oe_mode
 fi
 
 set_container_image_var
 
 KAS_REPO_MOUNT_OPT="${KAS_REPO_MOUNT_OPT:-${KAS_REPO_MOUNT_OPT_DEFAULT}}"
 
@@ -407,15 +435,15 @@
 	-e USER_ID="$(id -u)" -e GROUP_ID="$(id -g)" --rm --init
 
 if [ -n "${KAS_SSH_DIR}" ] ; then
 	if [ ! -d "${KAS_SSH_DIR}" ]; then
 		echo "Passed KAS_SSH_DIR '${KAS_SSH_DIR}' is not a directory"
 		exit 1
 	fi
-	set -- "$@" -v "$(readlink -f "${KAS_SSH_DIR}")":/var/kas/userdata/.ssh:ro
+	set -- "$@" -v "$(readlink -fv "${KAS_SSH_DIR}")":/var/kas/userdata/.ssh:ro
 fi
 
 if [ -n "${KAS_SSH_AUTH_SOCK}" ]; then
 	if [ ! -S "${KAS_SSH_AUTH_SOCK}" ]; then
 		echo "Passed SSH_AUTH_SOCK '${KAS_SSH_AUTH_SOCK}' is not a socket"
 		exit 1
 	fi
@@ -424,71 +452,72 @@
 fi
 
 if [ -n "${KAS_AWS_DIR}" ] ; then
 	if [ ! -d "${KAS_AWS_DIR}" ]; then
 		echo "Passed KAS_AWS_DIR '${KAS_AWS_DIR}' is not a directory"
 		exit 1
 	fi
-	set -- "$@" -v "$(readlink -f "${KAS_AWS_DIR}")":/var/kas/userdata/.aws:ro \
+	set -- "$@" -v "$(readlink -fv "${KAS_AWS_DIR}")":/var/kas/userdata/.aws:ro \
 		-e AWS_CONFIG_FILE="${AWS_CONFIG_FILE:-/var/kas/userdata/.aws/config}" \
 		-e AWS_SHARED_CREDENTIALS_FILE="${AWS_SHARED_CREDENTIALS_FILE:-/var/kas/userdata/.aws/credentials}"
 fi
 
 KAS_GIT_CREDENTIAL_HELPER_DEFAULT=""
 
 if [ -n "${KAS_GIT_CREDENTIAL_STORE}" ] ; then
 	if [ ! -f "${KAS_GIT_CREDENTIAL_STORE}" ]; then
 		echo "Passed KAS_GIT_CREDENTIAL_STORE '${KAS_GIT_CREDENTIAL_STORE}' is not a file"
 		exit 1
 	fi
 	KAS_GIT_CREDENTIAL_HELPER_DEFAULT="store --file=/var/kas/userdata/.git-credentials"
-	set -- "$@" -v "$(readlink -f "${KAS_GIT_CREDENTIAL_STORE}")":/var/kas/userdata/.git-credentials:ro
+	set -- "$@" -v "$(readlink -fv "${KAS_GIT_CREDENTIAL_STORE}")":/var/kas/userdata/.git-credentials:ro
 fi
 
 GIT_CREDENTIAL_HELPER="${GIT_CREDENTIAL_HELPER:-${KAS_GIT_CREDENTIAL_HELPER_DEFAULT}}"
 
 if [ -n "${GIT_CREDENTIAL_HELPER}" ] ; then
 	set -- "$@" -e GIT_CREDENTIAL_HELPER="${GIT_CREDENTIAL_HELPER}"
 fi
 
 if [ -f "${NETRC_FILE}" ]; then
-	set -- "$@" -v "$(readlink -f "${NETRC_FILE}")":/var/kas/userdata/.netrc:ro \
+	set -- "$@" -v "$(readlink -fv "${NETRC_FILE}")":/var/kas/userdata/.netrc:ro \
 		-e NETRC_FILE="/var/kas/userdata/.netrc"
 fi
 
 if [ -t 1 ]; then
 	set -- "$@" -t -i
 fi
 
 if [ -n "${DL_DIR}" ]; then
 	trace mkdir -p "${DL_DIR}"
 	set -- "$@" \
-		-v "$(readlink -f "${DL_DIR}")":/downloads:rw \
+		-v "$(readlink -fv "${DL_DIR}")":/downloads:rw \
 		-e DL_DIR=/downloads
 fi
 
 if [ -n "${SSTATE_DIR}" ]; then
 	trace mkdir -p "${SSTATE_DIR}"
 	set -- "$@" \
-		-v "$(readlink -f "${SSTATE_DIR}")":/sstate:rw \
+		-v "$(readlink -fv "${SSTATE_DIR}")":/sstate:rw \
 		-e SSTATE_DIR=/sstate
 fi
 
 if [ -n "${KAS_REPO_REF_DIR}" ]; then
 	if [ ! -d "${KAS_REPO_REF_DIR}" ]; then
 		echo "Passed KAS_REPO_REF_DIR '${KAS_REPO_REF_DIR}' is not a directory"
 		exit 1
 	fi
 	set -- "$@" \
-		-v "$(readlink -f "${KAS_REPO_REF_DIR}")":/repo-ref:rw \
+		-v "$(readlink -fv "${KAS_REPO_REF_DIR}")":/repo-ref:rw \
 		-e KAS_REPO_REF_DIR=/repo-ref
 fi
 
 for var in TERM KAS_DISTRO KAS_MACHINE KAS_TARGET KAS_TASK \
-           KAS_PREMIRRORS DISTRO_APT_PREMIRRORS BB_NUMBER_THREADS PARALLEL_MAKE; do
+           KAS_PREMIRRORS DISTRO_APT_PREMIRRORS BB_NUMBER_THREADS PARALLEL_MAKE \
+           GIT_CREDENTIAL_USEHTTPPATH; do
 	if [ -n "$(eval echo \$${var})" ]; then
 		set -- "$@" -e "${var}=$(eval echo \"\$${var}\")"
 	fi
 done
 
 # propagate only supported SHELL settings
 case "$SHELL" in
```

### Comparing `kas-3.2.3/kas.egg-info/PKG-INFO` & `kas-3.3/kas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.2
 Name: kas
-Version: 3.2.3
+Version: 3.3
 Summary: Setup tool for bitbake based projects
 Home-page: https://github.com/siemens/kas
 Maintainer: Jan Kiszka
 Maintainer-email: jan.kiszka@siemens.com
 License: MIT
-Download-URL: https://github.com/siemens/kas/archive/3.2.3.tar.gz
+Download-URL: https://github.com/siemens/kas/archive/3.3.tar.gz
 Description: Setup tool for bitbake based projects
         =====================================
         
         +--------------------+
         |    Build Status    |
         +====================+
         | |workflow-master|_ |
@@ -53,13 +53,14 @@
 Keywords: OpenEmbedded bitbake development
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.5
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.6
```

### Comparing `kas-3.2.3/kas.egg-info/SOURCES.txt` & `kas-3.3/kas.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 kas/__main__.py
 kas/__version__.py
 kas/config.py
 kas/configschema.py
 kas/context.py
 kas/includehandler.py
 kas/kas.py
+kas/kasusererror.py
 kas/libcmds.py
 kas/libkas.py
 kas/repos.py
 kas/schema-kas.json
 kas.egg-info/PKG-INFO
 kas.egg-info/SOURCES.txt
 kas.egg-info/dependency_links.txt
```

### Comparing `kas-3.2.3/setup.py` & `kas-3.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,19 +66,20 @@
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
 
         # Pick your license as you wish (should match "license" above)
         'License :: OSI Approved :: MIT License',
 
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     keywords='OpenEmbedded bitbake development',
 
     packages=find_packages(),
 
     package_data={'kas': ['*.json']},
 
@@ -91,10 +92,10 @@
     install_requires=[
         'PyYAML>=3.0,<6',
         'distro>=1.0.0,<2',
         'jsonschema>=2.5.0,<4',
         'kconfiglib>=14.1.0,<15',
     ],
 
-    # At least python 3.5 is needed by now for PyYAML:
-    python_requires='>=3.5',
+    # At least python 3.6 is needed by now:
+    python_requires='>=3.6',
 )
```

