# Comparing `tmp/coindicator-2.1.9.tar.gz` & `tmp/coindicator-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coindicator-2.1.9.tar", last modified: Mon Jun 19 12:28:40 2023, max compression
+gzip compressed data, was "coindicator-2.2.0.tar", last modified: Tue Jun 20 09:00:26 2023, max compression
```

## Comparing `coindicator-2.1.9.tar` & `coindicator-2.2.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 12:28:40.740574 coindicator-2.1.9/
--rw-rw-r--   0 sander    (1000) sander    (1000)       83 2023-06-16 13:19:52.000000 coindicator-2.1.9/.gitignore
--rw-rw-r--   0 sander    (1000) sander    (1000)      899 2022-10-30 19:56:43.000000 coindicator-2.1.9/.pre-commit-config.yaml
--rw-r--r--   0 sander    (1000) sander    (1000)     1106 2020-04-16 00:57:46.000000 coindicator-2.1.9/LICENSE
--rw-rw-r--   0 sander    (1000) sander    (1000)       29 2023-06-16 13:19:52.000000 coindicator-2.1.9/MANIFEST.in
--rw-rw-r--   0 sander    (1000) sander    (1000)     4402 2023-06-19 12:28:40.740574 coindicator-2.1.9/PKG-INFO
--rw-rw-r--   0 sander    (1000) sander    (1000)     3891 2023-06-19 12:03:38.000000 coindicator-2.1.9/README.md
--rw-rw-r--   0 sander    (1000) sander    (1000)      369 2023-06-16 13:19:52.000000 coindicator-2.1.9/coindicator.desktop
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 12:28:40.728574 coindicator-2.1.9/img/
--rw-rw-r--   0 sander    (1000) sander    (1000)    27147 2022-10-30 19:56:43.000000 coindicator-2.1.9/img/gitcoin.png
--rw-rw-r--   0 sander    (1000) sander    (1000)   172307 2022-10-30 19:56:43.000000 coindicator-2.1.9/img/screenshot.png
--rwxrwxr-x   0 sander    (1000) sander    (1000)     1542 2023-06-19 12:18:20.000000 coindicator-2.1.9/install.sh
--rw-rw-r--   0 sander    (1000) sander    (1000)      294 2023-06-16 13:19:52.000000 coindicator-2.1.9/pyproject.toml
--rw-rw-r--   0 sander    (1000) sander    (1000)      667 2023-06-19 12:20:03.000000 coindicator-2.1.9/requirements.txt
--rw-rw-r--   0 sander    (1000) sander    (1000)     1165 2023-06-19 12:28:40.744574 coindicator-2.1.9/setup.cfg
--rw-rw-r--   0 sander    (1000) sander    (1000)      521 2023-06-16 13:19:52.000000 coindicator-2.1.9/setup.py
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 12:28:40.720574 coindicator-2.1.9/src/
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 12:28:40.732574 coindicator-2.1.9/src/coin/
--rw-rw-r--   0 sander    (1000) sander    (1000)        0 2022-10-30 19:56:43.000000 coindicator-2.1.9/src/coin/__init__.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1537 2023-06-16 13:19:52.000000 coindicator-2.1.9/src/coin/about.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     6527 2023-06-19 12:22:07.000000 coindicator-2.1.9/src/coin/alarm.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     5794 2022-10-30 19:56:43.000000 coindicator-2.1.9/src/coin/asset_selection.py
--rwxrwxr-x   0 sander    (1000) sander    (1000)    12085 2023-06-19 12:22:14.000000 coindicator-2.1.9/src/coin/coin.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1751 2023-06-16 13:19:52.000000 coindicator-2.1.9/src/coin/coingecko_client.py
--rw-rw-r--   0 sander    (1000) sander    (1000)      609 2022-10-30 19:56:43.000000 coindicator-2.1.9/src/coin/config.py
--rw-rw-r--   0 sander    (1000) sander    (1000)      977 2023-06-16 13:19:52.000000 coindicator-2.1.9/src/coin/config.yaml
--rw-rw-r--   0 sander    (1000) sander    (1000)     1422 2022-10-30 19:56:43.000000 coindicator-2.1.9/src/coin/downloader.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1177 2022-10-30 19:56:43.000000 coindicator-2.1.9/src/coin/error.py
--rw-rw-r--   0 sander    (1000) sander    (1000)    10640 2023-06-19 12:08:35.000000 coindicator-2.1.9/src/coin/exchange.py
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 12:28:40.736574 coindicator-2.1.9/src/coin/exchanges/
--rw-rw-r--   0 sander    (1000) sander    (1000)     1761 2023-06-19 12:04:55.000000 coindicator-2.1.9/src/coin/exchanges/binance.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1569 2023-06-19 12:04:53.000000 coindicator-2.1.9/src/coin/exchanges/bitfinex.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1824 2023-06-19 12:04:53.000000 coindicator-2.1.9/src/coin/exchanges/bitkub.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1483 2023-06-19 12:04:53.000000 coindicator-2.1.9/src/coin/exchanges/bitstamp.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     2031 2023-06-19 12:03:08.000000 coindicator-2.1.9/src/coin/exchanges/bittrex.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1473 2023-06-19 12:03:08.000000 coindicator-2.1.9/src/coin/exchanges/cexio.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1489 2023-06-19 12:04:53.000000 coindicator-2.1.9/src/coin/exchanges/gemini.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1708 2023-06-19 12:04:53.000000 coindicator-2.1.9/src/coin/exchanges/hitbtc.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     2073 2023-06-19 12:04:53.000000 coindicator-2.1.9/src/coin/exchanges/kraken.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1273 2023-06-19 12:05:15.000000 coindicator-2.1.9/src/coin/exchanges/okcoin.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1547 2023-06-19 12:03:08.000000 coindicator-2.1.9/src/coin/exchanges/poloniex.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1271 2023-06-19 12:04:53.000000 coindicator-2.1.9/src/coin/exchanges/unocoin.py
--rw-rw-r--   0 sander    (1000) sander    (1000)    10370 2022-10-30 19:56:43.000000 coindicator-2.1.9/src/coin/indicator.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     2528 2023-06-19 12:22:38.000000 coindicator-2.1.9/src/coin/plugin_selection.py
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 12:28:40.740574 coindicator-2.1.9/src/coin/resources/
--rw-rw-r--   0 sander    (1000) sander    (1000)   294232 2023-06-16 13:19:52.000000 coindicator-2.1.9/src/coin/resources/ca-ching.wav
--rw-rw-r--   0 sander    (1000) sander    (1000)     5060 2022-10-30 19:56:43.000000 coindicator-2.1.9/src/coin/resources/icon.png
--rw-rw-r--   0 sander    (1000) sander    (1000)      983 2022-10-30 19:56:43.000000 coindicator-2.1.9/src/coin/resources/icon_32px.png
--rw-rw-r--   0 sander    (1000) sander    (1000)     1440 2022-10-30 19:56:43.000000 coindicator-2.1.9/src/coin/resources/icon_48px.png
--rw-rw-r--   0 sander    (1000) sander    (1000)     1673 2022-10-30 19:56:43.000000 coindicator-2.1.9/src/coin/resources/icon_64px.png
--rw-rw-r--   0 sander    (1000) sander    (1000)     1889 2022-10-30 19:56:43.000000 coindicator-2.1.9/src/coin/resources/loading.png
--rw-rw-r--   0 sander    (1000) sander    (1000)     4619 2022-10-30 19:56:43.000000 coindicator-2.1.9/src/coin/resources/logo_124px.png
--rw-rw-r--   0 sander    (1000) sander    (1000)     7329 2022-10-30 19:56:43.000000 coindicator-2.1.9/src/coin/resources/logo_124pxs.png
--rw-rw-r--   0 sander    (1000) sander    (1000)     6508 2022-10-30 19:56:43.000000 coindicator-2.1.9/src/coin/resources/logo_248px.png
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 12:28:40.740574 coindicator-2.1.9/src/coindicator.egg-info/
--rw-rw-r--   0 sander    (1000) sander    (1000)     4402 2023-06-19 12:28:40.000000 coindicator-2.1.9/src/coindicator.egg-info/PKG-INFO
--rw-rw-r--   0 sander    (1000) sander    (1000)     1388 2023-06-19 12:28:40.000000 coindicator-2.1.9/src/coindicator.egg-info/SOURCES.txt
--rw-rw-r--   0 sander    (1000) sander    (1000)        1 2023-06-19 12:28:40.000000 coindicator-2.1.9/src/coindicator.egg-info/dependency_links.txt
--rw-rw-r--   0 sander    (1000) sander    (1000)       47 2023-06-19 12:28:40.000000 coindicator-2.1.9/src/coindicator.egg-info/entry_points.txt
--rw-rw-r--   0 sander    (1000) sander    (1000)        1 2023-06-16 11:50:35.000000 coindicator-2.1.9/src/coindicator.egg-info/not-zip-safe
--rw-rw-r--   0 sander    (1000) sander    (1000)      192 2023-06-19 12:28:40.000000 coindicator-2.1.9/src/coindicator.egg-info/requires.txt
--rw-rw-r--   0 sander    (1000) sander    (1000)        5 2023-06-19 12:28:40.000000 coindicator-2.1.9/src/coindicator.egg-info/top_level.txt
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-20 09:00:26.227807 coindicator-2.2.0/
+-rw-rw-r--   0 sander    (1000) sander    (1000)       83 2023-06-16 13:19:52.000000 coindicator-2.2.0/.gitignore
+-rw-rw-r--   0 sander    (1000) sander    (1000)      899 2022-10-30 19:56:43.000000 coindicator-2.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 sander    (1000) sander    (1000)     1106 2020-04-16 00:57:46.000000 coindicator-2.2.0/LICENSE
+-rw-rw-r--   0 sander    (1000) sander    (1000)       29 2023-06-16 13:19:52.000000 coindicator-2.2.0/MANIFEST.in
+-rw-rw-r--   0 sander    (1000) sander    (1000)     4402 2023-06-20 09:00:26.227807 coindicator-2.2.0/PKG-INFO
+-rw-rw-r--   0 sander    (1000) sander    (1000)     3891 2023-06-19 12:03:38.000000 coindicator-2.2.0/README.md
+-rw-rw-r--   0 sander    (1000) sander    (1000)      369 2023-06-16 13:19:52.000000 coindicator-2.2.0/coindicator.desktop
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-20 09:00:26.215806 coindicator-2.2.0/img/
+-rw-rw-r--   0 sander    (1000) sander    (1000)    27147 2022-10-30 19:56:43.000000 coindicator-2.2.0/img/gitcoin.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)   172307 2022-10-30 19:56:43.000000 coindicator-2.2.0/img/screenshot.png
+-rwxrwxr-x   0 sander    (1000) sander    (1000)     1573 2023-06-20 08:18:13.000000 coindicator-2.2.0/install.sh
+-rw-rw-r--   0 sander    (1000) sander    (1000)      294 2023-06-16 13:19:52.000000 coindicator-2.2.0/pyproject.toml
+-rw-rw-r--   0 sander    (1000) sander    (1000)      798 2023-06-20 08:56:51.000000 coindicator-2.2.0/requirements.txt
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1174 2023-06-20 09:00:26.227807 coindicator-2.2.0/setup.cfg
+-rw-rw-r--   0 sander    (1000) sander    (1000)      521 2023-06-16 13:19:52.000000 coindicator-2.2.0/setup.py
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-20 09:00:26.211806 coindicator-2.2.0/src/
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-20 09:00:26.219806 coindicator-2.2.0/src/coin/
+-rw-rw-r--   0 sander    (1000) sander    (1000)        0 2022-10-30 19:56:43.000000 coindicator-2.2.0/src/coin/__init__.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1537 2023-06-16 13:19:52.000000 coindicator-2.2.0/src/coin/about.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     6480 2023-06-20 08:58:45.000000 coindicator-2.2.0/src/coin/alarm.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     5794 2022-10-30 19:56:43.000000 coindicator-2.2.0/src/coin/asset_selection.py
+-rwxrwxr-x   0 sander    (1000) sander    (1000)    12096 2023-06-20 08:58:45.000000 coindicator-2.2.0/src/coin/coin.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1751 2023-06-16 13:19:52.000000 coindicator-2.2.0/src/coin/coingecko_client.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)      609 2022-10-30 19:56:43.000000 coindicator-2.2.0/src/coin/config.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)      977 2023-06-16 13:19:52.000000 coindicator-2.2.0/src/coin/config.yaml
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1422 2022-10-30 19:56:43.000000 coindicator-2.2.0/src/coin/downloader.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1177 2022-10-30 19:56:43.000000 coindicator-2.2.0/src/coin/error.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)    10640 2023-06-19 12:08:35.000000 coindicator-2.2.0/src/coin/exchange.py
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-20 09:00:26.223806 coindicator-2.2.0/src/coin/exchanges/
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1761 2023-06-19 12:04:55.000000 coindicator-2.2.0/src/coin/exchanges/binance.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1569 2023-06-19 12:04:53.000000 coindicator-2.2.0/src/coin/exchanges/bitfinex.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1824 2023-06-19 12:04:53.000000 coindicator-2.2.0/src/coin/exchanges/bitkub.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1483 2023-06-19 12:04:53.000000 coindicator-2.2.0/src/coin/exchanges/bitstamp.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     2031 2023-06-19 12:03:08.000000 coindicator-2.2.0/src/coin/exchanges/bittrex.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1473 2023-06-19 12:03:08.000000 coindicator-2.2.0/src/coin/exchanges/cexio.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1489 2023-06-19 12:04:53.000000 coindicator-2.2.0/src/coin/exchanges/gemini.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1708 2023-06-19 12:04:53.000000 coindicator-2.2.0/src/coin/exchanges/hitbtc.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     2073 2023-06-19 12:04:53.000000 coindicator-2.2.0/src/coin/exchanges/kraken.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1273 2023-06-19 12:05:15.000000 coindicator-2.2.0/src/coin/exchanges/okcoin.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1547 2023-06-19 12:03:08.000000 coindicator-2.2.0/src/coin/exchanges/poloniex.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1271 2023-06-19 12:04:53.000000 coindicator-2.2.0/src/coin/exchanges/unocoin.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)    10370 2022-10-30 19:56:43.000000 coindicator-2.2.0/src/coin/indicator.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     2528 2023-06-19 12:22:38.000000 coindicator-2.2.0/src/coin/plugin_selection.py
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-20 09:00:26.227807 coindicator-2.2.0/src/coin/resources/
+-rw-rw-r--   0 sander    (1000) sander    (1000)   294232 2023-06-16 13:19:52.000000 coindicator-2.2.0/src/coin/resources/ca-ching.wav
+-rw-rw-r--   0 sander    (1000) sander    (1000)     5060 2022-10-30 19:56:43.000000 coindicator-2.2.0/src/coin/resources/icon.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)      983 2022-10-30 19:56:43.000000 coindicator-2.2.0/src/coin/resources/icon_32px.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1440 2022-10-30 19:56:43.000000 coindicator-2.2.0/src/coin/resources/icon_48px.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1673 2022-10-30 19:56:43.000000 coindicator-2.2.0/src/coin/resources/icon_64px.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1889 2022-10-30 19:56:43.000000 coindicator-2.2.0/src/coin/resources/loading.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)     4619 2022-10-30 19:56:43.000000 coindicator-2.2.0/src/coin/resources/logo_124px.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)     7329 2022-10-30 19:56:43.000000 coindicator-2.2.0/src/coin/resources/logo_124pxs.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)     6508 2022-10-30 19:56:43.000000 coindicator-2.2.0/src/coin/resources/logo_248px.png
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-20 09:00:26.227807 coindicator-2.2.0/src/coindicator.egg-info/
+-rw-rw-r--   0 sander    (1000) sander    (1000)     4402 2023-06-20 09:00:26.000000 coindicator-2.2.0/src/coindicator.egg-info/PKG-INFO
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1388 2023-06-20 09:00:26.000000 coindicator-2.2.0/src/coindicator.egg-info/SOURCES.txt
+-rw-rw-r--   0 sander    (1000) sander    (1000)        1 2023-06-20 09:00:26.000000 coindicator-2.2.0/src/coindicator.egg-info/dependency_links.txt
+-rw-rw-r--   0 sander    (1000) sander    (1000)       47 2023-06-20 09:00:26.000000 coindicator-2.2.0/src/coindicator.egg-info/entry_points.txt
+-rw-rw-r--   0 sander    (1000) sander    (1000)        1 2023-06-16 11:50:35.000000 coindicator-2.2.0/src/coindicator.egg-info/not-zip-safe
+-rw-rw-r--   0 sander    (1000) sander    (1000)      201 2023-06-20 09:00:26.000000 coindicator-2.2.0/src/coindicator.egg-info/requires.txt
+-rw-rw-r--   0 sander    (1000) sander    (1000)        5 2023-06-20 09:00:26.000000 coindicator-2.2.0/src/coindicator.egg-info/top_level.txt
```

### Comparing `coindicator-2.1.9/.pre-commit-config.yaml` & `coindicator-2.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.9/LICENSE` & `coindicator-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.9/PKG-INFO` & `coindicator-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coindicator
-Version: 2.1.9
+Version: 2.2.0
 Summary: Coinprice Indicator
 Home-page: https://github.com/bluppfisk/coindicator/
 Author: Sander Van de Moortel
 Author-email: sander.vandemoortel@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/bluppfisk/coindicator/
 Platform: Linux
```

### Comparing `coindicator-2.1.9/README.md` & `coindicator-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.9/img/gitcoin.png` & `coindicator-2.2.0/img/gitcoin.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.9/img/screenshot.png` & `coindicator-2.2.0/img/screenshot.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.9/install.sh` & `coindicator-2.2.0/install.sh`

 * *Files 6% similar despite different names*

```diff
@@ -39,13 +39,14 @@
 Type=Application
 Categories=Utility;
 Keywords=crypto;coin;ticker;price;exchange;
 StartupNotify=false
 Path=${args[0]}/venv/bin
 Exec=coindicator
 Icon=/tmp/logo_248px.png
+X-GNOME-UsesNotifications=true
 EOL
 
 cp ./src/coin/resources/logo_248px.png /tmp
 
 
 desktop-file-install --dir=$HOME/.local/share/applications /tmp/coindicator.desktop
```

### Comparing `coindicator-2.1.9/setup.cfg` & `coindicator-2.2.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -22,20 +22,20 @@
 include_package_data = True
 package_dir = 
 	=src
 install_requires = 
 	certifi>=2022.12.7
 	chardet~=3.0.4
 	idna~=2.7
-	notify2~=0.3.1
+	desktop-notifier~=3.5.3
 	PyYAML>=4.2b1
 	requests~=2.20
 	urllib3~=1.26.5
 	pygame~=2.1.2
-	PyGObject~=3.42.2
+	PyGObject~=3.44.1
 
 [options.packages.find]
 where = 
 	src
 
 [options.package_data]
 * =
```

### Comparing `coindicator-2.1.9/setup.py` & `coindicator-2.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.9/src/coin/about.py` & `coindicator-2.2.0/src/coin/about.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.9/src/coin/alarm.py` & `coindicator-2.2.0/src/coin/alarm.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Lets the user set an alert for a certain price point
 
-import notify2
+import desktop_notifier
 import pygame
 
 from coin.config import Config
 
 from gi.repository import Gdk, GdkPixbuf, Gtk
 from gi.repository.Gdk import Color
 
@@ -63,28 +63,27 @@
             + " "
             + direction
             + " "
             + self.parent.symbol
             + str(threshold)
         )
 
-        if notify2.init(self.app_name):
-            if pygame.init():
-                pygame.mixer.music.load(
-                    self.config["project_root"] / "resources/ca-ching.wav"
-                )
-                pygame.mixer.music.play()
-            logo = GdkPixbuf.Pixbuf.new_from_file(
-                str(self.config["project_root"] / "resources/icon_32px.png")
+        if pygame.init():
+            pygame.mixer.music.load(
+                self.config["project_root"] / "resources/ca-ching.wav"
             )
+            pygame.mixer.music.play()
 
-            n = notify2.Notification(title, message)
-            n.set_icon_from_pixbuf(logo)
-            n.set_urgency(2)  # highest
-            n.show()
+        notifier = desktop_notifier.DesktopNotifier(app_name=self.config["app"]["name"])
+        notifier.send_sync(
+            title,
+            message,
+            urgency=desktop_notifier.Urgency.Critical,
+            icon=str(self.config["project_root"] / "resources/icon_32px.png"),
+        )
 
 
 class AlarmSettingsWindow(Gtk.Window):
     def __init__(self, parent, price):
         Gtk.Window.__init__(self, title="Set price alert")
 
         self.parent = parent
```

### Comparing `coindicator-2.1.9/src/coin/asset_selection.py` & `coindicator-2.2.0/src/coin/asset_selection.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.9/src/coin/coin.py` & `coindicator-2.2.0/src/coin/coin.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 os.environ["PYGAME_HIDE_SUPPORT_PROMPT"] = "hide"
 
 import importlib
 import logging
 import signal
 from pathlib import Path
 
-import notify2
+import desktop_notifier
 import yaml
 from gi.repository import Gtk
 
 from coin.about import AboutWindow
 from coin.downloader import AsyncDownloadService, DownloadService
 from coin.indicator import Indicator
 from coin.plugin_selection import PluginSelectionWindow
@@ -290,23 +290,22 @@
             [ex for ex in self.exchanges.values() if ex.active and ex.discovery]
         ):
             return  # wait until all active exchanges with discovery finish discovery
 
         self.discoveries = 0
         self._load_assets()
 
-        if notify2.init(self.config.get("app").get("name")):
-            n = notify2.Notification(
-                self.config.get("app").get("name"),
-                "Finished discovering new assets",
-                str(self.icon),
-            )
-            n.set_urgency(1)
-            n.timeout = 2000
-            n.show()
+        notifier = desktop_notifier.DesktopNotifier(app_name=self.config["app"]["name"])
+        notifier.send_sync(
+            self.config.get("app").get("name"),
+            "Finished discovering new assets",
+            urgency=desktop_notifier.Urgency.Normal,
+            timeout=2000,
+            icon=self.icon,
+        )
 
         self.main_item.set_icon_full(str(self.icon), "App icon")
 
     def _select_plugins(self, _widget):
         PluginSelectionWindow(self)
 
     # Menu item to remove all tickers and quits the application
```

### Comparing `coindicator-2.1.9/src/coin/coingecko_client.py` & `coindicator-2.2.0/src/coin/coingecko_client.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.9/src/coin/config.py` & `coindicator-2.2.0/src/coin/config.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.9/src/coin/config.yaml` & `coindicator-2.2.0/src/coin/config.yaml`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.9/src/coin/downloader.py` & `coindicator-2.2.0/src/coin/downloader.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.9/src/coin/error.py` & `coindicator-2.2.0/src/coin/error.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.9/src/coin/exchange.py` & `coindicator-2.2.0/src/coin/exchange.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.9/src/coin/exchanges/binance.py` & `coindicator-2.2.0/src/coin/exchanges/binance.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.9/src/coin/exchanges/bitfinex.py` & `coindicator-2.2.0/src/coin/exchanges/bitfinex.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.9/src/coin/exchanges/bitkub.py` & `coindicator-2.2.0/src/coin/exchanges/bitkub.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.9/src/coin/exchanges/bitstamp.py` & `coindicator-2.2.0/src/coin/exchanges/bitstamp.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.9/src/coin/exchanges/bittrex.py` & `coindicator-2.2.0/src/coin/exchanges/bittrex.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.9/src/coin/exchanges/cexio.py` & `coindicator-2.2.0/src/coin/exchanges/cexio.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.9/src/coin/exchanges/gemini.py` & `coindicator-2.2.0/src/coin/exchanges/gemini.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.9/src/coin/exchanges/hitbtc.py` & `coindicator-2.2.0/src/coin/exchanges/hitbtc.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.9/src/coin/exchanges/kraken.py` & `coindicator-2.2.0/src/coin/exchanges/kraken.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.9/src/coin/exchanges/okcoin.py` & `coindicator-2.2.0/src/coin/exchanges/okcoin.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.9/src/coin/exchanges/poloniex.py` & `coindicator-2.2.0/src/coin/exchanges/poloniex.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.9/src/coin/exchanges/unocoin.py` & `coindicator-2.2.0/src/coin/exchanges/unocoin.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.9/src/coin/indicator.py` & `coindicator-2.2.0/src/coin/indicator.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.9/src/coin/plugin_selection.py` & `coindicator-2.2.0/src/coin/plugin_selection.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.9/src/coin/resources/ca-ching.wav` & `coindicator-2.2.0/src/coin/resources/ca-ching.wav`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.9/src/coin/resources/icon.png` & `coindicator-2.2.0/src/coin/resources/icon.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.9/src/coin/resources/icon_32px.png` & `coindicator-2.2.0/src/coin/resources/icon_32px.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.9/src/coin/resources/icon_48px.png` & `coindicator-2.2.0/src/coin/resources/icon_48px.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.9/src/coin/resources/icon_64px.png` & `coindicator-2.2.0/src/coin/resources/icon_64px.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.9/src/coin/resources/loading.png` & `coindicator-2.2.0/src/coin/resources/loading.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.9/src/coin/resources/logo_124px.png` & `coindicator-2.2.0/src/coin/resources/logo_124px.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.9/src/coin/resources/logo_124pxs.png` & `coindicator-2.2.0/src/coin/resources/logo_124pxs.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.9/src/coin/resources/logo_248px.png` & `coindicator-2.2.0/src/coin/resources/logo_248px.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.9/src/coindicator.egg-info/PKG-INFO` & `coindicator-2.2.0/src/coindicator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coindicator
-Version: 2.1.9
+Version: 2.2.0
 Summary: Coinprice Indicator
 Home-page: https://github.com/bluppfisk/coindicator/
 Author: Sander Van de Moortel
 Author-email: sander.vandemoortel@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/bluppfisk/coindicator/
 Platform: Linux
```

### Comparing `coindicator-2.1.9/src/coindicator.egg-info/SOURCES.txt` & `coindicator-2.2.0/src/coindicator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

