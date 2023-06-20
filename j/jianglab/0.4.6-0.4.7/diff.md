# Comparing `tmp/jianglab-0.4.6.tar.gz` & `tmp/jianglab-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.4.6.tar", last modified: Fri Jun 16 20:01:45 2023, max compression
+gzip compressed data, was "jianglab-0.4.7.tar", last modified: Tue Jun 20 00:55:13 2023, max compression
```

## Comparing `jianglab-0.4.6.tar` & `jianglab-0.4.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-16 20:01:45.856291 jianglab-0.4.6/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-16 20:01:45.855954 jianglab-0.4.6/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.4.6/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-16 20:01:45.852220 jianglab-0.4.6/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.4.6/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)    21183 2023-06-16 20:01:41.000000 jianglab-0.4.6/jianglab/common_functions.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.4.6/jianglab/params.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-16 20:01:45.855354 jianglab-0.4.6/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-16 20:01:45.000000 jianglab-0.4.6/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-06-16 20:01:45.000000 jianglab-0.4.6/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-06-16 20:01:45.000000 jianglab-0.4.6/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       79 2023-06-16 20:01:45.000000 jianglab-0.4.6/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-06-16 20:01:45.000000 jianglab-0.4.6/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-06-16 20:01:45.856420 jianglab-0.4.6/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)      974 2023-06-16 20:01:38.000000 jianglab-0.4.6/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-20 00:55:13.293694 jianglab-0.4.7/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-20 00:55:13.293345 jianglab-0.4.7/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.4.7/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-20 00:55:13.290531 jianglab-0.4.7/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.4.7/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)    22812 2023-06-20 00:54:58.000000 jianglab-0.4.7/jianglab/common_functions.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.4.7/jianglab/params.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-20 00:55:13.292777 jianglab-0.4.7/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-20 00:55:13.000000 jianglab-0.4.7/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-06-20 00:55:13.000000 jianglab-0.4.7/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-06-20 00:55:13.000000 jianglab-0.4.7/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       79 2023-06-20 00:55:13.000000 jianglab-0.4.7/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-06-20 00:55:13.000000 jianglab-0.4.7/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-06-20 00:55:13.293818 jianglab-0.4.7/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      974 2023-06-20 00:55:07.000000 jianglab-0.4.7/setup.py
```

### Comparing `jianglab-0.4.6/PKG-INFO` & `jianglab-0.4.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.4.6
+Version: 0.4.7
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.4.6/README.md` & `jianglab-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `jianglab-0.4.6/jianglab/common_functions.py` & `jianglab-0.4.7/jianglab/common_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -451,9 +451,43 @@
         data_dict = {"centers":centers, "lp_data":lp_data, "center_waveform":center_waveform}
         if save_data:
             save_instance(filepath[:-5]+".pkl", data_dict)
         if show_plot:
             plt.plot(center_waveform.mean(axis=0))
             plt.show()
 
-def func3():
-    pass
+
+
+def assign_gID_between_two_files(units_ref, unit_to_assign, search_range=1):
+
+    def find_closest_vector_index(reference_vector, vectors):
+        """
+        Find the closest vector to the reference vector among a list of vectors.
+        """
+        min_distance = float('inf')
+        closest_vector_index = None
+        for i,vector in enumerate(vectors):
+            distance = np.linalg.norm(reference_vector - vector)
+            if distance < min_distance:
+                min_distance = distance
+                closest_vector_index = i
+        return closest_vector_index
+    
+    used_IDs = []
+    for key in unit_to_assign["units_data"].keys():
+        assign_data = unit_to_assign["units_data"][key]
+        candidate_list = []
+        for ref_key in units_ref["units_data"].keys():          
+            ref_unit = units_ref["units_data"][ref_key]
+            if abs(assign_data["col"] - ref_unit["col"]) < search_range \
+            and abs(assign_data["row"] - ref_unit["row"]) < search_range:
+                if ref_unit["unitID"] not in used_IDs:
+                    candidate_list.append(units_ref["units_data"][ref_key])
+        if candidate_list == []:
+            unit_to_assign["units_data"][key]["globalID"] = -1
+        else:
+            waveform_list = [x["waveform"] for x in candidate_list]
+            closest_vector_index = find_closest_vector_index(assign_data["waveform"], waveform_list)
+            unit_to_assign["units_data"][key]["globalID"] = candidate_list[closest_vector_index]["unitID"]
+            used_IDs.append(unit_to_assign["units_data"][key]["globalID"])
+    print(used_IDs)
+    return unit_to_assign
```

### Comparing `jianglab-0.4.6/jianglab.egg-info/PKG-INFO` & `jianglab-0.4.7/jianglab.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.4.6
+Version: 0.4.7
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.4.6/setup.py` & `jianglab-0.4.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.4.6',
+    version='0.4.7',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
         "McsPyDataTools",
```

