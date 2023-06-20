# Comparing `tmp/tonic-1.2.7.dev9.tar.gz` & `tmp/tonic-1.2.8.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tonic-1.2.7.dev9.tar", last modified: Mon Apr 24 12:01:40 2023, max compression
+gzip compressed data, was "tonic-1.2.8.dev4.tar", last modified: Tue Jun 20 10:37:25 2023, max compression
```

## Comparing `tonic-1.2.7.dev9.tar` & `tonic-1.2.8.dev4.tar`

### file list

```diff
@@ -1,189 +1,189 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:01:40.840779 tonic-1.2.7.dev9/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:01:40.820778 tonic-1.2.7.dev9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:01:40.824778 tonic-1.2.7.dev9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/.github/workflows/ci-pipeline.yml
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-24 12:01:40.000000 tonic-1.2.7.dev9/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    38661 2023-04-24 12:01:40.000000 tonic-1.2.7.dev9/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-04-24 12:01:40.840779 tonic-1.2.7.dev9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:01:40.824778 tonic-1.2.7.dev9/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:01:40.824778 tonic-1.2.7.dev9/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:01:40.828778 tonic-1.2.7.dev9/docs/_static/event-cameras/
--rw-r--r--   0 runner    (1001) docker     (123)   460683 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/_static/event-cameras/eventstream.png
--rw-r--r--   0 runner    (1001) docker     (123)   209036 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/_static/event-cameras/framestream.png
--rw-r--r--   0 runner    (1001) docker     (123)    28336 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/_static/event-cameras/receptive-fields.png
--rw-r--r--   0 runner    (1001) docker     (123)    18392 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/_static/event-cameras/sampling-theorems.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:01:40.828778 tonic-1.2.7.dev9/docs/_static/snn/
--rw-r--r--   0 runner    (1001) docker     (123)   119778 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/_static/snn/neuron-models.png
--rw-r--r--   0 runner    (1001) docker     (123)    62505 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/_static/snn/surrogates.png
--rw-r--r--   0 runner    (1001) docker     (123)   196968 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/_static/tonic-logo-black.png
--rw-r--r--   0 runner    (1001) docker     (123)   193807 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/_static/tonic-logo-white.png
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/_static/tonic_favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:01:40.828778 tonic-1.2.7.dev9/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/_templates/class_dataset.rst
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/_templates/class_transform.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:01:40.828778 tonic-1.2.7.dev9/docs/about/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/about/about.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/about/info.rst
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/about/prototype.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/about/release_notes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/datasets.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:01:40.828778 tonic-1.2.7.dev9/docs/gallery/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/gallery/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:01:40.828778 tonic-1.2.7.dev9/docs/gallery/representations/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/gallery/representations/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/gallery/representations/plot_tobinarep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/gallery/representations/plot_toframe.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/gallery/representations/plot_toimage.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/gallery/representations/plot_totimesurface.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/gallery/representations/plot_tovoxelgrid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:01:40.832779 tonic-1.2.7.dev9/docs/gallery/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/gallery/transformations/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/gallery/transformations/plot_centercrop.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/gallery/transformations/plot_crop_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/gallery/transformations/plot_decimation.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/gallery/transformations/plot_denoise.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/gallery/transformations/plot_downsample.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/gallery/transformations/plot_drop_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/gallery/transformations/plot_drop_event_by_area.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/gallery/transformations/plot_drop_event_by_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/gallery/transformations/plot_drop_pixel.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/gallery/transformations/plot_merge_polarities.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/gallery/transformations/plot_random_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/gallery/transformations/plot_random_flip_lr.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/gallery/transformations/plot_random_flip_ud.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/gallery/transformations/plot_random_time_reversal.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/gallery/transformations/plot_refractory_period.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/gallery/transformations/plot_spatial_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/gallery/transformations/plot_time_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/gallery/transformations/plot_uniform_noise.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:01:40.832779 tonic-1.2.7.dev9/docs/getting_involved/
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/getting_involved/communication_channels.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7127 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/getting_involved/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/getting_involved/getting_involved.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:01:40.832779 tonic-1.2.7.dev9/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/getting_started/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/getting_started/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8975 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/getting_started/nmnist.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:01:40.832779 tonic-1.2.7.dev9/docs/how-tos/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/how-tos/how-tos.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/how-tos/loading-raw-events.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/how-tos/visualizing-data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/how-tos/wrapping_own_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:01:40.832779 tonic-1.2.7.dev9/docs/reading_material/
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/reading_material/design_choices.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11178 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/reading_material/intro-event-cameras.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/reading_material/intro-snns.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/reading_material/reading_material.rst
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/reading_material/training-snns.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/transformations.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:01:40.832779 tonic-1.2.7.dev9/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/tutorials/batching.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/tutorials/davis_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/tutorials/fast_dataloading.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12518 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/tutorials/large_datasets.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/tutorials/slicing.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/docs/tutorials/tutorials.rst
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-24 12:01:40.844779 tonic-1.2.7.dev9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:01:40.832779 tonic-1.2.7.dev9/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/test/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/test/prototype_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/test/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/test/test_audio_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/test/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/test/test_chained_transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:01:40.836778 tonic-1.2.7.dev9/test/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)   949253 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/test/test_data/sample.aedat4
--rw-r--r--   0 runner    (1001) docker     (123)    16165 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/test/test_data/sample_ncars.dat
--rw-r--r--   0 runner    (1001) docker     (123)    21625 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/test/test_data/sample_nmnist.bin
--rw-r--r--   0 runner    (1001) docker     (123)    38132 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/test/test_data/sample_stmnist.mat
--rw-r--r--   0 runner    (1001) docker     (123)     7514 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/test/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/test/test_dsec.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/test/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/test/test_prototype_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9114 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/test/test_representations.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/test/test_sliced_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/test/test_slicers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/test/test_tonic_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18669 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/test/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/test/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:01:40.836778 tonic-1.2.7.dev9/tonic/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9561 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/audio_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/cached_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/collation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:01:40.840779 tonic-1.2.7.dev9/tonic/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/datasets/asl_dvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/datasets/cifar10dvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/datasets/davisdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14707 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/datasets/dsec.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/datasets/dvs_lips.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/datasets/dvsgesture.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/datasets/hsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/datasets/mvsec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/datasets/ncaltech101.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/datasets/nmnist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/datasets/pokerdvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/datasets/s_mnist.py
--rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/datasets/tum_vie.py
--rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/datasets/visual_place_recognition.py
--rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/download_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:01:40.840779 tonic-1.2.7.dev9/tonic/functional/
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/functional/crop.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/functional/decimate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/functional/denoise.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/functional/drop_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/functional/drop_pixel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/functional/refractory_period.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/functional/spatial_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/functional/time_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/functional/time_skew.py
--rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/functional/to_averaged_timesurface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/functional/to_bina_rep.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/functional/to_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/functional/to_timesurface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/functional/to_voxel_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/functional/uniform_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     8277 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:01:40.840779 tonic-1.2.7.dev9/tonic/prototype/
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/prototype/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/prototype/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:01:40.840779 tonic-1.2.7.dev9/tonic/prototype/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/prototype/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/prototype/datasets/ncars.py
--rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/prototype/datasets/nmnist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/prototype/datasets/prophesee.py
--rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/prototype/datasets/stmnist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:01:40.840779 tonic-1.2.7.dev9/tonic/prototype/datasets/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/prototype/datasets/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/prototype/datasets/utils/_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/prototype/datasets/utils/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/prototype/slicers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/sliced_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/slicers.py
--rw-r--r--   0 runner    (1001) docker     (123)    37967 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   212526 2023-04-24 12:01:27.000000 tonic-1.2.7.dev9/tonic-logo-padded.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:01:40.836778 tonic-1.2.7.dev9/tonic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-04-24 12:01:40.000000 tonic-1.2.7.dev9/tonic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-04-24 12:01:40.000000 tonic-1.2.7.dev9/tonic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 12:01:40.000000 tonic-1.2.7.dev9/tonic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 12:01:40.000000 tonic-1.2.7.dev9/tonic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-24 12:01:40.000000 tonic-1.2.7.dev9/tonic.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-24 12:01:40.000000 tonic-1.2.7.dev9/tonic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-24 12:01:40.000000 tonic-1.2.7.dev9/tonic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.778264 tonic-1.2.8.dev4/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.754264 tonic-1.2.8.dev4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.758264 tonic-1.2.8.dev4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/.github/workflows/ci-pipeline.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-20 10:37:25.000000 tonic-1.2.8.dev4/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    39513 2023-06-20 10:37:25.000000 tonic-1.2.8.dev4/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-06-20 10:37:25.778264 tonic-1.2.8.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.762264 tonic-1.2.8.dev4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.762264 tonic-1.2.8.dev4/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.762264 tonic-1.2.8.dev4/docs/_static/event-cameras/
+-rw-r--r--   0 runner    (1001) docker     (123)   460683 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/_static/event-cameras/eventstream.png
+-rw-r--r--   0 runner    (1001) docker     (123)   209036 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/_static/event-cameras/framestream.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28336 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/_static/event-cameras/receptive-fields.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18392 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/_static/event-cameras/sampling-theorems.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.762264 tonic-1.2.8.dev4/docs/_static/snn/
+-rw-r--r--   0 runner    (1001) docker     (123)   119778 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/_static/snn/neuron-models.png
+-rw-r--r--   0 runner    (1001) docker     (123)    62505 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/_static/snn/surrogates.png
+-rw-r--r--   0 runner    (1001) docker     (123)   196968 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/_static/tonic-logo-black.png
+-rw-r--r--   0 runner    (1001) docker     (123)   193807 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/_static/tonic-logo-white.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/_static/tonic_favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.762264 tonic-1.2.8.dev4/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/_templates/class_dataset.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/_templates/class_transform.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.762264 tonic-1.2.8.dev4/docs/about/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/about/about.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/about/info.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/about/prototype.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/about/release_notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/datasets.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.762264 tonic-1.2.8.dev4/docs/gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.766264 tonic-1.2.8.dev4/docs/gallery/representations/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/representations/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/representations/plot_tobinarep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/representations/plot_toframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/representations/plot_toimage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/representations/plot_totimesurface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/representations/plot_tovoxelgrid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.766264 tonic-1.2.8.dev4/docs/gallery/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/transformations/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/transformations/plot_centercrop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/transformations/plot_crop_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/transformations/plot_decimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/transformations/plot_denoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/transformations/plot_downsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/transformations/plot_drop_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/transformations/plot_drop_event_by_area.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/transformations/plot_drop_event_by_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/transformations/plot_drop_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/transformations/plot_merge_polarities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/transformations/plot_random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/transformations/plot_random_flip_lr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/transformations/plot_random_flip_ud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/transformations/plot_random_time_reversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/transformations/plot_refractory_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/transformations/plot_spatial_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/transformations/plot_time_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/gallery/transformations/plot_uniform_noise.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.766264 tonic-1.2.8.dev4/docs/getting_involved/
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/getting_involved/communication_channels.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7127 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/getting_involved/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/getting_involved/getting_involved.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.766264 tonic-1.2.8.dev4/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/getting_started/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/getting_started/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8975 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/getting_started/nmnist.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.766264 tonic-1.2.8.dev4/docs/how-tos/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/how-tos/how-tos.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/how-tos/loading-raw-events.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/how-tos/visualizing-data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/how-tos/wrapping_own_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.766264 tonic-1.2.8.dev4/docs/reading_material/
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/reading_material/design_choices.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11178 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/reading_material/intro-event-cameras.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/reading_material/intro-snns.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/reading_material/reading_material.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/reading_material/training-snns.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/transformations.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.770264 tonic-1.2.8.dev4/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/tutorials/batching.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/tutorials/davis_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/tutorials/fast_dataloading.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12518 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/tutorials/large_datasets.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/tutorials/slicing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/docs/tutorials/tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-20 10:37:25.778264 tonic-1.2.8.dev4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.770264 tonic-1.2.8.dev4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/test/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/test/prototype_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/test/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/test/test_audio_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/test/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/test/test_chained_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.770264 tonic-1.2.8.dev4/test/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)   949253 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/test/test_data/sample.aedat4
+-rw-r--r--   0 runner    (1001) docker     (123)    16165 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/test/test_data/sample_ncars.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    21625 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/test/test_data/sample_nmnist.bin
+-rw-r--r--   0 runner    (1001) docker     (123)    38132 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/test/test_data/sample_stmnist.mat
+-rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/test/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/test/test_dsec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/test/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10105 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/test/test_prototype_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9644 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/test/test_representations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/test/test_sliced_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/test/test_slicers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/test/test_tonic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18669 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/test/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/test/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.774264 tonic-1.2.8.dev4/tonic/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9561 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/audio_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/cached_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/collation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.774264 tonic-1.2.8.dev4/tonic/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/datasets/asl_dvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/datasets/cifar10dvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/datasets/davisdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14707 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/datasets/dsec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/datasets/dvs_lips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/datasets/dvsgesture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/datasets/hsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/datasets/mvsec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/datasets/ncaltech101.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/datasets/nmnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/datasets/pokerdvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/datasets/s_mnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/datasets/tum_vie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/datasets/visual_place_recognition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/download_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.778264 tonic-1.2.8.dev4/tonic/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/functional/crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/functional/decimate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/functional/denoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/functional/drop_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/functional/drop_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/functional/refractory_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/functional/spatial_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/functional/time_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/functional/time_skew.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/functional/to_averaged_timesurface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/functional/to_bina_rep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/functional/to_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/functional/to_timesurface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/functional/to_voxel_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/functional/uniform_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8277 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.778264 tonic-1.2.8.dev4/tonic/prototype/
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/prototype/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/prototype/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.778264 tonic-1.2.8.dev4/tonic/prototype/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/prototype/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/prototype/datasets/ncars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/prototype/datasets/nmnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/prototype/datasets/prophesee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/prototype/datasets/stmnist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.778264 tonic-1.2.8.dev4/tonic/prototype/datasets/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/prototype/datasets/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/prototype/datasets/utils/_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/prototype/datasets/utils/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/prototype/slicers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/sliced_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/slicers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38208 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   212526 2023-06-20 10:37:06.000000 tonic-1.2.8.dev4/tonic-logo-padded.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:37:25.774264 tonic-1.2.8.dev4/tonic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-06-20 10:37:25.000000 tonic-1.2.8.dev4/tonic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-06-20 10:37:25.000000 tonic-1.2.8.dev4/tonic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 10:37:25.000000 tonic-1.2.8.dev4/tonic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 10:37:25.000000 tonic-1.2.8.dev4/tonic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-20 10:37:25.000000 tonic-1.2.8.dev4/tonic.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-20 10:37:25.000000 tonic-1.2.8.dev4/tonic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 10:37:25.000000 tonic-1.2.8.dev4/tonic.egg-info/top_level.txt
```

### Comparing `tonic-1.2.7.dev9/.github/workflows/ci-pipeline.yml` & `tonic-1.2.8.dev4/.github/workflows/ci-pipeline.yml`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/AUTHORS` & `tonic-1.2.8.dev4/AUTHORS`

 * *Files 4% similar despite different names*

```diff
@@ -27,12 +27,13 @@
 fabrizio.ottati <fabrizio.ottati@studenti.polito.it>
 guidoz <guidoz@users.noreply.github.com>
 k-chaney <chaneyk@seas.upenn.edu>
 kai.wang <kai.wang@synsense.ai>
 neworderofjamie <J.C.Knight@sussex.ac.uk>
 neworderofjamie <neworderofjamie@gmail.com>
 nogay.kuepelioglu <kupelioglun@mef.edu.tr>
+nogay.kuepelioglu <nogay.kuepelioglu@synsense.ai>
 sadique.sheik <sadique.sheik@synsense.ai>
 twelshm <twelshm@gmail.com>
 ugurcan.cakal <ugurcan.cakal@synsense.ai>
 wangkgege <wangk.gege@gmail.com>
 yannan xing <yannan.xing@synsense.ai>
```

### Comparing `tonic-1.2.7.dev9/ChangeLog` & `tonic-1.2.8.dev4/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,32 @@
 CHANGES
 =======
 
+* Add delta\_t as a parameter to time surface test
+* Remove print statements to evaluate correctness
+* Time surface returns time surfaces at interval
+
+v1.2.7
+------
+
+* raise error if single polarity is used for sensor size but data contains more than one polarity
+* add speaker information to SSC
+* upload POKERDVS to different server
+* host dataset samples on Gregor Nextcloud to fix tests
+* make list of classes in CIFAR10DVS a class attribute
+* add Gen4 downsampled version
+* update Gen4Automotive docstring
+* add Gen4Automotive dataset
+* update Prophesee docstrings
+* add dataset length to Gen1Automotive
+* make sure Prophesee datasets are shuffled correctly
+* remove transform/target\_transform from prototype datasets and use dicts as sensor\_sizes
+* add Gen1 automotive detection dataset
+* add Gen1AutomotiveDetection
+* Update training-snns.rst
 * add class map to Gen4 detection dataset and remove transform arguments
 * add prototype slicers
 * update pre-commit config
 * Added to test\_datasets.py to enable generating the speaker element of SHD dataset for tests
 * Exposed the extra/speaker property in the SHD dataset to users so that it can be accessed when needed
 * Update \`Bin\` docstring
 * Update \`FixLength\` docstring
```

### Comparing `tonic-1.2.7.dev9/LICENSE.txt` & `tonic-1.2.8.dev4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/PKG-INFO` & `tonic-1.2.8.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonic
-Version: 1.2.7.dev9
+Version: 1.2.8.dev4
 Summary: Neuromorphic datasets and transformations.
 Home-page: UNKNOWN
 Author: The Neuromorphs of Telluride
 Author-email: mail@lenzgregor.com
 License: GNU GPLv3
 Project-URL: Source code, https://github.com/neuromorphs/tonic
 Project-URL: Documentation, https://tonic.readthedocs.org
```

### Comparing `tonic-1.2.7.dev9/README.md` & `tonic-1.2.8.dev4/README.md`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/Makefile` & `tonic-1.2.8.dev4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/_static/event-cameras/eventstream.png` & `tonic-1.2.8.dev4/docs/_static/event-cameras/eventstream.png`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/_static/event-cameras/framestream.png` & `tonic-1.2.8.dev4/docs/_static/event-cameras/framestream.png`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/_static/event-cameras/receptive-fields.png` & `tonic-1.2.8.dev4/docs/_static/event-cameras/receptive-fields.png`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/_static/event-cameras/sampling-theorems.png` & `tonic-1.2.8.dev4/docs/_static/event-cameras/sampling-theorems.png`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/_static/snn/neuron-models.png` & `tonic-1.2.8.dev4/docs/_static/snn/neuron-models.png`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/_static/snn/surrogates.png` & `tonic-1.2.8.dev4/docs/_static/snn/surrogates.png`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/_static/tonic-logo-black.png` & `tonic-1.2.8.dev4/docs/_static/tonic-logo-black.png`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/_static/tonic-logo-white.png` & `tonic-1.2.8.dev4/docs/_static/tonic-logo-white.png`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/_static/tonic_favicon.png` & `tonic-1.2.8.dev4/docs/_static/tonic_favicon.png`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/about/info.rst` & `tonic-1.2.8.dev4/docs/about/info.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/about/prototype.rst` & `tonic-1.2.8.dev4/docs/about/prototype.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/about/release_notes.rst` & `tonic-1.2.8.dev4/docs/about/release_notes.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/conf.py` & `tonic-1.2.8.dev4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/datasets.rst` & `tonic-1.2.8.dev4/docs/datasets.rst`

 * *Files 4% similar despite different names*

```diff
@@ -53,8 +53,9 @@
 .. autosummary::
     :toctree: generated/
     :template: class_dataset.rst
 
     NMNIST
     NCARS
     STMNIST
+    Gen1AutomotiveDetection
     Gen4AutomotiveDetectionMini
```

### Comparing `tonic-1.2.7.dev9/docs/gallery/representations/plot_tobinarep.py` & `tonic-1.2.8.dev4/docs/gallery/representations/plot_tobinarep.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/gallery/representations/plot_toframe.py` & `tonic-1.2.8.dev4/docs/gallery/representations/plot_toframe.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/gallery/representations/plot_toimage.py` & `tonic-1.2.8.dev4/docs/gallery/representations/plot_toimage.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/gallery/representations/plot_totimesurface.py` & `tonic-1.2.8.dev4/docs/gallery/representations/plot_totimesurface.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/gallery/transformations/plot_centercrop.py` & `tonic-1.2.8.dev4/docs/gallery/transformations/plot_centercrop.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/gallery/transformations/plot_crop_time.py` & `tonic-1.2.8.dev4/docs/gallery/transformations/plot_crop_time.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/gallery/transformations/plot_decimation.py` & `tonic-1.2.8.dev4/docs/gallery/transformations/plot_decimation.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/gallery/transformations/plot_denoise.py` & `tonic-1.2.8.dev4/docs/gallery/transformations/plot_denoise.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/gallery/transformations/plot_downsample.py` & `tonic-1.2.8.dev4/docs/gallery/transformations/plot_downsample.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/gallery/transformations/plot_drop_event.py` & `tonic-1.2.8.dev4/docs/gallery/transformations/plot_drop_event.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/gallery/transformations/plot_drop_event_by_area.py` & `tonic-1.2.8.dev4/docs/gallery/transformations/plot_drop_event_by_area.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/gallery/transformations/plot_drop_event_by_time.py` & `tonic-1.2.8.dev4/docs/gallery/transformations/plot_drop_event_by_time.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/gallery/transformations/plot_drop_pixel.py` & `tonic-1.2.8.dev4/docs/gallery/transformations/plot_drop_pixel.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/gallery/transformations/plot_merge_polarities.py` & `tonic-1.2.8.dev4/docs/gallery/transformations/plot_merge_polarities.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/gallery/transformations/plot_random_crop.py` & `tonic-1.2.8.dev4/docs/gallery/transformations/plot_random_crop.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/gallery/transformations/plot_random_flip_lr.py` & `tonic-1.2.8.dev4/docs/gallery/transformations/plot_random_flip_lr.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/gallery/transformations/plot_random_flip_ud.py` & `tonic-1.2.8.dev4/docs/gallery/transformations/plot_random_flip_ud.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/gallery/transformations/plot_random_time_reversal.py` & `tonic-1.2.8.dev4/docs/gallery/transformations/plot_random_time_reversal.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/gallery/transformations/plot_refractory_period.py` & `tonic-1.2.8.dev4/docs/gallery/transformations/plot_refractory_period.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/gallery/transformations/plot_spatial_jitter.py` & `tonic-1.2.8.dev4/docs/gallery/transformations/plot_spatial_jitter.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/gallery/transformations/plot_time_jitter.py` & `tonic-1.2.8.dev4/docs/gallery/transformations/plot_time_jitter.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/gallery/transformations/plot_uniform_noise.py` & `tonic-1.2.8.dev4/docs/gallery/transformations/plot_uniform_noise.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/getting_involved/communication_channels.rst` & `tonic-1.2.8.dev4/docs/getting_involved/communication_channels.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/getting_involved/contribute.rst` & `tonic-1.2.8.dev4/docs/getting_involved/contribute.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/getting_started/install.rst` & `tonic-1.2.8.dev4/docs/getting_started/install.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/getting_started/nmnist.ipynb` & `tonic-1.2.8.dev4/docs/getting_started/nmnist.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/how-tos/loading-raw-events.ipynb` & `tonic-1.2.8.dev4/docs/how-tos/loading-raw-events.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/how-tos/visualizing-data.ipynb` & `tonic-1.2.8.dev4/docs/how-tos/visualizing-data.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/how-tos/wrapping_own_data.ipynb` & `tonic-1.2.8.dev4/docs/how-tos/wrapping_own_data.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/index.md` & `tonic-1.2.8.dev4/docs/index.md`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/make.bat` & `tonic-1.2.8.dev4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/reading_material/design_choices.rst` & `tonic-1.2.8.dev4/docs/reading_material/design_choices.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/reading_material/intro-event-cameras.rst` & `tonic-1.2.8.dev4/docs/reading_material/intro-event-cameras.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/reading_material/intro-snns.rst` & `tonic-1.2.8.dev4/docs/reading_material/intro-snns.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/reading_material/training-snns.rst` & `tonic-1.2.8.dev4/docs/reading_material/training-snns.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Links to SNN training frameworks
 ================================
 
 Tonic takes care of providing you with the right data in the right format. In order to train your spiking neural network, we refer the reader to a list of simulators in alphabetical order:
 
 * `BindsNet <https://github.com/BindsNET/bindsnet>`_
 * `Norse documentation <https://norse.github.io/norse/>`_ and `tutorial using Tonic and Norse <https://github.com/norse/notebooks/blob/master/poker-dvs_classifier.ipynb>`_.
-* `Rockpool <https://rockpool.ai/>`_
+* `Rockpool <https://rockpool.ai/>`_ and a `tutorial for audio classification <https://rockpool.ai/tutorials/rockpool-shd.html>`_.
 * `Sinabs <https://sinabs.ai/>`_
 * `snnTorch documentation <https://snntorch.readthedocs.io/>`_ and `tutorial using Tonic and snnTorch <https://snntorch.readthedocs.io/en/latest/tutorials/tutorial_7.html>`_.
```

### Comparing `tonic-1.2.7.dev9/docs/transformations.rst` & `tonic-1.2.8.dev4/docs/transformations.rst`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/tutorials/batching.ipynb` & `tonic-1.2.8.dev4/docs/tutorials/batching.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/tutorials/davis_data.ipynb` & `tonic-1.2.8.dev4/docs/tutorials/davis_data.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/tutorials/fast_dataloading.ipynb` & `tonic-1.2.8.dev4/docs/tutorials/fast_dataloading.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/tutorials/large_datasets.ipynb` & `tonic-1.2.8.dev4/docs/tutorials/large_datasets.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/docs/tutorials/slicing.ipynb` & `tonic-1.2.8.dev4/docs/tutorials/slicing.ipynb`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/setup.cfg` & `tonic-1.2.8.dev4/setup.cfg`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/test/dataset_utils.py` & `tonic-1.2.8.dev4/test/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/test/prototype_dataset_utils.py` & `tonic-1.2.8.dev4/test/prototype_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/test/test_audio_transforms.py` & `tonic-1.2.8.dev4/test/test_audio_transforms.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/test/test_caching.py` & `tonic-1.2.8.dev4/test/test_caching.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/test/test_chained_transforms.py` & `tonic-1.2.8.dev4/test/test_chained_transforms.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/test/test_data/sample.aedat4` & `tonic-1.2.8.dev4/test/test_data/sample.aedat4`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/test/test_data/sample_ncars.dat` & `tonic-1.2.8.dev4/test/test_data/sample_ncars.dat`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/test/test_data/sample_nmnist.bin` & `tonic-1.2.8.dev4/test/test_data/sample_nmnist.bin`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/test/test_data/sample_stmnist.mat` & `tonic-1.2.8.dev4/test/test_data/sample_stmnist.mat`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/test/test_datasets.py` & `tonic-1.2.8.dev4/test/test_datasets.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 import h5py
 import numpy as np
 from utils import create_random_input
 
 import tonic.datasets as datasets
 from tonic.download_utils import download_url
 
-base_url = "https://www.neuromorphic-vision.com/public/downloads/dataset_samples/"
+base_url = "https://nextcloud.lenzgregor.com/s/"
 
 
 class ASLDVSTestCaseTest(dataset_utils.DatasetTestCase):
     DATASET_CLASS = datasets.ASLDVS
     FEATURE_TYPES = (datasets.ASLDVS.dtype,)
     TARGET_TYPES = (int,)
     KWARGS = {}
 
     def inject_fake_data(self, tmpdir):
         testfolder = os.path.join(tmpdir, "ASLDVS/a")
         os.makedirs(testfolder, exist_ok=True)
-        filename = "a_0244.mat"
-        download_url(url=base_url + filename, root=testfolder, filename=filename)
+        filename = "2aeALcfARAS8Dkf/download/a_0244.mat"
+        download_url(url=base_url + filename, root=testfolder, filename="a_0244.mat")
         return {"n_samples": 1}
 
 
 class DVSGestureTestCaseTrain(dataset_utils.DatasetTestCase):
     DATASET_CLASS = datasets.DVSGesture
     FEATURE_TYPES = (datasets.DVSGesture.dtype,)
     TARGET_TYPES = (int,)
@@ -95,57 +95,61 @@
     TARGET_TYPES = (int,)
     KWARGS = {}
 
     def inject_fake_data(self, tmpdir):
         testfolder = os.path.join(tmpdir, "NCALTECH101/Caltech101/airplanes/")
         os.makedirs(testfolder, exist_ok=True)
         filename = "image_0006.bin"
-        download_url(url=base_url + filename, root=testfolder, filename=filename)
+        url = base_url + "sGTckK5fgit7QH3/download/" + filename
+        download_url(url=url, root=testfolder, filename=filename)
         return {"n_samples": 1}
 
 
 class NMNISTTestCaseTrain(dataset_utils.DatasetTestCase):
     DATASET_CLASS = datasets.NMNIST
     FEATURE_TYPES = (datasets.NMNIST.dtype,)
     TARGET_TYPES = (int,)
     KWARGS = {"train": True}
 
     def inject_fake_data(self, tmpdir):
         testfolder = os.path.join(tmpdir, "NMNIST/Train/1/")
         os.makedirs(testfolder, exist_ok=True)
-        filename = "image_0006.bin"
-        download_url(url=base_url + filename, root=testfolder, filename="24901.bin")
+        filename = "00015.bin"
+        url = base_url + "pi6WkPbg6tgd7ca/download/" + filename
+        download_url(url=url, root=testfolder, filename=filename)
         return {"n_samples": 1}
 
 
 class NMNISTTestCaseTest(dataset_utils.DatasetTestCase):
     DATASET_CLASS = datasets.NMNIST
     FEATURE_TYPES = (datasets.NMNIST.dtype,)
     TARGET_TYPES = (int,)
     KWARGS = {"train": False}
 
     def inject_fake_data(self, tmpdir):
         testfolder = os.path.join(tmpdir, "NMNIST/Test/1/")
         os.makedirs(testfolder, exist_ok=True)
-        filename = "image_0006.bin"
-        download_url(url=base_url + filename, root=testfolder, filename="04652.bin")
+        filename = "00015.bin"
+        url = base_url + "pi6WkPbg6tgd7ca/download/" + filename
+        download_url(url=url, root=testfolder, filename=filename)
         return {"n_samples": 1}
 
 
 def create_hsd_data(filename, n_samples):
     with h5py.File(filename, mode="w") as write_file:
         times = np.random.random(size=(n_samples, 100)).astype(np.float16)
         units = (np.random.random(size=(n_samples, 100)) * 700).astype(np.uint16)
         keys = ["zero", "one"]
-        speaker= (np.random.random(size=n_samples) * 20).astype(np.uint16)
+        speaker = (np.random.random(size=n_samples) * 20).astype(np.uint16)
         write_file.create_dataset("spikes/units", data=units)
         write_file.create_dataset("spikes/times", data=times)
         write_file.create_dataset("labels", data=[1] * n_samples)
         write_file.create_dataset("extra/keys", data=keys)
-        write_file.create_dataset("extra/speaker", data= speaker)
+        write_file.create_dataset("extra/speaker", data=speaker)
+
 
 class SHDTestCaseTrain(dataset_utils.DatasetTestCase):
     DATASET_CLASS = datasets.SHD
     FEATURE_TYPES = (datasets.SHD.dtype,)
     TARGET_TYPES = (int,)
     KWARGS = {"train": True}
```

### Comparing `tonic-1.2.7.dev9/test/test_dsec.py` & `tonic-1.2.8.dev4/test/test_dsec.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/test/test_io.py` & `tonic-1.2.8.dev4/test/test_io.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/test/test_prototype_datasets.py` & `tonic-1.2.8.dev4/test/test_prototype_datasets.py`

 * *Files 19% similar despite different names*

```diff
@@ -246,7 +246,57 @@
     TARGET_TYPES = (np.array,)
     KWARGS = {"split": "test"}
 
     def inject_fake_data(self, tmpdir):
         create_minidataset_folder(
             tmpdir, datasets.Gen4AutomotiveDetectionMini._TEST_FOLDER
         )
+
+
+#########################
+# Gen1AutomotiveDetection
+#########################
+
+
+def create_gen1dataset_folder(tmpdir, split_folder):
+    testfolder = Path(tmpdir, "detection_dataset_duration_60s_ratio_1.0", split_folder)
+    testfolder.mkdir(parents=True, exist_ok=True)
+    shutil.copyfile(
+        PATH_TO_TEST_DATA / "sample_ncars.dat",
+        Path(testfolder, "moorea_2019-02-19_004_td_610500000_670500000_td.dat"),
+    )
+    label = np.array([0.4, 0.2, 0.1, 0.1])
+    np.save(testfolder / "moorea_2019-02-19_004_td_610500000_670500000_bbox.npy", label)
+
+
+class Gen1AutomotiveDetectionTestCase_Train(dataset_utils.DatasetTestCase):
+    DATASET_CLASS = datasets.Gen1AutomotiveDetection
+    FEATURE_TYPES = (datasets.Gen1AutomotiveDetection._DTYPE,)
+    TARGET_TYPES = (np.array,)
+    KWARGS = {"split": "train"}
+
+    def inject_fake_data(self, tmpdir):
+        create_gen1dataset_folder(
+            tmpdir, datasets.Gen1AutomotiveDetection._TRAIN_FOLDER
+        )
+
+
+class Gen1AutomotiveDetectionTestCase_Valid(dataset_utils.DatasetTestCase):
+    DATASET_CLASS = datasets.Gen1AutomotiveDetection
+    FEATURE_TYPES = (datasets.Gen1AutomotiveDetection._DTYPE,)
+    TARGET_TYPES = (np.array,)
+    KWARGS = {"split": "valid"}
+
+    def inject_fake_data(self, tmpdir):
+        create_gen1dataset_folder(
+            tmpdir, datasets.Gen1AutomotiveDetection._VALID_FOLDER
+        )
+
+
+class Gen1AutomotiveDetectionTestCase_Test(dataset_utils.DatasetTestCase):
+    DATASET_CLASS = datasets.Gen1AutomotiveDetection
+    FEATURE_TYPES = (datasets.Gen1AutomotiveDetection._DTYPE,)
+    TARGET_TYPES = (np.array,)
+    KWARGS = {"split": "test"}
+
+    def inject_fake_data(self, tmpdir):
+        create_gen1dataset_folder(tmpdir, datasets.Gen1AutomotiveDetection._TEST_FOLDER)
```

### Comparing `tonic-1.2.7.dev9/test/test_representations.py` & `tonic-1.2.8.dev4/test/test_representations.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,14 +169,22 @@
     sensor_size = (20, 10, 2)
     orig_events, _ = create_random_input(n_events=30000, sensor_size=sensor_size)
     transform = transforms.ToFrame(sensor_size=None, time_window=25000)
     frames = transform(orig_events)
     assert frames.shape[1:] == sensor_size[::-1]
 
 
+def test_representation_frame_wrong_sensor_size():
+    sensor_size = (20, 10, 2)
+    orig_events, _ = create_random_input(n_events=30000, sensor_size=sensor_size)
+    transform = transforms.ToFrame(sensor_size=(20, 10, 1), time_window=25000)
+    with pytest.raises(ValueError):
+        frames = transform(orig_events)
+
+
 def test_representation_audio_frame():
     sensor_size = (200, 1, 2)
     orig_events, _ = create_random_input(
         sensor_size=sensor_size,
         dtype=np.dtype([("x", int), ("t", int), ("p", int)]),
     )
     transform = transforms.ToFrame(sensor_size=sensor_size, time_window=25000)
@@ -189,26 +197,31 @@
     orig_events, _ = create_random_input(n_events=10000, sensor_size=sensor_size)
     transform = transforms.ToImage(sensor_size=sensor_size)
     image = transform(orig_events)
     assert image.shape == sensor_size[::-1]
 
 
 @pytest.mark.parametrize(
-    "surface_dimensions, tau,", [((15, 15), 100), ((3, 3), 10), (None, 1e4)]
+    "surface_dimensions, tau, delta_t", [((15, 15), 100, 0), ((3, 3), 10, 1e4), (None, 1e4, 1e5)]
 )
-def test_representation_time_surface(surface_dimensions, tau):
+def test_representation_time_surface(surface_dimensions, tau, delta_t):
     orig_events, sensor_size = create_random_input(n_events=1000)
 
     transform = transforms.ToTimesurface(
-        sensor_size=sensor_size, surface_dimensions=surface_dimensions, tau=tau
+        sensor_size=sensor_size, surface_dimensions=surface_dimensions, tau=tau, delta_t=delta_t
     )
 
     surfaces = transform(orig_events)
 
-    assert surfaces.shape[0] == len(orig_events)
+    if delta_t == 0:
+        assert surfaces.shape[0] == len(orig_events)
+    else:
+        duration = orig_events["t"][-1] - orig_events["t"][0]
+        assert surfaces.shape[0] == duration // delta_t 
+        
     assert surfaces.shape[1] == 2
     if surface_dimensions:
         assert surfaces.shape[2:] == surface_dimensions
     else:
         assert surfaces.shape[2] == sensor_size[1]
         assert surfaces.shape[3] == sensor_size[0]
     assert surfaces is not orig_events
```

### Comparing `tonic-1.2.7.dev9/test/test_sliced_dataset.py` & `tonic-1.2.8.dev4/test/test_sliced_dataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/test/test_slicers.py` & `tonic-1.2.8.dev4/test/test_slicers.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/test/test_tonic_utils.py` & `tonic-1.2.8.dev4/test/test_tonic_utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/test/test_transforms.py` & `tonic-1.2.8.dev4/test/test_transforms.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/test/utils.py` & `tonic-1.2.8.dev4/test/utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/tonic/audio_transforms.py` & `tonic-1.2.8.dev4/tonic/audio_transforms.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/tonic/cached_dataset.py` & `tonic-1.2.8.dev4/tonic/cached_dataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/tonic/collation.py` & `tonic-1.2.8.dev4/tonic/collation.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/tonic/dataset.py` & `tonic-1.2.8.dev4/tonic/dataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/tonic/datasets/__init__.py` & `tonic-1.2.8.dev4/tonic/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/tonic/datasets/asl_dvs.py` & `tonic-1.2.8.dev4/tonic/datasets/asl_dvs.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/tonic/datasets/cifar10dvs.py` & `tonic-1.2.8.dev4/tonic/datasets/cifar10dvs.py`

 * *Files 7% similar despite different names*

```diff
@@ -50,55 +50,53 @@
     folder_name = ""
     dtype = np.dtype(
         [("t", np.uint64), ("x", np.uint16), ("y", np.uint16), ("p", bool)]
     )
     ordering = dtype.names
     sensor_size = (128, 128, 2)
 
+    classes = {
+        "airplane": 0,
+        "automobile": 1,
+        "bird": 2,
+        "cat": 3,
+        "deer": 4,
+        "dog": 5,
+        "frog": 6,
+        "horse": 7,
+        "ship": 8,
+        "truck": 9,
+    }
+
     def __init__(
         self,
         save_to: str,
         transform: Optional[Callable] = None,
         target_transform: Optional[Callable] = None,
         transforms: Optional[Callable] = None,
     ):
         super().__init__(
             save_to,
             transform=transform,
             target_transform=target_transform,
             transforms=transforms,
         )
 
-        # classes for CIFAR10DVS dataset
-
-        classes = {
-            "airplane": 0,
-            "automobile": 1,
-            "bird": 2,
-            "cat": 3,
-            "deer": 4,
-            "dog": 5,
-            "frog": 6,
-            "horse": 7,
-            "ship": 8,
-            "truck": 9,
-        }
-
         if not self._check_exists():
             self.download()
             for filename in self.data_filename:
                 extract_archive(os.path.join(self.location_on_system, filename))
 
         file_path = os.path.join(self.location_on_system, self.folder_name)
         for path, dirs, files in os.walk(file_path):
             dirs.sort()
             for file in files:
                 if file.endswith("aedat4"):
                     self.data.append(os.path.join(path, file))
-                    label_number = classes[os.path.basename(path)]
+                    label_number = self.classes[os.path.basename(path)]
                     self.targets.append(label_number)
 
     def __getitem__(self, index):
         """
         Returns:
             a tuple of (events, target) where target is the index of the target class.
         """
```

### Comparing `tonic-1.2.7.dev9/tonic/datasets/davisdataset.py` & `tonic-1.2.8.dev4/tonic/datasets/davisdataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/tonic/datasets/dsec.py` & `tonic-1.2.8.dev4/tonic/datasets/dsec.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/tonic/datasets/dvs_lips.py` & `tonic-1.2.8.dev4/tonic/datasets/dvs_lips.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/tonic/datasets/dvsgesture.py` & `tonic-1.2.8.dev4/tonic/datasets/dvsgesture.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/tonic/datasets/hsd.py` & `tonic-1.2.8.dev4/tonic/datasets/hsd.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,15 @@
         self.classes = file["extra/keys"][()]
         self._speaker = file["extra/speaker"][()]
 
     @property
     def speaker(self):
         return self._speaker[()]
 
+
 class SSC(HSD):
     """`Spiking Speech Commands <https://zenkelab.org/resources/spiking-heidelberg-datasets-shd/>`_
     ::
 
         @article{cramer2020heidelberg,
           title={The heidelberg spiking data sets for the systematic evaluation of spiking neural networks},
           author={Cramer, Benjamin and Stradmann, Yannik and Schemmel, Johannes and Zenke, Friedemann},
@@ -162,7 +163,8 @@
         self.data_filename = self.filename[:-4]
 
         if not self._check_exists():
             self.download()
 
         file = h5py.File(os.path.join(self.location_on_system, self.data_filename), "r")
         self.classes = file["extra/keys"][()]
+        self._speaker = file["extra/speaker"][()]
```

### Comparing `tonic-1.2.7.dev9/tonic/datasets/mvsec.py` & `tonic-1.2.8.dev4/tonic/datasets/mvsec.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/tonic/datasets/ncaltech101.py` & `tonic-1.2.8.dev4/tonic/datasets/ncaltech101.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/tonic/datasets/nmnist.py` & `tonic-1.2.8.dev4/tonic/datasets/nmnist.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/tonic/datasets/pokerdvs.py` & `tonic-1.2.8.dev4/tonic/datasets/pokerdvs.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,19 +27,19 @@
         train (bool): If True, uses training subset, otherwise testing subset.
         transform (callable, optional): A callable of transforms to apply to the data.
         target_transform (callable, optional): A callable of transforms to apply to the targets/labels.
         transforms (callable, optional): A callable of transforms that is applied to both data and
                                          labels at the same time.
     """
 
-    base_url = "https://www.neuromorphic-vision.com/public/downloads/"
+    base_url = "https://nextcloud.lenzgregor.com/s/"
     train_filename = "pips_train.tar.gz"
     test_filename = "pips_test.tar.gz"
-    train_url = base_url + train_filename
-    test_url = base_url + test_filename
+    train_url = base_url + "ZeCPYBS8kx4Wyjd/download/" + train_filename
+    test_url = base_url + "2iRfwg3y9eAMpGL/download/" + test_filename
     train_md5 = "412bcfb96826e4fcb290558e8c150aae"
     test_md5 = "eef2bf7d0d3defae89a6fa98b07c17af"
 
     classes = ["cl", "he", "di", "sp"]
     int_classes = dict(zip(classes, range(4)))
     sensor_size = (35, 35, 2)
     dtype = np.dtype([("t", int), ("x", int), ("y", int), ("p", int)])
```

### Comparing `tonic-1.2.7.dev9/tonic/datasets/s_mnist.py` & `tonic-1.2.8.dev4/tonic/datasets/s_mnist.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/tonic/datasets/tum_vie.py` & `tonic-1.2.8.dev4/tonic/datasets/tum_vie.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/tonic/datasets/visual_place_recognition.py` & `tonic-1.2.8.dev4/tonic/datasets/visual_place_recognition.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/tonic/download_utils.py` & `tonic-1.2.8.dev4/tonic/download_utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/tonic/functional/__init__.py` & `tonic-1.2.8.dev4/tonic/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/tonic/functional/crop.py` & `tonic-1.2.8.dev4/tonic/functional/crop.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/tonic/functional/decimate.py` & `tonic-1.2.8.dev4/tonic/functional/decimate.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/tonic/functional/denoise.py` & `tonic-1.2.8.dev4/tonic/functional/denoise.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/tonic/functional/drop_event.py` & `tonic-1.2.8.dev4/tonic/functional/drop_event.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/tonic/functional/drop_pixel.py` & `tonic-1.2.8.dev4/tonic/functional/drop_pixel.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/tonic/functional/refractory_period.py` & `tonic-1.2.8.dev4/tonic/functional/refractory_period.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/tonic/functional/spatial_jitter.py` & `tonic-1.2.8.dev4/tonic/functional/spatial_jitter.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/tonic/functional/time_jitter.py` & `tonic-1.2.8.dev4/tonic/functional/time_jitter.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/tonic/functional/time_skew.py` & `tonic-1.2.8.dev4/tonic/functional/time_skew.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/tonic/functional/to_averaged_timesurface.py` & `tonic-1.2.8.dev4/tonic/functional/to_averaged_timesurface.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/tonic/functional/to_bina_rep.py` & `tonic-1.2.8.dev4/tonic/functional/to_bina_rep.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/tonic/functional/to_frame.py` & `tonic-1.2.8.dev4/tonic/functional/to_frame.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,14 +55,18 @@
             sensor_size_y = int(events["y"].max() + 1)
             sensor_size = (sensor_size_x, sensor_size_y, sensor_size_p)
         else:
             sensor_size = (sensor_size_x, 1, sensor_size_p)
 
     # test for single polarity
     if sensor_size[2] == 1:
+        if np.unique(events["p"]).size > 1:
+            raise ValueError(
+                "Single polarity sensor, but events contain both polarities."
+            )
         events["p"] = 0
 
     if time_window:
         event_slices = slice_events_by_time(
             events, time_window, overlap=overlap, include_incomplete=include_incomplete
         )
     elif event_count:
```

### Comparing `tonic-1.2.7.dev9/tonic/functional/to_voxel_grid.py` & `tonic-1.2.8.dev4/tonic/functional/to_voxel_grid.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/tonic/functional/uniform_noise.py` & `tonic-1.2.8.dev4/tonic/functional/uniform_noise.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/tonic/io.py` & `tonic-1.2.8.dev4/tonic/io.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/tonic/prototype/README.md` & `tonic-1.2.8.dev4/tonic/prototype/README.md`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/tonic/prototype/datasets/ncars.py` & `tonic-1.2.8.dev4/tonic/prototype/datasets/ncars.py`

 * *Files 19% similar despite different names*

```diff
@@ -46,39 +46,30 @@
           month = {June},
           year = {2018}
         }
 
     Parameters:
         root (string): Location to decompressed archive.
         train (bool): If True, uses training subset, otherwise testing subset.
-        transform (callable, optional): A callable of transforms to apply to the data.
-        target_transform (callable, optional): A callable of transforms to apply to the targets/labels.
-        transforms (callable, optional): A callable of transforms that is applied to both data and labels at the same time.
     """
 
     _DTYPE = event_t
     _TRAIN_PATH = "n-cars_train"
     _TEST_PATH = "n-cars_test"
-    sensor_size = (120, 100, 2)
+    sensor_size = dict(x=120, y=100, p=2)
 
     def __init__(
         self,
         root: os.PathLike,
-        transform: Optional[Callable] = None,
-        target_transform: Optional[Callable] = None,
-        transforms: Optional[Callable] = None,
         train: Optional[bool] = True,
         skip_sha256_check: Optional[bool] = True,
     ) -> None:
         self.train = train
         super().__init__(
             Path(root, self.__class__.__name__),
-            transform,
-            target_transform,
-            transforms,
             False,
             skip_sha256_check,
         )
         assert (
             self._check_exists()
         ), "Error: the dataset files could not be found. You should download the dataset and manually extract it and, then, provide the path to the extracted archive as root."
```

### Comparing `tonic-1.2.7.dev9/tonic/prototype/datasets/nmnist.py` & `tonic-1.2.8.dev4/tonic/prototype/datasets/nmnist.py`

 * *Files 8% similar despite different names*

```diff
@@ -89,29 +89,23 @@
     _TEST_SHA256 = "6ecfd5d85dbb49a631961d8dc3101871c5be53e645004ee34064f6557d169f09"
     _TEST_FOLDER = "Test"
     sensor_size = (34, 34, 2)
 
     def __init__(
         self,
         root: os.PathLike,
-        transform: Optional[Callable] = None,
-        target_transform: Optional[Callable] = None,
-        transforms: Optional[Callable] = None,
         train: Optional[bool] = True,
         first_saccade_only: Optional[bool] = False,
         keep_compressed: Optional[bool] = False,
         skip_sha256_check: Optional[bool] = True,
     ) -> None:
         self.train = train
         self.first_saccade_only = first_saccade_only
         super().__init__(
             root=Path(root, self.__class__.__name__),
-            transform=transform,
-            target_transform=target_transform,
-            transforms=transforms,
             keep_compressed=keep_compressed,
             skip_sha256_check=skip_sha256_check,
         )
         self._download()
 
     def __len__(self) -> int:
         return 60_000 if self.train else 10_000
@@ -142,14 +136,15 @@
         self, dp: IterDataPipe[Tuple[Any, BinaryIO]]
     ) -> IterDataPipe[Tuple[str, BinaryIO]]:
         folder = self._TRAIN_FOLDER if self.train else self._TEST_FOLDER
         # Joining root with a folder to contain the data.
         filepath = os.path.join(self._root, folder)
         if (not os.path.isdir(filepath)) or (not os.listdir(filepath)):
             os.makedirs(filepath, exist_ok=True)
+
             # Decompressing in root.
             def read_bin(fdata):
                 return fdata.read()
 
             dp = Mapper(dp, read_bin, input_col=1)
 
             def filepath_fn(fpath):
```

### Comparing `tonic-1.2.7.dev9/tonic/prototype/datasets/stmnist.py` & `tonic-1.2.8.dev4/tonic/prototype/datasets/stmnist.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,30 +84,24 @@
 
     Returns:
         dp (IterDataPipe[Sample]): Torchdata data pipe that yields a tuple of events (or transformed events) and target.
     """
 
     _DTYPE = np.dtype([("x", int), ("y", int), ("t", int), ("p", int)])
     _SHA256 = "825bb5a64753fff4a2a2c32e3497fa8a951d9c94993e03ba25a057e17d83b884"
-    sensor_size = (10, 10, 2)
+    sensor_size = dict(x=10, y=10, p=2)
 
     def __init__(
         self,
         root: os.PathLike,
-        transform: Optional[Callable] = None,
-        target_transform: Optional[Callable] = None,
-        transforms: Optional[Callable] = None,
         keep_compressed: Optional[bool] = False,
         skip_sha256_check: Optional[bool] = True,
     ) -> None:
         super().__init__(
             Path(root, self.__class__.__name__),
-            transform,
-            target_transform,
-            transforms,
             keep_compressed,
             skip_sha256_check,
         )
         assert self._check_exists(), "Error: the archive is not present."
         if not self.skip_sha256:
             check_sha256(fpath=self._root, sha256_provided=self._SHA256)
 
@@ -125,14 +119,15 @@
     ) -> IterDataPipe[Tuple[str, BinaryIO]]:
         # Stripping the archive from self._root.
         root = os.sep.join(str(self._root).split(os.sep)[:-1])
         # Joining root with a folder to contain the data.
         root = os.path.join(root, "data_uncompressed")
         if not os.path.isdir(root):
             os.mkdir(root)
+
             # Decompressing in root.
             def read_bin(fdata):
                 return fdata.read()
 
             def filepath_fn(fpath):
                 fpath_i = fpath.split(os.sep)
                 start = fpath_i.index("data_submission") + len(os.sep)
```

### Comparing `tonic-1.2.7.dev9/tonic/prototype/datasets/utils/_dataset.py` & `tonic-1.2.8.dev4/tonic/prototype/datasets/utils/_dataset.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,17 +9,14 @@
 Sample = Tuple[np.ndarray, Any]
 
 
 class Dataset(IterDataPipe[Sample], abc.ABC):
     def __init__(
         self,
         root: Union[str, pathlib.Path],
-        transform: Optional[Callable] = None,
-        target_transform: Optional[Callable] = None,
-        transforms: Optional[Callable] = None,
         keep_compressed: Optional[bool] = False,
         skip_sha256_check: Optional[bool] = True,
         dependencies: Optional[Collection[str]] = (),
     ) -> None:
         # Code for importing dependencies. Useful if one wants to
         # use proprietary data format!
         for dependency in dependencies:
@@ -28,40 +25,29 @@
             except ModuleNotFoundError:
                 raise ModuleNotFoundError(
                     f"{type(self).__name__}() depends on third-party package '{dependency}'",
                     f"Please, install it.",
                 ) from None
         # Getting in root path.
         self._root = pathlib.Path(root).expanduser().resolve()
-        # Getting trasforms.
-        self.transform = transform
-        self.target_transform = target_transform
-        self.transforms = transforms
         # SHA256 skipping if the file has been already downloaded.
         self.skip_sha256 = skip_sha256_check
         # Flag to keep the archive compressed.
         self.keep_cmp = keep_compressed
         # Resource line, like...?
         resources = None
         # The datapipe.
         self._dp = self._datapipe_wrapper()
 
     def __iter__(self) -> Iterator[Sample]:
         """Iteration method for the data pipe."""
         yield from self._dp
 
     def _datapipe_wrapper(self):
-        dp = self._datapipe()
-        if self.transforms:
-            dp = Mapper(dp, self.transforms)
-        if self.transform:
-            dp = Mapper(dp, self.transform, input_col=0)
-        if self.target_transform:
-            dp = Mapper(dp, self.target_transform, input_col=1)
-        return dp
+        return self._datapipe()
 
     @abc.abstractmethod
     def _check_exists(self):
         pass
 
     @abc.abstractmethod
     def _datapipe(self):
```

### Comparing `tonic-1.2.7.dev9/tonic/prototype/datasets/utils/_utils.py` & `tonic-1.2.8.dev4/tonic/prototype/datasets/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/tonic/prototype/slicers.py` & `tonic-1.2.8.dev4/tonic/prototype/slicers.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/tonic/sliced_dataset.py` & `tonic-1.2.8.dev4/tonic/sliced_dataset.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/tonic/slicers.py` & `tonic-1.2.8.dev4/tonic/slicers.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/tonic/transforms.py` & `tonic-1.2.8.dev4/tonic/transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -912,29 +912,33 @@
     https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=7508476.
 
     Parameters:
         sensor_size: a 3-tuple of x,y,p for sensor_size
         surface_dimensions (int, int): width does not have to be equal to height, however both numbers have to be odd.
             if surface_dimensions is None: the time surface is defined globally, on the whole sensor grid.
         tau (float): time constant to decay events around occuring event with.
+        delta_t (float): the interval at which the time-surfaces are accumulated, if set 0 number of time-surfaces will
+            equal to the number of events. (defaults to 0.0) 
         decay (str): can be either 'lin' or 'exp', corresponding to linear or exponential decay.
     """
 
     sensor_size: Tuple[int, int, int]
     surface_dimensions: Union[None, Tuple[int, int]] = None
     tau: float = 5e3
+    delta_t: float = 0.0
     decay: str = "lin"
 
     def __call__(self, events):
 
         return functional.to_timesurface_numpy(
             events=events,
             sensor_size=self.sensor_size,
             surface_dimensions=self.surface_dimensions,
             tau=self.tau,
+            delta_t=self.delta_t,
             decay=self.decay,
         )
 
 
 @dataclass(frozen=True)
 class ToVoxelGrid:
     """Build a voxel grid with bilinear interpolation in the time domain from a set of events.
```

### Comparing `tonic-1.2.7.dev9/tonic/utils.py` & `tonic-1.2.8.dev4/tonic/utils.py`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/tonic-logo-padded.png` & `tonic-1.2.8.dev4/tonic-logo-padded.png`

 * *Files identical despite different names*

### Comparing `tonic-1.2.7.dev9/tonic.egg-info/PKG-INFO` & `tonic-1.2.8.dev4/tonic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonic
-Version: 1.2.7.dev9
+Version: 1.2.8.dev4
 Summary: Neuromorphic datasets and transformations.
 Home-page: UNKNOWN
 Author: The Neuromorphs of Telluride
 Author-email: mail@lenzgregor.com
 License: GNU GPLv3
 Project-URL: Source code, https://github.com/neuromorphs/tonic
 Project-URL: Documentation, https://tonic.readthedocs.org
```

### Comparing `tonic-1.2.7.dev9/tonic.egg-info/SOURCES.txt` & `tonic-1.2.8.dev4/tonic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

