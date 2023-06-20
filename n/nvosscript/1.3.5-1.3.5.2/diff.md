# Comparing `tmp/nvosscript-1.3.5.tar.gz` & `tmp/nvosscript-1.3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvosscript-1.3.5.tar", last modified: Tue Jun 13 09:22:57 2023, max compression
+gzip compressed data, was "nvosscript-1.3.5.2.tar", last modified: Tue Jun 20 02:28:19 2023, max compression
```

## Comparing `nvosscript-1.3.5.tar` & `nvosscript-1.3.5.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-06-13 09:22:57.305167 nvosscript-1.3.5/
--rw-r--r--   0 matador.wang   (503) staff       (20)     1073 2023-04-11 06:52:30.000000 nvosscript-1.3.5/LICENSE
--rw-r--r--   0 matador.wang   (503) staff       (20)      333 2023-06-13 09:22:57.305020 nvosscript-1.3.5/PKG-INFO
--rw-r--r--   0 matador.wang   (503) staff       (20)       78 2023-04-11 06:52:30.000000 nvosscript-1.3.5/README.md
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-06-13 09:22:57.299076 nvosscript-1.3.5/nvos/
--rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-04-11 06:52:30.000000 nvosscript-1.3.5/nvos/__init__.py
--rw-r--r--   0 matador.wang   (503) staff       (20)    13434 2023-06-13 09:20:36.000000 nvosscript-1.3.5/nvos/file.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     8487 2023-06-06 06:48:29.000000 nvosscript-1.3.5/nvos/remote.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     6143 2023-05-30 09:54:35.000000 nvosscript-1.3.5/nvos/run.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-06-13 09:22:57.299904 nvosscript-1.3.5/nvosscript.egg-info/
--rw-r--r--   0 matador.wang   (503) staff       (20)      333 2023-06-13 09:22:57.000000 nvosscript-1.3.5/nvosscript.egg-info/PKG-INFO
--rw-r--r--   0 matador.wang   (503) staff       (20)      759 2023-06-13 09:22:57.000000 nvosscript-1.3.5/nvosscript.egg-info/SOURCES.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)        1 2023-06-13 09:22:57.000000 nvosscript-1.3.5/nvosscript.egg-info/dependency_links.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)       41 2023-06-13 09:22:57.000000 nvosscript-1.3.5/nvosscript.egg-info/entry_points.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)       47 2023-06-13 09:22:57.000000 nvosscript-1.3.5/nvosscript.egg-info/requires.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)       27 2023-06-13 09:22:57.000000 nvosscript-1.3.5/nvosscript.egg-info/top_level.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)       38 2023-06-13 09:22:57.305217 nvosscript-1.3.5/setup.cfg
--rw-r--r--   0 matador.wang   (503) staff       (20)      805 2023-06-13 09:21:06.000000 nvosscript-1.3.5/setup.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-06-13 09:22:57.300559 nvosscript-1.3.5/skyeye/
--rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-05-04 01:42:28.000000 nvosscript-1.3.5/skyeye/__init__.py
--rw-r--r--   0 matador.wang   (503) staff       (20)      502 2023-05-30 09:54:35.000000 nvosscript-1.3.5/skyeye/handler.py
--rw-r--r--   0 matador.wang   (503) staff       (20)      778 2023-05-30 09:54:35.000000 nvosscript-1.3.5/skyeye/loghandler.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     2490 2023-05-30 09:54:35.000000 nvosscript-1.3.5/skyeye/remote.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-06-13 09:22:57.301272 nvosscript-1.3.5/start/
--rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-04-11 07:50:33.000000 nvosscript-1.3.5/start/__init__.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     1663 2023-05-30 09:54:35.000000 nvosscript-1.3.5/start/login.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     4500 2023-06-13 09:21:06.000000 nvosscript-1.3.5/start/main.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     1157 2023-05-30 09:54:35.000000 nvosscript-1.3.5/start/utils.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-06-13 09:22:57.297667 nvosscript-1.3.5/venv/
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-06-13 09:22:57.304455 nvosscript-1.3.5/venv/bin/
--rw-r--r--   0 matador.wang   (503) staff       (20)     1175 2023-05-09 08:53:30.000000 nvosscript-1.3.5/venv/bin/activate_this.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)     1735 2023-05-26 05:59:41.000000 nvosscript-1.3.5/venv/bin/jp.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      642 2023-05-26 05:59:42.000000 nvosscript-1.3.5/venv/bin/rst2html.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      764 2023-05-26 05:59:42.000000 nvosscript-1.3.5/venv/bin/rst2html4.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)     1099 2023-05-26 05:59:42.000000 nvosscript-1.3.5/venv/bin/rst2html5.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      841 2023-05-26 05:59:42.000000 nvosscript-1.3.5/venv/bin/rst2latex.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      664 2023-05-26 05:59:42.000000 nvosscript-1.3.5/venv/bin/rst2man.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      830 2023-05-26 05:59:42.000000 nvosscript-1.3.5/venv/bin/rst2odt.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      636 2023-05-26 05:59:42.000000 nvosscript-1.3.5/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      649 2023-05-26 05:59:42.000000 nvosscript-1.3.5/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      685 2023-05-26 05:59:42.000000 nvosscript-1.3.5/venv/bin/rst2s5.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      921 2023-05-26 05:59:42.000000 nvosscript-1.3.5/venv/bin/rst2xetex.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      650 2023-05-26 05:59:42.000000 nvosscript-1.3.5/venv/bin/rst2xml.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      718 2023-05-26 05:59:42.000000 nvosscript-1.3.5/venv/bin/rstpep2html.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-06-13 09:22:57.304701 nvosscript-1.3.5/win/
--rw-r--r--   0 matador.wang   (503) staff       (20)     1295 2023-05-11 08:47:40.000000 nvosscript-1.3.5/win/win_auto_script.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-06-20 02:28:19.647245 nvosscript-1.3.5.2/
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1073 2023-04-11 06:52:30.000000 nvosscript-1.3.5.2/LICENSE
+-rw-r--r--   0 matador.wang   (503) staff       (20)      335 2023-06-20 02:28:19.647092 nvosscript-1.3.5.2/PKG-INFO
+-rw-r--r--   0 matador.wang   (503) staff       (20)       78 2023-04-11 06:52:30.000000 nvosscript-1.3.5.2/README.md
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-06-20 02:28:19.640026 nvosscript-1.3.5.2/nvos/
+-rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-04-11 06:52:30.000000 nvosscript-1.3.5.2/nvos/__init__.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)    13884 2023-06-20 02:23:02.000000 nvosscript-1.3.5.2/nvos/file.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     8740 2023-06-20 02:24:29.000000 nvosscript-1.3.5.2/nvos/remote.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     6293 2023-06-20 02:23:27.000000 nvosscript-1.3.5.2/nvos/run.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-06-20 02:28:19.640952 nvosscript-1.3.5.2/nvosscript.egg-info/
+-rw-r--r--   0 matador.wang   (503) staff       (20)      335 2023-06-20 02:28:19.000000 nvosscript-1.3.5.2/nvosscript.egg-info/PKG-INFO
+-rw-r--r--   0 matador.wang   (503) staff       (20)      759 2023-06-20 02:28:19.000000 nvosscript-1.3.5.2/nvosscript.egg-info/SOURCES.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)        1 2023-06-20 02:28:19.000000 nvosscript-1.3.5.2/nvosscript.egg-info/dependency_links.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)       41 2023-06-20 02:28:19.000000 nvosscript-1.3.5.2/nvosscript.egg-info/entry_points.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)       47 2023-06-20 02:28:19.000000 nvosscript-1.3.5.2/nvosscript.egg-info/requires.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)       27 2023-06-20 02:28:19.000000 nvosscript-1.3.5.2/nvosscript.egg-info/top_level.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)       38 2023-06-20 02:28:19.647285 nvosscript-1.3.5.2/setup.cfg
+-rw-r--r--   0 matador.wang   (503) staff       (20)      808 2023-06-20 02:24:56.000000 nvosscript-1.3.5.2/setup.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-06-20 02:28:19.641826 nvosscript-1.3.5.2/skyeye/
+-rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-05-04 01:42:28.000000 nvosscript-1.3.5.2/skyeye/__init__.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)      502 2023-05-30 09:54:35.000000 nvosscript-1.3.5.2/skyeye/handler.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)      802 2023-06-19 10:04:39.000000 nvosscript-1.3.5.2/skyeye/loghandler.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     2531 2023-06-19 10:04:39.000000 nvosscript-1.3.5.2/skyeye/remote.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-06-20 02:28:19.642717 nvosscript-1.3.5.2/start/
+-rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-04-11 07:50:33.000000 nvosscript-1.3.5.2/start/__init__.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1663 2023-05-30 09:54:35.000000 nvosscript-1.3.5.2/start/login.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     4503 2023-06-20 02:24:56.000000 nvosscript-1.3.5.2/start/main.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1182 2023-06-20 02:18:44.000000 nvosscript-1.3.5.2/start/utils.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-06-20 02:28:19.638283 nvosscript-1.3.5.2/venv/
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-06-20 02:28:19.646383 nvosscript-1.3.5.2/venv/bin/
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1175 2023-05-09 08:53:30.000000 nvosscript-1.3.5.2/venv/bin/activate_this.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)     1735 2023-05-26 05:59:41.000000 nvosscript-1.3.5.2/venv/bin/jp.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      642 2023-05-26 05:59:42.000000 nvosscript-1.3.5.2/venv/bin/rst2html.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      764 2023-05-26 05:59:42.000000 nvosscript-1.3.5.2/venv/bin/rst2html4.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)     1099 2023-05-26 05:59:42.000000 nvosscript-1.3.5.2/venv/bin/rst2html5.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      841 2023-05-26 05:59:42.000000 nvosscript-1.3.5.2/venv/bin/rst2latex.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      664 2023-05-26 05:59:42.000000 nvosscript-1.3.5.2/venv/bin/rst2man.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      830 2023-05-26 05:59:42.000000 nvosscript-1.3.5.2/venv/bin/rst2odt.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      636 2023-05-26 05:59:42.000000 nvosscript-1.3.5.2/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      649 2023-05-26 05:59:42.000000 nvosscript-1.3.5.2/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      685 2023-05-26 05:59:42.000000 nvosscript-1.3.5.2/venv/bin/rst2s5.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      921 2023-05-26 05:59:42.000000 nvosscript-1.3.5.2/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      650 2023-05-26 05:59:42.000000 nvosscript-1.3.5.2/venv/bin/rst2xml.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      718 2023-05-26 05:59:42.000000 nvosscript-1.3.5.2/venv/bin/rstpep2html.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-06-20 02:28:19.646585 nvosscript-1.3.5.2/win/
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1295 2023-05-11 08:47:40.000000 nvosscript-1.3.5.2/win/win_auto_script.py
```

### Comparing `nvosscript-1.3.5/LICENSE` & `nvosscript-1.3.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.5/nvos/file.py` & `nvosscript-1.3.5.2/nvos/file.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,38 +9,38 @@
 
 
 # 初始化工作环境
 def init_work_space(workspace_path):
     if len(workspace_path) == 0:
         return False
     init_path = os.path.join(workspace_path, ".ndtc", "init")
-    with open(init_path, 'w') as f:
+    with open(init_path, 'w', encoding=utils.file_encoding) as f:
         f.write(workspace_path)
 
     nvos_dir = os.path.join(workspace_path, ".ndtc")
     project_space_list, success = sync_project_data(workspace_path)
     logger.info(f"sync_project_data end projectSpaceList: {project_space_list} success:{success} ")
     file_list = []
     find_json_config(workspace_path, file_list, project_space_list)
     # 将来可以优化上传文件信息，针对于已经上传过的就不在上传
-    with open(os.path.join(nvos_dir, "config"), 'w') as file:
+    with open(os.path.join(nvos_dir, "config"), 'w', encoding=utils.file_encoding) as file:
         for item in file_list:
             file.write(json.dumps(item) + "\n")
 
     remote.upload_file(workspace_path, file_list, project_space_list)
 
     workspace_env = []
     if os.path.exists(os.path.expanduser(os.path.join("~", '.ndtcrc', "workspace_env"))):
-        with open(os.path.expanduser(os.path.join("~", '.ndtcrc', "workspace_env")), 'r') as f:
+        with open(os.path.expanduser(os.path.join("~", '.ndtcrc', "workspace_env")), 'r', encoding=utils.file_encoding) as f:
             for line in f:
                 workspace_env.append(line.strip())
     workspace_env.append(workspace_path)
     workspace_env = list(set(workspace_env))
     utils.check_local_workspace()
-    with open(os.path.expanduser(os.path.join("~", '.ndtcrc', "workspace_env")), 'w') as f:
+    with open(os.path.expanduser(os.path.join("~", '.ndtcrc', "workspace_env")), 'w', encoding=utils.file_encoding) as f:
         for item in workspace_env:
             f.write(item + "\n")
 
     return True
 
 
 def pull_data_from_cloud(workspace_path):
@@ -51,15 +51,15 @@
 
 def push_data_to_cloud(workspace_path):
     logger.info(f"push_data_to_cloud start execute workspace_path: {workspace_path}")
     project_space_list, success = sync_project_data(workspace_path)
     nvos_path = os.path.join(workspace_path, ".ndtc")
 
     origin_file_list = []
-    with open(os.path.join(nvos_path, "config"), 'r') as f:
+    with open(os.path.join(nvos_path, "config"), 'r', encoding=utils.file_encoding) as f:
         for line in f:
             origin_file_list.append(json.loads(line))
     origin_file_map = {}
     for temp in origin_file_list:
         origin_file_map.update({"%s_%s" % (temp["file_path"], temp["git_branch"]): temp["file_size"]})
 
     file_list = []
@@ -69,37 +69,37 @@
         if "%s_%s" % (temp["file_path"], temp["git_branch"]) not in origin_file_map:
             add_file_list.append(temp)
     logger.info(f"push add_file_list: {add_file_list}")
     if len(add_file_list) > 0:
         remote.upload_file(workspace_path, add_file_list, project_space_list)
         logger.info(f"start save all file config ")
         origin_file_list.extend(add_file_list)
-        with open(os.path.join(nvos_path, "config"), 'w') as f:
+        with open(os.path.join(nvos_path, "config"), 'w', encoding=utils.file_encoding) as f:
             for item in origin_file_list:
                 f.write(json.dumps(item) + "\n")
 
 
 # 同步项目数据到远程
 def sync_project_data(workspace_path):
     logger.info(f"start execute sync_project_data {workspace_path}")
     project_space_path = os.path.join(workspace_path, ".ndtc", "project_space")
     origin_project_space_list = []
     if os.path.exists(project_space_path):
-        with open(project_space_path, 'r') as f:
+        with open(project_space_path, 'r', encoding=utils.file_encoding) as f:
             for line in f:
                 origin_project_space_list.append(json.loads(line.strip()))
     project_space_list = []
     find_project_space(workspace_path, project_space_list)
     project_space_list = filter_project_space(workspace_path, project_space_list)
     sync_project_offset(workspace_path, project_space_list)
     if len(project_space_list) != len(origin_project_space_list):
         logger.info(
             f"projectSpace changed projectSpaceList: {project_space_list}          originProjectSpaceList:{origin_project_space_list}")
         remote.save_workspace(workspace_path, project_space_list)
-        with open(project_space_path, 'w') as f:
+        with open(project_space_path, 'w', encoding=utils.file_encoding) as f:
             for item in project_space_list:
                 f.write(json.dumps(item) + "\n")
         return project_space_list, True
     logger.info("start compare projectSpace git branch  changed")
     upload_data = False
     for item in project_space_list:
         flag = False
@@ -108,41 +108,41 @@
                 "git_branch"]:
                 flag = True
         if not flag:
             remote.save_workspace(workspace_path, project_space_list)
             upload_data = True
             break
 
-    with open(project_space_path, 'w') as f:
+    with open(project_space_path, 'w', encoding=utils.file_encoding) as f:
         for item in project_space_list:
             f.write(json.dumps(item) + "\n")
     logger.info(f"end method sync_project_data project_space_list: {project_space_list}")
     return project_space_list, upload_data
 
 
 def sync_project_offset(workspace_path, project_space_list):
     offset_path = os.path.join(workspace_path, ".ndtc", "offset")
     if not os.path.exists(offset_path):
         for project_space in project_space_list:
             project_space["offset"] = 1
-        with open(offset_path, 'w') as f:
+        with open(offset_path, 'w', encoding=utils.file_encoding) as f:
             f.writelines(json.dumps(project_space_list))
     else:
-        with open(offset_path, 'r') as f:
+        with open(offset_path, 'r', encoding=utils.file_encoding) as f:
             offset_json_list = json.loads(f.readline())
         offer_map = {}
         filter_list = []
         for offset in offset_json_list:
             offer_map["%s_%s" % (offset["project_space"], offset["git_branch"])] = offset["offset"]
         for project_space in project_space_list:
             if not "%s_%s" % (project_space["project_space"], project_space["git_branch"]) in offer_map:
                 project_space["offset"] = 1
                 filter_list.append(project_space)
         offset_json_list.extend(filter_list)
-        with open(offset_path, 'w') as f:
+        with open(offset_path, 'w', encoding=utils.file_encoding) as f:
             f.writelines(json.dumps(offset_json_list))
 
 
 def filter_project_space(workspace_path, project_space_list):
     exit_git_data = []
     not_exit_git_data = []
     for project_space in project_space_list:
@@ -252,37 +252,37 @@
             result_list.append(result)
 
 
 def overwrite_file(workspace_path):
     logger.info(f"overwrite_file start overwrite file {workspace_path}")
     offset_file_path = os.path.join(workspace_path, ".ndtc", "offset")
 
-    with open(offset_file_path, 'r') as f:
+    with open(offset_file_path, 'r', encoding=utils.file_encoding) as f:
         offset_json_list = json.loads(f.readline())
     offer_map = {}
     for offset in offset_json_list:
         offer_map["%s_%s" % (offset["project_space"], offset["git_branch"])] = offset["offset"]
 
     project_space_path = os.path.join(workspace_path, ".ndtc", "project_space")
     project_space_list = []
-    with open(project_space_path, 'r') as f:
+    with open(project_space_path, 'r', encoding=utils.file_encoding) as f:
         for line in f:
             project_space_list.append(json.loads(line))
     logger.info(f"overwrite_file project_space_list: {project_space_list} offer_map:{offer_map}")
     for project_space in project_space_list:
         project_space["syncTag"] = offer_map.get(
             "%s_%s" % (project_space["project_space"], project_space["git_branch"]))
 
     response_list = remote.pull_workspace(workspace_path, project_space_list)
     for project_space in response_list["projectSpaceList"]:
         offer_map["%s_%s" % (project_space["fileDirectory"], project_space["gitBranch"])] = project_space["syncTag"]
         remote.download_file(project_space)
     for offset in offset_json_list:
         offset["offset"] = offer_map.get("%s_%s" % (offset["project_space"], offset["git_branch"]))
-    with open(offset_file_path, 'w') as f:
+    with open(offset_file_path, 'w', encoding=utils.file_encoding) as f:
         f.writelines(json.dumps(offset_json_list))
 
 
 def find_json_config(file_path, config_list, project_space_list):
     for file_name in os.listdir(file_path):
         if file_name == ".idea" or file_name == ".git" or file_name == ".repo" or file_name == ".ndtc" or file_name == ".DS_Store":
             continue
```

### Comparing `nvosscript-1.3.5/nvos/remote.py` & `nvosscript-1.3.5.2/nvos/remote.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import time
+import traceback
 
 import boto3
 import os
 import requests
 import hashlib
 import json
 import re
@@ -83,14 +84,16 @@
             flag = False
             for temp in filter_upload_re:
                 matchObj = re.match(temp, file_path["file_path"], re.M | re.I)
                 if matchObj:
                     flag = True
                     break
             if not flag:
+                f = file_path["file_path"]
+                logger.info(f"file :{f} ")
                 continue
 
             if project_space["project_space"] in file_path["file_path"]:
                 local_file_path = file_path["file_path"]
                 temp_file = {"local_file_path": local_file_path, "project_space": project_space["project_space"], "project_space_git_branch": project_space["git_branch"]}
                 upload_list.append(temp_file)
     upload_process(upload_list)
@@ -123,36 +126,37 @@
 
     get_current_env()
     url = "%s%s" % (daemon_network, "/file/upload")
 
     local_file_path = file["local_file_path"]
 
     try:
-        with open(local_file_path, 'r') as f:
+        with open(local_file_path, 'r', encoding=utils.file_encoding) as f:
             contents = f.read()
         post_param = {"projectSpaceGitBranch": file["project_space_git_branch"], "projectSpaceFileDirectory": file["project_space"], "userId": login.get_user_id(), "filePath": local_file_path, "fileContent": contents}
         post_data(url, post_param)
         logger.info(f"upload file local full path:{local_file_path}")
         global_var += 1
     except Exception:
+        traceback.print_exc()
         logger.exception('uploading_file error: %s', local_file_path)
 
 
 
 def download_file(project_space):
     get_current_env()
     url = "%s%s" % (daemon_network, "/file/download")
     for file in project_space["changedFileList"]:
         file_id = file["fileId"]
         file_full_path = file["fileFullPath"]
         try:
             post_param = {"id": file_id}
             data = post_data(url, post_param)
             file_content = data["fileContent"]
-            with open(file_full_path, "w") as f:
+            with open(file_full_path, "w", encoding=utils.file_encoding) as f:
                 f.write(file_content)
         except Exception:
             logger.info(f"this file sync fail  id:{file_id} ")
         else:
             logger.info(f"this file sync success  id:{file_id} ")
 
 def save_workspace(workspace_path, project_list):
@@ -211,24 +215,24 @@
 def switch_env(env):
     val = daemon_network_mapping.get(env)
     if len(val) == 0:
         return
     tip = daemon_network_front_mapping.get(env)
     result = {"cloud":val,"tip":tip,"env":env}
     utils.check_local_workspace()
-    with open(os.path.expanduser(os.path.join('~','.ndtcrc' ,'nvos_env')), 'w') as f:
+    with open(os.path.expanduser(os.path.join('~','.ndtcrc' ,'nvos_env')), 'w', encoding=utils.file_encoding) as f:
         f.writelines(json.dumps(result))
     print(f"this script current env:{env} and cloud linked:{tip}")
 
 
 def get_current_env():
     global daemon_network
     result = {}
     if os.path.exists(os.path.expanduser(os.path.join('~', '.ndtcrc', 'nvos_env'))):
-        with open(os.path.expanduser(os.path.join('~', '.ndtcrc', 'nvos_env')), 'r')as f:
+        with open(os.path.expanduser(os.path.join('~', '.ndtcrc', 'nvos_env')), 'r', encoding=utils.file_encoding)as f:
             result = json.loads(f.readline().strip())
             daemon_network = result["cloud"]
             tip = result["tip"]
             env = result["env"]
             logger.info(f"current env:{env} this cloud linked:{tip} daemon_network:{daemon_network}")
     if result == {}:
         result["cloud"] = daemon_network_mapping.get('prod')
```

### Comparing `nvosscript-1.3.5/nvos/run.py` & `nvosscript-1.3.5.2/nvos/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,25 +43,25 @@
     workspace_path, success = common_verify()
     if not success:
         return
 
     async_workspace = os.path.expanduser(os.path.join("~", '.ndtcrc', "aync_workspace"))
     all_workspace_list = []
     if os.path.exists(async_workspace):
-        with open(async_workspace, 'r') as f:
+        with open(async_workspace, 'r', encoding=utils.file_encoding) as f:
             for item in f:
                 all_workspace_list.append(item.strip())
 
     all_workspace_list = set(all_workspace_list)
     if model is None or model == "start".lower():
         all_workspace_list.add(workspace_path)
     elif model == "stop".lower():
         all_workspace_list.remove(workspace_path)
     utils.check_local_workspace()
-    with open(os.path.expanduser(os.path.join("~", '.ndtcrc', "aync_workspace")), "w") as f:
+    with open(os.path.expanduser(os.path.join("~", '.ndtcrc', "aync_workspace")), "w", encoding=utils.file_encoding) as f:
         for item in list(all_workspace_list):
             f.write(item + '\n')
 
     if platform.system() == 'Windows':
         return
     # 在运行时执行
 
@@ -87,27 +87,27 @@
             time.sleep(1)
 
 
 def execute_push(async_workspace):
     with concurrent.futures.ThreadPoolExecutor(max_workers=5) as executor:
         while True:
             all_push_workspace_list = []
-            with open(async_workspace, 'r') as f:
+            with open(async_workspace, 'r', encoding=utils.file_encoding) as f:
                 for item in f:
                     all_push_workspace_list.append(item.strip())
             for temp in all_push_workspace_list:
                 logger.info("command_async push current run workspace is " + temp)
                 executor.submit(file.push_data_to_cloud, temp)
             time.sleep(5)
 
 def execute_pull(async_workspace):
     with concurrent.futures.ThreadPoolExecutor(max_workers=5) as executor:
         while True:
             all_pull_workspace_list = []
-            with open(async_workspace, 'r') as f:
+            with open(async_workspace, 'r', encoding=utils.file_encoding) as f:
                 for item in f:
                     all_pull_workspace_list.append(item.strip())
             for temp in all_pull_workspace_list:
                 logger.info("command_async pull current run workspace is " + temp)
                 executor.submit(file.pull_data_from_cloud, temp)
             time.sleep(2)
 
@@ -153,15 +153,15 @@
         result = remote.get_current_env()
         print(f"current env:{result['env']} this cloud linked:{result['tip']}")
         return
 
     remote.switch_env(env)
     workspace_env = []
     if os.path.exists(os.path.expanduser(os.path.join("~", '.ndtcrc', "workspace_env"))):
-        with open(os.path.expanduser(os.path.join("~", '.ndtcrc', "workspace_env")), 'r') as f:
+        with open(os.path.expanduser(os.path.join("~", '.ndtcrc', "workspace_env")), 'r', encoding=utils.file_encoding) as f:
             for line in f:
                 workspace_env.append(line.strip())
         for item in workspace_env:
             try:
                 os.remove(os.path.join(item, ".ndtc", 'offset'))
                 os.remove(os.path.join(item, ".ndtc", 'project_space'))
                 os.remove(os.path.join(item, ".ndtc", 'config'))
```

### Comparing `nvosscript-1.3.5/nvosscript.egg-info/SOURCES.txt` & `nvosscript-1.3.5.2/nvosscript.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.5/setup.py` & `nvosscript-1.3.5.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name='nvosscript',
-    version='1.3.5',
+    version='1.3.5.02',
     description='nvos toolchain script',
     packages=find_namespace_packages(),
     author = 'andre.zhao',
     author_email = 'andre.zhao@nio.com',
     keywords='pack',
     readme = "README.md",
     install_requires=[
```

### Comparing `nvosscript-1.3.5/skyeye/loghandler.py` & `nvosscript-1.3.5.2/skyeye/loghandler.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,12 +18,12 @@
     with open(path, 'r') as f:
         for line in f:
             matchObj = re.search("\d\|\d+\|\d+\|.*", line, re.M | re.I)
             if matchObj:
                 logger_list.append(line)
 
     logger.info(f"filter logger info data is {logger_list}")
-    remote.upload_file(logger_list)
+    remote.upload_file(logger_list, os.path.basename(path))
```

### Comparing `nvosscript-1.3.5/skyeye/remote.py` & `nvosscript-1.3.5.2/skyeye/remote.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,37 +6,39 @@
 
 
 daemon_network = "https://nvos-toolchain.nioint.com"
 
 daemon_network_mapping = {
     "prod": "https://nvos-toolchain.nioint.com",
     "stg": "https://nvos-toolchain-stg.nioint.com",
-    "dev": "https://nvos-toolchain-dev.nioint.com",
+    "dev": "https://sky-eye-trace-dev.nioint.com",
     "local": "http://127.0.0.1:12800"
 }
 
 daemon_network_front_mapping = {
     "prod": "https://ndtc.nioint.com/#/nvosTool/spaceList",
     "stg": "https://ndtc-stg.nioint.com/#/nvosTool/spaceList",
     "dev": "https://soa-tools-dev.nioint.com/#/nvosTool/spaceList",
     "local": "http://127.0.0.1:12800"
 }
 
 # 导入全局日志记录器
 logger = logging.getLogger(__name__)
 
-def upload_file(data_list):
+def upload_file(data_list,file_name):
     get_current_env()
     url = daemon_network + "/v3/vehicleLogs"
     header = {
         "content-type": "application/x-www-form-urlencoded"
     }
+
     params = {
         "logDataList": data_list,
-        "username": login.get_user_id()
+        "username": login.get_user_id(),
+        "fileName": file_name
     }
     logger.info(f'request url:{url} params:{params}')
     r = requests.post(url, headers=header, data=params)
     logger.info(f"response status_code: {r.status_code} text: {r.text} ")
     if r.status_code == 200:
         result = r.text
         if result == "SUCCESS":
```

### Comparing `nvosscript-1.3.5/start/login.py` & `nvosscript-1.3.5.2/start/login.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.5/start/main.py` & `nvosscript-1.3.5.2/start/main.py`

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
-        print("1.3.5")
+        print("1.3.5.02")
     elif args.subcommand == 'env':
         switch_command_env(args.module, args.switch)
     elif args.subcommand == "upload":
         switch_command_upload(args.module, args.log)
     elif args.subcommand == "path":
         current_file_path = os.path.abspath(__file__)
         current_file_dir = os.path.dirname(current_file_path)
```

### Comparing `nvosscript-1.3.5/start/utils.py` & `nvosscript-1.3.5.2/start/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import os
 
 
+file_encoding = 'utf-8'
+
 def check_workspace_exist(current_path):
     if current_path == os.path.dirname(current_path):
         return "", False
     for file_name in os.listdir(current_path):
         if ".ndtc" == file_name:
             return current_path, True
     return check_workspace_exist(os.path.dirname(current_path))
```

### Comparing `nvosscript-1.3.5/venv/bin/activate_this.py` & `nvosscript-1.3.5.2/venv/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.5/venv/bin/jp.py` & `nvosscript-1.3.5.2/venv/bin/jp.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.5/venv/bin/rst2html.py` & `nvosscript-1.3.5.2/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.5/venv/bin/rst2html4.py` & `nvosscript-1.3.5.2/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.5/venv/bin/rst2html5.py` & `nvosscript-1.3.5.2/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.5/venv/bin/rst2latex.py` & `nvosscript-1.3.5.2/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.5/venv/bin/rst2man.py` & `nvosscript-1.3.5.2/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.5/venv/bin/rst2odt.py` & `nvosscript-1.3.5.2/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.5/venv/bin/rst2odt_prepstyles.py` & `nvosscript-1.3.5.2/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.5/venv/bin/rst2pseudoxml.py` & `nvosscript-1.3.5.2/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.5/venv/bin/rst2s5.py` & `nvosscript-1.3.5.2/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.5/venv/bin/rst2xetex.py` & `nvosscript-1.3.5.2/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.5/venv/bin/rst2xml.py` & `nvosscript-1.3.5.2/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.5/venv/bin/rstpep2html.py` & `nvosscript-1.3.5.2/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.3.5/win/win_auto_script.py` & `nvosscript-1.3.5.2/win/win_auto_script.py`

 * *Files identical despite different names*

