# Comparing `tmp/mobio-cli-1.0.4.tar.gz` & `tmp/mobio-cli-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobio-cli-1.0.4.tar", last modified: Thu Feb 16 07:54:30 2023, max compression
+gzip compressed data, was "mobio-cli-1.0.5.tar", last modified: Tue Jun 20 04:57:42 2023, max compression
```

## Comparing `mobio-cli-1.0.4.tar` & `mobio-cli-1.0.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-02-16 07:54:30.000000 mobio-cli-1.0.4/
--rw-r--r--   0 ChungNT    (501) staff       (20)        0 2021-05-04 11:47:35.000000 mobio-cli-1.0.4/MANIFEST.in
--rw-r--r--   0 ChungNT    (501) staff       (20)     1023 2023-02-16 07:54:30.000000 mobio-cli-1.0.4/PKG-INFO
--rw-r--r--   0 ChungNT    (501) staff       (20)      639 2023-02-16 07:54:14.000000 mobio-cli-1.0.4/README.md
-drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-02-16 07:54:30.000000 mobio-cli-1.0.4/mobio_cli/
--rw-r--r--   0 ChungNT    (501) staff       (20)        0 2021-04-26 18:02:24.000000 mobio-cli-1.0.4/mobio_cli/__init__.py
--rw-r--r--   0 ChungNT    (501) staff       (20)     5324 2023-02-15 09:44:10.000000 mobio-cli-1.0.4/mobio_cli/__main__.py
-drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-02-16 07:54:30.000000 mobio-cli-1.0.4/mobio_cli/templates/
--rw-r--r--   0 ChungNT    (501) staff       (20)     1187 2023-02-14 06:38:19.000000 mobio-cli-1.0.4/mobio_cli/templates/Dockerfile
--rw-r--r--   0 ChungNT    (501) staff       (20)     1496 2023-02-14 06:39:12.000000 mobio-cli-1.0.4/mobio_cli/templates/Dockerfile-release
--rw-r--r--   0 ChungNT    (501) staff       (20)       55 2021-05-04 19:20:07.000000 mobio-cli-1.0.4/mobio_cli/templates/README.md
--rw-r--r--   0 ChungNT    (501) staff       (20)      265 2021-10-07 09:50:11.000000 mobio-cli-1.0.4/mobio_cli/templates/app_{#PROJECT_NAME_SNAKE_LOWERCASE#}_api.{pymobio}
-drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-02-16 07:54:30.000000 mobio-cli-1.0.4/mobio_cli/templates/configs/
--rw-r--r--   0 ChungNT    (501) staff       (20)     1167 2023-02-15 08:52:06.000000 mobio-cli-1.0.4/mobio_cli/templates/configs/__init__.{pymobio}
--rw-r--r--   0 ChungNT    (501) staff       (20)     4745 2023-02-13 09:22:10.000000 mobio-cli-1.0.4/mobio_cli/templates/k8s-Jenkinsfile
--rw-r--r--   0 ChungNT    (501) staff       (20)      388 2021-08-17 17:39:15.000000 mobio-cli-1.0.4/mobio_cli/templates/prepare_env.sh
--rw-r--r--   0 ChungNT    (501) staff       (20)       66 2023-02-16 07:29:07.000000 mobio-cli-1.0.4/mobio_cli/templates/requirements.txt
-drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-02-16 07:54:30.000000 mobio-cli-1.0.4/mobio_cli/templates/resources/
-drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-02-16 07:54:30.000000 mobio-cli-1.0.4/mobio_cli/templates/resources/configs/
--rw-r--r--   0 ChungNT    (501) staff       (20)      268 2021-04-13 11:49:20.000000 mobio-cli-1.0.4/mobio_cli/templates/resources/configs/{#PROJECT_NAME_SNAKE_LOWERCASE#}.conf
-drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-02-16 07:54:30.000000 mobio-cli-1.0.4/mobio_cli/templates/resources/lang/
--rw-r--r--   0 ChungNT    (501) staff       (20)     1008 2023-02-15 08:46:40.000000 mobio-cli-1.0.4/mobio_cli/templates/resources/lang/message_en.json
--rw-r--r--   0 ChungNT    (501) staff       (20)     1158 2023-02-15 08:46:46.000000 mobio-cli-1.0.4/mobio_cli/templates/resources/lang/message_vi.json
-drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-02-16 07:54:30.000000 mobio-cli-1.0.4/mobio_cli/templates/src/
--rw-r--r--   0 ChungNT    (501) staff       (20)        0 2021-03-12 07:01:14.000000 mobio-cli-1.0.4/mobio_cli/templates/src/__init__.{pymobio}
-drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-02-16 07:54:30.000000 mobio-cli-1.0.4/mobio_cli/templates/src/apis/
--rw-r--r--   0 ChungNT    (501) staff       (20)     3808 2023-02-15 09:11:58.000000 mobio-cli-1.0.4/mobio_cli/templates/src/apis/__init__.{pymobio}
-drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-02-16 07:54:30.000000 mobio-cli-1.0.4/mobio_cli/templates/src/apis/v1_0/
--rw-r--r--   0 ChungNT    (501) staff       (20)       43 2021-04-23 02:12:16.000000 mobio-cli-1.0.4/mobio_cli/templates/src/apis/v1_0/__init__.{pymobio}
--rw-r--r--   0 ChungNT    (501) staff       (20)      297 2021-07-22 04:38:08.000000 mobio-cli-1.0.4/mobio_cli/templates/src/apis/v1_0/blueprints_api.{pymobio}
-drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-02-16 07:54:30.000000 mobio-cli-1.0.4/mobio_cli/templates/src/common/
--rw-r--r--   0 ChungNT    (501) staff       (20)       47 2023-02-15 08:19:00.000000 mobio-cli-1.0.4/mobio_cli/templates/src/common/__init__.{pymobio}
-drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-02-16 07:54:30.000000 mobio-cli-1.0.4/mobio_cli/templates/src/controllers/
--rw-r--r--   0 ChungNT    (501) staff       (20)        0 2021-08-17 18:16:25.000000 mobio-cli-1.0.4/mobio_cli/templates/src/controllers/empty
--rw-r--r--   0 ChungNT    (501) staff       (20)      760 2021-07-18 18:03:26.000000 mobio-cli-1.0.4/mobio_cli/templates/startup.sh
--rw-r--r--   0 ChungNT    (501) staff       (20)      214 2021-10-11 09:16:05.000000 mobio-cli-1.0.4/mobio_cli/templates/test.env
-drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-02-16 07:54:30.000000 mobio-cli-1.0.4/mobio_cli/templates/yaml/
-drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-02-16 07:54:30.000000 mobio-cli-1.0.4/mobio_cli/templates/yaml/BASE/
--rw-r--r--   0 ChungNT    (501) staff       (20)     1836 2023-02-16 04:27:56.000000 mobio-cli-1.0.4/mobio_cli/templates/yaml/BASE/deploy_{#PROJECT_NAME_SNAKE_LOWERCASE#}_app_api.yaml
-drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-02-16 07:54:30.000000 mobio-cli-1.0.4/mobio_cli.egg-info/
--rw-r--r--   0 ChungNT    (501) staff       (20)     1023 2023-02-16 07:54:30.000000 mobio-cli-1.0.4/mobio_cli.egg-info/PKG-INFO
--rw-r--r--   0 ChungNT    (501) staff       (20)     1184 2023-02-16 07:54:30.000000 mobio-cli-1.0.4/mobio_cli.egg-info/SOURCES.txt
--rw-r--r--   0 ChungNT    (501) staff       (20)        1 2023-02-16 07:54:30.000000 mobio-cli-1.0.4/mobio_cli.egg-info/dependency_links.txt
--rw-r--r--   0 ChungNT    (501) staff       (20)       55 2023-02-16 07:54:30.000000 mobio-cli-1.0.4/mobio_cli.egg-info/entry_points.txt
--rw-r--r--   0 ChungNT    (501) staff       (20)       10 2023-02-16 07:54:30.000000 mobio-cli-1.0.4/mobio_cli.egg-info/top_level.txt
--rw-r--r--   0 ChungNT    (501) staff       (20)       38 2023-02-16 07:54:30.000000 mobio-cli-1.0.4/setup.cfg
--rw-r--r--   0 ChungNT    (501) staff       (20)     1211 2023-02-16 07:54:30.000000 mobio-cli-1.0.4/setup.py
+drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-06-20 04:57:42.000000 mobio-cli-1.0.5/
+-rw-r--r--   0 ChungNT    (501) staff       (20)        0 2021-05-04 11:47:35.000000 mobio-cli-1.0.5/MANIFEST.in
+-rw-r--r--   0 ChungNT    (501) staff       (20)     1127 2023-06-20 04:57:42.000000 mobio-cli-1.0.5/PKG-INFO
+-rw-r--r--   0 ChungNT    (501) staff       (20)      743 2023-06-20 04:56:25.000000 mobio-cli-1.0.5/README.md
+drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-06-20 04:57:42.000000 mobio-cli-1.0.5/mobio_cli/
+-rw-r--r--   0 ChungNT    (501) staff       (20)        0 2021-04-26 18:02:24.000000 mobio-cli-1.0.5/mobio_cli/__init__.py
+-rw-r--r--   0 ChungNT    (501) staff       (20)     5324 2023-02-15 09:44:10.000000 mobio-cli-1.0.5/mobio_cli/__main__.py
+drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-06-20 04:57:42.000000 mobio-cli-1.0.5/mobio_cli/templates/
+-rw-r--r--   0 ChungNT    (501) staff       (20)     1187 2023-02-14 06:38:19.000000 mobio-cli-1.0.5/mobio_cli/templates/Dockerfile
+-rw-r--r--   0 ChungNT    (501) staff       (20)     1496 2023-02-14 06:39:12.000000 mobio-cli-1.0.5/mobio_cli/templates/Dockerfile-release
+-rw-r--r--   0 ChungNT    (501) staff       (20)       55 2021-05-04 19:20:07.000000 mobio-cli-1.0.5/mobio_cli/templates/README.md
+-rw-r--r--   0 ChungNT    (501) staff       (20)      265 2021-10-07 09:50:11.000000 mobio-cli-1.0.5/mobio_cli/templates/app_{#PROJECT_NAME_SNAKE_LOWERCASE#}_api.{pymobio}
+drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-06-20 04:57:42.000000 mobio-cli-1.0.5/mobio_cli/templates/configs/
+-rw-r--r--   0 ChungNT    (501) staff       (20)     1167 2023-02-15 08:52:06.000000 mobio-cli-1.0.5/mobio_cli/templates/configs/__init__.{pymobio}
+-rw-r--r--   0 ChungNT    (501) staff       (20)     4745 2023-02-13 09:22:10.000000 mobio-cli-1.0.5/mobio_cli/templates/k8s-Jenkinsfile
+-rw-r--r--   0 ChungNT    (501) staff       (20)      388 2021-08-17 17:39:15.000000 mobio-cli-1.0.5/mobio_cli/templates/prepare_env.sh
+-rw-r--r--   0 ChungNT    (501) staff       (20)       66 2023-06-20 04:54:55.000000 mobio-cli-1.0.5/mobio_cli/templates/requirements.txt
+drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-06-20 04:57:42.000000 mobio-cli-1.0.5/mobio_cli/templates/resources/
+drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-06-20 04:57:42.000000 mobio-cli-1.0.5/mobio_cli/templates/resources/configs/
+-rw-r--r--   0 ChungNT    (501) staff       (20)      268 2021-04-13 11:49:20.000000 mobio-cli-1.0.5/mobio_cli/templates/resources/configs/{#PROJECT_NAME_SNAKE_LOWERCASE#}.conf
+drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-06-20 04:57:42.000000 mobio-cli-1.0.5/mobio_cli/templates/resources/lang/
+-rw-r--r--   0 ChungNT    (501) staff       (20)     1008 2023-02-15 08:46:40.000000 mobio-cli-1.0.5/mobio_cli/templates/resources/lang/message_en.json
+-rw-r--r--   0 ChungNT    (501) staff       (20)     1158 2023-02-15 08:46:46.000000 mobio-cli-1.0.5/mobio_cli/templates/resources/lang/message_vi.json
+drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-06-20 04:57:42.000000 mobio-cli-1.0.5/mobio_cli/templates/src/
+-rw-r--r--   0 ChungNT    (501) staff       (20)        0 2021-03-12 07:01:14.000000 mobio-cli-1.0.5/mobio_cli/templates/src/__init__.{pymobio}
+drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-06-20 04:57:42.000000 mobio-cli-1.0.5/mobio_cli/templates/src/apis/
+-rw-r--r--   0 ChungNT    (501) staff       (20)     3808 2023-02-15 09:11:58.000000 mobio-cli-1.0.5/mobio_cli/templates/src/apis/__init__.{pymobio}
+drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-06-20 04:57:42.000000 mobio-cli-1.0.5/mobio_cli/templates/src/apis/v1_0/
+-rw-r--r--   0 ChungNT    (501) staff       (20)       43 2021-04-23 02:12:16.000000 mobio-cli-1.0.5/mobio_cli/templates/src/apis/v1_0/__init__.{pymobio}
+-rw-r--r--   0 ChungNT    (501) staff       (20)      297 2021-07-22 04:38:08.000000 mobio-cli-1.0.5/mobio_cli/templates/src/apis/v1_0/blueprints_api.{pymobio}
+drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-06-20 04:57:42.000000 mobio-cli-1.0.5/mobio_cli/templates/src/common/
+-rw-r--r--   0 ChungNT    (501) staff       (20)       47 2023-02-15 08:19:00.000000 mobio-cli-1.0.5/mobio_cli/templates/src/common/__init__.{pymobio}
+drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-06-20 04:57:42.000000 mobio-cli-1.0.5/mobio_cli/templates/src/controllers/
+-rw-r--r--   0 ChungNT    (501) staff       (20)        0 2021-08-17 18:16:25.000000 mobio-cli-1.0.5/mobio_cli/templates/src/controllers/empty
+-rw-r--r--   0 ChungNT    (501) staff       (20)      760 2021-07-18 18:03:26.000000 mobio-cli-1.0.5/mobio_cli/templates/startup.sh
+-rw-r--r--   0 ChungNT    (501) staff       (20)      214 2021-10-11 09:16:05.000000 mobio-cli-1.0.5/mobio_cli/templates/test.env
+drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-06-20 04:57:42.000000 mobio-cli-1.0.5/mobio_cli/templates/yaml/
+drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-06-20 04:57:42.000000 mobio-cli-1.0.5/mobio_cli/templates/yaml/BASE/
+-rw-r--r--   0 ChungNT    (501) staff       (20)     1932 2023-06-20 04:54:17.000000 mobio-cli-1.0.5/mobio_cli/templates/yaml/BASE/deploy_{#PROJECT_NAME_SNAKE_LOWERCASE#}_app_api.yaml
+drwxr-xr-x   0 ChungNT    (501) staff       (20)        0 2023-06-20 04:57:42.000000 mobio-cli-1.0.5/mobio_cli.egg-info/
+-rw-r--r--   0 ChungNT    (501) staff       (20)     1127 2023-06-20 04:57:42.000000 mobio-cli-1.0.5/mobio_cli.egg-info/PKG-INFO
+-rw-r--r--   0 ChungNT    (501) staff       (20)     1184 2023-06-20 04:57:42.000000 mobio-cli-1.0.5/mobio_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 ChungNT    (501) staff       (20)        1 2023-06-20 04:57:42.000000 mobio-cli-1.0.5/mobio_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 ChungNT    (501) staff       (20)       55 2023-06-20 04:57:42.000000 mobio-cli-1.0.5/mobio_cli.egg-info/entry_points.txt
+-rw-r--r--   0 ChungNT    (501) staff       (20)       10 2023-06-20 04:57:42.000000 mobio-cli-1.0.5/mobio_cli.egg-info/top_level.txt
+-rw-r--r--   0 ChungNT    (501) staff       (20)       38 2023-06-20 04:57:42.000000 mobio-cli-1.0.5/setup.cfg
+-rw-r--r--   0 ChungNT    (501) staff       (20)     1211 2023-06-20 04:57:41.000000 mobio-cli-1.0.5/setup.py
```

### Comparing `mobio-cli-1.0.4/PKG-INFO` & `mobio-cli-1.0.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobio-cli
-Version: 1.0.4
+Version: 1.0.5
 Summary: Command line create Mobio's projects
 Home-page: UNKNOWN
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -14,26 +14,30 @@
 
 ## Tool generate Mobio Python Project
 
 ## Copyright: MobioVN
 
 ## Version:
 
-Phiên bản hiện tại `1.0.4`. Xem [changelog](#Changlog)
+Phiên bản hiện tại `1.0.5`. Xem [changelog](#Changlog)
 
 ## Cài đặt:
 
 `pip3 install mobio-cli`
 
 ## Sử dụng:
 
 `mobio-cli`
 
 ## Changelog:
 
+#### v1.0.5:
+* Cập nhật file .yaml (Thêm secretRef).
+* Upgrade dependency mobio-base-sdk==1.0.13.
+
 #### v1.0.4:
 * Cập nhật lại version trong README.
 
 #### v1.0.3:
 * Tương thích với Mobio base SDK mới. [See](https://pypi.org/project/mobio-base-sdk/1.0.12/)
 * Sửa lại format các file sinh tự động theo thống nhất họp mới nhất.
 * Loại bỏ một số file (do đã được merge vào Base SDK): logging, lang_config, common/__init__,...
```

### Comparing `mobio-cli-1.0.4/README.md` & `mobio-cli-1.0.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 ## Tool generate Mobio Python Project
 
 ## Copyright: MobioVN
 
 ## Version:
 
-Phiên bản hiện tại `1.0.4`. Xem [changelog](#Changlog)
+Phiên bản hiện tại `1.0.5`. Xem [changelog](#Changlog)
 
 ## Cài đặt:
 
 `pip3 install mobio-cli`
 
 ## Sử dụng:
 
 `mobio-cli`
 
 ## Changelog:
 
+#### v1.0.5:
+* Cập nhật file .yaml (Thêm secretRef).
+* Upgrade dependency mobio-base-sdk==1.0.13.
+
 #### v1.0.4:
 * Cập nhật lại version trong README.
 
 #### v1.0.3:
 * Tương thích với Mobio base SDK mới. [See](https://pypi.org/project/mobio-base-sdk/1.0.12/)
 * Sửa lại format các file sinh tự động theo thống nhất họp mới nhất.
 * Loại bỏ một số file (do đã được merge vào Base SDK): logging, lang_config, common/__init__,...
```

### Comparing `mobio-cli-1.0.4/mobio_cli/__main__.py` & `mobio-cli-1.0.5/mobio_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `mobio-cli-1.0.4/mobio_cli/templates/Dockerfile` & `mobio-cli-1.0.5/mobio_cli/templates/Dockerfile`

 * *Files identical despite different names*

### Comparing `mobio-cli-1.0.4/mobio_cli/templates/Dockerfile-release` & `mobio-cli-1.0.5/mobio_cli/templates/Dockerfile-release`

 * *Files identical despite different names*

### Comparing `mobio-cli-1.0.4/mobio_cli/templates/configs/__init__.{pymobio}` & `mobio-cli-1.0.5/mobio_cli/templates/configs/__init__.{pymobio}`

 * *Files identical despite different names*

### Comparing `mobio-cli-1.0.4/mobio_cli/templates/k8s-Jenkinsfile` & `mobio-cli-1.0.5/mobio_cli/templates/k8s-Jenkinsfile`

 * *Files identical despite different names*

### Comparing `mobio-cli-1.0.4/mobio_cli/templates/resources/lang/message_en.json` & `mobio-cli-1.0.5/mobio_cli/templates/resources/lang/message_en.json`

 * *Files identical despite different names*

### Comparing `mobio-cli-1.0.4/mobio_cli/templates/resources/lang/message_vi.json` & `mobio-cli-1.0.5/mobio_cli/templates/resources/lang/message_vi.json`

 * *Files identical despite different names*

### Comparing `mobio-cli-1.0.4/mobio_cli/templates/src/apis/__init__.{pymobio}` & `mobio-cli-1.0.5/mobio_cli/templates/src/apis/__init__.{pymobio}`

 * *Files identical despite different names*

### Comparing `mobio-cli-1.0.4/mobio_cli/templates/startup.sh` & `mobio-cli-1.0.5/mobio_cli/templates/startup.sh`

 * *Files identical despite different names*

### Comparing `mobio-cli-1.0.4/mobio_cli/templates/yaml/BASE/deploy_{#PROJECT_NAME_SNAKE_LOWERCASE#}_app_api.yaml` & `mobio-cli-1.0.5/mobio_cli/templates/yaml/BASE/deploy_{#PROJECT_NAME_SNAKE_LOWERCASE#}_app_api.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -13,20 +13,22 @@
    metadata:
      labels:
        app: {#PROJECT_NAME_KEBAB_LOWERCASE#}-app-api
    spec:
      containers:
        - name: {#PROJECT_NAME_KEBAB_LOWERCASE#}
          image: {image}
-         imagePullPolicy: Always
+         imagePullPolicy: IfNotPresent
          command: ["/bin/sh", "-c"]
          args: ["cd ${#PROJECT_NAME_SNAKE_UPPERCASE#}_HOME; sh prepare_env.sh && uwsgi --http :{#PROJECT_PORT#} --wsgi-file app_{#PROJECT_NAME_SNAKE_LOWERCASE#}_api.py --callable app --master --processes 4 -b 65536 --lazy --enable-threads"]
          envFrom:
            - configMapRef:
                name: mobio-config
+           - secretRef:
+               name: mobio-secret
          ports:
            - containerPort: {#PROJECT_PORT#}
          resources:
            requests:
              memory: 70Mi
              cpu: 80m
            limits:
@@ -38,14 +40,15 @@
          livenessProbe:
            httpGet:
              port: {#PROJECT_PORT#}
              path: /api/v1.0/ping
            initialDelaySeconds: 120
            periodSeconds: 5
            timeoutSeconds: 4
+           successThreshold: 1
            failureThreshold: 3
      imagePullSecrets:
        - name: registrypullsecret
      volumes:
        - name: mobio-shared-data
          persistentVolumeClaim:
            claimName: mobio-resources-pvc
@@ -56,8 +59,8 @@
  name: {#PROJECT_NAME_KEBAB_LOWERCASE#}-app-api-service
  labels:
    app: {#PROJECT_NAME_KEBAB_LOWERCASE#}-app-api
 spec:
  ports:
    - port: {#PROJECT_PORT#}
  selector:
-   app: {#PROJECT_NAME_KEBAB_LOWERCASE#}-app-api
+   app: {#PROJECT_NAME_KEBAB_LOWERCASE#}-app-api
```

### Comparing `mobio-cli-1.0.4/mobio_cli.egg-info/PKG-INFO` & `mobio-cli-1.0.5/mobio_cli.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobio-cli
-Version: 1.0.4
+Version: 1.0.5
 Summary: Command line create Mobio's projects
 Home-page: UNKNOWN
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -14,26 +14,30 @@
 
 ## Tool generate Mobio Python Project
 
 ## Copyright: MobioVN
 
 ## Version:
 
-Phiên bản hiện tại `1.0.4`. Xem [changelog](#Changlog)
+Phiên bản hiện tại `1.0.5`. Xem [changelog](#Changlog)
 
 ## Cài đặt:
 
 `pip3 install mobio-cli`
 
 ## Sử dụng:
 
 `mobio-cli`
 
 ## Changelog:
 
+#### v1.0.5:
+* Cập nhật file .yaml (Thêm secretRef).
+* Upgrade dependency mobio-base-sdk==1.0.13.
+
 #### v1.0.4:
 * Cập nhật lại version trong README.
 
 #### v1.0.3:
 * Tương thích với Mobio base SDK mới. [See](https://pypi.org/project/mobio-base-sdk/1.0.12/)
 * Sửa lại format các file sinh tự động theo thống nhất họp mới nhất.
 * Loại bỏ một số file (do đã được merge vào Base SDK): logging, lang_config, common/__init__,...
```

### Comparing `mobio-cli-1.0.4/mobio_cli.egg-info/SOURCES.txt` & `mobio-cli-1.0.5/mobio_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mobio-cli-1.0.4/setup.py` & `mobio-cli-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             paths.append(os.path.join(path, filename))
     return paths
 
 
 data_files = package_data_files(os.path.join(__PACKAGE_NAME__, __TEMPLATE_DIR__))
 
 setup(name='mobio-cli',
-      version='1.0.4',
+      version='1.0.5',
       author='MOBIO',
       author_email='contact@mobio.vn',
       description='Command line create Mobio\'s projects',
       long_description=long_description,
       long_description_content_type='text/markdown',
       entry_points={
           'console_scripts': [
```

