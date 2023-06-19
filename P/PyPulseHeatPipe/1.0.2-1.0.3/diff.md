# Comparing `tmp/PyPulseHeatPipe-1.0.2.tar.gz` & `tmp/PyPulseHeatPipe-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyPulseHeatPipe-1.0.2.tar", last modified: Wed Apr 19 00:25:17 2023, max compression
+gzip compressed data, was "PyPulseHeatPipe-1.0.3.tar", last modified: Mon Jun 19 23:05:38 2023, max compression
```

## Comparing `PyPulseHeatPipe-1.0.2.tar` & `PyPulseHeatPipe-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-04-19 00:25:17.776937 PyPulseHeatPipe-1.0.2/
--rw-r--r--   0 nirmal     (501) staff       (20)    35149 2023-04-18 23:45:06.000000 PyPulseHeatPipe-1.0.2/LICENSE
--rw-r--r--   0 nirmal     (501) staff       (20)     1872 2023-04-19 00:25:17.776985 PyPulseHeatPipe-1.0.2/PKG-INFO
-drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-04-19 00:25:17.775547 PyPulseHeatPipe-1.0.2/PyPulseHeatPipe/
--rw-r--r--   0 nirmal     (501) staff       (20)       75 2023-04-18 23:27:03.000000 PyPulseHeatPipe-1.0.2/PyPulseHeatPipe/__init__.py
--rw-r--r--   0 nirmal     (501) staff       (20)    11083 2023-04-15 10:09:07.000000 PyPulseHeatPipe-1.0.2/PyPulseHeatPipe/analysis.py
-drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-04-19 00:25:17.776584 PyPulseHeatPipe-1.0.2/PyPulseHeatPipe.egg-info/
--rw-r--r--   0 nirmal     (501) staff       (20)     1872 2023-04-19 00:25:17.000000 PyPulseHeatPipe-1.0.2/PyPulseHeatPipe.egg-info/PKG-INFO
--rw-r--r--   0 nirmal     (501) staff       (20)      337 2023-04-19 00:25:17.000000 PyPulseHeatPipe-1.0.2/PyPulseHeatPipe.egg-info/SOURCES.txt
--rw-r--r--   0 nirmal     (501) staff       (20)        1 2023-04-19 00:25:17.000000 PyPulseHeatPipe-1.0.2/PyPulseHeatPipe.egg-info/dependency_links.txt
--rw-r--r--   0 nirmal     (501) staff       (20)        1 2023-04-19 00:07:50.000000 PyPulseHeatPipe-1.0.2/PyPulseHeatPipe.egg-info/not-zip-safe
--rw-r--r--   0 nirmal     (501) staff       (20)       72 2023-04-19 00:25:17.000000 PyPulseHeatPipe-1.0.2/PyPulseHeatPipe.egg-info/requires.txt
--rw-r--r--   0 nirmal     (501) staff       (20)       16 2023-04-19 00:25:17.000000 PyPulseHeatPipe-1.0.2/PyPulseHeatPipe.egg-info/top_level.txt
--rw-r--r--   0 nirmal     (501) staff       (20)     1524 2023-04-19 00:17:50.000000 PyPulseHeatPipe-1.0.2/README.md
--rw-r--r--   0 nirmal     (501) staff       (20)       79 2023-04-19 00:25:17.777170 PyPulseHeatPipe-1.0.2/setup.cfg
--rw-r--r--   0 nirmal     (501) staff       (20)      772 2023-04-19 00:24:56.000000 PyPulseHeatPipe-1.0.2/setup.py
-drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-04-19 00:25:17.776718 PyPulseHeatPipe-1.0.2/test/
--rw-r--r--   0 nirmal     (501) staff       (20)       88 2023-04-18 21:04:27.000000 PyPulseHeatPipe-1.0.2/test/test.py
+drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-06-19 23:05:38.255387 PyPulseHeatPipe-1.0.3/
+-rw-r--r--   0 nirmal     (501) staff       (20)    35149 2023-04-18 23:45:06.000000 PyPulseHeatPipe-1.0.3/LICENSE
+-rw-r--r--   0 nirmal     (501) staff       (20)     2039 2023-06-19 23:05:38.255429 PyPulseHeatPipe-1.0.3/PKG-INFO
+drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-06-19 23:05:38.254054 PyPulseHeatPipe-1.0.3/PyPulseHeatPipe/
+-rw-r--r--   0 nirmal     (501) staff       (20)       75 2023-04-18 23:27:03.000000 PyPulseHeatPipe-1.0.3/PyPulseHeatPipe/__init__.py
+-rw-r--r--   0 nirmal     (501) staff       (20)    12723 2023-06-19 22:52:55.000000 PyPulseHeatPipe-1.0.3/PyPulseHeatPipe/analysis.py
+drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-06-19 23:05:38.255010 PyPulseHeatPipe-1.0.3/PyPulseHeatPipe.egg-info/
+-rw-r--r--   0 nirmal     (501) staff       (20)     2039 2023-06-19 23:05:38.000000 PyPulseHeatPipe-1.0.3/PyPulseHeatPipe.egg-info/PKG-INFO
+-rw-r--r--   0 nirmal     (501) staff       (20)      346 2023-06-19 23:05:38.000000 PyPulseHeatPipe-1.0.3/PyPulseHeatPipe.egg-info/SOURCES.txt
+-rw-r--r--   0 nirmal     (501) staff       (20)        1 2023-06-19 23:05:38.000000 PyPulseHeatPipe-1.0.3/PyPulseHeatPipe.egg-info/dependency_links.txt
+-rw-r--r--   0 nirmal     (501) staff       (20)        1 2023-04-19 00:07:50.000000 PyPulseHeatPipe-1.0.3/PyPulseHeatPipe.egg-info/not-zip-safe
+-rw-r--r--   0 nirmal     (501) staff       (20)       70 2023-06-19 23:05:38.000000 PyPulseHeatPipe-1.0.3/PyPulseHeatPipe.egg-info/requires.txt
+-rw-r--r--   0 nirmal     (501) staff       (20)       16 2023-06-19 23:05:38.000000 PyPulseHeatPipe-1.0.3/PyPulseHeatPipe.egg-info/top_level.txt
+-rw-r--r--   0 nirmal     (501) staff       (20)     1686 2023-06-19 22:40:16.000000 PyPulseHeatPipe-1.0.3/README.md
+-rw-r--r--   0 nirmal     (501) staff       (20)       79 2023-06-19 23:05:38.255602 PyPulseHeatPipe-1.0.3/setup.cfg
+-rw-r--r--   0 nirmal     (501) staff       (20)      773 2023-06-19 22:31:12.000000 PyPulseHeatPipe-1.0.3/setup.py
+drwxr-xr-x   0 nirmal     (501) staff       (20)        0 2023-06-19 23:05:38.255157 PyPulseHeatPipe-1.0.3/test/
+-rw-r--r--   0 nirmal     (501) staff       (20)    12724 2023-06-19 22:23:29.000000 PyPulseHeatPipe-1.0.3/test/test_analysis.py
```

### Comparing `PyPulseHeatPipe-1.0.2/LICENSE` & `PyPulseHeatPipe-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PyPulseHeatPipe-1.0.2/PKG-INFO` & `PyPulseHeatPipe-1.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: PyPulseHeatPipe
-Version: 1.0.2
+Version: 1.0.3
 Summary: The data analysis Python package for the Pulsating Heat Pipe experimental data
 Home-page: https://github.com/nirmalparmarphd/PyPulseHeatPipe
-Author: Nirmal Parmar
+Author: Nirmal Parmar, PhD
 Author-email: nirmalparmarphd@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PulseHeatPipe
 
@@ -15,23 +15,23 @@
 
 ### pkg installation
 ```
 pip install PyPulseHeatPipe
 ```
 ## Useage: 
 ### imorting the module
-    from PyPulseHeatPipe import PulsHeatPipe
+    from PyPulseHeatPipe import PulseHeatPipe
 ### creating the reference variable 
-    analysis = PulseHaatPipe("datapath")
+    analysis = PulseHaatPipe("datapath", "sample_name")
 ### for a class help 
     help(analysis)
 ### for a function help
     help(analysis.data_etl)
 ### using a function from the class
-    df, df_conv = analysis.data_etl
+    df, df_conv = analysis.data_etl()
 
 ## list of avilable functions
 1. data_etl
 2. gibbs_fe
 3. data_chop
 4. data_stat
 5. data_property_avg
@@ -42,27 +42,38 @@
 
 Example:
 ```
 # importing module
 from PyPulseHeatPipe import PulseHeatPipe
 from PyPulseHeatPipe import DataVisualisation
 
-analysis = PulseHeatPipe("data/al2o3_diwater_exp/60_FR/")
-visual = DataVisualisation('Al2O3_DI_60FR')
+analysis = PulseHeatPipe("datapaht", "sample_name")
+visual = DataVisualisation("datapaht", "sample_name")
 
 # calling help
 help(analysis.data_etl)
 help(visual.plot_all_data)
 
 # using methods eg;
+# for ETL
 df, df_conv = analysis.data_etl()
+
+# for visulisation of all thermal properties
 visual.plot_all_data(df_gfe)
 
 ```
 **NOTE**: The experimental data file must prepared in '.xlsx' formate. The data must contain atleast following columns with mentioned titles:
 
-** Data.xlsx format**
+>**samle_data.xlsx format**
+
+| 't(min)' | 'Tc[C] | 'Te[C]' | 'P[mmHg]' | 'Q[W]' | alpha | beta | phase |
+| --- | --- | --- | --- | --- | --- | --- | --- |
+| 1 | 30 | 35 | 700 | 80 | 90 | 0 | 2 |
+| --- | --- | --- | --- | --- | --- | --- | --- |
+
+here,
+
+alpha = vertical angle of PHP
+
+beta = horizontal angle of PHP
 
-| 'Time (Min)' | 'Tc - AVG (oC) | 'Te - AVG (oC)' | 'Pressure (mm of Hg)' | 'Te - Tc (oC)' | 'Q (W)' |'Resistance (oC/W)' |
-| --- | --- | --- | --- | --- | --- | --- |
-| 1 | 30 | 35 | 700 | 5 | 80 | 0.06 |
-| --- | --- | --- | --- | --- | --- | --- |
+phase = phase split of the working fluid
```

### Comparing `PyPulseHeatPipe-1.0.2/PyPulseHeatPipe/analysis.py` & `PyPulseHeatPipe-1.0.3/test/test_analysis.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,77 +7,97 @@
 import matplotlib.pyplot as plt
 import seaborn as sns
 sns.set()
 
 ## Data Analysis
 class PulseHeatPipe:
     """
-    ## PulseHeatPipe - Manually defined functions for Advanced Data Analysis and Machine Learning.
+    ## PulseHeatPipe is a Python library to perform thermodynamic data analysis on experimental data of pulsating heat pipe. This library is developed to estimate optimal working condition based on the change in Gibbs free energy in the pusating heat pipe.
+
+    Please find more detail at https://github.com/nirmalparmarphd/PyPulseHeatPipe 
 
     ## Useage: 
     ### imorting the module
-    from analysis import PulsHeatPipe
-    ### creating the reference variable 
-    analysis = PulseHaatPipe("datapath")
+    from PyPulseHeatPipe import PulsHeatPipe, DataVisualisation
+    ### setting working directory
+    analysis = PulseHaatPipe("datapath", "sample)
     ### for a class help 
     help(analysis)
     ### for a function help
     help(analysis.data_etl)
     ### using a function from the class
     df, df_conv = analysis.data_etl
-    
-    ## list of avilable functions
-    1. data_etl
-    2. gibbs_fe
-    3. data_chop
-    4. data_stat
-    5. data_property_avg
-    6. best_TP
-    7. plot_all_data
-    8. plot_Te_Tc
-    9. plot_eu
     """
-    def __init__(self, datapath:str):
+    def __init__(self, datapath:str, sample:str):
         self.T_k = 273.15 # To convert in kelvin
         self.P_const = 750.062 # To convert in bar
         self.R_const = 8.314 # Real Gas constant
         self.dG_standard = 30.9 # dG of water
         self.P_standard = 1 # atomospher pressure
         self.datapath = datapath
-        print(f"Data loaded from directory: {self.datapath}")
+        self.sample = sample
+        print(f"Datapath loaded for working directory: {self.datapath}\n")
+        print(f"Sample name saved as: {self.sample}")
 
+    # sample xlsx blank file
+    def blank_file(self, blank='blank.xlsx'):
+        """
+        blank_file is a method to generate a blank sample (.xlsx) file to prepare data file that can futher used in thermodynamic analysis. 
+        
+        't(min)'= timestemp,
+        'Te[C]'= Eveporator Temperature,
+        'Tc[C]'= Condensor Temperature,
+        'P[mmHg]'= Pressure of PHP,
+        'Q[W]'= Power Supply,
+        'alpha'= Horizontal Angle of PHP,
+        'beta'= Vertical Angle of PHP, 
+        'phase'= Visible phase split (y/n)
+
+        useage: analysis = PulseHeatPipe("path")
+                analysis.blank_file()
+        """
+        self.blank = blank
+        df_blank = pd.DataFrame({'t(min)':[1] ,'Te[C]':[1], 'Tc[C]':[1],'P[mmHg]':[1], 'Q[W]':[1], 'alpha':[1], 'beta':[1], 'phase':[1]})
+        # creating blank file
+        df_blank_out = df_blank.to_excel(self.datapath + self.blank)
+        msg = (f"### {self.blank} file is created. Please enter the experimental data in this file. Do not ulter or change of the column's head. ###");
+        return msg
+    
     # data ETL    
-    def data_etl(self):
+    def data_etl(self, name='*', ext='.xlsx'):
         """
         data_etl loads experimental data from all experimental data files (xlsx).
         Filters data and keeps only important columns.
         Combine selected data and save to csv file.
         Conver units to MKS [K, bar] system and save to csv file. 
 
-        useage: analysis = PulseHeatPipe("path")
+        useage: analysis = PulseHeatPipe("path", "sample")
                 df, df_conv = analysis.data_etl()
         """
-        data_filenames_list = glob.glob((self.datapath + 'php_*.xlsx'))
+        self.name = name
+        self.ext = ext
+        data_filenames_list = glob.glob((self.datapath + self.name + self.ext))
         df_frames = []
+        print('list of files considered for ETL: \n',data_filenames_list)
         for i in range(0, len(data_filenames_list)) :
             # loading data in loop
-            df_raw = pd.read_excel((data_filenames_list[i]))
-            selected_columns = ['Time (Min)', 'Tc - AVG (oC)', 'Te - AVG (oC)', 'Pressure (mm of Hg)', 'Te - Tc (oC)', 'Q (W)','Resistance (oC/W)']
+            df_raw = pd.read_excel(data_filenames_list[i])
+            selected_columns = ['t(min)' ,'Te[C]', 'Tc[C]','P[mmHg]', 'Q[W]', 'alpha', 'beta', 'phase']
             df_selected_columns = df_raw[selected_columns]
             df_frames.append(df_selected_columns)
-            df = pd.concat(df_frames, axis=0, ignore_index=True).dropna()
-        # converting data to MKS
-        df_conv_fram = [df['Time (Min)'], df['Te - AVG (oC)']+self.T_k, df['Tc - AVG (oC)']+self.T_k, df['Te - Tc (oC)'] , df['Pressure (mm of Hg)']/self.P_const, df['Resistance (oC/W)']]
+        df = pd.concat(df_frames, axis=0, ignore_index=True).dropna()
+      
+        df_conv_fram = [df['t(min)'], df['Te[C]']+self.T_k, df['Tc[C]']+self.T_k, df['Te[C]']-df['Tc[C]'] , df['P[mmHg]']/self.P_const, df['Q[W]'], (df['Te[C]']-df['Tc[C]'])/df['Q[W]'] , df['alpha'], df['beta'], df['phase']]
         df_conv = pd.concat(df_conv_fram, axis=1, ignore_index=True).dropna()
-        df_conv_columns = ['t(min)' ,'Te[K]', 'Tc[K]', 'dT[K]', 'P[bar]', 'TR[K/W]']
+        df_conv_columns = ['t(min)' ,'Te[K]', 'Tc[K]', 'dT[K]', 'P[bar]', 'Q[W]', 'TR[K/W]','alpha', 'beta', 'phase']
         df_conv.columns = df_conv_columns
-        # saving data to csv
-        df_out = df.to_csv(self.datapath + "combined_data.csv")
-        df_conv_out = df_conv.to_csv(self.datapath + "combined_converted_data.csv")
-        print(f"Compiled and converted data is saved at: {self.datapath}'combined_converted_data.csv'")
+        # saving
+        df_out = df.to_csv(self.datapath + self.sample + "_combined_data.csv")
+        df_conv_out = df_conv.to_csv(self.datapath + self.sample + "_combined_converted_data.csv")
+        print(f"### Compiled and converted data is saved at: {self.datapath}'{self.sample}_combined_converted_data.csv' ###")
         return df, df_conv
     
     # to calculate gibbs free energy at given (T[K],P[bar])
     def gibbs_fe(self, data:pd.DataFrame):
         """
         gibbs_fe calculates the chagne in the gibbs free energy at a given vacuum pressure and temperature.
         dG = dG' + RTln(P/P')
@@ -89,15 +109,15 @@
         """
         Te = (data['Te[K]']) 
         Tc = (data['Tc[K]'])  
         P_vacuum = (data['P[bar]']) # converting to bar
         dG_vacuume_Te = self.R_const * Te * np.log(P_vacuum/self.P_standard)
         dG_vacuume_Tc = self.R_const * Tc * np.log(P_vacuum/self.P_standard)
         dG = dG_vacuume_Te - dG_vacuume_Tc
-        selected_columns = ['t(min)' ,'Te[K]', 'Tc[K]', 'dT[K]', 'P[bar]', 'TR[K/W]', 'GFE[KJ/mol]', 'GFE_Tc[KJ/mol]', 'dG[KJ/mol]']
+        selected_columns = ['t(min)' ,'Te[K]', 'Tc[K]', 'dT[K]', 'P[bar]', 'Q[W]', 'TR[K/W]','alpha', 'beta', 'phase', 'GFE_Te[KJ/mol]', 'GFE_Tc[KJ/mol]', 'dG[KJ/mol]']
         data = pd.concat([data, dG_vacuume_Te, dG_vacuume_Tc, dG], axis=1, ignore_index=True)
         data.columns = selected_columns
         data_out = data.to_csv(self.datapath + "gfe_combined.csv")
         msg = print(f"Gibbs Free Energy calculated data saved at: {self.datapath}'gfe_combined.csv")
         return data
     
     # To select data from specific Te range
@@ -114,24 +134,24 @@
         assert Tmin < Tmax, f"Entered wrong values: Correct range [Tmin:{round(Tmina,4)}, Tmax:{round(Tmaxa,4)} ]"
         print(f"Optimal range of temperature(Te) for data selection: [Tmin:{round(Tmina,4)}, Tmax:{round(Tmaxa)}]")
         data_T = data[data['Te[K]'] <= Tmax]
         data_T = data_T[data_T['Te[K]'] >= Tmin]
         return data_T
     
         # data mixing and re-arranging
-    def data_stat(self, data:pd.DataFrame):
+    def data_stat(self, data:pd.DataFrame, property = 'Te[K]'):
         """
         data_stat sorts and arrange value by a group from the experimental data loaded with data_etl function, calculates mean and standard deviation of the grouped data.
         Calculated result will be stored at the location of data files.
 
         df_mean, df_std = analysis.data_stat(data)
         """
-        df_mean = data.sort_values(by=['Te[K]']).groupby(['Te[K]'], as_index=False).mean()
+        df_mean = data.sort_values(by=property).groupby(property, as_index=False).mean()
         df_mean_out = df_mean.to_csv(self.datapath + 'combined_mean.csv')
-        df_std = data.sort_values(by=['Te[K]']).groupby(['Te[K]'], as_index=False).std().dropna()
+        df_std = data.sort_values(by=property).groupby(property, as_index=False).std().dropna()
         df_std_out = df_std.to_csv(self.datapath + 'combined_std.csv')
         print(f"Calculated mean and standard deviation values saved at {self.datapath}'combined_mean.csv' and 'combined_std.csv'")
         return df_mean, df_std
     
     # prepare average values for all thermal properties
     def data_property_avg(self, df_mean:pd.DataFrame, df_std:pd.DataFrame):
         """
@@ -140,21 +160,21 @@
         useage: analysis.data_property_avg(df_mean, df_std)
         """
         # avg values 
         Tc_avg = df_mean['Tc[K]'].mean()
         P_avg = df_mean['P[bar]'].mean()
         dT_avg = df_mean['dT[K]'].mean()
         TR_avg = df_mean['TR[K/W]'].mean()
-        GFE_avg = df_mean['GFE[KJ/mol]'].mean()
+        GFE_avg = df_mean['GFE_Tc[KJ/mol]'].mean()
         # std values
         Tc_std = df_std['Tc[K]'].mean()
         P_std = df_std['P[bar]'].mean()
         dT_std = df_std['dT[K]'].mean()
         TR_std = df_std['TR[K/W]'].mean()
-        GFE_std = df_std['GFE[KJ/mol]'].mean()
+        GFE_std = df_std['GFE_Tc[KJ/mol]'].mean()
         # calculated results
         msg = (f"Tc  average:     {round(Tc_avg,4)} +- {round(Tc_std,4)} [K]\n"
         f"P   average:     {round(P_avg,4)} +- {round(P_std,4)} [bar]\n"
         f"dT  average:     {round(dT_avg,4)} +- {round(dT_std,4)} [K]\n"
         f"TR  average:     {round(TR_avg,4)} +- {round(TR_std,4)} [K/W]\n"
         f"GFE average:     {round(GFE_avg,4)} +- {round(GFE_std,4)} [KJ/mol]\n");
         return print(msg)
@@ -164,21 +184,23 @@
         """ 
         best_TP finds best G(T,P) with lowest dG (Change in Gibbs Free Energy for Te->Tc values at constant Pressure) from the experimental dataset.
 
         useage: analysis.best_TP(data)
         """
         df_opt = data[data['dG[KJ/mol]'] == data['dG[KJ/mol]'].min()]
         df_opt_idx = df_opt.index
+        Tc_opt = data['Tc[K]'].loc[df_opt_idx]
         Te_opt = data['Te[K]'].loc[df_opt_idx]
         dT_opt = data['dT[K]'].loc[df_opt_idx]
         P_opt = data['P[bar]'].loc[df_opt_idx]
         dG_opt = data['dG[KJ/mol]'].loc[df_opt_idx]
-        GFE_opt = data['GFE[KJ/mol]'].loc[df_opt_idx]
+        GFE_opt = data['GFE_Tc[KJ/mol]'].loc[df_opt_idx]
         TR_opt = data['TR[K/W]'].loc[df_opt_idx]
         msg = (f'Optimal G(T,P) condition at lowest (optimal) dG[{round(dG_opt.iloc[0],4)}]\n'
+               f'Tc optimal:        {round(Tc_opt.iloc[0],4)}[K] \n'
                f'Te optimal:        {round(Te_opt.iloc[0],4)}[K] \n'
                f'P  optimal:        {round(P_opt.iloc[0],4)}[bar] \n'
                f'dT optimal:        {round(dT_opt.iloc[0],4)}[K] \n'
                f'TR optimal:        {round(TR_opt.iloc[0],4)}[K/W] \n'
                f'GFE optimal:       dG({round(Te_opt.iloc[0],4)}, {round(P_opt.iloc[0],4)}) = {round(GFE_opt.iloc[0],4)} [KJ/mol]\n');
         return print(msg)
     
@@ -190,18 +212,17 @@
         ### importing module
         from analysis import DataVisualisation
         ### creating the reference variable
         visual = DataVisualisation('sample')
         ### data visualisation; eg. plotting all data
         visual.plot_all_data()
     """
-    def __init__(self, sample: str):
-        super().__init__(sample)
-        self.sample = sample
-
+    def __init__(self, datapath: str, sample: str):
+        super().__init__(datapath, sample)
+        
     def plot_all_data(self, data:pd.DataFrame):
         """ Data Visualisation
             
             useage: visual.plot_all_data(data)
         """
         plt.figure(figsize=(10,5))
         sns.lineplot(data)
@@ -223,21 +244,21 @@
         plt.title(f"Te[K] vs Tc[K] - {self.sample}")
         plt.legend()
 
     def plot_eu(self, df_mean:pd.DataFrame, df_std:pd.DataFrame, property:str, point='.k', eu='r'):
         """ Data Visualisation
             
             useage: visual.plot_eu(df_mean, df_std, property='Tc[K]', point='.k', eu='r')
-                    here, choose value from property list: ['Tc[K]', 'dT[K]', 'P[bar]', 'TR[K/W]', 'GFE[KJ/mol]', 'GFE_Tc[KJ/mol]', 'dG[KJ/mol]']
+                    here, choose value from property list: ['Tc[K]', 'dT[K]', 'P[bar]', 'TR[K/W]', 'GFE_Te[KJ/mol]', 'GFE_Tc[KJ/mol]', 'dG[KJ/mol]']
         """
         self.property = property
         self.xproperty = 'Te[K]'
         self.point = point
         self.eu = eu
-        properties = ['Tc[K]', 'dT[K]', 'P[bar]', 'TR[K/W]', 'GFE[KJ/mol]', 'GFE_Tc[KJ/mol]', 'dG[KJ/mol]']
+        properties = ['Tc[K]', 'dT[K]', 'P[bar]', 'TR[K/W]', 'GFE_Te[KJ/mol]', 'GFE_Tc[KJ/mol]', 'dG[KJ/mol]']
         if self.property in properties:    
             plt.figure(figsize=(10,5));
             plt.plot(df_mean[self.xproperty], df_mean[self.property], self.point, label=self.property)
             idx = df_std.index
             df_mean_idx = df_mean.loc[idx]
             plt.fill_between(df_std[self.xproperty], df_mean_idx[self.property] - 2* df_std[self.property], df_mean_idx[self.property] + 2* df_std[self.property],color=self.eu, alpha=0.2, label='Expanded Uncertainty')
             plt.xlabel(self.xproperty)
```

### Comparing `PyPulseHeatPipe-1.0.2/PyPulseHeatPipe.egg-info/PKG-INFO` & `PyPulseHeatPipe-1.0.3/PyPulseHeatPipe.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: PyPulseHeatPipe
-Version: 1.0.2
+Version: 1.0.3
 Summary: The data analysis Python package for the Pulsating Heat Pipe experimental data
 Home-page: https://github.com/nirmalparmarphd/PyPulseHeatPipe
-Author: Nirmal Parmar
+Author: Nirmal Parmar, PhD
 Author-email: nirmalparmarphd@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PulseHeatPipe
 
@@ -15,23 +15,23 @@
 
 ### pkg installation
 ```
 pip install PyPulseHeatPipe
 ```
 ## Useage: 
 ### imorting the module
-    from PyPulseHeatPipe import PulsHeatPipe
+    from PyPulseHeatPipe import PulseHeatPipe
 ### creating the reference variable 
-    analysis = PulseHaatPipe("datapath")
+    analysis = PulseHaatPipe("datapath", "sample_name")
 ### for a class help 
     help(analysis)
 ### for a function help
     help(analysis.data_etl)
 ### using a function from the class
-    df, df_conv = analysis.data_etl
+    df, df_conv = analysis.data_etl()
 
 ## list of avilable functions
 1. data_etl
 2. gibbs_fe
 3. data_chop
 4. data_stat
 5. data_property_avg
@@ -42,27 +42,38 @@
 
 Example:
 ```
 # importing module
 from PyPulseHeatPipe import PulseHeatPipe
 from PyPulseHeatPipe import DataVisualisation
 
-analysis = PulseHeatPipe("data/al2o3_diwater_exp/60_FR/")
-visual = DataVisualisation('Al2O3_DI_60FR')
+analysis = PulseHeatPipe("datapaht", "sample_name")
+visual = DataVisualisation("datapaht", "sample_name")
 
 # calling help
 help(analysis.data_etl)
 help(visual.plot_all_data)
 
 # using methods eg;
+# for ETL
 df, df_conv = analysis.data_etl()
+
+# for visulisation of all thermal properties
 visual.plot_all_data(df_gfe)
 
 ```
 **NOTE**: The experimental data file must prepared in '.xlsx' formate. The data must contain atleast following columns with mentioned titles:
 
-** Data.xlsx format**
+>**samle_data.xlsx format**
+
+| 't(min)' | 'Tc[C] | 'Te[C]' | 'P[mmHg]' | 'Q[W]' | alpha | beta | phase |
+| --- | --- | --- | --- | --- | --- | --- | --- |
+| 1 | 30 | 35 | 700 | 80 | 90 | 0 | 2 |
+| --- | --- | --- | --- | --- | --- | --- | --- |
+
+here,
+
+alpha = vertical angle of PHP
+
+beta = horizontal angle of PHP
 
-| 'Time (Min)' | 'Tc - AVG (oC) | 'Te - AVG (oC)' | 'Pressure (mm of Hg)' | 'Te - Tc (oC)' | 'Q (W)' |'Resistance (oC/W)' |
-| --- | --- | --- | --- | --- | --- | --- |
-| 1 | 30 | 35 | 700 | 5 | 80 | 0.06 |
-| --- | --- | --- | --- | --- | --- | --- |
+phase = phase split of the working fluid
```

### Comparing `PyPulseHeatPipe-1.0.2/README.md` & `PyPulseHeatPipe-1.0.3/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 
 ### pkg installation
 ```
 pip install PyPulseHeatPipe
 ```
 ## Useage: 
 ### imorting the module
-    from PyPulseHeatPipe import PulsHeatPipe
+    from PyPulseHeatPipe import PulseHeatPipe
 ### creating the reference variable 
-    analysis = PulseHaatPipe("datapath")
+    analysis = PulseHaatPipe("datapath", "sample_name")
 ### for a class help 
     help(analysis)
 ### for a function help
     help(analysis.data_etl)
 ### using a function from the class
-    df, df_conv = analysis.data_etl
+    df, df_conv = analysis.data_etl()
 
 ## list of avilable functions
 1. data_etl
 2. gibbs_fe
 3. data_chop
 4. data_stat
 5. data_property_avg
@@ -31,27 +31,38 @@
 
 Example:
 ```
 # importing module
 from PyPulseHeatPipe import PulseHeatPipe
 from PyPulseHeatPipe import DataVisualisation
 
-analysis = PulseHeatPipe("data/al2o3_diwater_exp/60_FR/")
-visual = DataVisualisation('Al2O3_DI_60FR')
+analysis = PulseHeatPipe("datapaht", "sample_name")
+visual = DataVisualisation("datapaht", "sample_name")
 
 # calling help
 help(analysis.data_etl)
 help(visual.plot_all_data)
 
 # using methods eg;
+# for ETL
 df, df_conv = analysis.data_etl()
+
+# for visulisation of all thermal properties
 visual.plot_all_data(df_gfe)
 
 ```
 **NOTE**: The experimental data file must prepared in '.xlsx' formate. The data must contain atleast following columns with mentioned titles:
 
-** Data.xlsx format**
+>**samle_data.xlsx format**
+
+| 't(min)' | 'Tc[C] | 'Te[C]' | 'P[mmHg]' | 'Q[W]' | alpha | beta | phase |
+| --- | --- | --- | --- | --- | --- | --- | --- |
+| 1 | 30 | 35 | 700 | 80 | 90 | 0 | 2 |
+| --- | --- | --- | --- | --- | --- | --- | --- |
+
+here,
+
+alpha = vertical angle of PHP
+
+beta = horizontal angle of PHP
 
-| 'Time (Min)' | 'Tc - AVG (oC) | 'Te - AVG (oC)' | 'Pressure (mm of Hg)' | 'Te - Tc (oC)' | 'Q (W)' |'Resistance (oC/W)' |
-| --- | --- | --- | --- | --- | --- | --- |
-| 1 | 30 | 35 | 700 | 5 | 80 | 0.06 |
-| --- | --- | --- | --- | --- | --- | --- |
+phase = phase split of the working fluid
```

### Comparing `PyPulseHeatPipe-1.0.2/setup.py` & `PyPulseHeatPipe-1.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(name='PyPulseHeatPipe',
-        version='1.0.2',
+        version='1.0.3',
         license='GNU',
         url='https://github.com/nirmalparmarphd/PyPulseHeatPipe',
         description='The data analysis Python package for the Pulsating Heat Pipe experimental data', 
         long_description=long_description,
         long_description_content_type='text/markdown',
-        author='Nirmal Parmar',
+        author='Nirmal Parmar, PhD',
         author_email='nirmalparmarphd@gmail.com',
         packages=setuptools.find_packages(),
         include_package_data=True,
-        install_requires=['scikit-learn','numpy','keras', 'gitpython', 'pandas','h5py', 'scipy', 'matplotlib', 'seaborn'],
+        install_requires=['scikit-learn','numpy', 'gitpython', 'pandas','scipy', 'matplotlib', 'seaborn', 'openpyxl'],
         zip_safe=False)
```

