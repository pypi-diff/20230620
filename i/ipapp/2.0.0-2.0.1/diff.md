# Comparing `tmp/ipapp-2.0.0.tar.gz` & `tmp/ipapp-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipapp-2.0.0.tar", max compression
+gzip compressed data, was "ipapp-2.0.1.tar", max compression
```

## Comparing `ipapp-2.0.0.tar` & `ipapp-2.0.1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0     1085 2023-06-13 11:00:20.186944 ipapp-2.0.0/LICENSE
--rw-r--r--   0        0        0     1050 2023-06-13 11:00:20.186944 ipapp-2.0.0/README.md
--rw-r--r--   0        0        0      679 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/__init__.py
--rw-r--r--   0        0        0     6049 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/app.py
--rw-r--r--   0        0        0        0 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/asgi/__init__.py
--rw-r--r--   0        0        0     8079 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/asgi/uvicorn.py
--rw-r--r--   0        0        0     3668 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/autoreload.py
--rw-r--r--   0        0        0     4407 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/cli.py
--rw-r--r--   0        0        0      690 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/component.py
--rw-r--r--   0        0        0     9744 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/config.py
--rw-r--r--   0        0        0     6930 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/ctx.py
--rw-r--r--   0        0        0        0 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/db/__init__.py
--rw-r--r--   0        0        0    22205 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/db/oracle.py
--rw-r--r--   0        0        0    39149 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/db/pg.py
--rw-r--r--   0        0        0      158 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/error.py
--rw-r--r--   0        0        0      268 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/http/__init__.py
--rw-r--r--   0        0        0     5748 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/http/_base.py
--rw-r--r--   0        0        0     5829 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/http/client.py
--rw-r--r--   0        0        0    16861 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/http/server.py
--rw-r--r--   0        0        0     3259 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/logger/__init__.py
--rw-r--r--   0        0        0      471 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/logger/adapters/__init__.py
--rw-r--r--   0        0        0      810 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/logger/adapters/_abc.py
--rw-r--r--   0        0        0     5180 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/logger/adapters/prometheus.py
--rw-r--r--   0        0        0    18741 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/logger/adapters/requests.py
--rw-r--r--   0        0        0     1351 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/logger/adapters/sentry.py
--rw-r--r--   0        0        0     3065 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/logger/adapters/zipkin.py
--rw-r--r--   0        0        0     3163 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/logger/logger.py
--rw-r--r--   0        0        0    14493 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/logger/span.py
--rw-r--r--   0        0        0     6111 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/misc.py
--rw-r--r--   0        0        0        0 2023-06-13 11:00:20.190944 ipapp-2.0.0/ipapp/mq/__init__.py
--rw-r--r--   0        0        0    32905 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/mq/pika.py
--rw-r--r--   0        0        0        0 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/openapi/__init__.py
--rw-r--r--   0        0        0     8694 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/openapi/misc.py
--rw-r--r--   0        0        0    10428 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/openapi/models.py
--rw-r--r--   0        0        0     2879 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/openapi/templates.py
--rw-r--r--   0        0        0      210 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/__init__.py
--rw-r--r--   0        0        0       66 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/const.py
--rw-r--r--   0        0        0      124 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/error.py
--rw-r--r--   0        0        0      294 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/http/__init__.py
--rw-r--r--   0        0        0     2599 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/http/client.py
--rw-r--r--   0        0        0    15026 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/http/server.py
--rw-r--r--   0        0        0      173 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/jsonrpc/__init__.py
--rw-r--r--   0        0        0      880 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/jsonrpc/error.py
--rw-r--r--   0        0        0      424 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/jsonrpc/http/__init__.py
--rw-r--r--   0        0        0     2352 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/jsonrpc/http/client.py
--rw-r--r--   0        0        0     5450 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/jsonrpc/http/server.py
--rw-r--r--   0        0        0    23360 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/jsonrpc/main.py
--rw-r--r--   0        0        0        0 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/jsonrpc/mq/__init__.py
--rw-r--r--   0        0        0     8451 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/jsonrpc/mq/pika.py
--rw-r--r--   0        0        0       51 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/jsonrpc/openrpc/__init__.py
--rw-r--r--   0        0        0    11725 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/jsonrpc/openrpc/discover.py
--rw-r--r--   0        0        0     5853 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/jsonrpc/openrpc/models.py
--rw-r--r--   0        0        0    17002 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/main.py
--rw-r--r--   0        0        0        0 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/mq/__init__.py
--rw-r--r--   0        0        0    10032 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/mq/pika.py
--rw-r--r--   0        0        0      495 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/restrpc/__init__.py
--rw-r--r--   0        0        0     2488 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/restrpc/error.py
--rw-r--r--   0        0        0      424 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/restrpc/http/__init__.py
--rw-r--r--   0        0        0     2235 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/restrpc/http/client.py
--rw-r--r--   0        0        0    19028 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/restrpc/http/server.py
--rw-r--r--   0        0        0    18406 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/restrpc/main.py
--rw-r--r--   0        0        0        0 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/restrpc/openapi/__init__.py
--rw-r--r--   0        0        0     9426 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/rpc/restrpc/openapi/misc.py
--rw-r--r--   0        0        0      136 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/s3/__init__.py
--rw-r--r--   0        0        0    20855 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/s3/boto.py
--rw-r--r--   0        0        0       90 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/s3/exceptions.py
--rw-r--r--   0        0        0     5293 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/s3/models.py
--rw-r--r--   0        0        0        0 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/sftp/__init__.py
--rw-r--r--   0        0        0    17841 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/sftp/client.py
--rw-r--r--   0        0        0       56 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/sphinx/__init__.py
--rw-r--r--   0        0        0     4115 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/sphinx/config.py
--rw-r--r--   0        0        0        0 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/task/__init__.py
--rw-r--r--   0        0        0    39913 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/task/db.py
--rw-r--r--   0        0        0        0 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/utils/__init__.py
--rw-r--r--   0        0        0       69 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/utils/lock/__init__.py
--rw-r--r--   0        0        0     1223 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/utils/lock/local.py
--rw-r--r--   0        0        0     3643 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/utils/lock/main.py
--rw-r--r--   0        0        0     4350 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/utils/lock/pg.py
--rw-r--r--   0        0        0     5804 2023-06-13 11:00:20.194944 ipapp-2.0.0/ipapp/utils/lock/redis.py
--rw-r--r--   0        0        0     3893 2023-06-13 11:00:58.663153 ipapp-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     4615 1970-01-01 00:00:00.000000 ipapp-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-06-20 07:35:59.466908 ipapp-2.0.1/LICENSE
+-rw-r--r--   0        0        0     1050 2023-06-20 07:35:59.466908 ipapp-2.0.1/README.md
+-rw-r--r--   0        0        0      679 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/__init__.py
+-rw-r--r--   0        0        0     6049 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/app.py
+-rw-r--r--   0        0        0        0 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/asgi/__init__.py
+-rw-r--r--   0        0        0     8079 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/asgi/uvicorn.py
+-rw-r--r--   0        0        0     3668 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/autoreload.py
+-rw-r--r--   0        0        0     4407 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/cli.py
+-rw-r--r--   0        0        0      690 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/component.py
+-rw-r--r--   0        0        0     9744 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/config.py
+-rw-r--r--   0        0        0     6930 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/ctx.py
+-rw-r--r--   0        0        0        0 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/db/__init__.py
+-rw-r--r--   0        0        0    22205 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/db/oracle.py
+-rw-r--r--   0        0        0    39151 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/db/pg.py
+-rw-r--r--   0        0        0      158 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/error.py
+-rw-r--r--   0        0        0      268 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/http/__init__.py
+-rw-r--r--   0        0        0     5748 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/http/_base.py
+-rw-r--r--   0        0        0     5829 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/http/client.py
+-rw-r--r--   0        0        0    16861 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/http/server.py
+-rw-r--r--   0        0        0     3259 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/logger/__init__.py
+-rw-r--r--   0        0        0      471 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/logger/adapters/__init__.py
+-rw-r--r--   0        0        0      810 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/logger/adapters/_abc.py
+-rw-r--r--   0        0        0     6204 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/logger/adapters/prometheus.py
+-rw-r--r--   0        0        0    18741 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/logger/adapters/requests.py
+-rw-r--r--   0        0        0     1351 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/logger/adapters/sentry.py
+-rw-r--r--   0        0        0     3065 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/logger/adapters/zipkin.py
+-rw-r--r--   0        0        0     3163 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/logger/logger.py
+-rw-r--r--   0        0        0    14493 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/logger/span.py
+-rw-r--r--   0        0        0     6111 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/misc.py
+-rw-r--r--   0        0        0        0 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/mq/__init__.py
+-rw-r--r--   0        0        0    32905 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/mq/pika.py
+-rw-r--r--   0        0        0        0 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/openapi/__init__.py
+-rw-r--r--   0        0        0     8694 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/openapi/misc.py
+-rw-r--r--   0        0        0    10428 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/openapi/models.py
+-rw-r--r--   0        0        0     2879 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/openapi/templates.py
+-rw-r--r--   0        0        0      210 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/rpc/__init__.py
+-rw-r--r--   0        0        0       66 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/rpc/const.py
+-rw-r--r--   0        0        0      124 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/rpc/error.py
+-rw-r--r--   0        0        0      294 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/rpc/http/__init__.py
+-rw-r--r--   0        0        0     2599 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/rpc/http/client.py
+-rw-r--r--   0        0        0    15026 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/rpc/http/server.py
+-rw-r--r--   0        0        0      173 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/rpc/jsonrpc/__init__.py
+-rw-r--r--   0        0        0      880 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/rpc/jsonrpc/error.py
+-rw-r--r--   0        0        0      424 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/rpc/jsonrpc/http/__init__.py
+-rw-r--r--   0        0        0     2352 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/rpc/jsonrpc/http/client.py
+-rw-r--r--   0        0        0     5450 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/rpc/jsonrpc/http/server.py
+-rw-r--r--   0        0        0    23360 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/rpc/jsonrpc/main.py
+-rw-r--r--   0        0        0        0 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/rpc/jsonrpc/mq/__init__.py
+-rw-r--r--   0        0        0     8451 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/rpc/jsonrpc/mq/pika.py
+-rw-r--r--   0        0        0       51 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/rpc/jsonrpc/openrpc/__init__.py
+-rw-r--r--   0        0        0    11725 2023-06-20 07:35:59.470908 ipapp-2.0.1/ipapp/rpc/jsonrpc/openrpc/discover.py
+-rw-r--r--   0        0        0     5853 2023-06-20 07:35:59.474908 ipapp-2.0.1/ipapp/rpc/jsonrpc/openrpc/models.py
+-rw-r--r--   0        0        0    17002 2023-06-20 07:35:59.474908 ipapp-2.0.1/ipapp/rpc/main.py
+-rw-r--r--   0        0        0        0 2023-06-20 07:35:59.474908 ipapp-2.0.1/ipapp/rpc/mq/__init__.py
+-rw-r--r--   0        0        0    10032 2023-06-20 07:35:59.474908 ipapp-2.0.1/ipapp/rpc/mq/pika.py
+-rw-r--r--   0        0        0      495 2023-06-20 07:35:59.474908 ipapp-2.0.1/ipapp/rpc/restrpc/__init__.py
+-rw-r--r--   0        0        0     2488 2023-06-20 07:35:59.474908 ipapp-2.0.1/ipapp/rpc/restrpc/error.py
+-rw-r--r--   0        0        0      424 2023-06-20 07:35:59.474908 ipapp-2.0.1/ipapp/rpc/restrpc/http/__init__.py
+-rw-r--r--   0        0        0     2235 2023-06-20 07:35:59.474908 ipapp-2.0.1/ipapp/rpc/restrpc/http/client.py
+-rw-r--r--   0        0        0    19028 2023-06-20 07:35:59.474908 ipapp-2.0.1/ipapp/rpc/restrpc/http/server.py
+-rw-r--r--   0        0        0    18406 2023-06-20 07:35:59.474908 ipapp-2.0.1/ipapp/rpc/restrpc/main.py
+-rw-r--r--   0        0        0        0 2023-06-20 07:35:59.474908 ipapp-2.0.1/ipapp/rpc/restrpc/openapi/__init__.py
+-rw-r--r--   0        0        0     9426 2023-06-20 07:35:59.474908 ipapp-2.0.1/ipapp/rpc/restrpc/openapi/misc.py
+-rw-r--r--   0        0        0      136 2023-06-20 07:35:59.474908 ipapp-2.0.1/ipapp/s3/__init__.py
+-rw-r--r--   0        0        0    20855 2023-06-20 07:35:59.474908 ipapp-2.0.1/ipapp/s3/boto.py
+-rw-r--r--   0        0        0       90 2023-06-20 07:35:59.474908 ipapp-2.0.1/ipapp/s3/exceptions.py
+-rw-r--r--   0        0        0     5293 2023-06-20 07:35:59.474908 ipapp-2.0.1/ipapp/s3/models.py
+-rw-r--r--   0        0        0        0 2023-06-20 07:35:59.474908 ipapp-2.0.1/ipapp/sftp/__init__.py
+-rw-r--r--   0        0        0    17841 2023-06-20 07:35:59.474908 ipapp-2.0.1/ipapp/sftp/client.py
+-rw-r--r--   0        0        0       56 2023-06-20 07:35:59.474908 ipapp-2.0.1/ipapp/sphinx/__init__.py
+-rw-r--r--   0        0        0     4115 2023-06-20 07:35:59.474908 ipapp-2.0.1/ipapp/sphinx/config.py
+-rw-r--r--   0        0        0        0 2023-06-20 07:35:59.474908 ipapp-2.0.1/ipapp/task/__init__.py
+-rw-r--r--   0        0        0    39913 2023-06-20 07:35:59.474908 ipapp-2.0.1/ipapp/task/db.py
+-rw-r--r--   0        0        0        0 2023-06-20 07:35:59.474908 ipapp-2.0.1/ipapp/utils/__init__.py
+-rw-r--r--   0        0        0       69 2023-06-20 07:35:59.474908 ipapp-2.0.1/ipapp/utils/lock/__init__.py
+-rw-r--r--   0        0        0     1223 2023-06-20 07:35:59.474908 ipapp-2.0.1/ipapp/utils/lock/local.py
+-rw-r--r--   0        0        0     3643 2023-06-20 07:35:59.474908 ipapp-2.0.1/ipapp/utils/lock/main.py
+-rw-r--r--   0        0        0     4350 2023-06-20 07:35:59.474908 ipapp-2.0.1/ipapp/utils/lock/pg.py
+-rw-r--r--   0        0        0     5804 2023-06-20 07:35:59.474908 ipapp-2.0.1/ipapp/utils/lock/redis.py
+-rw-r--r--   0        0        0     3893 2023-06-20 07:36:27.531569 ipapp-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4615 1970-01-01 00:00:00.000000 ipapp-2.0.1/PKG-INFO
```

### Comparing `ipapp-2.0.0/LICENSE` & `ipapp-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/README.md` & `ipapp-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/__init__.py` & `ipapp-2.0.1/ipapp/__init__.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/app.py` & `ipapp-2.0.1/ipapp/app.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/asgi/uvicorn.py` & `ipapp-2.0.1/ipapp/asgi/uvicorn.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/autoreload.py` & `ipapp-2.0.1/ipapp/autoreload.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/cli.py` & `ipapp-2.0.1/ipapp/cli.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/component.py` & `ipapp-2.0.1/ipapp/component.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/config.py` & `ipapp-2.0.1/ipapp/config.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/ctx.py` & `ipapp-2.0.1/ipapp/ctx.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/db/oracle.py` & `ipapp-2.0.1/ipapp/db/oracle.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/db/pg.py` & `ipapp-2.0.1/ipapp/db/pg.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,31 +99,31 @@
     NAME_XACT_COMMITED = 'db::xact (commited)'
     NAME_XACT_REVERTED = 'db::xact (reverted)'
     NAME_EXECUTE = 'db::execute'
     NAME_EXECUTEMANY = 'db::executemany'
     NAME_QUERY_ONE = 'db::query_one'
     NAME_QUERY_ALL = 'db::query_all'
     NAME_PREPARE = 'db::prepare'
-    NAME_QUERY_ONE_PREPARED = 'db::execute_query_one'
-    NAME_QUERY_ALL_PREPARED = 'db::execute_query_all'
+    NAME_QUERY_ONE_PREPARED = 'db::query_one_prepared'
+    NAME_QUERY_ALL_PREPARED = 'db::query_all_prepared'
     NAME_CURSOR = 'db::cursor'
-    NAME_CURSOR_PREPARED = 'db::execute_cursor'
+    NAME_CURSOR_PREPARED = 'db::cursor_prepared'
 
     P8S_NAME_ACQUIRE = 'db_connection'
     P8S_NAME_XACT_COMMITED = 'db_xact_commited'
     P8S_NAME_XACT_REVERTED = 'db_xact_reverted'
     P8S_NAME_EXECUTE = 'db_execute'
     P8S_NAME_EXECUTEMANY = 'db_executemany'
-    P8S_NAME_QUERY_ONE = 'db::query_one'
-    P8S_NAME_QUERY_ALL = 'db::query_all'
+    P8S_NAME_QUERY_ONE = 'db_query_one'
+    P8S_NAME_QUERY_ALL = 'db_query_all'
     P8S_NAME_PREPARE = 'db_prepare'
-    P8S_NAME_QUERY_ONE_PREPARED = 'db_execute_query_one'
-    P8S_NAME_QUERY_ALL_PREPARED = 'db_execute_query_all'
-    P8S_NAME_CURSOR = 'db::cursor'
-    P8S_NAME_CURSOR_PREPARED = 'db::execute_cursor'
+    P8S_NAME_QUERY_ONE_PREPARED = 'db_query_one_prepared'
+    P8S_NAME_QUERY_ALL_PREPARED = 'db_query_all_prepared'
+    P8S_NAME_CURSOR = 'db_cursor'
+    P8S_NAME_CURSOR_PREPARED = 'db_cursor_prepared'
 
     TAG_POOL_MAX_SIZE = 'db.pool.size'
     TAG_POOL_FREE_COUNT = 'db.pool.free'
 
     TAG_QUERY_NAME = 'db.query'
 
     ANN_PID = 'pg_pid'
```

### Comparing `ipapp-2.0.0/ipapp/http/_base.py` & `ipapp-2.0.1/ipapp/http/_base.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/http/client.py` & `ipapp-2.0.1/ipapp/http/client.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/http/server.py` & `ipapp-2.0.1/ipapp/http/server.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/logger/__init__.py` & `ipapp-2.0.1/ipapp/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/logger/adapters/_abc.py` & `ipapp-2.0.1/ipapp/logger/adapters/_abc.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/logger/adapters/prometheus.py` & `ipapp-2.0.1/ipapp/logger/adapters/prometheus.py`

 * *Files 21% similar despite different names*

```diff
@@ -49,14 +49,19 @@
         'error': 'error.class',
     },
     'db_execute': {
         'le': DEFAULT_LE,  # le mapping to quantiles
         'error': 'error.class',
         'query': 'db.query',
     },
+    'db_executemany': {
+        'le': DEFAULT_LE,  # le mapping to quantiles
+        'error': 'error.class',
+        'query': 'db.query',
+    },
     'db_callproc': {
         'le': DEFAULT_LE,  # le mapping to quantiles
         'error': 'error.class',
         'query': 'db.proc',
     },
     'db_callfunc': {
         'le': DEFAULT_LE,  # le mapping to quantiles
@@ -74,14 +79,44 @@
         'query': 'db.query',
     },
     'db_fetch': {
         'le': DEFAULT_LE,  # le mapping to quantiles
         'error': 'error.class',
         'query': 'db.query',
     },
+    'db_query_one': {
+        'le': DEFAULT_LE,  # le mapping to quantiles
+        'error': 'error.class',
+        'query': 'db.query',
+    },
+    'db_query_all': {
+        'le': DEFAULT_LE,  # le mapping to quantiles
+        'error': 'error.class',
+        'query': 'db.query',
+    },
+    'db_query_one_prepared': {
+        'le': DEFAULT_LE,  # le mapping to quantiles
+        'error': 'error.class',
+        'query': 'db.query',
+    },
+    'db_query_all_prepared': {
+        'le': DEFAULT_LE,  # le mapping to quantiles
+        'error': 'error.class',
+        'query': 'db.query',
+    },
+    'db_cursor': {
+        'le': DEFAULT_LE,  # le mapping to quantiles
+        'error': 'error.class',
+        'query': 'db.query',
+    },
+    'db_cursor_prepared': {
+        'le': DEFAULT_LE,  # le mapping to quantiles
+        'error': 'error.class',
+        'query': 'db.query',
+    },
     'rpc_in': {
         'le': DEFAULT_LE,  # le mapping to quantiles
         'error': 'error.class',
         'method': 'rpc.method',
         'code': 'rpc.code',
     },
     'rpc_out': {
```

### Comparing `ipapp-2.0.0/ipapp/logger/adapters/requests.py` & `ipapp-2.0.1/ipapp/logger/adapters/requests.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/logger/adapters/sentry.py` & `ipapp-2.0.1/ipapp/logger/adapters/sentry.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/logger/adapters/zipkin.py` & `ipapp-2.0.1/ipapp/logger/adapters/zipkin.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/logger/logger.py` & `ipapp-2.0.1/ipapp/logger/logger.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/logger/span.py` & `ipapp-2.0.1/ipapp/logger/span.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/misc.py` & `ipapp-2.0.1/ipapp/misc.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/mq/pika.py` & `ipapp-2.0.1/ipapp/mq/pika.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/openapi/misc.py` & `ipapp-2.0.1/ipapp/openapi/misc.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/openapi/models.py` & `ipapp-2.0.1/ipapp/openapi/models.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/openapi/templates.py` & `ipapp-2.0.1/ipapp/openapi/templates.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/rpc/http/client.py` & `ipapp-2.0.1/ipapp/rpc/http/client.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/rpc/http/server.py` & `ipapp-2.0.1/ipapp/rpc/http/server.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/rpc/jsonrpc/error.py` & `ipapp-2.0.1/ipapp/rpc/jsonrpc/error.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/rpc/jsonrpc/http/client.py` & `ipapp-2.0.1/ipapp/rpc/jsonrpc/http/client.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/rpc/jsonrpc/http/server.py` & `ipapp-2.0.1/ipapp/rpc/jsonrpc/http/server.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/rpc/jsonrpc/main.py` & `ipapp-2.0.1/ipapp/rpc/jsonrpc/main.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/rpc/jsonrpc/mq/pika.py` & `ipapp-2.0.1/ipapp/rpc/jsonrpc/mq/pika.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/rpc/jsonrpc/openrpc/discover.py` & `ipapp-2.0.1/ipapp/rpc/jsonrpc/openrpc/discover.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/rpc/jsonrpc/openrpc/models.py` & `ipapp-2.0.1/ipapp/rpc/jsonrpc/openrpc/models.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/rpc/main.py` & `ipapp-2.0.1/ipapp/rpc/main.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/rpc/mq/pika.py` & `ipapp-2.0.1/ipapp/rpc/mq/pika.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/rpc/restrpc/error.py` & `ipapp-2.0.1/ipapp/rpc/restrpc/error.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/rpc/restrpc/http/client.py` & `ipapp-2.0.1/ipapp/rpc/restrpc/http/client.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/rpc/restrpc/http/server.py` & `ipapp-2.0.1/ipapp/rpc/restrpc/http/server.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/rpc/restrpc/main.py` & `ipapp-2.0.1/ipapp/rpc/restrpc/main.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/rpc/restrpc/openapi/misc.py` & `ipapp-2.0.1/ipapp/rpc/restrpc/openapi/misc.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/s3/boto.py` & `ipapp-2.0.1/ipapp/s3/boto.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/s3/models.py` & `ipapp-2.0.1/ipapp/s3/models.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/sftp/client.py` & `ipapp-2.0.1/ipapp/sftp/client.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/sphinx/config.py` & `ipapp-2.0.1/ipapp/sphinx/config.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/task/db.py` & `ipapp-2.0.1/ipapp/task/db.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/utils/lock/local.py` & `ipapp-2.0.1/ipapp/utils/lock/local.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/utils/lock/main.py` & `ipapp-2.0.1/ipapp/utils/lock/main.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/utils/lock/pg.py` & `ipapp-2.0.1/ipapp/utils/lock/pg.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/ipapp/utils/lock/redis.py` & `ipapp-2.0.1/ipapp/utils/lock/redis.py`

 * *Files identical despite different names*

### Comparing `ipapp-2.0.0/pyproject.toml` & `ipapp-2.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 force_grid_wrap = 0
 multi_line_output = 3
 use_parentheses = true
 include_trailing_comma = true
 
 [tool.poetry]
 name = "ipapp"
-version = "2.0.0"
+version = "2.0.1"
 description = "InPlat application framework"
 authors = ["InPlat"]
 classifiers = [
     'Intended Audience :: Developers',
     'Intended Audience :: Information Technology',
     'Intended Audience :: System Administrators',
     'Operating System :: Unix',
```

### Comparing `ipapp-2.0.0/PKG-INFO` & `ipapp-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipapp
-Version: 2.0.0
+Version: 2.0.1
 Summary: InPlat application framework
 Home-page: https://github.com/inplat/ipapp
 License: MIT
 Author: InPlat
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

