# Comparing `tmp/TDhelper-2.5.4.tar.gz` & `tmp/TDhelper-2.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TDhelper-2.5.4.tar", last modified: Mon Jun 19 15:24:43 2023, max compression
+gzip compressed data, was "TDhelper-2.5.5.tar", last modified: Tue Jun 20 13:48:28 2023, max compression
```

## Comparing `TDhelper-2.5.4.tar` & `TDhelper-2.5.5.tar`

### file list

```diff
@@ -1,227 +1,227 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.155065 TDhelper-2.5.4/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11361 2023-04-03 05:53:54.000000 TDhelper-2.5.4/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2889 2023-06-19 15:24:43.155065 TDhelper-2.5.4/PKG-INFO
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2573 2023-04-03 05:53:54.000000 TDhelper-2.5.4/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.115065 TDhelper-2.5.4/TDhelper/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.115065 TDhelper-2.5.4/TDhelper/Decorators/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/Decorators/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      904 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/Decorators/log.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      649 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/Decorators/performance.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.115065 TDhelper-2.5.4/TDhelper/Event/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4150 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/Event/Event.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/Event/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.115065 TDhelper-2.5.4/TDhelper/Event/classEvent/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/Event/classEvent/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1273 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/Event/classEvent/event.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      966 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/Event/classEvent/meta.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.115065 TDhelper-2.5.4/TDhelper/Event/webEvent/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    31736 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/Event/webEvent/Events.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/Event/webEvent/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.115065 TDhelper-2.5.4/TDhelper/MagicCls/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      105 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/MagicCls/FieldsType.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1740 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/MagicCls/MagicMeta.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       74 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/MagicCls/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1978 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/MagicCls/model.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      892 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/MagicCls/test.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.115065 TDhelper-2.5.4/TDhelper/Msg/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1165 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/Msg/AppPush.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2564 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/Msg/Config.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2170 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/Msg/Email.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1438 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/Msg/InterfaceMsg.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2113 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/Msg/SMS.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/Msg/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.125065 TDhelper-2.5.4/TDhelper/Scheduler/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/Scheduler/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      742 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/Scheduler/base.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      750 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/Scheduler/example_scheduler.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      828 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/Scheduler/interface.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1620 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/Scheduler/log_config.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4208 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/Scheduler/service.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.125065 TDhelper-2.5.4/TDhelper/Spider/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/Spider/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       63 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/Spider/cfg.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     8502 2023-06-12 08:38:42.000000 TDhelper-2.5.4/TDhelper/Spider/contentExtraction.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.125065 TDhelper-2.5.4/TDhelper/Spider/models/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      976 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/Spider/models/BadRequestModel.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2619 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/Spider/models/Cache_L1.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1332 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/Spider/models/Cache_L2.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2137 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/Spider/models/Cache_L2_Model.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/Spider/models/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      853 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/Spider/models/fingerprint.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      243 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/Spider/models/spider_event.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1702 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/Spider/models/status.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    43496 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/Spider/regex.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       50 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/Spider/spiderFactory.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    10838 2023-05-14 08:23:04.000000 TDhelper-2.5.4/TDhelper/Spider/spiderPools.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       73 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5366 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/apiCore.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.125065 TDhelper-2.5.4/TDhelper/bin/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/bin/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      541 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/bin/globalvar.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.125065 TDhelper-2.5.4/TDhelper/cache/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/cache/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      948 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/cache/memcache.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1130 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/cache/pools.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2739 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/cache/ring.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.125065 TDhelper-2.5.4/TDhelper/cache/webCache/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/cache/webCache/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      861 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/cache/webCache/interface.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2963 2023-04-26 14:20:15.000000 TDhelper-2.5.4/TDhelper/cache/webCache/mongo.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/cache/webCache/redis.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1228 2023-05-16 14:29:26.000000 TDhelper-2.5.4/TDhelper/cache/webCache/webCacheFactory.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.125065 TDhelper-2.5.4/TDhelper/db/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.125065 TDhelper-2.5.4/TDhelper/db/Db/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/db/Db/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1235 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/db/Db/base.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      238 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/db/Db/helper.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/db/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.125065 TDhelper-2.5.4/TDhelper/db/mongodb/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/db/mongodb/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1102 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/db/mongodb/base.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3718 2023-04-26 14:07:17.000000 TDhelper-2.5.4/TDhelper/db/mongodb/dbhelper.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1919 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/db/mongodb/objectId.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       44 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/db/mongodb/setting.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.125065 TDhelper-2.5.4/TDhelper/db/mysql/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/db/mysql/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      510 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/db/mysql/base.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/db/mysql/model.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1151 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/db/mysql/mysql_x.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      126 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/db/mysql/setting.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.125065 TDhelper-2.5.4/TDhelper/document/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       24 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/document/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.125065 TDhelper-2.5.4/TDhelper/document/excel/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.125065 TDhelper-2.5.4/TDhelper/document/excel/FieldType/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      104 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/document/excel/FieldType/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       36 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/document/excel/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.125065 TDhelper-2.5.4/TDhelper/document/excel/meta/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       21 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/document/excel/meta/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3854 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/document/excel/meta/modelMeta.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      818 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/document/excel/model.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      622 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/document/file.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.125065 TDhelper-2.5.4/TDhelper/document/ini/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/document/ini/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      123 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/document/ini/fields.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1718 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/document/ini/meta.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      440 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/document/ini/model.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      314 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/document/ini/test.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.135065 TDhelper-2.5.4/TDhelper/generic/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2220 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/generic/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.135065 TDhelper-2.5.4/TDhelper/generic/a/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/generic/a/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       48 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/generic/a/b.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1402 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/generic/classDocCfg.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.135065 TDhelper-2.5.4/TDhelper/generic/crypto/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1413 2023-05-16 14:56:25.000000 TDhelper-2.5.4/TDhelper/generic/crypto/MD5.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/generic/crypto/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4668 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/generic/dictHelper.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.135065 TDhelper-2.5.4/TDhelper/generic/dynamic/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/generic/dynamic/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.135065 TDhelper-2.5.4/TDhelper/generic/dynamic/base/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2582 2023-06-16 12:40:51.000000 TDhelper-2.5.4/TDhelper/generic/dynamic/base/Meta.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/generic/dynamic/base/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2825 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/generic/dynamic/test.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1417 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/generic/findAttribute.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      144 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/generic/randGetValue.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1146 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/generic/recursion.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5628 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/generic/requier.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3721 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/generic/standard_result.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4808 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/generic/threadPools.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3886 2023-05-16 14:56:32.000000 TDhelper-2.5.4/TDhelper/generic/transformationType.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.135065 TDhelper-2.5.4/TDhelper/network/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/network/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.135065 TDhelper-2.5.4/TDhelper/network/http/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7978 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/network/http/REST_HTTP.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    61039 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/network/http/RPC.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    34603 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/network/http/RPC1.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/network/http/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4663 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/network/http/http_helper.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3588 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/network/http/http_postdataformat.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    26267 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/network/http/m3u8.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    26805 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/network/http/m3u8_backup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.135065 TDhelper-2.5.4/TDhelper/network/http/status/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      165 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/network/http/status/M3U8_STATUS.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/network/http/status/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.135065 TDhelper-2.5.4/TDhelper/network/rpc/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.135065 TDhelper-2.5.4/TDhelper/network/rpc/Client/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/network/rpc/Client/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4800 2023-05-14 13:08:38.000000 TDhelper-2.5.4/TDhelper/network/rpc/Client/rpc.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12549 2023-06-19 15:23:41.000000 TDhelper-2.5.4/TDhelper/network/rpc/Client/service.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.135065 TDhelper-2.5.4/TDhelper/network/rpc/Core/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2141 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/network/rpc/Core/Meta.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/network/rpc/Core/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    16253 2023-05-19 10:18:42.000000 TDhelper-2.5.4/TDhelper/network/rpc/Core/struct.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.135065 TDhelper-2.5.4/TDhelper/network/rpc/Generic/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7381 2023-05-14 10:09:53.000000 TDhelper-2.5.4/TDhelper/network/rpc/Generic/Host.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/network/rpc/Generic/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.145065 TDhelper-2.5.4/TDhelper/network/rpc/Server/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/network/rpc/Server/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7837 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/network/rpc/Server/obsolete_Service.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4207 2023-05-14 12:54:46.000000 TDhelper-2.5.4/TDhelper/network/rpc/Server/server.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.145065 TDhelper-2.5.4/TDhelper/network/rpc/Struct/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2202 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/network/rpc/Struct/Result.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/network/rpc/Struct/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/network/rpc/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.145065 TDhelper-2.5.4/TDhelper/network/socket/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2001 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/network/socket/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.145065 TDhelper-2.5.4/TDhelper/network/socket/cache/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/network/socket/cache/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      518 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/network/socket/cache/queue.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2371 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/network/socket/client.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.145065 TDhelper-2.5.4/TDhelper/network/socket/model/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      757 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/network/socket/model/SOCKET_MODELS.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/network/socket/model/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.145065 TDhelper-2.5.4/TDhelper/network/socket/protocol/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/network/socket/protocol/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4531 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/network/socket/protocol/base.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4163 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/network/socket/server.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.145065 TDhelper-2.5.4/TDhelper/network/websocket/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/network/websocket/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3485 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/network/websocket/protocol.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1433 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/network/websocket/server.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1901 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/reflect.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.145065 TDhelper-2.5.4/TDhelper/robot/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/robot/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.145065 TDhelper-2.5.4/TDhelper/robot/control/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1149 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/robot/control/D_33890.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/robot/control/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1296 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/robot/control/device.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.145065 TDhelper-2.5.4/TDhelper/robot/people/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1117 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/robot/people/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5622 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/robot/people/leg.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.145065 TDhelper-2.5.4/TDhelper/robot/people/scripts/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/robot/people/scripts/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3111 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/robot/people/scripts/runScript.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1142 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/robot/people/scripts/script.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/robot/people/upperLimb.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/robot/people/vertebra.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.145065 TDhelper-2.5.4/TDhelper/robot/struct/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/robot/struct/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      621 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/robot/struct/ankle.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2131 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/robot/struct/base.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      613 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/robot/struct/hip.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      618 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/robot/struct/knee.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      697 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/robot/struct/toe.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.145065 TDhelper-2.5.4/TDhelper/shellScripts/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      335 2023-04-06 02:34:35.000000 TDhelper-2.5.4/TDhelper/shellScripts/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3190 2023-05-07 06:20:59.000000 TDhelper-2.5.4/TDhelper/shellScripts/saasHelper.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.145065 TDhelper-2.5.4/TDhelper/simulate/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/simulate/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2713 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/simulate/json.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.155065 TDhelper-2.5.4/TDhelper/structs/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/structs/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4359 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/structs/dir.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.155065 TDhelper-2.5.4/TDhelper/web/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/web/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     8255 2023-04-03 05:53:54.000000 TDhelper-2.5.4/TDhelper/web/permission.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     6908 2023-06-18 14:41:48.000000 TDhelper-2.5.4/TDhelper/web/permissionHelper.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.155065 TDhelper-2.5.4/TDhelper/web/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-18 14:42:30.000000 TDhelper-2.5.4/TDhelper/web/utils/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:24:43.115065 TDhelper-2.5.4/TDhelper.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2889 2023-06-19 15:24:42.000000 TDhelper-2.5.4/TDhelper.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5563 2023-06-19 15:24:43.000000 TDhelper-2.5.4/TDhelper.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-19 15:24:42.000000 TDhelper-2.5.4/TDhelper.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       62 2023-06-19 15:24:42.000000 TDhelper-2.5.4/TDhelper.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      754 2023-06-19 15:24:42.000000 TDhelper-2.5.4/TDhelper.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-06-19 15:24:42.000000 TDhelper-2.5.4/TDhelper.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-19 15:24:43.155065 TDhelper-2.5.4/setup.cfg
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1789 2023-06-19 15:23:57.000000 TDhelper-2.5.4/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.895109 TDhelper-2.5.5/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11361 2023-04-03 05:53:54.000000 TDhelper-2.5.5/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2889 2023-06-20 13:48:28.895109 TDhelper-2.5.5/PKG-INFO
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2573 2023-04-03 05:53:54.000000 TDhelper-2.5.5/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.845109 TDhelper-2.5.5/TDhelper/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.845109 TDhelper-2.5.5/TDhelper/Decorators/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/Decorators/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      904 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/Decorators/log.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      649 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/Decorators/performance.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.845109 TDhelper-2.5.5/TDhelper/Event/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4150 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/Event/Event.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/Event/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.845109 TDhelper-2.5.5/TDhelper/Event/classEvent/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/Event/classEvent/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1273 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/Event/classEvent/event.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      966 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/Event/classEvent/meta.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.845109 TDhelper-2.5.5/TDhelper/Event/webEvent/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    31736 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/Event/webEvent/Events.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/Event/webEvent/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.855109 TDhelper-2.5.5/TDhelper/MagicCls/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      105 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/MagicCls/FieldsType.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1740 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/MagicCls/MagicMeta.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       74 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/MagicCls/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1978 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/MagicCls/model.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      892 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/MagicCls/test.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.855109 TDhelper-2.5.5/TDhelper/Msg/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1165 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/Msg/AppPush.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2564 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/Msg/Config.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2170 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/Msg/Email.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1438 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/Msg/InterfaceMsg.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2113 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/Msg/SMS.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/Msg/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.855109 TDhelper-2.5.5/TDhelper/Scheduler/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/Scheduler/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      742 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/Scheduler/base.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      750 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/Scheduler/example_scheduler.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      828 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/Scheduler/interface.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1620 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/Scheduler/log_config.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4208 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/Scheduler/service.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.855109 TDhelper-2.5.5/TDhelper/Spider/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/Spider/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       63 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/Spider/cfg.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     8502 2023-06-12 08:38:42.000000 TDhelper-2.5.5/TDhelper/Spider/contentExtraction.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.855109 TDhelper-2.5.5/TDhelper/Spider/models/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      976 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/Spider/models/BadRequestModel.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2619 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/Spider/models/Cache_L1.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1332 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/Spider/models/Cache_L2.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2137 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/Spider/models/Cache_L2_Model.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/Spider/models/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      853 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/Spider/models/fingerprint.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      243 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/Spider/models/spider_event.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1702 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/Spider/models/status.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    43496 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/Spider/regex.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       50 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/Spider/spiderFactory.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    10838 2023-05-14 08:23:04.000000 TDhelper-2.5.5/TDhelper/Spider/spiderPools.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       73 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5366 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/apiCore.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.855109 TDhelper-2.5.5/TDhelper/bin/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/bin/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      541 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/bin/globalvar.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.865109 TDhelper-2.5.5/TDhelper/cache/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/cache/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      948 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/cache/memcache.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1130 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/cache/pools.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2739 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/cache/ring.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.865109 TDhelper-2.5.5/TDhelper/cache/webCache/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/cache/webCache/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      861 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/cache/webCache/interface.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2963 2023-04-26 14:20:15.000000 TDhelper-2.5.5/TDhelper/cache/webCache/mongo.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/cache/webCache/redis.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1228 2023-05-16 14:29:26.000000 TDhelper-2.5.5/TDhelper/cache/webCache/webCacheFactory.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.865109 TDhelper-2.5.5/TDhelper/db/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.865109 TDhelper-2.5.5/TDhelper/db/Db/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/db/Db/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1235 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/db/Db/base.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      238 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/db/Db/helper.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/db/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.865109 TDhelper-2.5.5/TDhelper/db/mongodb/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/db/mongodb/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1102 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/db/mongodb/base.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3718 2023-04-26 14:07:17.000000 TDhelper-2.5.5/TDhelper/db/mongodb/dbhelper.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1919 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/db/mongodb/objectId.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       44 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/db/mongodb/setting.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.865109 TDhelper-2.5.5/TDhelper/db/mysql/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/db/mysql/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      510 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/db/mysql/base.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/db/mysql/model.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1151 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/db/mysql/mysql_x.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      126 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/db/mysql/setting.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.865109 TDhelper-2.5.5/TDhelper/document/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       24 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/document/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.865109 TDhelper-2.5.5/TDhelper/document/excel/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.865109 TDhelper-2.5.5/TDhelper/document/excel/FieldType/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      104 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/document/excel/FieldType/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       36 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/document/excel/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.865109 TDhelper-2.5.5/TDhelper/document/excel/meta/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       21 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/document/excel/meta/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3854 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/document/excel/meta/modelMeta.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      818 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/document/excel/model.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      622 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/document/file.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.875109 TDhelper-2.5.5/TDhelper/document/ini/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/document/ini/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      123 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/document/ini/fields.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1718 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/document/ini/meta.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      440 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/document/ini/model.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      314 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/document/ini/test.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.885109 TDhelper-2.5.5/TDhelper/generic/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2220 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/generic/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.885109 TDhelper-2.5.5/TDhelper/generic/a/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/generic/a/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       48 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/generic/a/b.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1402 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/generic/classDocCfg.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.885109 TDhelper-2.5.5/TDhelper/generic/crypto/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1413 2023-05-16 14:56:25.000000 TDhelper-2.5.5/TDhelper/generic/crypto/MD5.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/generic/crypto/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4668 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/generic/dictHelper.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.885109 TDhelper-2.5.5/TDhelper/generic/dynamic/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/generic/dynamic/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.885109 TDhelper-2.5.5/TDhelper/generic/dynamic/base/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2782 2023-06-20 10:12:04.000000 TDhelper-2.5.5/TDhelper/generic/dynamic/base/Meta.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/generic/dynamic/base/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2825 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/generic/dynamic/test.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1417 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/generic/findAttribute.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      144 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/generic/randGetValue.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1146 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/generic/recursion.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5628 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/generic/requier.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3721 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/generic/standard_result.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4808 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/generic/threadPools.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3886 2023-05-16 14:56:32.000000 TDhelper-2.5.5/TDhelper/generic/transformationType.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.885109 TDhelper-2.5.5/TDhelper/network/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/network/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.885109 TDhelper-2.5.5/TDhelper/network/http/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7978 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/network/http/REST_HTTP.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    61039 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/network/http/RPC.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    34603 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/network/http/RPC1.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/network/http/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4663 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/network/http/http_helper.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3588 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/network/http/http_postdataformat.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    26267 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/network/http/m3u8.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    26805 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/network/http/m3u8_backup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.885109 TDhelper-2.5.5/TDhelper/network/http/status/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      165 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/network/http/status/M3U8_STATUS.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/network/http/status/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.885109 TDhelper-2.5.5/TDhelper/network/rpc/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.885109 TDhelper-2.5.5/TDhelper/network/rpc/Client/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/network/rpc/Client/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4913 2023-06-20 10:14:15.000000 TDhelper-2.5.5/TDhelper/network/rpc/Client/rpc.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12549 2023-06-19 15:23:41.000000 TDhelper-2.5.5/TDhelper/network/rpc/Client/service.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.885109 TDhelper-2.5.5/TDhelper/network/rpc/Core/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2141 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/network/rpc/Core/Meta.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/network/rpc/Core/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    16328 2023-06-20 11:26:44.000000 TDhelper-2.5.5/TDhelper/network/rpc/Core/struct.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.885109 TDhelper-2.5.5/TDhelper/network/rpc/Generic/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7381 2023-05-14 10:09:53.000000 TDhelper-2.5.5/TDhelper/network/rpc/Generic/Host.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/network/rpc/Generic/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.885109 TDhelper-2.5.5/TDhelper/network/rpc/Server/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/network/rpc/Server/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7837 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/network/rpc/Server/obsolete_Service.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4207 2023-05-14 12:54:46.000000 TDhelper-2.5.5/TDhelper/network/rpc/Server/server.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.885109 TDhelper-2.5.5/TDhelper/network/rpc/Struct/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2202 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/network/rpc/Struct/Result.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/network/rpc/Struct/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/network/rpc/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.885109 TDhelper-2.5.5/TDhelper/network/socket/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2001 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/network/socket/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.885109 TDhelper-2.5.5/TDhelper/network/socket/cache/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/network/socket/cache/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      518 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/network/socket/cache/queue.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2371 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/network/socket/client.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.885109 TDhelper-2.5.5/TDhelper/network/socket/model/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      757 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/network/socket/model/SOCKET_MODELS.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/network/socket/model/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.885109 TDhelper-2.5.5/TDhelper/network/socket/protocol/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/network/socket/protocol/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4531 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/network/socket/protocol/base.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4163 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/network/socket/server.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.885109 TDhelper-2.5.5/TDhelper/network/websocket/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/network/websocket/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3485 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/network/websocket/protocol.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1433 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/network/websocket/server.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1901 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/reflect.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.885109 TDhelper-2.5.5/TDhelper/robot/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/robot/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.895109 TDhelper-2.5.5/TDhelper/robot/control/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1149 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/robot/control/D_33890.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/robot/control/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1296 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/robot/control/device.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.895109 TDhelper-2.5.5/TDhelper/robot/people/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1117 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/robot/people/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5622 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/robot/people/leg.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.895109 TDhelper-2.5.5/TDhelper/robot/people/scripts/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/robot/people/scripts/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3111 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/robot/people/scripts/runScript.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1142 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/robot/people/scripts/script.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/robot/people/upperLimb.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/robot/people/vertebra.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.895109 TDhelper-2.5.5/TDhelper/robot/struct/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/robot/struct/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      621 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/robot/struct/ankle.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2131 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/robot/struct/base.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      613 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/robot/struct/hip.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      618 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/robot/struct/knee.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      697 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/robot/struct/toe.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.895109 TDhelper-2.5.5/TDhelper/shellScripts/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      335 2023-04-06 02:34:35.000000 TDhelper-2.5.5/TDhelper/shellScripts/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3190 2023-05-07 06:20:59.000000 TDhelper-2.5.5/TDhelper/shellScripts/saasHelper.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.895109 TDhelper-2.5.5/TDhelper/simulate/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/simulate/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2713 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/simulate/json.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.895109 TDhelper-2.5.5/TDhelper/structs/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/structs/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4359 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/structs/dir.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.895109 TDhelper-2.5.5/TDhelper/web/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/web/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     8255 2023-04-03 05:53:54.000000 TDhelper-2.5.5/TDhelper/web/permission.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     6908 2023-06-18 14:41:48.000000 TDhelper-2.5.5/TDhelper/web/permissionHelper.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.895109 TDhelper-2.5.5/TDhelper/web/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-18 14:42:30.000000 TDhelper-2.5.5/TDhelper/web/utils/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-20 13:48:28.845109 TDhelper-2.5.5/TDhelper.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2889 2023-06-20 13:48:28.000000 TDhelper-2.5.5/TDhelper.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5563 2023-06-20 13:48:28.000000 TDhelper-2.5.5/TDhelper.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-20 13:48:28.000000 TDhelper-2.5.5/TDhelper.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       62 2023-06-20 13:48:28.000000 TDhelper-2.5.5/TDhelper.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      754 2023-06-20 13:48:28.000000 TDhelper-2.5.5/TDhelper.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-06-20 13:48:28.000000 TDhelper-2.5.5/TDhelper.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-20 13:48:28.895109 TDhelper-2.5.5/setup.cfg
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1789 2023-06-20 13:47:57.000000 TDhelper-2.5.5/setup.py
```

### Comparing `TDhelper-2.5.4/LICENSE` & `TDhelper-2.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/PKG-INFO` & `TDhelper-2.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TDhelper
-Version: 2.5.4
+Version: 2.5.5
 Summary: reconsitution web.permissionHelper cls.
 Home-page: https://gitee.com/TonyDon/pyLib
 Author: TangJing
 Author-email: yeihizhi@163.com
 License: Apache 2.0
 Keywords: pip,TDhelper,featureextraction
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: TDhelper Version: 2.5.4 Summary: reconsitution
+Metadata-Version: 2.1 Name: TDhelper Version: 2.5.5 Summary: reconsitution
 web.permissionHelper cls. Home-page: https://gitee.com/TonyDon/pyLib Author:
 TangJing Author-email: yeihizhi@163.com License: Apache 2.0 Keywords:
 pip,TDhelper,featureextraction Description-Content-Type: text/markdown License-
 File: LICENSE # TDhelper LIb helper class lib. # ***Cache*** ## 1. pools ## 2.
 ring cache # ***db*** ## 1. sqllite ## 2. mongodb ## 3. mysql #
 ***Decorators*** ## 1. log # ***document*** ## 1. file ## 2. excel #
 ***Event*** ## 1. Event ## 2. classEvent ## 3. webEvent # ***generic*** #
```

### Comparing `TDhelper-2.5.4/README.md` & `TDhelper-2.5.5/README.md`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/Decorators/log.py` & `TDhelper-2.5.5/TDhelper/Decorators/log.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/Decorators/performance.py` & `TDhelper-2.5.5/TDhelper/Decorators/performance.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/Event/Event.py` & `TDhelper-2.5.5/TDhelper/Event/Event.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/Event/classEvent/event.py` & `TDhelper-2.5.5/TDhelper/Event/classEvent/event.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/Event/classEvent/meta.py` & `TDhelper-2.5.5/TDhelper/Event/classEvent/meta.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/Event/webEvent/Events.py` & `TDhelper-2.5.5/TDhelper/Event/webEvent/Events.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/MagicCls/MagicMeta.py` & `TDhelper-2.5.5/TDhelper/MagicCls/MagicMeta.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/MagicCls/model.py` & `TDhelper-2.5.5/TDhelper/MagicCls/model.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/MagicCls/test.py` & `TDhelper-2.5.5/TDhelper/MagicCls/test.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/Msg/AppPush.py` & `TDhelper-2.5.5/TDhelper/Msg/AppPush.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/Msg/Config.py` & `TDhelper-2.5.5/TDhelper/Msg/Config.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/Msg/Email.py` & `TDhelper-2.5.5/TDhelper/Msg/Email.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/Msg/InterfaceMsg.py` & `TDhelper-2.5.5/TDhelper/Msg/InterfaceMsg.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/Msg/SMS.py` & `TDhelper-2.5.5/TDhelper/Msg/SMS.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/Scheduler/base.py` & `TDhelper-2.5.5/TDhelper/Scheduler/base.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/Scheduler/example_scheduler.py` & `TDhelper-2.5.5/TDhelper/Scheduler/example_scheduler.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/Scheduler/interface.py` & `TDhelper-2.5.5/TDhelper/Scheduler/interface.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/Scheduler/log_config.py` & `TDhelper-2.5.5/TDhelper/Scheduler/log_config.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/Scheduler/service.py` & `TDhelper-2.5.5/TDhelper/Scheduler/service.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/Spider/contentExtraction.py` & `TDhelper-2.5.5/TDhelper/Spider/contentExtraction.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/Spider/models/BadRequestModel.py` & `TDhelper-2.5.5/TDhelper/Spider/models/BadRequestModel.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/Spider/models/Cache_L1.py` & `TDhelper-2.5.5/TDhelper/Spider/models/Cache_L1.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/Spider/models/Cache_L2.py` & `TDhelper-2.5.5/TDhelper/Spider/models/Cache_L2.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/Spider/models/Cache_L2_Model.py` & `TDhelper-2.5.5/TDhelper/Spider/models/Cache_L2_Model.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/Spider/models/fingerprint.py` & `TDhelper-2.5.5/TDhelper/Spider/models/fingerprint.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/Spider/models/status.py` & `TDhelper-2.5.5/TDhelper/Spider/models/status.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/Spider/regex.py` & `TDhelper-2.5.5/TDhelper/Spider/regex.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/Spider/spiderPools.py` & `TDhelper-2.5.5/TDhelper/Spider/spiderPools.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/apiCore.py` & `TDhelper-2.5.5/TDhelper/apiCore.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/bin/globalvar.py` & `TDhelper-2.5.5/TDhelper/bin/globalvar.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/cache/memcache.py` & `TDhelper-2.5.5/TDhelper/cache/memcache.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/cache/pools.py` & `TDhelper-2.5.5/TDhelper/cache/pools.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/cache/ring.py` & `TDhelper-2.5.5/TDhelper/cache/ring.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/cache/webCache/interface.py` & `TDhelper-2.5.5/TDhelper/cache/webCache/interface.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/cache/webCache/mongo.py` & `TDhelper-2.5.5/TDhelper/cache/webCache/mongo.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/cache/webCache/webCacheFactory.py` & `TDhelper-2.5.5/TDhelper/cache/webCache/webCacheFactory.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/db/Db/base.py` & `TDhelper-2.5.5/TDhelper/db/Db/base.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/db/mongodb/base.py` & `TDhelper-2.5.5/TDhelper/db/mongodb/base.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/db/mongodb/dbhelper.py` & `TDhelper-2.5.5/TDhelper/db/mongodb/dbhelper.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/db/mongodb/objectId.py` & `TDhelper-2.5.5/TDhelper/db/mongodb/objectId.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/db/mysql/mysql_x.py` & `TDhelper-2.5.5/TDhelper/db/mysql/mysql_x.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/document/excel/meta/modelMeta.py` & `TDhelper-2.5.5/TDhelper/document/excel/meta/modelMeta.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/document/excel/model.py` & `TDhelper-2.5.5/TDhelper/document/excel/model.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/document/file.py` & `TDhelper-2.5.5/TDhelper/document/file.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/document/ini/meta.py` & `TDhelper-2.5.5/TDhelper/document/ini/meta.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/generic/__init__.py` & `TDhelper-2.5.5/TDhelper/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/generic/classDocCfg.py` & `TDhelper-2.5.5/TDhelper/generic/classDocCfg.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/generic/crypto/MD5.py` & `TDhelper-2.5.5/TDhelper/generic/crypto/MD5.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/generic/dictHelper.py` & `TDhelper-2.5.5/TDhelper/generic/dictHelper.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/generic/dynamic/base/Meta.py` & `TDhelper-2.5.5/TDhelper/generic/dynamic/base/Meta.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
         def __init__(self,cls_name,fn_name,fn):
             self.__cls_name__=cls_name
             self.__name__=fn_name
             self.__fn__= fn
         
         def __call__(self,*args, **kwargs):
             return self.__fn__(self.__cls_name__,self.__name__,*args,**kwargs)
-
+    
     def __new__(cls, name, bases, dct):
         attrs = {
             "__name__":name,
             "__context__":{} if '__context__' not in dct else dct['__context__'],
             "__dynamic_methods__":[],
             "__set_hook__":cls.__set_hook_method__,
             "__hook_method__":dct["__hook_method__"] if '__hook_method__' in dct else None,
@@ -48,15 +48,17 @@
     def __set_hook_method__(self,fn):
         if fn:
             self.__hook_method__= fn
             for k in self.__dynamic_methods__:
                 self.__dict__[k]=self.FunctionOverride(self.__name__,k,fn)
 
 class dynamic_creator(metaclass=Meta):
-   
+    __self_handle__= lambda o: o,
+    __get_method_handle__= lambda o,k: getattr(o,k) if hasattr(o,k) else None
+    __has_method__=lambda o,k: True if o.__dynamic_methods__.__contains__(k) else False
     def __init__(self,fn=None):
         self.__set_hook__(fn)
         super(dynamic_creator,self).__init__()
         
     class Meta:
         __name__=None
         __construct__=None
```

### Comparing `TDhelper-2.5.4/TDhelper/generic/dynamic/test.py` & `TDhelper-2.5.5/TDhelper/generic/dynamic/test.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/generic/findAttribute.py` & `TDhelper-2.5.5/TDhelper/generic/findAttribute.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/generic/recursion.py` & `TDhelper-2.5.5/TDhelper/generic/recursion.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/generic/requier.py` & `TDhelper-2.5.5/TDhelper/generic/requier.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/generic/standard_result.py` & `TDhelper-2.5.5/TDhelper/generic/standard_result.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/generic/threadPools.py` & `TDhelper-2.5.5/TDhelper/generic/threadPools.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/generic/transformationType.py` & `TDhelper-2.5.5/TDhelper/generic/transformationType.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/network/http/REST_HTTP.py` & `TDhelper-2.5.5/TDhelper/network/http/REST_HTTP.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/network/http/RPC.py` & `TDhelper-2.5.5/TDhelper/network/http/RPC.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/network/http/RPC1.py` & `TDhelper-2.5.5/TDhelper/network/http/RPC1.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/network/http/http_helper.py` & `TDhelper-2.5.5/TDhelper/network/http/http_helper.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/network/http/http_postdataformat.py` & `TDhelper-2.5.5/TDhelper/network/http/http_postdataformat.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/network/http/m3u8.py` & `TDhelper-2.5.5/TDhelper/network/http/m3u8.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/network/http/m3u8_backup.py` & `TDhelper-2.5.5/TDhelper/network/http/m3u8_backup.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/network/rpc/Client/rpc.py` & `TDhelper-2.5.5/TDhelper/network/rpc/Client/rpc.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 performance.on_off(True)
 
 
 class client():
     __TOKEN_KEY__ = "api-token"
     __TOKEN__ = ""
     __LOGGER__ = logging
-
+    __service_exists__= lambda o,k: True if k in o.__dict__ else False
+    __get_service__= lambda o,k: getattr(o,k) if o.__service_exists__(k) else None
+    
     @performance.performance_testing
     def __init__(self, uri, path: list = [], token: str = "", sniffer: list = ["sniffer"], services: list = [], token_key=None, logger: dict = None, try_count=5, try_sleep=3):
         if logger:
             self.__LOGGER__.basicConfig(level=logging.INFO)
             self.__LOGGER__.config.dictConfig(logger)
         self.__TOKEN_KEY__ = token_key if token_key else self.__TOKEN_KEY__
         self.__TOKEN__ = token
@@ -48,17 +50,15 @@
                     self.__dict__["__srv_struct__"][k] = type(
                         k, (RPC_SERVICE,), {}).create_by_cnf(v, self.__TOKEN_KEY__)
                     methods = [kv for kv in v['methods'].keys()]
                     self.__dict__[k] = type(k, (dynamic_creator,), {
                                             "__dynamic_methods__": methods, "__hook_method__": self.__call__})()
             else:
                 self.__LOGGER__.error("not found rpc method.%s"%self.__context__["msg"])
-                s="not found rpc method.%s"%self.__context__["msg"]
-                print(s)
-                raise Exception(s)
+                raise Exception("not found rpc method.%s"%self.__context__["msg"])
         else:
             raise Exception("not found rpc instance config.")
         super(client, self).__init__()
 
     @performance.performance_testing
     def __call__(self, service_name, fun_name, *args, **kwargs):
         remote_func_name = ("".join([service_name, '.', fun_name]))
```

### Comparing `TDhelper-2.5.4/TDhelper/network/rpc/Client/service.py` & `TDhelper-2.5.5/TDhelper/network/rpc/Client/service.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/network/rpc/Core/Meta.py` & `TDhelper-2.5.5/TDhelper/network/rpc/Core/Meta.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/network/rpc/Core/struct.py` & `TDhelper-2.5.5/TDhelper/network/rpc/Core/struct.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,15 +208,16 @@
     host = None
     name: str = None
     description: str = None
     key: str = None
     secret: str = None
     protocol: str = "http://"
     methods = {}
-
+    __method_exists__= lambda o,k: True if k in o.__dict__ else False
+    
     def __init__(self, name=None, description=None, key=None, secret=None, protocol=None, host_cnf=None, methods_cnf=None, token_key="api-token"):
         self.__TOKEN_KEY__ = token_key
         self.name = name
         self.description = description
         self.key = key
         self.secret = secret
         self.protocol = protocol
@@ -386,15 +387,15 @@
                         else:
                             if item.default:
                                 m_headers[item.upper.replace("HTTP_HEADER_", "").replace(
                                     "http_header_", "").replace("_", "-")] = item.default
                             else:
                                 raise Exception(
                                     "not found http header key(%s)" % item.key)
-                elif item.key.lower().startswith("http_data"):
+                elif item.key.lower().startswith("http_data_"):
                     if "data" not in kwargs:
                         kwargs["data"] = {}
                     if (item.key.replace("http_data_", "") not in kwargs["data"]):
                         if item.key in kwargs:
                             kwargs["data"][item.key.replace(
                                 "http_data_",
                                 "")] = kwargs[item.key]
```

### Comparing `TDhelper-2.5.4/TDhelper/network/rpc/Generic/Host.py` & `TDhelper-2.5.5/TDhelper/network/rpc/Generic/Host.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/network/rpc/Server/obsolete_Service.py` & `TDhelper-2.5.5/TDhelper/network/rpc/Server/obsolete_Service.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/network/rpc/Server/server.py` & `TDhelper-2.5.5/TDhelper/network/rpc/Server/server.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/network/rpc/Struct/Result.py` & `TDhelper-2.5.5/TDhelper/network/rpc/Struct/Result.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/network/socket/__init__.py` & `TDhelper-2.5.5/TDhelper/network/socket/__init__.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/network/socket/cache/queue.py` & `TDhelper-2.5.5/TDhelper/network/socket/cache/queue.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/network/socket/client.py` & `TDhelper-2.5.5/TDhelper/network/socket/client.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/network/socket/model/SOCKET_MODELS.py` & `TDhelper-2.5.5/TDhelper/network/socket/model/SOCKET_MODELS.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/network/socket/protocol/base.py` & `TDhelper-2.5.5/TDhelper/network/socket/protocol/base.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/network/socket/server.py` & `TDhelper-2.5.5/TDhelper/network/socket/server.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/network/websocket/protocol.py` & `TDhelper-2.5.5/TDhelper/network/websocket/protocol.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/network/websocket/server.py` & `TDhelper-2.5.5/TDhelper/network/websocket/server.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/reflect.py` & `TDhelper-2.5.5/TDhelper/reflect.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/robot/control/D_33890.py` & `TDhelper-2.5.5/TDhelper/robot/control/D_33890.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/robot/control/device.py` & `TDhelper-2.5.5/TDhelper/robot/control/device.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/robot/people/__init__.py` & `TDhelper-2.5.5/TDhelper/robot/people/__init__.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/robot/people/leg.py` & `TDhelper-2.5.5/TDhelper/robot/people/leg.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/robot/people/scripts/runScript.py` & `TDhelper-2.5.5/TDhelper/robot/people/scripts/runScript.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/robot/people/scripts/script.py` & `TDhelper-2.5.5/TDhelper/robot/people/scripts/script.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/robot/struct/ankle.py` & `TDhelper-2.5.5/TDhelper/robot/struct/ankle.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/robot/struct/base.py` & `TDhelper-2.5.5/TDhelper/robot/struct/base.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/robot/struct/hip.py` & `TDhelper-2.5.5/TDhelper/robot/struct/hip.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/robot/struct/knee.py` & `TDhelper-2.5.5/TDhelper/robot/struct/knee.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/robot/struct/toe.py` & `TDhelper-2.5.5/TDhelper/robot/struct/toe.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/shellScripts/saasHelper.py` & `TDhelper-2.5.5/TDhelper/shellScripts/saasHelper.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/simulate/json.py` & `TDhelper-2.5.5/TDhelper/simulate/json.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/structs/dir.py` & `TDhelper-2.5.5/TDhelper/structs/dir.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/web/permission.py` & `TDhelper-2.5.5/TDhelper/web/permission.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper/web/permissionHelper.py` & `TDhelper-2.5.5/TDhelper/web/permissionHelper.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper.egg-info/PKG-INFO` & `TDhelper-2.5.5/TDhelper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TDhelper
-Version: 2.5.4
+Version: 2.5.5
 Summary: reconsitution web.permissionHelper cls.
 Home-page: https://gitee.com/TonyDon/pyLib
 Author: TangJing
 Author-email: yeihizhi@163.com
 License: Apache 2.0
 Keywords: pip,TDhelper,featureextraction
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: TDhelper Version: 2.5.4 Summary: reconsitution
+Metadata-Version: 2.1 Name: TDhelper Version: 2.5.5 Summary: reconsitution
 web.permissionHelper cls. Home-page: https://gitee.com/TonyDon/pyLib Author:
 TangJing Author-email: yeihizhi@163.com License: Apache 2.0 Keywords:
 pip,TDhelper,featureextraction Description-Content-Type: text/markdown License-
 File: LICENSE # TDhelper LIb helper class lib. # ***Cache*** ## 1. pools ## 2.
 ring cache # ***db*** ## 1. sqllite ## 2. mongodb ## 3. mysql #
 ***Decorators*** ## 1. log # ***document*** ## 1. file ## 2. excel #
 ***Event*** ## 1. Event ## 2. classEvent ## 3. webEvent # ***generic*** #
```

### Comparing `TDhelper-2.5.4/TDhelper.egg-info/SOURCES.txt` & `TDhelper-2.5.5/TDhelper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/TDhelper.egg-info/requires.txt` & `TDhelper-2.5.5/TDhelper.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `TDhelper-2.5.4/setup.py` & `TDhelper-2.5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 setuptools.setup(
     name="TDhelper",
-    version="2.5.4",
+    version="2.5.5",
     keywords=("pip", "TDhelper", "featureextraction"),
     description="reconsitution web.permissionHelper cls.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="Apache 2.0",
     url="https://gitee.com/TonyDon/pyLib",
     author="TangJing",
```

