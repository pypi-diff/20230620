# Comparing `tmp/trustee-1.1.2.tar.gz` & `tmp/trustee-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trustee-1.1.2.tar", max compression
+gzip compressed data, was "trustee-1.1.3.tar", max compression
```

## Comparing `trustee-1.1.2.tar` & `trustee-1.1.3.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0    35149 2020-09-22 21:40:48.095653 trustee-1.1.2/LICENSE
--rw-r--r--   0        0        0     4648 2022-12-13 19:00:18.380535 trustee-1.1.2/README.md
--rw-r--r--   0        0        0     1186 2023-04-14 14:43:40.515904 trustee-1.1.2/pyproject.toml
--rw-r--r--   0        0        0       54 2022-08-27 20:26:35.936347 trustee-1.1.2/trustee/__init__.py
--rw-r--r--   0        0        0       22 2022-08-28 04:55:52.025967 trustee-1.1.2/trustee/_version.py
--rw-r--r--   0        0        0        0 2022-08-27 20:26:23.511700 trustee-1.1.2/trustee/enums/__init__.py
--rw-r--r--   0        0        0      191 2020-08-25 15:03:18.309208 trustee-1.1.2/trustee/enums/feature_type.py
--rw-r--r--   0        0        0    26667 2022-09-26 21:19:32.238773 trustee-1.1.2/trustee/main.py
--rw-r--r--   0        0        0        0 2022-08-27 20:26:16.668910 trustee-1.1.2/trustee/report/__init__.py
--rw-r--r--   0        0        0    24655 2022-08-28 00:39:48.253906 trustee-1.1.2/trustee/report/plot.py
--rw-r--r--   0        0        0    60566 2022-09-26 20:55:32.595657 trustee-1.1.2/trustee/report/trust.py
--rw-r--r--   0        0        0        0 2022-08-27 20:26:08.556222 trustee-1.1.2/trustee/utils/__init__.py
--rw-r--r--   0        0        0    15265 2022-08-15 15:55:30.591959 trustee-1.1.2/trustee/utils/const.py
--rw-r--r--   0        0        0     5255 2022-08-15 16:08:24.990459 trustee-1.1.2/trustee/utils/dataset.py
--rw-r--r--   0        0        0      962 2022-03-06 17:56:36.811550 trustee-1.1.2/trustee/utils/log.py
--rw-r--r--   0        0        0      880 2021-06-29 22:34:28.093972 trustee-1.1.2/trustee/utils/persist.py
--rw-r--r--   0        0        0    13134 2022-08-07 22:44:17.450841 trustee-1.1.2/trustee/utils/plot.py
--rw-r--r--   0        0        0     2972 2023-04-14 14:35:56.230834 trustee-1.1.2/trustee/utils/rootpath.py
--rw-r--r--   0        0        0     6699 2022-08-27 02:52:29.080356 trustee-1.1.2/trustee/utils/tree.py
--rw-r--r--   0        0        0     5832 1970-01-01 00:00:00.000000 trustee-1.1.2/setup.py
--rw-r--r--   0        0        0     6106 1970-01-01 00:00:00.000000 trustee-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2020-09-22 21:40:48.095653 trustee-1.1.3/LICENSE
+-rw-r--r--   0        0        0     4618 2022-08-28 04:08:57.021619 trustee-1.1.3/README.md
+-rw-r--r--   0        0        0     1179 2022-08-28 04:15:02.737166 trustee-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0       54 2022-08-27 20:26:35.936347 trustee-1.1.3/trustee/__init__.py
+-rw-r--r--   0        0        0       22 2022-08-28 03:52:06.882355 trustee-1.1.3/trustee/_version.py
+-rw-r--r--   0        0        0        0 2022-08-27 20:26:23.511700 trustee-1.1.3/trustee/enums/__init__.py
+-rw-r--r--   0        0        0      191 2020-08-25 15:03:18.309208 trustee-1.1.3/trustee/enums/feature_type.py
+-rw-r--r--   0        0        0    15586 2022-08-28 00:36:20.656356 trustee-1.1.3/trustee/main.py
+-rw-r--r--   0        0        0        0 2022-08-27 20:26:16.668910 trustee-1.1.3/trustee/report/__init__.py
+-rw-r--r--   0        0        0    24655 2022-08-28 00:39:48.253906 trustee-1.1.3/trustee/report/plot.py
+-rw-r--r--   0        0        0    51820 2022-08-28 01:31:14.952085 trustee-1.1.3/trustee/report/trust.py
+-rw-r--r--   0        0        0        0 2022-08-27 20:26:08.556222 trustee-1.1.3/trustee/utils/__init__.py
+-rw-r--r--   0        0        0    15265 2022-08-15 15:55:30.591959 trustee-1.1.3/trustee/utils/const.py
+-rw-r--r--   0        0        0     5255 2022-08-15 16:08:24.990459 trustee-1.1.3/trustee/utils/dataset.py
+-rw-r--r--   0        0        0      962 2022-03-06 17:56:36.811550 trustee-1.1.3/trustee/utils/log.py
+-rw-r--r--   0        0        0      880 2021-06-29 22:34:28.093972 trustee-1.1.3/trustee/utils/persist.py
+-rw-r--r--   0        0        0    13134 2022-08-07 22:44:17.450841 trustee-1.1.3/trustee/utils/plot.py
+-rw-r--r--   0        0        0     6699 2022-08-27 02:52:29.080356 trustee-1.1.3/trustee/utils/tree.py
+-rw-r--r--   0        0        0     5730 2022-08-28 04:15:05.730326 trustee-1.1.3/setup.py
+-rw-r--r--   0        0        0     5980 2022-08-28 04:15:05.731495 trustee-1.1.3/PKG-INFO
```

### Comparing `trustee-1.1.2/LICENSE` & `trustee-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `trustee-1.1.2/README.md` & `trustee-1.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 clf = RandomForestClassifier(n_estimators=100)
 clf.fit(X_train, y_train)
 y_pred = clf.predict(X_test)
 
 trustee = ClassificationTrustee(expert=clf)
 trustee.fit(X_train, y_train, num_iter=50, num_stability_iter=10, samples_size=0.3, verbose=True)
-dt, pruned_dt, agreement, reward = trustee.explain()
+dt = trustee.explain()
 dt_y_pred = dt.predict(X_test)
 
 print("Model explanation global fidelity report:")
 print(classification_report(y_pred, dt_y_pred))
 print("Model explanation score report:")
 print(classification_report(y_test, dt_y_pred))
 ```
```

### Comparing `trustee-1.1.2/pyproject.toml` & `trustee-1.1.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trustee"
-version = "1.1.2"
+version = "1.1.3"
 readme = "README.md"
 description = "This package implements the Trustee framework to extract decision tree explanation from black-box ML models."
 homepage = "https://trusteeml.github.io"
 repository = "https://github.com/TrusteeML/trustee"
 authors = ["Arthur Selle Jacobs <asjacobs@inf.ufrgs.br>"]
 packages = [ { include = "trustee"} ]
 classifiers = [
@@ -19,23 +19,23 @@
 [tool.poetry.dependencies]
 python = ">=3.7"
 numpy = ">=1.19.0"
 scipy = "^1.4.1"
 pandas = "^1.1.0"
 scikit-learn = ">=0.23.2"
 matplotlib = "^3.3.1"
+rootpath = "^0.1.1"
 setuptools = "^57.0.0"
 prettytable = "3.0.0"
 termcolor = "^1.1.0"
 graphviz = ">=0.8.1"
-furo = "^2022.6.21"
-sphinxemoji = "^0.2.0"
-sphinx-gallery = "^0.11.1"
 
 [tool.poetry.dev-dependencies]
+furo = "^2022.6.21"
+sphinxemoji = "^0.2.0"
 Sphinx = "^5.1.1"
 
 [tool.black]
 line-length = 120
 
 [build-system]
 requires = ["poetry>=0.12", "setuptools>=^57.0.0"]
```

### Comparing `trustee-1.1.2/trustee/report/plot.py` & `trustee-1.1.3/trustee/report/plot.py`

 * *Files identical despite different names*

### Comparing `trustee-1.1.2/trustee/report/trust.py` & `trustee-1.1.3/trustee/report/trust.py`

 * *Files 23% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     plot_stability_heatmap,
     plot_dts_fidelity_by_size,
     plot_accuracy_by_feature_removed,
 )
 
 
 class TrustReport:
-    """Class to generate Trust Report."""
+    """Class to generate trust report"""
 
     def __init__(
         self,
         blackbox,
         X=None,
         y=None,
         X_train=None,
@@ -63,121 +63,15 @@
         logger=None,
         verbose=False,
         class_names=None,
         feature_names=None,
         is_classify=True,
     ):
         """
-        Builds Trust Report for given blackbox model using the Trustee method
-        to extract whitebox explanations as Decision Trees.
-
-        Parameters
-        ----------
-        blackbox: object
-            The ML blackbox model to analyze. The expert model must have a `predict` method call implemented for
-            Trustee to work properly, unless explicitly stated otherwise using the `predict_method_name`.
-
-        X: {array-like, sparse matrix} of shape (n_samples, n_features)
-            The training input samples. Internally, it will be converted to a pandas DataFrame.
-            Either (X, y) or (X_train, X_test, y_train, y_test) must be provided.
-
-        y: array-like of shape (n_samples,) or (n_samples, n_outputs)
-            The target values for X (class labels in classification, real numbers in regression).
-            Internally, it will be converted to a pandas Series.
-            Either (X, y) or (X_train, X_test, y_train, y_test) must be provided.
-
-        X_train: {array-like, sparse matrix} of shape (n_samples, n_features)
-            The training input samples. Internally, it will be converted to a pandas DataFrame.
-            Use this argument if a fixed train-test split is to be used.
-            Either (X, y) or (X_train, X_test, y_train, y_test) must be provided.
-
-        X_test: {array-like, sparse matrix} of shape (n_samples, n_features)
-            The training input samples. Internally, it will be converted to a pandas DataFrame.
-            Use this argument if a fixed train-test split is to be used.
-            Either (X, y) or (X_train, X_test, y_train, y_test) must be provided.
-
-        y_train: array-like of shape (n_samples,) or (n_samples, n_outputs)
-            The target values for X (class labels in classification, real numbers in regression).
-            Internally, it will be converted to a pandas Series.
-            Use this argument if a fixed train-test split is to be used.
-            Either (X, y) or (X_train, X_test, y_train, y_test) must be provided.
-
-        y: array-like of shape (n_samples,) or (n_samples, n_outputs)
-            The target values for X (class labels in classification, real numbers in regression).
-            Internally, it will be converted to a pandas Series.
-            Use this argument if a fixed train-test split is to be used.
-            Either (X, y) or (X_train, X_test, y_train, y_test) must be provided.
-
-        max_iter: int, default=10
-            Number of iterations to repeat several analyses in the Trust Report,
-            including feature removal and branch analysis.
-
-        num_pruning_iter: int, default=10
-            Number of iterations to repeat the pruning analysis.
-
-        train_size: float or int, default=0.7
-            If float, should be between 0.0 and 1.0 and represent the proportion of the dataset
-            to include in the train split. If int, represents the absolute number of train samples.
-
-        predict_method_name: str, default="predict"
-            The method interface to use to get predictions from the expert model.
-            If no value is passed, the default `predict` interface is used.
-
-        trustee_num_iter: int, default=50
-            Number of iterations to repeat Trustee inner-loop for.
-
-        trustee_num_stability_iter: int, default=5
-            Number of stability to repeat Trustee stabilization outer-loop for.
-
-        trustee_samples_size: float, default=None
-            The fraction of the training dataset to use to train the student decision tree model.
-            If None, the value is automatically set to the `num_samples` provided value.
-
-        trustee_max_leaf_nodes: int, default=None
-            Grow a tree with max_leaf_nodes in best-first fashion. Best nodes are defined as
-            relative reduction in impurity. If None then unlimited number of leaf nodes.
-
-        trustee_max_depth: int, default=None
-            The maximum depth of the tree. If None, then nodes are expanded until all leaves are pure.
-
-        trustee_ccp_alpha: float, default=0.0
-            Complexity parameter used for Minimal Cost-Complexity Pruning. The subtree with the
-            largest cost complexity that is smaller than ccp_alpha will be chosen. By default,
-            no pruning is performed. See Minimal Cost-Complexity Pruning here for details:
-            https://scikit-learn.org/stable/modules/tree.html#minimal-cost-complexity-pruning
-
-        analyze_branches: bool, default=False
-            Boolean indicating whether to perform the Trust Report branch analysis of Trustee explanations.
-
-        analyze_stability: bool, default=False
-            Boolean indicating whether to perform the Trust Report stability analysis of Trustee explanations.
-
-        skip_retrain: bool, default=False
-            Boolean indicating whether the Trust Report should attempt to retrain the given blackbox model.
-            Used to evaluate the impact of each feature in training by iteratively removing top features.
-            Works well for scikit-explain model, but can be troublesome for other libraries (especially AutoGluon).
-
-        top_k: int, default=10
-            Number of top-k branches, sorted by number of samples per branch, to keep after finding
-            decision tree with highest fidelity.
-
-        verbose: bool, default=False
-            Boolean indicating whether to log messages.
-
-        logger: Logger object , default=None
-            A logger object to log messages to. If none is given, the print() method will be used to log messages.
-
-        class_names: array-like of str, default=None
-            List of class names to use when plotting decision trees and graphs.
-
-        feature_names: array-like of str, default=None,
-            List of feature names to use when plotting decision trees and graphs.
-
-        is_classify: bool, default=True,
-            Whether given blackbox is a classifier or regressor. The outputted plots change depending on chosen value.
+        Builds trust report for given black-box model using the Trustee method to extract white-box explanations as Decision Trees.
         """
         self.blackbox = blackbox
         self.X = X
         self.y = y
         self.X_train = X_train
         self.X_test = X_test
         self.y_train = y_train
@@ -200,16 +94,14 @@
         self.verbose = verbose
         self.class_names = class_names
         self.feature_names = feature_names
         self.is_classify = is_classify
 
         self.step = 0
         """
-            Used for progress bar.
-
             total_steps = 
                 _prepare_data (1) + 
                 _collect_blackbox (1) +
                 _collect_trustee (1) + 
                 _collect_top_k_prunning (1) + 
                 _collect_ccp_prunning (num_pruning_iter) +
                 _collect_max_depth_prunning (num_pruning_iter) +
@@ -274,22 +166,15 @@
     def __setstate__(self, state):
         self.__dict__.update(state)
         self.logger = None
         self.blackbox = None
         self.trustee.expert = None
 
     def __str__(self):
-        """
-        Formats collected data into a report using PrettyTable.
-
-        Returns
-        -------
-        report: str
-            Formatted Trust Report.
-        """
+        """Formats collected data into a reporto using PrettyTable"""
         report = PrettyTable(title="Classification Trust Report", header=False)
 
         summary = PrettyTable(title="Summary")
         blackbox_report = PrettyTable(border=False, header=False)
         blackbox_report.align = "l"
         blackbox_report.add_row(["Model:", type(self.blackbox).__name__])
         blackbox_report.add_row(["Dataset size:", self.dataset_size])
@@ -686,43 +571,33 @@
             return f"\n{classification_report(y, y_pred, digits=3, zero_division=0)}"
 
         return f"R2 Score: {r2_score(y, y_pred)}"
 
     def _progress(self, finish=False, length=100, fill="█", end="\r"):
         """
         Call in a loop to create terminal progress bar
-
-        Parameters
-        ----------
-            finish: bool, default=False
-                Force progress bar to finish.
-
-            length: int, default=100
-                Character length of bar.
-
-            fill: str, default="█"
-                Bar fill character.
-
-            end: str, default="\r"
-                End character (e.g. "\r", "\r\n")
+        @params:
+            length      - Optional  : character length of bar (Int)
+            fill        - Optional  : bar fill character (Str)
+            end         - Optional  : end character (e.g. "\r", "\r\n") (Str)
         """
         self.step = self.step + 1
         if self.step > self.total_steps or finish:
             self.step = self.total_steps
 
         percent = f"{100 * (self.step / float(self.total_steps)):.1f}"
         filled_length = int(length * self.step // self.total_steps)
         progress_bar = fill * filled_length + "-" * (length - filled_length)
         print(f"\rProgress |{progress_bar}| {percent}% Complete", end=end)
         if self.step == self.total_steps or self.verbose:
             # if it's running verbose, log messages will get in the way, so we better print the bar multiple times
             print()
 
     def _prepare_data(self):
-        """Data preparation for Trust Report"""
+        """Data preparation for trust report"""
         log = self.logger.log if self.logger else print
 
         if self.verbose:
             log("Preparing data...")
 
         if (self.X is None and (self.X_train is None or self.X_test is None)) or (
             self.y is None and (self.y_train is None or self.y_test is None)
@@ -770,48 +645,18 @@
         self,
         X_train=None,
         X_test=None,
         trustee_num_stability_iter=None,
         trustee_ccp_alpha=0.0,
         trustee_max_leaf_nodes=None,
         trustee_max_depth=None,
+        trustee_use_features=None,
     ):
         """
-        Fits blackbox with the given X and y data, and uses Trustee to extract DT explanation
-
-        Parameters
-        ----------
-            X_train: {array-like, sparse matrix} of shape (n_samples, n_features), default=None
-                The training input samples.
-                If none is provided the default TrustReport value is used.
-
-            X_test: {array-like, sparse matrix} of shape (n_samples, n_features), default=None
-                The test input samples.
-                If none is provided the default TrustReport value is used.
-
-            trustee_num_stability_iter: int, default=None
-                Number of stability to repeat Trustee stabilization outer-loop for.
-                If none is provided the default TrustReport value is used.
-
-            trustee_ccp_alpha: float, default=0.0
-                Complexity parameter used for Minimal Cost-Complexity Pruning. The subtree with the
-                largest cost complexity that is smaller than ccp_alpha will be chosen. By default,
-                no pruning is performed. See Minimal Cost-Complexity Pruning here for details:
-                https://scikit-learn.org/stable/modules/tree.html#minimal-cost-complexity-pruning
-
-                If none is provided the default TrustReport value is used.
-
-            trustee_max_leaf_nodes: int, default=None
-                Grow a tree with max_leaf_nodes in best-first fashion. Best nodes are defined as
-                relative reduction in impurity. If None then unlimited number of leaf nodes.
-                If none is provided the default TrustReport value is used.
-
-            trustee_max_depth: int, default=None
-                The maximum depth of the tree. If None, then nodes are expanded until all leaves are pure.
-                If none is provided the default TrustReport value is used.
+        Fits blacbox with the given X and y data, and uses Trustee to extract DT explanation
         """
         log = self.logger.log if self.logger else print
 
         if self.verbose:
             log("Fitting blackbox model...")
 
         X_train = X_train if X_train is not None else self.X_train
@@ -880,25 +725,29 @@
             num_iter=self.trustee_num_iter,
             num_stability_iter=stability_iter,
             samples_size=self.trustee_sample_size,
             predict_method_name=self.predict_method_name,
             max_leaf_nodes=trustee_max_leaf_nodes if trustee_max_leaf_nodes else self.trustee_max_leaf_nodes,
             max_depth=trustee_max_depth if trustee_max_depth else self.trustee_max_depth,
             ccp_alpha=trustee_ccp_alpha if trustee_ccp_alpha else self.trustee_ccp_alpha,
+            use_features=trustee_use_features,
             verbose=self.verbose,
         )
 
         if self.verbose:
             log("Done!")
 
         dt, min_dt, agreement, reward = trustee.explain()
         if self.verbose:
             log(f"Model explanation training (agreement, fidelity): ({agreement}, {reward})")
             log(f"Top-k Prunned explanation size: {min_dt.tree_.node_count}")
 
+        if trustee_use_features:
+            X_test = X_test.iloc[:, trustee_use_features]
+
         dt_y_pred = dt.predict(X_test.values)
         min_dt_y_pred = min_dt.predict(X_test.values)
 
         if self.verbose:
             log("Model explanation global fidelity report:")
             log(self._score_report(y_pred, dt_y_pred))
             log("Top-k Model explanation global fidelity report:")
@@ -1020,16 +869,15 @@
 
         self.stability_iter = []
         for i in range(self.max_iter):
             if self.verbose:
                 log(f"Iteration {i}/{self.max_iter}")
 
             (trustee, y_pred, max_dt, max_dt_y_pred, min_dt, min_dt_y_pred) = self._fit_and_explain(
-                # prevents trustee`s outer loop from running so we can see how unstable explanations are
-                trustee_num_stability_iter=1
+                trustee_num_stability_iter=1  # prevents trustee`s outer loop from running so we can see how unstable explanations are
             )
             top_branches = trustee.get_top_branches(top_k=max_dt.get_n_leaves())
             self.stability_iter.append(
                 {
                     "max_dt": max_dt,
                     "min_dt": min_dt,
                     "max_dt_fidelity": self._score(y_pred, max_dt_y_pred),
@@ -1228,19 +1076,16 @@
 
     def _save_dts(self, output_dir, save_all=False):
         """
         Save the decision trees.
 
         Parameters
         ----------
-        output_dir: str
+        output_dir : str
             The output directory to save the decision trees.
-
-        save_all: bool, default=False
-            Whether to save all generated decision trees or just the main explanation.
         """
         log = self.logger.log if self.logger else print
         if self.verbose:
             log("Saving decision trees...")
 
         dot_data = tree.export_graphviz(
             self.max_dt,
@@ -1345,20 +1190,16 @@
 
     def plot(self, output_dir, aggregate=False):
         """
         Plot the analysis results.
 
         Parameters
         ----------
-        output_dir: str
+        output_dir : str
             The output directory to save the plots.
-
-        aggregate: bool, default=False
-            Whether to attempt to aggregate most important features based on the values seen in the data and branches.
-            Does not always work properly, but can be useful to analyze the given dataset.
         """
         log = self.logger.log if self.logger else print
         if self.verbose:
             log("Plotting...")
 
         plots_output_dir = f"{output_dir}/plots"
         if not os.path.exists(plots_output_dir):
@@ -1482,48 +1323,29 @@
 
         if self.verbose:
             log("Done!")
 
     @classmethod
     def load(cls, path):
         """
-        Load the Trust Report from a file.
+        Load the trust report from a file.
 
         Parameters
         ----------
-        path: str
+        path : str
             The path to the file.
-
-        Returns
-        -------
-        report: TrustReport
-            Loaded Trust Report from file.
         """
         report = None
         with open(path, "rb") as file:
             report = pickle.load(file)
 
         return report
 
     def save(self, output_dir, aggregate=False, save_all_dts=False):
-        """
-        Saves report and plots to output dir
-
-        Parameters
-        ----------
-        output_dir: str
-            The output directory to save the plots.
-
-        aggregate: bool, default=False
-            Whether to attempt to aggregate most important features based on the values seen in the data and branches.
-            Does not always work properly, but can be useful to analyze the given dataset.
-
-        save_all_dts: bool, default=False
-            Whether to save all generated decision trees or just the main explanation.
-        """
+        """Saves report and plots to output dir"""
         if output_dir:
             log = self.logger.log if self.logger else print
             if self.verbose:
                 log("Saving...")
 
             if not os.path.exists(output_dir):
                 os.makedirs(output_dir)
```

### Comparing `trustee-1.1.2/trustee/utils/const.py` & `trustee-1.1.3/trustee/utils/const.py`

 * *Files identical despite different names*

### Comparing `trustee-1.1.2/trustee/utils/dataset.py` & `trustee-1.1.3/trustee/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `trustee-1.1.2/trustee/utils/log.py` & `trustee-1.1.3/trustee/utils/log.py`

 * *Files identical despite different names*

### Comparing `trustee-1.1.2/trustee/utils/persist.py` & `trustee-1.1.3/trustee/utils/persist.py`

 * *Files identical despite different names*

### Comparing `trustee-1.1.2/trustee/utils/plot.py` & `trustee-1.1.3/trustee/utils/plot.py`

 * *Files identical despite different names*

### Comparing `trustee-1.1.2/trustee/utils/tree.py` & `trustee-1.1.3/trustee/utils/tree.py`

 * *Files identical despite different names*

### Comparing `trustee-1.1.2/setup.py` & `trustee-1.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,36 +4,34 @@
 packages = \
 ['trustee', 'trustee.enums', 'trustee.report', 'trustee.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['furo>=2022.6.21,<2023.0.0',
- 'graphviz>=0.8.1',
+['graphviz>=0.8.1',
  'matplotlib>=3.3.1,<4.0.0',
  'numpy>=1.19.0',
  'pandas>=1.1.0,<2.0.0',
  'prettytable==3.0.0',
+ 'rootpath>=0.1.1,<0.2.0',
  'scikit-learn>=0.23.2',
  'scipy>=1.4.1,<2.0.0',
  'setuptools>=57.0.0,<58.0.0',
- 'sphinx-gallery>=0.11.1,<0.12.0',
- 'sphinxemoji>=0.2.0,<0.3.0',
  'termcolor>=1.1.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'trustee',
-    'version': '1.1.2',
+    'version': '1.1.3',
     'description': 'This package implements the Trustee framework to extract decision tree explanation from black-box ML models.',
-    'long_description': '<img src="https://github.com/TrusteeML/trustee/blob/master/docs/_static/logo.png?raw=true" alt="Trustee" width="400"/>\n\nThis package implements the `trustee` framework to extract decision tree explanation from black-box ML models.\nFor more information, please visit the [documentation website](https://trusteeml.github.io).\n\nStandard AI/ML development pipeline extended by Trustee.\n<img alt="Trustee" src="https://github.com/TrusteeML/trustee/blob/master/docs/_static/flowchart.png?raw=true"  width="800">\n\nGetting Started\n---------------\n\nThis section contains basic information and instructions to get started with Trustee.\n\n### Python Version\n\nTrustee supports `Python >=3.7`.\n\n### Install Trustee\n\nUse the following command to install Trustee:\n\n```\n$ pip install trustee\n```\n\n### Sample Code\n\n```\nfrom sklearn import datasets\nfrom sklearn.ensemble import RandomForestClassifier\nfrom sklearn.model_selection import train_test_split\nfrom sklearn.metrics import classification_report\n\nfrom trustee import ClassificationTrustee\n\nX, y = datasets.load_iris(return_X_y=True)\nX_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.30)\n\nclf = RandomForestClassifier(n_estimators=100)\nclf.fit(X_train, y_train)\ny_pred = clf.predict(X_test)\n\ntrustee = ClassificationTrustee(expert=clf)\ntrustee.fit(X_train, y_train, num_iter=50, num_stability_iter=10, samples_size=0.3, verbose=True)\ndt, pruned_dt, agreement, reward = trustee.explain()\ndt_y_pred = dt.predict(X_test)\n\nprint("Model explanation global fidelity report:")\nprint(classification_report(y_pred, dt_y_pred))\nprint("Model explanation score report:")\nprint(classification_report(y_test, dt_y_pred))\n```\n\n### Usage Examples\n\nFor simple usage examples of Trustee and TrustReport, please check the `examples/` directory.\n\n### Other Use Cases\n\nFor other examples and use cases of how Trustee can used to scrutinize ML models, listed in the table below, please check our [Use Cases repository](https://github.com/TrusteeML/emperor).\n\n | Use Case           | Description                                                                                                                                                 |\n | ------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |\n | heartbleed\\_case/  | Trustee application to a Random Forest Classifier for an Intrustion Detection System, trained with CIC-IDS-2017 dataset pre-computed features.              |\n | kitsune\\_case/     | Trustee application to Kitsune model for anomaly detection in network traffic, trained with features extracted from Kitsune\\\'s Mirai attack trace.          |\n | iot\\_case/         | Trustee application to Random Forest Classifier to distguish IoT devices, trained with features extracted from the pcaps from the UNSW IoT Dataset.         |\n | moon\\_star\\_case/  | Trustee application to Neural Network Moon and Stars Shortcut learning toy example.                                                                         |\n | nprint\\_ids\\_case/ | Trustee application to the nPrintML AutoGluon Tabular Predictor for an Intrustion Detection System, also trained using pcaps from the CIC-IDS-2017 dataset. |\n | nprint\\_os\\_case/  | Trustee application to the nPrintML AutoGluon Tabular Predictor for OS Fingerprinting, also trained using with pcaps from the CIC-IDS-2017 dataset.         |\n | pensieve\\_case/    | Trustee application to the Pensieve RL model for adaptive bit-rate prediction, and comparison to related work Metis.                                        |\n | vpn\\_case/         | Trustee application the 1D-CNN trained to detect VPN traffic trained with the ISCX VPN-nonVPN dataset.                                                      |\n\n### Supported AI/ML Libraries\n\n | Library      | Supported          |\n | ------------ | ------------------ |\n | scikit-learn | :white_check_mark: |\n | Keras        | :white_check_mark: |\n | Tensorflow   | :white_check_mark: |\n | PyTorch      | :white_check_mark: |\n | AutoGluon    | :white_check_mark: |\n\n## Citing us\n\n```\n@inproceedings{Jacobs2022,\n\ttitle        = {AI/ML and Network Security: The Emperor has no Clothes},\n\tauthor       = {A. S. Jacobs and R. Beltiukov and W. Willinger and R. A. Ferreira and A. Gupta and L. Z. Granville},\n\tyear         = 2022,\n\tbooktitle    = {Proceedings of the 2022 ACM SIGSAC Conference on Computer and Communications Security},\n\tlocation     = {Los Angeles, CA, USA},\n\tpublisher    = {Association for Computing Machinery},\n\taddress      = {New York, NY, USA},\n\tseries       = {CCS \'22}\n}\n```',
+    'long_description': '<img src="https://github.com/TrusteeML/trustee/blob/master/docs/_static/logo.png?raw=true" alt="Trustee" width="400"/>\n\nThis package implements the `trustee` framework to extract decision tree explanation from black-box ML models.\nFor more information, please visit the [documentation website](https://trusteeml.github.io).\n\nStandard AI/ML development pipeline extended by Trustee.\n<img alt="Trustee" src="https://github.com/TrusteeML/trustee/blob/master/docs/_static/flowchart.png?raw=true"  width="800">\n\nGetting Started\n---------------\n\nThis section contains basic information and instructions to get started with Trustee.\n\n### Python Version\n\nTrustee supports `Python >=3.7`.\n\n### Install Trustee\n\nUse the following command to install Trustee:\n\n```\n$ pip install trustee\n```\n\n### Sample Code\n\n```\nfrom sklearn import datasets\nfrom sklearn.ensemble import RandomForestClassifier\nfrom sklearn.model_selection import train_test_split\nfrom sklearn.metrics import classification_report\n\nfrom trustee import ClassificationTrustee\n\nX, y = datasets.load_iris(return_X_y=True)\nX_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.30)\n\nclf = RandomForestClassifier(n_estimators=100)\nclf.fit(X_train, y_train)\ny_pred = clf.predict(X_test)\n\ntrustee = ClassificationTrustee(expert=clf)\ntrustee.fit(X_train, y_train, num_iter=50, num_stability_iter=10, samples_size=0.3, verbose=True)\ndt = trustee.explain()\ndt_y_pred = dt.predict(X_test)\n\nprint("Model explanation global fidelity report:")\nprint(classification_report(y_pred, dt_y_pred))\nprint("Model explanation score report:")\nprint(classification_report(y_test, dt_y_pred))\n```\n\n### Usage Examples\n\nFor simple usage examples of Trustee and TrustReport, please check the `examples/` directory.\n\n### Other Use Cases\n\nFor other examples and use cases of how Trustee can used to scrutinize ML models, listed in the table below, please check our [Use Cases repository](https://github.com/TrusteeML/emperor).\n\n | Use Case           | Description                                                                                                                                                 |\n | ------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |\n | heartbleed\\_case/  | Trustee application to a Random Forest Classifier for an Intrustion Detection System, trained with CIC-IDS-2017 dataset pre-computed features.              |\n | kitsune\\_case/     | Trustee application to Kitsune model for anomaly detection in network traffic, trained with features extracted from Kitsune\\\'s Mirai attack trace.          |\n | iot\\_case/         | Trustee application to Random Forest Classifier to distguish IoT devices, trained with features extracted from the pcaps from the UNSW IoT Dataset.         |\n | moon\\_star\\_case/  | Trustee application to Neural Network Moon and Stars Shortcut learning toy example.                                                                         |\n | nprint\\_ids\\_case/ | Trustee application to the nPrintML AutoGluon Tabular Predictor for an Intrustion Detection System, also trained using pcaps from the CIC-IDS-2017 dataset. |\n | nprint\\_os\\_case/  | Trustee application to the nPrintML AutoGluon Tabular Predictor for OS Fingerprinting, also trained using with pcaps from the CIC-IDS-2017 dataset.         |\n | pensieve\\_case/    | Trustee application to the Pensieve RL model for adaptive bit-rate prediction, and comparison to related work Metis.                                        |\n | vpn\\_case/         | Trustee application the 1D-CNN trained to detect VPN traffic trained with the ISCX VPN-nonVPN dataset.                                                      |\n\n### Supported AI/ML Libraries\n\n | Library      | Supported          |\n | ------------ | ------------------ |\n | scikit-learn | :white_check_mark: |\n | Keras        | :white_check_mark: |\n | Tensorflow   | :white_check_mark: |\n | PyTorch      | :white_check_mark: |\n | AutoGluon    | :white_check_mark: |\n\n## Citing us\n\n```\n@inproceedings{Jacobs2022,\n\ttitle        = {AI/ML and Network Security: The Emperor has no Clothes},\n\tauthor       = {A. S. Jacobs and R. Beltiukov and W. Willinger and R. A. Ferreira and A. Gupta and L. Z. Granville},\n\tyear         = 2022,\n\tbooktitle    = {Proceedings of the 2022 ACM SIGSAC Conference on Computer and Communications Security},\n\tlocation     = {Los Angeles, CA, USA},\n\tpublisher    = {Association for Computing Machinery},\n\taddress      = {New York, NY, USA},\n\tseries       = {CCS \'22}\n}\n```',
     'author': 'Arthur Selle Jacobs',
     'author_email': 'asjacobs@inf.ufrgs.br',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
+    'maintainer': None,
+    'maintainer_email': None,
     'url': 'https://trusteeml.github.io',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.7',
 }
```

### Comparing `trustee-1.1.2/PKG-INFO` & `trustee-1.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 Metadata-Version: 2.1
 Name: trustee
-Version: 1.1.2
+Version: 1.1.3
 Summary: This package implements the Trustee framework to extract decision tree explanation from black-box ML models.
 Home-page: https://trusteeml.github.io
 Author: Arthur Selle Jacobs
 Author-email: asjacobs@inf.ufrgs.br
 Requires-Python: >=3.7
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: furo (>=2022.6.21,<2023.0.0)
 Requires-Dist: graphviz (>=0.8.1)
 Requires-Dist: matplotlib (>=3.3.1,<4.0.0)
 Requires-Dist: numpy (>=1.19.0)
 Requires-Dist: pandas (>=1.1.0,<2.0.0)
 Requires-Dist: prettytable (==3.0.0)
+Requires-Dist: rootpath (>=0.1.1,<0.2.0)
 Requires-Dist: scikit-learn (>=0.23.2)
 Requires-Dist: scipy (>=1.4.1,<2.0.0)
 Requires-Dist: setuptools (>=57.0.0,<58.0.0)
-Requires-Dist: sphinx-gallery (>=0.11.1,<0.12.0)
-Requires-Dist: sphinxemoji (>=0.2.0,<0.3.0)
 Requires-Dist: termcolor (>=1.1.0,<2.0.0)
 Project-URL: Repository, https://github.com/TrusteeML/trustee
 Description-Content-Type: text/markdown
 
 <img src="https://github.com/TrusteeML/trustee/blob/master/docs/_static/logo.png?raw=true" alt="Trustee" width="400"/>
 
 This package implements the `trustee` framework to extract decision tree explanation from black-box ML models.
@@ -72,15 +70,15 @@
 
 clf = RandomForestClassifier(n_estimators=100)
 clf.fit(X_train, y_train)
 y_pred = clf.predict(X_test)
 
 trustee = ClassificationTrustee(expert=clf)
 trustee.fit(X_train, y_train, num_iter=50, num_stability_iter=10, samples_size=0.3, verbose=True)
-dt, pruned_dt, agreement, reward = trustee.explain()
+dt = trustee.explain()
 dt_y_pred = dt.predict(X_test)
 
 print("Model explanation global fidelity report:")
 print(classification_report(y_pred, dt_y_pred))
 print("Model explanation score report:")
 print(classification_report(y_test, dt_y_pred))
 ```
```

