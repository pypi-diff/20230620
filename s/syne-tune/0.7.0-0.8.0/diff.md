# Comparing `tmp/syne_tune-0.7.0.tar.gz` & `tmp/syne_tune-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syne_tune-0.7.0.tar", last modified: Thu May 25 13:19:49 2023, max compression
+gzip compressed data, was "syne_tune-0.8.0.tar", last modified: Tue Jun 20 15:04:45 2023, max compression
```

## Comparing `syne_tune-0.7.0.tar` & `syne_tune-0.8.0.tar`

### file list

```diff
@@ -1,303 +1,309 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.343604 syne_tune-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-05-25 13:19:34.000000 syne_tune-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-25 13:19:34.000000 syne_tune-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-25 13:19:34.000000 syne_tune-0.7.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    19123 2023-05-25 13:19:49.343604 syne_tune-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18283 2023-05-25 13:19:34.000000 syne_tune-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-25 13:19:49.343604 syne_tune-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-05-25 13:19:34.000000 syne_tune-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.319603 syne_tune-0.7.0/syne_tune/
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.319603 syne_tune-0.7.0/syne_tune/backend/
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15659 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/backend/local_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.319603 syne_tune-0.7.0/syne_tune/backend/python_backend/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/backend/python_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/backend/python_backend/python_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/backend/python_backend/python_entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.319603 syne_tune-0.7.0/syne_tune/backend/sagemaker_backend/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/backend/sagemaker_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/backend/sagemaker_backend/custom_framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/backend/sagemaker_backend/instance-types-cost.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/backend/sagemaker_backend/instance_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    24042 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/backend/sagemaker_backend/sagemaker_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    21131 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/backend/sagemaker_backend/sagemaker_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.319603 syne_tune-0.7.0/syne_tune/backend/simulator_backend/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/backend/simulator_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/backend/simulator_backend/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    22590 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/backend/simulator_backend/simulator_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/backend/simulator_backend/simulator_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/backend/simulator_backend/time_keeper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/backend/time_keeper.py
--rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/backend/trial_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/backend/trial_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.323603 syne_tune-0.7.0/syne_tune/blackbox_repository/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/blackbox_repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/blackbox_repository/blackbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/blackbox_repository/blackbox_offline.py
--rw-r--r--   0 runner    (1001) docker     (123)    22192 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/blackbox_repository/blackbox_surrogate.py
--rw-r--r--   0 runner    (1001) docker     (123)    17442 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/blackbox_repository/blackbox_tabular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.323603 syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/blackbox_recipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/recipes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.323603 syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/scripts/fcnet_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/scripts/icml2020_import.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.323603 syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10223 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/lcbench.py
--rw-r--r--   0 runner    (1001) docker     (123)    10468 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/scripts/nasbench201_import.py
--rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/scripts/pd1_import.py
--rw-r--r--   0 runner    (1001) docker     (123)    17778 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/scripts/yahpo_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/blackbox_repository/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/blackbox_repository/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)    18952 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/blackbox_repository/simulated_tabular_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/blackbox_repository/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.323603 syne_tune-0.7.0/syne_tune/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22237 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/callbacks/hyperband_remove_checkpoints_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/callbacks/hyperband_remove_checkpoints_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/callbacks/remove_checkpoints_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/callbacks/tensorboard_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)    43893 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/config_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.323603 syne_tune-0.7.0/syne_tune/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/experiments/aggregate_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    17083 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/experiments/experiment_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    14601 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/experiments/plot_per_trial.py
--rw-r--r--   0 runner    (1001) docker     (123)    29593 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/experiments/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    17712 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/experiments/results_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/num_gpu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.323603 syne_tune-0.7.0/syne_tune/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37757 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/baselines.py
--rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.327603 syne_tune-0.7.0/syne_tune/optimizer/schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17051 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/fifo.py
--rw-r--r--   0 runner    (1001) docker     (123)    59571 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/hyperband.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/hyperband_checkpoint_removal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/hyperband_cost_promotion.py
--rw-r--r--   0 runner    (1001) docker     (123)    12528 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/hyperband_pasha.py
--rw-r--r--   0 runner    (1001) docker     (123)    11942 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/hyperband_promotion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/hyperband_rush.py
--rw-r--r--   0 runner    (1001) docker     (123)    15115 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/hyperband_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/median_stopping_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/multi_fidelity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.327603 syne_tune-0.7.0/syne_tune/optimizer/schedulers/multiobjective/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/multiobjective/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7697 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/multiobjective/linear_scalarizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11212 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/multiobjective/moasha.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/multiobjective/multi_objective_regularized_evolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/multiobjective/multiobjective_priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/multiobjective/non_dominated_priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/multiobjective/nsga2_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/multiobjective/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.327603 syne_tune-0.7.0/syne_tune/optimizer/schedulers/neuralbands/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/neuralbands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/neuralbands/networks.py
--rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/neuralbands/neuralband.py
--rw-r--r--   0 runner    (1001) docker     (123)    22189 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/neuralbands/neuralband_supplement.py
--rw-r--r--   0 runner    (1001) docker     (123)    15111 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/pbt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/random_seeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     8676 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/ray_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/remove_checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/scheduler_searcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.331603 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.331603 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.331603 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/config_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)    13227 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/tuning_job_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.331603 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/custom_op.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    40693 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon.py
--rw-r--r--   0 runner    (1001) docker     (123)    14767 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon_blocks_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11243 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gpr_mcmc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.331603 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13474 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/gp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)    15300 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/posterior_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    19410 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.331603 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/gpind_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11496 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)    10699 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/posterior_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.335604 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10740 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/cross_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    13361 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/exponential_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/fabolas.py
--rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/freeze_thaw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/product_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/range_kernel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.335604 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18991 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/freeze_thaw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/gpiss_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    42009 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/issm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/model_params.py
--rw-r--r--   0 runner    (1001) docker     (123)    27009 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/posterior_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/mean.py
--rw-r--r--   0 runner    (1001) docker     (123)    13024 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/optimization_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16368 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    13238 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/slice.py
--rw-r--r--   0 runner    (1001) docker     (123)    10095 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/target_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/warping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.335604 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.335604 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/cost_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/linear_cost_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14332 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/sklearn_cost_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost_fifo_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6919 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_mcmc_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    18163 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    17447 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gpiss_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/kernel_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    15047 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21176 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_skipopt.py
--rw-r--r--   0 runner    (1001) docker     (123)    16104 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/sklearn_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/sklearn_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_multi_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_single_fidelity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.335604 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.339604 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12949 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/base_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    16077 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)    13322 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.339604 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/comparison_gpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/debug_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/test_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.339604 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bore/
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10866 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bore/bore.py
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bore/de.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bore/gp_classififer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bore/mlp_classififer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bore/multi_fidelity_bore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.339604 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/botorch/
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/botorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11845 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/botorch/botorch_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bracket_distribution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.339604 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/constrained/
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/constrained/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/constrained/constrained_gp_fifo_searcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.339604 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/cost_aware/
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/cost_aware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_fifo_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_multifidelity_searcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.339604 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/dyhpo/
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/dyhpo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18542 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/dyhpo/dyhpo_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    10575 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/dyhpo/hyperband_dyhpo.py
--rw-r--r--   0 runner    (1001) docker     (123)    15779 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/gp_fifo_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    13439 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/gp_multifidelity_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    42012 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/gp_searcher_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/gp_searcher_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.339604 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/hypertune/
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/hypertune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_bracket_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_searcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.339604 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/kde/
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/kde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17166 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/kde/kde_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/kde/multi_fidelity_kde_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    34597 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/model_based_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    15488 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/random_grid_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/regularized_evolution.py
--rw-r--r--   0 runner    (1001) docker     (123)    14507 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    14811 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/searcher_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/searcher_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/searcher_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.339604 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/utils/default_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/utils/exclusion_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    12859 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    31161 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/utils/scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/utils/warmstarting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.343604 syne_tune-0.7.0/syne_tune/optimizer/schedulers/synchronous/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/synchronous/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34062 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/synchronous/dehb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/synchronous/dehb_bracket.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/synchronous/dehb_bracket_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    19672 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/synchronous/hyperband.py
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket.py
--rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    12482 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/synchronous/hyperband_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/synchronous/hyperband_rung_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.343604 syne_tune-0.7.0/syne_tune/optimizer/schedulers/transfer_learning/
--rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/transfer_learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6999 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/transfer_learning/bounding_box.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.343604 syne_tune-0.7.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/normalization_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/quantile_based_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/transfer_learning/rush.py
--rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/transfer_learning/zero_shot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.343604 syne_tune-0.7.0/syne_tune/optimizer/schedulers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/utils/simple_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/optimizer/schedulers/utils/successive_halving.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.343604 syne_tune-0.7.0/syne_tune/remote/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/remote/estimators.py
--rw-r--r--   0 runner    (1001) docker     (123)    14281 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/remote/remote_launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/remote/remote_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/remote/remote_metrics_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/remote/scheduling.py
--rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/results_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/stopping_criterion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/try_import.py
--rw-r--r--   0 runner    (1001) docker     (123)    31764 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/tuner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/tuner_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)    10789 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/tuning_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    10441 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.343604 syne_tune-0.7.0/syne_tune/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/utils/config_as_json.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/utils/parse_bool.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-25 13:19:34.000000 syne_tune-0.7.0/syne_tune/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:19:49.319603 syne_tune-0.7.0/syne_tune.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19123 2023-05-25 13:19:49.000000 syne_tune-0.7.0/syne_tune.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15453 2023-05-25 13:19:49.000000 syne_tune-0.7.0/syne_tune.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 13:19:49.000000 syne_tune-0.7.0/syne_tune.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-25 13:19:49.000000 syne_tune-0.7.0/syne_tune.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-25 13:19:49.000000 syne_tune-0.7.0/syne_tune.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.744142 syne_tune-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-06-20 15:04:35.000000 syne_tune-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-20 15:04:35.000000 syne_tune-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-20 15:04:35.000000 syne_tune-0.8.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    19768 2023-06-20 15:04:45.744142 syne_tune-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18904 2023-06-20 15:04:35.000000 syne_tune-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-20 15:04:45.748142 syne_tune-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-20 15:04:35.000000 syne_tune-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.724142 syne_tune-0.8.0/syne_tune/
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.724142 syne_tune-0.8.0/syne_tune/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15659 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/backend/local_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.724142 syne_tune-0.8.0/syne_tune/backend/python_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/backend/python_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/backend/python_backend/python_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/backend/python_backend/python_entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.724142 syne_tune-0.8.0/syne_tune/backend/sagemaker_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/backend/sagemaker_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/backend/sagemaker_backend/custom_framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/backend/sagemaker_backend/instance-types-cost.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/backend/sagemaker_backend/instance_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24530 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/backend/sagemaker_backend/sagemaker_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21131 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/backend/sagemaker_backend/sagemaker_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.724142 syne_tune-0.8.0/syne_tune/backend/simulator_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/backend/simulator_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/backend/simulator_backend/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22589 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/backend/simulator_backend/simulator_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/backend/simulator_backend/simulator_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/backend/simulator_backend/time_keeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/backend/time_keeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/backend/trial_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/backend/trial_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.728142 syne_tune-0.8.0/syne_tune/blackbox_repository/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/blackbox_repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/blackbox_repository/blackbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/blackbox_repository/blackbox_offline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22192 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/blackbox_repository/blackbox_surrogate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17442 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/blackbox_repository/blackbox_tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.728142 syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/blackbox_recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/recipes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.728142 syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/scripts/fcnet_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/scripts/icml2020_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.728142 syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10223 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/lcbench.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10468 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/scripts/nasbench201_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/scripts/pd1_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17778 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/scripts/yahpo_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/blackbox_repository/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/blackbox_repository/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18952 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/blackbox_repository/simulated_tabular_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/blackbox_repository/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.728142 syne_tune-0.8.0/syne_tune/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22237 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/callbacks/hyperband_remove_checkpoints_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/callbacks/hyperband_remove_checkpoints_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/callbacks/remove_checkpoints_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/callbacks/tensorboard_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43893 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/config_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.728142 syne_tune-0.8.0/syne_tune/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/experiments/aggregate_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17164 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/experiments/experiment_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/experiments/multiobjective.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16366 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/experiments/plot_per_trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36758 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/experiments/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17712 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/experiments/results_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/num_gpu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.728142 syne_tune-0.8.0/syne_tune/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40558 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/baselines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.732142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17051 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/fifo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59571 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/hyperband.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/hyperband_checkpoint_removal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/hyperband_cost_promotion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12528 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/hyperband_pasha.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11942 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/hyperband_promotion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/hyperband_rush.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15115 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/hyperband_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/median_stopping_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/multi_fidelity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.732142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/multiobjective/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/multiobjective/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/multiobjective/linear_scalarizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11212 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/multiobjective/moasha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/multiobjective/multi_objective_regularized_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/multiobjective/multi_surrogate_multi_objective_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/multiobjective/multiobjective_priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/multiobjective/non_dominated_priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8757 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/multiobjective/nsga2_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/multiobjective/random_scalarization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/multiobjective/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.732142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/neuralbands/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/neuralbands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/neuralbands/networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/neuralbands/neuralband.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22189 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/neuralbands/neuralband_supplement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15111 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/pbt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/random_seeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8676 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/ray_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/remove_checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/scheduler_searcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.732142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.732142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.732142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/config_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13227 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/tuning_job_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.736142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/custom_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40693 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14767 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon_blocks_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11243 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gpr_mcmc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.736142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13474 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/gp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15300 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/posterior_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19410 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.736142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/gpind_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10699 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/posterior_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.736142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10504 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/cross_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13361 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/exponential_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/fabolas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/freeze_thaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/product_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/range_kernel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.736142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18991 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/freeze_thaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/gpiss_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42009 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/issm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/model_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27009 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/posterior_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13024 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/optimization_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16368 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13238 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10095 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/target_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/warping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.740142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.740142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/cost_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/linear_cost_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14332 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/sklearn_cost_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost_fifo_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6919 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_mcmc_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18163 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17447 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gpiss_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/kernel_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15047 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_skipopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16108 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/sklearn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_multi_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_single_fidelity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.740142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.740142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16077 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13375 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.740142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/comparison_gpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/debug_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/test_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.740142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bore/
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10866 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bore/bore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bore/de.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bore/gp_classififer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bore/mlp_classififer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bore/multi_fidelity_bore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.740142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/botorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/botorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12264 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/botorch/botorch_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/botorch/botorch_transfer_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bracket_distribution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.740142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/constrained/
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/constrained/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/constrained/constrained_gp_fifo_searcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.740142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/cost_aware/
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/cost_aware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_fifo_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_multifidelity_searcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.740142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/dyhpo/
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/dyhpo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18409 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/dyhpo/dyhpo_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10575 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/dyhpo/hyperband_dyhpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16141 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/gp_fifo_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13439 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/gp_multifidelity_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42227 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/gp_searcher_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/gp_searcher_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.744142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/hypertune/
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/hypertune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_bracket_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_searcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.744142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/kde/
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/kde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17166 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/kde/kde_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/kde/multi_fidelity_kde_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34595 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/model_based_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15674 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/random_grid_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/regularized_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14507 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14854 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/searcher_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/searcher_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/searcher_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.744142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/sklearn/sklearn_surrogate_searcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.744142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/utils/default_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/utils/exclusion_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12859 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31161 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/utils/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/utils/warmstarting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.744142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/synchronous/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/synchronous/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34062 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/synchronous/dehb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/synchronous/dehb_bracket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/synchronous/dehb_bracket_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19684 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/synchronous/hyperband.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12482 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/synchronous/hyperband_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/synchronous/hyperband_rung_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.744142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/transfer_learning/
+-rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/transfer_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/transfer_learning/bounding_box.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.744142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/normalization_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7623 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/quantile_based_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/transfer_learning/rush.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/transfer_learning/zero_shot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.744142 syne_tune-0.8.0/syne_tune/optimizer/schedulers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/utils/simple_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/optimizer/schedulers/utils/successive_halving.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.744142 syne_tune-0.8.0/syne_tune/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/remote/estimators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14281 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/remote/remote_launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/remote/remote_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/remote/remote_metrics_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/remote/scheduling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/results_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/stopping_criterion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/try_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31764 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/tuner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/tuner_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10789 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/tuning_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10441 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.744142 syne_tune-0.8.0/syne_tune/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/utils/config_as_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/utils/parse_bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 15:04:35.000000 syne_tune-0.8.0/syne_tune/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:04:45.724142 syne_tune-0.8.0/syne_tune.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19768 2023-06-20 15:04:45.000000 syne_tune-0.8.0/syne_tune.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15789 2023-06-20 15:04:45.000000 syne_tune-0.8.0/syne_tune.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:04:45.000000 syne_tune-0.8.0/syne_tune.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-20 15:04:45.000000 syne_tune-0.8.0/syne_tune.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-20 15:04:45.000000 syne_tune-0.8.0/syne_tune.egg-info/top_level.txt
```

### Comparing `syne_tune-0.7.0/LICENSE` & `syne_tune-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/PKG-INFO` & `syne_tune-0.8.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,56 +1,29 @@
-Metadata-Version: 2.1
-Name: syne_tune
-Version: 0.7.0
-Summary: Distributed Hyperparameter Optimization on SageMaker
-Author: AWS
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
-Provides-Extra: gpsearchers
-Provides-Extra: kde
-Provides-Extra: dev
-Provides-Extra: aws
-Provides-Extra: moo
-Provides-Extra: visual
-Provides-Extra: blackbox-repository
-Provides-Extra: benchmarks
-Provides-Extra: yahpo
-Provides-Extra: raytune
-Provides-Extra: botorch
-Provides-Extra: bore
-Provides-Extra: extra
-License-File: LICENSE
-License-File: NOTICE
-
 # Syne Tune: Large-Scale and Reproducible Hyperparameter Optimization
 
 [![release](https://img.shields.io/github/v/release/awslabs/syne-tune)](https://pypi.org/project/syne-tune/)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Downloads](https://pepy.tech/badge/syne-tune/month)](https://pepy.tech/project/syne-tune)
 [![Documentation](https://readthedocs.org/projects/syne-tune/badge/?version=latest)](https://syne-tune.readthedocs.io)
 [![Python Version](https://img.shields.io/static/v1?label=python&message=3.7%20%7C%203.8%20%7C%203.9&color=blue?style=flat-square&logo=python)](https://pypi.org/project/syne-tune/)
 [![codecov.io](https://codecov.io/github/awslabs/syne-tune/branch/main/graphs/badge.svg)](https://app.codecov.io/gh/awslabs/syne-tune)
 
-![Alt Text](docs/source/synetune.gif)
+![Syne Tune](docs/source/synetune.gif)
+
+**[Documentation](https://syne-tune.readthedocs.io/en/latest/index.html)** | **[Tutorials](https://syne-tune.readthedocs.io/en/latest/tutorials/basics/README.html)** | **[API Reference](https://syne-tune.readthedocs.io/en/latest/_apidoc/modules.html#)** | **[PyPI](https://pypi.org/project/syne-tune)** | **[Latest Blog Post](https://aws.amazon.com/blogs/machine-learning/hyperparameter-optimization-for-fine-tuning-pre-trained-transformer-models-from-hugging-face/)**
 
-[Documentation](https://syne-tune.readthedocs.io/en/latest/index.html)
+Syne Tune provides state-of-the-art algorithms for hyperparameter optimization (HPO) with the following key features:
 
-This package provides state-of-the-art algorithms for hyperparameter optimization (HPO) with the following key features:
 * Wide coverage (>20) of different HPO methods, including:
-  * Asynchronous versions to maximize utilization and distributed versions (i.e., with multiple workers);
+  * Asynchronous and distributed tuning (i.e., with multiple workers);
   * Multi-fidelity methods supporting model-based decisions (BOHB and MOBSTER);
-  * Hyperparameter transfer learning to speed up (repeated) tuning jobs;
+  * Transfer learning to speed up (repeated) tuning jobs;
   * Multi-objective optimizers that can tune multiple objectives simultaneously (such as accuracy and latency).
-* HPO can be run in different environments (locally, AWS, simulation) by changing just one line of code.
-* Out-of-the-box tabulated benchmarks that allows you simulate results in seconds while preserving the real dynamics of asynchronous or synchronous HPO with any number of workers.
+* Run on different compute environments (locally, AWS, simulation) by changing just one line of code.
+* Out-of-the-box tabulated benchmarks allow you to simulate results in seconds while preserving the real dynamics of asynchronous or synchronous HPO with any number of workers.
 
 ## Installing
 
 To install Syne Tune from pip, you can simply do:
 
 ```bash
 pip install 'syne-tune[extra]'
@@ -100,15 +73,15 @@
     for step in range(args.epochs):
         time.sleep(0.1)
         dummy_score = 1.0 / (0.1 + args.width * step / 100) + args.height * 0.1
         # Feed the score back to Syne Tune.
         report(epoch=step + 1, mean_loss=dummy_score)
 ```
 
-Once you have a script reporting metric, you can launch a tuning as-follow:
+Once you have a training script reporting a metric, you can launch a tuning as follows:
 
 ```python
 # launch_height_simple.py
 from syne_tune import Tuner, StoppingCriterion
 from syne_tune.backend import LocalBackend
 from syne_tune.config_space import randint
 from syne_tune.optimizer.baselines import ASHA
@@ -169,21 +142,23 @@
 
 The searchers fall into four broad categories, **deterministic**, **random**, **evolutionary** and **model-based**. The random searchers sample candidate hyperparameter configurations uniformly at random, while the model-based searchers sample them non-uniformly at random, according to a model (e.g., Gaussian process, density ration estimator, etc.) and an acquisition function. The evolutionary searchers make use of an evolutionary algorithm.
 
 Syne Tune also supports [BoTorch](https://github.com/awslabs/syne-tune/blob/main/syne_tune/optimizer/schedulers/searchers/botorch/botorch_searcher.py) searchers.
 
 ## Supported multi-objective optimization methods
 
-Method | Reference | Searcher | Asynchronous? | Multi-fidelity? | Transfer?
-:--- | :---: | :---: | :---: | :---: | :---: 
-Constrained Bayesian Optimization | Gardner, et al. (2014) | model-based | yes | no | no
-MOASHA | Schmucker, et al. (2021) | random | yes | yes | no
-NSGA-2 | Deb, et al. (2002) | evolutionary | no | no | no
+Method |          Reference          |   Searcher   | Asynchronous? | Multi-fidelity? | Transfer?
+:--- |:---------------------------:|:------------:| :---: | :---: | :---: 
+Constrained Bayesian Optimization |   Gardner, et al. (2014)    | model-based  | yes | no | no
+MOASHA |  Schmucker, et al. (2021)   |    random    | yes | yes | no
+NSGA-2 |     Deb, et al. (2002)      | evolutionary | no | no | no
+Multi Objective Multi Surrogate (MSMOS) | Guerrero-Viu, et al. (2021) | model-based  | no | no | no
+MSMOS wihh random scalarization |    Paria, et al. (2018)     | model-based  | no | no | no
 
-HPO methods listed can be used in a multi-objective setting by scalarization or non-dominated sorting. See [multiobjective_priority.py](syne_tune/optimizers/schedulers/multiobjective/multiobjective_priority.py) for details.
+HPO methods listed can be used in a multi-objective setting by scalarization or non-dominated sorting. See [multiobjective_priority.py](syne_tune/optimizer/schedulers/multiobjective/multiobjective_priority.py) for details.
 
 ## Examples
 
 You will find many examples in the [examples/](examples/) folder illustrating
 different functionalities provided by Syne Tune. For example:
 * [launch_height_baselines.py](examples/launch_height_baselines.py):
   launches HPO locally, tuning a simple script 
@@ -197,17 +172,17 @@
   launches the HPO loop on SageMaker rather than a local machine, trial can be executed either
   the remote machine or distributed again as separate SageMaker training jobs. See 
   [launch_height_sagemaker_remote_launcher.py](examples/launch_height_sagemaker_remote_launcher.py)
   for remote launching with the help of RemoteTuner also discussed in one of the FAQs.
 * [launch_height_sagemaker.py](examples/launch_height_sagemaker.py):
   launches HPO on SageMaker to tune a SageMaker Pytorch estimator
 * [launch_bayesopt_constrained.py](examples/launch_bayesopt_constrained.py):
-  launches Bayesian contrained hyperparameter optimization
+  launches Bayesian constrained hyperparameter optimization
 * [launch_height_sagemaker_custom_image.py](examples/launch_height_sagemaker_custom_image.py):
-  launches HPO on SageMaker to tune a entry point with a custom docker image
+  launches HPO on SageMaker to tune an entry point with a custom docker image
 * [launch_plot_results.py](examples/launch_plot_results.py): shows how to plot
   results of a HPO experiment
 * [launch_tensorboard_example.py](examples/launch_tensorboard_example.py):
   shows how results can be visualized on the fly with TensorBoard
 * [launch_nasbench201_simulated.py](examples/launch_nasbench201_simulated.py):
   demonstrates simulation of experiments on a tabulated benchmark
 * [launch_fashionmnist.py](examples/launch_fashionmnist.py):
```

### Comparing `syne_tune-0.7.0/README.md` & `syne_tune-0.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,58 @@
+Metadata-Version: 2.1
+Name: syne_tune
+Version: 0.8.0
+Summary: Distributed Hyperparameter Optimization on SageMaker
+Author: AWS
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/markdown
+Provides-Extra: gpsearchers
+Provides-Extra: kde
+Provides-Extra: dev
+Provides-Extra: aws
+Provides-Extra: moo
+Provides-Extra: visual
+Provides-Extra: sklearn
+Provides-Extra: blackbox-repository
+Provides-Extra: benchmarks
+Provides-Extra: yahpo
+Provides-Extra: raytune
+Provides-Extra: botorch
+Provides-Extra: bore
+Provides-Extra: extra
+License-File: LICENSE
+License-File: NOTICE
+
 # Syne Tune: Large-Scale and Reproducible Hyperparameter Optimization
 
 [![release](https://img.shields.io/github/v/release/awslabs/syne-tune)](https://pypi.org/project/syne-tune/)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Downloads](https://pepy.tech/badge/syne-tune/month)](https://pepy.tech/project/syne-tune)
 [![Documentation](https://readthedocs.org/projects/syne-tune/badge/?version=latest)](https://syne-tune.readthedocs.io)
 [![Python Version](https://img.shields.io/static/v1?label=python&message=3.7%20%7C%203.8%20%7C%203.9&color=blue?style=flat-square&logo=python)](https://pypi.org/project/syne-tune/)
 [![codecov.io](https://codecov.io/github/awslabs/syne-tune/branch/main/graphs/badge.svg)](https://app.codecov.io/gh/awslabs/syne-tune)
 
-![Alt Text](docs/source/synetune.gif)
+![Syne Tune](docs/source/synetune.gif)
+
+**[Documentation](https://syne-tune.readthedocs.io/en/latest/index.html)** | **[Tutorials](https://syne-tune.readthedocs.io/en/latest/tutorials/basics/README.html)** | **[API Reference](https://syne-tune.readthedocs.io/en/latest/_apidoc/modules.html#)** | **[PyPI](https://pypi.org/project/syne-tune)** | **[Latest Blog Post](https://aws.amazon.com/blogs/machine-learning/hyperparameter-optimization-for-fine-tuning-pre-trained-transformer-models-from-hugging-face/)**
 
-[Documentation](https://syne-tune.readthedocs.io/en/latest/index.html)
+Syne Tune provides state-of-the-art algorithms for hyperparameter optimization (HPO) with the following key features:
 
-This package provides state-of-the-art algorithms for hyperparameter optimization (HPO) with the following key features:
 * Wide coverage (>20) of different HPO methods, including:
-  * Asynchronous versions to maximize utilization and distributed versions (i.e., with multiple workers);
+  * Asynchronous and distributed tuning (i.e., with multiple workers);
   * Multi-fidelity methods supporting model-based decisions (BOHB and MOBSTER);
-  * Hyperparameter transfer learning to speed up (repeated) tuning jobs;
+  * Transfer learning to speed up (repeated) tuning jobs;
   * Multi-objective optimizers that can tune multiple objectives simultaneously (such as accuracy and latency).
-* HPO can be run in different environments (locally, AWS, simulation) by changing just one line of code.
-* Out-of-the-box tabulated benchmarks that allows you simulate results in seconds while preserving the real dynamics of asynchronous or synchronous HPO with any number of workers.
+* Run on different compute environments (locally, AWS, simulation) by changing just one line of code.
+* Out-of-the-box tabulated benchmarks allow you to simulate results in seconds while preserving the real dynamics of asynchronous or synchronous HPO with any number of workers.
 
 ## Installing
 
 To install Syne Tune from pip, you can simply do:
 
 ```bash
 pip install 'syne-tune[extra]'
@@ -72,15 +102,15 @@
     for step in range(args.epochs):
         time.sleep(0.1)
         dummy_score = 1.0 / (0.1 + args.width * step / 100) + args.height * 0.1
         # Feed the score back to Syne Tune.
         report(epoch=step + 1, mean_loss=dummy_score)
 ```
 
-Once you have a script reporting metric, you can launch a tuning as-follow:
+Once you have a training script reporting a metric, you can launch a tuning as follows:
 
 ```python
 # launch_height_simple.py
 from syne_tune import Tuner, StoppingCriterion
 from syne_tune.backend import LocalBackend
 from syne_tune.config_space import randint
 from syne_tune.optimizer.baselines import ASHA
@@ -141,21 +171,23 @@
 
 The searchers fall into four broad categories, **deterministic**, **random**, **evolutionary** and **model-based**. The random searchers sample candidate hyperparameter configurations uniformly at random, while the model-based searchers sample them non-uniformly at random, according to a model (e.g., Gaussian process, density ration estimator, etc.) and an acquisition function. The evolutionary searchers make use of an evolutionary algorithm.
 
 Syne Tune also supports [BoTorch](https://github.com/awslabs/syne-tune/blob/main/syne_tune/optimizer/schedulers/searchers/botorch/botorch_searcher.py) searchers.
 
 ## Supported multi-objective optimization methods
 
-Method | Reference | Searcher | Asynchronous? | Multi-fidelity? | Transfer?
-:--- | :---: | :---: | :---: | :---: | :---: 
-Constrained Bayesian Optimization | Gardner, et al. (2014) | model-based | yes | no | no
-MOASHA | Schmucker, et al. (2021) | random | yes | yes | no
-NSGA-2 | Deb, et al. (2002) | evolutionary | no | no | no
+Method |          Reference          |   Searcher   | Asynchronous? | Multi-fidelity? | Transfer?
+:--- |:---------------------------:|:------------:| :---: | :---: | :---: 
+Constrained Bayesian Optimization |   Gardner, et al. (2014)    | model-based  | yes | no | no
+MOASHA |  Schmucker, et al. (2021)   |    random    | yes | yes | no
+NSGA-2 |     Deb, et al. (2002)      | evolutionary | no | no | no
+Multi Objective Multi Surrogate (MSMOS) | Guerrero-Viu, et al. (2021) | model-based  | no | no | no
+MSMOS wihh random scalarization |    Paria, et al. (2018)     | model-based  | no | no | no
 
-HPO methods listed can be used in a multi-objective setting by scalarization or non-dominated sorting. See [multiobjective_priority.py](syne_tune/optimizers/schedulers/multiobjective/multiobjective_priority.py) for details.
+HPO methods listed can be used in a multi-objective setting by scalarization or non-dominated sorting. See [multiobjective_priority.py](syne_tune/optimizer/schedulers/multiobjective/multiobjective_priority.py) for details.
 
 ## Examples
 
 You will find many examples in the [examples/](examples/) folder illustrating
 different functionalities provided by Syne Tune. For example:
 * [launch_height_baselines.py](examples/launch_height_baselines.py):
   launches HPO locally, tuning a simple script 
@@ -169,17 +201,17 @@
   launches the HPO loop on SageMaker rather than a local machine, trial can be executed either
   the remote machine or distributed again as separate SageMaker training jobs. See 
   [launch_height_sagemaker_remote_launcher.py](examples/launch_height_sagemaker_remote_launcher.py)
   for remote launching with the help of RemoteTuner also discussed in one of the FAQs.
 * [launch_height_sagemaker.py](examples/launch_height_sagemaker.py):
   launches HPO on SageMaker to tune a SageMaker Pytorch estimator
 * [launch_bayesopt_constrained.py](examples/launch_bayesopt_constrained.py):
-  launches Bayesian contrained hyperparameter optimization
+  launches Bayesian constrained hyperparameter optimization
 * [launch_height_sagemaker_custom_image.py](examples/launch_height_sagemaker_custom_image.py):
-  launches HPO on SageMaker to tune a entry point with a custom docker image
+  launches HPO on SageMaker to tune an entry point with a custom docker image
 * [launch_plot_results.py](examples/launch_plot_results.py): shows how to plot
   results of a HPO experiment
 * [launch_tensorboard_example.py](examples/launch_tensorboard_example.py):
   shows how results can be visualized on the fly with TensorBoard
 * [launch_nasbench201_simulated.py](examples/launch_nasbench201_simulated.py):
   demonstrates simulation of experiments on a tabulated benchmark
 * [launch_fashionmnist.py](examples/launch_fashionmnist.py):
```

### Comparing `syne_tune-0.7.0/setup.py` & `syne_tune-0.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,23 +36,25 @@
     "syne_tune/blackbox_repository/conversion_scripts/scripts/requirements-yahpo.txt"
 )
 required_benchmarks = load_benchmark_requirements()
 required_dev = load_requirements("requirements-dev.txt")
 required_aws = load_requirements("requirements-aws.txt")
 required_moo = load_requirements("requirements-moo.txt")
 required_visual = load_requirements("requirements-visual.txt")
+required_sklearn = load_requirements("requirements-sklearn.txt")
 
 long_description = (Path(__file__).parent / "README.md").read_text()
 required_extra = (
     required_gpsearchers
     + required_kde
     + required_dev
     + required_aws
     + required_moo
     + required_visual
+    + required_sklearn
     + required_blackbox_repository
     + required_benchmarks
     + required_yahpo
     + required_ray
 )
 
 # Botorch only supports python version >= 3.8
@@ -75,14 +77,15 @@
     extras_require={
         "gpsearchers": required_gpsearchers,
         "kde": required_kde,
         "dev": required_dev,
         "aws": required_aws,
         "moo": required_moo,
         "visual": required_visual,
+        "sklearn": required_sklearn,
         "blackbox-repository": required_blackbox_repository,
         "benchmarks": required_benchmarks,
         "yahpo": required_yahpo,
         "raytune": required_ray,
         "botorch": required_botorch,
         "bore": required_bore,
         "extra": required_extra,
```

### Comparing `syne_tune-0.7.0/syne_tune/__init__.py` & `syne_tune-0.8.0/syne_tune/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/backend/__init__.py` & `syne_tune-0.8.0/syne_tune/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/backend/local_backend.py` & `syne_tune-0.8.0/syne_tune/backend/local_backend.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/backend/python_backend/__init__.py` & `syne_tune-0.8.0/syne_tune/backend/python_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/backend/python_backend/python_backend.py` & `syne_tune-0.8.0/syne_tune/backend/python_backend/python_backend.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/backend/python_backend/python_entrypoint.py` & `syne_tune-0.8.0/syne_tune/backend/python_backend/python_entrypoint.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/backend/sagemaker_backend/__init__.py` & `syne_tune-0.8.0/syne_tune/backend/sagemaker_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/backend/sagemaker_backend/custom_framework.py` & `syne_tune-0.8.0/syne_tune/backend/sagemaker_backend/custom_framework.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/backend/sagemaker_backend/instance-types-cost.csv` & `syne_tune-0.8.0/syne_tune/backend/sagemaker_backend/instance-types-cost.csv`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/backend/sagemaker_backend/instance_info.py` & `syne_tune-0.8.0/syne_tune/backend/sagemaker_backend/instance_info.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/backend/sagemaker_backend/sagemaker_backend.py` & `syne_tune-0.8.0/syne_tune/backend/sagemaker_backend/sagemaker_backend.py`

 * *Files 3% similar despite different names*

```diff
@@ -123,14 +123,16 @@
         self.paused_jobs = set()
         self.stopped_jobs = set()
         # Counts how often a trial has been resumed
         self.resumed_counter = dict()
         if s3_path is None:
             s3_path = s3_experiment_path()
         self.s3_path = s3_path.rstrip("/")
+        # ``tuner_name`` has to be set before the backend can be used. This is
+        # typically done when the ``Tuner`` is created
         self.tuner_name = None
         # Trials which may currently be busy (status in ``BUSY_STATUS``). The
         # corresponding jobs are polled for status in ``busy_trial_ids``, and
         # new trials are addd in :meth:`_schedule`.
         # Note: A trial can be in ``paused_jobs`` or ``stopped_jobs`` and still
         # be busy, because the underlying SM training job is still not completed
         self._busy_trial_id_candidates = set()
@@ -177,18 +179,22 @@
                 trial_res.status = Status.stopped
         return res
 
     @staticmethod
     def _numpy_serialize(mydict):
         return json.loads(dump_json_with_numpy(mydict))
 
+    def _assert_tuner_name_is_set(self):
+        assert (
+            self.tuner_name is not None
+        ), "tuner_name has to be set (by calling set_path) before the backend can be used"
+
     def _checkpoint_s3_uri_for_trial(self, trial_id: int) -> str:
-        res_path = self.s3_path
-        if self.tuner_name is not None:
-            res_path = f"{res_path}/{self.tuner_name}"
+        self._assert_tuner_name_is_set()
+        res_path = f"{self.s3_path}/{self.tuner_name}"
         return f"{res_path}/{str(trial_id)}/checkpoints/"
 
     def _config_json_filename(self, trial_id: int, with_path: bool) -> str:
         fname = CONFIG_JSON_FILENAME + f"_{trial_id}.json"
         if with_path and self.source_dir is not None:
             return str(Path(self.source_dir) / fname)
         else:
@@ -317,14 +323,15 @@
         :param trial_id: ID of trial
         :param job_running_number: Number of times the trial was resumed
         :return: sagemaker job name with the form
             ``[trial_id]-[job_running_number]-[tuner_name]``. ``trial_id`` is put
              first to avoid mismatch when searching for job information in
             SageMaker from prefix.
         """
+        self._assert_tuner_name_is_set()
         job_name = f"{trial_id}"
         if job_running_number > 0:
             job_name += f"-{job_running_number}"
         job_name += f"-{self.tuner_name}"
         return job_name
 
     def _pause_trial(self, trial_id: int, result: Optional[dict]):
@@ -518,16 +525,20 @@
                 f"{num_action_calls - num_successful_action_calls} "
                 "files. Error:\n" + result["first_error_message"]
             )
 
     def set_path(
         self, results_root: Optional[str] = None, tuner_name: Optional[str] = None
     ):
-        # we use the tuner-name to set the checkpoint directory
-        self.tuner_name = tuner_name
+        """
+        For this backend, it is mandatory to call this method passing ``tuner_name``
+        before the backend is used. ``results_root`` is ignored here.
+        """
+        if tuner_name is not None:
+            self.tuner_name = tuner_name
 
     def on_tuner_save(self):
         # Re-initialize the session after :class:`~syne_tune.Tuner` is serialized
         self.initialize_sagemaker_session()
 
     def _cleanup_after_trial(self, trial_id: int):
         if self.pass_args_as_json:
```

### Comparing `syne_tune-0.7.0/syne_tune/backend/sagemaker_backend/sagemaker_utils.py` & `syne_tune-0.8.0/syne_tune/backend/sagemaker_backend/sagemaker_utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/backend/simulator_backend/__init__.py` & `syne_tune-0.8.0/syne_tune/backend/simulator_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/backend/simulator_backend/events.py` & `syne_tune-0.8.0/syne_tune/backend/simulator_backend/events.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/backend/simulator_backend/simulator_backend.py` & `syne_tune-0.8.0/syne_tune/backend/simulator_backend/simulator_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -491,15 +491,15 @@
         config_str = " ".join(
             [f"--{key} {value}" for key, value in config_copy.items()]
         )
 
         dump_json_with_numpy(config, trial_path / "config.json")
         cmd = f"python {self.entry_point} {config_str}"
         env = dict(os.environ)
-        logging.info(f"running script with command: {cmd}")
+        logger.info(f"running script with command: {cmd}")
         with open(trial_path / "std.out", "a") as stdout:
             with open(trial_path / "std.err", "a") as stderr:
                 return_status = subprocess.run(
                     cmd.split(" "), stdout=stdout, stderr=stderr, env=env
                 )
         if return_status.returncode == 0:
             status = Status.completed
```

### Comparing `syne_tune-0.7.0/syne_tune/backend/simulator_backend/simulator_callback.py` & `syne_tune-0.8.0/syne_tune/backend/simulator_backend/simulator_callback.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/backend/simulator_backend/time_keeper.py` & `syne_tune-0.8.0/syne_tune/backend/simulator_backend/time_keeper.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/backend/time_keeper.py` & `syne_tune-0.8.0/syne_tune/backend/time_keeper.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/backend/trial_backend.py` & `syne_tune-0.8.0/syne_tune/backend/trial_backend.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/backend/trial_status.py` & `syne_tune-0.8.0/syne_tune/backend/trial_status.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/blackbox_repository/__init__.py` & `syne_tune-0.8.0/syne_tune/blackbox_repository/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/blackbox_repository/blackbox.py` & `syne_tune-0.8.0/syne_tune/blackbox_repository/blackbox.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/blackbox_repository/blackbox_offline.py` & `syne_tune-0.8.0/syne_tune/blackbox_repository/blackbox_offline.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/blackbox_repository/blackbox_surrogate.py` & `syne_tune-0.8.0/syne_tune/blackbox_repository/blackbox_surrogate.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/blackbox_repository/blackbox_tabular.py` & `syne_tune-0.8.0/syne_tune/blackbox_repository/blackbox_tabular.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/__init__.py` & `syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/blackbox_recipe.py` & `syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/blackbox_recipe.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/recipes.py` & `syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/recipes.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/scripts/__init__.py` & `syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/scripts/fcnet_import.py` & `syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/scripts/fcnet_import.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/scripts/icml2020_import.py` & `syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/scripts/icml2020_import.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/__init__.py` & `syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/api.py` & `syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/api.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/lcbench.py` & `syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/scripts/lcbench/lcbench.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/scripts/nasbench201_import.py` & `syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/scripts/nasbench201_import.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/scripts/pd1_import.py` & `syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/scripts/pd1_import.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/scripts/yahpo_import.py` & `syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/scripts/yahpo_import.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/blackbox_repository/conversion_scripts/utils.py` & `syne_tune-0.8.0/syne_tune/blackbox_repository/conversion_scripts/utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/blackbox_repository/repository.py` & `syne_tune-0.8.0/syne_tune/blackbox_repository/repository.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/blackbox_repository/serialize.py` & `syne_tune-0.8.0/syne_tune/blackbox_repository/serialize.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/blackbox_repository/simulated_tabular_backend.py` & `syne_tune-0.8.0/syne_tune/blackbox_repository/simulated_tabular_backend.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/blackbox_repository/utils.py` & `syne_tune-0.8.0/syne_tune/blackbox_repository/utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/callbacks/__init__.py` & `syne_tune-0.8.0/syne_tune/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/callbacks/hyperband_remove_checkpoints_callback.py` & `syne_tune-0.8.0/syne_tune/callbacks/hyperband_remove_checkpoints_callback.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/callbacks/hyperband_remove_checkpoints_score.py` & `syne_tune-0.8.0/syne_tune/callbacks/hyperband_remove_checkpoints_score.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/callbacks/remove_checkpoints_callback.py` & `syne_tune-0.8.0/syne_tune/callbacks/remove_checkpoints_callback.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/callbacks/tensorboard_callback.py` & `syne_tune-0.8.0/syne_tune/callbacks/tensorboard_callback.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/config_space.py` & `syne_tune-0.8.0/syne_tune/config_space.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/constants.py` & `syne_tune-0.8.0/syne_tune/constants.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/experiments/__init__.py` & `syne_tune-0.8.0/syne_tune/experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/experiments/aggregate_results.py` & `syne_tune-0.8.0/syne_tune/experiments/aggregate_results.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,14 @@
     """
     The aggregate is the interquartile mean (IQM). Error bars are bootstrap
     estimate of 95% confidence interval for true IQM. This is the normal
     interval, based on the bootstrap variance estimate. While other bootstrap
     CI estimates are available, they are more expensive to compute.
 
     Note: Error bar scale depends on number of runs `n` via `1 / sqrt(n)`.
-
     """
 
     def _remove_mass(amat: np.ndarray, mass: float, col_index):
         remaining_mass = mass * np.ones(amat.shape[0])
         for col in col_index:
             subtract = np.minimum(remaining_mass, amat[:, col])
             remaining_mass -= subtract
```

### Comparing `syne_tune-0.7.0/syne_tune/experiments/experiment_result.py` & `syne_tune-0.8.0/syne_tune/experiments/experiment_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,29 +25,30 @@
 from syne_tune.constants import (
     ST_METADATA_FILENAME,
     ST_RESULTS_DATAFRAME_FILENAME,
     ST_TUNER_DILL_FILENAME,
     ST_TUNER_CREATION_TIMESTAMP,
     ST_TUNER_TIME,
 )
-from syne_tune.optimizer.schedulers.multiobjective.utils import hypervolume_cumulative
 from syne_tune.try_import import try_import_aws_message, try_import_visual_message
 from syne_tune.util import experiment_path, s3_experiment_path
 
 try:
     import boto3
     from botocore.exceptions import ClientError
 except ImportError:
     print(try_import_aws_message())
 
 try:
     import matplotlib.pyplot as plt
 except ImportError:
     print(try_import_visual_message())
 
+logger = logging.getLogger(__name__)
+
 
 @dataclass
 class ExperimentResult:
     """
     Wraps results dataframe and provides retrieval services.
 
     :param name: Name of experiment
@@ -78,15 +79,15 @@
     def plot_hypervolume(
         self,
         metrics_to_plot: Union[List[int], List[str]] = None,
         reference_point: np.ndarray = None,
         figure_path: str = None,
         **plt_kwargs,
     ):
-        """Plot best hyervolume value as function of wallclock time
+        """Plot best hypervolume value as function of wallclock time
 
         :param reference_point: Reference point for hypervolume calculations.
             If None, the maximum values of each metric is used.
         :param figure_path: If specified, defines the path where the figure will be saved.
             If None, the figure is shown
         :param plt_kwargs: Arguments to :func:`matplotlib.pyplot.plot`
         """
@@ -101,14 +102,18 @@
             *[self._metric_name_mode(metric) for metric in metrics_to_plot]
         )
         assert np.all(
             [metric_mode == "max" for metric_mode in metric_modes]
         ), f"All metrics must be maximized but the following modes were selected: {metric_modes}"
 
         if self.results is not None and len(self.results) > 0:
+            from syne_tune.optimizer.schedulers.multiobjective.utils import (
+                hypervolume_cumulative,
+            )
+
             results_df = self.results.sort_values(ST_TUNER_TIME)
 
             x = self.results.loc[:, ST_TUNER_TIME]
             results_array = results_df[list(metric_names)].values
             hypervolume_indicator = hypervolume_cumulative(
                 results_array, reference_point
             )
@@ -206,15 +211,15 @@
             metric_name = self.metric_names()[metric]
         else:
             raise AttributeError(
                 f"metic must be <int> or <str> but {type(metric)} was provided"
             )
 
         if len(self.metric_names()) > 1 and verbose:
-            logging.warning(
+            logger.warning(
                 "Several metrics exists, this will "
                 f"use metric={metric_name} (index={metric}) out of {self.metric_names()}."
             )
 
         metric_mode = self.metric_mode()
         if len(metric_mode) > 1:
             metric_mode = metric_mode[metric]
@@ -246,18 +251,18 @@
     result_files = [
         ST_METADATA_FILENAME,
         ST_RESULTS_DATAFRAME_FILENAME,
         ST_TUNER_DILL_FILENAME,
     ]
     for file in result_files:
         try:
-            logging.info(f"downloading {file} on {s3_path}")
+            logger.info(f"downloading {file} on {s3_path}")
             s3.download_file(s3_bucket, f"{s3_key}/{file}", str(tgt_dir / file))
         except ClientError as e:
-            logging.info(f"could not find {file} on {s3_path}")
+            logger.info(f"could not find {file} on {s3_path}")
 
 
 def load_experiment(
     tuner_name: str,
     download_if_not_found: bool = True,
     load_tuner: bool = False,
     local_path: Optional[str] = None,
@@ -272,15 +277,15 @@
         ``~/{SYNE_TUNE_FOLDER}/`` is used.
     :param experiment_name: If given, this is used as first directory.
     :return: Result object
     """
     path = experiment_path(tuner_name, local_path)
     metadata_path = path / ST_METADATA_FILENAME
     if not (metadata_path.exists()) and download_if_not_found:
-        logging.info(
+        logger.info(
             f"experiment {tuner_name} not found locally, trying to get it from s3."
         )
         download_single_experiment(
             tuner_name=tuner_name, experiment_name=experiment_name
         )
     try:
         with open(metadata_path, "r") as f:
```

### Comparing `syne_tune-0.7.0/syne_tune/experiments/plot_per_trial.py` & `syne_tune-0.8.0/syne_tune/experiments/plot_per_trial.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # or in the "license" file accompanying this file. This file is distributed
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
-from typing import Optional, Tuple, Union, List, Iterable
+from typing import Optional, Tuple, Union, List, Iterable, Dict
 import logging
 import copy
 from dataclasses import dataclass
 
 import numpy as np
 import pandas as pd
 
@@ -43,57 +43,73 @@
 
 @dataclass
 class MultiFidelityParameters:
     """
     Parameters configuring the multi-fidelity version of
     :class:`TrialsOfExperimentResults`.
 
+    ``multifidelity_setups`` contains names of setups which are multi-fidelity,
+    the remaining ones are single-fidelity. It can also be a dictionary,
+    mapping a multi-fidelity setup name to ``True`` if this is a pause-and-resume
+    method (these are visualized differently), ``False`` otherwise (early
+    stopping method).
+
     :param rung_levels: See above. Positive integers, increasing
-    :param pause_resume_setups: Names of setups which are pause-and-resume
-        methods (these are visualized differently). Must be contained in
-        ``setups``
+    :param multifidelity_setups: See above
     """
 
     rung_levels: List[int]
-    pause_resume_setups: Iterable[str]
+    multifidelity_setups: Union[List[str], Dict[str, bool]]
 
     def check_params(self, setups: Iterable[str]):
-        assert set(setups).issuperset(self.pause_resume_setups), (
-            f"multi_fidelity_params.pause_resume_setups = {self.pause_resume_setups} "
+        if isinstance(self.multifidelity_setups, dict):
+            _mf_setups = list(self.multifidelity_setups.keys())
+        else:
+            _mf_setups = self.multifidelity_setups
+        assert set(setups).issuperset(_mf_setups), (
+            f"multi_fidelity_params.multifidelity_setups = {self.multifidelity_setups} "
             f"must be contained in setups = {setups}"
         )
         assert is_increasing(self.rung_levels) and is_positive_integer(
             self.rung_levels
         ), f"multi_fidelity_params.rung_levels = {self.rung_levels} must be increasing positive ints"
 
 
 class TrialsOfExperimentResults:
     """
     This class loads, processes, and plots metric results for single experiments,
     where the curves for different trials have different colours.
 
     Compared to :class:`~syne_tune.experiments.ComparativeResults`, each subfigure
-    uses data from a single experiment (one, benchmark, one seed, one setup). Both
+    uses data from a single experiment (one benchmark, one seed, one setup). Both
     benchmark and seed need to be chosen in :meth:`plot`. If there are different
-    setups, they give rise to subfigures (by default, one row with subfigures as
-    columns, but can be configured).
+    setups, they give rise to subfigures.
+
+    If ``plot_params.subplots`` is not given, the arrangement is one row with
+    columns corresponding to setups, and setup names as titles. Specify
+    ``plot_params.subplots`` in order to change this arrangement (e.g., to have
+    more than one row). Setups can be selected by using
+    ``plot_params.subplots.subplot_indices``. Also, if
+    ``plot_params.subplots.titles`` is not given, we use setup names, and each
+    subplot gets its own title (``plot_params.subplots.title_each_figure`` is
+    ignored).
 
     For ``plot_params``, we use the same
     :class:`~syne_tune.experiments.PlotParameters` as in
     :class:`~syne_tune.experiments.ComparativeResults`, but some fields are not
     used here (``title``, ``aggregate_mode``, ``show_one_trial``,
     ``subplots.legend_no``, ``subplots.xlims``).
 
     :param experiment_names: Tuple of experiment names (prefixes, without the
         timestamps)
     :param setups: Possible values of setup names
     :param metadata_to_setup: See above
     :param plot_params: Parameters controlling the plot. Can be overwritten
         in :meth:`plot`. See :class:`PlotParameters`
-    :param multi_fidelity_params: If given, we use a special variant taylored
+    :param multi_fidelity_params: If given, we use a special variant tailored
         to multi-fidelity methods (see :meth:`plot`).
     :param benchmark_key: Key for benchmark in metadata files. Defaults to
         "benchmark". If this is ``None``, there is only a single benchmark,
         and all results are merged together
     :param seed_key: Key for seed in metadata files. Defaults to "seed".
     :param with_subdirs: See above. Defaults to "*"
     :param datetime_bounds: See above
@@ -139,77 +155,96 @@
             f"Filtered results contain setup names {result['setup_names']}, "
             f"but should contain setup names {setups}"
         )
         self.setups = tuple(setups)
         self._default_plot_params = copy.deepcopy(plot_params)
         self._benchmark_key = benchmark_key
         if multi_fidelity_params is not None:
-            self._pause_resume_setups = set(multi_fidelity_params.pause_resume_setups)
+            self._multifidelity_setups = multi_fidelity_params.multifidelity_setups
+            if not isinstance(self._multifidelity_setups, dict):
+                self._multifidelity_setups = {
+                    name: False for name in self._multifidelity_setups
+                }
             # We need rung levels minus 1 below
             self._rung_levels = [
                 level - 1 for level in multi_fidelity_params.rung_levels
             ]
         else:
-            self._pause_resume_setups = None
-            self._rung_levels = None
+            self._multifidelity_setups = dict()
+            self._rung_levels = []
 
     def _plot_figure(
         self,
         df: pd.DataFrame,
         plot_params: PlotParameters,
         benchmark_name: Optional[str],
         seed: int,
     ):
         subplots = plot_params.subplots
         if subplots is not None:
-            subplots_kwargs = subplots.kwargs
             nrows = subplots.nrows
             ncols = subplots.ncols
+            subplot_indices = (
+                list(range(len(self.setups)))
+                if subplots.subplot_indices is None
+                else subplots.subplot_indices
+            )
             assert ncols * nrows >= len(
-                self.setups
-            ), f"Error in subplots.kwargs: ncols times nrows must be >= {len(self.setups)} (number of setups)"
+                subplot_indices
+            ), f"Error in subplots.kwargs: ncols times nrows must be >= {len(subplot_indices)} (number of setups)"
             subplots_kwargs = dict(
                 dict() if subplots.kwargs is None else subplots.kwargs,
                 nrows=nrows,
                 ncols=ncols,
             )
-            subplot_titles = subplots.titles
-            title_each_figure = subplots.title_each_figure
+            if subplots.titles is not None:
+                subplot_titles = subplots.titles
+                title_each_figure = subplots.title_each_figure
+            else:
+                # If ``plot_params.subplots.titles`` is not given, we use setup
+                # names as titles. In this case, each subfigure has its own
+                # title, not just each column
+                subplot_titles = [self.setups[ind] for ind in subplot_indices]
+                title_each_figure = True
         else:
             nrows = 1
             ncols = len(self.setups)
             subplots_kwargs = dict(nrows=nrows, ncols=ncols, sharey="all")
             subplot_titles = self.setups
             title_each_figure = False
+            subplot_indices = list(range(ncols))
         ylim = plot_params.ylim
         xlim = plot_params.xlim
         xlabel = plot_params.xlabel
         ylabel = plot_params.ylabel
         tick_params = plot_params.tick_params
         msg_prefix = f"seed = {seed}: "
         if benchmark_name is not None:
             msg_prefix = f"benchmark_name = {benchmark_name}, " + msg_prefix
-        is_multi_fidelity = self._rung_levels is not None
-        num_rungs = len(self._rung_levels) if is_multi_fidelity else 0
+        num_rungs = len(self._rung_levels)
 
         plt.figure(dpi=plot_params.dpi)
         figsize = (5 * ncols, 4 * nrows)
         fig, axs = plt.subplots(**subplots_kwargs, squeeze=False, figsize=figsize)
         for setup_name, setup_df in df.groupby("setup_name"):
             # Check that there is a single experiment per setup
             tuner_names = list(setup_df.tuner_name.unique())
             assert len(tuner_names) == 1, (
                 msg_prefix
                 + f"For setup_name = {setup_name} found tuner_names = {tuner_names}"
             )
             logger.info(msg_prefix + f"setup_name = {setup_name}: {tuner_names[0]}")
+            is_multi_fidelity = setup_name in self._multifidelity_setups
             pause_resume = (
-                setup_name in self._pause_resume_setups if is_multi_fidelity else False
+                self._multifidelity_setups[setup_name] if is_multi_fidelity else False
             )
-            subplot_no = self.setups.index(setup_name)
+            subplot_index = self.setups.index(setup_name)
+            if subplot_index not in subplot_indices:
+                continue
+            subplot_no = subplot_indices.index(subplot_index)
             row = subplot_no % nrows
             col = subplot_no // nrows
             ax = axs[row, col]
             current_color = [0] * (num_rungs + 1)
             for trial_id in setup_df.trial_id.unique():
                 sub_df = setup_df[setup_df["trial_id"] == trial_id]
                 y = np.array(sub_df[plot_params.metric])
```

### Comparing `syne_tune-0.7.0/syne_tune/experiments/plotting.py` & `syne_tune-0.8.0/syne_tune/experiments/plotting.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,25 +6,23 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # or in the "license" file accompanying this file. This file is distributed
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
-from typing import Dict, Any, Optional, Tuple, Union, List, Iterable
+from typing import Dict, Any, Optional, Tuple, Union, List, Iterable, Callable
 from dataclasses import dataclass
 import logging
 import copy
 
 import numpy as np
 import pandas as pd
 
-from syne_tune.constants import (
-    ST_TUNER_TIME,
-)
+from syne_tune.constants import ST_TUNER_TIME
 from syne_tune.experiments.aggregate_results import aggregate_and_errors_over_time
 from syne_tune.experiments.results_utils import (
     MapMetadataToSetup,
     MapMetadataToSubplot,
     DateTimeBounds,
     create_index_for_result_files,
     load_results_dataframe_per_benchmark,
@@ -70,28 +68,33 @@
     :param ncols: Number of columns of subplot matrix
     :param titles: If given, these are titles for each column in the
         arrangement of subplots. If ``title_each_figure == True``, these
         are titles for each subplot. If ``titles`` is not given, then
         ``PlotParameters.title`` is printed on top of the leftmost column
     :param title_each_figure: See ``titles``, defaults to ``False``
     :param kwargs: Extra arguments for ``plt.subplots``, apart from "nrows" and "ncols"
-    :param legend_no: Numbers of subplots where legend is to be shown. Defaults
-        to ``[]`` (no legends shown)
+    :param legend_no: Subplot indices where legend is to be shown. Defaults
+        to ``[]`` (no legends shown). This is not relative to ``subplot_indices``
     :param xlims: If this is given, must be a list with one entry per subfigure.
         In this case, the global ``xlim`` is overwritten by
-        ``(0, xlims[subplot_no])``
+        ``(0, xlims[subplot_no])``. If ``subplot_indices`` is given, ``xlims``
+        must have the same length, and ``xlims[j]`` refers to subplot index
+        ``subplot_indices[j]`` then
+    :param subplot_indices: If this is given, we only plot subfigures with indices
+        in this list, and in this order. Otherwise, we plot subfigures 0, 1, 2, ...
     """
 
     nrows: int = None
     ncols: int = None
     titles: List[str] = None
     title_each_figure: bool = None
     kwargs: Dict[str, Any] = None
     legend_no: List[int] = None
     xlims: List[int] = None
+    subplot_indices: List[int] = None
 
     def merge_defaults(
         self, default_params: "SubplotParameters"
     ) -> "SubplotParameters":
         new_params = _impute_with_defaults(
             original=self,
             default=default_params,
@@ -99,14 +102,15 @@
                 "nrows",
                 "ncols",
                 "titles",
                 "title_each_figure",
                 "kwargs",
                 "legend_no",
                 "xlims",
+                "subplot_indices",
             ],
         )
         default_values = [
             ("nrows", None),
             ("ncols", None),
             ("title_each_figure", False),
         ]
@@ -199,15 +203,15 @@
     mode: str = None
     title: str = None
     xlabel: str = None
     ylabel: str = None
     xlim: Tuple[float, float] = None
     ylim: Tuple[float, float] = None
     metric_multiplier: float = None
-    convert_to_min: bool = True
+    convert_to_min: bool = None
     tick_params: Dict[str, Any] = None
     aggregate_mode: str = None
     dpi: int = None
     grid: bool = None
     subplots: SubplotParameters = None
     show_init_trials: ShowTrialParameters = None
 
@@ -220,25 +224,27 @@
                 "mode",
                 "title",
                 "xlabel",
                 "ylabel",
                 "xlim",
                 "ylim",
                 "metric_multiplier",
+                "convert_to_min",
                 "tick_params",
                 "aggregate_mode",
                 "dpi",
                 "grid",
             ],
         )
         default_values = [
             ("metric", None),
             ("mode", "min"),
             ("title", ""),
             ("metric_multiplier", 1),
+            ("convert_to_min", True),
             ("aggregate_mode", DEFAULT_AGGREGATE_MODE),
             ("dpi", 200),
             ("grid", False),
             ("xlabel", DEFAULT_XLABEL),
         ]
         _check_and_set_defaults(new_params, default_values)
         if self.subplots is None:
@@ -256,14 +262,77 @@
         else:
             new_params["show_init_trials"] = self.show_init_trials.merge_defaults(
                 default_params.show_init_trials
             )
         return PlotParameters(**new_params)
 
 
+DataFrameColumnGenerator = Callable[[pd.DataFrame], pd.Series]
+
+
+DataFrameGroups = Dict[Tuple[int, str], List[Tuple[str, pd.DataFrame]]]
+
+
+def group_results_dataframe(df: pd.DataFrame) -> DataFrameGroups:
+    result = dict()
+    for (subplot_no, setup_name, tuner_name), tuner_df in df.groupby(
+        ["subplot_no", "setup_name", "tuner_name"]
+    ):
+        key = (int(subplot_no), setup_name)
+        value = (tuner_name, tuner_df)
+        if key in result:
+            result[key].append(value)
+        else:
+            result[key] = [value]
+    return result
+
+
+def filter_final_row_per_trial(grouped_dfs: DataFrameGroups) -> DataFrameGroups:
+    """
+    We filter rows such that only one row per trial ID remains, namely the
+    one with the largest time stamp. This makes sense for single-fidelity
+    methods, where reports have still been done after every epoch.
+    """
+    logger.info("Filtering results down to one row per trial (final result)")
+    result = dict()
+    for key, tuner_dfs in grouped_dfs.items():
+        new_tuner_dfs = []
+        for tuner_name, tuner_df in tuner_dfs:
+            df_by_trial = tuner_df.groupby("trial_id")
+            max_time_in_trial = df_by_trial[ST_TUNER_TIME].transform(max)
+            max_time_in_trial_mask = max_time_in_trial == tuner_df[ST_TUNER_TIME]
+            new_tuner_dfs.append((tuner_name, tuner_df[max_time_in_trial_mask]))
+        result[key] = new_tuner_dfs
+    return result
+
+
+def enrich_results(
+    grouped_dfs: DataFrameGroups,
+    column_name: str,
+    dataframe_column_generator: Optional[DataFrameColumnGenerator],
+) -> DataFrameGroups:
+    if dataframe_column_generator is None:
+        return grouped_dfs
+    logger.info("Enriching results by additional column (dataframe_column_generator)")
+    result = dict()
+    for key, tuner_dfs in grouped_dfs.items():
+        new_tuner_dfs = []
+        for tuner_name, tuner_df in tuner_dfs:
+            assert column_name not in tuner_df.columns, (
+                f"New column to be appended to results dataframe: {column_name} is "
+                f"already a column: {tuner_df.columns}"
+            )
+            new_column = dataframe_column_generator(tuner_df)
+            new_tuner_dfs.append(
+                (tuner_name, tuner_df.assign(**{column_name: new_column}))
+            )
+        result[key] = new_tuner_dfs
+    return result
+
+
 class ComparativeResults:
     """
     This class loads, processes, and plots results of a comparative study,
     combining several experiments for different methods, seeds, and
     benchmarks (optional). Note that an experiment corresponds to one run
     of HPO, resulting in files :const:`~syne_tune.constants.ST_METADATA_FILENAME`
     for metadata, and :const:`~syne_tune.constants.ST_RESULTS_DATAFRAME_FILENAME`
@@ -424,134 +493,202 @@
         if subplots is not None:
             nrows = subplots.nrows
             ncols = subplots.ncols
         else:
             nrows = ncols = 1
         return nrows, ncols
 
-    def _aggregrate_results(
+    def _extract_result_curves_per_experiment(
         self,
         df: pd.DataFrame,
         plot_params: PlotParameters,
         extra_results_keys: Optional[List[str]],
+        one_trial_special: bool,
+        setup_name: str,
+        subplot_no: int,
+        extra_results: Dict[str, Any],
+        prev_max_rt: Optional[float],
+        xlim: Tuple[float, float],
+    ) -> Tuple[np.ndarray, np.ndarray]:
+        """
+        Extracts curve data ``(runtimes, values)`` which go into aggregation.
+
+        :param df: Results grouped w.r.t. subplot, setup, and experiment.
+        :param plot_params: Plot parameters
+        :param extra_results_keys: If given, info is written into ``extra_results``
+        :param one_trial_special: Is this special iteration for plotting results of single
+            trial?
+        :param setup_name:
+        :param subplot_no:
+        :param extra_results: Dictionary written to if ``extra_results_keys`` are given
+        :param prev_max_rt: Only if ``one_trial_special == True``. Largest value of
+            ``runtimes`` returned for the same experiment
+        :param xlim: Range for x axis
+        :return: ``(runtimes, values)``
+        """
+        metric = plot_params.metric
+        metric_multiplier = plot_params.metric_multiplier
+        show_init_trials = plot_params.show_init_trials
+        if one_trial_special:
+            # Filter down the dataframe
+            df = df[df["trial_id"] <= show_init_trials.trial_id]
+        if plot_params.mode == "max":
+            ys = metric_multiplier * np.array(df[metric].cummax())
+            if plot_params.convert_to_min:
+                ys = 1 - ys
+        else:
+            ys = metric_multiplier * np.array(df[metric].cummin())
+        rt = np.array(df[ST_TUNER_TIME])
+        if one_trial_special:
+            # Extend curve to the end, so it can be seen
+            rt = np.append(rt, prev_max_rt)
+            ys = np.append(ys, ys[-1])
+        if xlim is not None:
+            # Slice w.r.t. time. Doing this here, speeds up
+            # aggregation
+            ind = np.logical_and(rt >= xlim[0], rt <= xlim[1])
+            rt = rt[ind]
+            ys = ys[ind]
+        # Collect extra results
+        if extra_results_keys is not None and not one_trial_special:
+            if self._metadata_subplot_level:
+                key_sequence = [setup_name, subplot_no]
+            else:
+                key_sequence = [setup_name]
+            final_pos = df[ST_TUNER_TIME].idxmax()
+            final_row = dict(df.loc[final_pos])
+            for key in extra_results_keys:
+                _insert_into_nested_dict(
+                    dictionary=extra_results,
+                    key_sequence=key_sequence + [key],
+                    value=final_row[key],
+                )
+        return rt, ys
+
+    def _aggregate_results(
+        self,
+        grouped_dfs: DataFrameGroups,
+        plot_params: PlotParameters,
+        extra_results_keys: Optional[List[str]],
     ) -> Dict[str, Any]:
         subplots = plot_params.subplots
         subplot_xlims = None if subplots is None else subplots.xlims
         fig_shape = self._figure_shape(plot_params)
         num_subplots = fig_shape[0] * fig_shape[1]
-        metric = plot_params.metric
-        mode = plot_params.mode
-        metric_multiplier = plot_params.metric_multiplier
-        convert_to_min = plot_params.convert_to_min
         xlim = plot_params.xlim
         aggregate_mode = plot_params.aggregate_mode
         show_init_trials = plot_params.show_init_trials
         do_show_init_trials = show_init_trials is not None
         setup_names = self.setups
         extra_results = dict()
         if do_show_init_trials:
             # Put extra name at the end
             setup_names = setup_names + (show_init_trials.new_setup_name,)
 
         stats = [[None] * len(setup_names) for _ in range(num_subplots)]
-        for (subplot_no, setup_name), setup_df in df.groupby(
-            ["subplot_no", "setup_name"]
-        ):
+        for (subplot_no, setup_name), tuner_dfs in grouped_dfs.items():
             if subplot_xlims is not None:
                 xlim = (0, subplot_xlims[subplot_no])
             if do_show_init_trials and show_init_trials.setup_name == setup_name:
                 num_iter = 2
             else:
                 num_iter = 1
             max_rt = None
             # If this setup is named as ``show_init_trials.setup_name``, we need
-            # to go over the data 2x. The first iteration is as usual, the
+            # to go over the data twice. The first iteration is as usual, the
             # second extracts the information for the single trial and extends
             # the curve.
             for it in range(num_iter):
                 one_trial_special = it == 1
                 if one_trial_special:
-                    # Filter down the dataframe
-                    trial_id = show_init_trials.trial_id
-                    setup_df = setup_df[setup_df["trial_id"] <= trial_id]
                     new_setup_name = show_init_trials.new_setup_name
                     prev_max_rt = max_rt
                 else:
                     new_setup_name = setup_name
-                traj = []
-                runtime = []
-                trial_nums = []
-                tuner_names = []
+                    prev_max_rt = None
+                trajectories = []
+                runtimes = []
                 max_rt = []
-                for tuner_name, sub_df in setup_df.groupby("tuner_name"):
-                    tuner_names.append(tuner_name)
-                    if mode == "max":
-                        ys = metric_multiplier * np.array(sub_df[metric].cummax())
-                        if convert_to_min:
-                            ys = 1 - ys
-                    else:
-                        ys = metric_multiplier * np.array(sub_df[metric].cummin())
-                    rt = np.array(sub_df[ST_TUNER_TIME])
-                    if one_trial_special:
-                        # Hack to extend curve to the end, so it can be
-                        # seen
-                        pos = len(runtime)
-                        rt = np.append(rt, prev_max_rt[pos])
-                        ys = np.append(ys, ys[-1])
+                for tuner_pos, (_, tuner_df) in enumerate(tuner_dfs):
+                    rt, ys = self._extract_result_curves_per_experiment(
+                        df=tuner_df,
+                        plot_params=plot_params,
+                        extra_results_keys=extra_results_keys,
+                        one_trial_special=one_trial_special,
+                        setup_name=setup_name,
+                        subplot_no=subplot_no,
+                        extra_results=extra_results,
+                        prev_max_rt=prev_max_rt[tuner_pos]
+                        if one_trial_special
+                        else None,
+                        xlim=xlim,
+                    )
+                    trajectories.append(ys)
+                    runtimes.append(rt)
                     max_rt.append(rt[-1])
-                    if xlim is not None:
-                        # Slice w.r.t. time. Doing this here, speeds up
-                        # aggregation
-                        ind = np.logical_and(rt >= xlim[0], rt <= xlim[1])
-                        rt = rt[ind]
-                        ys = ys[ind]
-                    traj.append(ys)
-                    runtime.append(rt)
-                    trial_nums.append(len(sub_df.trial_id.unique()))
-                    # Collect extra results
-                    if extra_results_keys is not None and not one_trial_special:
-                        if self._metadata_subplot_level:
-                            key_sequence = [setup_name, subplot_no]
-                        else:
-                            key_sequence = [setup_name]
-                        final_pos = sub_df[ST_TUNER_TIME].idxmax()
-                        final_row = dict(sub_df.loc[final_pos])
-                        for key in extra_results_keys:
-                            _insert_into_nested_dict(
-                                dictionary=extra_results,
-                                key_sequence=key_sequence + [key],
-                                value=final_row[key],
-                            )
 
                 setup_id = setup_names.index(new_setup_name)
-                stats[subplot_no][setup_id] = aggregate_and_errors_over_time(
-                    errors=traj, runtimes=runtime, mode=aggregate_mode
-                )
+                if len(trajectories) > 1:
+                    stats[subplot_no][setup_id] = aggregate_and_errors_over_time(
+                        errors=trajectories, runtimes=runtimes, mode=aggregate_mode
+                    )
+                else:
+                    # If there is only a single seed, we plot a curve without
+                    # error bars
+                    stats[subplot_no][setup_id] = {
+                        "time": runtimes[0],
+                        "aggregate": trajectories[0],
+                    }
                 if not one_trial_special:
                     if subplots is not None:
                         msg = f"[{subplot_no}, {setup_name}]: "
                     else:
                         msg = f"[{setup_name}]: "
                     msg += f"max_rt = {np.mean(max_rt):.2f} (+- {np.std(max_rt):.2f})"
                     logger.info(msg)
-                    num_repeats = len(tuner_names)
+                    num_repeats = len(tuner_dfs)
                     if num_repeats != self.num_runs:
                         if subplots is not None:
                             part = f"subplot = {subplot_no}, "
                         else:
                             part = ""
+                        tuner_names = [name for name, _ in tuner_dfs]
                         logger.warning(
                             f"{part}setup = {setup_name} has {num_repeats} repeats "
                             f"instead of {self.num_runs}:\n{tuner_names}"
                         )
+
         result = {"stats": stats, "setup_names": setup_names}
         if extra_results_keys is not None:
             result["extra_results"] = extra_results
         return result
 
+    def _transform_and_aggregrate_results(
+        self,
+        df: pd.DataFrame,
+        plot_params: PlotParameters,
+        extra_results_keys: Optional[List[str]],
+        dataframe_column_generator: Optional[DataFrameColumnGenerator],
+        one_result_per_trial: bool,
+    ) -> Dict[str, Any]:
+        # Group results according to subplot, setup, and tuner (experiment)
+        grouped_dfs = group_results_dataframe(df)
+        # Filter down to one result per trial
+        if one_result_per_trial:
+            grouped_dfs = filter_final_row_per_trial(grouped_dfs)
+        # If ``dataframe_column_generator`` is given, an additional column is
+        # appended to the grouped dataframes
+        grouped_dfs = enrich_results(
+            grouped_dfs=grouped_dfs,
+            column_name=plot_params.metric,
+            dataframe_column_generator=dataframe_column_generator,
+        )
+        # Extract curves and aggregate them
+        return self._aggregate_results(grouped_dfs, plot_params, extra_results_keys)
+
     def _plot_figure(
         self,
         stats: List[List[Dict[str, np.ndarray]]],
         plot_params: PlotParameters,
         setup_names: List[str],
     ):
         subplots = plot_params.subplots
@@ -565,45 +702,57 @@
                 ncols=ncols,
             )
             subplot_titles = subplots.titles
             legend_no = [] if subplots.legend_no is None else subplots.legend_no
             if not isinstance(legend_no, list):
                 legend_no = [legend_no]
             title_each_figure = subplots.title_each_figure
+            subplot_indices = (
+                list(range(len(stats)))
+                if subplots.subplot_indices is None
+                else subplots.subplot_indices
+            )
         else:
             subplot_xlims = None
             nrows = ncols = 1
             subplots_kwargs = dict(nrows=nrows, ncols=ncols)
             subplot_titles = None
             legend_no = [0]
             title_each_figure = False
+            subplot_indices = [0]
         if subplot_titles is None:
             subplot_titles = [plot_params.title] + ["" * (ncols - 1)]
         ylim = plot_params.ylim
         xlim = plot_params.xlim  # Can be overwritten by ``subplot_xlims``
         xlabel = plot_params.xlabel
         ylabel = plot_params.ylabel
         tick_params = plot_params.tick_params
 
         plt.figure(dpi=plot_params.dpi)
         figsize = (5 * ncols, 4 * nrows)
         fig, axs = plt.subplots(**subplots_kwargs, squeeze=False, figsize=figsize)
-        for subplot_no, stats_subplot in enumerate(stats):
+        for subplot_no, subplot_index in enumerate(subplot_indices):
+            stats_subplot = stats[subplot_index]
             row = subplot_no % nrows
             col = subplot_no // nrows
             ax = axs[row, col]
             # Plot curves in the order of ``setups``. Not all setups may feature in
             # each of the subplots
             for i, (curves, setup_name) in enumerate(zip(stats_subplot, setup_names)):
                 if curves is not None:
                     color = f"C{i}"
                     x = curves["time"]
                     ax.plot(x, curves["aggregate"], color=color, label=setup_name)
-                    ax.plot(x, curves["lower"], color=color, alpha=0.4, linestyle="--")
-                    ax.plot(x, curves["upper"], color=color, alpha=0.4, linestyle="--")
+                    if "lower" in curves:
+                        ax.plot(
+                            x, curves["lower"], color=color, alpha=0.4, linestyle="--"
+                        )
+                        ax.plot(
+                            x, curves["upper"], color=color, alpha=0.4, linestyle="--"
+                        )
             if subplot_xlims is not None:
                 xlim = (0, subplot_xlims[subplot_no])
             if xlim is not None:
                 ax.set_xlim(*xlim)
             if ylim is not None:
                 ax.set_ylim(*ylim)
             if xlabel is not None and row == nrows - 1:
@@ -615,26 +764,28 @@
             if subplot_titles is not None:
                 if title_each_figure:
                     ax.set_title(subplot_titles[subplot_no])
                 elif row == 0:
                     ax.set_title(subplot_titles[col])
             if plot_params.grid:
                 ax.grid(True)
-            if subplot_no in legend_no:
+            if subplot_index in legend_no:
                 ax.legend()
         plt.show()
         return fig, axs
 
     def plot(
         self,
         benchmark_name: Optional[str] = None,
         plot_params: Optional[PlotParameters] = None,
         file_name: Optional[str] = None,
         extra_results_keys: Optional[List[str]] = None,
-    ) -> Optional[Dict[str, Any]]:
+        dataframe_column_generator: Optional[DataFrameColumnGenerator] = None,
+        one_result_per_trial: bool = False,
+    ) -> Dict[str, Any]:
         """
         Create comparative plot from results of all experiments collected at
         construction, for benchmark ``benchmark_name`` (if there is a single
         benchmark only, this need not be given).
 
         If ``plot_params.show_init_trials`` is given, the best metric value
         curve for the data from trials ``<=  plot_params.show_init_trials.trial_id``
@@ -651,38 +802,56 @@
         dataframe. For each setup and seed, we collect the values for the
         largest time stamp. We return a nested dictionary ``extra_results``, so
         that ``extra_results[setup_name][key]`` contains values (over seeds),
         where ``key`` is in ``extra_results_keys``. If ``metadata_subplot_level``
         is ``True`` and ``metadata_to_subplot`` is given, the structure is
         ``extra_results[setup_name][subplot_no][key]``.
 
+        If ``dataframe_column_generator`` is given, it maps a result dataframe
+        for a single experiment to a new column named ``plot_params.metric``.
+        This is applied before computing cumulative maximum or minimum and
+        aggregation over seeds. This way, we can plot derived metrics which are
+        not contained in the results as columns. Note that the transformed
+        dataframe is not retained.
+
         :param benchmark_name: Name of benchmark for which to plot results.
             Not needed if there is only one benchmark
         :param plot_params: Parameters controlling the plot. Values provided
             here overwrite values provided at construction.
         :param file_name: If given, the figure is stored in a file of this name
         :param extra_results_keys: See above, optional
-        :return: ``extra_results`` if ``extra_results_keys`` is given, otherwise
-            ``None``
+        :param dataframe_column_generator: See above, optional
+        :param one_result_per_trial: If ``True``, results for each experiment
+            are filtered down to one row per trial (the one with the largest
+            time stamp). This is useful for results from a single-fidelity
+            method, where the training script reported results after every
+            epoch.
+        :return: Dictionary with "fig", "axs" (for further processing). If
+            ``extra_results_keys``, "extra_results" entry as stated above
         """
         benchmark_name = self._check_benchmark_name(benchmark_name)
         if plot_params is None:
             plot_params = PlotParameters()
         plot_params = plot_params.merge_defaults(self._default_plot_params)
         logger.info(f"Load results for benchmark {benchmark_name}")
         results_df = load_results_dataframe_per_benchmark(
             self._reverse_index[benchmark_name]
         )
         logger.info("Aggregate results")
-        result = self._aggregrate_results(
+        aggregate_result = self._transform_and_aggregrate_results(
             df=results_df,
             plot_params=plot_params,
             extra_results_keys=extra_results_keys,
+            dataframe_column_generator=dataframe_column_generator,
+            one_result_per_trial=one_result_per_trial,
         )
         fig, axs = self._plot_figure(
-            stats=result["stats"],
+            stats=aggregate_result["stats"],
             plot_params=plot_params,
-            setup_names=result["setup_names"],
+            setup_names=aggregate_result["setup_names"],
         )
         if file_name is not None:
             fig.savefig(file_name, dpi=plot_params.dpi)
-        return None if extra_results_keys is None else result["extra_results"]
+        results = {"fig": fig, "axs": axs}
+        if extra_results_keys is not None:
+            results["extra_results"] = aggregate_result["extra_results"]
+        return results
```

### Comparing `syne_tune-0.7.0/syne_tune/experiments/results_utils.py` & `syne_tune-0.8.0/syne_tune/experiments/results_utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/num_gpu.py` & `syne_tune-0.8.0/syne_tune/num_gpu.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/__init__.py` & `syne_tune-0.8.0/syne_tune/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/baselines.py` & `syne_tune-0.8.0/syne_tune/optimizer/baselines.py`

 * *Files 2% similar despite different names*

```diff
@@ -552,15 +552,15 @@
             resource_attr=resource_attr,
             **kwargs,
         )
 
 
 def _create_searcher_kwargs(
     config_space: Dict[str, Any],
-    metric: str,
+    metric: Union[str, List[str]],
     random_seed: Optional[int],
     kwargs: Dict[str, Any],
 ) -> Dict[str, Any]:
     searcher_kwargs = dict(
         config_space=config_space,
         metric=metric,
         points_to_evaluate=kwargs.get("points_to_evaluate"),
@@ -758,26 +758,25 @@
         metric: List[str],
         mode: Union[List[str], str] = "min",
         population_size: int = 100,
         sample_size: int = 10,
         random_seed: Optional[int] = None,
         **kwargs,
     ):
+        searcher_kwargs = _create_searcher_kwargs(
+            config_space, metric, random_seed, kwargs
+        )
+        searcher_kwargs["mode"] = mode
+        searcher_kwargs["population_size"] = population_size
+        searcher_kwargs["sample_size"] = sample_size
         super(MOREA, self).__init__(
             config_space=config_space,
             metric=metric,
             mode=mode,
-            searcher=MultiObjectiveRegularizedEvolution(
-                config_space=config_space,
-                metric=metric,
-                mode=mode,
-                population_size=population_size,
-                sample_size=sample_size,
-                random_seed=random_seed,
-            ),
+            searcher=MultiObjectiveRegularizedEvolution(**searcher_kwargs),
             random_seed=random_seed,
             **kwargs,
         )
 
 
 class NSGA2(FIFOScheduler):
     """
@@ -798,25 +797,24 @@
         config_space: Dict[str, Any],
         metric: List[str],
         mode: Union[List[str], str] = "min",
         population_size: int = 20,
         random_seed: Optional[int] = None,
         **kwargs,
     ):
+        searcher_kwargs = _create_searcher_kwargs(
+            config_space, metric, random_seed, kwargs
+        )
+        searcher_kwargs["mode"] = mode
+        searcher_kwargs["population_size"] = population_size
         super(NSGA2, self).__init__(
             config_space=config_space,
             metric=metric,
             mode=mode,
-            searcher=NSGA2Searcher(
-                config_space=config_space,
-                metric=metric,
-                mode=mode,
-                population_size=population_size,
-                random_seed=random_seed,
-            ),
+            searcher=NSGA2Searcher(**searcher_kwargs),
             random_seed=random_seed,
             **kwargs,
         )
 
 
 class ConstrainedBayesianOptimization(FIFOScheduler):
     """Constrained Bayesian Optimization.
@@ -996,14 +994,96 @@
             config_space=config_space,
             metric=metric,
             searcher=searcher_name,
             **kwargs,
         )
 
 
+class CQR(FIFOScheduler):
+    """
+    Single-fidelity Conformal Quantile Regression approach proposed in:
+        | Optimizing Hyperparameters with Conformal Quantile Regression.
+        | David Salinas, Jacek Golebiowski, Aaron Klein, Matthias Seeger, Cedric Archambeau.
+        | ICML 2023.
+    The method predict quantile performance with gradient boosted trees and calibrate prediction with conformal
+    predictions.
+    """
+
+    def __init__(
+        self,
+        config_space: Dict[str, Any],
+        metric: str,
+        mode: str = "min",
+        random_seed: Optional[int] = None,
+        **kwargs,
+    ):
+        try:
+            from syne_tune.optimizer.schedulers.searchers.conformal.surrogate_searcher import (
+                SurrogateSearcher,
+            )
+        except ImportError:
+            logging.info(try_import_blackbox_repository_message())
+            raise
+
+        searcher_kwargs = _create_searcher_kwargs(
+            config_space, metric, random_seed, kwargs
+        )
+        searcher_kwargs["mode"] = mode
+        super(CQR, self).__init__(
+            config_space=config_space,
+            metric=metric,
+            mode=mode,
+            searcher=SurrogateSearcher(**searcher_kwargs),
+            random_seed=random_seed,
+            **kwargs,
+        )
+
+
+class ASHACQR(HyperbandScheduler):
+    """
+    Multi-fidelity Conformal Quantile Regression approach proposed in:
+        | Optimizing Hyperparameters with Conformal Quantile Regression.
+        | David Salinas, Jacek Golebiowski, Aaron Klein, Matthias Seeger, Cedric Archambeau.
+        | ICML 2023.
+    The method predict quantile performance with gradient boosted trees and calibrate prediction with conformal
+    predictions.
+    """
+
+    def __init__(
+        self,
+        config_space: Dict[str, Any],
+        metric: str,
+        resource_attr: str,
+        mode: str = "min",
+        random_seed: Optional[int] = None,
+        **kwargs,
+    ):
+        try:
+            from syne_tune.optimizer.schedulers.searchers.conformal.surrogate_searcher import (
+                SurrogateSearcher,
+            )
+        except ImportError:
+            logging.info(try_import_blackbox_repository_message())
+            raise
+
+        searcher_kwargs = _create_searcher_kwargs(
+            config_space, metric, random_seed, kwargs
+        )
+        searcher_kwargs["mode"] = mode
+        super(ASHACQR, self).__init__(
+            config_space=config_space,
+            metric=metric,
+            mode=mode,
+            searcher=SurrogateSearcher(**searcher_kwargs),
+            resource_attr=resource_attr,
+            random_seed=random_seed,
+            **kwargs,
+        )
+
+
 # Dictionary that allows to also list baselines who don't need a wrapper class
 # such as :class:`PopulationBasedTraining`
 baselines_dict = {
     "Random Search": RandomSearch,
     "Grid Search": GridSearch,
     "Bayesian Optimization": BayesianOptimization,
     "ASHA": ASHA,
@@ -1016,8 +1096,10 @@
     "SyncHyperband": SyncHyperband,
     "SyncBOHB": SyncBOHB,
     "DEHB": DEHB,
     "SyncMOBSTER": SyncMOBSTER,
     "ConstrainedBayesianOptimization": ConstrainedBayesianOptimization,
     "ZeroShotTransfer": ZeroShotTransfer,
     "ASHACTS": ASHACTS,
+    "CQR": CQR,
+    "ASHACQR": ASHACQR,
 }
```

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/scheduler.py` & `syne_tune-0.8.0/syne_tune/optimizer/scheduler.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/__init__.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/fifo.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/fifo.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/hyperband.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/hyperband.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/hyperband_checkpoint_removal.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/hyperband_checkpoint_removal.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/hyperband_cost_promotion.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/hyperband_cost_promotion.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         was_promoted: bool = False,
     ):
         super().__init__(trial_id, metric_val, was_promoted)
         self.cost_val = cost_val
 
 
 class CostPromotionRungSystem(PromotionRungSystem):
-    """
+    r"""
     Cost-aware extension of promotion-based asynchronous Hyperband (ASHA).
 
     This code is equivalent with base
     :class:`~syne_tune.optimizer.schedulers.hyperband_promotion.PromotionRungSystem`,
     except the "promotable" condition in :meth:`_find_promotable_trial` is
     replaced.
```

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/hyperband_pasha.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/hyperband_pasha.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/hyperband_promotion.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/hyperband_promotion.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/hyperband_rush.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/hyperband_rush.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/hyperband_stopping.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/hyperband_stopping.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/median_stopping_rule.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/median_stopping_rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 from syne_tune.backend.trial_status import Trial
 from syne_tune.optimizer.scheduler import (
     TrialScheduler,
     SchedulerDecision,
     TrialSuggestion,
 )
 
+logger = logging.getLogger(__name__)
+
 
 class MedianStoppingRule(TrialScheduler):
     """
     Applies median stopping rule in top of an existing scheduler.
 
     * If result at time-step ranks less than the cutoff of other results observed
       at this time-step, the trial is interrupted and otherwise, the wrapped
@@ -106,15 +108,15 @@
 
         if (
             self.grace_condition(time_step=time_step)
             or normalized_rank <= self.rank_cutoff
         ):
             return self.scheduler.on_trial_result(trial=trial, result=result)
         else:
-            logging.info(
+            logger.info(
                 f"see new results {new_metric} at time-step {time_step} for trial {trial.trial_id}"
                 f" with rank {int(normalized_rank * 100)}%, "
                 f"stopping it as it does not rank on the top {int(self.rank_cutoff * 100)}%"
             )
             return SchedulerDecision.STOP
 
     def grace_condition(self, time_step: float) -> bool:
```

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/multi_fidelity.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/multiobjective/__init__.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/multiobjective/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/multiobjective/linear_scalarizer.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/multiobjective/linear_scalarizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,27 +34,30 @@
     https://stackoverflow.com/questions/3844801/check-if-all-elements-in-a-list-are-identical
     """
     g = groupby(iterable)
     return next(g, True) and not next(g, False)
 
 
 class LinearScalarizedScheduler(TrialScheduler):
-    """Scheduler with a Linear Scalarization of multiple objectives.
-    This method optimizes a single objective equal to the linear scalarization of given two objectives.
-    The scalarized single objective is named: 'scalarized_<metric1>_<metric2>_..._<metricN>'
+    """Scheduler with linear scalarization of multiple objectives
 
+    This method optimizes a single objective equal to the linear scalarization
+    of given two objectives. The scalarized single objective is named:
+    ``"scalarized_<metric1>_<metric2>_..._<metricN>"``.
 
     :param base_scheduler_factory: Factory method for the single-objective scheduler
-        used on the scalarized objective. It will be initialized inside this Scheduler
-        If None, FIFOScheduler is used.
+        used on the scalarized objective. It will be initialized inside this scheduler.
+        Defaults to :class:`~syne_tune.optimizer.schedulers.FIFOScheduler`.
     :param config_space: Configuration space for evaluation function
     :param metric: Names of metrics to optimize
-    :param mode: Modes of metrics to optimize (min or max). All must be matching.
-    :param scalarization_weights: Weights used to scalarize objectives, if None an array of 1s is used
-    :param base_scheduler_kwargs: Additional arguments to base_scheduler beyond config_space, metric and mode
+    :param mode: Modes of metrics to optimize ("min" or "max"). All must be matching.
+    :param scalarization_weights: Weights used to scalarize objectives. Defaults to
+        an array of 1s
+    :param base_scheduler_kwargs: Additional arguments to ``base_scheduler_factory``
+        beyond ``config_space``, ``metric``, ``mode``
     """
 
     scalarization_weights: np.ndarray
     single_objective_metric: str
     base_scheduler: TrialScheduler
 
     def __init__(
```

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/multiobjective/moasha.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/multiobjective/moasha.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/multiobjective/multi_objective_regularized_evolution.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/multiobjective/multi_objective_regularized_evolution.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,35 +50,32 @@
         population_size: int = 100,
         sample_size: int = 10,
         multiobjective_priority: Optional[MOPriority] = None,
         **kwargs,
     ):
 
         if isinstance(mode, str):
-            modes = [mode] * len(metric)
-        else:
-            modes = mode
+            mode = [mode] * len(metric)
 
         super(MultiObjectiveRegularizedEvolution, self).__init__(
             config_space,
             metric=metric,
-            mode=modes,
             points_to_evaluate=points_to_evaluate,
             population_size=population_size,
             sample_size=sample_size,
+            mode=mode,
             **kwargs,
         )
 
         if multiobjective_priority is None:
             self._multiobjective_priority = NonDominatedPriority()
         else:
             self._multiobjective_priority = multiobjective_priority
 
     def _update(self, trial_id: str, config: dict, result: dict):
-
         results = {}
         for mode, metric in zip(self._mode, self._metric):
             value = result[metric]
             if mode == "max":
                 value *= -1
             results[metric] = value
```

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/multiobjective/multiobjective_priority.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/multiobjective/multiobjective_priority.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/multiobjective/non_dominated_priority.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/multiobjective/non_dominated_priority.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/multiobjective/nsga2_searcher.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/multiobjective/nsga2_searcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,14 +63,18 @@
             super().__init__(vars=vars, n_obj=n_obj, n_ieq_constr=0, **kwargs)
 
     return _MultiObjectiveMixedVariableProblem(
         n_obj=n_obj, config_space=config_space, **kwargs
     )
 
 
+# TODO:
+# - ``points_to_evaluate`` should be used, to initialize the population
+# - Do we want the first K configs to be selected at random, so the
+#   behavior is the same to other searchers?
 class NSGA2Searcher(StochasticSearcher):
     """
     This is a wrapper around the NSGA-2 [1] implementation of pymoo [2].
 
         | [1] K. Deb, A. Pratap, S. Agarwal, and T. Meyarivan.
         | A fast and elitist multiobjective genetic algorithm: nsga-II.
         | Trans. Evol. Comp, 6(2):182–197, April 2002.
```

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/multiobjective/utils.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/multiobjective/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,58 +6,92 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # or in the "license" file accompanying this file. This file is distributed
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
+from typing import List
 import numpy as np
 
 from syne_tune.try_import import try_import_moo_message
 
 try:
     from pymoo.indicators.hv import HV
 except ImportError:
     print(try_import_moo_message())
 
 
 EPSILON = 1e-6
 
 
+def default_reference_point(results_array: np.ndarray) -> np.ndarray:
+    return results_array.max(axis=0) * (1 + EPSILON) + EPSILON
+
+
 def hypervolume(
     results_array: np.ndarray,
     reference_point: np.ndarray = None,
 ) -> float:
     """
     Compute the hypervolume of all results based on reference points
 
-    :param results_df: Array with experiment results ordered by time with shape (npoints, ndimensions)
+    :param results_array: Array with experiment results ordered by time with
+        shape ``(npoints, ndimensions)``.
     :param reference_point: Reference points for hypervolume calculations.
-        If None, the maximum values of each dimension of results_array is used.
+        If ``None``, the maximum values of each dimension of results_array is
+        used.
+    :return Hypervolume indicator
     """
     if reference_point is None:
-        reference_point = results_array.max(axis=0) * (1 + EPSILON) + EPSILON
+        reference_point = default_reference_point(results_array)
     indicator_fn = HV(ref_point=reference_point)
     return indicator_fn(results_array)
 
 
+def linear_interpolate(hv_indicator: np.ndarray, indices: List[int]):
+    for first, last in zip(indices[:-1], indices[1:]):
+        num = last - first + 1
+        v_first = hv_indicator[first]
+        v_last = hv_indicator[last]
+        hv_indicator[first : (last + 1)] = np.linspace(v_first, v_last, num=num)
+
+
+# TODO: Use code for incremental hypervolume (adding one more point). Computation
+# here can be slow.
+# At least we could check for each new row if it is dominated by rows before. If
+# so, the cumulative indicator remains the same.
 def hypervolume_cumulative(
     results_array: np.ndarray,
     reference_point: np.ndarray = None,
+    increment: int = 1,
 ) -> np.ndarray:
     """
     Compute the cumulative hypervolume of all results based on reference points
     Returns an array with hypervolumes given by an increasing range of points.
-    ``return_array[idx] = hypervolume(results_array[0: idx])``
+    ``return_array[idx] = hypervolume(results_array[0 : (idx + 1)])``.
+
+    The current implementation is very slow, since the hypervolume index is not
+    computed incrementally. A solution for now is to use ``increment > 1``,
+    in which case the HV index is only computed every ``increment`` entry, and
+    linearly interpolated in between.
 
-    :param results_array: Array with experiment results ordered by time with shape (npoints, ndimensions).
+    :param results_array: Array with experiment results ordered by time with
+        shape ``(npoints, ndimensions)``.
     :param reference_point: Reference points for hypervolume calculations.
-        If None, the maximum values of each dimension of results_array is used.
-    :return: Cumulative hypervolume array with dimensions (npoints, )
+        If ``None``, the maximum values of each dimension of results_array is
+        used.
+    :return: Cumulative hypervolume array, shape ``(npoints,)``
     """
     if reference_point is None:
-        reference_point = results_array.max(axis=0) * (1 + EPSILON) + EPSILON
+        reference_point = default_reference_point(results_array)
     indicator_fn = HV(ref_point=reference_point)
     hypervolume_indicator = np.zeros(shape=len(results_array))
-    for idx in range(len(results_array)):
-        hypervolume_indicator[idx] = indicator_fn(results_array[0:idx])
+    sz = len(results_array)
+    indices = list(range(0, sz, increment))
+    if indices[-1] != sz - 1:
+        indices.append(sz - 1)
+    for idx in indices:
+        hypervolume_indicator[idx] = indicator_fn(results_array[0 : (idx + 1)])
+    if increment > 1:
+        linear_interpolate(hypervolume_indicator, indices)
     return hypervolume_indicator
```

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/neuralbands/__init__.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/neuralbands/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/neuralbands/networks.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/neuralbands/networks.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/neuralbands/neuralband.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/neuralbands/neuralband.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/neuralbands/neuralband_supplement.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/neuralbands/neuralband_supplement.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/pbt.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/pbt.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/random_seeds.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/random_seeds.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/ray_scheduler.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/ray_scheduler.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/remove_checkpoints.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/remove_checkpoints.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/scheduler_searcher.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/scheduler_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/__init__.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/__init__.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/__init__.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/common.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/common.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/config_ext.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/config_ext.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/tuning_job_state.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/datatypes/tuning_job_state.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/__init__.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/constants.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/constants.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/custom_op.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/custom_op.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/distribution.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/distribution.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon_blocks_helpers.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gluon_blocks_helpers.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_model.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_regression.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gp_regression.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gpr_mcmc.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/gpr_mcmc.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/__init__.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/gp_model.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/gp_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/likelihood.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/likelihood.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/posterior_state.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/posterior_state.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/utils.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/hypertune/utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/__init__.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/gpind_model.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/gpind_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/likelihood.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/likelihood.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,21 +68,21 @@
     :param resource_attr_range: :math:`(r_{min}, r_{max})`
     :param target_transform: Invertible transform of target values y to
         latent values z, which are then modelled as Gaussian. Shared across
         different :math:`r`. Defaults to the identity
     :param separate_noise_variances: See above. Defaults to ``False``
     :param initial_noise_variance: Initial value for noise variance(s).
         Defaults to
-        :const:syne_tune.optimizer.schedulers.searchers.bayesopt.gpautograd.constants.INITIAL_NOISE_VARIANCE``
+        :const:`~syne_tune.optimizer.schedulers.searchers.bayesopt.gpautograd.constants.INITIAL_NOISE_VARIANCE`
     :param initial_covariance_scale: Initial value for covariance scales.
         Defaults to
-        :const:syne_tune.optimizer.schedulers.searchers.bayesopt.gpautograd.constants.INITIAL_COVARIANCE_SCALE``
+        :const:`~syne_tune.optimizer.schedulers.searchers.bayesopt.gpautograd.constants.INITIAL_COVARIANCE_SCALE`
     :param encoding_type: Encoding used for noise variance(s) and covariance
         scales. Defaults to
-        :const:syne_tune.optimizer.schedulers.searchers.bayesopt.gpautograd.constants.DEFAULT_ENCODING``
+        :const:`~syne_tune.optimizer.schedulers.searchers.bayesopt.gpautograd.constants.DEFAULT_ENCODING`
     """
 
     def __init__(
         self,
         kernel: KernelFunction,
         mean: Dict[int, MeanFunction],
         resource_attr_range: Tuple[int, int],
```

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/posterior_state.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/independent/posterior_state.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/__init__.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/base.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,35 +129,32 @@
 
     def _inverse_bandwidths(self):
         return encode_unwrap_parameter(self.inverse_bandwidths_internal, self.encoding)
 
     def forward(self, X1, X2):
         """Computes matrix of squared distances
 
-        :param X1: input matrix, shape ``(n1,d)``
-        :param X2: input matrix, shape ``(n2,d)``
+        :param X1: input matrix, shape ``(n1, d)``
+        :param X2: input matrix, shape ``(n2, d)``
         """
         # In case inverse_bandwidths if of size (1, dimension), dimension>1,
         # ARD is handled by broadcasting
         inverse_bandwidths = anp.reshape(self._inverse_bandwidths(), (1, -1))
 
+        X1_scaled = anp.multiply(X1, inverse_bandwidths)
+        X1_squared_norm = anp.sum(anp.square(X1_scaled), axis=1)
         if X2 is X1:
-            X1_scaled = anp.multiply(X1, inverse_bandwidths)
             D = -2.0 * anp.dot(X1_scaled, anp.transpose(X1_scaled))
-            X1_squared_norm = anp.sum(anp.square(X1_scaled), axis=1)
-            D = D + anp.reshape(X1_squared_norm, (1, -1))
-            D = D + anp.reshape(X1_squared_norm, (-1, 1))
+            X2_squared_norm = X1_squared_norm
         else:
-            X1_scaled = anp.multiply(X1, inverse_bandwidths)
             X2_scaled = anp.multiply(X2, inverse_bandwidths)
-            X1_squared_norm = anp.sum(anp.square(X1_scaled), axis=1)
-            X2_squared_norm = anp.sum(anp.square(X2_scaled), axis=1)
             D = -2.0 * anp.matmul(X1_scaled, anp.transpose(X2_scaled))
-            D = D + anp.reshape(X1_squared_norm, (-1, 1))
-            D = D + anp.reshape(X2_squared_norm, (1, -1))
+            X2_squared_norm = anp.sum(anp.square(X2_scaled), axis=1)
+        D = D + anp.reshape(X1_squared_norm, (-1, 1))
+        D = D + anp.reshape(X2_squared_norm, (1, -1))
 
         return anp.abs(D)
 
     def get_params(self) -> Dict[str, Any]:
         """
         Parameter keys are "inv_bw<k> "if ``dimension > 1``, and "inv_bw" if
         ``dimension == 1``.
@@ -222,15 +219,15 @@
             )
             with self.name_scope():
                 self.covariance_scale_internal = register_parameter(
                     self.params, "covariance_scale", self.encoding
                 )
 
     @property
-    def ARD(self) -> float:
+    def ARD(self) -> bool:
         return self.squared_distance.ARD
 
     def _covariance_scale(self):
         if self.has_covariance_scale:
             return encode_unwrap_parameter(
                 self.covariance_scale_internal, self.encoding
             )
@@ -243,22 +240,20 @@
         :param X1: input matrix, shape ``(n1,d)``
         :param X2: input matrix, shape ``(n2,d)``
         """
         covariance_scale = self._covariance_scale()
         X1 = self._check_input_shape(X1)
         if X2 is not X1:
             X2 = self._check_input_shape(X2)
-        D = self.squared_distance(X1, X2)
+        D = 5.0 * self.squared_distance(X1, X2)
         # Using the plain np.sqrt is numerically unstable for D ~ 0
         # (non-differentiability)
         # that's why we add NUMERICAL_JITTER
-        B = anp.sqrt(5.0 * D + NUMERICAL_JITTER)
-        K = anp.multiply((1.0 + B + 5.0 / 3.0 * D) * anp.exp(-B), covariance_scale)
-
-        return K
+        B = anp.sqrt(D + NUMERICAL_JITTER)
+        return anp.multiply((1.0 + B + D / 3.0) * anp.exp(-B), covariance_scale)
 
     def diagonal(self, X):
         X = self._check_input_shape(X)
         covariance_scale = self._covariance_scale()
         covariance_scale_times_ones = anp.multiply(
             anp.ones((getval(X.shape[0]), 1)), covariance_scale
         )
```

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/cross_validation.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/cross_validation.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/exponential_decay.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/exponential_decay.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/fabolas.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/fabolas.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/freeze_thaw.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/freeze_thaw.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/product_kernel.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/product_kernel.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/range_kernel.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/kernel/range_kernel.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/__init__.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/freeze_thaw.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/freeze_thaw.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/gpiss_model.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/gpiss_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/issm.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/issm.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/likelihood.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/likelihood.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/model_params.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/model_params.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/posterior_state.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/learncurve/posterior_state.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/likelihood.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/likelihood.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/mean.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/mean.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/optimization_utils.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/optimization_utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_state.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_state.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_utils.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/posterior_utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/slice.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/slice.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/target_transform.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/target_transform.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/warping.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/gpautograd/warping.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/__init__.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/__init__.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/cost_model.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/cost_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 )
 
 __all__ = ["CostValue", "CostModel"]
 
 
 @dataclass
 class CostValue:
-    """
+    r"""
     Represents cost value :math:`(c_0(x), c_1(x))`:
 
     * :math:`c_0(x)`: Startup cost for evaluation at config :math:`x`
     * :math:`c_1(x)`: Cost per unit of resource :math:`r` at config :math:`x`
 
     Our assumption is that, under the model, an evaluation at :math:`x` until
     resource level :math:`r = 1, 2, 3, \dots` costs
```

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/linear_cost_model.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/linear_cost_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/sklearn_cost_model.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/sklearn_cost_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost_fifo_model.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost_fifo_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/estimator.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/estimator.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_mcmc_model.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_mcmc_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_model.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gp_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gpiss_model.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/gpiss_model.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/kernel_factory.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/kernel_factory.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,14 +25,31 @@
     Warping,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.gpautograd.mean import (
     MeanFunction,
 )
 
 
+SUPPORTED_BASE_MODELS = (
+    "matern52-ard",
+    "matern52-noard",
+)
+
+
+def base_kernel_factory(name: str, dimension: int, **kwargs) -> KernelFunction:
+    assert (
+        name in SUPPORTED_BASE_MODELS
+    ), f"name = {name} not supported. Choose from:\n{SUPPORTED_BASE_MODELS}"
+    return Matern52(
+        dimension=dimension,
+        ARD=name == "matern52-ard",
+        has_covariance_scale=kwargs.get("has_covariance_scale", True),
+    )
+
+
 SUPPORTED_RESOURCE_MODELS = (
     "exp-decay-sum",
     "exp-decay-combined",
     "exp-decay-delta1",
     "freeze-thaw",
     "matern52",
     "matern52-res-warp",
@@ -57,43 +74,43 @@
     :param kernel_x: Kernel function over configs ``x``
     :param mean_x: Mean function over configs ``x``
     :param kwargs: Extra arguments (optional)
     :return: ``(res_kernel, res_mean)``, both over ``(x, r)``
     """
     dim_x = kernel_x.dimension
     if name == "matern52":
-        res_kernel = Matern52(dimension=dim_x + 1, ARD=True)
+        res_kernel = base_kernel_factory("matern52-ard", dimension=dim_x + 1)
         if isinstance(kernel_x, WarpedKernel):
             res_kernel = WarpedKernel(kernel=res_kernel, warpings=kernel_x.warpings)
         res_mean = mean_x
     elif name == "matern52-res-warp":
         # Warping on resource dimension (last one)
         res_warping = Warping(dimension=dim_x + 1, coordinate_range=(dim_x, dim_x + 1))
         if isinstance(kernel_x, WarpedKernel):
             warpings = kernel_x.warpings + [res_warping]
         else:
             warpings = [res_warping]
         res_kernel = WarpedKernel(
-            kernel=Matern52(dimension=dim_x + 1, ARD=True),
+            kernel=base_kernel_factory("matern52-ard", dimension=dim_x + 1),
             warpings=warpings,
         )
         res_mean = mean_x
     elif name == "freeze-thaw":
         res_kernel = FreezeThawKernelFunction(kernel_x, mean_x)
         res_mean = FreezeThawMeanFunction(kernel=res_kernel)
     elif name == "cross-validation":
         # ``CrossValidationKernelFunction`` needs two kernels, one over the main
         # effect f(x), the other over the residuals g_k(x). We use ``kernel_x``,
         # ``mean_x`` for the former, and create a ``Matern52`` kernel (no ARD) here
         # for the latter
         num_folds = kwargs.get("num_folds")
         assert (
             num_folds is not None
-        ), f"Resource kenel '{name}' needs num_folds argument"
-        kernel_residual = Matern52(dimension=dim_x, ARD=False)
+        ), f"Resource kernel '{name}' needs num_folds argument"
+        kernel_residual = base_kernel_factory("matern52-noard", dimension=dim_x)
         res_kernel = CrossValidationKernelFunction(
             kernel_main=kernel_x,
             kernel_residual=kernel_residual,
             mean_main=mean_x,
             num_folds=num_folds,
         )
         res_mean = CrossValidationMeanFunction(kernel=res_kernel)
```

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc_impl.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc_impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     """
     Minus expected improvement acquisition function
     (minus because the convention is to always minimize acquisition functions)
     """
 
     def __init__(
         self,
-        predictor: OutputPredictor,
+        predictor: Predictor,
         active_metric: str = None,
         jitter: float = 0.01,
         debug_collect_stats: bool = False,
     ):
         assert isinstance(predictor, Predictor)
         super().__init__(predictor, active_metric)
         self.jitter = jitter
@@ -164,17 +164,15 @@
     Lower confidence bound (LCB) acquisition function:
 
     .. math::
 
        h(\mu, \sigma) = \mu - \kappa * \sigma
     """
 
-    def __init__(
-        self, predictor: OutputPredictor, kappa: float, active_metric: str = None
-    ):
+    def __init__(self, predictor: Predictor, kappa: float, active_metric: str = None):
         super().__init__(predictor, active_metric)
         assert isinstance(predictor, Predictor)
         assert kappa > 0, "kappa must be positive"
         self.kappa = kappa
 
     def _head_needs_current_best(self) -> bool:
         return False
```

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_base.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_base.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_skipopt.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_skipopt.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_transformer.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_transformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,26 +128,26 @@
             self._use_single_model = True
         if not self._use_single_model:
             assert isinstance(estimator, dict), (
                 f"{estimator} is not an instance of Estimator. "
                 f"It is assumed that we are in the multi-output case and that it "
                 f"must be a Dict. No other types are supported. "
             )
-            _assert_same_keys(estimator, skip_optimization)
             # Default: Always refit model parameters for each output model
             if skip_optimization is None:
                 skip_optimization = {
                     output_name: NeverSkipPredicate()
                     for output_name in estimator.keys()
                 }
             else:
                 assert isinstance(skip_optimization, Dict), (
                     f"{skip_optimization} must be a Dict, consistently "
                     f"with {estimator}."
                 )
+                _assert_same_keys(estimator, skip_optimization)
                 skip_optimization = {
                     output_name: skip_optimization[output_name]
                     if skip_optimization.get(output_name) is not None
                     else NeverSkipPredicate()
                     for output_name in estimator.keys()
                 }
             # debug_log is shared by all output models
```

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/sklearn_predictor.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/predictor.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,78 +6,52 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # or in the "license" file accompanying this file. This file is distributed
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
-from typing import Optional, List, Dict
+from typing import Tuple, Dict
 
 import numpy as np
 
-from syne_tune.optimizer.schedulers.searchers.bayesopt.datatypes.tuning_job_state import (
-    TuningJobState,
-)
-from syne_tune.optimizer.schedulers.searchers.bayesopt.models.model_base import (
-    BasePredictor,
-)
-from syne_tune.optimizer.schedulers.searchers.bayesopt.sklearn.predictor import (
-    SklearnPredictor,
-)
 
-
-class SklearnPredictorWrapper(BasePredictor):
-    """
-    Wrapper class for the sklearn estimators to be used with ContributedEstimatorWrapper
+class SKLearnPredictor:
     """
+    Base class for predictors generated by scikit-learn based estimators of
+    :class:`~syne_tune.optimizer.schedulers.searchers.bayesopt.sklearn.estimator.SKLearnEstimator`.
 
-    def __init__(
-        self,
-        contributed_predictor: SklearnPredictor,
-        state: TuningJobState,
-        active_metric: Optional[str] = None,
-    ):
-        super().__init__(state, active_metric)
-        self.contributed_predictor = contributed_predictor
+    This is only for predictors who return means and stddevs in :meth:`predict`.
+    """
 
-    def predict(self, inputs: np.ndarray) -> List[Dict[str, np.ndarray]]:
+    def predict(self, X: np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
         """
         Returns signals which are statistics of the predictive distribution at
-        input points ``inputs``. By default:
-
-        * "mean": Predictive means.
-        * "std": Predictive stddevs, shape ``(n,)``
-
-        This function relies on the assigned ContributedPredictor to execute the predictions
+        input points ``inputs``.
 
         :param inputs: Input points, shape ``(n, d)``
-        :return: List of ``dict`` with keys :meth:`keys_predict`, of length 1
+        :return: ``(means, stds)``, where predictive means ``means`` and
+            predictive stddevs ``stds`` have shape ``(n,)``
         """
-
-        mean, std = self.contributed_predictor.predict(inputs)
-        outputs = {"mean": mean}
-        if std is not None:
-            outputs["std"] = std
-        return [outputs]
+        raise NotImplementedError
 
     def backward_gradient(
-        self, input: np.ndarray, head_gradients: List[Dict[str, np.ndarray]]
-    ) -> List[np.ndarray]:
-        """
+        self, input: np.ndarray, head_gradients: Dict[str, np.ndarray]
+    ) -> np.ndarray:
+        r"""
+        Needs to be implemented only if gradient-based local optimization of
+        an acquisition function is supported.
+
         Computes the gradient :math:`\nabla f(x)` for an acquisition
         function :math:`f(x)`, where :math:`x` is a single input point. This
         is using reverse mode differentiation, the head gradients are passed
         by the acquisition function. The head gradients are
         :math:`\partial_k f`, where :math:`k` runs over the statistics
         returned by :meth:`predict` for the single input point :math:`x`.
         The shape of head gradients is the same as the shape of the
         statistics.
 
         :param input: Single input point :math:`x`, shape ``(d,)``
         :param head_gradients: See above
-        :return: Gradient :math:`\nabla f(x)` (one-length list)
+        :return: Gradient :math:`\nabla f(x)`
         """
-        return [
-            self.contributed_predictor.backward_gradient(
-                input=input, head_gradients=head_gradients
-            )
-        ]
+        raise NotImplementedError
```

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_multi_fidelity.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_single_fidelity.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_single_fidelity.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/__init__.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/estimator.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/estimator.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,38 +6,55 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # or in the "license" file accompanying this file. This file is distributed
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
+from typing import Dict, Any
 import numpy as np
 
 from syne_tune.optimizer.schedulers.searchers.bayesopt.sklearn.predictor import (
-    SklearnPredictor,
+    SKLearnPredictor,
 )
 
 
-class SklearnEstimator:
+class SKLearnEstimator:
     """
-    Base class for the sklearn Estimators
+    Base class scikit-learn based estimators, giving rise to surrogate models
+    for Bayesian optimization.
     """
 
     def fit(
         self, X: np.ndarray, y: np.ndarray, update_params: bool
-    ) -> SklearnPredictor:
+    ) -> SKLearnPredictor:
         """
-        Implements :meth:`fit_from_state`, given transformed data.
+        Implements :meth:`fit_from_state`, given transformed data. Here,
+        ``y`` is normalized (zero mean, unit variance) iff
+        ``normalize_targets == True``.
 
-        :param X: Training data in ndarray of shape (n_samples, n_features)
-        :param y: Target values in ndarray of shape (n_samples,)
+        :param X: Feature matrix, shape ``(n_samples, n_features)``
+        :param y: Target values, shape ``(n_samples,)``
         :param update_params: Should model (hyper)parameters be updated?
+            Ignored if estimator has no hyperparameters
         :return: Predictor, wrapping the posterior state
         """
-        raise NotImplementedError()
+        raise NotImplementedError
+
+    def get_params(self) -> Dict[str, Any]:
+        """
+        :return: Current model hyperparameters
+        """
+        return dict()  # Default (estimator has no hyperparameters)
+
+    def set_params(self, param_dict: Dict[str, Any]):
+        """
+        :param param_dict: New model hyperparameters
+        """
+        pass  # Default (estimator has no hyperparameters)
 
     @property
     def normalize_targets(self) -> bool:
         """
         :return: Should targets in ``state`` be normalized before calling
             :meth:`fit`?
         """
```

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/__init__.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/base_classes.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/base_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
 from typing import (
     List,
     Iterable,
     Tuple,
-    Type,
     Optional,
     Set,
     Dict,
     Union,
-    Any,
     Iterator,
+    Callable,
+    Any,
 )
 import numpy as np
 
 from syne_tune.optimizer.schedulers.searchers.bayesopt.datatypes.common import (
     INTERNAL_METRIC_NAME,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.datatypes.tuning_job_state import (
@@ -80,16 +80,15 @@
 
     def __init__(self, state: TuningJobState, active_metric: Optional[str] = None):
         self.state = state
         if active_metric is None:
             active_metric = INTERNAL_METRIC_NAME
         self.active_metric = active_metric
 
-    @staticmethod
-    def keys_predict() -> Set[str]:
+    def keys_predict(self) -> Set[str]:
         """Keys of signals returned by :meth:`predict`.
 
         Note: In order to work with :class:`AcquisitionFunction` implementations,
         the following signals are required:
 
         * "mean": Predictive mean
         * "std": Predictive standard deviation
@@ -100,15 +99,16 @@
 
     def predict(self, inputs: np.ndarray) -> List[Dict[str, np.ndarray]]:
         """
         Returns signals which are statistics of the predictive distribution at
         input points ``inputs``. By default:
 
         * "mean": Predictive means. If the model supports fantasizing with a
-            number ``nf`` of fantasies, this has shape ``(n, nf)``, otherwise ``(n,)``
+          number ``nf`` of fantasies, this has shape ``(n, nf)``, otherwise
+          ``(n,)``
         * "std": Predictive stddevs, shape ``(n,)``
 
         If the hyperparameters of the surrogate model are being optimized (e.g.,
         by empirical Bayes), the returned list has length 1. If its
         hyperparameters are averaged over by MCMC, the returned list has one
         entry per MCMC sample.
 
@@ -154,29 +154,29 @@
         :return: Incumbent, see above
         """
         raise NotImplementedError
 
     def backward_gradient(
         self, input: np.ndarray, head_gradients: List[Dict[str, np.ndarray]]
     ) -> List[np.ndarray]:
-        """
-        Computes the gradient :math:`\nabla f(x)` for an acquisition
+        r"""
+        Computes the gradient :math:`\nabla_x f(x)` for an acquisition
         function :math:`f(x)`, where :math:`x` is a single input point. This
         is using reverse mode differentiation, the head gradients are passed
         by the acquisition function. The head gradients are
         :math:`\partial_k f`, where :math:`k` runs over the statistics
         returned by :meth:`predict` for the single input point :math:`x`.
         The shape of head gradients is the same as the shape of the
         statistics.
 
         Lists have ``> 1`` entry if MCMC is used, otherwise they are all size 1.
 
         :param input: Single input point :math:`x`, shape ``(d,)``
         :param head_gradients: See above
-        :return: Gradient :math:`\nabla f(x)` (several if MCMC is used)
+        :return: Gradient :math:`\nabla_x f(x)` (several if MCMC is used)
         """
         raise NotImplementedError
 
 
 # Useful type that allows for a dictionary mapping each output name to a Predictor.
 # This is needed for multi-output BO methods such as constrained BO, where each output
 # is associated to a predictor. This type includes the Union with the standard
@@ -230,21 +230,21 @@
         :return: Acquisition function values, shape ``(n,)``
         """
         raise NotImplementedError
 
     def compute_acq_with_gradient(
         self, input: np.ndarray, predictor: Optional[OutputPredictor] = None
     ) -> Tuple[float, np.ndarray]:
-        """
+        r"""
         For a single input point :math:`x`, compute acquisition function value
-        :math:`f(x)` and gradient :math:`\nabla f(x)`.
+        :math:`f(x)` and gradient :math:`\nabla_x f(x)`.
 
         :param input: Single input point :math:`x`, shape ``(d,)``
         :param predictor: If given, overrides ``self.predictor``
-        :return: :math:`(f(x), \nabla f(x))`
+        :return: :math:`(f(x), \nabla_x f(x))`
         """
         raise NotImplementedError
 
     def score(
         self,
         candidates: Iterable[Configuration],
         predictor: Optional[OutputPredictor] = None,
@@ -256,30 +256,18 @@
         else:
             active_predictor = predictor
         hp_ranges = active_predictor.hp_ranges_for_prediction()
         inputs = hp_ranges.to_ndarray_matrix(candidates)
         return list(self.compute_acq(inputs, predictor=predictor))
 
 
-AcquisitionClassAndArgs = Union[
-    Type[AcquisitionFunction], Tuple[Type[AcquisitionFunction], Dict[str, Any]]
-]
-
-ScoringClassAndArgs = Union[
-    Type[ScoringFunction], Tuple[Type[ScoringFunction], Dict[str, Any]]
-]
+AcquisitionFunctionConstructor = Callable[[Any], AcquisitionFunction]
 
 
-def unwrap_acquisition_class_and_kwargs(
-    acquisition_class: AcquisitionClassAndArgs,
-) -> (Type[AcquisitionFunction], Dict[str, Any]):
-    if isinstance(acquisition_class, tuple):
-        return acquisition_class
-    else:
-        return acquisition_class, dict()
+ScoringFunctionConstructor = Callable[[Any], ScoringFunction]
 
 
 class LocalOptimizer:
     """
     Class that tries to find a local candidate with a better score, typically
     using a local optimization method such as L-BFGS. It would normally
     encapsulate an acquisition function and predictor.
@@ -295,15 +283,15 @@
     :param active_metric: Name of internal metric
     """
 
     def __init__(
         self,
         hp_ranges: HyperparameterRanges,
         predictor: OutputPredictor,
-        acquisition_class: AcquisitionClassAndArgs,
+        acquisition_class: AcquisitionFunctionConstructor,
         active_metric: Optional[str] = None,
     ):
         self.hp_ranges = hp_ranges
         self.predictor = predictor
         if active_metric is None:
             active_metric = INTERNAL_METRIC_NAME
         if isinstance(predictor, dict):
```

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm_components.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/bo_algorithm_components.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,17 +17,16 @@
 from numpy.random import RandomState
 
 from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.base_classes import (
     Predictor,
     ScoringFunction,
     LocalOptimizer,
     OutputPredictor,
-    AcquisitionClassAndArgs,
-    unwrap_acquisition_class_and_kwargs,
     CandidateGenerator,
+    AcquisitionFunctionConstructor,
 )
 from syne_tune.optimizer.schedulers.searchers.utils.common import Configuration
 from syne_tune.optimizer.schedulers.searchers.utils.exclusion_list import ExclusionList
 from syne_tune.optimizer.schedulers.searchers.utils.hp_ranges import (
     HyperparameterRanges,
 )
 
@@ -81,33 +80,28 @@
 
 
 class LBFGSOptimizeAcquisition(LocalOptimizer):
     def __init__(
         self,
         hp_ranges: HyperparameterRanges,
         predictor: OutputPredictor,
-        acquisition_class: AcquisitionClassAndArgs,
+        acquisition_class: AcquisitionFunctionConstructor,
         active_metric: str = None,
     ):
         super().__init__(hp_ranges, predictor, acquisition_class, active_metric)
         # Number criterion evaluations in last recent optimize call
         self.num_evaluations = None
 
     def optimize(
         self, candidate: Configuration, predictor: Optional[OutputPredictor] = None
     ) -> Configuration:
         # Before local minimization, the model for this state_id should have been fitted.
         if predictor is None:
             predictor = self.predictor
-        acquisition_class, acquisition_kwargs = unwrap_acquisition_class_and_kwargs(
-            self.acquisition_class
-        )
-        acquisition_function = acquisition_class(
-            predictor, self.active_metric, **acquisition_kwargs
-        )
+        acquisition_function = self.acquisition_class(predictor, self.active_metric)
 
         x0 = self.hp_ranges.to_ndarray(candidate)
         bounds = self.hp_ranges.get_ndarray_bounds()
         n_evaluations = [0]  # wrapped in list to allow access from function
 
         # unwrap 2d arrays
         def f_df(x):
@@ -136,14 +130,20 @@
                 bounds,
             )
             result = self.hp_ranges.from_ndarray(optimized_x.flatten())
             return result
 
 
 class NoOptimization(LocalOptimizer):
+    def __init__(self, *args, **kwargs):
+        # In case of no-optimization, no setup is needed.
+        # This is necessary if a single NoOptimization instance is to be used
+        # For multi-objective (multi-metric) optimization
+        pass
+
     def optimize(
         self, candidate: Configuration, predictor: Optional[Predictor] = None
     ) -> Configuration:
         return candidate
 
 
 MAX_RETRIES_CANDIDATES_EN_BULK = 20
```

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/defaults.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/tuning_algorithms/defaults.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/__init__.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/comparison_gpy.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/comparison_gpy.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/debug_log.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/debug_log.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/test_objects.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bayesopt/utils/test_objects.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bore/__init__.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bore/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bore/bore.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bore/bore.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bore/de.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bore/de.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bore/gp_classififer.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bore/gp_classififer.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bore/mlp_classififer.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bore/mlp_classififer.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bore/multi_fidelity_bore.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bore/multi_fidelity_bore.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/botorch/__init__.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/botorch/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/botorch/botorch_searcher.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/botorch/botorch_searcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -158,14 +158,20 @@
         )
 
         assert isinstance(
             scheduler, TrialSchedulerWithSearcher
         ), "This searcher requires TrialSchedulerWithSearcher scheduler"
         super().configure_scheduler(scheduler)
 
+    def _get_gp_bounds(self):
+        return Tensor(self._hp_ranges.get_ndarray_bounds()).T
+
+    def _config_from_ndarray(self, candidate) -> dict:
+        return self._hp_ranges.from_ndarray(candidate)
+
     def _sample_next_candidate(self) -> Optional[dict]:
         """
         :return: A next candidate to evaluate, if possible it is obtained by
             fitting a GP on past data and maximizing EI. If this fails because
             of numerical difficulties with non PSD matrices, then the candidate
             is sampled at random.
         """
@@ -208,33 +214,37 @@
 
             config = None
             if self._restrict_configurations is None:
                 # Continuous optimization of acquisition function only if
                 # ``restrict_configurations`` not used
                 candidate, acq_value = optimize_acqf(
                     acq,
-                    bounds=Tensor(self._hp_ranges.get_ndarray_bounds()).T,
+                    bounds=self._get_gp_bounds(),
                     q=1,
                     num_restarts=3,
                     raw_samples=100,
                 )
                 candidate = candidate.detach().numpy()[0]
-                config = self._hp_ranges.from_ndarray(candidate)
+                config = self._config_from_ndarray(candidate)
                 if self.should_not_suggest(config):
                     logger.warning(
                         "Optimization of the acquisition function yielded a config that was already seen."
                     )
                     config = None
             return self._sample_and_pick_acq_best(acq) if config is None else config
         except NotPSDError as _:
             logging.warning("Chlolesky inversion failed, sampling randomly.")
             return self._get_random_config()
         except ModelFittingError as _:
             logging.warning("Botorch was unable to fit the model, sampling randomly.")
             return self._get_random_config()
+        except:
+            # BoTorch can raise different errors, easier to not try to catch them individually
+            logging.warning("Botorch was unable to fit the model, sampling randomly.")
+            return self._get_random_config()
 
     def _make_gp(self, X_tensor: Tensor, Y_tensor: Tensor) -> SingleTaskGP:
         double_precision = False
         if double_precision:
             X_tensor = X_tensor.double()
             Y_tensor = Y_tensor.double()
```

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/bracket_distribution.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/bracket_distribution.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/constrained/__init__.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/constrained/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/constrained/constrained_gp_fifo_searcher.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/constrained/constrained_gp_fifo_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/cost_aware/__init__.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/cost_aware/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_fifo_searcher.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_fifo_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_multifidelity_searcher.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_multifidelity_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/dyhpo/__init__.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/dyhpo/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/dyhpo/dyhpo_searcher.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/dyhpo/dyhpo_searcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,18 +77,14 @@
 
     def __init__(self, config_space: Dict[str, Any], **kwargs):
         assert (
             INTERNAL_KEY not in config_space
         ), f"Key {INTERNAL_KEY} must not be used in config_space (reserved)"
         super().__init__(config_space, **kwargs)
         self._debug_log_copy = None
-        # DEBUG
-        # self.acquisition_class = (
-        #     self.acquisition_class, {"debug_collect_stats": True}
-        # )
 
     def _get_config_modelbased(
         self, exclusion_candidates: ExclusionList, **kwargs
     ) -> Optional[Configuration]:
         # Allows us to call :meth:`get_config` in
         # :meth:`score_paused_trials_and_new_configs`. If this returns the dummy
         # here, we are ready to score configs there, otherwise we are still in
```

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/dyhpo/hyperband_dyhpo.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/dyhpo/hyperband_dyhpo.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/gp_fifo_searcher.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/gp_fifo_searcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     check_and_merge_defaults,
 )
 
 logger = logging.getLogger(__name__)
 
 
 class GPFIFOSearcher(BayesianOptimizationSearcher):
-    """Gaussian process Bayesian optimization for FIFO scheduler
+    r"""Gaussian process Bayesian optimization for FIFO scheduler
 
     This searcher must be used with
     :class:`~syne_tune.optimizer.schedulers.FIFOScheduler`. It provides
     Bayesian optimization, based on a Gaussian process surrogate model.
 
     It is *not* recommended creating :class:`GPFIFOSearcher` searcher objects
     directly, but rather to create
@@ -114,14 +114,20 @@
     :param boxcox_transform: If ``True``, target values are transformed before
         being fitted with a Gaussian marginal likelihood. This is using the Box-Cox
         transform with a parameter :math:`\lambda`, which is learned alongside
         other parameters of the surrogate model. The transform is :math:`\log y`
         for :math:`\lambda = 0`, and :math:`y - 1` for :math:`\lambda = 1`. This
         option requires the targets to be positive. Defaults to ``False``.
     :type boxcox_transform: bool, optional
+    :param gp_base_kernel: Selects the covariance (or kernel) function to be
+        used. Supported choices are
+        :const:`~syne_tune.optimizer.schedulers.searchers.bayesopt.models.kernel_factory.SUPPORTED_BASE_MODELS`.
+        Defaults to "matern52-ard" (Matern 5/2 with automatic relevance
+        determination).
+    :type gp_base_kernel: str, optional
     :param initial_scoring: Scoring function to rank initial candidates
         (local optimization of EI is started from top scorer):
 
         * "thompson_indep": Independent Thompson sampling; randomized score,
           which can increase exploration
         * "acq_func": score is the same (EI) acquisition function which is
           used for local optimization afterwards
@@ -176,15 +182,15 @@
     :type opt_skip_period: int, optional
     :param allow_duplicates: If ``True``, :meth:`get_config` may return the same
         configuration more than once. Defaults to ``False``
     :type allow_duplicates: bool, optional
     :param restrict_configurations: If given, the searcher only suggests
         configurations from this list. This needs
         ``skip_local_optimization == True``. If ``allow_duplicates == False``,
-         entries are popped off this list once suggested.
+        entries are popped off this list once suggested.
     :type restrict_configurations: List[dict], optional
     :param map_reward: In the scheduler, the metric may be minimized or
         maximized, but internally, Bayesian optimization is minimizing
         the criterion. ``map_reward`` converts from metric to internal
         criterion:
 
         * "minus_x": ``criterion = -metric``
```

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/gp_multifidelity_searcher.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/gp_multifidelity_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/gp_searcher_factory.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/gp_searcher_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,26 +8,29 @@
 #
 # or in the "license" file accompanying this file. This file is distributed
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
 from typing import Set, Optional, Dict, Any
 import logging
+from functools import partial
 
 from syne_tune.optimizer.schedulers.searchers.gp_searcher_utils import (
     map_reward_const_minus_x,
     MapReward,
     DEFAULT_INITIAL_SCORING,
     SUPPORTED_INITIAL_SCORING,
     resource_for_acquisition_factory,
     SUPPORTED_RESOURCE_FOR_ACQUISITION,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.models.kernel_factory import (
-    resource_kernel_factory,
+    SUPPORTED_BASE_MODELS,
+    base_kernel_factory,
     SUPPORTED_RESOURCE_MODELS,
+    resource_kernel_factory,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.datatypes.config_ext import (
     ExtendedConfiguration,
 )
 from syne_tune.optimizer.schedulers.searchers.utils import (
     HyperparameterRanges,
 )
@@ -35,15 +38,14 @@
     OptimizationConfig,
     DEFAULT_OPTIMIZATION_CONFIG,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.gpautograd.gp_regression import (
     GaussianProcessRegression,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.gpautograd.kernel import (
-    Matern52,
     KernelFunction,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.gpautograd.warping import (
     kernel_with_warping,
     WarpedKernel,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.gpautograd.mean import (
@@ -160,17 +162,17 @@
             logger.warning(
                 "Cannot use input_warping=True together with transfer_learning_task_attr. Will use input_warping=False"
             )
         # Transfer learning: Specific base kernel
         kernel = create_base_gp_kernel_for_warmstarting(hp_ranges, **kwargs)
     else:
         has_covariance_scale = kwargs.get("has_covariance_scale", True)
-        kernel = Matern52(
+        kernel = base_kernel_factory(
+            name=kwargs["gp_base_kernel"],
             dimension=hp_ranges.ndarray_size,
-            ARD=True,
             has_covariance_scale=has_covariance_scale,
         )
         if input_warping:
             # Use input warping on all coordinates which do not belong to a
             # categorical hyperparameter
             kernel = kernel_with_warping(kernel, hp_ranges)
             if kwargs.get("debug_log", False) and isinstance(kernel, WarpedKernel):
@@ -721,15 +723,15 @@
         random_seed=random_seed,
         is_hyperband=False,
         **_kwargs,
     )["estimator"]
     # Sharing debug_log attribute across models
     estimator_cost._debug_log = estimator._debug_log
     exponent_cost = kwargs.get("exponent_cost", 1.0)
-    acquisition_class = (EIpuAcquisitionFunction, dict(exponent_cost=exponent_cost))
+    acquisition_class = partial(EIpuAcquisitionFunction, exponent_cost=exponent_cost)
     # The same skip_optimization strategy applies to both models
     skip_optimization_cost = skip_optimization
 
     output_estimator = {
         INTERNAL_METRIC_NAME: estimator,
         INTERNAL_COST_NAME: estimator_cost,
     }
@@ -784,15 +786,15 @@
     skip_optimization = result.pop("skip_optimization")
     # We need two model factories: one for active metric (estimator),
     # the other for cost metric (estimator_cost)
     estimator_cost = CostEstimator(
         model=kwargs["cost_model"], fixed_resource=fixed_resource, num_samples=1
     )
     exponent_cost = kwargs.get("exponent_cost", 1.0)
-    acquisition_class = (EIpuAcquisitionFunction, dict(exponent_cost=exponent_cost))
+    acquisition_class = partial(EIpuAcquisitionFunction, exponent_cost=exponent_cost)
     # The same skip_optimization strategy applies to both models
     skip_optimization_cost = skip_optimization
 
     output_estimator = {
         INTERNAL_METRIC_NAME: estimator,
         INTERNAL_COST_NAME: estimator_cost,
     }
@@ -842,15 +844,15 @@
     skip_optimization = result.pop("skip_optimization")
     # We need two model factories: one for active metric (estimator),
     # the other for cost metric (estimator_cost)
     estimator_cost = CostEstimator(
         model=kwargs["cost_model"], fixed_resource=kwargs["max_epochs"], num_samples=1
     )
     exponent_cost = kwargs.get("exponent_cost", 1.0)
-    acquisition_class = (EIpuAcquisitionFunction, dict(exponent_cost=exponent_cost))
+    acquisition_class = partial(EIpuAcquisitionFunction, exponent_cost=exponent_cost)
     # The same skip_optimization strategy applies to both models
     skip_optimization_cost = skip_optimization
 
     output_estimator = {
         INTERNAL_METRIC_NAME: estimator,
         INTERNAL_COST_NAME: estimator_cost,
     }
@@ -899,14 +901,15 @@
         "cost_attr": "elapsed_time",
         "normalize_targets": True,
         "no_fantasizing": False,
         "allow_duplicates": False,
         "input_warping": False,
         "boxcox_transform": False,
         "max_size_top_fraction": 0.25,
+        "gp_base_kernel": "matern52-ard",
     }
     if is_restrict_configs:
         default_options["initial_scoring"] = "acq_func"
         default_options["skip_local_optimization"] = True
     if is_hyperband:
         if is_hypertune:
             default_options["model"] = "gp_independent"
@@ -949,14 +952,15 @@
         "normalize_targets": Boolean(),
         "no_fantasizing": Boolean(),
         "allow_duplicates": Boolean(),
         "input_warping": Boolean(),
         "boxcox_transform": Boolean(),
         "max_size_data_for_model": IntegerOrNone(1, None),
         "max_size_top_fraction": Float(0.0, 1.0),
+        "gp_base_kernel": Categorical(choices=SUPPORTED_BASE_MODELS),
     }
 
     if is_hyperband:
         model_choices = ("gp_multitask", "gp_independent")
         if not is_hypertune:
             model_choices = model_choices + ("gp_issm", "gp_expdecay")
         constraints["model"] = Categorical(choices=model_choices)
```

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/gp_searcher_utils.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/gp_searcher_utils.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/hypertune/__init__.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/hypertune/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_bracket_distribution.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_bracket_distribution.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_searcher.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/kde/__init__.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/kde/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/kde/kde_searcher.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/kde/kde_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/kde/multi_fidelity_kde_searcher.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/kde/multi_fidelity_kde_searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/model_based_searcher.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/model_based_searcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,20 +38,19 @@
     ModelStateTransformer,
     StateForModelConverter,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.models.estimator import (
     OutputEstimator,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.base_classes import (
-    AcquisitionClassAndArgs,
     LocalOptimizer,
     ScoringFunction,
     OutputPredictor,
-    unwrap_acquisition_class_and_kwargs,
     CandidateGenerator,
+    AcquisitionFunctionConstructor,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.bo_algorithm import (
     BayesianOptimizationAlgorithm,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.tuning_algorithms.bo_algorithm_components import (
     NoOptimization,
     RandomStatefulCandidateGenerator,
@@ -113,15 +112,15 @@
     random searcher until meth:`_get_config_modelbased` is first called.
     """
 
     def _create_internal(
         self,
         hp_ranges: HyperparameterRanges,
         estimator: OutputEstimator,
-        acquisition_class: AcquisitionClassAndArgs,
+        acquisition_class: AcquisitionFunctionConstructor,
         map_reward: Optional[MapReward] = None,
         init_state: TuningJobState = None,
         local_minimizer_class: Type[LocalOptimizer] = None,
         skip_optimization: SkipOptimizationPredicate = None,
         num_initial_candidates: int = DEFAULT_NUM_INITIAL_CANDIDATES,
         num_initial_random_choices: int = DEFAULT_NUM_INITIAL_RANDOM_EVALUATIONS,
         initial_scoring: Optional[str] = None,
@@ -153,15 +152,19 @@
             self.local_minimizer_class = (
                 DEFAULT_LOCAL_OPTIMIZER_CLASS
                 if local_minimizer_class is None
                 else local_minimizer_class
             )
         self.acquisition_class = acquisition_class
         if isinstance(estimator, dict):
-            estimator_main = estimator[INTERNAL_METRIC_NAME]
+            # If no estimator for INTERNAL_METRIC_NAME can be found,
+            # use the debug log from a first metric
+            estimator_main = estimator.get(
+                INTERNAL_METRIC_NAME, next(iter(estimator.values()))
+            )
         else:
             estimator_main = estimator
         self._debug_log = estimator_main.debug_log
         self.initial_scoring = check_initial_candidates_scorer(initial_scoring)
         self.skip_local_optimization = skip_local_optimization
         # Create state transformer
         # Initial state is empty (note that the state is mutable).
@@ -482,30 +485,25 @@
             )
             self._random_searcher.set_random_state(self.random_state)
 
 
 def create_initial_candidates_scorer(
     initial_scoring: str,
     predictor: OutputPredictor,
-    acquisition_class: AcquisitionClassAndArgs,
+    acquisition_class: AcquisitionFunctionConstructor,
     random_state: np.random.RandomState,
     active_metric: str = INTERNAL_METRIC_NAME,
 ) -> ScoringFunction:
     if initial_scoring == "thompson_indep":
         if isinstance(predictor, dict):
             assert active_metric in predictor
             predictor = predictor[active_metric]
         return IndependentThompsonSampling(predictor, random_state=random_state)
     else:
-        acquisition_class, acquisition_kwargs = unwrap_acquisition_class_and_kwargs(
-            acquisition_class
-        )
-        return acquisition_class(
-            predictor, active_metric=active_metric, **acquisition_kwargs
-        )
+        return acquisition_class(predictor, active_metric=active_metric)
 
 
 class BayesianOptimizationSearcher(ModelBasedSearcher):
     """Common Code for searchers using Bayesian optimization
 
     We implement Bayesian optimization, based on a model factory which
     parameterizes the state transformer. This implementation works with
```

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/random_grid_searcher.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/random_grid_searcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     :param resource_attr: Optional. Key in ``result`` passed to :meth:`_update`
         for resource value (for multi-fidelity schedulers)
     """
 
     def __init__(
         self,
         config_space: Dict[str, Any],
-        metric: str,
+        metric: Union[List[str], str],
         points_to_evaluate: Optional[List[dict]] = None,
         debug_log: Union[bool, DebugLogPrinter] = False,
         resource_attr: Optional[str] = None,
         allow_duplicates: Optional[bool] = None,
         restrict_configurations: Optional[List[Dict[str, Any]]] = None,
         **kwargs,
     ):
@@ -122,20 +122,24 @@
             if cs_size is not None:
                 msg += f" Configuration space has size {cs_size}."
             logger.warning(msg)
         return new_config
 
     def _update(self, trial_id: str, config: Dict[str, Any], result: Dict[str, Any]):
         if self._debug_log is not None:
-            metric_val = result[self._metric]
             if self._resource_attr is not None:
                 # For HyperbandScheduler, also add the resource attribute
                 resource = int(result[self._resource_attr])
                 trial_id = trial_id + f":{resource}"
-            msg = f"Update for trial_id {trial_id}: metric = {metric_val:.3f}"
+            msg = f"Update for trial_id {trial_id}: "
+            if isinstance(self._metric, list):
+                parts = [f"{name} = {result[name]:.3f}" for name in self._metric]
+                msg += ",".join(parts)
+            else:
+                msg += f"{result[self._metric]:.3f}"
             logger.info(msg)
 
     def clone_from_state(self, state: Dict[str, Any]):
         new_searcher = RandomSearcher(
             self.config_space,
             metric=self._metric,
             points_to_evaluate=[],
```

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/regularized_evolution.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/regularized_evolution.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
 import copy
 import logging
 
 from collections import deque
-from typing import Optional, List, Dict, Any
+from typing import Optional, List, Dict, Any, Union
 from dataclasses import dataclass
 
 from syne_tune.optimizer.schedulers.searchers import StochasticSearcher
 from syne_tune.config_space import config_space_size, Domain
 from syne_tune.optimizer.schedulers.searchers.utils import make_hyperparameter_ranges
 from syne_tune.optimizer.schedulers.searchers.searcher_base import (
     sample_random_configuration,
@@ -57,28 +57,26 @@
     :param sample_size: Size of the candidate set to obtain a parent for the
         mutation, defaults to 10
     """
 
     def __init__(
         self,
         config_space,
-        metric: str,
+        metric: Union[List[str], str],
         points_to_evaluate: Optional[List[dict]] = None,
-        mode: str = "min",
         population_size: int = 100,
         sample_size: int = 10,
         **kwargs,
     ):
         super(RegularizedEvolution, self).__init__(
             config_space, metric, points_to_evaluate=points_to_evaluate, **kwargs
         )
         assert (
             config_space_size(config_space) != 1
-        ), "config_space has size 1, does not offer any diversity"
-        self.mode = mode
+        ), f"config_space = {config_space} has size 1, does not offer any diversity"
         self.population_size = population_size
         self.sample_size = sample_size
         self.population = deque()
         self.num_sample_try = 1000  # number of times allowed to sample a mutation
         self._hp_ranges = make_hyperparameter_ranges(self.config_space)
         allow_duplicates = kwargs.get("allow_duplicates")
         if allow_duplicates is not None and (not allow_duplicates):
@@ -137,15 +135,15 @@
             config = self._mutate_config(parent.config)
 
         return config
 
     def _update(self, trial_id: str, config: Dict[str, Any], result: Dict[str, Any]):
         score = result[self._metric]
 
-        if self.mode == "max":
+        if self._mode == "max":
             score *= -1
 
         # Add element to the population
         element = PopulationElement(result=result, score=score, config=config)
         self.population.append(element)
 
         # Remove the oldest element of the population.
```

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/searcher.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/searcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/searcher_base.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/searcher_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # or in the "license" file accompanying this file. This file is distributed
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
-from typing import Optional, Dict, Any, List
+from typing import Optional, Dict, Any, List, Union
 import logging
 import numpy as np
 
 from syne_tune.optimizer.schedulers.searchers import BaseSearcher
 from syne_tune.optimizer.schedulers.searchers.utils.exclusion_list import ExclusionList
 from syne_tune.optimizer.schedulers.searchers.utils import (
     HyperparameterRanges,
@@ -82,15 +82,15 @@
     :param random_seed: Used if ``random_seed_generator`` is not given.
     :type random_seed: int, optional
     """
 
     def __init__(
         self,
         config_space: Dict[str, Any],
-        metric: str,
+        metric: Union[List[str], str],
         points_to_evaluate: Optional[List[Dict[str, Any]]] = None,
         **kwargs,
     ):
         super().__init__(
             config_space,
             metric=metric,
             points_to_evaluate=points_to_evaluate,
@@ -204,15 +204,15 @@
     :param allow_duplicates: See above. Defaults to ``False``
     :param restrict_configurations: See above, optional
     """
 
     def __init__(
         self,
         config_space: Dict[str, Any],
-        metric: str,
+        metric: Union[List[str], str],
         points_to_evaluate: Optional[List[Dict[str, Any]]] = None,
         allow_duplicates: Optional[bool] = None,
         restrict_configurations: Optional[List[Dict[str, Any]]] = None,
         **kwargs,
     ):
         super().__init__(
             config_space, metric=metric, points_to_evaluate=points_to_evaluate, **kwargs
```

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/searcher_callback.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/searcher_callback.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/searcher_factory.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/searcher_factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,26 +30,28 @@
 
 
 SUPPORTED_SEARCHERS_FIFO = {
     "random",
     "grid",
     "kde",
     "bore",
+    "cqr",
     "botorch",
     "bayesopt",
     "bayesopt_constrained",
     "bayesopt_cost",
 }
 
 
 SUPPORTED_SEARCHERS_HYPERBAND = {
     "random",
     "grid",
     "kde",
     "bore",
+    "cqr",
     "bayesopt",
     "bayesopt_cost",
     "hypertune",
     "dyhpo",
 }
 
 
@@ -109,14 +111,23 @@
             raise
 
         if scheduler == "fifo":
             searcher_cls = Bore
         else:
             supported_schedulers = _OUR_MULTIFIDELITY_SCHEDULERS
             searcher_cls = MultiFidelityBore
+    elif searcher_name == "cqr":
+        try:
+            from syne_tune.optimizer.schedulers.searchers.conformal.surrogate_searcher import (
+                SurrogateSearcher,
+            )
+        except ImportError:
+            logger.info(try_import_bore_message())
+            raise
+        searcher_cls = SurrogateSearcher
     elif searcher_name == "botorch":
         try:
             from syne_tune.optimizer.schedulers.searchers.botorch import (
                 BoTorchSearcher,
             )
         except ImportError:
             logger.info(try_import_botorch_message())
```

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/utils/__init__.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/utils/common.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/utils/common.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/utils/default_arguments.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/utils/default_arguments.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/utils/exclusion_list.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/utils/exclusion_list.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_factory.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_factory.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_impl.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_impl.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/utils/scaling.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/utils/scaling.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/searchers/utils/warmstarting.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/utils/warmstarting.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,19 +19,21 @@
     HyperparameterRanges,
 )
 from syne_tune.optimizer.schedulers.searchers.utils.common import (
     Configuration,
     ConfigurationFilter,
 )
 from syne_tune.optimizer.schedulers.searchers.bayesopt.gpautograd.kernel import (
-    Matern52,
     ProductKernelFunction,
     KernelFunction,
     RangeKernelFunction,
 )
+from syne_tune.optimizer.schedulers.searchers.bayesopt.models.kernel_factory import (
+    base_kernel_factory,
+)
 from syne_tune.config_space import (
     Categorical,
     Ordinal,
     OrdinalNearestNeighbor,
 )
 
 
@@ -124,19 +126,19 @@
     assert task_attr is not None
     # Note: This attribute is the first in ``hp_ranges``, see
     # ``create_hp_ranges_for_warmstarting``
     assert hp_ranges.internal_keys[0] == task_attr  # Sanity check
     _, categ_dim = hp_ranges.encoded_ranges[task_attr]
     full_dim = hp_ranges.ndarray_size
     model = kwargs.get("transfer_learning_model", "matern52_product")
-    kernel2 = Matern52(full_dim - categ_dim, ARD=True)
+    kernel2 = base_kernel_factory("matern52-ard", dimension=full_dim - categ_dim)
     if model == "matern52_product":
         # Kernel is a product of Matern with single length scale on task_id
         # attribute, and Matern ARD kernel on the rest
-        kernel1 = Matern52(categ_dim, ARD=False)
+        kernel1 = base_kernel_factory("matern52-noard", dimension=categ_dim)
         return ProductKernelFunction(kernel1, kernel2)
     else:
         assert (
             model == "matern52_same"
         ), f"transfer_learning_model = {model} not supported"
         # Kernel is Matern ARD on rest, ignoring the task_id attribute
         return RangeKernelFunction(dimension=full_dim, kernel=kernel2, start=categ_dim)
```

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/synchronous/__init__.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/synchronous/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/synchronous/dehb.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/synchronous/dehb.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/synchronous/dehb_bracket.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/synchronous/dehb_bracket.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/synchronous/dehb_bracket_manager.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/synchronous/dehb_bracket_manager.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/synchronous/hyperband.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/synchronous/hyperband.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,15 +194,15 @@
     :param mode: Mode to use for the metric given, can be "min" (default) or
         "max"
     :type mode: str, optional
     :param points_to_evaluate: List of configurations to be evaluated
         initially (in that order). Each config in the list can be partially
         specified, or even be an empty dict. For each hyperparameter not
         specified, the default value is determined using a midpoint heuristic.
-        If None (default), this is mapped to ``[dict()]``, a single default config
+        If ``None`` (default), this is mapped to ``[dict()]``, a single default config
         determined by the midpoint heuristic. If ``[]`` (empty list), no initial
         configurations are specified.
     :type points_to_evaluate: ``List[dict]``, optional
     :param random_seed: Master random seed. Generators used in the scheduler
         or searcher are seeded using
         :class:`~syne_tune.optimizer.schedulers.random_seeds.RandomSeedGenerator`.
         If not given, the master random seed is drawn at random here.
@@ -255,15 +255,15 @@
         )
         self._create_internal_common(**kwargs)
         # Bracket manager
         self.bracket_manager = SynchronousHyperbandBracketManager(
             bracket_rungs,
             mode=self.mode,
         )
-        # Maps trial_id to tuples (bracket_id, slot_in_rung), as returned
+        # Maps trial_id to tuples ``(bracket_id, slot_in_rung)``, as returned
         # by ``bracket_manager.next_job``, and required by
         # ``bracket_manager.on_result``. Entries are removed once passed to
         # ``on_result``. Note that a trial_id can be associated with different
         # job descriptions in its lifetime
         self._trial_to_pending_slot = dict()
         # Maps trial_id (active) to config
         self._trial_to_config = dict()
@@ -327,15 +327,15 @@
         if suggestion is not None:
             assert trial_id not in self._trial_to_pending_slot, (
                 f"Trial for trial_id = {trial_id} is already registered as "
                 + "pending, cannot resume or start it"
             )
             self._trial_to_pending_slot[trial_id] = (bracket_id, slot_in_rung)
         else:
-            # Searcher failed to return a config for a new trial_id. We report
+            # Searcher failed to return a config for a new ``trial_id``. We report
             # the corresponding job as failed, so that in case the experiment
             # is continued, the bracket is not blocked with a slot which remains
             # pending forever
             logger.warning(
                 "Searcher failed to suggest a configuration for new trial "
                 f"{trial_id}. The corresponding rung slot is marked as failed."
             )
```

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket_manager.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/synchronous/hyperband_bracket_manager.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/synchronous/hyperband_impl.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/synchronous/hyperband_impl.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/synchronous/hyperband_rung_system.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/synchronous/hyperband_rung_system.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/transfer_learning/__init__.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/transfer_learning/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/transfer_learning/bounding_box.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/transfer_learning/bounding_box.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 from syne_tune.config_space import (
     Categorical,
     restrict_domain,
     choice,
     config_space_size,
 )
 
+logger = logging.getLogger(__name__)
+
 
 class BoundingBox(TransferLearningMixin, TrialScheduler):
     """
     Simple baseline that computes a bounding-box of the best candidate found in
     previous tasks to restrict the search space to only good candidates. The
     bounding-box is obtained by restricting to the min-max of the best numerical
     hyperparameters and restricting to the set of the best candidates on categorical
@@ -136,15 +138,15 @@
                         upper=hp_df.loc[:, name].max(),
                     )
                 else:
                     # no known way to compute bounding over non numerical domains such as functional
                     new_config_space[name] = domain
             else:
                 new_config_space[name] = domain
-        logging.info(
+        logger.info(
             f"new configuration space obtained after computing bounding-box: {new_config_space}"
         )
 
         return new_config_space
 
     def suggest(self, trial_id: int) -> Optional[TrialSuggestion]:
         return self.scheduler.suggest(trial_id)
```

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/__init__.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/normalization_transforms.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/normalization_transforms.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/quantile_based_searcher.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/transfer_learning/quantile_based/quantile_based_searcher.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # or in the "license" file accompanying this file. This file is distributed
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
 import logging
-from typing import Dict, Optional, Any
+from typing import Dict, Optional, Any, Tuple
 import numpy as np
 import xgboost
 from sklearn.model_selection import train_test_split
 
 from syne_tune.blackbox_repository.blackbox_surrogate import BlackboxSurrogate
 from syne_tune.optimizer.schedulers.searchers import StochasticSearcher
 
@@ -26,14 +26,16 @@
 )
 from syne_tune.optimizer.schedulers.transfer_learning.quantile_based.normalization_transforms import (
     from_string,
 )
 from syne_tune.config_space import Domain
 from syne_tune.util import catchtime
 
+logger = logging.getLogger(__name__)
+
 
 def extract_input_output(
     transfer_learning_evaluations, normalization: str, random_state
 ):
     X = pd.concat(
         [evals.hyperparameters for evals in transfer_learning_evaluations.values()],
         ignore_index=True,
@@ -88,29 +90,35 @@
     if mu_pred.ndim == 1:
         mu_pred = mu_pred.reshape(-1, 1)
     res = np.std(y - mu_pred, axis=0)
     return res.mean()
 
 
 def subsample(
-    X_train,
-    z_train,
-    max_samples: int = 10000,
+    X: pd.DataFrame,
+    y: np.array,
+    max_samples: Optional[int] = 10000,
     random_state: np.random.RandomState = None,
-):
-    assert len(X_train) == len(z_train)
-    X_train.reset_index(inplace=True)
-    if max_samples is not None and max_samples < len(X_train):
+) -> Tuple[pd.DataFrame, np.array]:
+    """
+    Subsample both X and y with `max_samples` elements. If `max_samples` is not set then X and y are returned as such
+    and if it is set, the index of X is reset.
+    :return: (X, y) with `max_samples` sampled elements.
+    """
+    assert len(X) == len(y)
+    if max_samples is not None and max_samples < len(X):
         if random_state is None:
-            random_indices = np.random.permutation(len(X_train))[:max_samples]
+            random_indices = np.random.permutation(len(X))[:max_samples]
         else:
-            random_indices = random_state.permutation(len(X_train))[:max_samples]
-        X_train = X_train.loc[random_indices]
-        z_train = z_train[random_indices]
-    return X_train, z_train
+            random_indices = random_state.permutation(len(X))[:max_samples]
+        # reset the index to be able to address elements between [0, len(X_train)-1]
+        X.reset_index(inplace=True, drop=True)
+        X = X.loc[random_indices]
+        y = y[random_indices]
+    return X, y
 
 
 class QuantileBasedSurrogateSearcher(StochasticSearcher):
     """
     Implements the transfer-learning method:
 
         | A Quantile-based Approach for Hyperparameter Transfer Learning.
@@ -157,16 +165,15 @@
             config_space=config_space,
             transfer_learning_evaluations=transfer_learning_evaluations,
             normalization=normalization,
             max_fit_samples=max_fit_samples,
             model=xgboost.XGBRegressor(),
             random_state=self.random_state,
         )
-        logging.info(f"residual train: {sigma_train}")
-        logging.info(f"residual val: {sigma_val}")
+        logger.info(f"residual train: {sigma_train}\nresidual val: {sigma_val}")
 
         with catchtime("time to predict"):
             # note the candidates could also be sampled every time, we cache them rather to save compute time.
             num_candidates = 100000
             self.X_candidates = pd.DataFrame(
                 [self._sample_random_config() for _ in range(num_candidates)]
             )
```

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/transfer_learning/rush.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/transfer_learning/rush.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/transfer_learning/zero_shot.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/transfer_learning/zero_shot.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/utils/__init__.py` & `syne_tune-0.8.0/syne_tune/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/utils/simple_profiler.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/utils/simple_profiler.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/optimizer/schedulers/utils/successive_halving.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/utils/successive_halving.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/remote/__init__.py` & `syne_tune-0.8.0/syne_tune/optimizer/schedulers/searchers/sklearn/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,7 +6,12 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # or in the "license" file accompanying this file. This file is distributed
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
+from syne_tune.optimizer.schedulers.searchers.sklearn.sklearn_surrogate_searcher import (  # noqa: F401
+    SKLearnSurrogateSearcher,
+)
+
+__all__ = ["SKLearnSurrogateSearcher"]
```

### Comparing `syne_tune-0.7.0/syne_tune/remote/estimators.py` & `syne_tune-0.8.0/syne_tune/remote/estimators.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/remote/remote_launcher.py` & `syne_tune-0.8.0/syne_tune/remote/remote_launcher.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/remote/remote_main.py` & `syne_tune-0.8.0/syne_tune/remote/remote_main.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 
 from syne_tune import Tuner
 from syne_tune.backend import LocalBackend
 from syne_tune.backend.sagemaker_backend.sagemaker_utils import (
     backend_path_not_synced_to_s3,
 )
 
+logger = logging.getLogger(__name__)
+
 
 def decode_bool(hp: str):
     # Sagemaker encodes hyperparameters in estimators as literals which are compatible with Python,
     # except for true and false that are respectively encoded as 'True' and 'False'.
     assert hp in ["True", "False"]
     return hp == "True"
 
@@ -43,15 +45,15 @@
     root = logging.getLogger()
     root.setLevel(args.log_level)
 
     args.store_logs = decode_bool(args.store_logs)
     args.no_tuner_logging = decode_bool(args.no_tuner_logging)
 
     tuner_path = Path(args.tuner_path)
-    logging.info(f"load tuner from path {args.tuner_path}")
+    logger.info(f"load tuner from path {args.tuner_path}")
     tuner = Tuner.load(tuner_path)
 
     # The output of the tuner (results, metadata, tuner state) is written into
     # SageMaker checkpoint directory, which is synced regularly by SageMaker so
     # that results are updated continuously
     tuner.tuner_path = Path("/opt/ml/checkpoints/")
 
@@ -69,9 +71,9 @@
         backend_path = str(backend_path_not_synced_to_s3())
     trial_backend.set_path(results_root=backend_path)
 
     # Run the tuner on the sagemaker instance. If the simulation backend is
     # used, this needs a specific callback
     if args.no_tuner_logging == "True":
         logging.getLogger("syne_tune.tuner").setLevel(logging.ERROR)
-    logging.info("starting remote tuning")
+    logger.info("starting remote tuning")
     tuner.run()
```

### Comparing `syne_tune-0.7.0/syne_tune/remote/remote_metrics_callback.py` & `syne_tune-0.8.0/syne_tune/remote/remote_metrics_callback.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/remote/scheduling.py` & `syne_tune-0.8.0/syne_tune/remote/scheduling.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 # on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing
 # permissions and limitations under the License.
 import functools
 import logging
 import time
 
+logger = logging.getLogger(__name__)
+
 
 def backoff(errorname: str, ntimes_resource_wait: int = 100, length2sleep: float = 600):
     """
     Decorator that back offs for a fixed about of s after a given error is detected
     """
 
     def errorcatch(some_function):
@@ -26,15 +28,15 @@
             for idx in range(ntimes_resource_wait):
                 try:
                     return some_function(*args, **kwargs)
                 except Exception as e:
                     if not e.__class__.__name__ == errorname:
                         raise (e)
 
-                logging.info(
+                logger.info(
                     f"{errorname} detected when calling <{some_function.__name__}>, waiting {length2sleep / 60} minutes before retring"
                 )
                 time.sleep(length2sleep)
                 continue
 
         return wrapper
```

### Comparing `syne_tune-0.7.0/syne_tune/report.py` & `syne_tune-0.8.0/syne_tune/report.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/results_callback.py` & `syne_tune-0.8.0/syne_tune/results_callback.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/stopping_criterion.py` & `syne_tune-0.8.0/syne_tune/stopping_criterion.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/try_import.py` & `syne_tune-0.8.0/syne_tune/try_import.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,14 +74,20 @@
 
 def try_import_visual_message() -> str:
     return _try_import_message(
         "Dependencies for visualization are not imported", tag="visual"
     )
 
 
+def try_import_sklearn_message() -> str:
+    return _try_import_message(
+        "Dependencies for scikit-learn are not imported", tag="sklearn"
+    )
+
+
 def try_import_backends_message() -> str:
     return _try_import_message(
         "LocalBackend / PythonBackend are not imported", tag=None
     )
 
 
 def _try_import_message(message_text: str, tag: Optional[str]) -> str:
```

### Comparing `syne_tune-0.7.0/syne_tune/tuner.py` & `syne_tune-0.8.0/syne_tune/tuner.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/tuner_callback.py` & `syne_tune-0.8.0/syne_tune/tuner_callback.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/tuning_status.py` & `syne_tune-0.8.0/syne_tune/tuning_status.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/util.py` & `syne_tune-0.8.0/syne_tune/util.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/utils/__init__.py` & `syne_tune-0.8.0/syne_tune/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/utils/checkpoint.py` & `syne_tune-0.8.0/syne_tune/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/utils/config_as_json.py` & `syne_tune-0.8.0/syne_tune/utils/config_as_json.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune/utils/parse_bool.py` & `syne_tune-0.8.0/syne_tune/utils/parse_bool.py`

 * *Files identical despite different names*

### Comparing `syne_tune-0.7.0/syne_tune.egg-info/PKG-INFO` & `syne_tune-0.8.0/syne_tune.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syne-tune
-Version: 0.7.0
+Version: 0.8.0
 Summary: Distributed Hyperparameter Optimization on SageMaker
 Author: AWS
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,14 +12,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: gpsearchers
 Provides-Extra: kde
 Provides-Extra: dev
 Provides-Extra: aws
 Provides-Extra: moo
 Provides-Extra: visual
+Provides-Extra: sklearn
 Provides-Extra: blackbox-repository
 Provides-Extra: benchmarks
 Provides-Extra: yahpo
 Provides-Extra: raytune
 Provides-Extra: botorch
 Provides-Extra: bore
 Provides-Extra: extra
@@ -31,26 +32,27 @@
 [![release](https://img.shields.io/github/v/release/awslabs/syne-tune)](https://pypi.org/project/syne-tune/)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Downloads](https://pepy.tech/badge/syne-tune/month)](https://pepy.tech/project/syne-tune)
 [![Documentation](https://readthedocs.org/projects/syne-tune/badge/?version=latest)](https://syne-tune.readthedocs.io)
 [![Python Version](https://img.shields.io/static/v1?label=python&message=3.7%20%7C%203.8%20%7C%203.9&color=blue?style=flat-square&logo=python)](https://pypi.org/project/syne-tune/)
 [![codecov.io](https://codecov.io/github/awslabs/syne-tune/branch/main/graphs/badge.svg)](https://app.codecov.io/gh/awslabs/syne-tune)
 
-![Alt Text](docs/source/synetune.gif)
+![Syne Tune](docs/source/synetune.gif)
 
-[Documentation](https://syne-tune.readthedocs.io/en/latest/index.html)
+**[Documentation](https://syne-tune.readthedocs.io/en/latest/index.html)** | **[Tutorials](https://syne-tune.readthedocs.io/en/latest/tutorials/basics/README.html)** | **[API Reference](https://syne-tune.readthedocs.io/en/latest/_apidoc/modules.html#)** | **[PyPI](https://pypi.org/project/syne-tune)** | **[Latest Blog Post](https://aws.amazon.com/blogs/machine-learning/hyperparameter-optimization-for-fine-tuning-pre-trained-transformer-models-from-hugging-face/)**
+
+Syne Tune provides state-of-the-art algorithms for hyperparameter optimization (HPO) with the following key features:
 
-This package provides state-of-the-art algorithms for hyperparameter optimization (HPO) with the following key features:
 * Wide coverage (>20) of different HPO methods, including:
-  * Asynchronous versions to maximize utilization and distributed versions (i.e., with multiple workers);
+  * Asynchronous and distributed tuning (i.e., with multiple workers);
   * Multi-fidelity methods supporting model-based decisions (BOHB and MOBSTER);
-  * Hyperparameter transfer learning to speed up (repeated) tuning jobs;
+  * Transfer learning to speed up (repeated) tuning jobs;
   * Multi-objective optimizers that can tune multiple objectives simultaneously (such as accuracy and latency).
-* HPO can be run in different environments (locally, AWS, simulation) by changing just one line of code.
-* Out-of-the-box tabulated benchmarks that allows you simulate results in seconds while preserving the real dynamics of asynchronous or synchronous HPO with any number of workers.
+* Run on different compute environments (locally, AWS, simulation) by changing just one line of code.
+* Out-of-the-box tabulated benchmarks allow you to simulate results in seconds while preserving the real dynamics of asynchronous or synchronous HPO with any number of workers.
 
 ## Installing
 
 To install Syne Tune from pip, you can simply do:
 
 ```bash
 pip install 'syne-tune[extra]'
@@ -100,15 +102,15 @@
     for step in range(args.epochs):
         time.sleep(0.1)
         dummy_score = 1.0 / (0.1 + args.width * step / 100) + args.height * 0.1
         # Feed the score back to Syne Tune.
         report(epoch=step + 1, mean_loss=dummy_score)
 ```
 
-Once you have a script reporting metric, you can launch a tuning as-follow:
+Once you have a training script reporting a metric, you can launch a tuning as follows:
 
 ```python
 # launch_height_simple.py
 from syne_tune import Tuner, StoppingCriterion
 from syne_tune.backend import LocalBackend
 from syne_tune.config_space import randint
 from syne_tune.optimizer.baselines import ASHA
@@ -169,21 +171,23 @@
 
 The searchers fall into four broad categories, **deterministic**, **random**, **evolutionary** and **model-based**. The random searchers sample candidate hyperparameter configurations uniformly at random, while the model-based searchers sample them non-uniformly at random, according to a model (e.g., Gaussian process, density ration estimator, etc.) and an acquisition function. The evolutionary searchers make use of an evolutionary algorithm.
 
 Syne Tune also supports [BoTorch](https://github.com/awslabs/syne-tune/blob/main/syne_tune/optimizer/schedulers/searchers/botorch/botorch_searcher.py) searchers.
 
 ## Supported multi-objective optimization methods
 
-Method | Reference | Searcher | Asynchronous? | Multi-fidelity? | Transfer?
-:--- | :---: | :---: | :---: | :---: | :---: 
-Constrained Bayesian Optimization | Gardner, et al. (2014) | model-based | yes | no | no
-MOASHA | Schmucker, et al. (2021) | random | yes | yes | no
-NSGA-2 | Deb, et al. (2002) | evolutionary | no | no | no
+Method |          Reference          |   Searcher   | Asynchronous? | Multi-fidelity? | Transfer?
+:--- |:---------------------------:|:------------:| :---: | :---: | :---: 
+Constrained Bayesian Optimization |   Gardner, et al. (2014)    | model-based  | yes | no | no
+MOASHA |  Schmucker, et al. (2021)   |    random    | yes | yes | no
+NSGA-2 |     Deb, et al. (2002)      | evolutionary | no | no | no
+Multi Objective Multi Surrogate (MSMOS) | Guerrero-Viu, et al. (2021) | model-based  | no | no | no
+MSMOS wihh random scalarization |    Paria, et al. (2018)     | model-based  | no | no | no
 
-HPO methods listed can be used in a multi-objective setting by scalarization or non-dominated sorting. See [multiobjective_priority.py](syne_tune/optimizers/schedulers/multiobjective/multiobjective_priority.py) for details.
+HPO methods listed can be used in a multi-objective setting by scalarization or non-dominated sorting. See [multiobjective_priority.py](syne_tune/optimizer/schedulers/multiobjective/multiobjective_priority.py) for details.
 
 ## Examples
 
 You will find many examples in the [examples/](examples/) folder illustrating
 different functionalities provided by Syne Tune. For example:
 * [launch_height_baselines.py](examples/launch_height_baselines.py):
   launches HPO locally, tuning a simple script 
@@ -197,17 +201,17 @@
   launches the HPO loop on SageMaker rather than a local machine, trial can be executed either
   the remote machine or distributed again as separate SageMaker training jobs. See 
   [launch_height_sagemaker_remote_launcher.py](examples/launch_height_sagemaker_remote_launcher.py)
   for remote launching with the help of RemoteTuner also discussed in one of the FAQs.
 * [launch_height_sagemaker.py](examples/launch_height_sagemaker.py):
   launches HPO on SageMaker to tune a SageMaker Pytorch estimator
 * [launch_bayesopt_constrained.py](examples/launch_bayesopt_constrained.py):
-  launches Bayesian contrained hyperparameter optimization
+  launches Bayesian constrained hyperparameter optimization
 * [launch_height_sagemaker_custom_image.py](examples/launch_height_sagemaker_custom_image.py):
-  launches HPO on SageMaker to tune a entry point with a custom docker image
+  launches HPO on SageMaker to tune an entry point with a custom docker image
 * [launch_plot_results.py](examples/launch_plot_results.py): shows how to plot
   results of a HPO experiment
 * [launch_tensorboard_example.py](examples/launch_tensorboard_example.py):
   shows how results can be visualized on the fly with TensorBoard
 * [launch_nasbench201_simulated.py](examples/launch_nasbench201_simulated.py):
   demonstrates simulation of experiments on a tabulated benchmark
 * [launch_fashionmnist.py](examples/launch_fashionmnist.py):
```

### Comparing `syne_tune-0.7.0/syne_tune.egg-info/SOURCES.txt` & `syne_tune-0.8.0/syne_tune.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,15 @@
 syne_tune/callbacks/hyperband_remove_checkpoints_callback.py
 syne_tune/callbacks/hyperband_remove_checkpoints_score.py
 syne_tune/callbacks/remove_checkpoints_callback.py
 syne_tune/callbacks/tensorboard_callback.py
 syne_tune/experiments/__init__.py
 syne_tune/experiments/aggregate_results.py
 syne_tune/experiments/experiment_result.py
+syne_tune/experiments/multiobjective.py
 syne_tune/experiments/plot_per_trial.py
 syne_tune/experiments/plotting.py
 syne_tune/experiments/results_utils.py
 syne_tune/optimizer/__init__.py
 syne_tune/optimizer/baselines.py
 syne_tune/optimizer/scheduler.py
 syne_tune/optimizer/schedulers/__init__.py
@@ -93,17 +94,19 @@
 syne_tune/optimizer/schedulers/ray_scheduler.py
 syne_tune/optimizer/schedulers/remove_checkpoints.py
 syne_tune/optimizer/schedulers/scheduler_searcher.py
 syne_tune/optimizer/schedulers/multiobjective/__init__.py
 syne_tune/optimizer/schedulers/multiobjective/linear_scalarizer.py
 syne_tune/optimizer/schedulers/multiobjective/moasha.py
 syne_tune/optimizer/schedulers/multiobjective/multi_objective_regularized_evolution.py
+syne_tune/optimizer/schedulers/multiobjective/multi_surrogate_multi_objective_searcher.py
 syne_tune/optimizer/schedulers/multiobjective/multiobjective_priority.py
 syne_tune/optimizer/schedulers/multiobjective/non_dominated_priority.py
 syne_tune/optimizer/schedulers/multiobjective/nsga2_searcher.py
+syne_tune/optimizer/schedulers/multiobjective/random_scalarization.py
 syne_tune/optimizer/schedulers/multiobjective/utils.py
 syne_tune/optimizer/schedulers/neuralbands/__init__.py
 syne_tune/optimizer/schedulers/neuralbands/networks.py
 syne_tune/optimizer/schedulers/neuralbands/neuralband.py
 syne_tune/optimizer/schedulers/neuralbands/neuralband_supplement.py
 syne_tune/optimizer/schedulers/searchers/__init__.py
 syne_tune/optimizer/schedulers/searchers/bracket_distribution.py
@@ -172,16 +175,15 @@
 syne_tune/optimizer/schedulers/searchers/bayesopt/models/gpiss_model.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/models/kernel_factory.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/models/meanstd_acqfunc_impl.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_base.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_skipopt.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/models/model_transformer.py
-syne_tune/optimizer/schedulers/searchers/bayesopt/models/sklearn_estimator.py
-syne_tune/optimizer/schedulers/searchers/bayesopt/models/sklearn_predictor.py
+syne_tune/optimizer/schedulers/searchers/bayesopt/models/sklearn_model.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_multi_fidelity.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/models/subsample_state_single_fidelity.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/__init__.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/cost_model.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/linear_cost_model.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/models/cost/sklearn_cost_model.py
 syne_tune/optimizer/schedulers/searchers/bayesopt/sklearn/__init__.py
@@ -200,28 +202,31 @@
 syne_tune/optimizer/schedulers/searchers/bore/bore.py
 syne_tune/optimizer/schedulers/searchers/bore/de.py
 syne_tune/optimizer/schedulers/searchers/bore/gp_classififer.py
 syne_tune/optimizer/schedulers/searchers/bore/mlp_classififer.py
 syne_tune/optimizer/schedulers/searchers/bore/multi_fidelity_bore.py
 syne_tune/optimizer/schedulers/searchers/botorch/__init__.py
 syne_tune/optimizer/schedulers/searchers/botorch/botorch_searcher.py
+syne_tune/optimizer/schedulers/searchers/botorch/botorch_transfer_searcher.py
 syne_tune/optimizer/schedulers/searchers/constrained/__init__.py
 syne_tune/optimizer/schedulers/searchers/constrained/constrained_gp_fifo_searcher.py
 syne_tune/optimizer/schedulers/searchers/cost_aware/__init__.py
 syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_fifo_searcher.py
 syne_tune/optimizer/schedulers/searchers/cost_aware/cost_aware_gp_multifidelity_searcher.py
 syne_tune/optimizer/schedulers/searchers/dyhpo/__init__.py
 syne_tune/optimizer/schedulers/searchers/dyhpo/dyhpo_searcher.py
 syne_tune/optimizer/schedulers/searchers/dyhpo/hyperband_dyhpo.py
 syne_tune/optimizer/schedulers/searchers/hypertune/__init__.py
 syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_bracket_distribution.py
 syne_tune/optimizer/schedulers/searchers/hypertune/hypertune_searcher.py
 syne_tune/optimizer/schedulers/searchers/kde/__init__.py
 syne_tune/optimizer/schedulers/searchers/kde/kde_searcher.py
 syne_tune/optimizer/schedulers/searchers/kde/multi_fidelity_kde_searcher.py
+syne_tune/optimizer/schedulers/searchers/sklearn/__init__.py
+syne_tune/optimizer/schedulers/searchers/sklearn/sklearn_surrogate_searcher.py
 syne_tune/optimizer/schedulers/searchers/utils/__init__.py
 syne_tune/optimizer/schedulers/searchers/utils/common.py
 syne_tune/optimizer/schedulers/searchers/utils/default_arguments.py
 syne_tune/optimizer/schedulers/searchers/utils/exclusion_list.py
 syne_tune/optimizer/schedulers/searchers/utils/hp_ranges.py
 syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_factory.py
 syne_tune/optimizer/schedulers/searchers/utils/hp_ranges_impl.py
```

### Comparing `syne_tune-0.7.0/syne_tune.egg-info/requires.txt` & `syne_tune-0.8.0/syne_tune.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 boto3
 sagemaker>=2.112.0
 PyYaml
 ujson
 s3fs
 
 [benchmarks]
-torch
-torchvision
-transformers
-tqdm
 datasets==1.8.0
+tqdm
+torchvision
+torch
 filelock
+transformers
 
 [blackbox-repository]
 numpy<1.24.0,>=1.16.0
 pandas
 fastparquet==0.8.1
 s3fs
 scikit-learn
@@ -35,61 +35,61 @@
 GPy==1.12.0
 
 [botorch]
 botorch>=0.7.2
 
 [dev]
 pytest
-pytest-cov~=4.0.0
+pytest-cov~=4.1.0
 pytest-timeout
 black==22.3.0
 flake8
-sphinx
+sphinx<7.0.0
 sphinx-rtd-theme
 sphinx-autodoc-typehints
 myst-parser
 sphinx_copybutton
 sphinxcontrib-bibtex
 sphinxcontrib.jquery
 
 [extra]
 scipy>=1.3.3
 autograd>=1.3
 statsmodels
 pytest
-pytest-cov~=4.0.0
+pytest-cov~=4.1.0
 pytest-timeout
 black==22.3.0
 flake8
-sphinx
+sphinx<7.0.0
 sphinx-rtd-theme
 sphinx-autodoc-typehints
 myst-parser
 sphinx_copybutton
 sphinxcontrib-bibtex
 sphinxcontrib.jquery
 boto3
 sagemaker>=2.112.0
 PyYaml
 ujson
 s3fs
 pymoo>=0.6.0
 matplotlib
+scikit-learn
 numpy<1.24.0,>=1.16.0
 pandas
 fastparquet==0.8.1
-scikit-learn
 xgboost
 h5py
-torch
-torchvision
-transformers
-tqdm
 datasets==1.8.0
+tqdm
+torchvision
+torch
 filelock
+transformers
 onnxruntime>=1.10.0
 configspace
 yahpo-gym
 ray[tune]>=2.0.0
 scikit-optimize
 botorch>=0.7.2
 
@@ -104,14 +104,17 @@
 pymoo>=0.6.0
 
 [raytune]
 ray[tune]>=2.0.0
 scikit-learn
 scikit-optimize
 
+[sklearn]
+scikit-learn
+
 [visual]
 matplotlib
 
 [yahpo]
 onnxruntime>=1.10.0
 pyyaml
 configspace
```

