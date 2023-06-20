# Comparing `tmp/obrpy-0.0.9.tar.gz` & `tmp/obrpy-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obrpy-0.0.9.tar", last modified: Thu May 18 15:40:38 2023, max compression
+gzip compressed data, was "obrpy-0.1.0.tar", last modified: Tue Jun 20 12:52:42 2023, max compression
```

## Comparing `obrpy-0.0.9.tar` & `obrpy-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,58 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 15:40:38.900665 obrpy-0.0.9/
--rw-rw-rw-   0        0        0      283 2023-05-18 15:40:38.899665 obrpy-0.0.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-18 15:40:38.875665 obrpy-0.0.9/obrpy/
--rw-rw-rw-   0        0        0     1341 2023-02-23 12:03:19.000000 obrpy-0.0.9/obrpy/PathSelector.py
--rw-rw-rw-   0        0        0     8519 2023-05-18 15:40:14.000000 obrpy-0.0.9/obrpy/__init__.py
--rw-rw-rw-   0        0        0     1328 2023-05-10 14:52:06.000000 obrpy-0.0.9/obrpy/checkouts.py
--rw-rw-rw-   0        0        0     1063 2023-05-10 14:43:49.000000 obrpy-0.0.9/obrpy/clear.py
--rw-rw-rw-   0        0        0     2246 2023-05-10 14:46:47.000000 obrpy-0.0.9/obrpy/load.py
--rw-rw-rw-   0        0        0     8323 2023-05-10 11:38:23.000000 obrpy-0.0.9/obrpy/obr.py
--rw-rw-rw-   0        0        0     2123 2023-04-25 15:28:15.000000 obrpy-0.0.9/obrpy/obrsdk.py
--rw-rw-rw-   0        0        0     3212 2023-05-10 14:09:36.000000 obrpy-0.0.9/obrpy/save.py
--rw-rw-rw-   0        0        0     3741 2023-05-10 12:02:20.000000 obrpy-0.0.9/obrpy/settings.py
--rw-rw-rw-   0        0        0     3425 2023-05-03 08:58:35.000000 obrpy-0.0.9/obrpy/take_a_look.py
--rw-rw-rw-   0        0        0     3350 2023-05-10 15:00:23.000000 obrpy-0.0.9/obrpy/update.py
-drwxrwxrwx   0        0        0        0 2023-05-18 15:40:38.897667 obrpy-0.0.9/obrpy.egg-info/
--rw-rw-rw-   0        0        0      283 2023-05-18 15:40:38.000000 obrpy-0.0.9/obrpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      351 2023-05-18 15:40:38.000000 obrpy-0.0.9/obrpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 15:40:38.000000 obrpy-0.0.9/obrpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-18 15:40:38.000000 obrpy-0.0.9/obrpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-18 15:40:38.000000 obrpy-0.0.9/obrpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 15:40:38.900665 obrpy-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1333 2023-05-18 15:40:35.000000 obrpy-0.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-18 15:40:38.898665 obrpy-0.0.9/test/
--rw-rw-rw-   0        0        0      812 2023-05-10 14:57:34.000000 obrpy-0.0.9/test/test.py
+drwxrwxrwx   0        0        0        0 2023-06-20 12:52:42.009925 obrpy-0.1.0/
+-rw-rw-rw-   0        0        0      283 2023-06-20 12:52:42.008923 obrpy-0.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-20 12:52:39.992206 obrpy-0.1.0/obrpy/
+drwxrwxrwx   0        0        0        0 2023-06-20 12:52:40.026206 obrpy-0.1.0/obrpy/ANALYSIS/
+-rw-rw-rw-   0        0        0     9204 2023-05-30 09:48:03.000000 obrpy-0.1.0/obrpy/ANALYSIS/global_analysis.py
+-rw-rw-rw-   0        0        0     8104 2023-06-20 08:13:22.000000 obrpy-0.1.0/obrpy/ANALYSIS/local_analysis.py
+drwxrwxrwx   0        0        0        0 2023-06-20 12:52:40.029206 obrpy-0.1.0/obrpy/SIGNAL/
+-rw-rw-rw-   0        0        0     4814 2023-05-03 10:51:46.000000 obrpy-0.1.0/obrpy/SIGNAL/cross_spectrum.py
+-rw-rw-rw-   0        0        0     4762 2023-06-20 07:55:06.000000 obrpy-0.1.0/obrpy/SIGNAL/spectral_shift.py
+drwxrwxrwx   0        0        0        0 2023-06-20 12:52:40.047214 obrpy-0.1.0/obrpy/UTILS/
+-rw-rw-rw-   0        0        0    11916 2023-06-05 08:24:09.000000 obrpy-0.1.0/obrpy/UTILS/read_OBR.py
+-rw-rw-rw-   0        0        0    11436 2023-06-19 11:27:53.000000 obrpy-0.1.0/obrpy/UTILS/utils.py
+-rw-rw-rw-   0        0        0    12610 2023-06-20 08:28:47.000000 obrpy-0.1.0/obrpy/__init__.py
+-rw-rw-rw-   0        0        0     1447 2023-06-20 07:02:11.000000 obrpy-0.1.0/obrpy/checkouts.py
+-rw-rw-rw-   0        0        0      195 2023-06-20 06:55:40.000000 obrpy-0.1.0/obrpy/clear.py
+-rw-rw-rw-   0        0        0      683 2023-06-19 10:46:23.000000 obrpy-0.1.0/obrpy/fuego.py
+-rw-rw-rw-   0        0        0     1347 2023-06-19 10:11:39.000000 obrpy-0.1.0/obrpy/gui.py
+-rw-rw-rw-   0        0        0     1459 2023-06-20 06:56:41.000000 obrpy-0.1.0/obrpy/load.py
+-rw-rw-rw-   0        0        0     7468 2023-06-19 11:20:36.000000 obrpy-0.1.0/obrpy/obr.py
+drwxrwxrwx   0        0        0        0 2023-06-20 12:52:41.970922 obrpy-0.1.0/obrpy/obrsdk/
+-rw-rw-rw-   0        0        0    73728 2023-04-25 10:36:31.000000 obrpy-0.1.0/obrpy/obrsdk/CommandProcessor.dll
+-rw-rw-rw-   0        0        0    53248 2023-04-25 10:36:31.000000 obrpy-0.1.0/obrpy/obrsdk/CyUSBComm.dll
+-rw-rw-rw-   0        0        0   217088 2023-04-25 10:36:31.000000 obrpy-0.1.0/obrpy/obrsdk/KL2DLL32.DLL
+-rw-rw-rw-   0        0        0   282624 2023-04-25 10:36:31.000000 obrpy-0.1.0/obrpy/obrsdk/LtCore.dll
+-rw-rw-rw-   0        0        0 24322048 2023-04-25 10:36:31.000000 obrpy-0.1.0/obrpy/obrsdk/LtMath.dll
+-rw-rw-rw-   0        0        0   110592 2023-04-25 10:36:31.000000 obrpy-0.1.0/obrpy/obrsdk/Phoenix.dll
+-rw-rw-rw-   0        0        0   106496 2023-04-25 10:36:31.000000 obrpy-0.1.0/obrpy/obrsdk/RemoteInterface.dll
+-rw-rw-rw-   0        0        0    57344 2023-04-25 10:36:31.000000 obrpy-0.1.0/obrpy/obrsdk/boost_date_time-mt.dll
+-rw-rw-rw-   0        0        0    77824 2023-04-25 10:36:31.000000 obrpy-0.1.0/obrpy/obrsdk/boost_filesystem-mt.dll
+-rw-rw-rw-   0        0        0    11776 2023-04-25 10:36:31.000000 obrpy-0.1.0/obrpy/obrsdk/boost_system-mt.dll
+-rw-rw-rw-   0        0        0    53248 2023-04-25 10:36:31.000000 obrpy-0.1.0/obrpy/obrsdk/boost_thread-mt.dll
+-rw-rw-rw-   0        0        0   756640 2023-04-25 10:36:31.000000 obrpy-0.1.0/obrpy/obrsdk/libiomp5md.dll
+-rwxrwxrwx   0        0        0    66560 2023-04-25 11:55:06.000000 obrpy-0.1.0/obrpy/obrsdk/obr.exe
+-rw-rw-rw-   0        0        0   466944 2023-04-25 10:36:31.000000 obrpy-0.1.0/obrpy/obrsdk/ova32.dll
+-rw-rw-rw-   0        0        0   100692 2023-04-25 10:36:31.000000 obrpy-0.1.0/obrpy/obrsdk/ova32.lib
+-rw-rw-rw-   0        0        0    28672 2023-04-25 10:36:31.000000 obrpy-0.1.0/obrpy/obrsdk/ovaGUI.dll
+-rw-rw-rw-   0        0        0     2123 2023-04-25 15:28:15.000000 obrpy-0.1.0/obrpy/obrsdk.py
+-rw-rw-rw-   0        0        0      972 2023-06-05 07:51:39.000000 obrpy-0.1.0/obrpy/save.py
+-rw-rw-rw-   0        0        0     3214 2023-06-19 09:15:05.000000 obrpy-0.1.0/obrpy/settings.py
+-rw-rw-rw-   0        0        0     3481 2023-06-20 08:20:09.000000 obrpy-0.1.0/obrpy/take_a_look.py
+-rw-rw-rw-   0        0        0     1743 2023-06-19 11:08:24.000000 obrpy-0.1.0/obrpy/to_export.py
+-rw-rw-rw-   0        0        0     3472 2023-06-05 08:18:45.000000 obrpy-0.1.0/obrpy/to_import.py
+drwxrwxrwx   0        0        0        0 2023-06-20 12:52:40.016205 obrpy-0.1.0/obrpy.egg-info/
+-rw-rw-rw-   0        0        0      283 2023-06-20 12:52:39.000000 obrpy-0.1.0/obrpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1275 2023-06-20 12:52:39.000000 obrpy-0.1.0/obrpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 12:52:39.000000 obrpy-0.1.0/obrpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      445 2023-06-20 12:52:39.000000 obrpy-0.1.0/obrpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-20 12:52:39.000000 obrpy-0.1.0/obrpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 12:52:42.009925 obrpy-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     2019 2023-06-20 12:52:32.000000 obrpy-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 12:52:42.006928 obrpy-0.1.0/test/
+-rw-rw-rw-   0        0        0     1039 2023-06-01 11:42:02.000000 obrpy-0.1.0/test/test.py
+-rw-rw-rw-   0        0        0      983 2023-06-20 08:18:30.000000 obrpy-0.1.0/test/test_dataset.py
+-rw-rw-rw-   0        0        0     2576 2023-06-19 10:59:54.000000 obrpy-0.1.0/test/test_export_obrfiles.py
+-rw-rw-rw-   0        0        0      624 2023-06-19 11:01:21.000000 obrpy-0.1.0/test/test_export_settings.py
+-rw-rw-rw-   0        0        0      622 2023-06-19 11:11:13.000000 obrpy-0.1.0/test/test_export_slices.py
+-rw-rw-rw-   0        0        0     1792 2023-06-20 10:57:12.000000 obrpy-0.1.0/test/test_obr_ini.py
+-rw-rw-rw-   0        0        0      700 2023-06-19 11:12:23.000000 obrpy-0.1.0/test/test_slices.py
```

### Comparing `obrpy-0.0.9/obrpy/PathSelector.py` & `obrpy-0.1.0/obrpy/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,8 +33,10 @@
         self.enter_button.grid(row=2, column=4)
 
     def select_path(self):
         """ Select a path """
         path = filedialog.askdirectory()
         self.path_entry.delete(0, tk.END)
         self.path_entry.insert(0, path)
-        self.path = path
+        self.path = path
+
+
```

### Comparing `obrpy-0.0.9/obrpy/obr.py` & `obrpy-0.1.0/obrpy/obr.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,108 +1,74 @@
 import os
 import pandas as pd
 import numpy as np
 import glob
-import sys
 
-sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
 from .UTILS.read_OBR import multi_read_OBR
 
 def mainOBR(self,limit1=None,limit2=None) -> None:
     """ Computes the following sequence:
             
         * First generates OBR book from OBR filenames and the date recorded in each .obr
                 
-            self.genOBRbook()
+            self.initOBR()
 
         * Then open each one and reads relevant information in the specified segment
                 
             self.computeOBR(limit1,limit2)
 
-        * Finally OBR information is saved
-                
-            self.save_OBRfiles() 
         
         :optional limit1 (float/bool)=None: Initial point of the region of interest 
         :optional limit2 (float/bool)=None: Final   point of the region of interest 
     
     """
 
-    self.genOBRbook()
+    self.initOBR()
     self.computeOBR(limit1,limit2)
-    self.save_OBRfiles()
 
-def genOBRbook(self,auto_overwrite=False) -> pd.DataFrame:
+def initOBR(self,auto_overwrite=False):
     """
     Function to generate OBR book from OBR filenames and the date recorded in each .obr
 
         :optional: auto_overwrite (bool) = False: if True the OBRbook will be auto-overwritten
         :returns: df (pd.Dataframe): dataframe from OBR book file
 
     """
 
     # Check current information
 
-    if self.OBRbook == None:
-        print('OBR book not found')
-        print(' Creating a new one ...')
-        save_df  = True
-        save_obj = True
-    elif self.OBRbook != None and len(self.OBRfiles) == 0:
-        print('OBR book found but not registered')
-        print(' Registering ...')
-        save_df  = False
-        save_obj = True
-    else:
-        print('OBR book found and registered')
+    if len(self.obrfiles.files) != 0:
+        print('OBR files already registered')
         if auto_overwrite==True:
             print(' Auto-overwrite enabled, OBRbook will be overwitten')
-            save_df  = True
-            save_obj = True
         else:
-            if 'n' in input(' Do you want to overwrite?(yes/no)'):
-                return self.OBRbook
-            else:
-                save_df  = True
-                save_obj = True
+            ans = input('\nOBR files already initialized (overwrite/quit):')
+            if 'o' in ans:
+                pass
+            if 'q' in ans:
+                return
+
 
     # Get all OBR files
-    OBR_files = find_OBR(os.path.join(self.path,self.folders['OBR']))
+    OBR_filenames = find_OBR(os.path.join(self.path,self.folders['OBR']))
+    
     # Initialize dataframe
     df = pd.DataFrame()
 
-    # Loop through OBR files
-    for filename in OBR_files:
+    # Loop through OBR files saving them into obrfiles.files dict
+    for filename in OBR_filenames:
         # Get date
         date = get_date(os.path.join(self.path,self.folders['OBR'],filename))
         # Get ID from date
         ID = ID_generator(date)
         # Append to object OBRfile
-        if save_obj:
-            self.OBRfiles[filename.replace('.obr','')] = self.OBRfile(ID,filename,date)
-        # Append to dataframe
-        df = df.append({
-            'ID':           ID,
-            'filename':     filename,
-            'date':         date},
-             ignore_index=True)
-        
+        self.obrfiles.files[filename.replace('.obr','')] = self.OBRfile(ID,filename,date)
         
-    # Sort dataframe by ID
-    df.sort_values('ID')
+    print('Done!')
 
-    # Save dataframe to csv
-    if save_df:
-        self.OBRbook = df
-        self.save_OBRbook()
-        # Return dataframe
-        return df
-    else:
-        print('Done!')
-        return df
 
 def computeOBR(self,limit1=None,limit2=None) -> None:
     """
     Reads all .obr files and registers information: f,z and Data = [Pc,Sc,Hc]
     among currently existing (filename, name, flecha, temperature and date)
 
     * If RAM is not able to allocate enough memory the object will be saved and
@@ -113,50 +79,43 @@
     :optional: limit2 (bool) = None
 
         * If both limits (limit1 and limit2) are None, a prompt will be displayed asking for them
         * If some limit  (limit1 or  limit2) is False, no prompt will be displayed asking for them and will be assumed that the users wants to keep the whole OBR readouts 
 
     """
 
-    # Check if information files exists
-    if not isinstance(self.OBRbook,pd.DataFrame) and len(self.OBRfiles) == 0:
-        print('\n','OBR book not found or not registered')
-        print('Please, create/register a new one calling')
-        print('DATASET.genOBRbook()')
-        return
-    else:
-        pass
-
     # Check for region of interest
     if limit1==None and limit2==None:
 
         if self.settings.info['Calibration'] is None and self.settings.info['Test'] is None:
             # If there is not settings file, display warning
             print('WARNING: No settings found')
             print('Please if you want to configure the DOFS settings run:')
-            print('     your_obrpy_object.genSettingsTemplate()')
-            print('and edit it')
+            print('>>     your_obrpy_object.genSettings(Calibration_df, Test_df)')
+            print('or')
+            print('>>     your_obrpy_object.genSettingsTemplate()')
+            print('edit it and then import the values with:')
+            print('>>     your_obrpy_object.import_settings("your/path/to/your/file.xslx")')
             print('WARNING: No limits were specified')
             print(' if you want to compute the full lenght of sensors leave empty the next prompts')
 
             limit1 = input(' Region of interest start point [m]: ')
             limit2 = input(' Region of interest end point [m]: ')
 
             limit1 = False if limit1 == "" else float(limit1)
             limit2 = False if limit2 == "" else float(limit2)
 
-
         else:
+            print('No limits were specified, taking ones from seetings')
             # Gets limits from settings
-            
             limit1 = self.settings.z_ini
             limit2 = self.settings.z_fin
 
     # Generate datasets from selected data
-    for key, OBRfile in self.OBRfiles.items():
+    for key, OBRfile in self.obrfiles.files.items():
 
         import psutil
         if psutil.virtual_memory()[2] < 90:
 
             if not hasattr(OBRfile, 'Data') or OBRfile.Data is None:
                 # Read .obr file
                 f,z,Data = multi_read_OBR([OBRfile.name],os.path.join(self.path,self.folders['OBR']),limit1=limit1,limit2=limit2)
@@ -167,19 +126,19 @@
             else:
                 pass
 
         else:
             # Esta parte hay que mejorarla para la 2.0
             print('\nUnable to allocate more information')
             print("DON'T PANIC the information will be saved")
-            print('just run again DATASETS.computeOBR() until no more .obr files are read')
+            print('just run again computeOBR() until no more .obr files are read')
             self.save()
             return False
-            exit()
 
+    print('Done!')
     return True
 
 def find_OBR(path:str, verbose=False) -> list:
     """ Function to find all .obr files from a folder
 
         param:  path      (str)          : path to folder
         return: OBR_files (list of str)  : list of OBR filenames
@@ -220,16 +179,22 @@
     DateTime=np.fromfile(file, count=8,dtype= 'uint16',offset = offset)                              # Measurement date
 
     DateTime=f'{DateTime[0]},{DateTime[1]},{DateTime[3]},{DateTime[4]}:{DateTime[5]}:{DateTime[6]}'  # "2022,03,03,13:41:27"
 
     return DateTime
 
 def ID_generator(date:str) -> str:
-    """ Function to create OBRfile ID. As is written now, it just takes the date and converts it into a plain integer 
     
-            :param: date (str): date where the measure was taken, it is formatted as %Y,%M,%D,%h:%m:%s
-            :returns: date formatted as: %Y%M%D%h%m%s (str)
+    """Function to create OBRfile ID. Modifies the input date string by removing commas and colons and adds a hyphen between the day and hour.
+    
+    :param date: Date where the measure was taken, formatted as %Y,%m,%d,%H:%M:%S
+    :returns: Date formatted as %Y%m%d-%H%M%S
     
     """
     
-    return date.replace(',','').replace(':','')
-
+    # Replace commas and colons with empty strings
+    formatted_date = date.replace(',', '').replace(':', '')
+    
+    # Insert a hyphen between the day and hour
+    formatted_date = formatted_date[:8] + '-' + formatted_date[8:]
+    
+    return formatted_date
```

### Comparing `obrpy-0.0.9/obrpy/obrsdk.py` & `obrpy-0.1.0/obrpy/obrsdk.py`

 * *Files identical despite different names*

### Comparing `obrpy-0.0.9/obrpy/save.py` & `obrpy-0.1.0/obrpy/to_import.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,107 +1,106 @@
 import os
-import pickle as pickle
 import pandas as pd
+from copy import deepcopy
 
-def save(self) -> None:
-    """ Save the object in the root of folder """
-
-    # Change self and its objects to global
-
-    if 'self' in globals():
-        pass
-    else:
-        globals()['self'] = self
-
-    for key in self.__dict__.keys():
-        if isinstance(self.__dict__[key], object):
-            globals()[key] = self.__dict__[key]
-
-    # Define path
-
-    path_to_dataset = os.path.join(self.path,self.name)
-
-    # Save with pickle
-
-    with open(path_to_dataset, 'wb') as outp:
-        pickle.dump(self.__dict__, outp, pickle.HIGHEST_PROTOCOL)
-    print(f'---> {self.name} saved!')
-
-    # Return self and its objects to local
-
-    if 'self' in globals():
-        del globals()['self']
-    else:
-        pass
-
-    for key in self.__dict__.keys():
-        if isinstance(self.__dict__[key], object):
-            del globals()[key]
-        else:
-            pass
-
-def save_something(self,object_to_save: object,path_to:str) -> None:
+def outside_(self):
+    
+    self.outside_OBRbook()
+    self.outside_settings()
+    self.outside_OBRfiles()
+
+def outside_OBRfiles(self):
+    """ Adds, to each OBRfile object in OBRfiles dict, all new atributes created in the OBRbook and updates OBRbook df from main class """
+
+    # Check if OBRbook exists
+    if not isinstance(self.OBRbook, pd.DataFrame):
+        print('ERROR: No OBRbook found')
+        print(' Please, run genOBRbook() first')
+        return
+
+    # Open file
+    book = deepcopy(self.OBRbook)
+
+    # Get list of all columns
+    columns = list(book.columns)
+    new_columns = deepcopy(columns)
+
+    # Read new attribues from OBRbook
+    new_columns.remove('ID')
+    new_columns.remove('filename')
+    new_columns.remove('date')
+
+    # Create atributes in OBRfile objects
+    for o in self.OBRfiles.values():
+        for atr in new_columns:
+            new_value = book.loc[book['ID'] == str(o.ID), atr].values[0]
+            setattr(o, atr, new_value)
     
-    """ Function to save something
-        :param: object_to_save (obj): object to be saved
-        :param: path_to (str): path to the directory where the object will be saved"""
-
 
-    # Save with pickle
-    with open(path_to, 'wb') as outp:
-        pickle.dump(object_to_save, outp, pickle.HIGHEST_PROTOCOL)
-    print('--> object saved in',path_to)
+def outside_OBRbook(self):
+    """ Adds, to each OBRfile object in OBRfiles dict, all new atributes created in the OBRbook and updates OBRbook df from main class """
 
-def save_OBRfiles(self) -> None:
+    # Check if OBRbook.csv exists
+    book_path = os.path.join(self.path,self.folders['INFORMATION'],self.INFO['OBR book filename'])
+    if not os.path.exists(book_path):
+        print('ERROR: No OBRbook saved as .csv')
+        print(' Please, run genOBRbook() first')
+        return
+    
+    # Update OBRbook
+    self.OBRbook = pd.read_csv(book_path)
 
-    """ Save OBRfiles once computed """
+def outside_settings(self):
+    """ Update settings from settings file new information """
 
-    path_to = os.path.join(self.path,self.folders['PROCESSED_DATA'],self.INFO['OBRfiles filename'])
-    object_to_save = self.OBRfiles
-    self.save_something(object_to_save,path_to)
-    print('--> OBRfiles saved in',path_to)
+    # Check if settings.xlsx exists
+    book_path = os.path.join(self.path,self.folders['INFORMATION'],self.INFO['settings filename'])
+    if not os.path.exists(book_path):
+        print(f'ERROR: No seetings file found in {book_path}')
+        print(' Please, run genSettingsTemplate() then edit it')
+        return
+    
+    # Update settings
+    excel_file = pd.read_excel(book_path, sheet_name=None)
+    self.settings.info['Calibration']   = excel_file['Calibration']
+    self.settings.info['Test']          = excel_file['Test']
+    self.settings.update()
 
-def save_OBRbook(self) -> None:
+def outside_slicesbook(self):
+    """ Updates slicesbook """
 
-    """ Save OBRbook as .csv"""
+    # Check if slicesbook.csv exists
+    book_path = os.path.join(self.path,self.folders['INFORMATION'],self.INFO['slices book filename'])
+    if not os.path.exists(book_path):
+        print('ERROR: No slicesbook already saved as .csv')
+        print(' Please, run genSlices() first')
+        return
     
-    book_path = os.path.join(self.path,self.folders['INFORMATION'],self.INFO['OBR book filename'])
-    self.OBRbook.to_csv(book_path, index=False)
-    print('--> OBRbook saved in', book_path)
+    # Update OBRbook
+    self.slicesbook = pd.read_csv(book_path)
 
+def outside_slicesbook_from_slices(self):
 
-def save_settings(self) -> None:
-
-    """ Save settings to .xlsx """
+    # Extract the attribute names from the first object in the list
+    attrs = [a for a in dir(self.slices[0]) if not a.startswith('__') and not a.startswith('P') and not a.startswith('S')]
+    
+    # Convert the list of objects into a list of dictionaries
+    data = [{attr: getattr(slice, attr) for attr in attrs} for slice in self.slices.slices]
 
-    # overwrite settings
-    book_path = os.path.join(self.path,self.folders['INFORMATION'],self.INFO['settings filename'])
-    writer = pd.ExcelWriter( book_path, engine='xlsxwriter')
+    # Convert the list of dictionaries into a Pandas DataFrame
+    self.slicesbook = pd.DataFrame(data)
 
-    # create the "Calibration" sheet
-    calibration_data = self.settings.info['Calibration']
-    calibration_data.to_excel(writer, sheet_name='Calibration', index=False)
+def outside_slices(self):
 
-    # create the "Test" sheet
-    test_data =self.settings.info['Test']
-    test_data.to_excel(writer, sheet_name='Test', index=False)
+    """ Updates slices form slicesbook """
 
-    # save the Excel file
-    writer.save()
-    print('--> settings file saved in', book_path)
+    ### TO BE DONE ###
 
-def save_slicesbook(self) -> None:
+    pass
 
-    """ Save slices book as .csv"""
+def outside_slices_from_slicesbook(self):
     
-    book_path = os.path.join(self.path,self.folders['INFORMATION'],self.INFO['slices book filename'])
-    self.slicesbook.to_csv(book_path, index=False)
-    print('--> slices book saved in', book_path)
-
-
-def save_slices(self) -> None:
+    """ Updates slices form slicesbook """
 
-    """ Save slices once computed """
+    ### TO BE DONE ###
 
-    path_to = os.path.join(self.path,self.folders['PROCESSED_DATA'],self.INFO['slices filename'])
-    object_to_save = self.slices
-    self.save_something(object_to_save,path_to)
+    pass
```

### Comparing `obrpy-0.0.9/obrpy/take_a_look.py` & `obrpy-0.1.0/obrpy/take_a_look.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 import sys
 import os
 import matplotlib.pyplot as plt
 import numpy as np
 
+def take_a_look(self):
+    pass
+
+"""
+
 sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
 from UTILS.read_OBR import multi_read_OBR
 from SIGNAL.spectral_shift import global_spectral_shift
 from SIGNAL.cross_spectrum import global_cross_spectrum_SS
 
 def take_a_look(self,REF,files,limit1=0, limit2 = 20, delta = 300, window = 1000, val='ss',plot=True, common_origin=False):
 
@@ -67,20 +72,22 @@
             lbl = file.replace('_',' ')
             z = z-z[0] if common_origin else z
             #plt.plot(z,val,'o',markersize=0.75,label=f'{lbl}')
             plt.plot(z,val,label=f'{lbl}')
         plt.ylabel(ylabel,fontsize=20,labelpad=15).set_rotation(0) if val == 'ss' else plt.ylabel(ylabel,fontsize=10,labelpad=8).set_rotation(0)
         plt.xlabel('z [m]')
 
-        """
+        """ """
         lgnd = plt.legend(numpoints=1, fontsize=10)
 
         #change the marker size manually for both lines
         lgnd.legendHandles[0]._legmarker.set_markersize(6)
         lgnd.legendHandles[1]._legmarker.set_markersize(6)
         lgnd.legendHandles[2]._legmarker.set_markersize(6)
-        """
+        """ """
         plt.legend()
         plt.grid()
         plt.show()
 
     return val_distributions
+
+"""
```

### Comparing `obrpy-0.0.9/test/test.py` & `obrpy-0.1.0/test/test.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,17 +2,22 @@
 import os
 sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
 
 from obrpy import obrpy
 
 obrpy_obj = obrpy('C:/Users/temis/0_CCMSS/CCMSS/1_Software/FOS/OBRpy/obrpy-base/test/folder_test')
 
+obrpy_obj.mainOBR()
+obrpy_obj.genSettings("Calibration")
+
+input('Open OBRbook, add T0, T1, E0 and E1 columns. Open seetings, write the name of the columns in settings. Once finished press any key to continue')
+
 obrpy_obj.update_OBRbook()
 obrpy_obj.update_OBRfiles()
-obrpy_obj.save()
+obrpy_obj.update_settings()
 
 obrpy_obj.genSlices()
 
 exit()
 
 Y0 = obrpy_obj.OBRfiles['2'].Data
 Y1 = obrpy_obj.OBRfiles['B11'].Data
```

