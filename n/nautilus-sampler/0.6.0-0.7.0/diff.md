# Comparing `tmp/nautilus-sampler-0.6.0.tar.gz` & `tmp/nautilus-sampler-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautilus-sampler-0.6.0.tar", last modified: Sat Apr 22 16:59:35 2023, max compression
+gzip compressed data, was "nautilus-sampler-0.7.0.tar", last modified: Tue Jun 20 17:39:24 2023, max compression
```

## Comparing `nautilus-sampler-0.6.0.tar` & `nautilus-sampler-0.7.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     7214 2023-04-22 16:20:51.042005 nautilus-sampler-0.6.0/CHANGELOG.md
--rw-r--r--   0        0        0     1074 2022-09-13 17:16:29.198585 nautilus-sampler-0.6.0/LICENSE
--rw-r--r--   0        0        0     2328 2023-04-08 15:51:59.349856 nautilus-sampler-0.6.0/README.md
--rw-r--r--   0        0        0      218 2023-04-22 16:22:04.286320 nautilus-sampler-0.6.0/nautilus/__init__.py
--rw-r--r--   0        0        0      316 2023-04-13 13:59:25.226473 nautilus-sampler-0.6.0/nautilus/bounds/__init__.py
--rw-r--r--   0        0        0    21190 2023-04-17 13:48:20.350706 nautilus-sampler-0.6.0/nautilus/bounds/basic.py
--rw-r--r--   0        0        0    17091 2023-04-21 17:37:12.091755 nautilus-sampler-0.6.0/nautilus/bounds/neural.py
--rw-r--r--   0        0        0    12919 2023-04-18 20:14:08.615652 nautilus-sampler-0.6.0/nautilus/bounds/union.py
--rw-r--r--   0        0        0     5773 2023-04-17 13:39:44.038203 nautilus-sampler-0.6.0/nautilus/neural.py
--rw-r--r--   0        0        0     5967 2023-02-09 20:46:18.826604 nautilus-sampler-0.6.0/nautilus/prior.py
--rw-r--r--   0        0        0    47556 2023-04-17 13:39:44.039203 nautilus-sampler-0.6.0/nautilus/sampler.py
--rw-r--r--   0        0        0      676 2023-02-09 20:46:18.827604 nautilus-sampler-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     3911 2023-04-13 13:59:25.227473 nautilus-sampler-0.6.0/tests/test_blobs.py
--rw-r--r--   0        0        0    13616 2023-04-17 13:48:20.350706 nautilus-sampler-0.6.0/tests/test_bounds.py
--rw-r--r--   0        0        0     5450 2023-04-21 17:36:57.153594 nautilus-sampler-0.6.0/tests/test_io.py
--rw-r--r--   0        0        0      486 2023-04-17 13:39:44.039203 nautilus-sampler-0.6.0/tests/test_neural.py
--rw-r--r--   0        0        0      907 2023-04-13 13:59:25.228473 nautilus-sampler-0.6.0/tests/test_pool.py
--rw-r--r--   0        0        0     3714 2023-02-09 20:46:18.827604 nautilus-sampler-0.6.0/tests/test_prior.py
--rw-r--r--   0        0        0     6064 2023-04-17 13:48:20.350706 nautilus-sampler-0.6.0/tests/test_sampler.py
--rw-r--r--   0        0        0     2929 1970-01-01 00:00:00.000000 nautilus-sampler-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     8542 2023-06-20 17:19:59.212240 nautilus-sampler-0.7.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1074 2022-09-13 17:16:29.198585 nautilus-sampler-0.7.0/LICENSE
+-rw-r--r--   0        0        0     2609 2023-06-04 19:28:22.216277 nautilus-sampler-0.7.0/README.md
+-rw-r--r--   0        0        0      218 2023-06-20 17:20:06.770110 nautilus-sampler-0.7.0/nautilus/__init__.py
+-rw-r--r--   0        0        0      316 2023-04-13 13:59:25.226473 nautilus-sampler-0.7.0/nautilus/bounds/__init__.py
+-rw-r--r--   0        0        0    22429 2023-06-09 12:58:17.902177 nautilus-sampler-0.7.0/nautilus/bounds/basic.py
+-rw-r--r--   0        0        0    17825 2023-06-20 17:18:56.732706 nautilus-sampler-0.7.0/nautilus/bounds/neural.py
+-rw-r--r--   0        0        0    13354 2023-06-20 17:18:56.733706 nautilus-sampler-0.7.0/nautilus/bounds/union.py
+-rw-r--r--   0        0        0     5750 2023-06-09 12:58:17.902177 nautilus-sampler-0.7.0/nautilus/neural.py
+-rw-r--r--   0        0        0     5967 2023-02-09 20:46:18.826604 nautilus-sampler-0.7.0/nautilus/prior.py
+-rw-r--r--   0        0        0    49690 2023-06-20 17:18:56.733706 nautilus-sampler-0.7.0/nautilus/sampler.py
+-rw-r--r--   0        0        0      676 2023-02-09 20:46:18.827604 nautilus-sampler-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3871 2023-05-29 16:06:55.225559 nautilus-sampler-0.7.0/tests/test_blobs.py
+-rw-r--r--   0        0        0    14060 2023-06-20 17:18:56.734706 nautilus-sampler-0.7.0/tests/test_bounds.py
+-rw-r--r--   0        0        0     5647 2023-06-20 17:18:56.734706 nautilus-sampler-0.7.0/tests/test_io.py
+-rw-r--r--   0        0        0      486 2023-04-17 13:39:44.039203 nautilus-sampler-0.7.0/tests/test_neural.py
+-rw-r--r--   0        0        0     1040 2023-06-12 14:24:46.370732 nautilus-sampler-0.7.0/tests/test_pool.py
+-rw-r--r--   0        0        0     3714 2023-02-09 20:46:18.827604 nautilus-sampler-0.7.0/tests/test_prior.py
+-rw-r--r--   0        0        0     7563 2023-06-20 17:18:56.734706 nautilus-sampler-0.7.0/tests/test_sampler.py
+-rw-r--r--   0        0        0     3210 1970-01-01 00:00:00.000000 nautilus-sampler-0.7.0/PKG-INFO
```

### Comparing `nautilus-sampler-0.6.0/CHANGELOG.md` & `nautilus-sampler-0.7.0/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,28 @@
 # Changelog
 
 All notable changes to nautilus will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.7.0] - 2023-06-20
+
+### Changed
+- One can now change whether to discard points in the exploration phase after calling `run` by changing the `discard_exploration` argument of the sampler. To achieve this, information about points in the exploration phase is never dropped. Consequently, the sampler does not create a backup of the end of the exploration stage under "filename_exp.hdf5", anymore.
+- The computational overhead was slightly reduced when new bounds are rejected. Also, the output now specifically mentions when adding a new bound failed because the volume increased.
+- Added the function `sampler.asymptotic_sampling_efficiency` which returns an estimate of the sampling efficiency in the sampling phase.
+
+### Fixed
+- Likelihoods with large plateaus shouldn't crash, anymore.
+- Information updates about bounds are now written during the sampling phase. Previously, if computations were interrupted and restarted during the sampling phase, the volume estimates were noisier than necessary, and some points may have been proposed twice.
+
+### Deprecated
+- The `n_jobs` keyword argument for the sampler has been deprecated. The pool used for likelihood calls is now also used for sampler parallelization, by default. To use independent pools for likelihood calls and sampler calculations, pass a tuple to `pool`.
+
 ## [0.6.0] - 2023-04-22
 
 ### Changed
 - The code now uses the more modern `numpy.random.Generator` framework instead of `numpy.random.RandomState`.
 - Added the keyword arguments `n_points_min` and `split_threshold` to the sampler. Previously, they were not accessible.
 - The default value for `n_points_min` is now the number of dimensions plus 50. Previously, it was hard-coded to be the number of dimensions plus 1.
 - The multi-ellipsoidal decomposition has been tweaked with the goal of reducing computational overhead for high-dimensional problems.
```

### Comparing `nautilus-sampler-0.6.0/LICENSE` & `nautilus-sampler-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nautilus-sampler-0.6.0/README.md` & `nautilus-sampler-0.7.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -34,10 +34,14 @@
 corner.corner(points, weights=np.exp(log_w), labels='abc')
 ```
 
 ## Documentation
 
 You can find the documentation at [nautilus-sampler.readthedocs.io](https://nautilus-sampler.readthedocs.io).
 
+## Attribution
+
+A paper describing nautilus's underlying methods and performance has been submitted for publication. A draft of the paper will be uploaded to arXiv around the end of June 2023. Please cite the paper, once available, if you found nautilus helpful in your research.
+
 ## License
 
 Nautilus is licensed under the MIT License. The logo uses an image from the Illustris Collaboration.
```

### Comparing `nautilus-sampler-0.6.0/nautilus/bounds/basic.py` & `nautilus-sampler-0.7.0/nautilus/bounds/basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -252,30 +252,25 @@
         Natural log of the volume of the ellipsoid.
     rng : numpy.random.Generator
         Determines random number generation.
 
     """
 
     @classmethod
-    def compute(cls, points, enlarge_per_dim=1.1, fast=False,
-                max_iterations=1000, rng=None):
+    def compute(cls, points, enlarge_per_dim=1.1, max_iterations=1000,
+                rng=None):
         """Compute the bound.
 
         Parameters
         ----------
         points : numpy.ndarray with shape (n_points, n_dim)
             A 2-D array where each row represents a point.
         enlarge_per_dim : float, optional
             Along each dimension, the ellipsoid is enlarged by this factor.
             Default is 1.1.
-        fast : bool, optional
-            If True, calculate the bounding ellipsoid from the mean and
-            covariance of the points. If False, the ellipsoid (ignoring
-            `enlarge_per_dim`) is an approximation to a minimum volume
-            enclosing ellipsoid. Default is False.
         max_iterations : int, optional
             Maximum number of iterations before the minimization algorithm for
             the minimum volume enclosing ellipsoid is stopped. Ignored if
             `fast` is True. Default is 1000.
         rng : None or numpy.random.Generator, optional
             Determines random number generation. Default is None.
 
@@ -298,25 +293,17 @@
             raise ValueError(
                 "The 'enlarge_per_dim' factor cannot be smaller than unity.")
 
         if not points.shape[0] > bound.n_dim:
             raise ValueError('Number of points must be larger than number ' +
                              'dimensions.')
 
-        if not fast:
-            with threadpool_limits(limits=1):
-                bound.c, bound.A = minimum_volume_enclosing_ellipsoid(
-                    points, max_iterations=max_iterations)
-        else:
-            bound.c = np.mean(points, axis=0)
-            bound.A = np.linalg.inv(np.atleast_2d(np.cov(
-                points, rowvar=False)))
-            scale = np.amax(np.einsum(
-                '...i,ij,...j', points - bound.c, bound.A, points - bound.c))
-            bound.A /= scale
+        with threadpool_limits(limits=1):
+            bound.c, bound.A = minimum_volume_enclosing_ellipsoid(
+                points, max_iterations=max_iterations)
 
         bound.A /= enlarge_per_dim**2.0
         bound.B = np.linalg.cholesky(np.linalg.inv(bound.A))
         bound.B_inv = np.linalg.inv(bound.B)
         bound.log_v = (np.linalg.slogdet(bound.B)[1] +
                        bound.n_dim * np.log(2.) +
                        bound.n_dim * gammaln(1.5) -
@@ -499,44 +486,83 @@
         bound: UnitCubeEllipsoidMixture
             The bound.
 
         """
         bound = cls()
         bound.n_dim = points.shape[1]
 
-        kwargs = dict(enlarge_per_dim=enlarge_per_dim, max_iterations=100,
+        kwargs = dict(enlarge_per_dim=enlarge_per_dim, max_iterations=1000,
                       rng=rng)
 
-        # First, calculate a bounding ellipsoid along all dimensions.
+        # First, start by sampling all dimensions using an ellipsoid..
         ellipsoid = Ellipsoid.compute(points, **kwargs)
-        ellipsoid_fast = Ellipsoid.compute(points, fast=True, **kwargs)
         bound.dim_cube = np.zeros(bound.n_dim, dtype=bool)
-        # Now, estimate which dimensions have a smaller volume when using the
-        # cube.
-        for dim in range(bound.n_dim):
-            ellipsoid_dim_fast = Ellipsoid.compute(
-                np.delete(points, dim, axis=1), fast=True, **kwargs)
-            if ellipsoid_fast.volume() > ellipsoid_dim_fast.volume():
-                ellipsoid_dim = Ellipsoid.compute(
-                    np.delete(points, dim, axis=1), fast=False, **kwargs)
-                if ellipsoid.volume() > ellipsoid_dim.volume():
-                    bound.dim_cube[dim] = True
 
-        kwargs['max_iterations'] = 1000
+        # Sample dimensions from the unit cube until volume doesn't decrease.
+        while np.sum(~bound.dim_cube) > 1:
+            c = ellipsoid.c
+            A_inv = np.linalg.inv(ellipsoid.A)
+
+            # Start by projecting the current ellipsoid along each dimension to
+            # estimate dropping which dimension is most likely to lead to the
+            # biggest volume reduction.
+            log_v = np.zeros(np.sum(~bound.dim_cube))
+            for i in range(np.sum(~bound.dim_cube)):
+                points_proj = np.delete(points[:, ~bound.dim_cube], i, axis=1)
+                c_proj = np.delete(c, i)
+                A_inv_proj = np.delete(np.delete(A_inv, i, axis=0), i, axis=1)
+                A_proj = np.linalg.inv(A_inv_proj)
+                scale = np.amax(np.einsum('...i,ij,...j', points_proj - c_proj,
+                                A_proj, points_proj - c_proj))
+                A_proj /= scale
+                log_v[i] = np.linalg.slogdet(np.linalg.inv(A_proj))[1]
+
+            dim = np.arange(bound.n_dim)[~bound.dim_cube][np.argmin(log_v)]
+            bound.dim_cube[dim] = True
+            ellipsoid_proj = Ellipsoid.compute(
+                points[:, ~bound.dim_cube], **kwargs)
+
+            if ellipsoid_proj.volume() < ellipsoid.volume():
+                ellipsoid = ellipsoid_proj
+            else:
+                bound.dim_cube[dim] = False
+                break
+
+        # The above algorithm will not necessarily find the optimal combination
+        # of which dimensions to sample from the unit cube. In particular, the
+        # ellipsoid may have a volume larger than the unit cube. If that's the
+        # case, start from the unit cube and add dimensions to sample from
+        # ellipsoids until volume doesn't decrease.
+        if ellipsoid.volume() > 0:
+            ellipsoid = UnitCube.compute(points)
+            bound.dim_cube = np.ones(bound.n_dim, dtype=bool)
+            # Check which dimensions are better sampled from an ellipsoid,
+            # i.e., have smaller volumes.
+            tested = np.zeros(bound.n_dim, dtype=bool)
+            while ~np.all(tested):
+                for dim in np.arange(bound.n_dim)[~tested]:
+                    bound.dim_cube[dim] = False
+                    tested[dim] = True
+                    ellipsoid_test = Ellipsoid.compute(
+                        points[:, ~bound.dim_cube], **kwargs)
+                    if ellipsoid.volume() > ellipsoid_test.volume():
+                        ellipsoid = ellipsoid_test
+                        tested[bound.dim_cube] = False
+                    else:
+                        bound.dim_cube[dim] = True
 
         if np.any(bound.dim_cube):
             bound.cube = UnitCube.compute(np.sum(bound.dim_cube), rng=rng)
         else:
             bound.cube = None
 
         if np.all(bound.dim_cube):
             bound.ellipsoid = None
         else:
-            bound.ellipsoid = Ellipsoid.compute(
-                points[:, np.arange(bound.n_dim)[~bound.dim_cube]], **kwargs)
+            bound.ellipsoid = ellipsoid
 
         return bound
 
     def transform(self, points):
         """Transform points into the frame of the cube-ellipsoid mixture.
 
         Along dimensions where the boundary is not defined via the unit range,
```

### Comparing `nautilus-sampler-0.6.0/nautilus/bounds/neural.py` & `nautilus-sampler-0.7.0/nautilus/bounds/neural.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         bound.n_dim = points.shape[1]
 
         if rng is None:
             rng = np.random.default_rng()
 
         # Determine the outer bound.
         bound.outer_bound = Ellipsoid.compute(
-            points[log_l > log_l_min], enlarge_per_dim=enlarge_per_dim,
+            points[log_l >= log_l_min], enlarge_per_dim=enlarge_per_dim,
             rng=rng)
 
         if n_networks == 0:
             bound.emulator = None
             bound.score_predict_min = 0
             return bound
 
@@ -262,15 +262,15 @@
             bound.neural_bounds.append(NeuralBound.compute(
                 points[select], log_l[select], log_l_min,
                 enlarge_per_dim=enlarge_per_dim, n_networks=n_networks,
                 neural_network_kwargs=neural_network_kwargs, pool=pool,
                 rng=rng))
 
         bound.outer_bound = Union.compute(
-            points[log_l > log_l_min], enlarge_per_dim=enlarge_per_dim,
+            points[log_l >= log_l_min], enlarge_per_dim=enlarge_per_dim,
             n_points_min=n_points_min, bound_class=UnitCubeEllipsoidMixture,
             rng=rng)
 
         while bound.outer_bound.volume() - log_v_target > np.log(
                 split_threshold * enlarge_per_dim**points.shape[1]):
             if not bound.outer_bound.split_bound():
                 break
@@ -358,15 +358,20 @@
                     in_bound = np.any([bound.contains(points) for bound in
                                        self.neural_bounds], axis=0)
                     points = points[in_bound]
                     self.points = np.vstack([self.points, points])
                     self.n_sample += n_sample
                     self.n_reject += n_sample - len(points)
             else:
-                n_jobs = pool._processes
+                try:
+                    n_jobs = pool._processes
+                except AttributeError:
+                    n_jobs = pool.size
+                except AttributeError:
+                    raise ValueError('Cannot determine size of pool.')
                 n_points_per_job = (
                     (max(n_points - len(self.points), 10000)) // n_jobs) + 1
                 func = partial(self._reset_and_sample, n_points_per_job)
                 rngs = [np.random.default_rng(seed) for seed in
                         np.random.SeedSequence(self.rng.integers(
                             2**32 - 1)).spawn(n_jobs)]
                 bounds = pool.map(func, rngs)
@@ -434,17 +439,33 @@
         group.attrs['n_neural_bounds'] = len(self.neural_bounds)
 
         for i, neural_bound in enumerate(self.neural_bounds):
             neural_bound.write(group.create_group('neural_bound_{}'.format(i)))
 
         self.outer_bound.write(group.create_group('outer_bound'))
 
-        group.create_dataset('points', data=self.points)
+        group.create_dataset('points', data=self.points,
+                             maxshape=(None, self.n_dim))
+        group.attrs['n_sample'] = self.n_sample
+        group.attrs['n_reject'] = self.n_reject
+
+    def update(self, group):
+        """Update bound information previously written to an HDF5 group.
+
+        Parameters
+        ----------
+        group : h5py.Group
+            HDF5 group to write to.
+
+        """
         group.attrs['n_sample'] = self.n_sample
         group.attrs['n_reject'] = self.n_reject
+        self.outer_bound.update(group['outer_bound'])
+        group['points'].resize(self.points.shape)
+        group['points'][...] = self.points
 
     @classmethod
     def read(cls, group, rng=None):
         """Read the bound from an HDF5 group.
 
         Parameters
         ----------
```

### Comparing `nautilus-sampler-0.6.0/nautilus/bounds/union.py` & `nautilus-sampler-0.7.0/nautilus/bounds/union.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,15 +176,14 @@
 
         if not np.any(~self.block):
             return False
 
         index = np.argmax(np.where(~self.block, self.log_v, -np.inf))
         points = self.bounds[index].transform(self.points_bounds[index])
 
-        # print('mixture...')
         labels = GaussianMixture(
             n_components=2, n_init=10, random_state=self.rng.integers(
                 2**32 - 1)).fit_predict(points)
 
         if not np.all(np.bincount(labels) >= self.n_points_min):
             self.block[index] = True
             return self.split_bound(allow_overlap=allow_overlap)
@@ -316,15 +315,30 @@
 
         group.attrs['bound_class'] = self.bounds[0].__class__.__name__
         for i, bound in enumerate(self.bounds):
             bound.write(group.create_group('bound_{}'.format(i)))
 
         for i, points in enumerate(self.points_bounds):
             group.create_dataset('points_bound_{}'.format(i), data=points)
-        group.create_dataset('points', data=self.points)
+        group.create_dataset('points', data=self.points,
+                             maxshape=(None, self.n_dim))
+
+    def update(self, group):
+        """Update bound information previously written to an HDF5 group.
+
+        Parameters
+        ----------
+        group : h5py.Group
+            HDF5 group to write to.
+
+        """
+        group.attrs['n_sample'] = self.n_sample
+        group.attrs['n_reject'] = self.n_reject
+        group['points'].resize(self.points.shape)
+        group['points'][...] = self.points
 
     @classmethod
     def read(cls, group, rng=None):
         """Read the bound from an HDF5 group.
 
         Parameters
         ----------
```

### Comparing `nautilus-sampler-0.6.0/nautilus/neural.py` & `nautilus-sampler-0.7.0/nautilus/neural.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,16 +74,15 @@
         emulator = cls()
 
         emulator.mean = np.mean(x, axis=0)
         emulator.scale = np.std(x, axis=0)
 
         default_neural_network_kwargs = dict(
             hidden_layer_sizes=(100, 50, 20), alpha=0, learning_rate_init=1e-2,
-            max_iter=10000, tol=0, n_iter_no_change=10,
-            validation_fraction=0.1)
+            max_iter=10000, tol=0, n_iter_no_change=10)
         default_neural_network_kwargs.update(neural_network_kwargs)
         neural_network_kwargs = default_neural_network_kwargs
 
         if 'random_state' in neural_network_kwargs:
             warnings.warn("The 'random_state' keyword argument passed to the" +
                           " neural network is ignored.", Warning, stacklevel=2)
             del neural_network_kwargs['random_state']
@@ -130,15 +129,15 @@
         for i, network in enumerate(self.neural_networks):
 
             for key in network.__dict__:
                 if key in ['coefs_', 'intercepts_']:
                     continue
                 try:
                     group.attrs[key + '_{}'.format(i)] = getattr(network, key)
-                except TypeError:
+                except (TypeError, ValueError):
                     pass
 
             for k in range(network.n_layers_ - 1):
                 group.create_dataset('coefs_{}_{}'.format(k, i),
                                      data=network.coefs_[k])
                 group.create_dataset('intercepts_{}_{}'.format(k, i),
                                      data=network.intercepts_[k])
```

### Comparing `nautilus-sampler-0.6.0/nautilus/prior.py` & `nautilus-sampler-0.7.0/nautilus/prior.py`

 * *Files identical despite different names*

### Comparing `nautilus-sampler-0.6.0/nautilus/sampler.py` & `nautilus-sampler-0.7.0/nautilus/sampler.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     import h5py
 except ImportError:
     pass
 import numpy as np
 import warnings
 
 from functools import partial
-from multiprocessing import Pool, cpu_count
+from multiprocessing import Pool
 from pathlib import Path
 from scipy.special import logsumexp
 from threadpoolctl import threadpool_limits
 from tqdm import tqdm
 
 from .bounds import UnitCube, NautilusBound
 
@@ -36,18 +36,18 @@
         The maximum number of additions to the live set before a new bound is
         created.
     n_like_new_bound : int
         The maximum number of likelihood calls before a new bounds is created.
     enlarge_per_dim : float
         Along each dimension, outer ellipsoidal bounds are enlarged by this
         factor.
-    n_points_min : int or None, optional
+    n_points_min : int or None
         The minimum number of points each ellipsoid should have. Effectively,
         ellipsoids with less than twice that number will not be split further.
-    split_threshold: float, optional
+    split_threshold: float
         Threshold used for splitting the multi-ellipsoidal bound used for
         sampling. If the volume of the bound prior enlarging is larger than
         `split_threshold` times the target volume, the multi-ellipsiodal
         bound is split further, if possible.
     n_networks : int
         Number of networks used in the estimator.
     neural_network_kwargs : dict
@@ -57,65 +57,68 @@
         Number of likelihood evaluations that are performed at each step.
     vectorized : bool
         If True, the likelihood function can receive multiple input sets at
         once.
     pass_dict : bool
         If True, the likelihood function expects model parameters as
         dictionaries.
-    pool : object
+    pool_l : object
         Pool used to parallelize likelihood calls.
-    n_jobs : int or string
-        Number of parallel jobs to use for neural network training and sampling
-        new points.
+    pool_s : object
+        Pool used to parallelize sampler calculations.
     rng : np.random.Generator
         Random number generator of the sampler.
     n_like : int
         Total number of likelihood evaluations.
-    explored : bool, optional
+    explored : bool
         Whether the space has been explored and the shells have been
         constructed.
     bounds : list
         List of all the constructed bounds.
     points : list
         List of arrays where each array at position i lists the points
         belonging to the i-th bound/shell.
     log_l : list
         Log likelihood values of each point. Same ordering as `points`.
     blobs : list
         Blobs associated with each point. Same ordering as `points`.
     blobs_dtype : numpy.dtype
         Data type of the blobs.
+    _discard_exploration : bool
+        Whether to exclude points in the exploration phase.
     shell_n : numpy.ndarray
         Number of points for each bound/shell.
-    shell_n_sample_shell : numpy.ndarray
-        Number of points sampled in each bound that fall into the shell.
-    shell_n_sample_bound : numpy.ndarray
+    shell_n_sample : numpy.ndarray
         Number of points sampled in each bound.
     shell_n_eff : numpy.ndarray
         Effective sample size for each bound/shell.
     shell_log_l_min : numpy.ndarray
         Minimum logarithm of the likelihood required for an update in each
         bound/shell.
     shell_log_l : numpy.ndarray
         Logarithm of the mean likelihood of points in each bound/shell.
     shell_log_v : numpy.ndarray
         Logarithm of the volume of each bound/shell.
+    shell_n_sample_exp : numpy.ndarray
+        Number of points sampled in each bound during the exploration phase.
+    shell_end_exp : numpy.ndarray
+        Index at which points are coming from the sampling phase instead of the
+        exploration phase.
 
     """
 
     def __init__(self, prior, likelihood, n_dim=None, n_live=2000,
-                 n_update=None, enlarge=None, enlarge_per_dim=1.1,
-                 n_points_min=None, split_threshold=100,
-                 n_networks=4, neural_network_kwargs=dict(), prior_args=[],
+                 n_update=None, enlarge_per_dim=1.1, n_points_min=None,
+                 split_threshold=100, n_networks=4,
+                 neural_network_kwargs=dict(), prior_args=[],
                  prior_kwargs=dict(), likelihood_args=[],
                  likelihood_kwargs=dict(), n_batch=100,
-                 use_neural_networks=None, n_like_new_bound=None,
-                 vectorized=False, pass_dict=None, pool=None, n_jobs=1,
-                 random_state=None, seed=None,
-                 blobs_dtype=None, filepath=None, resume=True):
+                 n_like_new_bound=None, vectorized=False, pass_dict=None,
+                 pool=None, n_jobs=None, seed=None, blobs_dtype=None,
+                 filepath=None, resume=True):
         r"""
         Initialize the sampler.
 
         Parameters
         ----------
         prior : function or nautilus.Prior
             Prior describing the mapping of the unit hypercube to the
@@ -128,16 +131,14 @@
             `prior` to be an instance of `nautilus.Prior`.
         n_live : int, optional
             Number of so-called live points. New bounds are constructed so that
             they encompass the live points. Default is 3000.
         n_update : None or int, optional
             The maximum number of additions to the live set before a new bound
             is created. If None, use `n_live`. Default is None.
-        enlarge : float, optional
-            Deprecated.
         enlarge_per_dim : float, optional
             Along each dimension, outer ellipsoidal bounds are enlarged by this
             factor. Default is 1.1.
         n_points_min : int or None, optional
             The minimum number of points each ellipsoid should have.
             Effectively, ellipsoids with less than twice that number will not
             be split further. If None, uses `n_points_min = n_dim + 50`.
@@ -165,16 +166,14 @@
         n_batch : int, optional
             Number of likelihood evaluations that are performed at each step.
             If likelihood evaluations are parallelized, should be multiple
             of the number of parallel processes. Very large numbers can
             lead to new bounds being created long after `n_update` additions to
             the live set have been achieved. This will not cause any bias but
             could reduce efficiency. Default is 100.
-        use_neural_networks : bool, optional
-            Deprecated.
         n_like_new_bound : None or int, optional
             The maximum number of likelihood calls before a new bounds is
             created. If None, use 10 times `n_live`. Default is None.
         vectorized : bool, optional
             If True, the likelihood function can receive multiple input sets
             at once. For example, if the likelihood function receives arrays,
             it should be able to take an array with shape (n_points, n_dim)
@@ -183,28 +182,27 @@
             process dictionaries where each value is an array with shape
             (n_points). Default is False.
         pass_dict : bool or None, optional
             If True, the likelihood function expects model parameters as
             dictionaries. If False, it expects regular numpy arrays. Default is
             to set it to True if prior was a nautilus.Prior instance and False
             otherwise.
-        pool : object or int, optional
-            Object with a `map` function used for parallelization of likelihood
-            calls, e.g. a multiprocessing.Pool object, or a positive integer.
-            If it is an integer, it determines the number of workers in the
-            Pool. Default is None.
+        pool : None, object, int or tuple, optional
+            Pool used for parallelization of likelihood calls and sampler
+            calculations. If None, no parallelization is performed. If an
+            integer, the sampler will use a multiprocessing.Pool object with
+            the specified number of processes. Finally, if specifying a tuple,
+            the first one specifies the pool used for likelihood calls and the
+            second one the pool for sampler calculations. Default is None.
         n_jobs : int or string, optional
-            Number of parallel jobs to use for neural network training and
-            sampling new points. If the string 'max' is passed, all available
-            cores are used. Default is 'max'.
-        random_state : int or np.random.RandomState, optional
             Deprecated.
-        seed : int, optional
+        seed : None or int, optional
             Seed for random number generation used for reproducible results
-            accross different runs. Default is None.
+            accross different runs. If None, results are not reproducible.
+            Default is None.
         blobs_dtype : object or None, optional
             Object that can be converted to a data type object describing the
             blobs. If None, this will be inferred from the first blob. Default
             is None.
         filepath : string, pathlib.Path or None, optional
             Path to the file where results are saved. Must have a '.h5' or
             '.hdf5' extension. If None, no results are written. Default is
@@ -251,72 +249,70 @@
             n_update = n_live
         self.n_update = n_update
 
         if n_like_new_bound is None:
             n_like_new_bound = 10 * n_live
         self.n_like_new_bound = n_like_new_bound
 
-        if enlarge is not None:
-            warnings.warn("The 'enlarge' keyword argument has been " +
-                          "deprecated. Use 'enlarge_per_dim', instead.",
-                          DeprecationWarning, stacklevel=2)
-
         self.enlarge_per_dim = enlarge_per_dim
 
         if n_points_min is None:
             n_points_min = self.n_dim + 50
         self.n_points_min = n_points_min
 
         self.split_threshold = split_threshold
 
-        if use_neural_networks is not None:
-            warnings.warn("The 'use_neural_networks' keyword argument has " +
-                          "been deprecated. Set 'n_networks', instead.",
-                          DeprecationWarning, stacklevel=2)
-
         self.n_networks = n_networks
 
         self.neural_network_kwargs = neural_network_kwargs
         self.n_batch = n_batch
         self.vectorized = vectorized
         self.pass_dict = pass_dict
 
-        if isinstance(pool, int):
-            self.pool = Pool(pool)
-        elif pool is not None:
-            self.pool = pool
+        if pool is None or pool == 1:
+            self.pool_l = None
+            self.pool_s = None
+        elif isinstance(pool, int):
+            self.pool_l = Pool(pool)
+            self.pool_s = self.pool_l
+        elif isinstance(pool, tuple):
+            self.pool_l = pool[0]
+            if isinstance(self.pool_l, int):
+                self.pool_l = Pool(self.pool_l)
+            self.pool_s = pool[1]
+            if isinstance(self.pool_s, int):
+                self.pool_s = Pool(self.pool_s)
         else:
-            self.pool = None
+            self.pool_l = pool
+            self.pool_s = pool
 
-        if n_jobs == 'max':
-            n_jobs = cpu_count()
-        self.n_jobs = n_jobs
-
-        if random_state is not None:
-            warnings.warn("The 'random_state' keyword argument has been " +
-                          "deprecated. Use 'seed' instead.",
-                          DeprecationWarning, stacklevel=2)
+        if n_jobs is not None:
+            warnings.warn(
+                "The 'n_jobs' keyword argument has been deprecated .Use " +
+                "'pool', instead.", DeprecationWarning, stacklevel=2)
 
         self.rng = np.random.default_rng(seed)
 
         # The following variables carry the information about the run.
         self.n_like = 0
         self.explored = False
         self.bounds = []
         self.points = []
         self.log_l = []
         self.blobs = []
         self.blobs_dtype = blobs_dtype
+        self._discard_exploration = False
         self.shell_n = np.zeros(0, dtype=int)
-        self.shell_n_sample_shell = np.zeros(0, dtype=int)
-        self.shell_n_sample_bound = np.zeros(0, dtype=int)
+        self.shell_n_sample = np.zeros(0, dtype=int)
         self.shell_n_eff = np.zeros(0, dtype=float)
         self.shell_log_l_min = np.zeros(0, dtype=float)
         self.shell_log_l = np.zeros(0, dtype=float)
         self.shell_log_v = np.zeros(0, dtype=float)
+        self.shell_n_sample_exp = np.zeros(0, dtype=int)
+        self.shell_end_exp = np.zeros(0, dtype=int)
 
         self.filepath = filepath
         if resume and filepath is not None and Path(filepath).exists():
             with h5py.File(filepath, 'r') as fstream:
 
                 group = fstream['sampler']
 
@@ -324,18 +320,18 @@
                     bit_generator='PCG64',
                     state=dict(
                         state=int(group.attrs['rng_state']),
                         inc=int(group.attrs['rng_inc'])),
                     has_uint32=group.attrs['rng_has_uint32'],
                     uinteger=group.attrs['rng_uinteger'])
 
-                for key in ['n_like', 'explored', 'shell_n',
-                            'shell_n_sample_shell', 'shell_n_sample_bound',
-                            'shell_n_eff', 'shell_log_l_min', 'shell_log_l',
-                            'shell_log_v']:
+                for key in ['n_like', 'explored', '_discard_exploration',
+                            'shell_n', 'shell_n_sample', 'shell_n_eff',
+                            'shell_log_l_min', 'shell_log_l', 'shell_log_v',
+                            'shell_n_sample_exp', 'shell_end_exp']:
                     setattr(self, key, group.attrs[key])
 
                 for shell in range(len(self.shell_n)):
                     self.points.append(
                         np.array(group['points_{}'.format(shell)]))
                     self.log_l.append(
                         np.array(group['log_l_{}'.format(shell)]))
@@ -372,16 +368,14 @@
             Whether to discard points drawn in the exploration phase. This is
             required for a fully unbiased posterior and evidence estimate.
             Default is False.
         verbose : bool, optional
             If True, print additional information. Default is False.
 
         """
-        self._pool = Pool(self.n_jobs) if self.n_jobs > 1 else None
-
         if not self.explored:
 
             if verbose:
                 print('#########################')
                 print('### Exploration Phase ###')
                 print('#########################')
                 print()
@@ -399,34 +393,30 @@
             for shell in reversed(range(len(self.bounds))):
                 if self.shell_n[shell] == 0:
                     self.bounds.pop(shell)
                     self.points.pop(shell)
                     self.log_l.pop(shell)
                     if self.blobs_dtype is not None:
                         self.blobs.pop(shell)
-                    for key in ['shell_n', 'shell_n_sample_shell',
-                                'shell_n_sample_bound', 'shell_n_eff',
+                    for key in ['shell_n', 'shell_n_sample', 'shell_n_eff',
                                 'shell_log_l_min', 'shell_log_l',
                                 'shell_log_v']:
                         setattr(self, key, np.delete(
                             getattr(self, key), shell))
 
+            self.shell_n_sample_exp = np.copy(self.shell_n_sample)
+            self.shell_end_exp = np.array([len(p) for p in self.points])
             self.explored = True
+
             if self.filepath is not None:
                 self.write(self.filepath, overwrite=True)
 
-            if discard_exploration:
-                self.discard_points()
-                if self.filepath is not None:
-                    # Rename the old checkpoint file containing points in the
-                    # exploration phase and start a new one.
-                    path = Path(self.filepath)
-                    path.rename(Path(path.parent, path.stem + '_exp' +
-                                     path.suffix))
-                    self.write(self.filepath)
+        self.discard_exploration = discard_exploration
+        if self.filepath is not None:
+            self.write_shell_information_update(self.filepath)
 
         if n_shell is None:
             n_shell = self.n_batch
 
         if (np.any(self.shell_n < n_shell) or
                 self.effective_sample_size() < n_eff):
 
@@ -434,16 +424,47 @@
                 print('#########################')
                 print('##### Sampling Phase ####')
                 print('#########################')
                 print()
 
             self.add_points(n_shell=n_shell, n_eff=n_eff, verbose=verbose)
 
-        if self.n_jobs > 1:
-            self._pool.close()
+    @property
+    def discard_exploration(self):
+        """Return whether the exploration phase is discarded.
+
+        Returns
+        -------
+        discard_exploration : bool
+            Whether the exploration phase is discarded.
+
+        """
+        return self._discard_exploration
+
+    @discard_exploration.setter
+    def discard_exploration(self, discard_exploration):
+        """Set whether exploration phase should be discarded.
+
+        Parameters
+        ----------
+        discard_exploration : bool
+            Whether the exploration phase is discarded.
+
+        Raises
+        ------
+        ValueError
+            If `discard_exploration` is not a bool.
+
+        """
+        if not isinstance(discard_exploration, bool):
+            raise ValueError("'discard_exploration' must be a bool.")
+
+        self._discard_exploration = discard_exploration
+        for index in range(len(self.log_l)):
+            self.update_shell_info(index)
 
     def posterior(self, return_as_dict=None, equal_weight=False,
                   return_blobs=False):
         """Return the posterior sample estimate.
 
         Parameters
         ----------
@@ -477,23 +498,28 @@
         """
         if return_as_dict is None:
             if callable(self.prior) and self.pass_dict:
                 return_as_dict = True
             else:
                 return_as_dict = False
 
-        points = np.concatenate(self.points)
+        if self._discard_exploration and self.explored:
+            start = self.shell_end_exp
+        else:
+            start = np.zeros(len(self.points), dtype=int)
+
+        points = np.concatenate([p[s:] for p, s in zip(self.points, start)])
         log_v = np.repeat(self.shell_log_v -
                           np.log(np.maximum(self.shell_n, 1)), self.shell_n)
-        log_l = np.concatenate(self.log_l)
+        log_l = np.concatenate([l[s:] for l, s in zip(self.log_l, start)])
         log_w = log_v + log_l
         if return_blobs:
             if self.blobs_dtype is None:
                 raise ValueError('No blobs have been calculated.')
-            blobs = np.concatenate(self.blobs)
+            blobs = np.concatenate([b[s:] for b, s in zip(self.blobs, start)])
 
         if callable(self.prior):
             transform = self.prior
         else:
             if return_as_dict:
                 transform = self.prior.unit_to_dictionary
             else:
@@ -543,20 +569,42 @@
 
     def evidence(self):
         r"""Estimate the global evidence :math:`\log \mathcal{Z}`.
 
         Returns
         -------
         log_z : float
-            Estimate the global evidence :math:`\log \mathcal{Z}`.
+            Estimate of the global evidence :math:`\log \mathcal{Z}`.
 
         """
         select = ~np.isnan(self.shell_log_l)
         return logsumexp(self.shell_log_l[select] + self.shell_log_v[select])
 
+    def asymptotic_sampling_efficiency(self):
+        r"""Estimate the asymptotic sampling efficiency :math:`\eta`.
+
+        The asymptotic sampling efficiency is defined as
+        :math:`\eta = \lim_{N_{\rm like} \to \infty} N_{\rm eff} / N_{\rm like}`.
+        This is set after the exploration phase. However, the estimate will be
+        updated based on what is found in the sampling phase.
+
+        Returns
+        -------
+        eta : float
+            Estimate of the asymptotic sampling efficiency.
+
+        """
+        shell_log_z = self.shell_log_l + self.shell_log_v
+        shell_eta = self.shell_n_eff / self.shell_n
+        select = ~np.isnan(self.shell_log_l)
+        shell_log_z = shell_log_z[select]
+        shell_eta = shell_eta[select]
+        return np.exp(2 * logsumexp(shell_log_z) - 2 * logsumexp(
+            shell_log_z - 0.5 * np.log(shell_eta)))
+
     def sample_shell(self, index, shell_t=None):
         """Sample a batch of points uniformly from a shell.
 
         The shell at index :math:`i` is defined as the volume enclosed by the
         bound of index :math:`i` and enclosed by not other bound of index
         :math:`k` with :math:`k > i`.
 
@@ -590,15 +638,15 @@
         n_sample = 0
         idx_t = np.zeros(0, dtype=int)
         points_all = []
 
         with threadpool_limits(limits=1):
             while n_sample < self.n_batch:
                 points = self.bounds[index].sample(
-                    self.n_batch - n_sample, pool=self._pool)
+                    self.n_batch - n_sample, pool=self.pool_s)
                 n_bound += self.n_batch - n_sample
 
                 # Remove points that are actually in another shell.
                 in_shell = np.ones(len(points), dtype=bool)
                 for bound in self.bounds[index:][1:]:
                     in_shell = in_shell & ~bound.contains(points)
                     if np.all(~in_shell):
@@ -672,16 +720,16 @@
             args = transform(points)
 
         # Evaluate the likelihood.
         if self.vectorized:
             result = self.likelihood(args)
             if isinstance(result, tuple):
                 result = list(zip(*result))
-        elif self.pool is not None:
-            result = list(self.pool.map(self.likelihood, args))
+        elif self.pool_l is not None:
+            result = list(self.pool_l.map(self.likelihood, args))
         else:
             result = list(map(self.likelihood, args))
 
         if isinstance(result[0], tuple):
             log_l = np.array([r[0] for r in result])
             blobs = [r[1:] for r in result]
             if self.blobs_dtype is None:
@@ -709,22 +757,29 @@
 
         Parameters
         ----------
         index: int
             Index of the shell.
 
         """
-        log_l = self.log_l[index]
+        shell_n_sample = self.shell_n_sample[index]
+
+        if self._discard_exploration and self.explored:
+            start = self.shell_end_exp[index]
+            shell_n_sample -= self.shell_n_sample_exp[index]
+        else:
+            start = 0
+
+        log_l = self.log_l[index][start:]
         self.shell_n[index] = len(log_l)
 
         if self.shell_n[index] > 0:
             self.shell_log_v[index] = (
                 self.bounds[index].volume() +
-                np.log(self.shell_n_sample_shell[index] /
-                       self.shell_n_sample_bound[index]))
+                np.log(self.shell_n[index] / shell_n_sample))
             self.shell_log_l[index] = logsumexp(log_l) - np.log(len(log_l))
             if not np.all(log_l == -np.inf):
                 self.shell_n_eff[index] = np.exp(2 * logsumexp(log_l) -
                                                  logsumexp(2 * log_l))
             else:
                 self.shell_n_eff[index] = len(log_l)
         else:
@@ -738,79 +793,94 @@
         print('N_eff: {:>18.0f}'.format(self.effective_sample_size()))
         print('log Z: {:>18.3f}'.format(self.evidence()))
         if not self.explored:
             print('log V: {:>18.3f}'.format(self.shell_log_v[-1]))
             print('f_live: {:>17.3f}'.format(self.live_evidence_fraction()))
 
     def add_bound(self, verbose=False):
-        """Build a new bound from existing points.
+        """Try building a new bound from existing points.
+
+        If the new bound would be larger than the previious bound, we will
+        reject the new bound.
 
         Parameters
         ----------
         verbose : bool, optional
             If True, print additional information. Default is False.
 
         """
-        self.shell_n = np.append(self.shell_n, 0)
-        self.shell_n_sample_shell = np.append(self.shell_n_sample_shell, 0)
-        self.shell_n_sample_bound = np.append(self.shell_n_sample_bound, 0)
-        self.shell_n_eff = np.append(self.shell_n_eff, 0)
-        self.shell_log_l = np.append(self.shell_log_l, np.nan)
-        self.shell_log_v = np.append(self.shell_log_v, np.nan)
-
+        success = False
         # If this is the first bound, use the UnitCube bound.
         if len(self.bounds) == 0:
             log_l_min = -np.inf
             self.bounds.append(UnitCube.compute(self.n_dim, rng=self.rng))
+            success = True
         else:
             if verbose:
-                print('Adding bound {}'.format(len(self.bounds) + 1), end='\r')
+                print('Adding Bound {}'.format(len(self.bounds) + 1), end='\r')
             log_l = np.concatenate(self.log_l)
             points = np.concatenate(self.points)[np.argsort(log_l)]
             log_l = np.sort(log_l)
             log_l_min = 0.5 * (log_l[-self.n_live] + log_l[-self.n_live - 1])
             with threadpool_limits(limits=1):
                 bound = NautilusBound.compute(
                     points, log_l, log_l_min, self.live_volume(),
                     enlarge_per_dim=self.enlarge_per_dim,
                     n_points_min=self.n_points_min,
                     split_threshold=self.split_threshold,
                     n_networks=self.n_networks,
                     neural_network_kwargs=self.neural_network_kwargs,
-                    pool=self._pool, rng=self.rng)
-                bound.sample(1000, return_points=False, pool=self._pool)
-                if bound.volume() > self.bounds[-1].volume():
-                    bound = self.bounds[-1]
-            self.bounds.append(bound)
-
-        self.points.append([])
-        self.log_l.append([])
-        self.blobs.append([])
-        self.shell_log_l_min = np.append(self.shell_log_l_min, log_l_min)
+                    pool=self.pool_s, rng=self.rng)
+                bound.sample(1000, return_points=False, pool=self.pool_s)
+            if bound.volume() < self.bounds[-1].volume():
+                self.bounds.append(bound)
+                success = True
+
+        if success:
+            self.shell_n = np.append(self.shell_n, 0)
+            self.shell_n_sample = np.append(self.shell_n_sample, 0)
+            self.shell_n_eff = np.append(self.shell_n_eff, 0)
+            self.shell_log_l = np.append(self.shell_log_l, np.nan)
+            self.shell_log_v = np.append(self.shell_log_v, np.nan)
+            self.shell_log_l_min = np.append(self.shell_log_l_min, log_l_min)
+            self.points.append(np.zeros((0, self.n_dim)))
+            self.log_l.append(np.zeros(0))
+            self.blobs.append(np.zeros(0))
+        else:
+            self.shell_log_l_min[-1] = log_l_min
 
         if verbose:
-            print('Adding bound {:<7} done'.format(
-                str(len(self.bounds)) + ':'))
+            print('Adding Bound {:<5} {:>6}'.format(
+                str(len(self.bounds) + (not success)) + ':', 'done' if success
+                else 'failed'))
             if isinstance(self.bounds[-1], NautilusBound):
-                n_neural, n_sample =\
+                n_neural, n_ell =\
                     self.bounds[-1].number_of_networks_and_ellipsoids()
             else:
-                n_neural, n_sample = 0, 0
-            print("Neural nets: {:>12}".format(n_neural))
-            print("Ellipsoids: {:>13}".format(n_sample))
+                n_neural, n_ell = 0, 0
+            if success:
+                print("Ellipsoids: {:>13}".format(n_ell))
+                print("Neural Networks: {:>8}".format(n_neural))
 
     def fill_bound(self, verbose=False):
         """Fill a new bound with points until a new bound should be created.
 
         Parameters
         ----------
         verbose : bool, optional
             If True, print additional information. Default is False.
 
         """
+        self.points[-1] = [self.points[-1], ]
+        self.log_l[-1] = [self.log_l[-1], ]
+        if len(self.blobs[-1]) > 0:
+            self.blobs[-1] = [self.blobs[-1], ]
+        else:
+            self.blobs[-1] = []
+
         shell_t = []
         points_t = []
         log_l_t = []
         blobs_t = []
 
         # Check which points points from previous shells could be transferred
         # to the new bound.
@@ -827,15 +897,14 @@
                 self.log_l[shell] = self.log_l[shell][~in_bound]
 
                 if self.blobs_dtype is not None:
                     blobs_t.append(self.blobs[shell][in_bound])
                     self.blobs[shell] = self.blobs[shell][~in_bound]
 
                 self.shell_n[shell] -= np.sum(in_bound)
-                self.shell_n_sample_shell[shell] -= np.sum(in_bound)
                 self.update_shell_info(shell)
 
             shell_t = np.concatenate(shell_t)
             points_t = np.concatenate(points_t)
             log_l_t = np.concatenate(log_l_t)
             if self.blobs_dtype is not None:
                 blobs_t = np.concatenate(blobs_t)
@@ -846,15 +915,15 @@
         n_update_max = self.n_update
         n_like_max = self.n_like_new_bound
         if len(self.bounds) == 1:
             n_update_max += self.n_live
             n_like_max = np.inf
 
         if verbose:
-            pbar = tqdm(desc='Filling bound {}'.format(len(self.bounds)),
+            pbar = tqdm(desc='Filling Bound {}'.format(len(self.bounds)),
                         total=n_update_max, leave=False)
 
         while n_update < n_update_max and n_like < n_like_max:
             points, n_bound, idx_t = self.sample_shell(-1, shell_t)
             assert len(points) + len(idx_t) == n_bound
             log_l, blobs = self.evaluate_likelihood(points)
             self.points[-1].append(points)
@@ -869,31 +938,32 @@
                 log_l_t = np.delete(log_l_t, idx_t)
                 if self.blobs_dtype is not None:
                     self.blobs[-1].append(blobs_t[idx_t])
                     blobs_t = np.delete(blobs_t, idx_t, axis=0)
                 shell_t = np.delete(shell_t, idx_t)
 
             self.shell_n[-1] += n_bound
-            self.shell_n_sample_shell[-1] += n_bound
-            self.shell_n_sample_bound[-1] += n_bound
+            self.shell_n_sample[-1] += n_bound
             n_update += np.sum(log_l >= log_l_min)
             n_like += len(points)
 
             if verbose:
                 pbar.update(np.sum(log_l >= log_l_min))
 
         self.points[-1] = np.concatenate(self.points[-1])
         self.log_l[-1] = np.concatenate(self.log_l[-1])
         if self.blobs_dtype is not None:
             self.blobs[-1] = np.concatenate(self.blobs[-1])
+        else:
+            self.blobs[-1] = np.zeros(0)
         self.update_shell_info(-1)
 
         if verbose:
             pbar.close()
-            print('Filling bound {:<6} done'.format(
+            print('Filling Bound {:<6} done'.format(
                 str(len(self.bounds)) + ':'))
             self.print_status()
             print('')
 
     def live_evidence_fraction(self):
         """Estimate the fraction of the evidence contained in the live set.
 
@@ -944,36 +1014,24 @@
         Parameters
         ----------
         shell : int
             The index of the shell for which to add points.
 
         """
         points, n_bound = self.sample_shell(shell)
-        self.shell_n_sample_shell[shell] += len(points)
-        self.shell_n_sample_bound[shell] += n_bound
+        self.shell_n_sample[shell] += n_bound
         log_l, blobs = self.evaluate_likelihood(points)
         self.points[shell] = np.concatenate([self.points[shell], points])
         self.log_l[shell] = np.concatenate([self.log_l[shell], log_l])
         if self.blobs_dtype is not None:
             self.blobs[shell] = np.concatenate([self.blobs[shell], blobs])
         self.update_shell_info(shell)
         if self.filepath is not None:
             self.write_shell_update(self.filepath, shell)
 
-    def discard_points(self):
-        """Discard all points drawn."""
-        for i in range(len(self.bounds)):
-            self.shell_n_sample_shell[i] = 0
-            self.shell_n_sample_bound[i] = 0
-            self.points[i] = np.zeros((0, self.n_dim))
-            self.log_l[i] = np.zeros(0)
-            if self.blobs_dtype is not None:
-                self.blobs[i] = self.blobs[i][:0]
-            self.update_shell_info(i)
-
     def add_points(self, n_eff=0, n_shell=0, verbose=False):
         """Add samples to shells.
 
         This function add samples to the shell until very shell has a minimum
         number of points and a minimum effective sample size is achieved.
 
         Parameters
@@ -1124,17 +1182,18 @@
 
         fstream = h5py.File(filepath, 'x')
         group = fstream.create_group('sampler')
 
         for key in ['n_dim', 'n_live', 'n_update', 'n_like_new_bound',
                     'enlarge_per_dim', 'n_points_min', 'split_threshold',
                     'n_networks', 'n_batch', 'vectorized', 'pass_dict',
-                    'n_like', 'explored', 'shell_n', 'shell_n_sample_shell',
-                    'shell_n_sample_bound', 'shell_n_eff', 'shell_log_l_min',
-                    'shell_log_l', 'shell_log_v']:
+                    'n_like', 'explored', '_discard_exploration', 'shell_n',
+                    'shell_n_sample', 'shell_n_eff', 'shell_log_l_min',
+                    'shell_log_l', 'shell_log_v', 'shell_n_sample_exp',
+                    'shell_end_exp']:
             group.attrs[key] = getattr(self, key)
 
         for key in self.neural_network_kwargs.keys():
             group.attrs['neural_network_{}'.format(key)] =\
                 self.neural_network_kwargs[key]
 
         for shell in range(len(self.bounds)):
@@ -1168,46 +1227,49 @@
         Parameters
         ----------
         filepath : string or pathlib.Path
             Path to the file. Must have a '.h5' or '.hdf5' extension.
         shell : int
             Shell index for which to write the upate.
 
-        Raises
-        ------
-        RuntimeError
-            If file does not exist.
-
         """
-        filepath = Path(filepath)
-
-        if not filepath.exists():
-            raise RuntimeError(
-                "File {} does not exist.".format(str(filepath)))
-
-        fstream = h5py.File(filepath, 'r+')
+        fstream = h5py.File(Path(filepath), 'r+')
         group = fstream['sampler']
 
-        for key in ['n_like', 'shell_n', 'shell_n_sample_shell',
-                    'shell_n_sample_bound', 'shell_n_eff', 'shell_log_l_min',
-                    'shell_log_l', 'shell_log_v']:
+        for key in ['n_like', 'shell_n', 'shell_n_sample', 'shell_n_eff',
+                    'shell_log_l_min', 'shell_log_l', 'shell_log_v']:
             group.attrs[key] = getattr(self, key)
 
-        for key in self.neural_network_kwargs.keys():
-            group.attrs['neural_network_{}'.format(key)] =\
-                self.neural_network_kwargs[key]
-
         group['points_{}'.format(shell)].resize(self.points[shell].shape)
         group['points_{}'.format(shell)][...] = self.points[shell]
         group['log_l_{}'.format(shell)].resize(self.log_l[shell].shape)
         group['log_l_{}'.format(shell)][...] = self.log_l[shell]
         if self.blobs_dtype is not None:
             group['blobs_{}'.format(shell)].resize(self.blobs[shell].shape)
             group['blobs_{}'.format(shell)][...] = self.blobs[shell]
 
+        if isinstance(self.bounds[shell], NautilusBound):
+            self.bounds[shell].update(fstream['bound_{}'.format(shell)])
+
         rng_state = self.rng.bit_generator.state
         group.attrs['rng_state'] = str(rng_state['state']['state'])
         group.attrs['rng_inc'] = str(rng_state['state']['inc'])
         group.attrs['rng_has_uint32'] = rng_state['has_uint32']
         group.attrs['rng_uinteger'] = rng_state['uinteger']
 
         fstream.close()
+
+    def write_shell_information_update(self, filepath):
+        """Update the shell summary statistics.
+
+        Parameters
+        ----------
+        filepath : string or pathlib.Path
+            Path to the file. Must have a '.h5' or '.hdf5' extension.
+
+        """
+        with h5py.File(Path(filepath), 'r+') as fstream:
+            group = fstream['sampler']
+            for key in ['_discard_exploration', 'shell_n', 'shell_n_sample',
+                        'shell_n_eff', 'shell_log_l_min', 'shell_log_l',
+                        'shell_log_v', 'shell_n_sample_exp', 'shell_end_exp']:
+                group.attrs[key] = getattr(self, key)
```

### Comparing `nautilus-sampler-0.6.0/pyproject.toml` & `nautilus-sampler-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nautilus-sampler-0.6.0/tests/test_blobs.py` & `nautilus-sampler-0.7.0/tests/test_blobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     def likelihood(x):
         if vectorized:
             return np.ones(len(x)), (10 * x[:, 0]).astype(dtype)
         else:
             return 1, dtype(10 * x[0])
 
     sampler = Sampler(prior, likelihood, n_dim=2, n_live=10,
-                      vectorized=vectorized, n_jobs=1)
+                      vectorized=vectorized)
     sampler.run(f_live=1.0, n_eff=200, discard_exploration=discard_exploration)
     points, log_w, log_l, blobs = sampler.posterior(return_blobs=True)
 
     assert len(points) == len(blobs)
     assert blobs.dtype == dtype
     assert np.all((10 * points[:, 0]).astype(dtype) == blobs)
 
@@ -42,15 +42,15 @@
         if vectorized:
             return (np.ones(len(x)), x[:, 0].astype(np.float32),
                     x[:, 1].astype(np.float32))
         else:
             return 1, np.float32(x[0]), np.float32(x[1])
 
     sampler = Sampler(prior, likelihood, n_dim=2, n_live=10,
-                      vectorized=vectorized, n_jobs=1)
+                      vectorized=vectorized)
     sampler.run(f_live=1.0, n_eff=200, discard_exploration=discard_exploration)
     points, log_w, log_l, blobs = sampler.posterior(return_blobs=True)
 
     assert len(points) == len(blobs)
     assert blobs['blob_0'].dtype == np.float32
     assert blobs['blob_1'].dtype == np.float32
     assert np.all(points[:, 0].astype(np.float32) == blobs['blob_0'])
@@ -66,15 +66,15 @@
         if vectorized:
             return np.ones(len(x)), x[:, 0], x[:, 1]
         else:
             return 1, x[0], x[1]
 
     blobs_dtype = [('a', '|S10'), ('b', np.int16)]
     sampler = Sampler(prior, likelihood, n_dim=2, n_live=10,
-                      vectorized=vectorized, n_jobs=1, blobs_dtype=blobs_dtype)
+                      vectorized=vectorized, blobs_dtype=blobs_dtype)
     sampler.run(f_live=1.0, n_eff=200, discard_exploration=discard_exploration)
     points, log_w, log_l, blobs = sampler.posterior(return_blobs=True)
 
     assert len(points) == len(blobs)
     assert blobs['a'].dtype == blobs_dtype[0][1]
     assert blobs['b'].dtype == blobs_dtype[1][1]
     assert np.all(points[:, 0].astype(blobs_dtype[0][1]) == blobs['a'])
@@ -90,13 +90,13 @@
     def likelihood(x):
         if vectorized:
             return np.ones(len(x)), x[:, 0], x[:, 1]
         else:
             return 1, x[0], x[1]
 
     sampler = Sampler(prior, likelihood, n_dim=2, n_live=10,
-                      vectorized=vectorized, n_jobs=1, blobs_dtype=float)
+                      vectorized=vectorized, blobs_dtype=float)
     sampler.run(f_live=1.0, n_eff=200, discard_exploration=discard_exploration)
     points, log_w, log_l, blobs = sampler.posterior(return_blobs=True)
     assert len(points) == len(blobs)
     assert np.all(points[:, 0] == blobs[:, 0])
     assert np.all(points[:, 1] == blobs[:, 1])
```

### Comparing `nautilus-sampler-0.6.0/tests/test_bounds.py` & `nautilus-sampler-0.7.0/tests/test_bounds.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,14 +206,32 @@
     # allowed.
     assert union.split_bound()
     assert not union.split_bound()
     assert len(union.bounds) == 3
     assert np.all(union.contains(points))
 
 
+def test_union_split_stops(random_points_from_hypersphere):
+    # Test that splitting ellipsoids correctly stops after some time.
+
+    x = np.linspace(-1, 1, 30)
+    y = x**2
+    points = np.vstack([x, y]).T
+
+    bound = bounds.Union.compute(points)
+    n = 0
+
+    while bound.split_bound():
+        n += 1
+
+    assert n > 0
+    assert np.all(np.array([len(points) for points in bound.points_bounds]) >=
+                  bound.n_points_min)
+
+
 def test_union_sample_and_contains(random_points_from_hypersphere):
     # Test whether the union sampling and boundary work as expected.
 
     union = bounds.Union.compute(
         random_points_from_hypersphere + 50, enlarge_per_dim=1.0,
         unit=False, rng=np.random.default_rng(0))
     for i in range(4):
```

### Comparing `nautilus-sampler-0.6.0/tests/test_io.py` & `nautilus-sampler-0.7.0/tests/test_io.py`

 * *Files 11% similar despite different names*

```diff
@@ -84,14 +84,30 @@
     if ((rng_sync or bound_class in [UnitCube, Ellipsoid]) and not
             bound_class == NeuralBound):
         assert bound_write.volume() == bound_read.volume()
 
     points = np.random.random((10000, n_dim))
     assert np.all(bound_write.contains(points) == bound_read.contains(points))
 
+    if bound_class in [Union, NautilusBound]:
+        bound_write.sample(10000)
+        bound_write.update(h5py_group)
+
+        rng = np.random.default_rng(1)
+        if rng_sync:
+            rng.bit_generator.state = bound_write.rng.bit_generator.state
+
+        bound_read = bound_class.read(h5py_group, rng=rng)
+
+        assert (np.all(bound_write.sample(20000) == bound_read.sample(20000))
+                == rng_sync)
+
+        if rng_sync:
+            assert bound_write.volume() == bound_read.volume()
+
 
 @pytest.mark.parametrize("blobs", [True, False])
 @pytest.mark.parametrize("discard_exploration", [True, False])
 @pytest.mark.parametrize("n_networks", [0, 1, 2])
 def test_sampler_io(blobs, discard_exploration, n_networks):
     # Test that we can write and read a sampler correctly. In particular, also
     # test that the random number generator is correctly set after writing and
@@ -103,52 +119,36 @@
     def likelihood(x):
         if blobs:
             return -np.linalg.norm(x - 0.5) * 0.001, x[0]
         else:
             return -np.linalg.norm(x - 0.5) * 0.001
 
     sampler_write = Sampler(prior, likelihood, n_dim=2, n_live=100,
-                            n_networks=n_networks, n_jobs=1,
-                            filepath='test.hdf5', resume=False, seed=0)
-    sampler_write.run(f_live=0.45, n_eff=0, verbose=True)
+                            n_networks=n_networks, filepath='test.hdf5',
+                            resume=False, seed=0)
+    sampler_write.run(f_live=0.45, n_eff=1000,
+                      discard_exploration=discard_exploration, verbose=True)
     sampler_write.explored = False
+    # Reset the interal shell calculations.
+    sampler_write.discard_exploration = discard_exploration
     sampler_read = Sampler(prior, likelihood, n_dim=2, n_live=100,
-                           n_networks=n_networks, n_jobs=1,
-                           filepath='test.hdf5', resume=True)
+                           n_networks=n_networks, filepath='test.hdf5',
+                           resume=True)
     sampler_read.explored = False
+    # Reset the interal shell calculations.
+    sampler_read.discard_exploration = discard_exploration
+    assert sampler_write.evidence() == sampler_read.evidence()
 
-    sampler_write.run(f_live=0.45, n_eff=1000,
+    sampler_write.run(f_live=0.45, n_eff=5000,
                       discard_exploration=discard_exploration, verbose=True)
-    sampler_read.run(f_live=0.45, n_eff=1000,
+    sampler_read.run(f_live=0.45, n_eff=5000,
                      discard_exploration=discard_exploration, verbose=True)
 
     posterior_write = sampler_write.posterior()
     posterior_read = sampler_read.posterior()
 
     for arr_write, arr_read in zip(posterior_write, posterior_read):
         assert np.all(arr_write == arr_read)
 
     assert sampler_write.evidence() == sampler_read.evidence()
 
     Path('test.hdf5').unlink()
-
-
-def test_sampler_exploration_io():
-    # Test that the sampler correctly creates a backup of the state after the
-    # exploration stage.
-
-    def prior(x):
-        return x
-
-    def likelihood(x):
-        return -np.linalg.norm(x - 0.5) * 0.001
-
-    sampler = Sampler(prior, likelihood, n_dim=2, n_live=100,
-                      n_networks=1, n_jobs=1, filepath='test.hdf5',
-                      resume=False, seed=0)
-    sampler.run(n_eff=1000, discard_exploration=True)
-
-    assert Path('test.hdf5').is_file()
-    assert Path('test_exp.hdf5').is_file()
-
-    Path('test.hdf5').unlink()
-    Path('test_exp.hdf5').unlink()
```

### Comparing `nautilus-sampler-0.6.0/tests/test_prior.py` & `nautilus-sampler-0.7.0/tests/test_prior.py`

 * *Files identical despite different names*

### Comparing `nautilus-sampler-0.6.0/tests/test_sampler.py` & `nautilus-sampler-0.7.0/tests/test_sampler.py`

 * *Files 23% similar despite different names*

```diff
@@ -24,17 +24,58 @@
     def likelihood(x):
         if pass_dict:
             x = np.squeeze(np.column_stack([x['a'], x['b']]))
         return -np.linalg.norm(x - 0.5, axis=-1) * 0.001
 
     sampler = Sampler(
         prior, likelihood, n_dim=2, n_networks=n_networks,
-        vectorized=vectorized, pass_dict=pass_dict, n_live=500, n_jobs=1)
+        vectorized=vectorized, pass_dict=pass_dict, n_live=500)
     sampler.run(f_live=0.45, n_eff=0, verbose=False)
     points, log_w, log_l = sampler.posterior(return_as_dict=pass_dict)
+    assert sampler.effective_sample_size() > 0
+    sampler.evidence()
+    assert sampler.asymptotic_sampling_efficiency() > 0
+    assert sampler.asymptotic_sampling_efficiency() < 1
+
+
+@pytest.mark.parametrize("discard_exploration_start", [True, False])
+@pytest.mark.parametrize("discard_exploration_end", [True, False, 1])
+def test_sampler_switch_exploration(
+        discard_exploration_start, discard_exploration_end):
+    # Test that we can switch later whether to discard the exploration phase.
+
+    def prior(x):
+        return x
+
+    def likelihood(x):
+        return -np.linalg.norm(x - 0.5, axis=-1) * 0.001
+
+    sampler = Sampler(
+        prior, likelihood, n_dim=2, n_networks=1, vectorized=True, n_live=500)
+    sampler.run(f_live=0.45, n_eff=10000, verbose=False,
+                discard_exploration=discard_exploration_start)
+    assert sampler.discard_exploration == discard_exploration_start
+    points, log_w, log_l = sampler.posterior()
+    n_start = len(points)
+    log_z_start = sampler.evidence()
+
+    if not isinstance(discard_exploration_end, bool):
+        with pytest.raises(ValueError):
+            sampler.discard_exploration = discard_exploration_end
+        return
+
+    sampler.discard_exploration = discard_exploration_end
+    points, log_w, log_l = sampler.posterior()
+    n_end = len(points)
+    log_z_end = sampler.evidence()
+
+    assert ((discard_exploration_start == discard_exploration_end) ==
+            (n_start == n_end))
+    assert ((discard_exploration_start == discard_exploration_end) ==
+            (log_z_start == log_z_end))
 
 
 @pytest.mark.parametrize("custom_prior", [True, False])
 @pytest.mark.parametrize("vectorized", [True, False])
 @pytest.mark.parametrize("pass_dict", [True, False])
 def test_sampler_prior(custom_prior, vectorized, pass_dict):
     # Test that the sampler can handle all prior defintions.
@@ -54,15 +95,15 @@
     def likelihood(x):
         if isinstance(x, dict):
             x = np.squeeze(np.column_stack([x['a'], x['b']]))
         return -np.linalg.norm(x - 0.5, axis=-1) * 0.001
 
     sampler = Sampler(
         prior, likelihood, n_dim=2, n_networks=1, vectorized=vectorized,
-        pass_dict=pass_dict, n_live=500, n_jobs=1)
+        pass_dict=pass_dict, n_live=500)
     sampler.run(f_live=0.45, n_eff=0, verbose=False)
     points, log_w, log_l = sampler.posterior(return_as_dict=pass_dict)
     if custom_prior and pass_dict:
         with pytest.raises(ValueError):
             points, log_w, log_l = sampler.posterior(return_as_dict=False)
 
 
@@ -78,15 +119,15 @@
     def prior(x):
         return x
 
     def likelihood(x):
         return multivariate_normal.logpdf(x, mean=mean, cov=cov)
 
     sampler = Sampler(prior, likelihood, n_dim=n_dim, n_live=500,
-                      n_networks=n_networks, n_jobs=1, seed=0)
+                      n_networks=n_networks, seed=0)
     sampler.run(discard_exploration=discard_exploration, f_live=0.1,
                 verbose=False)
 
     assert np.abs(sampler.evidence()) < 0.05
 
     for equal_weight in [True, False]:
         points, log_w, log_l = sampler.posterior(equal_weight=equal_weight)
@@ -113,15 +154,15 @@
     def prior(x):
         return x
 
     def likelihood(x):
         return -np.linalg.norm(x - 0.5)**2 * 0.001
 
     sampler = Sampler(prior, likelihood, n_dim=2, enlarge_per_dim=100,
-                      n_networks=0, n_jobs=1, seed=0)
+                      n_networks=0, seed=0)
     sampler.run(f_live=0.1, n_eff=0)
 
     # The effective sample size should be very close to the number of calls
     # since the likelihood is extremely flat.
     assert np.isclose(sampler.n_like, sampler.effective_sample_size(), rtol=0,
                       atol=1)
     # Only one bound should be left.
@@ -149,16 +190,15 @@
     # close to 1 minus a correction for the fraction of points falling outside
     # the unit cube.
     np.random.seed(0)
     x_0 = np.random.normal(loc=0.5, scale=0.1, size=1000000)
     x_1 = np.random.normal(loc=0.5, scale=np.exp(20 * (x_0 - 0.5)) / 100)
     log_z_true = np.log(np.mean((x_0 > 0) & (x_0 < 1) & (x_1 > 0) & (x_1 < 1)))
 
-    sampler = Sampler(prior, likelihood, n_dim=2, n_networks=1, n_jobs=1,
-                      seed=0)
+    sampler = Sampler(prior, likelihood, n_dim=2, n_networks=1, seed=0)
     sampler.run()
     assert np.isclose(log_z_true, sampler.evidence(), rtol=0, atol=0.1)
     # Check whether the boundaries nautilus drew are strictly nested.
     shell_bound_occupation = sampler.shell_bound_occupation()
     if np.all(shell_bound_occupation ==
               np.tril(np.ones_like(shell_bound_occupation))):
         warnings.warn('The funnel distribution was too easy.', RuntimeWarning)
```

### Comparing `nautilus-sampler-0.6.0/PKG-INFO` & `nautilus-sampler-0.7.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nautilus-sampler
-Version: 0.6.0
+Version: 0.7.0
 Summary: Neural Network-Boosted Importance Sampling for Bayesian Statistics
 Author-email: "Johannes U. Lange" <julange.astro@pm.me>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: scikit-learn
@@ -52,11 +52,15 @@
 corner.corner(points, weights=np.exp(log_w), labels='abc')
 ```
 
 ## Documentation
 
 You can find the documentation at [nautilus-sampler.readthedocs.io](https://nautilus-sampler.readthedocs.io).
 
+## Attribution
+
+A paper describing nautilus's underlying methods and performance has been submitted for publication. A draft of the paper will be uploaded to arXiv around the end of June 2023. Please cite the paper, once available, if you found nautilus helpful in your research.
+
 ## License
 
 Nautilus is licensed under the MIT License. The logo uses an image from the Illustris Collaboration.
```

