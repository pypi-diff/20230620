# Comparing `tmp/localstripe-1.9.0.tar.gz` & `tmp/localstripe-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/localstripe-1.9.0.tar", last modified: Wed Aug 21 08:56:26 2019, max compression
+gzip compressed data, was "dist/localstripe-1.9.1.tar", last modified: Mon Aug 26 13:51:54 2019, max compression
```

## Comparing `localstripe-1.9.0.tar` & `localstripe-1.9.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2019-08-21 08:56:26.000000 localstripe-1.9.0/
--rw-rw-r--   0 adrien    (1000) adrien    (1000)      300 2019-08-21 08:56:26.000000 localstripe-1.9.0/PKG-INFO
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     6625 2019-08-02 07:05:05.000000 localstripe-1.9.0/README.rst
-drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2019-08-21 08:56:26.000000 localstripe-1.9.0/localstripe/
--rw-rw-r--   0 adrien    (1000) adrien    (1000)      843 2019-08-21 08:56:24.000000 localstripe-1.9.0/localstripe/__init__.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)      761 2018-03-19 15:38:10.000000 localstripe-1.9.0/localstripe/__main__.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     1326 2018-03-19 16:00:49.000000 localstripe-1.9.0/localstripe/errors.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)    10758 2019-07-30 13:46:18.000000 localstripe-1.9.0/localstripe/localstripe-v3.js
--rw-rw-r--   0 adrien    (1000) adrien    (1000)    87671 2019-08-21 08:56:24.000000 localstripe-1.9.0/localstripe/resources.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)    10615 2019-07-30 13:45:14.000000 localstripe-1.9.0/localstripe/server.py
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     2516 2018-12-09 17:29:49.000000 localstripe-1.9.0/localstripe/webhooks.py
-drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2019-08-21 08:56:26.000000 localstripe-1.9.0/localstripe.egg-info/
--rw-rw-r--   0 adrien    (1000) adrien    (1000)      300 2019-08-21 08:56:26.000000 localstripe-1.9.0/localstripe.egg-info/PKG-INFO
--rw-rw-r--   0 adrien    (1000) adrien    (1000)      412 2019-08-21 08:56:26.000000 localstripe-1.9.0/localstripe.egg-info/SOURCES.txt
--rw-rw-r--   0 adrien    (1000) adrien    (1000)        1 2019-08-21 08:56:26.000000 localstripe-1.9.0/localstripe.egg-info/dependency_links.txt
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       58 2019-08-21 08:56:26.000000 localstripe-1.9.0/localstripe.egg-info/entry_points.txt
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       38 2019-08-21 08:56:26.000000 localstripe-1.9.0/localstripe.egg-info/requires.txt
--rw-rw-r--   0 adrien    (1000) adrien    (1000)       12 2019-08-21 08:56:26.000000 localstripe-1.9.0/localstripe.egg-info/top_level.txt
--rw-rw-r--   0 adrien    (1000) adrien    (1000)      113 2019-08-21 08:56:26.000000 localstripe-1.9.0/setup.cfg
--rw-rw-r--   0 adrien    (1000) adrien    (1000)     1323 2019-07-12 11:10:14.000000 localstripe-1.9.0/setup.py
+drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2019-08-26 13:51:54.000000 localstripe-1.9.1/
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)      300 2019-08-26 13:51:54.000000 localstripe-1.9.1/PKG-INFO
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     6625 2019-07-29 07:46:22.000000 localstripe-1.9.1/README.rst
+drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2019-08-26 13:51:54.000000 localstripe-1.9.1/localstripe/
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)      843 2019-08-26 13:51:16.000000 localstripe-1.9.1/localstripe/__init__.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)      761 2018-03-20 09:03:27.000000 localstripe-1.9.1/localstripe/__main__.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     1326 2018-03-20 09:03:27.000000 localstripe-1.9.1/localstripe/errors.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)    10758 2019-07-31 07:30:44.000000 localstripe-1.9.1/localstripe/localstripe-v3.js
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)    87753 2019-08-26 13:51:01.000000 localstripe-1.9.1/localstripe/resources.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)    10615 2019-07-31 07:30:44.000000 localstripe-1.9.1/localstripe/server.py
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     2516 2018-12-13 08:39:46.000000 localstripe-1.9.1/localstripe/webhooks.py
+drwxrwxr-x   0 adrien    (1000) adrien    (1000)        0 2019-08-26 13:51:54.000000 localstripe-1.9.1/localstripe.egg-info/
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)      300 2019-08-26 13:51:54.000000 localstripe-1.9.1/localstripe.egg-info/PKG-INFO
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)      412 2019-08-26 13:51:54.000000 localstripe-1.9.1/localstripe.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)        1 2019-08-26 13:51:54.000000 localstripe-1.9.1/localstripe.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)       58 2019-08-26 13:51:54.000000 localstripe-1.9.1/localstripe.egg-info/entry_points.txt
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)       38 2019-08-26 13:51:54.000000 localstripe-1.9.1/localstripe.egg-info/requires.txt
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)       12 2019-08-26 13:51:54.000000 localstripe-1.9.1/localstripe.egg-info/top_level.txt
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)      113 2019-08-26 13:51:54.000000 localstripe-1.9.1/setup.cfg
+-rw-rw-r--   0 adrien    (1000) adrien    (1000)     1323 2019-07-10 15:47:32.000000 localstripe-1.9.1/setup.py
```

### Comparing `localstripe-1.9.0/README.rst` & `localstripe-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `localstripe-1.9.0/localstripe/__init__.py` & `localstripe-1.9.1/localstripe/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 import sys
 
 
 if sys.version_info < (3, 5):
     raise RuntimeError('Please run with Python >= 3.5')
 
 __author__ = 'Adrien Vergé'
-__version__ = '1.9.0'
+__version__ = '1.9.1'
```

### Comparing `localstripe-1.9.0/localstripe/__main__.py` & `localstripe-1.9.1/localstripe/__main__.py`

 * *Files identical despite different names*

### Comparing `localstripe-1.9.0/localstripe/errors.py` & `localstripe-1.9.1/localstripe/errors.py`

 * *Files identical despite different names*

### Comparing `localstripe-1.9.0/localstripe/localstripe-v3.js` & `localstripe-1.9.1/localstripe/localstripe-v3.js`

 * *Files identical despite different names*

### Comparing `localstripe-1.9.0/localstripe/resources.py` & `localstripe-1.9.1/localstripe/resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -2057,15 +2057,16 @@
             invoice = Invoice(
                 customer=self.customer,
                 subscription=self.id,
                 items=invoice_items,
                 tax_percent=self.tax_percent,
                 date=self.current_period_start)
             self.latest_invoice = invoice.id
-            Invoice._api_pay_invoice(invoice.id)
+            if invoice.status != 'paid':  # 0 € invoices are already 'paid'
+                Invoice._api_pay_invoice(invoice.id)
 
             if invoice.status == 'paid':
                 self.status = 'active'
             elif invoice.charge:
                 if invoice.charge.status == 'failed':
                     if self.status != 'incomplete':
                         self._on_recurring_payment_failure(invoice)
```

### Comparing `localstripe-1.9.0/localstripe/server.py` & `localstripe-1.9.1/localstripe/server.py`

 * *Files identical despite different names*

### Comparing `localstripe-1.9.0/localstripe/webhooks.py` & `localstripe-1.9.1/localstripe/webhooks.py`

 * *Files identical despite different names*

### Comparing `localstripe-1.9.0/setup.py` & `localstripe-1.9.1/setup.py`

 * *Files identical despite different names*

