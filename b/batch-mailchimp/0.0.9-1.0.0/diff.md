# Comparing `tmp/batch-mailchimp-0.0.9.tar.gz` & `tmp/batch-mailchimp-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/batch-mailchimp-0.0.9.tar", last modified: Thu Jun 11 21:05:03 2020, max compression
+gzip compressed data, was "batch-mailchimp-1.0.0.tar", last modified: Tue Jun 20 18:17:43 2023, max compression
```

## Comparing `batch-mailchimp-0.0.9.tar` & `batch-mailchimp-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 Andy       (501) staff       (20)        0 2020-06-11 21:05:03.000000 batch-mailchimp-0.0.9/
--rw-r--r--   0 Andy       (501) staff       (20)     3608 2020-06-11 21:05:03.000000 batch-mailchimp-0.0.9/PKG-INFO
-drwxr-xr-x   0 Andy       (501) staff       (20)        0 2020-06-11 21:05:03.000000 batch-mailchimp-0.0.9/batch_mailchimp/
--rw-r--r--   0 Andy       (501) staff       (20)     2386 2020-06-11 21:02:18.000000 batch-mailchimp-0.0.9/batch_mailchimp/__init__.py
--rw-r--r--   0 Andy       (501) staff       (20)     1188 2020-06-11 10:48:22.000000 batch-mailchimp-0.0.9/batch_mailchimp/batch_operations.py
-drwxr-xr-x   0 Andy       (501) staff       (20)        0 2020-06-11 21:05:03.000000 batch-mailchimp-0.0.9/batch_mailchimp.egg-info/
--rw-r--r--   0 Andy       (501) staff       (20)     3608 2020-06-11 21:05:03.000000 batch-mailchimp-0.0.9/batch_mailchimp.egg-info/PKG-INFO
--rw-r--r--   0 Andy       (501) staff       (20)      277 2020-06-11 21:05:03.000000 batch-mailchimp-0.0.9/batch_mailchimp.egg-info/SOURCES.txt
--rw-r--r--   0 Andy       (501) staff       (20)       18 2020-06-11 21:05:03.000000 batch-mailchimp-0.0.9/batch_mailchimp.egg-info/requires.txt
--rw-r--r--   0 Andy       (501) staff       (20)       16 2020-06-11 21:05:03.000000 batch-mailchimp-0.0.9/batch_mailchimp.egg-info/top_level.txt
--rw-r--r--   0 Andy       (501) staff       (20)        1 2020-06-11 21:05:03.000000 batch-mailchimp-0.0.9/batch_mailchimp.egg-info/dependency_links.txt
--rw-r--r--   0 Andy       (501) staff       (20)     1211 2020-06-11 21:04:48.000000 batch-mailchimp-0.0.9/setup.py
--rw-r--r--   0 Andy       (501) staff       (20)       59 2020-06-11 21:05:03.000000 batch-mailchimp-0.0.9/setup.cfg
--rw-r--r--   0 Andy       (501) staff       (20)     2039 2020-06-11 17:00:30.000000 batch-mailchimp-0.0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:17:43.269902 batch-mailchimp-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-20 18:17:31.000000 batch-mailchimp-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-06-20 18:17:43.269902 batch-mailchimp-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-06-20 18:17:31.000000 batch-mailchimp-1.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:17:43.269902 batch-mailchimp-1.0.0/batch_mailchimp/
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-06-20 18:17:31.000000 batch-mailchimp-1.0.0/batch_mailchimp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-06-20 18:17:31.000000 batch-mailchimp-1.0.0/batch_mailchimp/batches_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:17:43.269902 batch-mailchimp-1.0.0/batch_mailchimp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-06-20 18:17:43.000000 batch-mailchimp-1.0.0/batch_mailchimp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-20 18:17:43.000000 batch-mailchimp-1.0.0/batch_mailchimp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 18:17:43.000000 batch-mailchimp-1.0.0/batch_mailchimp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-20 18:17:43.000000 batch-mailchimp-1.0.0/batch_mailchimp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-20 18:17:43.000000 batch-mailchimp-1.0.0/batch_mailchimp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 18:17:43.269902 batch-mailchimp-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-20 18:17:31.000000 batch-mailchimp-1.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `batch-mailchimp-0.0.9/PKG-INFO` & `batch-mailchimp-1.0.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,105 +1,112 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: batch-mailchimp
-Version: 0.0.9
+Version: 1.0.0
 Summary: A python client for v3 of MailChimp API, with batch support
 Home-page: https://github.com/FullFact/python-batchmailchimp
 Author: Andy Lulham
 Author-email: andy.lulham@fullfact.org
 License: MIT
-Description: Python BatchMailchimp
-        =====================
-        
-        A light wrapper around `mailchimp3 <https://pypi.org/project/mailchimp3/>`__ that makes it easier to use batch
-        operations.
-        
-        Getting Started
-        ---------------
-        
-        Installation
-        ~~~~~~~~~~~~
-        
-        ::
-        
-           pip install batch-mailchimp
-        
-        Usage
-        ~~~~~
-        
-        This can be used as a drop-in replacement for mailchimp3 – just change
-        the import at the top, and everything should work the same:
-        
-        .. code:: python
-        
-           from batch_mailchimp import BatchMailChimp as MailChimp
-        
-           client = MailChimp(
-               mc_api='YOUR_API_KEY',
-               mc_user='YOUR_USERNAME')
-        
-        The additional functionality comes when we initialise the client with ``batch=True``:
-        
-        .. code:: python
-        
-           from batch_mailchimp import BatchMailChimp as MailChimp
-        
-           batch_client = MailChimp(
-               mc_api='YOUR_API_KEY',
-               mc_user='YOUR_USERNAME',
-               batch=True)
-        
-        If we do this, operations are stored up in the client, to be run later. For example:
-        
-        .. code:: python
-        
-           # add John Doe with email john.doe@example.com to list matching id '123456'
-           batch_client.lists.members.create(
-               '123456', {
-                   'email_address': 'john.doe@example.com',
-                   'status': 'subscribed',
-                   'merge_fields': {
-                       'FNAME': 'John',
-                       'LNAME': 'Doe',
-                   },
-               },
-           )
-        
-        All new operations will be added to the batch. When we’re ready, we can run all the operations in the batch:
-        
-        .. code:: python
-        
-           batch = batch_client.run_batch()
-        
-        We can check the batch’s status using:
-        
-        .. code:: python
-        
-           batch.status()
-        
-        API Structure and Endpoints
-        ---------------------------
-        
-        The API structure and endpoints match that of `mailchimp3 <https://pypi.org/project/mailchimp3/>`__. You should refer to their documentation for usage.
-        
-        Support
-        -------
-        
-        If you are having issues, please `create an issue <https://github.com/FullFact/python-batchmailchimp/issues>`__ or `submit a pull request <https://github.com/FullFact/python-batchmailchimp/pulls>`__.
-        
-        License
-        -------
-        
-        The project is licensed under the MIT License.
-        
 Keywords: mailchimp api v3 client wrapper
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+License-File: LICENSE
+
+Python BatchMailchimp
+=====================
+
+.. image:: https://img.shields.io/pypi/v/batch-mailchimp.svg
+    :alt: PyPI Package latest release
+    :target: https://pypi.org/project/batch-mailchimp/
+
+.. image:: https://img.shields.io/pypi/l/batch-mailchimp.svg
+    :alt: License
+    :target: https://pypi.org/project/batch-mailchimp/
+
+A light wrapper around `mailchimp-marketing <https://pypi.org/project/mailchimp-marketing/>`__ that makes it easier to use batch operations.
+
+Getting Started
+---------------
+
+Installation
+~~~~~~~~~~~~
+
+::
+
+   pip install batch-mailchimp
+
+Usage
+~~~~~
+
+This can be used as a drop-in replacement for mailchimp-marketing –
+just change the import at the top, and everything should work the same:
+
+.. code:: python
+
+   import batch_mailchimp as MailchimpMarketing
+
+   client = MailchimpMarketing.Client({
+       "api_key": "YOUR_API_KEY",
+   })
+
+The additional functionality comes when we initialise the client with ``batch=True``:
+
+.. code:: python
+
+   import batch_mailchimp as MailchimpMarketing
+
+   client = MailchimpMarketing.Client({
+       "api_key": "YOUR_API_KEY",
+       "batch": True,
+   })
+
+If we do this, operations are stored up in the client, to be run later. For example:
+
+.. code:: python
+
+   # add John Doe with email john.doe@example.com to list matching id '123456'
+   client.lists.members.create(
+       '123456', {
+           'email_address': 'john.doe@example.com',
+           'status': 'subscribed',
+           'merge_fields': {
+               'FNAME': 'John',
+               'LNAME': 'Doe',
+           },
+       },
+   )
+
+All new operations will be added to the batch. When we’re ready, we can run all the operations in the batch:
+
+.. code:: python
+
+   batch = batch_client.batches.run()
+
+We can check the batch’s status using:
+
+.. code:: python
+
+   batch.status()
+
+API Structure and Endpoints
+---------------------------
+
+The API structure and endpoints match that of `mailchimp3 <https://pypi.org/project/mailchimp3/>`__. You should refer to their documentation for usage.
+
+Support
+-------
+
+If you are having issues, please `create an issue <https://github.com/FullFact/python-batchmailchimp/issues>`__.
+
+License
+-------
+
+The project is licensed under the MIT License.
```

### Comparing `batch-mailchimp-0.0.9/batch_mailchimp.egg-info/PKG-INFO` & `batch-mailchimp-1.0.0/batch_mailchimp.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,105 +1,112 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: batch-mailchimp
-Version: 0.0.9
+Version: 1.0.0
 Summary: A python client for v3 of MailChimp API, with batch support
 Home-page: https://github.com/FullFact/python-batchmailchimp
 Author: Andy Lulham
 Author-email: andy.lulham@fullfact.org
 License: MIT
-Description: Python BatchMailchimp
-        =====================
-        
-        A light wrapper around `mailchimp3 <https://pypi.org/project/mailchimp3/>`__ that makes it easier to use batch
-        operations.
-        
-        Getting Started
-        ---------------
-        
-        Installation
-        ~~~~~~~~~~~~
-        
-        ::
-        
-           pip install batch-mailchimp
-        
-        Usage
-        ~~~~~
-        
-        This can be used as a drop-in replacement for mailchimp3 – just change
-        the import at the top, and everything should work the same:
-        
-        .. code:: python
-        
-           from batch_mailchimp import BatchMailChimp as MailChimp
-        
-           client = MailChimp(
-               mc_api='YOUR_API_KEY',
-               mc_user='YOUR_USERNAME')
-        
-        The additional functionality comes when we initialise the client with ``batch=True``:
-        
-        .. code:: python
-        
-           from batch_mailchimp import BatchMailChimp as MailChimp
-        
-           batch_client = MailChimp(
-               mc_api='YOUR_API_KEY',
-               mc_user='YOUR_USERNAME',
-               batch=True)
-        
-        If we do this, operations are stored up in the client, to be run later. For example:
-        
-        .. code:: python
-        
-           # add John Doe with email john.doe@example.com to list matching id '123456'
-           batch_client.lists.members.create(
-               '123456', {
-                   'email_address': 'john.doe@example.com',
-                   'status': 'subscribed',
-                   'merge_fields': {
-                       'FNAME': 'John',
-                       'LNAME': 'Doe',
-                   },
-               },
-           )
-        
-        All new operations will be added to the batch. When we’re ready, we can run all the operations in the batch:
-        
-        .. code:: python
-        
-           batch = batch_client.run_batch()
-        
-        We can check the batch’s status using:
-        
-        .. code:: python
-        
-           batch.status()
-        
-        API Structure and Endpoints
-        ---------------------------
-        
-        The API structure and endpoints match that of `mailchimp3 <https://pypi.org/project/mailchimp3/>`__. You should refer to their documentation for usage.
-        
-        Support
-        -------
-        
-        If you are having issues, please `create an issue <https://github.com/FullFact/python-batchmailchimp/issues>`__ or `submit a pull request <https://github.com/FullFact/python-batchmailchimp/pulls>`__.
-        
-        License
-        -------
-        
-        The project is licensed under the MIT License.
-        
 Keywords: mailchimp api v3 client wrapper
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+License-File: LICENSE
+
+Python BatchMailchimp
+=====================
+
+.. image:: https://img.shields.io/pypi/v/batch-mailchimp.svg
+    :alt: PyPI Package latest release
+    :target: https://pypi.org/project/batch-mailchimp/
+
+.. image:: https://img.shields.io/pypi/l/batch-mailchimp.svg
+    :alt: License
+    :target: https://pypi.org/project/batch-mailchimp/
+
+A light wrapper around `mailchimp-marketing <https://pypi.org/project/mailchimp-marketing/>`__ that makes it easier to use batch operations.
+
+Getting Started
+---------------
+
+Installation
+~~~~~~~~~~~~
+
+::
+
+   pip install batch-mailchimp
+
+Usage
+~~~~~
+
+This can be used as a drop-in replacement for mailchimp-marketing –
+just change the import at the top, and everything should work the same:
+
+.. code:: python
+
+   import batch_mailchimp as MailchimpMarketing
+
+   client = MailchimpMarketing.Client({
+       "api_key": "YOUR_API_KEY",
+   })
+
+The additional functionality comes when we initialise the client with ``batch=True``:
+
+.. code:: python
+
+   import batch_mailchimp as MailchimpMarketing
+
+   client = MailchimpMarketing.Client({
+       "api_key": "YOUR_API_KEY",
+       "batch": True,
+   })
+
+If we do this, operations are stored up in the client, to be run later. For example:
+
+.. code:: python
+
+   # add John Doe with email john.doe@example.com to list matching id '123456'
+   client.lists.members.create(
+       '123456', {
+           'email_address': 'john.doe@example.com',
+           'status': 'subscribed',
+           'merge_fields': {
+               'FNAME': 'John',
+               'LNAME': 'Doe',
+           },
+       },
+   )
+
+All new operations will be added to the batch. When we’re ready, we can run all the operations in the batch:
+
+.. code:: python
+
+   batch = batch_client.batches.run()
+
+We can check the batch’s status using:
+
+.. code:: python
+
+   batch.status()
+
+API Structure and Endpoints
+---------------------------
+
+The API structure and endpoints match that of `mailchimp3 <https://pypi.org/project/mailchimp3/>`__. You should refer to their documentation for usage.
+
+Support
+-------
+
+If you are having issues, please `create an issue <https://github.com/FullFact/python-batchmailchimp/issues>`__.
+
+License
+-------
+
+The project is licensed under the MIT License.
```

### Comparing `batch-mailchimp-0.0.9/setup.py` & `batch-mailchimp-1.0.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 
 setup(
     name='batch-mailchimp',
     description='A python client for v3 of MailChimp API, with batch support',
     url='https://github.com/FullFact/python-batchmailchimp',
     author='Andy Lulham',
     author_email='andy.lulham@fullfact.org',
-    version='0.0.9',
+    version='1.0.0',
     packages=find_packages(),
     license='MIT',
     keywords='mailchimp api v3 client wrapper',
     long_description=readme,
-    install_requires=['mailchimp3>=2.0.0'],
+    install_requires=['mailchimp-marketing>=3.0.80'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 2.7',
```

### Comparing `batch-mailchimp-0.0.9/README.rst` & `batch-mailchimp-1.0.0/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,69 +1,76 @@
 Python BatchMailchimp
 =====================
 
-A light wrapper around `mailchimp3 <https://pypi.org/project/mailchimp3/>`__ that makes it easier to use batch
-operations.
+.. image:: https://img.shields.io/pypi/v/batch-mailchimp.svg
+    :alt: PyPI Package latest release
+    :target: https://pypi.org/project/batch-mailchimp/
+
+.. image:: https://img.shields.io/pypi/l/batch-mailchimp.svg
+    :alt: License
+    :target: https://pypi.org/project/batch-mailchimp/
+
+A light wrapper around `mailchimp-marketing <https://pypi.org/project/mailchimp-marketing/>`__ that makes it easier to use batch operations.
 
 Getting Started
 ---------------
 
 Installation
 ~~~~~~~~~~~~
 
 ::
 
    pip install batch-mailchimp
 
 Usage
 ~~~~~
 
-This can be used as a drop-in replacement for mailchimp3 – just change
-the import at the top, and everything should work the same:
+This can be used as a drop-in replacement for mailchimp-marketing –
+just change the import at the top, and everything should work the same:
 
 .. code:: python
 
-   from batch_mailchimp import BatchMailChimp as MailChimp
+   import batch_mailchimp as MailchimpMarketing
 
-   client = MailChimp(
-       mc_api='YOUR_API_KEY',
-       mc_user='YOUR_USERNAME')
+   client = MailchimpMarketing.Client({
+       "api_key": "YOUR_API_KEY",
+   })
 
 The additional functionality comes when we initialise the client with ``batch=True``:
 
 .. code:: python
 
-   from batch_mailchimp import BatchMailChimp as MailChimp
+   import batch_mailchimp as MailchimpMarketing
 
-   batch_client = MailChimp(
-       mc_api='YOUR_API_KEY',
-       mc_user='YOUR_USERNAME',
-       batch=True)
+   client = MailchimpMarketing.Client({
+       "api_key": "YOUR_API_KEY",
+       "batch": True,
+   })
 
 If we do this, operations are stored up in the client, to be run later. For example:
 
 .. code:: python
 
    # add John Doe with email john.doe@example.com to list matching id '123456'
-   batch_client.lists.members.create(
+   client.lists.members.create(
        '123456', {
            'email_address': 'john.doe@example.com',
            'status': 'subscribed',
            'merge_fields': {
                'FNAME': 'John',
                'LNAME': 'Doe',
            },
        },
    )
 
 All new operations will be added to the batch. When we’re ready, we can run all the operations in the batch:
 
 .. code:: python
 
-   batch = batch_client.run_batch()
+   batch = batch_client.batches.run()
 
 We can check the batch’s status using:
 
 .. code:: python
 
    batch.status()
 
@@ -71,13 +78,13 @@
 ---------------------------
 
 The API structure and endpoints match that of `mailchimp3 <https://pypi.org/project/mailchimp3/>`__. You should refer to their documentation for usage.
 
 Support
 -------
 
-If you are having issues, please `create an issue <https://github.com/FullFact/python-batchmailchimp/issues>`__ or `submit a pull request <https://github.com/FullFact/python-batchmailchimp/pulls>`__.
+If you are having issues, please `create an issue <https://github.com/FullFact/python-batchmailchimp/issues>`__.
 
 License
 -------
 
 The project is licensed under the MIT License.
```

