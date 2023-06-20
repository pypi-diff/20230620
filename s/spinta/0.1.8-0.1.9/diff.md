# Comparing `tmp/spinta-0.1.8.tar.gz` & `tmp/spinta-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spinta-0.1.8.tar", last modified: Thu Jan 28 23:05:48 2021, max compression
+gzip compressed data, was "spinta-0.1.9.tar", last modified: Mon Feb  1 12:56:04 2021, max compression
```

## Comparing `spinta-0.1.8.tar` & `spinta-0.1.9.tar`

### file list

```diff
@@ -1,324 +1,327 @@
--rw-r--r--   0        0        0     1071 2019-05-30 05:53:10.268701 spinta-0.1.8/LICENSE
--rw-r--r--   0        0        0     1481 2019-05-30 05:53:10.268701 spinta-0.1.8/README.rst
--rw-r--r--   0        0        0     3020 2021-01-28 23:03:21.824151 spinta-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2019-02-02 03:22:22.999927 spinta-0.1.8/spinta/__init__.py
--rw-r--r--   0        0        0     2371 2020-09-10 09:42:58.151767 spinta-0.1.8/spinta/accesslog/__init__.py
--rw-r--r--   0        0        0     1749 2020-04-26 07:05:27.973123 spinta-0.1.8/spinta/accesslog/file.py
--rw-r--r--   0        0        0      866 2020-04-26 07:05:27.973123 spinta-0.1.8/spinta/accesslog/python.py
--rw-r--r--   0        0        0     6178 2020-12-10 12:04:26.583360 spinta-0.1.8/spinta/api.py
--rw-r--r--   0        0        0      635 2020-04-26 07:05:27.973123 spinta-0.1.8/spinta/asgi.py
--rw-r--r--   0        0        0    16110 2020-12-11 08:59:26.259953 spinta-0.1.8/spinta/auth.py
--rw-r--r--   0        0        0    31155 2020-12-08 12:43:51.513521 spinta-0.1.8/spinta/backends/__init__.py
--rw-r--r--   0        0        0      846 2021-01-20 18:14:31.603304 spinta-0.1.8/spinta/backends/components.py
--rw-r--r--   0        0        0        0 2020-04-26 07:05:27.976456 spinta-0.1.8/spinta/backends/fs/__init__.py
--rw-r--r--   0        0        0        0 2020-04-26 07:05:27.976456 spinta-0.1.8/spinta/backends/fs/commands/__init__.py
--rw-r--r--   0        0        0      234 2020-04-26 07:05:27.976456 spinta-0.1.8/spinta/backends/fs/commands/bootstrap.py
--rw-r--r--   0        0        0      555 2020-04-26 07:05:27.976456 spinta-0.1.8/spinta/backends/fs/commands/changes.py
--rw-r--r--   0        0        0      470 2020-04-26 07:05:27.976456 spinta-0.1.8/spinta/backends/fs/commands/decode.py
--rw-r--r--   0        0        0     1370 2020-04-26 07:05:27.976456 spinta-0.1.8/spinta/backends/fs/commands/encode.py
--rw-r--r--   0        0        0      778 2020-04-26 07:05:27.976456 spinta-0.1.8/spinta/backends/fs/commands/init.py
--rw-r--r--   0        0        0      338 2021-01-18 14:18:20.756589 spinta-0.1.8/spinta/backends/fs/commands/load.py
--rw-r--r--   0        0        0      309 2020-04-26 07:05:27.976456 spinta-0.1.8/spinta/backends/fs/commands/migrate.py
--rw-r--r--   0        0        0     1960 2020-04-26 07:05:27.976456 spinta-0.1.8/spinta/backends/fs/commands/read.py
--rw-r--r--   0        0        0     2455 2020-04-26 07:05:27.976456 spinta-0.1.8/spinta/backends/fs/commands/validate.py
--rw-r--r--   0        0        0      279 2021-01-21 12:02:21.049991 spinta-0.1.8/spinta/backends/fs/commands/wait.py
--rw-r--r--   0        0        0      629 2020-09-10 09:42:58.155100 spinta-0.1.8/spinta/backends/fs/commands/wipe.py
--rw-r--r--   0        0        0     3267 2020-09-10 09:42:58.155100 spinta-0.1.8/spinta/backends/fs/commands/write.py
--rw-r--r--   0        0        0      226 2021-01-21 12:02:21.039991 spinta-0.1.8/spinta/backends/fs/components.py
--rw-r--r--   0        0        0      716 2021-01-20 15:17:56.073284 spinta-0.1.8/spinta/backends/helpers.py
--rw-r--r--   0        0        0        0 2020-04-26 07:05:27.976456 spinta-0.1.8/spinta/backends/memory/__init__.py
--rw-r--r--   0        0        0        0 2020-04-26 07:05:27.976456 spinta-0.1.8/spinta/backends/memory/commands/__init__.py
--rw-r--r--   0        0        0        0 2020-04-26 07:05:27.976456 spinta-0.1.8/spinta/backends/memory/commands/auth.py
--rw-r--r--   0        0        0      226 2020-04-26 07:05:27.976456 spinta-0.1.8/spinta/backends/memory/commands/bootstrap.py
--rw-r--r--   0        0        0        0 2020-04-26 07:05:27.976456 spinta-0.1.8/spinta/backends/memory/commands/check.py
--rw-r--r--   0        0        0      301 2020-04-26 07:05:27.976456 spinta-0.1.8/spinta/backends/memory/commands/init.py
--rw-r--r--   0        0        0      289 2021-01-18 14:20:28.479922 spinta-0.1.8/spinta/backends/memory/commands/load.py
--rw-r--r--   0        0        0      610 2020-09-10 09:42:58.155100 spinta-0.1.8/spinta/backends/memory/commands/manifest.py
--rw-r--r--   0        0        0        0 2020-04-26 07:05:27.976456 spinta-0.1.8/spinta/backends/memory/commands/read.py
--rw-r--r--   0        0        0      246 2021-01-21 12:02:28.266657 spinta-0.1.8/spinta/backends/memory/commands/wait.py
--rw-r--r--   0        0        0      337 2021-01-07 20:21:35.063300 spinta-0.1.8/spinta/backends/memory/commands/wipe.py
--rw-r--r--   0        0        0        0 2020-04-26 07:05:27.976456 spinta-0.1.8/spinta/backends/memory/commands/write.py
--rw-r--r--   0        0        0      295 2021-01-20 17:45:43.893315 spinta-0.1.8/spinta/backends/memory/components.py
--rw-r--r--   0        0        0        0 2020-04-26 07:05:27.976456 spinta-0.1.8/spinta/backends/mongo/__init__.py
--rw-r--r--   0        0        0        0 2020-04-26 07:05:27.976456 spinta-0.1.8/spinta/backends/mongo/commands/__init__.py
--rw-r--r--   0        0        0      222 2020-04-26 07:05:27.976456 spinta-0.1.8/spinta/backends/mongo/commands/bootstrap.py
--rw-r--r--   0        0        0     1210 2020-04-26 07:05:27.976456 spinta-0.1.8/spinta/backends/mongo/commands/changes.py
--rw-r--r--   0        0        0      495 2020-04-26 07:05:27.976456 spinta-0.1.8/spinta/backends/mongo/commands/encode.py
--rw-r--r--   0        0        0      364 2020-09-10 09:42:58.155100 spinta-0.1.8/spinta/backends/mongo/commands/freeze.py
--rw-r--r--   0        0        0      358 2020-04-26 07:05:27.976456 spinta-0.1.8/spinta/backends/mongo/commands/init.py
--rw-r--r--   0        0        0      494 2021-01-18 14:20:28.509922 spinta-0.1.8/spinta/backends/mongo/commands/load.py
--rw-r--r--   0        0        0      297 2020-04-26 07:05:27.976456 spinta-0.1.8/spinta/backends/mongo/commands/migrate.py
--rw-r--r--   0        0        0    14655 2021-01-15 13:53:43.219944 spinta-0.1.8/spinta/backends/mongo/commands/query.py
--rw-r--r--   0        0        0     5655 2020-09-10 09:42:58.155100 spinta-0.1.8/spinta/backends/mongo/commands/read.py
--rw-r--r--   0        0        0     1528 2020-04-26 07:05:27.976456 spinta-0.1.8/spinta/backends/mongo/commands/validate.py
--rw-r--r--   0        0        0      284 2021-01-21 12:02:39.533324 spinta-0.1.8/spinta/backends/mongo/commands/wait.py
--rw-r--r--   0        0        0      782 2021-01-07 20:21:57.893299 spinta-0.1.8/spinta/backends/mongo/commands/wipe.py
--rw-r--r--   0        0        0     4105 2020-09-10 09:42:58.155100 spinta-0.1.8/spinta/backends/mongo/commands/write.py
--rw-r--r--   0        0        0     1908 2021-01-20 17:45:43.886648 spinta-0.1.8/spinta/backends/mongo/components.py
--rw-r--r--   0        0        0      250 2020-04-26 07:05:27.979790 spinta-0.1.8/spinta/backends/mongo/helpers.py
--rw-r--r--   0        0        0        0 2020-04-26 07:05:27.979790 spinta-0.1.8/spinta/backends/mongo/types/__init__.py
--rw-r--r--   0        0        0        0 2020-04-26 07:05:27.979790 spinta-0.1.8/spinta/backends/mongo/types/array/__init__.py
--rw-r--r--   0        0        0      694 2020-04-26 07:05:27.979790 spinta-0.1.8/spinta/backends/mongo/types/array/write.py
--rw-r--r--   0        0        0        0 2020-04-26 07:05:27.979790 spinta-0.1.8/spinta/backends/mongo/types/file/__init__.py
--rw-r--r--   0        0        0      965 2020-04-26 07:05:27.979790 spinta-0.1.8/spinta/backends/mongo/types/file/write.py
--rw-r--r--   0        0        0        0 2020-04-26 07:05:27.979790 spinta-0.1.8/spinta/backends/mongo/types/object/__init__.py
--rw-r--r--   0        0        0      793 2020-04-26 07:05:27.979790 spinta-0.1.8/spinta/backends/mongo/types/object/write.py
--rw-r--r--   0        0        0        0 2020-04-26 07:05:27.979790 spinta-0.1.8/spinta/backends/postgresql/__init__.py
--rw-r--r--   0        0        0        0 2020-04-26 07:05:27.979790 spinta-0.1.8/spinta/backends/postgresql/commands/__init__.py
--rw-r--r--   0        0        0      558 2020-04-26 07:05:27.979790 spinta-0.1.8/spinta/backends/postgresql/commands/bootstrap.py
--rw-r--r--   0        0        0     3531 2020-04-26 07:05:27.979790 spinta-0.1.8/spinta/backends/postgresql/commands/changes.py
--rw-r--r--   0        0        0     1489 2020-04-26 07:05:27.979790 spinta-0.1.8/spinta/backends/postgresql/commands/encode.py
--rw-r--r--   0        0        0     5868 2020-09-10 09:42:58.155100 spinta-0.1.8/spinta/backends/postgresql/commands/freeze.py
--rw-r--r--   0        0        0     3344 2020-04-26 07:05:27.979790 spinta-0.1.8/spinta/backends/postgresql/commands/init.py
--rw-r--r--   0        0        0        0 2020-04-26 07:05:27.979790 spinta-0.1.8/spinta/backends/postgresql/commands/link.py
--rw-r--r--   0        0        0      841 2021-01-18 14:21:03.739921 spinta-0.1.8/spinta/backends/postgresql/commands/load.py
--rw-r--r--   0        0        0     1879 2020-09-10 09:42:58.155100 spinta-0.1.8/spinta/backends/postgresql/commands/manifest.py
--rw-r--r--   0        0        0     1209 2021-01-19 06:59:24.266647 spinta-0.1.8/spinta/backends/postgresql/commands/migrate.py
--rw-r--r--   0        0        0    27508 2020-12-11 10:35:03.219921 spinta-0.1.8/spinta/backends/postgresql/commands/query.py
--rw-r--r--   0        0        0     3928 2020-09-10 09:42:58.155100 spinta-0.1.8/spinta/backends/postgresql/commands/read.py
--rw-r--r--   0        0        0      615 2020-04-26 07:05:27.979790 spinta-0.1.8/spinta/backends/postgresql/commands/validate.py
--rw-r--r--   0        0        0      700 2021-01-21 12:01:18.356658 spinta-0.1.8/spinta/backends/postgresql/commands/wait.py
--rw-r--r--   0        0        0     1335 2021-01-07 20:22:33.623299 spinta-0.1.8/spinta/backends/postgresql/commands/wipe.py
--rw-r--r--   0        0        0     3823 2020-04-26 07:05:27.979790 spinta-0.1.8/spinta/backends/postgresql/commands/write.py
--rw-r--r--   0        0        0     4219 2021-01-20 17:44:29.493315 spinta-0.1.8/spinta/backends/postgresql/components.py
--rw-r--r--   0        0        0      411 2020-04-26 07:05:27.979790 spinta-0.1.8/spinta/backends/postgresql/constants.py
--rw-r--r--   0        0        0     6472 2020-03-26 09:03:44.213110 spinta-0.1.8/spinta/backends/postgresql/files.py
--rw-r--r--   0        0        0     1430 2020-09-10 09:42:58.155100 spinta-0.1.8/spinta/backends/postgresql/helpers/__init__.py
--rw-r--r--   0        0        0     1704 2020-04-26 07:05:27.986456 spinta-0.1.8/spinta/backends/postgresql/helpers/changes.py
--rw-r--r--   0        0        0      706 2020-04-26 07:05:27.986456 spinta-0.1.8/spinta/backends/postgresql/helpers/manifest.py
--rw-r--r--   0        0        0     1096 2020-04-26 07:05:27.986456 spinta-0.1.8/spinta/backends/postgresql/helpers/validate.py
--rw-r--r--   0        0        0      304 2020-04-26 07:05:27.986456 spinta-0.1.8/spinta/backends/postgresql/sqlalchemy.py
--rw-r--r--   0        0        0        0 2020-04-26 07:05:27.986456 spinta-0.1.8/spinta/backends/postgresql/types/__init__.py
--rw-r--r--   0        0        0        0 2020-04-26 07:05:27.986456 spinta-0.1.8/spinta/backends/postgresql/types/array/__init__.py
--rw-r--r--   0        0        0     2266 2020-09-10 09:42:58.155100 spinta-0.1.8/spinta/backends/postgresql/types/array/freeze.py
--rw-r--r--   0        0        0     1985 2020-04-26 07:05:27.986456 spinta-0.1.8/spinta/backends/postgresql/types/array/init.py
--rw-r--r--   0        0        0      541 2021-01-07 20:22:49.246633 spinta-0.1.8/spinta/backends/postgresql/types/array/wipe.py
--rw-r--r--   0        0        0     4287 2020-04-26 07:05:27.986456 spinta-0.1.8/spinta/backends/postgresql/types/array/write.py
--rw-r--r--   0        0        0        0 2020-04-26 07:05:27.986456 spinta-0.1.8/spinta/backends/postgresql/types/file/__init__.py
--rw-r--r--   0        0        0     3019 2020-09-10 09:42:58.155100 spinta-0.1.8/spinta/backends/postgresql/types/file/freeze.py
--rw-r--r--   0        0        0     2022 2020-04-26 07:05:27.986456 spinta-0.1.8/spinta/backends/postgresql/types/file/init.py
--rw-r--r--   0        0        0     4164 2020-04-26 07:05:27.986456 spinta-0.1.8/spinta/backends/postgresql/types/file/read.py
--rw-r--r--   0        0        0     4585 2020-04-26 07:05:27.986456 spinta-0.1.8/spinta/backends/postgresql/types/file/write.py
--rw-r--r--   0        0        0        0 2020-04-26 07:05:27.986456 spinta-0.1.8/spinta/backends/postgresql/types/object/__init__.py
--rw-r--r--   0        0        0     1634 2020-09-10 09:42:58.155100 spinta-0.1.8/spinta/backends/postgresql/types/object/freeze.py
--rw-r--r--   0        0        0      665 2020-04-26 07:05:27.986456 spinta-0.1.8/spinta/backends/postgresql/types/object/init.py
--rw-r--r--   0        0        0     2545 2020-04-26 07:05:27.986456 spinta-0.1.8/spinta/backends/postgresql/types/object/read.py
--rw-r--r--   0        0        0      373 2021-01-07 20:22:12.533300 spinta-0.1.8/spinta/backends/postgresql/types/object/wipe.py
--rw-r--r--   0        0        0        0 2020-04-26 07:05:27.986456 spinta-0.1.8/spinta/backends/postgresql/types/ref/__init__.py
--rw-r--r--   0        0        0     2030 2020-09-10 09:42:58.155100 spinta-0.1.8/spinta/backends/postgresql/types/ref/freeze.py
--rw-r--r--   0        0        0     1230 2020-04-26 07:05:27.986456 spinta-0.1.8/spinta/backends/postgresql/types/ref/init.py
--rw-r--r--   0        0        0      661 2020-04-26 07:05:27.986456 spinta-0.1.8/spinta/backends/postgresql/types/ref/validate.py
--rw-r--r--   0        0        0     6955 2021-01-26 08:12:54.683294 spinta-0.1.8/spinta/backends/s3.py
--rw-r--r--   0        0        0        0 2021-01-21 08:40:26.719976 spinta-0.1.8/spinta/cli/__init__.py
--rw-r--r--   0        0        0     3640 2021-01-25 16:14:06.659794 spinta-0.1.8/spinta/cli/auth.py
--rw-r--r--   0        0        0      636 2021-01-21 09:52:47.733285 spinta-0.1.8/spinta/cli/config.py
--rw-r--r--   0        0        0     1240 2021-01-21 10:04:33.656615 spinta-0.1.8/spinta/cli/data.py
--rw-r--r--   0        0        0        0 2020-12-28 10:05:48.744968 spinta-0.1.8/spinta/cli/helpers/__init__.py
--rw-r--r--   0        0        0      898 2020-12-28 10:13:57.328306 spinta-0.1.8/spinta/cli/helpers/auth.py
--rw-r--r--   0        0        0     3181 2021-01-21 10:01:12.119949 spinta-0.1.8/spinta/cli/helpers/data.py
--rw-r--r--   0        0        0      891 2020-12-30 11:57:09.046687 spinta-0.1.8/spinta/cli/helpers/store.py
--rw-r--r--   0        0        0      285 2021-01-21 10:35:03.059938 spinta-0.1.8/spinta/cli/helpers/typer.py
--rw-r--r--   0        0        0     3057 2021-01-27 13:10:34.016628 spinta-0.1.8/spinta/cli/inspect.py
--rw-r--r--   0        0        0     2342 2021-01-25 16:19:02.756459 spinta-0.1.8/spinta/cli/main.py
--rw-r--r--   0        0        0     2990 2021-01-25 20:47:27.399948 spinta-0.1.8/spinta/cli/manifest.py
--rw-r--r--   0        0        0     1794 2021-01-21 10:15:32.293278 spinta-0.1.8/spinta/cli/migrate.py
--rw-r--r--   0        0        0     7052 2021-01-21 10:33:35.233272 spinta-0.1.8/spinta/cli/pii.py
--rw-r--r--   0        0        0     3562 2021-01-21 10:48:31.516600 spinta-0.1.8/spinta/cli/pull.py
--rw-r--r--   0        0        0    10016 2021-01-21 11:47:28.626662 spinta-0.1.8/spinta/cli/push.py
--rw-r--r--   0        0        0      956 2021-01-21 12:41:32.606644 spinta-0.1.8/spinta/cli/server.py
--rw-r--r--   0        0        0    13461 2021-01-21 12:40:59.896644 spinta-0.1.8/spinta/commands/__init__.py
--rw-r--r--   0        0        0      532 2020-09-10 09:42:58.155100 spinta-0.1.8/spinta/commands/auth.py
--rw-r--r--   0        0        0      280 2020-03-26 14:28:49.946654 spinta-0.1.8/spinta/commands/formats/__init__.py
--rw-r--r--   0        0        0     3090 2020-04-26 07:05:27.986456 spinta-0.1.8/spinta/commands/formats/ascii.py
--rw-r--r--   0        0        0     1658 2020-12-10 16:26:20.303337 spinta-0.1.8/spinta/commands/formats/csv.py
--rw-r--r--   0        0        0    10459 2020-12-11 09:48:32.916603 spinta-0.1.8/spinta/commands/formats/html.py
--rw-r--r--   0        0        0     2082 2020-09-10 09:42:58.155100 spinta-0.1.8/spinta/commands/formats/json.py
--rw-r--r--   0        0        0     1529 2020-04-26 07:05:27.986456 spinta-0.1.8/spinta/commands/formats/jsonl.py
--rw-r--r--   0        0        0      894 2019-05-01 06:33:24.263673 spinta-0.1.8/spinta/commands/helpers.py
--rw-r--r--   0        0        0     1324 2020-04-26 07:05:27.986456 spinta-0.1.8/spinta/commands/read.py
--rw-r--r--   0        0        0     3111 2020-04-26 07:05:27.986456 spinta-0.1.8/spinta/commands/search.py
--rw-r--r--   0        0        0      605 2020-04-26 07:05:27.986456 spinta-0.1.8/spinta/commands/version.py
--rw-r--r--   0        0        0    34083 2021-01-07 20:23:22.399966 spinta-0.1.8/spinta/commands/write.py
--rw-r--r--   0        0        0     1637 2020-12-08 12:43:51.353521 spinta-0.1.8/spinta/compat.py
--rw-r--r--   0        0        0    22840 2021-01-21 10:06:15.496614 spinta-0.1.8/spinta/components.py
--rw-r--r--   0        0        0     9569 2021-01-27 07:42:44.779958 spinta-0.1.8/spinta/config.py
--rw-r--r--   0        0        0     2754 2021-01-21 09:24:23.033295 spinta-0.1.8/spinta/config.yml
--rw-r--r--   0        0        0        0 2020-03-21 10:14:12.239947 spinta-0.1.8/spinta/core/__init__.py
--rw-r--r--   0        0        0      967 2020-09-10 09:42:58.158434 spinta-0.1.8/spinta/core/access.py
--rw-r--r--   0        0        0    13956 2021-01-21 08:49:51.656640 spinta-0.1.8/spinta/core/config.py
--rw-r--r--   0        0        0     1430 2021-01-26 20:00:10.906601 spinta-0.1.8/spinta/core/context.py
--rw-r--r--   0        0        0      816 2021-01-21 14:26:38.269942 spinta-0.1.8/spinta/core/enums.py
--rw-r--r--   0        0        0     7407 2020-12-08 12:43:51.353521 spinta-0.1.8/spinta/core/ufuncs.py
--rw-r--r--   0        0        0        0 2020-04-26 07:05:27.986456 spinta-0.1.8/spinta/datasets/__init__.py
--rw-r--r--   0        0        0        0 2020-04-26 07:05:27.986456 spinta-0.1.8/spinta/datasets/backends/__init__.py
--rw-r--r--   0        0        0        0 2020-04-26 07:05:27.986456 spinta-0.1.8/spinta/datasets/backends/csv/__init__.py
--rw-r--r--   0        0        0     1681 2021-01-18 14:21:37.686588 spinta-0.1.8/spinta/datasets/backends/csv/commands.py
--rw-r--r--   0        0        0      207 2020-04-26 07:05:27.986456 spinta-0.1.8/spinta/datasets/backends/csv/components.py
--rw-r--r--   0        0        0        0 2021-01-20 16:56:30.636664 spinta-0.1.8/spinta/datasets/backends/frictionless/__init__.py
--rw-r--r--   0        0        0        0 2021-01-20 16:56:30.626664 spinta-0.1.8/spinta/datasets/backends/frictionless/commands/__init__.py
--rw-r--r--   0        0        0      363 2021-01-20 17:09:34.603327 spinta-0.1.8/spinta/datasets/backends/frictionless/commands/load.py
--rw-r--r--   0        0        0      308 2021-01-25 15:52:35.836468 spinta-0.1.8/spinta/datasets/backends/frictionless/commands/wait.py
--rw-r--r--   0        0        0      348 2021-01-20 17:38:22.756651 spinta-0.1.8/spinta/datasets/backends/frictionless/commands/wipe.py
--rw-r--r--   0        0        0      110 2021-01-20 17:08:52.959994 spinta-0.1.8/spinta/datasets/backends/frictionless/components.py
--rw-r--r--   0        0        0        0 2020-04-26 07:05:27.986456 spinta-0.1.8/spinta/datasets/backends/sql/__init__.py
--rw-r--r--   0        0        0        0 2021-01-08 10:36:18.803259 spinta-0.1.8/spinta/datasets/backends/sql/commands/__init__.py
--rw-r--r--   0        0        0      223 2021-01-19 07:15:19.473309 spinta-0.1.8/spinta/datasets/backends/sql/commands/bootstrap.py
--rw-r--r--   0        0        0      507 2021-01-19 07:15:19.493309 spinta-0.1.8/spinta/datasets/backends/sql/commands/init.py
--rw-r--r--   0        0        0     4220 2021-01-26 20:51:04.526584 spinta-0.1.8/spinta/datasets/backends/sql/commands/inspect.py
--rw-r--r--   0        0        0      496 2021-01-18 14:22:24.283254 spinta-0.1.8/spinta/datasets/backends/sql/commands/load.py
--rw-r--r--   0        0        0    22238 2020-12-17 16:12:51.809815 spinta-0.1.8/spinta/datasets/backends/sql/commands/query.py
--rw-r--r--   0        0        0     3175 2021-01-18 13:53:52.373264 spinta-0.1.8/spinta/datasets/backends/sql/commands/read.py
--rw-r--r--   0        0        0      673 2021-01-19 07:15:19.506642 spinta-0.1.8/spinta/datasets/backends/sql/commands/wait.py
--rw-r--r--   0        0        0     1507 2021-01-07 20:18:11.676634 spinta-0.1.8/spinta/datasets/backends/sql/components.py
--rw-r--r--   0        0        0        0 2021-01-27 07:43:53.063291 spinta-0.1.8/spinta/datasets/backends/sqldump/__init__.py
--rw-r--r--   0        0        0        0 2021-01-27 07:45:51.933290 spinta-0.1.8/spinta/datasets/backends/sqldump/commands/__init__.py
--rw-r--r--   0        0        0     3235 2021-01-27 17:42:10.096891 spinta-0.1.8/spinta/datasets/backends/sqldump/commands/inspect.py
--rw-r--r--   0        0        0      537 2021-01-27 17:39:41.500216 spinta-0.1.8/spinta/datasets/backends/sqldump/commands/load.py
--rw-r--r--   0        0        0      588 2021-01-27 17:41:32.503556 spinta-0.1.8/spinta/datasets/backends/sqldump/components.py
--rw-r--r--   0        0        0        0 2021-01-27 14:43:29.126271 spinta-0.1.8/spinta/datasets/backends/sqldump/ufuncs/__init__.py
--rw-r--r--   0        0        0      364 2021-01-27 17:24:28.216830 spinta-0.1.8/spinta/datasets/backends/sqldump/ufuncs/components.py
--rw-r--r--   0        0        0      698 2021-01-27 17:47:46.256911 spinta-0.1.8/spinta/datasets/backends/sqldump/ufuncs/ufuncs.py
--rw-r--r--   0        0        0        0 2020-04-26 07:05:27.986456 spinta-0.1.8/spinta/datasets/commands/__init__.py
--rw-r--r--   0        0        0      376 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/datasets/commands/check.py
--rw-r--r--   0        0        0      939 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/datasets/commands/error.py
--rw-r--r--   0        0        0      319 2021-01-20 13:23:47.033323 spinta-0.1.8/spinta/datasets/commands/inspect.py
--rw-r--r--   0        0        0     1954 2020-12-17 20:02:03.593070 spinta-0.1.8/spinta/datasets/commands/link.py
--rw-r--r--   0        0        0     2280 2021-01-27 17:00:22.843413 spinta-0.1.8/spinta/datasets/commands/load.py
--rw-r--r--   0        0        0     1266 2020-12-08 12:43:51.353521 spinta-0.1.8/spinta/datasets/commands/read.py
--rw-r--r--   0        0        0      327 2021-01-07 20:23:41.829966 spinta-0.1.8/spinta/datasets/commands/wipe.py
--rw-r--r--   0        0        0     4968 2021-01-27 13:15:37.956626 spinta-0.1.8/spinta/datasets/components.py
--rw-r--r--   0        0        0      452 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/datasets/enums.py
--rw-r--r--   0        0        0     2119 2021-01-20 15:17:56.089951 spinta-0.1.8/spinta/datasets/helpers.py
--rw-r--r--   0        0        0        0 2020-09-10 09:42:58.158434 spinta-0.1.8/spinta/datasets/keymaps/__init__.py
--rw-r--r--   0        0        0      305 2020-09-10 09:42:58.158434 spinta-0.1.8/spinta/datasets/keymaps/components.py
--rw-r--r--   0        0        0     3062 2020-12-08 12:43:51.553521 spinta-0.1.8/spinta/datasets/keymaps/sqlalchemy.py
--rw-r--r--   0        0        0       81 2020-09-10 09:42:58.158434 spinta-0.1.8/spinta/datasets/utils.py
--rw-r--r--   0        0        0        0 2020-12-20 10:53:38.389942 spinta-0.1.8/spinta/dimensions/__init__.py
--rw-r--r--   0        0        0        0 2020-12-20 11:00:17.646606 spinta-0.1.8/spinta/dimensions/commands/__init__.py
--rw-r--r--   0        0        0      462 2020-12-20 13:01:32.526657 spinta-0.1.8/spinta/dimensions/commands/load.py
--rw-r--r--   0        0        0        0 2020-12-20 12:58:25.826658 spinta-0.1.8/spinta/dimensions/prefix/__init__.py
--rw-r--r--   0        0        0      618 2021-01-07 20:18:11.676634 spinta-0.1.8/spinta/dimensions/prefix/components.py
--rw-r--r--   0        0        0      978 2020-12-20 13:14:48.746652 spinta-0.1.8/spinta/dimensions/prefix/helpers.py
--rw-r--r--   0        0        0     3825 2020-12-30 11:19:49.503333 spinta-0.1.8/spinta/dispatcher.py
--rw-r--r--   0        0        0    11623 2021-01-27 17:16:21.313468 spinta-0.1.8/spinta/exceptions.py
--rw-r--r--   0        0        0     1331 2020-03-26 14:28:49.946654 spinta-0.1.8/spinta/fetcher.py
--rw-r--r--   0        0        0        0 2020-01-11 09:17:03.093164 spinta-0.1.8/spinta/hacks/__init__.py
--rw-r--r--   0        0        0      900 2020-03-21 10:14:12.243281 spinta-0.1.8/spinta/hacks/spyna.py
--rw-r--r--   0        0        0     1676 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/manifest/_schema/version.yml
--rw-r--r--   0        0        0     1110 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/manifest/_schema.yml
--rw-r--r--   0        0        0     1205 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/manifest/_txn.yml
--rw-r--r--   0        0        0        0 2020-03-21 10:14:12.243281 spinta-0.1.8/spinta/manifests/__init__.py
--rw-r--r--   0        0        0        0 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/manifests/backend/__init__.py
--rw-r--r--   0        0        0        0 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/manifests/backend/commands/__init__.py
--rw-r--r--   0        0        0      608 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/manifests/backend/commands/bootstrap.py
--rw-r--r--   0        0        0      256 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/manifests/backend/commands/configure.py
--rw-r--r--   0        0        0      378 2020-09-10 09:42:58.158434 spinta-0.1.8/spinta/manifests/backend/commands/freeze.py
--rw-r--r--   0        0        0      539 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/manifests/backend/commands/load.py
--rw-r--r--   0        0        0     1402 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/manifests/backend/commands/manifest.py
--rw-r--r--   0        0        0      589 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/manifests/backend/commands/migrate.py
--rw-r--r--   0        0        0      712 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/manifests/backend/commands/sync.py
--rw-r--r--   0        0        0       93 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/manifests/backend/components.py
--rw-r--r--   0        0        0     8173 2021-01-07 20:18:11.676634 spinta-0.1.8/spinta/manifests/backend/helpers.py
--rw-r--r--   0        0        0        0 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/manifests/commands/__init__.py
--rw-r--r--   0        0        0      675 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/manifests/commands/check.py
--rw-r--r--   0        0        0      993 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/manifests/commands/error.py
--rw-r--r--   0        0        0      430 2020-09-10 09:42:58.158434 spinta-0.1.8/spinta/manifests/commands/init.py
--rw-r--r--   0        0        0      314 2021-01-20 12:27:03.219899 spinta-0.1.8/spinta/manifests/commands/inspect.py
--rw-r--r--   0        0        0      437 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/manifests/commands/link.py
--rw-r--r--   0        0        0     2120 2021-01-21 08:09:45.639987 spinta-0.1.8/spinta/manifests/components.py
--rw-r--r--   0        0        0     4916 2021-01-26 20:25:44.239926 spinta-0.1.8/spinta/manifests/helpers.py
--rw-r--r--   0        0        0        0 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/manifests/internal/__init__.py
--rw-r--r--   0        0        0        0 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/manifests/internal/commands/__init__.py
--rw-r--r--   0        0        0      479 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/manifests/internal/commands/configure.py
--rw-r--r--   0        0        0     1660 2020-09-10 09:42:58.158434 spinta-0.1.8/spinta/manifests/internal/commands/load.py
--rw-r--r--   0        0        0      107 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/manifests/internal/components.py
--rw-r--r--   0        0        0        0 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/manifests/tabular/__init__.py
--rw-r--r--   0        0        0        0 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/manifests/tabular/commands/__init__.py
--rw-r--r--   0        0        0      438 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/manifests/tabular/commands/bootstrap.py
--rw-r--r--   0        0        0      595 2021-01-26 08:03:38.269964 spinta-0.1.8/spinta/manifests/tabular/commands/configure.py
--rw-r--r--   0        0        0     1610 2021-01-26 08:07:08.613296 spinta-0.1.8/spinta/manifests/tabular/commands/load.py
--rw-r--r--   0        0        0       93 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/manifests/tabular/components.py
--rw-r--r--   0        0        0      218 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/manifests/tabular/constants.py
--rw-r--r--   0        0        0    23498 2021-01-27 13:17:21.486626 spinta-0.1.8/spinta/manifests/tabular/helpers.py
--rw-r--r--   0        0        0        0 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/manifests/yaml/__init__.py
--rw-r--r--   0        0        0        0 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/manifests/yaml/commands/__init__.py
--rw-r--r--   0        0        0      423 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/manifests/yaml/commands/bootstrap.py
--rw-r--r--   0        0        0      478 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/manifests/yaml/commands/configure.py
--rw-r--r--   0        0        0     2051 2020-09-10 09:42:58.158434 spinta-0.1.8/spinta/manifests/yaml/commands/freeze.py
--rw-r--r--   0        0        0     1812 2020-09-10 09:42:58.158434 spinta-0.1.8/spinta/manifests/yaml/commands/load.py
--rw-r--r--   0        0        0     1327 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/manifests/yaml/commands/manifest.py
--rw-r--r--   0        0        0      360 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/manifests/yaml/commands/migrate.py
--rw-r--r--   0        0        0      313 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/manifests/yaml/commands/sync.py
--rw-r--r--   0        0        0       90 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/manifests/yaml/components.py
--rw-r--r--   0        0        0     4079 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/manifests/yaml/helpers.py
--rw-r--r--   0        0        0        0 2019-05-01 06:33:24.263673 spinta-0.1.8/spinta/methods.py
--rw-r--r--   0        0        0     1138 2020-12-10 12:18:59.933368 spinta-0.1.8/spinta/middlewares.py
--rw-r--r--   0        0        0      660 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-03-21 10:14:12.243281 spinta-0.1.8/spinta/migrations/schema/__init__.py
--rw-r--r--   0        0        0     2847 2020-09-10 09:42:58.158434 spinta-0.1.8/spinta/migrations/schema/alembic.py
--rw-r--r--   0        0        0     5950 2020-12-20 13:12:52.643320 spinta-0.1.8/spinta/nodes.py
--rw-r--r--   0        0        0      659 2020-01-11 09:17:03.096498 spinta-0.1.8/spinta/renderer.py
--rw-r--r--   0        0        0     8514 2020-09-10 09:42:58.161767 spinta-0.1.8/spinta/spyna.py
--rw-r--r--   0        0        0     3500 2020-01-11 09:17:03.096498 spinta-0.1.8/spinta/templates/base.html
--rw-r--r--   0        0        0      178 2020-01-11 09:17:03.096498 spinta-0.1.8/spinta/templates/error.html
--rw-r--r--   0        0        0       50 2019-05-01 06:33:24.263673 spinta-0.1.8/spinta/testing/__init__.py
--rw-r--r--   0        0        0     1753 2021-01-27 11:54:47.086654 spinta-0.1.8/spinta/testing/cli.py
--rw-r--r--   0        0        0     5859 2020-09-10 09:42:58.161767 spinta-0.1.8/spinta/testing/client.py
--rw-r--r--   0        0        0     2656 2021-01-26 08:39:54.229952 spinta-0.1.8/spinta/testing/config.py
--rw-r--r--   0        0        0     2800 2021-01-26 19:53:16.539937 spinta-0.1.8/spinta/testing/context.py
--rw-r--r--   0        0        0      236 2020-09-11 07:31:45.943388 spinta-0.1.8/spinta/testing/csv.py
--rw-r--r--   0        0        0     2126 2020-12-08 12:43:51.356854 spinta-0.1.8/spinta/testing/data.py
--rw-r--r--   0        0        0     1446 2021-01-21 13:28:21.726628 spinta-0.1.8/spinta/testing/datasets.py
--rw-r--r--   0        0        0     5544 2020-09-10 09:42:58.161767 spinta-0.1.8/spinta/testing/dtypes.py
--rw-r--r--   0        0        0        0 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/testing/manifest.py
--rw-r--r--   0        0        0     5448 2021-01-27 11:42:16.086658 spinta-0.1.8/spinta/testing/pytest.py
--rw-r--r--   0        0        0     3393 2021-01-26 19:44:12.049940 spinta-0.1.8/spinta/testing/tabular.py
--rw-r--r--   0        0        0      769 2020-03-21 10:14:12.246614 spinta-0.1.8/spinta/testing/ufuncs.py
--rw-r--r--   0        0        0     4995 2020-09-10 09:42:58.161767 spinta-0.1.8/spinta/testing/utils.py
--rw-r--r--   0        0        0        0 2019-06-14 18:23:09.532354 spinta-0.1.8/spinta/types/__init__.py
--rw-r--r--   0        0        0        0 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/types/array/__init__.py
--rw-r--r--   0        0        0      411 2021-01-07 20:18:11.676634 spinta-0.1.8/spinta/types/array/link.py
--rw-r--r--   0        0        0      973 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/types/command.py
--rw-r--r--   0        0        0     2948 2020-09-10 09:42:58.161767 spinta-0.1.8/spinta/types/config.py
--rw-r--r--   0        0        0     9575 2021-01-07 20:18:11.676634 spinta-0.1.8/spinta/types/datatype.py
--rw-r--r--   0        0        0        0 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/types/file/__init__.py
--rw-r--r--   0        0        0     1039 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/types/file/decode.py
--rw-r--r--   0        0        0     1070 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/types/file/helpers.py
--rw-r--r--   0        0        0      919 2021-01-26 19:02:09.116621 spinta-0.1.8/spinta/types/helpers.py
--rw-r--r--   0        0        0     9141 2021-01-20 18:31:24.789965 spinta-0.1.8/spinta/types/model.py
--rw-r--r--   0        0        0     8732 2021-01-20 17:46:21.926648 spinta-0.1.8/spinta/types/namespace.py
--rw-r--r--   0        0        0        0 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/types/object/__init__.py
--rw-r--r--   0        0        0      367 2021-01-07 20:18:11.679967 spinta-0.1.8/spinta/types/object/link.py
--rw-r--r--   0        0        0     1022 2020-09-10 09:42:58.161767 spinta-0.1.8/spinta/types/owner.py
--rw-r--r--   0        0        0     2420 2020-09-10 09:43:39.961767 spinta-0.1.8/spinta/types/project.py
--rw-r--r--   0        0        0        0 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/types/ref/__init__.py
--rw-r--r--   0        0        0     1367 2021-01-26 20:43:56.426586 spinta-0.1.8/spinta/types/ref/link.py
--rw-r--r--   0        0        0     4514 2021-01-25 16:00:46.789798 spinta-0.1.8/spinta/types/store.py
--rw-r--r--   0        0        0      764 2020-12-08 12:43:51.356854 spinta-0.1.8/spinta/ufuncs.py
--rw-r--r--   0        0        0     8342 2020-12-08 12:43:51.356854 spinta-0.1.8/spinta/urlparams.py
--rw-r--r--   0        0        0        0 2019-03-09 04:22:52.893518 spinta-0.1.8/spinta/utils/__init__.py
--rw-r--r--   0        0        0     1939 2020-04-26 07:05:27.993123 spinta-0.1.8/spinta/utils/aiotools.py
--rw-r--r--   0        0        0      345 2020-01-11 09:17:03.096498 spinta-0.1.8/spinta/utils/changes.py
--rw-r--r--   0        0        0      301 2020-09-10 09:42:58.161767 spinta-0.1.8/spinta/utils/config.py
--rw-r--r--   0        0        0     2554 2021-01-07 20:18:11.679967 spinta-0.1.8/spinta/utils/data.py
--rw-r--r--   0        0        0      444 2020-09-10 09:42:58.161767 spinta-0.1.8/spinta/utils/enums.py
--rw-r--r--   0        0        0      192 2020-01-11 09:17:03.096498 spinta-0.1.8/spinta/utils/errors.py
--rw-r--r--   0        0        0      373 2019-05-30 05:51:48.468805 spinta-0.1.8/spinta/utils/idgen.py
--rw-r--r--   0        0        0      342 2021-01-15 13:55:31.979943 spinta-0.1.8/spinta/utils/imports.py
--rw-r--r--   0        0        0     1926 2020-09-10 09:42:58.161767 spinta-0.1.8/spinta/utils/itertools.py
--rw-r--r--   0        0        0      730 2020-09-10 09:42:58.161767 spinta-0.1.8/spinta/utils/json.py
--rw-r--r--   0        0        0      920 2021-01-28 07:35:51.770038 spinta-0.1.8/spinta/utils/naming.py
--rw-r--r--   0        0        0     1580 2020-01-30 02:55:44.966631 spinta-0.1.8/spinta/utils/nestedstruct.py
--rw-r--r--   0        0        0     2296 2021-01-14 21:24:47.089957 spinta-0.1.8/spinta/utils/nin.py
--rw-r--r--   0        0        0     1424 2019-05-30 05:51:48.468805 spinta-0.1.8/spinta/utils/passwords.py
--rw-r--r--   0        0        0      869 2019-03-09 04:22:52.893518 spinta-0.1.8/spinta/utils/path.py
--rw-r--r--   0        0        0      530 2020-09-10 09:42:58.161767 spinta-0.1.8/spinta/utils/refs.py
--rw-r--r--   0        0        0     4498 2020-12-10 06:44:24.310063 spinta-0.1.8/spinta/utils/response.py
--rw-r--r--   0        0        0     2746 2020-03-26 14:28:49.949988 spinta-0.1.8/spinta/utils/schema.py
--rw-r--r--   0        0        0      587 2019-05-30 05:51:48.468805 spinta-0.1.8/spinta/utils/scopes.py
--rw-r--r--   0        0        0      774 2020-01-11 09:17:03.096498 spinta-0.1.8/spinta/utils/streams.py
--rw-r--r--   0        0        0      555 2020-01-11 09:17:03.096498 spinta-0.1.8/spinta/utils/tree.py
--rw-r--r--   0        0        0      747 2020-09-10 09:42:58.161767 spinta-0.1.8/spinta/utils/units.py
--rw-r--r--   0        0        0     2613 2020-09-11 08:52:26.560100 spinta-0.1.8/spinta/utils/url.py
--rw-r--r--   0        0        0     4709 2021-01-28 23:05:48.602743 spinta-0.1.8/setup.py
--rw-r--r--   0        0        0     3496 2021-01-28 23:05:48.603247 spinta-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1071 2019-05-30 05:53:10.268701 spinta-0.1.9/LICENSE
+-rw-r--r--   0        0        0     5934 2021-02-01 12:52:41.360807 spinta-0.1.9/README.rst
+-rw-r--r--   0        0        0     3020 2021-02-01 12:54:21.554146 spinta-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       78 2021-01-29 13:34:49.933553 spinta-0.1.9/spinta/__init__.py
+-rw-r--r--   0        0        0     2371 2020-09-10 09:42:58.151767 spinta-0.1.9/spinta/accesslog/__init__.py
+-rw-r--r--   0        0        0     1749 2020-04-26 07:05:27.973123 spinta-0.1.9/spinta/accesslog/file.py
+-rw-r--r--   0        0        0      866 2020-04-26 07:05:27.973123 spinta-0.1.9/spinta/accesslog/python.py
+-rw-r--r--   0        0        0     6178 2020-12-10 12:04:26.583360 spinta-0.1.9/spinta/api.py
+-rw-r--r--   0        0        0      635 2020-04-26 07:05:27.973123 spinta-0.1.9/spinta/asgi.py
+-rw-r--r--   0        0        0    16110 2020-12-11 08:59:26.259953 spinta-0.1.9/spinta/auth.py
+-rw-r--r--   0        0        0    31155 2020-12-08 12:43:51.513521 spinta-0.1.9/spinta/backends/__init__.py
+-rw-r--r--   0        0        0      846 2021-01-20 18:14:31.603304 spinta-0.1.9/spinta/backends/components.py
+-rw-r--r--   0        0        0        0 2020-04-26 07:05:27.976456 spinta-0.1.9/spinta/backends/fs/__init__.py
+-rw-r--r--   0        0        0        0 2020-04-26 07:05:27.976456 spinta-0.1.9/spinta/backends/fs/commands/__init__.py
+-rw-r--r--   0        0        0      234 2020-04-26 07:05:27.976456 spinta-0.1.9/spinta/backends/fs/commands/bootstrap.py
+-rw-r--r--   0        0        0      555 2020-04-26 07:05:27.976456 spinta-0.1.9/spinta/backends/fs/commands/changes.py
+-rw-r--r--   0        0        0      470 2020-04-26 07:05:27.976456 spinta-0.1.9/spinta/backends/fs/commands/decode.py
+-rw-r--r--   0        0        0     1370 2020-04-26 07:05:27.976456 spinta-0.1.9/spinta/backends/fs/commands/encode.py
+-rw-r--r--   0        0        0      778 2020-04-26 07:05:27.976456 spinta-0.1.9/spinta/backends/fs/commands/init.py
+-rw-r--r--   0        0        0      338 2021-01-18 14:18:20.756589 spinta-0.1.9/spinta/backends/fs/commands/load.py
+-rw-r--r--   0        0        0      309 2020-04-26 07:05:27.976456 spinta-0.1.9/spinta/backends/fs/commands/migrate.py
+-rw-r--r--   0        0        0     1960 2020-04-26 07:05:27.976456 spinta-0.1.9/spinta/backends/fs/commands/read.py
+-rw-r--r--   0        0        0     2455 2020-04-26 07:05:27.976456 spinta-0.1.9/spinta/backends/fs/commands/validate.py
+-rw-r--r--   0        0        0      279 2021-01-21 12:02:21.049991 spinta-0.1.9/spinta/backends/fs/commands/wait.py
+-rw-r--r--   0        0        0      629 2020-09-10 09:42:58.155100 spinta-0.1.9/spinta/backends/fs/commands/wipe.py
+-rw-r--r--   0        0        0     3267 2020-09-10 09:42:58.155100 spinta-0.1.9/spinta/backends/fs/commands/write.py
+-rw-r--r--   0        0        0      226 2021-01-21 12:02:21.039991 spinta-0.1.9/spinta/backends/fs/components.py
+-rw-r--r--   0        0        0      716 2021-01-20 15:17:56.073284 spinta-0.1.9/spinta/backends/helpers.py
+-rw-r--r--   0        0        0        0 2020-04-26 07:05:27.976456 spinta-0.1.9/spinta/backends/memory/__init__.py
+-rw-r--r--   0        0        0        0 2020-04-26 07:05:27.976456 spinta-0.1.9/spinta/backends/memory/commands/__init__.py
+-rw-r--r--   0        0        0        0 2020-04-26 07:05:27.976456 spinta-0.1.9/spinta/backends/memory/commands/auth.py
+-rw-r--r--   0        0        0      226 2020-04-26 07:05:27.976456 spinta-0.1.9/spinta/backends/memory/commands/bootstrap.py
+-rw-r--r--   0        0        0        0 2020-04-26 07:05:27.976456 spinta-0.1.9/spinta/backends/memory/commands/check.py
+-rw-r--r--   0        0        0      301 2020-04-26 07:05:27.976456 spinta-0.1.9/spinta/backends/memory/commands/init.py
+-rw-r--r--   0        0        0      289 2021-01-18 14:20:28.479922 spinta-0.1.9/spinta/backends/memory/commands/load.py
+-rw-r--r--   0        0        0      610 2020-09-10 09:42:58.155100 spinta-0.1.9/spinta/backends/memory/commands/manifest.py
+-rw-r--r--   0        0        0        0 2020-04-26 07:05:27.976456 spinta-0.1.9/spinta/backends/memory/commands/read.py
+-rw-r--r--   0        0        0      246 2021-01-21 12:02:28.266657 spinta-0.1.9/spinta/backends/memory/commands/wait.py
+-rw-r--r--   0        0        0      337 2021-01-07 20:21:35.063300 spinta-0.1.9/spinta/backends/memory/commands/wipe.py
+-rw-r--r--   0        0        0        0 2020-04-26 07:05:27.976456 spinta-0.1.9/spinta/backends/memory/commands/write.py
+-rw-r--r--   0        0        0      295 2021-01-20 17:45:43.893315 spinta-0.1.9/spinta/backends/memory/components.py
+-rw-r--r--   0        0        0        0 2020-04-26 07:05:27.976456 spinta-0.1.9/spinta/backends/mongo/__init__.py
+-rw-r--r--   0        0        0        0 2020-04-26 07:05:27.976456 spinta-0.1.9/spinta/backends/mongo/commands/__init__.py
+-rw-r--r--   0        0        0      222 2020-04-26 07:05:27.976456 spinta-0.1.9/spinta/backends/mongo/commands/bootstrap.py
+-rw-r--r--   0        0        0     1210 2020-04-26 07:05:27.976456 spinta-0.1.9/spinta/backends/mongo/commands/changes.py
+-rw-r--r--   0        0        0      495 2020-04-26 07:05:27.976456 spinta-0.1.9/spinta/backends/mongo/commands/encode.py
+-rw-r--r--   0        0        0      364 2020-09-10 09:42:58.155100 spinta-0.1.9/spinta/backends/mongo/commands/freeze.py
+-rw-r--r--   0        0        0      358 2020-04-26 07:05:27.976456 spinta-0.1.9/spinta/backends/mongo/commands/init.py
+-rw-r--r--   0        0        0      494 2021-01-18 14:20:28.509922 spinta-0.1.9/spinta/backends/mongo/commands/load.py
+-rw-r--r--   0        0        0      297 2020-04-26 07:05:27.976456 spinta-0.1.9/spinta/backends/mongo/commands/migrate.py
+-rw-r--r--   0        0        0    14655 2021-01-15 13:53:43.219944 spinta-0.1.9/spinta/backends/mongo/commands/query.py
+-rw-r--r--   0        0        0     5655 2020-09-10 09:42:58.155100 spinta-0.1.9/spinta/backends/mongo/commands/read.py
+-rw-r--r--   0        0        0     1528 2020-04-26 07:05:27.976456 spinta-0.1.9/spinta/backends/mongo/commands/validate.py
+-rw-r--r--   0        0        0      284 2021-01-21 12:02:39.533324 spinta-0.1.9/spinta/backends/mongo/commands/wait.py
+-rw-r--r--   0        0        0      782 2021-01-07 20:21:57.893299 spinta-0.1.9/spinta/backends/mongo/commands/wipe.py
+-rw-r--r--   0        0        0     4105 2020-09-10 09:42:58.155100 spinta-0.1.9/spinta/backends/mongo/commands/write.py
+-rw-r--r--   0        0        0     1908 2021-01-20 17:45:43.886648 spinta-0.1.9/spinta/backends/mongo/components.py
+-rw-r--r--   0        0        0      250 2020-04-26 07:05:27.979790 spinta-0.1.9/spinta/backends/mongo/helpers.py
+-rw-r--r--   0        0        0        0 2020-04-26 07:05:27.979790 spinta-0.1.9/spinta/backends/mongo/types/__init__.py
+-rw-r--r--   0        0        0        0 2020-04-26 07:05:27.979790 spinta-0.1.9/spinta/backends/mongo/types/array/__init__.py
+-rw-r--r--   0        0        0      694 2020-04-26 07:05:27.979790 spinta-0.1.9/spinta/backends/mongo/types/array/write.py
+-rw-r--r--   0        0        0        0 2020-04-26 07:05:27.979790 spinta-0.1.9/spinta/backends/mongo/types/file/__init__.py
+-rw-r--r--   0        0        0      965 2020-04-26 07:05:27.979790 spinta-0.1.9/spinta/backends/mongo/types/file/write.py
+-rw-r--r--   0        0        0        0 2020-04-26 07:05:27.979790 spinta-0.1.9/spinta/backends/mongo/types/object/__init__.py
+-rw-r--r--   0        0        0      793 2020-04-26 07:05:27.979790 spinta-0.1.9/spinta/backends/mongo/types/object/write.py
+-rw-r--r--   0        0        0        0 2020-04-26 07:05:27.979790 spinta-0.1.9/spinta/backends/postgresql/__init__.py
+-rw-r--r--   0        0        0        0 2020-04-26 07:05:27.979790 spinta-0.1.9/spinta/backends/postgresql/commands/__init__.py
+-rw-r--r--   0        0        0      558 2020-04-26 07:05:27.979790 spinta-0.1.9/spinta/backends/postgresql/commands/bootstrap.py
+-rw-r--r--   0        0        0     3531 2020-04-26 07:05:27.979790 spinta-0.1.9/spinta/backends/postgresql/commands/changes.py
+-rw-r--r--   0        0        0     1489 2020-04-26 07:05:27.979790 spinta-0.1.9/spinta/backends/postgresql/commands/encode.py
+-rw-r--r--   0        0        0     5868 2020-09-10 09:42:58.155100 spinta-0.1.9/spinta/backends/postgresql/commands/freeze.py
+-rw-r--r--   0        0        0     3362 2021-01-30 22:41:14.601317 spinta-0.1.9/spinta/backends/postgresql/commands/init.py
+-rw-r--r--   0        0        0        0 2020-04-26 07:05:27.979790 spinta-0.1.9/spinta/backends/postgresql/commands/link.py
+-rw-r--r--   0        0        0      841 2021-01-18 14:21:03.739921 spinta-0.1.9/spinta/backends/postgresql/commands/load.py
+-rw-r--r--   0        0        0     1879 2020-09-10 09:42:58.155100 spinta-0.1.9/spinta/backends/postgresql/commands/manifest.py
+-rw-r--r--   0        0        0     1209 2021-01-19 06:59:24.266647 spinta-0.1.9/spinta/backends/postgresql/commands/migrate.py
+-rw-r--r--   0        0        0    27508 2020-12-11 10:35:03.219921 spinta-0.1.9/spinta/backends/postgresql/commands/query.py
+-rw-r--r--   0        0        0     3928 2020-09-10 09:42:58.155100 spinta-0.1.9/spinta/backends/postgresql/commands/read.py
+-rw-r--r--   0        0        0      615 2020-04-26 07:05:27.979790 spinta-0.1.9/spinta/backends/postgresql/commands/validate.py
+-rw-r--r--   0        0        0      700 2021-01-21 12:01:18.356658 spinta-0.1.9/spinta/backends/postgresql/commands/wait.py
+-rw-r--r--   0        0        0     1335 2021-01-07 20:22:33.623299 spinta-0.1.9/spinta/backends/postgresql/commands/wipe.py
+-rw-r--r--   0        0        0     3823 2020-04-26 07:05:27.979790 spinta-0.1.9/spinta/backends/postgresql/commands/write.py
+-rw-r--r--   0        0        0     4219 2021-01-20 17:44:29.493315 spinta-0.1.9/spinta/backends/postgresql/components.py
+-rw-r--r--   0        0        0      411 2020-04-26 07:05:27.979790 spinta-0.1.9/spinta/backends/postgresql/constants.py
+-rw-r--r--   0        0        0     6472 2020-03-26 09:03:44.213110 spinta-0.1.9/spinta/backends/postgresql/files.py
+-rw-r--r--   0        0        0     1430 2020-09-10 09:42:58.155100 spinta-0.1.9/spinta/backends/postgresql/helpers/__init__.py
+-rw-r--r--   0        0        0     1704 2020-04-26 07:05:27.986456 spinta-0.1.9/spinta/backends/postgresql/helpers/changes.py
+-rw-r--r--   0        0        0      706 2020-04-26 07:05:27.986456 spinta-0.1.9/spinta/backends/postgresql/helpers/manifest.py
+-rw-r--r--   0        0        0     1096 2020-04-26 07:05:27.986456 spinta-0.1.9/spinta/backends/postgresql/helpers/validate.py
+-rw-r--r--   0        0        0      304 2020-04-26 07:05:27.986456 spinta-0.1.9/spinta/backends/postgresql/sqlalchemy.py
+-rw-r--r--   0        0        0        0 2020-04-26 07:05:27.986456 spinta-0.1.9/spinta/backends/postgresql/types/__init__.py
+-rw-r--r--   0        0        0        0 2020-04-26 07:05:27.986456 spinta-0.1.9/spinta/backends/postgresql/types/array/__init__.py
+-rw-r--r--   0        0        0     2266 2020-09-10 09:42:58.155100 spinta-0.1.9/spinta/backends/postgresql/types/array/freeze.py
+-rw-r--r--   0        0        0     1985 2020-04-26 07:05:27.986456 spinta-0.1.9/spinta/backends/postgresql/types/array/init.py
+-rw-r--r--   0        0        0      541 2021-01-07 20:22:49.246633 spinta-0.1.9/spinta/backends/postgresql/types/array/wipe.py
+-rw-r--r--   0        0        0     4287 2020-04-26 07:05:27.986456 spinta-0.1.9/spinta/backends/postgresql/types/array/write.py
+-rw-r--r--   0        0        0        0 2020-04-26 07:05:27.986456 spinta-0.1.9/spinta/backends/postgresql/types/file/__init__.py
+-rw-r--r--   0        0        0     3019 2020-09-10 09:42:58.155100 spinta-0.1.9/spinta/backends/postgresql/types/file/freeze.py
+-rw-r--r--   0        0        0     2022 2020-04-26 07:05:27.986456 spinta-0.1.9/spinta/backends/postgresql/types/file/init.py
+-rw-r--r--   0        0        0     4164 2020-04-26 07:05:27.986456 spinta-0.1.9/spinta/backends/postgresql/types/file/read.py
+-rw-r--r--   0        0        0     4585 2020-04-26 07:05:27.986456 spinta-0.1.9/spinta/backends/postgresql/types/file/write.py
+-rw-r--r--   0        0        0        0 2020-04-26 07:05:27.986456 spinta-0.1.9/spinta/backends/postgresql/types/object/__init__.py
+-rw-r--r--   0        0        0     1634 2020-09-10 09:42:58.155100 spinta-0.1.9/spinta/backends/postgresql/types/object/freeze.py
+-rw-r--r--   0        0        0      665 2020-04-26 07:05:27.986456 spinta-0.1.9/spinta/backends/postgresql/types/object/init.py
+-rw-r--r--   0        0        0     2545 2020-04-26 07:05:27.986456 spinta-0.1.9/spinta/backends/postgresql/types/object/read.py
+-rw-r--r--   0        0        0      373 2021-01-07 20:22:12.533300 spinta-0.1.9/spinta/backends/postgresql/types/object/wipe.py
+-rw-r--r--   0        0        0        0 2020-04-26 07:05:27.986456 spinta-0.1.9/spinta/backends/postgresql/types/ref/__init__.py
+-rw-r--r--   0        0        0     2030 2020-09-10 09:42:58.155100 spinta-0.1.9/spinta/backends/postgresql/types/ref/freeze.py
+-rw-r--r--   0        0        0     1230 2020-04-26 07:05:27.986456 spinta-0.1.9/spinta/backends/postgresql/types/ref/init.py
+-rw-r--r--   0        0        0      661 2020-04-26 07:05:27.986456 spinta-0.1.9/spinta/backends/postgresql/types/ref/validate.py
+-rw-r--r--   0        0        0     6955 2021-01-26 08:12:54.683294 spinta-0.1.9/spinta/backends/s3.py
+-rw-r--r--   0        0        0        0 2021-01-21 08:40:26.719976 spinta-0.1.9/spinta/cli/__init__.py
+-rw-r--r--   0        0        0     3640 2021-01-25 16:14:06.659794 spinta-0.1.9/spinta/cli/auth.py
+-rw-r--r--   0        0        0      636 2021-01-21 09:52:47.733285 spinta-0.1.9/spinta/cli/config.py
+-rw-r--r--   0        0        0     1240 2021-01-21 10:04:33.656615 spinta-0.1.9/spinta/cli/data.py
+-rw-r--r--   0        0        0        0 2020-12-28 10:05:48.744968 spinta-0.1.9/spinta/cli/helpers/__init__.py
+-rw-r--r--   0        0        0      898 2020-12-28 10:13:57.328306 spinta-0.1.9/spinta/cli/helpers/auth.py
+-rw-r--r--   0        0        0     3181 2021-01-21 10:01:12.119949 spinta-0.1.9/spinta/cli/helpers/data.py
+-rw-r--r--   0        0        0      936 2021-01-29 14:52:03.127155 spinta-0.1.9/spinta/cli/helpers/store.py
+-rw-r--r--   0        0        0      285 2021-01-21 10:35:03.059938 spinta-0.1.9/spinta/cli/helpers/typer.py
+-rw-r--r--   0        0        0      327 2021-01-29 18:36:24.843460 spinta-0.1.9/spinta/cli/init.py
+-rw-r--r--   0        0        0     3794 2021-01-29 19:12:25.950252 spinta-0.1.9/spinta/cli/inspect.py
+-rw-r--r--   0        0        0     2730 2021-02-01 11:23:28.500497 spinta-0.1.9/spinta/cli/main.py
+-rw-r--r--   0        0        0     2986 2021-02-01 11:23:46.957165 spinta-0.1.9/spinta/cli/manifest.py
+-rw-r--r--   0        0        0     1794 2021-02-01 08:30:25.996992 spinta-0.1.9/spinta/cli/migrate.py
+-rw-r--r--   0        0        0     7052 2021-01-21 10:33:35.233272 spinta-0.1.9/spinta/cli/pii.py
+-rw-r--r--   0        0        0     3562 2021-01-21 10:48:31.516600 spinta-0.1.9/spinta/cli/pull.py
+-rw-r--r--   0        0        0    10016 2021-01-21 11:47:28.626662 spinta-0.1.9/spinta/cli/push.py
+-rw-r--r--   0        0        0      956 2021-01-21 12:41:32.606644 spinta-0.1.9/spinta/cli/server.py
+-rw-r--r--   0        0        0     1197 2021-01-29 18:28:17.420098 spinta-0.1.9/spinta/cli/show.py
+-rw-r--r--   0        0        0    13461 2021-01-21 12:40:59.896644 spinta-0.1.9/spinta/commands/__init__.py
+-rw-r--r--   0        0        0      532 2020-09-10 09:42:58.155100 spinta-0.1.9/spinta/commands/auth.py
+-rw-r--r--   0        0        0      280 2020-03-26 14:28:49.946654 spinta-0.1.9/spinta/commands/formats/__init__.py
+-rw-r--r--   0        0        0     3090 2020-04-26 07:05:27.986456 spinta-0.1.9/spinta/commands/formats/ascii.py
+-rw-r--r--   0        0        0     1658 2020-12-10 16:26:20.303337 spinta-0.1.9/spinta/commands/formats/csv.py
+-rw-r--r--   0        0        0    10459 2020-12-11 09:48:32.916603 spinta-0.1.9/spinta/commands/formats/html.py
+-rw-r--r--   0        0        0     2082 2020-09-10 09:42:58.155100 spinta-0.1.9/spinta/commands/formats/json.py
+-rw-r--r--   0        0        0     1529 2020-04-26 07:05:27.986456 spinta-0.1.9/spinta/commands/formats/jsonl.py
+-rw-r--r--   0        0        0      894 2019-05-01 06:33:24.263673 spinta-0.1.9/spinta/commands/helpers.py
+-rw-r--r--   0        0        0     1324 2020-04-26 07:05:27.986456 spinta-0.1.9/spinta/commands/read.py
+-rw-r--r--   0        0        0     3111 2020-04-26 07:05:27.986456 spinta-0.1.9/spinta/commands/search.py
+-rw-r--r--   0        0        0      605 2020-04-26 07:05:27.986456 spinta-0.1.9/spinta/commands/version.py
+-rw-r--r--   0        0        0    34083 2021-01-07 20:23:22.399966 spinta-0.1.9/spinta/commands/write.py
+-rw-r--r--   0        0        0     1637 2020-12-08 12:43:51.353521 spinta-0.1.9/spinta/compat.py
+-rw-r--r--   0        0        0    22840 2021-01-21 10:06:15.496614 spinta-0.1.9/spinta/components.py
+-rw-r--r--   0        0        0     9572 2021-02-01 08:30:01.140324 spinta-0.1.9/spinta/config.py
+-rw-r--r--   0        0        0     2754 2021-01-21 09:24:23.033295 spinta-0.1.9/spinta/config.yml
+-rw-r--r--   0        0        0        0 2020-03-21 10:14:12.239947 spinta-0.1.9/spinta/core/__init__.py
+-rw-r--r--   0        0        0      967 2020-09-10 09:42:58.158434 spinta-0.1.9/spinta/core/access.py
+-rw-r--r--   0        0        0    13961 2021-02-01 08:04:41.356902 spinta-0.1.9/spinta/core/config.py
+-rw-r--r--   0        0        0     1430 2021-01-26 20:00:10.906601 spinta-0.1.9/spinta/core/context.py
+-rw-r--r--   0        0        0      816 2021-01-21 14:26:38.269942 spinta-0.1.9/spinta/core/enums.py
+-rw-r--r--   0        0        0     7407 2020-12-08 12:43:51.353521 spinta-0.1.9/spinta/core/ufuncs.py
+-rw-r--r--   0        0        0        0 2020-04-26 07:05:27.986456 spinta-0.1.9/spinta/datasets/__init__.py
+-rw-r--r--   0        0        0        0 2020-04-26 07:05:27.986456 spinta-0.1.9/spinta/datasets/backends/__init__.py
+-rw-r--r--   0        0        0        0 2020-04-26 07:05:27.986456 spinta-0.1.9/spinta/datasets/backends/csv/__init__.py
+-rw-r--r--   0        0        0     1681 2021-01-18 14:21:37.686588 spinta-0.1.9/spinta/datasets/backends/csv/commands.py
+-rw-r--r--   0        0        0      207 2020-04-26 07:05:27.986456 spinta-0.1.9/spinta/datasets/backends/csv/components.py
+-rw-r--r--   0        0        0        0 2021-01-20 16:56:30.636664 spinta-0.1.9/spinta/datasets/backends/frictionless/__init__.py
+-rw-r--r--   0        0        0        0 2021-01-20 16:56:30.626664 spinta-0.1.9/spinta/datasets/backends/frictionless/commands/__init__.py
+-rw-r--r--   0        0        0      363 2021-01-20 17:09:34.603327 spinta-0.1.9/spinta/datasets/backends/frictionless/commands/load.py
+-rw-r--r--   0        0        0      308 2021-01-25 15:52:35.836468 spinta-0.1.9/spinta/datasets/backends/frictionless/commands/wait.py
+-rw-r--r--   0        0        0      348 2021-01-20 17:38:22.756651 spinta-0.1.9/spinta/datasets/backends/frictionless/commands/wipe.py
+-rw-r--r--   0        0        0      110 2021-01-20 17:08:52.959994 spinta-0.1.9/spinta/datasets/backends/frictionless/components.py
+-rw-r--r--   0        0        0        0 2020-04-26 07:05:27.986456 spinta-0.1.9/spinta/datasets/backends/sql/__init__.py
+-rw-r--r--   0        0        0        0 2021-01-08 10:36:18.803259 spinta-0.1.9/spinta/datasets/backends/sql/commands/__init__.py
+-rw-r--r--   0        0        0      223 2021-01-19 07:15:19.473309 spinta-0.1.9/spinta/datasets/backends/sql/commands/bootstrap.py
+-rw-r--r--   0        0        0      507 2021-01-19 07:15:19.493309 spinta-0.1.9/spinta/datasets/backends/sql/commands/init.py
+-rw-r--r--   0        0        0     4220 2021-01-26 20:51:04.526584 spinta-0.1.9/spinta/datasets/backends/sql/commands/inspect.py
+-rw-r--r--   0        0        0      496 2021-01-18 14:22:24.283254 spinta-0.1.9/spinta/datasets/backends/sql/commands/load.py
+-rw-r--r--   0        0        0    22238 2020-12-17 16:12:51.809815 spinta-0.1.9/spinta/datasets/backends/sql/commands/query.py
+-rw-r--r--   0        0        0     3175 2021-01-18 13:53:52.373264 spinta-0.1.9/spinta/datasets/backends/sql/commands/read.py
+-rw-r--r--   0        0        0      673 2021-01-19 07:15:19.506642 spinta-0.1.9/spinta/datasets/backends/sql/commands/wait.py
+-rw-r--r--   0        0        0     1507 2021-01-07 20:18:11.676634 spinta-0.1.9/spinta/datasets/backends/sql/components.py
+-rw-r--r--   0        0        0        0 2021-01-27 07:43:53.063291 spinta-0.1.9/spinta/datasets/backends/sqldump/__init__.py
+-rw-r--r--   0        0        0        0 2021-01-27 07:45:51.933290 spinta-0.1.9/spinta/datasets/backends/sqldump/commands/__init__.py
+-rw-r--r--   0        0        0     3235 2021-01-27 17:42:10.096891 spinta-0.1.9/spinta/datasets/backends/sqldump/commands/inspect.py
+-rw-r--r--   0        0        0      537 2021-01-27 17:39:41.500216 spinta-0.1.9/spinta/datasets/backends/sqldump/commands/load.py
+-rw-r--r--   0        0        0      588 2021-01-27 17:41:32.503556 spinta-0.1.9/spinta/datasets/backends/sqldump/components.py
+-rw-r--r--   0        0        0        0 2021-01-27 14:43:29.126271 spinta-0.1.9/spinta/datasets/backends/sqldump/ufuncs/__init__.py
+-rw-r--r--   0        0        0      364 2021-01-27 17:24:28.216830 spinta-0.1.9/spinta/datasets/backends/sqldump/ufuncs/components.py
+-rw-r--r--   0        0        0      698 2021-01-27 17:47:46.256911 spinta-0.1.9/spinta/datasets/backends/sqldump/ufuncs/ufuncs.py
+-rw-r--r--   0        0        0        0 2020-04-26 07:05:27.986456 spinta-0.1.9/spinta/datasets/commands/__init__.py
+-rw-r--r--   0        0        0      376 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/datasets/commands/check.py
+-rw-r--r--   0        0        0      939 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/datasets/commands/error.py
+-rw-r--r--   0        0        0      319 2021-01-20 13:23:47.033323 spinta-0.1.9/spinta/datasets/commands/inspect.py
+-rw-r--r--   0        0        0     1954 2020-12-17 20:02:03.593070 spinta-0.1.9/spinta/datasets/commands/link.py
+-rw-r--r--   0        0        0     2280 2021-01-27 17:00:22.843413 spinta-0.1.9/spinta/datasets/commands/load.py
+-rw-r--r--   0        0        0     1266 2020-12-08 12:43:51.353521 spinta-0.1.9/spinta/datasets/commands/read.py
+-rw-r--r--   0        0        0      327 2021-01-07 20:23:41.829966 spinta-0.1.9/spinta/datasets/commands/wipe.py
+-rw-r--r--   0        0        0     4968 2021-01-27 13:15:37.956626 spinta-0.1.9/spinta/datasets/components.py
+-rw-r--r--   0        0        0      452 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/datasets/enums.py
+-rw-r--r--   0        0        0     2119 2021-01-20 15:17:56.089951 spinta-0.1.9/spinta/datasets/helpers.py
+-rw-r--r--   0        0        0        0 2020-09-10 09:42:58.158434 spinta-0.1.9/spinta/datasets/keymaps/__init__.py
+-rw-r--r--   0        0        0      305 2020-09-10 09:42:58.158434 spinta-0.1.9/spinta/datasets/keymaps/components.py
+-rw-r--r--   0        0        0     3062 2020-12-08 12:43:51.553521 spinta-0.1.9/spinta/datasets/keymaps/sqlalchemy.py
+-rw-r--r--   0        0        0       81 2020-09-10 09:42:58.158434 spinta-0.1.9/spinta/datasets/utils.py
+-rw-r--r--   0        0        0        0 2020-12-20 10:53:38.389942 spinta-0.1.9/spinta/dimensions/__init__.py
+-rw-r--r--   0        0        0        0 2020-12-20 11:00:17.646606 spinta-0.1.9/spinta/dimensions/commands/__init__.py
+-rw-r--r--   0        0        0      462 2020-12-20 13:01:32.526657 spinta-0.1.9/spinta/dimensions/commands/load.py
+-rw-r--r--   0        0        0        0 2020-12-20 12:58:25.826658 spinta-0.1.9/spinta/dimensions/prefix/__init__.py
+-rw-r--r--   0        0        0      618 2021-01-07 20:18:11.676634 spinta-0.1.9/spinta/dimensions/prefix/components.py
+-rw-r--r--   0        0        0      978 2020-12-20 13:14:48.746652 spinta-0.1.9/spinta/dimensions/prefix/helpers.py
+-rw-r--r--   0        0        0     3825 2020-12-30 11:19:49.503333 spinta-0.1.9/spinta/dispatcher.py
+-rw-r--r--   0        0        0    11734 2021-02-01 07:46:42.496840 spinta-0.1.9/spinta/exceptions.py
+-rw-r--r--   0        0        0     1331 2020-03-26 14:28:49.946654 spinta-0.1.9/spinta/fetcher.py
+-rw-r--r--   0        0        0        0 2020-01-11 09:17:03.093164 spinta-0.1.9/spinta/hacks/__init__.py
+-rw-r--r--   0        0        0      900 2020-03-21 10:14:12.243281 spinta-0.1.9/spinta/hacks/spyna.py
+-rw-r--r--   0        0        0     1676 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/manifest/_schema/version.yml
+-rw-r--r--   0        0        0     1110 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/manifest/_schema.yml
+-rw-r--r--   0        0        0     1205 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/manifest/_txn.yml
+-rw-r--r--   0        0        0        0 2020-03-21 10:14:12.243281 spinta-0.1.9/spinta/manifests/__init__.py
+-rw-r--r--   0        0        0        0 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/manifests/backend/__init__.py
+-rw-r--r--   0        0        0        0 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/manifests/backend/commands/__init__.py
+-rw-r--r--   0        0        0      608 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/manifests/backend/commands/bootstrap.py
+-rw-r--r--   0        0        0      256 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/manifests/backend/commands/configure.py
+-rw-r--r--   0        0        0      378 2020-09-10 09:42:58.158434 spinta-0.1.9/spinta/manifests/backend/commands/freeze.py
+-rw-r--r--   0        0        0      539 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/manifests/backend/commands/load.py
+-rw-r--r--   0        0        0     1402 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/manifests/backend/commands/manifest.py
+-rw-r--r--   0        0        0      589 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/manifests/backend/commands/migrate.py
+-rw-r--r--   0        0        0      712 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/manifests/backend/commands/sync.py
+-rw-r--r--   0        0        0       93 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/manifests/backend/components.py
+-rw-r--r--   0        0        0     8173 2021-01-07 20:18:11.676634 spinta-0.1.9/spinta/manifests/backend/helpers.py
+-rw-r--r--   0        0        0        0 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/manifests/commands/__init__.py
+-rw-r--r--   0        0        0      675 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/manifests/commands/check.py
+-rw-r--r--   0        0        0      993 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/manifests/commands/error.py
+-rw-r--r--   0        0        0      430 2020-09-10 09:42:58.158434 spinta-0.1.9/spinta/manifests/commands/init.py
+-rw-r--r--   0        0        0      314 2021-01-20 12:27:03.219899 spinta-0.1.9/spinta/manifests/commands/inspect.py
+-rw-r--r--   0        0        0      437 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/manifests/commands/link.py
+-rw-r--r--   0        0        0     2120 2021-01-21 08:09:45.639987 spinta-0.1.9/spinta/manifests/components.py
+-rw-r--r--   0        0        0     4993 2021-02-01 08:30:38.963659 spinta-0.1.9/spinta/manifests/helpers.py
+-rw-r--r--   0        0        0        0 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/manifests/internal/__init__.py
+-rw-r--r--   0        0        0        0 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/manifests/internal/commands/__init__.py
+-rw-r--r--   0        0        0      479 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/manifests/internal/commands/configure.py
+-rw-r--r--   0        0        0     1660 2020-09-10 09:42:58.158434 spinta-0.1.9/spinta/manifests/internal/commands/load.py
+-rw-r--r--   0        0        0      107 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/manifests/internal/components.py
+-rw-r--r--   0        0        0        0 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/manifests/tabular/__init__.py
+-rw-r--r--   0        0        0        0 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/manifests/tabular/commands/__init__.py
+-rw-r--r--   0        0        0      438 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/manifests/tabular/commands/bootstrap.py
+-rw-r--r--   0        0        0      595 2021-01-26 08:03:38.269964 spinta-0.1.9/spinta/manifests/tabular/commands/configure.py
+-rw-r--r--   0        0        0     1610 2021-01-26 08:07:08.613296 spinta-0.1.9/spinta/manifests/tabular/commands/load.py
+-rw-r--r--   0        0        0       93 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/manifests/tabular/components.py
+-rw-r--r--   0        0        0      218 2021-01-29 15:12:41.033893 spinta-0.1.9/spinta/manifests/tabular/constants.py
+-rw-r--r--   0        0        0    25558 2021-01-29 14:45:02.493797 spinta-0.1.9/spinta/manifests/tabular/helpers.py
+-rw-r--r--   0        0        0        0 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/manifests/yaml/__init__.py
+-rw-r--r--   0        0        0        0 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/manifests/yaml/commands/__init__.py
+-rw-r--r--   0        0        0      423 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/manifests/yaml/commands/bootstrap.py
+-rw-r--r--   0        0        0      478 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/manifests/yaml/commands/configure.py
+-rw-r--r--   0        0        0     2051 2020-09-10 09:42:58.158434 spinta-0.1.9/spinta/manifests/yaml/commands/freeze.py
+-rw-r--r--   0        0        0     1812 2020-09-10 09:42:58.158434 spinta-0.1.9/spinta/manifests/yaml/commands/load.py
+-rw-r--r--   0        0        0     1327 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/manifests/yaml/commands/manifest.py
+-rw-r--r--   0        0        0      360 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/manifests/yaml/commands/migrate.py
+-rw-r--r--   0        0        0      313 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/manifests/yaml/commands/sync.py
+-rw-r--r--   0        0        0       90 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/manifests/yaml/components.py
+-rw-r--r--   0        0        0     4079 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/manifests/yaml/helpers.py
+-rw-r--r--   0        0        0        0 2019-05-01 06:33:24.263673 spinta-0.1.9/spinta/methods.py
+-rw-r--r--   0        0        0     1138 2020-12-10 12:18:59.933368 spinta-0.1.9/spinta/middlewares.py
+-rw-r--r--   0        0        0      660 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-03-21 10:14:12.243281 spinta-0.1.9/spinta/migrations/schema/__init__.py
+-rw-r--r--   0        0        0     2847 2020-09-10 09:42:58.158434 spinta-0.1.9/spinta/migrations/schema/alembic.py
+-rw-r--r--   0        0        0     5950 2020-12-20 13:12:52.643320 spinta-0.1.9/spinta/nodes.py
+-rw-r--r--   0        0        0      659 2020-01-11 09:17:03.096498 spinta-0.1.9/spinta/renderer.py
+-rw-r--r--   0        0        0     8514 2020-09-10 09:42:58.161767 spinta-0.1.9/spinta/spyna.py
+-rw-r--r--   0        0        0     3500 2020-01-11 09:17:03.096498 spinta-0.1.9/spinta/templates/base.html
+-rw-r--r--   0        0        0      178 2020-01-11 09:17:03.096498 spinta-0.1.9/spinta/templates/error.html
+-rw-r--r--   0        0        0       50 2019-05-01 06:33:24.263673 spinta-0.1.9/spinta/testing/__init__.py
+-rw-r--r--   0        0        0     1753 2021-02-01 08:26:40.446979 spinta-0.1.9/spinta/testing/cli.py
+-rw-r--r--   0        0        0     5859 2020-09-10 09:42:58.161767 spinta-0.1.9/spinta/testing/client.py
+-rw-r--r--   0        0        0     2656 2021-01-26 08:39:54.229952 spinta-0.1.9/spinta/testing/config.py
+-rw-r--r--   0        0        0     2800 2021-01-30 22:35:27.174631 spinta-0.1.9/spinta/testing/context.py
+-rw-r--r--   0        0        0      236 2020-09-11 07:31:45.943388 spinta-0.1.9/spinta/testing/csv.py
+-rw-r--r--   0        0        0     2126 2020-12-08 12:43:51.356854 spinta-0.1.9/spinta/testing/data.py
+-rw-r--r--   0        0        0     1446 2021-01-21 13:28:21.726628 spinta-0.1.9/spinta/testing/datasets.py
+-rw-r--r--   0        0        0     5544 2020-09-10 09:42:58.161767 spinta-0.1.9/spinta/testing/dtypes.py
+-rw-r--r--   0        0        0        0 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/testing/manifest.py
+-rw-r--r--   0        0        0     5448 2021-01-27 11:42:16.086658 spinta-0.1.9/spinta/testing/pytest.py
+-rw-r--r--   0        0        0     1303 2021-01-29 14:44:26.997128 spinta-0.1.9/spinta/testing/tabular.py
+-rw-r--r--   0        0        0      769 2020-03-21 10:14:12.246614 spinta-0.1.9/spinta/testing/ufuncs.py
+-rw-r--r--   0        0        0     4995 2020-09-10 09:42:58.161767 spinta-0.1.9/spinta/testing/utils.py
+-rw-r--r--   0        0        0      349 2021-01-29 14:47:45.263806 spinta-0.1.9/spinta/testing/workarounds.py
+-rw-r--r--   0        0        0        0 2019-06-14 18:23:09.532354 spinta-0.1.9/spinta/types/__init__.py
+-rw-r--r--   0        0        0        0 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/types/array/__init__.py
+-rw-r--r--   0        0        0      411 2021-01-07 20:18:11.676634 spinta-0.1.9/spinta/types/array/link.py
+-rw-r--r--   0        0        0      973 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/types/command.py
+-rw-r--r--   0        0        0     2948 2020-09-10 09:42:58.161767 spinta-0.1.9/spinta/types/config.py
+-rw-r--r--   0        0        0     9575 2021-01-07 20:18:11.676634 spinta-0.1.9/spinta/types/datatype.py
+-rw-r--r--   0        0        0        0 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/types/file/__init__.py
+-rw-r--r--   0        0        0     1039 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/types/file/decode.py
+-rw-r--r--   0        0        0     1070 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/types/file/helpers.py
+-rw-r--r--   0        0        0      919 2021-01-26 19:02:09.116621 spinta-0.1.9/spinta/types/helpers.py
+-rw-r--r--   0        0        0     9052 2021-01-30 22:33:55.494625 spinta-0.1.9/spinta/types/model.py
+-rw-r--r--   0        0        0     8732 2021-01-20 17:46:21.926648 spinta-0.1.9/spinta/types/namespace.py
+-rw-r--r--   0        0        0        0 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/types/object/__init__.py
+-rw-r--r--   0        0        0      367 2021-01-07 20:18:11.679967 spinta-0.1.9/spinta/types/object/link.py
+-rw-r--r--   0        0        0     1022 2020-09-10 09:42:58.161767 spinta-0.1.9/spinta/types/owner.py
+-rw-r--r--   0        0        0     2420 2020-09-10 09:43:39.961767 spinta-0.1.9/spinta/types/project.py
+-rw-r--r--   0        0        0        0 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/types/ref/__init__.py
+-rw-r--r--   0        0        0     1367 2021-01-26 20:43:56.426586 spinta-0.1.9/spinta/types/ref/link.py
+-rw-r--r--   0        0        0     4514 2021-01-30 22:37:18.411304 spinta-0.1.9/spinta/types/store.py
+-rw-r--r--   0        0        0      764 2020-12-08 12:43:51.356854 spinta-0.1.9/spinta/ufuncs.py
+-rw-r--r--   0        0        0     8342 2020-12-08 12:43:51.356854 spinta-0.1.9/spinta/urlparams.py
+-rw-r--r--   0        0        0        0 2019-03-09 04:22:52.893518 spinta-0.1.9/spinta/utils/__init__.py
+-rw-r--r--   0        0        0     1939 2020-04-26 07:05:27.993123 spinta-0.1.9/spinta/utils/aiotools.py
+-rw-r--r--   0        0        0      345 2020-01-11 09:17:03.096498 spinta-0.1.9/spinta/utils/changes.py
+-rw-r--r--   0        0        0      301 2020-09-10 09:42:58.161767 spinta-0.1.9/spinta/utils/config.py
+-rw-r--r--   0        0        0     2554 2021-01-07 20:18:11.679967 spinta-0.1.9/spinta/utils/data.py
+-rw-r--r--   0        0        0      444 2020-09-10 09:42:58.161767 spinta-0.1.9/spinta/utils/enums.py
+-rw-r--r--   0        0        0      192 2020-01-11 09:17:03.096498 spinta-0.1.9/spinta/utils/errors.py
+-rw-r--r--   0        0        0      373 2019-05-30 05:51:48.468805 spinta-0.1.9/spinta/utils/idgen.py
+-rw-r--r--   0        0        0      342 2021-01-15 13:55:31.979943 spinta-0.1.9/spinta/utils/imports.py
+-rw-r--r--   0        0        0     1926 2020-09-10 09:42:58.161767 spinta-0.1.9/spinta/utils/itertools.py
+-rw-r--r--   0        0        0      730 2020-09-10 09:42:58.161767 spinta-0.1.9/spinta/utils/json.py
+-rw-r--r--   0        0        0      920 2021-01-28 07:35:51.770038 spinta-0.1.9/spinta/utils/naming.py
+-rw-r--r--   0        0        0     1580 2020-01-30 02:55:44.966631 spinta-0.1.9/spinta/utils/nestedstruct.py
+-rw-r--r--   0        0        0     2296 2021-01-14 21:24:47.089957 spinta-0.1.9/spinta/utils/nin.py
+-rw-r--r--   0        0        0     1424 2019-05-30 05:51:48.468805 spinta-0.1.9/spinta/utils/passwords.py
+-rw-r--r--   0        0        0      869 2019-03-09 04:22:52.893518 spinta-0.1.9/spinta/utils/path.py
+-rw-r--r--   0        0        0      530 2020-09-10 09:42:58.161767 spinta-0.1.9/spinta/utils/refs.py
+-rw-r--r--   0        0        0     4625 2021-02-01 07:46:58.990174 spinta-0.1.9/spinta/utils/response.py
+-rw-r--r--   0        0        0     2746 2020-03-26 14:28:49.949988 spinta-0.1.9/spinta/utils/schema.py
+-rw-r--r--   0        0        0      587 2019-05-30 05:51:48.468805 spinta-0.1.9/spinta/utils/scopes.py
+-rw-r--r--   0        0        0      774 2020-01-11 09:17:03.096498 spinta-0.1.9/spinta/utils/streams.py
+-rw-r--r--   0        0        0      555 2020-01-11 09:17:03.096498 spinta-0.1.9/spinta/utils/tree.py
+-rw-r--r--   0        0        0      747 2020-09-10 09:42:58.161767 spinta-0.1.9/spinta/utils/units.py
+-rw-r--r--   0        0        0     2613 2020-09-11 08:52:26.560100 spinta-0.1.9/spinta/utils/url.py
+-rw-r--r--   0        0        0     9303 2021-02-01 12:56:04.680559 spinta-0.1.9/setup.py
+-rw-r--r--   0        0        0     7949 2021-02-01 12:56:04.681772 spinta-0.1.9/PKG-INFO
```

### Comparing `spinta-0.1.8/LICENSE` & `spinta-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/pyproject.toml` & `spinta-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spinta"
-version = "0.1.8"
+version = "0.1.9"
 description = "A platform for describing, extracting, transforming, loading and serving open data."
 authors = ["Mantas Zimnickas <sirexas@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://gitlab.com/atviriduomenys/spinta"
 repository = "https://gitlab.com/atviriduomenys/spinta"
 documentation = "https://spinta.readthedocs.io/"
```

### Comparing `spinta-0.1.8/spinta/accesslog/__init__.py` & `spinta-0.1.9/spinta/accesslog/__init__.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/accesslog/file.py` & `spinta-0.1.9/spinta/accesslog/file.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/accesslog/python.py` & `spinta-0.1.9/spinta/accesslog/python.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/api.py` & `spinta-0.1.9/spinta/api.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/asgi.py` & `spinta-0.1.9/spinta/asgi.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/auth.py` & `spinta-0.1.9/spinta/auth.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/__init__.py` & `spinta-0.1.9/spinta/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/components.py` & `spinta-0.1.9/spinta/backends/components.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/fs/commands/changes.py` & `spinta-0.1.9/spinta/backends/fs/commands/changes.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/fs/commands/encode.py` & `spinta-0.1.9/spinta/backends/fs/commands/encode.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/fs/commands/init.py` & `spinta-0.1.9/spinta/backends/fs/commands/init.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/fs/commands/read.py` & `spinta-0.1.9/spinta/backends/fs/commands/read.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/fs/commands/validate.py` & `spinta-0.1.9/spinta/backends/fs/commands/validate.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/fs/commands/wipe.py` & `spinta-0.1.9/spinta/backends/fs/commands/wipe.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/fs/commands/write.py` & `spinta-0.1.9/spinta/backends/fs/commands/write.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/helpers.py` & `spinta-0.1.9/spinta/backends/helpers.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/memory/commands/manifest.py` & `spinta-0.1.9/spinta/backends/memory/commands/manifest.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/mongo/commands/changes.py` & `spinta-0.1.9/spinta/backends/mongo/commands/changes.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/mongo/commands/query.py` & `spinta-0.1.9/spinta/backends/mongo/commands/query.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/mongo/commands/read.py` & `spinta-0.1.9/spinta/backends/mongo/commands/read.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/mongo/commands/validate.py` & `spinta-0.1.9/spinta/backends/mongo/commands/validate.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/mongo/commands/wipe.py` & `spinta-0.1.9/spinta/backends/mongo/commands/wipe.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/mongo/commands/write.py` & `spinta-0.1.9/spinta/backends/mongo/commands/write.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/mongo/components.py` & `spinta-0.1.9/spinta/backends/mongo/components.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/mongo/types/array/write.py` & `spinta-0.1.9/spinta/backends/mongo/types/array/write.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/mongo/types/file/write.py` & `spinta-0.1.9/spinta/backends/mongo/types/file/write.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/mongo/types/object/write.py` & `spinta-0.1.9/spinta/backends/mongo/types/object/write.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/postgresql/commands/bootstrap.py` & `spinta-0.1.9/spinta/backends/postgresql/commands/bootstrap.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/postgresql/commands/changes.py` & `spinta-0.1.9/spinta/backends/postgresql/commands/changes.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/postgresql/commands/encode.py` & `spinta-0.1.9/spinta/backends/postgresql/commands/encode.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/postgresql/commands/freeze.py` & `spinta-0.1.9/spinta/backends/postgresql/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/postgresql/commands/init.py` & `spinta-0.1.9/spinta/backends/postgresql/commands/init.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from spinta.backends.postgresql.helpers.changes import get_changes_table
 
 
 @commands.prepare.register(Context, PostgreSQL, Manifest)
 def prepare(context: Context, backend: PostgreSQL, manifest: Manifest):
     # Prepare backend for models.
     for model in manifest.models.values():
-        if model.backend.name == backend.name:
+        if model.backend and model.backend.name == backend.name:
             commands.prepare(context, backend, model)
 
 
 @commands.prepare.register(Context, PostgreSQL, Model)
 def prepare(context: Context, backend: PostgreSQL, model: Model):
     columns = []
     for prop in model.properties.values():
```

### Comparing `spinta-0.1.8/spinta/backends/postgresql/commands/load.py` & `spinta-0.1.9/spinta/backends/postgresql/commands/load.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/postgresql/commands/manifest.py` & `spinta-0.1.9/spinta/backends/postgresql/commands/manifest.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/postgresql/commands/migrate.py` & `spinta-0.1.9/spinta/backends/postgresql/commands/migrate.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/postgresql/commands/query.py` & `spinta-0.1.9/spinta/backends/postgresql/commands/query.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/postgresql/commands/read.py` & `spinta-0.1.9/spinta/backends/postgresql/commands/read.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/postgresql/commands/validate.py` & `spinta-0.1.9/spinta/backends/postgresql/commands/validate.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/postgresql/commands/wait.py` & `spinta-0.1.9/spinta/backends/postgresql/commands/wait.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/postgresql/commands/wipe.py` & `spinta-0.1.9/spinta/backends/postgresql/commands/wipe.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/postgresql/commands/write.py` & `spinta-0.1.9/spinta/backends/postgresql/commands/write.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/postgresql/components.py` & `spinta-0.1.9/spinta/backends/postgresql/components.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/postgresql/files.py` & `spinta-0.1.9/spinta/backends/postgresql/files.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/postgresql/helpers/__init__.py` & `spinta-0.1.9/spinta/backends/postgresql/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/postgresql/helpers/changes.py` & `spinta-0.1.9/spinta/backends/postgresql/helpers/changes.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/postgresql/helpers/manifest.py` & `spinta-0.1.9/spinta/backends/postgresql/helpers/manifest.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/postgresql/helpers/validate.py` & `spinta-0.1.9/spinta/backends/postgresql/helpers/validate.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/postgresql/types/array/freeze.py` & `spinta-0.1.9/spinta/backends/postgresql/types/array/freeze.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/postgresql/types/array/init.py` & `spinta-0.1.9/spinta/backends/postgresql/types/array/init.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/postgresql/types/array/wipe.py` & `spinta-0.1.9/spinta/backends/postgresql/types/array/wipe.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/postgresql/types/array/write.py` & `spinta-0.1.9/spinta/backends/postgresql/types/array/write.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/postgresql/types/file/freeze.py` & `spinta-0.1.9/spinta/backends/postgresql/types/file/freeze.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/postgresql/types/file/init.py` & `spinta-0.1.9/spinta/backends/postgresql/types/file/init.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/postgresql/types/file/read.py` & `spinta-0.1.9/spinta/backends/postgresql/types/file/read.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/postgresql/types/file/write.py` & `spinta-0.1.9/spinta/backends/postgresql/types/file/write.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/postgresql/types/object/freeze.py` & `spinta-0.1.9/spinta/backends/postgresql/types/object/freeze.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/postgresql/types/object/init.py` & `spinta-0.1.9/spinta/backends/postgresql/types/object/init.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/postgresql/types/object/read.py` & `spinta-0.1.9/spinta/backends/postgresql/types/object/read.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/postgresql/types/ref/freeze.py` & `spinta-0.1.9/spinta/backends/postgresql/types/ref/freeze.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/postgresql/types/ref/init.py` & `spinta-0.1.9/spinta/backends/postgresql/types/ref/init.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/postgresql/types/ref/validate.py` & `spinta-0.1.9/spinta/backends/postgresql/types/ref/validate.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/backends/s3.py` & `spinta-0.1.9/spinta/backends/s3.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/cli/auth.py` & `spinta-0.1.9/spinta/cli/auth.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/cli/config.py` & `spinta-0.1.9/spinta/cli/config.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/cli/data.py` & `spinta-0.1.9/spinta/cli/data.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/cli/helpers/auth.py` & `spinta-0.1.9/spinta/cli/helpers/auth.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/cli/helpers/data.py` & `spinta-0.1.9/spinta/cli/helpers/data.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/cli/helpers/store.py` & `spinta-0.1.9/spinta/cli/helpers/store.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,15 +18,16 @@
     store = load_store(context)
     commands.link(context, store)
     commands.check(context, store)
     commands.prepare(context, store)
     return store
 
 
-def prepare_manifest(context: Context) -> Store:
+def prepare_manifest(context: Context, *, verbose: bool = True) -> Store:
     store = load_store(context)
-    click.echo(f"Loading manifest {store.manifest.name}...")
+    if verbose:
+        click.echo(f"Loading manifest {store.manifest.name}...")
     commands.load(context, store.manifest)
     commands.link(context, store.manifest)
     commands.check(context, store.manifest)
     commands.prepare(context, store.manifest)
     return store
```

### Comparing `spinta-0.1.8/spinta/cli/inspect.py` & `spinta-0.1.9/spinta/cli/inspect.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 import pathlib
 from typing import Optional
 from typing import TextIO
 from typing import Tuple
 
+from typer import Argument
 from typer import Context as TyperContext
 from typer import Option
+from typer import echo
 
 from spinta import commands
 from spinta.cli.helpers.auth import require_auth
 from spinta.cli.helpers.store import load_store
 from spinta.cli.helpers.store import prepare_manifest
 from spinta.components import Context
 from spinta.core.config import RawConfig
 from spinta.manifests.components import Manifest
 from spinta.manifests.tabular.helpers import datasets_to_tabular
 from spinta.manifests.tabular.helpers import load_ascii_tabular_manifest
+from spinta.manifests.tabular.helpers import render_tabular_manifest
 from spinta.manifests.tabular.helpers import write_tabular_manifest
 
 
 def _save_manifest(manifest: Manifest, dest: TextIO):
     # TODO: Currently saving is hardcoded to tabular manifest type, but it
     #       should be possible to save or probably freeze to any manifest type.
     rows = datasets_to_tabular(manifest)
     write_tabular_manifest(dest, rows)
 
 
 def inspect(
     ctx: TyperContext,
+    manifest: Optional[pathlib.Path] = Argument(None, help="Path to manifest."),
     resource: Optional[Tuple[str, str]] = Option((None, None), '-r', '--resource', help=(
         "Resource type and source URI (-r sql sqlite:////tmp/db.sqlite)"
     )),
     formula: str = Option('', '-f', '--formula', help=(
         "Formula if needed, to prepare resource for reading"
     )),
     output: Optional[pathlib.Path] = Option(None, '-o', '--output', help=(
@@ -48,15 +52,15 @@
         config = {
             'backends.null': {
                 'type': 'memory',
             },
             'manifests.inspect': {
                 'type': 'tabular',
                 'backend': 'null',
-                'keymap': 'default',
+                'keymap': '',
                 'mode': 'external',
                 'path': None,
             },
             'manifest': 'inspect',
         }
 
         # Add given manifest file to configuration
@@ -68,20 +72,42 @@
         d | r               | type            | source            | prepare
         dataset             |                 |                   |
           | {resource_type} | {resource_type} | {resource_source} | {formula}
         ''', strip=True)
         commands.check(context, store.manifest)
         commands.prepare(context, store.manifest)
 
+    elif manifest:
+        config = {
+            'backends': [],
+            'manifest': 'inspect',
+            'manifests.inspect': {
+                'type': 'tabular',
+                'backend': '',
+                'keymap': '',
+                'mode': 'internal',
+                'path': manifest,
+            },
+        }
+
+        # Add given manifest file to configuration
+        rc: RawConfig = context.get('rc')
+        context.set('rc', rc.fork(config))
+
+        # Load manifest
+        store = prepare_manifest(context)
+
     else:
         # Load manifest
         store = prepare_manifest(context)
 
     manifest = store.manifest
 
     with context:
         require_auth(context, auth)
         commands.inspect(context, manifest)
-        if output is None:
-            output = manifest.path
+
+    if output:
         with pathlib.Path(output).open('w') as f:
             _save_manifest(manifest, f)
+    else:
+        echo(render_tabular_manifest(manifest))
```

### Comparing `spinta-0.1.8/spinta/cli/main.py` & `spinta-0.1.9/spinta/cli/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,45 +4,51 @@
 import pathlib
 from typing import List
 from typing import Optional
 
 from typer import Context as TyperContext
 from typer import Option
 from typer import Typer
+from typer import echo
 
+import spinta
 from spinta.cli import auth
 from spinta.cli import config
 from spinta.cli import data
 from spinta.cli import inspect
 from spinta.cli import manifest
 from spinta.cli import migrate
 from spinta.cli import pii
 from spinta.cli import pull
 from spinta.cli import push
 from spinta.cli import server
+from spinta.cli.init import init
+from spinta.cli.show import show
 from spinta.cli.helpers.typer import add
 from spinta.core.context import create_context
 
 log = logging.getLogger(__name__)
 
 app = Typer()
 
 add(app, 'config', config.config, help="Show current configuration values")
 add(app, 'check', config.check, help="Check configuration and manifests")
 
 add(app, 'genkeys', auth.genkeys, help="Generate client token validation keys")
 add(app, 'token', auth.token, help="Tools for encoding/decode auth tokens")
 add(app, 'client', auth.client, help="Manage auth clients")
 
+add(app, 'init', init, help="Initialize new manifest table")
 add(app, 'inspect', inspect.inspect, help=(
     "Update manifest schema from an external data source"
 ))
 add(app, 'pii', pii.app, help="Manage Person Identifying Information")
 
-add(app, 'manifest', manifest.app, help="Manage manifests")
+add(app, 'copy', manifest.copy, help="Copy only specified metadata from a manifest")
+add(app, 'show', show, help="Show manifest as ascii table")
 
 add(app, 'bootstrap', migrate.bootstrap, help="Initialize backends")
 add(app, 'sync', migrate.sync, help="Sync source manifests into main manifest")
 add(app, 'migrate', migrate.migrate, help="Migrate schema changes to backends")
 add(app, 'freeze', migrate.freeze, help=(
     "Detect schema changes and create new schema version"
 ))
@@ -51,20 +57,23 @@
 add(app, 'pull', pull.pull, help="Pull data from an external data source")
 add(app, 'push', push.push, help="Push data into an external data store")
 
 add(app, 'run', server.run, help="Run development server")
 add(app, 'wait', server.wait, help="Wait while all backends are up")
 
 
-@app.callback()
+@app.callback(invoke_without_command=True)
 def main(
     ctx: TyperContext,
     option: Optional[List[str]] = Option(None, '-o', '--option', help=(
         "Set configuration option, example: `-o option.name=value`."
     )),
     env_file: Optional[pathlib.Path] = Option(None, '--env-file', help=(
         "Load configuration from a given .env file."
     )),
+    version: bool = Option(False, help="Show version number.")
 ):
     ctx.obj = ctx.obj or create_context('cli', args=option, envfile=env_file)
+    if version:
+        echo(spinta.__version__)
```

### Comparing `spinta-0.1.8/spinta/cli/manifest.py` & `spinta-0.1.9/spinta/cli/manifest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 app = Typer()
 
 
 @app.command(short_help="Copy manifest optionally transforming final copy")
 def copy(
     ctx: TyperContext,
-    external: bool = Option(True, help=(
+    source: bool = Option(True, help=(
         "Do not copy external data source metadata"
     )),
     # TODO: Change `str` to `Access`
     #       https://github.com/tiangolo/typer/issues/151
     access: str = Option('private', help=(
         "Copy properties with at least specified access"
     )),
@@ -37,15 +37,15 @@
     dest: pathlib.Path = Argument(None, help=(
         "Target manifest file to save a copy to"
     )),
 ):
     """Copy models from CSV manifest files into another CSV manifest file"""
     context: Context = ctx.obj
     access = get_enum_by_name(Access, access)
-    rows = _read_csv_files(context, files, external=external, access=access)
+    rows = _read_csv_files(context, files, external=source, access=access)
     with dest.open('w') as f:
         write_tabular_manifest(f, rows)
 
 
 def _read_csv_files(
     context: Context,
     files: List[pathlib.Path],
```

### Comparing `spinta-0.1.8/spinta/cli/migrate.py` & `spinta-0.1.9/spinta/cli/migrate.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/cli/pii.py` & `spinta-0.1.9/spinta/cli/pii.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/cli/pull.py` & `spinta-0.1.9/spinta/cli/pull.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/cli/push.py` & `spinta-0.1.9/spinta/cli/push.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/cli/server.py` & `spinta-0.1.9/spinta/cli/server.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/commands/__init__.py` & `spinta-0.1.9/spinta/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/commands/auth.py` & `spinta-0.1.9/spinta/commands/auth.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/commands/formats/ascii.py` & `spinta-0.1.9/spinta/commands/formats/ascii.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/commands/formats/csv.py` & `spinta-0.1.9/spinta/commands/formats/csv.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/commands/formats/html.py` & `spinta-0.1.9/spinta/commands/formats/html.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/commands/formats/json.py` & `spinta-0.1.9/spinta/commands/formats/json.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/commands/formats/jsonl.py` & `spinta-0.1.9/spinta/commands/formats/jsonl.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/commands/helpers.py` & `spinta-0.1.9/spinta/commands/helpers.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/commands/read.py` & `spinta-0.1.9/spinta/commands/read.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/commands/search.py` & `spinta-0.1.9/spinta/commands/search.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/commands/version.py` & `spinta-0.1.9/spinta/commands/version.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/commands/write.py` & `spinta-0.1.9/spinta/commands/write.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/compat.py` & `spinta-0.1.9/spinta/compat.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/components.py` & `spinta-0.1.9/spinta/components.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/config.py` & `spinta-0.1.9/spinta/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -114,32 +114,20 @@
         'html': 'spinta.commands.formats.html:Html',
     },
     'accesslog': {
         'type': 'file',
         'file': 'stdout',
         'buffer_size': 300,
     },
-    'backends': {
-        'default': {
-            'type': 'postgresql',
-            'dsn': 'postgresql://admin:admin123@localhost:54321/spinta',
-            'migrate': 'alembic',
-        },
-    },
     'manifests': {
         'default': {
-            'type': 'backend',
-            'backend': 'default',
-            'sync': 'yaml',
+            'type': 'memory',
+            'backend': '',
             'mode': 'internal',
-        },
-        'yaml': {
-            'type': 'yaml',
-            'backend': 'default',
-            'path': pathlib.Path(),
+            'keymap': '',
         },
     },
 
     'manifest': 'default',
 
     # Parameters for datasets, for example credentials. Example:
     #
@@ -158,15 +146,15 @@
 
     'debug': False,
 
     # How much time to wait in seconds for the backends to go up.
     'wait': 30,
 
     # Configuration path, where clients, keys and other things are stored.
-    'config_path': pathlib.Path('tests/config'),
+    'config_path': '',
 
     # Path to documentation folder. If set will serve the folder at `/docs`.
     'docs_path': None,
 
     'server_url': 'https://example.com/',
 
     # This prefix will be added to autogenerated scope names.
@@ -183,15 +171,15 @@
     'always_show_id': False,
 
     'default_auth_client': None,
 
     # Public JWK key for validating auth bearer tokens.
     'token_validation_key': None,
 
-    'env': 'dev',
+    'env': 'prod',
 
     'environments': {
         'dev': {
             'keymaps.default': {
                 'type': 'sqlalchemy',
                 'dsn': 'sqlite:///var/keymaps.db',
             },
@@ -222,18 +210,21 @@
                     'type': 'yaml',
                     'path': pathlib.Path() / 'tests/manifest',
                     'sync': None,
                     'keymap': 'default',
                     'mode': 'internal',
                 },
                 'yaml': {
+                    'type': 'yaml',
+                    'backend': 'default',
                     'path': pathlib.Path() / 'tests/manifest',
                 },
             },
             'default_auth_client': '3388ea36-4a4f-4821-900a-b574c8829d52',
+            'config_path': pathlib.Path('tests/config'),
         },
         'test': {
             'accesslog': {
                 'type': 'python',
             },
             'backends': {
                 'default': {
@@ -259,16 +250,22 @@
             },
             'manifests': {
                 # TODO: remove `default` manifest
                 'default': {
                     'type': 'yaml',
                     'path': pathlib.Path() / 'tests/manifest',
                     'sync': None,
+                    'backend': 'default',
                     'keymap': 'default',
                     'mode': 'internal',
                 },
+                'yaml': {
+                    'type': 'yaml',
+                    'backend': 'default',
+                    'path': pathlib.Path() / 'tests/manifest',
+                },
             },
             'config_path': pathlib.Path('tests/config'),
             'default_auth_client': 'baa448a8-205c-4faa-a048-a10e4b32a136',
         }
     },
 }
```

### Comparing `spinta-0.1.8/spinta/config.yml` & `spinta-0.1.9/spinta/config.yml`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/core/access.py` & `spinta-0.1.9/spinta/core/access.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/core/config.py` & `spinta-0.1.9/spinta/core/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -305,15 +305,15 @@
         )
         if file:
             for row in table:
                 print('  '.join([str(x).ljust(s) for x, s in zip(row, sizes)]), file=file)
         else:
             return table
 
-    def to_dict(self, *names) -> Dict[str, Any]:
+    def to_dict(self, *names: str) -> Dict[str, Any]:
         result = {}
         for key, val in self.getall(*names):
             key = '.'.join(key[len(names):])
             result[key] = val
         return result
 
     def _update_keys(self) -> Dict[Key, List[str]]:
```

### Comparing `spinta-0.1.8/spinta/core/context.py` & `spinta-0.1.9/spinta/core/context.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/core/enums.py` & `spinta-0.1.9/spinta/core/enums.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/core/ufuncs.py` & `spinta-0.1.9/spinta/core/ufuncs.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/datasets/backends/csv/commands.py` & `spinta-0.1.9/spinta/datasets/backends/csv/commands.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/datasets/backends/sql/commands/inspect.py` & `spinta-0.1.9/spinta/datasets/backends/sql/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/datasets/backends/sql/commands/query.py` & `spinta-0.1.9/spinta/datasets/backends/sql/commands/query.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/datasets/backends/sql/commands/read.py` & `spinta-0.1.9/spinta/datasets/backends/sql/commands/read.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/datasets/backends/sql/commands/wait.py` & `spinta-0.1.9/spinta/datasets/backends/sql/commands/wait.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/datasets/backends/sql/components.py` & `spinta-0.1.9/spinta/datasets/backends/sql/components.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/datasets/backends/sqldump/commands/inspect.py` & `spinta-0.1.9/spinta/datasets/backends/sqldump/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/datasets/backends/sqldump/commands/load.py` & `spinta-0.1.9/spinta/datasets/backends/sqldump/commands/load.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/datasets/backends/sqldump/components.py` & `spinta-0.1.9/spinta/datasets/backends/sqldump/components.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/datasets/backends/sqldump/ufuncs/ufuncs.py` & `spinta-0.1.9/spinta/datasets/backends/sqldump/ufuncs/ufuncs.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/datasets/commands/error.py` & `spinta-0.1.9/spinta/datasets/commands/error.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/datasets/commands/link.py` & `spinta-0.1.9/spinta/datasets/commands/link.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/datasets/commands/load.py` & `spinta-0.1.9/spinta/datasets/commands/load.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/datasets/commands/read.py` & `spinta-0.1.9/spinta/datasets/commands/read.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/datasets/components.py` & `spinta-0.1.9/spinta/datasets/components.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/datasets/helpers.py` & `spinta-0.1.9/spinta/datasets/helpers.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/datasets/keymaps/sqlalchemy.py` & `spinta-0.1.9/spinta/datasets/keymaps/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/dimensions/prefix/components.py` & `spinta-0.1.9/spinta/dimensions/prefix/components.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/dimensions/prefix/helpers.py` & `spinta-0.1.9/spinta/dimensions/prefix/helpers.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/dispatcher.py` & `spinta-0.1.9/spinta/dispatcher.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/exceptions.py` & `spinta-0.1.9/spinta/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -449,14 +449,18 @@
     template = "Key map is not configured."
 
 
 class BackendNotFound(UserError):
     template = "Can't find backend {name!r}."
 
 
+class NoBackendConfigured(UserError):
+    template = "Backend is not configured, can't proceed the request."
+
+
 class UnexpectedFormulaResult(UserError):
     template = (
         "Unexpected formula {formula} result. "
         "Expected {expected}, instead got a {received}."
     )
```

### Comparing `spinta-0.1.8/spinta/fetcher.py` & `spinta-0.1.9/spinta/fetcher.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/hacks/spyna.py` & `spinta-0.1.9/spinta/hacks/spyna.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/manifest/_schema/version.yml` & `spinta-0.1.9/spinta/manifest/_schema/version.yml`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/manifest/_schema.yml` & `spinta-0.1.9/spinta/manifest/_schema.yml`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/manifest/_txn.yml` & `spinta-0.1.9/spinta/manifest/_txn.yml`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/manifests/backend/commands/bootstrap.py` & `spinta-0.1.9/spinta/manifests/backend/commands/bootstrap.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/manifests/backend/commands/load.py` & `spinta-0.1.9/spinta/manifests/backend/commands/load.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/manifests/backend/commands/manifest.py` & `spinta-0.1.9/spinta/manifests/backend/commands/manifest.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/manifests/backend/commands/migrate.py` & `spinta-0.1.9/spinta/manifests/backend/commands/migrate.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/manifests/backend/commands/sync.py` & `spinta-0.1.9/spinta/manifests/backend/commands/sync.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/manifests/backend/helpers.py` & `spinta-0.1.9/spinta/manifests/backend/helpers.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/manifests/commands/check.py` & `spinta-0.1.9/spinta/manifests/commands/check.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/manifests/commands/error.py` & `spinta-0.1.9/spinta/manifests/commands/error.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/manifests/components.py` & `spinta-0.1.9/spinta/manifests/components.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/manifests/helpers.py` & `spinta-0.1.9/spinta/manifests/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 def create_manifest(
     context: Context,
     store: Store,
     name: str,
     seen: List[str] = None,
 ) -> Manifest:
-    rc = context.get('rc')
+    rc: RawConfig = context.get('rc')
     config = context.get('config')
     mtype = rc.get('manifests', name, 'type', required=True)
     Manifest = config.components['manifests'][mtype]
     manifest = Manifest()
     manifest.type = mtype
     _configure_manifest(context, rc, config, store, manifest, name, seen)
     return manifest
@@ -37,15 +37,15 @@
 def create_internal_manifest(context: Context, store: Store) -> InternalManifest:
     rc = context.get('rc')
     config = context.get('config')
     manifest = InternalManifest()
     manifest.type = 'yaml'
     _configure_manifest(
         context, rc, config, store, manifest, 'internal',
-        backend=store.manifest.backend.name,
+        backend=store.manifest.backend.name if store.manifest.backend else None,
     )
     return manifest
 
 
 def _configure_manifest(
     context: Context,
     rc: RawConfig,
@@ -62,15 +62,15 @@
     manifest.store = store
     manifest.parent = None
     manifest.access = rc.get('manifests', name, 'access') or 'protected'
     manifest.access = enum_by_name(manifest, 'access', Access, manifest.access)
     manifest.keymap = rc.get('manifests', name, 'keymap', default=None)
     manifest.keymap = store.keymaps[manifest.keymap] if manifest.keymap else None
     manifest.backend = rc.get('manifests', name, 'backend', default=backend)
-    manifest.backend = store.backends[manifest.backend]
+    manifest.backend = store.backends[manifest.backend] if manifest.backend else None
     manifest.endpoints = {}
     manifest.backends = {}
     manifest.objects = {name: {} for name in config.components['nodes']}
     manifest.sync = []
     manifest.prefixes = {}
     manifest.mode = enum_by_name(manifest, 'mode', Mode, (
         rc.get('manifests', name, 'mode') or 'internal'
```

### Comparing `spinta-0.1.8/spinta/manifests/internal/commands/load.py` & `spinta-0.1.9/spinta/manifests/internal/commands/load.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/manifests/tabular/commands/configure.py` & `spinta-0.1.9/spinta/manifests/tabular/commands/configure.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/manifests/tabular/commands/load.py` & `spinta-0.1.9/spinta/manifests/tabular/commands/load.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/manifests/tabular/helpers.py` & `spinta-0.1.9/spinta/manifests/tabular/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import pathlib
 import textwrap
 from typing import Any
 from typing import Dict
 from typing import Iterable
 from typing import Iterator
 from typing import List
+from typing import List
 from typing import Optional
 from typing import Set
 from typing import TextIO
 from typing import Tuple
 from typing import TypedDict
 
 from spinta import commands
@@ -20,16 +21,18 @@
 from spinta.components import Context
 from spinta.components import Model
 from spinta.core.enums import Access
 from spinta.core.ufuncs import unparse
 from spinta.datasets.components import Dataset
 from spinta.dimensions.prefix.components import UriPrefix
 from spinta.manifests.components import Manifest
+from spinta.manifests.components import Manifest
 from spinta.manifests.helpers import load_manifest_nodes
 from spinta.manifests.tabular.constants import DATASET
+from spinta.manifests.tabular.constants import DATASET
 from spinta.types.datatype import Ref
 from spinta.utils.data import take
 from spinta.utils.schema import NA
 
 ParsedRow = Tuple[int, Dict[str, Any]]
 
 
@@ -839,7 +842,69 @@
 
 SHORT_NAMES = {
     'd': 'dataset',
     'r': 'resource',
     'b': 'base',
     'm': 'model',
 }
+
+
+def render_tabular_manifest(manifest: Manifest, cols: List[str] = None) -> str:
+    rows = datasets_to_tabular(manifest)
+    cols = cols or DATASET
+    hs = 1 if 'id' in cols else 0  # hierarchical cols start
+    he = cols.index('property')    # hierarchical cols end
+    hsize = 1                      # hierarchical column size
+    bsize = 3                      # border size
+    sizes = dict(
+        [(c, len(c)) for c in cols[:hs]] +
+        [(c, 1) for c in cols[hs:he]] +
+        [(c, len(c)) for c in cols[he:]]
+    )
+    rows = list(rows)
+    for row in rows:
+        for i, col in enumerate(cols):
+            val = '' if row[col] is None else str(row[col])
+            if col == 'id':
+                sizes[col] = 2
+            elif i < he:
+                size = (hsize + bsize) * (he - hs - i) + sizes['property']
+                if size < len(val):
+                    sizes['property'] += len(val) - size
+            elif sizes[col] < len(val):
+                sizes[col] = len(val)
+
+    line = []
+    for col in cols:
+        size = sizes[col]
+        line.append(col[:size].ljust(size))
+    lines = [line]
+
+    for row in rows:
+        if 'id' in cols:
+            line = [row['id'][:2] if row['id'] else '  ']
+        else:
+            line = []
+
+        for i, col in enumerate(cols[hs:he + 1]):
+            val = row[col] or ''
+            if val:
+                depth = i
+                break
+        else:
+            val = ''
+            depth = 0
+
+        line += [' ' * hsize] * depth
+        size = (hsize + bsize) * (he - hs - depth) + sizes['property']
+        line += [val.ljust(size)]
+
+        for col in cols[he + 1:]:
+            val = '' if row[col] is None else str(row[col])
+            size = sizes[col]
+            line.append(val.ljust(size))
+
+        lines.append(line)
+
+    lines = [' | '.join(line) for line in lines]
+    lines = [l.rstrip() for l in lines]
+    return '\n'.join(lines)
```

### Comparing `spinta-0.1.8/spinta/manifests/yaml/commands/freeze.py` & `spinta-0.1.9/spinta/manifests/yaml/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/manifests/yaml/commands/load.py` & `spinta-0.1.9/spinta/manifests/yaml/commands/load.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/manifests/yaml/commands/manifest.py` & `spinta-0.1.9/spinta/manifests/yaml/commands/manifest.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/manifests/yaml/helpers.py` & `spinta-0.1.9/spinta/manifests/yaml/helpers.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/middlewares.py` & `spinta-0.1.9/spinta/middlewares.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/migrations/__init__.py` & `spinta-0.1.9/spinta/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/migrations/schema/alembic.py` & `spinta-0.1.9/spinta/migrations/schema/alembic.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/nodes.py` & `spinta-0.1.9/spinta/nodes.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/renderer.py` & `spinta-0.1.9/spinta/renderer.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/spyna.py` & `spinta-0.1.9/spinta/spyna.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/templates/base.html` & `spinta-0.1.9/spinta/templates/base.html`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/testing/cli.py` & `spinta-0.1.9/spinta/testing/cli.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/testing/client.py` & `spinta-0.1.9/spinta/testing/client.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/testing/config.py` & `spinta-0.1.9/spinta/testing/config.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/testing/context.py` & `spinta-0.1.9/spinta/testing/context.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/testing/data.py` & `spinta-0.1.9/spinta/testing/data.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/testing/datasets.py` & `spinta-0.1.9/spinta/testing/datasets.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/testing/dtypes.py` & `spinta-0.1.9/spinta/testing/dtypes.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/testing/pytest.py` & `spinta-0.1.9/spinta/testing/pytest.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/testing/ufuncs.py` & `spinta-0.1.9/spinta/testing/ufuncs.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/testing/utils.py` & `spinta-0.1.9/spinta/testing/utils.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/types/command.py` & `spinta-0.1.9/spinta/types/command.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/types/config.py` & `spinta-0.1.9/spinta/types/config.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/types/datatype.py` & `spinta-0.1.9/spinta/types/datatype.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/types/file/decode.py` & `spinta-0.1.9/spinta/types/file/decode.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/types/file/helpers.py` & `spinta-0.1.9/spinta/types/file/helpers.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/types/helpers.py` & `spinta-0.1.9/spinta/types/helpers.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/types/model.py` & `spinta-0.1.9/spinta/types/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,16 +38,14 @@
     model.mode = manifest.mode  # TODO: mode should be inherited from namespace.
     load_node(context, model, data)
 
     if model.keymap:
         model.keymap = manifest.store.keymaps[model.keymap]
     else:
         model.keymap = manifest.keymap
-    if model.external and model.keymap is None:
-        raise exceptions.NoKeyMap(model)
 
     manifest.add_model_endpoint(model)
     load_namespace(context, manifest, model)
     model.access = load_access_param(model, model.access)
     load_model_properties(context, model, Property, data.get('properties'))
 
     # XXX: Maybe it is worth to leave possibility to override _id access?
```

### Comparing `spinta-0.1.8/spinta/types/namespace.py` & `spinta-0.1.9/spinta/types/namespace.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/types/owner.py` & `spinta-0.1.9/spinta/types/owner.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/types/project.py` & `spinta-0.1.9/spinta/types/project.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/types/ref/link.py` & `spinta-0.1.9/spinta/types/ref/link.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/types/store.py` & `spinta-0.1.9/spinta/types/store.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/ufuncs.py` & `spinta-0.1.9/spinta/ufuncs.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/urlparams.py` & `spinta-0.1.9/spinta/urlparams.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/utils/aiotools.py` & `spinta-0.1.9/spinta/utils/aiotools.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/utils/data.py` & `spinta-0.1.9/spinta/utils/data.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/utils/itertools.py` & `spinta-0.1.9/spinta/utils/itertools.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/utils/json.py` & `spinta-0.1.9/spinta/utils/json.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/utils/naming.py` & `spinta-0.1.9/spinta/utils/naming.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/utils/nestedstruct.py` & `spinta-0.1.9/spinta/utils/nestedstruct.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/utils/nin.py` & `spinta-0.1.9/spinta/utils/nin.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/utils/passwords.py` & `spinta-0.1.9/spinta/utils/passwords.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/utils/path.py` & `spinta-0.1.9/spinta/utils/path.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/utils/refs.py` & `spinta-0.1.9/spinta/utils/refs.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/utils/response.py` & `spinta-0.1.9/spinta/utils/response.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,28 +3,31 @@
 
 from starlette.requests import Request
 
 from spinta import commands
 from spinta.commands.formats import Format
 from spinta.components import Context, Action, UrlParams, Node
 from spinta import exceptions
-
+from spinta.exceptions import NoBackendConfigured
 
 METHOD_TO_ACTION = {
     'POST': Action.INSERT,
     'PUT': Action.UPDATE,
     'PATCH': Action.PATCH,
     'DELETE': Action.DELETE,
 }
 
 
 async def create_http_response(context: Context, params: UrlParams, request: Request):
     store = context.get('store')
     manifest = store.manifest
 
+    if manifest.backend is None:
+        raise NoBackendConfigured(manifest)
+
     if request.method == 'GET':
         context.attach('transaction', manifest.backend.transaction)
 
         if params.changes:
             _enforce_limit(context, params)
             return await commands.changes(context, request, params.model, params.model.backend, action=Action.CHANGES, params=params)
```

### Comparing `spinta-0.1.8/spinta/utils/schema.py` & `spinta-0.1.9/spinta/utils/schema.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/utils/scopes.py` & `spinta-0.1.9/spinta/utils/scopes.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/utils/streams.py` & `spinta-0.1.9/spinta/utils/streams.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/utils/tree.py` & `spinta-0.1.9/spinta/utils/tree.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/utils/units.py` & `spinta-0.1.9/spinta/utils/units.py`

 * *Files identical despite different names*

### Comparing `spinta-0.1.8/spinta/utils/url.py` & `spinta-0.1.9/spinta/utils/url.py`

 * *Files identical despite different names*

