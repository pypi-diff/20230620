# Comparing `tmp/useful_rdkit_utils-0.2.6.tar.gz` & `tmp/useful_rdkit_utils-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "useful_rdkit_utils-0.2.6.tar", last modified: Sat Jun 10 19:37:12 2023, max compression
+gzip compressed data, was "useful_rdkit_utils-0.2.7.tar", last modified: Tue Jun 20 00:40:16 2023, max compression
```

## Comparing `useful_rdkit_utils-0.2.6.tar` & `useful_rdkit_utils-0.2.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 pwalters   (501) staff       (20)        0 2023-06-10 19:37:12.773552 useful_rdkit_utils-0.2.6/
--rw-r--r--   0 pwalters   (501) staff       (20)     3555 2022-11-25 17:16:15.000000 useful_rdkit_utils-0.2.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 pwalters   (501) staff       (20)     1068 2022-11-25 17:16:15.000000 useful_rdkit_utils-0.2.6/LICENSE
--rw-r--r--   0 pwalters   (501) staff       (20)      152 2022-11-25 17:16:15.000000 useful_rdkit_utils-0.2.6/MANIFEST.in
--rw-r--r--   0 pwalters   (501) staff       (20)     1459 2023-06-10 19:37:12.773614 useful_rdkit_utils-0.2.6/PKG-INFO
--rw-r--r--   0 pwalters   (501) staff       (20)     1140 2022-11-25 17:16:15.000000 useful_rdkit_utils-0.2.6/README.md
--rw-r--r--   0 pwalters   (501) staff       (20)      385 2023-06-10 19:37:12.773977 useful_rdkit_utils-0.2.6/setup.cfg
--rw-r--r--   0 pwalters   (501) staff       (20)     2245 2022-12-03 03:52:40.000000 useful_rdkit_utils-0.2.6/setup.py
-drwxr-xr-x   0 pwalters   (501) staff       (20)        0 2023-06-10 19:37:12.774377 useful_rdkit_utils-0.2.6/useful_rdkit_utils/
--rw-r--r--   0 pwalters   (501) staff       (20)      386 2022-11-27 21:51:25.000000 useful_rdkit_utils-0.2.6/useful_rdkit_utils/__init__.py
--rw-r--r--   0 pwalters   (501) staff       (20)      498 2023-06-10 19:37:12.774422 useful_rdkit_utils-0.2.6/useful_rdkit_utils/_version.py
--rw-r--r--   0 pwalters   (501) staff       (20)     1297 2022-11-25 17:16:15.000000 useful_rdkit_utils-0.2.6/useful_rdkit_utils/pandas_utils.py
--rw-r--r--   0 pwalters   (501) staff       (20)     4124 2022-11-25 17:16:15.000000 useful_rdkit_utils-0.2.6/useful_rdkit_utils/reos.py
--rw-r--r--   0 pwalters   (501) staff       (20)      834 2022-11-29 22:30:32.000000 useful_rdkit_utils-0.2.6/useful_rdkit_utils/ring_counts.csv
--rw-r--r--   0 pwalters   (501) staff       (20)      645 2022-11-28 00:30:51.000000 useful_rdkit_utils-0.2.6/useful_rdkit_utils/ring_freq_test.csv
--rw-r--r--   0 pwalters   (501) staff       (20)      524 2022-11-28 02:57:29.000000 useful_rdkit_utils-0.2.6/useful_rdkit_utils/ring_systems.csv
--rwxr-xr-x   0 pwalters   (501) staff       (20)     8963 2022-12-03 18:19:39.000000 useful_rdkit_utils-0.2.6/useful_rdkit_utils/ring_systems.py
--rw-r--r--   0 pwalters   (501) staff       (20)      524 2022-11-29 12:48:31.000000 useful_rdkit_utils-0.2.6/useful_rdkit_utils/ring_test.csv
--rw-r--r--   0 pwalters   (501) staff       (20)      310 2022-11-28 02:02:49.000000 useful_rdkit_utils-0.2.6/useful_rdkit_utils/seaborn_utils.py
-drwxr-xr-x   0 pwalters   (501) staff       (20)        0 2023-06-10 19:37:12.773383 useful_rdkit_utils-0.2.6/useful_rdkit_utils/tests/
--rw-r--r--   0 pwalters   (501) staff       (20)      113 2022-11-25 17:16:15.000000 useful_rdkit_utils-0.2.6/useful_rdkit_utils/tests/__init__.py
--rw-r--r--   0 pwalters   (501) staff       (20)      566 2022-11-25 17:16:15.000000 useful_rdkit_utils-0.2.6/useful_rdkit_utils/tests/test_reos.py
--rw-r--r--   0 pwalters   (501) staff       (20)     1620 2022-11-28 00:30:45.000000 useful_rdkit_utils-0.2.6/useful_rdkit_utils/tests/test_ring_systems.py
--rw-r--r--   0 pwalters   (501) staff       (20)     5151 2022-11-25 17:16:15.000000 useful_rdkit_utils-0.2.6/useful_rdkit_utils/tests/test_useful_rdkit_utils.py
--rw-r--r--   0 pwalters   (501) staff       (20)    12336 2022-12-20 01:59:21.000000 useful_rdkit_utils-0.2.6/useful_rdkit_utils/useful_rdkit_utils.py
-drwxr-xr-x   0 pwalters   (501) staff       (20)        0 2023-06-10 19:37:12.772626 useful_rdkit_utils-0.2.6/useful_rdkit_utils.egg-info/
--rw-r--r--   0 pwalters   (501) staff       (20)     1459 2023-06-10 19:37:12.000000 useful_rdkit_utils-0.2.6/useful_rdkit_utils.egg-info/PKG-INFO
--rw-r--r--   0 pwalters   (501) staff       (20)      841 2023-06-10 19:37:12.000000 useful_rdkit_utils-0.2.6/useful_rdkit_utils.egg-info/SOURCES.txt
--rw-r--r--   0 pwalters   (501) staff       (20)        1 2023-06-10 19:37:12.000000 useful_rdkit_utils-0.2.6/useful_rdkit_utils.egg-info/dependency_links.txt
--rw-r--r--   0 pwalters   (501) staff       (20)       70 2023-06-10 19:37:12.000000 useful_rdkit_utils-0.2.6/useful_rdkit_utils.egg-info/requires.txt
--rw-r--r--   0 pwalters   (501) staff       (20)       19 2023-06-10 19:37:12.000000 useful_rdkit_utils-0.2.6/useful_rdkit_utils.egg-info/top_level.txt
--rw-r--r--   0 pwalters   (501) staff       (20)    68611 2022-11-25 17:16:15.000000 useful_rdkit_utils-0.2.6/versioneer.py
+drwxr-xr-x   0 pwalters   (501) staff       (20)        0 2023-06-20 00:40:16.855433 useful_rdkit_utils-0.2.7/
+-rw-r--r--   0 pwalters   (501) staff       (20)     3555 2022-11-25 17:16:15.000000 useful_rdkit_utils-0.2.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 pwalters   (501) staff       (20)     1068 2022-11-25 17:16:15.000000 useful_rdkit_utils-0.2.7/LICENSE
+-rw-r--r--   0 pwalters   (501) staff       (20)      152 2022-11-25 17:16:15.000000 useful_rdkit_utils-0.2.7/MANIFEST.in
+-rw-r--r--   0 pwalters   (501) staff       (20)     1459 2023-06-20 00:40:16.855512 useful_rdkit_utils-0.2.7/PKG-INFO
+-rw-r--r--   0 pwalters   (501) staff       (20)     1140 2022-11-25 17:16:15.000000 useful_rdkit_utils-0.2.7/README.md
+-rw-r--r--   0 pwalters   (501) staff       (20)      385 2023-06-20 00:40:16.855803 useful_rdkit_utils-0.2.7/setup.cfg
+-rw-r--r--   0 pwalters   (501) staff       (20)     2245 2022-12-03 03:52:40.000000 useful_rdkit_utils-0.2.7/setup.py
+drwxr-xr-x   0 pwalters   (501) staff       (20)        0 2023-06-20 00:40:16.856284 useful_rdkit_utils-0.2.7/useful_rdkit_utils/
+-rw-r--r--   0 pwalters   (501) staff       (20)      386 2022-11-27 21:51:25.000000 useful_rdkit_utils-0.2.7/useful_rdkit_utils/__init__.py
+-rw-r--r--   0 pwalters   (501) staff       (20)      497 2023-06-20 00:40:16.856576 useful_rdkit_utils-0.2.7/useful_rdkit_utils/_version.py
+-rw-r--r--   0 pwalters   (501) staff       (20)     1297 2022-11-25 17:16:15.000000 useful_rdkit_utils-0.2.7/useful_rdkit_utils/pandas_utils.py
+-rw-r--r--   0 pwalters   (501) staff       (20)     4662 2023-06-19 23:54:53.000000 useful_rdkit_utils-0.2.7/useful_rdkit_utils/reos.py
+-rw-r--r--   0 pwalters   (501) staff       (20)      834 2022-11-29 22:30:32.000000 useful_rdkit_utils-0.2.7/useful_rdkit_utils/ring_counts.csv
+-rw-r--r--   0 pwalters   (501) staff       (20)      645 2022-11-28 00:30:51.000000 useful_rdkit_utils-0.2.7/useful_rdkit_utils/ring_freq_test.csv
+-rw-r--r--   0 pwalters   (501) staff       (20)      524 2022-11-28 02:57:29.000000 useful_rdkit_utils-0.2.7/useful_rdkit_utils/ring_systems.csv
+-rwxr-xr-x   0 pwalters   (501) staff       (20)     8963 2022-12-03 18:19:39.000000 useful_rdkit_utils-0.2.7/useful_rdkit_utils/ring_systems.py
+-rw-r--r--   0 pwalters   (501) staff       (20)      524 2022-11-29 12:48:31.000000 useful_rdkit_utils-0.2.7/useful_rdkit_utils/ring_test.csv
+-rw-r--r--   0 pwalters   (501) staff       (20)      310 2022-11-28 02:02:49.000000 useful_rdkit_utils-0.2.7/useful_rdkit_utils/seaborn_utils.py
+drwxr-xr-x   0 pwalters   (501) staff       (20)        0 2023-06-20 00:40:16.855151 useful_rdkit_utils-0.2.7/useful_rdkit_utils/tests/
+-rw-r--r--   0 pwalters   (501) staff       (20)      113 2022-11-25 17:16:15.000000 useful_rdkit_utils-0.2.7/useful_rdkit_utils/tests/__init__.py
+-rw-r--r--   0 pwalters   (501) staff       (20)      566 2022-11-25 17:16:15.000000 useful_rdkit_utils-0.2.7/useful_rdkit_utils/tests/test_reos.py
+-rw-r--r--   0 pwalters   (501) staff       (20)     1620 2022-11-28 00:30:45.000000 useful_rdkit_utils-0.2.7/useful_rdkit_utils/tests/test_ring_systems.py
+-rw-r--r--   0 pwalters   (501) staff       (20)     5151 2022-11-25 17:16:15.000000 useful_rdkit_utils-0.2.7/useful_rdkit_utils/tests/test_useful_rdkit_utils.py
+-rw-r--r--   0 pwalters   (501) staff       (20)    12336 2022-12-20 01:59:21.000000 useful_rdkit_utils-0.2.7/useful_rdkit_utils/useful_rdkit_utils.py
+drwxr-xr-x   0 pwalters   (501) staff       (20)        0 2023-06-20 00:40:16.854082 useful_rdkit_utils-0.2.7/useful_rdkit_utils.egg-info/
+-rw-r--r--   0 pwalters   (501) staff       (20)     1459 2023-06-20 00:40:16.000000 useful_rdkit_utils-0.2.7/useful_rdkit_utils.egg-info/PKG-INFO
+-rw-r--r--   0 pwalters   (501) staff       (20)      841 2023-06-20 00:40:16.000000 useful_rdkit_utils-0.2.7/useful_rdkit_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 pwalters   (501) staff       (20)        1 2023-06-20 00:40:16.000000 useful_rdkit_utils-0.2.7/useful_rdkit_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 pwalters   (501) staff       (20)       70 2023-06-20 00:40:16.000000 useful_rdkit_utils-0.2.7/useful_rdkit_utils.egg-info/requires.txt
+-rw-r--r--   0 pwalters   (501) staff       (20)       19 2023-06-20 00:40:16.000000 useful_rdkit_utils-0.2.7/useful_rdkit_utils.egg-info/top_level.txt
+-rw-r--r--   0 pwalters   (501) staff       (20)    68611 2022-11-25 17:16:15.000000 useful_rdkit_utils-0.2.7/versioneer.py
```

### Comparing `useful_rdkit_utils-0.2.6/CODE_OF_CONDUCT.md` & `useful_rdkit_utils-0.2.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.2.6/LICENSE` & `useful_rdkit_utils-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.2.6/PKG-INFO` & `useful_rdkit_utils-0.2.7/useful_rdkit_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: useful_rdkit_utils
-Version: 0.2.6
+Name: useful-rdkit-utils
+Version: 0.2.7
 Summary: Some useful RDKit functions
 Author: PatWalters
 Author-email: wpwalters@gmail.com
 License: MIT
 Platform: Linux
 Platform: Mac OS-X
 Platform: Unix
```

### Comparing `useful_rdkit_utils-0.2.6/README.md` & `useful_rdkit_utils-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.2.6/setup.py` & `useful_rdkit_utils-0.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.2.6/useful_rdkit_utils/pandas_utils.py` & `useful_rdkit_utils-0.2.7/useful_rdkit_utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.2.6/useful_rdkit_utils/reos.py` & `useful_rdkit_utils-0.2.7/useful_rdkit_utils/reos.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,21 +10,29 @@
     """REOS - Rapid Elimination Of Swill\n
     Walters, Ajay, Murcko, "Recognizing molecules with druglike properties"\n
     Curr. Opin. Chem. Bio., 3 (1999), 384-387\n
     https://doi.org/10.1016/S1367-5931(99)80058-1
     """
 
     def __init__(self, active_rules=None):
+        self.output_smarts = False
         if active_rules is None:
             active_rules = ['Glaxo']
         url = 'https://raw.githubusercontent.com/PatWalters/rd_filters/master/rd_filters/data/alert_collection.csv'
         self.rule_path = pystow.ensure('useful_rdkit_utils', 'data', url=url)
         self.rule_df = pd.read_csv(self.rule_path)
         self.read_rules(self.rule_path, active_rules)
 
+    def set_output_smarts(self, output_smarts):
+        """Determine whether SMARTS are returned
+        :param output_smarts: True or False
+        :return: None
+        """
+        self.output_smarts = output_smarts
+
     def parse_smarts(self):
         """Parse the SMARTS strings in the rules file to molecule objects and check for validity
 
         :return: True if all SMARTS are parsed, False otherwise
         """
         smarts_mol_list = []
         smarts_are_ok = True
@@ -91,19 +99,27 @@
 
     def process_mol(self, mol):
         """Match a molecule against the active rule set
 
         :param mol: input RDKit molecule
         :return: the first rule matched or "ok" if no rules are matched
         """
-        cols = ['description', 'rule_set_name', 'pat', 'max']
-        for desc, rule_set_name, pat, max_val in self.active_rule_df[cols].values:
+        cols = ['description', 'rule_set_name', 'smarts', 'pat', 'max']
+        if self.output_smarts:
+            ret_val = ("ok", "ok", "ok")
+        else:
+            ret_val = ("ok", "ok")
+        for desc, rule_set_name, smarts, pat, max_val in self.active_rule_df[cols].values:
             if len(mol.GetSubstructMatches(pat)) > max_val:
-                return rule_set_name, desc
-        return "ok", "ok"
+                if self.output_smarts:
+                    ret_val = rule_set_name, desc, smarts
+                else:
+                    ret_val = rule_set_name, desc
+                break
+        return ret_val
 
     def process_smiles(self, smiles):
         """Convert SMILES to an RDKit molecule and call process_mol
 
         :param smiles: input SMILES
         :return: process_mol result or None if the SMILES can't be parsed
         """
```

### Comparing `useful_rdkit_utils-0.2.6/useful_rdkit_utils/ring_counts.csv` & `useful_rdkit_utils-0.2.7/useful_rdkit_utils/ring_counts.csv`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.2.6/useful_rdkit_utils/ring_freq_test.csv` & `useful_rdkit_utils-0.2.7/useful_rdkit_utils/ring_freq_test.csv`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.2.6/useful_rdkit_utils/ring_systems.csv` & `useful_rdkit_utils-0.2.7/useful_rdkit_utils/ring_systems.csv`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.2.6/useful_rdkit_utils/ring_systems.py` & `useful_rdkit_utils-0.2.7/useful_rdkit_utils/ring_systems.py`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.2.6/useful_rdkit_utils/ring_test.csv` & `useful_rdkit_utils-0.2.7/useful_rdkit_utils/ring_test.csv`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.2.6/useful_rdkit_utils/tests/test_reos.py` & `useful_rdkit_utils-0.2.7/useful_rdkit_utils/tests/test_reos.py`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.2.6/useful_rdkit_utils/tests/test_ring_systems.py` & `useful_rdkit_utils-0.2.7/useful_rdkit_utils/tests/test_ring_systems.py`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.2.6/useful_rdkit_utils/tests/test_useful_rdkit_utils.py` & `useful_rdkit_utils-0.2.7/useful_rdkit_utils/tests/test_useful_rdkit_utils.py`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.2.6/useful_rdkit_utils/useful_rdkit_utils.py` & `useful_rdkit_utils-0.2.7/useful_rdkit_utils/useful_rdkit_utils.py`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.2.6/useful_rdkit_utils.egg-info/PKG-INFO` & `useful_rdkit_utils-0.2.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: useful-rdkit-utils
-Version: 0.2.6
+Name: useful_rdkit_utils
+Version: 0.2.7
 Summary: Some useful RDKit functions
 Author: PatWalters
 Author-email: wpwalters@gmail.com
 License: MIT
 Platform: Linux
 Platform: Mac OS-X
 Platform: Unix
```

### Comparing `useful_rdkit_utils-0.2.6/useful_rdkit_utils.egg-info/SOURCES.txt` & `useful_rdkit_utils-0.2.7/useful_rdkit_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.2.6/versioneer.py` & `useful_rdkit_utils-0.2.7/versioneer.py`

 * *Files identical despite different names*

