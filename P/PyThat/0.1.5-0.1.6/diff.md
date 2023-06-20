# Comparing `tmp/PyThat-0.1.5.tar.gz` & `tmp/PyThat-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyThat-0.1.5.tar", last modified: Thu Mar 16 16:16:11 2023, max compression
+gzip compressed data, was "PyThat-0.1.6.tar", last modified: Tue Jun 20 20:55:02 2023, max compression
```

## Comparing `PyThat-0.1.5.tar` & `PyThat-0.1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:16:11.487331 PyThat-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-16 16:15:56.000000 PyThat-0.1.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-03-16 16:16:11.487331 PyThat-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-03-16 16:15:56.000000 PyThat-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-16 16:15:56.000000 PyThat-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-03-16 16:16:11.487331 PyThat-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:16:11.483331 PyThat-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:16:11.483331 PyThat-0.1.5/src/PyThat/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-16 16:15:56.000000 PyThat-0.1.5/src/PyThat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31267 2023-03-16 16:15:56.000000 PyThat-0.1.5/src/PyThat/h5to_nc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:16:11.487331 PyThat-0.1.5/src/PyThat/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-03-16 16:15:56.000000 PyThat-0.1.5/src/PyThat/helpers/BLS.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 16:15:56.000000 PyThat-0.1.5/src/PyThat/helpers/FMR.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-03-16 16:15:56.000000 PyThat-0.1.5/src/PyThat/helpers/ROI.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 16:15:56.000000 PyThat-0.1.5/src/PyThat/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-03-16 16:15:56.000000 PyThat-0.1.5/src/PyThat/helpers/dB.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:16:11.487331 PyThat-0.1.5/src/PyThat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-03-16 16:16:11.000000 PyThat-0.1.5/src/PyThat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-03-16 16:16:11.000000 PyThat-0.1.5/src/PyThat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 16:16:11.000000 PyThat-0.1.5/src/PyThat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-16 16:16:11.000000 PyThat-0.1.5/src/PyThat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-16 16:16:11.000000 PyThat-0.1.5/src/PyThat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:55:02.080178 PyThat-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-20 20:54:48.000000 PyThat-0.1.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-20 20:55:02.080178 PyThat-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-20 20:54:48.000000 PyThat-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-20 20:54:48.000000 PyThat-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-20 20:55:02.080178 PyThat-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:55:02.080178 PyThat-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:55:02.080178 PyThat-0.1.6/src/PyThat/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-20 20:54:48.000000 PyThat-0.1.6/src/PyThat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31259 2023-06-20 20:54:48.000000 PyThat-0.1.6/src/PyThat/h5to_nc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:55:02.080178 PyThat-0.1.6/src/PyThat/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-06-20 20:54:48.000000 PyThat-0.1.6/src/PyThat/helpers/BLS.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 20:54:48.000000 PyThat-0.1.6/src/PyThat/helpers/FMR.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-20 20:54:48.000000 PyThat-0.1.6/src/PyThat/helpers/ROI.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 20:54:48.000000 PyThat-0.1.6/src/PyThat/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-20 20:54:48.000000 PyThat-0.1.6/src/PyThat/helpers/dB.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 20:55:02.080178 PyThat-0.1.6/src/PyThat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-20 20:55:02.000000 PyThat-0.1.6/src/PyThat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-20 20:55:02.000000 PyThat-0.1.6/src/PyThat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 20:55:02.000000 PyThat-0.1.6/src/PyThat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-20 20:55:02.000000 PyThat-0.1.6/src/PyThat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 20:55:02.000000 PyThat-0.1.6/src/PyThat.egg-info/top_level.txt
```

### Comparing `PyThat-0.1.5/LICENSE.txt` & `PyThat-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyThat-0.1.5/PKG-INFO` & `PyThat-0.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyThat
-Version: 0.1.5
+Version: 0.1.6
 Summary: Read Thatec h5 formatting and convert it to netcdf files and xarray objects.
 Home-page: https://github.com/mrschweizer/PyThat
 Author: Matthias Schweizer
 Author-email: mareschweizer@gmail.com
 Project-URL: Bug Tracker, https://github.com/mrschweizer/PyThat/issues
 Project-URL: Documentation, https://pythat.readthedocs.io/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PyThat-0.1.5/README.md` & `PyThat-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `PyThat-0.1.5/setup.cfg` & `PyThat-0.1.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = PyThat
-version = 0.1.5
+version = 0.1.6
 author = Matthias Schweizer
 author_email = mareschweizer@gmail.com
 description = Read Thatec h5 formatting and convert it to netcdf files and xarray objects.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mrschweizer/PyThat
 project_urls =
```

### Comparing `PyThat-0.1.5/src/PyThat/h5to_nc.py` & `PyThat-0.1.6/src/PyThat/h5to_nc.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,14 @@
                     self.dataset = self.dataset.chunk(chunks='auto')
             self.save_file_from_string(self.dataset, self.save_path)
             print('Saved dataset as {}'.format(self.save_path))
         elif self.array is not None:
             self.save_file_from_string(self.dataset, self.save_path)
             print('Saved as {}'.format(self.save_path))
 
-
     def open_netcdf(self):
         """This function opens the expected output netcdf if it exists.\n
         Otherwise save_netcdf() is called to create such a file."""
 
         if self.index is True:
             try:
                 self.save_path = self.path.with_suffix('.nc').absolute()
@@ -130,16 +129,14 @@
                           'labbook': self.labbook,
                           'logs': self.logs,
                           'measurement_tree': self.tree_string,
                           'scan_definition': self.definition}
         except KeyError:
             print('Metadata not found. It will not be available.')
 
-
-
     def construct_tree(self):
         self.definition = {self.check_for_sp_char(i): self.convert_to_dict(k) for (i, k) in self.f['scan_definition'].items()}
         if 'tree_view' in self.definition.keys():
             del(self.definition['tree_view'])
         self.devices = {self.check_for_sp_char(i): self.convert_to_dict(k, truncate=True) for (i, k) in self.f['devices'].items()}
         self.labbook = {self.check_for_sp_char(i): self.convert_to_dict(k) for (i, k) in self.f['labbook'].items()}
         self.logs = self.convert_to_dict(self.f['measurement/log'])
@@ -239,15 +236,14 @@
                 except KeyError:
                     pass
                 line = textwrap.indent(printout, ' '*2*int(j.tree_indent))
                 print_tree_list.append(line)
                 # print(line)
         self.tree_string = '\n'.join(print_tree_list)
 
-
         """User Input Index"""
         if self.index is None:
             # Get and parse user input for group and entry for self.target and self.index
             print("Please enter the Group number and the group internal number.")
             x = (0, 0)
             for i in range(3):
                 inp = input()
@@ -265,15 +261,14 @@
         elif self.index is True:
             pass
         else:
             # override possible_indicators, if index is specified
             possible_indicators = [self.index]
             print(f'Only one index selected: {possible_indicators[0]}')
 
-
         # create array with all core-data names
         # create self.metadata
         core_data_names = []
         for (i, k) in self.f['scan_definition'].items():
             meta_entry = self.get_metadata(i)
             if meta_entry is not None:
                 try:
@@ -423,15 +418,14 @@
             dims = list(coords.keys())
             units.reverse()
             dims.reverse()
             segments.reverse()
 
             self.indicator_name, indicator_unit = self.get_units(self.indicator_name)
 
-
             # iterate over metadata to innermost data to get names of all dimensions
             metadata = self.metadata[self.target[row][0]]
             if metadata is not None:
                 print(f'Get Metadata for: {self.target[row][0]}')
                 for i in range(len(data_shape)):
                     coord_name = metadata['name'][i]
                     scales = self.get_scales(self.target[row][0], i)
@@ -584,15 +578,14 @@
                     group_dict[key] = value
                 except KeyError:
                     pass
         except KeyError:
             print('The eLab Group could not be found in the hdf5 file.')
         return group_dict
 
-
     @staticmethod
     def check_for_sp_char(text):
         import re
         special_char = re.compile(r"%%%(\d+)%%%")
         text = str(text)
         res = special_char.finditer(text)
         for v in res:
@@ -726,12 +719,11 @@
         array = array.swap_dims({dim_name: temp_name})
     array = array.assign_coords({temp_name: temp})
     array = array.drop_vars(identicals_list)
     array = array.rename_dims({temp_name: new_dim})
     array = array.rename({temp_name: new_dim})
     return array
 
+
 # Add consolidate dims as methods to xarray.DataArray and xarray.Dataset
 xr.DataArray.consolidate_dims = consolidate_dims
 xr.Dataset.consolidate_dims = consolidate_dims
-
-
```

### Comparing `PyThat-0.1.5/src/PyThat/helpers/ROI.py` & `PyThat-0.1.6/src/PyThat/helpers/ROI.py`

 * *Files identical despite different names*

### Comparing `PyThat-0.1.5/src/PyThat.egg-info/PKG-INFO` & `PyThat-0.1.6/src/PyThat.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyThat
-Version: 0.1.5
+Version: 0.1.6
 Summary: Read Thatec h5 formatting and convert it to netcdf files and xarray objects.
 Home-page: https://github.com/mrschweizer/PyThat
 Author: Matthias Schweizer
 Author-email: mareschweizer@gmail.com
 Project-URL: Bug Tracker, https://github.com/mrschweizer/PyThat/issues
 Project-URL: Documentation, https://pythat.readthedocs.io/
 Classifier: Programming Language :: Python :: 3
```

