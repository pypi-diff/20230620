# Comparing `tmp/circular-dict-1.1.tar.gz` & `tmp/circular-dict-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circular-dict-1.1.tar", last modified: Mon Jun 19 13:56:52 2023, max compression
+gzip compressed data, was "circular-dict-1.2.tar", last modified: Mon Jun 19 23:36:11 2023, max compression
```

## Comparing `circular-dict-1.1.tar` & `circular-dict-1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 13:56:52.329385 circular-dict-1.1/
--rw-rw-rw-   0        0        0     1089 2023-06-19 11:41:28.000000 circular-dict-1.1/LICENSE
--rw-rw-rw-   0        0        0     1904 2023-06-19 13:56:52.328397 circular-dict-1.1/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-06-19 11:42:48.000000 circular-dict-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 13:56:52.313909 circular-dict-1.1/circular_dict/
--rw-rw-rw-   0        0        0     4788 2023-06-19 13:55:47.000000 circular-dict-1.1/circular_dict/CircularDict.py
--rw-rw-rw-   0        0        0       38 2023-06-19 12:09:31.000000 circular-dict-1.1/circular_dict/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 13:56:52.327376 circular-dict-1.1/circular_dict.egg-info/
--rw-rw-rw-   0        0        0     1904 2023-06-19 13:56:52.000000 circular-dict-1.1/circular_dict.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-06-19 13:56:52.000000 circular-dict-1.1/circular_dict.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 13:56:52.000000 circular-dict-1.1/circular_dict.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-19 13:56:52.000000 circular-dict-1.1/circular_dict.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 13:56:52.329385 circular-dict-1.1/setup.cfg
--rw-rw-rw-   0        0        0     1863 2023-06-19 13:56:49.000000 circular-dict-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:36:11.860331 circular-dict-1.2/
+-rw-rw-rw-   0        0        0     1089 2023-06-19 11:41:28.000000 circular-dict-1.2/LICENSE
+-rw-rw-rw-   0        0        0     5685 2023-06-19 23:36:11.859329 circular-dict-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4018 2023-06-19 23:35:50.000000 circular-dict-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 23:36:11.831329 circular-dict-1.2/circular_dict/
+-rw-rw-rw-   0        0        0     4798 2023-06-19 23:35:50.000000 circular-dict-1.2/circular_dict/CircularDict.py
+-rw-rw-rw-   0        0        0       38 2023-06-19 12:09:31.000000 circular-dict-1.2/circular_dict/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:36:11.857327 circular-dict-1.2/circular_dict.egg-info/
+-rw-rw-rw-   0        0        0     5685 2023-06-19 23:36:11.000000 circular-dict-1.2/circular_dict.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-06-19 23:36:11.000000 circular-dict-1.2/circular_dict.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 23:36:11.000000 circular-dict-1.2/circular_dict.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-19 23:36:11.000000 circular-dict-1.2/circular_dict.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 23:36:11.860331 circular-dict-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1863 2023-06-19 23:35:50.000000 circular-dict-1.2/setup.py
```

### Comparing `circular-dict-1.1/LICENSE` & `circular-dict-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `circular-dict-1.1/circular_dict/CircularDict.py` & `circular-dict-1.2/circular_dict/CircularDict.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,75 +32,75 @@
         :param maxsize_bytes: Optional[int]. Maximum size of items in the dictionary in bytes.
         :param args: Positional arguments passed to OrderedDict.
         :param kwargs: Keyword arguments passed to OrderedDict.
         """
         assert maxlen is not None or maxsize_bytes is not None, "Either maxlen or maxsize must be set"
         self.maxlen = maxlen
         self.maxsize_bytes = maxsize_bytes
-        self.currentsize = 0
+        self.current_size = 0
         super().__init__(*args, **kwargs)
 
     def is_empty(self) -> bool:
         """
         Check if the dictionary is empty.
 
         :return: bool. True if empty, False otherwise.
         """
         empty = len(self) == 0
         if empty:
-            assert self.currentsize == 0, f"currentsize must be 0 when the dictionary is empty. currentsize={self.currentsize}"
+            assert self.current_size == 0, f"currentsize must be 0 when the dictionary is empty. currentsize={self.current_size}"
         return empty
 
     def is_full(self) -> bool:
         """
         Check if the dictionary is full. A full dictionary will remove the oldest item when a new item is added.
 
         :return: bool. True if full, False otherwise.
         """
         if self.maxsize_bytes is not None:
-            assert self.currentsize <= self.maxsize_bytes, f"currentsize must be less than or equal to maxsize. currentsize={self.currentsize}, maxsize={self.maxsize_bytes}"
+            assert self.current_size <= self.maxsize_bytes, f"currentsize must be less than or equal to maxsize. currentsize={self.current_size}, maxsize={self.maxsize_bytes}"
 
         if self.maxlen is not None:
             assert len(self) <= self.maxlen, f"len(self) must be less than or equal to self.maxlen. len(self)={len(self)}, self.maxlen={self.maxlen}"
 
-        return (self.maxlen is not None and len(self) == self.maxlen) or (self.maxsize_bytes is not None and self.currentsize == self.maxsize_bytes)
+        return (self.maxlen is not None and len(self) == self.maxlen) or (self.maxsize_bytes is not None and self.current_size == self.maxsize_bytes)
 
     def __setitem__(self, key: Any, value: Any):
         """
         Set an item in the dictionary. If the key already exists, it will update the value.
         If the dictionary exceeds maxlen or maxsize, it will remove the oldest item until it no longer does.
 
         :param key: Any. Key to set or update. (It must be hashable)
         :param value: Any. Value to associate with the key.
         """
         item_size = sys.getsizeof(key) + sys.getsizeof(value)
 
         # If the element could not fit in the empty dictionary, raise an error
         if self.maxsize_bytes is not None:
             if item_size > self.maxsize_bytes:
-                raise ValueError(f"Item size {item_size} is larger than maxsize {self.maxsize_bytes}")
+                raise MemoryError(f"Item size {item_size} is larger than maxsize {self.maxsize_bytes}")
 
         # Delete the previous item if it exists to update the size accurately
         if key in self:
             del self[key]
 
         # Keep removing oldest items until there's enough space
-        while self.maxsize_bytes is not None and self.currentsize + item_size > self.maxsize_bytes:
+        while self.maxsize_bytes is not None and self.current_size + item_size > self.maxsize_bytes:
             self.popitem(last=False)
         # Keep removing oldest items until there's
         while self.maxlen is not None and len(self) >= self.maxlen:
             assert len(self) == self.maxlen, f"len(self) must be equal to self.maxlen. len(self)={len(self)}, self.maxlen={self.maxlen}"
             self.popitem(last=False)
 
         OrderedDict.__setitem__(self, key, value)
-        self.currentsize += item_size  # add size of new item
+        self.current_size += item_size  # add size of new item
 
     def __delitem__(self, key: Any):
         """
         Delete an item from the dictionary.
 
         :param key: Any. The key of the item to delete.
         """
         if key in self:
             value = self[key]
-            self.currentsize -= sys.getsizeof(key) + sys.getsizeof(value)
+            self.current_size -= sys.getsizeof(key) + sys.getsizeof(value)
             OrderedDict.__delitem__(self, key)
```

### Comparing `circular-dict-1.1/setup.py` & `circular-dict-1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='circular-dict',
-    version='1.1',
+    version='1.2',
     author='Eric-Canas',
     author_email='eric@ericcanas.com',
     url='https://github.com/Eric-Canas/CircularDict',
     description='CircularDict is a high-performance Python data structure that blends the functionality of dictionaries and circular buffers. '
                 'Inheriting the usage of traditional dictionaries, it allows you to define constraints on size and memory usage. '
                 'This way, the CircularDict will be always up-to-date with the last N added elements, ensuring that neither the maximum length nor '
                 'the memory usage limit is exceeded. It is ideal for caching large data structures while maintaining control over memory footprint. ',
```

