# Comparing `tmp/composer-0.14.1.tar.gz` & `tmp/composer-0.15.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composer-0.14.1.tar", last modified: Fri May  5 05:53:21 2023, max compression
+gzip compressed data, was "composer-0.15.0.tar", last modified: Tue Jun 20 19:10:26 2023, max compression
```

## Comparing `composer-0.14.1.tar` & `composer-0.15.0.tar`

### file list

```diff
@@ -1,341 +1,341 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.599103 composer-0.14.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10770 2023-05-05 05:53:05.000000 composer-0.14.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-05 05:53:05.000000 composer-0.14.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20919 2023-05-05 05:53:21.599103 composer-0.14.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20530 2023-05-05 05:53:05.000000 composer-0.14.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.527102 composer-0.14.1/composer/
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-05 05:53:05.000000 composer-0.14.1/composer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-05 05:53:05.000000 composer-0.14.1/composer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-05 05:53:05.000000 composer-0.14.1/composer/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.527102 composer-0.14.1/composer/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.527102 composer-0.14.1/composer/algorithms/alibi/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/alibi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/alibi/alibi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.527102 composer-0.14.1/composer/algorithms/alibi/attention_surgery_functions/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/alibi/attention_surgery_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8143 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/alibi/attention_surgery_functions/_bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/alibi/attention_surgery_functions/_gpt2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10272 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/alibi/attention_surgery_functions/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/alibi/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.531102 composer-0.14.1/composer/algorithms/augmix/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/augmix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12071 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/augmix/augmix.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/augmix/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.531102 composer-0.14.1/composer/algorithms/blurpool/
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/blurpool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/blurpool/blurpool.py
--rw-r--r--   0 runner    (1001) docker     (123)    13476 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/blurpool/blurpool_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/blurpool/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.531102 composer-0.14.1/composer/algorithms/channels_last/
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/channels_last/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/channels_last/channels_last.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/channels_last/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.535102 composer-0.14.1/composer/algorithms/colout/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/colout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13854 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/colout/colout.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/colout/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.535102 composer-0.14.1/composer/algorithms/cutmix/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/cutmix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17450 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/cutmix/cutmix.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/cutmix/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.535102 composer-0.14.1/composer/algorithms/cutout/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/cutout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/cutout/cutout.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/cutout/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.535102 composer-0.14.1/composer/algorithms/ema/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/ema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22128 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/ema/ema.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/ema/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.539102 composer-0.14.1/composer/algorithms/factorize/
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/factorize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12723 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/factorize/factorize.py
--rw-r--r--   0 runner    (1001) docker     (123)    15567 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/factorize/factorize_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    22318 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/factorize/factorize_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/factorize/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.539102 composer-0.14.1/composer/algorithms/fused_layernorm/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/fused_layernorm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/fused_layernorm/fused_layernorm.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/fused_layernorm/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.539102 composer-0.14.1/composer/algorithms/gated_linear_units/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/gated_linear_units/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/gated_linear_units/gated_linear_unit_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10310 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/gated_linear_units/gated_linear_units.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/gated_linear_units/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.539102 composer-0.14.1/composer/algorithms/ghost_batchnorm/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/ghost_batchnorm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/ghost_batchnorm/ghost_batchnorm.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/ghost_batchnorm/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.539102 composer-0.14.1/composer/algorithms/gradient_clipping/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/gradient_clipping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10785 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/gradient_clipping/gradient_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/gradient_clipping/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.539102 composer-0.14.1/composer/algorithms/gyro_dropout/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/gyro_dropout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/gyro_dropout/gyro_dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/gyro_dropout/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.543102 composer-0.14.1/composer/algorithms/label_smoothing/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/label_smoothing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/label_smoothing/label_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/label_smoothing/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.543102 composer-0.14.1/composer/algorithms/layer_freezing/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/layer_freezing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/layer_freezing/layer_freezing.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/layer_freezing/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.543102 composer-0.14.1/composer/algorithms/low_precision_groupnorm/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/low_precision_groupnorm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/low_precision_groupnorm/low_precision_groupnorm.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/low_precision_groupnorm/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.543102 composer-0.14.1/composer/algorithms/low_precision_layernorm/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/low_precision_layernorm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/low_precision_layernorm/low_precision_layernorm.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/low_precision_layernorm/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.547102 composer-0.14.1/composer/algorithms/mixup/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/mixup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/mixup/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     9983 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/mixup/mixup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.547102 composer-0.14.1/composer/algorithms/no_op_model/
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/no_op_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/no_op_model/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/no_op_model/no_op_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.547102 composer-0.14.1/composer/algorithms/progressive_resizing/
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/progressive_resizing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/progressive_resizing/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)    13610 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/progressive_resizing/progressive_resizing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.547102 composer-0.14.1/composer/algorithms/randaugment/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/randaugment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/randaugment/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     8973 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/randaugment/randaugment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.547102 composer-0.14.1/composer/algorithms/sam/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/sam/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/sam/sam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.551102 composer-0.14.1/composer/algorithms/selective_backprop/
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/selective_backprop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/selective_backprop/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/selective_backprop/selective_backprop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.551102 composer-0.14.1/composer/algorithms/seq_length_warmup/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/seq_length_warmup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/seq_length_warmup/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)    18808 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/seq_length_warmup/seq_length_warmup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.551102 composer-0.14.1/composer/algorithms/squeeze_excite/
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/squeeze_excite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/squeeze_excite/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     8294 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/squeeze_excite/squeeze_excite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.551102 composer-0.14.1/composer/algorithms/stochastic_depth/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/stochastic_depth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/stochastic_depth/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)    12897 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/stochastic_depth/stochastic_depth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/stochastic_depth/stochastic_layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.555102 composer-0.14.1/composer/algorithms/swa/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/swa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/swa/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)    13019 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/swa/swa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.555102 composer-0.14.1/composer/algorithms/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/utils/augmentation_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    11941 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/utils/augmentation_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.555102 composer-0.14.1/composer/algorithms/weight_standardization/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/weight_standardization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/weight_standardization/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-05-05 05:53:05.000000 composer-0.14.1/composer/algorithms/weight_standardization/weight_standardization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.559102 composer-0.14.1/composer/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-05 05:53:05.000000 composer-0.14.1/composer/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13162 2023-05-05 05:53:05.000000 composer-0.14.1/composer/callbacks/activation_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    20164 2023-05-05 05:53:05.000000 composer-0.14.1/composer/callbacks/checkpoint_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-05-05 05:53:05.000000 composer-0.14.1/composer/callbacks/early_stopper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-05-05 05:53:05.000000 composer-0.14.1/composer/callbacks/export_for_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-05-05 05:53:05.000000 composer-0.14.1/composer/callbacks/health_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-05-05 05:53:05.000000 composer-0.14.1/composer/callbacks/image_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-05 05:53:05.000000 composer-0.14.1/composer/callbacks/lr_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-05-05 05:53:05.000000 composer-0.14.1/composer/callbacks/memory_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17918 2023-05-05 05:53:05.000000 composer-0.14.1/composer/callbacks/mlperf.py
--rw-r--r--   0 runner    (1001) docker     (123)     9106 2023-05-05 05:53:05.000000 composer-0.14.1/composer/callbacks/optimizer_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-05-05 05:53:05.000000 composer-0.14.1/composer/callbacks/runtime_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)    16013 2023-05-05 05:53:05.000000 composer-0.14.1/composer/callbacks/speed_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-05-05 05:53:05.000000 composer-0.14.1/composer/callbacks/threshold_stopper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.559102 composer-0.14.1/composer/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-05 05:53:05.000000 composer-0.14.1/composer/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-05 05:53:05.000000 composer-0.14.1/composer/cli/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21453 2023-05-05 05:53:05.000000 composer-0.14.1/composer/cli/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.563102 composer-0.14.1/composer/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-05 05:53:05.000000 composer-0.14.1/composer/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-05-05 05:53:05.000000 composer-0.14.1/composer/core/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)    15030 2023-05-05 05:53:05.000000 composer-0.14.1/composer/core/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)    15029 2023-05-05 05:53:05.000000 composer-0.14.1/composer/core/data_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    24030 2023-05-05 05:53:05.000000 composer-0.14.1/composer/core/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    13340 2023-05-05 05:53:05.000000 composer-0.14.1/composer/core/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9510 2023-05-05 05:53:05.000000 composer-0.14.1/composer/core/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-05 05:53:05.000000 composer-0.14.1/composer/core/passes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-05-05 05:53:05.000000 composer-0.14.1/composer/core/precision.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-05 05:53:05.000000 composer-0.14.1/composer/core/serializable.py
--rw-r--r--   0 runner    (1001) docker     (123)    67948 2023-05-05 05:53:05.000000 composer-0.14.1/composer/core/state.py
--rw-r--r--   0 runner    (1001) docker     (123)    30173 2023-05-05 05:53:05.000000 composer-0.14.1/composer/core/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-05 05:53:05.000000 composer-0.14.1/composer/core/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.567102 composer-0.14.1/composer/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-05 05:53:05.000000 composer-0.14.1/composer/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24316 2023-05-05 05:53:05.000000 composer-0.14.1/composer/datasets/ade20k.py
--rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-05-05 05:53:05.000000 composer-0.14.1/composer/datasets/brats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-05-05 05:53:05.000000 composer-0.14.1/composer/datasets/c4.py
--rw-r--r--   0 runner    (1001) docker     (123)    13545 2023-05-05 05:53:05.000000 composer-0.14.1/composer/datasets/cifar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-05-05 05:53:05.000000 composer-0.14.1/composer/datasets/ffcv_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15042 2023-05-05 05:53:05.000000 composer-0.14.1/composer/datasets/imagenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    51670 2023-05-05 05:53:05.000000 composer-0.14.1/composer/datasets/in_context_learning_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-05-05 05:53:05.000000 composer-0.14.1/composer/datasets/lm_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-05-05 05:53:05.000000 composer-0.14.1/composer/datasets/mnist.py
--rw-r--r--   0 runner    (1001) docker     (123)    10213 2023-05-05 05:53:05.000000 composer-0.14.1/composer/datasets/synthetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-05-05 05:53:05.000000 composer-0.14.1/composer/datasets/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.567102 composer-0.14.1/composer/devices/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-05 05:53:05.000000 composer-0.14.1/composer/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-05-05 05:53:05.000000 composer-0.14.1/composer/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-05 05:53:05.000000 composer-0.14.1/composer/devices/device_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-05 05:53:05.000000 composer-0.14.1/composer/devices/device_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-05 05:53:05.000000 composer-0.14.1/composer/devices/device_mps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-05 05:53:05.000000 composer-0.14.1/composer/devices/device_tpu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.567102 composer-0.14.1/composer/functional/
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-05 05:53:05.000000 composer-0.14.1/composer/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.571102 composer-0.14.1/composer/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-05 05:53:05.000000 composer-0.14.1/composer/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9919 2023-05-05 05:53:05.000000 composer-0.14.1/composer/loggers/cometml_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     9322 2023-05-05 05:53:05.000000 composer-0.14.1/composer/loggers/console_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    11327 2023-05-05 05:53:05.000000 composer-0.14.1/composer/loggers/file_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-05-05 05:53:05.000000 composer-0.14.1/composer/loggers/in_memory_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-05-05 05:53:05.000000 composer-0.14.1/composer/loggers/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-05-05 05:53:05.000000 composer-0.14.1/composer/loggers/logger_destination.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-05 05:53:05.000000 composer-0.14.1/composer/loggers/mlflow_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-05-05 05:53:05.000000 composer-0.14.1/composer/loggers/mosaicml_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    15412 2023-05-05 05:53:05.000000 composer-0.14.1/composer/loggers/progress_bar_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    28802 2023-05-05 05:53:05.000000 composer-0.14.1/composer/loggers/remote_uploader_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9435 2023-05-05 05:53:05.000000 composer-0.14.1/composer/loggers/slack_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-05-05 05:53:05.000000 composer-0.14.1/composer/loggers/tensorboard_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    16974 2023-05-05 05:53:05.000000 composer-0.14.1/composer/loggers/wandb_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.575102 composer-0.14.1/composer/loss/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-05 05:53:05.000000 composer-0.14.1/composer/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-05-05 05:53:05.000000 composer-0.14.1/composer/loss/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-05-05 05:53:05.000000 composer-0.14.1/composer/loss/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.575102 composer-0.14.1/composer/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-05 05:53:05.000000 composer-0.14.1/composer/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16851 2023-05-05 05:53:05.000000 composer-0.14.1/composer/metrics/map.py
--rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-05-05 05:53:05.000000 composer-0.14.1/composer/metrics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    25727 2023-05-05 05:53:05.000000 composer-0.14.1/composer/metrics/nlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.575102 composer-0.14.1/composer/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9343 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.575102 composer-0.14.1/composer/models/bert/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/bert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/bert/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.575102 composer-0.14.1/composer/models/classify_mnist/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/classify_mnist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/classify_mnist/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.575102 composer-0.14.1/composer/models/deeplabv3/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/deeplabv3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11560 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/deeplabv3/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.579102 composer-0.14.1/composer/models/efficientnetb0/
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/efficientnetb0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9915 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/efficientnetb0/_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/efficientnetb0/efficientnets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/efficientnetb0/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.579102 composer-0.14.1/composer/models/gpt2/
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/gpt2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/gpt2/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    34533 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/initializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/mmdetection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.579102 composer-0.14.1/composer/models/resnet/
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/resnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6058 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/resnet/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.579102 composer-0.14.1/composer/models/resnet_cifar/
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/resnet_cifar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/resnet_cifar/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/resnet_cifar/resnets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.579102 composer-0.14.1/composer/models/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/tasks/classification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.579102 composer-0.14.1/composer/models/timm/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/timm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/timm/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.583102 composer-0.14.1/composer/models/unet/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/unet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/unet/_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/unet/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/unet/unet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.583102 composer-0.14.1/composer/models/vit_small_patch16/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/vit_small_patch16/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-05-05 05:53:05.000000 composer-0.14.1/composer/models/vit_small_patch16/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.583102 composer-0.14.1/composer/optim/
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-05-05 05:53:05.000000 composer-0.14.1/composer/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20226 2023-05-05 05:53:05.000000 composer-0.14.1/composer/optim/decoupled_weight_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)    35768 2023-05-05 05:53:05.000000 composer-0.14.1/composer/optim/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.587103 composer-0.14.1/composer/profiler/
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-05 05:53:05.000000 composer-0.14.1/composer/profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20858 2023-05-05 05:53:05.000000 composer-0.14.1/composer/profiler/json_trace_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-05-05 05:53:05.000000 composer-0.14.1/composer/profiler/json_trace_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-05-05 05:53:05.000000 composer-0.14.1/composer/profiler/marker.py
--rw-r--r--   0 runner    (1001) docker     (123)    11455 2023-05-05 05:53:05.000000 composer-0.14.1/composer/profiler/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-05 05:53:05.000000 composer-0.14.1/composer/profiler/profiler_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-05-05 05:53:05.000000 composer-0.14.1/composer/profiler/profiler_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-05-05 05:53:05.000000 composer-0.14.1/composer/profiler/system_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-05-05 05:53:05.000000 composer-0.14.1/composer/profiler/torch_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-05-05 05:53:05.000000 composer-0.14.1/composer/profiler/trace_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:05.000000 composer-0.14.1/composer/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.587103 composer-0.14.1/composer/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-05 05:53:05.000000 composer-0.14.1/composer/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-05-05 05:53:05.000000 composer-0.14.1/composer/trainer/_deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-05 05:53:05.000000 composer-0.14.1/composer/trainer/_scale_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-05-05 05:53:05.000000 composer-0.14.1/composer/trainer/_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)    23655 2023-05-05 05:53:05.000000 composer-0.14.1/composer/trainer/dist_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-05 05:53:05.000000 composer-0.14.1/composer/trainer/meta_safe_apply.py
--rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-05-05 05:53:05.000000 composer-0.14.1/composer/trainer/mosaic_fsdp.py
--rw-r--r--   0 runner    (1001) docker     (123)   153175 2023-05-05 05:53:05.000000 composer-0.14.1/composer/trainer/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.591102 composer-0.14.1/composer/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/auto_log_hparams.py
--rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/batch_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    30139 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    15335 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/collect_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    19867 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/file_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13407 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/fx_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/import_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15248 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/iter_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    18748 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/module_surgery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.595102 composer-0.14.1/composer/utils/object_store/
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/object_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8534 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/object_store/libcloud_object_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/object_store/object_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/object_store/oci_object_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     7268 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/object_store/s3_object_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    12144 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/object_store/sftp_object_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/reproducibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/retrying.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-05 05:53:05.000000 composer-0.14.1/composer/utils/string_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.527102 composer-0.14.1/composer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20919 2023-05-05 05:53:21.000000 composer-0.14.1/composer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-05-05 05:53:21.000000 composer-0.14.1/composer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-05 05:53:21.000000 composer-0.14.1/composer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-05 05:53:21.000000 composer-0.14.1/composer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-05-05 05:53:21.000000 composer-0.14.1/composer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 05:53:21.000000 composer-0.14.1/composer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    34985 2023-05-05 05:53:05.000000 composer-0.14.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 05:53:21.599103 composer-0.14.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-05-05 05:53:05.000000 composer-0.14.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:53:21.599103 composer-0.14.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-05 05:53:05.000000 composer-0.14.1/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-05 05:53:05.000000 composer-0.14.1/tests/test_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-05-05 05:53:05.000000 composer-0.14.1/tests/test_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-05-05 05:53:05.000000 composer-0.14.1/tests/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-05-05 05:53:05.000000 composer-0.14.1/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)    13253 2023-05-05 05:53:05.000000 composer-0.14.1/tests/test_full_nlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-05-05 05:53:05.000000 composer-0.14.1/tests/test_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-05-05 05:53:05.000000 composer-0.14.1/tests/test_notebooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-05-05 05:53:05.000000 composer-0.14.1/tests/test_passes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-05 05:53:05.000000 composer-0.14.1/tests/test_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-05-05 05:53:05.000000 composer-0.14.1/tests/test_simple_nlp.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-05 05:53:05.000000 composer-0.14.1/tests/test_smoketest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-05-05 05:53:05.000000 composer-0.14.1/tests/test_split_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-05-05 05:53:05.000000 composer-0.14.1/tests/test_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-05-05 05:53:05.000000 composer-0.14.1/tests/test_time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.810140 composer-0.15.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10770 2023-06-20 19:10:12.000000 composer-0.15.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-20 19:10:12.000000 composer-0.15.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20831 2023-06-20 19:10:26.810140 composer-0.15.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20463 2023-06-20 19:10:12.000000 composer-0.15.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.774140 composer-0.15.0/composer/
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-20 19:10:12.000000 composer-0.15.0/composer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-20 19:10:12.000000 composer-0.15.0/composer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-20 19:10:12.000000 composer-0.15.0/composer/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.774140 composer-0.15.0/composer/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.774140 composer-0.15.0/composer/algorithms/alibi/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/alibi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/alibi/alibi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.774140 composer-0.15.0/composer/algorithms/alibi/attention_surgery_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/alibi/attention_surgery_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8143 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/alibi/attention_surgery_functions/_bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/alibi/attention_surgery_functions/_gpt2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10272 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/alibi/attention_surgery_functions/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/alibi/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.778140 composer-0.15.0/composer/algorithms/augmix/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/augmix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12071 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/augmix/augmix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/augmix/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.778140 composer-0.15.0/composer/algorithms/blurpool/
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/blurpool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/blurpool/blurpool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13476 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/blurpool/blurpool_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/blurpool/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.778140 composer-0.15.0/composer/algorithms/channels_last/
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/channels_last/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/channels_last/channels_last.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/channels_last/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.778140 composer-0.15.0/composer/algorithms/colout/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/colout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13854 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/colout/colout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/colout/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.778140 composer-0.15.0/composer/algorithms/cutmix/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/cutmix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17450 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/cutmix/cutmix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/cutmix/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.778140 composer-0.15.0/composer/algorithms/cutout/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/cutout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/cutout/cutout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/cutout/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.778140 composer-0.15.0/composer/algorithms/ema/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/ema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22128 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/ema/ema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/ema/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.778140 composer-0.15.0/composer/algorithms/factorize/
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/factorize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12723 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/factorize/factorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15567 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/factorize/factorize_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22318 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/factorize/factorize_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/factorize/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.782140 composer-0.15.0/composer/algorithms/fused_layernorm/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/fused_layernorm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/fused_layernorm/fused_layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/fused_layernorm/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.782140 composer-0.15.0/composer/algorithms/gated_linear_units/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/gated_linear_units/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/gated_linear_units/gated_linear_unit_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10310 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/gated_linear_units/gated_linear_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/gated_linear_units/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.782140 composer-0.15.0/composer/algorithms/ghost_batchnorm/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/ghost_batchnorm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/ghost_batchnorm/ghost_batchnorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/ghost_batchnorm/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.782140 composer-0.15.0/composer/algorithms/gradient_clipping/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/gradient_clipping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10785 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/gradient_clipping/gradient_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/gradient_clipping/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.782140 composer-0.15.0/composer/algorithms/gyro_dropout/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/gyro_dropout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/gyro_dropout/gyro_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/gyro_dropout/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.782140 composer-0.15.0/composer/algorithms/label_smoothing/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/label_smoothing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/label_smoothing/label_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/label_smoothing/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.782140 composer-0.15.0/composer/algorithms/layer_freezing/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/layer_freezing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/layer_freezing/layer_freezing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/layer_freezing/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.782140 composer-0.15.0/composer/algorithms/low_precision_groupnorm/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/low_precision_groupnorm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/low_precision_groupnorm/low_precision_groupnorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/low_precision_groupnorm/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.782140 composer-0.15.0/composer/algorithms/low_precision_layernorm/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/low_precision_layernorm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/low_precision_layernorm/low_precision_layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/low_precision_layernorm/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.782140 composer-0.15.0/composer/algorithms/mixup/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/mixup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/mixup/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9983 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/mixup/mixup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.786140 composer-0.15.0/composer/algorithms/no_op_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/no_op_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/no_op_model/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/no_op_model/no_op_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.786140 composer-0.15.0/composer/algorithms/progressive_resizing/
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/progressive_resizing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/progressive_resizing/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13610 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/progressive_resizing/progressive_resizing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.786140 composer-0.15.0/composer/algorithms/randaugment/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/randaugment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/randaugment/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8973 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/randaugment/randaugment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.786140 composer-0.15.0/composer/algorithms/sam/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/sam/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/sam/sam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.786140 composer-0.15.0/composer/algorithms/selective_backprop/
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/selective_backprop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/selective_backprop/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/selective_backprop/selective_backprop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.786140 composer-0.15.0/composer/algorithms/seq_length_warmup/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/seq_length_warmup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/seq_length_warmup/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19203 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/seq_length_warmup/seq_length_warmup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.786140 composer-0.15.0/composer/algorithms/squeeze_excite/
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/squeeze_excite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/squeeze_excite/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8294 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/squeeze_excite/squeeze_excite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.786140 composer-0.15.0/composer/algorithms/stochastic_depth/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/stochastic_depth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/stochastic_depth/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12897 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/stochastic_depth/stochastic_depth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/stochastic_depth/stochastic_layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.786140 composer-0.15.0/composer/algorithms/swa/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/swa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/swa/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13019 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/swa/swa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.790140 composer-0.15.0/composer/algorithms/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/utils/augmentation_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11941 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/utils/augmentation_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.790140 composer-0.15.0/composer/algorithms/weight_standardization/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/weight_standardization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/weight_standardization/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-06-20 19:10:12.000000 composer-0.15.0/composer/algorithms/weight_standardization/weight_standardization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.790140 composer-0.15.0/composer/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-20 19:10:12.000000 composer-0.15.0/composer/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13162 2023-06-20 19:10:12.000000 composer-0.15.0/composer/callbacks/activation_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21076 2023-06-20 19:10:12.000000 composer-0.15.0/composer/callbacks/checkpoint_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-06-20 19:10:12.000000 composer-0.15.0/composer/callbacks/early_stopper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-06-20 19:10:12.000000 composer-0.15.0/composer/callbacks/export_for_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-06-20 19:10:12.000000 composer-0.15.0/composer/callbacks/health_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-06-20 19:10:12.000000 composer-0.15.0/composer/callbacks/image_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-06-20 19:10:12.000000 composer-0.15.0/composer/callbacks/lr_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-06-20 19:10:12.000000 composer-0.15.0/composer/callbacks/memory_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17924 2023-06-20 19:10:12.000000 composer-0.15.0/composer/callbacks/mlperf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9106 2023-06-20 19:10:12.000000 composer-0.15.0/composer/callbacks/optimizer_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-06-20 19:10:12.000000 composer-0.15.0/composer/callbacks/runtime_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16084 2023-06-20 19:10:12.000000 composer-0.15.0/composer/callbacks/speed_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-06-20 19:10:12.000000 composer-0.15.0/composer/callbacks/threshold_stopper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.790140 composer-0.15.0/composer/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-20 19:10:12.000000 composer-0.15.0/composer/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-20 19:10:12.000000 composer-0.15.0/composer/cli/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21453 2023-06-20 19:10:12.000000 composer-0.15.0/composer/cli/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.794140 composer-0.15.0/composer/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-20 19:10:12.000000 composer-0.15.0/composer/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-06-20 19:10:12.000000 composer-0.15.0/composer/core/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15622 2023-06-20 19:10:12.000000 composer-0.15.0/composer/core/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14725 2023-06-20 19:10:12.000000 composer-0.15.0/composer/core/data_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24030 2023-06-20 19:10:12.000000 composer-0.15.0/composer/core/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13340 2023-06-20 19:10:12.000000 composer-0.15.0/composer/core/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-06-20 19:10:12.000000 composer-0.15.0/composer/core/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-06-20 19:10:12.000000 composer-0.15.0/composer/core/passes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-06-20 19:10:12.000000 composer-0.15.0/composer/core/precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-20 19:10:12.000000 composer-0.15.0/composer/core/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74169 2023-06-20 19:10:12.000000 composer-0.15.0/composer/core/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30173 2023-06-20 19:10:12.000000 composer-0.15.0/composer/core/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-06-20 19:10:12.000000 composer-0.15.0/composer/core/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.794140 composer-0.15.0/composer/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-20 19:10:12.000000 composer-0.15.0/composer/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24316 2023-06-20 19:10:12.000000 composer-0.15.0/composer/datasets/ade20k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-06-20 19:10:12.000000 composer-0.15.0/composer/datasets/brats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-06-20 19:10:12.000000 composer-0.15.0/composer/datasets/c4.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13545 2023-06-20 19:10:12.000000 composer-0.15.0/composer/datasets/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-06-20 19:10:12.000000 composer-0.15.0/composer/datasets/ffcv_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15042 2023-06-20 19:10:12.000000 composer-0.15.0/composer/datasets/imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54555 2023-06-20 19:10:12.000000 composer-0.15.0/composer/datasets/in_context_learning_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-06-20 19:10:12.000000 composer-0.15.0/composer/datasets/lm_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-06-20 19:10:12.000000 composer-0.15.0/composer/datasets/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10213 2023-06-20 19:10:12.000000 composer-0.15.0/composer/datasets/synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-06-20 19:10:12.000000 composer-0.15.0/composer/datasets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.794140 composer-0.15.0/composer/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-20 19:10:12.000000 composer-0.15.0/composer/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-06-20 19:10:12.000000 composer-0.15.0/composer/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-20 19:10:12.000000 composer-0.15.0/composer/devices/device_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-20 19:10:12.000000 composer-0.15.0/composer/devices/device_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-20 19:10:12.000000 composer-0.15.0/composer/devices/device_mps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-20 19:10:12.000000 composer-0.15.0/composer/devices/device_tpu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.794140 composer-0.15.0/composer/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-06-20 19:10:12.000000 composer-0.15.0/composer/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.798140 composer-0.15.0/composer/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-20 19:10:12.000000 composer-0.15.0/composer/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9919 2023-06-20 19:10:12.000000 composer-0.15.0/composer/loggers/cometml_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-06-20 19:10:12.000000 composer-0.15.0/composer/loggers/console_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11327 2023-06-20 19:10:12.000000 composer-0.15.0/composer/loggers/file_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-06-20 19:10:12.000000 composer-0.15.0/composer/loggers/in_memory_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-06-20 19:10:12.000000 composer-0.15.0/composer/loggers/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-06-20 19:10:12.000000 composer-0.15.0/composer/loggers/logger_destination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-20 19:10:12.000000 composer-0.15.0/composer/loggers/mlflow_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-06-20 19:10:12.000000 composer-0.15.0/composer/loggers/mosaicml_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15255 2023-06-20 19:10:12.000000 composer-0.15.0/composer/loggers/progress_bar_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28802 2023-06-20 19:10:12.000000 composer-0.15.0/composer/loggers/remote_uploader_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9435 2023-06-20 19:10:12.000000 composer-0.15.0/composer/loggers/slack_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-06-20 19:10:12.000000 composer-0.15.0/composer/loggers/tensorboard_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17065 2023-06-20 19:10:12.000000 composer-0.15.0/composer/loggers/wandb_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.798140 composer-0.15.0/composer/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-20 19:10:12.000000 composer-0.15.0/composer/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-06-20 19:10:12.000000 composer-0.15.0/composer/loss/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-06-20 19:10:12.000000 composer-0.15.0/composer/loss/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.798140 composer-0.15.0/composer/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-20 19:10:12.000000 composer-0.15.0/composer/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16851 2023-06-20 19:10:12.000000 composer-0.15.0/composer/metrics/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-06-20 19:10:12.000000 composer-0.15.0/composer/metrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21771 2023-06-20 19:10:12.000000 composer-0.15.0/composer/metrics/nlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.798140 composer-0.15.0/composer/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-20 19:10:12.000000 composer-0.15.0/composer/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-06-20 19:10:12.000000 composer-0.15.0/composer/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.798140 composer-0.15.0/composer/models/bert/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-20 19:10:12.000000 composer-0.15.0/composer/models/bert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-06-20 19:10:12.000000 composer-0.15.0/composer/models/bert/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.798140 composer-0.15.0/composer/models/classify_mnist/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-20 19:10:12.000000 composer-0.15.0/composer/models/classify_mnist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-20 19:10:12.000000 composer-0.15.0/composer/models/classify_mnist/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.802140 composer-0.15.0/composer/models/deeplabv3/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-20 19:10:12.000000 composer-0.15.0/composer/models/deeplabv3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11560 2023-06-20 19:10:12.000000 composer-0.15.0/composer/models/deeplabv3/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.802140 composer-0.15.0/composer/models/efficientnetb0/
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-20 19:10:12.000000 composer-0.15.0/composer/models/efficientnetb0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9915 2023-06-20 19:10:12.000000 composer-0.15.0/composer/models/efficientnetb0/_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-06-20 19:10:12.000000 composer-0.15.0/composer/models/efficientnetb0/efficientnets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-20 19:10:12.000000 composer-0.15.0/composer/models/efficientnetb0/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.802140 composer-0.15.0/composer/models/gpt2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-20 19:10:12.000000 composer-0.15.0/composer/models/gpt2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-06-20 19:10:12.000000 composer-0.15.0/composer/models/gpt2/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37930 2023-06-20 19:10:12.000000 composer-0.15.0/composer/models/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-20 19:10:12.000000 composer-0.15.0/composer/models/initializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-06-20 19:10:12.000000 composer-0.15.0/composer/models/mmdetection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.802140 composer-0.15.0/composer/models/resnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-20 19:10:12.000000 composer-0.15.0/composer/models/resnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-06-20 19:10:12.000000 composer-0.15.0/composer/models/resnet/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.802140 composer-0.15.0/composer/models/resnet_cifar/
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-20 19:10:12.000000 composer-0.15.0/composer/models/resnet_cifar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-20 19:10:12.000000 composer-0.15.0/composer/models/resnet_cifar/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-06-20 19:10:12.000000 composer-0.15.0/composer/models/resnet_cifar/resnets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.802140 composer-0.15.0/composer/models/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-20 19:10:12.000000 composer-0.15.0/composer/models/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-06-20 19:10:12.000000 composer-0.15.0/composer/models/tasks/classification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.802140 composer-0.15.0/composer/models/timm/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-20 19:10:12.000000 composer-0.15.0/composer/models/timm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-20 19:10:12.000000 composer-0.15.0/composer/models/timm/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.802140 composer-0.15.0/composer/models/unet/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-20 19:10:12.000000 composer-0.15.0/composer/models/unet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-20 19:10:12.000000 composer-0.15.0/composer/models/unet/_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-06-20 19:10:12.000000 composer-0.15.0/composer/models/unet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-06-20 19:10:12.000000 composer-0.15.0/composer/models/unet/unet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.802140 composer-0.15.0/composer/models/vit_small_patch16/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-20 19:10:12.000000 composer-0.15.0/composer/models/vit_small_patch16/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-06-20 19:10:12.000000 composer-0.15.0/composer/models/vit_small_patch16/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.802140 composer-0.15.0/composer/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-20 19:10:12.000000 composer-0.15.0/composer/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20299 2023-06-20 19:10:12.000000 composer-0.15.0/composer/optim/decoupled_weight_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35768 2023-06-20 19:10:12.000000 composer-0.15.0/composer/optim/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.806140 composer-0.15.0/composer/profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-20 19:10:12.000000 composer-0.15.0/composer/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20858 2023-06-20 19:10:12.000000 composer-0.15.0/composer/profiler/json_trace_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-06-20 19:10:12.000000 composer-0.15.0/composer/profiler/json_trace_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-06-20 19:10:12.000000 composer-0.15.0/composer/profiler/marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11455 2023-06-20 19:10:12.000000 composer-0.15.0/composer/profiler/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-20 19:10:12.000000 composer-0.15.0/composer/profiler/profiler_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-20 19:10:12.000000 composer-0.15.0/composer/profiler/profiler_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-06-20 19:10:12.000000 composer-0.15.0/composer/profiler/system_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-06-20 19:10:12.000000 composer-0.15.0/composer/profiler/torch_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-06-20 19:10:12.000000 composer-0.15.0/composer/profiler/trace_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:12.000000 composer-0.15.0/composer/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.806140 composer-0.15.0/composer/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-20 19:10:12.000000 composer-0.15.0/composer/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-06-20 19:10:12.000000 composer-0.15.0/composer/trainer/_deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-06-20 19:10:12.000000 composer-0.15.0/composer/trainer/_scale_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-06-20 19:10:12.000000 composer-0.15.0/composer/trainer/_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30488 2023-06-20 19:10:12.000000 composer-0.15.0/composer/trainer/dist_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-20 19:10:12.000000 composer-0.15.0/composer/trainer/meta_safe_apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-06-20 19:10:12.000000 composer-0.15.0/composer/trainer/mosaic_fsdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   162446 2023-06-20 19:10:12.000000 composer-0.15.0/composer/trainer/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.810140 composer-0.15.0/composer/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-06-20 19:10:12.000000 composer-0.15.0/composer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-06-20 19:10:12.000000 composer-0.15.0/composer/utils/auto_log_hparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-06-20 19:10:12.000000 composer-0.15.0/composer/utils/batch_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32887 2023-06-20 19:10:12.000000 composer-0.15.0/composer/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15335 2023-06-20 19:10:12.000000 composer-0.15.0/composer/utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-20 19:10:12.000000 composer-0.15.0/composer/utils/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19867 2023-06-20 19:10:12.000000 composer-0.15.0/composer/utils/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28308 2023-06-20 19:10:12.000000 composer-0.15.0/composer/utils/file_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13407 2023-06-20 19:10:12.000000 composer-0.15.0/composer/utils/fx_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-06-20 19:10:12.000000 composer-0.15.0/composer/utils/import_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15248 2023-06-20 19:10:12.000000 composer-0.15.0/composer/utils/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-06-20 19:10:12.000000 composer-0.15.0/composer/utils/iter_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-20 19:10:12.000000 composer-0.15.0/composer/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18748 2023-06-20 19:10:12.000000 composer-0.15.0/composer/utils/module_surgery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.810140 composer-0.15.0/composer/utils/object_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-20 19:10:12.000000 composer-0.15.0/composer/utils/object_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-06-20 19:10:12.000000 composer-0.15.0/composer/utils/object_store/libcloud_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-06-20 19:10:12.000000 composer-0.15.0/composer/utils/object_store/object_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-06-20 19:10:12.000000 composer-0.15.0/composer/utils/object_store/oci_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7382 2023-06-20 19:10:12.000000 composer-0.15.0/composer/utils/object_store/s3_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12144 2023-06-20 19:10:12.000000 composer-0.15.0/composer/utils/object_store/sftp_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-06-20 19:10:12.000000 composer-0.15.0/composer/utils/reproducibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-06-20 19:10:12.000000 composer-0.15.0/composer/utils/retrying.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-06-20 19:10:12.000000 composer-0.15.0/composer/utils/string_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.774140 composer-0.15.0/composer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20831 2023-06-20 19:10:26.000000 composer-0.15.0/composer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-06-20 19:10:26.000000 composer-0.15.0/composer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-20 19:10:26.000000 composer-0.15.0/composer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-20 19:10:26.000000 composer-0.15.0/composer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-06-20 19:10:26.000000 composer-0.15.0/composer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 19:10:26.000000 composer-0.15.0/composer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    34175 2023-06-20 19:10:12.000000 composer-0.15.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 19:10:26.814140 composer-0.15.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-06-20 19:10:12.000000 composer-0.15.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:10:26.810140 composer-0.15.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-06-20 19:10:12.000000 composer-0.15.0/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-20 19:10:12.000000 composer-0.15.0/tests/test_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-06-20 19:10:12.000000 composer-0.15.0/tests/test_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-06-20 19:10:12.000000 composer-0.15.0/tests/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-06-20 19:10:12.000000 composer-0.15.0/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13319 2023-06-20 19:10:12.000000 composer-0.15.0/tests/test_full_nlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-06-20 19:10:12.000000 composer-0.15.0/tests/test_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-06-20 19:10:12.000000 composer-0.15.0/tests/test_notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-06-20 19:10:12.000000 composer-0.15.0/tests/test_passes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-06-20 19:10:12.000000 composer-0.15.0/tests/test_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-06-20 19:10:12.000000 composer-0.15.0/tests/test_simple_nlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-20 19:10:12.000000 composer-0.15.0/tests/test_smoketest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-06-20 19:10:12.000000 composer-0.15.0/tests/test_split_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-06-20 19:10:12.000000 composer-0.15.0/tests/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-06-20 19:10:12.000000 composer-0.15.0/tests/test_time.py
```

### Comparing `composer-0.14.1/LICENSE` & `composer-0.15.0/LICENSE`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/PKG-INFO` & `composer-0.15.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composer
-Version: 0.14.1
+Version: 0.15.0
 Summary: Composer is a PyTorch library that enables you to train neural networks faster, at lower cost, and to higher accuracy.
 Home-page: https://github.com/mosaicml/composer
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -27,15 +27,14 @@
 Provides-Extra: sentencepiece
 Provides-Extra: mlperf
 Provides-Extra: streaming
 Provides-Extra: libcloud
 Provides-Extra: oci
 Provides-Extra: onnx
 Provides-Extra: mlflow
-Provides-Extra: mcli
 Provides-Extra: all
 License-File: LICENSE
 
 <br />
 <p align="center">
     <a href="https://github.com/mosaicml/composer#gh-light-mode-only" class="only-light">
       <img src="https://storage.googleapis.com/docs.mosaicml.com/images/header_light.svg" width="50%"/>
@@ -63,15 +62,15 @@
     </a>
     <a href="https://pepy.tech/project/mosaicml/">
         <img alt="PyPi Downloads" src="https://static.pepy.tech/personalized-badge/mosaicml?period=month&units=international_system&left_color=grey&right_color=blue&left_text=Downloads/month">
     </a>
     <a href="https://docs.mosaicml.com/projects/composer/en/stable/">
         <img alt="Documentation" src="https://readthedocs.org/projects/composer/badge/?version=stable">
     </a>
-    <a href="https://join.slack.com/t/mosaicml-community/shared_invite/zt-w0tiddn9-WGTlRpfjcO9J5jyrMub1dg">
+    <a href="https://mosaicml.me/slack">
         <img alt="Chat @ Slack" src="https://img.shields.io/badge/slack-chat-2eb67d.svg?logo=slack">
     </a>
     <a href="https://github.com/mosaicml/composer/blob/dev/LICENSE">
         <img alt="License" src="https://img.shields.io/badge/License-Apache%202.0-green.svg?logo=slack">
     </a>
 </p>
 <br />
```

#### html2text {}

```diff
@@ -1,22 +1,21 @@
-Metadata-Version: 2.1 Name: composer Version: 0.14.1 Summary: Composer is a
+Metadata-Version: 2.1 Name: composer Version: 0.15.0 Summary: Composer is a
 PyTorch library that enables you to train neural networks faster, at lower
 cost, and to higher accuracy. Home-page: https://github.com/mosaicml/composer
 Author: MosaicML Author-email: team@mosaicml.com Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Requires-Python: >=3.8 Description-Content-Type:
 text/markdown Provides-Extra: base Provides-Extra: dev Provides-Extra:
 health_checker Provides-Extra: slack Provides-Extra: deepspeed Provides-Extra:
 wandb Provides-Extra: comet_ml Provides-Extra: tensorboard Provides-Extra: unet
 Provides-Extra: vit Provides-Extra: timm Provides-Extra: coco Provides-Extra:
 nlp Provides-Extra: sentencepiece Provides-Extra: mlperf Provides-Extra:
 streaming Provides-Extra: libcloud Provides-Extra: oci Provides-Extra: onnx
-Provides-Extra: mlflow Provides-Extra: mcli Provides-Extra: all License-File:
-LICENSE
+Provides-Extra: mlflow Provides-Extra: all License-File: LICENSE
   [https://storage.googleapis.com/docs.mosaicml.com/images/header_light.svg]
 ***** A PyTorch Library for Efficient Neural Network Training *****
 **** Train Faster, Reduce Cost, Get Better Models ****
 *** [Website] - [Getting_Started] - [Docs] - [Methods] - [We're_Hiring!] ***
 [PyPi_Version] [PyPi_Package_Version] [PyPi_Downloads] [Documentation] [Chat_@
                                Slack] [License]
```

### Comparing `composer-0.14.1/README.md` & `composer-0.15.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     </a>
     <a href="https://pepy.tech/project/mosaicml/">
         <img alt="PyPi Downloads" src="https://static.pepy.tech/personalized-badge/mosaicml?period=month&units=international_system&left_color=grey&right_color=blue&left_text=Downloads/month">
     </a>
     <a href="https://docs.mosaicml.com/projects/composer/en/stable/">
         <img alt="Documentation" src="https://readthedocs.org/projects/composer/badge/?version=stable">
     </a>
-    <a href="https://join.slack.com/t/mosaicml-community/shared_invite/zt-w0tiddn9-WGTlRpfjcO9J5jyrMub1dg">
+    <a href="https://mosaicml.me/slack">
         <img alt="Chat @ Slack" src="https://img.shields.io/badge/slack-chat-2eb67d.svg?logo=slack">
     </a>
     <a href="https://github.com/mosaicml/composer/blob/dev/LICENSE">
         <img alt="License" src="https://img.shields.io/badge/License-Apache%202.0-green.svg?logo=slack">
     </a>
 </p>
 <br />
```

### Comparing `composer-0.14.1/composer/__init__.py` & `composer-0.15.0/composer/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/__init__.py` & `composer-0.15.0/composer/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/alibi/__init__.py` & `composer-0.15.0/composer/algorithms/alibi/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/alibi/alibi.py` & `composer-0.15.0/composer/algorithms/alibi/alibi.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/alibi/attention_surgery_functions/__init__.py` & `composer-0.15.0/composer/algorithms/alibi/attention_surgery_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/alibi/attention_surgery_functions/_bert.py` & `composer-0.15.0/composer/algorithms/alibi/attention_surgery_functions/_bert.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/alibi/attention_surgery_functions/_gpt2.py` & `composer-0.15.0/composer/algorithms/alibi/attention_surgery_functions/_gpt2.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/alibi/attention_surgery_functions/utils.py` & `composer-0.15.0/composer/algorithms/alibi/attention_surgery_functions/utils.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/augmix/__init__.py` & `composer-0.15.0/composer/algorithms/augmix/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/augmix/augmix.py` & `composer-0.15.0/composer/algorithms/augmix/augmix.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/blurpool/__init__.py` & `composer-0.15.0/composer/algorithms/blurpool/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/blurpool/blurpool.py` & `composer-0.15.0/composer/algorithms/blurpool/blurpool.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/blurpool/blurpool_layers.py` & `composer-0.15.0/composer/algorithms/blurpool/blurpool_layers.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/channels_last/__init__.py` & `composer-0.15.0/composer/algorithms/channels_last/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/channels_last/channels_last.py` & `composer-0.15.0/composer/algorithms/channels_last/channels_last.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/channels_last/metadata.json` & `composer-0.15.0/composer/algorithms/channels_last/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/colout/__init__.py` & `composer-0.15.0/composer/algorithms/colout/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/colout/colout.py` & `composer-0.15.0/composer/algorithms/colout/colout.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/cutmix/__init__.py` & `composer-0.15.0/composer/algorithms/cutmix/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/cutmix/cutmix.py` & `composer-0.15.0/composer/algorithms/cutmix/cutmix.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/cutmix/metadata.json` & `composer-0.15.0/composer/algorithms/cutmix/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/cutout/cutout.py` & `composer-0.15.0/composer/algorithms/cutout/cutout.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/ema/ema.py` & `composer-0.15.0/composer/algorithms/ema/ema.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/factorize/__init__.py` & `composer-0.15.0/composer/algorithms/factorize/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/factorize/factorize.py` & `composer-0.15.0/composer/algorithms/factorize/factorize.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/factorize/factorize_core.py` & `composer-0.15.0/composer/algorithms/factorize/factorize_core.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/factorize/factorize_modules.py` & `composer-0.15.0/composer/algorithms/factorize/factorize_modules.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/fused_layernorm/__init__.py` & `composer-0.15.0/composer/algorithms/fused_layernorm/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/fused_layernorm/fused_layernorm.py` & `composer-0.15.0/composer/algorithms/fused_layernorm/fused_layernorm.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/fused_layernorm/metadata.json` & `composer-0.15.0/composer/algorithms/fused_layernorm/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/gated_linear_units/__init__.py` & `composer-0.15.0/composer/algorithms/gated_linear_units/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/gated_linear_units/gated_linear_unit_layers.py` & `composer-0.15.0/composer/algorithms/gated_linear_units/gated_linear_unit_layers.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/gated_linear_units/gated_linear_units.py` & `composer-0.15.0/composer/algorithms/gated_linear_units/gated_linear_units.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/gated_linear_units/metadata.json` & `composer-0.15.0/composer/algorithms/gated_linear_units/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/ghost_batchnorm/__init__.py` & `composer-0.15.0/composer/algorithms/ghost_batchnorm/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/ghost_batchnorm/ghost_batchnorm.py` & `composer-0.15.0/composer/algorithms/ghost_batchnorm/ghost_batchnorm.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/ghost_batchnorm/metadata.json` & `composer-0.15.0/composer/algorithms/ghost_batchnorm/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/gradient_clipping/gradient_clipping.py` & `composer-0.15.0/composer/algorithms/gradient_clipping/gradient_clipping.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/gradient_clipping/metadata.json` & `composer-0.15.0/composer/algorithms/gradient_clipping/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/gyro_dropout/gyro_dropout.py` & `composer-0.15.0/composer/algorithms/gyro_dropout/gyro_dropout.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/label_smoothing/__init__.py` & `composer-0.15.0/composer/algorithms/label_smoothing/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/label_smoothing/label_smoothing.py` & `composer-0.15.0/composer/algorithms/label_smoothing/label_smoothing.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/label_smoothing/metadata.json` & `composer-0.15.0/composer/algorithms/label_smoothing/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/layer_freezing/layer_freezing.py` & `composer-0.15.0/composer/algorithms/layer_freezing/layer_freezing.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/layer_freezing/metadata.json` & `composer-0.15.0/composer/algorithms/layer_freezing/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/low_precision_groupnorm/__init__.py` & `composer-0.15.0/composer/algorithms/low_precision_groupnorm/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/low_precision_groupnorm/low_precision_groupnorm.py` & `composer-0.15.0/composer/algorithms/low_precision_groupnorm/low_precision_groupnorm.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/low_precision_layernorm/__init__.py` & `composer-0.15.0/composer/algorithms/low_precision_layernorm/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/low_precision_layernorm/low_precision_layernorm.py` & `composer-0.15.0/composer/algorithms/low_precision_layernorm/low_precision_layernorm.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/mixup/metadata.json` & `composer-0.15.0/composer/algorithms/mixup/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/mixup/mixup.py` & `composer-0.15.0/composer/algorithms/mixup/mixup.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/no_op_model/__init__.py` & `composer-0.15.0/composer/algorithms/no_op_model/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/no_op_model/no_op_model.py` & `composer-0.15.0/composer/algorithms/no_op_model/no_op_model.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/progressive_resizing/__init__.py` & `composer-0.15.0/composer/algorithms/progressive_resizing/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/progressive_resizing/metadata.json` & `composer-0.15.0/composer/algorithms/progressive_resizing/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/progressive_resizing/progressive_resizing.py` & `composer-0.15.0/composer/algorithms/progressive_resizing/progressive_resizing.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/randaugment/metadata.json` & `composer-0.15.0/composer/algorithms/randaugment/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/randaugment/randaugment.py` & `composer-0.15.0/composer/algorithms/randaugment/randaugment.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/sam/__init__.py` & `composer-0.15.0/composer/algorithms/sam/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/sam/sam.py` & `composer-0.15.0/composer/algorithms/sam/sam.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/selective_backprop/__init__.py` & `composer-0.15.0/composer/algorithms/selective_backprop/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/selective_backprop/metadata.json` & `composer-0.15.0/composer/algorithms/selective_backprop/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/selective_backprop/selective_backprop.py` & `composer-0.15.0/composer/algorithms/selective_backprop/selective_backprop.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/seq_length_warmup/metadata.json` & `composer-0.15.0/composer/algorithms/seq_length_warmup/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/seq_length_warmup/seq_length_warmup.py` & `composer-0.15.0/composer/algorithms/seq_length_warmup/seq_length_warmup.py`

 * *Files 2% similar despite different names*

```diff
@@ -315,14 +315,19 @@
                     optimizer.zero_grad()
 
             # This error/state.device_train_microbatch_size handling mimics the logic in trainer._train_batch().
             except RuntimeError as e:
                 if state.auto_microbatching and _is_cuda_oom(e):
                     log.debug((f"Rank {dist.get_global_rank()} OOM'd."))
                     found_cuda_oom = 1
+                elif state.auto_microbatching and 'cuda' in str(e).lower() or 'c10' in str(e).lower():
+                    raise ValueError(
+                        textwrap.dedent(
+                            'Encountered non-addressable cuda error while using auto microbatching. '
+                            'If this repeatedly occurs, set `device_train_microbatch_size` manually.')) from e
                 else:
                     raise
 
             if state.auto_microbatching:
                 all_ranks_finished = False
                 while not all_ranks_finished:
                     # Propagate across all ranks if any rank hit CUDA OOM
```

### Comparing `composer-0.14.1/composer/algorithms/squeeze_excite/__init__.py` & `composer-0.15.0/composer/algorithms/squeeze_excite/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/squeeze_excite/squeeze_excite.py` & `composer-0.15.0/composer/algorithms/squeeze_excite/squeeze_excite.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/stochastic_depth/__init__.py` & `composer-0.15.0/composer/algorithms/stochastic_depth/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/stochastic_depth/metadata.json` & `composer-0.15.0/composer/algorithms/stochastic_depth/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/stochastic_depth/stochastic_depth.py` & `composer-0.15.0/composer/algorithms/stochastic_depth/stochastic_depth.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/stochastic_depth/stochastic_layers.py` & `composer-0.15.0/composer/algorithms/stochastic_depth/stochastic_layers.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/swa/swa.py` & `composer-0.15.0/composer/algorithms/swa/swa.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/utils/augmentation_common.py` & `composer-0.15.0/composer/algorithms/utils/augmentation_common.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/utils/augmentation_primitives.py` & `composer-0.15.0/composer/algorithms/utils/augmentation_primitives.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/warnings.py` & `composer-0.15.0/composer/algorithms/warnings.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/weight_standardization/metadata.json` & `composer-0.15.0/composer/algorithms/weight_standardization/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/algorithms/weight_standardization/weight_standardization.py` & `composer-0.15.0/composer/algorithms/weight_standardization/weight_standardization.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/callbacks/__init__.py` & `composer-0.15.0/composer/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/callbacks/activation_monitor.py` & `composer-0.15.0/composer/callbacks/activation_monitor.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/callbacks/checkpoint_saver.py` & `composer-0.15.0/composer/callbacks/checkpoint_saver.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import textwrap
 from typing import Callable, List, Optional, Union
 
 from composer.core import Callback, Event, State, Time, TimeUnit
 from composer.loggers import Logger
 from composer.utils import (FORMAT_NAME_WITH_DIST_AND_TIME_TABLE, FORMAT_NAME_WITH_DIST_TABLE, PartialFilePath,
                             checkpoint, create_symlink_file, dist, ensure_folder_has_no_conflicting_files,
-                            format_name_with_dist, is_model_deepspeed, reproducibility)
+                            format_name_with_dist, format_name_with_dist_and_time, is_model_deepspeed, reproducibility)
 
 log = logging.getLogger(__name__)
 
 __all__ = ['CheckpointSaver', 'checkpoint_periodically']
 
 
 def checkpoint_periodically(interval: Union[str, int, Time]) -> Callable[[State, Event], bool]:
@@ -375,43 +375,57 @@
 
         is_deepspeed = is_model_deepspeed(state.model)
 
         if is_deepspeed and '{rank}' not in self.filename.filename:
             raise ValueError(f'Save filename {self.filename.filename} must have {{rank}} for deepspeed.')
 
         # save the checkpoint to the filename
-        filename = self.filename.format(state, is_deepspeed)
+        filename_with_placeholders = self.filename.format(state, is_deepspeed, keep_placeholders=True)
 
         saved_path = checkpoint.save_checkpoint(
             state=state,
-            filename=filename,
+            filename=filename_with_placeholders,
             weights_only=self.weights_only,
         )
 
         if not saved_path:  # not all ranks save
             return
 
-        if self.latest_filename is not None:
+        if self.latest_filename is not None and self.num_checkpoints_to_keep != 0:
             symlink = self.latest_filename.format(state, is_deepspeed)
             os.makedirs(os.path.dirname(symlink), exist_ok=True)
             try:
                 os.remove(symlink)
             except FileNotFoundError:
                 pass
-            os.symlink(os.path.relpath(filename, os.path.dirname(symlink)), symlink)
+            os.symlink(os.path.relpath(saved_path, os.path.dirname(symlink)), symlink)
 
         # if remote file name provided, upload the checkpoint
         if self.remote_file_name is not None:
-            remote_file_name = self.remote_file_name.format(
-                state,
-                is_deepspeed,
-            ).lstrip('/')
+            if state.fsdp_sharded_state_dict_enabled:
+                remote_file_name = self.remote_file_name.format(
+                    state,
+                    is_deepspeed,
+                    keep_placeholders=True,
+                ).lstrip('/')
+                assert state.sharded_ckpt_prefix_dir is not None
+                remote_prefix = state.sharded_ckpt_prefix_dir
+                remote_file_name = os.path.join(
+                    pathlib.Path(remote_file_name).parent, remote_prefix,
+                    pathlib.Path(remote_file_name).name)
+                remote_file_name = format_name_with_dist_and_time(remote_file_name, state.run_name, state.timestamp)
+            else:
+                remote_file_name = self.remote_file_name.format(
+                    state,
+                    is_deepspeed,
+                ).lstrip('/')
 
-            logger.upload_file(remote_file_name=remote_file_name, file_path=filename, overwrite=self.overwrite)
+            logger.upload_file(remote_file_name=remote_file_name, file_path=saved_path, overwrite=self.overwrite)
 
+            # symlinks stay the same with sharded checkpointing
             if self.latest_remote_file_name is not None:
                 symlink_name = self.latest_remote_file_name.format(
                     state,
                     is_deepspeed,
                 ).lstrip('/') + '.symlink'
 
                 # create and upload a symlink file
@@ -420,15 +434,15 @@
                     create_symlink_file(remote_file_name, symlink_filename)
                     logger.upload_file(
                         remote_file_name=symlink_name,
                         file_path=symlink_filename,
                         overwrite=True,
                     )
 
-        self.saved_checkpoints.append(filename)
+        self.saved_checkpoints.append(saved_path)
 
         if self.num_checkpoints_to_keep >= 0:
             self._rotate_checkpoints()
 
     def _rotate_checkpoints(self):
         while len(self.saved_checkpoints) > self.num_checkpoints_to_keep:
             checkpoint = self.saved_checkpoints.pop(0)
```

### Comparing `composer-0.14.1/composer/callbacks/early_stopper.py` & `composer-0.15.0/composer/callbacks/early_stopper.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/callbacks/export_for_inference.py` & `composer-0.15.0/composer/callbacks/export_for_inference.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/callbacks/health_checker.py` & `composer-0.15.0/composer/callbacks/health_checker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright 2022 MosaicML Composer authors
 # SPDX-License-Identifier: Apache-2.0
 
 """Check GPU Health during training."""
 import logging
 import os
+import warnings
 from collections import deque
 from datetime import datetime
 from typing import List, Optional, Tuple
 
 import numpy as np
 import torch
 
@@ -48,14 +49,15 @@
         threshold: float = 10,
         sample_freq: int = 5,
         window_size: int = 120,
         wait: int = 120,
         slack_webhook_url: Optional[str] = None,
         test_mode: bool = False,
     ) -> None:
+        warnings.warn(f'HealthChecker is deprecated and will be removed in v0.16.')
         self.sample_freq = sample_freq
         self.window_size = window_size
         self.wait = wait
         self.slack_webhook_url = slack_webhook_url
         self.test_mode = test_mode
 
         if not self.slack_webhook_url:
```

### Comparing `composer-0.14.1/composer/callbacks/image_visualizer.py` & `composer-0.15.0/composer/callbacks/image_visualizer.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/callbacks/lr_monitor.py` & `composer-0.15.0/composer/callbacks/lr_monitor.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/callbacks/memory_monitor.py` & `composer-0.15.0/composer/callbacks/memory_monitor.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/callbacks/mlperf.py` & `composer-0.15.0/composer/callbacks/mlperf.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
                 root_folder='/submission',
                 index=0,
                 metric_name='MulticlassAccuracy',
                 metric_label='eval',
                 target='0.759',
             )
 
-    During training, the metric found in ``state.eval_metrics[metric_label][metric_name]``
+    During training, the metric found in ``state.eval_metrics[evaluator_label][metric_name]``
     will be compared against the target criterion.
 
     .. note::
 
         This is currently an experimental logger that has not been used (yet)
         to submit an actual result to MLPerf. Please use with caution.
 
@@ -111,15 +111,15 @@
         target (float, optional): The target metric before the mllogger marks the stop
             of the timing run. Default: ``0.759`` (resnet benchmark).
         division (str, optional): Division of submission. Currently only ``open`` division supported.
             Default: ``'open'``.
         metric_name (str, optional): name of the metric to compare against the target.
             Default: ``MulticlassAccuracy``.
         metric_label (str, optional): The label name. The metric will be accessed via
-            ``state.eval_metrics[metric_label][metric_name]``.
+            ``state.eval_metrics[evaluator_label][metric_name]``.
         submitter (str, optional): Submitting organization. Default: ``"MosaicML"``.
         system_name (str, optional): Name of the system (e.g. 8xA100_composer). If
             not provided, system name will default to ``[world_size]x[device_name]_composer``,
             e.g. ``8xNVIDIA_A100_80GB_composer``.
         status (str, optional): Submission status. One of (onprem, cloud, or preview).
             Default: ``"onprem"``.
         cache_clear_cmd (str, optional): Command to invoke during the cache clear. This callback
```

### Comparing `composer-0.14.1/composer/callbacks/optimizer_monitor.py` & `composer-0.15.0/composer/callbacks/optimizer_monitor.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/callbacks/runtime_estimator.py` & `composer-0.15.0/composer/callbacks/runtime_estimator.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/callbacks/speed_monitor.py` & `composer-0.15.0/composer/callbacks/speed_monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,17 +91,17 @@
 
     # Return 0 if no CUDA device (e.g., when running with CPU only)
     if not torch.cuda.is_available():
         return 0
 
     # torch.cuda.get_device_name() ex output: 'NVIDIA A100-SXM4-40GB'
     device_name = torch.cuda.get_device_name().lower()
-    if 'h100-sxm' in device_name:
+    if 'h100' in device_name and 'hbm3' in device_name:
         device_name = 'h100-sxm'
-    elif 'h100-pcie' in device_name:
+    elif 'h100' in device_name and ('pcie' in device_name or 'hbm2e' in device_name):
         device_name = 'h100-pcie'
     elif 'a100' in device_name:
         device_name = 'a100'
     elif 'v100-sxm' in device_name:
         device_name = 'v100-sxm'
     elif 'v100-pcie' in device_name:
         device_name = 'v100-pcie'
```

### Comparing `composer-0.14.1/composer/callbacks/threshold_stopper.py` & `composer-0.15.0/composer/callbacks/threshold_stopper.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/cli/launcher.py` & `composer-0.15.0/composer/cli/launcher.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/core/__init__.py` & `composer-0.15.0/composer/core/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/core/algorithm.py` & `composer-0.15.0/composer/core/algorithm.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
            DeepSpeed integration with this function returning True is not tested. It may not work as expected.
         """
         return False
 
     @property
     def backwards_create_graph(self) -> bool:
-        """Return ``True`` to indicate this algorithm requires a second derivative to be computed. Defaults to ``False``.
+        """Whether this algorithm requires the backwards pass to be differentiable. Defaults to ``False``.
 
         If it returns ``True``, ``create_graph=True`` will be passed to :meth:`torch.Tensor.backward` which will result in
         the graph of the gradient also being constructed. This allows the computation of second order derivatives.
         """
         return False
 
     @staticmethod
```

### Comparing `composer-0.14.1/composer/core/callback.py` & `composer-0.15.0/composer/core/callback.py`

 * *Files 2% similar despite different names*

```diff
@@ -365,14 +365,24 @@
         Args:
             state (State): The training state.
             logger (Logger): The logger.
         """
         del state, logger  # unused
         pass
 
+    def eval_before_all(self, state: State, logger: Logger) -> None:
+        """Called on the :attr:`.Event.EVAL_BEFORE_ALL` event.
+
+        Args:
+            state (State): The training state.
+            logger (Logger): The logger.
+        """
+        del state, logger  # unused
+        pass
+
     def eval_start(self, state: State, logger: Logger) -> None:
         """Called on the :attr:`.Event.EVAL_START` event.
 
         Args:
             state (State): The training state.
             logger (Logger): The logger.
         """
@@ -424,14 +434,24 @@
 
         Args:
             state (State): The training state.
             logger (Logger): The logger.
         """
         del state, logger  # unused
         pass
+
+    def eval_after_all(self, state: State, logger: Logger) -> None:
+        """Called on the :attr:`.Event.EVAL_AFTER_ALL` event.
+
+        Args:
+            state (State): The training state.
+            logger (Logger): The logger.
+        """
+        del state, logger  # unused
+        pass
 
     def fit_end(self, state: State, logger: Logger) -> None:
         """Called on the :attr:`.Event.FIT_END` event.
 
         Args:
             state (State): The training state.
             logger (Logger): The logger.
```

### Comparing `composer-0.14.1/composer/core/data_spec.py` & `composer-0.15.0/composer/core/data_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Copyright 2022 MosaicML Composer authors
 # SPDX-License-Identifier: Apache-2.0
 
 """Specifications for operating and training on data."""
 from __future__ import annotations
 
 import collections.abc
-import math
 import textwrap
 import warnings
 from typing import TYPE_CHECKING, Any, Callable, Iterable, List, Mapping, Optional, Sequence, Tuple, Union
 
 import torch
 import torch.utils.data
 from torch.utils.data.distributed import DistributedSampler
@@ -24,28 +23,24 @@
 
 def _split_list(l, microbatch_size: int):
     if len(l) < microbatch_size:
         warnings.warn(f'Cannot split list of length {len(l)} into batches of size {microbatch_size}. '
                       'As it is smaller, no splitting will be done. This may happen on the last batch '
                       'of a dataset if it is a smaller size than the microbatch size.')
         microbatch_size = len(l)
-    num_microbatches = math.ceil(len(l) / microbatch_size)
-    # Note: this is to match the behavior of tensor.chunk, which is used in _split_tensor
-    chunked_microbatch_size = math.ceil(len(l) / num_microbatches)
-    return [l[start:start + chunked_microbatch_size] for start in range(0, len(l), chunked_microbatch_size)]
+    return [l[start:start + microbatch_size] for start in range(0, len(l), microbatch_size)]
 
 
 def _split_tensor(t, microbatch_size: int):
     if len(t) < microbatch_size:
         warnings.warn(f'Cannot split tensor of length {len(t)} into batches of size {microbatch_size}. '
                       'As it is smaller, no splitting will be done. This may happen on the last batch '
                       'of a dataset if it is a smaller size than the microbatch size.')
         microbatch_size = len(t)
-    num_microbatches = math.ceil(len(t) / microbatch_size)
-    return t.chunk(num_microbatches)
+    return t.split(microbatch_size)
 
 
 def _split_mapping(m, microbatch_size: int):
     chunked = {}
     for k, v in m.items():
         if isinstance(v, torch.Tensor):
             chunked[k] = _split_tensor(v, microbatch_size)
```

### Comparing `composer-0.14.1/composer/core/engine.py` & `composer-0.15.0/composer/core/engine.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/core/evaluator.py` & `composer-0.15.0/composer/core/evaluator.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/core/event.py` & `composer-0.15.0/composer/core/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,41 +50,47 @@
                 # Un-scale gradients
 
                 # <AFTER_TRAIN_BATCH>
                 optimizer.step()
 
                 # <BATCH_END>
 
-                if should_eval(batch=True):
-                    for eval_dataloader in eval_dataloaders:
+                # <BEFORE_EVAL_ALL>
+                for eval_dataloader in eval_dataloaders:
+                    if should_eval(batch=True):
                         # <EVAL_START>
                         for batch in eval_dataloader:
                             # <EVAL_BATCH_START>
                             # <EVAL_BEFORE_FORWARD>
                             outputs, targets = model(batch)
                             # <EVAL_AFTER_FORWARD>
                             metrics.update(outputs, targets)
                             # <EVAL_BATCH_END>
                         # <EVAL_END>
 
+                # <AFTER_EVAL_ALL>
+
                 # <BATCH_CHECKPOINT>
             # <EPOCH_END>
 
-            if should_eval(batch=False):
-                for eval_dataloader in eval_dataloaders:
+            # <BEFORE_EVAL_ALL>
+            for eval_dataloader in eval_dataloaders:
+                if should_eval(batch=True):
                     # <EVAL_START>
                     for batch in eval_dataloader:
                         # <EVAL_BATCH_START>
                         # <EVAL_BEFORE_FORWARD>
                         outputs, targets = model(batch)
                         # <EVAL_AFTER_FORWARD>
                         metrics.update(outputs, targets)
                         # <EVAL_BATCH_END>
                     # <EVAL_END>
 
+            # <AFTER_EVAL_ALL>
+
             # <EPOCH_CHECKPOINT>
         # <FIT_END>
 
     Attributes:
         INIT: Invoked in the constructor of :class:`~.trainer.Trainer`. Model surgery (see
             :mod:`~composer.utils.module_surgery`) typically occurs here.
         AFTER_LOAD: Immediately after checkpoint is loaded in constructor of :class:`~.trainer.Trainer`.
@@ -118,20 +124,22 @@
         EPOCH_CHECKPOINT: After :attr:`.Event.EPOCH_END` and any epoch-wise evaluation. Saving checkpoints at this
             event allows the checkpoint saver to use the results from any epoch-wise evaluation to determine whether
             a checkpointshould be saved.
         FIT_END: Invoked at the end of each call to :meth:`.Trainer.fit`. This event exists primarily for logging information
             and flushing callbacks. Algorithms should not transform the training state on this event, as any changes will not
             be preserved in checkpoints.
 
+        EVAL_BEFORE_ALL: Before any evaluators process validation dataset.
         EVAL_START: Start of evaluation through the validation dataset.
         EVAL_BATCH_START: Before the call to ``model.eval_forward(batch)``
         EVAL_BEFORE_FORWARD: Before the call to ``model.eval_forward(batch)``
         EVAL_AFTER_FORWARD: After the call to ``model.eval_forward(batch)``
         EVAL_BATCH_END: After the call to ``model.eval_forward(batch)``
         EVAL_END: End of evaluation through the validation dataset.
+        EVAL_AFTER_ALL: After all evaluators process validation dataset.
     """
 
     INIT = 'init'
     AFTER_LOAD = 'after_load'
     FIT_START = 'fit_start'
 
     EPOCH_START = 'epoch_start'
@@ -158,20 +166,22 @@
     BATCH_CHECKPOINT = 'batch_checkpoint'
 
     EPOCH_END = 'epoch_end'
     EPOCH_CHECKPOINT = 'epoch_checkpoint'
 
     FIT_END = 'fit_end'
 
+    EVAL_BEFORE_ALL = 'eval_before_all'
     EVAL_START = 'eval_start'
     EVAL_BATCH_START = 'eval_batch_start'
     EVAL_BEFORE_FORWARD = 'eval_before_forward'
     EVAL_AFTER_FORWARD = 'eval_after_forward'
     EVAL_BATCH_END = 'eval_batch_end'
     EVAL_END = 'eval_end'
+    EVAL_AFTER_ALL = 'eval_after_all'
 
     PREDICT_START = 'predict_start'
     PREDICT_BATCH_START = 'predict_batch_start'
     PREDICT_BEFORE_FORWARD = 'predict_before_forward'
     PREDICT_AFTER_FORWARD = 'predict_after_forward'
     PREDICT_BATCH_END = 'predict_batch_end'
     PREDICT_END = 'predict_end'
@@ -225,12 +235,13 @@
     def is_eval(self) -> bool:
         """Whether the event is during the eval loop."""
         return self.value.startswith('eval')
 
 
 _BEFORE_EVENTS = (Event.FIT_START, Event.EPOCH_START, Event.BEFORE_DATALOADER, Event.BATCH_START,
                   Event.BEFORE_TRAIN_BATCH, Event.BEFORE_FORWARD, Event.BEFORE_LOSS, Event.BEFORE_BACKWARD,
-                  Event.EVAL_START, Event.EVAL_BATCH_START, Event.EVAL_BEFORE_FORWARD, Event.PREDICT_START,
-                  Event.PREDICT_BATCH_START, Event.PREDICT_BEFORE_FORWARD)
+                  Event.EVAL_BEFORE_ALL, Event.EVAL_START, Event.EVAL_BATCH_START, Event.EVAL_BEFORE_FORWARD,
+                  Event.PREDICT_START, Event.PREDICT_BATCH_START, Event.PREDICT_BEFORE_FORWARD)
 _AFTER_EVENTS = (Event.EPOCH_END, Event.BATCH_END, Event.AFTER_DATALOADER, Event.AFTER_TRAIN_BATCH, Event.AFTER_FORWARD,
-                 Event.AFTER_LOSS, Event.AFTER_BACKWARD, Event.EVAL_END, Event.EVAL_BATCH_END, Event.EVAL_AFTER_FORWARD,
-                 Event.FIT_END, Event.PREDICT_END, Event.PREDICT_BATCH_END, Event.PREDICT_AFTER_FORWARD)
+                 Event.AFTER_LOSS, Event.AFTER_BACKWARD, Event.EVAL_AFTER_ALL, Event.EVAL_END, Event.EVAL_BATCH_END,
+                 Event.EVAL_AFTER_FORWARD, Event.FIT_END, Event.PREDICT_END, Event.PREDICT_BATCH_END,
+                 Event.PREDICT_AFTER_FORWARD)
```

### Comparing `composer-0.14.1/composer/core/passes.py` & `composer-0.15.0/composer/core/passes.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/core/precision.py` & `composer-0.15.0/composer/core/precision.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/core/serializable.py` & `composer-0.15.0/composer/core/serializable.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/core/state.py` & `composer-0.15.0/composer/core/state.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,36 +68,55 @@
     from torch.distributed.fsdp import FullStateDictConfig
     from torch.distributed.fsdp import FullyShardedDataParallel as FSDP
     from torch.distributed.fsdp import LocalStateDictConfig, StateDictType
     # torch forgot to put ShardedStateDictConfig in torch/distributed/fsdp/__init__.py, so we
     # have to import it this way.
     from torch.distributed.fsdp.fully_sharded_data_parallel import ShardedStateDictConfig
 
+    fsdp_state_dict_type = None
+    state_dict_config = None
+    optim_state_dict_config = None
     # Full is the full monolithic state dict materialized in memory on just rank 0
     # with offloading to cpu if necessary
     if state_dict_type == 'full':
-        state_dict_config = FullStateDictConfig(offload_to_cpu=True, rank0_only=True)
         fsdp_state_dict_type = StateDictType.FULL_STATE_DICT
+        state_dict_config = FullStateDictConfig(offload_to_cpu=True, rank0_only=True)
+        if using_torch_2():
+            from torch.distributed.fsdp.fully_sharded_data_parallel import FullOptimStateDictConfig
+            optim_state_dict_config = FullOptimStateDictConfig(offload_to_cpu=True, rank0_only=True)
 
     # Sharded is sharded state dict, but unflattened parameters (not useful for FSDP, but
     # useful if you plan to use the state dict outside of FSDP).
     elif state_dict_type == 'sharded':
-        state_dict_config = ShardedStateDictConfig()
         fsdp_state_dict_type = StateDictType.SHARDED_STATE_DICT
+        state_dict_config = ShardedStateDictConfig()
+        if using_torch_2():
+            from torch.distributed.fsdp.fully_sharded_data_parallel import ShardedOptimStateDictConfig
+            optim_state_dict_config = ShardedOptimStateDictConfig()
 
     # Local is the FSDP standard sharded, flattened parameters. This is what the parameters
     # are formatted to for a single rank's FSDP module.
     elif state_dict_type == 'local':
-        state_dict_config = LocalStateDictConfig()
         fsdp_state_dict_type = StateDictType.LOCAL_STATE_DICT
+        state_dict_config = LocalStateDictConfig()
+        if using_torch_2():
+            from torch.distributed.fsdp.fully_sharded_data_parallel import LocalOptimStateDictConfig
+            optim_state_dict_config = LocalOptimStateDictConfig()
     else:
         raise NotImplementedError(f'No valid FSDP state_dict_type for {state_dict_type}')
 
-    with FSDP.state_dict_type(module, state_dict_type=fsdp_state_dict_type, state_dict_config=state_dict_config):
-        yield
+    if using_torch_2():
+        with FSDP.state_dict_type(module,
+                                  state_dict_type=fsdp_state_dict_type,
+                                  state_dict_config=state_dict_config,
+                                  optim_state_dict_config=optim_state_dict_config):
+            yield
+    else:
+        with FSDP.state_dict_type(module, state_dict_type=fsdp_state_dict_type, state_dict_config=state_dict_config):
+            yield
 
 
 def fsdp_get_optim_state_dict(model: torch.nn.Module,
                               optim: torch.optim.Optimizer,
                               state_dict_type: str = 'full') -> Dict[str, Any]:
     """Materializes a given model's optimizer's state_dict.
 
@@ -144,25 +163,26 @@
         # State dict is already local, so just return state dict.
         return optim.state_dict()
     else:
         raise NotImplementedError(f'No valid FSDP state_dict_type for {state_dict_type}')
 
 
 def _legacy_optim_state_dict_to_load(
-    optim_state_dict: Dict[str, Any],
+    optim_state_dict: Optional[Dict[str, Any]],
     model: torch.nn.Module,
     optim: torch.optim.Optimizer,
     state_dict_type: str = 'full',
 ):
     if version.parse(torch.__version__) < version.parse('1.13.0'):
         raise RuntimeError('To use FSDP with Composer, you must use torch>=1.13.0.')
     from torch.distributed.fsdp import FullyShardedDataParallel as FSDP
     if state_dict_type == 'sharded':
         # Optimizer and optimizer state dict are already sharded, but not
         # flattened, so we flatten the state dict then load it.
+        assert optim_state_dict is not None
         flattened_optim_state_dict = FSDP.flatten_sharded_optim_state_dict(sharded_optim_state_dict=optim_state_dict,
                                                                            model=model,
                                                                            optim=optim)
         return flattened_optim_state_dict
     elif state_dict_type == 'local':
         # Optimizer and optimizer state dict are already sharded and flattened,
         # so just load the state_dict.
@@ -259,14 +279,15 @@
         schedulers (types.PyTorchScheduler | Sequence[types.PyTorchScheduler], optional):
             The learning rate scheduler (can also be a list or tuple of schedulers).
         scaler (torch.cuda.amp.GradScaler, optional): The gradient scaler in use for mixed precision training.
         algorithms (Algorithm | Sequence[Algorithm], optional): The algorithms used for training.
         callbacks (Callback | Sequence[Callback], optional): The callbacks used for training.
         deepspeed_config (Dict[str, Any], optional): The configuration dictionary for deepspeed.
         fsdp_config (Dict[str, Any], optional): The configuration dictionary for FSDP.
+        fsdp_auto_wrap (bool, optional): Whether to automatically wrap the model with FSDP.
 
     Attributes:
         batch (types.Batch): The batch. This will be the entire batch during the :attr:`.Event.AFTER_DATALOADER`, or a
             microbatch between :attr:`.Event.BATCH_START` and :attr:`.Event.BATCH_END`.
         device (Device): The device used by this process. The trainer moves the model and loaded data to this device. This
             can be used in callbacks and algorithms to move data onto the correct device.
         train_metrics (Dict[str, Metric]): The current train metrics, organized by metric name. ``train_metrics`` will be deep-copied to
@@ -422,14 +443,15 @@
         # algorithms and callbacks
         algorithms: Optional[Union[Algorithm, Sequence[Algorithm]]] = None,
         callbacks: Optional[Union[Callback, Sequence[Callback]]] = None,
 
         # Distributed training configs
         deepspeed_config: Optional[Dict[str, Any]] = None,
         fsdp_config: Optional[Dict[str, Any]] = None,
+        fsdp_auto_wrap: bool = True,
     ):
         self.rank_zero_seed = rank_zero_seed
         self.model = model
         self.run_name = run_name
         self.device = device
         self.device_train_microbatch_size = device_train_microbatch_size
         self.auto_microbatching = auto_microbatching
@@ -462,21 +484,45 @@
         self._algorithms = list(ensure_tuple(algorithms))
         self._callbacks = list(ensure_tuple(callbacks))
 
         self.profiler: Optional[Profiler] = None
 
         self.deepspeed_config = deepspeed_config
         self.fsdp_config = fsdp_config
+        self.fsdp_auto_wrap = fsdp_auto_wrap
 
-        self.fsdp_state_dict_type: Optional[str] = None
-        if self.fsdp_enabled:
-            if self.fsdp_config is not None:
-                self.fsdp_state_dict_type = self.fsdp_config.get('state_dict_type', 'full')
-            else:
-                self.fsdp_state_dict_type = 'full'
+        if self.load_fsdp_monolith_rank0_only:
+            assert fsdp_config is not None
+            error_message = ''
+            if fsdp_config['use_orig_params'] == True:
+                error_message += textwrap.dedent(
+                    "load_fsdp_monolith_rank0_only requires fsdp_config['use_orig_params'] to be False. "
+                    "Either set fsdp_config['use_orig_params'] = False or set load_fsdp_monolith_rank0_only = False. ")
+            if fsdp_config['sync_module_states'] == False:
+                error_message += textwrap.dedent(
+                    "load_fsdp_monolith_rank0_only requires fsdp_config['sync_module_states'] to be True. "
+                    "Either set fsdp_config['sync_module_states'] = True or set load_fsdp_monolith_rank0_only = False. "
+                )
+            # Broadcast rank 0 meta check to all ranks so error can be raised on all ranks
+            rank0_on_meta = 0
+            if dist.get_global_rank() == 0 and next(model.parameters()).device.type == 'meta':
+                rank0_on_meta = 1
+            rank0_on_meta_tensor = self.device.tensor_to_device(torch.tensor([rank0_on_meta], dtype=torch.uint8))
+            dist.all_reduce(rank0_on_meta_tensor, reduce_operation='MAX')
+            if rank0_on_meta_tensor.item() == 1:
+                error_message += textwrap.dedent(
+                    'load_fsdp_monolith_rank0_only requires the rank 0 model to be on cpu or gpu, '
+                    'but detected model device as meta. Either move the model to cpu or gpu, or set '
+                    'load_fsdp_monolith_rank0_only = False. ')
+            if error_message != '':
+                raise ValueError(error_message)
+
+        self.sharded_ckpt_prefix_dir: Optional[str] = None
+        if self.fsdp_config is not None:
+            self.sharded_ckpt_prefix_dir = self.fsdp_config['sharded_ckpt_prefix_dir']
 
         # Set defaults for transient variables (to make pyright happy)
         self.batch: Any = None
         self.loss: Union[torch.Tensor, Sequence[torch.Tensor]] = torch.Tensor()
         self.outputs: Union[torch.Tensor, Sequence[torch.Tensor]] = torch.Tensor()
 
         # These attributes will be serialized using .state_dict(), and loaded with .load_state_dict()
@@ -706,29 +752,42 @@
         from torch.distributed.fsdp import FullyShardedDataParallel
         for module in self.model.modules():
             if isinstance(module, FullyShardedDataParallel):
                 return True
         return False
 
     @property
+    def fsdp_state_dict_type(self):
+        if not self.fsdp_enabled:
+            return None
+        if self.fsdp_config is not None:
+            return self.fsdp_config['state_dict_type']
+        return 'full'
+
+    @property
     def fsdp_sharded_state_dict_enabled(self):
-        if self.fsdp_config is None:
-            return False
-        return (self.fsdp_enabled and self.fsdp_state_dict_type in ['sharded', 'local'])
+        return self.fsdp_config is not None and self.fsdp_enabled and self.fsdp_state_dict_type in ['sharded', 'local']
+
+    @property
+    def load_fsdp_monolith_rank0_only(self):
+        return self.fsdp_config is not None and self.fsdp_auto_wrap and self.fsdp_config[
+            'state_dict_type'] == 'full' and self.fsdp_config['load_monolith_rank0_only'] == True
 
     def _get_integrations_state_dict(self) -> Dict[str, Any]:
         """Gets a dictionary of information about integrations to store in the state dict.
 
         This metadata is used for loading things from state dict that need to be done outside
         of the normal Composer load path (e.g. HuggingFace model/tokenizer).
         """
         from composer.models import HuggingFaceModel
         integrations = {}
         if isinstance(self.model, HuggingFaceModel):
             integrations['huggingface'] = self.model.get_metadata()
+        elif self.is_model_ddp and isinstance(self.model.module, HuggingFaceModel):
+            integrations['huggingface'] = self.model.module.get_metadata()
         return integrations
 
     def _get_state_metadata(self) -> Dict[str, Any]:
         """Gets a dictionary of metadata to store in the state dict.
 
         This metadata is used for checking compatibility between the current environment/setup
         and the environment/setup that was used for the checkpoint that is being loaded in
@@ -971,62 +1030,105 @@
             self._apply_required_algorithms(state_dict, logger, exclude_algorithms, algorithm_passes)
 
         if state_dict.get('is_model_ddp', False) and not self.is_model_ddp:
             # This check is for backwards compatibility, as pre-v0.6.0 checkpoints serialized the state
             # with the `module.` prefix
             torch.nn.modules.utils.consume_prefix_in_state_dict_if_present(state_dict['model'], 'module.')
 
-        if self.fsdp_enabled and self.fsdp_state_dict_type is not None:
-            with fsdp_state_dict_type_context(self.model, state_dict_type=self.fsdp_state_dict_type):
-                missing_keys, unexpected_keys = self.model.load_state_dict(state_dict['model'], strict=strict)
-        else:
-            missing_keys, unexpected_keys = self.model.load_state_dict(state_dict['model'], strict=strict)
-        if len(missing_keys) > 0:
+        # For FSDP monolith checkpoints, the model does not exist on ranks > 0
+        model_on_rank = state_dict['model'] is not None
+
+        missing_keys, unexpected_keys = [], []
+        try:
+            # Load model if it exists. For FSDP monolith checkpoints, the model does not exist on ranks > 0
+            if model_on_rank:
+                if self.fsdp_enabled and self.fsdp_state_dict_type is not None and not self.load_fsdp_monolith_rank0_only:
+                    log.debug(
+                        f'Loading model state dict with strict={strict} and FSDP state_dict_type={self.fsdp_state_dict_type}'
+                    )
+                    with fsdp_state_dict_type_context(self.model, state_dict_type=self.fsdp_state_dict_type):
+                        missing_keys, unexpected_keys = self.model.load_state_dict(state_dict['model'], strict=strict)
+                else:
+                    log.debug(f'Loading model state dict with strict={strict}')
+                    missing_keys, unexpected_keys = self.model.load_state_dict(state_dict['model'], strict=strict)
+        except RuntimeError as e:
+            if 'Missing key(s) in state_dict' in str(e) or 'Unexpected key(s) in state_dict' in str(e):
+                raise RuntimeError(
+                    textwrap.dedent('Failed to load checkpoint due to missing or unexpected keys in state_dict. '
+                                    'This is likely due to a change in the model architecture. If this is intentional, '
+                                    'you can set load_strict_model_weights=False in the Trainer.')) from e
+            else:
+                raise e
+
+        if model_on_rank and len(missing_keys) > 0:
             log.warning(f"Found these missing keys in the checkpoint: {', '.join(missing_keys)}")
-        if len(unexpected_keys) > 0:
-            if self.fsdp_config is not None and self.fsdp_config.get(
-                    'use_orig_params') and self.fsdp_state_dict_type == 'local':
+        if model_on_rank and len(unexpected_keys) > 0:
+            if self.fsdp_config is not None and self.fsdp_config[
+                    'use_orig_params'] and self.fsdp_state_dict_type == 'local':
                 log.warning(
                     'You are using use_orig_params=True and fsdp_state_dict_type=local. '
                     'This results in both the original parameters and the flat parameters being '
                     'in the state dict. If you see a warning with unexpected keys ending in ._flat_param, the model'
                     'was still loaded correctly.')
             log.warning(f"Found these unexpected keys in the checkpoint: {', '.join(unexpected_keys)}")
 
+        # If loading FSDP monolith checkpoint on rank 0 only, the model must be wrapped after loading
+        if self.load_fsdp_monolith_rank0_only:
+            assert self.fsdp_config is not None
+            log.info('Wrapping model with FSDP after loading model_state.')
+            from composer.trainer.dist_strategy import prepare_fsdp_module
+            prepare_fsdp_module(self.model, self.optimizers, self.fsdp_config, self.precision, self.device,
+                                self.auto_microbatching)
+            log.debug('Finished wrapping model with FSDP.')
+
     def load_optim_state(self, state_dict: Dict[str, Any]):
         """Load the optimizer state.
 
         Args:
             state_dict (Dict[str, Any]): The state to load.
         """
         serialized_value = state_dict['optimizers']
         for optimizer in ensure_tuple(self.optimizers):
-            if type(optimizer).__qualname__ not in serialized_value:
+            # Broadcast compatibility check as monolith rank 0 only loads won't have optimizer on all ranks
+            skip_optimizer_load = 1 if serialized_value is not None and type(
+                optimizer).__qualname__ not in serialized_value else 0
+            skip_optimizer_load_tensor = self.device.tensor_to_device(
+                torch.tensor([skip_optimizer_load], dtype=torch.uint8))
+            dist.all_reduce(skip_optimizer_load_tensor, reduce_operation='MAX')
+            if skip_optimizer_load_tensor.item() == 1:
                 warnings.warn(
                     f'{type(optimizer).__qualname__} is not in the state_dict. Its state will not be restored.',
                     category=UserWarning)
                 continue
-            optim_state_dict = serialized_value[type(optimizer).__qualname__]
+
+            optim_state_dict = serialized_value[type(optimizer).__qualname__] if serialized_value is not None else None
             if self.fsdp_enabled:
                 assert self.fsdp_state_dict_type is not None  # pyright
                 if version.parse(torch.__version__) < version.parse('1.13.0'):
                     raise RuntimeError('To use FSDP with Composer, you must use torch>=1.13.0.')
                 from torch.distributed.fsdp import FullyShardedDataParallel as FSDP
                 log.debug(f'Loading FSDP optimizer with fsdp_state_dict_type={self.fsdp_state_dict_type}')
-                if not using_torch_2():
-                    optim_state_dict = _legacy_optim_state_dict_to_load(optim_state_dict=optim_state_dict,
-                                                                        model=self.model,
-                                                                        optim=optimizer,
-                                                                        state_dict_type=self.fsdp_state_dict_type)
+                # Loading FSDP monolith on rank 0 only requires FSDP.scatter_full_optim_state_dict
+                # as the context manager does not seem to pass rank0_only=True for the optimizer config
+                if not using_torch_2() or self.load_fsdp_monolith_rank0_only:
+                    optim_state_dict = _legacy_optim_state_dict_to_load(
+                        optim_state_dict=optim_state_dict,
+                        model=self.model,
+                        optim=optimizer,
+                        state_dict_type=self.fsdp_state_dict_type,
+                    )
                 else:
+                    assert optim_state_dict is not None
                     with fsdp_state_dict_type_context(module=self.model, state_dict_type=self.fsdp_state_dict_type):
                         optim_state_dict = FSDP.optim_state_dict_to_load(  #  type: ignore
                             optim_state_dict=optim_state_dict, model=self.model, optim=optimizer)
+                assert optim_state_dict is not None
                 optimizer.load_state_dict(optim_state_dict)
             else:
+                assert optim_state_dict is not None
                 log.debug(f'Loading optimizer state dict')
                 optimizer.load_state_dict(optim_state_dict)
 
     def _load_dataset_state(self, obj: Dict[str, Any]) -> None:
         """Load the dataset state.
 
         Args:
@@ -1069,25 +1171,26 @@
                 ``self.model``. Defaults to False.
             exclude_algorithms (List[str], optional): List of algorithm names to exclude from autoloading. (default: ``None``)
             algorithm_passes (List[AlgorithmPass], optional): A list of algorithm passes to apply to autoloaded algorithms
                 to sort them into the correct order. (default: ``None``)
         """
         state = _ensure_backwards_compatible_checkpointing(state)
 
-        # Call load_model_state since it applies required algorithms
+        # Call load_model_state first since it applies required algorithms
         if 'model' in state:
             self.load_model_state(
                 state,
                 logger,
                 strict=strict,
                 exclude_algorithms=exclude_algorithms,
                 algorithm_passes=algorithm_passes,
             )
 
-        for attribute_name, serialized_value in state.items():
+        for attribute_name in sorted(list(state.keys())):  # Sort so all ranks load in the same order
+            serialized_value = state[attribute_name]
             # Skip removed attributes as well as algorithms and model, which was already loaded
             if attribute_name not in self.serialized_attributes or attribute_name == 'model':
                 continue
 
             # Integrations are extra information about other libraries (e.g. huggingface) and not attributes to be loaded here
             if attribute_name == 'integrations':
                 continue
```

### Comparing `composer-0.14.1/composer/core/time.py` & `composer-0.15.0/composer/core/time.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/core/types.py` & `composer-0.15.0/composer/core/types.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/datasets/__init__.py` & `composer-0.15.0/composer/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/datasets/ade20k.py` & `composer-0.15.0/composer/datasets/ade20k.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/datasets/brats.py` & `composer-0.15.0/composer/datasets/brats.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/datasets/c4.py` & `composer-0.15.0/composer/datasets/c4.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/datasets/cifar.py` & `composer-0.15.0/composer/datasets/cifar.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/datasets/ffcv_utils.py` & `composer-0.15.0/composer/datasets/ffcv_utils.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/datasets/imagenet.py` & `composer-0.15.0/composer/datasets/imagenet.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/datasets/in_context_learning_evaluation.py` & `composer-0.15.0/composer/datasets/in_context_learning_evaluation.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,22 +11,27 @@
 
 import torch
 import transformers
 from torch.utils.data import DataLoader, Dataset
 from tqdm import tqdm
 
 from composer.core import DataSpec
+from composer.core.data_spec import _default_split_batch, _split_list
 from composer.utils import MissingConditionalImportError, dist, get_file
 
 if TYPE_CHECKING:
     import transformers
 
 __all__ = ['InContextLearningLMTaskDataset', 'InContextLearningMultipleChoiceTaskDataset', 'get_icl_task_dataloader']
 
 
+def strip_data(samples):
+    return [{k: v.strip() if isinstance(v, str) else v for k, v in entry.items()} for entry in samples]
+
+
 def _tokenizer_needs_prefix_space(tokenizer) -> bool:
     # Test for whether a prefix space is needed before the continuation.
     # sentencepiece tokenization should not have a prefix space, but gpt2 style BPE should
     return len(tokenizer(' a', add_special_tokens=False)['input_ids']) == 1
 
 
 def _make_padded_input(context_enc, continuation_enc, max_seq_len, pad_tok_id, padding_side='right'):
@@ -140,14 +145,15 @@
         dataset = load_dataset('json', data_files=destination_path, split='train', streaming=False)
         self.samples = list(
             dataset.map(lambda examples: {
                 'context': examples['context'],
                 'answer': examples['answer'],
                 'aliases': examples['aliases']
             }))
+        self.samples = strip_data(self.samples)
         self.tokenizer = tokenizer
         self.max_seq_len = max_seq_len
         self.pad_tok_id = pad_tok_id
         self.padding_side = 'left'
         self.max_answer_length = 0
         fewshot_rng = random.Random(fewshot_random_seed)
         self.encoded_dataset = self.prep_examples(num_fewshot, prompt_string, example_delimiter, continuation_delimiter,
@@ -238,24 +244,46 @@
 
         batch = {
             'input_ids': torch.stack(inputs),
             'mode': 'generate',
             'labels': answers,
             'generation_length': self.max_answer_length,
             'generation_kwargs': {
-                'pad_token_id': self.pad_tok_id
+                'pad_token_id': self.pad_tok_id,
+                'use_cache': True
             }
         }
 
         batch['attention_mask'] = ~(batch['input_ids'] == self.pad_tok_id)
         return batch
 
     def get_num_samples_in_batch(self, batch) -> int:
         return batch['input_ids'].shape[0]
 
+    def split_batch(self, batch: Any, microbatch_size: int):
+        no_split = ['mode', 'generation_length', 'generation_kwargs']
+        normal_split = ['input_ids', 'attention_mask']
+        list_split = ['labels']
+        chunked = {}
+        for k, v in batch.items():
+            if k in no_split:
+                # Defer broadcasting until we know num_chunks
+                pass
+            elif k in list_split:
+                chunked[k] = _split_list(v, microbatch_size)
+            elif k in normal_split:
+                chunked[k] = _default_split_batch(v, microbatch_size)
+            else:
+                raise ValueError(f'Unexpected key {k}')
+        num_chunks = len(chunked['input_ids'])
+        for k, v in batch.items():
+            if isinstance(v, (int, float, str, bool, dict)):
+                chunked[k] = [v] * num_chunks
+        return [{k: v[idx] for k, v in chunked.items()} for idx in range(num_chunks)]
+
 
 class InContextLearningLMTaskDataset(Dataset):
     """A dataset that construct batches for in-context learning language modeling evaluation
 
     Args:
         dataset_uri (str): Either a local path, or a remote path beginning with ``s3://``, or another backend
             supported by :meth:`composer.utils.maybe_create_object_store_from_uri`. Dataset must consist of rows of JSON data points with "context",
@@ -296,14 +324,16 @@
                 get_file(dataset_uri, destination_path, overwrite=True)
         dataset = load_dataset('json', data_files=destination_path, split='train', streaming=False)
         self.samples = list(
             dataset.map(lambda examples: {
                 'continuation': examples['continuation'],
                 'context': examples['context'],
             }))
+        self.samples = strip_data(self.samples)
+
         self.tokenizer = tokenizer
         self.max_seq_len = max_seq_len
         self.pad_tok_id = pad_tok_id
         fewshot_rng = random.Random(fewshot_random_seed)
 
         self.prefix_space = _tokenizer_needs_prefix_space(self.tokenizer)
 
@@ -460,14 +490,16 @@
         dataset = load_dataset('json', data_files=destination_path, split='train', streaming=False)
         self.samples = list(
             dataset.map(lambda examples: {
                 'query': examples['query'],
                 'choices': examples['choices'],
                 'gold': examples['gold']
             }))
+        self.samples = strip_data(self.samples)
+
         self.num_choices = len(self.samples[0]['choices'])
         self.tokenizer = tokenizer
         self.max_seq_len = max_seq_len
         self.pad_tok_id = pad_tok_id
         fewshot_rng = random.Random(fewshot_random_seed)
 
         self.prefix_space = _tokenizer_needs_prefix_space(self.tokenizer)
@@ -504,14 +536,15 @@
             if num_fewshot > 0:
                 fewshot_idxs = _get_fewshot_sample_idxs(len(self.samples), num_fewshot, sample_idx, fewshot_rng)
                 for fewshot_idx in fewshot_idxs:
                     query, choices, gold_idx = self.samples[fewshot_idx]['query'], self.samples[fewshot_idx][
                         'choices'], self.samples[fewshot_idx]['gold']
                     if len(preamble) > 0:
                         query = f'{example_delimiter}{query}'
+                    assert isinstance(gold_idx, int)
                     preamble += f'{query}{continuation_delimiter}{choices[gold_idx]}'
             encoded_example = {}
             query, choices, gold_idx = self.samples[sample_idx]['query'], self.samples[sample_idx][
                 'choices'], self.samples[sample_idx]['gold'],
             if len(preamble) > 0:
                 query = f'{example_delimiter}{query}'
 
@@ -584,23 +617,52 @@
             'gold_indices': gold_idxs,
             'choice_groupings': choice_groupings
         }
         batch['attention_mask'] = ~(batch['input_ids'] == self.pad_tok_id)
         return batch
 
     def get_num_samples_in_batch(self, batch) -> int:
-        return batch['input_ids'].shape[0]
+        return batch['input_ids'].shape[0] // self.num_choices
 
     def split_batch(self, batch: Any, microbatch_size: int):
-        if self.get_num_samples_in_batch(batch) // self.num_choices > microbatch_size:
-            raise Exception('Multiple choice tasks do not currently support batch splitting. Please set '
-                            'dataloader batch size to a value less than or equal to the microbatch size. '
-                            'Accordingly, auto microbatching does not work, so the microbatch size '
-                            'should be manually set if using a batch size which does not fit in memory.')
-        return [batch]
+        """Split batch while ensuring all continuations are in the same microbatch.
+
+        In ICL Multiple Choice, we duplicate each data point for each possible continuation.
+        When splitting a batch, we have logical samples, which refer to one possible question,
+        and real samples, which refers to one possible continuation. As sample count and
+        microbatch_size are tracked in logical samples, we split logical attributes by
+        microbatch_size and real attributes by microbatch_size * num_choices.
+        """
+        no_split = ['mode']
+        # Real
+        real = ['input_ids', 'labels', 'attention_mask']
+        logical = ['gold_indices']
+        chunked = {}
+        for k, v in batch.items():
+            if k in no_split:
+                # Defer broadcasting primitives until we know num_chunks
+                pass
+            elif k == 'continuation_indices':
+                # List of list, so we have to directly call _split_list
+                chunked[k] = _split_list(v, microbatch_size * self.num_choices)
+            elif k == 'choice_groupings':
+                # List of list, so we have to directly call _split_list
+                chunked[k] = _split_list(v, microbatch_size)
+            elif k in real:
+                chunked[k] = _default_split_batch(v, microbatch_size * self.num_choices)
+            elif k in logical:
+                chunked[k] = _default_split_batch(v, microbatch_size)
+            else:
+                raise ValueError(f'Unexpected key {k}')
+        num_chunks = len(chunked['input_ids'])
+        # Broadcast primitives to all chunks
+        for k, v in batch.items():
+            if isinstance(v, (int, float, str, bool)):
+                chunked[k] = [v] * num_chunks
+        return [{k: v[idx] for k, v in chunked.items()} for idx in range(num_chunks)]
 
 
 class InContextLearningSchemaTaskDataset(InContextLearningMultipleChoiceTaskDataset):
     """A dataset that constructs batches for in-context learning schema evaluation
     A schema task involves sentences with a fill-in-the-blank where the user needs to choose the correct word
     to fill in from a set of N options. We use the partial evaluation technique from https://arxiv.org/abs/1806.02847
     to determine the model's choice of fill-in word.
@@ -654,14 +716,16 @@
         self.samples = list(
             dataset.map(
                 lambda examples: {
                     'context_options': examples['context_options'],
                     'continuation': examples['continuation'],
                     'gold': examples['gold']
                 }))
+        self.samples = strip_data(self.samples)
+
         self.num_choices = len(self.samples[0]['context_options'])
         self.tokenizer = tokenizer
         self.max_seq_len = max_seq_len
         self.pad_tok_id = pad_tok_id
         fewshot_rng = random.Random(fewshot_random_seed)
 
         self.prefix_space = _tokenizer_needs_prefix_space(self.tokenizer)
@@ -693,14 +757,15 @@
 
             preamble = prompt_string
             if num_fewshot > 0:
                 fewshot_idxs = _get_fewshot_sample_idxs(len(self.samples), num_fewshot, sample_idx, fewshot_rng)
                 for fewshot_idx in fewshot_idxs:
                     context_options, continuation, gold_idx = self.samples[fewshot_idx][
                         'context_options'], self.samples[fewshot_idx]['continuation'], self.samples[fewshot_idx]['gold']
+                    assert isinstance(gold_idx, int)
                     context = context_options[gold_idx]
                     if len(preamble) > 0:
                         context = f'{example_delimiter}{context}'
                     preamble += f'{context}{continuation_delimiter}{continuation}'
 
             encoded_example = {}
             context_options, continuation, gold_idx = self.samples[sample_idx]['context_options'], self.samples[
@@ -839,24 +904,28 @@
                                                  fewshot_random_seed=fewshot_random_seed)
         effective_batchsize = batch_size
     else:
         raise Exception(f'Unrecognized ICL task type: {icl_task_type}')
 
     sampler = dist.get_sampler(dataset, drop_last=False, shuffle=False)
 
+    split_batch = None
+    if isinstance(dataset, (InContextLearningMultipleChoiceTaskDataset, InContextLearningQATaskDataset)):
+        split_batch = dataset.split_batch
+
     return DataSpec(
         DataLoader(
             dataset,
             batch_size=effective_batchsize,
             sampler=sampler,
             collate_fn=dataset.collate_fn,
         ),
         device_transforms=None,
         get_num_samples_in_batch=dataset.get_num_samples_in_batch,
-        split_batch=dataset.split_batch if isinstance(dataset, InContextLearningMultipleChoiceTaskDataset) else None,
+        split_batch=split_batch,
     )
 
 
 def partition_dataset_by_category(dataset_uri: str, destination_path: str) -> Dict[str, str]:
     """If has_categories is enabled, we partition the dataset into a separate dataset for each category value in the data and write each partition to a local file.
 
     Args:
```

### Comparing `composer-0.14.1/composer/datasets/lm_dataset.py` & `composer-0.15.0/composer/datasets/lm_dataset.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/datasets/mnist.py` & `composer-0.15.0/composer/datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/datasets/synthetic.py` & `composer-0.15.0/composer/datasets/synthetic.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/datasets/utils.py` & `composer-0.15.0/composer/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/devices/device.py` & `composer-0.15.0/composer/devices/device.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/devices/device_cpu.py` & `composer-0.15.0/composer/devices/device_cpu.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/devices/device_gpu.py` & `composer-0.15.0/composer/devices/device_gpu.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/devices/device_mps.py` & `composer-0.15.0/composer/devices/device_mps.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/devices/device_tpu.py` & `composer-0.15.0/composer/devices/device_tpu.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/functional/__init__.py` & `composer-0.15.0/composer/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/loggers/__init__.py` & `composer-0.15.0/composer/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/loggers/cometml_logger.py` & `composer-0.15.0/composer/loggers/cometml_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/loggers/console_logger.py` & `composer-0.15.0/composer/loggers/console_logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,16 @@
                  log_traces: bool = False) -> None:
 
         if isinstance(log_interval, int):
             log_interval = Time(log_interval, TimeUnit.EPOCH)
         if isinstance(log_interval, str):
             log_interval = Time.from_timestring(log_interval)
 
+        self.last_logged_batch = 0
+
         if log_interval.unit not in (TimeUnit.EPOCH, TimeUnit.BATCH):
             raise ValueError('The `console_log_interval` argument must have units of EPOCH or BATCH.')
 
         self.log_interval = log_interval
         # set the stream
         if isinstance(stream, str):
             if stream.lower() == 'stdout':
@@ -92,29 +94,32 @@
 
     def epoch_end(self, state: State, logger: Logger) -> None:
         cur_epoch = int(state.timestamp.epoch)  # epoch gets incremented right before EPOCH_END
         unit = self.log_interval.unit
 
         if unit == TimeUnit.EPOCH and (cur_epoch % int(self.log_interval) == 0 or cur_epoch == 1):
             self.log_to_console(self.logged_metrics, prefix='Train ', state=state)
-        # Always clear logged metrics so they don't get logged in a subsequent eval call. The
-        # metrics will be recomputed and overridden in future batches so they can be safely
-        # discarded.
-        self.logged_metrics = {}
+            self.last_logged_batch = int(state.timestamp.batch)
+            self.logged_metrics = {}  # Clear logged metrics.
 
     def batch_end(self, state: State, logger: Logger) -> None:
         cur_batch = int(state.timestamp.batch)
         unit = self.log_interval.unit
         if unit == TimeUnit.BATCH and (cur_batch % int(self.log_interval) == 0 or cur_batch == 1):
             self.log_to_console(self.logged_metrics, prefix='Train ', state=state)
-            # Clear logged metrics.
-            self.logged_metrics = {}
+            self.last_logged_batch = cur_batch
+            self.logged_metrics = {}  # Clear logged metrics.
 
     def fit_end(self, state: State, logger: Logger) -> None:
         # Always clear logged metrics so they don't get logged in a subsequent eval call.
+        cur_batch = int(state.timestamp.batch)
+        if self.last_logged_batch != cur_batch:
+            self.log_to_console(self.logged_metrics, prefix='Train ',
+                                state=state)  # log at the end of training if you didn't just log
+
         self.logged_metrics = {}
 
     def eval_batch_end(self, state: State, logger: Logger) -> None:
         cur_batch = int(state.eval_timestamp.batch)
         if cur_batch in self.eval_batch_idxs_to_log:
             self.log_to_console({}, prefix='Eval ', state=state, is_train=False)
 
@@ -130,14 +135,15 @@
 
     def predict_start(self, state: State, logger: Logger) -> None:
         if not self.hparams_already_logged_to_console:
             self.hparams_already_logged_to_console = True
             self._log_hparams_to_console()
 
     def eval_start(self, state: State, logger: Logger) -> None:
+        self.logged_metrics = {}  # Clear logged metrics before eval so they don't get logged subsequently.
         total_eval_batches = self._get_total_eval_batches(state)
         deciles = np.linspace(0, 1, NUM_EVAL_LOGGING_EVENTS)
         batch_idxs = np.arange(1, total_eval_batches + 1)
         if total_eval_batches < NUM_EVAL_LOGGING_EVENTS:
             self.eval_batch_idxs_to_log = list(batch_idxs)
         else:
             self.eval_batch_idxs_to_log = list(np.quantile(batch_idxs, deciles).round().astype(dtype=int))
```

### Comparing `composer-0.14.1/composer/loggers/file_logger.py` & `composer-0.15.0/composer/loggers/file_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/loggers/in_memory_logger.py` & `composer-0.15.0/composer/loggers/in_memory_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/loggers/logger.py` & `composer-0.15.0/composer/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/loggers/logger_destination.py` & `composer-0.15.0/composer/loggers/logger_destination.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/loggers/mlflow_logger.py` & `composer-0.15.0/composer/loggers/mlflow_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/loggers/mosaicml_logger.py` & `composer-0.15.0/composer/loggers/mosaicml_logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,19 +10,22 @@
 import logging
 import operator
 import os
 import time
 from functools import reduce
 from typing import TYPE_CHECKING, Any, Dict, List, Optional
 
+import mcli
 import torch
 
+from composer.loggers import Logger
 from composer.loggers.logger import Logger
 from composer.loggers.logger_destination import LoggerDestination
-from composer.utils import MissingConditionalImportError, dist
+from composer.loggers.wandb_logger import WandBLogger
+from composer.utils import dist
 
 if TYPE_CHECKING:
     from composer.core import State
 
 log = logging.getLogger(__name__)
 
 __all__ = ['MosaicMLLogger']
@@ -58,35 +61,36 @@
         self.log_interval = log_interval
         self.ignore_keys = ignore_keys
         self._enabled = dist.get_global_rank() == 0
         if self._enabled:
             self.time_last_logged = 0
             self.buffered_metadata: Dict[str, Any] = {}
 
-            try:
-                import mcli
-                del mcli
-            except ImportError as e:
-                raise MissingConditionalImportError(extra_deps_group='mcli',
-                                                    conda_package='mcli',
-                                                    conda_channel='conda-forge') from e
             self.run_name = os.environ.get(RUN_NAME_ENV_VAR)
             if self.run_name is not None:
                 log.info(f'Logging to mosaic run {self.run_name}')
             else:
                 log.warning(f'Environment variable `{RUN_NAME_ENV_VAR}` not set, so MosaicMLLogger '
                             'is disabled as it is unable to identify which run to log to.')
                 self._enabled = False
 
     def log_hyperparameters(self, hyperparameters: Dict[str, Any]):
         self._log_metadata(hyperparameters)
 
     def log_metrics(self, metrics: Dict[str, Any], step: Optional[int] = None) -> None:
         self._log_metadata(metrics)
 
+    def after_load(self, state: State, logger: Logger) -> None:
+        # Log WandB run URL if it exists. Must run on after_load as WandB is setup on event init
+        for callback in state.callbacks:
+            if isinstance(callback, WandBLogger):
+                run_url = callback.run_url
+                if run_url is not None:
+                    self._log_metadata({'wandb/run_url': run_url})
+
     def batch_end(self, state: State, logger: Logger) -> None:
         self._flush_metadata()
 
     def epoch_end(self, state: State, logger: Logger) -> None:
         self._flush_metadata()
 
     def fit_end(self, state: State, logger: Logger) -> None:
@@ -109,21 +113,19 @@
                     continue
                 self.buffered_metadata[f'mosaicml/{key}'] = format_data_to_json_serializable(val)
             self._flush_metadata()
 
     def _flush_metadata(self, force_flush: bool = False) -> None:
         """Flush buffered metadata to MosaicML if enough time has passed since last flush."""
         if self._enabled and (time.time() - self.time_last_logged > self.log_interval or force_flush):
-            from mcli.api.exceptions import MAPIException
-            from mcli.sdk import update_run_metadata
             try:
-                update_run_metadata(self.run_name, self.buffered_metadata)
+                mcli.update_run_metadata(self.run_name, self.buffered_metadata)
                 self.buffered_metadata = {}
                 self.time_last_logged = time.time()
-            except MAPIException as e:
+            except mcli.MAPIException as e:
                 log.error(f'Failed to log metadata to Mosaic with error: {e}')
 
 
 def format_data_to_json_serializable(data: Any):
     """Recursively formats data to be JSON serializable.
 
     Args:
```

### Comparing `composer-0.14.1/composer/loggers/progress_bar_logger.py` & `composer-0.15.0/composer/loggers/progress_bar_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,20 +20,15 @@
 if TYPE_CHECKING:
     from composer.core import State, Timestamp
 
 __all__ = ['ProgressBarLogger']
 
 _IS_TRAIN_TO_KEYS_TO_LOG = {
     True: ['loss/train'],
-    False: [
-        'metrics/eval/Accuracy',
-        'metrics/eval/BinaryAccuracy',
-        'metrics/eval/MulticlassAccuracy',
-        'metrics/eval/MultilabelAccuracy',
-    ],
+    False: ['eval'],
 }
 
 
 class _ProgressBar:
 
     def __init__(
         self,
```

### Comparing `composer-0.14.1/composer/loggers/remote_uploader_downloader.py` & `composer-0.15.0/composer/loggers/remote_uploader_downloader.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/loggers/slack_logger.py` & `composer-0.15.0/composer/loggers/slack_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/loggers/tensorboard_logger.py` & `composer-0.15.0/composer/loggers/tensorboard_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/loggers/wandb_logger.py` & `composer-0.15.0/composer/loggers/wandb_logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,14 +103,15 @@
 
         # Set these variable directly to allow fetching an Artifact **without** initializing a WandB run
         # When used as a LoggerDestination, these values are overriden from global rank 0 to all ranks on Event.INIT
         self.entity = entity
         self.project = project
 
         self.run_dir: Optional[str] = None
+        self.run_url: Optional[str] = None
 
     def _set_is_in_atexit(self):
         self._is_in_atexit = True
 
     def log_hyperparameters(self, hyperparameters: Dict[str, Any]):
         if self._enabled:
             import wandb
@@ -200,14 +201,15 @@
             self._init_kwargs['name'] += f'-rank{dist.get_global_rank()}'
             self._init_kwargs['group'] = self._init_kwargs['group'] if 'group' in self._init_kwargs else name
         if self._enabled:
             wandb.init(**self._init_kwargs)
             assert wandb.run is not None, 'The wandb run is set after init'
             entity_and_project = [str(wandb.run.entity), str(wandb.run.project)]
             self.run_dir = wandb.run.dir
+            self.run_url = wandb.run.get_url()
             atexit.register(self._set_is_in_atexit)
         else:
             entity_and_project = [None, None]
         # Share the entity and project across all ranks, so they are available on ranks that did not initialize wandb
         dist.broadcast_object_list(entity_and_project)
         self.entity, self.project = entity_and_project
         assert self.entity is not None, 'entity should be defined'
@@ -286,15 +288,15 @@
         try:
             wandb_artifact = api.artifact('/'.join([self.entity, self.project, new_remote_file_name]))
         except wandb.errors.CommError as e:
             if 'does not contain artifact' in str(e):
                 raise FileNotFoundError(f'WandB Artifact {new_remote_file_name} not found') from e
             raise e
         with tempfile.TemporaryDirectory() as tmpdir:
-            wandb_artifact_folder = os.path.join(tmpdir, 'wandb_artifact_folder')
+            wandb_artifact_folder = os.path.join(tmpdir, 'wandb_artifact_folder/')
             wandb_artifact.download(root=wandb_artifact_folder)
             wandb_artifact_names = os.listdir(wandb_artifact_folder)
             # We only log one file per artifact
             if len(wandb_artifact_names) > 1:
                 raise RuntimeError(
                     'Found more than one file in WandB artifact. We assume the checkpoint is the only file in the WandB artifact.'
                 )
```

### Comparing `composer-0.14.1/composer/loss/loss.py` & `composer-0.15.0/composer/loss/loss.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/loss/utils.py` & `composer-0.15.0/composer/loss/utils.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/metrics/__init__.py` & `composer-0.15.0/composer/metrics/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 # Copyright 2022 MosaicML Composer authors
 # SPDX-License-Identifier: Apache-2.0
 
 """A collection of common torchmetrics."""
 
 from composer.metrics.map import MAP
 from composer.metrics.metrics import CrossEntropy, Dice, LossMetric, MIoU
-from composer.metrics.nlp import (BinaryF1Score, HFCrossEntropy, InContextLearningLMAccuracy,
+from composer.metrics.nlp import (BinaryF1Score, InContextLearningLMAccuracy,
                                   InContextLearningLMExpectedCalibrationError,
                                   InContextLearningMCExpectedCalibrationError, InContextLearningMetric,
                                   InContextLearningMultipleChoiceAccuracy, InContextLearningQAAccuracy,
-                                  LanguageCrossEntropy, LanguagePerplexity, MaskedAccuracy, Perplexity)
+                                  LanguageCrossEntropy, LanguagePerplexity, MaskedAccuracy)
 
 __all__ = [
     'MAP',
     'MIoU',
     'Dice',
     'CrossEntropy',
     'LossMetric',
-    'Perplexity',
     'BinaryF1Score',
-    'HFCrossEntropy',
     'LanguageCrossEntropy',
     'MaskedAccuracy',
     'LanguagePerplexity',
     'InContextLearningLMAccuracy',
     'InContextLearningMultipleChoiceAccuracy',
     'InContextLearningQAAccuracy',
     'InContextLearningMCExpectedCalibrationError',
```

### Comparing `composer-0.14.1/composer/metrics/map.py` & `composer-0.15.0/composer/metrics/map.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/metrics/metrics.py` & `composer-0.15.0/composer/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/metrics/nlp.py` & `composer-0.15.0/composer/metrics/nlp.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 # Copyright 2022 MosaicML Composer authors
 # SPDX-License-Identifier: Apache-2.0
 
 """A collection of common torchmetrics for NLP tasks."""
 import re
 import string
-import warnings
-from typing import Any, Dict, List, Mapping, Optional, Union
+from typing import Any, Dict, List, Mapping, Union
 
 import torch
 from torch import Tensor
 from torch.nn import functional as F
 from torchmetrics import Metric
 
-from composer.loss import soft_cross_entropy
-
 __all__ = [
-    'Perplexity',
     'InContextLearningLMAccuracy',
     'InContextLearningMultipleChoiceAccuracy',
     'InContextLearningQAAccuracy',
     'BinaryF1Score',
-    'HFCrossEntropy',
     'LanguageCrossEntropy',
     'MaskedAccuracy',
     'LanguagePerplexity',
     'InContextLearningLMExpectedCalibrationError',
     'InContextLearningMCExpectedCalibrationError',
 ]
 
@@ -76,32 +71,25 @@
     """Torchmetric that computes cross entropy on language modeling outputs.
 
     Adds metric state variables:
         sum_loss (float): The sum of the per-example loss in the batch.
         total_items (float): The number of batches to average across.
 
     Args:
-        vocab_size (int): The size of the tokenizer vocabulary.
         dist_sync_on_step (bool, optional): Synchronize metric state across processes at
             each forward() before returning the value at the step. Default: ``False``.
         ignore_index (int, optional): The class index to ignore. Default: ``-100``.
     """
 
     # Make torchmetrics call update only once
     full_state_update = False
 
-    def __init__(self, vocab_size: Optional[int] = None, dist_sync_on_step: bool = False, ignore_index: int = -100):
+    def __init__(self, dist_sync_on_step: bool = False, ignore_index: int = -100):
         super().__init__(dist_sync_on_step=dist_sync_on_step)
 
-        if vocab_size is not None:
-            warnings.warn(
-                DeprecationWarning(
-                    'The vocab_size argument is deprecated and will be removed in 0.15. It is no longer needed, because the correct shape of output and target is inferred based on the number of target elements.'
-                ))
-
         self.ignore_index = ignore_index
         self.loss_fn = torch.nn.CrossEntropyLoss(ignore_index=ignore_index, reduction='sum')
         self.add_state('sum_loss', default=torch.tensor(0.), dist_reduce_fx='sum')
         self.add_state('total_items', default=torch.tensor(0), dist_reduce_fx='sum')
 
     def update(self, output: Union[Mapping, Tensor], target: Tensor) -> None:
         """Updates the internal state with results from a new batch.
@@ -183,99 +171,14 @@
         assert isinstance(self.true_positive, Tensor)
         assert isinstance(self.false_positive, Tensor)
         assert isinstance(self.false_negative, Tensor)
         f1 = (self.true_positive) / (self.true_positive + (0.5 * (self.false_negative + self.false_positive)))
         return f1
 
 
-class HFCrossEntropy(Metric):
-    """Hugging Face compatible cross entropy loss.
-
-    Adds metric state variables:
-        sum_loss (float): The sum of the per-example loss in the batch.
-        total_batches (float): The number of batches to average across.
-
-    Args:
-        dist_sync_on_step (bool, optional): Synchronize metric state across processes at
-            each forward() before returning the value at the step. Default: ``False``
-    """
-
-    # Make torchmetrics call update only once
-    full_state_update = False
-
-    def __init__(self, dist_sync_on_step=False):
-        warnings.warn(
-            DeprecationWarning(
-                "'HFCrossEntropy' is deprecated and will be removed in 0.15. Please use `LanguageCrossEntropy' instead."
-            ))
-
-        super().__init__(dist_sync_on_step=dist_sync_on_step)
-
-        self.add_state('sum_loss', default=torch.tensor(0.), dist_reduce_fx='sum')
-        self.add_state('total_batches', default=torch.tensor(0), dist_reduce_fx='sum')
-
-    def update(self, output: Union[Mapping, Tensor], target: Tensor) -> None:
-        """Updates the internal state with results from a new batch.
-
-        Args:
-            output (Mapping): The output from the model, which must contain
-                either the Tensor or a Mapping type that contains the loss or model logits.
-            target (~torch.Tensor): A Tensor of ground-truth values to compare against.
-        """
-        # if logit modification algorithms aren't on, we take the loss directly from the model output
-        if isinstance(output, Mapping) and 'loss' in output:
-            loss = output['loss']
-        else:
-            if isinstance(output, Mapping):
-                logits = output['logits']
-            # recompute the loss on our own
-            elif isinstance(output, Tensor):
-                logits = output
-            else:
-                raise Exception(f'Type {type(output)} for the output is unsupported.')
-
-            loss = soft_cross_entropy(logits, target)
-
-        # accumulate loss over all batches
-        self.sum_loss += loss
-
-        # Note: This is a slightly different reduction than LanguageCrossEntropy, because LanguageCrossEntropy
-        # uses 'sum' reduction in its update call
-        self.total_batches += 1  #type: ignore (third-party)
-
-    def compute(self) -> Tensor:
-        """Aggregate the state over all processes to compute the metric.
-
-        Returns:
-            loss: The loss averaged across all batches as a :class:`~torch.Tensor`.
-        """
-        # Return average loss over entire dataset
-        return self.sum_loss / self.total_batches  #type: ignore (third-party)
-
-
-class Perplexity(HFCrossEntropy):
-    """Subclasses :class:`~composer.metrics.nlp.HFCrossEntropy` to implement perplexity.
-
-    If an algorithm modifies the loss function and it is no longer directly provided in the output, then this could be
-    expensive because it'll compute the loss twice.
-    """
-
-    def __init__(self, dist_sync_on_step=False):
-        warnings.warn(
-            DeprecationWarning(
-                "'Perplexity' is deprecated and will be removed in 0.15. Please use `LanguagePerplexity' instead."))
-
-        super().__init__(dist_sync_on_step=dist_sync_on_step)
-
-    def compute(self) -> Tensor:
-        """Returns torch.exp() of the HFCrossEntropy."""
-        avg_loss = super().compute()
-        return torch.exp(avg_loss)
-
-
 class LanguagePerplexity(LanguageCrossEntropy):
     """Subclasses :class:`~composer.metrics.nlp.LanguageCrossEntropy` to implement perplexity."""
 
     def compute(self) -> Tensor:
         """Returns torch.exp() of the LanguageCrossEntropy."""
         avg_loss = super().compute()
         return torch.exp(avg_loss)
```

### Comparing `composer-0.14.1/composer/models/__init__.py` & `composer-0.15.0/composer/models/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/models/base.py` & `composer-0.15.0/composer/models/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # SPDX-License-Identifier: Apache-2.0
 
 """The ComposerModel base interface."""
 from __future__ import annotations
 
 import abc
 import copy
-import warnings
 from typing import Any, Dict, Optional, Sequence, Union
 
 import torch
 from torch import Tensor
 from torchmetrics import Metric
 
 from composer.core import Batch
@@ -156,56 +155,14 @@
                 optimizer.zero_grad()
                 outputs = model.forward(batch)
                 loss = model.loss(outputs, batch)
                 loss.backward()
         """
         pass
 
-    def metrics(self, train: bool = False) -> Dict[str, Metric]:
-        """Get metrics for evaluating the model. Metrics should be instances of :class:`torchmetrics.Metric` defined in
-        :meth:`__init__`. This format enables accurate distributed logging. Metrics consume the outputs of
-        :meth:`validate`. To track multiple metrics, return a list of metrics in a :ref:`MetricCollection
-        </pages/overview.rst#metriccollection>`.
-
-        Args:
-            train (bool, optional): True to return metrics that should be computed
-                during training and False otherwise. This flag is set automatically by the
-                :class:`.Trainer`. Default: ``False``.
-
-        Returns:
-             Metric or MetricCollection: An instance of :class:`~torchmetrics.Metric` or :ref:`MetricCollection </pages/overview.rst#metriccollection>`.
-
-        .. warning:: Each metric keeps states which are updated with data seen so far.
-                     As a result, different metric instances should be used for training
-                     and validation. See:
-                     https://torchmetrics.readthedocs.io/en/latest/pages/overview.html
-                     for more details.
-
-        Example:
-
-        .. code-block:: python
-
-            from torchmetrics.classification import MulticlassAccuracy
-            from composer.models.loss import CrossEntropyLoss
-
-            def __init__(self, num_classes):
-                super().__init__()
-                self.train_acc = MulticlassAccuracy(num_classes=num_classes, average='micro') # torchmetric
-                self.val_acc = MulticlassAccuracy(num_classes=num_classes, average='micro')
-                self.val_loss = CrossEntropyLoss()
-
-            def metrics(self, train: bool = False):
-                return self.train_acc if train else MetricCollection([self.val_acc, self.val_loss])
-        """
-        warnings.warn(
-            DeprecationWarning(
-                'Using ``metrics()`` is no longer supported and will be removed in a future version. Please use ``get_metrics()`` instead.'
-            ))
-        return self.get_metrics(train)
-
     def eval_forward(
         self,
         batch: Any,
         outputs: Optional[Any] = None,
     ) -> Any:
         """Run the evaluation forward pass.
 
@@ -241,16 +198,16 @@
     def get_metrics(self, is_train: bool) -> Dict[str, Metric]:
         """Get the metrics.
 
         This method will be called by the trainer immediately after :attr:`.Event.INIT`.
 
         .. note::
 
-            Each item in the returned dictionary will be ``copy.deepcopy`` before it is used. This is to ensure that each dataloader (e.g. train, eval)
-            will be accumulating metrics separately.
+            Each item in the returned dictionary will be ``copy.deepcopy`` before it is used. This
+            is to ensure that each dataloader (e.g. train, eval) will be accumulating metrics separately.
 
             To share a metric across all dataloaders, wrap it with ``MetricSpec(metric=metric, share=False)``.
 
         Args:
             is_train (bool): Whether the training metrics or evaluation metrics should be returned.
 
         Returns:
```

### Comparing `composer-0.14.1/composer/models/bert/model.py` & `composer-0.15.0/composer/models/bert/model.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/models/classify_mnist/model.py` & `composer-0.15.0/composer/models/classify_mnist/model.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/models/deeplabv3/model.py` & `composer-0.15.0/composer/models/deeplabv3/model.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/models/efficientnetb0/__init__.py` & `composer-0.15.0/composer/models/efficientnetb0/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/models/efficientnetb0/_layers.py` & `composer-0.15.0/composer/models/efficientnetb0/_layers.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/models/efficientnetb0/efficientnets.py` & `composer-0.15.0/composer/models/efficientnetb0/efficientnets.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/models/efficientnetb0/model.py` & `composer-0.15.0/composer/models/efficientnetb0/model.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/models/gpt2/__init__.py` & `composer-0.15.0/composer/models/gpt2/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/models/gpt2/model.py` & `composer-0.15.0/composer/models/gpt2/model.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/models/huggingface.py` & `composer-0.15.0/composer/models/huggingface.py`

 * *Files 10% similar despite different names*

```diff
@@ -136,20 +136,137 @@
             log.warning('The shift_labels argument was set to False but the model is an instance of a'
                         ' HuggingFace Causal LM. This may lead to incorrect behavior.')
             # Note: No warning if shift_labels and not is_causal_lm, since the model may simply be a custom class.
 
         self.dummy_forward_called = False
 
     @staticmethod
+    def load_huggingface_tokenizer_from_saved_state(
+            hf_state: Dict[str, Any]) -> Optional[transformers.PreTrainedTokenizer]:
+        """A helper function that loads a HuggingFace tokenizer from a loaded in hf state.
+
+        Args:
+            hf_state (Dict[str, Any]): HF state loaded from a Composer checkpoint.
+
+        Returns:
+            Optional[transformers.PreTrainedTokenizer]: The loaded HuggingFace tokenizer
+        """
+        try:
+            import transformers
+        except ImportError as e:
+            raise MissingConditionalImportError(extra_deps_group='nlp',
+                                                conda_package='transformers',
+                                                conda_channel='conda-forge') from e
+        hf_tokenizer = None
+        hf_tokenizer_state = hf_state['tokenizer']
+        if hf_tokenizer_state != {}:
+            with tempfile.TemporaryDirectory() as _tmp_dir:
+                for filename, saved_content in hf_tokenizer_state.items():
+                    tokenizer_file_path = Path(_tmp_dir) / f'{filename}{saved_content["file_extension"]}'
+                    if saved_content['file_extension'] == '.json':
+                        with open(tokenizer_file_path, 'w') as _tmp_file:
+                            json.dump(saved_content['content'], _tmp_file)
+                    elif saved_content['file_extension'] == '.txt':
+                        with open(tokenizer_file_path, 'w') as _tmp_file:
+                            for line in saved_content['content']:
+                                _tmp_file.write(line)
+                                _tmp_file.write('\n')
+                    elif saved_content['file_extension'] == '.model':
+                        try:
+                            import sentencepiece as spm
+                        except ImportError as e:
+                            raise MissingConditionalImportError(extra_deps_group='sentencepiece',
+                                                                conda_package='sentencepiece') from e
+                        s = spm.SentencePieceProcessor()
+                        s.load_from_serialized_proto(saved_content['content'])
+                        with open(tokenizer_file_path, 'wb') as _tmp_file:
+                            _tmp_file.write(s.serialized_model_proto())
+                hf_tokenizer = transformers.AutoTokenizer.from_pretrained(_tmp_dir, trust_remote_code=True)
+
+                # we need to set the name_or_path back because otherwise it is the tmp dir we are loading from here
+                hf_tokenizer.name_or_path = hf_tokenizer_state['tokenizer_config']['content'].get('name_or_path', '')
+                hf_tokenizer.init_kwargs['name_or_path'] = hf_tokenizer.name_or_path
+
+                # for an unknown reason this key is missing when loading the saved tokenizer, but present with a value of None
+                # for the original tokenizer, so we default it to None
+                hf_tokenizer.init_kwargs['tokenizer_file'] = hf_tokenizer.init_kwargs.get('tokenizer_file', None)
+        return hf_tokenizer
+
+    @staticmethod
+    def load_huggingface_model_from_saved_state(
+            hf_state: Dict[str, Any], loaded_state_dict: Dict[str, Dict[str, Dict[str, Dict[str, Any]]]],
+            model_instantiation_class: type | str | None,
+            model_config_kwargs: Dict[str, Any] | None) -> transformers.PreTrainedModel:
+        """A helper function that loads a HuggingFace model class from a loaded in hf state.
+
+        Args:
+            hf_state (Dict[str, Any]): HF state loaded from a Composer checkpoint.
+            model_instantiation_class (Union[Type[:class:`transformers.PreTrainedModel`], Type[:class:`transformers.AutoModel`], str]), optional):
+                Class to use to create the HuggingFace model. Defaults to the model class used in the original checkpoint. If this argument is
+                a HuggingFace auto class (e.g. :class:`transformers.AutoModel` or :class:`transformers.AutoModelForSequenceClassification`), the ``from_config`` method will be used,
+                while if it is of type :class:`transformers.PreTrainedModel`, the constructor will be called. This argument can also be a string,
+                which will attempt to be imported as the class to use.
+            model_config_kwargs: Dict[str, Any]: Extra arguments to pass in for the model config creation (e.g. ``num_labels`` for creating a sequence classification model)
+        Returns:
+            transformers.PreTrainedModel: The loaded HuggingFace model
+        """
+        try:
+            import transformers
+        except ImportError as e:
+            raise MissingConditionalImportError(extra_deps_group='nlp',
+                                                conda_package='transformers',
+                                                conda_channel='conda-forge') from e
+        loaded_config = get_hf_config_from_composer_state_dict(loaded_state_dict, config_overrides=model_config_kwargs)
+
+        hf_model_state = hf_state['model']
+        if model_instantiation_class is not None:
+            # If the instantiation class is explicitly provided, use it
+            # If a string is provided, attempt to import the class it refers to
+            if isinstance(model_instantiation_class, str):
+                try:
+                    model_instantiation_class = import_object(':'.join(model_instantiation_class.rsplit('.',
+                                                                                                        maxsplit=1)))
+                except (ModuleNotFoundError, AttributeError):
+                    raise ValueError(
+                        textwrap.dedent(
+                            f'The provided model_instantiation_class string {model_instantiation_class} could not be imported. '
+                            f'Please make sure {model_instantiation_class} is discoverable on the python path, or pass the class '
+                            'in directly.'))
+
+            assert model_instantiation_class is not None  # pyright
+            # The AutoModel* classes have `from_config`, while the PreTrainedModel classes do not
+            # pyright can't tell this isn't a string at this point
+            if issubclass(
+                    model_instantiation_class,  # type: ignore
+                    transformers.models.auto.auto_factory._BaseAutoModelClass):
+                hf_model = model_instantiation_class.from_config(loaded_config)  # type: ignore
+            else:
+                hf_model = model_instantiation_class(loaded_config)  # type: ignore
+        else:
+            # If the instantiation class is not explicitly provided, attempt to import the saved class and use it
+            try:
+                saved_class = import_object(':'.join(hf_model_state['config']['class'].rsplit('.', maxsplit=1)))
+            except (ModuleNotFoundError, AttributeError):
+                raise ValueError(
+                    textwrap.dedent(
+                        f'The saved class {hf_model_state["config"]["class"]} could not be imported. '
+                        'Please either pass in the class to use explicitly via the model_instantiation_class '
+                        f'parameter, or make sure that {hf_model_state["config"]["class"]} is discoverable '
+                        'on the python path.'))
+            hf_model = saved_class(loaded_config)
+        return hf_model
+
+    @staticmethod
     def hf_from_composer_checkpoint(
         checkpoint_path: str,
         model_instantiation_class: Optional[Union[Type[transformers.PreTrainedModel], Type['_BaseAutoModelClass'],
                                                   str]] = None,
         model_config_kwargs: Optional[dict] = None,
-        local_checkpoint_save_location: Optional[Union[Path, str]] = None
+        local_checkpoint_save_location: Optional[Union[Path, str]] = None,
+        trust_remote_code: bool = False,
     ) -> Tuple[transformers.PreTrainedModel, Optional[transformers.PreTrainedTokenizer]]:
         """Loads a HuggingFace model (and tokenizer if present) from a composer checkpoint.
 
         .. note:: This function does not load the weights from the checkpoint. It just loads the correctly configured
             model and tokenizer classes.
 
         .. testsetup::
@@ -198,27 +315,22 @@
                 a HuggingFace auto class (e.g. :class:`transformers.AutoModel` or :class:`transformers.AutoModelForSequenceClassification`), the ``from_config`` method will be used,
                 while if it is of type :class:`transformers.PreTrainedModel`, the constructor will be called. This argument can also be a string,
                 which will attempt to be imported as the class to use.
             model_config_kwargs: Dict[str, Any]: Extra arguments to pass in for the model config creation (e.g. ``num_labels`` for creating a sequence classification model)
             local_checkpoint_save_location (Optional[Union[Path, str]], optional): If specified, where to save the checkpoint file to locally.
                                                                                    If the input ``checkpoint_path`` is already a local path, this will be a symlink.
                                                                                    Defaults to None, which will use a temporary file.
+            trust_remote_code (bool, optional): Whether to trust the remote code when loading the tokenizer. Defaults to False.
 
         Raises:
             ValueError: If the ``model_instantiation_class``, or the model class saved in the checkpoint, is not able to be imported
 
         Returns:
             Tuple[transformers.PreTrainedModel, Optional[transformers.PreTrainedTokenizer]]: The loaded HuggingFace model and (if present) tokenizer
         """
-        try:
-            import transformers
-        except ImportError as e:
-            raise MissingConditionalImportError(extra_deps_group='nlp',
-                                                conda_package='transformers',
-                                                conda_channel='conda-forge') from e
 
         # default local path to a tempfile if path is not provided
         if local_checkpoint_save_location is None:
             tmp_dir = tempfile.TemporaryDirectory()
             local_checkpoint_save_location = Path(tmp_dir.name) / 'local-composer-checkpoint.pt'
 
         if model_config_kwargs is None:
@@ -227,87 +339,18 @@
         # download the checkpoint file
         get_file(checkpoint_path, str(local_checkpoint_save_location))
 
         # load the state dict in
         loaded_state_dict = safe_torch_load(local_checkpoint_save_location)
 
         hf_state = loaded_state_dict['state']['integrations']['huggingface']
-        hf_model_state = hf_state['model']
-        hf_tokenizer_state = hf_state['tokenizer']
-
-        loaded_config = get_hf_config_from_composer_state_dict(loaded_state_dict, config_overrides=model_config_kwargs)
-
-        if model_instantiation_class is not None:
-            # If the instantiation class is explicitly provided, use it
-            # If a string is provided, attempt to import the class it refers to
-            if isinstance(model_instantiation_class, str):
-                try:
-                    model_instantiation_class = import_object(':'.join(model_instantiation_class.rsplit('.',
-                                                                                                        maxsplit=1)))
-                except (ModuleNotFoundError, AttributeError):
-                    raise ValueError(
-                        textwrap.dedent(
-                            f'The provided model_instantiation_class string {model_instantiation_class} could not be imported. '
-                            f'Please make sure {model_instantiation_class} is discoverable on the python path, or pass the class '
-                            'in directly.'))
-
-            assert model_instantiation_class is not None  # pyright
-            # The AutoModel* classes have `from_config`, while the PreTrainedModel classes do not
-            # pyright can't tell this isn't a string at this point
-            if issubclass(
-                    model_instantiation_class,  # type: ignore
-                    transformers.models.auto.auto_factory._BaseAutoModelClass):
-                hf_model = model_instantiation_class.from_config(loaded_config)  # type: ignore
-            else:
-                hf_model = model_instantiation_class(loaded_config)  # type: ignore
-        else:
-            # If the instantiation class is not explicitly provided, attempt to import the saved class and use it
-            try:
-                saved_class = import_object(':'.join(hf_model_state['config']['class'].rsplit('.', maxsplit=1)))
-            except (ModuleNotFoundError, AttributeError):
-                raise ValueError(
-                    textwrap.dedent(
-                        f'The saved class {hf_model_state["config"]["class"]} could not be imported. '
-                        'Please either pass in the class to use explicitly via the model_instantiation_class '
-                        f'parameter, or make sure that {hf_model_state["config"]["class"]} is discoverable '
-                        'on the python path.'))
-            hf_model = saved_class(loaded_config)
-
-        hf_tokenizer = None
-        if hf_tokenizer_state != {}:
-            with tempfile.TemporaryDirectory() as _tmp_dir:
-                for filename, saved_content in hf_tokenizer_state.items():
-                    tokenizer_file_path = Path(_tmp_dir) / f'{filename}{saved_content["file_extension"]}'
-                    if saved_content['file_extension'] == '.json':
-                        with open(tokenizer_file_path, 'w') as _tmp_file:
-                            json.dump(saved_content['content'], _tmp_file)
-                    elif saved_content['file_extension'] == '.txt':
-                        with open(tokenizer_file_path, 'w') as _tmp_file:
-                            for line in saved_content['content']:
-                                _tmp_file.write(line)
-                                _tmp_file.write('\n')
-                    elif saved_content['file_extension'] == '.model':
-                        try:
-                            import sentencepiece as spm
-                        except ImportError as e:
-                            raise MissingConditionalImportError(extra_deps_group='sentencepiece',
-                                                                conda_package='sentencepiece') from e
-                        s = spm.SentencePieceProcessor()
-                        s.load_from_serialized_proto(saved_content['content'])
-                        with open(tokenizer_file_path, 'wb') as _tmp_file:
-                            _tmp_file.write(s.serialized_model_proto())
-                hf_tokenizer = transformers.AutoTokenizer.from_pretrained(_tmp_dir)
-
-                # we need to set the name_or_path back because otherwise it is the tmp dir we are loading from here
-                hf_tokenizer.name_or_path = hf_tokenizer_state['tokenizer_config']['content'].get('name_or_path', '')
-                hf_tokenizer.init_kwargs['name_or_path'] = hf_tokenizer.name_or_path
-
-                # for an unknown reason this key is missing when loading the saved tokenizer, but present with a value of None
-                # for the original tokenizer, so we default it to None
-                hf_tokenizer.init_kwargs['tokenizer_file'] = hf_tokenizer.init_kwargs.get('tokenizer_file', None)
+        hf_tokenizer = HuggingFaceModel.load_huggingface_tokenizer_from_saved_state(hf_state)
+        hf_model = HuggingFaceModel.load_huggingface_model_from_saved_state(hf_state, loaded_state_dict,
+                                                                            model_instantiation_class,
+                                                                            model_config_kwargs)
 
         return hf_model, hf_tokenizer
 
     def forward(self, batch):
         if isinstance(batch, Mapping):
             # Further input validation is left to the huggingface forward call
             batch = {k: v for k, v in batch.items() if k in self.model_forward_args}
@@ -368,15 +411,15 @@
                 output = output['logits']
             else:
                 # if loss was computed (cached outputs from forward), loss is at index 0 and logits are at index 1
                 # if loss was not computed (no cached outputs during eval), loss is not present and logits are at index 0
                 output = output[1] if len(output[0].shape) == 0 else output[0]
 
             # if we are in the single class case, then remove the classes dimension
-            if output.shape[1] == 1:
+            if output.ndim == 2 and output.shape[1] == 1:
                 output = output.squeeze(dim=1)
         else:
             output = outputs if outputs else self.forward(batch)
 
         return output
 
     def get_metrics(self, is_train: bool = False) -> Dict[str, Metric]:
@@ -420,14 +463,17 @@
                     tokenizer_file_extension = tokenizer_file_path.suffix
                     if tokenizer_file_extension == '.txt':
                         with open(tokenizer_file_path) as _tokenizer_file:
                             tokenizer_file_content = _tokenizer_file.read().split('\n')
                     elif tokenizer_file_extension == '.json':
                         with open(tokenizer_file_path) as _tokenizer_file:
                             tokenizer_file_content = json.load(_tokenizer_file)
+                    elif tokenizer_file_extension == '.py':
+                        with open(tokenizer_file_path) as _tokenizer_file:
+                            tokenizer_file_content = _tokenizer_file.read()
                     elif tokenizer_file_extension == '.model':
                         try:
                             import sentencepiece as spm
                         except ImportError as e:
                             raise MissingConditionalImportError(extra_deps_group='sentencepiece',
                                                                 conda_package='sentencepiece') from e
                         s = spm.SentencePieceProcessor(model_file=str(tokenizer_file_path))
@@ -601,13 +647,19 @@
         local_checkpoint_save_location = Path(tmp_dir.name) / 'local-composer-checkpoint.pt'
 
     # download the checkpoint file
     get_file(str(checkpoint_path), str(local_checkpoint_save_location))
 
     composer_state_dict = safe_torch_load(local_checkpoint_save_location)
 
+    # load tokenizer
+    hf_state = composer_state_dict['state']['integrations']['huggingface']
+    hf_tokenizer = HuggingFaceModel.load_huggingface_tokenizer_from_saved_state(hf_state)
+    assert hf_tokenizer is not None
+    hf_tokenizer.save_pretrained(output_folder)
+
     config = get_hf_config_from_composer_state_dict(composer_state_dict)
     config.save_pretrained(output_folder)
 
     weights_state_dict = composer_state_dict['state']['model']
     torch.nn.modules.utils.consume_prefix_in_state_dict_if_present(weights_state_dict, prefix='model.')
     torch.save(weights_state_dict, Path(output_folder) / 'pytorch_model.bin')
```

### Comparing `composer-0.14.1/composer/models/initializers.py` & `composer-0.15.0/composer/models/initializers.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/models/mmdetection.py` & `composer-0.15.0/composer/models/mmdetection.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/models/resnet/__init__.py` & `composer-0.15.0/composer/models/resnet/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/models/resnet/model.py` & `composer-0.15.0/composer/models/resnet/model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 # Copyright 2022 MosaicML Composer authors
 # SPDX-License-Identifier: Apache-2.0
 
 """A :class:`.ComposerClassifier` wrapper around the torchvision implementations of the ResNet model family."""
 
 import logging
-import textwrap
-import warnings
 from typing import List, Optional
 
-import torchvision
-from packaging import version
 from torchmetrics import MetricCollection
 from torchmetrics.classification import MulticlassAccuracy
 from torchvision.models import resnet
 
 from composer.loss import loss_registry
 from composer.metrics import CrossEntropy
 from composer.models.initializers import Initializer
@@ -25,30 +21,27 @@
 
 valid_model_names = ['resnet18', 'resnet34', 'resnet50', 'resnet101', 'resnet152']
 
 
 def composer_resnet(model_name: str,
                     num_classes: int = 1000,
                     weights: Optional[str] = None,
-                    pretrained: bool = False,
                     groups: int = 1,
                     width_per_group: int = 64,
                     initializers: Optional[List[Initializer]] = None,
                     loss_name: str = 'soft_cross_entropy') -> ComposerClassifier:
     """Helper function to create a :class:`.ComposerClassifier` with a torchvision ResNet model.
 
     From `Deep Residual Learning for Image Recognition <https://arxiv.org/abs/1512.03385>`_ (He et al, 2015).
 
     Args:
         model_name (str): Name of the ResNet model instance. Either [``"resnet18"``, ``"resnet34"``, ``"resnet50"``, ``"resnet101"``,
             ``"resnet152"``].
         num_classes (int, optional): The number of classes. Needed for classification tasks. Default: ``1000``.
         weights (str, optional): If provided, pretrained weights can be specified, such as with ``IMAGENET1K_V2``. Default: ``None``.
-        pretrained (bool, optional): If True, use ImageNet pretrained weights. Default: ``False``. This parameter is deprecated and
-            will soon be removed in favor of ``weights``.
         groups (int, optional): Number of filter groups for the 3x3 convolution layer in bottleneck blocks. Default: ``1``.
         width_per_group (int, optional): Initial width for each convolution group. Width doubles after each stage.
             Default: ``64``.
         initializers (List[Initializer], optional): Initializers for the model. ``None`` for no initialization.
             Default: ``None``.
         loss_name (str, optional): Loss function to use. E.g. 'soft_cross_entropy' or
             'binary_cross_entropy_with_logits'. Loss function must be in
@@ -80,39 +73,17 @@
                     'performance. '
                     'Please ensure you are using `initializers. '
                     'linear_log_constant_bias`.')
 
     if initializers is None:
         initializers = []
 
-    # Configure pretrained/weights based on torchvision version
-    if pretrained and weights:
-        raise ValueError(
-            'composer_resnet expects only one of ``pretrained`` or ``weights`` to be specified, but both were specified.'
-        )
-    if pretrained:
-        weights = 'IMAGENET1K_V2'
-        warnings.warn(
-            DeprecationWarning(
-                'The ``pretrained`` argument for composer_resnet is deprecated and will be removed in the future when torch 1.11 is no longer supported. Please use ``weights`` instead.'
-            ))
-
     # Instantiate model
     model_fn = getattr(resnet, model_name)
-    model = None
-    if version.parse(torchvision.__version__) < version.parse('0.13.0'):
-        if weights:
-            pretrained = True
-            warnings.warn(
-                textwrap.dedent(f'The current torchvision version {torchvision.__version__} does not support the '
-                                '``weights`` argument, so ``pretrained=True`` will be used instead. To enable '
-                                '``weights``, please upgrade to the latest version of torchvision.'))
-        model = model_fn(pretrained=pretrained, num_classes=num_classes, groups=groups, width_per_group=width_per_group)
-    else:
-        model = model_fn(weights=weights, num_classes=num_classes, groups=groups, width_per_group=width_per_group)
+    model = model_fn(weights=weights, num_classes=num_classes, groups=groups, width_per_group=width_per_group)
 
     # Grab loss function from loss registry
     loss_fn = loss_registry[loss_name]
 
     # Create metrics for train and validation
     train_metrics = MulticlassAccuracy(num_classes=num_classes, average='micro')
     val_metrics = MetricCollection([CrossEntropy(), MulticlassAccuracy(num_classes=num_classes, average='micro')])
```

### Comparing `composer-0.14.1/composer/models/resnet_cifar/__init__.py` & `composer-0.15.0/composer/models/resnet_cifar/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/models/resnet_cifar/model.py` & `composer-0.15.0/composer/models/resnet_cifar/model.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/models/resnet_cifar/resnets.py` & `composer-0.15.0/composer/models/resnet_cifar/resnets.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/models/tasks/classification.py` & `composer-0.15.0/composer/models/tasks/classification.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/models/timm/model.py` & `composer-0.15.0/composer/models/timm/model.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/models/unet/_layers.py` & `composer-0.15.0/composer/models/unet/_layers.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/models/unet/model.py` & `composer-0.15.0/composer/models/unet/model.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/models/unet/unet.py` & `composer-0.15.0/composer/models/unet/unet.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/models/vit_small_patch16/model.py` & `composer-0.15.0/composer/models/vit_small_patch16/model.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/optim/__init__.py` & `composer-0.15.0/composer/optim/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/optim/decoupled_weight_decay.py` & `composer-0.15.0/composer/optim/decoupled_weight_decay.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,15 +221,15 @@
         super().__init__(params=params, lr=lr, betas=betas, eps=eps, weight_decay=weight_decay, amsgrad=amsgrad)
         for group in self.param_groups:
             group['initial_lr'] = group['lr']
         self.amsgrad = amsgrad
 
     @staticmethod
     def adamw(params: List[torch.Tensor], grads: List[torch.Tensor], exp_avgs: List[torch.Tensor],
-              exp_avg_sqs: List[torch.Tensor], max_exp_avg_sqs: List[torch.Tensor], state_steps: List[int], *,
+              exp_avg_sqs: List[torch.Tensor], max_exp_avg_sqs: List[torch.Tensor], state_steps: List[torch.Tensor], *,
               amsgrad: bool, beta1: float, beta2: float, lr: float, initial_lr: float, weight_decay: float,
               eps: float) -> None:
         r"""Functional API that performs AdamW algorithm computation with decoupled weight decay.
 
         Args:
             params (list): List of parameters to update.
             grads (list): List of parameter gradients.
@@ -245,15 +245,15 @@
             weight_decay (float): Factor for decoupled weight decay
             eps (float): Term added to the denominator to improve numerical stability.
         """
         for i, param in enumerate(params):
             grad = grads[i]
             exp_avg = exp_avgs[i]
             exp_avg_sq = exp_avg_sqs[i]
-            step = state_steps[i]
+            step = state_steps[i].item()
 
             # Perform stepweight decay
             if weight_decay != 0:
                 decay_factor = (lr / initial_lr) if initial_lr else 1.0
                 param.mul_(1 - decay_factor * weight_decay)
 
             bias_correction1 = 1 - beta1**step
@@ -311,15 +311,15 @@
                     raise RuntimeError('AdamW does not support sparse gradients')
                 grads.append(p.grad)
 
                 state = self.state[p]
 
                 # State initialization
                 if 'step' not in state:
-                    state['step'] = 0
+                    state['step'] = torch.zeros((), dtype=torch.float, device=p.device)
                     # Exponential moving average of gradient values
                     state['exp_avg'] = torch.zeros_like(p, memory_format=torch.preserve_format)
                     # Exponential moving average of squared gradient values
                     state['exp_avg_sq'] = torch.zeros_like(p, memory_format=torch.preserve_format)
                     if amsgrad:
                         # Maintains max of all exp. moving avg. of sq. grad. values
                         state['max_exp_avg_sq'] = torch.zeros_like(p, memory_format=torch.preserve_format)
@@ -412,15 +412,15 @@
         eps = self.param_groups[0]['eps']
         weight_decay = self.param_groups[0]['weight_decay']
         initial_lr = self.param_groups[0]['initial_lr']
 
         beta1, beta2 = self.param_groups[0]['betas']
         if param in self.state:
             param_optim_state = self.state[param]
-            step = param_optim_state['step']
+            step = param_optim_state['step'].item()
             bias_correction1 = 1 - beta1**step
             bias_correction2 = 1 - beta2**step
             denom = (param_optim_state['exp_avg_sq'].sqrt() / math.sqrt(bias_correction2)).add_(eps)
             step_size = lr / bias_correction1
             step_tensor = step_size * param_optim_state['exp_avg'].div(denom)
             decay_factor = (lr / initial_lr) if initial_lr else 1.0
             step_tensor.add_(param, alpha=-weight_decay * decay_factor)
```

### Comparing `composer-0.14.1/composer/optim/scheduler.py` & `composer-0.15.0/composer/optim/scheduler.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/profiler/__init__.py` & `composer-0.15.0/composer/profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/profiler/json_trace_handler.py` & `composer-0.15.0/composer/profiler/json_trace_handler.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/profiler/json_trace_merger.py` & `composer-0.15.0/composer/profiler/json_trace_merger.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/profiler/marker.py` & `composer-0.15.0/composer/profiler/marker.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/profiler/profiler.py` & `composer-0.15.0/composer/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/profiler/profiler_action.py` & `composer-0.15.0/composer/profiler/profiler_action.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/profiler/profiler_schedule.py` & `composer-0.15.0/composer/profiler/profiler_schedule.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/profiler/system_profiler.py` & `composer-0.15.0/composer/profiler/system_profiler.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/profiler/torch_profiler.py` & `composer-0.15.0/composer/profiler/torch_profiler.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/profiler/trace_handler.py` & `composer-0.15.0/composer/profiler/trace_handler.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/trainer/_deepspeed.py` & `composer-0.15.0/composer/trainer/_deepspeed.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/trainer/_scale_schedule.py` & `composer-0.15.0/composer/trainer/_scale_schedule.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/trainer/_scaler.py` & `composer-0.15.0/composer/trainer/_scaler.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/trainer/dist_strategy.py` & `composer-0.15.0/composer/trainer/dist_strategy.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 """Helpers for running distributed data parallel training."""
 
 import collections
 import logging
 import warnings
 from contextlib import contextmanager, nullcontext
-from typing import Any, Callable, ContextManager, Dict, Optional, Sequence, Union, cast
+from typing import Any, Callable, ContextManager, Dict, Iterator, List, Optional, Sequence, Tuple, Union, cast
 
 import torch
 from packaging import version
 from torch.nn.parallel import DistributedDataParallel
 from torchmetrics import Metric, MetricCollection
 
 from composer.core import Precision, State
@@ -119,14 +119,81 @@
         raise RuntimeError('Please call dist.initialize_dist() before calling ddp.prepare_module()')
 
     raise RuntimeError('When the world size is > 1, ``torch.distributed`` must be used. However, it is '
                        'not available in your installation of PyTorch. Please install or build PyTorch '
                        'with distributed support.')
 
 
+def set_fsdp_default(fsdp_config: Dict[str, Any]):
+    """Modify fsdp_config to set default values for missing keys."""
+    fsdp_config.setdefault('activation_checkpointing', False)
+    fsdp_config.setdefault('activation_checkpointing_reentrant', True)
+    fsdp_config.setdefault('activation_cpu_offload', False)
+    fsdp_config.setdefault('backward_prefetch', 'BACKWARD_POST')
+    fsdp_config.setdefault('cpu_offload', False)
+    fsdp_config.setdefault('flatten_parameters', True)
+    fsdp_config.setdefault('forward_prefetch', False)
+    fsdp_config.setdefault('ignored_modules', None)
+    fsdp_config.setdefault('keep_low_precision_grads', False)
+    fsdp_config.setdefault('limit_all_gathers', False)
+    fsdp_config.setdefault('load_monolith_rank0_only', False)
+    fsdp_config.setdefault('mixed_precision', 'DEFAULT')
+    fsdp_config.setdefault('sharded_ckpt_prefix_dir', 'ep{epoch}-ba{batch}')
+    fsdp_config.setdefault('sharding_strategy', 'FULL_SHARD')
+    fsdp_config.setdefault('state_dict_type', 'full')
+    fsdp_config.setdefault('sync_module_states', False)
+    fsdp_config.setdefault('use_orig_params', True)
+    fsdp_config.setdefault('verbose', False)
+    return fsdp_config
+
+
+def _recreate_fsdp_param_groups_from_unwrapped_opt_info(
+        fsdp_wrapped_named_params: Iterator[Tuple[str,
+                                                  torch.nn.Parameter]], non_wrapped_param_names_to_group_num: Dict[str,
+                                                                                                                   int],
+        group_num_to_optimizer_info: Dict[int, Dict[str, Any]]) -> List[Dict[str, Any]]:
+    """Helper function to recreate optimizer groups for FSDP wrapped modules.
+
+    Optimizer param groups are formatted as:
+    [
+        {'params': [p1, p2], 'lr' : lr1}, # group 0
+        {'params': [p3], 'lr' : lr2} # group 1
+    ]
+    ie. there are multiple parameters per group. Here, we track the group number in order to map
+    multiple parameters to the same group
+
+    Args:
+        fsdp_wrapped_named_params: output of model.named_parameters() of an FSDP wrapped model
+        non_wrapped_param_names_to_group_num: a Dict mapping from the original model param names
+                                            to the param group number
+        group_num_to_optimizer_info: stores info like lr, eps for each group
+
+    Returns a list of param groups, referencing the fsdp parameters
+    """
+    is_torch_2_0 = using_torch_2()
+    if not is_torch_2_0:
+        raise RuntimeError('Helper function is only supported in torch 2.0')
+
+    from torch.distributed.fsdp._common_utils import clean_tensor_name
+
+    # initialize an empty list of parameters for each optimizer group
+    for group_num in group_num_to_optimizer_info.keys():
+        group_num_to_optimizer_info[group_num]['params'] = []
+
+    for fsdp_name, param in fsdp_wrapped_named_params:
+
+        unwrapped_name = clean_tensor_name(fsdp_name)
+        # need to have a 1:1 mapping between a fsdp param name and the non-wrapped vanilla param name
+        retrieved_group_num = non_wrapped_param_names_to_group_num[unwrapped_name]
+        group_num_to_optimizer_info[retrieved_group_num]['params'].append(param)
+
+    # return sorted optimizer info groups
+    return [group_num_to_optimizer_info[num] for num in sorted(group_num_to_optimizer_info.keys())]
+
+
 def prepare_fsdp_module(
     model: torch.nn.Module,
     optimizers: Optional[Union[torch.optim.Optimizer, Sequence[torch.optim.Optimizer]]],
     fsdp_config: Dict[str, Any],
     precision: Precision,
     device: Device,
     auto_microbatching: bool,
@@ -150,14 +217,29 @@
     from torch.distributed.fsdp import FullyShardedDataParallel
     if not is_torch_2_0:
         from torch.distributed.fsdp.flatten_params_wrapper import FlattenParamsWrapper
 
     from composer.trainer.mosaic_fsdp import (MosaicFullyShardedDataParallel, backward_prefetch_map, get_cpu_offload,
                                               get_mixed_precision, sharding_map)
 
+    set_fsdp_default(fsdp_config)
+
+    # Check sync_module_states is True for mixed initialization
+    if fsdp_config['sync_module_states'] == False:
+        rank_on_meta = 1 if next(model.parameters()).device.type == 'meta' else 0
+        all_ranks_meta = device.tensor_to_device(torch.tensor([rank_on_meta], dtype=torch.uint8))
+        dist.all_reduce(all_ranks_meta, reduce_operation='MIN')
+        any_ranks_meta = device.tensor_to_device(torch.tensor([rank_on_meta], dtype=torch.uint8))
+        dist.all_reduce(any_ranks_meta, reduce_operation='MAX')
+        if all_ranks_meta.item() == 0 and any_ranks_meta.item() == 1:
+            raise ValueError('Detected mixed initialization where some ranks have model on cpu or '
+                             'gpu and some ranks are on meta. Either keep all ranks on the same '
+                             "device or set fsdp_config['sync_module_states'] = True. Otherwise, "
+                             'some weights may be randomly initialized when loading a checkpoint.')
+
     # Check if other ranks OOMed after forward/backward pass when using auto microbatching. This
     # may happen when close to memory limit or with uneven memory usage across ranks. Since we
     # need to do this before the model weights are gathered for the next FSDP block, we wrap every
     # FSPD block with a hook that checks if any other rank OOMed.
     def sync_hook(*args):
         # Check if any other rank hit an OOM
         found_cuda_oom_tensor = device.tensor_to_device(torch.tensor([0], dtype=torch.uint8))
@@ -166,32 +248,72 @@
         # Signal current rank is still in batch
         all_ranks_finished_tensor = device.tensor_to_device(torch.tensor([0], dtype=torch.uint8))
         dist.all_reduce(all_ranks_finished_tensor, reduce_operation='MIN')
 
         if found_cuda_oom == 1:
             raise RuntimeError('CUDA out of memory encountered on a different rank')
 
+    kwargs = {}
+    if is_torch_2_0:
+        # Support of new parameter `use_orig_params` in PyTorch 2.0 or higher.
+        # Setting this to `True` has FSDP use `module`'s original parameters via method
+        # `nn.Module.named_parameters` instead of FSDP's internal class `FlatParameter`. However,
+        # setting it to `False` exposes FSDP's internal class `FlatParameter` via method
+        # `nn.Module.named_parameters`.
+        # Setting it to `True` is mandatory when using `torch.compile()`.
+        kwargs['use_orig_params'] = fsdp_config['use_orig_params']
+
+    # necessary variables for optimizers with multiple param groups in FSDP
+    num_param_groups = None
+    param_name_to_group_num = None
+    group_num_to_param_group_info = None
+
+    optimizer_specific_info = None
     if optimizers:
         optimizers_tuple = ensure_tuple(optimizers)
         if len(optimizers_tuple) != 1:
             raise NotImplementedError(f'Only one optimizer is supported; found {len(optimizers_tuple)} optimizers')
 
         # clearing optimizer param groups and state
         # that will be recreated at the end of prepare_fsdp_module
         optim = optimizers_tuple[0]
+
+        num_param_groups = len(optim.param_groups)
+        if num_param_groups > 1:
+            if not (is_torch_2_0 and kwargs['use_orig_params']):
+                raise RuntimeError('Multiple optimizer groups with FSDP are only supported on torch 2.0 \
+                                   with use_orig_params=True.')
+            # optimizer.param_groups do not contain parameter names which are needed
+            # to keep track of the different parameters in each group
+            # so we use the pointers between model.parameters() and model.named_parameters()
+            # to get the names of the parameters within optimizer.param_groups
+            param_pointer_to_param_name = {id(p): n for n, p in model.named_parameters()}
+            param_name_to_group_num = {}
+            group_num_to_param_group_info = {}
+            for group_num, group in enumerate(optim.param_groups):
+                for param in group['params']:
+                    param_name_to_group_num[param_pointer_to_param_name[id(param)]] = group_num
+
+                # this includes optimizer-specific values like lr, eps
+                # this will be used as the kwargs for the optim param groups later
+                optimizer_specific_group_info = {k: v for k, v in group.items() if k != 'params'}
+                group_num_to_param_group_info[group_num] = optimizer_specific_group_info
+        else:
+            optimizer_specific_info = {k: v for k, v in optim.param_groups[0].items() if k != 'params'}
+
         optim.param_groups.clear()
         optim.state.clear()
 
-    sharding_map_key = fsdp_config.get('sharding_strategy', 'FULL_SHARD').upper()
+    sharding_map_key = fsdp_config['sharding_strategy'].upper()
     sharding_strategy = sharding_map[sharding_map_key]
 
-    cpu_offload = get_cpu_offload(cpu_offload=fsdp_config.get('cpu_offload', False))
+    cpu_offload = get_cpu_offload(cpu_offload=fsdp_config['cpu_offload'])
 
-    mixed_precision = fsdp_config.get('mixed_precision', 'DEFAULT')
-    keep_low_precision_grads = fsdp_config.get('keep_low_precision_grads', False)
+    mixed_precision = fsdp_config['mixed_precision']
+    keep_low_precision_grads = fsdp_config['keep_low_precision_grads']
     mixed_precision, param_dtype, _, _ = get_mixed_precision(precision,
                                                              mixed_precision=mixed_precision,
                                                              keep_low_precision_grads=keep_low_precision_grads)
 
     # Note: FSDP does support the use of torch.float32 with sharding.
     # They just never expected a user to pass in torch.float32 into mixed_precision as a param_dtype.
     # See: https://github.com/pytorch/pytorch/issues/90584
@@ -209,36 +331,27 @@
         if param_dtype == torch.float32:
             raise ValueError(
                 f'FSDP in PyTorch 1.13 does not support param_dtype `{param_dtype}` with sharding_strategy `{sharding_map_key}` '
                 f'Consider using `amp` or `bf16` for precision or setting param_dtype in mixed_precision to `None` '
                 f'with sharding strategy `{sharding_map_key}.`')
 
     if fsdp_config.get('min_params') is not None:
-        warnings.warn(DeprecationWarning('`min_params` in FSDP config will be depricated in composer version 0.16.0.'))
+        warnings.warn(DeprecationWarning('`min_params` in FSDP config will be deprecated in composer version 0.16.0.'))
 
-    backward_prefetch = backward_prefetch_map[fsdp_config.get('backward_prefetch', 'BACKWARD_POST').upper()]
+    backward_prefetch = backward_prefetch_map[fsdp_config['backward_prefetch'].upper()]
     min_params = int(float(fsdp_config.get('min_params', 1e9)))
-    activation_checkpointing = fsdp_config.get('activation_checkpointing', False)
-    activation_cpu_offload = fsdp_config.get('activation_cpu_offload', False)
-    sync_module_states = fsdp_config.get('sync_module_states', False)
-    forward_prefetch = fsdp_config.get('forward_prefetch', False)
-    limit_all_gathers = fsdp_config.get('limit_all_gathers', False)
-    ignored_modules = fsdp_config.get('ignored_modules', None)
-    state_dict_type = fsdp_config.get('state_dict_type', 'full')
-    activation_checkpointing_reentrant = fsdp_config.get('activation_checkpointing_reentrant', True)
-
-    kwargs = {}
-    if is_torch_2_0:
-        # Support of new parameter `use_orig_params` in PyTorch 2.0 or higher.
-        # Setting this to `True` has FSDP use `module`'s original parameters via method
-        # `nn.Module.named_parameters` instead of FSDP's internal class `FlatParameter`. However,
-        # setting it to `False` exposes FSDP's internal class `FlatParameter` via method
-        # `nn.Module.named_parameters`.
-        # Setting it to `True` is mandatory when using `torch.compile()`.
-        kwargs['use_orig_params'] = fsdp_config.get('use_orig_params', True)
+    activation_checkpointing = fsdp_config['activation_checkpointing']
+    activation_cpu_offload = fsdp_config['activation_cpu_offload']
+    sync_module_states = fsdp_config['sync_module_states']
+    forward_prefetch = fsdp_config['forward_prefetch']
+    limit_all_gathers = fsdp_config['limit_all_gathers']
+    ignored_modules = fsdp_config['ignored_modules']
+    state_dict_type = fsdp_config['state_dict_type']
+    activation_checkpointing_reentrant = fsdp_config['activation_checkpointing_reentrant']
+    sharded_ckpt_prefix_dir = fsdp_config['sharded_ckpt_prefix_dir']
 
     # We choose to not wrap the ComposerModel directly, but instead wrap any submodules like `ComposerModel.model`
     # This makes it safer to call ComposerModel-specific functions like 'eval_forward' that
     # may make calls to sharded submodules. If we only wrap the submodules, then any call that ComposerModel makes
     # to a FSDP-wrapped submodule's `forward()` function will be safe and all-gather the necessary weights before `forward()`.
     for obj_name, obj in model.named_children():
         if not isinstance(obj, (Metric, MetricCollection)):
@@ -406,28 +519,43 @@
                     checkpoint_wrapper_fn=second_wrap_fn,  # type: ignore
                     check_fn=_check_fn,  # type: ignore
                 )
 
             setattr(model, obj_name, fsdp_obj)
 
     # Print FSDP wrapped model and FSDP config if `verbose=True`
-    if fsdp_config.get('verbose', False):
+    if fsdp_config['verbose']:
         print(f'FSDP: Wrapped Model:')
         print(model)
         print(f'FSDP: Using sharding_strategy={sharding_strategy}')
         print(f'FSDP: Using cpu_offload={cpu_offload}')
         print(f'FSDP: Using mixed_precision={mixed_precision}')
         print(f'FSDP: Using backward_prefetch={backward_prefetch}')
         print(f'FSDP: Using min_params={min_params}')
         print(f'FSDP: Using activation_checkpointing={activation_checkpointing}')
         print(f'FSDP: Using activation_cpu_offload={activation_cpu_offload}')
         print(f'FSDP: Using sync_module_states={sync_module_states}')
         print(f'FSDP: Using forward_prefetch={forward_prefetch}')
         print(f'FSDP: Using limit_all_gathers={limit_all_gathers}')
         print(f'FSDP: Using state_dict_type={state_dict_type}')
+        print(f'FSDP: Using sharded_ckpt_prefix_dir={sharded_ckpt_prefix_dir}')
 
     # Rebuild optimizer now that parameters are sharded
     if optimizers:
         optimizers_tuple = ensure_tuple(optimizers)
         optim = optimizers_tuple[0]
         optim.param_groups.clear()
-        optim.add_param_group({'params': list(model.parameters())})
+
+        assert num_param_groups is not None
+        if num_param_groups > 1:
+            assert param_name_to_group_num is not None
+            assert group_num_to_param_group_info is not None
+
+            param_groups = _recreate_fsdp_param_groups_from_unwrapped_opt_info(model.named_parameters(),
+                                                                               param_name_to_group_num,
+                                                                               group_num_to_param_group_info)
+            for param_group in param_groups:
+                optim.add_param_group(param_group)
+        else:
+            assert optimizer_specific_info is not None
+            optimizer_specific_info.update({'params': list(model.parameters())})
+            optim.add_param_group(optimizer_specific_info)
```

### Comparing `composer-0.14.1/composer/trainer/meta_safe_apply.py` & `composer-0.15.0/composer/trainer/meta_safe_apply.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/trainer/mosaic_fsdp.py` & `composer-0.15.0/composer/trainer/mosaic_fsdp.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/trainer/trainer.py` & `composer-0.15.0/composer/trainer/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import contextlib
 import datetime
 import itertools
 import logging
 import os
 import random
 import re
+import textwrap
 import time
 import warnings
 from collections import defaultdict
 from copy import deepcopy
 from pathlib import Path
 from typing import Any, Callable, ContextManager, Dict, Iterable, List, Optional, Sequence, TextIO, Tuple, Union, cast
 
@@ -41,15 +42,16 @@
                               WandBLogger)
 from composer.models import ComposerModel
 from composer.optim import ComposerScheduler, DecoupledSGDW, compile_composer_scheduler
 from composer.profiler import Profiler
 from composer.trainer._deepspeed import _fix_batch_precision_for_deepspeed, _parse_deepspeed_config
 from composer.trainer._scale_schedule import scale_pytorch_scheduler
 from composer.trainer._scaler import ClosureGradScaler
-from composer.trainer.dist_strategy import DDPSyncStrategy, ddp_sync_context, prepare_ddp_module, prepare_fsdp_module
+from composer.trainer.dist_strategy import (DDPSyncStrategy, ddp_sync_context, prepare_ddp_module, prepare_fsdp_module,
+                                            set_fsdp_default)
 from composer.utils import (ExportFormat, MissingConditionalImportError, ObjectStore, Transform, checkpoint, dist,
                             ensure_tuple, export_with_logger, extract_hparams, format_name_with_dist, get_device,
                             get_file, is_tpu_installed, map_collection, maybe_create_object_store_from_uri,
                             maybe_create_remote_uploader_downloader_from_uri, model_eval_mode, parse_uri,
                             reproducibility, using_torch_2)
 from composer.utils.misc import is_model_deepspeed
 
@@ -415,14 +417,24 @@
             on this many batches. This parameter has no effect if it is greater than ``len(train_dataloader)``.
             If ``-1``, then the entire dataloader will be iterated over. (default: ``-1``)
 
             When using the profiler, it can be helpful to set this parameter to the length of the profile schedule.
             This setting will end each epoch early to avoid additional training that will not be profiled.
 
             This parameter is ignored if ``train_dataloader`` is not specified.
+        spin_dataloaders (bool, optional): If ``True``, dataloaders will be spun up to the current timestamp
+            by skipping samples which have already been trained on. If a dataloader has a way to resume from
+            the current batch without spinning, this will be a no-op. This ensures dataloaders continue from
+            the same batch when resuming training. (default: ``True``)
+
+            .. note:: Spinning dataloaders can be potentially very slow but is required to skip samples which
+                have already been trained on. If it is acceptable to repeat samples when resuming training,
+                it is possible to resume faster by setting ``spin_dataloaders=False``. This may have severe
+                performance implications and is generally not recommended unless you confidently understand the
+                implications.
         max_duration (Time | str | int, optional): The maximum duration to train. Can be an integer, which will be
             interpreted to be epochs, a str (e.g. ``1ep``, or ``10ba``), or a :class:`.Time` object.
 
             If ``max_duration`` is not specified when constructing the trainer, ``duration`` must be specified when invoking
             :meth:`.Trainer.fit`.
         algorithms (Algorithm | Sequence[Algorithm], optional): The algorithms to use during training. If ``None``, then
             no algorithms will be used. (default: ``None``)
@@ -465,20 +477,21 @@
                 would finish the entire cosine curve, ending with a learning rate near zero.
         step_schedulers_every_batch (bool, optional): By default, native
             `PyTorch schedulers <https://pytorch.org/docs/stable/optim.html#how-to-adjust-learning-rate>`_
             are updated every epoch, while :doc:`Composer Schedulers</trainer/schedulers>` are updated every step.
             Setting this to ``True`` will force schedulers to be stepped every batch,
             while ``False`` means schedulers stepped every epoch. ``None`` indicates the default behavior.
             (default: ``None``)
-        eval_dataloader (DataLoader | DataSpec | Evaluator | Sequence[Evaluator], optional): The :class:`.DataLoader`,
-            :class:`.DataSpec`, :class:`.Evaluator`, or sequence of evaluators for the evaluation data.
+        eval_dataloader (Iterable | DataLoader | DataSpec | Evaluator | Sequence[Evaluator], optional): The :class:`.Iterable`,
+            :class:`.DataLoader`, :class:`.DataSpec`, :class:`.Evaluator`, or sequence of evaluators for the evaluation data.
 
             To evaluate one or more specific metrics across one or more datasets, pass in an
-            :class:`.Evaluator`. If a :class:`.DataSpec` or :class:`.DataLoader` is passed in, then all
-            metrics returned by ``model.get_metrics()`` will be used during evaluation.
+            :class:`.Evaluator`. If a :class:`.DataLoader`, :class:`.DataSpec`, or :class:`.Iterable` is passed in, then all
+            metrics returned by ``model.get_metrics()`` will be used during evaluation. If a :class:`.Evaluator`
+            is specified in a list, all eval dataloaders must be :class:`.Evaluator` instances.
             ``None`` results in no evaluation. (default: ``None``)
         eval_interval (int | str | Time | (State, Event) -> bool, optional): Specifies how frequently to run evaluation.
             An integer, which will be interpreted to be epochs, a str (e.g. ``1ep``, or ``10ba``), a :class:`.Time`
             object, or a callable.
             Defaults to ``1`` (evaluate every epoch).
 
             If an integer (in epochs), :class:`.Time` string, or :class:`.Time` instance, the evaluator will be run
@@ -605,15 +618,15 @@
                     eval_interval="1ep",
                     load_path=checkpoint_path,
                     load_object_store=store,
                 )
         load_weights_only (bool, optional): Whether or not to only restore the weights from the checkpoint without
             restoring the associated state. Ignored if ``load_path`` is ``None``. (default: ``False``)
         load_strict_model_weights (bool, optional): Ensure that the set of weights in the checkpoint and model must exactly match.
-            Ignored if ``load_path`` is ``None``. (default: ``False``)
+            Ignored if ``load_path`` is ``None``. (default: ``True``)
         load_progress_bar (bool, optional): Display the progress bar for downloading the checkpoint.
             Ignored if ``load_path`` is either ``None`` or a local file path. (default: ``True``)
         load_ignore_keys (List[str] | (Dict) -> None, optional): A list of paths for the ``state_dict`` of the checkpoint,
             which, when provided, will be ignored from the state_dict before a checkpoint is loaded. Each path is a list
             of strings specifying the keys to index into ``state_dict`` joined together with `/` as a separator (as PyTorch
             uses `.` in parameter names). If a prefix is provided, all children are also ignored (see Example 2).
             See :mod:`composer.core.state` for the structure of state_dict.
@@ -640,14 +653,17 @@
             weights loaded.
 
             Example 1: ``load_exclude_algorithms = ["BlurPool"]`` would exclude BlurPool from loading.
 
             Example 2: ``load_exclude_algorithms = ["FusedLayerNorm", "Alibi"]`` would exclude FusedLayerNorm and Alibi from loading.
 
             (default: ``None``)
+        load_fsdp_monolith_rank0_only (bool, optional): If ``True``, when loading a monolith (non-sharded) checkpoint
+            with FSDP, only rank 0 will load the checkpoint and broadcast weights/optimizers to other ranks.
+            This will dramatically reduce the memory usage on system. (default: ``False``)
 
         save_folder (str, optional): Format string for the folder where checkpoints are saved.
             If ``None``, checkpoints will not be saved. Can also be a URI for S3 paths only.
             In the case of an S3 URI, the appropriate `~.RemoteUploader` object will be created
             automatically. (default: ``None``)
 
             .. seealso:: :class:`~.CheckpointSaver`
@@ -787,14 +803,15 @@
         # The Model
         model: ComposerModel,
 
         # Train Dataloader
         train_dataloader: Optional[Union[Iterable, DataSpec, Dict[str, Any]]] = None,
         train_dataloader_label: str = 'train',
         train_subset_num_batches: int = -1,
+        spin_dataloaders: bool = True,
 
         # Stopping Condition
         max_duration: Optional[Union[int, str, Time]] = None,
 
         # Algorithms
         algorithms: Optional[Union[Algorithm, Sequence[Algorithm]]] = None,
 
@@ -825,15 +842,15 @@
         log_traces: bool = False,
         auto_log_hparams: bool = False,
 
         # Load Checkpoint
         load_path: Optional[str] = None,
         load_object_store: Optional[Union[ObjectStore, LoggerDestination]] = None,
         load_weights_only: bool = False,
-        load_strict_model_weights: bool = False,
+        load_strict_model_weights: bool = True,
         load_progress_bar: bool = True,
         load_ignore_keys: Optional[Union[List[str], Callable[[Dict], None]]] = None,
         load_exclude_algorithms: Optional[List[str]] = None,
 
         # Save Checkpoint
         save_folder: Optional[str] = None,
         save_filename: str = 'ep{epoch}-ba{batch}-rank{rank}.pt',
@@ -845,15 +862,15 @@
 
         # Graceful Resumption
         autoresume: bool = False,
 
         # DeepSpeed
         deepspeed_config: Optional[Dict[str, Any]] = None,
         fsdp_config: Optional[Dict[str, Any]] = None,
-        fsdp_auto_wrap: Optional[bool] = True,
+        fsdp_auto_wrap: bool = True,
 
         # System/Numerics
         device: Optional[Union[str, Device]] = None,
         precision: Optional[Union[str, Precision]] = None,
         device_train_microbatch_size: Optional[Union[int, str]] = None,
 
         # Reproducibility
@@ -933,30 +950,20 @@
         # will be determined when dataloader is specified. train_dataloader is parsed after `Event.INIT` or in
         # fit()
         device_train_microbatch_size = _get_initial_device_train_microbatch_size(device_train_microbatch_size,
                                                                                  auto_microbatching, None)
 
         assert not isinstance(device_train_microbatch_size, str)
 
-        # Determine whether DeepSpeed and FSDP are enabled
-        self.deepspeed_config = deepspeed_config
-        self.fsdp_config = fsdp_config
-        self.deepspeed_enabled = self.deepspeed_config is not None
-        self.fsdp_enabled = self.fsdp_config is not None
-
         # Distributed
-        if self.deepspeed_enabled or self.fsdp_enabled or dist.get_world_size() > 1:
+        if deepspeed_config is not None or fsdp_config is not None or dist.get_world_size() > 1:
             # Deepspeed and FSDP both require torch.distributed to be initialized, even if the world size is 1
             # And torch.distributed is always required for multi-rank training
             dist.initialize_dist(device, dist_timeout)
 
-        # Handle FSDP wrapping
-        if self.fsdp_config is not None and fsdp_auto_wrap:
-            prepare_fsdp_module(model, optimizers, self.fsdp_config, precision, device, auto_microbatching)
-
         # Reproducibility
         rank_zero_seed, seed = _distribute_and_get_random_seed(seed, device)
         # If hparams is used to create the Trainer this function is called twice
         # which is okay because all runs with the hparams codepath will do this
         reproducibility.seed_all(seed)
         if deterministic_mode:
             reproducibility.configure_deterministic_mode()
@@ -969,15 +976,15 @@
                            f"{type(optimizers).__name__}(lr={optimizers.defaults['lr']})"))
 
         num_optimizers = len(ensure_tuple(optimizers))
         if num_optimizers != 1:
             raise NotImplementedError(f'Only one optimizer is supported; found {num_optimizers} optimizers')
 
         # Move the model and optimizers to the device
-        if not (self.deepspeed_enabled or self.fsdp_enabled):
+        if deepspeed_config is None and fsdp_config is None:
             # check if model is already on tpu
             if isinstance(device, DeviceTPU) and 'xla' not in str(next(model.parameters()).device):
                 raise ValueError(
                     'Use model.to(xm.xla_device()) to set the model to the TPU before providing to the trainer.')
             else:
                 model = device.module_to_device(model)
                 # Move any remaining optimizer parameters onto the device
@@ -1001,15 +1008,16 @@
             callbacks=callbacks,
             device_train_microbatch_size=device_train_microbatch_size,
             auto_microbatching=auto_microbatching,
             precision=precision,
             optimizers=optimizers,
             run_name=run_name,
             deepspeed_config=deepspeed_config,
-            fsdp_config=fsdp_config,
+            fsdp_config=set_fsdp_default(fsdp_config) if fsdp_config is not None else None,
+            fsdp_auto_wrap=fsdp_auto_wrap,
         )
 
         # Profiler
         if profiler is not None:
             warnings.warn('The profiler is enabled. Using the profiler adds additional overhead when training.')
             self.state.profiler = profiler
             self.state.profiler.bind_to_state(self.state)
@@ -1140,18 +1148,24 @@
         self.state.train_metrics = deepcopy(self.state.model.get_metrics(is_train=True))
         self.state.eval_metrics = {}
         if eval_dataloader is None:
             evaluators: List[Evaluator] = []
         else:
             eval_metrics = deepcopy(self.state.model.get_metrics(is_train=False))
             model_metric_names = [str(k) for k in eval_metrics.keys()]
+            eval_dataloader = ensure_tuple(eval_dataloader)
+
+            evaluator_types = [isinstance(evaluator, Evaluator) for evaluator in eval_dataloader]
+            if any(evaluator_types) and not all(evaluator_types):
+                raise ValueError('Mixing Evaluator with other classes is not allowed, please wrap'
+                                 'all other classes with the Evaluator class. These are the classes'
+                                 'that were detected:' + str([type(evaluator) for evaluator in eval_dataloader]))
 
             evaluators = [
-                ensure_evaluator(evaluator, default_metric_names=model_metric_names)
-                for evaluator in ensure_tuple(eval_dataloader)
+                ensure_evaluator(evaluator, default_metric_names=model_metric_names) for evaluator in eval_dataloader
             ]
             # match metric names to model metrics
             self.state.eval_metrics = {
                 evaluator.label: _filter_metrics(eval_metrics, evaluator.metric_names) for evaluator in evaluators
             }
 
             _set_evaluator_interval_and_subset_num_batches(
@@ -1183,14 +1197,15 @@
                                       train_subset_num_batches)
             if isinstance(self.state.device, DeviceTPU):
                 self.state.train_dataloader = pl.MpDeviceLoader(self.state.dataloader, xm.xla_device())
             else:
                 self.state.train_dataloader = self.state.dataloader
             self.state.device_train_microbatch_size = _get_initial_device_train_microbatch_size(
                 self.state.device_train_microbatch_size, self.state.auto_microbatching, self.state.train_dataloader)
+        self.spin_dataloaders = spin_dataloaders
 
         # Max Duration
         if max_duration is not None:
             self.state.max_duration = ensure_time(max_duration, TimeUnit.EPOCH)
 
         self.logger.log_hyperparameters({'rank_zero_seed': rank_zero_seed})
 
@@ -1207,18 +1222,46 @@
             self._scheduler_step_frequency = TimeUnit.BATCH if step_schedulers_every_batch else TimeUnit.EPOCH
 
         # Some algorithms require specific settings
         self._backwards_create_graph = any(map(lambda x: x.backwards_create_graph, self.state.algorithms))
         self._find_unused_parameters = any(map(lambda x: x.find_unused_parameters, self.state.algorithms))
         self._ddp_sync_strategy = _get_ddp_sync_strategy(ddp_sync_strategy, self._find_unused_parameters)
 
-        # If using DDP or DeepSpeed, we need to wrap the ComposerModel
-        # But store a reference to the original model for functions like `eval_forward`, `get_metrics`, etc.
+        # Suppressing GradScaler warnings as they are always created
+        # self._use_grad_scaling() will raise a RuntimeError if grad scaling is not available when it is required
+        warnings.filterwarnings(action='ignore', message='torch.cuda.amp.GradScaler')
+        self.state.scaler = ClosureGradScaler() if self._use_closures() else GradScaler()
+
+        if self.state.fsdp_config is not None:
+            if version.parse(torch.__version__) < version.parse('1.13.0'):
+                raise RuntimeError('To use FSDP with Composer, you must use torch>=1.13.0.')
+            from torch.distributed.fsdp.sharded_grad_scaler import ShardedGradScaler
+
+            # This state should never be reached, but we raise a ValueError just in case
+            if self._use_closures() and self.state.precision == Precision.AMP_FP16:
+                raise ValueError(f'Using closures and precision {self.state.precision} is not supported'
+                                 f' with FSDP. Please use another optimizer or precision type.')
+            self.state.scaler = ShardedGradScaler()
+
+        # suppressing FSDP warning when auto grad accum exits the forward pass before completing
+        warnings.filterwarnings(action='ignore', message='Forward order differs from that of the first iteration')
+
+        # If using DDP or DeepSpeed, we need to wrap the ComposerModel but store a reference to the
+        # original model for functions like `eval_forward`, `get_metrics`, etc.
         self._original_model = self.state.model
 
+        # If using PyTorch DDP, the model must be loaded before it is wrapped with DDP.
+        # If using DeepSpeed, the engine must be initialized before the model is loaded.
+        # If using FSDP, the model must be wrapped and then loaded unless loading a monolith
+        # checkpoint on rank 0 only, in which case the model be loaded before it is wrapped.
+
+        # FSDP wrap if not using monolith checkpoint on rank 0 only
+        if self.state.fsdp_config is not None and fsdp_auto_wrap and not self.state.load_fsdp_monolith_rank0_only:
+            prepare_fsdp_module(model, optimizers, self.state.fsdp_config, precision, device, auto_microbatching)
+
         # Configure Deepspeed
         if self.state.deepspeed_config is not None:
             for callback in self.state.callbacks:
                 if isinstance(callback, OptimizerMonitor):
                     raise ValueError('OptimizerMonitor is not supported with DeepSpeed because DeepSpeed clears '
                                      'the gradients before in the last call to .backward see: '
                                      'https://github.com/microsoft/DeepSpeed/issues/2329 for more details.')
@@ -1246,55 +1289,34 @@
             # so these attributes should not be serialized with the composer state.
             if 'model' in self.state.serialized_attributes:
                 self.state.serialized_attributes.remove('model')
 
             if 'optimizers' in self.state.serialized_attributes:
                 self.state.serialized_attributes.remove('optimizers')
 
-        # If using DeepSpeed, the model must be loaded from checkpoint after the engine has been
-        # initialized, but if using PyTorch DDP, the model must be loaded before it is wrapped with
-        # DDP.
-
-        # suppressing GradScaler warnings as they are always created
-        # self._use_grad_scaling() will raise a RuntimeError if grad scaling is not available when it is required
-        warnings.filterwarnings(action='ignore', message='torch.cuda.amp.GradScaler')
-        self.state.scaler = ClosureGradScaler() if self._use_closures() else GradScaler()
-
-        if self.fsdp_config is not None:
-            if version.parse(torch.__version__) < version.parse('1.13.0'):
-                raise RuntimeError('To use FSDP with Composer, you must use torch>=1.13.0.')
-            from torch.distributed.fsdp.sharded_grad_scaler import ShardedGradScaler
-
-            # This state should never be reached, but we raise a ValueError just in case
-            if self._use_closures() and self.state.precision == Precision.AMP_FP16:
-                raise ValueError(f'Using closures and precision {self.state.precision} is not supported'
-                                 f' with FSDP. Please use another optimizer or precision type.')
-            self.state.scaler = ShardedGradScaler()
-
-        # suppressing FSDP warning when auto grad accum exits the forward pass before completing
-        warnings.filterwarnings(action='ignore', message='Forward order differs from that of the first iteration')
-
         # Load Checkpoint
         self._rng_state = None
         # If autoresume is enabled, first check for existing checkpoints to load
         if autoresume:
             log.info('Searching for a previous checkpoint to autoresume')
+            error_message = ''
             if save_folder is None:
-                raise ValueError('The `save_folder` must be specified when autoresume is enabled.')
+                error_message += 'The `save_folder` must be specified when autoresume is enabled. '
             if save_overwrite:
-                raise ValueError(
+                error_message += textwrap.dedent(
                     'The flag `save_overwrite` must be False when autoresume is enabled as autoresume always loads the '
-                    'latest existing checkpoint in `save_folder`.')
+                    'latest existing checkpoint in `save_folder`. ')
             if save_latest_filename is None:
-                raise ValueError(
-                    'The `save_latest_filename` must be specified so autoresume knows where to load checkpoints from.')
+                error_message += 'The `save_latest_filename` must be specified so autoresume knows where to load checkpoints from. '
             if run_name is None:
-                raise ValueError(
-                    'The `run_name` must be specified when using autoresume so Event.INIT is run with the correct run name.'
-                )
+                error_message += 'The `run_name` must be specified when using autoresume so Event.INIT is run with the correct run name. '
+            if error_message != '':
+                raise ValueError(error_message)
+            assert save_folder is not None
+            assert save_latest_filename is not None
 
             remote_ud_has_multiple_concurrent_uploads = [
                 isinstance(logger_destination, RemoteUploaderDownloader) and
                 logger_destination._num_concurrent_uploads != 1 for logger_destination in self.logger.destinations
             ]
             if any(remote_ud_has_multiple_concurrent_uploads):
                 raise ValueError(
@@ -1337,28 +1359,33 @@
                 progress_bar=load_progress_bar,
                 ignore_keys=load_ignore_keys,
                 exclude_algorithms=load_exclude_algorithms,
                 algorithm_passes=self.engine.algorithm_passes,
             )
             self.state.run_name = run_name
 
+        # FSDP wrap if model is not yet wrapped and FSDP is enabled. This can happen if
+        # load_fsdp_monolith_rank0_only=True but no checkpoint was loaded.
+        if not self.state.fsdp_enabled and self.state.fsdp_config is not None and self.state.fsdp_auto_wrap and self.state.load_fsdp_monolith_rank0_only:
+            prepare_fsdp_module(model, optimizers, self.state.fsdp_config, precision, device, auto_microbatching)
+
         self.engine.run_event(Event.AFTER_LOAD)
 
         # reseed here. This helps with a couple of issues:
         # 1. rng state may change at Event.INIT/Event.AFTER_LOAD. For example, if an algorithm
         # creates a new module and module parameters are initialized randomly, rng state will
         # change. This reseeding nullifies such effects.
         # 2. While resuming from a checkpoint, we want to spin dataloader and bring it back to the
         # same state as at the time of the checkpoint. Therefore, spinning needs to start from the
         # same rng state as in the original run.
         log.info(f'Setting seed to {self.state.seed}')
         reproducibility.seed_all(self.state.seed)
 
-        if not (self.deepspeed_enabled or self.fsdp_enabled) and dist.get_world_size() > 1:
-            # Only wrap the module if required
+        # DDP wrap if required
+        if not self.state.deepspeed_enabled and not self.state.fsdp_enabled and dist.get_world_size() > 1:
             self.state.model = prepare_ddp_module(self.state.model, self._find_unused_parameters)
 
         # The model would need to be torch.compile()'d after being wrapped in a distributed strategy
         # to take advantage of any graph breaks.
         if is_torch_2_0 and not is_model_compiled and compile_config is not None:
             compiled_model = torch.compile(  # pyright: ignore [reportGeneralTypeIssues]
                 self.state.model, **compile_config)
@@ -1431,15 +1458,15 @@
         save_latest_remote_file_name = format_name_with_dist(save_latest_remote_file_name, self.state.run_name)
         latest_checkpoint_path = os.path.join(save_folder, save_latest_filename)
 
         log.info(
             f'Looking for autoresume checkpoint: {save_latest_remote_file_name} (remote), {latest_checkpoint_path} (local)'
         )
 
-        if self.deepspeed_enabled or self.state.fsdp_sharded_state_dict_enabled:
+        if self.state.deepspeed_enabled or self.state.fsdp_sharded_state_dict_enabled:
             # If latest checkpoint is not saved locally, try to fetch from loggers
             if not os.path.exists(latest_checkpoint_path):
                 log.debug(f'Attempting to download the checkpoint on to rank {dist.get_global_rank()}')
                 os.makedirs(save_folder, exist_ok=True)
                 self._try_checkpoint_download(latest_checkpoint_path, save_latest_remote_file_name, loggers,
                                               load_progress_bar)
 
@@ -1448,15 +1475,15 @@
 
             if all(latest_checkpoint_exists):  # All paths exist, so return the path.
                 return latest_checkpoint_path
             # Require all ranks to have their own local checkpoint if we wish to restore from it for
             # deepspeed or fsdp + sharding
             elif any(latest_checkpoint_exists):  # Some but not all exist, which is very bad.
                 missing_ranks = [n for (n, exist) in enumerate(latest_checkpoint_exists) if not exist]
-                mode = 'Deepspeed' if self.deepspeed_enabled else 'FSDP sharding'
+                mode = 'Deepspeed' if self.state.deepspeed_enabled else 'FSDP sharding'
                 raise RuntimeError(f'{mode} was enabled, but checkpoints missing on ranks: {missing_ranks}')
             else:  # None of the paths exists, so no autoresume necessary.
                 return None
         else:
             # broadcast the local checkpoint path to all ranks
             latest_checkpoint_path_list = [os.path.abspath(latest_checkpoint_path)]
             dist.broadcast_object_list(latest_checkpoint_path_list, src=0)
@@ -1473,14 +1500,15 @@
                 os.makedirs(save_folder, exist_ok=True)
                 self._try_checkpoint_download(latest_checkpoint_path, save_latest_remote_file_name, loggers,
                                               load_progress_bar)
 
             signal_file_path = os.path.join(os.path.dirname(latest_checkpoint_path),
                                             '.local_rank0_completed_autoresume')
             if dist.get_local_rank() == 0:
+                os.makedirs(os.path.dirname(signal_file_path), exist_ok=True)
                 with open(signal_file_path, 'wb') as f:
                     f.write(b'local_rank0_completed_autoresume')
 
             # Avoid the collective call until the local rank zero has finished trying to download the checkpoint
             # so that we don't timeout for large downloads. This syncs all processes on the node
             with dist.local_rank_zero_download_and_wait(signal_file_path):
                 # Then, wait to ensure every node has finished downloading the checkpoint
@@ -1509,14 +1537,15 @@
     def fit(
         self,
         *,
         # Train Dataloader
         train_dataloader: Optional[Union[Iterable, DataSpec, Dict[str, Any]]] = None,
         train_dataloader_label: str = 'train',
         train_subset_num_batches: Optional[int] = None,
+        spin_dataloaders: Optional[bool] = None,
 
         # Timing
         duration: Optional[Union[int, str, Time[int]]] = None,
         reset_time: bool = False,
 
         # Schedulers
         schedulers: Optional[Union[ComposerScheduler, PyTorchScheduler, Sequence[Union[ComposerScheduler,
@@ -1603,14 +1632,15 @@
             trainer.fit(reset_time=True, duration="3ep")
             assert trainer.state.timestamp.epoch == "3ep"
 
         Args:
             train_dataloader (Iterable | DataSpec | Dict[str, Any], optional): See :class:`.Trainer`.
             train_dataloader_label (str, optional): See :class:`.Trainer`.
             train_subset_num_batches (int, optional): See :class:`.Trainer`.
+            spin_dataloaders (bool, optional): See :class:`.Trainer`.
             reset_time (bool): Whether to reset the :attr:`.State.timestamp` to zero values. Defaults to False.
 
                 If ``True``, the timestamp will be zeroed out, causing :class:`.ComposerScheduler` and
                 :class:`.Algorithm` instances to start from the beginning, as if it is a new training run. The model
                 will be trained for ``duration``, if specified, or for :attr:`.State.max_duration`, which would have
                 been provided when constructing the :class:`.Trainer` or by a previous call to :meth:`.fit`.
 
@@ -1648,14 +1678,16 @@
             self.state.train_dataloader = self.state.dataloader
             self.state.device_train_microbatch_size = _get_initial_device_train_microbatch_size(
                 self.state.device_train_microbatch_size, self.state.auto_microbatching, self.state.train_dataloader)
         if self._train_data_spec is None:
             _raise_missing_argument_exception('train_dataloader')
         if train_subset_num_batches is not None:
             self.state.dataloader_len = train_subset_num_batches
+        if spin_dataloaders is not None:
+            self.spin_dataloaders = spin_dataloaders
 
         # Reset Time
         if reset_time:
             self.state.timestamp = Timestamp()
 
         # Max Duration
         if duration is not None:
@@ -1706,18 +1738,24 @@
 
         # Evaluators
         if eval_dataloader is not None:
             # Need to use the `original_model` rather than `state.model`, as `state.model`
             # could be DDP / DeepSpeed wrapped.
             eval_metrics = self._original_model.get_metrics(is_train=False)
             metric_names = [str(k) for k in eval_metrics.keys()]
+            eval_dataloader = ensure_tuple(eval_dataloader)
+
+            evaluator_types = [isinstance(evaluator, Evaluator) for evaluator in eval_dataloader]
+            if any(evaluator_types) and not all(evaluator_types):
+                raise ValueError('Mixing Evaluator with other classes is not allowed, please wrap'
+                                 'all other classes with the Evaluator class. These are the classes'
+                                 'that were detected:' + str([type(evaluator) for evaluator in eval_dataloader]))
 
             evaluators = [
-                ensure_evaluator(evaluator, default_metric_names=metric_names)
-                for evaluator in ensure_tuple(eval_dataloader)
+                ensure_evaluator(evaluator, default_metric_names=metric_names) for evaluator in eval_dataloader
             ]
 
             # match metric names to model metrics
             self.state.eval_metrics = {
                 evaluator.label: _filter_metrics(eval_metrics, evaluator.metric_names) for evaluator in evaluators
             }
 
@@ -1749,15 +1787,15 @@
                                  'second run with profiler.')
             self.state.device_train_microbatch_size = _get_initial_device_train_microbatch_size(
                 device_train_microbatch_size, self.state.auto_microbatching, self.state.train_dataloader)
 
         # Precision
         if precision is not None:
             if Precision(precision) != self.state.precision:
-                if self.deepspeed_enabled:
+                if self.state.deepspeed_enabled:
                     raise ValueError('Changing the precision when using DeepSpeed is not supported')
                 precision = Precision(precision)
                 _validate_precision(precision, self.state.device)
                 self.state.precision = precision
 
             # update scaler since precision was provided
             self.state.scaler = ClosureGradScaler() if self._use_closures() else GradScaler()
@@ -1814,16 +1852,16 @@
                 self.state.train_metric_values[metric_name] = computed_metrics[metric_name]
             else:
                 if dataloader_label not in self.state.eval_metrics:
                     self.state.eval_metrics[dataloader_label] = {}
                 self.state.eval_metrics[dataloader_label][metric_name] = metric
                 self.state.eval_metric_values[metric_name] = computed_metrics[metric_name]
 
-    def _spin_dataloaders(self):
-        """Spin the dataloaders to restore sampler state.
+    def _spin_dataloaders_to_cur_epoch(self):
+        """Spin the dataloaders to restore sampler state for current epoch.
 
         Only one batch must be loaded to seed the sampler's generator. since only the first batch is being loaded, the
         dataloader may not be completely iterated through.
         """
         log.debug('Spinning the dataloaders')
 
         # spin the evaluator dataloaders once to initialize its sampler deterministically
@@ -1879,15 +1917,16 @@
         assert self._train_data_spec is not None, 'The train data spec is set in __init__() or fit()'
         assert self.state.scaler is not None, 'scaler should have been set in __init__()'
 
         self.engine.run_event(Event.FIT_START)
 
         use_grad_scaling = self._use_grad_scaling(self.state.precision, self.state.scaler)
 
-        self._spin_dataloaders()
+        if self.spin_dataloaders:
+            self._spin_dataloaders_to_cur_epoch()
 
         if self.state.timestamp.batch_in_epoch == 0 and self._rng_state is not None:
             # only restore the rng state here if the step in the current epoch is zero.
             reproducibility.load_rng_state(self._rng_state)
             self._rng_state = None
 
         self.state.model.train()
@@ -1901,29 +1940,29 @@
                     self.logger.log_metrics({'time/epoch': self.state.timestamp.epoch.value})
 
                 dataloader = self.state.dataloader
                 if isinstance(dataloader, DataLoader) and isinstance(dataloader.sampler, DistributedSampler):
                     dataloader.sampler.set_epoch(int(self.state.timestamp.epoch))
 
                 for batch_idx, self.state.batch in enumerate(self._iter_dataloader(TrainerMode.TRAIN)):
-                    # Don't spin if dataloader handles it internally. Otherwise, if resuming, skip dataloader forward
-                    if 'train' not in self.state.dataset_resumption and batch_idx < int(
+                    # Spin dataloader forward unless dataloader handles internally with dataset_resumption
+                    if self.spin_dataloaders and 'train' not in self.state.dataset_resumption and batch_idx < int(
                             self.state.timestamp.batch_in_epoch):
                         # Restore the RNG state immediately before the next batch is yielded from the dataloader
                         if batch_idx + 1 == int(self.state.timestamp.batch_in_epoch) and self._rng_state is not None:
                             reproducibility.load_rng_state(self._rng_state)
                             self._rng_state = None
                         continue
 
                     self.state.batch = self.state.device.batch_to_device(self.state.batch)
                     self.state.batch = self._train_data_spec.device_transforms(self.state.batch)
                     rank_num_samples = self._train_data_spec.get_num_samples_in_batch(self.state.batch)
                     rank_num_tokens = self._train_data_spec.get_num_tokens_in_batch(self.state.batch)
 
-                    if self.deepspeed_enabled:
+                    if self.state.deepspeed_enabled:
                         self.state.batch = _fix_batch_precision_for_deepspeed(self.state.batch, self.state.precision)
 
                     self.engine.run_event(Event.AFTER_DATALOADER)
 
                     self.engine.run_event(Event.BATCH_START)
 
                     # Log time values
@@ -2049,35 +2088,44 @@
 
     def _eval_train_metrics(self, device_batch):
         assert self._train_data_spec is not None, 'The train data spec should be set on __init__ or fit()'
         assert self.state.train_metrics is not None, 'The train metrics should be set on __init__ or fit()'
 
         with torch.no_grad(),\
                 model_eval_mode(self.state.model),\
-                _get_precision_context(self.state.precision, self.deepspeed_enabled):
+                _get_precision_context(self.state.precision, self.state.deepspeed_enabled):
             eval_outputs = self._original_model.eval_forward(device_batch, self.state.outputs)
             for _, metric in self.state.train_metrics.items():
                 self._original_model.update_metric(
                     device_batch,
                     eval_outputs,
                     metric,
                 )
 
     def _run_evaluators(self, event: Event):
         """Runs evaluators periodically during training."""
+        evaluators_executing = []
         for evaluator in self.state.evaluators:
             assert evaluator.eval_interval is not None, 'eval_interval should have been set on __init__() or fit()'
             assert evaluator.subset_num_batches is not None, 'subset_num_batches should have been set on __init__() or fit()'
-            if evaluator.eval_interval(self.state, event):
+            evaluators_executing.append(evaluator.eval_interval(self.state, event))
+        if not any(evaluators_executing):
+            return
+
+        self.engine.run_event(Event.EVAL_BEFORE_ALL)
+        for index, evaluator in enumerate(self.state.evaluators):
+            if evaluators_executing[index]:
                 self._eval_loop(
                     evaluator=evaluator,
                     subset_num_batches=evaluator.subset_num_batches,
                     metrics=self.state.eval_metrics[evaluator.label],
                 )
 
+        self.engine.run_event(Event.EVAL_AFTER_ALL)
+
     def _train_batch(self, use_grad_scaling: bool) -> Dict[str, torch.Tensor]:
         """Compute loss by training on a full batch of data.
 
         Adaptively change microbatch size if enabled to maximize GPU usage.
 
         Args:
             use_grad_scaling (bool): Enables gradient scaling.
@@ -2108,31 +2156,36 @@
                 if self._use_closures():
                     for optimizer in self.state.optimizers:
                         if use_grad_scaling:
                             self.state.scaler.step(optimizer,
                                                    closure=lambda loss_dict=total_loss_dict, **kwargs: self.
                                                    _train_microbatches(microbatches, loss_dict, **kwargs))
                         else:
-                            optimizer.step(closure=lambda **kwargs: self._train_microbatches(
-                                microbatches, total_loss_dict, **kwargs).item())
+                            optimizer.step(closure=lambda loss_dict=total_loss_dict, **kwargs: self._train_microbatches(
+                                microbatches, loss_dict, **kwargs).item())
                 else:
                     self._train_microbatches(microbatches, total_loss_dict)
-                    if not self.deepspeed_enabled:
+                    if not self.state.deepspeed_enabled:
                         for optimizer in self.state.optimizers:
                             if use_grad_scaling:
                                 self.state.scaler.step(optimizer)
                             else:
                                 if isinstance(self.state.device, DeviceTPU):
                                     xm.optimizer_step(optimizer, barrier=True)
                                 else:
                                     optimizer.step()
             except RuntimeError as e:
                 if self.state.auto_microbatching and _is_cuda_oom(e):
                     log.debug((f"Rank {dist.get_global_rank()} OOM'd."))
                     found_cuda_oom = 1
+                elif self.state.auto_microbatching and 'cuda' in str(e).lower() or 'c10' in str(e).lower():
+                    raise RuntimeError(
+                        textwrap.dedent(
+                            'Encountered non-addressable cuda error while using auto microbatching. '
+                            'If this repeatedly occurs, set `device_train_microbatch_size` manually.')) from e
                 else:
                     raise
 
             if self.state.auto_microbatching:
                 all_ranks_finished = False
                 while not all_ranks_finished:
                     # Propagate across all ranks if any rank hit CUDA OOM
@@ -2192,15 +2245,15 @@
             self.engine.run_event(Event.BEFORE_TRAIN_BATCH)
 
             assert self.state.optimizers is not None
             assert self.state.scaler is not None
 
             use_grad_scaling = self._use_grad_scaling(self.state.precision, self.state.scaler)
 
-            if not self.deepspeed_enabled:
+            if not self.state.deepspeed_enabled:
                 for optimizer in self.state.optimizers:
                     try:
                         optimizer.zero_grad(set_to_none=True)
                     except TypeError:
                         optimizer.zero_grad()
 
             # Tracker for gradient accumulation
@@ -2244,15 +2297,15 @@
         assert self.state.scaler is not None
         assert self._train_data_spec is not None
 
         # Cache the device batch, because `self.state.batch` gets overridden in microbatching loop
         device_batch = deepcopy(self.state.batch)
 
         microbatch_num_samples = self._train_data_spec.get_num_samples_in_batch(self.state.batch)
-        if self.deepspeed_enabled or not isinstance(self.state.model, DistributedDataParallel):
+        if self.state.deepspeed_enabled or not isinstance(self.state.model, DistributedDataParallel):
             sync_context = contextlib.nullcontext()
         elif self.state.auto_microbatching and not self.first_batch_complete:
             # PyTorch DDP rebuilds gradient reduction buckets after 1) a forward pass where the
             # no_sync context was not set 2) a backward pass 3) a forward pass. If only a
             # subset of ranks OOM on the first batch, this will cause a deadlock since a rank
             # that did not OOM will complete steps (1), (2), and (3) on the first succesful
             # microbatch after the OOMs but an OOMing rank will have never completed (1) if
@@ -2268,15 +2321,15 @@
                 self._ddp_sync_strategy,
             )
 
         with sync_context:
             # Forward pass
             self.engine.run_event(Event.BEFORE_FORWARD)
 
-            with _get_precision_context(self.state.precision, self.deepspeed_enabled):
+            with _get_precision_context(self.state.precision, self.state.deepspeed_enabled):
                 self.state.outputs = self.state.model(self.state.batch)
 
             self.engine.run_event(Event.AFTER_FORWARD)
 
             # Check if other ranks OOMed after forward pass when using auto microbatching. This may
             # happen when close to memory limit or with uneven memory usage across ranks
             if self.state.auto_microbatching:
@@ -2290,15 +2343,15 @@
 
                 if found_cuda_oom == 1:
                     raise RuntimeError('CUDA out of memory encountered on a different rank')
 
             # Loss
             self.engine.run_event(Event.BEFORE_LOSS)
 
-            with _get_precision_context(self.state.precision, self.deepspeed_enabled):
+            with _get_precision_context(self.state.precision, self.state.deepspeed_enabled):
                 self.state.loss = self._original_model.loss(self.state.outputs, self.state.batch)
 
             assert self.state.loss is not None
             self.engine.run_event(Event.AFTER_LOSS)
 
             # Backward Pass
             self.engine.run_event(Event.BEFORE_BACKWARD)
@@ -2327,30 +2380,30 @@
             # For each loss to log: detach, clone, mean, then multiply by (microbatch size) / (batch size)
             for k, loss in microbatch_loss_dict.items():
                 microbatch_loss_dict[k] = loss.detach().clone().mean() * (microbatch_num_samples / current_batch_size)
 
             if use_grad_scaling:
                 microbatch_loss = cast(torch.Tensor, self.state.scaler.scale(microbatch_loss))
 
-            if self.deepspeed_enabled:
+            if self.state.deepspeed_enabled:
                 self.state.deepspeed_model.backward(microbatch_loss)
 
             else:
                 # Scale loss based on the number of samples in the microbatch to maintain gradient numerics
                 microbatch_loss.mul_(microbatch_num_samples / current_batch_size)
                 microbatch_loss.backward(create_graph=self._backwards_create_graph)
 
             self.engine.run_event(Event.AFTER_BACKWARD)
 
             # Use microbatch outputs to update training metrics
             if self.state.train_metrics is not None:
                 self.state.train_metrics = self._ensure_metrics_device_and_dtype(self.state.train_metrics)
                 self._eval_train_metrics(device_batch)
 
-        if self.deepspeed_enabled:
+        if self.state.deepspeed_enabled:
             self.state.deepspeed_model.step()
 
         return microbatch_loss_dict
 
     def predict(
         self,
         dataloader: Union[DataLoader, DataSpec],
@@ -2455,21 +2508,21 @@
                     self.state.batch = data_spec.device_transforms(self.state.batch)
 
                 # Count the batch size and num tokens before any events run
                 rank_num_samples = data_spec.get_num_samples_in_batch(self.state.batch)
                 rank_num_tokens = data_spec.get_num_tokens_in_batch(self.state.batch)
 
                 # Fix the batch if using DeepSpeed
-                if self.deepspeed_enabled:
+                if self.state.deepspeed_enabled:
                     self.state.batch = _fix_batch_precision_for_deepspeed(self.state.batch, self.state.precision)
 
                 self.engine.run_event(Event.PREDICT_BATCH_START)
 
                 self.engine.run_event(Event.PREDICT_BEFORE_FORWARD)
-                with _get_precision_context(self.state.precision, self.deepspeed_enabled):
+                with _get_precision_context(self.state.precision, self.state.deepspeed_enabled):
                     self.state.outputs = self.state.model(self.state.batch)
                 self.engine.run_event(Event.PREDICT_AFTER_FORWARD)
 
                 if return_outputs:
                     outputs.append(cpu_device.batch_to_device(self.state.outputs))
 
                 now = datetime.datetime.now()
@@ -2567,30 +2620,44 @@
                 eval_dataloader=[glue_mrpc_task, glue_mnli_task],
                 ...
             )
 
         The metrics used are defined in your model's ``get_metrics()`` method. For more information,
         see :doc:`/trainer/evaluation`.
 
+        .. note::
+
+            If evaluating with multiple GPUs using a DistributedSampler with `drop_last=False`, the last
+            batch will contain duplicate samples, which may affect metrics. To avoid this, as long as
+            the dataset passed to the DistributedSampler has a length defined, Composer will correctly
+            drop duplicate samples.
+
         Args:
-            eval_dataloader (DataLoader | DataSpec | Evaluator | Sequence[Evaluator], optional): Dataloaders
+            eval_dataloader (Iterable | DataLoader | DataSpec | Evaluator | Sequence[Evaluator], optional): Dataloaders
                 for evaluation.  If not provided, defaults to using the
                 ``eval_dataloader`` provided to the trainer init().
             subset_num_batches (int, optional): Evaluate on this many batches. Default to ``-1`` (the entire
                 dataloader. Can also be provided in the trainer.__init__() as ``eval_subset_num_batches``.
 
         """
         if eval_dataloader is not None:
             eval_passed_in = True
             eval_metrics = deepcopy(self._original_model.get_metrics(is_train=False))
             metric_names = [str(k) for k in eval_metrics.keys()]
 
+            eval_dataloader = ensure_tuple(eval_dataloader)
+
+            evaluator_types = [isinstance(evaluator, Evaluator) for evaluator in eval_dataloader]
+            if any(evaluator_types) and not all(evaluator_types):
+                raise ValueError('Mixing Evaluator with other classes is not allowed, please wrap'
+                                 'all other classes with the Evaluator class. These are the classes'
+                                 'that were detected:' + str([type(evaluator) for evaluator in eval_dataloader]))
+
             evaluators = [
-                ensure_evaluator(evaluator, default_metric_names=metric_names)
-                for evaluator in ensure_tuple(eval_dataloader)
+                ensure_evaluator(evaluator, default_metric_names=metric_names) for evaluator in eval_dataloader
             ]
 
             if self.state.eval_metrics:
                 for evaluator in evaluators:
                     if evaluator.label in self.state.eval_metrics:
                         warnings.warn(
                             f'eval_dataloader label \'{evaluator.label}\' was already provided in'
@@ -2666,75 +2733,122 @@
 
             metrics = self._ensure_metrics_device_and_dtype(metrics)
 
             for _, metric in metrics.items():
                 metric.reset()
 
             dataloader = self.state.dataloader
+            dist_sampler = None
+            drop_last = None
+            dataset_len = None
+            last_batch = False
             if isinstance(dataloader, DataLoader) and isinstance(dataloader.sampler, DistributedSampler):
                 # The distributed sampler uses `set_epoch` to set the random seed
                 # Because evaluation can run on each batch, we use the batch to seed the sampler
                 # so each evaluation will get a proper shuffle.
                 # The epoch provided to `set_epoch` need not be sequential, so this is fine.
-                dataloader.sampler.set_epoch(int(self.state.timestamp.batch))
+                dist_sampler = dataloader.sampler
+                dist_sampler.set_epoch(int(self.state.timestamp.batch))
+                drop_last = dataloader.drop_last
+                # Only compute the dataset length if drop_last is False, as otherwise we don't need
+                # to remove any duplicate samples.
+                if drop_last == False:
+                    try:
+                        dataset_len = len(dist_sampler.dataset)  # type: ignore
+                    except AttributeError:
+                        warnings.warn("DistributedSampler's dataset does not have length defined. When "
+                                      '`drop_last=False`, metrics may be incorrect, as DistributedSampler '
+                                      'duplicates samples to make the dataset divisible by world size. To '
+                                      'fix this, provide a dataset with a length attribute to the '
+                                      'DistributedSampler to correctly drop duplicate samples.')
 
             for self.state.batch in self._iter_dataloader(TrainerMode.EVAL):
                 self.state.batch = self.state.device.batch_to_device(self.state.batch)
                 if data_spec.device_transforms is not None:
                     self.state.batch = data_spec.device_transforms(self.state.batch)
 
                 # Count the batch size and num tokens before any events run
                 rank_num_samples = data_spec.get_num_samples_in_batch(self.state.batch)
                 rank_num_tokens = data_spec.get_num_tokens_in_batch(self.state.batch)
 
-                if self.deepspeed_enabled:
+                # If using a distributed sampler, keep track of last_batch for metrics update
+                if dist_sampler is not None and drop_last == False and dataset_len is not None:
+                    batch_num_samples_tensor = self.state.device.tensor_to_device(torch.tensor(rank_num_samples))
+                    dist.all_reduce(batch_num_samples_tensor, reduce_operation='SUM')
+                    batch_num_samples = batch_num_samples_tensor.item()
+                    last_batch = self.state.eval_timestamp.sample + batch_num_samples >= dataset_len
+
+                if self.state.deepspeed_enabled:
                     self.state.batch = _fix_batch_precision_for_deepspeed(self.state.batch, self.state.precision)
 
                 self.engine.run_event(Event.EVAL_BATCH_START)
 
                 # Cache the device batch, because `self.state.batch` gets overridden in microbatching loop
                 device_batch = self.state.batch
                 # Retry until we successfully complete evaluation
                 while True:
                     # Note: We use uint8 instead of bool as BOR is not supported on all torch.distributed backends
                     found_cuda_oom = 0
                     try:
-                        for self.state.batch in data_spec.split_batch(device_batch,
-                                                                      evaluator.device_eval_microbatch_size):
+                        microbatches = data_spec.split_batch(device_batch, evaluator.device_eval_microbatch_size)
+                        for i, self.state.batch in enumerate(microbatches):
+                            last_microbatch = i == len(microbatches) - 1
+                            skip_metric_update = False
+                            # Distributed samplers pad batches to be the same size. If using a
+                            # distributed sampler and on last batch, remove the padding
+                            if dist_sampler is not None and drop_last == False and dataset_len is not None and last_batch and last_microbatch:
+                                padding = dist_sampler.total_size - dataset_len
+                                if dist.get_global_rank() >= dist.get_world_size() - padding:
+                                    rank_num_samples -= 1
+                                    num_samples_in_microbatch = data_spec.get_num_samples_in_batch(self.state.batch)
+                                    # Skip updating metric if batch is only padded samples
+                                    if num_samples_in_microbatch == 1:
+                                        skip_metric_update = True
+                                    # Remove padded samples from batch
+                                    else:
+                                        self.state.batch = data_spec.split_batch(self.state.batch,
+                                                                                 num_samples_in_microbatch - 1)[0]
+
                             self.engine.run_event(Event.EVAL_BEFORE_FORWARD)
-                            with _get_precision_context(self.state.precision, self.deepspeed_enabled):
+
+                            with _get_precision_context(self.state.precision, self.state.deepspeed_enabled):
                                 self.state.outputs = self._original_model.eval_forward(self.state.batch)
-                                target = None
 
                             self.engine.run_event(Event.EVAL_AFTER_FORWARD)
 
+                            # Skip metric update if batch is only padded samples. We do this after
+                            # forward as all models must run forward for FSDP.
+                            if skip_metric_update:
+                                continue
+
                             # Run in same precision context to avoid NaNs
-                            with _get_precision_context(self.state.precision, self.deepspeed_enabled):
+                            with _get_precision_context(self.state.precision, self.state.deepspeed_enabled):
                                 if isinstance(self.state.device, DeviceMPS):
                                     # torchmetrics math has numerical errors on M1 devices
                                     # running the compute on CPU instead
                                     outputs = self.state.outputs.cpu()
                                 else:
                                     outputs = self.state.outputs
 
-                                if hasattr(self._original_model, 'validate'):
-                                    for _, metric in self.state.train_metrics.items():
-                                        metric.update(outputs, target)
-                                else:
-                                    for _, metric in metrics.items():
-                                        self._original_model.update_metric(
-                                            self.state.batch,
-                                            outputs,
-                                            metric,
-                                        )
+                                for _, metric in metrics.items():
+                                    self._original_model.update_metric(
+                                        self.state.batch,
+                                        outputs,
+                                        metric,
+                                    )
 
                     except RuntimeError as e:
                         if evaluator.auto_microbatching and _is_cuda_oom(e):
                             log.debug((f"Rank {dist.get_global_rank()} OOM'd."))
                             found_cuda_oom = 1
+                        elif self.state.auto_microbatching and 'cuda' in str(e).lower() or 'c10' in str(e).lower():
+                            raise ValueError(
+                                textwrap.dedent(
+                                    'Encountered non-addressable cuda error while using auto microbatching. '
+                                    'If this repeatedly occurs, set `device_eval_microbatch_size` manually.')) from e
                         else:
                             raise
                     if evaluator.auto_microbatching:
                         # Propagate across all ranks if any rank hit CUDA OOM
                         found_cuda_oom = self.state.device.tensor_to_device(
                             torch.tensor([found_cuda_oom], dtype=torch.uint8))
                         dist.all_reduce(found_cuda_oom, reduce_operation='MAX')
@@ -2789,15 +2903,15 @@
             using grad scaling.
 
         Raises:
             RuntimeError:
                 Occurs when attempting to use grad scaling without the scaler
                 enabled. Likely due to hardware not supporting the provided precision.
         """
-        if self.deepspeed_enabled:
+        if self.state.deepspeed_enabled:
             return False
 
         precision = Precision(precision)
         use_grad_scaling = precision == Precision.AMP_FP16
 
         if use_grad_scaling and (scaler is None or not scaler.is_enabled()):
             raise RuntimeError(f'Attempting to use grad scaling with {precision}, but scaler is not enabled.'
@@ -2840,15 +2954,15 @@
 
     def _use_closures(self) -> bool:
         """Determines based on precision and optimizers whether to use closures.
 
         We default to using closures unless AMP is enabled, in which case we only allow closures when using optimizers
         with the _step_supports_amp_closure flag.
         """
-        if self.deepspeed_enabled:
+        if self.state.deepspeed_enabled:
             return False
 
         if isinstance(self.state.device, DeviceTPU):
             return False
 
         if self.state.precision != Precision.AMP_FP16:
             return True
@@ -2877,14 +2991,29 @@
         """
         return checkpoint.save_checkpoint(
             state=self.state,
             filename=name,
             weights_only=weights_only,
         )
 
+    def save_checkpoint_to_save_folder(self):
+        """Checkpoints the training :class:`~.State` using a CheckpointSaver if it exists.
+
+        Raises:
+            ValueError: If ``_checkpoint_saver`` does not exist.
+
+        Returns:
+            None
+        """
+        if self._checkpoint_saver is None:
+            raise ValueError(
+                'In order to use save_checkpoint_to_save_folder you must pass a save_folder to the Trainer.')
+        else:
+            self._checkpoint_saver._save_checkpoint(self.state, self.logger)
+
     def export_for_inference(
         self,
         save_format: Union[str, ExportFormat],
         save_path: str,
         save_object_store: Optional[ObjectStore] = None,
         sample_input: Optional[Any] = None,
         transforms: Optional[Sequence[Transform]] = None,
```

### Comparing `composer-0.14.1/composer/utils/__init__.py` & `composer-0.15.0/composer/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/utils/auto_log_hparams.py` & `composer-0.15.0/composer/utils/auto_log_hparams.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/utils/batch_helpers.py` & `composer-0.15.0/composer/utils/batch_helpers.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/utils/checkpoint.py` & `composer-0.15.0/composer/utils/checkpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,28 +71,37 @@
 
 class PartialFilePath:
 
     def __init__(self, filename: str, folder: Optional[str] = None):
         self.folder = folder
         self.filename = filename
 
-    def format(self, state: State, is_deepspeed: bool = False) -> str:
+    def format(self, state: State, is_deepspeed: bool = False, keep_placeholders: bool = False) -> str:
         # if filename already has a suffix (e.g. file.pt), this would append to be file.pt.tar
         extra_suffix = '.tar' if is_deepspeed and not is_tar(self.filename) else ''
         if self.folder:
-            return os.path.join(
-                format_name_with_dist(self.folder, state.run_name),
-                format_name_with_dist_and_time(self.filename, state.run_name, state.timestamp),
-            ) + extra_suffix
+            if keep_placeholders:
+                return os.path.join(
+                    self.folder,
+                    self.filename,
+                ) + extra_suffix
+            else:
+                return os.path.join(
+                    format_name_with_dist(self.folder, state.run_name),
+                    format_name_with_dist_and_time(self.filename, state.run_name, state.timestamp),
+                ) + extra_suffix
         else:
-            return format_name_with_dist_and_time(
-                self.filename,
-                state.run_name,
-                state.timestamp,
-            ) + extra_suffix
+            if keep_placeholders:
+                return self.filename + extra_suffix
+            else:
+                return format_name_with_dist_and_time(
+                    self.filename,
+                    state.run_name,
+                    state.timestamp,
+                ) + extra_suffix
 
 
 def load_checkpoint(
     path: str,
     state: State,
     logger: Logger,
     object_store: Optional[Union[ObjectStore, LoggerDestination]] = None,
@@ -406,24 +415,56 @@
         # Loop through all paths to exclude
         paths_to_remove = [path.split('/') for path in filtered_paths]
         _remove_paths(state_dict, paths_to_remove)
 
     return filter_func
 
 
-def safe_torch_load(composer_states_filepath: Union[Path, str], map_location: str = 'cpu'):
+def safe_torch_load(
+    composer_states_filepath: Union[Path, str],
+    map_location: str = 'cpu',
+    load_fsdp_monolith_rank0_only: bool = False,
+) -> Dict[str, Any]:
     """Load a torch checkpoint, catching errors due to backwards compatibility issues.
 
     Args:
         composer_states_filepath: The path to the checkpoint file.
         map_location: The location to load the checkpoint to.
+        load_fsdp_monolith_rank0_only: Whether the checkpoint is a monolith FSDP checkpoint.
     """
     try:
-        state_dict = torch.load(composer_states_filepath, map_location=map_location)
-        return state_dict
+        if load_fsdp_monolith_rank0_only:
+            log.info(
+                'Loading monolith FSDP checkpoint. Only rank 0 will load and broadcast non-weight/optimizer state.')
+            state_dict_list = [None]
+            model = None
+            optimizer = None
+            if dist.get_global_rank() == 0:
+                state_dict_list[0] = torch.load(composer_states_filepath, map_location=map_location)
+                # Don't broadcast model/optimizer state if they exist
+                if 'model' in state_dict_list[0]['state']:
+                    model = state_dict_list[0]['state']['model']
+                    state_dict_list[0]['state']['model'] = None
+                if 'optimizers' in state_dict_list[0]['state']:
+                    optimizer = state_dict_list[0]['state']['optimizers']
+                    state_dict_list[0]['state']['optimizers'] = None
+
+            log.debug('Broadcasting state_dict to all ranks.')
+            dist.broadcast_object_list(state_dict_list, src=0)
+            state_dict: Dict[str, Any] = state_dict_list[0]  # type: ignore
+
+            if dist.get_global_rank() == 0:
+                if model is not None:
+                    state_dict['state']['model'] = model
+                if optimizer is not None:
+                    state_dict['state']['optimizers'] = optimizer
+
+            return state_dict
+        else:
+            return torch.load(composer_states_filepath, map_location=map_location)
     except TypeError as e:
         if 'Accuracy.__new__() missing 1 required positional argument' in str(e):
             raise Exception('As of v0.10.0, torchmetrics introduces a new required argument to Accuracy which '
                             'breaks backwards compatibility. Unfortunately, this means that older checkpoints '
                             'cannot be loaded with the metrics. In order to successfully load this model, please '
                             'pass `load_ignore_keys = ["state/train_metrics/*", "state/eval_metrics/*"]`.') from e
         raise e
@@ -439,15 +480,18 @@
     strict_model_weights: bool,
     ignore_keys: Optional[Union[List[str], Callable[[Dict], None]]],
     exclude_algorithms: Optional[List[str]],
     algorithm_passes: Optional[List[AlgorithmPass]],
 ) -> Optional[List[Dict[str, Any]]]:
     """Restore a checkpoint into ``state`` and returns the rng state dicts (if ``load_weights_only`` is False)."""
     # Now, all ranks load the checkpoint that local rank zero downloaded
-    state_dict = safe_torch_load(composer_states_filepath)
+    state_dict = safe_torch_load(
+        composer_states_filepath=composer_states_filepath,
+        load_fsdp_monolith_rank0_only=state.load_fsdp_monolith_rank0_only,
+    )
     if ignore_keys:
         # Filter provided list of key paths
         if not callable(ignore_keys):
             ignore_keys = glob_filter(ignore_keys)
         # Call function to modify state_dict
         ignore_keys(state_dict)
     log.debug(f"Loaded checkpoint with keys {state_dict.keys()} and state keys {state_dict['state'].keys()}")
@@ -517,15 +561,27 @@
     state_dict = {
         'state': state.state_dict(),
         'rng': reproducibility.get_rng_state(),
     }
     if weights_only and not is_deepspeed:
         state_dict['state'] = {'model': state_dict['state']['model']}
 
-    save_filename = PartialFilePath(filename).format(state, is_deepspeed)
+    # Sharded checkpoints get their own little folder.
+    if state.fsdp_sharded_state_dict_enabled:
+        assert state.sharded_ckpt_prefix_dir is not None
+        save_prefix_folder = state.sharded_ckpt_prefix_dir
+        # New name is now Trainer.save_folder / sharded_ckpt_prefix_dir / Trainer.save_filename
+        # e.g. path/to/my/checkpoints/ep{epoch}-ba{batch}/ep{epoch}-ba{batch}-rank{rank}.pt
+        save_filepath = Path(Path(filename).parent) / Path(save_prefix_folder) / Path(Path(filename).name)
+        # Fill in remaining placeholders.
+        save_filename = format_name_with_dist_and_time(str(save_filepath), state.run_name, state.timestamp)
+        log.debug('Saving sharded checkpoints to %s...', save_filename)
+    else:
+        save_filename = PartialFilePath(filename).format(state, is_deepspeed)
+
     dirname = os.path.dirname(save_filename)
     if dirname:
         os.makedirs(dirname, exist_ok=True)
 
     # only rank 0 saves the state_dict unless state.fsdp_sharded_state_dict_enabled=True.
     if dist.get_global_rank() == 0 or state.fsdp_sharded_state_dict_enabled:
         with open(save_filename, 'wb') as f:
```

### Comparing `composer-0.14.1/composer/utils/collect_env.py` & `composer-0.15.0/composer/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/utils/device.py` & `composer-0.15.0/composer/utils/device.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/utils/dist.py` & `composer-0.15.0/composer/utils/dist.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/utils/file_helpers.py` & `composer-0.15.0/composer/utils/file_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -411,21 +411,19 @@
                                   'WandBLogger with log_artifacts set to True')
 
     else:
         raise NotImplementedError(f'There is no implementation for the cloud backend {backend} via URI. Please use '
                                   's3 or one of the supported RemoteUploaderDownloader object stores')
 
 
-def get_file(
-    path: str,
-    destination: str,
-    object_store: Optional[Union[ObjectStore, LoggerDestination]] = None,
-    overwrite: bool = False,
-    progress_bar: bool = True,
-):
+def get_file(path: str,
+             destination: str,
+             object_store: Optional[Union[ObjectStore, LoggerDestination]] = None,
+             overwrite: bool = False,
+             progress_bar: bool = True):
     """Get a file from a local folder, URL, or object store.
 
     Args:
         path (str): The path to the file to retrieve.
 
             *   If ``object_store`` is specified, then the ``path`` should be the object name for the file to get.
                 Do not include the the cloud provider or bucket name.
@@ -477,41 +475,37 @@
             )
             # Read object name in the symlink
             with open(symlink_file_name, 'r') as f:
                 real_path = f.read()
                 log.debug(f'Read path {real_path} from symlink file.')
 
         # Recurse
-        return get_file(
-            path=real_path,
-            destination=destination,
-            object_store=object_store,
-            overwrite=overwrite,
-            progress_bar=progress_bar,
-        )
+        return get_file(path=real_path,
+                        destination=destination,
+                        object_store=object_store,
+                        overwrite=overwrite,
+                        progress_bar=progress_bar)
 
     try:
         _get_file(
             path=path,
             destination=destination,
             object_store=object_store,
             overwrite=overwrite,
             progress_bar=progress_bar,
         )
     except FileNotFoundError as e:
         new_path = path + '.symlink'
         try:
             # Follow the symlink
-            return get_file(
-                path=new_path,
-                destination=destination,
-                object_store=object_store,
-                overwrite=overwrite,
-                progress_bar=progress_bar,
-            )
+            return get_file(path=new_path,
+                            destination=destination,
+                            object_store=object_store,
+                            overwrite=overwrite,
+                            progress_bar=progress_bar)
         except FileNotFoundError as ee:
             # Raise the original not found error first, which contains the path to the user-specified file
             raise e from ee
 
 
 def _get_file(
     path: str,
@@ -574,14 +568,18 @@
             else:
                 os.rename(tmp_path, destination)
         return
 
     # It's a local filepath
     if not os.path.exists(path):
         raise FileNotFoundError(f'Local path {path} does not exist')
+
+    if os.path.exists(destination) and overwrite:
+        os.remove(destination)
+
     os.symlink(os.path.abspath(path), destination)
 
 
 def _get_callback(description: str):
     if len(description) > 60:
         description = description[:42] + '...' + description[-15:]
     pbar = None
```

### Comparing `composer-0.14.1/composer/utils/fx_utils.py` & `composer-0.15.0/composer/utils/fx_utils.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/utils/import_helpers.py` & `composer-0.15.0/composer/utils/import_helpers.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/utils/inference.py` & `composer-0.15.0/composer/utils/inference.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/utils/iter_helpers.py` & `composer-0.15.0/composer/utils/iter_helpers.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/utils/misc.py` & `composer-0.15.0/composer/utils/misc.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/utils/module_surgery.py` & `composer-0.15.0/composer/utils/module_surgery.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/utils/object_store/__init__.py` & `composer-0.15.0/composer/utils/object_store/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/utils/object_store/libcloud_object_store.py` & `composer-0.15.0/composer/utils/object_store/libcloud_object_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,14 +166,17 @@
         overwrite: bool = False,
         callback: Optional[Callable[[int, int], None]] = None,
     ):
         if os.path.exists(filename) and not overwrite:
             # If the file already exits, short-circuit and skip the download
             raise FileExistsError(f'filename {filename} exists and overwrite was set to False.')
 
+        dirname = os.path.dirname(filename)
+        if dirname:
+            os.makedirs(dirname, exist_ok=True)
         obj = self._get_object(object_name)
         # Download first to a tempfile, and then rename, in case if the file gets corrupted in transit
         tmp_filepath = str(filename) + f'.{uuid.uuid4()}.tmp'
         try:
             with open(tmp_filepath, 'wb+') as f:
                 stream = self._provider.download_object_as_stream(obj, chunk_size=self.chunk_size)
                 for chunk in iterate_with_callback(stream, obj.size, callback):
```

### Comparing `composer-0.14.1/composer/utils/object_store/object_store.py` & `composer-0.15.0/composer/utils/object_store/object_store.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/utils/object_store/oci_object_store.py` & `composer-0.15.0/composer/utils/object_store/oci_object_store.py`

 * *Files 3% similar despite different names*

```diff
@@ -122,14 +122,18 @@
         filename: Union[str, pathlib.Path],
         overwrite: bool = False,
         callback: Optional[Callable[[int, int], None]] = None,
     ):
         del callback
         if os.path.exists(filename) and not overwrite:
             raise FileExistsError(f'The file at {filename} already exists and overwrite is set to False')
+
+        dirname = os.path.dirname(filename)
+        if dirname:
+            os.makedirs(dirname, exist_ok=True)
         tmp_path = str(filename) + f'.{uuid.uuid4()}.tmp'
 
         try:
             response = self.client.get_object(
                 namespace_name=self.namespace,
                 bucket_name=self.bucket,
                 object_name=object_name,
```

### Comparing `composer-0.14.1/composer/utils/object_store/s3_object_store.py` & `composer-0.15.0/composer/utils/object_store/s3_object_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,15 +141,20 @@
         object_name: str,
         filename: Union[str, pathlib.Path],
         overwrite: bool = False,
         callback: Optional[Callable[[int, int], None]] = None,
     ):
         if os.path.exists(filename) and not overwrite:
             raise FileExistsError(f'The file at {filename} already exists and overwrite is set to False.')
+
+        dirname = os.path.dirname(filename)
+        if dirname:
+            os.makedirs(dirname, exist_ok=True)
         tmp_path = str(filename) + f'.{uuid.uuid4()}.tmp'
+
         if callback is None:
             cb_wrapper = None
         else:
             file_size = self.get_object_size(object_name)
             cb_wrapper = lambda bytes_transferred: callback(bytes_transferred, file_size)
 
         try:
```

### Comparing `composer-0.14.1/composer/utils/object_store/sftp_object_store.py` & `composer-0.15.0/composer/utils/object_store/sftp_object_store.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/utils/reproducibility.py` & `composer-0.15.0/composer/utils/reproducibility.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/utils/retrying.py` & `composer-0.15.0/composer/utils/retrying.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer/utils/string_enum.py` & `composer-0.15.0/composer/utils/string_enum.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer.egg-info/PKG-INFO` & `composer-0.15.0/composer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composer
-Version: 0.14.1
+Version: 0.15.0
 Summary: Composer is a PyTorch library that enables you to train neural networks faster, at lower cost, and to higher accuracy.
 Home-page: https://github.com/mosaicml/composer
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -27,15 +27,14 @@
 Provides-Extra: sentencepiece
 Provides-Extra: mlperf
 Provides-Extra: streaming
 Provides-Extra: libcloud
 Provides-Extra: oci
 Provides-Extra: onnx
 Provides-Extra: mlflow
-Provides-Extra: mcli
 Provides-Extra: all
 License-File: LICENSE
 
 <br />
 <p align="center">
     <a href="https://github.com/mosaicml/composer#gh-light-mode-only" class="only-light">
       <img src="https://storage.googleapis.com/docs.mosaicml.com/images/header_light.svg" width="50%"/>
@@ -63,15 +62,15 @@
     </a>
     <a href="https://pepy.tech/project/mosaicml/">
         <img alt="PyPi Downloads" src="https://static.pepy.tech/personalized-badge/mosaicml?period=month&units=international_system&left_color=grey&right_color=blue&left_text=Downloads/month">
     </a>
     <a href="https://docs.mosaicml.com/projects/composer/en/stable/">
         <img alt="Documentation" src="https://readthedocs.org/projects/composer/badge/?version=stable">
     </a>
-    <a href="https://join.slack.com/t/mosaicml-community/shared_invite/zt-w0tiddn9-WGTlRpfjcO9J5jyrMub1dg">
+    <a href="https://mosaicml.me/slack">
         <img alt="Chat @ Slack" src="https://img.shields.io/badge/slack-chat-2eb67d.svg?logo=slack">
     </a>
     <a href="https://github.com/mosaicml/composer/blob/dev/LICENSE">
         <img alt="License" src="https://img.shields.io/badge/License-Apache%202.0-green.svg?logo=slack">
     </a>
 </p>
 <br />
```

#### html2text {}

```diff
@@ -1,22 +1,21 @@
-Metadata-Version: 2.1 Name: composer Version: 0.14.1 Summary: Composer is a
+Metadata-Version: 2.1 Name: composer Version: 0.15.0 Summary: Composer is a
 PyTorch library that enables you to train neural networks faster, at lower
 cost, and to higher accuracy. Home-page: https://github.com/mosaicml/composer
 Author: MosaicML Author-email: team@mosaicml.com Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Requires-Python: >=3.8 Description-Content-Type:
 text/markdown Provides-Extra: base Provides-Extra: dev Provides-Extra:
 health_checker Provides-Extra: slack Provides-Extra: deepspeed Provides-Extra:
 wandb Provides-Extra: comet_ml Provides-Extra: tensorboard Provides-Extra: unet
 Provides-Extra: vit Provides-Extra: timm Provides-Extra: coco Provides-Extra:
 nlp Provides-Extra: sentencepiece Provides-Extra: mlperf Provides-Extra:
 streaming Provides-Extra: libcloud Provides-Extra: oci Provides-Extra: onnx
-Provides-Extra: mlflow Provides-Extra: mcli Provides-Extra: all License-File:
-LICENSE
+Provides-Extra: mlflow Provides-Extra: all License-File: LICENSE
   [https://storage.googleapis.com/docs.mosaicml.com/images/header_light.svg]
 ***** A PyTorch Library for Efficient Neural Network Training *****
 **** Train Faster, Reduce Cost, Get Better Models ****
 *** [Website] - [Getting_Started] - [Docs] - [Methods] - [We're_Hiring!] ***
 [PyPi_Version] [PyPi_Package_Version] [PyPi_Downloads] [Documentation] [Chat_@
                                Slack] [License]
```

### Comparing `composer-0.14.1/composer.egg-info/SOURCES.txt` & `composer-0.15.0/composer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/composer.egg-info/requires.txt` & `composer-0.15.0/composer.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,114 +1,114 @@
 pyyaml<7,>=6.0
 tqdm<5,>=4.62.3
-torchmetrics<0.11.4,>=0.10.0
+torchmetrics<0.12,>=0.10.0
 torch_optimizer<0.4,>=0.3.0
-torchvision<0.16,>=0.11.0
-torch<2.1,>=1.10.0
+torchvision<0.16,>=0.13.1
+torch<2.1,>=1.13.1
 requests<3,>=2.26.0
 numpy<1.25.0,>=1.21.5
 psutil<6,>=5.8.0
 coolname<3,>=1.1.0
 tabulate==0.9.0
 py-cpuinfo<10,>=8.0.0
 packaging<23,>=21.3.0
 importlib-metadata<7,>=5.0.0
+mosaicml-cli<0.5,>=0.4.0
 
 [all]
-ipython==8.11.0
-paramiko<3,>=2.11.0
-timm<0.6,>=0.5.4
 sphinxcontrib-images==0.9.4
-sentencepiece==0.1.98
-recommonmark==0.7.1
-deepspeed==0.8.3
-testbook==0.4.2
+oci<3.0.0,>=2.88.2
+toml==0.10.2
+sphinx_panels==0.6.0
+comet_ml<4.0.0,>=3.31.12
+onnx<2,>=1.12.0
+pytest_codeblocks==0.16.1
+sphinxcontrib.katex==0.9.5
+scikit-learn<2,>=1.0.1
+moto[s3]<5,>=4.0.1
+mlflow<3.0,>=2.0.1
+slack_sdk<4,>=3.19.5
+timm<0.6,>=0.5.4
+mosaicml-streaming<1.0
+junitparser==3.1.0
+GitPython==3.1.31
 pycocotools<3,>=2.0.4
-boto3<2,>=1.21.45
-transformers<4.29,>=4.11
+custom_inherit==2.4.1
+py-cpuinfo<10,>=8.0.0
+wandb<0.16,>=0.13.2
+apache-libcloud<4,>=3.3.1
 pypandoc==1.11
-junitparser==3.0.0
+onnxruntime<2,>=1.12.1
+paramiko<3,>=2.11.0
+recommonmark==0.7.1
 docutils==0.17.1
-traitlets==5.9.0
-pre-commit<3,>=2.18.1
-mock-ssh-server==0.9.1
-mosaicml-cli<0.4,>=0.3.6
+sphinxemoji==0.2.0
+monai<1.3,>=0.9.1
 furo==2022.9.29
-vit_pytorch==0.35.8
-sphinxext.opengraph==0.8.2
-setuptools<=59.5.0
-sphinxcontrib.katex==0.9.4
+coverage[toml]==7.2.7
 sphinx-argparse==0.4.0
-onnxruntime<2,>=1.12.1
-nbsphinx==0.9.1
-cryptography==38.0.4
 datasets<3,>=2.4
-GitPython==3.1.31
-jupyter==1.0.0
-wandb<0.16,>=0.13.2
-custom_inherit==2.4.1
-mlflow<3.0,>=2.0.1
+pynvml<12,>=11.5.0
+protobuf<3.21
 sphinx_markdown_tables==0.0.17
-mosaicml-streaming<1.0
-oci<3.0.0,>=2.88.2
-slack_sdk<4,>=3.19.5
-myst-parser==0.16.1
-pandoc==2.3
-pytest==7.3.1
+deepspeed==0.8.3
+cryptography==38.0.4
+sphinx-copybutton==0.5.2
 pytest-httpserver<1.1,>=1.0.4
-sphinx==4.4.0
-monai<1.2,>=0.9.1
-moto[s3]<5,>=4.0.1
-protobuf<3.21
-py-cpuinfo<10,>=8.0.0
-coverage[toml]==7.2.5
-onnx<2,>=1.12.0
-pytest_codeblocks==0.16.1
-pynvml<12,>=11.5.0
-comet_ml<4.0.0,>=3.31.12
-ipykernel==6.22.0
-sphinx_panels==0.6.0
-scikit-learn<2,>=1.0.1
-apache-libcloud<4,>=3.3.1
-yamllint==1.31.0
+pytest==7.3.1
+pre-commit<3,>=2.18.1
+vit_pytorch==0.35.8
 tensorboard<3.0.0,>=2.9.1
-sphinx-copybutton==0.5.2
+traitlets==5.9.0
+ipykernel==6.23.1
+boto3<2,>=1.21.45
 fasteners==0.18
-toml==0.10.2
-sphinxemoji==0.2.0
+jupyter==1.0.0
+sphinx==4.4.0
+testbook==0.4.2
+myst-parser==0.16.1
+pandoc==2.3
+mock-ssh-server==0.9.1
+transformers<4.31,>=4.11
+ipython==8.11.0
+sentencepiece==0.1.99
+nbsphinx==0.9.1
+setuptools<=59.5.0
+yamllint==1.32.0
+sphinxext.opengraph==0.8.2
 
 [base]
 
 [coco]
 pycocotools<3,>=2.0.4
 
 [comet_ml]
 comet_ml<4.0.0,>=3.31.12
 
 [deepspeed]
 deepspeed==0.8.3
 
 [dev]
 custom_inherit==2.4.1
-junitparser==3.0.0
-coverage[toml]==7.2.5
+junitparser==3.1.0
+coverage[toml]==7.2.7
 fasteners==0.18
 pytest==7.3.1
 toml==0.10.2
 ipython==8.11.0
-ipykernel==6.22.0
+ipykernel==6.23.1
 jupyter==1.0.0
-yamllint==1.31.0
+yamllint==1.32.0
 recommonmark==0.7.1
 sphinx==4.4.0
 pre-commit<3,>=2.18.1
 docutils==0.17.1
 sphinx_markdown_tables==0.0.17
 sphinx-argparse==0.4.0
-sphinxcontrib.katex==0.9.4
+sphinxcontrib.katex==0.9.5
 sphinxext.opengraph==0.8.2
 sphinxemoji==0.2.0
 furo==2022.9.29
 sphinx-copybutton==0.5.2
 testbook==0.4.2
 myst-parser==0.16.1
 sphinx_panels==0.6.0
@@ -127,37 +127,34 @@
 
 [health_checker]
 pynvml<12,>=11.5.0
 
 [libcloud]
 apache-libcloud<4,>=3.3.1
 
-[mcli]
-mosaicml-cli<0.4,>=0.3.6
-
 [mlflow]
 mlflow<3.0,>=2.0.1
 
 [mlperf]
 py-cpuinfo<10,>=8.0.0
 
 [nlp]
-transformers<4.29,>=4.11
+transformers<4.31,>=4.11
 datasets<3,>=2.4
 
 [oci]
 oci<3.0.0,>=2.88.2
 
 [onnx]
 onnx<2,>=1.12.0
 onnxruntime<2,>=1.12.1
 
 [sentencepiece]
 protobuf<3.21
-sentencepiece==0.1.98
+sentencepiece==0.1.99
 
 [slack]
 slack_sdk<4,>=3.19.5
 
 [streaming]
 mosaicml-streaming<1.0
 boto3<2,>=1.21.45
@@ -166,15 +163,15 @@
 [tensorboard]
 tensorboard<3.0.0,>=2.9.1
 
 [timm]
 timm<0.6,>=0.5.4
 
 [unet]
-monai<1.2,>=0.9.1
+monai<1.3,>=0.9.1
 scikit-learn<2,>=1.0.1
 
 [vit]
 vit_pytorch==0.35.8
 
 [wandb]
 wandb<0.16,>=0.13.2
```

### Comparing `composer-0.14.1/pyproject.toml` & `composer-0.15.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -92,33 +92,24 @@
 
     # Ignore the following warnings
     'ignore:Deterministic mode is activated:UserWarning',  # All tests run with deterministic mode
     'ignore:SubsetNumBatchesWarning',  # SubsetNumBatches is used extensively in testing
     # allow training metrics
     'ignore:Computing model evaluation metrics during training doubles the number of forward passes:UserWarning',
     'ignore:No optimizer was specified.:UserWarning',  # OK to not specify an optimizer in the tests
-    # Ignore deprecation warnings in pillow. TODO: remove this ignore for when we upgrade pillow-simd +
-    # use torchvision 0.13  -- it appears to be fixed in main -- see
-    # https://github.com/pytorch/vision/blob/main/torchvision/transforms/functional_pil.py
-    'ignore:.*is deprecated and will be removed in Pillow 10.*:DeprecationWarning',
-    # Ignore deprecation warnings in deepspeed. TODO: remove this when we upgrade to v0.6.1+ -- it has been fixed
-    'ignore::DeprecationWarning:deepspeed.*:',
-    # Ingore validate is deprecated warnings. TODO(ravi) Need to manually remove on hparams.validate functionality
-    'ignore:.*Instead, perform any validation directly in initialize_object\(\):DeprecationWarning',
     # Ignore a bug in the pytorch dataloader
     '''ignore:Exception ignored in. <function _MultiProcessingDataLoaderIter.__del__:pytest.PytestUnraisableExceptionWarning''',
     # Ignore torchvision complaining about no c libraries (happens in the conda build)
     'ignore:Failed to load image Python extension:UserWarning',
     # Ignore a deprecation warning in the conda build
     'ignore:distutils Version classes are deprecated:DeprecationWarning',
     # Ignore a UserWarning from TorchMetrics about potentially large memory usage when batch sizes are extremely large
     'ignore:Metric `SpearmanCorrcoef` will save all targets and predictions in the buffer:UserWarning:torchmetrics',
     # Ignore a UserWarning from torch 1.12 due to DeepSpeed's use of positional args
     'ignore:Positional args are being deprecated, use kwargs instead.*:UserWarning',
-    'ignore:Torchmetrics v0.9 introduced a new argument class property:UserWarning',
     'ignore:torch.distributed._all_gather_base is a private function and will be deprecated.*:UserWarning',
     'ignore:torch.distributed._reduce_scatter_base is a private function and will be deprecated.*:UserWarning',
     # Ignore tensorboard deprecation warnings
     'ignore:Call to deprecated create function Descriptor().*:DeprecationWarning:tensorboard',
     'ignore:Call to deprecated create function EnumDescriptor().*:DeprecationWarning:tensorboard',
     'ignore:Call to deprecated create function EnumValueDescriptor().*:DeprecationWarning:tensorboard',
     'ignore:Call to deprecated create function FieldDescriptor().*:DeprecationWarning:tensorboard',
```

### Comparing `composer-0.14.1/setup.py` & `composer-0.15.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,54 +71,55 @@
     else:
         assert end != -1, 'there should be a balanced number of start and ends'
         long_description = long_description[:start] + long_description[end + len(end_tag):]
 
 install_requires = [
     'pyyaml>=6.0,<7',
     'tqdm>=4.62.3,<5',
-    'torchmetrics>=0.10.0,<0.11.4',
+    'torchmetrics>=0.10.0,<0.12',
     'torch_optimizer>=0.3.0,<0.4',
-    'torchvision>=0.11.0,<0.16',
-    'torch>=1.10.0,<2.1',
+    'torchvision>=0.13.1,<0.16',
+    'torch>=1.13.1,<2.1',
     'requests>=2.26.0,<3',
     'numpy>=1.21.5,<1.25.0',
     'psutil>=5.8.0,<6',
     'coolname>=1.1.0,<3',
     'tabulate==0.9.0',  # for auto-generating tables
     'py-cpuinfo>=8.0.0,<10',
     'packaging>=21.3.0,<23',
     'importlib-metadata>=5.0.0,<7',
+    'mosaicml-cli>=0.4.0,<0.5',
 ]
 extra_deps = {}
 
 extra_deps['base'] = []
 
 extra_deps['dev'] = [
     # Imports for docs builds and running tests
     # Pinning versions strictly to avoid random test failures.
     # Should manually update dependency versions occassionally.
     'custom_inherit==2.4.1',
-    'junitparser==3.0.0',
-    'coverage[toml]==7.2.5',
+    'junitparser==3.1.0',
+    'coverage[toml]==7.2.7',
     'fasteners==0.18',  # object store tests require fasteners
     'pytest==7.3.1',
     'toml==0.10.2',
     'ipython==8.11.0',
-    'ipykernel==6.22.0',
+    'ipykernel==6.23.1',
     'jupyter==1.0.0',
-    'yamllint==1.31.0',
+    'yamllint==1.32.0',
     'recommonmark==0.7.1',
     'sphinx==4.4.0',
     'pre-commit>=2.18.1,<3',
     # embedding md in rst require docutils>=0.17. See
     # https://myst-parser.readthedocs.io/en/latest/sphinx/use.html?highlight=parser#include-markdown-files-into-an-rst-file
     'docutils==0.17.1',
     'sphinx_markdown_tables==0.0.17',
     'sphinx-argparse==0.4.0',
-    'sphinxcontrib.katex==0.9.4',
+    'sphinxcontrib.katex==0.9.5',
     'sphinxext.opengraph==0.8.2',
     'sphinxemoji==0.2.0',
     'furo==2022.9.29',
     'sphinx-copybutton==0.5.2',
     'testbook==0.4.2',
     'myst-parser==0.16.1',
     'sphinx_panels==0.6.0',
@@ -157,15 +158,15 @@
 ]
 
 extra_deps['tensorboard'] = [
     'tensorboard>=2.9.1,<3.0.0',
 ]
 
 extra_deps['unet'] = [
-    'monai>=0.9.1,<1.2',
+    'monai>=0.9.1,<1.3',
     'scikit-learn>=1.0.1,<2',
 ]
 
 extra_deps['vit'] = [
     'vit_pytorch==0.35.8',
 ]
 
@@ -174,21 +175,21 @@
 ]
 
 extra_deps['coco'] = [
     'pycocotools>=2.0.4,<3',
 ]
 
 extra_deps['nlp'] = [
-    'transformers>=4.11,<4.29',
+    'transformers>=4.11,<4.31',
     'datasets>=2.4,<3',
 ]
 
 extra_deps['sentencepiece'] = [
     'protobuf<3.21',
-    'sentencepiece==0.1.98',
+    'sentencepiece==0.1.99',
 ]
 
 extra_deps['mlperf'] = [
     # TODO: use pip when available: https://github.com/mlcommons/logging/issues/218
     # "mlperf_logging @ git+https://github.com/mlperf/logging.git",
     'py-cpuinfo>=8.0.0,<10',
 ]
@@ -212,18 +213,14 @@
     'onnxruntime>=1.12.1,<2',
 ]
 
 extra_deps['mlflow'] = [
     'mlflow>=2.0.1,<3.0',
 ]
 
-extra_deps['mcli'] = [
-    'mosaicml-cli>=0.3.6,<0.4',
-]
-
 extra_deps['all'] = set(dep for deps in extra_deps.values() for dep in deps)
 
 composer_data_files = ['py.typed']
 composer_data_files += package_files('composer', 'yamls', '.yaml')
 composer_data_files += package_files('composer', 'algorithms', '.json')
 
 package_name = os.environ.get('COMPOSER_PACKAGE_NAME', 'mosaicml')
```

### Comparing `composer-0.14.1/tests/test_device.py` & `composer-0.15.0/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/tests/test_docker.py` & `composer-0.15.0/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/tests/test_docs.py` & `composer-0.15.0/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/tests/test_engine.py` & `composer-0.15.0/tests/test_engine.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/tests/test_events.py` & `composer-0.15.0/tests/test_events.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,26 +30,34 @@
         model = SimpleModel()
         optimizer = torch.optim.Adam(model.parameters())
 
         train_dataset = RandomClassificationDataset()
         eval_dataset = RandomClassificationDataset()
         train_batch_size = 4
 
+        evaluator1 = DataLoader(
+            dataset=eval_dataset,
+            batch_size=8,
+            sampler=dist.get_sampler(eval_dataset),
+        )
+
+        evaluator2 = DataLoader(
+            dataset=eval_dataset,
+            batch_size=4,
+            sampler=dist.get_sampler(eval_dataset),
+        )
+
         return Trainer(
             model=model,
             train_dataloader=DataLoader(
                 dataset=train_dataset,
                 batch_size=train_batch_size,
                 sampler=dist.get_sampler(train_dataset),
             ),
-            eval_dataloader=DataLoader(
-                dataset=eval_dataset,
-                batch_size=8,
-                sampler=dist.get_sampler(eval_dataset),
-            ),
+            eval_dataloader=(evaluator1, evaluator2),
             device_train_microbatch_size=train_batch_size // 2,
             precision=precision,
             train_subset_num_batches=self.train_subset_num_batches,
             eval_subset_num_batches=self.eval_subset_num_batches,
             max_duration='2ep',
             optimizers=optimizer,
             callbacks=[EventCounterCallback()],
@@ -126,17 +134,19 @@
         elif eval_interval.unit == TimeUnit.EPOCH:
             total_evals = num_epochs // int(eval_interval)
         else:
             total_evals = 0
 
         if trainer.state.evaluators:
             steps_per_eval = self.eval_subset_num_batches
+            total_evals_start = total_evals * len(trainer.state.evaluators)
             total_eval_steps = total_evals * steps_per_eval * len(trainer.state.evaluators)
         else:
             total_eval_steps = 0
+            total_evals_start = 0
 
         expected_num_calls = {
             Event.INIT: 1,
             Event.AFTER_LOAD: 1,
             Event.EPOCH_START: num_epochs,
             Event.BATCH_START: total_steps,
             Event.BEFORE_DATALOADER: total_steps + num_epochs,  # extra call per epoch when dataloader is exhausted
@@ -149,20 +159,22 @@
             Event.AFTER_BACKWARD: total_microbatches,
             Event.BEFORE_TRAIN_BATCH: total_steps,
             Event.AFTER_TRAIN_BATCH: total_steps,
             Event.BATCH_END: total_steps,
             Event.BATCH_CHECKPOINT: total_steps,
             Event.EPOCH_END: num_epochs,
             Event.EPOCH_CHECKPOINT: num_epochs,
-            Event.EVAL_START: total_evals,
+            Event.EVAL_BEFORE_ALL: total_evals,
+            Event.EVAL_START: total_evals_start,
             Event.EVAL_BATCH_START: total_eval_steps,
             Event.EVAL_BEFORE_FORWARD: total_eval_steps,
             Event.EVAL_AFTER_FORWARD: total_eval_steps,
             Event.EVAL_BATCH_END: total_eval_steps,
-            Event.EVAL_END: total_evals,
+            Event.EVAL_END: total_evals_start,
+            Event.EVAL_AFTER_ALL: total_evals,
         }
 
         counter_callback = (cb for cb in trainer.state.callbacks if isinstance(cb, EventCounterCallback))
         counter_callback = next(counter_callback)
         for event, expected in expected_num_calls.items():
             actual = counter_callback.event_to_num_calls[event]
             assert expected == actual, f'{event} call mismatch: {expected} != {actual}'
```

### Comparing `composer-0.14.1/tests/test_full_nlp.py` & `composer-0.15.0/tests/test_full_nlp.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,14 +114,15 @@
     # The pretraining weights have not yet been loaded into the finetuning model
     assert not torch.equal(finetuning_embedding_layer.cpu(), pretraining_embedding_layer.cpu())
     finetuning_trainer = Trainer(model=model,
                                  train_dataloader=finetuning_train_dataloader,
                                  save_folder='finetuning_checkpoints',
                                  load_path=checkpoint_path,
                                  load_weights_only=True,
+                                 load_strict_model_weights=False,
                                  loggers=[rud],
                                  max_duration='1ep',
                                  seed=17,
                                  algorithms=algorithms,
                                  device=device)
     # Now they have been loaded
     assert torch.equal(finetuning_embedding_layer.cpu(), pretraining_embedding_layer.cpu())
```

### Comparing `composer-0.14.1/tests/test_loss.py` & `composer-0.15.0/tests/test_loss.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,17 +105,17 @@
 class TestSoftCrossEntropy:
 
     def test_infer_target_type(self, tensors):
         input, target_indices, target_onehot = tensors
         assert infer_target_type(input, target_indices) == 'indices'
         assert infer_target_type(input, target_onehot) == 'one_hot'
 
+    # Note: Weights xfail as our implementation differs from PyTorch
     @pytest.mark.parametrize('reduction', ['mean', 'sum'])
     @pytest.mark.parametrize('use_weights', [xfail(True), False])
-    # TODO(Cory): Remove this filterwarning
     @pytest.mark.filterwarnings(r'ignore:Some targets have less than 1 total probability:UserWarning')
     def test_soft_cross_entropy(self, tensors, use_weights, reduction):
         input, target_indices, target_onehot = tensors
         if use_weights:
             num_classes = target_onehot.shape[1]
             weights = torch.rand(size=[num_classes])
         else:
```

### Comparing `composer-0.14.1/tests/test_notebooks.py` & `composer-0.15.0/tests/test_notebooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,16 @@
         pytest.skip('The CI does not support SLURM and submitit')
     if notebook_name == 'auto_microbatching' and device == 'cpu':
         pytest.skip('auto_microbatching notebook only runs with a gpu')
     if notebook_name == 'TPU_Training_in_composer':
         pytest.skip('The CI does not support tpus')
     if notebook_name == 'ffcv_dataloaders' and device == 'cpu':
         pytest.skip('The FFCV notebook requires CUDA')
+    if notebook_name == 'ffcv_dataloaders' and device == 'gpu':
+        pytest.skip('CIFAR10 download is flaky')
     if notebook_name == 'finetune_huggingface':
         pytest.skip(
             "Error that is unreproducible locally: ModuleNotFoundError: No module named 'transformers.models.ernie_m.configuration_ernie_m'"
         )
     if notebook_name == 'pretrain_finetune_huggingface':
         pytest.skip(
             "Error that is unreproducible locally: No module named 'transformers.models.mega.configuration_mega'")
```

### Comparing `composer-0.14.1/tests/test_passes.py` & `composer-0.15.0/tests/test_passes.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/tests/test_precision.py` & `composer-0.15.0/tests/test_precision.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/tests/test_simple_nlp.py` & `composer-0.15.0/tests/test_simple_nlp.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/tests/test_smoketest.py` & `composer-0.15.0/tests/test_smoketest.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/tests/test_split_batch.py` & `composer-0.15.0/tests/test_split_batch.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/tests/test_state.py` & `composer-0.15.0/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `composer-0.14.1/tests/test_time.py` & `composer-0.15.0/tests/test_time.py`

 * *Files identical despite different names*

