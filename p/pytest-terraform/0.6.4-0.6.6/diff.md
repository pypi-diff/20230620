# Comparing `tmp/pytest-terraform-0.6.4.tar.gz` & `tmp/pytest_terraform-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-terraform-0.6.4.tar", max compression
+gzip compressed data, was "pytest_terraform-0.6.6.tar", max compression
```

## Comparing `pytest-terraform-0.6.4.tar` & `pytest_terraform-0.6.6.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     9383 2022-09-01 13:58:00.783953 pytest-terraform-0.6.4/README.md
--rw-r--r--   0        0        0     1457 2022-09-01 13:58:00.783953 pytest-terraform-0.6.4/pyproject.toml
--rw-r--r--   0        0        0      670 2022-09-01 13:58:00.783953 pytest-terraform-0.6.4/pytest_terraform/__init__.py
--rw-r--r--   0        0        0      500 2022-09-01 13:58:00.783953 pytest-terraform-0.6.4/pytest_terraform/exceptions.py
--rw-r--r--   0        0        0       93 2022-09-01 13:58:00.783953 pytest-terraform-0.6.4/pytest_terraform/hooks.py
--rw-r--r--   0        0        0     2003 2022-09-01 13:58:00.783953 pytest-terraform-0.6.4/pytest_terraform/lock.py
--rw-r--r--   0        0        0      835 2022-09-01 13:58:00.783953 pytest-terraform-0.6.4/pytest_terraform/options.py
--rw-r--r--   0        0        0     2955 2022-09-01 13:58:00.783953 pytest-terraform-0.6.4/pytest_terraform/plugin.py
--rw-r--r--   0        0        0    16442 2022-09-01 13:58:00.783953 pytest-terraform-0.6.4/pytest_terraform/tf.py
--rw-r--r--   0        0        0     7614 2022-09-01 13:58:00.783953 pytest-terraform-0.6.4/pytest_terraform/xdist.py
--rw-r--r--   0        0        0    10514 1970-01-01 00:00:00.000000 pytest-terraform-0.6.4/setup.py
--rw-r--r--   0        0        0    10446 1970-01-01 00:00:00.000000 pytest-terraform-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0     9196 2023-06-20 19:51:13.690254 pytest_terraform-0.6.6/README.md
+-rw-r--r--   0        0        0     1466 2023-06-20 19:51:13.690254 pytest_terraform-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0      670 2023-06-20 19:51:13.690254 pytest_terraform-0.6.6/pytest_terraform/__init__.py
+-rw-r--r--   0        0        0      500 2023-06-20 19:51:13.690254 pytest_terraform-0.6.6/pytest_terraform/exceptions.py
+-rw-r--r--   0        0        0       93 2023-06-20 19:51:13.690254 pytest_terraform-0.6.6/pytest_terraform/hooks.py
+-rw-r--r--   0        0        0     2003 2023-06-20 19:51:13.690254 pytest_terraform-0.6.6/pytest_terraform/lock.py
+-rw-r--r--   0        0        0      835 2023-06-20 19:51:13.690254 pytest_terraform-0.6.6/pytest_terraform/options.py
+-rw-r--r--   0        0        0     3102 2023-06-20 19:51:13.690254 pytest_terraform-0.6.6/pytest_terraform/plugin.py
+-rw-r--r--   0        0        0    16910 2023-06-20 19:51:13.690254 pytest_terraform-0.6.6/pytest_terraform/tf.py
+-rw-r--r--   0        0        0     7414 2023-06-20 19:51:13.690254 pytest_terraform-0.6.6/pytest_terraform/xdist.py
+-rw-r--r--   0        0        0    10260 1970-01-01 00:00:00.000000 pytest_terraform-0.6.6/PKG-INFO
```

### Comparing `pytest-terraform-0.6.4/README.md` & `pytest_terraform-0.6.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -96,20 +96,14 @@
 ## Options
 
 You can provide the path to the terraform binary else its auto discovered
 ```shell
 --tf-binary=$HOME/bin/terraform
 ```
 
-To avoid repeated downloading of plugins a plugin cache dir is utilized
-by default this is `.tfcache` in the current working directory.
-```shell
---tf-plugin-dir=$HOME/.cache/tfcache
-```
-
 Terraform modules referenced by fixtures are looked up in a few different
 locations, directly in the same directory as the test module, in a subdir
 named terraform, and in a sibling directory named terraform. An explicit
 directory can be given which will be looked at first for all modules.
 
 ```shell
 --tf-mod-dir=terraform
```

### Comparing `pytest-terraform-0.6.4/pyproject.toml` & `pytest_terraform-0.6.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [tool.poetry]
 name = "pytest-terraform"
-version = "0.6.4"
+version = "0.6.6"
 description = "A pytest plugin for using terraform fixtures"
 authors = ["Kapil Thangavelu <kapilt@gmail.com>"]
 license = "Apache-2.0"
 repository = "https://github.com/cloud-custodian/pytest-terraform"
 classifiers=[
    "Topic :: Software Development :: Testing",
    "Topic :: System :: Systems Administration",
    "Topic :: System :: Distributed Computing"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.6"
+python = ">=3.7,<4.0"
 pytest = ">= 6.0"
 jmespath = ">= 0.10.0"
 portalocker = ">= 1.7.0"
 pytest-xdist = ">= 1.31.0"
 
 [tool.poetry.dev-dependencies]
 black = ">=19.10b0"
 isort = ">=4.3.21"
 flake8 = ">=3.7.9"
 coverage = ">=6.1"
 pytest-cov = ">=2.8.1"
-pre-commit = "^2.1"
+pre-commit = ">=2.9.2"
 
 [tool.poetry.plugins.pytest11]
 terraform = "pytest_terraform.plugin"
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 testpaths = ["tests"]
```

### Comparing `pytest-terraform-0.6.4/pytest_terraform/__init__.py` & `pytest_terraform-0.6.6/pytest_terraform/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-terraform-0.6.4/pytest_terraform/lock.py` & `pytest_terraform-0.6.6/pytest_terraform/lock.py`

 * *Files identical despite different names*

### Comparing `pytest-terraform-0.6.4/pytest_terraform/options.py` & `pytest_terraform-0.6.6/pytest_terraform/options.py`

 * *Files identical despite different names*

### Comparing `pytest-terraform-0.6.4/pytest_terraform/plugin.py` & `pytest_terraform-0.6.6/pytest_terraform/plugin.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,30 +8,29 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import os
 import shutil
 from collections import defaultdict
 
 import pytest
 from pytest_terraform import hooks, tf, xdist
 
 
 @pytest.hookimpl(trylast=True)
 def pytest_configure(config):
     config.addinivalue_line("markers", "terraform: tests using terraform fixtures")
 
     cache_dir = config.getoption("dest_tf_plugin")
-    if not os.path.exists(cache_dir):
-        os.mkdir(cache_dir)
-    tf.LazyPluginCacheDir.value = os.path.abspath(cache_dir)
+
+    if cache_dir:
+        pass
 
     tf.LazyModuleDir.value = config.getoption("dest_tf_mod_dir") or config.getini(
         "terraform-mod-dir"
     )
 
     if tf.LazyReplay.value is None:
         tf.LazyReplay.value = config.getoption("dest_tf_replay")
@@ -40,14 +39,15 @@
     if tf.LazyTfBin.value is None and not tf.LazyReplay.value:
         raise ValueError(
             "pytest-terraform requires terraform binary on PATH or "
             "specified with --tf-binary"
         )
 
     tf.PytestConfig.value = config
+    tf.LazyTFDebug.value = config.getoption("dest_tf_debug") or False
 
     if config.pluginmanager.hasplugin("xdist"):
         config.pluginmanager.register(xdist.XDistTerraform(config))
         tf.terraform.scope_class_map = d = defaultdict(
             lambda: xdist.ScopedTerraformFixture
         )
         d["function"] = tf.TerraformFixture
@@ -69,24 +69,30 @@
     group.addoption(
         "--tf-replay",
         action="store_true",
         dest="dest_tf_replay",
         help=("Use recorded resources instead of invoking terraform"),
     )
     group.addoption(
+        "--tf-debug",
+        action="store_true",
+        dest="dest_tf_debug",
+        help=("Debug terraform output and plugin output"),
+    )
+    group.addoption(
         "--tf-mod-dir",
         action="store",
         dest="dest_tf_mod_dir",
         help=("Configue the parent directory to look for terraform modules"),
     )
     group.addoption(
         "--tf-plugin-dir",
         action="store",
         dest="dest_tf_plugin",
         default=".tfcache",
         help=(
-            "Use this directory for a terraform plugin cache "
-            "Default is to use .tfcache"
+            "[Depreceated] Use this directory for a terraform plugin cache "
+            "Default is to use .tfcache."
         ),
     )
 
     parser.addini("terraform-mod-dir", "Parent Directory for terraform modules")
```

### Comparing `pytest-terraform-0.6.4/pytest_terraform/tf.py` & `pytest_terraform-0.6.6/pytest_terraform/tf.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,41 +24,37 @@
 from py.path import local
 
 from .exceptions import InvalidState, ModuleNotFound, TerraformCommandFailed
 from .options import teardown as td
 
 
 class TerraformRunner(object):
-
     command_templates = {
         "init": "init {input} {color} {plugin_dir}",
         "apply": "apply {input} {color} {state} {approve} {plan}",
         "plan": "plan {input} {color} {state} {output}",
         "destroy": "destroy {input} {color} {state} {approve}",
         "show": "show {color} -json {state_path}",
     }
 
     template_defaults = {
         "input": "-input=false",
         "color": "-no-color",
         "approve": "-auto-approve",
     }
 
-    debug = False
-
     def __init__(
         self,
         work_dir,
         state_path=None,
         module_dir=None,
         plugin_cache=None,
         stream_output=None,
         tf_bin=None,
     ):
-
         self.work_dir = work_dir
         self.module_dir = module_dir
         # use parent dir of work/data dir to avoid
         # https://github.com/hashicorp/terraform/issues/22999
         self.state_path = state_path or os.path.join(work_dir, "..", "terraform.tfstate")
         self.stream_output = stream_output
         self.plugin_cache = plugin_cache or ""
@@ -68,16 +64,23 @@
         """run terraform apply"""
         if plan is True:
             plan_path = os.path.join(self.work_dir, "tfplan")
             self.plan(plan_path)
             apply_args = self._get_cmd_args("apply", plan=plan_path)
         elif plan:
             apply_args = self._get_cmd_args("apply", plan="")
-        self._run_cmd(apply_args)
-        return TerraformState.from_file(self.state_path, self)
+        try:
+            self._run_cmd(apply_args)
+            return TerraformState.from_file(self.state_path, self)
+        except subprocess.CalledProcessError as e:
+            try:
+                # Try to destroy partially applied resources
+                self.destroy()
+            finally:
+                raise e from None
 
     def plan(self, output=""):
         output = output and "-out=%s" % output or ""
         self._run_cmd(self._get_cmd_args("plan", output=output))
 
     def init(self):
         self._run_cmd(self._get_cmd_args("init", plugin_dir=""))
@@ -99,22 +102,23 @@
         return [tf_bin] + list(
             filter(None, self.command_templates[cmd_name].format(**kw).split(" "))
         )
 
     def _run_cmd(self, args, output=False):
         env = dict(os.environ)
         tf_env = {}
-        if LazyPluginCacheDir.resolve():
+        if LazyPluginCacheDir.resolve(False):
             tf_env["TF_PLUGIN_CACHE_DIR"] = LazyPluginCacheDir.resolve()
         tf_env["TF_IN_AUTOMATION"] = "yes"
         if self.module_dir:
             tf_env["TF_DATA_DIR"] = self.work_dir
         cwd = self.module_dir or self.work_dir
         env.update(tf_env)
-        print("run cmd", args, tf_env, cwd, file=sys.stderr)
+
+        write_log("run cmd", args, tf_env, cwd)
         run_cmd = subprocess.check_call
         if output:
             run_cmd = subprocess.check_output
         return run_cmd(args, cwd=cwd, stderr=subprocess.STDOUT, env=env)
 
 
 class TerraformStateJson(UserString):
@@ -262,15 +266,16 @@
             return (data["resources"], data["outputs"])
 
         resources = {}
         outputs = {}
 
         for r in data.get("resources", ()):
             rmap = resources.setdefault(r["type"], {})
-            rmap[r["name"]] = dict(r["instances"][0]["attributes"])
+            if len(r["instances"]) > 0:
+                rmap[r["name"]] = dict(r["instances"][0]["attributes"])
 
         outputs = data.get("outputs", {})
         for m in data.get("modules", ()):
             for k, r in m.get("resources", {}).items():
                 if k.startswith("data"):
                     continue
                 module, rname = k.split(".", 1)
@@ -319,24 +324,32 @@
     """
 
     def __init__(self, name):
         self.name = name
         self.value = None
 
     def resolve(self, default=None):
-        if not self.value and default:
+        if self.value is None and default is None:
             raise ValueError("PlaceHolderValue %s not resolved" % self.name)
         return self.value or default
 
 
 LazyReplay = PlaceHolderValue("tf_replay")
 LazyModuleDir = PlaceHolderValue("module_dir")
 LazyPluginCacheDir = PlaceHolderValue("plugin_cache")
 LazyTfBin = PlaceHolderValue("tf_bin_path")
 PytestConfig = PlaceHolderValue("pytestconfig")
+LazyTFDebug = PlaceHolderValue("tf_debug")
+
+
+def write_log(msg, *parts):
+    if LazyTFDebug.resolve(False):
+        if parts:
+            msg = " ".join((msg, *(map(str, parts))))
+        print("%s\n" % msg, file=sys.stderr)
 
 
 class TerraformFixture(object):
     def __init__(
         self,
         tf_bin,
         plugin_cache,
@@ -377,15 +390,15 @@
             return candidate
         raise ModuleNotFound(self.tf_root_module)
 
     def get_runner(self, module_dir, work_dir):
         return TerraformRunner(
             str(work_dir),
             module_dir=module_dir,
-            plugin_cache=LazyPluginCacheDir.resolve(),
+            plugin_cache=LazyPluginCacheDir.resolve(False),
             tf_bin=LazyTfBin.resolve(),
         )
 
     def __call__(self, request, tmpdir_factory, worker_id):
         module_dir = self.resolve_module_dir()
         if self.replay:
             replay_resources = os.path.join(module_dir, "tf_resources.json")
@@ -397,15 +410,15 @@
                 os.path.join(module_dir, "tf_resources.json")
             )
         work_dir = tmpdir_factory.mktemp(self.tf_root_module, numbered=True).join("work")
         self.runner = self.get_runner(module_dir, work_dir)
         return self.create(request, module_dir)
 
     def create(self, request, module_dir):
-        print("tf create %s" % self.tf_root_module, file=sys.stderr)
+        write_log("tf create %s" % self.tf_root_module)
         self.runner.init()
         if self.teardown_config != td.OFF:
             request.addfinalizer(self.tear_down)
         try:
             state = self.runner.apply()
             state_json = state.export()
             test_api = TerraformTestApi.from_string(state_json, self.runner)
@@ -417,15 +430,15 @@
 
             return test_api
         except Exception:
             raise
 
     def tear_down(self):
         # config behavor on runner
-        print("tf teardown %s" % self.tf_root_module, file=sys.stderr)
+        write_log("tf teardown %s" % self.tf_root_module)
         try:
             self.runner.destroy()
         except subprocess.CalledProcessError as e:
             if self.teardown_config == td.IGNORE:
                 return
             raise TerraformCommandFailed from e
```

### Comparing `pytest-terraform-0.6.4/pytest_terraform/xdist.py` & `pytest_terraform-0.6.6/pytest_terraform/xdist.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
-import sys
 
 from pytest_terraform import tf
 from pytest_terraform.lock import lock_create, lock_delete
 
 
 class ScopedTerraformFixture(tf.TerraformFixture):
     # specialized terraform fixture for use with
@@ -30,17 +29,16 @@
 
     def create(self, request, module_dir):
         if self.replay:
             super().create(request, module_dir)
 
         with lock_create(self.state_dir / self.name) as (success, result):
             if success:
-                print(
-                    "%s create %s - success: %s" % (self.wid, self.name, success),
-                    file=sys.stderr,
+                tf.write_log(
+                    "%s create %s - success: %s" % (self.wid, self.name, success)
                 )
                 tf_test_api = super(ScopedTerraformFixture, self).create(
                     request, module_dir
                 )
                 result.write(self.runner.work_dir.encode("utf8"))
                 return tf_test_api
             return tf.TerraformTestApi.load(
@@ -51,25 +49,21 @@
         # print('%s %s fix teardown' % (self.wid, self.name), file=sys.stderr)
         with lock_delete(self.state_dir / self.name) as success:
             #  print('%s %s teardown state:%s' % (
             #        self.wid, self.name, success), file=sys.stderr)
             if not success:
                 return
             work_dir = (self.state_dir / self.name).read_text("utf8")
-            print(
-                "%s teardown %s work-dir %s" % (self.wid, self.name, success),
-                file=sys.stderr,
-            )
+            tf.write_log("%s teardown %s work-dir %s" % (self.wid, self.name, success))
             super(ScopedTerraformFixture)
             runner = self.get_runner(self.resolve_module_dir(), work_dir)
             runner.destroy()
 
 
 class XDistTerraform(object):
-
     # Hooks
     # https://github.com/pytest-dev/pytest-xdist/blob/master/src/xdist/newhooks.py
 
     def __init__(self, config):
         self.config = config
         self.state_dir = None
         self.wid = None
@@ -109,25 +103,25 @@
         for i in items:
             for f in i.fixturenames:
                 if f in self.tracked_fixtures:
                     fixture_map.setdefault(f, set()).add(i.nodeid)
         return fixture_map
 
     # worker hooks
-    def pytest_collection_modifyitems(self, session, config, items):
+    def pytest_collection_finish(self, session):
         """write out the collections of fixtures -> test ids
 
         in xdist this is only called from the workers
         """
         self.tracked_fixtures = {
             t.name
             for t in tf.terraform.get_fixtures()
             if isinstance(t, ScopedTerraformFixture)
         }
-        self.fixture_map = self.generate_fixture_map(items)
+        self.fixture_map = self.generate_fixture_map(session.items)
 
     def pytest_runtest_teardown(self, item, nextitem):
         found = []
         for f in item.fixturenames:
             if f in self.tracked_fixtures:
                 found.append(f)
         if not found:
@@ -144,17 +138,16 @@
         for f in found:
             # print("%s check %s result %s" % (
             #       self.wid, f, self.completed.issuperset(self.fixture_map[f])),
             #       file=sys.stderr)
             # print('%s check result %s %s:%s' % (
             #       self.wid, completed, f, self.fixture_map[f]))
             if self.completed.issuperset(self.fixture_map[f]):
-                print(
+                tf.write_log(
                     "%s execute test:%s teardown %s" % (self.wid, item.nodeid, f),
-                    file=sys.stderr,
                 )
                 tf.terraform.get_fixture(f).tear_down()
                 self.fixture_map.pop(f)
 
     def pytest_sessionfinish(self, exitstatus):
         if self.wid == "master":
             # print("master session finish", file=sys.stderr)
@@ -169,22 +162,20 @@
         #            self.wid, self.fixture_map), file=sys.stderr)
 
         remains = []
         for f in self.tracked_fixtures:
             if f not in self.fixture_map:
                 continue
             if self.completed.issuperset(self.fixture_map[f]):
-                print(
-                    "%s worker session down cleanup %s" % (self.wid, f), file=sys.stderr
-                )
+                tf.write_log("%s worker session down cleanup %s" % (self.wid, f))
                 tf.terraform.get_fixture(f).tear_down()
             else:
                 remains.append(str((f, self.fixture_map[f].difference(self.completed))))
         if remains:
-            print("%s tf remains %s" % (self.wid, remains), file=sys.stderr)
+            tf.write_log("%s tf remains %s" % (self.wid, remains))
 
     # master hooks
     def pytest_report_teststatus(self, report, config):
         # only called from master
         if self.wid != "master" or report.when != "call":
             return
         self.test_log_writer.write(("%s\n" % report.nodeid).encode("utf8"))
```

### Comparing `pytest-terraform-0.6.4/setup.py` & `pytest_terraform-0.6.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,257 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pytest-terraform
+Version: 0.6.6
+Summary: A pytest plugin for using terraform fixtures
+Home-page: https://github.com/cloud-custodian/pytest-terraform
+License: Apache-2.0
+Author: Kapil Thangavelu
+Author-email: kapilt@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: System :: Distributed Computing
+Classifier: Topic :: System :: Systems Administration
+Requires-Dist: jmespath (>=0.10.0)
+Requires-Dist: portalocker (>=1.7.0)
+Requires-Dist: pytest (>=6.0)
+Requires-Dist: pytest-xdist (>=1.31.0)
+Project-URL: Repository, https://github.com/cloud-custodian/pytest-terraform
+Description-Content-Type: text/markdown
 
-packages = \
-['pytest_terraform']
+# Introduction
 
-package_data = \
-{'': ['*']}
+[![CI](https://github.com/cloud-custodian/pytest-terraform/workflows/CI/badge.svg?branch=master&event=push)](https://github.com/cloud-custodian/pytest-terraform/actions?query=branch%3Amaster)
+[![codecov](https://codecov.io/gh/cloud-custodian/pytest-terraform/branch/master/graph/badge.svg)](https://codecov.io/gh/cloud-custodian/pytest-terraform)
 
-install_requires = \
-['jmespath>=0.10.0',
- 'portalocker>=1.7.0',
- 'pytest-xdist>=1.31.0',
- 'pytest>=6.0']
-
-entry_points = \
-{'pytest11': ['terraform = pytest_terraform.plugin']}
-
-setup_kwargs = {
-    'name': 'pytest-terraform',
-    'version': '0.6.4',
-    'description': 'A pytest plugin for using terraform fixtures',
-    'long_description': '# Introduction\n\n[![CI](https://github.com/cloud-custodian/pytest-terraform/workflows/CI/badge.svg?branch=master&event=push)](https://github.com/cloud-custodian/pytest-terraform/actions?query=branch%3Amaster)\n[![codecov](https://codecov.io/gh/cloud-custodian/pytest-terraform/branch/master/graph/badge.svg)](https://codecov.io/gh/cloud-custodian/pytest-terraform)\n\npytest_terraform is a pytest plugin that enables executing terraform\nto provision infrastructure in a unit/functional test as a fixture.\n\nThis plugin features uses a fixture factory pattern to enable paramterized\nconstruction of fixtures via decorators.\n\n## Usage\n\npytest_terraform provides a `terraform` decorator with the following parameters:\n\n| Argument             | Required? | Type    | Default      | Description |\n| -----                | :---:     | ---     | ---          | ---         |\n| `terraform_dir`      | yes       | String  |              | Terraform module (directory) to execute. |\n| `scope`              | no        | String  | `"function"` | [Pytest scope](https://docs.pytest.org/en/stable/fixture.html#scope-sharing-fixtures-across-classes-modules-packages-or-session) - should be one of: `function`, or `session`. Other scopes like  `class`, `module`, and `package` should work but have not been fully tested. |\n| `replay`             | no        | Boolean | `True`       | Use recorded resources instead of invoking terraform. See [Replay Support](#replay-support) for more details. |\n| `name`               | no        | String  | `None`       | Name used for the fixture. This defaults to the `terraform_dir` when `None` is supplied. |\n| `teardown`           | no        | String  | `"default"`  | Configure which teardown mode is used for terraform resources. See [Teardown Options](#teardown-options) for more details. |\n\n### Example\n\n```python\nfrom boto3 import Session\nfrom pytest_terraform import terraform\n\n\n# We use the terraform decorator to create a fixture with the name of\n# the terraform module.\n#\n# The test function will be invoked after the terraform module is provisioned\n# with the results of the provisioning.\n#\n# The module `aws_sqs` will be searched for in several directories, the test\n# file directory, a sub directory `terraform`.\n#\n# This fixture specifies a session scope and will be run once per test run.\n#\n@terraform(\'aws_sqs\', scope=\'session\')\ndef test_sqs(aws_sqs):\n    # A test is passed a terraform resources class containing content from\n    # the terraform state file.\n    #\n    # Note the state file contents may vary across terraform versions.\n    #\n    # We can access nested datastructures with a jmespath expression.\n    assert aws_sqs["aws_sqs_queue.test_queue.tags"] == {\n        "Environment": "production"\n    }\n   queue_url = aws_sqs[\'test_queue.queue_url\']\n   print(queue_url)\n\n\ndef test_sqs_deliver(aws_sqs):\n   # Once a fixture has been defined with a decorator\n   # it can be reused in the same module by name, with provisioning\n   # respecting scopes.\n   #\n   sqs = Session().client(\'sqs\')\n   sqs.send_message(\n       QueueUrl=aws_sqs[\'test_queue.queue_url\'],\n       MessageBody=b"123")\n\n\n@terraform(\'aws_sqs\')\ndef test_sqs_dlq(aws_sqs):\n   # the fixture can also referenced again via decorator, if redefined\n   # with decorator the fixture parameters much match (ie same session scope).\n\n   # Module outputs are available as a separate mapping.\n   aws_sqs.outputs[\'QueueUrl\']\n```\n\n*Note* the fixture name should match the terraform module name\n\n*Note* The terraform state file is considered an internal\nimplementation detail of terraform, not per se a stable public interface\nacross versions.\n\n## Marks\n\nAll tests using terraform fixtures have a `terraform` mark applied so\nthey can be run/selected via the command line ie.\n\n```shell\npytest -k terraform tests/\n```\n\nto run all terraform tests only. See pytest mark documentation for\nadditional details, https://docs.pytest.org/en/stable/example/markers.html#mark-examples\n\n\n## Options\n\nYou can provide the path to the terraform binary else its auto discovered\n```shell\n--tf-binary=$HOME/bin/terraform\n```\n\nTo avoid repeated downloading of plugins a plugin cache dir is utilized\nby default this is `.tfcache` in the current working directory.\n```shell\n--tf-plugin-dir=$HOME/.cache/tfcache\n```\n\nTerraform modules referenced by fixtures are looked up in a few different\nlocations, directly in the same directory as the test module, in a subdir\nnamed terraform, and in a sibling directory named terraform. An explicit\ndirectory can be given which will be looked at first for all modules.\n\n```shell\n--tf-mod-dir=terraform\n```\n\nThis plugin also supports flight recording (see next section)\n```shell\n--tf-replay=[record|replay|disable]\n```\n\n### Teardown Options\n\n`pytest_terraform` supports three different teardown modes for the terraform decorator.\nThe default, `pytest_terraform.teardown.ON` will always attempt to teardown any and all modules via `terraform destory`.\nIf for any reason destroy fails it will raise an exception to alert the test runner.\nThe next mode, `pytest_terraform.teardown.IGNORE`, will invoke `terraform destroy` as with `teardown.ON` but will ignore any failures.\nThis mode is particularly help if your test function performs destructive actions against any objects created by the terraform module.\nThe final option is `pytest_terraform.teardown.OFF` which will remove the teardown method register all together.\nThis should generally only be used in very specific situations and is considered an edge case.\n\nThere is a special `pytest_terraform.teardown.DEFAULT` which is what the `teardown` parameter actually defaults to.\n\nTeardown options are available, for convenience, on the terraform decorator.\nFor example, set teardown to ignore:\n\n```python\nfrom pytest_terraform import terraform\n\n\n@terraform(\'aws_sqs\', teardown=terraform.TEARDOWN_IGNORE)\ndef test_sqs(aws_sqs):\n    assert aws_sqs["aws_sqs_queue.test_queue.tags"] == {\n        "Environment": "production"\n    }\n   queue_url = aws_sqs[\'test_queue.queue_url\']\n   print(queue_url)\n```\n\n## Hooks\n\npytest_terraform provides hooks via the pytest hook implementation.\nHooks should be added in the `conftest.py` file.\n\n### `pytest_terraform_modify_state`\n\nThis hook is executed after state has been captured from terraform apply and before writing to disk.\nThis hook does not modify state that\'s passed to the function under test.\nThe state is passed as the kwarg `tfstate` which is a `TerraformStateJson` UserString class with the following methods and properties:\n\n- `TerraformStateJson.dict` - The deserialized state as a dict\n- `TerraformStateJson.update(state: str)` - Replace the serialized state with a new state string\n- `TerraformStateJson.update_dict(state: dict)` - Replace the serialized state from a dictionary\n\n#### Example\n\n```python\ndef pytest_terraform_modify_state(tfstate):\n    print(str(tfstate))\n```\n\n#### Example AWS Account scrub\n\n```python\nimport re\n\ndef pytest_terraform_modify_state(tfstate):\n    """ Replace potential AWS account numbers with \'REDACTED\' """\n    tfstate.update(re.sub(r\'([0-9]+){12}\', \'REDACTED\', str(tfstate)))\n```\n\n## Flight Recording\n\nThe usage/philosophy of this plugin is based on using flight recording\nfor unit tests against cloud infrastructure. In flight recording rather\nthan mocking or stubbing infrastructure, actual resources are created\nand interacted with with responses recorded, with those responses\nsubsequently replayed for fast test execution. Beyond the fidelity\noffered, this also enables these tests to be executed/re-recorded against\nlive infrastructure for additional functional/release testing.\n\nhttps://cloudcustodian.io/docs/developer/tests.html#creating-cloud-resources-with-terraform\n\n### Replay Support\n\nBy default fixtures will save a `tf_resources.json` back to the module\ndirectory, that will be used when in replay mode.\n\nReplay can be configured by passing --tf-replay on the cli or via pytest config file.\n\n### Recording\n\nPassing the fixture parameter `replay` can control the replay behavior on an individual\ntest. The default is to operate in recording mode.\n\n@terraform(\'file_example\', replay=False)\ndef test_file_example(file_example):\n    assert file_example[\'local_file.bar.content\'] == \'bar!\'\n\n\n## XDist Compatibility\n\npytest_terraform supports pytest-xdist in multi-process (not distributed)\nmode.\n\nWhen run with python-xdist, pytest_terraform treats all non functional\nscopes as per test run fixtures across all workers, honoring their\noriginal scope lifecycle but with global semantics, instead of once\nper worker (xdist default).\n\nTo enable this the plugin does multi-process coodination using lock\nfiles, a test execution log, and a dependency mapping of fixtures\nto tests. Any worker can execute a module teardown when its done executing\nthe last test that depends on a given fixture. All provisioning and\nteardown are guarded by atomic file locks in the pytest execution\'s temp\ndirectory.\n\n### Root module references\n\n`terraform_remote_state` can be used to introduce a dependency between\na scoped root modules on an individual test, note we are not\nattempting to support same scope inter fixture dependencies as that\nimposes additional scheduling constraints outside of pytest native\ncapabilities. The higher scoped root module (ie session or module scoped)\nwill need to have output variables to enable this consumption.\n',
-    'author': 'Kapil Thangavelu',
-    'author_email': 'kapilt@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/cloud-custodian/pytest-terraform',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.6,<4.0',
-}
+pytest_terraform is a pytest plugin that enables executing terraform
+to provision infrastructure in a unit/functional test as a fixture.
 
+This plugin features uses a fixture factory pattern to enable paramterized
+construction of fixtures via decorators.
+
+## Usage
+
+pytest_terraform provides a `terraform` decorator with the following parameters:
+
+| Argument             | Required? | Type    | Default      | Description |
+| -----                | :---:     | ---     | ---          | ---         |
+| `terraform_dir`      | yes       | String  |              | Terraform module (directory) to execute. |
+| `scope`              | no        | String  | `"function"` | [Pytest scope](https://docs.pytest.org/en/stable/fixture.html#scope-sharing-fixtures-across-classes-modules-packages-or-session) - should be one of: `function`, or `session`. Other scopes like  `class`, `module`, and `package` should work but have not been fully tested. |
+| `replay`             | no        | Boolean | `True`       | Use recorded resources instead of invoking terraform. See [Replay Support](#replay-support) for more details. |
+| `name`               | no        | String  | `None`       | Name used for the fixture. This defaults to the `terraform_dir` when `None` is supplied. |
+| `teardown`           | no        | String  | `"default"`  | Configure which teardown mode is used for terraform resources. See [Teardown Options](#teardown-options) for more details. |
+
+### Example
+
+```python
+from boto3 import Session
+from pytest_terraform import terraform
+
+
+# We use the terraform decorator to create a fixture with the name of
+# the terraform module.
+#
+# The test function will be invoked after the terraform module is provisioned
+# with the results of the provisioning.
+#
+# The module `aws_sqs` will be searched for in several directories, the test
+# file directory, a sub directory `terraform`.
+#
+# This fixture specifies a session scope and will be run once per test run.
+#
+@terraform('aws_sqs', scope='session')
+def test_sqs(aws_sqs):
+    # A test is passed a terraform resources class containing content from
+    # the terraform state file.
+    #
+    # Note the state file contents may vary across terraform versions.
+    #
+    # We can access nested datastructures with a jmespath expression.
+    assert aws_sqs["aws_sqs_queue.test_queue.tags"] == {
+        "Environment": "production"
+    }
+   queue_url = aws_sqs['test_queue.queue_url']
+   print(queue_url)
+
+
+def test_sqs_deliver(aws_sqs):
+   # Once a fixture has been defined with a decorator
+   # it can be reused in the same module by name, with provisioning
+   # respecting scopes.
+   #
+   sqs = Session().client('sqs')
+   sqs.send_message(
+       QueueUrl=aws_sqs['test_queue.queue_url'],
+       MessageBody=b"123")
+
+
+@terraform('aws_sqs')
+def test_sqs_dlq(aws_sqs):
+   # the fixture can also referenced again via decorator, if redefined
+   # with decorator the fixture parameters much match (ie same session scope).
+
+   # Module outputs are available as a separate mapping.
+   aws_sqs.outputs['QueueUrl']
+```
+
+*Note* the fixture name should match the terraform module name
+
+*Note* The terraform state file is considered an internal
+implementation detail of terraform, not per se a stable public interface
+across versions.
+
+## Marks
+
+All tests using terraform fixtures have a `terraform` mark applied so
+they can be run/selected via the command line ie.
+
+```shell
+pytest -k terraform tests/
+```
+
+to run all terraform tests only. See pytest mark documentation for
+additional details, https://docs.pytest.org/en/stable/example/markers.html#mark-examples
+
+
+## Options
+
+You can provide the path to the terraform binary else its auto discovered
+```shell
+--tf-binary=$HOME/bin/terraform
+```
+
+Terraform modules referenced by fixtures are looked up in a few different
+locations, directly in the same directory as the test module, in a subdir
+named terraform, and in a sibling directory named terraform. An explicit
+directory can be given which will be looked at first for all modules.
+
+```shell
+--tf-mod-dir=terraform
+```
+
+This plugin also supports flight recording (see next section)
+```shell
+--tf-replay=[record|replay|disable]
+```
+
+### Teardown Options
+
+`pytest_terraform` supports three different teardown modes for the terraform decorator.
+The default, `pytest_terraform.teardown.ON` will always attempt to teardown any and all modules via `terraform destory`.
+If for any reason destroy fails it will raise an exception to alert the test runner.
+The next mode, `pytest_terraform.teardown.IGNORE`, will invoke `terraform destroy` as with `teardown.ON` but will ignore any failures.
+This mode is particularly help if your test function performs destructive actions against any objects created by the terraform module.
+The final option is `pytest_terraform.teardown.OFF` which will remove the teardown method register all together.
+This should generally only be used in very specific situations and is considered an edge case.
+
+There is a special `pytest_terraform.teardown.DEFAULT` which is what the `teardown` parameter actually defaults to.
+
+Teardown options are available, for convenience, on the terraform decorator.
+For example, set teardown to ignore:
+
+```python
+from pytest_terraform import terraform
+
+
+@terraform('aws_sqs', teardown=terraform.TEARDOWN_IGNORE)
+def test_sqs(aws_sqs):
+    assert aws_sqs["aws_sqs_queue.test_queue.tags"] == {
+        "Environment": "production"
+    }
+   queue_url = aws_sqs['test_queue.queue_url']
+   print(queue_url)
+```
+
+## Hooks
+
+pytest_terraform provides hooks via the pytest hook implementation.
+Hooks should be added in the `conftest.py` file.
+
+### `pytest_terraform_modify_state`
+
+This hook is executed after state has been captured from terraform apply and before writing to disk.
+This hook does not modify state that's passed to the function under test.
+The state is passed as the kwarg `tfstate` which is a `TerraformStateJson` UserString class with the following methods and properties:
+
+- `TerraformStateJson.dict` - The deserialized state as a dict
+- `TerraformStateJson.update(state: str)` - Replace the serialized state with a new state string
+- `TerraformStateJson.update_dict(state: dict)` - Replace the serialized state from a dictionary
+
+#### Example
+
+```python
+def pytest_terraform_modify_state(tfstate):
+    print(str(tfstate))
+```
+
+#### Example AWS Account scrub
+
+```python
+import re
+
+def pytest_terraform_modify_state(tfstate):
+    """ Replace potential AWS account numbers with 'REDACTED' """
+    tfstate.update(re.sub(r'([0-9]+){12}', 'REDACTED', str(tfstate)))
+```
+
+## Flight Recording
+
+The usage/philosophy of this plugin is based on using flight recording
+for unit tests against cloud infrastructure. In flight recording rather
+than mocking or stubbing infrastructure, actual resources are created
+and interacted with with responses recorded, with those responses
+subsequently replayed for fast test execution. Beyond the fidelity
+offered, this also enables these tests to be executed/re-recorded against
+live infrastructure for additional functional/release testing.
+
+https://cloudcustodian.io/docs/developer/tests.html#creating-cloud-resources-with-terraform
+
+### Replay Support
+
+By default fixtures will save a `tf_resources.json` back to the module
+directory, that will be used when in replay mode.
+
+Replay can be configured by passing --tf-replay on the cli or via pytest config file.
+
+### Recording
+
+Passing the fixture parameter `replay` can control the replay behavior on an individual
+test. The default is to operate in recording mode.
+
+@terraform('file_example', replay=False)
+def test_file_example(file_example):
+    assert file_example['local_file.bar.content'] == 'bar!'
+
+
+## XDist Compatibility
+
+pytest_terraform supports pytest-xdist in multi-process (not distributed)
+mode.
+
+When run with python-xdist, pytest_terraform treats all non functional
+scopes as per test run fixtures across all workers, honoring their
+original scope lifecycle but with global semantics, instead of once
+per worker (xdist default).
+
+To enable this the plugin does multi-process coodination using lock
+files, a test execution log, and a dependency mapping of fixtures
+to tests. Any worker can execute a module teardown when its done executing
+the last test that depends on a given fixture. All provisioning and
+teardown are guarded by atomic file locks in the pytest execution's temp
+directory.
+
+### Root module references
+
+`terraform_remote_state` can be used to introduce a dependency between
+a scoped root modules on an individual test, note we are not
+attempting to support same scope inter fixture dependencies as that
+imposes additional scheduling constraints outside of pytest native
+capabilities. The higher scoped root module (ie session or module scoped)
+will need to have output variables to enable this consumption.
 
-setup(**setup_kwargs)
```

