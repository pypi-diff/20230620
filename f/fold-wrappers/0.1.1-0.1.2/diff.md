# Comparing `tmp/fold_wrappers-0.1.1.tar.gz` & `tmp/fold_wrappers-0.1.2.tar.gz`

## Comparing `fold_wrappers-0.1.1.tar` & `fold_wrappers-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 fold_wrappers-0.1.1/.flake8
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 fold_wrappers-0.1.1/.isort.cfg
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 fold_wrappers-0.1.1/.vscode/settings.json
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 fold_wrappers-0.1.1/examples/statsforecast.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 fold_wrappers-0.1.1/fold_wrappers/__init__.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 fold_wrappers-0.1.1/fold_wrappers/arch.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 fold_wrappers-0.1.1/fold_wrappers/convenience.py
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 fold_wrappers-0.1.1/fold_wrappers/lightgbm.py
--rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 fold_wrappers-0.1.1/fold_wrappers/neuralforecast.py
--rw-r--r--   0        0        0     3210 2020-02-02 00:00:00.000000 fold_wrappers-0.1.1/fold_wrappers/prophet.py
--rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 fold_wrappers-0.1.1/fold_wrappers/sktime.py
--rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 fold_wrappers-0.1.1/fold_wrappers/statsforecast.py
--rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 fold_wrappers-0.1.1/fold_wrappers/statsmodels.py
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 fold_wrappers-0.1.1/fold_wrappers/xgboost.py
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 fold_wrappers-0.1.1/.gitignore
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 fold_wrappers-0.1.1/LICENSE
--rw-r--r--   0        0        0     9467 2020-02-02 00:00:00.000000 fold_wrappers-0.1.1/README.md
--rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 fold_wrappers-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    13324 2020-02-02 00:00:00.000000 fold_wrappers-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 fold_wrappers-0.1.2/.flake8
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 fold_wrappers-0.1.2/.isort.cfg
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 fold_wrappers-0.1.2/.vscode/settings.json
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 fold_wrappers-0.1.2/examples/statsforecast.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 fold_wrappers-0.1.2/fold_wrappers/__init__.py
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 fold_wrappers-0.1.2/fold_wrappers/arch.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 fold_wrappers-0.1.2/fold_wrappers/convenience.py
+-rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 fold_wrappers-0.1.2/fold_wrappers/lightgbm.py
+-rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 fold_wrappers-0.1.2/fold_wrappers/neuralforecast.py
+-rw-r--r--   0        0        0     3210 2020-02-02 00:00:00.000000 fold_wrappers-0.1.2/fold_wrappers/prophet.py
+-rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 fold_wrappers-0.1.2/fold_wrappers/sktime.py
+-rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 fold_wrappers-0.1.2/fold_wrappers/statsforecast.py
+-rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 fold_wrappers-0.1.2/fold_wrappers/statsmodels.py
+-rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 fold_wrappers-0.1.2/fold_wrappers/xgboost.py
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 fold_wrappers-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 fold_wrappers-0.1.2/LICENSE
+-rw-r--r--   0        0        0     9467 2020-02-02 00:00:00.000000 fold_wrappers-0.1.2/README.md
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 fold_wrappers-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    13324 2020-02-02 00:00:00.000000 fold_wrappers-0.1.2/PKG-INFO
```

### Comparing `fold_wrappers-0.1.1/.vscode/settings.json` & `fold_wrappers-0.1.2/.vscode/settings.json`

 * *Files 18% similar despite different names*

```diff
@@ -15,8 +15,12 @@
     "isort.args": [
         "--profile",
         "black"
     ],
     "terminal.integrated.env.osx": {
         "PYTHONPATH": "${workspaceFolder}",
     },
+    "[python]": {
+        "editor.defaultFormatter": "ms-python.black-formatter",
+        "editor.formatOnSave": true
+    }
 }
```

### Comparing `fold_wrappers-0.1.1/examples/statsforecast.py` & `fold_wrappers-0.1.2/examples/statsforecast.py`

 * *Files identical despite different names*

### Comparing `fold_wrappers-0.1.1/fold_wrappers/arch.py` & `fold_wrappers-0.1.2/fold_wrappers/arch.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,24 +16,25 @@
 
     def __init__(
         self,
         init_args: dict,
         use_exogenous: Optional[bool] = None,
         online_mode: bool = False,
         instance: Optional[Any] = None,
+        name: Optional[str] = None,
     ) -> None:
         self.init_args = init_args
         init_args = {} if init_args is None else init_args
         self.use_exogenous = use_exogenous
         self.properties.mode = (
             Model.Properties.Mode.online
             if online_mode
             else Model.Properties.Mode.minibatch
         )
-        self.name = "Arch"
+        self.name = name or "Arch"
         self.instance = instance
 
     def fit(
         self, X: pd.DataFrame, y: pd.Series, sample_weights: Optional[pd.Series] = None
     ) -> None:
         from arch import arch_model
```

### Comparing `fold_wrappers-0.1.1/fold_wrappers/convenience.py` & `fold_wrappers-0.1.2/fold_wrappers/convenience.py`

 * *Files identical despite different names*

### Comparing `fold_wrappers-0.1.1/fold_wrappers/lightgbm.py` & `fold_wrappers-0.1.2/fold_wrappers/lightgbm.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,56 @@
 from __future__ import annotations
 
-from typing import Any, Dict, Optional, Type, Union
+from typing import Any, Callable, Optional, Type, Union
 
 import pandas as pd
+from fold.base import Tunable
 from fold.models.base import Model
 
 
-class WrapLGBM(Model):
+class WrapLGBM(Model, Tunable):
     properties = Model.Properties(requires_X=True)
 
     def __init__(
         self,
         model_class: Type,
-        init_args: Optional[Dict],
+        init_args: Optional[dict] = {},
         instance: Optional[Any] = None,
+        params_to_try: Optional[dict] = None,
+        name: Optional[str] = None,
     ) -> None:
         self.init_args = init_args
-        init_args = {} if init_args is None else init_args
         self.model_class = model_class
 
         self.model = model_class(**init_args) if instance is None else instance
         from lightgbm import LGBMClassifier, LGBMRegressor
 
         if isinstance(self.model, LGBMRegressor):
             self.properties.model_type = Model.Properties.ModelType.regressor
         elif isinstance(self.model, LGBMClassifier):
             self.properties.model_type = Model.Properties.ModelType.classifier
         else:
             raise ValueError(f"Unknown model type: {type(self.model)}")
-        self.name = self.model_class.__class__.__name__
+        self.name = name or self.model.__class__.__name__
+        self.params_to_try = params_to_try
 
     @classmethod
     def from_model(
         cls,
         model,
+        name: Optional[str] = None,
+        params_to_try: Optional[dict] = None,
     ) -> WrapLGBM:
-        return WrapLGBM(model.__class__, {}, instance=model)
+        return WrapLGBM(
+            model.__class__,
+            init_args=model.get_params(),
+            instance=model,
+            name=name,
+            params_to_try=params_to_try,
+        )
 
     def fit(
         self, X: pd.DataFrame, y: pd.Series, sample_weights: Optional[pd.Series] = None
     ) -> None:
         self.model.fit(X, y, sample_weight=sample_weights)
 
     def update(
@@ -49,11 +60,35 @@
             X,
             y,
             sample_weight=sample_weights,
             init_model=self.model.get_booster(),
         )
 
     def predict(self, X: pd.DataFrame) -> Union[pd.Series, pd.DataFrame]:
-        return pd.Series(self.model.predict(X), index=X.index)
+        predictions = pd.Series(self.model.predict(X), index=X.index).rename(
+            f"predictions_{self.name}"
+        )
+        if self.properties.model_type == Model.Properties.ModelType.classifier:
+            probabilities = pd.DataFrame(
+                data=self.model.predict_proba(X),
+                index=X.index,
+                columns=[
+                    f"probabilities_{self.name}_{item}" for item in self.model.classes_
+                ],
+            )
+            return pd.concat([predictions, probabilities], axis="columns")
+        else:
+            return predictions
 
-    def predict_in_sample(self, X: pd.DataFrame) -> Union[pd.Series, pd.DataFrame]:
-        return pd.Series(self.model.predict(X), index=X.index)
+    predict_in_sample = predict
+
+    def get_params(self) -> dict:
+        return self.model.get_params()
+
+    def clone_with_params(
+        self, parameters: dict, clone_children: Optional[Callable] = None
+    ) -> Tunable:
+        return WrapLGBM(
+            self.model_class,
+            init_args=parameters,
+            name=self.name,
+        )
```

### Comparing `fold_wrappers-0.1.1/fold_wrappers/neuralforecast.py` & `fold_wrappers-0.1.2/fold_wrappers/neuralforecast.py`

 * *Files identical despite different names*

### Comparing `fold_wrappers-0.1.1/fold_wrappers/prophet.py` & `fold_wrappers-0.1.2/fold_wrappers/prophet.py`

 * *Files identical despite different names*

### Comparing `fold_wrappers-0.1.1/fold_wrappers/sktime.py` & `fold_wrappers-0.1.2/fold_wrappers/sktime.py`

 * *Files identical despite different names*

### Comparing `fold_wrappers-0.1.1/fold_wrappers/statsforecast.py` & `fold_wrappers-0.1.2/fold_wrappers/statsforecast.py`

 * *Files identical despite different names*

### Comparing `fold_wrappers-0.1.1/fold_wrappers/statsmodels.py` & `fold_wrappers-0.1.2/fold_wrappers/statsmodels.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,25 +16,26 @@
     def __init__(
         self,
         model_class: Type,
         init_args: dict,
         use_exogenous: Optional[bool] = None,
         online_mode: bool = False,
         instance: Optional[Any] = None,
+        name: Optional[str] = None,
     ) -> None:
         self.init_args = init_args
         init_args = {} if init_args is None else init_args
         self.model_class = model_class
         self.use_exogenous = use_exogenous
         self.properties.mode = (
             Model.Properties.Mode.online
             if online_mode
             else Model.Properties.Mode.minibatch
         )
-        self.name = self.model_class.__class__.__name__
+        self.name = name or self.model_class.__class__.__name__
         self.instance = instance
 
     def fit(
         self, X: pd.DataFrame, y: pd.Series, sample_weights: Optional[pd.Series] = None
     ) -> None:
         use_exogenous = (
             is_X_available(X) if self.use_exogenous is None else self.use_exogenous
```

### Comparing `fold_wrappers-0.1.1/.gitignore` & `fold_wrappers-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `fold_wrappers-0.1.1/LICENSE` & `fold_wrappers-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fold_wrappers-0.1.1/README.md` & `fold_wrappers-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `fold_wrappers-0.1.1/pyproject.toml` & `fold_wrappers-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling"]
  
 [project]
 name = "fold-wrappers"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Mark Aron Szulyovszky", email="mark@dreamfaster.ai" },
   { name="Daniel Szemerey", email="daniel@dreamfaster.ai" },
 ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Programming Language :: Python",
@@ -131,15 +131,15 @@
 pythonpath = [
   "src"
 ]
 testpaths = ["tests"]
 
 # bumpver command: ``bumpver update --patch``
 [tool.bumpver]
-current_version = "0.1.1"
+current_version = "0.1.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "chore(Release): Bump version from {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `fold_wrappers-0.1.1/PKG-INFO` & `fold_wrappers-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fold-wrappers
-Version: 0.1.1
+Version: 0.1.2
 Summary: 3rd party model wrappers for fold.
 Project-URL: Documentation, https://dream-faster.github.io/fold-wrappers
 Project-URL: Issues, https://github.com/dream-faster/fold-wrappers/issues
 Project-URL: Source, https://github.com/dream-faster/fold-wrappers
 Author-email: Mark Aron Szulyovszky <mark@dreamfaster.ai>, Daniel Szemerey <daniel@dreamfaster.ai>
 License: MIT License
```

