# Comparing `tmp/bletl-1.2.2.tar.gz` & `tmp/bletl-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bletl-1.2.2.tar", last modified: Mon Jan 16 16:42:23 2023, max compression
+gzip compressed data, was "bletl-1.3.1.tar", last modified: Tue Jun 20 12:43:55 2023, max compression
```

## Comparing `bletl-1.2.2.tar` & `bletl-1.3.1.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 16:42:23.503602 bletl-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    34452 2023-01-16 16:35:10.000000 bletl-1.2.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-01-16 16:35:10.000000 bletl-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-01-16 16:42:23.503602 bletl-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-01-16 16:35:10.000000 bletl-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 16:42:23.503602 bletl-1.2.2/bletl/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-01-16 16:35:10.000000 bletl-1.2.2/bletl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8703 2023-01-16 16:35:10.000000 bletl-1.2.2/bletl/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    11899 2023-01-16 16:35:10.000000 bletl-1.2.2/bletl/features.py
--rw-r--r--   0 runner    (1001) docker     (123)    18288 2023-01-16 16:35:10.000000 bletl-1.2.2/bletl/growth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-01-16 16:35:10.000000 bletl-1.2.2/bletl/heuristics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 16:42:23.503602 bletl-1.2.2/bletl/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-16 16:35:10.000000 bletl-1.2.2/bletl/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19487 2023-01-16 16:35:10.000000 bletl-1.2.2/bletl/parsing/bl1.py
--rw-r--r--   0 runner    (1001) docker     (123)    19721 2023-01-16 16:35:10.000000 bletl-1.2.2/bletl/parsing/blpro.py
--rw-r--r--   0 runner    (1001) docker     (123)    12337 2023-01-16 16:35:10.000000 bletl-1.2.2/bletl/splines.py
--rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-01-16 16:35:10.000000 bletl-1.2.2/bletl/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-01-16 16:35:10.000000 bletl-1.2.2/bletl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 16:42:23.503602 bletl-1.2.2/bletl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-01-16 16:42:23.000000 bletl-1.2.2/bletl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-01-16 16:42:23.000000 bletl-1.2.2/bletl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-16 16:42:23.000000 bletl-1.2.2/bletl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-16 16:35:14.000000 bletl-1.2.2/bletl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-01-16 16:42:23.000000 bletl-1.2.2/bletl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-16 16:42:23.000000 bletl-1.2.2/bletl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-01-16 16:35:10.000000 bletl-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-16 16:42:23.503602 bletl-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-01-16 16:35:10.000000 bletl-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 16:42:23.503602 bletl-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21930 2023-01-16 16:35:11.000000 bletl-1.2.2/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-01-16 16:35:11.000000 bletl-1.2.2/tests/test_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-01-16 16:35:11.000000 bletl-1.2.2/tests/test_growth.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-01-16 16:35:11.000000 bletl-1.2.2/tests/test_heuristics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9930 2023-01-16 16:35:11.000000 bletl-1.2.2/tests/test_splines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:43:55.626867 bletl-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34452 2023-06-20 12:34:36.000000 bletl-1.3.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-20 12:34:36.000000 bletl-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-06-20 12:43:55.622867 bletl-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-20 12:34:36.000000 bletl-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:43:55.622867 bletl-1.3.1/bletl/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-20 12:34:36.000000 bletl-1.3.1/bletl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9050 2023-06-20 12:34:36.000000 bletl-1.3.1/bletl/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12087 2023-06-20 12:34:36.000000 bletl-1.3.1/bletl/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18573 2023-06-20 12:34:36.000000 bletl-1.3.1/bletl/growth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-06-20 12:34:36.000000 bletl-1.3.1/bletl/heuristics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:43:55.622867 bletl-1.3.1/bletl/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-20 12:34:36.000000 bletl-1.3.1/bletl/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19710 2023-06-20 12:34:36.000000 bletl-1.3.1/bletl/parsing/bl1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21022 2023-06-20 12:34:36.000000 bletl-1.3.1/bletl/parsing/blpro.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 12:34:36.000000 bletl-1.3.1/bletl/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12503 2023-06-20 12:34:36.000000 bletl-1.3.1/bletl/splines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11195 2023-06-20 12:34:36.000000 bletl-1.3.1/bletl/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-06-20 12:34:36.000000 bletl-1.3.1/bletl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:43:55.622867 bletl-1.3.1/bletl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-06-20 12:43:55.000000 bletl-1.3.1/bletl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-20 12:43:55.000000 bletl-1.3.1/bletl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 12:43:55.000000 bletl-1.3.1/bletl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 12:34:44.000000 bletl-1.3.1/bletl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-20 12:43:55.000000 bletl-1.3.1/bletl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 12:43:55.000000 bletl-1.3.1/bletl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-20 12:34:36.000000 bletl-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 12:43:55.626867 bletl-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-20 12:34:36.000000 bletl-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:43:55.622867 bletl-1.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    23946 2023-06-20 12:34:37.000000 bletl-1.3.1/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-20 12:34:37.000000 bletl-1.3.1/tests/test_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-06-20 12:34:37.000000 bletl-1.3.1/tests/test_growth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-20 12:34:37.000000 bletl-1.3.1/tests/test_heuristics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9911 2023-06-20 12:34:37.000000 bletl-1.3.1/tests/test_splines.py
```

### Comparing `bletl-1.2.2/LICENSE.md` & `bletl-1.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bletl-1.2.2/README.md` & `bletl-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `bletl-1.2.2/bletl/__init__.py` & `bletl-1.3.1/bletl/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,8 +15,8 @@
     InvalidLotNumberError,
     LotInformationError,
     LotInformationMismatch,
     LotInformationNotFound,
     NoMeasurementData,
 )
 
-__version__ = "1.2.2"
+__version__ = "1.3.1"
```

### Comparing `bletl-1.2.2/bletl/core.py` & `bletl-1.3.1/bletl/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import pathlib
 import typing
 import urllib.error
 import urllib.request
 import warnings
 from collections.abc import Iterable
-from typing import Optional, Union
+from typing import Optional, Sequence, Union
 
 import numpy
 import pandas
 
 from . import parsing, utils
 from .types import (
     BioLectorModel,
@@ -88,22 +88,22 @@
     parser_cls = parsers[(model, version)]
     return parser_cls()
 
 
 def _parse(
     filepath: str,
     drop_incomplete_cycles: bool,
-    lot_number: int,
-    temp: int,
-    cal_0: float = None,
-    cal_100: float = None,
-    phi_min: float = None,
-    phi_max: float = None,
-    pH_0: float = None,
-    dpH: float = None,
+    lot_number: Optional[int],
+    temp: Optional[int],
+    cal_0: Optional[float] = None,
+    cal_100: Optional[float] = None,
+    phi_min: Optional[float] = None,
+    phi_max: Optional[float] = None,
+    pH_0: Optional[float] = None,
+    dpH: Optional[float] = None,
 ) -> BLData:
     """Parses a raw BioLector CSV file into a BLData object.
 
     Parameters
     ----------
     filepath : str or pathlib.Path
         Path pointing to the file of interest.
@@ -134,37 +134,47 @@
 
     Raises
     ------
     NotImlementedError
         When the file contents do not match with a known BioLector result file format.
     """
     parser = get_parser(filepath)
-    data = parser.parse(filepath, lot_number, temp, cal_0, cal_100, phi_min, phi_max, pH_0, dpH)
+    data = parser.parse(
+        filepath,
+        lot_number=lot_number,
+        temp=temp,
+        cal_0=cal_0,
+        cal_100=cal_100,
+        phi_min=phi_min,
+        phi_max=phi_max,
+        pH_0=pH_0,
+        dpH=dpH,
+    )
 
     if (not data.measurements.empty) and drop_incomplete_cycles:
         index_names, measurements = utils._unindex(data.measurements)
         latest_full_cycle = utils._last_full_cycle(measurements)
         measurements = measurements[measurements.cycle <= latest_full_cycle]
-        data._measurements = utils._reindex(measurements, index_names)
+        data._measurements = utils._reindex(measurements, index_names)  # type: ignore
 
     return data
 
 
 def parse(
-    filepaths,
+    filepaths: Union[str, Sequence[str]],
     *,
     drop_incomplete_cycles: bool = True,
-    lot_number: int = None,
-    temp: int = None,
-    cal_0: float = None,
-    cal_100: float = None,
-    phi_min: float = None,
-    phi_max: float = None,
-    pH_0: float = None,
-    dpH: float = None,
+    lot_number: Optional[int] = None,
+    temp: Optional[int] = None,
+    cal_0: Optional[float] = None,
+    cal_100: Optional[float] = None,
+    phi_min: Optional[float] = None,
+    phi_max: Optional[float] = None,
+    pH_0: Optional[float] = None,
+    dpH: Optional[float] = None,
 ) -> BLData:
     """Parses a raw BioLector CSV file into a BLData object and applies calibration.
 
     Parameters
     ----------
     filepaths : str or pathlib.Path or iterable
         Path pointing to the file(s) of interest.
```

### Comparing `bletl-1.2.2/bletl/features.py` & `bletl-1.3.1/bletl/features.py`

 * *Files 5% similar despite different names*

```diff
@@ -425,11 +425,14 @@
     for fs, ts_extractor in ts_extractors.items():
         data = pandas.DataFrame(columns=["id", "time", "x"])
         data["id"] = narrow["well"]
         data["time"] = narrow["time"]
         data["x"] = narrow[fs]
         _log.info("Applying tsfresh extractor to %s\n", fs)
         df_fs = ts_extractor._extract(data)
-        for i, mname in enumerate(df_fs.columns):
-            df_result[f"{fs}_{mname}"] = df_fs.to_numpy()[:, i]
+        # Rename columns to include the filterset name
+        df_fs.columns = [f"{fs}_{col}" for col in df_fs.columns]
+        # Add columns with new features for this filterset to the result
+        df_fs.index = [i for i in df_fs.index]
+        df_result = pandas.concat([df_result, df_fs], axis=1)
     _log.info("Extraction finished in: %s minutes", round((time.time() - s_time) / 60, ndigits=1))
     return df_result
```

### Comparing `bletl-1.2.2/bletl/growth.py` & `bletl-1.3.1/bletl/growth.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 import logging
 import typing
+from typing import Dict, Optional, Sequence, Tuple, Union
 
 import arviz
 import calibr8
 import numpy
 import pymc as pm
 from packaging import version
 
 try:
     import pytensor.tensor as pt
 except ModuleNotFoundError:
-    import aesara.tensor as pt
+    import aesara.tensor as pt  # type: ignore
 
 
 _log = logging.getLogger(__file__)
 
 
 class GrowthRateResult:
     """Represents the result of applying the µ(t) model to one dataset."""
 
     def __init__(
         self,
         *,
-        t_data: numpy.ndarray,
-        t_segments: numpy.ndarray,
-        y: numpy.ndarray,
+        t_data: Union[Sequence[float], numpy.ndarray],
+        t_segments: Union[Sequence[float], numpy.ndarray],
+        y: Union[Sequence[float], numpy.ndarray],
         calibration_model: calibr8.CalibrationModel,
-        switchpoints: typing.Dict[float, str],
+        switchpoints: Dict[float, str],
         pmodel: pm.Model,
-        theta_map: dict,
+        theta_map: Dict[str, numpy.ndarray],
     ):
         """Creates a result object of a growth rate analysis.
 
         Parameters
         ----------
         t_data : numpy.ndarray
             time vector of data timepoints
@@ -43,17 +44,17 @@
         switchpoints : dict
             maps switchpoint times to labels
         pmodel : pymc.Model
             the PyMC model underlying the analysis
         theta_map : dict
             the PyMC MAP estimate
         """
-        self._t_data = t_data
-        self._t_segments = t_segments
-        self._y = y
+        self._t_data = numpy.asarray(t_data)
+        self._t_segments = numpy.asarray(t_segments)
+        self._y = numpy.asarray(y)
         self._switchpoints = switchpoints
         self.calibration_model = calibration_model
         self._pmodel = pmodel
         self._theta_map = theta_map
         self._idata = None
         super().__init__()
 
@@ -69,66 +70,68 @@
 
     @property
     def y(self) -> numpy.ndarray:
         """Vector of backscatter observations."""
         return self._y
 
     @property
-    def switchpoints(self) -> typing.Dict[float, str]:
+    def switchpoints(self) -> Dict[float, str]:
         """Dictionary (by time) of known and detected switchpoints."""
         return self._switchpoints
 
     @property
-    def known_switchpoints(self) -> typing.Tuple[float]:
+    def known_switchpoints(self) -> Tuple[float, ...]:
         """Time values of previously known switchpoints in the model."""
         return tuple(t for t, label in self.switchpoints.items() if label != "detected")
 
     @property
-    def detected_switchpoints(self) -> typing.Tuple[float]:
+    def detected_switchpoints(self) -> Tuple[float, ...]:
         """Time values of switchpoints that were autodetected from the fit."""
         return tuple(t for t, label in self.switchpoints.items() if label == "detected")
 
     @property
     def pmodel(self) -> pm.Model:
         """The PyMC model underlying this analysis."""
         return self._pmodel
 
     @property
-    def theta_map(self) -> dict:
+    def theta_map(self) -> Dict[str, numpy.ndarray]:
         """MAP estimate of the model parameters."""
         return self._theta_map
 
     @property
-    def idata(self) -> typing.Optional[arviz.InferenceData]:
+    def idata(self) -> Optional[arviz.InferenceData]:
         """ArviZ InferenceData object of the MCMC trace."""
         return self._idata
 
     @property
     def mu_map(self) -> numpy.ndarray:
         """MAP estimate of the growth rates in segments between data points."""
         return self.theta_map["mu_t"]
 
     @property
     def x_map(self) -> numpy.ndarray:
         """MAP estimate of the biomass curve."""
         return self.theta_map["X"]
 
     @property
-    def mu_mcmc(self) -> typing.Optional[numpy.ndarray]:
+    def mu_mcmc(self) -> Optional[numpy.ndarray]:
         """Posterior samples of growth rates in segments between data points."""
         if not self.idata:
             return None
+        assert hasattr(self.idata, "posterior")
         return self.idata.posterior.mu_t.stack(sample=("chain", "draw")).values.T
 
     @property
-    def x_mcmc(self) -> typing.Optional[numpy.ndarray]:
+    def x_mcmc(self) -> Optional[numpy.ndarray]:
         """Posterior samples of biomass curve."""
-        if not self.idata:
+        if self.idata is None:
             return None
-        return self._idata.posterior["X"].stack(sample=("chain", "draw")).T
+        assert hasattr(self.idata, "posterior")
+        return self.idata.posterior["X"].stack(sample=("chain", "draw")).T
 
     def sample(self, **kwargs) -> None:
         """Runs MCMC sampling with default settings on the growth model.
 
         Parameters
         ----------
         **sample_kwargs
@@ -153,16 +156,16 @@
     *,
     init_dist: pt.TensorVariable,
     mu: float = 0,
     sigma: float,
     nu: float = 1,
     length: int,
     student_t: bool,
-    initval: numpy.ndarray = None,
-    dims: typing.Optional[str] = None,
+    initval: Optional[numpy.ndarray] = None,
+    dims: Optional[str] = None,
 ):
     """Create a random walk with either a Normal or Student-t distribution.
 
     For some PyMC versions and for Student-t distributed random walks,
     the distribution is created from a cumsum of a N-dimensional random variable.
 
     Parameters
@@ -211,15 +214,19 @@
         initval=initval,
         dims=dims,
     )
     return rw
 
 
 def _get_smoothed_mu(
-    t: numpy.ndarray, y: numpy.ndarray, cm_cdw: calibr8.CalibrationModel, *, clip=0.5
+    t: Sequence[float],
+    y: Sequence[float],
+    cm_cdw: calibr8.CalibrationModel,
+    *,
+    clip: float = 0.5,
 ) -> numpy.ndarray:
     """Calculate a rough estimate of the specific growth rate from smoothed observations.
 
     Parameters
     ----------
     t : numpy.ndarray
         Timepoints
@@ -232,18 +239,18 @@
 
     Returns
     -------
     mu : numpy.ndarray
         A vector of specific growth rates.
     """
     # apply moving average to reduce backscatter noise
-    y = numpy.convolve(y, numpy.ones(5) / 5, "same")
+    yarr = numpy.convolve(y, numpy.ones(5) / 5, "same")
 
     # convert to biomass
-    X = cm_cdw.predict_independent(y)
+    X = cm_cdw.predict_independent(yarr)
 
     # calculate growth rate
     dX = numpy.diff(X)
     dt = numpy.diff(t)
     Xsegment = numpy.mean([X[1:], X[:-1]], axis=0)
     mu = (dX / dt) / Xsegment
 
@@ -255,25 +262,25 @@
 
     # Replace NaNs that can show up with non-linear calibration models
     mu[numpy.isnan(mu)] = 0
     return mu
 
 
 def fit_mu_t(
-    t: typing.Sequence[float],
-    y: typing.Sequence[float],
+    t: Sequence[float],
+    y: Sequence[float],
     calibration_model: calibr8.CalibrationModel,
     *,
-    switchpoints: typing.Optional[typing.Union[typing.Sequence[float], typing.Dict[float, str]]] = None,
+    switchpoints: Optional[Union[Sequence[float], Dict[float, str]]] = None,
     mcmc_samples: int = 0,
     mu_prior: float = 0,
     drift_scale: float,
     nu: float = 5,
     x0_prior: float = 0.25,
-    student_t: typing.Optional[bool] = None,
+    student_t: Optional[bool] = None,
     switchpoint_prob: float = 0.01,
     replicate_id: str = "unnamed",
 ):
     """Models a vector of growth rates to describe the observations.
 
     A MAP estimate is automatically determined.
 
@@ -353,15 +360,15 @@
             _log.info(
                 "Creating model with %d switchpoints. StudentT=%b", len(t_switchpoints_known), student_t
             )
             # the growth rate vector is fragmented according to t_switchpoints_known
             mu_segments = []
             i_from = 0
             for i, t_switch in enumerate(t_switchpoints_known):
-                i_to = numpy.argmax(t > t_switch)
+                i_to = int(numpy.argmax(t > t_switch))
                 i_len = len(t[i_from:i_to])
                 name = f"mu_phase_{i}"
                 slc = slice(i_from, i_to)
                 mu_segments.append(
                     _make_random_walk(
                         name,
                         init_dist=init_dist,
@@ -456,18 +463,18 @@
         result.sample(draws=mcmc_samples)
 
     return result
 
 
 def detect_switchpoints(
     switchpoint_prob: float,
-    t_data: typing.Sequence[float],
+    t_data: Sequence[float],
     pmodel: pm.Model,
-    theta_map: typing.Dict[str, numpy.ndarray],
-) -> typing.Dict[float, str]:
+    theta_map: Dict[str, numpy.ndarray],
+) -> Dict[float, str]:
     """Helper function to detect switchpoints from a fitted random walk.
 
     Parameters
     ----------
     switchpoint_prob
         Probability threshold for detecting switchpoints.
         Random walk innovations with a prior probability less than this
@@ -505,22 +512,22 @@
             innov = numpy.diff(theta_map[rvname])
             # Now we can evaluate the CDFs  of the innovations.
             logcdfs = pm.logcdf(innov_dist, innov).eval()
             # We define switchpoints based on the time of the point with an extreme CDF value.
             # To get our <number of segments> length vector to align with the <number of points>,
             # we prepend a 0.5 as a placeholder for the CDF of the initial point of the random walk.
             cdf_evals += [0.5, *numpy.exp(logcdfs)]
-    cdf_evals = numpy.array(cdf_evals)
-    if len(cdf_evals) != len(t_data) - 1:
+    cdf_evals_arr = numpy.array(cdf_evals)
+    if len(cdf_evals_arr) != len(t_data) - 1:
         raise Exception(
-            f"Failed to find all random walk segments. Found {len(cdf_evals)}, expected {len(t_data) - 1}."
+            f"Failed to find all random walk segments. Found {len(cdf_evals_arr)}, expected {len(t_data) - 1}."
         )
     # Filter for the elements that lie outside of the [0.005, 0.995] interval (if switchpoint_prob=0.01).
     significance_mask = numpy.logical_or(
-        cdf_evals < (switchpoint_prob / 2),
-        cdf_evals > (1 - switchpoint_prob / 2),
+        cdf_evals_arr < (switchpoint_prob / 2),
+        cdf_evals_arr > (1 - switchpoint_prob / 2),
     )
     # Collect switchpoint information from points with significant CDF values.
     # Here we don't need to filter known switchpoints, because these correspond to the first
     # point in each random walk, for which we assigned non-significant 0.5 CDF placeholders above.
     switchpoints = {t: "detected" for t, is_switchpoint in zip(t_data, significance_mask) if is_switchpoint}
     return switchpoints
```

### Comparing `bletl-1.2.2/bletl/heuristics.py` & `bletl-1.3.1/bletl/heuristics.py`

 * *Files identical despite different names*

### Comparing `bletl-1.2.2/bletl/parsing/bl1.py` & `bletl-1.3.1/bletl/parsing/bl1.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,20 +88,20 @@
             data = self.calibrate_with_parameters(data, **cal_data)
 
         return data
 
     def calibrate_with_parameters(
         self,
         data: BLData,
-        cal_0: float = None,
-        cal_100: float = None,
-        phi_min: float = None,
-        phi_max: float = None,
-        pH_0: float = None,
-        dpH: float = None,
+        cal_0: Optional[float] = None,
+        cal_100: Optional[float] = None,
+        phi_min: Optional[float] = None,
+        phi_max: Optional[float] = None,
+        pH_0: Optional[float] = None,
+        dpH: Optional[float] = None,
     ):
         def process_backscatter(raw_data_df, cycle_ref_df, global_ref):
             """
             Calculation of referenced BS signal:
             (global_ref / cycle_ref) * amplitude
             """
             BS = pandas.DataFrame().reindex_like(raw_data_df)
@@ -178,22 +178,22 @@
                 times = data.measurements.xs(filter_number, level="filterset")["time"].unstack()
                 data[filter_name + f"{gain:.0f}"] = FilterTimeSeries(times, raw_values)
         return data
 
     def parse(
         self,
         filepath,
-        lot_number: int = None,
-        temp: int = None,
-        cal_0: float = None,
-        cal_100: float = None,
-        phi_min: float = None,
-        phi_max: float = None,
-        pH_0: float = None,
-        dpH: float = None,
+        lot_number: Optional[int] = None,
+        temp: Optional[int] = None,
+        cal_0: Optional[float] = None,
+        cal_100: Optional[float] = None,
+        phi_min: Optional[float] = None,
+        phi_max: Optional[float] = None,
+        pH_0: Optional[float] = None,
+        dpH: Optional[float] = None,
     ):
         headerlines, data = split_header_data(filepath)
 
         metadata = extract_metadata(headerlines)
         process_parameters = extract_process_parameters(headerlines)
         filtersets = extract_filtersets(headerlines)
         comments = extract_comments(data)
@@ -472,14 +472,16 @@
 
     Returns
     -------
     calibration_dict : dict
         Dictionary containing calibration data.
         Can be readily used in calibration function.
     """
+    assert utils.__spec__ is not None
+    assert utils.__spec__.origin is not None
     module_path = pathlib.Path(utils.__spec__.origin).parents[0]
     calibration_file = pathlib.Path(module_path, "cache", "CalibrationLot.ini")
 
     if not calibration_file.is_file():
         if not utils.download_calibration_data():
             return None
```

### Comparing `bletl-1.2.2/bletl/parsing/blpro.py` & `bletl-1.3.1/bletl/parsing/blpro.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,68 @@
 """Parsing functions for the BioLector Pro"""
 import collections
 import datetime
 import io
 import logging
+import os
 import pathlib
 import re
 import warnings
 import xml.etree.ElementTree
+from typing import Optional, Union
 
 import numpy
 import pandas
 
-from bletl.parsing.bl1 import fetch_calibration_data
-
 from .. import utils
 from ..types import (
     BioLectorModel,
     BLData,
     BLDParser,
     FilterTimeSeries,
     InvalidLotNumberError,
 )
 
 logger = logging.getLogger("blpro")
 
 
+_MF_WELL_NUMC_TO_ID = {
+    (colnumber + rownumber * 8): f"{row}{column:02d}"
+    for colnumber, column in enumerate(range(1, 9))
+    for rownumber, row in enumerate("CDEF")
+}
+"""Maps 0-based well numbers in MF mode by **C-style** counting order (→ then ↓) to alphanumeric well IDs."""
+
+_MF_WELL_NUMF_TO_ID = {
+    (rownumber + colnumber * 4): f"{row}{column:02d}"
+    for rownumber, row in enumerate("CDEF")
+    for colnumber, column in enumerate(range(1, 9))
+}
+"""Maps 0-based well numbers in MF mode by **Fortran-style** counting order (↓ then →) to alphanumeric well IDs."""
+
+_MF_WELL_NUMM_TO_ID = {
+    1 + (colnumber + rownumber * 8): f"{row}{column:02d}"
+    for rownumber, row in enumerate("CDEF")
+    for colnumber, column in enumerate(reversed(range(1, 9)) if rownumber % 2 else range(1, 9))
+}
+"""Maps 1-based well numbers in MF mode by **measurement counting order** (→→→ ↓ ←←← ↓ →→→ ...) to alphanumeric well IDs."""
+
+
 class BioLectorProParser(BLDParser):
     def parse(
         self,
-        filepath,
-        lot_number: int = None,
-        temp: int = None,
-        cal_0: float = None,
-        cal_100: float = None,
-        phi_min: float = None,
-        phi_max: float = None,
-        pH_0: float = None,
-        dpH: float = None,
+        filepath: Union[str, os.PathLike],
+        lot_number: Optional[int] = None,
+        temp: Optional[int] = None,
+        cal_0: Optional[float] = None,
+        cal_100: Optional[float] = None,
+        phi_min: Optional[float] = None,
+        phi_max: Optional[float] = None,
+        pH_0: Optional[float] = None,
+        dpH: Optional[float] = None,
     ) -> BLData:
         metadata, data = parse_metadata_data(filepath)
 
         bld = BLData(
             model=BioLectorModel.BLPro,
             environment=extract_environment(data),
             filtersets=extract_filtersets(metadata),
@@ -50,15 +72,15 @@
         )
 
         bld.metadata = metadata
         bld.fluidics = extract_fluidics(data)
         bld.valves, bld.module = extract_valves_module(data)
         bld.diagnostics = extract_diagnostics(data)
 
-        if not None in [lot_number, temp]:
+        if lot_number is not None and temp is not None:
             lot_cal_data = fetch_calibration_data(lot_number, temp)
         else:
             lot_cal_data = None
 
         if lot_cal_data or (not None in [cal_0, cal_100, phi_min, phi_max, pH_0, dpH]):
             for key, fts in transform_into_filtertimeseries(
                 bld.metadata, bld.measurements, bld.filtersets, True
@@ -325,14 +347,15 @@
         ("Well", "well", int),
         ("Time", "time", float),
         ("Reservoir", "reservoir", float),
         ("MF_Volume", "mf_volume", float),
         ("Temp_Ch4", "volume", float),
     ]
     df = utils.__to_typed_cols__(dfraw[dfraw["Type"] == "F"], ocol_ncol_type)
+    df["well"] = [_MF_WELL_NUMM_TO_ID[w] for w in df["well"]]
     df = df.sort_values(["well", "cycle"]).set_index(["well"])
     return standardize(df)
 
 
 def extract_valves_module(dfraw):
     ocol_ncol_type = [
         ("Cycle", "cycle", int),
@@ -344,23 +367,25 @@
     df = utils.__to_typed_cols__(dfraw[dfraw["Type"] == "N"], ocol_ncol_type)
 
     # table of valve actions
     df_valves = df[df["valve"] != "Module 1 (BASE)"].copy()
     df_valves.columns = ["cycle", "valve", "well", "acid", "base"]
     df_valves["valve"] = df_valves["valve"].str.replace("Valve ", "").astype(int)
     df_valves["well"] = df_valves["well"].str.replace("Well", "").astype(int)
+    # TODO: Which numbering style is this?
     df_valves["acid"] = df_valves["acid"].str.replace("Sollvolumen (Acid) ", "", regex=False).astype(float)
     df_valves["base"] = df_valves["base"].str.replace("Sollvolumen (Base) ", "", regex=False).astype(float)
     df_valves = standardize(df_valves).set_index(["well", "valve", "cycle"])
 
     # TODO: unknown column purpose
     df_module = df[df["valve"] == "Module 1 (BASE)"].copy()
     df_module.columns = ["cycle", "module", "valve", "well", "volume"]
     df_module["valve"] = df_module["valve"].str.replace("Valve ", "").astype(int)
     df_module["well"] = df_module["well"].str.replace("Well ", "").astype(int)
+    # TODO: Which numbering style is this?
     df_module["volume"] = df_module["volume"].str.replace("Volume ", "").astype(float)
     df_module = standardize(df_module).set_index(["well", "valve", "cycle"])
 
     return df_valves, df_module
 
 
 def extract_diagnostics(dfraw):
@@ -472,14 +497,16 @@
 
     Returns
     -------
     calibration_dict : dict
         Dictionary containing calibration data.
         Can be readily used in calibration function.
     """
+    assert utils.__spec__ is not None
+    assert utils.__spec__.origin is not None
     module_path = pathlib.Path(utils.__spec__.origin).parents[0]
     calibration_file = pathlib.Path(module_path, "cache", "CalibrationLot_II.xml")
 
     if not calibration_file.is_file():
         if not utils.download_calibration_data():
             return None
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bletl-1.2.2/bletl/splines.py` & `bletl-1.3.1/bletl/splines.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import copy
 import logging
 import multiprocessing
 import numbers
 import pickle
-from typing import Callable, Dict, Optional, Sequence, Tuple, Union
+from typing import Callable, Dict, List, Optional, Sequence, Tuple, Union
 
 import csaps
 import joblib
 import numpy
 import pandas
 import scipy.interpolate
 import scipy.optimize
@@ -43,29 +43,34 @@
             der = self.derivative(order - 1)
             der_f = lambda x: der(x)
             return lambda x: (der_f(x + epsilon) - der_f(x - epsilon)) / (2 * epsilon)
         raise NotImplementedError(
             f"{order}-order derivatives are not implemented for the UnivariateCubicSmoothingSpline"
         )
 
-    def __call__(self, xi: Union[float, numpy.ndarray]):
+    def __call__(
+        self,
+        x: csaps.UnivariateDataType,
+        nu: Optional[int] = None,
+        extrapolate: Optional[Union[bool, str]] = None,
+    ) -> numpy.ndarray:
         """Evaluate the spline at some coordinates.
 
         This method overrides the implementation of the base type
         to align it with the API of the `scipy.interpolate` splines.
 
         Parameters
         ----------
-        xi : float, numpy.ndarray
+        x : float, numpy.ndarray
             One or more coordinates at which the spline should be evaluated.
         """
         # scipy splines can be called on scalars
-        xi_arr = numpy.atleast_1d(xi)
+        xi_arr = numpy.atleast_1d(numpy.asarray(x))
         result = super().__call__(xi_arr)
-        if isinstance(xi, (int, float)):
+        if isinstance(x, (int, float)):
             return result[0]
         return result
 
 
 def _normalize_smoothing_factor(method: str, smooth: float, x: numpy.ndarray, y: numpy.ndarray) -> float:
     """Normalization of smoothing factor from the interval [0,1] to the value required by the Spline type.
 
@@ -115,15 +120,15 @@
         Options: "ucss" UnivariateCubicSmoothingSpline, "us" UnivariateSpline
 
     Returns
     -------
     mssr : float
         Mean sum of squared residuals of the splines fitted to data subsets.
     """
-    smoothing_factor = numpy.atleast_1d(smoothing_factor)
+    smoothing_factor_arr = numpy.atleast_1d(smoothing_factor)
     if k < 2:
         raise ValueError(f"Need k≥2 splits for crossvalidation. Setting was k={k}.")
     if len(values) < 3 * k:
         raise ValueError(
             f"Time series of {len(values)} elements is too short. " f"Need at least a length of 3*k ({3*k})."
         )
     ssrs = []
@@ -134,27 +139,27 @@
         test_mask = numpy.invert(train_mask)
         ssrs.append(
             _evaluate_spline_test_error(
                 x=timepoints,
                 y=values,
                 train_idxs=train_mask,
                 test_idxs=test_mask,
-                smoothing_factor=smoothing_factor,
+                smoothing_factor=smoothing_factor_arr,
                 method=method,
             )
         )
-    return numpy.mean(ssrs)
+    return float(numpy.mean(ssrs))
 
 
 def _evaluate_spline_test_error(
     x: numpy.ndarray,
     y: numpy.ndarray,
     train_idxs: numpy.ndarray,
     test_idxs: numpy.ndarray,
-    smoothing_factor: float,
+    smoothing_factor: numpy.ndarray,
     method: str,
 ) -> float:
     """Fits spline to a test set and returns the sum of squared error on the test set.
 
     Parameters
     ----------
     x : numpy.ndarray
@@ -230,15 +235,15 @@
 
 def get_multiple_splines(
     fts: FilterTimeSeries,
     wells: Sequence[str],
     k_folds: int = 5,
     method: str = "us",
     last_cycle: Optional[int] = None,
-) -> Dict[str, Union[UnivariateCubicSmoothingSpline, scipy.interpolate.UnivariateSpline]]:
+) -> List[Tuple[str, Union[UnivariateCubicSmoothingSpline, scipy.interpolate.UnivariateSpline]]]:
     """Returns multiple splines with k-fold crossvalidated smoothing factor
 
     Parameters
     ----------
     fts : FilterTimeSeries
         FilterTimeSeries containing timepoints and observed data-
     wells : list of str
@@ -251,15 +256,15 @@
 
     Returns
     -------
     splines : dict
         Dict with {well:spline} for each well of "wells"
     """
     x, y = fts.get_timeseries(wells[0])
-    if last_cycle == None:
+    if last_cycle is None:
         last_cycle = len(x)
     elif last_cycle > len(x):
         raise ValueError("Please change last_cycle.")
 
     def get_spline_parallel(arg):
         well, timepoints, values, k_folds = arg
         spline = get_crossvalidated_spline(timepoints, values, k_folds, method=method)
@@ -326,17 +331,17 @@
         If blanks are not provided for every well,
         of if an invalid blank option is passed.
     """
     # check inputs
     if wells == "all":
         wells = list(bsdata.time.columns)
     if blank == "first":
-        blank_dict = {well: data.iloc[0] for well, data in bsdata.value.iteritems()}
+        blank_dict = {well: data.iloc[0] for well, data in bsdata.value.items()}
     elif isinstance(blank, numbers.Number):
-        blank_dict = {well: blank for well, data in bsdata.value.iteritems()}
+        blank_dict = {well: blank for well, data in bsdata.value.items()}
     elif isinstance(blank, dict):
         if set(blank.keys()) != set(wells):
             raise ValueError("Please provide blanks for every well")
         blank_dict = blank
     else:
         raise ValueError("Please provide proper blank option.")
     # run spline fitting
```

### Comparing `bletl-1.2.2/bletl/types.py` & `bletl-1.3.1/bletl/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Specifies the base types for parsing and representing BioLector CSV files."""
 import abc
 import enum
-import pathlib
+import os
 import typing
 import warnings
-from typing import Dict, Optional, Tuple
+from typing import Dict, Optional, Tuple, Union
 
 import numpy
 import pandas
 
 
 class BioLectorModel(enum.Enum):
     """Enumeration of BioLector Models."""
@@ -18,21 +18,35 @@
     BLPro = "blpro"
     XT = "blXT"
 
 
 class BLData(dict):
     """Standardized data type for BioLector data."""
 
-    def __init__(self, model, environment, filtersets, references, measurements, comments):
+    def __init__(
+        self,
+        model: BioLectorModel,
+        environment: pandas.DataFrame,
+        filtersets: pandas.DataFrame,
+        references: pandas.DataFrame,
+        measurements: pandas.DataFrame,
+        comments: pandas.DataFrame,
+    ):
         self._model = model
         self._environment = environment
         self._filtersets = filtersets
         self._references = references
         self._measurements = measurements
         self._comments = comments
+        # Optional, depending on the BioLector Model
+        self.metadata: dict = {}
+        self.fluidics: Optional[pandas.DataFrame] = None
+        self.module: Optional[pandas.DataFrame] = None
+        self.valves: Optional[pandas.DataFrame] = None
+        self.diagnostics: Optional[pandas.DataFrame] = None
         super().__init__()
 
     @property
     def model(self) -> BioLectorModel:
         """BioLector model that the dataset was acquired with."""
         return self._model
 
@@ -43,15 +57,15 @@
 
     @property
     def filtersets(self) -> pandas.DataFrame:
         """Filtersets that were used in this process."""
         return self._filtersets
 
     @property
-    def wells(self) -> typing.Tuple[str]:
+    def wells(self) -> typing.Tuple[str, ...]:
         """Wells that were measured."""
         if len(self) == 0:
             return tuple()
         return tuple(self.values())[0].wells
 
     @property
     def references(self) -> pandas.DataFrame:
@@ -196,23 +210,25 @@
         )
 
 
 class FilterTimeSeries:
     """Generalizable data type for calibrated timeseries."""
 
     @property
-    def wells(self) -> typing.Tuple[str]:
+    def wells(self) -> typing.Tuple[str, ...]:
         """Well IDs that were measured."""
         return tuple(self.time.columns)
 
     def __init__(self, time_df: pandas.DataFrame, value_df: pandas.DataFrame):
         self.time = time_df
         self.value = value_df
 
-    def get_timeseries(self, well: str, *, last_cycle: int = None) -> Tuple[numpy.ndarray, numpy.ndarray]:
+    def get_timeseries(
+        self, well: str, *, last_cycle: Optional[int] = None
+    ) -> Tuple[numpy.ndarray, numpy.ndarray]:
         """Retrieves (time, value) for a specific well.
 
         Parameters
         ----------
         well : str
             Well id to retrieve.
         last_cycle : int, optional
@@ -264,15 +280,15 @@
     """Abstract type for parsers that read BioLector CSV files."""
 
     __metaclass__ = abc.ABCMeta
 
     @abc.abstractmethod
     def parse(
         self,
-        filepath: pathlib.Path,
+        filepath: Union[str, os.PathLike],
         *,
         lot_number: Optional[int] = None,
         temp: Optional[int] = None,
         cal_0: Optional[float] = None,
         cal_100: Optional[float] = None,
         phi_min: Optional[float] = None,
         phi_max: Optional[float] = None,
```

### Comparing `bletl-1.2.2/bletl/utils.py` & `bletl-1.3.1/bletl/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """Contains helper functions that do not depend on other modules within this package."""
 import datetime
 import pathlib
 import re
 import urllib
-from typing import Sequence, Tuple, Union
+from typing import Optional, Sequence, Tuple, Union
 
 import pandas
 
 from . import core
 
 
-def __to_typed_cols__(dfin: pandas.DataFrame, ocol_ncol_type: Tuple[str, str, type]) -> pandas.DataFrame:
+def __to_typed_cols__(
+    dfin: pandas.DataFrame, ocol_ncol_type: Sequence[Tuple[Optional[str], str, type]]
+) -> pandas.DataFrame:
     """Can be used to filter & convert data frame columns.
 
     Parameters
     ----------
     dfin : pandas.DataFrame
         Raw data frame to start from.
     ocol_ncol_type : list of tuples
@@ -31,15 +33,15 @@
         if ocol is None or not ocol in dfin:
             dfout[ncol] = None
         else:
             dfout[ncol] = dfin[ocol].astype(typ)
     return dfout
 
 
-def _unindex(dataframe: pandas.DataFrame) -> Tuple[Sequence[Union[str, None]], pandas.DataFrame]:
+def _unindex(dataframe: pandas.DataFrame) -> Tuple[Sequence[Optional[str]], pandas.DataFrame]:
     """Resets the index of the DataFrame.
 
     Parameters
     ----------
     dataframe : pandas.DataFrame
         Guess what.
 
@@ -106,18 +108,18 @@
         if "cycle" in columns and len(stack) > 0:
             fragment["cycle"] += max(stack["cycle"])
 
         # append the fragment to the stack
         stack = pandas.concat((stack, fragment))
 
     # re-apply the original indexing scheme
-    return _reindex(stack, index_names)
+    return _reindex(stack, index_names)  # type: ignore
 
 
-def _last_well_in_cycle(measurements: pandas.DataFrame) -> str:
+def _last_well_in_cycle(measurements: pandas.DataFrame) -> Optional[str]:
     """Finds the name of the last well measured in a cycle.
 
     Parameters
     ----------
     measurements : pandas.DataFrame
         Measurements data.
 
@@ -191,14 +193,16 @@
 
     Returns
     -------
     success : bool
         `True` if calibration data was downloaded successfully, `False` otherwise.
     """
     try:
+        assert core.__spec__ is not None
+        assert core.__spec__.origin is not None
         module_path = pathlib.Path(core.__spec__.origin).parents[0]
 
         url_bl1 = "http://updates.m2p-labs.com/CalibrationLot.ini"
         filepath_bl1 = pathlib.Path(module_path, "cache", "CalibrationLot.ini")
         filepath_bl1.parents[0].mkdir(exist_ok=True)
         urllib.request.urlretrieve(url_bl1, filepath_bl1)
```

### Comparing `bletl-1.2.2/bletl.egg-info/SOURCES.txt` & `bletl-1.3.1/bletl.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 pyproject.toml
 setup.py
 bletl/__init__.py
 bletl/core.py
 bletl/features.py
 bletl/growth.py
 bletl/heuristics.py
+bletl/py.typed
 bletl/splines.py
 bletl/types.py
 bletl/utils.py
 bletl.egg-info/PKG-INFO
 bletl.egg-info/SOURCES.txt
 bletl.egg-info/dependency_links.txt
 bletl.egg-info/not-zip-safe
```

### Comparing `bletl-1.2.2/setup.py` & `bletl-1.3.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,25 +22,29 @@
 
 __version__ = get_version()
 
 if __name__ == "__main__":
     setuptools.setup(
         name=__packagename__,
         packages=setuptools.find_packages(),
+        package_data={"bletl": ["py.typed"]},
         zip_safe=False,
         version=__version__,
         description="Package for parsing and transforming BioLector raw data.",
+        long_description=open(pathlib.Path(__file__).parent / "README.md").read(),
+        long_description_content_type="text/markdown",
         url="https://github.com/jubiotech/bletl",
         author="Michael Osthege",
         author_email="m.osthege@fz-juelich.de",
         license="GNU Affero General Public License v3.0",
         classifiers=[
             "Programming Language :: Python",
             "Operating System :: OS Independent",
             "Programming Language :: Python :: 3.8",
             "Programming Language :: Python :: 3.9",
             "Programming Language :: Python :: 3.10",
+            "Programming Language :: Python :: 3.11",
             "Intended Audience :: Science/Research",
             "License :: OSI Approved :: GNU Affero General Public License v3",
         ],
         install_requires=open(pathlib.Path(ROOT, "requirements.txt")).readlines(),
     )
```

### Comparing `bletl-1.2.2/tests/test_core.py` & `bletl-1.3.1/tests/test_core.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import numpy
 import pandas
 import pytest
 from numpy import random
 
 import bletl
 from bletl import core, parsing, utils
-from bletl.parsing import bl1
+from bletl.parsing import bl1, blpro
 
 dir_testfiles = pathlib.Path(pathlib.Path(__file__).absolute().parent, "data")
 
 BL1_files = [
     pathlib.Path(dir_testfiles, "BL1", "NT_1400rpm_30C_BS15_5min_20180618_102917.csv"),
     pathlib.Path(dir_testfiles, "BL1", "JH_ShakerSteps_20170302_070206.csv"),
     pathlib.Path(dir_testfiles, "BL1", "rj-cg-res_20170927_084112.csv"),
@@ -264,19 +264,18 @@
         fp = pathlib.Path(
             dir_testfiles, "BL1", "example_with_cal_data_NT_1400rpm_30C_BS20-pH-DO_10min_20180607_115856.csv"
         )
         data = bletl.parse(fp)
         unified_df = data["BS20"].get_unified_dataframe()
         assert isinstance(unified_df, pandas.DataFrame)
         numpy.testing.assert_approx_equal(unified_df.index[2], 0.35313, significant=4)
-        numpy.testing.assert_approx_equal(
-            unified_df.iloc[unified_df.index.get_loc(5, method="nearest"), unified_df.columns.get_loc("A05")],
-            63.8517,
-            significant=6,
-        )
+        idx = unified_df.index.get_indexer([5], method="nearest")
+        col = unified_df.columns.get_indexer(["A05"])
+        values = unified_df.iloc[idx, col].to_numpy()
+        numpy.testing.assert_approx_equal(values, 63.8517, significant=6)
 
     def test_get_narrow_data(self):
         fp = pathlib.Path(
             dir_testfiles, "BL1", "example_with_cal_data_NT_1400rpm_30C_BS20-pH-DO_10min_20180607_115856.csv"
         )
         data = bletl.parse(fp)
         narrow_data = data.get_narrow_data()
@@ -592,7 +591,47 @@
 
     def test_comments(self):
         d_1 = bletl.parse(BL1_files[0], lot_number=1818, temp=30)
         d_p = bletl.parse(BLPro_files[0])
 
         assert list(d_1.comments.columns) == list(d_p.comments.columns)
         return
+
+
+class TestBLProMF:
+    def test_well_num_mappings(self):
+        # C-style counts right then down
+        assert blpro._MF_WELL_NUMC_TO_ID[0] == "C01"
+        assert blpro._MF_WELL_NUMC_TO_ID[1] == "C02"
+        assert blpro._MF_WELL_NUMC_TO_ID[7] == "C08"
+        assert blpro._MF_WELL_NUMC_TO_ID[8] == "D01"
+        assert blpro._MF_WELL_NUMC_TO_ID[31] == "F08"
+        # F-style counts down then right
+        assert blpro._MF_WELL_NUMF_TO_ID[0] == "C01"
+        assert blpro._MF_WELL_NUMF_TO_ID[1] == "D01"
+        assert blpro._MF_WELL_NUMF_TO_ID[2] == "E01"
+        assert blpro._MF_WELL_NUMF_TO_ID[3] == "F01"
+        assert blpro._MF_WELL_NUMF_TO_ID[4] == "C02"
+        assert blpro._MF_WELL_NUMF_TO_ID[31] == "F08"
+        # Measurement order style is 1-based and goes left/right vice versa
+        assert blpro._MF_WELL_NUMM_TO_ID[1] == "C01"
+        assert blpro._MF_WELL_NUMM_TO_ID[2] == "C02"
+        assert blpro._MF_WELL_NUMM_TO_ID[8] == "C08"
+        assert blpro._MF_WELL_NUMM_TO_ID[9] == "D08"
+        assert blpro._MF_WELL_NUMM_TO_ID[16] == "D01"
+        assert blpro._MF_WELL_NUMM_TO_ID[32] == "F01"
+        pass
+
+    def test_issue_38(self):
+        fp = dir_testfiles / "BLPro" / "18-FZJ-Test2--2018-02-07-10-01-11.csv"
+        bldata = bletl.parse(fp)
+        assert bldata.fluidics.index.name == "well"
+        assert bldata.module.index.names == ["well", "valve", "cycle"]
+        assert bldata.valves.index.names == ["well", "valve", "cycle"]
+        # Check some initial and final well volumes against values shown in the BioLection
+        assert bldata.fluidics.loc["C01", "volume"][0] == 800
+        assert bldata.fluidics.loc["C01", "volume"][-1] == 1201.776
+        assert bldata.fluidics.loc["D01", "volume"][-1] == 1204.892
+        assert bldata.fluidics.loc["D02", "volume"][-1] == 954.68
+        assert bldata.fluidics.loc["E06", "volume"][-1] == 913.16
+        assert bldata.fluidics.loc["F01", "volume"][-1] == 1202.719
+        pass
```

### Comparing `bletl-1.2.2/tests/test_features.py` & `bletl-1.3.1/tests/test_features.py`

 * *Files identical despite different names*

### Comparing `bletl-1.2.2/tests/test_growth.py` & `bletl-1.3.1/tests/test_growth.py`

 * *Files identical despite different names*

### Comparing `bletl-1.2.2/tests/test_heuristics.py` & `bletl-1.3.1/tests/test_heuristics.py`

 * *Files identical despite different names*

### Comparing `bletl-1.2.2/tests/test_splines.py` & `bletl-1.3.1/tests/test_splines.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿import pathlib
+import pathlib
 
 import numpy
 import pytest
 import scipy.interpolate
 
 import bletl
 import bletl.splines
@@ -62,15 +62,15 @@
         # scalar blank for all
         mue_blank_scalar = bletl.splines.get_mue(bldata["BS3"], blank=2, wells=wells, method="us")
         mue_median = numpy.median(mue_blank_scalar.value.loc[60:75, "B03"])
         numpy.testing.assert_allclose(mue_median, 0.30, atol=0.01)
 
         # dictionary of scalars (first 5 cycles)
         blank_dict = {
-            well: data.iloc[:5].mean() for well, data in bldata["BS3"].value.iteritems() if well in wells
+            well: data.iloc[:5].mean() for well, data in bldata["BS3"].value.items() if well in wells
         }
         mue_blank_dict = bletl.splines.get_mue(bldata["BS3"], wells=wells, blank=blank_dict, method="us")
         mue_median = numpy.median(mue_blank_dict.value.loc[60:75, "B03"])
         numpy.testing.assert_allclose(mue_median, 0.38, atol=0.02)
 
         # check value error when the wells dictionary is incorrect
         with pytest.raises(ValueError):
@@ -94,15 +94,15 @@
 
         # scalar blank for all
         mue_blank_scalar = bletl.splines.get_mue(bldata["BS3"], blank=2, method="us")
         mue_median = numpy.median(mue_blank_scalar.value.loc[60:75, "B03"])
         numpy.testing.assert_allclose(mue_median, 0.30, atol=0.01)
 
         # dictionary of scalars (first 5 cycles)
-        blank_dict = {well: data.iloc[:5].mean() for well, data in bldata["BS3"].value.iteritems()}
+        blank_dict = {well: data.iloc[:5].mean() for well, data in bldata["BS3"].value.items()}
         mue_blank_dict = bletl.splines.get_mue(bldata["BS3"], blank=blank_dict, method="us")
         mue_median = numpy.median(mue_blank_dict.value.loc[60:75, "B03"])
         numpy.testing.assert_allclose(mue_median, 0.38, atol=0.02)
         return
 
 
 class TestSplineMueCsaps:
@@ -138,15 +138,15 @@
         # scalar blank for all
         mue_blank_scalar = bletl.splines.get_mue(bldata["BS3"], blank=2, wells=wells, method="ucss")
         mue_median = numpy.median(mue_blank_scalar.value.loc[60:75, "B03"])
         numpy.testing.assert_allclose(mue_median, 0.30, atol=0.02)
 
         # dictionary of scalars (first 5 cycles)
         blank_dict = {
-            well: data.iloc[:5].mean() for well, data in bldata["BS3"].value.iteritems() if well in wells
+            well: data.iloc[:5].mean() for well, data in bldata["BS3"].value.items() if well in wells
         }
         mue_blank_dict = bletl.splines.get_mue(bldata["BS3"], wells=wells, blank=blank_dict, method="ucss")
         mue_median = numpy.median(mue_blank_dict.value.loc[60:75, "B03"])
         numpy.testing.assert_allclose(mue_median, 0.38, atol=0.02)
 
         # check value error when the wells dictionary is incorrect
         with pytest.raises(ValueError):
@@ -170,15 +170,15 @@
 
         # scalar blank for all
         mue_blank_scalar = bletl.splines.get_mue(bldata["BS3"], blank=2, method="ucss")
         mue_median = numpy.median(mue_blank_scalar.value.loc[60:75, "B03"])
         numpy.testing.assert_allclose(mue_median, 0.30, atol=0.02)
 
         # dictionary of scalars (first 5 cycles)
-        blank_dict = {well: data.iloc[:5].mean() for well, data in bldata["BS3"].value.iteritems()}
+        blank_dict = {well: data.iloc[:5].mean() for well, data in bldata["BS3"].value.items()}
         mue_blank_dict = bletl.splines.get_mue(bldata["BS3"], blank=blank_dict, method="ucss")
         mue_median = numpy.median(mue_blank_dict.value.loc[60:75, "B03"])
         numpy.testing.assert_allclose(mue_median, 0.38, atol=0.02)
         return
 
 
 class TestSplineMethodEquivalence:
```

