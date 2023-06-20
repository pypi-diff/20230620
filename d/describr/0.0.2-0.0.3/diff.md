# Comparing `tmp/describr-0.0.2.tar.gz` & `tmp/describr-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "describr-0.0.2.tar", last modified: Tue Jun 20 16:47:25 2023, max compression
+gzip compressed data, was "describr-0.0.3.tar", last modified: Tue Jun 20 17:20:00 2023, max compression
```

## Comparing `describr-0.0.2.tar` & `describr-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 16:47:25.585224 describr-0.0.2/
--rw-rw-rw-   0        0        0     1099 2023-06-20 15:03:20.000000 describr-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     4995 2023-06-20 16:47:25.585224 describr-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3740 2023-06-20 15:28:09.000000 describr-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 16:47:25.568150 describr-0.0.2/describr/
--rw-rw-rw-   0        0        0      129 2023-06-20 16:29:45.000000 describr-0.0.2/describr/__init__.py
--rw-rw-rw-   0        0        0    16616 2023-06-20 14:40:14.000000 describr-0.0.2/describr/describr.py
-drwxrwxrwx   0        0        0        0 2023-06-20 16:47:25.583223 describr-0.0.2/describr.egg-info/
--rw-rw-rw-   0        0        0     4995 2023-06-20 16:47:25.000000 describr-0.0.2/describr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-06-20 16:47:25.000000 describr-0.0.2/describr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 16:47:25.000000 describr-0.0.2/describr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-20 16:47:25.000000 describr-0.0.2/describr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-20 16:47:25.000000 describr-0.0.2/describr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 16:47:25.585224 describr-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1613 2023-06-20 16:47:09.000000 describr-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 17:20:00.646918 describr-0.0.3/
+-rw-rw-rw-   0        0        0     1099 2023-06-20 15:03:20.000000 describr-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     4995 2023-06-20 17:20:00.645918 describr-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3740 2023-06-20 15:28:09.000000 describr-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 17:20:00.628884 describr-0.0.3/describr/
+-rw-rw-rw-   0        0        0      129 2023-06-20 17:14:14.000000 describr-0.0.3/describr/__init__.py
+-rw-rw-rw-   0        0        0    16621 2023-06-20 17:14:07.000000 describr-0.0.3/describr/describr.py
+drwxrwxrwx   0        0        0        0 2023-06-20 17:20:00.644916 describr-0.0.3/describr.egg-info/
+-rw-rw-rw-   0        0        0     4995 2023-06-20 17:20:00.000000 describr-0.0.3/describr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-06-20 17:20:00.000000 describr-0.0.3/describr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 17:20:00.000000 describr-0.0.3/describr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-20 17:20:00.000000 describr-0.0.3/describr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-20 17:20:00.000000 describr-0.0.3/describr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 17:20:00.646918 describr-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1613 2023-06-20 17:19:03.000000 describr-0.0.3/setup.py
```

### Comparing `describr-0.0.2/LICENSE` & `describr-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `describr-0.0.2/PKG-INFO` & `describr-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: describr
-Version: 0.0.2
+Version: 0.0.3
 Summary: Describr is a Python library that provides a convenient way to generate descriptive statistics for datasets.
 Home-page: https://github.com/famutimine/describr
 Author: Daniel Famutimi MD, MPH
 Author-email: danielfamutimi@gmail.com
 License: MIT
 Keywords: descriptive statistics
 Platform: UNKNOWN
```

### Comparing `describr-0.0.2/README.md` & `describr-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `describr-0.0.2/describr/describr.py` & `describr-0.0.3/describr/describr.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,15 @@
         column_order.insert(2, positive_class_columns[1])
         df_continuous = df_continuous[column_order]
 
         return df_continuous
 
     def _compute_continuous_stats_with_median(self, continuous_vars):
         continuous_vars.append(self.group_col)
-        continuous_median = df[continuous_vars].groupby(self.group_col).agg(['median', lambda x: x.quantile(0.25), lambda x: x.quantile(0.75)])
+        continuous_median = self.df[continuous_vars].groupby(self.group_col).agg(['median', lambda x: x.quantile(0.25), lambda x: x.quantile(0.75)])
         treatment_values = self.df[self.group_col].unique()
         continuous_median = continuous_median.T
         continuous_median.reset_index(inplace=True)
         new_columns = {'level_0': 'variable', 'level_1': 'stats'}
         continuous_median = continuous_median.rename(columns=new_columns)
         continuous_median['stats'] = continuous_median['stats'].replace({'<lambda_0>': 'Q1', '<lambda_1>': 'Q3'})
         continuous_median = continuous_median.rename(columns={col: self.group_col + '_' + str(col) + '_median' for col in continuous_median.columns[-2:]})
```

### Comparing `describr-0.0.2/describr.egg-info/PKG-INFO` & `describr-0.0.3/describr.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: describr
-Version: 0.0.2
+Version: 0.0.3
 Summary: Describr is a Python library that provides a convenient way to generate descriptive statistics for datasets.
 Home-page: https://github.com/famutimine/describr
 Author: Daniel Famutimi MD, MPH
 Author-email: danielfamutimi@gmail.com
 License: MIT
 Keywords: descriptive statistics
 Platform: UNKNOWN
```

### Comparing `describr-0.0.2/setup.py` & `describr-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from urllib.request import urlopen
 
 with urlopen("https://raw.githubusercontent.com/famutimine/describr/main/README.md") as fh:
     long_description = fh.read().decode()
 
 setuptools.setup(
     name='describr',
-    version='0.0.2',
+    version='0.0.3',
     description='Describr is a Python library that provides a convenient way to generate descriptive statistics for datasets.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/famutimine/describr',
     author='Daniel Famutimi MD, MPH',
     author_email='danielfamutimi@gmail.com',
     license='MIT',
```

