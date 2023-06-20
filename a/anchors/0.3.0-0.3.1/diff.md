# Comparing `tmp/anchors-0.3.0.tar.gz` & `tmp/anchors-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/anchors-0.3.0.tar", last modified: Tue Sep 22 01:54:12 2020, max compression
+gzip compressed data, was "anchors-0.3.1.tar", last modified: Tue Jun 20 16:00:36 2023, max compression
```

## Comparing `anchors-0.3.0.tar` & `anchors-0.3.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-22 01:54:12.489061 anchors-0.3.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)      167 2020-09-22 01:48:47.000000 anchors-0.3.0/AUTHORS.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     3505 2020-09-22 01:48:47.000000 anchors-0.3.0/CONTRIBUTING.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      167 2020-09-22 01:48:47.000000 anchors-0.3.0/HISTORY.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1078 2020-09-22 01:48:47.000000 anchors-0.3.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      262 2020-09-22 01:48:47.000000 anchors-0.3.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     3056 2020-09-22 01:54:12.489061 anchors-0.3.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1667 2020-09-22 01:48:47.000000 anchors-0.3.0/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-22 01:54:12.489061 anchors-0.3.0/anchors/
--rw-rw-r--   0 travis    (2000) travis    (2000)      195 2020-09-22 01:48:47.000000 anchors-0.3.0/anchors/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14248 2020-09-22 01:48:47.000000 anchors-0.3.0/anchors/score.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-22 01:54:12.489061 anchors-0.3.0/anchors.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3056 2020-09-22 01:54:12.000000 anchors-0.3.0/anchors.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      535 2020-09-22 01:54:12.000000 anchors-0.3.0/anchors.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-09-22 01:54:12.000000 anchors-0.3.0/anchors.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-09-22 01:54:12.000000 anchors-0.3.0/anchors.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)       92 2020-09-22 01:54:12.000000 anchors-0.3.0/anchors.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2020-09-22 01:54:12.000000 anchors-0.3.0/anchors.egg-info/top_level.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-22 01:54:12.489061 anchors-0.3.0/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)      608 2020-09-22 01:48:47.000000 anchors-0.3.0/docs/Makefile
--rw-rw-r--   0 travis    (2000) travis    (2000)      295 2020-09-22 01:48:47.000000 anchors-0.3.0/docs/anchors.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       28 2020-09-22 01:48:47.000000 anchors-0.3.0/docs/authors.rst
--rwxrwxr-x   0 travis    (2000) travis    (2000)     4932 2020-09-22 01:48:47.000000 anchors-0.3.0/docs/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       33 2020-09-22 01:48:47.000000 anchors-0.3.0/docs/contributing.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       28 2020-09-22 01:48:47.000000 anchors-0.3.0/docs/history.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      306 2020-09-22 01:48:47.000000 anchors-0.3.0/docs/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1110 2020-09-22 01:48:47.000000 anchors-0.3.0/docs/installation.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      769 2020-09-22 01:48:47.000000 anchors-0.3.0/docs/make.bat
--rw-rw-r--   0 travis    (2000) travis    (2000)       58 2020-09-22 01:48:47.000000 anchors-0.3.0/docs/modules.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       27 2020-09-22 01:48:47.000000 anchors-0.3.0/docs/readme.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      449 2020-09-22 01:54:12.493061 anchors-0.3.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1455 2020-09-22 01:48:47.000000 anchors-0.3.0/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-09-22 01:54:12.489061 anchors-0.3.0/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)       37 2020-09-22 01:48:47.000000 anchors-0.3.0/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1766 2020-09-22 01:48:47.000000 anchors-0.3.0/tests/test_anchors.py
+drwxr-xr-x   0 fu         (503) staff       (20)        0 2023-06-20 16:00:36.008257 anchors-0.3.1/
+-rw-r--r--   0 fu         (503) staff       (20)      167 2023-06-20 14:50:07.000000 anchors-0.3.1/AUTHORS.rst
+-rw-r--r--   0 fu         (503) staff       (20)     3505 2023-06-20 14:50:07.000000 anchors-0.3.1/CONTRIBUTING.rst
+-rw-r--r--   0 fu         (503) staff       (20)      167 2023-06-20 14:50:07.000000 anchors-0.3.1/HISTORY.rst
+-rw-r--r--   0 fu         (503) staff       (20)     1078 2023-06-20 14:50:07.000000 anchors-0.3.1/LICENSE
+-rw-r--r--   0 fu         (503) staff       (20)      262 2023-06-20 14:50:07.000000 anchors-0.3.1/MANIFEST.in
+-rw-r--r--   0 fu         (503) staff       (20)     2521 2023-06-20 16:00:36.008480 anchors-0.3.1/PKG-INFO
+-rw-r--r--   0 fu         (503) staff       (20)     1667 2023-06-20 14:50:07.000000 anchors-0.3.1/README.rst
+drwxr-xr-x   0 fu         (503) staff       (20)        0 2023-06-20 16:00:35.988506 anchors-0.3.1/anchors/
+-rw-r--r--   0 fu         (503) staff       (20)      195 2023-06-20 15:12:10.000000 anchors-0.3.1/anchors/__init__.py
+-rw-r--r--   0 fu         (503) staff       (20)    14248 2023-06-20 15:06:59.000000 anchors-0.3.1/anchors/score.py
+drwxr-xr-x   0 fu         (503) staff       (20)        0 2023-06-20 16:00:35.993675 anchors-0.3.1/anchors.egg-info/
+-rw-r--r--   0 fu         (503) staff       (20)     2521 2023-06-20 16:00:35.000000 anchors-0.3.1/anchors.egg-info/PKG-INFO
+-rw-r--r--   0 fu         (503) staff       (20)      535 2023-06-20 16:00:35.000000 anchors-0.3.1/anchors.egg-info/SOURCES.txt
+-rw-r--r--   0 fu         (503) staff       (20)        1 2023-06-20 16:00:35.000000 anchors-0.3.1/anchors.egg-info/dependency_links.txt
+-rw-r--r--   0 fu         (503) staff       (20)        1 2023-06-20 15:17:27.000000 anchors-0.3.1/anchors.egg-info/not-zip-safe
+-rw-r--r--   0 fu         (503) staff       (20)       92 2023-06-20 16:00:35.000000 anchors-0.3.1/anchors.egg-info/requires.txt
+-rw-r--r--   0 fu         (503) staff       (20)        8 2023-06-20 16:00:35.000000 anchors-0.3.1/anchors.egg-info/top_level.txt
+drwxr-xr-x   0 fu         (503) staff       (20)        0 2023-06-20 16:00:36.005021 anchors-0.3.1/docs/
+-rw-r--r--   0 fu         (503) staff       (20)      608 2023-06-20 14:50:07.000000 anchors-0.3.1/docs/Makefile
+-rw-r--r--   0 fu         (503) staff       (20)      295 2023-06-20 14:50:07.000000 anchors-0.3.1/docs/anchors.rst
+-rw-r--r--   0 fu         (503) staff       (20)       28 2023-06-20 14:50:07.000000 anchors-0.3.1/docs/authors.rst
+-rwxr-xr-x   0 fu         (503) staff       (20)     4932 2023-06-20 14:50:07.000000 anchors-0.3.1/docs/conf.py
+-rw-r--r--   0 fu         (503) staff       (20)       33 2023-06-20 14:50:07.000000 anchors-0.3.1/docs/contributing.rst
+-rw-r--r--   0 fu         (503) staff       (20)       28 2023-06-20 14:50:07.000000 anchors-0.3.1/docs/history.rst
+-rw-r--r--   0 fu         (503) staff       (20)      306 2023-06-20 14:50:07.000000 anchors-0.3.1/docs/index.rst
+-rw-r--r--   0 fu         (503) staff       (20)     1110 2023-06-20 14:50:07.000000 anchors-0.3.1/docs/installation.rst
+-rw-r--r--   0 fu         (503) staff       (20)      769 2023-06-20 14:50:07.000000 anchors-0.3.1/docs/make.bat
+-rw-r--r--   0 fu         (503) staff       (20)       58 2023-06-20 14:50:07.000000 anchors-0.3.1/docs/modules.rst
+-rw-r--r--   0 fu         (503) staff       (20)       27 2023-06-20 14:50:07.000000 anchors-0.3.1/docs/readme.rst
+-rw-r--r--   0 fu         (503) staff       (20)      449 2023-06-20 16:00:36.009394 anchors-0.3.1/setup.cfg
+-rw-r--r--   0 fu         (503) staff       (20)     1455 2023-06-20 15:15:05.000000 anchors-0.3.1/setup.py
+drwxr-xr-x   0 fu         (503) staff       (20)        0 2023-06-20 16:00:36.007112 anchors-0.3.1/tests/
+-rw-r--r--   0 fu         (503) staff       (20)       37 2023-06-20 14:57:07.000000 anchors-0.3.1/tests/__init__.py
+-rw-r--r--   0 fu         (503) staff       (20)     1766 2023-06-20 14:59:48.000000 anchors-0.3.1/tests/test_anchors.py
```

### Comparing `anchors-0.3.0/CONTRIBUTING.rst` & `anchors-0.3.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `anchors-0.3.0/LICENSE` & `anchors-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `anchors-0.3.0/PKG-INFO` & `anchors-0.3.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,88 +1,89 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: anchors
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python package for calculating scores from ancnchor or modifier screens
 Home-page: https://github.com/gpp-rnd/anchors
 Author: Peter Carl DeWeirdt
 Author-email: petedeweirdt@gmail.com
 License: MIT license
-Description: =======
-        anchors
-        =======
-        
-        
-        .. image:: https://img.shields.io/pypi/v/anchors.svg
-                :target: https://pypi.python.org/pypi/anchors
-        
-        .. image:: https://img.shields.io/travis/gpp-rnd/anchors.svg
-                :target: https://travis-ci.com/gpp-rnd/anchors
-        
-        .. image:: https://readthedocs.org/projects/anchors/badge/?version=latest
-                :target: https://anchors.readthedocs.io/en/latest/?badge=latest
-                :alt: Documentation Status
-        
-        
-        
-        
-        Python package for calculating scores from ancnchor or modifier screens
-        
-        
-        * Free software: MIT license
-        * Documentation: https://anchors.readthedocs.io.
-        
-        Tutorial
-        --------
-        To install::
-        
-            $ pip install anchors
-        
-        Basic Usage
-        ^^^^^^^^^^^
-        .. code:: python
-        
-            import pandas as pd
-            from anchors import get_guide_residuals, get_gene_residuals
-            lfc_df = pd.read_csv('https://raw.githubusercontent.com/PeterDeWeirdt/anchor_screen_parp_lfcs/master/parp_example_lfcs.csv')
-            refernce_condition_df = pd.read_csv('https://raw.githubusercontent.com/PeterDeWeirdt/anchor_screen_parp_lfcs/master/parp_example_mapping.csv')
-            guide_residuals, model_info, model_fit_plots = get_guide_residuals(lfc_df, refernce_condition_df)
-            guide_mapping_df = pd.read_csv('https://raw.githubusercontent.com/PeterDeWeirdt/anchor_screen_parp_lfcs/master/brunello_guide_map.csv')
-            gene_residuals = get_gene_residuals(guide_residuals, guide_mapping_df)
-        
-        Features
-        --------
-        
-        * TODO
-        
-        Credits
-        -------
-        
-        This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
-        
-        .. _Cookiecutter: https://github.com/audreyr/cookiecutter
-        .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
-        
-        
-        =======
-        History
-        =======
-        
-        0.1.0 (2020-09-21)
-        ------------------
-        
-        * First release on PyPI.
-        
-        0.3.0 (2020-09-21)
-        ------------------
-        
-        * Calculate guide and gene residuals.
-        
 Keywords: anchors
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.5
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+=======
+anchors
+=======
+
+
+.. image:: https://img.shields.io/pypi/v/anchors.svg
+        :target: https://pypi.python.org/pypi/anchors
+
+.. image:: https://img.shields.io/travis/gpp-rnd/anchors.svg
+        :target: https://travis-ci.com/gpp-rnd/anchors
+
+.. image:: https://readthedocs.org/projects/anchors/badge/?version=latest
+        :target: https://anchors.readthedocs.io/en/latest/?badge=latest
+        :alt: Documentation Status
+
+
+
+
+Python package for calculating scores from ancnchor or modifier screens
+
+
+* Free software: MIT license
+* Documentation: https://anchors.readthedocs.io.
+
+Tutorial
+--------
+To install::
+
+    $ pip install anchors
+
+Basic Usage
+^^^^^^^^^^^
+.. code:: python
+
+    import pandas as pd
+    from anchors import get_guide_residuals, get_gene_residuals
+    lfc_df = pd.read_csv('https://raw.githubusercontent.com/PeterDeWeirdt/anchor_screen_parp_lfcs/master/parp_example_lfcs.csv')
+    refernce_condition_df = pd.read_csv('https://raw.githubusercontent.com/PeterDeWeirdt/anchor_screen_parp_lfcs/master/parp_example_mapping.csv')
+    guide_residuals, model_info, model_fit_plots = get_guide_residuals(lfc_df, refernce_condition_df)
+    guide_mapping_df = pd.read_csv('https://raw.githubusercontent.com/PeterDeWeirdt/anchor_screen_parp_lfcs/master/brunello_guide_map.csv')
+    gene_residuals = get_gene_residuals(guide_residuals, guide_mapping_df)
+
+Features
+--------
+
+* TODO
+
+Credits
+-------
+
+This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
+
+.. _Cookiecutter: https://github.com/audreyr/cookiecutter
+.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+
+
+=======
+History
+=======
+
+0.1.0 (2020-09-21)
+------------------
+
+* First release on PyPI.
+
+0.3.0 (2020-09-21)
+------------------
+
+* Calculate guide and gene residuals.
```

### Comparing `anchors-0.3.0/README.rst` & `anchors-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `anchors-0.3.0/anchors/score.py` & `anchors-0.3.1/anchors/score.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,23 +180,21 @@
     array_like
         Residuals for the given condition
     dict
         Information about the fit model
     matplotlib.figure.Figure
         Plot of spline fit
     """
-    x_data = lfc_df[condition_x]
+    x_data = lfc_df[condition_x] # series type
     y_data = lfc_df[condition_y]
-    x_data = x_data.rename('x', axis=1)
-    y_data = y_data.rename('y', axis=1)
-    model_df = pd.concat([x_data, y_data], axis=1)
+    model_df = pd.DataFrame({'x': x_data, 'y':y_data}) # columns with x and y values with 'x' and 'y' headers
     optimal_degree = find_optimal_degree(model_df, degrees, folds, 'x', 'y')
     model_fit = fit_natural_cubic_spline(model_df, optimal_degree, 'x', 'y')
     model_info = {'model': 'spline', 'deg_fdm': optimal_degree, 'const': model_fit.params.xs('Intercept')}
-    predictions = model_fit.predict(x_data)
+    predictions = model_fit.predict(model_df['x'])
     residuals = y_data - predictions
     fig, _ = plot_model_fit(model_df, predictions, 'x', 'y', condition_x, condition_y)
     return residuals, model_info, fig
 
 
 def z_score_residuals(residual_df):
     """Standardize residuals by the mean and standard deveiation of each condition
```

### Comparing `anchors-0.3.0/anchors.egg-info/PKG-INFO` & `anchors-0.3.1/anchors.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,88 +1,89 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: anchors
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python package for calculating scores from ancnchor or modifier screens
 Home-page: https://github.com/gpp-rnd/anchors
 Author: Peter Carl DeWeirdt
 Author-email: petedeweirdt@gmail.com
 License: MIT license
-Description: =======
-        anchors
-        =======
-        
-        
-        .. image:: https://img.shields.io/pypi/v/anchors.svg
-                :target: https://pypi.python.org/pypi/anchors
-        
-        .. image:: https://img.shields.io/travis/gpp-rnd/anchors.svg
-                :target: https://travis-ci.com/gpp-rnd/anchors
-        
-        .. image:: https://readthedocs.org/projects/anchors/badge/?version=latest
-                :target: https://anchors.readthedocs.io/en/latest/?badge=latest
-                :alt: Documentation Status
-        
-        
-        
-        
-        Python package for calculating scores from ancnchor or modifier screens
-        
-        
-        * Free software: MIT license
-        * Documentation: https://anchors.readthedocs.io.
-        
-        Tutorial
-        --------
-        To install::
-        
-            $ pip install anchors
-        
-        Basic Usage
-        ^^^^^^^^^^^
-        .. code:: python
-        
-            import pandas as pd
-            from anchors import get_guide_residuals, get_gene_residuals
-            lfc_df = pd.read_csv('https://raw.githubusercontent.com/PeterDeWeirdt/anchor_screen_parp_lfcs/master/parp_example_lfcs.csv')
-            refernce_condition_df = pd.read_csv('https://raw.githubusercontent.com/PeterDeWeirdt/anchor_screen_parp_lfcs/master/parp_example_mapping.csv')
-            guide_residuals, model_info, model_fit_plots = get_guide_residuals(lfc_df, refernce_condition_df)
-            guide_mapping_df = pd.read_csv('https://raw.githubusercontent.com/PeterDeWeirdt/anchor_screen_parp_lfcs/master/brunello_guide_map.csv')
-            gene_residuals = get_gene_residuals(guide_residuals, guide_mapping_df)
-        
-        Features
-        --------
-        
-        * TODO
-        
-        Credits
-        -------
-        
-        This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
-        
-        .. _Cookiecutter: https://github.com/audreyr/cookiecutter
-        .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
-        
-        
-        =======
-        History
-        =======
-        
-        0.1.0 (2020-09-21)
-        ------------------
-        
-        * First release on PyPI.
-        
-        0.3.0 (2020-09-21)
-        ------------------
-        
-        * Calculate guide and gene residuals.
-        
 Keywords: anchors
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.5
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+=======
+anchors
+=======
+
+
+.. image:: https://img.shields.io/pypi/v/anchors.svg
+        :target: https://pypi.python.org/pypi/anchors
+
+.. image:: https://img.shields.io/travis/gpp-rnd/anchors.svg
+        :target: https://travis-ci.com/gpp-rnd/anchors
+
+.. image:: https://readthedocs.org/projects/anchors/badge/?version=latest
+        :target: https://anchors.readthedocs.io/en/latest/?badge=latest
+        :alt: Documentation Status
+
+
+
+
+Python package for calculating scores from ancnchor or modifier screens
+
+
+* Free software: MIT license
+* Documentation: https://anchors.readthedocs.io.
+
+Tutorial
+--------
+To install::
+
+    $ pip install anchors
+
+Basic Usage
+^^^^^^^^^^^
+.. code:: python
+
+    import pandas as pd
+    from anchors import get_guide_residuals, get_gene_residuals
+    lfc_df = pd.read_csv('https://raw.githubusercontent.com/PeterDeWeirdt/anchor_screen_parp_lfcs/master/parp_example_lfcs.csv')
+    refernce_condition_df = pd.read_csv('https://raw.githubusercontent.com/PeterDeWeirdt/anchor_screen_parp_lfcs/master/parp_example_mapping.csv')
+    guide_residuals, model_info, model_fit_plots = get_guide_residuals(lfc_df, refernce_condition_df)
+    guide_mapping_df = pd.read_csv('https://raw.githubusercontent.com/PeterDeWeirdt/anchor_screen_parp_lfcs/master/brunello_guide_map.csv')
+    gene_residuals = get_gene_residuals(guide_residuals, guide_mapping_df)
+
+Features
+--------
+
+* TODO
+
+Credits
+-------
+
+This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
+
+.. _Cookiecutter: https://github.com/audreyr/cookiecutter
+.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+
+
+=======
+History
+=======
+
+0.1.0 (2020-09-21)
+------------------
+
+* First release on PyPI.
+
+0.3.0 (2020-09-21)
+------------------
+
+* Calculate guide and gene residuals.
```

### Comparing `anchors-0.3.0/anchors.egg-info/SOURCES.txt` & `anchors-0.3.1/anchors.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anchors-0.3.0/docs/Makefile` & `anchors-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `anchors-0.3.0/docs/conf.py` & `anchors-0.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `anchors-0.3.0/docs/installation.rst` & `anchors-0.3.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `anchors-0.3.0/docs/make.bat` & `anchors-0.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `anchors-0.3.0/setup.py` & `anchors-0.3.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,10 +38,10 @@
     keywords='anchors',
     name='anchors',
     packages=find_packages(include=['anchors', 'anchors.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/gpp-rnd/anchors',
-    version='0.3.0',
+    version='0.3.1',
     zip_safe=False,
 )
```

### Comparing `anchors-0.3.0/tests/test_anchors.py` & `anchors-0.3.1/tests/test_anchors.py`

 * *Files identical despite different names*

