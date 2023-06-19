# Comparing `tmp/circular-dict-1.3.tar.gz` & `tmp/circular-dict-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circular-dict-1.3.tar", last modified: Mon Jun 19 23:39:08 2023, max compression
+gzip compressed data, was "circular-dict-1.4.tar", last modified: Mon Jun 19 23:50:40 2023, max compression
```

## Comparing `circular-dict-1.3.tar` & `circular-dict-1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 23:39:08.331064 circular-dict-1.3/
--rw-rw-rw-   0        0        0     1089 2023-06-19 11:41:28.000000 circular-dict-1.3/LICENSE
--rw-rw-rw-   0        0        0     5687 2023-06-19 23:39:08.330064 circular-dict-1.3/PKG-INFO
--rw-rw-rw-   0        0        0     4020 2023-06-19 23:38:49.000000 circular-dict-1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 23:39:08.319143 circular-dict-1.3/circular_dict/
--rw-rw-rw-   0        0        0     4798 2023-06-19 23:38:49.000000 circular-dict-1.3/circular_dict/CircularDict.py
--rw-rw-rw-   0        0        0       38 2023-06-19 12:09:31.000000 circular-dict-1.3/circular_dict/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:39:08.328063 circular-dict-1.3/circular_dict.egg-info/
--rw-rw-rw-   0        0        0     5687 2023-06-19 23:39:08.000000 circular-dict-1.3/circular_dict.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-06-19 23:39:08.000000 circular-dict-1.3/circular_dict.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 23:39:08.000000 circular-dict-1.3/circular_dict.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-19 23:39:08.000000 circular-dict-1.3/circular_dict.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 23:39:08.332067 circular-dict-1.3/setup.cfg
--rw-rw-rw-   0        0        0     1863 2023-06-19 23:38:49.000000 circular-dict-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:50:40.202142 circular-dict-1.4/
+-rw-rw-rw-   0        0        0     1089 2023-06-19 11:41:28.000000 circular-dict-1.4/LICENSE
+-rw-rw-rw-   0        0        0     5925 2023-06-19 23:50:40.202142 circular-dict-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4258 2023-06-19 23:50:27.000000 circular-dict-1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 23:50:40.184146 circular-dict-1.4/circular_dict/
+-rw-rw-rw-   0        0        0     4798 2023-06-19 23:50:27.000000 circular-dict-1.4/circular_dict/CircularDict.py
+-rw-rw-rw-   0        0        0       38 2023-06-19 12:09:31.000000 circular-dict-1.4/circular_dict/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:50:40.200183 circular-dict-1.4/circular_dict.egg-info/
+-rw-rw-rw-   0        0        0     5925 2023-06-19 23:50:40.000000 circular-dict-1.4/circular_dict.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-06-19 23:50:40.000000 circular-dict-1.4/circular_dict.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 23:50:40.000000 circular-dict-1.4/circular_dict.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-19 23:50:40.000000 circular-dict-1.4/circular_dict.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 23:50:40.203205 circular-dict-1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1863 2023-06-19 23:50:35.000000 circular-dict-1.4/setup.py
```

### Comparing `circular-dict-1.3/LICENSE` & `circular-dict-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `circular-dict-1.3/PKG-INFO` & `circular-dict-1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circular-dict
-Version: 1.3
+Version: 1.4
 Summary: CircularDict is a high-performance Python data structure that blends the functionality of dictionaries and circular buffers. Inheriting the usage of traditional dictionaries, it allows you to define constraints on size and memory usage. This way, the CircularDict will be always up-to-date with the last N added elements, ensuring that neither the maximum length nor the memory usage limit is exceeded. It is ideal for caching large data structures while maintaining control over memory footprint. 
 Home-page: https://github.com/Eric-Canas/CircularDict
 Author: Eric-Canas
 Author-email: eric@ericcanas.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -39,18 +39,23 @@
 
 ```bash
 pip install circular-dict
 ```
 
 ## Usage
 
-Working with **CircularDict** is as simple as using a standard Python `dict`, with additional parameters `maxlen` or `maxsize_bytes` on the initialization to control the buffer size. 
+Working with **CircularDict** is as simple as using a standard Python `dict`, with additional parameters `maxlen` or `maxsize_bytes` on the initialization to control the buffer size. You can use one of them or both.
+```python
+from circular_dict import CircularDict
+# Initialize a CircularDict with a maximum length of 3 items and a storage limit of 4Mb
+my_dict = CircularDict(maxlen=3, maxsize_bytes=4*1024*1024)
+```
 
-#### Example with `maxlen`
-You can use `maxlen` to define a maximum amount of items that the dictionary can store. It is useful for defining fixed size buffers.
+### Example with `maxlen`
+You can use `maxlen` to define the maximum amount of items that the dictionary can store. It is useful for defining fixed size buffers.
 
 ```python
 from circular_dict import CircularDict
 
 # Initialize a CircularDict with a maximum length of 3
 my_buffer = CircularDict(maxlen=3)
 
@@ -69,15 +74,15 @@
 
 Output:
 ```bash
 When filling it: {'item1': 'value1', 'item2': 'value2', 'item3': 'value3'}
 After adding an element beyond maxlen: {'item2': 'value2', 'item3': 'value3', 'item4': 'value4'}
 ```
 
-#### Example with `maxsize_bytes`
+### Example with `maxsize_bytes`
 You can use `maxsize_bytes` to define the maximum amount of memory that the `dict` can store. It is particularly beneficial when defining **caches**, to prevent **memory overflows**.
 
 ```python
 from circular_dict import CircularDict
 import numpy as np
 import sys
```

### Comparing `circular-dict-1.3/README.md` & `circular-dict-1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,18 +9,23 @@
 
 ```bash
 pip install circular-dict
 ```
 
 ## Usage
 
-Working with **CircularDict** is as simple as using a standard Python `dict`, with additional parameters `maxlen` or `maxsize_bytes` on the initialization to control the buffer size. 
+Working with **CircularDict** is as simple as using a standard Python `dict`, with additional parameters `maxlen` or `maxsize_bytes` on the initialization to control the buffer size. You can use one of them or both.
+```python
+from circular_dict import CircularDict
+# Initialize a CircularDict with a maximum length of 3 items and a storage limit of 4Mb
+my_dict = CircularDict(maxlen=3, maxsize_bytes=4*1024*1024)
+```
 
-#### Example with `maxlen`
-You can use `maxlen` to define a maximum amount of items that the dictionary can store. It is useful for defining fixed size buffers.
+### Example with `maxlen`
+You can use `maxlen` to define the maximum amount of items that the dictionary can store. It is useful for defining fixed size buffers.
 
 ```python
 from circular_dict import CircularDict
 
 # Initialize a CircularDict with a maximum length of 3
 my_buffer = CircularDict(maxlen=3)
 
@@ -39,15 +44,15 @@
 
 Output:
 ```bash
 When filling it: {'item1': 'value1', 'item2': 'value2', 'item3': 'value3'}
 After adding an element beyond maxlen: {'item2': 'value2', 'item3': 'value3', 'item4': 'value4'}
 ```
 
-#### Example with `maxsize_bytes`
+### Example with `maxsize_bytes`
 You can use `maxsize_bytes` to define the maximum amount of memory that the `dict` can store. It is particularly beneficial when defining **caches**, to prevent **memory overflows**.
 
 ```python
 from circular_dict import CircularDict
 import numpy as np
 import sys
```

### Comparing `circular-dict-1.3/circular_dict/CircularDict.py` & `circular-dict-1.4/circular_dict/CircularDict.py`

 * *Files identical despite different names*

### Comparing `circular-dict-1.3/circular_dict.egg-info/PKG-INFO` & `circular-dict-1.4/circular_dict.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circular-dict
-Version: 1.3
+Version: 1.4
 Summary: CircularDict is a high-performance Python data structure that blends the functionality of dictionaries and circular buffers. Inheriting the usage of traditional dictionaries, it allows you to define constraints on size and memory usage. This way, the CircularDict will be always up-to-date with the last N added elements, ensuring that neither the maximum length nor the memory usage limit is exceeded. It is ideal for caching large data structures while maintaining control over memory footprint. 
 Home-page: https://github.com/Eric-Canas/CircularDict
 Author: Eric-Canas
 Author-email: eric@ericcanas.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -39,18 +39,23 @@
 
 ```bash
 pip install circular-dict
 ```
 
 ## Usage
 
-Working with **CircularDict** is as simple as using a standard Python `dict`, with additional parameters `maxlen` or `maxsize_bytes` on the initialization to control the buffer size. 
+Working with **CircularDict** is as simple as using a standard Python `dict`, with additional parameters `maxlen` or `maxsize_bytes` on the initialization to control the buffer size. You can use one of them or both.
+```python
+from circular_dict import CircularDict
+# Initialize a CircularDict with a maximum length of 3 items and a storage limit of 4Mb
+my_dict = CircularDict(maxlen=3, maxsize_bytes=4*1024*1024)
+```
 
-#### Example with `maxlen`
-You can use `maxlen` to define a maximum amount of items that the dictionary can store. It is useful for defining fixed size buffers.
+### Example with `maxlen`
+You can use `maxlen` to define the maximum amount of items that the dictionary can store. It is useful for defining fixed size buffers.
 
 ```python
 from circular_dict import CircularDict
 
 # Initialize a CircularDict with a maximum length of 3
 my_buffer = CircularDict(maxlen=3)
 
@@ -69,15 +74,15 @@
 
 Output:
 ```bash
 When filling it: {'item1': 'value1', 'item2': 'value2', 'item3': 'value3'}
 After adding an element beyond maxlen: {'item2': 'value2', 'item3': 'value3', 'item4': 'value4'}
 ```
 
-#### Example with `maxsize_bytes`
+### Example with `maxsize_bytes`
 You can use `maxsize_bytes` to define the maximum amount of memory that the `dict` can store. It is particularly beneficial when defining **caches**, to prevent **memory overflows**.
 
 ```python
 from circular_dict import CircularDict
 import numpy as np
 import sys
```

### Comparing `circular-dict-1.3/setup.py` & `circular-dict-1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='circular-dict',
-    version='1.3',
+    version='1.4',
     author='Eric-Canas',
     author_email='eric@ericcanas.com',
     url='https://github.com/Eric-Canas/CircularDict',
     description='CircularDict is a high-performance Python data structure that blends the functionality of dictionaries and circular buffers. '
                 'Inheriting the usage of traditional dictionaries, it allows you to define constraints on size and memory usage. '
                 'This way, the CircularDict will be always up-to-date with the last N added elements, ensuring that neither the maximum length nor '
                 'the memory usage limit is exceeded. It is ideal for caching large data structures while maintaining control over memory footprint. ',
```

