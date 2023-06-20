# Comparing `tmp/devops-auto-tools-1.2.1.tar.gz` & `tmp/devops-auto-tools-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devops-auto-tools-1.2.1.tar", last modified: Tue Jun 20 10:11:38 2023, max compression
+gzip compressed data, was "devops-auto-tools-1.2.2.tar", last modified: Tue Jun 20 10:23:00 2023, max compression
```

## Comparing `devops-auto-tools-1.2.1.tar` & `devops-auto-tools-1.2.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 hthinh     (501) staff       (20)        0 2023-06-20 10:11:38.830373 devops-auto-tools-1.2.1/
--rw-r--r--   0 hthinh     (501) staff       (20)      397 2023-06-20 10:11:38.830029 devops-auto-tools-1.2.1/PKG-INFO
-drwxr-xr-x   0 hthinh     (501) staff       (20)        0 2023-06-20 10:11:38.819427 devops-auto-tools-1.2.1/devops_auto_tools.egg-info/
--rw-r--r--   0 hthinh     (501) staff       (20)      397 2023-06-20 10:11:38.000000 devops-auto-tools-1.2.1/devops_auto_tools.egg-info/PKG-INFO
--rw-r--r--   0 hthinh     (501) staff       (20)      525 2023-06-20 10:11:38.000000 devops-auto-tools-1.2.1/devops_auto_tools.egg-info/SOURCES.txt
--rw-r--r--   0 hthinh     (501) staff       (20)        1 2023-06-20 10:11:38.000000 devops-auto-tools-1.2.1/devops_auto_tools.egg-info/dependency_links.txt
--rw-r--r--   0 hthinh     (501) staff       (20)       89 2023-06-20 10:11:38.000000 devops-auto-tools-1.2.1/devops_auto_tools.egg-info/entry_points.txt
--rw-r--r--   0 hthinh     (501) staff       (20)       40 2023-06-20 10:11:38.000000 devops-auto-tools-1.2.1/devops_auto_tools.egg-info/requires.txt
--rw-r--r--   0 hthinh     (501) staff       (20)        6 2023-06-20 10:11:38.000000 devops-auto-tools-1.2.1/devops_auto_tools.egg-info/top_level.txt
--rw-r--r--   0 hthinh     (501) staff       (20)       38 2023-06-20 10:11:38.830484 devops-auto-tools-1.2.1/setup.cfg
--rw-rw-r--   0 hthinh     (501) staff       (20)      818 2023-06-20 10:11:19.000000 devops-auto-tools-1.2.1/setup.py
-drwxr-xr-x   0 hthinh     (501) staff       (20)        0 2023-06-20 10:11:38.820752 devops-auto-tools-1.2.1/tools/
--rw-rw-r--   0 hthinh     (501) staff       (20)       21 2022-12-14 07:50:30.000000 devops-auto-tools-1.2.1/tools/__init__.py
-drwxr-xr-x   0 hthinh     (501) staff       (20)        0 2023-06-20 10:11:38.824185 devops-auto-tools-1.2.1/tools/dtos/
--rw-rw-r--   0 hthinh     (501) staff       (20)        0 2022-06-28 06:04:52.000000 devops-auto-tools-1.2.1/tools/dtos/__init__.py
--rw-rw-r--   0 hthinh     (501) staff       (20)      128 2022-06-28 05:57:36.000000 devops-auto-tools-1.2.1/tools/dtos/aws_var.py
--rw-r--r--   0 hthinh     (501) staff       (20)      130 2023-06-20 09:05:33.000000 devops-auto-tools-1.2.1/tools/dtos/jump_var.py
--rw-r--r--   0 hthinh     (501) staff       (20)       80 2022-08-15 07:25:23.000000 devops-auto-tools-1.2.1/tools/dtos/ssh_var.py
--rw-r--r--   0 hthinh     (501) staff       (20)       50 2023-04-03 10:46:23.000000 devops-auto-tools-1.2.1/tools/dtos/utill_var.py
-drwxr-xr-x   0 hthinh     (501) staff       (20)        0 2023-06-20 10:11:38.829231 devops-auto-tools-1.2.1/tools/functions/
--rw-rw-r--   0 hthinh     (501) staff       (20)       29 2022-12-14 07:52:00.000000 devops-auto-tools-1.2.1/tools/functions/__init__.py
--rw-rw-r--   0 hthinh     (501) staff       (20)     2243 2023-04-03 10:44:55.000000 devops-auto-tools-1.2.1/tools/functions/aws.py
--rw-r--r--   0 hthinh     (501) staff       (20)     1157 2023-06-20 10:09:13.000000 devops-auto-tools-1.2.1/tools/functions/jump.py
--rw-r--r--   0 hthinh     (501) staff       (20)      589 2023-04-03 10:44:38.000000 devops-auto-tools-1.2.1/tools/functions/ssh.py
--rw-rw-r--   0 hthinh     (501) staff       (20)     1768 2023-06-20 09:48:45.000000 devops-auto-tools-1.2.1/tools/functions/utils.py
--rw-rw-r--   0 hthinh     (501) staff       (20)      528 2023-04-01 10:06:01.000000 devops-auto-tools-1.2.1/tools/main.py
+drwxr-xr-x   0 hthinh     (501) staff       (20)        0 2023-06-20 10:23:00.553623 devops-auto-tools-1.2.2/
+-rw-r--r--   0 hthinh     (501) staff       (20)      397 2023-06-20 10:23:00.553076 devops-auto-tools-1.2.2/PKG-INFO
+drwxr-xr-x   0 hthinh     (501) staff       (20)        0 2023-06-20 10:23:00.545027 devops-auto-tools-1.2.2/devops_auto_tools.egg-info/
+-rw-r--r--   0 hthinh     (501) staff       (20)      397 2023-06-20 10:23:00.000000 devops-auto-tools-1.2.2/devops_auto_tools.egg-info/PKG-INFO
+-rw-r--r--   0 hthinh     (501) staff       (20)      525 2023-06-20 10:23:00.000000 devops-auto-tools-1.2.2/devops_auto_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 hthinh     (501) staff       (20)        1 2023-06-20 10:23:00.000000 devops-auto-tools-1.2.2/devops_auto_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 hthinh     (501) staff       (20)       89 2023-06-20 10:23:00.000000 devops-auto-tools-1.2.2/devops_auto_tools.egg-info/entry_points.txt
+-rw-r--r--   0 hthinh     (501) staff       (20)       40 2023-06-20 10:23:00.000000 devops-auto-tools-1.2.2/devops_auto_tools.egg-info/requires.txt
+-rw-r--r--   0 hthinh     (501) staff       (20)        6 2023-06-20 10:23:00.000000 devops-auto-tools-1.2.2/devops_auto_tools.egg-info/top_level.txt
+-rw-r--r--   0 hthinh     (501) staff       (20)       38 2023-06-20 10:23:00.553810 devops-auto-tools-1.2.2/setup.cfg
+-rw-rw-r--   0 hthinh     (501) staff       (20)      818 2023-06-20 10:21:02.000000 devops-auto-tools-1.2.2/setup.py
+drwxr-xr-x   0 hthinh     (501) staff       (20)        0 2023-06-20 10:23:00.546220 devops-auto-tools-1.2.2/tools/
+-rw-rw-r--   0 hthinh     (501) staff       (20)       21 2022-12-14 07:50:30.000000 devops-auto-tools-1.2.2/tools/__init__.py
+drwxr-xr-x   0 hthinh     (501) staff       (20)        0 2023-06-20 10:23:00.549199 devops-auto-tools-1.2.2/tools/dtos/
+-rw-rw-r--   0 hthinh     (501) staff       (20)        0 2022-06-28 06:04:52.000000 devops-auto-tools-1.2.2/tools/dtos/__init__.py
+-rw-rw-r--   0 hthinh     (501) staff       (20)      128 2022-06-28 05:57:36.000000 devops-auto-tools-1.2.2/tools/dtos/aws_var.py
+-rw-r--r--   0 hthinh     (501) staff       (20)      130 2023-06-20 09:05:33.000000 devops-auto-tools-1.2.2/tools/dtos/jump_var.py
+-rw-r--r--   0 hthinh     (501) staff       (20)       80 2022-08-15 07:25:23.000000 devops-auto-tools-1.2.2/tools/dtos/ssh_var.py
+-rw-r--r--   0 hthinh     (501) staff       (20)       50 2023-04-03 10:46:23.000000 devops-auto-tools-1.2.2/tools/dtos/utill_var.py
+drwxr-xr-x   0 hthinh     (501) staff       (20)        0 2023-06-20 10:23:00.552297 devops-auto-tools-1.2.2/tools/functions/
+-rw-rw-r--   0 hthinh     (501) staff       (20)       29 2022-12-14 07:52:00.000000 devops-auto-tools-1.2.2/tools/functions/__init__.py
+-rw-rw-r--   0 hthinh     (501) staff       (20)     2243 2023-04-03 10:44:55.000000 devops-auto-tools-1.2.2/tools/functions/aws.py
+-rw-r--r--   0 hthinh     (501) staff       (20)     1189 2023-06-20 10:22:15.000000 devops-auto-tools-1.2.2/tools/functions/jump.py
+-rw-r--r--   0 hthinh     (501) staff       (20)      589 2023-04-03 10:44:38.000000 devops-auto-tools-1.2.2/tools/functions/ssh.py
+-rw-rw-r--   0 hthinh     (501) staff       (20)     1720 2023-06-20 10:20:35.000000 devops-auto-tools-1.2.2/tools/functions/utils.py
+-rw-rw-r--   0 hthinh     (501) staff       (20)      528 2023-04-01 10:06:01.000000 devops-auto-tools-1.2.2/tools/main.py
```

### Comparing `devops-auto-tools-1.2.1/devops_auto_tools.egg-info/SOURCES.txt` & `devops-auto-tools-1.2.2/devops_auto_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `devops-auto-tools-1.2.1/setup.py` & `devops-auto-tools-1.2.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='devops-auto-tools',
-    version='1.2.1',    
+    version='1.2.2',    
     description='A Python project for eks, ssh, jumpm-proxy manager',
     author='Baristi Trieu',
     author_email='ltqtrieu.0204@gmail.com',
     packages=find_packages(),
     license ='MIT',
     install_requires=[
         'simple_term_menu==1.4.1',
```

### Comparing `devops-auto-tools-1.2.1/tools/functions/aws.py` & `devops-auto-tools-1.2.2/tools/functions/aws.py`

 * *Files identical despite different names*

### Comparing `devops-auto-tools-1.2.1/tools/functions/jump.py` & `devops-auto-tools-1.2.2/tools/functions/ssh.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,26 @@
-from subprocess import call
+from subprocess import call, Popen, PIPE, run
 
 from tools.functions import utils
-from tools.dtos.jump_var import var
-from tools.dtos.utill_var import var as utils_var
+from tools.dtos.ssh_var import var
 
 def get_profiles():
   f = open(utils.get_config_path("~/.ssh/config"), 'r')
   lines = f.readlines()
   f.close()
   profiles = []
   for line in lines:
     if "Host " in line and "*" not in line:
       profiles.append(line.split("Host ")[1].split("\n")[0])
   return profiles
 
-def get_cidr():
-  return [
-    "All traffics",
-    "Specific cidrs"
-  ]
-
 def set_profile():
   var.profile = utils.render_choices(get_profiles())
   if var.profile != False:
     return True
   return False
 
-def set_cidr():
-  var.cidr = utils.render_choices(get_cidr())
-  if var.cidr != False:
-    if "All traffics (Not recommend)" in var.cidr:
-      var.cidr = "0.0.0.0/0"
-    else:
-      var.cidr = input("Enter cidr: ")
-    var.gateway_ip = input("Enter default gateway ipv4: ")
-    return True
-  return False
-  
-def set_proxy():
-  utils_var.allow_exist = False
-  utils.routing(var.gateway_ip, var.cidr)
-  call([ 
-    'sshuttle',
-    '-r', 
-    var.profile,
-    var.cidr, 
-    '-vv' 
+def set_ssh():
+  run([ 
+    'ssh', var.profile 
   ])
-  utils_var.allow_exist = True
   return False
```

### Comparing `devops-auto-tools-1.2.1/tools/functions/utils.py` & `devops-auto-tools-1.2.2/tools/functions/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import platform
 from simple_term_menu import TerminalMenu
 from subprocess import call
 from os.path import expanduser
 
-from tools.dtos.jump_var import var as jump_var
 from tools.dtos.utill_var import var as utils_var
 
 def render_choices(options:list):
   options.append("Back")
   terminal_menu = TerminalMenu(options)
   menu_entry_index = terminal_menu.show()
   result = options[menu_entry_index]
```

### Comparing `devops-auto-tools-1.2.1/tools/main.py` & `devops-auto-tools-1.2.2/tools/main.py`

 * *Files identical despite different names*

