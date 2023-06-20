# Comparing `tmp/pidgan-0.0.1.tar.gz` & `tmp/pidgan-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pidgan-0.0.1.tar", last modified: Wed Jun 14 09:18:23 2023, max compression
+gzip compressed data, was "pidgan-0.0.2.tar", last modified: Tue Jun 20 14:10:45 2023, max compression
```

## Comparing `pidgan-0.0.1.tar` & `pidgan-0.0.2.tar`

### file list

```diff
@@ -1,148 +1,94 @@
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.854516 pidgan-0.0.1/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)    35148 2023-02-05 20:35:00.000000 pidgan-0.0.1/LICENSE
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     4121 2023-06-14 09:18:23.854516 pidgan-0.0.1/PKG-INFO
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     3009 2023-06-14 09:16:05.000000 pidgan-0.0.1/README.md
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     1797 2023-06-13 21:30:56.000000 pidgan-0.0.1/pyproject.toml
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      233 2023-06-14 09:18:23.854516 pidgan-0.0.1/setup.cfg
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.803516 pidgan-0.0.1/src/
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.842516 pidgan-0.0.1/src/old_pkg/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)       32 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/__init__.py
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.842516 pidgan-0.0.1/src/old_pkg/algorithms/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)        0 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/algorithms/__init__.py
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.843516 pidgan-0.0.1/src/old_pkg/algorithms/gan/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     5929 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/algorithms/gan/BceGAN.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     7488 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/algorithms/gan/CramerGAN.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)    18380 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/algorithms/gan/GAN.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)    10770 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/algorithms/gan/WGAN_ALP.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     5657 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/algorithms/gan/WGAN_GP.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      152 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/algorithms/gan/__init__.py
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.843516 pidgan-0.0.1/src/old_pkg/algorithms/norm_flow/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     5562 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/algorithms/norm_flow/LbVAE.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)        0 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/algorithms/norm_flow/NormFlow.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)        0 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/algorithms/norm_flow/VAE_NF.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)       24 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/algorithms/norm_flow/__init__.py
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.843516 pidgan-0.0.1/src/old_pkg/callbacks/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     1431 2023-02-05 22:54:56.000000 pidgan-0.0.1/src/old_pkg/callbacks/HopaasReporter.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      644 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/callbacks/StopWatch.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)       75 2023-02-05 22:54:56.000000 pidgan-0.0.1/src/old_pkg/callbacks/__init__.py
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.844516 pidgan-0.0.1/src/old_pkg/callbacks/gan/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     2096 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/callbacks/gan/HopaasModelSaver.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     2406 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/callbacks/gan/ModelSaver.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      707 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/callbacks/gan/RefereeInitializer.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      205 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/callbacks/gan/__init__.py
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.844516 pidgan-0.0.1/src/old_pkg/callbacks/gan/schedulers/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      951 2023-02-05 22:54:56.000000 pidgan-0.0.1/src/old_pkg/callbacks/gan/schedulers/BaseLrScheduler.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      438 2023-02-05 22:54:56.000000 pidgan-0.0.1/src/old_pkg/callbacks/gan/schedulers/ExpLrScheduler.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      437 2023-02-05 22:54:56.000000 pidgan-0.0.1/src/old_pkg/callbacks/gan/schedulers/PowLrScheduler.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      132 2023-02-05 22:54:56.000000 pidgan-0.0.1/src/old_pkg/callbacks/gan/schedulers/__init__.py
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.844516 pidgan-0.0.1/src/old_pkg/layers/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     2436 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/layers/AddRandomFeatures.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     2020 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/layers/Triangular.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)       90 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/layers/__init__.py
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.845516 pidgan-0.0.1/src/old_pkg/metrics/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     6854 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/metrics/JS_div.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     5772 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/metrics/KL_div.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     4817 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/metrics/KS_test.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)        0 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/metrics/Variance.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      207 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/metrics/__init__.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     4030 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/metrics/chi2_test.py
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.845516 pidgan-0.0.1/src/old_pkg/preprocessing/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     3058 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/preprocessing/LbColTransformer.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      698 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/preprocessing/WeightedQuantileTransformer.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      126 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/preprocessing/__init__.py
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.846516 pidgan-0.0.1/src/old_pkg/trainers/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)    10011 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/trainers/BaseTrainer.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     7681 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/trainers/DataHandler.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)    30597 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/trainers/GanTrainer.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)        0 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/trainers/NormFlowTrainer.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)    15204 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/trainers/ScikitClassifier.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)    14261 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/trainers/ScikitTrainer.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)    12307 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/trainers/TensorTrainer.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      259 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/trainers/__init__.py
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.847516 pidgan-0.0.1/src/old_pkg/utils/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     1306 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/utils/ParamHandler.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      353 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/utils/__init__.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     1759 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/utils/argparser.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     4218 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/utils/data_from_trees.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     3872 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/utils/getBinCounts.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     1328 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/utils/getModelSummary.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     1340 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/utils/nan_filter.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     2248 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/utils/pre_preprocessing_step.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     7442 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/utils/preprocessor.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     1279 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/utils/warn_message.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)       21 2023-02-05 22:54:57.000000 pidgan-0.0.1/src/old_pkg/version.py
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.848516 pidgan-0.0.1/src/pidgan/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)       33 2023-06-13 10:49:46.000000 pidgan-0.0.1/src/pidgan/__init__.py
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.849516 pidgan-0.0.1/src/pidgan/algorithms/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     3979 2023-06-13 20:04:03.000000 pidgan-0.0.1/src/pidgan/algorithms/BceGAN.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     7739 2023-06-13 20:30:48.000000 pidgan-0.0.1/src/pidgan/algorithms/CramerGAN.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)    14532 2023-06-13 19:53:55.000000 pidgan-0.0.1/src/pidgan/algorithms/GAN.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     4413 2023-06-13 19:30:36.000000 pidgan-0.0.1/src/pidgan/algorithms/LSGAN.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     5116 2023-06-13 20:36:13.000000 pidgan-0.0.1/src/pidgan/algorithms/WGAN.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     6373 2023-06-13 20:26:51.000000 pidgan-0.0.1/src/pidgan/algorithms/WGAN_ALP.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     5521 2023-06-13 20:23:17.000000 pidgan-0.0.1/src/pidgan/algorithms/WGAN_GP.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      189 2023-06-13 19:30:41.000000 pidgan-0.0.1/src/pidgan/algorithms/__init__.py
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.849516 pidgan-0.0.1/src/pidgan/callbacks/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)        0 2023-06-12 11:42:13.000000 pidgan-0.0.1/src/pidgan/callbacks/__init__.py
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.850516 pidgan-0.0.1/src/pidgan/callbacks/schedulers/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     1823 2023-06-12 11:42:13.000000 pidgan-0.0.1/src/pidgan/callbacks/schedulers/LearnRateBaseScheduler.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     2044 2023-06-12 11:43:16.000000 pidgan-0.0.1/src/pidgan/callbacks/schedulers/LearnRateCosineDecay.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     2125 2023-06-12 11:43:21.000000 pidgan-0.0.1/src/pidgan/callbacks/schedulers/LearnRateExpDecay.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     2140 2023-06-12 11:43:27.000000 pidgan-0.0.1/src/pidgan/callbacks/schedulers/LearnRateInvTimeDecay.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     1422 2023-06-12 11:43:34.000000 pidgan-0.0.1/src/pidgan/callbacks/schedulers/LearnRatePiecewiseConstDecay.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     2177 2023-06-12 11:43:40.000000 pidgan-0.0.1/src/pidgan/callbacks/schedulers/LearnRatePolynomialDecay.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      295 2023-06-12 11:44:17.000000 pidgan-0.0.1/src/pidgan/callbacks/schedulers/__init__.py
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.851516 pidgan-0.0.1/src/pidgan/metrics/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      606 2023-06-13 11:36:24.000000 pidgan-0.0.1/src/pidgan/metrics/Accuracy.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      558 2023-06-12 11:43:57.000000 pidgan-0.0.1/src/pidgan/metrics/BaseMetric.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      696 2023-06-13 11:33:27.000000 pidgan-0.0.1/src/pidgan/metrics/BinaryCrossentropy.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      808 2023-06-13 11:36:24.000000 pidgan-0.0.1/src/pidgan/metrics/JSDivergence.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      526 2023-06-13 11:34:06.000000 pidgan-0.0.1/src/pidgan/metrics/KLDivergence.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      529 2023-06-13 11:34:10.000000 pidgan-0.0.1/src/pidgan/metrics/MeanAbsoluteError.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      527 2023-06-13 11:34:14.000000 pidgan-0.0.1/src/pidgan/metrics/MeanSquaredError.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      524 2023-06-13 11:34:18.000000 pidgan-0.0.1/src/pidgan/metrics/RootMeanSquaredError.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      596 2023-06-13 20:39:48.000000 pidgan-0.0.1/src/pidgan/metrics/WassersteinDistance.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      364 2023-06-12 11:43:57.000000 pidgan-0.0.1/src/pidgan/metrics/__init__.py
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.840516 pidgan-0.0.1/src/pidgan/optimization/
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.851516 pidgan-0.0.1/src/pidgan/optimization/callbacks/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     1661 2023-06-13 11:51:21.000000 pidgan-0.0.1/src/pidgan/optimization/callbacks/HopaasPruner.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)       39 2023-06-12 11:42:19.000000 pidgan-0.0.1/src/pidgan/optimization/callbacks/__init__.py
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.852516 pidgan-0.0.1/src/pidgan/optimization/scores/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      676 2023-06-12 11:46:08.000000 pidgan-0.0.1/src/pidgan/optimization/scores/BaseScore.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      210 2023-06-12 11:46:14.000000 pidgan-0.0.1/src/pidgan/optimization/scores/ChiSquare.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      973 2023-06-12 11:46:19.000000 pidgan-0.0.1/src/pidgan/optimization/scores/EMDistance.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      212 2023-06-12 11:46:24.000000 pidgan-0.0.1/src/pidgan/optimization/scores/JSDivergence.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      212 2023-06-12 11:46:30.000000 pidgan-0.0.1/src/pidgan/optimization/scores/KLDivergence.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      210 2023-06-12 11:46:35.000000 pidgan-0.0.1/src/pidgan/optimization/scores/KSDistance.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)       35 2023-06-12 11:42:19.000000 pidgan-0.0.1/src/pidgan/optimization/scores/__init__.py
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.852516 pidgan-0.0.1/src/pidgan/players/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)        0 2023-06-07 14:02:20.000000 pidgan-0.0.1/src/pidgan/players/__init__.py
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.852516 pidgan-0.0.1/src/pidgan/players/classifiers/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      164 2023-06-13 14:10:29.000000 pidgan-0.0.1/src/pidgan/players/classifiers/Classifier.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)       35 2023-06-13 14:10:43.000000 pidgan-0.0.1/src/pidgan/players/classifiers/__init__.py
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.852516 pidgan-0.0.1/src/pidgan/players/discriminators/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     3682 2023-06-13 19:31:15.000000 pidgan-0.0.1/src/pidgan/players/discriminators/Discriminator.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      235 2023-06-13 10:49:46.000000 pidgan-0.0.1/src/pidgan/players/discriminators/SkipDiscriminator.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)       41 2023-06-13 14:09:10.000000 pidgan-0.0.1/src/pidgan/players/discriminators/__init__.py
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.853516 pidgan-0.0.1/src/pidgan/players/generators/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     4320 2023-06-13 19:31:20.000000 pidgan-0.0.1/src/pidgan/players/generators/Generator.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      219 2023-06-13 10:49:46.000000 pidgan-0.0.1/src/pidgan/players/generators/SkipGenerator.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)       33 2023-06-13 19:30:36.000000 pidgan-0.0.1/src/pidgan/players/generators/__init__.py
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.853516 pidgan-0.0.1/src/pidgan/players/regressors/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      163 2023-06-13 14:09:36.000000 pidgan-0.0.1/src/pidgan/players/regressors/Regressor.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)       33 2023-06-13 14:09:46.000000 pidgan-0.0.1/src/pidgan/players/regressors/__init__.py
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.853516 pidgan-0.0.1/src/pidgan/utils/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     1409 2023-06-13 10:49:51.000000 pidgan-0.0.1/src/pidgan/utils/HPSingleton.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)       84 2023-06-12 11:37:54.000000 pidgan-0.0.1/src/pidgan/utils/__init__.py
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.853516 pidgan-0.0.1/src/pidgan/utils/checks/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)       82 2023-06-12 11:38:35.000000 pidgan-0.0.1/src/pidgan/utils/checks/__init__.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     2097 2023-06-12 11:39:39.000000 pidgan-0.0.1/src/pidgan/utils/checks/checkMetrics.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      816 2023-06-12 11:39:49.000000 pidgan-0.0.1/src/pidgan/utils/checks/checkOptimizer.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     1347 2023-06-13 10:49:46.000000 pidgan-0.0.1/src/pidgan/utils/getSummaryHTML.py
--rw-r--r--   0 mabarbet  (1009) z5        (1470)       22 2023-06-13 11:39:52.000000 pidgan-0.0.1/src/pidgan/version.py
-drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:18:23.848516 pidgan-0.0.1/src/pidgan.egg-info/
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     4121 2023-06-14 09:18:23.000000 pidgan-0.0.1/src/pidgan.egg-info/PKG-INFO
--rw-r--r--   0 mabarbet  (1009) z5        (1470)     4479 2023-06-14 09:18:23.000000 pidgan-0.0.1/src/pidgan.egg-info/SOURCES.txt
--rw-r--r--   0 mabarbet  (1009) z5        (1470)        1 2023-06-14 09:18:23.000000 pidgan-0.0.1/src/pidgan.egg-info/dependency_links.txt
--rw-r--r--   0 mabarbet  (1009) z5        (1470)      163 2023-06-14 09:18:23.000000 pidgan-0.0.1/src/pidgan.egg-info/requires.txt
--rw-r--r--   0 mabarbet  (1009) z5        (1470)       15 2023-06-14 09:18:23.000000 pidgan-0.0.1/src/pidgan.egg-info/top_level.txt
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-20 14:10:45.902905 pidgan-0.0.2/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)    35148 2023-02-05 20:35:00.000000 pidgan-0.0.2/LICENSE
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     4222 2023-06-20 14:10:45.902905 pidgan-0.0.2/PKG-INFO
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     3109 2023-06-14 09:39:41.000000 pidgan-0.0.2/README.md
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     1802 2023-06-16 18:32:35.000000 pidgan-0.0.2/pyproject.toml
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      233 2023-06-20 14:10:45.902905 pidgan-0.0.2/setup.cfg
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-20 14:10:45.892905 pidgan-0.0.2/src/
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-20 14:10:45.894905 pidgan-0.0.2/src/pidgan/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)       33 2023-06-13 10:49:46.000000 pidgan-0.0.2/src/pidgan/__init__.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-20 14:10:45.896905 pidgan-0.0.2/src/pidgan/algorithms/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     4083 2023-06-20 13:53:45.000000 pidgan-0.0.2/src/pidgan/algorithms/BceGAN.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     7753 2023-06-20 13:53:37.000000 pidgan-0.0.2/src/pidgan/algorithms/CramerGAN.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)    16846 2023-06-20 10:01:30.000000 pidgan-0.0.2/src/pidgan/algorithms/GAN.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     4516 2023-06-20 13:53:27.000000 pidgan-0.0.2/src/pidgan/algorithms/LSGAN.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     5218 2023-06-20 13:52:59.000000 pidgan-0.0.2/src/pidgan/algorithms/WGAN.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     6391 2023-06-20 13:53:17.000000 pidgan-0.0.2/src/pidgan/algorithms/WGAN_ALP.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     3817 2023-06-20 13:53:07.000000 pidgan-0.0.2/src/pidgan/algorithms/WGAN_GP.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      189 2023-06-13 19:30:41.000000 pidgan-0.0.2/src/pidgan/algorithms/__init__.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-20 14:10:45.896905 pidgan-0.0.2/src/pidgan/callbacks/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)        0 2023-06-12 11:42:13.000000 pidgan-0.0.2/src/pidgan/callbacks/__init__.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-20 14:10:45.897905 pidgan-0.0.2/src/pidgan/callbacks/schedulers/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     1823 2023-06-12 11:42:13.000000 pidgan-0.0.2/src/pidgan/callbacks/schedulers/LearnRateBaseScheduler.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     2044 2023-06-12 11:43:16.000000 pidgan-0.0.2/src/pidgan/callbacks/schedulers/LearnRateCosineDecay.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     2125 2023-06-12 11:43:21.000000 pidgan-0.0.2/src/pidgan/callbacks/schedulers/LearnRateExpDecay.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     2140 2023-06-12 11:43:27.000000 pidgan-0.0.2/src/pidgan/callbacks/schedulers/LearnRateInvTimeDecay.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     1422 2023-06-12 11:43:34.000000 pidgan-0.0.2/src/pidgan/callbacks/schedulers/LearnRatePiecewiseConstDecay.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     2177 2023-06-12 11:43:40.000000 pidgan-0.0.2/src/pidgan/callbacks/schedulers/LearnRatePolynomialDecay.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      295 2023-06-12 11:44:17.000000 pidgan-0.0.2/src/pidgan/callbacks/schedulers/__init__.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-20 14:10:45.898905 pidgan-0.0.2/src/pidgan/metrics/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      606 2023-06-13 11:36:24.000000 pidgan-0.0.2/src/pidgan/metrics/Accuracy.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      558 2023-06-12 11:43:57.000000 pidgan-0.0.2/src/pidgan/metrics/BaseMetric.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      696 2023-06-13 11:33:27.000000 pidgan-0.0.2/src/pidgan/metrics/BinaryCrossentropy.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      808 2023-06-13 11:36:24.000000 pidgan-0.0.2/src/pidgan/metrics/JSDivergence.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      526 2023-06-13 11:34:06.000000 pidgan-0.0.2/src/pidgan/metrics/KLDivergence.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      529 2023-06-13 11:34:10.000000 pidgan-0.0.2/src/pidgan/metrics/MeanAbsoluteError.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      527 2023-06-13 11:34:14.000000 pidgan-0.0.2/src/pidgan/metrics/MeanSquaredError.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      524 2023-06-13 11:34:18.000000 pidgan-0.0.2/src/pidgan/metrics/RootMeanSquaredError.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      596 2023-06-13 20:39:48.000000 pidgan-0.0.2/src/pidgan/metrics/WassersteinDistance.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      364 2023-06-12 11:43:57.000000 pidgan-0.0.2/src/pidgan/metrics/__init__.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-20 14:10:45.893905 pidgan-0.0.2/src/pidgan/optimization/
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-20 14:10:45.898905 pidgan-0.0.2/src/pidgan/optimization/callbacks/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     1661 2023-06-13 11:51:21.000000 pidgan-0.0.2/src/pidgan/optimization/callbacks/HopaasPruner.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)       39 2023-06-12 11:42:19.000000 pidgan-0.0.2/src/pidgan/optimization/callbacks/__init__.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-20 14:10:45.899905 pidgan-0.0.2/src/pidgan/optimization/scores/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      676 2023-06-12 11:46:08.000000 pidgan-0.0.2/src/pidgan/optimization/scores/BaseScore.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      210 2023-06-12 11:46:14.000000 pidgan-0.0.2/src/pidgan/optimization/scores/ChiSquare.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     1202 2023-06-19 16:31:22.000000 pidgan-0.0.2/src/pidgan/optimization/scores/EMDistance.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      212 2023-06-12 11:46:24.000000 pidgan-0.0.2/src/pidgan/optimization/scores/JSDivergence.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      212 2023-06-12 11:46:30.000000 pidgan-0.0.2/src/pidgan/optimization/scores/KLDivergence.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     1040 2023-06-19 16:31:22.000000 pidgan-0.0.2/src/pidgan/optimization/scores/KSDistance.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)       70 2023-06-19 13:29:44.000000 pidgan-0.0.2/src/pidgan/optimization/scores/__init__.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-20 14:10:45.899905 pidgan-0.0.2/src/pidgan/players/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)        0 2023-06-07 14:02:20.000000 pidgan-0.0.2/src/pidgan/players/__init__.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-20 14:10:45.899905 pidgan-0.0.2/src/pidgan/players/classifiers/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      164 2023-06-13 14:10:29.000000 pidgan-0.0.2/src/pidgan/players/classifiers/Classifier.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)       35 2023-06-13 14:10:43.000000 pidgan-0.0.2/src/pidgan/players/classifiers/__init__.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-20 14:10:45.900905 pidgan-0.0.2/src/pidgan/players/discriminators/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     3796 2023-06-16 09:28:10.000000 pidgan-0.0.2/src/pidgan/players/discriminators/Discriminator.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:51:54.000000 pidgan-0.0.2/src/pidgan/players/discriminators/GigaDiscriminator.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:47:55.000000 pidgan-0.0.2/src/pidgan/players/discriminators/MinibatchDiscriminator.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      235 2023-06-13 10:49:46.000000 pidgan-0.0.2/src/pidgan/players/discriminators/SkipDiscriminator.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)       41 2023-06-13 14:09:10.000000 pidgan-0.0.2/src/pidgan/players/discriminators/__init__.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-20 14:10:45.900905 pidgan-0.0.2/src/pidgan/players/generators/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     4387 2023-06-16 12:53:21.000000 pidgan-0.0.2/src/pidgan/players/generators/Generator.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:52:03.000000 pidgan-0.0.2/src/pidgan/players/generators/GigaGenerator.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 09:48:04.000000 pidgan-0.0.2/src/pidgan/players/generators/MinibatchGenerator.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      219 2023-06-13 10:49:46.000000 pidgan-0.0.2/src/pidgan/players/generators/SkipGenerator.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)       33 2023-06-13 19:30:36.000000 pidgan-0.0.2/src/pidgan/players/generators/__init__.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-20 14:10:45.901905 pidgan-0.0.2/src/pidgan/players/regressors/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      163 2023-06-13 14:09:36.000000 pidgan-0.0.2/src/pidgan/players/regressors/Regressor.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)       33 2023-06-13 14:09:46.000000 pidgan-0.0.2/src/pidgan/players/regressors/__init__.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-20 14:10:45.901905 pidgan-0.0.2/src/pidgan/preprocessing/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      759 2023-06-14 10:04:49.000000 pidgan-0.0.2/src/pidgan/preprocessing/WeightedQuantileTransformer.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)       69 2023-06-14 10:23:47.000000 pidgan-0.0.2/src/pidgan/preprocessing/__init__.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-20 14:10:45.901905 pidgan-0.0.2/src/pidgan/utils/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)        0 2023-06-14 10:33:16.000000 pidgan-0.0.2/src/pidgan/utils/__init__.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-20 14:10:45.901905 pidgan-0.0.2/src/pidgan/utils/checks/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)       82 2023-06-12 11:38:35.000000 pidgan-0.0.2/src/pidgan/utils/checks/__init__.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     2097 2023-06-12 11:39:39.000000 pidgan-0.0.2/src/pidgan/utils/checks/checkMetrics.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      816 2023-06-12 11:39:49.000000 pidgan-0.0.2/src/pidgan/utils/checks/checkOptimizer.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-20 14:10:45.901905 pidgan-0.0.2/src/pidgan/utils/preprocessing/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)       61 2023-06-14 10:33:46.000000 pidgan-0.0.2/src/pidgan/utils/preprocessing/__init__.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      827 2023-06-15 14:53:10.000000 pidgan-0.0.2/src/pidgan/utils/preprocessing/invertColumnTransformer.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-20 14:10:45.902905 pidgan-0.0.2/src/pidgan/utils/reports/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     1409 2023-06-13 10:49:51.000000 pidgan-0.0.2/src/pidgan/utils/reports/HPSingleton.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)       84 2023-06-14 10:33:08.000000 pidgan-0.0.2/src/pidgan/utils/reports/__init__.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     1347 2023-06-13 10:49:46.000000 pidgan-0.0.2/src/pidgan/utils/reports/getSummaryHTML.py
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)       22 2023-06-14 09:20:59.000000 pidgan-0.0.2/src/pidgan/version.py
+drwxr-xr-x   0 mabarbet  (1009) z5        (1470)        0 2023-06-20 14:10:45.895905 pidgan-0.0.2/src/pidgan.egg-info/
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     4222 2023-06-20 14:10:45.000000 pidgan-0.0.2/src/pidgan.egg-info/PKG-INFO
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)     2883 2023-06-20 14:10:45.000000 pidgan-0.0.2/src/pidgan.egg-info/SOURCES.txt
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)        1 2023-06-20 14:10:45.000000 pidgan-0.0.2/src/pidgan.egg-info/dependency_links.txt
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)      168 2023-06-20 14:10:45.000000 pidgan-0.0.2/src/pidgan.egg-info/requires.txt
+-rw-r--r--   0 mabarbet  (1009) z5        (1470)        7 2023-06-20 14:10:45.000000 pidgan-0.0.2/src/pidgan.egg-info/top_level.txt
```

### Comparing `pidgan-0.0.1/LICENSE` & `pidgan-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pidgan-0.0.1/PKG-INFO` & `pidgan-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pidgan
-Version: 0.0.1
+Version: 0.0.2
 Summary: GAN-based models to fast-simulate the LHCb PID detectors
 Author-email: Matteo Barbetti <matteo.barbetti@fi.infn.it>, Lucio Anderlini <lucio.anderlini@fi.infn.it>
 License: GPLv3 License
 Project-URL: repository, https://github.com/mbarbetti/pidgan
 Keywords: tensorflow,machine learning,deep learning,generative adversarial nets,lhcb experiment,lamarr,ultra-fast simulation,particle identification
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -35,17 +35,15 @@
 </h2>
 
 <p align="center">
   <a href="https://www.tensorflow.org/versions"><img alt="TensorFlow versions" src="https://img.shields.io/badge/tensorflow-2.7–2.12-f57000?style=flat"></a>
   <a href="https://scikit-learn.org/stable/whats_new.html"><img alt="scikit-learn versions" src="https://img.shields.io/badge/sklearn-1.0–1.2-f89939?style=flat"></a>
   <a href="https://www.python.org/downloads"><img alt="Python versions" src="https://img.shields.io/badge/python-3.7–3.11-blue?style=flat"></a>
   <a href="https://pypi.python.org/pypi/pidgan"><img alt="PyPI - Version" src="https://img.shields.io/pypi/v/pidgan"></a>
-  <!--
   <a href="LICENSE"><img alt="GitHub - License" src="https://img.shields.io/github/license/mbarbetti/pidgan"></a>
-  -->
 </p>
 
 <p align="center">
   <a href="https://github.com/mbarbetti/pidgan/actions/workflows/tests.yml"><img alt="GitHub - Tests" src="https://github.com/mbarbetti/pidgan/actions/workflows/tests.yml/badge.svg?branch=main"></a>
   <a href="https://codecov.io/gh/mbarbetti/pidgan"><img alt="Codecov" src="https://codecov.io/gh/mbarbetti/pidgan/branch/main/graph/badge.svg?token=ZLWDgWhnkq"></a>
 </p>
 
@@ -56,18 +54,24 @@
 
 <!--
 [![Docker - Version](https://img.shields.io/docker/v/mbarbetti/pidgan?label=docker)](https://hub.docker.com/r/mbarbetti/pidgan)
 -->
 
 ### Generative Adversarial Networks
 
-| Algorithms | Implementation |  Test  |                         Paper                        |
-|:----------:|:--------------:|:------:|:----------------------------------------------------:|
-|    `GAN`   |       ✅       |   ✅   |  [arXiv:1406.2661](https://arxiv.org/abs/1406.2661)  |
-|  `BceGAN`  |       ✅       |   ✅   |                                                      |
-|   `LSGAN`  |       ✅       |   ✅   | [arXiv:1611.04076](https://arxiv.org/abs/1611.04076) |
-|   `WGAN`   |       ✅       |   ✅   | [arXiv:1701.07875](https://arxiv.org/abs/1701.07875) |
-|  `WGAN_GP` |       ✅       |   ✅   | [arXiv:1704.00028](https://arxiv.org/abs/1704.00028) |
-| `CramerGAN`|       ✅       |   ✅   | [arXiv:1705.10743](https://arxiv.org/abs/1705.10743) |
-| `WGAN_ALP` |       ✅       |   ✅   | [arXiv:1907.05681](https://arxiv.org/abs/1907.05681) |
+| Algorithms* | Implementation |  Test  |                         Paper                        |
+|:-----------:|:--------------:|:------:|:----------------------------------------------------:|
+|    `GAN`    |       ✅       |   ✅   |  [arXiv:1406.2661](https://arxiv.org/abs/1406.2661)  |
+|  `BceGAN`   |       ✅       |   ✅   |                                                      |
+|   `LSGAN`   |       ✅       |   ✅   | [arXiv:1611.04076](https://arxiv.org/abs/1611.04076) |
+|   `WGAN`    |       ✅       |   ✅   | [arXiv:1701.07875](https://arxiv.org/abs/1701.07875) |
+|  `WGAN_GP`  |       ✅       |   ✅   | [arXiv:1704.00028](https://arxiv.org/abs/1704.00028) |
+| `CramerGAN` |       ✅       |   ✅   | [arXiv:1705.10743](https://arxiv.org/abs/1705.10743) |
+| `WGAN_ALP`  |       ✅       |   ✅   | [arXiv:1907.05681](https://arxiv.org/abs/1907.05681) |
 
-*All the algorithms available are designed to operate according to the **conditional version** proposed in [arXiv:1411.1784](https://arxiv.org/abs/1411.1784)
+*Designed to operate according to the **conditional version** proposed in [arXiv:1411.1784](https://arxiv.org/abs/1411.1784)
+
+<!--
+#### Some tricks:
+* [arXiv:1606.03498](https://arxiv.org/abs/1606.03498)
+* [arXiv:1701.04862](https://arxiv.org/abs/1701.04862)
+-->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pidgan Version: 0.0.1 Summary: GAN-based models to
+Metadata-Version: 2.1 Name: pidgan Version: 0.0.2 Summary: GAN-based models to
 fast-simulate the LHCb PID detectors Author-email: Matteo Barbetti
 barbetti@fi.infn.it>, Lucio Anderlini
 anderlini@fi.infn.it> License: GPLv3 License Project-URL: repository, https://
 github.com/mbarbetti/pidgan Keywords: tensorflow,machine learning,deep
 learning,generative adversarial nets,lhcb experiment,lamarr,ultra-fast
 simulation,particle identification Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
@@ -12,21 +12,21 @@
 Language :: Python :: 3.11 Classifier: Topic :: Scientific/Engineering ::
 Physics Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: <=3.11,>=3.7 Description-Content-Type: text/markdown Provides-
 Extra: lamarr Provides-Extra: style Provides-Extra: tests License-File: LICENSE
                              ****** PIDGAN ******
      ***** GAN-based models to fast-simulate the LHCb PID detectors *****
     [TensorFlow_versions] [scikit-learn_versions] [Python_versions] [PyPI_-
-                                   Version]
+                          Version] [GitHub_-_License]
                           [GitHub_-_Tests] [Codecov]
                      [GitHub_-_Style] [Code_style:_black]
- ### Generative Adversarial Networks | Algorithms | Implementation | Test |
-Paper | |:----------:|:--------------:|:------:|:------------------------------
-----------------------:| | `GAN` | â | â | [arXiv:1406.2661](https://
+ ### Generative Adversarial Networks | Algorithms* | Implementation | Test |
+Paper | |:-----------:|:--------------:|:------:|:-----------------------------
+-----------------------:| | `GAN` | â | â | [arXiv:1406.2661](https://
 arxiv.org/abs/1406.2661) | | `BceGAN` | â | â | | | `LSGAN` | â | â |
 [arXiv:1611.04076](https://arxiv.org/abs/1611.04076) | | `WGAN` | â | â |
 [arXiv:1701.07875](https://arxiv.org/abs/1701.07875) | | `WGAN_GP` | â | â
-| [arXiv:1704.00028](https://arxiv.org/abs/1704.00028) | | `CramerGAN`| â |
+| [arXiv:1704.00028](https://arxiv.org/abs/1704.00028) | | `CramerGAN` | â |
 â | [arXiv:1705.10743](https://arxiv.org/abs/1705.10743) | | `WGAN_ALP` | â
-| â | [arXiv:1907.05681](https://arxiv.org/abs/1907.05681) | *All the
-algorithms available are designed to operate according to the **conditional
-version** proposed in [arXiv:1411.1784](https://arxiv.org/abs/1411.1784)
+| â | [arXiv:1907.05681](https://arxiv.org/abs/1907.05681) | *Designed to
+operate according to the **conditional version** proposed in [arXiv:1411.1784]
+(https://arxiv.org/abs/1411.1784)
```

### Comparing `pidgan-0.0.1/README.md` & `pidgan-0.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -11,17 +11,15 @@
 </h2>
 
 <p align="center">
   <a href="https://www.tensorflow.org/versions"><img alt="TensorFlow versions" src="https://img.shields.io/badge/tensorflow-2.7–2.12-f57000?style=flat"></a>
   <a href="https://scikit-learn.org/stable/whats_new.html"><img alt="scikit-learn versions" src="https://img.shields.io/badge/sklearn-1.0–1.2-f89939?style=flat"></a>
   <a href="https://www.python.org/downloads"><img alt="Python versions" src="https://img.shields.io/badge/python-3.7–3.11-blue?style=flat"></a>
   <a href="https://pypi.python.org/pypi/pidgan"><img alt="PyPI - Version" src="https://img.shields.io/pypi/v/pidgan"></a>
-  <!--
   <a href="LICENSE"><img alt="GitHub - License" src="https://img.shields.io/github/license/mbarbetti/pidgan"></a>
-  -->
 </p>
 
 <p align="center">
   <a href="https://github.com/mbarbetti/pidgan/actions/workflows/tests.yml"><img alt="GitHub - Tests" src="https://github.com/mbarbetti/pidgan/actions/workflows/tests.yml/badge.svg?branch=main"></a>
   <a href="https://codecov.io/gh/mbarbetti/pidgan"><img alt="Codecov" src="https://codecov.io/gh/mbarbetti/pidgan/branch/main/graph/badge.svg?token=ZLWDgWhnkq"></a>
 </p>
 
@@ -32,18 +30,24 @@
 
 <!--
 [![Docker - Version](https://img.shields.io/docker/v/mbarbetti/pidgan?label=docker)](https://hub.docker.com/r/mbarbetti/pidgan)
 -->
 
 ### Generative Adversarial Networks
 
-| Algorithms | Implementation |  Test  |                         Paper                        |
-|:----------:|:--------------:|:------:|:----------------------------------------------------:|
-|    `GAN`   |       ✅       |   ✅   |  [arXiv:1406.2661](https://arxiv.org/abs/1406.2661)  |
-|  `BceGAN`  |       ✅       |   ✅   |                                                      |
-|   `LSGAN`  |       ✅       |   ✅   | [arXiv:1611.04076](https://arxiv.org/abs/1611.04076) |
-|   `WGAN`   |       ✅       |   ✅   | [arXiv:1701.07875](https://arxiv.org/abs/1701.07875) |
-|  `WGAN_GP` |       ✅       |   ✅   | [arXiv:1704.00028](https://arxiv.org/abs/1704.00028) |
-| `CramerGAN`|       ✅       |   ✅   | [arXiv:1705.10743](https://arxiv.org/abs/1705.10743) |
-| `WGAN_ALP` |       ✅       |   ✅   | [arXiv:1907.05681](https://arxiv.org/abs/1907.05681) |
+| Algorithms* | Implementation |  Test  |                         Paper                        |
+|:-----------:|:--------------:|:------:|:----------------------------------------------------:|
+|    `GAN`    |       ✅       |   ✅   |  [arXiv:1406.2661](https://arxiv.org/abs/1406.2661)  |
+|  `BceGAN`   |       ✅       |   ✅   |                                                      |
+|   `LSGAN`   |       ✅       |   ✅   | [arXiv:1611.04076](https://arxiv.org/abs/1611.04076) |
+|   `WGAN`    |       ✅       |   ✅   | [arXiv:1701.07875](https://arxiv.org/abs/1701.07875) |
+|  `WGAN_GP`  |       ✅       |   ✅   | [arXiv:1704.00028](https://arxiv.org/abs/1704.00028) |
+| `CramerGAN` |       ✅       |   ✅   | [arXiv:1705.10743](https://arxiv.org/abs/1705.10743) |
+| `WGAN_ALP`  |       ✅       |   ✅   | [arXiv:1907.05681](https://arxiv.org/abs/1907.05681) |
 
-*All the algorithms available are designed to operate according to the **conditional version** proposed in [arXiv:1411.1784](https://arxiv.org/abs/1411.1784)
+*Designed to operate according to the **conditional version** proposed in [arXiv:1411.1784](https://arxiv.org/abs/1411.1784)
+
+<!--
+#### Some tricks:
+* [arXiv:1606.03498](https://arxiv.org/abs/1606.03498)
+* [arXiv:1701.04862](https://arxiv.org/abs/1701.04862)
+-->
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
                              ****** PIDGAN ******
      ***** GAN-based models to fast-simulate the LHCb PID detectors *****
     [TensorFlow_versions] [scikit-learn_versions] [Python_versions] [PyPI_-
-                                   Version]
+                          Version] [GitHub_-_License]
                           [GitHub_-_Tests] [Codecov]
                      [GitHub_-_Style] [Code_style:_black]
- ### Generative Adversarial Networks | Algorithms | Implementation | Test |
-Paper | |:----------:|:--------------:|:------:|:------------------------------
-----------------------:| | `GAN` | â | â | [arXiv:1406.2661](https://
+ ### Generative Adversarial Networks | Algorithms* | Implementation | Test |
+Paper | |:-----------:|:--------------:|:------:|:-----------------------------
+-----------------------:| | `GAN` | â | â | [arXiv:1406.2661](https://
 arxiv.org/abs/1406.2661) | | `BceGAN` | â | â | | | `LSGAN` | â | â |
 [arXiv:1611.04076](https://arxiv.org/abs/1611.04076) | | `WGAN` | â | â |
 [arXiv:1701.07875](https://arxiv.org/abs/1701.07875) | | `WGAN_GP` | â | â
-| [arXiv:1704.00028](https://arxiv.org/abs/1704.00028) | | `CramerGAN`| â |
+| [arXiv:1704.00028](https://arxiv.org/abs/1704.00028) | | `CramerGAN` | â |
 â | [arXiv:1705.10743](https://arxiv.org/abs/1705.10743) | | `WGAN_ALP` | â
-| â | [arXiv:1907.05681](https://arxiv.org/abs/1907.05681) | *All the
-algorithms available are designed to operate according to the **conditional
-version** proposed in [arXiv:1411.1784](https://arxiv.org/abs/1411.1784)
+| â | [arXiv:1907.05681](https://arxiv.org/abs/1907.05681) | *Designed to
+operate according to the **conditional version** proposed in [arXiv:1411.1784]
+(https://arxiv.org/abs/1411.1784)
```

### Comparing `pidgan-0.0.1/pyproject.toml` & `pidgan-0.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.11",
   "Topic :: Scientific/Engineering :: Physics",
   "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 dependencies = [
   "tensorflow>=2.7",
-  "scikit-learn",
+  "scikit-learn>=1.0",
   # "hopaas-client",   # to be released on PyPI
   "pyyaml"
 ]
 
 [project.optional-dependencies]
 lamarr = [
   "numpy",
```

### Comparing `pidgan-0.0.1/src/old_pkg/preprocessing/WeightedQuantileTransformer.py` & `pidgan-0.0.2/src/pidgan/preprocessing/WeightedQuantileTransformer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import numpy as np
 from sklearn.preprocessing import QuantileTransformer
 
 
-class WeightedQuantileTransformer (QuantileTransformer):
-  def _compute_weight_distortion_1d(self, var, sample_weights):
-    indices = np.argsort (var)
-    cumulative = np.cumsum(sample_weights[indices])
-    cumulative /= cumulative[-1]
-    return np.interp(self.references_, cumulative, var[indices])
+class WeightedQuantileTransformer(QuantileTransformer):
+    def _compute_weight_distortion_1d(self, var, sample_weights):
+        indices = np.argsort(var)
+        cumulative = np.cumsum(sample_weights[indices])
+        cumulative /= cumulative[-1]
+        return np.interp(self.references_, cumulative, var[indices])
 
-  def fit (self, X, y=None, sample_weights=None):
-    QuantileTransformer.fit(self, X, y)
-    if sample_weights is not None:
-      self.quantiles_ = np.array([
-          self._compute_weight_distortion_1d(x, np.asarray(sample_weights)) 
-            for x, q in zip(X.T, self.quantiles_.T)
-          ]).T
-    return self
+    def fit(self, X, y=None, sample_weights=None):
+        QuantileTransformer.fit(self, X, y)
+        if sample_weights is not None:
+            self.quantiles_ = np.array(
+                [
+                    self._compute_weight_distortion_1d(x, np.asarray(sample_weights))
+                    for x in X.T
+                ]
+            ).T
+        return self
```

### Comparing `pidgan-0.0.1/src/old_pkg/utils/ParamHandler.py` & `pidgan-0.0.2/src/pidgan/utils/reports/HPSingleton.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,47 +1,53 @@
-import json
+import pprint
 
+import yaml
 
-class ParamHandler:
-  def __init__ ( self, **kwargs ) -> None:
-    self._params = dict (**kwargs) 
-    self._used_keys = set()
 
-  def update ( self, **kwargs ) -> None:
-    for key in kwargs.keys():
-      if key in self._used_keys: 
-        raise KeyError ( f"The parameter {key} was already used and is now read-only" )
-    self._params.update ( kwargs )
+class HPSingleton:
+    def __init__(self, **kwargs) -> None:
+        self._hparams = dict(**kwargs)
+        self._used_keys = set()
 
-  def get ( self, key, default ) -> dict:
-    if key not in self._params.keys(): self._params [ key ] = default
-    self._used_keys.add ( key ) 
-    return self._params [ key ]
+    def update(self, **kwargs) -> None:
+        for key in kwargs.keys():
+            if key in self._used_keys:
+                raise KeyError(
+                    f"The hyperparameter {key} was already used and is now read-only"
+                )
+        self._hparams.update(kwargs)
 
-  def clean ( self ) -> None:
-    self._params = dict() 
-    self._used_keys = set()
+    def get(self, key, value):
+        if key not in self._hparams.keys():
+            self._hparams[key] = value
+        self._used_keys.add(key)
+        return self._hparams[key]
 
-  def __del__ ( self ) -> None: 
-    for key in self._params.keys():
-      if key not in self._used_keys:
-        print ( f"[WARNING] The parameter {key} was defined but never used" ) 
-        print ( self._used_keys ) 
+    def clean(self) -> None:
+        self._hparams = dict()
+        self._used_keys = set()
 
-  def __str__ ( self ) -> str:
-    import pprint 
-    return pprint.pformat ( self._params )
+    def __del__(self) -> None:
+        for key in self._hparams.keys():
+            if key not in self._used_keys:
+                print(f"[WARNING] The hyperparameter {key} was defined but never used")
+                print(self._used_keys)
 
-  def get_dict ( self ) -> dict:
-    return dict ( **self._params ) 
+    def __str__(self) -> str:
+        return pprint.pformat(self._hparams)
 
-  def dump ( self, filename ) -> None:
-    with open ( filename, "w" ) as fp:
-      json.dump ( self._params, fp ) 
+    def get_dict(self) -> dict:
+        return dict(**self._hparams)
 
+    def dump(self, filename) -> None:
+        with open(filename, "w") as file:
+            yaml.dump(self.get_dict(), file)
 
-__PARAMETERS__ = None 
 
-def getInstance() -> ParamHandler:
-  global __PARAMETERS__
-  if __PARAMETERS__ is None: __PARAMETERS__ = ParamHandler()
-  return __PARAMETERS__
+__HPARAMS__ = None
+
+
+def initHPSingleton() -> HPSingleton:
+    global __HPARAMS__
+    if __HPARAMS__ is None:
+        __HPARAMS__ = HPSingleton()
+    return __HPARAMS__
```

### Comparing `pidgan-0.0.1/src/old_pkg/utils/getModelSummary.py` & `pidgan-0.0.2/src/pidgan/utils/reports/getSummaryHTML.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,36 @@
-def getModelSummary (model):
-  """Returns a HTML table containing the summary of 
-  a neural network implemented as a TensorFlow model.
-
-  Parameters
-  ----------
-    model : TensorFlow model
-      Neural network model implemented with TensorFlow.
-
-  Returns
-  -------
-    table_html : str
-      Table containing model summary in HTML format.
-
-    tot_params : int
-      Total number of trainable parameters.
-  """
-  headers = ["Layer (type)", "Output shape", "Param #"]
-  heads_html = "<tr>\n" + "" . join ( [ f"<th>{h}</th>\n" for h in headers ] ) + "</tr>\n"
-
-  rows = []
-  tot_params = 0
-  for layer in model.layers:
-    layer_type = f"<td>{layer.name} ({layer.__class__.__name__})</td>\n"
-    try:
-      output_shape = f"<td>{layer.get_output_at(0).get_shape()}</td>\n"
-    except:
-      output_shape = "<td>None</td>\n"   # print "None" in case of errors
-    num_params = f"<td>{layer.count_params()}</td>\n"
-    rows . append ( "<tr>\n" + layer_type + output_shape + num_params + "</tr>\n" )
-    tot_params += layer.count_params()
-  rows_html = "" . join ( [ f"{r}" for r in rows ] )
-
-  table_html = '<table width="40%" border="1px solid black">\n \
-                <thead>\n{}</thead>\n \
-                <tbody>\n{}</tbody>\n \
-                </table>' . format (heads_html, rows_html)
+import numpy as np
 
-  return table_html, tot_params
+
+def getSummaryHTML(model) -> tuple:
+    headers = ["Layer (type)", "Output shape", "Param #"]
+    heads_html = "<tr>\n" + "".join([f"<th>{h}</th>\n" for h in headers]) + "</tr>\n"
+
+    rows = []
+    train_params = 0
+    nontrain_params = 0
+    for layer in model.layers:
+        layer_type = f"<td>{layer.name} ({layer.__class__.__name__})</td>\n"
+        try:
+            output_shape = f"<td>{layer.get_output_at(0).get_shape()}</td>\n"
+        except RuntimeError:
+            output_shape = "<td>None</td>\n"  # print "None" in case of errors
+        num_params = f"<td>{layer.count_params()}</td>\n"
+        rows.append("<tr>\n" + layer_type + output_shape + num_params + "</tr>\n")
+        train_params += int(
+            np.sum([np.prod(v.get_shape()) for v in layer.trainable_weights])
+        )
+        nontrain_params += int(
+            np.sum([np.prod(v.get_shape()) for v in layer.non_trainable_weights])
+        )
+    rows_html = "".join([f"{r}" for r in rows])
+
+    table_html = '<table width="40%" border="1px solid black">\n \
+                  <thead>\n{}</thead>\n \
+                  <tbody>\n{}</tbody>\n \
+                  </table>'.format(
+        heads_html, rows_html
+    )
+
+    params_details = (train_params + nontrain_params, train_params, nontrain_params)
+
+    return table_html, params_details
```

### Comparing `pidgan-0.0.1/src/pidgan/algorithms/BceGAN.py` & `pidgan-0.0.2/src/pidgan/algorithms/BceGAN.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         self,
         generator,
         discriminator,
         referee=None,
         injected_noise_stddev=0.0,
         from_logits=False,
         label_smoothing=0.0,
-        name=None,
+        name="BceGAN",
         dtype=None,
     ):
         super().__init__(
             generator=generator,
             discriminator=discriminator,
             referee=referee,
             use_original_loss=True,
@@ -99,14 +99,17 @@
 
         real_loss = self._loss(tf.ones_like(r_out_ref), r_out_ref, sample_weight=w_ref)
         real_loss = tf.cast(real_loss, dtype=y_ref.dtype)
         fake_loss = self._loss(tf.zeros_like(r_out_gen), r_out_gen, sample_weight=w_gen)
         fake_loss = tf.cast(fake_loss, dtype=y_ref.dtype)
         return (real_loss + fake_loss) / 2.0
 
+    def _compute_threshold(self, model, x, y, sample_weight=None) -> tf.Tensor:
+        return 0.0
+
     @property
     def from_logits(self) -> bool:
         return self._from_logits
 
     @property
     def label_smoothing(self) -> float:
         return self._label_smoothing
```

### Comparing `pidgan-0.0.1/src/pidgan/algorithms/CramerGAN.py` & `pidgan-0.0.2/src/pidgan/algorithms/CramerGAN.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 
 class CramerGAN(WGAN_GP):
     def __init__(
         self,
         generator,
         discriminator,
         referee=None,
-        lipschitz_penalty=10.0,
+        lipschitz_penalty=1.0,
         penalty_strategy="two-sided",
         from_logits=None,
         label_smoothing=None,
-        name=None,
+        name="CramerGAN",
         dtype=None,
     ):
         super().__init__(
             generator=generator,
             discriminator=discriminator,
             referee=referee,
             lipschitz_penalty=lipschitz_penalty,
@@ -158,15 +158,15 @@
                 w_gen_1 * w_gen_2
             )
             fake_loss = tf.cast(fake_loss, dtype=y_ref.dtype)
             return (
                 fake_loss
                 - real_loss
                 + self._lipschitz_regularization(
-                    self._critic, x, y, sample_weight, training=training
+                    self._referee_critic, x, y, sample_weight, training=training
                 )
             )
 
     def _lipschitz_regularization(
         self, critic, x, y, sample_weight=None, training=True
     ) -> tf.Tensor:
         trainset_ref, trainset_gen_1, trainset_gen_2 = self._prepare_trainset(
```

### Comparing `pidgan-0.0.1/src/pidgan/algorithms/GAN.py` & `pidgan-0.0.2/src/pidgan/algorithms/GAN.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     def __init__(
         self,
         generator,
         discriminator,
         referee=None,
         use_original_loss=True,
         injected_noise_stddev=0.0,
-        name=None,
+        name="GAN",
         dtype=None,
     ) -> None:
         super().__init__(name=name, dtype=dtype)
         self._loss_name = "GAN original loss"
 
         # Generator
         if not isinstance(generator, Generator):
@@ -60,21 +60,28 @@
         assert isinstance(injected_noise_stddev, (int, float))
         assert injected_noise_stddev >= 0.0
         self._inj_noise_std = float(injected_noise_stddev)
 
     def call(self, x, y=None) -> tuple:
         g_out = self._generator(x)
         d_out_gen = self._discriminator((x, g_out))
-        r_out_gen = self._referee((x, g_out))
         if y is None:
-            return g_out, d_out_gen, r_out_gen
+            if self._referee is not None:
+                r_out_gen = self._referee((x, g_out))
+                return g_out, d_out_gen, r_out_gen
+            else:
+                return g_out, d_out_gen
         else:
             d_out_ref = self._discriminator((x, y))
-            r_out_ref = self._referee((x, y))
-            return g_out, (d_out_gen, d_out_ref), (r_out_gen, r_out_ref)
+            if self._referee is not None:
+                r_out_gen = self._referee((x, g_out))
+                r_out_ref = self._referee((x, y))
+                return g_out, (d_out_gen, d_out_ref), (r_out_gen, r_out_ref)
+            else:
+                return g_out, (d_out_gen, d_out_ref)
 
     def summary(self, **kwargs) -> None:
         print("_" * 65)
         self._generator.summary(**kwargs)
         self._discriminator.summary(**kwargs)
         if self._referee is not None:
             self._referee.summary(**kwargs)
@@ -157,34 +164,43 @@
             x, y = data
             sample_weight = None
         return x, y, sample_weight
 
     def _g_train_step(self, x, y, sample_weight=None) -> None:
         with tf.GradientTape() as tape:
             loss = self._compute_g_loss(x, y, sample_weight, training=True)
+
         trainable_vars = self._generator.trainable_weights
         gradients = tape.gradient(loss, trainable_vars)
         self._g_opt.apply_gradients(zip(gradients, trainable_vars))
-        self._g_loss.update_state(loss)
+
+        threshold = self._compute_threshold(self._discriminator, x, y, sample_weight)
+        self._g_loss.update_state(loss + threshold)
 
     def _d_train_step(self, x, y, sample_weight=None) -> None:
         with tf.GradientTape() as tape:
             loss = self._compute_d_loss(x, y, sample_weight, training=True)
+
         trainable_vars = self._discriminator.trainable_weights
         gradients = tape.gradient(loss, trainable_vars)
         self._d_opt.apply_gradients(zip(gradients, trainable_vars))
-        self._d_loss.update_state(loss)
+
+        threshold = self._compute_threshold(self._discriminator, x, y, sample_weight)
+        self._d_loss.update_state(loss - threshold)
 
     def _r_train_step(self, x, y, sample_weight=None) -> None:
         with tf.GradientTape() as tape:
             loss = self._compute_r_loss(x, y, sample_weight, training=True)
+
         trainable_vars = self._referee.trainable_weights
         gradients = tape.gradient(loss, trainable_vars)
         self._r_opt.apply_gradients(zip(gradients, trainable_vars))
-        self._r_loss.update_state(loss)
+
+        threshold = self._compute_threshold(self._referee, x, y, sample_weight)
+        self._r_loss.update_state(loss - threshold)
 
     def _prepare_trainset(
         self, x, y, sample_weight=None, training_generator=True
     ) -> tuple:
         batch_size = tf.cast(tf.shape(x)[0] / 2, tf.int32)
         x_ref, x_gen = tf.split(x[: batch_size * 2], 2, axis=0)
         y_ref = y[:batch_size]
@@ -299,26 +315,65 @@
             * tf.math.log(
                 tf.clip_by_value(1.0 - r_out_gen, MIN_LOG_VALUE, MAX_LOG_VALUE)
             )
         ) / tf.reduce_sum(w_gen)
         fake_loss = tf.cast(fake_loss, dtype=y_ref.dtype)
         return -(real_loss + fake_loss)
 
+    def _prepare_trainset_threshold(self, x, y, sample_weight=None) -> tuple:
+        batch_size = tf.cast(tf.shape(x)[0] / 2, tf.int32)
+        x_ref_1, x_ref_2 = tf.split(x[: batch_size * 2], 2, axis=0)
+        y_ref_1, y_ref_2 = tf.split(y[: batch_size * 2], 2, axis=0)
+
+        if sample_weight is not None:
+            w_ref_1, w_ref_2 = tf.split(sample_weight[: batch_size * 2], 2, axis=0)
+        else:
+            w_ref_1, w_ref_2 = tf.split(tf.ones(shape=(batch_size * 2,)), 2, axis=0)
+
+        return (x_ref_1, y_ref_1, w_ref_1), (x_ref_2, y_ref_2, w_ref_2)
+
+    def _compute_threshold(self, model, x, y, sample_weight=None) -> tf.Tensor:
+        trainset_ref_1, trainset_ref_2 = self._prepare_trainset_threshold(
+            x, y, sample_weight
+        )
+        x_ref_1, y_ref_1, w_ref_1 = trainset_ref_1
+        x_ref_2, y_ref_2, w_ref_2 = trainset_ref_2
+
+        m_out_ref_1 = model((x_ref_1, y_ref_1), training=False)
+        m_out_ref_2 = model((x_ref_2, y_ref_2), training=False)
+
+        loss_1 = tf.reduce_sum(
+            w_ref_1
+            * tf.math.log(tf.clip_by_value(m_out_ref_1, MIN_LOG_VALUE, MAX_LOG_VALUE))
+        ) / tf.reduce_sum(w_ref_1)
+        loss_1 = tf.cast(loss_1, dtype=y_ref_1.dtype)
+        loss_2 = tf.reduce_sum(
+            w_ref_2
+            * tf.math.log(
+                tf.clip_by_value(1.0 - m_out_ref_2, MIN_LOG_VALUE, MAX_LOG_VALUE)
+            )
+        ) / tf.reduce_sum(w_ref_2)
+        loss_2 = tf.cast(loss_2, dtype=y_ref_1.dtype)
+        return -(loss_1 + loss_2)
+
     def test_step(self, data) -> dict:
         x, y, sample_weight = self._unpack_data(data)
 
+        threshold = self._compute_threshold(self._discriminator, x, y, sample_weight)
+
         g_loss = self._compute_g_loss(x, y, sample_weight, training=False)
-        self._g_loss.update_state(g_loss)
+        self._g_loss.update_state(g_loss + threshold)
 
         d_loss = self._compute_d_loss(x, y, sample_weight, training=False)
-        self._d_loss.update_state(d_loss)
+        self._d_loss.update_state(d_loss - threshold)
 
         if self._referee is not None:
             r_loss = self._compute_r_loss(x, y, sample_weight, training=False)
-            self._r_loss.update_state(r_loss)
+            threshold = self._compute_threshold(self._referee, x, y, sample_weight)
+            self._r_loss.update_state(r_loss - threshold)
 
         train_dict = dict(g_loss=self._g_loss.result(), d_loss=self._d_loss.result())
         if self._referee is not None:
             train_dict.update(dict(r_loss=self._r_loss.result()))
         if self._metrics is not None:
             g_out = self._generator(x, training=False)
             d_out_gen = self._discriminator((x, g_out), training=False)
```

### Comparing `pidgan-0.0.1/src/pidgan/algorithms/LSGAN.py` & `pidgan-0.0.2/src/pidgan/algorithms/LSGAN.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     def __init__(
         self,
         generator,
         discriminator,
         referee=None,
         minimize_pearson_chi2=False,
         injected_noise_stddev=0,
-        name=None,
+        name="LSGAN",
         dtype=None,
     ) -> None:
         super().__init__(
             generator=generator,
             discriminator=discriminator,
             referee=referee,
             use_original_loss=True,
@@ -108,10 +108,13 @@
 
         real_loss = tf.reduce_sum(w_ref * (r_out_ref - 1.0) ** 2) / tf.reduce_sum(w_ref)
         real_loss = tf.cast(real_loss, dtype=y_ref.dtype)
         fake_loss = tf.reduce_sum(w_gen * (r_out_gen - a) ** 2) / tf.reduce_sum(w_gen)
         fake_loss = tf.cast(fake_loss, dtype=y_ref.dtype)
         return (real_loss + fake_loss) / 2.0
 
+    def _compute_threshold(self, model, x, y, sample_weight=None) -> tf.Tensor:
+        return 0.0
+
     @property
     def minimize_pearson_chi2(self) -> bool:
         return self._minimize_pearson_chi2
```

### Comparing `pidgan-0.0.1/src/pidgan/algorithms/WGAN.py` & `pidgan-0.0.2/src/pidgan/algorithms/WGAN.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         self,
         generator,
         discriminator,
         referee=None,
         clip_param=0.01,
         from_logits=None,
         label_smoothing=None,
-        name=None,
+        name="WGAN",
         dtype=None,
     ):
         super().__init__(
             generator=generator,
             discriminator=discriminator,
             referee=referee,
             use_original_loss=True,
@@ -114,14 +114,17 @@
         else:
             real_loss = tf.reduce_sum(w_ref * r_out_ref) / tf.reduce_sum(w_ref)
             real_loss = tf.cast(real_loss, dtype=y_ref.dtype)
             fake_loss = tf.reduce_sum(w_gen * r_out_gen) / tf.reduce_sum(w_gen)
             fake_loss = tf.cast(fake_loss, dtype=y_ref.dtype)
             return fake_loss - real_loss
 
+    def _compute_threshold(self, model, x, y, sample_weight=None) -> tf.Tensor:
+        return 0.0
+
     @property
     def clip_param(self) -> float:
         return self._clip_param
 
     @property
     def from_logits(self):  # TODO: add Union[None, bool]
         return self._from_logits
```

### Comparing `pidgan-0.0.1/src/pidgan/algorithms/WGAN_ALP.py` & `pidgan-0.0.2/src/pidgan/algorithms/WGAN_ALP.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import tensorflow as tf
 
 from pidgan.algorithms.WGAN_GP import WGAN_GP
 
 LIPSCHITZ_CONSTANT = 1.0
-FIXED_XI = 10.0
+FIXED_XI = 1.0
 SAMPLED_XI_MIN = 0.0
 SAMPLED_XI_MAX = 1.0
 EPSILON = 1e-12
 
 
 class WGAN_ALP(WGAN_GP):
     def __init__(
         self,
         generator,
         discriminator,
         referee=None,
-        lipschitz_penalty=100.0,
+        lipschitz_penalty=1.0,
         penalty_strategy="one-sided",
         from_logits=None,
         label_smoothing=None,
-        name=None,
+        name="WGAN-ALP",
         dtype=None,
     ):
         super().__init__(
             generator=generator,
             discriminator=discriminator,
             referee=referee,
             lipschitz_penalty=lipschitz_penalty,
@@ -94,15 +94,14 @@
                     clip_value_max=tf.reduce_max(xy_ref, axis=0),
                 )
                 xy_gen_hat = tf.clip_by_value(
                     xy_gen + FIXED_XI * d_gen,
                     clip_value_min=tf.reduce_min(xy_gen, axis=0),
                     clip_value_max=tf.reduce_max(xy_gen, axis=0),
                 )
-
                 x_ref_hat, y_ref_hat = (
                     xy_ref_hat[:, : tf.shape(x_ref)[1]],
                     xy_ref_hat[:, tf.shape(x_ref)[1] :],
                 )
                 c_out_ref_hat = critic((x_ref_hat, y_ref_hat), training=training)
                 x_gen_hat, y_gen_hat = (
                     xy_gen_hat[:, : tf.shape(x_ref)[1]],
@@ -126,20 +125,20 @@
             maxval=SAMPLED_XI_MAX,
             dtype=y_ref.dtype,
         )
         xi = tf.tile(xi[:, None], (1, tf.shape(xy_ref)[1]))
         xi_ref, xi_gen = tf.split(xi, 2, axis=0)
         d_ref, d_gen = tf.split(d, 2, axis=0)
         xy_ref_hat = tf.clip_by_value(
-            xy_ref + xi_ref * d_ref,
+            xy_ref + (0.5 + xi_ref) * d_ref,
             clip_value_min=tf.reduce_min(xy_ref, axis=0),
             clip_value_max=tf.reduce_max(xy_ref, axis=0),
         )
         xy_gen_hat = tf.clip_by_value(
-            xy_gen + xi_gen * d_gen,
+            xy_gen + (0.5 + xi_gen) * d_gen,
             clip_value_min=tf.reduce_min(xy_gen, axis=0),
             clip_value_max=tf.reduce_max(xy_gen, axis=0),
         )
 
         x_ref_hat, y_ref_hat = (
             xy_ref_hat[:, : tf.shape(x_ref)[1]],
             xy_ref_hat[:, tf.shape(x_ref)[1] :],
```

### Comparing `pidgan-0.0.1/src/pidgan/callbacks/schedulers/LearnRateBaseScheduler.py` & `pidgan-0.0.2/src/pidgan/callbacks/schedulers/LearnRateBaseScheduler.py`

 * *Files identical despite different names*

### Comparing `pidgan-0.0.1/src/pidgan/callbacks/schedulers/LearnRateCosineDecay.py` & `pidgan-0.0.2/src/pidgan/callbacks/schedulers/LearnRateCosineDecay.py`

 * *Files identical despite different names*

### Comparing `pidgan-0.0.1/src/pidgan/callbacks/schedulers/LearnRateExpDecay.py` & `pidgan-0.0.2/src/pidgan/callbacks/schedulers/LearnRateExpDecay.py`

 * *Files identical despite different names*

### Comparing `pidgan-0.0.1/src/pidgan/callbacks/schedulers/LearnRateInvTimeDecay.py` & `pidgan-0.0.2/src/pidgan/callbacks/schedulers/LearnRateInvTimeDecay.py`

 * *Files identical despite different names*

### Comparing `pidgan-0.0.1/src/pidgan/callbacks/schedulers/LearnRatePiecewiseConstDecay.py` & `pidgan-0.0.2/src/pidgan/callbacks/schedulers/LearnRatePiecewiseConstDecay.py`

 * *Files identical despite different names*

### Comparing `pidgan-0.0.1/src/pidgan/callbacks/schedulers/LearnRatePolynomialDecay.py` & `pidgan-0.0.2/src/pidgan/callbacks/schedulers/LearnRatePolynomialDecay.py`

 * *Files identical despite different names*

### Comparing `pidgan-0.0.1/src/pidgan/metrics/Accuracy.py` & `pidgan-0.0.2/src/pidgan/metrics/Accuracy.py`

 * *Files identical despite different names*

### Comparing `pidgan-0.0.1/src/pidgan/metrics/BaseMetric.py` & `pidgan-0.0.2/src/pidgan/metrics/BaseMetric.py`

 * *Files identical despite different names*

### Comparing `pidgan-0.0.1/src/pidgan/metrics/BinaryCrossentropy.py` & `pidgan-0.0.2/src/pidgan/metrics/BinaryCrossentropy.py`

 * *Files identical despite different names*

### Comparing `pidgan-0.0.1/src/pidgan/metrics/JSDivergence.py` & `pidgan-0.0.2/src/pidgan/metrics/JSDivergence.py`

 * *Files identical despite different names*

### Comparing `pidgan-0.0.1/src/pidgan/metrics/KLDivergence.py` & `pidgan-0.0.2/src/pidgan/metrics/KLDivergence.py`

 * *Files identical despite different names*

### Comparing `pidgan-0.0.1/src/pidgan/metrics/MeanAbsoluteError.py` & `pidgan-0.0.2/src/pidgan/metrics/MeanAbsoluteError.py`

 * *Files identical despite different names*

### Comparing `pidgan-0.0.1/src/pidgan/metrics/MeanSquaredError.py` & `pidgan-0.0.2/src/pidgan/metrics/MeanSquaredError.py`

 * *Files identical despite different names*

### Comparing `pidgan-0.0.1/src/pidgan/metrics/RootMeanSquaredError.py` & `pidgan-0.0.2/src/pidgan/metrics/RootMeanSquaredError.py`

 * *Files identical despite different names*

### Comparing `pidgan-0.0.1/src/pidgan/metrics/WassersteinDistance.py` & `pidgan-0.0.2/src/pidgan/metrics/WassersteinDistance.py`

 * *Files identical despite different names*

### Comparing `pidgan-0.0.1/src/pidgan/optimization/callbacks/HopaasPruner.py` & `pidgan-0.0.2/src/pidgan/optimization/callbacks/HopaasPruner.py`

 * *Files identical despite different names*

### Comparing `pidgan-0.0.1/src/pidgan/optimization/scores/BaseScore.py` & `pidgan-0.0.2/src/pidgan/optimization/scores/BaseScore.py`

 * *Files identical despite different names*

### Comparing `pidgan-0.0.1/src/pidgan/players/discriminators/Discriminator.py` & `pidgan-0.0.2/src/pidgan/players/discriminators/Discriminator.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,45 +52,48 @@
                 assert rate >= 0.0 and rate < 1.0
                 self._dropout_rate.append(float(rate))
 
         # Output activation
         self._output_activation = output_activation
 
         # Model
-        self._model = tf.keras.Sequential()
+        self._seq = list()
         for i, (units, rate) in enumerate(
             zip(self._mlp_hidden_units, self._dropout_rate)
         ):
-            self._model.add(
+            self._seq.append(
                 Dense(
                     units=units,
                     activation=None,
                     kernel_initializer="glorot_uniform",
                     bias_initializer="zeros",
-                    name=f"disc_dense_{i}" if name else None,
+                    name=f"dense_{i}" if name else None,
                     dtype=self.dtype,
                 )
             )
-            self._model.add(LeakyReLU(alpha=LEAKY_ALPHA))
-            self._model.add(Dropout(rate=rate))
-        self._model.add(
+            self._seq.append(
+                LeakyReLU(alpha=LEAKY_ALPHA, name=f"leaky_relu_{i}" if name else None)
+            )
+            self._seq.append(Dropout(rate=rate, name=f"dropout_{i}" if name else None))
+        self._seq.append(
             Dense(
                 units=output_dim,
                 activation=output_activation,
                 kernel_initializer="glorot_uniform",
                 bias_initializer="zeros",
-                name="disc_dense_out" if name else None,
+                name="dense_out" if name else None,
                 dtype=self.dtype,
             )
         )
 
     def call(self, inputs) -> tf.Tensor:
         x = tf.concat(inputs, axis=1)
-        out = self._model(x)
-        return out
+        for layer in self._seq:
+            x = layer(x)
+        return x
 
     @property
     def output_dim(self) -> int:
         return self._output_dim
 
     @property
     def latent_dim(self) -> int:
```

### Comparing `pidgan-0.0.1/src/pidgan/players/generators/Generator.py` & `pidgan-0.0.2/src/pidgan/players/generators/Generator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import tensorflow as tf
 from tensorflow.keras.layers import Dense, Dropout, LeakyReLU
 
 LEAKY_ALPHA = 0.1
+SEED = 42
 
 
 class Generator(tf.keras.Model):
     def __init__(
         self,
         output_dim,
         latent_dim,
@@ -57,51 +58,55 @@
                 assert rate >= 0.0 and rate < 1.0
                 self._dropout_rate.append(float(rate))
 
         # Output activation
         self._output_activation = output_activation
 
         # Model
-        self._model = tf.keras.Sequential()
+        self._seq = list()
         for i, (units, rate) in enumerate(
             zip(self._mlp_hidden_units, self._dropout_rate)
         ):
-            self._model.add(
+            self._seq.append(
                 Dense(
                     units=units,
                     activation=None,
                     kernel_initializer="glorot_uniform",
                     bias_initializer="zeros",
-                    name=f"gen_dense_{i}" if name else None,
+                    name=f"dense_{i}" if name else None,
                     dtype=self.dtype,
                 )
             )
-            self._model.add(LeakyReLU(alpha=LEAKY_ALPHA))
-            self._model.add(Dropout(rate=rate))
-        self._model.add(
+            self._seq.append(
+                LeakyReLU(alpha=LEAKY_ALPHA, name=f"leaky_relu_{i}" if name else None)
+            )
+            self._seq.append(Dropout(rate=rate, name=f"dropout_{i}" if name else None))
+        self._seq.append(
             Dense(
                 units=output_dim,
                 activation=output_activation,
                 kernel_initializer="glorot_uniform",
                 bias_initializer="zeros",
-                name="gen_dense_out" if name else None,
+                name="dense_out" if name else None,
                 dtype=self.dtype,
             )
         )
 
     def call(self, x) -> tf.Tensor:
         x = self._prepare_input(x, seed=None)
-        out = self._model(x)
-        tf.print("shape:", tf.shape(out))
-        return out
+        for layer in self._seq:
+            x = layer(x)
+        return x
 
     def generate(self, x, seed=None) -> tf.Tensor:
+        tf.random.set_seed(seed=SEED)
         x = self._prepare_input(x, seed=seed)
-        out = self._model(x)
-        return out
+        for layer in self._seq:
+            x = layer(x)
+        return x
 
     def _prepare_input(self, x, seed=None) -> tf.Tensor:
         latent_sample = tf.random.normal(
             shape=(tf.shape(x)[0], self._latent_dim),
             mean=0.0,
             stddev=1.0,
             dtype=self.dtype,
@@ -129,11 +134,7 @@
     @property
     def dropout_rate(self) -> list:
         return self._dropout_rate
 
     @property
     def output_activation(self):
         return self._output_activation
-
-    @property
-    def model(self) -> tf.keras.Model:
-        return self._model
```

### Comparing `pidgan-0.0.1/src/pidgan/utils/checks/checkMetrics.py` & `pidgan-0.0.2/src/pidgan/utils/checks/checkMetrics.py`

 * *Files identical despite different names*

### Comparing `pidgan-0.0.1/src/pidgan/utils/checks/checkOptimizer.py` & `pidgan-0.0.2/src/pidgan/utils/checks/checkOptimizer.py`

 * *Files identical despite different names*

### Comparing `pidgan-0.0.1/src/pidgan.egg-info/PKG-INFO` & `pidgan-0.0.2/src/pidgan.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pidgan
-Version: 0.0.1
+Version: 0.0.2
 Summary: GAN-based models to fast-simulate the LHCb PID detectors
 Author-email: Matteo Barbetti <matteo.barbetti@fi.infn.it>, Lucio Anderlini <lucio.anderlini@fi.infn.it>
 License: GPLv3 License
 Project-URL: repository, https://github.com/mbarbetti/pidgan
 Keywords: tensorflow,machine learning,deep learning,generative adversarial nets,lhcb experiment,lamarr,ultra-fast simulation,particle identification
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -35,17 +35,15 @@
 </h2>
 
 <p align="center">
   <a href="https://www.tensorflow.org/versions"><img alt="TensorFlow versions" src="https://img.shields.io/badge/tensorflow-2.7–2.12-f57000?style=flat"></a>
   <a href="https://scikit-learn.org/stable/whats_new.html"><img alt="scikit-learn versions" src="https://img.shields.io/badge/sklearn-1.0–1.2-f89939?style=flat"></a>
   <a href="https://www.python.org/downloads"><img alt="Python versions" src="https://img.shields.io/badge/python-3.7–3.11-blue?style=flat"></a>
   <a href="https://pypi.python.org/pypi/pidgan"><img alt="PyPI - Version" src="https://img.shields.io/pypi/v/pidgan"></a>
-  <!--
   <a href="LICENSE"><img alt="GitHub - License" src="https://img.shields.io/github/license/mbarbetti/pidgan"></a>
-  -->
 </p>
 
 <p align="center">
   <a href="https://github.com/mbarbetti/pidgan/actions/workflows/tests.yml"><img alt="GitHub - Tests" src="https://github.com/mbarbetti/pidgan/actions/workflows/tests.yml/badge.svg?branch=main"></a>
   <a href="https://codecov.io/gh/mbarbetti/pidgan"><img alt="Codecov" src="https://codecov.io/gh/mbarbetti/pidgan/branch/main/graph/badge.svg?token=ZLWDgWhnkq"></a>
 </p>
 
@@ -56,18 +54,24 @@
 
 <!--
 [![Docker - Version](https://img.shields.io/docker/v/mbarbetti/pidgan?label=docker)](https://hub.docker.com/r/mbarbetti/pidgan)
 -->
 
 ### Generative Adversarial Networks
 
-| Algorithms | Implementation |  Test  |                         Paper                        |
-|:----------:|:--------------:|:------:|:----------------------------------------------------:|
-|    `GAN`   |       ✅       |   ✅   |  [arXiv:1406.2661](https://arxiv.org/abs/1406.2661)  |
-|  `BceGAN`  |       ✅       |   ✅   |                                                      |
-|   `LSGAN`  |       ✅       |   ✅   | [arXiv:1611.04076](https://arxiv.org/abs/1611.04076) |
-|   `WGAN`   |       ✅       |   ✅   | [arXiv:1701.07875](https://arxiv.org/abs/1701.07875) |
-|  `WGAN_GP` |       ✅       |   ✅   | [arXiv:1704.00028](https://arxiv.org/abs/1704.00028) |
-| `CramerGAN`|       ✅       |   ✅   | [arXiv:1705.10743](https://arxiv.org/abs/1705.10743) |
-| `WGAN_ALP` |       ✅       |   ✅   | [arXiv:1907.05681](https://arxiv.org/abs/1907.05681) |
+| Algorithms* | Implementation |  Test  |                         Paper                        |
+|:-----------:|:--------------:|:------:|:----------------------------------------------------:|
+|    `GAN`    |       ✅       |   ✅   |  [arXiv:1406.2661](https://arxiv.org/abs/1406.2661)  |
+|  `BceGAN`   |       ✅       |   ✅   |                                                      |
+|   `LSGAN`   |       ✅       |   ✅   | [arXiv:1611.04076](https://arxiv.org/abs/1611.04076) |
+|   `WGAN`    |       ✅       |   ✅   | [arXiv:1701.07875](https://arxiv.org/abs/1701.07875) |
+|  `WGAN_GP`  |       ✅       |   ✅   | [arXiv:1704.00028](https://arxiv.org/abs/1704.00028) |
+| `CramerGAN` |       ✅       |   ✅   | [arXiv:1705.10743](https://arxiv.org/abs/1705.10743) |
+| `WGAN_ALP`  |       ✅       |   ✅   | [arXiv:1907.05681](https://arxiv.org/abs/1907.05681) |
 
-*All the algorithms available are designed to operate according to the **conditional version** proposed in [arXiv:1411.1784](https://arxiv.org/abs/1411.1784)
+*Designed to operate according to the **conditional version** proposed in [arXiv:1411.1784](https://arxiv.org/abs/1411.1784)
+
+<!--
+#### Some tricks:
+* [arXiv:1606.03498](https://arxiv.org/abs/1606.03498)
+* [arXiv:1701.04862](https://arxiv.org/abs/1701.04862)
+-->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pidgan Version: 0.0.1 Summary: GAN-based models to
+Metadata-Version: 2.1 Name: pidgan Version: 0.0.2 Summary: GAN-based models to
 fast-simulate the LHCb PID detectors Author-email: Matteo Barbetti
 barbetti@fi.infn.it>, Lucio Anderlini
 anderlini@fi.infn.it> License: GPLv3 License Project-URL: repository, https://
 github.com/mbarbetti/pidgan Keywords: tensorflow,machine learning,deep
 learning,generative adversarial nets,lhcb experiment,lamarr,ultra-fast
 simulation,particle identification Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
@@ -12,21 +12,21 @@
 Language :: Python :: 3.11 Classifier: Topic :: Scientific/Engineering ::
 Physics Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: <=3.11,>=3.7 Description-Content-Type: text/markdown Provides-
 Extra: lamarr Provides-Extra: style Provides-Extra: tests License-File: LICENSE
                              ****** PIDGAN ******
      ***** GAN-based models to fast-simulate the LHCb PID detectors *****
     [TensorFlow_versions] [scikit-learn_versions] [Python_versions] [PyPI_-
-                                   Version]
+                          Version] [GitHub_-_License]
                           [GitHub_-_Tests] [Codecov]
                      [GitHub_-_Style] [Code_style:_black]
- ### Generative Adversarial Networks | Algorithms | Implementation | Test |
-Paper | |:----------:|:--------------:|:------:|:------------------------------
-----------------------:| | `GAN` | â | â | [arXiv:1406.2661](https://
+ ### Generative Adversarial Networks | Algorithms* | Implementation | Test |
+Paper | |:-----------:|:--------------:|:------:|:-----------------------------
+-----------------------:| | `GAN` | â | â | [arXiv:1406.2661](https://
 arxiv.org/abs/1406.2661) | | `BceGAN` | â | â | | | `LSGAN` | â | â |
 [arXiv:1611.04076](https://arxiv.org/abs/1611.04076) | | `WGAN` | â | â |
 [arXiv:1701.07875](https://arxiv.org/abs/1701.07875) | | `WGAN_GP` | â | â
-| [arXiv:1704.00028](https://arxiv.org/abs/1704.00028) | | `CramerGAN`| â |
+| [arXiv:1704.00028](https://arxiv.org/abs/1704.00028) | | `CramerGAN` | â |
 â | [arXiv:1705.10743](https://arxiv.org/abs/1705.10743) | | `WGAN_ALP` | â
-| â | [arXiv:1907.05681](https://arxiv.org/abs/1907.05681) | *All the
-algorithms available are designed to operate according to the **conditional
-version** proposed in [arXiv:1411.1784](https://arxiv.org/abs/1411.1784)
+| â | [arXiv:1907.05681](https://arxiv.org/abs/1907.05681) | *Designed to
+operate according to the **conditional version** proposed in [arXiv:1411.1784]
+(https://arxiv.org/abs/1411.1784)
```

