# Comparing `tmp/artd-customer-0.0.1.tar.gz` & `tmp/artd-customer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "artd-customer-0.0.1.tar", last modified: Tue Jun 20 15:00:51 2023, max compression
+gzip compressed data, was "artd-customer-0.0.2.tar", last modified: Tue Jun 20 15:36:33 2023, max compression
```

## Comparing `artd-customer-0.0.1.tar` & `artd-customer-0.0.2.tar`

### file list

```diff
@@ -1,36 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:00:51.731423 artd-customer-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-20 15:00:48.000000 artd-customer-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-20 15:00:48.000000 artd-customer-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-20 15:00:51.731423 artd-customer-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-20 15:00:48.000000 artd-customer-0.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:00:51.727423 artd-customer-0.0.1/artd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:00:48.000000 artd-customer-0.0.1/artd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-20 15:00:48.000000 artd-customer-0.0.1/artd/asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-20 15:00:48.000000 artd-customer-0.0.1/artd/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-20 15:00:48.000000 artd-customer-0.0.1/artd/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-20 15:00:48.000000 artd-customer-0.0.1/artd/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:00:51.731423 artd-customer-0.0.1/artd_customer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:00:48.000000 artd-customer-0.0.1/artd_customer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:00:51.731423 artd-customer-0.0.1/artd_customer/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-20 15:00:48.000000 artd-customer-0.0.1/artd_customer/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-20 15:00:48.000000 artd-customer-0.0.1/artd_customer/__pycache__/admin.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-20 15:00:48.000000 artd-customer-0.0.1/artd_customer/__pycache__/apps.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-06-20 15:00:48.000000 artd-customer-0.0.1/artd_customer/__pycache__/models.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-06-20 15:00:48.000000 artd-customer-0.0.1/artd_customer/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-20 15:00:48.000000 artd-customer-0.0.1/artd_customer/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:00:51.731423 artd-customer-0.0.1/artd_customer/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    14505 2023-06-20 15:00:48.000000 artd-customer-0.0.1/artd_customer/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:00:48.000000 artd-customer-0.0.1/artd_customer/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:00:51.731423 artd-customer-0.0.1/artd_customer/migrations/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-06-20 15:00:48.000000 artd-customer-0.0.1/artd_customer/migrations/__pycache__/0001_initial.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-20 15:00:48.000000 artd-customer-0.0.1/artd_customer/migrations/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-06-20 15:00:48.000000 artd-customer-0.0.1/artd_customer/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-20 15:00:48.000000 artd-customer-0.0.1/artd_customer/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-20 15:00:48.000000 artd-customer-0.0.1/artd_customer/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:00:51.731423 artd-customer-0.0.1/artd_customer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-20 15:00:51.000000 artd-customer-0.0.1/artd_customer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-20 15:00:51.000000 artd-customer-0.0.1/artd_customer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:00:51.000000 artd-customer-0.0.1/artd_customer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-20 15:00:51.000000 artd-customer-0.0.1/artd_customer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 15:00:51.731423 artd-customer-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-20 15:00:50.000000 artd-customer-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:36:33.938219 artd-customer-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-20 15:36:30.000000 artd-customer-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-20 15:36:30.000000 artd-customer-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-20 15:36:33.938219 artd-customer-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-20 15:36:30.000000 artd-customer-0.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:36:33.934219 artd-customer-0.0.2/artd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:36:30.000000 artd-customer-0.0.2/artd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-20 15:36:30.000000 artd-customer-0.0.2/artd/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-06-20 15:36:30.000000 artd-customer-0.0.2/artd/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-20 15:36:30.000000 artd-customer-0.0.2/artd/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-20 15:36:30.000000 artd-customer-0.0.2/artd/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:36:33.934219 artd-customer-0.0.2/artd_customer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:36:30.000000 artd-customer-0.0.2/artd_customer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:36:33.938219 artd-customer-0.0.2/artd_customer/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-20 15:36:30.000000 artd-customer-0.0.2/artd_customer/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-20 15:36:30.000000 artd-customer-0.0.2/artd_customer/__pycache__/admin.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-20 15:36:30.000000 artd-customer-0.0.2/artd_customer/__pycache__/apps.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-06-20 15:36:30.000000 artd-customer-0.0.2/artd_customer/__pycache__/models.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-06-20 15:36:30.000000 artd-customer-0.0.2/artd_customer/__pycache__/tests.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-06-20 15:36:30.000000 artd-customer-0.0.2/artd_customer/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-20 15:36:30.000000 artd-customer-0.0.2/artd_customer/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:36:33.938219 artd-customer-0.0.2/artd_customer/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    14505 2023-06-20 15:36:30.000000 artd-customer-0.0.2/artd_customer/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:36:30.000000 artd-customer-0.0.2/artd_customer/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:36:33.938219 artd-customer-0.0.2/artd_customer/migrations/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-06-20 15:36:30.000000 artd-customer-0.0.2/artd_customer/migrations/__pycache__/0001_initial.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-20 15:36:30.000000 artd-customer-0.0.2/artd_customer/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-06-20 15:36:30.000000 artd-customer-0.0.2/artd_customer/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-06-20 15:36:30.000000 artd-customer-0.0.2/artd_customer/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:36:33.938219 artd-customer-0.0.2/artd_customer/utils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:36:33.938219 artd-customer-0.0.2/artd_customer/utils/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-20 15:36:30.000000 artd-customer-0.0.2/artd_customer/utils/__pycache__/generators.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-20 15:36:30.000000 artd-customer-0.0.2/artd_customer/utils/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-20 15:36:30.000000 artd-customer-0.0.2/artd_customer/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:36:33.938219 artd-customer-0.0.2/artd_customer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-20 15:36:33.000000 artd-customer-0.0.2/artd_customer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-20 15:36:33.000000 artd-customer-0.0.2/artd_customer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:36:33.000000 artd-customer-0.0.2/artd_customer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-20 15:36:33.000000 artd-customer-0.0.2/artd_customer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 15:36:33.938219 artd-customer-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-20 15:36:32.000000 artd-customer-0.0.2/setup.py
```

### Comparing `artd-customer-0.0.1/LICENSE` & `artd-customer-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `artd-customer-0.0.1/PKG-INFO` & `artd-customer-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artd-customer
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Django app to administrate customer
 Home-page: https://www.artd.com.co/
 Author: Jonathan Urzola Maladonado
 Author-email: jonathan@artd.com.co
 Keywords: pypi,cicd,python
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `artd-customer-0.0.1/README.rst` & `artd-customer-0.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `artd-customer-0.0.1/artd/settings.py` & `artd-customer-0.0.2/artd/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,18 @@
 INSTALLED_APPS = [
     "django.contrib.admin",
     "django.contrib.auth",
     "django.contrib.contenttypes",
     "django.contrib.sessions",
     "django.contrib.messages",
     "django.contrib.staticfiles",
+    "artd_location",
+    "artd_partner",
+    "django_json_widget",
+    "artd_customer",
 ]
 
 MIDDLEWARE = [
     "django.middleware.security.SecurityMiddleware",
     "django.contrib.sessions.middleware.SessionMiddleware",
     "django.middleware.common.CommonMiddleware",
     "django.middleware.csrf.CsrfViewMiddleware",
```

### Comparing `artd-customer-0.0.1/artd/urls.py` & `artd-customer-0.0.2/artd/urls.py`

 * *Files identical despite different names*

### Comparing `artd-customer-0.0.1/artd_customer/__pycache__/admin.cpython-310.pyc` & `artd-customer-0.0.2/artd_customer/__pycache__/admin.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `artd-customer-0.0.1/artd_customer/__pycache__/apps.cpython-310.pyc` & `artd-customer-0.0.2/artd_customer/__pycache__/apps.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `artd-customer-0.0.1/artd_customer/__pycache__/models.cpython-310.pyc` & `artd-customer-0.0.2/artd_customer/__pycache__/models.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `artd-customer-0.0.1/artd_customer/admin.py` & `artd-customer-0.0.2/artd_customer/admin.py`

 * *Files identical despite different names*

### Comparing `artd-customer-0.0.1/artd_customer/migrations/0001_initial.py` & `artd-customer-0.0.2/artd_customer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `artd-customer-0.0.1/artd_customer/migrations/__pycache__/0001_initial.cpython-310.pyc` & `artd-customer-0.0.2/artd_customer/migrations/__pycache__/0001_initial.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `artd-customer-0.0.1/artd_customer/models.py` & `artd-customer-0.0.2/artd_customer/models.py`

 * *Files identical despite different names*

### Comparing `artd-customer-0.0.1/artd_customer.egg-info/PKG-INFO` & `artd-customer-0.0.2/artd_customer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artd-customer
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Django app to administrate customer
 Home-page: https://www.artd.com.co/
 Author: Jonathan Urzola Maladonado
 Author-email: jonathan@artd.com.co
 Keywords: pypi,cicd,python
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `artd-customer-0.0.1/artd_customer.egg-info/SOURCES.txt` & `artd-customer-0.0.2/artd_customer.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -17,11 +17,14 @@
 artd_customer.egg-info/SOURCES.txt
 artd_customer.egg-info/dependency_links.txt
 artd_customer.egg-info/top_level.txt
 artd_customer/__pycache__/__init__.cpython-310.pyc
 artd_customer/__pycache__/admin.cpython-310.pyc
 artd_customer/__pycache__/apps.cpython-310.pyc
 artd_customer/__pycache__/models.cpython-310.pyc
+artd_customer/__pycache__/tests.cpython-310.pyc
 artd_customer/migrations/0001_initial.py
 artd_customer/migrations/__init__.py
 artd_customer/migrations/__pycache__/0001_initial.cpython-310.pyc
-artd_customer/migrations/__pycache__/__init__.cpython-310.pyc
+artd_customer/migrations/__pycache__/__init__.cpython-310.pyc
+artd_customer/utils/generators.py
+artd_customer/utils/__pycache__/generators.cpython-310.pyc
```

### Comparing `artd-customer-0.0.1/setup.py` & `artd-customer-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.rst").read_text()
 
 setup(
     name="artd-customer",
-    version="0.0.1",
+    version="0.0.2",
     include_package_data=True,
     author="Jonathan Urzola Maladonado",
     author_email="jonathan@artd.com.co",
     description="A Django app to administrate customer",
     long_description_content_type="text/markdown",
     url="https://www.artd.com.co/",
     long_description=long_description,
```

