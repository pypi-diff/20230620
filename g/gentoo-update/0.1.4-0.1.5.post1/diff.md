# Comparing `tmp/gentoo-update-0.1.4.tar.gz` & `tmp/gentoo-update-0.1.5.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gentoo-update-0.1.4.tar", last modified: Tue Jun 13 21:28:34 2023, max compression
+gzip compressed data, was "gentoo-update-0.1.5.post1.tar", last modified: Tue Jun 20 20:04:02 2023, max compression
```

## Comparing `gentoo-update-0.1.4.tar` & `gentoo-update-0.1.5.post1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:28:34.620321 gentoo-update-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-13 21:28:20.000000 gentoo-update-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-13 21:28:20.000000 gentoo-update-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-13 21:28:34.620321 gentoo-update-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-13 21:28:20.000000 gentoo-update-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:28:34.620321 gentoo-update-0.1.4/gentoo_update/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-13 21:28:20.000000 gentoo-update-0.1.4/gentoo_update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-06-13 21:28:20.000000 gentoo-update-0.1.4/gentoo_update/gentoo_update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:28:34.620321 gentoo-update-0.1.4/gentoo_update/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4545 2023-06-13 21:28:20.000000 gentoo-update-0.1.4/gentoo_update/scripts/updater.sh
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-06-13 21:28:20.000000 gentoo-update-0.1.4/gentoo_update/shell_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:28:34.620321 gentoo-update-0.1.4/gentoo_update.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-13 21:28:34.000000 gentoo-update-0.1.4/gentoo_update.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-13 21:28:34.000000 gentoo-update-0.1.4/gentoo_update.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 21:28:34.000000 gentoo-update-0.1.4/gentoo_update.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-13 21:28:34.000000 gentoo-update-0.1.4/gentoo_update.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 21:28:34.000000 gentoo-update-0.1.4/gentoo_update.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-13 21:28:34.620321 gentoo-update-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-13 21:28:20.000000 gentoo-update-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:28:34.620321 gentoo-update-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-13 21:28:20.000000 gentoo-update-0.1.4/tests/test_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:04:02.826374 gentoo-update-0.1.5.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-20 20:03:46.000000 gentoo-update-0.1.5.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-20 20:03:46.000000 gentoo-update-0.1.5.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-06-20 20:04:02.826374 gentoo-update-0.1.5.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-20 20:03:46.000000 gentoo-update-0.1.5.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:04:02.822374 gentoo-update-0.1.5.post1/gentoo_update/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-20 20:03:46.000000 gentoo-update-0.1.5.post1/gentoo_update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-06-20 20:03:46.000000 gentoo-update-0.1.5.post1/gentoo_update/gentoo_update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:04:02.826374 gentoo-update-0.1.5.post1/gentoo_update/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4792 2023-06-20 20:03:46.000000 gentoo-update-0.1.5.post1/gentoo_update/scripts/updater.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-06-20 20:03:46.000000 gentoo-update-0.1.5.post1/gentoo_update/shell_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:04:02.826374 gentoo-update-0.1.5.post1/gentoo_update.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-06-20 20:04:02.000000 gentoo-update-0.1.5.post1/gentoo_update.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-20 20:04:02.000000 gentoo-update-0.1.5.post1/gentoo_update.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 20:04:02.000000 gentoo-update-0.1.5.post1/gentoo_update.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-20 20:04:02.000000 gentoo-update-0.1.5.post1/gentoo_update.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-20 20:04:02.000000 gentoo-update-0.1.5.post1/gentoo_update.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-20 20:04:02.826374 gentoo-update-0.1.5.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-20 20:03:46.000000 gentoo-update-0.1.5.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:04:02.826374 gentoo-update-0.1.5.post1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-20 20:03:46.000000 gentoo-update-0.1.5.post1/tests/test_updater.py
```

### Comparing `gentoo-update-0.1.4/LICENSE` & `gentoo-update-0.1.5.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `gentoo-update-0.1.4/PKG-INFO` & `gentoo-update-0.1.5.post1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gentoo-update
-Version: 0.1.4
+Version: 0.1.5.post1
 Summary: Gentoo Linux updater
 Home-page: https://github.com/Lab-Brat/gentoo_update
 Author: Lab-Brat
 Author-email: labbrat_social@pm.me
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
@@ -22,29 +22,27 @@
 This project 
 [originates](https://wiki.gentoo.org/wiki/Google_Summer_of_Code/2023/Ideas/Automated_Gentoo_system_updater) 
 from 2023 Google Summer of Code.
 
 
 #### Usage
 `gentoo-update` is in [GURU](https://wiki.gentoo.org/wiki/Project:GURU) 
-overlay, and can be installed using emerge:
+overlay, and can be installed using `emerge`:
 ```bash
 emerge --ask app-admin/gentoo_update
 ```
-Because the project is in early stage of development it's not considered stable 
-and is masked by `~amd64`. To unmask it run:
-```bash
-echo 'app-admin/gentoo_update ~amd64' >> /etc/portage/package.accept_keywords/gentoo_update
-```
 
 Alternatively, updater can be installed with pip:
 ```
 pip install gentoo_update --break-system-packages
 ```
 
+The updater creates a subdirectory in Portage's default `PORTAGE_LOGDIR` located at `/var/log/portage/gentoo-update`. 
+However, if this variable is set to a different value in `make.conf`, it will use the new location instead of the default.  
+
 Here are some usage examples:
 * Basic security update
 ```bash
 gentoo-update
 ```
 
 * Full system update with extra update parameters
```

### Comparing `gentoo-update-0.1.4/README.md` & `gentoo-update-0.1.5.post1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -7,29 +7,27 @@
 This project 
 [originates](https://wiki.gentoo.org/wiki/Google_Summer_of_Code/2023/Ideas/Automated_Gentoo_system_updater) 
 from 2023 Google Summer of Code.
 
 
 #### Usage
 `gentoo-update` is in [GURU](https://wiki.gentoo.org/wiki/Project:GURU) 
-overlay, and can be installed using emerge:
+overlay, and can be installed using `emerge`:
 ```bash
 emerge --ask app-admin/gentoo_update
 ```
-Because the project is in early stage of development it's not considered stable 
-and is masked by `~amd64`. To unmask it run:
-```bash
-echo 'app-admin/gentoo_update ~amd64' >> /etc/portage/package.accept_keywords/gentoo_update
-```
 
 Alternatively, updater can be installed with pip:
 ```
 pip install gentoo_update --break-system-packages
 ```
 
+The updater creates a subdirectory in Portage's default `PORTAGE_LOGDIR` located at `/var/log/portage/gentoo-update`. 
+However, if this variable is set to a different value in `make.conf`, it will use the new location instead of the default.  
+
 Here are some usage examples:
 * Basic security update
 ```bash
 gentoo-update
 ```
 
 * Full system update with extra update parameters
```

### Comparing `gentoo-update-0.1.4/gentoo_update/gentoo_update.py` & `gentoo-update-0.1.5.post1/gentoo_update/gentoo_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import os
 import argparse
 from .shell_runner import ShellRunner
+from typing import List
 
-__version__ = "0.1.4"
+__version__ = "0.1.5-1"
 current_path = os.path.dirname(os.path.realpath(__file__))
 
 
-def create_cli():
+def create_cli() -> argparse.Namespace:
     """
     Define CLI command flags using argparse.
 
     Returns:
         parser.parse_args: Argparse commands
     """
     formatter = argparse.RawTextHelpFormatter
@@ -93,15 +94,15 @@
         help="Print updater version.\n",
     )
 
     args = parser.parse_args()
     return args
 
 
-def add_prefixes(args_list):
+def add_prefixes(args_list: List[str]) -> List[str]:
     """
     Function to add prefixes to a list of arguments passed to
     --update-mode full.
 
     Parameters:
     args_list (List[str]): A list of arguments without prefixes,
         example: v quiet-build=y
@@ -117,15 +118,15 @@
             prefixed_args.append("-" + arg)
         else:
             prefixed_args.append("--" + arg)
 
     return prefixed_args
 
 
-def main():
+def main() -> None:
     args = create_cli()
     runner = ShellRunner(args.quiet)
 
     runner.run_shell_script(
         args.update_mode,
         " ".join(add_prefixes(args.args)) if args.args else "NOARGS",
         args.config_update_mode,
```

### Comparing `gentoo-update-0.1.4/gentoo_update/scripts/updater.sh` & `gentoo-update-0.1.5.post1/gentoo_update/scripts/updater.sh`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/bin/bash
 
-set -e
+set -euo pipefail
 
 # ---------------------- VARIABLES ----------------------- #
 UPDATE_MODE="${1}"
 UPDATE_FLAGS="${2}"
 if [[ "${UPDATE_FLAGS}" == "NOARGS" ]]; then
 	UPDATE_FLAGS=""
 fi
@@ -91,34 +91,44 @@
 # ----------------------- CLEAN_UP ----------------------- #
 function clean_up() {
 	clean="${CLEAN}"
 	if [[ "${clean}" == 'y' ]]; then
 		echo "Cleaning packages that are not part of the tree..."
 		emerge --depclean
 
-		echo "Checking reverse dependencies..."
-		revdep-rebuild
+		if command -v revdep-rebuild >/dev/null 2>&1; then
+			echo "Checking reverse dependencies..."
+			revdep-rebuild
+
+			echo "Clean source code..."
+			eclean --deep distfiles
+		else
+			echo "app-portage/gentoolkit is not installed"
+		fi
 
-		echo "Clean source code..."
-		eclean --deep distfiles
 	else
 		echo "Clean up is not enabled."
 	fi
 }
 
 # -------------------- CHECK_RESTART --------------------- #
 function check_restart() {
 	restart="${DAEMON_RESTART}"
-	echo "Checking is any service needs a restart"
-	if [[ "${restart}" == 'y' ]]; then
-		# automatically restart all services
-		needrestart -r a
+
+	if command -v needrestart >/dev/null 2>&1; then
+		echo "Checking is any service needs a restart"
+		if [[ "${restart}" == 'y' ]]; then
+			# automatically restart all services
+			needrestart -r a
+		else
+			# list services that require a restart
+			needrestart -r l
+		fi
 	else
-		# list services that require a restart
-		needrestart -r l
+		echo "app-admin/needrestart is not installed"
 	fi
 }
 
 # ---------------------- GET_ELOGS ----------------------- #
 function read_elogs() {
 	elog_dir="/var/log/portage/elog"
```

### Comparing `gentoo-update-0.1.4/gentoo_update.egg-info/PKG-INFO` & `gentoo-update-0.1.5.post1/gentoo_update.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gentoo-update
-Version: 0.1.4
+Version: 0.1.5.post1
 Summary: Gentoo Linux updater
 Home-page: https://github.com/Lab-Brat/gentoo_update
 Author: Lab-Brat
 Author-email: labbrat_social@pm.me
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
@@ -22,29 +22,27 @@
 This project 
 [originates](https://wiki.gentoo.org/wiki/Google_Summer_of_Code/2023/Ideas/Automated_Gentoo_system_updater) 
 from 2023 Google Summer of Code.
 
 
 #### Usage
 `gentoo-update` is in [GURU](https://wiki.gentoo.org/wiki/Project:GURU) 
-overlay, and can be installed using emerge:
+overlay, and can be installed using `emerge`:
 ```bash
 emerge --ask app-admin/gentoo_update
 ```
-Because the project is in early stage of development it's not considered stable 
-and is masked by `~amd64`. To unmask it run:
-```bash
-echo 'app-admin/gentoo_update ~amd64' >> /etc/portage/package.accept_keywords/gentoo_update
-```
 
 Alternatively, updater can be installed with pip:
 ```
 pip install gentoo_update --break-system-packages
 ```
 
+The updater creates a subdirectory in Portage's default `PORTAGE_LOGDIR` located at `/var/log/portage/gentoo-update`. 
+However, if this variable is set to a different value in `make.conf`, it will use the new location instead of the default.  
+
 Here are some usage examples:
 * Basic security update
 ```bash
 gentoo-update
 ```
 
 * Full system update with extra update parameters
```

### Comparing `gentoo-update-0.1.4/setup.cfg` & `gentoo-update-0.1.5.post1/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -10,17 +10,19 @@
 classifiers = 
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3.10
 	Operating System :: POSIX :: Linux
 
 [options]
 python_requires = >=3.10
-packages = gentoo_update
 include_package_data = True
 
+[tool.setuptools.packages]
+find = {}
+
 [options.entry_points]
 console_scripts = 
 	gentoo-update = gentoo_update.gentoo_update:main
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `gentoo-update-0.1.4/tests/test_updater.py` & `gentoo-update-0.1.5.post1/tests/test_updater.py`

 * *Files identical despite different names*

