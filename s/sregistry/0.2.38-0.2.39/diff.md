# Comparing `tmp/sregistry-0.2.38.tar.gz` & `tmp/sregistry-0.2.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sregistry-0.2.38.tar", last modified: Thu Jun 30 23:31:56 2022, max compression
+gzip compressed data, was "sregistry-0.2.39.tar", last modified: Tue Jun 20 20:15:30 2023, max compression
```

## Comparing `sregistry-0.2.38.tar` & `sregistry-0.2.39.tar`

### file list

```diff
@@ -1,177 +1,177 @@
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-06-30 23:31:56.268614 sregistry-0.2.38/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    15830 2022-06-30 04:58:23.000000 sregistry-0.2.38/LICENSE
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      370 2022-06-30 04:58:23.000000 sregistry-0.2.38/MANIFEST.in
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4515 2022-06-30 23:31:56.268614 sregistry-0.2.38/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3031 2022-06-30 04:58:23.000000 sregistry-0.2.38/README.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       38 2022-06-30 23:31:56.268614 sregistry-0.2.38/setup.cfg
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6142 2022-06-30 04:58:23.000000 sregistry-0.2.38/setup.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-06-30 23:31:56.260614 sregistry-0.2.38/sregistry/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1175 2022-06-30 04:58:23.000000 sregistry-0.2.38/sregistry/README.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      287 2022-06-30 04:58:23.000000 sregistry-0.2.38/sregistry/__init__.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-06-30 23:31:56.260614 sregistry-0.2.38/sregistry/auth/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      407 2022-06-30 04:58:23.000000 sregistry-0.2.38/sregistry/auth/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3363 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/auth/secrets.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      898 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/auth/utils.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-06-30 23:31:56.260614 sregistry-0.2.38/sregistry/client/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    11099 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/client/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      643 2022-06-30 04:58:23.000000 sregistry-0.2.38/sregistry/client/add.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6655 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/client/backend.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7853 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/client/build.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      701 2022-06-30 04:58:23.000000 sregistry-0.2.38/sregistry/client/delete.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      692 2022-06-30 04:58:23.000000 sregistry-0.2.38/sregistry/client/get.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      835 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/client/images.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      650 2022-06-30 04:58:23.000000 sregistry-0.2.38/sregistry/client/inspect.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      666 2022-06-30 04:58:23.000000 sregistry-0.2.38/sregistry/client/labels.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      904 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/client/list.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      668 2022-06-30 04:58:23.000000 sregistry-0.2.38/sregistry/client/mv.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      932 2022-06-30 04:58:23.000000 sregistry-0.2.38/sregistry/client/pull.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      860 2022-06-30 04:58:23.000000 sregistry-0.2.38/sregistry/client/push.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      645 2022-06-30 04:58:23.000000 sregistry-0.2.38/sregistry/client/rename.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      721 2022-06-30 04:58:23.000000 sregistry-0.2.38/sregistry/client/rm.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      846 2022-06-30 04:58:23.000000 sregistry-0.2.38/sregistry/client/search.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      875 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/client/share.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2181 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/client/shell.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-06-30 23:31:56.260614 sregistry-0.2.38/sregistry/database/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      409 2022-06-30 04:58:23.000000 sregistry-0.2.38/sregistry/database/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1776 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/database/dummy.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5636 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/database/models.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    88236 2022-06-30 04:58:23.000000 sregistry-0.2.38/sregistry/database/robot.png
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    14518 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/database/sqlite.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4747 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/defaults.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-06-30 23:31:56.260614 sregistry-0.2.38/sregistry/logger/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       89 2022-06-30 04:58:23.000000 sregistry-0.2.38/sregistry/logger/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     9637 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/logger/message.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4323 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/logger/namer.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4463 2022-06-30 04:58:23.000000 sregistry-0.2.38/sregistry/logger/progress.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1930 2022-06-30 04:58:23.000000 sregistry-0.2.38/sregistry/logger/spinner.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-06-30 23:31:56.260614 sregistry-0.2.38/sregistry/main/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2065 2022-06-30 04:58:23.000000 sregistry-0.2.38/sregistry/main/README.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4208 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/__init__.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-06-30 23:31:56.260614 sregistry-0.2.38/sregistry/main/__template__/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2490 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/__template__/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3627 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/__template__/pull.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1618 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/__template__/push.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2384 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/__template__/query.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-06-30 23:31:56.260614 sregistry-0.2.38/sregistry/main/aws/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3997 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/aws/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3828 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/aws/api.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4754 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/aws/pull.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-06-30 23:31:56.260614 sregistry-0.2.38/sregistry/main/base/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4278 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/base/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2698 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/base/auth.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1084 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/base/headers.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    10161 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/base/http.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2655 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/base/inspect.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4032 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/base/settings.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-06-30 23:31:56.260614 sregistry-0.2.38/sregistry/main/docker/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6585 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/docker/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    18338 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/docker/api.py
--rwxrwxr-x   0 vanessa   (1000) vanessa   (1000)     3746 2022-06-30 04:58:23.000000 sregistry-0.2.38/sregistry/main/docker/blob2oci
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2474 2022-06-30 04:58:23.000000 sregistry-0.2.38/sregistry/main/docker/environment.tar
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5213 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/docker/pull.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3470 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/docker/utils.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-06-30 23:31:56.264614 sregistry-0.2.38/sregistry/main/dropbox/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2998 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/dropbox/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3157 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/dropbox/pull.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3064 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/dropbox/push.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2173 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/dropbox/query.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1048 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/dropbox/share.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-06-30 23:31:56.264614 sregistry-0.2.38/sregistry/main/gitlab/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3815 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/gitlab/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4086 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/gitlab/pull.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2232 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/gitlab/query.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-06-30 23:31:56.264614 sregistry-0.2.38/sregistry/main/globus/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3725 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/globus/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3159 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/globus/pull.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2529 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/globus/push.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4025 2022-06-30 23:31:50.000000 sregistry-0.2.38/sregistry/main/globus/query.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4705 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/globus/utils.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-06-30 23:31:56.264614 sregistry-0.2.38/sregistry/main/google_build/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        5 2022-06-30 04:58:23.000000 sregistry-0.2.38/sregistry/main/google_build/.gitignore
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1037 2022-06-30 04:58:23.000000 sregistry-0.2.38/sregistry/main/google_build/README.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5586 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/google_build/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    19934 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/google_build/build.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2083 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/google_build/client.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1532 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/google_build/delete.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2291 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/google_build/logs.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3094 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/google_build/pull.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3273 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/google_build/push.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3358 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/google_build/query.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      965 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/google_build/utils.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-06-30 23:31:56.264614 sregistry-0.2.38/sregistry/main/google_drive/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3834 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/google_drive/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3597 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/google_drive/pull.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2503 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/google_drive/push.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4508 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/google_drive/query.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1251 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/google_drive/share.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1333 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/google_drive/utils.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-06-30 23:31:56.264614 sregistry-0.2.38/sregistry/main/google_storage/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5010 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/google_storage/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    14751 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/google_storage/build.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1531 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/google_storage/delete.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2291 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/google_storage/logs.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2996 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/google_storage/pull.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3240 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/google_storage/push.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3209 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/google_storage/query.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1634 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/google_storage/utils.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-06-30 23:31:56.264614 sregistry-0.2.38/sregistry/main/hub/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      694 2022-06-30 04:58:23.000000 sregistry-0.2.38/sregistry/main/hub/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3297 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/hub/pull.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2390 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/hub/query.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-06-30 23:31:56.264614 sregistry-0.2.38/sregistry/main/nvidia/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4790 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/nvidia/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1908 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/nvidia/pull.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-06-30 23:31:56.264614 sregistry-0.2.38/sregistry/main/registry/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3421 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/registry/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2160 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/registry/auth.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3365 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/registry/build.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1293 2022-06-30 04:58:23.000000 sregistry-0.2.38/sregistry/main/registry/delete.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4505 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/registry/pull.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3589 2022-06-30 04:58:23.000000 sregistry-0.2.38/sregistry/main/registry/push.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5672 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/registry/query.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1720 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/registry/utils.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-06-30 23:31:56.264614 sregistry-0.2.38/sregistry/main/s3/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6526 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/s3/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1044 2022-06-30 04:58:23.000000 sregistry-0.2.38/sregistry/main/s3/delete.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3320 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/s3/pull.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1577 2022-06-30 04:58:23.000000 sregistry-0.2.38/sregistry/main/s3/push.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2855 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/s3/query.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-06-30 23:31:56.264614 sregistry-0.2.38/sregistry/main/swift/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6720 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/swift/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3673 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/swift/pull.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1794 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/swift/push.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2171 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/swift/query.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-06-30 23:31:56.264614 sregistry-0.2.38/sregistry/main/templates/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2022-06-30 04:58:23.000000 sregistry-0.2.38/sregistry/main/templates/__init__.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-06-30 23:31:56.264614 sregistry-0.2.38/sregistry/main/templates/build/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2022-06-30 04:58:23.000000 sregistry-0.2.38/sregistry/main/templates/build/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5777 2022-06-30 04:58:23.000000 sregistry-0.2.38/sregistry/main/templates/build/singularity-builder-apt.sh
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       18 2022-06-30 04:58:23.000000 sregistry-0.2.38/sregistry/main/templates/build/singularity-cloudbuild-git.json
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      117 2022-06-30 04:58:23.000000 sregistry-0.2.38/sregistry/main/templates/build/singularity-cloudbuild-local.json
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-06-30 23:31:56.264614 sregistry-0.2.38/sregistry/main/workers/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      372 2022-06-30 04:58:23.000000 sregistry-0.2.38/sregistry/main/workers/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5255 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/workers/aws.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8531 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/main/workers/tasks.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3523 2022-06-30 04:58:23.000000 sregistry-0.2.38/sregistry/main/workers/worker.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-06-30 23:31:56.264614 sregistry-0.2.38/sregistry/tests/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2022-06-30 04:58:23.000000 sregistry-0.2.38/sregistry/tests/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8025 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/tests/test_utils.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-06-30 23:31:56.268614 sregistry-0.2.38/sregistry/tests/testdata/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2022-06-30 04:58:23.000000 sregistry-0.2.38/sregistry/tests/testdata/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      211 2022-06-30 04:58:23.000000 sregistry-0.2.38/sregistry/tests/testdata/hashtest.tar.gz
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      108 2022-06-30 04:58:23.000000 sregistry-0.2.38/sregistry/tests/testdata/hashtest.txt
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-06-30 23:31:56.268614 sregistry-0.2.38/sregistry/utils/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      441 2022-06-30 04:58:23.000000 sregistry-0.2.38/sregistry/utils/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7479 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/utils/fileio.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6102 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/utils/names.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2022-06-30 04:58:23.000000 sregistry-0.2.38/sregistry/utils/recipes.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5101 2022-06-30 17:46:32.000000 sregistry-0.2.38/sregistry/utils/terminal.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5521 2022-06-30 23:31:50.000000 sregistry-0.2.38/sregistry/version.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-06-30 23:31:56.260614 sregistry-0.2.38/sregistry.egg-info/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4515 2022-06-30 23:31:56.000000 sregistry-0.2.38/sregistry.egg-info/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4582 2022-06-30 23:31:56.000000 sregistry-0.2.38/sregistry.egg-info/SOURCES.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2022-06-30 23:31:56.000000 sregistry-0.2.38/sregistry.egg-info/dependency_links.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       53 2022-06-30 23:31:56.000000 sregistry-0.2.38/sregistry.egg-info/entry_points.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2022-06-30 23:31:56.000000 sregistry-0.2.38/sregistry.egg-info/not-zip-safe
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2955 2022-06-30 23:31:56.000000 sregistry-0.2.38/sregistry.egg-info/requires.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       10 2022-06-30 23:31:56.000000 sregistry-0.2.38/sregistry.egg-info/top_level.txt
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-20 20:15:30.530179 sregistry-0.2.39/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    15830 2022-06-30 04:58:23.000000 sregistry-0.2.39/LICENSE
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      370 2022-06-30 04:58:23.000000 sregistry-0.2.39/MANIFEST.in
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4515 2023-06-20 20:15:30.526179 sregistry-0.2.39/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3031 2022-06-30 04:58:23.000000 sregistry-0.2.39/README.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       38 2023-06-20 20:15:30.530179 sregistry-0.2.39/setup.cfg
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6188 2023-06-20 20:15:27.000000 sregistry-0.2.39/setup.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-20 20:15:30.506179 sregistry-0.2.39/sregistry/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1175 2022-06-30 04:58:23.000000 sregistry-0.2.39/sregistry/README.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      287 2022-06-30 04:58:23.000000 sregistry-0.2.39/sregistry/__init__.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-20 20:15:30.506179 sregistry-0.2.39/sregistry/auth/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      407 2022-06-30 04:58:23.000000 sregistry-0.2.39/sregistry/auth/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3363 2022-06-30 17:46:32.000000 sregistry-0.2.39/sregistry/auth/secrets.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      898 2022-06-30 17:46:32.000000 sregistry-0.2.39/sregistry/auth/utils.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-20 20:15:30.510179 sregistry-0.2.39/sregistry/client/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    11099 2022-06-30 17:46:32.000000 sregistry-0.2.39/sregistry/client/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      642 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/client/add.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6654 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/client/backend.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7852 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/client/build.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      700 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/client/delete.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      691 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/client/get.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      835 2022-06-30 17:46:32.000000 sregistry-0.2.39/sregistry/client/images.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      649 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/client/inspect.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      665 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/client/labels.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      904 2022-06-30 17:46:32.000000 sregistry-0.2.39/sregistry/client/list.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      667 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/client/mv.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      931 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/client/pull.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      859 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/client/push.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      644 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/client/rename.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      720 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/client/rm.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      845 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/client/search.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      875 2022-06-30 17:46:32.000000 sregistry-0.2.39/sregistry/client/share.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2180 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/client/shell.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-20 20:15:30.510179 sregistry-0.2.39/sregistry/database/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      409 2022-06-30 04:58:23.000000 sregistry-0.2.39/sregistry/database/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1775 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/database/dummy.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5636 2022-06-30 17:46:32.000000 sregistry-0.2.39/sregistry/database/models.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    88236 2022-06-30 04:58:23.000000 sregistry-0.2.39/sregistry/database/robot.png
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    14509 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/database/sqlite.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4746 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/defaults.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-20 20:15:30.510179 sregistry-0.2.39/sregistry/logger/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       89 2022-06-30 04:58:23.000000 sregistry-0.2.39/sregistry/logger/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     9636 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/logger/message.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4322 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/logger/namer.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4460 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/logger/progress.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1930 2022-06-30 04:58:23.000000 sregistry-0.2.39/sregistry/logger/spinner.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-20 20:15:30.510179 sregistry-0.2.39/sregistry/main/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2065 2022-06-30 04:58:23.000000 sregistry-0.2.39/sregistry/main/README.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4207 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/__init__.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-20 20:15:30.514179 sregistry-0.2.39/sregistry/main/__template__/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2489 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/__template__/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3626 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/__template__/pull.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1618 2022-06-30 17:46:32.000000 sregistry-0.2.39/sregistry/main/__template__/push.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2383 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/__template__/query.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-20 20:15:30.514179 sregistry-0.2.39/sregistry/main/aws/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3997 2022-06-30 17:46:32.000000 sregistry-0.2.39/sregistry/main/aws/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3827 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/aws/api.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4751 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/aws/pull.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-20 20:15:30.514179 sregistry-0.2.39/sregistry/main/base/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4276 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/base/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2696 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/base/auth.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1084 2022-06-30 17:46:32.000000 sregistry-0.2.39/sregistry/main/base/headers.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    10149 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/base/http.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2655 2022-06-30 17:46:32.000000 sregistry-0.2.39/sregistry/main/base/inspect.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4032 2022-06-30 17:46:32.000000 sregistry-0.2.39/sregistry/main/base/settings.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-20 20:15:30.514179 sregistry-0.2.39/sregistry/main/docker/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6585 2022-06-30 17:46:32.000000 sregistry-0.2.39/sregistry/main/docker/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    18334 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/docker/api.py
+-rwxrwxr-x   0 vanessa   (1000) vanessa   (1000)     3746 2022-06-30 04:58:23.000000 sregistry-0.2.39/sregistry/main/docker/blob2oci
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2474 2022-06-30 04:58:23.000000 sregistry-0.2.39/sregistry/main/docker/environment.tar
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5209 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/docker/pull.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3470 2022-06-30 17:46:32.000000 sregistry-0.2.39/sregistry/main/docker/utils.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-20 20:15:30.514179 sregistry-0.2.39/sregistry/main/dropbox/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2997 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/dropbox/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3155 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/dropbox/pull.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3062 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/dropbox/push.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2170 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/dropbox/query.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1047 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/dropbox/share.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-20 20:15:30.514179 sregistry-0.2.39/sregistry/main/gitlab/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3814 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/gitlab/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4085 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/gitlab/pull.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2230 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/gitlab/query.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-20 20:15:30.514179 sregistry-0.2.39/sregistry/main/globus/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3723 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/globus/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3158 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/globus/pull.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2529 2022-06-30 17:46:32.000000 sregistry-0.2.39/sregistry/main/globus/push.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4022 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/globus/query.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4704 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/globus/utils.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-20 20:15:30.518179 sregistry-0.2.39/sregistry/main/google_build/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        5 2022-06-30 04:58:23.000000 sregistry-0.2.39/sregistry/main/google_build/.gitignore
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1037 2022-06-30 04:58:23.000000 sregistry-0.2.39/sregistry/main/google_build/README.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5584 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/google_build/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    19929 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/google_build/build.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2082 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/google_build/client.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1532 2022-06-30 17:46:32.000000 sregistry-0.2.39/sregistry/main/google_build/delete.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2289 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/google_build/logs.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3093 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/google_build/pull.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3271 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/google_build/push.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3358 2022-06-30 17:46:32.000000 sregistry-0.2.39/sregistry/main/google_build/query.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      965 2022-06-30 17:46:32.000000 sregistry-0.2.39/sregistry/main/google_build/utils.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-20 20:15:30.518179 sregistry-0.2.39/sregistry/main/google_drive/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3833 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/google_drive/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3596 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/google_drive/pull.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2503 2022-06-30 17:46:32.000000 sregistry-0.2.39/sregistry/main/google_drive/push.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4505 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/google_drive/query.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1251 2022-06-30 17:46:32.000000 sregistry-0.2.39/sregistry/main/google_drive/share.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1333 2022-06-30 17:46:32.000000 sregistry-0.2.39/sregistry/main/google_drive/utils.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-20 20:15:30.518179 sregistry-0.2.39/sregistry/main/google_storage/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5009 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/google_storage/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    14745 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/google_storage/build.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1531 2022-06-30 17:46:32.000000 sregistry-0.2.39/sregistry/main/google_storage/delete.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2289 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/google_storage/logs.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2995 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/google_storage/pull.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3239 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/google_storage/push.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3209 2022-06-30 17:46:32.000000 sregistry-0.2.39/sregistry/main/google_storage/query.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1634 2022-06-30 17:46:32.000000 sregistry-0.2.39/sregistry/main/google_storage/utils.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-20 20:15:30.518179 sregistry-0.2.39/sregistry/main/hub/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      693 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/hub/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3296 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/hub/pull.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2390 2022-06-30 17:46:32.000000 sregistry-0.2.39/sregistry/main/hub/query.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-20 20:15:30.522179 sregistry-0.2.39/sregistry/main/nvidia/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4790 2022-06-30 17:46:32.000000 sregistry-0.2.39/sregistry/main/nvidia/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1907 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/nvidia/pull.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-20 20:15:30.522179 sregistry-0.2.39/sregistry/main/registry/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3418 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/registry/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2160 2022-06-30 17:46:32.000000 sregistry-0.2.39/sregistry/main/registry/auth.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3365 2022-06-30 17:46:32.000000 sregistry-0.2.39/sregistry/main/registry/build.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1293 2022-06-30 04:58:23.000000 sregistry-0.2.39/sregistry/main/registry/delete.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4501 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/registry/pull.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3589 2022-06-30 04:58:23.000000 sregistry-0.2.39/sregistry/main/registry/push.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5670 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/registry/query.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1720 2022-06-30 17:46:32.000000 sregistry-0.2.39/sregistry/main/registry/utils.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-20 20:15:30.522179 sregistry-0.2.39/sregistry/main/s3/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6525 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/s3/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1044 2022-06-30 04:58:23.000000 sregistry-0.2.39/sregistry/main/s3/delete.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3318 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/s3/pull.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1577 2022-06-30 04:58:23.000000 sregistry-0.2.39/sregistry/main/s3/push.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2854 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/s3/query.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-20 20:15:30.522179 sregistry-0.2.39/sregistry/main/swift/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6715 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/swift/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3671 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/swift/pull.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1794 2022-06-30 17:46:32.000000 sregistry-0.2.39/sregistry/main/swift/push.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2168 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/swift/query.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-20 20:15:30.526179 sregistry-0.2.39/sregistry/main/templates/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2022-06-30 04:58:23.000000 sregistry-0.2.39/sregistry/main/templates/__init__.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-20 20:15:30.526179 sregistry-0.2.39/sregistry/main/templates/build/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2022-06-30 04:58:23.000000 sregistry-0.2.39/sregistry/main/templates/build/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5777 2022-06-30 04:58:23.000000 sregistry-0.2.39/sregistry/main/templates/build/singularity-builder-apt.sh
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       18 2022-06-30 04:58:23.000000 sregistry-0.2.39/sregistry/main/templates/build/singularity-cloudbuild-git.json
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      117 2022-06-30 04:58:23.000000 sregistry-0.2.39/sregistry/main/templates/build/singularity-cloudbuild-local.json
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-20 20:15:30.526179 sregistry-0.2.39/sregistry/main/workers/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      372 2022-06-30 04:58:23.000000 sregistry-0.2.39/sregistry/main/workers/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5254 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/workers/aws.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8525 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/workers/tasks.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3522 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/main/workers/worker.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-20 20:15:30.526179 sregistry-0.2.39/sregistry/tests/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2022-06-30 04:58:23.000000 sregistry-0.2.39/sregistry/tests/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8025 2022-06-30 17:46:32.000000 sregistry-0.2.39/sregistry/tests/test_utils.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-20 20:15:30.526179 sregistry-0.2.39/sregistry/tests/testdata/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2022-06-30 04:58:23.000000 sregistry-0.2.39/sregistry/tests/testdata/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      211 2022-06-30 04:58:23.000000 sregistry-0.2.39/sregistry/tests/testdata/hashtest.tar.gz
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      108 2022-06-30 04:58:23.000000 sregistry-0.2.39/sregistry/tests/testdata/hashtest.txt
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-20 20:15:30.526179 sregistry-0.2.39/sregistry/utils/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      441 2022-06-30 04:58:23.000000 sregistry-0.2.39/sregistry/utils/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7479 2022-06-30 17:46:32.000000 sregistry-0.2.39/sregistry/utils/fileio.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6101 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/utils/names.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2022-06-30 04:58:23.000000 sregistry-0.2.39/sregistry/utils/recipes.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5101 2022-06-30 17:46:32.000000 sregistry-0.2.39/sregistry/utils/terminal.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5561 2023-06-20 20:15:27.000000 sregistry-0.2.39/sregistry/version.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-20 20:15:30.506179 sregistry-0.2.39/sregistry.egg-info/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4515 2023-06-20 20:15:30.000000 sregistry-0.2.39/sregistry.egg-info/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4582 2023-06-20 20:15:30.000000 sregistry-0.2.39/sregistry.egg-info/SOURCES.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-06-20 20:15:30.000000 sregistry-0.2.39/sregistry.egg-info/dependency_links.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       53 2023-06-20 20:15:30.000000 sregistry-0.2.39/sregistry.egg-info/entry_points.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2022-06-30 23:31:56.000000 sregistry-0.2.39/sregistry.egg-info/not-zip-safe
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3107 2023-06-20 20:15:30.000000 sregistry-0.2.39/sregistry.egg-info/requires.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       10 2023-06-20 20:15:30.000000 sregistry-0.2.39/sregistry.egg-info/top_level.txt
```

### Comparing `sregistry-0.2.38/LICENSE` & `sregistry-0.2.39/LICENSE`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/PKG-INFO` & `sregistry-0.2.39/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sregistry
-Version: 0.2.38
+Version: 0.2.39
 Summary: Command line tool for working with container storage
 Home-page: http://www.github.com/singularityhub/sregistry-cli
 Author: Vanessa Sochat
 Author-email: vsochat@stanford.edu
 Maintainer: Vanessa Sochat
 Maintainer-email: vsochat@stanford.edu
 License: LICENSE
```

### Comparing `sregistry-0.2.38/README.md` & `sregistry-0.2.39/README.md`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/setup.py` & `sregistry-0.2.39/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,153 +2,155 @@
 import codecs
 import os
 
 ################################################################################
 # HELPER FUNCTIONS #############################################################
 ################################################################################
 
+
 def get_lookup():
-    '''get version by way of sregistry.version, returns a 
+    """get version by way of sregistry.version, returns a
     lookup dictionary with several global variables without
     needing to import singularity
-    '''
+    """
     lookup = dict()
-    version_file = os.path.join('sregistry', 'version.py')
+    version_file = os.path.join("sregistry", "version.py")
     with open(version_file) as filey:
         exec(filey.read(), lookup)
     return lookup
 
 
 # Read in requirements
-def get_reqs(lookup=None, key='INSTALL_REQUIRES'):
-    '''get requirements, mean reading in requirements and versions from
-    the lookup obtained with get_lookup'''
+def get_reqs(lookup=None, key="INSTALL_REQUIRES"):
+    """get requirements, mean reading in requirements and versions from
+    the lookup obtained with get_lookup"""
 
     if lookup == None:
         lookup = get_lookup()
 
     install_requires = []
     for module in lookup[key]:
         module_name = module[0]
         module_meta = module[1]
         if "exact_version" in module_meta:
-            dependency = "%s==%s" %(module_name,module_meta['exact_version'])
+            dependency = "%s==%s" % (module_name, module_meta["exact_version"])
         elif "min_version" in module_meta:
-            if module_meta['min_version'] == None:
+            if module_meta["min_version"] == None:
                 dependency = module_name
             else:
-                dependency = "%s>=%s" %(module_name,module_meta['min_version'])
+                dependency = "%s>=%s" % (module_name, module_meta["min_version"])
+        elif "max_version" in module_meta:
+            dependency = "%s<=%s" % (module_name, module_meta["max_version"])
         install_requires.append(dependency)
     return install_requires
 
 
-
 # Make sure everything is relative to setup.py
-install_path = os.path.dirname(os.path.abspath(__file__)) 
+install_path = os.path.dirname(os.path.abspath(__file__))
 os.chdir(install_path)
 
 # Get version information from the lookup
 lookup = get_lookup()
-VERSION = lookup['__version__']
-NAME = lookup['NAME']
-AUTHOR = lookup['AUTHOR']
-AUTHOR_EMAIL = lookup['AUTHOR_EMAIL']
-PACKAGE_URL = lookup['PACKAGE_URL']
-KEYWORDS = lookup['KEYWORDS']
-DESCRIPTION = lookup['DESCRIPTION']
-LICENSE = lookup['LICENSE']
-with open('README.md') as filey:
+VERSION = lookup["__version__"]
+NAME = lookup["NAME"]
+AUTHOR = lookup["AUTHOR"]
+AUTHOR_EMAIL = lookup["AUTHOR_EMAIL"]
+PACKAGE_URL = lookup["PACKAGE_URL"]
+KEYWORDS = lookup["KEYWORDS"]
+DESCRIPTION = lookup["DESCRIPTION"]
+LICENSE = lookup["LICENSE"]
+with open("README.md") as filey:
     LONG_DESCRIPTION = filey.read()
 
 ################################################################################
 # MAIN #########################################################################
 ################################################################################
 
 if __name__ == "__main__":
-
     INSTALL_REQUIRES = get_reqs(lookup)
 
     # These requirement DON'T include sqlalchemy, only client
 
-    INSTALL_BASIC_ALL = get_reqs(lookup,'INSTALL_BASIC_ALL')
-    AWS_BASIC = get_reqs(lookup,'INSTALL_BASIC_AWS')
-    S3_BASIC = get_reqs(lookup,'INSTALL_BASIC_S3')
-    DROPBOX_BASIC = get_reqs(lookup,'INSTALL_BASIC_DROPBOX')
-    REGISTRY_BASIC = get_reqs(lookup,'INSTALL_BASIC_REGISTRY')
-    GLOBUS_BASIC = get_reqs(lookup,'INSTALL_BASIC_GLOBUS')
-    GOOGLE_STORAGE_BASIC = get_reqs(lookup,'INSTALL_BASIC_GOOGLE_STORAGE')
-    GOOGLE_DRIVE_BASIC = get_reqs(lookup,'INSTALL_BASIC_GOOGLE_DRIVE')
-    GOOGLE_BUILD_BASIC = get_reqs(lookup,'INSTALL_BASIC_GOOGLE_BUILD')
-    GOOGLE_COMPUTE_BASIC = get_reqs(lookup,'INSTALL_BASIC_GOOGLE_COMPUTE')
-    SWIFT_BASIC = get_reqs(lookup,'INSTALL_BASIC_SWIFT')
-    TESTS_REQUIRES = get_reqs(lookup, 'TESTS_REQUIRES')
+    INSTALL_BASIC_ALL = get_reqs(lookup, "INSTALL_BASIC_ALL")
+    AWS_BASIC = get_reqs(lookup, "INSTALL_BASIC_AWS")
+    S3_BASIC = get_reqs(lookup, "INSTALL_BASIC_S3")
+    DROPBOX_BASIC = get_reqs(lookup, "INSTALL_BASIC_DROPBOX")
+    REGISTRY_BASIC = get_reqs(lookup, "INSTALL_BASIC_REGISTRY")
+    GLOBUS_BASIC = get_reqs(lookup, "INSTALL_BASIC_GLOBUS")
+    GOOGLE_STORAGE_BASIC = get_reqs(lookup, "INSTALL_BASIC_GOOGLE_STORAGE")
+    GOOGLE_DRIVE_BASIC = get_reqs(lookup, "INSTALL_BASIC_GOOGLE_DRIVE")
+    GOOGLE_BUILD_BASIC = get_reqs(lookup, "INSTALL_BASIC_GOOGLE_BUILD")
+    GOOGLE_COMPUTE_BASIC = get_reqs(lookup, "INSTALL_BASIC_GOOGLE_COMPUTE")
+    SWIFT_BASIC = get_reqs(lookup, "INSTALL_BASIC_SWIFT")
+    TESTS_REQUIRES = get_reqs(lookup, "TESTS_REQUIRES")
 
     # These requirement sets include sqlalchemy, for client+storage
 
-    INSTALL_REQUIRES_ALL = get_reqs(lookup,'INSTALL_REQUIRES_ALL')
-    AWS = get_reqs(lookup,'INSTALL_REQUIRES_AWS')
-    S3 = get_reqs(lookup,'INSTALL_REQUIRES_S3')
-    DROPBOX = get_reqs(lookup,'INSTALL_REQUIRES_DROPBOX')
-    REGISTRY = get_reqs(lookup,'INSTALL_REQUIRES_REGISTRY')
-    GLOBUS = get_reqs(lookup,'INSTALL_REQUIRES_GLOBUS')
-    GOOGLE_STORAGE = get_reqs(lookup,'INSTALL_REQUIRES_GOOGLE_STORAGE')
-    GOOGLE_DRIVE = get_reqs(lookup,'INSTALL_REQUIRES_GOOGLE_DRIVE')
-    GOOGLE_COMPUTE = get_reqs(lookup,'INSTALL_REQUIRES_GOOGLE_COMPUTE')
-    GOOGLE_BUILD = get_reqs(lookup,'INSTALL_REQUIRES_GOOGLE_BUILD')
-    SWIFT = get_reqs(lookup,'INSTALL_REQUIRES_SWIFT')
-
-    setup(name=NAME,
-          version=VERSION,
-          author=AUTHOR,
-          author_email=AUTHOR_EMAIL,
-          maintainer=AUTHOR,
-          maintainer_email=AUTHOR_EMAIL,
-          packages=find_packages(), 
-          include_package_data=True,
-          zip_safe=False,
-          url=PACKAGE_URL,
-          license=LICENSE,
-          description=DESCRIPTION,
-          long_description=LONG_DESCRIPTION,
-          long_description_content_type="text/markdown",
-          keywords=KEYWORDS,
-          setup_requires=["pytest-runner"],
-          install_requires = INSTALL_REQUIRES,
-          tests_require=TESTS_REQUIRES,
-          extras_require={
-              'all-basic': [INSTALL_BASIC_ALL],
-              'aws-basic': [AWS_BASIC],
-              'dropbox-basic': [DROPBOX_BASIC],
-              'google-compute-basic': [GOOGLE_COMPUTE_BASIC],
-              'google-storage-basic': [GOOGLE_STORAGE_BASIC],
-              'google-drive-basic': [GOOGLE_DRIVE_BASIC],
-              'google-build-basic': [GOOGLE_BUILD_BASIC],
-              'globus-basic': [GLOBUS_BASIC],
-              'registry-basic': [REGISTRY_BASIC],
-              's3-basic': [S3_BASIC],
-              'swift-basic': [SWIFT_BASIC],
-              'all': [INSTALL_REQUIRES_ALL],
-              'aws': [AWS],
-              'dropbox': [DROPBOX],
-              'google-compute': [GOOGLE_COMPUTE],
-              'google-storage': [GOOGLE_STORAGE],
-              'google-drive': [GOOGLE_DRIVE],
-              'google-build': [GOOGLE_BUILD],
-              'globus': [GLOBUS],
-              'registry': [REGISTRY],
-              's3': [S3],
-              'swift': [SWIFT]
-
-          },
-          scripts=['sregistry/main/docker/blob2oci'],
-          classifiers=[
-              'Intended Audience :: Science/Research',
-              'Intended Audience :: Developers',
-              'License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)',
-              'Programming Language :: C',
-              'Programming Language :: Python',
-              'Topic :: Software Development',
-              'Topic :: Scientific/Engineering',
-              'Operating System :: Unix',
-              'Programming Language :: Python :: 3.3',
-          ],
-          entry_points = {'console_scripts': ['sregistry=sregistry.client:main']})
+    INSTALL_REQUIRES_ALL = get_reqs(lookup, "INSTALL_REQUIRES_ALL")
+    AWS = get_reqs(lookup, "INSTALL_REQUIRES_AWS")
+    S3 = get_reqs(lookup, "INSTALL_REQUIRES_S3")
+    DROPBOX = get_reqs(lookup, "INSTALL_REQUIRES_DROPBOX")
+    REGISTRY = get_reqs(lookup, "INSTALL_REQUIRES_REGISTRY")
+    GLOBUS = get_reqs(lookup, "INSTALL_REQUIRES_GLOBUS")
+    GOOGLE_STORAGE = get_reqs(lookup, "INSTALL_REQUIRES_GOOGLE_STORAGE")
+    GOOGLE_DRIVE = get_reqs(lookup, "INSTALL_REQUIRES_GOOGLE_DRIVE")
+    GOOGLE_COMPUTE = get_reqs(lookup, "INSTALL_REQUIRES_GOOGLE_COMPUTE")
+    GOOGLE_BUILD = get_reqs(lookup, "INSTALL_REQUIRES_GOOGLE_BUILD")
+    SWIFT = get_reqs(lookup, "INSTALL_REQUIRES_SWIFT")
+
+    setup(
+        name=NAME,
+        version=VERSION,
+        author=AUTHOR,
+        author_email=AUTHOR_EMAIL,
+        maintainer=AUTHOR,
+        maintainer_email=AUTHOR_EMAIL,
+        packages=find_packages(),
+        include_package_data=True,
+        zip_safe=False,
+        url=PACKAGE_URL,
+        license=LICENSE,
+        description=DESCRIPTION,
+        long_description=LONG_DESCRIPTION,
+        long_description_content_type="text/markdown",
+        keywords=KEYWORDS,
+        setup_requires=["pytest-runner"],
+        install_requires=INSTALL_REQUIRES,
+        tests_require=TESTS_REQUIRES,
+        extras_require={
+            "all-basic": [INSTALL_BASIC_ALL],
+            "aws-basic": [AWS_BASIC],
+            "dropbox-basic": [DROPBOX_BASIC],
+            "google-compute-basic": [GOOGLE_COMPUTE_BASIC],
+            "google-storage-basic": [GOOGLE_STORAGE_BASIC],
+            "google-drive-basic": [GOOGLE_DRIVE_BASIC],
+            "google-build-basic": [GOOGLE_BUILD_BASIC],
+            "globus-basic": [GLOBUS_BASIC],
+            "registry-basic": [REGISTRY_BASIC],
+            "s3-basic": [S3_BASIC],
+            "swift-basic": [SWIFT_BASIC],
+            "all": [INSTALL_REQUIRES_ALL],
+            "aws": [AWS],
+            "dropbox": [DROPBOX],
+            "google-compute": [GOOGLE_COMPUTE],
+            "google-storage": [GOOGLE_STORAGE],
+            "google-drive": [GOOGLE_DRIVE],
+            "google-build": [GOOGLE_BUILD],
+            "globus": [GLOBUS],
+            "registry": [REGISTRY],
+            "s3": [S3],
+            "swift": [SWIFT],
+        },
+        scripts=["sregistry/main/docker/blob2oci"],
+        classifiers=[
+            "Intended Audience :: Science/Research",
+            "Intended Audience :: Developers",
+            "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
+            "Programming Language :: C",
+            "Programming Language :: Python",
+            "Topic :: Software Development",
+            "Topic :: Scientific/Engineering",
+            "Operating System :: Unix",
+            "Programming Language :: Python :: 3.3",
+        ],
+        entry_points={"console_scripts": ["sregistry=sregistry.client:main"]},
+    )
```

### Comparing `sregistry-0.2.38/sregistry/README.md` & `sregistry-0.2.39/sregistry/README.md`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/auth/secrets.py` & `sregistry-0.2.39/sregistry/auth/secrets.py`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/auth/utils.py` & `sregistry-0.2.39/sregistry/auth/utils.py`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/client/__init__.py` & `sregistry-0.2.39/sregistry/client/__init__.py`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/client/add.py` & `sregistry-0.2.39/sregistry/client/add.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 """
 
 from sregistry.logger import bot
 
 
 def main(args, parser, extra):
-
     from sregistry.main import get_client
 
     image = args.image
 
     cli = get_client(image, quiet=args.quiet)
 
     # If the client doesn't have the command, exit
```

### Comparing `sregistry-0.2.38/sregistry/client/backend.py` & `sregistry-0.2.39/sregistry/client/backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from sregistry.auth import get_secrets_file, read_client_secrets
 from sregistry.logger import bot
 from sregistry.utils import write_json
 import json
 
 
 def main(args, parser, extra):
-
     # No commands provided, print help, show clients
 
     if len(args.commands) == 0:
         usage()
         bot.exit("You must provide a valid command")
 
     # Get the chosen action
```

### Comparing `sregistry-0.2.38/sregistry/client/build.py` & `sregistry-0.2.39/sregistry/client/build.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,14 @@
     elif command == "logs":
         list_logs(args)
 
     # Option 3: The user is providing a Github repo!
     recipe = "Singularity"
 
     if "github" in command:
-
         # One argument indicates a recipe
         if len(args.commands) == 1:
             recipe = args.commands.pop(0)
 
     else:
         # If a command is provided, but not a Github repo
         bot.exit("%s is not a recognized option." % command)
```

### Comparing `sregistry-0.2.38/sregistry/client/delete.py` & `sregistry-0.2.39/sregistry/client/delete.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 """
 
 from sregistry.logger import bot
 
 
 def main(args, parser, extra):
-
     from sregistry.main import get_client
 
     image = args.image
     cli = get_client(image, quiet=args.quiet)
     cli.announce(args.command)
 
     # If the client doesn't have the command, exit
```

### Comparing `sregistry-0.2.38/sregistry/client/get.py` & `sregistry-0.2.39/sregistry/client/get.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 """
 
 from sregistry.logger import bot
 
 
 def main(args, parser, extra):
-
     from sregistry.main import get_client
 
     image = args.query
     cli = get_client(image, quiet=args.quiet)
 
     # If the client doesn't have the command, exit
     if not hasattr(cli, "get"):
```

### Comparing `sregistry-0.2.38/sregistry/client/images.py` & `sregistry-0.2.39/sregistry/client/images.py`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/client/inspect.py` & `sregistry-0.2.39/sregistry/client/inspect.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 """
 
 from sregistry.logger import bot
 
 
 def main(args, parser, extra):
-
     from sregistry.main import get_client
 
     image = args.query
 
     cli = get_client(image, quiet=args.quiet)
 
     # If the client doesn't have the command, exit
```

### Comparing `sregistry-0.2.38/sregistry/client/labels.py` & `sregistry-0.2.39/sregistry/client/labels.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 """
 
 from sregistry.logger import bot
 
 
 def main(args, parser, extra):
-
     from sregistry.main import get_client
 
     cli = get_client(quiet=args.quiet)
 
     # If the client doesn't have the command, exit
     if not hasattr(cli, "label_search"):
         msg = "label search is not implemented for %s. Why don't you add it?"
```

### Comparing `sregistry-0.2.38/sregistry/client/list.py` & `sregistry-0.2.39/sregistry/client/list.py`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/client/mv.py` & `sregistry-0.2.39/sregistry/client/mv.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 """
 
 from sregistry.logger import bot
 
 
 def main(args, parser, extra):
-
     from sregistry.main import get_client
 
     cli = get_client(quiet=args.quiet)
     cli.announce(args.command)
 
     # If the client doesn't have the command, exit
     if not hasattr(cli, "mv"):
```

### Comparing `sregistry-0.2.38/sregistry/client/pull.py` & `sregistry-0.2.39/sregistry/client/pull.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 """
 
 from sregistry.logger import bot
 
 
 def main(args, parser, extra):
-
     from sregistry.main import get_client
 
     image = args.image
     name = args.name
 
     # Customize client based on uri
     cli = get_client(image, quiet=args.quiet)
```

### Comparing `sregistry-0.2.38/sregistry/client/push.py` & `sregistry-0.2.39/sregistry/client/push.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 """
 
 from sregistry.logger import bot
 import os
 
 
 def main(args, parser, extra):
-
     from sregistry.main import get_client
 
     # Does the user have a valid image?
     image = args.image
     if not os.path.exists(image):
         bot.exit("%s does not exist" % image)
```

### Comparing `sregistry-0.2.38/sregistry/client/rename.py` & `sregistry-0.2.39/sregistry/client/rename.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 """
 
 from sregistry.logger import bot
 
 
 def main(args, parser, extra):
-
     from sregistry.main import get_client
 
     cli = get_client(debug=args.debug, quiet=args.quiet)
     cli.announce(args.command)
 
     if not hasattr(cli, "rename"):
         msg = "rename is not implemented for %s. Why don't you add it?"
```

### Comparing `sregistry-0.2.38/sregistry/client/rm.py` & `sregistry-0.2.39/sregistry/client/rm.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 """
 
 from sregistry.logger import bot
 
 
 def main(args, parser, extra):
-
     from sregistry.main import get_client
 
     image = args.image
 
     cli = get_client(image, quiet=args.quiet)
     cli.announce(args.command)
```

### Comparing `sregistry-0.2.38/sregistry/client/search.py` & `sregistry-0.2.39/sregistry/client/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 """
 
 from sregistry.logger import bot
 from sregistry.utils import remove_uri
 
 
 def main(args, parser, extra):
-
     from sregistry.main import get_client
 
     for query in args.query:
         original = query
         query = remove_uri(query)
 
         if query in ["", "*"]:
```

### Comparing `sregistry-0.2.38/sregistry/client/share.py` & `sregistry-0.2.39/sregistry/client/share.py`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/client/shell.py` & `sregistry-0.2.39/sregistry/client/shell.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 Mozilla Public License, v. 2.0. If a copy of the MPL was not distributed
 with this file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 """
 
 
 def main(args, parser, extra):
-
     lookup = {"ipython": ipython, "python": python, "bpython": bpython}
 
     shells = ["ipython", "python", "bpython"]
 
     # If the user supplies a client choice, make into a uri
     if args.endpoint is not None:
         if not args.endpoint.endswith("://"):
```

### Comparing `sregistry-0.2.38/sregistry/database/dummy.py` & `sregistry-0.2.39/sregistry/database/dummy.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     image_uri=None,
     image_name=None,
     url=None,
     metadata=None,
     save=True,
     copy=False,
 ):
-
     """dummy add simple returns an object that mimics a database entry, so the
     calling function (in push or pull) can interact with it equally. Most
     variables (other than image_path) are not used."""
 
     # We can only save if the image is provided
     if image_path is not None:
         if not os.path.exists(image_path):
```

### Comparing `sregistry-0.2.38/sregistry/database/models.py` & `sregistry-0.2.39/sregistry/database/models.py`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/database/robot.png` & `sregistry-0.2.39/sregistry/database/robot.png`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/database/sqlite.py` & `sregistry-0.2.39/sregistry/database/sqlite.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,14 @@
     """get a collection, if it exists, otherwise return None."""
     from sregistry.database.models import Collection
 
     return Collection.query.filter(Collection.name == name).first()
 
 
 def get_container(self, name, collection_id, tag="latest", version=None):
-
     """get a container, otherwise return None."""
     from sregistry.database.models import Container
 
     if not version:
         container = Container.query.filter_by(
             collection_id=collection_id, name=name, tag=tag
         ).first()
@@ -85,15 +84,14 @@
             collection_id=collection.id,
             name=names["image"],
             tag=names["tag"],
             version=names["version"],
         )
 
         if container and not quiet:
-
             # The container image file exists [local]
             if container.image:
                 print(container.image)
 
             # The container has a url (but not local file)
             elif container.url:
                 print(container.url)
@@ -163,29 +161,27 @@
     image_name: the image name (uri) to rename to.
     path: the name to rename (basename is taken)
     """
     container = self.get(image_name, quiet=True)
 
     if container:
         if container.image:
-
             # Derive a new filename and url in storage
             names = parse_image_name(remove_uri(path), version=container.version)
             storage = self._get_storage_name(names)
             dirname = os.path.dirname(storage)
 
             # This is the collection folder
             if not os.path.exists(dirname):
                 os.makedirs(dirname)
 
             container = self.cp(move_to=storage, container=container, command="rename")
 
             # On successful rename of file, update the uri
             if container is not None:
-
                 # Create the collection if doesn't exist
                 collection = self.get_or_create_collection(names["collection"])
                 self.session.commit()
 
                 # Then update the container
                 container = update_container_metadata(container, collection, names)
                 self.session.commit()
@@ -221,20 +217,18 @@
     ==========
     image_name: the parsed image name.
     path: the location to move the image to
     """
     container = self.get(image_name, quiet=True)
 
     if container is not None:
-
         image = container.image or ""
 
         # Only continue if image file exists
         if os.path.exists(image):
-
             # Default assume directory, use image name and path fully
             filename = os.path.basename(image)
             filedir = os.path.abspath(path)
 
             # If it's a file, use filename provided
             if not os.path.isdir(path):
                 filename = os.path.basename(path)
@@ -267,15 +261,14 @@
     # If a container isn't provided, look for it from image_uri
     if not container:
         container = self.get(image_name, quiet=True)
 
     image = container.image or ""
 
     if os.path.exists(image):
-
         filedir = os.path.dirname(move_to)
 
         # If the two are the same, doesn't make sense
         if move_to == image:
             bot.exit("%s is already the name." % image)
 
         # Ensure directory exists
@@ -330,15 +323,14 @@
     image_uri=None,
     image_name=None,
     url=None,
     metadata=None,
     save=True,
     copy=False,
 ):
-
     """get or create a container, including the collection to add it to.
     This function can be used from a file on the local system, or via a URL
     that has been downloaded. Either way, if one of url, version, or image_file
     is not provided, the model is created without it. If a version is not
     provided but a file path is, then the file hash is used.
 
     Parameters
@@ -391,15 +383,14 @@
             version = get_file_hash(image_path, "sha256")
         else:
             version = ""  # we can't determine a version, not in API/no file
         names = parse_image_name(remove_uri(image_uri), version=version)
 
     # If save, move to registry storage first
     if save and image_path:
-
         # If the user hasn't defined a custom name
         if image_name is None:
             image_name = self._get_storage_name(names)
         if copy:
             copyfile(image_path, image_name)
         else:
             shutil.move(image_path, image_name)
```

### Comparing `sregistry-0.2.38/sregistry/defaults.py` & `sregistry-0.2.39/sregistry/defaults.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,14 @@
 except ImportError:
     bot.warning("Database disabled. Install sqlalchemy for full functionality")
     DISABLE_DATABASE = True
 
 
 # If the user didn't disable caching or the database
 if not DISABLE_CACHE and DISABLE_DATABASE is False:
-
     # First priority goes to database path set in environment,
     # and if it's not set, default to home folder
     SREGISTRY_BASE = getenv("SREGISTRY_DATABASE", _database)
 
     # Storage defaults to a subfolder of the database, shub
     _storage = os.path.join(_database, "shub")
     SREGISTRY_STORAGE = getenv("SREGISTRY_STORAGE", _storage)
```

### Comparing `sregistry-0.2.38/sregistry/logger/message.py` & `sregistry-0.2.39/sregistry/logger/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,14 @@
         Parameters
         ==========
         iteration: current iteration (Int)
         total: total iterations (Int)
         length: character length of bar (Int)
         """
         if not self.level == QUIET:
-
             percent = 100 * (iteration / float(total))
             progress = int(length * iteration // total)
 
             if suffix is None:
                 suffix = ""
 
             if prefix is None:
```

### Comparing `sregistry-0.2.38/sregistry/logger/namer.py` & `sregistry-0.2.39/sregistry/logger/namer.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 """
 
 from random import choice
 
 
 class RobotNamer:
-
     _descriptors = [
         "chunky",
         "buttery",
         "delicious",
         "scruptious",
         "dinosaur",
         "boopy",
```

### Comparing `sregistry-0.2.38/sregistry/logger/progress.py` & `sregistry-0.2.39/sregistry/logger/progress.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,14 @@
         width=32,
         hide=None,
         empty_char=BAR_EMPTY_CHAR,
         filled_char=BAR_FILLED_CHAR,
         expected_size=None,
         every=1,
     ):
-
         self.label = label
         self.width = width
         self.hide = hide
 
         # Only show bar in terminals by default (better for piping, logging etc.)
         if hide is None:
             try:
@@ -134,25 +133,23 @@
     width=32,
     hide=None,
     empty_char=BAR_EMPTY_CHAR,
     filled_char=BAR_FILLED_CHAR,
     expected_size=None,
     every=1,
 ):
-
     """Progress iterator. Wrap your iterables with it."""
 
     count = len(it) if expected_size is None else expected_size
 
     with ProgressBar(
         label=label,
         width=width,
         hide=hide,
         empty_char=BAR_EMPTY_CHAR,
         filled_char=BAR_FILLED_CHAR,
         expected_size=count,
         every=every,
     ) as pbar:
-
         for i, item in enumerate(it):
             yield item
             pbar.show(i + 1)
```

### Comparing `sregistry-0.2.38/sregistry/logger/spinner.py` & `sregistry-0.2.39/sregistry/logger/spinner.py`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/main/README.md` & `sregistry-0.2.39/sregistry/main/README.md`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/main/__init__.py` & `sregistry-0.2.39/sregistry/main/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,14 @@
     Client.quiet = quiet
 
     # Create credentials cache, if it doesn't exist
     Client._credential_cache = get_credential_cache()
 
     # Add the database, if wanted
     if SREGISTRY_DATABASE is not None:
-
         # These are global functions used across modules
         from sregistry.database import (
             init_db,
             add,
             cp,
             get,
             mv,
```

### Comparing `sregistry-0.2.38/sregistry/main/__template__/__init__.py` & `sregistry-0.2.39/sregistry/main/__template__/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 # from .pull import pull
 # from .push import push
 # from .query import search
 
 
 class Client(ApiConnection):
     def __init__(self, secrets=None, base=None, **kwargs):
-
         # You probably want to think about where  your base is coming from!
         self.base = base
         self._update_secrets()
         self._update_headers()
         super(Client, self).__init__(**kwargs)
 
     def _update_secrets(self):
```

### Comparing `sregistry-0.2.38/sregistry/main/__template__/pull.py` & `sregistry-0.2.39/sregistry/main/__template__/pull.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,14 @@
         images = [images]
 
     bot.debug("Execution of PULL for %s images" % len(images))
 
     # If used internally we want to return a list to the user.
     finished = []
     for image in images:
-
         q = parse_image_name(remove_uri(image))
 
         # Verify image existence, and obtain id
         url = "..."  # write your custom endpoint URL here
         bot.debug("Retrieving manifest at %s" % url)
 
         # You can use the client get function to retrieve a url manifest
```

### Comparing `sregistry-0.2.38/sregistry/main/__template__/push.py` & `sregistry-0.2.39/sregistry/main/__template__/push.py`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/main/__template__/query.py` & `sregistry-0.2.39/sregistry/main/__template__/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     """
 
     # You can optionally better parse the image uri (query), but not
     # necessary
     # names = parse_image_name(remove_uri(query))
 
     if query is not None:
-
         # Here you might do a function that is a general list
         # Note that this means adding the function Client in __init__
         return self._container_query(query)
 
     # or default to listing (searching) all things.
     return self._search_all()
```

### Comparing `sregistry-0.2.38/sregistry/main/aws/__init__.py` & `sregistry-0.2.39/sregistry/main/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/main/aws/api.py` & `sregistry-0.2.39/sregistry/main/aws/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,14 @@
     tasks = []
     layers = []
 
     # Start with a fresh token
     self._update_token()
 
     for digest in digests:
-
         targz = "%s/%s.tar.gz" % (destination, digest["digest"])
         url = "%s/%s/blobs/%s" % (self.base, repo_name, digest["digest"])
 
         # Only download if not in cache already
         if not os.path.exists(targz):
             tasks.append((url, self.headers, targz))
         layers.append(targz)
```

### Comparing `sregistry-0.2.38/sregistry/main/aws/pull.py` & `sregistry-0.2.39/sregistry/main/aws/pull.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,30 +45,28 @@
 
     bot.debug("Execution of PULL for %s images" % len(images))
 
     # If used internally we want to return a list to the user.
 
     finished = []
     for image in images:
-
         q = parse_image_name(remove_uri(image), default_collection="aws")
 
         image_file = self._pull(
             file_name=file_name, save=save, force=force, names=q, kwargs=kwargs
         )
 
         finished.append(image_file)
 
     if len(finished) == 1:
         finished = finished[0]
     return finished
 
 
 def _pull(self, file_name, names, save=True, force=False, **kwargs):
-
     """pull an image from aws. This is a (less than ideal) workaround
        that actually does the following:
 
        - creates a sandbox folder
        - adds docker layers from S3
        - converts to a squashfs image with build
 
@@ -123,15 +121,14 @@
     if image_file is None:
         bot.info("Downloading with native Singularity, please wait...")
         image = file_name.replace("aws://", "docker://")
         image_file = Singularity.pull(image, pull_folder=sandbox)
 
     # Save to local storage
     if save is True:
-
         # Did we get the manifests?
         if hasattr(self, "manifest"):
             manifest = self.manifest
 
         container = self.add(
             image_path=image_file, image_uri=names["uri"], metadata=manifest, url=url
         )
```

### Comparing `sregistry-0.2.38/sregistry/main/base/__init__.py` & `sregistry-0.2.39/sregistry/main/base/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,19 +42,17 @@
 
 from sregistry.logger import bot
 from sregistry.defaults import SREGISTRY_DATABASE
 import os
 
 
 class ApiConnection(object):
-
     # Setup
 
     def __init__(self):
-
         self.headers = None
         self.base = None
         self._reset_headers()
 
         # If client initialized with _init_db, do it
         if hasattr(self, "_init_db"):
             self._init_db(SREGISTRY_DATABASE)
```

### Comparing `sregistry-0.2.38/sregistry/main/base/auth.py` & `sregistry-0.2.39/sregistry/main/base/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,21 +49,19 @@
     if has_secrets is False:
         message = "%s requires client secrets." % name
         bot.error(message)
         sys.exit(1)
 
     # Check 2: we have secrets and lookup, do we have all needed params?
     if params is not None:
-
         # Assume list so we can always parse through
         if not isinstance(params, list):
             params = [params]
 
         for param in params:
-
             # The parameter is not a key for the client
             if param not in self.secrets[name]:
                 bot.exit("Missing %s in client secrets." % param)
 
             # The parameter is a key, but empty or undefined
             elif self.secrets[name][param] in [None, ""]:
                 bot.exit("Undefined param %s in client secrets." % param)
```

### Comparing `sregistry-0.2.38/sregistry/main/base/headers.py` & `sregistry-0.2.39/sregistry/main/base/headers.py`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/main/base/http.py` & `sregistry-0.2.39/sregistry/main/base/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from sregistry.logger import bot
 import shutil
 import json
 import sys
 
 
 def delete(self, url, headers=None, return_json=True, default_headers=True):
-
     """delete request, use with caution"""
     bot.debug("DELETE %s" % url)
     return self._call(
         url,
         headers=headers,
         func=requests.delete,
         return_json=return_json,
@@ -53,29 +52,27 @@
     if status_code != 200:
         bot.error("%s, response status code %s." % (url, status_code))
         return False
     return True
 
 
 def put(self, url, headers=None, data=None, return_json=True, default_headers=True):
-
     """put request"""
     bot.debug("PUT %s" % url)
     return self._call(
         url,
         headers=headers,
         func=requests.put,
         data=data,
         return_json=return_json,
         default_headers=default_headers,
     )
 
 
 def post(self, url, headers=None, data=None, return_json=True, default_headers=True):
-
     """post will use requests to get a particular url"""
 
     bot.debug("POST %s" % url)
     return self._call(
         url,
         headers=headers,
         func=requests.post,
@@ -91,15 +88,14 @@
     headers=None,
     token=None,
     data=None,
     return_json=True,
     default_headers=True,
     quiet=False,
 ):
-
     """get will use requests to get a particular url"""
     bot.debug("GET %s" % url)
     return self._call(
         url,
         headers=headers,
         func=requests.get,
         data=data,
@@ -142,15 +138,14 @@
     if DISABLE_SSL_CHECK is True:
         bot.warning("Verify of certificates disabled! ::TESTING USE ONLY::")
 
     return not DISABLE_SSL_CHECK
 
 
 def download(self, url, file_name, headers=None, show_progress=True):
-
     """stream to a temporary file, rename on successful completion
 
     Parameters
     ==========
     file_name: the file name to stream to
     url: the url to stream from
     headers: additional headers to add
@@ -238,15 +233,14 @@
     response: a response that is ready to be iterated over to download in
               streamed chunks
     stream_to: the file to stream to
 
 
     """
     if response.status_code == 200:
-
         if show_progress is False:
             bot.quiet = True
 
         # Keep user updated with Progress Bar, if not quiet
         content_size = None
         if "Content-Length" in response.headers:
             progress = 0
@@ -282,15 +276,14 @@
     headers=None,
     return_json=True,
     stream=False,
     retry=True,
     default_headers=True,
     quiet=False,
 ):
-
     """call will issue the call, and issue a refresh token
     given a 401 response, and if the client has a _update_token function
 
     Parameters
     ==========
     func: the function (eg, post, get) to call
     url: the url to send file to
@@ -319,25 +312,22 @@
 
     # Errored response, try again with refresh
     if response.status_code in [500, 502]:
         bot.exit("Beep boop! %s: %s" % (response.reason, response.status_code))
 
     # Errored response, try again with refresh
     if response.status_code == 404:
-
         # Not found, we might want to continue on
         if quiet is False:
             bot.exit("Beep boop! %s: %s" % (response.reason, response.status_code))
 
     # Errored response, try again with refresh
     if response.status_code == 401:
-
         # If client has method to update token, try it once
         if retry is True and hasattr(self, "_update_token"):
-
             # A result of None indicates no update to the call
             self._update_token(response)
             return self._call(
                 url,
                 func,
                 data=data,
                 headers=headers,
@@ -348,16 +338,14 @@
 
         bot.exit(
             "Your credentials are expired! %s: %s"
             % (response.reason, response.status_code)
         )
 
     elif response.status_code == 200:
-
         if return_json:
-
             try:
                 response = response.json()
             except ValueError:
                 bot.exit("The server returned a malformed response.")
 
     return response
```

### Comparing `sregistry-0.2.38/sregistry/main/base/inspect.py` & `sregistry-0.2.39/sregistry/main/base/inspect.py`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/main/base/settings.py` & `sregistry-0.2.39/sregistry/main/base/settings.py`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/main/docker/__init__.py` & `sregistry-0.2.39/sregistry/main/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/main/docker/api.py` & `sregistry-0.2.39/sregistry/main/docker/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,14 @@
         self.manifests = {}
 
     # Obtain schema version 1 (metadata) and 2, and image config
     schemaVersions = ["v1", "v2", "config"]
     for schemaVersion in schemaVersions:
         manifest = self._get_manifest(repo_name, digest, schemaVersion)
         if manifest is not None:
-
             # If we don't have a config yet, try to get from version 2 manifest
             if schemaVersion == "v2" and "config" in manifest:
                 bot.debug("Attempting to get config as blob in verison 2 manifest")
                 url = self._get_layerLink(repo_name, manifest["config"]["digest"])
                 headers = {"Accept": manifest["config"]["mediaType"]}
                 self.manifests["config"] = self._get(url, headers=headers)
 
@@ -173,15 +172,14 @@
     # Create multiprocess download client
     workers = Workers()
 
     # Download each layer atomically
     tasks = []
     layers = []
     for digest in digests:
-
         targz = "%s/%s.tar.gz" % (destination, digest)
 
         # Only download if not in cache already
         if not os.path.exists(targz):
             url = "%s/%s/blobs/%s" % (self.base, repo_name, digest)
             tasks.append((url, self.headers, targz))
         layers.append(targz)
@@ -240,15 +238,14 @@
     reverseLayers = False
     schemaVersions = list(self.manifests.keys())
     schemaVersions.reverse()
     manifest = None
 
     # Select the manifest to use
     for schemaVersion in schemaVersions:
-
         manifest = self.manifests[schemaVersion]
 
         if manifest["schemaVersion"] == 1:
             reverseLayers = True
 
         # version 2 indices used by default
         layer_key = "layers"
@@ -387,15 +384,14 @@
     if not hasattr(self, "manifests"):
         bot.exit("Please retrieve manifests for an image first.")
 
     cmd = None
 
     # If we didn't find the config value in version 2
     if cmd is None and "config" in self.manifests:
-
         # First try, version 2.0 manifest config has upper level config
         manifest = self.manifests["config"]
         if "config" in manifest:
             if key in manifest["config"]:
                 cmd = manifest["config"][key]
 
         # Second try, config manifest (not from verison 2.0 schema blob)
```

### Comparing `sregistry-0.2.38/sregistry/main/docker/blob2oci` & `sregistry-0.2.39/sregistry/main/docker/blob2oci`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/main/docker/environment.tar` & `sregistry-0.2.39/sregistry/main/docker/environment.tar`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/main/docker/pull.py` & `sregistry-0.2.39/sregistry/main/docker/pull.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from sregistry.logger import bot
 from sregistry.utils import get_tmpdir, parse_image_name, remove_uri, extract_tar
 import shutil
 import os
 
 
 def pull(self, images, file_name=None, save=True, force=False, base=None, **kwargs):
-
     """pull an image from a docker hub. This is a (less than ideal) workaround
        that actually does the following:
 
        - creates a sandbox folder
        - adds docker layers, metadata folder, and custom metadata to it
        - converts to a squashfs image with build
 
@@ -47,15 +46,14 @@
         images = [images]
 
     bot.debug("Execution of PULL for %s images" % len(images))
 
     # If used internally we want to return a list to the user.
     finished = []
     for image in images:
-
         # 0. Update the base in case we aren't working with default
         base = self._update_base(image)
         q = parse_image_name(remove_uri(image), base=base)
 
         image_file = self._pull(
             file_name=file_name, save=save, force=force, names=q, kwargs=kwargs
         )
@@ -64,15 +62,14 @@
 
     if len(finished) == 1:
         finished = finished[0]
     return finished
 
 
 def _pull(self, file_name, names, save=True, force=False, uri="docker://", **kwargs):
-
     """pull an image from a docker hub. This is a (less than ideal) workaround
        that actually does the following:
 
        - creates a sandbox folder
        - adds docker layers, metadata folder, and custom metadata to it
        - converts to a squashfs image with build
 
@@ -132,15 +129,14 @@
     if image_file is None:
         bot.info("Downloading with native Singularity, please wait...")
         image = file_name.replace("docker://", uri)
         image_file = Singularity.pull(image, pull_folder=sandbox)
 
     # Save to local storage
     if save is True:
-
         # Did we get the manifests?
         manifests = {}
         if hasattr(self, "manifests"):
             manifests = self.manifests
 
         container = self.add(
             image_path=image_file, image_uri=names["uri"], metadata=manifests, url=url
```

### Comparing `sregistry-0.2.38/sregistry/main/docker/utils.py` & `sregistry-0.2.39/sregistry/main/docker/utils.py`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/main/dropbox/__init__.py` & `sregistry-0.2.39/sregistry/main/dropbox/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from .push import push
 from .query import search, search_all, container_query
 from .share import share
 
 
 class Client(ApiConnection):
     def __init__(self, secrets=None, base=None, **kwargs):
-
         # update token from the environment
         self._update_secrets()
         super(Client, self).__init__(**kwargs)
 
     def _speak(self):
         """if you want to add an extra print (of a parameter, for example)
         for the user when the client initalizes, write it here, eg:
```

### Comparing `sregistry-0.2.38/sregistry/main/dropbox/pull.py` & `sregistry-0.2.39/sregistry/main/dropbox/pull.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,14 @@
         images = [images]
 
     bot.debug("Execution of PULL for %s images" % len(images))
 
     # If used internally we want to return a list to the user.
     finished = []
     for image in images:
-
         names = parse_image_name(remove_uri(image))
 
         # Dropbox path is the path in storage with a slash
         dropbox_path = "/%s" % names["storage"]
 
         # If the user didn't provide a file, make one based on the names
         if file_name is None:
@@ -56,15 +55,14 @@
 
         # If the file already exists and force is False
         if os.path.exists(file_name) and force is False:
             bot.exit("Image exists! Remove first, or use --force to overwrite")
 
         # First ensure that exists
         if self.exists(dropbox_path) is True:
-
             # _stream is a function to stream using the response to start
             metadata, response = self.dbx.files_download(dropbox_path)
             image_file = self._stream(response, stream_to=file_name)
 
             # parse the metadata (and add inspected image)
             metadata = self._get_metadata(image_file, metadata)
```

### Comparing `sregistry-0.2.38/sregistry/main/dropbox/push.py` & `sregistry-0.2.39/sregistry/main/dropbox/push.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,23 +54,21 @@
     # If image is smaller than 150MB, use standard upload
     with open(path, "rb") as F:
         if file_size <= chunk_size:
             self.dbx.files_upload(F.read(), storage_path)
 
         # otherwise upload in chunks
         else:
-
             start = self.dbx.files_upload_session_start(F.read(chunk_size))
             cursor = dropbox.files.UploadSessionCursor(
                 session_id=start.session_id, offset=F.tell()
             )
             commit = dropbox.files.CommitInfo(path=storage_path)
 
             while F.tell() < file_size:
-
                 progress += chunk_size
 
                 # Finishing up the file, less than chunk_size to go
                 if file_size - F.tell() <= chunk_size:
                     self.dbx.files_upload_session_finish(
                         F.read(chunk_size), cursor, commit
                     )
```

### Comparing `sregistry-0.2.38/sregistry/main/dropbox/query.py` & `sregistry-0.2.39/sregistry/main/dropbox/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 def search(self, query=None, args=None):
     """query a Singularity registry for a list of images.
     If query is None, collections are listed.
 
     """
 
     if query is not None:
-
         # Here you might do a function that is a general list
         # Note that this means adding the function Client in __init__
         return self._container_query(query)
 
     # or default to listing (searching) all things.
     return self._search_all()
 
@@ -32,15 +31,14 @@
 def search_all(self):
     """a "show all" search that doesn't require a query"""
 
     results = []
 
     # Parse through folders (collections):
     for entry in self.dbx.files_list_folder("").entries:
-
         # Parse through containers
         for item in self.dbx.files_list_folder(entry.path_lower).entries:
             name = item.name.replace(".simg", "")
             results.append(["%s/%s" % (entry.name, name)])
 
     if len(results) == 0:
         bot.info("No container collections found.")
@@ -59,15 +57,14 @@
 
     results = []
 
     query = remove_uri(query)
 
     # Parse through folders (collections):
     for entry in self.dbx.files_list_folder("").entries:
-
         # Parse through containers
         for item in self.dbx.files_list_folder(entry.path_lower).entries:
             name = item.name.replace(".simg", "")
             name = "%s/%s" % (entry.name, name)
             if query in name:
                 results.append([name])
```

### Comparing `sregistry-0.2.38/sregistry/main/dropbox/share.py` & `sregistry-0.2.39/sregistry/main/dropbox/share.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
     names = parse_image_name(remove_uri(query))
 
     # Dropbox path is the path in storage with a slash
     dropbox_path = "/%s" % names["storage"]
 
     # First ensure that exists
     if self.exists(dropbox_path) is True:
-
         # Create new shared link
         try:
             share = self.dbx.sharing_create_shared_link_with_settings(dropbox_path)
 
         # Already exists!
         except:
             share = self.dbx.sharing_create_shared_link(dropbox_path)
```

### Comparing `sregistry-0.2.38/sregistry/main/gitlab/__init__.py` & `sregistry-0.2.39/sregistry/main/gitlab/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 from .pull import pull
 from .query import search, search_all
 
 
 class Client(ApiConnection):
     def __init__(self, secrets=None, base=None, **kwargs):
-
         super(Client, self).__init__(**kwargs)
         self._reset_headers()
         self._update_secrets()
         self._update_base()
 
     def _update_base(self):
         """update the base, including the URL for GitLab and the API endpoint."""
```

### Comparing `sregistry-0.2.38/sregistry/main/gitlab/pull.py` & `sregistry-0.2.39/sregistry/main/gitlab/pull.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,14 @@
         images = [images]
 
     bot.debug("Execution of PULL for %s images" % len(images))
 
     # If used internally we want to return a list to the user.
     finished = []
     for image in images:
-
         # Format job_id|collection|job_name
         # 122056733,singularityhub/gitlab-ci'
         # 122056733,singularityhub/gitlab-ci,build
 
         job_id, collection, job_name = self._parse_image_name(image)
         names = parse_image_name(remove_uri(collection))
```

### Comparing `sregistry-0.2.38/sregistry/main/gitlab/query.py` & `sregistry-0.2.39/sregistry/main/gitlab/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,22 +42,20 @@
     if response.status_code == 200:
         jobs = response.json()
 
         # We can't get a listing of artifacts
         # https://gitlab.com/gitlab-org/gitlab-ce/issues/51515
         # Parse through jobs (each can have different tags for a collection):
         for job in jobs:
-
             # Only show jobs that are successful
             if job["status"] == "success":
                 name = job["name"]
 
                 for artifact in job["artifacts"]:
                     if artifact["filename"].endswith("zip"):
-
                         # The user must browse to see the names
                         artifact_url = "%s/%s/-/jobs/%s/artifacts/browse/%s" % (
                             self.base,
                             collection,
                             job["id"],
                             name,
                         )
```

### Comparing `sregistry-0.2.38/sregistry/main/globus/__init__.py` & `sregistry-0.2.39/sregistry/main/globus/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,19 +32,17 @@
 from .query import search, list_endpoint, list_endpoints
 
 if sys.version_info[0] == 3:
     raw_input = input
 
 
 class Client(ApiConnection):
-
     # Initialization Calls
 
     def __init__(self, secrets=None, base=None, **kwargs):
-
         # These are unlikely to change
 
         self._client_id = "ae32247c-2c17-4c43-92b5-ba7fe9957dbb"
         self._redirect_url = "https://auth.globus.org/v2/web/auth-code"
         self._init_clients()
 
         super(Client, self).__init__(**kwargs)
```

### Comparing `sregistry-0.2.38/sregistry/main/globus/pull.py` & `sregistry-0.2.39/sregistry/main/globus/pull.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,14 @@
     if not isinstance(images, list):
         images = [images]
 
     bot.debug("Execution of PULL for %s images" % len(images))
 
     finished = []
     for image in images:
-
         # Split the name into endpoint and rest
 
         endpoint, remote = self._parse_endpoint_name(image)
         source = self.transfer_client.get_endpoint(endpoint)
 
         name = os.path.basename(remote)
         q = parse_image_name(name, default_collection=source["name"])
```

### Comparing `sregistry-0.2.38/sregistry/main/globus/push.py` & `sregistry-0.2.39/sregistry/main/globus/push.py`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/main/globus/query.py` & `sregistry-0.2.39/sregistry/main/globus/query.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,14 @@
     If no endpoint is provided but instead just a query, we use the query
     to search endpoints.
 
     """
 
     # No query is defined
     if query is None:
-
         # Option 1: No query or endpoints lists all shared and personal
         if args.endpoint is None:
             bot.info("Listing shared endpoints. Add query to expand search.")
             return self._list_endpoints()
 
         # Option 2: An endpoint without query will just list containers there
         else:
@@ -97,23 +96,21 @@
 
     endpoint, path = self._parse_endpoint_name(endpoint)
 
     # Get a list of files at endpoint, under specific path
     try:
         result = self.transfer_client.operation_ls(endpoint, path=path)
     except Exception as err:
-
         # Tell the user what went wrong!
         bot.custom(prefix="ERROR", message=err, color="RED")
         sys.exit(1)
 
     rows = []
 
     for filey in result:
-
         # Highlight container contenders with purple
         name = filey["name"]
         if query is None or query in name:
             if name.endswith("img"):
                 name = bot.addColor("PURPLE", name)
 
             rows.append([filey["type"], filey["permissions"], str(filey["size"]), name])
```

### Comparing `sregistry-0.2.38/sregistry/main/globus/utils.py` & `sregistry-0.2.39/sregistry/main/globus/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     else:
         path = "/".join(parts[1:])
 
     return endpoint, path
 
 
 def create_endpoint_cache(self, endpoint_id, cache=".singularity/shub"):
-
     """create a directory for sregistry in the user's
     base folder to share images.
 
     Parameters
     ==========
     endpoint_id: the endpoint id parameters
     cache: the relative path for the images cache folder at the
```

### Comparing `sregistry-0.2.38/sregistry/main/google_build/README.md` & `sregistry-0.2.39/sregistry/main/google_build/README.md`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/main/google_build/__init__.py` & `sregistry-0.2.39/sregistry/main/google_build/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,20 +33,18 @@
 from .logs import logs, list_logs, print_log
 from .pull import pull
 from .push import push, upload
 from .query import container_query, list_containers, search, search_all
 
 
 class Client(ApiConnection):
-
     # Custom variables that can be provided with client.get_client
     envars = {}
 
     def __init__(self, secrets=None, base=None, init=True, **kwargs):
-
         self._update_secrets()
         self._update_headers()
 
         # Do we need storage client now?
         if init is True:
             self._init_client()
```

### Comparing `sregistry-0.2.38/sregistry/main/google_build/build.py` & `sregistry-0.2.39/sregistry/main/google_build/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,14 @@
 
     """
     bot.debug("BUILD %s" % recipe)
 
     build_package = [recipe]
 
     if context:
-
         # If the user gives a ., include recursive $PWD
         if "." in context:
             context = glob(os.getcwd() + "/**/*", recursive=True)
         build_package = build_package + context
 
     # We need to get and save relative paths for the config.
     package = create_build_package(build_package, working_dir)
@@ -289,15 +288,14 @@
     bot.log("Generating build package for %s files..." % len(package_files))
     build_dir = get_tmpdir(prefix="sregistry-build")
     build_tar = "%s/build.tar.gz" % build_dir
     tar = tarfile.open(build_tar, "w:gz")
 
     # Create the tar.gz, making sure relative to working_dir
     for package_file in package_files:
-
         # Get a relative path
         relative_path = get_relative_path(package_file, working_dir)
         tar.add(package_file, arcname=relative_path)
     tar.close()
 
     # Get hash (sha256), and rename file
     sha256 = get_file_hash(build_tar)
@@ -333,15 +331,14 @@
     the present working directory. Optionally, the user can provide
     extra_data to post back with the build_id.
     """
     data = {"id": "$BUILD_ID"}
     substitutions = {}
 
     if extra_data is not None:
-
         # Keep a list of envars to add
         for key, val in extra_data.items():
             sub = "_SREGISTRY_%s" % key.upper()
             data[key] = "${%s}" % sub
             substitutions[sub] = val
 
     config["steps"].append(
@@ -497,15 +494,14 @@
     status = response["status"]
     bot.log("build %s: %s" % (build_id, status))
 
     return response
 
 
 def finish_build(self, build_id, config=None, response=None):
-
     """finish a build, meaning if the build was successful, we check the
     user preference to make it private. If it's set, we leave it
     private. Otherwise, we make it public (default).
 
     Parameters
     ==========
     build_id: the build id returned from submission to track the build.
@@ -514,15 +510,14 @@
     """
     # Get the build status, we will only complete on SUCCESS
     if not response:
         response = self._build_status(build_id)
 
     # If successful, update blob metadata and visibility
     if response["status"] == "SUCCESS":
-
         # Does the user want to keep the container private?
         env = "SREGISTRY_GOOGLE_STORAGE_PRIVATE"
         blob_location = get_blob_location(response, self._bucket_name)
         blob = self._bucket.get_blob(blob_location)
 
         # Make Public, if desired
         if not self._get_and_update_setting(env, self.envars.get(env)):
```

### Comparing `sregistry-0.2.38/sregistry/main/google_build/client.py` & `sregistry-0.2.39/sregistry/main/google_build/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     Client.envars = kwargs
 
     # Create credentials cache, if it doesn't exist
     Client._credential_cache = get_credential_cache()
 
     # Add the database, if wanted
     if SREGISTRY_DATABASE is not None:
-
         # These are global functions used across modules
         from sregistry.database import (
             init_db,
             add,
             cp,
             get,
             mv,
```

### Comparing `sregistry-0.2.38/sregistry/main/google_build/delete.py` & `sregistry-0.2.39/sregistry/main/google_build/delete.py`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/main/google_build/logs.py` & `sregistry-0.2.39/sregistry/main/google_build/logs.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     content = None
     results = self._list_logs()
     print(results)
 
     # If we are searching for a name
     if name is not None:
         for result in results:
-
             matches = False
 
             # Case 1: the name is in the storage path
             if name in result.name:
                 matches = True
 
             # Case 2: match in metadata
@@ -42,15 +41,14 @@
                     matches = True
 
             if matches is True:
                 content = self._print_log(result.name)
 
     # Otherwise return the last
     else:
-
         if len(results) > 0:
             latest = results[0]
 
             # Get the most recent
             for result in results:
                 if result.time_created >= latest.time_created:
                     latest = result
```

### Comparing `sregistry-0.2.38/sregistry/main/google_build/pull.py` & `sregistry-0.2.39/sregistry/main/google_build/pull.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,14 @@
         images = [images]
 
     bot.debug("Execution of PULL for %s images" % len(images))
 
     # If used internally we want to return a list to the user.
     finished = []
     for image in images:
-
         q = parse_image_name(remove_uri(image))
 
         # Use container search to find the container based on uri
         bot.info("Searching for %s in gs://%s" % (q["uri"], self._bucket_name))
         matches = self._container_query(q["uri"], quiet=True)
 
         if len(matches) == 0:
```

### Comparing `sregistry-0.2.38/sregistry/main/google_build/push.py` & `sregistry-0.2.39/sregistry/main/google_storage/push.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 from retrying import retry
 import os
 
 
 def push(self, path, name, tag=None):
     """push an image to Google Cloud Storage, meaning uploading it
 
+    Parameters
+    ==========
     path: should correspond to an absolte image path (or derive it)
     name: should be the complete uri that the user has requested to push.
     tag: should correspond with an image tag. This is provided to mirror Docker
     """
     path = os.path.abspath(path)
     bot.debug("PUSH %s" % path)
 
@@ -43,24 +45,15 @@
         source=path, destination=names["storage"], metadata=metadata
     )
 
     print(manifest["mediaLink"])
 
 
 @retry(wait_exponential_multiplier=1000, wait_exponential_max=10000)
-def upload(
-    self,
-    source,
-    destination,
-    bucket,
-    chunk_size=2 * 1024 * 1024,
-    metadata=None,
-    keep_private=True,
-):
-
+def upload(self, source, destination, chunk_size=2 * 1024 * 1024, metadata=None):
     """upload a file from a source to a destination. The client is expected
     to have a bucket (self._bucket) that is created when instantiated.
 
     This would be the method to do the same using the storage client,
     but not easily done for resumable
 
     blob = self._bucket.blob(destination)
@@ -71,35 +64,34 @@
     url = blob.public_url
     if isinstance(url, six.binary_type):
         url = url.decode('utf-8')
 
     return url
     """
     env = "SREGISTRY_GOOGLE_STORAGE_PRIVATE"
-    keep_private = self._get_and_update_setting(env) or keep_private
+    keep_private = self._get_and_update_setting(env)
 
     media = MediaFileUpload(source, chunksize=chunk_size, resumable=True)
     request = self._storage_service.objects().insert(
-        bucket=bucket.name, name=destination, media_body=media
+        bucket=self._bucket_name, name=destination, media_body=media
     )
 
     response = None
     total = request.resumable._size / (1024 * 1024.0)
 
     bar = ProgressBar(expected_size=total, filled_char="=", hide=self.quiet)
 
     while response is None:
         progress, response = request.next_chunk()
         if progress:
             bar.show(progress.resumable_progress / (1024 * 1024.0))
 
     # When we finish upload, get as blob
-    blob = bucket.blob(destination)
+    blob = self._bucket.blob(destination)
     if blob.exists():
-
         if not keep_private:
             blob.make_public()
 
         # If the user has a dictionary of metadata to update
         if metadata is not None:
             blob.metadata = metadata
             blob._properties["metadata"] = metadata
```

### Comparing `sregistry-0.2.38/sregistry/main/google_build/query.py` & `sregistry-0.2.39/sregistry/main/google_build/query.py`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/main/google_build/utils.py` & `sregistry-0.2.39/sregistry/main/google_build/utils.py`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/main/google_drive/__init__.py` & `sregistry-0.2.39/sregistry/main/google_drive/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 from .push import push
 from .share import share
 from .query import container_query, list_containers, search, search_all
 
 
 class Client(ApiConnection):
     def __init__(self, secrets=None, base=None, **kwargs):
-
         self._update_secrets()
         self._update_headers()
         self._init_client()
         super(Client, self).__init__(**kwargs)
 
     def _speak(self):
         """add the bucket name to be printed to the user at appropriate times"""
```

### Comparing `sregistry-0.2.38/sregistry/main/google_drive/pull.py` & `sregistry-0.2.39/sregistry/main/google_drive/pull.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
         images = [images]
 
     bot.debug("Execution of PULL for %s images" % len(images))
 
     # If used internally we want to return a list to the user.
     finished = []
     for image in images:
-
         q = parse_image_name(remove_uri(image))
 
         # Use container search to find the container based on uri
         bot.info("Searching for %s in drive://%s" % (q["uri"], self._base))
         matches = self._container_query(q["uri"], quiet=True)
 
         if len(matches) == 0:
```

### Comparing `sregistry-0.2.38/sregistry/main/google_drive/push.py` & `sregistry-0.2.39/sregistry/main/google_drive/push.py`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/main/google_drive/query.py` & `sregistry-0.2.39/sregistry/main/google_drive/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,14 @@
     results = self._list_containers()
     matches = []
 
     bot.info("[drive://%s] Containers" % self._base)
 
     rows = []
     for i in results:
-
         # Fallback to the image name without the extension
         uri = i["name"].replace(".simg", "")
 
         # However the properties should include the uri
         if "properties" in i:
             if "uri" in i["properties"]:
                 uri = i["properties"]["uri"]
@@ -111,15 +110,14 @@
     results, filters them down based on user criteria (the query)
     """
 
     results = self._list_containers()
 
     matches = []
     for result in results:
-
         is_match = False
         if query in result["id"]:
             is_match = True
 
         elif query in result["name"]:
             is_match = True
 
@@ -131,15 +129,14 @@
 
         if is_match is True:
             matches.append(result)
 
     if not quiet:
         bot.info("[drive://%s] Found %s containers" % (self._base, len(matches)))
         for image in matches:
-
             # If the image has properties, show to the user
             if "properties" in image:
                 image.update(image["properties"])
 
             bot.info(image["uri"])
 
             for key in sorted(image, key=len):
```

### Comparing `sregistry-0.2.38/sregistry/main/google_drive/share.py` & `sregistry-0.2.39/sregistry/main/google_drive/share.py`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/main/google_drive/utils.py` & `sregistry-0.2.39/sregistry/main/google_drive/utils.py`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/main/google_storage/__init__.py` & `sregistry-0.2.39/sregistry/main/google_storage/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 from .pull import pull
 from .push import push, upload
 from .query import container_query, list_containers, search, search_all
 
 
 class Client(ApiConnection):
     def __init__(self, secrets=None, base=None, init=True, **kwargs):
-
         self._update_secrets()
         self._update_headers()
 
         # Do we need storage/compute client now?
         if init is True:
             self._init_client()
```

### Comparing `sregistry-0.2.38/sregistry/main/google_storage/build.py` & `sregistry-0.2.39/sregistry/main/google_storage/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,14 @@
     config=None,
     name=None,
     commit=None,
     tag="latest",
     recipe="Singularity",
     preview=False,
 ):
-
     """trigger a build on Google Cloud (storage then compute) given a name
     recipe, and Github URI where the recipe can be found.
 
     Parameters
     ==========
     name: should be the complete uri that the user has requested to push.
     commit: a commit to use, not required, and can be parsed from URI
@@ -197,25 +196,22 @@
     retries: the number of retries before giving up
     delay: the delay between retry
 
     Note from @vsoch: this function is pretty nasty.
 
     """
     for _ in range(retries):
-
         # Retrieve list of instances
         instances = self._get_instances()
 
         for instance in instances["items"]:
             if instance["name"] == name:
-
                 # Iterate through network interfaces
                 for network in instance["networkInterfaces"]:
                     if network["name"] == "nic0":
-
                         # Access configurations
                         for subnet in network["accessConfigs"]:
                             if subnet["name"] == "External NAT":
                                 if "natIP" in subnet:
                                     return subnet["natIP"]
 
         sleep(delay)
@@ -267,15 +263,14 @@
     repo,
     config,
     tag=None,
     commit=None,
     recipe="Singularity",
     startup_script=None,
 ):
-
     """setup the build based on the selected configuration file, meaning
     producing the configuration file filled in based on the user's input
 
     Parameters
     ==========
     config: the complete configuration file provided by the client
     template: an optional custom start script to use
@@ -415,15 +410,14 @@
     )
 
     # Update metadata config object
 
     seen = ["SREGISTRY_BUILDER_STORAGE_BUCKET", "startup-script"]
 
     for key, value in defaults.items():
-
         # This also appends empty values, they are meaningful
         if value not in seen:
             entry = {"key": key, "value": value}
             metadata["items"].append(entry)
             seen.append(key)
 
     config["metadata"] = metadata
```

### Comparing `sregistry-0.2.38/sregistry/main/google_storage/delete.py` & `sregistry-0.2.39/sregistry/main/google_storage/delete.py`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/main/google_storage/logs.py` & `sregistry-0.2.39/sregistry/main/google_storage/logs.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     content = None
     results = self._list_logs()
     print(results)
 
     # If we are searching for a name
     if name is not None:
         for result in results:
-
             matches = False
 
             # Case 1: the name is in the storage path
             if name in result.name:
                 matches = True
 
             # Case 2: match in metadata
@@ -42,15 +41,14 @@
                     matches = True
 
             if matches is True:
                 content = self._print_log(result.name)
 
     # Otherwise return the last
     else:
-
         if len(results) > 0:
             latest = results[0]
 
             # Get the most recent
             for result in results:
                 if result.time_created >= latest.time_created:
                     latest = result
```

### Comparing `sregistry-0.2.38/sregistry/main/google_storage/pull.py` & `sregistry-0.2.39/sregistry/main/google_storage/pull.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,14 @@
         images = [images]
 
     bot.debug("Execution of PULL for %s images" % len(images))
 
     # If used internally we want to return a list to the user.
     finished = []
     for image in images:
-
         q = parse_image_name(remove_uri(image))
 
         # Use container search to find the container based on uri
         bot.info("Searching for %s in gs://%s" % (q["uri"], self._bucket_name))
         matches = self._container_query(q["uri"], quiet=True)
 
         if len(matches) == 0:
```

### Comparing `sregistry-0.2.38/sregistry/main/google_storage/push.py` & `sregistry-0.2.39/sregistry/main/google_build/push.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,16 +15,14 @@
 from retrying import retry
 import os
 
 
 def push(self, path, name, tag=None):
     """push an image to Google Cloud Storage, meaning uploading it
 
-    Parameters
-    ==========
     path: should correspond to an absolte image path (or derive it)
     name: should be the complete uri that the user has requested to push.
     tag: should correspond with an image tag. This is provided to mirror Docker
     """
     path = os.path.abspath(path)
     bot.debug("PUSH %s" % path)
 
@@ -45,15 +43,23 @@
         source=path, destination=names["storage"], metadata=metadata
     )
 
     print(manifest["mediaLink"])
 
 
 @retry(wait_exponential_multiplier=1000, wait_exponential_max=10000)
-def upload(self, source, destination, chunk_size=2 * 1024 * 1024, metadata=None):
+def upload(
+    self,
+    source,
+    destination,
+    bucket,
+    chunk_size=2 * 1024 * 1024,
+    metadata=None,
+    keep_private=True,
+):
     """upload a file from a source to a destination. The client is expected
     to have a bucket (self._bucket) that is created when instantiated.
 
     This would be the method to do the same using the storage client,
     but not easily done for resumable
 
     blob = self._bucket.blob(destination)
@@ -64,35 +70,34 @@
     url = blob.public_url
     if isinstance(url, six.binary_type):
         url = url.decode('utf-8')
 
     return url
     """
     env = "SREGISTRY_GOOGLE_STORAGE_PRIVATE"
-    keep_private = self._get_and_update_setting(env)
+    keep_private = self._get_and_update_setting(env) or keep_private
 
     media = MediaFileUpload(source, chunksize=chunk_size, resumable=True)
     request = self._storage_service.objects().insert(
-        bucket=self._bucket_name, name=destination, media_body=media
+        bucket=bucket.name, name=destination, media_body=media
     )
 
     response = None
     total = request.resumable._size / (1024 * 1024.0)
 
     bar = ProgressBar(expected_size=total, filled_char="=", hide=self.quiet)
 
     while response is None:
         progress, response = request.next_chunk()
         if progress:
             bar.show(progress.resumable_progress / (1024 * 1024.0))
 
     # When we finish upload, get as blob
-    blob = self._bucket.blob(destination)
+    blob = bucket.blob(destination)
     if blob.exists():
-
         if not keep_private:
             blob.make_public()
 
         # If the user has a dictionary of metadata to update
         if metadata is not None:
             blob.metadata = metadata
             blob._properties["metadata"] = metadata
```

### Comparing `sregistry-0.2.38/sregistry/main/google_storage/query.py` & `sregistry-0.2.39/sregistry/main/google_storage/query.py`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/main/google_storage/utils.py` & `sregistry-0.2.39/sregistry/main/google_storage/utils.py`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/main/hub/__init__.py` & `sregistry-0.2.39/sregistry/main/hub/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 from .pull import pull
 from .query import search, list_all, search_collection
 
 
 class Client(ApiConnection):
     def __init__(self, secrets=None, **kwargs):
-
         self._update_headers()
         super(Client, self).__init__(**kwargs)
         self.base = "https://www.singularity-hub.org/api"
 
 
 Client.pull = pull
 Client.search = search
```

### Comparing `sregistry-0.2.38/sregistry/main/hub/pull.py` & `sregistry-0.2.39/sregistry/main/hub/pull.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,14 @@
     if not isinstance(images, list):
         images = [images]
 
     bot.debug("Execution of PULL for %s images" % len(images))
 
     finished = []
     for image in images:
-
         q = parse_image_name(remove_uri(image), lowercase=False)
 
         # Verify image existence, and obtain id
         url = "%s/container/%s/%s:%s" % (
             self.base,
             q["collection"],
             q["image"],
```

### Comparing `sregistry-0.2.38/sregistry/main/hub/query.py` & `sregistry-0.2.39/sregistry/main/hub/query.py`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/main/nvidia/__init__.py` & `sregistry-0.2.39/sregistry/main/nvidia/__init__.py`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/main/nvidia/pull.py` & `sregistry-0.2.39/sregistry/main/nvidia/pull.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,15 +42,14 @@
 
     bot.debug("Execution of PULL for %s images" % len(images))
 
     # If used internally we want to return a list to the user.
 
     finished = []
     for image in images:
-
         q = parse_image_name(remove_uri(image), default_collection="nvidia")
 
         image_file = self._pull(
             file_name=file_name,
             uri="nvidia://",
             save=save,
             force=force,
```

### Comparing `sregistry-0.2.38/sregistry/main/registry/__init__.py` & `sregistry-0.2.39/sregistry/main/registry/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 from .push import push
 from .delete import delete
 from .query import search, search_all, collection_search, label_search, container_search
 
 
 class Client(ApiConnection):
     def __init__(self, secrets=None, base=None, **kwargs):
-
         self.base = base
         super(Client, self).__init__(**kwargs)
         self._update_secrets()
         self._update_headers()
 
     def _update_base(self):
         if self.base is not None:
@@ -53,24 +52,22 @@
         Parameters
         ==========
         q: the parsed image query (names), including the original
         """
 
         # If image uses http or https, add back
         if not q["registry"].startswith("http"):
-
             if q["original"].startswith("http:"):
                 q["registry"] = "http://%s" % q["registry"]
 
             elif q["original"].startswith("https:"):
                 q["registry"] = "https://%s" % q["registry"]
 
             # Otherwise, guess from the user's environment
             else:
-
                 prefix = "https://"
 
                 # The user can set an environment variable to specify nohttps
                 nohttps = os.environ.get("SREGISTRY_REGISTRY_NOHTTPS")
                 if nohttps is not None:
                     prefix = "http://"
                 q["registry"] = "%s%s" % (prefix, q["registry"])
```

### Comparing `sregistry-0.2.38/sregistry/main/registry/auth.py` & `sregistry-0.2.39/sregistry/main/registry/auth.py`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/main/registry/build.py` & `sregistry-0.2.39/sregistry/main/registry/build.py`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/main/registry/delete.py` & `sregistry-0.2.39/sregistry/main/registry/delete.py`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/main/registry/pull.py` & `sregistry-0.2.39/sregistry/main/registry/pull.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,14 @@
     if not isinstance(images, list):
         images = [images]
 
     bot.debug("Execution of PULL for %s images" % len(images))
 
     finished = []
     for image in images:
-
         q = parse_image_name(remove_uri(image))
 
         # If a custom registry is not set, use default base
         if q["registry"] is None:
             q["registry"] = self.base
 
         # If the registry is still None, no go
@@ -73,18 +72,16 @@
         try:
             manifest = self._get(url)
         except SSLError:
             bot.exit("Issue with %s, try exporting SREGISTRY_REGISTRY_NOHTTPS." % url)
 
         # Private container collection
         if isinstance(manifest, Response):
-
             # Requires token
             if manifest.status_code in [403, 401]:
-
                 SREGISTRY_EVENT = self.authorize(request_type="pull", names=q)
                 headers = {"Authorization": SREGISTRY_EVENT}
                 self._update_headers(headers)
                 manifest = self._get(url)
 
                 # Still denied
                 if isinstance(manifest, Response):
@@ -97,15 +94,14 @@
             elif manifest == 404:
                 bot.exit("Container not found (404)")
             elif manifest == 403:
                 bot.exit("Unauthorized (403)")
 
         # Successful pull
         if "image" in manifest:
-
             # Add self link to manifest
             manifest["selfLink"] = url
 
             if file_name is None:
                 file_name = q["storage"].replace("/", "-")
 
             # Clear headers of previous token
```

### Comparing `sregistry-0.2.38/sregistry/main/registry/push.py` & `sregistry-0.2.39/sregistry/main/registry/push.py`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/main/registry/query.py` & `sregistry-0.2.39/sregistry/main/registry/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,14 @@
     vsoch/dinosaur      list details of container vsoch/dinosaur
                           tag "latest" is used by default, and then the most recent
     vsoch/dinosaur:tag  list details for specific container
 
     """
 
     if query is not None:
-
         # List all containers in collection query/
         if query.endswith("/"):  # collection search
             return self._collection_search(query)
 
         # List containers across collections called /query
         elif query.startswith("/"):
             return self._container_search(query, across_collections=True)
@@ -191,12 +190,11 @@
         bot.info("No containers found.")
         sys.exit(1)
 
     bot.info("Containers %s" % query)
 
     rows = []
     for c in result:
-
         rows.append(["%s/%s" % (c["collection"], c["name"]), c["tag"]])
 
     bot.table(rows)
     return rows
```

### Comparing `sregistry-0.2.38/sregistry/main/registry/utils.py` & `sregistry-0.2.39/sregistry/main/registry/utils.py`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/main/s3/__init__.py` & `sregistry-0.2.39/sregistry/main/s3/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 from .pull import pull
 from .push import push
 from .delete import delete
 
 
 class Client(ApiConnection):
     def __init__(self, secrets=None, base=None, **kwargs):
-
         self.base = base
         self._update_secrets()
         self._update_headers()
         super(Client, self).__init__(**kwargs)
 
     def _speak(self):
         """add the bucket"""
```

### Comparing `sregistry-0.2.38/sregistry/main/s3/delete.py` & `sregistry-0.2.39/sregistry/main/s3/delete.py`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/main/s3/pull.py` & `sregistry-0.2.39/sregistry/main/s3/pull.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,14 @@
     if not isinstance(images, list):
         images = [images]
 
     bot.debug("Execution of PULL for %s images" % len(images))
 
     finished = []
     for image in images:
-
         image = remove_uri(image)
         names = parse_image_name(image)
 
         if file_name is None:
             file_name = names["storage"].replace("/", "-")
 
         # Assume the user provided the correct uri to start
@@ -54,15 +53,14 @@
         # First try to get the storage uri directly.
         try:
             self.bucket.download_file(uri, file_name)
 
         # If we can't find the file, help the user
         except botocore.exceptions.ClientError as e:
             if e.response["Error"]["Code"] == "404":
-
                 # Case 1, image not found, but not error with API
                 bot.error("Cannot find %s!" % file_name)
 
                 # Try to help the user with suggestions
                 results = self._search_all()
                 if len(results) > 0:
                     bot.info("Did you mean:\n" % "\n".join(results))
```

### Comparing `sregistry-0.2.38/sregistry/main/s3/push.py` & `sregistry-0.2.39/sregistry/main/s3/push.py`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/main/s3/query.py` & `sregistry-0.2.39/sregistry/main/s3/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,14 @@
     is returned. If across_collections is True, the container is searched
     for across collections. If across collections is True, details are
     not shown"""
 
     results = self._search_all(quiet=True)
     matches = []
     for result in results:
-
         # This is the container name
         if query in result[0]:
             matches.append(result)
 
     if len(matches) > 0:
         bot.info("Containers %s" % query)
         bot.table(matches)
```

### Comparing `sregistry-0.2.38/sregistry/main/swift/__init__.py` & `sregistry-0.2.39/sregistry/main/swift/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from .pull import pull
 from .push import push
 from .query import search, search_all, container_query
 
 
 class Client(ApiConnection):
     def __init__(self, secrets=None, base=None, **kwargs):
-
         self.config = dict()
         self._update_secrets()
         self.name = self.config.get("SREGISTRY_SWIFT_URL", "Swift Client Storage")
         super(Client, self).__init__(**kwargs)
 
     def _speak(self):
         """if you want to add an extra print (of a parameter, for example)
@@ -73,29 +72,27 @@
         # will need to collect for proper authentication
         self.config["SREGISTRY_SWIFT_AUTHTYPE"] = self._required_get_and_update(
             "SREGISTRY_SWIFT_AUTHTYPE"
         )
 
         # Check what auth version is requested and setup the connection
         if self.config["SREGISTRY_SWIFT_AUTHTYPE"] == "preauth":
-
             # Pre-Authenticated Token/URL - Use OS_AUTH_TOKEN/OS_STORAGE_URL
             # Retrieve the user token, user, and base. Exit if not found
             for envar in [
                 "SREGISTRY_SWIFT_OS_AUTH_TOKEN",
                 "SREGISTRY_SWIFT_OS_STORAGE_URL",
             ]:
                 self.config[envar] = self._required_get_and_update(envar)
 
             self.conn = swiftclient.Connection(
                 preauthurl=self.config["SREGISTRY_SWIFT_OS_STORAGE_URL"],
                 preauthtoken=self.config["SREGISTRY_SWIFT_OS_AUTH_TOKEN"],
             )
         elif self.config["SREGISTRY_SWIFT_AUTHTYPE"] == "keystonev3":
-
             # Keystone v3 Authentication
             # Retrieve the user token, user, and base. Exit if not found
             for envar in [
                 "SREGISTRY_SWIFT_USER",
                 "SREGISTRY_SWIFT_TOKEN",
                 "SREGISTRY_SWIFT_URL",
             ]:
@@ -116,15 +113,14 @@
                 key=self.config["SREGISTRY_SWIFT_TOKEN"],
                 os_options=_os_options,
                 authurl=auth_url,
                 auth_version="3",
             )
 
         elif self.config["SREGISTRY_SWIFT_AUTHTYPE"] == "keystonev2":
-
             # Keystone v2 Authentication
             # Retrieve the user token, user, and base. Exit if not found
             for envar in [
                 "SREGISTRY_SWIFT_USER",
                 "SREGISTRY_SWIFT_TOKEN",
                 "SREGISTRY_SWIFT_TENANT",
                 "SREGISTRY_SWIFT_REGION",
@@ -145,15 +141,14 @@
                 user=self.config["SREGISTRY_SWIFT_USER"],
                 key=self.config["SREGISTRY_SWIFT_TOKEN"],
                 os_options=_os_options,
                 authurl=auth_url,
                 auth_version="2",
             )
         else:
-
             # Legacy Authentication
             # Retrieve the user token, user, and base. Exit if not found
             for envar in [
                 "SREGISTRY_SWIFT_USER",
                 "SREGISTRY_SWIFT_TOKEN",
                 "SREGISTRY_SWIFT_URL",
             ]:
```

### Comparing `sregistry-0.2.38/sregistry/main/swift/pull.py` & `sregistry-0.2.39/sregistry/main/swift/pull.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,14 @@
         images = [images]
 
     bot.debug("Execution of PULL for %s images" % len(images))
 
     # If used internally we want to return a list to the user.
     finished = []
     for image in images:
-
         names = parse_image_name(remove_uri(image))
 
         # First try to get the collection
         collection = self._get_collection(names["collection"])
         if collection is None:
             bot.error("Collection %s does not exist." % names["collection"])
 
@@ -82,15 +81,14 @@
 
         # Write to file
         with open(file_name, "wb") as filey:
             filey.write(obj_tuple[1])
 
         # If we save to storage, the uri is the dropbox_path
         if save is True:
-
             names.update(obj_tuple[0])
             container = self.add(
                 image_path=file_name, image_uri=names["uri"], metadata=names
             )
 
             # When the container is created, this is the path to the image
             image_file = container.image
```

### Comparing `sregistry-0.2.38/sregistry/main/swift/push.py` & `sregistry-0.2.39/sregistry/main/swift/push.py`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/main/swift/query.py` & `sregistry-0.2.39/sregistry/main/swift/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 def search(self, query=None, args=None):
     """query a Singularity registry for a list of images.
     If query is None, collections are listed.
 
     """
 
     if query is not None:
-
         # Here you might do a function that is a general list
         # Note that this means adding the function Client in __init__
         return self._container_query(query)
 
     # or default to listing (searching) all things.
     return self._search_all()
 
@@ -33,15 +32,14 @@
 def search_all(self):
     """a "show all" search that doesn't require a query"""
 
     results = set()
 
     # Here we get names of collections, and then look up containers
     for container in self.conn.get_account()[1]:
-
         # The result here is just the name
         for result in self.conn.get_container(container["name"])[1]:
             results.add("%s/%s" % (container["name"], result["name"]))
 
     if len(results) == 0:
         bot.info("No container collections found.")
         sys.exit(1)
@@ -59,15 +57,14 @@
 
     results = set()
 
     query = remove_uri(query)
 
     # Here we get names of collections, and then look up containers
     for container in self.conn.get_account()[1]:
-
         # The result here is just the name
         for result in self.conn.get_container(container["name"])[1]:
             if query in result["name"]:
                 results.add("%s/%s" % (container["name"], result["name"]))
 
     if len(results) == 0:
         bot.info("No container collections found.")
```

### Comparing `sregistry-0.2.38/sregistry/main/templates/build/singularity-builder-apt.sh` & `sregistry-0.2.39/sregistry/main/templates/build/singularity-builder-apt.sh`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/main/workers/aws.py` & `sregistry-0.2.39/sregistry/main/workers/aws.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,14 @@
     # If we get permissions error, one more try with updated token
     if response.status_code in [401, 403]:
         headers = update_token(headers)
         return stream(url, headers, stream_to, retry=False)
 
     # Successful Response
     elif response.status_code == 200:
-
         # Keep user updated with Progress Bar
         content_size = None
         if "Content-Length" in response.headers:
             progress = 0
             content_size = int(response.headers["Content-Length"])
             bot.show_progress(progress, content_size, length=35)
```

### Comparing `sregistry-0.2.38/sregistry/main/workers/tasks.py` & `sregistry-0.2.39/sregistry/main/workers/tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,14 @@
 
     # Deal with token if necessary
     if response.status_code == 401 and retry is True:
         headers = update_token(response, headers)
         return stream(url, headers, stream_to, retry=False)
 
     if response.status_code == 200:
-
         # Keep user updated with Progress Bar
         content_size = None
         if "Content-Length" in response.headers:
             progress = 0
             content_size = int(response.headers["Content-Length"])
             bot.show_progress(progress, content_size, length=35)
 
@@ -167,15 +166,14 @@
 
     bot.exit("Problem with stream, response %s" % response.status_code)
 
 
 def call(
     url, func, data=None, headers=None, return_json=True, stream=False, retry=True
 ):
-
     """call will issue the call, and issue a refresh token
     given a 401 response, and if the client has a _update_token function
 
     Parameters
     ==========
     func: the function (eg, post, get) to call
     url: the url to send file to
@@ -201,18 +199,16 @@
 
     # Errored response, try again with refresh
     if response.status_code == 404:
         bot.exit("Beep boop! %s: %s" % (response.reason, response.status_code))
 
     # Errored response, try again with refresh
     if response.status_code == 401:
-
         # If client has method to update token, try it once
         if retry is True:
-
             # A result of None indicates no update to the call
             headers = update_token(response, headers)
             return call(
                 url,
                 func,
                 data=data,
                 headers=headers,
@@ -223,17 +219,15 @@
 
         bot.exit(
             "Your credentials are expired! %s: %s"
             % (response.reason, response.status_code)
         )
 
     elif response.status_code == 200:
-
         if return_json:
-
             try:
                 response = response.json()
             except ValueError:
                 bot.exit("The server returned a malformed response.")
 
     return response
```

### Comparing `sregistry-0.2.38/sregistry/main/workers/worker.py` & `sregistry-0.2.39/sregistry/main/workers/worker.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import time
 import signal
 import sys
 
 
 class Workers(object):
     def __init__(self, workers=None):
-
         if workers is None:
             workers = SREGISTRY_WORKERS
         self.workers = workers
         bot.debug("Using %s workers for multiprocess." % (self.workers))
 
     def start(self):
         bot.debug("Starting multiprocess")
```

### Comparing `sregistry-0.2.38/sregistry/tests/test_utils.py` & `sregistry-0.2.39/sregistry/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/utils/fileio.py` & `sregistry-0.2.39/sregistry/utils/fileio.py`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/utils/names.py` & `sregistry-0.2.39/sregistry/utils/names.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,14 @@
     defaults=True,
     ext="sif",
     default_collection="library",
     default_tag="latest",
     base=None,
     lowercase=True,
 ):
-
     """return a collection and repo name and tag
     for an image file.
 
     Parameters
     =========
     image_name: a user provided string indicating a collection,
                 image, and optionally a tag.
```

### Comparing `sregistry-0.2.38/sregistry/utils/terminal.py` & `sregistry-0.2.39/sregistry/utils/terminal.py`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry/version.py` & `sregistry-0.2.39/sregistry/version.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 This Source Code Form is subject to the terms of the
 Mozilla Public License, v. 2.0. If a copy of the MPL was not distributed
 with this file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 """
 
-__version__ = "0.2.38"
+__version__ = "0.2.39"
 AUTHOR = "Vanessa Sochat"
 AUTHOR_EMAIL = "vsochat@stanford.edu"
 NAME = "sregistry"
 PACKAGE_URL = "http://www.github.com/singularityhub/sregistry-cli"
 KEYWORDS = "singularity containers registry hub"
 DESCRIPTION = "Command line tool for working with container storage"
 LICENSE = "LICENSE"
@@ -100,74 +100,74 @@
 ################################################################################
 # Submodule Requirements (versions that include database)
 
 
 INSTALL_REQUIRES_REGISTRY = (
     ("requests-toolbelt", {"min_version": "0.8.0"}),
     ("python-dateutil", {"min_verison": "2.5.3"}),
-    ("sqlalchemy", {"min_version": None}),
+    ("sqlalchemy", {"max_version": "1.4.48"}),
 )
 
 INSTALL_REQUIRES_AWS = (
     ("awscli", {"min_version": "1.16.19"}),
-    ("sqlalchemy", {"min_version": None}),
+    ("sqlalchemy", {"max_version": "1.4.48"}),
 )
 
 INSTALL_REQUIRES_SWIFT = (
     ("python-swiftclient", {"min_version": "3.6.0"}),
-    ("sqlalchemy", {"min_version": None}),
+    ("sqlalchemy", {"max_version": "1.4.48"}),
     ("oauth2client", {"min_version": "3.0"}),
 )
 
 INSTALL_REQUIRES_DROPBOX = (
     ("dropbox", {"min_version": "8.5.1"}),
-    ("sqlalchemy", {"min_version": None}),
+    ("sqlalchemy", {"max_version": "1.4.48"}),
 )
 
 INSTALL_REQUIRES_GLOBUS = (
     ("oauth2client", {"min_version": "3.0"}),
     ("globus_sdk[jwt]", {"min_version": "1.5.0"}),
-    ("sqlalchemy", {"min_version": None}),
+    ("sqlalchemy", {"max_version": "1.4.48"}),
 )
 
 INSTALL_REQUIRES_GOOGLE_STORAGE = (
     ("oauth2client", {"min_version": "3.0"}),
     ("google-cloud-storage", {"min_version": "1.4.0"}),
     ("google-api-python-client", {"min_version": "1.6.4"}),
     ("retrying", {"exact_version": "1.3.3"}),
-    ("sqlalchemy", {"min_version": None}),
+    ("sqlalchemy", {"max_version": "1.4.48"}),
     ("httplib2", {"min_version": "0.18.0"}),
 )
 
 INSTALL_REQUIRES_GOOGLE_BUILD = (
     ("oauth2client", {"min_version": "3.0"}),
     ("google-cloud-storage", {"min_version": "1.4.0"}),
     ("google-api-python-client", {"min_version": "1.6.4"}),
     ("retrying", {"exact_version": "1.3.3"}),
-    ("sqlalchemy", {"min_version": None}),
+    ("sqlalchemy", {"max_version": "1.4.48"}),
     ("httplib2", {"min_version": "0.18.0"}),
 )
 
 INSTALL_REQUIRES_GOOGLE_DRIVE = (
     ("oauth2client", {"min_version": "3.0"}),
-    ("sqlalchemy", {"min_version": None}),
+    ("sqlalchemy", {"max_version": "1.4.48"}),
     ("google-api-python-client", {"min_version": "1.6.4"}),
     ("httplib2", {"min_version": "0.18.0"}),
 )
 
 INSTALL_REQUIRES_GOOGLE_COMPUTE = (
     ("oauth2client", {"min_version": "3.0"}),
-    ("sqlalchemy", {"min_version": None}),
+    ("sqlalchemy", {"max_version": "1.4.48"}),
     ("google-api-python-client", {"min_version": "1.6.4"}),
     ("google-cloud-storage", {"min_version": "1.4.0"}),
     ("httplib2", {"min_version": "0.18.0"}),
 )
 
 INSTALL_REQUIRES_S3 = (
-    ("sqlalchemy", {"min_version": None}),
+    ("sqlalchemy", {"max_version": "1.4.48"}),
     ("boto3", {"min_version": "1.7.83"}),
 )
 
 INSTALL_REQUIRES_ALL = (
     INSTALL_REQUIRES
     + INSTALL_REQUIRES_AWS
     + INSTALL_REQUIRES_S3
```

### Comparing `sregistry-0.2.38/sregistry.egg-info/PKG-INFO` & `sregistry-0.2.39/sregistry.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sregistry
-Version: 0.2.38
+Version: 0.2.39
 Summary: Command line tool for working with container storage
 Home-page: http://www.github.com/singularityhub/sregistry-cli
 Author: Vanessa Sochat
 Author-email: vsochat@stanford.edu
 Maintainer: Vanessa Sochat
 Maintainer-email: vsochat@stanford.edu
 License: LICENSE
```

### Comparing `sregistry-0.2.38/sregistry.egg-info/SOURCES.txt` & `sregistry-0.2.39/sregistry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sregistry-0.2.38/sregistry.egg-info/requires.txt` & `sregistry-0.2.39/sregistry.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -3,44 +3,44 @@
 pygments>=2.1.3
 
 [all]
 spython>=0.0.63
 requests>=2.18.4
 pygments>=2.1.3
 awscli>=1.16.19
-sqlalchemy
-sqlalchemy
+sqlalchemy<=1.4.48
+sqlalchemy<=1.4.48
 boto3>=1.7.83
 python-swiftclient>=3.6.0
-sqlalchemy
+sqlalchemy<=1.4.48
 oauth2client>=3.0
 dropbox>=8.5.1
-sqlalchemy
+sqlalchemy<=1.4.48
 requests-toolbelt>=0.8.0
 requests-toolbelt>=0.8.0
-sqlalchemy
+sqlalchemy<=1.4.48
 oauth2client>=3.0
-sqlalchemy
+sqlalchemy<=1.4.48
 google-api-python-client>=1.6.4
 google-cloud-storage>=1.4.0
 httplib2>=0.18.0
 oauth2client>=3.0
 google-cloud-storage>=1.4.0
 google-api-python-client>=1.6.4
 retrying==1.3.3
-sqlalchemy
+sqlalchemy<=1.4.48
 httplib2>=0.18.0
 oauth2client>=3.0
 google-cloud-storage>=1.4.0
 google-api-python-client>=1.6.4
 retrying==1.3.3
-sqlalchemy
+sqlalchemy<=1.4.48
 httplib2>=0.18.0
 oauth2client>=3.0
-sqlalchemy
+sqlalchemy<=1.4.48
 google-api-python-client>=1.6.4
 httplib2>=0.18.0
 
 [all-basic]
 spython>=0.0.63
 requests>=2.18.4
 pygments>=2.1.3
@@ -70,107 +70,107 @@
 httplib2>=0.18.0
 google-api-python-client>=1.6.4
 oauth2client>=3.0
 httplib2>=0.18.0
 
 [aws]
 awscli>=1.16.19
-sqlalchemy
+sqlalchemy<=1.4.48
 
 [aws-basic]
 awscli>=1.16.19
 
 [dropbox]
 dropbox>=8.5.1
-sqlalchemy
+sqlalchemy<=1.4.48
 
 [dropbox-basic]
 dropbox>=8.5.1
 
 [globus]
 oauth2client>=3.0
 globus_sdk[jwt]>=1.5.0
-sqlalchemy
+sqlalchemy<=1.4.48
 
 [globus-basic]
 oauth2client>=3.0
 globus_sdk[jwt]>=1.5.0
 
 [google-build]
 oauth2client>=3.0
 google-cloud-storage>=1.4.0
 google-api-python-client>=1.6.4
 retrying==1.3.3
-sqlalchemy
+sqlalchemy<=1.4.48
 httplib2>=0.18.0
 
 [google-build-basic]
 oauth2client>=3.0
 google-cloud-storage>=1.4.0
 google-api-python-client>=1.6.4
 retrying>=1.3.3
 httplib2>=0.18.0
 
 [google-compute]
 oauth2client>=3.0
-sqlalchemy
+sqlalchemy<=1.4.48
 google-api-python-client>=1.6.4
 google-cloud-storage>=1.4.0
 httplib2>=0.18.0
 
 [google-compute-basic]
 oauth2client>=3.0
 google-api-python-client>=1.6.4
 google-cloud-storage>=1.4.0
 httplib2>=0.18.0
 
 [google-drive]
 oauth2client>=3.0
-sqlalchemy
+sqlalchemy<=1.4.48
 google-api-python-client>=1.6.4
 httplib2>=0.18.0
 
 [google-drive-basic]
 google-api-python-client>=1.6.4
 oauth2client>=3.0
 httplib2>=0.18.0
 
 [google-storage]
 oauth2client>=3.0
 google-cloud-storage>=1.4.0
 google-api-python-client>=1.6.4
 retrying==1.3.3
-sqlalchemy
+sqlalchemy<=1.4.48
 httplib2>=0.18.0
 
 [google-storage-basic]
 oauth2client>=3.0
 google-cloud-storage>=1.4.0
 google-api-python-client>=1.6.4
 retrying>=1.3.3
 httplib2>=0.18.0
 
 [registry]
 requests-toolbelt>=0.8.0
 requests-toolbelt>=0.8.0
-sqlalchemy
+sqlalchemy<=1.4.48
 
 [registry-basic]
 requests-toolbelt>=0.8.0
 requests-toolbelt>=0.8.0
 
 [s3]
-sqlalchemy
+sqlalchemy<=1.4.48
 boto3>=1.7.83
 
 [s3-basic]
 boto3>=1.7.83
 
 [swift]
 python-swiftclient>=3.6.0
-sqlalchemy
+sqlalchemy<=1.4.48
 oauth2client>=3.0
 
 [swift-basic]
 python-swiftclient>=3.6.0
 python-keystoneclient>=3.5.0
 oauth2client>=3.0
```

