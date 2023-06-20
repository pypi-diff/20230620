# Comparing `tmp/ANBUtils-1.6.1.tar.gz` & `tmp/ANBUtils-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ANBUtils-1.6.1.tar", last modified: Tue Jun 13 11:16:39 2023, max compression
+gzip compressed data, was "dist/ANBUtils-1.6.2.tar", last modified: Tue Jun 20 12:52:37 2023, max compression
```

## Comparing `ANBUtils-1.6.1.tar` & `ANBUtils-1.6.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-13 11:16:39.215887 ANBUtils-1.6.1/
-drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-13 11:16:39.214067 ANBUtils-1.6.1/ANBUtils/
--rw-r--r--   0 redbson    (501) staff       (20)      881 2023-06-13 06:10:43.000000 ANBUtils-1.6.1/ANBUtils/__init__.py
--rw-r--r--   0 redbson    (501) staff       (20)     2484 2023-06-13 05:24:45.000000 ANBUtils-1.6.1/ANBUtils/a.py
--rw-r--r--   0 redbson    (501) staff       (20)    12407 2023-06-13 11:01:13.000000 ANBUtils-1.6.1/ANBUtils/db_worker.py
--rw-r--r--   0 redbson    (501) staff       (20)      932 2023-06-06 05:14:52.000000 ANBUtils-1.6.1/ANBUtils/easy_pickle.py
--rw-r--r--   0 redbson    (501) staff       (20)      890 2023-06-13 10:59:29.000000 ANBUtils-1.6.1/ANBUtils/environ_cheker.py
--rw-r--r--   0 redbson    (501) staff       (20)     3520 2023-06-13 11:04:14.000000 ANBUtils-1.6.1/ANBUtils/id_work.py
--rw-r--r--   0 redbson    (501) staff       (20)     1954 2023-06-13 04:36:50.000000 ANBUtils-1.6.1/ANBUtils/messenger.py
--rw-r--r--   0 redbson    (501) staff       (20)     4021 2023-06-06 05:17:20.000000 ANBUtils-1.6.1/ANBUtils/tbox.py
-drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-13 11:16:39.215423 ANBUtils-1.6.1/ANBUtils.egg-info/
--rw-r--r--   0 redbson    (501) staff       (20)     5284 2023-06-13 11:16:39.000000 ANBUtils-1.6.1/ANBUtils.egg-info/PKG-INFO
--rw-r--r--   0 redbson    (501) staff       (20)      344 2023-06-13 11:16:39.000000 ANBUtils-1.6.1/ANBUtils.egg-info/SOURCES.txt
--rw-r--r--   0 redbson    (501) staff       (20)        1 2023-06-13 11:16:39.000000 ANBUtils-1.6.1/ANBUtils.egg-info/dependency_links.txt
--rw-r--r--   0 redbson    (501) staff       (20)      108 2023-06-13 11:16:39.000000 ANBUtils-1.6.1/ANBUtils.egg-info/requires.txt
--rw-r--r--   0 redbson    (501) staff       (20)        9 2023-06-13 11:16:39.000000 ANBUtils-1.6.1/ANBUtils.egg-info/top_level.txt
--rw-r--r--   0 redbson    (501) staff       (20)     5284 2023-06-13 11:16:39.215688 ANBUtils-1.6.1/PKG-INFO
--rw-r--r--   0 redbson    (501) staff       (20)     4894 2023-06-13 11:16:05.000000 ANBUtils-1.6.1/README.md
--rw-r--r--   0 redbson    (501) staff       (20)       38 2023-06-13 11:16:39.215978 ANBUtils-1.6.1/setup.cfg
--rw-r--r--   0 redbson    (501) staff       (20)      917 2023-06-13 11:11:14.000000 ANBUtils-1.6.1/setup.py
+drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-20 12:52:37.094656 ANBUtils-1.6.2/
+drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-20 12:52:37.090532 ANBUtils-1.6.2/ANBUtils/
+-rw-r--r--   0 redbson    (501) staff       (20)      157 2023-06-20 12:51:49.000000 ANBUtils-1.6.2/ANBUtils/__info__.py
+-rw-r--r--   0 redbson    (501) staff       (20)      829 2023-06-20 12:48:41.000000 ANBUtils-1.6.2/ANBUtils/__init__.py
+-rw-r--r--   0 redbson    (501) staff       (20)     3129 2023-06-20 12:35:47.000000 ANBUtils-1.6.2/ANBUtils/a.py
+-rw-r--r--   0 redbson    (501) staff       (20)    12409 2023-06-16 06:57:29.000000 ANBUtils-1.6.2/ANBUtils/db_worker.py
+-rw-r--r--   0 redbson    (501) staff       (20)      932 2023-06-06 05:14:52.000000 ANBUtils-1.6.2/ANBUtils/easy_pickle.py
+-rw-r--r--   0 redbson    (501) staff       (20)      890 2023-06-13 10:59:29.000000 ANBUtils-1.6.2/ANBUtils/environ_cheker.py
+-rw-r--r--   0 redbson    (501) staff       (20)     3520 2023-06-13 11:04:14.000000 ANBUtils-1.6.2/ANBUtils/id_work.py
+-rw-r--r--   0 redbson    (501) staff       (20)     1954 2023-06-13 04:36:50.000000 ANBUtils-1.6.2/ANBUtils/messenger.py
+-rw-r--r--   0 redbson    (501) staff       (20)     4021 2023-06-06 05:17:20.000000 ANBUtils-1.6.2/ANBUtils/tbox.py
+drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-20 12:52:37.094204 ANBUtils-1.6.2/ANBUtils.egg-info/
+-rw-r--r--   0 redbson    (501) staff       (20)     5322 2023-06-20 12:52:37.000000 ANBUtils-1.6.2/ANBUtils.egg-info/PKG-INFO
+-rw-r--r--   0 redbson    (501) staff       (20)      365 2023-06-20 12:52:37.000000 ANBUtils-1.6.2/ANBUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 redbson    (501) staff       (20)        1 2023-06-20 12:52:37.000000 ANBUtils-1.6.2/ANBUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 redbson    (501) staff       (20)      108 2023-06-20 12:52:37.000000 ANBUtils-1.6.2/ANBUtils.egg-info/requires.txt
+-rw-r--r--   0 redbson    (501) staff       (20)        9 2023-06-20 12:52:37.000000 ANBUtils-1.6.2/ANBUtils.egg-info/top_level.txt
+-rw-r--r--   0 redbson    (501) staff       (20)     5322 2023-06-20 12:52:37.094475 ANBUtils-1.6.2/PKG-INFO
+-rw-r--r--   0 redbson    (501) staff       (20)     4894 2023-06-13 11:16:05.000000 ANBUtils-1.6.2/README.md
+-rw-r--r--   0 redbson    (501) staff       (20)       38 2023-06-20 12:52:37.094728 ANBUtils-1.6.2/setup.cfg
+-rw-r--r--   0 redbson    (501) staff       (20)      869 2023-06-20 12:52:13.000000 ANBUtils-1.6.2/setup.py
```

### Comparing `ANBUtils-1.6.1/ANBUtils/__init__.py` & `ANBUtils-1.6.2/ANBUtils/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-__title__ = 'ANBUtils'
-__author__ = 'redbson'
-__email__ = 'redbson@gmail.com'
+
+from .__info__ import *
+
 
 from .environ_cheker import environment_checker as _checker
 _checker()
 
 
 
 from .a import (
```

### Comparing `ANBUtils-1.6.1/ANBUtils/a.py` & `ANBUtils-1.6.2/ANBUtils/a.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+import warnings
+
+import dtale
+
+
 def print_rate_progress(n, s, step=0.02, message=''):
     """
     打印进度条及百分比。
 
     参数：
     n (int): 当前进度。
     s (int): 总进度。
@@ -11,16 +16,16 @@
     返回：
     无
 
     """
     if step >= 1:
         step = 0.1
     r = n / s
-    t = int(r / step)
-    print("\r%s%s %.2f%% %s" % ('-' * t, '*' * (50 - t), r * 100, message), end="")
+    t = int( r / step )
+    print( "\r%s%s %.2f%% %s" % ('-' * t, '*' * (50 - t), r * 100, message), end="" )
 
 
 def set_date_index(df, key):
     """
     将DataFrame的某一列转换为日期索引。
 
     参数：
@@ -28,91 +33,109 @@
     key (str): 日期列的名称。
 
     返回：
     pandas.DataFrame: 转换后的DataFrame。
 
     """
     import pandas as pd
-    data = [pd.Timestamp(i) for i in df[key]]
+    data = [pd.Timestamp( i ) for i in df[key]]
     del df[key]
-    idx = pd.DatetimeIndex(data)
-    df.set_index(idx, inplace=True)
+    idx = pd.DatetimeIndex( data )
+    df.set_index( idx, inplace=True )
     return df
 
 
 def digit(obj):
     """
     将数字格式化为可读性更好的字符串表示。
 
     参数：
     obj (int or float): 需要格式化的数字。
 
     返回：
     tuple: 格式化后的字符串和数字的位数。
 
     """
+
     def _f(x):
         if x < 1000:
             return x
 
         d = ('', 'K', 'M', 'B', 'T')
-        for i in range(1, 5):
+        for i in range( 1, 5 ):
             x /= 1000
             if x < 1:
                 return "%.2f%s" % (x * 1000, d[i - 1])
         return "%.2f%s" % (x, d[-1])
 
-    return len(str(obj)), _f(obj)
+    return len( str( obj ) ), _f( obj )
 
 
 def count(x):
     """
     计算列表的长度，并将长度格式化为可读性更好的字符串表示。
 
     参数：
     x (list): 需要计算长度的列表。
 
     返回：
     str: 格式化后的字符串。
 
     """
-    length = len(x)
-    return digit(length)[1]
+    length = len( x )
+    return digit( length )[1]
 
 
 def value(s):
     """
     从字符串中提取数字。
 
     参数：
     s (str): 需要提取数字的字符串。
 
     返回：
     list: 提取出的数字列表。
 
     """
-    if type(s) != str:
+    if type( s ) != str:
         return [0]
     import re
-    t = re.findall(r"\d+\.?\d*", s)
-    return [float(i) for i in t]
+    t = re.findall( r"\d+\.?\d*", s )
+    return [float( i ) for i in t]
 
 
 def count2int(x):
     """
     将带有单位的数字字符串转换为对应的整数。
 
     参数：
     x (int or str): 需要转换的数字或字符串。
 
     返回：
     int: 转换后的整数。
 
     """
     _d = {'K': 1000, 'M': 1000000, 'B': 1000000000, 'T': 1000000000000}
-    if isinstance(x, str):
+    if isinstance( x, str ):
         if x[-1] in _d.keys():
-            x = float(x[:-1]) * _d[x[-1]]
+            x = float( x[:-1] ) * _d[x[-1]]
         else:
             return 0
     return x
 
+
+def data_browser(df, sample_size=0):
+    max_sample_size = 1_000_000
+
+    if sample_size > 0:
+        if len( df ) >= sample_size > max_sample_size:
+            warnings.warn( "Data sample size is too large, automatically adjusting to 1 million.", Warning )
+            data = df.sample( n=max_sample_size )
+        elif sample_size > len( df ):
+            warnings.warn( "Data sample size is larger than data size, automatically adjusting to data size.", Warning )
+            data = df
+    else:
+        data = df
+
+    d = dtale.show( data )
+    d.open_browser()
+    return d
```

### Comparing `ANBUtils-1.6.1/ANBUtils/db_worker.py` & `ANBUtils-1.6.2/ANBUtils/db_worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,16 +165,16 @@
             dfs = []
             for i in range( n ):
                 if verbose:
                     print( 'processing {i:>2d} part ...'.format( i=i + 1 ) )
                 _df = self._to_df_base( col, match=match, projection=projection, skip=i * step, limit=step )
                 dfs.append( _df )
             df = pd.concat( dfs )
-            df.drop_duplicates( subset=['_id'], inplace=True )
-            df.reset_index( inplace=True, drop=True )
+            #df.drop_duplicates( subset=['_id'], inplace=True )
+            #df.reset_index( inplace=True, drop=True )
             if verbose:
                 print( 'done' )
 
         else:
             if verbose:
                 print( '{col} has {count:,d} records, {size:,.2f} MB, processing ...'.format( col=col, count=st_count,
                                                                                               size=st_size ) )
```

### Comparing `ANBUtils-1.6.1/ANBUtils/easy_pickle.py` & `ANBUtils-1.6.2/ANBUtils/easy_pickle.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.6.1/ANBUtils/environ_cheker.py` & `ANBUtils-1.6.2/ANBUtils/environ_cheker.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.6.1/ANBUtils/id_work.py` & `ANBUtils-1.6.2/ANBUtils/id_work.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.6.1/ANBUtils/messenger.py` & `ANBUtils-1.6.2/ANBUtils/messenger.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.6.1/ANBUtils/tbox.py` & `ANBUtils-1.6.2/ANBUtils/tbox.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.6.1/ANBUtils.egg-info/PKG-INFO` & `ANBUtils-1.6.2/ANBUtils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: ANBUtils
-Version: 1.6.1
+Version: 1.6.2
 Summary: ANBUilts is a versatile Python package that offers a comprehensive set of utility functions and tools for data analysis, database operations, and messaging integration.
 Home-page: https://github.com/redbson/ANBUtils
-Author: redbson
+Author: Yafei Hou
 Author-email: redbson@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # ANBUtils
 
 ANBUtils is a Python package that provides various utility functions for common tasks in data analysis and database operations. It includes functions for working with MongoDB, sending messages via DingTalk, and handling date and time operations.
 
@@ -143,7 +145,8 @@
 ANBUtils is an open-source project, and contributions are welcome. If you encounter any issues or have suggestions for improvements, please feel free to open an issue on the [GitHub repository](https://github.com/example-user/ANBUtils).
 
 For support or general questions, you can reach out to the project maintainers or the community through the GitHub repository.
 
 ## License
 
 ANBUtils is released under the [MIT License](https://opensource.org/licenses/MIT). Please refer to the LICENSE file for more details.
+
```

### Comparing `ANBUtils-1.6.1/PKG-INFO` & `ANBUtils-1.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: ANBUtils
-Version: 1.6.1
+Version: 1.6.2
 Summary: ANBUilts is a versatile Python package that offers a comprehensive set of utility functions and tools for data analysis, database operations, and messaging integration.
 Home-page: https://github.com/redbson/ANBUtils
-Author: redbson
+Author: Yafei Hou
 Author-email: redbson@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # ANBUtils
 
 ANBUtils is a Python package that provides various utility functions for common tasks in data analysis and database operations. It includes functions for working with MongoDB, sending messages via DingTalk, and handling date and time operations.
 
@@ -143,7 +145,8 @@
 ANBUtils is an open-source project, and contributions are welcome. If you encounter any issues or have suggestions for improvements, please feel free to open an issue on the [GitHub repository](https://github.com/example-user/ANBUtils).
 
 For support or general questions, you can reach out to the project maintainers or the community through the GitHub repository.
 
 ## License
 
 ANBUtils is released under the [MIT License](https://opensource.org/licenses/MIT). Please refer to the LICENSE file for more details.
+
```

### Comparing `ANBUtils-1.6.1/README.md` & `ANBUtils-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.6.1/setup.py` & `ANBUtils-1.6.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from setuptools import setup, find_packages
+import ANBUtils.__info__ as info
+
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
-with open('version', 'r', encoding='utf-8') as f:
-    version = f.read()
-
-
 
 setup(
     name="ANBUtils",
-    version=version,
+    version=info.__version__,
     packages=find_packages(),
-    author="redbson",
-    author_email="redbson@gmail.com",
-    url="https://github.com/redbson/ANBUtils",
+    author=info.__author__,
+    author_email=info.__author_email__,
+    url= info.__url__,
     description = "ANBUilts is a versatile Python package that offers a comprehensive set of utility functions and tools for data analysis, database operations, and messaging integration.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     python_requires='>=3.8',
     install_requires=[
         "matplotlib>=3.0.0",
         "numpy>=1.0.0",
```

