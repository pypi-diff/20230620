# Comparing `tmp/LeoX-0.5.0.tar.gz` & `tmp/LeoX-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/LeoX-0.5.0.tar", last modified: Mon Jun 12 15:50:00 2023, max compression
+gzip compressed data, was "LeoX-0.6.0.tar", last modified: Tue Jun 20 15:10:34 2023, max compression
```

## Comparing `LeoX-0.5.0.tar` & `LeoX-0.6.0.tar`

### file list

```diff
@@ -1,28 +1,23 @@
-drwxr-xr-x   0 ledso    (251734) ecsvip   (15071)        0 2023-06-12 15:50:00.893678 LeoX-0.5.0/
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)       62 2022-06-01 08:59:44.000000 LeoX-0.5.0/.gitignore
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)     1083 2021-09-27 19:02:46.000000 LeoX-0.5.0/LICENSE
-drwxr-xr-x   0 ledso    (251734) ecsvip   (15071)        0 2023-06-12 15:50:00.665677 LeoX-0.5.0/LeoX.egg-info/
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)     9626 2023-06-12 15:49:59.000000 LeoX-0.5.0/LeoX.egg-info/PKG-INFO
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)      402 2023-06-12 15:49:59.000000 LeoX-0.5.0/LeoX.egg-info/SOURCES.txt
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)        1 2023-06-12 15:49:59.000000 LeoX-0.5.0/LeoX.egg-info/dependency_links.txt
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)       41 2023-06-12 15:49:59.000000 LeoX-0.5.0/LeoX.egg-info/entry_points.txt
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)       19 2023-06-12 15:49:59.000000 LeoX-0.5.0/LeoX.egg-info/requires.txt
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)        3 2023-06-12 15:49:59.000000 LeoX-0.5.0/LeoX.egg-info/top_level.txt
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)       26 2021-09-27 19:02:46.000000 LeoX-0.5.0/MANIFEST.in
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)     9626 2023-06-12 15:50:00.892678 LeoX-0.5.0/PKG-INFO
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)     8347 2022-06-01 08:59:44.000000 LeoX-0.5.0/README.md
-drwxr-xr-x   0 ledso    (251734) ecsvip   (15071)        0 2023-06-12 15:50:00.672677 LeoX-0.5.0/batch_examples/
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)      174 2022-06-01 08:59:44.000000 LeoX-0.5.0/batch_examples/batch.sh
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)      326 2021-10-13 13:55:43.000000 LeoX-0.5.0/batch_examples/slurm.sh
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)      206 2022-06-01 08:59:44.000000 LeoX-0.5.0/batch_examples/ts.sh
-drwxr-xr-x   0 ledso    (251734) ecsvip   (15071)        0 2023-06-12 15:50:00.888678 LeoX-0.5.0/lx/
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)        0 2021-09-27 19:02:46.000000 LeoX-0.5.0/lx/__init__.py
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)     7484 2023-06-12 15:49:39.000000 LeoX-0.5.0/lx/__main__.py
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)       62 2023-06-12 15:49:39.000000 LeoX-0.5.0/lx/__version__.py
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)     2241 2022-06-01 08:59:44.000000 LeoX-0.5.0/lx/batch_lx.py
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)    11444 2023-06-12 15:49:39.000000 LeoX-0.5.0/lx/conf_search.py
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)     8053 2023-05-03 15:29:51.000000 LeoX-0.5.0/lx/ld.py
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)     7217 2022-06-01 08:59:44.000000 LeoX-0.5.0/lx/omega.py
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)    32940 2023-06-12 15:49:39.000000 LeoX-0.5.0/lx/tools.py
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)       38 2023-06-12 15:50:00.894678 LeoX-0.5.0/setup.cfg
--rw-r--r--   0 ledso    (251734) ecsvip   (15071)     3588 2023-06-12 15:49:39.000000 LeoX-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:10:34.761839 LeoX-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-20 15:10:24.000000 LeoX-0.6.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:10:34.761839 LeoX-0.6.0/LeoX.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8697 2023-06-20 15:10:34.000000 LeoX-0.6.0/LeoX.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-20 15:10:34.000000 LeoX-0.6.0/LeoX.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:10:34.000000 LeoX-0.6.0/LeoX.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-20 15:10:34.000000 LeoX-0.6.0/LeoX.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-20 15:10:34.000000 LeoX-0.6.0/LeoX.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-20 15:10:34.000000 LeoX-0.6.0/LeoX.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-20 15:10:24.000000 LeoX-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8697 2023-06-20 15:10:34.761839 LeoX-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-06-20 15:10:24.000000 LeoX-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:10:34.761839 LeoX-0.6.0/lx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:10:24.000000 LeoX-0.6.0/lx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7688 2023-06-20 15:10:24.000000 LeoX-0.6.0/lx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-20 15:10:24.000000 LeoX-0.6.0/lx/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-20 15:10:24.000000 LeoX-0.6.0/lx/batch_lx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11444 2023-06-20 15:10:24.000000 LeoX-0.6.0/lx/conf_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8053 2023-06-20 15:10:24.000000 LeoX-0.6.0/lx/ld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-06-20 15:10:24.000000 LeoX-0.6.0/lx/omega.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34404 2023-06-20 15:10:24.000000 LeoX-0.6.0/lx/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 15:10:34.761839 LeoX-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-06-20 15:10:24.000000 LeoX-0.6.0/setup.py
```

### Comparing `LeoX-0.5.0/LICENSE` & `LeoX-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `LeoX-0.5.0/LeoX.egg-info/PKG-INFO` & `LeoX-0.6.0/LeoX.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,130 +1,130 @@
 Metadata-Version: 2.1
 Name: LeoX
-Version: 0.5.0
+Version: 0.6.0
 Summary: Spectrum simulations with TD(A)-DFT
 Home-page: https://github.com/LeonardoESousa/LeoX
 Author: Leonardo Evaristo de Sousa
 Author-email: leonardo.sousa137@gmail.com
 License: MIT
-Description: 
-        ﻿# LeoX - Light emission and exciton diffusion in organic molecules 
-        
-        [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
-        [![license](https://img.shields.io/github/license/LeonardoESousa/LeoX?style=plastic)]()
-        [![down](https://img.shields.io/pypi/dm/LeoX)]()
-        [![maint](https://img.shields.io/maintenance/yes/2021)]()
-        [![commit](https://img.shields.io/github/last-commit/LeonardoESousa/LeoX?style=plastic)]()
-        
-        
-        
-        A package for absorption and fluorescence spectrum simulations using the nuclear ensemble method along with TD(A)-DFT. Estimation of singlet exciton properties (Förster radius, lifetime, diffusion length). Long-range separation parameter tuning. Stochastic conformational search.  Interfaces with the Gaussian (09 or 16) package.
-        
-        
-        Table of Contents
-        =================
-        <!--ts-->
-        * [Cite as:](#cite-as)
-        * [What does this program do?](#what-does-this-program-do)
-        * [What is necessary to use it?](#what-is-necessary-to-use-it)
-        * [How to install it?](#how-to-install-it)
-        * [How to use it?](#how-to-use-it)
-           
-        <!--te-->
-        
-        ## Cite as:
-        
-        > de Sousa, L. E., Bueno, F. T., e Silva, G. M., da Silva Filho, D. A., & de Oliveira Neto, P. H. (2019). Fast predictions of exciton diffusion length in organic materials. Journal of Materials Chemistry C, 7(14), 4066-4071.
-        
-        
-        ## What does this program do?
-        
-        1.  Spectrum simulation:
-            - Calculates Absorption and Fluorescence spectrum simulations using TD(A)-DFT.
-            - Calculations include vibrational contributions to the spectra. 
-            - Optionally, they may also include solvent effects either by PCM or by a state specific solvation model.
-        2.  Exciton properties:   
-            - Calculates Förster radius for transfers between two molecules of equal or different type.
-            - Calculates fluorescence lifetimes.
-            - Calculates singlet exciton diffusion lengths.
-        3.  Extra features:
-            - Tunes the w parameter of long-range separated functionals.
-            - Extracts last geometry from Gaussian log file.
-            - Runs a stochastic coformational search algorithm.
-        
-        
-        ## What is necessary to use it?
-        
-         -  The program requires that the Gaussian quantum chemistry software (G09 or G16) be installed, as it interfaces with it.
-        
-        -   The first step for running spectrum calculations or conformational searches is providing a Gaussian log file for a frequency calculation in the S0 state, if the goal is computing an absorption spectrum, or S1 state, if the objective is calculating a fluoresence spectrum. All frequencies must be real.  
-        
-        -   To obtain estimates for Förster radius, fluorescence lifetimes and singlet exciton diffusion lengths, it is necessary to first perform both absorption and emission spectra calculations for the molecule of interest.
-        
-        ## How to install it?
-        
-        Run:
-        
-        `pip install LeoX`
-        
-        Alternatively, clone the repository to your computer. Inside the LeoX folder, run:
-        
-        `pip install .`
-        
-        Depending on the operating system, the commands above may need to be replace by
-        
-        `pip3 install LeoX` or `pip3 install .`
-        
-        Once installed, you should be able to run the program from any folder by just using the `lx` command.
-        
-        ## How to use it?
-        
-        1. For spectrum simulations:
-        
-            - Create a folder for your project. Add the log file for the frequency calculation to your folder. Run the lx command. Choose option 1 and follow the instructions to select the parameters of the calculation.
-            - Add a bash script file to the folder to control execution. This file depends on which batch system you use. Examples for users of slurm or task spooler (ts) are presented [here](https://github.com/LeonardoESousa/LeoX/tree/master/batch_examples).
-            - Run the `lx` command again, choose option 2 and follow the instructions. Once the calculations are running, you may use option 4 to check the progress or option 9 to abort.
-            <img width="575" alt="LeoX1" src="https://user-images.githubusercontent.com/94139072/144780278-ef3b8ced-af82-4a9d-a8a5-667ebdcbdd71.png">
-        
-            - Once all calculations are done, run the `lx` command and choose option 3. Follow the instructions to set the parameters and the spectrum will be generated.
-            <img width="436" alt="LeoX2" src="https://user-images.githubusercontent.com/94139072/144780487-7d0a5800-c925-4dbc-8b88-041b6d7f35b3.png">
-            
-            - After the spectrum is generated, a file with the extension .lx will be created. For absorption spectra, the file will be named "cross_section.lx", whereas for fluorescence spectra, the file will be named "differential_rate.lx"
-            - It is possible to generate a spectrum with partially concluded calculations. Option 3 can be used multiple times without overwriting the previously generated spectrum. Each time a spectrum is generated, it will have a number at the beginning of the file name, such as "2cross_section.lx".
-            - Each spectrum file is expected to have three columns as indicated below, where the third column can be used to estimate if the amount of sampled geometries are enough for accurate spectrum simulation.
-            <img width="380" alt="LeoX3" src="https://user-images.githubusercontent.com/94139072/144781496-a7c1e1cc-56ea-4de4-85bd-6a0e7ed37d7e.png">
-        
-        
-        2. For exciton properties:
-        
-            - For exciton properties, you must first calculate the fluorescence and absorption spectra of the donor and acceptor molecules of interest to you. 
-            - Once this is done, copy the spectra to a folder and inside this folder run the `lx` command. Choose option 5. Follow the instructions to set the calculation parameters, exemplified below.  
-            <img width="450" alt="LeoX4" src="https://user-images.githubusercontent.com/94139072/144785795-70dec39b-c63d-41a7-9613-fcf4cd1c244f.png">
-           
-            - The correction for short distances takes into account the transition dipole moment of the donor molecule, extracted directly from the Gaussian log. Details can be obtained in the indicated published paper.
-            - A file called `ld.lx` will be generated with all the information.
-            <img width="450" alt="Captura de Tela 2021-12-06 às 01 13 13" src="https://user-images.githubusercontent.com/94139072/144786165-547a9a2e-cca3-434a-90a7-82c610d97d7e.png">
-        
-        
-            - Importantly, diffusion length estimates are only sensible if donor and acceptor molecules are of the same kind. To calculate the Förster radius for transfers between different molecules, you must provide the fluorescence spectrum of the donor molecule and the absorption spectrum of the acceptor molecule. The fluorescence lifetime shown will correspond to that of the donor molecule.  
-        
-        4. For conformational searches:
-            
-            - Create a folder. Add a frequency Gaussian .log file. Include also a bash script file according to your batch system (follow examples for slurm and task spooler [here](https://github.com/LeonardoESousa/LeoX/tree/master/batch_examples)). 
-            - Run the `lx` command in the folder and choose option 6. Follow the instructions to set the calculation parameters. 
-            - Answer the queries to determine the parameters of the conformational search (level of theory, initial temperature, temperature step, number of rounds, number of sampled geometries at each round). 
-            - Once the search starts running, the file conformation.lx will show the conformations found thus far, along with the average energies and Boltzmann populations at 300 K of each. 
-            - After the search is over, a folder named Conformers is created with the geometries of each conformer written to a gaussian input file that can be used for further optimization. 
-        
-        3. For range separation parameter tuning:
-        
-            - Create a folder. Add either a Gaussian .log file or .com file (for any kind of calculation). Include also a bash script file according to your batch system (follow examples for slurm and task spooler [here](https://github.com/LeonardoESousa/LeoX/tree/master/batch_examples)). 
-            - Run the `lx` command in the folder and choose option 7. Follow the instructions to set the calculation parameters. 
-            - You may choose between a relaxed on unrelaxed tuning procedure. In the case of the former, geometry optimizations are run for each range separation parameter value. In the case of unrelaxed tuning, the geometry provided in the .log or .com file will be used for all calculations. 
-         
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+﻿# LeoX - Light emission and exciton diffusion in organic molecules 
+
+[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
+[![license](https://img.shields.io/github/license/LeonardoESousa/LeoX?style=plastic)]()
+[![down](https://img.shields.io/pypi/dm/LeoX)]()
+[![maint](https://img.shields.io/maintenance/yes/2023)]()
+[![commit](https://img.shields.io/github/last-commit/LeonardoESousa/LeoX?style=plastic)]()
+
+
+
+A package for absorption and fluorescence spectrum simulations using the nuclear ensemble method along with TD(A)-DFT. Estimation of singlet exciton properties (Förster radius, lifetime, diffusion length). Long-range separation parameter tuning. Stochastic conformational search.  Interfaces with the Gaussian (09 or 16) package.
+
+
+Table of Contents
+=================
+<!--ts-->
+* [Cite as:](#cite-as)
+* [What does this program do?](#what-does-this-program-do)
+* [What is necessary to use it?](#what-is-necessary-to-use-it)
+* [How to install it?](#how-to-install-it)
+* [How to use it?](#how-to-use-it)
+   
+<!--te-->
+
+## Cite as:
+
+> de Sousa, L. E., Bueno, F. T., e Silva, G. M., da Silva Filho, D. A., & de Oliveira Neto, P. H. (2019). Fast predictions of exciton diffusion length in organic materials. Journal of Materials Chemistry C, 7(14), 4066-4071.
+
+
+## What does this program do?
+
+1.  Spectrum simulation:
+    - Calculates Absorption and Fluorescence spectrum simulations using TD(A)-DFT.
+    - Calculations include vibrational contributions to the spectra. 
+    - Optionally, they may also include solvent effects either by PCM or by a state specific solvation model.
+2.  Exciton properties:   
+    - Calculates Förster radius for transfers between two molecules of equal or different type.
+    - Calculates fluorescence lifetimes.
+    - Calculates singlet exciton diffusion lengths.
+3.  Extra features:
+    - Tunes the w parameter of long-range separated functionals.
+    - Extracts last geometry from Gaussian log file.
+    - Runs a stochastic coformational search algorithm.
+
+
+## What is necessary to use it?
+
+ -  The program requires that the Gaussian quantum chemistry software (G09 or G16) be installed, as it interfaces with it.
+
+-   The first step for running spectrum calculations or conformational searches is providing a Gaussian log file for a frequency calculation in the S0 state, if the goal is computing an absorption spectrum, or S1 state, if the objective is calculating a fluoresence spectrum. All frequencies must be real.  
+
+-   To obtain estimates for Förster radius, fluorescence lifetimes and singlet exciton diffusion lengths, it is necessary to first perform both absorption and emission spectra calculations for the molecule of interest.
+
+## How to install it?
+
+Run:
+
+`pip install LeoX`
+
+Alternatively, clone the repository to your computer. Inside the LeoX folder, run:
+
+`pip install .`
+
+Depending on the operating system, the commands above may need to be replace by
+
+`pip3 install LeoX` or `pip3 install .`
+
+Once installed, you should be able to run the program from any folder by just using the `lx` command.
+
+## How to use it?
+
+1. For spectrum simulations:
+
+    - Create a folder for your project. Add the log file for the frequency calculation to your folder. Run the lx command. Choose option 1 and follow the instructions to select the parameters of the calculation.
+    - Add a bash script file to the folder to control execution. This file depends on which batch system you use. Examples for users of slurm or task spooler (ts) are presented [here](https://github.com/LeonardoESousa/LeoX/tree/master/batch_examples).
+    - Run the `lx` command again, choose option 2 and follow the instructions. Once the calculations are running, you may use option 4 to check the progress or option 9 to abort.
+    <img width="575" alt="LeoX1" src="https://user-images.githubusercontent.com/94139072/144780278-ef3b8ced-af82-4a9d-a8a5-667ebdcbdd71.png">
+
+    - Once all calculations are done, run the `lx` command and choose option 3. Follow the instructions to set the parameters and the spectrum will be generated.
+    <img width="436" alt="LeoX2" src="https://user-images.githubusercontent.com/94139072/144780487-7d0a5800-c925-4dbc-8b88-041b6d7f35b3.png">
+    
+    - After the spectrum is generated, a file with the extension .lx will be created. For absorption spectra, the file will be named "cross_section.lx", whereas for fluorescence spectra, the file will be named "differential_rate.lx"
+    - It is possible to generate a spectrum with partially concluded calculations. Option 3 can be used multiple times without overwriting the previously generated spectrum. Each time a spectrum is generated, it will have a number at the beginning of the file name, such as "2cross_section.lx".
+    - Each spectrum file is expected to have three columns as indicated below, where the third column can be used to estimate if the amount of sampled geometries are enough for accurate spectrum simulation.
+    <img width="380" alt="LeoX3" src="https://user-images.githubusercontent.com/94139072/144781496-a7c1e1cc-56ea-4de4-85bd-6a0e7ed37d7e.png">
+
+
+2. For exciton properties:
+
+    - For exciton properties, you must first calculate the fluorescence and absorption spectra of the donor and acceptor molecules of interest to you. 
+    - Once this is done, copy the spectra to a folder and inside this folder run the `lx` command. Choose option 5. Follow the instructions to set the calculation parameters, exemplified below.  
+    <img width="450" alt="LeoX4" src="https://user-images.githubusercontent.com/94139072/144785795-70dec39b-c63d-41a7-9613-fcf4cd1c244f.png">
+   
+    - The correction for short distances takes into account the transition dipole moment of the donor molecule, extracted directly from the Gaussian log. Details can be obtained in the indicated published paper.
+    - A file called `ld.lx` will be generated with all the information.
+    <img width="450" alt="Captura de Tela 2021-12-06 às 01 13 13" src="https://user-images.githubusercontent.com/94139072/144786165-547a9a2e-cca3-434a-90a7-82c610d97d7e.png">
+
+
+    - Importantly, diffusion length estimates are only sensible if donor and acceptor molecules are of the same kind. To calculate the Förster radius for transfers between different molecules, you must provide the fluorescence spectrum of the donor molecule and the absorption spectrum of the acceptor molecule. The fluorescence lifetime shown will correspond to that of the donor molecule.  
+
+4. For conformational searches:
+    
+    - Create a folder. Add a frequency Gaussian .log file. Include also a bash script file according to your batch system (follow examples for slurm and task spooler [here](https://github.com/LeonardoESousa/LeoX/tree/master/batch_examples)). 
+    - Run the `lx` command in the folder and choose option 6. Follow the instructions to set the calculation parameters. 
+    - Answer the queries to determine the parameters of the conformational search (level of theory, initial temperature, temperature step, number of rounds, number of sampled geometries at each round). 
+    - Once the search starts running, the file conformation.lx will show the conformations found thus far, along with the average energies and Boltzmann populations at 300 K of each. 
+    - After the search is over, a folder named Conformers is created with the geometries of each conformer written to a gaussian input file that can be used for further optimization. 
+
+3. For range separation parameter tuning:
+
+    - Create a folder. Add either a Gaussian .log file or .com file (for any kind of calculation). Include also a bash script file according to your batch system (follow examples for slurm and task spooler [here](https://github.com/LeonardoESousa/LeoX/tree/master/batch_examples)). 
+    - Run the `lx` command in the folder and choose option 7. Follow the instructions to set the calculation parameters. 
+    - You may choose between a relaxed on unrelaxed tuning procedure. In the case of the former, geometry optimizations are run for each range separation parameter value. In the case of unrelaxed tuning, the geometry provided in the .log or .com file will be used for all calculations. 
+
```

### Comparing `LeoX-0.5.0/PKG-INFO` & `LeoX-0.6.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,130 +1,130 @@
 Metadata-Version: 2.1
 Name: LeoX
-Version: 0.5.0
+Version: 0.6.0
 Summary: Spectrum simulations with TD(A)-DFT
 Home-page: https://github.com/LeonardoESousa/LeoX
 Author: Leonardo Evaristo de Sousa
 Author-email: leonardo.sousa137@gmail.com
 License: MIT
-Description: 
-        ﻿# LeoX - Light emission and exciton diffusion in organic molecules 
-        
-        [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
-        [![license](https://img.shields.io/github/license/LeonardoESousa/LeoX?style=plastic)]()
-        [![down](https://img.shields.io/pypi/dm/LeoX)]()
-        [![maint](https://img.shields.io/maintenance/yes/2021)]()
-        [![commit](https://img.shields.io/github/last-commit/LeonardoESousa/LeoX?style=plastic)]()
-        
-        
-        
-        A package for absorption and fluorescence spectrum simulations using the nuclear ensemble method along with TD(A)-DFT. Estimation of singlet exciton properties (Förster radius, lifetime, diffusion length). Long-range separation parameter tuning. Stochastic conformational search.  Interfaces with the Gaussian (09 or 16) package.
-        
-        
-        Table of Contents
-        =================
-        <!--ts-->
-        * [Cite as:](#cite-as)
-        * [What does this program do?](#what-does-this-program-do)
-        * [What is necessary to use it?](#what-is-necessary-to-use-it)
-        * [How to install it?](#how-to-install-it)
-        * [How to use it?](#how-to-use-it)
-           
-        <!--te-->
-        
-        ## Cite as:
-        
-        > de Sousa, L. E., Bueno, F. T., e Silva, G. M., da Silva Filho, D. A., & de Oliveira Neto, P. H. (2019). Fast predictions of exciton diffusion length in organic materials. Journal of Materials Chemistry C, 7(14), 4066-4071.
-        
-        
-        ## What does this program do?
-        
-        1.  Spectrum simulation:
-            - Calculates Absorption and Fluorescence spectrum simulations using TD(A)-DFT.
-            - Calculations include vibrational contributions to the spectra. 
-            - Optionally, they may also include solvent effects either by PCM or by a state specific solvation model.
-        2.  Exciton properties:   
-            - Calculates Förster radius for transfers between two molecules of equal or different type.
-            - Calculates fluorescence lifetimes.
-            - Calculates singlet exciton diffusion lengths.
-        3.  Extra features:
-            - Tunes the w parameter of long-range separated functionals.
-            - Extracts last geometry from Gaussian log file.
-            - Runs a stochastic coformational search algorithm.
-        
-        
-        ## What is necessary to use it?
-        
-         -  The program requires that the Gaussian quantum chemistry software (G09 or G16) be installed, as it interfaces with it.
-        
-        -   The first step for running spectrum calculations or conformational searches is providing a Gaussian log file for a frequency calculation in the S0 state, if the goal is computing an absorption spectrum, or S1 state, if the objective is calculating a fluoresence spectrum. All frequencies must be real.  
-        
-        -   To obtain estimates for Förster radius, fluorescence lifetimes and singlet exciton diffusion lengths, it is necessary to first perform both absorption and emission spectra calculations for the molecule of interest.
-        
-        ## How to install it?
-        
-        Run:
-        
-        `pip install LeoX`
-        
-        Alternatively, clone the repository to your computer. Inside the LeoX folder, run:
-        
-        `pip install .`
-        
-        Depending on the operating system, the commands above may need to be replace by
-        
-        `pip3 install LeoX` or `pip3 install .`
-        
-        Once installed, you should be able to run the program from any folder by just using the `lx` command.
-        
-        ## How to use it?
-        
-        1. For spectrum simulations:
-        
-            - Create a folder for your project. Add the log file for the frequency calculation to your folder. Run the lx command. Choose option 1 and follow the instructions to select the parameters of the calculation.
-            - Add a bash script file to the folder to control execution. This file depends on which batch system you use. Examples for users of slurm or task spooler (ts) are presented [here](https://github.com/LeonardoESousa/LeoX/tree/master/batch_examples).
-            - Run the `lx` command again, choose option 2 and follow the instructions. Once the calculations are running, you may use option 4 to check the progress or option 9 to abort.
-            <img width="575" alt="LeoX1" src="https://user-images.githubusercontent.com/94139072/144780278-ef3b8ced-af82-4a9d-a8a5-667ebdcbdd71.png">
-        
-            - Once all calculations are done, run the `lx` command and choose option 3. Follow the instructions to set the parameters and the spectrum will be generated.
-            <img width="436" alt="LeoX2" src="https://user-images.githubusercontent.com/94139072/144780487-7d0a5800-c925-4dbc-8b88-041b6d7f35b3.png">
-            
-            - After the spectrum is generated, a file with the extension .lx will be created. For absorption spectra, the file will be named "cross_section.lx", whereas for fluorescence spectra, the file will be named "differential_rate.lx"
-            - It is possible to generate a spectrum with partially concluded calculations. Option 3 can be used multiple times without overwriting the previously generated spectrum. Each time a spectrum is generated, it will have a number at the beginning of the file name, such as "2cross_section.lx".
-            - Each spectrum file is expected to have three columns as indicated below, where the third column can be used to estimate if the amount of sampled geometries are enough for accurate spectrum simulation.
-            <img width="380" alt="LeoX3" src="https://user-images.githubusercontent.com/94139072/144781496-a7c1e1cc-56ea-4de4-85bd-6a0e7ed37d7e.png">
-        
-        
-        2. For exciton properties:
-        
-            - For exciton properties, you must first calculate the fluorescence and absorption spectra of the donor and acceptor molecules of interest to you. 
-            - Once this is done, copy the spectra to a folder and inside this folder run the `lx` command. Choose option 5. Follow the instructions to set the calculation parameters, exemplified below.  
-            <img width="450" alt="LeoX4" src="https://user-images.githubusercontent.com/94139072/144785795-70dec39b-c63d-41a7-9613-fcf4cd1c244f.png">
-           
-            - The correction for short distances takes into account the transition dipole moment of the donor molecule, extracted directly from the Gaussian log. Details can be obtained in the indicated published paper.
-            - A file called `ld.lx` will be generated with all the information.
-            <img width="450" alt="Captura de Tela 2021-12-06 às 01 13 13" src="https://user-images.githubusercontent.com/94139072/144786165-547a9a2e-cca3-434a-90a7-82c610d97d7e.png">
-        
-        
-            - Importantly, diffusion length estimates are only sensible if donor and acceptor molecules are of the same kind. To calculate the Förster radius for transfers between different molecules, you must provide the fluorescence spectrum of the donor molecule and the absorption spectrum of the acceptor molecule. The fluorescence lifetime shown will correspond to that of the donor molecule.  
-        
-        4. For conformational searches:
-            
-            - Create a folder. Add a frequency Gaussian .log file. Include also a bash script file according to your batch system (follow examples for slurm and task spooler [here](https://github.com/LeonardoESousa/LeoX/tree/master/batch_examples)). 
-            - Run the `lx` command in the folder and choose option 6. Follow the instructions to set the calculation parameters. 
-            - Answer the queries to determine the parameters of the conformational search (level of theory, initial temperature, temperature step, number of rounds, number of sampled geometries at each round). 
-            - Once the search starts running, the file conformation.lx will show the conformations found thus far, along with the average energies and Boltzmann populations at 300 K of each. 
-            - After the search is over, a folder named Conformers is created with the geometries of each conformer written to a gaussian input file that can be used for further optimization. 
-        
-        3. For range separation parameter tuning:
-        
-            - Create a folder. Add either a Gaussian .log file or .com file (for any kind of calculation). Include also a bash script file according to your batch system (follow examples for slurm and task spooler [here](https://github.com/LeonardoESousa/LeoX/tree/master/batch_examples)). 
-            - Run the `lx` command in the folder and choose option 7. Follow the instructions to set the calculation parameters. 
-            - You may choose between a relaxed on unrelaxed tuning procedure. In the case of the former, geometry optimizations are run for each range separation parameter value. In the case of unrelaxed tuning, the geometry provided in the .log or .com file will be used for all calculations. 
-         
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+﻿# LeoX - Light emission and exciton diffusion in organic molecules 
+
+[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
+[![license](https://img.shields.io/github/license/LeonardoESousa/LeoX?style=plastic)]()
+[![down](https://img.shields.io/pypi/dm/LeoX)]()
+[![maint](https://img.shields.io/maintenance/yes/2023)]()
+[![commit](https://img.shields.io/github/last-commit/LeonardoESousa/LeoX?style=plastic)]()
+
+
+
+A package for absorption and fluorescence spectrum simulations using the nuclear ensemble method along with TD(A)-DFT. Estimation of singlet exciton properties (Förster radius, lifetime, diffusion length). Long-range separation parameter tuning. Stochastic conformational search.  Interfaces with the Gaussian (09 or 16) package.
+
+
+Table of Contents
+=================
+<!--ts-->
+* [Cite as:](#cite-as)
+* [What does this program do?](#what-does-this-program-do)
+* [What is necessary to use it?](#what-is-necessary-to-use-it)
+* [How to install it?](#how-to-install-it)
+* [How to use it?](#how-to-use-it)
+   
+<!--te-->
+
+## Cite as:
+
+> de Sousa, L. E., Bueno, F. T., e Silva, G. M., da Silva Filho, D. A., & de Oliveira Neto, P. H. (2019). Fast predictions of exciton diffusion length in organic materials. Journal of Materials Chemistry C, 7(14), 4066-4071.
+
+
+## What does this program do?
+
+1.  Spectrum simulation:
+    - Calculates Absorption and Fluorescence spectrum simulations using TD(A)-DFT.
+    - Calculations include vibrational contributions to the spectra. 
+    - Optionally, they may also include solvent effects either by PCM or by a state specific solvation model.
+2.  Exciton properties:   
+    - Calculates Förster radius for transfers between two molecules of equal or different type.
+    - Calculates fluorescence lifetimes.
+    - Calculates singlet exciton diffusion lengths.
+3.  Extra features:
+    - Tunes the w parameter of long-range separated functionals.
+    - Extracts last geometry from Gaussian log file.
+    - Runs a stochastic coformational search algorithm.
+
+
+## What is necessary to use it?
+
+ -  The program requires that the Gaussian quantum chemistry software (G09 or G16) be installed, as it interfaces with it.
+
+-   The first step for running spectrum calculations or conformational searches is providing a Gaussian log file for a frequency calculation in the S0 state, if the goal is computing an absorption spectrum, or S1 state, if the objective is calculating a fluoresence spectrum. All frequencies must be real.  
+
+-   To obtain estimates for Förster radius, fluorescence lifetimes and singlet exciton diffusion lengths, it is necessary to first perform both absorption and emission spectra calculations for the molecule of interest.
+
+## How to install it?
+
+Run:
+
+`pip install LeoX`
+
+Alternatively, clone the repository to your computer. Inside the LeoX folder, run:
+
+`pip install .`
+
+Depending on the operating system, the commands above may need to be replace by
+
+`pip3 install LeoX` or `pip3 install .`
+
+Once installed, you should be able to run the program from any folder by just using the `lx` command.
+
+## How to use it?
+
+1. For spectrum simulations:
+
+    - Create a folder for your project. Add the log file for the frequency calculation to your folder. Run the lx command. Choose option 1 and follow the instructions to select the parameters of the calculation.
+    - Add a bash script file to the folder to control execution. This file depends on which batch system you use. Examples for users of slurm or task spooler (ts) are presented [here](https://github.com/LeonardoESousa/LeoX/tree/master/batch_examples).
+    - Run the `lx` command again, choose option 2 and follow the instructions. Once the calculations are running, you may use option 4 to check the progress or option 9 to abort.
+    <img width="575" alt="LeoX1" src="https://user-images.githubusercontent.com/94139072/144780278-ef3b8ced-af82-4a9d-a8a5-667ebdcbdd71.png">
+
+    - Once all calculations are done, run the `lx` command and choose option 3. Follow the instructions to set the parameters and the spectrum will be generated.
+    <img width="436" alt="LeoX2" src="https://user-images.githubusercontent.com/94139072/144780487-7d0a5800-c925-4dbc-8b88-041b6d7f35b3.png">
+    
+    - After the spectrum is generated, a file with the extension .lx will be created. For absorption spectra, the file will be named "cross_section.lx", whereas for fluorescence spectra, the file will be named "differential_rate.lx"
+    - It is possible to generate a spectrum with partially concluded calculations. Option 3 can be used multiple times without overwriting the previously generated spectrum. Each time a spectrum is generated, it will have a number at the beginning of the file name, such as "2cross_section.lx".
+    - Each spectrum file is expected to have three columns as indicated below, where the third column can be used to estimate if the amount of sampled geometries are enough for accurate spectrum simulation.
+    <img width="380" alt="LeoX3" src="https://user-images.githubusercontent.com/94139072/144781496-a7c1e1cc-56ea-4de4-85bd-6a0e7ed37d7e.png">
+
+
+2. For exciton properties:
+
+    - For exciton properties, you must first calculate the fluorescence and absorption spectra of the donor and acceptor molecules of interest to you. 
+    - Once this is done, copy the spectra to a folder and inside this folder run the `lx` command. Choose option 5. Follow the instructions to set the calculation parameters, exemplified below.  
+    <img width="450" alt="LeoX4" src="https://user-images.githubusercontent.com/94139072/144785795-70dec39b-c63d-41a7-9613-fcf4cd1c244f.png">
+   
+    - The correction for short distances takes into account the transition dipole moment of the donor molecule, extracted directly from the Gaussian log. Details can be obtained in the indicated published paper.
+    - A file called `ld.lx` will be generated with all the information.
+    <img width="450" alt="Captura de Tela 2021-12-06 às 01 13 13" src="https://user-images.githubusercontent.com/94139072/144786165-547a9a2e-cca3-434a-90a7-82c610d97d7e.png">
+
+
+    - Importantly, diffusion length estimates are only sensible if donor and acceptor molecules are of the same kind. To calculate the Förster radius for transfers between different molecules, you must provide the fluorescence spectrum of the donor molecule and the absorption spectrum of the acceptor molecule. The fluorescence lifetime shown will correspond to that of the donor molecule.  
+
+4. For conformational searches:
+    
+    - Create a folder. Add a frequency Gaussian .log file. Include also a bash script file according to your batch system (follow examples for slurm and task spooler [here](https://github.com/LeonardoESousa/LeoX/tree/master/batch_examples)). 
+    - Run the `lx` command in the folder and choose option 6. Follow the instructions to set the calculation parameters. 
+    - Answer the queries to determine the parameters of the conformational search (level of theory, initial temperature, temperature step, number of rounds, number of sampled geometries at each round). 
+    - Once the search starts running, the file conformation.lx will show the conformations found thus far, along with the average energies and Boltzmann populations at 300 K of each. 
+    - After the search is over, a folder named Conformers is created with the geometries of each conformer written to a gaussian input file that can be used for further optimization. 
+
+3. For range separation parameter tuning:
+
+    - Create a folder. Add either a Gaussian .log file or .com file (for any kind of calculation). Include also a bash script file according to your batch system (follow examples for slurm and task spooler [here](https://github.com/LeonardoESousa/LeoX/tree/master/batch_examples)). 
+    - Run the `lx` command in the folder and choose option 7. Follow the instructions to set the calculation parameters. 
+    - You may choose between a relaxed on unrelaxed tuning procedure. In the case of the former, geometry optimizations are run for each range separation parameter value. In the case of unrelaxed tuning, the geometry provided in the .log or .com file will be used for all calculations. 
+
```

### Comparing `LeoX-0.5.0/README.md` & `LeoX-0.6.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ﻿# LeoX - Light emission and exciton diffusion in organic molecules 
 
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
 [![license](https://img.shields.io/github/license/LeonardoESousa/LeoX?style=plastic)]()
 [![down](https://img.shields.io/pypi/dm/LeoX)]()
-[![maint](https://img.shields.io/maintenance/yes/2021)]()
+[![maint](https://img.shields.io/maintenance/yes/2023)]()
 [![commit](https://img.shields.io/github/last-commit/LeonardoESousa/LeoX?style=plastic)]()
 
 
 
 A package for absorption and fluorescence spectrum simulations using the nuclear ensemble method along with TD(A)-DFT. Estimation of singlet exciton properties (Förster radius, lifetime, diffusion length). Long-range separation parameter tuning. Stochastic conformational search.  Interfaces with the Gaussian (09 or 16) package.
```

### Comparing `LeoX-0.5.0/lx/__main__.py` & `LeoX-0.6.0/lx/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,17 +18,18 @@
     print("\t3 - Generate the spectrum")
     print("\t4 - Check the progress of the calculations")
     print('EXCITON ANALYSIS:')
     print("\t5 - Estimate Förster radius, fluorescence lifetime and exciton diffusion lengths")
     print('CONFORMATIONAL ANALYSIS:')
     print("\t6 - Perform conformational search")
     print('OTHER FEATURES:')
-    print("\t7 - Perform long-range parameter tuning") 
-    print("\t8 - Retrieve last geometry from log file") 
-    print("\t9 - Abort my calculations")
+    print("\t7 - Perform long-range parameter tuning")
+    print("\t8 - Get rid of imaginary frequencies")  
+    print("\t9 - Retrieve last geometry from log file") 
+    print("\t10 - Abort my calculations")
     op = input()
     if op == '1':
         freqlog = lx.tools.fetch_file("frequency",['.log'])
         F, _  = lx.tools.pega_freq(freqlog)
         if F[0] < 0:
             lx.tools.fatal_error("Imaginary frequency! Goodbye!")
         cm = lx.tools.get_cm(freqlog)
@@ -130,22 +131,25 @@
     elif op == '5':
         lx.tools.ld()
     elif op == '6':
         lx.tools.conformational()
     elif op == '7':
         lx.tools.omega_tuning()
     elif op == '8':
+        freqlog = lx.tools.fetch_file("Frequency log with imaginary frequencies",['.log'])
+        lx.tools.distort(freqlog)    
+    elif op == '9':
         freqlog = lx.tools.fetch_file("log",['.log'])
         base, _, nproc, mem, scrf, _ = lx.tools.busca_input(freqlog)
         cm = lx.tools.get_cm(freqlog)
         header = '%nproc={}\n%mem={}\n# {} {}\n\nTITLE\n\n{}\n'.format(nproc,mem,base,scrf,cm)
         G, atomos = lx.tools.pega_geom(freqlog)
         lx.tools.write_input(atomos,G,header,'','geom.lx')
         print('Geometry saved in the geom.lx file.')    
-    elif op == '9':
+    elif op == '10':
         lx.tools.abort_batch()
     else:
         lx.tools.fatal_error("It must be one of the options... Goodbye!")
 
 def main():
     try:
         freqlog = sys.argv[1]
```

### Comparing `LeoX-0.5.0/lx/batch_lx.py` & `LeoX-0.6.0/lx/batch_lx.py`

 * *Files identical despite different names*

### Comparing `LeoX-0.5.0/lx/conf_search.py` & `LeoX-0.6.0/lx/conf_search.py`

 * *Files identical despite different names*

### Comparing `LeoX-0.5.0/lx/ld.py` & `LeoX-0.6.0/lx/ld.py`

 * *Files identical despite different names*

### Comparing `LeoX-0.5.0/lx/omega.py` & `LeoX-0.6.0/lx/omega.py`

 * *Files identical despite different names*

### Comparing `LeoX-0.5.0/lx/tools.py` & `LeoX-0.6.0/lx/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,17 +211,54 @@
 ##CHECKS FOR EXISTING GEOMETRIES###############################
 def start_counter():
     files = [file for file in os.listdir('Geometries') if ".com" in file and "Geometr" in file]
     return len(files)
 ###############################################################
 
 ##SAMPLES GEOMETRIES###########################################
-def sample_geometries(freqlog,num_geoms,T, limit=np.inf):
+def distort(freqlog):
+    num_geoms = 1
+    T = 300
     G, atomos = pega_geom(freqlog)
     F, M      = pega_freq(freqlog)
+    NNC       = pega_modos(G,freqlog)
+    num_atom  = np.shape(G)[0]
+    A = np.zeros((3*num_atom,num_geoms))
+    # check for imaginary frequencies
+    if np.all(F > 0):
+        fatal_error("No imaginary frequencies found. Exiting...")
+    for i in range(0,len(F)):
+        if F[i] < 0:
+            f = -1*F[i]
+            q = 3*np.sqrt(hbar2/(2*M[i]*f*np.tanh(hbar*f/(2*kb*T))))
+            q = np.array(q)
+            A += np.outer(NNC[:,i],q)
+    for n in range(np.shape(A)[1]):
+        A1 = np.reshape(A[:,n],(num_atom,3))
+        try:
+            Gfinal = np.hstack((Gfinal,A1 + G))
+        except:
+            Gfinal = A1 + G
+    base, _, nproc, mem, scrf, spec = busca_input(freqlog)
+    cm = get_cm(freqlog)
+    header = "%nproc={}\n%mem={}\n# {} opt freq=noraman\n\nDISTORTED GEOM\n\n{}\n".format(nproc,mem,base,cm)
+    bottom = '\n'
+    for n in range(0,np.shape(A)[1],3):
+        Gfinal = Gfinal[:,n:n+3]
+        write_input(atomos,Gfinal,header,bottom,"distorted.com")
+    print("New input file written to distorted.com")    
+###############################################################
+
+##SAMPLES GEOMETRIES###########################################
+def sample_geometries(freqlog,num_geoms,T, limit=np.inf, warning=True):
+    G, atomos = pega_geom(freqlog)
+    F, M      = pega_freq(freqlog)
+    # check for negative frequencies
+    if warning and np.any(F < 0):
+        fatal_error("Negative frequencies detected. Check your frequency file. Goodbye.")
     F[F < 0] *= -1
     NNC       = pega_modos(G,freqlog)
     mask = F < limit*(c*100*2*pi)
     F = F[mask]
     NNC = NNC[:,mask]
     num_atom  = np.shape(G)[0]
     A = np.zeros((3*num_atom,num_geoms))
```

### Comparing `LeoX-0.5.0/setup.py` & `LeoX-0.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'LeoX'
 DESCRIPTION = 'Spectrum simulations with TD(A)-DFT'
 URL = 'https://github.com/LeonardoESousa/LeoX'
 EMAIL = 'leonardo.sousa137@gmail.com'
 AUTHOR = 'Leonardo Evaristo de Sousa'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.5.0'
+VERSION = '0.6.0'
 
 # What packages are required for this module to be executed?
 REQUIRED = ['numpy', 'scipy', 'pandas']
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
```

