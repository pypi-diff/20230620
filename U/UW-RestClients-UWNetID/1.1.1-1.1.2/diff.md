# Comparing `tmp/UW-RestClients-UWNetID-1.1.1.tar.gz` & `tmp/UW-RestClients-UWNetID-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UW-RestClients-UWNetID-1.1.1.tar", last modified: Fri Feb  3 22:11:10 2023, max compression
+gzip compressed data, was "UW-RestClients-UWNetID-1.1.2.tar", last modified: Tue Jun 20 18:20:11 2023, max compression
```

## Comparing `UW-RestClients-UWNetID-1.1.1.tar` & `UW-RestClients-UWNetID-1.1.2.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 22:11:10.301376 UW-RestClients-UWNetID-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      654 2023-02-03 22:11:10.301376 UW-RestClients-UWNetID-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      607 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 22:11:10.297376 UW-RestClients-UWNetID-1.1.1/UW_RestClients_UWNetID.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      654 2023-02-03 22:11:10.000000 UW-RestClients-UWNetID-1.1.1/UW_RestClients_UWNetID.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3517 2023-02-03 22:11:10.000000 UW-RestClients-UWNetID-1.1.1/UW_RestClients_UWNetID.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-03 22:11:10.000000 UW-RestClients-UWNetID-1.1.1/UW_RestClients_UWNetID.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       67 2023-02-03 22:11:10.000000 UW-RestClients-UWNetID-1.1.1/UW_RestClients_UWNetID.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-02-03 22:11:10.000000 UW-RestClients-UWNetID-1.1.1/UW_RestClients_UWNetID.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-02-03 22:11:10.301376 UW-RestClients-UWNetID-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 22:11:10.297376 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-02-03 22:11:09.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)     1807 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      982 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)     1729 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/category.py
--rw-r--r--   0 runner    (1001) docker     (122)      956 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/dao.py
--rw-r--r--   0 runner    (1001) docker     (122)    18105 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     2046 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/password.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 22:11:10.293376 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 22:11:10.293376 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 22:11:10.293376 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 22:11:10.293376 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 22:11:10.297376 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/
--rw-r--r--   0 runner    (1001) docker     (122)      121 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/category.POST
--rw-r--r--   0 runner    (1001) docker     (122)      401 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/subscription.json.POST
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 22:11:10.297376 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 22:11:10.297376 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/bill/
--rw-r--r--   0 runner    (1001) docker     (122)      363 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/bill/password
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 22:11:10.297376 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/bill/subscription/
--rw-r--r--   0 runner    (1001) docker     (122)      419 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/bill/subscription/233
--rw-r--r--   0 runner    (1001) docker     (122)      427 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/bill/subscription/234
--rw-r--r--   0 runner    (1001) docker     (122)     1895 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/bill/subscription/60
--rw-r--r--   0 runner    (1001) docker     (122)      615 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/bill/subscription/64
--rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/bill/supported.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 22:11:10.297376 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/eight/
--rw-r--r--   0 runner    (1001) docker     (122)      231 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/eight/password
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 22:11:10.297376 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/eight/subscription/
--rw-r--r--   0 runner    (1001) docker     (122)      631 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/eight/subscription/105
--rw-r--r--   0 runner    (1001) docker     (122)      389 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/eight/subscription/60
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 22:11:10.297376 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/emailinfo/
--rw-r--r--   0 runner    (1001) docker     (122)      226 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/emailinfo/admin.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 22:11:10.293376 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/fred/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 22:11:10.297376 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/fred/subscription/
--rw-r--r--   0 runner    (1001) docker     (122)      597 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/fred/subscription/60
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 22:11:10.293376 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/invalidnetid/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 22:11:10.297376 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/invalidnetid/subscription/
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/invalidnetid/subscription/105
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 22:11:10.293376 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/james/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 22:11:10.297376 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/james/subscription/
--rw-r--r--   0 runner    (1001) docker     (122)      826 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/james/subscription/60
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 22:11:10.297376 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/javerage/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 22:11:10.301376 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/javerage/category/
--rw-r--r--   0 runner    (1001) docker     (122)      289 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/javerage/category/25
--rw-r--r--   0 runner    (1001) docker     (122)      966 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/javerage/category/index.html
--rw-r--r--   0 runner    (1001) docker     (122)      256 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/javerage/password
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 22:11:10.301376 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/javerage/subscription/
--rw-r--r--   0 runner    (1001) docker     (122)      849 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/javerage/subscription/105
--rw-r--r--   0 runner    (1001) docker     (122)      791 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/javerage/subscription/233.POST
--rw-r--r--   0 runner    (1001) docker     (122)     1612 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/javerage/subscription/60
--rw-r--r--   0 runner    (1001) docker     (122)     3937 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/javerage/subscription/60,20,100,105,137,41
--rw-r--r--   0 runner    (1001) docker     (122)      627 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/javerage/subscription/64
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 22:11:10.301376 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/jbothell/
--rw-r--r--   0 runner    (1001) docker     (122)      234 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/jbothell/password
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 22:11:10.301376 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/jbothell/subscription/
--rw-r--r--   0 runner    (1001) docker     (122)      641 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/jbothell/subscription/105
--rw-r--r--   0 runner    (1001) docker     (122)     1385 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/jbothell/subscription/60
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 22:11:10.297376 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/jinternational/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 22:11:10.301376 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/jinternational/subscription/
--rw-r--r--   0 runner    (1001) docker     (122)     1093 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/jinternational/subscription/105
--rw-r--r--   0 runner    (1001) docker     (122)     2316 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/jinternational/subscription/60
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 22:11:10.297376 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/jnewstudent/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 22:11:10.301376 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/jnewstudent/subscription/
--rw-r--r--   0 runner    (1001) docker     (122)      647 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/jnewstudent/subscription/105
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 22:11:10.297376 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/none/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 22:11:10.301376 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/none/subscription/
--rw-r--r--   0 runner    (1001) docker     (122)      804 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/none/subscription/105
--rw-r--r--   0 runner    (1001) docker     (122)      359 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/none/subscription/60
--rw-r--r--   0 runner    (1001) docker     (122)      342 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/none/subscription/64
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 22:11:10.297376 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/phil/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 22:11:10.301376 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/phil/subscription/
--rw-r--r--   0 runner    (1001) docker     (122)     1877 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/phil/subscription/60
--rw-r--r--   0 runner    (1001) docker     (122)     5424 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/phil/subscription/60,64,105
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 22:11:10.297376 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/retiree/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 22:11:10.301376 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/retiree/subscription/
--rw-r--r--   0 runner    (1001) docker     (122)     1868 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/retiree/subscription/60
--rw-r--r--   0 runner    (1001) docker     (122)     4416 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/subscription.py
--rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/subscription_105.py
--rw-r--r--   0 runner    (1001) docker     (122)     1297 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/subscription_233.py
--rw-r--r--   0 runner    (1001) docker     (122)     5957 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/subscription_60.py
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/subscription_64.py
--rw-r--r--   0 runner    (1001) docker     (122)     1009 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/supported.py
--rw-r--r--   0 runner    (1001) docker     (122)      466 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 22:11:10.301376 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      175 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      993 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (122)      813 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/tests/test_category.py
--rw-r--r--   0 runner    (1001) docker     (122)     3548 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/tests/test_password.py
--rw-r--r--   0 runner    (1001) docker     (122)     6504 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/tests/test_subsciption.py
--rw-r--r--   0 runner    (1001) docker     (122)     2498 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/tests/test_subscription_105.py
--rw-r--r--   0 runner    (1001) docker     (122)      688 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/tests/test_subscription_233.py
--rw-r--r--   0 runner    (1001) docker     (122)     6882 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/tests/test_subscription_60.py
--rw-r--r--   0 runner    (1001) docker     (122)     1656 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/tests/test_subscription_64.py
--rw-r--r--   0 runner    (1001) docker     (122)     1122 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/tests/test_supported.py
--rw-r--r--   0 runner    (1001) docker     (122)      231 2023-02-03 22:11:01.000000 UW-RestClients-UWNetID-1.1.1/uw_uwnetid/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 18:20:11.770518 UW-RestClients-UWNetID-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      654 2023-06-20 18:20:11.766518 UW-RestClients-UWNetID-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      607 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 18:20:11.762519 UW-RestClients-UWNetID-1.1.2/UW_RestClients_UWNetID.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      654 2023-06-20 18:20:11.000000 UW-RestClients-UWNetID-1.1.2/UW_RestClients_UWNetID.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3517 2023-06-20 18:20:11.000000 UW-RestClients-UWNetID-1.1.2/UW_RestClients_UWNetID.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-20 18:20:11.000000 UW-RestClients-UWNetID-1.1.2/UW_RestClients_UWNetID.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       67 2023-06-20 18:20:11.000000 UW-RestClients-UWNetID-1.1.2/UW_RestClients_UWNetID.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-06-20 18:20:11.000000 UW-RestClients-UWNetID-1.1.2/UW_RestClients_UWNetID.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-20 18:20:11.770518 UW-RestClients-UWNetID-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 18:20:11.762519 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-20 18:20:11.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)     1807 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      982 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1729 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/category.py
+-rw-r--r--   0 runner    (1001) docker     (122)      956 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/dao.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18143 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2046 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/password.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 18:20:11.758519 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 18:20:11.758519 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 18:20:11.758519 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 18:20:11.758519 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 18:20:11.762519 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)      121 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/category.POST
+-rw-r--r--   0 runner    (1001) docker     (122)      401 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/subscription.json.POST
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 18:20:11.762519 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 18:20:11.762519 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/bill/
+-rw-r--r--   0 runner    (1001) docker     (122)      363 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/bill/password
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 18:20:11.762519 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/bill/subscription/
+-rw-r--r--   0 runner    (1001) docker     (122)      419 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/bill/subscription/233
+-rw-r--r--   0 runner    (1001) docker     (122)      427 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/bill/subscription/234
+-rw-r--r--   0 runner    (1001) docker     (122)     1895 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/bill/subscription/60
+-rw-r--r--   0 runner    (1001) docker     (122)      615 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/bill/subscription/64
+-rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/bill/supported.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 18:20:11.766518 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/eight/
+-rw-r--r--   0 runner    (1001) docker     (122)      231 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/eight/password
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 18:20:11.766518 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/eight/subscription/
+-rw-r--r--   0 runner    (1001) docker     (122)      631 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/eight/subscription/105
+-rw-r--r--   0 runner    (1001) docker     (122)      389 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/eight/subscription/60
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 18:20:11.766518 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/emailinfo/
+-rw-r--r--   0 runner    (1001) docker     (122)      226 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/emailinfo/admin.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 18:20:11.762519 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/fred/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 18:20:11.766518 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/fred/subscription/
+-rw-r--r--   0 runner    (1001) docker     (122)      597 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/fred/subscription/60
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 18:20:11.762519 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/invalidnetid/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 18:20:11.766518 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/invalidnetid/subscription/
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/invalidnetid/subscription/105
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 18:20:11.762519 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/james/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 18:20:11.766518 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/james/subscription/
+-rw-r--r--   0 runner    (1001) docker     (122)      826 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/james/subscription/60
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 18:20:11.766518 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/javerage/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 18:20:11.766518 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/javerage/category/
+-rw-r--r--   0 runner    (1001) docker     (122)      289 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/javerage/category/25
+-rw-r--r--   0 runner    (1001) docker     (122)      966 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/javerage/category/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)      256 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/javerage/password
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 18:20:11.766518 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/javerage/subscription/
+-rw-r--r--   0 runner    (1001) docker     (122)      849 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/javerage/subscription/105
+-rw-r--r--   0 runner    (1001) docker     (122)      791 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/javerage/subscription/233.POST
+-rw-r--r--   0 runner    (1001) docker     (122)     1612 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/javerage/subscription/60
+-rw-r--r--   0 runner    (1001) docker     (122)     3937 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/javerage/subscription/60,20,100,105,137,41
+-rw-r--r--   0 runner    (1001) docker     (122)      627 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/javerage/subscription/64
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 18:20:11.766518 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/jbothell/
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/jbothell/password
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 18:20:11.766518 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/jbothell/subscription/
+-rw-r--r--   0 runner    (1001) docker     (122)      641 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/jbothell/subscription/105
+-rw-r--r--   0 runner    (1001) docker     (122)     1385 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/jbothell/subscription/60
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 18:20:11.762519 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/jinternational/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 18:20:11.766518 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/jinternational/subscription/
+-rw-r--r--   0 runner    (1001) docker     (122)     1093 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/jinternational/subscription/105
+-rw-r--r--   0 runner    (1001) docker     (122)     2316 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/jinternational/subscription/60
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 18:20:11.762519 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/jnewstudent/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 18:20:11.766518 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/jnewstudent/subscription/
+-rw-r--r--   0 runner    (1001) docker     (122)      647 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/jnewstudent/subscription/105
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 18:20:11.762519 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/none/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 18:20:11.766518 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/none/subscription/
+-rw-r--r--   0 runner    (1001) docker     (122)      804 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/none/subscription/105
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/none/subscription/60
+-rw-r--r--   0 runner    (1001) docker     (122)      342 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/none/subscription/64
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 18:20:11.762519 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/phil/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 18:20:11.766518 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/phil/subscription/
+-rw-r--r--   0 runner    (1001) docker     (122)     1877 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/phil/subscription/60
+-rw-r--r--   0 runner    (1001) docker     (122)     5424 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/phil/subscription/60,64,105
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 18:20:11.762519 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/retiree/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 18:20:11.766518 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/retiree/subscription/
+-rw-r--r--   0 runner    (1001) docker     (122)     1868 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/retiree/subscription/60
+-rw-r--r--   0 runner    (1001) docker     (122)     4416 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/subscription_105.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1297 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/subscription_233.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5957 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/subscription_60.py
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/subscription_64.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1009 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/supported.py
+-rw-r--r--   0 runner    (1001) docker     (122)      466 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 18:20:11.766518 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      993 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      813 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/tests/test_category.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3548 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/tests/test_password.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6504 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/tests/test_subsciption.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2498 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/tests/test_subscription_105.py
+-rw-r--r--   0 runner    (1001) docker     (122)      688 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/tests/test_subscription_233.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6882 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/tests/test_subscription_60.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1656 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/tests/test_subscription_64.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1122 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/tests/test_supported.py
+-rw-r--r--   0 runner    (1001) docker     (122)      231 2023-06-20 18:20:02.000000 UW-RestClients-UWNetID-1.1.2/uw_uwnetid/util.py
```

### Comparing `UW-RestClients-UWNetID-1.1.1/LICENSE` & `UW-RestClients-UWNetID-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `UW-RestClients-UWNetID-1.1.1/PKG-INFO` & `UW-RestClients-UWNetID-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: UW-RestClients-UWNetID
-Version: 1.1.1
+Version: 1.1.2
 Summary: A library for connecting to the UW NetID API
 Home-page: https://github.com/uw-it-aca/uw-restclients-uwnetid
 Author: UW-IT AXDD
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
 Description: 
         See the README on `GitHub
```

### Comparing `UW-RestClients-UWNetID-1.1.1/README.md` & `UW-RestClients-UWNetID-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `UW-RestClients-UWNetID-1.1.1/UW_RestClients_UWNetID.egg-info/PKG-INFO` & `UW-RestClients-UWNetID-1.1.2/UW_RestClients_UWNetID.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: UW-RestClients-UWNetID
-Version: 1.1.1
+Version: 1.1.2
 Summary: A library for connecting to the UW NetID API
 Home-page: https://github.com/uw-it-aca/uw-restclients-uwnetid
 Author: UW-IT AXDD
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
 Description: 
         See the README on `GitHub
```

### Comparing `UW-RestClients-UWNetID-1.1.1/UW_RestClients_UWNetID.egg-info/SOURCES.txt` & `UW-RestClients-UWNetID-1.1.2/UW_RestClients_UWNetID.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `UW-RestClients-UWNetID-1.1.1/setup.py` & `UW-RestClients-UWNetID-1.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-UWNetID-1.1.1/uw_uwnetid/__init__.py` & `UW-RestClients-UWNetID-1.1.2/uw_uwnetid/__init__.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-UWNetID-1.1.1/uw_uwnetid/admin.py` & `UW-RestClients-UWNetID-1.1.2/uw_uwnetid/admin.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-UWNetID-1.1.1/uw_uwnetid/category.py` & `UW-RestClients-UWNetID-1.1.2/uw_uwnetid/category.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-UWNetID-1.1.1/uw_uwnetid/dao.py` & `UW-RestClients-UWNetID-1.1.2/uw_uwnetid/dao.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-UWNetID-1.1.1/uw_uwnetid/models.py` & `UW-RestClients-UWNetID-1.1.2/uw_uwnetid/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -326,14 +326,15 @@
     ALTID_SUPPORT_DEPARTMENTAL = 69
     GOOGLE_SUITE_ENDORSEE = 234
     OFFICE_365_ENDORSEE = 235
     CANVAS_PROVISIONEE = 236
     ZOOM_LICENSED_PROVISIONEE = 237
     ZOOM_BASIC_PROVISIONEE = 238
     HUSKY_ONNET_EXT_PROVISIONEE = 239
+    OFFICE_365_STUDENT_ENDORSEE = 291
 
     STATUS_ACTIVE = 1
     STATUS_GRACE = 2
     STATUS_FORMER = 3
 
     STATUS_CHOICES = (
         (STATUS_ACTIVE, "Active"),
```

### Comparing `UW-RestClients-UWNetID-1.1.1/uw_uwnetid/password.py` & `UW-RestClients-UWNetID-1.1.2/uw_uwnetid/password.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/bill/subscription/60` & `UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/bill/subscription/60`

 * *Files identical despite different names*

### Comparing `UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/bill/subscription/64` & `UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/bill/subscription/64`

 * *Files identical despite different names*

### Comparing `UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/bill/supported.json` & `UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/bill/supported.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/eight/subscription/105` & `UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/eight/subscription/105`

 * *Files identical despite different names*

### Comparing `UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/fred/subscription/60` & `UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/fred/subscription/60`

 * *Files identical despite different names*

### Comparing `UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/james/subscription/60` & `UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/james/subscription/60`

 * *Files identical despite different names*

### Comparing `UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/javerage/category/index.html` & `UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/javerage/category/index.html`

 * *Files identical despite different names*

### Comparing `UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/javerage/subscription/105` & `UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/javerage/subscription/105`

 * *Files identical despite different names*

### Comparing `UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/javerage/subscription/233.POST` & `UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/javerage/subscription/233.POST`

 * *Files identical despite different names*

### Comparing `UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/javerage/subscription/60` & `UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/javerage/subscription/60`

 * *Files identical despite different names*

### Comparing `UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/javerage/subscription/60,20,100,105,137,41` & `UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/javerage/subscription/60,20,100,105,137,41`

 * *Files identical despite different names*

### Comparing `UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/javerage/subscription/64` & `UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/javerage/subscription/64`

 * *Files identical despite different names*

### Comparing `UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/jbothell/subscription/105` & `UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/jbothell/subscription/105`

 * *Files identical despite different names*

### Comparing `UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/jbothell/subscription/60` & `UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/jbothell/subscription/60`

 * *Files identical despite different names*

### Comparing `UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/jinternational/subscription/105` & `UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/jinternational/subscription/105`

 * *Files identical despite different names*

### Comparing `UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/jinternational/subscription/60` & `UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/jinternational/subscription/60`

 * *Files identical despite different names*

### Comparing `UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/jnewstudent/subscription/105` & `UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/jnewstudent/subscription/105`

 * *Files identical despite different names*

### Comparing `UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/none/subscription/105` & `UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/none/subscription/105`

 * *Files identical despite different names*

### Comparing `UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/phil/subscription/60` & `UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/phil/subscription/60`

 * *Files identical despite different names*

### Comparing `UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/phil/subscription/60,64,105` & `UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/phil/subscription/60,64,105`

 * *Files identical despite different names*

### Comparing `UW-RestClients-UWNetID-1.1.1/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/retiree/subscription/60` & `UW-RestClients-UWNetID-1.1.2/uw_uwnetid/resources/uwnetid/file/nws/v1/uwnetid/retiree/subscription/60`

 * *Files identical despite different names*

### Comparing `UW-RestClients-UWNetID-1.1.1/uw_uwnetid/subscription.py` & `UW-RestClients-UWNetID-1.1.2/uw_uwnetid/subscription.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-UWNetID-1.1.1/uw_uwnetid/subscription_105.py` & `UW-RestClients-UWNetID-1.1.2/uw_uwnetid/subscription_105.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-UWNetID-1.1.1/uw_uwnetid/subscription_233.py` & `UW-RestClients-UWNetID-1.1.2/uw_uwnetid/subscription_233.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-UWNetID-1.1.1/uw_uwnetid/subscription_60.py` & `UW-RestClients-UWNetID-1.1.2/uw_uwnetid/subscription_60.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-UWNetID-1.1.1/uw_uwnetid/subscription_64.py` & `UW-RestClients-UWNetID-1.1.2/uw_uwnetid/subscription_64.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-UWNetID-1.1.1/uw_uwnetid/supported.py` & `UW-RestClients-UWNetID-1.1.2/uw_uwnetid/supported.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-UWNetID-1.1.1/uw_uwnetid/tests/test_admin.py` & `UW-RestClients-UWNetID-1.1.2/uw_uwnetid/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-UWNetID-1.1.1/uw_uwnetid/tests/test_category.py` & `UW-RestClients-UWNetID-1.1.2/uw_uwnetid/tests/test_category.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-UWNetID-1.1.1/uw_uwnetid/tests/test_password.py` & `UW-RestClients-UWNetID-1.1.2/uw_uwnetid/tests/test_password.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-UWNetID-1.1.1/uw_uwnetid/tests/test_subsciption.py` & `UW-RestClients-UWNetID-1.1.2/uw_uwnetid/tests/test_subsciption.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-UWNetID-1.1.1/uw_uwnetid/tests/test_subscription_105.py` & `UW-RestClients-UWNetID-1.1.2/uw_uwnetid/tests/test_subscription_105.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-UWNetID-1.1.1/uw_uwnetid/tests/test_subscription_233.py` & `UW-RestClients-UWNetID-1.1.2/uw_uwnetid/tests/test_subscription_233.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-UWNetID-1.1.1/uw_uwnetid/tests/test_subscription_60.py` & `UW-RestClients-UWNetID-1.1.2/uw_uwnetid/tests/test_subscription_60.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-UWNetID-1.1.1/uw_uwnetid/tests/test_subscription_64.py` & `UW-RestClients-UWNetID-1.1.2/uw_uwnetid/tests/test_subscription_64.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-UWNetID-1.1.1/uw_uwnetid/tests/test_supported.py` & `UW-RestClients-UWNetID-1.1.2/uw_uwnetid/tests/test_supported.py`

 * *Files identical despite different names*

