# Comparing `tmp/ablean-1.3.4.tar.gz` & `tmp/ablean-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ablean-1.3.4.tar", last modified: Fri Jun 10 02:23:07 2022, max compression
+gzip compressed data, was "ablean-1.3.5.tar", last modified: Tue Jun 20 10:20:44 2023, max compression
```

## Comparing `ablean-1.3.4.tar` & `ablean-1.3.5.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxrwx   0        0        0        0 2022-06-10 02:23:07.473300 ablean-1.3.4/
--rw-rw-rw-   0        0        0     2184 2022-06-06 10:43:40.000000 ablean-1.3.4/.gitignore
-drwxrwxrwx   0        0        0        0 2022-06-10 02:23:07.414443 ablean-1.3.4/.vscode/
--rw-rw-rw-   0        0        0     1445 2022-06-10 02:04:44.000000 ablean-1.3.4/.vscode/launch.json
--rw-rw-rw-   0        0        0    55819 2022-06-10 02:23:07.473300 ablean-1.3.4/PKG-INFO
--rw-rw-rw-   0        0        0    53240 2022-06-05 03:11:14.000000 ablean-1.3.4/README.md
-drwxrwxrwx   0        0        0        0 2022-06-10 02:23:07.417443 ablean-1.3.4/ablean/
--rw-rw-rw-   0        0        0      930 2022-06-10 02:22:49.000000 ablean-1.3.4/ablean/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-10 02:23:07.443300 ablean-1.3.4/ablean/commands/
--rw-rw-rw-   0        0        0     1273 2022-06-06 09:45:38.000000 ablean-1.3.4/ablean/commands/__init__.py
--rw-rw-rw-   0        0        0    12595 2022-06-05 10:53:45.000000 ablean-1.3.4/ablean/commands/backtest.py
--rw-rw-rw-   0        0        0    10248 2022-06-05 03:11:14.000000 ablean-1.3.4/ablean/commands/create_project.py
--rw-rw-rw-   0        0        0     1322 2022-06-10 02:17:02.000000 ablean-1.3.4/ablean/commands/download.py
--rw-rw-rw-   0        0        0     2098 2022-06-06 10:41:51.000000 ablean-1.3.4/ablean/commands/init.py
-drwxrwxrwx   0        0        0        0 2022-06-10 02:23:07.445300 ablean-1.3.4/ablean/components/
--rw-rw-rw-   0        0        0      676 2022-06-05 03:11:14.000000 ablean-1.3.4/ablean/components/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-10 02:23:07.449300 ablean-1.3.4/ablean/components/config/
--rw-rw-rw-   0        0        0      676 2022-06-05 03:11:14.000000 ablean-1.3.4/ablean/components/config/__init__.py
--rw-rw-rw-   0        0        0     2786 2022-06-05 03:11:14.000000 ablean-1.3.4/ablean/components/config/cli_config_manager.py
--rw-rw-rw-   0        0        0    13701 2022-06-06 10:41:19.000000 ablean-1.3.4/ablean/components/config/lean_config_manager.py
--rw-rw-rw-   0        0        0     5417 2022-06-05 03:11:14.000000 ablean-1.3.4/ablean/components/config/output_config_manager.py
--rw-rw-rw-   0        0        0     2435 2022-06-05 03:11:14.000000 ablean-1.3.4/ablean/components/config/project_config_manager.py
--rw-rw-rw-   0        0        0     3279 2022-06-05 07:48:48.000000 ablean-1.3.4/ablean/components/config/storage.py
--rw-rw-rw-   0        0        0     5080 2022-06-05 03:11:14.000000 ablean-1.3.4/ablean/components/lean_runner.py
--rw-rw-rw-   0        0        0     2787 2022-06-05 03:11:14.000000 ablean-1.3.4/ablean/components/module_manager.py
-drwxrwxrwx   0        0        0        0 2022-06-10 02:23:07.454300 ablean-1.3.4/ablean/components/util/
--rw-rw-rw-   0        0        0      676 2022-06-05 08:19:14.000000 ablean-1.3.4/ablean/components/util/__init__.py
--rw-rw-rw-   0        0        0     6356 2022-06-05 03:11:14.000000 ablean-1.3.4/ablean/components/util/logger.py
--rw-rw-rw-   0        0        0     1368 2022-06-05 03:11:14.000000 ablean-1.3.4/ablean/components/util/name_extraction.py
--rw-rw-rw-   0        0        0     3205 2022-06-05 03:11:14.000000 ablean-1.3.4/ablean/components/util/name_generator.py
--rw-rw-rw-   0        0        0     3261 2022-06-05 03:11:14.000000 ablean-1.3.4/ablean/components/util/path_manager.py
--rw-rw-rw-   0        0        0     4584 2022-06-05 03:11:14.000000 ablean-1.3.4/ablean/components/util/platform_manager.py
--rw-rw-rw-   0        0        0    21926 2022-06-05 04:02:32.000000 ablean-1.3.4/ablean/components/util/project_manager.py
--rw-rw-rw-   0        0        0     1689 2022-06-05 03:11:14.000000 ablean-1.3.4/ablean/components/util/temp_manager.py
--rw-rw-rw-   0        0        0     1680 2022-06-05 03:11:14.000000 ablean-1.3.4/ablean/components/util/xml_manager.py
--rw-rw-rw-   0        0        0     4445 2022-06-06 06:09:31.000000 ablean-1.3.4/ablean/constants.py
--rw-rw-rw-   0        0        0     3838 2022-06-05 03:11:14.000000 ablean-1.3.4/ablean/container.py
--rw-rw-rw-   0        0        0     8363 2022-06-09 08:32:05.000000 ablean-1.3.4/ablean/data_manager.py
-drwxrwxrwx   0        0        0        0 2022-06-10 02:23:07.468299 ablean-1.3.4/ablean/icons/
--rw-rw-rw-   0        0        0    34808 2022-06-05 03:11:14.000000 ablean-1.3.4/ablean/icons/icon.icns
--rw-rw-rw-   0        0        0    14816 2022-06-05 03:11:14.000000 ablean-1.3.4/ablean/icons/icon.ico
--rw-rw-rw-   0        0        0     5968 2022-06-06 09:47:56.000000 ablean-1.3.4/ablean/main.py
-drwxrwxrwx   0        0        0        0 2022-06-10 02:23:07.471300 ablean-1.3.4/ablean/models/
--rw-rw-rw-   0        0        0      676 2022-06-05 03:11:14.000000 ablean-1.3.4/ablean/models/__init__.py
--rw-rw-rw-   0        0        0     2305 2022-06-05 03:11:14.000000 ablean-1.3.4/ablean/models/errors.py
--rw-rw-rw-   0        0        0     1555 2022-06-05 03:11:14.000000 ablean-1.3.4/ablean/models/modules.py
--rw-rw-rw-   0        0        0     4037 2022-06-05 03:11:14.000000 ablean-1.3.4/ablean/models/options.py
--rw-rw-rw-   0        0        0     1507 2022-06-05 03:11:14.000000 ablean-1.3.4/ablean/models/pydantic.py
--rw-rw-rw-   0        0        0     1456 2022-06-05 03:11:14.000000 ablean-1.3.4/ablean/models/utils.py
--rw-rw-rw-   0        0        0     9966 2022-06-05 03:11:14.000000 ablean-1.3.4/ablean/myclick.py
-drwxrwxrwx   0        0        0        0 2022-06-10 02:23:07.440300 ablean-1.3.4/ablean.egg-info/
--rw-rw-rw-   0        0        0    55819 2022-06-10 02:23:06.000000 ablean-1.3.4/ablean.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1428 2022-06-10 02:23:07.000000 ablean-1.3.4/ablean.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-10 02:23:06.000000 ablean-1.3.4/ablean.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2022-06-10 02:23:07.000000 ablean-1.3.4/ablean.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      302 2022-06-10 02:23:07.000000 ablean-1.3.4/ablean.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-06-10 02:23:07.000000 ablean-1.3.4/ablean.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      913 2022-06-05 05:44:09.000000 ablean-1.3.4/pub.ps1
-drwxrwxrwx   0        0        0        0 2022-06-10 02:23:07.472299 ablean-1.3.4/scripts/
--rw-rw-rw-   0        0        0     3900 2022-06-05 03:31:44.000000 ablean-1.3.4/scripts/readme.py
--rw-rw-rw-   0        0        0       42 2022-06-10 02:23:07.473300 ablean-1.3.4/setup.cfg
--rw-rw-rw-   0        0        0     3443 2022-06-05 05:42:03.000000 ablean-1.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:20:44.472756 ablean-1.3.5/
+-rw-rw-rw-   0        0        0     2184 2022-06-06 10:43:40.000000 ablean-1.3.5/.gitignore
+drwxrwxrwx   0        0        0        0 2023-06-20 10:20:44.300584 ablean-1.3.5/.vscode/
+-rw-rw-rw-   0        0        0     1442 2023-04-20 14:13:20.000000 ablean-1.3.5/.vscode/launch.json
+-rw-rw-rw-   0        0        0    55778 2023-06-20 10:20:44.472756 ablean-1.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0    53240 2022-06-05 03:11:14.000000 ablean-1.3.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 10:20:44.318037 ablean-1.3.5/ablean/
+-rw-rw-rw-   0        0        0      930 2023-06-20 10:20:31.000000 ablean-1.3.5/ablean/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:20:44.371460 ablean-1.3.5/ablean/commands/
+-rw-rw-rw-   0        0        0     1273 2022-06-06 09:45:38.000000 ablean-1.3.5/ablean/commands/__init__.py
+-rw-rw-rw-   0        0        0    12595 2022-06-05 10:53:45.000000 ablean-1.3.5/ablean/commands/backtest.py
+-rw-rw-rw-   0        0        0    10248 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/commands/create_project.py
+-rw-rw-rw-   0        0        0     1322 2022-06-10 02:17:02.000000 ablean-1.3.5/ablean/commands/download.py
+-rw-rw-rw-   0        0        0     2098 2022-06-06 10:41:51.000000 ablean-1.3.5/ablean/commands/init.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:20:44.379490 ablean-1.3.5/ablean/components/
+-rw-rw-rw-   0        0        0      676 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/components/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:20:44.396826 ablean-1.3.5/ablean/components/config/
+-rw-rw-rw-   0        0        0      676 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/components/config/__init__.py
+-rw-rw-rw-   0        0        0     2786 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/components/config/cli_config_manager.py
+-rw-rw-rw-   0        0        0    13701 2022-06-06 10:41:19.000000 ablean-1.3.5/ablean/components/config/lean_config_manager.py
+-rw-rw-rw-   0        0        0     5417 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/components/config/output_config_manager.py
+-rw-rw-rw-   0        0        0     2435 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/components/config/project_config_manager.py
+-rw-rw-rw-   0        0        0     3279 2022-06-05 07:48:48.000000 ablean-1.3.5/ablean/components/config/storage.py
+-rw-rw-rw-   0        0        0     5080 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/components/lean_runner.py
+-rw-rw-rw-   0        0        0     2787 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/components/module_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:20:44.429169 ablean-1.3.5/ablean/components/util/
+-rw-rw-rw-   0        0        0      676 2022-06-05 08:19:14.000000 ablean-1.3.5/ablean/components/util/__init__.py
+-rw-rw-rw-   0        0        0     6356 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/components/util/logger.py
+-rw-rw-rw-   0        0        0     1368 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/components/util/name_extraction.py
+-rw-rw-rw-   0        0        0     3205 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/components/util/name_generator.py
+-rw-rw-rw-   0        0        0     3261 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/components/util/path_manager.py
+-rw-rw-rw-   0        0        0     4584 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/components/util/platform_manager.py
+-rw-rw-rw-   0        0        0    21926 2022-06-05 04:02:32.000000 ablean-1.3.5/ablean/components/util/project_manager.py
+-rw-rw-rw-   0        0        0     1689 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/components/util/temp_manager.py
+-rw-rw-rw-   0        0        0     1680 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/components/util/xml_manager.py
+-rw-rw-rw-   0        0        0     4445 2022-06-06 06:09:31.000000 ablean-1.3.5/ablean/constants.py
+-rw-rw-rw-   0        0        0     3838 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/container.py
+-rw-rw-rw-   0        0        0     8436 2022-06-22 06:13:42.000000 ablean-1.3.5/ablean/data_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:20:44.439354 ablean-1.3.5/ablean/icons/
+-rw-rw-rw-   0        0        0    34808 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/icons/icon.icns
+-rw-rw-rw-   0        0        0    14816 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/icons/icon.ico
+-rw-rw-rw-   0        0        0     5968 2022-06-06 09:47:56.000000 ablean-1.3.5/ablean/main.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:20:44.463267 ablean-1.3.5/ablean/models/
+-rw-rw-rw-   0        0        0      676 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/models/__init__.py
+-rw-rw-rw-   0        0        0     2305 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/models/errors.py
+-rw-rw-rw-   0        0        0     1555 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/models/modules.py
+-rw-rw-rw-   0        0        0     4037 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/models/options.py
+-rw-rw-rw-   0        0        0     1507 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/models/pydantic.py
+-rw-rw-rw-   0        0        0     1456 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/models/utils.py
+-rw-rw-rw-   0        0        0     9966 2022-06-05 03:11:14.000000 ablean-1.3.5/ablean/myclick.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:20:44.342254 ablean-1.3.5/ablean.egg-info/
+-rw-rw-rw-   0        0        0    55778 2023-06-20 10:20:44.000000 ablean-1.3.5/ablean.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1428 2023-06-20 10:20:44.000000 ablean-1.3.5/ablean.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 10:20:44.000000 ablean-1.3.5/ablean.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-20 10:20:44.000000 ablean-1.3.5/ablean.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      302 2023-06-20 10:20:44.000000 ablean-1.3.5/ablean.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-20 10:20:44.000000 ablean-1.3.5/ablean.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      913 2022-06-05 05:44:09.000000 ablean-1.3.5/pub.ps1
+drwxrwxrwx   0        0        0        0 2023-06-20 10:20:44.470762 ablean-1.3.5/scripts/
+-rw-rw-rw-   0        0        0     3900 2022-06-05 03:31:44.000000 ablean-1.3.5/scripts/readme.py
+-rw-rw-rw-   0        0        0       42 2023-06-20 10:20:44.473756 ablean-1.3.5/setup.cfg
+-rw-rw-rw-   0        0        0     3443 2022-06-05 05:42:03.000000 ablean-1.3.5/setup.py
```

### Comparing `ablean-1.3.4/.gitignore` & `ablean-1.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `ablean-1.3.4/.vscode/launch.json` & `ablean-1.3.5/.vscode/launch.json`

 * *Files 8% similar despite different names*

```diff
@@ -14,20 +14,20 @@
         {
             "name": "ablean",
             "type": "python",
             "request": "launch",
             "program": "${workspaceFolder}${pathSeparator}ablean${pathSeparator}main.py",
             "args": [
                 // "init",
-                // "backtest",
-                "download",
+                "backtest",
+                // "download",
                 // "--market", "deribit"
                 // "--date-start", "2022-06-03",
                 // "--date-end", "2022-06-04",
-                // "c:/work/repos/lean/demo1/deribit_backtest.py",
+                "c:/work/repos/lean/demo1/deribit_backtest.py",
                 // "--download-data",
                 // "--debug",
                 // "-h", "119.8.180.153",
                 // "-u", "data_sync",
                 // "-w", "5@peksync"
             ],
             "cwd": "${workspaceFolder}/temp",
```

### Comparing `ablean-1.3.4/PKG-INFO` & `ablean-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: ablean
-Version: 1.3.4
+Version: 1.3.5
 Summary: A CLI aimed at making it easier to run QuantConnect's LEAN engine locally and in the cloud
 Home-page: https://lean.io/cli
 Author: abl
 Author-email: support@quantconnect.com
-License: UNKNOWN
 Project-URL: Documentation, https://www.lean.io/docs/lean-cli/key-concepts/getting-started
 Project-URL: Source, https://github.com/QuantConnect/lean-cli
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -1134,9 +1132,7 @@
 If you need to add dependencies, first update `setup.py` (if it is a production dependency) or `requirements.txt` (if it is a development dependency) and then re-run `pip install -r requirements.txt`.
 
 The automated tests can be ran by running `pytest`. The filesystem and HTTP requests are mocked when running tests to make sure they run in an isolated environment.
 
 Can build the lean CLI by running `python setup.py sdist bdist_wheel` from the root of the project and to install it `pip install --force-reinstall dist/lean-dev-py3-none-any.whl`. To update the commands reference part of the readme run `python scripts/readme.py` from the root of the project, after installing the new version.
 
 Maintainers can publish new releases by pushing a Git tag containing the new version to GitHub. This will trigger a GitHub Actions workflow which releases the current `master` branch to PyPI with the value of the tag as version. Make sure the version is not prefixed with "v".
-
-
```

### Comparing `ablean-1.3.4/README.md` & `ablean-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `ablean-1.3.4/ablean/__init__.py` & `ablean-1.3.5/ablean/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # The version is always set to "dev" in the Git repository. When a new release is ready,
 # a maintainer will push a new Git tag which will trigger GitHub Actions to publish a new
 # package to PyPI with the version of the tag.
-__version__ = "1.3.4"
+__version__ = "1.3.5"
```

### Comparing `ablean-1.3.4/ablean/commands/__init__.py` & `ablean-1.3.5/ablean/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.4/ablean/commands/backtest.py` & `ablean-1.3.5/ablean/commands/backtest.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.4/ablean/commands/create_project.py` & `ablean-1.3.5/ablean/commands/create_project.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.4/ablean/commands/download.py` & `ablean-1.3.5/ablean/commands/download.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.4/ablean/commands/init.py` & `ablean-1.3.5/ablean/commands/init.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.4/ablean/components/__init__.py` & `ablean-1.3.5/ablean/components/__init__.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.4/ablean/components/config/__init__.py` & `ablean-1.3.5/ablean/components/config/__init__.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.4/ablean/components/config/cli_config_manager.py` & `ablean-1.3.5/ablean/components/config/cli_config_manager.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.4/ablean/components/config/lean_config_manager.py` & `ablean-1.3.5/ablean/components/config/lean_config_manager.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.4/ablean/components/config/output_config_manager.py` & `ablean-1.3.5/ablean/components/config/output_config_manager.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.4/ablean/components/config/project_config_manager.py` & `ablean-1.3.5/ablean/components/config/project_config_manager.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.4/ablean/components/config/storage.py` & `ablean-1.3.5/ablean/components/config/storage.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.4/ablean/components/lean_runner.py` & `ablean-1.3.5/ablean/components/lean_runner.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.4/ablean/components/module_manager.py` & `ablean-1.3.5/ablean/components/module_manager.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.4/ablean/components/util/__init__.py` & `ablean-1.3.5/ablean/components/util/__init__.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.4/ablean/components/util/logger.py` & `ablean-1.3.5/ablean/components/util/logger.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.4/ablean/components/util/name_extraction.py` & `ablean-1.3.5/ablean/components/util/name_extraction.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.4/ablean/components/util/name_generator.py` & `ablean-1.3.5/ablean/components/util/name_generator.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.4/ablean/components/util/path_manager.py` & `ablean-1.3.5/ablean/components/util/path_manager.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.4/ablean/components/util/platform_manager.py` & `ablean-1.3.5/ablean/components/util/platform_manager.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.4/ablean/components/util/project_manager.py` & `ablean-1.3.5/ablean/components/util/project_manager.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.4/ablean/components/util/temp_manager.py` & `ablean-1.3.5/ablean/components/util/temp_manager.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.4/ablean/components/util/xml_manager.py` & `ablean-1.3.5/ablean/components/util/xml_manager.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.4/ablean/constants.py` & `ablean-1.3.5/ablean/constants.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.4/ablean/container.py` & `ablean-1.3.5/ablean/container.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.4/ablean/data_manager.py` & `ablean-1.3.5/ablean/data_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import sys
 import pathlib
 import logging
 import argparse
 from typing import Dict, Optional
 from os import listdir, scandir
 from os.path import join, exists, isfile, getsize
-from paramiko import SSHClient
+from paramiko import SSHClient, AutoAddPolicy
 from scp import SCPClient
 from ablean.components.util.logger import Logger
 from ablean.components.config.lean_config_manager import LeanConfigManager
 from ablean.constants import DATA_HASH_FILE, DEFAULT_LEAN_CONFIG_FILE_NAME
 
 DATE_FORMAT = "%Y%m%d"
 OPTION_DATE_START_POS = -len('20220523_quote_european.zip')
@@ -159,14 +159,15 @@
         self.ssh_user = config["ssh-user"]
         self.ssh_password = config["ssh-pwd"]
         self.update_second_data = config["update-second-data"]
 
     def _create_scp(self):
         ssh = SSHClient()
         ssh.load_system_host_keys()
+        ssh.set_missing_host_key_policy(AutoAddPolicy())
         ssh.connect(
             self.ssh_host,
             port=self.ssh_port,
             username=self.ssh_user,
             password=self.ssh_password,
             compress=True,
         )
```

### Comparing `ablean-1.3.4/ablean/icons/icon.icns` & `ablean-1.3.5/ablean/icons/icon.icns`

 * *Files identical despite different names*

### Comparing `ablean-1.3.4/ablean/icons/icon.ico` & `ablean-1.3.5/ablean/icons/icon.ico`

 * *Files identical despite different names*

### Comparing `ablean-1.3.4/ablean/main.py` & `ablean-1.3.5/ablean/main.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.4/ablean/models/__init__.py` & `ablean-1.3.5/ablean/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.4/ablean/models/errors.py` & `ablean-1.3.5/ablean/models/errors.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.4/ablean/models/modules.py` & `ablean-1.3.5/ablean/models/modules.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.4/ablean/models/options.py` & `ablean-1.3.5/ablean/models/options.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.4/ablean/models/pydantic.py` & `ablean-1.3.5/ablean/models/pydantic.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.4/ablean/models/utils.py` & `ablean-1.3.5/ablean/models/utils.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.4/ablean/myclick.py` & `ablean-1.3.5/ablean/myclick.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.4/ablean.egg-info/PKG-INFO` & `ablean-1.3.5/ablean.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: ablean
-Version: 1.3.4
+Version: 1.3.5
 Summary: A CLI aimed at making it easier to run QuantConnect's LEAN engine locally and in the cloud
 Home-page: https://lean.io/cli
 Author: abl
 Author-email: support@quantconnect.com
-License: UNKNOWN
 Project-URL: Documentation, https://www.lean.io/docs/lean-cli/key-concepts/getting-started
 Project-URL: Source, https://github.com/QuantConnect/lean-cli
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -1134,9 +1132,7 @@
 If you need to add dependencies, first update `setup.py` (if it is a production dependency) or `requirements.txt` (if it is a development dependency) and then re-run `pip install -r requirements.txt`.
 
 The automated tests can be ran by running `pytest`. The filesystem and HTTP requests are mocked when running tests to make sure they run in an isolated environment.
 
 Can build the lean CLI by running `python setup.py sdist bdist_wheel` from the root of the project and to install it `pip install --force-reinstall dist/lean-dev-py3-none-any.whl`. To update the commands reference part of the readme run `python scripts/readme.py` from the root of the project, after installing the new version.
 
 Maintainers can publish new releases by pushing a Git tag containing the new version to GitHub. This will trigger a GitHub Actions workflow which releases the current `master` branch to PyPI with the value of the tag as version. Make sure the version is not prefixed with "v".
-
-
```

### Comparing `ablean-1.3.4/ablean.egg-info/SOURCES.txt` & `ablean-1.3.5/ablean.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ablean-1.3.4/pub.ps1` & `ablean-1.3.5/pub.ps1`

 * *Files identical despite different names*

### Comparing `ablean-1.3.4/scripts/readme.py` & `ablean-1.3.5/scripts/readme.py`

 * *Files identical despite different names*

### Comparing `ablean-1.3.4/setup.py` & `ablean-1.3.5/setup.py`

 * *Files identical despite different names*

