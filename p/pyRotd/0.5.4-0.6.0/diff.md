# Comparing `tmp/pyrotd-0.5.4.tar.gz` & `tmp/pyRotd-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyrotd-0.5.4.tar", last modified: Fri Jul 27 23:39:42 2018, max compression
+gzip compressed data, was "pyRotd-0.6.0.tar", last modified: Tue Jun 20 04:56:50 2023, max compression
```

## Comparing `pyrotd-0.5.4.tar` & `pyRotd-0.6.0.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-07-27 23:39:42.000000 pyrotd-0.5.4/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2694 2018-07-27 23:37:27.000000 pyrotd-0.5.4/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1139 2018-07-27 23:37:27.000000 pyrotd-0.5.4/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1032 2018-07-27 23:37:27.000000 pyrotd-0.5.4/HISTORY.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-07-27 23:39:42.000000 pyrotd-0.5.4/pyrotd.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)       13 2018-07-27 23:39:41.000000 pyrotd-0.5.4/pyrotd.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       17 2018-07-27 23:39:41.000000 pyrotd-0.5.4/pyrotd.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     5517 2018-07-27 23:39:41.000000 pyrotd-0.5.4/pyrotd.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2018-07-27 23:39:41.000000 pyrotd-0.5.4/pyrotd.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      301 2018-07-27 23:39:41.000000 pyrotd-0.5.4/pyrotd.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      324 2018-07-27 23:39:42.000000 pyrotd-0.5.4/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-07-27 23:39:42.000000 pyrotd-0.5.4/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1765 2018-07-27 23:37:27.000000 pyrotd-0.5.4/tests/test_osc_resp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-07-27 23:37:27.000000 pyrotd-0.5.4/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3845 2018-07-27 23:37:27.000000 pyrotd-0.5.4/tests/test_spectra.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       62 2018-07-27 23:37:27.000000 pyrotd-0.5.4/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       80 2018-07-27 23:37:27.000000 pyrotd-0.5.4/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     5517 2018-07-27 23:39:42.000000 pyrotd-0.5.4/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-07-27 23:39:42.000000 pyrotd-0.5.4/pyrotd/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11347 2018-07-27 23:37:27.000000 pyrotd-0.5.4/pyrotd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:56:50.905299 pyRotd-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-20 04:56:39.000000 pyRotd-0.6.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-20 04:56:39.000000 pyRotd-0.6.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-20 04:56:39.000000 pyRotd-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-20 04:56:39.000000 pyRotd-0.6.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-20 04:56:39.000000 pyRotd-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-06-20 04:56:50.905299 pyRotd-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-20 04:56:39.000000 pyRotd-0.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:56:50.905299 pyRotd-0.6.0/pyRotd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-06-20 04:56:50.000000 pyRotd-0.6.0/pyRotd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-20 04:56:50.000000 pyRotd-0.6.0/pyRotd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 04:56:50.000000 pyRotd-0.6.0/pyRotd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-20 04:56:50.000000 pyRotd-0.6.0/pyRotd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 04:56:50.000000 pyRotd-0.6.0/pyRotd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:56:50.905299 pyRotd-0.6.0/pyrotd/
+-rw-r--r--   0 runner    (1001) docker     (123)    15385 2023-06-20 04:56:39.000000 pyRotd-0.6.0/pyrotd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-20 04:56:39.000000 pyRotd-0.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-20 04:56:50.905299 pyRotd-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-20 04:56:39.000000 pyRotd-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:56:50.905299 pyRotd-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 04:56:39.000000 pyRotd-0.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-20 04:56:39.000000 pyRotd-0.6.0/tests/test_osc_resp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-06-20 04:56:39.000000 pyRotd-0.6.0/tests/test_spectra.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyrotd-0.5.4/README.rst` & `pyRotd-0.6.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,14 @@
+pyRotd
 ======
-pyrotd
-======
-
-.. image:: https://img.shields.io/pypi/v/pyrotd.svg
-    :target: https://pypi.python.org/pypi/pyrotd
-    :alt: PyPi Cheese Shop
-
-.. image:: https://img.shields.io/travis/arkottke/pyrotd.svg
-    :target: https://travis-ci.org/arkottke/pyrotd
-    :alt: Build Status
-
-.. image:: https://readthedocs.org/projects/pyrotd/badge/?version=latest&style=flat
-    :target: https://pyrotd.readthedocs.org
-    :alt: Documentation Status
-
-.. image:: https://coveralls.io/repos/github/arkottke/pyrotd/badge.svg?branch=master
-    :target: https://coveralls.io/github/arkottke/pyrotd?branch=master
-    :alt: Test Coverage
-
-.. image:: https://img.shields.io/badge/license-MIT-blue.svg
-    :target: https://github.com/arkottke/pyrotd/blob/master/LICENSE
-    :alt: License
 
-.. image:: https://zenodo.org/badge/2800441.svg
-    :target: https://zenodo.org/badge/latestdoi/2800441
+|PyPi Cheese Shop| |Documentation| |Build Status| |Code Quality| |Test Coverage| |License| |DOI|
 
 Acceleration response spectrum calculations implemented in Python.
 
-* Free software: MIT license
-* Documentation: https://pyrotd.readthedocs.org.
-
 Introduction
 ------------
 
 Simple Python functions for calculating psuedo-spectral acceleration and
 rotated psuedo-spectral acceleration. The response of the
 single-degree-of-freedom oscillator is computed in the frequency domain along
 with frequency-domain interpolation to accurately capture the high-frequency
@@ -69,8 +44,30 @@
 Rotated spectral accelerations may be computed for a pair of time series::
 
     rot_osc_resps = pyrotd.calc_rotated_spec_accels(
         time_step, accels_a, accels_b, osc_freqs, osc_damping)
 
 A more detailed example is in `this`_ Jupyter Notebook.
 
-.. _this: https://github.com/arkottke/pyrotd/blob/master/example.ipynb
+.. _this: https://github.com/arkottke/pyrotd/blob/master/examples/example-2.ipynb
+
+Citation
+--------
+
+Please cite this software using the DOI_.
+
+.. _DOI: https://zenodo.org/badge/latestdoi/2800441
+
+.. |PyPi Cheese Shop| image:: https://img.shields.io/pypi/v/pyrotd.svg
+   :target: https://img.shields.io/pypi/v/pyrotd.svg
+.. |Documentation| image:: https://readthedocs.org/projects/pyrotd/badge/?version=latest
+    :target: https://pyrotd.readthedocs.io/?badge=latest
+.. |Build Status| image:: https://travis-ci.org/arkottke/pyrotd.svg?branch=master
+   :target: https://travis-ci.org/arkottke/pyrotd
+.. |Code Quality| image:: https://api.codacy.com/project/badge/Grade/d449720a4b92474da6b18e040d6729f5    
+   :target: https://www.codacy.com/manual/arkottke/pyrotd
+.. |Test Coverage| image:: https://api.codacy.com/project/badge/Coverage/d449720a4b92474da6b18e040d6729f5    
+   :target: https://www.codacy.com/manual/arkottke/pyrotd
+.. |License| image:: https://img.shields.io/badge/license-MIT-blue.svg
+.. |DOI| image:: https://zenodo.org/badge/2800441.svg
+   :target: https://zenodo.org/badge/latestdoi/2800441
+
```

### Comparing `pyrotd-0.5.4/HISTORY.rst` & `pyRotd-0.6.0/HISTORY.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 History
 =======
 
+0.6.0 (2023-06-19)
+------------------
+- Added optimization based on Stewart et al. (2017) algorithm
+- Added support for computing rotated PGA, PGV, and PGD
+
 0.5.4 (2018-07-27)
 ------------------
 - Added MANIFEST.in
 
 0.5.3 (2018-07-27)
 ------------------
 - Fix packaging issues
```

### Comparing `pyrotd-0.5.4/tests/test_osc_resp.py` & `pyRotd-0.6.0/tests/test_osc_resp.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,74 +1,77 @@
 """Test oscillator response calculation."""
-
 import numpy as np
 import pytest
 
 import pyrotd
-
 from .test_spectra import load_at2
 
 osc_freq = 10
 
 
 def calc_oscillator_resp(motion, osc_damping, resp):
     return pyrotd.calc_oscillator_resp(
-        motion['freqs'],
-        motion['fourier_amps'],
+        motion["freqs"],
+        motion["fourier_amps"],
         osc_damping,
         osc_freq,
         peak_resp_only=True,
-        osc_type=resp)
+        osc_type=resp,
+    )
 
 
 @pytest.fixture
 def motion():
-    time_step, accels = load_at2('RSN8883_14383980_13849090.AT2')
+    time_step, accels = load_at2("RSN8883_14383980_13849090.AT2")
     fourier_amps = np.fft.rfft(accels)
-    freqs = np.linspace(0, 1. / (2 * time_step), num=fourier_amps.size)
+    freqs = np.linspace(0, 1.0 / (2 * time_step), num=fourier_amps.size)
 
     return {
-        'time_step': time_step,
-        'accels': accels,
-        'freqs': freqs,
-        'fourier_amps': fourier_amps,
+        "time_step": time_step,
+        "accels": accels,
+        "freqs": freqs,
+        "fourier_amps": fourier_amps,
     }
 
 
-@pytest.mark.parametrize('resp,power', [
-    ('sa', 0),
-    ('psv', 1),
-    ('sv', 1),
-    ('sd', 2),
-])
+@pytest.mark.parametrize(
+    "resp,power",
+    [
+        ("sa", 0),
+        ("psv", 1),
+        ("sv", 1),
+        ("sd", 2),
+    ],
+)
 def test_osc_resp(motion, resp, power):
     # For very light damping everything should be the same
     osc_damping = 0.005
 
-    ref_psa = calc_oscillator_resp(motion, osc_damping, 'psa')
+    ref_psa = calc_oscillator_resp(motion, osc_damping, "psa")
 
     calc_resp = pyrotd.calc_oscillator_resp(
-        motion['freqs'],
-        motion['fourier_amps'],
+        motion["freqs"],
+        motion["fourier_amps"],
         osc_damping,
         osc_freq,
         peak_resp_only=True,
-        osc_type=resp)
+        osc_type=resp,
+    )
     # Convert to PSA
-    calc_psa = calc_resp * (2 * np.pi * osc_freq)**power
-    np.testing.assert_allclose(calc_psa, ref_psa, rtol=1E-1)
+    calc_psa = calc_resp * (2 * np.pi * osc_freq) ** power
+    np.testing.assert_allclose(calc_psa, ref_psa, rtol=1e-1)
 
 
 @pytest.mark.xfail(strict=True)
 def test_sa(motion):
     osc_damping = 0.010
-    ref_psa = calc_oscillator_resp(motion, osc_damping, 'psa')
+    ref_psa = calc_oscillator_resp(motion, osc_damping, "psa")
 
     calc_psa = pyrotd.calc_oscillator_resp(
-        motion['freqs'],
-        motion['fourier_amps'],
+        motion["freqs"],
+        motion["fourier_amps"],
         osc_damping,
         osc_freq,
         peak_resp_only=True,
-        osc_type='sa',
+        osc_type="sa",
     )
-    np.testing.assert_allclose(calc_psa, ref_psa, rtol=1E-2)
+    np.testing.assert_allclose(calc_psa, ref_psa, rtol=1e-2)
```

### Comparing `pyrotd-0.5.4/tests/test_spectra.py` & `pyRotd-0.6.0/tests/test_spectra.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,124 +1,161 @@
 import gzip
 import json
 import os
 
+import matplotlib
 import numpy as np
 import pytest
 
 import pyrotd
 
-import matplotlib
-matplotlib.use('Agg')
+matplotlib.use("Agg")
 import matplotlib.pyplot as plt  # NOQA
 
 # Need to disable multiprocessing for pytest
 pyrotd.processes = 1
 
 
 def get_relpath(fname):
     """Path relative to tests"""
     return os.path.join(os.path.dirname(__file__), fname)
 
 
-with gzip.open(get_relpath('data/peer_nga_west2.json.gz')) as fp:
+with gzip.open(get_relpath("data/peer_nga_west2.json.gz")) as fp:
     records = json.load(fp)
 
 
 def load_at2(fname):
-    fpath = get_relpath('data/' + fname)
+    fpath = get_relpath("data/" + fname)
     with open(fpath) as fp:
         for _ in range(3):
             next(fp)
         line = next(fp)
         # count = int(line[5:12])
         time_step = float(line[17:25])
-        accels = np.array([p for l in fp for p in l.split()]).astype(float)
+        accels = np.array([part for line in fp for part in line.split()]).astype(float)
     return time_step, accels
 
 
 def iter_single_cases():
     """Iterate single response spectra with a single motion."""
     for record in records:
-        osc_freqs = 1 / np.array(record['period'])
-        time_step, accels_a = load_at2(record['fnames'][0])
-        accels_b = load_at2(record['fnames'][1])[1]
-
-        for spectrum in record['spectra']:
-            osc_damping = spectrum['damping']
-            for key, accels in zip(('h1', 'h2'), (accels_a, accels_b)):
+        osc_freqs = 1 / np.array(record["period"])
+        time_step, accels_a = load_at2(record["fnames"][0])
+        accels_b = load_at2(record["fnames"][1])[1]
+
+        for spectrum in record["spectra"]:
+            osc_damping = spectrum["damping"]
+            for key, accels in zip(("h1", "h2"), (accels_a, accels_b)):
                 if key not in spectrum:
                     continue
 
-                yield ('%s_%s_%d' % (record['rsn'], key,
-                                     100 * osc_damping), osc_damping,
-                       osc_freqs, spectrum[key], time_step, accels)
+                yield (
+                    "%s_%s_%d" % (record["rsn"], key, 100 * osc_damping),
+                    osc_damping,
+                    osc_freqs,
+                    spectrum[key],
+                    time_step,
+                    accels,
+                )
 
 
 def iter_rotated_cases():
     """Iterate rotated spectra with pairs of motions."""
     for record in records:
-        osc_freqs = 1 / np.array(record['period'])
-        time_step, accels_a = load_at2(record['fnames'][0])
-        accels_b = load_at2(record['fnames'][1])[1]
-
-        for spectrum in record['spectra']:
-            osc_damping = spectrum['damping']
-            yield ('%s_%s_%d' % (record['rsn'], 'rotd50',
-                                 100 * osc_damping), osc_damping, osc_freqs,
-                   spectrum['rotd50'], time_step, accels_a, accels_b)
+        osc_freqs = 1 / np.array(record["period"])
+        time_step, accels_a = load_at2(record["fnames"][0])
+        accels_b = load_at2(record["fnames"][1])[1]
+
+        for spectrum in record["spectra"]:
+            osc_damping = spectrum["damping"]
+            yield (
+                "%s_%s_%d" % (record["rsn"], "rotd50", 100 * osc_damping),
+                osc_damping,
+                osc_freqs,
+                spectrum["rotd50"],
+                time_step,
+                accels_a,
+                accels_b,
+            )
 
 
 def plot_comparison(name, osc_freqs, target, computed):
     # Create a plot
     fig = plt.figure()
     ax1 = fig.add_subplot(111)
 
-    ax1.plot(osc_freqs, computed, 'b-', label='Computed')
-    ax1.plot(osc_freqs, target, 'r--', label='Target')
+    ax1.plot(osc_freqs, computed, "b-", label="Computed")
+    ax1.plot(osc_freqs, target, "r--", label="Target")
 
     ax2 = ax1.twinx()
-    rel_diff = 100. * (computed - target) / target
+    rel_diff = 100.0 * (computed - target) / target
     ax2.plot(osc_freqs, rel_diff, linewidth=0.5)
 
-    ax1.set(
-        xscale='log', xlabel='Frequency (Hz)', yscale='log', ylabel='PSA (g)')
-    ax2.set_ylabel('Relative Difference (%)')
+    ax1.set(xscale="log", xlabel="Frequency (Hz)", yscale="log", ylabel="PSA (g)")
+    ax2.set_ylabel("Relative Difference (%)")
     ax1.grid()
     ax1.legend()
     fig.tight_layout()
-    fig.savefig('test-' + name)
+    fig.savefig("test-" + name)
     plt.close(fig)
 
 
 @pytest.mark.parametrize(
-    'name,osc_damping,osc_freqs,target,time_step,accels',
+    "name,osc_damping,osc_freqs,target,time_step,accels",
     iter_single_cases(),
 )
-def test_calc_response_spectrum(name, osc_damping, osc_freqs, target,
-                                time_step, accels):
-    resp_spec = pyrotd.calc_spec_accels(time_step, accels, osc_freqs,
-                                        osc_damping)
+def test_calc_response_spectrum(
+    name, osc_damping, osc_freqs, target, time_step, accels
+):
+    resp_spec = pyrotd.calc_spec_accels(
+        time_step,
+        accels,
+        osc_freqs,
+        osc_damping,
+    )
     computed = resp_spec.spec_accel
     if plt:
         plot_comparison(name, osc_freqs, target, computed)
     np.testing.assert_allclose(target, computed, rtol=0.05)
 
 
 @pytest.mark.parametrize(
-    'name,osc_damping,osc_freqs,target,time_step,accels_a,accels_b',
+    "name,osc_damping,osc_freqs,target,time_step,accels_a,accels_b",
     iter_rotated_cases(),
 )
-def test_calc_rotated_response_spectrum(name, osc_damping, osc_freqs, target,
-                                        time_step, accels_a, accels_b):
+@pytest.mark.parametrize("method", ["rigorous", "optimized"])
+def test_calc_rotated_response_spectrum(
+    name, osc_damping, osc_freqs, target, time_step, accels_a, accels_b, method
+):
     # Compute the rotated spectra
     rotated = pyrotd.calc_rotated_spec_accels(
         time_step,
         accels_a,
         accels_b,
         osc_freqs,
         osc_damping,
-        percentiles=[50])
+        percentiles=[50],
+        method=method,
+    )
     computed = rotated.spec_accel
     if plt:
-        plot_comparison(name, osc_freqs, target, computed)
+        plot_comparison(f"{name}-{method}", osc_freqs, target, computed)
     np.testing.assert_allclose(target, computed, rtol=0.10)
+
+
+@pytest.mark.parametrize("peak_type", ["pga", "pgv", "pgd"])
+def test_calc_rotated_peaks(peak_type):
+    fnames = ["RSN8883_14383980_13849090.AT2", "RSN8883_14383980_13849360.AT2"]
+    time_step, accels_a = load_at2(fnames[0])
+    _, accels_b = load_at2(fnames[1])
+
+    # Compute the rotated spectra
+    rotated = pyrotd.calc_rotated_peaks(
+        time_step,
+        accels_a,
+        accels_b,
+        peak_type=peak_type,
+        percentiles=[0, 10, 50, 90, 100],
+        method="optimized",
+    )
+    print(rotated)
```

### Comparing `pyrotd-0.5.4/pyrotd/__init__.py` & `pyRotd-0.6.0/pyrotd/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 #!/usr/bin/python
-
 import sys
 
 import numpy as np
-
 from pkg_resources import get_distribution
 
 if sys.version_info >= (3, 6):
     import functools
     import multiprocessing
+
     processes = max(multiprocessing.cpu_count() - 1, 1)
 else:
     processes = 1
 
-__author__ = 'Albert Kottke'
-__copyright__ = 'Copyright 2016-18 Albert Kottke'
-__license__ = 'MIT'
-__title__ = 'pyrotd'
-__version__ = get_distribution('pyrotd').version
-
-
-def calc_oscillator_resp(freq,
-                         fourier_amp,
-                         osc_damping,
-                         osc_freq,
-                         max_freq_ratio=5.,
-                         peak_resp_only=False,
-                         osc_type='psa'):
+__author__ = "Albert Kottke"
+__copyright__ = "Copyright 2016-18 Albert Kottke"
+__license__ = "MIT"
+__title__ = "pyrotd"
+__version__ = get_distribution("pyrotd").version
+
+G_TO_CMPS = 980.665
+
+
+def calc_oscillator_resp(
+    freq,
+    fourier_amp,
+    osc_damping,
+    osc_freq,
+    max_freq_ratio=5.0,
+    peak_resp_only=False,
+    osc_type="psa",
+):
     """Compute the time series response of an oscillator.
 
     Parameters
     ----------
     freq : array_like
         frequency of the Fourier acceleration spectrum [Hz]
     fourier_amp : array_like
@@ -57,25 +60,28 @@
     response : :class:`numpy.ndarray` or float
         time series response of the oscillator
     """
     ang_freq = 2 * np.pi * freq
     osc_ang_freq = 2 * np.pi * osc_freq
 
     # Single-degree of freedom transfer function
-    h = (1 / (ang_freq**2. - osc_ang_freq**2 -
-              2.j * osc_damping * osc_ang_freq * ang_freq))
-    if osc_type == 'sd':
+    h = 1 / (
+        ang_freq**2.0
+        - osc_ang_freq**2
+        - 2.0j * osc_damping * osc_ang_freq * ang_freq
+    )
+    if osc_type == "sd":
         pass
-    elif osc_type == 'sv':
-        h *= 1.j * ang_freq
-    elif osc_type == 'sa':
-        h *= -(ang_freq**2)
-    elif osc_type == 'psa':
+    elif osc_type == "sv":
+        h *= 1.0j * ang_freq
+    elif osc_type == "sa":
+        h *= 1 + (1.0j * ang_freq) ** 2
+    elif osc_type == "psa":
         h *= -(osc_ang_freq**2)
-    elif osc_type == 'psv':
+    elif osc_type == "psv":
         h *= -osc_ang_freq
     else:
         raise RuntimeError
 
     # Adjust the maximum frequency considered. The maximum frequency is 5
     # times the oscillator frequency. This provides that at the oscillator
     # frequency there are at least tenth samples per wavelength.
@@ -89,69 +95,89 @@
 
     if peak_resp_only:
         resp = np.abs(resp).max()
 
     return resp
 
 
-def calc_rotated_percentiles(accels, angles, percentiles=None):
+def calc_rotated_percentiles(accels, angles, percentiles=None, method="optimized"):
     """Compute the response spectrum for a time series.
 
+    This function computes the period-dependent rotated percentiles. If `optimized` is
+    *True*, then the percentiles are only computed at times greater than a threshold.
+    This optimized procedure is described in Equations 2.4 and 2.5 of Stewart et al.
+    (2017) PEER report [1]_.
+
+    .. _[1]: https://peer.berkeley.edu/sites/default/files/2017_09_stewart_9.10.18.pdf
+
     Parameters
     ----------
     accels : list of array_like
         pair of acceleration time series
     angles : array_like
         angles to which to compute the rotated time series
     percentiles : array_like or None
         percentiles to return
+    method : str, default of `optimized`
+        If `optimized`, then the rotation is done on a subset of values. If `rigorous`,
+        then all values are considered.
 
     Returns
     -------
     rotated_resp : :class:`np.recarray`
         Percentiles of the rotated response. Records have keys:
         'percentile', 'spec_accel', and 'angle'.
     """
     accels = np.asarray(accels)
-    percentiles = np.array([0, 50, 100]) \
-        if percentiles is None else np.asarray(percentiles)
-    angles = np.arange(0, 180, step=1) \
-        if angles is None else np.asarray(angles)
+
+    if method == "optimized":
+        # Use a reduced set of accelerations
+        level = 0.7 * np.min(np.max(np.abs(accels), axis=1))
+        vsum = np.sqrt(np.sum(accels**2, axis=0))
+        indices = vsum >= level
+        accels = accels[:, indices]
+
+    percentiles = (
+        np.array([0, 50, 100]) if percentiles is None else np.asarray(percentiles)
+    )
+    angles = np.arange(0, 180, step=1) if angles is None else np.asarray(angles)
 
     # Compute rotated time series
     radians = np.radians(angles)
     coeffs = np.c_[np.cos(radians), np.sin(radians)]
     rotated_time_series = np.dot(coeffs, accels)
     # Sort this array based on the response
     peak_responses = np.abs(rotated_time_series).max(axis=1)
-    rotated = np.rec.fromarrays(
-        [angles, peak_responses], names='angle,peak_resp')
-    rotated.sort(order='peak_resp')
+    rotated = np.rec.fromarrays([angles, peak_responses], names="angle,peak_resp")
+    rotated.sort(order="peak_resp")
     # Get the peak response at the requested percentiles
-    p_peak_resps = np.percentile(
-        rotated.peak_resp, percentiles, interpolation='linear')
+    p_peak_resps = np.percentile(rotated.peak_resp, percentiles, method="linear")
     # Can only return the orientations for the minimum and maximum value as the
     # orientation is not unique (i.e., two values correspond to the 50%
     # percentile).
     p_angles = np.select(
-        [np.isclose(percentiles, 0),
-         np.isclose(percentiles, 100), True],
-        [rotated.angle[0], rotated.angle[-1], np.nan])
+        [np.isclose(percentiles, 0), np.isclose(percentiles, 100), True],
+        [rotated.angle[0], rotated.angle[-1], np.nan],
+    )
     return np.rec.fromarrays(
-        [percentiles, p_peak_resps, p_angles],
-        names='percentile,spec_accel,angle')
+        [percentiles, p_peak_resps, p_angles], names="percentile,spec_accel,angle"
+    )
 
 
-def calc_rotated_oscillator_resp(angles,
-                                 percentiles,
-                                 freqs,
-                                 fourier_amps,
-                                 osc_damping,
-                                 osc_freq,
-                                 max_freq_ratio=5.):
+def calc_rotated_oscillator_resp(
+    angles,
+    percentiles,
+    freqs,
+    fourier_amps,
+    osc_damping,
+    osc_freq,
+    max_freq_ratio=5.0,
+    osc_type="psa",
+    method="optimized",
+):
     """Compute the percentiles of response of a rotated oscillator.
 
     Parameters
     ----------
     percentiles : array_like
         percentiles to return.
     angles : array_like
@@ -166,43 +192,58 @@
         frequency of the oscillator [Hz]
     max_freq_ratio : float, default=5
         minimum required ratio between the oscillator frequency and
         then maximum frequency of the time series. It is recommended that this
         value be 5.
     peak_resp_only : bool, default=False
         If only the peak response is returned.
+    osc_type : str, default='psa'
+        type of response. Options are:
+            'sd': spectral displacement
+            'sv': spectral velocity
+            'sa': spectral acceleration
+            'psv': psuedo-spectral velocity
+            'psa': psuedo-spectral acceleration
+    method : str, default of `optimized`
+        If `optimized`, then the rotation is done on a subset of values. If `rigorous`,
+        then all values are considered.
 
     Returns
     -------
     response : :class:`numpy.ndarray` or float
         time series response of the oscillator
     """
 
     # Compute the oscillator responses
-    osc_ts = np.vstack([
-        calc_oscillator_resp(
-            freqs,
-            fa,
-            osc_damping,
-            osc_freq,
-            max_freq_ratio=max_freq_ratio,
-            peak_resp_only=False) for fa in fourier_amps
-    ])
+    osc_ts = np.vstack(
+        [
+            calc_oscillator_resp(
+                freqs,
+                fa,
+                osc_damping,
+                osc_freq,
+                max_freq_ratio=max_freq_ratio,
+                peak_resp_only=False,
+                osc_type=osc_type,
+            )
+            for fa in fourier_amps
+        ]
+    )
     # Compute the rotated values of the oscillator response
-    rotated_percentiles = calc_rotated_percentiles(osc_ts, angles, percentiles)
+    rotated_percentiles = calc_rotated_percentiles(
+        osc_ts, angles, percentiles, method=method
+    )
 
     # Stack all of the results
-    return [(osc_freq, ) + rp.tolist() for rp in rotated_percentiles]
+    return [(osc_freq,) + rp.tolist() for rp in rotated_percentiles]
 
 
-def calc_spec_accels(time_step,
-                     accel_ts,
-                     osc_freqs,
-                     osc_damping=0.05,
-                     max_freq_ratio=5):
+def calc_spec_accels(
+    time_step, accel_ts, osc_freqs, osc_damping=0.05, max_freq_ratio=5, osc_type="psa"
+):
     """Compute the psuedo-spectral accelerations.
 
     Parameters
     ----------
     time_step : float
         time step of the time series [s]
     accel_ts : array_like
@@ -211,58 +252,75 @@
         natural frequency of the oscillators [Hz]
     osc_damping : float
         damping of the oscillator [decimal]. Default of 0.05 (i.e., 5%)
     max_freq_ratio : float, default=5
         minimum required ratio between the oscillator frequency and
         then maximum frequency of the time series. It is recommended that this
         value be 5.
+    osc_type : str, default='psa'
+        type of response. Options are:
+            'sd': spectral displacement
+            'sv': spectral velocity
+            'sa': spectral acceleration
+            'psv': psuedo-spectral velocity
+            'psa': psuedo-spectral acceleration
 
     Returns
     -------
     resp_spec : :class:`np.recarray`
         computed pseudo-spectral acceleration [g]. Records have keys:
         'osc_freq', and 'spec_accel'
     """
     fourier_amp = np.fft.rfft(accel_ts)
-    freq = np.linspace(0, 1. / (2 * time_step), num=fourier_amp.size)
+    freq = np.linspace(0, 1.0 / (2 * time_step), num=fourier_amp.size)
 
     if processes > 1:
         with multiprocessing.Pool(processes=processes) as pool:
             spec_accels = pool.map(
                 functools.partial(
                     calc_oscillator_resp,
                     freq,
                     fourier_amp,
                     osc_damping,
                     max_freq_ratio=max_freq_ratio,
-                    peak_resp_only=True), osc_freqs)
+                    peak_resp_only=True,
+                    osc_type=osc_type,
+                ),
+                osc_freqs,
+            )
     else:
         # Single process
         spec_accels = [
             calc_oscillator_resp(
                 freq,
                 fourier_amp,
                 osc_damping,
                 of,
                 max_freq_ratio=max_freq_ratio,
-                peak_resp_only=True) for of in osc_freqs
+                peak_resp_only=True,
+                osc_type=osc_type,
+            )
+            for of in osc_freqs
         ]
 
-    return np.rec.fromarrays(
-        [osc_freqs, spec_accels], names='osc_freq,spec_accel')
+    return np.rec.fromarrays([osc_freqs, spec_accels], names="osc_freq,spec_accel")
 
 
-def calc_rotated_spec_accels(time_step,
-                             accel_a,
-                             accel_b,
-                             osc_freqs,
-                             osc_damping=0.05,
-                             percentiles=None,
-                             angles=None,
-                             max_freq_ratio=5):
+def calc_rotated_spec_accels(
+    time_step,
+    accel_a,
+    accel_b,
+    osc_freqs,
+    osc_damping=0.05,
+    percentiles=None,
+    angles=None,
+    max_freq_ratio=5,
+    osc_type="psa",
+    method="optimized",
+):
     """Compute the rotated psuedo-spectral accelerations.
 
     Parameters
     ----------
     time_step : float
         time step of the time series [s]
     accel_a : array_like
@@ -279,53 +337,127 @@
     angles : array_like or None
         angles to which to compute the rotated time series. Default of
         np.arange(0, 180, step=1) (i.e., 0, 1, 2, .., 179).
     max_freq_ratio : float, default=5
         minimum required ratio between the oscillator frequency and
         then maximum frequency of the time series. It is recommended that this
         value be 5.
+    method : str, default of `optimized`
+        If `optimized`, then the rotation is done on a subset of values. If `rigorous`,
+        then all values are considered.
     Returns
     -------
     rotated_resp : :class:`np.recarray`
         computed pseudo-spectral acceleration [g] at each of the percentiles.
         Records have keys: 'osc_freq', 'percentile', 'spec_accel', and 'angle'
     """
-    percentiles = [0, 50, 100] \
-        if percentiles is None else np.asarray(percentiles)
-    angles = np.arange(0, 180, step=1) \
-        if angles is None else np.asarray(angles)
+    percentiles = [0, 50, 100] if percentiles is None else np.asarray(percentiles)
+    angles = np.arange(0, 180, step=1) if angles is None else np.asarray(angles)
 
-    assert len(accel_a) == len(accel_b), 'Time series not equal lengths!'
+    assert len(accel_a) == len(accel_b), "Time series not equal lengths!"
 
     # Compute the Fourier amplitude spectra
     fourier_amps = [np.fft.rfft(accel_a), np.fft.rfft(accel_b)]
-    freqs = np.linspace(0, 1. / (2 * time_step), num=fourier_amps[0].size)
+    freqs = np.linspace(0, 1.0 / (2 * time_step), num=fourier_amps[0].size)
 
     if processes > 1:
         with multiprocessing.Pool(processes=processes) as pool:
             groups = pool.map(
                 functools.partial(
                     calc_rotated_oscillator_resp,
                     angles,
                     percentiles,
                     freqs,
                     fourier_amps,
                     osc_damping,
-                    max_freq_ratio=max_freq_ratio), osc_freqs)
+                    max_freq_ratio=max_freq_ratio,
+                    osc_type=osc_type,
+                    method=method,
+                ),
+                osc_freqs,
+            )
     else:
         # Single process
         groups = [
             calc_rotated_oscillator_resp(
                 angles,
                 percentiles,
                 freqs,
                 fourier_amps,
                 osc_damping,
                 of,
-                max_freq_ratio=max_freq_ratio) for of in osc_freqs
+                max_freq_ratio=max_freq_ratio,
+                osc_type=osc_type,
+                method=method,
+            )
+            for of in osc_freqs
         ]
     records = [g for group in groups for g in group]
 
     # Reorganize the arrays grouping by the percentile
     rotated_resp = np.rec.fromrecords(
-        records, names='osc_freq,percentile,spec_accel,angle')
+        records, names="osc_freq,percentile,spec_accel,angle"
+    )
     return rotated_resp
+
+
+def calc_rotated_peaks(
+    time_step,
+    accel_a,
+    accel_b,
+    peak_type="pga",
+    percentiles=None,
+    angles=None,
+    method="optimized",
+):
+    """Compute the rotated peak values of input accelerations.
+
+    Parameters
+    ----------
+    time_step : float
+        time step of the time series [s]
+    accel_a : array_like
+        acceleration time series of the first motion [g]
+    accel_b : array_like
+        acceleration time series of the second motion that is perpendicular to
+        the first motion [g]
+    peak_type : str
+        Either: pga, pgv, or pgd
+    percentiles : array_like or None
+        percentiles to return. Default of [0, 50, 100],
+    angles : array_like or None
+        angles to which to compute the rotated time series. Default of
+        np.arange(0, 180, step=1) (i.e., 0, 1, 2, .., 179).
+    method : str, default of `optimized`
+        If `optimized`, then the rotation is done on a subset of values. If `rigorous`,
+        then all values are considered.
+    Returns
+    -------
+    rotated_peak : float
+        If `pga`, then the units are in *g*. Otherwise, they are reported in *cm/s* or
+        *cm* for `pgv` or `pgd`, respectively.
+    """
+    percentiles = [0, 50, 100] if percentiles is None else np.asarray(percentiles)
+    angles = np.arange(0, 180, step=1) if angles is None else np.asarray(angles)
+
+    assert len(accel_a) == len(accel_b), "Time series not equal lengths!"
+
+    if peak_type in ["pgv", "pgd"]:
+        # Compute the Fourier amplitude spectra
+        fourier_amps = np.vstack([np.fft.rfft(accel_a), np.fft.rfft(accel_b)])
+        fourier_amps *= G_TO_CMPS
+
+        # Convert to velocity or displacement using Fourier domain integration
+        power = 2 if peak_type == "pgd" else 1
+        freqs = np.linspace(0, 1.0 / (2 * time_step), num=fourier_amps[0].size)
+        fourier_amps[:, 1:] *= (2j * np.pi * freqs[1:]) ** (-power)
+
+        values = [np.fft.irfft(fourier_amps[0, :]), np.fft.irfft(fourier_amps[1, :])]
+    elif peak_type == "pga":
+        values = [accel_a, accel_b]
+    else:
+        raise NotImplementedError
+
+    ret = calc_rotated_percentiles(values, angles, percentiles, method=method)
+    ret.dtype.names = "percentile", peak_type, "angle"
+
+    return ret
```

