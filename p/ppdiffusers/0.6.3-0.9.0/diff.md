# Comparing `tmp/ppdiffusers-0.6.3.tar.gz` & `tmp/ppdiffusers-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ppdiffusers-0.6.3.tar", last modified: Wed Nov 30 09:37:02 2022, max compression
+gzip compressed data, was "ppdiffusers-0.9.0.tar", last modified: Tue Dec  6 03:35:06 2022, max compression
```

## Comparing `ppdiffusers-0.6.3.tar` & `ppdiffusers-0.9.0.tar`

### file list

```diff
@@ -1,103 +1,224 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 09:37:02.276518 ppdiffusers-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    13335 2022-11-30 09:37:02.276518 ppdiffusers-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    10981 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 09:37:02.252518 ppdiffusers-0.6.3/ppdiffusers/
--rw-r--r--   0 runner    (1001) docker     (122)     3571 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 09:37:02.256518 ppdiffusers-0.6.3/ppdiffusers/commands/
--rw-r--r--   0 runner    (1001) docker     (122)      987 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2342 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/commands/env.py
--rw-r--r--   0 runner    (1001) docker     (122)     1285 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/commands/ppdiffusers_cli.py
--rw-r--r--   0 runner    (1001) docker     (122)    16631 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/configuration_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1404 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/download_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     9052 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/fastdeploy_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    10069 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/initializer.py
--rw-r--r--   0 runner    (1001) docker     (122)     4122 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/modeling_paddle_pytorch_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    21315 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/modeling_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 09:37:02.260518 ppdiffusers-0.6.3/ppdiffusers/models/
--rw-r--r--   0 runner    (1001) docker     (122)      875 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16531 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/models/attention.py
--rw-r--r--   0 runner    (1001) docker     (122)     3917 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/models/ema.py
--rw-r--r--   0 runner    (1001) docker     (122)     3949 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (122)    23521 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (122)    12160 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/models/unet_2d.py
--rw-r--r--   0 runner    (1001) docker     (122)    15746 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/models/unet_2d_condition.py
--rw-r--r--   0 runner    (1001) docker     (122)    57199 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/models/unet_blocks.py
--rw-r--r--   0 runner    (1001) docker     (122)    23010 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/models/vae.py
--rw-r--r--   0 runner    (1001) docker     (122)     7183 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/onnx_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    12435 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/optimization.py
--rw-r--r--   0 runner    (1001) docker     (122)    22461 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/pipeline_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 09:37:02.260518 ppdiffusers-0.6.3/ppdiffusers/pipelines/
--rw-r--r--   0 runner    (1001) docker     (122)     2129 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/pipelines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 09:37:02.260518 ppdiffusers-0.6.3/ppdiffusers/pipelines/ddim/
--rw-r--r--   0 runner    (1001) docker     (122)      726 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/pipelines/ddim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4191 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/pipelines/ddim/pipeline_ddim.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 09:37:02.260518 ppdiffusers-0.6.3/ppdiffusers/pipelines/ddpm/
--rw-r--r--   0 runner    (1001) docker     (122)      726 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/pipelines/ddpm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3856 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/pipelines/ddpm/pipeline_ddpm.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 09:37:02.260518 ppdiffusers-0.6.3/ppdiffusers/pipelines/latent_diffusion/
--rw-r--r--   0 runner    (1001) docker     (122)      926 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/pipelines/latent_diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    26731 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/pipelines/latent_diffusion/pipeline_latent_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (122)     7361 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/pipelines/latent_diffusion/pipeline_latent_diffusion_superresolution.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 09:37:02.260518 ppdiffusers-0.6.3/ppdiffusers/pipelines/latent_diffusion_uncond/
--rw-r--r--   0 runner    (1001) docker     (122)      744 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/pipelines/latent_diffusion_uncond/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4543 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/pipelines/latent_diffusion_uncond/pipeline_latent_diffusion_uncond.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 09:37:02.264518 ppdiffusers-0.6.3/ppdiffusers/pipelines/pndm/
--rw-r--r--   0 runner    (1001) docker     (122)      726 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/pipelines/pndm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3943 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/pipelines/pndm/pipeline_pndm.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 09:37:02.264518 ppdiffusers-0.6.3/ppdiffusers/pipelines/score_sde_ve/
--rw-r--r--   0 runner    (1001) docker     (122)      740 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/pipelines/score_sde_ve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4187 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/pipelines/score_sde_ve/pipeline_score_sde_ve.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 09:37:02.268518 ppdiffusers-0.6.3/ppdiffusers/pipelines/stable_diffusion/
--rw-r--r--   0 runner    (1001) docker     (122)     2881 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/pipelines/stable_diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11392 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/pipelines/stable_diffusion/pipeline_fastdeploy_stable_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (122)    22062 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/pipelines/stable_diffusion/pipeline_fastdeploy_stable_diffusion_img2img.py
--rw-r--r--   0 runner    (1001) docker     (122)    22585 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/pipelines/stable_diffusion/pipeline_fastdeploy_stable_diffusion_inpaint.py
--rw-r--r--   0 runner    (1001) docker     (122)    11078 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/pipelines/stable_diffusion/pipeline_onnx_stable_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (122)    21752 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/pipelines/stable_diffusion/pipeline_onnx_stable_diffusion_img2img.py
--rw-r--r--   0 runner    (1001) docker     (122)    22111 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/pipelines/stable_diffusion/pipeline_onnx_stable_diffusion_inpaint.py
--rw-r--r--   0 runner    (1001) docker     (122)    20323 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (122)    61993 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_all_in_one.py
--rw-r--r--   0 runner    (1001) docker     (122)    22544 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_img2img.py
--rw-r--r--   0 runner    (1001) docker     (122)    23383 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_inpaint.py
--rw-r--r--   0 runner    (1001) docker     (122)    23074 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_inpaint_legacy.py
--rw-r--r--   0 runner    (1001) docker     (122)     6045 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/pipelines/stable_diffusion/safety_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 09:37:02.268518 ppdiffusers-0.6.3/ppdiffusers/pipelines/stochastic_karras_ve/
--rw-r--r--   0 runner    (1001) docker     (122)      746 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/pipelines/stochastic_karras_ve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5613 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/pipelines/stochastic_karras_ve/pipeline_stochastic_karras_ve.py
--rw-r--r--   0 runner    (1001) docker     (122)     2826 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/ppnlp_patch_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 09:37:02.272518 ppdiffusers-0.6.3/ppdiffusers/schedulers/
--rw-r--r--   0 runner    (1001) docker     (122)     1531 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14663 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/schedulers/scheduling_ddim.py
--rw-r--r--   0 runner    (1001) docker     (122)    14151 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/schedulers/scheduling_ddpm.py
--rw-r--r--   0 runner    (1001) docker     (122)    24636 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/schedulers/scheduling_dpmsolver_multistep.py
--rw-r--r--   0 runner    (1001) docker     (122)     9616 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/schedulers/scheduling_euler_ancestral_discrete.py
--rw-r--r--   0 runner    (1001) docker     (122)     9707 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/schedulers/scheduling_karras_ve.py
--rw-r--r--   0 runner    (1001) docker     (122)    12147 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/schedulers/scheduling_lms_discrete.py
--rw-r--r--   0 runner    (1001) docker     (122)    19128 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/schedulers/scheduling_pndm.py
--rw-r--r--   0 runner    (1001) docker     (122)    11774 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/schedulers/scheduling_sde_ve.py
--rw-r--r--   0 runner    (1001) docker     (122)     3391 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/schedulers/scheduling_sde_vp.py
--rw-r--r--   0 runner    (1001) docker     (122)     1349 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/schedulers/scheduling_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5430 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/training_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 09:37:02.276518 ppdiffusers-0.6.3/ppdiffusers/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     1871 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2819 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/utils/deprecation_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2319 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/utils/dummy_paddle_and_paddlenlp_and_fastdeploy_objects.py
--rw-r--r--   0 runner    (1001) docker     (122)     2229 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/utils/dummy_paddle_and_paddlenlp_and_onnx_objects.py
--rw-r--r--   0 runner    (1001) docker     (122)     3304 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/utils/dummy_paddle_and_paddlenlp_objects.py
--rw-r--r--   0 runner    (1001) docker     (122)     1221 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/utils/dummy_paddle_and_scipy_objects.py
--rw-r--r--   0 runner    (1001) docker     (122)     9913 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/utils/dummy_paddle_objects.py
--rw-r--r--   0 runner    (1001) docker     (122)     7623 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/utils/import_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     9577 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (122)     4191 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/utils/outputs.py
--rw-r--r--   0 runner    (1001) docker     (122)    10750 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/ppdiffusers/utils/testing_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)       18 2022-11-30 09:37:01.000000 ppdiffusers-0.6.3/ppdiffusers/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 09:37:02.256518 ppdiffusers-0.6.3/ppdiffusers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    13335 2022-11-30 09:37:02.000000 ppdiffusers-0.6.3/ppdiffusers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3845 2022-11-30 09:37:02.000000 ppdiffusers-0.6.3/ppdiffusers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-30 09:37:02.000000 ppdiffusers-0.6.3/ppdiffusers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2022-11-30 09:37:02.000000 ppdiffusers-0.6.3/ppdiffusers.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       35 2022-11-30 09:37:02.000000 ppdiffusers-0.6.3/ppdiffusers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2022-11-30 09:37:02.000000 ppdiffusers-0.6.3/ppdiffusers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-30 09:37:02.276518 ppdiffusers-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2324 2022-11-30 09:36:12.000000 ppdiffusers-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:35:06.720186 ppdiffusers-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2022-12-06 03:34:08.000000 ppdiffusers-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    37497 2022-12-06 03:35:06.720186 ppdiffusers-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    33087 2022-12-06 03:34:08.000000 ppdiffusers-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:35:06.696184 ppdiffusers-0.9.0/ppdiffusers/
+-rw-r--r--   0 runner    (1001) docker     (122)     4166 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:35:06.700184 ppdiffusers-0.9.0/ppdiffusers/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)      986 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2319 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/commands/env.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1248 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/commands/ppdiffusers_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22552 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/configuration_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1665 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/download_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:35:06.700184 ppdiffusers-0.9.0/ppdiffusers/experimental/
+-rw-r--r--   0 runner    (1001) docker     (122)      724 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:35:06.700184 ppdiffusers-0.9.0/ppdiffusers/experimental/rl/
+-rw-r--r--   0 runner    (1001) docker     (122)      743 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/experimental/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5063 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/experimental/rl/value_guided_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9029 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/fastdeploy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9751 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/initializer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4035 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/modeling_paddle_pytorch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21739 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/modeling_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:35:06.700184 ppdiffusers-0.9.0/ppdiffusers/models/
+-rw-r--r--   0 runner    (1001) docker     (122)      973 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32837 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/models/attention.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3913 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/models/ema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6578 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25703 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10291 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/models/unet_1d.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24919 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/models/unet_1d_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11374 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/models/unet_2d.py
+-rw-r--r--   0 runner    (1001) docker     (122)    60416 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/models/unet_2d_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16811 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/models/unet_2d_condition.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22441 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/models/vae.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11474 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25329 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipeline_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:35:06.700184 ppdiffusers-0.9.0/ppdiffusers/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (122)     2715 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:35:06.700184 ppdiffusers-0.9.0/ppdiffusers/pipelines/alt_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (122)     2006 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/alt_diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5858 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/alt_diffusion/modeling_roberta_series.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26789 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/alt_diffusion/pipeline_alt_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28965 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/alt_diffusion/pipeline_alt_diffusion_img2img.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:35:06.700184 ppdiffusers-0.9.0/ppdiffusers/pipelines/dance_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (122)      747 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/dance_diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5079 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/dance_diffusion/pipeline_dance_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:35:06.700184 ppdiffusers-0.9.0/ppdiffusers/pipelines/ddim/
+-rw-r--r--   0 runner    (1001) docker     (122)      726 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/ddim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4863 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/ddim/pipeline_ddim.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:35:06.700184 ppdiffusers-0.9.0/ppdiffusers/pipelines/ddpm/
+-rw-r--r--   0 runner    (1001) docker     (122)      726 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/ddpm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4732 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/ddpm/pipeline_ddpm.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:35:06.704185 ppdiffusers-0.9.0/ppdiffusers/pipelines/latent_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (122)      922 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/latent_diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29735 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/latent_diffusion/pipeline_latent_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7404 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/latent_diffusion/pipeline_latent_diffusion_superresolution.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:35:06.704185 ppdiffusers-0.9.0/ppdiffusers/pipelines/latent_diffusion_uncond/
+-rw-r--r--   0 runner    (1001) docker     (122)      744 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/latent_diffusion_uncond/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4760 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/latent_diffusion_uncond/pipeline_latent_diffusion_uncond.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:35:06.704185 ppdiffusers-0.9.0/ppdiffusers/pipelines/pndm/
+-rw-r--r--   0 runner    (1001) docker     (122)      726 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/pndm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3995 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/pndm/pipeline_pndm.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:35:06.704185 ppdiffusers-0.9.0/ppdiffusers/pipelines/repaint/
+-rw-r--r--   0 runner    (1001) docker     (122)      731 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/repaint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5649 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/repaint/pipeline_repaint.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:35:06.704185 ppdiffusers-0.9.0/ppdiffusers/pipelines/score_sde_ve/
+-rw-r--r--   0 runner    (1001) docker     (122)      740 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/score_sde_ve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4214 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/score_sde_ve/pipeline_score_sde_ve.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:35:06.704185 ppdiffusers-0.9.0/ppdiffusers/pipelines/stable_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (122)     3376 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/stable_diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32909 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/stable_diffusion/pipeline_cycle_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20648 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/stable_diffusion/pipeline_fastdeploy_stable_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22776 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/stable_diffusion/pipeline_fastdeploy_stable_diffusion_img2img.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24723 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/stable_diffusion/pipeline_fastdeploy_stable_diffusion_inpaint.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24488 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/stable_diffusion/pipeline_fastdeploy_stable_diffusion_inpaint_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8533 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/stable_diffusion/pipeline_fastdeploy_stable_diffusion_mega.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26872 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (122)    61613 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_all_in_one.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22042 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_image_variation.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29892 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_img2img.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35701 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_inpaint.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29152 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_inpaint_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8080 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_mega.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24117 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_upscale.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5645 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/stable_diffusion/safety_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:35:06.704185 ppdiffusers-0.9.0/ppdiffusers/pipelines/stable_diffusion_safe/
+-rw-r--r--   0 runner    (1001) docker     (122)     3123 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/stable_diffusion_safe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36519 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/stable_diffusion_safe/pipeline_stable_diffusion_safe.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5139 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/stable_diffusion_safe/safety_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:35:06.704185 ppdiffusers-0.9.0/ppdiffusers/pipelines/stochastic_karras_ve/
+-rw-r--r--   0 runner    (1001) docker     (122)      746 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/stochastic_karras_ve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5570 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/stochastic_karras_ve/pipeline_stochastic_karras_ve.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:35:06.708185 ppdiffusers-0.9.0/ppdiffusers/pipelines/versatile_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (122)     1479 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/versatile_diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    46545 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/versatile_diffusion/modeling_text_unet.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25064 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/versatile_diffusion/pipeline_versatile_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29016 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/versatile_diffusion/pipeline_versatile_diffusion_dual_guided.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20827 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/versatile_diffusion/pipeline_versatile_diffusion_image_variation.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23217 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/versatile_diffusion/pipeline_versatile_diffusion_text_to_image.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:35:06.708185 ppdiffusers-0.9.0/ppdiffusers/pipelines/vq_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (122)      932 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/vq_diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16660 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/pipelines/vq_diffusion/pipeline_vq_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25263 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/ppnlp_patch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:35:06.708185 ppdiffusers-0.9.0/ppdiffusers/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (122)     1995 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17865 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/schedulers/scheduling_ddim.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16673 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/schedulers/scheduling_ddpm.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25716 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/schedulers/scheduling_dpmsolver_multistep.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10682 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/schedulers/scheduling_euler_ancestral_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10896 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/schedulers/scheduling_euler_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10705 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/schedulers/scheduling_heun_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6559 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/schedulers/scheduling_ipndm.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12647 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/schedulers/scheduling_k_dpm_2_ancestral_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11754 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/schedulers/scheduling_k_dpm_2_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9657 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/schedulers/scheduling_karras_ve.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11289 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/schedulers/scheduling_lms_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19136 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/schedulers/scheduling_pndm.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13523 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/schedulers/scheduling_repaint.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11749 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/schedulers/scheduling_sde_ve.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3290 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/schedulers/scheduling_sde_vp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4952 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/schedulers/scheduling_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23568 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/schedulers/scheduling_vq_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5258 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/training_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:35:06.712185 ppdiffusers-0.9.0/ppdiffusers/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     2345 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2751 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/utils/deprecation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3334 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/utils/dummy_paddle_and_paddlenlp_and_fastdeploy_objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8708 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/utils/dummy_paddle_and_paddlenlp_objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1222 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/utils/dummy_paddle_and_scipy_objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14417 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/utils/dummy_paddle_objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9841 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/utils/import_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9522 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4099 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/utils/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1335 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/utils/pil_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13444 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/ppdiffusers/utils/testing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2022-12-06 03:35:06.000000 ppdiffusers-0.9.0/ppdiffusers/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:35:06.700184 ppdiffusers-0.9.0/ppdiffusers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    37497 2022-12-06 03:35:06.000000 ppdiffusers-0.9.0/ppdiffusers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     8819 2022-12-06 03:35:06.000000 ppdiffusers-0.9.0/ppdiffusers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-06 03:35:06.000000 ppdiffusers-0.9.0/ppdiffusers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2022-12-06 03:35:06.000000 ppdiffusers-0.9.0/ppdiffusers.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2022-12-06 03:35:06.000000 ppdiffusers-0.9.0/ppdiffusers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2022-12-06 03:35:06.000000 ppdiffusers-0.9.0/ppdiffusers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-06 03:35:06.720186 ppdiffusers-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2260 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:35:06.712185 ppdiffusers-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      610 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:35:06.712185 ppdiffusers-0.9.0/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (122)      610 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8499 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/models/test_models_unet_1d.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16181 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/models/test_models_unet_2d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7343 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/models/test_models_vae.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2913 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/models/test_models_vq.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:35:06.712185 ppdiffusers-0.9.0/tests/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (122)      610 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:35:06.712185 ppdiffusers-0.9.0/tests/pipelines/altdiffusion/
+-rw-r--r--   0 runner    (1001) docker     (122)      610 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/altdiffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9913 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/altdiffusion/test_alt_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6958 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/altdiffusion/test_alt_diffusion_img2img.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:35:06.712185 ppdiffusers-0.9.0/tests/pipelines/dance_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (122)      610 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/dance_diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3443 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/dance_diffusion/test_dance_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:35:06.712185 ppdiffusers-0.9.0/tests/pipelines/ddim/
+-rw-r--r--   0 runner    (1001) docker     (122)      610 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/ddim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3745 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/ddim/test_ddim.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:35:06.712185 ppdiffusers-0.9.0/tests/pipelines/ddpm/
+-rw-r--r--   0 runner    (1001) docker     (122)      610 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/ddpm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5083 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/ddpm/test_ddpm.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:35:06.716185 ppdiffusers-0.9.0/tests/pipelines/karras_ve/
+-rw-r--r--   0 runner    (1001) docker     (122)      610 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/karras_ve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3328 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/karras_ve/test_karras_ve.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:35:06.716185 ppdiffusers-0.9.0/tests/pipelines/latent_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (122)      610 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/latent_diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5909 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/latent_diffusion/test_latent_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3975 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/latent_diffusion/test_latent_diffusion_superresolution.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4255 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/latent_diffusion/test_latent_diffusion_uncond.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:35:06.716185 ppdiffusers-0.9.0/tests/pipelines/pndm/
+-rw-r--r--   0 runner    (1001) docker     (122)      610 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/pndm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3353 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/pndm/test_pndm.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:35:06.716185 ppdiffusers-0.9.0/tests/pipelines/repaint/
+-rw-r--r--   0 runner    (1001) docker     (122)      610 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/repaint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2021 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/repaint/test_repaint.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:35:06.716185 ppdiffusers-0.9.0/tests/pipelines/score_sde_ve/
+-rw-r--r--   0 runner    (1001) docker     (122)      610 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/score_sde_ve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3090 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/score_sde_ve/test_score_sde_ve.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:35:06.716185 ppdiffusers-0.9.0/tests/pipelines/stable_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (122)      610 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/stable_diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7808 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/stable_diffusion/test_cycle_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6410 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/stable_diffusion/test_fastdeploy_stable_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4547 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/stable_diffusion/test_fastdeploy_stable_diffusion_img2img.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4643 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/stable_diffusion/test_fastdeploy_stable_diffusion_inpaint.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3255 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/stable_diffusion/test_fastdeploy_stable_diffusion_inpaint_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32703 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/stable_diffusion/test_stable_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12471 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/stable_diffusion/test_stable_diffusion_image_variation.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21039 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/stable_diffusion/test_stable_diffusion_img2img.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20572 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/stable_diffusion/test_stable_diffusion_inpaint.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17202 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/stable_diffusion/test_stable_diffusion_inpaint_legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:35:06.716185 ppdiffusers-0.9.0/tests/pipelines/stable_diffusion_2/
+-rw-r--r--   0 runner    (1001) docker     (122)      610 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/stable_diffusion_2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22171 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/stable_diffusion_2/test_stable_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7040 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/stable_diffusion_2/test_stable_diffusion_inpaint.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6687 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/stable_diffusion_2/test_stable_diffusion_upscale.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12877 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/stable_diffusion_2/test_stable_diffusion_v_pred.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:35:06.716185 ppdiffusers-0.9.0/tests/pipelines/stable_diffusion_safe/
+-rw-r--r--   0 runner    (1001) docker     (122)      610 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/stable_diffusion_safe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14312 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/stable_diffusion_safe/test_safe_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:35:06.720186 ppdiffusers-0.9.0/tests/pipelines/versatile_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (122)      610 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/versatile_diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3884 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/versatile_diffusion/test_versatile_diffusion_dual_guided.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2210 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/versatile_diffusion/test_versatile_diffusion_image_variation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4587 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/versatile_diffusion/test_versatile_diffusion_mega.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3283 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/versatile_diffusion/test_versatile_diffusion_text_to_image.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-06 03:35:06.720186 ppdiffusers-0.9.0/tests/pipelines/vq_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (122)      610 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/vq_diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7927 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/pipelines/vq_diffusion/test_vq_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7376 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/test_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    23275 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/test_layers_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10374 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/test_modeling_common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2957 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/test_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22792 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/test_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (122)      961 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/test_pipelines_common.py
+-rw-r--r--   0 runner    (1001) docker     (122)      983 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/test_pipelines_fastdeploy_common.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    88379 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3247 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/test_training.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6661 2022-12-06 03:34:09.000000 ppdiffusers-0.9.0/tests/test_utils.py
```

### Comparing `ppdiffusers-0.6.3/LICENSE` & `ppdiffusers-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ppdiffusers-0.6.3/ppdiffusers/__init__.py` & `ppdiffusers-0.9.0/ppdiffusers/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,90 +8,121 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+# flake8: noqa
 
 from .ppnlp_patch_utils import *
-
 from .utils import (
+    is_fastdeploy_available,
     is_inflect_available,
     is_onnx_available,
-    is_scipy_available,
     is_paddle_available,
     is_paddlenlp_available,
+    is_scipy_available,
     is_unidecode_available,
-    is_fastdeploy_available,
 )
 from .version import VERSION
 
 __version__ = VERSION
 
 from .configuration_utils import ConfigMixin
-from .onnx_utils import OnnxRuntimeModel
 from .fastdeploy_utils import FastDeployRuntimeModel
 from .utils import logging
 
 if is_paddle_available():
     from .initializer import *
     from .modeling_utils import ModelMixin
-    from .models import AutoencoderKL, UNet2DConditionModel, UNet2DModel, VQModel
+    from .models import (
+        AutoencoderKL,
+        Transformer2DModel,
+        UNet1DModel,
+        UNet2DConditionModel,
+        UNet2DModel,
+        VQModel,
+    )
     from .optimization import (
         get_constant_schedule,
         get_constant_schedule_with_warmup,
         get_cosine_schedule_with_warmup,
         get_cosine_with_hard_restarts_schedule_with_warmup,
         get_linear_schedule_with_warmup,
         get_polynomial_decay_schedule_with_warmup,
         get_scheduler,
     )
     from .pipeline_utils import DiffusionPipeline
-    from .pipelines import DDIMPipeline, DDPMPipeline, KarrasVePipeline, LDMPipeline, LDMSuperResolutionPipeline, PNDMPipeline, ScoreSdeVePipeline
+    from .pipelines import (
+        DanceDiffusionPipeline,
+        DDIMPipeline,
+        DDPMPipeline,
+        KarrasVePipeline,
+        LDMPipeline,
+        LDMSuperResolutionPipeline,
+        PNDMPipeline,
+        RePaintPipeline,
+        ScoreSdeVePipeline,
+    )
     from .schedulers import (
-        EulerAncestralDiscreteScheduler,
         DDIMScheduler,
         DDPMScheduler,
         DPMSolverMultistepScheduler,
+        EulerAncestralDiscreteScheduler,
+        EulerDiscreteScheduler,
+        HeunDiscreteScheduler,
+        IPNDMScheduler,
         KarrasVeScheduler,
+        KDPM2AncestralDiscreteScheduler,
+        KDPM2DiscreteScheduler,
         PNDMScheduler,
+        RePaintScheduler,
         SchedulerMixin,
         ScoreSdeVeScheduler,
+        ScoreSdeVpScheduler,
+        VQDiffusionScheduler,
     )
     from .training_utils import EMAModel
 else:
     from .utils.dummy_paddle_objects import *  # noqa F403
 
 if is_paddle_available() and is_scipy_available():
     from .schedulers import LMSDiscreteScheduler
 else:
     from .utils.dummy_paddle_and_scipy_objects import *  # noqa F403
 
 if is_paddle_available() and is_paddlenlp_available():
-    from .pipelines import (LDMBertModel, LDMTextToImagePipeline,
-                            StableDiffusionImg2ImgPipeline,
-                            StableDiffusionInpaintPipeline,
-                            StableDiffusionInpaintPipelineLegacy,
-                            StableDiffusionPipeline,
-                            StableDiffusionPipelineAllinOne)
-else:
-    from .utils.dummy_paddle_and_paddlenlp_objects import *  # noqa F403
-
-if is_paddle_available() and is_paddlenlp_available() and is_onnx_available():
     from .pipelines import (
-        OnnxStableDiffusionImg2ImgPipeline,
-        OnnxStableDiffusionInpaintPipeline,
-        OnnxStableDiffusionPipeline,
+        AltDiffusionImg2ImgPipeline,
+        AltDiffusionPipeline,
+        CycleDiffusionPipeline,
+        LDMBertModel,
+        LDMTextToImagePipeline,
+        StableDiffusionImageVariationPipeline,
+        StableDiffusionImg2ImgPipeline,
+        StableDiffusionInpaintPipeline,
+        StableDiffusionInpaintPipelineLegacy,
+        StableDiffusionMegaPipeline,
+        StableDiffusionPipeline,
+        StableDiffusionPipelineAllinOne,
+        StableDiffusionPipelineSafe,
+        StableDiffusionUpscalePipeline,
+        VersatileDiffusionDualGuidedPipeline,
+        VersatileDiffusionImageVariationPipeline,
+        VersatileDiffusionPipeline,
+        VersatileDiffusionTextToImagePipeline,
+        VQDiffusionPipeline,
     )
 else:
-    from .utils.dummy_paddle_and_paddlenlp_and_onnx_objects import *  # noqa F403
+    from .utils.dummy_paddle_and_paddlenlp_objects import *  # noqa F403
 
-if is_paddle_available() and is_paddlenlp_available(
-) and is_fastdeploy_available():
+if is_paddle_available() and is_paddlenlp_available() and is_fastdeploy_available():
     from .pipelines import (
         FastDeployStableDiffusionImg2ImgPipeline,
         FastDeployStableDiffusionInpaintPipeline,
+        FastDeployStableDiffusionInpaintPipelineLegacy,
+        FastDeployStableDiffusionMegaPipeline,
         FastDeployStableDiffusionPipeline,
     )
 else:
     from .utils.dummy_paddle_and_paddlenlp_and_fastdeploy_objects import *  # noqa F403
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/commands/__init__.py` & `ppdiffusers-0.9.0/ppdiffusers/commands/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 # limitations under the License.
 
 from abc import ABC, abstractmethod
 from argparse import ArgumentParser
 
 
 class BasePPDiffusersCLICommand(ABC):
-
     @staticmethod
     @abstractmethod
     def register_subcommand(parser: ArgumentParser):
         raise NotImplementedError()
 
     @abstractmethod
     def run(self):
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/commands/env.py` & `ppdiffusers-0.9.0/ppdiffusers/commands/env.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 
 
 def info_command_factory(_):
     return EnvironmentCommand()
 
 
 class EnvironmentCommand(BasePPDiffusersCLICommand):
-
     @staticmethod
     def register_subcommand(parser: ArgumentParser):
         download_parser = parser.add_parser("env")
         download_parser.set_defaults(func=info_command_factory)
 
     def run(self):
 
@@ -54,17 +53,15 @@
             "Python version": platform.python_version(),
             "Paddle version (GPU?)": f"{pd_version} ({pd_cuda_available})",
             "PaddleNLP version": paddlenlp_version,
             "Using GPU in script?": "<fill in>",
             "Using distributed or parallel set-up in script?": "<fill in>",
         }
 
-        print(
-            "\nCopy-and-paste the text below in your GitHub issue and FILL OUT the two last points.\n"
-        )
+        print("\nCopy-and-paste the text below in your GitHub issue and FILL OUT the two last points.\n")
         print(self.format_dict(info))
 
         return info
 
     @staticmethod
     def format_dict(d):
         return "\n".join([f"- {prop}: {val}" for prop, val in d.items()]) + "\n"
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/commands/ppdiffusers_cli.py` & `ppdiffusers-0.9.0/ppdiffusers/commands/ppdiffusers_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,18 +15,16 @@
 
 from argparse import ArgumentParser
 
 from .env import EnvironmentCommand
 
 
 def main():
-    parser = ArgumentParser("PPDiffusers CLI tool",
-                            usage="ppdiffusers-cli <command> [<args>]")
-    commands_parser = parser.add_subparsers(
-        help="ppdiffusers-cli command helpers")
+    parser = ArgumentParser("PPDiffusers CLI tool", usage="ppdiffusers-cli <command> [<args>]")
+    commands_parser = parser.add_subparsers(help="ppdiffusers-cli command helpers")
 
     # Register commands
     EnvironmentCommand.register_subcommand(commands_parser)
 
     # Let's go
     args = parser.parse_args()
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/configuration_utils.py` & `ppdiffusers-0.9.0/ppdiffusers/configuration_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,66 +1,101 @@
 # Copyright (c) 2022 PaddlePaddle Authors. All Rights Reserved.
-# Copyright 2022 The HuggingFace Inc. team.
+# Copyright 2022 The HuggingFace Team. All rights reserved.
 # Copyright (c) 2022, NVIDIA CORPORATION.  All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """ ConfigMixin base class and utilities."""
-import dataclasses
 import functools
+import importlib
 import inspect
 import json
 import os
 import re
 from collections import OrderedDict
 from typing import Any, Dict, Tuple, Union
 
-from .download_utils import ppdiffusers_bos_download
+import numpy as np
 from requests import HTTPError
 
 from . import __version__
-from .utils import PPDIFFUSERS_CACHE, DOWNLOAD_SERVER, logging
+from .download_utils import ppdiffusers_bos_download
+from .utils import DOWNLOAD_SERVER, PPDIFFUSERS_CACHE, DummyObject, deprecate, logging
 
 logger = logging.get_logger(__name__)
 
 _re_configuration_file = re.compile(r"config\.(.*)\.json")
 
 
+class FrozenDict(OrderedDict):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        for key, value in self.items():
+            setattr(self, key, value)
+
+        self.__frozen = True
+
+    def __delitem__(self, *args, **kwargs):
+        raise Exception(f"You cannot use ``__delitem__`` on a {self.__class__.__name__} instance.")
+
+    def setdefault(self, *args, **kwargs):
+        raise Exception(f"You cannot use ``setdefault`` on a {self.__class__.__name__} instance.")
+
+    def pop(self, *args, **kwargs):
+        raise Exception(f"You cannot use ``pop`` on a {self.__class__.__name__} instance.")
+
+    def update(self, *args, **kwargs):
+        raise Exception(f"You cannot use ``update`` on a {self.__class__.__name__} instance.")
+
+    def __setattr__(self, name, value):
+        if hasattr(self, "__frozen") and self.__frozen:
+            raise Exception(f"You cannot use ``__setattr__`` on a {self.__class__.__name__} instance.")
+        super().__setattr__(name, value)
+
+    def __setitem__(self, name, value):
+        if hasattr(self, "__frozen") and self.__frozen:
+            raise Exception(f"You cannot use ``__setattr__`` on a {self.__class__.__name__} instance.")
+        super().__setitem__(name, value)
+
+
 class ConfigMixin:
     r"""
     Base class for all configuration classes. Stores all configuration parameters under `self.config` Also handles all
     methods for loading/downloading/saving classes inheriting from [`ConfigMixin`] with
         - [`~ConfigMixin.from_config`]
         - [`~ConfigMixin.save_config`]
 
     Class attributes:
         - **config_name** (`str`) -- A filename under which the config should stored when calling
           [`~ConfigMixin.save_config`] (should be overridden by parent class).
         - **ignore_for_config** (`List[str]`) -- A list of attributes that should not be saved in the config (should be
-          overridden by parent class).
+          overridden by subclass).
+        - **has_compatibles** (`bool`) -- Whether the class has compatible classes (should be overridden by subclass).
+        - **_deprecated_kwargs** (`List[str]`) -- Keyword arguments that are deprecated. Note that the init function
+          should only have a `kwargs` argument if at least one argument is deprecated (should be overridden by
+          subclass).
     """
     config_name = None
     ignore_for_config = []
+    has_compatibles = False
+    _deprecated_kwargs = []
 
     def register_to_config(self, **kwargs):
         if self.config_name is None:
-            raise NotImplementedError(
-                f"Make sure that {self.__class__} has defined a class name `config_name`"
-            )
-        kwargs["_class_name"] = self.__class__.__name__
-        kwargs["_ppdiffusers_version"] = __version__
+            raise NotImplementedError(f"Make sure that {self.__class__} has defined a class name `config_name`")
 
         # Special case for `kwargs` used in deprecation warning added to schedulers
         # TODO: remove this when we remove the deprecation warning, and the `kwargs` argument,
         # or solve in a more general way.
         kwargs.pop("kwargs", None)
         for key, value in kwargs.items():
             try:
@@ -70,330 +105,394 @@
                 raise err
 
         if not hasattr(self, "_internal_dict"):
             internal_dict = kwargs
         else:
             previous_dict = dict(self._internal_dict)
             internal_dict = {**self._internal_dict, **kwargs}
-            logger.debug(
-                f"Updating config from {previous_dict} to {internal_dict}")
+            logger.debug(f"Updating config from {previous_dict} to {internal_dict}")
 
         self._internal_dict = FrozenDict(internal_dict)
 
-    def save_config(self,
-                    save_directory: Union[str, os.PathLike],
-                    push_to_hub: bool = False,
-                    **kwargs):
+    def save_config(self, save_directory: Union[str, os.PathLike], push_to_hub: bool = False, **kwargs):
         """
         Save a configuration object to the directory `save_directory`, so that it can be re-loaded using the
         [`~ConfigMixin.from_config`] class method.
 
         Args:
             save_directory (`str` or `os.PathLike`):
                 Directory where the configuration JSON file will be saved (will be created if it does not exist).
         """
         if os.path.isfile(save_directory):
-            raise AssertionError(
-                f"Provided path ({save_directory}) should be a directory, not a file"
-            )
+            raise AssertionError(f"Provided path ({save_directory}) should be a directory, not a file")
 
         os.makedirs(save_directory, exist_ok=True)
 
         # If we save using the predefined names, we can load using `from_config`
         output_config_file = os.path.join(save_directory, self.config_name)
 
         self.to_json_file(output_config_file)
-        logger.info(f"ConfigMixinuration saved in {output_config_file}")
+        logger.info(f"Configuration saved in {output_config_file}")
+
+    @classmethod
+    def from_config(cls, config: Union[FrozenDict, Dict[str, Any]] = None, return_unused_kwargs=False, **kwargs):
+        r"""
+        Instantiate a Python class from a config dictionary
+
+        Parameters:
+            config (`Dict[str, Any]`):
+                A config dictionary from which the Python class will be instantiated. Make sure to only load
+                configuration files of compatible classes.
+            return_unused_kwargs (`bool`, *optional*, defaults to `False`):
+                Whether kwargs that are not consumed by the Python class should be returned or not.
+
+            kwargs (remaining dictionary of keyword arguments, *optional*):
+                Can be used to update the configuration object (after it being loaded) and initiate the Python class.
+                `**kwargs` will be directly passed to the underlying scheduler/model's `__init__` method and eventually
+                overwrite same named arguments of `config`.
+
+        Examples:
+
+        ```python
+        >>> from ppdiffusers import DDPMScheduler, DDIMScheduler, PNDMScheduler
+
+        >>> # Download scheduler from BOS and cache.
+        >>> scheduler = DDPMScheduler.from_pretrained("google/ddpm-cifar10-32")
+
+        >>> # Instantiate DDIM scheduler class with same config as DDPM
+        >>> scheduler = DDIMScheduler.from_config(scheduler.config)
+
+        >>> # Instantiate PNDM scheduler class with same config as DDPM
+        >>> scheduler = PNDMScheduler.from_config(scheduler.config)
+        ```
+        """
+        # <===== TO BE REMOVED WITH DEPRECATION
+        # TODO(Patrick) - make sure to remove the following lines when config=="model_path" is deprecated
+        if "pretrained_model_name_or_path" in kwargs:
+            config = kwargs.pop("pretrained_model_name_or_path")
+
+        if config is None:
+            raise ValueError("Please make sure to provide a config as the first positional argument.")
+        # ======>
+
+        if not isinstance(config, dict):
+            deprecation_message = "It is deprecated to pass a pretrained model name or path to `from_config`."
+            if "Scheduler" in cls.__name__:
+                deprecation_message += (
+                    f"If you were trying to load a scheduler, please use {cls}.from_pretrained(...) instead."
+                    " Otherwise, please make sure to pass a configuration dictionary instead. This functionality will"
+                    " be removed in v1.0.0."
+                )
+            elif "Model" in cls.__name__:
+                deprecation_message += (
+                    f"If you were trying to load a model, please use {cls}.load_config(...) followed by"
+                    f" {cls}.from_config(...) instead. Otherwise, please make sure to pass a configuration dictionary"
+                    " instead. This functionality will be removed in v1.0.0."
+                )
+            deprecate("config-passed-as-path", "1.0.0", deprecation_message, standard_warn=False)
+            config, kwargs = cls.load_config(pretrained_model_name_or_path=config, return_unused_kwargs=True, **kwargs)
+
+        init_dict, unused_kwargs, hidden_dict = cls.extract_init_dict(config, **kwargs)
+
+        # Allow dtype to be specified on initialization
+        if "dtype" in unused_kwargs:
+            # (TODO junnyu, donot use dtype)
+            unused_kwargs.pop("dtype")
+            # init_dict["dtype"] = unused_kwargs.pop("dtype")
+
+        # add possible deprecated kwargs
+        for deprecated_kwarg in cls._deprecated_kwargs:
+            if deprecated_kwarg in unused_kwargs:
+                init_dict[deprecated_kwarg] = unused_kwargs.pop(deprecated_kwarg)
+
+        # Return model and optionally state and/or unused_kwargs
+        model = cls(**init_dict)
+
+        # make sure to also save config parameters that might be used for compatible classes
+        model.register_to_config(**hidden_dict)
+
+        # add hidden kwargs of compatible classes to unused_kwargs
+        unused_kwargs = {**unused_kwargs, **hidden_dict}
+
+        if return_unused_kwargs:
+            return (model, unused_kwargs)
+        else:
+            return model
+
+    @classmethod
+    def get_config_dict(cls, *args, **kwargs):
+        deprecation_message = (
+            f" The function get_config_dict is deprecated. Please use {cls}.load_config instead. This function will be"
+            " removed in version v1.0.0"
+        )
+        deprecate("get_config_dict", "1.0.0", deprecation_message, standard_warn=False)
+        return cls.load_config(*args, **kwargs)
 
     @classmethod
-    def from_config(cls,
-                    pretrained_model_name_or_path: Union[str, os.PathLike],
-                    return_unused_kwargs=False,
-                    **kwargs):
+    def load_config(
+        cls, pretrained_model_name_or_path: Union[str, os.PathLike], return_unused_kwargs=False, **kwargs
+    ) -> Tuple[Dict[str, Any], Dict[str, Any]]:
         r"""
-        Instantiate a Python class from a pre-defined JSON-file.
+        Instantiate a Python class from a config dictionary
 
         Parameters:
             pretrained_model_name_or_path (`str` or `os.PathLike`, *optional*):
                 Can be either:
 
                     - A string, the *model id* of a model repo on huggingface.co. Valid model ids should have an
                       organization name, like `google/ddpm-celebahq-256`.
                     - A path to a *directory* containing model weights saved using [`~ConfigMixin.save_config`], e.g.,
                       `./my_model_directory/`.
 
             cache_dir (`Union[str, os.PathLike]`, *optional*):
                 Path to a directory in which a downloaded pretrained model configuration should be cached if the
                 standard cache should not be used.
-            ignore_mismatched_sizes (`bool`, *optional*, defaults to `False`):
-                Whether or not to raise an error if some of the weights from the checkpoint do not have the same size
-                as the weights of the model (if for instance, you are instantiating a model with 10 labels from a
-                checkpoint with 3 labels).
             output_loading_info(`bool`, *optional*, defaults to `False`):
                 Whether or not to also return a dictionary containing missing keys, unexpected keys and error messages.
             subfolder (`str`, *optional*, defaults to `""`):
                 In case the relevant files are located inside a subfolder of the model repo (either remote in
                 huggingface.co or downloaded locally), you can specify the folder name here.
-
-        <Tip>
-
-         It is required to be logged in (`huggingface-cli login`) when you want to use private or [gated
-         models](https://huggingface.co/docs/hub/models-gated#gated-models).
-
-        </Tip>
-
-        <Tip>
-
-        Activate the special ["offline-mode"](https://huggingface.co/transformers/installation.html#offline-mode) to
-        use this method in a firewalled environment.
-
-        </Tip>
-
         """
-        config_dict = cls.get_config_dict(
-            pretrained_model_name_or_path=pretrained_model_name_or_path,
-            **kwargs)
-        init_dict, unused_kwargs = cls.extract_init_dict(config_dict, **kwargs)
-
-        # Allow dtype to be specified on initialization
-        if "dtype" in unused_kwargs:
-            init_dict["dtype"] = unused_kwargs.pop("dtype")
-
-        # Return model and optionally state and/or unused_kwargs
-        model = cls(**init_dict)
-        return_tuple = (model, )
-
-        if return_unused_kwargs:
-            return return_tuple + (unused_kwargs, )
-        else:
-            return return_tuple if len(return_tuple) > 1 else model
-
-    @classmethod
-    def get_config_dict(cls, pretrained_model_name_or_path: Union[str,
-                                                                  os.PathLike],
-                        **kwargs) -> Tuple[Dict[str, Any], Dict[str, Any]]:
+        cache_dir = kwargs.pop("cache_dir", PPDIFFUSERS_CACHE)
         subfolder = kwargs.pop("subfolder", None)
 
         pretrained_model_name_or_path = str(pretrained_model_name_or_path)
 
         if cls.config_name is None:
             raise ValueError(
                 "`self.config_name` is not defined. Note that one should not load a config from "
                 "`ConfigMixin`. Please make sure to define `config_name` in a class inheriting from `ConfigMixin`"
             )
 
         if os.path.isfile(pretrained_model_name_or_path):
             config_file = pretrained_model_name_or_path
         elif os.path.isdir(pretrained_model_name_or_path):
-            if os.path.isfile(
-                    os.path.join(pretrained_model_name_or_path,
-                                 cls.config_name)):
+            if os.path.isfile(os.path.join(pretrained_model_name_or_path, cls.config_name)):
                 # Load from a Paddle checkpoint
-                config_file = os.path.join(pretrained_model_name_or_path,
-                                           cls.config_name)
+                config_file = os.path.join(pretrained_model_name_or_path, cls.config_name)
             elif subfolder is not None and os.path.isfile(
-                    os.path.join(pretrained_model_name_or_path, subfolder,
-                                 cls.config_name)):
-                config_file = os.path.join(pretrained_model_name_or_path,
-                                           subfolder, cls.config_name)
+                os.path.join(pretrained_model_name_or_path, subfolder, cls.config_name)
+            ):
+                config_file = os.path.join(pretrained_model_name_or_path, subfolder, cls.config_name)
             else:
                 raise EnvironmentError(
                     f"Error no file named {cls.config_name} found in directory {pretrained_model_name_or_path}."
                 )
         else:
             try:
                 # Load from URL or cache if already cached
                 config_file = ppdiffusers_bos_download(
                     pretrained_model_name_or_path,
                     filename=cls.config_name,
                     subfolder=subfolder,
+                    cache_dir=cache_dir,
                 )
             except HTTPError as err:
                 raise EnvironmentError(
                     "There was a specific connection error when trying to load"
-                    f" {pretrained_model_name_or_path}:\n{err}")
+                    f" {pretrained_model_name_or_path}:\n{err}"
+                )
             except ValueError:
                 raise EnvironmentError(
                     f"We couldn't connect to '{DOWNLOAD_SERVER}' to load this model, couldn't find it"
                     f" in the cached files and it looks like {pretrained_model_name_or_path} is not the path to a"
                     f" directory containing a {cls.config_name} file.\nCheckout your internet connection or see how to"
                     " run the library in offline mode at"
                     " 'https://huggingface.co/docs/diffusers/installation#offline-mode'."
                 )
             except EnvironmentError:
                 raise EnvironmentError(
                     f"Can't load config for '{pretrained_model_name_or_path}'. If you were trying to load it from "
                     "'https://huggingface.co/models', make sure you don't have a local directory with the same name. "
                     f"Otherwise, make sure '{pretrained_model_name_or_path}' is the correct path to a directory "
-                    f"containing a {cls.config_name} file")
+                    f"containing a {cls.config_name} file"
+                )
 
         try:
             # Load config dict
             config_dict = cls._dict_from_json_file(config_file)
         except (json.JSONDecodeError, UnicodeDecodeError):
-            raise EnvironmentError(
-                f"It looks like the config file at '{config_file}' is not a valid JSON file."
-            )
+            raise EnvironmentError(f"It looks like the config file at '{config_file}' is not a valid JSON file.")
+
+        if return_unused_kwargs:
+            return config_dict, kwargs
 
         return config_dict
 
+    @staticmethod
+    def _get_init_keys(cls):
+        return set(dict(inspect.signature(cls.__init__).parameters).keys())
+
     @classmethod
     def extract_init_dict(cls, config_dict, **kwargs):
-        expected_keys = set(
-            dict(inspect.signature(cls.__init__).parameters).keys())
+        # 0. Copy origin config dict
+        original_dict = {k: v for k, v in config_dict.items()}
+
+        # 1. Retrieve expected config attributes from __init__ signature
+        expected_keys = cls._get_init_keys(cls)
         expected_keys.remove("self")
         # remove general kwargs if present in dict
         if "kwargs" in expected_keys:
             expected_keys.remove("kwargs")
+
+        # 2. Remove attributes that cannot be expected from expected config attributes
         # remove keys to be ignored
         if len(cls.ignore_for_config) > 0:
             expected_keys = expected_keys - set(cls.ignore_for_config)
+
+        # load ppdiffusers library to import compatible and original scheduler
+        ppdiffusers_library = importlib.import_module(__name__.split(".")[0])
+
+        if cls.has_compatibles:
+            compatible_classes = [c for c in cls._get_compatibles() if not isinstance(c, DummyObject)]
+        else:
+            compatible_classes = []
+
+        expected_keys_comp_cls = set()
+        for c in compatible_classes:
+            expected_keys_c = cls._get_init_keys(c)
+            expected_keys_comp_cls = expected_keys_comp_cls.union(expected_keys_c)
+        expected_keys_comp_cls = expected_keys_comp_cls - cls._get_init_keys(cls)
+        config_dict = {k: v for k, v in config_dict.items() if k not in expected_keys_comp_cls}
+
+        # remove attributes from orig class that cannot be expected
+        orig_cls_name = config_dict.pop("_class_name", cls.__name__)
+        if orig_cls_name != cls.__name__ and hasattr(ppdiffusers_library, orig_cls_name):
+            orig_cls = getattr(ppdiffusers_library, orig_cls_name)
+            unexpected_keys_from_orig = cls._get_init_keys(orig_cls) - expected_keys
+            config_dict = {k: v for k, v in config_dict.items() if k not in unexpected_keys_from_orig}
+
+        # remove private attributes
+        config_dict = {k: v for k, v in config_dict.items() if not k.startswith("_")}
+
+        # 3. Create keyword arguments that will be passed to __init__ from expected keyword arguments
         init_dict = {}
         for key in expected_keys:
+            # if config param is passed to kwarg and is present in config dict
+            # it should overwrite existing config dict key
+            if key in kwargs and key in config_dict:
+                config_dict[key] = kwargs.pop(key)
+
             if key in kwargs:
                 # overwrite key
                 init_dict[key] = kwargs.pop(key)
             elif key in config_dict:
                 # use value from config dict
                 init_dict[key] = config_dict.pop(key)
 
-        config_dict = {
-            k: v
-            for k, v in config_dict.items() if not k.startswith("_")
-        }
-
+        # 4. Give nice warning if unexpected values have been passed
         if len(config_dict) > 0:
             logger.warning(
                 f"The config attributes {config_dict} were passed to {cls.__name__}, "
                 "but are not expected and will be ignored. Please verify your "
-                f"{cls.config_name} configuration file.")
-
-        unused_kwargs = {**config_dict, **kwargs}
+                f"{cls.config_name} configuration file."
+            )
 
+        # 5. Give nice info if config attributes are initiliazed to default because they have not been passed
         passed_keys = set(init_dict.keys())
         if len(expected_keys - passed_keys) > 0:
             logger.info(
                 f"{expected_keys - passed_keys} was not found in config. Values will be initialized to default values."
             )
 
-        return init_dict, unused_kwargs
+        # 6. Define unused keyword arguments
+        unused_kwargs = {**config_dict, **kwargs}
+
+        # 7. Define "hidden" config parameters that were saved for compatible classes
+        hidden_config_dict = {k: v for k, v in original_dict.items() if k not in init_dict}
+
+        return init_dict, unused_kwargs, hidden_config_dict
 
     @classmethod
     def _dict_from_json_file(cls, json_file: Union[str, os.PathLike]):
         with open(json_file, "r", encoding="utf-8") as reader:
             text = reader.read()
         return json.loads(text)
 
     def __repr__(self):
         return f"{self.__class__.__name__} {self.to_json_string()}"
 
     @property
     def config(self) -> Dict[str, Any]:
+        """
+        Returns the config of the class as a frozen dictionary
+
+        Returns:
+            `Dict[str, Any]`: Config of the class.
+        """
         return self._internal_dict
 
     def to_json_string(self) -> str:
         """
         Serializes this instance to a JSON string.
 
         Returns:
             `str`: String containing all the attributes that make up this configuration instance in JSON format.
         """
-        config_dict = self._internal_dict if hasattr(self,
-                                                     "_internal_dict") else {}
+        config_dict = self._internal_dict if hasattr(self, "_internal_dict") else {}
+        config_dict["_class_name"] = self.__class__.__name__
+        config_dict["_ppdiffusers_version"] = __version__
+
+        def to_json_saveable(value):
+            if isinstance(value, np.ndarray):
+                value = value.tolist()
+            return value
+
+        config_dict = {k: to_json_saveable(v) for k, v in config_dict.items()}
         return json.dumps(config_dict, indent=2, sort_keys=True) + "\n"
 
     def to_json_file(self, json_file_path: Union[str, os.PathLike]):
         """
         Save this instance to a JSON file.
 
         Args:
             json_file_path (`str` or `os.PathLike`):
                 Path to the JSON file in which this configuration instance's parameters will be saved.
         """
         with open(json_file_path, "w", encoding="utf-8") as writer:
             writer.write(self.to_json_string())
 
 
-class FrozenDict(OrderedDict):
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-        for key, value in self.items():
-            setattr(self, key, value)
-
-        self.__frozen = True
-
-    def __delitem__(self, *args, **kwargs):
-        raise Exception(
-            f"You cannot use ``__delitem__`` on a {self.__class__.__name__} instance."
-        )
-
-    def setdefault(self, *args, **kwargs):
-        raise Exception(
-            f"You cannot use ``setdefault`` on a {self.__class__.__name__} instance."
-        )
-
-    def pop(self, *args, **kwargs):
-        raise Exception(
-            f"You cannot use ``pop`` on a {self.__class__.__name__} instance.")
-
-    def update(self, *args, **kwargs):
-        raise Exception(
-            f"You cannot use ``update`` on a {self.__class__.__name__} instance."
-        )
-
-    def __setattr__(self, name, value):
-        if hasattr(self, "__frozen") and self.__frozen:
-            raise Exception(
-                f"You cannot use ``__setattr__`` on a {self.__class__.__name__} instance."
-            )
-        super().__setattr__(name, value)
-
-    def __setitem__(self, name, value):
-        if hasattr(self, "__frozen") and self.__frozen:
-            raise Exception(
-                f"You cannot use ``__setattr__`` on a {self.__class__.__name__} instance."
-            )
-        super().__setitem__(name, value)
-
-
 def register_to_config(init):
     r"""
     Decorator to apply on the init of classes inheriting from [`ConfigMixin`] so that all the arguments are
     automatically sent to `self.register_for_config`. To ignore a specific argument accepted by the init but that
     shouldn't be registered in the config, use the `ignore_for_config` class variable
 
     Warning: Once decorated, all private arguments (beginning with an underscore) are trashed and not sent to the init!
     """
 
     @functools.wraps(init)
     def inner_init(self, *args, **kwargs):
         # Ignore private kwargs in the init.
         init_kwargs = {k: v for k, v in kwargs.items() if not k.startswith("_")}
-        init(self, *args, **init_kwargs)
+        config_init_kwargs = {k: v for k, v in kwargs.items() if k.startswith("_")}
+
         if not isinstance(self, ConfigMixin):
             raise RuntimeError(
                 f"`@register_for_config` was applied to {self.__class__.__name__} init method, but this class does "
-                "not inherit from `ConfigMixin`.")
+                "not inherit from `ConfigMixin`."
+            )
 
         ignore = getattr(self, "ignore_for_config", [])
         # Get positional arguments aligned with kwargs
         new_kwargs = {}
         signature = inspect.signature(init)
         parameters = {
-            name: p.default
-            for i, (name, p) in enumerate(signature.parameters.items())
-            if i > 0 and name not in ignore
+            name: p.default for i, (name, p) in enumerate(signature.parameters.items()) if i > 0 and name not in ignore
         }
         for arg, name in zip(args, parameters.keys()):
             new_kwargs[name] = arg
 
         # Then add all kwargs
-        new_kwargs.update({
-            k: init_kwargs.get(k, default)
-            for k, default in parameters.items()
-            if k not in ignore and k not in new_kwargs
-        })
+        new_kwargs.update(
+            {
+                k: init_kwargs.get(k, default)
+                for k, default in parameters.items()
+                if k not in ignore and k not in new_kwargs
+            }
+        )
+        new_kwargs = {**config_init_kwargs, **new_kwargs}
         getattr(self, "register_to_config")(**new_kwargs)
+        init(self, *args, **init_kwargs)
 
     return inner_init
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/fastdeploy_utils.py` & `ppdiffusers-0.9.0/ppdiffusers/fastdeploy_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,75 +18,76 @@
 import shutil
 from pathlib import Path
 from typing import Optional, Union
 
 import numpy as np
 
 from .download_utils import ppdiffusers_bos_download
-
-from .utils import FASTDEPLOY_WEIGHTS_NAME, FASTDEPLOY_MODEL_NAME, is_fastdeploy_available, logging
+from .utils import (
+    FASTDEPLOY_MODEL_NAME,
+    FASTDEPLOY_WEIGHTS_NAME,
+    is_fastdeploy_available,
+    logging,
+)
 
 if is_fastdeploy_available():
     import fastdeploy as fd
 
 logger = logging.get_logger(__name__)
 
 
 class FastDeployRuntimeModel:
-
     def __init__(self, model=None, **kwargs):
-        logger.info(
-            "`ppdiffusers.FastDeployRuntimeModel` is experimental and might change in the future."
-        )
+        logger.info("`ppdiffusers.FastDeployRuntimeModel` is experimental and might change in the future.")
         self.model = model
         self.model_save_dir = kwargs.get("model_save_dir", None)
-        self.latest_model_name = kwargs.get("latest_model_name",
-                                            "inference.pdmodel")
-        self.latest_params_name = kwargs.get("latest_params_name",
-                                             "inference.pdiparams")
+        self.latest_model_name = kwargs.get("latest_model_name", "inference.pdmodel")
+        self.latest_params_name = kwargs.get("latest_params_name", "inference.pdiparams")
 
     def __call__(self, **kwargs):
         inputs = {k: np.array(v) for k, v in kwargs.items()}
         return self.model.infer(inputs)
 
     @staticmethod
-    def load_model(model_path: Union[str, Path],
-                   params_path: Union[str, Path],
-                   runtime_option=None):
+    def load_model(
+        model_path: Union[str, Path],
+        params_path: Union[str, Path],
+        runtime_options: Optional["fd.RuntimeOption"] = None,
+    ):
         """
         Loads an FastDeploy Inference Model with fastdeploy.RuntimeOption
 
         Arguments:
             model_path (`str` or `Path`):
                 Model path from which to load
             params_path (`str` or `Path`):
                 Params path from which to load
-            runtime_option(fd.RuntimeOption, *optional*):
+            runtime_options (fd.RuntimeOption, *optional*):
                 The RuntimeOption of fastdeploy to initialize the fastdeploy runtime. Default setting
                 the device to cpu and the backend to paddle inference
         """
-        option = runtime_option
-        if option is None or not isinstance(runtime_option, fd.RuntimeOption):
-            logger.info(
-                "No fastdeploy.RuntimeOption specified, using CPU device and paddle inference backend."
-            )
+        option = runtime_options
+        if option is None or not isinstance(runtime_options, fd.RuntimeOption):
+            logger.info("No fastdeploy.RuntimeOption specified, using CPU device and paddle inference backend.")
             option = fd.RuntimeOption()
             option.use_paddle_backend()
             option.use_cpu()
         option.set_model_path(model_path, params_path)
         return fd.Runtime(option)
 
-    def _save_pretrained(self,
-                         save_directory: Union[str, Path],
-                         model_file_name: Optional[str] = None,
-                         params_file_name: Optional[str] = None,
-                         **kwargs):
+    def _save_pretrained(
+        self,
+        save_directory: Union[str, Path],
+        model_file_name: Optional[str] = None,
+        params_file_name: Optional[str] = None,
+        **kwargs
+    ):
         """
         Save a model and its configuration file to a directory, so that it can be re-loaded using the
-        [`~optimum.onnxruntime.modeling_ort.ORTModel.from_pretrained`] class method. It will always save the
+        [`~FastDeployRuntimeModel.from_pretrained`] class method. It will always save the
         latest_model_name.
 
         Arguments:
             save_directory (`str` or `Path`):
                 Directory where to save the model file.
             model_file_name(`str`, *optional*):
                 Overwrites the default model file name from `"inference.pdmodel"` to `model_file_name`. This allows you to save the
@@ -112,105 +113,103 @@
 
     def save_pretrained(
         self,
         save_directory: Union[str, os.PathLike],
         **kwargs,
     ):
         """
-        Save a model to a directory, so that it can be re-loaded using the [`~OnnxModel.from_pretrained`] class
+        Save a model to a directory, so that it can be re-loaded using the [`~FastDeployRuntimeModel.from_pretrained`] class
         method.:
 
         Arguments:
             save_directory (`str` or `os.PathLike`):
                 Directory to which to save. Will be created if it doesn't exist.
         """
         if os.path.isfile(save_directory):
-            logger.error(
-                f"Provided path ({save_directory}) should be a directory, not a file"
-            )
+            logger.error(f"Provided path ({save_directory}) should be a directory, not a file")
             return
 
         os.makedirs(save_directory, exist_ok=True)
 
         # saving model weights/files
         self._save_pretrained(save_directory, **kwargs)
 
     @classmethod
     def _from_pretrained(
         cls,
         pretrained_model_name_or_path: Union[str, Path],
         cache_dir: Optional[str] = None,
         model_file_name: Optional[str] = None,
         params_file_name: Optional[str] = None,
-        runtime_option: Optional["fastdeploy.RuntimeOption"] = None,
+        runtime_options: Optional["fd.RuntimeOption"] = None,
         **kwargs,
     ):
         """
-        Load a model from a directory or the HF Hub.
+        Load a model from a directory or the BOS.
 
         Arguments:
             pretrained_model_name_or_path (`str` or `Path`):
                 Directory from which to load
             cache_dir (`Union[str, Path]`, *optional*):
                 Path to a directory in which a downloaded pretrained model configuration should be cached if the
                 standard cache should not be used.
-            model_file_name(`str`):
+            model_file_name (`str`):
                 Overwrites the default model file name from `"inference.pdmodel"` to `file_name`. This allows you to load
                 different model files from the same repository or directory.
-            params_file_name(`str`):
+            params_file_name (`str`):
                 Overwrites the default params file name from `"inference.pdiparams"` to `file_name`. This allows you to load
                 different model files from the same repository or directory.
-            runtime_option(`fastdeploy.RuntimeOption`, *optional*):
+            runtime_options (`fastdeploy.RuntimeOption`, *optional*):
                 The RuntimeOption of fastdeploy.
             kwargs (`Dict`, *optional*):
                 kwargs will be passed to the model during initialization
         """
         model_file_name = model_file_name if model_file_name is not None else FASTDEPLOY_MODEL_NAME
         params_file_name = params_file_name if params_file_name is not None else FASTDEPLOY_WEIGHTS_NAME
         # load model from local directory
         if os.path.isdir(pretrained_model_name_or_path):
             model = FastDeployRuntimeModel.load_model(
                 os.path.join(pretrained_model_name_or_path, model_file_name),
                 os.path.join(pretrained_model_name_or_path, params_file_name),
-                runtime_option=runtime_option,
+                runtime_options=runtime_options,
             )
             kwargs["model_save_dir"] = Path(pretrained_model_name_or_path)
         # load model from hub
         else:
             # download model
             model_cache_path = ppdiffusers_bos_download(
                 pretrained_model_name_or_path=pretrained_model_name_or_path,
                 filename=model_file_name,
+                cache_dir=cache_dir,
             )
             # download params
             params_cache_path = ppdiffusers_bos_download(
                 pretrained_model_name_or_path=pretrained_model_name_or_path,
                 filename=params_file_name,
+                cache_dir=cache_dir,
             )
             kwargs["model_save_dir"] = Path(model_cache_path).parent
             kwargs["latest_model_name"] = Path(model_cache_path).name
             kwargs["latest_params_name"] = Path(params_cache_path).name
             model = FastDeployRuntimeModel.load_model(
-                model_cache_path,
-                params_cache_path,
-                runtime_option=runtime_option)
+                model_cache_path, params_cache_path, runtime_options=runtime_options
+            )
         return cls(model=model, **kwargs)
 
     @classmethod
     def from_pretrained(
         cls,
-        model_id: Union[str, Path],
-        force_download: bool = True,
-        use_auth_token: Optional[str] = None,
+        pretrained_model_name_or_path: Union[str, Path],
+        cache_dir: Optional[str] = None,
+        model_file_name: Optional[str] = None,
+        params_file_name: Optional[str] = None,
+        runtime_options: Optional["fd.RuntimeOption"] = None,
         **model_kwargs,
     ):
-        revision = None
-        if len(str(model_id).split("@")) == 2:
-            model_id, revision = model_id.split("@")
-
         return cls._from_pretrained(
-            model_id=model_id,
-            revision=revision,
-            force_download=force_download,
-            use_auth_token=use_auth_token,
+            pretrained_model_name_or_path=pretrained_model_name_or_path,
+            cache_dir=cache_dir,
+            model_file_name=model_file_name,
+            params_file_name=params_file_name,
+            runtime_options=runtime_options,
             **model_kwargs,
         )
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/initializer.py` & `ppdiffusers-0.9.0/ppdiffusers/initializer.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,56 +7,55 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
 """
 This code is based on https://github.com/pytorch/pytorch/blob/master/torch/nn/init.py
 Ths copyright of pytorch/pytorch is a BSD-style license, as found in the LICENSE file.
 """
 
 import math
-import numpy as np
 
+import numpy as np
 import paddle
 import paddle.nn as nn
 
 __all__ = [
-    'uniform_',
-    'normal_',
-    'constant_',
-    'ones_',
-    'zeros_',
-    'xavier_uniform_',
-    'xavier_normal_',
-    'kaiming_uniform_',
-    'kaiming_normal_',
-    'linear_init_',
-    'conv_init_',
-    'reset_initialized_parameter',
+    "uniform_",
+    "normal_",
+    "constant_",
+    "ones_",
+    "zeros_",
+    "xavier_uniform_",
+    "xavier_normal_",
+    "kaiming_uniform_",
+    "kaiming_normal_",
+    "linear_init_",
+    "conv_init_",
+    "reset_initialized_parameter",
 ]
 
 
 def _no_grad_uniform_(tensor, a, b):
     with paddle.no_grad():
-        tensor.set_value(
-            paddle.uniform(shape=tensor.shape, dtype=tensor.dtype, min=a,
-                           max=b))
+        tensor.set_value(paddle.uniform(shape=tensor.shape, dtype=tensor.dtype, min=a, max=b))
     return tensor
 
 
-def _no_grad_normal_(tensor, mean=0., std=1.):
+def _no_grad_normal_(tensor, mean=0.0, std=1.0):
     with paddle.no_grad():
         tensor.set_value(paddle.normal(mean=mean, std=std, shape=tensor.shape))
     return tensor
 
 
-def _no_grad_fill_(tensor, value=0.):
+def _no_grad_fill_(tensor, value=0.0):
     with paddle.no_grad():
         tensor.set_value(paddle.full_like(tensor, value, dtype=tensor.dtype))
     return tensor
 
 
 def uniform_(tensor, a, b):
     """
@@ -67,28 +66,28 @@
         b (float|int): max value.
     Return:
         tensor
     """
     return _no_grad_uniform_(tensor, a, b)
 
 
-def normal_(tensor, mean=0., std=1.):
+def normal_(tensor, mean=0.0, std=1.0):
     """
     Modified tensor inspace using normal_
     Args:
         tensor (paddle.Tensor): paddle Tensor
         mean (float|int): mean value.
         std (float|int): std value.
     Return:
         tensor
     """
     return _no_grad_normal_(tensor, mean, std)
 
 
-def constant_(tensor, value=0.):
+def constant_(tensor, value=0.0):
     """
     Modified tensor inspace using constant_
     Args:
         tensor (paddle.Tensor): paddle Tensor
         value (float|int): value to fill tensor.
     Return:
         tensor
@@ -130,17 +129,15 @@
     Args:
         tensor (Tensor): paddle.Tensor
         reverse (bool: False): tensor data format order, False by default as [fout, fin, ...]. e.g. : conv.weight [cout, cin, kh, kw] is False; linear.weight [cin, cout] is True
     Return:
         Tuple[fan_in, fan_out]
     """
     if tensor.ndim < 2:
-        raise ValueError(
-            "Fan in and fan out can not be computed for tensor with fewer than 2 dimensions"
-        )
+        raise ValueError("Fan in and fan out can not be computed for tensor with fewer than 2 dimensions")
 
     if reverse:
         num_input_fmaps, num_output_fmaps = tensor.shape[0], tensor.shape[1]
     else:
         num_input_fmaps, num_output_fmaps = tensor.shape[1], tensor.shape[0]
 
     receptive_field_size = 1
@@ -149,15 +146,15 @@
 
     fan_in = num_input_fmaps * receptive_field_size
     fan_out = num_output_fmaps * receptive_field_size
 
     return fan_in, fan_out
 
 
-def xavier_uniform_(tensor, gain=1., reverse=False):
+def xavier_uniform_(tensor, gain=1.0, reverse=False):
     """
     Modified tensor inspace using xavier_uniform_
     Args:
         tensor (paddle.Tensor): paddle Tensor
         gain (float): super parameter, 1. default.
         reverse (bool):  reverse (bool: False): tensor data format order, False by default as [fout, fin, ...].
     Return:
@@ -165,15 +162,15 @@
     """
     fan_in, fan_out = _calculate_fan_in_and_fan_out(tensor, reverse=reverse)
     std = gain * math.sqrt(2.0 / float(fan_in + fan_out))
     k = math.sqrt(3.0) * std
     return _no_grad_uniform_(tensor, -k, k)
 
 
-def xavier_normal_(tensor, gain=1., reverse=False):
+def xavier_normal_(tensor, gain=1.0, reverse=False):
     """
     Modified tensor inspace using xavier_normal_
     Args:
         tensor (paddle.Tensor): paddle Tensor
         gain (float): super parameter, 1. default.
         reverse (bool):  reverse (bool: False): tensor data format order, False by default as [fout, fin, ...].
     Return:
@@ -183,57 +180,47 @@
     std = gain * math.sqrt(2.0 / float(fan_in + fan_out))
     return _no_grad_normal_(tensor, 0, std)
 
 
 # reference: https://pytorch.org/docs/stable/_modules/torch/nn/init.html
 def _calculate_correct_fan(tensor, mode, reverse=False):
     mode = mode.lower()
-    valid_modes = ['fan_in', 'fan_out']
+    valid_modes = ["fan_in", "fan_out"]
     if mode not in valid_modes:
-        raise ValueError("Mode {} not supported, please use one of {}".format(
-            mode, valid_modes))
+        raise ValueError("Mode {} not supported, please use one of {}".format(mode, valid_modes))
 
     fan_in, fan_out = _calculate_fan_in_and_fan_out(tensor, reverse)
 
-    return fan_in if mode == 'fan_in' else fan_out
+    return fan_in if mode == "fan_in" else fan_out
 
 
 def _calculate_gain(nonlinearity, param=None):
-    linear_fns = [
-        'linear', 'conv1d', 'conv2d', 'conv3d', 'conv_transpose1d',
-        'conv_transpose2d', 'conv_transpose3d'
-    ]
-    if nonlinearity in linear_fns or nonlinearity == 'sigmoid':
+    linear_fns = ["linear", "conv1d", "conv2d", "conv3d", "conv_transpose1d", "conv_transpose2d", "conv_transpose3d"]
+    if nonlinearity in linear_fns or nonlinearity == "sigmoid":
         return 1
-    elif nonlinearity == 'tanh':
+    elif nonlinearity == "tanh":
         return 5.0 / 3
-    elif nonlinearity == 'relu':
+    elif nonlinearity == "relu":
         return math.sqrt(2.0)
-    elif nonlinearity == 'leaky_relu':
+    elif nonlinearity == "leaky_relu":
         if param is None:
             negative_slope = 0.01
-        elif not isinstance(param, bool) and isinstance(
-                param, int) or isinstance(param, float):
+        elif not isinstance(param, bool) and isinstance(param, int) or isinstance(param, float):
             # True/False are instances of int, hence check above
             negative_slope = param
         else:
-            raise ValueError(
-                "negative_slope {} not a valid number".format(param))
+            raise ValueError("negative_slope {} not a valid number".format(param))
         return math.sqrt(2.0 / (1 + negative_slope**2))
-    elif nonlinearity == 'selu':
+    elif nonlinearity == "selu":
         return 3.0 / 4
     else:
         raise ValueError("Unsupported nonlinearity {}".format(nonlinearity))
 
 
-def kaiming_uniform_(tensor,
-                     a=0,
-                     mode='fan_in',
-                     nonlinearity='leaky_relu',
-                     reverse=False):
+def kaiming_uniform_(tensor, a=0, mode="fan_in", nonlinearity="leaky_relu", reverse=False):
     """
     Modified tensor inspace using kaiming_uniform method
     Args:
         tensor (paddle.Tensor): paddle Tensor
         mode (str): ['fan_in', 'fan_out'], 'fin_in' defalut
         nonlinearity (str): nonlinearity method name
         reverse (bool):  reverse (bool: False): tensor data format order, False by default as [fout, fin, ...].
@@ -243,19 +230,15 @@
     fan = _calculate_correct_fan(tensor, mode, reverse)
     gain = _calculate_gain(nonlinearity, a)
     std = gain / math.sqrt(fan)
     k = math.sqrt(3.0) * std
     return _no_grad_uniform_(tensor, -k, k)
 
 
-def kaiming_normal_(tensor,
-                    a=0,
-                    mode='fan_in',
-                    nonlinearity='leaky_relu',
-                    reverse=False):
+def kaiming_normal_(tensor, a=0, mode="fan_in", nonlinearity="leaky_relu", reverse=False):
     """
     Modified tensor inspace using kaiming_normal_
     Args:
         tensor (paddle.Tensor): paddle Tensor
         mode (str): ['fan_in', 'fan_out'], 'fin_in' defalut
         nonlinearity (str): nonlinearity method name
         reverse (bool):  reverse (bool: False): tensor data format order, False by default as [fout, fin, ...].
@@ -295,27 +278,26 @@
         model (paddle.Layer): paddle Layer
         include_self (bool: False): include_self for Layer.named_sublayers method. Indicate whether including itself
     Return:
         None
     """
     for _, m in model.named_sublayers(include_self=include_self):
         if isinstance(m, nn.Conv2D):
-            k = float(m._groups) / (m._in_channels * m._kernel_size[0] *
-                                    m._kernel_size[1])
+            k = float(m._groups) / (m._in_channels * m._kernel_size[0] * m._kernel_size[1])
             k = math.sqrt(k)
             _no_grad_uniform_(m.weight, -k, k)
-            if hasattr(m, 'bias') and getattr(m, 'bias') is not None:
+            if hasattr(m, "bias") and getattr(m, "bias") is not None:
                 _no_grad_uniform_(m.bias, -k, k)
 
         elif isinstance(m, nn.Linear):
-            k = math.sqrt(1. / m.weight.shape[0])
+            k = math.sqrt(1.0 / m.weight.shape[0])
             _no_grad_uniform_(m.weight, -k, k)
-            if hasattr(m, 'bias') and getattr(m, 'bias') is not None:
+            if hasattr(m, "bias") and getattr(m, "bias") is not None:
                 _no_grad_uniform_(m.bias, -k, k)
 
         elif isinstance(m, nn.Embedding):
-            _no_grad_normal_(m.weight, mean=0., std=1.)
+            _no_grad_normal_(m.weight, mean=0.0, std=1.0)
 
         elif isinstance(m, (nn.BatchNorm2D, nn.LayerNorm)):
-            _no_grad_fill_(m.weight, 1.)
-            if hasattr(m, 'bias') and getattr(m, 'bias') is not None:
+            _no_grad_fill_(m.weight, 1.0)
+            if hasattr(m, "bias") and getattr(m, "bias") is not None:
                 _no_grad_fill_(m.bias, 0)
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/modeling_paddle_pytorch_utils.py` & `ppdiffusers-0.9.0/ppdiffusers/modeling_paddle_pytorch_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # Copyright (c) 2022 PaddlePaddle Authors. All Rights Reserved.
-# Copyright 2022 The HuggingFace Inc. team.
+# Copyright 2022 The HuggingFace Team. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """ PyTorch - Paddle general utilities."""
 import re
+
 from .utils import logging
 
 logger = logging.get_logger(__name__)
 
 
 def rename_key(key):
     regex = r"\w+[.]\d+"
@@ -28,55 +29,53 @@
 
 
 #####################
 # PyTorch => Paddle #
 #####################
 
 
-def rename_key_and_reshape_tensor(pt_tuple_key, pt_tensor,
-                                  random_paddle_state_dict):
+def rename_key_and_reshape_tensor(pt_tuple_key, pt_tensor, random_paddle_state_dict):
     """Rename PT weight names to corresponding Paddle weight names and reshape tensor if necessary"""
 
     # conv norm or layer norm
-    renamed_pt_tuple_key = pt_tuple_key[:-1] + ("bias", )
-    if (any("norm" in str_ for str_ in pt_tuple_key)
-            and (pt_tuple_key[-1] in ["bias", "beta"])
-            and (pt_tuple_key[:-1] + ("bias", ) in random_paddle_state_dict)):
-        renamed_pt_tuple_key = pt_tuple_key[:-1] + ("bias", )
-        return renamed_pt_tuple_key, pt_tensor
-    elif pt_tuple_key[-1] in [
-            "weight", "gamma"
-    ] and pt_tuple_key[:-1] + ("bias", ) in random_paddle_state_dict:
-        renamed_pt_tuple_key = pt_tuple_key[:-1] + ("bias", )
+    renamed_pt_tuple_key = pt_tuple_key[:-1] + ("bias",)
+    if (
+        any("norm" in str_ for str_ in pt_tuple_key)
+        and (pt_tuple_key[-1] in ["bias", "beta"])
+        and (pt_tuple_key[:-1] + ("bias",) in random_paddle_state_dict)
+    ):
+        renamed_pt_tuple_key = pt_tuple_key[:-1] + ("bias",)
+        return renamed_pt_tuple_key, pt_tensor
+    elif pt_tuple_key[-1] in ["weight", "gamma"] and pt_tuple_key[:-1] + ("bias",) in random_paddle_state_dict:
+        renamed_pt_tuple_key = pt_tuple_key[:-1] + ("bias",)
         return renamed_pt_tuple_key, pt_tensor
 
     # embedding
-    if pt_tuple_key[-1] == "weight" and pt_tuple_key[:-1] + (
-            "weight", ) in random_paddle_state_dict:
-        pt_tuple_key = pt_tuple_key[:-1] + ("weight", )
+    if pt_tuple_key[-1] == "weight" and pt_tuple_key[:-1] + ("weight",) in random_paddle_state_dict:
+        pt_tuple_key = pt_tuple_key[:-1] + ("weight",)
         return renamed_pt_tuple_key, pt_tensor
 
     # conv layer
-    renamed_pt_tuple_key = pt_tuple_key[:-1] + ("weight", )
+    renamed_pt_tuple_key = pt_tuple_key[:-1] + ("weight",)
     if pt_tuple_key[-1] == "weight" and pt_tensor.ndim == 4:
         return renamed_pt_tuple_key, pt_tensor
 
     # linear layer
-    renamed_pt_tuple_key = pt_tuple_key[:-1] + ("weight", )
+    renamed_pt_tuple_key = pt_tuple_key[:-1] + ("weight",)
     if pt_tuple_key[-1] == "weight":
         pt_tensor = pt_tensor.t()
         return renamed_pt_tuple_key, pt_tensor
 
     # old PyTorch layer norm weight
-    renamed_pt_tuple_key = pt_tuple_key[:-1] + ("weight", )
+    renamed_pt_tuple_key = pt_tuple_key[:-1] + ("weight",)
     if pt_tuple_key[-1] == "gamma":
         return renamed_pt_tuple_key, pt_tensor
 
     # old PyTorch layer norm bias
-    renamed_pt_tuple_key = pt_tuple_key[:-1] + ("bias", )
+    renamed_pt_tuple_key = pt_tuple_key[:-1] + ("bias",)
     if pt_tuple_key[-1] == "beta":
         return renamed_pt_tuple_key, pt_tensor
 
     return pt_tuple_key, pt_tensor
 
 
 def convert_pytorch_state_dict_to_paddle(pt_state_dict, paddle_model):
@@ -88,20 +87,18 @@
 
     # Need to change some parameters name to match Paddle names
     for pt_key, pt_tensor in pt_state_dict.items():
         renamed_pt_key = rename_key(pt_key)
         pt_tuple_key = tuple(renamed_pt_key.split("."))
 
         # Correctly rename weight parameters
-        paddle_key, paddle_tensor = rename_key_and_reshape_tensor(
-            pt_tuple_key, pt_tensor, random_paddle_state_dict)
+        paddle_key, paddle_tensor = rename_key_and_reshape_tensor(pt_tuple_key, pt_tensor, random_paddle_state_dict)
 
         if paddle_key in random_paddle_state_dict:
-            if list(paddle_tensor.shape) != list(
-                    random_paddle_state_dict[paddle_key].shape):
+            if list(paddle_tensor.shape) != list(random_paddle_state_dict[paddle_key].shape):
                 raise ValueError(
                     f"Paddle checkpoint seems to be incorrect. Weight {pt_key} was expected to be of shape "
                     f"{random_paddle_state_dict[paddle_key].shape}, but is {paddle_tensor.shape}."
                 )
 
         # also add unexpected weight so that warning is thrown
         paddle_state_dict[paddle_key] = paddle_tensor.numpy()
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/modeling_utils.py` & `ppdiffusers-0.9.0/ppdiffusers/modeling_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Copyright (c) 2022 PaddlePaddle Authors. All Rights Reserved.
-# Copyright 2022 The HuggingFace Inc. team.
+# Copyright 2022 The HuggingFace Team. All rights reserved.
 # Copyright (c) 2022, NVIDIA CORPORATION.  All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -12,23 +12,28 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 from functools import partial
-from typing import Callable, List, Optional, Tuple, Union
+from typing import Callable, Optional, Union
 
 import paddle
 import paddle.nn as nn
-
-from .download_utils import ppdiffusers_bos_download
 from requests import HTTPError
 
-from .utils import CONFIG_NAME, PPDIFFUSERS_CACHE, DOWNLOAD_SERVER, WEIGHTS_NAME, logging
+from .download_utils import ppdiffusers_bos_download
+from .utils import (
+    CONFIG_NAME,
+    DOWNLOAD_SERVER,
+    PPDIFFUSERS_CACHE,
+    WEIGHTS_NAME,
+    logging,
+)
 
 logger = logging.get_logger(__name__)
 
 
 def freeze_params(params):
     for param in params:
         param.stop_gradient = True
@@ -45,29 +50,34 @@
 def get_parameter_dtype(parameter: nn.Layer):
     try:
         return next(parameter.named_parameters())[1].dtype
     except StopIteration:
         return paddle.get_default_dtype()
 
 
-def load_dict(checkpoint_file: Union[str, os.PathLike],
-              return_numpy: bool = True):
+def load_dict(checkpoint_file: Union[str, os.PathLike], map_location: str = "cpu"):
     """
     Reads a Paddle checkpoint file, returning properly formatted errors if they arise.
     """
     try:
-        return paddle.load(checkpoint_file, return_numpy=return_numpy)
+        if map_location == "cpu":
+            with paddle.device_scope("cpu"):
+                state_dict = paddle.load(checkpoint_file)
+        else:
+            state_dict = paddle.load(checkpoint_file)
+        return state_dict
     except Exception as e:
         try:
             with open(checkpoint_file) as f:
                 if f.read().startswith("version"):
                     raise OSError(
                         "You seem to have cloned a repository without having git-lfs installed. Please install "
                         "git-lfs and run `git lfs install` followed by `git lfs pull` in the folder "
-                        "you cloned.")
+                        "you cloned."
+                    )
                 else:
                     raise ValueError(
                         f"Unable to locate the file {checkpoint_file} which is necessary to load this pretrained "
                         "model. Make sure you have saved the model properly."
                     ) from e
         except (UnicodeDecodeError, ValueError):
             raise OSError(
@@ -84,17 +94,15 @@
     [`ModelMixin`] takes care of storing the configuration of the models and handles methods for loading, downloading
     and saving models.
 
         - **config_name** ([`str`]) -- A filename under which the model should be stored when calling
           [`~modeling_utils.ModelMixin.save_pretrained`].
     """
     config_name = CONFIG_NAME
-    _automatically_saved_args = [
-        "_ppdiffusers_version", "_class_name", "_name_or_path"
-    ]
+    _automatically_saved_args = ["_ppdiffusers_version", "_class_name", "_name_or_path"]
     _supports_gradient_checkpointing = False
 
     def __init__(self):
         super().__init__()
 
     @property
     def is_gradient_checkpointing(self) -> bool:
@@ -102,27 +110,26 @@
         Whether gradient checkpointing is activated for this model or not.
 
         Note that in other frameworks this feature can be referred to as "activation checkpointing" or "checkpoint
         activations".
         """
         return any(
             hasattr(m, "gradient_checkpointing") and m.gradient_checkpointing
-            for m in self.modules())
+            for m in self.sublayers(include_self=True)
+        )
 
     def enable_gradient_checkpointing(self):
         """
         Activates gradient checkpointing for the current model.
 
         Note that in other frameworks this feature can be referred to as "activation checkpointing" or "checkpoint
         activations".
         """
         if not self._supports_gradient_checkpointing:
-            raise ValueError(
-                f"{self.__class__.__name__} does not support gradient checkpointing."
-            )
+            raise ValueError(f"{self.__class__.__name__} does not support gradient checkpointing.")
         self.apply(partial(self._set_gradient_checkpointing, value=True))
 
     def disable_gradient_checkpointing(self):
         """
         Deactivates gradient checkpointing for the current model.
 
         Note that in other frameworks this feature can be referred to as "activation checkpointing" or "checkpoint
@@ -149,17 +156,15 @@
                 TPUs and need to call this function on all processes. In this case, set `is_main_process=True` only on
                 the main process to avoid race conditions.
             save_function (`Callable`):
                 The function to use to save the state dictionary. Useful on distributed training like TPUs when one
                 need to replace `paddle.save` by another method.
         """
         if os.path.isfile(save_directory):
-            logger.error(
-                f"Provided path ({save_directory}) should be a directory, not a file"
-            )
+            logger.error(f"Provided path ({save_directory}) should be a directory, not a file")
             return
 
         os.makedirs(save_directory, exist_ok=True)
 
         model_to_save = self
 
         # Attach architecture to the config
@@ -171,30 +176,24 @@
         state_dict = model_to_save.state_dict()
 
         # Clean the folder from a previous save
         for filename in os.listdir(save_directory):
             full_filename = os.path.join(save_directory, filename)
             # If we have a shard file that is not going to be replaced, we delete it, but only from the main process
             # in distributed settings to avoid race conditions.
-            if filename.startswith(WEIGHTS_NAME[:-4]) and os.path.isfile(
-                    full_filename) and is_main_process:
+            if filename.startswith(WEIGHTS_NAME[:-4]) and os.path.isfile(full_filename) and is_main_process:
                 os.remove(full_filename)
 
         # Save the model
         save_function(state_dict, os.path.join(save_directory, WEIGHTS_NAME))
 
-        logger.info(
-            f"Model weights saved in {os.path.join(save_directory, WEIGHTS_NAME)}"
-        )
+        logger.info(f"Model weights saved in {os.path.join(save_directory, WEIGHTS_NAME)}")
 
     @classmethod
-    def from_pretrained(
-            cls, pretrained_model_name_or_path: Optional[Union[str,
-                                                               os.PathLike]],
-            **kwargs):
+    def from_pretrained(cls, pretrained_model_name_or_path: Optional[Union[str, os.PathLike]], **kwargs):
         r"""
         Instantiate a pretrained paddle model from a pre-trained model configuration.
 
         The model is set in evaluation mode by default using `model.eval()` (Dropout modules are deactivated). To train
         the model, you should first set it back in training mode with `model.train()`.
 
         The warning *Weights from XXX not initialized from pretrained model* means that the weights of XXX do not come
@@ -209,89 +208,106 @@
                 Can be either:
 
                     - A string, the *model id* of a pretrained model hosted inside a model repo on huggingface.co.
                       Valid model ids should have an organization name, like `google/ddpm-celebahq-256`.
                     - A path to a *directory* containing model weights saved using [`~ModelMixin.save_config`], e.g.,
                       `./my_model_directory/`.
 
+            cache_dir (`Union[str, os.PathLike]`, *optional*):
+                Path to a directory in which a downloaded pretrained model configuration should be cached if the
+                standard cache should not be used.
             paddle_dtype (`str` or `paddle.dtype`, *optional*):
                 Override the default `paddle.dtype` and load the model under this dtype. If `"auto"` is passed the dtype
                 will be automatically derived from the model's weights.
             output_loading_info(`bool`, *optional*, defaults to `False`):
                 Whether or not to also return a dictionary containing missing keys, unexpected keys and error messages.
             subfolder (`str`, *optional*, defaults to `""`):
                 In case the relevant files are located inside a subfolder of the model repo (either remote in
                 huggingface.co or downloaded locally), you can specify the folder name here.
 
-            mirror (`str`, *optional*):
-                Mirror source to accelerate downloads in China. If you are from China and have an accessibility
-                problem, you can set this option to resolve it. Note that we do not guarantee the timeliness or safety.
-                Please refer to the mirror site for more information.
-
         """
+        cache_dir = kwargs.pop("cache_dir", PPDIFFUSERS_CACHE)
         ignore_mismatched_sizes = kwargs.pop("ignore_mismatched_sizes", False)
         output_loading_info = kwargs.pop("output_loading_info", False)
         paddle_dtype = kwargs.pop("paddle_dtype", None)
         subfolder = kwargs.pop("subfolder", None)
 
         # Load config if we don't provide a configuration
         config_path = pretrained_model_name_or_path
 
         # This variable will flag if we're loading a sharded checkpoint. In this case the archive file is just the
         # Load model
         pretrained_model_name_or_path = str(pretrained_model_name_or_path)
         if os.path.isdir(pretrained_model_name_or_path):
-            if os.path.isfile(
-                    os.path.join(pretrained_model_name_or_path, WEIGHTS_NAME)):
+            if os.path.isfile(os.path.join(pretrained_model_name_or_path, WEIGHTS_NAME)):
                 # Load from a Paddle checkpoint
-                model_file = os.path.join(pretrained_model_name_or_path,
-                                          WEIGHTS_NAME)
+                model_file = os.path.join(pretrained_model_name_or_path, WEIGHTS_NAME)
             elif subfolder is not None and os.path.isfile(
-                    os.path.join(pretrained_model_name_or_path, subfolder,
-                                 WEIGHTS_NAME)):
-                model_file = os.path.join(pretrained_model_name_or_path,
-                                          subfolder, WEIGHTS_NAME)
+                os.path.join(pretrained_model_name_or_path, subfolder, WEIGHTS_NAME)
+            ):
+                model_file = os.path.join(pretrained_model_name_or_path, subfolder, WEIGHTS_NAME)
             else:
                 raise EnvironmentError(
                     f"Error no file named {WEIGHTS_NAME} found in directory {pretrained_model_name_or_path}."
                 )
         else:
             try:
                 # Load from URL or cache if already cached
                 model_file = ppdiffusers_bos_download(
                     pretrained_model_name_or_path,
                     filename=WEIGHTS_NAME,
                     subfolder=subfolder,
+                    cache_dir=cache_dir,
                 )
             except HTTPError as err:
                 raise EnvironmentError(
                     "There was a specific connection error when trying to load"
-                    f" {pretrained_model_name_or_path}:\n{err}")
+                    f" {pretrained_model_name_or_path}:\n{err}"
+                )
             except ValueError:
                 raise EnvironmentError(
                     f"We couldn't connect to '{DOWNLOAD_SERVER}' to load this model, couldn't find it"
                     f" in the cached files and it looks like {pretrained_model_name_or_path} is not the path to a"
                     f" directory containing a file named {WEIGHTS_NAME} or"
                     " \nCheckout your internet connection or see how to run the library in"
                     " offline mode at 'https://huggingface.co/docs/diffusers/installation#offline-mode'."
                 )
             except EnvironmentError:
                 raise EnvironmentError(
                     f"Can't load the model for '{pretrained_model_name_or_path}'. If you were trying to load it from "
                     "'https://huggingface.co/models', make sure you don't have a local directory with the same name. "
                     f"Otherwise, make sure '{pretrained_model_name_or_path}' is the correct path to a directory "
-                    f"containing a file named {WEIGHTS_NAME}")
+                    f"containing a file named {WEIGHTS_NAME}"
+                )
 
-        model, unused_kwargs = cls.from_config(
+        config, unused_kwargs = cls.load_config(
             config_path,
+            cache_dir=cache_dir,
             return_unused_kwargs=True,
             subfolder=subfolder,
             **kwargs,
         )
-        state_dict = load_dict(model_file, return_numpy=True)
+        model = cls.from_config(config, **unused_kwargs)
+
+        state_dict = load_dict(model_file, map_location="cpu")
+
+        dtype = set(v.dtype for v in state_dict.values())
+
+        if len(dtype) > 1 and paddle.float32 not in dtype:
+            raise ValueError(
+                f"The weights of the model file {model_file} have a mixture of incompatible dtypes {dtype}. Please"
+                f" make sure that {model_file} weights have only one dtype."
+            )
+        elif len(dtype) > 1 and paddle.float32 in dtype:
+            dtype = paddle.float32
+        else:
+            dtype = dtype.pop()
+
+        # move model to correct dtype
+        model = model.to(dtype=dtype)
 
         model, missing_keys, unexpected_keys, mismatched_keys, error_msgs = cls._load_pretrained_model(
             model,
             state_dict,
             model_file,
             pretrained_model_name_or_path,
             ignore_mismatched_sizes=ignore_mismatched_sizes,
@@ -300,16 +316,15 @@
         loading_info = {
             "missing_keys": missing_keys,
             "unexpected_keys": unexpected_keys,
             "mismatched_keys": mismatched_keys,
             "error_msgs": error_msgs,
         }
 
-        if paddle_dtype is not None and not isinstance(paddle_dtype,
-                                                       paddle.dtype):
+        if paddle_dtype is not None and not isinstance(paddle_dtype, paddle.dtype):
             raise ValueError(
                 f"{paddle_dtype} needs to be of type `paddle.dtype`, e.g. `paddle.float16`, but is {type(paddle_dtype)}."
             )
         elif paddle_dtype is not None:
             model = model.to(dtype=paddle_dtype)
 
         model.register_to_config(_name_or_path=pretrained_model_name_or_path)
@@ -351,20 +366,20 @@
             ignore_mismatched_sizes,
         ):
             mismatched_keys = []
             if ignore_mismatched_sizes:
                 for checkpoint_key in loaded_keys:
                     model_key = checkpoint_key
 
-                    if (model_key in model_state_dict
-                            and list(state_dict[checkpoint_key].shape) !=
-                            model_state_dict[model_key].shape):
+                    if model_key in model_state_dict and list(state_dict[checkpoint_key].shape) != list(
+                        model_state_dict[model_key].shape
+                    ):
                         mismatched_keys.append(
-                            (checkpoint_key, state_dict[checkpoint_key].shape,
-                             model_state_dict[model_key].shape))
+                            (checkpoint_key, state_dict[checkpoint_key].shape, model_state_dict[model_key].shape)
+                        )
                         del state_dict[checkpoint_key]
             return mismatched_keys
 
         if state_dict is not None:
             # Whole checkpoint
             mismatched_keys = _find_mismatched_keys(
                 state_dict,
@@ -377,54 +392,55 @@
 
         if len(error_msgs) > 0:
             error_msg = "\n\t".join(error_msgs)
             if "size mismatch" in error_msg:
                 error_msg += (
                     "\n\tYou may consider adding `ignore_mismatched_sizes=True` in the model `from_pretrained` method."
                 )
-            raise RuntimeError(
-                f"Error(s) in loading state_dict for {model.__class__.__name__}:\n\t{error_msg}"
-            )
+            raise RuntimeError(f"Error(s) in loading state_dict for {model.__class__.__name__}:\n\t{error_msg}")
 
         if len(unexpected_keys) > 0:
             logger.warning(
                 f"Some weights of the model checkpoint at {pretrained_model_name_or_path} were not used when"
                 f" initializing {model.__class__.__name__}: {unexpected_keys}\n- This IS expected if you are"
                 f" initializing {model.__class__.__name__} from the checkpoint of a model trained on another task"
                 " or with another architecture (e.g. initializing a BertForSequenceClassification model from a"
                 " BertForPreTraining model).\n- This IS NOT expected if you are initializing"
                 f" {model.__class__.__name__} from the checkpoint of a model that you expect to be exactly"
                 " identical (initializing a BertForSequenceClassification model from a"
-                " BertForSequenceClassification model).")
-        else:
-            logger.info(
-                f"All model checkpoint weights were used when initializing {model.__class__.__name__}."
+                " BertForSequenceClassification model)."
             )
+        else:
+            logger.info(f"All model checkpoint weights were used when initializing {model.__class__.__name__}.\n")
         if len(missing_keys) > 0:
             logger.warning(
                 f"Some weights of {model.__class__.__name__} were not initialized from the model checkpoint at"
                 f" {pretrained_model_name_or_path} and are newly initialized: {missing_keys}\nYou should probably"
                 " TRAIN this model on a down-stream task to be able to use it for predictions and inference."
             )
         elif len(mismatched_keys) == 0:
             logger.info(
                 f"All the weights of {model.__class__.__name__} were initialized from the model checkpoint at"
                 f" {pretrained_model_name_or_path}.\nIf your task is similar to the task the model of the"
                 f" checkpoint was trained on, you can already use {model.__class__.__name__} for predictions"
-                " without further training.")
+                " without further training."
+            )
         if len(mismatched_keys) > 0:
-            mismatched_warning = "\n".join([
-                f"- {key}: found shape {shape1} in the checkpoint and {shape2} in the model instantiated"
-                for key, shape1, shape2 in mismatched_keys
-            ])
+            mismatched_warning = "\n".join(
+                [
+                    f"- {key}: found shape {shape1} in the checkpoint and {shape2} in the model instantiated"
+                    for key, shape1, shape2 in mismatched_keys
+                ]
+            )
             logger.warning(
                 f"Some weights of {model.__class__.__name__} were not initialized from the model checkpoint at"
                 f" {pretrained_model_name_or_path} and are newly initialized because the shapes did not"
                 f" match:\n{mismatched_warning}\nYou should probably TRAIN this model on a down-stream task to be"
-                " able to use it for predictions and inference.")
+                " able to use it for predictions and inference."
+            )
 
         return model, missing_keys, unexpected_keys, mismatched_keys, error_msgs
 
     @property
     def device(self):
         """
         `paddle.place`: The device on which the module is (assuming that all the module parameters are on the same
@@ -435,17 +451,15 @@
     @property
     def dtype(self) -> paddle.dtype:
         """
         `paddle.dtype`: The dtype of the module (assuming that all the module parameters have the same dtype).
         """
         return get_parameter_dtype(self)
 
-    def num_parameters(self,
-                       only_trainable: bool = False,
-                       exclude_embeddings: bool = False) -> int:
+    def num_parameters(self, only_trainable: bool = False, exclude_embeddings: bool = False) -> int:
         """
         Get number of (optionally, trainable or non-embeddings) parameters in the module.
 
         Args:
             only_trainable (`bool`, *optional*, defaults to `False`):
                 Whether or not to return only the number of trainable parameters
 
@@ -459,22 +473,19 @@
         if exclude_embeddings:
             embedding_param_names = [
                 f"{name}.weight"
                 for name, module_type in self.named_sublayers(include_self=True)
                 if isinstance(module_type, nn.Embedding)
             ]
             non_embedding_parameters = [
-                parameter for name, parameter in self.named_parameters()
-                if name not in embedding_param_names
+                parameter for name, parameter in self.named_parameters() if name not in embedding_param_names
             ]
-            return sum(p.numel() for p in non_embedding_parameters
-                       if not p.stop_gradient or not only_trainable)
+            return sum(p.numel() for p in non_embedding_parameters if not p.stop_gradient or not only_trainable)
         else:
-            return sum(p.numel() for p in self.parameters()
-                       if not p.stop_gradient or not only_trainable)
+            return sum(p.numel() for p in self.parameters() if not p.stop_gradient or not only_trainable)
 
 
 def unwrap_model(model: nn.Layer) -> nn.Layer:
     """
     Recursively unwraps a model from potential containers (as used in distributed training).
 
     Args:
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/models/__init__.py` & `ppdiffusers-0.9.0/ppdiffusers/experimental/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,10 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+# flake8: noqa
 
-from ..utils import is_paddle_available
-
-if is_paddle_available():
-    from .unet_2d import UNet2DModel
-    from .unet_2d_condition import UNet2DConditionModel
-    from .vae import AutoencoderKL, VQModel
+from .rl import ValueGuidedRLPipeline
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/models/ema.py` & `ppdiffusers-0.9.0/ppdiffusers/models/ema.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (c) 2022 PaddlePaddle Authors. All Rights Reserved.
+# Copyright 2022 The HuggingFace Team. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -26,79 +27,77 @@
         use_num_updates: Whether to use number of updates when computing
             averages.
     """
 
     def __init__(self, model, decay=0.9999, use_num_upates=True):
         super().__init__()
         if decay < 0.0 or decay > 1.0:
-            raise ValueError('Decay must be between 0 and 1')
+            raise ValueError("Decay must be between 0 and 1")
 
         self.m_name2s_name = {}
-        self.register_buffer('decay',
-                             paddle.to_tensor(decay, dtype=paddle.float32))
+        self.register_buffer("decay", paddle.to_tensor(decay, dtype=paddle.float32))
         self.register_buffer(
-            'num_updates',
-            paddle.to_tensor(0, dtype=paddle.int64)
-            if use_num_upates else paddle.to_tensor(-1, dtype=paddle.int64))
+            "num_updates",
+            paddle.to_tensor(0, dtype=paddle.int64) if use_num_upates else paddle.to_tensor(-1, dtype=paddle.int64),
+        )
 
         for name, p in model.named_parameters():
             if not p.stop_gradient:
-                #remove as '.'-character is not allowed in buffers
-                s_name = name.replace('.', '')
+                # remove as '.'-character is not allowed in buffers
+                s_name = name.replace(".", "")
                 self.m_name2s_name.update({name: s_name})
                 self.register_buffer(s_name, p.clone().detach())
 
         self.collected_params = []
 
     def forward(self, model):
         decay = self.decay
 
         if self.num_updates >= 0:
             self.num_updates += 1
-            decay = min(self.decay,
-                        (1 + self.num_updates) / (10 + self.num_updates))
+            decay = min(self.decay, (1 + self.num_updates) / (10 + self.num_updates))
 
         one_minus_decay = 1.0 - decay
 
         with paddle.no_grad():
             m_param = dict(model.named_parameters())
             shadow_params = dict(self.named_buffers())
 
             for key in m_param:
                 if not m_param[key].stop_gradient:
                     sname = self.m_name2s_name[key]
                     shadow_params[sname].scale_(decay)
                     shadow_params[sname].add_(m_param[key] * one_minus_decay)
                 else:
-                    assert not key in self.m_name2s_name
+                    assert key not in self.m_name2s_name
 
     def copy_to(self, model):
         m_param = dict(model.named_parameters())
         shadow_params = dict(self.named_buffers())
         for key in m_param:
             if not m_param[key].stop_gradient:
                 m_param[key].copy_(shadow_params[self.m_name2s_name[key]], True)
             else:
-                assert not key in self.m_name2s_name
+                assert key not in self.m_name2s_name
 
     def store(self, parameters):
         """
         Save the current parameters for restoring later.
         Args:
-          parameters: Iterable of `paddle.nn.Parameter`; the parameters to be
+          parameters: Iterable of `EagerParamBase`; the parameters to be
             temporarily stored.
         """
         self.collected_params = [param.clone() for param in parameters]
 
     def restore(self, parameters):
         """
         Restore the parameters stored with the `store` method.
         Useful to validate the model with EMA parameters without affecting the
         original optimization process. Store the parameters before the
         `copy_to` method. After validation (or model saving), use this to
         restore the former parameters.
         Args:
-          parameters: Iterable of `paddle.nn.Parameter`; the parameters to be
+          parameters: Iterable of `EagerParamBase`; the parameters to be
             updated with the stored parameters.
         """
         for c_param, param in zip(self.collected_params, parameters):
             param.copy_(c_param, True)
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/models/resnet.py` & `ppdiffusers-0.9.0/ppdiffusers/models/resnet.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,30 +16,95 @@
 from functools import partial
 
 import paddle
 import paddle.nn as nn
 import paddle.nn.functional as F
 
 
+class Upsample1D(nn.Layer):
+    """
+    An upsampling layer with an optional convolution.
+
+    Parameters:
+            channels: channels in the inputs and outputs.
+            use_conv: a bool determining if a convolution is applied.
+            use_conv_transpose:
+            out_channels:
+    """
+
+    def __init__(self, channels, use_conv=False, use_conv_transpose=False, out_channels=None, name="conv"):
+        super().__init__()
+        self.channels = channels
+        self.out_channels = out_channels or channels
+        self.use_conv = use_conv
+        self.use_conv_transpose = use_conv_transpose
+        self.name = name
+
+        self.conv = None
+        if use_conv_transpose:
+            self.conv = nn.Conv1DTranspose(channels, self.out_channels, 4, 2, 1)
+        elif use_conv:
+            self.conv = nn.Conv1D(self.channels, self.out_channels, 3, padding=1)
+
+    def forward(self, x):
+        assert x.shape[1] == self.channels
+        if self.use_conv_transpose:
+            return self.conv(x)
+
+        x = F.interpolate(x, scale_factor=2.0, mode="nearest")
+
+        if self.use_conv:
+            x = self.conv(x)
+
+        return x
+
+
+class Downsample1D(nn.Layer):
+    """
+    A downsampling layer with an optional convolution.
+
+    Parameters:
+        channels: channels in the inputs and outputs.
+        use_conv: a bool determining if a convolution is applied.
+        out_channels:
+        padding:
+    """
+
+    def __init__(self, channels, use_conv=False, out_channels=None, padding=1, name="conv"):
+        super().__init__()
+        self.channels = channels
+        self.out_channels = out_channels or channels
+        self.use_conv = use_conv
+        self.padding = padding
+        stride = 2
+        self.name = name
+
+        if use_conv:
+            self.conv = nn.Conv1D(self.channels, self.out_channels, 3, stride=stride, padding=padding)
+        else:
+            assert self.channels == self.out_channels
+            self.conv = nn.AvgPool1D(kernel_size=stride, stride=stride)
+
+    def forward(self, x):
+        assert x.shape[1] == self.channels
+        return self.conv(x)
+
+
 class Upsample2D(nn.Layer):
     """
     An upsampling layer with an optional convolution.
 
     Parameters:
         channels: channels in the inputs and outputs.
         use_conv: a bool determining if a convolution is applied.
-        dims: determines if the signal is 1D, 2D, or 3D. If 3D, then upsampling occurs in the inner-two dimensions.
+        use_conv_transpose:
+        out_channels:
     """
 
-    def __init__(self,
-                 channels,
-                 use_conv=False,
-                 use_conv_transpose=False,
-                 out_channels=None,
-                 name="conv"):
+    def __init__(self, channels, use_conv=False, use_conv_transpose=False, out_channels=None, name="conv"):
         super().__init__()
         self.channels = channels
         self.out_channels = out_channels or channels
         self.use_conv = use_conv
         self.use_conv_transpose = use_conv_transpose
         self.name = name
 
@@ -62,30 +127,26 @@
             return self.conv(hidden_states)
 
         # Cast to float32 to as 'upsample_nearest2d_out_frame' op does not support bfloat16
         # TODO(Suraj): Remove this cast once the issue is fixed in PyTorch
         # https://github.com/pytorch/pytorch/issues/86679
         dtype = hidden_states.dtype
         if dtype == paddle.bfloat16:
-            hidden_states = hidden_states.astype(paddle.float32)
+            hidden_states = hidden_states.cast("float32")
 
         # if `output_size` is passed we force the interpolation output
         # size and do not make use of `scale_factor=2`
         if output_size is None:
-            hidden_states = F.interpolate(hidden_states,
-                                          scale_factor=2.0,
-                                          mode="nearest")
+            hidden_states = F.interpolate(hidden_states, scale_factor=2.0, mode="nearest")
         else:
-            hidden_states = F.interpolate(hidden_states,
-                                          size=output_size,
-                                          mode="nearest")
+            hidden_states = F.interpolate(hidden_states, size=output_size, mode="nearest")
 
         # If the input is bfloat16, we cast back to bfloat16
         if dtype == paddle.bfloat16:
-            hidden_states = hidden_states.astype(dtype)
+            hidden_states = hidden_states.cast(dtype)
 
         # TODO(Suraj, Patrick) - clean up after weight dicts are correctly renamed
         if self.use_conv:
             if self.name == "conv":
                 hidden_states = self.conv(hidden_states)
             else:
                 hidden_states = self.Conv2d_0(hidden_states)
@@ -96,37 +157,29 @@
 class Downsample2D(nn.Layer):
     """
     A downsampling layer with an optional convolution.
 
     Parameters:
         channels: channels in the inputs and outputs.
         use_conv: a bool determining if a convolution is applied.
-        dims: determines if the signal is 1D, 2D, or 3D. If 3D, then downsampling occurs in the inner-two dimensions.
+        out_channels:
+        padding:
     """
 
-    def __init__(self,
-                 channels,
-                 use_conv=False,
-                 out_channels=None,
-                 padding=1,
-                 name="conv"):
+    def __init__(self, channels, use_conv=False, out_channels=None, padding=1, name="conv"):
         super().__init__()
         self.channels = channels
         self.out_channels = out_channels or channels
         self.use_conv = use_conv
         self.padding = padding
         stride = 2
         self.name = name
 
         if use_conv:
-            conv = nn.Conv2D(self.channels,
-                             self.out_channels,
-                             3,
-                             stride=stride,
-                             padding=padding)
+            conv = nn.Conv2D(self.channels, self.out_channels, 3, stride=stride, padding=padding)
         else:
             assert self.channels == self.out_channels
             conv = nn.AvgPool2D(kernel_size=stride, stride=stride)
 
         # TODO(Suraj, Patrick) - clean up after weight dicts are correctly renamed
         if name == "conv":
             self.Conv2d_0 = conv
@@ -145,38 +198,24 @@
         assert hidden_states.shape[1] == self.channels
         hidden_states = self.conv(hidden_states)
 
         return hidden_states
 
 
 class FirUpsample2D(nn.Layer):
-
-    def __init__(self,
-                 channels=None,
-                 out_channels=None,
-                 use_conv=False,
-                 fir_kernel=(1, 3, 3, 1)):
+    def __init__(self, channels=None, out_channels=None, use_conv=False, fir_kernel=(1, 3, 3, 1)):
         super().__init__()
         out_channels = out_channels if out_channels else channels
         if use_conv:
-            self.Conv2d_0 = nn.Conv2D(channels,
-                                      out_channels,
-                                      kernel_size=3,
-                                      stride=1,
-                                      padding=1)
+            self.Conv2d_0 = nn.Conv2D(channels, out_channels, kernel_size=3, stride=1, padding=1)
         self.use_conv = use_conv
         self.fir_kernel = fir_kernel
         self.out_channels = out_channels
 
-    def _upsample_2d(self,
-                     hidden_states,
-                     weight=None,
-                     kernel=None,
-                     factor=2,
-                     gain=1):
+    def _upsample_2d(self, hidden_states, weight=None, kernel=None, factor=2, gain=1):
         """Fused `upsample_2d()` followed by `Conv2d()`.
 
         Padding is performed only once at the beginning, not between the operations. The fused op is considerably more
         efficient than performing the same calculation using standard TensorFlow ops. It supports gradients of
         arbitrary order.
 
         Args:
@@ -217,32 +256,28 @@
             stride = (factor, factor)
             # Determine data dimensions.
             output_shape = (
                 (hidden_states.shape[2] - 1) * factor + convH,
                 (hidden_states.shape[3] - 1) * factor + convW,
             )
             output_padding = (
-                output_shape[0] - (hidden_states.shape[2] - 1) * stride[0] -
-                convH,
-                output_shape[1] - (hidden_states.shape[3] - 1) * stride[1] -
-                convW,
+                output_shape[0] - (hidden_states.shape[2] - 1) * stride[0] - convH,
+                output_shape[1] - (hidden_states.shape[3] - 1) * stride[1] - convW,
             )
             assert output_padding[0] >= 0 and output_padding[1] >= 0
             num_groups = hidden_states.shape[1] // inC
 
             # Transpose weights.
             weight = weight.reshape([num_groups, -1, inC, convH, convW])
             weight = paddle.flip(weight, axis=[3, 4]).transpose([0, 2, 1, 3, 4])
             weight = weight.reshape([num_groups * inC, -1, convH, convW])
 
-            inverse_conv = F.conv2d_transpose(hidden_states,
-                                              weight,
-                                              stride=stride,
-                                              output_padding=output_padding,
-                                              padding=0)
+            inverse_conv = F.conv2d_transpose(
+                hidden_states, weight, stride=stride, output_padding=output_padding, padding=0
+            )
 
             output = upfirdn2d_native(
                 inverse_conv,
                 paddle.to_tensor(kernel),
                 pad=((pad_value + 1) // 2 + factor - 1, pad_value // 2 + 1),
             )
         else:
@@ -254,51 +289,33 @@
                 pad=((pad_value + 1) // 2 + factor - 1, pad_value // 2),
             )
 
         return output
 
     def forward(self, hidden_states):
         if self.use_conv:
-            height = self._upsample_2d(hidden_states,
-                                       self.Conv2d_0.weight,
-                                       kernel=self.fir_kernel)
+            height = self._upsample_2d(hidden_states, self.Conv2d_0.weight, kernel=self.fir_kernel)
             height = height + self.Conv2d_0.bias.reshape([1, -1, 1, 1])
         else:
-            height = self._upsample_2d(hidden_states,
-                                       kernel=self.fir_kernel,
-                                       factor=2)
+            height = self._upsample_2d(hidden_states, kernel=self.fir_kernel, factor=2)
 
         return height
 
 
 class FirDownsample2D(nn.Layer):
-
-    def __init__(self,
-                 channels=None,
-                 out_channels=None,
-                 use_conv=False,
-                 fir_kernel=(1, 3, 3, 1)):
+    def __init__(self, channels=None, out_channels=None, use_conv=False, fir_kernel=(1, 3, 3, 1)):
         super().__init__()
         out_channels = out_channels if out_channels else channels
         if use_conv:
-            self.Conv2d_0 = nn.Conv2D(channels,
-                                      out_channels,
-                                      kernel_size=3,
-                                      stride=1,
-                                      padding=1)
+            self.Conv2d_0 = nn.Conv2D(channels, out_channels, kernel_size=3, stride=1, padding=1)
         self.fir_kernel = fir_kernel
         self.use_conv = use_conv
         self.out_channels = out_channels
 
-    def _downsample_2d(self,
-                       hidden_states,
-                       weight=None,
-                       kernel=None,
-                       factor=2,
-                       gain=1):
+    def _downsample_2d(self, hidden_states, weight=None, kernel=None, factor=2, gain=1):
         """Fused `Conv2d()` followed by `downsample_2d()`.
         Padding is performed only once at the beginning, not between the operations. The fused op is considerably more
         efficient than performing the same calculation using standard TensorFlow ops. It supports gradients of
         arbitrary order.
 
         Args:
             hidden_states: Input tensor of the shape `[N, C, H, W]` or `[N, H, W, C]`.
@@ -332,46 +349,37 @@
             pad_value = (kernel.shape[0] - factor) + (convW - 1)
             stride_value = [factor, factor]
             upfirdn_input = upfirdn2d_native(
                 hidden_states,
                 paddle.to_tensor(kernel),
                 pad=((pad_value + 1) // 2, pad_value // 2),
             )
-            output = F.conv2d(upfirdn_input,
-                              weight,
-                              stride=stride_value,
-                              padding=0)
+            output = F.conv2d(upfirdn_input, weight, stride=stride_value, padding=0)
         else:
             pad_value = kernel.shape[0] - factor
             output = upfirdn2d_native(
                 hidden_states,
                 paddle.to_tensor(kernel),
                 down=factor,
                 pad=((pad_value + 1) // 2, pad_value // 2),
             )
 
         return output
 
     def forward(self, hidden_states):
         if self.use_conv:
-            downsample_input = self._downsample_2d(hidden_states,
-                                                   weight=self.Conv2d_0.weight,
-                                                   kernel=self.fir_kernel)
-            hidden_states = downsample_input + self.Conv2d_0.bias.reshape(
-                [1, -1, 1, 1])
+            downsample_input = self._downsample_2d(hidden_states, weight=self.Conv2d_0.weight, kernel=self.fir_kernel)
+            hidden_states = downsample_input + self.Conv2d_0.bias.reshape([1, -1, 1, 1])
         else:
-            hidden_states = self._downsample_2d(hidden_states,
-                                                kernel=self.fir_kernel,
-                                                factor=2)
+            hidden_states = self._downsample_2d(hidden_states, kernel=self.fir_kernel, factor=2)
 
         return hidden_states
 
 
 class ResnetBlock2D(nn.Layer):
-
     def __init__(
         self,
         *,
         in_channels,
         out_channels=None,
         conv_shortcut=False,
         dropout=0.0,
@@ -399,78 +407,57 @@
         self.up = up
         self.down = down
         self.output_scale_factor = output_scale_factor
 
         if groups_out is None:
             groups_out = groups
 
-        self.norm1 = nn.GroupNorm(num_groups=groups,
-                                  num_channels=in_channels,
-                                  epsilon=eps)
-
-        self.conv1 = nn.Conv2D(in_channels,
-                               out_channels,
-                               kernel_size=3,
-                               stride=1,
-                               padding=1)
+        self.norm1 = nn.GroupNorm(num_groups=groups, num_channels=in_channels, epsilon=eps)
+
+        self.conv1 = nn.Conv2D(in_channels, out_channels, kernel_size=3, stride=1, padding=1)
 
         if temb_channels is not None:
             self.time_emb_proj = nn.Linear(temb_channels, out_channels)
         else:
             self.time_emb_proj = None
 
-        self.norm2 = nn.GroupNorm(num_groups=groups_out,
-                                  num_channels=out_channels,
-                                  epsilon=eps)
+        self.norm2 = nn.GroupNorm(num_groups=groups_out, num_channels=out_channels, epsilon=eps)
         self.dropout = nn.Dropout(dropout)
-        self.conv2 = nn.Conv2D(out_channels,
-                               out_channels,
-                               kernel_size=3,
-                               stride=1,
-                               padding=1)
+        self.conv2 = nn.Conv2D(out_channels, out_channels, kernel_size=3, stride=1, padding=1)
 
         if non_linearity == "swish":
             self.nonlinearity = lambda x: F.silu(x)
         elif non_linearity == "mish":
             self.nonlinearity = Mish()
         elif non_linearity == "silu":
             self.nonlinearity = nn.Silu()
 
         self.upsample = self.downsample = None
         if self.up:
             if kernel == "fir":
                 fir_kernel = (1, 3, 3, 1)
                 self.upsample = lambda x: upsample_2d(x, kernel=fir_kernel)
             elif kernel == "sde_vp":
-                self.upsample = partial(F.interpolate,
-                                        scale_factor=2.0,
-                                        mode="nearest")
+                self.upsample = partial(F.interpolate, scale_factor=2.0, mode="nearest")
             else:
                 self.upsample = Upsample2D(in_channels, use_conv=False)
         elif self.down:
             if kernel == "fir":
                 fir_kernel = (1, 3, 3, 1)
                 self.downsample = lambda x: downsample_2d(x, kernel=fir_kernel)
             elif kernel == "sde_vp":
                 self.downsample = partial(F.avg_pool2d, kernel_size=2, stride=2)
             else:
-                self.downsample = Downsample2D(in_channels,
-                                               use_conv=False,
-                                               padding=1,
-                                               name="op")
+                self.downsample = Downsample2D(in_channels, use_conv=False, padding=1, name="op")
 
         self.use_in_shortcut = self.in_channels != self.out_channels if use_in_shortcut is None else use_in_shortcut
 
         self.conv_shortcut = None
         if self.use_in_shortcut:
-            self.conv_shortcut = nn.Conv2D(in_channels,
-                                           out_channels,
-                                           kernel_size=1,
-                                           stride=1,
-                                           padding=0)
+            self.conv_shortcut = nn.Conv2D(in_channels, out_channels, kernel_size=1, stride=1, padding=0)
 
     def forward(self, input_tensor, temb):
         hidden_states = input_tensor
 
         hidden_states = self.norm1(hidden_states)
         hidden_states = self.nonlinearity(hidden_states)
 
@@ -492,26 +479,87 @@
 
         hidden_states = self.dropout(hidden_states)
         hidden_states = self.conv2(hidden_states)
 
         if self.conv_shortcut is not None:
             input_tensor = self.conv_shortcut(input_tensor)
 
-        output_tensor = (input_tensor +
-                         hidden_states) / self.output_scale_factor
+        output_tensor = (input_tensor + hidden_states) / self.output_scale_factor
 
         return output_tensor
 
 
 class Mish(nn.Layer):
-
     def forward(self, hidden_states):
         return hidden_states * paddle.tanh(F.softplus(hidden_states))
 
 
+# unet_rl.py
+def rearrange_dims(tensor):
+    if len(tensor.shape) == 2:
+        return tensor[:, :, None]
+    if len(tensor.shape) == 3:
+        return tensor[:, :, None, :]
+    elif len(tensor.shape) == 4:
+        return tensor[:, :, 0, :]
+    else:
+        raise ValueError(f"`len(tensor)`: {len(tensor)} has to be 2, 3 or 4.")
+
+
+class Conv1dBlock(nn.Layer):
+    """
+    Conv1d --> GroupNorm --> Mish
+    """
+
+    def __init__(self, inp_channels, out_channels, kernel_size, n_groups=8):
+        super().__init__()
+
+        self.conv1d = nn.Conv1D(inp_channels, out_channels, kernel_size, padding=kernel_size // 2)
+        self.group_norm = nn.GroupNorm(n_groups, out_channels)
+        self.mish = nn.Mish()
+
+    def forward(self, x):
+        x = self.conv1d(x)
+        x = rearrange_dims(x)
+        x = self.group_norm(x)
+        x = rearrange_dims(x)
+        x = self.mish(x)
+        return x
+
+
+# unet_rl.py
+class ResidualTemporalBlock1D(nn.Layer):
+    def __init__(self, inp_channels, out_channels, embed_dim, kernel_size=5):
+        super().__init__()
+        self.conv_in = Conv1dBlock(inp_channels, out_channels, kernel_size)
+        self.conv_out = Conv1dBlock(out_channels, out_channels, kernel_size)
+
+        self.time_emb_act = nn.Mish()
+        self.time_emb = nn.Linear(embed_dim, out_channels)
+
+        self.residual_conv = (
+            nn.Conv1D(inp_channels, out_channels, 1) if inp_channels != out_channels else nn.Identity()
+        )
+
+    def forward(self, x, t):
+        """
+        Args:
+            x : [ batch_size x inp_channels x horizon ]
+            t : [ batch_size x embed_dim ]
+
+        returns:
+            out : [ batch_size x out_channels x horizon ]
+        """
+        t = self.time_emb_act(t)
+        t = self.time_emb(t)
+        out = self.conv_in(x) + rearrange_dims(t)
+        out = self.conv_out(out)
+        return out + self.residual_conv(x)
+
+
 def upsample_2d(hidden_states, kernel=None, factor=2, gain=1):
     r"""Upsample2D a batch of 2D images with the given filter.
     Accepts a batch of 2D images of the shape `[N, C, H, W]` or `[N, H, W, C]` and upsamples each image with the given
     filter. The filter is normalized so that if the input pixels are constant, they will be scaled by the specified
     `gain`. Pixels outside the image are assumed to be zero, and the filter is padded with zeros so that its shape is
     a: multiple of the upsampling factor.
 
@@ -530,15 +578,18 @@
         kernel = [1] * factor
 
     kernel = paddle.to_tensor(kernel, dtype="float32")
     if kernel.ndim == 1:
         kernel = paddle.outer(kernel, kernel)
     kernel /= paddle.sum(kernel)
 
-    kernel = kernel * (gain * (factor**2))
+    if gain != 1:
+        kernel = kernel * (gain * (factor**2))
+    else:
+        kernel = kernel * (factor**2)
     pad_value = kernel.shape[0] - factor
     output = upfirdn2d_native(
         hidden_states,
         kernel,
         up=factor,
         pad=((pad_value + 1) // 2 + factor - 1, pad_value // 2),
     )
@@ -570,59 +621,82 @@
     kernel = paddle.to_tensor(kernel, dtype="float32")
     if kernel.ndim == 1:
         kernel = paddle.outer(kernel, kernel)
     kernel /= paddle.sum(kernel)
 
     kernel = kernel * gain
     pad_value = kernel.shape[0] - factor
-    output = upfirdn2d_native(hidden_states,
-                              kernel,
-                              down=factor,
-                              pad=((pad_value + 1) // 2, pad_value // 2))
+    output = upfirdn2d_native(hidden_states, kernel, down=factor, pad=((pad_value + 1) // 2, pad_value // 2))
     return output
 
 
+def dummy_pad(tensor, up_x=0, up_y=0):
+    if up_x > 0:
+        tensor = paddle.concat(
+            [
+                tensor,
+                paddle.zeros(
+                    [tensor.shape[0], tensor.shape[1], tensor.shape[2], tensor.shape[3], up_x, tensor.shape[5]],
+                    dtype=tensor.dtype,
+                ),
+            ],
+            axis=4,
+        )
+    if up_y > 0:
+        tensor = paddle.concat(
+            [
+                tensor,
+                paddle.zeros(
+                    [tensor.shape[0], tensor.shape[1], up_y, tensor.shape[3], tensor.shape[4], tensor.shape[5]],
+                    dtype=tensor.dtype,
+                ),
+            ],
+            axis=2,
+        )
+    return tensor
+
+
 def upfirdn2d_native(tensor, kernel, up=1, down=1, pad=(0, 0)):
     up_x = up_y = up
     down_x = down_y = down
     pad_x0 = pad_y0 = pad[0]
     pad_x1 = pad_y1 = pad[1]
 
     _, channel, in_h, in_w = tensor.shape
     tensor = tensor.reshape([-1, in_h, in_w, 1])
 
     _, in_h, in_w, minor = tensor.shape
     kernel_h, kernel_w = kernel.shape
 
     out = tensor.reshape([-1, in_h, 1, in_w, 1, minor])
-
-    # TODO F.pad
-    out = F.pad(out, [0, 0, 0, up_x - 1, 0, 0, 0, up_y - 1])
+    # (TODO, junnyu F.pad bug)
+    # F.pad(out, [0, 0, 0, up_x - 1, 0, 0, 0, up_y - 1])
+    out = dummy_pad(out, up_x - 1, up_y - 1)
     out = out.reshape([-1, in_h * up_y, in_w * up_x, minor])
 
-    out = F.pad(
-        out,
-        [0, 0,
-         max(pad_x0, 0),
-         max(pad_x1, 0),
-         max(pad_y0, 0),
-         max(pad_y1, 0)])
-    out = out[:,
-              max(-pad_y0, 0):out.shape[1] - max(-pad_y1, 0),
-              max(-pad_x0, 0):out.shape[2] - max(-pad_x1, 0), :, ]
+    # (TODO, junnyu F.pad bug)
+    # out = F.pad(out, [0, 0, max(pad_x0, 0), max(pad_x1, 0), max(pad_y0, 0), max(pad_y1, 0)])
+    out = out.unsqueeze(0)
+    out = F.pad(out, [max(pad_x0, 0), max(pad_x1, 0), max(pad_y0, 0), max(pad_y1, 0), 0, 0], data_format="NDHWC")
+    out = out.squeeze(0)
+
+    out = out[
+        :,
+        max(-pad_y0, 0) : out.shape[1] - max(-pad_y1, 0),
+        max(-pad_x0, 0) : out.shape[2] - max(-pad_x1, 0),
+        :,
+    ]
 
     out = out.transpose([0, 3, 1, 2])
-    out = out.reshape(
-        [-1, 1, in_h * up_y + pad_y0 + pad_y1, in_w * up_x + pad_x0 + pad_x1])
+    out = out.reshape([-1, 1, in_h * up_y + pad_y0 + pad_y1, in_w * up_x + pad_x0 + pad_x1])
     w = paddle.flip(kernel, [0, 1]).reshape([1, 1, kernel_h, kernel_w])
     out = F.conv2d(out, w)
-    out = out.reshape([
-        -1, minor, in_h * up_y + pad_y0 + pad_y1 - kernel_h + 1,
-        in_w * up_x + pad_x0 + pad_x1 - kernel_w + 1
-    ])
+    out = out.reshape(
+        [-1, minor, in_h * up_y + pad_y0 + pad_y1 - kernel_h + 1, in_w * up_x + pad_x0 + pad_x1 - kernel_w + 1]
+    )
     out = out.transpose([0, 2, 3, 1])
     out = out[:, ::down_y, ::down_x, :]
 
     out_h = (in_h * up_y + pad_y0 + pad_y1 - kernel_h) // down_y + 1
     out_w = (in_w * up_x + pad_x0 + pad_x1 - kernel_w) // down_x + 1
 
     return out.reshape([-1, channel, out_h, out_w])
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/models/unet_2d.py` & `ppdiffusers-0.9.0/ppdiffusers/models/unet_2d.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,26 +8,25 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 from dataclasses import dataclass
 from typing import Optional, Tuple, Union
 
 import paddle
 import paddle.nn as nn
 
 from ..configuration_utils import ConfigMixin, register_to_config
 from ..modeling_utils import ModelMixin
 from ..utils import BaseOutput
 from .embeddings import GaussianFourierProjection, TimestepEmbedding, Timesteps
-from .unet_blocks import UNetMidBlock2D, get_down_block, get_up_block
+from .unet_2d_blocks import UNetMidBlock2D, get_down_block, get_up_block
 
 
 @dataclass
 class UNet2DOutput(BaseOutput):
     """
     Args:
         sample (`paddle.Tensor` of shape `(batch_size, num_channels, height, width)`):
@@ -41,23 +40,23 @@
     r"""
     UNet2DModel is a 2D UNet model that takes in a noisy sample and a timestep and returns sample shaped output.
 
     This model inherits from [`ModelMixin`]. Check the superclass documentation for the generic methods the library
     implements for all the model (such as downloading or saving, etc.)
 
     Parameters:
-        sample_size (`paddle.Tensor` of shape `(batch_size, num_channels, height, width)`, *optional*):
-            Input sample size.
+        sample_size (`int` or `Tuple[int, int]`, *optional*, defaults to `None`):
+            Height and width of input/output sample.
         in_channels (`int`, *optional*, defaults to 3): Number of channels in the input image.
         out_channels (`int`, *optional*, defaults to 3): Number of channels in the output.
         center_input_sample (`bool`, *optional*, defaults to `False`): Whether to center the input sample.
         time_embedding_type (`str`, *optional*, defaults to `"positional"`): Type of time embedding to use.
         freq_shift (`int`, *optional*, defaults to 0): Frequency shift for fourier time embedding.
         flip_sin_to_cos (`bool`, *optional*, defaults to :
-            obj:`False`): Whether to flip sin to cos for fourier time embedding.
+            obj:`True`): Whether to flip sin to cos for fourier time embedding.
         down_block_types (`Tuple[str]`, *optional*, defaults to :
             obj:`("DownBlock2D", "AttnDownBlock2D", "AttnDownBlock2D", "AttnDownBlock2D")`): Tuple of downsample block
             types.
         up_block_types (`Tuple[str]`, *optional*, defaults to :
             obj:`("AttnUpBlock2D", "AttnUpBlock2D", "AttnUpBlock2D", "UpBlock2D")`): Tuple of upsample block types.
         block_out_channels (`Tuple[int]`, *optional*, defaults to :
             obj:`(224, 448, 672, 896)`): Tuple of block output channels.
@@ -69,25 +68,23 @@
         norm_num_groups (`int`, *optional*, defaults to `32`): The number of groups for the normalization.
         norm_eps (`float`, *optional*, defaults to `1e-5`): The epsilon for the normalization.
     """
 
     @register_to_config
     def __init__(
         self,
-        sample_size: Optional[int] = None,
+        sample_size: Optional[Union[int, Tuple[int, int]]] = None,
         in_channels: int = 3,
         out_channels: int = 3,
         center_input_sample: bool = False,
         time_embedding_type: str = "positional",
         freq_shift: int = 0,
         flip_sin_to_cos: bool = True,
-        down_block_types: Tuple[str] = ("DownBlock2D", "AttnDownBlock2D",
-                                        "AttnDownBlock2D", "AttnDownBlock2D"),
-        up_block_types: Tuple[str] = ("AttnUpBlock2D", "AttnUpBlock2D",
-                                      "AttnUpBlock2D", "UpBlock2D"),
+        down_block_types: Tuple[str] = ("DownBlock2D", "AttnDownBlock2D", "AttnDownBlock2D", "AttnDownBlock2D"),
+        up_block_types: Tuple[str] = ("AttnUpBlock2D", "AttnUpBlock2D", "AttnUpBlock2D", "UpBlock2D"),
         block_out_channels: Tuple[int] = (224, 448, 672, 896),
         layers_per_block: int = 2,
         mid_block_scale_factor: float = 1,
         downsample_padding: int = 1,
         act_fn: str = "silu",
         attention_head_dim: int = 8,
         norm_num_groups: int = 32,
@@ -95,31 +92,25 @@
     ):
         super().__init__()
 
         self.sample_size = sample_size
         time_embed_dim = block_out_channels[0] * 4
 
         # input
-        self.conv_in = nn.Conv2D(in_channels,
-                                 block_out_channels[0],
-                                 kernel_size=3,
-                                 padding=(1, 1))
+        self.conv_in = nn.Conv2D(in_channels, block_out_channels[0], kernel_size=3, padding=(1, 1))
 
         # time
         if time_embedding_type == "fourier":
-            self.time_proj = GaussianFourierProjection(
-                embedding_size=block_out_channels[0], scale=16)
+            self.time_proj = GaussianFourierProjection(embedding_size=block_out_channels[0], scale=16)
             timestep_input_dim = 2 * block_out_channels[0]
         elif time_embedding_type == "positional":
-            self.time_proj = Timesteps(block_out_channels[0], flip_sin_to_cos,
-                                       freq_shift)
+            self.time_proj = Timesteps(block_out_channels[0], flip_sin_to_cos, freq_shift)
             timestep_input_dim = block_out_channels[0]
 
-        self.time_embedding = TimestepEmbedding(timestep_input_dim,
-                                                time_embed_dim)
+        self.time_embedding = TimestepEmbedding(timestep_input_dim, time_embed_dim)
 
         self.down_blocks = nn.LayerList([])
         self.mid_block = None
         self.up_blocks = nn.LayerList([])
 
         # down
         output_channel = block_out_channels[0]
@@ -157,17 +148,15 @@
 
         # up
         reversed_block_out_channels = list(reversed(block_out_channels))
         output_channel = reversed_block_out_channels[0]
         for i, up_block_type in enumerate(up_block_types):
             prev_output_channel = output_channel
             output_channel = reversed_block_out_channels[i]
-            input_channel = reversed_block_out_channels[min(
-                i + 1,
-                len(block_out_channels) - 1)]
+            input_channel = reversed_block_out_channels[min(i + 1, len(block_out_channels) - 1)]
 
             is_final_block = i == len(block_out_channels) - 1
 
             up_block = get_up_block(
                 up_block_type,
                 num_layers=layers_per_block + 1,
                 in_channels=input_channel,
@@ -180,24 +169,20 @@
                 resnet_groups=norm_num_groups,
                 attn_num_head_channels=attention_head_dim,
             )
             self.up_blocks.append(up_block)
             prev_output_channel = output_channel
 
         # out
-        num_groups_out = norm_num_groups if norm_num_groups is not None else min(
-            block_out_channels[0] // 4, 32)
-        self.conv_norm_out = nn.GroupNorm(num_channels=block_out_channels[0],
-                                          num_groups=num_groups_out,
-                                          epsilon=norm_eps)
+        num_groups_out = norm_num_groups if norm_num_groups is not None else min(block_out_channels[0] // 4, 32)
+        self.conv_norm_out = nn.GroupNorm(
+            num_channels=block_out_channels[0], num_groups=num_groups_out, epsilon=norm_eps
+        )
         self.conv_act = nn.Silu()
-        self.conv_out = nn.Conv2D(block_out_channels[0],
-                                  out_channels,
-                                  3,
-                                  padding=1)
+        self.conv_out = nn.Conv2D(block_out_channels[0], out_channels, kernel_size=3, padding=1)
 
     def forward(
         self,
         sample: paddle.Tensor,
         timestep: Union[paddle.Tensor, float, int],
         return_dict: bool = True,
     ) -> Union[UNet2DOutput, Tuple]:
@@ -220,65 +205,58 @@
         timesteps = timestep
         if not paddle.is_tensor(timesteps):
             timesteps = paddle.to_tensor([timesteps], dtype="int64")
         elif paddle.is_tensor(timesteps) and len(timesteps.shape) == 0:
             timesteps = timesteps[None]
 
         # broadcast to batch dimension in a way that's compatible with ONNX/Core ML
-        timesteps = timesteps * paddle.ones(
-            (sample.shape[0], ), dtype=timesteps.dtype)
+        timesteps = timesteps * paddle.ones((sample.shape[0],), dtype=timesteps.dtype)
 
-        t_emb = self.time_proj(timesteps).astype(self.dtype)
+        t_emb = self.time_proj(timesteps).cast(self.dtype)
         emb = self.time_embedding(t_emb)
 
         # 2. pre-process
         skip_sample = sample
         sample = self.conv_in(sample)
 
         # 3. down
-        down_block_res_samples = (sample, )
+        down_block_res_samples = (sample,)
         for downsample_block in self.down_blocks:
             if hasattr(downsample_block, "skip_conv"):
                 sample, res_samples, skip_sample = downsample_block(
-                    hidden_states=sample, temb=emb, skip_sample=skip_sample)
+                    hidden_states=sample, temb=emb, skip_sample=skip_sample
+                )
             else:
-                sample, res_samples = downsample_block(hidden_states=sample,
-                                                       temb=emb)
+                sample, res_samples = downsample_block(hidden_states=sample, temb=emb)
 
             down_block_res_samples += res_samples
 
         # 4. mid
         sample = self.mid_block(sample, emb)
 
         # 5. up
         skip_sample = None
         for upsample_block in self.up_blocks:
-            res_samples = down_block_res_samples[-len(upsample_block.resnets):]
-            down_block_res_samples = down_block_res_samples[:-len(upsample_block
-                                                                  .resnets)]
+            res_samples = down_block_res_samples[-len(upsample_block.resnets) :]
+            down_block_res_samples = down_block_res_samples[: -len(upsample_block.resnets)]
 
             if hasattr(upsample_block, "skip_conv"):
-                sample, skip_sample = upsample_block(sample, res_samples, emb,
-                                                     skip_sample)
+                sample, skip_sample = upsample_block(sample, res_samples, emb, skip_sample)
             else:
                 sample = upsample_block(sample, res_samples, emb)
 
         # 6. post-process
-        # make sure hidden states is in float32
-        # when running in half-precision
-        sample = self.conv_norm_out(sample.astype("float32")).astype(
-            sample.dtype)
+        sample = self.conv_norm_out(sample)
         sample = self.conv_act(sample)
         sample = self.conv_out(sample)
 
         if skip_sample is not None:
             sample += skip_sample
 
         if self.config.time_embedding_type == "fourier":
-            timesteps = timesteps.reshape(
-                [sample.shape[0], *([1] * len(sample.shape[1:]))])
+            timesteps = timesteps.reshape([sample.shape[0], *([1] * len(sample.shape[1:]))])
             sample = sample / timesteps
 
         if not return_dict:
-            return (sample, )
+            return (sample,)
 
         return UNet2DOutput(sample=sample)
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/models/unet_2d_condition.py` & `ppdiffusers-0.9.0/ppdiffusers/models/unet_2d_condition.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,26 +8,25 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 from dataclasses import dataclass
 from typing import Optional, Tuple, Union
 
 import paddle
 import paddle.nn as nn
 
 from ..configuration_utils import ConfigMixin, register_to_config
 from ..modeling_utils import ModelMixin
 from ..utils import BaseOutput, logging
 from .embeddings import TimestepEmbedding, Timesteps
-from .unet_blocks import (
+from .unet_2d_blocks import (
     CrossAttnDownBlock2D,
     CrossAttnUpBlock2D,
     DownBlock2D,
     UNetMidBlock2DCrossAttn,
     UpBlock2D,
     get_down_block,
     get_up_block,
@@ -52,15 +51,16 @@
     UNet2DConditionModel is a conditional 2D UNet model that takes in a noisy sample, conditional state, and a timestep
     and returns sample shaped output.
 
     This model inherits from [`ModelMixin`]. Check the superclass documentation for the generic methods the library
     implements for all the models (such as downloading or saving, etc.)
 
     Parameters:
-        sample_size (`int`, *optional*): The size of the input sample.
+        sample_size (`int` or `Tuple[int, int]`, *optional*, defaults to `None`):
+            Height and width of input/output sample.
         in_channels (`int`, *optional*, defaults to 4): The number of channels in the input sample.
         out_channels (`int`, *optional*, defaults to 4): The number of channels in the output.
         center_input_sample (`bool`, *optional*, defaults to `False`): Whether to center the input sample.
         flip_sin_to_cos (`bool`, *optional*, defaults to `False`):
             Whether to flip the sin to cos in the time embedding.
         freq_shift (`int`, *optional*, defaults to 0): The frequency shift to apply to the time embedding.
         down_block_types (`Tuple[str]`, *optional*, defaults to `("CrossAttnDownBlock2D", "CrossAttnDownBlock2D", "CrossAttnDownBlock2D", "DownBlock2D")`):
@@ -92,50 +92,57 @@
         freq_shift: int = 0,
         down_block_types: Tuple[str] = (
             "CrossAttnDownBlock2D",
             "CrossAttnDownBlock2D",
             "CrossAttnDownBlock2D",
             "DownBlock2D",
         ),
-        up_block_types: Tuple[str] = ("UpBlock2D", "CrossAttnUpBlock2D",
-                                      "CrossAttnUpBlock2D",
-                                      "CrossAttnUpBlock2D"),
+        up_block_types: Tuple[str] = ("UpBlock2D", "CrossAttnUpBlock2D", "CrossAttnUpBlock2D", "CrossAttnUpBlock2D"),
+        only_cross_attention: Union[bool, Tuple[bool]] = False,
         block_out_channels: Tuple[int] = (320, 640, 1280, 1280),
         layers_per_block: int = 2,
         downsample_padding: int = 1,
         mid_block_scale_factor: float = 1,
         act_fn: str = "silu",
         norm_num_groups: int = 32,
         norm_eps: float = 1e-5,
         cross_attention_dim: int = 1280,
-        attention_head_dim: int = 8,
+        attention_head_dim: Union[int, Tuple[int]] = 8,
+        dual_cross_attention: bool = False,
+        use_linear_projection: bool = False,
+        num_class_embeds: Optional[int] = None,
     ):
         super().__init__()
 
         self.sample_size = sample_size
         time_embed_dim = block_out_channels[0] * 4
 
         # input
-        self.conv_in = nn.Conv2D(in_channels,
-                                 block_out_channels[0],
-                                 kernel_size=3,
-                                 padding=(1, 1))
+        self.conv_in = nn.Conv2D(in_channels, block_out_channels[0], kernel_size=3, padding=(1, 1))
 
         # time
-        self.time_proj = Timesteps(block_out_channels[0], flip_sin_to_cos,
-                                   freq_shift)
+        self.time_proj = Timesteps(block_out_channels[0], flip_sin_to_cos, freq_shift)
         timestep_input_dim = block_out_channels[0]
 
-        self.time_embedding = TimestepEmbedding(timestep_input_dim,
-                                                time_embed_dim)
+        self.time_embedding = TimestepEmbedding(timestep_input_dim, time_embed_dim)
+
+        # class embedding
+        if num_class_embeds is not None:
+            self.class_embedding = nn.Embedding(num_class_embeds, time_embed_dim)
 
         self.down_blocks = nn.LayerList([])
         self.mid_block = None
         self.up_blocks = nn.LayerList([])
 
+        if isinstance(only_cross_attention, bool):
+            only_cross_attention = [only_cross_attention] * len(down_block_types)
+
+        if isinstance(attention_head_dim, int):
+            attention_head_dim = (attention_head_dim,) * len(down_block_types)
+
         # down
         output_channel = block_out_channels[0]
         for i, down_block_type in enumerate(down_block_types):
             input_channel = output_channel
             output_channel = block_out_channels[i]
             is_final_block = i == len(block_out_channels) - 1
 
@@ -146,46 +153,53 @@
                 out_channels=output_channel,
                 temb_channels=time_embed_dim,
                 add_downsample=not is_final_block,
                 resnet_eps=norm_eps,
                 resnet_act_fn=act_fn,
                 resnet_groups=norm_num_groups,
                 cross_attention_dim=cross_attention_dim,
-                attn_num_head_channels=attention_head_dim,
+                attn_num_head_channels=attention_head_dim[i],
                 downsample_padding=downsample_padding,
+                dual_cross_attention=dual_cross_attention,
+                use_linear_projection=use_linear_projection,
+                only_cross_attention=only_cross_attention[i],
             )
             self.down_blocks.append(down_block)
 
         # mid
         self.mid_block = UNetMidBlock2DCrossAttn(
             in_channels=block_out_channels[-1],
             temb_channels=time_embed_dim,
             resnet_eps=norm_eps,
             resnet_act_fn=act_fn,
             output_scale_factor=mid_block_scale_factor,
             resnet_time_scale_shift="default",
             cross_attention_dim=cross_attention_dim,
-            attn_num_head_channels=attention_head_dim,
+            attn_num_head_channels=attention_head_dim[-1],
             resnet_groups=norm_num_groups,
+            dual_cross_attention=dual_cross_attention,
+            use_linear_projection=use_linear_projection,
+            only_cross_attention=only_cross_attention[-1],
         )
 
         # count how many layers upsample the images
         self.num_upsamplers = 0
 
         # up
         reversed_block_out_channels = list(reversed(block_out_channels))
+        reversed_attention_head_dim = list(reversed(attention_head_dim))
+        reversed_only_cross_attention = list(reversed(only_cross_attention))
+
         output_channel = reversed_block_out_channels[0]
         for i, up_block_type in enumerate(up_block_types):
             is_final_block = i == len(block_out_channels) - 1
 
             prev_output_channel = output_channel
             output_channel = reversed_block_out_channels[i]
-            input_channel = reversed_block_out_channels[min(
-                i + 1,
-                len(block_out_channels) - 1)]
+            input_channel = reversed_block_out_channels[min(i + 1, len(block_out_channels) - 1)]
 
             # add upsample block for all BUT final layer
             if not is_final_block:
                 add_upsample = True
                 self.num_upsamplers += 1
             else:
                 add_upsample = False
@@ -198,62 +212,63 @@
                 prev_output_channel=prev_output_channel,
                 temb_channels=time_embed_dim,
                 add_upsample=add_upsample,
                 resnet_eps=norm_eps,
                 resnet_act_fn=act_fn,
                 resnet_groups=norm_num_groups,
                 cross_attention_dim=cross_attention_dim,
-                attn_num_head_channels=attention_head_dim,
+                attn_num_head_channels=reversed_attention_head_dim[i],
+                dual_cross_attention=dual_cross_attention,
+                use_linear_projection=use_linear_projection,
+                only_cross_attention=reversed_only_cross_attention[i],
             )
             self.up_blocks.append(up_block)
             prev_output_channel = output_channel
 
         # out
-        self.conv_norm_out = nn.GroupNorm(num_channels=block_out_channels[0],
-                                          num_groups=norm_num_groups,
-                                          epsilon=norm_eps)
+        self.conv_norm_out = nn.GroupNorm(
+            num_channels=block_out_channels[0], num_groups=norm_num_groups, epsilon=norm_eps
+        )
         self.conv_act = nn.Silu()
-        self.conv_out = nn.Conv2D(block_out_channels[0],
-                                  out_channels,
-                                  3,
-                                  padding=1)
+        self.conv_out = nn.Conv2D(block_out_channels[0], out_channels, 3, padding=1)
 
     def set_attention_slice(self, slice_size):
-        if slice_size is not None and self.config.attention_head_dim % slice_size != 0:
+        head_dims = self.config.attention_head_dim
+        head_dims = [head_dims] if isinstance(head_dims, int) else head_dims
+        if slice_size is not None and any(dim % slice_size != 0 for dim in head_dims):
             raise ValueError(
-                f"Make sure slice_size {slice_size} is a divisor of "
-                f"the number of heads used in cross_attention {self.config.attention_head_dim}"
+                f"Make sure slice_size {slice_size} is a common divisor of "
+                f"the number of heads used in cross_attention: {head_dims}"
             )
-        if slice_size is not None and slice_size > self.config.attention_head_dim:
+        if slice_size is not None and slice_size > min(head_dims):
             raise ValueError(
-                f"Chunk_size {slice_size} has to be smaller or equal to "
-                f"the number of heads used in cross_attention {self.config.attention_head_dim}"
+                f"slice_size {slice_size} has to be smaller or equal to "
+                f"the lowest number of heads used in cross_attention: min({head_dims}) = {min(head_dims)}"
             )
 
         for block in self.down_blocks:
             if hasattr(block, "attentions") and block.attentions is not None:
                 block.set_attention_slice(slice_size)
 
         self.mid_block.set_attention_slice(slice_size)
 
         for block in self.up_blocks:
             if hasattr(block, "attentions") and block.attentions is not None:
                 block.set_attention_slice(slice_size)
 
     def _set_gradient_checkpointing(self, module, value=False):
-        if isinstance(
-                module,
-            (CrossAttnDownBlock2D, DownBlock2D, CrossAttnUpBlock2D, UpBlock2D)):
+        if isinstance(module, (CrossAttnDownBlock2D, DownBlock2D, CrossAttnUpBlock2D, UpBlock2D)):
             module.gradient_checkpointing = value
 
     def forward(
         self,
         sample: paddle.Tensor,
         timestep: Union[paddle.Tensor, float, int],
         encoder_hidden_states: paddle.Tensor,
+        class_labels: Optional[paddle.Tensor] = None,
         return_dict: bool = True,
     ):
         r"""
         Args:
             sample (`paddle.Tensor`): (batch, channel, height, width) noisy inputs tensor
             timestep (`paddle.Tensor` or `float` or `int`): (batch) timesteps
             encoder_hidden_states (`paddle.Tensor`): (batch, channel, height, width) encoder hidden states
@@ -272,16 +287,15 @@
         default_overall_up_factor = 2**self.num_upsamplers
 
         # upsample size should be forwarded when sample is not a multiple of `default_overall_up_factor`
         forward_upsample_size = False
         upsample_size = None
 
         if any(s % default_overall_up_factor != 0 for s in sample.shape[-2:]):
-            logger.info(
-                "Forward upsample size to force interpolation output size.")
+            logger.info("Forward upsample size to force interpolation output size.")
             forward_upsample_size = True
 
         # 0. center input if necessary
         if self.config.center_input_sample:
             sample = 2 * sample - 1.0
 
         # 1. time
@@ -289,80 +303,80 @@
         if not paddle.is_tensor(timesteps):
             # TODO: this requires sync between CPU and GPU. So try to pass timesteps as tensors if you can
             timesteps = paddle.to_tensor([timesteps], dtype="int64")
         elif paddle.is_tensor(timesteps) and len(timesteps.shape) == 0:
             timesteps = timesteps[None]
 
         # broadcast to batch dimension in a way that's compatible with ONNX/Core ML
-        timesteps = timesteps.expand([
-            sample.shape[0],
-        ])
+        timesteps = timesteps.expand(
+            [
+                sample.shape[0],
+            ]
+        )
 
         t_emb = self.time_proj(timesteps)
 
         # timesteps does not contain any weights and will always return f32 tensors
         # but time_embedding might actually be running in fp16. so we need to cast here.
         # there might be better ways to encapsulate this.
-        t_emb = t_emb.astype(self.dtype)
+        t_emb = t_emb.cast(self.dtype)
         emb = self.time_embedding(t_emb)
 
+        if self.config.num_class_embeds is not None:
+            if class_labels is None:
+                raise ValueError("class_labels should be provided when num_class_embeds > 0")
+            class_emb = self.class_embedding(class_labels).cast(self.dtype)
+            emb = emb + class_emb
+
         # 2. pre-process
         sample = self.conv_in(sample)
 
         # 3. down
-        down_block_res_samples = (sample, )
+        down_block_res_samples = (sample,)
         for downsample_block in self.down_blocks:
-            if hasattr(
-                    downsample_block,
-                    "attentions") and downsample_block.attentions is not None:
+            if hasattr(downsample_block, "attentions") and downsample_block.attentions is not None:
                 sample, res_samples = downsample_block(
                     hidden_states=sample,
                     temb=emb,
                     encoder_hidden_states=encoder_hidden_states,
                 )
             else:
-                sample, res_samples = downsample_block(hidden_states=sample,
-                                                       temb=emb)
+                sample, res_samples = downsample_block(hidden_states=sample, temb=emb)
 
             down_block_res_samples += res_samples
 
         # 4. mid
-        sample = self.mid_block(sample,
-                                emb,
-                                encoder_hidden_states=encoder_hidden_states)
+        sample = self.mid_block(sample, emb, encoder_hidden_states=encoder_hidden_states)
 
         # 5. up
         for i, upsample_block in enumerate(self.up_blocks):
             is_final_block = i == len(self.up_blocks) - 1
 
-            res_samples = down_block_res_samples[-len(upsample_block.resnets):]
-            down_block_res_samples = down_block_res_samples[:-len(upsample_block
-                                                                  .resnets)]
+            res_samples = down_block_res_samples[-len(upsample_block.resnets) :]
+            down_block_res_samples = down_block_res_samples[: -len(upsample_block.resnets)]
 
             # if we have not reached the final block and need to forward the
             # upsample size, we do it here
             if not is_final_block and forward_upsample_size:
                 upsample_size = down_block_res_samples[-1].shape[2:]
 
-            if hasattr(upsample_block,
-                       "attentions") and upsample_block.attentions is not None:
+            if hasattr(upsample_block, "attentions") and upsample_block.attentions is not None:
                 sample = upsample_block(
                     hidden_states=sample,
                     temb=emb,
                     res_hidden_states_tuple=res_samples,
                     encoder_hidden_states=encoder_hidden_states,
                     upsample_size=upsample_size,
                 )
             else:
-                sample = upsample_block(hidden_states=sample,
-                                        temb=emb,
-                                        res_hidden_states_tuple=res_samples,
-                                        upsample_size=upsample_size)
+                sample = upsample_block(
+                    hidden_states=sample, temb=emb, res_hidden_states_tuple=res_samples, upsample_size=upsample_size
+                )
         # 6. post-process
         sample = self.conv_norm_out(sample)
         sample = self.conv_act(sample)
         sample = self.conv_out(sample)
 
         if not return_dict:
-            return (sample, )
+            return (sample,)
 
         return UNet2DConditionOutput(sample=sample)
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/models/unet_blocks.py` & `ppdiffusers-0.9.0/ppdiffusers/models/unet_2d_blocks.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,40 +8,47 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 import numpy as np
 import paddle
 from paddle import nn
-
-from .attention import AttentionBlock, SpatialTransformer
-from .resnet import Downsample2D, FirDownsample2D, FirUpsample2D, ResnetBlock2D, Upsample2D
 from paddle.distributed.fleet.utils import recompute
 
+from .attention import AttentionBlock, DualTransformer2DModel, Transformer2DModel
+from .resnet import (
+    Downsample2D,
+    FirDownsample2D,
+    FirUpsample2D,
+    ResnetBlock2D,
+    Upsample2D,
+)
+
 
 def get_down_block(
     down_block_type,
     num_layers,
     in_channels,
     out_channels,
     temb_channels,
     add_downsample,
     resnet_eps,
     resnet_act_fn,
     attn_num_head_channels,
     resnet_groups=None,
     cross_attention_dim=None,
     downsample_padding=None,
+    dual_cross_attention=False,
+    use_linear_projection=False,
+    only_cross_attention=False,
 ):
-    down_block_type = down_block_type[7:] if down_block_type.startswith(
-        "UNetRes") else down_block_type
+    down_block_type = down_block_type[7:] if down_block_type.startswith("UNetRes") else down_block_type
     if down_block_type == "DownBlock2D":
         return DownBlock2D(
             num_layers=num_layers,
             in_channels=in_channels,
             out_channels=out_channels,
             temb_channels=temb_channels,
             add_downsample=add_downsample,
@@ -61,29 +68,30 @@
             resnet_act_fn=resnet_act_fn,
             resnet_groups=resnet_groups,
             downsample_padding=downsample_padding,
             attn_num_head_channels=attn_num_head_channels,
         )
     elif down_block_type == "CrossAttnDownBlock2D":
         if cross_attention_dim is None:
-            raise ValueError(
-                "cross_attention_dim must be specified for CrossAttnDownBlock2D"
-            )
+            raise ValueError("cross_attention_dim must be specified for CrossAttnDownBlock2D")
         return CrossAttnDownBlock2D(
             num_layers=num_layers,
             in_channels=in_channels,
             out_channels=out_channels,
             temb_channels=temb_channels,
             add_downsample=add_downsample,
             resnet_eps=resnet_eps,
             resnet_act_fn=resnet_act_fn,
             resnet_groups=resnet_groups,
             downsample_padding=downsample_padding,
             cross_attention_dim=cross_attention_dim,
             attn_num_head_channels=attn_num_head_channels,
+            dual_cross_attention=dual_cross_attention,
+            use_linear_projection=use_linear_projection,
+            only_cross_attention=only_cross_attention,
         )
     elif down_block_type == "SkipDownBlock2D":
         return SkipDownBlock2D(
             num_layers=num_layers,
             in_channels=in_channels,
             out_channels=out_channels,
             temb_channels=temb_channels,
@@ -111,14 +119,27 @@
             out_channels=out_channels,
             add_downsample=add_downsample,
             resnet_eps=resnet_eps,
             resnet_act_fn=resnet_act_fn,
             resnet_groups=resnet_groups,
             downsample_padding=downsample_padding,
         )
+    elif down_block_type == "AttnDownEncoderBlock2D":
+        return AttnDownEncoderBlock2D(
+            num_layers=num_layers,
+            in_channels=in_channels,
+            out_channels=out_channels,
+            add_downsample=add_downsample,
+            resnet_eps=resnet_eps,
+            resnet_act_fn=resnet_act_fn,
+            resnet_groups=resnet_groups,
+            downsample_padding=downsample_padding,
+            attn_num_head_channels=attn_num_head_channels,
+        )
+    raise ValueError(f"{down_block_type} does not exist.")
 
 
 def get_up_block(
     up_block_type,
     num_layers,
     in_channels,
     out_channels,
@@ -126,45 +147,49 @@
     temb_channels,
     add_upsample,
     resnet_eps,
     resnet_act_fn,
     attn_num_head_channels,
     resnet_groups=None,
     cross_attention_dim=None,
+    dual_cross_attention=False,
+    use_linear_projection=False,
+    only_cross_attention=False,
 ):
-    up_block_type = up_block_type[7:] if up_block_type.startswith(
-        "UNetRes") else up_block_type
+    up_block_type = up_block_type[7:] if up_block_type.startswith("UNetRes") else up_block_type
     if up_block_type == "UpBlock2D":
         return UpBlock2D(
             num_layers=num_layers,
             in_channels=in_channels,
             out_channels=out_channels,
             prev_output_channel=prev_output_channel,
             temb_channels=temb_channels,
             add_upsample=add_upsample,
             resnet_eps=resnet_eps,
             resnet_act_fn=resnet_act_fn,
             resnet_groups=resnet_groups,
         )
     elif up_block_type == "CrossAttnUpBlock2D":
         if cross_attention_dim is None:
-            raise ValueError(
-                "cross_attention_dim must be specified for CrossAttnUpBlock2D")
+            raise ValueError("cross_attention_dim must be specified for CrossAttnUpBlock2D")
         return CrossAttnUpBlock2D(
             num_layers=num_layers,
             in_channels=in_channels,
             out_channels=out_channels,
             prev_output_channel=prev_output_channel,
             temb_channels=temb_channels,
             add_upsample=add_upsample,
             resnet_eps=resnet_eps,
             resnet_act_fn=resnet_act_fn,
             resnet_groups=resnet_groups,
             cross_attention_dim=cross_attention_dim,
             attn_num_head_channels=attn_num_head_channels,
+            dual_cross_attention=dual_cross_attention,
+            use_linear_projection=use_linear_projection,
+            only_cross_attention=only_cross_attention,
         )
     elif up_block_type == "AttnUpBlock2D":
         return AttnUpBlock2D(
             num_layers=num_layers,
             in_channels=in_channels,
             out_channels=out_channels,
             prev_output_channel=prev_output_channel,
@@ -204,40 +229,48 @@
             in_channels=in_channels,
             out_channels=out_channels,
             add_upsample=add_upsample,
             resnet_eps=resnet_eps,
             resnet_act_fn=resnet_act_fn,
             resnet_groups=resnet_groups,
         )
+    elif up_block_type == "AttnUpDecoderBlock2D":
+        return AttnUpDecoderBlock2D(
+            num_layers=num_layers,
+            in_channels=in_channels,
+            out_channels=out_channels,
+            add_upsample=add_upsample,
+            resnet_eps=resnet_eps,
+            resnet_act_fn=resnet_act_fn,
+            resnet_groups=resnet_groups,
+            attn_num_head_channels=attn_num_head_channels,
+        )
     raise ValueError(f"{up_block_type} does not exist.")
 
 
 class UNetMidBlock2D(nn.Layer):
-
     def __init__(
         self,
         in_channels: int,
         temb_channels: int,
         dropout: float = 0.0,
         num_layers: int = 1,
         resnet_eps: float = 1e-6,
         resnet_time_scale_shift: str = "default",
         resnet_act_fn: str = "swish",
         resnet_groups: int = 32,
         resnet_pre_norm: bool = True,
         attn_num_head_channels=1,
         attention_type="default",
         output_scale_factor=1.0,
-        **kwargs,
     ):
         super().__init__()
 
         self.attention_type = attention_type
-        resnet_groups = resnet_groups if resnet_groups is not None else min(
-            in_channels // 4, 32)
+        resnet_groups = resnet_groups if resnet_groups is not None else min(in_channels // 4, 32)
 
         # there is always at least one resnet
         resnets = [
             ResnetBlock2D(
                 in_channels=in_channels,
                 out_channels=in_channels,
                 temb_channels=temb_channels,
@@ -255,29 +288,31 @@
         for _ in range(num_layers):
             attentions.append(
                 AttentionBlock(
                     in_channels,
                     num_head_channels=attn_num_head_channels,
                     rescale_output_factor=output_scale_factor,
                     eps=resnet_eps,
-                    num_groups=resnet_groups,
-                ))
+                    norm_num_groups=resnet_groups,
+                )
+            )
             resnets.append(
                 ResnetBlock2D(
                     in_channels=in_channels,
                     out_channels=in_channels,
                     temb_channels=temb_channels,
                     eps=resnet_eps,
                     groups=resnet_groups,
                     dropout=dropout,
                     time_embedding_norm=resnet_time_scale_shift,
                     non_linearity=resnet_act_fn,
                     output_scale_factor=output_scale_factor,
                     pre_norm=resnet_pre_norm,
-                ))
+                )
+            )
 
         self.attentions = nn.LayerList(attentions)
         self.resnets = nn.LayerList(resnets)
 
     def forward(self, hidden_states, temb=None, encoder_states=None):
         hidden_states = self.resnets[0](hidden_states, temb)
         for attn, resnet in zip(self.attentions, self.resnets[1:]):
@@ -287,15 +322,14 @@
                 hidden_states = attn(hidden_states, encoder_states)
             hidden_states = resnet(hidden_states, temb)
 
         return hidden_states
 
 
 class UNetMidBlock2DCrossAttn(nn.Layer):
-
     def __init__(
         self,
         in_channels: int,
         temb_channels: int,
         dropout: float = 0.0,
         num_layers: int = 1,
         resnet_eps: float = 1e-6,
@@ -303,22 +337,23 @@
         resnet_act_fn: str = "swish",
         resnet_groups: int = 32,
         resnet_pre_norm: bool = True,
         attn_num_head_channels=1,
         attention_type="default",
         output_scale_factor=1.0,
         cross_attention_dim=1280,
-        **kwargs,
+        dual_cross_attention=False,
+        use_linear_projection=False,
+        only_cross_attention=False,
     ):
         super().__init__()
 
         self.attention_type = attention_type
         self.attn_num_head_channels = attn_num_head_channels
-        resnet_groups = resnet_groups if resnet_groups is not None else min(
-            in_channels // 4, 32)
+        resnet_groups = resnet_groups if resnet_groups is not None else min(in_channels // 4, 32)
 
         # there is always at least one resnet
         resnets = [
             ResnetBlock2D(
                 in_channels=in_channels,
                 out_channels=in_channels,
                 temb_channels=temb_channels,
@@ -330,66 +365,85 @@
                 output_scale_factor=output_scale_factor,
                 pre_norm=resnet_pre_norm,
             )
         ]
         attentions = []
 
         for _ in range(num_layers):
-            attentions.append(
-                SpatialTransformer(
-                    in_channels,
-                    attn_num_head_channels,
-                    in_channels // attn_num_head_channels,
-                    depth=1,
-                    context_dim=cross_attention_dim,
-                    num_groups=resnet_groups,
-                ))
+            if not dual_cross_attention:
+                attentions.append(
+                    Transformer2DModel(
+                        attn_num_head_channels,
+                        in_channels // attn_num_head_channels,
+                        in_channels=in_channels,
+                        num_layers=1,
+                        cross_attention_dim=cross_attention_dim,
+                        norm_num_groups=resnet_groups,
+                        use_linear_projection=use_linear_projection,
+                        only_cross_attention=only_cross_attention,
+                    )
+                )
+            else:
+                attentions.append(
+                    DualTransformer2DModel(
+                        attn_num_head_channels,
+                        in_channels // attn_num_head_channels,
+                        in_channels=in_channels,
+                        num_layers=1,
+                        cross_attention_dim=cross_attention_dim,
+                        norm_num_groups=resnet_groups,
+                        use_linear_projection=use_linear_projection,
+                        only_cross_attention=only_cross_attention,
+                    )
+                )
             resnets.append(
                 ResnetBlock2D(
                     in_channels=in_channels,
                     out_channels=in_channels,
                     temb_channels=temb_channels,
                     eps=resnet_eps,
                     groups=resnet_groups,
                     dropout=dropout,
                     time_embedding_norm=resnet_time_scale_shift,
                     non_linearity=resnet_act_fn,
                     output_scale_factor=output_scale_factor,
                     pre_norm=resnet_pre_norm,
-                ))
+                )
+            )
 
         self.attentions = nn.LayerList(attentions)
         self.resnets = nn.LayerList(resnets)
 
     def set_attention_slice(self, slice_size):
-        if slice_size is not None and self.attn_num_head_channels % slice_size != 0:
+        head_dims = self.attn_num_head_channels
+        head_dims = [head_dims] if isinstance(head_dims, int) else head_dims
+        if slice_size is not None and any(dim % slice_size != 0 for dim in head_dims):
             raise ValueError(
-                f"Make sure slice_size {slice_size} is a divisor of "
-                f"the number of heads used in cross_attention {self.attn_num_head_channels}"
+                f"Make sure slice_size {slice_size} is a common divisor of "
+                f"the number of heads used in cross_attention: {head_dims}"
             )
-        if slice_size is not None and slice_size > self.attn_num_head_channels:
+        if slice_size is not None and slice_size > min(head_dims):
             raise ValueError(
-                f"Chunk_size {slice_size} has to be smaller or equal to "
-                f"the number of heads used in cross_attention {self.attn_num_head_channels}"
+                f"slice_size {slice_size} has to be smaller or equal to "
+                f"the lowest number of heads used in cross_attention: min({head_dims}) = {min(head_dims)}"
             )
 
         for attn in self.attentions:
             attn._set_attention_slice(slice_size)
 
     def forward(self, hidden_states, temb=None, encoder_hidden_states=None):
         hidden_states = self.resnets[0](hidden_states, temb)
         for attn, resnet in zip(self.attentions, self.resnets[1:]):
-            hidden_states = attn(hidden_states, encoder_hidden_states)
+            hidden_states = attn(hidden_states, encoder_hidden_states).sample
             hidden_states = resnet(hidden_states, temb)
 
         return hidden_states
 
 
 class AttnDownBlock2D(nn.Layer):
-
     def __init__(
         self,
         in_channels: int,
         out_channels: int,
         temb_channels: int,
         dropout: float = 0.0,
         num_layers: int = 1,
@@ -420,57 +474,58 @@
                     eps=resnet_eps,
                     groups=resnet_groups,
                     dropout=dropout,
                     time_embedding_norm=resnet_time_scale_shift,
                     non_linearity=resnet_act_fn,
                     output_scale_factor=output_scale_factor,
                     pre_norm=resnet_pre_norm,
-                ))
+                )
+            )
             attentions.append(
                 AttentionBlock(
                     out_channels,
                     num_head_channels=attn_num_head_channels,
                     rescale_output_factor=output_scale_factor,
                     eps=resnet_eps,
-                    num_groups=resnet_groups,
-                ))
+                    norm_num_groups=resnet_groups,
+                )
+            )
 
         self.attentions = nn.LayerList(attentions)
         self.resnets = nn.LayerList(resnets)
 
         if add_downsample:
-            self.downsamplers = nn.LayerList([
-                Downsample2D(in_channels,
-                             use_conv=True,
-                             out_channels=out_channels,
-                             padding=downsample_padding,
-                             name="op")
-            ])
+            self.downsamplers = nn.LayerList(
+                [
+                    Downsample2D(
+                        out_channels, use_conv=True, out_channels=out_channels, padding=downsample_padding, name="op"
+                    )
+                ]
+            )
         else:
             self.downsamplers = None
 
     def forward(self, hidden_states, temb=None):
         output_states = ()
 
         for resnet, attn in zip(self.resnets, self.attentions):
             hidden_states = resnet(hidden_states, temb)
             hidden_states = attn(hidden_states)
-            output_states += (hidden_states, )
+            output_states += (hidden_states,)
 
         if self.downsamplers is not None:
             for downsampler in self.downsamplers:
                 hidden_states = downsampler(hidden_states)
 
-            output_states += (hidden_states, )
+            output_states += (hidden_states,)
 
         return hidden_states, output_states
 
 
 class CrossAttnDownBlock2D(nn.Layer):
-
     def __init__(
         self,
         in_channels: int,
         out_channels: int,
         temb_channels: int,
         dropout: float = 0.0,
         num_layers: int = 1,
@@ -481,14 +536,17 @@
         resnet_pre_norm: bool = True,
         attn_num_head_channels=1,
         cross_attention_dim=1280,
         attention_type="default",
         output_scale_factor=1.0,
         downsample_padding=1,
         add_downsample=True,
+        dual_cross_attention=False,
+        use_linear_projection=False,
+        only_cross_attention=False,
     ):
         super().__init__()
         resnets = []
         attentions = []
 
         self.attention_type = attention_type
         self.attn_num_head_channels = attn_num_head_channels
@@ -503,90 +561,110 @@
                     eps=resnet_eps,
                     groups=resnet_groups,
                     dropout=dropout,
                     time_embedding_norm=resnet_time_scale_shift,
                     non_linearity=resnet_act_fn,
                     output_scale_factor=output_scale_factor,
                     pre_norm=resnet_pre_norm,
-                ))
-            attentions.append(
-                SpatialTransformer(
-                    out_channels,
-                    attn_num_head_channels,
-                    out_channels // attn_num_head_channels,
-                    depth=1,
-                    context_dim=cross_attention_dim,
-                    num_groups=resnet_groups,
-                ))
+                )
+            )
+            if not dual_cross_attention:
+                attentions.append(
+                    Transformer2DModel(
+                        attn_num_head_channels,
+                        out_channels // attn_num_head_channels,
+                        in_channels=out_channels,
+                        num_layers=1,
+                        cross_attention_dim=cross_attention_dim,
+                        norm_num_groups=resnet_groups,
+                        use_linear_projection=use_linear_projection,
+                        only_cross_attention=only_cross_attention,
+                    )
+                )
+            else:
+                attentions.append(
+                    DualTransformer2DModel(
+                        attn_num_head_channels,
+                        out_channels // attn_num_head_channels,
+                        in_channels=out_channels,
+                        num_layers=1,
+                        cross_attention_dim=cross_attention_dim,
+                        norm_num_groups=resnet_groups,
+                        use_linear_projection=use_linear_projection,
+                        only_cross_attention=only_cross_attention,
+                    )
+                )
         self.attentions = nn.LayerList(attentions)
         self.resnets = nn.LayerList(resnets)
 
         if add_downsample:
-            self.downsamplers = nn.LayerList([
-                Downsample2D(in_channels,
-                             use_conv=True,
-                             out_channels=out_channels,
-                             padding=downsample_padding,
-                             name="op")
-            ])
+            self.downsamplers = nn.LayerList(
+                [
+                    Downsample2D(
+                        out_channels, use_conv=True, out_channels=out_channels, padding=downsample_padding, name="op"
+                    )
+                ]
+            )
         else:
             self.downsamplers = None
 
         self.gradient_checkpointing = False
 
     def set_attention_slice(self, slice_size):
-        if slice_size is not None and self.attn_num_head_channels % slice_size != 0:
+        head_dims = self.attn_num_head_channels
+        head_dims = [head_dims] if isinstance(head_dims, int) else head_dims
+        if slice_size is not None and any(dim % slice_size != 0 for dim in head_dims):
             raise ValueError(
-                f"Make sure slice_size {slice_size} is a divisor of "
-                f"the number of heads used in cross_attention {self.attn_num_head_channels}"
+                f"Make sure slice_size {slice_size} is a common divisor of "
+                f"the number of heads used in cross_attention: {head_dims}"
             )
-        if slice_size is not None and slice_size > self.attn_num_head_channels:
+        if slice_size is not None and slice_size > min(head_dims):
             raise ValueError(
-                f"Chunk_size {slice_size} has to be smaller or equal to "
-                f"the number of heads used in cross_attention {self.attn_num_head_channels}"
+                f"slice_size {slice_size} has to be smaller or equal to "
+                f"the lowest number of heads used in cross_attention: min({head_dims}) = {min(head_dims)}"
             )
 
         for attn in self.attentions:
             attn._set_attention_slice(slice_size)
 
     def forward(self, hidden_states, temb=None, encoder_hidden_states=None):
         output_states = ()
 
         for resnet, attn in zip(self.resnets, self.attentions):
             if self.training and self.gradient_checkpointing:
 
-                def create_custom_forward(module):
-
+                def create_custom_forward(module, return_dict=None):
                     def custom_forward(*inputs):
-                        return module(*inputs)
+                        if return_dict is not None:
+                            return module(*inputs, return_dict=return_dict)[0]  # move [0]
+                        else:
+                            return module(*inputs)
 
                     return custom_forward
 
-                hidden_states = recompute(create_custom_forward(resnet),
-                                          hidden_states, temb)
-                hidden_states = recompute(create_custom_forward(attn),
-                                          hidden_states, encoder_hidden_states)
+                hidden_states = recompute(create_custom_forward(resnet), hidden_states, temb)
+                hidden_states = recompute(
+                    create_custom_forward(attn, return_dict=False), hidden_states, encoder_hidden_states
+                )  # [0]
             else:
                 hidden_states = resnet(hidden_states, temb)
-                hidden_states = attn(hidden_states,
-                                     context=encoder_hidden_states)
+                hidden_states = attn(hidden_states, encoder_hidden_states=encoder_hidden_states).sample
 
-            output_states += (hidden_states, )
+            output_states += (hidden_states,)
 
         if self.downsamplers is not None:
             for downsampler in self.downsamplers:
                 hidden_states = downsampler(hidden_states)
 
-            output_states += (hidden_states, )
+            output_states += (hidden_states,)
 
         return hidden_states, output_states
 
 
 class DownBlock2D(nn.Layer):
-
     def __init__(
         self,
         in_channels: int,
         out_channels: int,
         temb_channels: int,
         dropout: float = 0.0,
         num_layers: int = 1,
@@ -612,62 +690,60 @@
                     eps=resnet_eps,
                     groups=resnet_groups,
                     dropout=dropout,
                     time_embedding_norm=resnet_time_scale_shift,
                     non_linearity=resnet_act_fn,
                     output_scale_factor=output_scale_factor,
                     pre_norm=resnet_pre_norm,
-                ))
+                )
+            )
 
         self.resnets = nn.LayerList(resnets)
 
         if add_downsample:
-            self.downsamplers = nn.LayerList([
-                Downsample2D(in_channels,
-                             use_conv=True,
-                             out_channels=out_channels,
-                             padding=downsample_padding,
-                             name="op")
-            ])
+            self.downsamplers = nn.LayerList(
+                [
+                    Downsample2D(
+                        out_channels, use_conv=True, out_channels=out_channels, padding=downsample_padding, name="op"
+                    )
+                ]
+            )
         else:
             self.downsamplers = None
 
         self.gradient_checkpointing = False
 
     def forward(self, hidden_states, temb=None):
         output_states = ()
 
         for resnet in self.resnets:
             if self.training and self.gradient_checkpointing:
 
                 def create_custom_forward(module):
-
                     def custom_forward(*inputs):
                         return module(*inputs)
 
                     return custom_forward
 
-                hidden_states = recompute(create_custom_forward(resnet),
-                                          hidden_states, temb)
+                hidden_states = recompute(create_custom_forward(resnet), hidden_states, temb)
             else:
                 hidden_states = resnet(hidden_states, temb)
 
-            output_states += (hidden_states, )
+            output_states += (hidden_states,)
 
         if self.downsamplers is not None:
             for downsampler in self.downsamplers:
                 hidden_states = downsampler(hidden_states)
 
-            output_states += (hidden_states, )
+            output_states += (hidden_states,)
 
         return hidden_states, output_states
 
 
 class DownEncoderBlock2D(nn.Layer):
-
     def __init__(
         self,
         in_channels: int,
         out_channels: int,
         dropout: float = 0.0,
         num_layers: int = 1,
         resnet_eps: float = 1e-6,
@@ -692,26 +768,27 @@
                     eps=resnet_eps,
                     groups=resnet_groups,
                     dropout=dropout,
                     time_embedding_norm=resnet_time_scale_shift,
                     non_linearity=resnet_act_fn,
                     output_scale_factor=output_scale_factor,
                     pre_norm=resnet_pre_norm,
-                ))
+                )
+            )
 
         self.resnets = nn.LayerList(resnets)
 
         if add_downsample:
-            self.downsamplers = nn.LayerList([
-                Downsample2D(in_channels,
-                             use_conv=True,
-                             out_channels=out_channels,
-                             padding=downsample_padding,
-                             name="op")
-            ])
+            self.downsamplers = nn.LayerList(
+                [
+                    Downsample2D(
+                        out_channels, use_conv=True, out_channels=out_channels, padding=downsample_padding, name="op"
+                    )
+                ]
+            )
         else:
             self.downsamplers = None
 
     def forward(self, hidden_states):
         for resnet in self.resnets:
             hidden_states = resnet(hidden_states, temb=None)
 
@@ -719,15 +796,14 @@
             for downsampler in self.downsamplers:
                 hidden_states = downsampler(hidden_states)
 
         return hidden_states
 
 
 class AttnDownEncoderBlock2D(nn.Layer):
-
     def __init__(
         self,
         in_channels: int,
         out_channels: int,
         dropout: float = 0.0,
         num_layers: int = 1,
         resnet_eps: float = 1e-6,
@@ -754,35 +830,37 @@
                     eps=resnet_eps,
                     groups=resnet_groups,
                     dropout=dropout,
                     time_embedding_norm=resnet_time_scale_shift,
                     non_linearity=resnet_act_fn,
                     output_scale_factor=output_scale_factor,
                     pre_norm=resnet_pre_norm,
-                ))
+                )
+            )
             attentions.append(
                 AttentionBlock(
                     out_channels,
                     num_head_channels=attn_num_head_channels,
                     rescale_output_factor=output_scale_factor,
                     eps=resnet_eps,
-                    num_groups=resnet_groups,
-                ))
+                    norm_num_groups=resnet_groups,
+                )
+            )
 
         self.attentions = nn.LayerList(attentions)
         self.resnets = nn.LayerList(resnets)
 
         if add_downsample:
-            self.downsamplers = nn.LayerList([
-                Downsample2D(in_channels,
-                             use_conv=True,
-                             out_channels=out_channels,
-                             padding=downsample_padding,
-                             name="op")
-            ])
+            self.downsamplers = nn.LayerList(
+                [
+                    Downsample2D(
+                        out_channels, use_conv=True, out_channels=out_channels, padding=downsample_padding, name="op"
+                    )
+                ]
+            )
         else:
             self.downsamplers = None
 
     def forward(self, hidden_states):
         for resnet, attn in zip(self.resnets, self.attentions):
             hidden_states = resnet(hidden_states, temb=None)
             hidden_states = attn(hidden_states)
@@ -791,15 +869,14 @@
             for downsampler in self.downsamplers:
                 hidden_states = downsampler(hidden_states)
 
         return hidden_states
 
 
 class AttnSkipDownBlock2D(nn.Layer):
-
     def __init__(
         self,
         in_channels: int,
         out_channels: int,
         temb_channels: int,
         dropout: float = 0.0,
         num_layers: int = 1,
@@ -830,22 +907,24 @@
                     groups=min(in_channels // 4, 32),
                     groups_out=min(out_channels // 4, 32),
                     dropout=dropout,
                     time_embedding_norm=resnet_time_scale_shift,
                     non_linearity=resnet_act_fn,
                     output_scale_factor=output_scale_factor,
                     pre_norm=resnet_pre_norm,
-                ))
+                )
+            )
             self.attentions.append(
                 AttentionBlock(
                     out_channels,
                     num_head_channels=attn_num_head_channels,
                     rescale_output_factor=output_scale_factor,
                     eps=resnet_eps,
-                ))
+                )
+            )
 
         if add_downsample:
             self.resnet_down = ResnetBlock2D(
                 in_channels=out_channels,
                 out_channels=out_channels,
                 temb_channels=temb_channels,
                 eps=resnet_eps,
@@ -855,47 +934,42 @@
                 non_linearity=resnet_act_fn,
                 output_scale_factor=output_scale_factor,
                 pre_norm=resnet_pre_norm,
                 use_in_shortcut=True,
                 down=True,
                 kernel="fir",
             )
-            self.downsamplers = nn.LayerList(
-                [FirDownsample2D(in_channels, out_channels=out_channels)])
-            self.skip_conv = nn.Conv2D(3,
-                                       out_channels,
-                                       kernel_size=(1, 1),
-                                       stride=(1, 1))
+            self.downsamplers = nn.LayerList([FirDownsample2D(out_channels, out_channels=out_channels)])
+            self.skip_conv = nn.Conv2D(3, out_channels, kernel_size=(1, 1), stride=(1, 1))
         else:
             self.resnet_down = None
             self.downsamplers = None
             self.skip_conv = None
 
     def forward(self, hidden_states, temb=None, skip_sample=None):
         output_states = ()
 
         for resnet, attn in zip(self.resnets, self.attentions):
             hidden_states = resnet(hidden_states, temb)
             hidden_states = attn(hidden_states)
-            output_states += (hidden_states, )
+            output_states += (hidden_states,)
 
         if self.downsamplers is not None:
             hidden_states = self.resnet_down(hidden_states, temb)
             for downsampler in self.downsamplers:
                 skip_sample = downsampler(skip_sample)
 
             hidden_states = self.skip_conv(skip_sample) + hidden_states
 
-            output_states += (hidden_states, )
+            output_states += (hidden_states,)
 
         return hidden_states, output_states, skip_sample
 
 
 class SkipDownBlock2D(nn.Layer):
-
     def __init__(
         self,
         in_channels: int,
         out_channels: int,
         temb_channels: int,
         dropout: float = 0.0,
         num_layers: int = 1,
@@ -921,15 +995,16 @@
                     groups=min(in_channels // 4, 32),
                     groups_out=min(out_channels // 4, 32),
                     dropout=dropout,
                     time_embedding_norm=resnet_time_scale_shift,
                     non_linearity=resnet_act_fn,
                     output_scale_factor=output_scale_factor,
                     pre_norm=resnet_pre_norm,
-                ))
+                )
+            )
 
         if add_downsample:
             self.resnet_down = ResnetBlock2D(
                 in_channels=out_channels,
                 out_channels=out_channels,
                 temb_channels=temb_channels,
                 eps=resnet_eps,
@@ -939,46 +1014,41 @@
                 non_linearity=resnet_act_fn,
                 output_scale_factor=output_scale_factor,
                 pre_norm=resnet_pre_norm,
                 use_in_shortcut=True,
                 down=True,
                 kernel="fir",
             )
-            self.downsamplers = nn.LayerList(
-                [FirDownsample2D(in_channels, out_channels=out_channels)])
-            self.skip_conv = nn.Conv2D(3,
-                                       out_channels,
-                                       kernel_size=(1, 1),
-                                       stride=(1, 1))
+            self.downsamplers = nn.LayerList([FirDownsample2D(out_channels, out_channels=out_channels)])
+            self.skip_conv = nn.Conv2D(3, out_channels, kernel_size=(1, 1), stride=(1, 1))
         else:
             self.resnet_down = None
             self.downsamplers = None
             self.skip_conv = None
 
     def forward(self, hidden_states, temb=None, skip_sample=None):
         output_states = ()
 
         for resnet in self.resnets:
             hidden_states = resnet(hidden_states, temb)
-            output_states += (hidden_states, )
+            output_states += (hidden_states,)
 
         if self.downsamplers is not None:
             hidden_states = self.resnet_down(hidden_states, temb)
             for downsampler in self.downsamplers:
                 skip_sample = downsampler(skip_sample)
 
             hidden_states = self.skip_conv(skip_sample) + hidden_states
 
-            output_states += (hidden_states, )
+            output_states += (hidden_states,)
 
         return hidden_states, output_states, skip_sample
 
 
 class AttnUpBlock2D(nn.Layer):
-
     def __init__(
         self,
         in_channels: int,
         prev_output_channel: int,
         out_channels: int,
         temb_channels: int,
         dropout: float = 0.0,
@@ -996,72 +1066,67 @@
         super().__init__()
         resnets = []
         attentions = []
 
         self.attention_type = attention_type
 
         for i in range(num_layers):
-            res_skip_channels = in_channels if (i == num_layers -
-                                                1) else out_channels
+            res_skip_channels = in_channels if (i == num_layers - 1) else out_channels
             resnet_in_channels = prev_output_channel if i == 0 else out_channels
 
             resnets.append(
                 ResnetBlock2D(
                     in_channels=resnet_in_channels + res_skip_channels,
                     out_channels=out_channels,
                     temb_channels=temb_channels,
                     eps=resnet_eps,
                     groups=resnet_groups,
                     dropout=dropout,
                     time_embedding_norm=resnet_time_scale_shift,
                     non_linearity=resnet_act_fn,
                     output_scale_factor=output_scale_factor,
                     pre_norm=resnet_pre_norm,
-                ))
+                )
+            )
             attentions.append(
                 AttentionBlock(
                     out_channels,
                     num_head_channels=attn_num_head_channels,
                     rescale_output_factor=output_scale_factor,
                     eps=resnet_eps,
-                    num_groups=resnet_groups,
-                ))
+                    norm_num_groups=resnet_groups,
+                )
+            )
 
         self.attentions = nn.LayerList(attentions)
         self.resnets = nn.LayerList(resnets)
 
         if add_upsample:
-            self.upsamplers = nn.LayerList([
-                Upsample2D(out_channels,
-                           use_conv=True,
-                           out_channels=out_channels)
-            ])
+            self.upsamplers = nn.LayerList([Upsample2D(out_channels, use_conv=True, out_channels=out_channels)])
         else:
             self.upsamplers = None
 
     def forward(self, hidden_states, res_hidden_states_tuple, temb=None):
         for resnet, attn in zip(self.resnets, self.attentions):
             # pop res hidden states
             res_hidden_states = res_hidden_states_tuple[-1]
             res_hidden_states_tuple = res_hidden_states_tuple[:-1]
-            hidden_states = paddle.concat([hidden_states, res_hidden_states],
-                                          axis=1)
+            hidden_states = paddle.concat([hidden_states, res_hidden_states], axis=1)
 
             hidden_states = resnet(hidden_states, temb)
             hidden_states = attn(hidden_states)
 
         if self.upsamplers is not None:
             for upsampler in self.upsamplers:
                 hidden_states = upsampler(hidden_states)
 
         return hidden_states
 
 
 class CrossAttnUpBlock2D(nn.Layer):
-
     def __init__(
         self,
         in_channels: int,
         out_channels: int,
         prev_output_channel: int,
         temb_channels: int,
         dropout: float = 0.0,
@@ -1071,75 +1136,92 @@
         resnet_act_fn: str = "swish",
         resnet_groups: int = 32,
         resnet_pre_norm: bool = True,
         attn_num_head_channels=1,
         cross_attention_dim=1280,
         attention_type="default",
         output_scale_factor=1.0,
-        downsample_padding=1,
         add_upsample=True,
+        dual_cross_attention=False,
+        use_linear_projection=False,
+        only_cross_attention=False,
     ):
         super().__init__()
         resnets = []
         attentions = []
 
         self.attention_type = attention_type
         self.attn_num_head_channels = attn_num_head_channels
 
         for i in range(num_layers):
-            res_skip_channels = in_channels if (i == num_layers -
-                                                1) else out_channels
+            res_skip_channels = in_channels if (i == num_layers - 1) else out_channels
             resnet_in_channels = prev_output_channel if i == 0 else out_channels
 
             resnets.append(
                 ResnetBlock2D(
                     in_channels=resnet_in_channels + res_skip_channels,
                     out_channels=out_channels,
                     temb_channels=temb_channels,
                     eps=resnet_eps,
                     groups=resnet_groups,
                     dropout=dropout,
                     time_embedding_norm=resnet_time_scale_shift,
                     non_linearity=resnet_act_fn,
                     output_scale_factor=output_scale_factor,
                     pre_norm=resnet_pre_norm,
-                ))
-            attentions.append(
-                SpatialTransformer(
-                    out_channels,
-                    attn_num_head_channels,
-                    out_channels // attn_num_head_channels,
-                    depth=1,
-                    context_dim=cross_attention_dim,
-                    num_groups=resnet_groups,
-                ))
+                )
+            )
+            if not dual_cross_attention:
+                attentions.append(
+                    Transformer2DModel(
+                        attn_num_head_channels,
+                        out_channels // attn_num_head_channels,
+                        in_channels=out_channels,
+                        num_layers=1,
+                        cross_attention_dim=cross_attention_dim,
+                        norm_num_groups=resnet_groups,
+                        use_linear_projection=use_linear_projection,
+                        only_cross_attention=only_cross_attention,
+                    )
+                )
+            else:
+                attentions.append(
+                    DualTransformer2DModel(
+                        attn_num_head_channels,
+                        out_channels // attn_num_head_channels,
+                        in_channels=out_channels,
+                        num_layers=1,
+                        cross_attention_dim=cross_attention_dim,
+                        norm_num_groups=resnet_groups,
+                        use_linear_projection=use_linear_projection,
+                        only_cross_attention=only_cross_attention,
+                    )
+                )
         self.attentions = nn.LayerList(attentions)
         self.resnets = nn.LayerList(resnets)
 
         if add_upsample:
-            self.upsamplers = nn.LayerList([
-                Upsample2D(out_channels,
-                           use_conv=True,
-                           out_channels=out_channels)
-            ])
+            self.upsamplers = nn.LayerList([Upsample2D(out_channels, use_conv=True, out_channels=out_channels)])
         else:
             self.upsamplers = None
 
         self.gradient_checkpointing = False
 
     def set_attention_slice(self, slice_size):
-        if slice_size is not None and self.attn_num_head_channels % slice_size != 0:
+        head_dims = self.attn_num_head_channels
+        head_dims = [head_dims] if isinstance(head_dims, int) else head_dims
+        if slice_size is not None and any(dim % slice_size != 0 for dim in head_dims):
             raise ValueError(
-                f"Make sure slice_size {slice_size} is a divisor of "
-                f"the number of heads used in cross_attention {self.attn_num_head_channels}"
+                f"Make sure slice_size {slice_size} is a common divisor of "
+                f"the number of heads used in cross_attention: {head_dims}"
             )
-        if slice_size is not None and slice_size > self.attn_num_head_channels:
+        if slice_size is not None and slice_size > min(head_dims):
             raise ValueError(
-                f"Chunk_size {slice_size} has to be smaller or equal to "
-                f"the number of heads used in cross_attention {self.attn_num_head_channels}"
+                f"slice_size {slice_size} has to be smaller or equal to "
+                f"the lowest number of heads used in cross_attention: min({head_dims}) = {min(head_dims)}"
             )
 
         for attn in self.attentions:
             attn._set_attention_slice(slice_size)
 
         self.gradient_checkpointing = False
 
@@ -1151,44 +1233,42 @@
         encoder_hidden_states=None,
         upsample_size=None,
     ):
         for resnet, attn in zip(self.resnets, self.attentions):
             # pop res hidden states
             res_hidden_states = res_hidden_states_tuple[-1]
             res_hidden_states_tuple = res_hidden_states_tuple[:-1]
-            hidden_states = paddle.concat([hidden_states, res_hidden_states],
-                                          axis=1)
-
+            hidden_states = paddle.concat([hidden_states, res_hidden_states], axis=1)
             if self.training and self.gradient_checkpointing:
 
-                def create_custom_forward(module):
-
+                def create_custom_forward(module, return_dict=None):
                     def custom_forward(*inputs):
-                        return module(*inputs)
+                        if return_dict is not None:
+                            return module(*inputs, return_dict=return_dict)[0]  # move [0]
+                        else:
+                            return module(*inputs)
 
                     return custom_forward
 
-                hidden_states = recompute(create_custom_forward(resnet),
-                                          hidden_states, temb)
-                hidden_states = recompute(create_custom_forward(attn),
-                                          hidden_states, encoder_hidden_states)
+                hidden_states = recompute(create_custom_forward(resnet), hidden_states, temb)
+                hidden_states = recompute(
+                    create_custom_forward(attn, return_dict=False), hidden_states, encoder_hidden_states
+                )  # [0]
             else:
                 hidden_states = resnet(hidden_states, temb)
-                hidden_states = attn(hidden_states,
-                                     context=encoder_hidden_states)
+                hidden_states = attn(hidden_states, encoder_hidden_states=encoder_hidden_states).sample
 
         if self.upsamplers is not None:
             for upsampler in self.upsamplers:
                 hidden_states = upsampler(hidden_states, upsample_size)
 
         return hidden_states
 
 
 class UpBlock2D(nn.Layer):
-
     def __init__(
         self,
         in_channels: int,
         prev_output_channel: int,
         out_channels: int,
         temb_channels: int,
         dropout: float = 0.0,
@@ -1201,80 +1281,67 @@
         output_scale_factor=1.0,
         add_upsample=True,
     ):
         super().__init__()
         resnets = []
 
         for i in range(num_layers):
-            res_skip_channels = in_channels if (i == num_layers -
-                                                1) else out_channels
+            res_skip_channels = in_channels if (i == num_layers - 1) else out_channels
             resnet_in_channels = prev_output_channel if i == 0 else out_channels
 
             resnets.append(
                 ResnetBlock2D(
                     in_channels=resnet_in_channels + res_skip_channels,
                     out_channels=out_channels,
                     temb_channels=temb_channels,
                     eps=resnet_eps,
                     groups=resnet_groups,
                     dropout=dropout,
                     time_embedding_norm=resnet_time_scale_shift,
                     non_linearity=resnet_act_fn,
                     output_scale_factor=output_scale_factor,
                     pre_norm=resnet_pre_norm,
-                ))
+                )
+            )
 
         self.resnets = nn.LayerList(resnets)
 
         if add_upsample:
-            self.upsamplers = nn.LayerList([
-                Upsample2D(out_channels,
-                           use_conv=True,
-                           out_channels=out_channels)
-            ])
+            self.upsamplers = nn.LayerList([Upsample2D(out_channels, use_conv=True, out_channels=out_channels)])
         else:
             self.upsamplers = None
 
         self.gradient_checkpointing = False
 
-    def forward(self,
-                hidden_states,
-                res_hidden_states_tuple,
-                temb=None,
-                upsample_size=None):
+    def forward(self, hidden_states, res_hidden_states_tuple, temb=None, upsample_size=None):
         for resnet in self.resnets:
             # pop res hidden states
             res_hidden_states = res_hidden_states_tuple[-1]
             res_hidden_states_tuple = res_hidden_states_tuple[:-1]
-            hidden_states = paddle.concat([hidden_states, res_hidden_states],
-                                          axis=1)
-
+            hidden_states = paddle.concat([hidden_states, res_hidden_states], axis=1)
             if self.training and self.gradient_checkpointing:
 
                 def create_custom_forward(module):
-
                     def custom_forward(*inputs):
                         return module(*inputs)
 
                     return custom_forward
 
-                hidden_states = recompute(create_custom_forward(resnet),
-                                          hidden_states, temb)
+                hidden_states = recompute(create_custom_forward(resnet), hidden_states, temb)
             else:
                 hidden_states = resnet(hidden_states, temb)
 
         if self.upsamplers is not None:
             for upsampler in self.upsamplers:
                 hidden_states = upsampler(hidden_states, upsample_size)
 
         return hidden_states
 
 
 class UpDecoderBlock2D(nn.Layer):
-
     def __init__(
         self,
         in_channels: int,
         out_channels: int,
         dropout: float = 0.0,
         num_layers: int = 1,
         resnet_eps: float = 1e-6,
@@ -1299,24 +1366,21 @@
                     eps=resnet_eps,
                     groups=resnet_groups,
                     dropout=dropout,
                     time_embedding_norm=resnet_time_scale_shift,
                     non_linearity=resnet_act_fn,
                     output_scale_factor=output_scale_factor,
                     pre_norm=resnet_pre_norm,
-                ))
+                )
+            )
 
         self.resnets = nn.LayerList(resnets)
 
         if add_upsample:
-            self.upsamplers = nn.LayerList([
-                Upsample2D(out_channels,
-                           use_conv=True,
-                           out_channels=out_channels)
-            ])
+            self.upsamplers = nn.LayerList([Upsample2D(out_channels, use_conv=True, out_channels=out_channels)])
         else:
             self.upsamplers = None
 
     def forward(self, hidden_states):
         for resnet in self.resnets:
             hidden_states = resnet(hidden_states, temb=None)
 
@@ -1324,15 +1388,14 @@
             for upsampler in self.upsamplers:
                 hidden_states = upsampler(hidden_states)
 
         return hidden_states
 
 
 class AttnUpDecoderBlock2D(nn.Layer):
-
     def __init__(
         self,
         in_channels: int,
         out_channels: int,
         dropout: float = 0.0,
         num_layers: int = 1,
         resnet_eps: float = 1e-6,
@@ -1359,33 +1422,31 @@
                     eps=resnet_eps,
                     groups=resnet_groups,
                     dropout=dropout,
                     time_embedding_norm=resnet_time_scale_shift,
                     non_linearity=resnet_act_fn,
                     output_scale_factor=output_scale_factor,
                     pre_norm=resnet_pre_norm,
-                ))
+                )
+            )
             attentions.append(
                 AttentionBlock(
                     out_channels,
                     num_head_channels=attn_num_head_channels,
                     rescale_output_factor=output_scale_factor,
                     eps=resnet_eps,
-                    num_groups=resnet_groups,
-                ))
+                    norm_num_groups=resnet_groups,
+                )
+            )
 
         self.attentions = nn.LayerList(attentions)
         self.resnets = nn.LayerList(resnets)
 
         if add_upsample:
-            self.upsamplers = nn.LayerList([
-                Upsample2D(out_channels,
-                           use_conv=True,
-                           out_channels=out_channels)
-            ])
+            self.upsamplers = nn.LayerList([Upsample2D(out_channels, use_conv=True, out_channels=out_channels)])
         else:
             self.upsamplers = None
 
     def forward(self, hidden_states):
         for resnet, attn in zip(self.resnets, self.attentions):
             hidden_states = resnet(hidden_states, temb=None)
             hidden_states = attn(hidden_states)
@@ -1394,15 +1455,14 @@
             for upsampler in self.upsamplers:
                 hidden_states = upsampler(hidden_states)
 
         return hidden_states
 
 
 class AttnSkipUpBlock2D(nn.Layer):
-
     def __init__(
         self,
         in_channels: int,
         prev_output_channel: int,
         out_channels: int,
         temb_channels: int,
         dropout: float = 0.0,
@@ -1420,16 +1480,15 @@
         super().__init__()
         self.attentions = nn.LayerList([])
         self.resnets = nn.LayerList([])
 
         self.attention_type = attention_type
 
         for i in range(num_layers):
-            res_skip_channels = in_channels if (i == num_layers -
-                                                1) else out_channels
+            res_skip_channels = in_channels if (i == num_layers - 1) else out_channels
             resnet_in_channels = prev_output_channel if i == 0 else out_channels
 
             self.resnets.append(
                 ResnetBlock2D(
                     in_channels=resnet_in_channels + res_skip_channels,
                     out_channels=out_channels,
                     temb_channels=temb_channels,
@@ -1437,23 +1496,25 @@
                     groups=min(resnet_in_channels + res_skip_channels // 4, 32),
                     groups_out=min(out_channels // 4, 32),
                     dropout=dropout,
                     time_embedding_norm=resnet_time_scale_shift,
                     non_linearity=resnet_act_fn,
                     output_scale_factor=output_scale_factor,
                     pre_norm=resnet_pre_norm,
-                ))
+                )
+            )
 
         self.attentions.append(
             AttentionBlock(
                 out_channels,
                 num_head_channels=attn_num_head_channels,
                 rescale_output_factor=output_scale_factor,
                 eps=resnet_eps,
-            ))
+            )
+        )
 
         self.upsampler = FirUpsample2D(in_channels, out_channels=out_channels)
         if add_upsample:
             self.resnet_up = ResnetBlock2D(
                 in_channels=out_channels,
                 out_channels=out_channels,
                 temb_channels=temb_channels,
@@ -1465,41 +1526,31 @@
                 non_linearity=resnet_act_fn,
                 output_scale_factor=output_scale_factor,
                 pre_norm=resnet_pre_norm,
                 use_in_shortcut=True,
                 up=True,
                 kernel="fir",
             )
-            self.skip_conv = nn.Conv2D(out_channels,
-                                       3,
-                                       kernel_size=(3, 3),
-                                       stride=(1, 1),
-                                       padding=(1, 1))
-            self.skip_norm = nn.GroupNorm(num_groups=min(out_channels // 4, 32),
-                                          num_channels=out_channels,
-                                          epsilon=resnet_eps)
+            self.skip_conv = nn.Conv2D(out_channels, 3, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+            self.skip_norm = nn.GroupNorm(
+                num_groups=min(out_channels // 4, 32), num_channels=out_channels, epsilon=resnet_eps
+            )
             self.act = nn.Silu()
         else:
             self.resnet_up = None
             self.skip_conv = None
             self.skip_norm = None
             self.act = None
 
-    def forward(self,
-                hidden_states,
-                res_hidden_states_tuple,
-                temb=None,
-                skip_sample=None):
+    def forward(self, hidden_states, res_hidden_states_tuple, temb=None, skip_sample=None):
         for resnet in self.resnets:
             # pop res hidden states
             res_hidden_states = res_hidden_states_tuple[-1]
             res_hidden_states_tuple = res_hidden_states_tuple[:-1]
-            hidden_states = paddle.concat([hidden_states, res_hidden_states],
-                                          axis=1)
-
+            hidden_states = paddle.concat([hidden_states, res_hidden_states], axis=1)
             hidden_states = resnet(hidden_states, temb)
 
         hidden_states = self.attentions[0](hidden_states)
 
         if skip_sample is not None:
             skip_sample = self.upsampler(skip_sample)
         else:
@@ -1514,15 +1565,14 @@
 
             hidden_states = self.resnet_up(hidden_states, temb)
 
         return hidden_states, skip_sample
 
 
 class SkipUpBlock2D(nn.Layer):
-
     def __init__(
         self,
         in_channels: int,
         prev_output_channel: int,
         out_channels: int,
         temb_channels: int,
         dropout: float = 0.0,
@@ -1535,33 +1585,32 @@
         add_upsample=True,
         upsample_padding=1,
     ):
         super().__init__()
         self.resnets = nn.LayerList([])
 
         for i in range(num_layers):
-            res_skip_channels = in_channels if (i == num_layers -
-                                                1) else out_channels
+            res_skip_channels = in_channels if (i == num_layers - 1) else out_channels
             resnet_in_channels = prev_output_channel if i == 0 else out_channels
 
             self.resnets.append(
                 ResnetBlock2D(
                     in_channels=resnet_in_channels + res_skip_channels,
                     out_channels=out_channels,
                     temb_channels=temb_channels,
                     eps=resnet_eps,
-                    groups=min((resnet_in_channels + res_skip_channels) // 4,
-                               32),
+                    groups=min((resnet_in_channels + res_skip_channels) // 4, 32),
                     groups_out=min(out_channels // 4, 32),
                     dropout=dropout,
                     time_embedding_norm=resnet_time_scale_shift,
                     non_linearity=resnet_act_fn,
                     output_scale_factor=output_scale_factor,
                     pre_norm=resnet_pre_norm,
-                ))
+                )
+            )
 
         self.upsampler = FirUpsample2D(in_channels, out_channels=out_channels)
         if add_upsample:
             self.resnet_up = ResnetBlock2D(
                 in_channels=out_channels,
                 out_channels=out_channels,
                 temb_channels=temb_channels,
@@ -1573,40 +1622,31 @@
                 non_linearity=resnet_act_fn,
                 output_scale_factor=output_scale_factor,
                 pre_norm=resnet_pre_norm,
                 use_in_shortcut=True,
                 up=True,
                 kernel="fir",
             )
-            self.skip_conv = nn.Conv2D(out_channels,
-                                       3,
-                                       kernel_size=(3, 3),
-                                       stride=(1, 1),
-                                       padding=(1, 1))
-            self.skip_norm = nn.GroupNorm(num_groups=min(out_channels // 4, 32),
-                                          num_channels=out_channels,
-                                          epsilon=resnet_eps)
+            self.skip_conv = nn.Conv2D(out_channels, 3, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+            self.skip_norm = nn.GroupNorm(
+                num_groups=min(out_channels // 4, 32), num_channels=out_channels, epsilon=resnet_eps
+            )
             self.act = nn.Silu()
         else:
             self.resnet_up = None
             self.skip_conv = None
             self.skip_norm = None
             self.act = None
 
-    def forward(self,
-                hidden_states,
-                res_hidden_states_tuple,
-                temb=None,
-                skip_sample=None):
+    def forward(self, hidden_states, res_hidden_states_tuple, temb=None, skip_sample=None):
         for resnet in self.resnets:
             # pop res hidden states
             res_hidden_states = res_hidden_states_tuple[-1]
             res_hidden_states_tuple = res_hidden_states_tuple[:-1]
-            hidden_states = paddle.concat([hidden_states, res_hidden_states],
-                                          axis=1)
+            hidden_states = paddle.concat([hidden_states, res_hidden_states], axis=1)
 
             hidden_states = resnet(hidden_states, temb)
 
         if skip_sample is not None:
             skip_sample = self.upsampler(skip_sample)
         else:
             skip_sample = 0
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/models/vae.py` & `ppdiffusers-0.9.0/ppdiffusers/models/vae.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,26 +8,25 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 from dataclasses import dataclass
-from typing import Tuple, Union
+from typing import Optional, Tuple, Union
 
 import numpy as np
 import paddle
 import paddle.nn as nn
 
 from ..configuration_utils import ConfigMixin, register_to_config
 from ..modeling_utils import ModelMixin
 from ..utils import BaseOutput
-from .unet_blocks import UNetMidBlock2D, get_down_block, get_up_block
+from .unet_2d_blocks import UNetMidBlock2D, get_down_block, get_up_block
 
 
 @dataclass
 class DecoderOutput(BaseOutput):
     """
     Output of decoding method.
 
@@ -63,34 +62,29 @@
             `DiagonalGaussianDistribution` allows for sampling latents from the distribution.
     """
 
     latent_dist: "DiagonalGaussianDistribution"
 
 
 class Encoder(nn.Layer):
-
     def __init__(
         self,
         in_channels=3,
         out_channels=3,
-        down_block_types=("DownEncoderBlock2D", ),
-        block_out_channels=(64, ),
+        down_block_types=("DownEncoderBlock2D",),
+        block_out_channels=(64,),
         layers_per_block=2,
         norm_num_groups=32,
         act_fn="silu",
         double_z=True,
     ):
         super().__init__()
         self.layers_per_block = layers_per_block
 
-        self.conv_in = nn.Conv2D(in_channels,
-                                 block_out_channels[0],
-                                 kernel_size=3,
-                                 stride=1,
-                                 padding=1)
+        self.conv_in = nn.Conv2D(in_channels, block_out_channels[0], kernel_size=3, stride=1, padding=1)
 
         self.mid_block = None
         self.down_blocks = nn.LayerList([])
 
         # down
         output_channel = block_out_channels[0]
         for i, down_block_type in enumerate(down_block_types):
@@ -122,24 +116,21 @@
             resnet_time_scale_shift="default",
             attn_num_head_channels=None,
             resnet_groups=norm_num_groups,
             temb_channels=None,
         )
 
         # out
-        self.conv_norm_out = nn.GroupNorm(num_channels=block_out_channels[-1],
-                                          num_groups=norm_num_groups,
-                                          epsilon=1e-6)
+        self.conv_norm_out = nn.GroupNorm(
+            num_channels=block_out_channels[-1], num_groups=norm_num_groups, epsilon=1e-6
+        )
         self.conv_act = nn.Silu()
 
         conv_out_channels = 2 * out_channels if double_z else out_channels
-        self.conv_out = nn.Conv2D(block_out_channels[-1],
-                                  conv_out_channels,
-                                  3,
-                                  padding=1)
+        self.conv_out = nn.Conv2D(block_out_channels[-1], conv_out_channels, 3, padding=1)
 
     def forward(self, x):
         sample = x
         sample = self.conv_in(sample)
 
         # down
         for down_block in self.down_blocks:
@@ -153,33 +144,28 @@
         sample = self.conv_act(sample)
         sample = self.conv_out(sample)
 
         return sample
 
 
 class Decoder(nn.Layer):
-
     def __init__(
         self,
         in_channels=3,
         out_channels=3,
-        up_block_types=("UpDecoderBlock2D", ),
-        block_out_channels=(64, ),
+        up_block_types=("UpDecoderBlock2D",),
+        block_out_channels=(64,),
         layers_per_block=2,
         norm_num_groups=32,
         act_fn="silu",
     ):
         super().__init__()
         self.layers_per_block = layers_per_block
 
-        self.conv_in = nn.Conv2D(in_channels,
-                                 block_out_channels[-1],
-                                 kernel_size=3,
-                                 stride=1,
-                                 padding=1)
+        self.conv_in = nn.Conv2D(in_channels, block_out_channels[-1], kernel_size=3, stride=1, padding=1)
 
         self.mid_block = None
         self.up_blocks = nn.LayerList([])
 
         # mid
         self.mid_block = UNetMidBlock2D(
             in_channels=block_out_channels[-1],
@@ -214,22 +200,17 @@
                 attn_num_head_channels=None,
                 temb_channels=None,
             )
             self.up_blocks.append(up_block)
             prev_output_channel = output_channel
 
         # out
-        self.conv_norm_out = nn.GroupNorm(num_channels=block_out_channels[0],
-                                          num_groups=norm_num_groups,
-                                          epsilon=1e-6)
+        self.conv_norm_out = nn.GroupNorm(num_channels=block_out_channels[0], num_groups=norm_num_groups, epsilon=1e-6)
         self.conv_act = nn.Silu()
-        self.conv_out = nn.Conv2D(block_out_channels[0],
-                                  out_channels,
-                                  3,
-                                  padding=1)
+        self.conv_out = nn.Conv2D(block_out_channels[0], out_channels, 3, padding=1)
 
     def forward(self, z):
         sample = z
         sample = self.conv_in(sample)
 
         # middle
         sample = self.mid_block(sample)
@@ -251,179 +232,168 @@
     Improved version over VectorQuantizer, can be used as a drop-in replacement. Mostly avoids costly matrix
     multiplications and allows for post-hoc remapping of indices.
     """
 
     # NOTE: due to a bug the beta term was applied to the wrong term. for
     # backwards compatibility we use the buggy version by default, but you can
     # specify legacy=False to fix it.
-    def __init__(self,
-                 n_e,
-                 e_dim,
-                 beta,
-                 remap=None,
-                 unknown_index="random",
-                 sane_index_shape=False,
-                 legacy=True):
+    def __init__(
+        self, n_e, vq_embed_dim, beta, remap=None, unknown_index="random", sane_index_shape=False, legacy=True
+    ):
         super().__init__()
         self.n_e = n_e
-        self.e_dim = e_dim
+        self.vq_embed_dim = vq_embed_dim
         self.beta = beta
         self.legacy = legacy
 
-        self.embedding = nn.Embedding(self.n_e,
-                                      self.e_dim,
-                                      weight_attr=nn.initializer.Uniform(
-                                          -1.0 / self.n_e, 1.0 / self.n_e))
+        self.embedding = nn.Embedding(
+            self.n_e, self.vq_embed_dim, weight_attr=nn.initializer.Uniform(-1.0 / self.n_e, 1.0 / self.n_e)
+        )
 
         self.remap = remap
         if self.remap is not None:
             self.register_buffer("used", paddle.to_tensor(np.load(self.remap)))
             self.re_embed = self.used.shape[0]
             self.unknown_index = unknown_index  # "random" or "extra" or integer
             if self.unknown_index == "extra":
                 self.unknown_index = self.re_embed
                 self.re_embed = self.re_embed + 1
-            print(f"Remapping {self.n_e} indices to {self.re_embed} indices. "
-                  f"Using {self.unknown_index} for unknown indices.")
+            print(
+                f"Remapping {self.n_e} indices to {self.re_embed} indices. "
+                f"Using {self.unknown_index} for unknown indices."
+            )
         else:
             self.re_embed = n_e
 
         self.sane_index_shape = sane_index_shape
 
     def remap_to_used(self, inds):
         ishape = inds.shape
         assert len(ishape) > 1
         inds = inds.reshape([ishape[0], -1])
-        used = self.used.astype(inds.dtype)
-        match = (inds[:, :, None] == used[None, None, ...]).astype("int64")
+        used = self.used.cast(inds.dtype)
+        match = (inds[:, :, None] == used[None, None, ...]).cast("int64")
         new = match.argmax(-1)
         unknown = match.sum(2) < 1
         if self.unknown_index == "random":
-            new[unknown] = paddle.randint(0,
-                                          self.re_embed,
-                                          shape=new[unknown].shape)
+            new[unknown] = paddle.randint(0, self.re_embed, shape=new[unknown].shape)
         else:
             new[unknown] = self.unknown_index
         return new.reshape(ishape)
 
     def unmap_to_all(self, inds):
         ishape = inds.shape
         assert len(ishape) > 1
         inds = inds.reshape([ishape[0], -1])
-        used = self.used.astype(inds.dtype)
+        used = self.used.cast(inds.dtype)
         if self.re_embed > self.used.shape[0]:  # extra token
             inds[inds >= self.used.shape[0]] = 0  # simply set to zero
-        back = paddle.gather(used[None, :][inds.shape[0] * [0], :],
-                             inds,
-                             axis=1)
+        back = paddle.take_along_axis(used[None, :][inds.shape[0] * [0], :], inds, axis=1)
         return back.reshape(ishape)
 
     def forward(self, z):
         # reshape z -> (batch, height, width, channel) and flatten
         z = z.transpose([0, 2, 3, 1])
-        z_flattened = z.reshape([-1, self.e_dim])
+        z_flattened = z.reshape([-1, self.vq_embed_dim])
         # distances from z to embeddings e_j (z - e)^2 = z^2 + e^2 - 2 e * z
 
         d = (
-            paddle.sum(z_flattened**2, axis=1, keepdim=True) +
-            paddle.sum(self.embedding.weight**2, axis=1) - 2 *
-            paddle.matmul(z_flattened, self.embedding.weight, transpose_y=True))
+            paddle.sum(z_flattened**2, axis=1, keepdim=True)
+            + paddle.sum(self.embedding.weight**2, axis=1)
+            - 2 * paddle.matmul(z_flattened, self.embedding.weight, transpose_y=True)
+        )
 
         min_encoding_indices = paddle.argmin(d, axis=1)
         z_q = self.embedding(min_encoding_indices).reshape(z.shape)
         perplexity = None
         min_encodings = None
 
         # compute loss for embedding
         if not self.legacy:
-            loss = self.beta * paddle.mean((z_q.detach() - z)**2) + paddle.mean(
-                (z_q - z.detach())**2)
+            loss = self.beta * paddle.mean((z_q.detach() - z) ** 2) + paddle.mean((z_q - z.detach()) ** 2)
         else:
-            loss = paddle.mean((z_q.detach() - z)**2) + self.beta * paddle.mean(
-                (z_q - z.detach())**2)
+            loss = paddle.mean((z_q.detach() - z) ** 2) + self.beta * paddle.mean((z_q - z.detach()) ** 2)
 
         # preserve gradients
         z_q = z + (z_q - z).detach()
 
         # reshape back to match original input shape
         z_q = z_q.transpose([0, 3, 1, 2])
 
         if self.remap is not None:
-            min_encoding_indices = min_encoding_indices.reshape(
-                [z.shape[0], -1])  # add batch axis
+            min_encoding_indices = min_encoding_indices.reshape([z.shape[0], -1])  # add batch axis
             min_encoding_indices = self.remap_to_used(min_encoding_indices)
-            min_encoding_indices = min_encoding_indices.reshape([-1,
-                                                                 1])  # flatten
+            min_encoding_indices = min_encoding_indices.reshape([-1, 1])  # flatten
 
         if self.sane_index_shape:
-            min_encoding_indices = min_encoding_indices.reshape(
-                [z_q.shape[0], z_q.shape[2], z_q.shape[3]])
+            min_encoding_indices = min_encoding_indices.reshape([z_q.shape[0], z_q.shape[2], z_q.shape[3]])
 
         return z_q, loss, (perplexity, min_encodings, min_encoding_indices)
 
     def get_codebook_entry(self, indices, shape):
         # shape specifying (batch, height, width, channel)
         if self.remap is not None:
             indices = indices.reshape([shape[0], -1])  # add batch axis
             indices = self.unmap_to_all(indices)
-            indices = indices.reshape([
-                -1,
-            ])  # flatten again
+            indices = indices.reshape(
+                [
+                    -1,
+                ]
+            )  # flatten again
 
         # get quantized latent vectors
         z_q = self.embedding(indices)
 
         if shape is not None:
             z_q = z_q.reshape(shape)
             # reshape back to match original input shape
             z_q = z_q.transpose([0, 3, 1, 2])
 
         return z_q
 
 
 class DiagonalGaussianDistribution(object):
-
     def __init__(self, parameters, deterministic=False):
         self.parameters = parameters
         self.mean, self.logvar = paddle.chunk(parameters, 2, axis=1)
         self.logvar = paddle.clip(self.logvar, -30.0, 20.0)
         self.deterministic = deterministic
         self.std = paddle.exp(0.5 * self.logvar)
         self.var = paddle.exp(self.logvar)
         if self.deterministic:
-            self.var = self.std = paddle.zeros_like(self.mean,
-                                                    dtype=self.parameters.dtype)
+            self.var = self.std = paddle.zeros_like(self.mean, dtype=self.parameters.dtype)
 
-    def sample(self) -> paddle.Tensor:
-        sample = paddle.randn(self.mean.shape)
+    def sample(self, generator: Optional[paddle.Generator] = None) -> paddle.Tensor:
+        sample = paddle.randn(self.mean.shape, generator=generator)
+        # make sure sample is as the parameters and has same dtype
+        sample = sample.cast(self.parameters.dtype)
         x = self.mean + self.std * sample
         return x
 
     def kl(self, other=None):
         if self.deterministic:
             return paddle.to_tensor([0.0])
         else:
             if other is None:
-                return 0.5 * paddle.sum(
-                    paddle.pow(self.mean, 2) + self.var - 1.0 - self.logvar,
-                    axis=[1, 2, 3])
+                return 0.5 * paddle.sum(paddle.pow(self.mean, 2) + self.var - 1.0 - self.logvar, axis=[1, 2, 3])
             else:
                 return 0.5 * paddle.sum(
-                    paddle.pow(self.mean - other.mean, 2) / other.var +
-                    self.var / other.var - 1.0 - self.logvar + other.logvar,
+                    paddle.pow(self.mean - other.mean, 2) / other.var
+                    + self.var / other.var
+                    - 1.0
+                    - self.logvar
+                    + other.logvar,
                     axis=[1, 2, 3],
                 )
 
     def nll(self, sample, axis=[1, 2, 3]):
         if self.deterministic:
             return paddle.to_tensor([0.0])
         logtwopi = np.log(2.0 * np.pi)
-        return 0.5 * paddle.sum(logtwopi + self.logvar +
-                                paddle.pow(sample - self.mean, 2) / self.var,
-                                axis=axis)
+        return 0.5 * paddle.sum(logtwopi + self.logvar + paddle.pow(sample - self.mean, 2) / self.var, axis=axis)
 
     def mode(self):
         return self.mean
 
 
 class VQModel(ModelMixin, ConfigMixin):
     r"""VQ-VAE model from the paper Neural Discrete Representation Learning by Aaron van den Oord, Oriol Vinyals and Koray
@@ -441,30 +411,32 @@
             obj:`("UpDecoderBlock2D",)`): Tuple of upsample block types.
         block_out_channels (`Tuple[int]`, *optional*, defaults to :
             obj:`(64,)`): Tuple of block output channels.
         act_fn (`str`, *optional*, defaults to `"silu"`): The activation function to use.
         latent_channels (`int`, *optional*, defaults to `3`): Number of channels in the latent space.
         sample_size (`int`, *optional*, defaults to `32`): TODO
         num_vq_embeddings (`int`, *optional*, defaults to `256`): Number of codebook vectors in the VQ-VAE.
+        vq_embed_dim (`int`, *optional*): Hidden dim of codebook vectors in the VQ-VAE.
     """
 
     @register_to_config
     def __init__(
         self,
         in_channels: int = 3,
         out_channels: int = 3,
-        down_block_types: Tuple[str] = ("DownEncoderBlock2D", ),
-        up_block_types: Tuple[str] = ("UpDecoderBlock2D", ),
-        block_out_channels: Tuple[int] = (64, ),
+        down_block_types: Tuple[str] = ("DownEncoderBlock2D",),
+        up_block_types: Tuple[str] = ("UpDecoderBlock2D",),
+        block_out_channels: Tuple[int] = (64,),
         layers_per_block: int = 1,
         act_fn: str = "silu",
         latent_channels: int = 3,
         sample_size: int = 32,
         num_vq_embeddings: int = 256,
         norm_num_groups: int = 32,
+        vq_embed_dim: Optional[int] = None,
     ):
         super().__init__()
 
         # pass init params to Encoder
         self.encoder = Encoder(
             in_channels=in_channels,
             out_channels=latent_channels,
@@ -472,21 +444,19 @@
             block_out_channels=block_out_channels,
             layers_per_block=layers_per_block,
             act_fn=act_fn,
             norm_num_groups=norm_num_groups,
             double_z=False,
         )
 
-        self.quant_conv = nn.Conv2D(latent_channels, latent_channels, 1)
-        self.quantize = VectorQuantizer(num_vq_embeddings,
-                                        latent_channels,
-                                        beta=0.25,
-                                        remap=None,
-                                        sane_index_shape=False)
-        self.post_quant_conv = nn.Conv2D(latent_channels, latent_channels, 1)
+        vq_embed_dim = vq_embed_dim if vq_embed_dim is not None else latent_channels
+
+        self.quant_conv = nn.Conv2D(latent_channels, vq_embed_dim, 1)
+        self.quantize = VectorQuantizer(num_vq_embeddings, vq_embed_dim, beta=0.25, remap=None, sane_index_shape=False)
+        self.post_quant_conv = nn.Conv2D(vq_embed_dim, latent_channels, 1)
 
         # pass init params to Decoder
         self.decoder = Decoder(
             in_channels=latent_channels,
             out_channels=out_channels,
             up_block_types=up_block_types,
             block_out_channels=block_out_channels,
@@ -496,32 +466,29 @@
         )
 
     def encode(self, x: paddle.Tensor, return_dict: bool = True):
         h = self.encoder(x)
         h = self.quant_conv(h)
 
         if not return_dict:
-            return (h, )
+            return (h,)
 
         return VQEncoderOutput(latents=h)
 
-    def decode(self,
-               h: paddle.Tensor,
-               force_not_quantize: bool = False,
-               return_dict: bool = True):
+    def decode(self, h: paddle.Tensor, force_not_quantize: bool = False, return_dict: bool = True):
         # also go through quantization layer
         if not force_not_quantize:
             quant, emb_loss, info = self.quantize(h)
         else:
             quant = h
         quant = self.post_quant_conv(quant)
         dec = self.decoder(quant)
 
         if not return_dict:
-            return (dec, )
+            return (dec,)
 
         return DecoderOutput(sample=dec)
 
     def forward(self, sample: paddle.Tensor, return_dict: bool = True):
         r"""
         Args:
             sample (`paddle.Tensor`): Input sample.
@@ -529,15 +496,15 @@
                 Whether or not to return a [`DecoderOutput`] instead of a plain tuple.
         """
         x = sample
         h = self.encode(x).latents
         dec = self.decode(h).sample
 
         if not return_dict:
-            return (dec, )
+            return (dec,)
 
         return DecoderOutput(sample=dec)
 
 
 class AutoencoderKL(ModelMixin, ConfigMixin):
     r"""Variational Autoencoder (VAE) model with KL loss from the paper Auto-Encoding Variational Bayes by Diederik P. Kingma
     and Max Welling.
@@ -560,17 +527,17 @@
     """
 
     @register_to_config
     def __init__(
         self,
         in_channels: int = 3,
         out_channels: int = 3,
-        down_block_types: Tuple[str] = ("DownEncoderBlock2D", ),
-        up_block_types: Tuple[str] = ("UpDecoderBlock2D", ),
-        block_out_channels: Tuple[int] = (64, ),
+        down_block_types: Tuple[str] = ("DownEncoderBlock2D",),
+        up_block_types: Tuple[str] = ("UpDecoderBlock2D",),
+        block_out_channels: Tuple[int] = (64,),
         layers_per_block: int = 1,
         act_fn: str = "silu",
         latent_channels: int = 4,
         norm_num_groups: int = 32,
         sample_size: int = 32,
     ):
         super().__init__()
@@ -603,46 +570,49 @@
 
     def encode(self, x: paddle.Tensor, return_dict: bool = True):
         h = self.encoder(x)
         moments = self.quant_conv(h)
         posterior = DiagonalGaussianDistribution(moments)
 
         if not return_dict:
-            return (posterior, )
+            return (posterior,)
 
         return AutoencoderKLOutput(latent_dist=posterior)
 
+    # (TODO junnyu) support vae slice
+    # https://github.com/huggingface/diffusers/commit/c28d3c82ce6f56c4b373a8260c56357d13db900a#diff-64804f08bc5e7a09947fb4eced462f15965acfa2d797354d85033e788f23b443
     def decode(self, z: paddle.Tensor, return_dict: bool = True):
         z = self.post_quant_conv(z)
         dec = self.decoder(z)
 
         if not return_dict:
-            return (dec, )
+            return (dec,)
 
         return DecoderOutput(sample=dec)
 
     def forward(
         self,
         sample: paddle.Tensor,
         sample_posterior: bool = False,
         return_dict: bool = True,
-    ):
+        generator: Optional[paddle.Generator] = None,
+    ) -> Union[DecoderOutput, paddle.Tensor]:
         r"""
         Args:
             sample (`paddle.Tensor`): Input sample.
             sample_posterior (`bool`, *optional*, defaults to `False`):
                 Whether to sample from the posterior.
             return_dict (`bool`, *optional*, defaults to `True`):
                 Whether or not to return a [`DecoderOutput`] instead of a plain tuple.
         """
         x = sample
         posterior = self.encode(x).latent_dist
         if sample_posterior:
-            z = posterior.sample()
+            z = posterior.sample(generator=generator)
         else:
             z = posterior.mode()
         dec = self.decode(z).sample
 
         if not return_dict:
-            return (dec, )
+            return (dec,)
 
         return DecoderOutput(sample=dec)
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/optimization.py` & `ppdiffusers-0.9.0/ppdiffusers/optimization.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Copyright (c) 2022 PaddlePaddle Authors. All Rights Reserved.
-# Copyright 2022 The HuggingFace Inc. team.
+# Copyright 2022 The HuggingFace Team. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -46,17 +46,15 @@
 
     Return:
         `paddle.optimizer.lr.LambdaDecay` with the appropriate schedule.
     """
     return LambdaDecay(learning_rate, lambda _: 1, last_epoch=last_epoch)
 
 
-def get_constant_schedule_with_warmup(learning_rate: float,
-                                      num_warmup_steps: int,
-                                      last_epoch: int = -1):
+def get_constant_schedule_with_warmup(learning_rate: float, num_warmup_steps: int, last_epoch: int = -1):
     """
     Create a schedule with a constant learning rate preceded by a warmup period during which the learning rate
     increases linearly between 0 and the initial lr set in the optimizer.
 
     Args:
         learning_rate (`float`):
             The base learning rate. It is a python float number.
@@ -73,18 +71,17 @@
         if current_step < num_warmup_steps:
             return float(current_step) / float(max(1.0, num_warmup_steps))
         return 1.0
 
     return LambdaDecay(learning_rate, lr_lambda, last_epoch=last_epoch)
 
 
-def get_linear_schedule_with_warmup(learning_rate: float,
-                                    num_warmup_steps: int,
-                                    num_training_steps: int,
-                                    last_epoch: int = -1):
+def get_linear_schedule_with_warmup(
+    learning_rate: float, num_warmup_steps: int, num_training_steps: int, last_epoch: int = -1
+):
     """
     Create a schedule with a learning rate that decreases linearly from the initial lr set in the optimizer to 0, after
     a warmup period during which it increases linearly from 0 to the initial lr set in the optimizer.
 
     Args:
         learning_rate (`float`):
             The base learning rate. It is a python float number.
@@ -99,26 +96,23 @@
         `paddle.optimizer.lr.LambdaDecay` with the appropriate schedule.
     """
 
     def lr_lambda(current_step: int):
         if current_step < num_warmup_steps:
             return float(current_step) / float(max(1, num_warmup_steps))
         return max(
-            0.0,
-            float(num_training_steps - current_step) /
-            float(max(1, num_training_steps - num_warmup_steps)))
+            0.0, float(num_training_steps - current_step) / float(max(1, num_training_steps - num_warmup_steps))
+        )
 
     return LambdaDecay(learning_rate, lr_lambda, last_epoch)
 
 
-def get_cosine_schedule_with_warmup(learning_rate: float,
-                                    num_warmup_steps: int,
-                                    num_training_steps: int,
-                                    num_cycles: float = 0.5,
-                                    last_epoch: int = -1):
+def get_cosine_schedule_with_warmup(
+    learning_rate: float, num_warmup_steps: int, num_training_steps: int, num_cycles: float = 0.5, last_epoch: int = -1
+):
     """
     Create a schedule with a learning rate that decreases following the values of the cosine function between the
     initial lr set in the optimizer to 0, after a warmup period during which it increases linearly between 0 and the
     initial lr set in the optimizer.
 
     Args:
         learning_rate (`float`):
@@ -136,28 +130,23 @@
     Return:
         `paddle.optimizer.lr.LambdaDecay` with the appropriate schedule.
     """
 
     def lr_lambda(current_step):
         if current_step < num_warmup_steps:
             return float(current_step) / float(max(1, num_warmup_steps))
-        progress = float(current_step - num_warmup_steps) / float(
-            max(1, num_training_steps - num_warmup_steps))
-        return max(
-            0.0, 0.5 *
-            (1.0 + math.cos(math.pi * float(num_cycles) * 2.0 * progress)))
+        progress = float(current_step - num_warmup_steps) / float(max(1, num_training_steps - num_warmup_steps))
+        return max(0.0, 0.5 * (1.0 + math.cos(math.pi * float(num_cycles) * 2.0 * progress)))
 
     return LambdaDecay(learning_rate, lr_lambda, last_epoch)
 
 
-def get_cosine_with_hard_restarts_schedule_with_warmup(learning_rate: float,
-                                                       num_warmup_steps: int,
-                                                       num_training_steps: int,
-                                                       num_cycles: int = 1,
-                                                       last_epoch: int = -1):
+def get_cosine_with_hard_restarts_schedule_with_warmup(
+    learning_rate: float, num_warmup_steps: int, num_training_steps: int, num_cycles: int = 1, last_epoch: int = -1
+):
     """
     Create a schedule with a learning rate that decreases following the values of the cosine function between the
     initial lr set in the optimizer to 0, with several hard restarts, after a warmup period during which it increases
     linearly between 0 and the initial lr set in the optimizer.
 
     Args:
         learning_rate (`float`):
@@ -174,31 +163,30 @@
     Return:
         `paddle.optimizer.lr.LambdaDecay` with the appropriate schedule.
     """
 
     def lr_lambda(current_step):
         if current_step < num_warmup_steps:
             return float(current_step) / float(max(1, num_warmup_steps))
-        progress = float(current_step - num_warmup_steps) / float(
-            max(1, num_training_steps - num_warmup_steps))
+        progress = float(current_step - num_warmup_steps) / float(max(1, num_training_steps - num_warmup_steps))
         if progress >= 1.0:
             return 0.0
-        return max(
-            0.0, 0.5 * (1.0 + math.cos(math.pi *
-                                       ((float(num_cycles) * progress) % 1.0))))
+        return max(0.0, 0.5 * (1.0 + math.cos(math.pi * ((float(num_cycles) * progress) % 1.0))))
 
     return LambdaDecay(learning_rate, lr_lambda, last_epoch)
 
 
-def get_polynomial_decay_schedule_with_warmup(learning_rate: float,
-                                              num_warmup_steps: int,
-                                              num_training_steps: int,
-                                              lr_end: float = 1e-7,
-                                              power: float = 1.0,
-                                              last_epoch: int = -1):
+def get_polynomial_decay_schedule_with_warmup(
+    learning_rate: float,
+    num_warmup_steps: int,
+    num_training_steps: int,
+    lr_end: float = 1e-7,
+    power: float = 1.0,
+    last_epoch: int = -1,
+):
     """
     Create a schedule with a learning rate that decreases as a polynomial decay from the initial lr set in the
     optimizer to end lr defined by *lr_end*, after a warmup period during which it increases linearly from 0 to the
     initial lr set in the optimizer.
 
     Args:
         learning_rate (`float`):
@@ -221,16 +209,15 @@
     Return:
         `paddle.optimizer.lr.LambdaDecay` with the appropriate schedule.
 
     """
 
     lr_init = learning_rate
     if not (lr_init > lr_end):
-        raise ValueError(
-            f"lr_end ({lr_end}) must be be smaller than initial lr ({lr_init})")
+        raise ValueError(f"lr_end ({lr_end}) must be be smaller than initial lr ({lr_init})")
 
     def lr_lambda(current_step: int):
         if current_step < num_warmup_steps:
             return float(current_step) / float(max(1, num_warmup_steps))
         elif current_step > num_training_steps:
             return lr_end / lr_init  # as LambdaLR multiplies by lr_init
         else:
@@ -242,16 +229,15 @@
 
     return LambdaDecay(learning_rate, lr_lambda, last_epoch)
 
 
 TYPE_TO_SCHEDULER_FUNCTION = {
     SchedulerType.LINEAR: get_linear_schedule_with_warmup,
     SchedulerType.COSINE: get_cosine_schedule_with_warmup,
-    SchedulerType.COSINE_WITH_RESTARTS:
-    get_cosine_with_hard_restarts_schedule_with_warmup,
+    SchedulerType.COSINE_WITH_RESTARTS: get_cosine_with_hard_restarts_schedule_with_warmup,
     SchedulerType.POLYNOMIAL: get_polynomial_decay_schedule_with_warmup,
     SchedulerType.CONSTANT: get_constant_schedule,
     SchedulerType.CONSTANT_WITH_WARMUP: get_constant_schedule_with_warmup,
 }
 
 
 def get_scheduler(
@@ -278,24 +264,19 @@
     name = SchedulerType(name)
     schedule_func = TYPE_TO_SCHEDULER_FUNCTION[name]
     if name == SchedulerType.CONSTANT:
         return schedule_func(learning_rate=learning_rate)
 
     # All other schedulers require `num_warmup_steps`
     if num_warmup_steps is None:
-        raise ValueError(
-            f"{name} requires `num_warmup_steps`, please provide that argument."
-        )
+        raise ValueError(f"{name} requires `num_warmup_steps`, please provide that argument.")
 
     if name == SchedulerType.CONSTANT_WITH_WARMUP:
-        return schedule_func(learning_rate=learning_rate,
-                             num_warmup_steps=num_warmup_steps)
+        return schedule_func(learning_rate=learning_rate, num_warmup_steps=num_warmup_steps)
 
     # All other schedulers require `num_training_steps`
     if num_training_steps is None:
-        raise ValueError(
-            f"{name} requires `num_training_steps`, please provide that argument."
-        )
+        raise ValueError(f"{name} requires `num_training_steps`, please provide that argument.")
 
-    return schedule_func(learning_rate=learning_rate,
-                         num_warmup_steps=num_warmup_steps,
-                         num_training_steps=num_training_steps)
+    return schedule_func(
+        learning_rate=learning_rate, num_warmup_steps=num_warmup_steps, num_training_steps=num_training_steps
+    )
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/pipeline_utils.py` & `ppdiffusers-0.9.0/ppdiffusers/pipeline_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Copyright (c) 2022 PaddlePaddle Authors. All Rights Reserved.
-# Copyright 2022 The HuggingFace Inc. team.
+# Copyright 2022 The HuggingFace Team. All rights reserved.
 # Copyright (c) 2022, NVIDIA CORPORATION.  All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -19,43 +19,42 @@
 import os
 from dataclasses import dataclass
 from typing import Any, Dict, List, Optional, Union
 
 import numpy as np
 import paddle
 import paddle.nn as nn
-from packaging import version
-
 import PIL
+from packaging import version
 from PIL import Image
 from tqdm.auto import tqdm
 
+from . import FastDeployRuntimeModel
 from .configuration_utils import ConfigMixin
-from .utils import (PPDIFFUSERS_CACHE, BaseOutput, logging, deprecate,
-                    DOWNLOAD_SERVER)
-
-from . import OnnxRuntimeModel
+from .utils import PPDIFFUSERS_CACHE, BaseOutput, deprecate, logging
 
 INDEX_FILE = "model_state.pdparams"
+CUSTOM_PIPELINE_FILE_NAME = "pipeline.py"
 DUMMY_MODULES_FOLDER = "ppdiffusers.utils"
+PADDLENLP_DUMMY_MODULES_FOLDER = "paddlenlp.transformers.utils"
 
 logger = logging.get_logger(__name__)
 
 LOADABLE_CLASSES = {
     "ppdiffusers": {
         "ModelMixin": ["save_pretrained", "from_pretrained"],
-        "SchedulerMixin": ["save_config", "from_config"],
+        "SchedulerMixin": ["save_pretrained", "from_pretrained"],
         "DiffusionPipeline": ["save_pretrained", "from_pretrained"],
-        "OnnxRuntimeModel": ["save_pretrained", "from_pretrained"],
-        "LDMBertModel": ["save_pretrained", "from_pretrained"],
+        "FastDeployRuntimeModel": ["save_pretrained", "from_pretrained"],
     },
     "paddlenlp.transformers": {
         "PretrainedTokenizer": ["save_pretrained", "from_pretrained"],
         "PretrainedModel": ["save_pretrained", "from_pretrained"],
         "FeatureExtractionMixin": ["save_pretrained", "from_pretrained"],
+        "ProcessorMixin": ["save_pretrained", "from_pretrained"],
     },
 }
 
 ALL_IMPORTABLE_CLASSES = {}
 for library in LOADABLE_CLASSES:
     ALL_IMPORTABLE_CLASSES.update(LOADABLE_CLASSES[library])
 
@@ -70,51 +69,66 @@
             List of denoised PIL images of length `batch_size` or numpy array of shape `(batch_size, height, width,
             num_channels)`. PIL images or numpy array present the denoised images of the diffusion pipeline.
     """
 
     images: Union[List[PIL.Image.Image], np.ndarray]
 
 
+@dataclass
+class AudioPipelineOutput(BaseOutput):
+    """
+    Output class for audio pipelines.
+
+    Args:
+        audios (`np.ndarray`)
+            List of denoised samples of shape `(batch_size, num_channels, sample_rate)`. Numpy array present the
+            denoised audio samples of the diffusion pipeline.
+    """
+
+    audios: np.ndarray
+
+
 class DiffusionPipeline(ConfigMixin):
     r"""
     Base class for all models.
 
     [`DiffusionPipeline`] takes care of storing all components (models, schedulers, processors) for diffusion pipelines
     and handles methods for loading, downloading and saving models as well as a few methods common to all pipelines to:
 
         - move all Paddle modules to the device of your choice
         - enabling/disabling the progress bar for the denoising iteration
 
     Class attributes:
 
-        - **config_name** ([`str`]) -- name of the config file that will store the class and module names of all
-          components of the diffusion pipeline.
+        - **config_name** (`str`) -- name of the config file that will store the class and module names of all
+        - **_optional_components** (List[`str`]) -- list of all components that are optional so they don't have to be
+          passed for the pipeline to function (should be overridden by subclasses).
     """
     config_name = "model_index.json"
+    _optional_components = []
 
     def register_modules(self, **kwargs):
         # import it here to avoid circular import
         from . import pipelines
 
         for name, module in kwargs.items():
-            # retrive library
+            # retrieve library
             if module is None:
                 register_dict = {name: (None, None)}
             else:
-                if "paddlenlp" in module.__module__.split("."):
+                # TODO (junnyu) support paddlenlp.transformers
+                if "paddlenlp" in module.__module__.split(".") or "ppnlp_patch_utils" in module.__module__.split("."):
                     library = "paddlenlp.transformers"
                 else:
                     library = module.__module__.split(".")[0]
 
                 # check if the module is a pipeline module
-                pipeline_dir = module.__module__.split(".")[-2] if len(
-                    module.__module__.split(".")) > 2 else None
+                pipeline_dir = module.__module__.split(".")[-2] if len(module.__module__.split(".")) > 2 else None
                 path = module.__module__.split(".")
-                is_pipeline_module = pipeline_dir in path and hasattr(
-                    pipelines, pipeline_dir)
+                is_pipeline_module = pipeline_dir in path and hasattr(pipelines, pipeline_dir)
 
                 # if library is not in LOADABLE_CLASSES, then it is a custom module.
                 # Or if it's a pipeline module, then the module is inside the pipeline
                 # folder so we set the library to module name.
                 if library not in LOADABLE_CLASSES or is_pipeline_module:
                     library = pipeline_dir
 
@@ -141,69 +155,84 @@
         """
         self.save_config(save_directory)
 
         model_index_dict = dict(self.config)
         model_index_dict.pop("_class_name")
         # TODO (junnyu) support old version
         model_index_dict.pop("_diffusers_paddle_version", None)
+        model_index_dict.pop("_diffusers_version", None)
         model_index_dict.pop("_ppdiffusers_version", None)
         model_index_dict.pop("_module", None)
 
+        expected_modules, optional_kwargs = self._get_signature_keys(self)
+
+        def is_saveable_module(name, value):
+            if name not in expected_modules:
+                return False
+            if name in self._optional_components and value[0] is None:
+                return False
+            return True
+
+        model_index_dict = {k: v for k, v in model_index_dict.items() if is_saveable_module(k, v)}
+
         for pipeline_component_name in model_index_dict.keys():
             sub_model = getattr(self, pipeline_component_name)
+
             model_cls = sub_model.__class__
 
             save_method_name = None
             # search for the model's base class in LOADABLE_CLASSES
             for library_name, library_classes in LOADABLE_CLASSES.items():
                 library = importlib.import_module(library_name)
                 for base_class, save_load_methods in library_classes.items():
-                    class_candidate = getattr(library, base_class)
-                    if issubclass(model_cls, class_candidate):
+                    class_candidate = getattr(library, base_class, None)
+                    if class_candidate is not None and issubclass(model_cls, class_candidate):
                         # if we found a suitable base class in LOADABLE_CLASSES then grab its save method
                         save_method_name = save_load_methods[0]
                         break
                 if save_method_name is not None:
                     break
 
-            # TODO 1014 junnyu for save null safety checker
-            if pipeline_component_name == "safety_checker" and save_method_name is None:
-                continue
             save_method = getattr(sub_model, save_method_name)
             save_method(os.path.join(save_directory, pipeline_component_name))
 
     def to(self, paddle_device: Optional[str] = None):
         if paddle_device is None:
             return self
 
-        module_names, _ = self.extract_init_dict(dict(self.config))
+        module_names, _, _ = self.extract_init_dict(dict(self.config))
         for name in module_names.keys():
             module = getattr(self, name)
             if isinstance(module, nn.Layer):
-                module.to(device=paddle_device)
+                if module.dtype == paddle.float16 and str(paddle_device) in ["cpu"]:
+                    logger.warning(
+                        "Pipelines loaded with `paddle_dtype=paddle.float16` cannot run with `cpu` device. It"
+                        " is not recommended to move them to `cpu` as running them will fail. Please make"
+                        " sure to use an accelerator to run the pipeline in inference, due to the lack of"
+                        " support for`float16` operations on this device in Paddle. Please, remove the"
+                        " `paddle_dtype=paddle.float16` argument, or use another device for inference."
+                    )
+                module.to(paddle_device)
         return self
 
     @property
     def device(self):
         r"""
         Returns:
             `paddle.device`: The paddle device on which the pipeline is located.
         """
-        module_names, _ = self.extract_init_dict(dict(self.config))
+        module_names, _, _ = self.extract_init_dict(dict(self.config))
         for name in module_names.keys():
             module = getattr(self, name)
             if isinstance(module, nn.Layer):
                 return module.place
         return "cpu"
 
     @classmethod
-    def from_pretrained(
-            cls, pretrained_model_name_or_path: Optional[Union[str,
-                                                               os.PathLike]],
-            **kwargs):
+    def from_pretrained(cls, pretrained_model_name_or_path: Optional[Union[str, os.PathLike]], **kwargs):
         r"""
         Instantiate a Paddle diffusion pipeline from pre-trained pipeline weights.
 
         The pipeline is set in evaluation mode by default using `model.eval()` (Dropout modules are deactivated).
 
         The warning *Weights from XXX not initialized from pretrained model* means that the weights of XXX do not come
         pretrained with the rest of the model. It is up to you to train those weights with a downstream fine-tuning
@@ -228,274 +257,302 @@
             kwargs (remaining dictionary of keyword arguments, *optional*):
                 Can be used to overwrite load - and saveable variables - *i.e.* the pipeline components - of the
                 specific pipeline class. The overwritten components are then directly passed to the pipelines
                 `__init__` method. See example below for more information.
 
         Examples:
 
-        ```python
-            >>> from ppdiffusers import StableDiffusionPipeline
-            >>> # Download pipeline from https://bj.bcebos.com/paddlenlp/models/community/CompVis/stable-diffusion-v1-4 and cache.
-            >>> pipeline = StableDiffusionPipeline.from_pretrained("CompVis/stable-diffusion-v1-4")
-
-            >>> # Download pipeline, but overwrite scheduler
-            >>> from ppdiffusers import LMSDiscreteScheduler, StableDiffusionPipeline
-            >>> scheduler = LMSDiscreteScheduler(beta_start=0.00085, beta_end=0.012, beta_schedule="scaled_linear")
-            >>> pipeline = StableDiffusionPipeline.from_pretrained("CompVis/stable-diffusion-v1-4", scheduler=scheduler)
+        ```py
+        >>> from ppdiffusers import DiffusionPipeline
+
+        >>> # Download pipeline from bos and cache.
+        >>> pipeline = DiffusionPipeline.from_pretrained("CompVis/ldm-text2im-large-256")
+
+        >>> # Download pipeline that requires an authorization token
+        >>> # For more information on access tokens, please refer to this section
+        >>> # of the documentation](https://huggingface.co/docs/hub/security-tokens)
+        >>> pipeline = DiffusionPipeline.from_pretrained("runwayml/stable-diffusion-v1-5")
+
+        >>> # Use a different scheduler
+        >>> from ppdiffusers import LMSDiscreteScheduler
+
+        >>> scheduler = LMSDiscreteScheduler.from_config(pipeline.scheduler.config)
+        >>> pipeline.scheduler = scheduler
         ```
         """
+        cache_dir = kwargs.pop("cache_dir", PPDIFFUSERS_CACHE)
         paddle_dtype = kwargs.pop("paddle_dtype", None)
-        provider = kwargs.pop("provider", None)
-        sess_options = kwargs.pop("sess_options", None)
-        # do not use
-
-        # 1. Download the configs
-        config_dict = cls.get_config_dict(pretrained_model_name_or_path)
+        # (TODO junnyu, we donot suuport this.)
+        # custom_pipeline = kwargs.pop("custom_pipeline", None)
+        # for fastdeploy model
+        runtime_options = kwargs.pop("runtime_options", None)
+
+        # 1. Download the checkpoints and configs
+        if not os.path.isdir(pretrained_model_name_or_path):
+            config_dict = cls.load_config(
+                pretrained_model_name_or_path,
+                cache_dir=cache_dir,
+            )
+        else:
+            config_dict = cls.load_config(pretrained_model_name_or_path)
 
-        # 2. Load the pipeline class, if using custom module then load it from the hub
+        # 2. Load the pipeline class
         if cls != DiffusionPipeline:
             pipeline_class = cls
         else:
-            diffusers_module = importlib.import_module(
-                cls.__module__.split(".")[0])
-            pipeline_class = getattr(diffusers_module,
-                                     config_dict["_class_name"])
+            diffusers_module = importlib.import_module(cls.__module__.split(".")[0])
+            pipeline_class = getattr(diffusers_module, config_dict["_class_name"])
 
         # To be removed in 1.0.0
         # TODO (junnyu) support old version
-        _ppdiffusers_version = config_dict[
-            "_diffusers_paddle_version"] if "_diffusers_paddle_version" in config_dict else config_dict[
-                "_ppdiffusers_version"]
+        _ppdiffusers_version = (
+            config_dict["_diffusers_paddle_version"]
+            if "_diffusers_paddle_version" in config_dict
+            else config_dict["_ppdiffusers_version"]
+        )
         if pipeline_class.__name__ == "StableDiffusionInpaintPipeline" and version.parse(
-                version.parse(_ppdiffusers_version).base_version
+            version.parse(_ppdiffusers_version).base_version
         ) <= version.parse("0.5.1"):
-            from ppdiffusers import StableDiffusionInpaintPipeline, StableDiffusionInpaintPipelineLegacy
+            from . import (
+                StableDiffusionInpaintPipeline,
+                StableDiffusionInpaintPipelineLegacy,
+            )
 
             pipeline_class = StableDiffusionInpaintPipelineLegacy
 
             deprecation_message = (
                 "You are using a legacy checkpoint for inpainting with Stable Diffusion, therefore we are loading the"
                 f" {StableDiffusionInpaintPipelineLegacy} class instead of {StableDiffusionInpaintPipeline}. For"
                 " better inpainting results, we strongly suggest using Stable Diffusion's official inpainting"
                 " checkpoint: https://huggingface.co/runwayml/stable-diffusion-inpainting instead or adapting your"
                 f" checkpoint {pretrained_model_name_or_path} to the format of"
                 " https://huggingface.co/runwayml/stable-diffusion-inpainting. Note that we do not actively maintain"
                 " the {StableDiffusionInpaintPipelineLegacy} class and will likely remove it in version 1.0.0."
             )
-            deprecate("StableDiffusionInpaintPipelineLegacy",
-                      "1.0.0",
-                      deprecation_message,
-                      standard_warn=False)
+            deprecate("StableDiffusionInpaintPipelineLegacy", "1.0.0", deprecation_message, standard_warn=False)
 
         # some modules can be passed directly to the init
         # in this case they are already instantiated in `kwargs`
         # extract them here
-        expected_modules = set(
-            inspect.signature(pipeline_class.__init__).parameters.keys()) - set(
-                ["self"])
-        passed_class_obj = {
-            k: kwargs.pop(k)
-            for k in expected_modules if k in kwargs
-        }
+        expected_modules, optional_kwargs = cls._get_signature_keys(pipeline_class)
 
-        init_dict, unused_kwargs = pipeline_class.extract_init_dict(
-            config_dict, **kwargs)
+        passed_class_obj = {k: kwargs.pop(k) for k in expected_modules if k in kwargs}
+        passed_pipe_kwargs = {k: kwargs.pop(k) for k in optional_kwargs if k in kwargs}
 
-        if len(unused_kwargs) > 0:
-            logger.warning(f"Keyword arguments {unused_kwargs} not recognized.")
+        init_dict, unused_kwargs, _ = pipeline_class.extract_init_dict(config_dict, **kwargs)
 
-        init_kwargs = {}
+        # define init kwargs
+        init_kwargs = {k: init_dict.pop(k) for k in optional_kwargs if k in init_dict}
+        init_kwargs = {**init_kwargs, **passed_pipe_kwargs}
+
+        # remove `null` components
+        def load_module(name, value):
+            if value[0] is None:
+                return False
+            if name in passed_class_obj and passed_class_obj[name] is None:
+                return False
+            return True
 
+        init_dict = {k: v for k, v in init_dict.items() if load_module(k, v)}
+
+        if len(unused_kwargs) > 0:
+            logger.warning(
+                f"Keyword arguments {unused_kwargs} are not expected by {pipeline_class.__name__} and will be ignored."
+            )
         # import it here to avoid circular import
-        from . import pipelines
+        from . import ModelMixin, pipelines
 
         # 3. Load each module in the pipeline
         for name, (library_name, class_name) in init_dict.items():
-            # TODO 1014 junnyu for load null safety checker
-            if name == "safety_checker" and (library_name is None
-                                             or class_name is None):
-                logger.warn("You have disabled the safety checker!")
-                init_kwargs[name] = None
-                continue
-
             # TODO (junnyu) support old model_index.json
             if library_name == "diffusers_paddle":
                 library_name = "ppdiffusers"
+
             is_pipeline_module = hasattr(pipelines, library_name)
             loaded_sub_model = None
-            sub_model_should_be_defined = True
 
             # if the model is in a pipeline module, then we load it from the pipeline
             if name in passed_class_obj:
                 # 1. check that passed_class_obj has correct parent class
                 if not is_pipeline_module:
                     library = importlib.import_module(library_name)
                     class_obj = getattr(library, class_name)
                     importable_classes = LOADABLE_CLASSES[library_name]
-                    class_candidates = {
-                        c: getattr(library, c)
-                        for c in importable_classes.keys()
-                    }
+                    class_candidates = {c: getattr(library, c, None) for c in importable_classes.keys()}
 
                     expected_class_obj = None
                     for class_name, class_candidate in class_candidates.items():
-                        if issubclass(class_obj, class_candidate):
+                        if class_candidate is not None and issubclass(class_obj, class_candidate):
                             expected_class_obj = class_candidate
 
-                    if not issubclass(passed_class_obj[name].__class__,
-                                      expected_class_obj):
+                    if not issubclass(passed_class_obj[name].__class__, expected_class_obj):
                         raise ValueError(
                             f"{passed_class_obj[name]} is of type: {type(passed_class_obj[name])}, but should be"
-                            f" {expected_class_obj}")
-                elif passed_class_obj[name] is None:
-                    logger.warn(
-                        f"You have passed `None` for {name} to disable its functionality in {pipeline_class}. Note"
-                        f" that this might lead to problems when using {pipeline_class} and is not recommended."
-                    )
-                    sub_model_should_be_defined = False
+                            f" {expected_class_obj}"
+                        )
                 else:
-                    logger.warn(
+                    logger.warning(
                         f"You have passed a non-standard module {passed_class_obj[name]}. We cannot verify whether it"
-                        " has the correct type")
+                        " has the correct type"
+                    )
 
                 # set passed class object
                 loaded_sub_model = passed_class_obj[name]
             elif is_pipeline_module:
                 pipeline_module = getattr(pipelines, library_name)
                 class_obj = getattr(pipeline_module, class_name)
                 importable_classes = ALL_IMPORTABLE_CLASSES
-                class_candidates = {
-                    c: class_obj
-                    for c in importable_classes.keys()
-                }
+                class_candidates = {c: class_obj for c in importable_classes.keys()}
             else:
                 # else we just import it from the library.
                 library = importlib.import_module(library_name)
+
                 class_obj = getattr(library, class_name)
                 importable_classes = LOADABLE_CLASSES[library_name]
-                class_candidates = {
-                    c: getattr(library, c)
-                    for c in importable_classes.keys()
-                }
+                class_candidates = {c: getattr(library, c, None) for c in importable_classes.keys()}
 
-            if loaded_sub_model is None and sub_model_should_be_defined:
+            if loaded_sub_model is None:
                 load_method_name = None
                 for class_name, class_candidate in class_candidates.items():
-                    if issubclass(class_obj, class_candidate):
+                    if class_candidate is not None and issubclass(class_obj, class_candidate):
                         load_method_name = importable_classes[class_name][1]
 
                 if load_method_name is None:
                     none_module = class_obj.__module__
-                    if none_module.startswith(
-                            DUMMY_MODULES_FOLDER) and "dummy" in none_module:
+                    is_dummy_path = none_module.startswith(DUMMY_MODULES_FOLDER) or none_module.startswith(
+                        PADDLENLP_DUMMY_MODULES_FOLDER
+                    )
+                    if is_dummy_path and "dummy" in none_module:
                         # call class_obj for nice error message of missing requirements
                         class_obj()
 
                     raise ValueError(
                         f"The component {class_obj} of {pipeline_class} cannot be loaded as it does not seem to have"
                         f" any of the loading methods defined in {ALL_IMPORTABLE_CLASSES}."
                     )
 
                 load_method = getattr(class_obj, load_method_name)
                 loading_kwargs = {}
 
-                if issubclass(class_obj, OnnxRuntimeModel):
-                    loading_kwargs["provider"] = provider
-                    loading_kwargs["sess_options"] = sess_options
-
-                model_path_dir = os.path.join(
-                    pretrained_model_name_or_path, name) if os.path.isdir(
-                        pretrained_model_name_or_path
-                    ) else pretrained_model_name_or_path + "/" + name
+                if issubclass(class_obj, FastDeployRuntimeModel):
+                    if isinstance(runtime_options, dict):
+                        options = runtime_options.get(name, None)
+                    else:
+                        options = runtime_options
+                    loading_kwargs["runtime_options"] = options
+                    loading_kwargs["cache_dir"] = cache_dir
+
+                if issubclass(class_obj, ModelMixin):
+                    loading_kwargs["cache_dir"] = cache_dir
+
+                model_path_dir = (
+                    os.path.join(pretrained_model_name_or_path, name)
+                    if os.path.isdir(pretrained_model_name_or_path)
+                    else pretrained_model_name_or_path + "/" + name
+                )
+
                 loaded_sub_model = load_method(model_path_dir, **loading_kwargs)
 
             # TODO junnyu find a better way to covert to float16
             if isinstance(loaded_sub_model, nn.Layer):
-                if next(loaded_sub_model.named_parameters()
-                        )[1].dtype != paddle_dtype:
+                if next(loaded_sub_model.named_parameters())[1].dtype != paddle_dtype:
                     loaded_sub_model = loaded_sub_model.to(dtype=paddle_dtype)
                 # paddlenlp model is training mode not eval mode
                 loaded_sub_model.eval()
-            init_kwargs[
-                name] = loaded_sub_model  # UNet(...), # DiffusionSchedule(...)
+
+            init_kwargs[name] = loaded_sub_model  # UNet(...), # DiffusionScheduler(...)
 
         # 4. Potentially add passed objects if expected
         missing_modules = set(expected_modules) - set(init_kwargs.keys())
-        if len(missing_modules) > 0 and missing_modules <= set(
-                passed_class_obj.keys()):
+        passed_modules = list(passed_class_obj.keys())
+        optional_modules = pipeline_class._optional_components
+        if len(missing_modules) > 0 and missing_modules <= set(passed_modules + optional_modules):
             for module in missing_modules:
-                init_kwargs[module] = passed_class_obj[module]
+                init_kwargs[module] = passed_class_obj.get(module, None)
         elif len(missing_modules) > 0:
-            passed_modules = set(
-                list(init_kwargs.keys()) + list(passed_class_obj.keys()))
+            passed_modules = set(list(init_kwargs.keys()) + list(passed_class_obj.keys())) - optional_kwargs
             raise ValueError(
                 f"Pipeline {pipeline_class} expected {expected_modules}, but only {passed_modules} were passed."
             )
 
         # 5. Instantiate the pipeline
         model = pipeline_class(**init_kwargs)
         return model
 
+    @staticmethod
+    def _get_signature_keys(obj):
+        parameters = inspect.signature(obj.__init__).parameters
+        required_parameters = {k: v for k, v in parameters.items() if v.default == inspect._empty}
+        optional_parameters = set({k for k, v in parameters.items() if v.default != inspect._empty})
+        expected_modules = set(required_parameters.keys()) - set(["self"])
+        return expected_modules, optional_parameters
+
     @property
     def components(self) -> Dict[str, Any]:
         r"""
-        The `self.compenents` property can be useful to run different pipelines with the same weights and
+
+        The `self.components` property can be useful to run different pipelines with the same weights and
         configurations to not have to re-allocate memory.
+
         Examples:
+
         ```py
         >>> from ppdiffusers import (
         ...     StableDiffusionPipeline,
         ...     StableDiffusionImg2ImgPipeline,
         ...     StableDiffusionInpaintPipeline,
         ... )
-        >>> img2text = StableDiffusionPipeline.from_pretrained("CompVis/stable-diffusion-v1-4")
-        >>> img2img = StableDiffusionImg2ImgPipeline(**img2text.components)
-        >>> inpaint = StableDiffusionInpaintPipeline(**img2text.components)
+
+        >>> text2img = StableDiffusionPipeline.from_pretrained("runwayml/stable-diffusion-v1-5")
+        >>> img2img = StableDiffusionImg2ImgPipeline(**text2img.components)
+        >>> inpaint = StableDiffusionInpaintPipeline(**text2img.components)
         ```
+
         Returns:
-            A dictionaly containing all the modules needed to initialize the pipleline.
+            A dictionaly containing all the modules needed to initialize the pipeline.
         """
+        expected_modules, optional_parameters = self._get_signature_keys(self)
         components = {
-            k: getattr(self, k)
-            for k in self.config.keys() if not k.startswith("_")
+            k: getattr(self, k) for k in self.config.keys() if not k.startswith("_") and k not in optional_parameters
         }
-        expected_modules = set(
-            inspect.signature(self.__init__).parameters.keys()) - set(["self"])
 
         if set(components.keys()) != expected_modules:
             raise ValueError(
                 f"{self} has been incorrectly initialized or {self.__class__} is incorrectly implemented. Expected"
                 f" {expected_modules} to be defined, but {components} are defined."
             )
 
         return components
 
     @staticmethod
-    def numpy_to_pil(images, **kwargs):
+    def numpy_to_pil(images):
         """
         Convert a numpy image or a batch of images to a PIL image.
         """
         if images.ndim == 3:
             images = images[None, ...]
         images = (images * 255).round().astype("uint8")
-        pil_images = []
-        argument = kwargs.pop("argument", None)
-        for image in images:
-            image = Image.fromarray(image)
-            if argument is not None:
-                image.argument = argument
-            pil_images.append(image)
+        if images.shape[-1] == 1:
+            # special case for grayscale (single channel) images
+            pil_images = [Image.fromarray(image.squeeze(), mode="L") for image in images]
+        else:
+            pil_images = [Image.fromarray(image) for image in images]
 
         return pil_images
 
-    def progress_bar(self, iterable):
+    def progress_bar(self, iterable=None, total=None):
         if not hasattr(self, "_progress_bar_config"):
             self._progress_bar_config = {}
         elif not isinstance(self._progress_bar_config, dict):
             raise ValueError(
                 f"`self._progress_bar_config` should be of type `dict`, but is {type(self._progress_bar_config)}."
             )
 
-        return tqdm(iterable, **self._progress_bar_config)
+        if iterable is not None:
+            return tqdm(iterable, **self._progress_bar_config)
+        elif total is not None:
+            return tqdm(total=total, **self._progress_bar_config)
+        else:
+            raise ValueError("Either `total` or `iterable` has to be defined.")
 
     def set_progress_bar_config(self, **kwargs):
         self._progress_bar_config = kwargs
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/pipelines/ddim/__init__.py` & `ppdiffusers-0.9.0/ppdiffusers/pipelines/ddim/__init__.py`

 * *Files identical despite different names*

### Comparing `ppdiffusers-0.6.3/ppdiffusers/pipelines/ddim/pipeline_ddim.py` & `ppdiffusers-0.9.0/ppdiffusers/pipelines/pndm/pipeline_pndm.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,93 +7,88 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
-
 # limitations under the License.
 
 from typing import Optional, Tuple, Union
 
 import paddle
 
+from ...models import UNet2DModel
 from ...pipeline_utils import DiffusionPipeline, ImagePipelineOutput
+from ...schedulers import PNDMScheduler
 
 
-class DDIMPipeline(DiffusionPipeline):
+class PNDMPipeline(DiffusionPipeline):
     r"""
     This model inherits from [`DiffusionPipeline`]. Check the superclass documentation for the generic methods the
-    library implements for all the pipelines (such as downloading or saving, running on a particular device, etc.)
+    library implements for all the pipelines (such as downloading or saving, running on a particular xxxx, etc.)
 
     Parameters:
-        unet ([`UNet2DModel`]): U-Net architecture to denoise the encoded image.
+        unet (`UNet2DModel`): U-Net architecture to denoise the encoded image latents.
         scheduler ([`SchedulerMixin`]):
-            A scheduler to be used in combination with `unet` to denoise the encoded image. Can be one of
-            [`DDPMScheduler`], or [`DDIMScheduler`].
+            The `PNDMScheduler` to be used in combination with `unet` to denoise the encoded image.
     """
 
-    def __init__(self, unet, scheduler):
+    unet: UNet2DModel
+    scheduler: PNDMScheduler
+
+    def __init__(self, unet: UNet2DModel, scheduler: PNDMScheduler):
         super().__init__()
         self.register_modules(unet=unet, scheduler=scheduler)
 
     @paddle.no_grad()
     def __call__(
         self,
         batch_size: int = 1,
-        seed: Optional[int] = None,
-        eta: float = 0.0,
         num_inference_steps: int = 50,
+        generator: Optional[paddle.Generator] = None,
         output_type: Optional[str] = "pil",
         return_dict: bool = True,
         **kwargs,
     ) -> Union[ImagePipelineOutput, Tuple]:
         r"""
         Args:
-            batch_size (`int`, *optional*, defaults to 1):
-                The number of images to generate.
-            seed (`int`, *optional*):
-                A random seed.
-            eta (`float`, *optional*, defaults to 0.0):
-                The eta parameter which controls the scale of the variance (0 is DDIM and 1 is one type of DDPM).
-            num_inference_steps (`int`, *optional*, defaults to 50):
+            batch_size (`int`, `optional`, defaults to 1): The number of images to generate.
+            num_inference_steps (`int`, `optional`, defaults to 50):
                 The number of denoising steps. More denoising steps usually lead to a higher quality image at the
                 expense of slower inference.
-            output_type (`str`, *optional*, defaults to `"pil"`):
-                The output format of the generate image. Choose between
-                [PIL](https://pillow.readthedocs.io/en/stable/): `PIL.Image.Image` or `np.array`.
-            return_dict (`bool`, *optional*, defaults to `True`):
-                Whether or not to return a [`~pipeline_utils.ImagePipelineOutput`] instead of a plain tuple.
+            generator (`paddle.Generator`, `optional`): A [paddle
+                generator](to make generation deterministic.
+            output_type (`str`, `optional`, defaults to `"pil"`): The output format of the generate image. Choose
+                between [PIL](https://pillow.readthedocs.io/en/stable/): `PIL.Image.Image` or `np.array`.
+            return_dict (`bool`, `optional`, defaults to `True`): Whether or not to return a
+                [`~pipeline_utils.ImagePipelineOutput`] instead of a plain tuple.
 
         Returns:
             [`~pipeline_utils.ImagePipelineOutput`] or `tuple`: [`~pipelines.utils.ImagePipelineOutput`] if
             `return_dict` is True, otherwise a `tuple. When returning a tuple, the first element is a list with the
             generated images.
         """
-        if seed is not None:
-            paddle.seed(seed)
+        # For more information on the sampling method you can take a look at Algorithm 2 of
+        # the official paper: https://arxiv.org/pdf/2202.09778.pdf
+
         # Sample gaussian noise to begin loop
-        image = paddle.randn((batch_size, self.unet.in_channels,
-                              self.unet.sample_size, self.unet.sample_size))
+        image = paddle.randn(
+            (batch_size, self.unet.in_channels, self.unet.sample_size, self.unet.sample_size),
+            generator=generator,
+        )
 
-        # set step values
         self.scheduler.set_timesteps(num_inference_steps)
-
         for t in self.progress_bar(self.scheduler.timesteps):
-            # 1. predict noise model_output
             model_output = self.unet(image, t).sample
 
-            # 2. predict previous mean of image x_t-1 and add variance depending on eta
-            # eta corresponds to η in paper and should be between [0, 1]
-            # do x_t -> x_t-1
-            image = self.scheduler.step(model_output, t, image, eta).prev_sample
+            image = self.scheduler.step(model_output, t, image).prev_sample
 
         image = (image / 2 + 0.5).clip(0, 1)
         image = image.transpose([0, 2, 3, 1]).numpy()
         if output_type == "pil":
             image = self.numpy_to_pil(image)
 
         if not return_dict:
-            return (image, )
+            return (image,)
 
         return ImagePipelineOutput(images=image)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/pipelines/ddpm/__init__.py` & `ppdiffusers-0.9.0/ppdiffusers/pipelines/ddpm/__init__.py`

 * *Files identical despite different names*

### Comparing `ppdiffusers-0.6.3/ppdiffusers/pipelines/ddpm/pipeline_ddpm.py` & `ppdiffusers-0.9.0/ppdiffusers/pipelines/score_sde_ve/pipeline_score_sde_ve.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,88 +7,94 @@
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
-
 # limitations under the License.
 
 from typing import Optional, Tuple, Union
 
 import paddle
 
+from ...models import UNet2DModel
 from ...pipeline_utils import DiffusionPipeline, ImagePipelineOutput
+from ...schedulers import ScoreSdeVeScheduler
 
 
-class DDPMPipeline(DiffusionPipeline):
+class ScoreSdeVePipeline(DiffusionPipeline):
     r"""
-    This model inherits from [`DiffusionPipeline`]. Check the superclass documentation for the generic methods the
-    library implements for all the pipelines (such as downloading or saving, running on a particular device, etc.)
-
     Parameters:
-        unet ([`UNet2DModel`]): U-Net architecture to denoise the encoded image.
-        scheduler ([`SchedulerMixin`]):
-            A scheduler to be used in combination with `unet` to denoise the encoded image. Can be one of
-            [`DDPMScheduler`], or [`DDIMScheduler`].
+    This model inherits from [`DiffusionPipeline`]. Check the superclass documentation for the generic methods the
+    library implements for all the pipelines (such as downloading or saving, running on a particular xxxx, etc.)
+        unet ([`UNet2DModel`]): U-Net architecture to denoise the encoded image. scheduler ([`SchedulerMixin`]):
+            The [`ScoreSdeVeScheduler`] scheduler to be used in combination with `unet` to denoise the encoded image.
     """
+    unet: UNet2DModel
+    scheduler: ScoreSdeVeScheduler
 
-    def __init__(self, unet, scheduler):
+    def __init__(self, unet: UNet2DModel, scheduler: DiffusionPipeline):
         super().__init__()
         self.register_modules(unet=unet, scheduler=scheduler)
 
     @paddle.no_grad()
     def __call__(
         self,
         batch_size: int = 1,
-        seed: Optional[int] = None,
-        num_inference_steps: int = 1000,
+        num_inference_steps: int = 2000,
+        generator: Optional[paddle.Generator] = None,
         output_type: Optional[str] = "pil",
         return_dict: bool = True,
         **kwargs,
     ) -> Union[ImagePipelineOutput, Tuple]:
         r"""
         Args:
             batch_size (`int`, *optional*, defaults to 1):
                 The number of images to generate.
-            seed (`int`, *optional*):
-                A random seed.
-            num_inference_steps (`int`, *optional*, defaults to 1000):
-                The number of denoising steps. More denoising steps usually lead to a higher quality image at the
-                expense of slower inference.
+            generator (`paddle.Generator`, *optional*):
+                A [paddle generator] to make generation deterministic.
             output_type (`str`, *optional*, defaults to `"pil"`):
                 The output format of the generate image. Choose between
                 [PIL](https://pillow.readthedocs.io/en/stable/): `PIL.Image.Image` or `np.array`.
             return_dict (`bool`, *optional*, defaults to `True`):
                 Whether or not to return a [`~pipeline_utils.ImagePipelineOutput`] instead of a plain tuple.
 
         Returns:
             [`~pipeline_utils.ImagePipelineOutput`] or `tuple`: [`~pipelines.utils.ImagePipelineOutput`] if
             `return_dict` is True, otherwise a `tuple. When returning a tuple, the first element is a list with the
             generated images.
         """
-        if seed is not None:
-            paddle.seed(seed)
-        # Sample gaussian noise to begin loop
-        image = paddle.randn((batch_size, self.unet.in_channels,
-                              self.unet.sample_size, self.unet.sample_size))
 
-        # set step values
+        img_size = self.unet.config.sample_size
+        shape = (batch_size, 3, img_size, img_size)
+
+        model = self.unet
+
+        sample = paddle.randn(shape, generator=generator) * self.scheduler.init_noise_sigma
+
         self.scheduler.set_timesteps(num_inference_steps)
+        self.scheduler.set_sigmas(num_inference_steps)
+
+        for i, t in enumerate(self.progress_bar(self.scheduler.timesteps)):
+            sigma_t = self.scheduler.sigmas[i] * paddle.ones((shape[0],))
+
+            # correction step
+            for _ in range(self.scheduler.config.correct_steps):
+                model_output = self.unet(sample, sigma_t).sample
+                sample = self.scheduler.step_correct(model_output, sample, generator=generator).prev_sample
 
-        for t in self.progress_bar(self.scheduler.timesteps):
-            # 1. predict noise model_output
-            model_output = self.unet(image, t).sample
+            # prediction step
+            model_output = model(sample, sigma_t).sample
+            output = self.scheduler.step_pred(model_output, t, sample, generator=generator)
 
-            # 2. compute previous image: x_t -> x_t-1
-            image = self.scheduler.step(model_output, t, image).prev_sample
+            sample, sample_mean = output.prev_sample, output.prev_sample_mean
 
-        image = (image / 2 + 0.5).clip(0, 1)
-        image = image.transpose([0, 2, 3, 1]).numpy()
+        sample = sample_mean.clip(0, 1)
+        sample = sample.transpose([0, 2, 3, 1]).numpy()
         if output_type == "pil":
-            image = self.numpy_to_pil(image)
+            sample = self.numpy_to_pil(sample)
 
         if not return_dict:
-            return (image, )
+            return (sample,)
 
-        return ImagePipelineOutput(images=image)
+        return ImagePipelineOutput(images=sample)
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/pipelines/latent_diffusion/__init__.py` & `ppdiffusers-0.9.0/ppdiffusers/pipelines/pndm/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,12 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # flake8: noqa
-from ...utils import is_paddlenlp_available
-
-if is_paddlenlp_available():
-    from .pipeline_latent_diffusion import LDMBertModel, LDMTextToImagePipeline
-    from .pipeline_latent_diffusion_superresolution import LDMSuperResolutionPipeline
+from .pipeline_pndm import PNDMPipeline
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/pipelines/latent_diffusion/pipeline_latent_diffusion.py` & `ppdiffusers-0.9.0/ppdiffusers/pipelines/latent_diffusion/pipeline_latent_diffusion.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,62 +10,70 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import inspect
-from typing import Callable, List, Optional, Tuple, Union
+from typing import Callable, List, Optional, Union
 
 import paddle
 import paddle.nn as nn
+
+################################################################################
+# Code for the text transformer model
+################################################################################
+from paddlenlp.transformers import (
+    PretrainedModel,
+    PretrainedTokenizer,
+    register_base_model,
+)
+from paddlenlp.transformers.model_outputs import (
+    BaseModelOutputWithPoolingAndCrossAttentions,
+)
+
 from ...configuration_utils import FrozenDict
 from ...models import AutoencoderKL, UNet2DConditionModel, UNet2DModel, VQModel
 from ...pipeline_utils import DiffusionPipeline, ImagePipelineOutput
-from ...schedulers import DDIMScheduler, LMSDiscreteScheduler, PNDMScheduler
+from ...schedulers import (
+    DDIMScheduler,
+    DPMSolverMultistepScheduler,
+    EulerAncestralDiscreteScheduler,
+    EulerDiscreteScheduler,
+    LMSDiscreteScheduler,
+    PNDMScheduler,
+)
 from ...utils import deprecate, logging
 
 logger = logging.get_logger(__name__)  # pylint: disable=invalid-name
 
-################################################################################
-# Code for the text transformer model
-################################################################################
-""" 
-Paddle LDMBERT model.
-"""
-from paddlenlp.transformers import PretrainedModel, register_base_model, PretrainedTokenizer
-from paddlenlp.transformers.model_outputs import BaseModelOutputWithPoolingAndCrossAttentions
-
 
 class LDMBertPretrainedModel(PretrainedModel):
     pretrained_init_configuration = {}
     pretrained_resource_files_map = {}
     base_model_prefix = "ldmbert"
 
     def init_weights(self, layer):
         if isinstance(layer, (nn.Linear, nn.Embedding)):
             layer.weight.set_value(
-                paddle.normal(mean=0.0,
-                              std=self.initializer_range if hasattr(
-                                  self, "initializer_range") else
-                              self.ldmbert.config["initializer_range"],
-                              shape=layer.weight.shape))
+                paddle.normal(
+                    mean=0.0,
+                    std=self.initializer_range
+                    if hasattr(self, "initializer_range")
+                    else self.ldmbert.config["initializer_range"],
+                    shape=layer.weight.shape,
+                )
+            )
 
 
 class LDMBertEmbeddings(nn.Layer):
-
-    def __init__(self,
-                 vocab_size,
-                 hidden_size=768,
-                 hidden_dropout_prob=0.0,
-                 max_position_embeddings=512):
+    def __init__(self, vocab_size, hidden_size=768, hidden_dropout_prob=0.0, max_position_embeddings=512):
         super().__init__()
         self.word_embeddings = nn.Embedding(vocab_size, hidden_size)
-        self.position_embeddings = nn.Embedding(max_position_embeddings,
-                                                hidden_size)
+        self.position_embeddings = nn.Embedding(max_position_embeddings, hidden_size)
         self.dropout = nn.Dropout(hidden_dropout_prob)
 
     def forward(self, input_ids, position_ids=None):
         if position_ids is None:
             ones = paddle.ones_like(input_ids, dtype="int64")
             seq_length = paddle.cumsum(ones, axis=-1)
             position_ids = seq_length - ones
@@ -76,172 +84,172 @@
 
         embeddings = input_embedings + position_embeddings
         embeddings = self.dropout(embeddings)
         return embeddings
 
 
 class TransformerEncoderLayer(nn.TransformerEncoderLayer):
-
-    def __init__(self,
-                 d_model,
-                 nhead,
-                 dim_feedforward,
-                 dropout=0.1,
-                 activation="gelu",
-                 attn_dropout=None,
-                 act_dropout=None,
-                 normalize_before=False,
-                 weight_attr=None,
-                 bias_attr=None,
-                 head_dim=64):
-        super().__init__(d_model, nhead, dim_feedforward, dropout, activation,
-                         attn_dropout, act_dropout, normalize_before,
-                         weight_attr, bias_attr)
+    def __init__(
+        self,
+        d_model,
+        nhead,
+        dim_feedforward,
+        dropout=0.1,
+        activation="gelu",
+        attn_dropout=None,
+        act_dropout=None,
+        normalize_before=False,
+        weight_attr=None,
+        bias_attr=None,
+        head_dim=64,
+    ):
+        super().__init__(
+            d_model,
+            nhead,
+            dim_feedforward,
+            dropout,
+            activation,
+            attn_dropout,
+            act_dropout,
+            normalize_before,
+            weight_attr,
+            bias_attr,
+        )
         # update self attn
-        self.self_attn = LDMBertAttention(d_model,
-                                          head_dim,
-                                          nhead,
-                                          dropout=attn_dropout,
-                                          weight_attr=weight_attr,
-                                          bias_attr=False)
+        self.self_attn = LDMBertAttention(
+            d_model, head_dim, nhead, dropout=attn_dropout, weight_attr=weight_attr, bias_attr=False
+        )
 
 
 @register_base_model
 class LDMBertModel(LDMBertPretrainedModel):
+    _no_split_modules = []
 
-    def __init__(self,
-                 vocab_size=30522,
-                 max_position_embeddings=77,
-                 encoder_layers=32,
-                 encoder_ffn_dim=5120,
-                 encoder_attention_heads=8,
-                 head_dim=64,
-                 activation_function="gelu",
-                 d_model=1280,
-                 dropout=0.0,
-                 attention_dropout=0.0,
-                 activation_dropout=0.0,
-                 init_std=0.02,
-                 pad_token_id=0,
-                 **kwargs):
+    def __init__(
+        self,
+        vocab_size=30522,
+        max_position_embeddings=77,
+        encoder_layers=32,
+        encoder_ffn_dim=5120,
+        encoder_attention_heads=8,
+        head_dim=64,
+        activation_function="gelu",
+        d_model=1280,
+        dropout=0.0,
+        attention_dropout=0.0,
+        activation_dropout=0.0,
+        init_std=0.02,
+        pad_token_id=0,
+        **kwargs
+    ):
         super().__init__()
         self.pad_token_id = pad_token_id
         self.initializer_range = init_std
-        self.embeddings = LDMBertEmbeddings(vocab_size, d_model, dropout,
-                                            max_position_embeddings)
-        encoder_layer = TransformerEncoderLayer(d_model,
-                                                encoder_attention_heads,
-                                                encoder_ffn_dim,
-                                                dropout=dropout,
-                                                activation=activation_function,
-                                                attn_dropout=attention_dropout,
-                                                act_dropout=activation_dropout,
-                                                normalize_before=True,
-                                                head_dim=head_dim)
+        self.embeddings = LDMBertEmbeddings(vocab_size, d_model, dropout, max_position_embeddings)
+        encoder_layer = TransformerEncoderLayer(
+            d_model,
+            encoder_attention_heads,
+            encoder_ffn_dim,
+            dropout=dropout,
+            activation=activation_function,
+            attn_dropout=attention_dropout,
+            act_dropout=activation_dropout,
+            normalize_before=True,
+            head_dim=head_dim,
+        )
 
         self.encoder = nn.TransformerEncoder(encoder_layer, encoder_layers)
         self.final_layer_norm = nn.LayerNorm(d_model)
         self.apply(self.init_weights)
 
     def get_input_embeddings(self):
         return self.embeddings.word_embeddings
 
     def set_input_embeddings(self, value):
         self.embeddings.word_embeddings = value
 
-    def forward(self,
-                input_ids,
-                position_ids=None,
-                attention_mask=None,
-                output_hidden_states=False,
-                output_attentions=False,
-                return_dict=False):
+    def forward(
+        self,
+        input_ids,
+        position_ids=None,
+        attention_mask=None,
+        output_hidden_states=False,
+        output_attentions=False,
+        return_dict=False,
+    ):
 
         if attention_mask is not None and attention_mask.ndim == 2:
             # attention_mask [batch_size, sequence_length] -> [batch_size, 1, 1, sequence_length]
-            attention_mask = attention_mask.unsqueeze(axis=[1, 2]).astype(
-                paddle.get_default_dtype())
+            attention_mask = attention_mask.unsqueeze(axis=[1, 2]).astype(paddle.get_default_dtype())
             attention_mask = (1.0 - attention_mask) * -1e4
 
-        embedding_output = self.embeddings(input_ids=input_ids,
-                                           position_ids=position_ids)
+        embedding_output = self.embeddings(input_ids=input_ids, position_ids=position_ids)
 
         encoder_outputs = self.encoder(
             embedding_output,
             src_mask=attention_mask,
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
-            return_dict=return_dict)
+            return_dict=return_dict,
+        )
 
         if isinstance(encoder_outputs, type(embedding_output)):
             sequence_output = self.final_layer_norm(encoder_outputs)
-            return (sequence_output, )
+            return (sequence_output,)
         else:
             sequence_output = encoder_outputs[0]
             sequence_output = self.final_layer_norm(sequence_output)
             if not return_dict:
-                return (sequence_output, ) + encoder_outputs[1:]
+                return (sequence_output,) + encoder_outputs[1:]
             return BaseModelOutputWithPoolingAndCrossAttentions(
                 last_hidden_state=sequence_output,
                 hidden_states=encoder_outputs.hidden_states,
-                attentions=encoder_outputs.attentions)
+                attentions=encoder_outputs.attentions,
+            )
 
 
 class LDMBertAttention(nn.MultiHeadAttention):
-
-    def __init__(self,
-                 embed_dim,
-                 head_dim,
-                 num_heads,
-                 dropout=0.,
-                 kdim=None,
-                 vdim=None,
-                 need_weights=False,
-                 weight_attr=None,
-                 bias_attr=None):
-        super().__init__(embed_dim, num_heads, dropout, kdim, vdim,
-                         need_weights, weight_attr, bias_attr)
-        assert embed_dim > 0, ("Expected embed_dim to be greater than 0, "
-                               "but recieved {}".format(embed_dim))
-        assert num_heads > 0, ("Expected num_heads to be greater than 0, "
-                               "but recieved {}".format(num_heads))
+    def __init__(
+        self,
+        embed_dim,
+        head_dim,
+        num_heads,
+        dropout=0.0,
+        kdim=None,
+        vdim=None,
+        need_weights=False,
+        weight_attr=None,
+        bias_attr=None,
+    ):
+        super().__init__(embed_dim, num_heads, dropout, kdim, vdim, need_weights, weight_attr, bias_attr)
+        assert embed_dim > 0, "Expected embed_dim to be greater than 0, " "but recieved {}".format(embed_dim)
+        assert num_heads > 0, "Expected num_heads to be greater than 0, " "but recieved {}".format(num_heads)
 
         self.embed_dim = embed_dim
         self.kdim = kdim if kdim is not None else embed_dim
         self.vdim = vdim if vdim is not None else embed_dim
         self.num_heads = num_heads
         self.dropout = dropout
         self.need_weights = need_weights
 
         self.head_dim = head_dim
         self.inner_dim = head_dim * num_heads
         self.scaling = self.head_dim**-0.5
 
-        self.q_proj = nn.Linear(embed_dim,
-                                self.inner_dim,
-                                weight_attr,
-                                bias_attr=bias_attr)
-        self.k_proj = nn.Linear(self.kdim,
-                                self.inner_dim,
-                                weight_attr,
-                                bias_attr=bias_attr)
-        self.v_proj = nn.Linear(self.vdim,
-                                self.inner_dim,
-                                weight_attr,
-                                bias_attr=bias_attr)
+        self.q_proj = nn.Linear(embed_dim, self.inner_dim, weight_attr, bias_attr=bias_attr)
+        self.k_proj = nn.Linear(self.kdim, self.inner_dim, weight_attr, bias_attr=bias_attr)
+        self.v_proj = nn.Linear(self.vdim, self.inner_dim, weight_attr, bias_attr=bias_attr)
         self.out_proj = nn.Linear(self.inner_dim, embed_dim, weight_attr)
 
 
 class LDMBertModelForMaskedLM(LDMBertPretrainedModel):
-
     def __init__(self, ldmbert):
         super().__init__()
         self.ldmbert = ldmbert
-        self.to_logits = nn.Linear(ldmbert.config["hidden_size"],
-                                   ldmbert.config["vocab_size"])
+        self.to_logits = nn.Linear(ldmbert.config["hidden_size"], ldmbert.config["vocab_size"])
         self.apply(self.init_weights)
 
     def forward(
         self,
         input_ids=None,
         attention_mask=None,
         position_ids=None,
@@ -259,117 +267,291 @@
         )
         return outputs
 
 
 class LDMTextToImagePipeline(DiffusionPipeline):
     r"""
     This model inherits from [`DiffusionPipeline`]. Check the superclass documentation for the generic methods the
-    library implements for all the pipelines (such as downloading or saving, running on a particular device, etc.)
+    library implements for all the pipelines (such as downloading or saving, running on a particular xxxx, etc.)
 
     Parameters:
         vqvae ([`VQModel`]):
             Vector-quantized (VQ) Model to encode and decode images to and from latent representations.
         bert ([`LDMBertModel`]):
             Text-encoder model based on [BERT](https://paddlenlp.readthedocs.io/zh/latest/source/paddlenlp.transformers.bert.modeling.html#paddlenlp.transformers.bert.modeling.BertModel) architecture.
         tokenizer (`paddlenlp.transformers.BertTokenizer`):
             Tokenizer of class
             [BertTokenizer](https://paddlenlp.readthedocs.io/zh/latest/source/paddlenlp.transformers.bert.tokenizer.html#paddlenlp.transformers.bert.tokenizer.BertTokenizer).
         unet ([`UNet2DConditionModel`]): Conditional U-Net architecture to denoise the encoded image latents.
         scheduler ([`SchedulerMixin`]):
-            A scheduler to be used in combination with `unet` to denoise the encoded image latens. Can be one of
-            [`DDIMScheduler`], [`LMSDiscreteScheduler`], or [`PNDMScheduler`].
+            A scheduler to be used in combination with `unet` to denoise the encoded image latents. Can be one of
+            [`DDIMScheduler`], [`LMSDiscreteScheduler`], [`PNDMScheduler`], [`EulerDiscreteScheduler`], [`EulerAncestralDiscreteScheduler`]
+            or [`DPMSolverMultistepScheduler`].
     """
 
     def __init__(
         self,
         vqvae: Union[VQModel, AutoencoderKL],
         bert: PretrainedModel,
         tokenizer: PretrainedTokenizer,
         unet: Union[UNet2DModel, UNet2DConditionModel],
-        scheduler: Union[DDIMScheduler, PNDMScheduler, LMSDiscreteScheduler],
+        scheduler: Union[
+            DDIMScheduler,
+            PNDMScheduler,
+            LMSDiscreteScheduler,
+            EulerDiscreteScheduler,
+            EulerAncestralDiscreteScheduler,
+            DPMSolverMultistepScheduler,
+        ],
     ):
         super().__init__()
-        if hasattr(scheduler.config,
-                   "steps_offset") and scheduler.config.steps_offset != 1:
+        if hasattr(scheduler.config, "steps_offset") and scheduler.config.steps_offset != 1:
             deprecation_message = (
                 f"The configuration file of this scheduler: {scheduler} is outdated. `steps_offset`"
                 f" should be set to 1 instead of {scheduler.config.steps_offset}. Please make sure "
                 "to update the config accordingly as leaving `steps_offset` might led to incorrect results"
                 " in future versions. If you have downloaded this checkpoint from the Hugging Face Hub,"
                 " it would be very nice if you could open a Pull request for the `scheduler/scheduler_config.json`"
-                " file")
-            deprecate("steps_offset!=1",
-                      "1.0.0",
-                      deprecation_message,
-                      standard_warn=False)
+                " file"
+            )
+            deprecate("steps_offset!=1", "1.0.0", deprecation_message, standard_warn=False)
             new_config = dict(scheduler.config)
             new_config["steps_offset"] = 1
             scheduler._internal_dict = FrozenDict(new_config)
 
-        self.register_modules(vqvae=vqvae,
-                              bert=bert,
-                              tokenizer=tokenizer,
-                              unet=unet,
-                              scheduler=scheduler)
-
-    def enable_attention_slicing(self,
-                                 slice_size: Optional[Union[str,
-                                                            int]] = "auto"):
+        if hasattr(scheduler.config, "clip_sample") and scheduler.config.clip_sample is True:
+            deprecation_message = (
+                f"The configuration file of this scheduler: {scheduler} has not set the configuration `clip_sample`."
+                " `clip_sample` should be set to False in the configuration file. Please make sure to update the"
+                " config accordingly as not setting `clip_sample` in the config might lead to incorrect results in"
+                " future versions. If you have downloaded this checkpoint from the Hugging Face Hub, it would be very"
+                " nice if you could open a Pull request for the `scheduler/scheduler_config.json` file"
+            )
+            deprecate("clip_sample not set", "1.0.0", deprecation_message, standard_warn=False)
+            new_config = dict(scheduler.config)
+            new_config["clip_sample"] = False
+            scheduler._internal_dict = FrozenDict(new_config)
+
+        self.register_modules(vqvae=vqvae, bert=bert, tokenizer=tokenizer, unet=unet, scheduler=scheduler)
+        self.vae_scale_factor = 2 ** (len(self.vqvae.config.block_out_channels) - 1)
+
+    def enable_attention_slicing(self, slice_size: Optional[Union[str, int]] = "auto"):
         r"""
         Enable sliced attention computation.
 
         When this option is enabled, the attention module will split the input tensor in slices, to compute attention
         in several steps. This is useful to save some memory in exchange for a small speed decrease.
 
         Args:
             slice_size (`str` or `int`, *optional*, defaults to `"auto"`):
                 When `"auto"`, halves the input to the attention heads, so attention will be computed in two steps. If
                 a number is provided, uses as many slices as `attention_head_dim // slice_size`. In this case,
                 `attention_head_dim` must be a multiple of `slice_size`.
         """
         if slice_size == "auto":
-            # half the attention head size is usually a good trade-off between
-            # speed and memory
-            slice_size = self.unet.config.attention_head_dim // 2
+            if isinstance(self.unet.config.attention_head_dim, int):
+                # half the attention head size is usually a good trade-off between
+                # speed and memory
+                slice_size = self.unet.config.attention_head_dim // 2
+            else:
+                # if `attention_head_dim` is a list, take the smallest head size
+                slice_size = min(self.unet.config.attention_head_dim)
         self.unet.set_attention_slice(slice_size)
 
     def disable_attention_slicing(self):
         r"""
         Disable sliced attention computation. If `enable_attention_slicing` was previously invoked, this method will go
         back to computing attention in one step.
         """
         # set slice_size = `None` to disable `attention slicing`
         self.enable_attention_slicing(None)
 
+    def _encode_prompt(self, prompt, num_images_per_prompt, do_classifier_free_guidance, negative_prompt):
+        r"""
+        Encodes the prompt into text encoder hidden states.
+
+        Args:
+            prompt (`str` or `list(int)`):
+                prompt to be encoded
+            num_images_per_prompt (`int`):
+                number of images that should be generated per prompt
+            do_classifier_free_guidance (`bool`):
+                whether to use classifier free guidance or not
+            negative_prompt (`str` or `List[str]`):
+                The prompt or prompts not to guide the image generation. Ignored when not using guidance (i.e., ignored
+                if `guidance_scale` is less than `1`).
+        """
+        batch_size = len(prompt) if isinstance(prompt, list) else 1
+
+        text_inputs = self.tokenizer(
+            prompt,
+            padding="max_length",
+            max_length=self.tokenizer.model_max_length,
+            truncation=True,
+            return_tensors="pd",
+        )
+        text_input_ids = text_inputs.input_ids
+        untruncated_ids = self.tokenizer(prompt, padding="max_length", return_tensors="pd").input_ids
+
+        if not paddle.equal_all(text_input_ids, untruncated_ids):
+            removed_text = self.tokenizer.batch_decode(untruncated_ids[:, self.tokenizer.model_max_length - 1 : -1])
+            logger.warning(
+                "The following part of your input was truncated because LDMBert can only handle sequences up to"
+                f" {self.tokenizer.model_max_length} tokens: {removed_text}"
+            )
+
+        if self.bert.config.get("use_attention_mask", None) is not None and self.bert.config["use_attention_mask"]:
+            attention_mask = text_inputs.attention_mask
+        else:
+            attention_mask = None
+
+        text_embeddings = self.bert(
+            text_input_ids,
+            attention_mask=attention_mask,
+        )
+        text_embeddings = text_embeddings[0]
+
+        # duplicate text embeddings for each generation per prompt, using mps friendly method
+        bs_embed, seq_len, _ = text_embeddings.shape
+        text_embeddings = text_embeddings.tile([1, num_images_per_prompt, 1])
+        text_embeddings = text_embeddings.reshape([bs_embed * num_images_per_prompt, seq_len, -1])
+
+        # get unconditional embeddings for classifier free guidance
+        if do_classifier_free_guidance:
+            uncond_tokens: List[str]
+            if negative_prompt is None:
+                uncond_tokens = [""] * batch_size
+            elif type(prompt) is not type(negative_prompt):
+                raise TypeError(
+                    f"`negative_prompt` should be the same type to `prompt`, but got {type(negative_prompt)} !="
+                    f" {type(prompt)}."
+                )
+            elif isinstance(negative_prompt, str):
+                uncond_tokens = [negative_prompt]
+            elif batch_size != len(negative_prompt):
+                raise ValueError(
+                    f"`negative_prompt`: {negative_prompt} has batch size {len(negative_prompt)}, but `prompt`:"
+                    f" {prompt} has batch size {batch_size}. Please make sure that passed `negative_prompt` matches"
+                    " the batch size of `prompt`."
+                )
+            else:
+                uncond_tokens = negative_prompt
+
+            max_length = text_input_ids.shape[-1]
+            uncond_input = self.tokenizer(
+                uncond_tokens,
+                padding="max_length",
+                max_length=max_length,
+                truncation=True,
+                return_tensors="pd",
+            )
+
+            if self.bert.config.get("use_attention_mask", None) is not None and self.bert.config["use_attention_mask"]:
+                attention_mask = uncond_input.attention_mask
+            else:
+                attention_mask = None
+
+            uncond_embeddings = self.bert(
+                uncond_input.input_ids,
+                attention_mask=attention_mask,
+            )
+            uncond_embeddings = uncond_embeddings[0]
+
+            # duplicate unconditional embeddings for each generation per prompt, using mps friendly method
+            seq_len = uncond_embeddings.shape[1]
+            uncond_embeddings = uncond_embeddings.tile([1, num_images_per_prompt, 1])
+            uncond_embeddings = uncond_embeddings.reshape([batch_size * num_images_per_prompt, seq_len, -1])
+
+            # For classifier free guidance, we need to do two forward passes.
+            # Here we concatenate the unconditional and text embeddings into a single batch
+            # to avoid doing two forward passes
+            text_embeddings = paddle.concat([uncond_embeddings, text_embeddings])
+
+        return text_embeddings
+
+    def decode_latents(self, latents):
+        latents = 1 / 0.18215 * latents
+        image = self.vqvae.decode(latents).sample
+        image = (image / 2 + 0.5).clip(0, 1)
+        # we always cast to float32 as this does not cause significant overhead and is compatible with bfloa16
+        image = image.transpose([0, 2, 3, 1]).cast("float32").numpy()
+        return image
+
+    def prepare_extra_step_kwargs(self, generator, eta):
+        # prepare extra kwargs for the scheduler step, since not all schedulers have the same signature
+        # eta (η) is only used with the DDIMScheduler, it will be ignored for other schedulers.
+        # eta corresponds to η in DDIM paper: https://arxiv.org/abs/2010.02502
+        # and should be between [0, 1]
+
+        accepts_eta = "eta" in set(inspect.signature(self.scheduler.step).parameters.keys())
+        extra_step_kwargs = {}
+        if accepts_eta:
+            extra_step_kwargs["eta"] = eta
+
+        # check if the scheduler accepts generator
+        accepts_generator = "generator" in set(inspect.signature(self.scheduler.step).parameters.keys())
+        if accepts_generator:
+            extra_step_kwargs["generator"] = generator
+        return extra_step_kwargs
+
+    def check_inputs(self, prompt, height, width, callback_steps):
+        if not isinstance(prompt, str) and not isinstance(prompt, list):
+            raise ValueError(f"`prompt` has to be of type `str` or `list` but is {type(prompt)}")
+
+        if height % 8 != 0 or width % 8 != 0:
+            raise ValueError(f"`height` and `width` have to be divisible by 8 but are {height} and {width}.")
+
+        if (callback_steps is None) or (
+            callback_steps is not None and (not isinstance(callback_steps, int) or callback_steps <= 0)
+        ):
+            raise ValueError(
+                f"`callback_steps` has to be a positive integer but is {callback_steps} of type"
+                f" {type(callback_steps)}."
+            )
+
+    def prepare_latents(self, batch_size, num_channels_latents, height, width, dtype, generator, latents=None):
+        shape = [batch_size, num_channels_latents, height // self.vae_scale_factor, width // self.vae_scale_factor]
+        if latents is None:
+            latents = paddle.randn(shape, generator=generator, dtype=dtype)
+        else:
+            if latents.shape != shape:
+                raise ValueError(f"Unexpected latents shape, got {latents.shape}, expected {shape}")
+
+        # scale the initial noise by the standard deviation required by the scheduler
+        latents = latents * self.scheduler.init_noise_sigma
+        return latents
+
     @paddle.no_grad()
     def __call__(
         self,
         prompt: Union[str, List[str]],
-        height: Optional[int] = 256,
-        width: Optional[int] = 256,
-        num_inference_steps: Optional[int] = 50,
-        guidance_scale: Optional[float] = 1.0,
+        height: Optional[int] = None,
+        width: Optional[int] = None,
+        num_inference_steps: int = 50,
+        guidance_scale: float = 1.0,
         negative_prompt: Optional[Union[str, List[str]]] = None,
         num_images_per_prompt: Optional[int] = 1,
-        eta: Optional[float] = 0.0,
-        seed: Optional[int] = None,
+        eta: float = 0.0,
+        generator: Optional[paddle.Generator] = None,
         latents: Optional[paddle.Tensor] = None,
         output_type: Optional[str] = "pil",
         return_dict: bool = True,
         callback: Optional[Callable[[int, int, paddle.Tensor], None]] = None,
         callback_steps: Optional[int] = 1,
         **kwargs,
-    ) -> Union[Tuple, ImagePipelineOutput]:
+    ):
         r"""
+        Function invoked when calling the pipeline for generation.
+
         Args:
             prompt (`str` or `List[str]`):
                 The prompt or prompts to guide the image generation.
-            height (`int`, *optional*, defaults to 256):
+            height (`int`, *optional*, defaults to self.unet.config.sample_size * self.vae_scale_factor):
                 The height in pixels of the generated image.
-            width (`int`, *optional*, defaults to 256):
+            width (`int`, *optional*, defaults to self.unet.config.sample_size * self.vae_scale_factor):
                 The width in pixels of the generated image.
             num_inference_steps (`int`, *optional*, defaults to 50):
                 The number of denoising steps. More denoising steps usually lead to a higher quality image at the
                 expense of slower inference.
             guidance_scale (`float`, *optional*, defaults to 1.0):
                 Guidance scale as defined in [Classifier-Free Diffusion Guidance](https://arxiv.org/abs/2207.12598).
                 `guidance_scale` is defined as `w` of equation 2. of [Imagen
@@ -380,203 +562,103 @@
                 The prompt or prompts not to guide the image generation. Ignored when not using guidance (i.e., ignored
                 if `guidance_scale` is less than `1`).
             num_images_per_prompt (`int`, *optional*, defaults to 1):
                 The number of images to generate per prompt.
             eta (`float`, *optional*, defaults to 0.0):
                 Corresponds to parameter eta (η) in the DDIM paper: https://arxiv.org/abs/2010.02502. Only applies to
                 [`schedulers.DDIMScheduler`], will be ignored for others.
-            seed (`int`, *optional*):
-                Random number seed.
+            generator (`paddle.Generator`, *optional*):
+                A [paddle generator] to make generation deterministic.
             latents (`paddle.Tensor`, *optional*):
                 Pre-generated noisy latents, sampled from a Gaussian distribution, to be used as inputs for image
                 generation. Can be used to tweak the same generation with different prompts. If not provided, a latents
-                tensor will ge generated by sampling using the supplied random `seed`.
+                tensor will ge generated by sampling using the supplied random `generator`.
             output_type (`str`, *optional*, defaults to `"pil"`):
                 The output format of the generate image. Choose between
                 [PIL](https://pillow.readthedocs.io/en/stable/): `PIL.Image.Image` or `np.array`.
             return_dict (`bool`, *optional*, defaults to `True`):
-                Whether or not to return a [`~pipeline_utils.ImagePipelineOutput`] instead of a
+                Whether or not to return a [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] instead of a
                 plain tuple.
             callback (`Callable`, *optional*):
                 A function that will be called every `callback_steps` steps during inference. The function will be
                 called with the following arguments: `callback(step: int, timestep: int, latents: paddle.Tensor)`.
             callback_steps (`int`, *optional*, defaults to 1):
                 The frequency at which the `callback` function will be called. If not specified, the callback will be
                 called at every step.
-                
+
         Returns:
-            [`~pipeline_utils.ImagePipelineOutput`] or `tuple`: [`~pipeline_utils.ImagePipelineOutput`] if
-            `return_dict` is True, otherwise a `tuple. When returning a tuple, the first element is a list with the
-            generated images.
+            [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] or `tuple`:
+            [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] if `return_dict` is True, otherwise a `tuple.
+            When returning a tuple, the first element is a list with the generated images, and the second element is a
+            list of `bool`s denoting whether the corresponding generated image likely represents "not-safe-for-work"
+            (nsfw) content, according to the `safety_checker`.
         """
-        if isinstance(prompt, str):
-            batch_size = 1
-        elif isinstance(prompt, list):
-            batch_size = len(prompt)
-        else:
-            raise ValueError(
-                f"`prompt` has to be of type `str` or `list` but is {type(prompt)}"
-            )
-
-        if height % 8 != 0 or width % 8 != 0:
-            raise ValueError(
-                f"`height` and `width` have to be divisible by 8 but are {height} and {width}."
-            )
+        # 0. Default height and width to unet
+        height = height or self.unet.config.sample_size * self.vae_scale_factor
+        width = width or self.unet.config.sample_size * self.vae_scale_factor
 
-        if (callback_steps is None) or (callback_steps is not None and
-                                        (not isinstance(callback_steps, int)
-                                         or callback_steps <= 0)):
-            raise ValueError(
-                f"`callback_steps` has to be a positive integer but is {callback_steps} of type"
-                f" {type(callback_steps)}.")
-
-        # get prompt text embeddings
-        text_inputs = self.tokenizer(
-            prompt,
-            padding="max_length",
-            max_length=self.tokenizer.model_max_length,
-            return_tensors="pd",
-        )
-        text_input_ids = text_inputs.input_ids
-
-        if text_input_ids.shape[-1] > self.tokenizer.model_max_length:
-            removed_text = self.tokenizer.batch_decode(
-                text_input_ids[:, self.tokenizer.model_max_length:])
-            logger.warning(
-                "The following part of your input was truncated because CLIP can only handle sequences up to"
-                f" {self.tokenizer.model_max_length} tokens: {removed_text}")
-            text_input_ids = text_input_ids[:, :self.tokenizer.model_max_length]
-        text_embeddings = self.bert(text_input_ids)[0]
-
-        # duplicate text embeddings for each generation per prompt, using mps friendly method
-        bs_embed, seq_len, _ = text_embeddings.shape
-        text_embeddings = text_embeddings.tile([1, num_images_per_prompt, 1])
-        text_embeddings = text_embeddings.reshape(
-            [bs_embed * num_images_per_prompt, seq_len, -1])
+        # 1. Check inputs. Raise error if not correct
+        self.check_inputs(prompt, height, width, callback_steps)
 
+        # 2. Define call parameters
+        batch_size = 1 if isinstance(prompt, str) else len(prompt)
         # here `guidance_scale` is defined analog to the guidance weight `w` of equation (2)
         # of the Imagen paper: https://arxiv.org/pdf/2205.11487.pdf . `guidance_scale = 1`
         # corresponds to doing no classifier free guidance.
         do_classifier_free_guidance = guidance_scale > 1.0
-        # get unconditional embeddings for classifier free guidance
-        if do_classifier_free_guidance:
-            uncond_tokens: List[str]
-            if negative_prompt is None:
-                uncond_tokens = [""]
-            elif type(prompt) is not type(negative_prompt):
-                raise TypeError(
-                    f"`negative_prompt` should be the same type to `prompt`, but got {type(negative_prompt)} !="
-                    f" {type(prompt)}.")
-            elif isinstance(negative_prompt, str):
-                uncond_tokens = [negative_prompt]
-            elif batch_size != len(negative_prompt):
-                raise ValueError(
-                    f"`negative_prompt`: {negative_prompt} has batch size {len(negative_prompt)}, but `prompt`:"
-                    f" {prompt} has batch size {batch_size}. Please make sure that passed `negative_prompt` matches"
-                    " the batch size of `prompt`.")
-            else:
-                uncond_tokens = negative_prompt
-
-            max_length = text_input_ids.shape[-1]
-            uncond_input = self.tokenizer(
-                uncond_tokens,
-                padding="max_length",
-                max_length=max_length,
-                truncation=True,
-                return_tensors="pd",
-            )
-            uncond_embeddings = self.bert(uncond_input.input_ids)[0]
-
-            # duplicate unconditional embeddings for each generation per prompt, using mps friendly method
-            seq_len = uncond_embeddings.shape[1]
-            uncond_embeddings = uncond_embeddings.tile(
-                [batch_size, num_images_per_prompt, 1])
-            uncond_embeddings = uncond_embeddings.reshape(
-                [batch_size * num_images_per_prompt, seq_len, -1])
-
-            # For classifier free guidance, we need to do two forward passes.
-            # Here we concatenate the unconditional and text embeddings into a single batch
-            # to avoid doing two forward passes
-            text_embeddings = paddle.concat(
-                [uncond_embeddings, text_embeddings])
-
-        # get the initial random noise unless the user supplied it
 
-        # Unlike in other pipelines, latents need to be generated in the target device
-        # for 1-to-1 results reproducibility with the CompVis implementation.
-        # However this currently doesn't work in `mps`.
-        latents_shape = [
-            batch_size * num_images_per_prompt, self.unet.in_channels,
-            height // 8, width // 8
-        ]
-        if latents is None:
-            if seed is not None:
-                paddle.seed(seed)
-
-            latents = paddle.randn(latents_shape, dtype=text_embeddings.dtype)
-        else:
-            if latents.shape != latents_shape:
-                raise ValueError(
-                    f"Unexpected latents shape, got {latents.shape}, expected {latents_shape}"
-                )
+        # 3. Encode input prompt
+        text_embeddings = self._encode_prompt(
+            prompt, num_images_per_prompt, do_classifier_free_guidance, negative_prompt
+        )
 
-        # set timesteps
+        # 4. Prepare timesteps
         self.scheduler.set_timesteps(num_inference_steps)
+        timesteps = self.scheduler.timesteps
 
-        # Some schedulers like PNDM have timesteps as arrays
-        # It's more optimized to move all timesteps to correct device beforehand
-        timesteps_tensor = self.scheduler.timesteps
+        # 5. Prepare latent variables
+        num_channels_latents = self.unet.in_channels
+        latents = self.prepare_latents(
+            batch_size * num_images_per_prompt,
+            num_channels_latents,
+            height,
+            width,
+            text_embeddings.dtype,
+            generator,
+            latents,
+        )
 
-        # scale the initial noise by the standard deviation required by the scheduler
-        latents = latents * self.scheduler.init_noise_sigma
+        # 6. Prepare extra step kwargs. TODO: Logic should ideally just be moved out of the pipeline
+        extra_step_kwargs = self.prepare_extra_step_kwargs(generator, eta)
 
-        # prepare extra kwargs for the scheduler step, since not all schedulers have the same signature
-        # eta (η) is only used with the DDIMScheduler, it will be ignored for other schedulers.
-        # eta corresponds to η in DDIM paper: https://arxiv.org/abs/2010.02502
-        # and should be between [0, 1]
-        accepts_eta = "eta" in set(
-            inspect.signature(self.scheduler.step).parameters.keys())
-        extra_step_kwargs = {}
-        if accepts_eta:
-            extra_step_kwargs["eta"] = eta
-
-        for i, t in enumerate(self.progress_bar(timesteps_tensor)):
+        # 7. Denoising loop
+        for i, t in enumerate(self.progress_bar(timesteps)):
             # expand the latents if we are doing classifier free guidance
-            latent_model_input = paddle.concat(
-                [latents] * 2) if do_classifier_free_guidance else latents
-            latent_model_input = self.scheduler.scale_model_input(
-                latent_model_input, t)
+            latent_model_input = paddle.concat([latents] * 2) if do_classifier_free_guidance else latents
+            latent_model_input = self.scheduler.scale_model_input(latent_model_input, t)
 
             # predict the noise residual
-            noise_pred = self.unet(latent_model_input,
-                                   t,
-                                   encoder_hidden_states=text_embeddings).sample
+            noise_pred = self.unet(latent_model_input, t, encoder_hidden_states=text_embeddings).sample
 
             # perform guidance
             if do_classifier_free_guidance:
                 noise_pred_uncond, noise_pred_text = noise_pred.chunk(2)
-                noise_pred = noise_pred_uncond + guidance_scale * (
-                    noise_pred_text - noise_pred_uncond)
+                noise_pred = noise_pred_uncond + guidance_scale * (noise_pred_text - noise_pred_uncond)
 
             # compute the previous noisy sample x_t -> x_t-1
-            latents = self.scheduler.step(noise_pred, t, latents,
-                                          **extra_step_kwargs).prev_sample
+            latents = self.scheduler.step(noise_pred, t, latents, **extra_step_kwargs).prev_sample
 
             # call the callback, if provided
             if callback is not None and i % callback_steps == 0:
                 callback(i, t, latents)
 
-        latents = 1 / 0.18215 * latents
-        image = self.vqvae.decode(latents).sample
-
-        image = (image / 2 + 0.5).clip(0, 1)
-
-        # we always cast to float32 as this does not cause significant overhead and is compatible with bfloa16
-        image = image.transpose([0, 2, 3, 1]).astype("float32").numpy()
+        # 8. Post-processing
+        image = self.decode_latents(latents)
 
+        # 9. Convert to PIL
         if output_type == "pil":
             image = self.numpy_to_pil(image)
 
         if not return_dict:
-            return (image, )
+            return (image,)
 
         return ImagePipelineOutput(images=image)
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/pipelines/latent_diffusion/pipeline_latent_diffusion_superresolution.py` & `ppdiffusers-0.9.0/ppdiffusers/pipelines/latent_diffusion/pipeline_latent_diffusion_superresolution.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (c) 2022 PaddlePaddle Authors. All Rights Reserved.
+# Copyright 2022 The HuggingFace Team. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,165 +11,164 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import inspect
 from typing import Optional, Tuple, Union
+
 import numpy as np
+import paddle
 import PIL
 
-import paddle
-import paddle.nn as nn
 from ...models import UNet2DModel, VQModel
 from ...pipeline_utils import DiffusionPipeline, ImagePipelineOutput
 from ...schedulers import (
     DDIMScheduler,
+    DPMSolverMultistepScheduler,
+    EulerAncestralDiscreteScheduler,
+    EulerDiscreteScheduler,
     LMSDiscreteScheduler,
     PNDMScheduler,
 )
-from paddlenlp.utils.tools import compare_version
-if compare_version(PIL.__version__, "9.1.0") >= 0:
-    Resampling = PIL.Image.Resampling
-else:
-    Resampling = PIL.Image
+from ...utils import PIL_INTERPOLATION
 
 
 def preprocess(image):
     w, h = image.size
     w, h = map(lambda x: x - x % 32, (w, h))  # resize to integer multiple of 32
-    image = image.resize((w, h), resample=Resampling.LANCZOS)
+    image = image.resize((w, h), resample=PIL_INTERPOLATION["lanczos"])
     image = np.array(image).astype(np.float32) / 255.0
     image = image[None].transpose(0, 3, 1, 2)
     image = paddle.to_tensor(image)
     return 2.0 * image - 1.0
 
 
 class LDMSuperResolutionPipeline(DiffusionPipeline):
     r"""
     A pipeline for image super-resolution using Latent
+
     This class inherits from [`DiffusionPipeline`]. Check the superclass documentation for the generic methods the
-    library implements for all the pipelines (such as downloading or saving, running on a particular device, etc.)
+    library implements for all the pipelines (such as downloading or saving, running on a particular xxxx, etc.)
 
     Parameters:
         vqvae ([`VQModel`]):
             Vector-quantized (VQ) VAE Model to encode and decode images to and from latent representations.
         unet ([`UNet2DModel`]): U-Net architecture to denoise the encoded image.
         scheduler ([`SchedulerMixin`]):
-            A scheduler to be used in combination with `unet` to denoise the encoded image latents. Can be one of
-            [`DDIMScheduler`], [`LMSDiscreteScheduler`],[`PNDMScheduler`].
+            A scheduler to be used in combination with `unet` to denoise the encoded image latens. Can be one of
+            [`DDIMScheduler`], [`LMSDiscreteScheduler`], [`EulerDiscreteScheduler`],
+            [`EulerAncestralDiscreteScheduler`], [`DPMSolverMultistepScheduler`], or [`PNDMScheduler`].
     """
 
     def __init__(
         self,
         vqvae: VQModel,
         unet: UNet2DModel,
-        scheduler: Union[DDIMScheduler, PNDMScheduler, LMSDiscreteScheduler, ],
+        scheduler: Union[
+            DDIMScheduler,
+            PNDMScheduler,
+            LMSDiscreteScheduler,
+            EulerDiscreteScheduler,
+            EulerAncestralDiscreteScheduler,
+            DPMSolverMultistepScheduler,
+        ],
     ):
         super().__init__()
         self.register_modules(vqvae=vqvae, unet=unet, scheduler=scheduler)
 
     @paddle.no_grad()
     def __call__(
         self,
-        init_image: Union[paddle.Tensor, PIL.Image.Image],
+        image: Union[paddle.Tensor, PIL.Image.Image],
         batch_size: Optional[int] = 1,
         num_inference_steps: Optional[int] = 100,
         eta: Optional[float] = 0.0,
-        seed: Optional[int] = None,
+        generator: Optional[paddle.Generator] = None,
         output_type: Optional[str] = "pil",
         return_dict: bool = True,
         **kwargs,
     ) -> Union[Tuple, ImagePipelineOutput]:
         r"""
         Args:
-            init_image (`paddle.Tensor` or `PIL.Image.Image`):
+            image (`paddle.Tensor` or `PIL.Image.Image`):
                 `Image`, or tensor representing an image batch, that will be used as the starting point for the
                 process.
             batch_size (`int`, *optional*, defaults to 1):
                 Number of images to generate.
             num_inference_steps (`int`, *optional*, defaults to 100):
                 The number of denoising steps. More denoising steps usually lead to a higher quality image at the
                 expense of slower inference.
             eta (`float`, *optional*, defaults to 0.0):
                 Corresponds to parameter eta (η) in the DDIM paper: https://arxiv.org/abs/2010.02502. Only applies to
                 [`schedulers.DDIMScheduler`], will be ignored for others.
-            seed (`int`, *optional*):
-                The seed used by paddle.randn().
+            generator (`paddle.Generator`, *optional*):
+                A [paddle generator] to make generation deterministic.
             output_type (`str`, *optional*, defaults to `"pil"`):
                 The output format of the generate image. Choose between
                 [PIL](https://pillow.readthedocs.io/en/stable/): `PIL.Image.Image` or `np.array`.
             return_dict (`bool`, *optional*):
                 Whether or not to return a [`~pipeline_utils.ImagePipelineOutput`] instead of a plain tuple.
 
         Returns:
             [`~pipeline_utils.ImagePipelineOutput`] or `tuple`: [`~pipelines.utils.ImagePipelineOutput`] if
             `return_dict` is True, otherwise a `tuple. When returning a tuple, the first element is a list with the
             generated images.
         """
 
-        if isinstance(init_image, PIL.Image.Image):
+        if isinstance(image, PIL.Image.Image):
             batch_size = 1
-        elif isinstance(init_image, paddle.Tensor):
-            batch_size = init_image.shape[0]
+        elif isinstance(image, paddle.Tensor):
+            batch_size = image.shape[0]
         else:
-            raise ValueError(
-                f"`init_image` has to be of type `PIL.Image.Image` or `paddle.Tensor` but is {type(init_image)}"
-            )
+            raise ValueError(f"`image` has to be of type `PIL.Image.Image` or `paddle.Tensor` but is {type(image)}")
 
-        if isinstance(init_image, PIL.Image.Image):
-            init_image = preprocess(init_image)
+        if isinstance(image, PIL.Image.Image):
+            image = preprocess(image)
 
-        height, width = init_image.shape[-2:]
+        height, width = image.shape[-2:]
 
         # in_channels should be 6: 3 for latents, 3 for low resolution image
         latents_shape = (batch_size, self.unet.in_channels // 2, height, width)
-        latents_dtype = self.unet.dtype
+        latents_dtype = next(self.unet.named_parameters())[1].dtype
 
-        if seed is not None: paddle.seed(seed)
-        latents = paddle.randn(latents_shape, dtype=latents_dtype)
+        latents = paddle.randn(latents_shape, generator=generator, dtype=latents_dtype)
 
-        init_image = init_image.astype(latents_dtype)
+        image = image.cast(latents_dtype)
 
-        # set timesteps
         self.scheduler.set_timesteps(num_inference_steps)
-
-        # Some schedulers like PNDM have timesteps as arrays
-        # It's more optimized to move all timesteps to correct device beforehand
         timesteps_tensor = self.scheduler.timesteps
 
         # scale the initial noise by the standard deviation required by the scheduler
         latents = latents * self.scheduler.init_noise_sigma
 
         # prepare extra kwargs for the scheduler step, since not all schedulers have the same signature.
         # eta (η) is only used with the DDIMScheduler, it will be ignored for other schedulers.
         # eta corresponds to η in DDIM paper: https://arxiv.org/abs/2010.02502
         # and should be between [0, 1]
-        accepts_eta = "eta" in set(
-            inspect.signature(self.scheduler.step).parameters.keys())
+        accepts_eta = "eta" in set(inspect.signature(self.scheduler.step).parameters.keys())
         extra_kwargs = {}
         if accepts_eta:
             extra_kwargs["eta"] = eta
 
         for t in self.progress_bar(timesteps_tensor):
             # concat latents and low resolution image in the channel dimension.
-            latents_input = paddle.concat([latents, init_image], axis=1)
+            latents_input = paddle.concat([latents, image], axis=1)
             latents_input = self.scheduler.scale_model_input(latents_input, t)
             # predict the noise residual
             noise_pred = self.unet(latents_input, t).sample
             # compute the previous noisy sample x_t -> x_t-1
-            latents = self.scheduler.step(noise_pred, t, latents,
-                                          **extra_kwargs).prev_sample
+            latents = self.scheduler.step(noise_pred, t, latents, **extra_kwargs).prev_sample
 
         # decode the image latents with the VQVAE
         image = self.vqvae.decode(latents).sample
         image = paddle.clip(image, -1.0, 1.0)
         image = image / 2 + 0.5
-        image = image.transpose([0, 2, 3, 1]).numpy()
+        image = image.transpose([0, 2, 3, 1]).cast("float32").numpy()
 
         if output_type == "pil":
             image = self.numpy_to_pil(image)
 
         if not return_dict:
-            return (image, )
+            return (image,)
 
         return ImagePipelineOutput(images=image)
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/pipelines/latent_diffusion_uncond/__init__.py` & `ppdiffusers-0.9.0/ppdiffusers/pipelines/latent_diffusion_uncond/__init__.py`

 * *Files identical despite different names*

### Comparing `ppdiffusers-0.6.3/ppdiffusers/pipelines/latent_diffusion_uncond/pipeline_latent_diffusion_uncond.py` & `ppdiffusers-0.9.0/ppdiffusers/pipelines/latent_diffusion_uncond/pipeline_latent_diffusion_uncond.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,88 +22,89 @@
 from ...pipeline_utils import DiffusionPipeline, ImagePipelineOutput
 from ...schedulers import DDIMScheduler
 
 
 class LDMPipeline(DiffusionPipeline):
     r"""
     This model inherits from [`DiffusionPipeline`]. Check the superclass documentation for the generic methods the
-    library implements for all the pipelines (such as downloading or saving, running on a particular device, etc.)
+    library implements for all the pipelines (such as downloading or saving, running on a particular xxxx, etc.)
 
     Parameters:
         vqvae ([`VQModel`]):
             Vector-quantized (VQ) Model to encode and decode images to and from latent representations.
         unet ([`UNet2DModel`]): U-Net architecture to denoise the encoded image latents.
         scheduler ([`SchedulerMixin`]):
-            [`DDIMScheduler`] is to be used in combination with `unet` to denoise the encoded image latens.
+            [`DDIMScheduler`] is to be used in combination with `unet` to denoise the encoded image latents.
     """
 
-    def __init__(self, vqvae: VQModel, unet: UNet2DModel,
-                 scheduler: DDIMScheduler):
+    def __init__(self, vqvae: VQModel, unet: UNet2DModel, scheduler: DDIMScheduler):
         super().__init__()
         self.register_modules(vqvae=vqvae, unet=unet, scheduler=scheduler)
 
     @paddle.no_grad()
     def __call__(
         self,
         batch_size: int = 1,
-        seed: Optional[int] = None,
+        generator: Optional[paddle.Generator] = None,
         eta: float = 0.0,
         num_inference_steps: int = 50,
         output_type: Optional[str] = "pil",
         return_dict: bool = True,
         **kwargs,
     ) -> Union[Tuple, ImagePipelineOutput]:
         r"""
         Args:
             batch_size (`int`, *optional*, defaults to 1):
                 Number of images to generate.
-            seed (`int`, *optional*):
-                A random seed.
+            generator (`paddle.Generator`, *optional*):
+                A [paddle generator] to make generation deterministic.
             num_inference_steps (`int`, *optional*, defaults to 50):
                 The number of denoising steps. More denoising steps usually lead to a higher quality image at the
                 expense of slower inference.
             output_type (`str`, *optional*, defaults to `"pil"`):
                 The output format of the generate image. Choose between
                 [PIL](https://pillow.readthedocs.io/en/stable/): `PIL.Image.Image` or `np.array`.
             return_dict (`bool`, *optional*, defaults to `True`):
                 Whether or not to return a [`~pipeline_utils.ImagePipelineOutput`] instead of a plain tuple.
 
         Returns:
             [`~pipeline_utils.ImagePipelineOutput`] or `tuple`: [`~pipelines.utils.ImagePipelineOutput`] if
             `return_dict` is True, otherwise a `tuple. When returning a tuple, the first element is a list with the
             generated images.
         """
-        if seed is not None:
-            paddle.seed(seed)
 
-        latents = paddle.randn((batch_size, self.unet.in_channels,
-                                self.unet.sample_size, self.unet.sample_size), )
+        latents = paddle.randn(
+            (batch_size, self.unet.in_channels, self.unet.sample_size, self.unet.sample_size),
+            generator=generator,
+        )
+
+        # scale the initial noise by the standard deviation required by the scheduler
+        latents = latents * self.scheduler.init_noise_sigma
 
         self.scheduler.set_timesteps(num_inference_steps)
 
         # prepare extra kwargs for the scheduler step, since not all schedulers have the same signature
-        accepts_eta = "eta" in set(
-            inspect.signature(self.scheduler.step).parameters.keys())
+        accepts_eta = "eta" in set(inspect.signature(self.scheduler.step).parameters.keys())
 
         extra_kwargs = {}
         if accepts_eta:
             extra_kwargs["eta"] = eta
 
         for t in self.progress_bar(self.scheduler.timesteps):
+            latent_model_input = self.scheduler.scale_model_input(latents, t)
             # predict the noise residual
-            noise_prediction = self.unet(latents, t).sample
+            noise_prediction = self.unet(latent_model_input, t).sample
             # compute the previous noisy sample x_t -> x_t-1
-            latents = self.scheduler.step(noise_prediction, t, latents,
-                                          **extra_kwargs).prev_sample
+            latents = self.scheduler.step(noise_prediction, t, latents, **extra_kwargs).prev_sample
 
         # decode the image latents with the VAE
         image = self.vqvae.decode(latents).sample
 
         image = (image / 2 + 0.5).clip(0, 1)
-        image = image.transpose([0, 2, 3, 1]).numpy()
+        image = image.transpose([0, 2, 3, 1]).cast("float32").numpy()
         if output_type == "pil":
             image = self.numpy_to_pil(image)
 
         if not return_dict:
-            return (image, )
+            return (image,)
 
         return ImagePipelineOutput(images=image)
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/pipelines/pndm/__init__.py` & `ppdiffusers-0.9.0/ppdiffusers/pipelines/score_sde_ve/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # flake8: noqa
-from .pipeline_pndm import PNDMPipeline
+from .pipeline_score_sde_ve import ScoreSdeVePipeline
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/pipelines/score_sde_ve/__init__.py` & `ppdiffusers-0.9.0/ppdiffusers/pipelines/dance_diffusion/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # flake8: noqa
-from .pipeline_score_sde_ve import ScoreSdeVePipeline
+from .pipeline_dance_diffusion import DanceDiffusionPipeline
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/pipelines/score_sde_ve/pipeline_score_sde_ve.py` & `ppdiffusers-0.9.0/ppdiffusers/pipelines/dance_diffusion/pipeline_dance_diffusion.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,91 +13,103 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Optional, Tuple, Union
 
 import paddle
 
-from ...models import UNet2DModel
-from ...pipeline_utils import DiffusionPipeline, ImagePipelineOutput
-from ...schedulers import ScoreSdeVeScheduler
+from ...pipeline_utils import AudioPipelineOutput, DiffusionPipeline
+from ...utils import logging
 
+logger = logging.get_logger(__name__)  # pylint: disable=invalid-name
 
-class ScoreSdeVePipeline(DiffusionPipeline):
+
+class DanceDiffusionPipeline(DiffusionPipeline):
     r"""
-    Parameters:
     This model inherits from [`DiffusionPipeline`]. Check the superclass documentation for the generic methods the
-    library implements for all the pipelines (such as downloading or saving, running on a particular device, etc.)
-        unet ([`UNet2DModel`]): U-Net architecture to denoise the encoded image. scheduler ([`SchedulerMixin`]):
-            The [`ScoreSdeVeScheduler`] scheduler to be used in combination with `unet` to denoise the encoded image.
+    library implements for all the pipelines (such as downloading or saving, running on a particular xxxx, etc.)
+
+    Parameters:
+        unet ([`UNet1DModel`]): U-Net architecture to denoise the encoded image.
+        scheduler ([`SchedulerMixin`]):
+            A scheduler to be used in combination with `unet` to denoise the encoded image. Can be one of
+            [`IPNDMScheduler`].
     """
-    unet: UNet2DModel
-    scheduler: ScoreSdeVeScheduler
 
-    def __init__(self, unet: UNet2DModel, scheduler: DiffusionPipeline):
+    def __init__(self, unet, scheduler):
         super().__init__()
         self.register_modules(unet=unet, scheduler=scheduler)
 
     @paddle.no_grad()
     def __call__(
         self,
         batch_size: int = 1,
-        num_inference_steps: int = 2000,
-        seed: Optional[int] = None,
-        output_type: Optional[str] = "pil",
+        num_inference_steps: int = 100,
+        generator: Optional[paddle.Generator] = None,
+        audio_length_in_s: Optional[float] = None,
         return_dict: bool = True,
-        **kwargs,
-    ) -> Union[ImagePipelineOutput, Tuple]:
+    ) -> Union[AudioPipelineOutput, Tuple]:
         r"""
         Args:
             batch_size (`int`, *optional*, defaults to 1):
-                The number of images to generate.
-            seed (`int`, *optional*):
-                A random seed.
-            output_type (`str`, *optional*, defaults to `"pil"`):
-                The output format of the generate image. Choose between
-                [PIL](https://pillow.readthedocs.io/en/stable/): `PIL.Image.Image` or `np.array`.
+                The number of audio samples to generate.
+            num_inference_steps (`int`, *optional*, defaults to 50):
+                The number of denoising steps. More denoising steps usually lead to a higher quality audio sample at
+                the expense of slower inference.
+            generator (`paddle.Generator`, *optional*):
+                A [paddle generator] to make generation deterministic.
+            audio_length_in_s (`float`, *optional*, defaults to `self.unet.config.sample_size/self.unet.config.sample_rate`):
+                The length of the generated audio sample in seconds. Note that the output of the pipeline, *i.e.*
+                `sample_size`, will be `audio_length_in_s` * `self.unet.sample_rate`.
             return_dict (`bool`, *optional*, defaults to `True`):
-                Whether or not to return a [`~pipeline_utils.ImagePipelineOutput`] instead of a plain tuple.
+                Whether or not to return a [`~pipeline_utils.AudioPipelineOutput`] instead of a plain tuple.
 
         Returns:
-            [`~pipeline_utils.ImagePipelineOutput`] or `tuple`: [`~pipelines.utils.ImagePipelineOutput`] if
+            [`~pipeline_utils.AudioPipelineOutput`] or `tuple`: [`~pipelines.utils.AudioPipelineOutput`] if
             `return_dict` is True, otherwise a `tuple. When returning a tuple, the first element is a list with the
             generated images.
         """
-        if seed is not None:
-            paddle.seed(seed)
 
-        img_size = self.unet.config.sample_size
-        shape = (batch_size, 3, img_size, img_size)
+        if audio_length_in_s is None:
+            audio_length_in_s = self.unet.config.sample_size / self.unet.config.sample_rate
 
-        model = self.unet
+        sample_size = audio_length_in_s * self.unet.sample_rate
 
-        sample = paddle.randn(shape) * self.scheduler.init_noise_sigma
+        down_scale_factor = 2 ** len(self.unet.up_blocks)
+        if sample_size < 3 * down_scale_factor:
+            raise ValueError(
+                f"{audio_length_in_s} is too small. Make sure it's bigger or equal to"
+                f" {3 * down_scale_factor / self.unet.sample_rate}."
+            )
+
+        original_sample_size = int(sample_size)
+        if sample_size % down_scale_factor != 0:
+            sample_size = ((audio_length_in_s * self.unet.sample_rate) // down_scale_factor + 1) * down_scale_factor
+            logger.info(
+                f"{audio_length_in_s} is increased to {sample_size / self.unet.sample_rate} so that it can be handled"
+                f" by the model. It will be cut to {original_sample_size / self.unet.sample_rate} after the denoising"
+                " process."
+            )
+        sample_size = int(sample_size)
 
+        dtype = self.unet.dtype
+        audio = paddle.randn((batch_size, self.unet.in_channels, sample_size), generator=generator, dtype=dtype)
+
+        # set step values
         self.scheduler.set_timesteps(num_inference_steps)
-        self.scheduler.set_sigmas(num_inference_steps)
+        self.scheduler.timesteps = self.scheduler.timesteps.cast(dtype)
+
+        for t in self.progress_bar(self.scheduler.timesteps):
+            # 1. predict noise model_output
+            model_output = self.unet(audio, t).sample
+
+            # 2. compute previous image: x_t -> t_t-1
+            audio = self.scheduler.step(model_output, t, audio).prev_sample
 
-        for i, t in enumerate(self.progress_bar(self.scheduler.timesteps)):
-            sigma_t = self.scheduler.sigmas[i] * paddle.ones(shape[0])
+        audio = audio.clip(-1, 1).cast("float32").cpu().numpy()
 
-            # correction step
-            for _ in range(self.scheduler.config.correct_steps):
-                model_output = self.unet(sample, sigma_t).sample
-                sample = self.scheduler.step_correct(model_output,
-                                                     sample).prev_sample
-
-            # prediction step
-            model_output = model(sample, sigma_t).sample
-            output = self.scheduler.step_pred(model_output, t, sample)
-
-            sample, sample_mean = output.prev_sample, output.prev_sample_mean
-
-        sample = sample_mean.clip(0, 1)
-        sample = sample.transpose([0, 2, 3, 1]).numpy()
-        if output_type == "pil":
-            sample = self.numpy_to_pil(sample)
+        audio = audio[:, :, :original_sample_size]
 
         if not return_dict:
-            return (sample, )
+            return (audio,)
 
-        return ImagePipelineOutput(images=sample)
+        return AudioPipelineOutput(audios=audio)
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/pipelines/stable_diffusion/__init__.py` & `ppdiffusers-0.9.0/ppdiffusers/pipelines/stable_diffusion/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,24 +8,28 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+# flake8: noqa
 
 from dataclasses import dataclass
 from typing import List, Optional, Union
 
 import numpy as np
-
 import PIL
-from PIL import Image
 
-from ...utils import BaseOutput, is_onnx_available, is_paddle_available, is_paddlenlp_available, is_fastdeploy_available
+from ...utils import (
+    BaseOutput,
+    is_fastdeploy_available,
+    is_paddle_available,
+    is_paddlenlp_available,
+)
 
 
 @dataclass
 class StableDiffusionPipelineOutput(BaseOutput):
     """
     Output class for Stable Diffusion pipelines.
 
@@ -39,23 +43,43 @@
     """
 
     images: Union[List[PIL.Image.Image], np.ndarray]
     nsfw_content_detected: Optional[List[bool]]
 
 
 if is_paddlenlp_available() and is_paddle_available():
-    from .pipeline_stable_diffusion_all_in_one import StableDiffusionPipelineAllinOne
+    from .pipeline_cycle_diffusion import CycleDiffusionPipeline
     from .pipeline_stable_diffusion import StableDiffusionPipeline
+    from .pipeline_stable_diffusion_all_in_one import StableDiffusionPipelineAllinOne
     from .pipeline_stable_diffusion_img2img import StableDiffusionImg2ImgPipeline
     from .pipeline_stable_diffusion_inpaint import StableDiffusionInpaintPipeline
-    from .pipeline_stable_diffusion_inpaint_legacy import StableDiffusionInpaintPipelineLegacy
+    from .pipeline_stable_diffusion_inpaint_legacy import (
+        StableDiffusionInpaintPipelineLegacy,
+    )
+    from .pipeline_stable_diffusion_mega import StableDiffusionMegaPipeline
+    from .pipeline_stable_diffusion_upscale import StableDiffusionUpscalePipeline
     from .safety_checker import StableDiffusionSafetyChecker
 
-if is_paddlenlp_available() and is_onnx_available():
-    from .pipeline_onnx_stable_diffusion import OnnxStableDiffusionPipeline
-    from .pipeline_onnx_stable_diffusion_img2img import OnnxStableDiffusionImg2ImgPipeline
-    from .pipeline_onnx_stable_diffusion_inpaint import OnnxStableDiffusionInpaintPipeline
+if is_paddlenlp_available() and is_paddle_available():
+    from .pipeline_stable_diffusion_image_variation import (
+        StableDiffusionImageVariationPipeline,
+    )
+else:
+    from ...utils.dummy_paddle_and_paddlenlp_objects import (
+        StableDiffusionImageVariationPipeline,
+    )
+
 
 if is_paddlenlp_available() and is_fastdeploy_available():
     from .pipeline_fastdeploy_stable_diffusion import FastDeployStableDiffusionPipeline
-    from .pipeline_fastdeploy_stable_diffusion_img2img import FastDeployStableDiffusionImg2ImgPipeline
-    from .pipeline_fastdeploy_stable_diffusion_inpaint import FastDeployStableDiffusionInpaintPipeline
+    from .pipeline_fastdeploy_stable_diffusion_img2img import (
+        FastDeployStableDiffusionImg2ImgPipeline,
+    )
+    from .pipeline_fastdeploy_stable_diffusion_inpaint import (
+        FastDeployStableDiffusionInpaintPipeline,
+    )
+    from .pipeline_fastdeploy_stable_diffusion_inpaint_legacy import (
+        FastDeployStableDiffusionInpaintPipelineLegacy,
+    )
+    from .pipeline_fastdeploy_stable_diffusion_mega import (
+        FastDeployStableDiffusionMegaPipeline,
+    )
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/pipelines/stable_diffusion/pipeline_fastdeploy_stable_diffusion_img2img.py` & `ppdiffusers-0.9.0/ppdiffusers/pipelines/stable_diffusion/pipeline_fastdeploy_stable_diffusion_img2img.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,157 +14,324 @@
 
 import inspect
 from typing import Callable, List, Optional, Union
 
 import numpy as np
 import paddle
 import PIL
-from paddlenlp.utils.tools import compare_version
-if compare_version(PIL.__version__, "9.1.0") >= 0:
-    Resampling = PIL.Image.Resampling
-else:
-    Resampling = PIL.Image
 
 from paddlenlp.transformers import CLIPFeatureExtractor, CLIPTokenizer
 
-from ...configuration_utils import FrozenDict
 from ...fastdeploy_utils import FastDeployRuntimeModel
 from ...pipeline_utils import DiffusionPipeline
-from ...schedulers import DDIMScheduler, LMSDiscreteScheduler, PNDMScheduler
-from ...utils import deprecate, logging
+from ...schedulers import (
+    DDIMScheduler,
+    DPMSolverMultistepScheduler,
+    EulerAncestralDiscreteScheduler,
+    EulerDiscreteScheduler,
+    LMSDiscreteScheduler,
+    PNDMScheduler,
+)
+from ...utils import PIL_INTERPOLATION, logging
 from . import StableDiffusionPipelineOutput
 
 logger = logging.get_logger(__name__)  # pylint: disable=invalid-name
 
 
 def preprocess(image):
     w, h = image.size
     w, h = map(lambda x: x - x % 32, (w, h))  # resize to integer multiple of 32
-    image = image.resize((w, h), resample=Resampling.LANCZOS)
+    image = image.resize((w, h), resample=PIL_INTERPOLATION["lanczos"])
     image = np.array(image).astype(np.float32) / 255.0
     image = image[None].transpose(0, 3, 1, 2)
     return 2.0 * image - 1.0
 
 
 class FastDeployStableDiffusionImg2ImgPipeline(DiffusionPipeline):
     r"""
-    Pipeline for text-guided image to image generation using Stable Diffusion.
+    Pipeline for text-guided image-to-image generation using Stable Diffusion.
+
     This model inherits from [`DiffusionPipeline`]. Check the superclass documentation for the generic methods the
-    library implements for all the pipelines (such as downloading or saving, running on a particular device, etc.)
+    library implements for all the pipelines (such as downloading or saving etc.)
+
     Args:
-        vae ([`AutoencoderKL`]):
-            Variational Auto-Encoder (VAE) Model to encode and decode images to and from latent representations.
-        text_encoder ([`CLIPTextModel`]):
+        vae_encoder ([`FastDeployRuntimeModel`]):
+            Variational Auto-Encoder (VAE) Model to encode images to latent representations.
+        vae_decoder ([`FastDeployRuntimeModel`]):
+            Variational Auto-Encoder (VAE) Model to decode images from latent representations.
+        text_encoder ([`FastDeployRuntimeModel`]):
             Frozen text-encoder. Stable Diffusion uses the text portion of
             [CLIP](https://huggingface.co/docs/transformers/model_doc/clip#transformers.CLIPTextModel), specifically
             the [clip-vit-large-patch14](https://huggingface.co/openai/clip-vit-large-patch14) variant.
         tokenizer (`CLIPTokenizer`):
             Tokenizer of class
             [CLIPTokenizer](https://huggingface.co/docs/transformers/v4.21.0/en/model_doc/clip#transformers.CLIPTokenizer).
-        unet ([`UNet2DConditionModel`]): Conditional U-Net architecture to denoise the encoded image latents.
+        unet ([`FastDeployRuntimeModel`]): Conditional U-Net architecture to denoise the encoded image latents.
         scheduler ([`SchedulerMixin`]):
-            A scheduler to be used in combination with `unet` to denoise the encoded image latens. Can be one of
-            [`DDIMScheduler`], [`LMSDiscreteScheduler`], or [`PNDMScheduler`].
-        safety_checker ([`StableDiffusionSafetyChecker`]):
+            A scheduler to be used in combination with `unet` to denoise the encoded image latents. Can be one of
+            [`DDIMScheduler`], [`LMSDiscreteScheduler`], [`PNDMScheduler`], [`EulerDiscreteScheduler`], [`EulerAncestralDiscreteScheduler`]
+            or [`DPMSolverMultistepScheduler`].
+        safety_checker ([`FastDeployRuntimeModel`]):
             Classification module that estimates whether generated images could be considered offensive or harmful.
             Please, refer to the [model card](https://huggingface.co/runwayml/stable-diffusion-v1-5) for details.
         feature_extractor ([`CLIPFeatureExtractor`]):
             Model that extracts features from generated images to be used as inputs for the `safety_checker`.
     """
-    vae_encoder: FastDeployRuntimeModel
-    vae_decoder: FastDeployRuntimeModel
-    text_encoder: FastDeployRuntimeModel
-    tokenizer: CLIPTokenizer
-    unet: FastDeployRuntimeModel
-    scheduler: Union[DDIMScheduler, PNDMScheduler, LMSDiscreteScheduler]
-    safety_checker: FastDeployRuntimeModel
-    feature_extractor: CLIPFeatureExtractor
+    _optional_components = ["safety_checker", "feature_extractor"]
 
     def __init__(
         self,
         vae_encoder: FastDeployRuntimeModel,
         vae_decoder: FastDeployRuntimeModel,
         text_encoder: FastDeployRuntimeModel,
         tokenizer: CLIPTokenizer,
         unet: FastDeployRuntimeModel,
-        scheduler: Union[DDIMScheduler, PNDMScheduler, LMSDiscreteScheduler],
+        scheduler: Union[
+            DDIMScheduler,
+            PNDMScheduler,
+            LMSDiscreteScheduler,
+            EulerDiscreteScheduler,
+            EulerAncestralDiscreteScheduler,
+            DPMSolverMultistepScheduler,
+        ],
         safety_checker: FastDeployRuntimeModel,
         feature_extractor: CLIPFeatureExtractor,
+        requires_safety_checker: bool = True,
     ):
         super().__init__()
-
-        if hasattr(scheduler.config,
-                   "steps_offset") and scheduler.config.steps_offset != 1:
-            deprecation_message = (
-                f"The configuration file of this scheduler: {scheduler} is outdated. `steps_offset`"
-                f" should be set to 1 instead of {scheduler.config.steps_offset}. Please make sure "
-                "to update the config accordingly as leaving `steps_offset` might led to incorrect results"
-                " in future versions. If you have downloaded this checkpoint from the Hugging Face Hub,"
-                " it would be very nice if you could open a Pull request for the `scheduler/scheduler_config.json`"
-                " file")
-            deprecate("steps_offset!=1",
-                      "1.0.0",
-                      deprecation_message,
-                      standard_warn=False)
-            new_config = dict(scheduler.config)
-            new_config["steps_offset"] = 1
-            scheduler._internal_dict = FrozenDict(new_config)
-
-        if safety_checker is None:
+        if safety_checker is None and requires_safety_checker:
             logger.warning(
                 f"You have disabled the safety checker for {self.__class__} by passing `safety_checker=None`. Ensure"
                 " that you abide to the conditions of the Stable Diffusion license and do not expose unfiltered"
                 " results in services or applications open to the public. PaddleNLP team, diffusers team and Hugging Face"
                 " strongly recommend to keep the safety filter enabled in all public facing circumstances, disabling"
                 " it only for use-cases that involve analyzing network behavior or auditing its results. For more"
                 " information, please have a look at https://github.com/huggingface/diffusers/pull/254 ."
             )
+        if safety_checker is not None and feature_extractor is None:
+            raise ValueError(
+                "Make sure to define a feature extractor when loading {self.__class__} if you want to use the safety"
+                " checker. If you do not want to use the safety checker, you can pass `'safety_checker=None'` instead."
+            )
 
         self.register_modules(
             vae_encoder=vae_encoder,
             vae_decoder=vae_decoder,
             text_encoder=text_encoder,
             tokenizer=tokenizer,
             unet=unet,
             scheduler=scheduler,
             safety_checker=safety_checker,
             feature_extractor=feature_extractor,
         )
+        self.register_to_config(requires_safety_checker=requires_safety_checker)
+
+    def _encode_prompt(self, prompt, num_images_per_prompt, do_classifier_free_guidance, negative_prompt):
+        r"""
+        Encodes the prompt into text encoder hidden states.
+
+        Args:
+            prompt (`str` or `list(int)`):
+                prompt to be encoded
+            num_images_per_prompt (`int`):
+                number of images that should be generated per prompt
+            do_classifier_free_guidance (`bool`):
+                whether to use classifier free guidance or not
+            negative_prompt (`str` or `List[str]`):
+                The prompt or prompts not to guide the image generation. Ignored when not using guidance (i.e., ignored
+                if `guidance_scale` is less than `1`).
+        """
+        batch_size = len(prompt) if isinstance(prompt, list) else 1
+
+        # get prompt text embeddings
+        text_inputs = self.tokenizer(
+            prompt,
+            padding="max_length",
+            max_length=self.tokenizer.model_max_length,
+            truncation=True,
+            return_tensors="np",
+        )
+        text_input_ids = text_inputs.input_ids
+        untruncated_ids = self.tokenizer(prompt, padding="max_length", return_tensors="np").input_ids
+
+        if not np.array_equal(text_input_ids, untruncated_ids):
+            removed_text = self.tokenizer.batch_decode(untruncated_ids[:, self.tokenizer.model_max_length - 1 : -1])
+            logger.warning(
+                "The following part of your input was truncated because CLIP can only handle sequences up to"
+                f" {self.tokenizer.model_max_length} tokens: {removed_text}"
+            )
+
+        text_embeddings = self.text_encoder(input_ids=text_input_ids.astype(np.int64))[0]
+        text_embeddings = np.repeat(text_embeddings, num_images_per_prompt, axis=0)
+
+        # get unconditional embeddings for classifier free guidance
+        if do_classifier_free_guidance:
+            uncond_tokens: List[str]
+            if negative_prompt is None:
+                uncond_tokens = [""] * batch_size
+            elif type(prompt) is not type(negative_prompt):
+                raise TypeError(
+                    f"`negative_prompt` should be the same type to `prompt`, but got {type(negative_prompt)} !="
+                    f" {type(prompt)}."
+                )
+            elif isinstance(negative_prompt, str):
+                uncond_tokens = [negative_prompt] * batch_size
+            elif batch_size != len(negative_prompt):
+                raise ValueError(
+                    f"`negative_prompt`: {negative_prompt} has batch size {len(negative_prompt)}, but `prompt`:"
+                    f" {prompt} has batch size {batch_size}. Please make sure that passed `negative_prompt` matches"
+                    " the batch size of `prompt`."
+                )
+            else:
+                uncond_tokens = negative_prompt
+
+            max_length = text_input_ids.shape[-1]
+            uncond_input = self.tokenizer(
+                uncond_tokens,
+                padding="max_length",
+                max_length=max_length,
+                truncation=True,
+                return_tensors="np",
+            )
+            uncond_embeddings = self.text_encoder(input_ids=uncond_input.input_ids.astype(np.int64))[0]
+            uncond_embeddings = np.repeat(uncond_embeddings, num_images_per_prompt, axis=0)
+
+            # For classifier free guidance, we need to do two forward passes.
+            # Here we concatenate the unconditional and text embeddings into a single batch
+            # to avoid doing two forward passes
+            text_embeddings = np.concatenate([uncond_embeddings, text_embeddings])
+
+        return text_embeddings
+
+    def run_safety_checker(self, image, dtype):
+        if self.safety_checker is not None:
+            safety_checker_input = self.feature_extractor(
+                self.numpy_to_pil(image), return_tensors="np"
+            ).pixel_values.astype(dtype)
+            # There will throw an error if use safety_checker batchsize>1
+            images, has_nsfw_concept = [], []
+            for i in range(image.shape[0]):
+                image_i, has_nsfw_concept_i = self.safety_checker(
+                    clip_input=safety_checker_input[i : i + 1], images=image[i : i + 1]
+                )
+                images.append(image_i)
+                has_nsfw_concept.append(has_nsfw_concept_i[0])
+            image = np.concatenate(images)
+        else:
+            has_nsfw_concept = None
+        return image, has_nsfw_concept
+
+    def decode_latents(self, latents):
+        latents = 1 / 0.18215 * latents
+        image = np.concatenate(
+            [self.vae_decoder(latent_sample=latents[i : i + 1])[0] for i in range(latents.shape[0])]
+        )
+        image = np.clip(image / 2 + 0.5, 0, 1)
+        image = image.transpose([0, 2, 3, 1])
+        return image
+
+    def prepare_extra_step_kwargs(self, eta):
+        # prepare extra kwargs for the scheduler step, since not all schedulers have the same signature
+        # eta (η) is only used with the DDIMScheduler, it will be ignored for other schedulers.
+        # eta corresponds to η in DDIM paper: https://arxiv.org/abs/2010.02502
+        # and should be between [0, 1]
+
+        accepts_eta = "eta" in set(inspect.signature(self.scheduler.step).parameters.keys())
+        extra_step_kwargs = {}
+        if accepts_eta:
+            extra_step_kwargs["eta"] = eta
+
+        return extra_step_kwargs
+
+    def check_inputs(self, prompt, strength, callback_steps):
+        if not isinstance(prompt, str) and not isinstance(prompt, list):
+            raise ValueError(f"`prompt` has to be of type `str` or `list` but is {type(prompt)}")
+
+        if strength < 0 or strength > 1:
+            raise ValueError(f"The value of strength should in [1.0, 1.0] but is {strength}")
+
+        if (callback_steps is None) or (
+            callback_steps is not None and (not isinstance(callback_steps, int) or callback_steps <= 0)
+        ):
+            raise ValueError(
+                f"`callback_steps` has to be a positive integer but is {callback_steps} of type"
+                f" {type(callback_steps)}."
+            )
+
+    def get_timesteps(self, num_inference_steps, strength):
+        # get the original timestep using init_timestep
+        offset = self.scheduler.config.get("steps_offset", 0)
+        init_timestep = int(num_inference_steps * strength) + offset
+        init_timestep = min(init_timestep, num_inference_steps)
+
+        t_start = max(num_inference_steps - init_timestep + offset, 0)
+        timesteps = self.scheduler.timesteps.numpy()
+        timesteps = timesteps[t_start:]
+        return timesteps, num_inference_steps - t_start
+
+    def prepare_latents(self, image, timestep, batch_size, num_images_per_prompt, dtype, generator=None, noise=None):
+        if generator is None:
+            generator = np.random
+
+        image = image.astype(dtype)
+        init_latents = self.vae_encoder(sample=image)[0]
+        init_latents = 0.18215 * init_latents
+
+        if batch_size > init_latents.shape[0] and batch_size % init_latents.shape[0] != 0:
+            raise ValueError(
+                f"Cannot duplicate `image` of batch size {init_latents.shape[0]} to {batch_size} text prompts."
+            )
+        else:
+            init_latents = np.concatenate([init_latents] * num_images_per_prompt, axis=0)
+
+        # add noise to latents using the timesteps
+        if noise is None:
+            noise = paddle.to_tensor(generator.randn(*init_latents.shape).astype(dtype))
+        elif list(noise.shape) != list(init_latents.shape):
+            raise ValueError(f"Unexpected noise shape, got {noise.shape}, expected {init_latents.shape}")
+        elif isinstance(noise, np.ndarray):
+            noise = paddle.to_tensor(noise, dtype=dtype)
+
+        # get latents
+        init_latents = self.scheduler.add_noise(paddle.to_tensor(init_latents), noise, paddle.to_tensor(timestep))
+        latents = init_latents.numpy()
+
+        return latents
 
     def __call__(
         self,
         prompt: Union[str, List[str]],
-        init_image: Union[np.ndarray, PIL.Image.Image],
+        image: Union[np.ndarray, PIL.Image.Image],
         strength: float = 0.8,
         num_inference_steps: Optional[int] = 50,
         guidance_scale: Optional[float] = 7.5,
         negative_prompt: Optional[Union[str, List[str]]] = None,
         num_images_per_prompt: Optional[int] = 1,
         eta: Optional[float] = 0.0,
         generator: Optional[np.random.RandomState] = None,
+        noise: Optional[np.ndarray] = None,
         output_type: Optional[str] = "pil",
         return_dict: bool = True,
         callback: Optional[Callable[[int, int, np.ndarray], None]] = None,
         callback_steps: Optional[int] = 1,
-        **kwargs,
     ):
         r"""
         Function invoked when calling the pipeline for generation.
         Args:
             prompt (`str` or `List[str]`):
                 The prompt or prompts to guide the image generation.
-            init_image (`np.ndarray` or `PIL.Image.Image`):
+            image (`np.ndarray` or `PIL.Image.Image`):
                 `Image`, or tensor representing an image batch, that will be used as the starting point for the
                 process.
             strength (`float`, *optional*, defaults to 0.8):
-                Conceptually, indicates how much to transform the reference `init_image`. Must be between 0 and 1.
-                `init_image` will be used as a starting point, adding more noise to it the larger the `strength`. The
+                Conceptually, indicates how much to transform the reference `image`. Must be between 0 and 1.
+                `image` will be used as a starting point, adding more noise to it the larger the `strength`. The
                 number of denoising steps depends on the amount of noise initially added. When `strength` is 1, added
                 noise will be maximum and the denoising process will run for the full number of iterations specified in
-                `num_inference_steps`. A value of 1, therefore, essentially ignores `init_image`.
+                `num_inference_steps`. A value of 1, therefore, essentially ignores `image`.
             num_inference_steps (`int`, *optional*, defaults to 50):
                 The number of denoising steps. More denoising steps usually lead to a higher quality image at the
                 expense of slower inference. This parameter will be modulated by `strength`.
             guidance_scale (`float`, *optional*, defaults to 7.5):
                 Guidance scale as defined in [Classifier-Free Diffusion Guidance](https://arxiv.org/abs/2207.12598).
                 `guidance_scale` is defined as `w` of equation 2. of [Imagen
                 Paper](https://arxiv.org/pdf/2205.11487.pdf). Guidance scale is enabled by setting `guidance_scale >
@@ -176,14 +343,18 @@
             num_images_per_prompt (`int`, *optional*, defaults to 1):
                 The number of images to generate per prompt.
             eta (`float`, *optional*, defaults to 0.0):
                 Corresponds to parameter eta (η) in the DDIM paper: https://arxiv.org/abs/2010.02502. Only applies to
                 [`schedulers.DDIMScheduler`], will be ignored for others.
             generator (`np.random.RandomState`, *optional*):
                 A np.random.RandomState to make generation deterministic.
+            noise (`np.ndarray`, *optional*):
+                Pre-generated noise tensor, sampled from a Gaussian distribution, to be used as inputs for image
+                generation. If not provided, a noise tensor will ge generated by sampling using the supplied random
+                `generator`.
             output_type (`str`, *optional*, defaults to `"pil"`):
                 The output format of the generate image. Choose between
                 [PIL](https://pillow.readthedocs.io/en/stable/): `PIL.Image.Image` or `np.array`.
             return_dict (`bool`, *optional*, defaults to `True`):
                 Whether or not to return a [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] instead of a
                 plain tuple.
             callback (`Callable`, *optional*):
@@ -195,237 +366,87 @@
         Returns:
             [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] or `tuple`:
             [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] if `return_dict` is True, otherwise a `tuple.
             When returning a tuple, the first element is a list with the generated images, and the second element is a
             list of `bool`s denoting whether the corresponding generated image likely represents "not-safe-for-work"
             (nsfw) content, according to the `safety_checker`.
         """
-        if isinstance(prompt, str):
-            batch_size = 1
-        elif isinstance(prompt, list):
-            batch_size = len(prompt)
-        else:
-            raise ValueError(
-                f"`prompt` has to be of type `str` or `list` but is {type(prompt)}"
-            )
-
-        if strength < 0 or strength > 1:
-            raise ValueError(
-                f"The value of strength should in [0.0, 1.0] but is {strength}")
-
-        if (callback_steps is None) or (callback_steps is not None and
-                                        (not isinstance(callback_steps, int)
-                                         or callback_steps <= 0)):
-            raise ValueError(
-                f"`callback_steps` has to be a positive integer but is {callback_steps} of type"
-                f" {type(callback_steps)}.")
-        if generator is None:
-            generator = np.random
-
-        # set timesteps
-        self.scheduler.set_timesteps(num_inference_steps)
-
-        if isinstance(init_image, PIL.Image.Image):
-            init_image = preprocess(init_image)
-
-        # get prompt text embeddings
-        text_inputs = self.tokenizer(
-            prompt,
-            padding="max_length",
-            max_length=self.tokenizer.model_max_length,
-            return_tensors="np",
-        )
-        text_input_ids = text_inputs.input_ids
-
-        if text_input_ids.shape[-1] > self.tokenizer.model_max_length:
-            removed_text = self.tokenizer.batch_decode(
-                text_input_ids[:, self.tokenizer.model_max_length:])
-            logger.warning(
-                "The following part of your input was truncated because CLIP can only handle sequences up to"
-                f" {self.tokenizer.model_max_length} tokens: {removed_text}")
-            text_input_ids = text_input_ids[:, :self.tokenizer.model_max_length]
-        text_embeddings = self.text_encoder(
-            input_ids=text_input_ids.astype(np.int64))[0]
-
-        # duplicate text embeddings for each generation per prompt
-        text_embeddings = np.repeat(text_embeddings,
-                                    num_images_per_prompt,
-                                    axis=0)
+        # 1. Check inputs
+        self.check_inputs(prompt, strength, callback_steps)
 
+        # 2. Define call parameters
+        batch_size = 1 if isinstance(prompt, str) else len(prompt)
         # here `guidance_scale` is defined analog to the guidance weight `w` of equation (2)
         # of the Imagen paper: https://arxiv.org/pdf/2205.11487.pdf . `guidance_scale = 1`
         # corresponds to doing no classifier free guidance.
         do_classifier_free_guidance = guidance_scale > 1.0
-        # get unconditional embeddings for classifier free guidance
-        if do_classifier_free_guidance:
-            uncond_tokens: List[str]
-            if negative_prompt is None:
-                uncond_tokens = [""]
-            elif type(prompt) is not type(negative_prompt):
-                raise TypeError(
-                    f"`negative_prompt` should be the same type to `prompt`, but got {type(negative_prompt)} !="
-                    f" {type(prompt)}.")
-            elif isinstance(negative_prompt, str):
-                uncond_tokens = [negative_prompt] * batch_size
-            elif batch_size != len(negative_prompt):
-                raise ValueError(
-                    "The length of `negative_prompt` should be equal to batch_size."
-                )
-            else:
-                uncond_tokens = negative_prompt
-
-            max_length = text_input_ids.shape[-1]
-            uncond_input = self.tokenizer(
-                uncond_tokens,
-                padding="max_length",
-                max_length=max_length,
-                truncation=True,
-                return_tensors="np",
-            )
-            uncond_input_ids = uncond_input.input_ids
-            uncond_embeddings = self.text_encoder(
-                input_ids=uncond_input_ids.astype(np.int64))[0]
-
-            # duplicate unconditional embeddings for each generation per prompt
-            uncond_embeddings = np.repeat(uncond_embeddings,
-                                          num_images_per_prompt,
-                                          axis=0)
-
-            # For classifier free guidance, we need to do two forward passes.
-            # Here we concatenate the unconditional and text embeddings into a single batch
-            # to avoid doing two forward passes
-            text_embeddings = np.concatenate(
-                [uncond_embeddings, text_embeddings])
 
-        latents_dtype = text_embeddings.dtype
-        init_image = init_image.astype(latents_dtype)
-        # encode the init image into latents and scale the latents
-        init_latents = self.vae_encoder(sample=init_image)[0]
-        init_latents = 0.18215 * init_latents
-
-        if isinstance(prompt, str):
-            prompt = [prompt]
-        if len(prompt) > init_latents.shape[0] and len(
-                prompt) % init_latents.shape[0] == 0:
-            # expand init_latents for batch_size
-            deprecation_message = (
-                f"You have passed {len(prompt)} text prompts (`prompt`), but only {init_latents.shape[0]} initial"
-                " images (`init_image`). Initial images are now duplicating to match the number of text prompts. Note"
-                " that this behavior is deprecated and will be removed in a version 1.0.0. Please make sure to update"
-                " your script to pass as many init images as text prompts to suppress this warning."
-            )
-            deprecate("len(prompt) != len(init_image)",
-                      "1.0.0",
-                      deprecation_message,
-                      standard_warn=False)
-            additional_image_per_prompt = len(prompt) // init_latents.shape[0]
-            init_latents = np.concatenate([init_latents] *
-                                          additional_image_per_prompt *
-                                          num_images_per_prompt,
-                                          axis=0)
-        elif len(prompt) > init_latents.shape[0] and len(
-                prompt) % init_latents.shape[0] != 0:
-            raise ValueError(
-                f"Cannot duplicate `init_image` of batch size {init_latents.shape[0]} to {len(prompt)} text prompts."
-            )
-        else:
-            init_latents = np.concatenate([init_latents] *
-                                          num_images_per_prompt,
-                                          axis=0)
-
-        # get the original timestep using init_timestep
-        offset = self.scheduler.config.get("steps_offset", 0)
-        init_timestep = int(num_inference_steps * strength) + offset
-        init_timestep = min(init_timestep, num_inference_steps)
-
-        timesteps = self.scheduler.timesteps.numpy()[-init_timestep]
-        timesteps = np.array([timesteps] * batch_size * num_images_per_prompt,
-                             dtype="int64")
+        # 3. Encode input prompt
+        text_embeddings = self._encode_prompt(
+            prompt, num_images_per_prompt, do_classifier_free_guidance, negative_prompt
+        )
 
-        # add noise to latents using the timesteps
-        noise = generator.randn(*init_latents.shape).astype(latents_dtype)
-        init_latents = self.scheduler.add_noise(paddle.to_tensor(init_latents),
-                                                paddle.to_tensor(noise),
-                                                paddle.to_tensor(timesteps))
-        init_latents = init_latents.numpy()
+        # 4. Preprocess image
+        if isinstance(image, PIL.Image.Image):
+            image = preprocess(image)
 
-        # prepare extra kwargs for the scheduler step, since not all schedulers have the same signature
-        # eta (η) is only used with the DDIMScheduler, it will be ignored for other schedulers.
-        # eta corresponds to η in DDIM paper: https://arxiv.org/abs/2010.02502
-        # and should be between [0, 1]
-        accepts_eta = "eta" in set(
-            inspect.signature(self.scheduler.step).parameters.keys())
-        extra_step_kwargs = {}
-        if accepts_eta:
-            extra_step_kwargs["eta"] = eta
+        # 5. set timesteps
+        self.scheduler.set_timesteps(num_inference_steps)
+        timesteps, num_inference_steps = self.get_timesteps(num_inference_steps, strength)
+        latent_timestep = timesteps[:1].repeat(batch_size * num_images_per_prompt)
 
-        latents = init_latents
+        # 6. Prepare latent variables
+        latents = self.prepare_latents(
+            image, latent_timestep, batch_size, num_images_per_prompt, text_embeddings.dtype, generator, noise
+        )
 
-        t_start = max(num_inference_steps - init_timestep + offset, 0)
+        # 7. Prepare extra step kwargs.
+        extra_step_kwargs = self.prepare_extra_step_kwargs(eta)
 
-        timesteps = self.scheduler.timesteps[t_start:].numpy()
+        # 8. Denoising loop
+        num_warmup_steps = len(timesteps) - num_inference_steps * self.scheduler.order
+        with self.progress_bar(total=num_inference_steps) as progress_bar:
+            for i, t in enumerate(timesteps):
+                tensor_t = paddle.to_tensor(t)
+                # expand the latents if we are doing classifier free guidance
+                latent_model_input = np.concatenate([latents] * 2) if do_classifier_free_guidance else latents
+                latent_model_input = self.scheduler.scale_model_input(paddle.to_tensor(latent_model_input), tensor_t)
+                latent_model_input = latent_model_input.numpy()
+
+                # predict the noise residual
+                noise_pred = self.unet(
+                    sample=latent_model_input.astype(np.float32),
+                    timestep=np.array([t], dtype=np.int64),
+                    encoder_hidden_states=text_embeddings.astype(np.float32),
+                )[0]
+
+                # perform guidance
+                if do_classifier_free_guidance:
+                    noise_pred_uncond, noise_pred_text = np.split(noise_pred, 2)
+                    noise_pred = noise_pred_uncond + guidance_scale * (noise_pred_text - noise_pred_uncond)
+
+                # compute the previous noisy sample x_t -> x_t-1
+                scheduler_output = self.scheduler.step(
+                    paddle.to_tensor(noise_pred), tensor_t, paddle.to_tensor(latents), **extra_step_kwargs
+                )
+                latents = scheduler_output.prev_sample.numpy()
 
-        for i, t in enumerate(self.progress_bar(timesteps)):
-            # expand the latents if we are doing classifier free guidance
-            latent_model_input = np.concatenate(
-                [latents] * 2) if do_classifier_free_guidance else latents
-            latent_model_input = self.scheduler.scale_model_input(
-                latent_model_input, t)
-
-            # predict the noise residual
-            noise_pred = self.unet(sample=latent_model_input.astype(np.float32),
-                                   timestep=np.array([t], dtype=np.int64),
-                                   encoder_hidden_states=text_embeddings.astype(
-                                       np.float32))[0]
-
-            # perform guidance
-            if do_classifier_free_guidance:
-                noise_pred_uncond, noise_pred_text = np.split(noise_pred, 2)
-                noise_pred = noise_pred_uncond + guidance_scale * (
-                    noise_pred_text - noise_pred_uncond)
-
-            # compute the previous noisy sample x_t -> x_t-1
-            noise_pred = paddle.to_tensor(noise_pred)
-            latents = paddle.to_tensor(latents)
-            t = paddle.to_tensor(t)
-            latents = self.scheduler.step(noise_pred, t, latents,
-                                          **extra_step_kwargs).prev_sample
-            latents = latents.numpy()
-
-            # call the callback, if provided
-            if callback is not None and i % callback_steps == 0:
-                callback(i, t, latents)
+                # call the callback, if provided
+                if i == len(timesteps) - 1 or ((i + 1) > num_warmup_steps and (i + 1) % self.scheduler.order == 0):
+                    progress_bar.update()
+                    if callback is not None and i % callback_steps == 0:
+                        callback(i, t, latents)
 
-        latents = 1 / 0.18215 * latents
-        # image = self.vae_decoder(latent_sample=latents)[0]
-        # it seems likes there is a strange result for using half-precision vae decoder if batchsize>1
-        image = np.concatenate([
-            self.vae_decoder(latent_sample=latents[i:i + 1])[0]
-            for i in range(latents.shape[0])
-        ])
-        image = np.clip(image / 2 + 0.5, 0, 1)
-        image = image.transpose((0, 2, 3, 1))
+        # 9. Post-processing
+        image = self.decode_latents(latents)
 
-        if self.safety_checker is not None:
-            safety_checker_input = self.feature_extractor(
-                self.numpy_to_pil(image),
-                return_tensors="np").pixel_values.astype(image.dtype)
-            # There will throw an error if use safety_checker batchsize>1
-            images, has_nsfw_concept = [], []
-            for i in range(image.shape[0]):
-                image_i, has_nsfw_concept_i = self.safety_checker(
-                    clip_input=safety_checker_input[i:i + 1],
-                    images=image[i:i + 1])
-                images.append(image_i)
-                has_nsfw_concept.append(has_nsfw_concept_i[0])
-            image = np.concatenate(images)
-        else:
-            has_nsfw_concept = None
+        # 10. Run safety checker
+        image, has_nsfw_concept = self.run_safety_checker(image, text_embeddings.dtype)
 
+        # 11. Convert to PIL
         if output_type == "pil":
             image = self.numpy_to_pil(image)
 
         if not return_dict:
             return (image, has_nsfw_concept)
 
-        return StableDiffusionPipelineOutput(
-            images=image, nsfw_content_detected=has_nsfw_concept)
+        return StableDiffusionPipelineOutput(images=image, nsfw_content_detected=has_nsfw_concept)
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/pipelines/stable_diffusion/pipeline_fastdeploy_stable_diffusion_inpaint.py` & `ppdiffusers-0.9.0/ppdiffusers/pipelines/stable_diffusion/pipeline_fastdeploy_stable_diffusion_inpaint.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,27 +15,27 @@
 import inspect
 from typing import Callable, List, Optional, Union
 
 import numpy as np
 import paddle
 import PIL
 
-from paddlenlp.utils.tools import compare_version
-
-if compare_version(PIL.__version__, "9.1.0") >= 0:
-    Resampling = PIL.Image.Resampling
-else:
-    Resampling = PIL.Image
 from paddlenlp.transformers import CLIPFeatureExtractor, CLIPTokenizer
 
-from ...configuration_utils import FrozenDict
 from ...fastdeploy_utils import FastDeployRuntimeModel
 from ...pipeline_utils import DiffusionPipeline
-from ...schedulers import DDIMScheduler, LMSDiscreteScheduler, PNDMScheduler
-from ...utils import deprecate, logging
+from ...schedulers import (
+    DDIMScheduler,
+    DPMSolverMultistepScheduler,
+    EulerAncestralDiscreteScheduler,
+    EulerDiscreteScheduler,
+    LMSDiscreteScheduler,
+    PNDMScheduler,
+)
+from ...utils import PIL_INTERPOLATION, logging
 from . import StableDiffusionPipelineOutput
 
 logger = logging.get_logger(__name__)  # pylint: disable=invalid-name
 
 NUM_UNET_INPUT_CHANNELS = 9
 NUM_LATENT_CHANNELS = 4
 
@@ -44,112 +44,268 @@
     image = np.array(image.convert("RGB").resize((latents_shape[1] * 8, latents_shape[0] * 8)))
     image = image[None].transpose(0, 3, 1, 2)
     image = image.astype(np.float32) / 127.5 - 1.0
 
     image_mask = np.array(mask.convert("L").resize((latents_shape[1] * 8, latents_shape[0] * 8)))
     masked_image = image * (image_mask < 127.5)
 
-    mask = mask.resize((latents_shape[1], latents_shape[0]), Resampling.NEAREST)
+    mask = mask.resize((latents_shape[1], latents_shape[0]), PIL_INTERPOLATION["nearest"])
     mask = np.array(mask.convert("L"))
     mask = mask.astype(np.float32) / 255.0
     mask = mask[None, None]
     mask[mask < 0.5] = 0
     mask[mask >= 0.5] = 1
 
     return mask, masked_image
 
 
 class FastDeployStableDiffusionInpaintPipeline(DiffusionPipeline):
     r"""
-    Pipeline for text-guided image inpainting using Stable Diffusion. *This is an experimental feature*.
+    Pipeline for text-guided image inpainting using Stable Diffusion.
 
     This model inherits from [`DiffusionPipeline`]. Check the superclass documentation for the generic methods the
-    library implements for all the pipelines (such as downloading or saving, running on a particular device, etc.)
+    library implements for all the pipelines (such as downloading or saving etc.)
 
     Args:
-        vae ([`AutoencoderKL`]):
-            Variational Auto-Encoder (VAE) Model to encode and decode images to and from latent representations.
-        text_encoder ([`CLIPTextModel`]):
+        vae_encoder ([`FastDeployRuntimeModel`]):
+            Variational Auto-Encoder (VAE) Model to encode images to latent representations.
+        vae_decoder ([`FastDeployRuntimeModel`]):
+            Variational Auto-Encoder (VAE) Model to decode images from latent representations.
+        text_encoder ([`FastDeployRuntimeModel`]):
             Frozen text-encoder. Stable Diffusion uses the text portion of
             [CLIP](https://huggingface.co/docs/transformers/model_doc/clip#transformers.CLIPTextModel), specifically
             the [clip-vit-large-patch14](https://huggingface.co/openai/clip-vit-large-patch14) variant.
         tokenizer (`CLIPTokenizer`):
             Tokenizer of class
             [CLIPTokenizer](https://huggingface.co/docs/transformers/v4.21.0/en/model_doc/clip#transformers.CLIPTokenizer).
-        unet ([`UNet2DConditionModel`]): Conditional U-Net architecture to denoise the encoded image latents.
+        unet ([`FastDeployRuntimeModel`]): Conditional U-Net architecture to denoise the encoded image latents.
         scheduler ([`SchedulerMixin`]):
-            A scheduler to be used in combination with `unet` to denoise the encoded image latens. Can be one of
-            [`DDIMScheduler`], [`LMSDiscreteScheduler`], or [`PNDMScheduler`].
-        safety_checker ([`StableDiffusionSafetyChecker`]):
+            A scheduler to be used in combination with `unet` to denoise the encoded image latents. Can be one of
+            [`DDIMScheduler`], [`LMSDiscreteScheduler`], [`PNDMScheduler`], [`EulerDiscreteScheduler`], [`EulerAncestralDiscreteScheduler`]
+            or [`DPMSolverMultistepScheduler`].
+        safety_checker ([`FastDeployRuntimeModel`]):
             Classification module that estimates whether generated images could be considered offensive or harmful.
             Please, refer to the [model card](https://huggingface.co/runwayml/stable-diffusion-v1-5) for details.
         feature_extractor ([`CLIPFeatureExtractor`]):
             Model that extracts features from generated images to be used as inputs for the `safety_checker`.
     """
-    vae_encoder: FastDeployRuntimeModel
-    vae_decoder: FastDeployRuntimeModel
-    text_encoder: FastDeployRuntimeModel
-    tokenizer: CLIPTokenizer
-    unet: FastDeployRuntimeModel
-    scheduler: Union[DDIMScheduler, PNDMScheduler, LMSDiscreteScheduler]
-    safety_checker: FastDeployRuntimeModel
-    feature_extractor: CLIPFeatureExtractor
+    _optional_components = ["safety_checker", "feature_extractor"]
 
     def __init__(
         self,
         vae_encoder: FastDeployRuntimeModel,
         vae_decoder: FastDeployRuntimeModel,
         text_encoder: FastDeployRuntimeModel,
         tokenizer: CLIPTokenizer,
         unet: FastDeployRuntimeModel,
-        scheduler: Union[DDIMScheduler, PNDMScheduler, LMSDiscreteScheduler],
+        scheduler: Union[
+            DDIMScheduler,
+            PNDMScheduler,
+            LMSDiscreteScheduler,
+            EulerDiscreteScheduler,
+            EulerAncestralDiscreteScheduler,
+            DPMSolverMultistepScheduler,
+        ],
         safety_checker: FastDeployRuntimeModel,
         feature_extractor: CLIPFeatureExtractor,
+        requires_safety_checker: bool = True,
     ):
         super().__init__()
-        logger.info(
-            "`FastDeployStableDiffusionInpaintPipeline` is experimental and will very likely change in the future."
-        )
-
-        if hasattr(scheduler.config, "steps_offset") and scheduler.config.steps_offset != 1:
-            deprecation_message = (
-                f"The configuration file of this scheduler: {scheduler} is outdated. `steps_offset`"
-                f" should be set to 1 instead of {scheduler.config.steps_offset}. Please make sure "
-                "to update the config accordingly as leaving `steps_offset` might led to incorrect results"
-                " in future versions. If you have downloaded this checkpoint from the Hugging Face Hub,"
-                " it would be very nice if you could open a Pull request for the `scheduler/scheduler_config.json`"
-                " file"
-            )
-            deprecate("steps_offset!=1", "1.0.0", deprecation_message, standard_warn=False)
-            new_config = dict(scheduler.config)
-            new_config["steps_offset"] = 1
-            scheduler._internal_dict = FrozenDict(new_config)
-
-        if safety_checker is None:
+        if safety_checker is None and requires_safety_checker:
             logger.warning(
                 f"You have disabled the safety checker for {self.__class__} by passing `safety_checker=None`. Ensure"
                 " that you abide to the conditions of the Stable Diffusion license and do not expose unfiltered"
                 " results in services or applications open to the public. PaddleNLP team, diffusers team and Hugging Face"
                 " strongly recommend to keep the safety filter enabled in all public facing circumstances, disabling"
                 " it only for use-cases that involve analyzing network behavior or auditing its results. For more"
                 " information, please have a look at https://github.com/huggingface/diffusers/pull/254 ."
             )
+        if safety_checker is not None and feature_extractor is None:
+            raise ValueError(
+                "Make sure to define a feature extractor when loading {self.__class__} if you want to use the safety"
+                " checker. If you do not want to use the safety checker, you can pass `'safety_checker=None'` instead."
+            )
 
         self.register_modules(
             vae_encoder=vae_encoder,
             vae_decoder=vae_decoder,
             text_encoder=text_encoder,
             tokenizer=tokenizer,
             unet=unet,
             scheduler=scheduler,
             safety_checker=safety_checker,
             feature_extractor=feature_extractor,
         )
+        self.register_to_config(requires_safety_checker=requires_safety_checker)
+
+    def _encode_prompt(self, prompt, num_images_per_prompt, do_classifier_free_guidance, negative_prompt):
+        r"""
+        Encodes the prompt into text encoder hidden states.
+
+        Args:
+            prompt (`str` or `list(int)`):
+                prompt to be encoded
+            num_images_per_prompt (`int`):
+                number of images that should be generated per prompt
+            do_classifier_free_guidance (`bool`):
+                whether to use classifier free guidance or not
+            negative_prompt (`str` or `List[str]`):
+                The prompt or prompts not to guide the image generation. Ignored when not using guidance (i.e., ignored
+                if `guidance_scale` is less than `1`).
+        """
+        batch_size = len(prompt) if isinstance(prompt, list) else 1
+
+        # get prompt text embeddings
+        text_inputs = self.tokenizer(
+            prompt,
+            padding="max_length",
+            max_length=self.tokenizer.model_max_length,
+            truncation=True,
+            return_tensors="np",
+        )
+        text_input_ids = text_inputs.input_ids
+        untruncated_ids = self.tokenizer(prompt, padding="max_length", return_tensors="np").input_ids
+
+        if not np.array_equal(text_input_ids, untruncated_ids):
+            removed_text = self.tokenizer.batch_decode(untruncated_ids[:, self.tokenizer.model_max_length - 1 : -1])
+            logger.warning(
+                "The following part of your input was truncated because CLIP can only handle sequences up to"
+                f" {self.tokenizer.model_max_length} tokens: {removed_text}"
+            )
+
+        text_embeddings = self.text_encoder(input_ids=text_input_ids.astype(np.int64))[0]
+        text_embeddings = np.repeat(text_embeddings, num_images_per_prompt, axis=0)
+
+        # get unconditional embeddings for classifier free guidance
+        if do_classifier_free_guidance:
+            uncond_tokens: List[str]
+            if negative_prompt is None:
+                uncond_tokens = [""] * batch_size
+            elif type(prompt) is not type(negative_prompt):
+                raise TypeError(
+                    f"`negative_prompt` should be the same type to `prompt`, but got {type(negative_prompt)} !="
+                    f" {type(prompt)}."
+                )
+            elif isinstance(negative_prompt, str):
+                uncond_tokens = [negative_prompt] * batch_size
+            elif batch_size != len(negative_prompt):
+                raise ValueError(
+                    f"`negative_prompt`: {negative_prompt} has batch size {len(negative_prompt)}, but `prompt`:"
+                    f" {prompt} has batch size {batch_size}. Please make sure that passed `negative_prompt` matches"
+                    " the batch size of `prompt`."
+                )
+            else:
+                uncond_tokens = negative_prompt
+
+            max_length = text_input_ids.shape[-1]
+            uncond_input = self.tokenizer(
+                uncond_tokens,
+                padding="max_length",
+                max_length=max_length,
+                truncation=True,
+                return_tensors="np",
+            )
+            uncond_embeddings = self.text_encoder(input_ids=uncond_input.input_ids.astype(np.int64))[0]
+            uncond_embeddings = np.repeat(uncond_embeddings, num_images_per_prompt, axis=0)
+
+            # For classifier free guidance, we need to do two forward passes.
+            # Here we concatenate the unconditional and text embeddings into a single batch
+            # to avoid doing two forward passes
+            text_embeddings = np.concatenate([uncond_embeddings, text_embeddings])
+
+        return text_embeddings
+
+    def run_safety_checker(self, image, dtype):
+        if self.safety_checker is not None:
+            safety_checker_input = self.feature_extractor(
+                self.numpy_to_pil(image), return_tensors="np"
+            ).pixel_values.astype(dtype)
+            # There will throw an error if use safety_checker batchsize>1
+            images, has_nsfw_concept = [], []
+            for i in range(image.shape[0]):
+                image_i, has_nsfw_concept_i = self.safety_checker(
+                    clip_input=safety_checker_input[i : i + 1], images=image[i : i + 1]
+                )
+                images.append(image_i)
+                has_nsfw_concept.append(has_nsfw_concept_i[0])
+            image = np.concatenate(images)
+        else:
+            has_nsfw_concept = None
+        return image, has_nsfw_concept
+
+    def decode_latents(self, latents):
+        latents = 1 / 0.18215 * latents
+        image = np.concatenate(
+            [self.vae_decoder(latent_sample=latents[i : i + 1])[0] for i in range(latents.shape[0])]
+        )
+        image = np.clip(image / 2 + 0.5, 0, 1)
+        image = image.transpose([0, 2, 3, 1])
+        return image
+
+    def prepare_extra_step_kwargs(self, eta):
+        # prepare extra kwargs for the scheduler step, since not all schedulers have the same signature
+        # eta (η) is only used with the DDIMScheduler, it will be ignored for other schedulers.
+        # eta corresponds to η in DDIM paper: https://arxiv.org/abs/2010.02502
+        # and should be between [0, 1]
+
+        accepts_eta = "eta" in set(inspect.signature(self.scheduler.step).parameters.keys())
+        extra_step_kwargs = {}
+        if accepts_eta:
+            extra_step_kwargs["eta"] = eta
+
+        return extra_step_kwargs
+
+    def check_inputs(self, prompt, height, width, callback_steps):
+        if not isinstance(prompt, str) and not isinstance(prompt, list):
+            raise ValueError(f"`prompt` has to be of type `str` or `list` but is {type(prompt)}")
+
+        if height % 8 != 0 or width % 8 != 0:
+            raise ValueError(f"`height` and `width` have to be divisible by 8 but are {height} and {width}.")
+
+        if (callback_steps is None) or (
+            callback_steps is not None and (not isinstance(callback_steps, int) or callback_steps <= 0)
+        ):
+            raise ValueError(
+                f"`callback_steps` has to be a positive integer but is {callback_steps} of type"
+                f" {type(callback_steps)}."
+            )
+
+    def prepare_latents(self, batch_size, num_channels_latents, height, width, dtype, generator, latents=None):
+        if generator is None:
+            generator = np.random
+
+        latents_shape = (batch_size, num_channels_latents, height // 8, width // 8)
+        if latents is None:
+            latents = generator.randn(*latents_shape).astype(dtype)
+        elif latents.shape != latents_shape:
+            raise ValueError(f"Unexpected latents shape, got {latents.shape}, expected {latents_shape}")
+
+        # scale the initial noise by the standard deviation required by the scheduler
+        latents = latents * float(self.scheduler.init_noise_sigma)
+        return latents
+
+    def prepare_mask_latents(self, mask, masked_image, batch_size, dtype, do_classifier_free_guidance):
+        mask = mask.astype(dtype)
+        masked_image = masked_image.astype(dtype)
+
+        # encode the mask image into latents space so we can concatenate it to the latents
+        masked_image_latents = self.vae_encoder(sample=masked_image)[0]
+        masked_image_latents = 0.18215 * masked_image_latents
+
+        # duplicate mask and masked_image_latents for each generation per prompt, using mps friendly method
+        mask = mask.repeat(batch_size, 0)
+        masked_image_latents = masked_image_latents.repeat(batch_size, 0)
+
+        mask = np.concatenate([mask] * 2) if do_classifier_free_guidance else mask
+        masked_image_latents = (
+            np.concatenate([masked_image_latents] * 2) if do_classifier_free_guidance else masked_image_latents
+        )
+        masked_image_latents = masked_image_latents.astype(dtype)
+        return mask, masked_image_latents
 
-    @paddle.no_grad()
     def __call__(
         self,
         prompt: Union[str, List[str]],
         image: PIL.Image.Image,
         mask_image: PIL.Image.Image,
         height: int = 512,
         width: int = 512,
@@ -160,15 +316,14 @@
         eta: float = 0.0,
         generator: Optional[np.random.RandomState] = None,
         latents: Optional[np.ndarray] = None,
         output_type: Optional[str] = "pil",
         return_dict: bool = True,
         callback: Optional[Callable[[int, int, np.ndarray], None]] = None,
         callback_steps: Optional[int] = 1,
-        **kwargs,
     ):
         r"""
         Function invoked when calling the pipeline for generation.
 
         Args:
             prompt (`str` or `List[str]`):
                 The prompt or prompts to guide the image generation.
@@ -223,217 +378,117 @@
         Returns:
             [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] or `tuple`:
             [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] if `return_dict` is True, otherwise a `tuple.
             When returning a tuple, the first element is a list with the generated images, and the second element is a
             list of `bool`s denoting whether the corresponding generated image likely represents "not-safe-for-work"
             (nsfw) content, according to the `safety_checker`.
         """
-        if isinstance(prompt, str):
-            batch_size = 1
-        elif isinstance(prompt, list):
-            batch_size = len(prompt)
-        else:
-            raise ValueError(f"`prompt` has to be of type `str` or `list` but is {type(prompt)}")
-
-        if height % 8 != 0 or width % 8 != 0:
-            raise ValueError(f"`height` and `width` have to be divisible by 8 but are {height} and {width}.")
-
-        if (callback_steps is None) or (
-            callback_steps is not None and (not isinstance(callback_steps, int) or callback_steps <= 0)
-        ):
-            raise ValueError(
-                f"`callback_steps` has to be a positive integer but is {callback_steps} of type"
-                f" {type(callback_steps)}."
-            )
-
-        if generator is None:
-            generator = np.random
-
-        # set timesteps
-        self.scheduler.set_timesteps(num_inference_steps)
-
-        # get prompt text embeddings
-        text_inputs = self.tokenizer(
-            prompt,
-            padding="max_length",
-            max_length=self.tokenizer.model_max_length,
-            return_tensors="np",
-        )
-        text_input_ids = text_inputs.input_ids
-
-        if text_input_ids.shape[-1] > self.tokenizer.model_max_length:
-            removed_text = self.tokenizer.batch_decode(text_input_ids[:, self.tokenizer.model_max_length :])
-            logger.warning(
-                "The following part of your input was truncated because CLIP can only handle sequences up to"
-                f" {self.tokenizer.model_max_length} tokens: {removed_text}"
-            )
-            text_input_ids = text_input_ids[:, : self.tokenizer.model_max_length]
-        text_embeddings = self.text_encoder(input_ids=text_input_ids.astype(np.int64))[0]
-
-        # duplicate text embeddings for each generation per prompt
-        text_embeddings = np.repeat(text_embeddings, num_images_per_prompt, axis=0)
+        # 1. Check inputs
+        self.check_inputs(prompt, height, width, callback_steps)
 
+        # 2. Define call parameters
+        batch_size = 1 if isinstance(prompt, str) else len(prompt)
         # here `guidance_scale` is defined analog to the guidance weight `w` of equation (2)
         # of the Imagen paper: https://arxiv.org/pdf/2205.11487.pdf . `guidance_scale = 1`
         # corresponds to doing no classifier free guidance.
         do_classifier_free_guidance = guidance_scale > 1.0
-        # get unconditional embeddings for classifier free guidance
-        if do_classifier_free_guidance:
-            uncond_tokens: List[str]
-            if negative_prompt is None:
-                uncond_tokens = [""]
-            elif type(prompt) is not type(negative_prompt):
-                raise TypeError(
-                    f"`negative_prompt` should be the same type to `prompt`, but got {type(negative_prompt)} !="
-                    f" {type(prompt)}."
-                )
-            elif isinstance(negative_prompt, str):
-                uncond_tokens = [negative_prompt] * batch_size
-            elif batch_size != len(negative_prompt):
-                raise ValueError(
-                    f"`negative_prompt`: {negative_prompt} has batch size {len(negative_prompt)}, but `prompt`:"
-                    f" {prompt} has batch size {batch_size}. Please make sure that passed `negative_prompt` matches"
-                    " the batch size of `prompt`."
-                )
-            else:
-                uncond_tokens = negative_prompt
 
-            max_length = text_input_ids.shape[-1]
-            uncond_input = self.tokenizer(
-                uncond_tokens,
-                padding="max_length",
-                max_length=max_length,
-                truncation=True,
-                return_tensors="np",
-            )
-            uncond_input_ids = uncond_input.input_ids
-            uncond_embeddings = self.text_encoder(input_ids=uncond_input_ids.astype(np.int64))[0]
-
-            # duplicate unconditional embeddings for each generation per prompt
-            uncond_embeddings = np.repeat(uncond_embeddings, num_images_per_prompt, axis=0)
+        # 3. Encode input prompt
+        text_embeddings = self._encode_prompt(
+            prompt, num_images_per_prompt, do_classifier_free_guidance, negative_prompt
+        )
 
-            # For classifier free guidance, we need to do two forward passes.
-            # Here we concatenate the unconditional and text embeddings into a single batch
-            # to avoid doing two forward passes
-            text_embeddings = np.concatenate([uncond_embeddings, text_embeddings])
+        # 4. set timesteps
+        self.scheduler.set_timesteps(num_inference_steps)
+        timesteps = self.scheduler.timesteps.numpy()
 
+        # 5. Prepare latent variables
         num_channels_latents = NUM_LATENT_CHANNELS
-        latents_shape = (batch_size * num_images_per_prompt, num_channels_latents, height // 8, width // 8)
-        latents_dtype = text_embeddings.dtype
-        if latents is None:
-            latents = generator.randn(*latents_shape).astype(latents_dtype)
-        else:
-            if latents.shape != latents_shape:
-                raise ValueError(f"Unexpected latents shape, got {latents.shape}, expected {latents_shape}")
-
-        # prepare mask and masked_image
-        mask, masked_image = prepare_mask_and_masked_image(image, mask_image, latents_shape[-2:])
-        mask = mask.astype(latents.dtype)
-        masked_image = masked_image.astype(latents.dtype)
-
-        masked_image_latents = self.vae_encoder(sample=masked_image)[0]
-        masked_image_latents = 0.18215 * masked_image_latents
-
-        # duplicate mask and masked_image_latents for each generation per prompt
-        mask = mask.repeat(batch_size * num_images_per_prompt, 0)
-        masked_image_latents = masked_image_latents.repeat(batch_size * num_images_per_prompt, 0)
-
-        mask = np.concatenate([mask] * 2) if do_classifier_free_guidance else mask
-        masked_image_latents = (
-            np.concatenate([masked_image_latents] * 2) if do_classifier_free_guidance else masked_image_latents
+        latents = self.prepare_latents(
+            batch_size * num_images_per_prompt,
+            num_channels_latents,
+            height,
+            width,
+            text_embeddings.dtype,
+            generator,
+            latents,
         )
 
+        # 6. Preprocess mask and image
+        if isinstance(image, PIL.Image.Image) and isinstance(mask_image, PIL.Image.Image):
+            mask, masked_image = prepare_mask_and_masked_image(image, mask_image, latents.shape[-2:])
+
+        # 7. Prepare mask latent variables
+        mask, masked_image_latents = self.prepare_mask_latents(
+            mask,
+            masked_image,
+            batch_size * num_images_per_prompt,
+            text_embeddings.dtype,
+            do_classifier_free_guidance,
+        )
         num_channels_mask = mask.shape[1]
         num_channels_masked_image = masked_image_latents.shape[1]
 
+        # 8. Check that sizes of mask, masked image and latents match
         unet_input_channels = NUM_UNET_INPUT_CHANNELS
         if num_channels_latents + num_channels_mask + num_channels_masked_image != unet_input_channels:
             raise ValueError(
                 "Incorrect configuration settings! The config of `pipeline.unet` expects"
                 f" {unet_input_channels} but received `num_channels_latents`: {num_channels_latents} +"
                 f" `num_channels_mask`: {num_channels_mask} + `num_channels_masked_image`: {num_channels_masked_image}"
                 f" = {num_channels_latents+num_channels_masked_image+num_channels_mask}. Please verify the config of"
                 " `pipeline.unet` or your `mask_image` or `image` input."
             )
 
-        # set timesteps
-        self.scheduler.set_timesteps(num_inference_steps)
-
-        # scale the initial noise by the standard deviation required by the scheduler
-        init_noise_sigma = (
-            self.scheduler.init_noise_sigma.numpy()
-            if isinstance(self.scheduler.init_noise_sigma, paddle.Tensor)
-            else self.scheduler.init_noise_sigma
-        )
-        latents = latents * init_noise_sigma
+        # 9. Prepare extra step kwargs.
+        extra_step_kwargs = self.prepare_extra_step_kwargs(eta)
 
-        # prepare extra kwargs for the scheduler step, since not all schedulers have the same signature
-        # eta (η) is only used with the DDIMScheduler, it will be ignored for other schedulers.
-        # eta corresponds to η in DDIM paper: https://arxiv.org/abs/2010.02502
-        # and should be between [0, 1]
-        accepts_eta = "eta" in set(inspect.signature(self.scheduler.step).parameters.keys())
-        extra_step_kwargs = {}
-        if accepts_eta:
-            extra_step_kwargs["eta"] = eta
-        for i, t in enumerate(self.progress_bar(self.scheduler.timesteps)):
-            # expand the latents if we are doing classifier free guidance
-            latent_model_input = np.concatenate([latents] * 2) if do_classifier_free_guidance else latents
-            # concat latents, mask, masked_image_latnets in the channel dimension
-            latent_model_input = np.concatenate([latent_model_input, mask, masked_image_latents], axis=1)
-            latent_model_input = self.scheduler.scale_model_input(paddle.to_tensor(latent_model_input), t)
-            latent_model_input = latent_model_input.numpy()
-
-            # predict the noise residual
-            noise_pred = self.unet(
-                sample=latent_model_input.astype(np.float32),
-                timestep=np.array(t, dtype=np.int64),
-                encoder_hidden_states=text_embeddings.astype(np.float32),
-            )[0]
-            # perform guidance
-            if do_classifier_free_guidance:
-                noise_pred_uncond, noise_pred_text = np.split(noise_pred, 2)
-                noise_pred = noise_pred_uncond + guidance_scale * (noise_pred_text - noise_pred_uncond)
-
-            # compute the previous noisy sample x_t -> x_t-1
-
-            latents = self.scheduler.step(
-                paddle.to_tensor(noise_pred), paddle.to_tensor(t), paddle.to_tensor(latents), **extra_step_kwargs
-            ).prev_sample
-            latents = latents.numpy()
-
-            # call the callback, if provided
-            if callback is not None and i % callback_steps == 0:
-                callback(i, t, latents)
+        # 10. Denoising loop
+        num_warmup_steps = len(timesteps) - num_inference_steps * self.scheduler.order
+        with self.progress_bar(total=num_inference_steps) as progress_bar:
+            for i, t in enumerate(timesteps):
+                tensor_t = paddle.to_tensor(t)
+                # expand the latents if we are doing classifier free guidance
+                latent_model_input = np.concatenate([latents] * 2) if do_classifier_free_guidance else latents
+                # concat latents, mask, masked_image_latnets in the channel dimension
+                latent_model_input = self.scheduler.scale_model_input(paddle.to_tensor(latent_model_input), tensor_t)
+                latent_model_input = latent_model_input.numpy()
+                latent_model_input = np.concatenate([latent_model_input, mask, masked_image_latents], axis=1)
+
+                # predict the noise residual
+                noise_pred = self.unet(
+                    sample=latent_model_input.astype(np.float32),
+                    timestep=np.array([t], dtype=np.int64),
+                    encoder_hidden_states=text_embeddings.astype(np.float32),
+                )[0]
+
+                # perform guidance
+                if do_classifier_free_guidance:
+                    noise_pred_uncond, noise_pred_text = np.split(noise_pred, 2)
+                    noise_pred = noise_pred_uncond + guidance_scale * (noise_pred_text - noise_pred_uncond)
+
+                # compute the previous noisy sample x_t -> x_t-1
+                scheduler_output = self.scheduler.step(
+                    paddle.to_tensor(noise_pred), tensor_t, paddle.to_tensor(latents), **extra_step_kwargs
+                )
+                latents = scheduler_output.prev_sample.numpy()
 
-        latents = 1 / 0.18215 * latents
-        # image = self.vae_decoder(latent_sample=latents)[0]
-        # it seems likes there is a strange result for using half-precision vae decoder if batchsize>1
-        image = np.concatenate(
-            [self.vae_decoder(latent_sample=latents[i : i + 1])[0] for i in range(latents.shape[0])]
-        )
+                # call the callback, if provided
+                if i == len(timesteps) - 1 or ((i + 1) > num_warmup_steps and (i + 1) % self.scheduler.order == 0):
+                    progress_bar.update()
+                    if callback is not None and i % callback_steps == 0:
+                        callback(i, t, latents)
 
-        image = np.clip(image / 2 + 0.5, 0, 1)
-        image = image.transpose((0, 2, 3, 1))
+        # 11. Post-processing
+        image = self.decode_latents(latents)
 
-        if self.safety_checker is not None:
-            safety_checker_input = self.feature_extractor(
-                self.numpy_to_pil(image), return_tensors="np"
-            ).pixel_values.astype(image.dtype)
-            # There will throw an error if use safety_checker batchsize>1
-            images, has_nsfw_concept = [], []
-            for i in range(image.shape[0]):
-                image_i, has_nsfw_concept_i = self.safety_checker(
-                    clip_input=safety_checker_input[i : i + 1], images=image[i : i + 1]
-                )
-                images.append(image_i)
-                has_nsfw_concept.append(has_nsfw_concept_i[0])
-            image = np.concatenate(images)
-        else:
-            has_nsfw_concept = None
+        # 12. Run safety checker
+        image, has_nsfw_concept = self.run_safety_checker(image, text_embeddings.dtype)
 
+        # 13. Convert to PIL
         if output_type == "pil":
             image = self.numpy_to_pil(image)
 
         if not return_dict:
             return (image, has_nsfw_concept)
 
         return StableDiffusionPipelineOutput(images=image, nsfw_content_detected=has_nsfw_concept)
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/pipelines/stable_diffusion/pipeline_onnx_stable_diffusion_img2img.py` & `ppdiffusers-0.9.0/ppdiffusers/pipelines/stable_diffusion/pipeline_fastdeploy_stable_diffusion_inpaint_legacy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (c) 2022 PaddlePaddle Authors. All Rights Reserved.
+# Copyright 2022 The HuggingFace Team. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,157 +15,341 @@
 
 import inspect
 from typing import Callable, List, Optional, Union
 
 import numpy as np
 import paddle
 import PIL
-from paddlenlp.utils.tools import compare_version
-if compare_version(PIL.__version__, "9.1.0") >= 0:
-    Resampling = PIL.Image.Resampling
-else:
-    Resampling = PIL.Image
 
 from paddlenlp.transformers import CLIPFeatureExtractor, CLIPTokenizer
 
-from ...configuration_utils import FrozenDict
-from ...onnx_utils import OnnxRuntimeModel
+from ...fastdeploy_utils import FastDeployRuntimeModel
 from ...pipeline_utils import DiffusionPipeline
-from ...schedulers import DDIMScheduler, LMSDiscreteScheduler, PNDMScheduler
-from ...utils import deprecate, logging
+from ...schedulers import (
+    DDIMScheduler,
+    DPMSolverMultistepScheduler,
+    EulerAncestralDiscreteScheduler,
+    EulerDiscreteScheduler,
+    LMSDiscreteScheduler,
+    PNDMScheduler,
+)
+from ...utils import PIL_INTERPOLATION, logging
 from . import StableDiffusionPipelineOutput
 
 logger = logging.get_logger(__name__)  # pylint: disable=invalid-name
 
 
-def preprocess(image):
+def preprocess_image(image):
     w, h = image.size
     w, h = map(lambda x: x - x % 32, (w, h))  # resize to integer multiple of 32
-    image = image.resize((w, h), resample=Resampling.LANCZOS)
+    image = image.resize((w, h), resample=PIL_INTERPOLATION["lanczos"])
     image = np.array(image).astype(np.float32) / 255.0
     image = image[None].transpose(0, 3, 1, 2)
     return 2.0 * image - 1.0
 
 
-class OnnxStableDiffusionImg2ImgPipeline(DiffusionPipeline):
+def preprocess_mask(mask, scale_factor=8):
+    mask = mask.convert("L")
+    w, h = mask.size
+    w, h = map(lambda x: x - x % 32, (w, h))  # resize to integer multiple of 32
+    mask = mask.resize((w // scale_factor, h // scale_factor), resample=PIL_INTERPOLATION["nearest"])
+    mask = np.array(mask).astype(np.float32) / 255.0
+    mask = np.tile(mask, (4, 1, 1))
+    mask = mask[None].transpose(0, 1, 2, 3)  # what does this step do?
+    mask = 1 - mask  # repaint white, keep black
+    return mask
+
+
+class FastDeployStableDiffusionInpaintPipelineLegacy(DiffusionPipeline):
     r"""
-    Pipeline for text-guided image to image generation using Stable Diffusion.
+    Pipeline for text-guided image inpainting legacy using Stable Diffusion.
+
     This model inherits from [`DiffusionPipeline`]. Check the superclass documentation for the generic methods the
-    library implements for all the pipelines (such as downloading or saving, running on a particular device, etc.)
+    library implements for all the pipelines (such as downloading or saving etc.)
+
     Args:
-        vae ([`AutoencoderKL`]):
-            Variational Auto-Encoder (VAE) Model to encode and decode images to and from latent representations.
-        text_encoder ([`CLIPTextModel`]):
+        vae_encoder ([`FastDeployRuntimeModel`]):
+            Variational Auto-Encoder (VAE) Model to encode images to latent representations.
+        vae_decoder ([`FastDeployRuntimeModel`]):
+            Variational Auto-Encoder (VAE) Model to decode images from latent representations.
+        text_encoder ([`FastDeployRuntimeModel`]):
             Frozen text-encoder. Stable Diffusion uses the text portion of
             [CLIP](https://huggingface.co/docs/transformers/model_doc/clip#transformers.CLIPTextModel), specifically
             the [clip-vit-large-patch14](https://huggingface.co/openai/clip-vit-large-patch14) variant.
         tokenizer (`CLIPTokenizer`):
             Tokenizer of class
             [CLIPTokenizer](https://huggingface.co/docs/transformers/v4.21.0/en/model_doc/clip#transformers.CLIPTokenizer).
-        unet ([`UNet2DConditionModel`]): Conditional U-Net architecture to denoise the encoded image latents.
+        unet ([`FastDeployRuntimeModel`]): Conditional U-Net architecture to denoise the encoded image latents.
         scheduler ([`SchedulerMixin`]):
-            A scheduler to be used in combination with `unet` to denoise the encoded image latens. Can be one of
-            [`DDIMScheduler`], [`LMSDiscreteScheduler`], or [`PNDMScheduler`].
-        safety_checker ([`StableDiffusionSafetyChecker`]):
+            A scheduler to be used in combination with `unet` to denoise the encoded image latents. Can be one of
+            [`DDIMScheduler`], [`LMSDiscreteScheduler`], [`PNDMScheduler`], [`EulerDiscreteScheduler`], [`EulerAncestralDiscreteScheduler`]
+            or [`DPMSolverMultistepScheduler`].
+        safety_checker ([`FastDeployRuntimeModel`]):
             Classification module that estimates whether generated images could be considered offensive or harmful.
             Please, refer to the [model card](https://huggingface.co/runwayml/stable-diffusion-v1-5) for details.
         feature_extractor ([`CLIPFeatureExtractor`]):
             Model that extracts features from generated images to be used as inputs for the `safety_checker`.
     """
-    vae_encoder: OnnxRuntimeModel
-    vae_decoder: OnnxRuntimeModel
-    text_encoder: OnnxRuntimeModel
-    tokenizer: CLIPTokenizer
-    unet: OnnxRuntimeModel
-    scheduler: Union[DDIMScheduler, PNDMScheduler, LMSDiscreteScheduler]
-    safety_checker: OnnxRuntimeModel
-    feature_extractor: CLIPFeatureExtractor
+    _optional_components = ["safety_checker", "feature_extractor"]
 
     def __init__(
         self,
-        vae_encoder: OnnxRuntimeModel,
-        vae_decoder: OnnxRuntimeModel,
-        text_encoder: OnnxRuntimeModel,
+        vae_encoder: FastDeployRuntimeModel,
+        vae_decoder: FastDeployRuntimeModel,
+        text_encoder: FastDeployRuntimeModel,
         tokenizer: CLIPTokenizer,
-        unet: OnnxRuntimeModel,
-        scheduler: Union[DDIMScheduler, PNDMScheduler, LMSDiscreteScheduler],
-        safety_checker: OnnxRuntimeModel,
+        unet: FastDeployRuntimeModel,
+        scheduler: Union[
+            DDIMScheduler,
+            PNDMScheduler,
+            LMSDiscreteScheduler,
+            EulerDiscreteScheduler,
+            EulerAncestralDiscreteScheduler,
+            DPMSolverMultistepScheduler,
+        ],
+        safety_checker: FastDeployRuntimeModel,
         feature_extractor: CLIPFeatureExtractor,
+        requires_safety_checker: bool = True,
     ):
         super().__init__()
 
-        if hasattr(scheduler.config,
-                   "steps_offset") and scheduler.config.steps_offset != 1:
-            deprecation_message = (
-                f"The configuration file of this scheduler: {scheduler} is outdated. `steps_offset`"
-                f" should be set to 1 instead of {scheduler.config.steps_offset}. Please make sure "
-                "to update the config accordingly as leaving `steps_offset` might led to incorrect results"
-                " in future versions. If you have downloaded this checkpoint from the Hugging Face Hub,"
-                " it would be very nice if you could open a Pull request for the `scheduler/scheduler_config.json`"
-                " file")
-            deprecate("steps_offset!=1",
-                      "1.0.0",
-                      deprecation_message,
-                      standard_warn=False)
-            new_config = dict(scheduler.config)
-            new_config["steps_offset"] = 1
-            scheduler._internal_dict = FrozenDict(new_config)
-
-        if safety_checker is None:
+        if safety_checker is None and requires_safety_checker:
             logger.warning(
                 f"You have disabled the safety checker for {self.__class__} by passing `safety_checker=None`. Ensure"
                 " that you abide to the conditions of the Stable Diffusion license and do not expose unfiltered"
                 " results in services or applications open to the public. PaddleNLP team, diffusers team and Hugging Face"
                 " strongly recommend to keep the safety filter enabled in all public facing circumstances, disabling"
                 " it only for use-cases that involve analyzing network behavior or auditing its results. For more"
                 " information, please have a look at https://github.com/huggingface/diffusers/pull/254 ."
             )
+        if safety_checker is not None and feature_extractor is None:
+            raise ValueError(
+                "Make sure to define a feature extractor when loading {self.__class__} if you want to use the safety"
+                " checker. If you do not want to use the safety checker, you can pass `'safety_checker=None'` instead."
+            )
 
         self.register_modules(
             vae_encoder=vae_encoder,
             vae_decoder=vae_decoder,
             text_encoder=text_encoder,
             tokenizer=tokenizer,
             unet=unet,
             scheduler=scheduler,
             safety_checker=safety_checker,
             feature_extractor=feature_extractor,
         )
 
+        self.register_to_config(requires_safety_checker=requires_safety_checker)
+
+    def _encode_prompt(self, prompt, num_images_per_prompt, do_classifier_free_guidance, negative_prompt):
+        r"""
+        Encodes the prompt into text encoder hidden states.
+
+        Args:
+            prompt (`str` or `list(int)`):
+                prompt to be encoded
+            num_images_per_prompt (`int`):
+                number of images that should be generated per prompt
+            do_classifier_free_guidance (`bool`):
+                whether to use classifier free guidance or not
+            negative_prompt (`str` or `List[str]`):
+                The prompt or prompts not to guide the image generation. Ignored when not using guidance (i.e., ignored
+                if `guidance_scale` is less than `1`).
+        """
+        batch_size = len(prompt) if isinstance(prompt, list) else 1
+
+        # get prompt text embeddings
+        text_inputs = self.tokenizer(
+            prompt,
+            padding="max_length",
+            max_length=self.tokenizer.model_max_length,
+            truncation=True,
+            return_tensors="np",
+        )
+        text_input_ids = text_inputs.input_ids
+        untruncated_ids = self.tokenizer(prompt, padding="max_length", return_tensors="np").input_ids
+
+        if not np.array_equal(text_input_ids, untruncated_ids):
+            removed_text = self.tokenizer.batch_decode(untruncated_ids[:, self.tokenizer.model_max_length - 1 : -1])
+            logger.warning(
+                "The following part of your input was truncated because CLIP can only handle sequences up to"
+                f" {self.tokenizer.model_max_length} tokens: {removed_text}"
+            )
+
+        text_embeddings = self.text_encoder(input_ids=text_input_ids.astype(np.int64))[0]
+        text_embeddings = np.repeat(text_embeddings, num_images_per_prompt, axis=0)
+
+        # get unconditional embeddings for classifier free guidance
+        if do_classifier_free_guidance:
+            uncond_tokens: List[str]
+            if negative_prompt is None:
+                uncond_tokens = [""] * batch_size
+            elif type(prompt) is not type(negative_prompt):
+                raise TypeError(
+                    f"`negative_prompt` should be the same type to `prompt`, but got {type(negative_prompt)} !="
+                    f" {type(prompt)}."
+                )
+            elif isinstance(negative_prompt, str):
+                uncond_tokens = [negative_prompt] * batch_size
+            elif batch_size != len(negative_prompt):
+                raise ValueError(
+                    f"`negative_prompt`: {negative_prompt} has batch size {len(negative_prompt)}, but `prompt`:"
+                    f" {prompt} has batch size {batch_size}. Please make sure that passed `negative_prompt` matches"
+                    " the batch size of `prompt`."
+                )
+            else:
+                uncond_tokens = negative_prompt
+
+            max_length = text_input_ids.shape[-1]
+            uncond_input = self.tokenizer(
+                uncond_tokens,
+                padding="max_length",
+                max_length=max_length,
+                truncation=True,
+                return_tensors="np",
+            )
+            uncond_embeddings = self.text_encoder(input_ids=uncond_input.input_ids.astype(np.int64))[0]
+            uncond_embeddings = np.repeat(uncond_embeddings, num_images_per_prompt, axis=0)
+
+            # For classifier free guidance, we need to do two forward passes.
+            # Here we concatenate the unconditional and text embeddings into a single batch
+            # to avoid doing two forward passes
+            text_embeddings = np.concatenate([uncond_embeddings, text_embeddings])
+
+        return text_embeddings
+
+    def run_safety_checker(self, image, dtype):
+        if self.safety_checker is not None:
+            safety_checker_input = self.feature_extractor(
+                self.numpy_to_pil(image), return_tensors="np"
+            ).pixel_values.astype(dtype)
+            # There will throw an error if use safety_checker batchsize>1
+            images, has_nsfw_concept = [], []
+            for i in range(image.shape[0]):
+                image_i, has_nsfw_concept_i = self.safety_checker(
+                    clip_input=safety_checker_input[i : i + 1], images=image[i : i + 1]
+                )
+                images.append(image_i)
+                has_nsfw_concept.append(has_nsfw_concept_i[0])
+            image = np.concatenate(images)
+        else:
+            has_nsfw_concept = None
+        return image, has_nsfw_concept
+
+    def decode_latents(self, latents):
+        latents = 1 / 0.18215 * latents
+        image = np.concatenate(
+            [self.vae_decoder(latent_sample=latents[i : i + 1])[0] for i in range(latents.shape[0])]
+        )
+        image = np.clip(image / 2 + 0.5, 0, 1)
+        image = image.transpose([0, 2, 3, 1])
+        return image
+
+    def prepare_extra_step_kwargs(self, eta):
+        # prepare extra kwargs for the scheduler step, since not all schedulers have the same signature
+        # eta (η) is only used with the DDIMScheduler, it will be ignored for other schedulers.
+        # eta corresponds to η in DDIM paper: https://arxiv.org/abs/2010.02502
+        # and should be between [0, 1]
+
+        accepts_eta = "eta" in set(inspect.signature(self.scheduler.step).parameters.keys())
+        extra_step_kwargs = {}
+        if accepts_eta:
+            extra_step_kwargs["eta"] = eta
+
+        return extra_step_kwargs
+
+    def check_inputs(self, prompt, strength, callback_steps):
+        if not isinstance(prompt, str) and not isinstance(prompt, list):
+            raise ValueError(f"`prompt` has to be of type `str` or `list` but is {type(prompt)}")
+
+        if strength < 0 or strength > 1:
+            raise ValueError(f"The value of strength should in [1.0, 1.0] but is {strength}")
+
+        if (callback_steps is None) or (
+            callback_steps is not None and (not isinstance(callback_steps, int) or callback_steps <= 0)
+        ):
+            raise ValueError(
+                f"`callback_steps` has to be a positive integer but is {callback_steps} of type"
+                f" {type(callback_steps)}."
+            )
+
+    def get_timesteps(self, num_inference_steps, strength):
+        # get the original timestep using init_timestep
+        offset = self.scheduler.config.get("steps_offset", 0)
+        init_timestep = int(num_inference_steps * strength) + offset
+        init_timestep = min(init_timestep, num_inference_steps)
+
+        t_start = max(num_inference_steps - init_timestep + offset, 0)
+        timesteps = self.scheduler.timesteps.numpy()
+        timesteps = timesteps[t_start:]
+
+        return timesteps, num_inference_steps - t_start
+
+    def prepare_latents(self, image, timestep, batch_size, num_images_per_prompt, dtype, generator=None, noise=None):
+        if generator is None:
+            generator = np.random
+
+        image = image.astype(dtype)
+        init_latents = self.vae_encoder(sample=image)[0]
+        init_latents = 0.18215 * init_latents
+
+        # Expand init_latents for batch_size and num_images_per_prompt
+        init_latents = np.concatenate([init_latents] * batch_size * num_images_per_prompt, axis=0)
+        init_latents_orig = paddle.to_tensor(init_latents)
+
+        # add noise to latents using the timesteps
+        if noise is None:
+            noise = paddle.to_tensor(generator.randn(*init_latents.shape).astype(dtype))
+        elif list(noise.shape) != list(init_latents.shape):
+            raise ValueError(f"Unexpected noise shape, got {noise.shape}, expected {init_latents.shape}")
+        elif isinstance(noise, np.ndarray):
+            noise = paddle.to_tensor(noise, dtype=dtype)
+
+        init_latents = self.scheduler.add_noise(paddle.to_tensor(init_latents), noise, paddle.to_tensor(timestep))
+        latents = init_latents.numpy()
+        return latents, init_latents_orig, noise
+
     def __call__(
         self,
         prompt: Union[str, List[str]],
-        init_image: Union[np.ndarray, PIL.Image.Image],
+        image: Union[np.ndarray, PIL.Image.Image],
+        mask_image: Union[np.ndarray, PIL.Image.Image],
         strength: float = 0.8,
         num_inference_steps: Optional[int] = 50,
         guidance_scale: Optional[float] = 7.5,
         negative_prompt: Optional[Union[str, List[str]]] = None,
         num_images_per_prompt: Optional[int] = 1,
         eta: Optional[float] = 0.0,
         generator: Optional[np.random.RandomState] = None,
+        noise: Optional[np.ndarray] = None,
         output_type: Optional[str] = "pil",
         return_dict: bool = True,
         callback: Optional[Callable[[int, int, np.ndarray], None]] = None,
         callback_steps: Optional[int] = 1,
-        **kwargs,
     ):
         r"""
         Function invoked when calling the pipeline for generation.
+
         Args:
             prompt (`str` or `List[str]`):
                 The prompt or prompts to guide the image generation.
-            init_image (`np.ndarray` or `PIL.Image.Image`):
+            image (`nd.ndarray` or `PIL.Image.Image`):
                 `Image`, or tensor representing an image batch, that will be used as the starting point for the
-                process.
+                process. This is the image whose masked region will be inpainted.
+            mask_image (`nd.ndarray` or `PIL.Image.Image`):
+                `Image`, or tensor representing an image batch, to mask `image`. White pixels in the mask will be
+                replaced by noise and therefore repainted, while black pixels will be preserved. If `mask_image` is a
+                PIL image, it will be converted to a single channel (luminance) before use. If it's a tensor, it should
+                contain one color channel (L) instead of 3, so the expected shape would be `(B, H, W, 1)`.uu
             strength (`float`, *optional*, defaults to 0.8):
-                Conceptually, indicates how much to transform the reference `init_image`. Must be between 0 and 1.
-                `init_image` will be used as a starting point, adding more noise to it the larger the `strength`. The
+                Conceptually, indicates how much to transform the reference `image`. Must be between 0 and 1.
+                `image` will be used as a starting point, adding more noise to it the larger the `strength`. The
                 number of denoising steps depends on the amount of noise initially added. When `strength` is 1, added
                 noise will be maximum and the denoising process will run for the full number of iterations specified in
-                `num_inference_steps`. A value of 1, therefore, essentially ignores `init_image`.
+                `num_inference_steps`. A value of 1, therefore, essentially ignores `image`.
             num_inference_steps (`int`, *optional*, defaults to 50):
                 The number of denoising steps. More denoising steps usually lead to a higher quality image at the
                 expense of slower inference. This parameter will be modulated by `strength`.
             guidance_scale (`float`, *optional*, defaults to 7.5):
                 Guidance scale as defined in [Classifier-Free Diffusion Guidance](https://arxiv.org/abs/2207.12598).
                 `guidance_scale` is defined as `w` of equation 2. of [Imagen
                 Paper](https://arxiv.org/pdf/2205.11487.pdf). Guidance scale is enabled by setting `guidance_scale >
@@ -172,256 +357,129 @@
                 usually at the expense of lower image quality.
             negative_prompt (`str` or `List[str]`, *optional*):
                 The prompt or prompts not to guide the image generation. Ignored when not using guidance (i.e., ignored
                 if `guidance_scale` is less than `1`).
             num_images_per_prompt (`int`, *optional*, defaults to 1):
                 The number of images to generate per prompt.
             eta (`float`, *optional*, defaults to 0.0):
-                Corresponds to parameter eta (η) in the DDIM paper: https://arxiv.org/abs/2010.02502. Only applies to
+                Corresponds to parameter eta (?) in the DDIM paper: https://arxiv.org/abs/2010.02502. Only applies to
                 [`schedulers.DDIMScheduler`], will be ignored for others.
             generator (`np.random.RandomState`, *optional*):
                 A np.random.RandomState to make generation deterministic.
+            noise (`np.ndarray`, *optional*):
+                Pre-generated noise tensor, sampled from a Gaussian distribution, to be used as inputs for image
+                generation. If not provided, a noise tensor will ge generated by sampling using the supplied random
+                `generator`.
             output_type (`str`, *optional*, defaults to `"pil"`):
                 The output format of the generate image. Choose between
                 [PIL](https://pillow.readthedocs.io/en/stable/): `PIL.Image.Image` or `np.array`.
             return_dict (`bool`, *optional*, defaults to `True`):
                 Whether or not to return a [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] instead of a
                 plain tuple.
             callback (`Callable`, *optional*):
                 A function that will be called every `callback_steps` steps during inference. The function will be
                 called with the following arguments: `callback(step: int, timestep: int, latents: np.ndarray)`.
             callback_steps (`int`, *optional*, defaults to 1):
                 The frequency at which the `callback` function will be called. If not specified, the callback will be
                 called at every step.
+
         Returns:
             [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] or `tuple`:
             [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] if `return_dict` is True, otherwise a `tuple.
             When returning a tuple, the first element is a list with the generated images, and the second element is a
             list of `bool`s denoting whether the corresponding generated image likely represents "not-safe-for-work"
             (nsfw) content, according to the `safety_checker`.
         """
-        if isinstance(prompt, str):
-            batch_size = 1
-        elif isinstance(prompt, list):
-            batch_size = len(prompt)
-        else:
-            raise ValueError(
-                f"`prompt` has to be of type `str` or `list` but is {type(prompt)}"
-            )
-
-        if strength < 0 or strength > 1:
-            raise ValueError(
-                f"The value of strength should in [0.0, 1.0] but is {strength}")
-
-        if (callback_steps is None) or (callback_steps is not None and
-                                        (not isinstance(callback_steps, int)
-                                         or callback_steps <= 0)):
-            raise ValueError(
-                f"`callback_steps` has to be a positive integer but is {callback_steps} of type"
-                f" {type(callback_steps)}.")
-        if generator is None:
-            generator = np.random
-
-        # set timesteps
-        self.scheduler.set_timesteps(num_inference_steps)
-
-        if isinstance(init_image, PIL.Image.Image):
-            init_image = preprocess(init_image)
-
-        # get prompt text embeddings
-        text_inputs = self.tokenizer(
-            prompt,
-            padding="max_length",
-            max_length=self.tokenizer.model_max_length,
-            return_tensors="np",
-        )
-        text_input_ids = text_inputs.input_ids
-
-        if text_input_ids.shape[-1] > self.tokenizer.model_max_length:
-            removed_text = self.tokenizer.batch_decode(
-                text_input_ids[:, self.tokenizer.model_max_length:])
-            logger.warning(
-                "The following part of your input was truncated because CLIP can only handle sequences up to"
-                f" {self.tokenizer.model_max_length} tokens: {removed_text}")
-            text_input_ids = text_input_ids[:, :self.tokenizer.model_max_length]
-        text_embeddings = self.text_encoder(
-            input_ids=text_input_ids.astype(np.int32))[0]
-
-        # duplicate text embeddings for each generation per prompt
-        text_embeddings = np.repeat(text_embeddings,
-                                    num_images_per_prompt,
-                                    axis=0)
+        # 1. Check inputs
+        self.check_inputs(prompt, strength, callback_steps)
 
+        # 2. Define call parameters
+        batch_size = 1 if isinstance(prompt, str) else len(prompt)
         # here `guidance_scale` is defined analog to the guidance weight `w` of equation (2)
         # of the Imagen paper: https://arxiv.org/pdf/2205.11487.pdf . `guidance_scale = 1`
         # corresponds to doing no classifier free guidance.
         do_classifier_free_guidance = guidance_scale > 1.0
-        # get unconditional embeddings for classifier free guidance
-        if do_classifier_free_guidance:
-            uncond_tokens: List[str]
-            if negative_prompt is None:
-                uncond_tokens = [""]
-            elif type(prompt) is not type(negative_prompt):
-                raise TypeError(
-                    f"`negative_prompt` should be the same type to `prompt`, but got {type(negative_prompt)} !="
-                    f" {type(prompt)}.")
-            elif isinstance(negative_prompt, str):
-                uncond_tokens = [negative_prompt] * batch_size
-            elif batch_size != len(negative_prompt):
-                raise ValueError(
-                    "The length of `negative_prompt` should be equal to batch_size."
-                )
-            else:
-                uncond_tokens = negative_prompt
 
-            max_length = text_input_ids.shape[-1]
-            uncond_input = self.tokenizer(
-                uncond_tokens,
-                padding="max_length",
-                max_length=max_length,
-                truncation=True,
-                return_tensors="np",
-            )
-            uncond_input_ids = uncond_input.input_ids
-            uncond_embeddings = self.text_encoder(
-                input_ids=uncond_input_ids.astype(np.int32))[0]
-
-            # duplicate unconditional embeddings for each generation per prompt
-            uncond_embeddings = np.repeat(uncond_embeddings,
-                                          num_images_per_prompt,
-                                          axis=0)
-
-            # For classifier free guidance, we need to do two forward passes.
-            # Here we concatenate the unconditional and text embeddings into a single batch
-            # to avoid doing two forward passes
-            text_embeddings = np.concatenate(
-                [uncond_embeddings, text_embeddings])
-
-        latents_dtype = text_embeddings.dtype
-        init_image = init_image.astype(latents_dtype)
-        # encode the init image into latents and scale the latents
-        init_latents = self.vae_encoder(sample=init_image)[0]
-        init_latents = 0.18215 * init_latents
+        # 3. Encode input prompt
+        text_embeddings = self._encode_prompt(
+            prompt, num_images_per_prompt, do_classifier_free_guidance, negative_prompt
+        )
 
-        if isinstance(prompt, str):
-            prompt = [prompt]
-        if len(prompt) > init_latents.shape[0] and len(
-                prompt) % init_latents.shape[0] == 0:
-            # expand init_latents for batch_size
-            deprecation_message = (
-                f"You have passed {len(prompt)} text prompts (`prompt`), but only {init_latents.shape[0]} initial"
-                " images (`init_image`). Initial images are now duplicating to match the number of text prompts. Note"
-                " that this behavior is deprecated and will be removed in a version 1.0.0. Please make sure to update"
-                " your script to pass as many init images as text prompts to suppress this warning."
-            )
-            deprecate("len(prompt) != len(init_image)",
-                      "1.0.0",
-                      deprecation_message,
-                      standard_warn=False)
-            additional_image_per_prompt = len(prompt) // init_latents.shape[0]
-            init_latents = np.concatenate([init_latents] *
-                                          additional_image_per_prompt *
-                                          num_images_per_prompt,
-                                          axis=0)
-        elif len(prompt) > init_latents.shape[0] and len(
-                prompt) % init_latents.shape[0] != 0:
-            raise ValueError(
-                f"Cannot duplicate `init_image` of batch size {init_latents.shape[0]} to {len(prompt)} text prompts."
-            )
-        else:
-            init_latents = np.concatenate([init_latents] *
-                                          num_images_per_prompt,
-                                          axis=0)
+        # 4. Preprocess image and mask
+        if isinstance(image, PIL.Image.Image):
+            image = preprocess_image(image)
 
-        # get the original timestep using init_timestep
-        offset = self.scheduler.config.get("steps_offset", 0)
-        init_timestep = int(num_inference_steps * strength) + offset
-        init_timestep = min(init_timestep, num_inference_steps)
+        if isinstance(mask_image, PIL.Image.Image):
+            mask_image = preprocess_mask(mask_image)
 
-        timesteps = self.scheduler.timesteps.numpy()[-init_timestep]
-        timesteps = np.array([timesteps] * batch_size * num_images_per_prompt,
-                             dtype="int64")
+        # 5. set timesteps
+        self.scheduler.set_timesteps(num_inference_steps)
+        timesteps, num_inference_steps = self.get_timesteps(num_inference_steps, strength)
+        latent_timestep = timesteps[:1].repeat(batch_size * num_images_per_prompt)
 
-        # add noise to latents using the timesteps
-        noise = generator.randn(*init_latents.shape).astype(latents_dtype)
-        init_latents = self.scheduler.add_noise(paddle.to_tensor(init_latents),
-                                                paddle.to_tensor(noise),
-                                                paddle.to_tensor(timesteps))
-        init_latents = init_latents.numpy()
+        # 6. Prepare latent variables
+        # encode the init image into latents and scale the latents
+        latents, init_latents_orig, noise = self.prepare_latents(
+            image, latent_timestep, batch_size, num_images_per_prompt, text_embeddings.dtype, generator, noise
+        )
 
-        # prepare extra kwargs for the scheduler step, since not all schedulers have the same signature
-        # eta (η) is only used with the DDIMScheduler, it will be ignored for other schedulers.
-        # eta corresponds to η in DDIM paper: https://arxiv.org/abs/2010.02502
-        # and should be between [0, 1]
-        accepts_eta = "eta" in set(
-            inspect.signature(self.scheduler.step).parameters.keys())
-        extra_step_kwargs = {}
-        if accepts_eta:
-            extra_step_kwargs["eta"] = eta
+        # 7. Prepare mask latent
+        mask = mask_image.astype(latents.dtype)
+        mask = np.concatenate([mask] * batch_size * num_images_per_prompt)
+
+        # 8. Prepare extra step kwargs.
+        extra_step_kwargs = self.prepare_extra_step_kwargs(eta)
+
+        # 9. Denoising loop
+        num_warmup_steps = len(timesteps) - num_inference_steps * self.scheduler.order
+        with self.progress_bar(total=num_inference_steps) as progress_bar:
+            for i, t in enumerate(timesteps):
+                tensor_t = paddle.to_tensor(t)
+                # expand the latents if we are doing classifier free guidance
+                latent_model_input = np.concatenate([latents] * 2) if do_classifier_free_guidance else latents
+                latent_model_input = self.scheduler.scale_model_input(paddle.to_tensor(latent_model_input), tensor_t)
+                latent_model_input = latent_model_input.numpy()
+
+                # predict the noise residual
+                noise_pred = self.unet(
+                    sample=latent_model_input.astype(np.float32),
+                    timestep=np.array([t], dtype=np.int64),
+                    encoder_hidden_states=text_embeddings.astype(np.float32),
+                )[0]
+
+                # perform guidance
+                if do_classifier_free_guidance:
+                    noise_pred_uncond, noise_pred_text = np.split(noise_pred, 2)
+                    noise_pred = noise_pred_uncond + guidance_scale * (noise_pred_text - noise_pred_uncond)
+
+                # compute the previous noisy sample x_t -> x_t-1
+                scheduler_output = self.scheduler.step(
+                    paddle.to_tensor(noise_pred), tensor_t, paddle.to_tensor(latents), **extra_step_kwargs
+                )
+                latents = scheduler_output.prev_sample.numpy()
 
-        latents = init_latents
+                init_latents_proper = self.scheduler.add_noise(init_latents_orig, noise, tensor_t)
 
-        t_start = max(num_inference_steps - init_timestep + offset, 0)
+                init_latents_proper = init_latents_proper.numpy()
 
-        timesteps = self.scheduler.timesteps[t_start:].numpy()
+                latents = (init_latents_proper * mask) + (latents * (1 - mask))
 
-        for i, t in enumerate(self.progress_bar(timesteps)):
-            # expand the latents if we are doing classifier free guidance
-            latent_model_input = np.concatenate(
-                [latents] * 2) if do_classifier_free_guidance else latents
-            latent_model_input = self.scheduler.scale_model_input(
-                latent_model_input, t)
-
-            # predict the noise residual
-            noise_pred = self.unet(sample=latent_model_input,
-                                   timestep=np.array([t]),
-                                   encoder_hidden_states=text_embeddings)[0]
-
-            # perform guidance
-            if do_classifier_free_guidance:
-                noise_pred_uncond, noise_pred_text = np.split(noise_pred, 2)
-                noise_pred = noise_pred_uncond + guidance_scale * (
-                    noise_pred_text - noise_pred_uncond)
-
-            # compute the previous noisy sample x_t -> x_t-1
-            latents = self.scheduler.step(noise_pred, t, latents,
-                                          **extra_step_kwargs).prev_sample
-            latents = latents.numpy()
-
-            # call the callback, if provided
-            if callback is not None and i % callback_steps == 0:
-                callback(i, t, latents)
+                # call the callback, if provided
+                if i == len(timesteps) - 1 or ((i + 1) > num_warmup_steps and (i + 1) % self.scheduler.order == 0):
+                    progress_bar.update()
+                    if callback is not None and i % callback_steps == 0:
+                        callback(i, t, latents)
 
-        latents = 1 / 0.18215 * latents
-        # image = self.vae_decoder(latent_sample=latents)[0]
-        # it seems likes there is a strange result for using half-precision vae decoder if batchsize>1
-        image = np.concatenate([
-            self.vae_decoder(latent_sample=latents[i:i + 1])[0]
-            for i in range(latents.shape[0])
-        ])
-        image = np.clip(image / 2 + 0.5, 0, 1)
-        image = image.transpose((0, 2, 3, 1))
+        # 10. Post-processing
+        image = self.decode_latents(latents)
 
-        if self.safety_checker is not None:
-            safety_checker_input = self.feature_extractor(
-                self.numpy_to_pil(image),
-                return_tensors="np").pixel_values.astype(image.dtype)
-            # There will throw an error if use safety_checker batchsize>1
-            images, has_nsfw_concept = [], []
-            for i in range(image.shape[0]):
-                image_i, has_nsfw_concept_i = self.safety_checker(
-                    clip_input=safety_checker_input[i:i + 1],
-                    images=image[i:i + 1])
-                images.append(image_i)
-                has_nsfw_concept.append(has_nsfw_concept_i[0])
-            image = np.concatenate(images)
-        else:
-            has_nsfw_concept = None
+        # 11. Run safety checker
+        image, has_nsfw_concept = self.run_safety_checker(image, text_embeddings.dtype)
 
+        # 12. Convert to PIL
         if output_type == "pil":
             image = self.numpy_to_pil(image)
 
         if not return_dict:
             return (image, has_nsfw_concept)
 
-        return StableDiffusionPipelineOutput(
-            images=image, nsfw_content_detected=has_nsfw_concept)
+        return StableDiffusionPipelineOutput(images=image, nsfw_content_detected=has_nsfw_concept)
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/pipelines/stable_diffusion/pipeline_onnx_stable_diffusion_inpaint.py` & `ppdiffusers-0.9.0/ppdiffusers/pipelines/versatile_diffusion/pipeline_versatile_diffusion_text_to_image.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 PaddlePaddle Authors. All Rights Reserved.
+# Copyright 2022 The HuggingFace Team. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,180 +11,329 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import inspect
 from typing import Callable, List, Optional, Union
 
-import numpy as np
 import paddle
-import PIL
 
-from paddlenlp.utils.tools import compare_version
+from paddlenlp.transformers import CLIPTextModelWithProjection, CLIPTokenizer
 
-if compare_version(PIL.__version__, "9.1.0") >= 0:
-    Resampling = PIL.Image.Resampling
-else:
-    Resampling = PIL.Image
-from paddlenlp.transformers import CLIPFeatureExtractor, CLIPTokenizer
-
-from ...configuration_utils import FrozenDict
-from ...onnx_utils import OnnxRuntimeModel
-from ...pipeline_utils import DiffusionPipeline
+from ...models import AutoencoderKL, UNet2DConditionModel
+from ...models.attention import Transformer2DModel
+from ...pipeline_utils import DiffusionPipeline, ImagePipelineOutput
 from ...schedulers import DDIMScheduler, LMSDiscreteScheduler, PNDMScheduler
-from ...utils import deprecate, logging
-from . import StableDiffusionPipelineOutput
+from ...utils import logging
+from .modeling_text_unet import UNetFlatConditionModel
 
 logger = logging.get_logger(__name__)  # pylint: disable=invalid-name
 
-NUM_UNET_INPUT_CHANNELS = 9
-NUM_LATENT_CHANNELS = 4
 
-
-def prepare_mask_and_masked_image(image, mask, latents_shape):
-    image = np.array(image.convert("RGB").resize((latents_shape[1] * 8, latents_shape[0] * 8)))
-    image = image[None].transpose(0, 3, 1, 2)
-    image = image.astype(np.float32) / 127.5 - 1.0
-
-    image_mask = np.array(mask.convert("L").resize((latents_shape[1] * 8, latents_shape[0] * 8)))
-    masked_image = image * (image_mask < 127.5)
-
-    mask = mask.resize((latents_shape[1], latents_shape[0]), Resampling.NEAREST)
-    mask = np.array(mask.convert("L"))
-    mask = mask.astype(np.float32) / 255.0
-    mask = mask[None, None]
-    mask[mask < 0.5] = 0
-    mask[mask >= 0.5] = 1
-
-    return mask, masked_image
-
-
-class OnnxStableDiffusionInpaintPipeline(DiffusionPipeline):
+class VersatileDiffusionTextToImagePipeline(DiffusionPipeline):
     r"""
-    Pipeline for text-guided image inpainting using Stable Diffusion. *This is an experimental feature*.
+    Pipeline for text-to-image generation using Versatile Diffusion.
 
     This model inherits from [`DiffusionPipeline`]. Check the superclass documentation for the generic methods the
     library implements for all the pipelines (such as downloading or saving, running on a particular device, etc.)
 
     Args:
         vae ([`AutoencoderKL`]):
             Variational Auto-Encoder (VAE) Model to encode and decode images to and from latent representations.
-        text_encoder ([`CLIPTextModel`]):
-            Frozen text-encoder. Stable Diffusion uses the text portion of
-            [CLIP](https://huggingface.co/docs/transformers/model_doc/clip#transformers.CLIPTextModel), specifically
+        text_encoder ([`CLIPTextModelWithProjection`]):
+            Frozen text-encoder. Versatile Diffusion uses the text portion of
+            [CLIP](https://huggingface.co/docs/transformers/model_doc/clip#transformers.CLIPTextModelWithProjection), specifically
+            the [clip-vit-large-patch14](https://huggingface.co/openai/clip-vit-large-patch14) variant.
+        image_encoder ([`CLIPVisionModelWithProjection`]):
+            Frozen vision-encoder. Versatile Diffusion uses the vision portion of
+            [CLIP](https://huggingface.co/docs/transformers/model_doc/clip#transformers.CLIPVisionModelWithProjection), specifically
             the [clip-vit-large-patch14](https://huggingface.co/openai/clip-vit-large-patch14) variant.
         tokenizer (`CLIPTokenizer`):
             Tokenizer of class
             [CLIPTokenizer](https://huggingface.co/docs/transformers/v4.21.0/en/model_doc/clip#transformers.CLIPTokenizer).
-        unet ([`UNet2DConditionModel`]): Conditional U-Net architecture to denoise the encoded image latents.
+        image_unet ([`UNet2DConditionModel`]): Conditional U-Net architecture to denoise the encoded image latents.
+        text_unet ([`UNetFlatConditionModel`]): xxx.
         scheduler ([`SchedulerMixin`]):
-            A scheduler to be used in combination with `unet` to denoise the encoded image latens. Can be one of
+            A scheduler to be used in combination with `unet` to denoise the encoded image latents. Can be one of
             [`DDIMScheduler`], [`LMSDiscreteScheduler`], or [`PNDMScheduler`].
-        safety_checker ([`StableDiffusionSafetyChecker`]):
-            Classification module that estimates whether generated images could be considered offensive or harmful.
-            Please, refer to the [model card](https://huggingface.co/runwayml/stable-diffusion-v1-5) for details.
-        feature_extractor ([`CLIPFeatureExtractor`]):
-            Model that extracts features from generated images to be used as inputs for the `safety_checker`.
     """
-    vae_encoder: OnnxRuntimeModel
-    vae_decoder: OnnxRuntimeModel
-    text_encoder: OnnxRuntimeModel
     tokenizer: CLIPTokenizer
-    unet: OnnxRuntimeModel
+    text_encoder: CLIPTextModelWithProjection
+    image_unet: UNet2DConditionModel
+    text_unet: UNetFlatConditionModel
+    vae: AutoencoderKL
     scheduler: Union[DDIMScheduler, PNDMScheduler, LMSDiscreteScheduler]
-    safety_checker: OnnxRuntimeModel
-    feature_extractor: CLIPFeatureExtractor
+    _optional_components = ["text_unet"]
 
     def __init__(
         self,
-        vae_encoder: OnnxRuntimeModel,
-        vae_decoder: OnnxRuntimeModel,
-        text_encoder: OnnxRuntimeModel,
         tokenizer: CLIPTokenizer,
-        unet: OnnxRuntimeModel,
+        text_encoder: CLIPTextModelWithProjection,
+        image_unet: UNet2DConditionModel,
+        text_unet: UNetFlatConditionModel,
+        vae: AutoencoderKL,
         scheduler: Union[DDIMScheduler, PNDMScheduler, LMSDiscreteScheduler],
-        safety_checker: OnnxRuntimeModel,
-        feature_extractor: CLIPFeatureExtractor,
     ):
         super().__init__()
-        logger.info("`OnnxStableDiffusionInpaintPipeline` is experimental and will very likely change in the future.")
+        self.register_modules(
+            tokenizer=tokenizer,
+            text_encoder=text_encoder,
+            image_unet=image_unet,
+            text_unet=text_unet,
+            vae=vae,
+            scheduler=scheduler,
+        )
+        self.vae_scale_factor = 2 ** (len(self.vae.config.block_out_channels) - 1)
+        if self.text_unet is not None:
+            self._swap_unet_attention_blocks()
 
-        if hasattr(scheduler.config, "steps_offset") and scheduler.config.steps_offset != 1:
-            deprecation_message = (
-                f"The configuration file of this scheduler: {scheduler} is outdated. `steps_offset`"
-                f" should be set to 1 instead of {scheduler.config.steps_offset}. Please make sure "
-                "to update the config accordingly as leaving `steps_offset` might led to incorrect results"
-                " in future versions. If you have downloaded this checkpoint from the Hugging Face Hub,"
-                " it would be very nice if you could open a Pull request for the `scheduler/scheduler_config.json`"
-                " file"
-            )
-            deprecate("steps_offset!=1", "1.0.0", deprecation_message, standard_warn=False)
-            new_config = dict(scheduler.config)
-            new_config["steps_offset"] = 1
-            scheduler._internal_dict = FrozenDict(new_config)
+    def _swap_unet_attention_blocks(self):
+        """
+        Swap the `Transformer2DModel` blocks between the image and text UNets
+        """
+        for name, module in self.image_unet.named_sublayers(include_self=True):
+            if isinstance(module, Transformer2DModel):
+                parent_name, index = name.rsplit(".", 1)
+                index = int(index)
+                self.image_unet.get_sublayer(parent_name)[index], self.text_unet.get_sublayer(parent_name)[index] = (
+                    self.text_unet.get_sublayer(parent_name)[index],
+                    self.image_unet.get_sublayer(parent_name)[index],
+                )
+
+    def remove_unused_weights(self):
+        self.register_modules(text_unet=None)
+
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.enable_attention_slicing with unet->image_unet
+    def enable_attention_slicing(self, slice_size: Optional[Union[str, int]] = "auto"):
+        r"""
+        Enable sliced attention computation.
+
+        When this option is enabled, the attention module will split the input tensor in slices, to compute attention
+        in several steps. This is useful to save some memory in exchange for a small speed decrease.
+
+        Args:
+            slice_size (`str` or `int`, *optional*, defaults to `"auto"`):
+                When `"auto"`, halves the input to the attention heads, so attention will be computed in two steps. If
+                a number is provided, uses as many slices as `attention_head_dim // slice_size`. In this case,
+                `attention_head_dim` must be a multiple of `slice_size`.
+        """
+        if slice_size == "auto":
+            if isinstance(self.image_unet.config.attention_head_dim, int):
+                # half the attention head size is usually a good trade-off between
+                # speed and memory
+                slice_size = self.image_unet.config.attention_head_dim // 2
+            else:
+                # if `attention_head_dim` is a list, take the smallest head size
+                slice_size = min(self.image_unet.config.attention_head_dim)
+        self.image_unet.set_attention_slice(slice_size)
+
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.disable_attention_slicing
+    def disable_attention_slicing(self):
+        r"""
+        Disable sliced attention computation. If `enable_attention_slicing` was previously invoked, this method will go
+        back to computing attention in one step.
+        """
+        # set slice_size = `None` to disable `attention slicing`
+        self.enable_attention_slicing(None)
+
+    def _encode_text_prompt(self, prompt, num_images_per_prompt, do_classifier_free_guidance, negative_prompt):
+        r"""
+        Encodes the prompt into text encoder hidden states.
+
+        Args:
+            prompt (`str` or `list(int)`):
+                prompt to be encoded
+            num_images_per_prompt (`int`):
+                number of images that should be generated per prompt
+            do_classifier_free_guidance (`bool`):
+                whether to use classifier free guidance or not
+            negative_prompt (`str` or `List[str]`):
+                The prompt or prompts not to guide the image generation. Ignored when not using guidance (i.e., ignored
+                if `guidance_scale` is less than `1`).
+        """
+
+        def normalize_embeddings(encoder_output):
+            embeds = paddle.matmul(encoder_output.last_hidden_state, self.text_encoder.text_projection)
+            embeds_pooled = encoder_output.text_embeds
+            embeds = embeds / paddle.norm(embeds_pooled.unsqueeze(1), axis=-1, keepdim=True)
+            return embeds
+
+        batch_size = len(prompt) if isinstance(prompt, list) else 1
+
+        text_inputs = self.tokenizer(
+            prompt,
+            padding="max_length",
+            max_length=self.tokenizer.model_max_length,
+            truncation=True,
+            return_tensors="pd",
+        )
+        text_input_ids = text_inputs.input_ids
+        untruncated_ids = self.tokenizer(prompt, padding="max_length", return_tensors="pd").input_ids
 
-        if safety_checker is None:
+        if not paddle.equal_all(text_input_ids, untruncated_ids):
+            removed_text = self.tokenizer.batch_decode(untruncated_ids[:, self.tokenizer.model_max_length - 1 : -1])
             logger.warning(
-                f"You have disabled the safety checker for {self.__class__} by passing `safety_checker=None`. Ensure"
-                " that you abide to the conditions of the Stable Diffusion license and do not expose unfiltered"
-                " results in services or applications open to the public. PaddleNLP team, diffusers team and Hugging Face"
-                " strongly recommend to keep the safety filter enabled in all public facing circumstances, disabling"
-                " it only for use-cases that involve analyzing network behavior or auditing its results. For more"
-                " information, please have a look at https://github.com/huggingface/diffusers/pull/254 ."
+                "The following part of your input was truncated because CLIP can only handle sequences up to"
+                f" {self.tokenizer.model_max_length} tokens: {removed_text}"
             )
 
-        self.register_modules(
-            vae_encoder=vae_encoder,
-            vae_decoder=vae_decoder,
-            text_encoder=text_encoder,
-            tokenizer=tokenizer,
-            unet=unet,
-            scheduler=scheduler,
-            safety_checker=safety_checker,
-            feature_extractor=feature_extractor,
+        config = (
+            self.text_encoder.config
+            if isinstance(self.text_encoder.config, dict)
+            else self.text_encoder.config.to_dict()
         )
+        if config.get("use_attention_mask", None) is not None and config["use_attention_mask"]:
+            attention_mask = text_inputs.attention_mask
+        else:
+            attention_mask = None
+
+        text_embeddings = self.text_encoder(text_input_ids, attention_mask=attention_mask, return_dict=True)
+        text_embeddings = normalize_embeddings(text_embeddings)
+
+        # duplicate text embeddings for each generation per prompt, using mps friendly method
+        bs_embed, seq_len, _ = text_embeddings.shape
+        text_embeddings = text_embeddings.tile([1, num_images_per_prompt, 1])
+        text_embeddings = text_embeddings.reshape([bs_embed * num_images_per_prompt, seq_len, -1])
+
+        # get unconditional embeddings for classifier free guidance
+        if do_classifier_free_guidance:
+            uncond_tokens: List[str]
+            if negative_prompt is None:
+                uncond_tokens = [""] * batch_size
+            elif type(prompt) is not type(negative_prompt):
+                raise TypeError(
+                    f"`negative_prompt` should be the same type to `prompt`, but got {type(negative_prompt)} !="
+                    f" {type(prompt)}."
+                )
+            elif isinstance(negative_prompt, str):
+                uncond_tokens = [negative_prompt]
+            elif batch_size != len(negative_prompt):
+                raise ValueError(
+                    f"`negative_prompt`: {negative_prompt} has batch size {len(negative_prompt)}, but `prompt`:"
+                    f" {prompt} has batch size {batch_size}. Please make sure that passed `negative_prompt` matches"
+                    " the batch size of `prompt`."
+                )
+            else:
+                uncond_tokens = negative_prompt
+
+            max_length = text_input_ids.shape[-1]
+            uncond_input = self.tokenizer(
+                uncond_tokens,
+                padding="max_length",
+                max_length=max_length,
+                truncation=True,
+                return_tensors="pd",
+            )
+
+            if config.get("use_attention_mask", None) is not None and config["use_attention_mask"]:
+                attention_mask = uncond_input.attention_mask
+            else:
+                attention_mask = None
+
+            uncond_embeddings = self.text_encoder(
+                uncond_input.input_ids, attention_mask=attention_mask, return_dict=True
+            )
+            uncond_embeddings = normalize_embeddings(uncond_embeddings)
+
+            # duplicate unconditional embeddings for each generation per prompt, using mps friendly method
+            seq_len = uncond_embeddings.shape[1]
+            uncond_embeddings = uncond_embeddings.tile([1, num_images_per_prompt, 1])
+            uncond_embeddings = uncond_embeddings.reshape([batch_size * num_images_per_prompt, seq_len, -1])
+
+            # For classifier free guidance, we need to do two forward passes.
+            # Here we concatenate the unconditional and text embeddings into a single batch
+            # to avoid doing two forward passes
+            text_embeddings = paddle.concat([uncond_embeddings, text_embeddings])
+
+        return text_embeddings
+
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.decode_latents
+    def decode_latents(self, latents):
+        latents = 1 / 0.18215 * latents
+        image = self.vae.decode(latents).sample
+        image = (image / 2 + 0.5).clip(0, 1)
+        # we always cast to float32 as this does not cause significant overhead and is compatible with bfloa16
+        image = image.transpose([0, 2, 3, 1]).cast("float32").numpy()
+        return image
+
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.prepare_extra_step_kwargs
+    def prepare_extra_step_kwargs(self, generator, eta):
+        # prepare extra kwargs for the scheduler step, since not all schedulers have the same signature
+        # eta (η) is only used with the DDIMScheduler, it will be ignored for other schedulers.
+        # eta corresponds to η in DDIM paper: https://arxiv.org/abs/2010.02502
+        # and should be between [0, 1]
+
+        accepts_eta = "eta" in set(inspect.signature(self.scheduler.step).parameters.keys())
+        extra_step_kwargs = {}
+        if accepts_eta:
+            extra_step_kwargs["eta"] = eta
+
+        # check if the scheduler accepts generator
+        accepts_generator = "generator" in set(inspect.signature(self.scheduler.step).parameters.keys())
+        if accepts_generator:
+            extra_step_kwargs["generator"] = generator
+        return extra_step_kwargs
+
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.check_inputs
+    def check_inputs(self, prompt, height, width, callback_steps):
+        if not isinstance(prompt, str) and not isinstance(prompt, list):
+            raise ValueError(f"`prompt` has to be of type `str` or `list` but is {type(prompt)}")
+
+        if height % 8 != 0 or width % 8 != 0:
+            raise ValueError(f"`height` and `width` have to be divisible by 8 but are {height} and {width}.")
+
+        if (callback_steps is None) or (
+            callback_steps is not None and (not isinstance(callback_steps, int) or callback_steps <= 0)
+        ):
+            raise ValueError(
+                f"`callback_steps` has to be a positive integer but is {callback_steps} of type"
+                f" {type(callback_steps)}."
+            )
+
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.prepare_latents
+    def prepare_latents(self, batch_size, num_channels_latents, height, width, dtype, generator, latents=None):
+        shape = [batch_size, num_channels_latents, height // self.vae_scale_factor, width // self.vae_scale_factor]
+        if latents is None:
+            latents = paddle.randn(shape, generator=generator, dtype=dtype)
+        else:
+            if latents.shape != shape:
+                raise ValueError(f"Unexpected latents shape, got {latents.shape}, expected {shape}")
+
+        # scale the initial noise by the standard deviation required by the scheduler
+        latents = latents * self.scheduler.init_noise_sigma
+        return latents
 
     @paddle.no_grad()
     def __call__(
         self,
         prompt: Union[str, List[str]],
-        image: PIL.Image.Image,
-        mask_image: PIL.Image.Image,
-        height: int = 512,
-        width: int = 512,
+        height: Optional[int] = None,
+        width: Optional[int] = None,
         num_inference_steps: int = 50,
         guidance_scale: float = 7.5,
         negative_prompt: Optional[Union[str, List[str]]] = None,
         num_images_per_prompt: Optional[int] = 1,
         eta: float = 0.0,
-        generator: Optional[np.random.RandomState] = None,
-        latents: Optional[np.ndarray] = None,
+        generator: Optional[paddle.Generator] = None,
+        latents: Optional[paddle.Tensor] = None,
         output_type: Optional[str] = "pil",
         return_dict: bool = True,
-        callback: Optional[Callable[[int, int, np.ndarray], None]] = None,
+        callback: Optional[Callable[[int, int, paddle.Tensor], None]] = None,
         callback_steps: Optional[int] = 1,
         **kwargs,
     ):
         r"""
         Function invoked when calling the pipeline for generation.
 
         Args:
             prompt (`str` or `List[str]`):
                 The prompt or prompts to guide the image generation.
-            image (`PIL.Image.Image`):
-                `Image`, or tensor representing an image batch which will be inpainted, *i.e.* parts of the image will
-                be masked out with `mask_image` and repainted according to `prompt`.
-            mask_image (`PIL.Image.Image`):
-                `Image`, or tensor representing an image batch, to mask `image`. White pixels in the mask will be
-                repainted, while black pixels will be preserved. If `mask_image` is a PIL image, it will be converted
-                to a single channel (luminance) before use. If it's a tensor, it should contain one color channel (L)
-                instead of 3, so the expected shape would be `(B, H, W, 1)`.
-            height (`int`, *optional*, defaults to 512):
+            height (`int`, *optional*, defaults to self.image_unet.config.sample_size * self.vae_scale_factor):
                 The height in pixels of the generated image.
-            width (`int`, *optional*, defaults to 512):
+            width (`int`, *optional*, defaults to self.image_unet.config.sample_size * self.vae_scale_factor):
                 The width in pixels of the generated image.
             num_inference_steps (`int`, *optional*, defaults to 50):
                 The number of denoising steps. More denoising steps usually lead to a higher quality image at the
                 expense of slower inference.
             guidance_scale (`float`, *optional*, defaults to 7.5):
                 Guidance scale as defined in [Classifier-Free Diffusion Guidance](https://arxiv.org/abs/2207.12598).
                 `guidance_scale` is defined as `w` of equation 2. of [Imagen
@@ -195,234 +344,120 @@
                 The prompt or prompts not to guide the image generation. Ignored when not using guidance (i.e., ignored
                 if `guidance_scale` is less than `1`).
             num_images_per_prompt (`int`, *optional*, defaults to 1):
                 The number of images to generate per prompt.
             eta (`float`, *optional*, defaults to 0.0):
                 Corresponds to parameter eta (η) in the DDIM paper: https://arxiv.org/abs/2010.02502. Only applies to
                 [`schedulers.DDIMScheduler`], will be ignored for others.
-            generator (`np.random.RandomState`, *optional*):
-                A np.random.RandomState to make generation deterministic.
-            latents (`np.ndarray`, *optional*):
+            generator (`paddle.Generator`, *optional*):
+                A [paddle generator] to make generation
+                deterministic.
+            latents (`paddle.Tensor`, *optional*):
                 Pre-generated noisy latents, sampled from a Gaussian distribution, to be used as inputs for image
                 generation. Can be used to tweak the same generation with different prompts. If not provided, a latents
                 tensor will ge generated by sampling using the supplied random `generator`.
             output_type (`str`, *optional*, defaults to `"pil"`):
                 The output format of the generate image. Choose between
                 [PIL](https://pillow.readthedocs.io/en/stable/): `PIL.Image.Image` or `np.array`.
             return_dict (`bool`, *optional*, defaults to `True`):
                 Whether or not to return a [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] instead of a
                 plain tuple.
             callback (`Callable`, *optional*):
                 A function that will be called every `callback_steps` steps during inference. The function will be
-                called with the following arguments: `callback(step: int, timestep: int, latents: np.ndarray)`.
+                called with the following arguments: `callback(step: int, timestep: int, latents: paddle.Tensor)`.
             callback_steps (`int`, *optional*, defaults to 1):
                 The frequency at which the `callback` function will be called. If not specified, the callback will be
                 called at every step.
 
+        Examples:
+
+        ```py
+        >>> from ppdiffusers import VersatileDiffusionTextToImagePipeline
+        >>> import paddle
+
+        >>> pipe = VersatileDiffusionTextToImagePipeline.from_pretrained(
+        ...     "shi-labs/versatile-diffusion"
+        ... )
+        >>> pipe.remove_unused_weights()
+
+        >>> generator = paddle.Generator().manual_seed(0)
+        >>> image = pipe("an astronaut riding on a horse on mars", generator=generator).images[0]
+        >>> image.save("./astronaut.png")
+        ```
+
         Returns:
             [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] or `tuple`:
             [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] if `return_dict` is True, otherwise a `tuple.
             When returning a tuple, the first element is a list with the generated images, and the second element is a
             list of `bool`s denoting whether the corresponding generated image likely represents "not-safe-for-work"
             (nsfw) content, according to the `safety_checker`.
         """
-        if isinstance(prompt, str):
-            batch_size = 1
-        elif isinstance(prompt, list):
-            batch_size = len(prompt)
-        else:
-            raise ValueError(f"`prompt` has to be of type `str` or `list` but is {type(prompt)}")
-
-        if height % 8 != 0 or width % 8 != 0:
-            raise ValueError(f"`height` and `width` have to be divisible by 8 but are {height} and {width}.")
-
-        if (callback_steps is None) or (
-            callback_steps is not None and (not isinstance(callback_steps, int) or callback_steps <= 0)
-        ):
-            raise ValueError(
-                f"`callback_steps` has to be a positive integer but is {callback_steps} of type"
-                f" {type(callback_steps)}."
-            )
-
-        if generator is None:
-            generator = np.random
-
-        # set timesteps
-        self.scheduler.set_timesteps(num_inference_steps)
-
-        # get prompt text embeddings
-        text_inputs = self.tokenizer(
-            prompt,
-            padding="max_length",
-            max_length=self.tokenizer.model_max_length,
-            return_tensors="np",
-        )
-        text_input_ids = text_inputs.input_ids
+        # 0. Default height and width to unet
+        height = height or self.image_unet.config.sample_size * self.vae_scale_factor
+        width = width or self.image_unet.config.sample_size * self.vae_scale_factor
 
-        if text_input_ids.shape[-1] > self.tokenizer.model_max_length:
-            removed_text = self.tokenizer.batch_decode(text_input_ids[:, self.tokenizer.model_max_length :])
-            logger.warning(
-                "The following part of your input was truncated because CLIP can only handle sequences up to"
-                f" {self.tokenizer.model_max_length} tokens: {removed_text}"
-            )
-            text_input_ids = text_input_ids[:, : self.tokenizer.model_max_length]
-        text_embeddings = self.text_encoder(input_ids=text_input_ids.astype(np.int32))[0]
-
-        # duplicate text embeddings for each generation per prompt
-        text_embeddings = np.repeat(text_embeddings, num_images_per_prompt, axis=0)
+        # 1. Check inputs. Raise error if not correct
+        self.check_inputs(prompt, height, width, callback_steps)
 
+        # 2. Define call parameters
+        batch_size = 1 if isinstance(prompt, str) else len(prompt)
         # here `guidance_scale` is defined analog to the guidance weight `w` of equation (2)
         # of the Imagen paper: https://arxiv.org/pdf/2205.11487.pdf . `guidance_scale = 1`
         # corresponds to doing no classifier free guidance.
         do_classifier_free_guidance = guidance_scale > 1.0
-        # get unconditional embeddings for classifier free guidance
-        if do_classifier_free_guidance:
-            uncond_tokens: List[str]
-            if negative_prompt is None:
-                uncond_tokens = [""]
-            elif type(prompt) is not type(negative_prompt):
-                raise TypeError(
-                    f"`negative_prompt` should be the same type to `prompt`, but got {type(negative_prompt)} !="
-                    f" {type(prompt)}."
-                )
-            elif isinstance(negative_prompt, str):
-                uncond_tokens = [negative_prompt] * batch_size
-            elif batch_size != len(negative_prompt):
-                raise ValueError(
-                    f"`negative_prompt`: {negative_prompt} has batch size {len(negative_prompt)}, but `prompt`:"
-                    f" {prompt} has batch size {batch_size}. Please make sure that passed `negative_prompt` matches"
-                    " the batch size of `prompt`."
-                )
-            else:
-                uncond_tokens = negative_prompt
-
-            max_length = text_input_ids.shape[-1]
-            uncond_input = self.tokenizer(
-                uncond_tokens,
-                padding="max_length",
-                max_length=max_length,
-                truncation=True,
-                return_tensors="np",
-            )
-            uncond_input_ids = uncond_input.input_ids
-            uncond_embeddings = self.text_encoder(input_ids=uncond_input_ids.astype(np.int32))[0]
-
-            # duplicate unconditional embeddings for each generation per prompt
-            uncond_embeddings = np.repeat(uncond_embeddings, num_images_per_prompt, axis=0)
-
-            # For classifier free guidance, we need to do two forward passes.
-            # Here we concatenate the unconditional and text embeddings into a single batch
-            # to avoid doing two forward passes
-            text_embeddings = np.concatenate([uncond_embeddings, text_embeddings])
 
-        num_channels_latents = NUM_LATENT_CHANNELS
-        latents_shape = (batch_size * num_images_per_prompt, num_channels_latents, height // 8, width // 8)
-        latents_dtype = text_embeddings.dtype
-        if latents is None:
-            latents = generator.randn(*latents_shape).astype(latents_dtype)
-        else:
-            if latents.shape != latents_shape:
-                raise ValueError(f"Unexpected latents shape, got {latents.shape}, expected {latents_shape}")
-
-        # prepare mask and masked_image
-        mask, masked_image = prepare_mask_and_masked_image(image, mask_image, latents_shape[-2:])
-        mask = mask.astype(latents.dtype)
-        masked_image = masked_image.astype(latents.dtype)
-
-        masked_image_latents = self.vae_encoder(sample=masked_image)[0]
-        masked_image_latents = 0.18215 * masked_image_latents
-
-        # duplicate mask and masked_image_latents for each generation per prompt
-        mask = mask.repeat(batch_size * num_images_per_prompt, 0)
-        masked_image_latents = masked_image_latents.repeat(batch_size * num_images_per_prompt, 0)
-
-        mask = np.concatenate([mask] * 2) if do_classifier_free_guidance else mask
-        masked_image_latents = (
-            np.concatenate([masked_image_latents] * 2) if do_classifier_free_guidance else masked_image_latents
+        # 3. Encode input prompt
+        text_embeddings = self._encode_text_prompt(
+            prompt, num_images_per_prompt, do_classifier_free_guidance, negative_prompt
         )
 
-        num_channels_mask = mask.shape[1]
-        num_channels_masked_image = masked_image_latents.shape[1]
-
-        unet_input_channels = NUM_UNET_INPUT_CHANNELS
-        if num_channels_latents + num_channels_mask + num_channels_masked_image != unet_input_channels:
-            raise ValueError(
-                "Incorrect configuration settings! The config of `pipeline.unet` expects"
-                f" {unet_input_channels} but received `num_channels_latents`: {num_channels_latents} +"
-                f" `num_channels_mask`: {num_channels_mask} + `num_channels_masked_image`: {num_channels_masked_image}"
-                f" = {num_channels_latents+num_channels_masked_image+num_channels_mask}. Please verify the config of"
-                " `pipeline.unet` or your `mask_image` or `image` input."
-            )
-
-        # set timesteps
+        # 4. Prepare timesteps
         self.scheduler.set_timesteps(num_inference_steps)
+        timesteps = self.scheduler.timesteps
 
-        # scale the initial noise by the standard deviation required by the scheduler
-        latents = latents * self.scheduler.init_noise_sigma
+        # 5. Prepare latent variables
+        num_channels_latents = self.image_unet.in_channels
+        latents = self.prepare_latents(
+            batch_size * num_images_per_prompt,
+            num_channels_latents,
+            height,
+            width,
+            text_embeddings.dtype,
+            generator,
+            latents,
+        )
 
-        # prepare extra kwargs for the scheduler step, since not all schedulers have the same signature
-        # eta (η) is only used with the DDIMScheduler, it will be ignored for other schedulers.
-        # eta corresponds to η in DDIM paper: https://arxiv.org/abs/2010.02502
-        # and should be between [0, 1]
-        accepts_eta = "eta" in set(inspect.signature(self.scheduler.step).parameters.keys())
-        extra_step_kwargs = {}
-        if accepts_eta:
-            extra_step_kwargs["eta"] = eta
+        # 6. Prepare extra step kwargs.
+        extra_step_kwargs = self.prepare_extra_step_kwargs(generator, eta)
 
-        for i, t in enumerate(self.progress_bar(self.scheduler.timesteps)):
+        # 7. Denoising loop
+        for i, t in enumerate(self.progress_bar(timesteps)):
             # expand the latents if we are doing classifier free guidance
-            latent_model_input = np.concatenate([latents] * 2) if do_classifier_free_guidance else latents
-            # concat latents, mask, masked_image_latnets in the channel dimension
-            latent_model_input = np.concatenate([latent_model_input, mask, masked_image_latents], axis=1)
-            latent_model_input = self.scheduler.scale_model_input(paddle.to_tensor(latent_model_input), t)
-            latent_model_input = latent_model_input.numpy()
+            latent_model_input = paddle.concat([latents] * 2) if do_classifier_free_guidance else latents
+            latent_model_input = self.scheduler.scale_model_input(latent_model_input, t)
 
             # predict the noise residual
-            noise_pred = self.unet(
-                sample=latent_model_input, timestep=np.array([t]), encoder_hidden_states=text_embeddings
-            )[0]
+            noise_pred = self.image_unet(latent_model_input, t, encoder_hidden_states=text_embeddings).sample
+
             # perform guidance
             if do_classifier_free_guidance:
-                noise_pred_uncond, noise_pred_text = np.split(noise_pred, 2)
+                noise_pred_uncond, noise_pred_text = noise_pred.chunk(2)
                 noise_pred = noise_pred_uncond + guidance_scale * (noise_pred_text - noise_pred_uncond)
 
             # compute the previous noisy sample x_t -> x_t-1
             latents = self.scheduler.step(noise_pred, t, latents, **extra_step_kwargs).prev_sample
-            latents = latents.numpy()
 
             # call the callback, if provided
             if callback is not None and i % callback_steps == 0:
                 callback(i, t, latents)
 
-        latents = 1 / 0.18215 * latents
-        # image = self.vae_decoder(latent_sample=latents)[0]
-        # it seems likes there is a strange result for using half-precision vae decoder if batchsize>1
-        image = np.concatenate(
-            [self.vae_decoder(latent_sample=latents[i : i + 1])[0] for i in range(latents.shape[0])]
-        )
-
-        image = np.clip(image / 2 + 0.5, 0, 1)
-        image = image.transpose((0, 2, 3, 1))
-
-        if self.safety_checker is not None:
-            safety_checker_input = self.feature_extractor(
-                self.numpy_to_pil(image), return_tensors="np"
-            ).pixel_values.astype(image.dtype)
-            # There will throw an error if use safety_checker batchsize>1
-            images, has_nsfw_concept = [], []
-            for i in range(image.shape[0]):
-                image_i, has_nsfw_concept_i = self.safety_checker(
-                    clip_input=safety_checker_input[i : i + 1], images=image[i : i + 1]
-                )
-                images.append(image_i)
-                has_nsfw_concept.append(has_nsfw_concept_i[0])
-            image = np.concatenate(images)
-        else:
-            has_nsfw_concept = None
+        # 9. Post-processing
+        image = self.decode_latents(latents)
 
+        # 10. Convert to PIL
         if output_type == "pil":
             image = self.numpy_to_pil(image)
 
         if not return_dict:
-            return (image, has_nsfw_concept)
+            return (image,)
 
-        return StableDiffusionPipelineOutput(images=image, nsfw_content_detected=has_nsfw_concept)
+        return ImagePipelineOutput(images=image)
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/pipelines/stable_diffusion/pipeline_stable_diffusion.py` & `ppdiffusers-0.9.0/ppdiffusers/pipelines/stable_diffusion/pipeline_fastdeploy_stable_diffusion.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,164 +12,286 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import inspect
 from typing import Callable, List, Optional, Union
 
+import numpy as np
 import paddle
 
-from paddlenlp.transformers import CLIPFeatureExtractor, CLIPTextModel, CLIPTokenizer
+from paddlenlp.transformers import CLIPFeatureExtractor, CLIPTokenizer
 
-from ...configuration_utils import FrozenDict
-from ...models import AutoencoderKL, UNet2DConditionModel
+from ...fastdeploy_utils import FastDeployRuntimeModel
 from ...pipeline_utils import DiffusionPipeline
-from ...schedulers import DDIMScheduler, LMSDiscreteScheduler, PNDMScheduler, EulerAncestralDiscreteScheduler
-from ...utils import deprecate, logging
+from ...schedulers import (
+    DDIMScheduler,
+    DPMSolverMultistepScheduler,
+    EulerAncestralDiscreteScheduler,
+    EulerDiscreteScheduler,
+    LMSDiscreteScheduler,
+    PNDMScheduler,
+)
+from ...utils import logging
 from . import StableDiffusionPipelineOutput
-from .safety_checker import StableDiffusionSafetyChecker
 
-logger = logging.get_logger(__name__)  # pylint: disable=invalid-name
+logger = logging.get_logger(__name__)
 
 
-class StableDiffusionPipeline(DiffusionPipeline):
+class FastDeployStableDiffusionPipeline(DiffusionPipeline):
     r"""
     Pipeline for text-to-image generation using Stable Diffusion.
 
     This model inherits from [`DiffusionPipeline`]. Check the superclass documentation for the generic methods the
-    library implements for all the pipelines (such as downloading or saving, running on a particular device, etc.)
+    library implements for all the pipelines (such as downloading or saving etc.)
 
     Args:
-        vae ([`AutoencoderKL`]):
-            Variational Auto-Encoder (VAE) Model to encode and decode images to and from latent representations.
-        text_encoder ([`CLIPTextModel`]):
+        vae_encoder ([`FastDeployRuntimeModel`]):
+            Variational Auto-Encoder (VAE) Model to encode images to latent representations.
+        vae_decoder ([`FastDeployRuntimeModel`]):
+            Variational Auto-Encoder (VAE) Model to decode images from latent representations.
+        text_encoder ([`FastDeployRuntimeModel`]):
             Frozen text-encoder. Stable Diffusion uses the text portion of
             [CLIP](https://huggingface.co/docs/transformers/model_doc/clip#transformers.CLIPTextModel), specifically
             the [clip-vit-large-patch14](https://huggingface.co/openai/clip-vit-large-patch14) variant.
         tokenizer (`CLIPTokenizer`):
             Tokenizer of class
             [CLIPTokenizer](https://huggingface.co/docs/transformers/v4.21.0/en/model_doc/clip#transformers.CLIPTokenizer).
-        unet ([`UNet2DConditionModel`]): Conditional U-Net architecture to denoise the encoded image latents.
+        unet ([`FastDeployRuntimeModel`]): Conditional U-Net architecture to denoise the encoded image latents.
         scheduler ([`SchedulerMixin`]):
-            A scheduler to be used in combination with `unet` to denoise the encoded image latens. Can be one of
-            [`DDIMScheduler`], [`LMSDiscreteScheduler`], or [`PNDMScheduler`].
-        safety_checker ([`StableDiffusionSafetyChecker`]):
+            A scheduler to be used in combination with `unet` to denoise the encoded image latents. Can be one of
+            [`DDIMScheduler`], [`LMSDiscreteScheduler`], [`PNDMScheduler`], [`EulerDiscreteScheduler`], [`EulerAncestralDiscreteScheduler`]
+            or [`DPMSolverMultistepScheduler`].
+        safety_checker ([`FastDeployRuntimeModel`]):
             Classification module that estimates whether generated images could be considered offensive or harmful.
-            Please, refer to the [model card](https://huggingface.co/junnyu/stable-diffusion-v1-4-paddle) for details.
+            Please, refer to the [model card](https://huggingface.co/runwayml/stable-diffusion-v1-5) for details.
         feature_extractor ([`CLIPFeatureExtractor`]):
             Model that extracts features from generated images to be used as inputs for the `safety_checker`.
     """
+    _optional_components = ["vae_encoder", "safety_checker", "feature_extractor"]
 
     def __init__(
         self,
-        vae: AutoencoderKL,
-        text_encoder: CLIPTextModel,
+        vae_encoder: FastDeployRuntimeModel,
+        vae_decoder: FastDeployRuntimeModel,
+        text_encoder: FastDeployRuntimeModel,
         tokenizer: CLIPTokenizer,
-        unet: UNet2DConditionModel,
-        scheduler: Union[DDIMScheduler, PNDMScheduler, LMSDiscreteScheduler,
-                         EulerAncestralDiscreteScheduler],
-        safety_checker: StableDiffusionSafetyChecker,
+        unet: FastDeployRuntimeModel,
+        scheduler: Union[
+            DDIMScheduler,
+            PNDMScheduler,
+            LMSDiscreteScheduler,
+            EulerDiscreteScheduler,
+            EulerAncestralDiscreteScheduler,
+            DPMSolverMultistepScheduler,
+        ],
+        safety_checker: FastDeployRuntimeModel,
         feature_extractor: CLIPFeatureExtractor,
+        requires_safety_checker: bool = True,
     ):
         super().__init__()
-
-        if hasattr(scheduler.config,
-                   "steps_offset") and scheduler.config.steps_offset != 1:
-            deprecation_message = (
-                f"The configuration file of this scheduler: {scheduler} is outdated. `steps_offset`"
-                f" should be set to 1 instead of {scheduler.config.steps_offset}. Please make sure "
-                "to update the config accordingly as leaving `steps_offset` might led to incorrect results"
-                " in future versions. If you have downloaded this checkpoint from the Hugging Face Hub,"
-                " it would be very nice if you could open a Pull request for the `scheduler/scheduler_config.json`"
-                " file")
-            deprecate("steps_offset!=1",
-                      "1.0.0",
-                      deprecation_message,
-                      standard_warn=False)
-            new_config = dict(scheduler.config)
-            new_config["steps_offset"] = 1
-            scheduler._internal_dict = FrozenDict(new_config)
-
-        if safety_checker is None:
-            logger.warn(
+        if safety_checker is None and requires_safety_checker:
+            logger.warning(
                 f"You have disabled the safety checker for {self.__class__} by passing `safety_checker=None`. Ensure"
                 " that you abide to the conditions of the Stable Diffusion license and do not expose unfiltered"
                 " results in services or applications open to the public. PaddleNLP team, diffusers team and Hugging Face"
                 " strongly recommend to keep the safety filter enabled in all public facing circumstances, disabling"
                 " it only for use-cases that involve analyzing network behavior or auditing its results. For more"
                 " information, please have a look at https://github.com/huggingface/diffusers/pull/254 ."
             )
+        if safety_checker is not None and feature_extractor is None:
+            raise ValueError(
+                "Make sure to define a feature extractor when loading {self.__class__} if you want to use the safety"
+                " checker. If you do not want to use the safety checker, you can pass `'safety_checker=None'` instead."
+            )
 
         self.register_modules(
-            vae=vae,
+            vae_encoder=vae_encoder,
+            vae_decoder=vae_decoder,
             text_encoder=text_encoder,
             tokenizer=tokenizer,
             unet=unet,
             scheduler=scheduler,
             safety_checker=safety_checker,
             feature_extractor=feature_extractor,
         )
+        self.register_to_config(requires_safety_checker=requires_safety_checker)
 
-    def enable_attention_slicing(self,
-                                 slice_size: Optional[Union[str,
-                                                            int]] = "auto"):
+    def _encode_prompt(self, prompt, num_images_per_prompt, do_classifier_free_guidance, negative_prompt):
         r"""
-        Enable sliced attention computation.
-
-        When this option is enabled, the attention module will split the input tensor in slices, to compute attention
-        in several steps. This is useful to save some memory in exchange for a small speed decrease.
+        Encodes the prompt into text encoder hidden states.
 
         Args:
-            slice_size (`str` or `int`, *optional*, defaults to `"auto"`):
-                When `"auto"`, halves the input to the attention heads, so attention will be computed in two steps. If
-                a number is provided, uses as many slices as `attention_head_dim // slice_size`. In this case,
-                `attention_head_dim` must be a multiple of `slice_size`.
+            prompt (`str` or `list(int)`):
+                prompt to be encoded
+            num_images_per_prompt (`int`):
+                number of images that should be generated per prompt
+            do_classifier_free_guidance (`bool`):
+                whether to use classifier free guidance or not
+            negative_prompt (`str` or `List[str]`):
+                The prompt or prompts not to guide the image generation. Ignored when not using guidance (i.e., ignored
+                if `guidance_scale` is less than `1`).
         """
-        if slice_size == "auto":
-            # half the attention head size is usually a good trade-off between
-            # speed and memory
-            slice_size = self.unet.config.attention_head_dim // 2
-        self.unet.set_attention_slice(slice_size)
+        batch_size = len(prompt) if isinstance(prompt, list) else 1
 
-    def disable_attention_slicing(self):
-        r"""
-        Disable sliced attention computation. If `enable_attention_slicing` was previously invoked, this method will go
-        back to computing attention in one step.
-        """
-        # set slice_size = `None` to disable `attention slicing`
-        self.enable_attention_slicing(None)
+        # get prompt text embeddings
+        text_inputs = self.tokenizer(
+            prompt,
+            padding="max_length",
+            max_length=self.tokenizer.model_max_length,
+            truncation=True,
+            return_tensors="np",
+        )
+        text_input_ids = text_inputs.input_ids
+        untruncated_ids = self.tokenizer(prompt, padding="max_length", return_tensors="np").input_ids
+
+        if not np.array_equal(text_input_ids, untruncated_ids):
+            removed_text = self.tokenizer.batch_decode(untruncated_ids[:, self.tokenizer.model_max_length - 1 : -1])
+            logger.warning(
+                "The following part of your input was truncated because CLIP can only handle sequences up to"
+                f" {self.tokenizer.model_max_length} tokens: {removed_text}"
+            )
+
+        text_embeddings = self.text_encoder(input_ids=text_input_ids.astype(np.int64))[0]
+        text_embeddings = np.repeat(text_embeddings, num_images_per_prompt, axis=0)
+
+        # get unconditional embeddings for classifier free guidance
+        if do_classifier_free_guidance:
+            uncond_tokens: List[str]
+            if negative_prompt is None:
+                uncond_tokens = [""] * batch_size
+            elif type(prompt) is not type(negative_prompt):
+                raise TypeError(
+                    f"`negative_prompt` should be the same type to `prompt`, but got {type(negative_prompt)} !="
+                    f" {type(prompt)}."
+                )
+            elif isinstance(negative_prompt, str):
+                uncond_tokens = [negative_prompt] * batch_size
+            elif batch_size != len(negative_prompt):
+                raise ValueError(
+                    f"`negative_prompt`: {negative_prompt} has batch size {len(negative_prompt)}, but `prompt`:"
+                    f" {prompt} has batch size {batch_size}. Please make sure that passed `negative_prompt` matches"
+                    " the batch size of `prompt`."
+                )
+            else:
+                uncond_tokens = negative_prompt
+
+            max_length = text_input_ids.shape[-1]
+            uncond_input = self.tokenizer(
+                uncond_tokens,
+                padding="max_length",
+                max_length=max_length,
+                truncation=True,
+                return_tensors="np",
+            )
+            uncond_embeddings = self.text_encoder(input_ids=uncond_input.input_ids.astype(np.int64))[0]
+            uncond_embeddings = np.repeat(uncond_embeddings, num_images_per_prompt, axis=0)
+
+            # For classifier free guidance, we need to do two forward passes.
+            # Here we concatenate the unconditional and text embeddings into a single batch
+            # to avoid doing two forward passes
+            text_embeddings = np.concatenate([uncond_embeddings, text_embeddings])
+
+        return text_embeddings
+
+    def run_safety_checker(self, image, dtype):
+        if self.safety_checker is not None:
+            safety_checker_input = self.feature_extractor(
+                self.numpy_to_pil(image), return_tensors="np"
+            ).pixel_values.astype(dtype)
+            # There will throw an error if use safety_checker batchsize>1
+            images, has_nsfw_concept = [], []
+            for i in range(image.shape[0]):
+                image_i, has_nsfw_concept_i = self.safety_checker(
+                    clip_input=safety_checker_input[i : i + 1], images=image[i : i + 1]
+                )
+                images.append(image_i)
+                has_nsfw_concept.append(has_nsfw_concept_i[0])
+            image = np.concatenate(images)
+        else:
+            has_nsfw_concept = None
+        return image, has_nsfw_concept
+
+    def decode_latents(self, latents):
+        latents = 1 / 0.18215 * latents
+        image = np.concatenate(
+            [self.vae_decoder(latent_sample=latents[i : i + 1])[0] for i in range(latents.shape[0])]
+        )
+        image = np.clip(image / 2 + 0.5, 0, 1)
+        image = image.transpose([0, 2, 3, 1])
+        return image
+
+    def prepare_extra_step_kwargs(self, eta):
+        # prepare extra kwargs for the scheduler step, since not all schedulers have the same signature
+        # eta (η) is only used with the DDIMScheduler, it will be ignored for other schedulers.
+        # eta corresponds to η in DDIM paper: https://arxiv.org/abs/2010.02502
+        # and should be between [0, 1]
+
+        accepts_eta = "eta" in set(inspect.signature(self.scheduler.step).parameters.keys())
+        extra_step_kwargs = {}
+        if accepts_eta:
+            extra_step_kwargs["eta"] = eta
+
+        return extra_step_kwargs
+
+    def check_inputs(self, prompt, height, width, callback_steps):
+        if not isinstance(prompt, str) and not isinstance(prompt, list):
+            raise ValueError(f"`prompt` has to be of type `str` or `list` but is {type(prompt)}")
+
+        if height % 8 != 0 or width % 8 != 0:
+            raise ValueError(f"`height` and `width` have to be divisible by 8 but are {height} and {width}.")
+
+        if (callback_steps is None) or (
+            callback_steps is not None and (not isinstance(callback_steps, int) or callback_steps <= 0)
+        ):
+            raise ValueError(
+                f"`callback_steps` has to be a positive integer but is {callback_steps} of type"
+                f" {type(callback_steps)}."
+            )
+
+    def prepare_latents(self, batch_size, num_channels_latents, height, width, dtype, generator, latents=None):
+        if generator is None:
+            generator = np.random
+
+        latents_shape = (batch_size, num_channels_latents, height // 8, width // 8)
+        if latents is None:
+            latents = generator.randn(*latents_shape).astype(dtype)
+        elif latents.shape != latents_shape:
+            raise ValueError(f"Unexpected latents shape, got {latents.shape}, expected {latents_shape}")
+
+        # scale the initial noise by the standard deviation required by the scheduler
+        latents = latents * float(self.scheduler.init_noise_sigma)
+        return latents
 
-    @paddle.no_grad()
     def __call__(
         self,
         prompt: Union[str, List[str]],
-        height: int = 512,
-        width: int = 512,
-        num_inference_steps: int = 50,
-        guidance_scale: float = 7.5,
+        height: Optional[int] = 512,
+        width: Optional[int] = 512,
+        num_inference_steps: Optional[int] = 50,
+        guidance_scale: Optional[float] = 7.5,
         negative_prompt: Optional[Union[str, List[str]]] = None,
         num_images_per_prompt: Optional[int] = 1,
-        eta: float = 0.0,
-        seed: Optional[int] = None,
-        latents: Optional[paddle.Tensor] = None,
+        eta: Optional[float] = 0.0,
+        generator: Optional[np.random.RandomState] = None,
+        latents: Optional[np.ndarray] = None,
         output_type: Optional[str] = "pil",
         return_dict: bool = True,
-        callback: Optional[Callable[[int, int, paddle.Tensor], None]] = None,
+        callback: Optional[Callable[[int, int, np.ndarray], None]] = None,
         callback_steps: Optional[int] = 1,
-        **kwargs,
     ):
         r"""
         Function invoked when calling the pipeline for generation.
 
         Args:
             prompt (`str` or `List[str]`):
                 The prompt or prompts to guide the image generation.
-            height (`int`, *optional*, defaults to 512):
+            height (`int`, *optional*, 512):
                 The height in pixels of the generated image.
-            width (`int`, *optional*, defaults to 512):
+            width (`int`, *optional*, 512):
                 The width in pixels of the generated image.
             num_inference_steps (`int`, *optional*, defaults to 50):
                 The number of denoising steps. More denoising steps usually lead to a higher quality image at the
                 expense of slower inference.
             guidance_scale (`float`, *optional*, defaults to 7.5):
                 Guidance scale as defined in [Classifier-Free Diffusion Guidance](https://arxiv.org/abs/2207.12598).
                 `guidance_scale` is defined as `w` of equation 2. of [Imagen
@@ -180,222 +302,115 @@
                 The prompt or prompts not to guide the image generation. Ignored when not using guidance (i.e., ignored
                 if `guidance_scale` is less than `1`).
             num_images_per_prompt (`int`, *optional*, defaults to 1):
                 The number of images to generate per prompt.
             eta (`float`, *optional*, defaults to 0.0):
                 Corresponds to parameter eta (η) in the DDIM paper: https://arxiv.org/abs/2010.02502. Only applies to
                 [`schedulers.DDIMScheduler`], will be ignored for others.
-            seed (`int`, *optional*):
-                Random number seed.
-            latents (`paddle.Tensor`, *optional*):
+            generator (`np.random.RandomState`, *optional*):
+                A np.random.RandomState to make generation deterministic.
+            latents (`np.ndarray`, *optional*):
                 Pre-generated noisy latents, sampled from a Gaussian distribution, to be used as inputs for image
                 generation. Can be used to tweak the same generation with different prompts. If not provided, a latents
-                tensor will ge generated by sampling using the supplied random `seed`.
+                tensor will ge generated by sampling using the supplied random `generator`.
             output_type (`str`, *optional*, defaults to `"pil"`):
                 The output format of the generate image. Choose between
                 [PIL](https://pillow.readthedocs.io/en/stable/): `PIL.Image.Image` or `np.array`.
             return_dict (`bool`, *optional*, defaults to `True`):
                 Whether or not to return a [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] instead of a
                 plain tuple.
             callback (`Callable`, *optional*):
                 A function that will be called every `callback_steps` steps during inference. The function will be
-                called with the following arguments: `callback(step: int, timestep: int, latents: paddle.Tensor)`.
+                called with the following arguments: `callback(step: int, timestep: int, latents: np.ndarray)`.
             callback_steps (`int`, *optional*, defaults to 1):
                 The frequency at which the `callback` function will be called. If not specified, the callback will be
                 called at every step.
 
         Returns:
             [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] or `tuple`:
             [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] if `return_dict` is True, otherwise a `tuple.
             When returning a tuple, the first element is a list with the generated images, and the second element is a
             list of `bool`s denoting whether the corresponding generated image likely represents "not-safe-for-work"
             (nsfw) content, according to the `safety_checker`.
         """
+        # 1. Check inputs. Raise error if not correct
+        self.check_inputs(prompt, height, width, callback_steps)
 
-        if isinstance(prompt, str):
-            batch_size = 1
-        elif isinstance(prompt, list):
-            batch_size = len(prompt)
-        else:
-            raise ValueError(
-                f"`prompt` has to be of type `str` or `list` but is {type(prompt)}"
-            )
-
-        if height % 8 != 0 or width % 8 != 0:
-            raise ValueError(
-                f"`height` and `width` have to be divisible by 8 but are {height} and {width}."
-            )
-
-        if (callback_steps is None) or (callback_steps is not None and
-                                        (not isinstance(callback_steps, int)
-                                         or callback_steps <= 0)):
-            raise ValueError(
-                f"`callback_steps` has to be a positive integer but is {callback_steps} of type"
-                f" {type(callback_steps)}.")
-
-        # get prompt text embeddings
-        text_inputs = self.tokenizer(
-            prompt,
-            padding="max_length",
-            max_length=self.tokenizer.model_max_length,
-            return_tensors="pd",
-        )
-        text_input_ids = text_inputs.input_ids
-
-        if text_input_ids.shape[-1] > self.tokenizer.model_max_length:
-            removed_text = self.tokenizer.batch_decode(
-                text_input_ids[:, self.tokenizer.model_max_length:])
-            logger.warning(
-                "The following part of your input was truncated because CLIP can only handle sequences up to"
-                f" {self.tokenizer.model_max_length} tokens: {removed_text}")
-            text_input_ids = text_input_ids[:, :self.tokenizer.model_max_length]
-        attention_mask = paddle.ones_like(text_input_ids)
-        text_embeddings = self.text_encoder(text_input_ids,
-                                            attention_mask=attention_mask)[0]
-
-        # duplicate text embeddings for each generation per prompt, using mps friendly method
-        bs_embed, seq_len, _ = text_embeddings.shape
-        text_embeddings = text_embeddings.tile([1, num_images_per_prompt, 1])
-        text_embeddings = text_embeddings.reshape(
-            [bs_embed * num_images_per_prompt, seq_len, -1])
+        # 2. Define call parameters
+        batch_size = 1 if isinstance(prompt, str) else len(prompt)
 
         # here `guidance_scale` is defined analog to the guidance weight `w` of equation (2)
         # of the Imagen paper: https://arxiv.org/pdf/2205.11487.pdf . `guidance_scale = 1`
         # corresponds to doing no classifier free guidance.
         do_classifier_free_guidance = guidance_scale > 1.0
-        # get unconditional embeddings for classifier free guidance
-        if do_classifier_free_guidance:
-            uncond_tokens: List[str]
-            if negative_prompt is None:
-                uncond_tokens = [""]
-            elif type(prompt) is not type(negative_prompt):
-                raise TypeError(
-                    f"`negative_prompt` should be the same type to `prompt`, but got {type(negative_prompt)} !="
-                    f" {type(prompt)}.")
-            elif isinstance(negative_prompt, str):
-                uncond_tokens = [negative_prompt]
-            elif batch_size != len(negative_prompt):
-                raise ValueError(
-                    f"`negative_prompt`: {negative_prompt} has batch size {len(negative_prompt)}, but `prompt`:"
-                    f" {prompt} has batch size {batch_size}. Please make sure that passed `negative_prompt` matches"
-                    " the batch size of `prompt`.")
-            else:
-                uncond_tokens = negative_prompt
-
-            max_length = text_input_ids.shape[-1]
-            uncond_input = self.tokenizer(
-                uncond_tokens,
-                padding="max_length",
-                max_length=max_length,
-                truncation=True,
-                return_tensors="pd",
-            )
-            # paddlenlp's attention_mask is not like transforemrs's attention_mask
-            attention_mask = paddle.ones_like(uncond_input.input_ids)
-            uncond_embeddings = self.text_encoder(
-                uncond_input.input_ids, attention_mask=attention_mask)[0]
-
-            # duplicate unconditional embeddings for each generation per prompt, using mps friendly method
-            seq_len = uncond_embeddings.shape[1]
-            uncond_embeddings = uncond_embeddings.tile(
-                [batch_size, num_images_per_prompt, 1])
-            uncond_embeddings = uncond_embeddings.reshape(
-                [batch_size * num_images_per_prompt, seq_len, -1])
 
-            # For classifier free guidance, we need to do two forward passes.
-            # Here we concatenate the unconditional and text embeddings into a single batch
-            # to avoid doing two forward passes
-            text_embeddings = paddle.concat(
-                [uncond_embeddings, text_embeddings])
-
-        # get the initial random noise unless the user supplied it
-
-        # Unlike in other pipelines, latents need to be generated in the target device
-        # for 1-to-1 results reproducibility with the CompVis implementation.
-        # However this currently doesn't work in `mps`.
-        latents_shape = [
-            batch_size * num_images_per_prompt, self.unet.in_channels,
-            height // 8, width // 8
-        ]
-        if latents is None:
-            if seed is not None:
-                paddle.seed(seed)
-
-            latents = paddle.randn(latents_shape, dtype=text_embeddings.dtype)
-        else:
-            if latents.shape != latents_shape:
-                raise ValueError(
-                    f"Unexpected latents shape, got {latents.shape}, expected {latents_shape}"
-                )
+        # 3. Encode input prompt
+        text_embeddings = self._encode_prompt(
+            prompt, num_images_per_prompt, do_classifier_free_guidance, negative_prompt
+        )
 
-        # set timesteps
+        # 4. Prepare timesteps
         self.scheduler.set_timesteps(num_inference_steps)
+        timesteps = self.scheduler.timesteps.numpy()
 
-        # Some schedulers like PNDM have timesteps as arrays
-        # It's more optimized to move all timesteps to correct device beforehand
-        timesteps_tensor = self.scheduler.timesteps
-
-        # scale the initial noise by the standard deviation required by the scheduler
-        latents = latents * self.scheduler.init_noise_sigma
-
-        # prepare extra kwargs for the scheduler step, since not all schedulers have the same signature
-        # eta (η) is only used with the DDIMScheduler, it will be ignored for other schedulers.
-        # eta corresponds to η in DDIM paper: https://arxiv.org/abs/2010.02502
-        # and should be between [0, 1]
-        accepts_eta = "eta" in set(
-            inspect.signature(self.scheduler.step).parameters.keys())
-        extra_step_kwargs = {}
-        if accepts_eta:
-            extra_step_kwargs["eta"] = eta
-
-        for i, t in enumerate(self.progress_bar(timesteps_tensor)):
-            # expand the latents if we are doing classifier free guidance
-            latent_model_input = paddle.concat(
-                [latents] * 2) if do_classifier_free_guidance else latents
-            latent_model_input = self.scheduler.scale_model_input(
-                latent_model_input, t)
-
-            # predict the noise residual
-            noise_pred = self.unet(latent_model_input,
-                                   t,
-                                   encoder_hidden_states=text_embeddings).sample
-
-            # perform guidance
-            if do_classifier_free_guidance:
-                noise_pred_uncond, noise_pred_text = noise_pred.chunk(2)
-                noise_pred = noise_pred_uncond + guidance_scale * (
-                    noise_pred_text - noise_pred_uncond)
-
-            # compute the previous noisy sample x_t -> x_t-1
-            latents = self.scheduler.step(noise_pred, t, latents,
-                                          **extra_step_kwargs).prev_sample
-
-            # call the callback, if provided
-            if callback is not None and i % callback_steps == 0:
-                callback(i, t, latents)
+        # 5. Prepare latent variables
+        num_channels_latents = 4
+        latents = self.prepare_latents(
+            batch_size * num_images_per_prompt,
+            num_channels_latents,
+            height,
+            width,
+            text_embeddings.dtype,
+            generator,
+            latents,
+        )
+        # 6. Prepare extra step kwargs.
+        extra_step_kwargs = self.prepare_extra_step_kwargs(eta)
 
-        latents = 1 / 0.18215 * latents
-        image = self.vae.decode(latents).sample
+        # 7. Denoising loop
+        num_warmup_steps = len(timesteps) - num_inference_steps * self.scheduler.order
+        with self.progress_bar(total=num_inference_steps) as progress_bar:
+            for i, t in enumerate(timesteps):
+                tensor_t = paddle.to_tensor(t)
+                # expand the latents if we are doing classifier free guidance
+                latent_model_input = np.concatenate([latents] * 2) if do_classifier_free_guidance else latents
+                latent_model_input = self.scheduler.scale_model_input(paddle.to_tensor(latent_model_input), tensor_t)
+                latent_model_input = latent_model_input.numpy()
+
+                # predict the noise residual
+                noise_pred = self.unet(
+                    sample=latent_model_input.astype(np.float32),
+                    timestep=np.array([t], dtype=np.int64),
+                    encoder_hidden_states=text_embeddings.astype(np.float32),
+                )[0]
+
+                # perform guidance
+                if do_classifier_free_guidance:
+                    noise_pred_uncond, noise_pred_text = np.split(noise_pred, 2)
+                    noise_pred = noise_pred_uncond + guidance_scale * (noise_pred_text - noise_pred_uncond)
+
+                # compute the previous noisy sample x_t -> x_t-1
+                scheduler_output = self.scheduler.step(
+                    paddle.to_tensor(noise_pred), tensor_t, paddle.to_tensor(latents), **extra_step_kwargs
+                )
+                latents = scheduler_output.prev_sample.numpy()
 
-        image = (image / 2 + 0.5).clip(0, 1)
+                # call the callback, if provided
+                if i == len(timesteps) - 1 or ((i + 1) > num_warmup_steps and (i + 1) % self.scheduler.order == 0):
+                    progress_bar.update()
+                    if callback is not None and i % callback_steps == 0:
+                        callback(i, t, latents)
 
-        # we always cast to float32 as this does not cause significant overhead and is compatible with bfloa16
-        image = image.transpose([0, 2, 3, 1]).astype("float32").numpy()
+        # 8. Post-processing
+        image = self.decode_latents(latents)
 
-        if self.safety_checker is not None:
-            safety_checker_input = self.feature_extractor(
-                self.numpy_to_pil(image), return_tensors="pd")
-            image, has_nsfw_concept = self.safety_checker(
-                images=image,
-                clip_input=safety_checker_input.pixel_values.astype(
-                    text_embeddings.dtype))
-        else:
-            has_nsfw_concept = None
+        # 9. Run safety checker
+        image, has_nsfw_concept = self.run_safety_checker(image, text_embeddings.dtype)
 
+        # 10. Convert to PIL
         if output_type == "pil":
             image = self.numpy_to_pil(image)
 
         if not return_dict:
             return (image, has_nsfw_concept)
 
-        return StableDiffusionPipelineOutput(
-            images=image, nsfw_content_detected=has_nsfw_concept)
+        return StableDiffusionPipelineOutput(images=image, nsfw_content_detected=has_nsfw_concept)
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_all_in_one.py` & `ppdiffusers-0.9.0/ppdiffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_all_in_one.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,44 +10,46 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import inspect
+import os
+import random
+import re
+import time
 from typing import Callable, List, Optional, Union
 
-import random
+import numpy as np
 import paddle
 import PIL
 import PIL.Image
-import numpy as np
-import re
-import inspect
-import os
-import time
+from packaging import version
 
 from paddlenlp.transformers import CLIPFeatureExtractor, CLIPTextModel, CLIPTokenizer
+
 from ...configuration_utils import FrozenDict
 from ...models import AutoencoderKL, UNet2DConditionModel
 from ...pipeline_utils import DiffusionPipeline
-from ...schedulers import DDIMScheduler, LMSDiscreteScheduler, PNDMScheduler, EulerAncestralDiscreteScheduler
-from ...utils import deprecate, logging
+from ...schedulers import (
+    DDIMScheduler,
+    DPMSolverMultistepScheduler,
+    EulerAncestralDiscreteScheduler,
+    EulerDiscreteScheduler,
+    LMSDiscreteScheduler,
+    PNDMScheduler,
+)
+from ...utils import PIL_INTERPOLATION, deprecate, logging
+from ...utils.testing_utils import load_image
 from . import StableDiffusionPipelineOutput
 from .safety_checker import StableDiffusionSafetyChecker
-from ...utils.testing_utils import load_image
 
 logger = logging.get_logger(__name__)  # pylint: disable=invalid-name
 
-from paddlenlp.utils.tools import compare_version
-if compare_version(PIL.__version__, "9.1.0") >= 0:
-    Resampling = PIL.Image.Resampling
-else:
-    Resampling = PIL.Image
-
 
 def save_all(images, FORMAT="jpg", OUTDIR="./outputs/"):
     if not isinstance(images, (list, tuple)):
         images = [images]
     for image in images:
         PRECISION = "fp32"
         argument = image.argument
@@ -58,20 +60,20 @@
         HEIGHT = argument["height"]
         WIDTH = argument["width"]
         SEED = argument["seed"]
         STRENGTH = argument.get("strength", 1)
         INFERENCE_STEPS = argument["num_inference_steps"]
         GUIDANCE_SCALE = argument["guidance_scale"]
 
-        filename = f'{str(epoch_time)}_scale_{GUIDANCE_SCALE}_steps_{INFERENCE_STEPS}_seed_{SEED}.{FORMAT}'
-        filedir = f'{OUTDIR}/{filename}'
+        filename = f"{str(epoch_time)}_scale_{GUIDANCE_SCALE}_steps_{INFERENCE_STEPS}_seed_{SEED}.{FORMAT}"
+        filedir = f"{OUTDIR}/{filename}"
         image.save(filedir)
-        with open(f'{OUTDIR}/{epoch_time}_prompt.txt', 'w') as file:
+        with open(f"{OUTDIR}/{epoch_time}_prompt.txt", "w") as file:
             file.write(
-                f'PROMPT: {PROMPT}\nNEG_PROMPT: {NEGPROMPT}\n\nINFERENCE_STEPS: {INFERENCE_STEPS}\nHeight: {HEIGHT}\nWidth: {WIDTH}\nSeed: {SEED}\n\nPrecision: {PRECISION}\nSTRENGTH: {STRENGTH}\nGUIDANCE_SCALE: {GUIDANCE_SCALE}'
+                f"PROMPT: {PROMPT}\nNEG_PROMPT: {NEGPROMPT}\n\nINFERENCE_STEPS: {INFERENCE_STEPS}\nHeight: {HEIGHT}\nWidth: {WIDTH}\nSeed: {SEED}\n\nPrecision: {PRECISION}\nSTRENGTH: {STRENGTH}\nGUIDANCE_SCALE: {GUIDANCE_SCALE}"
             )
 
 
 re_attention = re.compile(
     r"""
 \\\(|
 \\\)|
@@ -82,15 +84,17 @@
 \(|
 \[|
 :([+-]?[.\d]+)\)|
 \)|
 ]|
 [^\\()\[\]:]+|
 :
-""", re.X)
+""",
+    re.X,
+)
 
 
 def parse_prompt_attention(text):
     """
     Parses a string with attention tokens and returns a list of pairs: text and its associated weight.
     Accepted tokens are:
       (abc) - increases attention to abc by a multiplier of 1.1
@@ -135,25 +139,25 @@
         for p in range(start_position, len(res)):
             res[p][1] *= multiplier
 
     for m in re_attention.finditer(text):
         text = m.group(0)
         weight = m.group(1)
 
-        if text.startswith('\\'):
+        if text.startswith("\\"):
             res.append([text[1:], 1.0])
-        elif text == '(':
+        elif text == "(":
             round_brackets.append(len(res))
-        elif text == '[':
+        elif text == "[":
             square_brackets.append(len(res))
         elif weight is not None and len(round_brackets) > 0:
             multiply_range(round_brackets.pop(), float(weight))
-        elif text == ')' and len(round_brackets) > 0:
+        elif text == ")" and len(round_brackets) > 0:
             multiply_range(round_brackets.pop(), round_bracket_multiplier)
-        elif text == ']' and len(square_brackets) > 0:
+        elif text == "]" and len(square_brackets) > 0:
             multiply_range(square_brackets.pop(), square_bracket_multiplier)
         else:
             res.append([text, 1.0])
 
     for pos in round_brackets:
         multiply_range(pos, round_bracket_multiplier)
 
@@ -171,16 +175,15 @@
             res.pop(i + 1)
         else:
             i += 1
 
     return res
 
 
-def get_prompts_with_weights(pipe: DiffusionPipeline, prompt: List[str],
-                             max_length: int):
+def get_prompts_with_weights(pipe: DiffusionPipeline, prompt: List[str], max_length: int):
     r"""
     Tokenize a list of prompts and return its tokens with weights of each token.
 
     No padding, starting or ending token is included.
     """
     tokens = []
     weights = []
@@ -206,75 +209,59 @@
             text_weight = text_weight[:max_length]
 
         tokens.append(text_token)
         weights.append(text_weight)
     return tokens, weights
 
 
-def pad_tokens_and_weights(tokens,
-                           weights,
-                           max_length,
-                           bos,
-                           eos,
-                           pad,
-                           no_boseos_middle=True,
-                           chunk_length=77):
+def pad_tokens_and_weights(tokens, weights, max_length, bos, eos, pad, no_boseos_middle=True, chunk_length=77):
     r"""
     Pad the tokens (with starting and ending tokens) and weights (with 1.0) to max_length.
     """
     max_embeddings_multiples = (max_length - 2) // (chunk_length - 2)
     weights_length = max_length if no_boseos_middle else max_embeddings_multiples * chunk_length
     for i in range(len(tokens)):
-        tokens[i] = [bos] + tokens[i] + [
-            eos
-        ] + [pad] * (max_length - 2 - len(tokens[i]))
+        tokens[i] = [bos] + tokens[i] + [eos] + [pad] * (max_length - 2 - len(tokens[i]))
         if no_boseos_middle:
-            weights[i] = [
-                1.
-            ] + weights[i] + [1.] * (max_length - 1 - len(weights[i]))
+            weights[i] = [1.0] + weights[i] + [1.0] * (max_length - 1 - len(weights[i]))
         else:
             w = []
             if len(weights[i]) == 0:
-                w = [1.] * weights_length
+                w = [1.0] * weights_length
             else:
                 for j in range((len(weights[i]) - 1) // chunk_length + 1):
-                    w.append(1.)  # weight for starting token in this chunk
-                    w += weights[i][j *
-                                    chunk_length:min(len(weights[i]), (j + 1) *
-                                                     chunk_length)]
-                    w.append(1.)  # weight for ending token in this chunk
-                w += [1.] * (weights_length - len(w))
+                    w.append(1.0)  # weight for starting token in this chunk
+                    w += weights[i][j * chunk_length : min(len(weights[i]), (j + 1) * chunk_length)]
+                    w.append(1.0)  # weight for ending token in this chunk
+                w += [1.0] * (weights_length - len(w))
             weights[i] = w[:]
 
     return tokens, weights
 
 
-def get_unweighted_text_embeddings(pipe: DiffusionPipeline,
-                                   text_input: paddle.Tensor,
-                                   chunk_length: int,
-                                   no_boseos_middle: Optional[bool] = True):
+def get_unweighted_text_embeddings(
+    pipe: DiffusionPipeline, text_input: paddle.Tensor, chunk_length: int, no_boseos_middle: Optional[bool] = True
+):
     """
     When the length of tokens is a multiple of the capacity of the text encoder,
     it should be split into chunks and sent to the text encoder individually.
     """
     max_embeddings_multiples = (text_input.shape[1] - 2) // (chunk_length - 2)
     if max_embeddings_multiples > 1:
         text_embeddings = []
         for i in range(max_embeddings_multiples):
             # extract the i-th chunk
-            text_input_chunk = text_input[:, i * (chunk_length - 2):(i + 1) *
-                                          (chunk_length - 2) + 2].clone()
+            text_input_chunk = text_input[:, i * (chunk_length - 2) : (i + 1) * (chunk_length - 2) + 2].clone()
 
             # cover the head and the tail by the starting and the ending tokens
             text_input_chunk[:, 0] = text_input[0, 0]
             text_input_chunk[:, -1] = text_input[0, -1]
 
             attention_mask = paddle.ones_like(text_input_chunk)
-            text_embedding = pipe.text_encoder(text_input_chunk,
-                                               attention_mask=attention_mask)[0]
+            text_embedding = pipe.text_encoder(text_input_chunk, attention_mask=attention_mask)[0]
 
             if no_boseos_middle:
                 if i == 0:
                     # discard the ending token
                     text_embedding = text_embedding[:, :-1]
                 elif i == max_embeddings_multiples - 1:
                     # discard the starting token
@@ -283,280 +270,313 @@
                     # discard both starting and ending tokens
                     text_embedding = text_embedding[:, 1:-1]
 
             text_embeddings.append(text_embedding)
         text_embeddings = paddle.concat(text_embeddings, axis=1)
     else:
         attention_mask = paddle.ones_like(text_input)
-        text_embeddings = pipe.text_encoder(text_input,
-                                            attention_mask=attention_mask)[0]
+        text_embeddings = pipe.text_encoder(text_input, attention_mask=attention_mask)[0]
     return text_embeddings
 
 
 def get_weighted_text_embeddings(
-        pipe: DiffusionPipeline,
-        prompt: Union[str, List[str]],
-        uncond_prompt: Optional[Union[str, List[str]]] = None,
-        max_embeddings_multiples: Optional[int] = 1,
-        no_boseos_middle: Optional[bool] = False,
-        skip_parsing: Optional[bool] = False,
-        skip_weighting: Optional[bool] = False,
-        **kwargs):
+    pipe: DiffusionPipeline,
+    prompt: Union[str, List[str]],
+    uncond_prompt: Optional[Union[str, List[str]]] = None,
+    max_embeddings_multiples: Optional[int] = 1,
+    no_boseos_middle: Optional[bool] = False,
+    skip_parsing: Optional[bool] = False,
+    skip_weighting: Optional[bool] = False,
+    **kwargs
+):
     r"""
-    Prompts can be assigned with local weights using brackets. For example, 
+    Prompts can be assigned with local weights using brackets. For example,
     prompt 'A (very beautiful) masterpiece' highlights the words 'very beautiful',
     and the embedding tokens corresponding to the words get multiplied by a constant, 1.1.
-    
+
     Also, to regularize of the embedding, the weighted embedding would be scaled to preserve the original mean.
 
     Args:
         pipe (`DiffusionPipeline`):
             Pipe to provide access to the tokenizer and the text encoder.
         prompt (`str` or `List[str]`):
             The prompt or prompts to guide the image generation.
         uncond_prompt (`str` or `List[str]`):
             The unconditional prompt or prompts for guide the image generation. If unconditional prompt
             is provided, the embeddings of prompt and uncond_prompt are concatenated.
         max_embeddings_multiples (`int`, *optional*, defaults to `1`):
             The max multiple length of prompt embeddings compared to the max output length of text encoder.
         no_boseos_middle (`bool`, *optional*, defaults to `False`):
-            If the length of text token is multiples of the capacity of text encoder, whether reserve the starting and 
+            If the length of text token is multiples of the capacity of text encoder, whether reserve the starting and
             ending token in each of the chunk in the middle.
         skip_parsing (`bool`, *optional*, defaults to `False`):
             Skip the parsing of brackets.
         skip_weighting (`bool`, *optional*, defaults to `False`):
             Skip the weighting. When the parsing is skipped, it is forced True.
     """
-    max_length = (pipe.tokenizer.model_max_length -
-                  2) * max_embeddings_multiples + 2
+    max_length = (pipe.tokenizer.model_max_length - 2) * max_embeddings_multiples + 2
     if isinstance(prompt, str):
         prompt = [prompt]
 
     if not skip_parsing:
-        prompt_tokens, prompt_weights = get_prompts_with_weights(
-            pipe, prompt, max_length - 2)
+        prompt_tokens, prompt_weights = get_prompts_with_weights(pipe, prompt, max_length - 2)
         if uncond_prompt is not None:
             if isinstance(uncond_prompt, str):
                 uncond_prompt = [uncond_prompt]
-            uncond_tokens, uncond_weights = get_prompts_with_weights(
-                pipe, uncond_prompt, max_length - 2)
+            uncond_tokens, uncond_weights = get_prompts_with_weights(pipe, uncond_prompt, max_length - 2)
     else:
         prompt_tokens = [
-            token[1:-1] for token in pipe.tokenizer(
-                prompt, max_length=max_length, truncation=True).input_ids
+            token[1:-1] for token in pipe.tokenizer(prompt, max_length=max_length, truncation=True).input_ids
         ]
-        prompt_weights = [[1.] * len(token) for token in prompt_tokens]
+        prompt_weights = [[1.0] * len(token) for token in prompt_tokens]
         if uncond_prompt is not None:
             if isinstance(uncond_prompt, str):
                 uncond_prompt = [uncond_prompt]
             uncond_tokens = [
                 token[1:-1]
-                for token in pipe.tokenizer(uncond_prompt,
-                                            max_length=max_length,
-                                            truncation=True).input_ids
+                for token in pipe.tokenizer(uncond_prompt, max_length=max_length, truncation=True).input_ids
             ]
-            uncond_weights = [[1.] * len(token) for token in uncond_tokens]
+            uncond_weights = [[1.0] * len(token) for token in uncond_tokens]
 
     # round up the longest length of tokens to a multiple of (model_max_length - 2)
     max_length = max([len(token) for token in prompt_tokens])
     if uncond_prompt is not None:
-        max_length = max(max_length,
-                         max([len(token) for token in uncond_tokens]))
+        max_length = max(max_length, max([len(token) for token in uncond_tokens]))
 
-    max_embeddings_multiples = min(max_embeddings_multiples, (max_length - 1) //
-                                   (pipe.tokenizer.model_max_length - 2) + 1)
+    max_embeddings_multiples = min(
+        max_embeddings_multiples, (max_length - 1) // (pipe.tokenizer.model_max_length - 2) + 1
+    )
     max_embeddings_multiples = max(1, max_embeddings_multiples)
-    max_length = (pipe.tokenizer.model_max_length -
-                  2) * max_embeddings_multiples + 2
+    max_length = (pipe.tokenizer.model_max_length - 2) * max_embeddings_multiples + 2
 
     # pad the length of tokens and weights
     # support bert tokenizer
     bos = pipe.tokenizer.bos_token_id if pipe.tokenizer.bos_token_id is not None else pipe.tokenizer.cls_token_id
     eos = pipe.tokenizer.eos_token_id if pipe.tokenizer.eos_token_id is not None else pipe.tokenizer.sep_token_id
     pad = pipe.tokenizer.pad_token_id
     prompt_tokens, prompt_weights = pad_tokens_and_weights(
         prompt_tokens,
         prompt_weights,
         max_length,
         bos,
         eos,
         pad,
         no_boseos_middle=no_boseos_middle,
-        chunk_length=pipe.tokenizer.model_max_length)
+        chunk_length=pipe.tokenizer.model_max_length,
+    )
     prompt_tokens = paddle.to_tensor(prompt_tokens)
     if uncond_prompt is not None:
         uncond_tokens, uncond_weights = pad_tokens_and_weights(
             uncond_tokens,
             uncond_weights,
             max_length,
             bos,
             eos,
             pad,
             no_boseos_middle=no_boseos_middle,
-            chunk_length=pipe.tokenizer.model_max_length)
+            chunk_length=pipe.tokenizer.model_max_length,
+        )
         uncond_tokens = paddle.to_tensor(uncond_tokens)
 
     # get the embeddings
     text_embeddings = get_unweighted_text_embeddings(
-        pipe,
-        prompt_tokens,
-        pipe.tokenizer.model_max_length,
-        no_boseos_middle=no_boseos_middle)
-    prompt_weights = paddle.to_tensor(prompt_weights,
-                                      dtype=text_embeddings.dtype)
+        pipe, prompt_tokens, pipe.tokenizer.model_max_length, no_boseos_middle=no_boseos_middle
+    )
+    prompt_weights = paddle.to_tensor(prompt_weights, dtype=text_embeddings.dtype)
     if uncond_prompt is not None:
         uncond_embeddings = get_unweighted_text_embeddings(
-            pipe,
-            uncond_tokens,
-            pipe.tokenizer.model_max_length,
-            no_boseos_middle=no_boseos_middle)
-        uncond_weights = paddle.to_tensor(uncond_weights,
-                                          dtype=uncond_embeddings.dtype)
+            pipe, uncond_tokens, pipe.tokenizer.model_max_length, no_boseos_middle=no_boseos_middle
+        )
+        uncond_weights = paddle.to_tensor(uncond_weights, dtype=uncond_embeddings.dtype)
 
     # assign weights to the prompts and normalize in the sense of mean
     # TODO: should we normalize by chunk or in a whole (current implementation)?
     if (not skip_parsing) and (not skip_weighting):
         previous_mean = text_embeddings.mean(axis=[-2, -1])
         text_embeddings *= prompt_weights.unsqueeze(-1)
         text_embeddings *= previous_mean / text_embeddings.mean(axis=[-2, -1])
         if uncond_prompt is not None:
             previous_mean = uncond_embeddings.mean(axis=[-2, -1])
             uncond_embeddings *= uncond_weights.unsqueeze(-1)
-            uncond_embeddings *= previous_mean / uncond_embeddings.mean(
-                axis=[-2, -1])
+            uncond_embeddings *= previous_mean / uncond_embeddings.mean(axis=[-2, -1])
 
     # For classifier free guidance, we need to do two forward passes.
     # Here we concatenate the unconditional and text embeddings into a single batch
     # to avoid doing two forward passes
     if uncond_prompt is not None:
         text_embeddings = paddle.concat([uncond_embeddings, text_embeddings])
 
     return text_embeddings
 
 
 def preprocess_image(image):
     w, h = image.size
     w, h = map(lambda x: x - x % 32, (w, h))  # resize to integer multiple of 32
-    image = image.resize((w, h), resample=Resampling.LANCZOS)
+    image = image.resize((w, h), resample=PIL_INTERPOLATION["lanczos"])
     image = np.array(image).astype(np.float32) / 255.0
     image = image[None].transpose(0, 3, 1, 2)
     image = paddle.to_tensor(image)
     return 2.0 * image - 1.0
 
 
 def preprocess_mask(mask):
     mask = mask.convert("L")
     w, h = mask.size
     w, h = map(lambda x: x - x % 32, (w, h))  # resize to integer multiple of 32
-    mask = mask.resize((w // 8, h // 8), resample=Resampling.NEAREST)
+    mask = mask.resize((w // 8, h // 8), resample=PIL_INTERPOLATION["nearest"])
     mask = np.array(mask).astype(np.float32) / 255.0
     mask = np.tile(mask, (4, 1, 1))
     mask = mask[None].transpose(0, 1, 2, 3)  # what does this step do?
     mask = 1 - mask  # repaint white, keep black
     mask = paddle.to_tensor(mask)
     return mask
 
 
 class StableDiffusionPipelineAllinOne(DiffusionPipeline):
     r"""
     Pipeline for text-to-image image-to-image inpainting generation using Stable Diffusion.
 
     This model inherits from [`DiffusionPipeline`]. Check the superclass documentation for the generic methods the
-    library implements for all the pipelines (such as downloading or saving, running on a particular device, etc.)
+    library implements for all the pipelines (such as downloading or saving, running on a particular xxxx, etc.)
 
     Args:
         vae ([`AutoencoderKL`]):
             Variational Auto-Encoder (VAE) Model to encode and decode images to and from latent representations.
         text_encoder ([`CLIPTextModel`]):
             Frozen text-encoder. Stable Diffusion uses the text portion of
             [CLIP](https://huggingface.co/docs/transformers/model_doc/clip#transformers.CLIPTextModel), specifically
             the [clip-vit-large-patch14](https://huggingface.co/openai/clip-vit-large-patch14) variant.
         tokenizer (`CLIPTokenizer`):
             Tokenizer of class
             [CLIPTokenizer](https://huggingface.co/docs/transformers/v4.21.0/en/model_doc/clip#transformers.CLIPTokenizer).
         unet ([`UNet2DConditionModel`]): Conditional U-Net architecture to denoise the encoded image latents.
         scheduler ([`SchedulerMixin`]):
-            A scheduler to be used in combination with `unet` to denoise the encoded image latens. Can be one of
-            [`DDIMScheduler`], [`LMSDiscreteScheduler`], or [`PNDMScheduler`].
+            A scheduler to be used in combination with `unet` to denoise the encoded image latents. Can be one of
+            [`DDIMScheduler`], [`LMSDiscreteScheduler`], [`PNDMScheduler`], [`EulerDiscreteScheduler`], [`EulerAncestralDiscreteScheduler`]
+            or [`DPMSolverMultistepScheduler`].
         safety_checker ([`StableDiffusionSafetyChecker`]):
             Classification module that estimates whether generated images could be considered offensive or harmful.
             Please, refer to the [model card](https://huggingface.co/junnyu/stable-diffusion-v1-4-paddle) for details.
         feature_extractor ([`CLIPFeatureExtractor`]):
             Model that extracts features from generated images to be used as inputs for the `safety_checker`.
     """
+    _optional_components = ["safety_checker", "feature_extractor"]
 
     def __init__(
         self,
         vae: AutoencoderKL,
         text_encoder: CLIPTextModel,
         tokenizer: CLIPTokenizer,
         unet: UNet2DConditionModel,
-        scheduler: Union[DDIMScheduler, PNDMScheduler, LMSDiscreteScheduler,
-                         EulerAncestralDiscreteScheduler],
+        scheduler: Union[
+            DDIMScheduler,
+            PNDMScheduler,
+            LMSDiscreteScheduler,
+            EulerDiscreteScheduler,
+            EulerAncestralDiscreteScheduler,
+            DPMSolverMultistepScheduler,
+        ],
         safety_checker: StableDiffusionSafetyChecker,
         feature_extractor: CLIPFeatureExtractor,
+        requires_safety_checker: bool = False,
     ):
-        super().__init__()
-
-        if hasattr(scheduler.config,
-                   "steps_offset") and scheduler.config.steps_offset != 1:
+        if hasattr(scheduler.config, "steps_offset") and scheduler.config.steps_offset != 1:
             deprecation_message = (
                 f"The configuration file of this scheduler: {scheduler} is outdated. `steps_offset`"
                 f" should be set to 1 instead of {scheduler.config.steps_offset}. Please make sure "
                 "to update the config accordingly as leaving `steps_offset` might led to incorrect results"
                 " in future versions. If you have downloaded this checkpoint from the Hugging Face Hub,"
                 " it would be very nice if you could open a Pull request for the `scheduler/scheduler_config.json`"
-                " file")
-            deprecate("steps_offset!=1",
-                      "1.0.0",
-                      deprecation_message,
-                      standard_warn=False)
+                " file"
+            )
+            deprecate("steps_offset!=1", "1.0.0", deprecation_message, standard_warn=False)
             new_config = dict(scheduler.config)
             new_config["steps_offset"] = 1
             scheduler._internal_dict = FrozenDict(new_config)
 
-        if safety_checker is None:
-            logger.warn(
+        if hasattr(scheduler.config, "clip_sample") and scheduler.config.clip_sample is True:
+            deprecation_message = (
+                f"The configuration file of this scheduler: {scheduler} has not set the configuration `clip_sample`."
+                " `clip_sample` should be set to False in the configuration file. Please make sure to update the"
+                " config accordingly as not setting `clip_sample` in the config might lead to incorrect results in"
+                " future versions. If you have downloaded this checkpoint from the Hugging Face Hub, it would be very"
+                " nice if you could open a Pull request for the `scheduler/scheduler_config.json` file"
+            )
+            deprecate("clip_sample not set", "1.0.0", deprecation_message, standard_warn=False)
+            new_config = dict(scheduler.config)
+            new_config["clip_sample"] = False
+            scheduler._internal_dict = FrozenDict(new_config)
+
+        if safety_checker is None and requires_safety_checker:
+            logger.warning(
                 f"You have disabled the safety checker for {self.__class__} by passing `safety_checker=None`. Ensure"
                 " that you abide to the conditions of the Stable Diffusion license and do not expose unfiltered"
                 " results in services or applications open to the public. PaddleNLP team, diffusers team and Hugging Face"
                 " strongly recommend to keep the safety filter enabled in all public facing circumstances, disabling"
                 " it only for use-cases that involve analyzing network behavior or auditing its results. For more"
                 " information, please have a look at https://github.com/huggingface/diffusers/pull/254 ."
             )
+        if safety_checker is not None and feature_extractor is None:
+            raise ValueError(
+                "Make sure to define a feature extractor when loading {self.__class__} if you want to use the safety"
+                " checker. If you do not want to use the safety checker, you can pass `'safety_checker=None'` instead."
+            )
+        is_unet_version_less_0_9_0 = hasattr(unet.config, "_ppdiffusers_version") and version.parse(
+            version.parse(unet.config._ppdiffusers_version).base_version
+        ) < version.parse("0.9.0.dev0")
+        is_unet_sample_size_less_64 = hasattr(unet.config, "sample_size") and unet.config.sample_size < 64
+        if is_unet_version_less_0_9_0 and is_unet_sample_size_less_64:
+            deprecation_message = (
+                "The configuration file of the unet has set the default `sample_size` to smaller than"
+                " 64 which seems highly unlikely .If you're checkpoint is a fine-tuned version of any of the"
+                " following: \n- CompVis/stable-diffusion-v1-4 \n- CompVis/stable-diffusion-v1-3 \n-"
+                " CompVis/stable-diffusion-v1-2 \n- CompVis/stable-diffusion-v1-1 \n- runwayml/stable-diffusion-v1-5"
+                " \n- runwayml/stable-diffusion-inpainting \n you should change 'sample_size' to 64 in the"
+                " configuration file. Please make sure to update the config accordingly as leaving `sample_size=32`"
+                " in the config might lead to incorrect results in future versions. If you have downloaded this"
+                " checkpoint from the Hugging Face Hub, it would be very nice if you could open a Pull request for"
+                " the `unet/config.json` file"
+            )
+            deprecate("sample_size<64", "1.0.0", deprecation_message, standard_warn=False)
+            new_config = dict(unet.config)
+            new_config["sample_size"] = 64
+            unet._internal_dict = FrozenDict(new_config)
 
         self.register_modules(
             vae=vae,
             text_encoder=text_encoder,
             tokenizer=tokenizer,
             unet=unet,
             scheduler=scheduler,
             safety_checker=safety_checker,
             feature_extractor=feature_extractor,
         )
+        self.register_to_config(requires_safety_checker=requires_safety_checker)
 
-    def enable_attention_slicing(self,
-                                 slice_size: Optional[Union[str,
-                                                            int]] = "auto"):
+    def enable_attention_slicing(self, slice_size: Optional[Union[str, int]] = "auto"):
         r"""
         Enable sliced attention computation.
 
         When this option is enabled, the attention module will split the input tensor in slices, to compute attention
         in several steps. This is useful to save some memory in exchange for a small speed decrease.
 
         Args:
             slice_size (`str` or `int`, *optional*, defaults to `"auto"`):
                 When `"auto"`, halves the input to the attention heads, so attention will be computed in two steps. If
                 a number is provided, uses as many slices as `attention_head_dim // slice_size`. In this case,
                 `attention_head_dim` must be a multiple of `slice_size`.
         """
         if slice_size == "auto":
-            # half the attention head size is usually a good trade-off between
-            # speed and memory
-            slice_size = self.unet.config.attention_head_dim // 2
+            if isinstance(self.unet.config.attention_head_dim, int):
+                # half the attention head size is usually a good trade-off between
+                # speed and memory
+                slice_size = self.unet.config.attention_head_dim // 2
+            else:
+                # if `attention_head_dim` is a list, take the smallest head size
+                slice_size = min(self.unet.config.attention_head_dim)
         self.unet.set_attention_slice(slice_size)
 
     def disable_attention_slicing(self):
         r"""
         Disable sliced attention computation. If `enable_attention_slicing` was previously invoked, this method will go
         back to computing attention in one step.
         """
@@ -565,14 +585,157 @@
 
     def __call__(self, *args, **kwargs):
         return self.text2image(*args, **kwargs)
 
     def text2img(self, *args, **kwargs):
         return self.text2image(*args, **kwargs)
 
+    def _encode_prompt(
+        self,
+        prompt,
+        negative_prompt,
+        max_embeddings_multiples,
+        no_boseos_middle,
+        skip_parsing,
+        skip_weighting,
+        do_classifier_free_guidance,
+        num_images_per_prompt,
+    ):
+        if do_classifier_free_guidance and negative_prompt is None:
+            negative_prompt = ""
+        text_embeddings = get_weighted_text_embeddings(
+            self, prompt, negative_prompt, max_embeddings_multiples, no_boseos_middle, skip_parsing, skip_weighting
+        )
+
+        bs_embed, seq_len, _ = text_embeddings.shape
+        text_embeddings = text_embeddings.tile([1, num_images_per_prompt, 1])
+        text_embeddings = text_embeddings.reshape([bs_embed * num_images_per_prompt, seq_len, -1])
+        return text_embeddings
+
+    def run_safety_checker(self, image, dtype):
+        if self.safety_checker is not None:
+            safety_checker_input = self.feature_extractor(self.numpy_to_pil(image), return_tensors="pd")
+            image, has_nsfw_concept = self.safety_checker(
+                images=image, clip_input=safety_checker_input.pixel_values.cast(dtype)
+            )
+        else:
+            has_nsfw_concept = None
+        return image, has_nsfw_concept
+
+    def decode_latents(self, latents):
+        latents = 1 / 0.18215 * latents
+        image = self.vae.decode(latents).sample
+        image = (image / 2 + 0.5).clip(0, 1)
+        # we always cast to float32 as this does not cause significant overhead and is compatible with bfloa16
+        image = image.transpose([0, 2, 3, 1]).cast("float32").numpy()
+        return image
+
+    def prepare_extra_step_kwargs(self, eta):
+        # prepare extra kwargs for the scheduler step, since not all schedulers have the same signature
+        # eta (η) is only used with the DDIMScheduler, it will be ignored for other schedulers.
+        # eta corresponds to η in DDIM paper: https://arxiv.org/abs/2010.02502
+        # and should be between [0, 1]
+
+        accepts_eta = "eta" in set(inspect.signature(self.scheduler.step).parameters.keys())
+        extra_step_kwargs = {}
+        if accepts_eta:
+            extra_step_kwargs["eta"] = eta
+
+        return extra_step_kwargs
+
+    def check_inputs_text2img(self, prompt, height, width, callback_steps):
+        if not isinstance(prompt, str) and not isinstance(prompt, list):
+            raise ValueError(f"`prompt` has to be of type `str` or `list` but is {type(prompt)}")
+
+        if height % 8 != 0 or width % 8 != 0:
+            raise ValueError(f"`height` and `width` have to be divisible by 8 but are {height} and {width}.")
+
+        if (callback_steps is None) or (
+            callback_steps is not None and (not isinstance(callback_steps, int) or callback_steps <= 0)
+        ):
+            raise ValueError(
+                f"`callback_steps` has to be a positive integer but is {callback_steps} of type"
+                f" {type(callback_steps)}."
+            )
+
+    def check_inputs_img2img_inpaint(self, prompt, strength, callback_steps):
+        if not isinstance(prompt, str) and not isinstance(prompt, list):
+            raise ValueError(f"`prompt` has to be of type `str` or `list` but is {type(prompt)}")
+
+        if strength < 0 or strength > 1:
+            raise ValueError(f"The value of strength should in [1.0, 1.0] but is {strength}")
+
+        if (callback_steps is None) or (
+            callback_steps is not None and (not isinstance(callback_steps, int) or callback_steps <= 0)
+        ):
+            raise ValueError(
+                f"`callback_steps` has to be a positive integer but is {callback_steps} of type"
+                f" {type(callback_steps)}."
+            )
+
+    def prepare_latents_text2img(self, batch_size, num_channels_latents, height, width, dtype, latents=None):
+        shape = [batch_size, num_channels_latents, height // 8, width // 8]
+        if latents is None:
+            latents = paddle.randn(shape, dtype=dtype)
+        else:
+            if latents.shape != shape:
+                raise ValueError(f"Unexpected latents shape, got {latents.shape}, expected {shape}")
+
+        # scale the initial noise by the standard deviation required by the scheduler
+        latents = latents * self.scheduler.init_noise_sigma
+        return latents
+
+    def prepare_latents_img2img(self, image, timestep, num_images_per_prompt, dtype):
+        image = image.cast(dtype=dtype)
+        init_latent_dist = self.vae.encode(image).latent_dist
+        init_latents = init_latent_dist.sample()
+        init_latents = 0.18215 * init_latents
+
+        b, c, h, w = init_latents.shape
+        init_latents = init_latents.tile([1, num_images_per_prompt, 1, 1])
+        init_latents = init_latents.reshape([b * num_images_per_prompt, c, h, w])
+
+        # add noise to latents using the timesteps
+        noise = paddle.randn(init_latents.shape, dtype=dtype)
+
+        # get latents
+        init_latents = self.scheduler.add_noise(init_latents, noise, timestep)
+        latents = init_latents
+
+        return latents
+
+    def get_timesteps(self, num_inference_steps, strength):
+        # get the original timestep using init_timestep
+        offset = self.scheduler.config.get("steps_offset", 0)
+        init_timestep = int(num_inference_steps * strength) + offset
+        init_timestep = min(init_timestep, num_inference_steps)
+
+        t_start = max(num_inference_steps - init_timestep + offset, 0)
+        timesteps = self.scheduler.timesteps[t_start:]
+
+        return timesteps
+
+    def prepare_latents_inpaint(self, image, timestep, num_images_per_prompt, dtype):
+        image = image.cast(dtype)
+        init_latent_dist = self.vae.encode(image).latent_dist
+        init_latents = init_latent_dist.sample()
+        init_latents = 0.18215 * init_latents
+
+        b, c, h, w = init_latents.shape
+        init_latents = init_latents.tile([1, num_images_per_prompt, 1, 1])
+        init_latents = init_latents.reshape([b * num_images_per_prompt, c, h, w])
+
+        init_latents_orig = init_latents
+
+        # add noise to latents using the timesteps
+        noise = paddle.randn(init_latents.shape, dtype=dtype)
+        init_latents = self.scheduler.add_noise(init_latents, noise, timestep)
+        latents = init_latents
+        return latents, init_latents_orig, noise
+
     @paddle.no_grad()
     def text2image(
         self,
         prompt: Union[str, List[str]],
         height: int = 512,
         width: int = 512,
         num_inference_steps: int = 50,
@@ -643,159 +806,113 @@
             [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] or `tuple`:
             [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] if `return_dict` is True, otherwise a `tuple.
             When returning a tuple, the first element is a list with the generated images, and the second element is a
             list of `bool`s denoting whether the corresponding generated image likely represents "not-safe-for-work"
             (nsfw) content, according to the `safety_checker`.
         """
         seed = random.randint(0, 2**32) if seed is None else seed
-        argument = dict(prompt=prompt,
-                        negative_prompt=negative_prompt,
-                        height=height,
-                        width=width,
-                        num_inference_steps=num_inference_steps,
-                        guidance_scale=guidance_scale,
-                        num_images_per_prompt=num_images_per_prompt,
-                        eta=eta,
-                        seed=seed,
-                        latents=latents,
-                        max_embeddings_multiples=max_embeddings_multiples,
-                        no_boseos_middle=no_boseos_middle,
-                        skip_parsing=skip_parsing,
-                        skip_weighting=skip_weighting,
-                        epoch_time=time.time())
-        if isinstance(prompt, str):
-            batch_size = 1
-        elif isinstance(prompt, list):
-            batch_size = len(prompt)
-        else:
-            raise ValueError(
-                f"`prompt` has to be of type `str` or `list` but is {type(prompt)}"
-            )
-
-        if height % 8 != 0 or width % 8 != 0:
-            raise ValueError(
-                f"`height` and `width` have to be divisible by 8 but are {height} and {width}."
-            )
-
-        if (callback_steps is None) or (callback_steps is not None and
-                                        (not isinstance(callback_steps, int)
-                                         or callback_steps <= 0)):
-            raise ValueError(
-                f"`callback_steps` has to be a positive integer but is {callback_steps} of type"
-                f" {type(callback_steps)}.")
+        argument = dict(
+            prompt=prompt,
+            negative_prompt=negative_prompt,
+            height=height,
+            width=width,
+            num_inference_steps=num_inference_steps,
+            guidance_scale=guidance_scale,
+            num_images_per_prompt=num_images_per_prompt,
+            eta=eta,
+            seed=seed,
+            latents=latents,
+            max_embeddings_multiples=max_embeddings_multiples,
+            no_boseos_middle=no_boseos_middle,
+            skip_parsing=skip_parsing,
+            skip_weighting=skip_weighting,
+            epoch_time=time.time(),
+        )
+        paddle.seed(seed)
+        # 1. Check inputs. Raise error if not correct
+        self.check_inputs_text2img(prompt, height, width, callback_steps)
 
+        # 2. Define call parameters
+        batch_size = 1 if isinstance(prompt, str) else len(prompt)
+        # here `guidance_scale` is defined analog to the guidance weight `w` of equation (2)
+        # of the Imagen paper: https://arxiv.org/pdf/2205.11487.pdf . `guidance_scale = 1`
+        # corresponds to doing no classifier free guidance.
         do_classifier_free_guidance = guidance_scale > 1.0
-        # get unconditional embeddings for classifier free guidance
-        if do_classifier_free_guidance:
-            if negative_prompt is None:
-                negative_prompt = [""]
-
-        text_embeddings = get_weighted_text_embeddings(
-            self, prompt, negative_prompt, max_embeddings_multiples,
-            no_boseos_middle, skip_parsing, skip_weighting)
-
-        # get the initial random noise unless the user supplied it
-
-        # Unlike in other pipelines, latents need to be generated in the target device
-        # for 1-to-1 results reproducibility with the CompVis implementation.
-        # However this currently doesn't work in `mps`.
-        latents_shape = [
-            batch_size * num_images_per_prompt, self.unet.in_channels,
-            height // 8, width // 8
-        ]
-        if latents is None:
-            if seed is not None:
-                paddle.seed(seed)
 
-            latents = paddle.randn(latents_shape, dtype=text_embeddings.dtype)
-        else:
-            if latents.shape != latents_shape:
-                raise ValueError(
-                    f"Unexpected latents shape, got {latents.shape}, expected {latents_shape}"
-                )
+        # 3. Encode input prompt
+        text_embeddings = self._encode_prompt(
+            prompt,
+            negative_prompt,
+            max_embeddings_multiples,
+            no_boseos_middle,
+            skip_parsing,
+            skip_weighting,
+            do_classifier_free_guidance,
+            num_images_per_prompt,
+        )
 
-        # set timesteps
+        # 4. Prepare timesteps
         self.scheduler.set_timesteps(num_inference_steps)
+        timesteps = self.scheduler.timesteps
 
-        # Some schedulers like PNDM have timesteps as arrays
-        # It's more optimized to move all timesteps to correct device beforehand
-        timesteps_tensor = self.scheduler.timesteps
-
-        # scale the initial noise by the standard deviation required by the scheduler
-        latents = latents * self.scheduler.init_noise_sigma
+        # 5. Prepare latent variables
+        num_channels_latents = self.unet.in_channels
+        latents = self.prepare_latents_text2img(
+            batch_size * num_images_per_prompt,
+            num_channels_latents,
+            height,
+            width,
+            text_embeddings.dtype,
+            latents,
+        )
 
-        # prepare extra kwargs for the scheduler step, since not all schedulers have the same signature
-        # eta (η) is only used with the DDIMScheduler, it will be ignored for other schedulers.
-        # eta corresponds to η in DDIM paper: https://arxiv.org/abs/2010.02502
-        # and should be between [0, 1]
-        accepts_eta = "eta" in set(
-            inspect.signature(self.scheduler.step).parameters.keys())
-        extra_step_kwargs = {}
-        if accepts_eta:
-            extra_step_kwargs["eta"] = eta
+        # 6. Prepare extra step kwargs. TODO: Logic should ideally just be moved out of the pipeline
+        extra_step_kwargs = self.prepare_extra_step_kwargs(eta)
 
-        for i, t in enumerate(self.progress_bar(timesteps_tensor)):
+        # 7. Denoising loop
+        for i, t in enumerate(self.progress_bar(timesteps)):
             # expand the latents if we are doing classifier free guidance
-            latent_model_input = paddle.concat(
-                [latents] * 2) if do_classifier_free_guidance else latents
-            latent_model_input = self.scheduler.scale_model_input(
-                latent_model_input, t)
+            latent_model_input = paddle.concat([latents] * 2) if do_classifier_free_guidance else latents
+            latent_model_input = self.scheduler.scale_model_input(latent_model_input, t)
 
             # predict the noise residual
-            noise_pred = self.unet(latent_model_input,
-                                   t,
-                                   encoder_hidden_states=text_embeddings).sample
+            noise_pred = self.unet(latent_model_input, t, encoder_hidden_states=text_embeddings).sample
 
             # perform guidance
             if do_classifier_free_guidance:
                 noise_pred_uncond, noise_pred_text = noise_pred.chunk(2)
-                noise_pred = noise_pred_uncond + guidance_scale * (
-                    noise_pred_text - noise_pred_uncond)
+                noise_pred = noise_pred_uncond + guidance_scale * (noise_pred_text - noise_pred_uncond)
 
             # compute the previous noisy sample x_t -> x_t-1
-            latents = self.scheduler.step(noise_pred, t, latents,
-                                          **extra_step_kwargs).prev_sample
+            latents = self.scheduler.step(noise_pred, t, latents, **extra_step_kwargs).prev_sample
 
             # call the callback, if provided
             if callback is not None and i % callback_steps == 0:
                 callback(i, t, latents)
 
-        latents = 1 / 0.18215 * latents
-        image = self.vae.decode(latents).sample
-
-        image = (image / 2 + 0.5).clip(0, 1)
-
-        # we always cast to float32 as this does not cause significant overhead and is compatible with bfloa16
-        image = image.transpose([0, 2, 3, 1]).astype("float32").numpy()
+        # 8. Post-processing
+        image = self.decode_latents(latents)
 
-        if self.safety_checker is not None:
-            safety_checker_input = self.feature_extractor(self.numpy_to_pil(
-                image, argument=argument),
-                                                          return_tensors="pd")
-            image, has_nsfw_concept = self.safety_checker(
-                images=image,
-                clip_input=safety_checker_input.pixel_values.astype(
-                    text_embeddings.dtype))
-        else:
-            has_nsfw_concept = None
+        # 9. Run safety checker
+        image, has_nsfw_concept = self.run_safety_checker(image, text_embeddings.dtype)
 
+        # 10. Convert to PIL
         if output_type == "pil":
             image = self.numpy_to_pil(image, argument=argument)
 
         if not return_dict:
             return (image, has_nsfw_concept)
 
-        return StableDiffusionPipelineOutput(
-            images=image, nsfw_content_detected=has_nsfw_concept)
+        return StableDiffusionPipelineOutput(images=image, nsfw_content_detected=has_nsfw_concept)
 
     @paddle.no_grad()
     def img2img(
         self,
         prompt: Union[str, List[str]],
-        init_image: Union[paddle.Tensor, PIL.Image.Image],
+        image: Union[paddle.Tensor, PIL.Image.Image],
         strength: float = 0.8,
         height=None,
         width=None,
         num_inference_steps: Optional[int] = 50,
         guidance_scale: Optional[float] = 7.5,
         negative_prompt: Optional[Union[str, List[str]]] = None,
         num_images_per_prompt: Optional[int] = 1,
@@ -814,23 +931,23 @@
     ):
         r"""
         Function invoked when calling the pipeline for generation.
 
         Args:
             prompt (`str` or `List[str]`):
                 The prompt or prompts to guide the image generation.
-            init_image (`paddle.Tensor` or `PIL.Image.Image`):
+            image (`paddle.Tensor` or `PIL.Image.Image`):
                 `Image`, or tensor representing an image batch, that will be used as the starting point for the
                 process.
             strength (`float`, *optional*, defaults to 0.8):
-                Conceptually, indicates how much to transform the reference `init_image`. Must be between 0 and 1.
-                `init_image` will be used as a starting point, adding more noise to it the larger the `strength`. The
+                Conceptually, indicates how much to transform the reference `image`. Must be between 0 and 1.
+                `image` will be used as a starting point, adding more noise to it the larger the `strength`. The
                 number of denoising steps depends on the amount of noise initially added. When `strength` is 1, added
                 noise will be maximum and the denoising process will run for the full number of iterations specified in
-                `num_inference_steps`. A value of 1, therefore, essentially ignores `init_image`.
+                `num_inference_steps`. A value of 1, therefore, essentially ignores `image`.
             num_inference_steps (`int`, *optional*, defaults to 50):
                 The number of denoising steps. More denoising steps usually lead to a higher quality image at the
                 expense of slower inference. This parameter will be modulated by `strength`.
             guidance_scale (`float`, *optional*, defaults to 7.5):
                 Guidance scale as defined in [Classifier-Free Diffusion Guidance](https://arxiv.org/abs/2207.12598).
                 `guidance_scale` is defined as `w` of equation 2. of [Imagen
                 Paper](https://arxiv.org/pdf/2205.11487.pdf). Guidance scale is enabled by setting `guidance_scale >
@@ -863,208 +980,128 @@
             [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] or `tuple`:
             [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] if `return_dict` is True, otherwise a `tuple.
             When returning a tuple, the first element is a list with the generated images, and the second element is a
             list of `bool`s denoting whether the corresponding generated image likely represents "not-safe-for-work"
             (nsfw) content, according to the `safety_checker`.
         """
         seed = random.randint(0, 2**32) if seed is None else seed
-        init_image_str = init_image
-        if isinstance(init_image_str, str):
-            init_image = load_image(init_image_str)
+        image_str = image
+        if isinstance(image_str, str):
+            image = load_image(image_str)
 
         if height is None and width is None:
-            width = (init_image.size[0] // 8) * 8
-            height = (init_image.size[1] // 8) * 8
+            width = (image.size[0] // 8) * 8
+            height = (image.size[1] // 8) * 8
         elif height is None and width is not None:
-            height = (init_image.size[1] // 8) * 8
+            height = (image.size[1] // 8) * 8
         elif width is None and height is not None:
-            width = (init_image.size[0] // 8) * 8
+            width = (image.size[0] // 8) * 8
         else:
             height = height
             width = width
 
-        argument = dict(prompt=prompt,
-                        init_image=init_image_str,
-                        negative_prompt=negative_prompt,
-                        height=height,
-                        width=width,
-                        strength=strength,
-                        num_inference_steps=num_inference_steps,
-                        guidance_scale=guidance_scale,
-                        num_images_per_prompt=num_images_per_prompt,
-                        eta=eta,
-                        seed=seed,
-                        max_embeddings_multiples=max_embeddings_multiples,
-                        no_boseos_middle=no_boseos_middle,
-                        skip_parsing=skip_parsing,
-                        skip_weighting=skip_weighting,
-                        epoch_time=time.time())
-
-        if isinstance(prompt, str):
-            batch_size = 1
-        elif isinstance(prompt, list):
-            batch_size = len(prompt)
-        else:
-            raise ValueError(
-                f"`prompt` has to be of type `str` or `list` but is {type(prompt)}"
-            )
-
-        if strength < 0 or strength > 1:
-            raise ValueError(
-                f"The value of strength should in [0.0, 1.0] but is {strength}")
-
-        if (callback_steps is None) or (callback_steps is not None and
-                                        (not isinstance(callback_steps, int)
-                                         or callback_steps <= 0)):
-            raise ValueError(
-                f"`callback_steps` has to be a positive integer but is {callback_steps} of type"
-                f" {type(callback_steps)}.")
-
-        # set timesteps
-        self.scheduler.set_timesteps(num_inference_steps)
+        argument = dict(
+            prompt=prompt,
+            image=image_str,
+            negative_prompt=negative_prompt,
+            height=height,
+            width=width,
+            strength=strength,
+            num_inference_steps=num_inference_steps,
+            guidance_scale=guidance_scale,
+            num_images_per_prompt=num_images_per_prompt,
+            eta=eta,
+            seed=seed,
+            max_embeddings_multiples=max_embeddings_multiples,
+            no_boseos_middle=no_boseos_middle,
+            skip_parsing=skip_parsing,
+            skip_weighting=skip_weighting,
+            epoch_time=time.time(),
+        )
+        paddle.seed(seed)
 
-        if isinstance(init_image, PIL.Image.Image):
-            init_image = init_image.resize((width, height))
-            init_image = preprocess_image(init_image)
+        # 1. Check inputs
+        self.check_inputs_img2img_inpaint(prompt, strength, callback_steps)
 
+        # 2. Define call parameters
+        batch_size = 1 if isinstance(prompt, str) else len(prompt)
+        # here `guidance_scale` is defined analog to the guidance weight `w` of equation (2)
+        # of the Imagen paper: https://arxiv.org/pdf/2205.11487.pdf . `guidance_scale = 1`
+        # corresponds to doing no classifier free guidance.
         do_classifier_free_guidance = guidance_scale > 1.0
-        # get unconditional embeddings for classifier free guidance
-        if do_classifier_free_guidance:
-            if negative_prompt is None:
-                negative_prompt = [""]
 
-        text_embeddings = get_weighted_text_embeddings(
-            self, prompt, negative_prompt, max_embeddings_multiples,
-            no_boseos_middle, skip_parsing, skip_weighting)
-
-        # encode the init image into latents and scale the latents
-        latents_dtype = text_embeddings.dtype
-        init_image = init_image.astype(latents_dtype)
-        init_latent_dist = self.vae.encode(init_image).latent_dist
-        init_latents = init_latent_dist.sample()
-        init_latents = 0.18215 * init_latents
-
-        if isinstance(prompt, str):
-            prompt = [prompt]
-        if len(prompt) > init_latents.shape[0] and len(
-                prompt) % init_latents.shape[0] == 0:
-            # expand init_latents for batch_size
-            deprecation_message = (
-                f"You have passed {len(prompt)} text prompts (`prompt`), but only {init_latents.shape[0]} initial"
-                " images (`init_image`). Initial images are now duplicating to match the number of text prompts. Note"
-                " that this behavior is deprecated is will be removed in a version 1.0.0. Please make sure to update"
-                " your script to pass as many init images as text prompts to suppress this warning."
-            )
-            deprecate("len(prompt) != len(init_image)",
-                      "1.0.0",
-                      deprecation_message,
-                      standard_warn=False)
-            additional_image_per_prompt = len(prompt) // init_latents.shape[0]
-            init_latents = paddle.concat([init_latents] *
-                                         additional_image_per_prompt *
-                                         num_images_per_prompt)
-        elif len(prompt) > init_latents.shape[0] and len(
-                prompt) % init_latents.shape[0] != 0:
-            raise ValueError(
-                f"Cannot duplicate `init_image` of batch size {init_latents.shape[0]} to {len(prompt)} text prompts."
-            )
-        else:
-            init_latents = paddle.concat([init_latents] * num_images_per_prompt)
-
-        # get the original timestep using init_timestep
-        offset = self.scheduler.config.get("steps_offset", 0)
-        init_timestep = int(num_inference_steps * strength) + offset
-        init_timestep = min(init_timestep, num_inference_steps)
-
-        timesteps = self.scheduler.timesteps[-init_timestep]
-        timesteps = timesteps.tile([
-            batch_size * num_images_per_prompt,
-        ])
-
-        if seed is not None:
-            paddle.seed(seed)
-        # add noise to latents using the timesteps
-        noise = paddle.randn(init_latents.shape, dtype=latents_dtype)
-        init_latents = self.scheduler.add_noise(init_latents, noise, timesteps)
+        # 3. Encode input prompt
+        text_embeddings = self._encode_prompt(
+            prompt,
+            negative_prompt,
+            max_embeddings_multiples,
+            no_boseos_middle,
+            skip_parsing,
+            skip_weighting,
+            do_classifier_free_guidance,
+            num_images_per_prompt,
+        )
 
-        # prepare extra kwargs for the scheduler step, since not all schedulers have the same signature
-        # eta (η) is only used with the DDIMScheduler, it will be ignored for other schedulers.
-        # eta corresponds to η in DDIM paper: https://arxiv.org/abs/2010.02502
-        # and should be between [0, 1]
-        accepts_eta = "eta" in set(
-            inspect.signature(self.scheduler.step).parameters.keys())
-        extra_step_kwargs = {}
-        if accepts_eta:
-            extra_step_kwargs["eta"] = eta
+        # 4. Preprocess image
+        if isinstance(image, PIL.Image.Image):
+            image = image.resize((width, height))
+            image = preprocess_image(image)
 
-        latents = init_latents
+        # 5. set timesteps
+        self.scheduler.set_timesteps(num_inference_steps)
+        timesteps = self.get_timesteps(num_inference_steps, strength)
+        latent_timestep = timesteps[:1].tile([batch_size * num_images_per_prompt])
 
-        t_start = max(num_inference_steps - init_timestep + offset, 0)
+        # 6. Prepare latent variables
+        latents = self.prepare_latents_img2img(image, latent_timestep, num_images_per_prompt, text_embeddings.dtype)
 
-        # Some schedulers like PNDM have timesteps as arrays
-        # It's more optimized to move all timesteps to correct device beforehand
-        timesteps = self.scheduler.timesteps[t_start:]
+        # 7. Prepare extra step kwargs. TODO: Logic should ideally just be moved out of the pipeline
+        extra_step_kwargs = self.prepare_extra_step_kwargs(eta)
 
+        # 8. Denoising loop
         for i, t in enumerate(self.progress_bar(timesteps)):
             # expand the latents if we are doing classifier free guidance
-            latent_model_input = paddle.concat(
-                [latents] * 2) if do_classifier_free_guidance else latents
-            latent_model_input = self.scheduler.scale_model_input(
-                latent_model_input, t)
+            latent_model_input = paddle.concat([latents] * 2) if do_classifier_free_guidance else latents
+            latent_model_input = self.scheduler.scale_model_input(latent_model_input, t)
 
             # predict the noise residual
-            noise_pred = self.unet(latent_model_input,
-                                   t,
-                                   encoder_hidden_states=text_embeddings).sample
+            noise_pred = self.unet(latent_model_input, t, encoder_hidden_states=text_embeddings).sample
 
             # perform guidance
             if do_classifier_free_guidance:
                 noise_pred_uncond, noise_pred_text = noise_pred.chunk(2)
-                noise_pred = noise_pred_uncond + guidance_scale * (
-                    noise_pred_text - noise_pred_uncond)
+                noise_pred = noise_pred_uncond + guidance_scale * (noise_pred_text - noise_pred_uncond)
 
             # compute the previous noisy sample x_t -> x_t-1
-            latents = self.scheduler.step(noise_pred, t, latents,
-                                          **extra_step_kwargs).prev_sample
+            latents = self.scheduler.step(noise_pred, t, latents, **extra_step_kwargs).prev_sample
 
             # call the callback, if provided
             if callback is not None and i % callback_steps == 0:
                 callback(i, t, latents)
 
-        latents = 1 / 0.18215 * latents
-        image = self.vae.decode(latents).sample
+        # 9. Post-processing
+        image = self.decode_latents(latents)
 
-        image = (image / 2 + 0.5).clip(0, 1)
-        image = image.transpose([0, 2, 3, 1]).numpy()
-
-        if self.safety_checker is not None:
-            safety_checker_input = self.feature_extractor(self.numpy_to_pil(
-                image, argument=argument),
-                                                          return_tensors="pd")
-            image, has_nsfw_concept = self.safety_checker(
-                images=image,
-                clip_input=safety_checker_input.pixel_values.astype(
-                    text_embeddings.dtype))
-        else:
-            has_nsfw_concept = None
+        # 10. Run safety checker
+        image, has_nsfw_concept = self.run_safety_checker(image, text_embeddings.dtype)
 
+        # 11. Convert to PIL
         if output_type == "pil":
             image = self.numpy_to_pil(image, argument=argument)
 
         if not return_dict:
             return (image, has_nsfw_concept)
 
-        return StableDiffusionPipelineOutput(
-            images=image, nsfw_content_detected=has_nsfw_concept)
+        return StableDiffusionPipelineOutput(images=image, nsfw_content_detected=has_nsfw_concept)
 
     @paddle.no_grad()
     def inpaint(
         self,
         prompt: Union[str, List[str]],
-        init_image: Union[paddle.Tensor, PIL.Image.Image],
+        image: Union[paddle.Tensor, PIL.Image.Image],
         mask_image: Union[paddle.Tensor, PIL.Image.Image],
         height=None,
         width=None,
         strength: float = 0.8,
         num_inference_steps: Optional[int] = 50,
         guidance_scale: Optional[float] = 7.5,
         negative_prompt: Optional[Union[str, List[str]]] = None,
@@ -1084,26 +1121,26 @@
     ):
         r"""
         Function invoked when calling the pipeline for generation.
 
         Args:
             prompt (`str` or `List[str]`):
                 The prompt or prompts to guide the image generation.
-            init_image (`paddle.Tensor` or `PIL.Image.Image`):
+            image (`paddle.Tensor` or `PIL.Image.Image`):
                 `Image`, or tensor representing an image batch, that will be used as the starting point for the
                 process. This is the image whose masked region will be inpainted.
             mask_image (`paddle.Tensor` or `PIL.Image.Image`):
-                `Image`, or tensor representing an image batch, to mask `init_image`. White pixels in the mask will be
+                `Image`, or tensor representing an image batch, to mask `image`. White pixels in the mask will be
                 replaced by noise and therefore repainted, while black pixels will be preserved. If `mask_image` is a
                 PIL image, it will be converted to a single channel (luminance) before use. If it's a tensor, it should
                 contain one color channel (L) instead of 3, so the expected shape would be `(B, H, W, 1)`.
             strength (`float`, *optional*, defaults to 0.8):
                 Conceptually, indicates how much to inpaint the masked area. Must be between 0 and 1. When `strength`
                 is 1, the denoising process will be run on the masked area for the full number of iterations specified
-                in `num_inference_steps`. `init_image` will be used as a reference for the masked area, adding more
+                in `num_inference_steps`. `image` will be used as a reference for the masked area, adding more
                 noise to that region the larger the `strength`. If `strength` is 0, no inpainting will occur.
             num_inference_steps (`int`, *optional*, defaults to 50):
                 The reference number of denoising steps. More denoising steps usually lead to a higher quality image at
                 the expense of slower inference. This parameter will be modulated by `strength`, as explained above.
             guidance_scale (`float`, *optional*, defaults to 7.5):
                 Guidance scale as defined in [Classifier-Free Diffusion Guidance](https://arxiv.org/abs/2207.12598).
                 `guidance_scale` is defined as `w` of equation 2. of [Imagen
@@ -1137,197 +1174,152 @@
             [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] or `tuple`:
             [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] if `return_dict` is True, otherwise a `tuple.
             When returning a tuple, the first element is a list with the generated images, and the second element is a
             list of `bool`s denoting whether the corresponding generated image likely represents "not-safe-for-work"
             (nsfw) content, according to the `safety_checker`.
         """
         seed = random.randint(0, 2**32) if seed is None else seed
-        init_image_str = init_image
+        image_str = image
         mask_image_str = mask_image
 
-        if isinstance(init_image_str, str):
-            init_image = load_image(init_image_str)
+        if isinstance(image_str, str):
+            image = load_image(image_str)
         if isinstance(mask_image_str, str):
             mask_image = load_image(mask_image_str)
 
         if height is None and width is None:
-            width = (init_image.size[0] // 8) * 8
-            height = (init_image.size[1] // 8) * 8
+            width = (image.size[0] // 8) * 8
+            height = (image.size[1] // 8) * 8
         elif height is None and width is not None:
-            height = (init_image.size[1] // 8) * 8
+            height = (image.size[1] // 8) * 8
         elif width is None and height is not None:
-            width = (init_image.size[0] // 8) * 8
+            width = (image.size[0] // 8) * 8
         else:
             height = height
             width = width
 
-        argument = dict(prompt=prompt,
-                        init_image=init_image_str,
-                        negative_prompt=negative_prompt,
-                        height=height,
-                        width=width,
-                        strength=strength,
-                        num_inference_steps=num_inference_steps,
-                        guidance_scale=guidance_scale,
-                        num_images_per_prompt=num_images_per_prompt,
-                        eta=eta,
-                        seed=seed,
-                        max_embeddings_multiples=max_embeddings_multiples,
-                        no_boseos_middle=no_boseos_middle,
-                        skip_parsing=skip_parsing,
-                        skip_weighting=skip_weighting,
-                        epoch_time=time.time())
-        if isinstance(prompt, str):
-            batch_size = 1
-        elif isinstance(prompt, list):
-            batch_size = len(prompt)
-        else:
-            raise ValueError(
-                f"`prompt` has to be of type `str` or `list` but is {type(prompt)}"
-            )
-
-        if strength < 0 or strength > 1:
-            raise ValueError(
-                f"The value of strength should in [0.0, 1.0] but is {strength}")
-
-        if (callback_steps is None) or (callback_steps is not None and
-                                        (not isinstance(callback_steps, int)
-                                         or callback_steps <= 0)):
-            raise ValueError(
-                f"`callback_steps` has to be a positive integer but is {callback_steps} of type"
-                f" {type(callback_steps)}.")
+        argument = dict(
+            prompt=prompt,
+            image=image_str,
+            mask_image=mask_image_str,
+            negative_prompt=negative_prompt,
+            height=height,
+            width=width,
+            strength=strength,
+            num_inference_steps=num_inference_steps,
+            guidance_scale=guidance_scale,
+            num_images_per_prompt=num_images_per_prompt,
+            eta=eta,
+            seed=seed,
+            max_embeddings_multiples=max_embeddings_multiples,
+            no_boseos_middle=no_boseos_middle,
+            skip_parsing=skip_parsing,
+            skip_weighting=skip_weighting,
+            epoch_time=time.time(),
+        )
+        paddle.seed(seed)
 
-        # set timesteps
-        self.scheduler.set_timesteps(num_inference_steps)
+        # 1. Check inputs
+        self.check_inputs_img2img_inpaint(prompt, strength, callback_steps)
 
+        # 2. Define call parameters
+        batch_size = 1 if isinstance(prompt, str) else len(prompt)
         # here `guidance_scale` is defined analog to the guidance weight `w` of equation (2)
         # of the Imagen paper: https://arxiv.org/pdf/2205.11487.pdf . `guidance_scale = 1`
         # corresponds to doing no classifier free guidance.
         do_classifier_free_guidance = guidance_scale > 1.0
-        # get unconditional embeddings for classifier free guidance
-        if do_classifier_free_guidance:
-            if negative_prompt is None:
-                negative_prompt = [""]
-
-        text_embeddings = get_weighted_text_embeddings(
-            self, prompt, negative_prompt, max_embeddings_multiples,
-            no_boseos_middle, skip_parsing, skip_weighting)
-
-        if isinstance(init_image, PIL.Image.Image):
-            init_image = init_image.resize((width, height))
-            init_image = preprocess_image(init_image)
 
-        # encode the init image into latents and scale the latents
-        latents_dtype = text_embeddings.dtype
-        init_image = init_image.astype(latents_dtype)
-        init_latent_dist = self.vae.encode(init_image).latent_dist
-        init_latents = init_latent_dist.sample()
-        init_latents = 0.18215 * init_latents
+        # 3. Encode input prompt
+        text_embeddings = self._encode_prompt(
+            prompt,
+            negative_prompt,
+            max_embeddings_multiples,
+            no_boseos_middle,
+            skip_parsing,
+            skip_weighting,
+            do_classifier_free_guidance,
+            num_images_per_prompt,
+        )
 
-        # Expand init_latents for batch_size and num_images_per_prompt
-        init_latents = paddle.concat([init_latents] * batch_size *
-                                     num_images_per_prompt,
-                                     axis=0)
-        init_latents_orig = init_latents
+        if not isinstance(image, paddle.Tensor):
+            image = image.resize((width, height))
+            image = preprocess_image(image)
 
-        # preprocess mask
-        if isinstance(mask_image, PIL.Image.Image):
+        if not isinstance(mask_image, paddle.Tensor):
             mask_image = mask_image.resize((width, height))
             mask_image = preprocess_mask(mask_image)
 
-        mask_image = mask_image.astype(latents_dtype)
-        mask = paddle.concat([mask_image] * batch_size * num_images_per_prompt)
-
-        # check sizes
-        if not mask.shape == init_latents.shape:
-            raise ValueError("The mask and init_image should be the same size!")
-
-        # get the original timestep using init_timestep
-        offset = self.scheduler.config.get("steps_offset", 0)
-        init_timestep = int(num_inference_steps * strength) + offset
-        init_timestep = min(init_timestep, num_inference_steps)
-
-        timesteps = self.scheduler.timesteps[-init_timestep]
-        timesteps = timesteps.tile([
-            batch_size * num_images_per_prompt,
-        ])
-
-        # add noise to latents using the timesteps
-        if seed is not None:
-            paddle.seed(seed)
-        noise = paddle.randn(init_latents.shape, dtype=latents_dtype)
-        init_latents = self.scheduler.add_noise(init_latents, noise, timesteps)
-
-        # prepare extra kwargs for the scheduler step, since not all schedulers have the same signature
-        # eta (η) is only used with the DDIMScheduler, it will be ignored for other schedulers.
-        # eta corresponds to η in DDIM paper: https://arxiv.org/abs/2010.02502
-        # and should be between [0, 1]
-        accepts_eta = "eta" in set(
-            inspect.signature(self.scheduler.step).parameters.keys())
-        extra_step_kwargs = {}
-        if accepts_eta:
-            extra_step_kwargs["eta"] = eta
+        # 5. set timesteps
+        self.scheduler.set_timesteps(num_inference_steps)
+        timesteps = self.get_timesteps(num_inference_steps, strength)
+        latent_timestep = timesteps[:1].tile([batch_size * num_images_per_prompt])
 
-        latents = init_latents
+        # 6. Prepare latent variables
+        # encode the init image into latents and scale the latents
+        latents, init_latents_orig, noise = self.prepare_latents_inpaint(
+            image, latent_timestep, num_images_per_prompt, text_embeddings.dtype
+        )
 
-        t_start = max(num_inference_steps - init_timestep + offset, 0)
+        # 7. Prepare mask latent
+        mask = mask_image.cast(latents.dtype)
+        mask = paddle.concat([mask] * batch_size * num_images_per_prompt)
 
-        # Some schedulers like PNDM have timesteps as arrays
-        # It's more optimized to move all timesteps to correct device beforehand
-        timesteps = self.scheduler.timesteps[t_start:]
+        # 8. Prepare extra step kwargs. TODO: Logic should ideally just be moved out of the pipeline
+        extra_step_kwargs = self.prepare_extra_step_kwargs(eta)
 
+        # 9. Denoising loop
         for i, t in enumerate(self.progress_bar(timesteps)):
             # expand the latents if we are doing classifier free guidance
-            latent_model_input = paddle.concat(
-                [latents] * 2) if do_classifier_free_guidance else latents
-            latent_model_input = self.scheduler.scale_model_input(
-                latent_model_input, t)
+            latent_model_input = paddle.concat([latents] * 2) if do_classifier_free_guidance else latents
+            latent_model_input = self.scheduler.scale_model_input(latent_model_input, t)
 
             # predict the noise residual
-            noise_pred = self.unet(latent_model_input,
-                                   t,
-                                   encoder_hidden_states=text_embeddings).sample
+            noise_pred = self.unet(latent_model_input, t, encoder_hidden_states=text_embeddings).sample
 
             # perform guidance
             if do_classifier_free_guidance:
                 noise_pred_uncond, noise_pred_text = noise_pred.chunk(2)
-                noise_pred = noise_pred_uncond + guidance_scale * (
-                    noise_pred_text - noise_pred_uncond)
+                noise_pred = noise_pred_uncond + guidance_scale * (noise_pred_text - noise_pred_uncond)
 
             # compute the previous noisy sample x_t -> x_t-1
-            latents = self.scheduler.step(noise_pred, t, latents,
-                                          **extra_step_kwargs).prev_sample
+            latents = self.scheduler.step(noise_pred, t, latents, **extra_step_kwargs).prev_sample
             # masking
-            init_latents_proper = self.scheduler.add_noise(
-                init_latents_orig, noise, t)
+            init_latents_proper = self.scheduler.add_noise(init_latents_orig, noise, t)
 
             latents = (init_latents_proper * mask) + (latents * (1 - mask))
 
             # call the callback, if provided
             if callback is not None and i % callback_steps == 0:
                 callback(i, t, latents)
 
-        latents = 1 / 0.18215 * latents
-        image = self.vae.decode(latents).sample
-
-        image = (image / 2 + 0.5).clip(0, 1)
-        image = image.transpose([0, 2, 3, 1]).numpy()
+        # 10. Post-processing
+        image = self.decode_latents(latents)
 
-        if self.safety_checker is not None:
-            safety_checker_input = self.feature_extractor(self.numpy_to_pil(
-                image, argument=argument),
-                                                          return_tensors="pd")
-            image, has_nsfw_concept = self.safety_checker(
-                images=image,
-                clip_input=safety_checker_input.pixel_values.astype(
-                    text_embeddings.dtype))
-        else:
-            has_nsfw_concept = None
+        # 11. Run safety checker
+        image, has_nsfw_concept = self.run_safety_checker(image, text_embeddings.dtype)
 
+        # 12. Convert to PIL
         if output_type == "pil":
             image = self.numpy_to_pil(image, argument=argument)
 
         if not return_dict:
             return (image, has_nsfw_concept)
 
-        return StableDiffusionPipelineOutput(
-            images=image, nsfw_content_detected=has_nsfw_concept)
+        return StableDiffusionPipelineOutput(images=image, nsfw_content_detected=has_nsfw_concept)
+
+    @staticmethod
+    def numpy_to_pil(images, **kwargs):
+        """
+        Convert a numpy image or a batch of images to a PIL image.
+        """
+        if images.ndim == 3:
+            images = images[None, ...]
+        images = (images * 255).round().astype("uint8")
+        pil_images = []
+        argument = kwargs.pop("argument", None)
+        for image in images:
+            image = PIL.Image.fromarray(image)
+            if argument is not None:
+                image.argument = argument
+            pil_images.append(image)
+
+        return pil_images
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_img2img.py` & `ppdiffusers-0.9.0/ppdiffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_image_variation.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,206 +12,309 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import inspect
 from typing import Callable, List, Optional, Union
 
-import numpy as np
 import paddle
-
 import PIL
-from paddlenlp.utils.tools import compare_version
-if compare_version(PIL.__version__, "9.1.0") >= 0:
-    Resampling = PIL.Image.Resampling
-else:
-    Resampling = PIL.Image
+from packaging import version
 
-from paddlenlp.transformers import CLIPFeatureExtractor, CLIPTextModel, CLIPTokenizer
+from paddlenlp.transformers import CLIPFeatureExtractor, CLIPVisionModelWithProjection
 
 from ...configuration_utils import FrozenDict
 from ...models import AutoencoderKL, UNet2DConditionModel
 from ...pipeline_utils import DiffusionPipeline
-from ...schedulers import DDIMScheduler, LMSDiscreteScheduler, PNDMScheduler, EulerAncestralDiscreteScheduler
+from ...schedulers import (
+    DDIMScheduler,
+    DPMSolverMultistepScheduler,
+    EulerAncestralDiscreteScheduler,
+    EulerDiscreteScheduler,
+    LMSDiscreteScheduler,
+    PNDMScheduler,
+)
 from ...utils import deprecate, logging
 from . import StableDiffusionPipelineOutput
 from .safety_checker import StableDiffusionSafetyChecker
 
 logger = logging.get_logger(__name__)  # pylint: disable=invalid-name
 
 
-def preprocess(image):
-    w, h = image.size
-    w, h = map(lambda x: x - x % 32, (w, h))  # resize to integer multiple of 32
-    image = image.resize((w, h), resample=Resampling.LANCZOS)
-    image = np.array(image).astype(np.float32) / 255.0
-    image = image[None].transpose(0, 3, 1, 2)
-    image = paddle.to_tensor(image)
-    return 2.0 * image - 1.0
-
-
-class StableDiffusionImg2ImgPipeline(DiffusionPipeline):
+class StableDiffusionImageVariationPipeline(DiffusionPipeline):
     r"""
-    Pipeline for text-guided image to image generation using Stable Diffusion.
+    Pipeline to generate variations from an input image using Stable Diffusion.
 
     This model inherits from [`DiffusionPipeline`]. Check the superclass documentation for the generic methods the
-    library implements for all the pipelines (such as downloading or saving, running on a particular device, etc.)
+    library implements for all the pipelines (such as downloading or saving etc.)
 
     Args:
         vae ([`AutoencoderKL`]):
             Variational Auto-Encoder (VAE) Model to encode and decode images to and from latent representations.
-        text_encoder ([`CLIPTextModel`]):
-            Frozen text-encoder. Stable Diffusion uses the text portion of
-            [CLIP](https://huggingface.co/docs/transformers/model_doc/clip#transformers.CLIPTextModel), specifically
-            the [clip-vit-large-patch14](https://huggingface.co/openai/clip-vit-large-patch14) variant.
-        tokenizer (`CLIPTokenizer`):
-            Tokenizer of class
-            [CLIPTokenizer](https://huggingface.co/docs/transformers/v4.21.0/en/model_doc/clip#transformers.CLIPTokenizer).
+        image_encoder ([`CLIPVisionModelWithProjection`]):
+            Frozen CLIP image-encoder. Stable Diffusion Image Variation uses the vision portion of
+            [CLIP](https://huggingface.co/docs/transformers/model_doc/clip#transformers.CLIPVisionModelWithProjection),
+            specifically the [clip-vit-large-patch14](https://huggingface.co/openai/clip-vit-large-patch14) variant.
         unet ([`UNet2DConditionModel`]): Conditional U-Net architecture to denoise the encoded image latents.
         scheduler ([`SchedulerMixin`]):
-            A scheduler to be used in combination with `unet` to denoise the encoded image latens. Can be one of
+            A scheduler to be used in combination with `unet` to denoise the encoded image latents. Can be one of
             [`DDIMScheduler`], [`LMSDiscreteScheduler`], or [`PNDMScheduler`].
         safety_checker ([`StableDiffusionSafetyChecker`]):
             Classification module that estimates whether generated images could be considered offensive or harmful.
-            Please, refer to the [model card](https://huggingface.co/junnyu/stable-diffusion-v1-4-paddle) for details.
+            Please, refer to the [model card](https://huggingface.co/runwayml/stable-diffusion-v1-5) for details.
         feature_extractor ([`CLIPFeatureExtractor`]):
             Model that extracts features from generated images to be used as inputs for the `safety_checker`.
     """
+    _optional_components = ["safety_checker", "feature_extractor"]
 
     def __init__(
         self,
         vae: AutoencoderKL,
-        text_encoder: CLIPTextModel,
-        tokenizer: CLIPTokenizer,
+        image_encoder: CLIPVisionModelWithProjection,
         unet: UNet2DConditionModel,
-        scheduler: Union[DDIMScheduler, PNDMScheduler, LMSDiscreteScheduler,
-                         EulerAncestralDiscreteScheduler],
+        scheduler: Union[
+            DDIMScheduler,
+            PNDMScheduler,
+            LMSDiscreteScheduler,
+            EulerDiscreteScheduler,
+            EulerAncestralDiscreteScheduler,
+            DPMSolverMultistepScheduler,
+        ],
         safety_checker: StableDiffusionSafetyChecker,
         feature_extractor: CLIPFeatureExtractor,
+        requires_safety_checker: bool = True,
     ):
         super().__init__()
 
-        if hasattr(scheduler.config,
-                   "steps_offset") and scheduler.config.steps_offset != 1:
-            deprecation_message = (
-                f"The configuration file of this scheduler: {scheduler} is outdated. `steps_offset`"
-                f" should be set to 1 instead of {scheduler.config.steps_offset}. Please make sure "
-                "to update the config accordingly as leaving `steps_offset` might led to incorrect results"
-                " in future versions. If you have downloaded this checkpoint from the Hugging Face Hub,"
-                " it would be very nice if you could open a Pull request for the `scheduler/scheduler_config.json`"
-                " file")
-            deprecate("steps_offset!=1",
-                      "1.0.0",
-                      deprecation_message,
-                      standard_warn=False)
-            new_config = dict(scheduler.config)
-            new_config["steps_offset"] = 1
-            scheduler._internal_dict = FrozenDict(new_config)
-
-        if safety_checker is None:
+        if safety_checker is None and requires_safety_checker:
             logger.warn(
                 f"You have disabled the safety checker for {self.__class__} by passing `safety_checker=None`. Ensure"
                 " that you abide to the conditions of the Stable Diffusion license and do not expose unfiltered"
-                " results in services or applications open to the public. PaddleNLP team, diffusers team and Hugging Face"
+                " results in services or applications open to the public. Both the diffusers team and Hugging Face"
                 " strongly recommend to keep the safety filter enabled in all public facing circumstances, disabling"
                 " it only for use-cases that involve analyzing network behavior or auditing its results. For more"
                 " information, please have a look at https://github.com/huggingface/diffusers/pull/254 ."
             )
-
+        if safety_checker is not None and feature_extractor is None:
+            raise ValueError(
+                "Make sure to define a feature extractor when loading {self.__class__} if you want to use the safety"
+                " checker. If you do not want to use the safety checker, you can pass `'safety_checker=None'` instead."
+            )
+        is_unet_version_less_0_9_0 = hasattr(unet.config, "_ppdiffusers_version") and version.parse(
+            version.parse(unet.config._ppdiffusers_version).base_version
+        ) < version.parse("0.9.0.dev0")
+        is_unet_sample_size_less_64 = hasattr(unet.config, "sample_size") and unet.config.sample_size < 64
+        if is_unet_version_less_0_9_0 and is_unet_sample_size_less_64:
+            deprecation_message = (
+                "The configuration file of the unet has set the default `sample_size` to smaller than"
+                " 64 which seems highly unlikely .If you're checkpoint is a fine-tuned version of any of the"
+                " following: \n- CompVis/stable-diffusion-v1-4 \n- CompVis/stable-diffusion-v1-3 \n-"
+                " CompVis/stable-diffusion-v1-2 \n- CompVis/stable-diffusion-v1-1 \n- runwayml/stable-diffusion-v1-5"
+                " \n- runwayml/stable-diffusion-inpainting \n you should change 'sample_size' to 64 in the"
+                " configuration file. Please make sure to update the config accordingly as leaving `sample_size=32`"
+                " in the config might lead to incorrect results in future versions. If you have downloaded this"
+                " checkpoint from the Hugging Face Hub, it would be very nice if you could open a Pull request for"
+                " the `unet/config.json` file"
+            )
+            deprecate("sample_size<64", "1.0.0", deprecation_message, standard_warn=False)
+            new_config = dict(unet.config)
+            new_config["sample_size"] = 64
+            unet._internal_dict = FrozenDict(new_config)
         self.register_modules(
             vae=vae,
-            text_encoder=text_encoder,
-            tokenizer=tokenizer,
+            image_encoder=image_encoder,
             unet=unet,
             scheduler=scheduler,
             safety_checker=safety_checker,
             feature_extractor=feature_extractor,
         )
+        self.vae_scale_factor = 2 ** (len(self.vae.config.block_out_channels) - 1)
+        self.register_to_config(requires_safety_checker=requires_safety_checker)
 
-    def enable_attention_slicing(self,
-                                 slice_size: Optional[Union[str,
-                                                            int]] = "auto"):
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.enable_attention_slicing
+    def enable_attention_slicing(self, slice_size: Optional[Union[str, int]] = "auto"):
         r"""
         Enable sliced attention computation.
 
         When this option is enabled, the attention module will split the input tensor in slices, to compute attention
         in several steps. This is useful to save some memory in exchange for a small speed decrease.
 
         Args:
             slice_size (`str` or `int`, *optional*, defaults to `"auto"`):
                 When `"auto"`, halves the input to the attention heads, so attention will be computed in two steps. If
                 a number is provided, uses as many slices as `attention_head_dim // slice_size`. In this case,
                 `attention_head_dim` must be a multiple of `slice_size`.
         """
         if slice_size == "auto":
-            # half the attention head size is usually a good trade-off between
-            # speed and memory
-            slice_size = self.unet.config.attention_head_dim // 2
+            if isinstance(self.unet.config.attention_head_dim, int):
+                # half the attention head size is usually a good trade-off between
+                # speed and memory
+                slice_size = self.unet.config.attention_head_dim // 2
+            else:
+                # if `attention_head_dim` is a list, take the smallest head size
+                slice_size = min(self.unet.config.attention_head_dim)
         self.unet.set_attention_slice(slice_size)
 
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.disable_attention_slicing
     def disable_attention_slicing(self):
         r"""
         Disable sliced attention computation. If `enable_attention_slicing` was previously invoked, this method will go
         back to computing attention in one step.
         """
-        # set slice_size = `None` to disable `set_attention_slice`
+        # set slice_size = `None` to disable `attention slicing`
         self.enable_attention_slicing(None)
 
+    def _encode_image(self, image, num_images_per_prompt, do_classifier_free_guidance):
+        dtype = self.image_encoder.dtype
+
+        if not isinstance(image, paddle.Tensor):
+            image = self.feature_extractor(images=image, return_tensors="pd").pixel_values
+
+        image = image.cast(dtype)
+        image_embeddings = self.image_encoder(image, return_dict=True).image_embeds
+        image_embeddings = image_embeddings.unsqueeze(1)
+
+        # duplicate image embeddings for each generation per prompt, using mps friendly method
+        bs_embed, seq_len, _ = image_embeddings.shape
+        image_embeddings = image_embeddings.tile([1, num_images_per_prompt, 1])
+        image_embeddings = image_embeddings.reshape([bs_embed * num_images_per_prompt, seq_len, -1])
+
+        if do_classifier_free_guidance:
+            uncond_embeddings = paddle.zeros_like(image_embeddings)
+
+            # For classifier free guidance, we need to do two forward passes.
+            # Here we concatenate the unconditional and text embeddings into a single batch
+            # to avoid doing two forward passes
+            image_embeddings = paddle.concat([uncond_embeddings, image_embeddings])
+
+        return image_embeddings
+
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.run_safety_checker
+    def run_safety_checker(self, image, dtype):
+        if self.safety_checker is not None:
+            safety_checker_input = self.feature_extractor(self.numpy_to_pil(image), return_tensors="pd")
+            image, has_nsfw_concept = self.safety_checker(
+                images=image, clip_input=safety_checker_input.pixel_values.cast(dtype)
+            )
+        else:
+            has_nsfw_concept = None
+        return image, has_nsfw_concept
+
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.decode_latents
+    def decode_latents(self, latents):
+        latents = 1 / 0.18215 * latents
+        image = self.vae.decode(latents).sample
+        image = (image / 2 + 0.5).clip(0, 1)
+        # we always cast to float32 as this does not cause significant overhead and is compatible with bfloa16
+        image = image.transpose([0, 2, 3, 1]).cast("float32").numpy()
+        return image
+
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.prepare_extra_step_kwargs
+    def prepare_extra_step_kwargs(self, generator, eta):
+        # prepare extra kwargs for the scheduler step, since not all schedulers have the same signature
+        # eta (η) is only used with the DDIMScheduler, it will be ignored for other schedulers.
+        # eta corresponds to η in DDIM paper: https://arxiv.org/abs/2010.02502
+        # and should be between [0, 1]
+
+        accepts_eta = "eta" in set(inspect.signature(self.scheduler.step).parameters.keys())
+        extra_step_kwargs = {}
+        if accepts_eta:
+            extra_step_kwargs["eta"] = eta
+
+        # check if the scheduler accepts generator
+        accepts_generator = "generator" in set(inspect.signature(self.scheduler.step).parameters.keys())
+        if accepts_generator:
+            extra_step_kwargs["generator"] = generator
+        return extra_step_kwargs
+
+    def check_inputs(self, image, height, width, callback_steps):
+        if (
+            not isinstance(image, paddle.Tensor)
+            and not isinstance(image, PIL.Image.Image)
+            and not isinstance(image, list)
+        ):
+            raise ValueError(
+                f"`image` has to be of type `paddle.Tensor` or `PIL.Image.Image` or `list` but is {type(image)}"
+            )
+
+        if height % 8 != 0 or width % 8 != 0:
+            raise ValueError(f"`height` and `width` have to be divisible by 8 but are {height} and {width}.")
+
+        if (callback_steps is None) or (
+            callback_steps is not None and (not isinstance(callback_steps, int) or callback_steps <= 0)
+        ):
+            raise ValueError(
+                f"`callback_steps` has to be a positive integer but is {callback_steps} of type"
+                f" {type(callback_steps)}."
+            )
+
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.prepare_latents
+    def prepare_latents(self, batch_size, num_channels_latents, height, width, dtype, generator, latents=None):
+        shape = [batch_size, num_channels_latents, height // self.vae_scale_factor, width // self.vae_scale_factor]
+        if latents is None:
+            latents = paddle.randn(shape, generator=generator, dtype=dtype)
+        else:
+            if latents.shape != shape:
+                raise ValueError(f"Unexpected latents shape, got {latents.shape}, expected {shape}")
+
+        # scale the initial noise by the standard deviation required by the scheduler
+        latents = latents * self.scheduler.init_noise_sigma
+        return latents
+
     @paddle.no_grad()
     def __call__(
         self,
-        prompt: Union[str, List[str]],
-        init_image: Union[paddle.Tensor, PIL.Image.Image],
-        strength: float = 0.8,
-        num_inference_steps: Optional[int] = 50,
-        guidance_scale: Optional[float] = 7.5,
-        negative_prompt: Optional[Union[str, List[str]]] = None,
+        image: Union[PIL.Image.Image, List[PIL.Image.Image], paddle.Tensor],
+        height: Optional[int] = None,
+        width: Optional[int] = None,
+        num_inference_steps: int = 50,
+        guidance_scale: float = 7.5,
         num_images_per_prompt: Optional[int] = 1,
-        eta: Optional[float] = 0.0,
-        seed: Optional[int] = None,
+        eta: float = 0.0,
+        generator: Optional[paddle.Generator] = None,
+        latents: Optional[paddle.Tensor] = None,
         output_type: Optional[str] = "pil",
         return_dict: bool = True,
         callback: Optional[Callable[[int, int, paddle.Tensor], None]] = None,
         callback_steps: Optional[int] = 1,
-        **kwargs,
     ):
         r"""
         Function invoked when calling the pipeline for generation.
 
         Args:
-            prompt (`str` or `List[str]`):
-                The prompt or prompts to guide the image generation.
-            init_image (`paddle.Tensor` or `PIL.Image.Image`):
-                `Image`, or tensor representing an image batch, that will be used as the starting point for the
-                process.
-            strength (`float`, *optional*, defaults to 0.8):
-                Conceptually, indicates how much to transform the reference `init_image`. Must be between 0 and 1.
-                `init_image` will be used as a starting point, adding more noise to it the larger the `strength`. The
-                number of denoising steps depends on the amount of noise initially added. When `strength` is 1, added
-                noise will be maximum and the denoising process will run for the full number of iterations specified in
-                `num_inference_steps`. A value of 1, therefore, essentially ignores `init_image`.
+            image (`PIL.Image.Image` or `List[PIL.Image.Image]` or `paddle.Tensor`):
+                The image or images to guide the image generation. If you provide a tensor, it needs to comply with the
+                configuration of
+                [this](https://huggingface.co/lambdalabs/sd-image-variations-diffusers/blob/main/feature_extractor/preprocessor_config.json)
+                `CLIPFeatureExtractor`
+            height (`int`, *optional*, defaults to self.unet.config.sample_size * self.vae_scale_factor):
+                The height in pixels of the generated image.
+            width (`int`, *optional*, defaults to self.unet.config.sample_size * self.vae_scale_factor):
+                The width in pixels of the generated image.
             num_inference_steps (`int`, *optional*, defaults to 50):
                 The number of denoising steps. More denoising steps usually lead to a higher quality image at the
-                expense of slower inference. This parameter will be modulated by `strength`.
+                expense of slower inference.
             guidance_scale (`float`, *optional*, defaults to 7.5):
                 Guidance scale as defined in [Classifier-Free Diffusion Guidance](https://arxiv.org/abs/2207.12598).
                 `guidance_scale` is defined as `w` of equation 2. of [Imagen
                 Paper](https://arxiv.org/pdf/2205.11487.pdf). Guidance scale is enabled by setting `guidance_scale >
                 1`. Higher guidance scale encourages to generate images that are closely linked to the text `prompt`,
                 usually at the expense of lower image quality.
-            negative_prompt (`str` or `List[str]`, *optional*):
-                The prompt or prompts not to guide the image generation. Ignored when not using guidance (i.e., ignored
-                if `guidance_scale` is less than `1`).
             num_images_per_prompt (`int`, *optional*, defaults to 1):
                 The number of images to generate per prompt.
             eta (`float`, *optional*, defaults to 0.0):
                 Corresponds to parameter eta (η) in the DDIM paper: https://arxiv.org/abs/2010.02502. Only applies to
                 [`schedulers.DDIMScheduler`], will be ignored for others.
-            seed (`int`, *optional*):
-                A random seed.
+            generator (`paddle.Generator`, *optional*):
+                A [paddle generator] to make generation
+                deterministic.
+            latents (`paddle.Tensor`, *optional*):
+                Pre-generated noisy latents, sampled from a Gaussian distribution, to be used as inputs for image
+                generation. Can be used to tweak the same generation with different prompts. If not provided, a latents
+                tensor will ge generated by sampling using the supplied random `generator`.
             output_type (`str`, *optional*, defaults to `"pil"`):
                 The output format of the generate image. Choose between
                 [PIL](https://pillow.readthedocs.io/en/stable/): `PIL.Image.Image` or `np.array`.
             return_dict (`bool`, *optional*, defaults to `True`):
                 Whether or not to return a [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] instead of a
                 plain tuple.
             callback (`Callable`, *optional*):
@@ -224,224 +327,87 @@
         Returns:
             [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] or `tuple`:
             [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] if `return_dict` is True, otherwise a `tuple.
             When returning a tuple, the first element is a list with the generated images, and the second element is a
             list of `bool`s denoting whether the corresponding generated image likely represents "not-safe-for-work"
             (nsfw) content, according to the `safety_checker`.
         """
-        if isinstance(prompt, str):
-            batch_size = 1
-        elif isinstance(prompt, list):
-            batch_size = len(prompt)
-        else:
-            raise ValueError(
-                f"`prompt` has to be of type `str` or `list` but is {type(prompt)}"
-            )
+        # 0. Default height and width to unet
+        height = height or self.unet.config.sample_size * self.vae_scale_factor
+        width = width or self.unet.config.sample_size * self.vae_scale_factor
 
-        if strength < 0 or strength > 1:
-            raise ValueError(
-                f"The value of strength should in [0.0, 1.0] but is {strength}")
-
-        if (callback_steps is None) or (callback_steps is not None and
-                                        (not isinstance(callback_steps, int)
-                                         or callback_steps <= 0)):
-            raise ValueError(
-                f"`callback_steps` has to be a positive integer but is {callback_steps} of type"
-                f" {type(callback_steps)}.")
-
-        # set timesteps
-        self.scheduler.set_timesteps(num_inference_steps)
-
-        if isinstance(init_image, PIL.Image.Image):
-            init_image = preprocess(init_image)
-
-        # get prompt text embeddings
-        text_inputs = self.tokenizer(
-            prompt,
-            padding="max_length",
-            max_length=self.tokenizer.model_max_length,
-            return_tensors="pd",
-        )
-        text_input_ids = text_inputs.input_ids
-
-        if text_input_ids.shape[-1] > self.tokenizer.model_max_length:
-            removed_text = self.tokenizer.batch_decode(
-                text_input_ids[:, self.tokenizer.model_max_length:])
-            logger.warning(
-                "The following part of your input was truncated because CLIP can only handle sequences up to"
-                f" {self.tokenizer.model_max_length} tokens: {removed_text}")
-            text_input_ids = text_input_ids[:, :self.tokenizer.model_max_length]
-        attention_mask = paddle.ones_like(text_input_ids)
-        text_embeddings = self.text_encoder(text_input_ids,
-                                            attention_mask=attention_mask)[0]
-
-        # duplicate text embeddings for each generation per prompt, using mps friendly method
-        bs_embed, seq_len, _ = text_embeddings.shape
-        text_embeddings = text_embeddings.tile([1, num_images_per_prompt, 1])
-        text_embeddings = text_embeddings.reshape(
-            [bs_embed * num_images_per_prompt, seq_len, -1])
+        # 1. Check inputs. Raise error if not correct
+        self.check_inputs(image, height, width, callback_steps)
 
+        # 2. Define call parameters
+        if isinstance(image, PIL.Image.Image):
+            batch_size = 1
+        elif isinstance(image, list):
+            batch_size = len(image)
+        else:
+            batch_size = image.shape[0]
         # here `guidance_scale` is defined analog to the guidance weight `w` of equation (2)
         # of the Imagen paper: https://arxiv.org/pdf/2205.11487.pdf . `guidance_scale = 1`
         # corresponds to doing no classifier free guidance.
         do_classifier_free_guidance = guidance_scale > 1.0
-        # get unconditional embeddings for classifier free guidance
-        if do_classifier_free_guidance:
-            uncond_tokens: List[str]
-            if negative_prompt is None:
-                uncond_tokens = [""]
-            elif type(prompt) is not type(negative_prompt):
-                raise TypeError(
-                    f"`negative_prompt` should be the same type to `prompt`, but got {type(negative_prompt)} !="
-                    f" {type(prompt)}.")
-            elif isinstance(negative_prompt, str):
-                uncond_tokens = [negative_prompt]
-            elif batch_size != len(negative_prompt):
-                raise ValueError(
-                    "The length of `negative_prompt` should be equal to batch_size."
-                )
-            else:
-                uncond_tokens = negative_prompt
-
-            max_length = text_input_ids.shape[-1]
-            uncond_input = self.tokenizer(
-                uncond_tokens,
-                padding="max_length",
-                max_length=max_length,
-                truncation=True,
-                return_tensors="pd",
-            )
-            attention_mask = paddle.ones_like(uncond_input.input_ids)
-            uncond_embeddings = self.text_encoder(
-                uncond_input.input_ids, attention_mask=attention_mask)[0]
-
-            # duplicate unconditional embeddings for each generation per prompt, using mps friendly method
-            seq_len = uncond_embeddings.shape[1]
-            uncond_embeddings = uncond_embeddings.tile(
-                [batch_size, num_images_per_prompt, 1])
-            uncond_embeddings = uncond_embeddings.reshape(
-                [batch_size * num_images_per_prompt, seq_len, -1])
-
-            # For classifier free guidance, we need to do two forward passes.
-            # Here we concatenate the unconditional and text embeddings into a single batch
-            # to avoid doing two forward passes
-            text_embeddings = paddle.concat(
-                [uncond_embeddings, text_embeddings])
 
-        # encode the init image into latents and scale the latents
-        latents_dtype = text_embeddings.dtype
-        init_image = init_image.astype(latents_dtype)
-        init_latent_dist = self.vae.encode(init_image).latent_dist
-        init_latents = init_latent_dist.sample()
-        init_latents = 0.18215 * init_latents
-
-        if isinstance(prompt, str):
-            prompt = [prompt]
-        if len(prompt) > init_latents.shape[0] and len(
-                prompt) % init_latents.shape[0] == 0:
-            # expand init_latents for batch_size
-            deprecation_message = (
-                f"You have passed {len(prompt)} text prompts (`prompt`), but only {init_latents.shape[0]} initial"
-                " images (`init_image`). Initial images are now duplicating to match the number of text prompts. Note"
-                " that this behavior is deprecated is will be removed in a version 1.0.0. Please make sure to update"
-                " your script to pass as many init images as text prompts to suppress this warning."
-            )
-            deprecate("len(prompt) != len(init_image)",
-                      "1.0.0",
-                      deprecation_message,
-                      standard_warn=False)
-            additional_image_per_prompt = len(prompt) // init_latents.shape[0]
-            init_latents = paddle.concat([init_latents] *
-                                         additional_image_per_prompt *
-                                         num_images_per_prompt)
-        elif len(prompt) > init_latents.shape[0] and len(
-                prompt) % init_latents.shape[0] != 0:
-            raise ValueError(
-                f"Cannot duplicate `init_image` of batch size {init_latents.shape[0]} to {len(prompt)} text prompts."
-            )
-        else:
-            init_latents = paddle.concat([init_latents] * num_images_per_prompt)
+        # 3. Encode input image
+        image_embeddings = self._encode_image(image, num_images_per_prompt, do_classifier_free_guidance)
 
-        # get the original timestep using init_timestep
-        offset = self.scheduler.config.get("steps_offset", 0)
-        init_timestep = int(num_inference_steps * strength) + offset
-        init_timestep = min(init_timestep, num_inference_steps)
+        # 4. Prepare timesteps
+        self.scheduler.set_timesteps(num_inference_steps)
+        timesteps = self.scheduler.timesteps
 
-        timesteps = self.scheduler.timesteps[-init_timestep]
-        timesteps = timesteps.tile([
+        # 5. Prepare latent variables
+        num_channels_latents = self.unet.in_channels
+        latents = self.prepare_latents(
             batch_size * num_images_per_prompt,
-        ])
-
-        if seed is not None:
-            paddle.seed(seed)
-        # add noise to latents using the timesteps
-        noise = paddle.randn(init_latents.shape, dtype=latents_dtype)
-        init_latents = self.scheduler.add_noise(init_latents, noise, timesteps)
-
-        # prepare extra kwargs for the scheduler step, since not all schedulers have the same signature
-        # eta (η) is only used with the DDIMScheduler, it will be ignored for other schedulers.
-        # eta corresponds to η in DDIM paper: https://arxiv.org/abs/2010.02502
-        # and should be between [0, 1]
-        accepts_eta = "eta" in set(
-            inspect.signature(self.scheduler.step).parameters.keys())
-        extra_step_kwargs = {}
-        if accepts_eta:
-            extra_step_kwargs["eta"] = eta
-
-        latents = init_latents
-
-        t_start = max(num_inference_steps - init_timestep + offset, 0)
+            num_channels_latents,
+            height,
+            width,
+            image_embeddings.dtype,
+            generator,
+            latents,
+        )
 
-        # Some schedulers like PNDM have timesteps as arrays
-        # It's more optimized to move all timesteps to correct device beforehand
-        timesteps = self.scheduler.timesteps[t_start:]
-
-        for i, t in enumerate(self.progress_bar(timesteps)):
-            # expand the latents if we are doing classifier free guidance
-            latent_model_input = paddle.concat(
-                [latents] * 2) if do_classifier_free_guidance else latents
-            latent_model_input = self.scheduler.scale_model_input(
-                latent_model_input, t)
-
-            # predict the noise residual
-            noise_pred = self.unet(latent_model_input,
-                                   t,
-                                   encoder_hidden_states=text_embeddings).sample
-
-            # perform guidance
-            if do_classifier_free_guidance:
-                noise_pred_uncond, noise_pred_text = noise_pred.chunk(2)
-                noise_pred = noise_pred_uncond + guidance_scale * (
-                    noise_pred_text - noise_pred_uncond)
-
-            # compute the previous noisy sample x_t -> x_t-1
-            latents = self.scheduler.step(noise_pred, t, latents,
-                                          **extra_step_kwargs).prev_sample
-
-            # call the callback, if provided
-            if callback is not None and i % callback_steps == 0:
-                callback(i, t, latents)
+        # 6. Prepare extra step kwargs. TODO: Logic should ideally just be moved out of the pipeline
+        extra_step_kwargs = self.prepare_extra_step_kwargs(generator, eta)
 
-        latents = 1 / 0.18215 * latents
-        image = self.vae.decode(latents).sample
+        # 7. Denoising loop
+        num_warmup_steps = len(timesteps) - num_inference_steps * self.scheduler.order
+        with self.progress_bar(total=num_inference_steps) as progress_bar:
+            for i, t in enumerate(timesteps):
+                # expand the latents if we are doing classifier free guidance
+                latent_model_input = paddle.concat([latents] * 2) if do_classifier_free_guidance else latents
+                latent_model_input = self.scheduler.scale_model_input(latent_model_input, t)
+
+                # predict the noise residual
+                noise_pred = self.unet(latent_model_input, t, encoder_hidden_states=image_embeddings).sample
+
+                # perform guidance
+                if do_classifier_free_guidance:
+                    noise_pred_uncond, noise_pred_text = noise_pred.chunk(2)
+                    noise_pred = noise_pred_uncond + guidance_scale * (noise_pred_text - noise_pred_uncond)
+
+                # compute the previous noisy sample x_t -> x_t-1
+                latents = self.scheduler.step(noise_pred, t, latents, **extra_step_kwargs).prev_sample
+
+                # call the callback, if provided
+                if i == len(timesteps) - 1 or ((i + 1) > num_warmup_steps and (i + 1) % self.scheduler.order == 0):
+                    progress_bar.update()
+                    if callback is not None and i % callback_steps == 0:
+                        callback(i, t, latents)
 
-        image = (image / 2 + 0.5).clip(0, 1)
-        image = image.transpose([0, 2, 3, 1]).numpy()
+        # 8. Post-processing
+        image = self.decode_latents(latents)
 
-        if self.safety_checker is not None:
-            safety_checker_input = self.feature_extractor(
-                self.numpy_to_pil(image), return_tensors="pd")
-            image, has_nsfw_concept = self.safety_checker(
-                images=image,
-                clip_input=safety_checker_input.pixel_values.astype(
-                    text_embeddings.dtype))
-        else:
-            has_nsfw_concept = None
+        # 9. Run safety checker
+        image, has_nsfw_concept = self.run_safety_checker(image, image_embeddings.dtype)
 
+        # 10. Convert to PIL
         if output_type == "pil":
             image = self.numpy_to_pil(image)
 
         if not return_dict:
             return (image, has_nsfw_concept)
 
-        return StableDiffusionPipelineOutput(
-            images=image, nsfw_content_detected=has_nsfw_concept)
+        return StableDiffusionPipelineOutput(images=image, nsfw_content_detected=has_nsfw_concept)
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_inpaint.py` & `ppdiffusers-0.9.0/ppdiffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_upscale.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,287 +14,187 @@
 # limitations under the License.
 
 import inspect
 from typing import Callable, List, Optional, Union
 
 import numpy as np
 import paddle
-import paddle.nn.functional as F
 import PIL
 
-from paddlenlp.utils.tools import compare_version
+from paddlenlp.transformers import CLIPTextModel, CLIPTokenizer
 
-if compare_version(PIL.__version__, "9.1.0") >= 0:
-    Resampling = PIL.Image.Resampling
-else:
-    Resampling = PIL.Image
-from paddlenlp.transformers import CLIPFeatureExtractor, CLIPTextModel, CLIPTokenizer
-
-from ...configuration_utils import FrozenDict
 from ...models import AutoencoderKL, UNet2DConditionModel
-from ...pipeline_utils import DiffusionPipeline
+from ...pipeline_utils import DiffusionPipeline, ImagePipelineOutput
 from ...schedulers import (
     DDIMScheduler,
-    EulerAncestralDiscreteScheduler,
+    DDPMScheduler,
     LMSDiscreteScheduler,
     PNDMScheduler,
 )
-from ...utils import deprecate, logging
-from . import StableDiffusionPipelineOutput
-from .safety_checker import StableDiffusionSafetyChecker
+from ...utils import logging
 
 logger = logging.get_logger(__name__)  # pylint: disable=invalid-name
 
 
-def prepare_mask_and_masked_image(image, mask):
+def preprocess(image):
+    # resize to multiple of 64
+    width, height = image.size
+    width = width - width % 64
+    height = height - height % 64
+    image = image.resize((width, height))
+
     image = np.array(image.convert("RGB"))
     image = image[None].transpose(0, 3, 1, 2)
-    image = paddle.to_tensor(image, dtype="float32") / 127.5 - 1.0
-
-    mask = np.array(mask.convert("L"))
-    mask = mask.astype(np.float32) / 255.0
-    mask = mask[None, None]
-    mask[mask < 0.5] = 0
-    mask[mask >= 0.5] = 1
-    mask = paddle.to_tensor(mask)
-
-    masked_image = image * (mask < 0.5)
+    image = paddle.to_tensor(image).cast("float32") / 127.5 - 1.0
+    return image
 
-    return mask, masked_image
 
-
-class StableDiffusionInpaintPipeline(DiffusionPipeline):
+class StableDiffusionUpscalePipeline(DiffusionPipeline):
     r"""
-    Pipeline for text-guided image inpainting using Stable Diffusion. *This is an experimental feature*.
+    Pipeline for text-guided image super-resolution using Stable Diffusion 2.
+
     This model inherits from [`DiffusionPipeline`]. Check the superclass documentation for the generic methods the
-    library implements for all the pipelines (such as downloading or saving, running on a particular device, etc.)
+    library implements for all the pipelines (such as downloading or saving etc.)
+
     Args:
         vae ([`AutoencoderKL`]):
             Variational Auto-Encoder (VAE) Model to encode and decode images to and from latent representations.
         text_encoder ([`CLIPTextModel`]):
             Frozen text-encoder. Stable Diffusion uses the text portion of
             [CLIP](https://huggingface.co/docs/transformers/model_doc/clip#transformers.CLIPTextModel), specifically
             the [clip-vit-large-patch14](https://huggingface.co/openai/clip-vit-large-patch14) variant.
         tokenizer (`CLIPTokenizer`):
             Tokenizer of class
             [CLIPTokenizer](https://huggingface.co/docs/transformers/v4.21.0/en/model_doc/clip#transformers.CLIPTokenizer).
         unet ([`UNet2DConditionModel`]): Conditional U-Net architecture to denoise the encoded image latents.
+        low_res_scheduler ([`SchedulerMixin`]):
+            A scheduler used to add initial noise to the low res conditioning image. It must be an instance of
+            [`DDPMScheduler`].
         scheduler ([`SchedulerMixin`]):
-            A scheduler to be used in combination with `unet` to denoise the encoded image latens. Can be one of
+            A scheduler to be used in combination with `unet` to denoise the encoded image latents. Can be one of
             [`DDIMScheduler`], [`LMSDiscreteScheduler`], or [`PNDMScheduler`].
-        safety_checker ([`StableDiffusionSafetyChecker`]):
-            Classification module that estimates whether generated images could be considered offensive or harmful.
-            Please, refer to the [model card](https://huggingface.co/runwayml/stable-diffusion-v1-5) for details.
-        feature_extractor ([`CLIPFeatureExtractor`]):
-            Model that extracts features from generated images to be used as inputs for the `safety_checker`.
     """
 
     def __init__(
         self,
         vae: AutoencoderKL,
         text_encoder: CLIPTextModel,
         tokenizer: CLIPTokenizer,
         unet: UNet2DConditionModel,
-        scheduler: Union[DDIMScheduler, PNDMScheduler, LMSDiscreteScheduler, EulerAncestralDiscreteScheduler],
-        safety_checker: StableDiffusionSafetyChecker,
-        feature_extractor: CLIPFeatureExtractor,
+        low_res_scheduler: DDPMScheduler,
+        scheduler: Union[DDIMScheduler, PNDMScheduler, LMSDiscreteScheduler],
+        max_noise_level: int = 350,
     ):
         super().__init__()
 
-        if hasattr(scheduler.config, "steps_offset") and scheduler.config.steps_offset != 1:
-            deprecation_message = (
-                f"The configuration file of this scheduler: {scheduler} is outdated. `steps_offset`"
-                f" should be set to 1 instead of {scheduler.config.steps_offset}. Please make sure "
-                "to update the config accordingly as leaving `steps_offset` might led to incorrect results"
-                " in future versions. If you have downloaded this checkpoint from the Hugging Face Hub,"
-                " it would be very nice if you could open a Pull request for the `scheduler/scheduler_config.json`"
-                " file"
-            )
-            deprecate("steps_offset!=1", "1.0.0", deprecation_message, standard_warn=False)
-            new_config = dict(scheduler.config)
-            new_config["steps_offset"] = 1
-            scheduler._internal_dict = FrozenDict(new_config)
-
-        if safety_checker is None:
-            logger.warn(
-                f"You have disabled the safety checker for {self.__class__} by passing `safety_checker=None`. Ensure"
-                " that you abide to the conditions of the Stable Diffusion license and do not expose unfiltered"
-                " results in services or applications open to the public. PaddleNLP team, diffusers team and Hugging Face"
-                " strongly recommend to keep the safety filter enabled in all public facing circumstances, disabling"
-                " it only for use-cases that involve analyzing network behavior or auditing its results. For more"
-                " information, please have a look at https://github.com/huggingface/diffusers/pull/254 ."
-            )
-
         self.register_modules(
             vae=vae,
             text_encoder=text_encoder,
             tokenizer=tokenizer,
             unet=unet,
+            low_res_scheduler=low_res_scheduler,
             scheduler=scheduler,
-            safety_checker=safety_checker,
-            feature_extractor=feature_extractor,
         )
+        self.register_to_config(max_noise_level=max_noise_level)
 
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.enable_attention_slicing
     def enable_attention_slicing(self, slice_size: Optional[Union[str, int]] = "auto"):
         r"""
         Enable sliced attention computation.
+
         When this option is enabled, the attention module will split the input tensor in slices, to compute attention
         in several steps. This is useful to save some memory in exchange for a small speed decrease.
+
         Args:
             slice_size (`str` or `int`, *optional*, defaults to `"auto"`):
                 When `"auto"`, halves the input to the attention heads, so attention will be computed in two steps. If
                 a number is provided, uses as many slices as `attention_head_dim // slice_size`. In this case,
                 `attention_head_dim` must be a multiple of `slice_size`.
         """
         if slice_size == "auto":
-            # half the attention head size is usually a good trade-off between
-            # speed and memory
-            slice_size = self.unet.config.attention_head_dim // 2
+            if isinstance(self.unet.config.attention_head_dim, int):
+                # half the attention head size is usually a good trade-off between
+                # speed and memory
+                slice_size = self.unet.config.attention_head_dim // 2
+            else:
+                # if `attention_head_dim` is a list, take the smallest head size
+                slice_size = min(self.unet.config.attention_head_dim)
+
         self.unet.set_attention_slice(slice_size)
 
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.disable_attention_slicing
     def disable_attention_slicing(self):
         r"""
         Disable sliced attention computation. If `enable_attention_slicing` was previously invoked, this method will go
         back to computing attention in one step.
         """
         # set slice_size = `None` to disable `attention slicing`
         self.enable_attention_slicing(None)
 
-    @paddle.no_grad()
-    def __call__(
-        self,
-        prompt: Union[str, List[str]],
-        image: Union[paddle.Tensor, PIL.Image.Image],
-        mask_image: Union[paddle.Tensor, PIL.Image.Image],
-        height: int = 512,
-        width: int = 512,
-        num_inference_steps: int = 50,
-        guidance_scale: float = 7.5,
-        negative_prompt: Optional[Union[str, List[str]]] = None,
-        num_images_per_prompt: Optional[int] = 1,
-        eta: float = 0.0,
-        seed: Optional[int] = None,
-        latents: Optional[paddle.Tensor] = None,
-        output_type: Optional[str] = "pil",
-        return_dict: bool = True,
-        callback: Optional[Callable[[int, int, paddle.Tensor], None]] = None,
-        callback_steps: Optional[int] = 1,
-        **kwargs,
-    ):
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline._encode_prompt
+    def _encode_prompt(self, prompt, num_images_per_prompt, do_classifier_free_guidance, negative_prompt):
         r"""
-        Function invoked when calling the pipeline for generation.
+        Encodes the prompt into text encoder hidden states.
+
         Args:
-            prompt (`str` or `List[str]`):
-                The prompt or prompts to guide the image generation.
-            image (`PIL.Image.Image`):
-                `Image`, or tensor representing an image batch which will be inpainted, *i.e.* parts of the image will
-                be masked out with `mask_image` and repainted according to `prompt`.
-            mask_image (`PIL.Image.Image`):
-                `Image`, or tensor representing an image batch, to mask `image`. White pixels in the mask will be
-                repainted, while black pixels will be preserved. If `mask_image` is a PIL image, it will be converted
-                to a single channel (luminance) before use. If it's a tensor, it should contain one color channel (L)
-                instead of 3, so the expected shape would be `(B, H, W, 1)`.
-            height (`int`, *optional*, defaults to 512):
-                The height in pixels of the generated image.
-            width (`int`, *optional*, defaults to 512):
-                The width in pixels of the generated image.
-            num_inference_steps (`int`, *optional*, defaults to 50):
-                The number of denoising steps. More denoising steps usually lead to a higher quality image at the
-                expense of slower inference.
-            guidance_scale (`float`, *optional*, defaults to 7.5):
-                Guidance scale as defined in [Classifier-Free Diffusion Guidance](https://arxiv.org/abs/2207.12598).
-                `guidance_scale` is defined as `w` of equation 2. of [Imagen
-                Paper](https://arxiv.org/pdf/2205.11487.pdf). Guidance scale is enabled by setting `guidance_scale >
-                1`. Higher guidance scale encourages to generate images that are closely linked to the text `prompt`,
-                usually at the expense of lower image quality.
-            negative_prompt (`str` or `List[str]`, *optional*):
+            prompt (`str` or `list(int)`):
+                prompt to be encoded
+            num_images_per_prompt (`int`):
+                number of images that should be generated per prompt
+            do_classifier_free_guidance (`bool`):
+                whether to use classifier free guidance or not
+            negative_prompt (`str` or `List[str]`):
                 The prompt or prompts not to guide the image generation. Ignored when not using guidance (i.e., ignored
                 if `guidance_scale` is less than `1`).
-            num_images_per_prompt (`int`, *optional*, defaults to 1):
-                The number of images to generate per prompt.
-            eta (`float`, *optional*, defaults to 0.0):
-                Corresponds to parameter eta (η) in the DDIM paper: https://arxiv.org/abs/2010.02502. Only applies to
-                [`schedulers.DDIMScheduler`], will be ignored for others.
-            seed (`int`, *optional*):
-                A random seed.
-            latents (`paddle.Tensor`, *optional*):
-                Pre-generated noisy latents, sampled from a Gaussian distribution, to be used as inputs for image
-                generation. Can be used to tweak the same generation with different prompts. If not provided, a latents
-                tensor will ge generated by sampling using the supplied random `seed`.
-            output_type (`str`, *optional*, defaults to `"pil"`):
-                The output format of the generate image. Choose between
-                [PIL](https://pillow.readthedocs.io/en/stable/): `PIL.Image.Image` or `np.array`.
-            return_dict (`bool`, *optional*, defaults to `True`):
-                Whether or not to return a [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] instead of a
-                plain tuple.
-            callback (`Callable`, *optional*):
-                A function that will be called every `callback_steps` steps during inference. The function will be
-                called with the following arguments: `callback(step: int, timestep: int, latents: paddle.Tensor)`.
-            callback_steps (`int`, *optional*, defaults to 1):
-                The frequency at which the `callback` function will be called. If not specified, the callback will be
-                called at every step.
-        Returns:
-            [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] or `tuple`:
-            [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] if `return_dict` is True, otherwise a `tuple.
-            When returning a tuple, the first element is a list with the generated images, and the second element is a
-            list of `bool`s denoting whether the corresponding generated image likely represents "not-safe-for-work"
-            (nsfw) content, according to the `safety_checker`.
         """
+        batch_size = len(prompt) if isinstance(prompt, list) else 1
 
-        if isinstance(prompt, str):
-            batch_size = 1
-        elif isinstance(prompt, list):
-            batch_size = len(prompt)
-        else:
-            raise ValueError(f"`prompt` has to be of type `str` or `list` but is {type(prompt)}")
-
-        if height % 8 != 0 or width % 8 != 0:
-            raise ValueError(f"`height` and `width` have to be divisible by 8 but are {height} and {width}.")
-
-        if (callback_steps is None) or (
-            callback_steps is not None and (not isinstance(callback_steps, int) or callback_steps <= 0)
-        ):
-            raise ValueError(
-                f"`callback_steps` has to be a positive integer but is {callback_steps} of type"
-                f" {type(callback_steps)}."
-            )
-
-        # get prompt text embeddings
         text_inputs = self.tokenizer(
             prompt,
             padding="max_length",
             max_length=self.tokenizer.model_max_length,
+            truncation=True,
             return_tensors="pd",
         )
         text_input_ids = text_inputs.input_ids
+        untruncated_ids = self.tokenizer(prompt, padding="max_length", return_tensors="pd").input_ids
 
-        if text_input_ids.shape[-1] > self.tokenizer.model_max_length:
-            removed_text = self.tokenizer.batch_decode(text_input_ids[:, self.tokenizer.model_max_length :])
+        if not paddle.equal_all(text_input_ids, untruncated_ids):
+            removed_text = self.tokenizer.batch_decode(untruncated_ids[:, self.tokenizer.model_max_length - 1 : -1])
             logger.warning(
                 "The following part of your input was truncated because CLIP can only handle sequences up to"
                 f" {self.tokenizer.model_max_length} tokens: {removed_text}"
             )
-            text_input_ids = text_input_ids[:, : self.tokenizer.model_max_length]
-        attention_mask = paddle.ones_like(text_input_ids)
-        text_embeddings = self.text_encoder(text_input_ids, attention_mask=attention_mask)[0]
+
+        config = (
+            self.text_encoder.config
+            if isinstance(self.text_encoder.config, dict)
+            else self.text_encoder.config.to_dict()
+        )
+        if config.get("use_attention_mask", None) is not None and config["use_attention_mask"]:
+            attention_mask = text_inputs.attention_mask
+        else:
+            attention_mask = None
+
+        text_embeddings = self.text_encoder(
+            text_input_ids,
+            attention_mask=attention_mask,
+        )
+        text_embeddings = text_embeddings[0]
 
         # duplicate text embeddings for each generation per prompt, using mps friendly method
         bs_embed, seq_len, _ = text_embeddings.shape
         text_embeddings = text_embeddings.tile([1, num_images_per_prompt, 1])
         text_embeddings = text_embeddings.reshape([bs_embed * num_images_per_prompt, seq_len, -1])
 
-        # here `guidance_scale` is defined analog to the guidance weight `w` of equation (2)
-        # of the Imagen paper: https://arxiv.org/pdf/2205.11487.pdf . `guidance_scale = 1`
-        # corresponds to doing no classifier free guidance.
-        do_classifier_free_guidance = guidance_scale > 1.0
         # get unconditional embeddings for classifier free guidance
         if do_classifier_free_guidance:
             uncond_tokens: List[str]
             if negative_prompt is None:
-                uncond_tokens = [""]
+                uncond_tokens = [""] * batch_size
             elif type(prompt) is not type(negative_prompt):
                 raise TypeError(
                     f"`negative_prompt` should be the same type to `prompt`, but got {type(negative_prompt)} !="
                     f" {type(prompt)}."
                 )
             elif isinstance(negative_prompt, str):
                 uncond_tokens = [negative_prompt]
@@ -311,133 +211,286 @@
             uncond_input = self.tokenizer(
                 uncond_tokens,
                 padding="max_length",
                 max_length=max_length,
                 truncation=True,
                 return_tensors="pd",
             )
-            attention_mask = paddle.ones_like(uncond_input.input_ids)
-            uncond_embeddings = self.text_encoder(uncond_input.input_ids, attention_mask=attention_mask)[0]
+
+            if config.get("use_attention_mask", None) is not None and config["use_attention_mask"]:
+                attention_mask = uncond_input.attention_mask
+            else:
+                attention_mask = None
+
+            uncond_embeddings = self.text_encoder(
+                uncond_input.input_ids,
+                attention_mask=attention_mask,
+            )
+            uncond_embeddings = uncond_embeddings[0]
 
             # duplicate unconditional embeddings for each generation per prompt, using mps friendly method
             seq_len = uncond_embeddings.shape[1]
-            uncond_embeddings = uncond_embeddings.tile([batch_size, num_images_per_prompt, 1])
+            uncond_embeddings = uncond_embeddings.tile([1, num_images_per_prompt, 1])
             uncond_embeddings = uncond_embeddings.reshape([batch_size * num_images_per_prompt, seq_len, -1])
 
             # For classifier free guidance, we need to do two forward passes.
             # Here we concatenate the unconditional and text embeddings into a single batch
             # to avoid doing two forward passes
             text_embeddings = paddle.concat([uncond_embeddings, text_embeddings])
 
-        # get the initial random noise unless the user supplied it
-        # Unlike in other pipelines, latents need to be generated in the target device
-        # for 1-to-1 results reproducibility with the CompVis implementation.
-        # However this currently doesn't work in `mps`.
-        num_channels_latents = self.vae.config.latent_channels
-        latents_shape = [batch_size * num_images_per_prompt, num_channels_latents, height // 8, width // 8]
-        latents_dtype = text_embeddings.dtype
-        if latents is None:
-            if seed is not None:
-                paddle.seed(seed)
-            latents = paddle.randn(latents_shape, dtype=latents_dtype)
-        else:
-            if latents.shape != latents_shape:
-                raise ValueError(f"Unexpected latents shape, got {latents.shape}, expected {latents_shape}")
-            latents = latents
-
-        # prepare mask and masked_image
-        mask, masked_image = prepare_mask_and_masked_image(image, mask_image)
-        mask = mask.astype(dtype=text_embeddings.dtype)
-        masked_image = masked_image.astype(dtype=text_embeddings.dtype)
-
-        # resize the mask to latents shape as we concatenate the mask to the latents
-        mask = F.interpolate(mask, size=(height // 8, width // 8))
-
-        # encode the mask image into latents space so we can concatenate it to the latents
-        masked_image_latents = self.vae.encode(masked_image).latent_dist.sample()
-        masked_image_latents = 0.18215 * masked_image_latents
-
-        # duplicate mask and masked_image_latents for each generation per prompt, using mps friendly method
-        mask = mask.tile([num_images_per_prompt, 1, 1, 1])
-        masked_image_latents = masked_image_latents.tile([num_images_per_prompt, 1, 1, 1])
-
-        mask = paddle.concat([mask] * 2) if do_classifier_free_guidance else mask
-        masked_image_latents = (
-            paddle.concat([masked_image_latents] * 2) if do_classifier_free_guidance else masked_image_latents
-        )
-
-        num_channels_mask = mask.shape[1]
-        num_channels_masked_image = masked_image_latents.shape[1]
-
-        if num_channels_latents + num_channels_mask + num_channels_masked_image != self.unet.config.in_channels:
-            raise ValueError(
-                f"Incorrect configuration settings! The config of `pipeline.unet`: {self.unet.config} expects"
-                f" {self.unet.config.in_channels} but received `num_channels_latents`: {num_channels_latents} +"
-                f" `num_channels_mask`: {num_channels_mask} + `num_channels_masked_image`: {num_channels_masked_image}"
-                f" = {num_channels_latents+num_channels_masked_image+num_channels_mask}. Please verify the config of"
-                " `pipeline.unet` or your `mask_image` or `image` input."
-            )
-
-        # set timesteps
-        self.scheduler.set_timesteps(num_inference_steps)
-
-        # Some schedulers like PNDM have timesteps as arrays
-        # It's more optimized to move all timesteps to correct device beforehand
-        timesteps_tensor = self.scheduler.timesteps
-
-        # scale the initial noise by the standard deviation required by the scheduler
-        latents = latents * self.scheduler.init_noise_sigma
+        return text_embeddings
 
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.prepare_extra_step_kwargs
+    def prepare_extra_step_kwargs(self, generator, eta):
         # prepare extra kwargs for the scheduler step, since not all schedulers have the same signature
         # eta (η) is only used with the DDIMScheduler, it will be ignored for other schedulers.
         # eta corresponds to η in DDIM paper: https://arxiv.org/abs/2010.02502
         # and should be between [0, 1]
+
         accepts_eta = "eta" in set(inspect.signature(self.scheduler.step).parameters.keys())
         extra_step_kwargs = {}
         if accepts_eta:
             extra_step_kwargs["eta"] = eta
-        for i, t in enumerate(self.progress_bar(timesteps_tensor)):
-            # expand the latents if we are doing classifier free guidance
-            latent_model_input = paddle.concat([latents] * 2) if do_classifier_free_guidance else latents
-
-            # concat latents, mask, masked_image_latents in the channel dimension
-            latent_model_input = paddle.concat([latent_model_input, mask, masked_image_latents], axis=1)
-
-            latent_model_input = self.scheduler.scale_model_input(latent_model_input, t)
-
-            # predict the noise residual
-            noise_pred = self.unet(latent_model_input, t, encoder_hidden_states=text_embeddings).sample
-            # perform guidance
-            if do_classifier_free_guidance:
-                noise_pred_uncond, noise_pred_text = noise_pred.chunk(2)
-                noise_pred = noise_pred_uncond + guidance_scale * (noise_pred_text - noise_pred_uncond)
-
-            # compute the previous noisy sample x_t -> x_t-1
-            latents = self.scheduler.step(noise_pred, t, latents, **extra_step_kwargs).prev_sample
-
-            # call the callback, if provided
-            if callback is not None and i % callback_steps == 0:
-                callback(i, t, latents)
 
-        latents = 1 / 0.18215 * latents
+        # check if the scheduler accepts generator
+        accepts_generator = "generator" in set(inspect.signature(self.scheduler.step).parameters.keys())
+        if accepts_generator:
+            extra_step_kwargs["generator"] = generator
+        return extra_step_kwargs
+
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.decode_latents with 0.18215->0.08333
+    def decode_latents(self, latents):
+        latents = 1 / 0.08333 * latents
         image = self.vae.decode(latents).sample
-
         image = (image / 2 + 0.5).clip(0, 1)
-
         # we always cast to float32 as this does not cause significant overhead and is compatible with bfloa16
-        image = image.transpose([0, 2, 3, 1]).astype("float32").numpy()
+        image = image.transpose([0, 2, 3, 1]).cast("float32").numpy()
+        return image
 
-        if self.safety_checker is not None:
-            safety_checker_input = self.feature_extractor(self.numpy_to_pil(image), return_tensors="pd")
-            image, has_nsfw_concept = self.safety_checker(
-                images=image, clip_input=safety_checker_input.pixel_values.astype(text_embeddings.dtype)
+    def check_inputs(self, prompt, image, noise_level, callback_steps):
+        if not isinstance(prompt, str) and not isinstance(prompt, list):
+            raise ValueError(f"`prompt` has to be of type `str` or `list` but is {type(prompt)}")
+
+        if (
+            not isinstance(image, paddle.Tensor)
+            and not isinstance(image, PIL.Image.Image)
+            and not isinstance(image, list)
+        ):
+            raise ValueError(
+                f"`image` has to be of type `torch.Tensor`, `PIL.Image.Image` or `list` but is {type(image)}"
             )
+
+        # verify batch size of prompt and image are same if image is a list or tensor
+        if isinstance(image, list) or isinstance(image, paddle.Tensor):
+            if isinstance(prompt, str):
+                batch_size = 1
+            else:
+                batch_size = len(prompt)
+            if isinstance(image, list):
+                image_batch_size = len(image)
+            else:
+                image_batch_size = image.shape[0]
+            if batch_size != image_batch_size:
+                raise ValueError(
+                    f"`prompt` has batch size {batch_size} and `image` has batch size {image_batch_size}."
+                    " Please make sure that passed `prompt` matches the batch size of `image`."
+                )
+
+        # check noise level
+        if noise_level > self.config.max_noise_level:
+            raise ValueError(f"`noise_level` has to be <= {self.config.max_noise_level} but is {noise_level}")
+
+        if (callback_steps is None) or (
+            callback_steps is not None and (not isinstance(callback_steps, int) or callback_steps <= 0)
+        ):
+            raise ValueError(
+                f"`callback_steps` has to be a positive integer but is {callback_steps} of type"
+                f" {type(callback_steps)}."
+            )
+
+    def prepare_latents(self, batch_size, num_channels_latents, height, width, dtype, generator, latents=None):
+        shape = [batch_size, num_channels_latents, height, width]
+        if latents is None:
+            latents = paddle.randn(shape, generator=generator, dtype=dtype)
         else:
-            has_nsfw_concept = None
+            if latents.shape != shape:
+                raise ValueError(f"Unexpected latents shape, got {latents.shape}, expected {shape}")
+
+        # scale the initial noise by the standard deviation required by the scheduler
+        latents = latents * self.scheduler.init_noise_sigma
+        return latents
+
+    @paddle.no_grad()
+    def __call__(
+        self,
+        prompt: Union[str, List[str]],
+        image: Union[paddle.Tensor, PIL.Image.Image, List[PIL.Image.Image]],
+        num_inference_steps: int = 75,
+        guidance_scale: float = 9.0,
+        noise_level: int = 20,
+        negative_prompt: Optional[Union[str, List[str]]] = None,
+        num_images_per_prompt: Optional[int] = 1,
+        eta: float = 0.0,
+        generator: Optional[paddle.Generator] = None,
+        latents: Optional[paddle.Tensor] = None,
+        output_type: Optional[str] = "pil",
+        return_dict: bool = True,
+        callback: Optional[Callable[[int, int, paddle.Tensor], None]] = None,
+        callback_steps: Optional[int] = 1,
+    ):
+        r"""
+        Function invoked when calling the pipeline for generation.
+
+        Args:
+            prompt (`str` or `List[str]`):
+                The prompt or prompts to guide the image generation.
+            image (`PIL.Image.Image` or List[`PIL.Image.Image`] or `paddle.Tensor`):
+                `Image`, or tensor representing an image batch which will be upscaled. *
+            num_inference_steps (`int`, *optional*, defaults to 50):
+                The number of denoising steps. More denoising steps usually lead to a higher quality image at the
+                expense of slower inference.
+            guidance_scale (`float`, *optional*, defaults to 7.5):
+                Guidance scale as defined in [Classifier-Free Diffusion Guidance](https://arxiv.org/abs/2207.12598).
+                `guidance_scale` is defined as `w` of equation 2. of [Imagen
+                Paper](https://arxiv.org/pdf/2205.11487.pdf). Guidance scale is enabled by setting `guidance_scale >
+                1`. Higher guidance scale encourages to generate images that are closely linked to the text `prompt`,
+                usually at the expense of lower image quality.
+            negative_prompt (`str` or `List[str]`, *optional*):
+                The prompt or prompts not to guide the image generation. Ignored when not using guidance (i.e., ignored
+                if `guidance_scale` is less than `1`).
+            num_images_per_prompt (`int`, *optional*, defaults to 1):
+                The number of images to generate per prompt.
+            eta (`float`, *optional*, defaults to 0.0):
+                Corresponds to parameter eta (η) in the DDIM paper: https://arxiv.org/abs/2010.02502. Only applies to
+                [`schedulers.DDIMScheduler`], will be ignored for others.
+            generator (`paddle.Generator`, *optional*):
+                A [paddle generator] to make generation
+                deterministic.
+            latents (`paddle.Tensor`, *optional*):
+                Pre-generated noisy latents, sampled from a Gaussian distribution, to be used as inputs for image
+                generation. Can be used to tweak the same generation with different prompts. If not provided, a latents
+                tensor will ge generated by sampling using the supplied random `generator`.
+            output_type (`str`, *optional*, defaults to `"pil"`):
+                The output format of the generate image. Choose between
+                [PIL](https://pillow.readthedocs.io/en/stable/): `PIL.Image.Image` or `np.array`.
+            return_dict (`bool`, *optional*, defaults to `True`):
+                Whether or not to return a [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] instead of a
+                plain tuple.
+            callback (`Callable`, *optional*):
+                A function that will be called every `callback_steps` steps during inference. The function will be
+                called with the following arguments: `callback(step: int, timestep: int, latents: paddle.Tensor)`.
+            callback_steps (`int`, *optional*, defaults to 1):
+                The frequency at which the `callback` function will be called. If not specified, the callback will be
+                called at every step.
+
+        Returns:
+            [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] or `tuple`:
+            [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] if `return_dict` is True, otherwise a `tuple.
+            When returning a tuple, the first element is a list with the generated images, and the second element is a
+            list of `bool`s denoting whether the corresponding generated image likely represents "not-safe-for-work"
+            (nsfw) content, according to the `safety_checker`.
+        """
+
+        # 1. Check inputs
+        self.check_inputs(prompt, image, noise_level, callback_steps)
+
+        # 2. Define call parameters
+        batch_size = 1 if isinstance(prompt, str) else len(prompt)
+        # here `guidance_scale` is defined analog to the guidance weight `w` of equation (2)
+        # of the Imagen paper: https://arxiv.org/pdf/2205.11487.pdf . `guidance_scale = 1`
+        # corresponds to doing no classifier free guidance.
+        do_classifier_free_guidance = guidance_scale > 1.0
+
+        # 3. Encode input prompt
+        text_embeddings = self._encode_prompt(
+            prompt, num_images_per_prompt, do_classifier_free_guidance, negative_prompt
+        )
+
+        # 4. Preprocess image
+        image = [image] if isinstance(image, PIL.Image.Image) else image
+        if isinstance(image, list):
+            image = [preprocess(img) for img in image]
+            image = paddle.concat(image, axis=0)
+        image = image.cast(text_embeddings.dtype)
+
+        # 5. set timesteps
+        self.scheduler.set_timesteps(num_inference_steps)
+        timesteps = self.scheduler.timesteps
+
+        # 5. Add noise to image
+        noise_level = paddle.to_tensor([noise_level], dtype="int64")
+        noise = paddle.randn(image.shape, generator=generator, dtype=text_embeddings.dtype)
+        image = self.low_res_scheduler.add_noise(image, noise, noise_level)
+        batch_multiplier = 2 if do_classifier_free_guidance else 1
+        image = paddle.concat([image] * batch_multiplier * num_images_per_prompt)
+        noise_level = paddle.concat([noise_level] * image.shape[0])
+
+        # 6. Prepare latent variables
+        height, width = image.shape[2:]
+        num_channels_latents = self.vae.config.latent_channels
+        latents = self.prepare_latents(
+            batch_size * num_images_per_prompt,
+            num_channels_latents,
+            height,
+            width,
+            text_embeddings.dtype,
+            generator,
+            latents,
+        )
+
+        # 7. Check that sizes of image and latents match
+        num_channels_image = image.shape[1]
+        if num_channels_latents + num_channels_image != self.unet.config.in_channels:
+            raise ValueError(
+                f"Incorrect configuration settings! The config of `pipeline.unet`: {self.unet.config} expects"
+                f" {self.unet.config.in_channels} but received `num_channels_latents`: {num_channels_latents} +"
+                f" `num_channels_image`: {num_channels_image} "
+                f" = {num_channels_latents+num_channels_image}. Please verify the config of"
+                " `pipeline.unet` or your `image` input."
+            )
+
+        # 8. Prepare extra step kwargs. TODO: Logic should ideally just be moved out of the pipeline
+        extra_step_kwargs = self.prepare_extra_step_kwargs(generator, eta)
+
+        # 9. Denoising loop
+        num_warmup_steps = len(timesteps) - num_inference_steps * self.scheduler.order
+        with self.progress_bar(total=num_inference_steps) as progress_bar:
+            for i, t in enumerate(timesteps):
+                # expand the latents if we are doing classifier free guidance
+                latent_model_input = paddle.concat([latents] * 2) if do_classifier_free_guidance else latents
+
+                # concat latents, mask, masked_image_latents in the channel dimension
+                latent_model_input = self.scheduler.scale_model_input(latent_model_input, t)
+                latent_model_input = paddle.concat([latent_model_input, image], axis=1)
+
+                # predict the noise residual
+                noise_pred = self.unet(
+                    latent_model_input, t, encoder_hidden_states=text_embeddings, class_labels=noise_level
+                ).sample
+
+                # perform guidance
+                if do_classifier_free_guidance:
+                    noise_pred_uncond, noise_pred_text = noise_pred.chunk(2)
+                    noise_pred = noise_pred_uncond + guidance_scale * (noise_pred_text - noise_pred_uncond)
+
+                # compute the previous noisy sample x_t -> x_t-1
+                latents = self.scheduler.step(noise_pred, t, latents, **extra_step_kwargs).prev_sample
+
+                # call the callback, if provided
+                if i == len(timesteps) - 1 or ((i + 1) > num_warmup_steps and (i + 1) % self.scheduler.order == 0):
+                    progress_bar.update()
+                    if callback is not None and i % callback_steps == 0:
+                        callback(i, t, latents)
+
+        # 10. Post-processing
+        # make sure the VAE is in float32 mode, as it overflows in float16
+        # self.vae.to(dtype=paddle.float32)
+        image = self.decode_latents(latents.cast("float32"))
 
+        # 11. Convert to PIL
         if output_type == "pil":
             image = self.numpy_to_pil(image)
 
         if not return_dict:
-            return (image, has_nsfw_concept)
+            return (image,)
 
-        return StableDiffusionPipelineOutput(images=image, nsfw_content_detected=has_nsfw_concept)
+        return ImagePipelineOutput(images=image)
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_inpaint_legacy.py` & `ppdiffusers-0.9.0/ppdiffusers/pipelines/versatile_diffusion/pipeline_versatile_diffusion_image_variation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 PaddlePaddle Authors. All Rights Reserved.
+# Copyright 2022 The HuggingFace Team. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,440 +13,393 @@
 # limitations under the License.
 
 import inspect
 from typing import Callable, List, Optional, Union
 
 import numpy as np
 import paddle
-
 import PIL
-from paddlenlp.utils.tools import compare_version
-if compare_version(PIL.__version__, "9.1.0") >= 0:
-    Resampling = PIL.Image.Resampling
-else:
-    Resampling = PIL.Image
 
-from tqdm.auto import tqdm
-from paddlenlp.transformers import CLIPFeatureExtractor, CLIPTextModel, CLIPTokenizer
+from paddlenlp.transformers import CLIPFeatureExtractor, CLIPVisionModelWithProjection
 
-from ...configuration_utils import FrozenDict
 from ...models import AutoencoderKL, UNet2DConditionModel
-from ...pipeline_utils import DiffusionPipeline
-from ...schedulers import DDIMScheduler, LMSDiscreteScheduler, PNDMScheduler, EulerAncestralDiscreteScheduler
-from ...utils import deprecate, logging
-from . import StableDiffusionPipelineOutput
-from .safety_checker import StableDiffusionSafetyChecker
-
-logger = logging.get_logger(__name__)
-
-
-def preprocess_image(image):
-    w, h = image.size
-    w, h = map(lambda x: x - x % 32, (w, h))  # resize to integer multiple of 32
-    image = image.resize((w, h), resample=Resampling.LANCZOS)
-    image = np.array(image).astype(np.float32) / 255.0
-    image = image[None].transpose(0, 3, 1, 2)
-    image = paddle.to_tensor(image)
-    return 2.0 * image - 1.0
-
-
-def preprocess_mask(mask):
-    mask = mask.convert("L")
-    w, h = mask.size
-    w, h = map(lambda x: x - x % 32, (w, h))  # resize to integer multiple of 32
-    mask = mask.resize((w // 8, h // 8), resample=Resampling.NEAREST)
-    mask = np.array(mask).astype(np.float32) / 255.0
-    mask = np.tile(mask, (4, 1, 1))
-    mask = mask[None].transpose(0, 1, 2, 3)  # what does this step do?
-    mask = 1 - mask  # repaint white, keep black
-    mask = paddle.to_tensor(mask)
-    return mask
+from ...pipeline_utils import DiffusionPipeline, ImagePipelineOutput
+from ...schedulers import DDIMScheduler, LMSDiscreteScheduler, PNDMScheduler
+from ...utils import logging
+
+logger = logging.get_logger(__name__)  # pylint: disable=invalid-name
 
 
-class StableDiffusionInpaintPipelineLegacy(DiffusionPipeline):
+class VersatileDiffusionImageVariationPipeline(DiffusionPipeline):
     r"""
-    Pipeline for text-guided image inpainting using Stable Diffusion. *This is an experimental feature*.
+    Pipeline for image variation using Versatile Diffusion.
+
     This model inherits from [`DiffusionPipeline`]. Check the superclass documentation for the generic methods the
     library implements for all the pipelines (such as downloading or saving, running on a particular device, etc.)
+
     Args:
         vae ([`AutoencoderKL`]):
             Variational Auto-Encoder (VAE) Model to encode and decode images to and from latent representations.
-        text_encoder ([`CLIPTextModel`]):
-            Frozen text-encoder. Stable Diffusion uses the text portion of
-            [CLIP](https://huggingface.co/docs/transformers/model_doc/clip#transformers.CLIPTextModel), specifically
+        image_encoder ([`CLIPVisionModelWithProjection`]):
+            Frozen vision-encoder. Versatile Diffusion uses the vision portion of
+            [CLIP](https://huggingface.co/docs/transformers/model_doc/clip#transformers.CLIPVisionModelWithProjection), specifically
             the [clip-vit-large-patch14](https://huggingface.co/openai/clip-vit-large-patch14) variant.
-        tokenizer (`CLIPTokenizer`):
-            Tokenizer of class
-            [CLIPTokenizer](https://huggingface.co/docs/transformers/v4.21.0/en/model_doc/clip#transformers.CLIPTokenizer).
-        unet ([`UNet2DConditionModel`]): Conditional U-Net architecture to denoise the encoded image latents.
+        image_unet ([`UNet2DConditionModel`]): Conditional U-Net architecture to denoise the encoded image latents.
         scheduler ([`SchedulerMixin`]):
-            A scheduler to be used in combination with `unet` to denoise the encoded image latens. Can be one of
+            A scheduler to be used in combination with `unet` to denoise the encoded image latents. Can be one of
             [`DDIMScheduler`], [`LMSDiscreteScheduler`], or [`PNDMScheduler`].
-        safety_checker ([`StableDiffusionSafetyChecker`]):
-            Classification module that estimates whether generated images could be considered offensive or harmful.
-            Please, refer to the [model card](https://huggingface.co/runwayml/stable-diffusion-v1-5) for details.
-        feature_extractor ([`CLIPFeatureExtractor`]):
-            Model that extracts features from generated images to be used as inputs for the `safety_checker`.
+        image_feature_extractor ([`CLIPFeatureExtractor`]):
+             that extracts features from generated images to be used as inputs for the `safety_checker`.
     """
+    image_feature_extractor: CLIPFeatureExtractor
+    image_encoder: CLIPVisionModelWithProjection
+    image_unet: UNet2DConditionModel
+    vae: AutoencoderKL
+    scheduler: Union[DDIMScheduler, PNDMScheduler, LMSDiscreteScheduler]
 
     def __init__(
         self,
+        image_feature_extractor: CLIPFeatureExtractor,
+        image_encoder: CLIPVisionModelWithProjection,
+        image_unet: UNet2DConditionModel,
         vae: AutoencoderKL,
-        text_encoder: CLIPTextModel,
-        tokenizer: CLIPTokenizer,
-        unet: UNet2DConditionModel,
-        scheduler: Union[DDIMScheduler, PNDMScheduler, LMSDiscreteScheduler,
-                         EulerAncestralDiscreteScheduler],
-        safety_checker: StableDiffusionSafetyChecker,
-        feature_extractor: CLIPFeatureExtractor,
+        scheduler: Union[DDIMScheduler, PNDMScheduler, LMSDiscreteScheduler],
     ):
         super().__init__()
-        if hasattr(scheduler.config,
-                   "steps_offset") and scheduler.config.steps_offset != 1:
-            deprecation_message = (
-                f"The configuration file of this scheduler: {scheduler} is outdated. `steps_offset`"
-                f" should be set to 1 instead of {scheduler.config.steps_offset}. Please make sure "
-                "to update the config accordingly as leaving `steps_offset` might led to incorrect results"
-                " in future versions. If you have downloaded this checkpoint from the Hugging Face Hub,"
-                " it would be very nice if you could open a Pull request for the `scheduler/scheduler_config.json`"
-                " file")
-            deprecate("steps_offset!=1",
-                      "1.0.0",
-                      deprecation_message,
-                      standard_warn=False)
-            new_config = dict(scheduler.config)
-            new_config["steps_offset"] = 1
-            scheduler._internal_dict = FrozenDict(new_config)
-
-        if safety_checker is None:
-            logger.warn(
-                f"You have disabled the safety checker for {self.__class__} by passing `safety_checker=None`. Ensure"
-                " that you abide to the conditions of the Stable Diffusion license and do not expose unfiltered"
-                " results in services or applications open to the public. PaddleNLP team, diffusers team and Hugging Face"
-                " strongly recommend to keep the safety filter enabled in all public facing circumstances, disabling"
-                " it only for use-cases that involve analyzing network behavior or auditing its results. For more"
-                " information, please have a look at https://github.com/huggingface/diffusers/pull/254 ."
-            )
-
         self.register_modules(
+            image_feature_extractor=image_feature_extractor,
+            image_encoder=image_encoder,
+            image_unet=image_unet,
             vae=vae,
-            text_encoder=text_encoder,
-            tokenizer=tokenizer,
-            unet=unet,
             scheduler=scheduler,
-            safety_checker=safety_checker,
-            feature_extractor=feature_extractor,
         )
+        self.vae_scale_factor = 2 ** (len(self.vae.config.block_out_channels) - 1)
 
-    def enable_attention_slicing(self,
-                                 slice_size: Optional[Union[str,
-                                                            int]] = "auto"):
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.enable_attention_slicing with unet->image_unet
+    def enable_attention_slicing(self, slice_size: Optional[Union[str, int]] = "auto"):
         r"""
         Enable sliced attention computation.
+
         When this option is enabled, the attention module will split the input tensor in slices, to compute attention
         in several steps. This is useful to save some memory in exchange for a small speed decrease.
+
         Args:
             slice_size (`str` or `int`, *optional*, defaults to `"auto"`):
                 When `"auto"`, halves the input to the attention heads, so attention will be computed in two steps. If
                 a number is provided, uses as many slices as `attention_head_dim // slice_size`. In this case,
                 `attention_head_dim` must be a multiple of `slice_size`.
         """
         if slice_size == "auto":
-            # half the attention head size is usually a good trade-off between
-            # speed and memory
-            slice_size = self.unet.config.attention_head_dim // 2
-        self.unet.set_attention_slice(slice_size)
+            if isinstance(self.image_unet.config.attention_head_dim, int):
+                # half the attention head size is usually a good trade-off between
+                # speed and memory
+                slice_size = self.image_unet.config.attention_head_dim // 2
+            else:
+                # if `attention_head_dim` is a list, take the smallest head size
+                slice_size = min(self.image_unet.config.attention_head_dim)
+        self.image_unet.set_attention_slice(slice_size)
 
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.disable_attention_slicing
     def disable_attention_slicing(self):
         r"""
         Disable sliced attention computation. If `enable_attention_slicing` was previously invoked, this method will go
         back to computing attention in one step.
         """
-        # set slice_size = `None` to disable `set_attention_slice`
+        # set slice_size = `None` to disable `attention slicing`
         self.enable_attention_slicing(None)
 
+    def _encode_image_prompt(self, prompt, num_images_per_prompt, do_classifier_free_guidance, negative_prompt):
+        r"""
+        Encodes the prompt into image encoder hidden states.
+
+        Args:
+            prompt (`str` or `list(int)`):
+                prompt to be encoded
+            num_images_per_prompt (`int`):
+                number of images that should be generated per prompt
+            do_classifier_free_guidance (`bool`):
+                whether to use classifier free guidance or not
+            negative_prompt (`str` or `List[str]`):
+                The prompt or prompts not to guide the image generation. Ignored when not using guidance (i.e., ignored
+                if `guidance_scale` is less than `1`).
+        """
+
+        def normalize_embeddings(encoder_output):
+            embeds = self.image_encoder.vision_model.ln_post(encoder_output.last_hidden_state)
+            embeds = paddle.matmul(embeds, self.image_encoder.vision_projection)
+            embeds_pooled = embeds[:, 0:1]
+            embeds = embeds / paddle.norm(embeds_pooled, axis=-1, keepdim=True)
+            return embeds
+
+        batch_size = len(prompt) if isinstance(prompt, list) else 1
+
+        # get prompt text embeddings
+        image_input = self.image_feature_extractor(images=prompt, return_tensors="pd")
+        pixel_values = image_input.pixel_values.cast(self.image_encoder.dtype)
+        image_embeddings = self.image_encoder(pixel_values, return_dict=True)
+        image_embeddings = normalize_embeddings(image_embeddings)
+
+        # duplicate image embeddings for each generation per prompt, using mps friendly method
+        bs_embed, seq_len, _ = image_embeddings.shape
+        image_embeddings = image_embeddings.tile([1, num_images_per_prompt, 1])
+        image_embeddings = image_embeddings.reshape([bs_embed * num_images_per_prompt, seq_len, -1])
+
+        # get unconditional embeddings for classifier free guidance
+        if do_classifier_free_guidance:
+            uncond_images: List[str]
+            if negative_prompt is None:
+                uncond_images = [np.zeros((512, 512, 3)) + 0.5] * batch_size
+            elif type(prompt) is not type(negative_prompt):
+                raise TypeError(
+                    f"`negative_prompt` should be the same type to `prompt`, but got {type(negative_prompt)} !="
+                    f" {type(prompt)}."
+                )
+            elif isinstance(negative_prompt, PIL.Image.Image):
+                uncond_images = [negative_prompt]
+            elif batch_size != len(negative_prompt):
+                raise ValueError(
+                    f"`negative_prompt`: {negative_prompt} has batch size {len(negative_prompt)}, but `prompt`:"
+                    f" {prompt} has batch size {batch_size}. Please make sure that passed `negative_prompt` matches"
+                    " the batch size of `prompt`."
+                )
+            else:
+                uncond_images = negative_prompt
+
+            uncond_images = self.image_feature_extractor(images=uncond_images, return_tensors="pd")
+            pixel_values = uncond_images.pixel_values.cast(self.image_encoder.dtype)
+            uncond_embeddings = self.image_encoder(pixel_values, return_dict=True)
+            uncond_embeddings = normalize_embeddings(uncond_embeddings)
+
+            # duplicate unconditional embeddings for each generation per prompt, using mps friendly method
+            seq_len = uncond_embeddings.shape[1]
+            uncond_embeddings = uncond_embeddings.tile([1, num_images_per_prompt, 1])
+            uncond_embeddings = uncond_embeddings.reshape([batch_size * num_images_per_prompt, seq_len, -1])
+
+            # For classifier free guidance, we need to do two forward passes.
+            # Here we concatenate the unconditional and conditional embeddings into a single batch
+            # to avoid doing two forward passes
+            image_embeddings = paddle.concat([uncond_embeddings, image_embeddings])
+
+        return image_embeddings
+
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.decode_latents
+    def decode_latents(self, latents):
+        latents = 1 / 0.18215 * latents
+        image = self.vae.decode(latents).sample
+        image = (image / 2 + 0.5).clip(0, 1)
+        # we always cast to float32 as this does not cause significant overhead and is compatible with bfloa16
+        image = image.transpose([0, 2, 3, 1]).cast("float32").numpy()
+        return image
+
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.prepare_extra_step_kwargs
+    def prepare_extra_step_kwargs(self, generator, eta):
+        # prepare extra kwargs for the scheduler step, since not all schedulers have the same signature
+        # eta (η) is only used with the DDIMScheduler, it will be ignored for other schedulers.
+        # eta corresponds to η in DDIM paper: https://arxiv.org/abs/2010.02502
+        # and should be between [0, 1]
+
+        accepts_eta = "eta" in set(inspect.signature(self.scheduler.step).parameters.keys())
+        extra_step_kwargs = {}
+        if accepts_eta:
+            extra_step_kwargs["eta"] = eta
+
+        # check if the scheduler accepts generator
+        accepts_generator = "generator" in set(inspect.signature(self.scheduler.step).parameters.keys())
+        if accepts_generator:
+            extra_step_kwargs["generator"] = generator
+        return extra_step_kwargs
+
+    def check_inputs(self, image, height, width, callback_steps):
+        if not isinstance(image, PIL.Image.Image) and not isinstance(image, paddle.Tensor):
+            raise ValueError(f"`image` has to be of type `PIL.Image.Image` or `paddle.Tensor` but is {type(image)}")
+
+        if height % 8 != 0 or width % 8 != 0:
+            raise ValueError(f"`height` and `width` have to be divisible by 8 but are {height} and {width}.")
+
+        if (callback_steps is None) or (
+            callback_steps is not None and (not isinstance(callback_steps, int) or callback_steps <= 0)
+        ):
+            raise ValueError(
+                f"`callback_steps` has to be a positive integer but is {callback_steps} of type"
+                f" {type(callback_steps)}."
+            )
+
+    # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.prepare_latents
+    def prepare_latents(self, batch_size, num_channels_latents, height, width, dtype, generator, latents=None):
+        shape = [batch_size, num_channels_latents, height // self.vae_scale_factor, width // self.vae_scale_factor]
+        if latents is None:
+            latents = paddle.randn(shape, generator=generator, dtype=dtype)
+        else:
+            if latents.shape != shape:
+                raise ValueError(f"Unexpected latents shape, got {latents.shape}, expected {shape}")
+
+        # scale the initial noise by the standard deviation required by the scheduler
+        latents = latents * self.scheduler.init_noise_sigma
+        return latents
+
     @paddle.no_grad()
     def __call__(
         self,
-        prompt: Union[str, List[str]],
-        init_image: Union[paddle.Tensor, PIL.Image.Image],
-        mask_image: Union[paddle.Tensor, PIL.Image.Image],
-        strength: float = 0.8,
-        num_inference_steps: Optional[int] = 50,
-        guidance_scale: Optional[float] = 7.5,
+        image: Union[PIL.Image.Image, List[PIL.Image.Image], paddle.Tensor],
+        height: Optional[int] = None,
+        width: Optional[int] = None,
+        num_inference_steps: int = 50,
+        guidance_scale: float = 7.5,
         negative_prompt: Optional[Union[str, List[str]]] = None,
         num_images_per_prompt: Optional[int] = 1,
-        eta: Optional[float] = 0.0,
-        seed: Optional[int] = None,
+        eta: float = 0.0,
+        generator: Optional[paddle.Generator] = None,
+        latents: Optional[paddle.Tensor] = None,
         output_type: Optional[str] = "pil",
         return_dict: bool = True,
         callback: Optional[Callable[[int, int, paddle.Tensor], None]] = None,
         callback_steps: Optional[int] = 1,
         **kwargs,
     ):
         r"""
         Function invoked when calling the pipeline for generation.
+
         Args:
-            prompt (`str` or `List[str]`):
-                The prompt or prompts to guide the image generation.
-            init_image (`paddle.Tensor` or `PIL.Image.Image`):
-                `Image`, or tensor representing an image batch, that will be used as the starting point for the
-                process. This is the image whose masked region will be inpainted.
-            mask_image (`paddle.Tensor` or `PIL.Image.Image`):
-                `Image`, or tensor representing an image batch, to mask `init_image`. White pixels in the mask will be
-                replaced by noise and therefore repainted, while black pixels will be preserved. If `mask_image` is a
-                PIL image, it will be converted to a single channel (luminance) before use. If it's a tensor, it should
-                contain one color channel (L) instead of 3, so the expected shape would be `(B, H, W, 1)`.
-            strength (`float`, *optional*, defaults to 0.8):
-                Conceptually, indicates how much to inpaint the masked area. Must be between 0 and 1. When `strength`
-                is 1, the denoising process will be run on the masked area for the full number of iterations specified
-                in `num_inference_steps`. `init_image` will be used as a reference for the masked area, adding more
-                noise to that region the larger the `strength`. If `strength` is 0, no inpainting will occur.
+            image (`PIL.Image.Image`, `List[PIL.Image.Image]` or `paddle.Tensor`):
+                The image prompt or prompts to guide the image generation.
+            height (`int`, *optional*, defaults to self.image_unet.config.sample_size * self.vae_scale_factor):
+                The height in pixels of the generated image.
+            width (`int`, *optional*, defaults to self.image_unet.config.sample_size * self.vae_scale_factor):
+                The width in pixels of the generated image.
             num_inference_steps (`int`, *optional*, defaults to 50):
-                The reference number of denoising steps. More denoising steps usually lead to a higher quality image at
-                the expense of slower inference. This parameter will be modulated by `strength`, as explained above.
+                The number of denoising steps. More denoising steps usually lead to a higher quality image at the
+                expense of slower inference.
             guidance_scale (`float`, *optional*, defaults to 7.5):
                 Guidance scale as defined in [Classifier-Free Diffusion Guidance](https://arxiv.org/abs/2207.12598).
                 `guidance_scale` is defined as `w` of equation 2. of [Imagen
                 Paper](https://arxiv.org/pdf/2205.11487.pdf). Guidance scale is enabled by setting `guidance_scale >
                 1`. Higher guidance scale encourages to generate images that are closely linked to the text `prompt`,
                 usually at the expense of lower image quality.
             negative_prompt (`str` or `List[str]`, *optional*):
                 The prompt or prompts not to guide the image generation. Ignored when not using guidance (i.e., ignored
                 if `guidance_scale` is less than `1`).
             num_images_per_prompt (`int`, *optional*, defaults to 1):
                 The number of images to generate per prompt.
             eta (`float`, *optional*, defaults to 0.0):
                 Corresponds to parameter eta (η) in the DDIM paper: https://arxiv.org/abs/2010.02502. Only applies to
                 [`schedulers.DDIMScheduler`], will be ignored for others.
-            seed (`int`, *optional*):
-                A random seed.
+            generator (`paddle.Generator`, *optional*):
+                A [paddle generator] to make generation
+                deterministic.
+            latents (`paddle.Tensor`, *optional*):
+                Pre-generated noisy latents, sampled from a Gaussian distribution, to be used as inputs for image
+                generation. Can be used to tweak the same generation with different prompts. If not provided, a latents
+                tensor will ge generated by sampling using the supplied random `generator`.
             output_type (`str`, *optional*, defaults to `"pil"`):
                 The output format of the generate image. Choose between
                 [PIL](https://pillow.readthedocs.io/en/stable/): `PIL.Image.Image` or `np.array`.
             return_dict (`bool`, *optional*, defaults to `True`):
                 Whether or not to return a [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] instead of a
                 plain tuple.
             callback (`Callable`, *optional*):
                 A function that will be called every `callback_steps` steps during inference. The function will be
                 called with the following arguments: `callback(step: int, timestep: int, latents: paddle.Tensor)`.
             callback_steps (`int`, *optional*, defaults to 1):
                 The frequency at which the `callback` function will be called. If not specified, the callback will be
                 called at every step.
+
+        Examples:
+
+        ```py
+        >>> from ppdiffusers import VersatileDiffusionImageVariationPipeline
+        >>> import paddle
+        >>> import requests
+        >>> from io import BytesIO
+        >>> from PIL import Image
+
+        >>> # let's download an initial image
+        >>> url = "https://huggingface.co/datasets/diffusers/images/resolve/main/benz.jpg"
+
+        >>> response = requests.get(url)
+        >>> image = Image.open(BytesIO(response.content)).convert("RGB")
+
+        >>> pipe = VersatileDiffusionImageVariationPipeline.from_pretrained(
+        ...     "shi-labs/versatile-diffusion"
+        ... )
+
+        >>> generator = paddle.Generator().manual_seed(0)
+        >>> image = pipe(image, generator=generator).images[0]
+        >>> image.save("./car_variation.png")
+        ```
+
         Returns:
             [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] or `tuple`:
             [`~pipelines.stable_diffusion.StableDiffusionPipelineOutput`] if `return_dict` is True, otherwise a `tuple.
             When returning a tuple, the first element is a list with the generated images, and the second element is a
             list of `bool`s denoting whether the corresponding generated image likely represents "not-safe-for-work"
             (nsfw) content, according to the `safety_checker`.
         """
-        if isinstance(prompt, str):
-            batch_size = 1
-        elif isinstance(prompt, list):
-            batch_size = len(prompt)
-        else:
-            raise ValueError(
-                f"`prompt` has to be of type `str` or `list` but is {type(prompt)}"
-            )
-
-        if strength < 0 or strength > 1:
-            raise ValueError(
-                f"The value of strength should in [0.0, 1.0] but is {strength}")
+        # 0. Default height and width to unet
+        height = height or self.image_unet.config.sample_size * self.vae_scale_factor
+        width = width or self.image_unet.config.sample_size * self.vae_scale_factor
 
-        if (callback_steps is None) or (callback_steps is not None and
-                                        (not isinstance(callback_steps, int)
-                                         or callback_steps <= 0)):
-            raise ValueError(
-                f"`callback_steps` has to be a positive integer but is {callback_steps} of type"
-                f" {type(callback_steps)}.")
-
-        # set timesteps
-        self.scheduler.set_timesteps(num_inference_steps)
-
-        # get prompt text embeddings
-        text_inputs = self.tokenizer(
-            prompt,
-            padding="max_length",
-            max_length=self.tokenizer.model_max_length,
-            return_tensors="pd",
-        )
-        text_input_ids = text_inputs.input_ids
-
-        if text_input_ids.shape[-1] > self.tokenizer.model_max_length:
-            removed_text = self.tokenizer.batch_decode(
-                text_input_ids[:, self.tokenizer.model_max_length:])
-            logger.warning(
-                "The following part of your input was truncated because CLIP can only handle sequences up to"
-                f" {self.tokenizer.model_max_length} tokens: {removed_text}")
-            text_input_ids = text_input_ids[:, :self.tokenizer.model_max_length]
-        attention_mask = paddle.ones_like(text_input_ids)
-        text_embeddings = self.text_encoder(text_input_ids,
-                                            attention_mask=attention_mask)[0]
-
-        # duplicate text embeddings for each generation per prompt, using mps friendly method
-        bs_embed, seq_len, _ = text_embeddings.shape
-        text_embeddings = text_embeddings.tile([1, num_images_per_prompt, 1])
-        text_embeddings = text_embeddings.reshape(
-            [bs_embed * num_images_per_prompt, seq_len, -1])
+        # 1. Check inputs. Raise error if not correct
+        self.check_inputs(image, height, width, callback_steps)
 
+        # 2. Define call parameters
+        batch_size = 1 if isinstance(image, PIL.Image.Image) else len(image)
         # here `guidance_scale` is defined analog to the guidance weight `w` of equation (2)
         # of the Imagen paper: https://arxiv.org/pdf/2205.11487.pdf . `guidance_scale = 1`
         # corresponds to doing no classifier free guidance.
         do_classifier_free_guidance = guidance_scale > 1.0
-        # get unconditional embeddings for classifier free guidance
-        if do_classifier_free_guidance:
-            uncond_tokens: List[str]
-            if negative_prompt is None:
-                uncond_tokens = [""]
-            elif type(prompt) is not type(negative_prompt):
-                raise TypeError(
-                    f"`negative_prompt` should be the same type to `prompt`, but got {type(negative_prompt)} !="
-                    f" {type(prompt)}.")
-            elif isinstance(negative_prompt, str):
-                uncond_tokens = [negative_prompt]
-            elif batch_size != len(negative_prompt):
-                raise ValueError(
-                    f"`negative_prompt`: {negative_prompt} has batch size {len(negative_prompt)}, but `prompt`:"
-                    f" {prompt} has batch size {batch_size}. Please make sure that passed `negative_prompt` matches"
-                    " the batch size of `prompt`.")
-            else:
-                uncond_tokens = negative_prompt
-
-            max_length = text_input_ids.shape[-1]
-            uncond_input = self.tokenizer(
-                uncond_tokens,
-                padding="max_length",
-                max_length=max_length,
-                truncation=True,
-                return_tensors="pd",
-            )
-            attention_mask = paddle.ones_like(uncond_input.input_ids)
-            uncond_embeddings = self.text_encoder(
-                uncond_input.input_ids, attention_mask=attention_mask)[0]
-
-            # duplicate unconditional embeddings for each generation per prompt, using mps friendly method
-            seq_len = uncond_embeddings.shape[1]
-            uncond_embeddings = uncond_embeddings.tile(
-                [batch_size, num_images_per_prompt, 1])
-            uncond_embeddings = uncond_embeddings.reshape(
-                [batch_size * num_images_per_prompt, seq_len, -1])
 
-            # For classifier free guidance, we need to do two forward passes.
-            # Here we concatenate the unconditional and text embeddings into a single batch
-            # to avoid doing two forward passes
-            text_embeddings = paddle.concat(
-                [uncond_embeddings, text_embeddings])
+        # 3. Encode input prompt
+        image_embeddings = self._encode_image_prompt(
+            image, num_images_per_prompt, do_classifier_free_guidance, negative_prompt
+        )
 
-        # preprocess image
-        if not isinstance(init_image, paddle.Tensor):
-            init_image = preprocess_image(init_image)
-
-        # encode the init image into latents and scale the latents
-        latents_dtype = text_embeddings.dtype
-        init_image = init_image.astype(dtype=latents_dtype)
-        init_latent_dist = self.vae.encode(init_image).latent_dist
-        init_latents = init_latent_dist.sample()
-        init_latents = 0.18215 * init_latents
-
-        # Expand init_latents for batch_size and num_images_per_prompt
-        init_latents = paddle.concat([init_latents] * batch_size *
-                                     num_images_per_prompt,
-                                     axis=0)
-        init_latents_orig = init_latents
-
-        # preprocess mask
-        if not isinstance(mask_image, paddle.Tensor):
-            mask_image = preprocess_mask(mask_image)
-        mask_image = mask_image.astype(dtype=latents_dtype)
-        mask = paddle.concat([mask_image] * batch_size * num_images_per_prompt)
-
-        # check sizes
-        if not mask.shape == init_latents.shape:
-            raise ValueError("The mask and init_image should be the same size!")
-
-        # get the original timestep using init_timestep
-        offset = self.scheduler.config.get("steps_offset", 0)
-        init_timestep = int(num_inference_steps * strength) + offset
-        init_timestep = min(init_timestep, num_inference_steps)
+        # 4. Prepare timesteps
+        self.scheduler.set_timesteps(num_inference_steps)
+        timesteps = self.scheduler.timesteps
 
-        timesteps = self.scheduler.timesteps[-init_timestep]
-        timesteps = timesteps.tile([
+        # 5. Prepare latent variables
+        num_channels_latents = self.image_unet.in_channels
+        latents = self.prepare_latents(
             batch_size * num_images_per_prompt,
-        ])
-
-        # add noise to latents using the timesteps
-        if seed is not None:
-            paddle.seed(seed)
-        noise = paddle.randn(init_latents.shape, dtype=latents_dtype)
-        init_latents = self.scheduler.add_noise(init_latents, noise, timesteps)
-
-        # prepare extra kwargs for the scheduler step, since not all schedulers have the same signature
-        # eta (η) is only used with the DDIMScheduler, it will be ignored for other schedulers.
-        # eta corresponds to η in DDIM paper: https://arxiv.org/abs/2010.02502
-        # and should be between [0, 1]
-        accepts_eta = "eta" in set(
-            inspect.signature(self.scheduler.step).parameters.keys())
-        extra_step_kwargs = {}
-        if accepts_eta:
-            extra_step_kwargs["eta"] = eta
-
-        latents = init_latents
-
-        t_start = max(num_inference_steps - init_timestep + offset, 0)
+            num_channels_latents,
+            height,
+            width,
+            image_embeddings.dtype,
+            generator,
+            latents,
+        )
 
-        # Some schedulers like PNDM have timesteps as arrays
-        # It's more optimized to move all timesteps to correct device beforehand
-        timesteps = self.scheduler.timesteps[t_start:]
+        # 6. Prepare extra step kwargs.
+        extra_step_kwargs = self.prepare_extra_step_kwargs(generator, eta)
 
-        for i, t in tqdm(enumerate(timesteps)):
+        # 7. Denoising loop
+        for i, t in enumerate(self.progress_bar(timesteps)):
             # expand the latents if we are doing classifier free guidance
-            latent_model_input = paddle.concat(
-                [latents] * 2) if do_classifier_free_guidance else latents
-            latent_model_input = self.scheduler.scale_model_input(
-                latent_model_input, t)
+            latent_model_input = paddle.concat([latents] * 2) if do_classifier_free_guidance else latents
+            latent_model_input = self.scheduler.scale_model_input(latent_model_input, t)
 
             # predict the noise residual
-            noise_pred = self.unet(latent_model_input,
-                                   t,
-                                   encoder_hidden_states=text_embeddings).sample
+            noise_pred = self.image_unet(latent_model_input, t, encoder_hidden_states=image_embeddings).sample
 
             # perform guidance
             if do_classifier_free_guidance:
                 noise_pred_uncond, noise_pred_text = noise_pred.chunk(2)
-                noise_pred = noise_pred_uncond + guidance_scale * (
-                    noise_pred_text - noise_pred_uncond)
+                noise_pred = noise_pred_uncond + guidance_scale * (noise_pred_text - noise_pred_uncond)
 
             # compute the previous noisy sample x_t -> x_t-1
-            latents = self.scheduler.step(noise_pred, t, latents,
-                                          **extra_step_kwargs).prev_sample
-            # masking
-            init_latents_proper = self.scheduler.add_noise(
-                init_latents_orig, noise, t)
-
-            latents = (init_latents_proper * mask) + (latents * (1 - mask))
+            latents = self.scheduler.step(noise_pred, t, latents, **extra_step_kwargs).prev_sample
 
             # call the callback, if provided
             if callback is not None and i % callback_steps == 0:
                 callback(i, t, latents)
 
-        latents = 1 / 0.18215 * latents
-        image = self.vae.decode(latents).sample
-
-        image = (image / 2 + 0.5).clip(0, 1)
-        image = image.transpose([0, 2, 3, 1]).numpy()
-
-        if self.safety_checker is not None:
-            safety_checker_input = self.feature_extractor(
-                self.numpy_to_pil(image), return_tensors="pd")
-            image, has_nsfw_concept = self.safety_checker(
-                images=image, clip_input=safety_checker_input.pixel_values)
-        else:
-            has_nsfw_concept = None
+        # 8. Post-processing
+        image = self.decode_latents(latents)
 
+        # 9. Convert to PIL
         if output_type == "pil":
             image = self.numpy_to_pil(image)
 
         if not return_dict:
-            return (image, has_nsfw_concept)
+            return (image,)
 
-        return StableDiffusionPipelineOutput(
-            images=image, nsfw_content_detected=has_nsfw_concept)
+        return ImagePipelineOutput(images=image)
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/pipelines/stable_diffusion/safety_checker.py` & `ppdiffusers-0.9.0/ppdiffusers/pipelines/stable_diffusion/safety_checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (c) 2022 PaddlePaddle Authors. All Rights Reserved.
+# Copyright 2022 The HuggingFace Team. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,131 +12,112 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import numpy as np
 import paddle
 import paddle.nn.functional as F
+
 from paddlenlp.transformers import CLIPPretrainedModel, CLIPVisionModel
 
 from ...utils import logging
 
 logger = logging.get_logger(__name__)
 
 
 def cosine_distance(image_embeds, text_embeds):
     normalized_image_embeds = F.normalize(image_embeds)
     normalized_text_embeds = F.normalize(text_embeds)
-    return paddle.matmul(normalized_image_embeds,
-                         normalized_text_embeds,
-                         transpose_y=True)
+    return paddle.matmul(normalized_image_embeds, normalized_text_embeds, transpose_y=True)
 
 
 class StableDiffusionSafetyChecker(CLIPPretrainedModel):
     base_model_class = CLIPVisionModel
 
     def __init__(self, clip):
         super().__init__()
         self.clip = clip
         projection_dim = clip.config["projection_dim"]
         vision_embed_dim = clip.config["vision_embed_dim"]
         self.vision_projection = paddle.create_parameter(
-            (vision_embed_dim, projection_dim),
-            dtype=paddle.get_default_dtype())
+            (vision_embed_dim, projection_dim), dtype=paddle.get_default_dtype()
+        )
 
-        self.register_buffer("concept_embeds", paddle.ones([17,
-                                                            projection_dim]))
-        self.register_buffer("special_care_embeds",
-                             paddle.ones([3, projection_dim]))
+        self.register_buffer("concept_embeds", paddle.ones([17, projection_dim]))
+        self.register_buffer("special_care_embeds", paddle.ones([3, projection_dim]))
 
         self.register_buffer("concept_embeds_weights", paddle.ones([17]))
         self.register_buffer("special_care_embeds_weights", paddle.ones([3]))
 
     @paddle.no_grad()
     def forward(self, clip_input, images):
         pooled_output = self.clip.vision_model(clip_input)[1]  # pooled_output
         image_embeds = paddle.matmul(pooled_output, self.vision_projection)
 
         # we always cast to float32 as this does not cause significant overhead and is compatible with bfloa16
-        special_cos_dist = cosine_distance(
-            image_embeds, self.special_care_embeds).astype("float32").numpy()
-        cos_dist = cosine_distance(
-            image_embeds, self.concept_embeds).astype("float32").numpy()
+        special_cos_dist = cosine_distance(image_embeds, self.special_care_embeds).astype("float32").numpy()
+        cos_dist = cosine_distance(image_embeds, self.concept_embeds).astype("float32").numpy()
 
         result = []
         batch_size = image_embeds.shape[0]
         for i in range(batch_size):
-            result_img = {
-                "special_scores": {},
-                "special_care": [],
-                "concept_scores": {},
-                "bad_concepts": []
-            }
+            result_img = {"special_scores": {}, "special_care": [], "concept_scores": {}, "bad_concepts": []}
 
             # increase this value to create a stronger `nfsw` filter
             # at the cost of increasing the possibility of filtering benign images
             adjustment = 0.0
 
             for concept_idx in range(len(special_cos_dist[0])):
                 concept_cos = special_cos_dist[i][concept_idx]
-                concept_threshold = self.special_care_embeds_weights[
-                    concept_idx].item()
-                result_img["special_scores"][concept_idx] = round(
-                    concept_cos - concept_threshold + adjustment, 3)
+                concept_threshold = self.special_care_embeds_weights[concept_idx].item()
+                result_img["special_scores"][concept_idx] = round(concept_cos - concept_threshold + adjustment, 3)
                 if result_img["special_scores"][concept_idx] > 0:
-                    result_img["special_care"].append({
-                        concept_idx, result_img["special_scores"][concept_idx]
-                    })
+                    result_img["special_care"].append({concept_idx, result_img["special_scores"][concept_idx]})
                     adjustment = 0.01
 
             for concept_idx in range(len(cos_dist[0])):
                 concept_cos = cos_dist[i][concept_idx]
-                concept_threshold = self.concept_embeds_weights[
-                    concept_idx].item()
-                result_img["concept_scores"][concept_idx] = round(
-                    concept_cos - concept_threshold + adjustment, 3)
+                concept_threshold = self.concept_embeds_weights[concept_idx].item()
+                result_img["concept_scores"][concept_idx] = round(concept_cos - concept_threshold + adjustment, 3)
                 if result_img["concept_scores"][concept_idx] > 0:
                     result_img["bad_concepts"].append(concept_idx)
 
             result.append(result_img)
 
         has_nsfw_concepts = [len(res["bad_concepts"]) > 0 for res in result]
 
         for idx, has_nsfw_concept in enumerate(has_nsfw_concepts):
             if has_nsfw_concept:
                 images[idx] = np.zeros(images[idx].shape)  # black image
 
         if any(has_nsfw_concepts):
             logger.warning(
                 "Potential NSFW content was detected in one or more images. A black image will be returned instead."
-                " Try again with a different prompt and/or seed.")
+                " Try again with a different prompt and/or seed."
+            )
 
         return images, has_nsfw_concepts
 
-    @paddle.no_grad()
-    def forward_onnx(self, clip_input: paddle.Tensor, images: paddle.Tensor):
+    def forward_fastdeploy(self, clip_input: paddle.Tensor, images: paddle.Tensor):
         pooled_output = self.clip.vision_model(clip_input)[1]  # pooled_output
         image_embeds = paddle.matmul(pooled_output, self.vision_projection)
 
-        special_cos_dist = cosine_distance(image_embeds,
-                                           self.special_care_embeds)
+        special_cos_dist = cosine_distance(image_embeds, self.special_care_embeds)
         cos_dist = cosine_distance(image_embeds, self.concept_embeds)
 
         # increase this value to create a stronger `nsfw` filter
         # at the cost of increasing the possibility of filtering benign images
         adjustment = 0.0
 
         special_scores = special_cos_dist - self.special_care_embeds_weights + adjustment
         # special_scores = special_scores.round(decimals=3)
         special_care = paddle.any(special_scores > 0, axis=1)
         special_adjustment = special_care * 0.01
-        special_adjustment = special_adjustment.unsqueeze(1).expand(
-            [-1, cos_dist.shape[1]])
+        special_adjustment = special_adjustment.unsqueeze(1).expand([-1, cos_dist.shape[1]])
 
-        concept_scores = (cos_dist -
-                          self.concept_embeds_weights) + special_adjustment
+        concept_scores = (cos_dist - self.concept_embeds_weights) + special_adjustment
         # concept_scores = concept_scores.round(decimals=3)
         has_nsfw_concepts = paddle.any(concept_scores > 0, axis=1)
 
         images[has_nsfw_concepts] = 0.0  # black image
 
         return images, has_nsfw_concepts
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/pipelines/stochastic_karras_ve/__init__.py` & `ppdiffusers-0.9.0/ppdiffusers/pipelines/stochastic_karras_ve/__init__.py`

 * *Files identical despite different names*

### Comparing `ppdiffusers-0.6.3/ppdiffusers/pipelines/stochastic_karras_ve/pipeline_stochastic_karras_ve.py` & `ppdiffusers-0.9.0/ppdiffusers/pipelines/stochastic_karras_ve/pipeline_stochastic_karras_ve.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,88 +46,83 @@
         self.register_modules(unet=unet, scheduler=scheduler)
 
     @paddle.no_grad()
     def __call__(
         self,
         batch_size: int = 1,
         num_inference_steps: int = 50,
-        seed: Optional[int] = None,
+        generator: Optional[paddle.Generator] = None,
         output_type: Optional[str] = "pil",
         return_dict: bool = True,
         **kwargs,
     ) -> Union[Tuple, ImagePipelineOutput]:
         r"""
         Args:
             batch_size (`int`, *optional*, defaults to 1):
                 The number of images to generate.
-            seed (`int`, *optional*):
-                A random seed.
+            generator (`paddle.Generator`, *optional*):
+                A [paddle generator] to make generation deterministic.
             num_inference_steps (`int`, *optional*, defaults to 50):
                 The number of denoising steps. More denoising steps usually lead to a higher quality image at the
                 expense of slower inference.
             output_type (`str`, *optional*, defaults to `"pil"`):
                 The output format of the generate image. Choose between
                 [PIL](https://pillow.readthedocs.io/en/stable/): `PIL.Image.Image` or `np.array`.
             return_dict (`bool`, *optional*, defaults to `True`):
                 Whether or not to return a [`~pipeline_utils.ImagePipelineOutput`] instead of a plain tuple.
 
         Returns:
             [`~pipeline_utils.ImagePipelineOutput`] or `tuple`: [`~pipelines.utils.ImagePipelineOutput`] if
             `return_dict` is True, otherwise a `tuple. When returning a tuple, the first element is a list with the
             generated images.
         """
-        if seed is not None:
-            paddle.seed(seed)
+
         img_size = self.unet.config.sample_size
         shape = (batch_size, 3, img_size, img_size)
 
         model = self.unet
 
         # sample x_0 ~ N(0, sigma_0^2 * I)
-        sample = paddle.randn(shape) * self.scheduler.init_noise_sigma
+        sample = paddle.randn(shape, generator=generator) * self.scheduler.init_noise_sigma
 
         self.scheduler.set_timesteps(num_inference_steps)
 
         for t in self.progress_bar(self.scheduler.timesteps):
             # here sigma_t == t_i from the paper
             sigma = self.scheduler.schedule[t]
             sigma_prev = self.scheduler.schedule[t - 1] if t > 0 else 0
 
             # 1. Select temporarily increased noise level sigma_hat
             # 2. Add new noise to move from sample_i to sample_hat
-            sample_hat, sigma_hat = self.scheduler.add_noise_to_input(
-                sample, sigma)
+            sample_hat, sigma_hat = self.scheduler.add_noise_to_input(sample, sigma, generator=generator)
 
             # 3. Predict the noise residual given the noise magnitude `sigma_hat`
             # The model inputs and output are adjusted by following eq. (213) in [1].
-            model_output = (sigma_hat / 2) * model(
-                (sample_hat + 1) / 2, sigma_hat / 2).sample
+            model_output = (sigma_hat / 2) * model((sample_hat + 1) / 2, sigma_hat / 2).sample
 
             # 4. Evaluate dx/dt at sigma_hat
             # 5. Take Euler step from sigma to sigma_prev
-            step_output = self.scheduler.step(model_output, sigma_hat,
-                                              sigma_prev, sample_hat)
+            step_output = self.scheduler.step(model_output, sigma_hat, sigma_prev, sample_hat)
 
             if sigma_prev != 0:
                 # 6. Apply 2nd order correction
                 # The model inputs and output are adjusted by following eq. (213) in [1].
-                model_output = (sigma_prev / 2) * model(
-                    (step_output.prev_sample + 1) / 2, sigma_prev / 2).sample
+                model_output = (sigma_prev / 2) * model((step_output.prev_sample + 1) / 2, sigma_prev / 2).sample
                 step_output = self.scheduler.step_correct(
                     model_output,
                     sigma_hat,
                     sigma_prev,
                     sample_hat,
                     step_output.prev_sample,
                     step_output["derivative"],
                 )
             sample = step_output.prev_sample
 
         sample = (sample / 2 + 0.5).clip(0, 1)
         image = sample.transpose([0, 2, 3, 1]).numpy()
         if output_type == "pil":
-            image = self.numpy_to_pil(sample)
+            image = self.numpy_to_pil(image)
 
         if not return_dict:
-            return (image, )
+            return (image,)
 
         return ImagePipelineOutput(images=image)
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/schedulers/scheduling_ddim.py` & `ppdiffusers-0.9.0/ppdiffusers/schedulers/scheduling_ddim.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,26 +14,26 @@
 # limitations under the License.
 
 # DISCLAIMER: This code is strongly influenced by https://github.com/pesser/pytorch_diffusion
 # and https://github.com/hojonathanho/diffusion
 
 import math
 from dataclasses import dataclass
-from typing import Optional, Tuple, Union
+from typing import List, Optional, Tuple, Union
 
 import numpy as np
 import paddle
 
 from ..configuration_utils import ConfigMixin, register_to_config
-from ..utils import BaseOutput
+from ..utils import _COMPATIBLE_STABLE_DIFFUSION_SCHEDULERS, BaseOutput, deprecate
 from .scheduling_utils import SchedulerMixin
 
 
 @dataclass
-# Copied from ppdiffusers.schedulers.scheduling_ddpm.DDPMSchedulerOutput with DDPM->DDIM
+# Copied from diffusers.schedulers.scheduling_ddpm.DDPMSchedulerOutput with DDPM->DDIM
 class DDIMSchedulerOutput(BaseOutput):
     """
     Output class for the scheduler's step function output.
 
     Args:
         prev_sample (`paddle.Tensor` of shape `(batch_size, num_channels, height, width)` for images):
             Computed sample (x_{t-1}) of previous timestep. `prev_sample` should be used as next model input in the
@@ -43,16 +43,15 @@
             `pred_original_sample` can be used to preview progress or for guidance.
     """
 
     prev_sample: paddle.Tensor
     pred_original_sample: Optional[paddle.Tensor] = None
 
 
-def betas_for_alpha_bar(num_diffusion_timesteps,
-                        max_beta=0.999) -> paddle.Tensor:
+def betas_for_alpha_bar(num_diffusion_timesteps, max_beta=0.999) -> paddle.Tensor:
     """
     Create a beta schedule that discretizes the given alpha_t_bar function, which defines the cumulative product of
     (1-beta) over time from t = [0,1].
 
     Contains a function alpha_bar that takes an argument t and transforms it to the cumulative product of (1-beta) up
     to that part of the diffusion process.
 
@@ -63,15 +62,15 @@
                      prevent singularities.
 
     Returns:
         betas (`np.ndarray`): the betas used by the scheduler to step the model outputs
     """
 
     def alpha_bar(time_step):
-        return math.cos((time_step + 0.008) / 1.008 * math.pi / 2)**2
+        return math.cos((time_step + 0.008) / 1.008 * math.pi / 2) ** 2
 
     betas = []
     for i in range(num_diffusion_timesteps):
         t1 = i / num_diffusion_timesteps
         t2 = (i + 1) / num_diffusion_timesteps
         betas.append(min(1 - alpha_bar(t2) / alpha_bar(t1), max_beta))
     return paddle.to_tensor(betas)
@@ -80,16 +79,16 @@
 class DDIMScheduler(SchedulerMixin, ConfigMixin):
     """
     Denoising diffusion implicit models is a scheduler that extends the denoising procedure introduced in denoising
     diffusion probabilistic models (DDPMs) with non-Markovian guidance.
 
     [`~ConfigMixin`] takes care of storing all config attributes that are passed in the scheduler's `__init__`
     function, such as `num_train_timesteps`. They can be accessed via `scheduler.config.num_train_timesteps`.
-    [`~ConfigMixin`] also provides general loading and saving functionality via the [`~ConfigMixin.save_config`] and
-    [`~ConfigMixin.from_config`] functions.
+    [`SchedulerMixin`] provides general loading and saving functionality via the [`SchedulerMixin.save_pretrained`] and
+    [`~SchedulerMixin.from_pretrained`] functions.
 
     For more details, see the original paper: https://arxiv.org/abs/2010.02502
 
     Args:
         num_train_timesteps (`int`): number of diffusion steps used to train the model.
         beta_start (`float`): the starting `beta` value of inference.
         beta_end (`float`): the final `beta` value.
@@ -104,70 +103,75 @@
             each diffusion step uses the value of alphas product at that step and at the previous one. For the final
             step there is no previous alpha. When this option is `True` the previous alpha product is fixed to `1`,
             otherwise it uses the value of alpha at step 0.
         steps_offset (`int`, default `0`):
             an offset added to the inference steps. You can use a combination of `offset=1` and
             `set_alpha_to_one=False`, to make the last step use step 0 for the previous alpha product, as done in
             stable diffusion.
-
+        prediction_type (`str`, default `epsilon`, optional):
+            prediction type of the scheduler function, one of `epsilon` (predicting the noise of the diffusion
+            process), `sample` (directly predicting the noisy sample`) or `v_prediction` (see section 2.4
+            https://imagen.research.google/video/paper.pdf)
     """
 
+    _compatibles = _COMPATIBLE_STABLE_DIFFUSION_SCHEDULERS.copy()
+    _deprecated_kwargs = ["predict_epsilon"]
+    order = 1
+
     @register_to_config
     def __init__(
         self,
         num_train_timesteps: int = 1000,
         beta_start: float = 0.0001,
         beta_end: float = 0.02,
         beta_schedule: str = "linear",
-        trained_betas: Optional[np.ndarray] = None,
+        trained_betas: Optional[Union[np.ndarray, List[float]]] = None,
         clip_sample: bool = True,
         set_alpha_to_one: bool = True,
         steps_offset: int = 0,
+        prediction_type: str = "epsilon",
+        **kwargs,
     ):
+        message = (
+            "Please make sure to instantiate your scheduler with `prediction_type` instead. E.g. `scheduler ="
+            " DDIMScheduler.from_pretrained(<model_id>, prediction_type='epsilon')`."
+        )
+        predict_epsilon = deprecate("predict_epsilon", "0.10.0", message, take_from=kwargs)
+        if predict_epsilon is not None:
+            self.register_to_config(prediction_type="epsilon" if predict_epsilon else "sample")
         if trained_betas is not None:
-            self.betas = paddle.to_tensor(trained_betas)
+            self.betas = paddle.to_tensor(trained_betas, dtype="float32")
         elif beta_schedule == "linear":
-            self.betas = paddle.linspace(beta_start,
-                                         beta_end,
-                                         num_train_timesteps,
-                                         dtype="float32")
+            self.betas = paddle.linspace(beta_start, beta_end, num_train_timesteps, dtype="float32")
         elif beta_schedule == "scaled_linear":
             # this schedule is very specific to the latent diffusion model.
-            self.betas = (paddle.linspace(beta_start**0.5,
-                                          beta_end**0.5,
-                                          num_train_timesteps,
-                                          dtype="float32")**2)
+            self.betas = paddle.linspace(beta_start**0.5, beta_end**0.5, num_train_timesteps, dtype="float32") ** 2
         elif beta_schedule == "squaredcos_cap_v2":
             # Glide cosine schedule
             self.betas = betas_for_alpha_bar(num_train_timesteps)
         else:
-            raise NotImplementedError(
-                f"{beta_schedule} does is not implemented for {self.__class__}")
+            raise NotImplementedError(f"{beta_schedule} does is not implemented for {self.__class__}")
 
         self.alphas = 1.0 - self.betas
         self.alphas_cumprod = paddle.cumprod(self.alphas, 0)
 
         # At every step in ddim, we are looking into the previous alphas_cumprod
         # For the final step, there is no previous alphas_cumprod because we are already at 0
         # `set_alpha_to_one` decides whether we set this parameter simply to one or
         # whether we use the final alpha of the "non-previous" one.
-        self.final_alpha_cumprod = paddle.to_tensor(
-            1.0) if set_alpha_to_one else self.alphas_cumprod[0]
+        self.final_alpha_cumprod = paddle.to_tensor(1.0) if set_alpha_to_one else self.alphas_cumprod[0]
 
         # standard deviation of the initial noise distribution
         self.init_noise_sigma = 1.0
 
         # setable values
         self.num_inference_steps = None
-        self.timesteps = paddle.to_tensor(
-            np.arange(0, num_train_timesteps)[::-1].copy().astype("int64"))
+        self.timesteps = paddle.to_tensor(np.arange(0, num_train_timesteps)[::-1].copy().astype(np.int64))
 
-    def scale_model_input(self,
-                          sample: paddle.Tensor,
-                          timestep: Optional[int] = None) -> paddle.Tensor:
+    def scale_model_input(self, sample: paddle.Tensor, timestep: Optional[int] = None) -> paddle.Tensor:
         """
         Ensures interchangeability with schedulers that need to scale the denoising model input depending on the
         current timestep.
 
         Args:
             sample (`paddle.Tensor`): input sample
             timestep (`int`, optional): current timestep
@@ -175,21 +179,19 @@
         Returns:
             `paddle.Tensor`: scaled input sample
         """
         return sample
 
     def _get_variance(self, timestep, prev_timestep):
         alpha_prod_t = self.alphas_cumprod[timestep]
-        alpha_prod_t_prev = self.alphas_cumprod[
-            prev_timestep] if prev_timestep >= 0 else self.final_alpha_cumprod
+        alpha_prod_t_prev = self.alphas_cumprod[prev_timestep] if prev_timestep >= 0 else self.final_alpha_cumprod
         beta_prod_t = 1 - alpha_prod_t
         beta_prod_t_prev = 1 - alpha_prod_t_prev
 
-        variance = (beta_prod_t_prev /
-                    beta_prod_t) * (1 - alpha_prod_t / alpha_prod_t_prev)
+        variance = (beta_prod_t_prev / beta_prod_t) * (1 - alpha_prod_t / alpha_prod_t_prev)
 
         return variance
 
     def set_timesteps(self, num_inference_steps: int):
         """
         Sets the discrete timesteps used for the diffusion chain. Supporting function to be run before inference.
 
@@ -197,39 +199,47 @@
             num_inference_steps (`int`):
                 the number of diffusion steps used when generating samples with a pre-trained model.
         """
         self.num_inference_steps = num_inference_steps
         step_ratio = self.config.num_train_timesteps // self.num_inference_steps
         # creates integer timesteps by multiplying by ratio
         # casting to int to avoid issues when num_inference_step is power of 3
-        timesteps = (np.arange(0, num_inference_steps) *
-                     step_ratio).round()[::-1].copy().astype("int64")
+        timesteps = (np.arange(0, num_inference_steps) * step_ratio).round()[::-1].copy().astype(np.int64)
         self.timesteps = paddle.to_tensor(timesteps)
         self.timesteps += self.config.steps_offset
 
     def step(
         self,
         model_output: paddle.Tensor,
         timestep: int,
         sample: paddle.Tensor,
         eta: float = 0.0,
         use_clipped_model_output: bool = False,
+        generator=None,
+        variance_noise: Optional[paddle.Tensor] = None,
         return_dict: bool = True,
     ) -> Union[DDIMSchedulerOutput, Tuple]:
         """
         Predict the sample at the previous timestep by reversing the SDE. Core function to propagate the diffusion
         process from the learned model outputs (most often the predicted noise).
 
         Args:
             model_output (`paddle.Tensor`): direct output from learned diffusion model.
             timestep (`int`): current discrete timestep in the diffusion chain.
             sample (`paddle.Tensor`):
                 current instance of sample being created by diffusion process.
             eta (`float`): weight of noise for added noise in diffusion step.
-            use_clipped_model_output (`bool`): TODO
+            use_clipped_model_output (`bool`): if `True`, compute "corrected" `model_output` from the clipped
+                predicted original sample. Necessary because predicted original sample is clipped to [-1, 1] when
+                `self.config.clip_sample` is `True`. If no clipping has happened, "corrected" `model_output` would
+                coincide with the one provided as input and `use_clipped_model_output` will have not effect.
+            generator: random number generator.
+            variance_noise (`paddle.Tensor`): instead of generating noise for the variance using `generator`, we
+                can directly provide the noise for the variance itself. This is useful for methods such as
+                CycleDiffusion. (https://arxiv.org/abs/2210.05559)
             return_dict (`bool`): option for returning tuple rather than DDIMSchedulerOutput class
 
         Returns:
             [`~schedulers.scheduling_utils.DDIMSchedulerOutput`] or `tuple`:
             [`~schedulers.scheduling_utils.DDIMSchedulerOutput`] if `return_dict` is True, otherwise a `tuple`. When
             returning a tuple, the first element is the sample tensor.
 
@@ -251,78 +261,106 @@
         # - pred_prev_sample -> "x_t-1"
 
         # 1. get previous step value (=t-1)
         prev_timestep = timestep - self.config.num_train_timesteps // self.num_inference_steps
 
         # 2. compute alphas, betas
         alpha_prod_t = self.alphas_cumprod[timestep]
-        alpha_prod_t_prev = self.alphas_cumprod[
-            prev_timestep] if prev_timestep >= 0 else self.final_alpha_cumprod
+        alpha_prod_t_prev = self.alphas_cumprod[prev_timestep] if prev_timestep >= 0 else self.final_alpha_cumprod
 
         beta_prod_t = 1 - alpha_prod_t
 
         # 3. compute predicted original sample from predicted noise also called
         # "predicted x_0" of formula (12) from https://arxiv.org/pdf/2010.02502.pdf
-        pred_original_sample = (sample - beta_prod_t**
-                                (0.5) * model_output) / alpha_prod_t**(0.5)
+        if self.config.prediction_type == "epsilon":
+            pred_original_sample = (sample - beta_prod_t ** (0.5) * model_output) / alpha_prod_t ** (0.5)
+        elif self.config.prediction_type == "sample":
+            pred_original_sample = model_output
+        elif self.config.prediction_type == "v_prediction":
+            pred_original_sample = (alpha_prod_t**0.5) * sample - (beta_prod_t**0.5) * model_output
+            # predict V
+            model_output = (alpha_prod_t**0.5) * model_output + (beta_prod_t**0.5) * sample
+        else:
+            raise ValueError(
+                f"prediction_type given as {self.config.prediction_type} must be one of `epsilon`, `sample`, or"
+                " `v_prediction`"
+            )
 
         # 4. Clip "predicted x_0"
         if self.config.clip_sample:
             pred_original_sample = paddle.clip(pred_original_sample, -1, 1)
 
         # 5. compute variance: "sigma_t(η)" -> see formula (16)
         # σ_t = sqrt((1 − α_t−1)/(1 − α_t)) * sqrt(1 − α_t/α_t−1)
         variance = self._get_variance(timestep, prev_timestep)
-        std_dev_t = eta * variance**(0.5)
+        std_dev_t = eta * variance ** (0.5)
 
         if use_clipped_model_output:
             # the model_output is always re-derived from the clipped x_0 in Glide
-            model_output = (sample - alpha_prod_t**
-                            (0.5) * pred_original_sample) / beta_prod_t**(0.5)
+            model_output = (sample - alpha_prod_t ** (0.5) * pred_original_sample) / beta_prod_t ** (0.5)
 
         # 6. compute "direction pointing to x_t" of formula (12) from https://arxiv.org/pdf/2010.02502.pdf
-        pred_sample_direction = (1 - alpha_prod_t_prev -
-                                 std_dev_t**2)**(0.5) * model_output
+        pred_sample_direction = (1 - alpha_prod_t_prev - std_dev_t**2) ** (0.5) * model_output
 
         # 7. compute x_t without "random noise" of formula (12) from https://arxiv.org/pdf/2010.02502.pdf
-        prev_sample = alpha_prod_t_prev**(
-            0.5) * pred_original_sample + pred_sample_direction
+        prev_sample = alpha_prod_t_prev ** (0.5) * pred_original_sample + pred_sample_direction
 
         if eta > 0:
-            # randn_like does not support seed https://github.com/pytorch/pytorch/issues/27072
-            noise = paddle.randn(model_output.shape, dtype=model_output.dtype)
-            variance = self._get_variance(timestep,
-                                          prev_timestep)**(0.5) * eta * noise
+            # randn_like does not support generator https://github.com/pytorch/pytorch/issues/27072
+            if variance_noise is not None and generator is not None:
+                raise ValueError(
+                    "Cannot pass both generator and variance_noise. Please make sure that either `generator` or"
+                    " `variance_noise` stays `None`."
+                )
+
+            if variance_noise is None:
+                variance_noise = paddle.randn(model_output.shape, generator=generator, dtype=model_output.dtype)
+            variance = self._get_variance(timestep, prev_timestep) ** (0.5) * eta * variance_noise
 
             prev_sample = prev_sample + variance
 
         if not return_dict:
-            return (prev_sample, )
+            return (prev_sample,)
 
-        return DDIMSchedulerOutput(prev_sample=prev_sample,
-                                   pred_original_sample=pred_original_sample)
+        return DDIMSchedulerOutput(prev_sample=prev_sample, pred_original_sample=pred_original_sample)
 
     def add_noise(
         self,
         original_samples: paddle.Tensor,
         noise: paddle.Tensor,
         timesteps: paddle.Tensor,
     ) -> paddle.Tensor:
         # Make sure alphas_cumprod and timestep have same dtype as original_samples
-        self.alphas_cumprod = self.alphas_cumprod.astype(original_samples.dtype)
+        self.alphas_cumprod = self.alphas_cumprod.cast(original_samples.dtype)
 
-        sqrt_alpha_prod = self.alphas_cumprod[timesteps]**0.5
+        sqrt_alpha_prod = self.alphas_cumprod[timesteps] ** 0.5
         sqrt_alpha_prod = sqrt_alpha_prod.flatten()
         while len(sqrt_alpha_prod.shape) < len(original_samples.shape):
             sqrt_alpha_prod = sqrt_alpha_prod.unsqueeze(-1)
 
-        sqrt_one_minus_alpha_prod = (1 - self.alphas_cumprod[timesteps])**0.5
+        sqrt_one_minus_alpha_prod = (1 - self.alphas_cumprod[timesteps]) ** 0.5
         sqrt_one_minus_alpha_prod = sqrt_one_minus_alpha_prod.flatten()
-        while len(sqrt_one_minus_alpha_prod.shape) < len(
-                original_samples.shape):
+        while len(sqrt_one_minus_alpha_prod.shape) < len(original_samples.shape):
             sqrt_one_minus_alpha_prod = sqrt_one_minus_alpha_prod.unsqueeze(-1)
 
         noisy_samples = sqrt_alpha_prod * original_samples + sqrt_one_minus_alpha_prod * noise
         return noisy_samples
 
+    def get_velocity(self, sample: paddle.Tensor, noise: paddle.Tensor, timesteps: paddle.Tensor) -> paddle.Tensor:
+        # Make sure alphas_cumprod and timestep have same dtype as sample
+        self.alphas_cumprod = self.alphas_cumprod.cast(sample.dtype)
+
+        sqrt_alpha_prod = self.alphas_cumprod[timesteps] ** 0.5
+        sqrt_alpha_prod = sqrt_alpha_prod.flatten()
+        while len(sqrt_alpha_prod.shape) < len(sample.shape):
+            sqrt_alpha_prod = sqrt_alpha_prod.unsqueeze(-1)
+
+        sqrt_one_minus_alpha_prod = (1 - self.alphas_cumprod[timesteps]) ** 0.5
+        sqrt_one_minus_alpha_prod = sqrt_one_minus_alpha_prod.flatten()
+        while len(sqrt_one_minus_alpha_prod.shape) < len(sample.shape):
+            sqrt_one_minus_alpha_prod = sqrt_one_minus_alpha_prod.unsqueeze(-1)
+
+        velocity = sqrt_alpha_prod * noise - sqrt_one_minus_alpha_prod * sample
+        return velocity
+
     def __len__(self):
         return self.config.num_train_timesteps
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/schedulers/scheduling_ddpm.py` & `ppdiffusers-0.9.0/ppdiffusers/schedulers/scheduling_repaint.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,51 @@
 # Copyright (c) 2022 PaddlePaddle Authors. All Rights Reserved.
-# Copyright 2022 UC Berkeley Team and The HuggingFace Team. All rights reserved.
+# Copyright 2022 ETH Zurich Computer Vision Lab and The HuggingFace Team. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# DISCLAIMER: This file is strongly influenced by https://github.com/ermongroup/ddim
-
 import math
 from dataclasses import dataclass
 from typing import Optional, Tuple, Union
 
 import numpy as np
 import paddle
 import paddle.nn.functional as F
 
 from ..configuration_utils import ConfigMixin, register_to_config
 from ..utils import BaseOutput
 from .scheduling_utils import SchedulerMixin
 
 
 @dataclass
-class DDPMSchedulerOutput(BaseOutput):
+class RePaintSchedulerOutput(BaseOutput):
     """
     Output class for the scheduler's step function output.
 
     Args:
         prev_sample (`paddle.Tensor` of shape `(batch_size, num_channels, height, width)` for images):
             Computed sample (x_{t-1}) of previous timestep. `prev_sample` should be used as next model input in the
             denoising loop.
         pred_original_sample (`paddle.Tensor` of shape `(batch_size, num_channels, height, width)` for images):
-            The predicted denoised sample (x_{0}) based on the model output from the current timestep.
-            `pred_original_sample` can be used to preview progress or for guidance.
+            The predicted denoised sample (x_{0}) based on the model output from
+             the current timestep. `pred_original_sample` can be used to preview progress or for guidance.
     """
 
     prev_sample: paddle.Tensor
-    pred_original_sample: Optional[paddle.Tensor] = None
+    pred_original_sample: paddle.Tensor
 
 
 def betas_for_alpha_bar(num_diffusion_timesteps, max_beta=0.999):
     """
     Create a beta schedule that discretizes the given alpha_t_bar function, which defines the cumulative product of
     (1-beta) over time from t = [0,1].
 
@@ -61,268 +59,263 @@
                      prevent singularities.
 
     Returns:
         betas (`np.ndarray`): the betas used by the scheduler to step the model outputs
     """
 
     def alpha_bar(time_step):
-        return math.cos((time_step + 0.008) / 1.008 * math.pi / 2)**2
+        return math.cos((time_step + 0.008) / 1.008 * math.pi / 2) ** 2
 
     betas = []
     for i in range(num_diffusion_timesteps):
         t1 = i / num_diffusion_timesteps
         t2 = (i + 1) / num_diffusion_timesteps
         betas.append(min(1 - alpha_bar(t2) / alpha_bar(t1), max_beta))
     return paddle.to_tensor(betas, dtype="float32")
 
 
-class DDPMScheduler(SchedulerMixin, ConfigMixin):
+class RePaintScheduler(SchedulerMixin, ConfigMixin):
     """
-    Denoising diffusion probabilistic models (DDPMs) explores the connections between denoising score matching and
-    Langevin dynamics sampling.
+    RePaint is a schedule for DDPM inpainting inside a given mask.
 
     [`~ConfigMixin`] takes care of storing all config attributes that are passed in the scheduler's `__init__`
     function, such as `num_train_timesteps`. They can be accessed via `scheduler.config.num_train_timesteps`.
-    [`~ConfigMixin`] also provides general loading and saving functionality via the [`~ConfigMixin.save_config`] and
-    [`~ConfigMixin.from_config`] functions.
+    [`SchedulerMixin`] provides general loading and saving functionality via the [`SchedulerMixin.save_pretrained`] and
+    [`~SchedulerMixin.from_pretrained`] functions.
 
-    For more details, see the original paper: https://arxiv.org/abs/2006.11239
+    For more details, see the original paper: https://arxiv.org/pdf/2201.09865.pdf
 
     Args:
         num_train_timesteps (`int`): number of diffusion steps used to train the model.
         beta_start (`float`): the starting `beta` value of inference.
         beta_end (`float`): the final `beta` value.
         beta_schedule (`str`):
             the beta schedule, a mapping from a beta range to a sequence of betas for stepping the model. Choose from
             `linear`, `scaled_linear`, or `squaredcos_cap_v2`.
+        eta (`float`):
+            The weight of noise for added noise in a diffusion step. Its value is between 0.0 and 1.0 -0.0 is DDIM and
+            1.0 is DDPM scheduler respectively.
         trained_betas (`np.ndarray`, optional):
             option to pass an array of betas directly to the constructor to bypass `beta_start`, `beta_end` etc.
         variance_type (`str`):
             options to clip the variance used when adding noise to the denoised sample. Choose from `fixed_small`,
             `fixed_small_log`, `fixed_large`, `fixed_large_log`, `learned` or `learned_range`.
         clip_sample (`bool`, default `True`):
             option to clip predicted sample between -1 and 1 for numerical stability.
 
     """
 
+    order = 1
+
     @register_to_config
     def __init__(
         self,
         num_train_timesteps: int = 1000,
         beta_start: float = 0.0001,
         beta_end: float = 0.02,
         beta_schedule: str = "linear",
+        eta: float = 0.0,
         trained_betas: Optional[np.ndarray] = None,
-        variance_type: str = "fixed_small",
         clip_sample: bool = True,
     ):
-
         if trained_betas is not None:
             self.betas = paddle.to_tensor(trained_betas)
         elif beta_schedule == "linear":
-            self.betas = paddle.linspace(beta_start,
-                                         beta_end,
-                                         num_train_timesteps,
-                                         dtype="float32")
+            self.betas = paddle.linspace(beta_start, beta_end, num_train_timesteps, dtype="float32")
         elif beta_schedule == "scaled_linear":
             # this schedule is very specific to the latent diffusion model.
-            self.betas = (paddle.linspace(beta_start**0.5,
-                                          beta_end**0.5,
-                                          num_train_timesteps,
-                                          dtype="float32")**2)
+            self.betas = paddle.linspace(beta_start**0.5, beta_end**0.5, num_train_timesteps, dtype="float32") ** 2
         elif beta_schedule == "squaredcos_cap_v2":
             # Glide cosine schedule
             self.betas = betas_for_alpha_bar(num_train_timesteps)
         elif beta_schedule == "sigmoid":
             # GeoDiff sigmoid schedule
             betas = paddle.linspace(-6, 6, num_train_timesteps)
             self.betas = F.sigmoid(betas) * (beta_end - beta_start) + beta_start
         else:
-            raise NotImplementedError(
-                f"{beta_schedule} does is not implemented for {self.__class__}")
+            raise NotImplementedError(f"{beta_schedule} does is not implemented for {self.__class__}")
 
         self.alphas = 1.0 - self.betas
         self.alphas_cumprod = paddle.cumprod(self.alphas, 0)
         self.one = paddle.to_tensor(1.0)
 
+        self.final_alpha_cumprod = paddle.to_tensor(1.0)
+
         # standard deviation of the initial noise distribution
         self.init_noise_sigma = 1.0
 
         # setable values
         self.num_inference_steps = None
-        self.timesteps = paddle.to_tensor(
-            np.arange(0, num_train_timesteps)[::-1].copy().astype("int64"))
+        self.timesteps = paddle.to_tensor(np.arange(0, num_train_timesteps)[::-1].copy())
 
-        self.variance_type = variance_type
+        self.eta = eta
 
-    def scale_model_input(self,
-                          sample: paddle.Tensor,
-                          timestep: Optional[int] = None) -> paddle.Tensor:
+    def scale_model_input(self, sample: paddle.Tensor, timestep: Optional[int] = None) -> paddle.Tensor:
         """
         Ensures interchangeability with schedulers that need to scale the denoising model input depending on the
         current timestep.
 
         Args:
             sample (`paddle.Tensor`): input sample
             timestep (`int`, optional): current timestep
 
         Returns:
             `paddle.Tensor`: scaled input sample
         """
         return sample
 
-    def set_timesteps(self, num_inference_steps: int):
-        """
-        Sets the discrete timesteps used for the diffusion chain. Supporting function to be run before inference.
-
-        Args:
-            num_inference_steps (`int`):
-                the number of diffusion steps used when generating samples with a pre-trained model.
-        """
-        num_inference_steps = min(self.config.num_train_timesteps,
-                                  num_inference_steps)
+    def set_timesteps(
+        self,
+        num_inference_steps: int,
+        jump_length: int = 10,
+        jump_n_sample: int = 10,
+    ):
+        num_inference_steps = min(self.config.num_train_timesteps, num_inference_steps)
         self.num_inference_steps = num_inference_steps
-        timesteps = np.arange(
-            0, self.config.num_train_timesteps,
-            self.config.num_train_timesteps //
-            self.num_inference_steps)[::-1].copy()
+
+        timesteps = []
+
+        jumps = {}
+        for j in range(0, num_inference_steps - jump_length, jump_length):
+            jumps[j] = jump_n_sample - 1
+
+        t = num_inference_steps
+        while t >= 1:
+            t = t - 1
+            timesteps.append(t)
+
+            if jumps.get(t, 0) > 0:
+                jumps[t] = jumps[t] - 1
+                for _ in range(jump_length):
+                    t = t + 1
+                    timesteps.append(t)
+
+        timesteps = np.array(timesteps) * (self.config.num_train_timesteps // self.num_inference_steps)
         self.timesteps = paddle.to_tensor(timesteps)
 
-    def _get_variance(self, t, predicted_variance=None, variance_type=None):
+    def _get_variance(self, t):
+        prev_timestep = t - self.config.num_train_timesteps // self.num_inference_steps
+
         alpha_prod_t = self.alphas_cumprod[t]
-        alpha_prod_t_prev = self.alphas_cumprod[t - 1] if t > 0 else self.one
+        alpha_prod_t_prev = self.alphas_cumprod[prev_timestep] if prev_timestep >= 0 else self.final_alpha_cumprod
+        beta_prod_t = 1 - alpha_prod_t
+        beta_prod_t_prev = 1 - alpha_prod_t_prev
 
-        # For t > 0, compute predicted variance βt (see formula (6) and (7) from https://arxiv.org/pdf/2006.11239.pdf)
-        # and sample from it to get previous sample
-        # x_{t-1} ~ N(pred_prev_sample, variance) == add variance to pred_sample
-        variance = (1 - alpha_prod_t_prev) / (1 - alpha_prod_t) * self.betas[t]
-
-        if variance_type is None:
-            variance_type = self.config.variance_type
-
-        # hacks - were probably added for training stability
-        if variance_type == "fixed_small":
-            variance = paddle.clip(variance, min=1e-20)
-        # for rl-diffuser https://arxiv.org/abs/2205.09991
-        elif variance_type == "fixed_small_log":
-            variance = paddle.log(paddle.clip(variance, min=1e-20))
-        elif variance_type == "fixed_large":
-            variance = self.betas[t]
-        elif variance_type == "fixed_large_log":
-            # Glide max_log
-            variance = paddle.log(self.betas[t])
-        elif variance_type == "learned":
-            return predicted_variance
-        elif variance_type == "learned_range":
-            min_log = variance
-            max_log = self.betas[t]
-            frac = (predicted_variance + 1) / 2
-            variance = frac * max_log + (1 - frac) * min_log
+        # For t > 0, compute predicted variance βt (see formula (6) and (7) from
+        # https://arxiv.org/pdf/2006.11239.pdf) and sample from it to get
+        # previous sample x_{t-1} ~ N(pred_prev_sample, variance) == add
+        # variance to pred_sample
+        # Is equivalent to formula (16) in https://arxiv.org/pdf/2010.02502.pdf
+        # without eta.
+        # variance = (1 - alpha_prod_t_prev) / (1 - alpha_prod_t) * self.betas[t]
+        variance = (beta_prod_t_prev / beta_prod_t) * (1 - alpha_prod_t / alpha_prod_t_prev)
 
         return variance
 
     def step(
         self,
         model_output: paddle.Tensor,
         timestep: int,
         sample: paddle.Tensor,
-        predict_epsilon=True,
+        original_image: paddle.Tensor,
+        mask: paddle.Tensor,
+        generator: Optional[paddle.Generator] = None,
         return_dict: bool = True,
-    ) -> Union[DDPMSchedulerOutput, Tuple]:
+    ) -> Union[RePaintSchedulerOutput, Tuple]:
         """
         Predict the sample at the previous timestep by reversing the SDE. Core function to propagate the diffusion
         process from the learned model outputs (most often the predicted noise).
 
         Args:
-            model_output (`paddle.Tensor`): direct output from learned diffusion model.
+            model_output (`paddle.Tensor`): direct output from learned
+                diffusion model.
             timestep (`int`): current discrete timestep in the diffusion chain.
             sample (`paddle.Tensor`):
                 current instance of sample being created by diffusion process.
-            predict_epsilon (`bool`):
-                optional flag to use when model predicts the samples directly instead of the noise, epsilon.
-            return_dict (`bool`): option for returning tuple rather than DDPMSchedulerOutput class
+            original_image (`paddle.Tensor`):
+                the original image to inpaint on.
+            mask (`paddle.Tensor`):
+                the mask where 0.0 values define which part of the original image to inpaint (change).
+            generator (`paddle.Generator`, *optional*): random number generator.
+            return_dict (`bool`): option for returning tuple rather than
+                DDPMSchedulerOutput class
 
         Returns:
-            [`~schedulers.scheduling_utils.DDPMSchedulerOutput`] or `tuple`:
-            [`~schedulers.scheduling_utils.DDPMSchedulerOutput`] if `return_dict` is True, otherwise a `tuple`. When
+            [`~schedulers.scheduling_utils.RePaintSchedulerOutput`] or `tuple`:
+            [`~schedulers.scheduling_utils.RePaintSchedulerOutput`] if `return_dict` is True, otherwise a `tuple`. When
             returning a tuple, the first element is the sample tensor.
 
         """
         t = timestep
-
-        if model_output.shape[1] == sample.shape[
-                1] * 2 and self.variance_type in ["learned", "learned_range"]:
-            model_output, predicted_variance = paddle.split(model_output,
-                                                            sample.shape[1],
-                                                            axis=1)
-        else:
-            predicted_variance = None
+        prev_timestep = timestep - self.config.num_train_timesteps // self.num_inference_steps
 
         # 1. compute alphas, betas
         alpha_prod_t = self.alphas_cumprod[t]
-        alpha_prod_t_prev = self.alphas_cumprod[t - 1] if t > 0 else self.one
+        alpha_prod_t_prev = self.alphas_cumprod[prev_timestep] if prev_timestep >= 0 else self.final_alpha_cumprod
         beta_prod_t = 1 - alpha_prod_t
-        beta_prod_t_prev = 1 - alpha_prod_t_prev
 
         # 2. compute predicted original sample from predicted noise also called
         # "predicted x_0" of formula (15) from https://arxiv.org/pdf/2006.11239.pdf
-        if predict_epsilon:
-            pred_original_sample = (sample - beta_prod_t**
-                                    (0.5) * model_output) / alpha_prod_t**(0.5)
-        else:
-            pred_original_sample = model_output
+        pred_original_sample = (sample - beta_prod_t**0.5 * model_output) / alpha_prod_t**0.5
 
         # 3. Clip "predicted x_0"
         if self.config.clip_sample:
             pred_original_sample = paddle.clip(pred_original_sample, -1, 1)
 
-        # 4. Compute coefficients for pred_original_sample x_0 and current sample x_t
-        # See formula (7) from https://arxiv.org/pdf/2006.11239.pdf
-        pred_original_sample_coeff = (alpha_prod_t_prev**(0.5) *
-                                      self.betas[t]) / beta_prod_t
-        current_sample_coeff = self.alphas[t]**(
-            0.5) * beta_prod_t_prev / beta_prod_t
-
-        # 5. Compute predicted previous sample µ_t
-        # See formula (7) from https://arxiv.org/pdf/2006.11239.pdf
-        pred_prev_sample = pred_original_sample_coeff * pred_original_sample + current_sample_coeff * sample
+        # We choose to follow RePaint Algorithm 1 to get x_{t-1}, however we
+        # substitute formula (7) in the algorithm coming from DDPM paper
+        # (formula (4) Algorithm 2 - Sampling) with formula (12) from DDIM paper.
+        # DDIM schedule gives the same results as DDPM with eta = 1.0
+        # Noise is being reused in 7. and 8., but no impact on quality has
+        # been observed.
+
+        # 5. Add noise
+        noise = paddle.randn(model_output.shape, dtype=model_output.dtype, generator=generator)
+        std_dev_t = self.eta * self._get_variance(timestep) ** 0.5
 
-        # 6. Add noise
         variance = 0
-        if t > 0:
-            noise = paddle.randn(model_output.shape, dtype=model_output.dtype)
-            variance = (self._get_variance(
-                t, predicted_variance=predicted_variance)**0.5) * noise
+        if t > 0 and self.eta > 0:
+            variance = std_dev_t * noise
+
+        # 6. compute "direction pointing to x_t" of formula (12)
+        # from https://arxiv.org/pdf/2010.02502.pdf
+        pred_sample_direction = (1 - alpha_prod_t_prev - std_dev_t**2) ** 0.5 * model_output
 
-        pred_prev_sample = pred_prev_sample + variance
+        # 7. compute x_{t-1} of formula (12) from https://arxiv.org/pdf/2010.02502.pdf
+        prev_unknown_part = alpha_prod_t_prev**0.5 * pred_original_sample + pred_sample_direction + variance
+
+        # 8. Algorithm 1 Line 5 https://arxiv.org/pdf/2201.09865.pdf
+        prev_known_part = (alpha_prod_t**0.5) * original_image + ((1 - alpha_prod_t) ** 0.5) * noise
+
+        # 9. Algorithm 1 Line 8 https://arxiv.org/pdf/2201.09865.pdf
+        pred_prev_sample = mask * prev_known_part + (1.0 - mask) * prev_unknown_part
 
         if not return_dict:
-            return (pred_prev_sample, )
+            return (
+                pred_prev_sample,
+                pred_original_sample,
+            )
+
+        return RePaintSchedulerOutput(prev_sample=pred_prev_sample, pred_original_sample=pred_original_sample)
+
+    def undo_step(self, sample, timestep, generator=None):
+        n = self.config.num_train_timesteps // self.num_inference_steps
+
+        for i in range(n):
+            beta = self.betas[timestep + i]
+            noise = paddle.randn(sample.shape, generator=generator)
+
+            # 10. Algorithm 1 Line 10 https://arxiv.org/pdf/2201.09865.pdf
+            sample = (1 - beta) ** 0.5 * sample + beta**0.5 * noise
 
-        return DDPMSchedulerOutput(prev_sample=pred_prev_sample,
-                                   pred_original_sample=pred_original_sample)
+        return sample
 
     def add_noise(
         self,
         original_samples: paddle.Tensor,
         noise: paddle.Tensor,
         timesteps: paddle.Tensor,
     ) -> paddle.Tensor:
-        # Make sure alphas_cumprod and timestep have same dtype as original_samples
-        self.alphas_cumprod = self.alphas_cumprod.astype(original_samples.dtype)
-
-        sqrt_alpha_prod = self.alphas_cumprod[timesteps]**0.5
-        sqrt_alpha_prod = sqrt_alpha_prod.flatten()
-        while len(sqrt_alpha_prod.shape) < len(original_samples.shape):
-            sqrt_alpha_prod = sqrt_alpha_prod.unsqueeze(-1)
-
-        sqrt_one_minus_alpha_prod = (1 - self.alphas_cumprod[timesteps])**0.5
-        sqrt_one_minus_alpha_prod = sqrt_one_minus_alpha_prod.flatten()
-        while len(sqrt_one_minus_alpha_prod.shape) < len(
-                original_samples.shape):
-            sqrt_one_minus_alpha_prod = sqrt_one_minus_alpha_prod.unsqueeze(-1)
-
-        noisy_samples = sqrt_alpha_prod * original_samples + sqrt_one_minus_alpha_prod * noise
-        return noisy_samples
+        raise NotImplementedError("Use `DDPMScheduler.add_noise()` to train for sampling with RePaint.")
 
     def __len__(self):
         return self.config.num_train_timesteps
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/schedulers/scheduling_dpmsolver_multistep.py` & `ppdiffusers-0.9.0/ppdiffusers/schedulers/scheduling_dpmsolver_multistep.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import math
 from typing import List, Optional, Tuple, Union
 
 import numpy as np
 import paddle
 
 from ..configuration_utils import ConfigMixin, register_to_config
+from ..utils import _COMPATIBLE_STABLE_DIFFUSION_SCHEDULERS, deprecate
 from .scheduling_utils import SchedulerMixin, SchedulerOutput
 
 
 def betas_for_alpha_bar(num_diffusion_timesteps, max_beta=0.999):
     """
     Create a beta schedule that discretizes the given alpha_t_bar function, which defines the cumulative product of
     (1-beta) over time from t = [0,1].
@@ -40,22 +41,22 @@
                      prevent singularities.
 
     Returns:
         betas (`np.ndarray`): the betas used by the scheduler to step the model outputs
     """
 
     def alpha_bar(time_step):
-        return math.cos((time_step + 0.008) / 1.008 * math.pi / 2)**2
+        return math.cos((time_step + 0.008) / 1.008 * math.pi / 2) ** 2
 
     betas = []
     for i in range(num_diffusion_timesteps):
         t1 = i / num_diffusion_timesteps
         t2 = (i + 1) / num_diffusion_timesteps
         betas.append(min(1 - alpha_bar(t2) / alpha_bar(t1), max_beta))
-    return paddle.to_tensor(betas, dtype=paddle.float32)
+    return paddle.to_tensor(betas, dtype="float32")
 
 
 class DPMSolverMultistepScheduler(SchedulerMixin, ConfigMixin):
     """
     DPM-Solver (and the improved version DPM-Solver++) is a fast dedicated high-order solver for diffusion ODEs with
     the convergence order guarantee. Empirically, sampling by DPM-Solver with only 20 steps can generate high-quality
     samples, and it can generate quite good samples even in only 10 steps.
@@ -68,33 +69,33 @@
     We also support the "dynamic thresholding" method in Imagen (https://arxiv.org/abs/2205.11487). For pixel-space
     diffusion models, you can set both `algorithm_type="dpmsolver++"` and `thresholding=True` to use the dynamic
     thresholding. Note that the thresholding method is unsuitable for latent-space diffusion models (such as
     stable-diffusion).
 
     [`~ConfigMixin`] takes care of storing all config attributes that are passed in the scheduler's `__init__`
     function, such as `num_train_timesteps`. They can be accessed via `scheduler.config.num_train_timesteps`.
-    [`~ConfigMixin`] also provides general loading and saving functionality via the [`~ConfigMixin.save_config`] and
-    [`~ConfigMixin.from_config`] functions.
+    [`SchedulerMixin`] provides general loading and saving functionality via the [`SchedulerMixin.save_pretrained`] and
+    [`~SchedulerMixin.from_pretrained`] functions.
 
     Args:
         num_train_timesteps (`int`): number of diffusion steps used to train the model.
         beta_start (`float`): the starting `beta` value of inference.
         beta_end (`float`): the final `beta` value.
         beta_schedule (`str`):
             the beta schedule, a mapping from a beta range to a sequence of betas for stepping the model. Choose from
             `linear`, `scaled_linear`, or `squaredcos_cap_v2`.
         trained_betas (`np.ndarray`, optional):
             option to pass an array of betas directly to the constructor to bypass `beta_start`, `beta_end` etc.
         solver_order (`int`, default `2`):
             the order of DPM-Solver; can be `1` or `2` or `3`. We recommend to use `solver_order=2` for guided
             sampling, and `solver_order=3` for unconditional sampling.
-        predict_epsilon (`bool`, default `True`):
-            we currently support both the noise prediction model and the data prediction model. If the model predicts
-            the noise / epsilon, set `predict_epsilon` to `True`. If the model predicts the data / x0 directly, set
-            `predict_epsilon` to `False`.
+        prediction_type (`str`, default `epsilon`, optional):
+            prediction type of the scheduler function, one of `epsilon` (predicting the noise of the diffusion
+            process), `sample` (directly predicting the noisy sample`) or `v_prediction` (see section 2.4
+            https://imagen.research.google/video/paper.pdf)
         thresholding (`bool`, default `False`):
             whether to use the "dynamic thresholding" method (introduced by Imagen, https://arxiv.org/abs/2205.11487).
             For pixel-space diffusion models, you can set both `algorithm_type=dpmsolver++` and `thresholding=True` to
             use the dynamic thresholding. Note that the thresholding method is unsuitable for latent-space diffusion
             models (such as stable-diffusion).
         dynamic_thresholding_ratio (`float`, default `0.995`):
             the ratio for the dynamic thresholding method. Default is `0.995`, the same as Imagen
@@ -113,113 +114,105 @@
             slightly better, so we recommend to use the `midpoint` type.
         lower_order_final (`bool`, default `True`):
             whether to use lower-order solvers in the final steps. Only valid for < 15 inference steps. We empirically
             find this trick can stabilize the sampling of DPM-Solver for steps < 15, especially for steps <= 10.
 
     """
 
-    _compatible_classes = [
-        "DDIMScheduler",
-        "DDPMScheduler",
-        "PNDMScheduler",
-        "LMSDiscreteScheduler",
-        "EulerDiscreteScheduler",
-        "EulerAncestralDiscreteScheduler",
-    ]
+    _compatibles = _COMPATIBLE_STABLE_DIFFUSION_SCHEDULERS.copy()
+    _deprecated_kwargs = ["predict_epsilon"]
+    order = 1
 
     @register_to_config
     def __init__(
         self,
         num_train_timesteps: int = 1000,
         beta_start: float = 0.0001,
         beta_end: float = 0.02,
         beta_schedule: str = "linear",
-        trained_betas: Optional[np.ndarray] = None,
+        trained_betas: Optional[Union[np.ndarray, List[float]]] = None,
         solver_order: int = 2,
-        predict_epsilon: bool = True,
+        prediction_type: str = "epsilon",
         thresholding: bool = False,
         dynamic_thresholding_ratio: float = 0.995,
         sample_max_value: float = 1.0,
         algorithm_type: str = "dpmsolver++",
         solver_type: str = "midpoint",
         lower_order_final: bool = True,
+        **kwargs,
     ):
+        message = (
+            "Please make sure to instantiate your scheduler with `prediction_type` instead. E.g. `scheduler ="
+            " DPMSolverMultistepScheduler.from_pretrained(<model_id>, prediction_type='epsilon')`."
+        )
+        predict_epsilon = deprecate("predict_epsilon", "0.10.0", message, take_from=kwargs)
+        if predict_epsilon is not None:
+            self.register_to_config(prediction_type="epsilon" if predict_epsilon else "sample")
         if trained_betas is not None:
-            self.betas = paddle.to_tensor(trained_betas)
+            self.betas = paddle.to_tensor(trained_betas, dtype="float32")
         elif beta_schedule == "linear":
-            self.betas = paddle.linspace(beta_start,
-                                         beta_end,
-                                         num_train_timesteps,
-                                         dtype=paddle.float32)
+            self.betas = paddle.linspace(beta_start, beta_end, num_train_timesteps, dtype="float32")
         elif beta_schedule == "scaled_linear":
             # this schedule is very specific to the latent diffusion model.
-            self.betas = (paddle.linspace(beta_start**0.5,
-                                          beta_end**0.5,
-                                          num_train_timesteps,
-                                          dtype=paddle.float32)**2)
+            self.betas = paddle.linspace(beta_start**0.5, beta_end**0.5, num_train_timesteps, dtype="float32") ** 2
         elif beta_schedule == "squaredcos_cap_v2":
             # Glide cosine schedule
             self.betas = betas_for_alpha_bar(num_train_timesteps)
         else:
-            raise NotImplementedError(
-                f"{beta_schedule} does is not implemented for {self.__class__}")
+            raise NotImplementedError(f"{beta_schedule} does is not implemented for {self.__class__}")
 
         self.alphas = 1.0 - self.betas
         self.alphas_cumprod = paddle.cumprod(self.alphas, 0)
         # Currently we only support VP-type noise schedule
         self.alpha_t = paddle.sqrt(self.alphas_cumprod)
         self.sigma_t = paddle.sqrt(1 - self.alphas_cumprod)
         self.lambda_t = paddle.log(self.alpha_t) - paddle.log(self.sigma_t)
 
         # standard deviation of the initial noise distribution
         self.init_noise_sigma = 1.0
 
         # settings for DPM-Solver
         if algorithm_type not in ["dpmsolver", "dpmsolver++"]:
-            raise NotImplementedError(
-                f"{algorithm_type} does is not implemented for {self.__class__}"
-            )
+            raise NotImplementedError(f"{algorithm_type} does is not implemented for {self.__class__}")
         if solver_type not in ["midpoint", "heun"]:
-            raise NotImplementedError(
-                f"{solver_type} does is not implemented for {self.__class__}")
+            raise NotImplementedError(f"{solver_type} does is not implemented for {self.__class__}")
 
         # setable values
         self.num_inference_steps = None
-        timesteps = np.linspace(0,
-                                num_train_timesteps - 1,
-                                num_train_timesteps,
-                                dtype=np.float32)[::-1].copy()
+        timesteps = np.linspace(0, num_train_timesteps - 1, num_train_timesteps, dtype=np.float32)[::-1].copy()
         self.timesteps = paddle.to_tensor(timesteps)
         self.model_outputs = [None] * solver_order
         self.lower_order_nums = 0
 
     def set_timesteps(self, num_inference_steps: int):
         """
         Sets the timesteps used for the diffusion chain. Supporting function to be run before inference.
 
         Args:
             num_inference_steps (`int`):
                 the number of diffusion steps used when generating samples with a pre-trained model.
         """
         self.num_inference_steps = num_inference_steps
-        timesteps = (np.linspace(0, self.num_train_timesteps - 1,
-                                 num_inference_steps +
-                                 1).round()[::-1][:-1].copy().astype(np.int64))
+        timesteps = (
+            np.linspace(0, self.num_train_timesteps - 1, num_inference_steps + 1)
+            .round()[::-1][:-1]
+            .copy()
+            .astype(np.int64)
+        )
         self.timesteps = paddle.to_tensor(timesteps)
         self.model_outputs = [
             None,
         ] * self.config.solver_order
         self.lower_order_nums = 0
 
-    def convert_model_output(self, model_output: paddle.Tensor, timestep: int,
-                             sample: paddle.Tensor) -> paddle.Tensor:
+    def convert_model_output(self, model_output: paddle.Tensor, timestep: int, sample: paddle.Tensor) -> paddle.Tensor:
         """
         Convert the model output to the corresponding type that the algorithm (DPM-Solver / DPM-Solver++) needs.
 
-        DPM-Solver is designed to discretize an integral of the noise prediciton model, and DPM-Solver++ is designed to
+        DPM-Solver is designed to discretize an integral of the noise prediction model, and DPM-Solver++ is designed to
         discretize an integral of the data prediction model. So we need to first convert the model output to the
         corresponding type to match the algorithm.
 
         Note that the algorithm type and the model type is decoupled. That is to say, we can use either DPM-Solver or
         DPM-Solver++ for both noise prediction model and data prediction model.
 
         Args:
@@ -229,43 +222,60 @@
                 current instance of sample being created by diffusion process.
 
         Returns:
             `paddle.Tensor`: the converted model output.
         """
         # DPM-Solver++ needs to solve an integral of the data prediction model.
         if self.config.algorithm_type == "dpmsolver++":
-            if self.config.predict_epsilon:
-                alpha_t, sigma_t = self.alpha_t[timestep], self.sigma_t[
-                    timestep]
+            if self.config.prediction_type == "epsilon":
+                alpha_t, sigma_t = self.alpha_t[timestep], self.sigma_t[timestep]
                 x0_pred = (sample - sigma_t * model_output) / alpha_t
-            else:
+            elif self.config.prediction_type == "sample":
                 x0_pred = model_output
+            elif self.config.prediction_type == "v_prediction":
+                alpha_t, sigma_t = self.alpha_t[timestep], self.sigma_t[timestep]
+                x0_pred = alpha_t * sample - sigma_t * model_output
+            else:
+                raise ValueError(
+                    f"prediction_type given as {self.config.prediction_type} must be one of `epsilon`, `sample`, or"
+                    " `v_prediction` for the DPMSolverMultistepScheduler."
+                )
+
             if self.config.thresholding:
                 # Dynamic thresholding in https://arxiv.org/abs/2205.11487
+                orig_dtype = x0_pred.dtype
+                if orig_dtype not in [paddle.float32, paddle.float64]:
+                    x0_pred = x0_pred.cast("float32")
                 dynamic_max_val = paddle.quantile(
-                    paddle.abs(x0_pred).reshape((x0_pred.shape[0], -1)),
-                    self.config.dynamic_thresholding_ratio,
-                    axis=1)
+                    paddle.abs(x0_pred).reshape((x0_pred.shape[0], -1)), self.config.dynamic_thresholding_ratio, axis=1
+                )
                 dynamic_max_val = paddle.maximum(
                     dynamic_max_val,
-                    self.config.sample_max_value *
-                    paddle.ones_like(dynamic_max_val),
-                )[(..., ) + (None, ) * (x0_pred.ndim - 1)]
-                x0_pred = paddle.clip(x0_pred, -dynamic_max_val,
-                                      dynamic_max_val) / dynamic_max_val
+                    self.config.sample_max_value * paddle.ones_like(dynamic_max_val),
+                )[(...,) + (None,) * (x0_pred.ndim - 1)]
+                x0_pred = paddle.clip(x0_pred, -dynamic_max_val, dynamic_max_val) / dynamic_max_val
+                x0_pred = x0_pred.cast(orig_dtype)
             return x0_pred
         # DPM-Solver needs to solve an integral of the noise prediction model.
         elif self.config.algorithm_type == "dpmsolver":
-            if self.config.predict_epsilon:
+            if self.config.prediction_type == "epsilon":
                 return model_output
-            else:
-                alpha_t, sigma_t = self.alpha_t[timestep], self.sigma_t[
-                    timestep]
+            elif self.config.prediction_type == "sample":
+                alpha_t, sigma_t = self.alpha_t[timestep], self.sigma_t[timestep]
                 epsilon = (sample - alpha_t * model_output) / sigma_t
                 return epsilon
+            elif self.config.prediction_type == "v_prediction":
+                alpha_t, sigma_t = self.alpha_t[timestep], self.sigma_t[timestep]
+                epsilon = alpha_t * model_output + sigma_t * sample
+                return epsilon
+            else:
+                raise ValueError(
+                    f"prediction_type given as {self.config.prediction_type} must be one of `epsilon`, `sample`, or"
+                    " `v_prediction` for the DPMSolverMultistepScheduler."
+                )
 
     def dpm_solver_first_order_update(
         self,
         model_output: paddle.Tensor,
         timestep: int,
         prev_timestep: int,
         sample: paddle.Tensor,
@@ -281,27 +291,22 @@
             prev_timestep (`int`): previous discrete timestep in the diffusion chain.
             sample (`paddle.Tensor`):
                 current instance of sample being created by diffusion process.
 
         Returns:
             `paddle.Tensor`: the sample tensor at the previous timestep.
         """
-        lambda_t, lambda_s = self.lambda_t[prev_timestep], self.lambda_t[
-            timestep]
+        lambda_t, lambda_s = self.lambda_t[prev_timestep], self.lambda_t[timestep]
         alpha_t, alpha_s = self.alpha_t[prev_timestep], self.alpha_t[timestep]
         sigma_t, sigma_s = self.sigma_t[prev_timestep], self.sigma_t[timestep]
         h = lambda_t - lambda_s
         if self.config.algorithm_type == "dpmsolver++":
-            x_t = (sigma_t /
-                   sigma_s) * sample - (alpha_t *
-                                        (paddle.exp(-h) - 1.0)) * model_output
+            x_t = (sigma_t / sigma_s) * sample - (alpha_t * (paddle.exp(-h) - 1.0)) * model_output
         elif self.config.algorithm_type == "dpmsolver":
-            x_t = (alpha_t /
-                   alpha_s) * sample - (sigma_t *
-                                        (paddle.exp(h) - 1.0)) * model_output
+            x_t = (alpha_t / alpha_s) * sample - (sigma_t * (paddle.exp(h) - 1.0)) * model_output
         return x_t
 
     def multistep_dpm_solver_second_order_update(
         self,
         model_output_list: List[paddle.Tensor],
         timestep_list: List[int],
         prev_timestep: int,
@@ -319,41 +324,48 @@
                 current instance of sample being created by diffusion process.
 
         Returns:
             `paddle.Tensor`: the sample tensor at the previous timestep.
         """
         t, s0, s1 = prev_timestep, timestep_list[-1], timestep_list[-2]
         m0, m1 = model_output_list[-1], model_output_list[-2]
-        lambda_t, lambda_s0, lambda_s1 = self.lambda_t[t], self.lambda_t[
-            s0], self.lambda_t[s1]
+        lambda_t, lambda_s0, lambda_s1 = self.lambda_t[t], self.lambda_t[s0], self.lambda_t[s1]
         alpha_t, alpha_s0 = self.alpha_t[t], self.alpha_t[s0]
         sigma_t, sigma_s0 = self.sigma_t[t], self.sigma_t[s0]
         h, h_0 = lambda_t - lambda_s0, lambda_s0 - lambda_s1
         r0 = h_0 / h
         D0, D1 = m0, (1.0 / r0) * (m0 - m1)
         if self.config.algorithm_type == "dpmsolver++":
             # See https://arxiv.org/abs/2211.01095 for detailed derivations
             if self.config.solver_type == "midpoint":
-                x_t = ((sigma_t / sigma_s0) * sample -
-                       (alpha_t * (paddle.exp(-h) - 1.0)) * D0 - 0.5 *
-                       (alpha_t * (paddle.exp(-h) - 1.0)) * D1)
+                x_t = (
+                    (sigma_t / sigma_s0) * sample
+                    - (alpha_t * (paddle.exp(-h) - 1.0)) * D0
+                    - 0.5 * (alpha_t * (paddle.exp(-h) - 1.0)) * D1
+                )
             elif self.config.solver_type == "heun":
-                x_t = ((sigma_t / sigma_s0) * sample -
-                       (alpha_t * (paddle.exp(-h) - 1.0)) * D0 +
-                       (alpha_t * ((paddle.exp(-h) - 1.0) / h + 1.0)) * D1)
+                x_t = (
+                    (sigma_t / sigma_s0) * sample
+                    - (alpha_t * (paddle.exp(-h) - 1.0)) * D0
+                    + (alpha_t * ((paddle.exp(-h) - 1.0) / h + 1.0)) * D1
+                )
         elif self.config.algorithm_type == "dpmsolver":
             # See https://arxiv.org/abs/2206.00927 for detailed derivations
             if self.config.solver_type == "midpoint":
-                x_t = ((alpha_t / alpha_s0) * sample -
-                       (sigma_t * (paddle.exp(h) - 1.0)) * D0 - 0.5 *
-                       (sigma_t * (paddle.exp(h) - 1.0)) * D1)
+                x_t = (
+                    (alpha_t / alpha_s0) * sample
+                    - (sigma_t * (paddle.exp(h) - 1.0)) * D0
+                    - 0.5 * (sigma_t * (paddle.exp(h) - 1.0)) * D1
+                )
             elif self.config.solver_type == "heun":
-                x_t = ((alpha_t / alpha_s0) * sample -
-                       (sigma_t * (paddle.exp(h) - 1.0)) * D0 -
-                       (sigma_t * ((paddle.exp(h) - 1.0) / h - 1.0)) * D1)
+                x_t = (
+                    (alpha_t / alpha_s0) * sample
+                    - (sigma_t * (paddle.exp(h) - 1.0)) * D0
+                    - (sigma_t * ((paddle.exp(h) - 1.0) / h - 1.0)) * D1
+                )
         return x_t
 
     def multistep_dpm_solver_third_order_update(
         self,
         model_output_list: List[paddle.Tensor],
         timestep_list: List[int],
         prev_timestep: int,
@@ -369,18 +381,16 @@
             prev_timestep (`int`): previous discrete timestep in the diffusion chain.
             sample (`paddle.Tensor`):
                 current instance of sample being created by diffusion process.
 
         Returns:
             `paddle.Tensor`: the sample tensor at the previous timestep.
         """
-        t, s0, s1, s2 = prev_timestep, timestep_list[-1], timestep_list[
-            -2], timestep_list[-3]
-        m0, m1, m2 = model_output_list[-1], model_output_list[
-            -2], model_output_list[-3]
+        t, s0, s1, s2 = prev_timestep, timestep_list[-1], timestep_list[-2], timestep_list[-3]
+        m0, m1, m2 = model_output_list[-1], model_output_list[-2], model_output_list[-3]
         lambda_t, lambda_s0, lambda_s1, lambda_s2 = (
             self.lambda_t[t],
             self.lambda_t[s0],
             self.lambda_t[s1],
             self.lambda_t[s2],
         )
         alpha_t, alpha_s0 = self.alpha_t[t], self.alpha_t[s0]
@@ -389,24 +399,28 @@
         r0, r1 = h_0 / h, h_1 / h
         D0 = m0
         D1_0, D1_1 = (1.0 / r0) * (m0 - m1), (1.0 / r1) * (m1 - m2)
         D1 = D1_0 + (r0 / (r0 + r1)) * (D1_0 - D1_1)
         D2 = (1.0 / (r0 + r1)) * (D1_0 - D1_1)
         if self.config.algorithm_type == "dpmsolver++":
             # See https://arxiv.org/abs/2206.00927 for detailed derivations
-            x_t = ((sigma_t / sigma_s0) * sample -
-                   (alpha_t * (paddle.exp(-h) - 1.0)) * D0 +
-                   (alpha_t * ((paddle.exp(-h) - 1.0) / h + 1.0)) * D1 -
-                   (alpha_t * ((paddle.exp(-h) - 1.0 + h) / h**2 - 0.5)) * D2)
+            x_t = (
+                (sigma_t / sigma_s0) * sample
+                - (alpha_t * (paddle.exp(-h) - 1.0)) * D0
+                + (alpha_t * ((paddle.exp(-h) - 1.0) / h + 1.0)) * D1
+                - (alpha_t * ((paddle.exp(-h) - 1.0 + h) / h**2 - 0.5)) * D2
+            )
         elif self.config.algorithm_type == "dpmsolver":
             # See https://arxiv.org/abs/2206.00927 for detailed derivations
-            x_t = ((alpha_t / alpha_s0) * sample -
-                   (sigma_t * (paddle.exp(h) - 1.0)) * D0 -
-                   (sigma_t * ((paddle.exp(h) - 1.0) / h - 1.0)) * D1 -
-                   (sigma_t * ((paddle.exp(h) - 1.0 - h) / h**2 - 0.5)) * D2)
+            x_t = (
+                (alpha_t / alpha_s0) * sample
+                - (sigma_t * (paddle.exp(h) - 1.0)) * D0
+                - (sigma_t * ((paddle.exp(h) - 1.0) / h - 1.0)) * D1
+                - (sigma_t * ((paddle.exp(h) - 1.0 - h) / h**2 - 0.5)) * D2
+            )
         return x_t
 
     def step(
         self,
         model_output: paddle.Tensor,
         timestep: int,
         sample: paddle.Tensor,
@@ -433,53 +447,49 @@
             )
 
         step_index = (self.timesteps == timestep).nonzero()
         if len(step_index) == 0:
             step_index = len(self.timesteps) - 1
         else:
             step_index = step_index.item()
-        prev_timestep = 0 if step_index == len(
-            self.timesteps) - 1 else self.timesteps[step_index + 1]
-        lower_order_final = ((step_index == len(self.timesteps) - 1)
-                             and self.config.lower_order_final
-                             and len(self.timesteps) < 15)
-        lower_order_second = ((step_index == len(self.timesteps) - 2)
-                              and self.config.lower_order_final
-                              and len(self.timesteps) < 15)
+        prev_timestep = 0 if step_index == len(self.timesteps) - 1 else self.timesteps[step_index + 1]
+        lower_order_final = (
+            (step_index == len(self.timesteps) - 1) and self.config.lower_order_final and len(self.timesteps) < 15
+        )
+        lower_order_second = (
+            (step_index == len(self.timesteps) - 2) and self.config.lower_order_final and len(self.timesteps) < 15
+        )
 
         model_output = self.convert_model_output(model_output, timestep, sample)
         for i in range(self.config.solver_order - 1):
             self.model_outputs[i] = self.model_outputs[i + 1]
         self.model_outputs[-1] = model_output
 
         if self.config.solver_order == 1 or self.lower_order_nums < 1 or lower_order_final:
-            prev_sample = self.dpm_solver_first_order_update(
-                model_output, timestep, prev_timestep, sample)
+            prev_sample = self.dpm_solver_first_order_update(model_output, timestep, prev_timestep, sample)
         elif self.config.solver_order == 2 or self.lower_order_nums < 2 or lower_order_second:
             timestep_list = [self.timesteps[step_index - 1], timestep]
             prev_sample = self.multistep_dpm_solver_second_order_update(
-                self.model_outputs, timestep_list, prev_timestep, sample)
+                self.model_outputs, timestep_list, prev_timestep, sample
+            )
         else:
-            timestep_list = [
-                self.timesteps[step_index - 2], self.timesteps[step_index - 1],
-                timestep
-            ]
+            timestep_list = [self.timesteps[step_index - 2], self.timesteps[step_index - 1], timestep]
             prev_sample = self.multistep_dpm_solver_third_order_update(
-                self.model_outputs, timestep_list, prev_timestep, sample)
+                self.model_outputs, timestep_list, prev_timestep, sample
+            )
 
         if self.lower_order_nums < self.config.solver_order:
             self.lower_order_nums += 1
 
         if not return_dict:
-            return (prev_sample, )
+            return (prev_sample,)
 
         return SchedulerOutput(prev_sample=prev_sample)
 
-    def scale_model_input(self, sample: paddle.Tensor, *args,
-                          **kwargs) -> paddle.Tensor:
+    def scale_model_input(self, sample: paddle.Tensor, *args, **kwargs) -> paddle.Tensor:
         """
         Ensures interchangeability with schedulers that need to scale the denoising model input depending on the
         current timestep.
 
         Args:
             sample (`paddle.Tensor`): input sample
 
@@ -490,26 +500,25 @@
 
     def add_noise(
         self,
         original_samples: paddle.Tensor,
         noise: paddle.Tensor,
         timesteps: paddle.Tensor,
     ) -> paddle.Tensor:
-        # Make sure alphas_cumprod and timestep have same device and dtype as original_samples
-        self.alphas_cumprod = self.alphas_cumprod.astype(original_samples.dtype)
+        # Make sure alphas_cumprod and timestep have same dtype as original_samples
+        self.alphas_cumprod = self.alphas_cumprod.cast(original_samples.dtype)
 
-        sqrt_alpha_prod = self.alphas_cumprod[timesteps]**0.5
+        sqrt_alpha_prod = self.alphas_cumprod[timesteps] ** 0.5
         sqrt_alpha_prod = sqrt_alpha_prod.flatten()
         while len(sqrt_alpha_prod.shape) < len(original_samples.shape):
             sqrt_alpha_prod = sqrt_alpha_prod.unsqueeze(-1)
 
-        sqrt_one_minus_alpha_prod = (1 - self.alphas_cumprod[timesteps])**0.5
+        sqrt_one_minus_alpha_prod = (1 - self.alphas_cumprod[timesteps]) ** 0.5
         sqrt_one_minus_alpha_prod = sqrt_one_minus_alpha_prod.flatten()
-        while len(sqrt_one_minus_alpha_prod.shape) < len(
-                original_samples.shape):
+        while len(sqrt_one_minus_alpha_prod.shape) < len(original_samples.shape):
             sqrt_one_minus_alpha_prod = sqrt_one_minus_alpha_prod.unsqueeze(-1)
 
         noisy_samples = sqrt_alpha_prod * original_samples + sqrt_one_minus_alpha_prod * noise
         return noisy_samples
 
     def __len__(self):
         return self.config.num_train_timesteps
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/schedulers/scheduling_euler_ancestral_discrete.py` & `ppdiffusers-0.9.0/ppdiffusers/schedulers/scheduling_euler_ancestral_discrete.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,27 +10,28 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from dataclasses import dataclass
-from typing import Optional, Tuple, Union
+from typing import List, Optional, Tuple, Union
 
 import numpy as np
 import paddle
 
 from ..configuration_utils import ConfigMixin, register_to_config
-from ..utils import BaseOutput, logging
+from ..utils import _COMPATIBLE_STABLE_DIFFUSION_SCHEDULERS, BaseOutput, logging
 from .scheduling_utils import SchedulerMixin
 
 logger = logging.get_logger(__name__)  # pylint: disable=invalid-name
 
 
 @dataclass
+# Copied from diffusers.schedulers.scheduling_ddpm.DDPMSchedulerOutput with DDPM->EulerAncestralDiscrete
 class EulerAncestralDiscreteSchedulerOutput(BaseOutput):
     """
     Output class for the scheduler's step function output.
 
     Args:
         prev_sample (`paddle.Tensor` of shape `(batch_size, num_channels, height, width)` for images):
             Computed sample (x_{t-1}) of previous timestep. `prev_sample` should be used as next model input in the
@@ -47,49 +48,47 @@
 class EulerAncestralDiscreteScheduler(SchedulerMixin, ConfigMixin):
     """
     Ancestral sampling with Euler method steps. Based on the original k-diffusion implementation by Katherine Crowson:
     https://github.com/crowsonkb/k-diffusion/blob/481677d114f6ea445aa009cf5bd7a9cdee909e47/k_diffusion/sampling.py#L72
 
     [`~ConfigMixin`] takes care of storing all config attributes that are passed in the scheduler's `__init__`
     function, such as `num_train_timesteps`. They can be accessed via `scheduler.config.num_train_timesteps`.
-    [`~ConfigMixin`] also provides general loading and saving functionality via the [`~ConfigMixin.save_config`] and
-    [`~ConfigMixin.from_config`] functions.
+    [`SchedulerMixin`] provides general loading and saving functionality via the [`SchedulerMixin.save_pretrained`] and
+    [`~SchedulerMixin.from_pretrained`] functions.
 
     Args:
         num_train_timesteps (`int`): number of diffusion steps used to train the model.
         beta_start (`float`): the starting `beta` value of inference.
         beta_end (`float`): the final `beta` value.
         beta_schedule (`str`):
             the beta schedule, a mapping from a beta range to a sequence of betas for stepping the model. Choose from
             `linear` or `scaled_linear`.
         trained_betas (`np.ndarray`, optional):
             option to pass an array of betas directly to the constructor to bypass `beta_start`, `beta_end` etc.
-
+        prediction_type (`str`, default `epsilon`, optional):
+            prediction type of the scheduler function, one of `epsilon` (predicting the noise of the diffusion
+            process), `sample` (directly predicting the noisy sample`) or `v_prediction` (see section 2.4
+            https://imagen.research.google/video/paper.pdf)
     """
 
-    _compatible_classes = [
-        "DDIMScheduler",
-        "DDPMScheduler",
-        "LMSDiscreteScheduler",
-        "PNDMScheduler",
-        "EulerDiscreteScheduler",
-        "DPMSolverMultistepScheduler",
-    ]
+    _compatibles = _COMPATIBLE_STABLE_DIFFUSION_SCHEDULERS.copy()
+    order = 1
 
     @register_to_config
     def __init__(
         self,
         num_train_timesteps: int = 1000,
         beta_start: float = 0.0001,
         beta_end: float = 0.02,
         beta_schedule: str = "linear",
-        trained_betas: Optional[np.ndarray] = None,
+        trained_betas: Optional[Union[np.ndarray, List[float]]] = None,
+        prediction_type: str = "epsilon",
     ):
         if trained_betas is not None:
-            self.betas = paddle.to_tensor(trained_betas)
+            self.betas = paddle.to_tensor(trained_betas, dtype="float32")
         elif beta_schedule == "linear":
             self.betas = paddle.linspace(beta_start, beta_end, num_train_timesteps, dtype="float32")
         elif beta_schedule == "scaled_linear":
             # this schedule is very specific to the latent diffusion model.
             self.betas = paddle.linspace(beta_start**0.5, beta_end**0.5, num_train_timesteps, dtype="float32") ** 2
         else:
             raise NotImplementedError(f"{beta_schedule} does is not implemented for {self.__class__}")
@@ -103,15 +102,15 @@
 
         # standard deviation of the initial noise distribution
         self.init_noise_sigma = self.sigmas.max()
 
         # setable values
         self.num_inference_steps = None
         timesteps = np.linspace(0, num_train_timesteps - 1, num_train_timesteps, dtype=float)[::-1].copy()
-        self.timesteps = paddle.to_tensor(timesteps)
+        self.timesteps = paddle.to_tensor(timesteps, dtype="float32")
         self.is_scale_input_called = False
 
     def scale_model_input(self, sample: paddle.Tensor, timestep: Union[float, paddle.Tensor]) -> paddle.Tensor:
         """
         Scales the denoising model input by `(sigma**2 + 1) ** 0.5` to match the Euler algorithm.
 
         Args:
@@ -138,63 +137,73 @@
         self.num_inference_steps = num_inference_steps
 
         timesteps = np.linspace(0, self.config.num_train_timesteps - 1, num_inference_steps, dtype=float)[::-1].copy()
         sigmas = np.array(((1 - self.alphas_cumprod) / self.alphas_cumprod) ** 0.5)
         sigmas = np.interp(timesteps, np.arange(0, len(sigmas)), sigmas)
         sigmas = np.concatenate([sigmas, [0.0]]).astype(np.float32)
         self.sigmas = paddle.to_tensor(sigmas)
-        self.timesteps = paddle.to_tensor(timesteps)
+        self.timesteps = paddle.to_tensor(timesteps, dtype="float32")
 
     def step(
         self,
         model_output: paddle.Tensor,
         timestep: Union[float, paddle.Tensor],
         sample: paddle.Tensor,
+        generator: Optional[paddle.Generator] = None,
         return_dict: bool = True,
     ) -> Union[EulerAncestralDiscreteSchedulerOutput, Tuple]:
         """
         Predict the sample at the previous timestep by reversing the SDE. Core function to propagate the diffusion
         process from the learned model outputs (most often the predicted noise).
 
         Args:
             model_output (`paddle.Tensor`): direct output from learned diffusion model.
             timestep (`float`): current timestep in the diffusion chain.
             sample (`paddle.Tensor`):
                 current instance of sample being created by diffusion process.
+            generator (`paddle.Generator`, optional): Random number generator.
             return_dict (`bool`): option for returning tuple rather than EulerAncestralDiscreteSchedulerOutput class
 
         Returns:
             [`~schedulers.scheduling_utils.EulerAncestralDiscreteSchedulerOutput`] or `tuple`:
             [`~schedulers.scheduling_utils.EulerAncestralDiscreteSchedulerOutput`] if `return_dict` is True, otherwise
             a `tuple`. When returning a tuple, the first element is the sample tensor.
 
         """
         if not self.is_scale_input_called:
-            logger.warn(
+            logger.warning(
                 "The `scale_model_input` function should be called before `step` to ensure correct denoising. "
                 "See `StableDiffusionPipeline` for a usage example."
             )
         step_index = (self.timesteps == timestep).nonzero().item()
         sigma = self.sigmas[step_index]
 
         # 1. compute predicted original sample (x_0) from sigma-scaled predicted noise
-        pred_original_sample = sample - sigma * model_output
+        if self.config.prediction_type == "epsilon":
+            pred_original_sample = sample - sigma * model_output
+        elif self.config.prediction_type == "v_prediction":
+            # * c_out + input * c_skip
+            pred_original_sample = model_output * (-sigma / (sigma**2 + 1) ** 0.5) + (sample / (sigma**2 + 1))
+        else:
+            raise ValueError(
+                f"prediction_type given as {self.config.prediction_type} must be one of `epsilon`, or `v_prediction`"
+            )
         sigma_from = self.sigmas[step_index]
         sigma_to = self.sigmas[step_index + 1]
         sigma_up = (sigma_to**2 * (sigma_from**2 - sigma_to**2) / sigma_from**2) ** 0.5
         sigma_down = (sigma_to**2 - sigma_up**2) ** 0.5
 
         # 2. Convert to an ODE derivative
         derivative = (sample - pred_original_sample) / sigma
 
         dt = sigma_down - sigma
 
         prev_sample = sample + derivative * dt
 
-        noise = paddle.randn(model_output.shape, dtype=model_output.dtype)
+        noise = paddle.randn(model_output.shape, dtype=model_output.dtype, generator=generator)
 
         prev_sample = prev_sample + noise * sigma_up
 
         if not return_dict:
             return (prev_sample,)
 
         return EulerAncestralDiscreteSchedulerOutput(
@@ -203,16 +212,16 @@
 
     def add_noise(
         self,
         original_samples: paddle.Tensor,
         noise: paddle.Tensor,
         timesteps: paddle.Tensor,
     ) -> paddle.Tensor:
-        # Make sure sigmas and timesteps have the same device and dtype as original_samples
-        self.sigmas = self.sigmas.astype(original_samples.dtype)
+        # Make sure sigmas and timesteps have the same dtype as original_samples
+        self.sigmas = self.sigmas.cast(original_samples.dtype)
 
         schedule_timesteps = self.timesteps
         step_indices = [(schedule_timesteps == t).nonzero().item() for t in timesteps]
 
         sigma = self.sigmas[step_indices].flatten()
         while len(sigma.shape) < len(original_samples.shape):
             sigma = sigma.unsqueeze(-1)
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/schedulers/scheduling_karras_ve.py` & `ppdiffusers-0.9.0/ppdiffusers/schedulers/scheduling_karras_ve.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,16 +52,16 @@
 
     [1] Karras, Tero, et al. "Elucidating the Design Space of Diffusion-Based Generative Models."
     https://arxiv.org/abs/2206.00364 [2] Song, Yang, et al. "Score-based generative modeling through stochastic
     differential equations." https://arxiv.org/abs/2011.13456
 
     [`~ConfigMixin`] takes care of storing all config attributes that are passed in the scheduler's `__init__`
     function, such as `num_train_timesteps`. They can be accessed via `scheduler.config.num_train_timesteps`.
-    [`~ConfigMixin`] also provides general loading and saving functionality via the [`~ConfigMixin.save_config`] and
-    [`~ConfigMixin.from_config`] functions.
+    [`SchedulerMixin`] provides general loading and saving functionality via the [`SchedulerMixin.save_pretrained`] and
+    [`~SchedulerMixin.from_pretrained`] functions.
 
     For more details on the parameters, see the original paper's Appendix E.: "Elucidating the Design Space of
     Diffusion-Based Generative Models." https://arxiv.org/abs/2206.00364. The grid search values used to find the
     optimal {s_noise, s_churn, s_min, s_max} for a specific model are described in Table 5 of the paper.
 
     Args:
         sigma_min (`float`): minimum noise magnitude
@@ -73,36 +73,35 @@
         s_min (`float`): the start value of the sigma range where we add noise (enable stochasticity).
             A reasonable range is [0, 10].
         s_max (`float`): the end value of the sigma range where we add noise.
             A reasonable range is [0.2, 80].
 
     """
 
+    order = 2
+
     @register_to_config
     def __init__(
         self,
         sigma_min: float = 0.02,
         sigma_max: float = 100,
         s_noise: float = 1.007,
         s_churn: float = 80,
         s_min: float = 0.05,
         s_max: float = 50,
     ):
-
         # standard deviation of the initial noise distribution
         self.init_noise_sigma = sigma_max
 
         # setable values
         self.num_inference_steps: int = None
         self.timesteps: paddle.Tensor = None
         self.schedule: paddle.Tensor = None  # sigma(t_i)
 
-    def scale_model_input(self,
-                          sample: paddle.Tensor,
-                          timestep: Optional[int] = None) -> paddle.Tensor:
+    def scale_model_input(self, sample: paddle.Tensor, timestep: Optional[int] = None) -> paddle.Tensor:
         """
         Ensures interchangeability with schedulers that need to scale the denoising model input depending on the
         current timestep.
 
         Args:
             sample (`paddle.Tensor`): input sample
             timestep (`int`, optional): current timestep
@@ -120,40 +119,41 @@
             num_inference_steps (`int`):
                 the number of diffusion steps used when generating samples with a pre-trained model.
 
         """
         self.num_inference_steps = num_inference_steps
         timesteps = np.arange(0, self.num_inference_steps)[::-1].copy()
         self.timesteps = paddle.to_tensor(timesteps)
-        schedule = [(self.config.sigma_max**2 *
-                     (self.config.sigma_min**2 / self.config.sigma_max**2)
-                     **(i / (num_inference_steps - 1))) for i in self.timesteps]
+        schedule = [
+            (
+                self.config.sigma_max**2
+                * (self.config.sigma_min**2 / self.config.sigma_max**2) ** (i / (num_inference_steps - 1))
+            )
+            for i in self.timesteps
+        ]
         self.schedule = paddle.to_tensor(schedule, dtype="float32")
 
     def add_noise_to_input(
-        self,
-        sample: paddle.Tensor,
-        sigma: float,
+        self, sample: paddle.Tensor, sigma: float, generator: Optional[paddle.Generator] = None
     ) -> Tuple[paddle.Tensor, float]:
         """
         Explicit Langevin-like "churn" step of adding noise to the sample according to a factor gamma_i ≥ 0 to reach a
         higher noise level sigma_hat = sigma_i + gamma_i*sigma_i.
 
         TODO Args:
         """
         if self.config.s_min <= sigma <= self.config.s_max:
-            gamma = min(self.config.s_churn / self.num_inference_steps,
-                        2**0.5 - 1)
+            gamma = min(self.config.s_churn / self.num_inference_steps, 2**0.5 - 1)
         else:
             gamma = 0
 
         # sample eps ~ N(0, S_noise^2 * I)
-        eps = self.config.s_noise * paddle.randn(sample.shape)
+        eps = self.config.s_noise * paddle.randn(sample.shape, generator=generator)
         sigma_hat = sigma + gamma * sigma
-        sample_hat = sample + ((sigma_hat**2 - sigma**2)**0.5 * eps)
+        sample_hat = sample + ((sigma_hat**2 - sigma**2) ** 0.5 * eps)
 
         return sample_hat, sigma_hat
 
     def step(
         self,
         model_output: paddle.Tensor,
         sigma_hat: float,
@@ -183,17 +183,17 @@
         pred_original_sample = sample_hat + sigma_hat * model_output
         derivative = (sample_hat - pred_original_sample) / sigma_hat
         sample_prev = sample_hat + (sigma_prev - sigma_hat) * derivative
 
         if not return_dict:
             return (sample_prev, derivative)
 
-        return KarrasVeOutput(prev_sample=sample_prev,
-                              derivative=derivative,
-                              pred_original_sample=pred_original_sample)
+        return KarrasVeOutput(
+            prev_sample=sample_prev, derivative=derivative, pred_original_sample=pred_original_sample
+        )
 
     def step_correct(
         self,
         model_output: paddle.Tensor,
         sigma_hat: float,
         sigma_prev: float,
         sample_hat: paddle.Tensor,
@@ -215,19 +215,18 @@
 
         Returns:
             prev_sample (TODO): updated sample in the diffusion chain. derivative (TODO): TODO
 
         """
         pred_original_sample = sample_prev + sigma_prev * model_output
         derivative_corr = (sample_prev - pred_original_sample) / sigma_prev
-        sample_prev = sample_hat + (sigma_prev - sigma_hat) * (
-            0.5 * derivative + 0.5 * derivative_corr)
+        sample_prev = sample_hat + (sigma_prev - sigma_hat) * (0.5 * derivative + 0.5 * derivative_corr)
 
         if not return_dict:
             return (sample_prev, derivative)
 
-        return KarrasVeOutput(prev_sample=sample_prev,
-                              derivative=derivative,
-                              pred_original_sample=pred_original_sample)
+        return KarrasVeOutput(
+            prev_sample=sample_prev, derivative=derivative, pred_original_sample=pred_original_sample
+        )
 
     def add_noise(self, original_samples, noise, timesteps):
         raise NotImplementedError()
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/schedulers/scheduling_lms_discrete.py` & `ppdiffusers-0.9.0/ppdiffusers/schedulers/scheduling_lms_discrete.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,28 +10,27 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import warnings
 from dataclasses import dataclass
-from typing import Optional, Tuple, Union
+from typing import List, Optional, Tuple, Union
 
 import numpy as np
 import paddle
-
 from scipy import integrate
 
 from ..configuration_utils import ConfigMixin, register_to_config
-from ..utils import BaseOutput, deprecate
+from ..utils import _COMPATIBLE_STABLE_DIFFUSION_SCHEDULERS, BaseOutput
 from .scheduling_utils import SchedulerMixin
 
 
 @dataclass
-# Copied from ppdiffusers.schedulers.scheduling_ddpm.DDPMSchedulerOutput with DDPM->LMSDiscrete
+# Copied from diffusers.schedulers.scheduling_ddpm.DDPMSchedulerOutput with DDPM->LMSDiscrete
 class LMSDiscreteSchedulerOutput(BaseOutput):
     """
     Output class for the scheduler's step function output.
 
     Args:
         prev_sample (`paddle.Tensor` of shape `(batch_size, num_channels, height, width)` for images):
             Computed sample (x_{t-1}) of previous timestep. `prev_sample` should be used as next model input in the
@@ -49,93 +48,86 @@
     """
     Linear Multistep Scheduler for discrete beta schedules. Based on the original k-diffusion implementation by
     Katherine Crowson:
     https://github.com/crowsonkb/k-diffusion/blob/481677d114f6ea445aa009cf5bd7a9cdee909e47/k_diffusion/sampling.py#L181
 
     [`~ConfigMixin`] takes care of storing all config attributes that are passed in the scheduler's `__init__`
     function, such as `num_train_timesteps`. They can be accessed via `scheduler.config.num_train_timesteps`.
-    [`~ConfigMixin`] also provides general loading and saving functionality via the [`~ConfigMixin.save_config`] and
-    [`~ConfigMixin.from_config`] functions.
+    [`SchedulerMixin`] provides general loading and saving functionality via the [`SchedulerMixin.save_pretrained`] and
+    [`~SchedulerMixin.from_pretrained`] functions.
 
     Args:
         num_train_timesteps (`int`): number of diffusion steps used to train the model.
         beta_start (`float`): the starting `beta` value of inference.
         beta_end (`float`): the final `beta` value.
         beta_schedule (`str`):
             the beta schedule, a mapping from a beta range to a sequence of betas for stepping the model. Choose from
             `linear` or `scaled_linear`.
         trained_betas (`np.ndarray`, optional):
             option to pass an array of betas directly to the constructor to bypass `beta_start`, `beta_end` etc.
-
+        prediction_type (`str`, default `epsilon`, optional):
+            prediction type of the scheduler function, one of `epsilon` (predicting the noise of the diffusion
+            process), `sample` (directly predicting the noisy sample`) or `v_prediction` (see section 2.4
+            https://imagen.research.google/video/paper.pdf)
     """
 
+    _compatibles = _COMPATIBLE_STABLE_DIFFUSION_SCHEDULERS.copy()
+    order = 1
+
     @register_to_config
     def __init__(
         self,
         num_train_timesteps: int = 1000,
         beta_start: float = 0.0001,
         beta_end: float = 0.02,
         beta_schedule: str = "linear",
-        trained_betas: Optional[np.ndarray] = None,
+        trained_betas: Optional[Union[np.ndarray, List[float]]] = None,
+        prediction_type: str = "epsilon",
     ):
-
         if trained_betas is not None:
-            self.betas = paddle.to_tensor(trained_betas)
+            self.betas = paddle.to_tensor(trained_betas, dtype="float32")
         elif beta_schedule == "linear":
-            self.betas = paddle.linspace(beta_start,
-                                         beta_end,
-                                         num_train_timesteps,
-                                         dtype="float32")
+            self.betas = paddle.linspace(beta_start, beta_end, num_train_timesteps, dtype="float32")
         elif beta_schedule == "scaled_linear":
             # this schedule is very specific to the latent diffusion model.
-            self.betas = (paddle.linspace(beta_start**0.5,
-                                          beta_end**0.5,
-                                          num_train_timesteps,
-                                          dtype="float32")**2)
+            self.betas = paddle.linspace(beta_start**0.5, beta_end**0.5, num_train_timesteps, dtype="float32") ** 2
         else:
-            raise NotImplementedError(
-                f"{beta_schedule} does is not implemented for {self.__class__}")
+            raise NotImplementedError(f"{beta_schedule} does is not implemented for {self.__class__}")
 
         self.alphas = 1.0 - self.betas
         self.alphas_cumprod = paddle.cumprod(self.alphas, 0)
 
-        sigmas = np.array(
-            ((1 - self.alphas_cumprod) / self.alphas_cumprod)**0.5)
+        sigmas = np.array(((1 - self.alphas_cumprod) / self.alphas_cumprod) ** 0.5)
         sigmas = np.concatenate([sigmas[::-1], [0.0]]).astype(np.float32)
         self.sigmas = paddle.to_tensor(sigmas)
 
         # standard deviation of the initial noise distribution
         self.init_noise_sigma = self.sigmas.max()
 
         # setable values
         self.num_inference_steps = None
-        timesteps = np.linspace(0,
-                                num_train_timesteps - 1,
-                                num_train_timesteps,
-                                dtype=np.float32)[::-1].copy()
-        self.timesteps = paddle.to_tensor(timesteps)
+        timesteps = np.linspace(0, num_train_timesteps - 1, num_train_timesteps, dtype=float)[::-1].copy()
+        self.timesteps = paddle.to_tensor(timesteps, dtype="float32")
         self.derivatives = []
         self.is_scale_input_called = False
 
-    def scale_model_input(
-            self, sample: paddle.Tensor,
-            timestep: Union[float, paddle.Tensor]) -> paddle.Tensor:
+    def scale_model_input(self, sample: paddle.Tensor, timestep: Union[float, paddle.Tensor]) -> paddle.Tensor:
         """
         Scales the denoising model input by `(sigma**2 + 1) ** 0.5` to match the K-LMS algorithm.
 
         Args:
             sample (`paddle.Tensor`): input sample
             timestep (`float` or `paddle.Tensor`): the current timestep in the diffusion chain
 
         Returns:
             `paddle.Tensor`: scaled input sample
         """
         step_index = (self.timesteps == timestep).nonzero().item()
         sigma = self.sigmas[step_index]
-        sample = sample / ((sigma**2 + 1)**0.5)
+        sample = sample / ((sigma**2 + 1) ** 0.5)
         self.is_scale_input_called = True
         return sample
 
     def get_lms_coefficient(self, order, t, current_order):
         """
         Compute a linear multistep coefficient.
 
@@ -146,45 +138,37 @@
         """
 
         def lms_derivative(tau):
             prod = 1.0
             for k in range(order):
                 if current_order == k:
                     continue
-                prod *= (tau - self.sigmas[t - k]) / (
-                    self.sigmas[t - current_order] - self.sigmas[t - k])
+                prod *= (tau - self.sigmas[t - k]) / (self.sigmas[t - current_order] - self.sigmas[t - k])
             return prod
 
-        integrated_coeff = integrate.quad(lms_derivative,
-                                          self.sigmas[t],
-                                          self.sigmas[t + 1],
-                                          epsrel=1e-4)[0]
+        integrated_coeff = integrate.quad(lms_derivative, self.sigmas[t], self.sigmas[t + 1], epsrel=1e-4)[0]
 
         return integrated_coeff
 
     def set_timesteps(self, num_inference_steps: int):
         """
         Sets the timesteps used for the diffusion chain. Supporting function to be run before inference.
 
         Args:
             num_inference_steps (`int`):
                 the number of diffusion steps used when generating samples with a pre-trained model.
         """
         self.num_inference_steps = num_inference_steps
 
-        timesteps = np.linspace(0,
-                                self.config.num_train_timesteps - 1,
-                                num_inference_steps,
-                                dtype=float)[::-1].copy()
-        sigmas = np.array(
-            ((1 - self.alphas_cumprod) / self.alphas_cumprod)**0.5)
+        timesteps = np.linspace(0, self.config.num_train_timesteps - 1, num_inference_steps, dtype=float)[::-1].copy()
+        sigmas = np.array(((1 - self.alphas_cumprod) / self.alphas_cumprod) ** 0.5)
         sigmas = np.interp(timesteps, np.arange(0, len(sigmas)), sigmas)
         sigmas = np.concatenate([sigmas, [0.0]]).astype(np.float32)
         self.sigmas = paddle.to_tensor(sigmas)
-        self.timesteps = paddle.to_tensor(timesteps)
+        self.timesteps = paddle.to_tensor(timesteps, dtype="float32")
 
         self.derivatives = []
 
     def step(
         self,
         model_output: paddle.Tensor,
         timestep: Union[float, paddle.Tensor],
@@ -209,83 +193,64 @@
             [`~schedulers.scheduling_utils.LMSDiscreteSchedulerOutput`] if `return_dict` is True, otherwise a `tuple`.
             When returning a tuple, the first element is the sample tensor.
 
         """
         if not self.is_scale_input_called:
             warnings.warn(
                 "The `scale_model_input` function should be called before `step` to ensure correct denoising. "
-                "See `StableDiffusionPipeline` for a usage example.")
+                "See `StableDiffusionPipeline` for a usage example."
+            )
 
-        # if (isinstance(timestep, int) or isinstance(timestep, paddle.Tensor)):
-        #     deprecate(
-        #         "timestep as an index",
-        #         "0.8.0",
-        #         "Passing integer indices (e.g. from `enumerate(timesteps)`) as timesteps to"
-        #         " `LMSDiscreteScheduler.step()` will not be supported in future versions. Make sure to pass"
-        #         " one of the `scheduler.timesteps` as a timestep.",
-        #         standard_warn=False,
-        #     )
-        #     step_index = timestep
-        # else:
         step_index = (self.timesteps == timestep).nonzero().item()
         sigma = self.sigmas[step_index]
 
         # 1. compute predicted original sample (x_0) from sigma-scaled predicted noise
-        pred_original_sample = sample - sigma * model_output
+        if self.config.prediction_type == "epsilon":
+            pred_original_sample = sample - sigma * model_output
+        elif self.config.prediction_type == "v_prediction":
+            # * c_out + input * c_skip
+            pred_original_sample = model_output * (-sigma / (sigma**2 + 1) ** 0.5) + (sample / (sigma**2 + 1))
+        else:
+            raise ValueError(
+                f"prediction_type given as {self.config.prediction_type} must be one of `epsilon`, or `v_prediction`"
+            )
 
         # 2. Convert to an ODE derivative
         derivative = (sample - pred_original_sample) / sigma
         self.derivatives.append(derivative)
         if len(self.derivatives) > order:
             self.derivatives.pop(0)
 
         # 3. Compute linear multistep coefficients
         order = min(step_index + 1, order)
-        lms_coeffs = [
-            self.get_lms_coefficient(order, step_index, curr_order)
-            for curr_order in range(order)
-        ]
+        lms_coeffs = [self.get_lms_coefficient(order, step_index, curr_order) for curr_order in range(order)]
 
         # 4. Compute previous sample based on the derivatives path
-        prev_sample = sample + sum(coeff * derivative
-                                   for coeff, derivative in zip(
-                                       lms_coeffs, reversed(self.derivatives)))
+        prev_sample = sample + sum(
+            coeff * derivative for coeff, derivative in zip(lms_coeffs, reversed(self.derivatives))
+        )
 
         if not return_dict:
-            return (prev_sample, )
+            return (prev_sample,)
 
-        return LMSDiscreteSchedulerOutput(
-            prev_sample=prev_sample, pred_original_sample=pred_original_sample)
+        return LMSDiscreteSchedulerOutput(prev_sample=prev_sample, pred_original_sample=pred_original_sample)
 
     def add_noise(
         self,
         original_samples: paddle.Tensor,
         noise: paddle.Tensor,
         timesteps: paddle.Tensor,
     ) -> paddle.Tensor:
         # Make sure sigmas and timesteps have the same dtype as original_samples
-        self.sigmas = self.sigmas.astype(original_samples.dtype)
-
+        sigmas = self.sigmas.cast(original_samples.dtype)
         schedule_timesteps = self.timesteps
 
-        # if isinstance(timesteps, paddle.Tensor):
-        #     deprecate(
-        #         "timesteps as indices",
-        #         "0.8.0",
-        #         "Passing integer indices  (e.g. from `enumerate(timesteps)`) as timesteps to"
-        #         " `LMSDiscreteScheduler.add_noise()` will not be supported in future versions. Make sure to"
-        #         " pass values from `scheduler.timesteps` as timesteps.",
-        #         standard_warn=False,
-        #     )
-        #     step_indices = timesteps
-        # else:
-        step_indices = [(schedule_timesteps == t).nonzero().item()
-                        for t in timesteps]
+        step_indices = [(schedule_timesteps == t).nonzero().item() for t in timesteps]
 
-        sigma = self.sigmas[step_indices].flatten()
+        sigma = sigmas[step_indices].flatten()
         while len(sigma.shape) < len(original_samples.shape):
             sigma = sigma.unsqueeze(-1)
 
         noisy_samples = original_samples + noise * sigma
         return noisy_samples
 
     def __len__(self):
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/schedulers/scheduling_pndm.py` & `ppdiffusers-0.9.0/ppdiffusers/schedulers/scheduling_pndm.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # DISCLAIMER: This file is strongly influenced by https://github.com/ermongroup/ddim
 
 import math
-from typing import Optional, Tuple, Union
+from typing import List, Optional, Tuple, Union
 
 import numpy as np
 import paddle
 
 from ..configuration_utils import ConfigMixin, register_to_config
-from ..utils import deprecate
+from ..utils import _COMPATIBLE_STABLE_DIFFUSION_SCHEDULERS
 from .scheduling_utils import SchedulerMixin, SchedulerOutput
 
 
 def betas_for_alpha_bar(num_diffusion_timesteps, max_beta=0.999):
     """
     Create a beta schedule that discretizes the given alpha_t_bar function, which defines the cumulative product of
     (1-beta) over time from t = [0,1].
@@ -41,15 +41,15 @@
                      prevent singularities.
 
     Returns:
         betas (`np.ndarray`): the betas used by the scheduler to step the model outputs
     """
 
     def alpha_bar(time_step):
-        return math.cos((time_step + 0.008) / 1.008 * math.pi / 2)**2
+        return math.cos((time_step + 0.008) / 1.008 * math.pi / 2) ** 2
 
     betas = []
     for i in range(num_diffusion_timesteps):
         t1 = i / num_diffusion_timesteps
         t2 = (i + 1) / num_diffusion_timesteps
         betas.append(min(1 - alpha_bar(t2) / alpha_bar(t1), max_beta))
     return paddle.to_tensor(betas, dtype="float32")
@@ -58,16 +58,16 @@
 class PNDMScheduler(SchedulerMixin, ConfigMixin):
     """
     Pseudo numerical methods for diffusion models (PNDM) proposes using more advanced ODE integration techniques,
     namely Runge-Kutta method and a linear multi-step method.
 
     [`~ConfigMixin`] takes care of storing all config attributes that are passed in the scheduler's `__init__`
     function, such as `num_train_timesteps`. They can be accessed via `scheduler.config.num_train_timesteps`.
-    [`~ConfigMixin`] also provides general loading and saving functionality via the [`~ConfigMixin.save_config`] and
-    [`~ConfigMixin.from_config`] functions.
+    [`SchedulerMixin`] provides general loading and saving functionality via the [`SchedulerMixin.save_pretrained`] and
+    [`~SchedulerMixin.from_pretrained`] functions.
 
     For more details, see the original paper: https://arxiv.org/abs/2202.09778
 
     Args:
         num_train_timesteps (`int`): number of diffusion steps used to train the model.
         beta_start (`float`): the starting `beta` value of inference.
         beta_end (`float`): the final `beta` value.
@@ -79,58 +79,58 @@
         skip_prk_steps (`bool`):
             allows the scheduler to skip the Runge-Kutta steps that are defined in the original paper as being required
             before plms steps; defaults to `False`.
         set_alpha_to_one (`bool`, default `False`):
             each diffusion step uses the value of alphas product at that step and at the previous one. For the final
             step there is no previous alpha. When this option is `True` the previous alpha product is fixed to `1`,
             otherwise it uses the value of alpha at step 0.
+        prediction_type (`str`, default `epsilon`, optional):
+            prediction type of the scheduler function, one of `epsilon` (predicting the noise of the diffusion
+            process), `sample` (directly predicting the noisy sample`) or `v_prediction` (see section 2.4
+            https://imagen.research.google/video/paper.pdf)
         steps_offset (`int`, default `0`):
             an offset added to the inference steps. You can use a combination of `offset=1` and
             `set_alpha_to_one=False`, to make the last step use step 0 for the previous alpha product, as done in
             stable diffusion.
 
     """
 
+    _compatibles = _COMPATIBLE_STABLE_DIFFUSION_SCHEDULERS.copy()
+    order = 1
+
     @register_to_config
     def __init__(
         self,
         num_train_timesteps: int = 1000,
         beta_start: float = 0.0001,
         beta_end: float = 0.02,
         beta_schedule: str = "linear",
-        trained_betas: Optional[np.ndarray] = None,
+        trained_betas: Optional[Union[np.ndarray, List[float]]] = None,
         skip_prk_steps: bool = False,
         set_alpha_to_one: bool = False,
+        prediction_type: str = "epsilon",
         steps_offset: int = 0,
     ):
         if trained_betas is not None:
-            self.betas = paddle.to_tensor(trained_betas)
+            self.betas = paddle.to_tensor(trained_betas, dtype="float32")
         elif beta_schedule == "linear":
-            self.betas = paddle.linspace(beta_start,
-                                         beta_end,
-                                         num_train_timesteps,
-                                         dtype="float32")
+            self.betas = paddle.linspace(beta_start, beta_end, num_train_timesteps, dtype="float32")
         elif beta_schedule == "scaled_linear":
             # this schedule is very specific to the latent diffusion model.
-            self.betas = (paddle.linspace(beta_start**0.5,
-                                          beta_end**0.5,
-                                          num_train_timesteps,
-                                          dtype="float32")**2)
+            self.betas = paddle.linspace(beta_start**0.5, beta_end**0.5, num_train_timesteps, dtype="float32") ** 2
         elif beta_schedule == "squaredcos_cap_v2":
             # Glide cosine schedule
             self.betas = betas_for_alpha_bar(num_train_timesteps)
         else:
-            raise NotImplementedError(
-                f"{beta_schedule} does is not implemented for {self.__class__}")
+            raise NotImplementedError(f"{beta_schedule} does is not implemented for {self.__class__}")
 
         self.alphas = 1.0 - self.betas
         self.alphas_cumprod = paddle.cumprod(self.alphas, 0)
 
-        self.final_alpha_cumprod = paddle.to_tensor(
-            1.0) if set_alpha_to_one else self.alphas_cumprod[0]
+        self.final_alpha_cumprod = paddle.to_tensor(1.0) if set_alpha_to_one else self.alphas_cumprod[0]
 
         # standard deviation of the initial noise distribution
         self.init_noise_sigma = 1.0
 
         # For now we only support F-PNDM, i.e. the runge-kutta method
         # For more information on the algorithm please take a look at the paper: https://arxiv.org/pdf/2202.09778.pdf
         # mainly at formula (9), (12), (13) and the Algorithm 2.
@@ -140,60 +140,53 @@
         self.cur_model_output = 0
         self.counter = 0
         self.cur_sample = None
         self.ets = []
 
         # setable values
         self.num_inference_steps = None
-        self._timesteps = np.arange(
-            0, num_train_timesteps)[::-1].copy().astype("int64")
+        self._timesteps = np.arange(0, num_train_timesteps)[::-1].copy()
         self.prk_timesteps = None
         self.plms_timesteps = None
         self.timesteps = None
 
-    def set_timesteps(self, num_inference_steps: int) -> paddle.Tensor:
+    def set_timesteps(self, num_inference_steps: int):
         """
         Sets the discrete timesteps used for the diffusion chain. Supporting function to be run before inference.
 
         Args:
             num_inference_steps (`int`):
                 the number of diffusion steps used when generating samples with a pre-trained model.
         """
 
         self.num_inference_steps = num_inference_steps
         step_ratio = self.config.num_train_timesteps // self.num_inference_steps
         # creates integer timesteps by multiplying by ratio
         # casting to int to avoid issues when num_inference_step is power of 3
-        self._timesteps = (np.arange(0, num_inference_steps) *
-                           step_ratio).round()
+        self._timesteps = (np.arange(0, num_inference_steps) * step_ratio).round()
         self._timesteps += self.config.steps_offset
 
         if self.config.skip_prk_steps:
             # for some models like stable diffusion the prk steps can/should be skipped to
             # produce better results. When using PNDM with `self.config.skip_prk_steps` the implementation
             # is based on crowsonkb's PLMS sampler implementation: https://github.com/CompVis/latent-diffusion/pull/51
             self.prk_timesteps = np.array([])
-            self.plms_timesteps = np.concatenate([
-                self._timesteps[:-1], self._timesteps[-2:-1],
-                self._timesteps[-1:]
-            ])[::-1].copy()
+            self.plms_timesteps = np.concatenate([self._timesteps[:-1], self._timesteps[-2:-1], self._timesteps[-1:]])[
+                ::-1
+            ].copy()
         else:
-            prk_timesteps = np.array(
-                self._timesteps[-self.pndm_order:]).repeat(2) + np.tile(
-                    np.array([
-                        0, self.config.num_train_timesteps //
-                        num_inference_steps // 2
-                    ]), self.pndm_order)
-            self.prk_timesteps = (
-                prk_timesteps[:-1].repeat(2)[1:-1])[::-1].copy()
-            self.plms_timesteps = self._timesteps[:-3][::-1].copy(
-            )  # we copy to avoid having negative strides which are not supported by paddle
+            prk_timesteps = np.array(self._timesteps[-self.pndm_order :]).repeat(2) + np.tile(
+                np.array([0, self.config.num_train_timesteps // num_inference_steps // 2]), self.pndm_order
+            )
+            self.prk_timesteps = (prk_timesteps[:-1].repeat(2)[1:-1])[::-1].copy()
+            self.plms_timesteps = self._timesteps[:-3][
+                ::-1
+            ].copy()  # we copy to avoid having negative strides which are not supported by paddle
 
-        timesteps = np.concatenate([self.prk_timesteps,
-                                    self.plms_timesteps]).astype(np.int64)
+        timesteps = np.concatenate([self.prk_timesteps, self.plms_timesteps]).astype(np.int64)
         self.timesteps = paddle.to_tensor(timesteps)
 
         self.ets = []
         self.counter = 0
 
     def step(
         self,
@@ -217,25 +210,18 @@
 
         Returns:
             [`~schedulers.scheduling_utils.SchedulerOutput`] or `tuple`:
             [`~schedulers.scheduling_utils.SchedulerOutput`] if `return_dict` is True, otherwise a `tuple`. When
             returning a tuple, the first element is the sample tensor.
 
         """
-        if self.counter < len(
-                self.prk_timesteps) and not self.config.skip_prk_steps:
-            return self.step_prk(model_output=model_output,
-                                 timestep=timestep,
-                                 sample=sample,
-                                 return_dict=return_dict)
+        if self.counter < len(self.prk_timesteps) and not self.config.skip_prk_steps:
+            return self.step_prk(model_output=model_output, timestep=timestep, sample=sample, return_dict=return_dict)
         else:
-            return self.step_plms(model_output=model_output,
-                                  timestep=timestep,
-                                  sample=sample,
-                                  return_dict=return_dict)
+            return self.step_plms(model_output=model_output, timestep=timestep, sample=sample, return_dict=return_dict)
 
     def step_prk(
         self,
         model_output: paddle.Tensor,
         timestep: int,
         sample: paddle.Tensor,
         return_dict: bool = True,
@@ -276,20 +262,19 @@
         elif (self.counter - 3) % 4 == 0:
             model_output = self.cur_model_output + 1 / 6 * model_output
             self.cur_model_output = 0
 
         # cur_sample should not be `None`
         cur_sample = self.cur_sample if self.cur_sample is not None else sample
 
-        prev_sample = self._get_prev_sample(cur_sample, timestep, prev_timestep,
-                                            model_output)
+        prev_sample = self._get_prev_sample(cur_sample, timestep, prev_timestep, model_output)
         self.counter += 1
 
         if not return_dict:
-            return (prev_sample, )
+            return (prev_sample,)
 
         return SchedulerOutput(prev_sample=prev_sample)
 
     def step_plms(
         self,
         model_output: paddle.Tensor,
         timestep: int,
@@ -318,15 +303,16 @@
             )
 
         if not self.config.skip_prk_steps and len(self.ets) < 3:
             raise ValueError(
                 f"{self.__class__} can only be run AFTER scheduler has been run "
                 "in 'prk' mode for at least 12 iterations "
                 "See: https://github.com/huggingface/diffusers/blob/main/src/diffusers/pipelines/pipeline_pndm.py "
-                "for more information.")
+                "for more information."
+            )
 
         prev_timestep = timestep - self.config.num_train_timesteps // self.num_inference_steps
 
         if self.counter != 1:
             self.ets = self.ets[-3:]
             self.ets.append(model_output)
         else:
@@ -339,31 +325,27 @@
         elif len(self.ets) == 1 and self.counter == 1:
             model_output = (model_output + self.ets[-1]) / 2
             sample = self.cur_sample
             self.cur_sample = None
         elif len(self.ets) == 2:
             model_output = (3 * self.ets[-1] - self.ets[-2]) / 2
         elif len(self.ets) == 3:
-            model_output = (23 * self.ets[-1] - 16 * self.ets[-2] +
-                            5 * self.ets[-3]) / 12
+            model_output = (23 * self.ets[-1] - 16 * self.ets[-2] + 5 * self.ets[-3]) / 12
         else:
-            model_output = (1 / 24) * (55 * self.ets[-1] - 59 * self.ets[-2] +
-                                       37 * self.ets[-3] - 9 * self.ets[-4])
+            model_output = (1 / 24) * (55 * self.ets[-1] - 59 * self.ets[-2] + 37 * self.ets[-3] - 9 * self.ets[-4])
 
-        prev_sample = self._get_prev_sample(sample, timestep, prev_timestep,
-                                            model_output)
+        prev_sample = self._get_prev_sample(sample, timestep, prev_timestep, model_output)
         self.counter += 1
 
         if not return_dict:
-            return (prev_sample, )
+            return (prev_sample,)
 
         return SchedulerOutput(prev_sample=prev_sample)
 
-    def scale_model_input(self, sample: paddle.Tensor, *args,
-                          **kwargs) -> paddle.Tensor:
+    def scale_model_input(self, sample: paddle.Tensor, *args, **kwargs) -> paddle.Tensor:
         """
         Ensures interchangeability with schedulers that need to scale the denoising model input depending on the
         current timestep.
 
         Args:
             sample (`paddle.Tensor`): input sample
 
@@ -382,54 +364,60 @@
         # alpha_prod_t_prev -> α_(t−δ)
         # beta_prod_t -> (1 - α_t)
         # beta_prod_t_prev -> (1 - α_(t−δ))
         # sample -> x_t
         # model_output -> e_θ(x_t, t)
         # prev_sample -> x_(t−δ)
         alpha_prod_t = self.alphas_cumprod[timestep]
-        alpha_prod_t_prev = self.alphas_cumprod[
-            prev_timestep] if prev_timestep >= 0 else self.final_alpha_cumprod
+        alpha_prod_t_prev = self.alphas_cumprod[prev_timestep] if prev_timestep >= 0 else self.final_alpha_cumprod
         beta_prod_t = 1 - alpha_prod_t
         beta_prod_t_prev = 1 - alpha_prod_t_prev
 
+        if self.config.prediction_type == "v_prediction":
+            model_output = (alpha_prod_t**0.5) * model_output + (beta_prod_t**0.5) * sample
+        elif self.config.prediction_type != "epsilon":
+            raise ValueError(
+                f"prediction_type given as {self.config.prediction_type} must be one of `epsilon` or `v_prediction`"
+            )
+
         # corresponds to (α_(t−δ) - α_t) divided by
         # denominator of x_t in formula (9) and plus 1
         # Note: (α_(t−δ) - α_t) / (sqrt(α_t) * (sqrt(α_(t−δ)) + sqr(α_t))) =
         # sqrt(α_(t−δ)) / sqrt(α_t))
-        sample_coeff = (alpha_prod_t_prev / alpha_prod_t)**(0.5)
+        sample_coeff = (alpha_prod_t_prev / alpha_prod_t) ** (0.5)
 
         # corresponds to denominator of e_θ(x_t, t) in formula (9)
-        model_output_denom_coeff = alpha_prod_t * beta_prod_t_prev**(0.5) + (
-            alpha_prod_t * beta_prod_t * alpha_prod_t_prev)**(0.5)
+        model_output_denom_coeff = alpha_prod_t * beta_prod_t_prev ** (0.5) + (
+            alpha_prod_t * beta_prod_t * alpha_prod_t_prev
+        ) ** (0.5)
 
         # full formula (9)
-        prev_sample = (sample_coeff * sample -
-                       (alpha_prod_t_prev - alpha_prod_t) * model_output /
-                       model_output_denom_coeff)
+        prev_sample = (
+            sample_coeff * sample - (alpha_prod_t_prev - alpha_prod_t) * model_output / model_output_denom_coeff
+        )
 
         return prev_sample
 
     def add_noise(
         self,
         original_samples: paddle.Tensor,
         noise: paddle.Tensor,
         timesteps: paddle.Tensor,
     ) -> paddle.Tensor:
         # Make sure alphas_cumprod and timestep have same dtype as original_samples
-        self.alphas_cumprod = self.alphas_cumprod.astype(original_samples.dtype)
+        self.alphas_cumprod = self.alphas_cumprod.cast(original_samples.dtype)
 
-        sqrt_alpha_prod = self.alphas_cumprod[timesteps]**0.5
+        sqrt_alpha_prod = self.alphas_cumprod[timesteps] ** 0.5
         sqrt_alpha_prod = sqrt_alpha_prod.flatten()
         while len(sqrt_alpha_prod.shape) < len(original_samples.shape):
             sqrt_alpha_prod = sqrt_alpha_prod.unsqueeze(-1)
 
-        sqrt_one_minus_alpha_prod = (1 - self.alphas_cumprod[timesteps])**0.5
+        sqrt_one_minus_alpha_prod = (1 - self.alphas_cumprod[timesteps]) ** 0.5
         sqrt_one_minus_alpha_prod = sqrt_one_minus_alpha_prod.flatten()
-        while len(sqrt_one_minus_alpha_prod.shape) < len(
-                original_samples.shape):
+        while len(sqrt_one_minus_alpha_prod.shape) < len(original_samples.shape):
             sqrt_one_minus_alpha_prod = sqrt_one_minus_alpha_prod.unsqueeze(-1)
 
         noisy_samples = sqrt_alpha_prod * original_samples + sqrt_one_minus_alpha_prod * noise
         return noisy_samples
 
     def __len__(self):
         return self.config.num_train_timesteps
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/schedulers/scheduling_sde_ve.py` & `ppdiffusers-0.9.0/ppdiffusers/schedulers/scheduling_sde_ve.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,86 +47,81 @@
     """
     The variance exploding stochastic differential equation (SDE) scheduler.
 
     For more information, see the original paper: https://arxiv.org/abs/2011.13456
 
     [`~ConfigMixin`] takes care of storing all config attributes that are passed in the scheduler's `__init__`
     function, such as `num_train_timesteps`. They can be accessed via `scheduler.config.num_train_timesteps`.
-    [`~ConfigMixin`] also provides general loading and saving functionality via the [`~ConfigMixin.save_config`] and
-    [`~ConfigMixin.from_config`] functions.
+    [`SchedulerMixin`] provides general loading and saving functionality via the [`SchedulerMixin.save_pretrained`] and
+    [`~SchedulerMixin.from_pretrained`] functions.
 
     Args:
         num_train_timesteps (`int`): number of diffusion steps used to train the model.
         snr (`float`):
             coefficient weighting the step from the model_output sample (from the network) to the random noise.
         sigma_min (`float`):
                 initial noise scale for sigma sequence in sampling procedure. The minimum sigma should mirror the
                 distribution of the data.
         sigma_max (`float`): maximum value used for the range of continuous timesteps passed into the model.
         sampling_eps (`float`): the end value of sampling, where timesteps decrease progressively from 1 to
         epsilon.
         correct_steps (`int`): number of correction steps performed on a produced sample.
     """
 
+    order = 1
+
     @register_to_config
     def __init__(
         self,
         num_train_timesteps: int = 2000,
         snr: float = 0.15,
         sigma_min: float = 0.01,
         sigma_max: float = 1348.0,
         sampling_eps: float = 1e-5,
         correct_steps: int = 1,
     ):
-
         # standard deviation of the initial noise distribution
         self.init_noise_sigma = sigma_max
 
         # setable values
         self.timesteps = None
 
         self.set_sigmas(num_train_timesteps, sigma_min, sigma_max, sampling_eps)
 
-    def scale_model_input(self,
-                          sample: paddle.Tensor,
-                          timestep: Optional[int] = None) -> paddle.Tensor:
+    def scale_model_input(self, sample: paddle.Tensor, timestep: Optional[int] = None) -> paddle.Tensor:
         """
         Ensures interchangeability with schedulers that need to scale the denoising model input depending on the
         current timestep.
 
         Args:
             sample (`paddle.Tensor`): input sample
             timestep (`int`, optional): current timestep
 
         Returns:
             `paddle.Tensor`: scaled input sample
         """
         return sample
 
-    def set_timesteps(self,
-                      num_inference_steps: int,
-                      sampling_eps: float = None):
+    def set_timesteps(self, num_inference_steps: int, sampling_eps: float = None):
         """
         Sets the continuous timesteps used for the diffusion chain. Supporting function to be run before inference.
 
         Args:
             num_inference_steps (`int`):
                 the number of diffusion steps used when generating samples with a pre-trained model.
             sampling_eps (`float`, optional): final timestep value (overrides value given at Scheduler instantiation).
 
         """
         sampling_eps = sampling_eps if sampling_eps is not None else self.config.sampling_eps
 
         self.timesteps = paddle.linspace(1, sampling_eps, num_inference_steps)
 
-    def set_sigmas(self,
-                   num_inference_steps: int,
-                   sigma_min: float = None,
-                   sigma_max: float = None,
-                   sampling_eps: float = None):
+    def set_sigmas(
+        self, num_inference_steps: int, sigma_min: float = None, sigma_max: float = None, sampling_eps: float = None
+    ):
         """
         Sets the noise scales used for the diffusion chain. Supporting function to be run before inference.
 
         The sigmas control the weight of the `drift` and `diffusion` components of sample update.
 
         Args:
             num_inference_steps (`int`):
@@ -139,131 +134,129 @@
         """
         sigma_min = sigma_min if sigma_min is not None else self.config.sigma_min
         sigma_max = sigma_max if sigma_max is not None else self.config.sigma_max
         sampling_eps = sampling_eps if sampling_eps is not None else self.config.sampling_eps
         if self.timesteps is None:
             self.set_timesteps(num_inference_steps, sampling_eps)
 
-        self.sigmas = sigma_min * (sigma_max / sigma_min)**(self.timesteps /
-                                                            sampling_eps)
+        self.sigmas = sigma_min * (sigma_max / sigma_min) ** (self.timesteps / sampling_eps)
         self.discrete_sigmas = paddle.exp(
-            paddle.linspace(math.log(sigma_min), math.log(sigma_max),
-                            num_inference_steps))
-        self.sigmas = paddle.to_tensor(
-            [sigma_min * (sigma_max / sigma_min)**t for t in self.timesteps])
+            paddle.linspace(math.log(sigma_min), math.log(sigma_max), num_inference_steps)
+        )
+        self.sigmas = paddle.to_tensor([sigma_min * (sigma_max / sigma_min) ** t for t in self.timesteps])
 
     def get_adjacent_sigma(self, timesteps, t):
         return paddle.where(
             timesteps == 0,
             paddle.zeros_like(t),
             self.discrete_sigmas[timesteps - 1],
         )
 
     def step_pred(
         self,
         model_output: paddle.Tensor,
         timestep: int,
         sample: paddle.Tensor,
+        generator: Optional[paddle.Generator] = None,
         return_dict: bool = True,
     ) -> Union[SdeVeOutput, Tuple]:
         """
         Predict the sample at the previous timestep by reversing the SDE. Core function to propagate the diffusion
         process from the learned model outputs (most often the predicted noise).
 
         Args:
             model_output (`paddle.Tensor`): direct output from learned diffusion model.
             timestep (`int`): current discrete timestep in the diffusion chain.
             sample (`paddle.Tensor`):
                 current instance of sample being created by diffusion process.
+            generator: random number generator.
             return_dict (`bool`): option for returning tuple rather than SchedulerOutput class
 
         Returns:
             [`~schedulers.scheduling_sde_ve.SdeVeOutput`] or `tuple`: [`~schedulers.scheduling_sde_ve.SdeVeOutput`] if
             `return_dict` is True, otherwise a `tuple`. When returning a tuple, the first element is the sample tensor.
 
         """
         if self.timesteps is None:
             raise ValueError(
                 "`self.timesteps` is not set, you need to run 'set_timesteps' after creating the scheduler"
             )
 
-        timestep = timestep * paddle.ones((sample.shape[0], ))
-        timesteps = (timestep * (len(self.timesteps) - 1)).astype("int64")
+        timestep = timestep * paddle.ones((sample.shape[0],))  # paddle.repeat_interleave(timestep, sample.shape[0])
+        timesteps = (timestep * (len(self.timesteps) - 1)).cast("int64")
 
         sigma = self.discrete_sigmas[timesteps]
         adjacent_sigma = self.get_adjacent_sigma(timesteps, timestep)
         drift = paddle.zeros_like(sample)
-        diffusion = (sigma**2 - adjacent_sigma**2)**0.5
+        diffusion = (sigma**2 - adjacent_sigma**2) ** 0.5
 
         # equation 6 in the paper: the model_output modeled by the network is grad_x log pt(x)
         # also equation 47 shows the analog from SDE models to ancestral sampling methods
         diffusion = diffusion.flatten()
         while len(diffusion.shape) < len(sample.shape):
             diffusion = diffusion.unsqueeze(-1)
         drift = drift - diffusion**2 * model_output
 
         #  equation 6: sample noise for the diffusion term of
-        noise = paddle.randn(sample.shape)
+        noise = paddle.randn(sample.shape, generator=generator)
         prev_sample_mean = sample - drift  # subtract because `dt` is a small negative timestep
         # TODO is the variable diffusion the correct scaling term for the noise?
         prev_sample = prev_sample_mean + diffusion * noise  # add impact of diffusion field g
 
         if not return_dict:
             return (prev_sample, prev_sample_mean)
 
-        return SdeVeOutput(prev_sample=prev_sample,
-                           prev_sample_mean=prev_sample_mean)
+        return SdeVeOutput(prev_sample=prev_sample, prev_sample_mean=prev_sample_mean)
 
     def step_correct(
         self,
         model_output: paddle.Tensor,
         sample: paddle.Tensor,
+        generator: Optional[paddle.Generator] = None,
         return_dict: bool = True,
     ) -> Union[SchedulerOutput, Tuple]:
         """
         Correct the predicted sample based on the output model_output of the network. This is often run repeatedly
         after making the prediction for the previous timestep.
 
         Args:
             model_output (`paddle.Tensor`): direct output from learned diffusion model.
             sample (`paddle.Tensor`):
                 current instance of sample being created by diffusion process.
+            generator: random number generator.
             return_dict (`bool`): option for returning tuple rather than SchedulerOutput class
 
         Returns:
             [`~schedulers.scheduling_sde_ve.SdeVeOutput`] or `tuple`: [`~schedulers.scheduling_sde_ve.SdeVeOutput`] if
             `return_dict` is True, otherwise a `tuple`. When returning a tuple, the first element is the sample tensor.
 
         """
         if self.timesteps is None:
             raise ValueError(
                 "`self.timesteps` is not set, you need to run 'set_timesteps' after creating the scheduler"
             )
 
         # For small batch sizes, the paper "suggest replacing norm(z) with sqrt(d), where d is the dim. of z"
         # sample noise for correction
-        noise = paddle.randn(sample.shape)
+        noise = paddle.randn(sample.shape, generator=generator)
 
         # compute step size from the model_output, the noise, and the snr
-        grad_norm = paddle.norm(model_output.reshape(
-            [model_output.shape[0], -1]),
-                                axis=-1).mean()
-        noise_norm = paddle.norm(noise.reshape([noise.shape[0], -1]),
-                                 axis=-1).mean()
-        step_size = (self.config.snr * noise_norm / grad_norm)**2 * 2
-        step_size = step_size * paddle.ones((sample.shape[0], ))
+        grad_norm = paddle.norm(model_output.reshape([model_output.shape[0], -1]), axis=-1).mean()
+        noise_norm = paddle.norm(noise.reshape([noise.shape[0], -1]), axis=-1).mean()
+        step_size = (self.config.snr * noise_norm / grad_norm) ** 2 * 2
+        step_size = step_size * paddle.ones((sample.shape[0],))
         # self.repeat_scalar(step_size, sample.shape[0])
 
         # compute corrected sample: model_output term and noise term
         step_size = step_size.flatten()
         while len(step_size.shape) < len(sample.shape):
             step_size = step_size.unsqueeze(-1)
         prev_sample_mean = sample + step_size * model_output
-        prev_sample = prev_sample_mean + ((step_size * 2)**0.5) * noise
+        prev_sample = prev_sample_mean + ((step_size * 2) ** 0.5) * noise
 
         if not return_dict:
-            return (prev_sample, )
+            return (prev_sample,)
 
         return SchedulerOutput(prev_sample=prev_sample)
 
     def __len__(self):
         return self.config.num_train_timesteps
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/schedulers/scheduling_sde_vp.py` & `ppdiffusers-0.9.0/ppdiffusers/schedulers/scheduling_sde_vp.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,71 +25,65 @@
 
 class ScoreSdeVpScheduler(SchedulerMixin, ConfigMixin):
     """
     The variance preserving stochastic differential equation (SDE) scheduler.
 
     [`~ConfigMixin`] takes care of storing all config attributes that are passed in the scheduler's `__init__`
     function, such as `num_train_timesteps`. They can be accessed via `scheduler.config.num_train_timesteps`.
-    [`~ConfigMixin`] also provides general loading and saving functionality via the [`~ConfigMixin.save_config`] and
-    [`~ConfigMixin.from_config`] functions.
+    [`SchedulerMixin`] provides general loading and saving functionality via the [`SchedulerMixin.save_pretrained`] and
+    [`~SchedulerMixin.from_pretrained`] functions.
 
     For more information, see the original paper: https://arxiv.org/abs/2011.13456
 
     UNDER CONSTRUCTION
 
     """
 
+    order = 1
+
     @register_to_config
-    def __init__(
-        self,
-        num_train_timesteps=2000,
-        beta_min=0.1,
-        beta_max=20,
-        sampling_eps=1e-3,
-    ):
+    def __init__(self, num_train_timesteps=2000, beta_min=0.1, beta_max=20, sampling_eps=1e-3):
         self.sigmas = None
         self.discrete_sigmas = None
         self.timesteps = None
 
     def set_timesteps(self, num_inference_steps):
-        self.timesteps = paddle.linspace(1, self.config.sampling_eps,
-                                         num_inference_steps)
+        self.timesteps = paddle.linspace(1, self.config.sampling_eps, num_inference_steps)
 
-    def step_pred(self, score, x, t):
+    def step_pred(self, score, x, t, generator=None):
         if self.timesteps is None:
             raise ValueError(
                 "`self.timesteps` is not set, you need to run 'set_timesteps' after creating the scheduler"
             )
 
         # TODO(Patrick) better comments + non-Paddle
         # postprocess model score
-        log_mean_coeff = (-0.25 * t**2 *
-                          (self.config.beta_max - self.config.beta_min) -
-                          0.5 * t * self.config.beta_min)
+        log_mean_coeff = (
+            -0.25 * t**2 * (self.config.beta_max - self.config.beta_min) - 0.5 * t * self.config.beta_min
+        )
         std = paddle.sqrt(1.0 - paddle.exp(2.0 * log_mean_coeff))
         std = std.flatten()
         while len(std.shape) < len(score.shape):
             std = std.unsqueeze(-1)
         score = -score / std
 
         # compute
         dt = -1.0 / len(self.timesteps)
 
-        beta_t = self.config.beta_min + t * (self.config.beta_max -
-                                             self.config.beta_min)
+        beta_t = self.config.beta_min + t * (self.config.beta_max - self.config.beta_min)
         beta_t = beta_t.flatten()
         while len(beta_t.shape) < len(x.shape):
             beta_t = beta_t.unsqueeze(-1)
         drift = -0.5 * beta_t * x
 
         diffusion = paddle.sqrt(beta_t)
         drift = drift - diffusion**2 * score
         x_mean = x + drift * dt
 
         # add noise
-        noise = paddle.randn(x.shape)
+        noise = paddle.randn(x.shape, generator=generator)
         x = x_mean + diffusion * math.sqrt(-dt) * noise
 
         return x, x_mean
 
     def __len__(self):
         return self.config.num_train_timesteps
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/schedulers/scheduling_utils.py` & `ppdiffusers-0.9.0/tests/test_pipelines_common.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,26 @@
 # Copyright (c) 2022 PaddlePaddle Authors. All Rights Reserved.
-# Copyright 2022 The HuggingFace Team. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from dataclasses import dataclass
 
-import paddle
+from ppdiffusers.utils.testing_utils import require_paddle
 
-from ..utils import BaseOutput
 
-SCHEDULER_CONFIG_NAME = "scheduler_config.json"
-
-
-@dataclass
-class SchedulerOutput(BaseOutput):
-    """
-    Base class for the scheduler's step function output.
-
-    Args:
-        prev_sample (`paddle.Tensor` of shape `(batch_size, num_channels, height, width)` for images):
-            Computed sample (x_{t-1}) of previous timestep. `prev_sample` should be used as next model input in the
-            denoising loop.
-    """
-
-    prev_sample: paddle.Tensor
-
-
-class SchedulerMixin:
+@require_paddle
+class PipelineTesterMixin:
     """
-    Mixin containing common functions for the schedulers.
+    This mixin is designed to be used with unittest.TestCase classes.
+    It provides a set of common tests for each Paddle pipeline, e.g. saving and loading the pipeline,
+    equivalence of dict and tuple outputs, etc.
     """
 
-    config_name = SCHEDULER_CONFIG_NAME
+    pass
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/training_utils.py` & `ppdiffusers-0.9.0/ppdiffusers/training_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Copyright (c) 2022 PaddlePaddle Authors. All Rights Reserved.
-# Copyright 2022 The HuggingFace Inc. team.
+# Copyright 2022 The HuggingFace Team. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -41,48 +41,43 @@
     os.environ["FLAGS_cudnn_deterministic"] = "True"
     os.environ["FLAGS_benchmark"] = "True"
 
 
 def set_seed(seed: int = None):
     """
     Args:
-    Helper function for reproducible behavior to set the seed in `random`, `numpy`, `torch`.
+    Helper function for reproducible behavior to set the seed in `random`, `numpy`, `paddle`.
         seed (`int`): The seed to set.
     """
     if seed is not None:
         random.seed(seed)
         np.random.seed(seed)
         paddle.seed(seed)
 
 
 class EMAModel:
     """
     Exponential Moving Average of models weights
     """
 
-    def __init__(self,
-                 model,
-                 update_after_step=0,
-                 inv_gamma=1.0,
-                 power=2 / 3,
-                 min_value=0.0,
-                 max_value=0.9999):
+    def __init__(self, model, update_after_step=0, inv_gamma=1.0, power=2 / 3, min_value=0.0, max_value=0.9999):
         """
         @crowsonkb's notes on EMA Warmup:
             If gamma=1 and power=1, implements a simple average. gamma=1, power=2/3 are good values for models you plan
             to train for a million or more steps (reaches decay factor 0.999 at 31.6K steps, 0.9999 at 1M steps),
             gamma=1, power=3/4 for models you plan to train for less (reaches decay factor 0.999 at 10K steps, 0.9999
             at 215.4k steps).
         Args:
             inv_gamma (float): Inverse multiplicative factor of EMA warmup. Default: 1.
             power (float): Exponential factor of EMA warmup. Default: 2/3.
             min_value (float): The minimum EMA decay rate. Default: 0.
         """
 
-        self.averaged_model = copy.deepcopy(model).eval()
+        self.averaged_model = copy.deepcopy(model)
+        self.averaged_model.eval()
         for params in self.averaged_model.parameters():
             params.stop_gradient = True
 
         self.update_after_step = update_after_step
         self.inv_gamma = inv_gamma
         self.power = power
         self.min_value = min_value
@@ -92,15 +87,15 @@
         self.optimization_step = 0
 
     def get_decay(self, optimization_step):
         """
         Compute the decay factor for the exponential moving average.
         """
         step = max(0, optimization_step - self.update_after_step - 1)
-        value = 1 - (1 + step / self.inv_gamma)**-self.power
+        value = 1 - (1 + step / self.inv_gamma) ** -self.power
 
         if step <= 0:
             return 0.0
 
         return max(self.min_value, min(value, self.max_value))
 
     @paddle.no_grad()
@@ -112,24 +107,23 @@
 
         for key, param in new_model.named_parameters():
             if isinstance(param, dict):
                 continue
             try:
                 ema_param = ema_params[key]
             except KeyError:
-                ema_param = param.astype("float32").clone(
-                ) if param.ndim == 1 else copy.deepcopy(param)
+                ema_param = param.cast("float32").clone() if param.ndim == 1 else copy.deepcopy(param)
                 ema_params[key] = ema_param
 
-            if not param.stop_gradient:
-                ema_params[key].copy_(param.astype(ema_param.dtype), True)
+            if param.stop_gradient:
+                ema_params[key].copy_(param.cast(ema_param.dtype), True)
                 ema_param = ema_params[key]
             else:
-                ema_param = ema_param.multiply(self.decay)
-                ema_param.add_(param.astype(ema_param.dtype) * (1 - self.decay))
+                ema_param.scale_(self.decay)
+                ema_param.add_(param.cast(ema_param.dtype) * (1 - self.decay))
 
             ema_state_dict[key] = ema_param
 
         for key, param in new_model.named_buffers():
             ema_state_dict[key] = param
 
         self.averaged_model.load_dict(ema_state_dict)
@@ -142,21 +136,17 @@
         rank = paddle.distributed.get_rank()
         is_main_process = rank == 0
         main_process_desc = "main local process"
 
         try:
             if not is_main_process:
                 # tell all replicas to wait
-                logger.debug(
-                    f"{rank}: waiting for the {main_process_desc} to perform {desc}"
-                )
+                logger.debug(f"{rank}: waiting for the {main_process_desc} to perform {desc}")
                 paddle.distributed.barrier()
             yield
         finally:
             if is_main_process:
                 # the wait is over
-                logger.debug(
-                    f"{rank}: {main_process_desc} completed {desc}, releasing all replicas"
-                )
+                logger.debug(f"{rank}: {main_process_desc} completed {desc}, releasing all replicas")
                 paddle.distributed.barrier()
     else:
         yield
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/utils/__init__.py` & `ppdiffusers-0.9.0/ppdiffusers/utils/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,47 +8,71 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+# flake8: noqa
 
 import os
+
 from .deprecation_utils import deprecate
 from .import_utils import (
     ENV_VARS_TRUE_AND_AUTO_VALUES,
     ENV_VARS_TRUE_VALUES,
     USE_PADDLE,
     DummyObject,
+    is_fastdeploy_available,
     is_inflect_available,
     is_modelcards_available,
     is_onnx_available,
-    is_scipy_available,
     is_paddle_available,
+    is_paddle_version,
     is_paddlenlp_available,
+    is_scipy_available,
     is_unidecode_available,
-    is_fastdeploy_available,
     requires_backends,
 )
 from .logging import get_logger
 from .outputs import BaseOutput
+from .pil_utils import PIL_INTERPOLATION
 
 if is_paddle_available():
-    from .testing_utils import floats_tensor, load_image, parse_flag_from_env, slow
+    from .testing_utils import (
+        floats_tensor,
+        image_grid,
+        load_hf_numpy,
+        load_image,
+        load_numpy,
+        load_ppnlp_numpy,
+        paddle_all_close,
+        parse_flag_from_env,
+        slow,
+    )
 
 logger = get_logger(__name__)
 
-from paddlenlp.utils.env import _get_sub_home, _get_ppnlp_home
+from paddlenlp.utils.env import _get_ppnlp_home, _get_sub_home
 
 ppnlp_cache_home = _get_ppnlp_home()
-default_cache_path = _get_sub_home('models')
+default_cache_path = _get_sub_home("models")
 
 CONFIG_NAME = "config.json"
 WEIGHTS_NAME = "model_state.pdparams"
-ONNX_WEIGHTS_NAME = "model.onnx"
 FASTDEPLOY_WEIGHTS_NAME = "inference.pdiparams"
 FASTDEPLOY_MODEL_NAME = "inference.pdmodel"
 DOWNLOAD_SERVER = "https://bj.bcebos.com/paddlenlp/models/community"
 PPDIFFUSERS_CACHE = default_cache_path
 PPDIFFUSERS_DYNAMIC_MODULE_NAME = "ppdiffusers_modules"
 PPNLP_MODULES_CACHE = os.getenv("PPNLP_MODULES_CACHE", _get_sub_home("modules"))
+
+_COMPATIBLE_STABLE_DIFFUSION_SCHEDULERS = [
+    "DDIMScheduler",
+    "DDPMScheduler",
+    "PNDMScheduler",
+    "LMSDiscreteScheduler",
+    "EulerDiscreteScheduler",
+    "HeunDiscreteScheduler",
+    "EulerAncestralDiscreteScheduler",
+    "DPMSolverMultistepScheduler",
+]
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/utils/deprecation_utils.py` & `ppdiffusers-0.9.0/ppdiffusers/utils/deprecation_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,54 +16,49 @@
 import inspect
 import warnings
 from typing import Any, Dict, Optional, Union
 
 from packaging import version
 
 
-def deprecate(*args,
-              take_from: Optional[Union[Dict, Any]] = None,
-              standard_warn=True):
+def deprecate(*args, take_from: Optional[Union[Dict, Any]] = None, standard_warn=True):
     from .. import __version__
 
     deprecated_kwargs = take_from
     values = ()
     if not isinstance(args[0], tuple):
-        args = (args, )
+        args = (args,)
 
     for attribute, version_name, message in args:
-        if version.parse(version.parse(
-                __version__).base_version) >= version.parse(version_name):
+        if version.parse(version.parse(__version__).base_version) >= version.parse(version_name):
             raise ValueError(
-                f"The deprecation tuple {(attribute, version_name, message)} should be removed since diffusers'"
-                f" version {__version__} is >= {version_name}")
+                f"The deprecation tuple {(attribute, version_name, message)} should be removed since ppdiffusers'"
+                f" version {__version__} is >= {version_name}"
+            )
 
         warning = None
-        if isinstance(deprecated_kwargs,
-                      dict) and attribute in deprecated_kwargs:
-            values += (deprecated_kwargs.pop(attribute), )
+        if isinstance(deprecated_kwargs, dict) and attribute in deprecated_kwargs:
+            values += (deprecated_kwargs.pop(attribute),)
             warning = f"The `{attribute}` argument is deprecated and will be removed in version {version_name}."
         elif hasattr(deprecated_kwargs, attribute):
-            values += (getattr(deprecated_kwargs, attribute), )
+            values += (getattr(deprecated_kwargs, attribute),)
             warning = f"The `{attribute}` attribute is deprecated and will be removed in version {version_name}."
         elif deprecated_kwargs is None:
             warning = f"`{attribute}` is deprecated and will be removed in version {version_name}."
 
         if warning is not None:
             warning = warning + " " if standard_warn else ""
-            warnings.warn(warning + message, DeprecationWarning)
+            warnings.warn(warning + message, FutureWarning, stacklevel=2)
 
     if isinstance(deprecated_kwargs, dict) and len(deprecated_kwargs) > 0:
         call_frame = inspect.getouterframes(inspect.currentframe())[1]
         filename = call_frame.filename
         line_number = call_frame.lineno
         function = call_frame.function
         key, value = next(iter(deprecated_kwargs.items()))
-        raise TypeError(
-            f"{function} in {filename} line {line_number-1} got an unexpected keyword argument `{key}`"
-        )
+        raise TypeError(f"{function} in {filename} line {line_number-1} got an unexpected keyword argument `{key}`")
 
     if len(values) == 0:
         return
     elif len(values) == 1:
         return values[0]
     return values
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/utils/dummy_paddle_and_paddlenlp_and_fastdeploy_objects.py` & `ppdiffusers-0.9.0/ppdiffusers/utils/dummy_paddle_and_paddlenlp_and_fastdeploy_objects.py`

 * *Files 24% similar despite different names*

```diff
@@ -30,30 +30,60 @@
         requires_backends(cls, ["paddle", "paddlenlp", "fastdeploy"])
 
     @classmethod
     def from_pretrained(cls, *args, **kwargs):
         requires_backends(cls, ["paddle", "paddlenlp", "fastdeploy"])
 
 
-class FastdeployStableDiffusionInpaintPipeline(metaclass=DummyObject):
+class FastDeployStableDiffusionInpaintPipeline(metaclass=DummyObject):
     _backends = ["paddle", "paddlenlp", "fastdeploy"]
 
     def __init__(self, *args, **kwargs):
         requires_backends(self, ["paddle", "paddlenlp", "fastdeploy"])
 
     @classmethod
     def from_config(cls, *args, **kwargs):
         requires_backends(cls, ["paddle", "paddlenlp", "fastdeploy"])
 
     @classmethod
     def from_pretrained(cls, *args, **kwargs):
         requires_backends(cls, ["paddle", "paddlenlp", "fastdeploy"])
 
 
-class FastdeployStableDiffusionPipeline(metaclass=DummyObject):
+class FastDeployStableDiffusionInpaintPipelineLegacy(metaclass=DummyObject):
+    _backends = ["paddle", "paddlenlp", "fastdeploy"]
+
+    def __init__(self, *args, **kwargs):
+        requires_backends(self, ["paddle", "paddlenlp", "fastdeploy"])
+
+    @classmethod
+    def from_config(cls, *args, **kwargs):
+        requires_backends(cls, ["paddle", "paddlenlp", "fastdeploy"])
+
+    @classmethod
+    def from_pretrained(cls, *args, **kwargs):
+        requires_backends(cls, ["paddle", "paddlenlp", "fastdeploy"])
+
+
+class FastDeployStableDiffusionMegaPipeline(metaclass=DummyObject):
+    _backends = ["paddle", "paddlenlp", "fastdeploy"]
+
+    def __init__(self, *args, **kwargs):
+        requires_backends(self, ["paddle", "paddlenlp", "fastdeploy"])
+
+    @classmethod
+    def from_config(cls, *args, **kwargs):
+        requires_backends(cls, ["paddle", "paddlenlp", "fastdeploy"])
+
+    @classmethod
+    def from_pretrained(cls, *args, **kwargs):
+        requires_backends(cls, ["paddle", "paddlenlp", "fastdeploy"])
+
+
+class FastDeployStableDiffusionPipeline(metaclass=DummyObject):
     _backends = ["paddle", "paddlenlp", "fastdeploy"]
 
     def __init__(self, *args, **kwargs):
         requires_backends(self, ["paddle", "paddlenlp", "fastdeploy"])
 
     @classmethod
     def from_config(cls, *args, **kwargs):
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/utils/dummy_paddle_and_scipy_objects.py` & `ppdiffusers-0.9.0/ppdiffusers/utils/dummy_paddle_and_scipy_objects.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -27,8 +27,8 @@
 
     @classmethod
     def from_config(cls, *args, **kwargs):
         requires_backends(cls, ["paddle", "scipy"])
 
     @classmethod
     def from_pretrained(cls, *args, **kwargs):
-        requires_backends(cls, ["paddle", "scipy"])
+        requires_backends(cls, ["paddle", "scipy"])
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/utils/dummy_paddle_objects.py` & `ppdiffusers-0.9.0/ppdiffusers/utils/dummy_paddle_objects.py`

 * *Files 14% similar despite different names*

```diff
@@ -45,14 +45,44 @@
         requires_backends(cls, ["paddle"])
 
     @classmethod
     def from_pretrained(cls, *args, **kwargs):
         requires_backends(cls, ["paddle"])
 
 
+class Transformer2DModel(metaclass=DummyObject):
+    _backends = ["paddle"]
+
+    def __init__(self, *args, **kwargs):
+        requires_backends(self, ["paddle"])
+
+    @classmethod
+    def from_config(cls, *args, **kwargs):
+        requires_backends(cls, ["paddle"])
+
+    @classmethod
+    def from_pretrained(cls, *args, **kwargs):
+        requires_backends(cls, ["paddle"])
+
+
+class UNet1DModel(metaclass=DummyObject):
+    _backends = ["paddle"]
+
+    def __init__(self, *args, **kwargs):
+        requires_backends(self, ["paddle"])
+
+    @classmethod
+    def from_config(cls, *args, **kwargs):
+        requires_backends(cls, ["paddle"])
+
+    @classmethod
+    def from_pretrained(cls, *args, **kwargs):
+        requires_backends(cls, ["paddle"])
+
+
 class UNet2DConditionModel(metaclass=DummyObject):
     _backends = ["paddle"]
 
     def __init__(self, *args, **kwargs):
         requires_backends(self, ["paddle"])
 
     @classmethod
@@ -103,16 +133,15 @@
 
 
 def get_cosine_schedule_with_warmup(*args, **kwargs):
     requires_backends(get_cosine_schedule_with_warmup, ["paddle"])
 
 
 def get_cosine_with_hard_restarts_schedule_with_warmup(*args, **kwargs):
-    requires_backends(get_cosine_with_hard_restarts_schedule_with_warmup,
-                      ["paddle"])
+    requires_backends(get_cosine_with_hard_restarts_schedule_with_warmup, ["paddle"])
 
 
 def get_linear_schedule_with_warmup(*args, **kwargs):
     requires_backends(get_linear_schedule_with_warmup, ["paddle"])
 
 
 def get_polynomial_decay_schedule_with_warmup(*args, **kwargs):
@@ -134,14 +163,29 @@
         requires_backends(cls, ["paddle"])
 
     @classmethod
     def from_pretrained(cls, *args, **kwargs):
         requires_backends(cls, ["paddle"])
 
 
+class DanceDiffusionPipeline(metaclass=DummyObject):
+    _backends = ["paddle"]
+
+    def __init__(self, *args, **kwargs):
+        requires_backends(self, ["paddle"])
+
+    @classmethod
+    def from_config(cls, *args, **kwargs):
+        requires_backends(cls, ["paddle"])
+
+    @classmethod
+    def from_pretrained(cls, *args, **kwargs):
+        requires_backends(cls, ["paddle"])
+
+
 class DDIMPipeline(metaclass=DummyObject):
     _backends = ["paddle"]
 
     def __init__(self, *args, **kwargs):
         requires_backends(self, ["paddle"])
 
     @classmethod
@@ -209,14 +253,44 @@
         requires_backends(cls, ["paddle"])
 
     @classmethod
     def from_pretrained(cls, *args, **kwargs):
         requires_backends(cls, ["paddle"])
 
 
+class KDPM2AncestralDiscreteScheduler(metaclass=DummyObject):
+    _backends = ["paddle"]
+
+    def __init__(self, *args, **kwargs):
+        requires_backends(self, ["paddle"])
+
+    @classmethod
+    def from_config(cls, *args, **kwargs):
+        requires_backends(cls, ["paddle"])
+
+    @classmethod
+    def from_pretrained(cls, *args, **kwargs):
+        requires_backends(cls, ["paddle"])
+
+
+class KDPM2DiscreteScheduler(metaclass=DummyObject):
+    _backends = ["paddle"]
+
+    def __init__(self, *args, **kwargs):
+        requires_backends(self, ["paddle"])
+
+    @classmethod
+    def from_config(cls, *args, **kwargs):
+        requires_backends(cls, ["paddle"])
+
+    @classmethod
+    def from_pretrained(cls, *args, **kwargs):
+        requires_backends(cls, ["paddle"])
+
+
 class PNDMPipeline(metaclass=DummyObject):
     _backends = ["paddle"]
 
     def __init__(self, *args, **kwargs):
         requires_backends(self, ["paddle"])
 
     @classmethod
@@ -224,14 +298,29 @@
         requires_backends(cls, ["paddle"])
 
     @classmethod
     def from_pretrained(cls, *args, **kwargs):
         requires_backends(cls, ["paddle"])
 
 
+class RePaintPipeline(metaclass=DummyObject):
+    _backends = ["paddle"]
+
+    def __init__(self, *args, **kwargs):
+        requires_backends(self, ["paddle"])
+
+    @classmethod
+    def from_config(cls, *args, **kwargs):
+        requires_backends(cls, ["paddle"])
+
+    @classmethod
+    def from_pretrained(cls, *args, **kwargs):
+        requires_backends(cls, ["paddle"])
+
+
 class ScoreSdeVePipeline(metaclass=DummyObject):
     _backends = ["paddle"]
 
     def __init__(self, *args, **kwargs):
         requires_backends(self, ["paddle"])
 
     @classmethod
@@ -239,30 +328,30 @@
         requires_backends(cls, ["paddle"])
 
     @classmethod
     def from_pretrained(cls, *args, **kwargs):
         requires_backends(cls, ["paddle"])
 
 
-class DDIMScheduler(metaclass=DummyObject):
+class ScoreSdeVpPipeline(metaclass=DummyObject):
     _backends = ["paddle"]
 
     def __init__(self, *args, **kwargs):
         requires_backends(self, ["paddle"])
 
     @classmethod
     def from_config(cls, *args, **kwargs):
         requires_backends(cls, ["paddle"])
 
     @classmethod
     def from_pretrained(cls, *args, **kwargs):
         requires_backends(cls, ["paddle"])
 
 
-class EulerAncestralDiscreteScheduler(metaclass=DummyObject):
+class DDIMScheduler(metaclass=DummyObject):
     _backends = ["paddle"]
 
     def __init__(self, *args, **kwargs):
         requires_backends(self, ["paddle"])
 
     @classmethod
     def from_config(cls, *args, **kwargs):
@@ -299,14 +388,74 @@
         requires_backends(cls, ["paddle"])
 
     @classmethod
     def from_pretrained(cls, *args, **kwargs):
         requires_backends(cls, ["paddle"])
 
 
+class EulerAncestralDiscreteScheduler(metaclass=DummyObject):
+    _backends = ["paddle"]
+
+    def __init__(self, *args, **kwargs):
+        requires_backends(self, ["paddle"])
+
+    @classmethod
+    def from_config(cls, *args, **kwargs):
+        requires_backends(cls, ["paddle"])
+
+    @classmethod
+    def from_pretrained(cls, *args, **kwargs):
+        requires_backends(cls, ["paddle"])
+
+
+class EulerDiscreteScheduler(metaclass=DummyObject):
+    _backends = ["paddle"]
+
+    def __init__(self, *args, **kwargs):
+        requires_backends(self, ["paddle"])
+
+    @classmethod
+    def from_config(cls, *args, **kwargs):
+        requires_backends(cls, ["paddle"])
+
+    @classmethod
+    def from_pretrained(cls, *args, **kwargs):
+        requires_backends(cls, ["paddle"])
+
+
+class HeunDiscreteScheduler(metaclass=DummyObject):
+    _backends = ["paddle"]
+
+    def __init__(self, *args, **kwargs):
+        requires_backends(self, ["paddle"])
+
+    @classmethod
+    def from_config(cls, *args, **kwargs):
+        requires_backends(cls, ["paddle"])
+
+    @classmethod
+    def from_pretrained(cls, *args, **kwargs):
+        requires_backends(cls, ["paddle"])
+
+
+class IPNDMScheduler(metaclass=DummyObject):
+    _backends = ["paddle"]
+
+    def __init__(self, *args, **kwargs):
+        requires_backends(self, ["paddle"])
+
+    @classmethod
+    def from_config(cls, *args, **kwargs):
+        requires_backends(cls, ["paddle"])
+
+    @classmethod
+    def from_pretrained(cls, *args, **kwargs):
+        requires_backends(cls, ["paddle"])
+
+
 class KarrasVeScheduler(metaclass=DummyObject):
     _backends = ["paddle"]
 
     def __init__(self, *args, **kwargs):
         requires_backends(self, ["paddle"])
 
     @classmethod
@@ -329,14 +478,29 @@
         requires_backends(cls, ["paddle"])
 
     @classmethod
     def from_pretrained(cls, *args, **kwargs):
         requires_backends(cls, ["paddle"])
 
 
+class RePaintScheduler(metaclass=DummyObject):
+    _backends = ["paddle"]
+
+    def __init__(self, *args, **kwargs):
+        requires_backends(self, ["paddle"])
+
+    @classmethod
+    def from_config(cls, *args, **kwargs):
+        requires_backends(cls, ["paddle"])
+
+    @classmethod
+    def from_pretrained(cls, *args, **kwargs):
+        requires_backends(cls, ["paddle"])
+
+
 class SchedulerMixin(metaclass=DummyObject):
     _backends = ["paddle"]
 
     def __init__(self, *args, **kwargs):
         requires_backends(self, ["paddle"])
 
     @classmethod
@@ -352,14 +516,29 @@
     _backends = ["paddle"]
 
     def __init__(self, *args, **kwargs):
         requires_backends(self, ["paddle"])
 
     @classmethod
     def from_config(cls, *args, **kwargs):
+        requires_backends(cls, ["paddle"])
+
+    @classmethod
+    def from_pretrained(cls, *args, **kwargs):
+        requires_backends(cls, ["paddle"])
+
+
+class VQDiffusionScheduler(metaclass=DummyObject):
+    _backends = ["paddle"]
+
+    def __init__(self, *args, **kwargs):
+        requires_backends(self, ["paddle"])
+
+    @classmethod
+    def from_config(cls, *args, **kwargs):
         requires_backends(cls, ["paddle"])
 
     @classmethod
     def from_pretrained(cls, *args, **kwargs):
         requires_backends(cls, ["paddle"])
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/utils/import_utils.py` & `ppdiffusers-0.9.0/ppdiffusers/utils/import_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
 Import utilities: Utilities related to imports and our lazy inits.
 """
 import importlib.util
+import operator as op
 import os
 import sys
 from collections import OrderedDict
+from typing import Union
 
-from packaging import version
+from packaging.version import Version, parse
 
 from . import logging
 
 # The package importlib_metadata is in a different place, depending on the python version.
 if sys.version_info < (3, 8):
     import importlib_metadata
 else:
@@ -33,75 +35,80 @@
 logger = logging.get_logger(__name__)  # pylint: disable=invalid-name
 
 ENV_VARS_TRUE_VALUES = {"1", "ON", "YES", "TRUE"}
 ENV_VARS_TRUE_AND_AUTO_VALUES = ENV_VARS_TRUE_VALUES.union({"AUTO"})
 
 USE_PADDLE = os.environ.get("USE_PADDLE", "AUTO").upper()
 
+STR_OPERATION_TO_FUNC = {">": op.gt, ">=": op.ge, "==": op.eq, "!=": op.ne, "<=": op.le, "<": op.lt}
+
 _paddle_version = "N/A"
 if USE_PADDLE in ENV_VARS_TRUE_AND_AUTO_VALUES:
     _paddle_available = importlib.util.find_spec("paddle") is not None
     if _paddle_available:
         try:
             import paddle
+
             _paddle_version = paddle.__version__
             logger.info(f"Paddle version {_paddle_version} available.")
         except importlib_metadata.PackageNotFoundError:
             _paddle_available = False
 else:
     logger.info("Disabling Paddle because USE_PADDLE is not set.")
     _paddle_available = False
 
 _paddlenlp_available = importlib.util.find_spec("paddlenlp") is not None
 try:
     _paddlenlp_version = importlib_metadata.version("paddlenlp")
-    logger.debug(
-        f"Successfully imported paddlenlp version {_paddlenlp_version}")
+    logger.debug(f"Successfully imported paddlenlp version {_paddlenlp_version}")
 except importlib_metadata.PackageNotFoundError:
     _paddlenlp_available = False
 
 _inflect_available = importlib.util.find_spec("inflect") is not None
 try:
     _inflect_version = importlib_metadata.version("inflect")
     logger.debug(f"Successfully imported inflect version {_inflect_version}")
 except importlib_metadata.PackageNotFoundError:
     _inflect_available = False
 
 _unidecode_available = importlib.util.find_spec("unidecode") is not None
 try:
     _unidecode_version = importlib_metadata.version("unidecode")
-    logger.debug(
-        f"Successfully imported unidecode version {_unidecode_version}")
+    logger.debug(f"Successfully imported unidecode version {_unidecode_version}")
 except importlib_metadata.PackageNotFoundError:
     _unidecode_available = False
 
 _modelcards_available = importlib.util.find_spec("modelcards") is not None
 try:
     _modelcards_version = importlib_metadata.version("modelcards")
-    logger.debug(
-        f"Successfully imported modelcards version {_modelcards_version}")
+    logger.debug(f"Successfully imported modelcards version {_modelcards_version}")
 except importlib_metadata.PackageNotFoundError:
     _modelcards_available = False
 
+_onnxruntime_version = "N/A"
 _onnx_available = importlib.util.find_spec("onnxruntime") is not None
 if _onnx_available:
-    candidates = ("onnxruntime", "onnxruntime-gpu", "onnxruntime-directml",
-                  "onnxruntime-openvino")
+    candidates = (
+        "onnxruntime",
+        "onnxruntime-gpu",
+        "onnxruntime-directml",
+        "onnxruntime-openvino",
+        "ort_nightly_directml",
+    )
     _onnxruntime_version = None
     # For the metadata, we have to look for both onnxruntime and onnxruntime-gpu
     for pkg in candidates:
         try:
             _onnxruntime_version = importlib_metadata.version(pkg)
             break
         except importlib_metadata.PackageNotFoundError:
             pass
     _onnx_available = _onnxruntime_version is not None
     if _onnx_available:
-        logger.debug(
-            f"Successfully imported onnxruntime version {_onnxruntime_version}")
+        logger.debug(f"Successfully imported onnxruntime version {_onnxruntime_version}")
 
 _scipy_available = importlib.util.find_spec("scipy") is not None
 try:
     _scipy_version = importlib_metadata.version("scipy")
     logger.debug(f"Successfully imported scipy version {_scipy_version}")
 except importlib_metadata.PackageNotFoundError:
     _scipy_available = False
@@ -115,16 +122,15 @@
         try:
             _fastdeploy_version = importlib_metadata.version(pkg)
             break
         except importlib_metadata.PackageNotFoundError:
             pass
     _fastdeploy_available = _fastdeploy_version is not None
     if _fastdeploy_available:
-        logger.debug(
-            f"Successfully imported fastdeploy version {_fastdeploy_version}")
+        logger.debug(f"Successfully imported fastdeploy version {_fastdeploy_version}")
 
 
 def is_paddle_available():
     return _paddle_available
 
 
 def is_paddlenlp_available():
@@ -152,24 +158,31 @@
 
 
 def is_fastdeploy_available():
     return _fastdeploy_available
 
 
 # docstyle-ignore
+FASTDEPLOY_IMPORT_ERROR = """
+{0} requires the fastdeploy library but it was not found in your environment. You can install it with pip: `pip install
+fastdeploy-gpu-python -f https://www.paddlepaddle.org.cn/whl/fastdeploy.html`
+"""
+
+# docstyle-ignore
 INFLECT_IMPORT_ERROR = """
 {0} requires the inflect library but it was not found in your environment. You can install it with pip: `pip install
 inflect`
 """
 
 # docstyle-ignore
 PADDLE_IMPORT_ERROR = """
 {0} requires the Paddle library but it was not found in your environment. Checkout the instructions on the
 installation page: https://www.paddlepaddle.org.cn/install/quick and follow the ones that match your environment.
 """
+
 # docstyle-ignore
 ONNX_IMPORT_ERROR = """
 {0} requires the onnxruntime library but it was not found in your environment. You can install it with pip: `pip
 install onnxruntime`
 """
 
 # docstyle-ignore
@@ -186,22 +199,25 @@
 
 # docstyle-ignore
 UNIDECODE_IMPORT_ERROR = """
 {0} requires the unidecode library but it was not found in your environment. You can install it with pip: `pip install
 Unidecode`
 """
 
-BACKENDS_MAPPING = OrderedDict([
-    ("inflect", (is_inflect_available, INFLECT_IMPORT_ERROR)),
-    ("onnx", (is_onnx_available, ONNX_IMPORT_ERROR)),
-    ("scipy", (is_scipy_available, SCIPY_IMPORT_ERROR)),
-    ("paddle", (is_paddle_available, PADDLE_IMPORT_ERROR)),
-    ("paddlenlp", (is_paddlenlp_available, PADDLENLP_IMPORT_ERROR)),
-    ("unidecode", (is_unidecode_available, UNIDECODE_IMPORT_ERROR)),
-])
+BACKENDS_MAPPING = OrderedDict(
+    [
+        ("fastdeploy", (is_fastdeploy_available, FASTDEPLOY_IMPORT_ERROR)),
+        ("inflect", (is_inflect_available, INFLECT_IMPORT_ERROR)),
+        ("onnx", (is_onnx_available, ONNX_IMPORT_ERROR)),
+        ("scipy", (is_scipy_available, SCIPY_IMPORT_ERROR)),
+        ("paddle", (is_paddle_available, PADDLE_IMPORT_ERROR)),
+        ("paddlenlp", (is_paddlenlp_available, PADDLENLP_IMPORT_ERROR)),
+        ("unidecode", (is_unidecode_available, UNIDECODE_IMPORT_ERROR)),
+    ]
+)
 
 
 def requires_backends(obj, backends):
     if not isinstance(backends, (list, tuple)):
         backends = [backends]
 
     name = obj.__name__ if hasattr(obj, "__name__") else obj.__class__.__name__
@@ -217,7 +233,40 @@
     `requires_backend` each time a user tries to access any method of that class.
     """
 
     def __getattr__(cls, key):
         if key.startswith("_"):
             return super().__getattr__(cls, key)
         requires_backends(cls, cls._backends)
+
+
+# This function was copied from: https://github.com/huggingface/accelerate/blob/874c4967d94badd24f893064cc3bef45f57cadf7/src/accelerate/utils/versions.py#L319
+def compare_versions(library_or_version: Union[str, Version], operation: str, requirement_version: str):
+    """
+    Args:
+    Compares a library version to some requirement using a given operation.
+        library_or_version (`str` or `packaging.version.Version`):
+            A library name or a version to check.
+        operation (`str`):
+            A string representation of an operator, such as `">"` or `"<="`.
+        requirement_version (`str`):
+            The version to compare the library version against
+    """
+    if operation not in STR_OPERATION_TO_FUNC.keys():
+        raise ValueError(f"`operation` must be one of {list(STR_OPERATION_TO_FUNC.keys())}, received {operation}")
+    operation = STR_OPERATION_TO_FUNC[operation]
+    if isinstance(library_or_version, str):
+        library_or_version = parse(importlib_metadata.version(library_or_version))
+    return operation(library_or_version, parse(requirement_version))
+
+
+# This function was copied from: https://github.com/huggingface/accelerate/blob/874c4967d94badd24f893064cc3bef45f57cadf7/src/accelerate/utils/versions.py#L338
+def is_paddle_version(operation: str, version: str):
+    """
+    Args:
+    Compares the current Paddle version to a given reference with an operation.
+        operation (`str`):
+            A string representation of an operator, such as `">"` or `"<="`
+        version (`str`):
+            A string version of Paddle
+    """
+    return compare_versions(parse(_paddle_version), operation, version)
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/utils/logging.py` & `ppdiffusers-0.9.0/ppdiffusers/utils/logging.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,25 +44,26 @@
 _default_log_level = logging.WARNING
 
 _tqdm_active = True
 
 
 def _get_default_logging_level():
     """
-    If DIFFUSERS_VERBOSITY env var is set to one of the valid choices return that as the new default level. If it is
+    If PPDIFFUSERS_VERBOSITY env var is set to one of the valid choices return that as the new default level. If it is
     not - fall back to `_default_log_level`
     """
-    env_level_str = os.getenv("DIFFUSERS_VERBOSITY", None)
+    env_level_str = os.getenv("PPDIFFUSERS_VERBOSITY", None)
     if env_level_str:
         if env_level_str in log_levels:
             return log_levels[env_level_str]
         else:
             logging.getLogger().warning(
-                f"Unknown option DIFFUSERS_VERBOSITY={env_level_str}, "
-                f"has to be one of: { ', '.join(log_levels.keys()) }")
+                f"Unknown option PPDIFFUSERS_VERBOSITY={env_level_str}, "
+                f"has to be one of: { ', '.join(log_levels.keys()) }"
+            )
     return _default_log_level
 
 
 def _get_library_name() -> str:
     return __name__.split(".")[0]
 
 
@@ -116,22 +117,22 @@
 
     _configure_library_root_logger()
     return logging.getLogger(name)
 
 
 def get_verbosity() -> int:
     """
-    Return the current level for the paddlenlp Diffusers Paddle' root logger as an int.
+    Return the current level for the PaddleNLP PPDiffusers' root logger as an int.
 
     Returns:
         `int`: The logging level.
 
     <Tip>
 
-    paddlenlp Diffusers Paddle has following logging levels:
+    PaddleNLP PPDiffusers has following logging levels:
 
     - 50: `ppdiffusers.logging.CRITICAL` or `ppdiffusers.logging.FATAL`
     - 40: `ppdiffusers.logging.ERROR`
     - 30: `ppdiffusers.logging.WARNING` or `ppdiffusers.logging.WARN`
     - 20: `ppdiffusers.logging.INFO`
     - 10: `ppdiffusers.logging.DEBUG`
 
@@ -139,15 +140,15 @@
 
     _configure_library_root_logger()
     return _get_library_root_logger().getEffectiveLevel()
 
 
 def set_verbosity(verbosity: int) -> None:
     """
-    Set the verbosity level for the paddlenlp Diffusers Paddle' root logger.
+    Set the verbosity level for the PaddleNLP PPDiffusers' root logger.
 
     Args:
         verbosity (`int`):
             Logging level, e.g., one of:
 
             - `ppdiffusers.logging.CRITICAL` or `ppdiffusers.logging.FATAL`
             - `ppdiffusers.logging.ERROR`
@@ -177,104 +178,101 @@
 
 def set_verbosity_error():
     """Set the verbosity to the `ERROR` level."""
     return set_verbosity(ERROR)
 
 
 def disable_default_handler() -> None:
-    """Disable the default handler of the paddlenlp Diffusers Paddle' root logger."""
+    """Disable the default handler of the PaddleNLP PPDiffusers' root logger."""
 
     _configure_library_root_logger()
 
     assert _default_handler is not None
     _get_library_root_logger().removeHandler(_default_handler)
 
 
 def enable_default_handler() -> None:
-    """Enable the default handler of the paddlenlp Diffusers Paddle' root logger."""
+    """Enable the default handler of the PaddleNLP PPDiffusers' root logger."""
 
     _configure_library_root_logger()
 
     assert _default_handler is not None
     _get_library_root_logger().addHandler(_default_handler)
 
 
 def add_handler(handler: logging.Handler) -> None:
-    """adds a handler to the paddlenlp Diffusers Paddle' root logger."""
+    """adds a handler to the PaddleNLP PPDiffusers' root logger."""
 
     _configure_library_root_logger()
 
     assert handler is not None
     _get_library_root_logger().addHandler(handler)
 
 
 def remove_handler(handler: logging.Handler) -> None:
-    """removes given handler from the paddlenlp Diffusers Paddle' root logger."""
+    """removes given handler from the PaddleNLP PPDiffusers' root logger."""
 
     _configure_library_root_logger()
 
-    assert handler is not None and handler not in _get_library_root_logger(
-    ).handlers
+    assert handler is not None and handler not in _get_library_root_logger().handlers
     _get_library_root_logger().removeHandler(handler)
 
 
 def disable_propagation() -> None:
     """
     Disable propagation of the library log outputs. Note that log propagation is disabled by default.
     """
 
     _configure_library_root_logger()
     _get_library_root_logger().propagate = False
 
 
 def enable_propagation() -> None:
     """
-    Enable propagation of the library log outputs. Please disable the paddlenlp Diffusers Paddle' default handler to prevent
+    Enable propagation of the library log outputs. Please disable the PaddleNLP PPDiffusers' default handler to prevent
     double logging if the root logger has been configured.
     """
 
     _configure_library_root_logger()
     _get_library_root_logger().propagate = True
 
 
 def enable_explicit_format() -> None:
     """
-    Enable explicit formatting for every paddlenlp Diffusers Paddle' logger. The explicit formatter is as follows:
+    Enable explicit formatting for every PaddleNLP PPDiffusers' logger. The explicit formatter is as follows:
     ```
         [LEVELNAME|FILENAME|LINE NUMBER] TIME >> MESSAGE
     ```
     All handlers currently bound to the root logger are affected by this method.
     """
     handlers = _get_library_root_logger().handlers
 
     for handler in handlers:
-        formatter = logging.Formatter(
-            "[%(levelname)s|%(filename)s:%(lineno)s] %(asctime)s >> %(message)s"
-        )
+        formatter = logging.Formatter("[%(levelname)s|%(filename)s:%(lineno)s] %(asctime)s >> %(message)s")
         handler.setFormatter(formatter)
 
 
 def reset_format() -> None:
     """
-    Resets the formatting for paddlenlp Diffusers Paddle' loggers.
+    Resets the formatting for PaddleNLP PPDiffusers' loggers.
 
     All handlers currently bound to the root logger are affected by this method.
     """
     handlers = _get_library_root_logger().handlers
 
     for handler in handlers:
         handler.setFormatter(None)
 
 
 def warning_advice(self, *args, **kwargs):
     """
-    This method is identical to `logger.warning()`, but if env var DIFFUSERS_NO_ADVISORY_WARNINGS=1 is set, this
+    This method is identical to `logger.warning()`, but if env var PPDIFFUSERS_NO_ADVISORY_WARNINGS=1 is set, this
     warning will not be printed
     """
-    no_advisory_warnings = os.getenv("DIFFUSERS_NO_ADVISORY_WARNINGS", False)
+    no_advisory_warnings = os.getenv("PPDIFFUSERS_NO_ADVISORY_WARNINGS", False)
     if no_advisory_warnings:
         return
     self.warning(*args, **kwargs)
 
 
 logging.Logger.warning_advice = warning_advice
 
@@ -300,15 +298,14 @@
         return self
 
     def __exit__(self, type_, value, traceback):
         return
 
 
 class _tqdm_cls:
-
     def __call__(self, *args, **kwargs):
         if _tqdm_active:
             return tqdm_lib.tqdm(*args, **kwargs)
         else:
             return EmptyTqdm(*args, **kwargs)
 
     def set_lock(self, *args, **kwargs):
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/utils/outputs.py` & `ppdiffusers-0.9.0/ppdiffusers/utils/outputs.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 
 def is_tensor(x):
     """
     Tests if `x` is a `paddle.Tensor` or `np.ndarray`.
     """
     if is_paddle_available():
         import paddle
+
         return paddle.is_tensor(x)
 
     return isinstance(x, np.ndarray)
 
 
 class BaseOutput(OrderedDict):
     """
@@ -54,44 +55,36 @@
         class_fields = fields(self)
 
         # Safety and consistency checks
         if not len(class_fields):
             raise ValueError(f"{self.__class__.__name__} has no fields.")
 
         first_field = getattr(self, class_fields[0].name)
-        other_fields_are_none = all(
-            getattr(self, field.name) is None for field in class_fields[1:])
+        other_fields_are_none = all(getattr(self, field.name) is None for field in class_fields[1:])
 
         if other_fields_are_none and isinstance(first_field, dict):
             for key, value in first_field.items():
                 self[key] = value
         else:
             for field in class_fields:
                 v = getattr(self, field.name)
                 if v is not None:
                     self[field.name] = v
 
     def __delitem__(self, *args, **kwargs):
-        raise Exception(
-            f"You cannot use ``__delitem__`` on a {self.__class__.__name__} instance."
-        )
+        raise Exception(f"You cannot use ``__delitem__`` on a {self.__class__.__name__} instance.")
 
     def setdefault(self, *args, **kwargs):
-        raise Exception(
-            f"You cannot use ``setdefault`` on a {self.__class__.__name__} instance."
-        )
+        raise Exception(f"You cannot use ``setdefault`` on a {self.__class__.__name__} instance.")
 
     def pop(self, *args, **kwargs):
-        raise Exception(
-            f"You cannot use ``pop`` on a {self.__class__.__name__} instance.")
+        raise Exception(f"You cannot use ``pop`` on a {self.__class__.__name__} instance.")
 
     def update(self, *args, **kwargs):
-        raise Exception(
-            f"You cannot use ``update`` on a {self.__class__.__name__} instance."
-        )
+        raise Exception(f"You cannot use ``update`` on a {self.__class__.__name__} instance.")
 
     def __getitem__(self, k):
         if isinstance(k, str):
             inner_dict = {k: v for (k, v) in self.items()}
             return inner_dict[k]
         else:
             return self.to_tuple()[k]
@@ -115,10 +108,10 @@
         # try to fix: https://github.com/PaddlePaddle/PaddleNLP/issues/3355
         # when trying to get the keys of `OrderedDict`, `keys` method return empty values.
         # TODO(wj-Mcat): this bug should be fixed in Paddle framework
         tuples = ()
         for field in fields(self):
             if getattr(self, field.name, None) is None:
                 continue
-            tuples = tuples + (getattr(self, field.name), )
+            tuples = tuples + (getattr(self, field.name),)
 
         return tuples
```

### Comparing `ppdiffusers-0.6.3/ppdiffusers/utils/testing_utils.py` & `ppdiffusers-0.9.0/ppdiffusers/utils/testing_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,32 +10,55 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import inspect
+import logging
 import os
 import random
 import re
 import unittest
+import urllib.parse
 from distutils.util import strtobool
+from io import BytesIO, StringIO
 from pathlib import Path
 from typing import Union
 
-import paddle
-
+import numpy as np
 import PIL.Image
 import PIL.ImageOps
 import requests
 
-from .import_utils import is_paddle_available, is_onnx_available
+from .import_utils import is_fastdeploy_available, is_paddle_available
+
+if is_paddle_available():
+    import paddle
 
 global_rng = random.Random()
-paddle_device = "gpu" if paddle.device.is_compiled_with_cuda() else "cpu"
+
+
+def image_grid(imgs, rows, cols):
+    assert len(imgs) == rows * cols
+    w, h = imgs[0].size
+    grid = PIL.Image.new("RGB", size=(cols * w, rows * h))
+
+    for i, img in enumerate(imgs):
+        grid.paste(img, box=(i % cols * w, i // cols * h))
+    return grid
+
+
+def paddle_all_close(a, b, *args, **kwargs):
+    if not is_paddle_available():
+        raise ValueError("Paddle needs to be installed to use this function.")
+
+    if not paddle.allclose(a, b, *args, **kwargs):
+        assert False, f"Max diff is absolute {(a - b).abs().max()}. Diff tensor is {(a - b).abs()}."
+    return True
 
 
 def get_tests_dir(append_path=None):
     """
     Args:
         append_path: optional path to append to the tests dir path
     Return:
@@ -83,15 +106,15 @@
     for dim in shape:
         total_dims *= dim
 
     values = []
     for _ in range(total_dims):
         values.append(rng.random() * scale)
 
-    return paddle.to_tensor(values, dtype="float32").reshape(shape)
+    return paddle.to_tensor(data=values, dtype=paddle.float32).reshape(shape)
 
 
 def slow(test_case):
     """
     Decorator marking a test as slow.
 
     Slow tests are skipped by default. Set the RUN_SLOW environment variable to a truthy value to run them.
@@ -100,30 +123,45 @@
     return unittest.skipUnless(_run_slow_tests, "test is slow")(test_case)
 
 
 def require_paddle(test_case):
     """
     Decorator marking a test that requires Paddle. These tests are skipped when Paddle isn't installed.
     """
-    return unittest.skipUnless(is_paddle_available(),
-                               "test requires Paddle")(test_case)
+    return unittest.skipUnless(is_paddle_available(), "test requires Paddle")(test_case)
 
 
-def require_torch_gpu(test_case):
-    """Decorator marking a test that requires CUDA and Paddle."""
-    return unittest.skipUnless(is_paddle_available() and paddle_device == "gpu",
-                               "test requires Paddle+CUDA")(test_case)
-
-
-def require_onnxruntime(test_case):
+def require_fastdeploy(test_case):
     """
-    Decorator marking a test that requires onnxruntime. These tests are skipped when onnxruntime isn't installed.
+    Decorator marking a test that requires fastdeploy. These tests are skipped when fastdeploy isn't installed.
     """
-    return unittest.skipUnless(is_onnx_available(),
-                               "test requires onnxruntime")(test_case)
+    return unittest.skipUnless(is_fastdeploy_available(), "test requires fastdeploy")(test_case)
+
+
+def load_numpy(arry: Union[str, np.ndarray]) -> np.ndarray:
+    if isinstance(arry, str):
+        if arry.startswith("http://") or arry.startswith("https://"):
+            response = requests.get(arry)
+            response.raise_for_status()
+            arry = np.load(BytesIO(response.content))
+        elif os.path.isfile(arry):
+            arry = np.load(arry)
+        else:
+            raise ValueError(
+                f"Incorrect path or url, URLs must start with `http://` or `https://`, and {arry} is not a valid path"
+            )
+    elif isinstance(arry, np.ndarray):
+        pass
+    else:
+        raise ValueError(
+            "Incorrect format used for numpy ndarray. Should be an url linking to an image, a local path, or a"
+            " ndarray."
+        )
+
+    return arry
 
 
 def load_image(image: Union[str, PIL.Image.Image]) -> PIL.Image.Image:
     """
     Args:
     Loads `image` to a PIL Image.
         image (`str` or `PIL.Image.Image`):
@@ -137,24 +175,41 @@
         elif os.path.isfile(image):
             image = PIL.Image.open(image)
         else:
             raise ValueError(
                 f"Incorrect path or url, URLs must start with `http://` or `https://`, and {image} is not a valid path"
             )
     elif isinstance(image, PIL.Image.Image):
-        pass
+        image = image
     else:
         raise ValueError(
             "Incorrect format used for image. Should be an url linking to an image, a local path, or a PIL image."
         )
     image = PIL.ImageOps.exif_transpose(image)
     image = image.convert("RGB")
     return image
 
 
+def load_hf_numpy(path) -> np.ndarray:
+    if not path.startswith("http://") or path.startswith("https://"):
+        path = os.path.join(
+            "https://huggingface.co/datasets/fusing/diffusers-testing/resolve/main", urllib.parse.quote(path)
+        )
+
+    return load_numpy(path)
+
+
+def load_ppnlp_numpy(path) -> np.ndarray:
+    if not path.startswith("http://") or path.startswith("https://"):
+        path = os.path.join(
+            "https://paddlenlp.bj.bcebos.com/models/community/CompVis/data/diffusers-testing", urllib.parse.quote(path)
+        )
+    return load_numpy(path)
+
+
 # --- pytest conf functions --- #
 
 # to avoid multiple invocation from tests/conftest.py and examples/conftest.py - make sure it's called only once
 pytest_opt_registered = {}
 
 
 def pytest_addoption_shared(parser):
@@ -167,16 +222,15 @@
     """
     option = "--make-reports"
     if option not in pytest_opt_registered:
         parser.addoption(
             option,
             action="store",
             default=False,
-            help=
-            "generate report files. The value of this option is used as a prefix to report names",
+            help="generate report files. The value of this option is used as a prefix to report names",
         )
         pytest_opt_registered[option] = 1
 
 
 def pytest_terminal_summary_main(tr, id):
     """
     Generate multiple reports at the end of test suite run - each report goes into a dedicated file in the current
@@ -235,32 +289,29 @@
     if dlist:
         dlist.sort(key=lambda x: x.duration, reverse=True)
         with open(report_files["durations"], "w") as f:
             durations_min = 0.05  # sec
             f.write("slowest durations\n")
             for i, rep in enumerate(dlist):
                 if rep.duration < durations_min:
-                    f.write(
-                        f"{len(dlist)-i} durations < {durations_min} secs were omitted"
-                    )
+                    f.write(f"{len(dlist)-i} durations < {durations_min} secs were omitted")
                     break
                 f.write(f"{rep.duration:02.2f}s {rep.when:<8} {rep.nodeid}\n")
 
     def summary_failures_short(tr):
         # expecting that the reports were --tb=long (default) so we chop them off here to the last frame
         reports = tr.getreports("failed")
         if not reports:
             return
         tr.write_sep("=", "FAILURES SHORT STACK")
         for rep in reports:
             msg = tr._getfailureheadline(rep)
             tr.write_sep("_", msg, red=True, bold=True)
             # chop off the optional leading extra frames, leaving only the last one
-            longrepr = re.sub(r".*_ _ _ (_ ){10,}_ _ ", "", rep.longreprtext, 0,
-                              re.M | re.S)
+            longrepr = re.sub(r".*_ _ _ (_ ){10,}_ _ ", "", rep.longreprtext, 0, re.M | re.S)
             tr._tw.line(longrepr)
             # note: not printing out any rep.sections to keep the report short
 
     # use ready-made report funcs, we are just hijacking the filehandle to log to a dedicated file each
     # adapted from https://github.com/pytest-dev/pytest/blob/897f151e/src/_pytest/terminal.py#L814
     # note: some pytest plugins may interfere by hijacking the default `terminalreporter` (e.g.
     # pytest-instafail does that)
@@ -303,7 +354,46 @@
         tr._tw = create_terminal_writer(config, f)
         tr.summary_stats()
 
     # restore:
     tr._tw = orig_writer
     tr.reportchars = orig_reportchars
     config.option.tbstyle = orig_tbstyle
+
+
+class CaptureLogger:
+    """
+    Args:
+    Context manager to capture `logging` streams
+        logger: 'logging` logger object
+    Returns:
+        The captured output is available via `self.out`
+    Example:
+    ```python
+    >>> from ppdiffusers import logging
+    >>> from ppdiffusers.testing_utils import CaptureLogger
+
+    >>> msg = "Testing 1, 2, 3"
+    >>> logging.set_verbosity_info()
+    >>> logger = logging.get_logger("ppdiffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.py")
+    >>> with CaptureLogger(logger) as cl:
+    ...     logger.info(msg)
+    >>> assert cl.out, msg + "\n"
+    ```
+    """
+
+    def __init__(self, logger):
+        self.logger = logger
+        self.io = StringIO()
+        self.sh = logging.StreamHandler(self.io)
+        self.out = ""
+
+    def __enter__(self):
+        self.logger.addHandler(self.sh)
+        return self
+
+    def __exit__(self, *exc):
+        self.logger.removeHandler(self.sh)
+        self.out = self.io.getvalue()
+
+    def __repr__(self):
+        return f"captured: {self.out}\n"
```

### Comparing `ppdiffusers-0.6.3/setup.py` & `ppdiffusers-0.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,64 +8,64 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
+
 from setuptools import find_packages, setup
 
 description = "PPDiffusers: Diffusers toolbox implemented based on PaddlePaddle"
 
 with open("requirements.txt") as fin:
     REQUIRED_PACKAGES = fin.read()
 
 
 def read(file: str):
     current_dir = os.path.dirname(__file__)
     path = os.path.join(current_dir, file)
-    with open(path, 'r', encoding='utf-8') as f:
+    with open(path, "r", encoding="utf-8") as f:
         content = f.read().strip()
     return content
 
 
 def read_version():
     """read version of ppdiffusers"""
     return read("VERSION")
 
 
 def read_readme():
     return read("README.md")
 
 
 def read_requirements():
-    content = read('requirements.txt')
+    content = read("requirements.txt")
     packages = content.split("\n")
     return packages
 
 
-setup(name="ppdiffusers",
-      packages=find_packages(),
-      version=read_version(),
-      author="PaddleNLP Team",
-      author_email="paddlenlp@baidu.com",
-      description=description,
-      long_description=read_readme(),
-      long_description_content_type="text/markdown",
-      url="https://github.com/PaddlePaddle/PaddleNLP/ppdiffusers",
-      keywords=["ppdiffusers", "paddle", "paddlenlp"],
-      install_requires=REQUIRED_PACKAGES,
-      python_requires='>=3.6',
-      entry_points={
-          "console_scripts":
-          ["ppdiffusers-cli=ppdiffusers.commands.ppdiffusers_cli:main"]
-      },
-      classifiers=[
-          'Programming Language :: Python :: 3',
-          'Programming Language :: Python :: 3.6',
-          'Programming Language :: Python :: 3.7',
-          'Programming Language :: Python :: 3.8',
-          'Programming Language :: Python :: 3.9',
-          'License :: OSI Approved :: Apache Software License',
-          'Operating System :: OS Independent',
-      ],
-      license='Apache 2.0')
+setup(
+    name="ppdiffusers",
+    packages=find_packages(),
+    version=read_version(),
+    author="PaddleNLP Team",
+    author_email="paddlenlp@baidu.com",
+    description=description,
+    long_description=read_readme(),
+    long_description_content_type="text/markdown",
+    url="https://github.com/PaddlePaddle/PaddleNLP/ppdiffusers",
+    keywords=["ppdiffusers", "paddle", "paddlenlp"],
+    install_requires=REQUIRED_PACKAGES,
+    python_requires=">=3.6",
+    entry_points={"console_scripts": ["ppdiffusers-cli=ppdiffusers.commands.ppdiffusers_cli:main"]},
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "License :: OSI Approved :: Apache Software License",
+        "Operating System :: OS Independent",
+    ],
+    license="Apache 2.0",
+)
```

