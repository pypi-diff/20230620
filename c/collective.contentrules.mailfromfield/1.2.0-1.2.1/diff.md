# Comparing `tmp/collective.contentrules.mailfromfield-1.2.0.tar.gz` & `tmp/collective.contentrules.mailfromfield-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.contentrules.mailfromfield-1.2.0.tar", last modified: Mon Jun 19 12:49:40 2023, max compression
+gzip compressed data, was "collective.contentrules.mailfromfield-1.2.1.tar", last modified: Tue Jun 20 07:31:14 2023, max compression
```

## Comparing `collective.contentrules.mailfromfield-1.2.0.tar` & `collective.contentrules.mailfromfield-1.2.1.tar`

### file list

```diff
@@ -1,47 +1,45 @@
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-19 12:49:40.757548 collective.contentrules.mailfromfield-1.2.0/
--rw-r--r--   0 cekk       (501) staff       (20)      225 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/MANIFEST.in
--rw-r--r--   0 cekk       (501) staff       (20)    11265 2023-06-19 12:49:40.757773 collective.contentrules.mailfromfield-1.2.0/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     6547 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/README.rst
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-19 12:49:40.748477 collective.contentrules.mailfromfield-1.2.0/collective/
--rw-r--r--   0 cekk       (501) staff       (20)       80 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-19 12:49:40.751164 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/
--rw-r--r--   0 cekk       (501) staff       (20)       80 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-19 12:49:40.752343 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/
--rw-r--r--   0 cekk       (501) staff       (20)      322 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-19 12:49:40.753143 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/actions/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/actions/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     1240 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/actions/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)    10004 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/actions/mail.py
--rw-r--r--   0 cekk       (501) staff       (20)      507 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/configure.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-19 12:49:40.754326 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/locales/
--rw-r--r--   0 cekk       (501) staff       (20)     2575 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/locales/collective.contentrules.mailfromfield.pot
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-19 12:49:40.746713 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/locales/it/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-19 12:49:40.755548 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/locales/it/LC_MESSAGES/
--rw-r--r--   0 cekk       (501) staff       (20)     2572 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/locales/it/LC_MESSAGES/collective.contentrules.mailfromfield.mo
--rw-r--r--   0 cekk       (501) staff       (20)     3752 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/locales/it/LC_MESSAGES/collective.contentrules.mailfromfield.po
--rw-r--r--   0 cekk       (501) staff       (20)      783 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/locales/it/LC_MESSAGES/plone.mo
--rw-r--r--   0 cekk       (501) staff       (20)      929 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/locales/it/LC_MESSAGES/plone.po
--rw-r--r--   0 cekk       (501) staff       (20)      744 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/locales/plone-manual.pot
--rw-r--r--   0 cekk       (501) staff       (20)      745 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/locales/plone.pot
--rwxr-xr-x   0 cekk       (501) staff       (20)      335 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/locales/rebuildAll.sh
--rw-r--r--   0 cekk       (501) staff       (20)     1030 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/testing.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-19 12:49:40.756080 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/tests/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/tests/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)    10943 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/tests/test_actions_mailfromfield.py
--rw-r--r--   0 cekk       (501) staff       (20)      963 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/vocabularies.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-19 12:49:40.750878 collective.contentrules.mailfromfield-1.2.0/collective.contentrules.mailfromfield.egg-info/
--rw-r--r--   0 cekk       (501) staff       (20)    11265 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective.contentrules.mailfromfield.egg-info/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     1786 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective.contentrules.mailfromfield.egg-info/SOURCES.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective.contentrules.mailfromfield.egg-info/dependency_links.txt
--rw-r--r--   0 cekk       (501) staff       (20)       59 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective.contentrules.mailfromfield.egg-info/entry_points.txt
--rw-r--r--   0 cekk       (501) staff       (20)       35 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective.contentrules.mailfromfield.egg-info/namespace_packages.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective.contentrules.mailfromfield.egg-info/not-zip-safe
--rw-r--r--   0 cekk       (501) staff       (20)       63 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective.contentrules.mailfromfield.egg-info/requires.txt
--rw-r--r--   0 cekk       (501) staff       (20)       11 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/collective.contentrules.mailfromfield.egg-info/top_level.txt
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-19 12:49:40.757290 collective.contentrules.mailfromfield-1.2.0/docs/
--rw-r--r--   0 cekk       (501) staff       (20)     1375 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/docs/HISTORY.rst
--rw-r--r--   0 cekk       (501) staff       (20)     1439 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/docs/INSTALL.txt
--rw-r--r--   0 cekk       (501) staff       (20)    17987 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/docs/LICENSE.GPL
--rw-r--r--   0 cekk       (501) staff       (20)      773 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/docs/LICENSE.txt
--rw-r--r--   0 cekk       (501) staff       (20)      518 2023-06-19 12:49:40.758457 collective.contentrules.mailfromfield-1.2.0/setup.cfg
--rw-r--r--   0 cekk       (501) staff       (20)     2140 2023-06-19 12:49:40.000000 collective.contentrules.mailfromfield-1.2.0/setup.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-20 07:31:14.760792 collective.contentrules.mailfromfield-1.2.1/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      225 2023-06-20 07:31:14.000000 collective.contentrules.mailfromfield-1.2.1/MANIFEST.in
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     9342 2023-06-20 07:31:14.760792 collective.contentrules.mailfromfield-1.2.1/PKG-INFO
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6547 2023-06-20 07:31:14.000000 collective.contentrules.mailfromfield-1.2.1/README.rst
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-20 07:31:14.760792 collective.contentrules.mailfromfield-1.2.1/collective/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       80 2023-06-20 07:31:14.000000 collective.contentrules.mailfromfield-1.2.1/collective/__init__.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-20 07:31:14.760792 collective.contentrules.mailfromfield-1.2.1/collective/contentrules/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       80 2023-06-20 07:31:14.000000 collective.contentrules.mailfromfield-1.2.1/collective/contentrules/__init__.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-20 07:31:14.760792 collective.contentrules.mailfromfield-1.2.1/collective/contentrules/mailfromfield/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      322 2023-06-20 07:31:14.000000 collective.contentrules.mailfromfield-1.2.1/collective/contentrules/mailfromfield/__init__.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-20 07:31:14.760792 collective.contentrules.mailfromfield-1.2.1/collective/contentrules/mailfromfield/actions/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-20 07:31:14.000000 collective.contentrules.mailfromfield-1.2.1/collective/contentrules/mailfromfield/actions/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1240 2023-06-20 07:31:14.000000 collective.contentrules.mailfromfield-1.2.1/collective/contentrules/mailfromfield/actions/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     9822 2023-06-20 07:31:14.000000 collective.contentrules.mailfromfield-1.2.1/collective/contentrules/mailfromfield/actions/mail.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      507 2023-06-20 07:31:14.000000 collective.contentrules.mailfromfield-1.2.1/collective/contentrules/mailfromfield/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-20 07:31:14.760792 collective.contentrules.mailfromfield-1.2.1/collective/contentrules/mailfromfield/locales/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2575 2023-06-20 07:31:14.000000 collective.contentrules.mailfromfield-1.2.1/collective/contentrules/mailfromfield/locales/collective.contentrules.mailfromfield.pot
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-20 07:31:14.760792 collective.contentrules.mailfromfield-1.2.1/collective/contentrules/mailfromfield/locales/it/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-20 07:31:14.760792 collective.contentrules.mailfromfield-1.2.1/collective/contentrules/mailfromfield/locales/it/LC_MESSAGES/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3752 2023-06-20 07:31:14.000000 collective.contentrules.mailfromfield-1.2.1/collective/contentrules/mailfromfield/locales/it/LC_MESSAGES/collective.contentrules.mailfromfield.po
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      929 2023-06-20 07:31:14.000000 collective.contentrules.mailfromfield-1.2.1/collective/contentrules/mailfromfield/locales/it/LC_MESSAGES/plone.po
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      744 2023-06-20 07:31:14.000000 collective.contentrules.mailfromfield-1.2.1/collective/contentrules/mailfromfield/locales/plone-manual.pot
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      745 2023-06-20 07:31:14.000000 collective.contentrules.mailfromfield-1.2.1/collective/contentrules/mailfromfield/locales/plone.pot
+-rwxrwxr-x   0 mauro     (1000) mauro     (1000)      335 2023-06-20 07:31:14.000000 collective.contentrules.mailfromfield-1.2.1/collective/contentrules/mailfromfield/locales/rebuildAll.sh
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1030 2023-06-20 07:31:14.000000 collective.contentrules.mailfromfield-1.2.1/collective/contentrules/mailfromfield/testing.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-20 07:31:14.760792 collective.contentrules.mailfromfield-1.2.1/collective/contentrules/mailfromfield/tests/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-06-20 07:31:14.000000 collective.contentrules.mailfromfield-1.2.1/collective/contentrules/mailfromfield/tests/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    10943 2023-06-20 07:31:14.000000 collective.contentrules.mailfromfield-1.2.1/collective/contentrules/mailfromfield/tests/test_actions_mailfromfield.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      963 2023-06-20 07:31:14.000000 collective.contentrules.mailfromfield-1.2.1/collective/contentrules/mailfromfield/vocabularies.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-20 07:31:14.760792 collective.contentrules.mailfromfield-1.2.1/collective.contentrules.mailfromfield.egg-info/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     9342 2023-06-20 07:31:14.000000 collective.contentrules.mailfromfield-1.2.1/collective.contentrules.mailfromfield.egg-info/PKG-INFO
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1614 2023-06-20 07:31:14.000000 collective.contentrules.mailfromfield-1.2.1/collective.contentrules.mailfromfield.egg-info/SOURCES.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-06-20 07:31:14.000000 collective.contentrules.mailfromfield-1.2.1/collective.contentrules.mailfromfield.egg-info/dependency_links.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       40 2023-06-20 07:31:14.000000 collective.contentrules.mailfromfield-1.2.1/collective.contentrules.mailfromfield.egg-info/entry_points.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       35 2023-06-20 07:31:14.000000 collective.contentrules.mailfromfield-1.2.1/collective.contentrules.mailfromfield.egg-info/namespace_packages.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-06-20 07:31:14.000000 collective.contentrules.mailfromfield-1.2.1/collective.contentrules.mailfromfield.egg-info/not-zip-safe
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       63 2023-06-20 07:31:14.000000 collective.contentrules.mailfromfield-1.2.1/collective.contentrules.mailfromfield.egg-info/requires.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       11 2023-06-20 07:31:14.000000 collective.contentrules.mailfromfield-1.2.1/collective.contentrules.mailfromfield.egg-info/top_level.txt
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-06-20 07:31:14.760792 collective.contentrules.mailfromfield-1.2.1/docs/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1478 2023-06-20 07:31:14.000000 collective.contentrules.mailfromfield-1.2.1/docs/HISTORY.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1439 2023-06-20 07:31:14.000000 collective.contentrules.mailfromfield-1.2.1/docs/INSTALL.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    17987 2023-06-20 07:31:14.000000 collective.contentrules.mailfromfield-1.2.1/docs/LICENSE.GPL
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      773 2023-06-20 07:31:14.000000 collective.contentrules.mailfromfield-1.2.1/docs/LICENSE.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      518 2023-06-20 07:31:14.760792 collective.contentrules.mailfromfield-1.2.1/setup.cfg
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2140 2023-06-20 07:31:14.000000 collective.contentrules.mailfromfield-1.2.1/setup.py
```

### Comparing `collective.contentrules.mailfromfield-1.2.0/PKG-INFO` & `collective.contentrules.mailfromfield-1.2.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,268 +1,18 @@
 Metadata-Version: 2.1
 Name: collective.contentrules.mailfromfield
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Plone content rule for send e-mail to addresses taken from the content
-Home-page: UNKNOWN
 Author: RedTurtle Technology
 Author-email: sviluppoplone@redturtle.it
 License: GPL
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.contentrules.mailfromfield
 Project-URL: Source, https://github.com/RedTurtle/collective.contentrules.mailfromfield
 Project-URL: Tracker, https://github.com/RedTurtle/collective.contentrules.mailfromfield/issues
-Description: 
-        .. image:: https://img.shields.io/pypi/v/collective.contentrules.mailfromfield.svg
-            :target: https://pypi.org/project/collective.contentrules.mailfromfield/
-            :alt: Latest Version
-        
-        .. image:: https://img.shields.io/pypi/pyversions/collective.contentrules.mailfromfield.svg?style=plastic
-            :target: https://pypi.org/project/collective.contentrules.mailfromfield/
-            :alt: Supported - Python Versions
-        
-        .. image:: https://img.shields.io/pypi/dm/collective.contentrules.mailfromfield.svg
-            :target: https://pypi.org/project/collective.contentrules.mailfromfield/
-            :alt: Number of PyPI downloads
-        
-        .. image:: https://img.shields.io/pypi/l/collective.contentrules.mailfromfield.svg
-            :target: https://pypi.org/project/collective.contentrules.mailfromfield/
-            :alt: License
-        
-        .. image:: https://github.com/RedTurtle/collective.contentrules.mailfromfield/actions/workflows/tests.yml/badge.svg
-            :target: https://github.com/RedTurtle/collective.contentrules.mailfromfield/actions
-            :alt: Tests
-            
-        .. image:: https://coveralls.io/repos/github/RedTurtle/collective.contentrules.mailfromfield/badge.svg?branch=master
-            :target: https://coveralls.io/github/RedTurtle/collective.contentrules.mailfromfield?branch=master
-            :alt: Coverage
-        
-        .. contents::
-        
-        Introduction
-        ============
-        
-        This product will add to Plone a new content rules, someway similar to the default "*Send an email*" ones.
-        The difference is that the email recipient is taken dinamically from a site content, not from a
-        static list of values.
-        
-        In this way the same rule, applied in different places in the site, can send the message to different users.
-        
-        How to use
-        ==========
-        
-        The rules can be enabled globally and locally like every one else, as default Plone feature.
-        In the rule configuration panel you need to fill a set of information:
-        
-        ``Subject``
-            The e-mail subject. You can place inside this text some markers (see below).
-        ``Sender email``
-            The sender of the e-mail. You can leave this empty and automatically use the one from the
-            general mail settings.
-        ``Source field``
-            You must put there the name of the attribute from which you want to retrieve the recipient
-            e-mail. See next section.
-        ``Target element``
-            You need to select if the recipient's e-mail must be taken from:
-        
-            * the container where the rules is activated on
-            * the content who notified the event that started the rule execution
-            * the parent of that content
-        
-            See below for details.
-        ``Mail message``
-            The body text of the e-mail that will be sent. The text is the same for all section where
-            the rule is activated on.
-        
-            You can place inside this text some markers (see below).
-        
-        How it take the email data
-        --------------------------
-        
-        First of all you must choose the *Target element*.
-        
-        If you choose to keep default "*From rule's container*" option address will be read from the section you have
-        activated the rule on.
-        
-        *Example*: if you activated the rule on folder ``/site/section`` and the rule will raise event when
-        working on a document ``/site/section/folder/foo`` the email address will be taken
-        from the folder.
-        
-        Changing to "*From content that triggered the event*" will change the behavior, trying to get email data
-        from the content that raised the event.
-        
-        *Example*: if you activated the rule on a folder ``/site/section`` and the rule  will raise event when
-        working on a document ``/site/section/folder/foo`` the email address will be taken
-        from the ``foo`` document.
-        
-        Finally, if you choose "*From content's parent*", adresses will the taken from the container of the content
-        that triggered the event.
-        
-        *Example*: if you activated the rule on a folder ``/site/section`` and the rule  will raise event when
-        working on a document ``/site/section/folder/foo`` the email address will be taken
-        from ``folder``.
-        
-        What it try to read
-        -------------------
-        
-        The rule try to get from the object:
-        
-        * an attribute of the given name
-        * a callable method from the given name
-        * an Archetypes field with given id
-        * a ZMI property with given id
-        
-        The rule try to read, one after one, all this data. The first match found will be the one used;
-        if not one give results, no e-mail is sent at all.
-        
-        Message interpolation
-        ---------------------
-        
-        Marker labels that follow can be used in the message text and subject.
-        
-        ``${title}``
-            The title of the content that triggered the event (``foo`` title in our example)
-        ``${url}``
-            The URL of the content that triggered the event (``foo`` URL in our example)
-        ``${section_name}``
-            The title of the folder where the rule is activated on (``section`` title in our example)
-        ``${section_url}``
-            The URL of the folder where the rule is activated on (``section`` URL in our example)
-        
-        A real Plone use case
-        ---------------------
-        
-        A Plone site use `Signup Sheet`__ for manage internal training session. The form fieldset is
-        customized as normal, but one of the field is ``director_email``.
-        
-        __ http://plone.org/products/signupsheet
-        
-        We want that this e-mail address is notified when a user subscribe and the user
-        itself put there the e-mail address of the proper director.
-        
-        To reach this we need to:
-        
-        * create a new rule triggered on "*Object added to this container*"
-        * add a filter condition based on content type *Registrant*
-        * add an action using the "*Send email to address taken from the content*"
-        * specify in the action the SignupSheet field with the director email
-        * specify in the action that we want to take the email from the target content
-          (the Registrant itself)
-        
-        TODO
-        ====
-        
-        * why don't support also looking in annotations?
-        * right now the rules check all mail source until one is found with a defined order;
-          maybe is better to leave this choice to the configuration
-        * Dexterity support (probably already there, but needs to be tested)
-        
-        Requirements
-        ============
-        
-        This product has been tested on:
-        
-        * Plone 4.2 with 0.4 version
-        * Plone 4.3 with 0.4 version
-        * Plone 5.0
-        * Plone 5.1
-        
-        Credits
-        =======
-        
-        Developed with the support of `S. Anna Hospital, Ferrara`__; S. Anna Hospital supports the
-        `PloneGov initiative`__.
-        
-        .. image:: http://www.ospfe.it/ospfe-logo.jpg
-           :alt: OspFE logo
-        
-        __ http://www.ospfe.it/
-        __ http://www.plonegov.it/
-        
-        This product was largely developed looking at the source of `collective.contentrules.mailtogroup`__.
-        
-        __ http://plone.org/products/collective.contentrules.mailtogroup
-        
-        Authors
-        =======
-        
-        This product was developed by RedTurtle Technology team.
-        
-        .. image:: http://www.redturtle.it/redturtle_banner.png
-           :alt: RedTurtle Technology Site
-           :target: http://www.redturtle.it/
-        
-        
-        Changelog
-        =========
-        
-        1.2.0 (2023-06-19)
-        ------------------
-        
-        - Change mail send method and allow to eventually add attachments.
-          [cekk]
-        
-        1.1.0 (2023-06-19)
-        ------------------
-        
-        - Plone 6 support
-          [foxtrot-dfm1]
-        
-        1.0.1 (2021-03-10)
-        ------------------
-        
-        - Allow to get to the end of the action execution if no mail is provided.
-          You don't want the page to break if the email is missing. 
-          For the anonymous user this wold be a bad UX
-          [lucabel]
-        
-        
-        1.0.0 (2020-11-23)
-        ------------------
-        
-        - Migrate code to Plone 5/python 3.
-          [lucabel]
-        - Add support for plone.stringinterp.
-          [cekk]
-        
-        0.4.0 (2015-03-13)
-        ------------------
-        
-        Dropped Plone 3 compatibility
-        
-        - Fixed some label that were not i18n compatible
-          [keul]
-        - Fixed wrong documentation mess introduced on version 0.3:
-          the new "parent" option was wrongly descripted
-          [keul]
-        - Updated documentation to reflect changes done in version 0.3
-          [keul]
-        
-        0.3.0 (2014-05-06)
-        ------------------
-        
-        - Fix unicode error while replacing strings [nicolasenno]
-        - Do not fail if a rule is activated on a non-AT content [keul]
-        - Do not try to send mail to empty string recipients [keul]
-        - Refactoring [alert]
-        - Added parent option in the target vocabulary [alert]
-        
-        0.2.0 (2013-05-02)
-        ------------------
-        
-        * lowered logging level to debug
-          [keul]
-        * fixed ruleAction factory
-          [cekk]
-        
-        0.1.0 (2011-10-21)
-        ------------------
-        
-        * Initial release
-        
 Keywords: plone rules mail plonegov
-Platform: UNKNOWN
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone :: 5.2
 Classifier: Framework :: Plone :: 6.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
@@ -271,7 +21,262 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Communications :: Email
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
 Provides-Extra: test
+
+
+.. image:: https://img.shields.io/pypi/v/collective.contentrules.mailfromfield.svg
+    :target: https://pypi.org/project/collective.contentrules.mailfromfield/
+    :alt: Latest Version
+
+.. image:: https://img.shields.io/pypi/pyversions/collective.contentrules.mailfromfield.svg?style=plastic
+    :target: https://pypi.org/project/collective.contentrules.mailfromfield/
+    :alt: Supported - Python Versions
+
+.. image:: https://img.shields.io/pypi/dm/collective.contentrules.mailfromfield.svg
+    :target: https://pypi.org/project/collective.contentrules.mailfromfield/
+    :alt: Number of PyPI downloads
+
+.. image:: https://img.shields.io/pypi/l/collective.contentrules.mailfromfield.svg
+    :target: https://pypi.org/project/collective.contentrules.mailfromfield/
+    :alt: License
+
+.. image:: https://github.com/RedTurtle/collective.contentrules.mailfromfield/actions/workflows/tests.yml/badge.svg
+    :target: https://github.com/RedTurtle/collective.contentrules.mailfromfield/actions
+    :alt: Tests
+    
+.. image:: https://coveralls.io/repos/github/RedTurtle/collective.contentrules.mailfromfield/badge.svg?branch=master
+    :target: https://coveralls.io/github/RedTurtle/collective.contentrules.mailfromfield?branch=master
+    :alt: Coverage
+
+.. contents::
+
+Introduction
+============
+
+This product will add to Plone a new content rules, someway similar to the default "*Send an email*" ones.
+The difference is that the email recipient is taken dinamically from a site content, not from a
+static list of values.
+
+In this way the same rule, applied in different places in the site, can send the message to different users.
+
+How to use
+==========
+
+The rules can be enabled globally and locally like every one else, as default Plone feature.
+In the rule configuration panel you need to fill a set of information:
+
+``Subject``
+    The e-mail subject. You can place inside this text some markers (see below).
+``Sender email``
+    The sender of the e-mail. You can leave this empty and automatically use the one from the
+    general mail settings.
+``Source field``
+    You must put there the name of the attribute from which you want to retrieve the recipient
+    e-mail. See next section.
+``Target element``
+    You need to select if the recipient's e-mail must be taken from:
+
+    * the container where the rules is activated on
+    * the content who notified the event that started the rule execution
+    * the parent of that content
+
+    See below for details.
+``Mail message``
+    The body text of the e-mail that will be sent. The text is the same for all section where
+    the rule is activated on.
+
+    You can place inside this text some markers (see below).
+
+How it take the email data
+--------------------------
+
+First of all you must choose the *Target element*.
+
+If you choose to keep default "*From rule's container*" option address will be read from the section you have
+activated the rule on.
+
+*Example*: if you activated the rule on folder ``/site/section`` and the rule will raise event when
+working on a document ``/site/section/folder/foo`` the email address will be taken
+from the folder.
+
+Changing to "*From content that triggered the event*" will change the behavior, trying to get email data
+from the content that raised the event.
+
+*Example*: if you activated the rule on a folder ``/site/section`` and the rule  will raise event when
+working on a document ``/site/section/folder/foo`` the email address will be taken
+from the ``foo`` document.
+
+Finally, if you choose "*From content's parent*", adresses will the taken from the container of the content
+that triggered the event.
+
+*Example*: if you activated the rule on a folder ``/site/section`` and the rule  will raise event when
+working on a document ``/site/section/folder/foo`` the email address will be taken
+from ``folder``.
+
+What it try to read
+-------------------
+
+The rule try to get from the object:
+
+* an attribute of the given name
+* a callable method from the given name
+* an Archetypes field with given id
+* a ZMI property with given id
+
+The rule try to read, one after one, all this data. The first match found will be the one used;
+if not one give results, no e-mail is sent at all.
+
+Message interpolation
+---------------------
+
+Marker labels that follow can be used in the message text and subject.
+
+``${title}``
+    The title of the content that triggered the event (``foo`` title in our example)
+``${url}``
+    The URL of the content that triggered the event (``foo`` URL in our example)
+``${section_name}``
+    The title of the folder where the rule is activated on (``section`` title in our example)
+``${section_url}``
+    The URL of the folder where the rule is activated on (``section`` URL in our example)
+
+A real Plone use case
+---------------------
+
+A Plone site use `Signup Sheet`__ for manage internal training session. The form fieldset is
+customized as normal, but one of the field is ``director_email``.
+
+__ http://plone.org/products/signupsheet
+
+We want that this e-mail address is notified when a user subscribe and the user
+itself put there the e-mail address of the proper director.
+
+To reach this we need to:
+
+* create a new rule triggered on "*Object added to this container*"
+* add a filter condition based on content type *Registrant*
+* add an action using the "*Send email to address taken from the content*"
+* specify in the action the SignupSheet field with the director email
+* specify in the action that we want to take the email from the target content
+  (the Registrant itself)
+
+TODO
+====
+
+* why don't support also looking in annotations?
+* right now the rules check all mail source until one is found with a defined order;
+  maybe is better to leave this choice to the configuration
+* Dexterity support (probably already there, but needs to be tested)
+
+Requirements
+============
+
+This product has been tested on:
+
+* Plone 4.2 with 0.4 version
+* Plone 4.3 with 0.4 version
+* Plone 5.0
+* Plone 5.1
+
+Credits
+=======
+
+Developed with the support of `S. Anna Hospital, Ferrara`__; S. Anna Hospital supports the
+`PloneGov initiative`__.
+
+.. image:: http://www.ospfe.it/ospfe-logo.jpg
+   :alt: OspFE logo
+
+__ http://www.ospfe.it/
+__ http://www.plonegov.it/
+
+This product was largely developed looking at the source of `collective.contentrules.mailtogroup`__.
+
+__ http://plone.org/products/collective.contentrules.mailtogroup
+
+Authors
+=======
+
+This product was developed by RedTurtle Technology team.
+
+.. image:: http://www.redturtle.it/redturtle_banner.png
+   :alt: RedTurtle Technology Site
+   :target: http://www.redturtle.it/
+
+
+Changelog
+=========
+
+1.2.1 (2023-06-20)
+------------------
+
+- send email on successful transaction commit (#9)
+  [mamico]
+
+
+1.2.0 (2023-06-19)
+------------------
+
+- Change mail send method and allow to eventually add attachments.
+  [cekk]
+
+1.1.0 (2023-06-19)
+------------------
+
+- Plone 6 support
+  [foxtrot-dfm1]
+
+1.0.1 (2021-03-10)
+------------------
+
+- Allow to get to the end of the action execution if no mail is provided.
+  You don't want the page to break if the email is missing. 
+  For the anonymous user this wold be a bad UX
+  [lucabel]
+
+
+1.0.0 (2020-11-23)
+------------------
+
+- Migrate code to Plone 5/python 3.
+  [lucabel]
+- Add support for plone.stringinterp.
+  [cekk]
+
+0.4.0 (2015-03-13)
+------------------
+
+Dropped Plone 3 compatibility
+
+- Fixed some label that were not i18n compatible
+  [keul]
+- Fixed wrong documentation mess introduced on version 0.3:
+  the new "parent" option was wrongly descripted
+  [keul]
+- Updated documentation to reflect changes done in version 0.3
+  [keul]
+
+0.3.0 (2014-05-06)
+------------------
+
+- Fix unicode error while replacing strings [nicolasenno]
+- Do not fail if a rule is activated on a non-AT content [keul]
+- Do not try to send mail to empty string recipients [keul]
+- Refactoring [alert]
+- Added parent option in the target vocabulary [alert]
+
+0.2.0 (2013-05-02)
+------------------
+
+* lowered logging level to debug
+  [keul]
+* fixed ruleAction factory
+  [cekk]
+
+0.1.0 (2011-10-21)
+------------------
+
+* Initial release
```

### Comparing `collective.contentrules.mailfromfield-1.2.0/README.rst` & `collective.contentrules.mailfromfield-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/actions/configure.zcml` & `collective.contentrules.mailfromfield-1.2.1/collective/contentrules/mailfromfield/actions/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/actions/mail.py` & `collective.contentrules.mailfromfield-1.2.1/collective/contentrules/mailfromfield/actions/mail.py`

 * *Files 2% similar despite different names*

```diff
@@ -270,17 +270,15 @@
         msg["Subject"] = subject
         msg["From"] = source
         msg["To"] = ""
 
         self.manage_attachments(msg=msg)
         for email_recipient in recipients:
             msg.replace_header("To", email_recipient)
-            # we set immediate=True because we need to catch exceptions.
-            # by default (False) exceptions are handled by MailHost and we can't catch them.
-            mailhost.send(msg, charset=email_charset, immediate=True)
+            mailhost.send(msg, charset=email_charset)
 
             logger.debug("sending to: %s" % email_recipient)
         return True
 
     def manage_attachments(self, msg):
         """
         Customize this when needed
```

### Comparing `collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/locales/collective.contentrules.mailfromfield.pot` & `collective.contentrules.mailfromfield-1.2.1/collective/contentrules/mailfromfield/locales/collective.contentrules.mailfromfield.pot`

 * *Files identical despite different names*

### Comparing `collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/locales/it/LC_MESSAGES/collective.contentrules.mailfromfield.po` & `collective.contentrules.mailfromfield-1.2.1/collective/contentrules/mailfromfield/locales/it/LC_MESSAGES/collective.contentrules.mailfromfield.po`

 * *Files identical despite different names*

### Comparing `collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/locales/it/LC_MESSAGES/plone.mo` & `collective.contentrules.mailfromfield-1.2.1/collective/contentrules/mailfromfield/locales/it/LC_MESSAGES/plone.po`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,59 @@
-00000000: de12 0495 0000 0000 0300 0000 1c00 0000  ................
-00000010: 3400 0000 0000 0000 4c00 0000 0000 0000  4.......L.......
-00000020: 4c00 0000 4200 0000 4d00 0000 2c00 0000  L...B...M...,...
-00000030: 9000 0000 dd01 0000 bd00 0000 4500 0000  ............E...
-00000040: 9b02 0000 2d00 0000 e102 0000 0053 656e  ....-........Sen
-00000050: 6420 616e 2065 6d61 696c 2c20 7461 6b65  d an email, take
-00000060: 2074 6865 2072 6563 6970 6965 6e74 2066   the recipient f
-00000070: 726f 6d20 6461 7461 206f 6620 7468 6520  rom data of the 
-00000080: 636f 6e74 656e 7420 6974 7365 6c66 2e00  content itself..
-00000090: 5365 6e64 2065 6d61 696c 2074 6f20 6164  Send email to ad
-000000a0: 6472 6573 7320 7461 6b65 6e20 6672 6f6d  dress taken from
-000000b0: 2074 6865 2063 6f6e 7465 6e74 0050 726f   the content.Pro
-000000c0: 6a65 6374 2d49 642d 5665 7273 696f 6e3a  ject-Id-Version:
-000000d0: 2050 4143 4b41 4745 2056 4552 5349 4f4e   PACKAGE VERSION
-000000e0: 0a50 4f54 2d43 7265 6174 696f 6e2d 4461  .POT-Creation-Da
-000000f0: 7465 3a20 3230 3135 2d30 332d 3133 2031  te: 2015-03-13 1
-00000100: 313a 3232 2b30 3030 300a 504f 2d52 6576  1:22+0000.PO-Rev
-00000110: 6973 696f 6e2d 4461 7465 3a20 5945 4152  ision-Date: YEAR
-00000120: 2d4d 4f2d 4441 2048 4f3a 4d49 202b 5a4f  -MO-DA HO:MI +ZO
-00000130: 4e45 0a4c 6173 742d 5472 616e 736c 6174  NE.Last-Translat
-00000140: 6f72 3a20 4c75 6361 2046 6162 6272 6920  or: Luca Fabbri 
-00000150: 3c6b 6575 6c40 7265 6474 7572 746c 652e  <keul@redturtle.
-00000160: 6974 3e0a 4c61 6e67 7561 6765 2d54 6561  it>.Language-Tea
-00000170: 6d3a 2052 6564 5475 7274 6c65 2054 6563  m: RedTurtle Tec
-00000180: 686e 6f6c 6f67 7920 3c73 7669 6c75 7070  hnology <svilupp
-00000190: 6f70 6c6f 6e65 4072 6564 7475 7274 6c65  oplone@redturtle
-000001a0: 2e69 743e 0a4d 494d 452d 5665 7273 696f  .it>.MIME-Versio
-000001b0: 6e3a 2031 2e30 0a43 6f6e 7465 6e74 2d54  n: 1.0.Content-T
-000001c0: 7970 653a 2074 6578 742f 706c 6169 6e3b  ype: text/plain;
-000001d0: 2063 6861 7273 6574 3d75 7466 2d38 0a43   charset=utf-8.C
-000001e0: 6f6e 7465 6e74 2d54 7261 6e73 6665 722d  ontent-Transfer-
-000001f0: 456e 636f 6469 6e67 3a20 3862 6974 0a50  Encoding: 8bit.P
-00000200: 6c75 7261 6c2d 466f 726d 733a 206e 706c  lural-Forms: npl
-00000210: 7572 616c 733d 313b 2070 6c75 7261 6c3d  urals=1; plural=
-00000220: 300a 4c61 6e67 7561 6765 2d43 6f64 653a  0.Language-Code:
-00000230: 2069 740a 4c61 6e67 7561 6765 2d4e 616d   it.Language-Nam
-00000240: 653a 2049 7461 6c69 616e 0a50 7265 6665  e: Italian.Prefe
-00000250: 7272 6564 2d45 6e63 6f64 696e 6773 3a20  rred-Encodings: 
-00000260: 7574 662d 3820 6c61 7469 6e31 0a44 6f6d  utf-8 latin1.Dom
-00000270: 6169 6e3a 2070 6c6f 6e65 0a58 2d49 732d  ain: plone.X-Is-
-00000280: 4661 6c6c 6261 636b 2d46 6f72 3a20 6974  Fallback-For: it
-00000290: 2d63 6820 6974 2d69 740a 0049 6e76 6961  -ch it-it..Invia
-000002a0: 2075 6e61 2065 2d6d 6169 6c2c 2070 7265   una e-mail, pre
-000002b0: 6e64 6920 6920 6465 7374 696e 6174 6172  ndi i destinatar
-000002c0: 6920 6461 6920 6461 7469 2064 656c 2063  i dai dati del c
-000002d0: 6f6e 7465 6e75 746f 2073 7465 7373 6f2e  ontenuto stesso.
-000002e0: 0049 6e76 6961 2065 2d6d 6169 6c20 6164  .Invia e-mail ad
-000002f0: 2069 6e64 6972 697a 7a69 2070 7265 7369   indirizzi presi
-00000300: 2064 616c 2063 6f6e 7465 6e75 746f 00     dal contenuto.
+00000000: 2320 2d2d 2d20 504c 4541 5345 2045 4449  # --- PLEASE EDI
+00000010: 5420 5448 4520 4c49 4e45 5320 4245 4c4f  T THE LINES BELO
+00000020: 5720 434f 5252 4543 544c 5920 2d2d 2d0a  W CORRECTLY ---.
+00000030: 2320 534f 4d45 2044 4553 4352 4950 5449  # SOME DESCRIPTI
+00000040: 5645 2054 4954 4c45 2e0a 2320 4649 5253  VE TITLE..# FIRS
+00000050: 5420 4155 5448 4f52 203c 454d 4149 4c40  T AUTHOR <EMAIL@
+00000060: 4144 4452 4553 533e 2c20 5945 4152 2e0a  ADDRESS>, YEAR..
+00000070: 6d73 6769 6420 2222 0a6d 7367 7374 7220  msgid "".msgstr 
+00000080: 2222 0a22 5072 6f6a 6563 742d 4964 2d56  ""."Project-Id-V
+00000090: 6572 7369 6f6e 3a20 5041 434b 4147 4520  ersion: PACKAGE 
+000000a0: 5645 5253 494f 4e5c 6e22 0a22 504f 542d  VERSION\n"."POT-
+000000b0: 4372 6561 7469 6f6e 2d44 6174 653a 2032  Creation-Date: 2
+000000c0: 3031 352d 3033 2d31 3320 3131 3a32 322b  015-03-13 11:22+
+000000d0: 3030 3030 5c6e 220a 2250 4f2d 5265 7669  0000\n"."PO-Revi
+000000e0: 7369 6f6e 2d44 6174 653a 2059 4541 522d  sion-Date: YEAR-
+000000f0: 4d4f 2d44 4120 484f 3a4d 4920 2b5a 4f4e  MO-DA HO:MI +ZON
+00000100: 455c 6e22 0a22 4c61 7374 2d54 7261 6e73  E\n"."Last-Trans
+00000110: 6c61 746f 723a 204c 7563 6120 4661 6262  lator: Luca Fabb
+00000120: 7269 203c 6b65 756c 4072 6564 7475 7274  ri <keul@redturt
+00000130: 6c65 2e69 743e 5c6e 220a 224c 616e 6775  le.it>\n"."Langu
+00000140: 6167 652d 5465 616d 3a20 5265 6454 7572  age-Team: RedTur
+00000150: 746c 6520 5465 6368 6e6f 6c6f 6779 203c  tle Technology <
+00000160: 7376 696c 7570 706f 706c 6f6e 6540 7265  sviluppoplone@re
+00000170: 6474 7572 746c 652e 6974 3e5c 6e22 0a22  dturtle.it>\n"."
+00000180: 4d49 4d45 2d56 6572 7369 6f6e 3a20 312e  MIME-Version: 1.
+00000190: 305c 6e22 0a22 436f 6e74 656e 742d 5479  0\n"."Content-Ty
+000001a0: 7065 3a20 7465 7874 2f70 6c61 696e 3b20  pe: text/plain; 
+000001b0: 6368 6172 7365 743d 7574 662d 385c 6e22  charset=utf-8\n"
+000001c0: 0a22 436f 6e74 656e 742d 5472 616e 7366  ."Content-Transf
+000001d0: 6572 2d45 6e63 6f64 696e 673a 2038 6269  er-Encoding: 8bi
+000001e0: 745c 6e22 0a22 506c 7572 616c 2d46 6f72  t\n"."Plural-For
+000001f0: 6d73 3a20 6e70 6c75 7261 6c73 3d31 3b20  ms: nplurals=1; 
+00000200: 706c 7572 616c 3d30 5c6e 220a 224c 616e  plural=0\n"."Lan
+00000210: 6775 6167 652d 436f 6465 3a20 6974 5c6e  guage-Code: it\n
+00000220: 220a 224c 616e 6775 6167 652d 4e61 6d65  "."Language-Name
+00000230: 3a20 4974 616c 6961 6e5c 6e22 0a22 5072  : Italian\n"."Pr
+00000240: 6566 6572 7265 642d 456e 636f 6469 6e67  eferred-Encoding
+00000250: 733a 2075 7466 2d38 206c 6174 696e 315c  s: utf-8 latin1\
+00000260: 6e22 0a22 446f 6d61 696e 3a20 706c 6f6e  n"."Domain: plon
+00000270: 655c 6e22 0a22 582d 4973 2d46 616c 6c62  e\n"."X-Is-Fallb
+00000280: 6163 6b2d 466f 723a 2069 742d 6368 2069  ack-For: it-ch i
+00000290: 742d 6974 5c6e 220a 0a6d 7367 6964 2022  t-it\n"..msgid "
+000002a0: 5365 6e64 2061 6e20 656d 6169 6c2c 2074  Send an email, t
+000002b0: 616b 6520 7468 6520 7265 6369 7069 656e  ake the recipien
+000002c0: 7420 6672 6f6d 2064 6174 6120 6f66 2074  t from data of t
+000002d0: 6865 2063 6f6e 7465 6e74 2069 7473 656c  he content itsel
+000002e0: 662e 220a 6d73 6773 7472 2022 496e 7669  f.".msgstr "Invi
+000002f0: 6120 756e 6120 652d 6d61 696c 2c20 7072  a una e-mail, pr
+00000300: 656e 6469 2069 2064 6573 7469 6e61 7461  endi i destinata
+00000310: 7269 2064 6169 2064 6174 6920 6465 6c20  ri dai dati del 
+00000320: 636f 6e74 656e 7574 6f20 7374 6573 736f  contenuto stesso
+00000330: 2e22 0a0a 6d73 6769 6420 2253 656e 6420  ."..msgid "Send 
+00000340: 656d 6169 6c20 746f 2061 6464 7265 7373  email to address
+00000350: 2074 616b 656e 2066 726f 6d20 7468 6520   taken from the 
+00000360: 636f 6e74 656e 7422 0a6d 7367 7374 7220  content".msgstr 
+00000370: 2249 6e76 6961 2065 2d6d 6169 6c20 6164  "Invia e-mail ad
+00000380: 2069 6e64 6972 697a 7a69 2070 7265 7369   indirizzi presi
+00000390: 2064 616c 2063 6f6e 7465 6e75 746f 220a   dal contenuto".
+000003a0: 0a                                       .
```

### Comparing `collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/locales/it/LC_MESSAGES/plone.po` & `collective.contentrules.mailfromfield-1.2.1/collective/contentrules/mailfromfield/locales/plone-manual.pot`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 # --- PLEASE EDIT THE LINES BELOW CORRECTLY ---
 # SOME DESCRIPTIVE TITLE.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2015-03-13 11:22+0000\n"
+"POT-Creation-Date: 2011-10-20 08:09+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
-"Last-Translator: Luca Fabbri <keul@redturtle.it>\n"
-"Language-Team: RedTurtle Technology <sviluppoplone@redturtle.it>\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0\n"
-"Language-Code: it\n"
-"Language-Name: Italian\n"
+"Language-Code: en\n"
+"Language-Name: English\n"
 "Preferred-Encodings: utf-8 latin1\n"
 "Domain: plone\n"
-"X-Is-Fallback-For: it-ch it-it\n"
-
-msgid "Send an email, take the recipient from data of the content itself."
-msgstr "Invia una e-mail, prendi i destinatari dai dati del contenuto stesso."
 
 msgid "Send email to address taken from the content"
-msgstr "Invia e-mail ad indirizzi presi dal contenuto"
+msgstr ""
 
+msgid "Send an email, take the recipient from data of the content itself."
+msgstr ""
```

### Comparing `collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/locales/plone-manual.pot` & `collective.contentrules.mailfromfield-1.2.1/collective/contentrules/mailfromfield/locales/plone.pot`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # --- PLEASE EDIT THE LINES BELOW CORRECTLY ---
 # SOME DESCRIPTIVE TITLE.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"POT-Creation-Date: 2011-10-20 08:09+0000\n"
+"POT-Creation-Date: 2015-03-13 11:22+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0\n"
 "Language-Code: en\n"
 "Language-Name: English\n"
 "Preferred-Encodings: utf-8 latin1\n"
 "Domain: plone\n"
 
-msgid "Send email to address taken from the content"
+msgid "Send an email, take the recipient from data of the content itself."
 msgstr ""
 
-msgid "Send an email, take the recipient from data of the content itself."
+msgid "Send email to address taken from the content"
 msgstr ""
+
```

### Comparing `collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/testing.py` & `collective.contentrules.mailfromfield-1.2.1/collective/contentrules/mailfromfield/testing.py`

 * *Files identical despite different names*

### Comparing `collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/tests/test_actions_mailfromfield.py` & `collective.contentrules.mailfromfield-1.2.1/collective/contentrules/mailfromfield/tests/test_actions_mailfromfield.py`

 * *Files identical despite different names*

### Comparing `collective.contentrules.mailfromfield-1.2.0/collective/contentrules/mailfromfield/vocabularies.py` & `collective.contentrules.mailfromfield-1.2.1/collective/contentrules/mailfromfield/vocabularies.py`

 * *Files identical despite different names*

### Comparing `collective.contentrules.mailfromfield-1.2.0/collective.contentrules.mailfromfield.egg-info/PKG-INFO` & `collective.contentrules.mailfromfield-1.2.1/collective.contentrules.mailfromfield.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,268 +1,18 @@
 Metadata-Version: 2.1
 Name: collective.contentrules.mailfromfield
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Plone content rule for send e-mail to addresses taken from the content
-Home-page: UNKNOWN
 Author: RedTurtle Technology
 Author-email: sviluppoplone@redturtle.it
 License: GPL
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.contentrules.mailfromfield
 Project-URL: Source, https://github.com/RedTurtle/collective.contentrules.mailfromfield
 Project-URL: Tracker, https://github.com/RedTurtle/collective.contentrules.mailfromfield/issues
-Description: 
-        .. image:: https://img.shields.io/pypi/v/collective.contentrules.mailfromfield.svg
-            :target: https://pypi.org/project/collective.contentrules.mailfromfield/
-            :alt: Latest Version
-        
-        .. image:: https://img.shields.io/pypi/pyversions/collective.contentrules.mailfromfield.svg?style=plastic
-            :target: https://pypi.org/project/collective.contentrules.mailfromfield/
-            :alt: Supported - Python Versions
-        
-        .. image:: https://img.shields.io/pypi/dm/collective.contentrules.mailfromfield.svg
-            :target: https://pypi.org/project/collective.contentrules.mailfromfield/
-            :alt: Number of PyPI downloads
-        
-        .. image:: https://img.shields.io/pypi/l/collective.contentrules.mailfromfield.svg
-            :target: https://pypi.org/project/collective.contentrules.mailfromfield/
-            :alt: License
-        
-        .. image:: https://github.com/RedTurtle/collective.contentrules.mailfromfield/actions/workflows/tests.yml/badge.svg
-            :target: https://github.com/RedTurtle/collective.contentrules.mailfromfield/actions
-            :alt: Tests
-            
-        .. image:: https://coveralls.io/repos/github/RedTurtle/collective.contentrules.mailfromfield/badge.svg?branch=master
-            :target: https://coveralls.io/github/RedTurtle/collective.contentrules.mailfromfield?branch=master
-            :alt: Coverage
-        
-        .. contents::
-        
-        Introduction
-        ============
-        
-        This product will add to Plone a new content rules, someway similar to the default "*Send an email*" ones.
-        The difference is that the email recipient is taken dinamically from a site content, not from a
-        static list of values.
-        
-        In this way the same rule, applied in different places in the site, can send the message to different users.
-        
-        How to use
-        ==========
-        
-        The rules can be enabled globally and locally like every one else, as default Plone feature.
-        In the rule configuration panel you need to fill a set of information:
-        
-        ``Subject``
-            The e-mail subject. You can place inside this text some markers (see below).
-        ``Sender email``
-            The sender of the e-mail. You can leave this empty and automatically use the one from the
-            general mail settings.
-        ``Source field``
-            You must put there the name of the attribute from which you want to retrieve the recipient
-            e-mail. See next section.
-        ``Target element``
-            You need to select if the recipient's e-mail must be taken from:
-        
-            * the container where the rules is activated on
-            * the content who notified the event that started the rule execution
-            * the parent of that content
-        
-            See below for details.
-        ``Mail message``
-            The body text of the e-mail that will be sent. The text is the same for all section where
-            the rule is activated on.
-        
-            You can place inside this text some markers (see below).
-        
-        How it take the email data
-        --------------------------
-        
-        First of all you must choose the *Target element*.
-        
-        If you choose to keep default "*From rule's container*" option address will be read from the section you have
-        activated the rule on.
-        
-        *Example*: if you activated the rule on folder ``/site/section`` and the rule will raise event when
-        working on a document ``/site/section/folder/foo`` the email address will be taken
-        from the folder.
-        
-        Changing to "*From content that triggered the event*" will change the behavior, trying to get email data
-        from the content that raised the event.
-        
-        *Example*: if you activated the rule on a folder ``/site/section`` and the rule  will raise event when
-        working on a document ``/site/section/folder/foo`` the email address will be taken
-        from the ``foo`` document.
-        
-        Finally, if you choose "*From content's parent*", adresses will the taken from the container of the content
-        that triggered the event.
-        
-        *Example*: if you activated the rule on a folder ``/site/section`` and the rule  will raise event when
-        working on a document ``/site/section/folder/foo`` the email address will be taken
-        from ``folder``.
-        
-        What it try to read
-        -------------------
-        
-        The rule try to get from the object:
-        
-        * an attribute of the given name
-        * a callable method from the given name
-        * an Archetypes field with given id
-        * a ZMI property with given id
-        
-        The rule try to read, one after one, all this data. The first match found will be the one used;
-        if not one give results, no e-mail is sent at all.
-        
-        Message interpolation
-        ---------------------
-        
-        Marker labels that follow can be used in the message text and subject.
-        
-        ``${title}``
-            The title of the content that triggered the event (``foo`` title in our example)
-        ``${url}``
-            The URL of the content that triggered the event (``foo`` URL in our example)
-        ``${section_name}``
-            The title of the folder where the rule is activated on (``section`` title in our example)
-        ``${section_url}``
-            The URL of the folder where the rule is activated on (``section`` URL in our example)
-        
-        A real Plone use case
-        ---------------------
-        
-        A Plone site use `Signup Sheet`__ for manage internal training session. The form fieldset is
-        customized as normal, but one of the field is ``director_email``.
-        
-        __ http://plone.org/products/signupsheet
-        
-        We want that this e-mail address is notified when a user subscribe and the user
-        itself put there the e-mail address of the proper director.
-        
-        To reach this we need to:
-        
-        * create a new rule triggered on "*Object added to this container*"
-        * add a filter condition based on content type *Registrant*
-        * add an action using the "*Send email to address taken from the content*"
-        * specify in the action the SignupSheet field with the director email
-        * specify in the action that we want to take the email from the target content
-          (the Registrant itself)
-        
-        TODO
-        ====
-        
-        * why don't support also looking in annotations?
-        * right now the rules check all mail source until one is found with a defined order;
-          maybe is better to leave this choice to the configuration
-        * Dexterity support (probably already there, but needs to be tested)
-        
-        Requirements
-        ============
-        
-        This product has been tested on:
-        
-        * Plone 4.2 with 0.4 version
-        * Plone 4.3 with 0.4 version
-        * Plone 5.0
-        * Plone 5.1
-        
-        Credits
-        =======
-        
-        Developed with the support of `S. Anna Hospital, Ferrara`__; S. Anna Hospital supports the
-        `PloneGov initiative`__.
-        
-        .. image:: http://www.ospfe.it/ospfe-logo.jpg
-           :alt: OspFE logo
-        
-        __ http://www.ospfe.it/
-        __ http://www.plonegov.it/
-        
-        This product was largely developed looking at the source of `collective.contentrules.mailtogroup`__.
-        
-        __ http://plone.org/products/collective.contentrules.mailtogroup
-        
-        Authors
-        =======
-        
-        This product was developed by RedTurtle Technology team.
-        
-        .. image:: http://www.redturtle.it/redturtle_banner.png
-           :alt: RedTurtle Technology Site
-           :target: http://www.redturtle.it/
-        
-        
-        Changelog
-        =========
-        
-        1.2.0 (2023-06-19)
-        ------------------
-        
-        - Change mail send method and allow to eventually add attachments.
-          [cekk]
-        
-        1.1.0 (2023-06-19)
-        ------------------
-        
-        - Plone 6 support
-          [foxtrot-dfm1]
-        
-        1.0.1 (2021-03-10)
-        ------------------
-        
-        - Allow to get to the end of the action execution if no mail is provided.
-          You don't want the page to break if the email is missing. 
-          For the anonymous user this wold be a bad UX
-          [lucabel]
-        
-        
-        1.0.0 (2020-11-23)
-        ------------------
-        
-        - Migrate code to Plone 5/python 3.
-          [lucabel]
-        - Add support for plone.stringinterp.
-          [cekk]
-        
-        0.4.0 (2015-03-13)
-        ------------------
-        
-        Dropped Plone 3 compatibility
-        
-        - Fixed some label that were not i18n compatible
-          [keul]
-        - Fixed wrong documentation mess introduced on version 0.3:
-          the new "parent" option was wrongly descripted
-          [keul]
-        - Updated documentation to reflect changes done in version 0.3
-          [keul]
-        
-        0.3.0 (2014-05-06)
-        ------------------
-        
-        - Fix unicode error while replacing strings [nicolasenno]
-        - Do not fail if a rule is activated on a non-AT content [keul]
-        - Do not try to send mail to empty string recipients [keul]
-        - Refactoring [alert]
-        - Added parent option in the target vocabulary [alert]
-        
-        0.2.0 (2013-05-02)
-        ------------------
-        
-        * lowered logging level to debug
-          [keul]
-        * fixed ruleAction factory
-          [cekk]
-        
-        0.1.0 (2011-10-21)
-        ------------------
-        
-        * Initial release
-        
 Keywords: plone rules mail plonegov
-Platform: UNKNOWN
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone :: 5.2
 Classifier: Framework :: Plone :: 6.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
@@ -271,7 +21,262 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Communications :: Email
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
 Provides-Extra: test
+
+
+.. image:: https://img.shields.io/pypi/v/collective.contentrules.mailfromfield.svg
+    :target: https://pypi.org/project/collective.contentrules.mailfromfield/
+    :alt: Latest Version
+
+.. image:: https://img.shields.io/pypi/pyversions/collective.contentrules.mailfromfield.svg?style=plastic
+    :target: https://pypi.org/project/collective.contentrules.mailfromfield/
+    :alt: Supported - Python Versions
+
+.. image:: https://img.shields.io/pypi/dm/collective.contentrules.mailfromfield.svg
+    :target: https://pypi.org/project/collective.contentrules.mailfromfield/
+    :alt: Number of PyPI downloads
+
+.. image:: https://img.shields.io/pypi/l/collective.contentrules.mailfromfield.svg
+    :target: https://pypi.org/project/collective.contentrules.mailfromfield/
+    :alt: License
+
+.. image:: https://github.com/RedTurtle/collective.contentrules.mailfromfield/actions/workflows/tests.yml/badge.svg
+    :target: https://github.com/RedTurtle/collective.contentrules.mailfromfield/actions
+    :alt: Tests
+    
+.. image:: https://coveralls.io/repos/github/RedTurtle/collective.contentrules.mailfromfield/badge.svg?branch=master
+    :target: https://coveralls.io/github/RedTurtle/collective.contentrules.mailfromfield?branch=master
+    :alt: Coverage
+
+.. contents::
+
+Introduction
+============
+
+This product will add to Plone a new content rules, someway similar to the default "*Send an email*" ones.
+The difference is that the email recipient is taken dinamically from a site content, not from a
+static list of values.
+
+In this way the same rule, applied in different places in the site, can send the message to different users.
+
+How to use
+==========
+
+The rules can be enabled globally and locally like every one else, as default Plone feature.
+In the rule configuration panel you need to fill a set of information:
+
+``Subject``
+    The e-mail subject. You can place inside this text some markers (see below).
+``Sender email``
+    The sender of the e-mail. You can leave this empty and automatically use the one from the
+    general mail settings.
+``Source field``
+    You must put there the name of the attribute from which you want to retrieve the recipient
+    e-mail. See next section.
+``Target element``
+    You need to select if the recipient's e-mail must be taken from:
+
+    * the container where the rules is activated on
+    * the content who notified the event that started the rule execution
+    * the parent of that content
+
+    See below for details.
+``Mail message``
+    The body text of the e-mail that will be sent. The text is the same for all section where
+    the rule is activated on.
+
+    You can place inside this text some markers (see below).
+
+How it take the email data
+--------------------------
+
+First of all you must choose the *Target element*.
+
+If you choose to keep default "*From rule's container*" option address will be read from the section you have
+activated the rule on.
+
+*Example*: if you activated the rule on folder ``/site/section`` and the rule will raise event when
+working on a document ``/site/section/folder/foo`` the email address will be taken
+from the folder.
+
+Changing to "*From content that triggered the event*" will change the behavior, trying to get email data
+from the content that raised the event.
+
+*Example*: if you activated the rule on a folder ``/site/section`` and the rule  will raise event when
+working on a document ``/site/section/folder/foo`` the email address will be taken
+from the ``foo`` document.
+
+Finally, if you choose "*From content's parent*", adresses will the taken from the container of the content
+that triggered the event.
+
+*Example*: if you activated the rule on a folder ``/site/section`` and the rule  will raise event when
+working on a document ``/site/section/folder/foo`` the email address will be taken
+from ``folder``.
+
+What it try to read
+-------------------
+
+The rule try to get from the object:
+
+* an attribute of the given name
+* a callable method from the given name
+* an Archetypes field with given id
+* a ZMI property with given id
+
+The rule try to read, one after one, all this data. The first match found will be the one used;
+if not one give results, no e-mail is sent at all.
+
+Message interpolation
+---------------------
+
+Marker labels that follow can be used in the message text and subject.
+
+``${title}``
+    The title of the content that triggered the event (``foo`` title in our example)
+``${url}``
+    The URL of the content that triggered the event (``foo`` URL in our example)
+``${section_name}``
+    The title of the folder where the rule is activated on (``section`` title in our example)
+``${section_url}``
+    The URL of the folder where the rule is activated on (``section`` URL in our example)
+
+A real Plone use case
+---------------------
+
+A Plone site use `Signup Sheet`__ for manage internal training session. The form fieldset is
+customized as normal, but one of the field is ``director_email``.
+
+__ http://plone.org/products/signupsheet
+
+We want that this e-mail address is notified when a user subscribe and the user
+itself put there the e-mail address of the proper director.
+
+To reach this we need to:
+
+* create a new rule triggered on "*Object added to this container*"
+* add a filter condition based on content type *Registrant*
+* add an action using the "*Send email to address taken from the content*"
+* specify in the action the SignupSheet field with the director email
+* specify in the action that we want to take the email from the target content
+  (the Registrant itself)
+
+TODO
+====
+
+* why don't support also looking in annotations?
+* right now the rules check all mail source until one is found with a defined order;
+  maybe is better to leave this choice to the configuration
+* Dexterity support (probably already there, but needs to be tested)
+
+Requirements
+============
+
+This product has been tested on:
+
+* Plone 4.2 with 0.4 version
+* Plone 4.3 with 0.4 version
+* Plone 5.0
+* Plone 5.1
+
+Credits
+=======
+
+Developed with the support of `S. Anna Hospital, Ferrara`__; S. Anna Hospital supports the
+`PloneGov initiative`__.
+
+.. image:: http://www.ospfe.it/ospfe-logo.jpg
+   :alt: OspFE logo
+
+__ http://www.ospfe.it/
+__ http://www.plonegov.it/
+
+This product was largely developed looking at the source of `collective.contentrules.mailtogroup`__.
+
+__ http://plone.org/products/collective.contentrules.mailtogroup
+
+Authors
+=======
+
+This product was developed by RedTurtle Technology team.
+
+.. image:: http://www.redturtle.it/redturtle_banner.png
+   :alt: RedTurtle Technology Site
+   :target: http://www.redturtle.it/
+
+
+Changelog
+=========
+
+1.2.1 (2023-06-20)
+------------------
+
+- send email on successful transaction commit (#9)
+  [mamico]
+
+
+1.2.0 (2023-06-19)
+------------------
+
+- Change mail send method and allow to eventually add attachments.
+  [cekk]
+
+1.1.0 (2023-06-19)
+------------------
+
+- Plone 6 support
+  [foxtrot-dfm1]
+
+1.0.1 (2021-03-10)
+------------------
+
+- Allow to get to the end of the action execution if no mail is provided.
+  You don't want the page to break if the email is missing. 
+  For the anonymous user this wold be a bad UX
+  [lucabel]
+
+
+1.0.0 (2020-11-23)
+------------------
+
+- Migrate code to Plone 5/python 3.
+  [lucabel]
+- Add support for plone.stringinterp.
+  [cekk]
+
+0.4.0 (2015-03-13)
+------------------
+
+Dropped Plone 3 compatibility
+
+- Fixed some label that were not i18n compatible
+  [keul]
+- Fixed wrong documentation mess introduced on version 0.3:
+  the new "parent" option was wrongly descripted
+  [keul]
+- Updated documentation to reflect changes done in version 0.3
+  [keul]
+
+0.3.0 (2014-05-06)
+------------------
+
+- Fix unicode error while replacing strings [nicolasenno]
+- Do not fail if a rule is activated on a non-AT content [keul]
+- Do not try to send mail to empty string recipients [keul]
+- Refactoring [alert]
+- Added parent option in the target vocabulary [alert]
+
+0.2.0 (2013-05-02)
+------------------
+
+* lowered logging level to debug
+  [keul]
+* fixed ruleAction factory
+  [cekk]
+
+0.1.0 (2011-10-21)
+------------------
+
+* Initial release
```

### Comparing `collective.contentrules.mailfromfield-1.2.0/collective.contentrules.mailfromfield.egg-info/SOURCES.txt` & `collective.contentrules.mailfromfield-1.2.1/collective.contentrules.mailfromfield.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -19,17 +19,15 @@
 collective/contentrules/mailfromfield/actions/__init__.py
 collective/contentrules/mailfromfield/actions/configure.zcml
 collective/contentrules/mailfromfield/actions/mail.py
 collective/contentrules/mailfromfield/locales/collective.contentrules.mailfromfield.pot
 collective/contentrules/mailfromfield/locales/plone-manual.pot
 collective/contentrules/mailfromfield/locales/plone.pot
 collective/contentrules/mailfromfield/locales/rebuildAll.sh
-collective/contentrules/mailfromfield/locales/it/LC_MESSAGES/collective.contentrules.mailfromfield.mo
 collective/contentrules/mailfromfield/locales/it/LC_MESSAGES/collective.contentrules.mailfromfield.po
-collective/contentrules/mailfromfield/locales/it/LC_MESSAGES/plone.mo
 collective/contentrules/mailfromfield/locales/it/LC_MESSAGES/plone.po
 collective/contentrules/mailfromfield/tests/__init__.py
 collective/contentrules/mailfromfield/tests/test_actions_mailfromfield.py
 docs/HISTORY.rst
 docs/INSTALL.txt
 docs/LICENSE.GPL
 docs/LICENSE.txt
```

### Comparing `collective.contentrules.mailfromfield-1.2.0/docs/HISTORY.rst` & `collective.contentrules.mailfromfield-1.2.1/docs/HISTORY.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+1.2.1 (2023-06-20)
+------------------
+
+- send email on successful transaction commit (#9)
+  [mamico]
+
+
 1.2.0 (2023-06-19)
 ------------------
 
 - Change mail send method and allow to eventually add attachments.
   [cekk]
 
 1.1.0 (2023-06-19)
```

### Comparing `collective.contentrules.mailfromfield-1.2.0/docs/INSTALL.txt` & `collective.contentrules.mailfromfield-1.2.1/docs/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `collective.contentrules.mailfromfield-1.2.0/docs/LICENSE.GPL` & `collective.contentrules.mailfromfield-1.2.1/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.contentrules.mailfromfield-1.2.0/docs/LICENSE.txt` & `collective.contentrules.mailfromfield-1.2.1/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `collective.contentrules.mailfromfield-1.2.0/setup.cfg` & `collective.contentrules.mailfromfield-1.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `collective.contentrules.mailfromfield-1.2.0/setup.py` & `collective.contentrules.mailfromfield-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import os
 
-version = "1.2.0"
+version = "1.2.1"
 
 tests_require = ["plone.app.robotframework"]
 
 setup(
     name="collective.contentrules.mailfromfield",
     version=version,
     description="A Plone content rule for send e-mail to addresses taken from the content",
```

