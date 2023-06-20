# Comparing `tmp/circular-dict-1.4.tar.gz` & `tmp/circular-dict-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circular-dict-1.4.tar", last modified: Mon Jun 19 23:50:40 2023, max compression
+gzip compressed data, was "circular-dict-1.5.tar", last modified: Tue Jun 20 08:15:53 2023, max compression
```

## Comparing `circular-dict-1.4.tar` & `circular-dict-1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 23:50:40.202142 circular-dict-1.4/
--rw-rw-rw-   0        0        0     1089 2023-06-19 11:41:28.000000 circular-dict-1.4/LICENSE
--rw-rw-rw-   0        0        0     5925 2023-06-19 23:50:40.202142 circular-dict-1.4/PKG-INFO
--rw-rw-rw-   0        0        0     4258 2023-06-19 23:50:27.000000 circular-dict-1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 23:50:40.184146 circular-dict-1.4/circular_dict/
--rw-rw-rw-   0        0        0     4798 2023-06-19 23:50:27.000000 circular-dict-1.4/circular_dict/CircularDict.py
--rw-rw-rw-   0        0        0       38 2023-06-19 12:09:31.000000 circular-dict-1.4/circular_dict/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:50:40.200183 circular-dict-1.4/circular_dict.egg-info/
--rw-rw-rw-   0        0        0     5925 2023-06-19 23:50:40.000000 circular-dict-1.4/circular_dict.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-06-19 23:50:40.000000 circular-dict-1.4/circular_dict.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 23:50:40.000000 circular-dict-1.4/circular_dict.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-19 23:50:40.000000 circular-dict-1.4/circular_dict.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 23:50:40.203205 circular-dict-1.4/setup.cfg
--rw-rw-rw-   0        0        0     1863 2023-06-19 23:50:35.000000 circular-dict-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:15:53.700155 circular-dict-1.5/
+-rw-rw-rw-   0        0        0     1089 2023-06-19 11:41:28.000000 circular-dict-1.5/LICENSE
+-rw-rw-rw-   0        0        0     5925 2023-06-20 08:15:53.699152 circular-dict-1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4258 2023-06-20 08:15:45.000000 circular-dict-1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 08:15:53.666321 circular-dict-1.5/circular_dict/
+-rw-rw-rw-   0        0        0     4798 2023-06-19 23:50:27.000000 circular-dict-1.5/circular_dict/CircularDict.py
+-rw-rw-rw-   0        0        0       38 2023-06-19 12:09:31.000000 circular-dict-1.5/circular_dict/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:15:53.696617 circular-dict-1.5/circular_dict.egg-info/
+-rw-rw-rw-   0        0        0     5925 2023-06-20 08:15:53.000000 circular-dict-1.5/circular_dict.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-06-20 08:15:53.000000 circular-dict-1.5/circular_dict.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 08:15:53.000000 circular-dict-1.5/circular_dict.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-20 08:15:53.000000 circular-dict-1.5/circular_dict.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 08:15:53.701152 circular-dict-1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1863 2023-06-20 08:15:45.000000 circular-dict-1.5/setup.py
```

### Comparing `circular-dict-1.4/LICENSE` & `circular-dict-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `circular-dict-1.4/PKG-INFO` & `circular-dict-1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circular-dict
-Version: 1.4
+Version: 1.5
 Summary: CircularDict is a high-performance Python data structure that blends the functionality of dictionaries and circular buffers. Inheriting the usage of traditional dictionaries, it allows you to define constraints on size and memory usage. This way, the CircularDict will be always up-to-date with the last N added elements, ensuring that neither the maximum length nor the memory usage limit is exceeded. It is ideal for caching large data structures while maintaining control over memory footprint. 
 Home-page: https://github.com/Eric-Canas/CircularDict
 Author: Eric-Canas
 Author-email: eric@ericcanas.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -63,15 +63,15 @@
 my_buffer['item1'] = 'value1'
 my_buffer['item2'] = 'value2'
 my_buffer['item3'] = 'value3'
 
 print(f"When filling it: {circ_dict}")
 
 # Add another item
-circ_dict['item4'] = 'value4'
+my_buffer['item4'] = 'value4'
 
 print(f"After adding an element beyond maxlen: {circ_dict}")
 ```
 
 Output:
 ```bash
 When filling it: {'item1': 'value1', 'item2': 'value2', 'item3': 'value3'}
```

### Comparing `circular-dict-1.4/README.md` & `circular-dict-1.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 my_buffer['item1'] = 'value1'
 my_buffer['item2'] = 'value2'
 my_buffer['item3'] = 'value3'
 
 print(f"When filling it: {circ_dict}")
 
 # Add another item
-circ_dict['item4'] = 'value4'
+my_buffer['item4'] = 'value4'
 
 print(f"After adding an element beyond maxlen: {circ_dict}")
 ```
 
 Output:
 ```bash
 When filling it: {'item1': 'value1', 'item2': 'value2', 'item3': 'value3'}
```

### Comparing `circular-dict-1.4/circular_dict/CircularDict.py` & `circular-dict-1.5/circular_dict/CircularDict.py`

 * *Files identical despite different names*

### Comparing `circular-dict-1.4/circular_dict.egg-info/PKG-INFO` & `circular-dict-1.5/circular_dict.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circular-dict
-Version: 1.4
+Version: 1.5
 Summary: CircularDict is a high-performance Python data structure that blends the functionality of dictionaries and circular buffers. Inheriting the usage of traditional dictionaries, it allows you to define constraints on size and memory usage. This way, the CircularDict will be always up-to-date with the last N added elements, ensuring that neither the maximum length nor the memory usage limit is exceeded. It is ideal for caching large data structures while maintaining control over memory footprint. 
 Home-page: https://github.com/Eric-Canas/CircularDict
 Author: Eric-Canas
 Author-email: eric@ericcanas.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -63,15 +63,15 @@
 my_buffer['item1'] = 'value1'
 my_buffer['item2'] = 'value2'
 my_buffer['item3'] = 'value3'
 
 print(f"When filling it: {circ_dict}")
 
 # Add another item
-circ_dict['item4'] = 'value4'
+my_buffer['item4'] = 'value4'
 
 print(f"After adding an element beyond maxlen: {circ_dict}")
 ```
 
 Output:
 ```bash
 When filling it: {'item1': 'value1', 'item2': 'value2', 'item3': 'value3'}
```

### Comparing `circular-dict-1.4/setup.py` & `circular-dict-1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='circular-dict',
-    version='1.4',
+    version='1.5',
     author='Eric-Canas',
     author_email='eric@ericcanas.com',
     url='https://github.com/Eric-Canas/CircularDict',
     description='CircularDict is a high-performance Python data structure that blends the functionality of dictionaries and circular buffers. '
                 'Inheriting the usage of traditional dictionaries, it allows you to define constraints on size and memory usage. '
                 'This way, the CircularDict will be always up-to-date with the last N added elements, ensuring that neither the maximum length nor '
                 'the memory usage limit is exceeded. It is ideal for caching large data structures while maintaining control over memory footprint. ',
```

