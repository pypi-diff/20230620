# Comparing `tmp/ostatslib-0.5.0.tar.gz` & `tmp/ostatslib-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ostatslib-0.5.0.tar", max compression
+gzip compressed data, was "ostatslib-0.5.1.tar", max compression
```

## Comparing `ostatslib-0.5.0.tar` & `ostatslib-0.5.1.tar`

### file list

```diff
@@ -1,64 +1,63 @@
--rw-r--r--   0        0        0     1109 2023-06-08 22:51:08.653916 ostatslib-0.5.0/LICENSE
--rw-r--r--   0        0        0      606 2023-06-08 22:51:08.653916 ostatslib-0.5.0/README.md
--rw-r--r--   0        0        0        0 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/__init__.py
--rw-r--r--   0        0        0      124 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/actions/__init__.py
--rw-r--r--   0        0        0      910 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/actions/action.py
--rw-r--r--   0        0        0     8118 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/actions/actions_space.py
--rw-r--r--   0        0        0      331 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/actions/classifiers/__init__.py
--rw-r--r--   0        0        0     2524 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/actions/classifiers/decision_tree.py
--rw-r--r--   0        0        0     2750 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/actions/classifiers/linear_support_vector_classification.py
--rw-r--r--   0        0        0     2371 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/actions/classifiers/logistic_regression.py
--rw-r--r--   0        0        0     2696 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/actions/classifiers/random_forest.py
--rw-r--r--   0        0        0     2623 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/actions/classifiers/support_vector_classification.py
--rw-r--r--   0        0        0       91 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/actions/clustering/__init__.py
--rw-r--r--   0        0        0     2364 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/actions/clustering/dbscan.py
--rw-r--r--   0        0        0     1440 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/actions/clustering/k_means.py
--rw-r--r--   0        0        0      606 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/actions/exploratory_actions/__init__.py
--rw-r--r--   0        0        0      546 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/actions/exploratory_actions/_get_exploratory_reward.py
--rw-r--r--   0        0        0     1688 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/actions/exploratory_actions/get_log_rows_count.py
--rw-r--r--   0        0        0     2087 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/actions/exploratory_actions/get_response_unique_values_ratio.py
--rw-r--r--   0        0        0     1721 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/actions/exploratory_actions/infer_response_dtype.py
--rw-r--r--   0        0        0     2461 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/actions/exploratory_actions/is_response_dichotomous_check.py
--rw-r--r--   0        0        0     1900 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/actions/exploratory_actions/is_response_discrete_check.py
--rw-r--r--   0        0        0     1942 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/actions/exploratory_actions/is_response_positive_values_only_check.py
--rw-r--r--   0        0        0     1657 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/actions/exploratory_actions/is_response_quantitative_check.py
--rw-r--r--   0        0        0     3070 2023-06-08 22:51:08.653916 ostatslib-0.5.0/ostatslib/actions/exploratory_actions/time_convertible_variable_search.py
--rw-r--r--   0        0        0      464 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/actions/regression_models/__init__.py
--rw-r--r--   0        0        0     2735 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/actions/regression_models/decision_tree_regression.py
--rw-r--r--   0        0        0     5919 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/actions/regression_models/linear_regression.py
--rw-r--r--   0        0        0     2729 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/actions/regression_models/linear_support_vector_regression.py
--rw-r--r--   0        0        0     3097 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/actions/regression_models/poisson_regression.py
--rw-r--r--   0        0        0     2823 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/actions/regression_models/random_forest_regression.py
--rw-r--r--   0        0        0     2562 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/actions/regression_models/support_vector_regression.py
--rw-r--r--   0        0        0     5072 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/actions/regression_models/time_series_auto_arima.py
--rw-r--r--   0        0        0      456 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/actions/utils/__init__.py
--rw-r--r--   0        0        0      458 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/actions/utils/calculate_score_reward.py
--rw-r--r--   0        0        0     1783 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/actions/utils/explainability_rewards.py
--rw-r--r--   0        0        0     1224 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/actions/utils/model_selection.py
--rw-r--r--   0        0        0      727 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/actions/utils/reward_cap.py
--rw-r--r--   0        0        0      841 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/actions/utils/split_response_from_explanatory_variables.py
--rw-r--r--   0        0        0      473 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/actions/utils/update_state_score.py
--rw-r--r--   0        0        0     1972 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/actions/utils/validate_state.py
--rw-r--r--   0        0        0      124 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/agents/__init__.py
--rw-r--r--   0        0        0     2177 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/agents/agent.py
--rw-r--r--   0        0        0     2195 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/agents/analysis_result.py
--rw-r--r--   0        0        0     1927 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/agents/ppo_agent.py
--rw-r--r--   0        0        0      385 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/config.py
--rw-r--r--   0        0        0       73 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/environments/__init__.py
--rw-r--r--   0        0        0     2708 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/environments/gym_environment.py
--rw-r--r--   0        0        0      101 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/environments/utils/__init__.py
--rw-r--r--   0        0        0     1106 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/environments/utils/_generate_from_datacooker.py
--rw-r--r--   0        0        0     1475 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/environments/utils/_generate_from_pmlb.py
--rw-r--r--   0        0        0     3639 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/environments/utils/_generate_from_sklearn.py
--rw-r--r--   0        0        0      602 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/environments/utils/generate_training_dataset.py
--rw-r--r--   0        0        0       48 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/states/__init__.py
--rw-r--r--   0        0        0     1477 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/states/analysis_features_set.py
--rw-r--r--   0        0        0     2264 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/states/data_features_set.py
--rw-r--r--   0        0        0     1876 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/states/features_set.py
--rw-r--r--   0        0        0     3401 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/states/models_features_set.py
--rw-r--r--   0        0        0     5033 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/states/state.py
--rw-r--r--   0        0        0      604 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/states/state_iterator.py
--rw-r--r--   0        0        0       82 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/states/utils/__init__.py
--rw-r--r--   0        0        0      937 2023-06-08 22:51:08.657916 ostatslib-0.5.0/ostatslib/states/utils/init_features_set.py
--rw-r--r--   0        0        0     1061 2023-06-08 22:51:08.657916 ostatslib-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1655 1970-01-01 00:00:00.000000 ostatslib-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1109 2023-06-20 12:48:16.053874 ostatslib-0.5.1/LICENSE
+-rw-r--r--   0        0        0      606 2023-06-20 12:48:16.053874 ostatslib-0.5.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/__init__.py
+-rw-r--r--   0        0        0      124 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/actions/__init__.py
+-rw-r--r--   0        0        0      910 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/actions/action.py
+-rw-r--r--   0        0        0     8118 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/actions/actions_space.py
+-rw-r--r--   0        0        0      331 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/actions/classifiers/__init__.py
+-rw-r--r--   0        0        0     2765 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/actions/classifiers/decision_tree.py
+-rw-r--r--   0        0        0     2898 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/actions/classifiers/linear_support_vector_classification.py
+-rw-r--r--   0        0        0     2587 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/actions/classifiers/logistic_regression.py
+-rw-r--r--   0        0        0     2936 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/actions/classifiers/random_forest.py
+-rw-r--r--   0        0        0     2799 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/actions/classifiers/support_vector_classification.py
+-rw-r--r--   0        0        0       91 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/actions/clustering/__init__.py
+-rw-r--r--   0        0        0     2662 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/actions/clustering/dbscan.py
+-rw-r--r--   0        0        0     1734 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/actions/clustering/k_means.py
+-rw-r--r--   0        0        0      606 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/actions/exploratory_actions/__init__.py
+-rw-r--r--   0        0        0      546 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/actions/exploratory_actions/_get_exploratory_reward.py
+-rw-r--r--   0        0        0     1640 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/actions/exploratory_actions/get_log_rows_count.py
+-rw-r--r--   0        0        0     2251 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/actions/exploratory_actions/get_response_unique_values_ratio.py
+-rw-r--r--   0        0        0     1598 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/actions/exploratory_actions/infer_response_dtype.py
+-rw-r--r--   0        0        0     2712 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/actions/exploratory_actions/is_response_dichotomous_check.py
+-rw-r--r--   0        0        0     2138 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/actions/exploratory_actions/is_response_discrete_check.py
+-rw-r--r--   0        0        0     2143 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/actions/exploratory_actions/is_response_positive_values_only_check.py
+-rw-r--r--   0        0        0     1882 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/actions/exploratory_actions/is_response_quantitative_check.py
+-rw-r--r--   0        0        0     2992 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/actions/exploratory_actions/time_convertible_variable_search.py
+-rw-r--r--   0        0        0      464 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/actions/regression_models/__init__.py
+-rw-r--r--   0        0        0     2913 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/actions/regression_models/decision_tree_regression.py
+-rw-r--r--   0        0        0     6143 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/actions/regression_models/linear_regression.py
+-rw-r--r--   0        0        0     2893 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/actions/regression_models/linear_support_vector_regression.py
+-rw-r--r--   0        0        0     3317 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/actions/regression_models/poisson_regression.py
+-rw-r--r--   0        0        0     3001 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/actions/regression_models/random_forest_regression.py
+-rw-r--r--   0        0        0     2754 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/actions/regression_models/support_vector_regression.py
+-rw-r--r--   0        0        0     4910 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/actions/regression_models/time_series_auto_arima.py
+-rw-r--r--   0        0        0      456 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/actions/utils/__init__.py
+-rw-r--r--   0        0        0      458 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/actions/utils/calculate_score_reward.py
+-rw-r--r--   0        0        0     1783 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/actions/utils/explainability_rewards.py
+-rw-r--r--   0        0        0     1193 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/actions/utils/model_selection.py
+-rw-r--r--   0        0        0      727 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/actions/utils/reward_cap.py
+-rw-r--r--   0        0        0      841 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/actions/utils/split_response_from_explanatory_variables.py
+-rw-r--r--   0        0        0      473 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/actions/utils/update_state_score.py
+-rw-r--r--   0        0        0     1017 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/actions/utils/validate_state.py
+-rw-r--r--   0        0        0      124 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/agents/__init__.py
+-rw-r--r--   0        0        0     2177 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/agents/agent.py
+-rw-r--r--   0        0        0     2195 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/agents/analysis_result.py
+-rw-r--r--   0        0        0     2683 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/agents/ppo_agent.py
+-rw-r--r--   0        0        0      385 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/config.py
+-rw-r--r--   0        0        0       73 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/environments/__init__.py
+-rw-r--r--   0        0        0      200 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/environments/data_generators/__init__.py
+-rw-r--r--   0        0        0     1102 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/environments/data_generators/datacooker_generator.py
+-rw-r--r--   0        0        0     1471 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/environments/data_generators/pmlb_generator.py
+-rw-r--r--   0        0        0     3635 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/environments/data_generators/sklearn_generator.py
+-rw-r--r--   0        0        0     3364 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/environments/gym_environment.py
+-rw-r--r--   0        0        0       48 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/states/__init__.py
+-rw-r--r--   0        0        0     1477 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/states/analysis_features_set.py
+-rw-r--r--   0        0        0     2264 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/states/data_features_set.py
+-rw-r--r--   0        0        0     1876 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/states/features_set.py
+-rw-r--r--   0        0        0     3401 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/states/models_features_set.py
+-rw-r--r--   0        0        0     5033 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/states/state.py
+-rw-r--r--   0        0        0      604 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/states/state_iterator.py
+-rw-r--r--   0        0        0       82 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/states/utils/__init__.py
+-rw-r--r--   0        0        0      937 2023-06-20 12:48:16.057874 ostatslib-0.5.1/ostatslib/states/utils/init_features_set.py
+-rw-r--r--   0        0        0     1061 2023-06-20 12:48:16.061874 ostatslib-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1604 1970-01-01 00:00:00.000000 ostatslib-0.5.1/PKG-INFO
```

### Comparing `ostatslib-0.5.0/LICENSE` & `ostatslib-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ostatslib-0.5.0/README.md` & `ostatslib-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `ostatslib-0.5.0/ostatslib/actions/action.py` & `ostatslib-0.5.1/ostatslib/actions/action.py`

 * *Files identical despite different names*

### Comparing `ostatslib-0.5.0/ostatslib/actions/actions_space.py` & `ostatslib-0.5.1/ostatslib/actions/actions_space.py`

 * *Files identical despite different names*

### Comparing `ostatslib-0.5.0/ostatslib/actions/classifiers/decision_tree.py` & `ostatslib-0.5.1/ostatslib/actions/classifiers/decision_tree.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Decision Tree module
 """
 
+
 import operator
 from pandas import DataFrame
 from sklearn.tree import DecisionTreeClassifier
 from ostatslib import config
 from ostatslib.states import State
 
 from ..action import Action, ActionInfo, ActionResult
@@ -19,48 +20,53 @@
 
 _ACTION_NAME = "Decision Tree"
 _VALIDATIONS = [('response_variable_label', operator.truth, None),
                 ('is_response_discrete', operator.gt, 0),
                 ('decision_tree_score_reward', operator.eq, 0)]
 
 
-@validate_state(action_name=_ACTION_NAME, validator_fns=_VALIDATIONS)
 @reward_cap
 @comprehensible_model
-def _decision_tree(state: State, data: DataFrame) -> ActionResult[DecisionTreeClassifier]:
+def _action(state: State, data: DataFrame) -> ActionResult[DecisionTreeClassifier]:
     """
     Fits data to a decision tree classifier
 
     Args:
         state (State): current environment state
         data (DataFrame): data under analysis
 
     Returns:
         ActionResult[DecisionTreeClassifier]: action result
     """
+    if not validate_state(state, _VALIDATIONS):
+        return state, config.MIN_REWARD, ActionInfo(action_name=_ACTION_NAME,
+                                                    action_fn=_action,
+                                                    model=None,
+                                                    raised_exception=False)
+
     y_values, x_values = split_response_from_explanatory_variables(state, data)
     classifier: DecisionTreeClassifier = DecisionTreeClassifier()
     param_grid = {'criterion': ['gini', 'entropy', 'log_loss'],
                   'max_features': ['sqrt', 'log2', None]}
 
     try:
         classifier, score = model_selection(classifier,
                                             param_grid,
                                             x_values,
                                             y_values)
     except ValueError:
         state.set('decision_tree_score_reward', config.MIN_REWARD)
         return state, config.MIN_REWARD, ActionInfo(action_name=_ACTION_NAME,
-                                                    action_fn=_decision_tree,
+                                                    action_fn=_action,
                                                     model=None,
                                                     raised_exception=True)
 
     update_state_score(state, score)
     reward = calculate_score_reward(score)
     state.set('decision_tree_score_reward', reward)
     return state, reward, ActionInfo(action_name=_ACTION_NAME,
-                                     action_fn=_decision_tree,
+                                     action_fn=_action,
                                      model=classifier,
                                      raised_exception=False)
 
 
-decision_tree: Action[DecisionTreeClassifier] = _decision_tree
+decision_tree: Action[DecisionTreeClassifier] = _action
```

### Comparing `ostatslib-0.5.0/ostatslib/actions/classifiers/linear_support_vector_classification.py` & `ostatslib-0.5.1/ostatslib/actions/classifiers/random_forest.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,74 @@
 """
-Linear Support Vector Classification module
+Random Forest module
 """
 
 import operator
 from pandas import DataFrame
-from sklearn.svm import LinearSVC
+from sklearn.ensemble import RandomForestClassifier
 from ostatslib import config
 from ostatslib.states import State
 
 from ..action import Action, ActionInfo, ActionResult
 from ..utils import (calculate_score_reward,
                      reward_cap,
                      opaque_model,
                      split_response_from_explanatory_variables,
                      update_state_score,
                      validate_state,
                      model_selection)
 
-_ACTION_NAME = "Linear Support Vector Classification"
+_ACTION_NAME = "Random Forest"
 _VALIDATIONS = [('response_variable_label', operator.truth, None),
                 ('is_response_discrete', operator.gt, 0),
-                ('log_rows_count', operator.gt, 0),
-                ('log_rows_count', operator.lt, 0.81),
-                ('linear_support_vector_classification_score_reward', operator.eq, 0)]
+                ('response_unique_values_ratio', operator.ne, 0),
+                ('response_unique_values_ratio', operator.lt, 0.1),
+                ('random_forest_score_reward', operator.eq, 0)]
 
 
-@validate_state(action_name=_ACTION_NAME, validator_fns=_VALIDATIONS)
 @reward_cap
 @opaque_model
-def _linear_support_vector_classification(state: State, data: DataFrame) -> ActionResult[LinearSVC]:
+def _action(state: State, data: DataFrame) -> ActionResult[RandomForestClassifier]:
     """
-    Fits data to a LinearSVC model
+    Fits data to a random forest classifier
 
     Args:
         state (State): current environment state
         data (DataFrame): data under analysis
 
     Returns:
-        ActionResult[LinearSVC]: action result
+        ActionResult[RandomForestClassifier]: action result
     """
+    if not validate_state(state, _VALIDATIONS):
+        return state, config.MIN_REWARD, ActionInfo(action_name=_ACTION_NAME,
+                                                    action_fn=_action,
+                                                    model=None,
+                                                    raised_exception=False)
+
     y_values, x_values = split_response_from_explanatory_variables(state, data)
-    classifier: LinearSVC = LinearSVC()
-    param_grid = {'penalty': ['l1', 'l2'],
-                  'loss': ['squared_hinge', 'hinge']}
+    classifier: RandomForestClassifier = RandomForestClassifier()
+    param_grid = {'criterion': ['gini', 'entropy', 'log_loss'],
+                  'max_features': ['sqrt', 'log2'],
+                  'max_depth': [x_values.shape[1], 20]}
 
     try:
         classifier, score = model_selection(classifier,
                                             param_grid,
                                             x_values,
                                             y_values)
     except ValueError:
-        state.set('linear_support_vector_classification_score_reward',
-                  config.MIN_REWARD)
+        state.set('random_forest_score_reward', config.MIN_REWARD)
         return state, config.MIN_REWARD, ActionInfo(action_name=_ACTION_NAME,
-                                                    action_fn=_linear_support_vector_classification,
+                                                    action_fn=_action,
                                                     model=None,
                                                     raised_exception=True)
 
     update_state_score(state, score)
     reward = calculate_score_reward(score)
-    state.set('linear_support_vector_classification_score_reward', reward)
+    state.set('random_forest_score_reward', reward)
     return state, reward, ActionInfo(action_name=_ACTION_NAME,
-                                     action_fn=_linear_support_vector_classification,
+                                     action_fn=_action,
                                      model=classifier,
                                      raised_exception=False)
 
 
-linear_support_vector_classification: Action[LinearSVC] = _linear_support_vector_classification
+random_forest: Action[RandomForestClassifier] = _action
```

### Comparing `ostatslib-0.5.0/ostatslib/actions/classifiers/logistic_regression.py` & `ostatslib-0.5.1/ostatslib/actions/classifiers/logistic_regression.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,44 +19,49 @@
 _ACTION_NAME = "Logistic Regression"
 _VALIDATIONS = [('response_variable_label', operator.truth, None),
                 ('is_response_dichotomous', operator.gt, 0),
                 ('response_variable_label', operator.truth, None),
                 ('logistic_regression_score_reward', operator.eq, 0)]
 
 
-@validate_state(action_name=_ACTION_NAME, validator_fns=_VALIDATIONS)
 @reward_cap
 @interpretable_model
-def _logistic_regression(state: State, data: DataFrame) -> ActionResult[LogisticRegressionCV]:
+def _action(state: State, data: DataFrame) -> ActionResult[LogisticRegressionCV]:
     """
     Fits data to a logistic regression model.
 
     Args:
         state (State): current environment state
         data (DataFrame): data under analysis
 
     Returns:
         ActionResult[LogisticRegressionCV]: action result
     """
+    if not validate_state(state, _VALIDATIONS):
+        return state, config.MIN_REWARD, ActionInfo(action_name=_ACTION_NAME,
+                                                    action_fn=_action,
+                                                    model=None,
+                                                    raised_exception=False)
+
     y_values, x_values = split_response_from_explanatory_variables(state, data)
     regression = LogisticRegressionCV(cv=5)
 
     try:
         regression = regression.fit(x_values, y_values)
     except ValueError:
         state.set('logistic_regression_score_reward', config.MIN_REWARD)
         return state, config.MIN_REWARD, ActionInfo(action_name=_ACTION_NAME,
-                                                    action_fn=_logistic_regression,
+                                                    action_fn=_action,
                                                     model=None,
                                                     raised_exception=True)
 
     score: float = regression.score(x_values, y_values)
     update_state_score(state, score)
     reward: float = calculate_score_reward(score)
     state.set('logistic_regression_score_reward', reward)
     return state, reward, ActionInfo(action_name=_ACTION_NAME,
-                                     action_fn=_logistic_regression,
+                                     action_fn=_action,
                                      model=regression,
                                      raised_exception=False)
 
 
-logistic_regression: Action[LogisticRegressionCV] = _logistic_regression
+logistic_regression: Action[LogisticRegressionCV] = _action
```

### Comparing `ostatslib-0.5.0/ostatslib/actions/classifiers/random_forest.py` & `ostatslib-0.5.1/ostatslib/actions/regression_models/support_vector_regression.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,69 +1,73 @@
 """
-Random Forest module
+Support Vector Regression module
 """
 
 import operator
 from pandas import DataFrame
-from sklearn.ensemble import RandomForestClassifier
+from sklearn.svm import SVR
 from ostatslib import config
-from ostatslib.states import State
 
+from ostatslib.states import State
 from ..action import Action, ActionInfo, ActionResult
 from ..utils import (calculate_score_reward,
                      reward_cap,
                      opaque_model,
                      split_response_from_explanatory_variables,
                      update_state_score,
                      validate_state,
                      model_selection)
 
-_ACTION_NAME = "Random Forest"
-_VALIDATIONS = [('response_variable_label', operator.truth, None),
-                ('is_response_discrete', operator.gt, 0),
-                ('response_unique_values_ratio', operator.ne, 0),
-                ('response_unique_values_ratio', operator.lt, 0.1),
-                ('random_forest_score_reward', operator.eq, 0)]
+_ACTION_NAME = "Support Vector Regression"
+_VALIDATIONS = [('is_response_quantitative', operator.gt, 0),
+                ('response_variable_label', operator.truth, None),
+                ('log_rows_count', operator.gt, 0),
+                ('log_rows_count', operator.lt, 0.71),
+                ('support_vector_regression_score_reward', operator.eq, 0)]
 
 
-@validate_state(action_name=_ACTION_NAME, validator_fns=_VALIDATIONS)
 @reward_cap
 @opaque_model
-def _random_forest(state: State, data: DataFrame) -> ActionResult[RandomForestClassifier]:
+def _action(state: State, data: DataFrame) -> ActionResult[SVR]:
     """
-    Fits data to a random forest classifier
+    Fits data to a SVR model
 
     Args:
         state (State): current environment state
         data (DataFrame): data under analysis
 
     Returns:
-        ActionResult[RandomForestClassifier]: action result
+        ActionResult[SVR]: action result
     """
+    if not validate_state(state, _VALIDATIONS):
+        return state, config.MIN_REWARD, ActionInfo(action_name=_ACTION_NAME,
+                                                    action_fn=_action,
+                                                    model=None,
+                                                    raised_exception=False)
+
     y_values, x_values = split_response_from_explanatory_variables(state, data)
-    classifier: RandomForestClassifier = RandomForestClassifier()
-    param_grid = {'criterion': ['gini', 'entropy', 'log_loss'],
-                  'max_features': ['sqrt', 'log2'],
-                  'max_depth': [x_values.shape[1], 20]}
+    regressor: SVR = SVR()
+    param_grid = {'C': [1, 10, 100],
+                  'kernel': ['poly', 'rbf']}
 
     try:
-        classifier, score = model_selection(classifier,
-                                            param_grid,
-                                            x_values,
-                                            y_values)
+        regressor, score = model_selection(regressor,
+                                           param_grid,
+                                           x_values,
+                                           y_values)
     except ValueError:
-        state.set('random_forest_score_reward', config.MIN_REWARD)
+        state.set('support_vector_regression_score_reward', config.MIN_REWARD)
         return state, config.MIN_REWARD, ActionInfo(action_name=_ACTION_NAME,
-                                                    action_fn=_random_forest,
+                                                    action_fn=_action,
                                                     model=None,
                                                     raised_exception=True)
 
     update_state_score(state, score)
     reward = calculate_score_reward(score)
-    state.set('random_forest_score_reward', reward)
+    state.set('support_vector_regression_score_reward', reward)
     return state, reward, ActionInfo(action_name=_ACTION_NAME,
-                                     action_fn=_random_forest,
-                                     model=classifier,
+                                     action_fn=_action,
+                                     model=regressor,
                                      raised_exception=False)
 
 
-random_forest: Action[RandomForestClassifier] = _random_forest
+support_vector_regression: Action[SVR] = _action
```

### Comparing `ostatslib-0.5.0/ostatslib/actions/classifiers/support_vector_classification.py` & `ostatslib-0.5.1/ostatslib/actions/classifiers/support_vector_classification.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,49 +21,54 @@
 _VALIDATIONS = [('response_variable_label', operator.truth, None),
                 ('is_response_discrete', operator.gt, 0),
                 ('log_rows_count', operator.gt, 0),
                 ('log_rows_count', operator.lt, 0.71),
                 ('support_vector_classification_score_reward', operator.eq, 0)]
 
 
-@validate_state(action_name=_ACTION_NAME, validator_fns=_VALIDATIONS)
 @reward_cap
 @opaque_model
-def _support_vector_classification(state: State, data: DataFrame) -> ActionResult[SVC]:
+def _action(state: State, data: DataFrame) -> ActionResult[SVC]:
     """
     Fits data to a SVC model
 
     Args:
         state (State): current environment state
         data (DataFrame): data under analysis
 
     Returns:
         ActionResult[SVC]: action result
     """
+    if not validate_state(state, _VALIDATIONS):
+        return state, config.MIN_REWARD, ActionInfo(action_name=_ACTION_NAME,
+                                                    action_fn=_action,
+                                                    model=None,
+                                                    raised_exception=False)
+
     y_values, x_values = split_response_from_explanatory_variables(state, data)
     classifier: SVC = SVC()
     param_grid = {'C': [1, 10, 100],
                   'kernel': ['poly', 'rbf']}
 
     try:
         classifier, score = model_selection(classifier,
                                             param_grid,
                                             x_values,
                                             y_values)
     except ValueError:
         state.set('support_vector_classification_score_reward',
                   config.MIN_REWARD)
         return state, config.MIN_REWARD, ActionInfo(action_name=_ACTION_NAME,
-                                                    action_fn=_support_vector_classification,
+                                                    action_fn=_action,
                                                     model=None,
                                                     raised_exception=True)
 
     update_state_score(state, score)
     reward = calculate_score_reward(score)
     state.set('support_vector_classification_score_reward', reward)
     return state, reward, ActionInfo(action_name=_ACTION_NAME,
-                                     action_fn=_support_vector_classification,
+                                     action_fn=_action,
                                      model=classifier,
                                      raised_exception=False)
 
 
-support_vector_classification: Action[SVC] = _support_vector_classification
+support_vector_classification: Action[SVC] = _action
```

### Comparing `ostatslib-0.5.0/ostatslib/actions/clustering/dbscan.py` & `ostatslib-0.5.1/ostatslib/actions/clustering/dbscan.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,65 +5,71 @@
 import operator
 import numpy as np
 from kneed import KneeLocator
 from pandas import DataFrame
 from sklearn.cluster import DBSCAN
 from sklearn.metrics import silhouette_score
 from sklearn.neighbors import NearestNeighbors
+from ostatslib import config
 
 from ostatslib.states import State
 from ..action import Action, ActionInfo, ActionResult
 from ..utils import (calculate_score_reward,
                      reward_cap,
                      update_state_score,
                      validate_state)
 
 _ACTION_NAME = "DBSCAN"
 _VALIDATIONS = [('response_variable_label', operator.eq, ''),
                 ('clusters_count', operator.eq, 0)]
 
 
-@validate_state(action_name=_ACTION_NAME, validator_fns=_VALIDATIONS)
 @reward_cap
-def _dbscan(state: State, data: DataFrame) -> ActionResult[DBSCAN]:
+def _action(state: State, data: DataFrame) -> ActionResult[DBSCAN]:
     """
     Fits data to a DBSCAN cluster
 
     Args:
         state (State): current environment state
         data (DataFrame): data under analysis
 
     Returns:
         ActionResult[DBSCAN]: action result
     """
+    if not validate_state(state, _VALIDATIONS):
+        return state, config.MIN_REWARD, ActionInfo(action_name=_ACTION_NAME,
+                                                    action_fn=_action,
+                                                    model=None,
+                                                    raised_exception=False)
+
     max_curvature_point = __get_max_curvature_point(data)
     db_scan = DBSCAN(eps=max_curvature_point)
     db_scan.fit(data)
 
     if np.all(db_scan.labels_ == -1) or np.all(db_scan.labels_ == 0):
         score = 0
     else:
         score = silhouette_score(data, db_scan.labels_)
 
     reward: float = calculate_score_reward(score)
     update_state_score(state, score)
     return state, reward, ActionInfo(action_name=_ACTION_NAME,
-                                     action_fn=_dbscan,
+                                     action_fn=_action,
                                      model=db_scan,
                                      raised_exception=False)
 
 
 def __get_max_curvature_point(data: DataFrame) -> float:
     n_rows, n_columns = data.shape
     if n_rows < 2 * n_columns:
         min_points = 5
     elif n_rows < 10 * n_columns:
         min_points = n_columns
     else:
-        min_points = 2* n_columns
+        min_points = 2 * n_columns
 
     neighbors_fit = NearestNeighbors(
         n_neighbors=min_points, metric='euclidean').fit(data)
     distances, _ = neighbors_fit.kneighbors(data)
     distances = np.sort(distances.sum(axis=1), axis=0)
     elbow_locator = KneeLocator(
         range(0, len(distances)),
@@ -74,8 +80,8 @@
 
     if elbow_locator.elbow_y is None:
         return 0.5
 
     return elbow_locator.elbow_y
 
 
-dbscan: Action[DBSCAN] = _dbscan
+dbscan: Action[DBSCAN] = _action
```

### Comparing `ostatslib-0.5.0/ostatslib/actions/exploratory_actions/__init__.py` & `ostatslib-0.5.1/ostatslib/actions/exploratory_actions/__init__.py`

 * *Files identical despite different names*

### Comparing `ostatslib-0.5.0/ostatslib/actions/exploratory_actions/_get_exploratory_reward.py` & `ostatslib-0.5.1/ostatslib/actions/exploratory_actions/_get_exploratory_reward.py`

 * *Files identical despite different names*

### Comparing `ostatslib-0.5.0/ostatslib/actions/exploratory_actions/get_log_rows_count.py` & `ostatslib-0.5.1/ostatslib/actions/exploratory_actions/get_log_rows_count.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,31 +13,31 @@
 
 
 ROW_COUNT_UPPER_LIMIT = 150000
 LOG_COMPRESSION_CONSTANT = 5.176
 """compression rate to keep log10(150K lines) close to 1"""
 
 
-def _get_log_rows_count(state: State,
-                        data: DataFrame) -> ActionResult[None]:
+def _action(state: State,
+            data: DataFrame) -> ActionResult[None]:
     """
     Gets log rows count: log(#rows)/c, where c is a compression constant
 
     Args:
         state (State): state
         data (DataFrame): data
 
     Returns:
         ActionResult[None]: action result
     """
     log_rows_count = __calculate_log_rows_count(data)
     reward = __calculate_reward(state, log_rows_count)
     state = __update_state(state, log_rows_count)
     return state, reward, ActionInfo(action_name=_ACTION_NAME,
-                                     action_fn=_get_log_rows_count,
+                                     action_fn=_action,
                                      model=None,
                                      raised_exception=False)
 
 
 def __calculate_log_rows_count(data: DataFrame) -> float:
     rows_count = len(data.index)
 
@@ -55,8 +55,8 @@
 
 
 def __update_state(state: State, log_rows_count: float) -> State:
     state.set("log_rows_count", log_rows_count)
     return state
 
 
-get_log_rows_count: Action[None] = _get_log_rows_count
+get_log_rows_count: Action[None] = _action
```

### Comparing `ostatslib-0.5.0/ostatslib/actions/exploratory_actions/get_response_unique_values_ratio.py` & `ostatslib-0.5.1/ostatslib/actions/exploratory_actions/get_response_unique_values_ratio.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,33 +10,38 @@
 from ..action import Action, ActionInfo, ActionResult
 from ..utils import validate_state
 
 _ACTION_NAME = "Get Response Unique Values Ratio"
 _VALIDATIONS = [('response_variable_label', operator.truth, None)]
 
 
-@validate_state(action_name=_ACTION_NAME, validator_fns=_VALIDATIONS)
-def _get_response_unique_values_ratio(state: State,
-                                      data: DataFrame) -> ActionResult[None]:
+def _action(state: State,
+            data: DataFrame) -> ActionResult[None]:
     """
     Gets response unique values ratio to total rows
 
     Args:
         state (State): state
         data (DataFrame): data
 
     Returns:
         ActionResult[None]: action result
     """
+    if not validate_state(state, _VALIDATIONS):
+        return state, config.MIN_REWARD, ActionInfo(action_name=_ACTION_NAME,
+                                                    action_fn=_action,
+                                                    model=None,
+                                                    raised_exception=False)
+
     response_unique_values_ratio = __calculate_response_unique_values_ratio(state,
                                                                             data)
     reward = __calculate_reward(state, response_unique_values_ratio)
     state = __update_state(state, response_unique_values_ratio)
     return state, reward, ActionInfo(action_name=_ACTION_NAME,
-                                     action_fn=_get_response_unique_values_ratio,
+                                     action_fn=_action,
                                      model=None,
                                      raised_exception=False)
 
 
 def __calculate_response_unique_values_ratio(state: State, data: DataFrame) -> float:
     response_var_label = state.get("response_variable_label")
     response_values: Series = data[response_var_label]
@@ -52,8 +57,8 @@
 
 
 def __update_state(state: State, response_unique_values_ratio: float) -> State:
     state.set("response_unique_values_ratio", response_unique_values_ratio)
     return state
 
 
-get_response_unique_values_ratio: Action[None] = _get_response_unique_values_ratio
+get_response_unique_values_ratio: Action[None] = _action
```

### Comparing `ostatslib-0.5.0/ostatslib/actions/exploratory_actions/infer_response_dtype.py` & `ostatslib-0.5.1/ostatslib/actions/exploratory_actions/infer_response_dtype.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 from ..action import Action, ActionInfo, ActionResult
 from ..utils import validate_state
 
 _ACTION_NAME = "Infer Response DType"
 _VALIDATIONS = [('response_variable_label', operator.truth, None)]
 
 
-@validate_state(action_name=_ACTION_NAME, validator_fns=_VALIDATIONS)
-def _infer_response_dtype(state: State, data: DataFrame) -> ActionResult[None]:
+
+def _action(state: State, data: DataFrame) -> ActionResult[None]:
     """
     Infer response dtype
 
     Args:
         state (State): state
         data (DataFrame): data
 
@@ -31,22 +31,24 @@
     state_copy: State = state.copy()
     response_var_label: str = state.get("response_variable_label")
 
     try:
         response: Series = data[response_var_label]
     except KeyError:
         return state, config.MIN_REWARD, ActionInfo(action_name=_ACTION_NAME,
-                                                    action_fn=_infer_response_dtype,
+                                                    action_fn=_action,
                                                     model=None,
                                                     raised_exception=True)
 
     inferred_dtype = infer_dtype(response)
     state.set('response_inferred_dtype', inferred_dtype)
     reward = get_exploratory_reward(state, state_copy)
 
     return state, reward, ActionInfo(action_name=_ACTION_NAME,
-                                     action_fn=_infer_response_dtype,
+                                     action_fn=_action,
                                      model=None,
                                      raised_exception=False)
 
 
-infer_response_dtype: Action[None] = _infer_response_dtype
+
+
+infer_response_dtype: Action[None] = _action
```

### Comparing `ostatslib-0.5.0/ostatslib/actions/exploratory_actions/is_response_dichotomous_check.py` & `ostatslib-0.5.1/ostatslib/actions/exploratory_actions/is_response_dichotomous_check.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,42 +2,50 @@
 is_response_dichotomous_check module
 """
 
 import operator
 from pandas import DataFrame, Series
 from pandas.api.types import infer_dtype
 import numpy as np
+from ostatslib import config
 
 from ostatslib.states import State
 from ._get_exploratory_reward import get_exploratory_reward
 from ..action import Action, ActionInfo, ActionResult
 from ..utils import validate_state
 
 _ACTION_NAME = "Is Response Dichotomous Check"
 _VALIDATIONS = [('response_variable_label', operator.truth, None)]
 
-@validate_state(action_name=_ACTION_NAME, validator_fns=_VALIDATIONS)
-def _is_response_dichotomous_check(state: State, data: DataFrame) -> ActionResult[None]:
+
+def _action(state: State, data: DataFrame) -> ActionResult[None]:
     """
     Check if response variable is dichotomous
 
     Args:
         state (State): state
         data (DataFrame): data
 
     Returns:
         ActionResult[None]: action result
     """
+    if not validate_state(state, _VALIDATIONS):
+        return state, config.MIN_REWARD, ActionInfo(action_name=_ACTION_NAME,
+                                                    action_fn=_action,
+                                                    model=None,
+                                                    raised_exception=False)
+
     state_copy: State = state.copy()
     response_var_label: str = state.get("response_variable_label")
     response: Series = data[response_var_label]
-    state.set("is_response_dichotomous", __get_is_dichotomous_feature_value(response))
+    state.set("is_response_dichotomous",
+              __get_is_dichotomous_feature_value(response))
     reward = get_exploratory_reward(state, state_copy)
     return state, reward, ActionInfo(action_name=_ACTION_NAME,
-                                     action_fn=_is_response_dichotomous_check,
+                                     action_fn=_action,
                                      model=None,
                                      raised_exception=False)
 
 
 def __get_is_dichotomous_feature_value(values: Series) -> int:
     return 1 if __is_dichotomous_check(values) else -1
 
@@ -55,17 +63,17 @@
         case "categorical" | "string" | "object" | "mixed-integer":
             return True
         case "integer":
             return bool(__is_within_possible_boolean_range_of_integers(unique_values))
         case "floating" | "decimal" | "mixed-integer-float":
             first, second = unique_values
             return bool(first.is_integer() and second.is_integer() and
-                bool(__is_within_possible_boolean_range_of_integers(unique_values)))
+                        bool(__is_within_possible_boolean_range_of_integers(unique_values)))
         case _:
             return False
 
 
 def __is_within_possible_boolean_range_of_integers(unique_values):
     return np.any((unique_values >= -1) | (unique_values <= 2))
 
 
-is_response_dichotomous_check: Action[None] = _is_response_dichotomous_check
+is_response_dichotomous_check: Action[None] = _action
```

### Comparing `ostatslib-0.5.0/ostatslib/actions/exploratory_actions/is_response_discrete_check.py` & `ostatslib-0.5.1/ostatslib/actions/exploratory_actions/is_response_discrete_check.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,55 @@
 """
 is_response_discrete_check module
 """
 
 import operator
 from pandas import DataFrame, Series
 import numpy as np
+from ostatslib import config
 
 from ostatslib.states import State
 from ._get_exploratory_reward import get_exploratory_reward
 from ..action import Action, ActionInfo, ActionResult
 from ..utils import validate_state
 
 _ACTION_NAME = "Is Response Discrete Check"
 _VALIDATIONS = [('response_variable_label', operator.truth, None)]
 
-@validate_state(action_name=_ACTION_NAME, validator_fns=_VALIDATIONS)
-def _is_response_discrete_check(state: State, data: DataFrame) -> ActionResult[None]:
+
+def _action(state: State, data: DataFrame) -> ActionResult[None]:
     """
     Check if response variable is discrete
 
     Args:
         state (State): state
         data (DataFrame): data
 
     Returns:
         ActionResult[None]: action result
     """
+    if not validate_state(state, _VALIDATIONS):
+        return state, config.MIN_REWARD, ActionInfo(action_name=_ACTION_NAME,
+                                                    action_fn=_action,
+                                                    model=None,
+                                                    raised_exception=False)
+
     state_copy: State = state.copy()
     response_var_label: str = state.get("response_variable_label")
     response: Series = data[response_var_label]
 
     is_discrete: bool = __is_discrete_check(response)
     if is_discrete:
         state.set("is_response_discrete", 1)
     else:
         state.set("is_response_discrete", -1)
 
     reward = get_exploratory_reward(state, state_copy)
     return state, reward, ActionInfo(action_name=_ACTION_NAME,
-                                     action_fn=_is_response_discrete_check,
+                                     action_fn=_action,
                                      model=None,
                                      raised_exception=False)
 
 
 def __is_discrete_check(values: Series) -> bool:
     unique_values = values.unique()
 
@@ -56,8 +63,8 @@
             is_whole = float(value).is_integer()
             if not is_whole:
                 return False
 
     return True
 
 
-is_response_discrete_check: Action[None] = _is_response_discrete_check
+is_response_discrete_check: Action[None] = _action
```

### Comparing `ostatslib-0.5.0/ostatslib/actions/exploratory_actions/is_response_positive_values_only_check.py` & `ostatslib-0.5.1/ostatslib/actions/exploratory_actions/is_response_positive_values_only_check.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,48 +2,54 @@
 """
 is_response_positive_values_only_check module
 """
 
 import operator
 from pandas import DataFrame, Series
 import numpy as np
+from ostatslib import config
 
 from ostatslib.states import State
 from ._get_exploratory_reward import get_exploratory_reward
 from ..action import Action, ActionInfo, ActionResult
 from ..utils import validate_state
 
 _ACTION_NAME = "Is Response Positive Values Only Check"
 _VALIDATIONS = [('response_variable_label', operator.truth, None)]
 
-@validate_state(action_name=_ACTION_NAME, validator_fns=_VALIDATIONS)
-def _is_response_positive_values_only_check(state: State, data: DataFrame) -> ActionResult[None]:
+
+def _action(state: State, data: DataFrame) -> ActionResult[None]:
     """
     Check if response variable values are positive only
 
     Args:
         state (State): state
         data (DataFrame): data
 
     Returns:
         ActionResult[None]: action result
     """
+    if not validate_state(state, _VALIDATIONS):
+        return state, config.MIN_REWARD, ActionInfo(action_name=_ACTION_NAME,
+                                                    action_fn=_action,
+                                                    model=None,
+                                                    raised_exception=False)
     state_copy: State = state.copy()
     response_var_label: str = state.get("response_variable_label")
     response: Series = data[response_var_label]
 
     is_positive_only: bool = __positive_only_check(response)
     if is_positive_only:
         state.set("is_response_positive_values_only", 1)
     else:
         state.set("is_response_positive_values_only", -1)
 
     reward = get_exploratory_reward(state, state_copy)
     return state, reward, ActionInfo(action_name=_ACTION_NAME,
-                                     action_fn=_is_response_positive_values_only_check,
+                                     action_fn=_action,
                                      model=None,
                                      raised_exception=False)
 
 
 def __positive_only_check(values: Series) -> bool:
     unique_values = values.unique()
     is_numeric = np.issubdtype(unique_values.dtype, np.number)
@@ -53,8 +59,8 @@
             unique_values.astype(float, copy=False)
         except Exception:
             return False
 
     return unique_values.min() >= 0
 
 
-is_response_positive_values_only_check: Action[None] = _is_response_positive_values_only_check
+is_response_positive_values_only_check: Action[None] = _action
```

### Comparing `ostatslib-0.5.0/ostatslib/actions/exploratory_actions/is_response_quantitative_check.py` & `ostatslib-0.5.1/ostatslib/actions/exploratory_actions/is_response_quantitative_check.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,57 @@
 """
 is_response_quantitative_check module
 """
 
 import operator
 from pandas import DataFrame, Series
 import numpy as np
+from ostatslib import config
 
 from ostatslib.states import State
 from ._get_exploratory_reward import get_exploratory_reward
 from ..action import Action, ActionInfo, ActionResult
 from ..utils import validate_state
 
 _ACTION_NAME = "Is Response Quantitative Check"
 _VALIDATIONS = [('response_variable_label', operator.truth, None)]
 
-@validate_state(action_name=_ACTION_NAME, validator_fns=_VALIDATIONS)
-def _is_response_quantitative_check(state: State, data: DataFrame) -> ActionResult[None]:
+
+def _action(state: State, data: DataFrame) -> ActionResult[None]:
     """
     Check if response variable is quantitative
 
     Args:
         state (State): state
         data (DataFrame): data
 
     Returns:
         ActionResult[None]: action result
     """
+    if not validate_state(state, _VALIDATIONS):
+        return state, config.MIN_REWARD, ActionInfo(action_name=_ACTION_NAME,
+                                                    action_fn=_action,
+                                                    model=None,
+                                                    raised_exception=False)
     state_copy: State = state.copy()
     response_var_label: str = state.get("response_variable_label")
     response: Series = data[response_var_label]
 
     is_quantitative: bool = __is_quantitative_check(response)
     if is_quantitative:
         state.set("is_response_quantitative", 1)
     else:
         state.set("is_response_quantitative", -1)
 
     reward = get_exploratory_reward(state, state_copy)
     return state, reward, ActionInfo(action_name=_ACTION_NAME,
-                                     action_fn=_is_response_quantitative_check,
+                                     action_fn=_action,
                                      model=None,
                                      raised_exception=False)
 
 
 def __is_quantitative_check(values: Series) -> bool:
     unique_values = values.unique()
     return np.issubdtype(unique_values.dtype, np.number)
 
 
-is_response_quantitative_check: Action[None] = _is_response_quantitative_check
+is_response_quantitative_check: Action[None] = _action
```

### Comparing `ostatslib-0.5.0/ostatslib/actions/exploratory_actions/time_convertible_variable_search.py` & `ostatslib-0.5.1/ostatslib/actions/exploratory_actions/time_convertible_variable_search.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "datetime64", "datetime", "date",
     "period",
     "time",
     "timedelta64", "timedelta",
 ]
 
 
-def _time_convertible_variable_search(state: State, data: DataFrame) -> ActionResult[None]:
+def _action(state: State, data: DataFrame) -> ActionResult[None]:
     """
     Gets log rows count: log(#rows)/c, where c is a compression constant
 
     Args:
         state (State): state
         data (DataFrame): data
 
@@ -39,15 +39,15 @@
         variables_dataframe = data
 
     date_convertible_variable = __date_variable_search(variables_dataframe)
 
     reward: float = __calculate_reward(state, date_convertible_variable)
     __update_state(state, date_convertible_variable)
     return state, reward, ActionInfo(action_name=_ACTION_NAME,
-                                     action_fn=_time_convertible_variable_search,
+                                     action_fn=_action,
                                      model=None,
                                      raised_exception=False)
 
 
 def __date_variable_search(variables_dataframe: DataFrame) -> str | None:
     time_related_variables: list[tuple[str, str]] = []
 
@@ -85,8 +85,8 @@
 
 
 def __update_state(state: State, date_convertible_variable: str | None) -> State:
     state.set("time_convertible_variable", date_convertible_variable)
     return state
 
 
-time_convertible_variable_search: Action[None] = _time_convertible_variable_search
+time_convertible_variable_search: Action[None] = _action
```

### Comparing `ostatslib-0.5.0/ostatslib/actions/regression_models/decision_tree_regression.py` & `ostatslib-0.5.1/ostatslib/actions/regression_models/decision_tree_regression.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,49 +20,54 @@
 _ACTION_NAME = "Decision Tree Regression"
 _VALIDATIONS = [('is_response_quantitative', operator.gt, 0),
                 ('is_response_dichotomous', operator.lt, 0),
                 ('response_variable_label', operator.truth, None),
                 ('decision_tree_regression_score_reward', operator.eq, 0)]
 
 
-@validate_state(action_name=_ACTION_NAME, validator_fns=_VALIDATIONS)
 @reward_cap
 @comprehensible_model
-def _decision_tree_regression(state: State,
-                              data: DataFrame) -> ActionResult[DecisionTreeRegressor]:
+def _action(state: State,
+            data: DataFrame) -> ActionResult[DecisionTreeRegressor]:
     """
     Fits data to a decision tree regressor
 
     Args:
         state (State): current environment state
         data (DataFrame): data under analysis
 
     Returns:
         ActionResult[DecisionTreeRegressor]: action result
     """
+    if not validate_state(state, _VALIDATIONS):
+        return state, config.MIN_REWARD, ActionInfo(action_name=_ACTION_NAME,
+                                                    action_fn=_action,
+                                                    model=None,
+                                                    raised_exception=False)
+
     y_values, x_values = split_response_from_explanatory_variables(state, data)
     regressor: DecisionTreeRegressor = DecisionTreeRegressor()
     param_grid = {'criterion': ['squared_error', 'friedman_mse', 'absolute_error'],
                   'max_features': ['sqrt', 'log2', None]}
 
     try:
         regressor, score = model_selection(regressor,
                                            param_grid,
                                            x_values,
                                            y_values)
     except ValueError:
         state.set('decision_tree_regression_score_reward', config.MIN_REWARD)
         return state, config.MIN_REWARD, ActionInfo(action_name=_ACTION_NAME,
-                                                    action_fn=_decision_tree_regression,
+                                                    action_fn=_action,
                                                     model=None,
                                                     raised_exception=True)
 
     update_state_score(state, score)
     reward = calculate_score_reward(score)
     state.set('decision_tree_regression_score_reward', reward)
     return state, reward, ActionInfo(action_name=_ACTION_NAME,
-                                     action_fn=_decision_tree_regression,
+                                     action_fn=_action,
                                      model=regressor,
                                      raised_exception=False)
 
 
-decision_tree_regression: Action[DecisionTreeRegressor] = _decision_tree_regression
+decision_tree_regression: Action[DecisionTreeRegressor] = _action
```

### Comparing `ostatslib-0.5.0/ostatslib/actions/regression_models/linear_regression.py` & `ostatslib-0.5.1/ostatslib/actions/regression_models/linear_regression.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,43 +27,48 @@
 
 _ACTION_NAME = "Linear Regression"
 _VALIDATIONS = [('response_variable_label', operator.truth, None),
                 ('is_response_quantitative', operator.gt, 0),
                 ('linear_regression_score_reward', operator.eq, 0)]
 
 
-@validate_state(action_name=_ACTION_NAME, validator_fns=_VALIDATIONS)
 @reward_cap
 @interpretable_model
-def _linear_regression(state: State, data: DataFrame) -> ActionResult[RegressionResults]:
+def _action(state: State, data: DataFrame) -> ActionResult[RegressionResults]:
     """
     Fits data to a linear regression model.
 
     Args:
         state (State): current environment state
         data (DataFrame): data under analysis
 
     Returns:
         ActionResult[RegressionResults]: action result
     """
+    if not validate_state(state, _VALIDATIONS):
+        return state, config.MIN_REWARD, ActionInfo(action_name=_ACTION_NAME,
+                                                    action_fn=_action,
+                                                    model=None,
+                                                    raised_exception=False)
+
     response_var, explanatory_vars = split_response_from_explanatory_variables(
         state, data)
     try:
         regression: RegressionResults = OLS(
             response_var, add_constant(explanatory_vars)).fit()
     except ValueError:
         return state, config.MIN_REWARD, ActionInfo(action_name=_ACTION_NAME,
-                                                    action_fn=_linear_regression,
+                                                    action_fn=_action,
                                                     model=None,
                                                     raised_exception=True)
 
     reward = __calculate_reward(state, regression)
     update_state_score(state, regression.rsquared)
     return state, reward, ActionInfo(action_name=_ACTION_NAME,
-                                     action_fn=_linear_regression,
+                                     action_fn=_action,
                                      model=regression,
                                      raised_exception=False)
 
 
 def __calculate_reward(state: State, regression: RegressionResults) -> float:
     explanatory_vars: np.ndarray = regression.model.exog
     residuals: np.ndarray = regression.resid.values
@@ -152,8 +157,8 @@
         state.set("is_linear_model_regression_recursive_residuals_mean_zero", 0.5)
         return 0.05
 
     state.set("is_linear_model_regression_recursive_residuals_mean_zero", 1)
     return 0
 
 
-linear_regression: Action[RegressionResults] = _linear_regression
+linear_regression: Action[RegressionResults] = _action
```

### Comparing `ostatslib-0.5.0/ostatslib/actions/regression_models/linear_support_vector_regression.py` & `ostatslib-0.5.1/ostatslib/actions/regression_models/random_forest_regression.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,69 +1,75 @@
 """
-Linear Support Vector Regression module
+Random Forest Regression module
 """
 
 import operator
 from pandas import DataFrame
-from sklearn.svm import LinearSVR
-from ostatslib import config
+from sklearn.ensemble import RandomForestRegressor
 
+from ostatslib import config
 from ostatslib.states import State
 from ..action import Action, ActionInfo, ActionResult
 from ..utils import (calculate_score_reward,
                      reward_cap,
                      opaque_model,
                      split_response_from_explanatory_variables,
                      update_state_score,
                      validate_state,
                      model_selection)
 
-_ACTION_NAME = "Linear Support Vector Regression"
+_ACTION_NAME = "Random Forest Regression"
 _VALIDATIONS = [('is_response_quantitative', operator.gt, 0),
+                ('is_response_dichotomous', operator.lt, 0),
                 ('response_variable_label', operator.truth, None),
-                ('log_rows_count', operator.gt, 0),
-                ('log_rows_count', operator.lt, 0.81),
-                ('linear_support_vector_regression_score_reward', operator.eq, 0)]
+                ('random_forest_regression_score_reward', operator.eq, 0),
+                ('response_unique_values_ratio', operator.gt, 0.5)]
 
 
-@validate_state(action_name=_ACTION_NAME, validator_fns=_VALIDATIONS)
 @reward_cap
 @opaque_model
-def _linear_support_vector_regression(state: State, data: DataFrame) -> ActionResult[LinearSVR]:
+def _action(state: State,
+            data: DataFrame) -> ActionResult[RandomForestRegressor]:
     """
-    Fits data to a LinearSVR model
+    Fits data to a random forest regressor
 
     Args:
         state (State): current environment state
         data (DataFrame): data under analysis
 
     Returns:
-        ActionResult[LinearSVR]: action result
+        ActionResult[RandomForestRegressor]: action result
     """
+    if not validate_state(state, _VALIDATIONS):
+        return state, config.MIN_REWARD, ActionInfo(action_name=_ACTION_NAME,
+                                                    action_fn=_action,
+                                                    model=None,
+                                                    raised_exception=False)
+
     y_values, x_values = split_response_from_explanatory_variables(state, data)
-    regressor: LinearSVR = LinearSVR()
-    param_grid = {'C': [1, 10, 100],
-                  'loss': ['epsilon_insensitive', 'squared_epsilon_insensitive']}
+    regressor: RandomForestRegressor = RandomForestRegressor()
+    param_grid = {'criterion': ['squared_error', 'friedman_mse'],
+                  'max_features': ['sqrt', 'log2'],
+                  'max_depth': [x_values.shape[1], 20]}
 
     try:
         regressor, score = model_selection(regressor,
                                            param_grid,
                                            x_values,
                                            y_values)
     except ValueError:
-        state.set('linear_support_vector_regression_score_reward',
-                  config.MIN_REWARD)
+        state.set('random_forest_regression_score_reward', config.MIN_REWARD)
         return state, config.MIN_REWARD, ActionInfo(action_name=_ACTION_NAME,
-                                                    action_fn=_linear_support_vector_regression,
+                                                    action_fn=_action,
                                                     model=None,
                                                     raised_exception=True)
 
     update_state_score(state, score)
     reward = calculate_score_reward(score)
-    state.set('linear_support_vector_regression_score_reward', reward)
+    state.set('random_forest_regression_score_reward', reward)
     return state, reward, ActionInfo(action_name=_ACTION_NAME,
-                                     action_fn=_linear_support_vector_regression,
+                                     action_fn=_action,
                                      model=regressor,
                                      raised_exception=False)
 
 
-linear_support_vector_regression: Action[LinearSVR] = _linear_support_vector_regression
+random_forest_regression: Action[RandomForestRegressor] = _action
```

### Comparing `ostatslib-0.5.0/ostatslib/actions/regression_models/poisson_regression.py` & `ostatslib-0.5.1/ostatslib/actions/regression_models/poisson_regression.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,28 +22,33 @@
 _VALIDATIONS = [('response_variable_label', operator.truth, None),
                 ('is_response_positive_values_only', operator.gt, 0),
                 ('is_response_discrete', operator.gt, 0),
                 ('log_rows_count', operator.lt, 0.81),
                 ('poisson_regression_score_reward', operator.eq, 0)]
 
 
-@validate_state(action_name=_ACTION_NAME, validator_fns=_VALIDATIONS)
 @reward_cap
 @interpretable_model
-def _poisson_regression(state: State, data: DataFrame) -> ActionResult[GLMResults]:
+def _action(state: State, data: DataFrame) -> ActionResult[GLMResults]:
     """
     Fits data to a poisson regression model.
 
     Args:
         state (State): current environment state
         data (DataFrame): data under analysis
 
     Returns:
         ActionResult[GLMResults]: action result
     """
+    if not validate_state(state, _VALIDATIONS):
+        return state, config.MIN_REWARD, ActionInfo(action_name=_ACTION_NAME,
+                                                    action_fn=_action,
+                                                    model=None,
+                                                    raised_exception=False)
+
     response_var, explanatory_vars = split_response_from_explanatory_variables(state,
                                                                                data)
     try:
         poisson_family = families.Poisson()
         regression: GLMResults = GLM(response_var,
                                      explanatory_vars,
                                      poisson_family).fit()
@@ -57,20 +62,20 @@
 
     state.set('does_poisson_regression_raises_perfect_separation_error', -1)
     score = regression.pseudo_rsquared()
     reward = calculate_score_reward(score)
     state = update_state_score(state, score)
     state.set('poisson_regression_score_reward', reward)
     return state, reward, ActionInfo(action_name=_ACTION_NAME,
-                                     action_fn=_poisson_regression,
+                                     action_fn=_action,
                                      model=regression,
                                      raised_exception=False)
 
 
 def __raised_exception_action_result(state):
     return state, config.MIN_REWARD, ActionInfo(action_name=_ACTION_NAME,
-                                                action_fn=_poisson_regression,
+                                                action_fn=_action,
                                                 model=None,
                                                 raised_exception=True)
 
 
-poisson_regression: Action[GLMResults] = _poisson_regression
+poisson_regression: Action[GLMResults] = _action
```

### Comparing `ostatslib-0.5.0/ostatslib/actions/regression_models/random_forest_regression.py` & `ostatslib-0.5.1/ostatslib/actions/regression_models/linear_support_vector_regression.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,70 +1,74 @@
 """
-Random Forest Regression module
+Linear Support Vector Regression module
 """
 
 import operator
 from pandas import DataFrame
-from sklearn.ensemble import RandomForestRegressor
-
+from sklearn.svm import LinearSVR
 from ostatslib import config
+
 from ostatslib.states import State
 from ..action import Action, ActionInfo, ActionResult
 from ..utils import (calculate_score_reward,
                      reward_cap,
                      opaque_model,
                      split_response_from_explanatory_variables,
                      update_state_score,
                      validate_state,
                      model_selection)
 
-_ACTION_NAME = "Random Forest Regression"
+_ACTION_NAME = "Linear Support Vector Regression"
 _VALIDATIONS = [('is_response_quantitative', operator.gt, 0),
-                ('is_response_dichotomous', operator.lt, 0),
                 ('response_variable_label', operator.truth, None),
-                ('random_forest_regression_score_reward', operator.eq, 0),
-                ('response_unique_values_ratio', operator.gt, 0.5)]
+                ('log_rows_count', operator.gt, 0),
+                ('log_rows_count', operator.lt, 0.81),
+                ('linear_support_vector_regression_score_reward', operator.eq, 0)]
 
 
-@validate_state(action_name=_ACTION_NAME, validator_fns=_VALIDATIONS)
 @reward_cap
 @opaque_model
-def _random_forest_regression(state: State,
-                              data: DataFrame) -> ActionResult[RandomForestRegressor]:
+def _action(state: State, data: DataFrame) -> ActionResult[LinearSVR]:
     """
-    Fits data to a random forest regressor
+    Fits data to a LinearSVR model
 
     Args:
         state (State): current environment state
         data (DataFrame): data under analysis
 
     Returns:
-        ActionResult[RandomForestRegressor]: action result
+        ActionResult[LinearSVR]: action result
     """
+    if not validate_state(state, _VALIDATIONS):
+        return state, config.MIN_REWARD, ActionInfo(action_name=_ACTION_NAME,
+                                                    action_fn=_action,
+                                                    model=None,
+                                                    raised_exception=False)
+
     y_values, x_values = split_response_from_explanatory_variables(state, data)
-    regressor: RandomForestRegressor = RandomForestRegressor()
-    param_grid = {'criterion': ['squared_error', 'friedman_mse'],
-                  'max_features': ['sqrt', 'log2'],
-                  'max_depth': [x_values.shape[1], 20]}
+    regressor: LinearSVR = LinearSVR()
+    param_grid = {'C': [1, 10, 100],
+                  'loss': ['epsilon_insensitive', 'squared_epsilon_insensitive']}
 
     try:
         regressor, score = model_selection(regressor,
                                            param_grid,
                                            x_values,
                                            y_values)
     except ValueError:
-        state.set('random_forest_regression_score_reward', config.MIN_REWARD)
+        state.set('linear_support_vector_regression_score_reward',
+                  config.MIN_REWARD)
         return state, config.MIN_REWARD, ActionInfo(action_name=_ACTION_NAME,
-                                                    action_fn=_random_forest_regression,
+                                                    action_fn=_action,
                                                     model=None,
                                                     raised_exception=True)
 
     update_state_score(state, score)
     reward = calculate_score_reward(score)
-    state.set('random_forest_regression_score_reward', reward)
+    state.set('linear_support_vector_regression_score_reward', reward)
     return state, reward, ActionInfo(action_name=_ACTION_NAME,
-                                     action_fn=_random_forest_regression,
+                                     action_fn=_action,
                                      model=regressor,
                                      raised_exception=False)
 
 
-random_forest_regression: Action[RandomForestRegressor] = _random_forest_regression
+linear_support_vector_regression: Action[LinearSVR] = _action
```

### Comparing `ostatslib-0.5.0/ostatslib/actions/regression_models/time_series_auto_arima.py` & `ostatslib-0.5.1/ostatslib/actions/regression_models/time_series_auto_arima.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,32 +23,30 @@
 
 _ACTION_NAME = "Time Series - SARIMAX"
 _VALIDATIONS = [('response_variable_label', operator.truth, None),
                 ('is_response_quantitative', operator.gt, 0),
                 ('time_series_auto_arima_score_reward', operator.eq, 0)]
 
 
-@validate_state(action_name=_ACTION_NAME, validator_fns=_VALIDATIONS)
 @reward_cap
 @interpretable_model
-def _time_series_auto_arima(state: State,
-                            data: DataFrame) -> ActionResult[SARIMAXResults]:
+def _action(state: State, data: DataFrame) -> ActionResult[SARIMAXResults]:
     """
     Fits data to an ARIMA model
 
     Args:
         state (State): current environment state
         data (DataFrame): data under analysis
 
     Returns:
         ActionResult[SARIMAXResults]: action result
     """
     if not __is_valid_state(state):
         return state, config.MIN_REWARD, ActionInfo(action_name=_ACTION_NAME,
-                                                    action_fn=_time_series_auto_arima,
+                                                    action_fn=_action,
                                                     model=None,
                                                     raised_exception=False)
 
     y_data, x_data = __build_time_index_dataframes_for_y_and_x(state, data)
     data_length = len(y_data)
     training_split_index = int(data_length * TRAINING_FRACTION)
     y_training, y_testing = (y_data.iloc[:training_split_index],
@@ -65,15 +63,15 @@
     forecast: Series = model.forecast(data_length - training_split_index,
                                       exog=x_testing)
     score: float = 1 - \
         __calculate_mean_abs_percentage_error(forecast, y_testing)
 
     reward: float = __calculate_reward(state, model, score)
     return state, reward, ActionInfo(action_name=_ACTION_NAME,
-                                     action_fn=_time_series_auto_arima,
+                                     action_fn=_action,
                                      model=model,
                                      raised_exception=False)
 
 
 def __is_valid_state(state: State) -> bool:
     if bool(state.get("time_convertible_variable")) and \
         state.get("is_response_quantitative") > 0 and \
@@ -141,8 +139,8 @@
         x_data = x_data.set_index(state.get("time_convertible_variable"))
 
     y_data = DataFrame({y_values.name: y_values.values}, index=time)
 
     return y_data, x_data
 
 
-time_series_auto_arima: Action[SARIMAXResults] = _time_series_auto_arima
+time_series_auto_arima: Action[SARIMAXResults] = _action
```

### Comparing `ostatslib-0.5.0/ostatslib/actions/utils/explainability_rewards.py` & `ostatslib-0.5.1/ostatslib/actions/utils/explainability_rewards.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,16 +21,15 @@
 
     Args:
         action_function (Action[TModel]): action
 
     Returns:
         Action[TModel]: action
     """
-    wraps(action_function)
-
+    @wraps(action_function)
     def function_wrapper(state: State, data: DataFrame):
         state, reward, info = action_function(state, data)
         reward += OPAQUE_PENALTY
         return state, reward, info
 
     return function_wrapper
 
@@ -42,16 +41,15 @@
 
     Args:
         action_function (Action[TModel]): action
 
     Returns:
         Action[TModel]: action
     """
-    wraps(action_function)
-
+    @wraps(action_function)
     def function_wrapper(state: State, data: DataFrame):
         state, reward, info = action_function(state, data)
         reward += INTERPRETABLE_REWARD
         return state, reward, info
 
     return function_wrapper
 
@@ -63,15 +61,14 @@
 
     Args:
         action_function (Action[TModel]): action
 
     Returns:
         Action[TModel]: action
     """
-    wraps(action_function)
-
+    @wraps(action_function)
     def function_wrapper(state: State, data: DataFrame):
         state, reward, info = action_function(state, data)
         reward += COMPREHENSIBLE_REWARD
         return state, reward, info
 
     return function_wrapper
```

### Comparing `ostatslib-0.5.0/ostatslib/actions/utils/model_selection.py` & `ostatslib-0.5.1/ostatslib/actions/utils/model_selection.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,9 +31,8 @@
     search = HalvingGridSearchCV(classifier,
                                  param_grid,
                                  cv=5,
                                  factor=2,
                                  n_jobs=None).fit(X, y)
     fitted_model: TModel = search.best_estimator_
     score = search.best_score_
-    print(fitted_model, score)
     return fitted_model, score
```

### Comparing `ostatslib-0.5.0/ostatslib/actions/utils/reward_cap.py` & `ostatslib-0.5.1/ostatslib/actions/utils/reward_cap.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
     Args:
         action_function (Action[TModel]): action
 
     Returns:
         Action[TModel]: action
     """
-    wraps(action_function)
-
+    @wraps(action_function)
     def function_wrapper(state: State, data: DataFrame):
         state, reward, info = action_function(state, data)
         reward = min(max(config.MIN_REWARD, reward), config.MAX_REWARD)
         return state, reward, info
 
     return function_wrapper
```

### Comparing `ostatslib-0.5.0/ostatslib/actions/utils/split_response_from_explanatory_variables.py` & `ostatslib-0.5.1/ostatslib/actions/utils/split_response_from_explanatory_variables.py`

 * *Files identical despite different names*

### Comparing `ostatslib-0.5.0/ostatslib/agents/agent.py` & `ostatslib-0.5.1/ostatslib/agents/agent.py`

 * *Files identical despite different names*

### Comparing `ostatslib-0.5.0/ostatslib/agents/analysis_result.py` & `ostatslib-0.5.1/ostatslib/agents/analysis_result.py`

 * *Files identical despite different names*

### Comparing `ostatslib-0.5.0/ostatslib/agents/ppo_agent.py` & `ostatslib-0.5.1/ostatslib/agents/ppo_agent.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,52 +2,71 @@
 PPO Agent module
 """
 
 import torch as th
 from numpy import ndarray
 from stable_baselines3 import PPO
 from stable_baselines3.common.env_util import make_vec_env
+from stable_baselines3.common.vec_env import SubprocVecEnv
 from stable_baselines3.common.callbacks import CheckpointCallback
 from stable_baselines3.common.logger import configure
 
 from ostatslib.agents.agent import Agent
 from ostatslib.environments import GymEnvironment
 
 POLICY = "MultiInputPolicy"
 POLICY_KWARGS = {
     'activation_fn': th.nn.ReLU,
     'share_features_extractor': False
 }
 
 TRAINING_LOGS_PATH = "./.logs/"
 
+
 class PPOAgent(Agent):
     """
     Agent built on PPO algorithm model
     """
 
-    def __init__(self, path: str | None = None, training_envs_count: int = 10) -> None:
+    def __init__(self,
+                 path: str | None = None,
+                 training_envs_count: int = 3,
+                 environment_kwargs: dict | None = None) -> None:
+        self.__environment_kwargs = environment_kwargs
         self.__model = self.__init__model(path, training_envs_count)
 
-    def train(self, steps: int = 100000, save_freq: int = 1) -> None:
+    def train(self, steps: int = 1000000, save_freq: int = 100000) -> None:
         n_envs = self.__model.n_envs if self.__model.n_envs is not None else 1
         save_freq = max(save_freq // n_envs, 1)
         checkpoint_callback = CheckpointCallback(save_freq=save_freq,
                                                  save_path=TRAINING_LOGS_PATH,
                                                  save_replay_buffer=True)
-        logger = configure(TRAINING_LOGS_PATH, ["stdout", "csv", "tensorboard"])
+        logger = configure(TRAINING_LOGS_PATH,
+                           ["stdout", "csv", "tensorboard"])
         self.__model.set_logger(logger)
         self.__model.learn(total_timesteps=steps, callback=checkpoint_callback)
 
     def save(self, path: str) -> None:
         self.__model.save(path)
 
     def _predict(self, observation: dict) -> ndarray:
         action, _ = self.__model.predict(observation, deterministic=True)
         return action[0]
 
     def __init__model(self, path: str | None, training_envs_count: int) -> PPO:
+        environments = make_vec_env(GymEnvironment,
+                                    training_envs_count,
+                                    env_kwargs=self.__environment_kwargs,
+                                    vec_env_cls=SubprocVecEnv)
         if path is None:
-            environments = make_vec_env(GymEnvironment, training_envs_count)
-            return PPO(POLICY, environments, verbose=1, n_steps=6144, policy_kwargs=POLICY_KWARGS)
-
-        return PPO.load(path)
+            return PPO(POLICY,
+                       environments,
+                       verbose=1,
+                       n_steps=2048,
+                       policy_kwargs=POLICY_KWARGS)
+
+        return PPO.load(path,
+                        environments,
+                        custom_objects={
+                            'observation_space': environments.observation_space,
+                            'action_space': environments.action_space
+                        })
```

### Comparing `ostatslib-0.5.0/ostatslib/environments/gym_environment.py` & `ostatslib-0.5.1/ostatslib/environments/gym_environment.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,54 @@
 """
 GymEnvironment module
 """
 
-from typing import Any
+from typing import Any, Callable
+from random import choice
 from numpy import ndarray
 from pandas import DataFrame
 from gymnasium import Env
 from gymnasium.spaces import Dict
 from ostatslib import config
 from ostatslib.actions import ActionsSpace
 from ostatslib.actions.action import ActionInfo
 from ostatslib.actions.actions_space import _invalid_action_step
+from ostatslib.environments.data_generators import (datacooker_generator,
+                                                    pmlb_generator,
+                                                    sklearn_generator)
 from ostatslib.states import State
-from .utils import generate_training_dataset
 
 ObsType = Dict
+DataGeneratorFn = Callable[[], tuple[DataFrame, State]]
+
+DEFAULT_DATA_GENERATORS = [
+    datacooker_generator,
+    pmlb_generator,
+    sklearn_generator]
 
 
 class GymEnvironment(Env):
     """
     Statistical environment implemented as Gymnasium environment
     """
 
     __state: State
     __data: DataFrame
+    __data_generators: list[DataGeneratorFn]
 
-    def __init__(self) -> None:
-        self.__init_state_and_data()
+    def __init__(self, data_generators: list[DataGeneratorFn] | None = None) -> None:
         self.observation_space = State().as_gymnasium_space
         self.action_space: ActionsSpace = ActionsSpace()
         self.reward_range = config.REWARD_RANGE
+        if data_generators is None:
+            self.__data_generators = DEFAULT_DATA_GENERATORS
+        else:
+            self.__data_generators = data_generators
         self.__steps_taken = 0
+        self.__init_state_and_data()
 
     def render(self) -> None:
         print("Render has no effect yet")
 
     def reset(self,
               *,
               seed: int | None = None,
@@ -78,8 +92,9 @@
         self.__state = state
 
     def __is_done(self, state: State, reward: float) -> bool:
         return (state.get("score") > config.MIN_ACCEPTED_SCORE and reward > config.MAX_REWARD/2)\
             or self.__steps_taken >= config.MAX_STEPS
 
     def __init_state_and_data(self):
-        self.__data, self.__state = generate_training_dataset()
+        generator = choice(self.__data_generators)
+        self.__data, self.__state = generator()
```

### Comparing `ostatslib-0.5.0/ostatslib/environments/utils/_generate_from_datacooker.py` & `ostatslib-0.5.1/ostatslib/environments/data_generators/datacooker_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from scipy.stats import norm
 from datacooker.recipes import LogitRecipe, PoissonRecipe, Recipe
 from datacooker.variables import ContinousVariable
 
 from ostatslib.states import State
 
 
-def generate_from_datacooker() -> tuple[DataFrame, State]:
+def datacooker_generator() -> tuple[DataFrame, State]:
     """
     Generate Datacooker dataset
 
     Returns:
         tuple[DataFrame, State]: dataset and initial state
     """
     dataset_type = choice([LogitRecipe, PoissonRecipe, Recipe])
```

### Comparing `ostatslib-0.5.0/ostatslib/environments/utils/_generate_from_pmlb.py` & `ostatslib-0.5.1/ostatslib/environments/data_generators/pmlb_generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from ostatslib.states import State
 
 PMLB_CACHE_FOLDER = './.pmlb_cache'
 SKIP_DATASETS = ['poker', '1595_poker',
                  '1191_BNG_pbc', '1196_BNG_pharynx', 'kddcup']
 
 
-def generate_from_pmlb() -> tuple[DataFrame, State]:
+def pmlb_generator() -> tuple[DataFrame, State]:
     """
     Randomly selects a dataset from Penn Machine Learning Benchmarks
 
     Returns:
         tuple[DataFrame, State]: dataset and initial state
     """
     pmlb_gen_fn = choice([
```

### Comparing `ostatslib-0.5.0/ostatslib/environments/utils/_generate_from_sklearn.py` & `ostatslib-0.5.1/ostatslib/environments/data_generators/sklearn_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from pandas import DataFrame
 import sklearn.datasets as sklearn_dts
 import numpy as np
 
 from ostatslib.states import State
 
 
-def generate_from_sklearn() -> tuple[DataFrame, State]:
+def sklearn_generator() -> tuple[DataFrame, State]:
     """
     Generates a dataset from sklearn's toy datasets or generated
     https://scikit-learn.org/stable/datasets.html
 
     Returns:
         tuple[DataFrame, State]: dataset and initial state
     """
```

### Comparing `ostatslib-0.5.0/ostatslib/states/analysis_features_set.py` & `ostatslib-0.5.1/ostatslib/states/analysis_features_set.py`

 * *Files identical despite different names*

### Comparing `ostatslib-0.5.0/ostatslib/states/data_features_set.py` & `ostatslib-0.5.1/ostatslib/states/data_features_set.py`

 * *Files identical despite different names*

### Comparing `ostatslib-0.5.0/ostatslib/states/features_set.py` & `ostatslib-0.5.1/ostatslib/states/features_set.py`

 * *Files identical despite different names*

### Comparing `ostatslib-0.5.0/ostatslib/states/models_features_set.py` & `ostatslib-0.5.1/ostatslib/states/models_features_set.py`

 * *Files identical despite different names*

### Comparing `ostatslib-0.5.0/ostatslib/states/state.py` & `ostatslib-0.5.1/ostatslib/states/state.py`

 * *Files identical despite different names*

### Comparing `ostatslib-0.5.0/ostatslib/states/state_iterator.py` & `ostatslib-0.5.1/ostatslib/states/state_iterator.py`

 * *Files identical despite different names*

### Comparing `ostatslib-0.5.0/ostatslib/states/utils/init_features_set.py` & `ostatslib-0.5.1/ostatslib/states/utils/init_features_set.py`

 * *Files identical despite different names*

### Comparing `ostatslib-0.5.0/pyproject.toml` & `ostatslib-0.5.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "ostatslib"
-version = "0.5.0"
+version = "0.5.1"
 description = "Open Statistical Analysis Agent Library"
 authors = ["Guilherme <g.lisboa.oliveira@outlook.com>"]
 repository = "https://github.com/OStatsAA/ostatslib"
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.10,<3.12"
+python = ">=3.11,<3.12"
 numpy = "^1.23.4"
 pandas = "^2.0.1"
 statsmodels = ">=0.13.2,<0.15.0"
 scipy = "^1.9.3"
 scikit-learn = "^1.1.2"
 pmdarima = "^2.0.2"
 tabulate = "^0.9.0"
```

### Comparing `ostatslib-0.5.0/PKG-INFO` & `ostatslib-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: ostatslib
-Version: 0.5.0
+Version: 0.5.1
 Summary: Open Statistical Analysis Agent Library
 Home-page: https://github.com/OStatsAA/ostatslib
 License: MIT
 Author: Guilherme
 Author-email: g.lisboa.oliveira@outlook.com
-Requires-Python: >=3.10,<3.12
+Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: datacooker (>=0.4.1,<0.5.0)
 Requires-Dist: kneed (>=0.8.3,<0.9.0)
 Requires-Dist: numpy (>=1.23.4,<2.0.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: pmdarima (>=2.0.2,<3.0.0)
 Requires-Dist: pmlb (>=1.0.1.post3,<2.0.0)
```

