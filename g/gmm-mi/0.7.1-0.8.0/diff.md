# Comparing `tmp/gmm_mi-0.7.1.tar.gz` & `tmp/gmm_mi-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmm_mi-0.7.1.tar", last modified: Mon Jun 19 13:21:42 2023, max compression
+gzip compressed data, was "gmm_mi-0.8.0.tar", last modified: Tue Jun 20 13:18:56 2023, max compression
```

## Comparing `gmm_mi-0.7.1.tar` & `gmm_mi-0.8.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-06-19 13:21:42.211077 gmm_mi-0.7.1/
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    35149 2022-08-06 22:31:49.000000 gmm_mi-0.7.1/LICENSE.txt
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)      625 2022-08-06 22:32:40.000000 gmm_mi-0.7.1/LICENSE_EXT.txt
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    10845 2023-06-19 13:21:42.210077 gmm_mi-0.7.1/PKG-INFO
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    10270 2023-05-30 14:51:38.000000 gmm_mi-0.7.1/README.md
-drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-06-19 13:21:42.171077 gmm_mi-0.7.1/gmm_mi/
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        0 2022-08-10 10:00:35.000000 gmm_mi-0.7.1/gmm_mi/__init__.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     7226 2022-10-10 13:21:45.000000 gmm_mi-0.7.1/gmm_mi/cross_validation.py
-drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-06-19 13:21:42.190077 gmm_mi-0.7.1/gmm_mi/data/
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        0 2022-08-10 10:03:30.000000 gmm_mi-0.7.1/gmm_mi/data/__init__.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     2823 2022-09-08 16:08:51.000000 gmm_mi-0.7.1/gmm_mi/data/synthetic_data.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    25656 2023-06-08 14:41:11.000000 gmm_mi-0.7.1/gmm_mi/gmm.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    12706 2022-10-10 13:23:09.000000 gmm_mi-0.7.1/gmm_mi/initializations.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    45647 2023-06-19 12:54:39.000000 gmm_mi-0.7.1/gmm_mi/mi.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     2202 2023-01-04 21:01:21.000000 gmm_mi-0.7.1/gmm_mi/param_holders.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     2234 2022-10-10 13:21:54.000000 gmm_mi-0.7.1/gmm_mi/single_fit.py
-drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-06-19 13:21:42.204077 gmm_mi-0.7.1/gmm_mi/utils/
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        0 2022-08-02 10:30:25.000000 gmm_mi-0.7.1/gmm_mi/utils/__init__.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     1852 2022-10-10 13:17:18.000000 gmm_mi-0.7.1/gmm_mi/utils/analytic_MI.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    29790 2023-01-04 21:01:21.000000 gmm_mi-0.7.1/gmm_mi/utils/plotting.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)      929 2022-09-30 20:11:49.000000 gmm_mi-0.7.1/gmm_mi/utils/transformations.py
-drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-06-19 13:21:42.185077 gmm_mi-0.7.1/gmm_mi.egg-info/
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    10845 2023-06-19 13:21:42.000000 gmm_mi-0.7.1/gmm_mi.egg-info/PKG-INFO
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)      525 2023-06-19 13:21:42.000000 gmm_mi-0.7.1/gmm_mi.egg-info/SOURCES.txt
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        1 2023-06-19 13:21:42.000000 gmm_mi-0.7.1/gmm_mi.egg-info/dependency_links.txt
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)       77 2023-06-19 13:21:42.000000 gmm_mi-0.7.1/gmm_mi.egg-info/requires.txt
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)       17 2023-06-19 13:21:42.000000 gmm_mi-0.7.1/gmm_mi.egg-info/top_level.txt
-drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-06-19 13:21:42.208077 gmm_mi-0.7.1/notebooks/
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        0 2022-08-02 10:30:55.000000 gmm_mi-0.7.1/notebooks/__init__.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)       38 2023-06-19 13:21:42.212077 gmm_mi-0.7.1/setup.cfg
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     1153 2023-06-19 12:55:12.000000 gmm_mi-0.7.1/setup.py
+drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-06-20 13:18:56.462938 gmm_mi-0.8.0/
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    35149 2022-08-06 22:31:49.000000 gmm_mi-0.8.0/LICENSE.txt
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)      625 2022-08-06 22:32:40.000000 gmm_mi-0.8.0/LICENSE_EXT.txt
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    11444 2023-06-20 13:18:56.461938 gmm_mi-0.8.0/PKG-INFO
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    10869 2023-06-20 11:26:24.000000 gmm_mi-0.8.0/README.md
+drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-06-20 13:18:56.345937 gmm_mi-0.8.0/gmm_mi/
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        0 2022-08-10 10:00:35.000000 gmm_mi-0.8.0/gmm_mi/__init__.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     7226 2022-10-10 13:21:45.000000 gmm_mi-0.8.0/gmm_mi/cross_validation.py
+drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-06-20 13:18:56.367938 gmm_mi-0.8.0/gmm_mi/data/
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        0 2022-08-10 10:03:30.000000 gmm_mi-0.8.0/gmm_mi/data/__init__.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     2823 2022-09-08 16:08:51.000000 gmm_mi-0.8.0/gmm_mi/data/synthetic_data.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    25656 2023-06-08 14:41:11.000000 gmm_mi-0.8.0/gmm_mi/gmm.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    12706 2022-10-10 13:23:09.000000 gmm_mi-0.8.0/gmm_mi/initializations.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    47491 2023-06-20 13:05:07.000000 gmm_mi-0.8.0/gmm_mi/mi.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     2202 2023-01-04 21:01:21.000000 gmm_mi-0.8.0/gmm_mi/param_holders.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     2234 2022-10-10 13:21:54.000000 gmm_mi-0.8.0/gmm_mi/single_fit.py
+drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-06-20 13:18:56.429938 gmm_mi-0.8.0/gmm_mi/utils/
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        0 2022-08-02 10:30:25.000000 gmm_mi-0.8.0/gmm_mi/utils/__init__.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     1852 2022-10-10 13:17:18.000000 gmm_mi-0.8.0/gmm_mi/utils/analytic_MI.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    31198 2023-06-20 13:09:07.000000 gmm_mi-0.8.0/gmm_mi/utils/plotting.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)      929 2022-09-30 20:11:49.000000 gmm_mi-0.8.0/gmm_mi/utils/transformations.py
+drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-06-20 13:18:56.361938 gmm_mi-0.8.0/gmm_mi.egg-info/
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    11444 2023-06-20 13:18:56.000000 gmm_mi-0.8.0/gmm_mi.egg-info/PKG-INFO
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)      525 2023-06-20 13:18:56.000000 gmm_mi-0.8.0/gmm_mi.egg-info/SOURCES.txt
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        1 2023-06-20 13:18:56.000000 gmm_mi-0.8.0/gmm_mi.egg-info/dependency_links.txt
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)       77 2023-06-20 13:18:56.000000 gmm_mi-0.8.0/gmm_mi.egg-info/requires.txt
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)       17 2023-06-20 13:18:56.000000 gmm_mi-0.8.0/gmm_mi.egg-info/top_level.txt
+drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-06-20 13:18:56.458938 gmm_mi-0.8.0/notebooks/
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        0 2022-08-02 10:30:55.000000 gmm_mi-0.8.0/notebooks/__init__.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)       38 2023-06-20 13:18:56.463938 gmm_mi-0.8.0/setup.cfg
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     1153 2023-06-20 10:31:04.000000 gmm_mi-0.8.0/setup.py
```

### Comparing `gmm_mi-0.7.1/LICENSE.txt` & `gmm_mi-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.7.1/LICENSE_EXT.txt` & `gmm_mi-0.8.0/LICENSE_EXT.txt`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.7.1/PKG-INFO` & `gmm_mi-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmm_mi
-Version: 0.7.1
+Version: 0.8.0
 Summary: Estimate mutual information distribution with Gaussian mixture models
 Home-page: https://github.com/dpiras/GMM-MI
 Author: Davide Piras
 Author-email: dr.davide.piras@gmail.com
 License: GNU General Public License v3.0 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -69,14 +69,23 @@
     # the extra arguments can be changed
     ax = mi_estimator.plot_fitted_model(ax=ax, color='salmon', alpha=0.8, linewidth=4)
     ax.tick_params(axis='both', which='both', labelsize=20)
     ax.set_xlabel('X1', fontsize=30)
     ax.set_ylabel('X2', fontsize=30)
     ax.legend(fontsize=25, frameon=False)    
 
+You can also draw contour plots for the input data and samples obtained from the fitted model. For example (smoothness of the contour plot heavily depends on the number of samples available):
+
+    fig = mi_estimator.plot_fitted_contours(parameters=['X1', 'X2'], 
+                                        shade_alpha=0.4, linewidths=2, 
+                                        legend_kwargs = {'loc': 'lower right'},
+                                        kde=True, # smooths contours; set this to False to accelerate plotting
+                                        )
+    fig.set_size_inches(7, 7)
+
 To choose the GMM-MI hyperparameters, we provide three classes: `GMMFitParamHolder`, `SelectComponentsParamHolder`, and `MIDistParamHolder`. An example is as follows:
 
     from gmm_mi.param_holders import GMMFitParamHolder, SelectComponentsParamHolder, MIDistParamHolder
 
     # parameters for every GMM fit that is being run
     gmm_fit_params = GMMFitParamHolder(threshold_fit=1e-5, reg_covar=1e-15)
     # parameters to choose the number of components
```

### Comparing `gmm_mi-0.7.1/README.md` & `gmm_mi-0.8.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -53,14 +53,23 @@
     # the extra arguments can be changed
     ax = mi_estimator.plot_fitted_model(ax=ax, color='salmon', alpha=0.8, linewidth=4)
     ax.tick_params(axis='both', which='both', labelsize=20)
     ax.set_xlabel('X1', fontsize=30)
     ax.set_ylabel('X2', fontsize=30)
     ax.legend(fontsize=25, frameon=False)    
 
+You can also draw contour plots for the input data and samples obtained from the fitted model. For example (smoothness of the contour plot heavily depends on the number of samples available):
+
+    fig = mi_estimator.plot_fitted_contours(parameters=['X1', 'X2'], 
+                                        shade_alpha=0.4, linewidths=2, 
+                                        legend_kwargs = {'loc': 'lower right'},
+                                        kde=True, # smooths contours; set this to False to accelerate plotting
+                                        )
+    fig.set_size_inches(7, 7)
+
 To choose the GMM-MI hyperparameters, we provide three classes: `GMMFitParamHolder`, `SelectComponentsParamHolder`, and `MIDistParamHolder`. An example is as follows:
 
     from gmm_mi.param_holders import GMMFitParamHolder, SelectComponentsParamHolder, MIDistParamHolder
 
     # parameters for every GMM fit that is being run
     gmm_fit_params = GMMFitParamHolder(threshold_fit=1e-5, reg_covar=1e-15)
     # parameters to choose the number of components
```

### Comparing `gmm_mi-0.7.1/gmm_mi/cross_validation.py` & `gmm_mi-0.8.0/gmm_mi/cross_validation.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.7.1/gmm_mi/data/synthetic_data.py` & `gmm_mi-0.8.0/gmm_mi/data/synthetic_data.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.7.1/gmm_mi/gmm.py` & `gmm_mi-0.8.0/gmm_mi/gmm.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.7.1/gmm_mi/initializations.py` & `gmm_mi-0.8.0/gmm_mi/initializations.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.7.1/gmm_mi/mi.py` & `gmm_mi-0.8.0/gmm_mi/mi.py`

 * *Files 3% similar despite different names*

```diff
@@ -598,50 +598,93 @@
         See the respective methods for all information.
         """ 
         self.fit(X=X, Y=Y, verbose=verbose)
         MI_mean, MI_std = self.estimate(mi_dist_params=mi_dist_params, include_kl=include_kl, 
                                        kl_order=kl_order, base=base, verbose=verbose)
         return MI_mean, MI_std            
                     
-    def plot_fitted_model(self, ax=None, return_gmm=False, **kwargs):
-        """Fit model to inout data and plot its contours.
+    def _single_fit(self):
+        """Fit final model to input data. 
+        This will be used to draw GMM components and/or contours.
         Only works if the model has been fitted successfully first.
+          
+        Returns
+        -------
+        gmm : instance of GMM class
+            The fitted GMM model.
+        """
+        if not self.fit_done:
+            raise NotFittedError(
+                "This EstimateMI instance is not fitted yet. Call `fit` with appropriate "
+                "arguments before using this estimator."
+                                )
+            
+        gmm = single_fit(X=self.X, n_components=self.best_components, reg_covar=self.reg_covar, 
+                 threshold_fit=self.threshold_fit, random_state=self.best_seed, max_iter=self.max_iter, 
+                 w_init=self.w_init, m_init=self.m_init, p_init=self.p_init)
+        return gmm
+
+    def plot_fitted_model(self, ax=None, **kwargs):
+        """Plot GMM contours over the input data.
+        Only works if the model has been fitted successfully first,
+        and only in the case of 2D input data (i.e. not in the conditional case).
+        Works in the continuous case only.
         
         Parameters
         ----------
         ax : instance of the axes.Axes class from pyplot, default=None
             The panel where to plot the samples. 
-        return_gmm : bool
-            Whether or not to return also a GMM class instance with the fitted model
         kwargs : dictionary
             The extra keyword arguments to pass to the plotting function.
         
         Returns
         -------
-        fig: instance of the figure.Figure class from pyplot
-            The output figure.
         ax : instance of the axes.Axes class from pyplot
             The output panel.
-        """
-        if not self.fit_done:
-            raise NotFittedError(
-                "This EstimateMI instance is not fitted yet. Call `fit` with appropriate "
-                "arguments before using this estimator."
-                                )
-            
+        """     
         from gmm_mi.utils.plotting import plot_gmm_contours
-        gmm = single_fit(X=self.X, n_components=self.best_components, reg_covar=self.reg_covar, 
-                 threshold_fit=self.threshold_fit, random_state=self.best_seed, max_iter=self.max_iter, 
-                 w_init=self.w_init, m_init=self.m_init, p_init=self.p_init)
+        if self.conditional:
+            raise NotImplementedError("When computing conditional MI, to visualise the contours "
+                                      "you need to call `plot_fitted_contours`.")
+        gmm = self._single_fit()    
         ax = plot_gmm_contours(gmm, ax=ax, label='Fitted model', **kwargs)
-        if return_gmm:
-            return ax, gmm
-        else:
-            return ax
-               
+        return ax
+ 
+    def plot_fitted_contours(self, parameters=None, extents=None, n_samples=None, **kwargs):
+        """Plot overall fitted distribution contours over the input data.
+        The contours are created using `chainconsumer`.
+        Only works if the model has been fitted successfully first, and in the continuous case only.
+        
+        Parameters
+        ----------
+        parameters : list, default=None
+            List of strings with the parameters name, to put in the labels.
+        extents : dictionary, default=None
+            Contains the ranges of each parameter. Key must be a string, value a tuple/list.
+        n_samples : int, default=None
+            The number of samples to draw from the fitted GMM to draw the contours.
+            If None, draws the same number of samples as in the input data.
+        kwargs : dictionary
+            The extra keyword arguments to pass to the plotting function.
+        
+        Returns
+        -------
+        fig: instance of the figure.Figure class from pyplot
+            The output figure.
+
+        """
+        from gmm_mi.utils.plotting import plot_contours
+        gmm = self._single_fit()  
+        if n_samples:
+            fitted_samples = gmm.sample(n_samples)[0]
+        else:    
+            fitted_samples = gmm.sample(self.X.shape[0])[0]
+        fig = plot_contours(self.X, fitted_samples, parameters, extents, **kwargs)
+        return fig
+             
     def _calculate_MI_categorical(self):
         """Calculate mutual information (MI) integral given a Gaussian mixture model in 2D.
         Use only Monte Carlo (MC) method. 
         The complete formula can be found in Appendix B of Piras et al. (2022).
 
         Returns
         -------
```

### Comparing `gmm_mi-0.7.1/gmm_mi/param_holders.py` & `gmm_mi-0.8.0/gmm_mi/param_holders.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.7.1/gmm_mi/single_fit.py` & `gmm_mi-0.8.0/gmm_mi/single_fit.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.7.1/gmm_mi/utils/analytic_MI.py` & `gmm_mi-0.8.0/gmm_mi/utils/analytic_MI.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.7.1/gmm_mi/utils/plotting.py` & `gmm_mi-0.8.0/gmm_mi/utils/plotting.py`

 * *Files 3% similar despite different names*

```diff
@@ -206,15 +206,49 @@
     contours = find_contours(contour_levels)   
     # draw the ellipse
     for contour in contours:
         ax.add_patch(Ellipse(mean, contour*width, contour*height, angle=angle, fill=fill, 
                              label=label if component_count==0 else "", **kwargs))
         ax.scatter(mean[0], mean[1], s=weight_size*weight, marker=marker, **kwargs)
 
-    
+
+def plot_contours(input_samples, fitted_samples, parameters, extents, **kwargs):
+    """Plot contours given samples of some distribution, even high-dimensional.
+    The contours are created using `chainconsumer` (https://samreay.github.io/ChainConsumer/).
+
+    Parameters
+    ----------
+    input_samples : array-like of shape (n_samples, n_features)
+        The input samples that were used to fit the GMM.
+    fitted_samples : array-like of shape (n_samples, n_features)
+        The samples obtained from the fitted GMM model.
+    parameters : list, default=None
+        List of strings with the parameters name, to put in the labels.
+    extents : dictionary, default=None
+        Contains the ranges of each parameter. Key must be a string, value a tuple/list.
+    kwargs : dictionary
+        The extra keyword arguments to pass to the plotting function.
+
+    Returns
+    -------
+    fig: instance of the figure.Figure class from pyplot
+        The output figure.
+    """
+    try:
+        from chainconsumer import ChainConsumer
+    except:
+        raise ModuleNotFoundError('To plot contours, you need to `pip install chainconsumer` first')
+            
+    c = ChainConsumer().add_chain(input_samples, parameters=parameters, name='Input data')
+    c.add_chain(fitted_samples, parameters=parameters, name='Fitted model')
+    c.configure(**kwargs) 
+    fig = c.plotter.plot(extents=extents)
+    return fig
+
+
 def plot_gmm_contours(gmm, ax=None, fill=False, label='', xlabel='X1', ylabel='X2', **kwargs):
     """Draw the contour ellipses corresponding to a given Gaussian mixture model (GMM).
     
     Parameters
     ----------
     gmm : instance of the GMM class
         The GMM whose contours are going to be displayed.
```

### Comparing `gmm_mi-0.7.1/gmm_mi/utils/transformations.py` & `gmm_mi-0.8.0/gmm_mi/utils/transformations.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.7.1/gmm_mi.egg-info/PKG-INFO` & `gmm_mi-0.8.0/gmm_mi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmm-mi
-Version: 0.7.1
+Version: 0.8.0
 Summary: Estimate mutual information distribution with Gaussian mixture models
 Home-page: https://github.com/dpiras/GMM-MI
 Author: Davide Piras
 Author-email: dr.davide.piras@gmail.com
 License: GNU General Public License v3.0 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -69,14 +69,23 @@
     # the extra arguments can be changed
     ax = mi_estimator.plot_fitted_model(ax=ax, color='salmon', alpha=0.8, linewidth=4)
     ax.tick_params(axis='both', which='both', labelsize=20)
     ax.set_xlabel('X1', fontsize=30)
     ax.set_ylabel('X2', fontsize=30)
     ax.legend(fontsize=25, frameon=False)    
 
+You can also draw contour plots for the input data and samples obtained from the fitted model. For example (smoothness of the contour plot heavily depends on the number of samples available):
+
+    fig = mi_estimator.plot_fitted_contours(parameters=['X1', 'X2'], 
+                                        shade_alpha=0.4, linewidths=2, 
+                                        legend_kwargs = {'loc': 'lower right'},
+                                        kde=True, # smooths contours; set this to False to accelerate plotting
+                                        )
+    fig.set_size_inches(7, 7)
+
 To choose the GMM-MI hyperparameters, we provide three classes: `GMMFitParamHolder`, `SelectComponentsParamHolder`, and `MIDistParamHolder`. An example is as follows:
 
     from gmm_mi.param_holders import GMMFitParamHolder, SelectComponentsParamHolder, MIDistParamHolder
 
     # parameters for every GMM fit that is being run
     gmm_fit_params = GMMFitParamHolder(threshold_fit=1e-5, reg_covar=1e-15)
     # parameters to choose the number of components
```

### Comparing `gmm_mi-0.7.1/gmm_mi.egg-info/SOURCES.txt` & `gmm_mi-0.8.0/gmm_mi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.7.1/setup.py` & `gmm_mi-0.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 PACKAGENAME = 'gmm_mi'
 
 setup(
     name='gmm_mi',
-    version="0.7.1",
+    version="0.8.0",
     author='Davide Piras',
     author_email='dr.davide.piras@gmail.com',
     description='Estimate mutual information distribution with Gaussian mixture models',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/dpiras/GMM-MI',
     license='GNU General Public License v3.0 (GPLv3)',
```

