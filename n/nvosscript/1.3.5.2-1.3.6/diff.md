# Comparing `tmp/nvosscript-1.3.5.2.tar.gz` & `tmp/nvosscript-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvosscript-1.3.5.2.tar", last modified: Tue Jun 20 02:28:19 2023, max compression
+gzip compressed data, was "nvosscript-1.3.6.tar", last modified: Tue Jun 20 08:45:16 2023, max compression
```

## Comparing `nvosscript-1.3.5.2.tar` & `nvosscript-1.3.6.tar`

### file list

```diff
@@ -1,46 +1,30 @@
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-06-20 02:28:19.647245 nvosscript-1.3.5.2/
--rw-r--r--   0 matador.wang   (503) staff       (20)     1073 2023-04-11 06:52:30.000000 nvosscript-1.3.5.2/LICENSE
--rw-r--r--   0 matador.wang   (503) staff       (20)      335 2023-06-20 02:28:19.647092 nvosscript-1.3.5.2/PKG-INFO
--rw-r--r--   0 matador.wang   (503) staff       (20)       78 2023-04-11 06:52:30.000000 nvosscript-1.3.5.2/README.md
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-06-20 02:28:19.640026 nvosscript-1.3.5.2/nvos/
--rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-04-11 06:52:30.000000 nvosscript-1.3.5.2/nvos/__init__.py
--rw-r--r--   0 matador.wang   (503) staff       (20)    13884 2023-06-20 02:23:02.000000 nvosscript-1.3.5.2/nvos/file.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     8740 2023-06-20 02:24:29.000000 nvosscript-1.3.5.2/nvos/remote.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     6293 2023-06-20 02:23:27.000000 nvosscript-1.3.5.2/nvos/run.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-06-20 02:28:19.640952 nvosscript-1.3.5.2/nvosscript.egg-info/
--rw-r--r--   0 matador.wang   (503) staff       (20)      335 2023-06-20 02:28:19.000000 nvosscript-1.3.5.2/nvosscript.egg-info/PKG-INFO
--rw-r--r--   0 matador.wang   (503) staff       (20)      759 2023-06-20 02:28:19.000000 nvosscript-1.3.5.2/nvosscript.egg-info/SOURCES.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)        1 2023-06-20 02:28:19.000000 nvosscript-1.3.5.2/nvosscript.egg-info/dependency_links.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)       41 2023-06-20 02:28:19.000000 nvosscript-1.3.5.2/nvosscript.egg-info/entry_points.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)       47 2023-06-20 02:28:19.000000 nvosscript-1.3.5.2/nvosscript.egg-info/requires.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)       27 2023-06-20 02:28:19.000000 nvosscript-1.3.5.2/nvosscript.egg-info/top_level.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)       38 2023-06-20 02:28:19.647285 nvosscript-1.3.5.2/setup.cfg
--rw-r--r--   0 matador.wang   (503) staff       (20)      808 2023-06-20 02:24:56.000000 nvosscript-1.3.5.2/setup.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-06-20 02:28:19.641826 nvosscript-1.3.5.2/skyeye/
--rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-05-04 01:42:28.000000 nvosscript-1.3.5.2/skyeye/__init__.py
--rw-r--r--   0 matador.wang   (503) staff       (20)      502 2023-05-30 09:54:35.000000 nvosscript-1.3.5.2/skyeye/handler.py
--rw-r--r--   0 matador.wang   (503) staff       (20)      802 2023-06-19 10:04:39.000000 nvosscript-1.3.5.2/skyeye/loghandler.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     2531 2023-06-19 10:04:39.000000 nvosscript-1.3.5.2/skyeye/remote.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-06-20 02:28:19.642717 nvosscript-1.3.5.2/start/
--rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-04-11 07:50:33.000000 nvosscript-1.3.5.2/start/__init__.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     1663 2023-05-30 09:54:35.000000 nvosscript-1.3.5.2/start/login.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     4503 2023-06-20 02:24:56.000000 nvosscript-1.3.5.2/start/main.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     1182 2023-06-20 02:18:44.000000 nvosscript-1.3.5.2/start/utils.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-06-20 02:28:19.638283 nvosscript-1.3.5.2/venv/
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-06-20 02:28:19.646383 nvosscript-1.3.5.2/venv/bin/
--rw-r--r--   0 matador.wang   (503) staff       (20)     1175 2023-05-09 08:53:30.000000 nvosscript-1.3.5.2/venv/bin/activate_this.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)     1735 2023-05-26 05:59:41.000000 nvosscript-1.3.5.2/venv/bin/jp.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      642 2023-05-26 05:59:42.000000 nvosscript-1.3.5.2/venv/bin/rst2html.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      764 2023-05-26 05:59:42.000000 nvosscript-1.3.5.2/venv/bin/rst2html4.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)     1099 2023-05-26 05:59:42.000000 nvosscript-1.3.5.2/venv/bin/rst2html5.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      841 2023-05-26 05:59:42.000000 nvosscript-1.3.5.2/venv/bin/rst2latex.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      664 2023-05-26 05:59:42.000000 nvosscript-1.3.5.2/venv/bin/rst2man.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      830 2023-05-26 05:59:42.000000 nvosscript-1.3.5.2/venv/bin/rst2odt.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      636 2023-05-26 05:59:42.000000 nvosscript-1.3.5.2/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      649 2023-05-26 05:59:42.000000 nvosscript-1.3.5.2/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      685 2023-05-26 05:59:42.000000 nvosscript-1.3.5.2/venv/bin/rst2s5.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      921 2023-05-26 05:59:42.000000 nvosscript-1.3.5.2/venv/bin/rst2xetex.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      650 2023-05-26 05:59:42.000000 nvosscript-1.3.5.2/venv/bin/rst2xml.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      718 2023-05-26 05:59:42.000000 nvosscript-1.3.5.2/venv/bin/rstpep2html.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-06-20 02:28:19.646585 nvosscript-1.3.5.2/win/
--rw-r--r--   0 matador.wang   (503) staff       (20)     1295 2023-05-11 08:47:40.000000 nvosscript-1.3.5.2/win/win_auto_script.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-06-20 08:45:16.191358 nvosscript-1.3.6/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1073 2023-03-22 09:01:10.000000 nvosscript-1.3.6/LICENSE
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-06-20 08:45:16.191199 nvosscript-1.3.6/PKG-INFO
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       78 2023-03-22 09:07:29.000000 nvosscript-1.3.6/README.md
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-06-20 08:45:16.187465 nvosscript-1.3.6/nvos/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-03-21 08:49:46.000000 nvosscript-1.3.6/nvos/__init__.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)    13886 2023-06-20 08:38:00.000000 nvosscript-1.3.6/nvos/file.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     8796 2023-06-20 08:44:42.000000 nvosscript-1.3.6/nvos/remote.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     6293 2023-06-20 07:09:18.000000 nvosscript-1.3.6/nvos/run.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-06-20 08:45:16.188342 nvosscript-1.3.6/nvosscript.egg-info/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-06-20 08:45:16.000000 nvosscript-1.3.6/nvosscript.egg-info/PKG-INFO
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      449 2023-06-20 08:45:16.000000 nvosscript-1.3.6/nvosscript.egg-info/SOURCES.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        1 2023-06-20 08:45:16.000000 nvosscript-1.3.6/nvosscript.egg-info/dependency_links.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       41 2023-06-20 08:45:16.000000 nvosscript-1.3.6/nvosscript.egg-info/entry_points.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       47 2023-06-20 08:45:16.000000 nvosscript-1.3.6/nvosscript.egg-info/requires.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       28 2023-06-20 08:45:16.000000 nvosscript-1.3.6/nvosscript.egg-info/top_level.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       38 2023-06-20 08:45:16.191405 nvosscript-1.3.6/setup.cfg
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      805 2023-06-20 07:21:24.000000 nvosscript-1.3.6/setup.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-06-20 08:45:16.189437 nvosscript-1.3.6/skyeye/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-18 06:53:13.000000 nvosscript-1.3.6/skyeye/__init__.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      502 2023-05-29 07:46:09.000000 nvosscript-1.3.6/skyeye/handler.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      802 2023-05-31 08:56:53.000000 nvosscript-1.3.6/skyeye/loghandler.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     2531 2023-06-14 01:42:31.000000 nvosscript-1.3.6/skyeye/remote.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-06-20 08:45:16.190605 nvosscript-1.3.6/start/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-04 03:24:28.000000 nvosscript-1.3.6/start/__init__.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1663 2023-05-29 07:39:37.000000 nvosscript-1.3.6/start/login.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     4500 2023-06-20 07:21:24.000000 nvosscript-1.3.6/start/main.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1182 2023-06-20 07:09:18.000000 nvosscript-1.3.6/start/utils.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-06-20 08:45:16.190854 nvosscript-1.3.6/win/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1295 2023-05-10 02:46:01.000000 nvosscript-1.3.6/win/win_auto_script.py
```

### Comparing `nvosscript-1.3.5.2/LICENSE` & `nvosscript-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.5.2/nvos/file.py` & `nvosscript-1.3.6/nvos/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,18 +219,18 @@
         git_branch_data = ""
         for line in git_branch_val:
             if "*" in line:
                 git_branch_data = line.split("*")[1].strip()
         return git_branch_data
     except subprocess.CalledProcessError as e:
         error_message = e.stderr.strip()
-        print(f"Git命令执行出错：{error_message}")
+        logger.exception(f"Git命令执行出错：{error_message}")
         return "(no branch)"
-    except Exception as e:
-        print(f"Error: {os.path.join(os.getcwd(), '.ndtc')} : {e.strerror}")
+    except Exception:
+        logger.exception(f"Error: {os.path.join(os.getcwd(), '.ndtc')}")
         return "(no branch)"
 
 
 # 获取项目的空间
 def find_project_space(workspace_path, result_list):
     for file_path in os.listdir(workspace_path):
         if file_path == ".idea" or file_path == ".repo" or file_path == ".ndtc" or file_path == ".DS_Store":
```

### Comparing `nvosscript-1.3.5.2/nvos/remote.py` & `nvosscript-1.3.6/nvos/remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     aws_sk = s3_secret["sk"]
     aws_region = s3_secret["regionId"]
     s3 = boto3.resource('s3', region_name=aws_region, aws_access_key_id=aws_ak,
                         aws_secret_access_key=aws_sk)
     bucket = s3.Bucket(bucket_name)
     file_name = "/log/" + login.get_user_id() + "/ndtc.log"
     bucket.upload_file(file_path, file_name)
+    print("success upload file name " + file_name)
 
 def upload_linux_client_script():
     file_name = "/nvos-script/linux/nvosscript.zip"
     file_path = os.path.join(os.getcwd(), 'nvosscript.zip');
     upload_client_script(file_name, file_path)
 
 
@@ -151,15 +152,15 @@
         try:
             post_param = {"id": file_id}
             data = post_data(url, post_param)
             file_content = data["fileContent"]
             with open(file_full_path, "w", encoding=utils.file_encoding) as f:
                 f.write(file_content)
         except Exception:
-            logger.info(f"this file sync fail  id:{file_id} ")
+            logger.exception(f"this file sync fail  id:{file_id} ")
         else:
             logger.info(f"this file sync success  id:{file_id} ")
 
 def save_workspace(workspace_path, project_list):
     get_current_env()
     url = "%s%s" % (daemon_network, "/workspace/add")
     post_param = {"userId": login.get_user_id(), "fileDirectory": workspace_path, "projectSpaceList": project_list}
```

### Comparing `nvosscript-1.3.5.2/nvos/run.py` & `nvosscript-1.3.6/nvos/run.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.5.2/setup.py` & `nvosscript-1.3.6/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name='nvosscript',
-    version='1.3.5.02',
+    version='1.3.6',
     description='nvos toolchain script',
     packages=find_namespace_packages(),
     author = 'andre.zhao',
     author_email = 'andre.zhao@nio.com',
     keywords='pack',
     readme = "README.md",
     install_requires=[
```

### Comparing `nvosscript-1.3.5.2/skyeye/loghandler.py` & `nvosscript-1.3.6/skyeye/loghandler.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.5.2/skyeye/remote.py` & `nvosscript-1.3.6/skyeye/remote.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.5.2/start/login.py` & `nvosscript-1.3.6/start/login.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.5.2/start/main.py` & `nvosscript-1.3.6/start/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     elif args.subcommand == "async":
         run.command_async(args.model)
     elif args.subcommand == "pull":
         run.command_pull()
     elif args.subcommand == "push":
         run.command_push()
     elif args.subcommand == "version":
-        print("1.3.5.02")
+        print("1.3.6")
     elif args.subcommand == 'env':
         switch_command_env(args.module, args.switch)
     elif args.subcommand == "upload":
         switch_command_upload(args.module, args.log)
     elif args.subcommand == "path":
         current_file_path = os.path.abspath(__file__)
         current_file_dir = os.path.dirname(current_file_path)
```

### Comparing `nvosscript-1.3.5.2/start/utils.py` & `nvosscript-1.3.6/start/utils.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.5.2/win/win_auto_script.py` & `nvosscript-1.3.6/win/win_auto_script.py`

 * *Files identical despite different names*

