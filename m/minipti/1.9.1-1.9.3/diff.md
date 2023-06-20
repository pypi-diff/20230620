# Comparing `tmp/minipti-1.9.1.tar.gz` & `tmp/minipti-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minipti-1.9.1.tar", last modified: Thu May 11 14:50:41 2023, max compression
+gzip compressed data, was "minipti-1.9.3.tar", last modified: Tue Jun 20 13:03:51 2023, max compression
```

## Comparing `minipti-1.9.1.tar` & `minipti-1.9.3.tar`

### file list

```diff
@@ -1,32 +1,31 @@
-drwxrwxr-x   0 jonas     (1000) jonas     (1000)        0 2023-05-11 14:50:41.626368 minipti-1.9.1/
--rw-rw-r--   0 jonas     (1000) jonas     (1000)     1061 2023-05-11 09:17:20.000000 minipti-1.9.1/LICENSE
--rw-rw-r--   0 jonas     (1000) jonas     (1000)     5153 2023-05-11 14:50:41.626368 minipti-1.9.1/PKG-INFO
--rw-rw-r--   0 jonas     (1000) jonas     (1000)     4396 2023-05-11 14:48:18.000000 minipti-1.9.1/README.md
--rw-rw-r--   0 jonas     (1000) jonas     (1000)      998 2023-05-11 14:50:32.000000 minipti-1.9.1/pyproject.toml
--rw-rw-r--   0 jonas     (1000) jonas     (1000)       38 2023-05-11 14:50:41.626368 minipti-1.9.1/setup.cfg
-drwxrwxr-x   0 jonas     (1000) jonas     (1000)        0 2023-05-11 14:50:41.626368 minipti-1.9.1/src/
-drwxrwxr-x   0 jonas     (1000) jonas     (1000)        0 2023-05-11 14:50:41.626368 minipti-1.9.1/src/minipti/
--rw-rw-r--   0 jonas     (1000) jonas     (1000)      239 2023-05-10 09:18:55.000000 minipti-1.9.1/src/minipti/__init__.py
--rw-rw-r--   0 jonas     (1000) jonas     (1000)      399 2023-05-08 17:02:55.000000 minipti-1.9.1/src/minipti/__main__.py
-drwxrwxr-x   0 jonas     (1000) jonas     (1000)        0 2023-05-11 14:50:41.626368 minipti-1.9.1/src/minipti/algorithm/
--rw-rw-r--   0 jonas     (1000) jonas     (1000)       93 2023-05-09 16:58:29.000000 minipti-1.9.1/src/minipti/algorithm/__init__.py
--rw-rw-r--   0 jonas     (1000) jonas     (1000)    17825 2023-05-11 12:27:16.000000 minipti-1.9.1/src/minipti/algorithm/interferometry.py
--rw-rw-r--   0 jonas     (1000) jonas     (1000)    13828 2023-05-11 13:36:17.000000 minipti-1.9.1/src/minipti/algorithm/pti.py
-drwxrwxr-x   0 jonas     (1000) jonas     (1000)        0 2023-05-11 14:50:41.626368 minipti-1.9.1/src/minipti/gui/
--rw-rw-r--   0 jonas     (1000) jonas     (1000)       64 2023-05-04 07:02:16.000000 minipti-1.9.1/src/minipti/gui/__init__.py
--rw-rw-r--   0 jonas     (1000) jonas     (1000)    18829 2023-05-11 06:42:56.000000 minipti-1.9.1/src/minipti/gui/controller.py
--rw-rw-r--   0 jonas     (1000) jonas     (1000)    42380 2023-05-11 13:41:38.000000 minipti-1.9.1/src/minipti/gui/model.py
--rw-rw-r--   0 jonas     (1000) jonas     (1000)    50562 2023-05-11 13:50:55.000000 minipti-1.9.1/src/minipti/gui/view.py
-drwxrwxr-x   0 jonas     (1000) jonas     (1000)        0 2023-05-11 14:50:41.626368 minipti-1.9.1/src/minipti/hardware/
--rw-rw-r--   0 jonas     (1000) jonas     (1000)       92 2023-05-04 07:02:16.000000 minipti-1.9.1/src/minipti/hardware/__init__.py
--rw-rw-r--   0 jonas     (1000) jonas     (1000)     9105 2023-05-09 16:58:29.000000 minipti-1.9.1/src/minipti/hardware/laser.py
--rw-rw-r--   0 jonas     (1000) jonas     (1000)    15129 2023-05-11 09:08:15.000000 minipti-1.9.1/src/minipti/hardware/motherboard.py
--rw-rw-r--   0 jonas     (1000) jonas     (1000)    10783 2023-05-10 10:15:43.000000 minipti-1.9.1/src/minipti/hardware/serial_device.py
--rw-rw-r--   0 jonas     (1000) jonas     (1000)     9682 2023-05-10 09:59:50.000000 minipti-1.9.1/src/minipti/hardware/tec.py
--rw-rw-r--   0 jonas     (1000) jonas     (1000)     1628 2023-05-04 07:02:16.000000 minipti-1.9.1/src/minipti/json_parser.py
-drwxrwxr-x   0 jonas     (1000) jonas     (1000)        0 2023-05-11 14:50:41.626368 minipti-1.9.1/src/minipti.egg-info/
--rw-rw-r--   0 jonas     (1000) jonas     (1000)     5153 2023-05-11 14:50:41.000000 minipti-1.9.1/src/minipti.egg-info/PKG-INFO
--rw-rw-r--   0 jonas     (1000) jonas     (1000)      656 2023-05-11 14:50:41.000000 minipti-1.9.1/src/minipti.egg-info/SOURCES.txt
--rw-rw-r--   0 jonas     (1000) jonas     (1000)        1 2023-05-11 14:50:41.000000 minipti-1.9.1/src/minipti.egg-info/dependency_links.txt
--rw-rw-r--   0 jonas     (1000) jonas     (1000)      129 2023-05-11 14:50:41.000000 minipti-1.9.1/src/minipti.egg-info/requires.txt
--rw-rw-r--   0 jonas     (1000) jonas     (1000)        8 2023-05-11 14:50:41.000000 minipti-1.9.1/src/minipti.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 13:03:51.706331 minipti-1.9.3/
+-rw-rw-rw-   0        0        0     1082 2023-06-13 15:11:03.000000 minipti-1.9.3/LICENSE
+-rw-rw-rw-   0        0        0     5277 2023-06-20 13:03:51.704333 minipti-1.9.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4503 2023-06-13 15:11:03.000000 minipti-1.9.3/README.md
+-rw-rw-rw-   0        0        0     1042 2023-06-20 13:03:21.000000 minipti-1.9.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-20 13:03:51.706331 minipti-1.9.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-20 13:03:51.656043 minipti-1.9.3/src/
+-rw-rw-rw-   0        0        0      264 2023-06-13 15:11:03.000000 minipti-1.9.3/src/__init__.py
+-rw-rw-rw-   0        0        0      478 2023-06-20 09:21:49.000000 minipti-1.9.3/src/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 13:03:51.665471 minipti-1.9.3/src/algorithm/
+-rw-rw-rw-   0        0        0      113 2023-06-13 15:11:03.000000 minipti-1.9.3/src/algorithm/__init__.py
+-rw-rw-rw-   0        0        0    18237 2023-06-20 12:58:31.000000 minipti-1.9.3/src/algorithm/interferometry.py
+-rw-rw-rw-   0        0        0    14330 2023-06-19 10:02:24.000000 minipti-1.9.3/src/algorithm/pti.py
+drwxrwxrwx   0        0        0        0 2023-06-20 13:03:51.674575 minipti-1.9.3/src/gui/
+-rw-rw-rw-   0        0        0       67 2023-06-13 15:11:03.000000 minipti-1.9.3/src/gui/__init__.py
+-rw-rw-rw-   0        0        0    23199 2023-06-19 10:02:24.000000 minipti-1.9.3/src/gui/controller.py
+-rw-rw-rw-   0        0        0    49115 2023-06-19 10:02:24.000000 minipti-1.9.3/src/gui/model.py
+-rw-rw-rw-   0        0        0    53546 2023-06-20 12:53:06.000000 minipti-1.9.3/src/gui/view.py
+drwxrwxrwx   0        0        0        0 2023-06-20 13:03:51.688335 minipti-1.9.3/src/hardware/
+-rw-rw-rw-   0        0        0       96 2023-06-13 15:11:03.000000 minipti-1.9.3/src/hardware/__init__.py
+-rw-rw-rw-   0        0        0    10952 2023-06-20 12:58:31.000000 minipti-1.9.3/src/hardware/laser.py
+-rw-rw-rw-   0        0        0    16266 2023-06-20 12:58:31.000000 minipti-1.9.3/src/hardware/motherboard.py
+-rw-rw-rw-   0        0        0    15155 2023-06-20 12:58:31.000000 minipti-1.9.3/src/hardware/serial_device.py
+-rw-rw-rw-   0        0        0    12687 2023-06-20 12:58:31.000000 minipti-1.9.3/src/hardware/tec.py
+-rw-rw-rw-   0        0        0     1676 2023-06-13 15:11:03.000000 minipti-1.9.3/src/json_parser.py
+drwxrwxrwx   0        0        0        0 2023-06-20 13:03:51.702333 minipti-1.9.3/src/minipti.egg-info/
+-rw-rw-rw-   0        0        0     5277 2023-06-20 13:03:51.000000 minipti-1.9.3/src/minipti.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      536 2023-06-20 13:03:51.000000 minipti-1.9.3/src/minipti.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 13:03:51.000000 minipti-1.9.3/src/minipti.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      129 2023-06-20 13:03:51.000000 minipti-1.9.3/src/minipti.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       53 2023-06-20 13:03:51.000000 minipti-1.9.3/src/minipti.egg-info/top_level.txt
```

### Comparing `minipti-1.9.1/LICENSE` & `minipti-1.9.3/LICENSE`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 FHNW
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 FHNW
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `minipti-1.9.1/PKG-INFO` & `minipti-1.9.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,124 +1,124 @@
-Metadata-Version: 2.1
-Name: minipti
-Version: 1.9.1
-Summary: Provides algorithm and GUI for photo thermal interferometry and 3x3 couplers
-Author-email: Jonas Bilal <jonasbilal@outlook.com>
-Project-URL: Homepage, https://www.fhnw.ch/en/about-fhnw/schools/school-of-engineering/institutes/institute-for-sensors-and-electronics/aerosol-measurement-technology
-Project-URL: Source, https://github.com/bilaljo/MiniPTI
-Project-URL: Bug Tracker, https://github.com/bilaljo/MiniPTI/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: algorithm
-Provides-Extra: gui
-License-File: LICENSE
-
-# MiniPTI
-
-<p style="text-align: center;">
-<img alt="flowchart" src="https://www.fhnw.ch/de/medien/logos/media/fhnw_e_10mm.jpg" class="centre">
-</p>
-
-In this repository a GUI is provided to control the MiniPTI as also presented in [Waveguide based passively demodulated photothermal interferometer for light absorption measurements of trace substances](https://doi.org/10.1364/AO.476868). In addition to the GUI, Python implementations of the presented algorithms and the driver software for the MiniPTI hardware are also provided as libraries.
-
-# 1. installation
-In order to make the library light-weighted different installation options exist.
-
-To install only the interferometry library you can install it with
-```
-pip install minipti
-```
-To additionally use the inversion algorithm you can type
-```bash
-pip install minipti[algorithm]
-```
-To install the entire package (GUI, algorithms and hardware drivers) you can type
-```bash
-pip install minipti[gui]
-```
-# 2. Usage and GUI
-The GUI can be used via
-```bash
-python -m minipti
-```
-
-## 2.1 Home Tab
-<p style="text-align: center;">
-<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/home.png">
-</p>
-
-## 2.2 Pump Laser Tab
-### 2.2.1 Pump Laser Driver Tab
-<p style="text-align: center;">
-<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/pump_laser_tab.png">
-</p>
-
-### 2.2.2 Pump Laser Tec Driver Tab
-<p style="text-align: center;">
-<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/pump_tec.png">
-</p>
-
-## 2.3 Probe Laser Tab
-### 2.3.1 Probe Laser Driver Tab
-<p style="text-align: center;">
-<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/probe_laser_tab.png">
-</p>
-
-### 2.3.1 Probe Laser Tec Driver Tab
-<p style="text-align: center;">
-<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/probe_tec.png">
-</p>
-
-## 2.3 Plotting Tabs
-### 2.3.1 DC Signals
-<p style="text-align: center;">
-<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/dc_tab.png">
-</p>
-
-### 2.3.2 Amplitudes
-<p style="text-align: center;">
-<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/amplitudes_tab.png">
-</p>
-
-### 2.3.3 Output Phases
-<p style="text-align: center;">
-<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/output_phases_tab.png">
-</p>
-
-### 2.3.4 Interferometric Phase
-<p style="text-align: center;">
-<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/phase_tab.png">
-</p>
-
-### 2.3.5 Sensitivity
-<p style="text-align: center;">
-<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/sensitivity_tab.png">
-</p>
-
-### 2.3.6 Symmetry
-<p style="text-align: center;">
-<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/sym_tab.png">
-</p>
-
-### 2.3.7 PTI Signal
-<p style="text-align: center;">
-<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/pti_signal_tab.png">
-</p>
-
-# 3. libraries
-
-## 3.1 Algorithm
-The subpackage Algorithm contains the implementation of the algorithms and can be divided into the subpackages interferometry and pti. interferometry contains the algorithms for the interferometric phase and characterisation of the interferometer. pti contains the algorithms for decimation and PTI inversion.
-
-It is also possible to use only the interferometer subpackage without having to install dependencies for the other packages.
-
-### 3.1.1 Interferometry
-interferometry contains the classes interferometer and characterisation.
-Examples of usage can be found under <a href="https://github.com/bilaljo/MiniPTI/blob/main/examples/interferometry.py">examples/interferometer.py</a> and
-<a href="https://github.com/bilaljo/MiniPTI/blob/main/examples/characterisation.py">examples/characterisation.py</a>.
-### 3.1.2 PTI
-pti contains the classes decimation inversion. Example calls can be found under <a href="https://github.com/bilaljo/MiniPTI/blob/main/examples/pti_inversion.py">examples/pti_inversion.py</a>
-## 3.2 Hardware
-Hardware contains the classes to control the motherboard (DAQ + BMS), laser (Probe and Pump Laser) and TEC driver as well as the valve control.
+Metadata-Version: 2.1
+Name: minipti
+Version: 1.9.3
+Summary: Provides algorithm and GUI for photo thermal interferometry and 3x3 couplers
+Author-email: Jonas Bilal <jonasbilal@outlook.com>
+Project-URL: Homepage, https://www.fhnw.ch/en/about-fhnw/schools/school-of-engineering/institutes/institute-for-sensors-and-electronics/aerosol-measurement-technology
+Project-URL: Source, https://github.com/bilaljo/MiniPTI
+Project-URL: Bug Tracker, https://github.com/bilaljo/MiniPTI/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: algorithm
+Provides-Extra: gui
+License-File: LICENSE
+
+# MiniPTI
+
+<p style="text-align: center;">
+<img alt="flowchart" src="https://www.fhnw.ch/de/medien/logos/media/fhnw_e_10mm.jpg" class="centre">
+</p>
+
+In this repository a GUI is provided to control the MiniPTI as also presented in [Waveguide based passively demodulated photothermal interferometer for light absorption measurements of trace substances](https://doi.org/10.1364/AO.476868). In addition to the GUI, Python implementations of the presented algorithms and the driver software for the MiniPTI hardware are also provided as libraries.
+
+# 1. installation
+In order to make the library light-weighted different installation options exist.
+
+To install only the interferometry library you can install it with
+```
+pip install minipti
+```
+To additionally use the inversion algorithm you can type
+```bash
+pip install minipti[algorithm]
+```
+To install the entire package (GUI, algorithms and hardware drivers) you can type
+```bash
+pip install minipti[gui]
+```
+# 2. Usage and GUI
+The GUI can be used via
+```bash
+python -m minipti
+```
+
+## 2.1 Home Tab
+<p style="text-align: center;">
+<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/home.png">
+</p>
+
+## 2.2 Pump Laser Tab
+### 2.2.1 Pump Laser Driver Tab
+<p style="text-align: center;">
+<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/pump_laser_tab.png">
+</p>
+
+### 2.2.2 Pump Laser Tec Driver Tab
+<p style="text-align: center;">
+<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/pump_tec.png">
+</p>
+
+## 2.3 Probe Laser Tab
+### 2.3.1 Probe Laser Driver Tab
+<p style="text-align: center;">
+<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/probe_laser_tab.png">
+</p>
+
+### 2.3.1 Probe Laser Tec Driver Tab
+<p style="text-align: center;">
+<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/probe_tec.png">
+</p>
+
+## 2.3 Plotting Tabs
+### 2.3.1 DC Signals
+<p style="text-align: center;">
+<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/dc_tab.png">
+</p>
+
+### 2.3.2 Amplitudes
+<p style="text-align: center;">
+<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/amplitudes_tab.png">
+</p>
+
+### 2.3.3 Output Phases
+<p style="text-align: center;">
+<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/output_phases_tab.png">
+</p>
+
+### 2.3.4 Interferometric Phase
+<p style="text-align: center;">
+<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/phase_tab.png">
+</p>
+
+### 2.3.5 Sensitivity
+<p style="text-align: center;">
+<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/sensitivity_tab.png">
+</p>
+
+### 2.3.6 Symmetry
+<p style="text-align: center;">
+<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/sym_tab.png">
+</p>
+
+### 2.3.7 PTI Signal
+<p style="text-align: center;">
+<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/pti_signal_tab.png">
+</p>
+
+# 3. libraries
+
+## 3.1 Algorithm
+The subpackage Algorithm contains the implementation of the algorithms and can be divided into the subpackages interferometry and pti. interferometry contains the algorithms for the interferometric phase and characterisation of the interferometer. pti contains the algorithms for decimation and PTI inversion.
+
+It is also possible to use only the interferometer subpackage without having to install dependencies for the other packages.
+
+### 3.1.1 Interferometry
+interferometry contains the classes interferometer and characterisation.
+Examples of usage can be found under <a href="https://github.com/bilaljo/MiniPTI/blob/main/examples/interferometry.py">examples/interferometer.py</a> and
+<a href="https://github.com/bilaljo/MiniPTI/blob/main/examples/characterisation.py">examples/characterisation.py</a>.
+### 3.1.2 PTI
+pti contains the classes decimation inversion. Example calls can be found under <a href="https://github.com/bilaljo/MiniPTI/blob/main/examples/pti_inversion.py">examples/pti_inversion.py</a>
+## 3.2 Hardware
+Hardware contains the classes to control the motherboard (DAQ + BMS), laser (Probe and Pump Laser) and TEC driver as well as the valve control.
```

### Comparing `minipti-1.9.1/README.md` & `minipti-1.9.3/README.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,107 +1,107 @@
-# MiniPTI
-
-<p style="text-align: center;">
-<img alt="flowchart" src="https://www.fhnw.ch/de/medien/logos/media/fhnw_e_10mm.jpg" class="centre">
-</p>
-
-In this repository a GUI is provided to control the MiniPTI as also presented in [Waveguide based passively demodulated photothermal interferometer for light absorption measurements of trace substances](https://doi.org/10.1364/AO.476868). In addition to the GUI, Python implementations of the presented algorithms and the driver software for the MiniPTI hardware are also provided as libraries.
-
-# 1. installation
-In order to make the library light-weighted different installation options exist.
-
-To install only the interferometry library you can install it with
-```
-pip install minipti
-```
-To additionally use the inversion algorithm you can type
-```bash
-pip install minipti[algorithm]
-```
-To install the entire package (GUI, algorithms and hardware drivers) you can type
-```bash
-pip install minipti[gui]
-```
-# 2. Usage and GUI
-The GUI can be used via
-```bash
-python -m minipti
-```
-
-## 2.1 Home Tab
-<p style="text-align: center;">
-<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/home.png">
-</p>
-
-## 2.2 Pump Laser Tab
-### 2.2.1 Pump Laser Driver Tab
-<p style="text-align: center;">
-<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/pump_laser_tab.png">
-</p>
-
-### 2.2.2 Pump Laser Tec Driver Tab
-<p style="text-align: center;">
-<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/pump_tec.png">
-</p>
-
-## 2.3 Probe Laser Tab
-### 2.3.1 Probe Laser Driver Tab
-<p style="text-align: center;">
-<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/probe_laser_tab.png">
-</p>
-
-### 2.3.1 Probe Laser Tec Driver Tab
-<p style="text-align: center;">
-<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/probe_tec.png">
-</p>
-
-## 2.3 Plotting Tabs
-### 2.3.1 DC Signals
-<p style="text-align: center;">
-<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/dc_tab.png">
-</p>
-
-### 2.3.2 Amplitudes
-<p style="text-align: center;">
-<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/amplitudes_tab.png">
-</p>
-
-### 2.3.3 Output Phases
-<p style="text-align: center;">
-<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/output_phases_tab.png">
-</p>
-
-### 2.3.4 Interferometric Phase
-<p style="text-align: center;">
-<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/phase_tab.png">
-</p>
-
-### 2.3.5 Sensitivity
-<p style="text-align: center;">
-<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/sensitivity_tab.png">
-</p>
-
-### 2.3.6 Symmetry
-<p style="text-align: center;">
-<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/sym_tab.png">
-</p>
-
-### 2.3.7 PTI Signal
-<p style="text-align: center;">
-<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/pti_signal_tab.png">
-</p>
-
-# 3. libraries
-
-## 3.1 Algorithm
-The subpackage Algorithm contains the implementation of the algorithms and can be divided into the subpackages interferometry and pti. interferometry contains the algorithms for the interferometric phase and characterisation of the interferometer. pti contains the algorithms for decimation and PTI inversion.
-
-It is also possible to use only the interferometer subpackage without having to install dependencies for the other packages.
-
-### 3.1.1 Interferometry
-interferometry contains the classes interferometer and characterisation.
-Examples of usage can be found under <a href="https://github.com/bilaljo/MiniPTI/blob/main/examples/interferometry.py">examples/interferometer.py</a> and
-<a href="https://github.com/bilaljo/MiniPTI/blob/main/examples/characterisation.py">examples/characterisation.py</a>.
-### 3.1.2 PTI
-pti contains the classes decimation inversion. Example calls can be found under <a href="https://github.com/bilaljo/MiniPTI/blob/main/examples/pti_inversion.py">examples/pti_inversion.py</a>
-## 3.2 Hardware
-Hardware contains the classes to control the motherboard (DAQ + BMS), laser (Probe and Pump Laser) and TEC driver as well as the valve control.
+# MiniPTI
+
+<p style="text-align: center;">
+<img alt="flowchart" src="https://www.fhnw.ch/de/medien/logos/media/fhnw_e_10mm.jpg" class="centre">
+</p>
+
+In this repository a GUI is provided to control the MiniPTI as also presented in [Waveguide based passively demodulated photothermal interferometer for light absorption measurements of trace substances](https://doi.org/10.1364/AO.476868). In addition to the GUI, Python implementations of the presented algorithms and the driver software for the MiniPTI hardware are also provided as libraries.
+
+# 1. installation
+In order to make the library light-weighted different installation options exist.
+
+To install only the interferometry library you can install it with
+```
+pip install minipti
+```
+To additionally use the inversion algorithm you can type
+```bash
+pip install minipti[algorithm]
+```
+To install the entire package (GUI, algorithms and hardware drivers) you can type
+```bash
+pip install minipti[gui]
+```
+# 2. Usage and GUI
+The GUI can be used via
+```bash
+python -m minipti
+```
+
+## 2.1 Home Tab
+<p style="text-align: center;">
+<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/home.png">
+</p>
+
+## 2.2 Pump Laser Tab
+### 2.2.1 Pump Laser Driver Tab
+<p style="text-align: center;">
+<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/pump_laser_tab.png">
+</p>
+
+### 2.2.2 Pump Laser Tec Driver Tab
+<p style="text-align: center;">
+<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/pump_tec.png">
+</p>
+
+## 2.3 Probe Laser Tab
+### 2.3.1 Probe Laser Driver Tab
+<p style="text-align: center;">
+<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/probe_laser_tab.png">
+</p>
+
+### 2.3.1 Probe Laser Tec Driver Tab
+<p style="text-align: center;">
+<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/probe_tec.png">
+</p>
+
+## 2.3 Plotting Tabs
+### 2.3.1 DC Signals
+<p style="text-align: center;">
+<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/dc_tab.png">
+</p>
+
+### 2.3.2 Amplitudes
+<p style="text-align: center;">
+<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/amplitudes_tab.png">
+</p>
+
+### 2.3.3 Output Phases
+<p style="text-align: center;">
+<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/output_phases_tab.png">
+</p>
+
+### 2.3.4 Interferometric Phase
+<p style="text-align: center;">
+<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/phase_tab.png">
+</p>
+
+### 2.3.5 Sensitivity
+<p style="text-align: center;">
+<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/sensitivity_tab.png">
+</p>
+
+### 2.3.6 Symmetry
+<p style="text-align: center;">
+<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/sym_tab.png">
+</p>
+
+### 2.3.7 PTI Signal
+<p style="text-align: center;">
+<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/pti_signal_tab.png">
+</p>
+
+# 3. libraries
+
+## 3.1 Algorithm
+The subpackage Algorithm contains the implementation of the algorithms and can be divided into the subpackages interferometry and pti. interferometry contains the algorithms for the interferometric phase and characterisation of the interferometer. pti contains the algorithms for decimation and PTI inversion.
+
+It is also possible to use only the interferometer subpackage without having to install dependencies for the other packages.
+
+### 3.1.1 Interferometry
+interferometry contains the classes interferometer and characterisation.
+Examples of usage can be found under <a href="https://github.com/bilaljo/MiniPTI/blob/main/examples/interferometry.py">examples/interferometer.py</a> and
+<a href="https://github.com/bilaljo/MiniPTI/blob/main/examples/characterisation.py">examples/characterisation.py</a>.
+### 3.1.2 PTI
+pti contains the classes decimation inversion. Example calls can be found under <a href="https://github.com/bilaljo/MiniPTI/blob/main/examples/pti_inversion.py">examples/pti_inversion.py</a>
+## 3.2 Hardware
+Hardware contains the classes to control the motherboard (DAQ + BMS), laser (Probe and Pump Laser) and TEC driver as well as the valve control.
```

### Comparing `minipti-1.9.1/pyproject.toml` & `minipti-1.9.3/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-[project]
-dependencies = [
-    "numpy",
-    "scipy",
-    "pandas"
-]
-name = "minipti"
-version = "1.9.1"
-authors = [
-    { name = "Jonas Bilal", email = "jonasbilal@outlook.com" },
-]
-
-description = "Provides algorithm and GUI for photo thermal interferometry and 3x3 couplers"
-readme = "README.md"
-requires-python = ">=3.9"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-
-[project.optional-dependencies]
-algorithm = [
-    "minipti",
-    "beartype",
-    "dacite",
-    "h5py",
-    "nptyping",
-]
-
-gui = [
-    "minipti[algorithm]",
-    # Hardware
-    "fastcrc",
-    "pyserial",
-    # GUI
-    "PyQt5",
-    "pyqtgraph"
-]
-
-[project.urls]
-"Homepage" = "https://www.fhnw.ch/en/about-fhnw/schools/school-of-engineering/institutes/institute-for-sensors-and-electronics/aerosol-measurement-technology"
-"Source" = "https://github.com/bilaljo/MiniPTI"
-"Bug Tracker" = "https://github.com/bilaljo/MiniPTI/issues"
+[project]
+dependencies = [
+    "numpy",
+    "scipy",
+    "pandas"
+]
+name = "minipti"
+version = "1.9.3"
+authors = [
+    { name = "Jonas Bilal", email = "jonasbilal@outlook.com" },
+]
+
+description = "Provides algorithm and GUI for photo thermal interferometry and 3x3 couplers"
+readme = "README.md"
+requires-python = ">=3.9"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+
+[project.optional-dependencies]
+algorithm = [
+    "minipti",
+    "beartype",
+    "dacite",
+    "h5py",
+    "nptyping",
+]
+
+gui = [
+    "minipti[algorithm]",
+    # Hardware
+    "fastcrc",
+    "pyserial",
+    # GUI
+    "PyQt5",
+    "pyqtgraph"
+]
+
+[project.urls]
+"Homepage" = "https://www.fhnw.ch/en/about-fhnw/schools/school-of-engineering/institutes/institute-for-sensors-and-electronics/aerosol-measurement-technology"
+"Source" = "https://github.com/bilaljo/MiniPTI"
+"Bug Tracker" = "https://github.com/bilaljo/MiniPTI/issues"
```

### Comparing `minipti-1.9.1/src/minipti/algorithm/interferometry.py` & `minipti-1.9.3/src/algorithm/interferometry.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,408 +1,417 @@
-"""
-API for characterisation and phases of an interferometer.
-"""
-
-import csv
-import itertools
-import logging
-import os
-import threading
-from typing import Union, Generator, Iterable
-from collections import defaultdict
-
-import numpy as np
-import pandas as pd
-from scipy import optimize, linalg
-
-
-class Interferometer:
-    """
-    Provides the API for calculating the interferometric phase based on its characteristic values.
-    """
-    DC_HEADERS = [[f"PD{i}" for i in range(1, 4)],
-                  [f"DC CH{i}" for i in range(1, 4)]]
-
-    OPTIMAL_SYMMETRY = 86.58
-
-    def __init__(self, settings_path=f"{os.path.dirname(__file__)}/configs/settings.csv",
-                 decimation_filepath="data/Decimation.csv", output_phases=np.empty(shape=3),
-                 amplitudes=np.empty(shape=3), offsets=np.empty(shape=3)):
-        self.settings_path = settings_path
-        self.decimation_filepath = decimation_filepath
-        self.phase: Union[float, np.ndarray] = 0
-        self._output_phases = output_phases
-        self._amplitudes = amplitudes
-        self._offsets = offsets
-        self.absoloute_symmetry: Union[float, np.ndarray] = 100
-        self.relative_symmetry: Union[float, np.ndarray] = 100
-        self._locks = {"Output Phases": threading.Lock(), "Amplitudes": threading.Lock(),
-                       "Offsets": threading.Lock()}
-
-    def load_settings(self) -> None:
-        """
-        Read the characteristic values (amplitude, offset and output phase).
-        """
-        settings = pd.read_csv(self.settings_path, index_col="Setting")
-        self.output_phases = np.deg2rad(settings.loc["Output Phases [deg]"].to_numpy())
-        self.amplitudes = settings.loc["Amplitude [V]"].to_numpy()
-        self.offsets = settings.loc["Offset [V]"].to_numpy()
-
-    def __eq__(self, other) -> bool:
-        return self.amplitudes == other.amplitudes and self.offsets == other.amplitudes and \
-            self.output_phases == other.output_phases
-
-    def __repr__(self) -> str:
-        class_name = self.__class__.__name__
-        representation = f"{class_name}(setting_path={self.settings_path}," \
-                         f" decimation_path={self.decimation_filepath}\n"
-        representation += f"phae={self.phase}, output_phases={self.output_phases}," \
-                          f" amplitudes={self.amplitudes}\n"
-        representation += f"offsets={self.offsets}) phases={self.phase}"
-        return representation
-
-    def __str__(self) -> str:
-        output_phase_str = "Output Phases [deg]:\n"
-        amplitude_str = "Amplitudes [V]:\n"
-        offset_str = "Offsets [V]:\n"
-        for i in range(2):
-            output_phase_str += f"CH {i + 1}: {round(np.rad2deg(self.output_phases[i]), 2)},"
-            amplitude_str += f"CH {i + 1}: {round(self.amplitudes[i], 2)},"
-            offset_str += f"CH {i + 1}: {round(self.offsets[i], 2)},"
-        output_phase_str += f"CH3: {round(np.rad2deg(self.output_phases[2]), 2)}, "
-        amplitude_str += f"CH3: {round(self.amplitudes[2], 2)},"
-        offset_str += f"CH3: {round(self.offsets[2], 2)},"
-        return amplitude_str + "\n" + offset_str + "\n" + output_phase_str
-
-    @property
-    def amplitudes(self) -> np.ndarray:
-        with self._locks["Amplitudes"]:
-            amplitudes = self._amplitudes
-        return amplitudes
-
-    @amplitudes.setter
-    def amplitudes(self, amplitudes: np.ndarray):
-        with self._locks["Amplitudes"]:
-            self._amplitudes = amplitudes
-
-    @property
-    def offsets(self) -> np.ndarray:
-        with self._locks["Offsets"]:
-            offsets = self._offsets
-        return offsets
-
-    @offsets.setter
-    def offsets(self, offsets: np.ndarray):
-        with self._locks["Offsets"]:
-            self._offsets = offsets
-
-    @property
-    def output_phases(self) -> np.ndarray:
-        with self._locks["Output Phases"]:
-            output_phase = self._output_phases
-        return output_phase
-
-    @output_phases.setter
-    def output_phases(self, output_phases: np.ndarray):
-        with self._locks["Output Phases"]:
-            self._output_phases = output_phases
-
-    def read_decimation(self) -> Union[pd.DataFrame, None]:
-        try:
-            with open(self.decimation_filepath, "r", encoding="UTF-8") as csv_file:
-                dc_delimiter = str(csv.Sniffer().sniff(csv_file.readline()).delimiter)
-        except FileNotFoundError:
-            logging.error("Could not find %s", self.decimation_filepath)
-            return None
-        return pd.read_csv(self.decimation_filepath, delimiter=dc_delimiter, skiprows=[1])
-
-    @staticmethod
-    def error_handing_intensity(intensity):
-        if not isinstance(intensity, np.ndarray):
-            intensity = np.array(intensity)
-        if len(intensity.shape) != 2:
-            raise ValueError(f"Expected length of shape of 2, got {len(intensity.shape)} instead.")
-        if not (intensity.shape[0] == 3 or intensity.shape[1] == 3):
-            raise ValueError(f"Expected length of (3, n) or (n, 3), got {intensity.shape} instead.")
-        if intensity.shape[0] == intensity.shape[1]:
-            raise ValueError("Same shape for both dimensions. Could determine which dimension"
-                             " describes channels.")
-
-    def calculate_amplitudes(self, intensity: np.ndarray):
-        """
-        The amplitude of perfect sine wave can be calculated according to A = (I_max - I_min) / 2.
-        This function is only used as approximation.
-        """
-        Interferometer.error_handing_intensity(intensity)
-        if intensity.shape[1] == 3:
-            self.amplitudes = (np.max(intensity, axis=0) - np.min(intensity, axis=0)) / 2
-        else:
-            self.amplitudes = (np.max(intensity, axis=1) - np.min(intensity, axis=1)) / 2
-
-    def calculate_offsets(self, intensity: np.ndarray):
-        """
-        The offset of perfect sine wave can be calculated according to A = (I_max + I_min) / 2.
-        This function is only used as approximation.
-        """
-        Interferometer.error_handing_intensity(intensity)
-        if intensity.shape[1] == 3:
-            self.offsets = (np.max(intensity, axis=0) + np.min(intensity, axis=0)) / 2
-        else:
-            self.offsets = (np.max(intensity, axis=1) + np.min(intensity, axis=1)) / 2
-
-    def _error_function(self, intensity: np.ndarray):
-        intensity_scaled = (intensity - self.offsets) / self.amplitudes
-
-        def error(phase: Iterable):
-            try:
-                return np.cos(phase - self.output_phases) - intensity_scaled
-            except TypeError:
-                return np.cos(np.array(phase) - np.array(self.output_phases)) - intensity_scaled
-
-        return error
-
-    def _error_function_df(self, phase: Iterable):
-        try:
-            return -np.sin(phase - self.output_phases).reshape((3, 1))
-        except AttributeError:
-            return -np.sin(np.array(phase) - np.array(self.output_phases)).reshape((3, 1))
-
-    def _calculate_phase(self, intensity: np.ndarray):
-        res = optimize.least_squares(fun=self._error_function(intensity), method="lm", x0=np.array(0),
-                                     tr_solver="exact",  jac=self._error_function_df).x
-        return res % (2 * np.pi)
-
-    def calculate_phase(self, intensities: np.ndarray):
-        """
-        Calculated the interferometric phase with the defined characteristic parameters.
-        """
-        if len(intensities) == 3:  # Only one Sample of 3 Values
-            self.phase = self._calculate_phase(intensities)[0]
-        else:
-            self.phase = np.fromiter(map(self._calculate_phase, intensities), dtype=float)
-
-
-class Characterization:
-    """
-    Provided an API for the characterization_live of an interferometer as described in [1].
-    [1]:
-    """
-    MAX_ITERATIONS = 30
-    STEP_SIZE = 100
-
-    def __init__(self, interferometer=Interferometer(), use_settings=True):
-        self.interferometer = interferometer
-        self.tracking_phase = []
-        self._occurred_phases = np.full(Characterization.STEP_SIZE, False)
-        self.use_settings = use_settings
-        self.time_stamp = 0
-        self.event = threading.Event()
-        self.destination_folder = os.getcwd()
-        self.init_headers = True
-        self._signals = np.empty(1)
-        self.phases = []
-
-    def __repr__(self) -> str:
-        class_name = self.__class__.__name__
-        representation = f"{class_name}(signals={self._signals}, use_settings={self.use_settings}," \
-                         f"destination_folder={self.destination_folder}, phases={np.array(self.phases)}," \
-                         f" init_headers={self.init_headers}, tracking_phase={np.array(self.tracking_phase)}" \
-                         f" time_stamp={self.time_stamp}, interferometer={self.interferometer})"
-        return representation
-
-    @property
-    def enough_values(self) -> bool:
-        return np.all(self._occurred_phases)
-
-    @property
-    def occurred_phases(self) -> np.ndarray:
-        return self._occurred_phases
-
-    def calculate_symmetry(self) -> None:
-        sensitivity = np.empty(shape=(3, len(self.phases)))
-        for i in range(3):
-            amplitude = self.interferometer.amplitudes[i]
-            output_phase = self.interferometer.output_phases[i]
-            sensitivity[i] = amplitude * np.abs(np.sin(np.array(self.phases) - output_phase))
-        total_sensitivity = np.sum(sensitivity, axis=0)
-        absoloute_symmetry = np.min(total_sensitivity) / np.max(total_sensitivity) * 100
-        relative_symmetry = absoloute_symmetry / Interferometer.OPTIMAL_SYMMETRY * 100
-        self.interferometer.absoloute_symmetry = absoloute_symmetry
-        self.interferometer.relative_symmetry = relative_symmetry
-
-    def characterise(self, live=False) -> None:
-        if self.init_headers:
-            units = {}
-            # The output data has no headers and relies on this order
-            for channel in range(1, 4):
-                units[f"Output Phase CH{channel}"] = "deg"
-                units[f"Amplitude CH{channel}"] = "V"
-                units[f"Offset CH{channel}"] = "V"
-            units["Symmetry"] = "%"
-            units["Relative Symmetry"] = "%"
-            pd.DataFrame(units, index=["s"]).to_csv(f"{self.destination_folder}/Characterisation.csv",
-                                                    index_label="Time Stamp")
-            self.init_headers = False
-        if live:
-            self._calculate_online()
-        else:
-            self._calculate_offline()
-            self.init_headers = True
-
-    def add_phase(self, phase: float) -> None:
-        """
-        Adds a phase to list of occurred phase and mark its corresponding index in the occurred
-        array.
-        Args:
-            phase (float): The occurred interferometric phase in rad.
-        """
-        self.time_stamp += 1
-        if phase > 2 * np.pi:
-            phase %= 2 * np.pi  # Phase is out of range
-        self.tracking_phase.append(phase)
-        k = int(Characterization.STEP_SIZE * phase / (2 * np.pi))
-        self._occurred_phases[k] = True
-
-    def clear(self) -> None:
-        """
-        Resets the characterisation buffers.
-        """
-        self.tracking_phase = []
-        self._signals = []
-        self._occurred_phases = np.full(Characterization.STEP_SIZE, False)
-        self.event.clear()
-
-    def _init_parameters(self, dc_signals=None) -> None:
-        if self.use_settings:
-            settings = pd.read_csv(self.interferometer.settings_path, index_col="Setting")
-            self.interferometer.output_phases = np.deg2rad(settings.loc["Output Phases [deg]"])
-            self.interferometer.amplitudes = settings.loc["Amplitude [V]"]
-            self.interferometer.offsets = settings.loc["Offset [V]"]
-        else:
-            self.interferometer.calculate_offsets(dc_signals)
-            self.interferometer.calculate_amplitudes(dc_signals)
-            self.interferometer.output_phases = np.array([0, 2 * np.pi / 3, 4 * np.pi / 3])
-
-    def process_characterisation(self, dc_signals: np.ndarray) -> Generator[int, None, int]:
-        last_index: int = 0
-        data_length = dc_signals.size // 3  # 3 Channels
-        if self.use_settings:
-            self._init_parameters()
-        else:
-            self._init_parameters(dc_signals)
-        for i in range(data_length):
-            self.interferometer.calculate_phase(dc_signals[i])
-            self.add_phase(self.interferometer.phase)
-            if self.enough_values:
-                self._signals = dc_signals[last_index:i + 1].T
-                self.phases = self.tracking_phase
-                if not self.use_settings:
-                    self._iterate_characterization()
-                    self.use_settings = True  # For next time these values can be used now
-                else:
-                    self._characterise_interferometer()
-                self.calculate_symmetry()
-                last_index = i + 1
-            yield i
-            if self.enough_values:
-                self.clear()
-        self.clear()
-        return last_index
-
-    def _characterise_interferometer(self) -> None:
-        """
-        Calculates with the least squares method the output phases and min and max intensities for
-        every channel. If no min/max values and output phases are given (either none or nan) the
-        function try to estimate them best-possible.
-        """
-        output_phases = []
-        amplitudes = []
-        offsets = []
-
-        def add_values(result):
-            output_phases.append((np.arctan2(result[1], result[0])) % (2 * np.pi))
-            amplitudes.append(np.sqrt(result[0] ** 2 + result[1] ** 2))
-            offsets.append(result[2])
-
-        cosine_values = np.cos(self.phases)
-        sine_values = np.sin(self.phases)
-        results, _, _, _ = linalg.lstsq(np.array([cosine_values, np.ones(len(cosine_values))]).T,
-                                        self._signals[0], check_finite=False)
-        amplitudes.append(results[0])
-        offsets.append(results[1])
-        output_phases.append(0)
-
-        parameters = np.array([cosine_values, sine_values, np.ones(len(sine_values))]).T
-
-        results, _, _, _ = linalg.lstsq(parameters, self._signals[1], check_finite=False)
-        add_values(results)
-
-        results, _, _, _ = linalg.lstsq(parameters, self._signals[2], check_finite=False)
-        add_values(results)
-
-        self.interferometer.output_phases = output_phases
-        self.interferometer.amplitudes = amplitudes
-        self.interferometer.offsets = offsets
-
-    def _iterate_characterization(self) -> None:
-        logging.info("Start iteration...")
-        for _ in itertools.repeat(None, Characterization.MAX_ITERATIONS):
-            self.interferometer.calculate_phase(self._signals.T)
-            self.phases = self.interferometer.phase
-            self._characterise_interferometer()
-            logging.info("Current estimation:\n%s", str(self.interferometer))
-        logging.info("Final values:\n%s", str(self.interferometer))
-
-    def _add_characterised_data(self, output_data: defaultdict) -> None:
-        for channel in range(3):
-            output_phase_deg = np.rad2deg(self.interferometer.output_phases[channel])
-            output_data[f"Output Phase CH{channel + 1}"].append(output_phase_deg)
-            output_data[f"Amplitude CH{channel + 1}"].append(self.interferometer.amplitudes[channel])
-            output_data[f"Offset CH{channel + 1}"].append(self.interferometer.offsets[channel])
-        output_data["Symmetry"].append(self.interferometer.absoloute_symmetry)
-        output_data["Relative Symmetry"].append(self.interferometer.relative_symmetry)
-
-    def _calculate_offline(self, dc_signals=None):
-        output_data = defaultdict(list)
-        time_stamps = []
-        if dc_signals is None:
-            data = self.interferometer.read_decimation()
-            for header in Interferometer.DC_HEADERS:
-                try:
-                    dc_signals = data[header].to_numpy()
-                    break
-                except KeyError:
-                    continue
-            else:
-                raise KeyError("Invalid key for DC values given")
-        self.clear()
-        process_characterisation: Generator[int, None, int] = self.process_characterisation(dc_signals)
-        while True:
-            try:
-                i = next(process_characterisation)
-                if self.enough_values:
-                    time_stamps.append(i)
-                    self._add_characterised_data(output_data)
-            except StopIteration as ex:
-                last_index = ex.value
-                break
-        if last_index == 0:
-            logging.warning("Not enough values for characterization")
-        else:
-            pd.DataFrame(output_data, index=time_stamps).to_csv(f"{self.destination_folder}/Characterisation.csv",
-                                                                mode="a", index_label="Time Stamp", header=False)
-            logging.info("Characterization finished")
-            logging.info("Saved data into %s", self.destination_folder)
-
-    def _calculate_online(self) -> None:
-        self.event.wait()
-        self._signals = np.array(self._signals).T
-        self._characterise_interferometer()
-        characterised_data = {}
-        for i in range(3):
-            characterised_data[f"Output Phase CH{1 + i}"] = np.rad2deg(self.interferometer.output_phases[i])
-            characterised_data[f"Amplitude CH{1 + i}"] = self.interferometer.amplitudes[i]
-            characterised_data[f"Offset CH{1 + i}"] = self.interferometer.offsets[i]
-        pd.DataFrame(characterised_data, index=[self.time_stamp]).to_csv(
-            f"{self.destination_folder}/Characterisation.csv",
-            mode="a", header=False, index_label="Time Stamp")
-        self.clear()
+"""
+API for characterisation and phases of an interferometer.
+"""
+
+import csv
+import itertools
+import logging
+import os
+import threading
+import typing
+from typing import Union, Generator
+from collections import defaultdict
+
+import numpy as np
+import pandas as pd
+from scipy import optimize, linalg
+
+
+class _Locks(typing.NamedTuple):
+    output_phases = threading.Lock()
+    amplitudes = threading.Lock()
+    offsets = threading.Lock()
+
+
+class Interferometer:
+    """
+    Provides the API for calculating the interferometric phase based on its characteristic values.
+    """
+    CHANNELS = 3
+
+    DC_HEADERS = [[f"PD{i}" for i in range(1, 4)],
+                  [f"DC CH{i}" for i in range(1, 4)]]
+
+    OPTIMAL_SYMMETRY = 86.58  # %
+
+    def __init__(self, settings_path=f"{os.path.dirname(__file__)}/configs/settings.csv",
+                 decimation_filepath="data/Decimation.csv", output_phases=np.empty(shape=3),
+                 amplitudes=np.empty(shape=3), offsets=np.empty(shape=3)):
+        self.settings_path = settings_path
+        self.decimation_filepath = decimation_filepath
+        self.phase: Union[float, np.ndarray] = 0
+        self._output_phases = output_phases
+        self._amplitudes = amplitudes
+        self._offsets = offsets
+        self.absolute_symmetry: Union[float, np.ndarray] = 100
+        self.relative_symmetry: Union[float, np.ndarray] = 100
+        self._locks = _Locks()
+
+    def load_settings(self) -> None:
+        """
+        Read the characteristic values (amplitude, offset and output phase).
+        """
+        settings = pd.read_csv(self.settings_path, index_col="Setting")
+        self.output_phases = np.deg2rad(settings.loc["Output Phases [deg]"].to_numpy())
+        self.amplitudes = settings.loc["Amplitude [V]"].to_numpy()
+        self.offsets = settings.loc["Offset [V]"].to_numpy()
+
+    def __eq__(self, other) -> bool:
+        return self.amplitudes == other.amplitudes and self.offsets == other.amplitudes and \
+            self.output_phases == other.output_phases
+
+    def __repr__(self) -> str:
+        class_name = self.__class__.__name__
+        representation = f"{class_name}(setting_path={self.settings_path}," \
+                         f" decimation_path={self.decimation_filepath}\n"
+        representation += f"phae={self.phase}, output_phases={self.output_phases}," \
+                          f" amplitudes={self.amplitudes}\n"
+        representation += f"offsets={self.offsets}) phases={self.phase}"
+        return representation
+
+    def __str__(self) -> str:
+        output_phase_str = "Output Phases [deg]:\n"
+        amplitude_str = "Amplitudes [V]:\n"
+        offset_str = "Offsets [V]:\n"
+        for i in range(2):
+            output_phase_str += f"CH {i + 1}: {round(np.rad2deg(self.output_phases[i]), 2)}, "
+            amplitude_str += f"CH {i + 1}: {round(self.amplitudes[i], 2)}, "
+            offset_str += f"CH {i + 1}: {round(self.offsets[i], 2)}, "
+        output_phase_str += f"CH3: {round(np.rad2deg(self.output_phases[2]), 2)}"
+        amplitude_str += f"CH3: {round(self.amplitudes[2], 2)}"
+        offset_str += f"CH3: {round(self.offsets[2], 2)}"
+        return amplitude_str + "\n" + offset_str + "\n" + output_phase_str
+
+    @property
+    def amplitudes(self) -> np.ndarray:
+        with self._locks.amplitudes:
+            amplitudes = self._amplitudes
+        return amplitudes
+
+    @amplitudes.setter
+    def amplitudes(self, amplitudes: np.ndarray):
+        with self._locks.amplitudes:
+            self._amplitudes = amplitudes
+
+    @property
+    def offsets(self) -> np.ndarray:
+        with self._locks.offsets:
+            offsets = self._offsets
+        return offsets
+
+    @offsets.setter
+    def offsets(self, offsets: np.ndarray):
+        with self._locks.offsets:
+            self._offsets = offsets
+
+    @property
+    def output_phases(self) -> np.ndarray:
+        with self._locks.output_phases:
+            output_phase = self._output_phases
+        return output_phase
+
+    @output_phases.setter
+    def output_phases(self, output_phases: np.ndarray):
+        with self._locks.output_phases:
+            self._output_phases = output_phases
+
+    def read_decimation(self) -> Union[pd.DataFrame, None]:
+        try:
+            with open(self.decimation_filepath, "r", encoding="UTF-8") as csv_file:
+                dc_delimiter = str(csv.Sniffer().sniff(csv_file.readline()).delimiter)
+        except FileNotFoundError:
+            logging.error("Could not find %s", self.decimation_filepath)
+            return None
+        return pd.read_csv(self.decimation_filepath, delimiter=dc_delimiter, skiprows=[1])
+
+    def calculate_amplitudes(self, intensity: np.ndarray):
+        """
+        The amplitude of perfect sine wave can be calculated according to A = (I_max - I_min) / 2.
+        This function is only used as approximation.
+        """
+        if intensity.shape[0] == 3:
+            self.amplitudes = (np.max(intensity, axis=1) - np.min(intensity, axis=1)) / 2
+        else:
+            self.amplitudes = (np.max(intensity, axis=0) - np.min(intensity, axis=0)) / 2
+
+    def calculate_offsets(self, intensity: np.ndarray):
+        """
+        The offset of perfect sine wave can be calculated according to B = (I_max + I_min) / 2.
+        This function is only used as approximation.
+        """
+        if intensity.shape[0] == 3:
+            self.offsets = (np.max(intensity, axis=1) + np.min(intensity, axis=1)) / 2
+        else:
+            self.offsets = (np.max(intensity, axis=0) + np.min(intensity, axis=0)) / 2
+
+    def _error_function(self, intensity: np.ndarray):
+        intensity_scaled = (intensity - self.offsets) / self.amplitudes
+
+        def error(phase: np.ndarray):
+            try:
+                return np.cos(phase - self.output_phases) - intensity_scaled
+            except TypeError:
+                return np.cos(np.array(phase) - np.array(self.output_phases)) - intensity_scaled
+
+        return error
+
+    def _error_function_df(self, phase: np.ndarray):
+        try:
+            return -np.sin(phase - self.output_phases).reshape((3, 1))
+        except AttributeError:
+            return -np.sin(np.array(phase) - np.array(self.output_phases)).reshape((3, 1))
+
+    def _calculate_phase(self, intensity: np.ndarray):
+        res = optimize.least_squares(fun=self._error_function(intensity), method="lm", x0=np.array(0),
+                                     tr_solver="exact",  jac=self._error_function_df).x
+        return res % (2 * np.pi)
+
+    def calculate_phase(self, intensities: np.ndarray):
+        """
+        Calculated the interferometric phase with the defined characteristic parameters.
+        """
+        if intensities.size // Interferometer.CHANNELS == 1:  # Only one Sample of 3 Values
+            self.phase = self._calculate_phase(intensities)[0]
+        else:
+            if intensities.shape[1] == 3:
+                self.phase = np.fromiter(map(self._calculate_phase, intensities), dtype=float)
+            else:
+                self.phase = np.fromiter(map(self._calculate_phase, intensities.T), dtype=float)
+
+
+class Characterization:
+    """
+    Provided an API for the characterization_live of an interferometer as described in [1].
+    [1]:
+    """
+    MAX_ITERATIONS = 30
+    STEP_SIZE = 100
+
+    def __init__(self, interferometer=Interferometer(), use_configuration=True, use_parameters=True):
+        self.interferometer = interferometer
+        self.tracking_phase = []
+        self._occurred_phases = np.full(Characterization.STEP_SIZE, False)
+        self.use_configuration = use_configuration
+        self.use_parameters = use_parameters
+        self.time_stamp = 0
+        self.event = threading.Event()
+        self.destination_folder = os.getcwd()
+        self.init_headers = True
+        self._signals = np.empty(1)
+        self.phases = []
+
+    @property
+    def signals(self) -> np.ndarray:
+        return self._signals
+
+    @signals.setter
+    def signals(self, data: np.ndarray) -> None:
+        if data.shape[0] == 3:
+            self._signals = data
+        else:
+            self._signals = data.T
+
+    def __repr__(self) -> str:
+        class_name = self.__class__.__name__
+        representation = f"{class_name}(signals={self._signals}, use_settings={self.use_configuration}," \
+                         f"destination_folder={self.destination_folder}, phases={np.array(self.phases)}," \
+                         f" init_headers={self.init_headers}, tracking_phase={np.array(self.tracking_phase)}" \
+                         f" time_stamp={self.time_stamp}, interferometer={self.interferometer})"
+        return representation
+
+    @property
+    def enough_values(self) -> bool:
+        return np.all(self._occurred_phases)
+
+    @property
+    def occurred_phases(self) -> np.ndarray:
+        return self._occurred_phases
+
+    def calculate_symmetry(self) -> None:
+        sensitivity = np.empty(shape=(3, len(self.phases)))
+        for i in range(3):
+            amplitude = self.interferometer.amplitudes[i]
+            output_phase = self.interferometer.output_phases[i]
+            sensitivity[i] = amplitude * np.abs(np.sin(np.array(self.phases) - output_phase))
+        total_sensitivity = np.sum(sensitivity, axis=0)
+        absolute_symmetry = np.min(total_sensitivity) / np.max(total_sensitivity) * 100
+        relative_symmetry = absolute_symmetry / Interferometer.OPTIMAL_SYMMETRY * 100
+        self.interferometer.absolute_symmetry = absolute_symmetry
+        self.interferometer.relative_symmetry = relative_symmetry
+
+    def characterise(self, live=False) -> None:
+        """
+        Characterises the interferometer either live (with data from the motherboard) or offline.
+        Args:
+            live (bool): Decides if running live with motherboard connected or offline with already measured data.
+        """
+        if self.init_headers:
+            units = {}
+            # The output data has no headers and relies on this order
+            for channel in range(1, 4):
+                units[f"Output Phase CH{channel}"] = "deg"
+                units[f"Amplitude CH{channel}"] = "V"
+                units[f"Offset CH{channel}"] = "V"
+            units["Symmetry"] = "%"
+            units["Relative Symmetry"] = "%"
+            pd.DataFrame(units, index=["s"]).to_csv(f"{self.destination_folder}/Characterisation.csv",
+                                                    index_label="Time Stamp")
+            self.init_headers = False
+        if live:
+            self._calculate_online()
+        else:
+            self._calculate_offline()
+            self.init_headers = True
+
+    def add_phase(self, phase: float) -> None:
+        """
+        Adds a phase to list of occurred phase and mark its corresponding index in the occurred
+        array.
+        Args:
+            phase (float): The occurred interferometric phase in rad.
+        """
+        self.time_stamp += 1
+        if phase > 2 * np.pi:
+            phase %= 2 * np.pi  # Phase is out of range
+        self.tracking_phase.append(phase)
+        k = int(Characterization.STEP_SIZE * phase / (2 * np.pi))
+        self._occurred_phases[k] = True
+
+    def clear(self) -> None:
+        """
+        Resets the characterisation buffers.
+        """
+        self.tracking_phase = []
+        self._signals = []
+        self._occurred_phases = np.full(Characterization.STEP_SIZE, False)
+        self.event.clear()
+
+    def _load_settings(self) -> None:
+        settings = pd.read_csv(self.interferometer.settings_path, index_col="Setting")
+        self.interferometer.output_phases = np.deg2rad(settings.loc["Output Phases [deg]"])
+        self.interferometer.amplitudes = settings.loc["Amplitude [V]"]
+        self.interferometer.offsets = settings.loc["Offset [V]"]
+        self.use_parameters = True
+
+    def _estimate_settings(self, dc_signals: np.ndarray) -> None:
+        self.interferometer.calculate_offsets(dc_signals)
+        self.interferometer.calculate_amplitudes(dc_signals)
+        self.interferometer.output_phases = np.array([0, 2 * np.pi / 3, 4 * np.pi / 3])
+        self.use_parameters = False
+
+    def process_characterisation(self, dc_signals: np.ndarray) -> Generator[int, None, None]:
+        last_index: int = 0
+        data_length: int = dc_signals.size // Interferometer.CHANNELS
+        if self.use_configuration:
+            self._load_settings()
+        else:
+            self._estimate_settings(dc_signals)
+        for i in range(data_length):
+            self.interferometer.calculate_phase(dc_signals[i])
+            self.add_phase(self.interferometer.phase)
+            if self.enough_values:
+                self.signals = dc_signals[last_index:i + 1]
+                self.phases = self.tracking_phase
+                if not self.use_parameters:
+                    self._iterate_characterization()
+                    self.use_parameters = True  # For next time these values can be used now
+                else:
+                    self._characterise_interferometer()
+                self.calculate_symmetry()
+                last_index = i + 1
+                self.clear()
+                yield i
+        if last_index == 0:
+            raise ValueError("Not enough values for characterisation")
+
+    def _characterise_interferometer(self) -> None:
+        """
+        Calculates with the least squares method the output phases and min and max intensities for
+        every channel. If no min/max values and output phases are given (either none or nan) the
+        function try to estimate them best-possible.
+        """
+        output_phases = []
+        amplitudes = []
+        offsets = []
+
+        def add_values(result):
+            output_phases.append((np.arctan2(result[1], result[0])) % (2 * np.pi))
+            amplitudes.append(np.sqrt(result[0] ** 2 + result[1] ** 2))
+            offsets.append(result[2])
+
+        cosine_values = np.cos(self.phases)
+        sine_values = np.sin(self.phases)
+        results, _, _, _ = linalg.lstsq(np.array([cosine_values, np.ones(len(cosine_values))]).T,
+                                        self.signals[0], check_finite=False)
+        amplitudes.append(results[0])
+        offsets.append(results[1])
+        output_phases.append(0)
+
+        parameters = np.array([cosine_values, sine_values, np.ones(len(sine_values))]).T
+
+        results, _, _, _ = linalg.lstsq(parameters, self.signals[1], check_finite=False)
+        add_values(results)
+
+        results, _, _, _ = linalg.lstsq(parameters, self.signals[2], check_finite=False)
+        add_values(results)
+
+        self.interferometer.output_phases = output_phases
+        self.interferometer.amplitudes = amplitudes
+        self.interferometer.offsets = offsets
+
+    def _iterate_characterization(self) -> None:
+        logging.info("Start iteration ...")
+        for _ in itertools.repeat(None, Characterization.MAX_ITERATIONS):
+            self.interferometer.calculate_phase(self.signals)
+            self.phases = self.interferometer.phase
+            self._characterise_interferometer()
+            logging.info("Current estimation:\n%s", str(self.interferometer))
+        logging.info("Final values:\n%s", str(self.interferometer))
+
+    def _add_characterised_data(self, output_data: defaultdict) -> None:
+        for channel in range(3):
+            output_phase_deg = np.rad2deg(self.interferometer.output_phases[channel])
+            output_data[f"Output Phase CH{channel + 1}"].append(output_phase_deg)
+            output_data[f"Amplitude CH{channel + 1}"].append(self.interferometer.amplitudes[channel])
+            output_data[f"Offset CH{channel + 1}"].append(self.interferometer.offsets[channel])
+        output_data["Symmetry"].append(self.interferometer.absolute_symmetry)
+        output_data["Relative Symmetry"].append(self.interferometer.relative_symmetry)
+
+    def _calculate_offline(self, dc_signals=None):
+        output_data = defaultdict(list)
+        time_stamps = []
+        if dc_signals is None:
+            data = self.interferometer.read_decimation()
+            for header in Interferometer.DC_HEADERS:
+                try:
+                    dc_signals = data[header].to_numpy()
+                    break
+                except KeyError:
+                    continue
+            else:
+                raise KeyError("Invalid key for DC values given")
+        process_characterisation = self.process_characterisation(dc_signals)
+        try:
+            for i in process_characterisation:
+                time_stamps.append(i)
+                self._add_characterised_data(output_data)
+        except ValueError:
+            logging.warning("Not enough values for characterization")
+        else:
+            pd.DataFrame(output_data, index=time_stamps).to_csv(f"{self.destination_folder}/Characterisation.csv",
+                                                                mode="a", index_label="Time Stamp", header=False)
+            logging.info("Characterization finished")
+            logging.info("Saved data into %s", self.destination_folder)
+
+    def _calculate_online(self) -> None:
+        self.event.wait()
+        self._signals = np.array(self._signals).T
+        self._characterise_interferometer()
+        characterised_data = {}
+        for i in range(3):
+            characterised_data[f"Output Phase CH{1 + i}"] = np.rad2deg(self.interferometer.output_phases[i])
+            characterised_data[f"Amplitude CH{1 + i}"] = self.interferometer.amplitudes[i]
+            characterised_data[f"Offset CH{1 + i}"] = self.interferometer.offsets[i]
+        file_destination: str = f"{self.destination_folder}/Characterisation.csv"
+        pd.DataFrame(characterised_data, index=[self.time_stamp]).to_csv(file_destination, mode="a", header=False,
+                                                                         index_label="Time Stamp")
+        self.clear()
```

### Comparing `minipti-1.9.1/src/minipti/gui/model.py` & `minipti-1.9.3/src/gui/model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,1143 +1,1260 @@
-import abc
-import copy
-import csv
-import enum
-import itertools
-import logging
-import os
-import platform
-import subprocess
-import threading
-import time
-import typing
-from typing import Union
-from collections import deque
-from dataclasses import dataclass, asdict
-from datetime import datetime
-
-import numpy as np
-import pandas as pd
-from PyQt5 import QtCore
-from scipy import ndimage
-
-from .. import algorithm
-from .. import hardware
-
-
-class SettingsTable(QtCore.QAbstractTableModel):
-    HEADERS = ["Detector 1", "Detector 2", "Detector 3"]
-    INDEX = ["Amplitude [V]", "Offset [V]", "Output Phases [deg]", "Response Phases [deg]"]
-    SIGNIFICANT_VALUES = 4
-
-    def __init__(self):
-        QtCore.QAbstractTableModel.__init__(self)
-        self._data = pd.DataFrame(columns=SettingsTable.HEADERS, index=SettingsTable.INDEX)
-        self._file_path = f"{os.path.dirname(os.path.dirname(__file__))}/algorithm/configs/settings.csv"
-        self._observer_callbacks = []
-        signals.settings.connect(self.update_settings)
-
-    @QtCore.pyqtSlot(algorithm.interferometry.Interferometer)
-    def update_settings(self, interferometer: algorithm.interferometry.Interferometer) -> None:
-        self.update_settings_parameters(interferometer)
-
-    def rowCount(self, parent=None) -> int:
-        return self._data.shape[0]
-
-    def columnCount(self, parent=None) -> int:
-        return self._data.shape[1]
-
-    def data(self, index, role: int = ...) -> Union[str, None]:
-        if index.isValid():
-            if role == QtCore.Qt.DisplayRole or role == QtCore.Qt.EditRole:
-                value = self._data.at[
-                    SettingsTable.INDEX[index.row()], SettingsTable.HEADERS[index.column()]]
-                return str(round(value, SettingsTable.SIGNIFICANT_VALUES))
-
-    def flags(self, index):
-        return QtCore.Qt.ItemIsSelectable | QtCore.Qt.ItemIsEnabled | QtCore.Qt.ItemIsEditable
-
-    def setData(self, index, value, role: int = ...):
-        if index.isValid():
-            if role == QtCore.Qt.EditRole:
-                self._data.at[SettingsTable.INDEX[index.row()], SettingsTable.HEADERS[
-                    index.column()]] = float(value)
-                return True
-
-    def headerData(self, section, orientation, role=QtCore.Qt.DisplayRole):
-        if orientation == QtCore.Qt.Horizontal and role == QtCore.Qt.DisplayRole:
-            return SettingsTable.HEADERS[section]
-        elif orientation == QtCore.Qt.Vertical and role == QtCore.Qt.DisplayRole:
-            return SettingsTable.INDEX[section]
-        return super().headerData(section, orientation, role)
-
-    @property
-    def table_data(self) -> pd.DataFrame:
-        return self._data
-
-    @table_data.setter
-    def table_data(self, data) -> None:
-        self._data = data
-
-    @property
-    def file_path(self) -> str:
-        return self._file_path
-
-    @file_path.setter
-    def file_path(self, file_path: str) -> None:
-        if os.path.exists(file_path):
-            self._file_path = file_path
-
-    def save(self) -> None:
-        self._data.to_csv(self.file_path, index_label="Setting", index=True)
-
-    def load(self) -> None:
-        self.table_data = pd.read_csv(self.file_path, index_col="Setting")
-
-    def update_settings_parameters(self, interferometer: algorithm.interferometry.Interferometer):
-        self.table_data.loc["Output Phases [deg]"] = np.rad2deg(interferometer.output_phases)
-        self.table_data.loc["Amplitude [V]"] = interferometer.amplitudes
-        self.table_data.loc["Offset [V]"] = interferometer.offsets
-
-    def update_settings_paths(self, interferometer: algorithm.interferometry.Interferometer,
-                              inversion: algorithm.pti.Inversion) -> None:
-        interferometer.settings_path = self.file_path
-        inversion.settings_path = self.file_path
-        interferometer.load_settings()
-        inversion.load_response_phase()
-
-    def setup_settings_file(self) -> None:
-        # If no settings found, a new empty file is created filled with NaN.
-        algorithm_dir: str = f"{os.path.dirname(os.path.dirname(__file__))}/algorithm"
-        if not os.path.exists(f"{algorithm_dir}/configs/settings.csv"):
-            self.save()
-        else:
-            try:
-                settings = pd.read_csv(f"{algorithm_dir}/configs/settings.csv", index_col="Setting")
-            except FileNotFoundError:
-                self.save()
-            else:
-                if list(settings.columns) != SettingsTable.HEADERS or list(
-                        settings.index) != SettingsTable.INDEX:
-                    self.save()  # The file is in any way broken.
-                else:
-                    self.table_data = settings
-
-
-class Logging(logging.Handler):
-    LOGGING_HISTORY = 50
-
-    def __init__(self):
-        logging.Handler.__init__(self)
-        self.logging_messages = deque(maxlen=Logging.LOGGING_HISTORY)
-        self.formatter = logging.Formatter('%(levelname)s %(asctime)s: %(message)s\n',
-                                           datefmt='%Y-%m-%d %H:%M:%S')
-        logging.getLogger().addHandler(self)
-
-    def emit(self, record: logging.LogRecord) -> None:
-        log = self.format(record)
-        if "ERROR" in log:
-            log = f"<p style='color:red'>{log}</p>"
-        elif "INFO" in log:
-            log = f"<p style='color:green'>{log}</p>"
-        elif "WARNING" in log:
-            log = f"<p style='color:orange'>{log}</p>"
-        elif "DEBUG" in log:
-            log = f"<p style='color:blue'>{log}</p>"
-        elif "CRITICAL" in log:
-            log = f"<b><p style='color:darkred'>{log}</p></b>"
-        self.logging_messages.append(log)
-        signals.logging_update.emit(self.logging_messages)
-
-
-def find_delimiter(file_path: str) -> typing.Union[str, None]:
-    delimiter_sniffer = csv.Sniffer()
-    if not file_path:
-        return
-    with open(file_path, "r") as file:
-        delimiter = str(delimiter_sniffer.sniff(file.readline()).delimiter)
-    return delimiter
-
-
-def running_average(data, mean_size: int) -> list[float]:
-    i = 1
-    current_mean = data[0]
-    result = [current_mean]
-    while i < Calculation.MEAN_INTERVAL and i < len(data):
-        current_mean += data[i]
-        result.append(current_mean / i)
-        i += 1
-    result.extend(ndimage.uniform_filter1d(data[mean_size:], size=mean_size))
-    return result
-
-
-class Buffer:
-    """
-    The buffer contains the queues for incoming data and the timer for them.
-    """
-    QUEUE_SIZE = 1000
-
-    def __init__(self):
-        self.time_counter = itertools.count()
-        self.time = deque(maxlen=Buffer.QUEUE_SIZE)
-
-    def __getitem__(self, key):
-        return getattr(self, key.casefold().replace(" ", "_"))
-
-    def __setitem__(self, key, value) -> None:
-        setattr(self, key.casefold().replace(" ", "_"), value)
-
-    def __iter__(self):
-        for member in dir(self):
-            if not callable(getattr(self, member)) and not member.startswith(
-                    "__") and member != "time_counter":
-                yield getattr(self, member)
-
-    @abc.abstractmethod
-    def append(self, *args: typing.Any) -> None:
-        ...
-
-    def clear(self) -> None:
-        for member in dir(self):
-            if not callable(getattr(self, member)) and not member.startswith("__"):
-                if member == self.time_counter:
-                    self.time_counter = itertools.count()  # Reset counter
-                else:
-                    setattr(self, member, deque(maxlen=Buffer.QUEUE_SIZE))
-
-
-class PTI(typing.NamedTuple):
-    decimation: algorithm.pti.Decimation
-    inversion: algorithm.pti.Inversion
-
-
-class Interferometry(typing.NamedTuple):
-    interferometer: algorithm.interferometry.Interferometer
-    characterization: algorithm.interferometry.Characterization
-
-
-class PTIBuffer(Buffer):
-    MEAN_SIZE = 60
-    CHANNELS = 3
-
-    def __init__(self):
-        Buffer.__init__(self)
-        self.dc_values = [deque(maxlen=Buffer.QUEUE_SIZE) for _ in range(PTIBuffer.CHANNELS)]
-        self.interferometric_phase = deque(maxlen=Buffer.QUEUE_SIZE)
-        self.sensitivity = [deque(maxlen=Buffer.QUEUE_SIZE) for _ in range(PTIBuffer.CHANNELS)]
-        self.pti_signal = deque(maxlen=Buffer.QUEUE_SIZE)
-        self.pti_signal_mean = deque(maxlen=Buffer.QUEUE_SIZE)
-        self._pti_signal_mean_queue = deque(maxlen=PTIBuffer.MEAN_SIZE)
-
-    def append(self, pti_data: PTI, interferometer: algorithm.interferometry.Interferometer) -> None:
-        for i in range(3):
-            self.dc_values[i].append(pti_data.decimation.dc_signals[i])
-            self.sensitivity[i].append(pti_data.inversion.sensitivity[i])
-        self.interferometric_phase.append(interferometer.phase)
-        self.pti_signal.append(pti_data.inversion.pti_signal)
-        self._pti_signal_mean_queue.append(pti_data.inversion.pti_signal)
-        self.pti_signal_mean.append(np.mean(self._pti_signal_mean_queue))
-        self.time.append(next(self.time_counter))
-
-
-class CharacterisationBuffer(Buffer):
-    CHANNELS = 3
-
-    def __init__(self):
-        Buffer.__init__(self)
-        # The first channel has always the phase 0 by definition hence it is not needed.
-        self.output_phases = [deque(maxlen=Buffer.QUEUE_SIZE) for _ in range(self.CHANNELS - 1)]
-        self.amplitudes = [deque(maxlen=Buffer.QUEUE_SIZE) for _ in range(CharacterisationBuffer.CHANNELS)]
-        self.symmetry = deque(maxlen=Buffer.QUEUE_SIZE)
-        self.relative_symmetry = deque(maxlen=Buffer.QUEUE_SIZE)
-
-    def append(self, characterization: algorithm.interferometry.Characterization,
-               interferometer: algorithm.interferometry.Interferometer) -> None:
-        for i in range(3):
-            self.amplitudes[i].append(interferometer.amplitudes[i])
-        for i in range(2):
-            self.output_phases[i].append(interferometer.output_phases[i + 1])
-        self.symmetry.append(interferometer.absoloute_symmetry)
-        self.relative_symmetry.append(interferometer.relative_symmetry)
-        self.time.append(characterization.time_stamp)
-
-
-class LaserBuffer(Buffer):
-    def __init__(self):
-        Buffer.__init__(self)
-        self.pump_laser_voltage = deque(maxlen=Buffer.QUEUE_SIZE)
-        self.pump_laser_current = deque(maxlen=Buffer.QUEUE_SIZE)
-        self.probe_laser_current = deque(maxlen=Buffer.QUEUE_SIZE)
-
-    def append(self, laser_data: hardware.laser.Data) -> None:
-        self.time.append(next(self.time_counter) / 10)
-        self.pump_laser_current.append(laser_data.pump_laser_current)
-        self.pump_laser_voltage.append(laser_data.pump_laser_voltage)
-        self.probe_laser_current.append(laser_data.probe_laser_current)
-
-
-class TecBuffer(Buffer):
-    PUMP_LASER = hardware.tec.Driver.PUMP_LASER
-    PROBE_LASER = hardware.tec.Driver.PROBE_LASER
-
-    def __init__(self):
-        Buffer.__init__(self)
-        self.set_point: list[deque] = [deque(maxlen=Buffer.QUEUE_SIZE),
-                                       deque(maxlen=Buffer.QUEUE_SIZE)]
-        self.actual_value: list[deque] = [deque(maxlen=Buffer.QUEUE_SIZE),
-                                          deque(maxlen=Buffer.QUEUE_SIZE)]
-
-    def append(self, tec_data: hardware.tec.Data) -> None:
-        self.set_point[TecBuffer.PUMP_LASER].append(tec_data.set_point.pump_laser)
-        self.set_point[TecBuffer.PROBE_LASER].append(tec_data.set_point.probe_laser)
-        self.actual_value[TecBuffer.PUMP_LASER].append(tec_data.actual_temperature.pump_laser)
-        self.actual_value[TecBuffer.PROBE_LASER].append(tec_data.actual_temperature.probe_laser)
-        self.time.append(next(self.time_counter) / 10)
-
-
-class Mode(enum.IntEnum):
-    DISABLED = 0
-    CONTINUOUS_WAVE = 1
-    PULSED = 2
-
-
-@dataclass
-class Battery:
-    percentage: int
-    minutes_left: int
-
-
-@dataclass(init=False, frozen=True)
-class Signals(QtCore.QObject):
-    decimation = QtCore.pyqtSignal(pd.DataFrame)
-    decimation_live = QtCore.pyqtSignal(Buffer)
-    inversion = QtCore.pyqtSignal(pd.DataFrame)
-    inversion_live = QtCore.pyqtSignal(Buffer)
-    characterization = QtCore.pyqtSignal(pd.DataFrame)
-    characterization_live = QtCore.pyqtSignal(Buffer)
-    settings_pti = QtCore.pyqtSignal()
-    logging_update = QtCore.pyqtSignal(deque)
-    daq_running = QtCore.pyqtSignal()
-    settings = QtCore.pyqtSignal(algorithm.interferometry.Interferometer)
-    destination_folder_changed = QtCore.pyqtSignal(str)
-    battery_state = QtCore.pyqtSignal(Battery)
-    valve_change = QtCore.pyqtSignal(hardware.motherboard.Valve)
-    bypass = QtCore.pyqtSignal(bool)
-    tec_data = QtCore.pyqtSignal(Buffer)
-    tec_data_display = QtCore.pyqtSignal(hardware.tec.Data)
-
-    def __init__(self):
-        QtCore.QObject.__init__(self)
-
-
-@dataclass
-class LaserSignals(QtCore.QObject):
-    photo_gain = QtCore.pyqtSignal(int)
-    current_probe_laser = QtCore.pyqtSignal(int, float)
-    max_current_probe_laser = QtCore.pyqtSignal(float)
-    probe_laser_mode = QtCore.pyqtSignal(int)
-    laser_voltage = QtCore.pyqtSignal(int, float)
-    current_dac = QtCore.pyqtSignal(int, int)
-    matrix_dac = QtCore.pyqtSignal(int, list)
-    data = QtCore.pyqtSignal(Buffer)
-    data_display = QtCore.pyqtSignal(hardware.laser.Data)
-    pump_laser_enabled = QtCore.pyqtSignal(bool)
-    probe_laser_enabled = QtCore.pyqtSignal(bool)
-
-    def __init__(self):
-        QtCore.QObject.__init__(self)
-
-
-class TecMode(enum.IntEnum):
-    COOLING = 0
-    HEATING = 1
-
-
-@dataclass(init=False, frozen=True)
-class TecSignals(QtCore.QObject):
-    mode = QtCore.pyqtSignal(TecMode)
-    p_value = QtCore.pyqtSignal(float)
-    d_value = QtCore.pyqtSignal(float)
-    i_1_value = QtCore.pyqtSignal(float)
-    i_2_value = QtCore.pyqtSignal(float)
-    setpoint_temperature = QtCore.pyqtSignal(float)
-    loop_time = QtCore.pyqtSignal(float)
-    reference_resistor = QtCore.pyqtSignal(float)
-    max_power = QtCore.pyqtSignal(float)
-    enabled = QtCore.pyqtSignal(bool)
-
-    def __init__(self):
-        QtCore.QObject.__init__(self)
-
-
-def shutdown_procedure() -> None:
-    Motherboard.driver.close()
-    Laser.driver.close()
-    Tec.driver.close()
-    time.sleep(0.5)  # Give the calculations threads time to finish their write operation
-    if platform.system() == "Windows":
-        subprocess.run(r"shutdown /s /t 1", shell=True)
-    else:
-        subprocess.run("sleep 0.5s && echo poweroff", shell=True)
-
-
-class Calculation:
-    MEAN_INTERVAL = 60
-
-    def __init__(self, queue_size=1000):
-        self.settings_path = ""
-        self.queue_size = queue_size
-        self.dc_signals = []
-        self.pti_buffer = PTIBuffer()
-        self.characterisation_buffer = CharacterisationBuffer()
-        self.pti_signal_mean_queue = deque(maxlen=60)
-        self.current_time = 0
-        self.interferometry = Interferometry(algorithm.interferometry.Interferometer(),
-                                             algorithm.interferometry.Characterization())
-        self.interferometry.characterization.interferometer = self.interferometry.interferometer
-        self.pti = PTI(algorithm.pti.Decimation(),
-                       algorithm.pti.Inversion(interferometer=self.interferometry.interferometer))
-        self.interferometry.characterization.interferometer = self.interferometry.interferometer
-        self._destination_folder = os.getcwd()
-        self.save_raw_data = False
-
-    def set_raw_data_saving(self) -> None:
-        if self.save_raw_data:
-            self.pti.decimation.save_raw_data = False
-        else:
-            self.pti.decimation.save_raw_data = True
-
-    @property
-    def destination_folder(self) -> str:
-        return self._destination_folder
-
-    @destination_folder.setter
-    def destination_folder(self, folder: str) -> None:
-        self.interferometry.characterization.destination_folder = folder
-        self.pti.inversion.destination_folder = folder
-        self._destination_folder = folder
-        signals.destination_folder_changed.emit(folder)
-
-    def live_calculation(self) -> tuple[threading.Thread, threading.Thread]:
-        self.pti.inversion.init_header = True
-        self.pti.decimation.init_header = True
-        self.interferometry.characterization.init_online = True
-        self.interferometry.interferometer.load_settings()
-
-        def calculate_characterization() -> None:
-            while Motherboard.driver.running.is_set():
-                self.interferometry.characterization.characterise(live=True)
-                self.characterisation_buffer.append(self.interferometry.characterization,
-                                                    self.interferometry.interferometer)
-                signals.characterization_live.emit(self.characterisation_buffer)
-
-        def calculate_inversion():
-            while Motherboard.driver.running.is_set():
-                self.pti.decimation.ref = np.array(Motherboard.driver.ref_signal)
-                self.pti.decimation.dc_coupled = np.array(Motherboard.driver.dc_coupled)
-                self.pti.decimation.ac_coupled = np.array(Motherboard.driver.ac_coupled)
-                self.pti.decimation.decimate(live=True)
-                self.pti.inversion.lock_in = self.pti.decimation.lock_in
-                self.pti.inversion.dc_signals = self.pti.decimation.dc_signals
-                signals.decimation_live.emit(self.pti_buffer)
-                self.pti.inversion.invert(live=True)
-                self.interferometry.characterization.add_phase(self.interferometry.interferometer.phase)
-                self.dc_signals.append(copy.deepcopy(self.pti.decimation.dc_signals))
-                if self.interferometry.characterization.enough_values:
-                    self.interferometry.characterization._signals = copy.deepcopy(self.dc_signals)
-                    self.interferometry.characterization.phases = copy.deepcopy(
-                        self.interferometry.characterization.tracking_phase)
-                    self.interferometry.characterization.event.set()
-                    self.dc_signals = []
-                self.pti_buffer.append(self.pti, self.interferometry.interferometer)
-                signals.inversion_live.emit(self.pti_buffer)
-
-        characterization_thread = threading.Thread(target=calculate_characterization, daemon=True)
-        inversion_thread = threading.Thread(target=calculate_inversion, daemon=True)
-        characterization_thread.start()
-        inversion_thread.start()
-        return characterization_thread, inversion_thread
-
-    def calculate_characterisation(self, dc_file_path: str, use_settings=False, settings_path="") -> None:
-        self.interferometry.interferometer.decimation_filepath = dc_file_path
-        self.interferometry.interferometer.settings_path = settings_path
-        self.interferometry.characterization.use_settings = use_settings
-        self.interferometry.characterization.characterise()
-        signals.settings.emit(self.interferometry.interferometer)
-
-    def calculate_decimation(self, decimation_path: str) -> None:
-        self.pti.decimation.file_path = decimation_path
-        self.pti.decimation.decimate()
-
-    def calculate_inversion(self, settings_path: str, inversion_path: str) -> None:
-        self.interferometry.interferometer.decimation_filepath = inversion_path
-        self.interferometry.interferometer.settings_path = settings_path
-        self.interferometry.interferometer.load_settings()
-        self.pti.inversion.invert()
-
-    @staticmethod
-    def kelvin_to_celsius(temperature: float) -> float:
-        return temperature - 273.15
-
-    def process_bms_data(self) -> None:
-        units = {"Date": "Y:M:D", "Time": "H:M:S", "External DC Power": "bool",
-                 "Charging Battery": "bool",
-                 "Minutes Left": "min", "Charging Level": "%", "Temperature": "°C", "Current": "mA",
-                 "Voltage": "V", "Full Charge Capacity": "mAh", "Remaining Charge Capacity": "mAh"}
-        pd.DataFrame(units).to_csv(self._destination_folder + "/BMS.csv")
-
-        def incoming_data() -> None:
-            while Motherboard.driver.running.is_set():
-                bms_data: hardware.motherboard.BMSData = Motherboard.driver.bms
-                bms_data.battery_temperature = Calculation.kelvin_to_celsius(
-                    bms_data.battery_temperature)
-                signals.battery_state.emit(Battery(bms_data.battery_percentage, bms_data.minutes_left))
-                now = datetime.now()
-                output_data = {"Date": str(now.strftime("%Y-%m-%d")),
-                               "Time": str(now.strftime("%H:%M:%S"))}
-                for key, value in asdict(bms_data).values():
-                    output_data[key.replace("_", " ").title()] = value
-                pd.DataFrame(output_data).to_csv(self._destination_folder + "/BMS.csv",
-                                                 header=False, mode="a")
-        threading.Thread(target=incoming_data).start()
-
-
-class ProbeLaserMode(enum.IntEnum):
-    CONSTANT_LIGHT = 0
-    CONSTANT_CURRENT = 1
-
-
-class Serial:
-    """
-    This class is a base class for subclasses of the driver objects from driver/serial.
-    """
-
-    driver = hardware.serial_device.Driver()
-
-    @classmethod
-    def find_port(cls) -> None:
-        cls.driver.find_port()
-
-    @classmethod
-    def open(cls) -> None:
-        """
-        Connects to a serial device and listens to incoming data.
-        """
-        cls.driver.open()
-
-    @classmethod
-    def close(cls) -> None:
-        """
-        Disconnects to a serial device and stops listening to data
-        """
-        cls.driver.close()
-
-    @staticmethod
-    @abc.abstractmethod
-    def save_configuration() -> None:
-        ...
-
-    @abc.abstractmethod
-    def fire_configuration_change(self) -> None:
-        """
-        By initiation of a Serial Object (on which the laser model relies) the configuration is
-        already set and do not fire events to update the GUI. This function is hence only called
-        once to manually activate the firing.
-        """
-
-    @abc.abstractmethod
-    def load_configuration(self) -> None:
-        self.fire_configuration_change()
-
-    @staticmethod
-    def _incoming_data() -> None:
-        """
-        Listens to incoming data and emits them as _signals to the view as long a serial connection
-        is established.
-        """
-
-    @staticmethod
-    def process_measured_data() -> threading.Thread:
-        processing_thread = threading.Thread(target=Serial._incoming_data, daemon=True)
-        processing_thread.start()
-        return processing_thread
-
-
-class Motherboard(Serial):
-    driver = hardware.motherboard.Driver()
-
-    def __init__(self):
-        Serial.__init__(self)
-        self.bms_data: tuple[float, float] = (0, 0)
-
-    @property
-    def connected(self) -> bool:
-        return self.driver.connected.is_set()
-
-    @classmethod
-    def open(cls) -> None:
-        cls.driver.open()
-        cls.driver.run()
-
-    def run(self) -> bool:
-        if not self.driver.connected.is_set():
-            return False
-        self.driver.reset()
-        self.driver.running.set()
-        return True
-
-    def stop(self) -> None:
-        self.driver.running.clear()
-
-    @property
-    def shutdown_event(self) -> threading.Event:
-        return self.driver.shutdown
-
-    @property
-    def valve_period(self) -> int:
-        return self.driver.config.valve.period
-
-    @valve_period.setter
-    def valve_period(self, period: int) -> None:
-        if period < 0:
-            raise ValueError("Invalid value for period")
-        self.driver.config.valve.period = period
-
-    @property
-    def valve_duty_cycle(self) -> int:
-        return self.driver.config.valve.duty_cycle
-
-    @valve_duty_cycle.setter
-    def valve_duty_cycle(self, duty_cycle: int) -> None:
-        if not 0 < self.driver.config.valve.duty_cycle < 100:
-            raise ValueError("Invalid value for duty cycle")
-        self.driver.config.valve.duty_cycle = duty_cycle
-
-    @property
-    def automatic_valve_switch(self) -> bool:
-        return self.driver.config.valve.automatic_switch
-
-    @automatic_valve_switch.setter
-    def automatic_valve_switch(self, automatic_switch: bool) -> None:
-        self.driver.config.valve.automatic_switch = automatic_switch
-        if automatic_switch:
-            self.driver.automatic_switch.set()
-            self.driver.automatic_valve_change()
-        else:
-            self.driver.automatic_switch.clear()
-
-    @property
-    def bypass(self) -> bool:
-        return self.driver.bypass
-
-    @bypass.setter
-    def bypass(self, state: bool) -> None:
-        self.driver.bypass = state
-        signals.bypass.emit(state)
-
-    def load_configuration(self) -> None:
-        Motherboard.driver.load_config()
-        self.fire_configuration_change()
-
-    @staticmethod
-    def save_configuration() -> None:
-        Motherboard.driver.save_config()
-
-    @property
-    def config_path(self) -> str:
-        return self.driver.config_path
-
-    @config_path.setter
-    def config_path(self, config_path: str) -> None:
-        if not os.path.exists(config_path):
-            raise ValueError("File does not exist")
-        self.driver.config_path = config_path
-
-    def fire_configuration_change(self) -> None:
-        signals.valve_change.emit(Motherboard.driver.config.valve)
-
-
-class Laser(Serial):
-    buffer = LaserBuffer()
-    driver = hardware.laser.Driver()
-
-    def __init__(self):
-        Serial.__init__(self)
-        self.config_path = "hardware/configs/laser.json"
-
-    def load_configuration(self) -> None:
-        Laser.driver.load_configuration()
-        self.fire_configuration_change()
-
-    @staticmethod
-    def save_configuration() -> None:
-        Laser.driver.save_configuration()
-
-    @staticmethod
-    def apply_configuration() -> None:
-        Laser.driver.apply_configuration()
-
-    @staticmethod
-    def _incoming_data():
-        while Laser.driver.running.is_set():
-            received_data = Laser.driver.data.get(block=True)
-            Laser.buffer.append(received_data)
-            laser_signals.data.emit(Laser.buffer)
-            laser_signals.data_display.emit(received_data)
-
-    def fire_configuration_change(self) -> None:
-        ...
-
-
-class PumpLaser(Laser):
-    def __init__(self):
-        Laser.__init__(self)
-
-    @property
-    def connected(self) -> bool:
-        return self.driver.connected.is_set()
-
-    @property
-    def driver_bits(self) -> int:
-        return self.driver.pump_laser.bit_value
-
-    @driver_bits.setter
-    def driver_bits(self, bits: int) -> None:
-        # With increasing the slider decreases its value but the voltage should increase
-        # - hence we subtract the bits.
-        self.driver.pump_laser.bit_value = hardware.laser.PumpLaser.NUMBER_OF_STEPS - bits
-        self.fire_driver_bits_signal()
-        self.driver.set_driver_voltage()
-
-    def fire_driver_bits_signal(self) -> None:
-        bits: int = self.driver.pump_laser.bit_value
-        voltage: float = hardware.laser.PumpLaser.bit_to_voltage(bits)
-        bits = hardware.laser.PumpLaser.NUMBER_OF_STEPS - bits
-        laser_signals.laser_voltage.emit(bits, voltage)
-
-    @property
-    def enabled(self) -> bool:
-        return self.driver.pump_laser_enabled
-
-    @enabled.setter
-    def enabled(self, state: bool):
-        self.driver.pump_laser_enabled = state
-        laser_signals.pump_laser_enabled.emit(state)
-
-    @property
-    def current_bits_dac_1(self) -> int:
-        return self.driver.pump_laser.DAC_1.bit_value
-
-    @current_bits_dac_1.setter
-    def current_bits_dac_1(self, bits: int) -> None:
-        self.driver.pump_laser.DAC_1.bit_value = bits
-        self.fire_current_bits_dac_1()
-        self.driver.set_dac_1()
-
-    def fire_current_bits_dac_1(self) -> None:
-        laser_signals.current_dac.emit(0, self.driver.pump_laser.DAC_1.bit_value)
-
-    @property
-    def current_bits_dac_2(self) -> int:
-        return self.driver.pump_laser.DAC_2.bit_value
-
-    @current_bits_dac_2.setter
-    def current_bits_dac_2(self, bits: int) -> None:
-        self.driver.pump_laser.DAC_2.bit_value = bits
-        self.fire_current_bits_dac2()
-        self.driver.set_dac_2()
-
-    def fire_current_bits_dac2(self) -> None:
-        laser_signals.current_dac.emit(1, self.driver.pump_laser.DAC_2.bit_value)
-
-    @property
-    def dac_1_matrix(self) -> hardware.laser.DAC:
-        return self.driver.pump_laser.DAC_1
-
-    @property
-    def dac_2_matrix(self) -> hardware.laser.DAC:
-        return self.driver.pump_laser.DAC_2
-
-    @staticmethod
-    def _set_indices(dac_number: int, dac: hardware.laser.DAC) -> None:
-        indices: typing.Annotated[list[int], 3] = []
-        for i in range(3):
-            if dac.continuous_wave[i]:
-                indices.append(Mode.CONTINUOUS_WAVE)
-            elif dac.pulsed_mode[i]:
-                indices.append(Mode.PULSED)
-            else:
-                indices.append(Mode.DISABLED)
-        laser_signals.matrix_dac.emit(dac_number, indices)
-
-    @dac_1_matrix.setter
-    def dac_1_matrix(self, dac: hardware.laser.DAC) -> None:
-        self.driver.pump_laser.DAC_1 = dac
-        self.fire_dac_matrix_1()
-
-    def fire_dac_matrix_1(self) -> None:
-        PumpLaser._set_indices(dac_number=0, dac=self.dac_1_matrix)
-
-    @dac_2_matrix.setter
-    def dac_2_matrix(self, dac: hardware.laser.DAC) -> None:
-        self.driver.pump_laser.DAC_2 = dac
-        self.fire_dac_matrix_2()
-
-    def fire_dac_matrix_2(self) -> None:
-        PumpLaser._set_indices(dac_number=1, dac=self.dac_2_matrix)
-
-    def update_dac_mode(self, dac: hardware.laser.DAC, channel: int, mode: int) -> None:
-        if mode == Mode.CONTINUOUS_WAVE:
-            dac.continuous_wave[channel] = True
-            dac.pulsed_mode[channel] = False
-        elif mode == Mode.PULSED:
-            dac.continuous_wave[channel] = False
-            dac.pulsed_mode[channel] = True
-        elif mode == Mode.DISABLED:
-            dac.continuous_wave[channel] = False
-            dac.pulsed_mode[channel] = False
-        self.driver.set_dac_matrix()
-
-    def fire_configuration_change(self) -> None:
-        self.fire_driver_bits_signal()
-        self.fire_current_bits_dac_1()
-        self.fire_current_bits_dac2()
-        self.fire_dac_matrix_1()
-        self.fire_dac_matrix_2()
-
-
-class ProbeLaser(Laser):
-    def __init__(self):
-        Laser.__init__(self)
-
-    @property
-    def connected(self) -> bool:
-        return self.driver.connected.is_set()
-
-    @property
-    def current_bits_probe_laser(self) -> int:
-        return self.driver.probe_laser.current_bits
-
-    @current_bits_probe_laser.setter
-    def current_bits_probe_laser(self, bits: int) -> None:
-        self.driver.probe_laser.current_bits = bits
-        bit, current = self.fire_current_bits_signal()
-        laser_signals.current_probe_laser.emit(hardware.laser.Driver.CURRENT_BITS - bits, current)
-        self.driver.set_probe_laser_current()
-
-    def fire_current_bits_signal(self) -> tuple[int, float]:
-        bits: int = self.driver.probe_laser.current_bits
-        current: float = hardware.laser.ProbeLaser.bit_to_current(bits)
-        laser_signals.current_probe_laser.emit(hardware.laser.Driver.CURRENT_BITS - bits, current)
-        return bits, current
-
-    @property
-    def enabled(self) -> bool:
-        return self.driver.probe_laser_enabled
-
-    @enabled.setter
-    def enabled(self, state: bool) -> None:
-        self.driver.probe_laser_enabled = state
-        laser_signals.probe_laser_enabled.emit(state)
-
-    @property
-    def photo_diode_gain(self) -> int:
-        return self.driver.probe_laser.photo_diode_gain
-
-    @photo_diode_gain.setter
-    def photo_diode_gain(self, photo_diode_gain: int) -> None:
-        self.driver.probe_laser.photo_diode_gain = photo_diode_gain
-        self.fire_photo_diode_gain_signal()
-        self.driver.set_photo_gain()
-
-    def fire_photo_diode_gain_signal(self) -> None:
-        laser_signals.photo_gain.emit(self.driver.probe_laser.photo_diode_gain - 1)
-
-    @property
-    def probe_laser_max_current(self) -> float:
-        return self.driver.probe_laser.max_current_mA
-
-    @probe_laser_max_current.setter
-    def probe_laser_max_current(self, current: float) -> None:
-        if self.driver.probe_laser.max_current_mA != current:
-            self.driver.probe_laser.max_current_mA = current
-            self.fire_max_current_signal()
-
-    def fire_max_current_signal(self) -> None:
-        laser_signals.max_current_probe_laser.emit(self.driver.probe_laser.max_current_mA)
-
-    @property
-    def probe_laser_mode(self) -> ProbeLaserMode:
-        if self.driver.probe_laser.constant_light:
-            return ProbeLaserMode.CONSTANT_LIGHT
-        else:
-            return ProbeLaserMode.CONSTANT_CURRENT
-
-    @probe_laser_mode.setter
-    def probe_laser_mode(self, mode: ProbeLaserMode) -> None:
-        if mode == ProbeLaserMode.CONSTANT_CURRENT:
-            self.driver.probe_laser.constant_current = True
-            self.driver.probe_laser.constant_light = False
-        elif mode == ProbeLaserMode.CONSTANT_LIGHT:
-            self.driver.probe_laser.constant_current = False
-            self.driver.probe_laser.constant_light = True
-        self.driver.set_probe_laser_mode()
-        self.fire_laser_mode_signal()
-
-    def fire_laser_mode_signal(self) -> None:
-        if self.driver.probe_laser.constant_light:
-            laser_signals.probe_laser_mode.emit(ProbeLaserMode.CONSTANT_LIGHT)
-        else:
-            laser_signals.probe_laser_mode.emit(ProbeLaserMode.CONSTANT_CURRENT)
-
-    def fire_configuration_change(self) -> None:
-        self.fire_current_bits_signal()
-        self.fire_laser_mode_signal()
-        self.fire_photo_diode_gain_signal()
-        self.fire_max_current_signal()
-
-
-class Tec(Serial):
-    driver = hardware.tec.Driver()
-    _buffer = TecBuffer()
-
-    def __init__(self, laser: str):
-        Serial.__init__(self)
-        self.laser = laser
-
-    @property
-    def connected(self) -> bool:
-        return self.driver.connected.is_set()
-
-    @property
-    def enabled(self) -> bool:
-        if self.laser == "Pump Laser":
-            return self.driver.pump_laser_enabled
-        else:
-            return self.driver.probe_laser_enabled
-
-    @enabled.setter
-    def enabled(self, state) -> None:
-        if self.laser == "Pump Laser":
-            self.driver.pump_laser_enabled = state
-            tec_signals["Pump Laser"].enabled.emit(state)
-        else:
-            self.driver.probe_laser_enabled = state
-            tec_signals["Probe Laser"].enabled.emit(state)
-
-    @property
-    def config_path(self) -> str:
-        return Tec.driver.config_path
-
-    @config_path.setter
-    def config_path(self, config_path: str) -> None:
-        Tec.driver.config_path = config_path
-
-    @staticmethod
-    def save_configuration() -> None:
-        Tec.driver.save_configuration()
-
-    def load_configuration(self) -> None:
-        Tec.driver.load_config()
-        self.fire_configuration_change()
-
-    @staticmethod
-    def apply_configuration() -> None:
-        Tec.driver.apply_configuration()
-
-    @property
-    def p_value(self) -> float:
-        return self.driver[self.laser].pid.proportional_value
-
-    @p_value.setter
-    def p_value(self, p_value: float) -> None:
-        self.driver[self.laser].pid.proportional_value = p_value
-        self.driver.set_pid_p_value(self.laser)
-
-    @property
-    def i_1_value(self) -> float:
-        return self.driver[self.laser].pid.integral_value[0]
-
-    @i_1_value.setter
-    def i_1_value(self, i_value: float) -> None:
-        self.driver[self.laser].pid.integral_value[0] = i_value
-        self.driver.set_pid_i_value(self.laser, 0)
-
-    @property
-    def i_2_value(self) -> float:
-        return self.driver[self.laser].pid.integral_value[1]
-
-    @i_2_value.setter
-    def i_2_value(self, i_value: float) -> None:
-        self.driver[self.laser].pid.integral_value[1] = i_value
-        self.driver.set_pid_i_value(self.laser, 1)
-
-    @property
-    def d_value(self) -> float:
-        return self.driver[self.laser].pid.derivative_value
-
-    @d_value.setter
-    def d_value(self, d_value: float) -> None:
-        self.driver[self.laser].pid.derivative_value = d_value
-        self.driver.set_pid_d_value(self.laser)
-
-    @property
-    def setpoint_temperature(self) -> float:
-        return self.driver[self.laser].system_parameter.setpoint_temperature
-
-    @setpoint_temperature.setter
-    def setpoint_temperature(self, setpoint_temperature: float) -> None:
-        self.driver[self.laser].system_parameter.setpoint_temperature = setpoint_temperature
-        self.driver.set_setpoint_temperature_value(self.laser)
-
-    @property
-    def loop_time(self) -> float:
-        return self.driver[self.laser].system_parameter.loop_time
-
-    @loop_time.setter
-    def loop_time(self, loop_time: float) -> None:
-        self.driver[self.laser].system_parameter.loop_time = loop_time
-        self.driver.set_loop_time_value(self.laser)
-
-    @property
-    def reference_resistor(self) -> float:
-        return self.driver[self.laser].system_parameter.reference_resistor
-
-    @reference_resistor.setter
-    def reference_resistor(self, reference_resistor: float) -> None:
-        self.driver[self.laser].system_parameter.reference_resistor = reference_resistor
-        self.driver.set_reference_resistor_value(self.laser)
-
-    @property
-    def max_power(self) -> float:
-        return self.driver[self.laser].system_parameter.reference_resistor
-
-    @max_power.setter
-    def max_power(self, max_power: float) -> None:
-        self.driver[self.laser].system_parameter.reference_resistor = max_power
-        self.driver.set_max_power_value(self.laser)
-
-    @property
-    def cooling(self) -> bool:
-        return self.driver[self.laser].mode.cooling
-
-    @cooling.setter
-    def cooling(self, mode: bool) -> None:
-        if mode:
-            self.driver[self.laser].mode.heating = False
-            self.driver[self.laser].mode.cooling = True
-            tec_signals[self.laser].mode.emit(TecMode.COOLING)
-            self.driver.set_mode(self.laser)
-        else:
-            self.driver[self.laser].mode.cooling = False
-            tec_signals[self.laser].mode.emit(TecMode.HEATING)
-            self.driver.set_mode(self.laser)
-
-    @property
-    def heating(self) -> bool:
-        return self.driver[self.laser].mode.heating
-
-    @heating.setter
-    def heating(self, mode: bool) -> None:
-        if mode:
-            self.driver[self.laser].mode.heating = True
-            self.driver[self.laser].mode.cooling = False
-            tec_signals[self.laser].mode.emit(TecMode.HEATING)
-            self.driver.set_mode(self.laser)
-        else:
-            self.driver[self.laser].mode.heating = False
-            tec_signals[self.laser].mode.emit(TecMode.COOLING)
-            self.driver.set_mode(self.laser)
-
-    def fire_configuration_change(self) -> None:
-        tec_signals[self.laser].d_value.emit(self.d_value)
-        tec_signals[self.laser].p_value.emit(self.p_value)
-        tec_signals[self.laser].i_1_value.emit(self.i_2_value)
-        tec_signals[self.laser].i_2_value.emit(self.i_2_value)
-        tec_signals[self.laser].setpoint_temperature.emit(self.setpoint_temperature)
-        tec_signals[self.laser].loop_time.emit(self.loop_time)
-        tec_signals[self.laser].reference_resistor.emit(self.reference_resistor)
-        tec_signals[self.laser].max_power.emit(self.max_power)
-        if self.cooling:
-            tec_signals[self.laser].mode.emit(TecMode.COOLING)
-        else:
-            tec_signals[self.laser].mode.emit(TecMode.HEATING)
-
-    def _incoming_data(self) -> None:
-        while self.driver.connected.is_set():
-            received_data = Tec.driver.data.get(block=True)
-            Tec._buffer.append(received_data)
-            signals.tec_data.emit(Tec._buffer)
-            signals.tec_data_display.emit(received_data)
-
-
-def _process_data(file_path: str, headers: list[str, ...]) -> pd.DataFrame:
-    if not file_path:
-        raise FileNotFoundError("No file path given")
-    delimiter = find_delimiter(file_path)
-    try:
-        data = pd.read_csv(file_path, delimiter=delimiter, skiprows=[1], index_col="Time")
-    except ValueError:
-        try:
-            data = pd.read_csv(file_path, delimiter=delimiter, skiprows=[1], index_col="Time Stamp")
-        except ValueError:  # Data isn't saved with any index
-            data = pd.read_csv(file_path, delimiter=delimiter, skiprows=[1])
-    for header in headers:
-        for header_data in data.columns:
-            if header == header_data:
-                break
-        else:
-            raise KeyError(f"Header {header} not found in file")
-    return data
-
-
-def process_dc_data(dc_file_path: str) -> None:
-    headers = [f"DC CH{i}" for i in range(1, 4)]
-    try:
-        data = _process_data(dc_file_path, headers)
-    except KeyError:
-        headers = [f"PD{i}" for i in range(1, 4)]
-        data = _process_data(dc_file_path, headers)
-    except FileNotFoundError:
-        return
-    signals.decimation.emit(data)
-
-
-def process_inversion_data(inversion_file_path: str) -> None:
-    try:
-        headers = ["Interferometric Phase", "Sensitivity CH1", "Sensitivity CH2", "Sensitivity CH3", "PTI Signal"]
-        data = _process_data(inversion_file_path, headers)
-        data["PTI Signal 60 s Mean"] = running_average(data["PTI Signal"], mean_size=60)
-    except KeyError:
-        headers = ["Sensitivity CH1", "Sensitivity CH2", "Sensitivity CH3", "Interferometric Phase"]
-        data = _process_data(inversion_file_path, headers)
-    except FileNotFoundError:
-        return
-    signals.inversion.emit(data)
-
-
-def process_characterization_data(characterization_file_path: str) -> None:
-    headers = [f"Amplitude CH{i}" for i in range(1, 4)]
-    headers += [f"Output Phase CH{i}" for i in range(1, 4)]
-    headers += [f"Offset CH{i}" for i in range(1, 4)]
-    headers += ["Symmetry", "Relative Symmetry"]
-    try:
-        data = _process_data(characterization_file_path, headers)
-    except FileNotFoundError:
-        return
-    signals.characterization.emit(data)
-
-
-class TecLaserSignals(typing.NamedTuple):
-    probe_laser = TecSignals()
-    pump_laser = TecSignals()
-
-    def __getitem__(self, item) -> TecSignals:
-        if item == "Pump Laser" or item == "Probe Laser":
-            return getattr(self, item.replace(" ", "_").casefold())
-        else:
-            raise KeyError("Can only subscribe Pump Laser or Probe Laser")
-
-
-signals = Signals()
-laser_signals = LaserSignals()
-tec_signals = TecLaserSignals()
+import abc
+import copy
+import csv
+import enum
+import itertools
+import logging
+import os
+import platform
+import subprocess
+import threading
+import time
+import typing
+from typing import Union
+from collections import deque
+from dataclasses import dataclass, asdict
+from datetime import datetime
+
+
+import numpy as np
+import pandas as pd
+from PyQt5 import QtCore
+from scipy import ndimage
+
+from .. import algorithm
+from .. import hardware
+
+
+class DestinationFolder:
+    def __init__(self):
+        self._destination_folder = os.getcwd()
+
+    @property
+    def folder(self) -> str:
+        return self._destination_folder
+
+    @folder.setter
+    def folder(self, folder: str) -> None:
+        self._destination_folder = folder
+        signals.destination_folder_changed.emit(self._destination_folder)
+
+
+class SettingsTable(QtCore.QAbstractTableModel):
+    HEADERS = ["Detector 1", "Detector 2", "Detector 3"]
+    INDEX = ["Amplitude [V]", "Offset [V]", "Output Phases [deg]", "Response Phases [rad]"]
+    SIGNIFICANT_VALUES = 4
+
+    def __init__(self):
+        QtCore.QAbstractTableModel.__init__(self)
+        self._data = pd.DataFrame(columns=SettingsTable.HEADERS, index=SettingsTable.INDEX)
+        self.file_path = f"{os.path.dirname(os.path.dirname(__file__))}/algorithm/configs/settings.csv"
+        self._observer_callbacks = []
+        signals.settings.connect(self.update_settings)
+
+    @QtCore.pyqtSlot(algorithm.interferometry.Interferometer)
+    def update_settings(self, interferometer: algorithm.interferometry.Interferometer) -> None:
+        self.update_settings_parameters(interferometer)
+
+    def rowCount(self, parent=None) -> int:
+        return self._data.shape[0]
+
+    def columnCount(self, parent=None) -> int:
+        return self._data.shape[1]
+
+    def data(self, index, role: int = ...) -> Union[str, None]:
+        if index.isValid():
+            if role == QtCore.Qt.DisplayRole or role == QtCore.Qt.EditRole:
+                value = self._data.at[
+                    SettingsTable.INDEX[index.row()], SettingsTable.HEADERS[index.column()]]
+                return str(round(value, SettingsTable.SIGNIFICANT_VALUES))
+
+    def flags(self, index):
+        return QtCore.Qt.ItemIsSelectable | QtCore.Qt.ItemIsEnabled | QtCore.Qt.ItemIsEditable
+
+    def setData(self, index, value, role: int = ...):
+        if index.isValid():
+            if role == QtCore.Qt.EditRole:
+                self._data.at[SettingsTable.INDEX[index.row()], SettingsTable.HEADERS[
+                    index.column()]] = float(value)
+                return True
+
+    def headerData(self, section, orientation, role=QtCore.Qt.DisplayRole):
+        if orientation == QtCore.Qt.Horizontal and role == QtCore.Qt.DisplayRole:
+            return SettingsTable.HEADERS[section]
+        elif orientation == QtCore.Qt.Vertical and role == QtCore.Qt.DisplayRole:
+            return SettingsTable.INDEX[section]
+        return super().headerData(section, orientation, role)
+
+    @property
+    def table_data(self) -> pd.DataFrame:
+        return self._data
+
+    @table_data.setter
+    def table_data(self, data) -> None:
+        self._data = data
+
+    def save(self) -> None:
+        self._data.to_csv(self.file_path, index_label="Setting", index=True)
+
+    def load(self) -> None:
+        self.table_data = pd.read_csv(self.file_path, index_col="Setting")
+
+    def update_settings_parameters(self, interferometer: algorithm.interferometry.Interferometer):
+        self.table_data.loc["Output Phases [deg]"] = np.rad2deg(interferometer.output_phases)
+        self.table_data.loc["Amplitude [V]"] = interferometer.amplitudes
+        self.table_data.loc["Offset [V]"] = interferometer.offsets
+
+    def update_settings_paths(self, interferometer: algorithm.interferometry.Interferometer,
+                              inversion: algorithm.pti.Inversion) -> None:
+        interferometer.settings_path = self.file_path
+        inversion.settings_path = self.file_path
+        interferometer.load_settings()
+        inversion.load_response_phase()
+
+    def setup_settings_file(self) -> None:
+        # If no settings found, a new empty file is created filled with NaN.
+        algorithm_dir: str = f"{os.path.dirname(os.path.dirname(__file__))}/algorithm"
+        if not os.path.exists(f"{algorithm_dir}/configs/settings.csv"):
+            self.save()
+        else:
+            try:
+                settings = pd.read_csv(f"{algorithm_dir}/configs/settings.csv", index_col="Setting")
+            except FileNotFoundError:
+                self.save()
+            else:
+                if list(settings.columns) != SettingsTable.HEADERS or list(settings.index) != SettingsTable.INDEX:
+                    self.save()  # The file is in any way broken.
+                else:
+                    self.table_data = settings
+
+
+class Logging(logging.Handler):
+    LOGGING_HISTORY = 50
+
+    def __init__(self):
+        logging.Handler.__init__(self)
+        self.logging_messages = deque(maxlen=Logging.LOGGING_HISTORY)
+        self.formatter = logging.Formatter("[%(threadName)s] %(levelname)s %(asctime)s: %(message)s",
+                                           datefmt="%Y-%m-%d %H:%M:%S")
+        logging.getLogger().addHandler(self)
+        root_logger = logging.getLogger()
+        console_handler = logging.StreamHandler()
+        console_handler.setFormatter(self.formatter)
+        root_logger.addHandler(console_handler)
+
+    def emit(self, record: logging.LogRecord) -> None:
+        log = self.format(record)
+        if "ERROR" in log:
+            log = f"<p style='color:red'>{log}</p>"
+        elif "INFO" in log:
+            log = f"<p style='color:green'>{log}</p>"
+        elif "WARNING" in log:
+            log = f"<p style='color:orange'>{log}</p>"
+        elif "DEBUG" in log:
+            log = f"<p style='color:blue'>{log}</p>"
+        elif "CRITICAL" in log:
+            log = f"<b><p style='color:darkred'>{log}</p></b>"
+        self.logging_messages.append(log)
+        signals.logging_update.emit(self.logging_messages)
+
+
+def find_delimiter(file_path: str) -> typing.Union[str, None]:
+    delimiter_sniffer = csv.Sniffer()
+    if not file_path:
+        return
+    with open(file_path, "r") as file:
+        delimiter = str(delimiter_sniffer.sniff(file.readline()).delimiter)
+    return delimiter
+
+
+def running_average(data, mean_size: int) -> list[float]:
+    i = 1
+    current_mean = data[0]
+    result = [current_mean]
+    while i < Calculation.MEAN_INTERVAL and i < len(data):
+        current_mean += data[i]
+        result.append(current_mean / i)
+        i += 1
+    result.extend(ndimage.uniform_filter1d(data[mean_size:], size=mean_size))
+    return result
+
+
+class Buffer:
+    """
+    The buffer contains the queues for incoming data and the timer for them.
+    """
+    QUEUE_SIZE = 1000
+
+    def __init__(self):
+        self.time_counter = itertools.count()
+        self.time = deque(maxlen=Buffer.QUEUE_SIZE)
+
+    def __getitem__(self, key):
+        return getattr(self, key.casefold().replace(" ", "_"))
+
+    def __setitem__(self, key, value) -> None:
+        setattr(self, key.casefold().replace(" ", "_"), value)
+
+    def __iter__(self):
+        for member in dir(self):
+            if not callable(getattr(self, member)) and not member.startswith(
+                    "__") and member != "time_counter":
+                yield getattr(self, member)
+
+    @abc.abstractmethod
+    def append(self, *args: typing.Any) -> None:
+        ...
+
+    def clear(self) -> None:
+        for member in dir(self):
+            if not callable(getattr(self, member)) and not member.startswith("__"):
+                if member == self.time_counter:
+                    self.time_counter = itertools.count()  # Reset counter
+                else:
+                    setattr(self, member, deque(maxlen=Buffer.QUEUE_SIZE))
+
+
+class PTI(typing.NamedTuple):
+    decimation: algorithm.pti.Decimation
+    inversion: algorithm.pti.Inversion
+
+
+class Interferometry(typing.NamedTuple):
+    interferometer: algorithm.interferometry.Interferometer
+    characterization: algorithm.interferometry.Characterization
+
+
+class PTIBuffer(Buffer):
+    MEAN_SIZE = 60
+    CHANNELS = 3
+
+    def __init__(self):
+        Buffer.__init__(self)
+        self.dc_values = [deque(maxlen=Buffer.QUEUE_SIZE) for _ in range(PTIBuffer.CHANNELS)]
+        self.interferometric_phase = deque(maxlen=Buffer.QUEUE_SIZE)
+        self.sensitivity = [deque(maxlen=Buffer.QUEUE_SIZE) for _ in range(PTIBuffer.CHANNELS)]
+        self.pti_signal = deque(maxlen=Buffer.QUEUE_SIZE)
+        self.pti_signal_mean = deque(maxlen=Buffer.QUEUE_SIZE)
+        self._pti_signal_mean_queue = deque(maxlen=PTIBuffer.MEAN_SIZE)
+
+    def append(self, pti_data: PTI, interferometer: algorithm.interferometry.Interferometer) -> None:
+        for i in range(3):
+            self.dc_values[i].append(pti_data.decimation.dc_signals[i])
+            self.sensitivity[i].append(pti_data.inversion.sensitivity[i])
+        self.interferometric_phase.append(interferometer.phase)
+        self.pti_signal.append(pti_data.inversion.pti_signal)
+        self._pti_signal_mean_queue.append(pti_data.inversion.pti_signal)
+        self.pti_signal_mean.append(np.mean(self._pti_signal_mean_queue))
+        self.time.append(next(self.time_counter))
+
+
+class CharacterisationBuffer(Buffer):
+    CHANNELS = 3
+
+    def __init__(self):
+        Buffer.__init__(self)
+        # The first channel has always the phase 0 by definition hence it is not needed.
+        self.output_phases = [deque(maxlen=Buffer.QUEUE_SIZE) for _ in range(self.CHANNELS - 1)]
+        self.amplitudes = [deque(maxlen=Buffer.QUEUE_SIZE) for _ in range(CharacterisationBuffer.CHANNELS)]
+        self.symmetry = deque(maxlen=Buffer.QUEUE_SIZE)
+        self.relative_symmetry = deque(maxlen=Buffer.QUEUE_SIZE)
+
+    def append(self, characterization: algorithm.interferometry.Characterization,
+               interferometer: algorithm.interferometry.Interferometer) -> None:
+        for i in range(3):
+            self.amplitudes[i].append(interferometer.amplitudes[i])
+        for i in range(2):
+            self.output_phases[i].append(interferometer.output_phases[i + 1])
+        self.symmetry.append(interferometer.absolute_symmetry)
+        self.relative_symmetry.append(interferometer.relative_symmetry)
+        self.time.append(characterization.time_stamp)
+
+
+class LaserBuffer(Buffer):
+    def __init__(self):
+        Buffer.__init__(self)
+        self.pump_laser_voltage = deque(maxlen=Buffer.QUEUE_SIZE)
+        self.pump_laser_current = deque(maxlen=Buffer.QUEUE_SIZE)
+        self.probe_laser_current = deque(maxlen=Buffer.QUEUE_SIZE)
+
+    def append(self, laser_data: hardware.laser.Data) -> None:
+        self.time.append(next(self.time_counter) / 10)
+        self.pump_laser_current.append(laser_data.high_power_laser_current)
+        self.pump_laser_voltage.append(laser_data.high_power_laser_voltage)
+        self.probe_laser_current.append(laser_data.low_power_laser_current)
+
+
+class TecBuffer(Buffer):
+    def __init__(self):
+        Buffer.__init__(self)
+        self.set_point: list[deque] = [deque(maxlen=Buffer.QUEUE_SIZE), deque(maxlen=Buffer.QUEUE_SIZE)]
+        self.actual_value: list[deque] = [deque(maxlen=Buffer.QUEUE_SIZE), deque(maxlen=Buffer.QUEUE_SIZE)]
+
+    def append(self, tec_data: hardware.tec.Data) -> None:
+        self.set_point[Tec.PUMP_LASER].append(tec_data.set_point[Tec.PUMP_LASER])
+        self.set_point[Tec.PROBE_LASER].append(tec_data.set_point[Tec.PROBE_LASER])
+        self.actual_value[Tec.PUMP_LASER].append(tec_data.actual_temperature[Tec.PUMP_LASER])
+        self.actual_value[Tec.PROBE_LASER].append(tec_data.actual_temperature[Tec.PROBE_LASER])
+        self.time.append(next(self.time_counter) / 10)
+
+
+class Mode(enum.IntEnum):
+    DISABLED = 0
+    CONTINUOUS_WAVE = 1
+    PULSED = 2
+
+
+@dataclass
+class Battery:
+    percentage: int
+    minutes_left: int
+
+
+@dataclass(init=False, frozen=True)
+class Signals(QtCore.QObject):
+    decimation = QtCore.pyqtSignal(pd.DataFrame)
+    decimation_live = QtCore.pyqtSignal(Buffer)
+    inversion = QtCore.pyqtSignal(pd.DataFrame)
+    inversion_live = QtCore.pyqtSignal(Buffer)
+    characterization = QtCore.pyqtSignal(pd.DataFrame)
+    characterization_live = QtCore.pyqtSignal(Buffer)
+    settings_pti = QtCore.pyqtSignal()
+    logging_update = QtCore.pyqtSignal(deque)
+    daq_running = QtCore.pyqtSignal(bool)
+    settings = QtCore.pyqtSignal(algorithm.interferometry.Interferometer)
+    destination_folder_changed = QtCore.pyqtSignal(str)
+    battery_state = QtCore.pyqtSignal(Battery)
+    valve_change = QtCore.pyqtSignal(hardware.motherboard.Valve)
+    bypass = QtCore.pyqtSignal(bool)
+    tec_data = QtCore.pyqtSignal(Buffer)
+    tec_data_display = QtCore.pyqtSignal(hardware.tec.Data)
+    clear_daq = QtCore.pyqtSignal()
+
+    def __init__(self):
+        QtCore.QObject.__init__(self)
+
+
+@dataclass
+class LaserSignals(QtCore.QObject):
+    photo_gain = QtCore.pyqtSignal(int)
+    current_probe_laser = QtCore.pyqtSignal(int, float)
+    max_current_probe_laser = QtCore.pyqtSignal(float)
+    probe_laser_mode = QtCore.pyqtSignal(int)
+    laser_voltage = QtCore.pyqtSignal(int, float)
+    current_dac = QtCore.pyqtSignal(int, int)
+    matrix_dac = QtCore.pyqtSignal(int, list)
+    data = QtCore.pyqtSignal(Buffer)
+    data_display = QtCore.pyqtSignal(hardware.laser.Data)
+    pump_laser_enabled = QtCore.pyqtSignal(bool)
+    probe_laser_enabled = QtCore.pyqtSignal(bool)
+    clear_pumplaser = QtCore.pyqtSignal()
+    clear_probelaser = QtCore.pyqtSignal()
+
+    def __init__(self):
+        QtCore.QObject.__init__(self)
+
+
+class TecMode(enum.IntEnum):
+    COOLING = 0
+    HEATING = 1
+
+
+@dataclass(init=False, frozen=True)
+class TecSignals(QtCore.QObject):
+    mode = QtCore.pyqtSignal(TecMode)
+    p_value = QtCore.pyqtSignal(int)
+    d_value = QtCore.pyqtSignal(int)
+    i_1_value = QtCore.pyqtSignal(int)
+    i_2_value = QtCore.pyqtSignal(int)
+    setpoint_temperature = QtCore.pyqtSignal(float)
+    loop_time = QtCore.pyqtSignal(int)
+    reference_resistor = QtCore.pyqtSignal(float)
+    max_power = QtCore.pyqtSignal(int)
+    enabled = QtCore.pyqtSignal(bool)
+    clear_plots = QtCore.pyqtSignal()
+    use_ntc = QtCore.pyqtSignal(bool)
+
+    def __init__(self):
+        QtCore.QObject.__init__(self)
+
+
+def shutdown_procedure() -> None:
+    Laser.driver.close()
+    Tec.driver.close()
+    time.sleep(0.5)  # Give the calculations threads time to finish their write operation
+    Motherboard.shutdown()
+    if platform.system() == "Windows":
+        subprocess.run(r"shutdown /s /t 1", shell=True)
+    else:
+        subprocess.run("sleep 0.5s && poweroff", shell=True)
+
+
+class Calculation:
+    MEAN_INTERVAL = 60
+
+    def __init__(self, queue_size=1000):
+        self.settings_path = ""
+        self.queue_size = queue_size
+        self.dc_signals = []
+        self.pti_buffer = PTIBuffer()
+        self.characterisation_buffer = CharacterisationBuffer()
+        self.pti_signal_mean_queue = deque(maxlen=60)
+        self.current_time = 0
+        self.interferometry = Interferometry(algorithm.interferometry.Interferometer(),
+                                             algorithm.interferometry.Characterization())
+        self.interferometry.characterization.interferometer = self.interferometry.interferometer
+        self.pti = PTI(algorithm.pti.Decimation(),
+                       algorithm.pti.Inversion(interferometer=self.interferometry.interferometer))
+        self.interferometry.characterization.interferometer = self.interferometry.interferometer
+        self._destination_folder = os.getcwd()
+        self.save_raw_data = False
+        signals.destination_folder_changed.connect(self._update_destination_folder)
+        signals.clear_daq.connect(self.clear_buffer)
+
+    def clear_buffer(self) -> None:
+        self.pti_buffer = PTIBuffer()
+        self.characterisation_buffer = CharacterisationBuffer()
+
+    def set_raw_data_saving(self) -> None:
+        if self.save_raw_data:
+            self.pti.decimation.save_raw_data = False
+        else:
+            self.pti.decimation.save_raw_data = True
+
+    def _update_destination_folder(self, folder: str) -> None:
+        self.interferometry.characterization.destination_folder = folder
+        self.pti.inversion.destination_folder = folder
+        self.pti.decimation.destination_folder = folder
+        self._destination_folder = folder
+
+    def process_daq_data(self) -> tuple[threading.Thread, threading.Thread]:
+        self.pti.inversion.init_header = True
+        self.pti.decimation.init_header = True
+        self.interferometry.characterization.init_online = True
+        self.interferometry.interferometer.load_settings()
+
+        def calculate_characterization() -> None:
+            while Motherboard.driver.running.is_set():
+                self.interferometry.characterization.characterise(live=True)
+                self.characterisation_buffer.append(self.interferometry.characterization,
+                                                    self.interferometry.interferometer)
+                signals.characterization_live.emit(self.characterisation_buffer)
+
+        def calculate_inversion():
+            while Motherboard.driver.running.is_set():
+                self.pti.decimation.ref = np.array(Motherboard.driver.ref_signal)
+                self.pti.decimation.dc_coupled = np.array(Motherboard.driver.dc_coupled)
+                self.pti.decimation.ac_coupled = np.array(Motherboard.driver.ac_coupled)
+                self.pti.decimation.decimate(live=True)
+                self.pti.inversion.lock_in = self.pti.decimation.lock_in
+                self.pti.inversion.dc_signals = self.pti.decimation.dc_signals
+                signals.decimation_live.emit(self.pti_buffer)
+                self.pti.inversion.invert(live=True)
+                self.interferometry.characterization.add_phase(self.interferometry.interferometer.phase)
+                self.dc_signals.append(copy.deepcopy(self.pti.decimation.dc_signals))
+                if self.interferometry.characterization.enough_values:
+                    self.interferometry.characterization._signals = copy.deepcopy(self.dc_signals)
+                    self.interferometry.characterization.phases = copy.deepcopy(
+                        self.interferometry.characterization.tracking_phase)
+                    self.interferometry.characterization.event.set()
+                    self.dc_signals = []
+                self.pti_buffer.append(self.pti, self.interferometry.interferometer)
+                signals.inversion_live.emit(self.pti_buffer)
+
+        characterization_thread = threading.Thread(target=calculate_characterization, daemon=True)
+        inversion_thread = threading.Thread(target=calculate_inversion, daemon=True)
+        characterization_thread.start()
+        inversion_thread.start()
+        return characterization_thread, inversion_thread
+
+    def calculate_characterisation(self, dc_file_path: str, use_settings=False, settings_path="") -> None:
+        self.interferometry.interferometer.decimation_filepath = dc_file_path
+        self.interferometry.interferometer.settings_path = settings_path
+        self.interferometry.characterization.use_configuration = use_settings
+        self.interferometry.characterization.characterise()
+        signals.settings.emit(self.interferometry.interferometer)
+
+    def calculate_decimation(self, decimation_path: str) -> None:
+        self.pti.decimation.file_path = decimation_path
+        self.pti.decimation.decimate()
+
+    def calculate_inversion(self, settings_path: str, inversion_path: str) -> None:
+        self.interferometry.interferometer.decimation_filepath = inversion_path
+        self.interferometry.interferometer.settings_path = settings_path
+        self.interferometry.interferometer.load_settings()
+        self.pti.inversion.invert()
+
+
+class ProbeLaserMode(enum.IntEnum):
+    CONSTANT_LIGHT = 0
+    CONSTANT_CURRENT = 1
+
+
+class Serial:
+    """
+    This class is a base class for subclasses of the driver objects from driver/serial.
+    """
+
+    driver = hardware.serial_device.Driver()
+
+    def __init__(self):
+        signals.destination_folder_changed.connect(self._update_file_path)
+        self._destination_folder = os.getcwd()
+        self._init_headers = True
+        self._running = False
+        signals.daq_running.connect(self._daq_running_changed)
+
+    def _daq_running_changed(self, running) -> None:
+        self._running = running
+
+    # @QtCore.pyqtSlot(str)
+    def _update_file_path(self, destination_folder: str) -> None:
+        self._destination_folder = destination_folder
+        self._init_headers = True
+
+    @classmethod
+    def find_port(cls) -> None:
+        cls.driver.find_port()
+
+    @classmethod
+    def open(cls) -> None:
+        """
+        Connects to a serial device and listens to incoming data.
+        """
+        cls.driver.open()
+
+    @classmethod
+    def run(cls) -> None:
+        cls.driver.run()
+
+    @classmethod
+    def close(cls) -> None:
+        """
+        Disconnects to a serial device and stops listening to data
+        """
+        cls.driver.close()
+
+    @classmethod
+    @abc.abstractmethod
+    def save_configuration(cls) -> None:
+        ...
+
+    @abc.abstractmethod
+    def fire_configuration_change(self) -> None:
+        """
+        By initiation of a Serial Object (on which the laser model relies) the configuration is
+        already set and do not fire events to update the GUI. This function is hence only called
+        once to manually activate the firing.
+        """
+
+    @abc.abstractmethod
+    def load_configuration(self) -> None:
+        self.fire_configuration_change()
+
+    def _incoming_data(self) -> None:
+        """
+        Listens to incoming data and emits them as _signals to the view as long a serial connection
+        is established.
+        """
+
+    def process_measured_data(self) -> threading.Thread:
+        processing_thread = threading.Thread(target=self._incoming_data, daemon=True)
+        processing_thread.start()
+        return processing_thread
+
+
+class Motherboard(Serial):
+    driver = hardware.motherboard.Driver()
+
+    def __init__(self):
+        Serial.__init__(self)
+        self.bms_data: tuple[float, float] = (0, 0)
+
+    @property
+    def connected(self) -> bool:
+        return self.driver.connected.is_set()
+
+    @staticmethod
+    def centi_kelvin_to_celsius(temperature: float) -> float:
+        return round((temperature - 273.15) / 100, 2)
+
+    def _incoming_data(self) -> None:
+        while self.driver.connected.is_set():
+            bms_data = Motherboard.driver.bms
+            bms_data.battery_temperature = Motherboard.centi_kelvin_to_celsius(bms_data.battery_temperature)
+            signals.battery_state.emit(Battery(bms_data.battery_percentage, bms_data.minutes_left))
+            if self.running:
+                if self._init_headers:
+                    units = {"Time": "H:M:S", "External DC Power": "bool",
+                             "Charging Battery": "bool",
+                             "Minutes Left": "min", "Charging Level": "%", "Temperature": "°C", "Current": "mA",
+                             "Voltage": "V", "Full Charge Capacity": "mAh", "Remaining Charge Capacity": "mAh"}
+                    pd.DataFrame(units, index=["Y:M:D"]).to_csv(self._destination_folder + "/BMS.csv",
+                                                                index_label="Date")
+                    self.init_header = False
+                now = datetime.now()
+                output_data = {"Time": str(now.strftime("%H:%M:%S"))}
+                for key, value in asdict(bms_data).items():
+                    output_data[key.replace("_", " ").title()] = value
+                bms_data_frame = pd.DataFrame(output_data, index=[str(now.strftime("%Y-%m-%d"))])
+                bms_data_frame.to_csv(self._destination_folder + "/BMS.csv", header=False, mode="a")
+
+    @property
+    def running(self) -> bool:
+        return self._running
+
+    @running.setter
+    def running(self, running):
+        self._running = running
+        if running:
+            # Before we start a new run, we clear all old data
+            self.driver.reset()
+            signals.clear_daq.emit()
+            self.driver.running.set()
+            signals.daq_running.emit(True)
+
+        else:
+            self.driver.running.clear()
+            signals.daq_running.emit(False)
+
+    @property
+    def shutdown_event(self) -> threading.Event:
+        return self.driver.shutdown
+
+    @property
+    def valve_period(self) -> int:
+        return self.driver.config.valve.period
+
+    @valve_period.setter
+    def valve_period(self, period: int) -> None:
+        if period < 0:
+            raise ValueError("Invalid value for period")
+        self.driver.config.valve.period = period
+
+    @property
+    def valve_duty_cycle(self) -> int:
+        return self.driver.config.valve.duty_cycle
+
+    @valve_duty_cycle.setter
+    def valve_duty_cycle(self, duty_cycle: int) -> None:
+        if not 0 < self.driver.config.valve.duty_cycle < 100:
+            raise ValueError("Invalid value for duty cycle")
+        self.driver.config.valve.duty_cycle = duty_cycle
+
+    @property
+    def automatic_valve_switch(self) -> bool:
+        return self.driver.config.valve.automatic_switch
+
+    @automatic_valve_switch.setter
+    def automatic_valve_switch(self, automatic_switch: bool) -> None:
+        self.driver.config.valve.automatic_switch = automatic_switch
+        if automatic_switch:
+            self.driver.automatic_switch.set()
+            self.driver.automatic_valve_change()
+        else:
+            self.driver.automatic_switch.clear()
+
+    @property
+    def bypass(self) -> bool:
+        return self.driver.bypass
+
+    @bypass.setter
+    def bypass(self, state: bool) -> None:
+        self.driver.bypass = state
+        signals.bypass.emit(state)
+
+    @staticmethod
+    def shutdown() -> None:
+        Motherboard.driver.do_shutdown()
+
+    def load_configuration(self) -> None:
+        Motherboard.driver.load_config()
+        self.fire_configuration_change()
+
+    @classmethod
+    def save_configuration(cls) -> None:
+        cls.driver.save_config()
+
+    @property
+    def config_path(self) -> str:
+        return self.driver.config_path
+
+    @config_path.setter
+    def config_path(self, config_path: str) -> None:
+        if not os.path.exists(config_path):
+            raise ValueError("File does not exist")
+        self.driver.config_path = config_path
+
+    def fire_configuration_change(self) -> None:
+        signals.valve_change.emit(Motherboard.driver.config.valve)
+
+
+class Laser(Serial):
+    buffer = LaserBuffer()
+    driver = hardware.laser.Driver()
+
+    def __init__(self):
+        Serial.__init__(self)
+        self._config_path = "hardware/configs/laser.json"
+
+    @property
+    @abc.abstractmethod
+    def config_path(self) -> str:
+        ...
+
+    @config_path.setter
+    @abc.abstractmethod
+    def config_path(self, config_path: str) -> None:
+        ...
+
+    @property
+    @abc.abstractmethod
+    def enabled(self) -> bool:
+        ...
+
+    @enabled.setter
+    @abc.abstractmethod
+    def enabled(self, enabled: bool) -> None:
+        ...
+
+    @abc.abstractmethod
+    def load_configuration(self) -> None:
+        ...
+
+    @abc.abstractmethod
+    def save_configuration(self) -> None:
+        ...
+
+    @abc.abstractmethod
+    def apply_configuration(self) -> None:
+        ...
+
+    def _incoming_data(self):
+        while self.driver.connected.is_set():
+            if self._running:
+                if self._init_headers:
+                    units = {"Time": "H:M:S",
+                             "Pump Laser Enabled": "bool",
+                             "Pump Laser Voltage": "V",
+                             "Probe Laser Enabled": "bool",
+                             "Pump Laser Current": "mA",
+                             "Probe Laser Current": "mA"}
+                    pd.DataFrame(units, index=["Y:M:D"]).to_csv(self._destination_folder + "/laser.csv",
+                                                                index_label="Date")
+                    self._init_headers = False
+            received_data: hardware.laser.Data = self.driver.data.get(block=True)
+            Laser.buffer.append(received_data)
+            laser_signals.data.emit(Laser.buffer)
+            laser_signals.data_display.emit(received_data)
+            if self._running:
+                now = datetime.now()
+                output_data = {"Time": str(now.strftime("%H:%M:%S")),
+                               "Pump Laser Enabled": received_data.high_power_laser_enabled,
+                               "Pump Laser Voltage": received_data.high_power_laser_voltage,
+                               "Probe Laser Enabled": received_data.low_power_laser_enabled,
+                               "Pump Laser Current": received_data.high_power_laser_current,
+                               "Probe Laser Current": received_data.low_power_laser_current}
+                laser_data_frame = pd.DataFrame(output_data, index=[str(now.strftime("%Y-%m-%d"))])
+                pd.DataFrame(laser_data_frame).to_csv(f"{self._destination_folder}/laser.csv", mode="a", header=False)
+
+    def fire_configuration_change(self) -> None:
+        ...
+
+
+class PumpLaser(Laser):
+    def __init__(self):
+        Laser.__init__(self)
+        self.pump_laser = self.driver.high_power_laser
+
+    @property
+    def connected(self) -> bool:
+        return self.driver.connected.is_set()
+
+    @property
+    def driver_bits(self) -> int:
+        return self.pump_laser.configuration.bit_value
+
+    @driver_bits.setter
+    def driver_bits(self, bits: int) -> None:
+        # With increasing the slider decreases its value but the voltage should increase, hence we subtract the bits.
+        self.pump_laser.configuration.bit_value = hardware.laser.HighPowerLaserConfig.NUMBER_OF_STEPS - bits
+        self.fire_driver_bits_signal()
+        self.pump_laser.set_voltage()
+
+    @property
+    def config_path(self) -> str:
+        return self.pump_laser.config_path
+
+    @config_path.setter
+    @abc.abstractmethod
+    def config_path(self, config_path: str) -> None:
+        self.pump_laser.config_path = config_path
+
+    def save_configuration(self) -> None:
+        self.pump_laser.save_configuration()
+
+    def load_configuration(self) -> None:
+        self.pump_laser.load_configuration()
+
+    def apply_configuration(self) -> None:
+        self.pump_laser.apply_configuration()
+
+    def fire_driver_bits_signal(self) -> None:
+        bits: int = self.pump_laser.configuration.bit_value
+        voltage: float = hardware.laser.HighPowerLaserConfig.bit_to_voltage(bits)
+        bits = hardware.laser.HighPowerLaserConfig.NUMBER_OF_STEPS - bits
+        laser_signals.laser_voltage.emit(bits, voltage)
+
+    @property
+    def enabled(self) -> bool:
+        return self.pump_laser.enabled
+
+    @enabled.setter
+    def enabled(self, enable: bool):
+        if enable:
+            laser_signals.clear_pumplaser.emit()
+        self.pump_laser.enabled = enable
+        laser_signals.pump_laser_enabled.emit(enable)
+
+    @property
+    def current_bits_dac_1(self) -> int:
+        return self.pump_laser.configuration.DAC[0].bit_value
+
+    @current_bits_dac_1.setter
+    def current_bits_dac_1(self, bits: int) -> None:
+        self.pump_laser.configuration.DAC[0].bit_value = bits
+        self.fire_current_bits_dac_1()
+        self.pump_laser.set_dac(0)
+
+    def fire_current_bits_dac_1(self) -> None:
+        laser_signals.current_dac.emit(0, self.pump_laser.configuration.DAC[0].bit_value)
+
+    @property
+    def current_bits_dac_2(self) -> int:
+        return self.pump_laser.configuration.DAC[1].bit_value
+
+    @current_bits_dac_2.setter
+    def current_bits_dac_2(self, bits: int) -> None:
+        self.pump_laser.configuration.DAC[1].bit_value = bits
+        self.fire_current_bits_dac2()
+        self.pump_laser.set_dac(1)
+
+    def fire_current_bits_dac2(self) -> None:
+        laser_signals.current_dac.emit(1, self.pump_laser.configuration.DAC[1].bit_value)
+
+    @property
+    def dac_1_matrix(self) -> hardware.laser.DAC:
+        return self.pump_laser.configuration.DAC[0]
+
+    @property
+    def dac_2_matrix(self) -> hardware.laser.DAC:
+        return self.pump_laser.configuration.DAC[1]
+
+    @staticmethod
+    def _set_indices(dac_number: int, dac: hardware.laser.DAC) -> None:
+        indices: typing.Annotated[list[int], 3] = []
+        for i in range(3):
+            if dac.continuous_wave[i]:
+                indices.append(Mode.CONTINUOUS_WAVE)
+            elif dac.pulsed_mode[i]:
+                indices.append(Mode.PULSED)
+            else:
+                indices.append(Mode.DISABLED)
+        laser_signals.matrix_dac.emit(dac_number, indices)
+
+    @dac_1_matrix.setter
+    def dac_1_matrix(self, dac: hardware.laser.DAC) -> None:
+        self.pump_laser.configuration.DAC[0] = dac
+        self.fire_dac_matrix_1()
+
+    def fire_dac_matrix_1(self) -> None:
+        PumpLaser._set_indices(dac_number=0, dac=self.dac_1_matrix)
+
+    @dac_2_matrix.setter
+    def dac_2_matrix(self, dac: hardware.laser.DAC) -> None:
+        self.pump_laser.configuration.DAC[1] = dac
+        self.fire_dac_matrix_2()
+
+    def fire_dac_matrix_2(self) -> None:
+        PumpLaser._set_indices(dac_number=1, dac=self.dac_2_matrix)
+
+    def update_dac_mode(self, dac: hardware.laser.DAC, channel: int, mode: int) -> None:
+        if mode == Mode.CONTINUOUS_WAVE:
+            dac.continuous_wave[channel] = True
+            dac.pulsed_mode[channel] = False
+        elif mode == Mode.PULSED:
+            dac.continuous_wave[channel] = False
+            dac.pulsed_mode[channel] = True
+        elif mode == Mode.DISABLED:
+            dac.continuous_wave[channel] = False
+            dac.pulsed_mode[channel] = False
+        self.pump_laser.set_dac_matrix()
+
+    def fire_configuration_change(self) -> None:
+        self.fire_driver_bits_signal()
+        self.fire_current_bits_dac_1()
+        self.fire_current_bits_dac2()
+        self.fire_dac_matrix_1()
+        self.fire_dac_matrix_2()
+
+
+class ProbeLaser(Laser):
+    def __init__(self):
+        Laser.__init__(self)
+        self.probe_laser = self.driver.low_power_laser
+
+    @property
+    def connected(self) -> bool:
+        return self.driver.connected.is_set()
+
+    @property
+    def current_bits_probe_laser(self) -> int:
+        return self.probe_laser.configuration.current.bits
+
+    @current_bits_probe_laser.setter
+    def current_bits_probe_laser(self, bits: int) -> None:
+        self.probe_laser.configuration.current.bits = bits
+        self.probe_laser.set_current()
+        bit, current = self.fire_current_bits_signal()
+        laser_signals.current_probe_laser.emit(hardware.laser.LowPowerLaser.CURRENT_BITS - bits, current)
+
+    @property
+    def config_path(self) -> str:
+        return self.probe_laser.config_path
+
+    @config_path.setter
+    @abc.abstractmethod
+    def config_path(self, config_path: str) -> None:
+        self.probe_laser.config_path = config_path
+
+    def save_configuration(self) -> None:
+        self.probe_laser.save_configuration()
+
+    def load_configuration(self) -> None:
+        self.probe_laser.load_configuration()
+
+    def fire_current_bits_signal(self) -> tuple[int, float]:
+        bits: int = self.probe_laser.configuration.current.bits
+        current: float = hardware.laser.LowPowerLaserConfig.bit_to_current(bits)
+        laser_signals.current_probe_laser.emit(hardware.laser.LowPowerLaser.CURRENT_BITS - bits, current)
+        return bits, current
+
+    @property
+    def enabled(self) -> bool:
+        return self.probe_laser.enabled
+
+    @enabled.setter
+    def enabled(self, enable: bool) -> None:
+        if enable:
+            laser_signals.clear_probelaser.emit()
+        self.probe_laser.enabled = enable
+        laser_signals.probe_laser_enabled.emit(enable)
+
+    @property
+    def photo_diode_gain(self) -> int:
+        return self.probe_laser.configuration.photo_diode_gain
+
+    @photo_diode_gain.setter
+    def photo_diode_gain(self, photo_diode_gain: int) -> None:
+        self.probe_laser.configuration.photo_diode_gain = photo_diode_gain
+        self.fire_photo_diode_gain_signal()
+        self.probe_laser.set_photo_diode_gain()
+
+    def fire_photo_diode_gain_signal(self) -> None:
+        laser_signals.photo_gain.emit(self.probe_laser.configuration.photo_diode_gain - 1)
+
+    @property
+    def probe_laser_max_current(self) -> float:
+        return self.probe_laser.configuration.current.max_mA
+
+    @probe_laser_max_current.setter
+    def probe_laser_max_current(self, current: float) -> None:
+        if self.probe_laser.configuration.current.max_mA != current:
+            self.probe_laser.configuration.current.max_mA = current
+            self.fire_max_current_signal()
+
+    def fire_max_current_signal(self) -> None:
+        laser_signals.max_current_probe_laser.emit(self.probe_laser.configuration.current.max_mA)
+
+    @property
+    def probe_laser_mode(self) -> ProbeLaserMode:
+        if self.probe_laser.configuration.mode.constant_light:
+            return ProbeLaserMode.CONSTANT_LIGHT
+        else:
+            return ProbeLaserMode.CONSTANT_CURRENT
+
+    @probe_laser_mode.setter
+    def probe_laser_mode(self, mode: ProbeLaserMode) -> None:
+        if mode == ProbeLaserMode.CONSTANT_CURRENT:
+            self.driver.low_power_laser.configuration.mode.constant_current = True
+            self.driver.low_power_laser.configuration.mode.constant_light = False
+        elif mode == ProbeLaserMode.CONSTANT_LIGHT:
+            self.driver.low_power_laser.configuration.mode.constant_current = False
+            self.driver.low_power_laser.configuration.mode.constant_light = True
+        self.probe_laser.set_mode()
+        self.fire_laser_mode_signal()
+
+    def fire_laser_mode_signal(self) -> None:
+        if self.probe_laser.configuration.mode.constant_light:
+            laser_signals.probe_laser_mode.emit(ProbeLaserMode.CONSTANT_LIGHT)
+        else:
+            laser_signals.probe_laser_mode.emit(ProbeLaserMode.CONSTANT_CURRENT)
+
+    def fire_configuration_change(self) -> None:
+        self.fire_current_bits_signal()
+        self.fire_laser_mode_signal()
+        self.fire_photo_diode_gain_signal()
+        self.fire_max_current_signal()
+
+    def apply_configuration(self) -> None:
+        self.probe_laser.apply_configuration()
+
+
+class Tec(Serial):
+    PUMP_LASER = 0
+    PROBE_LASER = 1
+
+    driver = hardware.tec.Driver()
+    _buffer = TecBuffer()
+
+    def __init__(self, channel: int):
+        Serial.__init__(self)
+        self.tec = self.driver.tec[channel]
+        self.tec_signals = tec_signals[channel]
+
+    @property
+    def connected(self) -> bool:
+        return self.driver.connected.is_set()
+
+    @property
+    def enabled(self) -> bool:
+        return self.tec.enabled
+
+    @enabled.setter
+    def enabled(self, enable) -> None:
+        if enable:
+            self.tec_signals.clear_plots.emit()
+        self.tec.enabled = enable
+        self.tec_signals.enabled.emit(enable)
+
+    @property
+    def config_path(self) -> str:
+        return self.tec.config_path
+
+    @config_path.setter
+    def config_path(self, config_path: str) -> None:
+        self.tec.config_path = config_path
+
+    def save_configuration(self) -> None:
+        self.tec.save_configuration()
+
+    def load_configuration(self) -> None:
+        self.tec.load_configuration()
+        self.fire_configuration_change()
+
+    def apply_configuration(self) -> None:
+        self.tec.apply_configuration()
+
+    @property
+    def p_value(self) -> float:
+        return self.tec.configuration.pid.proportional_value
+
+    @p_value.setter
+    def p_value(self, p_value: float) -> None:
+        self.tec.configuration.pid.proportional_value = p_value
+        self.tec.set_pid_p_value()
+
+    @property
+    def i_1_value(self) -> float:
+        return self.tec.configuration.pid.integral_value[0]
+
+    @i_1_value.setter
+    def i_1_value(self, i_value: int) -> None:
+        self.tec.configuration.pid.integral_value[0] = i_value
+        self.tec.set_pid_i_value(0)
+
+    @property
+    def i_2_value(self) -> float:
+        return self.tec.configuration.pid.integral_value[1]
+
+    @i_2_value.setter
+    def i_2_value(self, i_value: float) -> None:
+        self.tec.configuration.pid.integral_value[1] = i_value
+        self.tec.set_pid_i_value(1)
+
+    @property
+    def d_value(self) -> int:
+        return self.tec.configuration.pid.derivative_value
+
+    @d_value.setter
+    def d_value(self, d_value: int) -> None:
+        if isinstance(d_value, int) and d_value >= 0:
+            self.tec.configuration.pid.derivative_value = d_value
+            self.tec.set_pid_p_value()
+        else:
+            self.tec_signals.d_value.emit(self.tec.configuration.pid.derivative_value)
+
+    @property
+    def setpoint_temperature(self) -> float:
+        return self.tec.configuration.system_parameter.setpoint_temperature
+
+    @setpoint_temperature.setter
+    def setpoint_temperature(self, setpoint_temperature: float) -> None:
+        self.tec.configuration.system_parameter.setpoint_temperature = setpoint_temperature
+        self.tec.set_setpoint_temperature_value()
+
+    @property
+    def loop_time(self) -> int:
+        return self.tec.configuration.system_parameter.loop_time
+
+    @loop_time.setter
+    def loop_time(self, loop_time: int) -> None:
+        self.tec.configuration.system_parameter.loop_time = loop_time
+        self.tec.set_loop_time_value()
+
+    @property
+    def reference_resistor(self) -> int:
+        return self.tec.configuration.system_parameter.reference_resistor
+
+    @reference_resistor.setter
+    def reference_resistor(self, reference_resistor: float) -> None:
+        self.tec.configuration.system_parameter.reference_resistor = reference_resistor
+        self.tec.set_reference_resistor_value()
+
+    @property
+    def max_power(self) -> float:
+        return self.tec.configuration.system_parameter.max_power
+
+    @max_power.setter
+    def max_power(self, max_power: float) -> None:
+        self.tec.configuration.system_parameter.max_power = max_power
+        self.tec.set_max_power_value()
+
+    @property
+    def cooling(self) -> bool:
+        return self.tec.configuration.mode.cooling
+
+    @cooling.setter
+    def cooling(self, cooling: bool) -> None:
+        self.tec.configuration.mode.cooling = cooling
+        self.tec.configuration.mode.heating = not cooling
+        self.tec.set_mode()
+        if cooling:
+            self.tec_signals.mode.emit(TecMode.COOLING)
+        else:
+            self.tec_signals.mode.emit(TecMode.HEATING)
+
+    @property
+    def heating(self) -> bool:
+        return not self.cooling
+
+    @heating.setter
+    def heating(self, heating: bool) -> None:
+        self.cooling = not heating
+
+    def fire_configuration_change(self) -> None:
+        self.tec_signals.d_value.emit(self.d_value)
+        self.tec_signals.p_value.emit(self.p_value)
+        self.tec_signals.i_1_value.emit(self.i_2_value)
+        self.tec_signals.i_2_value.emit(self.i_2_value)
+        self.tec_signals.setpoint_temperature.emit(self.setpoint_temperature)
+        self.tec_signals.loop_time.emit(self.loop_time)
+        self.tec_signals.reference_resistor.emit(self.reference_resistor)
+        self.tec_signals.max_power.emit(self.max_power)
+        if self.cooling:
+            self.tec_signals.mode.emit(TecMode.COOLING)
+        else:
+            self.tec_signals.mode.emit(TecMode.HEATING)
+        self.tec_signals.use_ntc.emit(self.tec.configuration.temperature_element.NTC)
+
+    def _incoming_data(self) -> None:
+        while self.driver.connected.is_set():
+            if self._running:
+                if self._init_headers:
+                    units = {"Time": "H:M:S",
+                             "TEC Pump Laser Enabled": "bool",
+                             "TEC Probe Laser Enabled": "bool",
+                             "Measured Temperature Pump Laser": "°C",
+                             "Set Point Temperature Pump Laser": "°C",
+                             "Measured Temperature Probe Laser": "°C",
+                             "Set Point Temperature Probe Laser": "°C"}
+                    pd.DataFrame(units, index=["Y:M:D"]).to_csv(f"{self._destination_folder}/tec.csv",
+                                                                index_label="Date")
+                    self._init_headders = False
+            received_data: hardware.tec.Data = self.driver.data.get(block=True)
+            self._buffer.append(received_data)
+            signals.tec_data.emit(self._buffer)
+            signals.tec_data_display.emit(received_data)
+            if self._running:
+                now = datetime.now()
+                tec_data = {"Time": str(now.strftime("%H:%M:%S")),
+                            "TEC Pump Laser Enabled": self.driver.tec[Tec.PUMP_LASER].enabled,
+                            "TEC Probe Laser Enabled": self.driver.tec[Tec.PROBE_LASER].enabled,
+                            "Measured Temperature Pump Laser": received_data.actual_temperature[Tec.PUMP_LASER],
+                            "Set Point Temperature Pump Laser": received_data.set_point[Tec.PUMP_LASER],
+                            "Measured Temperature Probe Laser": received_data.actual_temperature[Tec.PROBE_LASER],
+                            "Set Point Temperature Probe Laser": received_data.set_point[Tec.PROBE_LASER]}
+                tec_data_frame = pd.DataFrame(tec_data, index=[str(now.strftime("%Y-%m-%d"))])
+                pd.DataFrame(tec_data_frame).to_csv(f"{self._destination_folder}/tec.csv", header=False, mode="a")
+
+
+def _process_data(file_path: str, headers: list[str, ...]) -> pd.DataFrame:
+    if not file_path:
+        raise FileNotFoundError("No file path given")
+    delimiter = find_delimiter(file_path)
+    try:
+        data = pd.read_csv(file_path, delimiter=delimiter, skiprows=[1], index_col="Time")
+    except ValueError:
+        try:
+            data = pd.read_csv(file_path, delimiter=delimiter, skiprows=[1], index_col="Time Stamp")
+        except ValueError:  # Data isn't saved with any index
+            data = pd.read_csv(file_path, delimiter=delimiter, skiprows=[1])
+    for header in headers:
+        for header_data in data.columns:
+            if header == header_data:
+                break
+        else:
+            raise KeyError(f"Header {header} not found in file")
+    return data
+
+
+def process_dc_data(dc_file_path: str) -> None:
+    headers = [f"DC CH{i}" for i in range(1, 4)]
+    try:
+        data = _process_data(dc_file_path, headers)
+    except KeyError:
+        headers = [f"PD{i}" for i in range(1, 4)]
+        data = _process_data(dc_file_path, headers)
+    except FileNotFoundError:
+        return
+    signals.decimation.emit(data)
+
+
+def process_inversion_data(inversion_file_path: str) -> None:
+    try:
+        headers = ["Interferometric Phase", "Sensitivity CH1", "Sensitivity CH2", "Sensitivity CH3", "PTI Signal"]
+        data = _process_data(inversion_file_path, headers)
+        data["PTI Signal 60 s Mean"] = running_average(data["PTI Signal"], mean_size=60)
+    except KeyError:
+        headers = ["Sensitivity CH1", "Sensitivity CH2", "Sensitivity CH3", "Interferometric Phase"]
+        data = _process_data(inversion_file_path, headers)
+    except FileNotFoundError:
+        return
+    signals.inversion.emit(data)
+
+
+def process_characterization_data(characterization_file_path: str) -> None:
+    headers = [f"Amplitude CH{i}" for i in range(1, 4)]
+    headers += [f"Output Phase CH{i}" for i in range(1, 4)]
+    headers += [f"Offset CH{i}" for i in range(1, 4)]
+    headers += ["Symmetry", "Relative Symmetry"]
+    try:
+        data = _process_data(characterization_file_path, headers)
+    except FileNotFoundError:
+        return
+    signals.characterization.emit(data)
+
+
+signals = Signals()
+laser_signals = LaserSignals()
+tec_signals = [TecSignals(), TecSignals()]
```

### Comparing `minipti-1.9.1/src/minipti/gui/view.py` & `minipti-1.9.3/src/gui/view.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,1034 +1,1074 @@
-import abc
-import collections
-import enum
-import functools
-import typing
-from typing import NamedTuple, Union
-
-import pandas as pd
-import pyqtgraph as pg
-from PyQt5 import QtWidgets, QtCore, QtGui
-from PyQt5.QtCore import Qt
-
-from .. import hardware
-from . import controller
-from . import model
-
-
-class MainWindow(QtWidgets.QMainWindow):
-    HORIZONTAL_SIZE = 1100
-    VERTICAL_SIZE = 800
-
-    def __init__(self, main_controller):
-        QtWidgets.QMainWindow.__init__(self)
-        self.setWindowTitle("MiniPTI")
-        self.setWindowIcon(QtGui.QIcon("images/icon.png"))
-        self.main_controller = main_controller
-        self.tab_bar = QtWidgets.QTabWidget(self)
-        self.setCentralWidget(self.tab_bar)
-        self.tabs: Union[Tab, None] = None
-        self.current_pump_laser = PumpLaserCurrent()
-        self.current_probe_laser = ProbeLaserCurrent()
-        self.temperature_probe_laser = TecTemperature(laser="Probe Laser")
-        self.temperature_pump_laser = TecTemperature(laser="Pump Laser")
-        self.dc = DC()
-        self.amplitudes = Amplitudes()
-        self.output_phases = OutputPhases()
-        self.interferometric_phase = InterferometricPhase()
-        self.sensitivity = Sensitivity()
-        self.symmetry = Symmetry()
-        self.pti_signal = PTISignal()
-        self._init_tabs()
-        self.resize(MainWindow.HORIZONTAL_SIZE, MainWindow.VERTICAL_SIZE)
-        self.show()
-
-    def _init_pump_laser_tab(self) -> QtWidgets.QTabWidget:
-        tab = QtWidgets.QTabWidget()
-        sub_layout = QtWidgets.QSplitter()
-        pump_laser = PumpLaser()
-        pump_laser_tab = QtWidgets.QTabWidget()
-        pump_laser_tab.setLayout(QtWidgets.QHBoxLayout())
-        sub_layout.insertWidget(0, pump_laser)
-        sub_layout.insertWidget(1, self.current_pump_laser.window)
-        pump_laser_tab.layout().addWidget(sub_layout)
-        tab.addTab(pump_laser_tab, "Laser Driver")
-        sub_layout = QtWidgets.QSplitter()
-        tec_tab = QtWidgets.QTabWidget()
-        tec_tab.setLayout(QtWidgets.QHBoxLayout())
-        sub_layout.insertWidget(0, Tec(laser="Pump Laser"))
-        sub_layout.insertWidget(1, self.temperature_pump_laser.window)
-        tec_tab.layout().addWidget(sub_layout)
-        tab.addTab(tec_tab, "Tec Driver")
-        return tab
-
-    def _init_probe_laser_tab(self) -> QtWidgets.QTabWidget:
-        tab = QtWidgets.QTabWidget()
-        sub_layout = QtWidgets.QSplitter()
-        probe_laser = ProbeLaser()
-        probe_laser_tab = QtWidgets.QTabWidget()
-        probe_laser_tab.setLayout(QtWidgets.QHBoxLayout())
-        sub_layout.insertWidget(0, probe_laser)
-        sub_layout.insertWidget(1, self.current_probe_laser.window)
-        probe_laser_tab.layout().addWidget(sub_layout)
-        tab.addTab(probe_laser_tab, "Laser Driver")
-        sub_layout = QtWidgets.QSplitter()
-        tec_tab = QtWidgets.QTabWidget()
-        tec_tab.setLayout(QtWidgets.QHBoxLayout())
-        sub_layout.insertWidget(0, Tec(laser="Probe Laser"))
-        sub_layout.insertWidget(1, self.temperature_probe_laser.window)
-        tec_tab.layout().addWidget(sub_layout)
-        tab.addTab(tec_tab, "Tec Driver")
-        return tab
-
-    def _init_tabs(self):
-        self.tabs = Tab(home=Home(self, self.main_controller),
-                        pump_laser=self._init_pump_laser_tab(),
-                        probe_laser=self._init_probe_laser_tab(),
-                        dc=QtWidgets.QTabWidget(),
-                        amplitudes=QtWidgets.QTabWidget(),
-                        output_phases=QtWidgets.QTabWidget(),
-                        sensitivity=QtWidgets.QTabWidget(),
-                        symmetry=QtWidgets.QTabWidget(),
-                        interferometric_phase=QtWidgets.QTabWidget(),
-                        pti_signal=QtWidgets.QTabWidget())
-        self.tab_bar.addTab(self.tabs.home, "Home")
-        self.tab_bar.addTab(self.tabs.pump_laser, "Pump Laser")
-        self.tab_bar.addTab(self.tabs.probe_laser, "Probe Laser")
-        # DC Plot
-        self.tabs.dc.setLayout(QtWidgets.QHBoxLayout())
-        self.tabs.dc.layout().addWidget(self.dc.window)
-        self.tab_bar.addTab(self.tabs.dc, "DC Signals")
-        # Amplitudes Plot
-        self.tabs.amplitudes.setLayout(QtWidgets.QHBoxLayout())
-        self.tabs.amplitudes.layout().addWidget(self.amplitudes.window)
-        self.tab_bar.addTab(self.tabs.amplitudes, "Amplitudes")
-        # Output Phases Plot
-        self.tabs.output_phases.setLayout(QtWidgets.QHBoxLayout())
-        self.tabs.output_phases.layout().addWidget(self.output_phases.window)
-        self.tab_bar.addTab(self.tabs.output_phases, "Output Phases")
-        # Interferometric Phase Plot
-        self.tabs.interferometric_phase.setLayout(QtWidgets.QHBoxLayout())
-        self.tabs.interferometric_phase.layout().addWidget(self.interferometric_phase.window)
-        self.tab_bar.addTab(self.tabs.interferometric_phase, "Interferometric Phase")
-        # Sensitivity Plot
-        self.tabs.sensitivity.setLayout(QtWidgets.QHBoxLayout())
-        self.tabs.sensitivity.layout().addWidget(self.sensitivity.window)
-        self.tab_bar.addTab(self.tabs.sensitivity, "Sensitivity")
-        # Symmetry Plot
-        self.tabs.symmetry.setLayout(QtWidgets.QHBoxLayout())
-        self.tabs.symmetry.layout().addWidget(self.symmetry.window)
-        self.tab_bar.addTab(self.tabs.symmetry, "Symmetry")
-        # PTI Signal Plot
-        self.tabs.pti_signal.setLayout(QtWidgets.QHBoxLayout())
-        self.tabs.pti_signal.layout().addWidget(self.pti_signal.window)
-        self.tab_bar.addTab(self.tabs.pti_signal, "PTI Signal")
-
-    def closeEvent(self, close_event):
-        close = QtWidgets.QMessageBox.question(self, "QUIT", "Are you sure you want to close?",
-                                               QtWidgets.QMessageBox.StandardButton.Yes |
-                                               QtWidgets.QMessageBox.StandardButton.No)
-        if close == QtWidgets.QMessageBox.StandardButton.Yes:
-            close_event.accept()
-            self.main_controller.close()
-        else:
-            close_event.ignore()
-
-
-class Tab(NamedTuple):
-    home: "Home"
-    pump_laser: QtWidgets.QTabWidget
-    probe_laser: QtWidgets.QTabWidget
-    dc: QtWidgets.QTabWidget
-    amplitudes: QtWidgets.QTabWidget
-    output_phases: QtWidgets.QTabWidget
-    interferometric_phase: QtWidgets.QTabWidget
-    sensitivity: QtWidgets.QTabWidget
-    symmetry: QtWidgets.QTabWidget
-    pti_signal: QtWidgets.QTabWidget
-
-
-class _Frames:
-    def __init__(self):
-        self.frames = {}  # type: dict[str, QtWidgets.QGroupBox]
-
-    def create_frame(self, master: QtWidgets.QWidget, title, x_position, y_position,
-                     x_span=1, y_span=1) -> None:
-        self.frames[title] = QtWidgets.QGroupBox()
-        self.frames[title].setTitle(title)
-        self.frames[title].setLayout(QtWidgets.QGridLayout())
-        try:
-            master.layout().addWidget(self.frames[title], x_position, y_position, x_span, y_span)
-        except TypeError:
-            master.layout().addWidget(self.frames[title])
-
-    @abc.abstractmethod
-    def _init_frames(self) -> None:
-        ...
-
-
-class _CreateButton:
-    def __init__(self):
-        self.buttons = {}  # type: dict[str, QtWidgets.QPushButton]
-
-    def create_button(self, master, title, slot, master_title="") -> None:
-        self.buttons[master_title + title] = QtWidgets.QPushButton(master, text=title)
-        self.buttons[master_title + title].clicked.connect(slot)
-        master.layout().addWidget(self.buttons[master_title + title])
-
-    @abc.abstractmethod
-    def _init_buttons(self) -> None:
-        ...
-
-
-class SettingsView(QtWidgets.QTableView):
-    def __init__(self, parent, settings_model: QtCore.QAbstractTableModel):
-        QtWidgets.QTableView.__init__(self, parent=parent)
-        header = self.horizontalHeader()
-        header.setStretchLastSection(True)
-        index = self.verticalHeader()
-        index.setSectionResizeMode(QtWidgets.QHeaderView.Stretch)
-        header.setSectionResizeMode(QtWidgets.QHeaderView.Stretch)
-        index.setStretchLastSection(True)
-        self.resizeColumnsToContents()
-        self.resizeRowsToContents()
-        self.setModel(settings_model)
-
-
-def toggle_button(checked, button: QtWidgets.QPushButton) -> None:
-    if checked:
-        button.setStyleSheet("background-color : lightgreen")
-    else:
-        button.setStyleSheet("background-color : light gray")
-
-
-class Home(QtWidgets.QTabWidget, _Frames, _CreateButton):
-    def __init__(self, main_window: QtWidgets.QMainWindow, main_app: QtWidgets.QApplication):
-        QtWidgets.QTabWidget.__init__(self)
-        _Frames.__init__(self)
-        _CreateButton.__init__(self)
-        self.setLayout(QtWidgets.QGridLayout())
-        self.controller = controller.Home(self, main_app)
-        self.logging_window = QtWidgets.QLabel()
-        model.signals.logging_update.connect(self.logging_update)
-        self._init_frames()
-        self.settings = SettingsView(parent=self.frames["Setting"], settings_model=self.controller.settings_model)
-        self.frames["Setting"].layout().addWidget(self.settings)
-        self.scroll = QtWidgets.QScrollArea(widgetResizable=True)
-        self.scroll.setWidgetResizable(True)
-        self.frames["Log"] = QtWidgets.QDockWidget('Log', self)
-        self.scroll.setWidget(self.logging_window)
-        self.frames["Log"].setWidget(self.scroll)
-        self.frames["Battery"] = QtWidgets.QDockWidget("Battery", self)
-        self.charge_level = QtWidgets.QLabel("NaN % left")
-        self.minutes_left = QtWidgets.QLabel("NaN Minutes left")
-        sub_layout = QtWidgets.QWidget()
-        sub_layout.setMaximumWidth(150)
-        sub_layout.setLayout(QtWidgets.QVBoxLayout())
-        sub_layout.layout().addWidget(self.charge_level)
-        sub_layout.layout().addWidget(self.minutes_left)
-        self.frames["Battery"].setWidget(sub_layout)
-        self.scroll.setWidget(self.logging_window)
-        main_window.addDockWidget(Qt.BottomDockWidgetArea, self.frames["Log"])
-        main_window.addDockWidget(Qt.BottomDockWidgetArea, self.frames["Battery"])
-        main_window.setCorner(Qt.BottomRightCorner, Qt.RightDockWidgetArea)
-        self.destination_folder = QtWidgets.QLabel(self.controller.calculation_model.destination_folder)
-        model.signals.destination_folder_changed.connect(self.update_destination_folder)
-        self.save_raw_data = QtWidgets.QCheckBox("Save Raw Data")
-        self.automatic_valve_switch = QtWidgets.QCheckBox("Automatic Valve Switch")
-        self.duty_cyle_valve = QtWidgets.QLabel("%")
-        self.period_valve = QtWidgets.QLabel("s")
-        self.duty_cycle_field = QtWidgets.QLineEdit()
-        self.period_field = QtWidgets.QLineEdit()
-        self._init_buttons()
-        self._init_raw_data_button()
-        self._init_valves()
-        self._init_signals()
-        self.controller.fire_motherboard_configuration_change()
-
-    def update_destination_folder(self) -> None:
-        self.destination_folder.setText(self.controller.calculation_model.destination_folder)
-
-    @QtCore.pyqtSlot(model.Battery)
-    def update_battery_state(self, battery: model.Battery) -> None:
-        self.charge_level.setText(f"{battery.percentage} % left")
-        self.minutes_left.setText(f"Minutes left: {battery.minutes_left}")
-
-    @QtCore.pyqtSlot(hardware.motherboard.Valve)
-    def update_valve(self, valve: hardware.motherboard.Valve) -> None:
-        self.duty_cycle_field.setText(str(valve.duty_cycle))
-        self.period_field.setText(str(valve.period))
-        self.automatic_valve_switch.setChecked(valve.automatic_switch)
-
-    def _init_frames(self) -> None:
-        sub_layout = QtWidgets.QWidget()
-        sub_layout.setLayout(QtWidgets.QGridLayout())
-        self.create_frame(master=sub_layout, title="File Path", x_position=0, y_position=1)
-        self.create_frame(master=sub_layout, title="Shutdown", x_position=0, y_position=2)
-        self.create_frame(master=self, title="Setting", x_position=0, y_position=0, x_span=2)
-        self.create_frame(master=self, title="Offline Processing", x_position=2, y_position=0)
-        self.create_frame(master=self, title="Plot Data", x_position=2, y_position=1)
-        self.create_frame(master=self, title="Measurement", x_position=3, y_position=0)
-        self.create_frame(master=self, title="Drivers", x_position=3, y_position=1)
-        self.create_frame(master=self, title="Pump Laser", x_position=4, y_position=0)
-        self.create_frame(master=self, title="Probe Laser", x_position=4, y_position=1)
-        self.layout().addWidget(sub_layout, 1, 1)
-        self.create_frame(master=self, title="Valve", x_position=0, y_position=1)
-
-    def _init_buttons(self) -> None:
-        self.create_button(master=self.frames["Shutdown"], title="Shutdown and Close",
-                           slot=self.controller.shutdown_by_button)
-
-        # SettingsTable buttons
-        sub_layout = QtWidgets.QWidget()
-        self.frames["Setting"].layout().addWidget(sub_layout)
-        sub_layout.setLayout(QtWidgets.QHBoxLayout())
-        self.create_button(master=sub_layout, title="Save Settings", slot=self.controller.save_settings)
-        self.create_button(master=sub_layout, title="Load Settings", slot=self.controller.load_settings)
-        sub_layout.layout().addWidget(self.save_raw_data)
-
-        # Offline Processing buttons
-        sub_layout = QtWidgets.QWidget()
-        sub_layout.setLayout(QtWidgets.QHBoxLayout())
-        self.frames["Offline Processing"].layout().addWidget(sub_layout)
-        self.create_button(master=sub_layout, title="Decimation", slot=self.controller.calculate_decimation)
-        self.create_button(master=sub_layout, title="Inversion", slot=self.controller.calculate_inversion)
-        self.create_button(master=sub_layout, title="Characterisation", slot=self.controller.calculate_characterisation)
-
-        # Plotting buttons
-        sub_layout = QtWidgets.QWidget(parent=self.frames["Plot Data"])
-        sub_layout.setLayout(QtWidgets.QHBoxLayout())
-        self.frames["Plot Data"].layout().addWidget(sub_layout)
-        self.create_button(master=sub_layout, title="Decimation", slot=self.controller.plot_dc)
-        self.create_button(master=sub_layout, title="Inversion", slot=self.controller.plot_inversion)
-        self.create_button(master=sub_layout, title="Characterisation", slot=self.controller.plot_characterisation)
-
-        # Driver buttons
-        sub_layout = QtWidgets.QWidget(parent=self.frames["Drivers"])
-        sub_layout.setLayout(QtWidgets.QHBoxLayout())
-        self.frames["Drivers"].layout().addWidget(sub_layout)
-        self.create_button(master=sub_layout, title="Scan Ports", slot=self.controller.find_devices)
-        self.create_button(master=sub_layout, title="Connect Devices", slot=self.controller.connect_devices)
-
-        # Output File Location
-        sub_layout = QtWidgets.QWidget(parent=self.frames["File Path"])
-        sub_layout.setLayout(QtWidgets.QVBoxLayout())
-        self.frames["File Path"].layout().addWidget(sub_layout)
-        self.create_button(master=sub_layout, title="Destination Folder", slot=self.controller.set_destination_folder)
-        sub_layout.layout().addWidget(self.destination_folder)
-
-        # Valve Control
-        sub_layout = QtWidgets.QWidget(parent=self.frames["Valve"])
-        sub_layout.setLayout(QtWidgets.QGridLayout())
-        sub_layout.layout().addWidget(self.automatic_valve_switch, 0, 0)
-        sub_layout.layout().addWidget(QtWidgets.QLabel("Valve Period"), 1, 0)
-        sub_layout.layout().addWidget(self.period_field, 1, 1)
-        sub_layout.layout().addWidget(QtWidgets.QLabel("s"), 1, 2)
-        sub_layout.layout().addWidget(QtWidgets.QLabel("Valve Duty Cycle"), 2, 0)
-        sub_layout.layout().addWidget(self.duty_cycle_field, 2, 1)
-        sub_layout.layout().addWidget(QtWidgets.QLabel("%"), 2, 2)
-        self.frames["Valve"].layout().addWidget(sub_layout)
-        sub_layout = QtWidgets.QWidget(parent=self.frames["Valve"])
-        sub_layout.setLayout(QtWidgets.QHBoxLayout())
-        self.create_button(master=sub_layout, title="Save Settings",
-                           slot=self.controller.save_motherboard_configuration)
-        self.create_button(master=sub_layout, title="Load Settings",
-                           slot=self.controller.load_motherboard_configuration)
-        self.frames["Valve"].layout().addWidget(sub_layout)
-
-        # Measurement Buttons
-        sub_layout = QtWidgets.QWidget(parent=self.frames["Measurement"])
-        sub_layout.setLayout(QtWidgets.QHBoxLayout())
-        self.frames["Measurement"].layout().addWidget(sub_layout)
-        self.create_button(master=sub_layout, title="Run Measurement", slot=self.controller.run_measurement)
-        self.create_button(master=sub_layout, title="Clean Air", slot=self.controller.update_bypass)
-
-        # Pump Laser
-        sub_layout = QtWidgets.QWidget(parent=self.frames["Pump Laser"])
-        sub_layout.setLayout(QtWidgets.QHBoxLayout())
-        self.create_button(master=sub_layout, title="Enable Laser", slot=self.controller.enable_pump_laser,
-                           master_title="Pump Laser")
-        self.create_button(master=sub_layout, title="Enable Tec", slot=self.controller.enable_tec_pump_laser,
-                           master_title="Pump Laser")
-        self.frames["Pump Laser"].layout().addWidget(sub_layout)
-
-        # Probe Laser
-        sub_layout = QtWidgets.QWidget(parent=self.frames["Probe Laser"])
-        sub_layout.setLayout(QtWidgets.QHBoxLayout())
-        self.create_button(master=sub_layout, title="Enable Laser", slot=self.controller.enable_probe_laser,
-                           master_title="Probe Laser")
-        self.create_button(master=sub_layout, title="Enable Tec", slot=self.controller.enable_tec_probe_laser,
-                           master_title="Probe Laser")
-        self.frames["Probe Laser"].layout().addWidget(sub_layout)
-
-    def logging_update(self, log_queue: collections.deque) -> None:
-        self.logging_window.setText("".join(log_queue))
-
-    def _init_raw_data_button(self) -> None:
-        self.save_raw_data.setChecked(self.controller.calculation_model.save_raw_data)
-        self.save_raw_data.stateChanged.connect(self.controller.calculation_model.set_raw_data_saving)
-
-    def _init_valves(self) -> None:
-        self.automatic_valve_switch.stateChanged.connect(self._automatic_switch_changed)
-        self.period_field.editingFinished.connect(self._period_changed)
-        self.duty_cycle_field.editingFinished.connect(self._duty_cycle_changed)
-
-    def _automatic_switch_changed(self) -> None:
-        self.controller.update_automatic_valve_switch(self.automatic_valve_switch.isChecked())
-
-    def _period_changed(self) -> None:
-        self.controller.update_valve_period(self.period_field.text())
-
-    def _duty_cycle_changed(self) -> None:
-        self.controller.update_valve_duty_cycle(self.duty_cycle_field.text())
-
-    @QtCore.pyqtSlot(bool)
-    def update_clean_air(self, state: bool) -> None:
-        toggle_button(state, self.buttons["Clean Air"])
-
-    @QtCore.pyqtSlot(bool)
-    def update_enable_pump_laser(self, state: bool):
-        toggle_button(state, self.buttons["Pump Laser Enable Laser"])
-
-    @QtCore.pyqtSlot(bool)
-    def update_enable_probe_laser(self, state: bool):
-        toggle_button(state, self.buttons["Probe Laser Enable Laser"])
-
-    @QtCore.pyqtSlot(bool)
-    def update_enable_pump_laser_tec(self, state: bool):
-        toggle_button(state, self.buttons["Pump Laser Enable Tec"])
-
-    @QtCore.pyqtSlot(bool)
-    def update_enable_probe_laser_tec(self, state: bool):
-        toggle_button(state, self.buttons["Probe Laser Enable Tec"])
-
-    def _init_signals(self) -> None:
-        model.signals.valve_change.connect(self.update_valve)
-        model.signals.bypass.connect(self.update_clean_air)
-        model.laser_signals.pump_laser_enabled.connect(self.update_enable_pump_laser)
-        model.laser_signals.probe_laser_enabled.connect(self.update_enable_probe_laser)
-        model.tec_signals.pump_laser.enabled.connect(self.update_enable_pump_laser_tec)
-        model.tec_signals.probe_laser.enabled.connect(self.update_enable_probe_laser_tec)
-
-
-class Slider(QtWidgets.QWidget):
-    def __init__(self, minimum=0, maximum=100, unit="%"):
-        QtWidgets.QWidget.__init__(self)
-        self.slider = QtWidgets.QSlider()
-        self.setLayout(QtWidgets.QHBoxLayout())
-        self.layout().addWidget(self.slider)
-        self.slider.setOrientation(QtCore.Qt.Orientation.Horizontal)
-        self.slider_value = QtWidgets.QLabel()
-        self.layout().addWidget(self.slider_value)
-        self.slider.setMinimum(minimum)
-        self.slider.setMaximum(maximum)
-        self.unit = unit
-        self.index_value = 0  # type: typing.Any
-
-    @functools.singledispatchmethod
-    def update_value(self, value: int) -> None:
-        self.slider_value.setText(f"{value} " + self.unit)
-
-    @update_value.register
-    def _(self, value: float) -> None:
-        self.slider_value.setText(f"{round(value, 2)} " + self.unit)
-
-
-class ModeIndices(enum.IntEnum):
-    DISABLED = 0
-    CONTINUOUS_WAVE = 1
-    PULSED = 2
-
-
-class PumpLaser(QtWidgets.QWidget, _Frames, _CreateButton):
-    MIN_DRIVER_BIT = 0
-    MAX_DRIVER_BIT = (1 << 7) - 1
-    MIN_CURRENT = 0
-    MAX_CURRENT = (1 << 12) - 1
-
-    def __init__(self):
-        QtWidgets.QWidget.__init__(self)
-        _CreateButton.__init__(self)
-        _Frames.__init__(self)
-        self.model = None
-        self.setLayout(QtWidgets.QGridLayout())
-        self.current_display = QtWidgets.QLabel("0 mA")
-        self.voltage_display = QtWidgets.QLabel("0 V")
-        self.driver_voltage = Slider(minimum=PumpLaser.MIN_DRIVER_BIT, maximum=PumpLaser.MAX_DRIVER_BIT, unit="V")
-        self.current = [Slider(minimum=PumpLaser.MIN_CURRENT, maximum=PumpLaser.MAX_CURRENT, unit="Bit"),
-                        Slider(minimum=PumpLaser.MIN_CURRENT, maximum=PumpLaser.MAX_CURRENT, unit="Bit")]
-        self.mode_matrix = [[QtWidgets.QComboBox() for _ in range(3)], [QtWidgets.QComboBox() for _ in range(3)]]
-        self.controller = controller.PumpLaser(self)
-        self._init_frames()
-        self._init_current_configuration()
-        self._init_voltage_configuration()
-        self._init_buttons()
-        self.frames["Driver Voltage"].layout().addWidget(self.driver_voltage)
-        self.frames["Measured Values"].layout().addWidget(self.current_display)
-        self.frames["Measured Values"].layout().addWidget(self.voltage_display)
-        self._init_signals()
-        self.controller.fire_configuration_change()
-
-    def _init_signals(self) -> None:
-        model.laser_signals.laser_voltage.connect(self._update_voltage_slider)
-        model.laser_signals.current_dac.connect(self._update_current_dac)
-        model.laser_signals.matrix_dac.connect(self._update_dac_matrix)
-        model.laser_signals.data_display.connect(self._update_current_voltage)
-
-    @QtCore.pyqtSlot()
-    def _update_current_voltage(self, value: hardware.laser.Data) -> None:
-        self.current_display.setText(str(value.pump_laser_current) + " mA")
-        self.voltage_display.setText(str(value.pump_laser_voltage) + " V")
-
-    def _init_voltage_configuration(self) -> None:
-        self.driver_voltage.slider.valueChanged.connect(self.controller.update_driver_voltage)
-
-    def _init_current_configuration(self) -> None:
-        self.current[0].slider.valueChanged.connect(self.controller.update_current_dac1)
-        self.current[1].slider.valueChanged.connect(self.controller.update_current_dac2)
-        for i in range(3):
-            self.mode_matrix[0][i].currentIndexChanged.connect(self.controller.update_dac1(i))
-            self.mode_matrix[1][i].currentIndexChanged.connect(self.controller.update_dac2(i))
-
-    @QtCore.pyqtSlot(int, list)
-    def _update_dac_matrix(self, dac_number: int, configuration: typing.Annotated[list[int], 3]) -> None:
-        for channel in range(3):
-            if configuration[channel] == model.Mode.CONTINUOUS_WAVE:
-                    self.mode_matrix[dac_number][channel].setCurrentIndex(ModeIndices.CONTINUOUS_WAVE)
-            elif configuration[channel] == model.Mode.PULSED:
-                self.mode_matrix[dac_number][channel].setCurrentIndex(ModeIndices.PULSED)
-            elif configuration[channel] == model.Mode.DISABLED:
-                self.mode_matrix[dac_number][channel].setCurrentIndex(ModeIndices.DISABLED)
-
-    @QtCore.pyqtSlot(int, float)
-    def _update_voltage_slider(self, index: int, value: float) -> None:
-        self.driver_voltage.slider.setValue(index)
-        self.driver_voltage.update_value(value)
-
-    @QtCore.pyqtSlot(int, int)
-    def _update_current_dac(self, dac: int, index: int) -> None:
-        self.current[dac].slider.setValue(index)
-        self.current[dac].update_value(index)
-
-    def _init_frames(self) -> None:
-        self.create_frame(master=self, title="Measured Values", x_position=1, y_position=0)
-        self.create_frame(master=self, title="Driver Voltage", x_position=2, y_position=0)
-        for i in range(1, 3):
-            self.create_frame(master=self, title=f"Current {i}", x_position=i + 2, y_position=0)
-        self.create_frame(master=self, title="Configuration", x_position=5, y_position=0)
-
-    def _init_buttons(self) -> None:
-        dac_inner_frames = [QtWidgets.QWidget() for _ in range(2)]  # For slider and button-matrices
-        for j in range(2):
-            dac_inner_frames[j].setLayout(QtWidgets.QGridLayout())
-            self.frames[f"Current {j + 1}"].layout().addWidget(self.current[j])
-            for i in range(3):
-                sub_frames = [QtWidgets.QWidget() for _ in range(3)]
-                sub_frames[i].setLayout(QtWidgets.QVBoxLayout())
-                dac_inner_frames[j].layout().addWidget(sub_frames[i], 1, i)
-                self.mode_matrix[j][i].addItem("Disabled")
-                self.mode_matrix[j][i].addItem("Continuous Wave")
-                self.mode_matrix[j][i].addItem("Pulsed Mode")
-                sub_frames[i].layout().addWidget(QtWidgets.QLabel(f"Channel {i + 1}"))
-                sub_frames[i].layout().addWidget(self.mode_matrix[j][i])
-            self.frames[f"Current {j + 1}"].layout().addWidget(dac_inner_frames[j])
-
-        config = QtWidgets.QWidget()
-        config.setLayout(QtWidgets.QHBoxLayout())
-        self.create_button(master=config, title="Save Configuration",
-                           slot=self.controller.save_configuration)
-        self.create_button(master=config, title="Load Configuration",
-                           slot=self.controller.load_configuration)
-        self.create_button(master=config, title="Apply Configuration",
-                           slot=self.controller.apply_configuration)
-        self.frames["Configuration"].layout().addWidget(config, 4, 0)
-
-
-class ProbeLaser(QtWidgets.QWidget, _CreateButton, _Frames):
-    MIN_CURRENT_BIT = 0
-    MAX_CURRENT_BIT = (1 << 8) - 1
-    CONSTANT_CURRENT = 0
-    CONSTANT_LIGHT = 1
-
-    def __init__(self):
-        QtWidgets.QWidget.__init__(self)
-        _Frames.__init__(self)
-        _CreateButton.__init__(self)
-        self.frames = {}
-        self.setLayout(QtWidgets.QGridLayout())
-        self.current_slider = Slider(minimum=ProbeLaser.MIN_CURRENT_BIT, maximum=ProbeLaser.MAX_CURRENT_BIT, unit="mA")
-        self.controller = controller.ProbeLaser(self)
-        self.laser_mode = QtWidgets.QComboBox()
-        self.photo_gain = QtWidgets.QComboBox()
-        self.current_display = QtWidgets.QLabel("0 mA")
-        self._init_frames()
-        self._init_slider()
-        self._init_buttons()
-        self.photo_gain.currentIndexChanged.connect(self.controller.update_photo_gain)
-        self.laser_mode.currentIndexChanged.connect(self.controller.update_probe_laser_mode)
-        self.frames["Measured Values"].layout().addWidget(self.current_display)
-        self.max_current_display = QtWidgets.QLineEdit("")
-        self.max_current_display.editingFinished.connect(self._max_current_changed)
-        self.frames["Maximum Current"].layout().addWidget(self.max_current_display, 0, 0)
-        self.frames["Maximum Current"].layout().addWidget(QtWidgets.QLabel("mA"), 0, 1)
-        self._init_signals()
-        self.controller.fire_configuration_change()
-
-    def _init_signals(self) -> None:
-        model.laser_signals.current_probe_laser.connect(self._update_current_slider)
-        model.laser_signals.photo_gain.connect(self._update_photo_gain)
-        model.laser_signals.probe_laser_mode.connect(self._update_mode)
-        model.laser_signals.data_display.connect(self._update_current)
-        model.laser_signals.max_current_probe_laser.connect(self._update_max_current)
-
-    @QtCore.pyqtSlot(hardware.laser.Data)
-    def _update_current(self, value: hardware.laser.Data) -> None:
-        self.current_display.setText(str(value.probe_laser_current) + " mA")
-
-    @functools.singledispatchmethod
-    def _update_max_current(self, value: int):
-        self.max_current_display.setText(str(value) + " mA")
-
-    @_update_max_current.register
-    def _(self, value: float):
-        self.max_current_display.setText(str(round(value, 2)) + " mA")
-
-    def _max_current_changed(self) -> None:
-        return self.controller.update_max_current_probe_laser(self.max_current_display.text())
-
-    def _init_frames(self) -> None:
-        self.create_frame(master=self, title="Maximum Current", x_position=0, y_position=0)
-        self.create_frame(master=self, title="Measured Values", x_position=1, y_position=0)
-        self.create_frame(master=self, title="Current", x_position=2, y_position=0)
-        self.create_frame(master=self, title="Mode", x_position=3, y_position=0)
-        self.create_frame(master=self, title="Photo Diode Gain", x_position=4, y_position=0)
-        self.create_frame(master=self, title="Configuration", x_position=5, y_position=0)
-
-    def _init_slider(self) -> None:
-        self.frames["Current"].layout().addWidget(self.current_slider)
-        self.current_slider.slider.valueChanged.connect(self.controller.update_current_probe_laser)
-
-    @QtCore.pyqtSlot(int, float)
-    def _update_current_slider(self, index: int, value: float) -> None:
-        self.current_slider.slider.setValue(index)
-        self.current_slider.update_value(value)
-
-    def _init_buttons(self) -> None:
-        sub_layout = QtWidgets.QWidget()
-        sub_layout.setLayout(QtWidgets.QVBoxLayout())
-        self.laser_mode.addItem("Constant Light")
-        self.laser_mode.addItem("Constant Current")
-        sub_layout.layout().addWidget(self.laser_mode)
-        self.frames["Mode"].layout().addWidget(sub_layout)
-        sub_layout = QtWidgets.QWidget()
-        sub_layout.setLayout(QtWidgets.QVBoxLayout())
-        self.photo_gain.addItem("1x")
-        self.photo_gain.addItem("2x")
-        self.photo_gain.addItem("3x")
-        self.photo_gain.addItem("4x")
-        sub_layout.layout().addWidget(self.photo_gain)
-        self.frames["Photo Diode Gain"].layout().addWidget(sub_layout)
-        config = QtWidgets.QWidget()
-        config.setLayout(QtWidgets.QHBoxLayout())
-        self.create_button(master=config, title="Save Configuration", slot=self.controller.save_configuration)
-        self.create_button(master=config, title="Load Configuration", slot=self.controller.load_configuration)
-        self.create_button(master=config, title="Apply Configuration", slot=self.controller.load_configuration)
-        self.frames["Configuration"].layout().addWidget(config, 3, 0)
-
-    @QtCore.pyqtSlot(int)
-    def _update_photo_gain(self, index: int) -> None:
-        self.photo_gain.setCurrentIndex(index)
-
-    @QtCore.pyqtSlot(int)
-    def _update_mode(self, index: int):
-        self.laser_mode.setCurrentIndex(index)
-
-
-class TecTextFields:
-    def __init__(self):
-        self.p_value = QtWidgets.QLineEdit()
-        self.i_value = [QtWidgets.QLineEdit(), QtWidgets.QLineEdit()]
-        self.d_value = QtWidgets.QLineEdit()
-        self.setpoint_temperature = QtWidgets.QLineEdit()
-        self.loop_time = QtWidgets.QLineEdit()
-        self.reference_resistor = QtWidgets.QLineEdit()
-        self.max_power = QtWidgets.QLineEdit()
-
-
-class Tec(QtWidgets.QWidget, _Frames, _CreateButton):
-    def __init__(self, laser: str):
-        QtWidgets.QWidget.__init__(self)
-        _Frames.__init__(self)
-        _CreateButton.__init__(self)
-        self.laser = laser
-        self.setLayout(QtWidgets.QGridLayout())
-        self.controller = controller.Tec(laser, self)
-        self.text_fields = TecTextFields()
-        self.temperature_display = QtWidgets.QLabel("NaN °C")
-        self._init_frames()
-        self._init_text_fields()
-        self._init_buttons()
-        self._init_signals()
-        self.controller.fire_configuration_change()
-
-    def _init_signals(self) -> None:
-        model.signals.tec_data_display.connect(self.update_temperature)
-        model.tec_signals[self.laser].p_value.connect(
-            Tec._update_text_field(self.text_fields.p_value))
-        model.tec_signals[self.laser].i_1_value.connect(
-            Tec._update_text_field(self.text_fields.i_value[0]))
-        model.tec_signals[self.laser].i_2_value.connect(
-            Tec._update_text_field(self.text_fields.i_value[1]))
-        model.tec_signals[self.laser].d_value.connect(
-            Tec._update_text_field(self.text_fields.d_value))
-        model.tec_signals[self.laser].setpoint_temperature.connect(
-            Tec._update_text_field(self.text_fields.setpoint_temperature))
-        model.tec_signals[self.laser].loop_time.connect(
-            Tec._update_text_field(self.text_fields.loop_time))
-        model.tec_signals[self.laser].reference_resistor.connect(
-            Tec._update_text_field(self.text_fields.reference_resistor))
-        model.tec_signals[self.laser].max_power.connect(
-            Tec._update_text_field(self.text_fields.max_power))
-        model.tec_signals[self.laser].mode.connect(self.update_mode)
-
-    def _init_frames(self) -> None:
-        self.create_frame(master=self, title="pid Configuration", x_position=0, y_position=0)
-        self.create_frame(master=self, title="System Settings", x_position=1, y_position=0)
-        self.create_frame(master=self, title="Temperature", x_position=2, y_position=0)
-        self.create_frame(master=self, title="Configuration", x_position=3, y_position=0)
-
-    @staticmethod
-    def _update_text_field(text_field: QtWidgets.QLineEdit):
-        @QtCore.pyqtSlot(float)
-        def update(value: float):
-            text_field.setText(str(round(value, 2)))
-
-        return update
-
-    @QtCore.pyqtSlot(hardware.tec.Data)
-    def update_temperature(self, value: hardware.tec.Data) -> None:
-        self.temperature_display.setText(str(value.actual_temperature[self.laser]) + " °C")
-
-    @QtCore.pyqtSlot(model.TecMode)
-    def update_mode(self, mode: model.TecMode):
-        if mode == model.TecMode.COOLING:
-            toggle_button(False, self.buttons["Heat"])
-            toggle_button(True, self.buttons["Cool"])
-        else:
-            toggle_button(True, self.buttons["Heat"])
-            toggle_button(False, self.buttons["Cool"])
-
-    def _init_text_fields(self) -> None:
-        self.frames["pid Configuration"].layout().addWidget(QtWidgets.QLabel("P Value"), 0, 0)
-        self.frames["pid Configuration"].layout().addWidget(self.text_fields.p_value, 0, 1)
-        self.text_fields.p_value.editingFinished.connect(self.p_value_changed)
-
-        self.frames["pid Configuration"].layout().addWidget(QtWidgets.QLabel("I<sub>1</sub> Value"), 1, 0)
-        self.frames["pid Configuration"].layout().addWidget(self.text_fields.i_value[0], 1, 1)
-        self.text_fields.i_value[0].editingFinished.connect(self.i_1_value_changed)
-
-        self.frames["pid Configuration"].layout().addWidget(QtWidgets.QLabel("I<sub>2</sub> Value"), 2, 0)
-        self.frames["pid Configuration"].layout().addWidget(self.text_fields.i_value[1], 2, 1)
-        self.text_fields.i_value[1].editingFinished.connect(self.i_2_value_changed)
-
-        self.frames["pid Configuration"].layout().addWidget(QtWidgets.QLabel("D Value"), 3, 0)
-        self.frames["pid Configuration"].layout().addWidget(self.text_fields.d_value, 3, 1)
-        self.text_fields.d_value.editingFinished.connect(self.d_value_changed)
-
-        self.frames["System Settings"].layout().addWidget(QtWidgets.QLabel("Setpoint Temperature"), 0, 0)
-        self.frames["System Settings"].layout().addWidget(self.text_fields.setpoint_temperature, 0, 1)
-        self.text_fields.setpoint_temperature.editingFinished.connect(self.setpoint_temperature_changed)
-
-        self.frames["System Settings"].layout().addWidget(QtWidgets.QLabel("Loop Time"), 1, 0)
-        self.frames["System Settings"].layout().addWidget(self.text_fields.loop_time, 1, 1)
-        self.text_fields.loop_time.editingFinished.connect(self.loop_time_changed)
-
-        self.frames["System Settings"].layout().addWidget(QtWidgets.QLabel("Reference Resistor"), 2, 0)
-        self.frames["System Settings"].layout().addWidget(self.text_fields.reference_resistor, 2, 1)
-        self.text_fields.reference_resistor.editingFinished.connect(self.reference_resistor_changed)
-
-        self.frames["System Settings"].layout().addWidget(QtWidgets.QLabel("Max Power"), 3, 0)
-        self.frames["System Settings"].layout().addWidget(self.text_fields.max_power, 3, 1)
-        self.text_fields.max_power.editingFinished.connect(self.max_power_changed)
-
-        self.frames["Temperature"].layout().addWidget(self.temperature_display)
-
-    def d_value_changed(self) -> None:
-        self.controller.update_d_value(self.text_fields.d_value.text())
-
-    def i_1_value_changed(self) -> None:
-        self.controller.update_i_1_value(self.text_fields.i_value[0].text())
-
-    def i_2_value_changed(self) -> None:
-        self.controller.update_i_2_value(self.text_fields.i_value[1].text())
-
-    def p_value_changed(self) -> None:
-        self.controller.update_p_value(self.text_fields.p_value.text())
-
-    def setpoint_temperature_changed(self) -> None:
-        self.controller.update_setpoint_temperature(self.text_fields.setpoint_temperature.text())
-
-    def loop_time_changed(self) -> None:
-        self.controller.update_loop_time(self.text_fields.loop_time.text())
-
-    def reference_resistor_changed(self) -> None:
-        self.controller.update_reference_resistor(self.text_fields.reference_resistor.text())
-
-    def max_power_changed(self) -> None:
-        self.controller.update_max_power(self.text_fields.max_power.text())
-
-    def _init_buttons(self) -> None:
-        config = QtWidgets.QWidget()
-        config.setLayout(QtWidgets.QHBoxLayout())
-        self.create_button(master=config, title="Save Configuration", slot=self.controller.save_configuration)
-        self.create_button(master=config, title="Load Configuration", slot=self.controller.load_configuration)
-        self.create_button(master=config, title="Apply Configuration", slot=self.controller.load_configuration)
-        self.frames["Configuration"].layout().addWidget(config, 3, 0)
-
-        self.create_button(master=self.frames["Temperature"], title="Heat", slot=self.controller.set_heating)
-        self.create_button(master=self.frames["Temperature"], title="Cool", slot=self.controller.set_cooling)
-
-
-class _MatplotlibColors:
-    BLUE = "#045993"
-    ORANGE = "#db6000"
-    GREEN = "#118011"
-
-
-class _Plotting(pg.PlotWidget):
-    def __init__(self):
-        pg.PlotWidget.__init__(self)
-        pg.setConfigOption('leftButtonPan', False)
-        pg.setConfigOptions(antialias=True)
-        pg.setConfigOption('background', "white")
-        pg.setConfigOption('foreground', 'k')
-        self.window = pg.GraphicsLayoutWidget()
-        self.plot = self.window.addPlot()
-        self.curves = self.plot.plot(pen=pg.mkPen(_MatplotlibColors.BLUE))
-        self.plot.showGrid(x=True, y=True)
-        self.plot.addLegend()
-
-    @abc.abstractmethod
-    def update_data(self, data: pd.DataFrame) -> None:
-        ...
-
-    @abc.abstractmethod
-    def update_data_live(self, data: model.Buffer) -> None:
-        ...
-
-
-class DC(_Plotting):
-    def __init__(self):
-        _Plotting.__init__(self)
-        self.curves = [self.plot.plot(pen=pg.mkPen(_MatplotlibColors.BLUE), name="DC CH1"),
-                       self.plot.plot(pen=pg.mkPen(_MatplotlibColors.ORANGE), name="DC CH2"),
-                       self.plot.plot(pen=pg.mkPen(_MatplotlibColors.GREEN), name="DC CH3")]
-        self.plot.setLabel(axis="bottom", text="Time [s]")
-        self.plot.setLabel(axis="left", text="Intensity [V]")
-        model.signals.decimation.connect(self.update_data)
-        model.signals.decimation_live.connect(self.update_data_live)
-
-    def update_data(self, data: pd.DataFrame) -> None:
-        for channel in range(3):
-            try:
-                self.curves[channel].setData(data[f"DC CH{channel + 1}"].to_numpy())
-            except KeyError:
-                self.curves[channel].setData(data[f"PD{channel + 1}"].to_numpy())
-
-    def update_data_live(self, data: model.PTIBuffer) -> None:
-        for channel in range(3):
-            self.curves[channel].setData(data.dc_values[channel])
-
-
-class Amplitudes(_Plotting):
-    def __init__(self):
-        _Plotting.__init__(self)
-        self.curves = [self.plot.scatterPlot(pen=pg.mkPen(_MatplotlibColors.BLUE),
-                                             brush=pg.mkBrush(_MatplotlibColors.BLUE),
-                                             name="Amplitude CH1"),
-                       self.plot.scatterPlot(pen=pg.mkPen(_MatplotlibColors.ORANGE),
-                                             brush=pg.mkBrush(_MatplotlibColors.ORANGE),
-                                             name="Amplitude CH2"),
-                       self.plot.scatterPlot(pen=pg.mkPen(_MatplotlibColors.GREEN),
-                                             brush=pg.mkBrush(_MatplotlibColors.GREEN),
-                                             name="Amplitude CH3")]
-        self.plot.setLabel(axis="bottom", text="Time [s]")
-        self.plot.setLabel(axis="left", text="Amplitude [V]")
-        model.signals.characterization.connect(self.update_data)
-        model.signals.characterization_live.connect(self.update_data_live)
-
-    def update_data(self, data: pd.DataFrame) -> None:
-        for channel in range(3):
-            self.curves[channel].setData(data.index, data[f"Amplitude CH{channel + 1}"].to_numpy())
-
-    def update_data_live(self, data: model.CharacterisationBuffer) -> None:
-        for channel in range(3):
-            self.curves[channel].setData(data.time, data.amplitudes[channel])
-
-
-class OutputPhases(_Plotting):
-    def __init__(self):
-        _Plotting.__init__(self)
-        self.curves = [self.plot.scatterPlot(pen=pg.mkPen(_MatplotlibColors.ORANGE), name="Output Phase CH2",
-                                             brush=pg.mkBrush(_MatplotlibColors.ORANGE)),
-                       self.plot.scatterPlot(pen=pg.mkPen(_MatplotlibColors.GREEN), name="Output Phase CH3",
-                                             brush=pg.mkBrush(_MatplotlibColors.GREEN))]
-        self.plot.setLabel(axis="bottom", text="Time [s]")
-        self.plot.setLabel(axis="left", text="Output Phase [deg]")
-        model.signals.characterization.connect(self.update_data)
-        model.signals.characterization_live.connect(self.update_data_live)
-
-    def update_data(self, data: pd.DataFrame) -> None:
-        for channel in range(2):
-            self.curves[channel].setData(data.index, data[f"Output Phase CH{channel + 2}"].to_numpy())
-
-    def update_data_live(self, data: model.CharacterisationBuffer) -> None:
-        for channel in range(2):
-            self.curves[channel].setData(data.time, data.output_phases[channel])
-
-
-class InterferometricPhase(_Plotting):
-    def __init__(self):
-        _Plotting.__init__(self)
-        self.curves = self.plot.plot(pen=pg.mkPen(_MatplotlibColors.BLUE))
-        self.plot.setLabel(axis="bottom", text="Time [s]")
-        self.plot.setLabel(axis="left", text="Interferometric Phase [rad]")
-        model.signals.inversion.connect(self.update_data)
-        model.signals.inversion_live.connect(self.update_data_live)
-
-    def update_data(self, data: pd.DataFrame) -> None:
-        self.curves.setData(data["Interferometric Phase"].to_numpy())
-
-    def update_data_live(self, data: model.PTIBuffer) -> None:
-        self.curves.setData(data.time, data.interferometric_phase)
-
-
-class Sensitivity(_Plotting):
-    def __init__(self):
-        _Plotting.__init__(self)
-        self.curves = [self.plot.plot(pen=pg.mkPen(_MatplotlibColors.BLUE), name="CH1"),
-                       self.plot.plot(pen=pg.mkPen(_MatplotlibColors.ORANGE), name="CH2"),
-                       self.plot.plot(pen=pg.mkPen(_MatplotlibColors.GREEN), name="CH3")]
-        self.plot.setLabel(axis="bottom", text="Time [s]")
-        self.plot.setLabel(axis="left", text="Sensitivity [V/rad]")
-        model.signals.inversion.connect(self.update_data)
-        model.signals.inversion_live.connect(self.update_data_live)
-
-    def update_data(self, data: pd.DataFrame) -> None:
-        for channel in range(3):
-            self.curves[channel].setData(data[f"Sensitivity CH{channel + 1}"].to_numpy())
-
-    def update_data_live(self, data: model.PTIBuffer) -> None:
-        for channel in range(3):
-            self.curves[channel].setData(data.time, data.sensitivity[channel])
-
-
-class Symmetry(_Plotting):
-    def __init__(self):
-        _Plotting.__init__(self)
-        self.curves = [self.plot.scatterPlot(pen=pg.mkPen(_MatplotlibColors.BLUE), name="Absolute Symmetry",
-                                             brush=pg.mkBrush(_MatplotlibColors.BLUE)),
-                       self.plot.scatterPlot(pen=pg.mkPen(_MatplotlibColors.ORANGE), name="Relative Symmetry",
-                                             brush=pg.mkBrush(_MatplotlibColors.ORANGE))]
-        self.plot.setLabel(axis="bottom", text="Time [s]")
-        self.plot.setLabel(axis="left", text="Symmetry [%]")
-        model.signals.characterization.connect(self.update_data)
-        model.signals.characterization_live.connect(self.update_data_live)
-
-    def update_data(self, data: pd.DataFrame) -> None:
-        self.curves[0].setData(data.index, data["Symmetry"].to_numpy())
-        self.curves[1].setData(data.index, data["Relative Symmetry"].to_numpy())
-
-    def update_data_live(self, data: model.CharacterisationBuffer) -> None:
-        self.curves[0].setData(data.time, data.symmetry)
-        self.curves[1].setData(data.time, data.relative_symmetry)
-
-
-class PTISignal(_Plotting):
-    def __init__(self):
-        _Plotting.__init__(self)
-        self.curves = {"PTI Signal": self.plot.scatterPlot(pen=pg.mkPen(_MatplotlibColors.BLUE), name="1 s", size=6),
-                       "PTI Signal Mean": self.plot.plot(pen=pg.mkPen(_MatplotlibColors.ORANGE), name="60 s Mean")}
-        self.plot.setLabel(axis="bottom", text="Time [s]")
-        self.plot.setLabel(axis="left", text="PTI Signal [µrad]")
-        model.signals.inversion.connect(self.update_data)
-        model.signals.inversion_live.connect(self.update_data_live)
-
-    def update_data(self, data: pd.DataFrame) -> None:
-        try:
-            self.curves["PTI Signal"].setData(data["PTI Signal"].to_numpy())
-            self.curves["PTI Signal Mean"].setData(data["PTI Signal 60 s Mean"].to_numpy())
-        except KeyError:
-            pass
-
-    def update_data_live(self, data: model.PTIBuffer) -> None:
-        self.curves["PTI Signal"].setData(data.time, data.pti_signal)
-        self.curves["PTI Signal Mean"].setData(data.time, data.pti_signal_mean)
-
-
-class PumpLaserCurrent(_Plotting):
-    def __init__(self):
-        _Plotting.__init__(self)
-        self.curves = self.plot.plot(pen=pg.mkPen(_MatplotlibColors.BLUE))
-        self.plot.setLabel(axis="bottom", text="Time [s]")
-        self.plot.setLabel(axis="left", text="Current [mA]")
-        model.laser_signals.data.connect(self.update_data_live)
-
-    def update_data(self, data: pd.DataFrame) -> None:
-        raise NotImplementedError
-
-    def update_data_live(self, data: model.LaserBuffer) -> None:
-        self.curves.setData(data.time, data.pump_laser_current)
-
-
-class PumpLaserVoltage(_Plotting):
-    def __init__(self):
-        _Plotting.__init__(self)
-        self.curves = self.plot.plot(pen=pg.mkPen(_MatplotlibColors.BLUE))
-        self.plot.setLabel(axis="bottom", text="Time [s]")
-        self.plot.setLabel(axis="left", text="Voltage [V]")
-        model.laser_signals.data.connect(self.update_data_live)
-
-    def update_data(self, data: pd.DataFrame) -> None:
-        raise NotImplementedError("There is no need to plot laser data offline")
-
-    def update_data_live(self, data: model.LaserBuffer) -> None:
-        self.curves.setData(data.time, data.pump_laser_voltage)
-
-
-class ProbeLaserCurrent(_Plotting):
-    def __init__(self):
-        _Plotting.__init__(self)
-        self.curves = self.plot.plot(pen=pg.mkPen(_MatplotlibColors.BLUE))
-        self.plot.setLabel(axis="bottom", text="Time [s]")
-        self.plot.setLabel(axis="left", text="Current [mA]")
-        model.laser_signals.data.connect(self.update_data_live)
-
-    def update_data(self, data: pd.DataFrame) -> None:
-        raise NotImplementedError("There is no need to plot laser data offline")
-
-    def update_data_live(self, data: model.LaserBuffer) -> None:
-        self.curves.setData(data.time, data.probe_laser_current)
-
-
-class TecTemperature(_Plotting):
-    ACTUAL = 0
-    MEASURAED = 1
-
-    def __init__(self, laser: str):
-        _Plotting.__init__(self)
-        self.curves = [self.plot.plot(pen=pg.mkPen(_MatplotlibColors.BLUE), name="Setpoint Temperature"),
-                       self.plot.plot(pen=pg.mkPen(_MatplotlibColors.ORANGE), name="Measured Temperature")]
-        self.plot.setLabel(axis="bottom", text="Time [s]")
-        self.plot.setLabel(axis="left", text="Temperature [°C]")
-        if laser == "Pump Laser":
-            self.laser = model.TecBuffer.PUMP_LASER
-        else:
-            self.laser = model.TecBuffer.PROBE_LASER
-        model.signals.tec_data.connect(self.update_data_live)
-
-    def update_data(self, data: pd.DataFrame) -> None:
-        raise NotImplementedError("There is no need to plot laser data offline")
-
-    def update_data_live(self, data: model.TecBuffer) -> None:
-        self.curves[TecTemperature.ACTUAL].setData(data.time, data.actual_value[self.laser])
-        self.curves[TecTemperature.MEASURAED].setData(data.time, data.set_point[self.laser])
+import abc
+import collections
+import enum
+import functools
+import typing
+from typing import NamedTuple, Union
+
+import pandas as pd
+import pyqtgraph as pg
+from PyQt5 import QtWidgets, QtCore, QtGui
+from PyQt5.QtCore import Qt
+
+from .. import hardware
+from . import controller
+from . import model
+
+
+class MainWindow(QtWidgets.QMainWindow):
+    HORIZONTAL_SIZE = 1200
+    VERTICAL_SIZE = 900
+
+    def __init__(self, main_controller):
+        QtWidgets.QMainWindow.__init__(self)
+        self.setWindowTitle("MiniPTI")
+        self.setWindowIcon(QtGui.QIcon("images/icon.png"))
+        self.main_controller = main_controller
+        self.tab_bar = QtWidgets.QTabWidget(self)
+        self.setCentralWidget(self.tab_bar)
+        self.tabs: Union[Tab, None] = None
+        self.current_pump_laser = PumpLaserCurrent()
+        self.current_probe_laser = ProbeLaserCurrent()
+        self.temperature_probe_laser = TecTemperature(channel=model.Tec.PROBE_LASER)
+        self.temperature_pump_laser = TecTemperature(channel=model.Tec.PUMP_LASER)
+        self.dc = DC()
+        self.amplitudes = Amplitudes()
+        self.output_phases = OutputPhases()
+        self.interferometric_phase = InterferometricPhase()
+        self.sensitivity = Sensitivity()
+        self.symmetry = Symmetry()
+        self.pti_signal = PTISignal()
+        self._init_tabs()
+        self.resize(MainWindow.HORIZONTAL_SIZE, MainWindow.VERTICAL_SIZE)
+        self.show()
+
+    def _init_pump_laser_tab(self) -> QtWidgets.QTabWidget:
+        tab = QtWidgets.QTabWidget()
+        sub_layout = QtWidgets.QSplitter()
+        pump_laser = PumpLaser()
+        pump_laser_tab = QtWidgets.QTabWidget()
+        pump_laser_tab.setLayout(QtWidgets.QHBoxLayout())
+        sub_layout.insertWidget(0, pump_laser)
+        sub_layout.insertWidget(1, self.current_pump_laser.window)
+        pump_laser_tab.layout().addWidget(sub_layout)
+        tab.addTab(pump_laser_tab, "Laser Driver")
+        sub_layout = QtWidgets.QSplitter()
+        tec_tab = QtWidgets.QTabWidget()
+        tec_tab.setLayout(QtWidgets.QHBoxLayout())
+        sub_layout.insertWidget(0, Tec(model.Tec.PUMP_LASER))
+        sub_layout.insertWidget(1, self.temperature_pump_laser.window)
+        tec_tab.layout().addWidget(sub_layout)
+        tab.addTab(tec_tab, "Tec Driver")
+        return tab
+
+    def _init_probe_laser_tab(self) -> QtWidgets.QTabWidget:
+        tab = QtWidgets.QTabWidget()
+        sub_layout = QtWidgets.QSplitter()
+        probe_laser = ProbeLaser()
+        probe_laser_tab = QtWidgets.QTabWidget()
+        probe_laser_tab.setLayout(QtWidgets.QHBoxLayout())
+        sub_layout.insertWidget(0, probe_laser)
+        sub_layout.insertWidget(1, self.current_probe_laser.window)
+        probe_laser_tab.layout().addWidget(sub_layout)
+        tab.addTab(probe_laser_tab, "Laser Driver")
+        sub_layout = QtWidgets.QSplitter()
+        tec_tab = QtWidgets.QTabWidget()
+        tec_tab.setLayout(QtWidgets.QHBoxLayout())
+        sub_layout.insertWidget(0, Tec(model.Tec.PROBE_LASER))
+        sub_layout.insertWidget(1, self.temperature_probe_laser.window)
+        tec_tab.layout().addWidget(sub_layout)
+        tab.addTab(tec_tab, "Tec Driver")
+        return tab
+
+    def _init_tabs(self):
+        self.tabs = Tab(home=Home(self, self.main_controller),
+                        settings=Settings(self.main_controller),
+                        pump_laser=self._init_pump_laser_tab(),
+                        probe_laser=self._init_probe_laser_tab(),
+                        dc=QtWidgets.QTabWidget(),
+                        amplitudes=QtWidgets.QTabWidget(),
+                        output_phases=QtWidgets.QTabWidget(),
+                        sensitivity=QtWidgets.QTabWidget(),
+                        symmetry=QtWidgets.QTabWidget(),
+                        interferometric_phase=QtWidgets.QTabWidget(),
+                        pti_signal=QtWidgets.QTabWidget())
+        self.tab_bar.addTab(self.tabs.home, "Home")
+        self.tab_bar.addTab(self.tabs.settings, "Settings")
+        self.tab_bar.addTab(self.tabs.pump_laser, "Pump Laser")
+        self.tab_bar.addTab(self.tabs.probe_laser, "Probe Laser")
+        # DC Plot
+        self.tabs.dc.setLayout(QtWidgets.QHBoxLayout())
+        self.tabs.dc.layout().addWidget(self.dc.window)
+        self.tab_bar.addTab(self.tabs.dc, "DC Signals")
+        # Amplitudes Plot
+        self.tabs.amplitudes.setLayout(QtWidgets.QHBoxLayout())
+        self.tabs.amplitudes.layout().addWidget(self.amplitudes.window)
+        self.tab_bar.addTab(self.tabs.amplitudes, "Amplitudes")
+        # Output Phases Plot
+        self.tabs.output_phases.setLayout(QtWidgets.QHBoxLayout())
+        self.tabs.output_phases.layout().addWidget(self.output_phases.window)
+        self.tab_bar.addTab(self.tabs.output_phases, "Output Phases")
+        # Interferometric Phase Plot
+        self.tabs.interferometric_phase.setLayout(QtWidgets.QHBoxLayout())
+        self.tabs.interferometric_phase.layout().addWidget(self.interferometric_phase.window)
+        self.tab_bar.addTab(self.tabs.interferometric_phase, "Interferometric Phase")
+        # Sensitivity Plot
+        self.tabs.sensitivity.setLayout(QtWidgets.QHBoxLayout())
+        self.tabs.sensitivity.layout().addWidget(self.sensitivity.window)
+        self.tab_bar.addTab(self.tabs.sensitivity, "Sensitivity")
+        # Symmetry Plot
+        self.tabs.symmetry.setLayout(QtWidgets.QHBoxLayout())
+        self.tabs.symmetry.layout().addWidget(self.symmetry.window)
+        self.tab_bar.addTab(self.tabs.symmetry, "Symmetry")
+        # PTI Signal Plot
+        self.tabs.pti_signal.setLayout(QtWidgets.QHBoxLayout())
+        self.tabs.pti_signal.layout().addWidget(self.pti_signal.window)
+        self.tab_bar.addTab(self.tabs.pti_signal, "PTI Signal")
+
+    def closeEvent(self, close_event):
+        close = QtWidgets.QMessageBox.question(self, "QUIT", "Are you sure you want to close?",
+                                               QtWidgets.QMessageBox.StandardButton.Yes |
+                                               QtWidgets.QMessageBox.StandardButton.No)
+        if close == QtWidgets.QMessageBox.StandardButton.Yes:
+            close_event.accept()
+            self.main_controller.close()
+        else:
+            close_event.ignore()
+
+
+class Tab(NamedTuple):
+    home: "Home"
+    settings: "Settings"
+    pump_laser: QtWidgets.QTabWidget
+    probe_laser: QtWidgets.QTabWidget
+    dc: QtWidgets.QTabWidget
+    amplitudes: QtWidgets.QTabWidget
+    output_phases: QtWidgets.QTabWidget
+    interferometric_phase: QtWidgets.QTabWidget
+    sensitivity: QtWidgets.QTabWidget
+    symmetry: QtWidgets.QTabWidget
+    pti_signal: QtWidgets.QTabWidget
+
+
+class _Frames:
+    def __init__(self):
+        self.frames = {}  # type: dict[str, Union[QtWidgets.QGroupBox, QtWidgets.QDockWidget]]
+
+    def create_frame(self, master: QtWidgets.QWidget, title, x_position, y_position,
+                     x_span=1, y_span=1) -> None:
+        self.frames[title] = QtWidgets.QGroupBox()
+        self.frames[title].setTitle(title)
+        self.frames[title].setLayout(QtWidgets.QGridLayout())
+        try:
+            master.layout().addWidget(self.frames[title], x_position, y_position, x_span, y_span)
+        except TypeError:
+            master.layout().addWidget(self.frames[title])
+
+    @abc.abstractmethod
+    def _init_frames(self) -> None:
+        ...
+
+
+class _CreateButton:
+    def __init__(self):
+        self.buttons = {}  # type: dict[str, QtWidgets.QPushButton]
+
+    def create_button(self, master, title, slot, master_title="") -> None:
+        if master_title:
+            master_title += " "
+        self.buttons[master_title + title] = QtWidgets.QPushButton(master, text=title)
+        self.buttons[master_title + title].clicked.connect(slot)
+        master.layout().addWidget(self.buttons[master_title + title])
+
+    def _init_buttons(self) -> None:
+        ...
+
+
+class SettingsView(QtWidgets.QTableView):
+    def __init__(self, parent, settings_model: QtCore.QAbstractTableModel):
+        QtWidgets.QTableView.__init__(self, parent=parent)
+        header = self.horizontalHeader()
+        header.setStretchLastSection(True)
+        index = self.verticalHeader()
+        index.setSectionResizeMode(QtWidgets.QHeaderView.Stretch)
+        header.setSectionResizeMode(QtWidgets.QHeaderView.Stretch)
+        index.setStretchLastSection(True)
+        self.resizeColumnsToContents()
+        self.resizeRowsToContents()
+        self.setModel(settings_model)
+
+
+def toggle_button(checked, button: QtWidgets.QPushButton) -> None:
+    if checked:
+        button.setStyleSheet("background-color : lightgreen")
+    else:
+        button.setStyleSheet("background-color : light gray")
+
+
+class Home(QtWidgets.QTabWidget, _Frames, _CreateButton):
+    def __init__(self, main_window: QtWidgets.QMainWindow, main_app: QtWidgets.QApplication):
+        QtWidgets.QTabWidget.__init__(self)
+        _Frames.__init__(self)
+        _CreateButton.__init__(self)
+        self.setLayout(QtWidgets.QGridLayout())
+        self.controller = controller.Home(self, main_app)
+        self.logging_window = QtWidgets.QLabel()
+        self._init_frames()
+        model.signals.logging_update.connect(self.logging_update)
+        self.scroll = QtWidgets.QScrollArea(widgetResizable=True)
+        self.scroll.setWidgetResizable(True)
+        self.frames["Log"] = QtWidgets.QDockWidget("Log", self)
+        self.frames["Log"].setWidget(self.scroll)
+        self.frames["Battery"] = QtWidgets.QDockWidget("Battery", self)
+        self.charge_level = QtWidgets.QLabel("NaN % left")
+        self.minutes_left = QtWidgets.QLabel("NaN Minutes left")
+        sub_layout = QtWidgets.QWidget()
+        sub_layout.setMaximumWidth(150)
+        sub_layout.setLayout(QtWidgets.QVBoxLayout())
+        sub_layout.layout().addWidget(self.charge_level)
+        sub_layout.layout().addWidget(self.minutes_left)
+        self.frames["Battery"].setWidget(sub_layout)
+        self.scroll.setWidget(self.logging_window)
+        main_window.addDockWidget(Qt.BottomDockWidgetArea, self.frames["Log"])
+        main_window.addDockWidget(Qt.BottomDockWidgetArea, self.frames["Battery"])
+        main_window.setCorner(Qt.BottomRightCorner, Qt.RightDockWidgetArea)
+        self._init_buttons()
+        self._init_signals()
+        self.controller.fire_motherboard_configuration_change()
+        model.signals.battery_state.connect(self.update_battery_state)
+        model.signals.bypass.connect(self.update_clean_air)
+
+    @QtCore.pyqtSlot(model.Battery)
+    def update_battery_state(self, battery: model.Battery) -> None:
+        self.minutes_left.setText(f"Minutes left: {battery.minutes_left}")
+        self.charge_level.setText(f"{battery.percentage} % left")
+
+    def _init_frames(self) -> None:
+        sub_layout = QtWidgets.QWidget()
+        sub_layout.setLayout(QtWidgets.QGridLayout())
+        self.create_frame(master=self, title="Offline Processing", x_position=2, y_position=0)
+        self.create_frame(master=self, title="Plot Data", x_position=2, y_position=1)
+        self.create_frame(master=self, title="Measurement", x_position=3, y_position=0)
+        self.create_frame(master=self, title="Drivers", x_position=3, y_position=1)
+        self.create_frame(master=self, title="Pump Laser", x_position=4, y_position=0)
+        self.create_frame(master=self, title="Probe Laser", x_position=4, y_position=1)
+        self.layout().addWidget(sub_layout, 1, 1)
+
+    def _init_buttons(self) -> None:
+        # Offline Processing buttons
+        sub_layout = QtWidgets.QWidget()
+        sub_layout.setLayout(QtWidgets.QHBoxLayout())
+        self.frames["Offline Processing"].layout().addWidget(sub_layout)
+        self.create_button(master=sub_layout, title="Decimation", slot=self.controller.calculate_decimation)
+        self.create_button(master=sub_layout, title="Inversion", slot=self.controller.calculate_inversion)
+        self.create_button(master=sub_layout, title="Characterisation", slot=self.controller.calculate_characterisation)
+
+        # Plotting buttons
+        sub_layout = QtWidgets.QWidget(parent=self.frames["Plot Data"])
+        sub_layout.setLayout(QtWidgets.QHBoxLayout())
+        self.frames["Plot Data"].layout().addWidget(sub_layout)
+        self.create_button(master=sub_layout, title="Decimation", slot=self.controller.plot_dc)
+        self.create_button(master=sub_layout, title="Inversion", slot=self.controller.plot_inversion)
+        self.create_button(master=sub_layout, title="Characterisation", slot=self.controller.plot_characterisation)
+
+        # Driver buttons
+        sub_layout = QtWidgets.QWidget(parent=self.frames["Drivers"])
+        sub_layout.setLayout(QtWidgets.QHBoxLayout())
+        self.frames["Drivers"].layout().addWidget(sub_layout)
+        self.create_button(master=sub_layout, title="Scan Ports", slot=self.controller.find_devices)
+        self.create_button(master=sub_layout, title="Connect Devices", slot=self.controller.connect_devices)
+
+        # Measurement Buttons
+        sub_layout = QtWidgets.QWidget(parent=self.frames["Measurement"])
+        sub_layout.setLayout(QtWidgets.QHBoxLayout())
+        self.frames["Measurement"].layout().addWidget(sub_layout)
+        self.create_button(master=sub_layout, title="Run Measurement", slot=self.controller.enable_motherboard)
+        self.create_button(master=sub_layout, title="Clean Air", slot=self.controller.update_bypass)
+
+        # Pump Laser
+        sub_layout = QtWidgets.QWidget(parent=self.frames["Pump Laser"])
+        sub_layout.setLayout(QtWidgets.QHBoxLayout())
+        self.create_button(master=sub_layout, title="Enable Laser", slot=self.controller.enable_pump_laser,
+                           master_title="Pump Laser")
+        self.create_button(master=sub_layout, title="Enable Tec", slot=self.controller.enable_tec_pump_laser,
+                           master_title="Pump Laser")
+        self.frames["Pump Laser"].layout().addWidget(sub_layout)
+
+        # Probe Laser
+        sub_layout = QtWidgets.QWidget(parent=self.frames["Probe Laser"])
+        sub_layout.setLayout(QtWidgets.QHBoxLayout())
+        self.create_button(master=sub_layout, title="Enable Laser", slot=self.controller.enable_probe_laser,
+                           master_title="Probe Laser")
+        self.create_button(master=sub_layout, title="Enable Tec", slot=self.controller.enable_tec_probe_laser,
+                           master_title="Probe Laser")
+        self.frames["Probe Laser"].layout().addWidget(sub_layout)
+
+    def logging_update(self, log_queue: collections.deque) -> None:
+        self.logging_window.setText("".join(log_queue))
+
+    @QtCore.pyqtSlot(bool)
+    def update_run_measurement(self, state: bool) -> None:
+        toggle_button(state, self.buttons["Run Measurement"])
+
+    @QtCore.pyqtSlot(bool)
+    def update_clean_air(self, state: bool) -> None:
+        toggle_button(state, self.buttons["Clean Air"])
+
+    @QtCore.pyqtSlot(bool)
+    def update_enable_pump_laser(self, state: bool):
+        toggle_button(state, self.buttons["Pump Laser Enable Laser"])
+
+    @QtCore.pyqtSlot(bool)
+    def update_enable_probe_laser(self, state: bool):
+        toggle_button(state, self.buttons["Probe Laser Enable Laser"])
+
+    @QtCore.pyqtSlot(bool)
+    def update_enable_pump_laser_tec(self, state: bool):
+        toggle_button(state, self.buttons["Pump Laser Enable Tec"])
+
+    @QtCore.pyqtSlot(bool)
+    def update_enable_probe_laser_tec(self, state: bool):
+        toggle_button(state, self.buttons["Probe Laser Enable Tec"])
+
+    def _init_signals(self) -> None:
+        model.signals.daq_running.connect(self.update_run_measurement)
+        model.laser_signals.pump_laser_enabled.connect(self.update_enable_pump_laser)
+        model.laser_signals.probe_laser_enabled.connect(self.update_enable_probe_laser)
+        model.tec_signals[model.Tec.PUMP_LASER].enabled.connect(self.update_enable_pump_laser_tec)
+        model.tec_signals[model.Tec.PROBE_LASER].enabled.connect(self.update_enable_probe_laser_tec)
+
+
+class Settings(QtWidgets.QTabWidget, _Frames, _CreateButton):
+    def __init__(self, main_app: QtWidgets.QApplication):
+        QtWidgets.QTabWidget.__init__(self)
+        _Frames.__init__(self)
+        _CreateButton.__init__(self)
+        self.setLayout(QtWidgets.QGridLayout())
+        self.controller = controller.Home(self, main_app)
+        self.destination_folder = QtWidgets.QLabel(self.controller.destination_folder.folder)
+        self._init_frames()
+        self.settings = SettingsView(parent=self.frames["Configuration"], settings_model=self.controller.settings_model)
+        self.frames["Configuration"].layout().addWidget(self.settings)
+        self.destination_folder = QtWidgets.QLabel(self.controller.destination_folder.folder)
+        self.save_raw_data = QtWidgets.QCheckBox("Save Raw Data")
+        self.automatic_valve_switch = QtWidgets.QCheckBox("Automatic Valve Switch")
+        self.duty_cyle_valve = QtWidgets.QLabel("%")
+        self.period_valve = QtWidgets.QLabel("s")
+        self.duty_cycle_field = QtWidgets.QLineEdit()
+        self.period_field = QtWidgets.QLineEdit()
+        self.average_period = QtWidgets.QComboBox()
+        self._init_frames()
+        self._init_average_period_box()
+        self._init_buttons()
+        self._init_raw_data_button()
+        self._init_valves()
+        model.signals.destination_folder_changed.connect(self.update_destination_folder)
+        model.signals.valve_change.connect(self.update_valve)
+
+    @QtCore.pyqtSlot(hardware.motherboard.Valve)
+    def update_valve(self, valve: hardware.motherboard.Valve) -> None:
+        self.duty_cycle_field.setText(str(valve.duty_cycle))
+        self.period_field.setText(str(valve.period))
+        self.automatic_valve_switch.setChecked(valve.automatic_switch)
+
+    @QtCore.pyqtSlot(str)
+    def update_destination_folder(self, destionation_folder: str) -> None:
+        self.destination_folder.setText(destionation_folder)
+
+    def _init_average_period_box(self) -> None:
+        for i in range(80, 8000):
+            if i % 80 == 0:
+                self.average_period.addItem(f"{i / 8000 * 1000} ms")
+        for i in range(8000, 8000 * 4 + 1):
+            if i % 80 == 0:
+                self.average_period.addItem(f"{i / 8000 } s")
+        self.frames["Measurement"].layout().addWidget(self.average_period)
+
+    def _init_frames(self) -> None:
+        self.create_frame(master=self, title="File Path", x_position=2, y_position=1)
+        self.create_frame(master=self, title="Shutdown", x_position=0, y_position=1)
+        self.create_frame(master=self, title="Measurement", x_position=1, y_position=1)
+        self.create_frame(master=self, title="Configuration", x_position=0, y_position=0, x_span=5)
+        self.create_frame(master=self, title="Valve", x_position=3, y_position=1, x_span=2)
+
+    def _init_buttons(self) -> None:
+        sub_layout = QtWidgets.QWidget()
+        self.frames["Configuration"].layout().addWidget(sub_layout)
+        sub_layout.setLayout(QtWidgets.QHBoxLayout())
+        self.create_button(master=sub_layout, title="Save Settings", slot=self.controller.save_settings)
+        self.create_button(master=sub_layout, title="Save Settings As", slot=self.controller.save_settings_as)
+        self.create_button(master=sub_layout, title="Load Settings", slot=self.controller.load_settings)
+        self.frames["Measurement"].layout().addWidget(self.save_raw_data)
+
+        self.create_button(master=self.frames["Shutdown"], title="Shutdown and Close",
+                           slot=self.controller.shutdown_by_button)
+
+        # Valve Control
+        sub_layout = QtWidgets.QWidget(parent=self.frames["Valve"])
+        sub_layout.setLayout(QtWidgets.QGridLayout())
+        sub_layout.layout().addWidget(self.automatic_valve_switch, 0, 0)
+        sub_layout.layout().addWidget(QtWidgets.QLabel("Valve Period"), 1, 0)
+        sub_layout.layout().addWidget(self.period_field, 1, 1)
+        sub_layout.layout().addWidget(QtWidgets.QLabel("s"), 1, 2)
+        sub_layout.layout().addWidget(QtWidgets.QLabel("Valve Duty Cycle"), 2, 0)
+        sub_layout.layout().addWidget(self.duty_cycle_field, 2, 1)
+        sub_layout.layout().addWidget(QtWidgets.QLabel("%"), 2, 2)
+        self.frames["Valve"].layout().addWidget(sub_layout)
+        sub_layout = QtWidgets.QWidget(parent=self.frames["Valve"])
+        sub_layout.setLayout(QtWidgets.QHBoxLayout())
+        self.create_button(master=sub_layout, title="Save Settings",
+                           slot=self.controller.save_motherboard_configuration)
+        self.create_button(master=sub_layout, title="Load Settings",
+                           slot=self.controller.load_motherboard_configuration)
+        self.frames["Valve"].layout().addWidget(sub_layout)
+
+        sub_layout = QtWidgets.QWidget(parent=self.frames["File Path"])
+        sub_layout.setLayout(QtWidgets.QHBoxLayout())
+        self.frames["File Path"].layout().addWidget(sub_layout)
+        self.create_button(master=sub_layout, title="Destination Folder", slot=self.controller.set_destination_folder)
+        sub_layout.layout().addWidget(self.destination_folder)
+
+    def _init_raw_data_button(self) -> None:
+        self.save_raw_data.stateChanged.connect(self.controller.calculation_model.set_raw_data_saving)
+
+    def _init_valves(self) -> None:
+        self.automatic_valve_switch.stateChanged.connect(self._automatic_switch_changed)
+        self.period_field.editingFinished.connect(self._period_changed)
+        self.duty_cycle_field.editingFinished.connect(self._duty_cycle_changed)
+
+    def _automatic_switch_changed(self) -> None:
+        self.controller.update_automatic_valve_switch(self.automatic_valve_switch.isChecked())
+
+    def _period_changed(self) -> None:
+        self.controller.update_valve_period(self.period_field.text())
+
+    def _duty_cycle_changed(self) -> None:
+        self.controller.update_valve_duty_cycle(self.duty_cycle_field.text())
+
+
+class Slider(QtWidgets.QWidget):
+    def __init__(self, minimum=0, maximum=100, unit="%"):
+        QtWidgets.QWidget.__init__(self)
+        self.slider = QtWidgets.QSlider()
+        self.setLayout(QtWidgets.QHBoxLayout())
+        self.layout().addWidget(self.slider)
+        self.slider.setOrientation(QtCore.Qt.Orientation.Horizontal)
+        self.slider_value = QtWidgets.QLabel()
+        self.layout().addWidget(self.slider_value)
+        self.slider.setMinimum(minimum)
+        self.slider.setMaximum(maximum)
+        self.unit = unit
+        self.index_value = 0  # type: typing.Any
+
+    @functools.singledispatchmethod
+    def update_value(self, value: int) -> None:
+        self.slider_value.setText(f"{value} " + self.unit)
+
+    @update_value.register
+    def _(self, value: float) -> None:
+        self.slider_value.setText(f"{round(value, 2)} " + self.unit)
+
+
+class ModeIndices(enum.IntEnum):
+    DISABLED = 0
+    CONTINUOUS_WAVE = 1
+    PULSED = 2
+
+
+class _CreateConfigurationButtons(_CreateButton):
+    def __init__(self, parent_controller):
+        _CreateButton.__init__(self)
+        self.controller = parent_controller
+
+    def __call__(self) -> QtWidgets.QWidget:
+        sub_layout = QtWidgets.QWidget()
+        sub_layout.setLayout(QtWidgets.QHBoxLayout())
+        config = QtWidgets.QWidget()
+        config.setLayout(QtWidgets.QVBoxLayout())
+        self.create_button(master=sub_layout, title="Save Configuration",
+                           slot=self.controller.save_configuration)
+        self.create_button(master=sub_layout, title="Save Configuration As",
+                           slot=self.controller.save_configuration_as)
+        config.layout().addWidget(sub_layout)
+        sub_layout = QtWidgets.QWidget()
+        sub_layout.setLayout(QtWidgets.QHBoxLayout())
+        self.create_button(master=sub_layout, title="Load Configuration",
+                           slot=self.controller.load_configuration)
+        self.create_button(master=sub_layout, title="Apply Configuration",
+                           slot=self.controller.apply_configuration)
+        config.layout().addWidget(sub_layout)
+        return config
+
+
+class PumpLaser(QtWidgets.QWidget, _Frames, _CreateButton):
+    _MIN_DRIVER_BIT = 0
+    _MAX_DRIVER_BIT = (1 << 7) - 1
+    _MIN_CURRENT = 0
+    _MAX_CURRENT = (1 << 12) - 1
+
+    def __init__(self):
+        QtWidgets.QWidget.__init__(self)
+        _CreateButton.__init__(self)
+        _Frames.__init__(self)
+        self.model = None
+        self.setLayout(QtWidgets.QGridLayout())
+        self.current_display = QtWidgets.QLabel("0 mA")
+        self.voltage_display = QtWidgets.QLabel("0 V")
+        self.driver_voltage = Slider(minimum=PumpLaser._MIN_DRIVER_BIT, maximum=PumpLaser._MAX_DRIVER_BIT, unit="V")
+        self.current = [Slider(minimum=PumpLaser._MIN_CURRENT, maximum=PumpLaser._MAX_CURRENT, unit="Bit"),
+                        Slider(minimum=PumpLaser._MIN_CURRENT, maximum=PumpLaser._MAX_CURRENT, unit="Bit")]
+        self.mode_matrix = [[QtWidgets.QComboBox() for _ in range(3)], [QtWidgets.QComboBox() for _ in range(3)]]
+        self.controller = controller.PumpLaser(self)
+        self.create_configuration_buttons = _CreateConfigurationButtons(self.controller)
+        self._init_frames()
+        self._init_current_configuration()
+        self._init_voltage_configuration()
+        self._init_buttons()
+        self.frames["Driver Voltage"].layout().addWidget(self.driver_voltage)
+        self.frames["Measured Values"].layout().addWidget(self.current_display)
+        self.frames["Measured Values"].layout().addWidget(self.voltage_display)
+        self._init_signals()
+        self.controller.fire_configuration_change()
+
+    def _init_signals(self) -> None:
+        model.laser_signals.laser_voltage.connect(self._update_voltage_slider)
+        model.laser_signals.current_dac.connect(self._update_current_dac)
+        model.laser_signals.matrix_dac.connect(self._update_dac_matrix)
+        model.laser_signals.data_display.connect(self._update_current_voltage)
+
+    @QtCore.pyqtSlot(hardware.laser.Data)
+    def _update_current_voltage(self, value: hardware.laser.Data) -> None:
+        self.current_display.setText(str(value.high_power_laser_current) + " mA")
+        self.voltage_display.setText(str(value.high_power_laser_voltage) + " V")
+
+    def _init_voltage_configuration(self) -> None:
+        self.driver_voltage.slider.valueChanged.connect(self.controller.update_driver_voltage)
+
+    def _init_current_configuration(self) -> None:
+        self.current[0].slider.valueChanged.connect(self.controller.update_current_dac1)
+        self.current[1].slider.valueChanged.connect(self.controller.update_current_dac2)
+        for i in range(3):
+            self.mode_matrix[0][i].currentIndexChanged.connect(self.controller.update_dac1(i))
+            self.mode_matrix[1][i].currentIndexChanged.connect(self.controller.update_dac2(i))
+
+    @QtCore.pyqtSlot(int, list)
+    def _update_dac_matrix(self, dac_number: int, configuration: typing.Annotated[list[int], 3]) -> None:
+        for channel in range(3):
+            if configuration[channel] == model.Mode.CONTINUOUS_WAVE:
+                self.mode_matrix[dac_number][channel].setCurrentIndex(ModeIndices.CONTINUOUS_WAVE)
+            elif configuration[channel] == model.Mode.PULSED:
+                self.mode_matrix[dac_number][channel].setCurrentIndex(ModeIndices.PULSED)
+            elif configuration[channel] == model.Mode.DISABLED:
+                self.mode_matrix[dac_number][channel].setCurrentIndex(ModeIndices.DISABLED)
+
+    @QtCore.pyqtSlot(int, float)
+    def _update_voltage_slider(self, index: int, value: float) -> None:
+        self.driver_voltage.slider.setValue(index)
+        self.driver_voltage.update_value(value)
+
+    @QtCore.pyqtSlot(int, int)
+    def _update_current_dac(self, dac: int, index: int) -> None:
+        self.current[dac].slider.setValue(index)
+        self.current[dac].update_value(index)
+
+    def _init_frames(self) -> None:
+        self.create_frame(master=self, title="Measured Values", x_position=1, y_position=0)
+        self.create_frame(master=self, title="Driver Voltage", x_position=2, y_position=0)
+        for i in range(1, 3):
+            self.create_frame(master=self, title=f"Current {i}", x_position=i + 2, y_position=0)
+        self.create_frame(master=self, title="Configuration", x_position=5, y_position=0)
+
+    def _init_buttons(self) -> None:
+        dac_inner_frames = [QtWidgets.QWidget() for _ in range(2)]  # For slider and button-matrices
+        for j in range(2):
+            dac_inner_frames[j].setLayout(QtWidgets.QGridLayout())
+            self.frames[f"Current {j + 1}"].layout().addWidget(self.current[j])
+            for i in range(3):
+                sub_frames = [QtWidgets.QWidget() for _ in range(3)]
+                sub_frames[i].setLayout(QtWidgets.QVBoxLayout())
+                dac_inner_frames[j].layout().addWidget(sub_frames[i], 1, i)
+                self.mode_matrix[j][i].addItem("Disabled")
+                self.mode_matrix[j][i].addItem("Continuous Wave")
+                self.mode_matrix[j][i].addItem("Pulsed Mode")
+                sub_frames[i].layout().addWidget(QtWidgets.QLabel(f"Channel {i + 1}"))
+                sub_frames[i].layout().addWidget(self.mode_matrix[j][i])
+            self.frames[f"Current {j + 1}"].layout().addWidget(dac_inner_frames[j])
+        config = self.create_configuration_buttons()
+        self.frames["Configuration"].layout().addWidget(config, 3, 0)
+        self.frames["Configuration"].layout().addWidget(config, 4, 0)
+
+
+class ProbeLaser(QtWidgets.QWidget, _CreateButton, _Frames):
+    MIN_CURRENT_BIT = 5
+    MAX_CURRENT_BIT = (1 << 8) - 1
+    CONSTANT_CURRENT = 0
+    CONSTANT_LIGHT = 1
+
+    def __init__(self):
+        QtWidgets.QWidget.__init__(self)
+        _Frames.__init__(self)
+        _CreateButton.__init__(self)
+        self.frames = {}
+        self.setLayout(QtWidgets.QGridLayout())
+        self.current_slider = Slider(minimum=ProbeLaser.MIN_CURRENT_BIT, maximum=ProbeLaser.MAX_CURRENT_BIT, unit="mA")
+        self.controller = controller.ProbeLaser(self)
+        self.laser_mode = QtWidgets.QComboBox()
+        self.photo_gain = QtWidgets.QComboBox()
+        self.current_display = QtWidgets.QLabel("0")
+        self.create_configuration_buttons = _CreateConfigurationButtons(self.controller)
+        self._init_frames()
+        self._init_slider()
+        self._init_buttons()
+        self.photo_gain.currentIndexChanged.connect(self.controller.update_photo_gain)
+        self.laser_mode.currentIndexChanged.connect(self.controller.update_probe_laser_mode)
+        self.frames["Measured Values"].layout().addWidget(self.current_display)
+        self.max_current_display = QtWidgets.QLineEdit("")
+        self.max_current_display.editingFinished.connect(self._max_current_changed)
+        self.frames["Maximum Current"].layout().addWidget(self.max_current_display, 0, 0)
+        self.frames["Maximum Current"].layout().addWidget(QtWidgets.QLabel("mA"), 0, 1)
+        self._init_signals()
+        self.controller.fire_configuration_change()
+
+    def _init_signals(self) -> None:
+        model.laser_signals.current_probe_laser.connect(self._update_current_slider)
+        model.laser_signals.photo_gain.connect(self._update_photo_gain)
+        model.laser_signals.probe_laser_mode.connect(self._update_mode)
+        model.laser_signals.data_display.connect(self._update_current)
+        model.laser_signals.max_current_probe_laser.connect(self._update_max_current)
+
+    @QtCore.pyqtSlot(hardware.laser.Data)
+    def _update_current(self, value: hardware.laser.Data) -> None:
+        self.current_display.setText(str(value.low_power_laser_current))
+
+    @functools.singledispatchmethod
+    def _update_max_current(self, value: int):
+        self.max_current_display.setText(str(value))
+
+    @_update_max_current.register
+    def _(self, value: float):
+        self.max_current_display.setText(str(round(value, 2)))
+
+    def _max_current_changed(self) -> None:
+        return self.controller.update_max_current_probe_laser(self.max_current_display.text())
+
+    def _init_frames(self) -> None:
+        self.create_frame(master=self, title="Maximum Current", x_position=0, y_position=0)
+        self.create_frame(master=self, title="Measured Values", x_position=1, y_position=0)
+        self.create_frame(master=self, title="Current", x_position=2, y_position=0)
+        self.create_frame(master=self, title="Mode", x_position=3, y_position=0)
+        self.create_frame(master=self, title="Photo Diode Gain", x_position=4, y_position=0)
+        self.create_frame(master=self, title="Configuration", x_position=5, y_position=0)
+
+    def _init_slider(self) -> None:
+        self.frames["Current"].layout().addWidget(self.current_slider)
+        self.current_slider.slider.valueChanged.connect(self.controller.update_current_probe_laser)
+
+    @QtCore.pyqtSlot(int, float)
+    def _update_current_slider(self, index: int, value: float) -> None:
+        self.current_slider.slider.setValue(index)
+        self.current_slider.update_value(value)
+
+    def _init_buttons(self) -> None:
+        sub_layout = QtWidgets.QWidget()
+        sub_layout.setLayout(QtWidgets.QVBoxLayout())
+        self.laser_mode.addItem("Constant Light")
+        self.laser_mode.addItem("Constant Current")
+        sub_layout.layout().addWidget(self.laser_mode)
+        self.frames["Mode"].layout().addWidget(sub_layout)
+        sub_layout = QtWidgets.QWidget()
+        sub_layout.setLayout(QtWidgets.QVBoxLayout())
+        self.photo_gain.addItem("1x")
+        self.photo_gain.addItem("2x")
+        self.photo_gain.addItem("3x")
+        self.photo_gain.addItem("4x")
+        sub_layout.layout().addWidget(self.photo_gain)
+        self.frames["Photo Diode Gain"].layout().addWidget(sub_layout)
+        config = self.create_configuration_buttons()
+        self.frames["Configuration"].layout().addWidget(config, 3, 0)
+
+    @QtCore.pyqtSlot(int)
+    def _update_photo_gain(self, index: int) -> None:
+        self.photo_gain.setCurrentIndex(index)
+
+    @QtCore.pyqtSlot(int)
+    def _update_mode(self, index: int):
+        self.laser_mode.setCurrentIndex(index)
+
+
+class TecTextFields:
+    def __init__(self):
+        self.p_value = QtWidgets.QLineEdit()
+        self.i_value = [QtWidgets.QLineEdit(), QtWidgets.QLineEdit()]
+        self.d_value = QtWidgets.QLineEdit()
+        self.setpoint_temperature = QtWidgets.QLineEdit()
+        self.loop_time = QtWidgets.QLineEdit()
+        self.reference_resistor = QtWidgets.QLineEdit()
+        self.max_power = QtWidgets.QLineEdit()
+
+
+class Tec(QtWidgets.QWidget, _Frames, _CreateButton):
+    def __init__(self, laser: int):
+        QtWidgets.QWidget.__init__(self)
+        _Frames.__init__(self)
+        _CreateButton.__init__(self)
+        self.laser = laser
+        self.setLayout(QtWidgets.QGridLayout())
+        self.controller = controller.Tec(laser, self)
+        self.text_fields = TecTextFields()
+        self.temperature_display = QtWidgets.QLabel("NaN °C")
+        self.create_configuration_buttons = _CreateConfigurationButtons(self.controller)
+        self._init_frames()
+        self._init_text_fields()
+        self._init_buttons()
+        self._init_signals()
+        self.controller.fire_configuration_change()
+
+    def _init_signals(self) -> None:
+        model.signals.tec_data_display.connect(self.update_temperature)
+        model.tec_signals[self.laser].p_value.connect(Tec._update_text_field(self.text_fields.p_value))
+        model.tec_signals[self.laser].i_1_value.connect(Tec._update_text_field(self.text_fields.i_value[0]))
+        model.tec_signals[self.laser].i_2_value.connect(Tec._update_text_field(self.text_fields.i_value[1]))
+        model.tec_signals[self.laser].d_value.connect(Tec._update_text_field(self.text_fields.d_value))
+        model.tec_signals[self.laser].setpoint_temperature.connect(
+            Tec._update_text_field(self.text_fields.setpoint_temperature))
+        model.tec_signals[self.laser].loop_time.connect(Tec._update_text_field(self.text_fields.loop_time,
+                                                                               floating=False))
+        model.tec_signals[self.laser].reference_resistor.connect(
+            Tec._update_text_field(self.text_fields.reference_resistor))
+        model.tec_signals[self.laser].max_power.connect(Tec._update_text_field(self.text_fields.max_power,
+                                                                               floating=False))
+        model.tec_signals[self.laser].mode.connect(self.update_mode)
+
+    def _init_frames(self) -> None:
+        self.create_frame(master=self, title="PID Configuration", x_position=0, y_position=0)
+        self.create_frame(master=self, title="System Settings", x_position=1, y_position=0)
+        self.create_frame(master=self, title="Temperature", x_position=2, y_position=0)
+        self.create_frame(master=self, title="Configuration", x_position=3, y_position=0)
+
+    @staticmethod
+    def _update_text_field(text_field: QtWidgets.QLineEdit, floating=True):
+        if floating:
+            @QtCore.pyqtSlot(float)
+            def update(value: float) -> None:
+                text_field.setText(str(round(value, 2)))
+        else:
+            @QtCore.pyqtSlot(int)
+            def update(value: int) -> None:
+                text_field.setText(str(value))
+
+        return update
+
+    @QtCore.pyqtSlot(hardware.tec.Data)
+    def update_temperature(self, value: hardware.tec.Data) -> None:
+        self.temperature_display.setText(str(value.actual_temperature[self.laser]) + " °C")
+
+    @QtCore.pyqtSlot(model.TecMode)
+    def update_mode(self, mode: model.TecMode):
+        if mode == model.TecMode.COOLING:
+            toggle_button(False, self.buttons["Heat"])
+            toggle_button(True, self.buttons["Cool"])
+        else:
+            toggle_button(True, self.buttons["Heat"])
+            toggle_button(False, self.buttons["Cool"])
+
+    @QtCore.pyqtSlot(bool)
+    def _update_resistor_visibility(self, use_ntc: bool) -> None:
+        self.text_fields.reference_resistor.setDisabled(use_ntc)
+
+    def _init_text_fields(self) -> None:
+        self.frames["PID Configuration"].layout().addWidget(QtWidgets.QLabel("P Value"), 0, 0)
+        self.frames["PID Configuration"].layout().addWidget(self.text_fields.p_value, 0, 1)
+        self.text_fields.p_value.editingFinished.connect(self.p_value_changed)
+
+        self.frames["PID Configuration"].layout().addWidget(QtWidgets.QLabel("I<sub>1</sub> Value"), 2, 0)
+        self.frames["PID Configuration"].layout().addWidget(self.text_fields.i_value[0], 2, 1)
+        self.text_fields.i_value[0].editingFinished.connect(self.i_1_value_changed)
+
+        self.frames["PID Configuration"].layout().addWidget(QtWidgets.QLabel("I<sub>2</sub> Value"), 4, 0)
+        self.frames["PID Configuration"].layout().addWidget(self.text_fields.i_value[1], 4, 1)
+        self.text_fields.i_value[1].editingFinished.connect(self.i_2_value_changed)
+
+        self.frames["PID Configuration"].layout().addWidget(QtWidgets.QLabel("D Value"), 6, 0)
+        self.frames["PID Configuration"].layout().addWidget(self.text_fields.d_value, 6, 1)
+        self.text_fields.d_value.editingFinished.connect(self.d_value_changed)
+
+        self.frames["System Settings"].layout().addWidget(QtWidgets.QLabel("Setpoint Temperature"), 0, 0)
+        self.frames["System Settings"].layout().addWidget(self.text_fields.setpoint_temperature, 0, 1)
+        self.text_fields.setpoint_temperature.editingFinished.connect(self.setpoint_temperature_changed)
+
+        self.frames["System Settings"].layout().addWidget(QtWidgets.QLabel("Loop Time [ms]"), 1, 0)
+        self.frames["System Settings"].layout().addWidget(self.text_fields.loop_time, 1, 1)
+        self.text_fields.loop_time.editingFinished.connect(self.loop_time_changed)
+
+        self.frames["System Settings"].layout().addWidget(QtWidgets.QLabel("Reference Resistor"), 2, 0)
+        self.frames["System Settings"].layout().addWidget(self.text_fields.reference_resistor, 2, 1)
+        self.text_fields.reference_resistor.editingFinished.connect(self.reference_resistor_changed)
+        model.tec_signals[self.laser].use_ntc.connect(self._update_resistor_visibility)
+
+        self.frames["System Settings"].layout().addWidget(QtWidgets.QLabel("Max Power"), 3, 0)
+        self.frames["System Settings"].layout().addWidget(self.text_fields.max_power, 3, 1)
+        self.text_fields.max_power.editingFinished.connect(self.max_power_changed)
+
+        self.frames["Temperature"].layout().addWidget(self.temperature_display)
+
+    def d_value_changed(self) -> None:
+        self.controller.update_d_value(self.text_fields.d_value.text())
+
+    def i_1_value_changed(self) -> None:
+        self.controller.update_i_1_value(self.text_fields.i_value[0].text())
+
+    def i_2_value_changed(self) -> None:
+        self.controller.update_i_2_value(self.text_fields.i_value[1].text())
+
+    def p_value_changed(self) -> None:
+        self.controller.update_p_value(self.text_fields.p_value.text())
+
+    def setpoint_temperature_changed(self) -> None:
+        self.controller.update_setpoint_temperature(self.text_fields.setpoint_temperature.text())
+
+    def loop_time_changed(self) -> None:
+        self.controller.update_loop_time(self.text_fields.loop_time.text())
+
+    def reference_resistor_changed(self) -> None:
+        self.controller.update_reference_resistor(self.text_fields.reference_resistor.text())
+
+    def max_power_changed(self) -> None:
+        self.controller.update_max_power(self.text_fields.max_power.text())
+
+    def _init_buttons(self) -> None:
+        self.create_button(master=self.frames["Temperature"], title="Heat", slot=self.controller.set_heating)
+        self.create_button(master=self.frames["Temperature"], title="Cool", slot=self.controller.set_cooling)
+        config = self.create_configuration_buttons()
+        self.frames["Configuration"].layout().addWidget(config, 3, 0)
+
+
+class _MatplotlibColors:
+    BLUE = "#045993"
+    ORANGE = "#db6000"
+    GREEN = "#118011"
+
+
+class _Plotting(pg.PlotWidget):
+    def __init__(self):
+        pg.PlotWidget.__init__(self)
+        pg.setConfigOption('leftButtonPan', False)
+        pg.setConfigOptions(antialias=True)
+        pg.setConfigOption('background', "white")
+        pg.setConfigOption('foreground', 'k')
+        self.window = pg.GraphicsLayoutWidget()
+        self.plot = self.window.addPlot()
+        self.curves = self.plot.plot(pen=pg.mkPen(_MatplotlibColors.BLUE))
+        self.plot.showGrid(x=True, y=True)
+        self.plot.addLegend()
+
+    @QtCore.pyqtSlot()
+    def clear(self) -> None:
+        self.window.clear()
+
+    @abc.abstractmethod
+    def update_data_live(self, data: model.Buffer) -> None:
+        ...
+
+
+class _DAQPlots(_Plotting):
+    def __init__(self):
+        _Plotting.__init__(self)
+        model.signals.clear_daq.connect(self.clear)
+
+    @abc.abstractmethod
+    def update_data(self, data: pd.DataFrame) -> None:
+        ...
+
+
+class DC(_DAQPlots):
+    def __init__(self):
+        _DAQPlots.__init__(self)
+        self.curves = [self.plot.plot(pen=pg.mkPen(_MatplotlibColors.BLUE), name="DC CH1"),
+                       self.plot.plot(pen=pg.mkPen(_MatplotlibColors.ORANGE), name="DC CH2"),
+                       self.plot.plot(pen=pg.mkPen(_MatplotlibColors.GREEN), name="DC CH3")]
+        self.plot.setLabel(axis="bottom", text="Time [s]")
+        self.plot.setLabel(axis="left", text="Intensity [V]")
+        model.signals.decimation.connect(self.update_data)
+        model.signals.decimation_live.connect(self.update_data_live)
+
+    def update_data(self, data: pd.DataFrame) -> None:
+        for channel in range(3):
+            try:
+                self.curves[channel].setData(data[f"DC CH{channel + 1}"].to_numpy())
+            except KeyError:
+                self.curves[channel].setData(data[f"PD{channel + 1}"].to_numpy())
+
+    def update_data_live(self, data: model.PTIBuffer) -> None:
+        for channel in range(3):
+            self.curves[channel].setData(data.time, data.dc_values[channel])
+
+
+class Amplitudes(_DAQPlots):
+    def __init__(self):
+        _DAQPlots.__init__(self)
+        self.curves = [self.plot.scatterPlot(pen=pg.mkPen(_MatplotlibColors.BLUE),
+                                             brush=pg.mkBrush(_MatplotlibColors.BLUE),
+                                             name="Amplitude CH1"),
+                       self.plot.scatterPlot(pen=pg.mkPen(_MatplotlibColors.ORANGE),
+                                             brush=pg.mkBrush(_MatplotlibColors.ORANGE),
+                                             name="Amplitude CH2"),
+                       self.plot.scatterPlot(pen=pg.mkPen(_MatplotlibColors.GREEN),
+                                             brush=pg.mkBrush(_MatplotlibColors.GREEN),
+                                             name="Amplitude CH3")]
+        self.plot.setLabel(axis="bottom", text="Time [s]")
+        self.plot.setLabel(axis="left", text="Amplitude [V]")
+        model.signals.characterization.connect(self.update_data)
+        model.signals.characterization_live.connect(self.update_data_live)
+
+    def update_data(self, data: pd.DataFrame) -> None:
+        for channel in range(3):
+            self.curves[channel].setData(data.index, data[f"Amplitude CH{channel + 1}"].to_numpy())
+
+    def update_data_live(self, data: model.CharacterisationBuffer) -> None:
+        for channel in range(3):
+            self.curves[channel].setData(data.time, data.amplitudes[channel])
+
+
+class OutputPhases(_DAQPlots):
+    def __init__(self):
+        _DAQPlots.__init__(self)
+        self.curves = [self.plot.scatterPlot(pen=pg.mkPen(_MatplotlibColors.ORANGE), name="Output Phase CH2",
+                                             brush=pg.mkBrush(_MatplotlibColors.ORANGE)),
+                       self.plot.scatterPlot(pen=pg.mkPen(_MatplotlibColors.GREEN), name="Output Phase CH3",
+                                             brush=pg.mkBrush(_MatplotlibColors.GREEN))]
+        self.plot.setLabel(axis="bottom", text="Time [s]")
+        self.plot.setLabel(axis="left", text="Output Phase [deg]")
+        model.signals.characterization.connect(self.update_data)
+        model.signals.characterization_live.connect(self.update_data_live)
+
+    def update_data(self, data: pd.DataFrame) -> None:
+        for channel in range(2):
+            self.curves[channel].setData(data.index, data[f"Output Phase CH{channel + 2}"].to_numpy())
+
+    def update_data_live(self, data: model.CharacterisationBuffer) -> None:
+        for channel in range(2):
+            self.curves[channel].setData(data.time, data.output_phases[channel])
+
+
+class InterferometricPhase(_DAQPlots):
+    def __init__(self):
+        _DAQPlots.__init__(self)
+        self.curves = self.plot.plot(pen=pg.mkPen(_MatplotlibColors.BLUE))
+        self.plot.setLabel(axis="bottom", text="Time [s]")
+        self.plot.setLabel(axis="left", text="Interferometric Phase [rad]")
+        model.signals.inversion.connect(self.update_data)
+        model.signals.inversion_live.connect(self.update_data_live)
+
+    def update_data(self, data: pd.DataFrame) -> None:
+        self.curves.setData(data["Interferometric Phase"].to_numpy())
+
+    def update_data_live(self, data: model.PTIBuffer) -> None:
+        self.curves.setData(data.time, data.interferometric_phase)
+
+
+class Sensitivity(_DAQPlots):
+    def __init__(self):
+        _DAQPlots.__init__(self)
+        self.curves = [self.plot.plot(pen=pg.mkPen(_MatplotlibColors.BLUE), name="CH1"),
+                       self.plot.plot(pen=pg.mkPen(_MatplotlibColors.ORANGE), name="CH2"),
+                       self.plot.plot(pen=pg.mkPen(_MatplotlibColors.GREEN), name="CH3")]
+        self.plot.setLabel(axis="bottom", text="Time [s]")
+        self.plot.setLabel(axis="left", text="Sensitivity [V/rad]")
+        model.signals.inversion.connect(self.update_data)
+        model.signals.inversion_live.connect(self.update_data_live)
+
+    def update_data(self, data: pd.DataFrame) -> None:
+        for channel in range(3):
+            self.curves[channel].setData(data[f"Sensitivity CH{channel + 1}"].to_numpy())
+
+    def update_data_live(self, data: model.PTIBuffer) -> None:
+        for channel in range(3):
+            self.curves[channel].setData(data.time, data.sensitivity[channel])
+
+
+class Symmetry(_DAQPlots):
+    def __init__(self):
+        _DAQPlots.__init__(self)
+        self.curves = [self.plot.scatterPlot(pen=pg.mkPen(_MatplotlibColors.BLUE), name="Absolute Symmetry",
+                                             brush=pg.mkBrush(_MatplotlibColors.BLUE)),
+                       self.plot.scatterPlot(pen=pg.mkPen(_MatplotlibColors.ORANGE), name="Relative Symmetry",
+                                             brush=pg.mkBrush(_MatplotlibColors.ORANGE))]
+        self.plot.setLabel(axis="bottom", text="Time [s]")
+        self.plot.setLabel(axis="left", text="Symmetry [%]")
+        model.signals.characterization.connect(self.update_data)
+        model.signals.characterization_live.connect(self.update_data_live)
+
+    def update_data(self, data: pd.DataFrame) -> None:
+        self.curves[0].setData(data.index, data["Symmetry"].to_numpy())
+        self.curves[1].setData(data.index, data["Relative Symmetry"].to_numpy())
+
+    def update_data_live(self, data: model.CharacterisationBuffer) -> None:
+        self.curves[0].setData(data.time, data.symmetry)
+        self.curves[1].setData(data.time, data.relative_symmetry)
+
+
+class PTISignal(_DAQPlots):
+    def __init__(self):
+        _DAQPlots.__init__(self)
+        self.curves = {"PTI Signal": self.plot.scatterPlot(pen=pg.mkPen(_MatplotlibColors.BLUE), name="1 s", size=6),
+                       "PTI Signal Mean": self.plot.plot(pen=pg.mkPen(_MatplotlibColors.ORANGE), name="60 s Mean")}
+        self.plot.setLabel(axis="bottom", text="Time [s]")
+        self.plot.setLabel(axis="left", text="PTI Signal [µrad]")
+        model.signals.inversion.connect(self.update_data)
+        model.signals.inversion_live.connect(self.update_data_live)
+
+    def update_data(self, data: pd.DataFrame) -> None:
+        try:
+            self.curves["PTI Signal"].setData(data["PTI Signal"].to_numpy())
+            self.curves["PTI Signal Mean"].setData(data["PTI Signal 60 s Mean"].to_numpy())
+        except KeyError:
+            pass
+
+    def update_data_live(self, data: model.PTIBuffer) -> None:
+        self.curves["PTI Signal"].setData(data.time, data.pti_signal)
+        self.curves["PTI Signal Mean"].setData(data.time, data.pti_signal_mean)
+
+
+class PumpLaserCurrent(_Plotting):
+    def __init__(self):
+        _Plotting.__init__(self)
+        self.curves = self.plot.plot(pen=pg.mkPen(_MatplotlibColors.BLUE))
+        self.plot.setLabel(axis="bottom", text="Time [s]")
+        self.plot.setLabel(axis="left", text="Current [mA]")
+        model.laser_signals.data.connect(self.update_data_live)
+        model.laser_signals.clear_pumplaser.connect(self.clear)
+
+    def update_data_live(self, data: model.LaserBuffer) -> None:
+        self.curves.setData(data.time, data.pump_laser_current)
+
+
+class ProbeLaserCurrent(_Plotting):
+    def __init__(self):
+        _Plotting.__init__(self)
+        self.curves = self.plot.plot(pen=pg.mkPen(_MatplotlibColors.BLUE))
+        self.plot.setLabel(axis="bottom", text="Time [s]")
+        self.plot.setLabel(axis="left", text="Current [mA]")
+        model.laser_signals.data.connect(self.update_data_live)
+        model.laser_signals.clear_probelaser.connect(self.clear)
+
+    def update_data_live(self, data: model.LaserBuffer) -> None:
+        self.curves.setData(data.time, data.probe_laser_current)
+
+
+class TecTemperature(_Plotting):
+    SET_POINT = 0
+    MEASURAED = 1
+
+    def __init__(self, channel: int):
+        _Plotting.__init__(self)
+        self.curves = [self.plot.plot(pen=pg.mkPen(_MatplotlibColors.BLUE), name="Setpoint Temperature"),
+                       self.plot.plot(pen=pg.mkPen(_MatplotlibColors.ORANGE), name="Measured Temperature")]
+        self.plot.setLabel(axis="bottom", text="Time [s]")
+        self.plot.setLabel(axis="left", text="Temperature [°C]")
+        self.laser = channel
+        model.tec_signals[channel].clear_plots.connect(self.clear)
+        model.signals.tec_data.connect(self.update_data_live)
+
+    def update_data_live(self, data: model.TecBuffer) -> None:
+        self.curves[TecTemperature.SET_POINT].setData(data.time, data.set_point[self.laser])
+        self.curves[TecTemperature.MEASURAED].setData(data.time, data.actual_value[self.laser])
```

### Comparing `minipti-1.9.1/src/minipti/hardware/motherboard.py` & `minipti-1.9.3/src/hardware/motherboard.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,382 +1,399 @@
-import enum
-import itertools
-import logging
-import os
-import queue
-import threading
-import time
-from collections import deque
-from configparser import ConfigParser
-from dataclasses import dataclass, asdict
-from typing import Sequence, Union
-
-from fastcrc import crc16
-
-from . import serial_device
-
-
-@dataclass
-class DAQData:
-    ref_signal: Union[queue.Queue, deque, Sequence]
-    ac_coupled: Union[queue.Queue, deque, Sequence]
-    dc_coupled: Union[queue.Queue, deque, Sequence]
-
-
-_Samples = deque[int]
-
-
-class BMS(enum.IntEnum):
-    SHUTDOWN = 0xFF
-    SHUTDOWN_INDEX = 2
-    VALID_IDENTIFIER_INDEX = 4
-    EXTERNAL_DC_POWER_INDEX = 6
-    CHARGING_INDEX = 8
-    MINUTES_LEFT_INDEX = 10
-    BATTERY_PERCENTAGE_INDEX = 14
-    BATTERY_TEMPERATURE_INDEX = 16
-    CURRENT_INDEX = 20
-    VOLTAGE_INDEX = 24
-    FULL_CHARGED_CAPACITY_INDEX = 28
-    REMAINING_CAPACITY_INDEX = 32
-
-
-@dataclass
-class BMSData:
-    external_dc_power: bool
-    charging: bool
-    minutes_left: int
-    battery_percentage: int
-    battery_temperature: float  # °C
-    battery_current: int  # mA
-    battery_voltage: int  # mV
-    full_charged_capacity: int  # mAh
-    remaining_capacity: int  # mAh
-
-
-@dataclass
-class PackageData:
-    DAQ: DAQData
-    BMS: queue.Queue
-
-
-@dataclass
-class Valve:
-    automatic_switch: bool
-    period: int
-    duty_cycle: int
-
-
-@dataclass
-class DAQ:
-    number_of_samples: int
-    ref_period: int
-
-
-@dataclass
-class MotherBoardConfig:
-    valve: Valve
-    daq: DAQ
-
-
-class Driver(serial_device.Driver):
-    """
-    This class provides an interface for receiving data from the serial port of a USB connected DAQ
-    system. The data is accordingly to a defined protocol encoded and build into a packages of
-    samples.
-    """
-    _PACKAGE_SIZE_START_INDEX = 2
-    _PACKAGE_SIZE_END_INDEX = 10
-    _CRC_START_INDEX = 4
-    _PACKAGE_SIZE = 4110
-    _WORD_SIZE = 32
-
-    HARDWARE_ID = b"0001"
-    NAME = "Motherboard"
-
-    _CHANNELS = 3
-
-    def __init__(self):
-        serial_device.Driver.__init__(self)
-        self.connected = threading.Event()
-        self._package_data = PackageData(DAQData(queue.Queue(maxsize=Driver._QUEUE_SIZE),
-                                                 queue.Queue(maxsize=Driver._QUEUE_SIZE),
-                                                 queue.Queue(maxsize=Driver._QUEUE_SIZE)),
-                                         queue.Queue(maxsize=Driver._QUEUE_SIZE))
-        self._buffer = ""
-        self._encoded_buffer = DAQData(deque(), [deque(), deque(), deque()],
-                                       [deque(), deque(), deque()])
-        self._sample_numbers = deque(maxlen=2)
-        self.synchronize = False
-        self.config: Union[MotherBoardConfig, None] = None
-        self.shutdown = threading.Event()
-        self.config_path = f"{os.path.dirname(__file__)}/configs/motherboard.ini"
-        self.config_parser = ConfigParser()
-        self.automatic_switch = threading.Event()
-        self.bypass = False
-        self.load_config()
-
-    @property
-    def device_id(self) -> bytes:
-        return Driver.HARDWARE_ID
-
-    @property
-    def device_name(self) -> str:
-        return Driver.NAME
-
-    @property
-    def bms(self) -> BMSData:
-        return self._package_data.BMS.get(block=True)
-
-    @property
-    def ref_signal(self) -> deque:
-        return self._package_data.DAQ.ref_signal.get(block=True)
-
-    @property
-    def dc_coupled(self) -> deque:
-        return self._package_data.DAQ.dc_coupled.get(block=True)
-
-    @property
-    def ac_coupled(self) -> deque:
-        return self._package_data.DAQ.ac_coupled.get(block=True)
-
-    @property
-    def buffer_size(self) -> int:
-        return len(self._buffer)
-
-    @property
-    def encoded_buffer_ref_size(self) -> int:
-        return len(self._encoded_buffer.ref_signal)
-
-    @property
-    def encoded_buffer_ac_size(self) -> int:
-        return len(self._encoded_buffer.ac_coupled[0])
-
-    @property
-    def encoded_buffer_dc_size(self) -> int:
-        return len(self._encoded_buffer.dc_coupled[0])
-
-    @property
-    def bms_package_empty(self) -> bool:
-        return self._package_data.BMS.empty()
-
-    @property
-    def saved_sample_numbers(self) -> int:
-        return len(self._sample_numbers)
-
-    def clear_buffer(self) -> None:
-        self._buffer = ""
-
-    @staticmethod
-    def _binary_to_2_complement(number: int, byte_length: int) -> int:
-        if number & (1 << (byte_length - 1)):
-            return number - (1 << byte_length)
-        return number
-
-    def load_config(self) -> None:
-        self.config_parser.read(self.config_path)
-        valve_config = Valve(automatic_switch=self.config_parser.getboolean("Valve", "automatic_switch"),
-                             period=self.config_parser.getint("Valve", "period"),
-                             duty_cycle=self.config_parser.getint("Valve", "duty_cycle"))
-        daq_config = DAQ(number_of_samples=self.config_parser.getint("DAQ", "number_of_samples"),
-                         ref_period=self.config_parser.getint("DAQ", "ref_period"))
-        self.config = MotherBoardConfig(valve_config, daq_config)
-        if valve_config.automatic_switch:
-            self.automatic_switch.set()
-
-    def save_config(self) -> None:
-        self.config_parser["Valve"] = asdict(self.config.valve)
-        with open(self.config_path, "w") as savefile:
-            self.config_parser.write(savefile)
-
-    @staticmethod
-    def _encode(raw_data: Sequence) -> tuple[_Samples, list[_Samples], list[_Samples]]:
-        """
-        A block of data has the following structure:
-        Ref, DC 1, DC 2, DC 3, DC, 4 AC 1, AC 2, AC 3, AC 4
-        These byte words are 4 bytes wide and hex decimal decoded. These big byte word of size 32
-        repeats periodically. It starts with below the first 10 bytes (meta information) and ends
-        before the last 4 bytes (crc checksum).
-        """
-        raw_data = raw_data[Driver._PACKAGE_SIZE_END_INDEX:Driver._PACKAGE_SIZE - Driver._CRC_START_INDEX]
-        ref: _Samples = deque()
-        ac: list[_Samples] = [deque(), deque(), deque()]
-        dc: list[_Samples] = [deque(), deque(), deque(), deque()]
-        for i in range(0, len(raw_data), Driver._WORD_SIZE):
-            ref.append(int(raw_data[i:i + 4], base=16))
-            # AC signed
-            ac_value = Driver._binary_to_2_complement(int(raw_data[i + 4:i + 8], base=16), 16)
-            ac[0].append(ac_value)
-            ac_value = Driver._binary_to_2_complement(int(raw_data[i + 8:i + 12], base=16), 16)
-            ac[1].append(ac_value)
-            ac_value = Driver._binary_to_2_complement(int(raw_data[i + 12:i + 16], base=16), 16)
-            ac[2].append(ac_value)
-            # DC unsigned
-            dc[0].append(int(raw_data[i + 16:i + 20], base=16))
-            dc[1].append(int(raw_data[i + 20:i + 24], base=16))
-            dc[2].append(int(raw_data[i + 24:i + 28], base=16))
-            dc[3].append(int(raw_data[i + 28:i + 32], base=16))
-        return ref, ac, dc
-
-    def reset(self) -> None:
-        self._reset()
-        self.clear_buffer()
-
-    def _reset(self) -> None:
-        self.synchronize = True
-        self._encoded_buffer.ref_signal = deque()
-        self._encoded_buffer.dc_coupled = [deque(), deque(), deque()]
-        self._encoded_buffer.ac_coupled = [deque(), deque(), deque()]
-        self._sample_numbers = deque(maxlen=2)
-
-    def encode_data(self) -> None:
-        split_data = (self._buffer + self.received_data.get(block=True)).split("\n")
-        for i in range(len(split_data) - 1):
-            data = split_data[i]
-            if not data:
-                continue
-            if data[:2] == "00" and len(data) == 4110:
-                self._encode_daq(data)
-            elif data[:2] == "01" and len(data) == 40:
-                self._encode_bms(data)
-            elif data[0] == "S" and len(data) == 7:
-                self._check_ack(data)
-        # Remaining data without a termination symbol must be buffered
-        self._buffer = split_data[-1]
-
-    def _encode_daq(self, data: str) -> None:
-        """
-        The data is encoded according to the following protocol:
-            - The first two bytes describes the send command
-            - Byte 2 up to 10 describe the package number of the send package
-            - Byte 10 to 32 contain the data as period sequence of blocks in hex decimal
-            - The last 4 bytes represent a CRC checksum in hex decimal
-        """
-        if not Driver._crc_check(data, "DAQ"):
-            self._reset()  # The data is not trustful, and it should be waited for new
-            return
-        self._sample_numbers.append(data[Driver._PACKAGE_SIZE_START_INDEX:Driver._PACKAGE_SIZE_END_INDEX])
-        if len(self._sample_numbers) > 1 and not self._check_package_difference():
-            self._reset()
-        ref_signal, ac_coupled, dc_coupled = Driver._encode(data)
-        if self.synchronize:
-            self._synchronize_with_ref(ref_signal, ac_coupled, dc_coupled)
-        self._encoded_buffer.ref_signal.extend(ref_signal)
-        for channel in range(Driver._CHANNELS):
-            self._encoded_buffer.dc_coupled[channel].extend(dc_coupled[channel])
-            self._encoded_buffer.ac_coupled[channel].extend(ac_coupled[channel])
-
-    def _encode_bms(self, data: str) -> None:
-        """
-        The BMS data is encoded according to the following scheme:
-        Every byte is an ASCII symbol. The bytes have the following meanings:
-        1 - 2:
-            Represent the package identifier
-        2 - 4:
-        - The next two bytes are the countdown of a shutdown. Attention: if this value is below 255 (0xFF),
-          the motherboard will shut down itself soon.
-        - The next
-        """
-        if not Driver._crc_check(data, "BMS"):
-            return
-        if int(data[BMS.SHUTDOWN_INDEX:BMS.SHUTDOWN_INDEX + 2], base=16) < BMS.SHUTDOWN:
-            self.shutdown.set()
-        if not int(data[BMS.VALID_IDENTIFIER_INDEX: BMS.VALID_IDENTIFIER_INDEX + 2], base=16):
-            logging.error("Invalid package from BMS")
-            return
-        bms = BMSData(
-            external_dc_power=bool(int(data[BMS.EXTERNAL_DC_POWER_INDEX:BMS.EXTERNAL_DC_POWER_INDEX + 2], base=16)),
-            charging=bool(int(data[BMS.CHARGING_INDEX:BMS.CHARGING_INDEX + 2], base=16)),
-            minutes_left=int(data[BMS.MINUTES_LEFT_INDEX:BMS.MINUTES_LEFT_INDEX + 4], base=16),
-            battery_percentage=int(data[BMS.BATTERY_PERCENTAGE_INDEX:BMS.BATTERY_PERCENTAGE_INDEX + 2], base=16),
-            battery_temperature=int(data[BMS.BATTERY_TEMPERATURE_INDEX:BMS.BATTERY_TEMPERATURE_INDEX + 4], base=16),
-            battery_current=Driver._binary_to_2_complement(int(data[BMS.CURRENT_INDEX:BMS.CURRENT_INDEX + 4], base=16),
-                                                           byte_length=16),
-            battery_voltage=int(data[BMS.VOLTAGE_INDEX: BMS.VOLTAGE_INDEX + 4], base=16),
-            full_charged_capacity=int(data[BMS.FULL_CHARGED_CAPACITY_INDEX:BMS.FULL_CHARGED_CAPACITY_INDEX + 4],
-                                      base=16),
-            remaining_capacity=int(data[BMS.REMAINING_CAPACITY_INDEX:BMS.REMAINING_CAPACITY_INDEX + 4], base=16)
-        )
-        self._package_data.BMS.put(bms)
-
-    @staticmethod
-    def _crc_check(data: str, source) -> bool:
-        crc_calculated = crc16.arc(data[:-Driver._CRC_START_INDEX].encode())
-        crc_received = int(data[-Driver._CRC_START_INDEX:], base=16)
-        if crc_calculated != crc_received:  # Corrupted data
-            logging.error(f"CRC value of {source} isn't equal to transmitted. Got {crc_received:04X} "
-                          f"instead of {crc_calculated:04X}.")
-            return False
-        return True
-
-    def _check_package_difference(self) -> bool:
-        package_difference = int(self._sample_numbers[1], base=16) - int(self._sample_numbers[0],  base=16)
-        if package_difference != 1:
-            logging.error(f"Missing {package_difference} packages.")
-            return False
-        return True
-
-    def _synchronize_with_ref(self, ref_signal: _Samples, ac_coupled: list[_Samples],
-                              dc_coupled: list[_Samples]) -> None:
-        while sum(itertools.islice(ref_signal, 0, self.config.daq.ref_period // 2)):
-            ref_signal.popleft()
-            for channel in range(Driver._CHANNELS):
-                ac_coupled[channel].popleft()
-                dc_coupled[channel].popleft()
-            dc_coupled[3].popleft()
-        if len(ref_signal) < self.config.daq.ref_period // 2:
-            return
-        self.synchronize = False
-
-    def build_sample_package(self) -> None:
-        """
-        Creates a package of samples that represents approximately 1 s data. It contains 8000
-        samples.
-        """
-        self._package_data.DAQ.ref_signal.put([self._encoded_buffer.ref_signal.popleft()
-                                               for _ in range(self.config.daq.number_of_samples)])
-        dc_package = [[], [], []]
-        ac_package = [[], [], []]
-        for _ in itertools.repeat(None, self.config.daq.number_of_samples):
-            for channel in range(Driver._CHANNELS):
-                dc_package[channel].append(self._encoded_buffer.dc_coupled[channel].popleft())
-                ac_package[channel].append(self._encoded_buffer.ac_coupled[channel].popleft())
-        self._package_data.DAQ.dc_coupled.put(dc_package)
-        self._package_data.DAQ.ac_coupled.put(ac_package)
-
-    def set_valve(self) -> None:
-        if self.bypass:
-            self.write("SBP0000")
-            self.bypass = False
-        else:
-            self.write("SBP0001")
-            self.bypass = True
-
-    def _process_data(self) -> None:
-        self._reset()
-        self._package_data = PackageData(DAQData(queue.Queue(maxsize=Driver._QUEUE_SIZE),
-                                                 queue.Queue(maxsize=Driver._QUEUE_SIZE),
-                                                 queue.Queue(maxsize=Driver._QUEUE_SIZE)),
-                                         queue.Queue(maxsize=Driver._QUEUE_SIZE))
-        self._buffer = ""
-        self._encoded_buffer = DAQData(deque(), [deque(), deque(), deque()], [deque(), deque(), deque()])
-        self._sample_numbers = deque(maxlen=2)
-        while self.connected.is_set():
-            self.encode_data()
-            if len(self._encoded_buffer.ref_signal) >= self.config.daq.number_of_samples:
-                self.build_sample_package()
-
-    def automatic_valve_change(self) -> None:
-        """
-        Periodically bypass a valve. The duty cycle defines how much time for each part (bypassed
-        or not) is spent.
-        """
-        def switch() -> None:
-            while self.connected and self.automatic_switch.set():
-                if self.bypass:
-                    self.set_valve()
-                    time.sleep(self.config.valve.period * self.config.valve.duty_cycle / 100)
-                else:
-                    self.set_valve()
-                    time.sleep(self.config.valve.period * (1 - self.config.valve.duty_cycle / 100))
-
-        threading.Thread(target=switch, daemon=True).start()
+import enum
+import itertools
+import logging
+import os
+import queue
+import threading
+import time
+from collections import deque
+from configparser import ConfigParser
+from dataclasses import dataclass, asdict
+from typing import Sequence, Union
+
+from fastcrc import crc16
+
+from . import serial_device
+
+
+@dataclass
+class DAQData:
+    ref_signal: Union[queue.Queue, deque, Sequence]
+    ac_coupled: Union[queue.Queue, deque, Sequence]
+    dc_coupled: Union[queue.Queue, deque, Sequence]
+
+
+_Samples = deque[int]
+
+
+class BMS(enum.IntEnum):
+    SHUTDOWN = 0xFF
+    SHUTDOWN_INDEX = 1
+    VALID_IDENTIFIER_INDEX = 3
+    EXTERNAL_DC_POWER_INDEX = 5
+    CHARGING_INDEX = 7
+    MINUTES_LEFT_INDEX = 9
+    BATTERY_PERCENTAGE_INDEX = 13
+    BATTERY_TEMPERATURE_INDEX = 15
+    CURRENT_INDEX = 19
+    VOLTAGE_INDEX = 23
+    FULL_CHARGED_CAPACITY_INDEX = 27
+    REMAINING_CAPACITY_INDEX = 31
+
+
+@dataclass
+class BMSData:
+    external_dc_power: bool
+    charging: bool
+    minutes_left: Union[int, float]
+    battery_percentage: int
+    battery_temperature: float  # °C
+    battery_current: int  # mA
+    battery_voltage: int  # mV
+    full_charged_capacity: int  # mAh
+    remaining_capacity: int  # mAh
+
+
+@dataclass
+class PackageData:
+    DAQ: DAQData
+    BMS: queue.Queue
+
+
+@dataclass
+class Valve:
+    automatic_switch: bool
+    period: int
+    duty_cycle: int
+
+
+@dataclass
+class DAQ:
+    number_of_samples: int
+    ref_period: int
+
+
+@dataclass
+class MotherBoardConfig:
+    valve: Valve
+    daq: DAQ
+
+
+class Driver(serial_device.Driver):
+    """
+    This class provides an interface for receiving data from the serial port of a USB connected DAQ
+    system. The data is accordingly to a defined protocol encoded and build into a packages of
+    samples.
+    """
+    _PACKAGE_SIZE_START_INDEX = 1
+    _PACKAGE_SIZE_END_INDEX = 9
+    _CRC_START_INDEX = 4
+    _DAQ_PACKAGE_SIZE = 4109
+    _BMS_PACKAGE_SIZE = 39
+    _WORD_SIZE = 32
+
+    HARDWARE_ID = b"0001"
+    NAME = "Motherboard"
+
+    _CHANNELS = 3
+
+    def __init__(self):
+        serial_device.Driver.__init__(self)
+        self.connected = threading.Event()
+        self.data = PackageData(DAQData(queue.Queue(maxsize=Driver._QUEUE_SIZE),
+                                        queue.Queue(maxsize=Driver._QUEUE_SIZE),
+                                        queue.Queue(maxsize=Driver._QUEUE_SIZE)),
+                                queue.Queue(maxsize=Driver._QUEUE_SIZE))
+        self._buffer = ""
+        self._encoded_buffer = DAQData(deque(), [deque(), deque(), deque()],
+                                       [deque(), deque(), deque()])
+        self._sample_numbers = deque(maxlen=2)
+        self.synchronize = False
+        self.config: Union[MotherBoardConfig, None] = None
+        self.shutdown = threading.Event()
+        self.config_path = f"{os.path.dirname(__file__)}/configs/motherboard.ini"
+        self.config_parser = ConfigParser()
+        self.automatic_switch = threading.Event()
+        self.bypass = False
+        self.running = threading.Event()
+        self.running.clear()
+        self.load_config()
+
+    @property
+    def device_id(self) -> bytes:
+        return Driver.HARDWARE_ID
+
+    @property
+    def device_name(self) -> str:
+        return Driver.NAME
+
+    @property
+    def bms(self) -> BMSData:
+        return self.data.BMS.get(block=True)
+
+    @property
+    def ref_signal(self) -> deque:
+        return self.data.DAQ.ref_signal.get(block=True)
+
+    @property
+    def dc_coupled(self) -> deque:
+        return self.data.DAQ.dc_coupled.get(block=True)
+
+    @property
+    def ac_coupled(self) -> deque:
+        return self.data.DAQ.ac_coupled.get(block=True)
+
+    @property
+    def buffer_size(self) -> int:
+        return len(self._buffer)
+
+    @property
+    def encoded_buffer_ref_size(self) -> int:
+        return len(self._encoded_buffer.ref_signal)
+
+    @property
+    def encoded_buffer_ac_size(self) -> int:
+        return len(self._encoded_buffer.ac_coupled[0])
+
+    @property
+    def encoded_buffer_dc_size(self) -> int:
+        return len(self._encoded_buffer.dc_coupled[0])
+
+    @property
+    def bms_package_empty(self) -> bool:
+        return self.data.BMS.empty()
+
+    @property
+    def saved_sample_numbers(self) -> int:
+        return len(self._sample_numbers)
+
+    def clear_buffer(self) -> None:
+        self._buffer = ""
+        self.data.DAQ = DAQData(queue.Queue(maxsize=Driver._QUEUE_SIZE),
+                                queue.Queue(maxsize=Driver._QUEUE_SIZE),
+                                queue.Queue(maxsize=Driver._QUEUE_SIZE))
+
+    @staticmethod
+    def _binary_to_2_complement(number: int, byte_length: int) -> int:
+        if number & (1 << (byte_length - 1)):
+            return number - (1 << byte_length)
+        return number
+
+    def load_config(self) -> None:
+        self.config_parser.read(self.config_path)
+        valve_config = Valve(automatic_switch=self.config_parser.getboolean("Valve", "automatic_switch"),
+                             period=self.config_parser.getint("Valve", "period"),
+                             duty_cycle=self.config_parser.getint("Valve", "duty_cycle"))
+        daq_config = DAQ(number_of_samples=self.config_parser.getint("DAQ", "number_of_samples"),
+                         ref_period=self.config_parser.getint("DAQ", "ref_period"))
+        self.config = MotherBoardConfig(valve_config, daq_config)
+        if valve_config.automatic_switch:
+            self.automatic_switch.set()
+
+    def save_config(self) -> None:
+        self.config_parser["Valve"] = asdict(self.config.valve)
+        with open(self.config_path, "w") as savefile:
+            self.config_parser.write(savefile)
+
+    @staticmethod
+    def _encode(raw_data: Sequence) -> tuple[_Samples, list[_Samples], list[_Samples]]:
+        """
+        A block of data has the following structure:
+        Ref, DC 1, DC 2, DC 3, DC, 4 AC 1, AC 2, AC 3, AC 4
+        These byte words are 4 bytes wide and hex decimal decoded. These big byte word of size 32
+        repeats periodically. It starts with below the first 10 bytes (meta information) and ends
+        before the last 4 bytes (crc checksum).
+        """
+        raw_data = raw_data[Driver._PACKAGE_SIZE_END_INDEX:Driver._DAQ_PACKAGE_SIZE - Driver._CRC_START_INDEX]
+        ref: _Samples = deque()
+        ac: list[_Samples] = [deque(), deque(), deque()]
+        dc: list[_Samples] = [deque(), deque(), deque(), deque()]
+        for i in range(0, len(raw_data), Driver._WORD_SIZE):
+            ref.append(int(raw_data[i:i + 4], base=16))
+            # AC signed
+            ac_value = Driver._binary_to_2_complement(int(raw_data[i + 4:i + 8], base=16), 16)
+            ac[0].append(ac_value)
+            ac_value = Driver._binary_to_2_complement(int(raw_data[i + 8:i + 12], base=16), 16)
+            ac[1].append(ac_value)
+            ac_value = Driver._binary_to_2_complement(int(raw_data[i + 12:i + 16], base=16), 16)
+            ac[2].append(ac_value)
+            # DC unsigned
+            dc[0].append(int(raw_data[i + 16:i + 20], base=16))
+            dc[1].append(int(raw_data[i + 20:i + 24], base=16))
+            dc[2].append(int(raw_data[i + 24:i + 28], base=16))
+            dc[3].append(int(raw_data[i + 28:i + 32], base=16))
+        return ref, ac, dc
+
+    def reset(self) -> None:
+        self._reset()
+        self.clear_buffer()
+
+    def _reset(self) -> None:
+        self.synchronize = True
+        self._encoded_buffer.ref_signal = deque()
+        self._encoded_buffer.dc_coupled = [deque(), deque(), deque()]
+        self._encoded_buffer.ac_coupled = [deque(), deque(), deque()]
+        self._sample_numbers = deque(maxlen=2)
+
+    def _encode_data(self) -> None:
+        try:
+            received_data = self._buffer + self.get_data()
+        except OSError:
+            return
+        split_data = received_data.split("\n")
+        for i in range(len(split_data) - 1):
+            data = split_data[i]
+            if data[0] == "D" and len(data) == Driver._DAQ_PACKAGE_SIZE:
+                self._encode_daq(data)
+            elif data[0] == "B" and len(data) == Driver._BMS_PACKAGE_SIZE:
+                self._encode_bms(data)
+            elif data[0] == "S" and len(data) == 7:
+                self._check_ack(data)
+        # Remaining data without a termination symbol must be buffered
+        self._buffer = split_data[-1]
+
+    def _encode_daq(self, data: str) -> None:
+        """
+        The data is encoded according to the following protocol:
+            - The first two bytes describes the send command
+            - Byte 2 up to 10 describe the package number of the send package
+            - Byte 10 to 32 contain the data as period sequence of blocks in hex decimal
+            - The last 4 bytes represent a CRC checksum in hex decimal
+        """
+        if not Driver._crc_check(data, "DAQ"):
+            self._reset()  # The data is not trustful, and it should be waited for new
+            return
+        self._sample_numbers.append(data[Driver._PACKAGE_SIZE_START_INDEX:Driver._PACKAGE_SIZE_END_INDEX])
+        if len(self._sample_numbers) > 1 and not self._check_package_difference():
+            self._reset()
+        ref_signal, ac_coupled, dc_coupled = Driver._encode(data)
+        if self.synchronize:
+            self._synchronize_with_ref(ref_signal, ac_coupled, dc_coupled)
+        self._encoded_buffer.ref_signal.extend(ref_signal)
+        for channel in range(Driver._CHANNELS):
+            self._encoded_buffer.dc_coupled[channel].extend(dc_coupled[channel])
+            self._encoded_buffer.ac_coupled[channel].extend(ac_coupled[channel])
+
+    def _encode_bms(self, data: str) -> None:
+        """
+        The BMS data is encoded according to the following scheme:
+        Every byte is an ASCII symbol. The bytes have the following meanings:
+        1 - 2:
+            Represent the package identifier
+        2 - 4:
+        - The next two bytes are the countdown of a shutdown. Attention: if this value is below 255 (0xFF),
+          the motherboard will shut down itself soon.
+        - The next
+        """
+        if not Driver._crc_check(data, "BMS"):
+            return
+        if int(data[BMS.SHUTDOWN_INDEX:BMS.SHUTDOWN_INDEX + 2], base=16) < BMS.SHUTDOWN:
+            self.shutdown.set()
+        if not int(data[BMS.VALID_IDENTIFIER_INDEX:BMS.VALID_IDENTIFIER_INDEX + 2], base=16):
+            logging.error("Invalid package from BMS")
+            return
+        bms = BMSData(
+            external_dc_power=bool(int(data[BMS.EXTERNAL_DC_POWER_INDEX:BMS.EXTERNAL_DC_POWER_INDEX + 2], base=16)),
+            charging=bool(int(data[BMS.CHARGING_INDEX:BMS.CHARGING_INDEX + 2], base=16)),
+            minutes_left=int(data[BMS.MINUTES_LEFT_INDEX:BMS.MINUTES_LEFT_INDEX + 4], base=16),
+            battery_percentage=int(data[BMS.BATTERY_PERCENTAGE_INDEX:BMS.BATTERY_PERCENTAGE_INDEX + 2], base=16),
+            battery_temperature=int(data[BMS.BATTERY_TEMPERATURE_INDEX:BMS.BATTERY_TEMPERATURE_INDEX + 4], base=16),
+            battery_current=Driver._binary_to_2_complement(int(data[BMS.CURRENT_INDEX:BMS.CURRENT_INDEX + 4], base=16),
+                                                           byte_length=16),
+            battery_voltage=int(data[BMS.VOLTAGE_INDEX: BMS.VOLTAGE_INDEX + 4], base=16),
+            full_charged_capacity=int(data[BMS.FULL_CHARGED_CAPACITY_INDEX:BMS.FULL_CHARGED_CAPACITY_INDEX + 4],
+                                      base=16),
+            remaining_capacity=int(data[BMS.REMAINING_CAPACITY_INDEX:BMS.REMAINING_CAPACITY_INDEX + 4], base=16))
+        if bms.charging:
+            bms.minutes_left = float("inf")
+        self.data.BMS.put(bms)
+
+    @staticmethod
+    def _crc_check(data: str, source) -> bool:
+        crc_calculated = crc16.arc(data[:-Driver._CRC_START_INDEX].encode())
+        crc_received = int(data[-Driver._CRC_START_INDEX:], base=16)
+        if crc_calculated != crc_received:  # Corrupted data
+            logging.error(f"CRC value of {source} isn't equal to transmitted. Got {crc_received:04X} "
+                          f"instead of {crc_calculated:04X}.")
+            return False
+        return True
+
+    def _check_package_difference(self) -> bool:
+        package_difference = int(self._sample_numbers[1], base=16) - int(self._sample_numbers[0],  base=16)
+        if package_difference != 1:
+            logging.error(f"Missing {package_difference} packages.")
+            return False
+        return True
+
+    def _synchronize_with_ref(self, ref_signal: _Samples, ac_coupled: list[_Samples],
+                              dc_coupled: list[_Samples]) -> None:
+        while sum(itertools.islice(ref_signal, 0, self.config.daq.ref_period // 2)):
+            ref_signal.popleft()
+            for channel in range(Driver._CHANNELS):
+                ac_coupled[channel].popleft()
+                dc_coupled[channel].popleft()
+            dc_coupled[3].popleft()
+        if len(ref_signal) < self.config.daq.ref_period // 2:
+            return
+        self.synchronize = False
+
+    def build_sample_package(self) -> None:
+        """
+        Creates a package of samples that represents approximately 1 s data. It contains 8000
+        samples.
+        """
+        ref = [self._encoded_buffer.ref_signal.popleft() for _ in range(self.config.daq.number_of_samples)]
+        for i in range(len(ref), self.config.daq.ref_period):
+            if sum(ref[i:i + self.config.daq.ref_period // 2]):
+                logging.warning("Not synchron with reference signal. Trying to synchronise")
+                self.synchronize = True
+                return
+        self.data.DAQ.ref_signal.put(ref)
+        dc_package = [[], [], []]
+        ac_package = [[], [], []]
+        for _ in itertools.repeat(None, self.config.daq.number_of_samples):
+            for channel in range(Driver._CHANNELS):
+                dc_package[channel].append(self._encoded_buffer.dc_coupled[channel].popleft())
+                ac_package[channel].append(self._encoded_buffer.ac_coupled[channel].popleft())
+        self.data.DAQ.dc_coupled.put(dc_package)
+        self.data.DAQ.ac_coupled.put(ac_package)
+
+    def set_valve(self) -> None:
+        if self.bypass:
+            self.write(serial_device.SerialStream("SBP0000"))
+            self.bypass = False
+        else:
+            self.write(serial_device.SerialStream("SBP0001"))
+            self.bypass = True
+
+    def _process_data(self) -> None:
+        self._reset()
+        self.data = PackageData(DAQData(queue.Queue(maxsize=Driver._QUEUE_SIZE),
+                                        queue.Queue(maxsize=Driver._QUEUE_SIZE),
+                                        queue.Queue(maxsize=Driver._QUEUE_SIZE)),
+                                queue.Queue(maxsize=Driver._QUEUE_SIZE))
+        self._buffer = ""
+        self._encoded_buffer = DAQData(deque(), [deque(), deque(), deque()], [deque(), deque(), deque()])
+        self._sample_numbers = deque(maxlen=2)
+        while self.connected.is_set():
+            self._encode_data()
+            if self.running.is_set() and len(self._encoded_buffer.ref_signal) >= self.config.daq.number_of_samples:
+                self.build_sample_package()
+
+    def automatic_valve_change(self) -> None:
+        """
+        Periodically bypass a valve. The duty cycle defines how much time for each part (bypassed
+        or not) is spent.
+        """
+        def switch() -> None:
+            while self.connected and self.automatic_switch.set():
+                if self.bypass:
+                    self.set_valve()
+                    time.sleep(self.config.valve.period * self.config.valve.duty_cycle / 100)
+                else:
+                    self.set_valve()
+                    time.sleep(self.config.valve.period * (1 - self.config.valve.duty_cycle / 100))
+
+        threading.Thread(target=switch, daemon=True).start()
+
+    def do_shutdown(self) -> None:
+        self.write(serial_device.SerialStream("SHD0001"))
```

### Comparing `minipti-1.9.1/src/minipti.egg-info/PKG-INFO` & `minipti-1.9.3/src/minipti.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,124 +1,124 @@
-Metadata-Version: 2.1
-Name: minipti
-Version: 1.9.1
-Summary: Provides algorithm and GUI for photo thermal interferometry and 3x3 couplers
-Author-email: Jonas Bilal <jonasbilal@outlook.com>
-Project-URL: Homepage, https://www.fhnw.ch/en/about-fhnw/schools/school-of-engineering/institutes/institute-for-sensors-and-electronics/aerosol-measurement-technology
-Project-URL: Source, https://github.com/bilaljo/MiniPTI
-Project-URL: Bug Tracker, https://github.com/bilaljo/MiniPTI/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: algorithm
-Provides-Extra: gui
-License-File: LICENSE
-
-# MiniPTI
-
-<p style="text-align: center;">
-<img alt="flowchart" src="https://www.fhnw.ch/de/medien/logos/media/fhnw_e_10mm.jpg" class="centre">
-</p>
-
-In this repository a GUI is provided to control the MiniPTI as also presented in [Waveguide based passively demodulated photothermal interferometer for light absorption measurements of trace substances](https://doi.org/10.1364/AO.476868). In addition to the GUI, Python implementations of the presented algorithms and the driver software for the MiniPTI hardware are also provided as libraries.
-
-# 1. installation
-In order to make the library light-weighted different installation options exist.
-
-To install only the interferometry library you can install it with
-```
-pip install minipti
-```
-To additionally use the inversion algorithm you can type
-```bash
-pip install minipti[algorithm]
-```
-To install the entire package (GUI, algorithms and hardware drivers) you can type
-```bash
-pip install minipti[gui]
-```
-# 2. Usage and GUI
-The GUI can be used via
-```bash
-python -m minipti
-```
-
-## 2.1 Home Tab
-<p style="text-align: center;">
-<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/home.png">
-</p>
-
-## 2.2 Pump Laser Tab
-### 2.2.1 Pump Laser Driver Tab
-<p style="text-align: center;">
-<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/pump_laser_tab.png">
-</p>
-
-### 2.2.2 Pump Laser Tec Driver Tab
-<p style="text-align: center;">
-<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/pump_tec.png">
-</p>
-
-## 2.3 Probe Laser Tab
-### 2.3.1 Probe Laser Driver Tab
-<p style="text-align: center;">
-<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/probe_laser_tab.png">
-</p>
-
-### 2.3.1 Probe Laser Tec Driver Tab
-<p style="text-align: center;">
-<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/probe_tec.png">
-</p>
-
-## 2.3 Plotting Tabs
-### 2.3.1 DC Signals
-<p style="text-align: center;">
-<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/dc_tab.png">
-</p>
-
-### 2.3.2 Amplitudes
-<p style="text-align: center;">
-<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/amplitudes_tab.png">
-</p>
-
-### 2.3.3 Output Phases
-<p style="text-align: center;">
-<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/output_phases_tab.png">
-</p>
-
-### 2.3.4 Interferometric Phase
-<p style="text-align: center;">
-<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/phase_tab.png">
-</p>
-
-### 2.3.5 Sensitivity
-<p style="text-align: center;">
-<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/sensitivity_tab.png">
-</p>
-
-### 2.3.6 Symmetry
-<p style="text-align: center;">
-<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/sym_tab.png">
-</p>
-
-### 2.3.7 PTI Signal
-<p style="text-align: center;">
-<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/pti_signal_tab.png">
-</p>
-
-# 3. libraries
-
-## 3.1 Algorithm
-The subpackage Algorithm contains the implementation of the algorithms and can be divided into the subpackages interferometry and pti. interferometry contains the algorithms for the interferometric phase and characterisation of the interferometer. pti contains the algorithms for decimation and PTI inversion.
-
-It is also possible to use only the interferometer subpackage without having to install dependencies for the other packages.
-
-### 3.1.1 Interferometry
-interferometry contains the classes interferometer and characterisation.
-Examples of usage can be found under <a href="https://github.com/bilaljo/MiniPTI/blob/main/examples/interferometry.py">examples/interferometer.py</a> and
-<a href="https://github.com/bilaljo/MiniPTI/blob/main/examples/characterisation.py">examples/characterisation.py</a>.
-### 3.1.2 PTI
-pti contains the classes decimation inversion. Example calls can be found under <a href="https://github.com/bilaljo/MiniPTI/blob/main/examples/pti_inversion.py">examples/pti_inversion.py</a>
-## 3.2 Hardware
-Hardware contains the classes to control the motherboard (DAQ + BMS), laser (Probe and Pump Laser) and TEC driver as well as the valve control.
+Metadata-Version: 2.1
+Name: minipti
+Version: 1.9.3
+Summary: Provides algorithm and GUI for photo thermal interferometry and 3x3 couplers
+Author-email: Jonas Bilal <jonasbilal@outlook.com>
+Project-URL: Homepage, https://www.fhnw.ch/en/about-fhnw/schools/school-of-engineering/institutes/institute-for-sensors-and-electronics/aerosol-measurement-technology
+Project-URL: Source, https://github.com/bilaljo/MiniPTI
+Project-URL: Bug Tracker, https://github.com/bilaljo/MiniPTI/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: algorithm
+Provides-Extra: gui
+License-File: LICENSE
+
+# MiniPTI
+
+<p style="text-align: center;">
+<img alt="flowchart" src="https://www.fhnw.ch/de/medien/logos/media/fhnw_e_10mm.jpg" class="centre">
+</p>
+
+In this repository a GUI is provided to control the MiniPTI as also presented in [Waveguide based passively demodulated photothermal interferometer for light absorption measurements of trace substances](https://doi.org/10.1364/AO.476868). In addition to the GUI, Python implementations of the presented algorithms and the driver software for the MiniPTI hardware are also provided as libraries.
+
+# 1. installation
+In order to make the library light-weighted different installation options exist.
+
+To install only the interferometry library you can install it with
+```
+pip install minipti
+```
+To additionally use the inversion algorithm you can type
+```bash
+pip install minipti[algorithm]
+```
+To install the entire package (GUI, algorithms and hardware drivers) you can type
+```bash
+pip install minipti[gui]
+```
+# 2. Usage and GUI
+The GUI can be used via
+```bash
+python -m minipti
+```
+
+## 2.1 Home Tab
+<p style="text-align: center;">
+<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/home.png">
+</p>
+
+## 2.2 Pump Laser Tab
+### 2.2.1 Pump Laser Driver Tab
+<p style="text-align: center;">
+<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/pump_laser_tab.png">
+</p>
+
+### 2.2.2 Pump Laser Tec Driver Tab
+<p style="text-align: center;">
+<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/pump_tec.png">
+</p>
+
+## 2.3 Probe Laser Tab
+### 2.3.1 Probe Laser Driver Tab
+<p style="text-align: center;">
+<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/probe_laser_tab.png">
+</p>
+
+### 2.3.1 Probe Laser Tec Driver Tab
+<p style="text-align: center;">
+<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/probe_tec.png">
+</p>
+
+## 2.3 Plotting Tabs
+### 2.3.1 DC Signals
+<p style="text-align: center;">
+<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/dc_tab.png">
+</p>
+
+### 2.3.2 Amplitudes
+<p style="text-align: center;">
+<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/amplitudes_tab.png">
+</p>
+
+### 2.3.3 Output Phases
+<p style="text-align: center;">
+<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/output_phases_tab.png">
+</p>
+
+### 2.3.4 Interferometric Phase
+<p style="text-align: center;">
+<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/phase_tab.png">
+</p>
+
+### 2.3.5 Sensitivity
+<p style="text-align: center;">
+<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/sensitivity_tab.png">
+</p>
+
+### 2.3.6 Symmetry
+<p style="text-align: center;">
+<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/sym_tab.png">
+</p>
+
+### 2.3.7 PTI Signal
+<p style="text-align: center;">
+<img alt="flowchart" src="https://raw.githubusercontent.com/bilaljo/MiniPTI/main/images/gui/pti_signal_tab.png">
+</p>
+
+# 3. libraries
+
+## 3.1 Algorithm
+The subpackage Algorithm contains the implementation of the algorithms and can be divided into the subpackages interferometry and pti. interferometry contains the algorithms for the interferometric phase and characterisation of the interferometer. pti contains the algorithms for decimation and PTI inversion.
+
+It is also possible to use only the interferometer subpackage without having to install dependencies for the other packages.
+
+### 3.1.1 Interferometry
+interferometry contains the classes interferometer and characterisation.
+Examples of usage can be found under <a href="https://github.com/bilaljo/MiniPTI/blob/main/examples/interferometry.py">examples/interferometer.py</a> and
+<a href="https://github.com/bilaljo/MiniPTI/blob/main/examples/characterisation.py">examples/characterisation.py</a>.
+### 3.1.2 PTI
+pti contains the classes decimation inversion. Example calls can be found under <a href="https://github.com/bilaljo/MiniPTI/blob/main/examples/pti_inversion.py">examples/pti_inversion.py</a>
+## 3.2 Hardware
+Hardware contains the classes to control the motherboard (DAQ + BMS), laser (Probe and Pump Laser) and TEC driver as well as the valve control.
```

