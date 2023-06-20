# Comparing `tmp/ftw.solr-2.9.4.tar.gz` & `tmp/ftw.solr-2.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ftw.solr-2.9.4.tar", last modified: Thu Jul 29 06:30:34 2021, max compression
+gzip compressed data, was "dist/ftw.solr-2.9.5.tar", last modified: Tue Aug 17 14:19:21 2021, max compression
```

## Comparing `ftw.solr-2.9.4.tar` & `ftw.solr-2.9.5.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 niklausjohner   (501) staff       (20)        0 2021-07-29 06:30:34.000000 ftw.solr-2.9.4/
--rw-r--r--   0 niklausjohner   (501) staff       (20)    11821 2021-07-29 06:30:34.000000 ftw.solr-2.9.4/PKG-INFO
-drwxr-xr-x   0 niklausjohner   (501) staff       (20)        0 2021-07-29 06:30:34.000000 ftw.solr-2.9.4/ftw/
--rw-r--r--   0 niklausjohner   (501) staff       (20)       80 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/__init__.py
-drwxr-xr-x   0 niklausjohner   (501) staff       (20)        0 2021-07-29 06:30:34.000000 ftw.solr-2.9.4/ftw/solr/
--rw-r--r--   0 niklausjohner   (501) staff       (20)     2942 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/interfaces.py
--rw-r--r--   0 niklausjohner   (501) staff       (20)     1326 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/zcml.py
--rw-r--r--   0 niklausjohner   (501) staff       (20)     2766 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/configure.zcml
--rw-r--r--   0 niklausjohner   (501) staff       (20)     5631 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/query.py
-drwxr-xr-x   0 niklausjohner   (501) staff       (20)        0 2021-07-29 06:30:34.000000 ftw.solr-2.9.4/ftw/solr/tests/
--rw-r--r--   0 niklausjohner   (501) staff       (20)      619 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/tests/test_maintenance.py
--rw-r--r--   0 niklausjohner   (501) staff       (20)     1693 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/tests/test_setup.py
--rw-r--r--   0 niklausjohner   (501) staff       (20)     6266 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/tests/test_converters.py
--rw-r--r--   0 niklausjohner   (501) staff       (20)     2303 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/tests/test_response.py
--rw-r--r--   0 niklausjohner   (501) staff       (20)    19179 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/tests/test_handlers.py
--rw-r--r--   0 niklausjohner   (501) staff       (20)     4137 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/tests/test_search.py
--rw-r--r--   0 niklausjohner   (501) staff       (20)     6463 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/tests/test_contentlisting.py
--rw-r--r--   0 niklausjohner   (501) staff       (20)    13052 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/tests/test_connection.py
--rw-r--r--   0 niklausjohner   (501) staff       (20)        0 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/tests/__init__.py
--rw-r--r--   0 niklausjohner   (501) staff       (20)     1746 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/tests/test_schema.py
--rw-r--r--   0 niklausjohner   (501) staff       (20)     4232 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/tests/test_indexer.py
--rw-r--r--   0 niklausjohner   (501) staff       (20)      617 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/tests/utils.py
--rw-r--r--   0 niklausjohner   (501) staff       (20)     8893 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/tests/test_query.py
--rw-r--r--   0 niklausjohner   (501) staff       (20)      639 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/tests/test_helpers.py
--rw-r--r--   0 niklausjohner   (501) staff       (20)    10449 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/tests/test_integration.py
-drwxr-xr-x   0 niklausjohner   (501) staff       (20)        0 2021-07-29 06:30:34.000000 ftw.solr-2.9.4/ftw/solr/tests/data/
--rw-r--r--   0 niklausjohner   (501) staff       (20)      770 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/tests/data/bad_request.json
--rw-r--r--   0 niklausjohner   (501) staff       (20)     2327 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/tests/data/search.json
--rw-r--r--   0 niklausjohner   (501) staff       (20)      690 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/tests/data/doc.json
--rw-r--r--   0 niklausjohner   (501) staff       (20)     1135 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/tests/data/highlighting.json
--rw-r--r--   0 niklausjohner   (501) staff       (20)     2616 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/tests/data/search_with_facets.json
--rw-r--r--   0 niklausjohner   (501) staff       (20)     2754 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/tests/data/schema.json
--rw-r--r--   0 niklausjohner   (501) staff       (20)     2222 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/tests/test_document.py
--rw-r--r--   0 niklausjohner   (501) staff       (20)     7073 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/handlers.py
--rw-r--r--   0 niklausjohner   (501) staff       (20)       66 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/__init__.py
--rw-r--r--   0 niklausjohner   (501) staff       (20)      361 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/setuphandlers.py
--rw-r--r--   0 niklausjohner   (501) staff       (20)     4177 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/contentlisting.py
--rw-r--r--   0 niklausjohner   (501) staff       (20)    13273 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/connection.py
-drwxr-xr-x   0 niklausjohner   (501) staff       (20)        0 2021-07-29 06:30:34.000000 ftw.solr-2.9.4/ftw/solr/browser/
--rw-r--r--   0 niklausjohner   (501) staff       (20)      429 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/browser/configure.zcml
--rw-r--r--   0 niklausjohner   (501) staff       (20)    12005 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/browser/maintenance.py
--rw-r--r--   0 niklausjohner   (501) staff       (20)        0 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/browser/__init__.py
--rw-r--r--   0 niklausjohner   (501) staff       (20)     7648 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/patches.py
--rw-r--r--   0 niklausjohner   (501) staff       (20)     2037 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/indexer.py
--rw-r--r--   0 niklausjohner   (501) staff       (20)     2435 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/document.py
--rw-r--r--   0 niklausjohner   (501) staff       (20)     1959 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/search.py
--rw-r--r--   0 niklausjohner   (501) staff       (20)      433 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/meta.zcml
-drwxr-xr-x   0 niklausjohner   (501) staff       (20)        0 2021-07-29 06:30:34.000000 ftw.solr-2.9.4/ftw/solr/upgrades/
--rw-r--r--   0 niklausjohner   (501) staff       (20)        0 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/upgrades/__init__.py
-drwxr-xr-x   0 niklausjohner   (501) staff       (20)        0 2021-07-29 06:30:34.000000 ftw.solr-2.9.4/ftw/solr/upgrades/20200401111512_update_modified_index/
--rw-r--r--   0 niklausjohner   (501) staff       (20)        0 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/upgrades/20200401111512_update_modified_index/__init__.py
--rw-r--r--   0 niklausjohner   (501) staff       (20)     5413 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/upgrades/20200401111512_update_modified_index/upgrade.py
-drwxr-xr-x   0 niklausjohner   (501) staff       (20)        0 2021-07-29 06:30:34.000000 ftw.solr-2.9.4/ftw/solr/upgrades/20190816143230_add_enable_setting/
--rw-r--r--   0 niklausjohner   (501) staff       (20)      104 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/upgrades/20190816143230_add_enable_setting/registry.xml
--rw-r--r--   0 niklausjohner   (501) staff       (20)        0 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/upgrades/20190816143230_add_enable_setting/__init__.py
--rw-r--r--   0 niklausjohner   (501) staff       (20)      207 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/upgrades/20190816143230_add_enable_setting/upgrade.py
--rw-r--r--   0 niklausjohner   (501) staff       (20)     1556 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/converters.py
-drwxr-xr-x   0 niklausjohner   (501) staff       (20)        0 2021-07-29 06:30:34.000000 ftw.solr-2.9.4/ftw/solr/profiles/
-drwxr-xr-x   0 niklausjohner   (501) staff       (20)        0 2021-07-29 06:30:34.000000 ftw.solr-2.9.4/ftw/solr/profiles/default/
--rw-r--r--   0 niklausjohner   (501) staff       (20)      255 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/profiles/default/componentregistry.xml
--rw-r--r--   0 niklausjohner   (501) staff       (20)      105 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/profiles/default/registry.xml
--rw-r--r--   0 niklausjohner   (501) staff       (20)      150 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/profiles/default/browserlayer.xml
--rw-r--r--   0 niklausjohner   (501) staff       (20)       62 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/profiles/default/metadata.xml
-drwxr-xr-x   0 niklausjohner   (501) staff       (20)        0 2021-07-29 06:30:34.000000 ftw.solr-2.9.4/ftw/solr/profiles/uninstall/
--rw-r--r--   0 niklausjohner   (501) staff       (20)      274 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/profiles/uninstall/componentregistry.xml
--rw-r--r--   0 niklausjohner   (501) staff       (20)      118 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 niklausjohner   (501) staff       (20)     1974 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/testing.py
--rw-r--r--   0 niklausjohner   (501) staff       (20)      609 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/helpers.py
--rw-r--r--   0 niklausjohner   (501) staff       (20)     3464 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/commands.py
--rw-r--r--   0 niklausjohner   (501) staff       (20)     1297 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw/solr/schema.py
--rw-r--r--   0 niklausjohner   (501) staff       (20)       56 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/MANIFEST.in
-drwxr-xr-x   0 niklausjohner   (501) staff       (20)        0 2021-07-29 06:30:34.000000 ftw.solr-2.9.4/docs/
--rw-r--r--   0 niklausjohner   (501) staff       (20)    17987 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/docs/LICENSE.GPL
--rw-r--r--   0 niklausjohner   (501) staff       (20)     4321 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/docs/HISTORY.txt
--rw-r--r--   0 niklausjohner   (501) staff       (20)      736 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/docs/LICENSE.txt
--rw-r--r--   0 niklausjohner   (501) staff       (20)     1877 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/setup.py
--rw-r--r--   0 niklausjohner   (501) staff       (20)      337 2021-07-29 06:30:34.000000 ftw.solr-2.9.4/setup.cfg
--rw-r--r--   0 niklausjohner   (501) staff       (20)     3777 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/README.rst
-drwxr-xr-x   0 niklausjohner   (501) staff       (20)        0 2021-07-29 06:30:34.000000 ftw.solr-2.9.4/ftw.solr.egg-info/
--rw-r--r--   0 niklausjohner   (501) staff       (20)    11821 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw.solr.egg-info/PKG-INFO
--rw-r--r--   0 niklausjohner   (501) staff       (20)        1 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw.solr.egg-info/not-zip-safe
--rw-r--r--   0 niklausjohner   (501) staff       (20)        4 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw.solr.egg-info/namespace_packages.txt
--rw-r--r--   0 niklausjohner   (501) staff       (20)     2203 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw.solr.egg-info/SOURCES.txt
--rw-r--r--   0 niklausjohner   (501) staff       (20)      109 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw.solr.egg-info/entry_points.txt
--rw-r--r--   0 niklausjohner   (501) staff       (20)      352 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw.solr.egg-info/requires.txt
--rw-r--r--   0 niklausjohner   (501) staff       (20)        4 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw.solr.egg-info/top_level.txt
--rw-r--r--   0 niklausjohner   (501) staff       (20)        1 2021-07-29 06:30:33.000000 ftw.solr-2.9.4/ftw.solr.egg-info/dependency_links.txt
+drwxr-xr-x   0 niklausjohner   (501) staff       (20)        0 2021-08-17 14:19:21.000000 ftw.solr-2.9.5/
+-rw-r--r--   0 niklausjohner   (501) staff       (20)    11954 2021-08-17 14:19:21.000000 ftw.solr-2.9.5/PKG-INFO
+drwxr-xr-x   0 niklausjohner   (501) staff       (20)        0 2021-08-17 14:19:21.000000 ftw.solr-2.9.5/ftw/
+-rw-r--r--   0 niklausjohner   (501) staff       (20)       80 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/__init__.py
+drwxr-xr-x   0 niklausjohner   (501) staff       (20)        0 2021-08-17 14:19:21.000000 ftw.solr-2.9.5/ftw/solr/
+-rw-r--r--   0 niklausjohner   (501) staff       (20)     2942 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/interfaces.py
+-rw-r--r--   0 niklausjohner   (501) staff       (20)     1326 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/zcml.py
+-rw-r--r--   0 niklausjohner   (501) staff       (20)     2766 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/configure.zcml
+-rw-r--r--   0 niklausjohner   (501) staff       (20)     5631 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/query.py
+drwxr-xr-x   0 niklausjohner   (501) staff       (20)        0 2021-08-17 14:19:21.000000 ftw.solr-2.9.5/ftw/solr/tests/
+-rw-r--r--   0 niklausjohner   (501) staff       (20)      619 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/tests/test_maintenance.py
+-rw-r--r--   0 niklausjohner   (501) staff       (20)     1693 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/tests/test_setup.py
+-rw-r--r--   0 niklausjohner   (501) staff       (20)     6266 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/tests/test_converters.py
+-rw-r--r--   0 niklausjohner   (501) staff       (20)     2303 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/tests/test_response.py
+-rw-r--r--   0 niklausjohner   (501) staff       (20)    19179 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/tests/test_handlers.py
+-rw-r--r--   0 niklausjohner   (501) staff       (20)     4842 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/tests/test_search.py
+-rw-r--r--   0 niklausjohner   (501) staff       (20)     6463 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/tests/test_contentlisting.py
+-rw-r--r--   0 niklausjohner   (501) staff       (20)    13052 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/tests/test_connection.py
+-rw-r--r--   0 niklausjohner   (501) staff       (20)        0 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/tests/__init__.py
+-rw-r--r--   0 niklausjohner   (501) staff       (20)     1746 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/tests/test_schema.py
+-rw-r--r--   0 niklausjohner   (501) staff       (20)     4232 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/tests/test_indexer.py
+-rw-r--r--   0 niklausjohner   (501) staff       (20)      617 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/tests/utils.py
+-rw-r--r--   0 niklausjohner   (501) staff       (20)     8893 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/tests/test_query.py
+-rw-r--r--   0 niklausjohner   (501) staff       (20)      639 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/tests/test_helpers.py
+-rw-r--r--   0 niklausjohner   (501) staff       (20)    10449 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/tests/test_integration.py
+drwxr-xr-x   0 niklausjohner   (501) staff       (20)        0 2021-08-17 14:19:21.000000 ftw.solr-2.9.5/ftw/solr/tests/data/
+-rw-r--r--   0 niklausjohner   (501) staff       (20)      770 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/tests/data/bad_request.json
+-rw-r--r--   0 niklausjohner   (501) staff       (20)     2327 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/tests/data/search.json
+-rw-r--r--   0 niklausjohner   (501) staff       (20)      690 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/tests/data/doc.json
+-rw-r--r--   0 niklausjohner   (501) staff       (20)     1135 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/tests/data/highlighting.json
+-rw-r--r--   0 niklausjohner   (501) staff       (20)     2616 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/tests/data/search_with_facets.json
+-rw-r--r--   0 niklausjohner   (501) staff       (20)     2754 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/tests/data/schema.json
+-rw-r--r--   0 niklausjohner   (501) staff       (20)     2222 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/tests/test_document.py
+-rw-r--r--   0 niklausjohner   (501) staff       (20)     7073 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/handlers.py
+-rw-r--r--   0 niklausjohner   (501) staff       (20)       66 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/__init__.py
+-rw-r--r--   0 niklausjohner   (501) staff       (20)      361 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/setuphandlers.py
+-rw-r--r--   0 niklausjohner   (501) staff       (20)     4177 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/contentlisting.py
+-rw-r--r--   0 niklausjohner   (501) staff       (20)    13273 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/connection.py
+drwxr-xr-x   0 niklausjohner   (501) staff       (20)        0 2021-08-17 14:19:21.000000 ftw.solr-2.9.5/ftw/solr/browser/
+-rw-r--r--   0 niklausjohner   (501) staff       (20)      429 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/browser/configure.zcml
+-rw-r--r--   0 niklausjohner   (501) staff       (20)    12005 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/browser/maintenance.py
+-rw-r--r--   0 niklausjohner   (501) staff       (20)        0 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/browser/__init__.py
+-rw-r--r--   0 niklausjohner   (501) staff       (20)     7648 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/patches.py
+-rw-r--r--   0 niklausjohner   (501) staff       (20)     2037 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/indexer.py
+-rw-r--r--   0 niklausjohner   (501) staff       (20)     2435 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/document.py
+-rw-r--r--   0 niklausjohner   (501) staff       (20)     2671 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/search.py
+-rw-r--r--   0 niklausjohner   (501) staff       (20)      433 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/meta.zcml
+drwxr-xr-x   0 niklausjohner   (501) staff       (20)        0 2021-08-17 14:19:21.000000 ftw.solr-2.9.5/ftw/solr/upgrades/
+-rw-r--r--   0 niklausjohner   (501) staff       (20)        0 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/upgrades/__init__.py
+drwxr-xr-x   0 niklausjohner   (501) staff       (20)        0 2021-08-17 14:19:21.000000 ftw.solr-2.9.5/ftw/solr/upgrades/20200401111512_update_modified_index/
+-rw-r--r--   0 niklausjohner   (501) staff       (20)        0 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/upgrades/20200401111512_update_modified_index/__init__.py
+-rw-r--r--   0 niklausjohner   (501) staff       (20)     5413 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/upgrades/20200401111512_update_modified_index/upgrade.py
+drwxr-xr-x   0 niklausjohner   (501) staff       (20)        0 2021-08-17 14:19:21.000000 ftw.solr-2.9.5/ftw/solr/upgrades/20190816143230_add_enable_setting/
+-rw-r--r--   0 niklausjohner   (501) staff       (20)      104 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/upgrades/20190816143230_add_enable_setting/registry.xml
+-rw-r--r--   0 niklausjohner   (501) staff       (20)        0 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/upgrades/20190816143230_add_enable_setting/__init__.py
+-rw-r--r--   0 niklausjohner   (501) staff       (20)      207 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/upgrades/20190816143230_add_enable_setting/upgrade.py
+-rw-r--r--   0 niklausjohner   (501) staff       (20)     1556 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/converters.py
+drwxr-xr-x   0 niklausjohner   (501) staff       (20)        0 2021-08-17 14:19:21.000000 ftw.solr-2.9.5/ftw/solr/profiles/
+drwxr-xr-x   0 niklausjohner   (501) staff       (20)        0 2021-08-17 14:19:21.000000 ftw.solr-2.9.5/ftw/solr/profiles/default/
+-rw-r--r--   0 niklausjohner   (501) staff       (20)      255 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/profiles/default/componentregistry.xml
+-rw-r--r--   0 niklausjohner   (501) staff       (20)      105 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/profiles/default/registry.xml
+-rw-r--r--   0 niklausjohner   (501) staff       (20)      150 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/profiles/default/browserlayer.xml
+-rw-r--r--   0 niklausjohner   (501) staff       (20)       62 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/profiles/default/metadata.xml
+drwxr-xr-x   0 niklausjohner   (501) staff       (20)        0 2021-08-17 14:19:21.000000 ftw.solr-2.9.5/ftw/solr/profiles/uninstall/
+-rw-r--r--   0 niklausjohner   (501) staff       (20)      274 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/profiles/uninstall/componentregistry.xml
+-rw-r--r--   0 niklausjohner   (501) staff       (20)      118 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 niklausjohner   (501) staff       (20)     1974 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/testing.py
+-rw-r--r--   0 niklausjohner   (501) staff       (20)      609 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/helpers.py
+-rw-r--r--   0 niklausjohner   (501) staff       (20)     3464 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/commands.py
+-rw-r--r--   0 niklausjohner   (501) staff       (20)     1297 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw/solr/schema.py
+-rw-r--r--   0 niklausjohner   (501) staff       (20)       56 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/MANIFEST.in
+drwxr-xr-x   0 niklausjohner   (501) staff       (20)        0 2021-08-17 14:19:21.000000 ftw.solr-2.9.5/docs/
+-rw-r--r--   0 niklausjohner   (501) staff       (20)    17987 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/docs/LICENSE.GPL
+-rw-r--r--   0 niklausjohner   (501) staff       (20)     4406 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/docs/HISTORY.txt
+-rw-r--r--   0 niklausjohner   (501) staff       (20)      736 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/docs/LICENSE.txt
+-rw-r--r--   0 niklausjohner   (501) staff       (20)     1877 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/setup.py
+-rw-r--r--   0 niklausjohner   (501) staff       (20)      337 2021-08-17 14:19:21.000000 ftw.solr-2.9.5/setup.cfg
+-rw-r--r--   0 niklausjohner   (501) staff       (20)     3777 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/README.rst
+drwxr-xr-x   0 niklausjohner   (501) staff       (20)        0 2021-08-17 14:19:21.000000 ftw.solr-2.9.5/ftw.solr.egg-info/
+-rw-r--r--   0 niklausjohner   (501) staff       (20)    11954 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw.solr.egg-info/PKG-INFO
+-rw-r--r--   0 niklausjohner   (501) staff       (20)        1 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw.solr.egg-info/not-zip-safe
+-rw-r--r--   0 niklausjohner   (501) staff       (20)        4 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw.solr.egg-info/namespace_packages.txt
+-rw-r--r--   0 niklausjohner   (501) staff       (20)     2203 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw.solr.egg-info/SOURCES.txt
+-rw-r--r--   0 niklausjohner   (501) staff       (20)      109 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw.solr.egg-info/entry_points.txt
+-rw-r--r--   0 niklausjohner   (501) staff       (20)      352 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw.solr.egg-info/requires.txt
+-rw-r--r--   0 niklausjohner   (501) staff       (20)        4 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw.solr.egg-info/top_level.txt
+-rw-r--r--   0 niklausjohner   (501) staff       (20)        1 2021-08-17 14:19:20.000000 ftw.solr-2.9.5/ftw.solr.egg-info/dependency_links.txt
```

### Comparing `ftw.solr-2.9.4/PKG-INFO` & `ftw.solr-2.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftw.solr
-Version: 2.9.4
+Version: 2.9.5
 Summary: Solr integration for Plone
 Home-page: https://pypi.python.org/pypi/ftw.solr
 Author: Thomas Buchberger
 Author-email: t.buchberger@4teamwork.ch
 License: GPL version 2
 Description: Introduction
         ============
@@ -158,14 +158,20 @@
         
         ``ftw.solr`` is licensed under GNU General Public License, version 2.
         
         
         Changelog
         =========
         
+        2.9.5 (2021-08-17)
+        ------------------
+        
+        - Add unrestricted_search method. [njohner]
+        
+        
         2.9.4 (2021-07-29)
         ------------------
         
         - SolrDocument returns None for existing fields with missing value. [njohner]
         
         
         2.9.3 (2021-04-22)
```

### Comparing `ftw.solr-2.9.4/ftw/solr/interfaces.py` & `ftw.solr-2.9.5/ftw/solr/interfaces.py`

 * *Files identical despite different names*

### Comparing `ftw.solr-2.9.4/ftw/solr/zcml.py` & `ftw.solr-2.9.5/ftw/solr/zcml.py`

 * *Files identical despite different names*

### Comparing `ftw.solr-2.9.4/ftw/solr/configure.zcml` & `ftw.solr-2.9.5/ftw/solr/configure.zcml`

 * *Files identical despite different names*

### Comparing `ftw.solr-2.9.4/ftw/solr/query.py` & `ftw.solr-2.9.5/ftw/solr/query.py`

 * *Files identical despite different names*

### Comparing `ftw.solr-2.9.4/ftw/solr/tests/test_maintenance.py` & `ftw.solr-2.9.5/ftw/solr/tests/test_maintenance.py`

 * *Files identical despite different names*

### Comparing `ftw.solr-2.9.4/ftw/solr/tests/test_setup.py` & `ftw.solr-2.9.5/ftw/solr/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `ftw.solr-2.9.4/ftw/solr/tests/test_converters.py` & `ftw.solr-2.9.5/ftw/solr/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `ftw.solr-2.9.4/ftw/solr/tests/test_response.py` & `ftw.solr-2.9.5/ftw/solr/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `ftw.solr-2.9.4/ftw/solr/tests/test_handlers.py` & `ftw.solr-2.9.5/ftw/solr/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `ftw.solr-2.9.4/ftw/solr/tests/test_search.py` & `ftw.solr-2.9.5/ftw/solr/tests/test_search.py`

 * *Files 11% similar despite different names*

```diff
@@ -101,7 +101,24 @@
             {u'hl': u'on', u'hl.fl': u'SearchableText'},
             )
 
     def test_search_with_custom_request_handler(self):
         self.solr.search(request_handler='/query')
         args, kwargs = self.conn.search.call_args
         self.assertEqual(kwargs, {'request_handler': u'/query'})
+
+    def test_search_contains_security_filters(self):
+        self.solr.search()
+        args, kwargs = self.conn.search.call_args
+        self.assertEqual(
+            args[0][u'filter'],
+            [u'allowedRolesAndUsers:(Member OR Authenticated OR Anonymous OR '
+             u'user\\:AuthenticatedUsers OR user\\:test_user_1_)'])
+
+    def test_search_does_not_allow_unrestricted_keyword(self):
+        with self.assertRaises(TypeError):
+            self.solr.search(unrestricted=True)
+
+    def test_unrestricted_search_does_not_contain_security_filters(self):
+        self.solr.unrestricted_search()
+        args, kwargs = self.conn.search.call_args
+        self.assertEqual(args[0][u'filter'], [])
```

### Comparing `ftw.solr-2.9.4/ftw/solr/tests/test_contentlisting.py` & `ftw.solr-2.9.5/ftw/solr/tests/test_contentlisting.py`

 * *Files identical despite different names*

### Comparing `ftw.solr-2.9.4/ftw/solr/tests/test_connection.py` & `ftw.solr-2.9.5/ftw/solr/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `ftw.solr-2.9.4/ftw/solr/tests/test_schema.py` & `ftw.solr-2.9.5/ftw/solr/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `ftw.solr-2.9.4/ftw/solr/tests/test_indexer.py` & `ftw.solr-2.9.5/ftw/solr/tests/test_indexer.py`

 * *Files identical despite different names*

### Comparing `ftw.solr-2.9.4/ftw/solr/tests/utils.py` & `ftw.solr-2.9.5/ftw/solr/tests/utils.py`

 * *Files identical despite different names*

### Comparing `ftw.solr-2.9.4/ftw/solr/tests/test_query.py` & `ftw.solr-2.9.5/ftw/solr/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `ftw.solr-2.9.4/ftw/solr/tests/test_helpers.py` & `ftw.solr-2.9.5/ftw/solr/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `ftw.solr-2.9.4/ftw/solr/tests/test_integration.py` & `ftw.solr-2.9.5/ftw/solr/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `ftw.solr-2.9.4/ftw/solr/tests/data/bad_request.json` & `ftw.solr-2.9.5/ftw/solr/tests/data/bad_request.json`

 * *Files identical despite different names*

### Comparing `ftw.solr-2.9.4/ftw/solr/tests/data/search.json` & `ftw.solr-2.9.5/ftw/solr/tests/data/search.json`

 * *Files identical despite different names*

### Comparing `ftw.solr-2.9.4/ftw/solr/tests/data/doc.json` & `ftw.solr-2.9.5/ftw/solr/tests/data/doc.json`

 * *Files identical despite different names*

### Comparing `ftw.solr-2.9.4/ftw/solr/tests/data/highlighting.json` & `ftw.solr-2.9.5/ftw/solr/tests/data/highlighting.json`

 * *Files identical despite different names*

### Comparing `ftw.solr-2.9.4/ftw/solr/tests/data/search_with_facets.json` & `ftw.solr-2.9.5/ftw/solr/tests/data/search_with_facets.json`

 * *Files identical despite different names*

### Comparing `ftw.solr-2.9.4/ftw/solr/tests/data/schema.json` & `ftw.solr-2.9.5/ftw/solr/tests/data/schema.json`

 * *Files identical despite different names*

### Comparing `ftw.solr-2.9.4/ftw/solr/tests/test_document.py` & `ftw.solr-2.9.5/ftw/solr/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `ftw.solr-2.9.4/ftw/solr/handlers.py` & `ftw.solr-2.9.5/ftw/solr/handlers.py`

 * *Files identical despite different names*

### Comparing `ftw.solr-2.9.4/ftw/solr/contentlisting.py` & `ftw.solr-2.9.5/ftw/solr/contentlisting.py`

 * *Files identical despite different names*

### Comparing `ftw.solr-2.9.4/ftw/solr/connection.py` & `ftw.solr-2.9.5/ftw/solr/connection.py`

 * *Files identical despite different names*

### Comparing `ftw.solr-2.9.4/ftw/solr/browser/maintenance.py` & `ftw.solr-2.9.5/ftw/solr/browser/maintenance.py`

 * *Files identical despite different names*

### Comparing `ftw.solr-2.9.4/ftw/solr/patches.py` & `ftw.solr-2.9.5/ftw/solr/patches.py`

 * *Files identical despite different names*

### Comparing `ftw.solr-2.9.4/ftw/solr/indexer.py` & `ftw.solr-2.9.5/ftw/solr/indexer.py`

 * *Files identical despite different names*

### Comparing `ftw.solr-2.9.4/ftw/solr/document.py` & `ftw.solr-2.9.5/ftw/solr/document.py`

 * *Files identical despite different names*

### Comparing `ftw.solr-2.9.4/ftw/solr/search.py` & `ftw.solr-2.9.5/ftw/solr/search.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,31 +16,44 @@
 
     @property
     def manager(self):
         if self._manager is None:
             self._manager = queryUtility(ISolrConnectionManager)
         return self._manager
 
-    def search(self, request_handler=u'/select', query=u'*:*', filters=None,
-               start=0, rows=1000, sort=None, **params):
+    def _search(self, request_handler=u'/select', query=u'*:*', filters=None,
+                start=0, rows=1000, sort=None, unrestricted=False, **params):
         conn = self.manager.connection
         params = {u'params': params}
         params[u'query'] = query
         params[u'offset'] = start
         params[u'limit'] = rows
         if sort is not None:
             params[u'sort'] = sort
         if filters is None:
             filters = []
         if not isinstance(filters, list):
             filters = [filters]
-        filters.insert(0, self.security_filter())
+        if not unrestricted:
+            filters.insert(0, self.security_filter())
         params[u'filter'] = filters
         return conn.search(params, request_handler=request_handler)
 
+    def search(self, request_handler=u'/select', query=u'*:*', filters=None,
+               start=0, rows=1000, sort=None, **params):
+        return self._search(
+            request_handler=request_handler, query=query, filters=filters,
+            start=start, rows=rows, sort=sort, unrestricted=False, **params)
+
+    def unrestricted_search(self, request_handler=u'/select', query=u'*:*',
+                            filters=None, start=0, rows=1000, sort=None, **params):
+        return self._search(
+            request_handler=request_handler, query=query, filters=filters,
+            start=start, rows=rows, sort=sort, unrestricted=True, **params)
+
     def security_filter(self):
         user = getSecurityManager().getUser()
         roles = user.getRoles()
         if 'Anonymous' in roles:
             return u'allowedRolesAndUsers:Anonymous'
         roles = list(roles)
         roles.append('Anonymous')
```

### Comparing `ftw.solr-2.9.4/ftw/solr/upgrades/20200401111512_update_modified_index/upgrade.py` & `ftw.solr-2.9.5/ftw/solr/upgrades/20200401111512_update_modified_index/upgrade.py`

 * *Files identical despite different names*

### Comparing `ftw.solr-2.9.4/ftw/solr/converters.py` & `ftw.solr-2.9.5/ftw/solr/converters.py`

 * *Files identical despite different names*

### Comparing `ftw.solr-2.9.4/ftw/solr/testing.py` & `ftw.solr-2.9.5/ftw/solr/testing.py`

 * *Files identical despite different names*

### Comparing `ftw.solr-2.9.4/ftw/solr/helpers.py` & `ftw.solr-2.9.5/ftw/solr/helpers.py`

 * *Files identical despite different names*

### Comparing `ftw.solr-2.9.4/ftw/solr/commands.py` & `ftw.solr-2.9.5/ftw/solr/commands.py`

 * *Files identical despite different names*

### Comparing `ftw.solr-2.9.4/ftw/solr/schema.py` & `ftw.solr-2.9.5/ftw/solr/schema.py`

 * *Files identical despite different names*

### Comparing `ftw.solr-2.9.4/docs/LICENSE.GPL` & `ftw.solr-2.9.5/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `ftw.solr-2.9.4/docs/HISTORY.txt` & `ftw.solr-2.9.5/docs/HISTORY.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+2.9.5 (2021-08-17)
+------------------
+
+- Add unrestricted_search method. [njohner]
+
+
 2.9.4 (2021-07-29)
 ------------------
 
 - SolrDocument returns None for existing fields with missing value. [njohner]
 
 
 2.9.3 (2021-04-22)
```

### Comparing `ftw.solr-2.9.4/docs/LICENSE.txt` & `ftw.solr-2.9.5/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ftw.solr-2.9.4/setup.py` & `ftw.solr-2.9.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     'pytz',
     'mock',
     'ftw.testing',
 ]
 
 setup(
     name='ftw.solr',
-    version='2.9.4',
+    version='2.9.5',
     description="Solr integration for Plone",
     long_description=long_description,
     # Get more from https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: 4.3",
```

### Comparing `ftw.solr-2.9.4/README.rst` & `ftw.solr-2.9.5/README.rst`

 * *Files identical despite different names*

### Comparing `ftw.solr-2.9.4/ftw.solr.egg-info/PKG-INFO` & `ftw.solr-2.9.5/ftw.solr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftw.solr
-Version: 2.9.4
+Version: 2.9.5
 Summary: Solr integration for Plone
 Home-page: https://pypi.python.org/pypi/ftw.solr
 Author: Thomas Buchberger
 Author-email: t.buchberger@4teamwork.ch
 License: GPL version 2
 Description: Introduction
         ============
@@ -158,14 +158,20 @@
         
         ``ftw.solr`` is licensed under GNU General Public License, version 2.
         
         
         Changelog
         =========
         
+        2.9.5 (2021-08-17)
+        ------------------
+        
+        - Add unrestricted_search method. [njohner]
+        
+        
         2.9.4 (2021-07-29)
         ------------------
         
         - SolrDocument returns None for existing fields with missing value. [njohner]
         
         
         2.9.3 (2021-04-22)
```

### Comparing `ftw.solr-2.9.4/ftw.solr.egg-info/SOURCES.txt` & `ftw.solr-2.9.5/ftw.solr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

