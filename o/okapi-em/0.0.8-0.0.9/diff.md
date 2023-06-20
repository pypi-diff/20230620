# Comparing `tmp/okapi-em-0.0.8.tar.gz` & `tmp/okapi-em-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "okapi-em-0.0.8.tar", last modified: Tue Jan 10 22:11:38 2023, max compression
+gzip compressed data, was "okapi-em-0.0.9.tar", last modified: Tue Jun 20 16:12:42 2023, max compression
```

## Comparing `okapi-em-0.0.8.tar` & `okapi-em-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-01-10 22:11:38.417612 okapi-em-0.0.8/
--rw-rw-rw-   0        0        0    11558 2022-04-08 13:56:42.000000 okapi-em-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      101 2022-10-13 11:57:49.000000 okapi-em-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     4631 2023-01-10 22:11:38.417612 okapi-em-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3671 2022-12-15 16:04:39.000000 okapi-em-0.0.8/README.md
--rw-rw-rw-   0        0        0      184 2022-10-13 11:57:50.000000 okapi-em-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0     1564 2023-01-10 22:11:38.452223 okapi-em-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-01-10 22:11:38.199114 okapi-em-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-01-10 22:11:38.288908 okapi-em-0.0.8/src/okapi_em/
--rw-rw-rw-   0        0        0      652 2023-01-10 17:06:33.000000 okapi-em-0.0.8/src/okapi_em/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-10 22:11:38.409586 okapi-em-0.0.8/src/okapi_em/_tests/
--rw-rw-rw-   0        0        0        0 2022-10-13 11:57:50.000000 okapi-em-0.0.8/src/okapi_em/_tests/__init__.py
--rw-rw-rw-   0        0        0     1339 2023-01-10 22:10:29.000000 okapi-em-0.0.8/src/okapi_em/_tests/test_widget.py
--rw-rw-rw-   0        0        0    31822 2023-01-10 22:10:29.000000 okapi-em-0.0.8/src/okapi_em/_widget.py
--rw-rw-rw-   0        0        0     1435 2022-10-19 16:43:45.000000 okapi-em-0.0.8/src/okapi_em/filters.py
--rw-rw-rw-   0        0        0     6407 2022-10-19 16:43:45.000000 okapi-em-0.0.8/src/okapi_em/measure_charging.py
--rw-rw-rw-   0        0        0      351 2022-10-13 11:57:50.000000 okapi-em-0.0.8/src/okapi_em/napari.yaml
--rw-rw-rw-   0        0        0     3350 2023-01-10 15:03:30.000000 okapi-em-0.0.8/src/okapi_em/quoll_wrapper.py
--rw-rw-rw-   0        0        0    18501 2022-11-11 09:58:14.000000 okapi-em-0.0.8/src/okapi_em/slice_alignment.py
-drwxrwxrwx   0        0        0        0 2023-01-10 22:11:38.401347 okapi-em-0.0.8/src/okapi_em.egg-info/
--rw-rw-rw-   0        0        0     4631 2023-01-10 22:11:38.000000 okapi-em-0.0.8/src/okapi_em.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      532 2023-01-10 22:11:38.000000 okapi-em-0.0.8/src/okapi_em.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-10 22:11:38.000000 okapi-em-0.0.8/src/okapi_em.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-01-10 22:11:38.000000 okapi-em-0.0.8/src/okapi_em.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      132 2023-01-10 22:11:38.000000 okapi-em-0.0.8/src/okapi_em.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-01-10 22:11:38.000000 okapi-em-0.0.8/src/okapi_em.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 16:12:42.050691 okapi-em-0.0.9/
+-rw-rw-rw-   0        0        0    11558 2022-04-08 13:56:42.000000 okapi-em-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      101 2022-10-13 11:57:49.000000 okapi-em-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     5683 2023-06-20 16:12:42.051690 okapi-em-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4723 2023-02-09 16:47:46.000000 okapi-em-0.0.9/README.md
+-rw-rw-rw-   0        0        0      184 2022-10-13 11:57:50.000000 okapi-em-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0     1566 2023-06-20 16:12:42.053691 okapi-em-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-20 16:12:41.988268 okapi-em-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-06-20 16:12:42.015863 okapi-em-0.0.9/src/okapi_em/
+-rw-rw-rw-   0        0        0      652 2023-06-20 16:11:28.000000 okapi-em-0.0.9/src/okapi_em/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:12:42.049684 okapi-em-0.0.9/src/okapi_em/_tests/
+-rw-rw-rw-   0        0        0        0 2022-10-13 11:57:50.000000 okapi-em-0.0.9/src/okapi_em/_tests/__init__.py
+-rw-rw-rw-   0        0        0     1044 2023-06-20 16:11:28.000000 okapi-em-0.0.9/src/okapi_em/_tests/test_slice_alignment.py
+-rw-rw-rw-   0        0        0     1339 2023-01-10 22:10:29.000000 okapi-em-0.0.9/src/okapi_em/_tests/test_widget.py
+-rw-rw-rw-   0        0        0    37925 2023-06-20 16:11:28.000000 okapi-em-0.0.9/src/okapi_em/_widget.py
+-rw-rw-rw-   0        0        0     1435 2022-10-19 16:43:45.000000 okapi-em-0.0.9/src/okapi_em/filters.py
+-rw-rw-rw-   0        0        0     6407 2022-10-19 16:43:45.000000 okapi-em-0.0.9/src/okapi_em/measure_charging.py
+-rw-rw-rw-   0        0        0      351 2022-10-13 11:57:50.000000 okapi-em-0.0.9/src/okapi_em/napari.yaml
+-rw-rw-rw-   0        0        0     3350 2023-01-10 15:03:30.000000 okapi-em-0.0.9/src/okapi_em/quoll_wrapper.py
+-rw-rw-rw-   0        0        0    32858 2023-06-20 16:11:28.000000 okapi-em-0.0.9/src/okapi_em/slice_alignment.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:12:42.045190 okapi-em-0.0.9/src/okapi_em.egg-info/
+-rw-rw-rw-   0        0        0     5683 2023-06-20 16:12:41.000000 okapi-em-0.0.9/src/okapi_em.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      576 2023-06-20 16:12:41.000000 okapi-em-0.0.9/src/okapi_em.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 16:12:41.000000 okapi-em-0.0.9/src/okapi_em.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-20 16:12:41.000000 okapi-em-0.0.9/src/okapi_em.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      131 2023-06-20 16:12:41.000000 okapi-em-0.0.9/src/okapi_em.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-20 16:12:41.000000 okapi-em-0.0.9/src/okapi_em.egg-info/top_level.txt
```

### Comparing `okapi-em-0.0.8/LICENSE` & `okapi-em-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `okapi-em-0.0.8/PKG-INFO` & `okapi-em-0.0.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okapi-em
-Version: 0.0.8
+Version: 0.0.9
 Summary: napari plugin to deal with charging artifacts in tomography electron microscopy data
 Author: Luis Perdigao
 Author-email: luis.perdigao@rfi.ac.uk
 License: Apache-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: napari
@@ -36,14 +36,19 @@
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/okapi-em)](https://napari-hub.org/plugins/okapi-em)
 -->
 
 A napari plugin for processing serial-FIB-SEM data.
 
 Powered by [chafer] and [quoll].
 
+
+A full description of this software is presented in biorXiv preprint paper:
+
+https://doi.org/10.1101/2022.12.15.520541
+
 This [napari] plugin contains the following tools:
 
 - slice alignment using constrained SIFT
 - two charge artifact suppression filters
     - directional fourier bandapass filter
     - line-by-line filter function optimiser and subtraction (requires charge artifact labels) - uses [chafer]
 - fourier ring correlation (FRC) resolution estimation - uses [quoll]
@@ -60,53 +65,59 @@
 https://napari.org/plugins/stable/index.html
 -->
 
 ## Installation
 
 You can install `okapi-em` via [pip]:
 
-`pip install okapi-em`
-
-For development mode it can be installed, clone this package then navigate to the cloned `okapi-em` folder and run:
-
-`pip install -e .`
-
-This should install in any machine, however ...
+`>pip install okapi-em`
 
-Currently the FRC calculation provided by the [quoll] package which is optional because
-of its stringent environmemt requirements from miplib package. These currently are:
+or using napari's plugin installation engine `Plugins->Install/Uninstall Plugins...` and filter for **Okapi-EM**.
 
-- python 3.7
-- linux OS
+For installing in development mode , clone this package then navigate to the cloned `okapi-em` folder and run:
 
-This issue will be addressed in future version.
+`>pip install -e .`
 
+Okapi-EM is a napari plugin. Launching napari is therefore required.
 
-To install okapi-em with quoll included:
+`>napari`
 
-`pip install okapi-em[all]`
+and then navigate `Menu->Plugins->Okapi-EM`
 
-Note that to launch napari in python 3.7 you will need to use the command:
+Note that to launch napari in older versions of python (<=3.7) you will need to use the command:
 
-`python -m napari`
+`>python -m napari`
 
+## Computing requirements
+Okapi-EM does not require powerful computers to run. None of the tools use GPU accelaration.
 
+The minimum recommended RAM depends on the size of the data being used in napari. For a full image stack of 1Gb, it is recommended that user ensure that 3Gb of RAM is available or can be used. Modern OS's can extend physical RAM using `swap` memory (Linux) or cache (in Windows and also known as virtual memory), but processing can be significantly slower.
 
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
 ## License
 
 Distributed under the terms of the [Apache Software License 2.0] license,
 "okapi-em" is free and open source software
 
+## Citing
+
+Please cite usage using the following reference.
+
+Perdigão, L. M. A. et al. Okapi-EM – a napari plugin for processing and analysing cryogenic serial FIB/SEM images. 2022.12.15.520541 Preprint at https://doi.org/10.1101/2022.12.15.520541 (2022).
+
+
 ## Issues
 
+There is currently a known issue with napari running in Linux machines, that it does not find the OpenGL driver correctly.
+This will hopefully be resolved in the near future. If you bump into this issue we recommend trying to downgrade the python version. This is not an Okapi-EM problem.
+
 If you encounter any problems, please file an issue along with a detailed description.
 
 [quoll]: https://github.com/rosalindfranklininstitute/quoll
 [chafer]: https://github.com/rosalindfranklininstitute/chafer
 [napari]: https://github.com/napari/napari
 [Cookiecutter]: https://github.com/audreyr/cookiecutter
 [@napari]: https://github.com/napari
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `okapi-em-0.0.8/README.md` & `okapi-em-0.0.9/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -11,14 +11,19 @@
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/okapi-em)](https://napari-hub.org/plugins/okapi-em)
 -->
 
 A napari plugin for processing serial-FIB-SEM data.
 
 Powered by [chafer] and [quoll].
 
+
+A full description of this software is presented in biorXiv preprint paper:
+
+https://doi.org/10.1101/2022.12.15.520541
+
 This [napari] plugin contains the following tools:
 
 - slice alignment using constrained SIFT
 - two charge artifact suppression filters
     - directional fourier bandapass filter
     - line-by-line filter function optimiser and subtraction (requires charge artifact labels) - uses [chafer]
 - fourier ring correlation (FRC) resolution estimation - uses [quoll]
@@ -35,53 +40,59 @@
 https://napari.org/plugins/stable/index.html
 -->
 
 ## Installation
 
 You can install `okapi-em` via [pip]:
 
-`pip install okapi-em`
-
-For development mode it can be installed, clone this package then navigate to the cloned `okapi-em` folder and run:
-
-`pip install -e .`
-
-This should install in any machine, however ...
+`>pip install okapi-em`
 
-Currently the FRC calculation provided by the [quoll] package which is optional because
-of its stringent environmemt requirements from miplib package. These currently are:
+or using napari's plugin installation engine `Plugins->Install/Uninstall Plugins...` and filter for **Okapi-EM**.
 
-- python 3.7
-- linux OS
+For installing in development mode , clone this package then navigate to the cloned `okapi-em` folder and run:
 
-This issue will be addressed in future version.
+`>pip install -e .`
 
+Okapi-EM is a napari plugin. Launching napari is therefore required.
 
-To install okapi-em with quoll included:
+`>napari`
 
-`pip install okapi-em[all]`
+and then navigate `Menu->Plugins->Okapi-EM`
 
-Note that to launch napari in python 3.7 you will need to use the command:
+Note that to launch napari in older versions of python (<=3.7) you will need to use the command:
 
-`python -m napari`
+`>python -m napari`
 
+## Computing requirements
+Okapi-EM does not require powerful computers to run. None of the tools use GPU accelaration.
 
+The minimum recommended RAM depends on the size of the data being used in napari. For a full image stack of 1Gb, it is recommended that user ensure that 3Gb of RAM is available or can be used. Modern OS's can extend physical RAM using `swap` memory (Linux) or cache (in Windows and also known as virtual memory), but processing can be significantly slower.
 
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
 ## License
 
 Distributed under the terms of the [Apache Software License 2.0] license,
 "okapi-em" is free and open source software
 
+## Citing
+
+Please cite usage using the following reference.
+
+Perdigão, L. M. A. et al. Okapi-EM – a napari plugin for processing and analysing cryogenic serial FIB/SEM images. 2022.12.15.520541 Preprint at https://doi.org/10.1101/2022.12.15.520541 (2022).
+
+
 ## Issues
 
+There is currently a known issue with napari running in Linux machines, that it does not find the OpenGL driver correctly.
+This will hopefully be resolved in the near future. If you bump into this issue we recommend trying to downgrade the python version. This is not an Okapi-EM problem.
+
 If you encounter any problems, please file an issue along with a detailed description.
 
 [quoll]: https://github.com/rosalindfranklininstitute/quoll
 [chafer]: https://github.com/rosalindfranklininstitute/chafer
 [napari]: https://github.com/napari/napari
 [Cookiecutter]: https://github.com/audreyr/cookiecutter
 [@napari]: https://github.com/napari
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `okapi-em-0.0.8/setup.cfg` & `okapi-em-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206f 6b61 7069 2d65 6d0d 0a76 6572   = okapi-em..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e38 0d0a 6175  sion = 0.0.8..au
+00000020: 7369 6f6e 203d 2030 2e30 2e39 0d0a 6175  sion = 0.0.9..au
 00000030: 7468 6f72 203d 204c 7569 7320 5065 7264  thor = Luis Perd
 00000040: 6967 616f 0d0a 6175 7468 6f72 5f65 6d61  igao..author_ema
 00000050: 696c 203d 206c 7569 732e 7065 7264 6967  il = luis.perdig
 00000060: 616f 4072 6669 2e61 632e 756b 0d0a 6c69  ao@rfi.ac.uk..li
 00000070: 6365 6e73 6520 3d20 4170 6163 6865 2d32  cense = Apache-2
 00000080: 2e30 0d0a 6465 7363 7269 7074 696f 6e20  .0..description 
 00000090: 3d20 6e61 7061 7269 2070 6c75 6769 6e20  = napari plugin 
@@ -58,41 +58,41 @@
 00000390: 6573 203d 200d 0a09 6e75 6d70 790d 0a09  es = ...numpy...
 000003a0: 6d61 6769 6367 7569 0d0a 0963 6861 6665  magicgui...chafe
 000003b0: 720d 0a09 6e61 7061 7269 5b61 6c6c 5d0d  r...napari[all].
 000003c0: 0a09 6f70 656e 6376 2d70 7974 686f 6e20  ..opencv-python 
 000003d0: 2320 6376 3220 6675 6e63 7469 6f6e 7320  # cv2 functions 
 000003e0: 666f 7220 736c 6963 652d 616c 6967 6e6d  for slice-alignm
 000003f0: 656e 740d 0a09 7175 6f6c 6c3e 3d30 2e30  ent...quoll>=0.0
-00000400: 2e34 0d0a 0970 7971 7435 0d0a 0d0a 5b6f  .4...pyqt5....[o
-00000410: 7074 696f 6e73 2e65 7874 7261 735f 7265  ptions.extras_re
-00000420: 7175 6972 655d 0d0a 7465 7374 696e 6720  quire]..testing 
-00000430: 3d20 0d0a 0974 6f78 0d0a 0970 7974 6573  = ...tox...pytes
-00000440: 7420 2023 2068 7474 7073 3a2f 2f64 6f63  t  # https://doc
-00000450: 732e 7079 7465 7374 2e6f 7267 2f65 6e2f  s.pytest.org/en/
-00000460: 6c61 7465 7374 2f63 6f6e 7465 6e74 732e  latest/contents.
-00000470: 6874 6d6c 0d0a 0970 7974 6573 742d 636f  html...pytest-co
-00000480: 7620 2023 2068 7474 7073 3a2f 2f70 7974  v  # https://pyt
-00000490: 6573 742d 636f 762e 7265 6164 7468 6564  est-cov.readthed
-000004a0: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
-000004b0: 2f0d 0a09 7079 7465 7374 2d71 7420 2023  /...pytest-qt  #
-000004c0: 2068 7474 7073 3a2f 2f70 7974 6573 742d   https://pytest-
-000004d0: 7174 2e72 6561 6474 6865 646f 6373 2e69  qt.readthedocs.i
-000004e0: 6f2f 656e 2f6c 6174 6573 742f 0d0a 616c  o/en/latest/..al
-000004f0: 6c20 3d20 0d0a 0969 6d61 6765 696f 2d66  l = ...imageio-f
-00000500: 666d 7065 6720 2361 6e6e 6f79 696e 676c  fmpeg #annoyingl
-00000510: 7920 6e61 7061 7269 2031 2e34 2e31 3420  y napari 1.4.14 
-00000520: 6e65 6564 7320 7468 6973 2062 7574 2069  needs this but i
-00000530: 7320 6e6f 7420 696e 7374 616c 6c65 6420  s not installed 
-00000540: 756e 6c65 7373 2073 7065 6369 6669 6564  unless specified
-00000550: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
-00000560: 6b61 6765 732e 6669 6e64 5d0d 0a77 6865  kages.find]..whe
-00000570: 7265 203d 2073 7263 0d0a 0d0a 5b6f 7074  re = src....[opt
-00000580: 696f 6e73 2e70 6163 6b61 6765 5f64 6174  ions.package_dat
-00000590: 615d 0d0a 2a20 3d20 2a2e 7961 6d6c 0d0a  a]..* = *.yaml..
-000005a0: 0d0a 5b6f 7074 696f 6e73 2e65 6e74 7279  ..[options.entry
-000005b0: 5f70 6f69 6e74 735d 0d0a 6e61 7061 7269  _points]..napari
-000005c0: 2e6d 616e 6966 6573 7420 3d20 0d0a 096f  .manifest = ...o
-000005d0: 6b61 7069 2d65 6d20 3d20 6f6b 6170 695f  kapi-em = okapi_
-000005e0: 656d 3a6e 6170 6172 692e 7961 6d6c 0d0a  em:napari.yaml..
-000005f0: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
-00000600: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
-00000610: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
+00000400: 2e34 0d0a 090d 0a09 7174 7079 0d0a 0d0a  .4......qtpy....
+00000410: 5b6f 7074 696f 6e73 2e65 7874 7261 735f  [options.extras_
+00000420: 7265 7175 6972 655d 0d0a 7465 7374 696e  require]..testin
+00000430: 6720 3d20 0d0a 0974 6f78 0d0a 0970 7974  g = ...tox...pyt
+00000440: 6573 7420 2023 2068 7474 7073 3a2f 2f64  est  # https://d
+00000450: 6f63 732e 7079 7465 7374 2e6f 7267 2f65  ocs.pytest.org/e
+00000460: 6e2f 6c61 7465 7374 2f63 6f6e 7465 6e74  n/latest/content
+00000470: 732e 6874 6d6c 0d0a 0970 7974 6573 742d  s.html...pytest-
+00000480: 636f 7620 2023 2068 7474 7073 3a2f 2f70  cov  # https://p
+00000490: 7974 6573 742d 636f 762e 7265 6164 7468  ytest-cov.readth
+000004a0: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
+000004b0: 7374 2f0d 0a09 7079 7465 7374 2d71 7420  st/...pytest-qt 
+000004c0: 2023 2068 7474 7073 3a2f 2f70 7974 6573   # https://pytes
+000004d0: 742d 7174 2e72 6561 6474 6865 646f 6373  t-qt.readthedocs
+000004e0: 2e69 6f2f 656e 2f6c 6174 6573 742f 0d0a  .io/en/latest/..
+000004f0: 616c 6c20 3d20 0d0a 0969 6d61 6765 696f  all = ...imageio
+00000500: 2d66 666d 7065 6720 2361 6e6e 6f79 696e  -ffmpeg #annoyin
+00000510: 676c 7920 6e61 7061 7269 2031 2e34 2e31  gly napari 1.4.1
+00000520: 3420 6e65 6564 7320 7468 6973 2062 7574  4 needs this but
+00000530: 2069 7320 6e6f 7420 696e 7374 616c 6c65   is not installe
+00000540: 6420 756e 6c65 7373 2073 7065 6369 6669  d unless specifi
+00000550: 6564 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  ed....[options.p
+00000560: 6163 6b61 6765 732e 6669 6e64 5d0d 0a77  ackages.find]..w
+00000570: 6865 7265 203d 2073 7263 0d0a 0d0a 5b6f  here = src....[o
+00000580: 7074 696f 6e73 2e70 6163 6b61 6765 5f64  ptions.package_d
+00000590: 6174 615d 0d0a 2a20 3d20 2a2e 7961 6d6c  ata]..* = *.yaml
+000005a0: 0d0a 0d0a 5b6f 7074 696f 6e73 2e65 6e74  ....[options.ent
+000005b0: 7279 5f70 6f69 6e74 735d 0d0a 6e61 7061  ry_points]..napa
+000005c0: 7269 2e6d 616e 6966 6573 7420 3d20 0d0a  ri.manifest = ..
+000005d0: 096f 6b61 7069 2d65 6d20 3d20 6f6b 6170  .okapi-em = okap
+000005e0: 695f 656d 3a6e 6170 6172 692e 7961 6d6c  i_em:napari.yaml
+000005f0: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
+00000600: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
+00000610: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
```

### Comparing `okapi-em-0.0.8/src/okapi_em/__init__.py` & `okapi-em-0.0.9/src/okapi_em/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,10 +10,10 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 '''
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 from ._widget import MainQWidget
```

### Comparing `okapi-em-0.0.8/src/okapi_em/_tests/test_widget.py` & `okapi-em-0.0.9/src/okapi_em/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `okapi-em-0.0.8/src/okapi_em/_widget.py` & `okapi-em-0.0.9/src/okapi_em/_widget.py`

 * *Files 10% similar despite different names*

```diff
@@ -87,15 +87,14 @@
         self.tabChargeSuppr.setLayout(self.t0_vbox0)
 
         # Filter: Directional band-pass
         # Radiobutton followed by a box with controls for this filter
         self.rbDirFFT = QRadioButton("Directional band-pass FFT filter")
         self.rbDirFFT.setChecked(False)
         self.t0_vbox0.addWidget( self.rbDirFFT)
-        #TODO, may need 'connection'
         #Options for this filter are contained in the next box grpBox1
         self.grpBox1 = QGroupBox("") #Box, no title, radiobutton does it
         #self.tabChargeSuppr.addWidget(self.grpBox1)
         self.t0_vbox0.addWidget(self.grpBox1)
 
         self.vbox2 = QVBoxLayout()
         self.grpBox1.setLayout(self.vbox2)
@@ -177,19 +176,19 @@
     def ui_do_tab_SliceAlignment(self):
         # /tabSliceAlignemnt \
         self.tabSliceAlignment = QWidget()
         self.tabwidget.addTab(self.tabSliceAlignment, "Slice Alignment")
         self.tabSliceAlignment_l = QVBoxLayout() #Items organised vertically
         self.tabSliceAlignment.setLayout(self.tabSliceAlignment_l)
         
-        self.chkbxTranslate= QCheckBox("Translate")
+        self.chkbxTranslate= QCheckBox("Translation")
         self.chkbxTranslate.setChecked(True)
         self.tabSliceAlignment_l.addWidget(self.chkbxTranslate)
-        self.chkbxAffine= QCheckBox("Linear all free (ov. below)")
-        self.tabSliceAlignment_l.addWidget(self.chkbxAffine)
+        self.chkbxLinear= QCheckBox("Linear all free (ov. below)")
+        self.tabSliceAlignment_l.addWidget(self.chkbxLinear)
 
         hl_Rot = QHBoxLayout()
         self.tabSliceAlignment_l.addLayout(hl_Rot)
         self.chkbxRotation = QCheckBox("rotation (ov. shear)")
         hl_Rot.addWidget(self.chkbxRotation)
         self.chkbxShearX = QCheckBox("shear X")
         self.chkbxShearX.setChecked(True)
@@ -203,14 +202,43 @@
         hl_Scaling.addWidget(self.chkbxScaling)
         self.chkbxStretchX = QCheckBox("stretch x")
         hl_Scaling.addWidget(self.chkbxStretchX)
         self.chkbxStretchY = QCheckBox("stretch y")
         hl_Scaling.addWidget(self.chkbxStretchY)
         self.chkbxStretchY.setChecked(True)
 
+        #parameters to control slice alignment feature matching
+        qgrid_adj_params = QGridLayout()
+        self.tabSliceAlignment_l.addLayout(qgrid_adj_params)
+        label_slice_align0 = QLabel("Ratio test:")
+        qgrid_adj_params.addWidget(label_slice_align0,0,0)
+        self.spb_SliceAlign_RatioTest=QDoubleSpinBox()
+        self.spb_SliceAlign_RatioTest.setMinimum(0.1)
+        self.spb_SliceAlign_RatioTest.setMaximum(1.0)
+        self.spb_SliceAlign_RatioTest.setDecimals(2)
+        self.spb_SliceAlign_RatioTest.setSingleStep(0.1)
+        self.spb_SliceAlign_RatioTest.setValue(0.80)
+        self.spb_SliceAlign_RatioTest.setToolTip("Ratio test filters matching features based in the ratio to second match score.\nHigher value gets more matches but lower match confidence.\nValues from 0.1 to 1.0.")
+        qgrid_adj_params.addWidget(self.spb_SliceAlign_RatioTest, 0,1)
+
+        label_d2dmedian_ratio = QLabel("D2Dmedian ratio:")
+        qgrid_adj_params.addWidget(label_d2dmedian_ratio,1,0)
+        self.spb_SliceAlign_D2Dmedian_Ratio=QDoubleSpinBox()
+        self.spb_SliceAlign_D2Dmedian_Ratio.setMinimum(0.01)
+        self.spb_SliceAlign_D2Dmedian_Ratio.setMaximum(10.0)
+        self.spb_SliceAlign_D2Dmedian_Ratio.setDecimals(2)
+        self.spb_SliceAlign_D2Dmedian_Ratio.setSingleStep(0.01)
+        self.spb_SliceAlign_D2Dmedian_Ratio.setValue(0.05)
+        self.spb_SliceAlign_D2Dmedian_Ratio.setToolTip("Distance to median ratio filter.\nHigher value gets more matches but less precision.\nValues from 0.001 to 10.0. default 0.05")
+        qgrid_adj_params.addWidget(self.spb_SliceAlign_D2Dmedian_Ratio, 1,1)
+
+        self.btn_testSA=QPushButton("Test/preview slice alignment")
+        qgrid_adj_params.addWidget(self.btn_testSA, 2,0)
+        self.btn_testSA.clicked.connect(self.btn_testSA_onclick) #Signal
+
         #Button to start the alignement
         self.btnSACalculate = QPushButton("Align")
         self.tabSliceAlignment_l.addWidget(self.btnSACalculate)
         self.btnSACalculate.clicked.connect(self.btnSACalculate_onclick) #Signal
 
 
     def ui_do_tab_ResMeas(self):
@@ -401,53 +429,68 @@
 
     def btnSACalculate_onclick(self):
         print("btnSACalculate_onclick()")
 
         res=None
 
         data3d = self.w_setselect.get_active_image_selected_data()
+        if  data3d is None:
+            raise ValueError("Could not get active image data.")
 
-        if data3d.ndim==3:
-
-            #Ensure data3d is napari and not dask
-            data3d = np.array(data3d)
-
-            #Estimate number of iterations for progress bar
-            nslices = data3d.shape[0]
-            niterations = 2*(nslices+1)
-
-            pbr=progress(total=niterations,desc="Alignment progress")
+        if data3d.ndim!=3:
+            raise ValueError("Data selected is not 3D")
+        
 
-            def callbkfn():
-                pbr.update(1)
-                pbr.refresh()
+        #Ensure data3d is napari and not dask
+        data3d = np.asarray(data3d)
 
-            #Show or not show Activity dialog?
-            #activ_dialog=self.viewer.window._qt_viewer.window()._activity_dialog #Warning this will be unavailable in the future
-            #activ_dialog.show()
+        #Estimate number of iterations for progress bar
+        nslices = data3d.shape[0]
+        niterations = 2*(nslices+1) #TODO: Proably should be 2nslices
 
-            #res= slice_alignment.align_stack(data3d, slice_alignment.ALIGNMENT_METHOD_DEFAULT,callbkfn)
-            sa_method = slice_alignment.ALIGNMENT_METHOD_DEFAULT
+        pbr=progress(total=niterations,desc="Alignment progress")
 
-            sa_method['translation'] = self.chkbxTranslate.isChecked()
-            sa_method['affine'] = self.chkbxAffine.isChecked()
-            sa_method['rotation'] = self.chkbxRotation.isChecked()
-            sa_method['shearing_x'] = self.chkbxShearX.isChecked()
-            sa_method['shearing_y'] = self.chkbxShearY.isChecked()
-            sa_method['scaling'] = self.chkbxScaling.isChecked()
-            sa_method['stretching_x'] = self.chkbxStretchX.isChecked()
-            sa_method['stretching_y'] = self.chkbxStretchY.isChecked()
+        def callbkfn():
+            pbr.update(1)
+            pbr.refresh()
 
-            res= slice_alignment.align_stack(data3d, sa_method,callbkfn)
+        #Show or not show Activity dialog?
+        #activ_dialog=self.viewer.window._qt_viewer.window()._activity_dialog #Warning this will be unavailable in the future
+        #activ_dialog.show()
+
+        #res= slice_alignment.align_stack(data3d, slice_alignment.ALIGNMENT_METHOD_DEFAULT,callbkfn)
+        # sa_method = slice_alignment.ALIGNMENT_METHOD_DEFAULT
+
+        # sa_method['translation'] = self.chkbxTranslate.isChecked()
+        # #sa_method['affine'] = self.chkbxAffine.isChecked()
+        # sa_method['linear'] = self.chkbxLinear.isChecked()
+        # sa_method['rotation'] = self.chkbxRotation.isChecked()
+        # sa_method['shearing_x'] = self.chkbxShearX.isChecked()
+        # sa_method['shearing_y'] = self.chkbxShearY.isChecked()
+        # sa_method['scaling'] = self.chkbxScaling.isChecked()
+        # sa_method['stretching_x'] = self.chkbxStretchX.isChecked()
+        # sa_method['stretching_y'] = self.chkbxStretchY.isChecked()
+
+        #res= slice_alignment.align_stack(data3d, sa_method,callbkfn)
+
+        p0= self.get_UI_SA_parameters()
+
+        res, _= slice_alignment.align_stack1(data3d,
+                                        p0['method'],
+                                        d2dmedian_ratio=p0['d2dmedian'],
+                                        ratio_test=p0['reldist2match'],
+                                        callbk_tick_fn=callbkfn
+                                    )
 
-            pbr.close()
-            #activ_dialog.hide()
+        pbr.close()
+        #activ_dialog.hide()
 
-            if not res is None:
-                self.viewer.add_image(res, name="stack aligned")
+        if not res is None:
+            self.viewer.add_image(res, name="stack aligned")
+        
 
     def btnQuollCalcFRC_onclick(self):
         #NOT USED
 
         print("btnQuollCalcFRC_onclick()")
 
         with progress(total=2,desc="FRC calculation in progress") as pbr:
@@ -503,14 +546,67 @@
                 # display a heatmap
                 self.viewer.add_image(heatmap,name="FRC heatmap",
                     colormap="viridis",
                     opacity=0.3
                 )
         return
 
+    def btn_testSA_onclick(self):
+        #Preview of slice alignment with current slice and next
+
+        #Code similar to get_active_image_selected_data_slice()
+        curData = self.w_setselect.get_active_image_selected_data()
+
+        if curData is None:
+            raise ValueError("No data")
+        
+        if curData.ndim!=3:
+            raise ValueError("Data is not 3-dimensional. This plugin only works with 3D data")
+        
+        dims0 = self.viewer.dims
+        nslice = dims0.current_step[0] #Gets the slice number that is currently being viewed, 1st index is the slice number
+        if nslice==curData.shape[0]:
+            raise ValueError("Cannot use this button with the last slice.")
+        
+        order0 = dims0.order[0] #Gets the axis (or plane), that the Viewer is currently viewing
+        if order0 != 0: #z
+            ValueError("Stack alignment only works along z direction. Please change visualisation to XY plane and ndisplay=2 for this button to work.")
+
+        data_2slice = curData[nslice:nslice+2, :,:]
+
+        p0= self.get_UI_SA_parameters()
+
+        res, _= slice_alignment.align_stack1(data_2slice,
+                                          p0['method'],
+                                          d2dmedian_ratio=p0['d2dmedian'],
+                                          ratio_test=p0['reldist2match']
+                                          )
+
+        if not res is None:
+            self.viewer.add_image(res, name="stack-align preview")
+
+
+    def get_UI_SA_parameters(self):
+        sa_method = slice_alignment.ALIGNMENT_METHOD_DEFAULT
+        sa_method['translation'] = self.chkbxTranslate.isChecked()
+        #sa_method['affine'] = self.chkbxAffine.isChecked()
+        sa_method['linear'] = self.chkbxLinear.isChecked()
+        sa_method['rotation'] = self.chkbxRotation.isChecked()
+        sa_method['shearing_x'] = self.chkbxShearX.isChecked()
+        sa_method['shearing_y'] = self.chkbxShearY.isChecked()
+        sa_method['scaling'] = self.chkbxScaling.isChecked()
+        sa_method['stretching_x'] = self.chkbxStretchX.isChecked()
+        sa_method['stretching_y'] = self.chkbxStretchY.isChecked()
+
+        d2dmedian = self.spb_SliceAlign_D2Dmedian_Ratio.value()
+        reldist2match = self.spb_SliceAlign_RatioTest.value()
+
+        return {'method':sa_method,'d2dmedian':d2dmedian, 'reldist2match':reldist2match}
+                
+
     def hello_World(self):
         #prints on the console something enlighting. Only used in CI automated tests
         print ("Hello World, from Okapi-EM!")
 
 
 class widget_ImageSetCurrentSelect(QWidget):
     '''
@@ -564,48 +660,91 @@
         # layout.addWidget(self.l_nslice_v,5,1)
         # self.l_nslice_v.hide() #Hide
 
         self.curImage=None
 
     def b_set_on_click(self):
         print("b_set_on_click()")
-        active0=self.get_active_image() #This also sets default image
-        if not active0 is None:
-            self.l_name_v.setText(active0.name)
-
-            #Check layer is image
-            #self.set_default_napari_image(active0)
+        self.set_active_image_from_nap_layers()
+        
+        #active0=self.get_active_image() #This also sets default image   
+        return
 
     def set_default_napari_image(self,nap_image):
         print("set_default_napari_image()")
         self.curImage=None
         print(f"type(nap_image) : {type(nap_image) }")
         if isinstance(nap_image, napari.layers.Image) or isinstance(nap_image, napari.layers.Labels):
             self.l_name_v.setText(nap_image.name)
             print("Current active layer name is: ", nap_image.name)
             self.curImage = nap_image
             self.l_shape_v.setText(str(self.curImage.data.shape))
+        else:
+            print("Not a valid layer for Okapi-EM.")
+            self.curImage=None
+            self.l_name_v.setText("")
+            self.l_shape_v.setText("")
+        
+        return
 
     def get_active_image(self):
+        print("get_active_image()`")
+        
+        if not self.curImage is None:
+            if self.curImage in self.viewer.layers: #Ensure that image was not deleted
+                return self.curImage
+                
+        #curImage not available anymore
+
+        # try to grab an image from selected
+        self.set_active_image_from_nap_layers()
+        if not self.curImage is None:
+            return self.curImage
+
+        return None
+    
+    def set_active_image_from_nap_layers(self):
+        #Set active image from napari layers
+        print("set_active_image_from_nap_layers()")
+        
         active0=None
         if not self.viewer is None:
             active0 = self.viewer.layers.selection.active #check if any layer is active
             self.set_default_napari_image(active0)
+
         else:
-            print("get_active_image(): no napari.viewer, cannot get active image")
+            raise ValueError("No Viewer")
 
-        return active0
+        return
 
     def get_active_image_selected_data(self) ->ImageData:
         print("get_active_image_selected_data()")
-        if self.curImage is None:
-            self.b_set_on_click() #Does the same thing as clicking the button to set default image data
-            #return self.curImage.data
+
+        im = self.get_active_image()
+        if not im is None:
+            return self.curImage.data
         
-        return self.curImage.data
+        return None
+    
+        # if self.curImage in self.viewer.layers: #Ensure that image was not deleted
+        #     return self.curImage.data
+        # else:
+            
+        
+            # if self.curImage is None:
+            #     #Try to grab an image
+            #     self.b_set_on_click() #Does the same thing as clicking the button to set default image data
+                
+            #     if self.curImage is None: #Check if any layer is selected
+            #         #Clear selection
+
+            #         raise ValueError("Could not get active image data.")
+            #     else:
+                    
+
 
     def get_active_image_selected_data_slice(self):
         print("get_active_image_selected_data_slice()")
 
         curDataSlice=None
 
         curData = self.get_active_image_selected_data()
```

### Comparing `okapi-em-0.0.8/src/okapi_em/filters.py` & `okapi-em-0.0.9/src/okapi_em/filters.py`

 * *Files identical despite different names*

### Comparing `okapi-em-0.0.8/src/okapi_em/measure_charging.py` & `okapi-em-0.0.9/src/okapi_em/measure_charging.py`

 * *Files identical despite different names*

### Comparing `okapi-em-0.0.8/src/okapi_em/quoll_wrapper.py` & `okapi-em-0.0.9/src/okapi_em/quoll_wrapper.py`

 * *Files identical despite different names*

### Comparing `okapi-em-0.0.8/src/okapi_em.egg-info/PKG-INFO` & `okapi-em-0.0.9/src/okapi_em.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okapi-em
-Version: 0.0.8
+Version: 0.0.9
 Summary: napari plugin to deal with charging artifacts in tomography electron microscopy data
 Author: Luis Perdigao
 Author-email: luis.perdigao@rfi.ac.uk
 License: Apache-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: napari
@@ -36,14 +36,19 @@
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/okapi-em)](https://napari-hub.org/plugins/okapi-em)
 -->
 
 A napari plugin for processing serial-FIB-SEM data.
 
 Powered by [chafer] and [quoll].
 
+
+A full description of this software is presented in biorXiv preprint paper:
+
+https://doi.org/10.1101/2022.12.15.520541
+
 This [napari] plugin contains the following tools:
 
 - slice alignment using constrained SIFT
 - two charge artifact suppression filters
     - directional fourier bandapass filter
     - line-by-line filter function optimiser and subtraction (requires charge artifact labels) - uses [chafer]
 - fourier ring correlation (FRC) resolution estimation - uses [quoll]
@@ -60,53 +65,59 @@
 https://napari.org/plugins/stable/index.html
 -->
 
 ## Installation
 
 You can install `okapi-em` via [pip]:
 
-`pip install okapi-em`
-
-For development mode it can be installed, clone this package then navigate to the cloned `okapi-em` folder and run:
-
-`pip install -e .`
-
-This should install in any machine, however ...
+`>pip install okapi-em`
 
-Currently the FRC calculation provided by the [quoll] package which is optional because
-of its stringent environmemt requirements from miplib package. These currently are:
+or using napari's plugin installation engine `Plugins->Install/Uninstall Plugins...` and filter for **Okapi-EM**.
 
-- python 3.7
-- linux OS
+For installing in development mode , clone this package then navigate to the cloned `okapi-em` folder and run:
 
-This issue will be addressed in future version.
+`>pip install -e .`
 
+Okapi-EM is a napari plugin. Launching napari is therefore required.
 
-To install okapi-em with quoll included:
+`>napari`
 
-`pip install okapi-em[all]`
+and then navigate `Menu->Plugins->Okapi-EM`
 
-Note that to launch napari in python 3.7 you will need to use the command:
+Note that to launch napari in older versions of python (<=3.7) you will need to use the command:
 
-`python -m napari`
+`>python -m napari`
 
+## Computing requirements
+Okapi-EM does not require powerful computers to run. None of the tools use GPU accelaration.
 
+The minimum recommended RAM depends on the size of the data being used in napari. For a full image stack of 1Gb, it is recommended that user ensure that 3Gb of RAM is available or can be used. Modern OS's can extend physical RAM using `swap` memory (Linux) or cache (in Windows and also known as virtual memory), but processing can be significantly slower.
 
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
 ## License
 
 Distributed under the terms of the [Apache Software License 2.0] license,
 "okapi-em" is free and open source software
 
+## Citing
+
+Please cite usage using the following reference.
+
+Perdigão, L. M. A. et al. Okapi-EM – a napari plugin for processing and analysing cryogenic serial FIB/SEM images. 2022.12.15.520541 Preprint at https://doi.org/10.1101/2022.12.15.520541 (2022).
+
+
 ## Issues
 
+There is currently a known issue with napari running in Linux machines, that it does not find the OpenGL driver correctly.
+This will hopefully be resolved in the near future. If you bump into this issue we recommend trying to downgrade the python version. This is not an Okapi-EM problem.
+
 If you encounter any problems, please file an issue along with a detailed description.
 
 [quoll]: https://github.com/rosalindfranklininstitute/quoll
 [chafer]: https://github.com/rosalindfranklininstitute/chafer
 [napari]: https://github.com/napari/napari
 [Cookiecutter]: https://github.com/audreyr/cookiecutter
 [@napari]: https://github.com/napari
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `okapi-em-0.0.8/src/okapi_em.egg-info/SOURCES.txt` & `okapi-em-0.0.9/src/okapi_em.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -13,8 +13,9 @@
 src/okapi_em.egg-info/PKG-INFO
 src/okapi_em.egg-info/SOURCES.txt
 src/okapi_em.egg-info/dependency_links.txt
 src/okapi_em.egg-info/entry_points.txt
 src/okapi_em.egg-info/requires.txt
 src/okapi_em.egg-info/top_level.txt
 src/okapi_em/_tests/__init__.py
+src/okapi_em/_tests/test_slice_alignment.py
 src/okapi_em/_tests/test_widget.py
```

