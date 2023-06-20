# Comparing `tmp/agsi-2.3.tar.gz` & `tmp/agsi-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agsi-2.3.tar", last modified: Tue Jun 20 09:53:31 2023, max compression
+gzip compressed data, was "agsi-2.5.tar", last modified: Tue Jun 20 10:21:12 2023, max compression
```

## Comparing `agsi-2.3.tar` & `agsi-2.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-20 09:53:31.016108 agsi-2.3/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       56 2023-05-26 04:44:18.000000 agsi-2.3/.gitignore
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      212 2023-06-20 09:53:31.016108 agsi-2.3/PKG-INFO
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      190 2023-05-25 15:22:54.000000 agsi-2.3/README.md
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-20 09:53:31.012108 agsi-2.3/agsi/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       35 2023-05-25 15:09:48.000000 agsi-2.3/agsi/__init__.py
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-20 09:53:31.016108 agsi-2.3/agsi/data/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)    16491 2023-06-20 09:50:45.000000 agsi-2.3/agsi/data/FarmData.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        0 2023-05-25 15:09:48.000000 agsi-2.3/agsi/data/__init__.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)     8979 2023-06-14 10:44:20.000000 agsi-2.3/agsi/data/utils.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)  1075510 2023-06-15 07:22:38.000000 agsi-2.3/agsi/demo_V2.ipynb
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       12 2023-05-25 15:09:48.000000 agsi-2.3/agsi/main.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      111 2023-05-25 15:09:48.000000 agsi-2.3/agsi/requirements.txt
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-20 09:53:31.016108 agsi-2.3/agsi.egg-info/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      212 2023-06-20 09:53:30.000000 agsi-2.3/agsi.egg-info/PKG-INFO
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      302 2023-06-20 09:53:30.000000 agsi-2.3/agsi.egg-info/SOURCES.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        1 2023-06-20 09:53:30.000000 agsi-2.3/agsi.egg-info/dependency_links.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       60 2023-06-20 09:53:30.000000 agsi-2.3/agsi.egg-info/requires.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        5 2023-06-20 09:53:30.000000 agsi-2.3/agsi.egg-info/top_level.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       38 2023-06-20 09:53:31.016108 agsi-2.3/setup.cfg
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      367 2023-06-20 09:52:40.000000 agsi-2.3/setup.py
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-20 10:21:12.948170 agsi-2.5/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       56 2023-05-26 04:44:18.000000 agsi-2.5/.gitignore
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      212 2023-06-20 10:21:12.948170 agsi-2.5/PKG-INFO
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      190 2023-05-25 15:22:54.000000 agsi-2.5/README.md
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-20 10:21:12.948170 agsi-2.5/agsi/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       35 2023-05-25 15:09:48.000000 agsi-2.5/agsi/__init__.py
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-20 10:21:12.948170 agsi-2.5/agsi/data/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)    16773 2023-06-20 10:20:40.000000 agsi-2.5/agsi/data/FarmData.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        0 2023-05-25 15:09:48.000000 agsi-2.5/agsi/data/__init__.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)     8979 2023-06-14 10:44:20.000000 agsi-2.5/agsi/data/utils.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)  1075510 2023-06-15 07:22:38.000000 agsi-2.5/agsi/demo_V2.ipynb
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       12 2023-05-25 15:09:48.000000 agsi-2.5/agsi/main.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      111 2023-05-25 15:09:48.000000 agsi-2.5/agsi/requirements.txt
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-20 10:21:12.948170 agsi-2.5/agsi.egg-info/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      212 2023-06-20 10:21:12.000000 agsi-2.5/agsi.egg-info/PKG-INFO
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      302 2023-06-20 10:21:12.000000 agsi-2.5/agsi.egg-info/SOURCES.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        1 2023-06-20 10:21:12.000000 agsi-2.5/agsi.egg-info/dependency_links.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       60 2023-06-20 10:21:12.000000 agsi-2.5/agsi.egg-info/requires.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        5 2023-06-20 10:21:12.000000 agsi-2.5/agsi.egg-info/top_level.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       38 2023-06-20 10:21:12.948170 agsi-2.5/setup.cfg
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      367 2023-06-20 10:21:08.000000 agsi-2.5/setup.py
```

### Comparing `agsi-2.3/agsi/data/FarmData.py` & `agsi-2.5/agsi/data/FarmData.py`

 * *Files 1% similar despite different names*

```diff
@@ -358,20 +358,34 @@
   
   def get_chips(self,chip_size=200,valid_threshold=0.1,modality_type="drone",resolution=75,timestamp=None):
      
       block_image=self.get_modality(modality_type=modality_type,timestamp=timestamp)
       return Chip(block_image,chip_size,valid_threshold)
   
   def get_times(self):
+     
      times = self.info['data_path'].keys()
      return list(times)
   
+  def get_modality_list(self):
+     
+     timestamps=self.get_times()
+     modality=[]
+
+     for timestamp in timestamps:
+        for mod in self.get_modalities_for_times(timestamp):
+            modality.append(mod)
+
+     modality=list(set(modality))
+     return modality
+
+  
   def get_times_for_modality(self,modality):
-     all_timestamps=self.get_times()
      
+     all_timestamps=self.get_times()
      fetch_timestamps=[]
      for timestamp in all_timestamps:
         if modality in self.info['data_path'][timestamp]:
            fetch_timestamps.append(timestamp)
 
      return fetch_timestamps
```

### Comparing `agsi-2.3/agsi/data/utils.py` & `agsi-2.5/agsi/data/utils.py`

 * *Files identical despite different names*

### Comparing `agsi-2.3/agsi/demo_V2.ipynb` & `agsi-2.5/agsi/demo_V2.ipynb`

 * *Files identical despite different names*

