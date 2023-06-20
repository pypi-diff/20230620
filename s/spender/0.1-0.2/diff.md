# Comparing `tmp/spender-0.1.tar.gz` & `tmp/spender-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spender-0.1.tar", last modified: Wed Nov 16 01:12:19 2022, max compression
+gzip compressed data, was "spender-0.2.tar", last modified: Tue Jun 20 21:57:41 2023, max compression
```

## Comparing `spender-0.1.tar` & `spender-0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2022-11-16 01:12:19.800074 spender-0.1/
--rw-r--r--   0 pmelchior   (501) staff       (20)     1082 2022-08-08 22:13:56.000000 spender-0.1/LICENSE
--rw-r--r--   0 pmelchior   (501) staff       (20)     2223 2022-11-16 01:12:19.799953 spender-0.1/PKG-INFO
--rw-r--r--   0 pmelchior   (501) staff       (20)     1506 2022-11-15 23:10:37.000000 spender-0.1/README.md
--rw-r--r--   0 pmelchior   (501) staff       (20)       38 2022-11-16 01:12:19.800120 spender-0.1/setup.cfg
--rw-r--r--   0 pmelchior   (501) staff       (20)     1058 2022-11-16 01:12:11.000000 spender-0.1/setup.py
-drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2022-11-16 01:12:19.798936 spender-0.1/spender/
--rw-r--r--   0 pmelchior   (501) staff       (20)     2069 2022-11-16 00:22:19.000000 spender-0.1/spender/__init__.py
-drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2022-11-16 01:12:19.799775 spender-0.1/spender/data/
--rw-r--r--   0 pmelchior   (501) staff       (20)        0 2022-08-08 22:13:56.000000 spender-0.1/spender/data/__init__.py
--rwxr-xr-x   0 pmelchior   (501) staff       (20)      906 2022-11-15 17:35:33.000000 spender-0.1/spender/data/emission_lines.py
--rw-r--r--   0 pmelchior   (501) staff       (20)    17743 2022-11-15 23:00:52.000000 spender-0.1/spender/data/sdss.py
--rw-r--r--   0 pmelchior   (501) staff       (20)     3919 2022-11-15 22:18:58.000000 spender-0.1/spender/instrument.py
--rw-r--r--   0 pmelchior   (501) staff       (20)    17701 2022-11-15 23:50:08.000000 spender-0.1/spender/model.py
--rw-r--r--   0 pmelchior   (501) staff       (20)     3479 2022-11-15 23:09:11.000000 spender-0.1/spender/util.py
-drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2022-11-16 01:12:19.799473 spender-0.1/spender.egg-info/
--rw-r--r--   0 pmelchior   (501) staff       (20)     2223 2022-11-16 01:12:19.000000 spender-0.1/spender.egg-info/PKG-INFO
--rw-r--r--   0 pmelchior   (501) staff       (20)      332 2022-11-16 01:12:19.000000 spender-0.1/spender.egg-info/SOURCES.txt
--rw-r--r--   0 pmelchior   (501) staff       (20)        1 2022-11-16 01:12:19.000000 spender-0.1/spender.egg-info/dependency_links.txt
--rw-r--r--   0 pmelchior   (501) staff       (20)       68 2022-11-16 01:12:19.000000 spender-0.1/spender.egg-info/requires.txt
--rw-r--r--   0 pmelchior   (501) staff       (20)        8 2022-11-16 01:12:19.000000 spender-0.1/spender.egg-info/top_level.txt
+drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2023-06-20 21:57:41.661634 spender-0.2/
+-rw-r--r--   0 pmelchior   (501) staff       (20)     1082 2022-08-08 22:13:56.000000 spender-0.2/LICENSE
+-rw-r--r--   0 pmelchior   (501) staff       (20)     4947 2023-06-20 21:57:41.661492 spender-0.2/PKG-INFO
+-rw-r--r--   0 pmelchior   (501) staff       (20)     4259 2023-06-20 21:36:05.000000 spender-0.2/README.md
+-rw-r--r--   0 pmelchior   (501) staff       (20)       38 2023-06-20 21:57:41.661673 spender-0.2/setup.cfg
+-rw-r--r--   0 pmelchior   (501) staff       (20)     1049 2023-06-20 21:19:50.000000 spender-0.2/setup.py
+drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2023-06-20 21:57:41.659998 spender-0.2/spender/
+-rw-r--r--   0 pmelchior   (501) staff       (20)     2791 2023-06-20 20:43:19.000000 spender-0.2/spender/__init__.py
+drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2023-06-20 21:57:41.661080 spender-0.2/spender/data/
+-rw-r--r--   0 pmelchior   (501) staff       (20)        0 2022-08-08 22:13:56.000000 spender-0.2/spender/data/__init__.py
+-rwxr-xr-x   0 pmelchior   (501) staff       (20)     1082 2023-05-17 22:05:49.000000 spender-0.2/spender/data/emission_lines.py
+-rw-r--r--   0 pmelchior   (501) staff       (20)    19391 2023-05-17 22:05:49.000000 spender-0.2/spender/data/sdss.py
+-rw-r--r--   0 pmelchior   (501) staff       (20)     3933 2023-05-17 22:05:49.000000 spender-0.2/spender/instrument.py
+-rw-r--r--   0 pmelchior   (501) staff       (20)    16440 2023-05-17 22:05:49.000000 spender-0.2/spender/model.py
+-rw-r--r--   0 pmelchior   (501) staff       (20)     3569 2023-05-17 22:05:49.000000 spender-0.2/spender/util.py
+drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2023-06-20 21:57:41.660636 spender-0.2/spender.egg-info/
+-rw-r--r--   0 pmelchior   (501) staff       (20)     4947 2023-06-20 21:57:41.000000 spender-0.2/spender.egg-info/PKG-INFO
+-rw-r--r--   0 pmelchior   (501) staff       (20)      332 2023-06-20 21:57:41.000000 spender-0.2/spender.egg-info/SOURCES.txt
+-rw-r--r--   0 pmelchior   (501) staff       (20)        1 2023-06-20 21:57:41.000000 spender-0.2/spender.egg-info/dependency_links.txt
+-rw-r--r--   0 pmelchior   (501) staff       (20)       68 2023-06-20 21:57:41.000000 spender-0.2/spender.egg-info/requires.txt
+-rw-r--r--   0 pmelchior   (501) staff       (20)        8 2023-06-20 21:57:41.000000 spender-0.2/spender.egg-info/top_level.txt
```

### Comparing `spender-0.1/LICENSE` & `spender-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spender-0.1/setup.py` & `spender-0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 long_description = open('README.md').read()
 
 setup(
     name="spender",
     description="Spectrum encoder and decoder",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version="0.1",
+    version="0.2",
     license="MIT",
     author="Peter Melchior",
     author_email="peter.m.melchior@gmail.com",
-    url="https://github.com/pmelchior/spectrum-encoder",
+    url="https://github.com/pmelchior/spender",
     packages=["spender", "spender.data"],
     package_data={"skymapper.data": ['*.txt']},
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: MIT License",
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
```

### Comparing `spender-0.1/spender/data/sdss.py` & `spender-0.2/spender/data/sdss.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,32 @@
-import glob, os, urllib.request
+import glob
+import os
+import urllib.request
+from functools import partial
+
+import astropy.io.fits as fits
+import astropy.table as aTable
 import numpy as np
 import torch
+import pickle
 from torch.utils.data import DataLoader
-from torchinterp1d import Interp1d
-import astropy.io.fits as fits
-import astropy.table as aTable
-from functools import partial
+from torchinterp1d import interp1d
 
 from ..instrument import Instrument, get_skyline_mask
 from ..util import BatchedFilesDataset, load_batch
 
+
 class SDSS(Instrument):
     """SDSS instrument
 
     Implements basic parameterization of the SDSS-II spectrograph as well as functions
     to download and organize the spectra from the DR16 data archive.
     """
-    _wave_obs = 10**torch.arange(3.578, 3.97, 0.0001)
+
+    _wave_obs = 10 ** torch.arange(3.578, 3.97, 0.0001)
     _skyline_mask = get_skyline_mask(_wave_obs)
     _base_url = "https://data.sdss.org/sas/dr16/sdss/spectro/redux/26/spectra/lite/"
 
     def __init__(self, lsf=None, calibration=None):
         """Create instrument
 
         Parameters
@@ -29,15 +35,23 @@
             (optional) Line spread function model
         calibration: callable
             (optional) function to calibrate the observed spectrum
         """
         super().__init__(SDSS._wave_obs, lsf=lsf, calibration=calibration)
 
     @classmethod
-    def get_data_loader(cls, dir, which=None, tag=None, batch_size=1024, shuffle=False, shuffle_instance=False):
+    def get_data_loader(
+        cls,
+        dir,
+        which=None,
+        tag=None,
+        batch_size=1024,
+        shuffle=False,
+        shuffle_instance=False,
+    ):
         """Get a dataloader for batches of spectra
 
         Parameters
         ----------
         dir: string
             Root directory for data storage
         which: ['train', 'valid', 'test'] or None
@@ -53,19 +67,21 @@
 
         Returns
         -------
         :class:`torch.utils.data.DataLoader`
         """
         files = cls.list_batches(dir, which=which, tag=tag)
         if which in ["train", "valid"]:
-            subset = slice(0,3)
+            subset = slice(0, 3)
         else:
             subset = None
         load_fct = partial(load_batch, subset=subset)
-        data = BatchedFilesDataset(files, load_fct, shuffle=shuffle, shuffle_instance=shuffle_instance)
+        data = BatchedFilesDataset(
+            files, load_fct, shuffle=shuffle, shuffle_instance=shuffle_instance
+        )
         return DataLoader(data, batch_size=batch_size)
 
     @classmethod
     def list_batches(cls, dir, which=None, tag=None):
         """List all batch files
 
         Parameters
@@ -78,29 +94,33 @@
             Name to specify which batch files to load
 
         Returns
         -------
         list of filepaths
         """
         if tag is None:
-            tag = "chunk1024"
+            tag = "variable"
         classname = cls.__mro__[0].__name__
         filename = f"{classname}{tag}_*.pkl"
         batch_files = glob.glob(dir + "/" + filename)
         batches = [item for item in batch_files if not "copy" in item]
 
         NBATCH = len(batches)
-        train_batches = batches[:int(0.7*NBATCH)]
-        valid_batches = batches[int(0.7*NBATCH):int(0.85*NBATCH)]
-        test_batches = batches[int(0.85*NBATCH):]
-
-        if which == "test": return test_batches
-        elif which == "valid": return valid_batches
-        elif which == "train": return train_batches
-        else: return batches
+        train_batches = batches[: int(0.7 * NBATCH)]
+        valid_batches = batches[int(0.7 * NBATCH) : int(0.85 * NBATCH)]
+        test_batches = batches[int(0.85 * NBATCH) :]
+
+        if which == "test":
+            return test_batches
+        elif which == "valid":
+            return valid_batches
+        elif which == "train":
+            return train_batches
+        else:
+            return batches
 
     @classmethod
     def save_batch(cls, dir, batch, tag=None, counter=None):
         """Save batch into a pickled file
 
         Parameters
         ----------
@@ -121,15 +141,15 @@
         if tag is None:
             tag = f"chunk{len(batch)}"
         if counter is None:
             counter = ""
         classname = cls.__mro__[0].__name__
         filename = os.path.join(dir, f"{classname}{tag}_{counter}.pkl")
 
-        with open(filename, 'wb') as f:
+        with open(filename, "wb") as f:
             pickle.dump(batch, f)
 
     @classmethod
     def save_in_batches(cls, dir, ids, tag=None, batch_size=1024):
         """Save all spectra for given ids into batch files
 
         Parameters
@@ -148,15 +168,15 @@
         None
 
         """
         N = len(ids)
         idx = np.arange(0, N, batch_size)
         batches = np.array_split(ids, idx[1:])
         for counter, ids_ in zip(idx, batches):
-            print (f"saving batch {counter} / {N}")
+            print(f"saving batch {counter} / {N}")
             batch = cls.make_batch(dir, ids_)
             cls.save_batch(dir, batch, tag=tag, counter=counter)
 
     @classmethod
     def get_spectrum(cls, dir, plate, mjd, fiberid, return_file=False):
         """Download and prepare spectrum for analysis
 
@@ -174,17 +194,21 @@
             Whether to return the local file name or the prepared spectrum
 
         Returns
         -------
         Either the local file name or the prepared spectrum
         """
 
-        filename = "spec-%s-%i-%s.fits" % (str(plate).zfill(4), mjd, str(fiberid).zfill(4))
-        classname = cls.__mro__[0].__name__.lower()
-        dirname = os.path.join(dir, f"{classname}-spectra")
+        plate, mjd, fiberid = [int(i) for i in [plate, mjd, fiberid]]
+        filename = "spec-%s-%i-%s.fits" % (
+            str(plate).zfill(4),
+            mjd,
+            str(fiberid).zfill(4),
+        )
+        dirname = os.path.join(dir, str(plate).zfill(4))
         flocal = os.path.join(dirname, filename)
         if not os.path.isfile(flocal):
             os.makedirs(dirname, exist_ok=True)
             url = "%s/%s/%s" % (cls._base_url, str(plate).zfill(4), filename)
             print(f"downloading {url}")
             urllib.request.urlretrieve(url, flocal)
 
@@ -209,284 +233,334 @@
         return_file: bool
             Whether to return the local file name or actual image
 
         Returns
         -------
         Either the local file name or :class:`IPython.display.Image`
         """
-        filename = "im-%s-%i-%s.jpeg" % (str(plate).zfill(4), mjd, str(fiberid).zfill(4))
+        filename = "im-%s-%i-%s.jpeg" % (
+            str(plate).zfill(4),
+            mjd,
+            str(fiberid).zfill(4),
+        )
         dirname = os.path.join(dir, "sdss-images")
         flocal = os.path.join(dirname, filename)
         if not os.path.isfile(flocal):
             os.makedirs(dirname, exist_ok=True)
             # get RA/DEC from spectrum file
             specname = cls.get_spectrum(dir, plate, mjd, fiberid, return_file=True)
             hdulist = fits.open(specname)
             specinfo = hdulist[2].data[0]
-            ra, dec = specinfo['PLUG_RA'], specinfo['PLUG_DEC']
+            ra, dec = specinfo["PLUG_RA"], specinfo["PLUG_DEC"]
             # query skyserver cutout service
             print(f"downloading image at {ra}/{dec}")
             image_url = "https://skyserver.sdss.org/dr16/SkyServerWS/ImgCutout/getjpeg"
-            scale, size, opt = 0.2, 256, "S" # "S" = outline of fiber
-            params = {"ra":ra, "dec":dec, "scale": scale,
-                      "height": size, "width": size, "opt": opt}
-            url = image_url + "?" + "&".join('='.join((key,str(val))) for (key,val) in params.items())
+            scale, size, opt = 0.2, 256, "S"  # "S" = outline of fiber
+            params = {
+                "ra": ra,
+                "dec": dec,
+                "scale": scale,
+                "height": size,
+                "width": size,
+                "opt": opt,
+            }
+            url = (
+                image_url
+                + "?"
+                + "&".join("=".join((key, str(val))) for (key, val) in params.items())
+            )
             urllib.request.urlretrieve(url, flocal)
 
         if return_file:
             return flocal
 
         from IPython import display
+
         return display.Image(flocal)
 
     @classmethod
-    def prepare_spectrum(cls, filename):
+    def prepare_spectrum(cls, filename, z=None):
         """Prepare spectrum for analysis
 
         This method creates an extended mask, using the original SDSS `and_mask` and
         the skyline mask of the instrument. The weights for all masked regions is set to
         0, but the spectrum itself is not altered.
 
         The spectrum and weights are then cast into a fixed-format data vector, which
         standardizes the variable wavelengths of each observation.
 
         A normalization is computed as the median flux in the relatively flat region
-        between 5300 and 5850 A. The spectrum is divided by this factor, the weights
+        between restframe 5300 and 5850 A. The spectrum is divided by this factor, the weights
         are muliplied with the square of this factor.
 
-        Redshift estimate and errors as determined by the SDSS pipeline are read from
-        the file headers.
-
         Parameter
         ---------
         filename: string
-            Path to local file containing the spetrum
+            Path to local file containing the spectrum
+        z: float or None
+            Redshift of the spectrum
+            If None, redshift and its error will be read from the file and returned
 
         Returns
         -------
         spec: `torch.tensor`, shape (L, )
             Normalized spectrum
         w: `torch.tensor`, shape (L, )
             Inverse variance weights of normalized spectrum
-        z: `torch.tensor`, shape (1, )
-            Redshift from SDSS pipeline
-        id: `torch.tensor`, shape (3, )
-            SDSS plate, mjd, fiberid triple
         norm: `torch.tensor`, shape (1, )
-            Normalization factor
-        zerr: torch.tensor`, shape (1, )
-            Redshift error from SDSS pipeline
+            Flux normalization factor
+        z: `torch.tensor`, shape (1, )
+            Redshift (only returned when argument z=None)
+        zerr: `torch.tensor`, shape (1, )
+            Redshift error (only returned when argument z=None)
         """
         hdulist = fits.open(filename)
         data = hdulist[1].data
-        loglam = data['loglam']
-        flux = data['flux']
-        ivar = data['ivar']
+        loglam = data["loglam"]
+        flux = data["flux"]
+        ivar = data["ivar"]
 
         # apply bitmask, remove small values
-        mask = data['and_mask'].astype(bool) | (ivar <= 1e-6)
+        mask = data["and_mask"].astype(bool) | (ivar <= 1e-6)
         ivar[mask] = 0
 
         # loglam is subset of _wave_obs, need to insert into extended tensor
         L = len(cls._wave_obs)
         start = int(np.around((loglam[0] - torch.log10(cls._wave_obs[0]).item())/0.0001))
-        end = min(start+len(loglam), L)
+        if start<0:
+            flux = flux[-start:]
+            ivar = ivar[-start:]
+            end = min(start+len(loglam), L)
+            start = 0
+        else:
+            end = min(start+len(loglam), L)
         spec = torch.zeros(L)
         w = torch.zeros(L)
-         # explicit type conversion to float32 to get to little endian
+        # explicit type conversion to float32 to get to little endian
         spec[start:end]  = torch.from_numpy(flux.astype(np.float32))
         w[start:end] = torch.from_numpy(ivar.astype(np.float32))
 
         # remove regions around skylines
         w[cls._skyline_mask] = 0
 
-        # get plate, mjd, fiberid info
-        specinfo = hdulist[2].data[0]
-        id = torch.tensor((specinfo['PLATE'], specinfo['MJD'], specinfo['FIBERID']), dtype=torch.int)
-
-        # get redshift and error
-        z = torch.tensor(specinfo['Z'])
-        zerr = torch.tensor(specinfo['Z_ERR'])
+        extended_return = False
+        if z is None:
+            # get plate, mjd, fiberid info
+            specinfo = hdulist[2].data[0]
+            # get redshift and error
+            z = torch.tensor(specinfo["Z"])
+            zerr = torch.tensor(specinfo["Z_ERR"])
+            extended_return = True
 
         # normalize spectrum:
         # for redshift invariant encoder: select norm window in restframe
         wave_rest = cls._wave_obs / (1 + z)
         # flatish region that is well observed out to z ~ 0.5
         sel = (w > 0) & (wave_rest > 5300) & (wave_rest < 5850)
-        norm = torch.median(spec[sel])
+        if sel.count_nonzero() == 0: norm = torch.tensor(0)
+        else: norm = torch.median(spec[sel])
         # remove spectra (from training) for which no valid norm could be found
         if not torch.isfinite(norm):
             norm = 0
         else:
             spec /= norm
         w *= norm**2
 
-        return spec, w, z, id, norm, zerr
-
+        if extended_return:
+            return spec, w, norm, z, zerr
+        return spec, w, norm
+    
     @classmethod
-    def make_batch(cls, dir, ids):
+    def make_batch(cls, dir, fields):
         """Make a batch of spectra from their IDs
 
         Parameters
         ----------
         dir: string
             Root directory for data storage
-        ids: list of (plate, mjd, fiberid)
-            Identifier of spectrum
+        fields: list of (plate, mjd, fiberid, [z, z_err])
+            List of object qualifiers from query()
 
         Returns
         -------
         spec: `torch.tensor`, shape (N, L)
             Normalized spectrum
         w: `torch.tensor`, shape (N, L)
             Inverse variance weights of normalized spectrum
         z: `torch.tensor`, shape (N, )
             Redshift from SDSS pipeline
-        id: `torch.tensor`, shape (N, 3)
-            SDSS plate, mjd, fiberid triple
         norm: `torch.tensor`, shape (N, )
             Normalization factor
         zerr: torch.tensor`, shape (N, )
             Redshift error from SDSS pipeline
         """
 
-        files = [ cls.get_spectrum(dir, plate, mjd, fiberid, return_file=True) for plate, mjd, fiberid in ids ]
-        N = len(files)
+        N = len(fields)
         L = len(cls._wave_obs)
         spec = torch.empty((N, L))
         w = torch.empty((N, L))
         z = torch.empty(N)
         id = torch.empty((N, 3), dtype=torch.int)
         norm = torch.empty(N)
         zerr = torch.empty(N)
-        for i, f in enumerate(files):
-            spec[i], w[i], z[i], id[i], norm[i], zerr[i] = cls.prepare_spectrum(f)
-        return spec, w, z, id, norm, zerr
+        for i in range(N):
+            if len(fields[i]) == 5:
+                plate, mjd, fiberid, z_, zerr_ = fields[i]
+                f = cls.get_spectrum(dir, plate, mjd, fiberid, return_file=True)
+                spec[i], w[i], norm[i] = cls.prepare_spectrum(f, z_)
+                z[i], zerr[i] = z_, zerr_
+            elif len(fields[i]) == 3:
+                plate, mjd, fiberid = fields[i]
+                f = cls.get_spectrum(dir, plate, mjd, fiberid, return_file=True)
+                spec[i], w[i], norm[i], z[i], zerr[i] = cls.prepare_spectrum(f)
+            else:
+                raise AttributeError("fields must contain (plate, mjd, fiberid, z, z_err) or (plate, mjd, fiberid)")
+            id[i] = torch.tensor((plate, mjd, fiberid), dtype=torch.int)
+        return spec, w, z, norm, zerr
 
     @classmethod
-    def get_ids(cls, dir, selection_fct=None):
-        """Select IDs from main specrum table that matches `selection_fct`
+    def query(cls, dir, fields=["PLATE", "MJD", "FIBERID", "Z", "Z_ERR"], selection_fct=None):
+        """Select fields from main specrum table for objects that match `selection_fct`
 
         NOTE: This function will download the file `specObj-dr16.fits` from the data
         archive. This file is *not* small...
 
         Parameters
         ----------
         dir: string
             Root directory for data storage
+        fields: list of string
+            Catalog field names to return
         selection_fct: callable
             Function to select matches from all items in the main table
 
         Returns
         -------
-        ids: `torch.tensor`, shape (N, 3)
-            SDSS plate, mjd, fiberid triple
+        fields: `torch.tensor`, shape (N, F)
+            Tensor of fields for the selected objects
 
         """
         main_file = os.path.join(dir, "specObj-dr16.fits")
         if not os.path.isfile(main_file):
             url = "https://data.sdss.org/sas/dr16/sdss/spectro/redux/specObj-dr16.fits"
-            print (f"downloading {url}, this will take a while...")
+            print(f"downloading {url}, this will take a while...")
             urllib.request.urlretrieve(url, main_file)
 
         print(f"opening {main_file}")
         specobj = aTable.Table.read(main_file)
 
         if selection_fct is None:
             # apply default selections
             classname = cls.__mro__[0].__name__.lower()
-            sel = ((specobj['SURVEY'] == f'{classname}  ') & # SDSS survey
-                    (specobj['PLATEQUALITY'] == 'good    ') &
-                    (specobj['TARGETTYPE'] == 'SCIENCE ')
-                   )
-            sel &= ((specobj['Z'] > 0.) & (specobj['Z_ERR'] < 1e-4))
-            sel &= ((specobj['SOURCETYPE'] == 'GALAXY                   ') &
-                         (specobj['CLASS'] == 'GALAXY'))
+            sel = (
+                (specobj["SURVEY"] == f"{classname}  ")
+                & (specobj["PLATEQUALITY"] == "good    ")  # SDSS survey
+                & (specobj["TARGETTYPE"] == "SCIENCE ")
+            )
+            sel &= (specobj["Z"] > 0.0) & (specobj["Z_ERR"] < 1e-4)
+            sel &= (specobj["SOURCETYPE"] == "GALAXY                   ") & (
+                specobj["CLASS"] == "GALAXY"
+            )
         else:
             sel = selection_fct(specobj)
 
-        plate = specobj['PLATE'][sel]
-        mjd = specobj['MJD'][sel]
-        fiberid = specobj['FIBERID'][sel]
-        return tuple(zip(plate, mjd, fiberid))
+        return specobj[fields][sel]
 
     @classmethod
-    def augment_spectra(cls, batch, redshift=True, noise=True, mask=True, ratio=0.05):
+    def augment_spectra(cls, batch, redshift=True, noise=True, mask=True, ratio=0.05, z_new=None):
         """Augment spectra for greater diversity
 
         Parameters
         ----------
         batch: `torch.tensor`, shape (N, L)
             Spectrum batch
         redshift: bool
             Modify redshift by up to 0.2 (keeping it within 0...0.5)
         noise: bool
             Whether to add noise to the spectrum (up to 0.2*max(spectrum))
         mask: bool
             Whether to block out a fraction (given by `ratio`) of the spectrum
+        ratio: float
+            Fraction of the spectrum that will be masked
+        z_new: float
+            Adopt this redshift for all spectra in the batch
 
         Returns
         -------
         spec: `torch.tensor`, shape (N, L)
             Altered spectrum
         w: `torch.tensor`, shape (N, L)
             Altered inverse variance weights of spectrum
         z: `torch.tensor`, shape (N, )
             Altered redshift
         """
+
         spec, w, z = batch[:3]
         batch_size, spec_size = spec.shape
         device = spec.device
         wave_obs = cls._wave_obs.to(device)
 
         if redshift:
-            # uniform distribution of redshift offsets, width = z_lim
-            z_lim = 0.2
-            z_base = torch.relu(z-z_lim)
-            z_new = z_base+z_lim*(torch.rand(batch_size, device=device))
+            if z_new == None:
+                # uniform distribution of redshift offsets, width = z_lim
+                z_lim = 0.5
+                z_base = torch.relu(z-z_lim)
+                z_new = z_base+z_lim*(torch.rand(batch_size, device=device))
             # keep redshifts between 0 and 0.5
-            z_new = torch.minimum(torch.nn.functional.relu(z_new), 0.5 * torch.ones(batch_size, device=device))
-            zfactor = ((1 + z_new)/(1 + z))
+            z_new = torch.minimum(
+                torch.nn.functional.relu(z_new),
+                0.5 * torch.ones(batch_size, device=device),
+            )
+            zfactor = (1 + z_new) / (1 + z)
             wave_redshifted = (wave_obs.unsqueeze(1) * zfactor).T
 
             # redshift linear interpolation
-            spec_new = Interp1d()(wave_redshifted, spec, wave_obs)
+            spec_new = interp1d(wave_redshifted, spec, wave_obs)
             # ensure extrapolated values have zero weights
             w_new = torch.clone(w)
-            w_new[:,0] = 0
-            w_new[:,-1] = 0
-            w_new = Interp1d()(wave_redshifted, w_new, wave_obs)
+            w_new[:, 0] = 0
+            w_new[:, -1] = 0
+            w_new = interp1d(wave_redshifted, w_new, wave_obs)
             w_new = torch.nn.functional.relu(w_new)
         else:
             spec_new, w_new, z_new = torch.clone(spec), torch.clone(w), z
 
         # add noise
         if noise:
             sigma = 0.2 * torch.max(spec, 1, keepdim=True)[0]
-            noise = sigma * torch.distributions.Normal(0, 1).sample(spec.shape).to(device)
-            noise_mask = torch.distributions.Uniform(0, 1).sample(spec.shape).to(device)>ratio
-            noise[noise_mask]=0
+            noise = sigma * torch.distributions.Normal(0, 1).sample(spec.shape).to(
+                device
+            )
+            noise_mask = (
+                torch.distributions.Uniform(0, 1).sample(spec.shape).to(device) > ratio
+            )
+            noise[noise_mask] = 0
             spec_new += noise
             # add variance in quadrature, avoid division by 0
-            w_new = 1/(1/(w_new + 1e-6) + noise**2)
+            w_new = 1 / (1 / (w_new + 1e-6) + noise**2)
 
         if mask:
             length = int(spec_size * ratio)
-            start = torch.randint(0, spec_size-length, (1,)).item()
-            spec_new[:, start:start+length] = 0
-            w_new[:, start:start+length] = 0
+            start = torch.randint(0, spec_size - length, (1,)).item()
+            spec_new[:, start : start + length] = 0
+            w_new[:, start : start + length] = 0
 
         return spec_new, w_new, z_new
 
 
 class BOSS(SDSS):
     """BOSS instrument
 
     This is a variant of :class:`SDSS` with a different observed wavelength vector and
     data archive URL.
     """
-    _wave_obs = 10**torch.arange(3.549, 4.0175, 0.0001)
+
+    _wave_obs = 10 ** torch.arange(3.549, 4.0175, 0.0001)
     _skyline_mask = get_skyline_mask(_wave_obs)
-    _base_url = "https://data.sdss.org/sas/dr16/eboss/spectro/redux/v5_13_0/spectra/lite/"
+    _base_url = (
+        "https://data.sdss.org/sas/dr16/eboss/spectro/redux/v5_13_0/spectra/lite/"
+    )
 
     def __init__(self, lsf=None, calibration=None):
-        super(Instrument, self).__init__(BOSS._wave_obs, lsf=lsf, calibration=calibration)
+        super(Instrument, self).__init__(
+            BOSS._wave_obs, lsf=lsf, calibration=calibration
+        )
```

### Comparing `spender-0.1/spender/instrument.py` & `spender-0.2/spender/instrument.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-import torch, os
+import os
+
 import numpy as np
+import torch
 from torch import nn
-from torchinterp1d import Interp1d
+
 
 class BaseInstrument(nn.Module):
     """Base class for instruments
 
     Container for wavelength vector, LSF and calibration functions.
 
     CAUTION:
@@ -16,49 +18,55 @@
     wave_obs: `torch.tensor`
         Observed wavelengths
     lsf: :class:`LSF`
         (optional) Line spread function model
     calibration: callable
         (optional) function to calibrate the observed spectrum
     """
-    def __init__(self,
-                 wave_obs,
-                 lsf=None,
-                 calibration=None,
-                ):
+
+    def __init__(
+        self,
+        wave_obs,
+        lsf=None,
+        calibration=None,
+    ):
 
         super(BaseInstrument, self).__init__()
 
         self.calibration = calibration
         if lsf is not None:
             assert isinstance(lsf, (LSF, torch.Tensor))
             if isinstance(lsf, LSF):
                 self.lsf = lsf
             else:
                 self.lsf = LSF(lsf)
         else:
             self.lsf = None
 
         # register wavelength tensors on the same device as the entire model
-        self.register_buffer('wave_obs', wave_obs)
+        self.register_buffer("wave_obs", wave_obs)
 
     @property
     def name(self):
         return self.__class__.__name__
 
+
 class LSF(nn.Conv1d):
     def __init__(self, kernel, requires_grad=True):
-        super(LSF, self).__init__(1, 1, len(kernel), bias=False, padding='same')
+        super(LSF, self).__init__(1, 1, len(kernel), bias=False, padding="same")
         # if LSF should be fit, set `requires_grad=True`
-        self.weight = nn.Parameter(kernel.flip(0).reshape(1,1,-1), requires_grad=requires_grad)
+        self.weight = nn.Parameter(
+            kernel.flip(0).reshape(1, 1, -1), requires_grad=requires_grad
+        )
 
     def forward(self, x):
         # convolution with flux preservation
         return super(LSF, self).forward(x) / self.weight.sum()
 
+
 def get_skyline_mask(wave_obs, min_intensity=2, mask_size=5):
     """Return vector that masks the major skylines
 
     For ever line in the skyline list in the file `data/sky-lines.txt` that is brighter
     than a threshold, this method creates a mask whose size scales logarithmically with
     line brightness.
 
@@ -73,43 +81,54 @@
         is the minmum size for lines with `min_intensity`.
     Returns
     -------
     mask, `torch.tensor` of dtype `bool` with same shape as `wave_obs`
     """
     this_dir, this_filename = os.path.split(__file__)
     filename = os.path.join(this_dir, "data", "sky-lines.txt")
-    skylines = np.genfromtxt(filename, names=['wavelength', 'intensity', 'name', 'status'], dtype=None, encoding=None)
+    skylines = np.genfromtxt(
+        filename,
+        names=["wavelength", "intensity", "name", "status"],
+        dtype=None,
+        encoding=None,
+    )
     # wavelength in nm, need A
-    skylines['wavelength'] *= 10
+    skylines["wavelength"] *= 10
 
     mask = torch.zeros(len(wave_obs), dtype=torch.bool)
-    for line in skylines[skylines['intensity'] > min_intensity]:
+    for line in skylines[skylines["intensity"] > min_intensity]:
         # increase masking area with intensity
-        mask_size_ = mask_size * (1 + np.log10(line['intensity'] / min_intensity))
-        mask |= (wave_obs - line['wavelength']).abs() <  mask_size_
+        mask_size_ = mask_size * (1 + np.log10(line["intensity"] / min_intensity))
+        mask |= (wave_obs - line["wavelength"]).abs() < mask_size_
     return mask
 
+
 # allow registry of new instruments
 # see https://effectivepython.com/2015/02/02/register-class-existence-with-metaclasses
 instrument_register = {}
 
+
 def register_class(target_class):
     instrument_register[target_class.__name__] = target_class
 
+
 class Meta(type):
     """Meta class to enable registration of instruments"""
+
     def __new__(meta, name, bases, class_dict):
         cls = type.__new__(meta, name, bases, class_dict)
         # remove those that are directly derived from the base class
         if BaseInstrument not in bases:
             register_class(cls)
         return cls
 
+
 class Instrument(BaseInstrument, metaclass=Meta):
     """Instrument class
 
     Container for wavelength vector, LSF and calibration functions.
 
     See `spender.instrument.instrument_register` for all known classes that derive from
     :class:`Instrument`.
     """
+
     pass
```

### Comparing `spender-0.1/spender/model.py` & `spender-0.2/spender/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import numpy as np
 import torch
 from torch import nn
-from torchinterp1d import Interp1d
+from torchinterp1d import interp1d
+
 
 class MLP(nn.Sequential):
     """Multi-Layer Perceptron
 
     A simple implementation with a configurable number of hidden layers and
     activation functions.
 
@@ -19,31 +19,29 @@
         Dimensions for every hidden layer
     act: list of callables
         Activation functions after every layer. Needs to have len(n_hidden) + 1
         If `None`, will be set to `LeakyReLU` for every layer.
     dropout: float
         Dropout probability
     """
-    def __init__(self,
-                 n_in,
-                 n_out,
-                 n_hidden=(16, 16, 16),
-                 act=None,
-                 dropout=0):
+
+    def __init__(self, n_in, n_out, n_hidden=(16, 16, 16), act=None, dropout=0):
 
         if act is None:
-            act = [ nn.LeakyReLU(), ] * (len(n_hidden) + 1)
+            act = [
+                nn.LeakyReLU(),
+            ] * (len(n_hidden) + 1)
         assert len(act) == len(n_hidden) + 1
 
         layer = []
         n_ = [n_in, *n_hidden, n_out]
-        for i in range(len(n_)-1):
-                layer.append(nn.Linear(n_[i], n_[i+1]))
-                layer.append(act[i])
-                layer.append(nn.Dropout(p=dropout))
+        for i in range(len(n_) - 1):
+            layer.append(nn.Linear(n_[i], n_[i + 1]))
+            layer.append(act[i])
+            layer.append(nn.Dropout(p=dropout))
 
         super(MLP, self).__init__(*layer)
 
 
 class SpeculatorActivation(nn.Module):
     """Activation function from the Speculator paper
 
@@ -56,14 +54,15 @@
     Parameters
     ----------
     n_parameter: int
         Number of parameters for the activation function to act on
     plus_one: bool
         Whether to add 1 to the output
     """
+
     def __init__(self, n_parameter, plus_one=False):
         super().__init__()
         self.plus_one = plus_one
         self.beta = nn.Parameter(torch.randn(n_parameter), requires_grad=True)
         self.gamma = nn.Parameter(torch.randn(n_parameter), requires_grad=True)
 
     def forward(self, x):
@@ -79,14 +78,15 @@
         """
         # eq 8 in Alsing+2020
         x = (self.gamma + (1 - self.gamma) * torch.sigmoid(self.beta * x)) * x
         if self.plus_one:
             return x + 1
         return x
 
+
 class SpectrumEncoder(nn.Module):
     """Spectrum encoder
 
     Modified version of the encoder by Serrà et al. (2018), which combines a 3 layer CNN
     with a dot-product attention module. This encoder adds a MLP to further compress the
     attended values into a low-dimensional latent space.
 
@@ -99,61 +99,59 @@
     n_latent: int
         Dimension of latent space
     n_hidden: list of int
         Dimensions for every hidden layer of the :class:`MLP`
     act: list of callables
         Activation functions after every layer. Needs to have len(n_hidden) + 1
         If `None`, will be set to `LeakyReLU` for every layer.
-    n_aux: int
-        Dimensions of auxiliary inputs for the :class:`MLP`
     dropout: float
         Dropout probability
     """
-    def __init__(self,
-                 instrument,
-                 n_latent,
-                 n_hidden=(128, 64, 32),
-                 act=None,
-                 n_aux=1,
-                 dropout=0):
+
+    def __init__(
+        self, instrument, n_latent, n_hidden=(128, 64, 32), act=None, dropout=0
+    ):
 
         super(SpectrumEncoder, self).__init__()
         self.instrument = instrument
         self.n_latent = n_latent
-        self.n_aux = n_aux
-
+        
         filters = [128, 256, 512]
         sizes = [5, 11, 21]
-        self.conv1, self.conv2, self.conv3 = self._conv_blocks(filters, sizes, dropout=dropout)
+        self.conv1, self.conv2, self.conv3 = self._conv_blocks(
+            filters, sizes, dropout=dropout
+        )
         self.n_feature = filters[-1] // 2
 
         # pools and softmax work for spectra and weights
-        self.pool1, self.pool2 = tuple(nn.MaxPool1d(s, padding=s//2) for s in sizes[:2])
+        self.pool1, self.pool2 = tuple(
+            nn.MaxPool1d(s, padding=s // 2) for s in sizes[:2]
+        )
         self.softmax = nn.Softmax(dim=-1)
 
-        # small MLP to go from CNN features + aux to latents
+        # small MLP to go from CNN features to latents
         if act is None:
-            act = [ nn.PReLU(n) for n in n_hidden ]
+            act = [nn.PReLU(n) for n in n_hidden]
             # last activation identity to have latents centered around 0
             act.append(nn.Identity())
-        self.mlp = MLP(self.n_feature + n_aux, self.n_latent, n_hidden=n_hidden, act=act, dropout=dropout)
-
+        self.mlp = MLP(self.n_feature, self.n_latent, n_hidden=n_hidden, act=act, dropout=dropout)
 
     def _conv_blocks(self, filters, sizes, dropout=0):
         convs = []
         for i in range(len(filters)):
-            f_in = 1 if i == 0 else filters[i-1]
+            f_in = 1 if i == 0 else filters[i - 1]
             f = filters[i]
             s = sizes[i]
             p = s // 2
-            conv = nn.Conv1d(in_channels=f_in,
-                             out_channels=f,
-                             kernel_size=s,
-                             padding=p,
-                            )
+            conv = nn.Conv1d(
+                in_channels=f_in,
+                out_channels=f,
+                kernel_size=s,
+                padding=p,
+            )
             norm = nn.InstanceNorm1d(f)
             act = nn.PReLU(f)
             drop = nn.Dropout(p=dropout)
             convs.append(nn.Sequential(conv, norm, act, drop))
         return tuple(convs)
 
     def _downsample(self, x):
@@ -164,23 +162,21 @@
         x = self.conv3(x)
         C = x.shape[1] // 2
         # split half channels into attention value and key
         h, a = torch.split(x, [C, C], dim=1)
 
         return h, a
 
-    def forward(self, y, aux=None):
+    def forward(self, y):
         """Forward method
 
         Parameters
         ----------
         y: `torch.tensor`, shape (N, L)
             Batch of observed spectra
-        aux: `torch.tensor`, shape (N, n_aux)
-            (optional) Batch of auxiliary inputs to MLP
 
         Returns
         -------
         s: `torch.tensor`, shape (N, n_latent)
             Batch of latents that encode `spectra`
         """
         # run through CNNs
@@ -192,17 +188,15 @@
         # for Grad-FAM (Feature Activation Map)
         if ~self.training and a.requires_grad == True:
             a.register_hook(self._attention_hook)
 
         # apply attention
         x = torch.sum(h * a, dim=2)
 
-        # redshift depending feature combination to final latents
-        if aux is not None and aux is not False:
-            x = torch.cat((x, aux), dim=-1)
+        # run attended features into MLP for final latents
         x = self.mlp(x)
         return x
 
     @property
     def n_parameters(self):
         """Number of parameters in this model"""
         return sum(p.numel() for p in self.parameters() if p.requires_grad)
@@ -213,18 +207,18 @@
     @property
     def attention_grad(self):
         """Gradient of the attention weights
 
         Factor to compute the importance of attention for Grad-FAM method.
 
         Requires a previous `loss.backward` call for any scalar loss function based on
-        outputs of this classes `forward` method. This functionality is switched off
+        outputs of this class's `forward` method. This functionality is switched off
         during training.
         """
-        if hasattr(self, '_attention_grad'):
+        if hasattr(self, "_attention_grad"):
             return self._attention_grad
         else:
             return None
 
 
 class SpectrumDecoder(nn.Module):
     """Spectrum decoder
@@ -243,40 +237,42 @@
         Dimensions for every hidden layer of the :class:`MLP`
     act: list of callables
         Activation functions after every layer. Needs to have len(n_hidden) + 1
         If `None`, will be set to :class:`SpeculatorActivation` for every layer.
     dropout: float
         Dropout probability
     """
-    def __init__(self,
-                 wave_rest,
-                 n_latent=5,
-                 n_hidden=(64, 256, 1024),
-                 act=None,
-                 dropout=0,
-                ):
+
+    def __init__(
+        self,
+        wave_rest,
+        n_latent=5,
+        n_hidden=(64, 256, 1024),
+        act=None,
+        dropout=0,
+    ):
 
         super(SpectrumDecoder, self).__init__()
 
         if act is None:
-            act = [ SpeculatorActivation(n) for n in n_hidden ]
+            act = [SpeculatorActivation(n) for n in n_hidden]
             act.append(SpeculatorActivation(len(wave_rest), plus_one=True))
 
         self.mlp = MLP(
             n_latent,
             len(wave_rest),
             n_hidden=n_hidden,
             act=act,
             dropout=dropout,
         )
 
         self.n_latent = n_latent
 
         # register wavelength tensors on the same device as the entire model
-        self.register_buffer('wave_rest', wave_rest)
+        self.register_buffer("wave_rest", wave_rest)
 
     def decode(self, s):
         """Decode latents into restframe spectrum
 
         Parameter
         ---------
         s: `torch.tensor`, shape (N, S)
@@ -333,15 +329,15 @@
         wave_redshifted = (self.wave_rest.unsqueeze(1) * (1 + z)).T
 
         if instrument in [False, None]:
             wave_obs = self.wave_rest
         else:
             wave_obs = instrument.wave_obs
 
-        spectrum = Interp1d()(wave_redshifted, x, wave_obs)
+        spectrum = interp1d(wave_redshifted, x, wave_obs)
 
         # convolve with LSF
         if instrument.lsf is not None:
             spectrum = instrument.lsf(spectrum.unsqueeze(1)).squeeze(1)
 
         # apply calibration function to observed spectrum
         if instrument is not None and instrument.calibration is not None:
@@ -368,39 +364,40 @@
     Parameter
     ---------
     encoder: `nn.Module`
         Encoder
     decoder: `nn.Module`
         Decoder
     """
-    def __init__(self,
-                 encoder,
-                 decoder,
-                ):
+
+    def __init__(
+        self,
+        encoder,
+        decoder,
+    ):
 
         super(BaseAutoencoder, self).__init__()
         assert encoder.n_latent == decoder.n_latent
         self.encoder = encoder
         self.decoder = decoder
 
-    def encode(self, y, aux=None):
+    def encode(self, x):
         """Encode from observed spectrum to latents
 
         Parameters
         ----------
         y: `torch.tensor`, shape (N, L)
             Batch of observed spectra
-        aux: `torch.tensor`, shape (N, n_aux)
-            (optional) Batch of auxiliary inputs to MLP
+
         Returns
         -------
         s: `torch.tensor`, shape (N, n_latent)
             Batch of latents that encode `spectra`
         """
-        return self.encoder(y, aux=aux)
+        return self.encoder(x)
 
     def decode(self, s):
         """Decode latents into restframe spectrum
 
         Parameter
         ---------
         s: `torch.tensor`, shape (N, S)
@@ -409,28 +406,26 @@
         Returns
         -------
         x: `torch.tensor`, shape (N, L)
             Batch of restframe spectra
         """
         return self.decoder(s)
 
-    def _forward(self, y, instrument=None, z=None, s=None, aux=None):
+    def _forward(self, y, instrument=None, z=None, s=None):
         if s is None:
-            if aux is None and z is not None:
-                aux = z.unsqueeze(1)
-            s = self.encode(y, aux=aux)
+            s = self.encode(y)
         if instrument is None:
             instrument = self.encoder.instrument
 
         x = self.decode(s)
         y = self.decoder.transform(x, instrument=instrument, z=z)
 
         return s, x, y
 
-    def forward(self, y, instrument=None, z=None, s=None, aux=None):
+    def forward(self, y, instrument=None, z=None, s=None):
         """Forward method
 
         Transforms observed spectra into their reconstruction for a given intrument
         and redshift.
 
         Parameter
         ---------
@@ -439,26 +434,24 @@
         instrument: :class:`spender.Instrument`
             Instrument to generate spectrum for
         z: `torch.tensor`, shape (N, 1)
             Redshifts for each spectrum. When given, `aux` is ignored.
         s: `torch.tensor`, shape (N, S)
             (optional) Batch of latents. When given, encoding is omitted and these
             latents are used instead.
-        aux: `torch.tensor`, shape (N, n_aux)
-            (optional) Batch of auxiliary inputs to encoder MLP
 
         Returns
         -------
         y: `torch.tensor`, shape (N, L)
             Batch of spectra at redshift `z` as observed by `instrument`
         """
-        s, x, y_ = self._forward(y, instrument=instrument, z=z, s=s, aux=aux)
+        s, x, y_ = self._forward(y, instrument=instrument, z=z, s=s)
         return y_
 
-    def loss(self, y, w, instrument=None, z=None, s=None, aux=None, individual=False):
+    def loss(self, y, w, instrument=None, z=None, s=None, individual=False):
         """Weighted MSE loss
 
         Parameter
         --------
         y: `torch.tensor`, shape (N, L)
             Batch of observed spectra
         w: `torch.tensor`, shape (N, L)
@@ -466,24 +459,22 @@
         instrument: :class:`spender.Instrument`
             Instrument to generate spectrum for
         z: `torch.tensor`, shape (N, 1)
             Redshifts for each spectrum. When given, `aux` is ignored.
         s: `torch.tensor`, shape (N, S)
             (optional) Batch of latents. When given, encoding is omitted and these
             latents are used instead.
-        aux: `torch.tensor`, shape (N, n_aux)
-            (optional) Batch of auxiliary inputs to encoder MLP
         individual: bool
             Whether the loss is computed for each spectrum individually or aggregated
 
         Returns
         -------
         float or `torch.tensor`, shape (N,) of weighted MSE loss
         """
-        y_ = self.forward(y, instrument=instrument, z=z, s=s, aux=aux)
+        y_ = self.forward(y, instrument=instrument, z=z, s=s)
         return self._loss(y, w, y_, individual=individual)
 
     def _loss(self, y, w, y_, individual=False):
         # loss = total squared deviation in units of variance
         # if the model is identical to observed spectrum (up to the noise),
         # then loss per object = D (number of non-zero bins)
 
@@ -522,33 +513,31 @@
     ---------
     instrument: :class:`spender.Instrument`
         Observing instrument
     wave_rest: `torch.tensor`
         Restframe wavelengths
     n_latent: int
         Dimension of latent space
-    n_aux: int
-        Dimensions of auxiliary inputs for the encoder :class:`MLP`. Set to 1 to use the
-        redshift as auxiliary.
     n_hidden: list of int
         Dimensions for every hidden layer of the decoder :class:`MLP`
     act: list of callables
         Activation functions for the decoder. Needs to have len(n_hidden) + 1
         If `None`, will be set to `LeakyReLU` for every layer.
     """
-    def __init__(self,
-                 instrument,
-                 wave_rest,
-                 n_latent=10,
-                 n_aux=1,
-                 n_hidden=(64, 256, 1024),
-                 act=None,
-                ):
 
-        encoder = SpectrumEncoder(instrument, n_latent, n_aux=n_aux)
+    def __init__(
+        self,
+        instrument,
+        wave_rest,
+        n_latent=10,
+        n_hidden=(64, 256, 1024),
+        act=None,
+    ):
+
+        encoder = SpectrumEncoder(instrument, n_latent)
 
         decoder = SpectrumDecoder(
             wave_rest,
             n_latent,
             n_hidden=n_hidden,
             act=act,
         )
```

### Comparing `spender-0.1/spender/util.py` & `spender-0.2/spender/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,47 @@
+import io
+import pickle
+import random
+from itertools import chain
+
+import GPUtil
+import humanize
+import psutil
 import torch
-import torch.nn.functional as F
 from torch.utils.data import IterableDataset
-from itertools import chain
-import pickle, humanize, psutil, GPUtil, io, random
-from torchinterp1d import Interp1d
+from torchinterp1d import interp1d
+
 
 ############ Functions for creating batched files ###############
 class CPU_Unpickler(pickle.Unpickler):
     def find_class(self, module, name):
-        if module == 'torch.storage' and name == '_load_from_bytes':
-            return lambda b: torch.load(io.BytesIO(b), map_location='cpu')
-        else: return super().find_class(module, name)
+        if module == "torch.storage" and name == "_load_from_bytes":
+            return lambda b: torch.load(io.BytesIO(b), map_location="cpu")
+        else:
+            return super().find_class(module, name)
+
 
 def load_batch(batch_name, subset=None):
-    with open(batch_name, 'rb') as f:
+    with open(batch_name, "rb") as f:
         if torch.cuda.is_available():
             batch = pickle.load(f)
         else:
             batch = CPU_Unpickler(f).load()
 
     if subset is not None:
         return batch[subset]
     return batch
 
+
 class BatchedFilesDataset(IterableDataset):
     """Creates a dataset from a list of batched files
 
     This class allows the use of batched files, whose size can be optimized for loading
     performance, as input for a :class:`torch.utils.data.DataLoader`, whose batch size
-    can be chosen indepdently to optimize training.
+    can be chosen independently to optimize training.
 
     See https://medium.com/speechmatics/how-to-build-a-streaming-dataloader-with-pytorch-a66dd891d9dd
     for details.
 
     The file list and the items in each loaded file can be shuffled if desired.
 
     Parameters
@@ -43,24 +52,25 @@
         Function to return batch when given filename
     shuffle: bool
         Whether to shuffle the order of the batch files
     shuffle_instance: bool
         Whether to shuffle spectra within each batch
 
     """
+
     def __init__(self, file_list, load_fct, shuffle=False, shuffle_instance=False):
         assert len(file_list), "File list cannot be empty"
         self.file_list = file_list
         self.shuffle = shuffle
         self.shuffle_instance = shuffle_instance
         self.load_fct = load_fct
 
     def process_data(self, idx):
         if self.shuffle:
-            idx = random.randint(0, len(self.file_list) -1)
+            idx = random.randint(0, len(self.file_list) - 1)
         batch_name = self.file_list[idx]
         data = self.load_fct(batch_name)
         data = list(zip(*data))
         if self.shuffle_instance:
             random.shuffle(data)
         for x in data:
             yield x
@@ -72,29 +82,34 @@
         return self.get_stream()
 
     def __len__(self):
         return len(self.file_list)
 
 
 def mem_report():
-    print("CPU RAM Free: " + humanize.naturalsize( psutil.virtual_memory().available ))
+    print("CPU RAM Free: " + humanize.naturalsize(psutil.virtual_memory().available))
 
-    if torch.cuda.device_count() ==0: return
+    if torch.cuda.device_count() == 0:
+        return
 
     GPUs = GPUtil.getGPUs()
     for i, gpu in enumerate(GPUs):
-        print('GPU {:d} ... Mem Free: {:.0f}MB / {:.0f}MB | Utilization {:3.0f}%'.format(i, gpu.memoryFree, gpu.memoryTotal, gpu.memoryUtil*100))
+        print(
+            "GPU {:d} ... Mem Free: {:.0f}MB / {:.0f}MB | Utilization {:3.0f}%".format(
+                i, gpu.memoryFree, gpu.memoryTotal, gpu.memoryUtil * 100
+            )
+        )
     return
 
 
-def resample_to_restframe(wave_obs,wave_rest,y,w,z):
-    wave_z = (wave_rest.unsqueeze(1)*(1 + z)).T
-    wave_obs = wave_obs.repeat(y.shape[0],1)
+def resample_to_restframe(wave_obs, wave_rest, y, w, z):
+    wave_z = (wave_rest.unsqueeze(1) * (1 + z)).T
+    wave_obs = wave_obs.repeat(y.shape[0], 1)
     # resample observed spectra to restframe
-    yrest = Interp1d()(wave_obs, y, wave_z)
-    wrest =  Interp1d()(wave_obs, w, wave_z)
+    yrest = interp1d(wave_obs, y, wave_z)
+    wrest = interp1d(wave_obs, w, wave_z)
 
     # interpolation = extrapolation outside of observed region, need to mask
-    msk = (wave_z<=wave_obs.min())|(wave_z>=wave_obs.max())
+    msk = (wave_z <= wave_obs.min()) | (wave_z >= wave_obs.max())
     # yrest[msk]=0 # not needed because all spectral elements are weighted
-    wrest[msk]=0
-    return yrest,wrest
+    wrest[msk] = 0
+    return yrest, wrest
```

