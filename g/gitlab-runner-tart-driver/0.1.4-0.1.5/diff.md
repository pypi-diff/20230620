# Comparing `tmp/gitlab-runner-tart-driver-0.1.4.tar.gz` & `tmp/gitlab-runner-tart-driver-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab-runner-tart-driver-0.1.4.tar", last modified: Mon Apr 24 09:46:19 2023, max compression
+gzip compressed data, was "gitlab-runner-tart-driver-0.1.5.tar", last modified: Tue Jun 20 14:35:08 2023, max compression
```

## Comparing `gitlab-runner-tart-driver-0.1.4.tar` & `gitlab-runner-tart-driver-0.1.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 09:46:19.975574 gitlab-runner-tart-driver-0.1.4/
--rw-rw-rw-   0 root         (0) root         (0)     3303 2023-04-24 09:46:08.000000 gitlab-runner-tart-driver-0.1.4/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)       48 2023-04-24 09:46:08.000000 gitlab-runner-tart-driver-0.1.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    18383 2023-04-24 09:46:19.975574 gitlab-runner-tart-driver-0.1.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    17862 2023-04-24 09:46:08.000000 gitlab-runner-tart-driver-0.1.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 09:46:19.968573 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-24 09:46:08.000000 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-04-24 09:46:08.000000 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)      596 2023-04-24 09:46:08.000000 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 09:46:19.972574 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-24 09:46:08.000000 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      952 2023-04-24 09:46:08.000000 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/commands/cleanup.py
--rw-rw-rw-   0 root         (0) root         (0)      760 2023-04-24 09:46:08.000000 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/commands/config.py
--rw-rw-rw-   0 root         (0) root         (0)    10205 2023-04-24 09:46:08.000000 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/commands/prepare.py
--rw-rw-rw-   0 root         (0) root         (0)     2145 2023-04-24 09:46:08.000000 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/commands/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 09:46:19.974574 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/modules/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-24 09:46:08.000000 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/modules/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1061 2023-04-24 09:46:08.000000 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/modules/gitlab_custom_command_config.py
--rw-rw-rw-   0 root         (0) root         (0)      405 2023-04-24 09:46:08.000000 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/modules/gitlab_custom_driver_config.py
--rw-rw-rw-   0 root         (0) root         (0)     8703 2023-04-24 09:46:08.000000 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/modules/tart.py
--rw-rw-rw-   0 root         (0) root         (0)      923 2023-04-24 09:46:08.000000 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/modules/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 09:46:19.974574 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/scripts/
--rwxrwxrwx   0 root         (0) root         (0)     2533 2023-04-24 09:46:08.000000 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/scripts/install-gitlab-runner.sh.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 09:46:19.970574 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver.egg-info/
--rw-r--r--   0 root         (0) root         (0)    18383 2023-04-24 09:46:19.000000 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1060 2023-04-24 09:46:19.000000 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 09:46:19.000000 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       82 2023-04-24 09:46:19.000000 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 09:46:19.000000 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       47 2023-04-24 09:46:19.000000 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-04-24 09:46:19.000000 gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       31 2023-04-24 09:46:08.000000 gitlab-runner-tart-driver-0.1.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 09:46:19.975574 gitlab-runner-tart-driver-0.1.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1461 2023-04-24 09:46:08.000000 gitlab-runner-tart-driver-0.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 14:35:08.922506 gitlab-runner-tart-driver-0.1.5/
+-rw-rw-rw-   0 root         (0) root         (0)     3303 2023-06-20 14:35:01.000000 gitlab-runner-tart-driver-0.1.5/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       48 2023-06-20 14:35:01.000000 gitlab-runner-tart-driver-0.1.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    18383 2023-06-20 14:35:08.921506 gitlab-runner-tart-driver-0.1.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    17862 2023-06-20 14:35:01.000000 gitlab-runner-tart-driver-0.1.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 14:35:08.918506 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-20 14:35:01.000000 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-06-20 14:35:01.000000 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      596 2023-06-20 14:35:01.000000 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 14:35:08.920506 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 14:35:01.000000 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      952 2023-06-20 14:35:01.000000 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/commands/cleanup.py
+-rw-rw-rw-   0 root         (0) root         (0)      760 2023-06-20 14:35:01.000000 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/commands/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    10206 2023-06-20 14:35:01.000000 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/commands/prepare.py
+-rw-rw-rw-   0 root         (0) root         (0)     2145 2023-06-20 14:35:01.000000 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/commands/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 14:35:08.921506 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/modules/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 14:35:01.000000 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/modules/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1061 2023-06-20 14:35:01.000000 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/modules/gitlab_custom_command_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      405 2023-06-20 14:35:01.000000 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/modules/gitlab_custom_driver_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     8703 2023-06-20 14:35:01.000000 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/modules/tart.py
+-rw-rw-rw-   0 root         (0) root         (0)      923 2023-06-20 14:35:01.000000 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/modules/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 14:35:08.921506 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)     2533 2023-06-20 14:35:01.000000 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/scripts/install-gitlab-runner.sh.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 14:35:08.919506 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    18383 2023-06-20 14:35:08.000000 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1060 2023-06-20 14:35:08.000000 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 14:35:08.000000 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       82 2023-06-20 14:35:08.000000 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 14:35:08.000000 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       47 2023-06-20 14:35:08.000000 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-06-20 14:35:08.000000 gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-06-20 14:35:01.000000 gitlab-runner-tart-driver-0.1.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 14:35:08.922506 gitlab-runner-tart-driver-0.1.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2023-06-20 14:35:01.000000 gitlab-runner-tart-driver-0.1.5/setup.py
```

### Comparing `gitlab-runner-tart-driver-0.1.4/LICENSE.txt` & `gitlab-runner-tart-driver-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.4/PKG-INFO` & `gitlab-runner-tart-driver-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-runner-tart-driver
-Version: 0.1.4
+Version: 0.1.5
 Home-page: https://gitlab.com/schmieder.matthias/gitlab-runner-tart-driver
 Author: Matthias Schmieder
 Author-email: schmieder.matthias@gmail.com
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
```

### Comparing `gitlab-runner-tart-driver-0.1.4/README.md` & `gitlab-runner-tart-driver-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/cli.py` & `gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/cli.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/commands/cleanup.py` & `gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/commands/cleanup.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/commands/config.py` & `gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/commands/config.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/commands/prepare.py` & `gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/commands/prepare.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,15 +242,15 @@
 
     ssh_session = tart.ssh_session(name=p.vm_name(), username=p.tart_ssh_username, password=p.tart_ssh_password)
     ssh_session.exec_ssh_command(
         f"sudo mkdir -p {remote_script_dir} && sudo chown {p.tart_ssh_username}:{p.tart_ssh_username} {remote_script_dir}",
     )
 
     for volume in volume_mounts:
-        click.echo("[INFO] Setting up volume mount '{volume.name}'")
+        click.echo(f"[INFO] Setting up volume mount '{volume.name}'")
         ssh_session.exec_ssh_command(
             f"sudo mkdir -p $(dirname {volume.dest}); sudo ln -sf '/Volumes/My Shared Files/{volume.name}' {volume.dest}",
         )
 
     # if cache and builds volumes are not mounted, make sure to create them locally inside the VM
     if not cache_dir:
         ssh_session.exec_ssh_command(
```

### Comparing `gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/commands/run.py` & `gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/commands/run.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/modules/gitlab_custom_command_config.py` & `gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/modules/gitlab_custom_command_config.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/modules/tart.py` & `gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/modules/tart.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/modules/utils.py` & `gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/modules/utils.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver/scripts/install-gitlab-runner.sh.j2` & `gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver/scripts/install-gitlab-runner.sh.j2`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver.egg-info/PKG-INFO` & `gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-runner-tart-driver
-Version: 0.1.4
+Version: 0.1.5
 Home-page: https://gitlab.com/schmieder.matthias/gitlab-runner-tart-driver
 Author: Matthias Schmieder
 Author-email: schmieder.matthias@gmail.com
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
```

### Comparing `gitlab-runner-tart-driver-0.1.4/gitlab_runner_tart_driver.egg-info/SOURCES.txt` & `gitlab-runner-tart-driver-0.1.5/gitlab_runner_tart_driver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.4/setup.py` & `gitlab-runner-tart-driver-0.1.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 # read the long description from README.md
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
-version = "0.1.4"
+version = "0.1.5"
 
 version = f"{version}{os.environ.get('PIP_VERSION_POSTFIX','')}"
 
 # read the requirements from requirements.txt
 requirements = []
 with pathlib.Path("requirements.txt").open() as requirements_txt:
     requirements = [str(requirement) for requirement in pkg_resources.parse_requirements(requirements_txt)]
```

