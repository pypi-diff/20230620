# Comparing `tmp/pike-smb2-0.4.0a4.tar.gz` & `tmp/pike-smb2-0.4.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pike-smb2-0.4.0a4.tar", last modified: Tue Dec 20 22:15:53 2022, max compression
+gzip compressed data, was "pike-smb2-0.4.0a5.tar", last modified: Wed Dec 21 03:09:57 2022, max compression
```

## Comparing `pike-smb2-0.4.0a4.tar` & `pike-smb2-0.4.0a5.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:15:53.819020 pike-smb2-0.4.0a4/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      117 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:15:53.803019 pike-smb2-0.4.0a4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:15:53.803019 pike-smb2-0.4.0a4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/.github/workflows/test_samba.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/.github/workflows/wheels.yml
--rw-r--r--   0 runner    (1001) docker     (123)      117 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      149 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/.gitignorerevs
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10202 2022-12-20 22:15:53.819020 pike-smb2-0.4.0a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6290 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:15:53.803019 pike-smb2-0.4.0a4/buildwheel/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/buildwheel/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      195 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/buildwheel/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      487 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/buildwheel/wheel27.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:15:53.803019 pike-smb2-0.4.0a4/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      647 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/doc/class-hierarchy.dot
--rw-r--r--   0 runner    (1001) docker     (123)      315 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/doc/container-model.dot
--rw-r--r--   0 runner    (1001) docker     (123)      492 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/doc/object-model.dot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:15:53.807019 pike-smb2-0.4.0a4/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:15:53.807019 pike-smb2-0.4.0a4/doc/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/doc/source/_templates/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)      346 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/doc/source/autosummary.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9471 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/doc/source/high_level.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3979 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/doc/source/model.rst
--rw-r--r--   0 runner    (1001) docker     (123)      173 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/doc/source/open.rst
--rw-r--r--   0 runner    (1001) docker     (123)      135 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/doc/source/path.rst
--rw-r--r--   0 runner    (1001) docker     (123)      758 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/doc/source/pytest.rst
--rw-r--r--   0 runner    (1001) docker     (123)      168 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/doc/source/tree_connect.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:15:53.807019 pike-smb2-0.4.0a4/pykerb/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/pykerb/MakeKitBuild
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/pykerb/base64.c
--rw-r--r--   0 runner    (1001) docker     (123)      746 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/pykerb/base64.h
--rw-r--r--   0 runner    (1001) docker     (123)    16691 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/pykerb/kerberos.c
--rw-r--r--   0 runner    (1001) docker     (123)     9825 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/pykerb/kerberos.py
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/pykerb/kerberosbasic.c
--rw-r--r--   0 runner    (1001) docker     (123)      898 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/pykerb/kerberosbasic.h
--rw-r--r--   0 runner    (1001) docker     (123)    28331 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/pykerb/kerberosgss.c
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/pykerb/kerberosgss.h
--rw-r--r--   0 runner    (1001) docker     (123)     4440 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/pykerb/kerberospw.c
--rw-r--r--   0 runner    (1001) docker     (123)      867 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/pykerb/kerberospw.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:15:53.807019 pike-smb2-0.4.0a4/pykerb/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:15:53.811019 pike-smb2-0.4.0a4/pykerb/vendor/py3c/
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/pykerb/vendor/py3c/capsulethunk.h
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/pykerb/vendor/py3c/comparison.h
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/pykerb/vendor/py3c/compat.h
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/pykerb/vendor/py3c/fileshim.h
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/pykerb/vendor/py3c/py3shims.h
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/pykerb/vendor/py3c/tpflags.h
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/pykerb/vendor/py3c.h
--rw-r--r--   0 runner    (1001) docker     (123)      717 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:15:53.811019 pike-smb2-0.4.0a4/samba/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/samba/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      178 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/samba/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      600 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/samba/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       13 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/samba/admin_password
--rwxr-xr-x   0 runner    (1001) docker     (123)      164 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/samba/build_and_test_wheels.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      316 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/samba/build_and_test_wheels27.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      665 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/samba/dc.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/samba/docker-compose.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      333 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/samba/krb5.conf.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      323 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/samba/run_all.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/samba/share.conf
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2022-12-20 22:15:53.823020 pike-smb2-0.4.0a4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1316 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:15:53.803019 pike-smb2-0.4.0a4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:15:53.815020 pike-smb2-0.4.0a4/src/pike/
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/src/pike/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/src/pike/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    23725 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/src/pike/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    11098 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/src/pike/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/src/pike/digest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/src/pike/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17920 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/src/pike/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    81933 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/src/pike/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/src/pike/netbios.py
--rw-r--r--   0 runner    (1001) docker     (123)    25680 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/src/pike/ntlm.py
--rw-r--r--   0 runner    (1001) docker     (123)    84326 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/src/pike/ntstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/src/pike/nttime.py
--rw-r--r--   0 runner    (1001) docker     (123)    25417 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/src/pike/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/src/pike/pytest_support.py
--rw-r--r--   0 runner    (1001) docker     (123)   136885 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/src/pike/smb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:15:53.819020 pike-smb2-0.4.0a4/src/pike/test/
--rw-r--r--   0 runner    (1001) docker     (123)    27985 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/src/pike/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/src/pike/test/acl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6534 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/src/pike/test/appinstanceid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/src/pike/test/changenotify.py
--rw-r--r--   0 runner    (1001) docker     (123)     5497 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/src/pike/test/compound.py
--rw-r--r--   0 runner    (1001) docker     (123)    44139 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/src/pike/test/copychunk.py
--rw-r--r--   0 runner    (1001) docker     (123)    23712 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/src/pike/test/credit.py
--rw-r--r--   0 runner    (1001) docker     (123)    11364 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/src/pike/test/durable.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/src/pike/test/echo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/src/pike/test/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/src/pike/test/invalid_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/src/pike/test/invalid_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/src/pike/test/ioctl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/src/pike/test/lease.py
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/src/pike/test/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/src/pike/test/multichannel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/src/pike/test/negotiate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/src/pike/test/oplock.py
--rw-r--r--   0 runner    (1001) docker     (123)    10254 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/src/pike/test/persistent.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/src/pike/test/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     5485 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/src/pike/test/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/src/pike/test/querydirectory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6939 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/src/pike/test/queryondiskid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6705 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/src/pike/test/readwrite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/src/pike/test/reparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/src/pike/test/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/src/pike/test/set.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/src/pike/test/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    15036 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/src/pike/transport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:15:53.819020 pike-smb2-0.4.0a4/src/pike_smb2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10202 2022-12-20 22:15:53.000000 pike-smb2-0.4.0a4/src/pike_smb2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2022-12-20 22:15:53.000000 pike-smb2-0.4.0a4/src/pike_smb2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 22:15:53.000000 pike-smb2-0.4.0a4/src/pike_smb2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-20 22:15:53.000000 pike-smb2-0.4.0a4/src/pike_smb2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2022-12-20 22:15:53.000000 pike-smb2-0.4.0a4/src/pike_smb2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2022-12-20 22:15:53.000000 pike-smb2-0.4.0a4/src/pike_smb2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 22:15:53.819020 pike-smb2-0.4.0a4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     9551 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/tests/test_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5385 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     9406 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/tests/test_path.py
--rw-r--r--   0 runner    (1001) docker     (123)    18297 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/tests/test_smb3_encryption_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/tests/test_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2022-12-20 22:15:42.000000 pike-smb2-0.4.0a4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 03:09:57.042028 pike-smb2-0.4.0a5/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 03:09:57.026028 pike-smb2-0.4.0a5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 03:09:57.030028 pike-smb2-0.4.0a5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/.github/workflows/test_samba.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/.github/workflows/wheels.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/.gitignorerevs
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10183 2022-12-21 03:09:57.042028 pike-smb2-0.4.0a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 03:09:57.030028 pike-smb2-0.4.0a5/buildwheel/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/buildwheel/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/buildwheel/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      487 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/buildwheel/wheel27.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 03:09:57.030028 pike-smb2-0.4.0a5/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/doc/class-hierarchy.dot
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/doc/container-model.dot
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/doc/object-model.dot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 03:09:57.030028 pike-smb2-0.4.0a5/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 03:09:57.030028 pike-smb2-0.4.0a5/doc/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/doc/source/_templates/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/doc/source/autosummary.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9471 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/doc/source/high_level.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/doc/source/model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/doc/source/open.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/doc/source/path.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/doc/source/pytest.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/doc/source/tree_connect.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 03:09:57.034028 pike-smb2-0.4.0a5/pykerb/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/pykerb/MakeKitBuild
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/pykerb/base64.c
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/pykerb/base64.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16691 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/pykerb/kerberos.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9825 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/pykerb/kerberos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/pykerb/kerberosbasic.c
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/pykerb/kerberosbasic.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28331 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/pykerb/kerberosgss.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/pykerb/kerberosgss.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4440 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/pykerb/kerberospw.c
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/pykerb/kerberospw.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 03:09:57.034028 pike-smb2-0.4.0a5/pykerb/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 03:09:57.034028 pike-smb2-0.4.0a5/pykerb/vendor/py3c/
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/pykerb/vendor/py3c/capsulethunk.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/pykerb/vendor/py3c/comparison.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/pykerb/vendor/py3c/compat.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/pykerb/vendor/py3c/fileshim.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/pykerb/vendor/py3c/py3shims.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/pykerb/vendor/py3c/tpflags.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/pykerb/vendor/py3c.h
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 03:09:57.034028 pike-smb2-0.4.0a5/samba/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/samba/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/samba/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/samba/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/samba/admin_password
+-rwxr-xr-x   0 runner    (1001) docker     (123)      164 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/samba/build_and_test_wheels.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      317 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/samba/build_and_test_wheels27.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      665 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/samba/dc.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/samba/docker-compose.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      333 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/samba/krb5.conf.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      323 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/samba/run_all.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/samba/share.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2022-12-21 03:09:57.042028 pike-smb2-0.4.0a5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1315 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 03:09:57.030028 pike-smb2-0.4.0a5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 03:09:57.038028 pike-smb2-0.4.0a5/src/pike/
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/src/pike/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/src/pike/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23725 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/src/pike/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11098 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/src/pike/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/src/pike/digest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/src/pike/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17920 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/src/pike/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81933 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/src/pike/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/src/pike/netbios.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25680 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/src/pike/ntlm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84326 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/src/pike/ntstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/src/pike/nttime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25417 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/src/pike/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/src/pike/pytest_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)   136885 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/src/pike/smb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 03:09:57.038028 pike-smb2-0.4.0a5/src/pike/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    27985 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/src/pike/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/src/pike/test/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6534 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/src/pike/test/appinstanceid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/src/pike/test/changenotify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5497 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/src/pike/test/compound.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44139 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/src/pike/test/copychunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23712 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/src/pike/test/credit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11364 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/src/pike/test/durable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/src/pike/test/echo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/src/pike/test/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/src/pike/test/invalid_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/src/pike/test/invalid_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/src/pike/test/ioctl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/src/pike/test/lease.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/src/pike/test/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/src/pike/test/multichannel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/src/pike/test/negotiate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/src/pike/test/oplock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10254 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/src/pike/test/persistent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/src/pike/test/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     5485 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/src/pike/test/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/src/pike/test/querydirectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6939 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/src/pike/test/queryondiskid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6705 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/src/pike/test/readwrite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/src/pike/test/reparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/src/pike/test/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/src/pike/test/set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/src/pike/test/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15036 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/src/pike/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 03:09:57.042028 pike-smb2-0.4.0a5/src/pike_smb2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10183 2022-12-21 03:09:56.000000 pike-smb2-0.4.0a5/src/pike_smb2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2022-12-21 03:09:57.000000 pike-smb2-0.4.0a5/src/pike_smb2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-21 03:09:56.000000 pike-smb2-0.4.0a5/src/pike_smb2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-21 03:09:56.000000 pike-smb2-0.4.0a5/src/pike_smb2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2022-12-21 03:09:56.000000 pike-smb2-0.4.0a5/src/pike_smb2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2022-12-21 03:09:56.000000 pike-smb2-0.4.0a5/src/pike_smb2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 03:09:57.042028 pike-smb2-0.4.0a5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9551 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/tests/test_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5385 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9406 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/tests/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18297 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/tests/test_smb3_encryption_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/tests/test_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2022-12-21 03:09:49.000000 pike-smb2-0.4.0a5/tox.ini
```

### Comparing `pike-smb2-0.4.0a4/.github/workflows/test_samba.yml` & `pike-smb2-0.4.0a5/.github/workflows/test_samba.yml`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/.github/workflows/wheels.yml` & `pike-smb2-0.4.0a5/.github/workflows/wheels.yml`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/LICENSE` & `pike-smb2-0.4.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/PKG-INFO` & `pike-smb2-0.4.0a5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pike-smb2
-Version: 0.4.0a4
-Summary: "Pure python SMB client"
+Version: 0.4.0a5
+Summary: Pure python SMB client
 Home-page: https://github.com/emc-isilon/pike
-Author: "Brian Koropoff"
-Author-email: "Brian.Koropoff@emc.com"
-Maintainer: "Masen Furer"
-Maintainer-email: "m_github@0x26.net"
+Author: Brian Koropoff
+Author-email: Brian.Koropoff@emc.com
+Maintainer: Masen Furer
+Maintainer-email: m_github@0x26.net
 License: Simplified BSD License
 Project-URL: Source, https://github.com/emc-isilon/pike
 Project-URL: Bug Reports, https://github.com/emc-isilon/pike/issues
 Keywords: smb,smb-testing,smb-client
 Platform: unix
 Platform: linux
 Platform: osx
@@ -83,15 +83,15 @@
 
     $ python -m pip install pike-smb2
 
 ## Build instructions
 
 Ubuntu 14.04 / 16.04
 
-    apt-get install -y --no-install-recommends krb5-user libkrb5-dev python-dev build-essential python2.7 python-pip py3c-dev
+    apt-get install -y --no-install-recommends krb5-user libkrb5-dev python-dev build-essential python2.7 python-pip
     pip install setuptools pycryptodomex
     python setup.py install
 
 ## Running tests
 
 The tests in the test subdirectory are ordinary Python unittest tests and
 can be run as usual.  The following environment variables are used by
```

### Comparing `pike-smb2-0.4.0a4/README.md` & `pike-smb2-0.4.0a5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
     $ python -m pip install pike-smb2
 
 ## Build instructions
 
 Ubuntu 14.04 / 16.04
 
-    apt-get install -y --no-install-recommends krb5-user libkrb5-dev python-dev build-essential python2.7 python-pip py3c-dev
+    apt-get install -y --no-install-recommends krb5-user libkrb5-dev python-dev build-essential python2.7 python-pip
     pip install setuptools pycryptodomex
     python setup.py install
 
 ## Running tests
 
 The tests in the test subdirectory are ordinary Python unittest tests and
 can be run as usual.  The following environment variables are used by
```

### Comparing `pike-smb2-0.4.0a4/doc/class-hierarchy.dot` & `pike-smb2-0.4.0a5/doc/class-hierarchy.dot`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/doc/source/_templates/module.rst` & `pike-smb2-0.4.0a5/doc/source/_templates/module.rst`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/doc/source/conf.py` & `pike-smb2-0.4.0a5/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/doc/source/index.rst` & `pike-smb2-0.4.0a5/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/doc/source/model.rst` & `pike-smb2-0.4.0a5/doc/source/model.rst`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/doc/source/pytest.rst` & `pike-smb2-0.4.0a5/doc/source/pytest.rst`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/pykerb/base64.c` & `pike-smb2-0.4.0a5/pykerb/base64.c`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/pykerb/base64.h` & `pike-smb2-0.4.0a5/pykerb/base64.h`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/pykerb/kerberos.c` & `pike-smb2-0.4.0a5/pykerb/kerberos.c`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/pykerb/kerberos.py` & `pike-smb2-0.4.0a5/pykerb/kerberos.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/pykerb/kerberosbasic.c` & `pike-smb2-0.4.0a5/pykerb/kerberosbasic.c`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/pykerb/kerberosbasic.h` & `pike-smb2-0.4.0a5/pykerb/kerberosbasic.h`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/pykerb/kerberosgss.c` & `pike-smb2-0.4.0a5/pykerb/kerberosgss.c`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/pykerb/kerberosgss.h` & `pike-smb2-0.4.0a5/pykerb/kerberosgss.h`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/pykerb/kerberospw.c` & `pike-smb2-0.4.0a5/pykerb/kerberospw.c`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/pykerb/kerberospw.h` & `pike-smb2-0.4.0a5/pykerb/kerberospw.h`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/pykerb/vendor/py3c/capsulethunk.h` & `pike-smb2-0.4.0a5/pykerb/vendor/py3c/capsulethunk.h`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/pykerb/vendor/py3c/comparison.h` & `pike-smb2-0.4.0a5/pykerb/vendor/py3c/comparison.h`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/pykerb/vendor/py3c/compat.h` & `pike-smb2-0.4.0a5/pykerb/vendor/py3c/compat.h`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/pykerb/vendor/py3c/fileshim.h` & `pike-smb2-0.4.0a5/pykerb/vendor/py3c/fileshim.h`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/pykerb/vendor/py3c/py3shims.h` & `pike-smb2-0.4.0a5/pykerb/vendor/py3c/py3shims.h`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/pykerb/vendor/py3c/tpflags.h` & `pike-smb2-0.4.0a5/pykerb/vendor/py3c/tpflags.h`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/pykerb/vendor/py3c.h` & `pike-smb2-0.4.0a5/pykerb/vendor/py3c.h`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/pyproject.toml` & `pike-smb2-0.4.0a5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/samba/README.md` & `pike-smb2-0.4.0a5/samba/README.md`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/samba/dc.sh` & `pike-smb2-0.4.0a5/samba/dc.sh`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/samba/docker-compose.yml` & `pike-smb2-0.4.0a5/samba/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/setup.cfg` & `pike-smb2-0.4.0a5/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [metadata]
 name = pike-smb2
-description = "Pure python SMB client"
+description = Pure python SMB client
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
-author = "Brian Koropoff"
-author_email = "Brian.Koropoff@emc.com"
-maintainer = "Masen Furer"
-maintainer_email = "m_github@0x26.net"
+author = Brian Koropoff
+author_email = Brian.Koropoff@emc.com
+maintainer = Masen Furer
+maintainer_email = m_github@0x26.net
 license = Simplified BSD License
 url = https://github.com/emc-isilon/pike
 project_urls = 
 	Source = https://github.com/emc-isilon/pike
 	Bug Reports = https://github.com/emc-isilon/pike/issues
 platforms = unix, linux, osx, cygwin, win32
 keywords = smb, smb-testing, smb-client
```

### Comparing `pike-smb2-0.4.0a4/setup.py` & `pike-smb2-0.4.0a5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     from setuptools import setup, Extension
 except ImportError:
     from distutils.core import setup, Extension
 from distutils.errors import CCompilerError, DistutilsExecError, DistutilsPlatformError
 
 _HERED = os.path.abspath(os.path.dirname(__file__))
 
-
 try:
     libgssapi_krb5 = ctypes.CDLL("libgssapi_krb5.so")
     defines = [
         ("HAVE_GSS_SET_CRED_OPTION", hasattr(libgssapi_krb5, "gss_set_cred_option")),
         (
             "HAVE_GSSSPI_SET_CRED_OPTION",
             hasattr(libgssapi_krb5, "gssspi_set_cred_option"),
```

### Comparing `pike-smb2-0.4.0a4/src/pike/__init__.py` & `pike-smb2-0.4.0a5/src/pike/__init__.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/src/pike/auth.py` & `pike-smb2-0.4.0a5/src/pike/auth.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/src/pike/core.py` & `pike-smb2-0.4.0a5/src/pike/core.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/src/pike/crypto.py` & `pike-smb2-0.4.0a5/src/pike/crypto.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/src/pike/digest.py` & `pike-smb2-0.4.0a5/src/pike/digest.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/src/pike/exceptions.py` & `pike-smb2-0.4.0a5/src/pike/exceptions.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/src/pike/io.py` & `pike-smb2-0.4.0a5/src/pike/io.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/src/pike/model.py` & `pike-smb2-0.4.0a5/src/pike/model.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/src/pike/netbios.py` & `pike-smb2-0.4.0a5/src/pike/netbios.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/src/pike/ntlm.py` & `pike-smb2-0.4.0a5/src/pike/ntlm.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/src/pike/ntstatus.py` & `pike-smb2-0.4.0a5/src/pike/ntstatus.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/src/pike/nttime.py` & `pike-smb2-0.4.0a5/src/pike/nttime.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/src/pike/path.py` & `pike-smb2-0.4.0a5/src/pike/path.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/src/pike/pytest_support.py` & `pike-smb2-0.4.0a5/src/pike/pytest_support.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/src/pike/smb2.py` & `pike-smb2-0.4.0a5/src/pike/smb2.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/src/pike/test/__init__.py` & `pike-smb2-0.4.0a5/src/pike/test/__init__.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/src/pike/test/acl.py` & `pike-smb2-0.4.0a5/src/pike/test/acl.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/src/pike/test/appinstanceid.py` & `pike-smb2-0.4.0a5/src/pike/test/appinstanceid.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/src/pike/test/changenotify.py` & `pike-smb2-0.4.0a5/src/pike/test/changenotify.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/src/pike/test/compound.py` & `pike-smb2-0.4.0a5/src/pike/test/compound.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/src/pike/test/copychunk.py` & `pike-smb2-0.4.0a5/src/pike/test/copychunk.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/src/pike/test/credit.py` & `pike-smb2-0.4.0a5/src/pike/test/credit.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/src/pike/test/durable.py` & `pike-smb2-0.4.0a5/src/pike/test/durable.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/src/pike/test/encryption.py` & `pike-smb2-0.4.0a5/src/pike/test/encryption.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/src/pike/test/invalid_session.py` & `pike-smb2-0.4.0a5/src/pike/test/invalid_session.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/src/pike/test/invalid_tree.py` & `pike-smb2-0.4.0a5/src/pike/test/invalid_tree.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/src/pike/test/ioctl.py` & `pike-smb2-0.4.0a5/src/pike/test/ioctl.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/src/pike/test/lease.py` & `pike-smb2-0.4.0a5/src/pike/test/lease.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/src/pike/test/lock.py` & `pike-smb2-0.4.0a5/src/pike/test/lock.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/src/pike/test/multichannel.py` & `pike-smb2-0.4.0a5/src/pike/test/multichannel.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/src/pike/test/negotiate.py` & `pike-smb2-0.4.0a5/src/pike/test/negotiate.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/src/pike/test/oplock.py` & `pike-smb2-0.4.0a5/src/pike/test/oplock.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/src/pike/test/persistent.py` & `pike-smb2-0.4.0a5/src/pike/test/persistent.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/src/pike/test/query.py` & `pike-smb2-0.4.0a5/src/pike/test/query.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/src/pike/test/querydirectory.py` & `pike-smb2-0.4.0a5/src/pike/test/querydirectory.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/src/pike/test/queryondiskid.py` & `pike-smb2-0.4.0a5/src/pike/test/queryondiskid.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/src/pike/test/readwrite.py` & `pike-smb2-0.4.0a5/src/pike/test/readwrite.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/src/pike/test/reparse.py` & `pike-smb2-0.4.0a5/src/pike/test/reparse.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/src/pike/test/session.py` & `pike-smb2-0.4.0a5/src/pike/test/session.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/src/pike/test/set.py` & `pike-smb2-0.4.0a5/src/pike/test/set.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/src/pike/transport.py` & `pike-smb2-0.4.0a5/src/pike/transport.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/src/pike_smb2.egg-info/PKG-INFO` & `pike-smb2-0.4.0a5/src/pike_smb2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pike-smb2
-Version: 0.4.0a4
-Summary: "Pure python SMB client"
+Version: 0.4.0a5
+Summary: Pure python SMB client
 Home-page: https://github.com/emc-isilon/pike
-Author: "Brian Koropoff"
-Author-email: "Brian.Koropoff@emc.com"
-Maintainer: "Masen Furer"
-Maintainer-email: "m_github@0x26.net"
+Author: Brian Koropoff
+Author-email: Brian.Koropoff@emc.com
+Maintainer: Masen Furer
+Maintainer-email: m_github@0x26.net
 License: Simplified BSD License
 Project-URL: Source, https://github.com/emc-isilon/pike
 Project-URL: Bug Reports, https://github.com/emc-isilon/pike/issues
 Keywords: smb,smb-testing,smb-client
 Platform: unix
 Platform: linux
 Platform: osx
@@ -83,15 +83,15 @@
 
     $ python -m pip install pike-smb2
 
 ## Build instructions
 
 Ubuntu 14.04 / 16.04
 
-    apt-get install -y --no-install-recommends krb5-user libkrb5-dev python-dev build-essential python2.7 python-pip py3c-dev
+    apt-get install -y --no-install-recommends krb5-user libkrb5-dev python-dev build-essential python2.7 python-pip
     pip install setuptools pycryptodomex
     python setup.py install
 
 ## Running tests
 
 The tests in the test subdirectory are ordinary Python unittest tests and
 can be run as usual.  The following environment variables are used by
```

### Comparing `pike-smb2-0.4.0a4/src/pike_smb2.egg-info/SOURCES.txt` & `pike-smb2-0.4.0a5/src/pike_smb2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/tests/test_auth.py` & `pike-smb2-0.4.0a5/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/tests/test_callbacks.py` & `pike-smb2-0.4.0a5/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/tests/test_client.py` & `pike-smb2-0.4.0a5/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/tests/test_io.py` & `pike-smb2-0.4.0a5/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/tests/test_path.py` & `pike-smb2-0.4.0a5/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/tests/test_smb3_encryption_vector.py` & `pike-smb2-0.4.0a5/tests/test_smb3_encryption_vector.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/tests/test_write.py` & `pike-smb2-0.4.0a5/tests/test_write.py`

 * *Files identical despite different names*

### Comparing `pike-smb2-0.4.0a4/tox.ini` & `pike-smb2-0.4.0a5/tox.ini`

 * *Files identical despite different names*

