# Comparing `tmp/seaborn-analyzer-0.3.0.tar.gz` & `tmp/seaborn-analyzer-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seaborn-analyzer-0.3.0.tar", last modified: Mon Jun 19 08:11:46 2023, max compression
+gzip compressed data, was "seaborn-analyzer-0.3.1.tar", last modified: Tue Jun 20 06:28:48 2023, max compression
```

## Comparing `seaborn-analyzer-0.3.0.tar` & `seaborn-analyzer-0.3.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 knakamura   (501) staff       (20)        0 2023-06-19 08:11:46.069201 seaborn-analyzer-0.3.0/
--rw-r--r--   0 knakamura   (501) staff       (20)     1522 2021-10-26 17:55:27.000000 seaborn-analyzer-0.3.0/LICENSE
--rw-r--r--   0 knakamura   (501) staff       (20)    15891 2023-06-19 08:11:46.068953 seaborn-analyzer-0.3.0/PKG-INFO
--rw-r--r--   0 knakamura   (501) staff       (20)    14461 2023-06-19 08:03:26.000000 seaborn-analyzer-0.3.0/README.rst
-drwxr-xr-x   0 knakamura   (501) staff       (20)        0 2023-06-19 08:11:46.067335 seaborn-analyzer-0.3.0/seaborn_analyzer/
--rw-r--r--   0 knakamura   (501) staff       (20)      178 2023-06-19 08:03:43.000000 seaborn-analyzer-0.3.0/seaborn_analyzer/__init__.py
--rw-r--r--   0 knakamura   (501) staff       (20)    54281 2023-06-19 07:33:33.000000 seaborn-analyzer-0.3.0/seaborn_analyzer/_cv_eval_set.py
--rw-r--r--   0 knakamura   (501) staff       (20)    82441 2023-06-19 07:44:36.000000 seaborn-analyzer-0.3.0/seaborn_analyzer/custom_class_plot.py
--rw-r--r--   0 knakamura   (501) staff       (20)    22202 2021-10-26 17:55:27.000000 seaborn-analyzer-0.3.0/seaborn_analyzer/custom_hist_plot.py
--rw-r--r--   0 knakamura   (501) staff       (20)    12128 2021-11-01 17:19:31.000000 seaborn-analyzer-0.3.0/seaborn_analyzer/custom_pair_plot.py
--rw-r--r--   0 knakamura   (501) staff       (20)    97795 2022-04-23 10:03:42.000000 seaborn-analyzer-0.3.0/seaborn_analyzer/custom_reg_plot.py
--rw-r--r--   0 knakamura   (501) staff       (20)     1635 2023-06-19 07:33:38.000000 seaborn-analyzer-0.3.0/seaborn_analyzer/multiclass_fitparams.py
-drwxr-xr-x   0 knakamura   (501) staff       (20)        0 2023-06-19 08:11:46.068508 seaborn-analyzer-0.3.0/seaborn_analyzer.egg-info/
--rw-r--r--   0 knakamura   (501) staff       (20)    15891 2023-06-19 08:11:46.000000 seaborn-analyzer-0.3.0/seaborn_analyzer.egg-info/PKG-INFO
--rw-r--r--   0 knakamura   (501) staff       (20)      477 2023-06-19 08:11:46.000000 seaborn-analyzer-0.3.0/seaborn_analyzer.egg-info/SOURCES.txt
--rw-r--r--   0 knakamura   (501) staff       (20)        1 2023-06-19 08:11:46.000000 seaborn-analyzer-0.3.0/seaborn_analyzer.egg-info/dependency_links.txt
--rw-r--r--   0 knakamura   (501) staff       (20)      155 2023-06-19 08:11:46.000000 seaborn-analyzer-0.3.0/seaborn_analyzer.egg-info/requires.txt
--rw-r--r--   0 knakamura   (501) staff       (20)       17 2023-06-19 08:11:46.000000 seaborn-analyzer-0.3.0/seaborn_analyzer.egg-info/top_level.txt
--rw-r--r--   0 knakamura   (501) staff       (20)       38 2023-06-19 08:11:46.069255 seaborn-analyzer-0.3.0/setup.cfg
--rw-r--r--   0 knakamura   (501) staff       (20)     2163 2023-06-19 08:02:59.000000 seaborn-analyzer-0.3.0/setup.py
+drwxr-xr-x   0 knakamura   (501) staff       (20)        0 2023-06-20 06:28:48.334785 seaborn-analyzer-0.3.1/
+-rw-r--r--   0 knakamura   (501) staff       (20)     1522 2021-10-26 17:55:27.000000 seaborn-analyzer-0.3.1/LICENSE
+-rw-r--r--   0 knakamura   (501) staff       (20)    15891 2023-06-20 06:28:48.334570 seaborn-analyzer-0.3.1/PKG-INFO
+-rw-r--r--   0 knakamura   (501) staff       (20)    14461 2023-06-20 06:27:32.000000 seaborn-analyzer-0.3.1/README.rst
+drwxr-xr-x   0 knakamura   (501) staff       (20)        0 2023-06-20 06:28:48.333405 seaborn-analyzer-0.3.1/seaborn_analyzer/
+-rw-r--r--   0 knakamura   (501) staff       (20)      178 2023-06-20 06:27:22.000000 seaborn-analyzer-0.3.1/seaborn_analyzer/__init__.py
+-rw-r--r--   0 knakamura   (501) staff       (20)    53653 2023-06-20 05:30:27.000000 seaborn-analyzer-0.3.1/seaborn_analyzer/_cv_eval_set.py
+-rw-r--r--   0 knakamura   (501) staff       (20)    53800 2023-06-20 05:32:06.000000 seaborn-analyzer-0.3.1/seaborn_analyzer/_cv_eval_set_sklearn.py
+-rw-r--r--   0 knakamura   (501) staff       (20)    82441 2023-06-19 07:44:36.000000 seaborn-analyzer-0.3.1/seaborn_analyzer/custom_class_plot.py
+-rw-r--r--   0 knakamura   (501) staff       (20)    22202 2021-10-26 17:55:27.000000 seaborn-analyzer-0.3.1/seaborn_analyzer/custom_hist_plot.py
+-rw-r--r--   0 knakamura   (501) staff       (20)    12128 2021-11-01 17:19:31.000000 seaborn-analyzer-0.3.1/seaborn_analyzer/custom_pair_plot.py
+-rw-r--r--   0 knakamura   (501) staff       (20)    97795 2022-04-23 10:03:42.000000 seaborn-analyzer-0.3.1/seaborn_analyzer/custom_reg_plot.py
+-rw-r--r--   0 knakamura   (501) staff       (20)     1635 2023-06-19 07:33:38.000000 seaborn-analyzer-0.3.1/seaborn_analyzer/multiclass_fitparams.py
+drwxr-xr-x   0 knakamura   (501) staff       (20)        0 2023-06-20 06:28:48.334360 seaborn-analyzer-0.3.1/seaborn_analyzer.egg-info/
+-rw-r--r--   0 knakamura   (501) staff       (20)    15891 2023-06-20 06:28:48.000000 seaborn-analyzer-0.3.1/seaborn_analyzer.egg-info/PKG-INFO
+-rw-r--r--   0 knakamura   (501) staff       (20)      518 2023-06-20 06:28:48.000000 seaborn-analyzer-0.3.1/seaborn_analyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 knakamura   (501) staff       (20)        1 2023-06-20 06:28:48.000000 seaborn-analyzer-0.3.1/seaborn_analyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 knakamura   (501) staff       (20)      155 2023-06-20 06:28:48.000000 seaborn-analyzer-0.3.1/seaborn_analyzer.egg-info/requires.txt
+-rw-r--r--   0 knakamura   (501) staff       (20)       17 2023-06-20 06:28:48.000000 seaborn-analyzer-0.3.1/seaborn_analyzer.egg-info/top_level.txt
+-rw-r--r--   0 knakamura   (501) staff       (20)       38 2023-06-20 06:28:48.334826 seaborn-analyzer-0.3.1/setup.cfg
+-rw-r--r--   0 knakamura   (501) staff       (20)     2163 2023-06-19 08:02:59.000000 seaborn-analyzer-0.3.1/setup.py
```

### Comparing `seaborn-analyzer-0.3.0/LICENSE` & `seaborn-analyzer-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `seaborn-analyzer-0.3.0/PKG-INFO` & `seaborn-analyzer-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seaborn-analyzer
-Version: 0.3.0
+Version: 0.3.1
 Summary: seaborn-analyzer: data visualization of regression, classification and distribution
 Home-page: https://github.com/c60evaporator/seaborn-analyzer
 Download-URL: https://github.com/c60evaporator/seaborn-analyzer
 Author: Kenta Nakamura
 Author-email: c60evaporator@gmail.com
 Maintainer: Kenta Nakamura
 Maintainer-email: c60evaporator@gmail.com
@@ -65,15 +65,15 @@
 If you want to know the usage of the other classes, see `API Reference
 <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#api-reference>`__ and `Examples
 <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#examples>`__
 
 ============
 Requirements
 ============
-seaborn-analyzer 0.3.0 requires
+seaborn-analyzer 0.3.1 requires
 
 * Python >=3.6
 * Numpy >=1.20.3
 * Pandas >=1.2.4
 * Matplotlib >=3.1.3
 * Seaborn >=0.11.1
 * Scipy >=1.6.3
```

### Comparing `seaborn-analyzer-0.3.0/README.rst` & `seaborn-analyzer-0.3.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 If you want to know the usage of the other classes, see `API Reference
 <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#api-reference>`__ and `Examples
 <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#examples>`__
 
 ============
 Requirements
 ============
-seaborn-analyzer 0.3.0 requires
+seaborn-analyzer 0.3.1 requires
 
 * Python >=3.6
 * Numpy >=1.20.3
 * Pandas >=1.2.4
 * Matplotlib >=3.1.3
 * Seaborn >=0.11.1
 * Scipy >=1.6.3
```

### Comparing `seaborn-analyzer-0.3.0/seaborn_analyzer/_cv_eval_set.py` & `seaborn-analyzer-0.3.1/seaborn_analyzer/_cv_eval_set.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import copy
-from joblib import Parallel
 import numpy as np
 import time
 import numbers
 from itertools import product
 from collections import defaultdict
 from sklearn import clone
 from sklearn.pipeline import Pipeline
 from sklearn.model_selection import check_cv, GridSearchCV, RandomizedSearchCV
 from sklearn.model_selection._validation import _fit_and_score, _insert_error_scores, _aggregate_score_dicts, _normalize_score_results, _translate_train_sizes, _incremental_fit_estimator
 from sklearn.utils.validation import indexable, check_random_state, _check_fit_params
 from sklearn.metrics import check_scoring
 from sklearn.metrics._scorer import _check_multimetric_scoring
 from sklearn.base import is_classifier
-from sklearn.utils.fixes import delayed
+from sklearn.utils.parallel import delayed, Parallel
 from lightgbm import LGBMModel
 from lightgbm import early_stopping, log_evaluation
 
 def init_eval_set(src_eval_set_selection, src_fit_params, X, y):
         """
         fit_paramsにeval_metricが入力されており、eval_setが入力されていないときの処理
         
@@ -95,31 +94,43 @@
             if 'verbose' in fit_params_modified.keys():
                 fit_params_modified['callbacks'].append(log_evaluation(fit_params_modified['verbose']))
                 fit_params_modified.pop('verbose')
             if 'early_stopping_rounds' in fit_params_modified.keys():
                 fit_params_modified['callbacks'].append(early_stopping(fit_params_modified['early_stopping_rounds'], False, False))
                 fit_params_modified.pop('early_stopping_rounds')
 
-def _fit_and_score_eval_set(eval_set_selection, transformer,
-                            estimator, X, y, scorer, train, test, verbose,
-                            parameters, fit_params, return_train_score=False,
-                            return_parameters=False, return_n_test_samples=False,
-                            return_times=False, return_estimator=False,
-                            split_progress=None, candidate_progress=None,
-                            error_score=np.nan,
-                            print_message=None):
+def _fit_and_score_eval_set(
+    eval_set_selection,
+    transformer,
+    estimator,
+    X, 
+    y, 
+    scorer,
+    train,
+    test,
+    verbose,
+    parameters,
+    fit_params,
+    return_train_score=False,
+    return_parameters=False,
+    return_n_test_samples=False,
+    return_times=False,
+    return_estimator=False,
+    split_progress=None,
+    candidate_progress=None,
+    error_score=np.nan,
+    ):
 
     """Fit estimator and compute scores for a given dataset split."""
     # eval_setの中から学習データ or テストデータのみを抽出
     fit_params_modified = _eval_set_selection(eval_set_selection, transformer,
                                               fit_params, train, test)
     # LightGBMのearly_stoppingをコールバック関数に変更
     _lgbm_early_stop_transform(estimator, fit_params_modified)
-    if print_message is not None:
-        print(print_message)
+
     # 学習してスコア計算
     result = _fit_and_score(estimator, X, y, scorer, train, test, verbose, parameters,
                             fit_params_modified,
                             return_train_score=return_train_score,
                             return_parameters=return_parameters, return_n_test_samples=return_n_test_samples,
                             return_times=return_times, return_estimator=return_estimator,
                             split_progress=split_progress, candidate_progress=candidate_progress,
@@ -130,19 +141,31 @@
     """estimatorがパイプラインのとき、最終学習器以外の変換器(前処理クラスのリスト)を作成"""
     if isinstance(estimator, Pipeline) and eval_set_selection != 'original':
         transformer = Pipeline([step for i, step in enumerate(estimator.steps) if i < len(estimator) - 1])
         return transformer
     else:
         return None
 
-def cross_validate_eval_set(eval_set_selection,
-                            estimator, X, y=None, groups=None, scoring=None, cv=None,
-                            n_jobs=None, verbose=0, fit_params=None,
-                            pre_dispatch='2*n_jobs', return_train_score=False,
-                            return_estimator=False, error_score=np.nan):
+def cross_validate_eval_set(
+    eval_set_selection,
+    estimator,
+    X, 
+    y=None, 
+    *,
+    groups=None, 
+    scoring=None, 
+    cv=None,
+    n_jobs=None,
+    verbose=0,
+    fit_params=None,
+    pre_dispatch='2*n_jobs',
+    return_train_score=False,
+    return_estimator=False,
+    error_score=np.nan,
+):
     """
     Evaluate a scores by cross-validation with `eval_set` argument in `fit_params`
 
     This method is suitable for calculating cross validation scores with `early_stopping_round` in XGBoost or LightGBM.
 
     Parameters
     ----------
@@ -290,18 +313,28 @@
 
     # We clone the estimator to make sure that all the folds are
     # independent, and that it is pickle-able.
     parallel = Parallel(n_jobs=n_jobs, verbose=verbose,
                         pre_dispatch=pre_dispatch)
     results = parallel(
         delayed(_fit_and_score_eval_set)(
-            eval_set_selection, transformer,
-            clone(estimator), X, y, scorers, train, test, verbose, None,
-            fit_params, return_train_score=return_train_score,
-            return_times=True, return_estimator=return_estimator,
+            eval_set_selection, 
+            transformer,
+            clone(estimator), 
+            X, 
+            y, 
+            scorers, 
+            train, 
+            test, 
+            verbose, 
+            None,
+            fit_params, 
+            return_train_score=return_train_score,
+            return_times=True, 
+            return_estimator=return_estimator,
             error_score=error_score)
         for train, test in cv.split(X, y, groups))
 
     # For callabe scoring, the return type is only know after calling. If the
     # return type is a dictionary, the error scores can now be inserted with
     # the correct key.
     if callable(scoring):
@@ -324,18 +357,29 @@
         ret['test_%s' % name] = test_scores_dict[name]
         if return_train_score:
             key = 'train_%s' % name
             ret[key] = train_scores_dict[name]
 
     return ret
 
-def cross_val_score_eval_set(eval_set_selection,
-                             estimator, X, y=None, groups=None, scoring=None,
-                             cv=None, n_jobs=None, verbose=0, fit_params=None,
-                             pre_dispatch='2*n_jobs', error_score=np.nan):
+def cross_val_score_eval_set(
+    eval_set_selection,
+    estimator, 
+    X,
+    y=None,
+    *, 
+    groups=None, 
+    scoring=None,
+    cv=None,
+    n_jobs=None,
+    verbose=0,
+    fit_params=None,
+    pre_dispatch='2*n_jobs',
+    error_score=np.nan,
+):
     """
     Evaluate a score by cross-validation with `eval_set` argument in `fit_params`
 
     This method is suitable for calculating cross validation score with `early_stopping_round` in XGBoost or LightGBM.
 
     Parameters
     ----------
@@ -449,18 +493,31 @@
                                          scoring={'score': scorer}, cv=cv,
                                          n_jobs=n_jobs, verbose=verbose,
                                          fit_params=fit_params,
                                          pre_dispatch=pre_dispatch,
                                          error_score=error_score)
     return cv_results['test_score']
 
-def validation_curve_eval_set(eval_set_selection,
-                              estimator, X, y, param_name, param_range, groups=None,
-                              cv=None, scoring=None, n_jobs=None, pre_dispatch="all",
-                              verbose=0, error_score=np.nan, fit_params=None):
+def validation_curve_eval_set(
+    eval_set_selection,
+    estimator,
+    X, 
+    y,
+    *,
+    param_name, 
+    param_range, 
+    groups=None,
+    cv=None, 
+    scoring=None, 
+    n_jobs=None, 
+    pre_dispatch="all",
+    verbose=0, 
+    error_score=np.nan, 
+    fit_params=None
+):
     """Validation curve.
 
     Determine training and test scores for varying parameter values with `eval_set` argument in `fit_params`
 
     Parameters
     ----------
     eval_set_selection : {'all', 'train', 'test', 'original', 'original_transformed'}
@@ -535,26 +592,26 @@
         Number of predispatched jobs for parallel execution (default is
         all). The option can reduce the allocated memory. The str can
         be an expression like '2*n_jobs'.
 
     verbose : int, default=0
         Controls the verbosity: the higher, the more messages.
 
-    fit_params : dict, default=None
-        Parameters to pass to the fit method of the estimator.
-
-        .. versionadded:: 0.24
-
     error_score : 'raise' or numeric, default=np.nan
         Value to assign to the score if an error occurs in estimator fitting.
         If set to 'raise', the error is raised.
         If a numeric value is given, FitFailedWarning is raised.
 
         .. versionadded:: 0.20
 
+    fit_params : dict, default=None
+        Parameters to pass to the fit method of the estimator.
+
+        .. versionadded:: 0.24
+
     Returns
     -------
     train_scores : array of shape (n_ticks, n_cv_folds)
         Scores on training sets.
 
     test_scores : array of shape (n_ticks, n_cv_folds)
         Scores on test set.
@@ -563,40 +620,63 @@
 
     cv = check_cv(cv, y, classifier=is_classifier(estimator))
     scorer = check_scoring(estimator, scoring=scoring)
 
     # 最終学習器以外の前処理変換器作成
     transformer = _make_transformer(eval_set_selection, estimator)
 
-    parallel = Parallel(n_jobs=n_jobs, pre_dispatch=pre_dispatch,
-                        verbose=verbose)
-    results = parallel(delayed(_fit_and_score_eval_set)(
-        eval_set_selection, transformer,
-        clone(estimator), X, y, scorer, train, test, verbose,
-        parameters={param_name: v}, fit_params=fit_params,
-        return_train_score=True, error_score=error_score,
-        print_message=f'Caluculating score. {param_name}={v}')
-
+    parallel = Parallel(n_jobs=n_jobs, pre_dispatch=pre_dispatch, verbose=verbose)
+    results = parallel(
+        delayed(_fit_and_score_eval_set)(
+            eval_set_selection,
+            transformer,
+            clone(estimator), 
+            X, 
+            y, 
+            scorer, 
+            train, 
+            test, 
+            verbose,
+            parameters={param_name: v}, 
+            fit_params=fit_params,
+            return_train_score=True, 
+            error_score=error_score,
+        )
         # NOTE do not change order of iteration to allow one time cv splitters
-        for train, test in cv.split(X, y, groups) for v in param_range)
+        for train, test in cv.split(X, y, groups) 
+        for v in param_range
+    )
     n_params = len(param_range)
 
     results = _aggregate_score_dicts(results)
     train_scores = results["train_scores"].reshape(-1, n_params).T
     test_scores = results["test_scores"].reshape(-1, n_params).T
 
     return train_scores, test_scores
 
-def learning_curve_eval_set(eval_set_selection,
-                            estimator, X, y, groups=None,
-                            train_sizes=np.linspace(0.1, 1.0, 5), cv=None,
-                            scoring=None, exploit_incremental_learning=False,
-                            n_jobs=None, pre_dispatch="all", verbose=0, shuffle=False,
-                            random_state=None, error_score=np.nan, return_times=False,
-                            fit_params=None):
+def learning_curve_eval_set(
+    eval_set_selection,
+    estimator,
+    X, 
+    y,
+    *,
+    groups=None,
+    train_sizes=np.linspace(0.1, 1.0, 5), 
+    cv=None,
+    scoring=None, 
+    exploit_incremental_learning=False,
+    n_jobs=None, 
+    pre_dispatch="all",
+    verbose=0, 
+    shuffle=False,
+    random_state=None, 
+    error_score=np.nan,
+    return_times=False,
+    fit_params=None,
+):
     """Learning curve.
 
     Determines cross-validated training and test scores for different training set sizes with `eval_set` argument in `fit_params`
 
     Parameters
     ----------
     eval_set_selection : {'all', 'train', 'test', 'original', 'original_transformed'}
@@ -738,50 +818,71 @@
 
     scorer = check_scoring(estimator, scoring=scoring)
 
     n_max_training_samples = len(cv_iter[0][0])
     # Because the lengths of folds can be significantly different, it is
     # not guaranteed that we use all of the available training data when we
     # use the first 'n_max_training_samples' samples.
-    train_sizes_abs = _translate_train_sizes(train_sizes,
-                                             n_max_training_samples)
+    train_sizes_abs = _translate_train_sizes(train_sizes, n_max_training_samples)
     n_unique_ticks = train_sizes_abs.shape[0]
     if verbose > 0:
         print("[learning_curve] Training set sizes: " + str(train_sizes_abs))
 
     # 最終学習器以外の前処理変換器作成
     transformer = _make_transformer(eval_set_selection, estimator)
 
-    parallel = Parallel(n_jobs=n_jobs, pre_dispatch=pre_dispatch,
-                        verbose=verbose)
+    parallel = Parallel(n_jobs=n_jobs, pre_dispatch=pre_dispatch, verbose=verbose)
 
     if shuffle:
         rng = check_random_state(random_state)
         cv_iter = ((rng.permutation(train), test) for train, test in cv_iter)
 
     if exploit_incremental_learning:
         classes = np.unique(y) if is_classifier(estimator) else None
-        out = parallel(delayed(_incremental_fit_estimator)(
-            clone(estimator), X, y, classes, train, test, train_sizes_abs,
-            scorer, verbose, return_times, error_score=error_score,
-            fit_params=fit_params)
+        out = parallel(
+            delayed(_incremental_fit_estimator)(
+                clone(estimator), 
+                X, 
+                y, 
+                classes, 
+                train, 
+                test, 
+                train_sizes_abs,
+                scorer, 
+                verbose, 
+                return_times, 
+                error_score=error_score,
+                fit_params=fit_params
+            )
             for train, test in cv_iter
         )
         out = np.asarray(out).transpose((2, 1, 0))
     else:
         train_test_proportions = []
         for train, test in cv_iter:
             for n_train_samples in train_sizes_abs:
                 train_test_proportions.append((train[:n_train_samples], test))
 
-        results = parallel(delayed(_fit_and_score_eval_set)(
-            eval_set_selection, transformer,
-            clone(estimator), X, y, scorer, train, test, verbose,
-            parameters=None, fit_params=fit_params, return_train_score=True,
-            error_score=error_score, return_times=return_times)
+        results = parallel(
+            delayed(_fit_and_score_eval_set)(
+                eval_set_selection, 
+                transformer,
+                clone(estimator), 
+                X, 
+                y, 
+                scorer, 
+                train, 
+                test, 
+                verbose,
+                parameters=None, 
+                fit_params=fit_params, 
+                return_train_score=True,
+                error_score=error_score, 
+                return_times=return_times
+            )
             for train, test in train_test_proportions
         )
         results = _aggregate_score_dicts(results)
         train_scores = results["train_scores"].reshape(-1, n_unique_ticks).T
         test_scores = results["test_scores"].reshape(-1, n_unique_ticks).T
         out = [train_scores, test_scores]
 
@@ -817,29 +918,39 @@
             If "test", select test data from `X` and `y` using cv.split().
 
             If "original", use raw `eval_set`.
 
             If "original_transformed", use `eval_set` transformed by fit_transform() of pipeline if `estimater` is pipeline.
 
         X : array-like of shape (n_samples, n_features)
-            Training vector, where n_samples is the number of samples and
-            n_features is the number of features.
+            Training vector, where `n_samples` is the number of samples and
+            `n_features` is the number of features.
 
         y : array-like of shape (n_samples, n_output) \
             or (n_samples,), default=None
             Target relative to X for classification or regression;
             None for unsupervised learning.
 
         groups : array-like of shape (n_samples,), default=None
             Group labels for the samples used while splitting the dataset into
             train/test set. Only used in conjunction with a "Group" :term:`cv`
             instance (e.g., :class:`~sklearn.model_selection.GroupKFold`).
 
         **fit_params : dict of str -> object
-            Parameters passed to the ``fit`` method of the estimator
+            Parameters passed to the `fit` method of the estimator.
+
+            If a fit parameter is an array-like whose length is equal to
+            `num_samples` then it will be split across CV groups along with `X`
+            and `y`. For example, the :term:`sample_weight` parameter is split
+            because `len(sample_weights) = len(X)`.
+
+        Returns
+        -------
+        self : object
+            Instance of fitted estimator.
         """
         estimator = self.estimator
         refit_metric = "score"
 
         if callable(self.scoring):
             scorers = self.scoring
         elif self.scoring is None or isinstance(self.scoring, str):
@@ -856,88 +967,95 @@
         n_splits = cv_orig.get_n_splits(X, y, groups)
 
         base_estimator = clone(self.estimator)
 
         # 最終学習器以外の前処理変換器作成
         transformer = _make_transformer(eval_set_selection, estimator)
 
-        parallel = Parallel(n_jobs=self.n_jobs,
-                            pre_dispatch=self.pre_dispatch)
+        parallel = Parallel(n_jobs=self.n_jobs, pre_dispatch=self.pre_dispatch)
 
-        fit_and_score_kwargs = dict(scorer=scorers,
-                                    fit_params=fit_params,
-                                    return_train_score=self.return_train_score,
-                                    return_n_test_samples=True,
-                                    return_times=True,
-                                    return_parameters=False,
-                                    error_score=self.error_score,
-                                    verbose=self.verbose)
+        fit_and_score_kwargs = dict(
+            scorer=scorers,
+            fit_params=fit_params,
+            return_train_score=self.return_train_score,
+            return_n_test_samples=True,
+            return_times=True,
+            return_parameters=False,
+            error_score=self.error_score,
+            verbose=self.verbose,
+        )
         results = {}
         with parallel:
             all_candidate_params = []
             all_out = []
             all_more_results = defaultdict(list)
 
-            def evaluate_candidates(candidate_params, cv=None,
-                                    more_results=None):
+            def evaluate_candidates(candidate_params, cv=None, more_results=None):
                 cv = cv or cv_orig
                 candidate_params = list(candidate_params)
                 n_candidates = len(candidate_params)
 
                 if self.verbose > 0:
-                    print("Fitting {0} folds for each of {1} candidates,"
+                    print(
+                        "Fitting {0} folds for each of {1} candidates,"
                           " totalling {2} fits".format(
-                              n_splits, n_candidates, n_candidates * n_splits))
-
-                out = parallel(delayed(_fit_and_score_eval_set)(
-                                        eval_set_selection, transformer,
-                                        clone(base_estimator),
-                                        X, y,
-                                        train=train, test=test,
-                                        parameters=parameters,
-                                        split_progress=(
-                                            split_idx,
-                                            n_splits),
-                                        candidate_progress=(
-                                            cand_idx,
-                                            n_candidates),
-                                        print_message=f'cand={cand_idx}/{n_candidates}, cv={split_idx}: {parameters}',
-                                        **fit_and_score_kwargs)
-                               for (cand_idx, parameters),
-                                   (split_idx, (train, test)) in product(
-                                   enumerate(candidate_params),
-                                   enumerate(cv.split(X, y, groups))))
+                              n_splits, n_candidates, n_candidates * n_splits
+                        )
+                    )
+
+                out = parallel(
+                    delayed(_fit_and_score_eval_set)(
+                        eval_set_selection, 
+                        transformer,
+                        clone(base_estimator),
+                        X, 
+                        y,
+                        train=train, 
+                        test=test,
+                        parameters=parameters,
+                        split_progress=(split_idx, n_splits),
+                        candidate_progress=(cand_idx, n_candidates),
+                        **fit_and_score_kwargs,
+                    )
+                    for (cand_idx, parameters), (split_idx, (train, test)) in product(
+                        enumerate(candidate_params),enumerate(cv.split(X, y, groups))
+                    )
+                )
 
                 if len(out) < 1:
-                    raise ValueError('No fits were performed. '
-                                     'Was the CV iterator empty? '
-                                     'Were there no candidates?')
+                    raise ValueError(
+                        "No fits were performed. "
+                        "Was the CV iterator empty? "
+                        "Were there no candidates?"
+                    )
                 elif len(out) != n_candidates * n_splits:
-                    raise ValueError('cv.split and cv.get_n_splits returned '
-                                     'inconsistent results. Expected {} '
-                                     'splits, got {}'
-                                     .format(n_splits,
-                                             len(out) // n_candidates))
+                    raise ValueError(
+                        "cv.split and cv.get_n_splits returned "
+                        "inconsistent results. Expected {} "
+                        "splits, got {}".format(n_splits, len(out) // n_candidates)
+                    )
 
                 # For callable self.scoring, the return type is only know after
                 # calling. If the return type is a dictionary, the error scores
                 # can now be inserted with the correct key. The type checking
                 # of out will be done in `_insert_error_scores`.
                 if callable(self.scoring):
                     _insert_error_scores(out, self.error_score)
+
                 all_candidate_params.extend(candidate_params)
                 all_out.extend(out)
+
                 if more_results is not None:
                     for key, value in more_results.items():
                         all_more_results[key].extend(value)
 
                 nonlocal results
                 results = self._format_results(
-                    all_candidate_params, n_splits, all_out,
-                    all_more_results)
+                    all_candidate_params, n_splits, all_out, all_more_results
+                )
 
                 return results
 
             self._run_search(evaluate_candidates)
 
             # multimetric is determined here because in the case of a callable
             # self.scoring the return type is only known after calling
@@ -949,43 +1067,42 @@
                 self._check_refit_for_multimetric(first_test_score)
                 refit_metric = self.refit
 
         # For multi-metric evaluation, store the best_index_, best_params_ and
         # best_score_ iff refit is one of the scorer names
         # In single metric evaluation, refit_metric is "score"
         if self.refit or not self.multimetric_:
-            # If callable, refit is expected to return the index of the best
-            # parameter set.
-            if callable(self.refit):
-                self.best_index_ = self.refit(results)
-                if not isinstance(self.best_index_, numbers.Integral):
-                    raise TypeError('best_index_ returned is not an integer')
-                if (self.best_index_ < 0 or
-                   self.best_index_ >= len(results["params"])):
-                    raise IndexError('best_index_ index out of range')
-            else:
-                self.best_index_ = results["rank_test_%s"
-                                           % refit_metric].argmin()
-                self.best_score_ = results["mean_test_%s" % refit_metric][
-                                           self.best_index_]
+            self.best_index_ = self._select_best_index(
+                self.refit, refit_metric, results
+            )
+            if not callable(self.refit):
+                # With a non-custom callable, we can select the best score
+                # based on the best index
+                self.best_score_ = results[f"mean_test_{refit_metric}"][
+                    self.best_index_
+                ]
             self.best_params_ = results["params"][self.best_index_]
 
         if self.refit:
             # we clone again after setting params in case some
             # of the params are estimators as well.
-            self.best_estimator_ = clone(clone(base_estimator).set_params(
-                **self.best_params_))
+            self.best_estimator_ = clone(
+                clone(base_estimator).set_params(**self.best_params_)
+            )
             refit_start_time = time.time()
             if y is not None:
                 self.best_estimator_.fit(X, y, **fit_params)
             else:
                 self.best_estimator_.fit(X, **fit_params)
             refit_end_time = time.time()
             self.refit_time_ = refit_end_time - refit_start_time
 
+            if hasattr(self.best_estimator_, "feature_names_in_"):
+                self.feature_names_in_ = self.best_estimator_.feature_names_in_
+
         # Store the only scorer not as a dict for single metric evaluation
         self.scorer_ = scorers
 
         self.cv_results_ = results
         self.n_splits_ = n_splits
 
         return self
@@ -998,41 +1115,51 @@
             X, y=None, groups=None, **fit_params):
         """Run fit with all sets of parameters.
 
         Parameters
         ----------
         eval_set_selection : {'all', 'train', 'test', 'original', 'original_transformed'}
             Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LightGBM or XGBoost.
-            
+                
             If "all", use all data in `X` and `y`.
 
             If "train", select train data from `X` and `y` using cv.split().
 
             If "test", select test data from `X` and `y` using cv.split().
 
             If "original", use raw `eval_set`.
 
             If "original_transformed", use `eval_set` transformed by fit_transform() of pipeline if `estimater` is pipeline.
 
         X : array-like of shape (n_samples, n_features)
-            Training vector, where n_samples is the number of samples and
-            n_features is the number of features.
+            Training vector, where `n_samples` is the number of samples and
+            `n_features` is the number of features.
 
         y : array-like of shape (n_samples, n_output) \
             or (n_samples,), default=None
             Target relative to X for classification or regression;
             None for unsupervised learning.
 
         groups : array-like of shape (n_samples,), default=None
             Group labels for the samples used while splitting the dataset into
             train/test set. Only used in conjunction with a "Group" :term:`cv`
             instance (e.g., :class:`~sklearn.model_selection.GroupKFold`).
 
         **fit_params : dict of str -> object
-            Parameters passed to the ``fit`` method of the estimator
+            Parameters passed to the `fit` method of the estimator.
+
+            If a fit parameter is an array-like whose length is equal to
+            `num_samples` then it will be split across CV groups along with `X`
+            and `y`. For example, the :term:`sample_weight` parameter is split
+            because `len(sample_weights) = len(X)`.
+
+        Returns
+        -------
+        self : object
+            Instance of fitted estimator.
         """
         estimator = self.estimator
         refit_metric = "score"
 
         if callable(self.scoring):
             scorers = self.scoring
         elif self.scoring is None or isinstance(self.scoring, str):
@@ -1049,88 +1176,95 @@
         n_splits = cv_orig.get_n_splits(X, y, groups)
 
         base_estimator = clone(self.estimator)
 
         # 最終学習器以外の前処理変換器作成
         transformer = _make_transformer(eval_set_selection, estimator)
 
-        parallel = Parallel(n_jobs=self.n_jobs,
-                            pre_dispatch=self.pre_dispatch)
+        parallel = Parallel(n_jobs=self.n_jobs, pre_dispatch=self.pre_dispatch)
 
-        fit_and_score_kwargs = dict(scorer=scorers,
-                                    fit_params=fit_params,
-                                    return_train_score=self.return_train_score,
-                                    return_n_test_samples=True,
-                                    return_times=True,
-                                    return_parameters=False,
-                                    error_score=self.error_score,
-                                    verbose=self.verbose)
+        fit_and_score_kwargs = dict(
+            scorer=scorers,
+            fit_params=fit_params,
+            return_train_score=self.return_train_score,
+            return_n_test_samples=True,
+            return_times=True,
+            return_parameters=False,
+            error_score=self.error_score,
+            verbose=self.verbose,
+        )
         results = {}
         with parallel:
             all_candidate_params = []
             all_out = []
             all_more_results = defaultdict(list)
 
-            def evaluate_candidates(candidate_params, cv=None,
-                                    more_results=None):
+            def evaluate_candidates(candidate_params, cv=None, more_results=None):
                 cv = cv or cv_orig
                 candidate_params = list(candidate_params)
                 n_candidates = len(candidate_params)
 
                 if self.verbose > 0:
-                    print("Fitting {0} folds for each of {1} candidates,"
+                    print(
+                        "Fitting {0} folds for each of {1} candidates,"
                           " totalling {2} fits".format(
-                              n_splits, n_candidates, n_candidates * n_splits))
-
-                out = parallel(delayed(_fit_and_score_eval_set)(
-                                        eval_set_selection, transformer,
-                                        clone(base_estimator),
-                                        X, y,
-                                        train=train, test=test,
-                                        parameters=parameters,
-                                        split_progress=(
-                                            split_idx,
-                                            n_splits),
-                                        candidate_progress=(
-                                            cand_idx,
-                                            n_candidates),
-                                        print_message=f'cand={cand_idx}/{n_candidates}, cv={split_idx}: {parameters}',
-                                        **fit_and_score_kwargs)
-                               for (cand_idx, parameters),
-                                   (split_idx, (train, test)) in product(
-                                   enumerate(candidate_params),
-                                   enumerate(cv.split(X, y, groups))))
+                              n_splits, n_candidates, n_candidates * n_splits
+                        )
+                    )
+
+                out = parallel(
+                    delayed(_fit_and_score_eval_set)(
+                        eval_set_selection, 
+                        transformer,
+                        clone(base_estimator),
+                        X, 
+                        y,
+                        train=train, 
+                        test=test,
+                        parameters=parameters,
+                        split_progress=(split_idx, n_splits),
+                        candidate_progress=(cand_idx, n_candidates),
+                        **fit_and_score_kwargs,
+                    )
+                    for (cand_idx, parameters), (split_idx, (train, test)) in product(
+                        enumerate(candidate_params),enumerate(cv.split(X, y, groups))
+                    )
+                )
 
                 if len(out) < 1:
-                    raise ValueError('No fits were performed. '
-                                     'Was the CV iterator empty? '
-                                     'Were there no candidates?')
+                    raise ValueError(
+                        "No fits were performed. "
+                        "Was the CV iterator empty? "
+                        "Were there no candidates?"
+                    )
                 elif len(out) != n_candidates * n_splits:
-                    raise ValueError('cv.split and cv.get_n_splits returned '
-                                     'inconsistent results. Expected {} '
-                                     'splits, got {}'
-                                     .format(n_splits,
-                                             len(out) // n_candidates))
+                    raise ValueError(
+                        "cv.split and cv.get_n_splits returned "
+                        "inconsistent results. Expected {} "
+                        "splits, got {}".format(n_splits, len(out) // n_candidates)
+                    )
 
                 # For callable self.scoring, the return type is only know after
                 # calling. If the return type is a dictionary, the error scores
                 # can now be inserted with the correct key. The type checking
                 # of out will be done in `_insert_error_scores`.
                 if callable(self.scoring):
                     _insert_error_scores(out, self.error_score)
+
                 all_candidate_params.extend(candidate_params)
                 all_out.extend(out)
+
                 if more_results is not None:
                     for key, value in more_results.items():
                         all_more_results[key].extend(value)
 
                 nonlocal results
                 results = self._format_results(
-                    all_candidate_params, n_splits, all_out,
-                    all_more_results)
+                    all_candidate_params, n_splits, all_out, all_more_results
+                )
 
                 return results
 
             self._run_search(evaluate_candidates)
 
             # multimetric is determined here because in the case of a callable
             # self.scoring the return type is only known after calling
@@ -1142,43 +1276,42 @@
                 self._check_refit_for_multimetric(first_test_score)
                 refit_metric = self.refit
 
         # For multi-metric evaluation, store the best_index_, best_params_ and
         # best_score_ iff refit is one of the scorer names
         # In single metric evaluation, refit_metric is "score"
         if self.refit or not self.multimetric_:
-            # If callable, refit is expected to return the index of the best
-            # parameter set.
-            if callable(self.refit):
-                self.best_index_ = self.refit(results)
-                if not isinstance(self.best_index_, numbers.Integral):
-                    raise TypeError('best_index_ returned is not an integer')
-                if (self.best_index_ < 0 or
-                   self.best_index_ >= len(results["params"])):
-                    raise IndexError('best_index_ index out of range')
-            else:
-                self.best_index_ = results["rank_test_%s"
-                                           % refit_metric].argmin()
-                self.best_score_ = results["mean_test_%s" % refit_metric][
-                                           self.best_index_]
+            self.best_index_ = self._select_best_index(
+                self.refit, refit_metric, results
+            )
+            if not callable(self.refit):
+                # With a non-custom callable, we can select the best score
+                # based on the best index
+                self.best_score_ = results[f"mean_test_{refit_metric}"][
+                    self.best_index_
+                ]
             self.best_params_ = results["params"][self.best_index_]
 
         if self.refit:
             # we clone again after setting params in case some
             # of the params are estimators as well.
-            self.best_estimator_ = clone(clone(base_estimator).set_params(
-                **self.best_params_))
+            self.best_estimator_ = clone(
+                clone(base_estimator).set_params(**self.best_params_)
+            )
             refit_start_time = time.time()
             if y is not None:
                 self.best_estimator_.fit(X, y, **fit_params)
             else:
                 self.best_estimator_.fit(X, **fit_params)
             refit_end_time = time.time()
             self.refit_time_ = refit_end_time - refit_start_time
 
+            if hasattr(self.best_estimator_, "feature_names_in_"):
+                self.feature_names_in_ = self.best_estimator_.feature_names_in_
+
         # Store the only scorer not as a dict for single metric evaluation
         self.scorer_ = scorers
 
         self.cv_results_ = results
         self.n_splits_ = n_splits
 
         return self
```

### Comparing `seaborn-analyzer-0.3.0/seaborn_analyzer/custom_class_plot.py` & `seaborn-analyzer-0.3.1/seaborn_analyzer/custom_class_plot.py`

 * *Files identical despite different names*

### Comparing `seaborn-analyzer-0.3.0/seaborn_analyzer/custom_hist_plot.py` & `seaborn-analyzer-0.3.1/seaborn_analyzer/custom_hist_plot.py`

 * *Files identical despite different names*

### Comparing `seaborn-analyzer-0.3.0/seaborn_analyzer/custom_pair_plot.py` & `seaborn-analyzer-0.3.1/seaborn_analyzer/custom_pair_plot.py`

 * *Files identical despite different names*

### Comparing `seaborn-analyzer-0.3.0/seaborn_analyzer/custom_reg_plot.py` & `seaborn-analyzer-0.3.1/seaborn_analyzer/custom_reg_plot.py`

 * *Files identical despite different names*

### Comparing `seaborn-analyzer-0.3.0/seaborn_analyzer/multiclass_fitparams.py` & `seaborn-analyzer-0.3.1/seaborn_analyzer/multiclass_fitparams.py`

 * *Files identical despite different names*

### Comparing `seaborn-analyzer-0.3.0/seaborn_analyzer.egg-info/PKG-INFO` & `seaborn-analyzer-0.3.1/seaborn_analyzer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seaborn-analyzer
-Version: 0.3.0
+Version: 0.3.1
 Summary: seaborn-analyzer: data visualization of regression, classification and distribution
 Home-page: https://github.com/c60evaporator/seaborn-analyzer
 Download-URL: https://github.com/c60evaporator/seaborn-analyzer
 Author: Kenta Nakamura
 Author-email: c60evaporator@gmail.com
 Maintainer: Kenta Nakamura
 Maintainer-email: c60evaporator@gmail.com
@@ -65,15 +65,15 @@
 If you want to know the usage of the other classes, see `API Reference
 <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#api-reference>`__ and `Examples
 <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#examples>`__
 
 ============
 Requirements
 ============
-seaborn-analyzer 0.3.0 requires
+seaborn-analyzer 0.3.1 requires
 
 * Python >=3.6
 * Numpy >=1.20.3
 * Pandas >=1.2.4
 * Matplotlib >=3.1.3
 * Seaborn >=0.11.1
 * Scipy >=1.6.3
```

### Comparing `seaborn-analyzer-0.3.0/setup.py` & `seaborn-analyzer-0.3.1/setup.py`

 * *Files identical despite different names*

