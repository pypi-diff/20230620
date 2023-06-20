# Comparing `tmp/vllm-0.0.1.tar.gz` & `tmp/vllm-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vllm-0.0.1.tar", last modified: Mon Jun 19 08:21:03 2023, max compression
+gzip compressed data, was "vllm-0.1.0.tar", last modified: Tue Jun 20 06:21:30 2023, max compression
```

## Comparing `vllm-0.0.1.tar` & `vllm-0.1.0.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 gcpuser   (1005) gcpuser   (1006)        0 2023-06-19 08:21:03.105968 vllm-0.0.1/
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)    11357 2023-06-19 06:53:19.000000 vllm-0.0.1/LICENSE
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)       67 2023-06-19 06:53:19.000000 vllm-0.0.1/MANIFEST.in
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)     3220 2023-06-19 08:21:03.105968 vllm-0.0.1/PKG-INFO
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)     2502 2023-06-19 06:53:19.000000 vllm-0.0.1/README.md
-drwxr-xr-x   0 gcpuser   (1005) gcpuser   (1006)        0 2023-06-19 08:21:03.073965 vllm-0.0.1/csrc/
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)      234 2023-06-19 06:53:19.000000 vllm-0.0.1/csrc/activation.cpp
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)     1359 2023-06-19 06:53:19.000000 vllm-0.0.1/csrc/activation_kernels.cu
-drwxr-xr-x   0 gcpuser   (1005) gcpuser   (1006)        0 2023-06-19 08:21:03.077965 vllm-0.0.1/csrc/attention/
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)      135 2023-06-19 06:53:19.000000 vllm-0.0.1/csrc/attention/attention_dtypes.h
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)     1721 2023-06-19 06:53:19.000000 vllm-0.0.1/csrc/attention/attention_generic.cuh
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)    19900 2023-06-19 06:53:19.000000 vllm-0.0.1/csrc/attention/attention_kernels.cu
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)     1850 2023-06-19 06:53:19.000000 vllm-0.0.1/csrc/attention/attention_utils.cuh
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)    10962 2023-06-19 06:53:19.000000 vllm-0.0.1/csrc/attention/dtype_bfloat16.cuh
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)    10793 2023-06-19 06:53:19.000000 vllm-0.0.1/csrc/attention/dtype_float16.cuh
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)     5559 2023-06-19 06:53:19.000000 vllm-0.0.1/csrc/attention/dtype_float32.cuh
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)      512 2023-06-19 06:53:19.000000 vllm-0.0.1/csrc/attention.cpp
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)     1151 2023-06-19 06:53:19.000000 vllm-0.0.1/csrc/cache.cpp
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)    14699 2023-06-19 06:53:19.000000 vllm-0.0.1/csrc/cache_kernels.cu
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)      292 2023-06-19 06:53:19.000000 vllm-0.0.1/csrc/layernorm.cpp
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)     1904 2023-06-19 06:53:19.000000 vllm-0.0.1/csrc/layernorm_kernels.cu
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)      357 2023-06-19 06:53:19.000000 vllm-0.0.1/csrc/pos_encoding.cpp
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)     2901 2023-06-19 06:53:19.000000 vllm-0.0.1/csrc/pos_encoding_kernels.cu
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)     1592 2023-06-19 06:53:19.000000 vllm-0.0.1/csrc/reduction_utils.cuh
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)      153 2023-06-19 06:53:19.000000 vllm-0.0.1/pyproject.toml
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)      228 2023-06-19 06:53:19.000000 vllm-0.0.1/requirements.txt
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)       38 2023-06-19 08:21:03.105968 vllm-0.0.1/setup.cfg
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)     6082 2023-06-19 07:06:27.000000 vllm-0.0.1/setup.py
-drwxr-xr-x   0 gcpuser   (1005) gcpuser   (1006)        0 2023-06-19 08:21:03.081966 vllm-0.0.1/vllm/
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)      580 2023-06-19 07:08:01.000000 vllm-0.0.1/vllm/__init__.py
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)     1831 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/block.py
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)     8486 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/config.py
-drwxr-xr-x   0 gcpuser   (1005) gcpuser   (1006)        0 2023-06-19 08:21:03.085966 vllm-0.0.1/vllm/core/
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)        0 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/core/__init__.py
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)    10341 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/core/block_manager.py
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)      896 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/core/policy.py
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)    17867 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/core/scheduler.py
-drwxr-xr-x   0 gcpuser   (1005) gcpuser   (1006)        0 2023-06-19 08:21:03.089967 vllm-0.0.1/vllm/engine/
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)        0 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/engine/__init__.py
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)     6546 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/engine/arg_utils.py
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)     8929 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/engine/async_llm_engine.py
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)    13352 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/engine/llm_engine.py
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)     4233 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/engine/ray_utils.py
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)     3579 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/engine/tokenizer_utils.py
-drwxr-xr-x   0 gcpuser   (1005) gcpuser   (1006)        0 2023-06-19 08:21:03.089967 vllm-0.0.1/vllm/entrypoints/
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)        0 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/entrypoints/__init__.py
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)     2970 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/entrypoints/api_server.py
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)     5728 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/entrypoints/llm.py
-drwxr-xr-x   0 gcpuser   (1005) gcpuser   (1006)        0 2023-06-19 08:21:03.089967 vllm-0.0.1/vllm/entrypoints/openai/
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)        0 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/entrypoints/openai/__init__.py
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)    12233 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/entrypoints/openai/api_server.py
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)     3895 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/entrypoints/openai/protocol.py
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)     1577 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/logger.py
-drwxr-xr-x   0 gcpuser   (1005) gcpuser   (1006)        0 2023-06-19 08:21:03.093967 vllm-0.0.1/vllm/model_executor/
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)      247 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/model_executor/__init__.py
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)     2194 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/model_executor/input_metadata.py
-drwxr-xr-x   0 gcpuser   (1005) gcpuser   (1006)        0 2023-06-19 08:21:03.097967 vllm-0.0.1/vllm/model_executor/layers/
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)        0 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/model_executor/layers/__init__.py
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)     1190 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/model_executor/layers/activation.py
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)     9322 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/model_executor/layers/attention.py
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)      773 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/model_executor/layers/layernorm.py
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)    16062 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/model_executor/layers/sampler.py
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)     1836 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/model_executor/model_loader.py
-drwxr-xr-x   0 gcpuser   (1005) gcpuser   (1006)        0 2023-06-19 08:21:03.101968 vllm-0.0.1/vllm/model_executor/models/
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)      358 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/model_executor/models/__init__.py
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)    12118 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/model_executor/models/gpt2.py
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)    10979 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/model_executor/models/gpt_neox.py
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)    11763 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/model_executor/models/llama.py
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)    12958 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/model_executor/models/opt.py
-drwxr-xr-x   0 gcpuser   (1005) gcpuser   (1006)        0 2023-06-19 08:21:03.101968 vllm-0.0.1/vllm/model_executor/parallel_utils/
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)      244 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/model_executor/parallel_utils/__init__.py
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)    22861 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/model_executor/parallel_utils/parallel_state.py
-drwxr-xr-x   0 gcpuser   (1005) gcpuser   (1006)        0 2023-06-19 08:21:03.105968 vllm-0.0.1/vllm/model_executor/parallel_utils/tensor_parallel/
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)     1418 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/model_executor/parallel_utils/tensor_parallel/__init__.py
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)    18207 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/model_executor/parallel_utils/tensor_parallel/layers.py
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)     8586 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/model_executor/parallel_utils/tensor_parallel/mappings.py
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)     6056 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/model_executor/parallel_utils/tensor_parallel/random.py
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)     2460 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/model_executor/parallel_utils/tensor_parallel/utils.py
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)      546 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/model_executor/utils.py
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)     4304 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/model_executor/weight_utils.py
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)     3959 2023-06-19 07:06:34.000000 vllm-0.0.1/vllm/outputs.py
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)     6521 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/sampling_params.py
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)     7767 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/sequence.py
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)      730 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/utils.py
-drwxr-xr-x   0 gcpuser   (1005) gcpuser   (1006)        0 2023-06-19 08:21:03.105968 vllm-0.0.1/vllm/worker/
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)        0 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/worker/__init__.py
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)     5503 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/worker/cache_engine.py
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)    12283 2023-06-19 06:53:19.000000 vllm-0.0.1/vllm/worker/worker.py
-drwxr-xr-x   0 gcpuser   (1005) gcpuser   (1006)        0 2023-06-19 08:21:03.081966 vllm-0.0.1/vllm.egg-info/
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)     3220 2023-06-19 08:21:02.000000 vllm-0.0.1/vllm.egg-info/PKG-INFO
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)     2290 2023-06-19 08:21:03.000000 vllm-0.0.1/vllm.egg-info/SOURCES.txt
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)        1 2023-06-19 08:21:02.000000 vllm-0.0.1/vllm.egg-info/dependency_links.txt
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)      113 2023-06-19 08:21:02.000000 vllm-0.0.1/vllm.egg-info/requires.txt
--rw-r--r--   0 gcpuser   (1005) gcpuser   (1006)        5 2023-06-19 08:21:02.000000 vllm-0.0.1/vllm.egg-info/top_level.txt
+drwxr-xr-x   0 gcpuser   (1004) gcpuser   (1005)        0 2023-06-20 06:21:30.432776 vllm-0.1.0/
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)    11357 2023-05-23 02:52:42.000000 vllm-0.1.0/LICENSE
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)       67 2023-06-06 03:03:42.000000 vllm-0.1.0/MANIFEST.in
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     4975 2023-06-20 06:21:30.432776 vllm-0.1.0/PKG-INFO
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     4257 2023-06-20 06:13:44.000000 vllm-0.1.0/README.md
+drwxr-xr-x   0 gcpuser   (1004) gcpuser   (1005)        0 2023-06-20 06:21:30.412774 vllm-0.1.0/csrc/
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)      234 2023-04-26 10:55:08.000000 vllm-0.1.0/csrc/activation.cpp
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     1359 2023-06-17 10:11:46.000000 vllm-0.1.0/csrc/activation_kernels.cu
+drwxr-xr-x   0 gcpuser   (1004) gcpuser   (1005)        0 2023-06-20 06:21:30.416774 vllm-0.1.0/csrc/attention/
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)      135 2023-06-03 23:33:23.000000 vllm-0.1.0/csrc/attention/attention_dtypes.h
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     1721 2023-06-17 10:11:46.000000 vllm-0.1.0/csrc/attention/attention_generic.cuh
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)    19900 2023-06-17 10:11:46.000000 vllm-0.1.0/csrc/attention/attention_kernels.cu
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     1850 2023-06-17 10:11:46.000000 vllm-0.1.0/csrc/attention/attention_utils.cuh
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)    10962 2023-06-17 10:11:46.000000 vllm-0.1.0/csrc/attention/dtype_bfloat16.cuh
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)    10793 2023-06-17 10:11:46.000000 vllm-0.1.0/csrc/attention/dtype_float16.cuh
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     5559 2023-06-17 10:11:46.000000 vllm-0.1.0/csrc/attention/dtype_float32.cuh
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)      512 2023-04-26 10:55:08.000000 vllm-0.1.0/csrc/attention.cpp
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     1151 2023-04-26 18:32:38.000000 vllm-0.1.0/csrc/cache.cpp
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)    14699 2023-06-17 10:11:46.000000 vllm-0.1.0/csrc/cache_kernels.cu
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)      292 2023-04-26 10:55:08.000000 vllm-0.1.0/csrc/layernorm.cpp
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     1904 2023-06-17 10:11:46.000000 vllm-0.1.0/csrc/layernorm_kernels.cu
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)      357 2023-05-23 02:52:42.000000 vllm-0.1.0/csrc/pos_encoding.cpp
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     2901 2023-06-17 10:11:46.000000 vllm-0.1.0/csrc/pos_encoding_kernels.cu
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     1592 2023-06-17 10:11:46.000000 vllm-0.1.0/csrc/reduction_utils.cuh
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)      153 2023-06-06 03:03:42.000000 vllm-0.1.0/pyproject.toml
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)      228 2023-05-28 17:19:12.000000 vllm-0.1.0/requirements.txt
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)       38 2023-06-20 06:21:30.432776 vllm-0.1.0/setup.cfg
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     6082 2023-06-20 06:13:44.000000 vllm-0.1.0/setup.py
+drwxr-xr-x   0 gcpuser   (1004) gcpuser   (1005)        0 2023-06-20 06:21:30.420775 vllm-0.1.0/vllm/
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)      580 2023-06-20 06:07:35.000000 vllm-0.1.0/vllm/__init__.py
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     1831 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/block.py
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     8486 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/config.py
+drwxr-xr-x   0 gcpuser   (1004) gcpuser   (1005)        0 2023-06-20 06:21:30.420775 vllm-0.1.0/vllm/core/
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)        0 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/core/__init__.py
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)    10341 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/core/block_manager.py
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)      896 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/core/policy.py
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)    17867 2023-06-18 19:39:38.000000 vllm-0.1.0/vllm/core/scheduler.py
+drwxr-xr-x   0 gcpuser   (1004) gcpuser   (1005)        0 2023-06-20 06:21:30.424775 vllm-0.1.0/vllm/engine/
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)        0 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/engine/__init__.py
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     6546 2023-06-18 19:39:38.000000 vllm-0.1.0/vllm/engine/arg_utils.py
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     8929 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/engine/async_llm_engine.py
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)    13352 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/engine/llm_engine.py
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     4233 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/engine/ray_utils.py
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     3788 2023-06-20 06:20:08.000000 vllm-0.1.0/vllm/engine/tokenizer_utils.py
+drwxr-xr-x   0 gcpuser   (1004) gcpuser   (1005)        0 2023-06-20 06:21:30.424775 vllm-0.1.0/vllm/entrypoints/
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)        0 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/entrypoints/__init__.py
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     2970 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/entrypoints/api_server.py
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     5728 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/entrypoints/llm.py
+drwxr-xr-x   0 gcpuser   (1004) gcpuser   (1005)        0 2023-06-20 06:21:30.424775 vllm-0.1.0/vllm/entrypoints/openai/
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)        0 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/entrypoints/openai/__init__.py
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)    12233 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/entrypoints/openai/api_server.py
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     3895 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/entrypoints/openai/protocol.py
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     1577 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/logger.py
+drwxr-xr-x   0 gcpuser   (1004) gcpuser   (1005)        0 2023-06-20 06:21:30.424775 vllm-0.1.0/vllm/model_executor/
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)      247 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/model_executor/__init__.py
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     2194 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/model_executor/input_metadata.py
+drwxr-xr-x   0 gcpuser   (1004) gcpuser   (1005)        0 2023-06-20 06:21:30.428775 vllm-0.1.0/vllm/model_executor/layers/
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)        0 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/model_executor/layers/__init__.py
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     1190 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/model_executor/layers/activation.py
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     9322 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/model_executor/layers/attention.py
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)      773 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/model_executor/layers/layernorm.py
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)    16062 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/model_executor/layers/sampler.py
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     1836 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/model_executor/model_loader.py
+drwxr-xr-x   0 gcpuser   (1004) gcpuser   (1005)        0 2023-06-20 06:21:30.428775 vllm-0.1.0/vllm/model_executor/models/
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)      358 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/model_executor/models/__init__.py
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)    12118 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/model_executor/models/gpt2.py
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)    10979 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/model_executor/models/gpt_neox.py
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)    11763 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/model_executor/models/llama.py
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)    12958 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/model_executor/models/opt.py
+drwxr-xr-x   0 gcpuser   (1004) gcpuser   (1005)        0 2023-06-20 06:21:30.428775 vllm-0.1.0/vllm/model_executor/parallel_utils/
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)      244 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/model_executor/parallel_utils/__init__.py
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)    22861 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/model_executor/parallel_utils/parallel_state.py
+drwxr-xr-x   0 gcpuser   (1004) gcpuser   (1005)        0 2023-06-20 06:21:30.428775 vllm-0.1.0/vllm/model_executor/parallel_utils/tensor_parallel/
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     1418 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/model_executor/parallel_utils/tensor_parallel/__init__.py
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)    18207 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/model_executor/parallel_utils/tensor_parallel/layers.py
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     8586 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/model_executor/parallel_utils/tensor_parallel/mappings.py
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     6056 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/model_executor/parallel_utils/tensor_parallel/random.py
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     2460 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/model_executor/parallel_utils/tensor_parallel/utils.py
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)      546 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/model_executor/utils.py
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     4304 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/model_executor/weight_utils.py
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     3959 2023-06-20 06:13:44.000000 vllm-0.1.0/vllm/outputs.py
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     6521 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/sampling_params.py
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     7767 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/sequence.py
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)      730 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/utils.py
+drwxr-xr-x   0 gcpuser   (1004) gcpuser   (1005)        0 2023-06-20 06:21:30.432776 vllm-0.1.0/vllm/worker/
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)        0 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/worker/__init__.py
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     5503 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/worker/cache_engine.py
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)    12283 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/worker/worker.py
+drwxr-xr-x   0 gcpuser   (1004) gcpuser   (1005)        0 2023-06-20 06:21:30.420775 vllm-0.1.0/vllm.egg-info/
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     4975 2023-06-20 06:21:30.000000 vllm-0.1.0/vllm.egg-info/PKG-INFO
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     2290 2023-06-20 06:21:30.000000 vllm-0.1.0/vllm.egg-info/SOURCES.txt
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)        1 2023-06-20 06:21:30.000000 vllm-0.1.0/vllm.egg-info/dependency_links.txt
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)      113 2023-06-20 06:21:30.000000 vllm-0.1.0/vllm.egg-info/requires.txt
+-rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)        5 2023-06-20 06:21:30.000000 vllm-0.1.0/vllm.egg-info/top_level.txt
```

### Comparing `vllm-0.0.1/LICENSE` & `vllm-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/csrc/activation_kernels.cu` & `vllm-0.1.0/csrc/activation_kernels.cu`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/csrc/attention/attention_generic.cuh` & `vllm-0.1.0/csrc/attention/attention_generic.cuh`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/csrc/attention/attention_kernels.cu` & `vllm-0.1.0/csrc/attention/attention_kernels.cu`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/csrc/attention/attention_utils.cuh` & `vllm-0.1.0/csrc/attention/attention_utils.cuh`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/csrc/attention/dtype_bfloat16.cuh` & `vllm-0.1.0/csrc/attention/dtype_bfloat16.cuh`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/csrc/attention/dtype_float16.cuh` & `vllm-0.1.0/csrc/attention/dtype_float16.cuh`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/csrc/attention/dtype_float32.cuh` & `vllm-0.1.0/csrc/attention/dtype_float32.cuh`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/csrc/attention.cpp` & `vllm-0.1.0/csrc/attention.cpp`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/csrc/cache.cpp` & `vllm-0.1.0/csrc/cache.cpp`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/csrc/cache_kernels.cu` & `vllm-0.1.0/csrc/cache_kernels.cu`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/csrc/layernorm_kernels.cu` & `vllm-0.1.0/csrc/layernorm_kernels.cu`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/csrc/pos_encoding_kernels.cu` & `vllm-0.1.0/csrc/pos_encoding_kernels.cu`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/csrc/reduction_utils.cuh` & `vllm-0.1.0/csrc/reduction_utils.cuh`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/setup.py` & `vllm-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/vllm/__init__.py` & `vllm-0.1.0/vllm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from vllm.engine.async_llm_engine import AsyncLLMEngine
 from vllm.engine.llm_engine import LLMEngine
 from vllm.engine.ray_utils import initialize_cluster
 from vllm.entrypoints.llm import LLM
 from vllm.outputs import CompletionOutput, RequestOutput
 from vllm.sampling_params import SamplingParams
 
-__version__ = "0.0.1"
+__version__ = "0.1.0"
 
 __all__ = [
     "LLM",
     "SamplingParams",
     "RequestOutput",
     "CompletionOutput",
     "LLMEngine",
```

### Comparing `vllm-0.0.1/vllm/block.py` & `vllm-0.1.0/vllm/block.py`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/vllm/config.py` & `vllm-0.1.0/vllm/config.py`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/vllm/core/block_manager.py` & `vllm-0.1.0/vllm/core/block_manager.py`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/vllm/core/policy.py` & `vllm-0.1.0/vllm/core/policy.py`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/vllm/core/scheduler.py` & `vllm-0.1.0/vllm/core/scheduler.py`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/vllm/engine/arg_utils.py` & `vllm-0.1.0/vllm/engine/arg_utils.py`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/vllm/engine/async_llm_engine.py` & `vllm-0.1.0/vllm/engine/async_llm_engine.py`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/vllm/engine/llm_engine.py` & `vllm-0.1.0/vllm/engine/llm_engine.py`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/vllm/engine/ray_utils.py` & `vllm-0.1.0/vllm/engine/ray_utils.py`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/vllm/engine/tokenizer_utils.py` & `vllm-0.1.0/vllm/engine/tokenizer_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,20 @@
 def get_tokenizer(
     model_name: str,
     *args,
     **kwargs,
 ) -> Union[PreTrainedTokenizer, PreTrainedTokenizerFast]:
     """Gets a tokenizer for the given model name via Huggingface."""
     config = AutoConfig.from_pretrained(model_name)
-    if config.model_type == "llama" and getattr(kwargs, "use_fast", True):
+    if "open_llama" in model_name:
+        kwargs["use_fast"] = False
+        logger.info(
+            "OpenLLaMA models do not support the fast tokenizer. "
+            "Using the slow tokenizer instead.")
+    elif config.model_type == "llama" and getattr(kwargs, "use_fast", True):
         # LLaMA fast tokenizer causes protobuf errors in some environments.
         # However, we found that the below LLaMA fast tokenizer works well in
         # most environments.
         model_name = "hf-internal-testing/llama-tokenizer"
         logger.info(
             f"Using the LLaMA fast tokenizer in '{model_name}' to avoid "
             "potential protobuf errors.")
```

### Comparing `vllm-0.0.1/vllm/entrypoints/api_server.py` & `vllm-0.1.0/vllm/entrypoints/api_server.py`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/vllm/entrypoints/llm.py` & `vllm-0.1.0/vllm/entrypoints/llm.py`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/vllm/entrypoints/openai/api_server.py` & `vllm-0.1.0/vllm/entrypoints/openai/api_server.py`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/vllm/entrypoints/openai/protocol.py` & `vllm-0.1.0/vllm/entrypoints/openai/protocol.py`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/vllm/logger.py` & `vllm-0.1.0/vllm/logger.py`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/vllm/model_executor/input_metadata.py` & `vllm-0.1.0/vllm/model_executor/input_metadata.py`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/vllm/model_executor/layers/activation.py` & `vllm-0.1.0/vllm/model_executor/layers/activation.py`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/vllm/model_executor/layers/attention.py` & `vllm-0.1.0/vllm/model_executor/layers/attention.py`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/vllm/model_executor/layers/layernorm.py` & `vllm-0.1.0/vllm/model_executor/layers/layernorm.py`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/vllm/model_executor/layers/sampler.py` & `vllm-0.1.0/vllm/model_executor/layers/sampler.py`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/vllm/model_executor/model_loader.py` & `vllm-0.1.0/vllm/model_executor/model_loader.py`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/vllm/model_executor/models/gpt2.py` & `vllm-0.1.0/vllm/model_executor/models/gpt2.py`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/vllm/model_executor/models/gpt_neox.py` & `vllm-0.1.0/vllm/model_executor/models/gpt_neox.py`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/vllm/model_executor/models/llama.py` & `vllm-0.1.0/vllm/model_executor/models/llama.py`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/vllm/model_executor/models/opt.py` & `vllm-0.1.0/vllm/model_executor/models/opt.py`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/vllm/model_executor/parallel_utils/parallel_state.py` & `vllm-0.1.0/vllm/model_executor/parallel_utils/parallel_state.py`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/vllm/model_executor/parallel_utils/tensor_parallel/__init__.py` & `vllm-0.1.0/vllm/model_executor/parallel_utils/tensor_parallel/__init__.py`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/vllm/model_executor/parallel_utils/tensor_parallel/layers.py` & `vllm-0.1.0/vllm/model_executor/parallel_utils/tensor_parallel/layers.py`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/vllm/model_executor/parallel_utils/tensor_parallel/mappings.py` & `vllm-0.1.0/vllm/model_executor/parallel_utils/tensor_parallel/mappings.py`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/vllm/model_executor/parallel_utils/tensor_parallel/random.py` & `vllm-0.1.0/vllm/model_executor/parallel_utils/tensor_parallel/random.py`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/vllm/model_executor/parallel_utils/tensor_parallel/utils.py` & `vllm-0.1.0/vllm/model_executor/parallel_utils/tensor_parallel/utils.py`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/vllm/model_executor/utils.py` & `vllm-0.1.0/vllm/model_executor/utils.py`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/vllm/model_executor/weight_utils.py` & `vllm-0.1.0/vllm/model_executor/weight_utils.py`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/vllm/outputs.py` & `vllm-0.1.0/vllm/outputs.py`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/vllm/sampling_params.py` & `vllm-0.1.0/vllm/sampling_params.py`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/vllm/sequence.py` & `vllm-0.1.0/vllm/sequence.py`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/vllm/utils.py` & `vllm-0.1.0/vllm/utils.py`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/vllm/worker/cache_engine.py` & `vllm-0.1.0/vllm/worker/cache_engine.py`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/vllm/worker/worker.py` & `vllm-0.1.0/vllm/worker/worker.py`

 * *Files identical despite different names*

### Comparing `vllm-0.0.1/vllm.egg-info/SOURCES.txt` & `vllm-0.1.0/vllm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

