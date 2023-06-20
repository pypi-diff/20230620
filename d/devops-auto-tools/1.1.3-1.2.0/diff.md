# Comparing `tmp/devops-auto-tools-1.1.3.tar.gz` & `tmp/devops-auto-tools-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devops-auto-tools-1.1.3.tar", last modified: Mon Apr  3 11:18:51 2023, max compression
+gzip compressed data, was "devops-auto-tools-1.2.0.tar", last modified: Tue Jun 20 10:05:26 2023, max compression
```

## Comparing `devops-auto-tools-1.1.3.tar` & `devops-auto-tools-1.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 hthinh     (501) staff       (20)        0 2023-04-03 11:18:51.212110 devops-auto-tools-1.1.3/
--rw-r--r--   0 hthinh     (501) staff       (20)      397 2023-04-03 11:18:51.211591 devops-auto-tools-1.1.3/PKG-INFO
-drwxr-xr-x   0 hthinh     (501) staff       (20)        0 2023-04-03 11:18:51.205087 devops-auto-tools-1.1.3/devops_auto_tools.egg-info/
--rw-r--r--   0 hthinh     (501) staff       (20)      397 2023-04-03 11:18:51.000000 devops-auto-tools-1.1.3/devops_auto_tools.egg-info/PKG-INFO
--rw-r--r--   0 hthinh     (501) staff       (20)      525 2023-04-03 11:18:51.000000 devops-auto-tools-1.1.3/devops_auto_tools.egg-info/SOURCES.txt
--rw-r--r--   0 hthinh     (501) staff       (20)        1 2023-04-03 11:18:51.000000 devops-auto-tools-1.1.3/devops_auto_tools.egg-info/dependency_links.txt
--rw-r--r--   0 hthinh     (501) staff       (20)       89 2023-04-03 11:18:51.000000 devops-auto-tools-1.1.3/devops_auto_tools.egg-info/entry_points.txt
--rw-r--r--   0 hthinh     (501) staff       (20)       40 2023-04-03 11:18:51.000000 devops-auto-tools-1.1.3/devops_auto_tools.egg-info/requires.txt
--rw-r--r--   0 hthinh     (501) staff       (20)        6 2023-04-03 11:18:51.000000 devops-auto-tools-1.1.3/devops_auto_tools.egg-info/top_level.txt
--rw-r--r--   0 hthinh     (501) staff       (20)       38 2023-04-03 11:18:51.212268 devops-auto-tools-1.1.3/setup.cfg
--rw-rw-r--   0 hthinh     (501) staff       (20)      818 2023-04-03 11:18:30.000000 devops-auto-tools-1.1.3/setup.py
-drwxr-xr-x   0 hthinh     (501) staff       (20)        0 2023-04-03 11:18:51.206121 devops-auto-tools-1.1.3/tools/
--rw-rw-r--   0 hthinh     (501) staff       (20)       21 2022-12-14 07:50:30.000000 devops-auto-tools-1.1.3/tools/__init__.py
-drwxr-xr-x   0 hthinh     (501) staff       (20)        0 2023-04-03 11:18:51.208411 devops-auto-tools-1.1.3/tools/dtos/
--rw-rw-r--   0 hthinh     (501) staff       (20)        0 2022-06-28 06:04:52.000000 devops-auto-tools-1.1.3/tools/dtos/__init__.py
--rw-rw-r--   0 hthinh     (501) staff       (20)      128 2022-06-28 05:57:36.000000 devops-auto-tools-1.1.3/tools/dtos/aws_var.py
--rw-r--r--   0 hthinh     (501) staff       (20)      103 2023-04-01 09:52:48.000000 devops-auto-tools-1.1.3/tools/dtos/jump_var.py
--rw-r--r--   0 hthinh     (501) staff       (20)       80 2022-08-15 07:25:23.000000 devops-auto-tools-1.1.3/tools/dtos/ssh_var.py
--rw-r--r--   0 hthinh     (501) staff       (20)       50 2023-04-03 10:46:23.000000 devops-auto-tools-1.1.3/tools/dtos/utill_var.py
-drwxr-xr-x   0 hthinh     (501) staff       (20)        0 2023-04-03 11:18:51.211064 devops-auto-tools-1.1.3/tools/functions/
--rw-rw-r--   0 hthinh     (501) staff       (20)       29 2022-12-14 07:52:00.000000 devops-auto-tools-1.1.3/tools/functions/__init__.py
--rw-rw-r--   0 hthinh     (501) staff       (20)     2243 2023-04-03 10:44:55.000000 devops-auto-tools-1.1.3/tools/functions/aws.py
--rw-r--r--   0 hthinh     (501) staff       (20)     1040 2023-04-03 11:14:59.000000 devops-auto-tools-1.1.3/tools/functions/jump.py
--rw-r--r--   0 hthinh     (501) staff       (20)      589 2023-04-03 10:44:38.000000 devops-auto-tools-1.1.3/tools/functions/ssh.py
--rw-rw-r--   0 hthinh     (501) staff       (20)      988 2023-04-03 11:12:20.000000 devops-auto-tools-1.1.3/tools/functions/utils.py
--rw-rw-r--   0 hthinh     (501) staff       (20)      528 2023-04-01 10:06:01.000000 devops-auto-tools-1.1.3/tools/main.py
+drwxr-xr-x   0 hthinh     (501) staff       (20)        0 2023-06-20 10:05:26.741245 devops-auto-tools-1.2.0/
+-rw-r--r--   0 hthinh     (501) staff       (20)      397 2023-06-20 10:05:26.740699 devops-auto-tools-1.2.0/PKG-INFO
+drwxr-xr-x   0 hthinh     (501) staff       (20)        0 2023-06-20 10:05:26.733501 devops-auto-tools-1.2.0/devops_auto_tools.egg-info/
+-rw-r--r--   0 hthinh     (501) staff       (20)      397 2023-06-20 10:05:26.000000 devops-auto-tools-1.2.0/devops_auto_tools.egg-info/PKG-INFO
+-rw-r--r--   0 hthinh     (501) staff       (20)      525 2023-06-20 10:05:26.000000 devops-auto-tools-1.2.0/devops_auto_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 hthinh     (501) staff       (20)        1 2023-06-20 10:05:26.000000 devops-auto-tools-1.2.0/devops_auto_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 hthinh     (501) staff       (20)       89 2023-06-20 10:05:26.000000 devops-auto-tools-1.2.0/devops_auto_tools.egg-info/entry_points.txt
+-rw-r--r--   0 hthinh     (501) staff       (20)       40 2023-06-20 10:05:26.000000 devops-auto-tools-1.2.0/devops_auto_tools.egg-info/requires.txt
+-rw-r--r--   0 hthinh     (501) staff       (20)        6 2023-06-20 10:05:26.000000 devops-auto-tools-1.2.0/devops_auto_tools.egg-info/top_level.txt
+-rw-r--r--   0 hthinh     (501) staff       (20)       38 2023-06-20 10:05:26.741383 devops-auto-tools-1.2.0/setup.cfg
+-rw-rw-r--   0 hthinh     (501) staff       (20)      818 2023-06-20 10:05:13.000000 devops-auto-tools-1.2.0/setup.py
+drwxr-xr-x   0 hthinh     (501) staff       (20)        0 2023-06-20 10:05:26.734585 devops-auto-tools-1.2.0/tools/
+-rw-rw-r--   0 hthinh     (501) staff       (20)       21 2022-12-14 07:50:30.000000 devops-auto-tools-1.2.0/tools/__init__.py
+drwxr-xr-x   0 hthinh     (501) staff       (20)        0 2023-06-20 10:05:26.737151 devops-auto-tools-1.2.0/tools/dtos/
+-rw-rw-r--   0 hthinh     (501) staff       (20)        0 2022-06-28 06:04:52.000000 devops-auto-tools-1.2.0/tools/dtos/__init__.py
+-rw-rw-r--   0 hthinh     (501) staff       (20)      128 2022-06-28 05:57:36.000000 devops-auto-tools-1.2.0/tools/dtos/aws_var.py
+-rw-r--r--   0 hthinh     (501) staff       (20)      130 2023-06-20 09:05:33.000000 devops-auto-tools-1.2.0/tools/dtos/jump_var.py
+-rw-r--r--   0 hthinh     (501) staff       (20)       80 2022-08-15 07:25:23.000000 devops-auto-tools-1.2.0/tools/dtos/ssh_var.py
+-rw-r--r--   0 hthinh     (501) staff       (20)       50 2023-04-03 10:46:23.000000 devops-auto-tools-1.2.0/tools/dtos/utill_var.py
+drwxr-xr-x   0 hthinh     (501) staff       (20)        0 2023-06-20 10:05:26.739786 devops-auto-tools-1.2.0/tools/functions/
+-rw-rw-r--   0 hthinh     (501) staff       (20)       29 2022-12-14 07:52:00.000000 devops-auto-tools-1.2.0/tools/functions/__init__.py
+-rw-rw-r--   0 hthinh     (501) staff       (20)     2243 2023-04-03 10:44:55.000000 devops-auto-tools-1.2.0/tools/functions/aws.py
+-rw-r--r--   0 hthinh     (501) staff       (20)     1157 2023-06-20 09:58:33.000000 devops-auto-tools-1.2.0/tools/functions/jump.py
+-rw-r--r--   0 hthinh     (501) staff       (20)      589 2023-04-03 10:44:38.000000 devops-auto-tools-1.2.0/tools/functions/ssh.py
+-rw-rw-r--   0 hthinh     (501) staff       (20)     1768 2023-06-20 09:48:45.000000 devops-auto-tools-1.2.0/tools/functions/utils.py
+-rw-rw-r--   0 hthinh     (501) staff       (20)      528 2023-04-01 10:06:01.000000 devops-auto-tools-1.2.0/tools/main.py
```

### Comparing `devops-auto-tools-1.1.3/devops_auto_tools.egg-info/SOURCES.txt` & `devops-auto-tools-1.2.0/devops_auto_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `devops-auto-tools-1.1.3/setup.py` & `devops-auto-tools-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='devops-auto-tools',
-    version='1.1.3',    
+    version='1.2.0',    
     description='A Python project for eks, ssh, jumpm-proxy manager',
     author='Baristi Trieu',
     author_email='ltqtrieu.0204@gmail.com',
     packages=find_packages(),
     license ='MIT',
     install_requires=[
         'simple_term_menu==1.4.1',
```

### Comparing `devops-auto-tools-1.1.3/tools/functions/aws.py` & `devops-auto-tools-1.2.0/tools/functions/aws.py`

 * *Files identical despite different names*

### Comparing `devops-auto-tools-1.1.3/tools/functions/jump.py` & `devops-auto-tools-1.2.0/tools/functions/jump.py`

 * *Files 22% similar despite different names*

```diff
@@ -25,23 +25,25 @@
   if var.profile != False:
     return True
   return False
 
 def set_cidr():
   var.cidr = utils.render_choices(get_cidr())
   if var.cidr != False:
-    if "All traffics" in var.cidr:
+    if "All traffics (Not recommend)" in var.cidr:
       var.cidr = "0.0.0.0/0"
     else:
       var.cidr = input("Enter cidr: ")
+    var.gateway_ip = input("Enter default gateway ipv4: ")
     return True
   return False
   
 def set_proxy():
   utils_var.allow_exist = False
+  utils.routing(var.gateway_ip, var.cidr)
   call([ 
     'sshuttle',
     '-r', 
     var.profile,
     var.cidr, 
     '-vv' 
   ])
```

### Comparing `devops-auto-tools-1.1.3/tools/functions/ssh.py` & `devops-auto-tools-1.2.0/tools/functions/ssh.py`

 * *Files identical despite different names*

### Comparing `devops-auto-tools-1.1.3/tools/main.py` & `devops-auto-tools-1.2.0/tools/main.py`

 * *Files identical despite different names*

