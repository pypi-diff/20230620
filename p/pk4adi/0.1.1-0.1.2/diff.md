# Comparing `tmp/pk4adi-0.1.1.tar.gz` & `tmp/pk4adi-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pk4adi-0.1.1.tar", last modified: Sat Jun 17 08:25:35 2023, max compression
+gzip compressed data, was "pk4adi-0.1.2.tar", last modified: Mon Jun 19 08:37:57 2023, max compression
```

## Comparing `pk4adi-0.1.1.tar` & `pk4adi-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 08:25:35.152740 pk4adi-0.1.1/
--rw-rw-rw-   0        0        0     1088 2023-01-04 20:12:34.000000 pk4adi-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     8227 2023-06-17 08:25:35.152244 pk4adi-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     7545 2023-06-17 08:02:23.000000 pk4adi-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-17 08:25:35.122940 pk4adi-0.1.1/pk4adi/
--rw-rw-rw-   0        0        0      282 2023-06-17 08:01:07.000000 pk4adi-0.1.1/pk4adi/__init__.py
--rw-rw-rw-   0        0        0     9589 2023-06-17 08:00:07.000000 pk4adi-0.1.1/pk4adi/pk.py
--rw-rw-rw-   0        0        0     7821 2023-06-17 08:00:17.000000 pk4adi-0.1.1/pk4adi/pkc.py
--rw-rw-rw-   0        0        0      968 2023-06-17 08:00:25.000000 pk4adi-0.1.1/pk4adi/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-17 08:25:35.150753 pk4adi-0.1.1/pk4adi.egg-info/
--rw-rw-rw-   0        0        0     8227 2023-06-17 08:25:35.000000 pk4adi-0.1.1/pk4adi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-06-17 08:25:35.000000 pk4adi-0.1.1/pk4adi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 08:25:35.000000 pk4adi-0.1.1/pk4adi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-06-17 08:25:35.000000 pk4adi-0.1.1/pk4adi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-17 08:25:35.000000 pk4adi-0.1.1/pk4adi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-17 08:25:35.152740 pk4adi-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1841 2023-06-17 08:00:35.000000 pk4adi-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:37:57.738282 pk4adi-0.1.2/
+-rw-rw-rw-   0        0        0     1088 2023-01-04 20:12:34.000000 pk4adi-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     8330 2023-06-19 08:37:57.737107 pk4adi-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7644 2023-06-19 08:27:21.000000 pk4adi-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 08:37:57.698869 pk4adi-0.1.2/pk4adi/
+-rw-rw-rw-   0        0        0      282 2023-06-19 08:31:30.000000 pk4adi-0.1.2/pk4adi/__init__.py
+-rw-rw-rw-   0        0        0     9739 2023-06-19 08:08:20.000000 pk4adi-0.1.2/pk4adi/pk.py
+-rw-rw-rw-   0        0        0     7985 2023-06-19 08:15:09.000000 pk4adi-0.1.2/pk4adi/pkc.py
+-rw-rw-rw-   0        0        0      968 2023-06-17 09:21:37.000000 pk4adi-0.1.2/pk4adi/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:37:57.733629 pk4adi-0.1.2/pk4adi.egg-info/
+-rw-rw-rw-   0        0        0     8330 2023-06-19 08:37:57.000000 pk4adi-0.1.2/pk4adi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-06-19 08:37:57.000000 pk4adi-0.1.2/pk4adi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 08:37:57.000000 pk4adi-0.1.2/pk4adi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-06-19 08:37:57.000000 pk4adi-0.1.2/pk4adi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-19 08:37:57.000000 pk4adi-0.1.2/pk4adi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 08:37:57.738595 pk4adi-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1845 2023-06-19 08:28:36.000000 pk4adi-0.1.2/setup.py
```

### Comparing `pk4adi-0.1.1/LICENSE` & `pk4adi-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pk4adi-0.1.1/PKG-INFO` & `pk4adi-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pk4adi
-Version: 0.1.1
+Version: 0.1.2
 Summary: Using PK to Measure the Performance of Anesthetic Depth Indicators.
-Home-page: https://github.com/xfz329/pk.git
+Home-page: https://github.com/xfz329/pk4adi.git
 Author: silencejiang
 Author-email: silencejiang@zju.edu.cn
 License: MIT License
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -17,25 +17,25 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pk4adi
 
 ## Project Information
 
-The package's name pk4adi is short for "PK for anesthetic depth indicators". The PK (Prediction probability) was firstly proposed by [Docor Warren D. Smith](https://www.csus.edu/faculty/s/smithwd/) in the paper [Measuring the Performance of Anesthetic Depth Indicators](https://pubs.asahq.org/anesthesiology/article/84/1/38/35261/Measuring-the-Performance-of-Anesthetic-Depth) in 1996. Docor Warren D. Smith and his team provide a tool to calculate PK writen using the xls macro language.
+The package's name pk4adi is short for "PK for anesthetic depth indicators". The PK (Prediction probability) was firstly proposed by [Docor Warren D. Smith](https://www.csus.edu/faculty/s/smithwd/) in the paper [Measuring the Performance of Anesthetic Depth Indicators](https://pubs.asahq.org/anesthesiology/article/84/1/38/35261/Measuring-the-Performance-of-Anesthetic-Depth) in 1996. Docor Warren D. Smith and his team provide a tool to calculate PK writen using the excel macro language.
 
-Our team provide a reimplementation of the PK tools developed using the Python language with easy using apis in this package. The project is fully open source in the [github](https://github.com/xfz329/pk). The lastest version released could be found [here](https://github.com/xfz329/pk/releases). 
+Our team provide a reimplementation of the PK tools developed using the Python language with easy using apis in this package. The project is fully open source in the [github](https://github.com/xfz329/pk4adi). The lastest version released could be found [here](https://github.com/xfz329/pk4adi/releases). 
 
-Please feel free to contact us(silencejiang@zju.edu.cn). Any kind of feedbacks is welcomed. You could report any bugs or issues when using pk4adi in the github [project](https://github.com/xfz329/pk/issues).
+Moreover, a gui version of pk4adi is under development, which is names [pk4adi_gui](https://github.com/xfz329/pk4adi_gui) actually. This project is also open source in the github.
 
-Specially, a gui version of pk4adi is under development. We will also open source the gui version project.
+Please feel free to contact us(silencejiang@zju.edu.cn). Any kind of feedback is welcomed. You could report any bugs or issues when using pk4adi in the github [project](https://github.com/xfz329/pk4adi/issues).
 
 ## Changelogs
 
-Please refer the [changelog.md](https://github.com/xfz329/pk/blob/main/CHANGELOG.md) for details.
+Please refer the [changelog.md](https://github.com/xfz329/pk4adi/blob/main/CHANGELOG.md) for details.
 
 ## Requirements
 
 ### Python
 
 ```
 Python 3.8 or greater.
@@ -57,25 +57,27 @@
 pip install pk4adi
 ```
 
 ## APIs
 
 1. calculate_pk of module pk.py.
 ```
-calculate_pk(x_in , y_in):
+calculate_pk(x_in , y_in , auto_print = True):
 
 Compute the pk value to Measure the Performance of Anesthetic Depth Indicators.
-print_pk() will be called before return the ans.
+print_pk() will be called before return the ans by default.
 
 Parameters
 ----------
 x_in : a list or a pandas series (pandas.Series()).
     Indicator.
 y_in : a list or a pandas series (pandas.Series()).
     State.
+auto_print : bool.
+    Whether print the ans before returning the ans or not.
 
 Returns
 -------
 ans : a dict.
     A dict containing all the matrix and variables involved in.
     Use to script 'print(ans.keys())' to get the details.
     The most important variables all already been printed.
@@ -100,25 +102,27 @@
 Returns
 -------
 Nothing will be returned.
 
 ```   
 3. compare_pks of module pkc.py.
 ```
-compare_pks(pk1, pk2):
+compare_pks(pk1, pk2 , auto_print = True):
 
 Compare two answers of the pk values, which is the output of the function calculate_pk().
-print_pks() will be called before return the ans.
+print_pks() will be called before return the ans by default.
 
 Parameters
 ----------
 pk1 : a dict.
     The output of the function calculate_pk().
 pk2 : a dict.
     The output of the function calculate_pk().
+auto_print : bool.
+    Whether print the ans before returning the ans or not.
 
 Returns
 -------
 ans : a dict.
     A dict containing all the matrix and variables involved in.
     Use to script 'print(ans.keys())' to get the details.
     The most important variables all already been printed.
@@ -187,44 +191,26 @@
 ```python
 from pk4adi.pk import calculate_pk
 from pk4adi.pkc import compare_pks
 
 x1 = [ 1, 1, 2, 2, 2, 2, 3, 3, 3, 3, 4, 4, 4, 4, 4, 5, 5, 5, 5, 6, 6, 6, 6, 6 ]
 y1 = [ 1, 1, 1, 1, 1, 2, 1, 1, 3, 3, 2, 2, 2, 2, 2, 1, 3, 3, 3, 3, 3, 3, 3, 3 ]
 
-pk1 = calculate_pk(x_in = x1, y_in = y1)
+pk1 = calculate_pk(x_in = x1, y_in = y1 , auto_print = False)
 
 x2 = [ 1, 1, 2, 2, 2, 2, 3, 3, 3, 3, 4, 4, 4, 4, 4, 5, 5, 5, 5, 6, 6, 6, 6, 6 ]
 y2 = [ 1, 1, 2, 1, 1, 2, 1, 2, 3, 3, 2, 2, 1, 2, 2, 2, 3, 3, 3, 3, 2, 3, 3, 2 ]
 
-pk2 = calculate_pk(x_in = x2, y_in = y2)
+pk2 = calculate_pk(x_in = x2, y_in = y2 , auto_print = False)
 
 ans = compare_pks(pk1, pk2)
 ```
 You will get the following output.
 ```
 ==============
-PK calculation
-==============
-
-   PK    SE0    SE1  jack_ok      PKj    SEj
------  -----  -----  ---------  -----  -----
-0.867  0.065  0.066  True       0.866  0.070
-
-
-==============
-PK calculation
-==============
-
-   PK    SE0    SE1  jack_ok      PKj    SEj
------  -----  -----  ---------  -----  -----
-0.798  0.073  0.068  True       0.799  0.073
-
-
-==============
 PKs comparison
 ==============
 
 =================
 For Group (z-test)
 =================
 
@@ -257,18 +243,18 @@
 
 # Development
 
 ## Contribute
 
 Please feel free to contact us(silencejiang@zju.edu.cn). Any kind of feedbacks is welcomed and appreciated.
 - Check out the wiki for development info (coming soon!).
-- Fork us from @xfz329's [main](https://github.com/xfz329/pk).
-- Report an issue [here](https://github.com/xfz329/pk/issues).
-- Report a bug with data.
+- Fork us from @xfz329's [main](https://github.com/xfz329/pk4adi) and star us.
+- Report an issue or a bug with data [here](https://github.com/xfz329/pk4adi/issues).
+- Any other free discussion [here](https://github.com/xfz329/pk4adi/discussions).
 
 ## References
 1. [Measuring the Performance of Anesthetic Depth Indicators](https://pubs.asahq.org/anesthesiology/article/84/1/38/35261/Measuring-the-Performance-of-Anesthetic-Depth)
-2. [A measure of association for assessing prediction accuracy that is a general](https://onlinelibrary.wiley.com/doi/10.1002/(SICI)1097-0258(19960615)15:11%3C1199::AID-SIM218%3E3.0.CO;2-Y)
+2. [A measure of association for assessing prediction accuracy that is a generalization of non-parametric ROC area](https://onlinelibrary.wiley.com/doi/10.1002/(SICI)1097-0258(19960615)15:11%3C1199::AID-SIM218%3E3.0.CO;2-Y)
 3. [Excel 4.0 Macro Functions Reference - My Online Training Hub](https://d13ot9o61jdzpp.cloudfront.net/files/Excel%204.0%20Macro%20Functions%20Reference.pdf)
```

### Comparing `pk4adi-0.1.1/README.md` & `pk4adi-0.1.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # pk4adi
 
 ## Project Information
 
-The package's name pk4adi is short for "PK for anesthetic depth indicators". The PK (Prediction probability) was firstly proposed by [Docor Warren D. Smith](https://www.csus.edu/faculty/s/smithwd/) in the paper [Measuring the Performance of Anesthetic Depth Indicators](https://pubs.asahq.org/anesthesiology/article/84/1/38/35261/Measuring-the-Performance-of-Anesthetic-Depth) in 1996. Docor Warren D. Smith and his team provide a tool to calculate PK writen using the xls macro language.
+The package's name pk4adi is short for "PK for anesthetic depth indicators". The PK (Prediction probability) was firstly proposed by [Docor Warren D. Smith](https://www.csus.edu/faculty/s/smithwd/) in the paper [Measuring the Performance of Anesthetic Depth Indicators](https://pubs.asahq.org/anesthesiology/article/84/1/38/35261/Measuring-the-Performance-of-Anesthetic-Depth) in 1996. Docor Warren D. Smith and his team provide a tool to calculate PK writen using the excel macro language.
 
-Our team provide a reimplementation of the PK tools developed using the Python language with easy using apis in this package. The project is fully open source in the [github](https://github.com/xfz329/pk). The lastest version released could be found [here](https://github.com/xfz329/pk/releases). 
+Our team provide a reimplementation of the PK tools developed using the Python language with easy using apis in this package. The project is fully open source in the [github](https://github.com/xfz329/pk4adi). The lastest version released could be found [here](https://github.com/xfz329/pk4adi/releases). 
 
-Please feel free to contact us(silencejiang@zju.edu.cn). Any kind of feedbacks is welcomed. You could report any bugs or issues when using pk4adi in the github [project](https://github.com/xfz329/pk/issues).
+Moreover, a gui version of pk4adi is under development, which is names [pk4adi_gui](https://github.com/xfz329/pk4adi_gui) actually. This project is also open source in the github.
 
-Specially, a gui version of pk4adi is under development. We will also open source the gui version project.
+Please feel free to contact us(silencejiang@zju.edu.cn). Any kind of feedback is welcomed. You could report any bugs or issues when using pk4adi in the github [project](https://github.com/xfz329/pk4adi/issues).
 
 ## Changelogs
 
-Please refer the [changelog.md](https://github.com/xfz329/pk/blob/main/CHANGELOG.md) for details.
+Please refer the [changelog.md](https://github.com/xfz329/pk4adi/blob/main/CHANGELOG.md) for details.
 
 ## Requirements
 
 ### Python
 
 ```
 Python 3.8 or greater.
@@ -38,25 +38,27 @@
 pip install pk4adi
 ```
 
 ## APIs
 
 1. calculate_pk of module pk.py.
 ```
-calculate_pk(x_in , y_in):
+calculate_pk(x_in , y_in , auto_print = True):
 
 Compute the pk value to Measure the Performance of Anesthetic Depth Indicators.
-print_pk() will be called before return the ans.
+print_pk() will be called before return the ans by default.
 
 Parameters
 ----------
 x_in : a list or a pandas series (pandas.Series()).
     Indicator.
 y_in : a list or a pandas series (pandas.Series()).
     State.
+auto_print : bool.
+    Whether print the ans before returning the ans or not.
 
 Returns
 -------
 ans : a dict.
     A dict containing all the matrix and variables involved in.
     Use to script 'print(ans.keys())' to get the details.
     The most important variables all already been printed.
@@ -81,25 +83,27 @@
 Returns
 -------
 Nothing will be returned.
 
 ```   
 3. compare_pks of module pkc.py.
 ```
-compare_pks(pk1, pk2):
+compare_pks(pk1, pk2 , auto_print = True):
 
 Compare two answers of the pk values, which is the output of the function calculate_pk().
-print_pks() will be called before return the ans.
+print_pks() will be called before return the ans by default.
 
 Parameters
 ----------
 pk1 : a dict.
     The output of the function calculate_pk().
 pk2 : a dict.
     The output of the function calculate_pk().
+auto_print : bool.
+    Whether print the ans before returning the ans or not.
 
 Returns
 -------
 ans : a dict.
     A dict containing all the matrix and variables involved in.
     Use to script 'print(ans.keys())' to get the details.
     The most important variables all already been printed.
@@ -168,44 +172,26 @@
 ```python
 from pk4adi.pk import calculate_pk
 from pk4adi.pkc import compare_pks
 
 x1 = [ 1, 1, 2, 2, 2, 2, 3, 3, 3, 3, 4, 4, 4, 4, 4, 5, 5, 5, 5, 6, 6, 6, 6, 6 ]
 y1 = [ 1, 1, 1, 1, 1, 2, 1, 1, 3, 3, 2, 2, 2, 2, 2, 1, 3, 3, 3, 3, 3, 3, 3, 3 ]
 
-pk1 = calculate_pk(x_in = x1, y_in = y1)
+pk1 = calculate_pk(x_in = x1, y_in = y1 , auto_print = False)
 
 x2 = [ 1, 1, 2, 2, 2, 2, 3, 3, 3, 3, 4, 4, 4, 4, 4, 5, 5, 5, 5, 6, 6, 6, 6, 6 ]
 y2 = [ 1, 1, 2, 1, 1, 2, 1, 2, 3, 3, 2, 2, 1, 2, 2, 2, 3, 3, 3, 3, 2, 3, 3, 2 ]
 
-pk2 = calculate_pk(x_in = x2, y_in = y2)
+pk2 = calculate_pk(x_in = x2, y_in = y2 , auto_print = False)
 
 ans = compare_pks(pk1, pk2)
 ```
 You will get the following output.
 ```
 ==============
-PK calculation
-==============
-
-   PK    SE0    SE1  jack_ok      PKj    SEj
------  -----  -----  ---------  -----  -----
-0.867  0.065  0.066  True       0.866  0.070
-
-
-==============
-PK calculation
-==============
-
-   PK    SE0    SE1  jack_ok      PKj    SEj
------  -----  -----  ---------  -----  -----
-0.798  0.073  0.068  True       0.799  0.073
-
-
-==============
 PKs comparison
 ==============
 
 =================
 For Group (z-test)
 =================
 
@@ -238,16 +224,16 @@
 
 # Development
 
 ## Contribute
 
 Please feel free to contact us(silencejiang@zju.edu.cn). Any kind of feedbacks is welcomed and appreciated.
 - Check out the wiki for development info (coming soon!).
-- Fork us from @xfz329's [main](https://github.com/xfz329/pk).
-- Report an issue [here](https://github.com/xfz329/pk/issues).
-- Report a bug with data.
+- Fork us from @xfz329's [main](https://github.com/xfz329/pk4adi) and star us.
+- Report an issue or a bug with data [here](https://github.com/xfz329/pk4adi/issues).
+- Any other free discussion [here](https://github.com/xfz329/pk4adi/discussions).
 
 ## References
 1. [Measuring the Performance of Anesthetic Depth Indicators](https://pubs.asahq.org/anesthesiology/article/84/1/38/35261/Measuring-the-Performance-of-Anesthetic-Depth)
-2. [A measure of association for assessing prediction accuracy that is a general](https://onlinelibrary.wiley.com/doi/10.1002/(SICI)1097-0258(19960615)15:11%3C1199::AID-SIM218%3E3.0.CO;2-Y)
+2. [A measure of association for assessing prediction accuracy that is a generalization of non-parametric ROC area](https://onlinelibrary.wiley.com/doi/10.1002/(SICI)1097-0258(19960615)15:11%3C1199::AID-SIM218%3E3.0.CO;2-Y)
 3. [Excel 4.0 Macro Functions Reference - My Online Training Hub](https://d13ot9o61jdzpp.cloudfront.net/files/Excel%204.0%20Macro%20Functions%20Reference.pdf)
```

### Comparing `pk4adi-0.1.1/pk4adi/pk.py` & `pk4adi-0.1.2/pk4adi/pk.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,25 +9,27 @@
 import math
 import pandas as pd
 import numpy as np
 from pk4adi.utils import print_table
 
 __all__  = ["calculate_pk", "print_pk"]
 
-def calculate_pk(x_in , y_in):
+def calculate_pk(x_in , y_in, auto_print = True):
     """
     Compute the pk value to Measure the Performance of Anesthetic Depth Indicators.
-        print_pk() will be called before return the ans.
+        print_pk() will be called before return the ans by default.
 
     Parameters
     ----------
     x_in : a list or a pandas series (pandas.Series()).
         Indicator.
     y_in : a list or a pandas series (pandas.Series()).
         State.
+    auto_print : bool.
+        Whether print the ans before returning the ans or not.
 
     Returns
     -------
     ans : a dict.
         A dict containing all the matrix and variables involved in.
         Use to script 'print(ans.keys())' to get the details.
         The most important variables all already been printed.
@@ -254,15 +256,16 @@
     ans.update({"PKm" : data["PKm"]})
     ans.update({"SPKm" : SPKm})
     ans.update({"SSPKm" : SSPKm})
     ans.update({"PKj" : PKj})
     ans.update({"SEj" : SEj})
 
     # format and print.
-    print_pk(ans)
+    if auto_print:
+        print_pk(ans)
 
     # return the ans.
     return ans
 
 def print_pk(result, floatfmt=".3f", tablefmt='simple'):
     """
     Pretty display of a pk calculation result.
@@ -300,13 +303,13 @@
         print_table(df, floatfmt, tablefmt)
 
 
 if __name__ == "__main__":
 
     x = [ 0, 0, 0, 0, 0, 0]
     y = [ 1, 1, 1, 1, 1, 2]
-    calculate_pk(x, y)
+    calculate_pk(x, y , False)
 
     x = [0, 0, 0, 0, 0, 0, 1, 1, 2]
     y = [1, 1, 1, 1, 1, 2, 3, 3, 4]
     calculate_pk(x, y)
```

### Comparing `pk4adi-0.1.1/pk4adi/pkc.py` & `pk4adi-0.1.2/pk4adi/pkc.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,25 +10,27 @@
 import pandas as pd
 from scipy.stats import norm, t
 from pk4adi.utils import print_table
 from pk4adi.pk import calculate_pk
 
 __all__  = ["compare_pks", "print_pks"]
 
-def compare_pks(pk1, pk2):
+def compare_pks(pk1, pk2, auto_print = True):
     """
     Compare two answers of the pk values, which is the output of the function calculate_pk().
-        print_pks() will be called before return the ans.
+        print_pks() will be called before return the ans by default.
 
     Parameters
     ----------
     pk1 : a dict.
         The output of the function calculate_pk().
     pk2 : a dict.
         The output of the function calculate_pk().
+    auto_print : bool.
+        Whether print the ans before returning the ans or not.
 
     Returns
     -------
     ans : a dict.
         A dict containing all the matrix and variables involved in.
         Use to script 'print(ans.keys())' to get the details.
         The most important variables all already been printed.
@@ -92,15 +94,16 @@
     ans.update({"PKDJ": PKDJ})
     ans.update({"SEDJ": SEDJ})
     ans.update({"TD": TD})
     ans.update({"TP": TP})
     ans.update({"TJ": TJ})
 
     # format and print.
-    print_pks(ans)
+    if auto_print:
+        print_pks(ans)
 
     # return the ans.
     return ans
 
 
 def print_pks(result, floatfmt=".3f", tablefmt='simple'):
     """
@@ -262,18 +265,17 @@
         return "P < 0.001"
 
 if __name__ == "__main__":
 
     x1 = [ 1, 1, 2, 2, 2, 2, 3, 3, 3, 3, 4, 4, 4, 4, 4, 5, 5, 5, 5, 6, 6, 6, 6, 6 ]
     y1 = [ 1, 1, 1, 1, 1, 2, 1, 1, 3, 3, 2, 2, 2, 2, 2, 1, 3, 3, 3, 3, 3, 3, 3, 3 ]
 
-    pk1 = calculate_pk(x_in = x1, y_in = y1)
+    pk1 = calculate_pk(x_in = x1, y_in = y1 , auto_print = False)
 
     x2 = [ 1, 1, 2, 2, 2, 2, 3, 3, 3, 3, 4, 4, 4, 4, 4, 5, 5, 5, 5, 6, 6, 6, 6, 6 ]
     y2 = [ 1, 1, 2, 1, 1, 2, 1, 2, 3, 3, 2, 2, 1, 2, 2, 2, 3, 3, 3, 3, 2, 3, 3, 2 ]
 
-    pk2 = calculate_pk(x_in = x2, y_in = y2)
+    pk2 = calculate_pk(x_in = x2, y_in = y2 , auto_print = False)
 
     ans = compare_pks(pk1, pk2)
-    print_pks(ans)
```

### Comparing `pk4adi-0.1.1/pk4adi/utils.py` & `pk4adi-0.1.2/pk4adi/utils.py`

 * *Files identical despite different names*

### Comparing `pk4adi-0.1.1/pk4adi.egg-info/PKG-INFO` & `pk4adi-0.1.2/pk4adi.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pk4adi
-Version: 0.1.1
+Version: 0.1.2
 Summary: Using PK to Measure the Performance of Anesthetic Depth Indicators.
-Home-page: https://github.com/xfz329/pk.git
+Home-page: https://github.com/xfz329/pk4adi.git
 Author: silencejiang
 Author-email: silencejiang@zju.edu.cn
 License: MIT License
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -17,25 +17,25 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pk4adi
 
 ## Project Information
 
-The package's name pk4adi is short for "PK for anesthetic depth indicators". The PK (Prediction probability) was firstly proposed by [Docor Warren D. Smith](https://www.csus.edu/faculty/s/smithwd/) in the paper [Measuring the Performance of Anesthetic Depth Indicators](https://pubs.asahq.org/anesthesiology/article/84/1/38/35261/Measuring-the-Performance-of-Anesthetic-Depth) in 1996. Docor Warren D. Smith and his team provide a tool to calculate PK writen using the xls macro language.
+The package's name pk4adi is short for "PK for anesthetic depth indicators". The PK (Prediction probability) was firstly proposed by [Docor Warren D. Smith](https://www.csus.edu/faculty/s/smithwd/) in the paper [Measuring the Performance of Anesthetic Depth Indicators](https://pubs.asahq.org/anesthesiology/article/84/1/38/35261/Measuring-the-Performance-of-Anesthetic-Depth) in 1996. Docor Warren D. Smith and his team provide a tool to calculate PK writen using the excel macro language.
 
-Our team provide a reimplementation of the PK tools developed using the Python language with easy using apis in this package. The project is fully open source in the [github](https://github.com/xfz329/pk). The lastest version released could be found [here](https://github.com/xfz329/pk/releases). 
+Our team provide a reimplementation of the PK tools developed using the Python language with easy using apis in this package. The project is fully open source in the [github](https://github.com/xfz329/pk4adi). The lastest version released could be found [here](https://github.com/xfz329/pk4adi/releases). 
 
-Please feel free to contact us(silencejiang@zju.edu.cn). Any kind of feedbacks is welcomed. You could report any bugs or issues when using pk4adi in the github [project](https://github.com/xfz329/pk/issues).
+Moreover, a gui version of pk4adi is under development, which is names [pk4adi_gui](https://github.com/xfz329/pk4adi_gui) actually. This project is also open source in the github.
 
-Specially, a gui version of pk4adi is under development. We will also open source the gui version project.
+Please feel free to contact us(silencejiang@zju.edu.cn). Any kind of feedback is welcomed. You could report any bugs or issues when using pk4adi in the github [project](https://github.com/xfz329/pk4adi/issues).
 
 ## Changelogs
 
-Please refer the [changelog.md](https://github.com/xfz329/pk/blob/main/CHANGELOG.md) for details.
+Please refer the [changelog.md](https://github.com/xfz329/pk4adi/blob/main/CHANGELOG.md) for details.
 
 ## Requirements
 
 ### Python
 
 ```
 Python 3.8 or greater.
@@ -57,25 +57,27 @@
 pip install pk4adi
 ```
 
 ## APIs
 
 1. calculate_pk of module pk.py.
 ```
-calculate_pk(x_in , y_in):
+calculate_pk(x_in , y_in , auto_print = True):
 
 Compute the pk value to Measure the Performance of Anesthetic Depth Indicators.
-print_pk() will be called before return the ans.
+print_pk() will be called before return the ans by default.
 
 Parameters
 ----------
 x_in : a list or a pandas series (pandas.Series()).
     Indicator.
 y_in : a list or a pandas series (pandas.Series()).
     State.
+auto_print : bool.
+    Whether print the ans before returning the ans or not.
 
 Returns
 -------
 ans : a dict.
     A dict containing all the matrix and variables involved in.
     Use to script 'print(ans.keys())' to get the details.
     The most important variables all already been printed.
@@ -100,25 +102,27 @@
 Returns
 -------
 Nothing will be returned.
 
 ```   
 3. compare_pks of module pkc.py.
 ```
-compare_pks(pk1, pk2):
+compare_pks(pk1, pk2 , auto_print = True):
 
 Compare two answers of the pk values, which is the output of the function calculate_pk().
-print_pks() will be called before return the ans.
+print_pks() will be called before return the ans by default.
 
 Parameters
 ----------
 pk1 : a dict.
     The output of the function calculate_pk().
 pk2 : a dict.
     The output of the function calculate_pk().
+auto_print : bool.
+    Whether print the ans before returning the ans or not.
 
 Returns
 -------
 ans : a dict.
     A dict containing all the matrix and variables involved in.
     Use to script 'print(ans.keys())' to get the details.
     The most important variables all already been printed.
@@ -187,44 +191,26 @@
 ```python
 from pk4adi.pk import calculate_pk
 from pk4adi.pkc import compare_pks
 
 x1 = [ 1, 1, 2, 2, 2, 2, 3, 3, 3, 3, 4, 4, 4, 4, 4, 5, 5, 5, 5, 6, 6, 6, 6, 6 ]
 y1 = [ 1, 1, 1, 1, 1, 2, 1, 1, 3, 3, 2, 2, 2, 2, 2, 1, 3, 3, 3, 3, 3, 3, 3, 3 ]
 
-pk1 = calculate_pk(x_in = x1, y_in = y1)
+pk1 = calculate_pk(x_in = x1, y_in = y1 , auto_print = False)
 
 x2 = [ 1, 1, 2, 2, 2, 2, 3, 3, 3, 3, 4, 4, 4, 4, 4, 5, 5, 5, 5, 6, 6, 6, 6, 6 ]
 y2 = [ 1, 1, 2, 1, 1, 2, 1, 2, 3, 3, 2, 2, 1, 2, 2, 2, 3, 3, 3, 3, 2, 3, 3, 2 ]
 
-pk2 = calculate_pk(x_in = x2, y_in = y2)
+pk2 = calculate_pk(x_in = x2, y_in = y2 , auto_print = False)
 
 ans = compare_pks(pk1, pk2)
 ```
 You will get the following output.
 ```
 ==============
-PK calculation
-==============
-
-   PK    SE0    SE1  jack_ok      PKj    SEj
------  -----  -----  ---------  -----  -----
-0.867  0.065  0.066  True       0.866  0.070
-
-
-==============
-PK calculation
-==============
-
-   PK    SE0    SE1  jack_ok      PKj    SEj
------  -----  -----  ---------  -----  -----
-0.798  0.073  0.068  True       0.799  0.073
-
-
-==============
 PKs comparison
 ==============
 
 =================
 For Group (z-test)
 =================
 
@@ -257,18 +243,18 @@
 
 # Development
 
 ## Contribute
 
 Please feel free to contact us(silencejiang@zju.edu.cn). Any kind of feedbacks is welcomed and appreciated.
 - Check out the wiki for development info (coming soon!).
-- Fork us from @xfz329's [main](https://github.com/xfz329/pk).
-- Report an issue [here](https://github.com/xfz329/pk/issues).
-- Report a bug with data.
+- Fork us from @xfz329's [main](https://github.com/xfz329/pk4adi) and star us.
+- Report an issue or a bug with data [here](https://github.com/xfz329/pk4adi/issues).
+- Any other free discussion [here](https://github.com/xfz329/pk4adi/discussions).
 
 ## References
 1. [Measuring the Performance of Anesthetic Depth Indicators](https://pubs.asahq.org/anesthesiology/article/84/1/38/35261/Measuring-the-Performance-of-Anesthetic-Depth)
-2. [A measure of association for assessing prediction accuracy that is a general](https://onlinelibrary.wiley.com/doi/10.1002/(SICI)1097-0258(19960615)15:11%3C1199::AID-SIM218%3E3.0.CO;2-Y)
+2. [A measure of association for assessing prediction accuracy that is a generalization of non-parametric ROC area](https://onlinelibrary.wiley.com/doi/10.1002/(SICI)1097-0258(19960615)15:11%3C1199::AID-SIM218%3E3.0.CO;2-Y)
 3. [Excel 4.0 Macro Functions Reference - My Online Training Hub](https://d13ot9o61jdzpp.cloudfront.net/files/Excel%204.0%20Macro%20Functions%20Reference.pdf)
```

### Comparing `pk4adi-0.1.1/setup.py` & `pk4adi-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 
 setup(
     name="pk4adi",
     version=__version__,
     author="silencejiang",
     author_email="silencejiang@zju.edu.cn",
-    url='https://github.com/xfz329/pk.git',
+    url='https://github.com/xfz329/pk4adi.git',
     description=short_description,
     long_description_content_type="text/markdown",
     long_description=long_description,
     python_requires=">=3.8",
     install_requires=get_install_requires(),
     packages=find_packages(),
     license='MIT License',
```

