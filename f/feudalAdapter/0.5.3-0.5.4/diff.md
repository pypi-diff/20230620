# Comparing `tmp/feudalAdapter-0.5.3.tar.gz` & `tmp/feudalAdapter-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feudalAdapter-0.5.3.tar", last modified: Mon Oct 10 12:43:15 2022, max compression
+gzip compressed data, was "feudalAdapter-0.5.4.tar", last modified: Tue Jun 20 08:15:16 2023, max compression
```

## Comparing `feudalAdapter-0.5.3.tar` & `feudalAdapter-0.5.4.tar`

### file list

```diff
@@ -1,104 +1,105 @@
-drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2022-10-10 12:43:15.453848 feudalAdapter-0.5.3/
--rw-r--r--   0 diana     (1000) diana     (1000)     1115 2022-10-08 20:36:35.000000 feudalAdapter-0.5.3/.gitlab-ci.yml
--rw-r--r--   0 diana     (1000) diana     (1000)      409 2022-10-10 12:43:12.000000 feudalAdapter-0.5.3/AUTHORS
--rw-r--r--   0 diana     (1000) diana     (1000)    20582 2022-10-10 12:43:12.000000 feudalAdapter-0.5.3/ChangeLog
--rw-r--r--   0 diana     (1000) diana     (1000)     8427 2022-05-31 16:26:19.000000 feudalAdapter-0.5.3/LDAP.md
--rw-r--r--   0 diana     (1000) diana     (1000)     1130 2022-05-31 16:26:19.000000 feudalAdapter-0.5.3/LICENSE
--rw-r--r--   0 diana     (1000) diana     (1000)    17582 2022-10-10 12:43:15.453848 feudalAdapter-0.5.3/PKG-INFO
--rw-r--r--   0 diana     (1000) diana     (1000)    16606 2022-09-06 15:38:34.000000 feudalAdapter-0.5.3/README.md
--rw-r--r--   0 diana     (1000) diana     (1000)     2672 2022-05-31 16:26:19.000000 feudalAdapter-0.5.3/conftest.py
--rw-r--r--   0 diana     (1000) diana     (1000)      403 2022-09-06 15:38:34.000000 feudalAdapter-0.5.3/devel-requirements.txt
-drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2022-10-10 12:43:15.443848 feudalAdapter-0.5.3/examples/
--rw-r--r--   0 diana     (1000) diana     (1000)      206 2022-09-06 15:38:34.000000 feudalAdapter-0.5.3/examples/diana-accept.json
--rw-r--r--   0 diana     (1000) diana     (1000)     1193 2022-09-06 15:38:34.000000 feudalAdapter-0.5.3/examples/diana-deploy.json
--rw-r--r--   0 diana     (1000) diana     (1000)      208 2022-09-06 15:38:34.000000 feudalAdapter-0.5.3/examples/diana-get_status.json
--rw-r--r--   0 diana     (1000) diana     (1000)      206 2022-09-06 15:38:34.000000 feudalAdapter-0.5.3/examples/diana-reject.json
--rw-r--r--   0 diana     (1000) diana     (1000)      129 2022-09-06 15:38:34.000000 feudalAdapter-0.5.3/examples/diana-test-approval.json
--rw-r--r--   0 diana     (1000) diana     (1000)     2565 2022-05-31 16:26:19.000000 feudalAdapter-0.5.3/examples/lukas_deply.json
--rw-r--r--   0 diana     (1000) diana     (1000)     7306 2022-05-31 16:26:19.000000 feudalAdapter-0.5.3/examples/marcus-deploy-egi.json
--rw-r--r--   0 diana     (1000) diana     (1000)     1990 2022-05-31 16:26:19.000000 feudalAdapter-0.5.3/examples/marcus-deploy-iam-groups.json
--rw-r--r--   0 diana     (1000) diana     (1000)     1791 2022-05-31 16:26:19.000000 feudalAdapter-0.5.3/examples/marcus-deploy-no-groups.json
--rw-r--r--   0 diana     (1000) diana     (1000)     2657 2022-05-31 16:26:19.000000 feudalAdapter-0.5.3/examples/marcus-deploy-no-pref-username.json
--rw-r--r--   0 diana     (1000) diana     (1000)     2786 2022-05-31 16:26:19.000000 feudalAdapter-0.5.3/examples/marcus-deploy-other-id.json
--rw-r--r--   0 diana     (1000) diana     (1000)      205 2022-05-31 16:26:19.000000 feudalAdapter-0.5.3/examples/marcus-get_status.json
--rw-r--r--   0 diana     (1000) diana     (1000)     7310 2022-05-31 16:26:19.000000 feudalAdapter-0.5.3/examples/marcus-undeploy-egi.json
--rw-r--r--   0 diana     (1000) diana     (1000)      207 2022-05-31 16:26:19.000000 feudalAdapter-0.5.3/examples/marcus-undeploy-minimal.json
--rw-r--r--   0 diana     (1000) diana     (1000)      223 2022-05-31 16:26:19.000000 feudalAdapter-0.5.3/examples/marcus-undeploy-old.json
--rw-r--r--   0 diana     (1000) diana     (1000)     1217 2022-05-31 16:26:19.000000 feudalAdapter-0.5.3/examples/marcus-undeploy-other-id.json
--rw-r--r--   0 diana     (1000) diana     (1000)      760 2022-05-31 16:26:19.000000 feudalAdapter-0.5.3/examples/marcus-undeploy.json
-drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2022-10-10 12:43:15.447181 feudalAdapter-0.5.3/feudalAdapter.egg-info/
--rw-r--r--   0 diana     (1000) diana     (1000)    17582 2022-10-10 12:43:12.000000 feudalAdapter-0.5.3/feudalAdapter.egg-info/PKG-INFO
--rw-r--r--   0 diana     (1000) diana     (1000)     2420 2022-10-10 12:43:15.000000 feudalAdapter-0.5.3/feudalAdapter.egg-info/SOURCES.txt
--rw-r--r--   0 diana     (1000) diana     (1000)        1 2022-10-10 12:43:12.000000 feudalAdapter-0.5.3/feudalAdapter.egg-info/dependency_links.txt
--rw-r--r--   0 diana     (1000) diana     (1000)      104 2022-10-10 12:43:12.000000 feudalAdapter-0.5.3/feudalAdapter.egg-info/entry_points.txt
--rw-r--r--   0 diana     (1000) diana     (1000)        1 2022-06-02 15:50:40.000000 feudalAdapter-0.5.3/feudalAdapter.egg-info/not-zip-safe
--rw-r--r--   0 diana     (1000) diana     (1000)       47 2022-10-10 12:43:12.000000 feudalAdapter-0.5.3/feudalAdapter.egg-info/pbr.json
--rw-r--r--   0 diana     (1000) diana     (1000)      412 2022-10-10 12:43:12.000000 feudalAdapter-0.5.3/feudalAdapter.egg-info/requires.txt
--rw-r--r--   0 diana     (1000) diana     (1000)       32 2022-10-10 12:43:12.000000 feudalAdapter-0.5.3/feudalAdapter.egg-info/top_level.txt
--rw-r--r--   0 diana     (1000) diana     (1000)    12589 2022-10-08 20:36:35.000000 feudalAdapter-0.5.3/feudal_adapter_template.conf
-drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2022-10-10 12:43:15.447181 feudalAdapter-0.5.3/feudal_globalconfig/
--rw-r--r--   0 diana     (1000) diana     (1000)        0 2022-05-31 16:26:19.000000 feudalAdapter-0.5.3/feudal_globalconfig/__init__.py
--rw-r--r--   0 diana     (1000) diana     (1000)       89 2022-05-31 16:26:19.000000 feudalAdapter-0.5.3/feudal_globalconfig/globalconfig.py
-drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2022-10-10 12:43:15.447181 feudalAdapter-0.5.3/ldf_adapter/
--rw-r--r--   0 diana     (1000) diana     (1000)    35785 2022-10-08 20:36:35.000000 feudalAdapter-0.5.3/ldf_adapter/__init__.py
-drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2022-10-10 12:43:15.447181 feudalAdapter-0.5.3/ldf_adapter/approval/
--rw-r--r--   0 diana     (1000) diana     (1000)    12504 2022-10-08 20:36:35.000000 feudalAdapter-0.5.3/ldf_adapter/approval/__init__.py
-drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2022-10-10 12:43:15.450514 feudalAdapter-0.5.3/ldf_adapter/approval/db/
--rw-r--r--   0 diana     (1000) diana     (1000)      185 2022-09-06 16:21:30.000000 feudalAdapter-0.5.3/ldf_adapter/approval/db/__init__.py
--rw-r--r--   0 diana     (1000) diana     (1000)     3289 2022-09-06 15:38:34.000000 feudalAdapter-0.5.3/ldf_adapter/approval/db/generic.py
--rw-r--r--   0 diana     (1000) diana     (1000)    20008 2022-10-10 11:04:57.000000 feudalAdapter-0.5.3/ldf_adapter/approval/db/sqlite.py
--rw-r--r--   0 diana     (1000) diana     (1000)     1843 2022-09-06 15:38:34.000000 feudalAdapter-0.5.3/ldf_adapter/approval/models.py
-drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2022-10-10 12:43:15.450514 feudalAdapter-0.5.3/ldf_adapter/backend/
--rw-r--r--   0 diana     (1000) diana     (1000)      407 2022-09-06 16:21:30.000000 feudalAdapter-0.5.3/ldf_adapter/backend/__init__.py
--rw-r--r--   0 diana     (1000) diana     (1000)    18388 2022-10-08 20:36:35.000000 feudalAdapter-0.5.3/ldf_adapter/backend/bwidm.py
--rw-r--r--   0 diana     (1000) diana     (1000)     6172 2022-10-08 20:36:35.000000 feudalAdapter-0.5.3/ldf_adapter/backend/generic.py
--rw-r--r--   0 diana     (1000) diana     (1000)    35962 2022-10-08 20:36:35.000000 feudalAdapter-0.5.3/ldf_adapter/backend/ldap.py
--rw-r--r--   0 diana     (1000) diana     (1000)    33787 2022-10-08 20:36:35.000000 feudalAdapter-0.5.3/ldf_adapter/backend/local_unix.py
--rw-r--r--   0 diana     (1000) diana     (1000)     1343 2022-09-06 15:38:34.000000 feudalAdapter-0.5.3/ldf_adapter/cmdline_params.py
--rw-r--r--   0 diana     (1000) diana     (1000)    12601 2022-10-08 20:36:35.000000 feudalAdapter-0.5.3/ldf_adapter/config.py
--rw-r--r--   0 diana     (1000) diana     (1000)     3330 2022-09-06 15:38:34.000000 feudalAdapter-0.5.3/ldf_adapter/eduperson.py
--rwxr-xr-x   0 diana     (1000) diana     (1000)     2381 2022-09-06 15:38:34.000000 feudalAdapter-0.5.3/ldf_adapter/interface.py
--rw-r--r--   0 diana     (1000) diana     (1000)     4052 2022-09-06 15:38:34.000000 feudalAdapter-0.5.3/ldf_adapter/logsetup.py
--rw-r--r--   0 diana     (1000) diana     (1000)     4834 2022-09-06 16:21:30.000000 feudalAdapter-0.5.3/ldf_adapter/name_generators.py
-drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2022-10-10 12:43:15.450514 feudalAdapter-0.5.3/ldf_adapter/notifier/
--rw-r--r--   0 diana     (1000) diana     (1000)      184 2022-09-06 16:21:30.000000 feudalAdapter-0.5.3/ldf_adapter/notifier/__init__.py
--rw-r--r--   0 diana     (1000) diana     (1000)     1486 2022-09-06 16:21:30.000000 feudalAdapter-0.5.3/ldf_adapter/notifier/courier.py
--rw-r--r--   0 diana     (1000) diana     (1000)     6348 2022-09-06 16:21:30.000000 feudalAdapter-0.5.3/ldf_adapter/notifier/email.py
--rw-r--r--   0 diana     (1000) diana     (1000)     2259 2022-09-06 15:38:34.000000 feudalAdapter-0.5.3/ldf_adapter/notifier/generic.py
--rw-r--r--   0 diana     (1000) diana     (1000)     5241 2022-09-06 15:38:34.000000 feudalAdapter-0.5.3/ldf_adapter/results.py
--rw-r--r--   0 diana     (1000) diana     (1000)    16461 2022-09-06 16:21:30.000000 feudalAdapter-0.5.3/ldf_adapter/userinfo.py
--rw-r--r--   0 diana     (1000) diana     (1000)     6987 2022-09-06 16:21:30.000000 feudalAdapter-0.5.3/ldf_adapter/utils.py
--rw-r--r--   0 diana     (1000) diana     (1000)      182 2022-05-31 16:26:19.000000 feudalAdapter-0.5.3/pytest.ini
--rw-r--r--   0 diana     (1000) diana     (1000)      412 2022-09-06 15:38:34.000000 feudalAdapter-0.5.3/requirements.txt
--rw-r--r--   0 diana     (1000) diana     (1000)     1391 2022-10-10 12:43:15.453848 feudalAdapter-0.5.3/setup.cfg
--rwxr-xr-x   0 diana     (1000) diana     (1000)      110 2022-05-31 16:26:19.000000 feudalAdapter-0.5.3/setup.py
--rw-r--r--   0 diana     (1000) diana     (1000)     6217 2022-09-06 15:38:34.000000 feudalAdapter-0.5.3/states.md
--rwxr-xr-x   0 diana     (1000) diana     (1000)     6539 2022-05-31 16:26:19.000000 feudalAdapter-0.5.3/subiss-to-unix.py
-drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2022-10-10 12:43:15.450514 feudalAdapter-0.5.3/templates/
--rw-r--r--   0 diana     (1000) diana     (1000)     1084 2022-09-06 15:38:34.000000 feudalAdapter-0.5.3/templates/admin.deploy.template
--rw-r--r--   0 diana     (1000) diana     (1000)     1051 2022-09-06 15:38:34.000000 feudalAdapter-0.5.3/templates/admin.deploy.update.template
--rw-r--r--   0 diana     (1000) diana     (1000)      302 2022-09-06 15:38:34.000000 feudalAdapter-0.5.3/templates/admin.test.template
--rw-r--r--   0 diana     (1000) diana     (1000)      991 2022-09-06 15:38:34.000000 feudalAdapter-0.5.3/templates/admin.update.template
--rw-r--r--   0 diana     (1000) diana     (1000)      255 2022-09-06 15:38:34.000000 feudalAdapter-0.5.3/templates/unknown.template
--rw-r--r--   0 diana     (1000) diana     (1000)      380 2022-09-06 15:38:34.000000 feudalAdapter-0.5.3/templates/user.deploy.template
--rw-r--r--   0 diana     (1000) diana     (1000)      417 2022-09-06 15:38:34.000000 feudalAdapter-0.5.3/templates/user.deploy.update.template
--rw-r--r--   0 diana     (1000) diana     (1000)      395 2022-09-06 15:38:34.000000 feudalAdapter-0.5.3/templates/user.update.template
-drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2022-10-10 12:43:15.453848 feudalAdapter-0.5.3/tests/
--rw-r--r--   0 diana     (1000) diana     (1000)        0 2022-09-06 16:13:04.000000 feudalAdapter-0.5.3/tests/__init__.py
-drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2022-10-10 12:43:15.453848 feudalAdapter-0.5.3/tests/approval/
-drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2022-10-10 12:43:15.453848 feudalAdapter-0.5.3/tests/approval/db/
--rw-r--r--   0 diana     (1000) diana     (1000)     7601 2022-09-06 16:21:36.000000 feudalAdapter-0.5.3/tests/approval/db/generic.py
--rw-r--r--   0 diana     (1000) diana     (1000)    23145 2022-09-06 15:38:34.000000 feudalAdapter-0.5.3/tests/approval/db/sqlite.py
--rw-r--r--   0 diana     (1000) diana     (1000)        0 2022-09-06 15:38:34.000000 feudalAdapter-0.5.3/tests/approval/pending_deployment.py
-drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2022-10-10 12:43:15.453848 feudalAdapter-0.5.3/tests/backend/
--rw-r--r--   0 diana     (1000) diana     (1000)        0 2022-09-06 16:35:16.000000 feudalAdapter-0.5.3/tests/backend/__init__.py
--rw-r--r--   0 diana     (1000) diana     (1000)    18764 2022-10-08 20:36:35.000000 feudalAdapter-0.5.3/tests/backend/ldap.py
--rw-r--r--   0 diana     (1000) diana     (1000)    19654 2022-10-08 20:36:35.000000 feudalAdapter-0.5.3/tests/backend/local_unix.py
--rw-r--r--   0 diana     (1000) diana     (1000)      217 2022-09-07 08:21:18.000000 feudalAdapter-0.5.3/tests/conftest.py
--rw-r--r--   0 diana     (1000) diana     (1000)     5778 2022-09-06 15:38:34.000000 feudalAdapter-0.5.3/tests/eduperson.py
--rw-r--r--   0 diana     (1000) diana     (1000)    11209 2022-10-08 20:36:35.000000 feudalAdapter-0.5.3/tests/feudal_adapter.conf
--rw-r--r--   0 diana     (1000) diana     (1000)    17765 2022-09-06 16:21:36.000000 feudalAdapter-0.5.3/tests/name_generators.py
--rw-r--r--   0 diana     (1000) diana     (1000)     5645 2022-09-06 16:32:23.000000 feudalAdapter-0.5.3/tests/settings.py
--rw-r--r--   0 diana     (1000) diana     (1000)    13297 2022-10-08 20:36:35.000000 feudalAdapter-0.5.3/tests/user.py
--rw-r--r--   0 diana     (1000) diana     (1000)    14757 2022-09-06 16:37:04.000000 feudalAdapter-0.5.3/tests/userinfo.py
--rw-r--r--   0 diana     (1000) diana     (1000)     1209 2022-08-19 18:02:48.000000 feudalAdapter-0.5.3/tox.ini
+drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-06-20 08:15:16.777137 feudalAdapter-0.5.4/
+-rw-r--r--   0 diana     (1000) diana     (1000)     1212 2023-06-16 10:14:56.000000 feudalAdapter-0.5.4/.gitlab-ci.yml
+-rw-r--r--   0 diana     (1000) diana     (1000)      409 2023-06-20 08:15:13.000000 feudalAdapter-0.5.4/AUTHORS
+-rw-r--r--   0 diana     (1000) diana     (1000)    20780 2023-06-20 08:15:13.000000 feudalAdapter-0.5.4/ChangeLog
+-rw-r--r--   0 diana     (1000) diana     (1000)     8427 2022-02-17 10:03:18.000000 feudalAdapter-0.5.4/LDAP.md
+-rw-r--r--   0 diana     (1000) diana     (1000)     1130 2020-12-22 11:09:29.000000 feudalAdapter-0.5.4/LICENSE
+-rw-r--r--   0 diana     (1000) diana     (1000)    17562 2023-06-20 08:15:16.777137 feudalAdapter-0.5.4/PKG-INFO
+-rw-r--r--   0 diana     (1000) diana     (1000)    16606 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/README.md
+-rw-r--r--   0 diana     (1000) diana     (1000)     2672 2020-12-22 11:09:29.000000 feudalAdapter-0.5.4/conftest.py
+-rw-r--r--   0 diana     (1000) diana     (1000)      403 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/devel-requirements.txt
+drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-06-20 08:15:16.730471 feudalAdapter-0.5.4/examples/
+-rw-r--r--   0 diana     (1000) diana     (1000)      206 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/examples/diana-accept.json
+-rw-r--r--   0 diana     (1000) diana     (1000)     2238 2022-11-07 10:43:24.000000 feudalAdapter-0.5.4/examples/diana-deploy-punch4nfdi.json
+-rw-r--r--   0 diana     (1000) diana     (1000)     1193 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/examples/diana-deploy.json
+-rw-r--r--   0 diana     (1000) diana     (1000)      208 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/examples/diana-get_status.json
+-rw-r--r--   0 diana     (1000) diana     (1000)      206 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/examples/diana-reject.json
+-rw-r--r--   0 diana     (1000) diana     (1000)      129 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/examples/diana-test-approval.json
+-rw-r--r--   0 diana     (1000) diana     (1000)     2565 2020-12-22 11:09:29.000000 feudalAdapter-0.5.4/examples/lukas_deply.json
+-rw-r--r--   0 diana     (1000) diana     (1000)     7306 2022-02-17 10:03:18.000000 feudalAdapter-0.5.4/examples/marcus-deploy-egi.json
+-rw-r--r--   0 diana     (1000) diana     (1000)     1990 2021-01-26 21:58:12.000000 feudalAdapter-0.5.4/examples/marcus-deploy-iam-groups.json
+-rw-r--r--   0 diana     (1000) diana     (1000)     1791 2021-01-26 21:58:12.000000 feudalAdapter-0.5.4/examples/marcus-deploy-no-groups.json
+-rw-r--r--   0 diana     (1000) diana     (1000)     2657 2021-01-08 15:30:24.000000 feudalAdapter-0.5.4/examples/marcus-deploy-no-pref-username.json
+-rw-r--r--   0 diana     (1000) diana     (1000)     2786 2022-02-17 10:03:18.000000 feudalAdapter-0.5.4/examples/marcus-deploy-other-id.json
+-rw-r--r--   0 diana     (1000) diana     (1000)      205 2021-01-08 15:30:24.000000 feudalAdapter-0.5.4/examples/marcus-get_status.json
+-rw-r--r--   0 diana     (1000) diana     (1000)     7310 2022-02-17 10:03:18.000000 feudalAdapter-0.5.4/examples/marcus-undeploy-egi.json
+-rw-r--r--   0 diana     (1000) diana     (1000)      207 2022-02-17 10:03:18.000000 feudalAdapter-0.5.4/examples/marcus-undeploy-minimal.json
+-rw-r--r--   0 diana     (1000) diana     (1000)      223 2022-02-17 10:03:18.000000 feudalAdapter-0.5.4/examples/marcus-undeploy-old.json
+-rw-r--r--   0 diana     (1000) diana     (1000)     1217 2022-02-17 10:03:18.000000 feudalAdapter-0.5.4/examples/marcus-undeploy-other-id.json
+-rw-r--r--   0 diana     (1000) diana     (1000)      760 2021-01-08 15:30:24.000000 feudalAdapter-0.5.4/examples/marcus-undeploy.json
+drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-06-20 08:15:16.733804 feudalAdapter-0.5.4/feudalAdapter.egg-info/
+-rw-r--r--   0 diana     (1000) diana     (1000)    17562 2023-06-20 08:15:13.000000 feudalAdapter-0.5.4/feudalAdapter.egg-info/PKG-INFO
+-rw-r--r--   0 diana     (1000) diana     (1000)     2458 2023-06-20 08:15:16.000000 feudalAdapter-0.5.4/feudalAdapter.egg-info/SOURCES.txt
+-rw-r--r--   0 diana     (1000) diana     (1000)        1 2023-06-20 08:15:13.000000 feudalAdapter-0.5.4/feudalAdapter.egg-info/dependency_links.txt
+-rw-r--r--   0 diana     (1000) diana     (1000)      103 2023-06-20 08:15:13.000000 feudalAdapter-0.5.4/feudalAdapter.egg-info/entry_points.txt
+-rw-r--r--   0 diana     (1000) diana     (1000)        1 2020-12-22 14:42:04.000000 feudalAdapter-0.5.4/feudalAdapter.egg-info/not-zip-safe
+-rw-r--r--   0 diana     (1000) diana     (1000)       47 2023-06-20 08:15:13.000000 feudalAdapter-0.5.4/feudalAdapter.egg-info/pbr.json
+-rw-r--r--   0 diana     (1000) diana     (1000)      412 2023-06-20 08:15:13.000000 feudalAdapter-0.5.4/feudalAdapter.egg-info/requires.txt
+-rw-r--r--   0 diana     (1000) diana     (1000)       32 2023-06-20 08:15:13.000000 feudalAdapter-0.5.4/feudalAdapter.egg-info/top_level.txt
+-rw-r--r--   0 diana     (1000) diana     (1000)    12589 2022-11-07 10:43:24.000000 feudalAdapter-0.5.4/feudal_adapter_template.conf
+drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-06-20 08:15:16.733804 feudalAdapter-0.5.4/feudal_globalconfig/
+-rw-r--r--   0 diana     (1000) diana     (1000)        0 2021-01-15 14:31:35.000000 feudalAdapter-0.5.4/feudal_globalconfig/__init__.py
+-rw-r--r--   0 diana     (1000) diana     (1000)       89 2022-02-17 10:03:18.000000 feudalAdapter-0.5.4/feudal_globalconfig/globalconfig.py
+drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-06-20 08:15:16.737137 feudalAdapter-0.5.4/ldf_adapter/
+-rw-r--r--   0 diana     (1000) diana     (1000)    35785 2023-06-16 10:05:18.000000 feudalAdapter-0.5.4/ldf_adapter/__init__.py
+drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-06-20 08:15:16.737137 feudalAdapter-0.5.4/ldf_adapter/approval/
+-rw-r--r--   0 diana     (1000) diana     (1000)    12504 2023-06-16 10:06:16.000000 feudalAdapter-0.5.4/ldf_adapter/approval/__init__.py
+drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-06-20 08:15:16.737137 feudalAdapter-0.5.4/ldf_adapter/approval/db/
+-rw-r--r--   0 diana     (1000) diana     (1000)      185 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/ldf_adapter/approval/db/__init__.py
+-rw-r--r--   0 diana     (1000) diana     (1000)     3289 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/ldf_adapter/approval/db/generic.py
+-rw-r--r--   0 diana     (1000) diana     (1000)    20008 2023-06-16 10:06:16.000000 feudalAdapter-0.5.4/ldf_adapter/approval/db/sqlite.py
+-rw-r--r--   0 diana     (1000) diana     (1000)     1843 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/ldf_adapter/approval/models.py
+drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-06-20 08:15:16.740471 feudalAdapter-0.5.4/ldf_adapter/backend/
+-rw-r--r--   0 diana     (1000) diana     (1000)      407 2023-06-16 10:05:17.000000 feudalAdapter-0.5.4/ldf_adapter/backend/__init__.py
+-rw-r--r--   0 diana     (1000) diana     (1000)    18388 2023-06-16 10:05:17.000000 feudalAdapter-0.5.4/ldf_adapter/backend/bwidm.py
+-rw-r--r--   0 diana     (1000) diana     (1000)     6172 2022-11-07 10:43:24.000000 feudalAdapter-0.5.4/ldf_adapter/backend/generic.py
+-rw-r--r--   0 diana     (1000) diana     (1000)    35962 2023-06-16 10:06:16.000000 feudalAdapter-0.5.4/ldf_adapter/backend/ldap.py
+-rw-r--r--   0 diana     (1000) diana     (1000)    33784 2023-06-16 10:06:34.000000 feudalAdapter-0.5.4/ldf_adapter/backend/local_unix.py
+-rw-r--r--   0 diana     (1000) diana     (1000)     1343 2023-06-16 10:05:17.000000 feudalAdapter-0.5.4/ldf_adapter/cmdline_params.py
+-rw-r--r--   0 diana     (1000) diana     (1000)    12853 2023-06-16 10:07:10.000000 feudalAdapter-0.5.4/ldf_adapter/config.py
+-rw-r--r--   0 diana     (1000) diana     (1000)     3330 2023-06-16 10:05:17.000000 feudalAdapter-0.5.4/ldf_adapter/eduperson.py
+-rwxr-xr-x   0 diana     (1000) diana     (1000)     2381 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/ldf_adapter/interface.py
+-rw-r--r--   0 diana     (1000) diana     (1000)     4052 2023-06-16 10:05:17.000000 feudalAdapter-0.5.4/ldf_adapter/logsetup.py
+-rw-r--r--   0 diana     (1000) diana     (1000)     4833 2023-06-16 10:06:33.000000 feudalAdapter-0.5.4/ldf_adapter/name_generators.py
+drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-06-20 08:15:16.747137 feudalAdapter-0.5.4/ldf_adapter/notifier/
+-rw-r--r--   0 diana     (1000) diana     (1000)      184 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/ldf_adapter/notifier/__init__.py
+-rw-r--r--   0 diana     (1000) diana     (1000)     1486 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/ldf_adapter/notifier/courier.py
+-rw-r--r--   0 diana     (1000) diana     (1000)     6348 2023-06-16 10:06:16.000000 feudalAdapter-0.5.4/ldf_adapter/notifier/email.py
+-rw-r--r--   0 diana     (1000) diana     (1000)     2259 2023-06-16 10:05:17.000000 feudalAdapter-0.5.4/ldf_adapter/notifier/generic.py
+-rw-r--r--   0 diana     (1000) diana     (1000)     5241 2023-06-16 10:05:17.000000 feudalAdapter-0.5.4/ldf_adapter/results.py
+-rw-r--r--   0 diana     (1000) diana     (1000)    16459 2023-06-16 10:06:34.000000 feudalAdapter-0.5.4/ldf_adapter/userinfo.py
+-rw-r--r--   0 diana     (1000) diana     (1000)     6987 2023-06-16 10:05:17.000000 feudalAdapter-0.5.4/ldf_adapter/utils.py
+-rw-r--r--   0 diana     (1000) diana     (1000)      182 2022-02-17 10:03:18.000000 feudalAdapter-0.5.4/pytest.ini
+-rw-r--r--   0 diana     (1000) diana     (1000)      412 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/requirements.txt
+-rw-r--r--   0 diana     (1000) diana     (1000)     1391 2023-06-20 08:15:16.780470 feudalAdapter-0.5.4/setup.cfg
+-rwxr-xr-x   0 diana     (1000) diana     (1000)      110 2020-12-22 11:09:29.000000 feudalAdapter-0.5.4/setup.py
+-rw-r--r--   0 diana     (1000) diana     (1000)     6217 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/states.md
+-rwxr-xr-x   0 diana     (1000) diana     (1000)     6539 2020-11-06 10:06:35.000000 feudalAdapter-0.5.4/subiss-to-unix.py
+drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-06-20 08:15:16.757137 feudalAdapter-0.5.4/templates/
+-rw-r--r--   0 diana     (1000) diana     (1000)     1084 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/templates/admin.deploy.template
+-rw-r--r--   0 diana     (1000) diana     (1000)     1051 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/templates/admin.deploy.update.template
+-rw-r--r--   0 diana     (1000) diana     (1000)      302 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/templates/admin.test.template
+-rw-r--r--   0 diana     (1000) diana     (1000)      991 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/templates/admin.update.template
+-rw-r--r--   0 diana     (1000) diana     (1000)      255 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/templates/unknown.template
+-rw-r--r--   0 diana     (1000) diana     (1000)      380 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/templates/user.deploy.template
+-rw-r--r--   0 diana     (1000) diana     (1000)      417 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/templates/user.deploy.update.template
+-rw-r--r--   0 diana     (1000) diana     (1000)      395 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/templates/user.update.template
+drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-06-20 08:15:16.767137 feudalAdapter-0.5.4/tests/
+-rw-r--r--   0 diana     (1000) diana     (1000)        0 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/tests/__init__.py
+drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-06-20 08:15:16.767137 feudalAdapter-0.5.4/tests/approval/
+drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-06-20 08:15:16.770470 feudalAdapter-0.5.4/tests/approval/db/
+-rw-r--r--   0 diana     (1000) diana     (1000)     7601 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/tests/approval/db/generic.py
+-rw-r--r--   0 diana     (1000) diana     (1000)    23145 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/tests/approval/db/sqlite.py
+-rw-r--r--   0 diana     (1000) diana     (1000)        0 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/tests/approval/pending_deployment.py
+drwxr-xr-x   0 diana     (1000) diana     (1000)        0 2023-06-20 08:15:16.777137 feudalAdapter-0.5.4/tests/backend/
+-rw-r--r--   0 diana     (1000) diana     (1000)        0 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/tests/backend/__init__.py
+-rw-r--r--   0 diana     (1000) diana     (1000)    18764 2022-11-07 10:43:24.000000 feudalAdapter-0.5.4/tests/backend/ldap.py
+-rw-r--r--   0 diana     (1000) diana     (1000)    19654 2022-11-07 10:43:24.000000 feudalAdapter-0.5.4/tests/backend/local_unix.py
+-rw-r--r--   0 diana     (1000) diana     (1000)      217 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/tests/conftest.py
+-rw-r--r--   0 diana     (1000) diana     (1000)     5778 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/tests/eduperson.py
+-rw-r--r--   0 diana     (1000) diana     (1000)    11209 2022-11-07 10:43:24.000000 feudalAdapter-0.5.4/tests/feudal_adapter.conf
+-rw-r--r--   0 diana     (1000) diana     (1000)    17765 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/tests/name_generators.py
+-rw-r--r--   0 diana     (1000) diana     (1000)     5645 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/tests/settings.py
+-rw-r--r--   0 diana     (1000) diana     (1000)    13297 2022-11-07 10:43:24.000000 feudalAdapter-0.5.4/tests/user.py
+-rw-r--r--   0 diana     (1000) diana     (1000)    14757 2022-09-21 14:19:00.000000 feudalAdapter-0.5.4/tests/userinfo.py
+-rw-r--r--   0 diana     (1000) diana     (1000)     1218 2023-06-16 10:00:21.000000 feudalAdapter-0.5.4/tox.ini
```

### Comparing `feudalAdapter-0.5.3/.gitlab-ci.yml` & `feudalAdapter-0.5.4/.gitlab-ci.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 stages:
-    - test
-    - build
-    - deploy
+  - test
+  - build
+  - deploy
 
 .install_dependencies:
   before_script:
     - pip install --upgrade pip
     - pip install tox
 
 pylint:
@@ -40,14 +40,20 @@
 
 python310:
   image: python:3.10
   extends: .install_dependencies
   stage: test
   script: tox -e py310
 
+python311:
+  image: python:3.11
+  extends: .install_dependencies
+  stage: test
+  script: tox -e py311
+
 coverage:
   image: python:3.10
   extends: .install_dependencies
   stage: test
   script: tox -e report
   coverage: '/TOTAL.+ ([0-9]{1,3}%)/'
   artifacts:
```

### Comparing `feudalAdapter-0.5.3/ChangeLog` & `feudalAdapter-0.5.4/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 CHANGES
 =======
 
+v0.5.4
+------
+
+* add tests for python 3.11 to gitlab ci
+* apply black
+* add python 3.11 to test envs in tox
+* use default\_factory for fields of custom types
+* add example for punch4nfdi exception
+
 v0.5.3
 ------
 
 * create folder hierarchy for pending db
 
 v0.5.2
 ------
```

### Comparing `feudalAdapter-0.5.3/LDAP.md` & `feudalAdapter-0.5.4/LDAP.md`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/LICENSE` & `feudalAdapter-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/PKG-INFO` & `feudalAdapter-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: feudalAdapter
-Version: 0.5.3
+Version: 0.5.4
 Summary: Adapter to connect provisioning events with a backend
 Home-page: https://git.scc.kit.edu/feudal/feudal_adapter_ldf
 Author: Joshua Bachmeier
 Author-email: joshua.bachmeier@student.kit.edu
 License: MIT
 Project-URL: Bug Tracker, https://git.scc.kit.edu/feudal/feudal_adapter_ldf/issues
 Project-URL: Documentation, https://git.scc.kit.edu/feudal/feudal_adapter_ldf
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
 Classifier: Natural Language :: English
@@ -478,9 +477,7 @@
 # Feudal systemd service
 
 To enable a feudal service this might be helpful:
 ```
 systemctl --user --now enable feudalClient@0
 ```
 
-
-
```

### Comparing `feudalAdapter-0.5.3/README.md` & `feudalAdapter-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/conftest.py` & `feudalAdapter-0.5.4/conftest.py`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/examples/diana-deploy.json` & `feudalAdapter-0.5.4/examples/diana-deploy.json`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/examples/lukas_deply.json` & `feudalAdapter-0.5.4/examples/lukas_deply.json`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/examples/marcus-deploy-egi.json` & `feudalAdapter-0.5.4/examples/marcus-deploy-egi.json`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/examples/marcus-deploy-iam-groups.json` & `feudalAdapter-0.5.4/examples/marcus-deploy-iam-groups.json`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/examples/marcus-deploy-no-groups.json` & `feudalAdapter-0.5.4/examples/marcus-deploy-no-groups.json`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/examples/marcus-deploy-no-pref-username.json` & `feudalAdapter-0.5.4/examples/marcus-deploy-no-pref-username.json`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/examples/marcus-deploy-other-id.json` & `feudalAdapter-0.5.4/examples/marcus-deploy-other-id.json`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/examples/marcus-undeploy-egi.json` & `feudalAdapter-0.5.4/examples/marcus-undeploy-egi.json`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/examples/marcus-undeploy-other-id.json` & `feudalAdapter-0.5.4/examples/marcus-undeploy-other-id.json`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/examples/marcus-undeploy.json` & `feudalAdapter-0.5.4/examples/marcus-undeploy.json`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/feudalAdapter.egg-info/PKG-INFO` & `feudalAdapter-0.5.4/feudalAdapter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: feudalAdapter
-Version: 0.5.3
+Version: 0.5.4
 Summary: Adapter to connect provisioning events with a backend
 Home-page: https://git.scc.kit.edu/feudal/feudal_adapter_ldf
 Author: Joshua Bachmeier
 Author-email: joshua.bachmeier@student.kit.edu
 License: MIT
 Project-URL: Bug Tracker, https://git.scc.kit.edu/feudal/feudal_adapter_ldf/issues
 Project-URL: Documentation, https://git.scc.kit.edu/feudal/feudal_adapter_ldf
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
 Classifier: Natural Language :: English
@@ -478,9 +477,7 @@
 # Feudal systemd service
 
 To enable a feudal service this might be helpful:
 ```
 systemctl --user --now enable feudalClient@0
 ```
 
-
-
```

### Comparing `feudalAdapter-0.5.3/feudalAdapter.egg-info/SOURCES.txt` & `feudalAdapter-0.5.4/feudalAdapter.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 requirements.txt
 setup.cfg
 setup.py
 states.md
 subiss-to-unix.py
 tox.ini
 examples/diana-accept.json
+examples/diana-deploy-punch4nfdi.json
 examples/diana-deploy.json
 examples/diana-get_status.json
 examples/diana-reject.json
 examples/diana-test-approval.json
 examples/lukas_deply.json
 examples/marcus-deploy-egi.json
 examples/marcus-deploy-iam-groups.json
```

### Comparing `feudalAdapter-0.5.3/feudal_adapter_template.conf` & `feudalAdapter-0.5.4/feudal_adapter_template.conf`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/ldf_adapter/__init__.py` & `feudalAdapter-0.5.4/ldf_adapter/__init__.py`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/ldf_adapter/approval/__init__.py` & `feudalAdapter-0.5.4/ldf_adapter/approval/__init__.py`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/ldf_adapter/approval/db/generic.py` & `feudalAdapter-0.5.4/ldf_adapter/approval/db/generic.py`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/ldf_adapter/approval/db/sqlite.py` & `feudalAdapter-0.5.4/ldf_adapter/approval/db/sqlite.py`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/ldf_adapter/approval/models.py` & `feudalAdapter-0.5.4/ldf_adapter/approval/models.py`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/ldf_adapter/backend/bwidm.py` & `feudalAdapter-0.5.4/ldf_adapter/backend/bwidm.py`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/ldf_adapter/backend/generic.py` & `feudalAdapter-0.5.4/ldf_adapter/backend/generic.py`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/ldf_adapter/backend/ldap.py` & `feudalAdapter-0.5.4/ldf_adapter/backend/ldap.py`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/ldf_adapter/backend/local_unix.py` & `feudalAdapter-0.5.4/ldf_adapter/backend/local_unix.py`

 * *Files 0% similar despite different names*

```diff
@@ -627,15 +627,14 @@
     # usernames and group names can only be 32 characters long.
     # My fix is to remove characters a) after the first '_' if there is one.
     #                                b) from the beginning if there is none
     # Also adds two dots as an indicator for where the shortening took place
 
     excess_chars = len(word) - 32
     if excess_chars > 0:
-
         if len(word.split("_")) == 1:  # no '_' found:
             word = "__" + word[excess_chars + 2 :]
             # logger.warning(F"shortened {orig_word} to {word}")
 
         elif len(word.split("_")) > 1:  # at least one '_' found:
             fragments = word.split("_")
             if (
@@ -831,15 +830,14 @@
     # to progressively remove the characters in excess.
     # .. used to indicate where the shortening took place.
     orig_excess_chars = len(word) - 32
     excess_chars = len(word) - 32
     fragments = word.split("_")
 
     if excess_chars > 0:
-
         for n in range(len(fragments)):
             if len(fragments[n]) <= 3:
                 continue
             if excess_chars == 0:
                 break
             excess_chars += 2
 
@@ -848,15 +846,14 @@
                 excess_chars -= 1
                 if excess_chars == 0:
                     break
 
             fragments[n] = fragments[n] + ".."
 
     if orig_excess_chars > 0:
-
         if excess_chars > 0:
             return None
         else:
             if len(fragments) > 1:
                 word = "_".join(fragments)
             else:
                 word = fragments[0]
```

### Comparing `feudalAdapter-0.5.3/ldf_adapter/cmdline_params.py` & `feudalAdapter-0.5.4/ldf_adapter/cmdline_params.py`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/ldf_adapter/config.py` & `feudalAdapter-0.5.4/ldf_adapter/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -384,32 +384,32 @@
     courier: Optional[ConfigCourier] = None
 
 
 @dataclass
 class ConfigBackends(ConfigListOfSections):
     """Collection of config sections for all backends"""
 
-    local_unix: ConfigLocalUnix = ConfigLocalUnix()
-    ldap: ConfigLdap = ConfigLdap()
-    bwidm: ConfigBwIdm = ConfigBwIdm()
+    local_unix: ConfigLocalUnix = field(default_factory=ConfigLocalUnix)
+    ldap: ConfigLdap = field(default_factory=ConfigLdap)
+    bwidm: ConfigBwIdm = field(default_factory=ConfigBwIdm)
 
 
 @dataclass
 class Configuration:
     """All configuration settings for the feudal adapter"""
 
-    ldf_adapter: ConfigLdfAdapter = ConfigLdfAdapter()
-    messages: ConfigMessages = ConfigMessages()
-    approval: ConfigApproval = ConfigApproval()
-    notifier: ConfigNotifiers = ConfigNotifiers()
-    assurance: ConfigAssurance = ConfigAssurance()
-    username_generator: ConfigUsernameGenerator = ConfigUsernameGenerator()
-    login_info: ConfigLoginInfo = ConfigLoginInfo()
-    backend: ConfigBackends = ConfigBackends()
-    verbose_info_plugin: ConfigVerboseInfoPlugin = ConfigVerboseInfoPlugin()
+    ldf_adapter: ConfigLdfAdapter = field(default_factory=ConfigLdfAdapter)
+    messages: ConfigMessages = field(default_factory=ConfigMessages)
+    approval: ConfigApproval = field(default_factory=ConfigApproval)
+    notifier: ConfigNotifiers = field(default_factory=ConfigNotifiers)
+    assurance: ConfigAssurance = field(default_factory=ConfigAssurance)
+    username_generator: ConfigUsernameGenerator = field(default_factory=ConfigUsernameGenerator)
+    login_info: ConfigLoginInfo = field(default_factory=ConfigLoginInfo)
+    backend: ConfigBackends = field(default_factory=ConfigBackends)
+    verbose_info_plugin: ConfigVerboseInfoPlugin = field(default_factory=ConfigVerboseInfoPlugin)
 
     @classmethod
     def load(cls, config: ConfigParser):
         """Loads all config settings from the given config parser"""
         return cls(**{f.name: f.type.load(config) for f in fields(cls)})
```

### Comparing `feudalAdapter-0.5.3/ldf_adapter/eduperson.py` & `feudalAdapter-0.5.4/ldf_adapter/eduperson.py`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/ldf_adapter/interface.py` & `feudalAdapter-0.5.4/ldf_adapter/interface.py`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/ldf_adapter/logsetup.py` & `feudalAdapter-0.5.4/ldf_adapter/logsetup.py`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/ldf_adapter/name_generators.py` & `feudalAdapter-0.5.4/ldf_adapter/name_generators.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,14 @@
         """suggest a valid username"""
         # Copy forbidden names:
         for name in forbidden_names or []:
             if name.lower() not in self.dont_use_these_names:
                 self.dont_use_these_names.append(name.lower())
 
         while True:
-
             self.next_strategy_idx += 1
             try:
                 candidate_name = (
                     self.strategies[self.next_strategy_idx]
                     .format(**locals())
                     .lower()
                     .replace("@", "-")
```

### Comparing `feudalAdapter-0.5.3/ldf_adapter/notifier/courier.py` & `feudalAdapter-0.5.4/ldf_adapter/notifier/courier.py`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/ldf_adapter/notifier/email.py` & `feudalAdapter-0.5.4/ldf_adapter/notifier/email.py`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/ldf_adapter/notifier/generic.py` & `feudalAdapter-0.5.4/ldf_adapter/notifier/generic.py`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/ldf_adapter/results.py` & `feudalAdapter-0.5.4/ldf_adapter/results.py`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/ldf_adapter/userinfo.py` & `feudalAdapter-0.5.4/ldf_adapter/userinfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,15 +218,15 @@
         attr = self.userinfo.get("eduperson_entitlement", [])
         if not isinstance(attr, list):
             attr = [attr]
 
         def try_entitlement(attr):
             try:
                 return eduperson.Entitlement(attr)
-            except (ValueError):
+            except ValueError:
                 return None
 
         return filter(lambda x: x, map(try_entitlement, attr))
 
     @property
     def group(self):
         """Return the unparsed group attribute of the user"""
```

### Comparing `feudalAdapter-0.5.3/ldf_adapter/utils.py` & `feudalAdapter-0.5.4/ldf_adapter/utils.py`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/setup.cfg` & `feudalAdapter-0.5.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/states.md` & `feudalAdapter-0.5.4/states.md`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/subiss-to-unix.py` & `feudalAdapter-0.5.4/subiss-to-unix.py`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/templates/admin.deploy.template` & `feudalAdapter-0.5.4/templates/admin.deploy.template`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/templates/admin.deploy.update.template` & `feudalAdapter-0.5.4/templates/admin.deploy.update.template`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/templates/admin.update.template` & `feudalAdapter-0.5.4/templates/admin.update.template`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/tests/approval/db/generic.py` & `feudalAdapter-0.5.4/tests/approval/db/generic.py`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/tests/approval/db/sqlite.py` & `feudalAdapter-0.5.4/tests/approval/db/sqlite.py`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/tests/backend/ldap.py` & `feudalAdapter-0.5.4/tests/backend/ldap.py`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/tests/backend/local_unix.py` & `feudalAdapter-0.5.4/tests/backend/local_unix.py`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/tests/eduperson.py` & `feudalAdapter-0.5.4/tests/eduperson.py`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/tests/feudal_adapter.conf` & `feudalAdapter-0.5.4/tests/feudal_adapter.conf`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/tests/name_generators.py` & `feudalAdapter-0.5.4/tests/name_generators.py`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/tests/settings.py` & `feudalAdapter-0.5.4/tests/settings.py`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/tests/user.py` & `feudalAdapter-0.5.4/tests/user.py`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/tests/userinfo.py` & `feudalAdapter-0.5.4/tests/userinfo.py`

 * *Files identical despite different names*

### Comparing `feudalAdapter-0.5.3/tox.ini` & `feudalAdapter-0.5.4/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 envlist =
   clean
   pylint,
   py37,
   py38,
   py39,
   py310,
+  py311,
   pyright,
   black,
   report
 
 [base]
 deps =
        -rrequirements.txt
```

