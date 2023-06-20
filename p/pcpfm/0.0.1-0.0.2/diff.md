# Comparing `tmp/pcpfm-0.0.1.tar.gz` & `tmp/pcpfm-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcpfm-0.0.1.tar", last modified: Sun Jun  4 23:29:14 2023, max compression
+gzip compressed data, was "pcpfm-0.0.2.tar", last modified: Tue Jun 20 19:41:32 2023, max compression
```

## Comparing `pcpfm-0.0.1.tar` & `pcpfm-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 mitchjo  (935526437) 1088672553        0 2023-06-04 23:29:14.550370 pcpfm-0.0.1/
--rw-r--r--   0 mitchjo  (935526437) 1088672553     1298 2023-06-02 20:20:23.000000 pcpfm-0.0.1/LICENSE
--rw-r--r--   0 mitchjo  (935526437) 1088672553     9343 2023-06-04 23:29:14.549948 pcpfm-0.0.1/PKG-INFO
--rw-r--r--   0 mitchjo  (935526437) 1088672553     8475 2023-06-02 16:51:22.000000 pcpfm-0.0.1/README.md
-drwxr-xr-x   0 mitchjo  (935526437) 1088672553        0 2023-06-04 23:29:14.546036 pcpfm-0.0.1/pcpfm/
--rw-r--r--   0 mitchjo  (935526437) 1088672553    16703 2023-06-04 21:38:56.000000 pcpfm-0.0.1/pcpfm/Acquisition.py
--rw-r--r--   0 mitchjo  (935526437) 1088672553    15619 2023-06-01 15:48:56.000000 pcpfm-0.0.1/pcpfm/EmpCpds.py
--rw-r--r--   0 mitchjo  (935526437) 1088672553    14322 2023-06-04 21:32:17.000000 pcpfm-0.0.1/pcpfm/Experiment.py
--rw-r--r--   0 mitchjo  (935526437) 1088672553    32508 2023-06-04 20:43:48.000000 pcpfm-0.0.1/pcpfm/FeatureTable.py
--rw-r--r--   0 mitchjo  (935526437) 1088672553     2421 2023-06-02 13:45:01.000000 pcpfm-0.0.1/pcpfm/ThermoRawFileConverter.py
--rw-r--r--   0 mitchjo  (935526437) 1088672553       21 2023-06-04 21:21:16.000000 pcpfm-0.0.1/pcpfm/__init__.py
--rw-r--r--   0 mitchjo  (935526437) 1088672553    15527 2023-06-04 21:38:36.000000 pcpfm-0.0.1/pcpfm/main.py
-drwxr-xr-x   0 mitchjo  (935526437) 1088672553        0 2023-06-04 23:29:14.549441 pcpfm-0.0.1/pcpfm.egg-info/
--rw-r--r--   0 mitchjo  (935526437) 1088672553     9343 2023-06-04 23:29:14.000000 pcpfm-0.0.1/pcpfm.egg-info/PKG-INFO
--rw-r--r--   0 mitchjo  (935526437) 1088672553      346 2023-06-04 23:29:14.000000 pcpfm-0.0.1/pcpfm.egg-info/SOURCES.txt
--rw-r--r--   0 mitchjo  (935526437) 1088672553        1 2023-06-04 23:29:14.000000 pcpfm-0.0.1/pcpfm.egg-info/dependency_links.txt
--rw-r--r--   0 mitchjo  (935526437) 1088672553       41 2023-06-04 23:29:14.000000 pcpfm-0.0.1/pcpfm.egg-info/entry_points.txt
--rw-r--r--   0 mitchjo  (935526437) 1088672553       62 2023-06-04 23:29:14.000000 pcpfm-0.0.1/pcpfm.egg-info/requires.txt
--rw-r--r--   0 mitchjo  (935526437) 1088672553        6 2023-06-04 23:29:14.000000 pcpfm-0.0.1/pcpfm.egg-info/top_level.txt
--rw-r--r--   0 mitchjo  (935526437) 1088672553       38 2023-06-04 23:29:14.550428 pcpfm-0.0.1/setup.cfg
--rw-r--r--   0 mitchjo  (935526437) 1088672553     1501 2023-06-04 21:24:17.000000 pcpfm-0.0.1/setup.py
+drwxr-xr-x   0 mitchjo  (935526437) 1088672553        0 2023-06-20 19:41:32.462859 pcpfm-0.0.2/
+-rw-r--r--   0 mitchjo  (935526437) 1088672553     1298 2023-06-02 20:20:23.000000 pcpfm-0.0.2/LICENSE
+-rw-r--r--   0 mitchjo  (935526437) 1088672553    10220 2023-06-20 19:41:32.462569 pcpfm-0.0.2/PKG-INFO
+-rw-r--r--   0 mitchjo  (935526437) 1088672553     9352 2023-06-19 23:43:01.000000 pcpfm-0.0.2/README.md
+drwxr-xr-x   0 mitchjo  (935526437) 1088672553        0 2023-06-20 19:41:32.437116 pcpfm-0.0.2/pcpfm/
+-rw-r--r--   0 mitchjo  (935526437) 1088672553    15714 2023-06-12 19:47:19.000000 pcpfm-0.0.2/pcpfm/Acquisition.py
+-rw-r--r--   0 mitchjo  (935526437) 1088672553    16044 2023-06-14 19:33:31.000000 pcpfm-0.0.2/pcpfm/EmpCpds.py
+-rw-r--r--   0 mitchjo  (935526437) 1088672553    15781 2023-06-18 20:28:49.000000 pcpfm-0.0.2/pcpfm/Experiment.py
+-rw-r--r--   0 mitchjo  (935526437) 1088672553    43499 2023-06-18 20:25:02.000000 pcpfm-0.0.2/pcpfm/FeatureTable.py
+-rw-r--r--   0 mitchjo  (935526437) 1088672553     2436 2023-06-09 16:59:59.000000 pcpfm-0.0.2/pcpfm/ThermoRawFileConverter.py
+-rw-r--r--   0 mitchjo  (935526437) 1088672553       21 2023-06-20 19:40:02.000000 pcpfm-0.0.2/pcpfm/__init__.py
+-rw-r--r--   0 mitchjo  (935526437) 1088672553    18425 2023-06-18 20:23:29.000000 pcpfm-0.0.2/pcpfm/main.py
+drwxr-xr-x   0 mitchjo  (935526437) 1088672553        0 2023-06-20 19:41:32.462104 pcpfm-0.0.2/pcpfm.egg-info/
+-rw-r--r--   0 mitchjo  (935526437) 1088672553    10220 2023-06-20 19:41:32.000000 pcpfm-0.0.2/pcpfm.egg-info/PKG-INFO
+-rw-r--r--   0 mitchjo  (935526437) 1088672553      346 2023-06-20 19:41:32.000000 pcpfm-0.0.2/pcpfm.egg-info/SOURCES.txt
+-rw-r--r--   0 mitchjo  (935526437) 1088672553        1 2023-06-20 19:41:32.000000 pcpfm-0.0.2/pcpfm.egg-info/dependency_links.txt
+-rw-r--r--   0 mitchjo  (935526437) 1088672553       41 2023-06-20 19:41:32.000000 pcpfm-0.0.2/pcpfm.egg-info/entry_points.txt
+-rw-r--r--   0 mitchjo  (935526437) 1088672553       71 2023-06-20 19:41:32.000000 pcpfm-0.0.2/pcpfm.egg-info/requires.txt
+-rw-r--r--   0 mitchjo  (935526437) 1088672553        6 2023-06-20 19:41:32.000000 pcpfm-0.0.2/pcpfm.egg-info/top_level.txt
+-rw-r--r--   0 mitchjo  (935526437) 1088672553       38 2023-06-20 19:41:32.462923 pcpfm-0.0.2/setup.cfg
+-rw-r--r--   0 mitchjo  (935526437) 1088672553     1501 2023-06-04 21:24:17.000000 pcpfm-0.0.2/setup.py
```

### Comparing `pcpfm-0.0.1/LICENSE` & `pcpfm-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pcpfm-0.0.1/PKG-INFO` & `pcpfm-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcpfm
-Version: 0.0.1
+Version: 0.0.2
 Summary: LC-MS metabolomics data processing pipeline
 Home-page: https://github.com/jmmitc06/PythonCentricPipelineForMetabolomics
 Author: Joshua Mitchell
 Author-email: joshua.mitchell@jax.org
 License: MIT
 Keywords: metabolomics bioinformatics mass spectrometry
 Classifier: Intended Audience :: Developers
@@ -16,16 +16,32 @@
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+# Disclaimer
+
+Thanks for your interest in the PCPFM! If you talked to me at the Metabolomics2023 conference thanks for giving this project a try. This project is still an alpha. While I'm not aware of any issues that could cause data quality issues, use at your at your own risk!
+
+I just did a major refactor and the Nextflow implementation is out of date along with some of the documentation. I will be working on fixing these things by the end of June. If there is a feature or change you think would make a good addition, feel free to contact me and/or open an issue on the repo. 
+
 # PythonCentricPipelineForMetabolomics (PCPFM)
 
+NOTE - documentation below is out of date and will be updated in the next week or so 06/16
+
+to-implement:
+  - new nextflow wrappers
+  - direct annotation of feature tables
+  - auto drop samples based on QC metrics
+  - auto drop features based on QC metrics
+  - mzML experiment construction
+
+
 ## Overview
 
 The PythonCentricPipelineForMetabolomics (PCPMF) is an all-in-one pipeline for processing LC-MS based metabolomics datasets. Currently supported is limited to datasets collected on Thermo instruments; however, this will be expanded in the future. 
 
 The pipeline includes ingesting and converting .raw files to their .mzML representations with the ThermoRawFileParser, feature extraction and pre-annotation with Asari and Khipu respectively, optional manual and/or automated QA/QC, feature normalization, blank masking and (soon) batch correction. 
 
 The input to the pipeline is a .csv file that minimally has 'Name' and 'Filepath' field storing each Acquisition's name and raw filepath respectively. This csv file is intended to be the sequence file used during acquisition on the LC-MS. An Experiment object, which encaptulates all acquisitions from an experiment (should be the same ionization, chromatography, and mass spectrometry method), is used to move data and intermediates between steps. All information is stored in a user-defined experiment directory
```

### Comparing `pcpfm-0.0.1/README.md` & `pcpfm-0.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,25 @@
+# Disclaimer
+
+Thanks for your interest in the PCPFM! If you talked to me at the Metabolomics2023 conference thanks for giving this project a try. This project is still an alpha. While I'm not aware of any issues that could cause data quality issues, use at your at your own risk!
+
+I just did a major refactor and the Nextflow implementation is out of date along with some of the documentation. I will be working on fixing these things by the end of June. If there is a feature or change you think would make a good addition, feel free to contact me and/or open an issue on the repo. 
+
 # PythonCentricPipelineForMetabolomics (PCPFM)
 
+NOTE - documentation below is out of date and will be updated in the next week or so 06/16
+
+to-implement:
+  - new nextflow wrappers
+  - direct annotation of feature tables
+  - auto drop samples based on QC metrics
+  - auto drop features based on QC metrics
+  - mzML experiment construction
+
+
 ## Overview
 
 The PythonCentricPipelineForMetabolomics (PCPMF) is an all-in-one pipeline for processing LC-MS based metabolomics datasets. Currently supported is limited to datasets collected on Thermo instruments; however, this will be expanded in the future. 
 
 The pipeline includes ingesting and converting .raw files to their .mzML representations with the ThermoRawFileParser, feature extraction and pre-annotation with Asari and Khipu respectively, optional manual and/or automated QA/QC, feature normalization, blank masking and (soon) batch correction. 
 
 The input to the pipeline is a .csv file that minimally has 'Name' and 'Filepath' field storing each Acquisition's name and raw filepath respectively. This csv file is intended to be the sequence file used during acquisition on the LC-MS. An Experiment object, which encaptulates all acquisitions from an experiment (should be the same ionization, chromatography, and mass spectrometry method), is used to move data and intermediates between steps. All information is stored in a user-defined experiment directory
```

### Comparing `pcpfm-0.0.1/pcpfm/Acquisition.py` & `pcpfm-0.0.2/pcpfm/Acquisition.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
             name (str): the name for the acuqisition, from sequence file
             source_filepath (str): a string pointing to the ORIGIN path of the acqusition
             metadata_dict (dict): a dictionary storing metadata from the sequence file for the acquisition
         """        
         self.name = name
         self.metadata_tags = metadata_dict
         self.source_filepath = source_filepath
-        
+
         self.raw_filepath = None
         self.mzml_filepath = None
         self.spectra = {}
 
         self.__min_mz = None
         self.__max_mz = None
         self.__min_rt = None
@@ -131,18 +131,18 @@
             bool: True if the acquistion matches or False if the acquisition fails the filter 
         """        
         passed_filter = True
         for key, rules in filter.items():
             values_to_filter = self.metadata_tags[key].lower()
             if "includes" in rules:
                 for must_include in rules["includes"]:
-                    passed_filter = passed_filter and must_include in values_to_filter
+                    passed_filter = passed_filter and must_include.lower() in values_to_filter
             if "lacks" in rules:
                 for not_include in rules["lacks"]:
-                    passed_filter = passed_filter and not_include not in values_to_filter
+                    passed_filter = passed_filter and not_include.lower() not in values_to_filter
         return passed_filter
             
     def __extract_mzml(self, ms_level=None):
         """
         This reads the mzml file for the acquisition and populates the spectra datamember.
 
         The spectra field contains spectra (collections of peaks), peaks, and the peaks sorted by mz and the sorted
@@ -328,29 +328,7 @@
                 pass
             report_fh = open(os.path.join(output_directory, self.name + "_report.txt"), 'w+')
             report_fh.write("Null matches: " + str(null_match_count) + "\n")
             for standard in search_results["standards"]:
                 report_fh.write(standard["name"] + " - Num Matching Peaks: " + str(standard["matching_peaks"]) + " - Detected: " + str(standard["detected"])  + "\n")
             report_fh.close()
         return search_results
-
-    @staticmethod
-    def construct_acquisition_from_sequence_and_metadata_dict(sequence_dict, metadata_dict):
-        """
-        This constructs the acquisition from a sequence dict and metadata dicts. These come from the 
-        sequence and metadata file respectively. 
-
-        I believe this is no longer used and can be deprecated. 
-
-        Args:
-            sequence_dict (dict): all fields for the acquisition in the sequence file
-            metadata_dict (dict): all fields for the acquisition in the metadata file
-
-        Returns:
-            Acquisition: the Acquisition object for this MS acquistiion
-        """        
-        acquisition_source_filepath = sequence_dict["Filepath"]
-        if validate_path(acquisition_source_filepath, fatal=True):
-            acquisition_source_filepath = retrieve_abs_path(acquisition_source_filepath)
-        acquisition_name = sequence_dict["Name"]
-        return Acqusition(acquisition_name, acquisition_source_filepath, metadata_dict)
-
```

### Comparing `pcpfm-0.0.1/pcpfm/EmpCpds.py` & `pcpfm-0.0.2/pcpfm/EmpCpds.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,69 +28,78 @@
         This method saves the empirical compound dictionary to the annotation_subdirectory. 
         The path is determined by the moniker for the empCpds object, however, an alternative moniker can be provided 
         which effectively saves a new empCpd object. This also updates the empCpds registry in the experiment with the 
         path to the stored json.
 
         Args:
             save_as_moniker (str, optional): an alternative moniker to which to save the table. Defaults to None. 
-        """        
+        """
+        print(save_as_moniker)
         save_as_moniker = self.moniker if save_as_moniker is None else save_as_moniker
         self.experiment.empCpds[save_as_moniker] = os.path.join(self.experiment.annotation_subdirectory, save_as_moniker + "_empCpds.json")
         with open(self.experiment.empCpds[save_as_moniker], 'w+') as out_fh:
             json.dump(self.dict_empCpds, out_fh, indent=4)
 
     @staticmethod
-    def load(experiment, moniker):
+    def load(moniker, experiment):
         """
         This method generates the empCpd object for the provided moniker.
 
         Args:
             experiment (Experiment object): the experiment for which the empCpd was generated
             moniker (string): the empCpd moniker to load
 
         Returns:
             empCpds: the empCpds object for the specified moniker
         """        
         return empCpds(json.load(open(experiment.empCpds[moniker])), experiment, moniker)
 
     @staticmethod
-    def construct_empCpds_from_feature_table(experiment, feature_table_moniker='full', empCpd_moniker='default', add_singletons=True):
+    def construct_empCpds_from_feature_table(experiment, isotopes=isotope_search_patterns, adducts=None, extended_adducts=extended_adducts, feature_table_moniker='full', empCpd_moniker='default', add_singletons=True, rt_search_window=2, mz_tolerance=5, charges=[1,2,3]):
         """_summary_
 
         Args:
             experiment (_type_): _description_
             feature_table_moniker (str, optional): _description_. Defaults to 'full'.
             empCpd_moniker (str, optional): _description_. Defaults to 'default'.
             add_singletons (bool, optional): _description_. Defaults to True.
 
         Returns:
             _type_: _description_
-        """        
+        """
+        if experiment.ionization_mode == 'pos' and adducts is None:
+            adducts = adduct_search_patterns
+        elif experiment.ionization_mode == 'neg' and adducts is None:
+            adducts = adduct_search_patterns_neg
         peaklist = read_table_to_peaks(experiment.feature_tables[feature_table_moniker], has_header=True, mz_col=1, rtime_col=2, feature_id=0)
         for p in peaklist:
             p['id'] = p['id_number']
             p['representative_intensity'] = None
         ECCON = epdsConstructor(peaklist, experiment.ionization_mode)
         dict_empCpds = ECCON.peaks_to_epdDict(
-            [(1.003355, '13C/12C', (0, 0.8)), (1.003355*2, '13C/12C*2', (0, 0.8)), (1.003355*3, '13C/12C*3', (0, 0.8))],
+            isotopes,
             adduct_search_patterns,
             extended_adducts,
-            5,
+            mz_tolerance_ppm=mz_tolerance,
+            rt_tolerance=rt_search_window,
+            charges=charges
         )
         all_feature_ids = set()
         for empCpd in dict_empCpds.values():
             for peak in empCpd["MS1_pseudo_Spectra"]:
                 all_feature_ids.add(peak['id_number'])
         if add_singletons:
             for peak in peaklist:
                 if peak['id_number'] not in all_feature_ids:
                     peak['ion_relation'] = None
                     dict_empCpds[len(dict_empCpds)] = {'interim_id': len(dict_empCpds), 'neutral_formula_mass': '', 'neutral_formula': '', 'MS1_pseudo_Spectra': [peak]}
-        return empCpds(dict_empCpds, experiment, empCpd_moniker)
-    
+        empCpd = empCpds(dict_empCpds, experiment, empCpd_moniker)
+        empCpd.save()
+        return empCpd
+
     def MS1_annotate(self, annotation_sources, rt_tolerance=5):
         """
         Given multiple annotation sources in the JSON format compliant with JMS, annotate based on neutral formula 
         match to the annotation sources.
 
         Args:
             annotation_sources (list[str]): list of filepaths to annotation sources in JSON format
```

### Comparing `pcpfm-0.0.1/pcpfm/Experiment.py` & `pcpfm-0.0.2/pcpfm/Experiment.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import csv
 import shutil
 import json
 import os
 
 from pcpfm.ThermoRawFileConverter import ThermoRawFileConverter
 from pcpfm.Acquisition import Acqusition
+from pcpfm.FeatureTable import FeatureTable
+import pcpfm.EmpCpds as EmpCpds
 
 class Experiment:
     subdirectories = {
         "asari_results": "asari_results/",
         "converted": "converted_acquisitions/",
         "raw": "raw_acquisitions/",
         "annotations": "annotations/",
@@ -47,15 +49,15 @@
             organized_samples (dict, optional): dictionary of acquisitions organized into types of samples #DEPRECATED - REMOVE. Defaults to None.
             log (logging_object, optional): logging instance, #DEPRECATED - REMOVE. Defaults to None.
             feature_tables (dict, optional): mapping of feature table monikers to feature tables on disk. Defaults to None.
             empCpds (dict, optional): mapping of empCpd monikers to empCpds on disk. Defaults to None.
         """        
         # provided parameters
         self.experiment_name = experiment_name
-        self.experiment_directory = experiment_directory
+        self.experiment_directory = os.path.abspath(experiment_directory)
         self.acquisitions = [] if acquisitions is None else acquisitions
         self.QCQA_results = {} if qcqa_results is None else qcqa_results
         self.organized_samples = {} if organized_samples is None else organized_samples
         self.drop_results = drop_results
         self.ionization_mode = ionization_mode
         self.full_feature_table_path = full_feature_table_path
         self.preferred_feature_table_path = preferred_feature_table_path
@@ -140,19 +142,27 @@
         if delete_feature_table:
             os.remove(self.feature_tables[moniker])
             del self.feature_tables[moniker]
         elif delete_empCpds:
             os.remove(self.empCpds[moniker])
             del self.empCpds[moniker]
 
-    def retrieve(self, moniker, feature_table=False, empCpds=False):
+    def retrieve(self, moniker, feature_table=False, empCpds=False, as_object=False):
         if feature_table:
-            return self.feature_tables[moniker]
+            feature_table_path = self.feature_tables[moniker]
+            if as_object:
+                return FeatureTable(feature_table_path, self, moniker)
+            else:
+                return feature_table_path
         elif empCpds:
-            return self.empCpds[moniker]
+            empCpd_path = self.empCpds[moniker]
+            if as_object:
+                return EmpCpds.empCpds.load(moniker, self)
+            else:
+                return empCpd_path
 
     def save(self):
         """
         Serialize the experiment and acquisitions and store it on disk
         """        
         with open(os.path.join(self.experiment_directory, "experiment.json"), "w") as save_filehandle:
             JSON_repr = {
@@ -216,15 +226,16 @@
             return_field (str, optional): if defined, return that field from the acquisition, else the object. Defaults to "name".
 
         Returns:
             list: list of passing acquisitions or fields from passing acquisitions
         """        
         if return_field:
             return [getattr(acquisition, return_field) for acquisition in self.acquisitions if acquisition.filter(filter)]
-        return [acquisition for acquisition in self.acquisitions if acquisition.filter(filter)]
+        else:
+            return [acquisition for acquisition in self.acquisitions if acquisition.filter(filter)]
 
     def construct_experiment_from_CSV(experiment_directory, CSV_filepath, ionization_mode, filter=None, name_field='Name', path_field='Filepath'):
         """
         For a given sequence file, create the experiment object, including the addition of acquisitions
 
         Args:
             experiment_directory (str): path to the directory with experiment data and intermediates
@@ -237,15 +248,19 @@
         Returns:
             experiment: the experiment object
         """        
         filter = {} if filter is None else json.loads(filter)
         experiment = Experiment('', experiment_directory)
         with open(CSV_filepath, encoding='utf-8-sig') as CSV_fh:
             for acquisition_info in csv.DictReader(CSV_fh):
-                print(acquisition_info)
+                #print(acquisition_info)
+                if path_field not in acquisition_info:
+                    path_field = "Path"
+                if name_field not in acquisition_info:
+                    name_field = "File Name"
                 if name_field not in acquisition_info or path_field not in acquisition_info:
                     raise Exception()
                 acquisition = Acqusition(acquisition_info[name_field], acquisition_info[path_field], acquisition_info)
                 if acquisition.filter(filter):
                     experiment.add_acquisition(acquisition)
         experiment.ionization_mode = ionization_mode
         return experiment
@@ -257,8 +272,27 @@
         print("empCpds:")
         for moniker, path in self.empCpds.items():
             print("\t", moniker, " - ", path)
         print("feature tables:")
         for moniker, path in self.feature_tables.items():
             print("\t", moniker, " - ", path)
 
+    def batches(self, field="name", batch_field="Batch", debug=False, skip_batch=False):
+        batches = {}
+        for acquisition in self.acquisitions:
+            if skip_batch:
+                batch_name = "no_batch"
+            elif debug:
+                batch_name = acquisition.metadata_tags['Position'].split(":")[0]
+            else:
+                if batch_field in acquisition.metadata_tags:
+                    batch_name = acquisition.metadata_tags[batch_field]
+                else:
+                    batch_name = "no_batch"
+            if batch_name not in batches:
+                batches[batch_name] = []
+            if field:
+                batches[batch_name].append(getattr(acquisition, field))
+            else:
+                batches[batch_name].append(acquisition)
+        return batches
```

### Comparing `pcpfm-0.0.1/pcpfm/FeatureTable.py` & `pcpfm-0.0.2/pcpfm/FeatureTable.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import csv
 import numpy as np
 import seaborn as sns
 import matplotlib.pyplot as plt
 import scipy.stats
 import os
 import pandas as pd
+from combat.pycombat import pycombat 
 from sklearn.preprocessing import StandardScaler
 from sklearn.decomposition import PCA
 from sklearn.manifold import TSNE
 
 class FeatureTable:
-    def __init__(self, feature_table_filepath, experiment):
+    def __init__(self, feature_table_filepath, experiment, moniker):
         """
         This object wraps a feature table
 
         Args:
             feature_table_filepath (str): path to the feature table on disk
             experiment (Experiment object): the experiment object for this feature table
         """        
@@ -33,14 +34,19 @@
                     try:
                         feature_matrix_row.append(np.float64(feature[column_name]))
                     except:
                         feature_matrix_row.append(feature[column_name])
                 feature_matrix.append(feature_matrix_row)
         self.feature_matrix = np.array(feature_matrix).T
 
+    def save(self, table, new_moniker):
+        output_path = os.path.join(self.experiment.filtered_feature_tables_subdirectory, new_moniker + "_Feature_table.tsv")
+        self.experiment.feature_tables[new_moniker] = output_path
+        table.to_csv(os.path.join(self.experiment.filtered_feature_tables_subdirectory, output_path), sep="\t")
+
     def selected_feature_matrix(self, tag=None, sort=False):
         """
         Select columns in the feature table based on metadata, optionally sorted.
 
         Args:
             tag (str, optional): Sample type must match this field. Defaults to None.
             sort (bool, optional): if true, sort the sample names. Defaults to False.
@@ -452,16 +458,193 @@
             plt.show()
         result = {
             "Type": "MissingFeatureZScores",
             "Config": {"intensity_cutoff": intensity_cutoff},
             "Result": {name: float(z_score) for name, z_score in zip(acquisition_names, missing_feature_z_scores)}
         }
         return result
-    
-    def curate(self, blank_names, sample_names, drop_percentile, blank_intensity_ratio, TIC_normalization_percentile, output_path, interactive_plot=False):
+
+    def drop_samples(self, new_moniker, drop_others=True, keep_types=[], drop_types=[], type_field="Sample Type", drop_name=None):
+        retain, drop = [], []
+        if not drop_name:
+            for keep_type in keep_types:
+                retain += list(self.experiment.filter_samples({type_field: {"includes": [keep_type]}}))
+            for drop_type in drop_types:
+                drop += list(self.experiment.filter_samples({type_field: {"includes": [drop_type]}}))
+        elif drop_name:
+            drop = [a.name for a in self.experiment.acquisitions if a.name == drop_name]
+        else:
+            pass
+        for name in {a.name for a in self.experiment.acquisitions}:
+            if name not in drop and name not in retain:
+                if drop_others:
+                    drop.append(name)
+                else:
+                    retain.append(name)
+        selected_columns = [header_field for header_field in self.feature_matrix_header if header_field not in drop]
+        table = pd.DataFrame(np.array([self.select_feature_column(x) for x in selected_columns]).T, columns=selected_columns)
+        self.save(table, new_moniker)
+
+    def blank_mask(self, new_moniker, by_batch=True, blank_intensity_ratio=3, logic_mode="and", blank_type="Blank", sample_type="Unknown", type_field="Sample Type"):
+        def __any_logical(row, columns):
+            return np.any(row[columns] == True)
+
+        def __all_logical(row, columns):
+            return np.all(row[columns] == True)
+        
+        def __non_zero_mean(row, columns):
+            non_zero_columns = [x for x in row[columns] if x > 0]
+            if non_zero_columns:
+                return np.mean(non_zero_columns)
+            else:
+                0
+        
+        blank_names = [x for x in self.experiment.filter_samples({type_field: {"includes": [blank_type]}}) if x in self.feature_matrix_header]
+        sample_names = [x for x in self.experiment.filter_samples({type_field: {"includes": [sample_type]}}) if x in self.feature_matrix_header]
+        table = pd.DataFrame(np.array([self.select_feature_column(x) for x in sample_names + blank_names]).T, columns=sample_names + blank_names)
+        blank_mask_columns = []
+        for batch_name, batch_name_list in self.experiment.batches(skip_batch=by_batch).items():
+            batch_blanks = [x for x in batch_name_list if x in blank_names]
+            batch_samples = [x for x in batch_name_list if x in sample_names]
+            blank_means = table.apply(__non_zero_mean, axis=1, args=(batch_blanks,))
+            sample_means = table.apply(__non_zero_mean, axis=1, args=(batch_samples,))
+            to_filter = [blank_mean * blank_intensity_ratio > sample_mean for blank_mean, sample_mean in zip(blank_means, sample_means)]
+            mask_column_name = "masked" + batch_name
+            blank_mask_columns.append(mask_column_name)
+            table[mask_column_name] = to_filter
+        print(np.sum(to_filter))
+
+        if logic_mode == "and":
+            table["mask_feature"] = table.apply(__all_logical, axis=1, args=(blank_mask_columns,))
+        elif logic_mode == "or":
+            table["mask_feature"] = table.apply(__any_logical, axis=1, args=(blank_mask_columns,))
+
+        for blank_mask_column in blank_mask_columns:
+            table.drop(columns=blank_mask_column, inplace=True)
+
+        for header_field in self.feature_matrix_header:
+            if header_field not in blank_names + sample_names:
+                table[header_field] = self.select_feature_column(header_field)
+        table = table[table["mask_feature"] == False]
+        table.drop(columns="mask_feature", inplace=True)
+        self.save(table, new_moniker)
+
+    def interpolate_missing_features(self, new_moniker, ratio=0.5, by_batch=True):
+        def calc_interpolated_value(row, sample_names):
+            values = [x for x in row[sample_names] if x > 0]
+            if values:
+                return min(values) * ratio
+            else:
+                return 0
+        sample_names = [a.name for a in self.experiment.acquisitions if a.name in self.feature_matrix_header]
+        table = pd.DataFrame(np.array([self.select_feature_column(x) for x in sample_names]).T, columns=sample_names)
+        for _, batch_name_list in self.experiment.batches(skip_batch=not by_batch).items():
+            filtered_batch_name_list = [x for x in batch_name_list if x in sample_names]
+            table["feature_interpolate_value"] = table.apply(calc_interpolated_value, axis=1, args=(filtered_batch_name_list,))
+            for sample_name in filtered_batch_name_list:
+                table[sample_name] = table[[sample_name, "feature_interpolate_value"]].max(axis=1)
+            table.drop(columns="feature_interpolate_value", inplace=True)
+        for header_field in self.feature_matrix_header:
+            if header_field not in sample_names and header_field:
+                table[header_field] = self.select_feature_column(header_field)
+        self.save(table, new_moniker)
+
+    def TIC_normalize(self, new_moniker, TIC_normalization_percentile=0.90, by_batch=True, sample_type="Unknown", type_field="Sample Type", normalize_mode='median', interactive=False):
+        sample_names = self.experiment.filter_samples({type_field: {"includes": [sample_type]}})
+        table = pd.DataFrame(np.array([self.select_feature_column(x) for x in sample_names]).T, columns=sample_names)
+        for _, batch_name_list in self.experiment.batches(skip_batch=not by_batch).items():
+            filtered_batch_name_list = [x for x in batch_name_list if x in sample_names]
+            table["percent_inclusion"] = np.sum(table[filtered_batch_name_list] > 0, axis=1) / len(filtered_batch_name_list)
+            TICs = {sample: np.sum(table[table["percent_inclusion"] > TIC_normalization_percentile][sample]) for sample in filtered_batch_name_list}
+            if interactive:
+                uncorr_TICs = {sample: np.sum(table[sample]) for sample in filtered_batch_name_list}
+                plt.bar(list(uncorr_TICs.keys()), list(uncorr_TICs.values()))
+                plt.show()
+                plt.bar(list(TICs.keys()), list(TICs.values()))
+                plt.show()
+
+            function_map = {
+                "median": np.median,
+                "mean": np.mean,
+            }
+
+            norm_factors = {sample: function_map[normalize_mode](list(TICs.values()))/value for sample, value in TICs.items()}
+            for sample, norm_factor in norm_factors.items():
+                table[sample] = table[sample] * norm_factor
+            if interactive:
+                corr_TICs = {sample: np.sum(table[sample]) for sample in filtered_batch_name_list}
+                plt.bar(list(norm_factors.keys()), list(norm_factors.values()))
+                plt.show()
+                plt.bar(list(corr_TICs.keys()), list(corr_TICs.values()))
+                plt.show()
+                corr_selected_TICs = {sample: np.sum(table[table["percent_inclusion"] > TIC_normalization_percentile][sample]) for sample in filtered_batch_name_list}
+                plt.bar(list(corr_selected_TICs.keys()), list(corr_selected_TICs.values()))
+                plt.show()
+
+        for header_field in self.feature_matrix_header:
+            if header_field not in sample_names and header_field:
+                table[header_field] = self.select_feature_column(header_field)
+        self.save(table, new_moniker)
+
+    def batch_correct(self, new_moniker):
+        batch_idx_map = {}
+        for batch_idx, (_, acquisition_name_list) in enumerate(self.experiment.batches.items()):
+            for acquisition_name in acquisition_name_list:
+                batch_idx_map[acquisition_name] = batch_idx
+        sample_names = [a.name for a in self.experiment.acquisitions if a.name in self.feature_matrix_header]
+        batches = [batch_idx_map[a.name] for a in self.experiment.acquisitions if a.name in self.feature_matrix_header]
+        table = pd.DataFrame(np.array([self.select_feature_column(x) for x in sample_names]).T, columns=sample_names)
+        batch_corrected = pycombat(table, batches)
+        for header_field in self.feature_matrix_header:
+            if header_field not in batch_corrected.columns:
+                batch_corrected[header_field] = self.select_feature_column(header_field)
+        self.save(batch_corrected, new_moniker)
+
+    def log_transform(self, new_moniker, log_mode="log10"):
+        log_types = {
+            "log10": np.log10,
+            "log2": np.log2
+        }
+
+        sample_names = [x.name for x in self.experiment.acquisitions if x.name in self.feature_matrix_header]
+        table = pd.DataFrame(np.array([self.select_feature_column(x) for x in sample_names]).T, columns=sample_names)
+        table = log_types[log_mode](table + 1)
+        for header_field in self.feature_matrix_header:
+            if header_field not in table.columns and header_field:
+                table[header_field] = self.select_feature_column(header_field) 
+        self.save(table, new_moniker)
+
+    def drop_missing_features(self, new_moniker, by_batch=True, drop_percentile=0.8, logic_mode="and", sample_type="Unknown", type_field="Sample Type"):
+        def __any(row, columns, drop_percentile):
+            return not np.any(row[columns] >= drop_percentile)
+
+        def __all(row, columns, drop_percentile):
+            return not np.all(row[columns] >= drop_percentile)
+
+        sample_names = self.experiment.filter_samples({type_field: {"includes": [sample_type]}})
+        table = pd.DataFrame(np.array([self.select_feature_column(x) for x in sample_names]).T, columns=sample_names)
+        batch_columns = []
+        for batch_name, batch_name_list in self.experiment.batches(skip_batch=not by_batch).items():
+            batch_column = "percent_inclusion" + batch_name
+            filtered_batch_name_list = [x for x in batch_name_list if x in sample_names]
+            table[batch_column] = np.sum(table[filtered_batch_name_list] > 0, axis=1) / len(filtered_batch_name_list)
+            batch_columns.append(batch_column)
+
+        if logic_mode == "and":
+            table["drop_feature"] = table.apply(__all, axis=1, args=(batch_columns, drop_percentile))
+        elif logic_mode == "or":
+            table["drop_feature"] = table.apply(__any, axis=1, args=(batch_columns, drop_percentile))
+        
+        for header_field in self.feature_matrix_header:
+            if header_field not in table.columns:
+                table[header_field] = self.select_feature_column(header_field)
+        table = table[table["drop_feature"] == False].copy()
+        self.save(table, new_moniker)
+
+    def curate(self, blank_names, sample_names, drop_percentile, blank_intensity_ratio, TIC_normalization_percentile, output_path, interactive_plot=True):
         """
         Performa blank masking, drop missing features, normalize by TIC, and output the curated table to the specififed path.
 
         # TODO - needs an option for batch correction.
         # TODO - needs an option for interpolation
         # TODO - add support to normalize on top N features
 
@@ -579,13 +762,13 @@
         if missing_feature_distribution:
             qcqa_result.append(self.missing_feature_distribution(selected_feature_matrix, selected_acquisition_names, interactive_plot=interactive))
         if missing_feature_outlier_detection:
             qcqa_result.append(self.missing_feature_outlier_detection(selected_feature_matrix, selected_acquisition_names, interactive_plot=interactive))
         if median_correlation_outlier_detection:
             qcqa_result.append(self.median_correlation_outlier_detection(selected_feature_matrix, selected_acquisition_names, interactive_plot=interactive))
         if intensity_analysis:
-            qcqa_result.append(self.intensity_analysis(selected_feature_matrix, selected_acquisition_names, drop_missing=True, interactive_plot=interactive))
+            qcqa_result.append(self.intensity_analysis(selected_feature_matrix, selected_acquisition_names, interactive_plot=interactive))
         if feature_distribution:
             qcqa_result.append(self.feature_distribution(selected_feature_matrix, selected_acquisition_names, interactive_plot=interactive))
         if feature_outlier_detection:
             qcqa_result.append(self.feature_distribution_outlier_detection(selected_feature_matrix, selected_acquisition_names, interactive_plot=interactive))
         return qcqa_result
```

### Comparing `pcpfm-0.0.1/pcpfm/ThermoRawFileConverter.py` & `pcpfm-0.0.2/pcpfm/ThermoRawFileConverter.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
         Args:
             raw_acquisition (Acquisition): Acquisition object to convert
             output_directory (str): output directory
         """        
         try:
             output_filepath = os.path.join(output_directory, os.path.basename(raw_acquisition.raw_filepath)).replace(".raw", ".mzML")
-            subprocess.run([self.mono_path, self.exe_path, '-f=1', '-i', raw_acquisition.raw_filepath, '-b', output_filepath])
+            subprocess.run([self.mono_path, self.exe_path, '-f=1', '-i', raw_acquisition.raw_filepath, '-b', output_filepath, ' >/dev/null'])
         except:
             pass
 
     def convert_multi(self, raw_acquisitions, output_directory):
         """
         Convert multiple acquisitions and put the resulting .mzML into the output directory in parallel
```

### Comparing `pcpfm-0.0.1/pcpfm.egg-info/PKG-INFO` & `pcpfm-0.0.2/pcpfm.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcpfm
-Version: 0.0.1
+Version: 0.0.2
 Summary: LC-MS metabolomics data processing pipeline
 Home-page: https://github.com/jmmitc06/PythonCentricPipelineForMetabolomics
 Author: Joshua Mitchell
 Author-email: joshua.mitchell@jax.org
 License: MIT
 Keywords: metabolomics bioinformatics mass spectrometry
 Classifier: Intended Audience :: Developers
@@ -16,16 +16,32 @@
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+# Disclaimer
+
+Thanks for your interest in the PCPFM! If you talked to me at the Metabolomics2023 conference thanks for giving this project a try. This project is still an alpha. While I'm not aware of any issues that could cause data quality issues, use at your at your own risk!
+
+I just did a major refactor and the Nextflow implementation is out of date along with some of the documentation. I will be working on fixing these things by the end of June. If there is a feature or change you think would make a good addition, feel free to contact me and/or open an issue on the repo. 
+
 # PythonCentricPipelineForMetabolomics (PCPFM)
 
+NOTE - documentation below is out of date and will be updated in the next week or so 06/16
+
+to-implement:
+  - new nextflow wrappers
+  - direct annotation of feature tables
+  - auto drop samples based on QC metrics
+  - auto drop features based on QC metrics
+  - mzML experiment construction
+
+
 ## Overview
 
 The PythonCentricPipelineForMetabolomics (PCPMF) is an all-in-one pipeline for processing LC-MS based metabolomics datasets. Currently supported is limited to datasets collected on Thermo instruments; however, this will be expanded in the future. 
 
 The pipeline includes ingesting and converting .raw files to their .mzML representations with the ThermoRawFileParser, feature extraction and pre-annotation with Asari and Khipu respectively, optional manual and/or automated QA/QC, feature normalization, blank masking and (soon) batch correction. 
 
 The input to the pipeline is a .csv file that minimally has 'Name' and 'Filepath' field storing each Acquisition's name and raw filepath respectively. This csv file is intended to be the sequence file used during acquisition on the LC-MS. An Experiment object, which encaptulates all acquisitions from an experiment (should be the same ionization, chromatography, and mass spectrometry method), is used to move data and intermediates between steps. All information is stored in a user-defined experiment directory
```

### Comparing `pcpfm-0.0.1/setup.py` & `pcpfm-0.0.2/setup.py`

 * *Files identical despite different names*

