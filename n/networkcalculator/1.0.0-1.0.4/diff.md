# Comparing `tmp/networkcalculator-1.0.0.tar.gz` & `tmp/networkcalculator-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "networkcalculator-1.0.0.tar", last modified: Sun May 28 01:02:42 2023, max compression
+gzip compressed data, was "networkcalculator-1.0.4.tar", last modified: Mon Jun 19 23:19:16 2023, max compression
```

## Comparing `networkcalculator-1.0.0.tar` & `networkcalculator-1.0.4.tar`

### file list

```diff
@@ -1,10 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 01:02:42.456754 networkcalculator-1.0.0/
--rw-rw-rw-   0        0        0      507 2023-05-28 01:02:42.456754 networkcalculator-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     7903 2023-05-28 00:44:56.000000 networkcalculator-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 01:02:42.455754 networkcalculator-1.0.0/networkcalculator.egg-info/
--rw-rw-rw-   0        0        0      507 2023-05-28 01:02:42.000000 networkcalculator-1.0.0/networkcalculator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-05-28 01:02:42.000000 networkcalculator-1.0.0/networkcalculator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 01:02:42.000000 networkcalculator-1.0.0/networkcalculator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 01:02:42.000000 networkcalculator-1.0.0/networkcalculator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-28 01:02:42.456754 networkcalculator-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      627 2023-05-28 01:00:04.000000 networkcalculator-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:16.073254 networkcalculator-1.0.4/
+-rw-rw-rw-   0        0        0     1094 2023-06-18 18:29:24.000000 networkcalculator-1.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     7599 2023-06-19 23:19:16.073254 networkcalculator-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5522 2023-06-19 17:38:05.000000 networkcalculator-1.0.4/README.md
+-rw-rw-rw-   0        0        0       86 2023-06-19 14:18:05.000000 networkcalculator-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      815 2023-06-19 23:19:16.074254 networkcalculator-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      785 2023-06-19 23:18:54.000000 networkcalculator-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:16.052252 networkcalculator-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:16.062254 networkcalculator-1.0.4/src/cidr/
+-rw-rw-rw-   0        0        0        0 2023-06-19 14:01:58.000000 networkcalculator-1.0.4/src/cidr/__init__.py
+-rw-rw-rw-   0        0        0     5179 2023-06-19 17:28:02.000000 networkcalculator-1.0.4/src/cidr/network_calculator.py
+-rw-rw-rw-   0        0        0     1140 2023-06-19 15:39:01.000000 networkcalculator-1.0.4/src/cidr/network_calculator_test.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:16.066254 networkcalculator-1.0.4/src/feeds/
+-rw-rw-rw-   0        0        0        0 2023-06-19 14:01:58.000000 networkcalculator-1.0.4/src/feeds/__init__.py
+-rw-rw-rw-   0        0        0     8814 2023-06-19 18:02:12.000000 networkcalculator-1.0.4/src/feeds/bandwidth_calculator.py
+-rw-rw-rw-   0        0        0     3333 2023-06-19 18:05:24.000000 networkcalculator-1.0.4/src/feeds/bandwidth_calculator_test.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:16.069254 networkcalculator-1.0.4/src/networkcalculator.egg-info/
+-rw-rw-rw-   0        0        0     7599 2023-06-19 23:19:16.000000 networkcalculator-1.0.4/src/networkcalculator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      511 2023-06-19 23:19:16.000000 networkcalculator-1.0.4/src/networkcalculator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 23:19:16.000000 networkcalculator-1.0.4/src/networkcalculator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-19 23:19:16.000000 networkcalculator-1.0.4/src/networkcalculator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:16.072254 networkcalculator-1.0.4/src/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-19 14:02:58.000000 networkcalculator-1.0.4/src/tests/__init__.py
+-rw-rw-rw-   0        0        0     3333 2023-06-19 18:05:24.000000 networkcalculator-1.0.4/src/tests/bandwidth_calculator_test.py
+-rw-rw-rw-   0        0        0     5179 2023-06-19 19:19:05.000000 networkcalculator-1.0.4/src/tests/network_calculator.py
```

### Comparing `networkcalculator-1.0.0/setup.py` & `networkcalculator-1.0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 from setuptools import setup, find_packages
 
 setup(
     name='networkcalculator',
-    version='1.0.0',
+    version='1.0.4',
     author='Ray Bernard',
     author_email='ray.bernard@outlook.com',
     description='A network calculator package',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+
+
+
     ],
 )
```

