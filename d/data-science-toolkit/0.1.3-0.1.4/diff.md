# Comparing `tmp/data-science-toolkit-0.1.3.tar.gz` & `tmp/data-science-toolkit-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-science-toolkit-0.1.3.tar", last modified: Fri Jun 16 11:02:33 2023, max compression
+gzip compressed data, was "data-science-toolkit-0.1.4.tar", last modified: Tue Jun 20 03:16:54 2023, max compression
```

## Comparing `data-science-toolkit-0.1.3.tar` & `data-science-toolkit-0.1.4.tar`

### file list

```diff
@@ -1,29 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 11:02:33.077655 data-science-toolkit-0.1.3/
--rw-rw-rw-   0        0        0     1096 2022-03-25 12:00:42.000000 data-science-toolkit-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     1963 2023-06-16 11:02:33.076655 data-science-toolkit-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1355 2022-04-14 01:06:21.000000 data-science-toolkit-0.1.3/README.md
--rw-rw-rw-   0        0        0      387 2022-03-25 12:00:42.000000 data-science-toolkit-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-16 11:02:33.078654 data-science-toolkit-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1434 2023-06-16 10:57:42.000000 data-science-toolkit-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-16 11:02:32.878657 data-science-toolkit-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-16 11:02:32.962655 data-science-toolkit-0.1.3/src/data_science_toolkit/
--rw-rw-rw-   0        0        0        0 2022-03-25 12:00:42.000000 data-science-toolkit-0.1.3/src/data_science_toolkit/__init__.py
--rw-rw-rw-   0        0        0    10268 2022-03-25 12:00:42.000000 data-science-toolkit-0.1.3/src/data_science_toolkit/chart.py
--rw-rw-rw-   0        0        0     6375 2022-05-20 00:30:43.000000 data-science-toolkit-0.1.3/src/data_science_toolkit/csm.py
--rw-rw-rw-   0        0        0    77033 2023-06-16 10:57:32.000000 data-science-toolkit-0.1.3/src/data_science_toolkit/dataframe.py
--rw-rw-rw-   0        0        0    12467 2022-05-20 00:36:43.000000 data-science-toolkit-0.1.3/src/data_science_toolkit/gis.py
--rw-rw-rw-   0        0        0     8456 2022-03-25 12:00:42.000000 data-science-toolkit-0.1.3/src/data_science_toolkit/imagefactory.py
--rw-rw-rw-   0        0        0    25115 2023-05-13 00:40:51.000000 data-science-toolkit-0.1.3/src/data_science_toolkit/lib.py
--rw-rw-rw-   0        0        0    28669 2023-03-15 23:27:50.000000 data-science-toolkit-0.1.3/src/data_science_toolkit/model.py
--rw-rw-rw-   0        0        0     7636 2022-05-20 00:33:21.000000 data-science-toolkit-0.1.3/src/data_science_toolkit/r3.py
--rw-rw-rw-   0        0        0     4983 2021-02-01 01:53:23.000000 data-science-toolkit-0.1.3/src/data_science_toolkit/rl.py
--rw-rw-rw-   0        0        0     1445 2022-05-19 23:54:12.000000 data-science-toolkit-0.1.3/src/data_science_toolkit/rl_dqn.py
--rw-rw-rw-   0        0        0     5488 2023-03-15 23:28:40.000000 data-science-toolkit-0.1.3/src/data_science_toolkit/vectorizer.py
-drwxrwxrwx   0        0        0        0 2023-06-16 11:02:33.060655 data-science-toolkit-0.1.3/src/data_science_toolkit.egg-info/
--rw-rw-rw-   0        0        0     1963 2023-06-16 11:02:32.000000 data-science-toolkit-0.1.3/src/data_science_toolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      709 2023-06-16 11:02:32.000000 data-science-toolkit-0.1.3/src/data_science_toolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 11:02:32.000000 data-science-toolkit-0.1.3/src/data_science_toolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      209 2023-06-16 11:02:32.000000 data-science-toolkit-0.1.3/src/data_science_toolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-16 11:02:32.000000 data-science-toolkit-0.1.3/src/data_science_toolkit.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-16 11:02:33.073655 data-science-toolkit-0.1.3/test/
--rw-rw-rw-   0        0        0       85 2022-03-25 12:00:42.000000 data-science-toolkit-0.1.3/test/test.py
+drwxrwxrwx   0        0        0        0 2023-06-20 03:16:54.517604 data-science-toolkit-0.1.4/
+-rw-rw-rw-   0        0        0      136 2023-06-20 03:07:34.000000 data-science-toolkit-0.1.4/.gitignore
+-rw-rw-rw-   0        0        0      734 2023-06-20 03:07:34.000000 data-science-toolkit-0.1.4/.readthedocs.yaml
+-rw-rw-rw-   0        0        0     1096 2023-06-20 03:07:34.000000 data-science-toolkit-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     1963 2023-06-20 03:16:54.516605 data-science-toolkit-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1355 2023-06-20 03:07:34.000000 data-science-toolkit-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 03:16:54.468633 data-science-toolkit-0.1.4/docs/
+-rw-rw-rw-   0        0        0     2215 2023-06-20 03:07:34.000000 data-science-toolkit-0.1.4/docs/conf.py
+-rw-rw-rw-   0        0        0      970 2023-06-20 03:07:34.000000 data-science-toolkit-0.1.4/docs/dst.rst
+-rw-rw-rw-   0        0        0      412 2023-06-20 03:07:34.000000 data-science-toolkit-0.1.4/docs/index.rst
+-rw-rw-rw-   0        0        0       53 2023-06-20 03:07:34.000000 data-science-toolkit-0.1.4/docs/modules.rst
+-rw-rw-rw-   0        0        0     1974 2023-06-20 03:07:34.000000 data-science-toolkit-0.1.4/docs/requirements.txt
+-rw-rw-rw-   0        0        0      600 2023-06-20 03:07:34.000000 data-science-toolkit-0.1.4/dst_test.ipynb
+drwxrwxrwx   0        0        0        0 2023-06-20 03:16:54.470631 data-science-toolkit-0.1.4/media/
+-rw-rw-rw-   0        0        0   176934 2023-06-20 03:07:34.000000 data-science-toolkit-0.1.4/media/dst_logo.png
+-rw-rw-rw-   0        0        0      387 2023-06-20 03:07:34.000000 data-science-toolkit-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0     1636 2023-06-20 03:07:34.000000 data-science-toolkit-0.1.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 03:16:54.518604 data-science-toolkit-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1434 2023-06-20 03:08:31.000000 data-science-toolkit-0.1.4/setup.py
+-rw-rw-rw-   0        0        0      714 2023-06-20 03:07:34.000000 data-science-toolkit-0.1.4/setupp.cfg
+drwxrwxrwx   0        0        0        0 2023-06-20 03:16:54.443652 data-science-toolkit-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-20 03:16:54.496616 data-science-toolkit-0.1.4/src/data_science_toolkit/
+-rw-rw-rw-   0        0        0        0 2023-06-20 03:07:34.000000 data-science-toolkit-0.1.4/src/data_science_toolkit/__init__.py
+-rw-rw-rw-   0        0        0    10268 2023-06-20 03:07:34.000000 data-science-toolkit-0.1.4/src/data_science_toolkit/chart.py
+-rw-rw-rw-   0        0        0     6375 2023-06-20 03:07:34.000000 data-science-toolkit-0.1.4/src/data_science_toolkit/csm.py
+-rw-rw-rw-   0        0        0    79200 2023-06-20 03:08:20.000000 data-science-toolkit-0.1.4/src/data_science_toolkit/dataframe.py
+-rw-rw-rw-   0        0        0    12467 2023-06-20 03:07:34.000000 data-science-toolkit-0.1.4/src/data_science_toolkit/gis.py
+-rw-rw-rw-   0        0        0     8456 2023-06-20 03:07:34.000000 data-science-toolkit-0.1.4/src/data_science_toolkit/imagefactory.py
+-rw-rw-rw-   0        0        0    25115 2023-06-20 03:07:34.000000 data-science-toolkit-0.1.4/src/data_science_toolkit/lib.py
+-rw-rw-rw-   0        0        0    28669 2023-06-20 03:07:34.000000 data-science-toolkit-0.1.4/src/data_science_toolkit/model.py
+-rw-rw-rw-   0        0        0     7636 2023-06-20 03:07:34.000000 data-science-toolkit-0.1.4/src/data_science_toolkit/r3.py
+-rw-rw-rw-   0        0        0     4983 2023-06-20 03:07:34.000000 data-science-toolkit-0.1.4/src/data_science_toolkit/rl.py
+-rw-rw-rw-   0        0        0     1445 2023-06-20 03:07:34.000000 data-science-toolkit-0.1.4/src/data_science_toolkit/rl_dqn.py
+-rw-rw-rw-   0        0        0     5488 2023-06-20 03:07:34.000000 data-science-toolkit-0.1.4/src/data_science_toolkit/vectorizer.py
+drwxrwxrwx   0        0        0        0 2023-06-20 03:16:54.509609 data-science-toolkit-0.1.4/src/data_science_toolkit.egg-info/
+-rw-rw-rw-   0        0        0     1963 2023-06-20 03:16:54.000000 data-science-toolkit-0.1.4/src/data_science_toolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      896 2023-06-20 03:16:54.000000 data-science-toolkit-0.1.4/src/data_science_toolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 03:16:54.000000 data-science-toolkit-0.1.4/src/data_science_toolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      209 2023-06-20 03:16:54.000000 data-science-toolkit-0.1.4/src/data_science_toolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-20 03:16:54.000000 data-science-toolkit-0.1.4/src/data_science_toolkit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 03:16:54.513607 data-science-toolkit-0.1.4/test/
+-rw-rw-rw-   0        0        0      597 2023-06-20 03:07:34.000000 data-science-toolkit-0.1.4/test/kitchen.py
+-rw-rw-rw-   0        0        0       85 2023-06-20 03:07:34.000000 data-science-toolkit-0.1.4/test/test.py
```

### Comparing `data-science-toolkit-0.1.3/LICENSE` & `data-science-toolkit-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `data-science-toolkit-0.1.3/PKG-INFO` & `data-science-toolkit-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-science-toolkit
-Version: 0.1.3
+Version: 0.1.4
 Summary: Data Science Toolkit (DST) is a Python library that helps implement data science related project with ease.
 Home-page: https://github.com/elhachimi-ch/dst
 Author: EL HACHIMI CHOUAIB
 Author-email: elhachimi.ch@gmail.com
 Project-URL: Bug Tracker, https://github.com/elhachimi-ch/dst/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `data-science-toolkit-0.1.3/README.md` & `data-science-toolkit-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `data-science-toolkit-0.1.3/setup.py` & `data-science-toolkit-0.1.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
     
     
 setuptools.setup(
     name="data-science-toolkit",
-    version="0.1.03",
+    version="0.1.04",
     author="EL HACHIMI CHOUAIB",
     author_email="elhachimi.ch@gmail.com",
     description="Data Science Toolkit (DST) is a Python library that helps implement data science related project with ease.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/elhachimi-ch/dst",
     project_urls={
```

### Comparing `data-science-toolkit-0.1.3/src/data_science_toolkit/chart.py` & `data-science-toolkit-0.1.4/src/data_science_toolkit/chart.py`

 * *Files identical despite different names*

### Comparing `data-science-toolkit-0.1.3/src/data_science_toolkit/csm.py` & `data-science-toolkit-0.1.4/src/data_science_toolkit/csm.py`

 * *Files identical despite different names*

### Comparing `data-science-toolkit-0.1.3/src/data_science_toolkit/dataframe.py` & `data-science-toolkit-0.1.4/src/data_science_toolkit/dataframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,59 +25,59 @@
 
 class DataFrame:
     """
     """
     __vectorizer = None
     __generator = None
 
-    def __init__(self, data_link=None, columns_names_as_list=None, data_types_in_order=None, delimiter=',',
+    def __init__(self, data_path=None, columns_names_as_list=None, data_types_in_order=None, delimiter=',',
                  data_type='csv', has_header=True, line_index=None, skip_empty_line=False, sheet_name=0,
                  skip_rows=None, **kwargs
                  ):
         
-        if data_link is not None:
+        if data_path is not None:
             if data_type == 'csv':
                 if has_header is True:
-                    self.dataframe = pd.read_csv(data_link, encoding='utf-8', delimiter=delimiter, 
+                    self.dataframe = pd.read_csv(data_path, encoding='utf-8', delimiter=delimiter, 
                                                low_memory=False, on_bad_lines='skip', skip_blank_lines=False,
                                                skiprows=skip_rows, **kwargs)
                 else:
-                    self.dataframe = pd.read_csv(data_link, encoding='utf-8', delimiter=delimiter, 
+                    self.dataframe = pd.read_csv(data_path, encoding='utf-8', delimiter=delimiter, 
                                                low_memory=False, on_bad_lines='skip', skip_blank_lines=False,
-                                               header=None)
+                                               header=None, **kwargs)
             elif data_type == 'json':
-                self.dataframe = pd.read_json(data_link, encoding='utf-8')
+                self.dataframe = pd.read_json(data_path, encoding='utf-8')
             elif data_type == 'xls':
-                self.dataframe = pd.read_excel(data_link, sheet_name=sheet_name,
-                                                 skiprows=skip_rows)
+                self.dataframe = pd.read_excel(data_path, sheet_name=sheet_name,
+                                                 skiprows=skip_rows, **kwargs)
             elif data_type == 'pkl':
-                self.dataframe = pd.read_pickle(data_link)
+                self.dataframe = pd.read_pickle(data_path, **kwargs)
             elif data_type == 'dict':
-                self.dataframe = pd.DataFrame.from_dict(data_link)
+                self.dataframe = pd.DataFrame.from_dict(data_path, **kwargs)
             elif data_type == 'matrix':
-                index_name = [i for i in range(len(data_link))]
-                colums_name = [i for i in range(len(data_link[0]))]
-                self.dataframe = pd.DataFrame(data=data_link, index=index_name, columns=colums_name)
+                index_name = [i for i in range(len(data_path))]
+                colums_name = [i for i in range(len(data_path[0]))]
+                self.dataframe = pd.DataFrame(data=data_path, index=index_name, columns=colums_name, **kwargs)
             elif data_type == 'list':
-                y = data_link
+                y = data_path
                 if (not isinstance(y, pd.core.series.Series or not isinstance(y, pd.core.frame.DataFrame))):
                     y = np.array(y)
                     y = np.reshape(y, (y.shape[0],))
                     y = pd.Series(y)
                 self.dataframe = pd.DataFrame()
                 if columns_names_as_list is not None:
                     self.dataframe[columns_names_as_list[0]] = y
                 else:
                     self.dataframe['0'] = y
                     
                 
                 """data = array([['','Col1','Col2'],['Row1',1,2],['Row2',3,4]])
                 pd.DataFrame(data=data[1:,1:], index=data[1:,0], columns=data[0,1:]) """
             elif data_type == 'df':
-                self.dataframe = data_link
+                self.dataframe = data_path
             types = {}
             if data_types_in_order is not None and columns_names_as_list is not None:
                 self.dataframe.columns = columns_names_as_list
                 for i in range(len(columns_names_as_list)):
                     types[columns_names_as_list[i]] = data_types_in_order[i]
             elif columns_names_as_list is not None:
                 self.dataframe.columns = columns_names_as_list
@@ -98,15 +98,15 @@
         if isinstance(language_or_stopwords_list, list) is True:
             stopwords = language_or_stopwords_list
         elif language_or_stopwords_list == 'arabic':
             stopwords = Lib.read_text_file_as_list('data/arabic_stopwords.csv')
         else:
             nltk.download('stopwords')
             stopwords = nltk.corpus.stopwords.words(language_or_stopwords_list)
-        self.transform_column(column, column, DataFrame.remove_stopwords_lambda, in_place, stopwords)
+        self.transform_column(column, DataFrame.remove_stopwords_lambda, in_place, stopwords)
         return self.dataframe
     
     @staticmethod
     def remove_stopwords_lambda(document, stopwords_list):
         document = str.lower(document)
         stopwords = stopwords_list
         words = word_tokenize(document)
@@ -160,14 +160,17 @@
         if data_type == 'matrix':
             index_name = [i for i in range(len(data))]
             colums_name = [i for i in range(len(data[0]))]
             self.dataframe = pd.DataFrame(data=data, index=index_name, columns=colums_name)
         elif data_type == 'df':
             self.dataframe = data
 
+    def is_empty(self):
+        return self.get_shape()[0] == 0
+    
     def get_columns_types(self, show=True):
         types = self.get_dataframe().dtypes
         if show:
             print(types)
         return types
     
     def set_data_types(self, column_dict_types):
@@ -446,17 +449,55 @@
             #self.reset_index()
         else:
             self.dataframe = self.get_dataframe().append(row_as_dict, ignore_index=True)
 
     def pivot(self, index_columns_as_list, column_columns_as_list, column_of_values, agg_func):
         return self.get_dataframe().pivot_table(index=index_columns_as_list, columns=column_columns_as_list, values=column_of_values, aggfunc=agg_func)
 
-    def group_by(self, column_name):
-        self.set_dataframe(self.get_dataframe().groupby(column_name).count())
+    def group_by(self, column_name, agg_func='sum', in_place=False, **kwargs):
+        if in_place is True:
+            if agg_func == 'sum':
+                self.set_dataframe(self.get_dataframe().groupby(column_name, **kwargs).sum())
+            elif agg_func == 'count':
+                self.set_dataframe(self.get_dataframe().groupby(column_name, **kwargs).count())
+            elif agg_func == 'min':
+                self.set_dataframe(self.get_dataframe().groupby(column_name, **kwargs).min())
+            elif agg_func == 'max':
+                self.set_dataframe(self.get_dataframe().groupby(column_name, **kwargs).max())
+            elif agg_func == 'mean':
+                self.set_dataframe(self.get_dataframe().groupby(column_name, **kwargs).mean())
+        else:
+            if agg_func == 'sum':
+                return self.get_dataframe().groupby(column_name, **kwargs).sum()
+            elif agg_func == 'count':
+                return self.get_dataframe().groupby(column_name, **kwargs).count()
+            elif agg_func == 'min':
+                return self.get_dataframe().groupby(column_name, **kwargs).min()
+            elif agg_func == 'max':
+                return self.get_dataframe().groupby(column_name, **kwargs).max()
+            elif agg_func == 'mean':
+                return self.get_dataframe().groupby(column_name, **kwargs).mean()
+        
+        
+    def colmun_to_one_hot_encoding(self, column_name, drop_original_column=True, **kwargs):
+        # Perform one-hot encoding on the 'Country' column
+        df_encoded = pd.get_dummies(self.get_dataframe()[column_name], dtype=int, **kwargs)
+
+        # Concatenate the original DataFrame with the encoded columns
+        df = pd.concat([self.get_dataframe(), df_encoded], axis=1, **kwargs)
+
+        # Print the updated DataFrame
+        self.dataframe = df
+         # Drop the original 'Country' column
+        if drop_original_column is True:
+            self.drop_column(column_name)
         
+        return self.dataframe
+    
+    
     def get_nan_indexes_of_column(self, column_name):
         return list(self.get_dataframe().loc[pd.isna(self.get_column(column_name)), :].index)
         
     def missing_data_checking(self, column_name=None):
         if column_name is not None:
             if any(pd.isna(self.get_dataframe()[column_name])) is True:
                 miss = self.dataframe[column_name].isnull().sum()
@@ -569,15 +610,15 @@
                                             data_type='df')
                         data_temp.reset_index()
                         data_temp.resample_timeseries(skip_rows=2)
                         data_temp.reindex_dataframe("valid_time")
                         data_temp.keep_columns(['t2m'])
                         data.append_dataframe(data_temp.get_dataframe())
                     
-                    data.transform_column('t2m', 't2m', lambda o: o - 273.15)
+                    data.transform_column('t2m', lambda o: o - 273.15)
                     nan_indices = self.get_nan_indexes_of_column(column_to_fill)
                     for p in nan_indices:
                         self.set_row('Ta', p, data.get_row(p)['t2m'])
                     print('Imputation of missing data for Ta from ERA5-Land was done!')
                     
                 elif column_to_fill == 'Hr':
                     data.keep_columns(['t2m', 'd2m'])
@@ -585,16 +626,16 @@
                         data_temp = DataFrame(gis.get_era5_land_grib_as_dataframe("E:\projects\pythonsnippets\era5_r3_" + column_to_fill + '_' + str(y) + ".grib", "ta"),
                                             data_type='df')
                         data_temp.reset_index()
                         data_temp.resample_timeseries(skip_rows=2)
                         data_temp.reindex_dataframe("valid_time")
                         data_temp.keep_columns(['t2m', 'd2m'])
                         data.append_dataframe(data_temp.get_dataframe())
-                    data.transform_column('t2m', 't2m', lambda o: o - 273.15)
-                    data.transform_column('d2m', 'd2m', lambda o: o - 273.15)
+                    data.transform_column('t2m', lambda o: o - 273.15)
+                    data.transform_column('d2m', lambda o: o - 273.15)
                     data.add_transformed_columns('era5_hr', '100*exp(-((243.12*17.62*t2m)-(d2m*17.62*t2m)-d2m*17.62*(243.12+t2m))/((243.12+t2m)*(243.12+d2m)))')
                     nan_indices = self.get_missing_data_indexes_in_column(column_to_fill)
                     for p in nan_indices:
                         self.set_row('Hr', p, data.get_row(p)['era5_hr'])
                     
                     print('Imputation of missing data for Hr from ERA5-Land was done!')
                 elif column_to_fill == 'Rg':
@@ -621,15 +662,15 @@
                                 
                             new_value = (data.get_row(p)['ssrd'] - previous_hour)/3600
                         l.append(new_value)
 
                     data.add_column('rg', l)
                     data.keep_columns(['rg'])
                     data.rename_columns({'rg': 'ssrd'})
-                    data.transform_column('ssrd', 'ssrd', lambda o : o if abs(o) < 1500 else 0 )    
+                    data.transform_column('ssrd', lambda o : o if abs(o) < 1500 else 0 )    
                     data.export('rg.csv', index=True)
                     nan_indices = self.get_nan_indexes_of_column(column_to_fill)
                     for p in nan_indices:
                         self.set_row('Rg', p, data.get_row(p)['ssrd'])
                     
                     print('Imputation of missing data for Rg from ERA5-Land was done!')
         
@@ -788,16 +829,20 @@
         #print(np.reshape(self.get_column(column).iloc[-window_size:].to_numpy(), (window_size, 1)))
         #print(self.__vectorizer.transform([np.array(self.get_column(column).iloc[-window_size:])]))
         return self.__vectorizer.transform(np.reshape(self.get_column(column).iloc[-window_size:].to_numpy(), (window_size, 1)))
 
     def write_column_in_file(self, column, path='data/out.csv'):
         Lib.write_liste_in_file(path, self.get_column(column).apply(str))
 
-    def check_duplicated_rows(self):
-        return any(self.get_dataframe().duplicated())
+    def check_duplicated_rows(self, **kwargs):
+        # Count duplicated rows
+        duplicate_count = self.get_dataframe().duplicated(**kwargs).sum()
+        # Display the count of duplicated rows
+        print("Number of duplicated rows:", duplicate_count)
+        return duplicate_count
 
     def check_duplicated_in_column(self, column):
         return any(self.get_column(column).duplicated())
 
     def write_check_duplicated_column_result_in_file(self, column, path='data/latin_comments.csv'):
         Lib.write_liste_in_file(path, self.get_column(column).duplicated().apply(str))
 
@@ -821,37 +866,37 @@
             
     def select_datetime_range(self, start_datetime, end_datetime, in_place=True, *args):
         if in_place is True:
             self.dataframe = self.dataframe.loc[start_datetime:end_datetime]
         else:
             return self.dataframe.loc[start_datetime:end_datetime]
 
-    def transform_column(self, column_to_trsform, column_src, fun_de_trasformation, in_place=True, *args):
+    def transform_column(self, column_name, transformation_func, in_place=True, *args):
         """_summary_
 
         Args:
             column_to_trsform (_type_): column to transform
             column_src (_type_): Column to use as a source for the transformation
             fun_de_trasformation (_type_): The function of transformation, if it has multiple arguments pass them as args:
             example: data.transform_column(column, column, Lib.remove_stopwords, True, stopwords)
             in_place (bool, optional): If true the changes will affect the original dataframe. Defaults to True.
 
         Returns:
             _type_: _description_
         """
         if in_place is True:
             if (len(args) != 0):
-                self.set_column(column_to_trsform, self.get_column(column_src).apply(fun_de_trasformation, args=(args[0],)))
+                self.set_column(column_name, self.get_column(column_name).apply(transformation_func, args=(args[0],)))
             else:
-                self.set_column(column_to_trsform, self.get_column(column_src).apply(fun_de_trasformation))
+                self.set_column(column_name, self.get_column(column_name).apply(transformation_func))
         else:
             if (len(args) != 0):
-                return self.get_column(column_src).apply(fun_de_trasformation, args=(args[0],))
+                return self.get_column(column_name).apply(transformation_func, args=(args[0],))
             else:
-                return self.get_column(column_src).apply(fun_de_trasformation)
+                return self.get_column(column_name).apply(transformation_func)
             
     def to_no_accent_column(self, column):
         self.trasform_column(column, column, Lib.no_accent)
         self.set_column(column, self.get_column(column))
 
     def write_dataframe_in_file(self, out_file='data/out.csv', delimiter=','):
         Lib.write_liste_csv(self.get_dataframe().values, out_file, delimiter)
@@ -864,15 +909,15 @@
         return self.get_dataframe().pivot_table(index=[column], aggfunc='size')
     
     def get_distinct_values_as_list(self, column):
         return list(self.get_dataframe().pivot_table(index=[column], aggfunc='size').index)
     
     def column_to_numerical_values(self, column):
         maping = list(self.get_dataframe().pivot_table(index=[column], aggfunc='size').index)
-        self.transform_column(column, column, lambda o : maping.index(o))
+        self.transform_column(column, lambda o : maping.index(o))
         return maping
     
     def reverse_column_from_numerical_values(self, column, maping):
         self.trasform_column(column, column, lambda o : maping[int(o)])
 
     def count_occurence_of_row_as_count_column(self, column):
         column_name = 'count'
@@ -1014,15 +1059,15 @@
         if type == 'json':
             destination_path='data/json_dataframe.json'
             self.get_dataframe().to_json(destination_path)
         elif type == 'csv':
             self.get_dataframe().to_csv(destination_path, index=index)
         elif type == 'pkl':
             self.get_dataframe().to_pickle(destination_path)
-        print('DataFrame exported successfully to /' + destination_path)
+        print('DataFrame exported successfully to ' + destination_path)
         
     def sample(self, n=10, frac=None):
         if frac is not None:
             return self.get_dataframe().sample(n=frac)
         return self.get_dataframe().sample(n=n)
 
     """
@@ -1077,21 +1122,21 @@
 
     def eliminate_outliers_quantile(self, column, min_quantile, max_quantile):
         min_q, max_q = self.get_column(column).quantile(min_quantile), self.get_column(column).quantile(max_quantile)
         self.filter_dataframe(column, self.outliers_decision_function, min_q, max_q)
 
     def scale_column(self, column):
         max_column = self.get_column(column).describe()['max']
-        self.transform_column(column, column, self.scale_trasform_fun, max_column)
+        self.transform_column(column, self.scale_trasform_fun, max_column)
 
-    def drop_duplicated_rows(self, column):
-        self.set_dataframe(self.dataframe.drop_duplicates(subset=column, keep='first'))
+    def drop_duplicated_rows(self, **kwargs):
+        self.set_dataframe(self.dataframe.drop_duplicates(keep='first', **kwargs))
         
-    def drop_duplicated_indexes(self):
-        self.dataframe = self.dataframe[~self.dataframe.index.duplicated(keep='first')]
+    def drop_duplicated_indexes(self, **kwargs):
+        self.dataframe = self.dataframe[~self.dataframe.index.duplicated(keep='first', **kwargs)]
         
     def plot_dataframe(self):
         self.get_dataframe().plot()
         plt.show()
         
     def to_numpy(self):
         return self.get_dataframe().values
@@ -1298,15 +1343,15 @@
         
     def column_to_date(self, column_name, format='%Y-%m-%d %H:%M:%S', extraction_func=None):
         if extraction_func is None:
             self.set_column(column_name, pd.to_datetime(self.get_column(column_name)))
             self.set_column(column_name, self.get_column(column_name).dt.strftime(format))
             self.set_column(column_name, pd.to_datetime(self.get_column(column_name)))
         else:
-            self.transform_column(column_name, column_name, extraction_func)
+            self.transform_column(column_name, extraction_func)
         
     
         
     def datetime_reformate(self, date_time_column_name, new_format='%Y-%m-%d %H:%M:%S'):
         self.set_column(date_time_column_name, self.get_column(date_time_column_name).dt.strftime(new_format))
         return self.get_dataframe()
 
@@ -1488,15 +1533,15 @@
             self.concatinate(dest_dataframe.get_dataframe())
             return dest_dataframe.get_dataframe()
         elif scaler_type == 'adjusted_log':
             def log_function(o, min_column):
                 return np.log(1 + o - min_column)
             for name in columns_names_as_list:
                 min_column = self.get_column(name).min()
-                self.transform_column(name, name, log_function, min_column)
+                self.transform_column(name, log_function, min_column)
             return self.get_columns(columns_names_as_list)
                         
     def scale_dataframe(self, scaler_type='min_max', in_place=True):
         """A method  to standardize the independent features present in the dataframe in a fixed range.
 
         Args:
             column_name ([type]): 
@@ -1514,15 +1559,15 @@
             self.__vectorizer = StandardScaler() 
             self.set_dataframe(self.__vectorizer.fit_transform(X=self.get_dataframe()))
         elif scaler_type == 'adjusted_log':
             def log_function(o, min_column):
                 return np.log(1 + o - min_column)
             for name in self.get_columns_names():
                 min_column = self.get_column(name).min()
-                self.transform_column(name, name, log_function, min_column)
+                self.transform_column(name, log_function, min_column)
         self.convert_dataframe_type()
         return self.get_dataframe()
     def load_dataset(self, dataset='iris'):
         """
         boston: Load and return the boston house-prices dataset (regression)
         iris: Load and return the iris dataset (classification).
         """
```

### Comparing `data-science-toolkit-0.1.3/src/data_science_toolkit/gis.py` & `data-science-toolkit-0.1.4/src/data_science_toolkit/gis.py`

 * *Files identical despite different names*

### Comparing `data-science-toolkit-0.1.3/src/data_science_toolkit/imagefactory.py` & `data-science-toolkit-0.1.4/src/data_science_toolkit/imagefactory.py`

 * *Files identical despite different names*

### Comparing `data-science-toolkit-0.1.3/src/data_science_toolkit/lib.py` & `data-science-toolkit-0.1.4/src/data_science_toolkit/lib.py`

 * *Files identical despite different names*

### Comparing `data-science-toolkit-0.1.3/src/data_science_toolkit/model.py` & `data-science-toolkit-0.1.4/src/data_science_toolkit/model.py`

 * *Files identical despite different names*

### Comparing `data-science-toolkit-0.1.3/src/data_science_toolkit/r3.py` & `data-science-toolkit-0.1.4/src/data_science_toolkit/r3.py`

 * *Files identical despite different names*

### Comparing `data-science-toolkit-0.1.3/src/data_science_toolkit/rl.py` & `data-science-toolkit-0.1.4/src/data_science_toolkit/rl.py`

 * *Files identical despite different names*

### Comparing `data-science-toolkit-0.1.3/src/data_science_toolkit/rl_dqn.py` & `data-science-toolkit-0.1.4/src/data_science_toolkit/rl_dqn.py`

 * *Files identical despite different names*

### Comparing `data-science-toolkit-0.1.3/src/data_science_toolkit/vectorizer.py` & `data-science-toolkit-0.1.4/src/data_science_toolkit/vectorizer.py`

 * *Files identical despite different names*

### Comparing `data-science-toolkit-0.1.3/src/data_science_toolkit.egg-info/PKG-INFO` & `data-science-toolkit-0.1.4/src/data_science_toolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-science-toolkit
-Version: 0.1.3
+Version: 0.1.4
 Summary: Data Science Toolkit (DST) is a Python library that helps implement data science related project with ease.
 Home-page: https://github.com/elhachimi-ch/dst
 Author: EL HACHIMI CHOUAIB
 Author-email: elhachimi.ch@gmail.com
 Project-URL: Bug Tracker, https://github.com/elhachimi-ch/dst/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

