# Comparing `tmp/dpamber-0.3.1.tar.gz` & `tmp/dpamber-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpamber-0.3.1.tar", last modified: Mon Jun 19 07:38:21 2023, max compression
+gzip compressed data, was "dpamber-0.3.2.tar", last modified: Tue Jun 20 21:55:11 2023, max compression
```

## Comparing `dpamber-0.3.1.tar` & `dpamber-0.3.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:38:21.883931 dpamber-0.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:38:21.875931 dpamber-0.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:38:21.879931 dpamber-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-19 07:38:12.000000 dpamber-0.3.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-19 07:38:12.000000 dpamber-0.3.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-19 07:38:12.000000 dpamber-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-19 07:38:12.000000 dpamber-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-19 07:38:21.883931 dpamber-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-19 07:38:12.000000 dpamber-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:38:21.879931 dpamber-0.3.1/dpamber/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-19 07:38:12.000000 dpamber-0.3.1/dpamber/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-06-19 07:38:12.000000 dpamber-0.3.1/dpamber/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-19 07:38:12.000000 dpamber-0.3.1/dpamber/corr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-19 07:38:12.000000 dpamber-0.3.1/dpamber/model_devi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-06-19 07:38:12.000000 dpamber-0.3.1/dpamber/qmbuffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-19 07:38:12.000000 dpamber-0.3.1/dpamber/qmwater_corr.py
--rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-06-19 07:38:12.000000 dpamber-0.3.1/dpamber/read_amber.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-06-19 07:38:12.000000 dpamber-0.3.1/dpamber/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:38:21.879931 dpamber-0.3.1/dpamber.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-19 07:38:21.000000 dpamber-0.3.1/dpamber.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-19 07:38:21.000000 dpamber-0.3.1/dpamber.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 07:38:21.000000 dpamber-0.3.1/dpamber.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-19 07:38:21.000000 dpamber-0.3.1/dpamber.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-19 07:38:21.000000 dpamber-0.3.1/dpamber.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-19 07:38:21.000000 dpamber-0.3.1/dpamber.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-19 07:38:12.000000 dpamber-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-19 07:38:12.000000 dpamber-0.3.1/renovate.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 07:38:21.883931 dpamber-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:38:21.879931 dpamber-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-19 07:38:12.000000 dpamber-0.3.1/tests/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:38:21.883931 dpamber-0.3.1/tests/corr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:38:21.875931 dpamber-0.3.1/tests/corr/dataset/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:38:21.883931 dpamber-0.3.1/tests/corr/dataset/C6H11HW168O6OW83P1/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-19 07:38:12.000000 dpamber-0.3.1/tests/corr/dataset/C6H11HW168O6OW83P1/box.raw
--rw-r--r--   0 runner    (1001) docker     (123)    20625 2023-06-19 07:38:12.000000 dpamber-0.3.1/tests/corr/dataset/C6H11HW168O6OW83P1/coord.raw
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-19 07:38:12.000000 dpamber-0.3.1/tests/corr/dataset/C6H11HW168O6OW83P1/energy.raw
--rw-r--r--   0 runner    (1001) docker     (123)    21026 2023-06-19 07:38:12.000000 dpamber-0.3.1/tests/corr/dataset/C6H11HW168O6OW83P1/force.raw
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 07:38:12.000000 dpamber-0.3.1/tests/corr/dataset/C6H11HW168O6OW83P1/nopbc
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-19 07:38:12.000000 dpamber-0.3.1/tests/corr/dataset/C6H11HW168O6OW83P1/type.raw
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-19 07:38:12.000000 dpamber-0.3.1/tests/corr/dataset/C6H11HW168O6OW83P1/type_map.raw
--rw-r--r--   0 runner    (1001) docker     (123)    73252 2023-06-19 07:38:12.000000 dpamber-0.3.1/tests/corr/high_level.mdfrc
--rw-r--r--   0 runner    (1001) docker     (123)    27097 2023-06-19 07:38:12.000000 dpamber-0.3.1/tests/corr/high_level.mdout
--rw-r--r--   0 runner    (1001) docker     (123)    73252 2023-06-19 07:38:12.000000 dpamber-0.3.1/tests/corr/low_level.mdfrc
--rw-r--r--   0 runner    (1001) docker     (123)    27017 2023-06-19 07:38:12.000000 dpamber-0.3.1/tests/corr/low_level.mdout
--rw-r--r--   0 runner    (1001) docker     (123)  1036937 2023-06-19 07:38:12.000000 dpamber-0.3.1/tests/corr/qmmm.parm7
--rw-r--r--   0 runner    (1001) docker     (123)    97988 2023-06-19 07:38:12.000000 dpamber-0.3.1/tests/corr/rc.nc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:38:21.883931 dpamber-0.3.1/tests/md/
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-19 07:38:12.000000 dpamber-0.3.1/tests/md/md.mdout
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-06-19 07:38:12.000000 dpamber-0.3.1/tests/test_corr.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-19 07:38:12.000000 dpamber-0.3.1/tests/test_model_devi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:38:21.883931 dpamber-0.3.1/tests/uncoverage/
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-19 07:38:12.000000 dpamber-0.3.1/tests/uncoverage/uncoverage.mdout
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-19 07:38:12.000000 dpamber-0.3.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:11.114879 dpamber-0.3.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:11.106879 dpamber-0.3.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:11.106879 dpamber-0.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-20 21:54:58.000000 dpamber-0.3.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-20 21:54:58.000000 dpamber-0.3.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-20 21:54:58.000000 dpamber-0.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-20 21:54:58.000000 dpamber-0.3.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-06-20 21:55:11.114879 dpamber-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-20 21:54:58.000000 dpamber-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:11.110879 dpamber-0.3.2/dpamber/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-20 21:54:58.000000 dpamber-0.3.2/dpamber/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-06-20 21:54:58.000000 dpamber-0.3.2/dpamber/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-20 21:54:58.000000 dpamber-0.3.2/dpamber/corr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-06-20 21:54:58.000000 dpamber-0.3.2/dpamber/model_devi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-06-20 21:54:58.000000 dpamber-0.3.2/dpamber/qmbuffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-20 21:54:58.000000 dpamber-0.3.2/dpamber/qmwater_corr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-06-20 21:54:58.000000 dpamber-0.3.2/dpamber/read_amber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-06-20 21:54:58.000000 dpamber-0.3.2/dpamber/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:11.110879 dpamber-0.3.2/dpamber.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-06-20 21:55:11.000000 dpamber-0.3.2/dpamber.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-20 21:55:11.000000 dpamber-0.3.2/dpamber.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 21:55:11.000000 dpamber-0.3.2/dpamber.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-20 21:55:11.000000 dpamber-0.3.2/dpamber.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-20 21:55:11.000000 dpamber-0.3.2/dpamber.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 21:55:11.000000 dpamber-0.3.2/dpamber.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-20 21:54:58.000000 dpamber-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-20 21:54:58.000000 dpamber-0.3.2/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 21:55:11.114879 dpamber-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:11.110879 dpamber-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-20 21:54:58.000000 dpamber-0.3.2/tests/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:11.110879 dpamber-0.3.2/tests/corr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:11.106879 dpamber-0.3.2/tests/corr/dataset/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:11.114879 dpamber-0.3.2/tests/corr/dataset/C6H11HW168O6OW83P1/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-20 21:54:58.000000 dpamber-0.3.2/tests/corr/dataset/C6H11HW168O6OW83P1/box.raw
+-rw-r--r--   0 runner    (1001) docker     (123)    20625 2023-06-20 21:54:58.000000 dpamber-0.3.2/tests/corr/dataset/C6H11HW168O6OW83P1/coord.raw
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-20 21:54:58.000000 dpamber-0.3.2/tests/corr/dataset/C6H11HW168O6OW83P1/energy.raw
+-rw-r--r--   0 runner    (1001) docker     (123)    21026 2023-06-20 21:54:58.000000 dpamber-0.3.2/tests/corr/dataset/C6H11HW168O6OW83P1/force.raw
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:54:58.000000 dpamber-0.3.2/tests/corr/dataset/C6H11HW168O6OW83P1/nopbc
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-20 21:54:58.000000 dpamber-0.3.2/tests/corr/dataset/C6H11HW168O6OW83P1/type.raw
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-20 21:54:58.000000 dpamber-0.3.2/tests/corr/dataset/C6H11HW168O6OW83P1/type_map.raw
+-rw-r--r--   0 runner    (1001) docker     (123)    73252 2023-06-20 21:54:58.000000 dpamber-0.3.2/tests/corr/high_level.mdfrc
+-rw-r--r--   0 runner    (1001) docker     (123)    27097 2023-06-20 21:54:58.000000 dpamber-0.3.2/tests/corr/high_level.mdout
+-rw-r--r--   0 runner    (1001) docker     (123)    73252 2023-06-20 21:54:58.000000 dpamber-0.3.2/tests/corr/low_level.mdfrc
+-rw-r--r--   0 runner    (1001) docker     (123)    27017 2023-06-20 21:54:58.000000 dpamber-0.3.2/tests/corr/low_level.mdout
+-rw-r--r--   0 runner    (1001) docker     (123)  1036937 2023-06-20 21:54:58.000000 dpamber-0.3.2/tests/corr/qmmm.parm7
+-rw-r--r--   0 runner    (1001) docker     (123)    97988 2023-06-20 21:54:58.000000 dpamber-0.3.2/tests/corr/rc.nc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:11.114879 dpamber-0.3.2/tests/md/
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-20 21:54:58.000000 dpamber-0.3.2/tests/md/md.mdout
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-06-20 21:54:58.000000 dpamber-0.3.2/tests/test_corr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-20 21:54:58.000000 dpamber-0.3.2/tests/test_model_devi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:55:11.114879 dpamber-0.3.2/tests/uncoverage/
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-20 21:54:58.000000 dpamber-0.3.2/tests/uncoverage/uncoverage.mdout
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-20 21:54:58.000000 dpamber-0.3.2/tox.ini
```

### Comparing `dpamber-0.3.1/.github/workflows/release.yml` & `dpamber-0.3.2/.github/workflows/release.yml`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
   release:
     name: Release to pypi
     runs-on: ubuntu-latest
     permissions:
         # IMPORTANT: this permission is mandatory for trusted publishing
         id-token: write
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Setup python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: 3.x
         architecture: x64
     - name: Install dependencies
       run: python -m pip install build
     - run: python -m build
     - name: Publish a Python distribution to PyPI
```

### Comparing `dpamber-0.3.1/.gitignore` & `dpamber-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dpamber-0.3.1/.pre-commit-config.yaml` & `dpamber-0.3.2/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -21,10 +21,10 @@
       args: ["--fix"]
 -   repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
     -   id: black-jupyter
 # Python inside docs
 -   repo: https://github.com/asottile/blacken-docs
-    rev: 1.13.0
+    rev: 1.14.0
     hooks:
     -   id: blacken-docs
```

### Comparing `dpamber-0.3.1/PKG-INFO` & `dpamber-0.3.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpamber
-Version: 0.3.1
+Version: 0.3.2
 Summary: Some useful tools related to Amber and DP.
 Project-URL: Homepage, https://github.com/njzjz/dpamber
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
@@ -49,16 +49,16 @@
 ```sh
 dpamber corr --cutoff 6. --qm_region ":1" --parm7_file some_param.param7 --nc some_coord.nc --hl high_level --ll low_level --out dataset
 ```
 where `--cutoff` takes cutoff radius of the QM/MM interaction for training. `--qm_region` takes AMBER mask format for the QM region. `--parm7_file` and `--nc` take the PARM7 file and the trajectory (NetCDF) file, respectively. `--ll` and `--hl` are the prefixes of low-level and high-level files, including the mdout file (`.mdout`), the mden file (`.mden`) and the mdfrc file (`.mdfrc`). The output dataset directory should be put in `--out`.
 
 See details from `dpamber corr -h`.
 
-### model-devi: calculate model deviation
+### devi: calculate model deviation
 
-`model-devi` can be used to calculate the model deviation of a given trajectory.
+`devi` can be used to calculate the model deviation of a given trajectory.
 You need to install DeePMD-kit using
 ```sh
 pip install dpamber[dpgpu]
 ```
 
-See `dpamber model-devi -h` for details.
+See `dpamber devi -h` for details.
```

### Comparing `dpamber-0.3.1/README.md` & `dpamber-0.3.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -36,16 +36,16 @@
 ```sh
 dpamber corr --cutoff 6. --qm_region ":1" --parm7_file some_param.param7 --nc some_coord.nc --hl high_level --ll low_level --out dataset
 ```
 where `--cutoff` takes cutoff radius of the QM/MM interaction for training. `--qm_region` takes AMBER mask format for the QM region. `--parm7_file` and `--nc` take the PARM7 file and the trajectory (NetCDF) file, respectively. `--ll` and `--hl` are the prefixes of low-level and high-level files, including the mdout file (`.mdout`), the mden file (`.mden`) and the mdfrc file (`.mdfrc`). The output dataset directory should be put in `--out`.
 
 See details from `dpamber corr -h`.
 
-### model-devi: calculate model deviation
+### devi: calculate model deviation
 
-`model-devi` can be used to calculate the model deviation of a given trajectory.
+`devi` can be used to calculate the model deviation of a given trajectory.
 You need to install DeePMD-kit using
 ```sh
 pip install dpamber[dpgpu]
 ```
 
-See `dpamber model-devi -h` for details.
+See `dpamber devi -h` for details.
```

### Comparing `dpamber-0.3.1/dpamber/cli.py` & `dpamber-0.3.2/dpamber/cli.py`

 * *Files identical despite different names*

### Comparing `dpamber-0.3.1/dpamber/corr.py` & `dpamber-0.3.2/dpamber/corr.py`

 * *Files identical despite different names*

### Comparing `dpamber-0.3.1/dpamber/model_devi.py` & `dpamber-0.3.2/dpamber/model_devi.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,16 @@
     else:
         interactwith = qm_region
 
     stds = []
     for ii, ss in enumerate(tqdm(sy)):
         ms = ss.pick_by_amber_mask(parm7, interactwith, pass_coords=True)
         ss = list(ms.systems.values())[0]
-        ss = ss.remove_atom_names("EP")
+        if "EP" in ss["atom_names"]:
+            ss = ss.remove_atom_names("EP")
         devi = calc_model_devi(ss["coords"], ss["cells"], ss["atom_types"], dps)
         devi[0, 0] = ii
         stds.append(devi)
     stds = np.concatenate(stds)
     np.savetxt(
         "model_devi.out",
         stds,
```

### Comparing `dpamber-0.3.1/dpamber/qmbuffer.py` & `dpamber-0.3.2/dpamber/qmbuffer.py`

 * *Files identical despite different names*

### Comparing `dpamber-0.3.1/dpamber/qmwater_corr.py` & `dpamber-0.3.2/dpamber/qmwater_corr.py`

 * *Files identical despite different names*

### Comparing `dpamber-0.3.1/dpamber/read_amber.py` & `dpamber-0.3.2/dpamber/read_amber.py`

 * *Files identical despite different names*

### Comparing `dpamber-0.3.1/dpamber/utils.py` & `dpamber-0.3.2/dpamber/utils.py`

 * *Files identical despite different names*

### Comparing `dpamber-0.3.1/dpamber.egg-info/PKG-INFO` & `dpamber-0.3.2/dpamber.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpamber
-Version: 0.3.1
+Version: 0.3.2
 Summary: Some useful tools related to Amber and DP.
 Project-URL: Homepage, https://github.com/njzjz/dpamber
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
@@ -49,16 +49,16 @@
 ```sh
 dpamber corr --cutoff 6. --qm_region ":1" --parm7_file some_param.param7 --nc some_coord.nc --hl high_level --ll low_level --out dataset
 ```
 where `--cutoff` takes cutoff radius of the QM/MM interaction for training. `--qm_region` takes AMBER mask format for the QM region. `--parm7_file` and `--nc` take the PARM7 file and the trajectory (NetCDF) file, respectively. `--ll` and `--hl` are the prefixes of low-level and high-level files, including the mdout file (`.mdout`), the mden file (`.mden`) and the mdfrc file (`.mdfrc`). The output dataset directory should be put in `--out`.
 
 See details from `dpamber corr -h`.
 
-### model-devi: calculate model deviation
+### devi: calculate model deviation
 
-`model-devi` can be used to calculate the model deviation of a given trajectory.
+`devi` can be used to calculate the model deviation of a given trajectory.
 You need to install DeePMD-kit using
 ```sh
 pip install dpamber[dpgpu]
 ```
 
-See `dpamber model-devi -h` for details.
+See `dpamber devi -h` for details.
```

### Comparing `dpamber-0.3.1/dpamber.egg-info/SOURCES.txt` & `dpamber-0.3.2/dpamber.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dpamber-0.3.1/pyproject.toml` & `dpamber-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dpamber-0.3.1/tests/corr/dataset/C6H11HW168O6OW83P1/coord.raw` & `dpamber-0.3.2/tests/corr/dataset/C6H11HW168O6OW83P1/coord.raw`

 * *Files identical despite different names*

### Comparing `dpamber-0.3.1/tests/corr/dataset/C6H11HW168O6OW83P1/force.raw` & `dpamber-0.3.2/tests/corr/dataset/C6H11HW168O6OW83P1/force.raw`

 * *Files identical despite different names*

### Comparing `dpamber-0.3.1/tests/corr/high_level.mdfrc` & `dpamber-0.3.2/tests/corr/high_level.mdfrc`

 * *Files identical despite different names*

### Comparing `dpamber-0.3.1/tests/corr/high_level.mdout` & `dpamber-0.3.2/tests/corr/high_level.mdout`

 * *Files identical despite different names*

### Comparing `dpamber-0.3.1/tests/corr/low_level.mdfrc` & `dpamber-0.3.2/tests/corr/low_level.mdfrc`

 * *Files identical despite different names*

### Comparing `dpamber-0.3.1/tests/corr/low_level.mdout` & `dpamber-0.3.2/tests/corr/low_level.mdout`

 * *Files identical despite different names*

### Comparing `dpamber-0.3.1/tests/corr/qmmm.parm7` & `dpamber-0.3.2/tests/corr/qmmm.parm7`

 * *Files identical despite different names*

### Comparing `dpamber-0.3.1/tests/corr/rc.nc` & `dpamber-0.3.2/tests/corr/rc.nc`

 * *Files identical despite different names*

### Comparing `dpamber-0.3.1/tests/md/md.mdout` & `dpamber-0.3.2/tests/md/md.mdout`

 * *Files identical despite different names*

### Comparing `dpamber-0.3.1/tests/test_corr.py` & `dpamber-0.3.2/tests/test_corr.py`

 * *Files identical despite different names*

### Comparing `dpamber-0.3.1/tests/test_model_devi.py` & `dpamber-0.3.2/tests/test_model_devi.py`

 * *Files identical despite different names*

### Comparing `dpamber-0.3.1/tests/uncoverage/uncoverage.mdout` & `dpamber-0.3.2/tests/uncoverage/uncoverage.mdout`

 * *Files identical despite different names*

