# Comparing `tmp/opal-server-0.7.0.tar.gz` & `tmp/opal-server-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opal-server-0.7.0.tar", last modified: Wed May 10 19:01:52 2023, max compression
+gzip compressed data, was "opal-server-0.7.1.tar", last modified: Tue Jun 20 13:40:53 2023, max compression
```

## Comparing `opal-server-0.7.0.tar` & `opal-server-0.7.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.878517 opal-server-0.7.0/
--rw-r--r--   0 asafc      (501) staff       (20)     8558 2023-05-10 19:01:52.878184 opal-server-0.7.0/PKG-INFO
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.874484 opal-server-0.7.0/opal_server/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-server-0.7.0/opal_server/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     2136 2023-05-10 06:45:11.000000 opal-server-0.7.0/opal_server/cli.py
--rw-r--r--   0 asafc      (501) staff       (20)    10459 2023-05-10 17:44:40.000000 opal-server-0.7.0/opal_server/config.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.875663 opal-server-0.7.0/opal_server/data/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-server-0.7.0/opal_server/data/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     5297 2022-10-12 14:50:19.000000 opal-server-0.7.0/opal_server/data/api.py
--rw-r--r--   0 asafc      (501) staff       (20)     6110 2023-05-10 06:45:11.000000 opal-server-0.7.0/opal_server/data/data_update_publisher.py
--rw-r--r--   0 asafc      (501) staff       (20)    13130 2023-05-10 06:45:11.000000 opal-server-0.7.0/opal_server/git_fetcher.py
--rw-r--r--   0 asafc      (501) staff       (20)      987 2022-10-01 21:13:25.000000 opal-server-0.7.0/opal_server/loadlimiting.py
--rw-r--r--   0 asafc      (501) staff       (20)      153 2022-10-01 21:13:25.000000 opal-server-0.7.0/opal_server/main.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.875775 opal-server-0.7.0/opal_server/policy/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-server-0.7.0/opal_server/policy/__init__.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.875946 opal-server-0.7.0/opal_server/policy/bundles/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-server-0.7.0/opal_server/policy/bundles/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     4447 2023-05-10 17:44:40.000000 opal-server-0.7.0/opal_server/policy/bundles/api.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.876374 opal-server-0.7.0/opal_server/policy/watcher/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-10 06:45:11.000000 opal-server-0.7.0/opal_server/policy/watcher/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     4459 2023-02-27 16:56:34.000000 opal-server-0.7.0/opal_server/policy/watcher/callbacks.py
--rw-r--r--   0 asafc      (501) staff       (20)     5689 2023-05-10 17:44:40.000000 opal-server-0.7.0/opal_server/policy/watcher/factory.py
--rw-r--r--   0 asafc      (501) staff       (20)     4283 2023-05-10 06:45:11.000000 opal-server-0.7.0/opal_server/policy/watcher/task.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.876837 opal-server-0.7.0/opal_server/policy/webhook/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-server-0.7.0/opal_server/policy/webhook/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     5691 2023-05-10 06:45:11.000000 opal-server-0.7.0/opal_server/policy/webhook/api.py
--rw-r--r--   0 asafc      (501) staff       (20)     6110 2023-02-24 20:59:56.000000 opal-server-0.7.0/opal_server/policy/webhook/deps.py
--rw-r--r--   0 asafc      (501) staff       (20)     1234 2022-10-01 21:13:25.000000 opal-server-0.7.0/opal_server/policy/webhook/listener.py
--rw-r--r--   0 asafc      (501) staff       (20)     1331 2022-10-01 21:13:25.000000 opal-server-0.7.0/opal_server/publisher.py
--rw-r--r--   0 asafc      (501) staff       (20)     3659 2023-05-10 06:45:11.000000 opal-server-0.7.0/opal_server/pubsub.py
--rw-r--r--   0 asafc      (501) staff       (20)     1390 2022-10-11 10:23:16.000000 opal-server-0.7.0/opal_server/redis.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.877665 opal-server-0.7.0/opal_server/scopes/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-server-0.7.0/opal_server/scopes/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)    12600 2023-05-10 06:45:11.000000 opal-server-0.7.0/opal_server/scopes/api.py
--rw-r--r--   0 asafc      (501) staff       (20)     1621 2023-05-10 06:45:11.000000 opal-server-0.7.0/opal_server/scopes/loader.py
--rw-r--r--   0 asafc      (501) staff       (20)     1325 2022-10-11 10:23:16.000000 opal-server-0.7.0/opal_server/scopes/scope_repository.py
--rw-r--r--   0 asafc      (501) staff       (20)     7285 2023-05-10 06:45:11.000000 opal-server-0.7.0/opal_server/scopes/service.py
--rw-r--r--   0 asafc      (501) staff       (20)     2811 2023-05-10 06:45:11.000000 opal-server-0.7.0/opal_server/scopes/task.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.877992 opal-server-0.7.0/opal_server/security/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:13:25.000000 opal-server-0.7.0/opal_server/security/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     1423 2022-10-11 10:23:16.000000 opal-server-0.7.0/opal_server/security/api.py
--rw-r--r--   0 asafc      (501) staff       (20)     1277 2022-10-01 21:13:25.000000 opal-server-0.7.0/opal_server/security/jwks.py
--rw-r--r--   0 asafc      (501) staff       (20)    17522 2023-05-10 06:45:11.000000 opal-server-0.7.0/opal_server/server.py
--rw-r--r--   0 asafc      (501) staff       (20)    12533 2023-02-01 11:46:28.000000 opal-server-0.7.0/opal_server/statistics.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-10 19:01:52.875306 opal-server-0.7.0/opal_server.egg-info/
--rw-r--r--   0 asafc      (501) staff       (20)     8558 2023-05-10 19:01:52.000000 opal-server-0.7.0/opal_server.egg-info/PKG-INFO
--rw-r--r--   0 asafc      (501) staff       (20)     1246 2023-05-10 19:01:52.000000 opal-server-0.7.0/opal_server.egg-info/SOURCES.txt
--rw-r--r--   0 asafc      (501) staff       (20)        1 2023-05-10 19:01:52.000000 opal-server-0.7.0/opal_server.egg-info/dependency_links.txt
--rw-r--r--   0 asafc      (501) staff       (20)       52 2023-05-10 19:01:52.000000 opal-server-0.7.0/opal_server.egg-info/entry_points.txt
--rw-r--r--   0 asafc      (501) staff       (20)      565 2023-05-10 19:01:52.000000 opal-server-0.7.0/opal_server.egg-info/requires.txt
--rw-r--r--   0 asafc      (501) staff       (20)       12 2023-05-10 19:01:52.000000 opal-server-0.7.0/opal_server.egg-info/top_level.txt
--rw-r--r--   0 asafc      (501) staff       (20)       38 2023-05-10 19:01:52.878557 opal-server-0.7.0/setup.cfg
--rw-r--r--   0 asafc      (501) staff       (20)     2979 2022-10-01 21:13:25.000000 opal-server-0.7.0/setup.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:53.110936 opal-server-0.7.1/
+-rw-r--r--   0 roekatz    (501) staff       (20)     9134 2023-06-20 13:40:53.110675 opal-server-0.7.1/PKG-INFO
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:53.099852 opal-server-0.7.1/opal_server/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.7.1/opal_server/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2136 2023-05-29 10:10:14.000000 opal-server-0.7.1/opal_server/cli.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    11023 2023-06-03 11:34:06.000000 opal-server-0.7.1/opal_server/config.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:53.103609 opal-server-0.7.1/opal_server/data/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.7.1/opal_server/data/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     5303 2023-06-18 09:48:03.000000 opal-server-0.7.1/opal_server/data/api.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     6169 2023-06-20 13:37:00.000000 opal-server-0.7.1/opal_server/data/data_update_publisher.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    13130 2023-05-29 10:10:14.000000 opal-server-0.7.1/opal_server/git_fetcher.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      987 2022-12-08 13:40:17.000000 opal-server-0.7.1/opal_server/loadlimiting.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      153 2022-12-08 13:40:17.000000 opal-server-0.7.1/opal_server/main.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:53.103754 opal-server-0.7.1/opal_server/policy/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.7.1/opal_server/policy/__init__.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:53.104066 opal-server-0.7.1/opal_server/policy/bundles/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.7.1/opal_server/policy/bundles/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4447 2023-05-29 10:10:14.000000 opal-server-0.7.1/opal_server/policy/bundles/api.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:53.106801 opal-server-0.7.1/opal_server/policy/watcher/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2023-05-29 10:10:14.000000 opal-server-0.7.1/opal_server/policy/watcher/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4529 2023-06-18 09:48:03.000000 opal-server-0.7.1/opal_server/policy/watcher/callbacks.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     6422 2023-06-03 11:34:06.000000 opal-server-0.7.1/opal_server/policy/watcher/factory.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     4568 2023-06-18 09:48:03.000000 opal-server-0.7.1/opal_server/policy/watcher/task.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:53.107936 opal-server-0.7.1/opal_server/policy/webhook/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.7.1/opal_server/policy/webhook/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     5691 2023-05-29 10:10:14.000000 opal-server-0.7.1/opal_server/policy/webhook/api.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     6110 2023-05-29 10:10:14.000000 opal-server-0.7.1/opal_server/policy/webhook/deps.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1234 2022-12-08 13:40:17.000000 opal-server-0.7.1/opal_server/policy/webhook/listener.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1331 2022-12-08 13:40:17.000000 opal-server-0.7.1/opal_server/publisher.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     3659 2023-06-18 09:46:46.000000 opal-server-0.7.1/opal_server/pubsub.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1390 2023-05-09 07:59:18.000000 opal-server-0.7.1/opal_server/redis.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:53.109591 opal-server-0.7.1/opal_server/scopes/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.7.1/opal_server/scopes/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    12555 2023-06-18 09:48:03.000000 opal-server-0.7.1/opal_server/scopes/api.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1621 2023-05-29 10:10:14.000000 opal-server-0.7.1/opal_server/scopes/loader.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1325 2023-05-09 07:59:18.000000 opal-server-0.7.1/opal_server/scopes/scope_repository.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     7256 2023-06-20 13:37:00.000000 opal-server-0.7.1/opal_server/scopes/service.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     2811 2023-05-29 10:10:14.000000 opal-server-0.7.1/opal_server/scopes/task.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:53.110367 opal-server-0.7.1/opal_server/security/
+-rw-r--r--   0 roekatz    (501) staff       (20)        0 2022-12-08 13:40:17.000000 opal-server-0.7.1/opal_server/security/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1423 2023-05-09 07:59:18.000000 opal-server-0.7.1/opal_server/security/api.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     1277 2022-12-08 13:40:17.000000 opal-server-0.7.1/opal_server/security/jwks.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    17522 2023-05-29 10:10:14.000000 opal-server-0.7.1/opal_server/server.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    12533 2023-06-18 09:47:49.000000 opal-server-0.7.1/opal_server/statistics.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 13:40:53.103162 opal-server-0.7.1/opal_server.egg-info/
+-rw-r--r--   0 roekatz    (501) staff       (20)     9134 2023-06-20 13:40:53.000000 opal-server-0.7.1/opal_server.egg-info/PKG-INFO
+-rw-r--r--   0 roekatz    (501) staff       (20)     1246 2023-06-20 13:40:53.000000 opal-server-0.7.1/opal_server.egg-info/SOURCES.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)        1 2023-06-20 13:40:53.000000 opal-server-0.7.1/opal_server.egg-info/dependency_links.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)       52 2023-06-20 13:40:53.000000 opal-server-0.7.1/opal_server.egg-info/entry_points.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)      565 2023-06-20 13:40:53.000000 opal-server-0.7.1/opal_server.egg-info/requires.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)       12 2023-06-20 13:40:53.000000 opal-server-0.7.1/opal_server.egg-info/top_level.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)       38 2023-06-20 13:40:53.110993 opal-server-0.7.1/setup.cfg
+-rw-r--r--   0 roekatz    (501) staff       (20)     2979 2022-12-08 13:40:17.000000 opal-server-0.7.1/setup.py
```

### Comparing `opal-server-0.7.0/PKG-INFO` & `opal-server-0.7.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opal-server
-Version: 0.7.0
+Version: 0.7.1
 Summary: OPAL is an administration layer for Open Policy Agent (OPA), detecting changes to both policy and data and pushing live updates to your agents. The opal-server creates a pub/sub channel clients can subscribe to (i.e: acts as coordinator). The server also tracks a git repository (via webhook) for updates to policy (or static data) and accepts continuous data update notifications via REST api, which are then pushed to clients.
 Home-page: https://github.com/permitio/opal
 Author: Or Weis, Asaf Cohen
 Author-email: or@permit.io
 License: Apache 2.0
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
@@ -48,34 +48,37 @@
 
 <a href="https://bit.ly/permit-slack" target="_blank">
     <img src="https://img.shields.io/badge/Slack%20Community-4A154B?logo=slack&logoColor=white" alt="Join our Slack!">
 </a>
 <a href="https://twitter.com/intent/follow?original_referer=https%3A%2F%2Fpublish.twitter.com%2F%3FbuttonType%3DFollowButton%26query%3Dhttps%253A%252F%252Ftwitter.com%252Fpermit_io%26widget%3DButton&ref_src=twsrc%5Etfw&region=follow_link&screen_name=permit_io&tw_p=followbutton"><img src="https://img.shields.io/twitter/follow/permit_io?label=Follow%20%40permit_io&style=social">
 </a>
 
-
-
 ## What is OPAL?
 
-OPAL is an administration layer for <a href="https://www.openpolicyagent.org/">Open Policy Agent (OPA)</a>, detecting changes to both policy and policy data in realtime and pushing live updates to your agents. OPAL brings open-policy up to the speed needed by live applications.
+OPAL is an administration layer for Policy Engines such as <a target="_blank" href="https://www.openpolicyagent.org/">Open Policy Agent (OPA)</a>, and <a target="_blank" href="https://github.com/permitio/cedar-agent">AWS' Cedar Agent</a> detecting changes to both policy and policy data in realtime and pushing live updates to your agents. OPAL brings open-policy up to the speed needed by live applications.
 
 As your application state changes (whether it's via your APIs, DBs, git, S3 or 3rd-party SaaS services), OPAL will make sure your services are always in sync with the authorization data and policy they need (and only those they need).
 
-Check out our main site at <a href="https://opal.ac">OPAL.ac</a>, <a href="https://youtu.be/tG8jrdcc7Zo">this video</a> briefly explaining OPAL and how it works with OPA, and a deeper dive into it at [this OWASP DevSlop talk](https://www.youtube.com/watch?v=1_Iz0tRQCH4).
+Check out our main site at <a target="_blank" href="https://opal.ac">OPAL.ac</a>, <a target="_blank" href="https://youtu.be/tG8jrdcc7Zo">this video</a> briefly explaining OPAL and how it works with OPA, and a deeper dive into it at [this OWASP DevSlop talk](https://www.youtube.com/watch?v=1_Iz0tRQCH4).
 
 ## Why use OPAL?
 
 OPAL is the easiest way to keep your solution's authorization layer up-to-date in realtime. It aggregates policy and data from across the field and integrates them seamlessly into the authorization layer, and is microservices and cloud-native.
 
-## OPA + OPAL = 💜
+## OPA + OPAL == 💜
 
 While OPA (Open Policy Agent) decouples policy from code in a highly-performant and elegant way, the challenge of keeping policy agents up-to-date remains.
 This is especially true in applications, where each user interaction or API call may affect access-control decisions.
 OPAL runs in the background, supercharging policy-agents, keeping them in sync with events in realtime.
 
+## AWS Cedar + OPAL == 💪
+
+Cedar is a very powerful policy language, which powers AWS' AVP (Amazon Verified Permissions) - but what if you want to enjoy the power of Cedar on another cloud, locally, or on premise?
+This is where [Cedar-Agent](https://github.com/permitio/cedar-agent) and OPAL come in.
+
 ## Documentation
 
 - 📃 &nbsp; [Full documentation is available here](https://docs.opal.ac)
 - 💡 &nbsp; [Intro to OPAL](https://docs.opal.ac/getting-started/intro)
 - 🚀 &nbsp; Getting Started:
 
   OPAL is available both as **python packages** with a built-in CLI as well as pre-built **docker images** ready-to-go.
@@ -152,7 +155,8 @@
 [badge-slack-link]: https://io.permit.io/join_community
 [follow-twitter-link]: https://i.ibb.co/k4x55Lr/Group-750.png
 [badge-twitter-link]: https://twitter.com/opal_ac
 
 ## There's more!
 
 - Check out [OPToggles](https://github.com/permitio/OPToggles), which enables you to create user targeted feature flags/toggles based on Open Policy managed authorization rules!
+- Check out [Cedar-Agent](https://github.com/permitio/cedar-agent), the easiest way to deploy & run AWS Cedar.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: opal-server Version: 0.7.0 Summary: OPAL is an
+Metadata-Version: 2.1 Name: opal-server Version: 0.7.1 Summary: OPAL is an
 administration layer for Open Policy Agent (OPA), detecting changes to both
 policy and data and pushing live updates to your agents. The opal-server
 creates a pub/sub channel clients can subscribe to (i.e: acts as coordinator).
 The server also tracks a git repository (via webhook) for updates to policy (or
 static data) and accepts continuous data update notifications via REST api,
 which are then pushed to clients. Home-page: https://github.com/permitio/opal
 Author: Or Weis, Asaf Cohen Author-email: or@permit.io License: Apache 2.0
@@ -15,43 +15,47 @@
 Requires-Python: >=3.7 Description-Content-Type: text/markdown
                                     [opal]
                            ****** â¡OPALâ¡ ******
                  ***** Open Policy Administration Layer *****
 [Tests] [Package] [Package] [Downloads] [Docker_pulls] [Join_our_Slack!]
 [https://img.shields.io/twitter/follow/
 permit_io?label=Follow%20%40permit_io&style=social] ## What is OPAL? OPAL is an
-administration layer for Open_Policy_Agent_(OPA), detecting changes to both
-policy and policy data in realtime and pushing live updates to your agents.
-OPAL brings open-policy up to the speed needed by live applications. As your
-application state changes (whether it's via your APIs, DBs, git, S3 or 3rd-
-party SaaS services), OPAL will make sure your services are always in sync with
-the authorization data and policy they need (and only those they need). Check
-out our main site at OPAL.ac, this_video briefly explaining OPAL and how it
-works with OPA, and a deeper dive into it at [this OWASP DevSlop talk](https://
-www.youtube.com/watch?v=1_Iz0tRQCH4). ## Why use OPAL? OPAL is the easiest way
-to keep your solution's authorization layer up-to-date in realtime. It
-aggregates policy and data from across the field and integrates them seamlessly
-into the authorization layer, and is microservices and cloud-native. ## OPA +
-OPAL = ð While OPA (Open Policy Agent) decouples policy from code in a
-highly-performant and elegant way, the challenge of keeping policy agents up-
-to-date remains. This is especially true in applications, where each user
-interaction or API call may affect access-control decisions. OPAL runs in the
-background, supercharging policy-agents, keeping them in sync with events in
-realtime. ## Documentation - ð   [Full documentation is available here]
-(https://docs.opal.ac) - ð¡   [Intro to OPAL](https://docs.opal.ac/getting-
-started/intro) - ð   Getting Started: OPAL is available both as **python
-packages** with a built-in CLI as well as pre-built **docker images** ready-to-
-go. - [Play with a live playground environment in docker-compose](https://
-docs.opal.ac/getting-started/quickstart/opal-playground/overview)  - [Try the
-getting started guide for containers](https://docs.opal.ac/getting-started/
-running-opal/overview)  - [Check out the Helm Chart for Kubernetes](https://
-github.com/permitio/opal-helm-chart) - A video demo of OPAL is available [here]
-(https://www.youtube.com/watch?v=IkR6EGY3QfM) - You can also check out this
-webinar and Q&A about OPAL [on our YouTube channel](https://www.youtube.com/
-watch?v=A5adHlkmdC0&t=1s)
+administration layer for Policy Engines such as Open_Policy_Agent_(OPA), and
+AWS'_Cedar_Agent detecting changes to both policy and policy data in realtime
+and pushing live updates to your agents. OPAL brings open-policy up to the
+speed needed by live applications. As your application state changes (whether
+it's via your APIs, DBs, git, S3 or 3rd-party SaaS services), OPAL will make
+sure your services are always in sync with the authorization data and policy
+they need (and only those they need). Check out our main site at OPAL.ac, this
+video briefly explaining OPAL and how it works with OPA, and a deeper dive into
+it at [this OWASP DevSlop talk](https://www.youtube.com/watch?v=1_Iz0tRQCH4).
+## Why use OPAL? OPAL is the easiest way to keep your solution's authorization
+layer up-to-date in realtime. It aggregates policy and data from across the
+field and integrates them seamlessly into the authorization layer, and is
+microservices and cloud-native. ## OPA + OPAL == ð While OPA (Open Policy
+Agent) decouples policy from code in a highly-performant and elegant way, the
+challenge of keeping policy agents up-to-date remains. This is especially true
+in applications, where each user interaction or API call may affect access-
+control decisions. OPAL runs in the background, supercharging policy-agents,
+keeping them in sync with events in realtime. ## AWS Cedar + OPAL == ðª Cedar
+is a very powerful policy language, which powers AWS' AVP (Amazon Verified
+Permissions) - but what if you want to enjoy the power of Cedar on another
+cloud, locally, or on premise? This is where [Cedar-Agent](https://github.com/
+permitio/cedar-agent) and OPAL come in. ## Documentation - ð   [Full
+documentation is available here](https://docs.opal.ac) - ð¡   [Intro to OPAL]
+(https://docs.opal.ac/getting-started/intro) - ð   Getting Started: OPAL is
+available both as **python packages** with a built-in CLI as well as pre-built
+**docker images** ready-to-go. - [Play with a live playground environment in
+docker-compose](https://docs.opal.ac/getting-started/quickstart/opal-
+playground/overview)  - [Try the getting started guide for containers](https://
+docs.opal.ac/getting-started/running-opal/overview)  - [Check out the Helm
+Chart for Kubernetes](https://github.com/permitio/opal-helm-chart) - A video
+demo of OPAL is available [here](https://www.youtube.com/watch?v=IkR6EGY3QfM) -
+You can also check out this webinar and Q&A about OPAL [on our YouTube channel]
+(https://www.youtube.com/watch?v=A5adHlkmdC0&t=1s)
 - ðª   TL;DR - This one command will download and run a working configuration
 of OPAL server and OPAL client on your machine: ``` curl -L https://
 raw.githubusercontent.com/permitio/opal/master/docker/docker-compose-
 example.yml \ > docker-compose.yml && docker-compose up ```
 [https://asciinema.org/a/409288.svg]
 - ð§    "How-To"s - [How to get started with OPAL (Packages and CLI)](https://
 docs.opal.ac/getting-started/running-opal/as-python-package/overview) - [How to
@@ -83,8 +87,9 @@
 and docs) - Prior to submitting a PR - open an issue on GitHub, or make sure
 your PR addresses an existing issue well. [join-slack-link]: https://i.ibb.co/
 wzrGHQL/Group-749.png [badge-slack-link]: https://io.permit.io/join_community
 [follow-twitter-link]: https://i.ibb.co/k4x55Lr/Group-750.png [badge-twitter-
 link]: https://twitter.com/opal_ac ## There's more! - Check out [OPToggles]
 (https://github.com/permitio/OPToggles), which enables you to create user
 targeted feature flags/toggles based on Open Policy managed authorization
-rules!
+rules! - Check out [Cedar-Agent](https://github.com/permitio/cedar-agent), the
+easiest way to deploy & run AWS Cedar.
```

### Comparing `opal-server-0.7.0/opal_server/cli.py` & `opal-server-0.7.1/opal_server/cli.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.0/opal_server/config.py` & `opal-server-0.7.1/opal_server/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,19 @@
 
 
 class PolicySourceTypes(str, Enum):
     Git = "GIT"
     Api = "API"
 
 
+class PolicyBundleServerType(str, Enum):
+    HTTP = "HTTP"
+    AWS_S3 = "AWS-S3"
+
+
 class ServerRole(str, Enum):
     Primary = "primary"
     Secondary = "secondary"
 
 
 class OpalServerConfig(Confi):
     # ws server
@@ -103,18 +108,29 @@
     )
     POLICY_REPO_CLONE_TIMEOUT = confi.int(
         "POLICY_REPO_CLONE_TIMEOUT", 0
     )  # if 0, waits forever until successful clone
     LEADER_LOCK_FILE_PATH = confi.str(
         "LEADER_LOCK_FILE_PATH", "/tmp/opal_server_leader.lock"
     )
+    POLICY_BUNDLE_SERVER_TYPE = confi.enum(
+        "POLICY_BUNDLE_SERVER_TYPE",
+        PolicyBundleServerType,
+        PolicyBundleServerType.HTTP,
+        description="The type of bundle server e.g. basic HTTP , AWS S3. (affects how we authenticate with it)",
+    )
     POLICY_BUNDLE_SERVER_TOKEN = confi.str(
         "POLICY_BUNDLE_SERVER_TOKEN",
         None,
-        description="Bearer token to sent to API bundle server",
+        description="Secret token to be sent to API bundle server",
+    )
+    POLICY_BUNDLE_SERVER_TOKEN_ID = confi.str(
+        "POLICY_BUNDLE_SERVER_TOKEN_ID",
+        None,
+        description="The id of the secret token to be sent to API bundle server",
     )
     POLICY_BUNDLE_TMP_PATH = confi.str(
         "POLICY_BUNDLE_TMP_PATH",
         "/tmp/bundle.tar.gz",
         description="Path for temp policy file, need to be writeable",
     )
     POLICY_BUNDLE_GIT_ADD_PATTERN = confi.str(
@@ -155,15 +171,17 @@
         "STATISTICS_STATE_SYNC_CHANNEL",
         "__opal_stats_state_sync",
         description="The topic other servers with statistics provide their state to a waking-up server",
     )
 
     # Data updates
     ALL_DATA_TOPIC = confi.str(
-        "ALL_DATA_TOPIC", DEFAULT_DATA_TOPIC, description="Top level topic for data"
+        "ALL_DATA_TOPIC",
+        DEFAULT_DATA_TOPIC,
+        description="Top level topic for data",
     )
     ALL_DATA_ROUTE = confi.str("ALL_DATA_ROUTE", "/policy-data")
     ALL_DATA_URL = confi.str(
         "ALL_DATA_URL",
         confi.delay("http://localhost:7002{ALL_DATA_ROUTE}"),
         description="URL for all data config [If you choose to have it all at one place]",
     )
@@ -239,15 +257,15 @@
         "127.0.0.1",
         description="(if run via CLI)  Address for the server to bind",
     )
 
     SERVER_PORT = confi.str(
         "SERVER_PORT",
         None,
-        # Users have expirienced errors when kubernetes sets the envar OPAL_SERVER_PORT="tcp://..." (which fails to parse as a port integer).
+        # Users have experienced errors when kubernetes sets the env-var OPAL_SERVER_PORT="tcp://..." (which fails to parse as a port integer).
         description="Deprecated, use SERVER_BIND_PORT instead",
     )
 
     SERVER_BIND_PORT = confi.int(
         "SERVER_BIND_PORT",
         7002,
         description="(if run via CLI)  Port for the server to bind",
```

### Comparing `opal-server-0.7.0/opal_server/data/api.py` & `opal-server-0.7.1/opal_server/data/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,11 +124,11 @@
             restrict_optional_topics_to_publish(
                 authenticator, claims, update
             )  # may throw Unauthorized
         except Unauthorized as e:
             logger.error(f"Unauthorized to publish update: {repr(e)}")
             raise
 
-        data_update_publisher.publish_data_updates(update)
+        await data_update_publisher.publish_data_updates(update)
         return {"status": "ok"}
 
     return router
```

### Comparing `opal-server-0.7.0/opal_server/data/data_update_publisher.py` & `opal-server-0.7.1/opal_server/data/data_update_publisher.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
                             f"{prefix}{PREFIX_DELIMITER}{current_topic}"
                         )
                     else:
                         topic_combos.append(current_topic)
 
         return topic_combos
 
-    def publish_data_updates(self, update: DataUpdate):
+    async def publish_data_updates(self, update: DataUpdate):
         """Notify OPAL subscribers of a new data update by topic.
 
         Args:
             topics (List[str]): topics (with hierarchy) to notify subscribers of
             update (DataUpdate): update data-source configuration for subscribers to fetch data from
         """
         all_topic_combos = set()
@@ -103,26 +103,28 @@
         logger.info(
             "[{pid}] Publishing data update to topics: {topics}, reason: {reason}, entries: {entries}",
             pid=os.getpid(),
             topics=all_topic_combos,
             reason=update.reason,
             entries=logged_entries,
         )
-        self._publisher.publish(list(all_topic_combos), update)
+
+        async with self._publisher:
+            await self._publisher.publish(list(all_topic_combos), update)
 
     async def _periodic_update_callback(
         self, update: DataSourceEntryWithPollingInterval
     ):
         """Called for every periodic update based on repeat_every."""
         logger.info(
             "[{pid}] Sending Periodic update: {source}", pid=os.getpid(), source=update
         )
         # Create new publish entry
 
-        return self.publish_data_updates(
+        return await self.publish_data_updates(
             DataUpdate(reason="Periodic Update", entries=[update])
         )
 
     def create_polling_updates(self, sources: ServerDataSourceConfig):
         # For every entry with a non zero period update interval, bind an interval to it
         updaters = []
         if hasattr(sources, "config") and hasattr(sources.config, "entries"):
```

### Comparing `opal-server-0.7.0/opal_server/git_fetcher.py` & `opal-server-0.7.1/opal_server/git_fetcher.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.0/opal_server/loadlimiting.py` & `opal-server-0.7.1/opal_server/loadlimiting.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.0/opal_server/policy/bundles/api.py` & `opal-server-0.7.1/opal_server/policy/bundles/api.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.0/opal_server/policy/watcher/callbacks.py` & `opal-server-0.7.1/opal_server/policy/watcher/callbacks.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,8 +112,11 @@
     repo, prompting the client to ask for *all* contents of these directories
     (and not just diffs)."""
     notification = await create_policy_update(
         old_commit, new_commit, file_extensions, bundle_ignore
     )
 
     if notification:
-        publisher.publish(topics=notification.topics, data=notification.update.dict())
+        async with publisher:
+            await publisher.publish(
+                topics=notification.topics, data=notification.update.dict()
+            )
```

### Comparing `opal-server-0.7.0/opal_server/policy/watcher/factory.py` & `opal-server-0.7.1/opal_server/policy/watcher/factory.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,14 +21,16 @@
     remote_source_url: str = None,
     clone_path_finder: RepoClonePathFinder = None,
     branch_name: str = None,
     ssh_key: Optional[str] = None,
     polling_interval: int = None,
     request_timeout: int = None,
     policy_bundle_token: str = None,
+    policy_bundle_token_id: str = None,
+    policy_bundle_server_type: str = None,
     extensions: Optional[List[str]] = None,
     bundle_ignore: Optional[List[str]] = None,
 ) -> BasePolicyWatcherTask:
     """Create a PolicyWatcherTask with Git / API policy source defined by env
     vars Load all the defaults from config if called without params.
 
     Args:
@@ -37,14 +39,16 @@
         remote_source_url(str): the base address to request the policy from
         clone_path_finder(RepoClonePathFinder): from which the local dir path for the repo clone would be retrieved
         branch_name(str):  name of remote branch in git to pull
         ssh_key (str, optional): private ssh key used to gain access to the cloned repo
         polling_interval(int):  how many seconds need to wait between polling
         request_timeout(int):  how many seconds need to wait until timeout
         policy_bundle_token(int):  auth token to include in connections to OPAL server. Defaults to POLICY_BUNDLE_SERVER_TOKEN.
+        policy_bundle_token_id(int):  id token to include in connections to OPAL server. Defaults to POLICY_BUNDLE_SERVER_TOKEN_ID.
+        policy_bundle_server_type (str): type of policy bundle server (HTTP S3). Defaults to POLICY_BUNDLE_SERVER_TYPE
         extensions(list(str), optional):  list of extantions to check when new policy arrive default is FILTER_FILE_EXTENSIONS
         bundle_ignore(list(str), optional):  list of glob paths to use for excluding files from bundle default is OPA_BUNDLE_IGNORE
     """
     if opal_server_config.SCOPES:
         return ScopesPolicyWatcherTask(pubsub_endpoint)
 
     # load defaults
@@ -101,19 +105,27 @@
         remote_source_url = load_conf_if_none(
             remote_source_url, opal_server_config.POLICY_BUNDLE_URL
         )
         if remote_source_url is None:
             logger.warning(
                 "POLICY_BUNDLE_URL is unset but policy watcher is enabled! disabling watcher."
             )
+        policy_bundle_token_id = load_conf_if_none(
+            policy_bundle_token_id, opal_server_config.POLICY_BUNDLE_SERVER_TOKEN_ID
+        )
+        policy_bundle_server_type = load_conf_if_none(
+            policy_bundle_server_type, opal_server_config.POLICY_BUNDLE_SERVER_TYPE
+        )
         watcher = ApiPolicySource(
             remote_source_url=remote_source_url,
             local_clone_path=clone_path,
             polling_interval=polling_interval,
             token=policy_bundle_token,
+            token_id=policy_bundle_token_id,
+            bundle_server_type=policy_bundle_server_type,
             policy_bundle_path=opal_server_config.POLICY_BUNDLE_TMP_PATH,
             policy_bundle_git_add_pattern=opal_server_config.POLICY_BUNDLE_GIT_ADD_PATTERN,
         )
     else:
         raise ValueError("Unknown value for OPAL_POLICY_SOURCE_TYPE")
     watcher.add_on_new_policy_callback(
         partial(
```

### Comparing `opal-server-0.7.0/opal_server/policy/watcher/task.py` & `opal-server-0.7.1/opal_server/policy/watcher/task.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,25 +13,31 @@
 class BasePolicyWatcherTask:
     """Manages the asyncio tasks of the policy watcher."""
 
     def __init__(self, pubsub_endpoint: PubSubEndpoint):
         self._tasks: List[asyncio.Task] = []
         self._should_stop: Optional[asyncio.Event] = None
         self._pubsub_endpoint = pubsub_endpoint
+        self._webhook_tasks: List[asyncio.Task] = []
 
     async def __aenter__(self):
         await self.start()
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.stop()
 
     async def _on_webhook(self, topic: Topic, data: Any):
-        logger.info("Webhook listener triggered")
-        self._tasks.append(asyncio.create_task(self.trigger(topic, data)))
+        logger.info(f"Webhook listener triggered ({len(self._webhook_tasks)})")
+        for task in self._webhook_tasks:
+            if task.done():
+                # Clean references to finished tasks
+                self._webhook_tasks.remove(task)
+
+        self._webhook_tasks.append(asyncio.create_task(self.trigger(topic, data)))
 
     async def _listen_to_webhook_notifications(self):
         # Webhook api route can be hit randomly in all workers, so it publishes a message to the webhook topic.
         # This listener, running in the leader's context, would actually trigger the repo pull
         if self._pubsub_endpoint.broadcaster is not None:
             async with self._pubsub_endpoint.broadcaster.get_listening_context():
                 logger.info(
@@ -54,15 +60,15 @@
         logger.info("Launching policy watcher")
         self._tasks.append(asyncio.create_task(self._listen_to_webhook_notifications()))
         self._init_should_stop()
 
     async def stop(self):
         """stops all policy watcher tasks."""
         logger.info("Stopping policy watcher")
-        for task in self._tasks:
+        for task in self._tasks + self._webhook_tasks:
             if not task.done():
                 task.cancel()
         await asyncio.gather(*self._tasks, return_exceptions=True)
 
     async def trigger(self, topic: Topic, data: Any):
         """triggers the policy watcher from outside to check for changes (git
         pull)"""
```

### Comparing `opal-server-0.7.0/opal_server/policy/webhook/api.py` & `opal-server-0.7.1/opal_server/policy/webhook/api.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.0/opal_server/policy/webhook/deps.py` & `opal-server-0.7.1/opal_server/policy/webhook/deps.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.0/opal_server/policy/webhook/listener.py` & `opal-server-0.7.1/opal_server/policy/webhook/listener.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.0/opal_server/publisher.py` & `opal-server-0.7.1/opal_server/publisher.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.0/opal_server/pubsub.py` & `opal-server-0.7.1/opal_server/pubsub.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.0/opal_server/redis.py` & `opal-server-0.7.1/opal_server/redis.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.0/opal_server/scopes/api.py` & `opal-server-0.7.1/opal_server/scopes/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -338,16 +338,15 @@
             require_peer_type(authenticator, claims, PeerType.datasource)
 
             restrict_optional_topics_to_publish(authenticator, claims, update)
 
             for entry in update.entries:
                 entry.topics = [f"data:{topic}" for topic in entry.topics]
 
-            async with ScopedServerSideTopicPublisher(
-                pubsub_endpoint, scope_id
-            ) as publisher:
-                DataUpdatePublisher(publisher).publish_data_updates(update)
+            await DataUpdatePublisher(
+                ScopedServerSideTopicPublisher(pubsub_endpoint, scope_id)
+            ).publish_data_updates(update)
         except Unauthorized as ex:
             logger.error(f"Unauthorized to publish update: {repr(ex)}")
             raise
 
     return router
```

### Comparing `opal-server-0.7.0/opal_server/scopes/loader.py` & `opal-server-0.7.1/opal_server/scopes/loader.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.0/opal_server/scopes/scope_repository.py` & `opal-server-0.7.1/opal_server/scopes/scope_repository.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.0/opal_server/scopes/service.py` & `opal-server-0.7.1/opal_server/scopes/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,16 +90,15 @@
     async def trigger_notification(self, notification: PolicyUpdateMessageNotification):
         logger.info(
             f"Triggering policy update for scope {self._scope_id}: {notification.dict()}"
         )
         async with ScopedServerSideTopicPublisher(
             self._pubsub_endpoint, self._scope_id
         ) as publisher:
-            publisher.publish(notification.topics, notification.update)
-            await publisher.wait()
+            await publisher.publish(notification.topics, notification.update)
 
 
 class ScopesService:
     def __init__(
         self,
         base_dir: Path,
         scopes: ScopeRepository,
```

### Comparing `opal-server-0.7.0/opal_server/scopes/task.py` & `opal-server-0.7.1/opal_server/scopes/task.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.0/opal_server/security/api.py` & `opal-server-0.7.1/opal_server/security/api.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.0/opal_server/security/jwks.py` & `opal-server-0.7.1/opal_server/security/jwks.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.0/opal_server/server.py` & `opal-server-0.7.1/opal_server/server.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.0/opal_server/statistics.py` & `opal-server-0.7.1/opal_server/statistics.py`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.0/opal_server.egg-info/PKG-INFO` & `opal-server-0.7.1/opal_server.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opal-server
-Version: 0.7.0
+Version: 0.7.1
 Summary: OPAL is an administration layer for Open Policy Agent (OPA), detecting changes to both policy and data and pushing live updates to your agents. The opal-server creates a pub/sub channel clients can subscribe to (i.e: acts as coordinator). The server also tracks a git repository (via webhook) for updates to policy (or static data) and accepts continuous data update notifications via REST api, which are then pushed to clients.
 Home-page: https://github.com/permitio/opal
 Author: Or Weis, Asaf Cohen
 Author-email: or@permit.io
 License: Apache 2.0
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
@@ -48,34 +48,37 @@
 
 <a href="https://bit.ly/permit-slack" target="_blank">
     <img src="https://img.shields.io/badge/Slack%20Community-4A154B?logo=slack&logoColor=white" alt="Join our Slack!">
 </a>
 <a href="https://twitter.com/intent/follow?original_referer=https%3A%2F%2Fpublish.twitter.com%2F%3FbuttonType%3DFollowButton%26query%3Dhttps%253A%252F%252Ftwitter.com%252Fpermit_io%26widget%3DButton&ref_src=twsrc%5Etfw&region=follow_link&screen_name=permit_io&tw_p=followbutton"><img src="https://img.shields.io/twitter/follow/permit_io?label=Follow%20%40permit_io&style=social">
 </a>
 
-
-
 ## What is OPAL?
 
-OPAL is an administration layer for <a href="https://www.openpolicyagent.org/">Open Policy Agent (OPA)</a>, detecting changes to both policy and policy data in realtime and pushing live updates to your agents. OPAL brings open-policy up to the speed needed by live applications.
+OPAL is an administration layer for Policy Engines such as <a target="_blank" href="https://www.openpolicyagent.org/">Open Policy Agent (OPA)</a>, and <a target="_blank" href="https://github.com/permitio/cedar-agent">AWS' Cedar Agent</a> detecting changes to both policy and policy data in realtime and pushing live updates to your agents. OPAL brings open-policy up to the speed needed by live applications.
 
 As your application state changes (whether it's via your APIs, DBs, git, S3 or 3rd-party SaaS services), OPAL will make sure your services are always in sync with the authorization data and policy they need (and only those they need).
 
-Check out our main site at <a href="https://opal.ac">OPAL.ac</a>, <a href="https://youtu.be/tG8jrdcc7Zo">this video</a> briefly explaining OPAL and how it works with OPA, and a deeper dive into it at [this OWASP DevSlop talk](https://www.youtube.com/watch?v=1_Iz0tRQCH4).
+Check out our main site at <a target="_blank" href="https://opal.ac">OPAL.ac</a>, <a target="_blank" href="https://youtu.be/tG8jrdcc7Zo">this video</a> briefly explaining OPAL and how it works with OPA, and a deeper dive into it at [this OWASP DevSlop talk](https://www.youtube.com/watch?v=1_Iz0tRQCH4).
 
 ## Why use OPAL?
 
 OPAL is the easiest way to keep your solution's authorization layer up-to-date in realtime. It aggregates policy and data from across the field and integrates them seamlessly into the authorization layer, and is microservices and cloud-native.
 
-## OPA + OPAL = 💜
+## OPA + OPAL == 💜
 
 While OPA (Open Policy Agent) decouples policy from code in a highly-performant and elegant way, the challenge of keeping policy agents up-to-date remains.
 This is especially true in applications, where each user interaction or API call may affect access-control decisions.
 OPAL runs in the background, supercharging policy-agents, keeping them in sync with events in realtime.
 
+## AWS Cedar + OPAL == 💪
+
+Cedar is a very powerful policy language, which powers AWS' AVP (Amazon Verified Permissions) - but what if you want to enjoy the power of Cedar on another cloud, locally, or on premise?
+This is where [Cedar-Agent](https://github.com/permitio/cedar-agent) and OPAL come in.
+
 ## Documentation
 
 - 📃 &nbsp; [Full documentation is available here](https://docs.opal.ac)
 - 💡 &nbsp; [Intro to OPAL](https://docs.opal.ac/getting-started/intro)
 - 🚀 &nbsp; Getting Started:
 
   OPAL is available both as **python packages** with a built-in CLI as well as pre-built **docker images** ready-to-go.
@@ -152,7 +155,8 @@
 [badge-slack-link]: https://io.permit.io/join_community
 [follow-twitter-link]: https://i.ibb.co/k4x55Lr/Group-750.png
 [badge-twitter-link]: https://twitter.com/opal_ac
 
 ## There's more!
 
 - Check out [OPToggles](https://github.com/permitio/OPToggles), which enables you to create user targeted feature flags/toggles based on Open Policy managed authorization rules!
+- Check out [Cedar-Agent](https://github.com/permitio/cedar-agent), the easiest way to deploy & run AWS Cedar.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: opal-server Version: 0.7.0 Summary: OPAL is an
+Metadata-Version: 2.1 Name: opal-server Version: 0.7.1 Summary: OPAL is an
 administration layer for Open Policy Agent (OPA), detecting changes to both
 policy and data and pushing live updates to your agents. The opal-server
 creates a pub/sub channel clients can subscribe to (i.e: acts as coordinator).
 The server also tracks a git repository (via webhook) for updates to policy (or
 static data) and accepts continuous data update notifications via REST api,
 which are then pushed to clients. Home-page: https://github.com/permitio/opal
 Author: Or Weis, Asaf Cohen Author-email: or@permit.io License: Apache 2.0
@@ -15,43 +15,47 @@
 Requires-Python: >=3.7 Description-Content-Type: text/markdown
                                     [opal]
                            ****** â¡OPALâ¡ ******
                  ***** Open Policy Administration Layer *****
 [Tests] [Package] [Package] [Downloads] [Docker_pulls] [Join_our_Slack!]
 [https://img.shields.io/twitter/follow/
 permit_io?label=Follow%20%40permit_io&style=social] ## What is OPAL? OPAL is an
-administration layer for Open_Policy_Agent_(OPA), detecting changes to both
-policy and policy data in realtime and pushing live updates to your agents.
-OPAL brings open-policy up to the speed needed by live applications. As your
-application state changes (whether it's via your APIs, DBs, git, S3 or 3rd-
-party SaaS services), OPAL will make sure your services are always in sync with
-the authorization data and policy they need (and only those they need). Check
-out our main site at OPAL.ac, this_video briefly explaining OPAL and how it
-works with OPA, and a deeper dive into it at [this OWASP DevSlop talk](https://
-www.youtube.com/watch?v=1_Iz0tRQCH4). ## Why use OPAL? OPAL is the easiest way
-to keep your solution's authorization layer up-to-date in realtime. It
-aggregates policy and data from across the field and integrates them seamlessly
-into the authorization layer, and is microservices and cloud-native. ## OPA +
-OPAL = ð While OPA (Open Policy Agent) decouples policy from code in a
-highly-performant and elegant way, the challenge of keeping policy agents up-
-to-date remains. This is especially true in applications, where each user
-interaction or API call may affect access-control decisions. OPAL runs in the
-background, supercharging policy-agents, keeping them in sync with events in
-realtime. ## Documentation - ð   [Full documentation is available here]
-(https://docs.opal.ac) - ð¡   [Intro to OPAL](https://docs.opal.ac/getting-
-started/intro) - ð   Getting Started: OPAL is available both as **python
-packages** with a built-in CLI as well as pre-built **docker images** ready-to-
-go. - [Play with a live playground environment in docker-compose](https://
-docs.opal.ac/getting-started/quickstart/opal-playground/overview)  - [Try the
-getting started guide for containers](https://docs.opal.ac/getting-started/
-running-opal/overview)  - [Check out the Helm Chart for Kubernetes](https://
-github.com/permitio/opal-helm-chart) - A video demo of OPAL is available [here]
-(https://www.youtube.com/watch?v=IkR6EGY3QfM) - You can also check out this
-webinar and Q&A about OPAL [on our YouTube channel](https://www.youtube.com/
-watch?v=A5adHlkmdC0&t=1s)
+administration layer for Policy Engines such as Open_Policy_Agent_(OPA), and
+AWS'_Cedar_Agent detecting changes to both policy and policy data in realtime
+and pushing live updates to your agents. OPAL brings open-policy up to the
+speed needed by live applications. As your application state changes (whether
+it's via your APIs, DBs, git, S3 or 3rd-party SaaS services), OPAL will make
+sure your services are always in sync with the authorization data and policy
+they need (and only those they need). Check out our main site at OPAL.ac, this
+video briefly explaining OPAL and how it works with OPA, and a deeper dive into
+it at [this OWASP DevSlop talk](https://www.youtube.com/watch?v=1_Iz0tRQCH4).
+## Why use OPAL? OPAL is the easiest way to keep your solution's authorization
+layer up-to-date in realtime. It aggregates policy and data from across the
+field and integrates them seamlessly into the authorization layer, and is
+microservices and cloud-native. ## OPA + OPAL == ð While OPA (Open Policy
+Agent) decouples policy from code in a highly-performant and elegant way, the
+challenge of keeping policy agents up-to-date remains. This is especially true
+in applications, where each user interaction or API call may affect access-
+control decisions. OPAL runs in the background, supercharging policy-agents,
+keeping them in sync with events in realtime. ## AWS Cedar + OPAL == ðª Cedar
+is a very powerful policy language, which powers AWS' AVP (Amazon Verified
+Permissions) - but what if you want to enjoy the power of Cedar on another
+cloud, locally, or on premise? This is where [Cedar-Agent](https://github.com/
+permitio/cedar-agent) and OPAL come in. ## Documentation - ð   [Full
+documentation is available here](https://docs.opal.ac) - ð¡   [Intro to OPAL]
+(https://docs.opal.ac/getting-started/intro) - ð   Getting Started: OPAL is
+available both as **python packages** with a built-in CLI as well as pre-built
+**docker images** ready-to-go. - [Play with a live playground environment in
+docker-compose](https://docs.opal.ac/getting-started/quickstart/opal-
+playground/overview)  - [Try the getting started guide for containers](https://
+docs.opal.ac/getting-started/running-opal/overview)  - [Check out the Helm
+Chart for Kubernetes](https://github.com/permitio/opal-helm-chart) - A video
+demo of OPAL is available [here](https://www.youtube.com/watch?v=IkR6EGY3QfM) -
+You can also check out this webinar and Q&A about OPAL [on our YouTube channel]
+(https://www.youtube.com/watch?v=A5adHlkmdC0&t=1s)
 - ðª   TL;DR - This one command will download and run a working configuration
 of OPAL server and OPAL client on your machine: ``` curl -L https://
 raw.githubusercontent.com/permitio/opal/master/docker/docker-compose-
 example.yml \ > docker-compose.yml && docker-compose up ```
 [https://asciinema.org/a/409288.svg]
 - ð§    "How-To"s - [How to get started with OPAL (Packages and CLI)](https://
 docs.opal.ac/getting-started/running-opal/as-python-package/overview) - [How to
@@ -83,8 +87,9 @@
 and docs) - Prior to submitting a PR - open an issue on GitHub, or make sure
 your PR addresses an existing issue well. [join-slack-link]: https://i.ibb.co/
 wzrGHQL/Group-749.png [badge-slack-link]: https://io.permit.io/join_community
 [follow-twitter-link]: https://i.ibb.co/k4x55Lr/Group-750.png [badge-twitter-
 link]: https://twitter.com/opal_ac ## There's more! - Check out [OPToggles]
 (https://github.com/permitio/OPToggles), which enables you to create user
 targeted feature flags/toggles based on Open Policy managed authorization
-rules!
+rules! - Check out [Cedar-Agent](https://github.com/permitio/cedar-agent), the
+easiest way to deploy & run AWS Cedar.
```

### Comparing `opal-server-0.7.0/opal_server.egg-info/SOURCES.txt` & `opal-server-0.7.1/opal_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opal-server-0.7.0/opal_server.egg-info/requires.txt` & `opal-server-0.7.1/opal_server.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 websockets<11,>=10.3
 ddtrace<2,>=1.1.4
 slowapi<1,>=0.1.5
 aioredis<3,>=2.0.1
 pygit2<2,>=1.9.2
 asgiref<4,>=3.5.2
 redis<5,>=4.3.4
-opal-common==0.7.0
+opal-common==0.7.1
 charset-normalizer<3,>=2.0.12
 idna<4,>=3.3
 typer<1,>=0.4.1
 fastapi<1,>=0.78.0
-fastapi_websocket_pubsub==0.3.3
+fastapi_websocket_pubsub==0.3.4
 fastapi_websocket_rpc<1,>=0.1.21
 gunicorn<21,>=20.1.0
 pydantic[email]<2,>=1.9.1
 uvicorn[standard]<1,>=0.17.6
 fastapi-utils<1,>=0.2.1
 setuptools>=65.5.1
```

### Comparing `opal-server-0.7.0/setup.py` & `opal-server-0.7.1/setup.py`

 * *Files identical despite different names*

